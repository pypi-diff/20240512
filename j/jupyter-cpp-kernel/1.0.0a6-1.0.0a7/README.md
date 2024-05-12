# Comparing `tmp/jupyter-cpp-kernel-1.0.0a6.tar.gz` & `tmp/jupyter-cpp-kernel-1.0.0a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyter-cpp-kernel-1.0.0a6.tar", last modified: Fri Jan 26 14:48:45 2024, max compression
+gzip compressed data, was "jupyter-cpp-kernel-1.0.0a7.tar", last modified: Fri Feb  2 00:16:41 2024, max compression
```

## Comparing `jupyter-cpp-kernel-1.0.0a6.tar` & `jupyter-cpp-kernel-1.0.0a7.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0 shiroinekotfs  (1000) shiroinekotfs  (1000)        0 2024-01-26 14:48:45.499188 jupyter-cpp-kernel-1.0.0a6/
--rwxrwxrwx   0 shiroinekotfs  (1000) shiroinekotfs  (1000)     1092 2024-01-26 14:44:22.000000 jupyter-cpp-kernel-1.0.0a6/LICENSE
--rwxrwxrwx   0 shiroinekotfs  (1000) shiroinekotfs  (1000)      418 2023-11-09 00:27:49.000000 jupyter-cpp-kernel-1.0.0a6/MANIFEST.in
--rwxrwxrwx   0 shiroinekotfs  (1000) shiroinekotfs  (1000)     2965 2024-01-26 14:48:45.488974 jupyter-cpp-kernel-1.0.0a6/PKG-INFO
--rwxrwxrwx   0 shiroinekotfs  (1000) shiroinekotfs  (1000)     2159 2024-01-26 14:45:41.000000 jupyter-cpp-kernel-1.0.0a6/README.md
--rwxrwxrwx   0 shiroinekotfs  (1000) shiroinekotfs  (1000)      298 2023-10-20 08:54:30.000000 jupyter-cpp-kernel-1.0.0a6/SECURITY.md
-drwxrwxrwx   0 shiroinekotfs  (1000) shiroinekotfs  (1000)        0 2024-01-26 14:48:45.032289 jupyter-cpp-kernel-1.0.0a6/jupyter-cpp-kernel/
--rwxrwxrwx   0 shiroinekotfs  (1000) shiroinekotfs  (1000)        0 2023-10-20 08:17:06.000000 jupyter-cpp-kernel-1.0.0a6/jupyter-cpp-kernel/__init__.py
--rwxrwxrwx   0 shiroinekotfs  (1000) shiroinekotfs  (1000)      129 2023-10-20 08:17:06.000000 jupyter-cpp-kernel-1.0.0a6/jupyter-cpp-kernel/__main__.py
--rwxrwxrwx   0 shiroinekotfs  (1000) shiroinekotfs  (1000)    12244 2024-01-26 14:44:22.000000 jupyter-cpp-kernel-1.0.0a6/jupyter-cpp-kernel/kernel.py
-drwxrwxrwx   0 shiroinekotfs  (1000) shiroinekotfs  (1000)        0 2024-01-26 14:48:45.076086 jupyter-cpp-kernel-1.0.0a6/jupyter-cpp-kernel/resources/
-drwxrwxrwx   0 shiroinekotfs  (1000) shiroinekotfs  (1000)        0 2024-01-26 14:48:45.143524 jupyter-cpp-kernel-1.0.0a6/jupyter-cpp-kernel/resources/basicf/
--rwxrwxrwx   0 shiroinekotfs  (1000) shiroinekotfs  (1000)     3748 2023-11-09 00:27:49.000000 jupyter-cpp-kernel-1.0.0a6/jupyter-cpp-kernel/resources/basicf/dlfcn.h
--rwxrwxrwx   0 shiroinekotfs  (1000) shiroinekotfs  (1000)     4016 2024-01-26 14:44:22.000000 jupyter-cpp-kernel-1.0.0a6/jupyter-cpp-kernel/resources/basicf/mathdefs.hpp
--rwxrwxrwx   0 shiroinekotfs  (1000) shiroinekotfs  (1000)     9070 2023-11-09 00:27:49.000000 jupyter-cpp-kernel-1.0.0a6/jupyter-cpp-kernel/resources/basicf/rstdio.h
--rwxrwxrwx   0 shiroinekotfs  (1000) shiroinekotfs  (1000)     1439 2024-01-26 14:44:22.000000 jupyter-cpp-kernel-1.0.0a6/jupyter-cpp-kernel/resources/gcpph.hpp
--rwxrwxrwx   0 shiroinekotfs  (1000) shiroinekotfs  (1000)     1587 2024-01-26 14:44:22.000000 jupyter-cpp-kernel-1.0.0a6/jupyter-cpp-kernel/resources/master.cpp
-drwxrwxrwx   0 shiroinekotfs  (1000) shiroinekotfs  (1000)        0 2024-01-26 14:48:45.207252 jupyter-cpp-kernel-1.0.0a6/jupyter-cpp-kernel/resources/output/
--rwxrwxrwx   0 shiroinekotfs  (1000) shiroinekotfs  (1000)     2850 2024-01-26 14:44:22.000000 jupyter-cpp-kernel-1.0.0a6/jupyter-cpp-kernel/resources/output/jdisplay.hpp
--rwxrwxrwx   0 shiroinekotfs  (1000) shiroinekotfs  (1000)     1367 2024-01-26 14:44:22.000000 jupyter-cpp-kernel-1.0.0a6/jupyter-cpp-kernel/resources/output/ytlinkpro.hpp
-drwxrwxrwx   0 shiroinekotfs  (1000) shiroinekotfs  (1000)        0 2024-01-26 14:48:45.473141 jupyter-cpp-kernel-1.0.0a6/jupyter_cpp_kernel.egg-info/
--rwxrwxrwx   0 shiroinekotfs  (1000) shiroinekotfs  (1000)     2965 2024-01-26 14:48:44.000000 jupyter-cpp-kernel-1.0.0a6/jupyter_cpp_kernel.egg-info/PKG-INFO
--rwxrwxrwx   0 shiroinekotfs  (1000) shiroinekotfs  (1000)      784 2024-01-26 14:48:44.000000 jupyter-cpp-kernel-1.0.0a6/jupyter_cpp_kernel.egg-info/SOURCES.txt
--rwxrwxrwx   0 shiroinekotfs  (1000) shiroinekotfs  (1000)        1 2024-01-26 14:48:44.000000 jupyter-cpp-kernel-1.0.0a6/jupyter_cpp_kernel.egg-info/dependency_links.txt
--rwxrwxrwx   0 shiroinekotfs  (1000) shiroinekotfs  (1000)       19 2024-01-26 14:48:44.000000 jupyter-cpp-kernel-1.0.0a6/jupyter_cpp_kernel.egg-info/top_level.txt
-drwxrwxrwx   0 shiroinekotfs  (1000) shiroinekotfs  (1000)        0 2024-01-26 14:48:45.413932 jupyter-cpp-kernel-1.0.0a6/kernel_spec/
--rwxrwxrwx   0 shiroinekotfs  (1000) shiroinekotfs  (1000)      191 2023-10-20 08:17:06.000000 jupyter-cpp-kernel-1.0.0a6/kernel_spec/kernel.json
--rwxrwxrwx   0 shiroinekotfs  (1000) shiroinekotfs  (1000)     5218 2023-10-20 08:17:06.000000 jupyter-cpp-kernel-1.0.0a6/kernel_spec/logo-32x32.png
--rwxrwxrwx   0 shiroinekotfs  (1000) shiroinekotfs  (1000)    19133 2023-10-20 08:17:06.000000 jupyter-cpp-kernel-1.0.0a6/kernel_spec/logo-64x64.png
--rwxrwxrwx   0 shiroinekotfs  (1000) shiroinekotfs  (1000)     1919 2023-10-20 08:17:06.000000 jupyter-cpp-kernel-1.0.0a6/kernel_spec/logo-svg.svg
--rwxrwxrwx   0 shiroinekotfs  (1000) shiroinekotfs  (1000)      111 2023-10-20 08:17:06.000000 jupyter-cpp-kernel-1.0.0a6/pyproject.toml
--rwxrwxrwx   0 shiroinekotfs  (1000) shiroinekotfs  (1000)      808 2024-01-26 14:48:45.519442 jupyter-cpp-kernel-1.0.0a6/setup.cfg
--rwxrwxrwx   0 shiroinekotfs  (1000) shiroinekotfs  (1000)     1194 2024-01-26 14:44:22.000000 jupyter-cpp-kernel-1.0.0a6/setup.py
-drwxrwxrwx   0 shiroinekotfs  (1000) shiroinekotfs  (1000)        0 2024-01-26 14:48:44.872621 jupyter-cpp-kernel-1.0.0a6/share/
-drwxrwxrwx   0 shiroinekotfs  (1000) shiroinekotfs  (1000)        0 2024-01-26 14:48:45.439232 jupyter-cpp-kernel-1.0.0a6/share/cpp_header/
--rwxrwxrwx   0 shiroinekotfs  (1000) shiroinekotfs  (1000)      978 2024-01-26 14:44:22.000000 jupyter-cpp-kernel-1.0.0a6/share/cpp_header/check_cpp.hpp
+drwxrwxrwx   0 shiroinekotfs  (1000) shiroinekotfs  (1000)        0 2024-02-02 00:16:41.392012 jupyter-cpp-kernel-1.0.0a7/
+-rwxrwxrwx   0 shiroinekotfs  (1000) shiroinekotfs  (1000)     1092 2024-01-26 14:44:22.000000 jupyter-cpp-kernel-1.0.0a7/LICENSE
+-rwxrwxrwx   0 shiroinekotfs  (1000) shiroinekotfs  (1000)      418 2023-11-09 00:27:49.000000 jupyter-cpp-kernel-1.0.0a7/MANIFEST.in
+-rwxrwxrwx   0 shiroinekotfs  (1000) shiroinekotfs  (1000)     2965 2024-02-02 00:16:41.386493 jupyter-cpp-kernel-1.0.0a7/PKG-INFO
+-rwxrwxrwx   0 shiroinekotfs  (1000) shiroinekotfs  (1000)     2159 2024-01-26 14:45:41.000000 jupyter-cpp-kernel-1.0.0a7/README.md
+-rwxrwxrwx   0 shiroinekotfs  (1000) shiroinekotfs  (1000)      298 2023-10-20 08:54:30.000000 jupyter-cpp-kernel-1.0.0a7/SECURITY.md
+drwxrwxrwx   0 shiroinekotfs  (1000) shiroinekotfs  (1000)        0 2024-02-02 00:16:40.909709 jupyter-cpp-kernel-1.0.0a7/jupyter-cpp-kernel/
+-rwxrwxrwx   0 shiroinekotfs  (1000) shiroinekotfs  (1000)        0 2023-10-20 08:17:06.000000 jupyter-cpp-kernel-1.0.0a7/jupyter-cpp-kernel/__init__.py
+-rwxrwxrwx   0 shiroinekotfs  (1000) shiroinekotfs  (1000)      129 2023-10-20 08:17:06.000000 jupyter-cpp-kernel-1.0.0a7/jupyter-cpp-kernel/__main__.py
+-rwxrwxrwx   0 shiroinekotfs  (1000) shiroinekotfs  (1000)    12347 2024-02-02 00:16:07.000000 jupyter-cpp-kernel-1.0.0a7/jupyter-cpp-kernel/kernel.py
+drwxrwxrwx   0 shiroinekotfs  (1000) shiroinekotfs  (1000)        0 2024-02-02 00:16:40.963353 jupyter-cpp-kernel-1.0.0a7/jupyter-cpp-kernel/resources/
+drwxrwxrwx   0 shiroinekotfs  (1000) shiroinekotfs  (1000)        0 2024-02-02 00:16:41.065615 jupyter-cpp-kernel-1.0.0a7/jupyter-cpp-kernel/resources/basicf/
+-rwxrwxrwx   0 shiroinekotfs  (1000) shiroinekotfs  (1000)     3748 2023-11-09 00:27:49.000000 jupyter-cpp-kernel-1.0.0a7/jupyter-cpp-kernel/resources/basicf/dlfcn.h
+-rwxrwxrwx   0 shiroinekotfs  (1000) shiroinekotfs  (1000)     4016 2024-01-26 14:44:22.000000 jupyter-cpp-kernel-1.0.0a7/jupyter-cpp-kernel/resources/basicf/mathdefs.hpp
+-rwxrwxrwx   0 shiroinekotfs  (1000) shiroinekotfs  (1000)     9070 2023-11-09 00:27:49.000000 jupyter-cpp-kernel-1.0.0a7/jupyter-cpp-kernel/resources/basicf/rstdio.h
+-rwxrwxrwx   0 shiroinekotfs  (1000) shiroinekotfs  (1000)     1439 2024-01-26 14:44:22.000000 jupyter-cpp-kernel-1.0.0a7/jupyter-cpp-kernel/resources/gcpph.hpp
+-rwxrwxrwx   0 shiroinekotfs  (1000) shiroinekotfs  (1000)     1587 2024-01-26 14:44:22.000000 jupyter-cpp-kernel-1.0.0a7/jupyter-cpp-kernel/resources/master.cpp
+drwxrwxrwx   0 shiroinekotfs  (1000) shiroinekotfs  (1000)        0 2024-02-02 00:16:41.130658 jupyter-cpp-kernel-1.0.0a7/jupyter-cpp-kernel/resources/output/
+-rwxrwxrwx   0 shiroinekotfs  (1000) shiroinekotfs  (1000)     2850 2024-01-26 14:44:22.000000 jupyter-cpp-kernel-1.0.0a7/jupyter-cpp-kernel/resources/output/jdisplay.hpp
+-rwxrwxrwx   0 shiroinekotfs  (1000) shiroinekotfs  (1000)     1367 2024-01-26 14:44:22.000000 jupyter-cpp-kernel-1.0.0a7/jupyter-cpp-kernel/resources/output/ytlinkpro.hpp
+drwxrwxrwx   0 shiroinekotfs  (1000) shiroinekotfs  (1000)        0 2024-02-02 00:16:41.372961 jupyter-cpp-kernel-1.0.0a7/jupyter_cpp_kernel.egg-info/
+-rwxrwxrwx   0 shiroinekotfs  (1000) shiroinekotfs  (1000)     2965 2024-02-02 00:16:40.000000 jupyter-cpp-kernel-1.0.0a7/jupyter_cpp_kernel.egg-info/PKG-INFO
+-rwxrwxrwx   0 shiroinekotfs  (1000) shiroinekotfs  (1000)      784 2024-02-02 00:16:40.000000 jupyter-cpp-kernel-1.0.0a7/jupyter_cpp_kernel.egg-info/SOURCES.txt
+-rwxrwxrwx   0 shiroinekotfs  (1000) shiroinekotfs  (1000)        1 2024-02-02 00:16:40.000000 jupyter-cpp-kernel-1.0.0a7/jupyter_cpp_kernel.egg-info/dependency_links.txt
+-rwxrwxrwx   0 shiroinekotfs  (1000) shiroinekotfs  (1000)       19 2024-02-02 00:16:40.000000 jupyter-cpp-kernel-1.0.0a7/jupyter_cpp_kernel.egg-info/top_level.txt
+drwxrwxrwx   0 shiroinekotfs  (1000) shiroinekotfs  (1000)        0 2024-02-02 00:16:41.311570 jupyter-cpp-kernel-1.0.0a7/kernel_spec/
+-rwxrwxrwx   0 shiroinekotfs  (1000) shiroinekotfs  (1000)      191 2023-10-20 08:17:06.000000 jupyter-cpp-kernel-1.0.0a7/kernel_spec/kernel.json
+-rwxrwxrwx   0 shiroinekotfs  (1000) shiroinekotfs  (1000)     5218 2023-10-20 08:17:06.000000 jupyter-cpp-kernel-1.0.0a7/kernel_spec/logo-32x32.png
+-rwxrwxrwx   0 shiroinekotfs  (1000) shiroinekotfs  (1000)    19133 2023-10-20 08:17:06.000000 jupyter-cpp-kernel-1.0.0a7/kernel_spec/logo-64x64.png
+-rwxrwxrwx   0 shiroinekotfs  (1000) shiroinekotfs  (1000)     1919 2023-10-20 08:17:06.000000 jupyter-cpp-kernel-1.0.0a7/kernel_spec/logo-svg.svg
+-rwxrwxrwx   0 shiroinekotfs  (1000) shiroinekotfs  (1000)      111 2023-10-20 08:17:06.000000 jupyter-cpp-kernel-1.0.0a7/pyproject.toml
+-rwxrwxrwx   0 shiroinekotfs  (1000) shiroinekotfs  (1000)      808 2024-02-02 00:16:41.403556 jupyter-cpp-kernel-1.0.0a7/setup.cfg
+-rwxrwxrwx   0 shiroinekotfs  (1000) shiroinekotfs  (1000)     1194 2024-02-02 00:12:24.000000 jupyter-cpp-kernel-1.0.0a7/setup.py
+drwxrwxrwx   0 shiroinekotfs  (1000) shiroinekotfs  (1000)        0 2024-02-02 00:16:40.730891 jupyter-cpp-kernel-1.0.0a7/share/
+drwxrwxrwx   0 shiroinekotfs  (1000) shiroinekotfs  (1000)        0 2024-02-02 00:16:41.337839 jupyter-cpp-kernel-1.0.0a7/share/cpp_header/
+-rwxrwxrwx   0 shiroinekotfs  (1000) shiroinekotfs  (1000)      978 2024-01-26 14:44:22.000000 jupyter-cpp-kernel-1.0.0a7/share/cpp_header/check_cpp.hpp
```

### Comparing `jupyter-cpp-kernel-1.0.0a6/LICENSE` & `jupyter-cpp-kernel-1.0.0a7/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyter-cpp-kernel-1.0.0a6/PKG-INFO` & `jupyter-cpp-kernel-1.0.0a7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyter-cpp-kernel
-Version: 1.0.0a6
+Version: 1.0.0a7
 Summary: C++ 14 kernel for Jupyter
 Home-page: https://github.com/shiroinekotfs/jupyter-cpp-kernel
 Download-URL: https://github.com/shiroinekotfs/jupyter-cpp-kernel/releases
 Author: shiroinekotfs
 Author-email: shiroineko.tfs@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/shiroinekotfs/jupyter-cpp-kernel/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: jupyter-cpp-kernel Version: 1.0.0a6 Summary: C++ 14
