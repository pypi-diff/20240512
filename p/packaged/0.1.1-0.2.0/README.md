# Comparing `tmp/packaged-0.1.1.tar.gz` & `tmp/packaged-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "packaged-0.1.1.tar", last modified: Sat May 11 01:07:12 2024, max compression
+gzip compressed data, was "packaged-0.2.0.tar", last modified: Sat May 11 12:37:17 2024, max compression
```

## Comparing `packaged-0.1.1.tar` & `packaged-0.2.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 tusharsadhwani   (501) staff       (20)        0 2024-05-11 01:07:12.427004 packaged-0.1.1/
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)     1072 2024-05-04 21:39:47.000000 packaged-0.1.1/LICENSE
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)     2426 2024-05-11 01:07:12.426928 packaged-0.1.1/PKG-INFO
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)     1267 2024-05-11 01:01:30.000000 packaged-0.1.1/README.md
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)     1254 2024-05-11 01:07:12.427318 packaged-0.1.1/setup.cfg
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)       37 2024-05-09 19:00:34.000000 packaged-0.1.1/setup.py
-drwxr-xr-x   0 tusharsadhwani   (501) staff       (20)        0 2024-05-11 01:07:12.424192 packaged-0.1.1/src/
-drwxr-xr-x   0 tusharsadhwani   (501) staff       (20)        0 2024-05-11 01:07:12.425291 packaged-0.1.1/src/packaged/
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)     4038 2024-05-10 23:59:49.000000 packaged-0.1.1/src/packaged/__init__.py
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)      184 2024-05-04 21:39:47.000000 packaged-0.1.1/src/packaged/__main__.py
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)     1308 2024-05-10 23:59:49.000000 packaged-0.1.1/src/packaged/cli.py
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)       59 2024-05-04 21:39:47.000000 packaged-0.1.1/src/packaged/py.typed
-drwxr-xr-x   0 tusharsadhwani   (501) staff       (20)        0 2024-05-11 01:07:12.426372 packaged-0.1.1/src/packaged.egg-info/
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)     2426 2024-05-11 01:07:12.000000 packaged-0.1.1/src/packaged.egg-info/PKG-INFO
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)      346 2024-05-11 01:07:12.000000 packaged-0.1.1/src/packaged.egg-info/SOURCES.txt
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)        1 2024-05-11 01:07:12.000000 packaged-0.1.1/src/packaged.egg-info/dependency_links.txt
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)       46 2024-05-11 01:07:12.000000 packaged-0.1.1/src/packaged.egg-info/entry_points.txt
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)       64 2024-05-11 01:07:12.000000 packaged-0.1.1/src/packaged.egg-info/requires.txt
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)        9 2024-05-11 01:07:12.000000 packaged-0.1.1/src/packaged.egg-info/top_level.txt
+drwxr-xr-x   0 tusharsadhwani   (501) staff       (20)        0 2024-05-11 12:37:17.871799 packaged-0.2.0/
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)     1072 2024-05-04 21:39:47.000000 packaged-0.2.0/LICENSE
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)     3173 2024-05-11 12:37:17.871720 packaged-0.2.0/PKG-INFO
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)     2014 2024-05-11 12:36:37.000000 packaged-0.2.0/README.md
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)     1254 2024-05-11 12:37:17.872120 packaged-0.2.0/setup.cfg
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)       37 2024-05-09 19:00:34.000000 packaged-0.2.0/setup.py
+drwxr-xr-x   0 tusharsadhwani   (501) staff       (20)        0 2024-05-11 12:37:17.868249 packaged-0.2.0/src/
+drwxr-xr-x   0 tusharsadhwani   (501) staff       (20)        0 2024-05-11 12:37:17.869918 packaged-0.2.0/src/packaged/
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)     4507 2024-05-11 12:34:12.000000 packaged-0.2.0/src/packaged/__init__.py
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)      184 2024-05-04 21:39:47.000000 packaged-0.2.0/src/packaged/__main__.py
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)     1514 2024-05-11 12:33:41.000000 packaged-0.2.0/src/packaged/cli.py
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)       59 2024-05-04 21:39:47.000000 packaged-0.2.0/src/packaged/py.typed
+drwxr-xr-x   0 tusharsadhwani   (501) staff       (20)        0 2024-05-11 12:37:17.871093 packaged-0.2.0/src/packaged.egg-info/
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)     3173 2024-05-11 12:37:17.000000 packaged-0.2.0/src/packaged.egg-info/PKG-INFO
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)      346 2024-05-11 12:37:17.000000 packaged-0.2.0/src/packaged.egg-info/SOURCES.txt
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)        1 2024-05-11 12:37:17.000000 packaged-0.2.0/src/packaged.egg-info/dependency_links.txt
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)       46 2024-05-11 12:37:17.000000 packaged-0.2.0/src/packaged.egg-info/entry_points.txt
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)       64 2024-05-11 12:37:17.000000 packaged-0.2.0/src/packaged.egg-info/requires.txt
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)        9 2024-05-11 12:37:17.000000 packaged-0.2.0/src/packaged.egg-info/top_level.txt
```

### Comparing `packaged-0.1.1/LICENSE` & `packaged-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `packaged-0.1.1/README.md` & `packaged-0.2.0/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -13,47 +13,75 @@
 ```bash
 packaged <source_directory> <output_path> <build_command> <startup_command>
 ```
 
 Such as:
 
 ```bash
