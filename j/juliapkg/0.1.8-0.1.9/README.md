# Comparing `tmp/juliapkg-0.1.8.tar.gz` & `tmp/juliapkg-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "juliapkg-0.1.8.tar", last modified: Wed Aug  3 18:57:37 2022, max compression
+gzip compressed data, was "juliapkg-0.1.9.tar", last modified: Sat Aug  6 12:27:03 2022, max compression
```

## Comparing `juliapkg-0.1.8.tar` & `juliapkg-0.1.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2022-08-03 18:57:37.553303 juliapkg-0.1.8/
--rw-rw-rw-   0        0        0     1096 2022-02-07 17:47:49.000000 juliapkg-0.1.8/LICENSE
--rw-rw-rw-   0        0        0     5437 2022-08-03 18:57:37.553303 juliapkg-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     5059 2022-07-18 09:46:35.000000 juliapkg-0.1.8/README.md
--rw-rw-rw-   0        0        0        0 2022-02-07 15:00:59.000000 juliapkg-0.1.8/pyproject.toml
--rw-rw-rw-   0        0        0      628 2022-08-03 18:57:37.563347 juliapkg-0.1.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2022-08-03 18:57:37.502869 juliapkg-0.1.8/src/
-drwxrwxrwx   0        0        0        0 2022-08-03 18:57:37.533209 juliapkg-0.1.8/src/juliapkg/
--rw-rw-rw-   0        0        0       98 2022-03-04 17:45:54.000000 juliapkg-0.1.8/src/juliapkg/__init__.py
--rw-rw-rw-   0        0        0     5605 2022-08-03 18:51:14.000000 juliapkg-0.1.8/src/juliapkg/compat.py
--rw-rw-rw-   0        0        0    14218 2022-07-18 10:24:38.000000 juliapkg-0.1.8/src/juliapkg/deps.py
--rw-rw-rw-   0        0        0     7449 2022-07-28 10:27:59.000000 juliapkg-0.1.8/src/juliapkg/find_julia.py
--rw-rw-rw-   0        0        0     7051 2022-07-28 09:25:43.000000 juliapkg-0.1.8/src/juliapkg/install_julia.py
--rw-rw-rw-   0        0        0       24 2022-02-15 17:12:29.000000 juliapkg-0.1.8/src/juliapkg/juliapkg.json
--rw-rw-rw-   0        0        0     3052 2022-07-18 10:25:13.000000 juliapkg-0.1.8/src/juliapkg/state.py
-drwxrwxrwx   0        0        0        0 2022-08-03 18:57:37.553303 juliapkg-0.1.8/src/juliapkg.egg-info/
--rw-rw-rw-   0        0        0     5437 2022-08-03 18:57:37.000000 juliapkg-0.1.8/src/juliapkg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      431 2022-08-03 18:57:37.000000 juliapkg-0.1.8/src/juliapkg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-08-03 18:57:37.000000 juliapkg-0.1.8/src/juliapkg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-02-15 17:13:50.000000 juliapkg-0.1.8/src/juliapkg.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       22 2022-08-03 18:57:37.000000 juliapkg-0.1.8/src/juliapkg.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2022-08-03 18:57:37.000000 juliapkg-0.1.8/src/juliapkg.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2022-08-06 12:27:03.024925 juliapkg-0.1.9/
+-rw-rw-rw-   0        0        0     1096 2022-02-07 17:47:49.000000 juliapkg-0.1.9/LICENSE
+-rw-rw-rw-   0        0        0     5437 2022-08-06 12:27:03.025926 juliapkg-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     5059 2022-07-18 09:46:35.000000 juliapkg-0.1.9/README.md
+-rw-rw-rw-   0        0        0        0 2022-02-07 15:00:59.000000 juliapkg-0.1.9/pyproject.toml
+-rw-rw-rw-   0        0        0      628 2022-08-06 12:27:03.031931 juliapkg-0.1.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2022-08-06 12:27:02.945025 juliapkg-0.1.9/src/
+drwxrwxrwx   0        0        0        0 2022-08-06 12:27:02.992670 juliapkg-0.1.9/src/juliapkg/
+-rw-rw-rw-   0        0        0       98 2022-03-04 17:45:54.000000 juliapkg-0.1.9/src/juliapkg/__init__.py
+-rw-rw-rw-   0        0        0     5605 2022-08-06 12:11:14.000000 juliapkg-0.1.9/src/juliapkg/compat.py
+-rw-rw-rw-   0        0        0    14183 2022-08-06 12:18:03.000000 juliapkg-0.1.9/src/juliapkg/deps.py
+-rw-rw-rw-   0        0        0     7445 2022-08-06 12:11:55.000000 juliapkg-0.1.9/src/juliapkg/find_julia.py
+-rw-rw-rw-   0        0        0     7051 2022-07-28 09:25:43.000000 juliapkg-0.1.9/src/juliapkg/install_julia.py
+-rw-rw-rw-   0        0        0       24 2022-08-06 12:19:18.000000 juliapkg-0.1.9/src/juliapkg/juliapkg.json
+-rw-rw-rw-   0        0        0     3052 2022-07-18 10:25:13.000000 juliapkg-0.1.9/src/juliapkg/state.py
+drwxrwxrwx   0        0        0        0 2022-08-06 12:27:03.021922 juliapkg-0.1.9/src/juliapkg.egg-info/
+-rw-rw-rw-   0        0        0     5437 2022-08-06 12:27:02.000000 juliapkg-0.1.9/src/juliapkg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      431 2022-08-06 12:27:02.000000 juliapkg-0.1.9/src/juliapkg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-08-06 12:27:02.000000 juliapkg-0.1.9/src/juliapkg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2022-02-15 17:13:50.000000 juliapkg-0.1.9/src/juliapkg.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       22 2022-08-06 12:27:02.000000 juliapkg-0.1.9/src/juliapkg.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2022-08-06 12:27:02.000000 juliapkg-0.1.9/src/juliapkg.egg-info/top_level.txt
```

### Comparing `juliapkg-0.1.8/LICENSE` & `juliapkg-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `juliapkg-0.1.8/PKG-INFO` & `juliapkg-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: juliapkg
-Version: 0.1.8
+Version: 0.1.9
 Summary: Julia version manager and package manager
 License: MIT
 Project-URL: Home, http://github.com/cjdoris/pyjuliapkg
 Classifier: Framework :: Django
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `juliapkg-0.1.8/README.md` & `juliapkg-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `juliapkg-0.1.8/setup.cfg` & `juliapkg-0.1.9/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206a 756c 6961 706b 670d 0a76 6572   = juliapkg..ver
-00000020: 7369 6f6e 203d 2030 2e31 2e38 0d0a 6465  sion = 0.1.8..de
+00000020: 7369 6f6e 203d 2030 2e31 2e39 0d0a 6465  sion = 0.1.9..de
 00000030: 7363 7269 7074 696f 6e20 3d20 4a75 6c69  scription = Juli
 00000040: 6120 7665 7273 696f 6e20 6d61 6e61 6765  a version manage
 00000050: 7220 616e 6420 7061 636b 6167 6520 6d61  r and package ma
 00000060: 6e61 6765 720d 0a6c 6f6e 675f 6465 7363  nager..long_desc
 00000070: 7269 7074 696f 6e20 3d20 6669 6c65 3a20  ription = file: 
 00000080: 5245 4144 4d45 2e6d 640d 0a6c 6f6e 675f  README.md..long_
 00000090: 6465 7363 7269 7074 696f 6e5f 636f 6e74  description_cont
```

