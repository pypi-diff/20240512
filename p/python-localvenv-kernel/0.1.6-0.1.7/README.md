# Comparing `tmp/python-localvenv-kernel-0.1.6.tar.gz` & `tmp/python-localvenv-kernel-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-localvenv-kernel-0.1.6.tar", last modified: Wed Mar 27 19:43:23 2024, max compression
+gzip compressed data, was "python-localvenv-kernel-0.1.7.tar", last modified: Sun May 12 19:43:10 2024, max compression
```

## Comparing `python-localvenv-kernel-0.1.6.tar` & `python-localvenv-kernel-0.1.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 19:43:23.680372 python-localvenv-kernel-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-03-27 19:43:15.000000 python-localvenv-kernel-0.1.6/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     3513 2024-03-27 19:43:23.680372 python-localvenv-kernel-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-03-27 19:43:15.000000 python-localvenv-kernel-0.1.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-27 19:43:23.684373 python-localvenv-kernel-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2328 2024-03-27 19:43:15.000000 python-localvenv-kernel-0.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 19:43:23.680372 python-localvenv-kernel-0.1.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 19:43:23.680372 python-localvenv-kernel-0.1.6/src/localvenv_kernel/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 19:43:15.000000 python-localvenv-kernel-0.1.6/src/localvenv_kernel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3726 2024-03-27 19:43:15.000000 python-localvenv-kernel-0.1.6/src/localvenv_kernel/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      916 2024-03-27 19:43:15.000000 python-localvenv-kernel-0.1.6/src/localvenv_kernel/kernelspec.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 19:43:23.680372 python-localvenv-kernel-0.1.6/src/python_localvenv_kernel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3513 2024-03-27 19:43:23.000000 python-localvenv-kernel-0.1.6/src/python_localvenv_kernel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-03-27 19:43:23.000000 python-localvenv-kernel-0.1.6/src/python_localvenv_kernel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 19:43:23.000000 python-localvenv-kernel-0.1.6/src/python_localvenv_kernel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-27 19:43:23.000000 python-localvenv-kernel-0.1.6/src/python_localvenv_kernel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-27 19:43:23.000000 python-localvenv-kernel-0.1.6/src/python_localvenv_kernel.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 19:43:23.680372 python-localvenv-kernel-0.1.6/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-03-27 19:43:15.000000 python-localvenv-kernel-0.1.6/test/test_kernel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:43:10.406596 python-localvenv-kernel-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-12 19:43:07.000000 python-localvenv-kernel-0.1.7/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3513 2024-05-12 19:43:10.406596 python-localvenv-kernel-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-05-12 19:43:07.000000 python-localvenv-kernel-0.1.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 19:43:10.406596 python-localvenv-kernel-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2328 2024-05-12 19:43:07.000000 python-localvenv-kernel-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:43:10.406596 python-localvenv-kernel-0.1.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:43:10.406596 python-localvenv-kernel-0.1.7/src/localvenv_kernel/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 19:43:07.000000 python-localvenv-kernel-0.1.7/src/localvenv_kernel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4147 2024-05-12 19:43:07.000000 python-localvenv-kernel-0.1.7/src/localvenv_kernel/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-05-12 19:43:07.000000 python-localvenv-kernel-0.1.7/src/localvenv_kernel/kernelspec.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:43:10.406596 python-localvenv-kernel-0.1.7/src/python_localvenv_kernel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3513 2024-05-12 19:43:10.000000 python-localvenv-kernel-0.1.7/src/python_localvenv_kernel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-05-12 19:43:10.000000 python-localvenv-kernel-0.1.7/src/python_localvenv_kernel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 19:43:10.000000 python-localvenv-kernel-0.1.7/src/python_localvenv_kernel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-12 19:43:10.000000 python-localvenv-kernel-0.1.7/src/python_localvenv_kernel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-12 19:43:10.000000 python-localvenv-kernel-0.1.7/src/python_localvenv_kernel.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:43:10.406596 python-localvenv-kernel-0.1.7/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-05-12 19:43:07.000000 python-localvenv-kernel-0.1.7/test/test_kernel.py
```

### Comparing `python-localvenv-kernel-0.1.6/LICENSE.md` & `python-localvenv-kernel-0.1.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `python-localvenv-kernel-0.1.6/PKG-INFO` & `python-localvenv-kernel-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-localvenv-kernel
-Version: 0.1.6
+Version: 0.1.7
 Summary: Python Jupyter kernel delegating to a local virtual environment
 Home-page: https://github.com/goerz/python-localvenv-kernel
 Author: Michael H. Goerz
 Author-email: mail@michaelgoerz.net
 License: MIT
 Keywords: Interactive,Interpreter,Shell,Web
 Classifier: Framework :: Jupyter
```