-packaged path/to/project my_project.bin 'pip install .' 'python -m your_package'
+packaged my_project.bin 'pip install .' 'python -m your_package' path/to/project
 ```
 
-### Example
+## Examples
 
-There's an `example` folder where you can test this:
+All examples below create a self contained executable. You can send the produced
+binary file to another machine with the same OS and architecture, and it will
+run the same.
+
+### Graphs / matplotlib
 
 ```bash
-packaged ./example/matplotlib ./curve.bin 'pip install -r requirements.txt' 'python bubble_sort_curve.py'
+packaged ./curve.bin 'pip install -r requirements.txt' 'python bubble_sort_curve.py' ./example/matplotlib
 ```
 
 This produces a `./curve.bin` binary with:
 
 - Python 3.11
 - `matplotlib`
 - `numba`
 - `llvmlite`
 - `pillow`
 
-... and is directly executable. You can send this binary file to another machine
-with the same OS and architecture, and it will run the same.
+That outputs an interactive graph GUI.
+
+### Textual Demo
+
+Since the dependencies themselves contain all the source code needed, you can
+skip the last argument. With this, no other files will be packaged other than
+what is produced in the build step.
+
+```bash
+packaged './textualdemo.bin' 'pip install textual' 'python -m textual'
+```
+
+This will simply package the `textual` library's own demo into a single file.
+
+### Chimp game (pygame)
+
+Pygame ships with various games as well, `pygame.examples.chimp` is one of them:
+
+```bash
+packaged './chimp' 'pip install pygame' 'python -m pygame.examples.chimp'
+```
+
+Another fun game that you can try out are `pygame.examples.aliens`.
 
 ## Local Development / Testing
 
+To test and modify the package locally:
+
 - Create and activate a virtual environment
 - Run `pip install -r requirements-dev.txt` to do an editable install
 - Run `pytest` to run tests
+- Make changes as needed
 
-## Type Checking
+### Type Checking
 
 Run `mypy .`
 
-## Create and upload a package to PyPI
+### Create and upload a package to PyPI
 
 Make sure to bump the version in `setup.cfg`.
 
 Then run the following commands:
 
 ```bash
 rm -rf build dist
```

### Comparing `packaged-0.1.1/setup.cfg` & `packaged-0.2.0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = packaged
-version = 0.1.1
+version = 0.2.0
 description = The easiest way to ship python applications.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/tusharsadhwani/packaged
 author = Tushar Sadhwani
 author_email = tushar.sadhwani000@gmail.com
 license = MIT