### Comparing `juliapkg-0.1.8/src/juliapkg/compat.py` & `juliapkg-0.1.9/src/juliapkg/compat.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
                     elif prefix == '~':
                         if minor is None:
                             nfixed = 1
                         else:
                             nfixed = 2
                     clause = Range(version, nfixed)
                 elif part.startswith('='):
-                    version = Version(part[2:])
+                    version = Version(part[1:])
                     clause = Eq(version)
                 else:
                     raise ValueError(f'invalid version: {part!r}')
                 clauses.append(clause)
         return cls(clauses)
```

### Comparing `juliapkg-0.1.8/src/juliapkg/deps.py` & `juliapkg-0.1.9/src/juliapkg/deps.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from .find_julia import julia_version, find_julia
 from .install_julia import log
 
 logger = logging.getLogger('juliapkg')
 
 ### META
 
-META_VERSION = 3  # increment whenever the format changes
+META_VERSION = 4  # increment whenever the format changes
 
 def load_meta():
     fn = STATE['meta']
     if os.path.exists(fn):
         with open(fn) as fp:
             meta = json.load(fp)
             if meta.get('meta_version') == META_VERSION:
@@ -105,35 +105,32 @@
         logger.debug('was offline now online')
         return False
     # resolve whenever swapping between dev/not dev
     isdev = deps['dev']
     if isdev != STATE["dev"]:
         logger.debug('changed dev %s to %s', isdev, STATE['dev'])
         return False
-    # resolve whenever anything in sys.path changes
-    timestamp = deps["timestamp"]
-    timestamp = max(os.path.getmtime(STATE["meta"]), timestamp)
-    sys_path = deps["sys_path"]
-    if sys_path != sys.path:
-        logger.debug('sys.path changed %s to %s', sys_path, sys.path)
+    # resolve whenever any deps files change
+    files0 = set(deps_files())
+    files = deps['deps_files']
+    filesdiff = set(files.keys()).difference(files0)
+    if filesdiff:
+        logger.debug('deps files added %s', filesdiff)
         return False
-    for path in sys.path:
-        here = not path
-        if here:
-            path = os.getcwd()
-        if not os.path.exists(path):
-            continue
-        if (not here) and (os.path.getmtime(path) > timestamp):
-            logger.debug('directory changed %r', path)
+    filesdiff = files0.difference(files.keys())
+    if filesdiff:
+        logger.debug('deps files removed %s', filesdiff)
+        return False
+    for (filename, fileinfo) in files.items():
+        if not os.path.isfile(filename):
+            logger.debug('deps file no longer exists %r', filename)
+            return False
+        if os.path.getmtime(filename) > fileinfo['timestamp']:
+            logger.debug('deps file has changed %r', filename)
             return False
