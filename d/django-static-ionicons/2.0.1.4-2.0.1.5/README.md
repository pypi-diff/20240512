# Comparing `tmp/django-static-ionicons-2.0.1.4.tar.gz` & `tmp/django-static-ionicons-2.0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-static-ionicons-2.0.1.4.tar", last modified: Fri Sep 15 08:29:07 2023, max compression
+gzip compressed data, was "django-static-ionicons-2.0.1.5.tar", last modified: Sun May 12 12:43:24 2024, max compression
```

## Comparing `django-static-ionicons-2.0.1.4.tar` & `django-static-ionicons-2.0.1.5.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 test       (501) staff       (20)        0 2023-09-15 08:29:07.106844 django-static-ionicons-2.0.1.4/
--rw-r--r--   0 test       (501) staff       (20)     1067 2023-09-15 08:25:46.000000 django-static-ionicons-2.0.1.4/LICENSE
--rw-r--r--   0 test       (501) staff       (20)      195 2023-09-15 08:25:46.000000 django-static-ionicons-2.0.1.4/MANIFEST.in
--rw-r--r--   0 test       (501) staff       (20)     1353 2023-09-15 08:29:07.106735 django-static-ionicons-2.0.1.4/PKG-INFO
--rw-r--r--   0 test       (501) staff       (20)      665 2023-09-15 08:28:41.000000 django-static-ionicons-2.0.1.4/README.md
-drwxr-xr-x   0 test       (501) staff       (20)        0 2023-09-15 08:29:07.104672 django-static-ionicons-2.0.1.4/django_static_ionicons/
--rw-r--r--   0 test       (501) staff       (20)        0 2023-09-15 08:25:46.000000 django-static-ionicons-2.0.1.4/django_static_ionicons/__init__.py
--rw-r--r--   0 test       (501) staff       (20)        0 2023-09-15 08:25:46.000000 django-static-ionicons-2.0.1.4/django_static_ionicons/admin.py
--rw-r--r--   0 test       (501) staff       (20)        0 2023-09-15 08:25:46.000000 django-static-ionicons-2.0.1.4/django_static_ionicons/apps.py
-drwxr-xr-x   0 test       (501) staff       (20)        0 2023-09-15 08:29:07.105343 django-static-ionicons-2.0.1.4/django_static_ionicons/migrations/
--rw-r--r--   0 test       (501) staff       (20)        0 2023-09-15 08:25:46.000000 django-static-ionicons-2.0.1.4/django_static_ionicons/migrations/__init__.py
--rw-r--r--   0 test       (501) staff       (20)        0 2023-09-15 08:25:46.000000 django-static-ionicons-2.0.1.4/django_static_ionicons/models.py
-drwxr-xr-x   0 test       (501) staff       (20)        0 2023-09-15 08:29:07.103344 django-static-ionicons-2.0.1.4/django_static_ionicons/static/
-drwxr-xr-x   0 test       (501) staff       (20)        0 2023-09-15 08:29:07.103442 django-static-ionicons-2.0.1.4/django_static_ionicons/static/ionicons/
-drwxr-xr-x   0 test       (501) staff       (20)        0 2023-09-15 08:29:07.105582 django-static-ionicons-2.0.1.4/django_static_ionicons/static/ionicons/css/
--rw-r--r--   0 test       (501) staff       (20)    57193 2023-09-15 08:25:46.000000 django-static-ionicons-2.0.1.4/django_static_ionicons/static/ionicons/css/ionicons.css
--rw-r--r--   0 test       (501) staff       (20)    51284 2023-09-15 08:25:46.000000 django-static-ionicons-2.0.1.4/django_static_ionicons/static/ionicons/css/ionicons.min.css
-drwxr-xr-x   0 test       (501) staff       (20)        0 2023-09-15 08:29:07.106494 django-static-ionicons-2.0.1.4/django_static_ionicons/static/ionicons/fonts/
--rw-r--r--   0 test       (501) staff       (20)   120724 2023-09-15 08:25:46.000000 django-static-ionicons-2.0.1.4/django_static_ionicons/static/ionicons/fonts/ionicons.eot
--rw-r--r--   0 test       (501) staff       (20)   333834 2023-09-15 08:25:46.000000 django-static-ionicons-2.0.1.4/django_static_ionicons/static/ionicons/fonts/ionicons.svg
--rw-r--r--   0 test       (501) staff       (20)   188508 2023-09-15 08:25:46.000000 django-static-ionicons-2.0.1.4/django_static_ionicons/static/ionicons/fonts/ionicons.ttf
--rw-r--r--   0 test       (501) staff       (20)    67904 2023-09-15 08:25:46.000000 django-static-ionicons-2.0.1.4/django_static_ionicons/static/ionicons/fonts/ionicons.woff
--rw-r--r--   0 test       (501) staff       (20)        0 2023-09-15 08:25:46.000000 django-static-ionicons-2.0.1.4/django_static_ionicons/tests.py
--rw-r--r--   0 test       (501) staff       (20)        0 2023-09-15 08:25:46.000000 django-static-ionicons-2.0.1.4/django_static_ionicons/views.py
-drwxr-xr-x   0 test       (501) staff       (20)        0 2023-09-15 08:29:07.105225 django-static-ionicons-2.0.1.4/django_static_ionicons.egg-info/
--rw-r--r--   0 test       (501) staff       (20)     1353 2023-09-15 08:29:07.000000 django-static-ionicons-2.0.1.4/django_static_ionicons.egg-info/PKG-INFO
--rw-r--r--   0 test       (501) staff       (20)      874 2023-09-15 08:29:07.000000 django-static-ionicons-2.0.1.4/django_static_ionicons.egg-info/SOURCES.txt
--rw-r--r--   0 test       (501) staff       (20)        1 2023-09-15 08:29:07.000000 django-static-ionicons-2.0.1.4/django_static_ionicons.egg-info/dependency_links.txt
--rw-r--r--   0 test       (501) staff       (20)        1 2023-09-15 08:29:07.000000 django-static-ionicons-2.0.1.4/django_static_ionicons.egg-info/not-zip-safe
--rw-r--r--   0 test       (501) staff       (20)       23 2023-09-15 08:29:07.000000 django-static-ionicons-2.0.1.4/django_static_ionicons.egg-info/top_level.txt
--rw-r--r--   0 test       (501) staff       (20)        0 2023-09-15 08:25:46.000000 django-static-ionicons-2.0.1.4/requirements.txt
--rw-r--r--   0 test       (501) staff       (20)       38 2023-09-15 08:29:07.106880 django-static-ionicons-2.0.1.4/setup.cfg
--rw-r--r--   0 test       (501) staff       (20)     1518 2023-09-15 08:27:40.000000 django-static-ionicons-2.0.1.4/setup.py
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-12 12:43:24.905355 django-static-ionicons-2.0.1.5/
+-rw-r--r--   0 test       (501) staff       (20)     1036 2024-05-12 12:40:49.000000 django-static-ionicons-2.0.1.5/LICENSE
+-rw-r--r--   0 test       (501) staff       (20)      195 2023-09-15 08:25:46.000000 django-static-ionicons-2.0.1.5/MANIFEST.in
+-rw-r--r--   0 test       (501) staff       (20)     1292 2024-05-12 12:43:24.905222 django-static-ionicons-2.0.1.5/PKG-INFO
+-rw-r--r--   0 test       (501) staff       (20)      643 2024-05-12 12:41:49.000000 django-static-ionicons-2.0.1.5/README.md
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-12 12:43:24.900172 django-static-ionicons-2.0.1.5/django_static_ionicons/
+-rw-r--r--   0 test       (501) staff       (20)        0 2023-09-15 08:25:46.000000 django-static-ionicons-2.0.1.5/django_static_ionicons/__init__.py
+-rw-r--r--   0 test       (501) staff       (20)        0 2023-09-15 08:25:46.000000 django-static-ionicons-2.0.1.5/django_static_ionicons/admin.py
+-rw-r--r--   0 test       (501) staff       (20)        0 2023-09-15 08:25:46.000000 django-static-ionicons-2.0.1.5/django_static_ionicons/apps.py
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-12 12:43:24.900920 django-static-ionicons-2.0.1.5/django_static_ionicons/migrations/
+-rw-r--r--   0 test       (501) staff       (20)        0 2023-09-15 08:25:46.000000 django-static-ionicons-2.0.1.5/django_static_ionicons/migrations/__init__.py
+-rw-r--r--   0 test       (501) staff       (20)        0 2023-09-15 08:25:46.000000 django-static-ionicons-2.0.1.5/django_static_ionicons/models.py
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-12 12:43:24.898678 django-static-ionicons-2.0.1.5/django_static_ionicons/static/
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-12 12:43:24.898795 django-static-ionicons-2.0.1.5/django_static_ionicons/static/ionicons/
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-12 12:43:24.901755 django-static-ionicons-2.0.1.5/django_static_ionicons/static/ionicons/css/
+-rw-r--r--   0 test       (501) staff       (20)    57193 2023-09-15 08:25:46.000000 django-static-ionicons-2.0.1.5/django_static_ionicons/static/ionicons/css/ionicons.css
+-rw-r--r--   0 test       (501) staff       (20)    51284 2023-09-15 08:25:46.000000 django-static-ionicons-2.0.1.5/django_static_ionicons/static/ionicons/css/ionicons.min.css
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-12 12:43:24.904378 django-static-ionicons-2.0.1.5/django_static_ionicons/static/ionicons/fonts/
+-rw-r--r--   0 test       (501) staff       (20)   120724 2023-09-15 08:25:46.000000 django-static-ionicons-2.0.1.5/django_static_ionicons/static/ionicons/fonts/ionicons.eot
+-rw-r--r--   0 test       (501) staff       (20)   333834 2023-09-15 08:25:46.000000 django-static-ionicons-2.0.1.5/django_static_ionicons/static/ionicons/fonts/ionicons.svg
+-rw-r--r--   0 test       (501) staff       (20)   188508 2023-09-15 08:25:46.000000 django-static-ionicons-2.0.1.5/django_static_ionicons/static/ionicons/fonts/ionicons.ttf
+-rw-r--r--   0 test       (501) staff       (20)    67904 2023-09-15 08:25:46.000000 django-static-ionicons-2.0.1.5/django_static_ionicons/static/ionicons/fonts/ionicons.woff
+-rw-r--r--   0 test       (501) staff       (20)        0 2023-09-15 08:25:46.000000 django-static-ionicons-2.0.1.5/django_static_ionicons/tests.py
+-rw-r--r--   0 test       (501) staff       (20)        0 2023-09-15 08:25:46.000000 django-static-ionicons-2.0.1.5/django_static_ionicons/views.py
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-12 12:43:24.900776 django-static-ionicons-2.0.1.5/django_static_ionicons.egg-info/
+-rw-r--r--   0 test       (501) staff       (20)     1292 2024-05-12 12:43:24.000000 django-static-ionicons-2.0.1.5/django_static_ionicons.egg-info/PKG-INFO
+-rw-r--r--   0 test       (501) staff       (20)      874 2024-05-12 12:43:24.000000 django-static-ionicons-2.0.1.5/django_static_ionicons.egg-info/SOURCES.txt
+-rw-r--r--   0 test       (501) staff       (20)        1 2024-05-12 12:43:24.000000 django-static-ionicons-2.0.1.5/django_static_ionicons.egg-info/dependency_links.txt
+-rw-r--r--   0 test       (501) staff       (20)        1 2024-05-12 12:43:24.000000 django-static-ionicons-2.0.1.5/django_static_ionicons.egg-info/not-zip-safe
+-rw-r--r--   0 test       (501) staff       (20)       23 2024-05-12 12:43:24.000000 django-static-ionicons-2.0.1.5/django_static_ionicons.egg-info/top_level.txt
+-rw-r--r--   0 test       (501) staff       (20)        0 2023-09-15 08:25:46.000000 django-static-ionicons-2.0.1.5/requirements.txt
+-rw-r--r--   0 test       (501) staff       (20)       38 2024-05-12 12:43:24.905410 django-static-ionicons-2.0.1.5/setup.cfg
+-rw-r--r--   0 test       (501) staff       (20)     1428 2024-05-12 12:43:22.000000 django-static-ionicons-2.0.1.5/setup.py
```

### Comparing `django-static-ionicons-2.0.1.4/LICENSE` & `django-static-ionicons-2.0.1.5/LICENSE`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 MIT License
 
-Copyright (c) 2017 zencore.cn
-
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `django-static-ionicons-2.0.1.4/PKG-INFO` & `django-static-ionicons-2.0.1.5/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: django-static-ionicons
-Version: 2.0.1.4
+Version: 2.0.1.5
 Summary: Django application contain ionicons static files.
