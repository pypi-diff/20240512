# Comparing `tmp/bundle_cpp-0.1.1.tar.gz` & `tmp/bundle_cpp-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bundle_cpp-0.1.1.tar", max compression
+gzip compressed data, was "bundle_cpp-0.1.2.tar", max compression
```

## Comparing `bundle_cpp-0.1.1.tar` & `bundle_cpp-0.1.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      418 2024-05-11 01:07:09.583472 bundle_cpp-0.1.1/README.md
--rw-r--r--   0        0        0     2291 2024-05-10 23:54:31.667449 bundle_cpp-0.1.1/bundle_cpp/__init__.py
--rw-r--r--   0        0        0     1856 2024-05-10 22:28:57.529469 bundle_cpp-0.1.1/bundle_cpp/__main__.py
--rw-r--r--   0        0        0     1168 2024-05-11 01:08:05.584500 bundle_cpp-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1008 1970-01-01 00:00:00.000000 bundle_cpp-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      418 2024-05-12 09:32:09.611817 bundle_cpp-0.1.2/README.md
+-rw-r--r--   0        0        0     2785 2024-05-12 11:18:14.371601 bundle_cpp-0.1.2/bundle_cpp/__init__.py
+-rw-r--r--   0        0        0     1783 2024-05-12 11:10:06.231835 bundle_cpp-0.1.2/bundle_cpp/__main__.py
+-rw-r--r--   0        0        0     1168 2024-05-12 11:20:31.045388 bundle_cpp-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1008 1970-01-01 00:00:00.000000 bundle_cpp-0.1.2/PKG-INFO
```

### Comparing `bundle_cpp-0.1.1/bundle_cpp/__init__.py` & `bundle_cpp-0.1.2/bundle_cpp/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 from typing import List
 from pathlib import Path
 from typing import Optional as Opt
 import re
+import os
+
+WD = Path(os.getcwd())
 
 
 def _read(p: Path) -> List[str]:
     with p.open() as f:
         return f.readlines()
 
 
 def bundle(
     src: Path,
     include_paths: List[Path] = None,
+    add_line=False,
+    # relpath = True,
 ) -> str:
     if include_paths is None:
         include_paths = []
 
     is_once = set()
     edges = set()
 
@@ -55,33 +60,45 @@
             line: str,
         ) -> bool:
             ptn = r"^\s*#\s*pragma\s+once\s*\n$"
             return re.match(ptn, line) is not None
 
         lines = _read(file)
         result_lines = []
-        for l in lines:
+        al = True
+        for i, l in enumerate(lines):
             if is_pragma_once(l):
                 is_once.add(file)
+                al = True
                 continue
             dep = included_file(l)
             if dep is None:
+                if al and add_line:
+                    f = file
+                    # if relpath:
+                    #     f.relative_to(WD, walk_up=True)
+                    result_lines.append(
+                        f'#line {i + 1} "{f}"\n'
+                    )
+                    al = False
                 result_lines.append(l)
                 continue
             if dep in is_once:
+                al = True
                 continue
             e = (file, dep)
             if e in edges:
                 raise "circular includes"
             edges.add(e)
             result_lines.append(expand(dep))
+            al = True
             edges.remove(e)
 
-        result_lines.reverse()
-        while result_lines:
-            if result_lines[-1] != "\n":
-                break
-            result_lines.pop()
-        result_lines.reverse()
+        # result_lines.reverse()
+        # while result_lines:
+        #     if result_lines[-1] != "\n":
+        #         break
+        #     result_lines.pop()
+        # result_lines.reverse()
         return "".join(result_lines)
 
     return expand(src)
```

### Comparing `bundle_cpp-0.1.1/bundle_cpp/__main__.py` & `bundle_cpp-0.1.2/bundle_cpp/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 @dataclass
 class CLIParam:
     src: Path
     include_paths: List[Path] = dataclasses.field(
         default_factory=list
     )
     dst: Opt[Path] = None
+    add_line: bool = False
 
 
 def cli():
     # https://docs.python.org/3/library/argparse.html
     parser = argparse.ArgumentParser()
     parser.add_argument(
         "-I",
@@ -36,42 +37,45 @@
         "-o",
         type=str,
         metavar="out_file",
         # default="generated.cpp",
         dest="dst",
         help="e.g. main_generated.cpp. not set, print stdout.",
     )
+    parser.add_argument(
+        "-l",
+        "--add-line",
+        action="store_true",
+        help='add #line <__LINE__> "<__FILE__>"',
+    )
     g = parser.add_argument_group("required positional")
     g.add_argument(
         "src_file",
         type=str,
         help="e.g. main.cpp",
     )
+
     args = parser.parse_args()
     include_paths = [
         Path(p).resolve() for p in args.include_paths
     ]
     dst = None if args.dst is None else Path(args.dst).resolve()
     args = CLIParam(
         Path(args.src_file).resolve(),
         include_paths,
         dst,
+        add_line=args.add_line,
     )
-    res = bundle(args.src, args.include_paths)[:-1]
+    res = bundle(
+        args.src,
+        args.include_paths,
+        args.add_line,
+    )[:-1]
     if args.dst is None:
         print(res)
         return
     with args.dst.open("w") as f:
         f.write(res)
 
 
 if __name__ == "__main__":
     cli()
-    # f = f"{CFD}/main2.cpp"
-    # paths = [CFD]
-    # print(os.path.abspath("/root/"))
-    # f = f"{CFD}/cycle_include/main.cpp"
-    # f = f"{CFD}/pragma_once/main.cpp"
-    # f = f"{CFD}/twice/main.cpp"
-    # f = f"{CFD}/../../lib/cpp/template_v1.hpp"
-    # print(bundle(f, paths))
-    # print(bundle(f, paths).split('\n'))
```

### Comparing `bundle_cpp-0.1.1/pyproject.toml` & `bundle_cpp-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "bundle-cpp"
-version = "0.1.1"
+version = "0.1.2"
 description = "expand includes and create a single file"
 authors = ["kagemeka <kagemeka1@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "bundle_cpp" }]
 # exclude = ["tests"]
```

### Comparing `bundle_cpp-0.1.1/PKG-INFO` & `bundle_cpp-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bundle-cpp
-Version: 0.1.1
+Version: 0.1.2
 Summary: expand includes and create a single file
 License: MIT
 Author: kagemeka
 Author-email: kagemeka1@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

