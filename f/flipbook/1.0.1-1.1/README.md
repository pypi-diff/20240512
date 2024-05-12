# Comparing `tmp/flipbook-1.0.1.tar.gz` & `tmp/flipbook-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flipbook-1.0.1.tar", last modified: Tue Jan  9 02:43:44 2024, max compression
+gzip compressed data, was "flipbook-1.1.tar", last modified: Sun May 12 10:43:38 2024, max compression
```

## Comparing `flipbook-1.0.1.tar` & `flipbook-1.1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 weisburd   (502) staff       (20)        0 2024-01-09 02:43:44.918723 flipbook-1.0.1/
--rw-r--r--   0 weisburd   (502) staff       (20)     1060 2021-04-01 18:19:14.000000 flipbook-1.0.1/LICENSE
--rw-r--r--   0 weisburd   (502) staff       (20)     6587 2024-01-09 02:43:44.918285 flipbook-1.0.1/PKG-INFO
--rw-r--r--   0 weisburd   (502) staff       (20)     5587 2024-01-03 12:37:44.000000 flipbook-1.0.1/README.md
-drwxr-xr-x   0 weisburd   (502) staff       (20)        0 2024-01-09 02:43:44.879825 flipbook-1.0.1/flipbook/
--rw-r--r--   0 weisburd   (502) staff       (20)    19523 2024-01-03 17:46:16.000000 flipbook-1.0.1/flipbook/__init__.py
--rw-r--r--   0 weisburd   (502) staff       (20)       64 2021-09-15 14:02:24.000000 flipbook-1.0.1/flipbook/__main__.py
--rw-r--r--   0 weisburd   (502) staff       (20)     5391 2023-10-11 13:55:32.000000 flipbook-1.0.1/flipbook/data_page.py
--rw-r--r--   0 weisburd   (502) staff       (20)     2458 2023-12-23 23:34:18.000000 flipbook-1.0.1/flipbook/main_list.py
--rw-r--r--   0 weisburd   (502) staff       (20)     2859 2021-08-24 02:49:47.000000 flipbook-1.0.1/flipbook/save.py
-drwxr-xr-x   0 weisburd   (502) staff       (20)        0 2024-01-09 02:43:44.873858 flipbook-1.0.1/flipbook/static/
-drwxr-xr-x   0 weisburd   (502) staff       (20)        0 2024-01-09 02:43:44.884597 flipbook-1.0.1/flipbook/static/css/
--rw-r--r--   0 weisburd   (502) staff       (20)     6535 2023-01-15 18:16:35.000000 flipbook-1.0.1/flipbook/static/css/datatables.min.css
--rw-r--r--   0 weisburd   (502) staff       (20)   628536 2023-01-15 18:13:29.000000 flipbook-1.0.1/flipbook/static/css/semantic.min.css
-drwxr-xr-x   0 weisburd   (502) staff       (20)        0 2024-01-09 02:43:44.872973 flipbook-1.0.1/flipbook/static/css/themes/
-drwxr-xr-x   0 weisburd   (502) staff       (20)        0 2024-01-09 02:43:44.873191 flipbook-1.0.1/flipbook/static/css/themes/default/
-drwxr-xr-x   0 weisburd   (502) staff       (20)        0 2024-01-09 02:43:44.873400 flipbook-1.0.1/flipbook/static/css/themes/default/assets/
-drwxr-xr-x   0 weisburd   (502) staff       (20)        0 2024-01-09 02:43:44.892472 flipbook-1.0.1/flipbook/static/css/themes/default/assets/fonts/
--rw-r--r--   0 weisburd   (502) staff       (20)   105784 2023-01-15 18:31:14.000000 flipbook-1.0.1/flipbook/static/css/themes/default/assets/fonts/icons.ttf
--rw-r--r--   0 weisburd   (502) staff       (20)    50524 2023-01-15 18:31:07.000000 flipbook-1.0.1/flipbook/static/css/themes/default/assets/fonts/icons.woff
--rw-r--r--   0 weisburd   (502) staff       (20)    40148 2023-01-15 18:30:56.000000 flipbook-1.0.1/flipbook/static/css/themes/default/assets/fonts/icons.woff2
-drwxr-xr-x   0 weisburd   (502) staff       (20)        0 2024-01-09 02:43:44.893855 flipbook-1.0.1/flipbook/static/images/
--rw-r--r--   0 weisburd   (502) staff       (20)     5591 2021-09-28 17:09:18.000000 flipbook-1.0.1/flipbook/static/images/favicon.png
-drwxr-xr-x   0 weisburd   (502) staff       (20)        0 2024-01-09 02:43:44.911287 flipbook-1.0.1/flipbook/static/js/
--rw-r--r--   0 weisburd   (502) staff       (20)   328879 2023-01-15 18:17:35.000000 flipbook-1.0.1/flipbook/static/js/datatables.min.js
--rw-r--r--   0 weisburd   (502) staff       (20)    89476 2020-05-08 07:05:03.000000 flipbook-1.0.1/flipbook/static/js/jquery.min.js
--rw-r--r--   0 weisburd   (502) staff       (20)     1741 2020-05-04 16:11:46.000000 flipbook-1.0.1/flipbook/static/js/jquery.serialize-object.min.js
--rw-r--r--   0 weisburd   (502) staff       (20)   970387 2020-05-04 16:15:03.000000 flipbook-1.0.1/flipbook/static/js/pdfmake.min.js
--rw-r--r--   0 weisburd   (502) staff       (20)     4754 2020-05-04 16:15:40.000000 flipbook-1.0.1/flipbook/static/js/purl.min.js
--rw-r--r--   0 weisburd   (502) staff       (20)   275730 2023-01-15 18:13:38.000000 flipbook-1.0.1/flipbook/static/js/semantic.min.js
--rw-r--r--   0 weisburd   (502) staff       (20)   870284 2020-05-04 16:15:03.000000 flipbook-1.0.1/flipbook/static/js/vfs_fonts.js
-drwxr-xr-x   0 weisburd   (502) staff       (20)        0 2024-01-09 02:43:44.917071 flipbook-1.0.1/flipbook/templates/
--rw-r--r--   0 weisburd   (502) staff       (20)    16123 2023-10-11 14:00:48.000000 flipbook-1.0.1/flipbook/templates/data_page.html
--rw-r--r--   0 weisburd   (502) staff       (20)     5556 2023-01-15 18:18:44.000000 flipbook-1.0.1/flipbook/templates/main_list.html
--rw-r--r--   0 weisburd   (502) staff       (20)     6583 2021-11-01 11:55:01.000000 flipbook-1.0.1/flipbook/utils.py
-drwxr-xr-x   0 weisburd   (502) staff       (20)        0 2024-01-09 02:43:44.882839 flipbook-1.0.1/flipbook.egg-info/
--rw-r--r--   0 weisburd   (502) staff       (20)     6587 2024-01-09 02:43:44.000000 flipbook-1.0.1/flipbook.egg-info/PKG-INFO
--rw-r--r--   0 weisburd   (502) staff       (20)      949 2024-01-09 02:43:44.000000 flipbook-1.0.1/flipbook.egg-info/SOURCES.txt
--rw-r--r--   0 weisburd   (502) staff       (20)        1 2024-01-09 02:43:44.000000 flipbook-1.0.1/flipbook.egg-info/dependency_links.txt
--rw-r--r--   0 weisburd   (502) staff       (20)      117 2024-01-09 02:43:44.000000 flipbook-1.0.1/flipbook.egg-info/entry_points.txt
--rw-r--r--   0 weisburd   (502) staff       (20)      184 2024-01-09 02:43:44.000000 flipbook-1.0.1/flipbook.egg-info/requires.txt
--rw-r--r--   0 weisburd   (502) staff       (20)       38 2024-01-09 02:43:44.000000 flipbook-1.0.1/flipbook.egg-info/top_level.txt
--rw-r--r--   0 weisburd   (502) staff       (20)       38 2024-01-09 02:43:44.918833 flipbook-1.0.1/setup.cfg
--rw-r--r--   0 weisburd   (502) staff       (20)     2585 2024-01-09 02:43:05.000000 flipbook-1.0.1/setup.py
+drwxr-xr-x   0 weisburd   (502) staff       (20)        0 2024-05-12 10:43:38.112563 flipbook-1.1/
+-rw-r--r--   0 weisburd   (502) staff       (20)     1060 2021-04-01 18:19:14.000000 flipbook-1.1/LICENSE
+-rw-r--r--   0 weisburd   (502) staff       (20)     6949 2024-05-12 10:43:38.111296 flipbook-1.1/PKG-INFO
+-rw-r--r--   0 weisburd   (502) staff       (20)     5587 2024-01-03 12:37:44.000000 flipbook-1.1/README.md
+drwxr-xr-x   0 weisburd   (502) staff       (20)        0 2024-05-12 10:43:38.073797 flipbook-1.1/flipbook/
+-rw-r--r--   0 weisburd   (502) staff       (20)    19651 2024-05-12 10:42:50.000000 flipbook-1.1/flipbook/__init__.py
+-rw-r--r--   0 weisburd   (502) staff       (20)       64 2021-09-15 14:02:24.000000 flipbook-1.1/flipbook/__main__.py
+-rw-r--r--   0 weisburd   (502) staff       (20)     5437 2024-05-12 10:28:26.000000 flipbook-1.1/flipbook/data_page.py
+-rw-r--r--   0 weisburd   (502) staff       (20)     2458 2023-12-23 23:34:18.000000 flipbook-1.1/flipbook/main_list.py
+-rw-r--r--   0 weisburd   (502) staff       (20)     2859 2021-08-24 02:49:47.000000 flipbook-1.1/flipbook/save.py
+drwxr-xr-x   0 weisburd   (502) staff       (20)        0 2024-05-12 10:43:38.067422 flipbook-1.1/flipbook/static/
+drwxr-xr-x   0 weisburd   (502) staff       (20)        0 2024-05-12 10:43:38.083735 flipbook-1.1/flipbook/static/css/
+-rw-r--r--   0 weisburd   (502) staff       (20)     6535 2023-01-15 18:16:35.000000 flipbook-1.1/flipbook/static/css/datatables.min.css
+-rw-r--r--   0 weisburd   (502) staff       (20)   628536 2023-01-15 18:13:29.000000 flipbook-1.1/flipbook/static/css/semantic.min.css
+drwxr-xr-x   0 weisburd   (502) staff       (20)        0 2024-05-12 10:43:38.066477 flipbook-1.1/flipbook/static/css/themes/
+drwxr-xr-x   0 weisburd   (502) staff       (20)        0 2024-05-12 10:43:38.066745 flipbook-1.1/flipbook/static/css/themes/default/
+drwxr-xr-x   0 weisburd   (502) staff       (20)        0 2024-05-12 10:43:38.066938 flipbook-1.1/flipbook/static/css/themes/default/assets/
+drwxr-xr-x   0 weisburd   (502) staff       (20)        0 2024-05-12 10:43:38.090895 flipbook-1.1/flipbook/static/css/themes/default/assets/fonts/
+-rw-r--r--   0 weisburd   (502) staff       (20)   105784 2023-01-15 18:31:14.000000 flipbook-1.1/flipbook/static/css/themes/default/assets/fonts/icons.ttf
+-rw-r--r--   0 weisburd   (502) staff       (20)    50524 2023-01-15 18:31:07.000000 flipbook-1.1/flipbook/static/css/themes/default/assets/fonts/icons.woff
+-rw-r--r--   0 weisburd   (502) staff       (20)    40148 2023-01-15 18:30:56.000000 flipbook-1.1/flipbook/static/css/themes/default/assets/fonts/icons.woff2
+drwxr-xr-x   0 weisburd   (502) staff       (20)        0 2024-05-12 10:43:38.092038 flipbook-1.1/flipbook/static/images/
+-rw-r--r--   0 weisburd   (502) staff       (20)     5591 2021-09-28 17:09:18.000000 flipbook-1.1/flipbook/static/images/favicon.png
+drwxr-xr-x   0 weisburd   (502) staff       (20)        0 2024-05-12 10:43:38.103984 flipbook-1.1/flipbook/static/js/
+-rw-r--r--   0 weisburd   (502) staff       (20)   328879 2023-01-15 18:17:35.000000 flipbook-1.1/flipbook/static/js/datatables.min.js
+-rw-r--r--   0 weisburd   (502) staff       (20)    89476 2020-05-08 07:05:03.000000 flipbook-1.1/flipbook/static/js/jquery.min.js
+-rw-r--r--   0 weisburd   (502) staff       (20)     1741 2020-05-04 16:11:46.000000 flipbook-1.1/flipbook/static/js/jquery.serialize-object.min.js
+-rw-r--r--   0 weisburd   (502) staff       (20)   970387 2020-05-04 16:15:03.000000 flipbook-1.1/flipbook/static/js/pdfmake.min.js
+-rw-r--r--   0 weisburd   (502) staff       (20)     4754 2020-05-04 16:15:40.000000 flipbook-1.1/flipbook/static/js/purl.min.js
+-rw-r--r--   0 weisburd   (502) staff       (20)   275730 2023-01-15 18:13:38.000000 flipbook-1.1/flipbook/static/js/semantic.min.js
+-rw-r--r--   0 weisburd   (502) staff       (20)   870284 2020-05-04 16:15:03.000000 flipbook-1.1/flipbook/static/js/vfs_fonts.js
+drwxr-xr-x   0 weisburd   (502) staff       (20)        0 2024-05-12 10:43:38.109715 flipbook-1.1/flipbook/templates/
+-rw-r--r--   0 weisburd   (502) staff       (20)    16299 2024-05-12 10:40:45.000000 flipbook-1.1/flipbook/templates/data_page.html
+-rw-r--r--   0 weisburd   (502) staff       (20)     5556 2023-01-15 18:18:44.000000 flipbook-1.1/flipbook/templates/main_list.html
+-rw-r--r--   0 weisburd   (502) staff       (20)     6583 2021-11-01 11:55:01.000000 flipbook-1.1/flipbook/utils.py
+drwxr-xr-x   0 weisburd   (502) staff       (20)        0 2024-05-12 10:43:38.081593 flipbook-1.1/flipbook.egg-info/
+-rw-r--r--   0 weisburd   (502) staff       (20)     6949 2024-05-12 10:43:37.000000 flipbook-1.1/flipbook.egg-info/PKG-INFO
+-rw-r--r--   0 weisburd   (502) staff       (20)      949 2024-05-12 10:43:37.000000 flipbook-1.1/flipbook.egg-info/SOURCES.txt
+-rw-r--r--   0 weisburd   (502) staff       (20)        1 2024-05-12 10:43:37.000000 flipbook-1.1/flipbook.egg-info/dependency_links.txt
+-rw-r--r--   0 weisburd   (502) staff       (20)      117 2024-05-12 10:43:37.000000 flipbook-1.1/flipbook.egg-info/entry_points.txt
+-rw-r--r--   0 weisburd   (502) staff       (20)      184 2024-05-12 10:43:37.000000 flipbook-1.1/flipbook.egg-info/requires.txt
+-rw-r--r--   0 weisburd   (502) staff       (20)       38 2024-05-12 10:43:37.000000 flipbook-1.1/flipbook.egg-info/top_level.txt
+-rw-r--r--   0 weisburd   (502) staff       (20)       38 2024-05-12 10:43:38.112789 flipbook-1.1/setup.cfg
+-rw-r--r--   0 weisburd   (502) staff       (20)     2583 2024-05-12 10:41:12.000000 flipbook-1.1/setup.py
```

### Comparing `flipbook-1.0.1/LICENSE` & `flipbook-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `flipbook-1.0.1/PKG-INFO` & `flipbook-1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flipbook
-Version: 1.0.1
+Version: 1.1
 Summary: Starts a simple image server that lets you quickly flip through image files from a local directory using your web browser and optionally answering customizable questions about each one
 Home-page: https://github.com/broadinstitute/flipbook
 License: MIT
 Keywords: curation,NGS,sequencing,STRs,REviewer,read visualization,machine learning
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -14,14 +14,26 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: configargparse>=1.5.5
+Requires-Dist: flask-cors>=4.0.0
+Requires-Dist: gunicorn>=21.2.0
+Requires-Dist: jinja2>=3.1.2
+Requires-Dist: openpyxl>=3.1.1
+Requires-Dist: pandas>=2.0.3
+Requires-Dist: requests>=2.31.0
+Requires-Dist: wcmatch>=8.4.1
+Requires-Dist: xlrd>=2.0.1
+Requires-Dist: xlwt>=1.3.0
+Requires-Dist: flask==2.1
+Requires-Dist: Werkzeug==2.0.0
 
 ## FlipBook
 
 This tool provides a simple user interface for quickly flipping through images stored in some directory on your computer.
 It also optionally shows a form where you can take notes or answer questions about each image or set of images.
 
 ### Example uses:
```