+Home-page: UNKNOWN
 Author: Chen ZhiXing
-Author-email: chenzhixing@zencore.cn
 Maintainer: Chen ZhiXing
-Maintainer-email: chenzhixing@zencore.cn
 License: MIT
 Keywords: django-static-ionicons
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Description-Content-Type: text/markdown
@@ -38,37 +38,43 @@
     "django_static_ionicons",
     ...
 ]
 ```
 
 ## Usage
 
-**app/templates/demo.html**
+*app/templates/demo.html*
 
-```
+```django
 {% load staticfiles %}
 
 <link rel="stylesheet" type="text/css" href="{% static "ionicons/css/ionicons.css" %}">
 ```
 
 ## Releases
 
-### v2.0.1 2017/12/21
+### v2.0.1
 
 - First release.
 
-### v2.0.1.1 2018/03/27
+### v2.0.1.1
 
 - Repackage.
 
-### v2.0.1.2 2020/02/26
+### v2.0.1.2
 
 - Add demo page.
 
-### v2.0.1.3 2020/09/02
+### v2.0.1.3
 
 - No depends on django.
 - Turn to the package as a pure static wrapper package.
 
-### v2.0.1.4 2023/09/15
+### v2.0.1.4
+
+- Doc update.
+
+### v2.0.1.5
 
 - Doc update.
