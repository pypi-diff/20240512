# Comparing `tmp/appmode-0.9.0.tar.gz` & `tmp/appmode-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "appmode-0.9.0.tar", last modified: Thu May 18 14:21:18 2023, max compression
+gzip compressed data, was "appmode-1.0.0.tar", last modified: Sun May 12 14:12:01 2024, max compression
```

## Comparing `appmode-0.9.0.tar` & `appmode-1.0.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-05-18 14:21:18.633572 appmode-0.9.0/
--rw-rw-r--   0 ole       (1000) ole       (1000)     1086 2023-05-18 11:58:38.000000 appmode-0.9.0/LICENSE.txt
--rw-rw-r--   0 ole       (1000) ole       (1000)      180 2023-05-18 11:58:38.000000 appmode-0.9.0/MANIFEST.in
--rw-rw-r--   0 ole       (1000) ole       (1000)      512 2023-05-18 14:21:18.633572 appmode-0.9.0/PKG-INFO
--rw-rw-r--   0 ole       (1000) ole       (1000)     3819 2023-05-18 14:01:34.000000 appmode-0.9.0/README.md
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-05-18 14:21:18.633572 appmode-0.9.0/appmode/
--rw-rw-r--   0 ole       (1000) ole       (1000)      331 2023-05-18 14:19:59.000000 appmode-0.9.0/appmode/__init__.py
--rw-rw-r--   0 ole       (1000) ole       (1000)      862 2023-05-18 11:58:38.000000 appmode-0.9.0/appmode/appmode.html
--rw-rw-r--   0 ole       (1000) ole       (1000)      789 2023-05-18 11:58:38.000000 appmode-0.9.0/appmode/appmode_bottom.css
--rw-rw-r--   0 ole       (1000) ole       (1000)      197 2023-05-18 11:58:38.000000 appmode-0.9.0/appmode/appmode_top.css
--rw-rw-r--   0 ole       (1000) ole       (1000)     7366 2023-05-18 12:09:02.000000 appmode-0.9.0/appmode/server_extension.py
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-05-18 14:21:18.633572 appmode-0.9.0/appmode/static/
--rw-rw-r--   0 ole       (1000) ole       (1000)     2528 2023-05-18 11:58:38.000000 appmode-0.9.0/appmode/static/gears.svg
--rw-rw-r--   0 ole       (1000) ole       (1000)     7157 2023-05-18 11:58:38.000000 appmode-0.9.0/appmode/static/main.js
-drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2023-05-18 14:21:18.633572 appmode-0.9.0/appmode.egg-info/
--rw-rw-r--   0 ole       (1000) ole       (1000)      512 2023-05-18 14:21:18.000000 appmode-0.9.0/appmode.egg-info/PKG-INFO
--rw-rw-r--   0 ole       (1000) ole       (1000)      364 2023-05-18 14:21:18.000000 appmode-0.9.0/appmode.egg-info/SOURCES.txt
--rw-rw-r--   0 ole       (1000) ole       (1000)        1 2023-05-18 14:21:18.000000 appmode-0.9.0/appmode.egg-info/dependency_links.txt
--rw-rw-r--   0 ole       (1000) ole       (1000)       12 2023-05-18 14:21:18.000000 appmode-0.9.0/appmode.egg-info/requires.txt
--rw-rw-r--   0 ole       (1000) ole       (1000)        8 2023-05-18 14:21:18.000000 appmode-0.9.0/appmode.egg-info/top_level.txt
--rw-rw-r--   0 ole       (1000) ole       (1000)       38 2023-05-18 14:21:18.633572 appmode-0.9.0/setup.cfg
--rw-rw-r--   0 ole       (1000) ole       (1000)     1366 2023-05-18 11:58:38.000000 appmode-0.9.0/setup.py
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2024-05-12 14:12:01.865690 appmode-1.0.0/
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1086 2024-05-12 14:06:49.000000 appmode-1.0.0/LICENSE
+-rw-rw-r--   0 ole       (1000) ole       (1000)      180 2024-05-12 12:45:27.000000 appmode-1.0.0/MANIFEST.in
+-rw-rw-r--   0 ole       (1000) ole       (1000)      508 2024-05-12 14:12:01.865690 appmode-1.0.0/PKG-INFO
+-rw-rw-r--   0 ole       (1000) ole       (1000)     3832 2024-05-12 14:06:49.000000 appmode-1.0.0/README.md
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2024-05-12 14:12:01.861690 appmode-1.0.0/appmode/
+-rw-rw-r--   0 ole       (1000) ole       (1000)      392 2024-05-12 14:06:49.000000 appmode-1.0.0/appmode/__init__.py
+-rw-rw-r--   0 ole       (1000) ole       (1000)      862 2024-05-12 12:45:27.000000 appmode-1.0.0/appmode/appmode.html
+-rw-rw-r--   0 ole       (1000) ole       (1000)      789 2024-05-12 12:45:27.000000 appmode-1.0.0/appmode/appmode_bottom.css
+-rw-rw-r--   0 ole       (1000) ole       (1000)      197 2024-05-12 12:45:27.000000 appmode-1.0.0/appmode/appmode_top.css
+-rw-rw-r--   0 ole       (1000) ole       (1000)     5731 2024-05-12 14:01:41.000000 appmode-1.0.0/appmode/server_extension.py
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2024-05-12 14:12:01.865690 appmode-1.0.0/appmode/static/
+-rw-rw-r--   0 ole       (1000) ole       (1000)     2528 2024-05-12 12:45:27.000000 appmode-1.0.0/appmode/static/gears.svg
+-rw-rw-r--   0 ole       (1000) ole       (1000)     7646 2024-05-12 12:49:17.000000 appmode-1.0.0/appmode/static/main.js
+drwxrwxr-x   0 ole       (1000) ole       (1000)        0 2024-05-12 14:12:01.861690 appmode-1.0.0/appmode.egg-info/
+-rw-rw-r--   0 ole       (1000) ole       (1000)      508 2024-05-12 14:12:01.000000 appmode-1.0.0/appmode.egg-info/PKG-INFO
+-rw-rw-r--   0 ole       (1000) ole       (1000)      360 2024-05-12 14:12:01.000000 appmode-1.0.0/appmode.egg-info/SOURCES.txt
+-rw-rw-r--   0 ole       (1000) ole       (1000)        1 2024-05-12 14:12:01.000000 appmode-1.0.0/appmode.egg-info/dependency_links.txt
+-rw-rw-r--   0 ole       (1000) ole       (1000)       13 2024-05-12 14:12:01.000000 appmode-1.0.0/appmode.egg-info/requires.txt
+-rw-rw-r--   0 ole       (1000) ole       (1000)        8 2024-05-12 14:12:01.000000 appmode-1.0.0/appmode.egg-info/top_level.txt
+-rw-rw-r--   0 ole       (1000) ole       (1000)       38 2024-05-12 14:12:01.865690 appmode-1.0.0/setup.cfg
+-rw-rw-r--   0 ole       (1000) ole       (1000)     1375 2024-05-12 14:06:49.000000 appmode-1.0.0/setup.py
```

### Comparing `appmode-0.9.0/LICENSE.txt` & `appmode-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `appmode-0.9.0/README.md` & `appmode-1.0.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -2,31 +2,31 @@
 
 **A Jupyter extensions that turns notebooks into web applications.**
 
 ![screenshots](./screenshots.png)
 
 ## Try it live
 
-[![Binder](https://mybinder.org/badge.svg)](https://mybinder.org/v2/gh/oschuett/appmode/master?urlpath=%2Fapps%2Fexample_app.ipynb)
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/oschuett/appmode/master?urlpath=%2Fapps%2Fexample_app.ipynb)
 
 Click the binder badge to try it live without installing anything. This will take you directly to the "app" version of the notebook.
 
 
 ## Installation
 
 If you use `conda`, you can install it as:
 ```
 conda install --channel conda-forge appmode
 ```
 
 If you use ``pip``, you can install it as:
 ```
 pip install appmode