### Comparing `flipbook-1.0.1/README.md` & `flipbook-1.1/README.md`

 * *Files identical despite different names*

### Comparing `flipbook-1.0.1/flipbook/__init__.py` & `flipbook-1.1/flipbook/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,14 +60,15 @@
                "causes FlipBook to write out a set of static html pages for all the images it finds and then exit. "
                "The generated pages can then be viewed in a browser, uploaded to some other web server (such as "
                "GitHub Pages, embedded in another existing website, etc. The generated web pages are identical to "
                "the standard FlipBook user interface except they don't contain the forms for entering responses about "
                "each image - and so just allow flipping through the images.")
 
 p.add_argument("-z", "--zoom", type=float, help="Optional zoom factor for images. This can be > or < 1.0")
+p.add_argument("--scroll-to-image", action="store_true", help="Automatically scroll to the image after opening the data page.")
 
 #p.add_argument("-c", "--config-file", help="Path of yaml config file", env_var="FLIPBOOK_CONFIG_FILE")
 p.add_argument("-v", "--verbose", action='count', default=0, help="Print more info")
 p.add_argument("--host", default="127.0.0.1", env_var="HOST", help="Listen for connections on this hostname or IP")
 p.add_argument("-p", "--port", default="8080", env_var="PORT", type=int, help="Listen for connections on this port")
 p.add_argument("--dev-mode", action="store_true", env_var="DEV", help="Run server in developer mode so it reloads "
                "html templates and source code if they're changed")