+
+
```

### Comparing `django-static-ionicons-2.0.1.4/django_static_ionicons/static/ionicons/css/ionicons.css` & `django-static-ionicons-2.0.1.5/django_static_ionicons/static/ionicons/css/ionicons.css`

 * *Files identical despite different names*

### Comparing `django-static-ionicons-2.0.1.4/django_static_ionicons/static/ionicons/css/ionicons.min.css` & `django-static-ionicons-2.0.1.5/django_static_ionicons/static/ionicons/css/ionicons.min.css`

 * *Files identical despite different names*

### Comparing `django-static-ionicons-2.0.1.4/django_static_ionicons/static/ionicons/fonts/ionicons.eot` & `django-static-ionicons-2.0.1.5/django_static_ionicons/static/ionicons/fonts/ionicons.eot`

 * *Files identical despite different names*

### Comparing `django-static-ionicons-2.0.1.4/django_static_ionicons/static/ionicons/fonts/ionicons.svg` & `django-static-ionicons-2.0.1.5/django_static_ionicons/static/ionicons/fonts/ionicons.svg`

 * *Files identical despite different names*

### Comparing `django-static-ionicons-2.0.1.4/django_static_ionicons/static/ionicons/fonts/ionicons.ttf` & `django-static-ionicons-2.0.1.5/django_static_ionicons/static/ionicons/fonts/ionicons.ttf`

 * *Files identical despite different names*

### Comparing `django-static-ionicons-2.0.1.4/django_static_ionicons/static/ionicons/fonts/ionicons.woff` & `django-static-ionicons-2.0.1.5/django_static_ionicons/static/ionicons/fonts/ionicons.woff`

 * *Files identical despite different names*

### Comparing `django-static-ionicons-2.0.1.4/django_static_ionicons.egg-info/PKG-INFO` & `django-static-ionicons-2.0.1.5/django_static_ionicons.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: django-static-ionicons
-Version: 2.0.1.4
+Version: 2.0.1.5
 Summary: Django application contain ionicons static files.