```

### Comparing `packaged-0.1.1/src/packaged/__init__.py` & `packaged-0.2.0/src/packaged/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """packaged - The easiest way to ship python applications."""
 
 from __future__ import annotations
 
 import os.path
 import shutil
 import subprocess
+import tempfile
 import urllib.request
 
 import yen
 
 
 MAKESELF_VERSION = "2.5.0"
 MAKESELF_DOWNLOAD_URL = (
@@ -17,14 +18,22 @@
 )
 MAKESELF_DOWNLOAD_PATH = os.path.join(os.path.dirname(__file__), ".build_deps")
 MAKESELF_PATH = os.path.join(
     MAKESELF_DOWNLOAD_PATH, f"makeself-{MAKESELF_VERSION}", "makeself.sh"
 )
 
 
+class SourceDirectoryNotFound(Exception):
+    """Raised when provided directory to package does not exist."""
+
+    def __init__(self, directory_path: str) -> None:
+        super().__init__(directory_path)
+        self.directory_path = directory_path
+
+
 def ensure_makeself() -> None:
     """If `makeself.sh` doesn't exist, downloads it."""
     if os.path.exists(MAKESELF_PATH):
         return
 
     if not os.path.exists(MAKESELF_DOWNLOAD_PATH):
         os.mkdir(MAKESELF_DOWNLOAD_PATH)
@@ -38,17 +47,26 @@
         stdout=subprocess.DEVNULL,
         stderr=subprocess.DEVNULL,
         cwd=MAKESELF_DOWNLOAD_PATH,
     )
 
 
 def create_package(
-    source_directory: str, output_path: str, build_command: str, startup_command: str
+    source_directory: str | None,
+    output_path: str,
+    build_command: str,
+    startup_command: str,
 ) -> None:
     """Create the makeself executable, with the startup script in it."""
+    if source_directory is None:
+        source_directory = tempfile.mkdtemp()
+
+    if not os.path.isdir(source_directory):
+        raise SourceDirectoryNotFound(source_directory)
+
     startup_script_name = "_packaged_startup.sh"
     startup_script_path = os.path.join(source_directory, startup_script_name)
 
     packaged_python_path = os.path.join(source_directory, ".packaged_python")
     if os.path.exists(packaged_python_path):
         shutil.rmtree(packaged_python_path)
```

### Comparing `packaged-0.1.1/src/packaged/cli.py` & `packaged-0.2.0/src/packaged/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from __future__ import annotations
 
 import argparse
 import os.path
 import platform
 
-from packaged import ensure_makeself, create_package
+from packaged import SourceDirectoryNotFound, ensure_makeself, create_package
 
 
 class CLIArgs:
     source_directory: str
     output_path: str
     build_command: str
     startup_command: str
@@ -20,32 +20,37 @@
     """Print error message"""
     print(f"\033[1;31mError:\033[m {message}")
 
 
 def cli(argv: list[str] | None = None) -> int:
     """CLI interface."""
     parser = argparse.ArgumentParser()
-    parser.add_argument(
-        "source_directory",
-        help="folder containing your python source to package",
-        type=os.path.abspath,
-    )
     parser.add_argument("output_path", help="Filename for the generated binary")
     parser.add_argument(
         "build_command", help="Python command to run when building the package"
     )
     parser.add_argument("startup_command", help="Command to run when the script starts")
+    parser.add_argument(
+        "source_directory",
+        help="Folder containing your python source to package",
+        type=os.path.abspath,
+        nargs="?",
+        default=None,
+    )
     args = parser.parse_args(argv, namespace=CLIArgs)
 
     if platform.system() == "Windows":
         error("Sorry, Windows is not supported yet. Ask for it on GitHub!")
         return 2
 
     ensure_makeself()
-    create_package(
-        args.source_directory,
-        args.output_path,
-        args.build_command,
-        args.startup_command,
-    )
+    try:
+        create_package(
+            args.source_directory,
+            args.output_path,
+            args.build_command,
+            args.startup_command,
+        )
+    except SourceDirectoryNotFound as exc:
+        error(f"Folder {exc.directory_path!r} does not exist.")
 
     return 0
```