```

### Comparing `flipbook-1.0.1/flipbook/data_page.py` & `flipbook-1.1/flipbook/data_page.py`

 * *Files 3% similar despite different names*

```diff
@@ -123,11 +123,12 @@
         get_data_page_url=get_data_page_url if not is_static_website else get_static_data_page_url,
         form_schema=FORM_SCHEMA,
         form_radio_button_keyboard_shortcuts=FORM_RADIO_BUTTON_KEYBOARD_SHORTCUTS,
         form_responses=FORM_RESPONSES.get(relative_dir, {}),
         is_static_website=is_static_website,
         show_one_key_per_line=args.show_one_key_per_line,
         zoom=args.zoom,
+        scroll_to_image=args.scroll_to_image,
     )
 
     return Response(html, mimetype='text/html')
```

### Comparing `flipbook-1.0.1/flipbook/main_list.py` & `flipbook-1.1/flipbook/main_list.py`

 * *Files identical despite different names*

### Comparing `flipbook-1.0.1/flipbook/save.py` & `flipbook-1.1/flipbook/save.py`

 * *Files identical despite different names*

### Comparing `flipbook-1.0.1/flipbook/static/css/datatables.min.css` & `flipbook-1.1/flipbook/static/css/datatables.min.css`

 * *Files identical despite different names*

### Comparing `flipbook-1.0.1/flipbook/static/css/semantic.min.css` & `flipbook-1.1/flipbook/static/css/semantic.min.css`

 * *Files identical despite different names*

### Comparing `flipbook-1.0.1/flipbook/static/css/themes/default/assets/fonts/icons.ttf` & `flipbook-1.1/flipbook/static/css/themes/default/assets/fonts/icons.ttf`

 * *Files identical despite different names*

### Comparing `flipbook-1.0.1/flipbook/static/css/themes/default/assets/fonts/icons.woff` & `flipbook-1.1/flipbook/static/css/themes/default/assets/fonts/icons.woff`

 * *Files identical despite different names*

### Comparing `flipbook-1.0.1/flipbook/static/css/themes/default/assets/fonts/icons.woff2` & `flipbook-1.1/flipbook/static/css/themes/default/assets/fonts/icons.woff2`

 * *Files identical despite different names*

### Comparing `flipbook-1.0.1/flipbook/static/images/favicon.png` & `flipbook-1.1/flipbook/static/images/favicon.png`

 * *Files identical despite different names*

### Comparing `flipbook-1.0.1/flipbook/static/js/datatables.min.js` & `flipbook-1.1/flipbook/static/js/datatables.min.js`

 * *Files identical despite different names*

### Comparing `flipbook-1.0.1/flipbook/static/js/jquery.min.js` & `flipbook-1.1/flipbook/static/js/jquery.min.js`

 * *Files identical despite different names*

### Comparing `flipbook-1.0.1/flipbook/static/js/jquery.serialize-object.min.js` & `flipbook-1.1/flipbook/static/js/jquery.serialize-object.min.js`

 * *Files identical despite different names*

### Comparing `flipbook-1.0.1/flipbook/static/js/pdfmake.min.js` & `flipbook-1.1/flipbook/static/js/pdfmake.min.js`

 * *Files identical despite different names*

### Comparing `flipbook-1.0.1/flipbook/static/js/purl.min.js` & `flipbook-1.1/flipbook/static/js/purl.min.js`

 * *Files identical despite different names*

### Comparing `flipbook-1.0.1/flipbook/static/js/semantic.min.js` & `flipbook-1.1/flipbook/static/js/semantic.min.js`

 * *Files identical despite different names*

### Comparing `flipbook-1.0.1/flipbook/static/js/vfs_fonts.js` & `flipbook-1.1/flipbook/static/js/vfs_fonts.js`

 * *Files identical despite different names*

### Comparing `flipbook-1.0.1/flipbook/templates/data_page.html` & `flipbook-1.1/flipbook/templates/data_page.html`

 * *Files 5% similar despite different names*

```diff
@@ -332,10 +332,15 @@
         }
 
         // prevent arrow keys from selecting radio buttons
         if (event.keyCode >= 37 && event.keyCode <= 40 && (event.target.tagName || '').toLowerCase() == 'input' && event.target.type == 'radio') {
           return false
         }
       })