-jupyter nbextension     enable --py --sys-prefix appmode
-jupyter serverextension enable --py --sys-prefix appmode
+jupyter nbclassic-extension enable --py --sys-prefix appmode
+jupyter server    extension enable --py --sys-prefix appmode
 ```
 
 If you want to use [mybinder](https://mybinder.org) add the following `environment.yml` file to your repository:
 ```
 channels:
   - conda-forge
 dependencies:
```

### Comparing `appmode-0.9.0/appmode/appmode.html` & `appmode-1.0.0/appmode/appmode.html`

 * *Files identical despite different names*

### Comparing `appmode-0.9.0/appmode/appmode_bottom.css` & `appmode-1.0.0/appmode/appmode_bottom.css`

 * *Files identical despite different names*

### Comparing `appmode-0.9.0/appmode/static/gears.svg` & `appmode-1.0.0/appmode/static/gears.svg`

 * *Files identical despite different names*

### Comparing `appmode-0.9.0/appmode/static/main.js` & `appmode-1.0.0/appmode/static/main.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -48,15 +48,17 @@
     //==========================================================================
     function goto_app_mode() {
         // kill Jupyter session
         Jupyter.notebook.session.delete();
 
         // build new URL
         var base_url = Jupyter.notebook.base_url;
-        var prefix = base_url + "notebooks/"
+        var nbclassic_path = document.nbclassicPath
+        if (nbclassic_path.charAt(0) == "/") nbclassic_path = nbclassic_path.substr(1) + "/";
+        var prefix = base_url + nbclassic_path + "notebooks/"
         var path = window.location.pathname.substring(prefix.length);
         var search = window.location.search;
         var scroll = "appmode_scroll=" + $('#site').scrollTop();
         if (search.search(/appmode_scroll=\d+/) != -1) {
             search = search.replace(/appmode_scroll=\d+/g, scroll);
         } else if (search.length == 0) {
             search = "?" + scroll;
@@ -68,17 +70,19 @@
         window.location.href = base_url + "apps/" + path + search;
     }
 
     //==========================================================================
     function goto_normal_mode() {
         // build new URL
         var base_url = Jupyter.notebook.base_url;
+        var nbclassic_path = document.nbclassicPath
+        if (nbclassic_path.charAt(0) == "/") nbclassic_path = nbclassic_path.substr(1) + "/";
         var prefix = base_url + "apps/"
         var path = window.location.pathname.substring(prefix.length);
-        var new_url = base_url + "notebooks/" + path + window.location.search;
+        var new_url = base_url + nbclassic_path + "notebooks/" + path + window.location.search;
 
         // goto new URL
         // Not using location.pathname as it might urlencode the path again
         window.location.href = new_url;
     }
 
     //==========================================================================
@@ -95,15 +99,17 @@
         }
     }
 
     //==========================================================================
     function initialize_step2() {
         // scroll to last position if in normal mode
         var base_url = Jupyter.notebook.base_url;
-        if (window.location.pathname.startsWith(base_url + "notebooks/")) {
+        var nbclassic_path = document.nbclassicPath
+        if (nbclassic_path.charAt(0) == "/") nbclassic_path = nbclassic_path.substr(1) + "/";
+        if (window.location.pathname.startsWith(base_url + nbclassic_path + "notebooks/")) {
             var url = window.location.href;
             var m = url.match(/appmode_scroll=(\d+)/);
             if (m)
                 $('#site').scrollTop(m[1]);
         }
 
         var nb = Jupyter.notebook;
```

### Comparing `appmode-0.9.0/setup.py` & `appmode-1.0.0/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -21,28 +21,28 @@
     author = 'Ole Schuett',
     author_email = 'ole.schuett@cp2k.org',
     url='http://github.com/oschuett/appmode',
     description='A Jupyter extensions that turns notebooks into web applications.',
 
     packages=["appmode"],
     include_package_data = True,
-    install_requires=['notebook>=5'],
-    python_requires='>=3.5',
+    install_requires=['nbclassic>=1'],
+    python_requires='>=3.7',
     data_files=[('share/jupyter/nbextensions/appmode', [
                     'appmode/static/main.js',
                     'appmode/static/gears.svg'
     ])],
 
     classifiers=[
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.5",
+        "Programming Language :: Python :: 3.7",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
 
 )
 
 print("\nPlease run the following commands to enable appmode:")
-print("  jupyter serverextension enable --py --sys-prefix appmode")
-print("  jupyter nbextension     enable --py --sys-prefix appmode")
+print("  jupyter nbclassic-extension enable --py --sys-prefix appmode")
+print("  jupyter server    extension enable --py --sys-prefix appmode")
 
 #EOF
```