+Metadata-Version: 2.1 Name: jupyter-cpp-kernel Version: 1.0.0a7 Summary: C++ 14
 kernel for Jupyter Home-page: https://github.com/shiroinekotfs/jupyter-cpp-
 kernel Download-URL: https://github.com/shiroinekotfs/jupyter-cpp-kernel/
 releases Author: shiroinekotfs Author-email: shiroineko.tfs@gmail.com License:
 MIT Project-URL: Bug Tracker, https://github.com/shiroinekotfs/jupyter-cpp-
 kernel/issues Keywords: windows,macos,linux,jupyter,cpp,cpp14,jupyter-
 kernels,pip Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: C++ Classifier: License :: OSI Approved :: MIT License
```

### Comparing `jupyter-cpp-kernel-1.0.0a6/README.md` & `jupyter-cpp-kernel-1.0.0a7/README.md`

 * *Files identical despite different names*

### Comparing `jupyter-cpp-kernel-1.0.0a6/jupyter-cpp-kernel/kernel.py` & `jupyter-cpp-kernel-1.0.0a7/jupyter-cpp-kernel/kernel.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,15 +88,15 @@
     language_version = 'C++14'
     language_info = {
                      'name': 'text/markdown',
                      'mimetype': 'text/markdown',
                      'file_extension': '.cpp'
                     }
     