+
+      // optionally scroll to image
+      {% if scroll_to_image %}
+        $('html,body').animate({scrollTop: $("a[name='section1']").offset().top},"fast");
+      {% endif %}
     </script>
 </body>
 </html>
```

### Comparing `flipbook-1.0.1/flipbook/templates/main_list.html` & `flipbook-1.1/flipbook/templates/main_list.html`

 * *Files identical despite different names*

### Comparing `flipbook-1.0.1/flipbook/utils.py` & `flipbook-1.1/flipbook/utils.py`

 * *Files identical despite different names*

### Comparing `flipbook-1.0.1/flipbook.egg-info/PKG-INFO` & `flipbook-1.1/flipbook.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flipbook
-Version: 1.0.1
+Version: 1.1
 Summary: Starts a simple image server that lets you quickly flip through image files from a local directory using your web browser and optionally answering customizable questions about each one
 Home-page: https://github.com/broadinstitute/flipbook
 License: MIT
 Keywords: curation,NGS,sequencing,STRs,REviewer,read visualization,machine learning
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -14,14 +14,26 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: configargparse>=1.5.5
+Requires-Dist: flask-cors>=4.0.0
+Requires-Dist: gunicorn>=21.2.0
+Requires-Dist: jinja2>=3.1.2
+Requires-Dist: openpyxl>=3.1.1
+Requires-Dist: pandas>=2.0.3
+Requires-Dist: requests>=2.31.0
+Requires-Dist: wcmatch>=8.4.1
+Requires-Dist: xlrd>=2.0.1
+Requires-Dist: xlwt>=1.3.0
+Requires-Dist: flask==2.1
+Requires-Dist: Werkzeug==2.0.0
 
 ## FlipBook
 
 This tool provides a simple user interface for quickly flipping through images stored in some directory on your computer.
 It also optionally shows a form where you can take notes or answer questions about each image or set of images.
 
 ### Example uses:
```

### Comparing `flipbook-1.0.1/flipbook.egg-info/SOURCES.txt` & `flipbook-1.1/flipbook.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flipbook-1.0.1/setup.py` & `flipbook-1.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     # when starting the server, so use a previous version of flask and Werkzeug
     "flask==2.1",
     "Werkzeug==2.0.0",
 ]
 
 setup(
     name='flipbook',
-    version="1.0.1",
+    version="1.1",
     description="Starts a simple image server that lets you quickly flip through image files from a local directory "
                 "using your web browser and optionally answering customizable questions about each one",
     install_requires=install_requires,
     entry_points = {
         'console_scripts': [
             'flipbook = flipbook:main',
             'compare_flipbook_form_response_tables = compare_form_response_tables:main',
```