+Home-page: UNKNOWN
 Author: Chen ZhiXing
-Author-email: chenzhixing@zencore.cn
 Maintainer: Chen ZhiXing
-Maintainer-email: chenzhixing@zencore.cn
 License: MIT
 Keywords: django-static-ionicons
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Description-Content-Type: text/markdown
@@ -38,37 +38,43 @@
     "django_static_ionicons",
     ...
 ]
 ```
 
 ## Usage
 
-**app/templates/demo.html**
+*app/templates/demo.html*
 
-```
+```django
 {% load staticfiles %}
 
 <link rel="stylesheet" type="text/css" href="{% static "ionicons/css/ionicons.css" %}">
 ```
 
 ## Releases
 
-### v2.0.1 2017/12/21
+### v2.0.1
 
 - First release.
 
-### v2.0.1.1 2018/03/27
+### v2.0.1.1
 
 - Repackage.
 
-### v2.0.1.2 2020/02/26
+### v2.0.1.2
 
 - Add demo page.
 
-### v2.0.1.3 2020/09/02
+### v2.0.1.3
 
 - No depends on django.
 - Turn to the package as a pure static wrapper package.
 
-### v2.0.1.4 2023/09/15
+### v2.0.1.4
+
+- Doc update.
+
+### v2.0.1.5
 
 - Doc update.
+
+
```

### Comparing `django-static-ionicons-2.0.1.4/django_static_ionicons.egg-info/SOURCES.txt` & `django-static-ionicons-2.0.1.5/django_static_ionicons.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-static-ionicons-2.0.1.4/setup.py` & `django-static-ionicons-2.0.1.5/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,22 +9,20 @@
 
 with open(os.path.join(here, "requirements.txt"), "r", encoding="utf-8") as fobj:
     requires = [x.strip() for x in fobj.readlines() if x.strip()]
 
 
 setup(
     name="django-static-ionicons",
-    version="2.0.1.4",
+    version="2.0.1.5",
     description="Django application contain ionicons static files.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Chen ZhiXing",
-    author_email="chenzhixing@zencore.cn",
     maintainer="Chen ZhiXing",
-    maintainer_email="chenzhixing@zencore.cn",
     license="MIT",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
```