### Comparing `python-localvenv-kernel-0.1.6/README.md` & `python-localvenv-kernel-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `python-localvenv-kernel-0.1.6/setup.py` & `python-localvenv-kernel-0.1.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 # NOTE: Editable installs won't copy the kernel file. See `Makefile`
 
 with open(os.path.join(current_dir, "README.md")) as fp:
     README = fp.read()
 
 setup(
     name="python-localvenv-kernel",
-    version="0.1.6",
+    version="0.1.7",
     author="Michael H. Goerz",
     author_email="mail@michaelgoerz.net",
     url="https://github.com/goerz/python-localvenv-kernel",
     license="MIT",
     description=(
         "Python Jupyter kernel delegating to a local virtual environment"
     ),
```

### Comparing `python-localvenv-kernel-0.1.6/src/localvenv_kernel/__main__.py` & `python-localvenv-kernel-0.1.7/src/localvenv_kernel/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -51,14 +51,23 @@
 
             ERROR: {exc_info.output.strip()}
 
             Make sure that the 'ipykernel' package is installed in the virtual
             environment {venv_folder}
             """
         )
+    except OSError as exc_info:
+        error(
+            f"""
+            {' '.join([str(a) for a in cmd_check_kernel])}
+            failed:
+
+            ERROR: {exc_info}
+            """
+        )
     cmd = [
         python,
         "-m",
         "ipykernel_launcher",
         *sys.argv[1:],
     ]
     print(
@@ -134,13 +143,17 @@
 
 def find_python(venv):
     if "KERNEL_VENV_PYTHON" in os.environ:
         python = venv / os.path.normpath(os.environ["KERNEL_VENV_PYTHON"])
     else:
         python = venv / "bin" / "python"
         if platform.system() == "Windows":
-            python = venv / "Scripts" / "python"
+            python = venv / "Scripts" / "python.exe"  # python -m venv
+            if not python.is_file():  # some versions of conda (?)
+                python = venv / "python.exe"
+    if not python.is_file():
+        print(f"WARNING: file '{python}' does not exist")
     return python
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `python-localvenv-kernel-0.1.6/src/localvenv_kernel/kernelspec.py` & `python-localvenv-kernel-0.1.7/src/localvenv_kernel/kernelspec.py`

 * *Files identical despite different names*

### Comparing `python-localvenv-kernel-0.1.6/src/python_localvenv_kernel.egg-info/PKG-INFO` & `python-localvenv-kernel-0.1.7/src/python_localvenv_kernel.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-localvenv-kernel
-Version: 0.1.6
+Version: 0.1.7
 Summary: Python Jupyter kernel delegating to a local virtual environment
 Home-page: https://github.com/goerz/python-localvenv-kernel
 Author: Michael H. Goerz
 Author-email: mail@michaelgoerz.net
 License: MIT
 Keywords: Interactive,Interpreter,Shell,Web
 Classifier: Framework :: Jupyter
```

### Comparing `python-localvenv-kernel-0.1.6/test/test_kernel.py` & `python-localvenv-kernel-0.1.7/test/test_kernel.py`

 * *Files identical despite different names*