-        if os.path.isdir(path):
-            fn = os.path.join(path, "juliapkg.json")
-            if os.path.exists(fn) and os.path.getmtime(fn) > timestamp:
-                logger.debug('file changed %r', fn)
-                return False
     return deps
 
 def deps_files():
     ans = []
     # the default deps file
     ans.append(cur_deps_file())
     # look in sys.path
@@ -278,16 +275,18 @@
         run([exe, '--project='+project, '--startup-file=no', '-e', '; '.join(script)], check=True)
     # record that we resolved
     save_meta({
         "meta_version": META_VERSION,
         "dev": STATE["dev"],
         "version": str(ver),
         "executable": exe,
-        "timestamp": time.time(),
-        "sys_path": sys.path,
+        "deps_files": {
+            filename: {'timestamp': os.path.getmtime(filename)}
+            for filename in deps_files()
+        },
         "pkgs": [pkg.dict() for pkg in pkgs],
         "offline": bool(STATE['offline']),
         "override_executable": STATE['override_executable'],
     })
     STATE['resolved'] = True
     STATE['executable'] = exe
     STATE['version'] = ver
```

### Comparing `juliapkg-0.1.8/src/juliapkg/find_julia.py` & `juliapkg-0.1.9/src/juliapkg/find_julia.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,22 +48,22 @@
     if prefix is not None:
         ext = '.exe' if os.name == 'nt' else ''
         pr_exe = shutil.which(os.path.join(prefix, 'bin', 'julia' + ext))
         pr_ver = julia_version(pr_exe)
         if pr_ver is not None:
             if compat is None or pr_ver in compat:
                 if upgrade and bestcompat is None:
-                    bestcompat = Compat.parse('==' + best_julia_version(compat)[0])
+                    bestcompat = Compat.parse('=' + best_julia_version(compat)[0])
                 if bestcompat is None or pr_ver in bestcompat:
                     return (pr_exe, pr_ver)
     # see if juliaup is installed
     try_jl = True
     ju_exe = shutil.which('juliaup')
     if ju_exe:
-        ju_compat = Compat.parse('==' + ju_best_julia_version(compat)[0]) if upgrade else compat
+        ju_compat = Compat.parse('=' + ju_best_julia_version(compat)[0]) if upgrade else compat
         ans = ju_find_julia(ju_compat, install=install)
         if ans:
             return ans
         try_jl = install
     if try_jl:
         # see if julia is installed
         jl_exe = shutil.which('julia')
@@ -73,15 +73,15 @@
                 return (jl_exe, jl_ver)
             else:
                 log(f'WARNING: You have Julia {jl_ver} installed but {compat} is required.')
                 log(f'  It is recommended that you upgrade Julia or install JuliaUp.')
     # install into the prefix
     if install and prefix is not None:
         if upgrade and bestcompat is None:
-            bestcompat = Compat.parse('==' + best_julia_version(compat)[0])
+            bestcompat = Compat.parse('=' + best_julia_version(compat)[0])
         ver, info = best_julia_version(bestcompat if upgrade else compat)
         log(f'WARNING: About to install Julia {ver} to {prefix}.')
         log(f'  If you use juliapkg in more than one environment, you are likely to have Julia')
         log(f'  installed in multiple locations. It is recommended to install JuliaUp')
         log(f'  (https://github.com/JuliaLang/juliaup) or Julia (https://julialang.org/downloads)')
         log(f'  yourself.')
         install_julia(info, prefix)
@@ -140,15 +140,15 @@
                 break
             else:
                 msg = proc.stderr.decode('utf-8').strip()
                 if msg not in msgs:
                     msgs.append(msg)
         if msgs:
             log(f'WARNING: Failed to install Julia {ver} using JuliaUp: {msgs}')
-        ans = ju_find_julia_noinstall(Compat.parse('==' + ver))
+        ans = ju_find_julia_noinstall(Compat.parse('=' + ver))
         if ans:
             return ans
         Exception(f'JuliaUp just installed Julia {ver} but cannot find it')
 
 def ju_find_julia_noinstall(compat=None):
     judir = os.path.join(STATE['depot'], 'juliaup')
     metaname = os.path.join(judir, 'juliaup.json')
```

### Comparing `juliapkg-0.1.8/src/juliapkg/install_julia.py` & `juliapkg-0.1.9/src/juliapkg/install_julia.py`

 * *Files identical despite different names*

### Comparing `juliapkg-0.1.8/src/juliapkg/state.py` & `juliapkg-0.1.9/src/juliapkg/state.py`

 * *Files identical despite different names*

### Comparing `juliapkg-0.1.8/src/juliapkg.egg-info/PKG-INFO` & `juliapkg-0.1.9/src/juliapkg.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: juliapkg
-Version: 0.1.8
+Version: 0.1.9
 Summary: Julia version manager and package manager
 License: MIT
 Project-URL: Home, http://github.com/cjdoris/pyjuliapkg
 Classifier: Framework :: Django
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