-    introduction = "C++ 14 kernel for Jupyter (master), version 1.0.0a6\n\n"
+    introduction = "C++ 14 kernel for Jupyter (master), version 1.0.0a7\n\n"
     cp_banner = "Copyright (C) 2024 shiroinekotfs\nCopyright (C) Brendan Rius\nCopyright (C) Free Software Foundation, Inc\n\n"
     links_guide = "Legal information: https://github.com/shiroinekotfs/jupyter-cpp-kernel/blob/master/LICENSE\nNotebook tutorial: https://github.com/shiroinekotfs/jupyter-cpp-kernel-doc\n\nAuthor GitHub profile: https://github.com/shiroinekotfs\n"
     reporting_links = "Reporting the issue: https://github.com/shiroinekotfs/jupyter-cpp-kernel/issues"
 
     banner = introduction + cp_banner + links_guide + reporting_links
 
     main_head = "#include <iostream>\n" + "int main(){\n"
@@ -132,15 +132,18 @@
     def new_temp_file(self, **kwargs):
         # We don't want the file to be deleted when closed, but only when the kernel stops
         file = tempfile.NamedTemporaryFile(delete=False, mode='w', **kwargs)
         self.files.append(file.name)
         return file
 
     def _write_to_stdout(self, contents):
-        contents = contents.replace("\r\n", "\r\n\r\n")
+        if os.name == 'nt':
+            contents = contents.replace("\r\n", "\r\n\r\n")
+        else:
+            contents = contents.replace("\n", "\n\n")
         self.send_response(self.iopub_socket, 
                            'display_data',
                            {
                             'data':{
                                'text/markdown': contents
                                 },
                             'metadata': {}
```

### Comparing `jupyter-cpp-kernel-1.0.0a6/jupyter-cpp-kernel/resources/basicf/dlfcn.h` & `jupyter-cpp-kernel-1.0.0a7/jupyter-cpp-kernel/resources/basicf/dlfcn.h`

 * *Files identical despite different names*

### Comparing `jupyter-cpp-kernel-1.0.0a6/jupyter-cpp-kernel/resources/basicf/mathdefs.hpp` & `jupyter-cpp-kernel-1.0.0a7/jupyter-cpp-kernel/resources/basicf/mathdefs.hpp`

 * *Files identical despite different names*

### Comparing `jupyter-cpp-kernel-1.0.0a6/jupyter-cpp-kernel/resources/basicf/rstdio.h` & `jupyter-cpp-kernel-1.0.0a7/jupyter-cpp-kernel/resources/basicf/rstdio.h`

 * *Files identical despite different names*

### Comparing `jupyter-cpp-kernel-1.0.0a6/jupyter-cpp-kernel/resources/gcpph.hpp` & `jupyter-cpp-kernel-1.0.0a7/jupyter-cpp-kernel/resources/gcpph.hpp`

 * *Files identical despite different names*

### Comparing `jupyter-cpp-kernel-1.0.0a6/jupyter-cpp-kernel/resources/master.cpp` & `jupyter-cpp-kernel-1.0.0a7/jupyter-cpp-kernel/resources/master.cpp`

 * *Files identical despite different names*

### Comparing `jupyter-cpp-kernel-1.0.0a6/jupyter-cpp-kernel/resources/output/jdisplay.hpp` & `jupyter-cpp-kernel-1.0.0a7/jupyter-cpp-kernel/resources/output/jdisplay.hpp`

 * *Files identical despite different names*

### Comparing `jupyter-cpp-kernel-1.0.0a6/jupyter-cpp-kernel/resources/output/ytlinkpro.hpp` & `jupyter-cpp-kernel-1.0.0a7/jupyter-cpp-kernel/resources/output/ytlinkpro.hpp`

 * *Files identical despite different names*

### Comparing `jupyter-cpp-kernel-1.0.0a6/jupyter_cpp_kernel.egg-info/PKG-INFO` & `jupyter-cpp-kernel-1.0.0a7/jupyter_cpp_kernel.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyter-cpp-kernel
-Version: 1.0.0a6
+Version: 1.0.0a7
 Summary: C++ 14 kernel for Jupyter
 Home-page: https://github.com/shiroinekotfs/jupyter-cpp-kernel
 Download-URL: https://github.com/shiroinekotfs/jupyter-cpp-kernel/releases
 Author: shiroinekotfs
 Author-email: shiroineko.tfs@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/shiroinekotfs/jupyter-cpp-kernel/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: jupyter-cpp-kernel Version: 1.0.0a6 Summary: C++ 14
+Metadata-Version: 2.1 Name: jupyter-cpp-kernel Version: 1.0.0a7 Summary: C++ 14
 kernel for Jupyter Home-page: https://github.com/shiroinekotfs/jupyter-cpp-
 kernel Download-URL: https://github.com/shiroinekotfs/jupyter-cpp-kernel/
 releases Author: shiroinekotfs Author-email: shiroineko.tfs@gmail.com License:
 MIT Project-URL: Bug Tracker, https://github.com/shiroinekotfs/jupyter-cpp-
 kernel/issues Keywords: windows,macos,linux,jupyter,cpp,cpp14,jupyter-
 kernels,pip Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: C++ Classifier: License :: OSI Approved :: MIT License
```

### Comparing `jupyter-cpp-kernel-1.0.0a6/jupyter_cpp_kernel.egg-info/SOURCES.txt` & `jupyter-cpp-kernel-1.0.0a7/jupyter_cpp_kernel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jupyter-cpp-kernel-1.0.0a6/kernel_spec/logo-32x32.png` & `jupyter-cpp-kernel-1.0.0a7/kernel_spec/logo-32x32.png`

 * *Files identical despite different names*

### Comparing `jupyter-cpp-kernel-1.0.0a6/kernel_spec/logo-64x64.png` & `jupyter-cpp-kernel-1.0.0a7/kernel_spec/logo-64x64.png`

 * *Files identical despite different names*

### Comparing `jupyter-cpp-kernel-1.0.0a6/kernel_spec/logo-svg.svg` & `jupyter-cpp-kernel-1.0.0a7/kernel_spec/logo-svg.svg`

 * *Files identical despite different names*

### Comparing `jupyter-cpp-kernel-1.0.0a6/setup.cfg` & `jupyter-cpp-kernel-1.0.0a7/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [metadata]
 description-file = README.md
 name = jupyter-cpp-kernel
-version = 1.0.0a6
+version = 1.0.0a7
 author = shiroinekotfs (ft. Brendan Rius)
 author_email = shiroineko.tfs@gmail.com
 description = C++ kernel for Jupyter. Easily adopt and deploy for testing environment.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/shiroinekotfs/jupyter-cpp-kernel
 project_urls =
```

### Comparing `jupyter-cpp-kernel-1.0.0a6/setup.py` & `jupyter-cpp-kernel-1.0.0a7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 
 setup(name='jupyter-cpp-kernel',
-      version='1.0.0a6',
+      version='1.0.0a7',
       description='C++ 14 kernel for Jupyter',
       author='shiroinekotfs',
       author_email='shiroineko.tfs@gmail.com',
       license='MIT',
       classifiers=[
         'Programming Language :: Python :: 3',
         'Programming Language :: C++',
```

### Comparing `jupyter-cpp-kernel-1.0.0a6/share/cpp_header/check_cpp.hpp` & `jupyter-cpp-kernel-1.0.0a7/share/cpp_header/check_cpp.hpp`

 * *Files identical despite different names*

