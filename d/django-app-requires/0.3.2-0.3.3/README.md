# Comparing `tmp/django-app-requires-0.3.2.tar.gz` & `tmp/django-app-requires-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-app-requires-0.3.2.tar", last modified: Wed Sep 13 07:29:05 2023, max compression
+gzip compressed data, was "django-app-requires-0.3.3.tar", last modified: Sun May 12 14:14:31 2024, max compression
```

## Comparing `django-app-requires-0.3.2.tar` & `django-app-requires-0.3.3.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 test       (501) staff       (20)        0 2023-09-13 07:29:05.853278 django-app-requires-0.3.2/
--rw-r--r--   0 test       (501) staff       (20)     1067 2022-06-01 13:01:41.000000 django-app-requires-0.3.2/LICENSE
--rw-r--r--   0 test       (501) staff       (20)      308 2022-09-13 02:41:33.000000 django-app-requires-0.3.2/MANIFEST.in
--rw-r--r--   0 test       (501) staff       (20)     3360 2023-09-13 07:29:05.853160 django-app-requires-0.3.2/PKG-INFO
--rw-r--r--   0 test       (501) staff       (20)     2477 2023-09-13 06:51:15.000000 django-app-requires-0.3.2/README.md
-drwxr-xr-x   0 test       (501) staff       (20)        0 2023-09-13 07:29:05.848954 django-app-requires-0.3.2/django_app_requires/
--rw-r--r--   0 test       (501) staff       (20)      100 2022-06-01 13:00:11.000000 django-app-requires-0.3.2/django_app_requires/__init__.py
--rw-r--r--   0 test       (501) staff       (20)     3331 2023-09-13 06:50:31.000000 django-app-requires-0.3.2/django_app_requires/utils.py
-drwxr-xr-x   0 test       (501) staff       (20)        0 2023-09-13 07:29:05.849745 django-app-requires-0.3.2/django_app_requires.egg-info/
--rw-r--r--   0 test       (501) staff       (20)     3360 2023-09-13 07:29:05.000000 django-app-requires-0.3.2/django_app_requires.egg-info/PKG-INFO
--rw-r--r--   0 test       (501) staff       (20)     1057 2023-09-13 07:29:05.000000 django-app-requires-0.3.2/django_app_requires.egg-info/SOURCES.txt
--rw-r--r--   0 test       (501) staff       (20)        1 2023-09-13 07:29:05.000000 django-app-requires-0.3.2/django_app_requires.egg-info/dependency_links.txt
--rw-r--r--   0 test       (501) staff       (20)        1 2023-09-13 07:29:05.000000 django-app-requires-0.3.2/django_app_requires.egg-info/not-zip-safe
--rw-r--r--   0 test       (501) staff       (20)       16 2023-09-13 07:29:05.000000 django-app-requires-0.3.2/django_app_requires.egg-info/requires.txt
--rw-r--r--   0 test       (501) staff       (20)       95 2023-09-13 07:29:05.000000 django-app-requires-0.3.2/django_app_requires.egg-info/top_level.txt
-drwxr-xr-x   0 test       (501) staff       (20)        0 2023-09-13 07:29:05.850937 django-app-requires-0.3.2/django_app_requires_first_placeholder/
--rw-r--r--   0 test       (501) staff       (20)      107 2022-06-05 13:04:20.000000 django-app-requires-0.3.2/django_app_requires_first_placeholder/__init__.py
--rw-r--r--   0 test       (501) staff       (20)       63 2022-06-05 13:03:42.000000 django-app-requires-0.3.2/django_app_requires_first_placeholder/admin.py
--rw-r--r--   0 test       (501) staff       (20)     2408 2023-09-13 06:50:46.000000 django-app-requires-0.3.2/django_app_requires_first_placeholder/apps.py
-drwxr-xr-x   0 test       (501) staff       (20)        0 2023-09-13 07:29:05.851433 django-app-requires-0.3.2/django_app_requires_first_placeholder/migrations/
--rw-r--r--   0 test       (501) staff       (20)        0 2022-06-05 13:03:42.000000 django-app-requires-0.3.2/django_app_requires_first_placeholder/migrations/__init__.py
--rw-r--r--   0 test       (501) staff       (20)       57 2022-06-05 13:03:42.000000 django-app-requires-0.3.2/django_app_requires_first_placeholder/models.py
--rw-r--r--   0 test       (501) staff       (20)       60 2022-06-05 13:03:42.000000 django-app-requires-0.3.2/django_app_requires_first_placeholder/tests.py
--rw-r--r--   0 test       (501) staff       (20)       63 2022-06-05 13:03:42.000000 django-app-requires-0.3.2/django_app_requires_first_placeholder/views.py
-drwxr-xr-x   0 test       (501) staff       (20)        0 2023-09-13 07:29:05.852572 django-app-requires-0.3.2/django_app_requires_last_placeholder/
--rw-r--r--   0 test       (501) staff       (20)      105 2022-06-05 07:49:41.000000 django-app-requires-0.3.2/django_app_requires_last_placeholder/__init__.py
--rw-r--r--   0 test       (501) staff       (20)       63 2022-06-05 07:46:24.000000 django-app-requires-0.3.2/django_app_requires_last_placeholder/admin.py
--rw-r--r--   0 test       (501) staff       (20)      799 2023-09-13 06:50:39.000000 django-app-requires-0.3.2/django_app_requires_last_placeholder/apps.py
-drwxr-xr-x   0 test       (501) staff       (20)        0 2023-09-13 07:29:05.853001 django-app-requires-0.3.2/django_app_requires_last_placeholder/migrations/
--rw-r--r--   0 test       (501) staff       (20)        0 2022-06-05 07:46:24.000000 django-app-requires-0.3.2/django_app_requires_last_placeholder/migrations/__init__.py
--rw-r--r--   0 test       (501) staff       (20)       57 2022-06-05 07:46:24.000000 django-app-requires-0.3.2/django_app_requires_last_placeholder/models.py
--rw-r--r--   0 test       (501) staff       (20)       60 2022-06-05 07:46:24.000000 django-app-requires-0.3.2/django_app_requires_last_placeholder/tests.py
--rw-r--r--   0 test       (501) staff       (20)       63 2022-06-05 07:46:24.000000 django-app-requires-0.3.2/django_app_requires_last_placeholder/views.py
--rw-r--r--   0 test       (501) staff       (20)       20 2023-09-13 06:50:51.000000 django-app-requires-0.3.2/requirements.txt
--rw-r--r--   0 test       (501) staff       (20)       38 2023-09-13 07:29:05.853314 django-app-requires-0.3.2/setup.cfg
--rw-r--r--   0 test       (501) staff       (20)     1705 2023-09-13 06:53:47.000000 django-app-requires-0.3.2/setup.py
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-12 14:14:31.453507 django-app-requires-0.3.3/
+-rw-r--r--   0 test       (501) staff       (20)     1036 2024-05-12 14:09:22.000000 django-app-requires-0.3.3/LICENSE
+-rw-r--r--   0 test       (501) staff       (20)      308 2022-09-13 02:41:33.000000 django-app-requires-0.3.3/MANIFEST.in
+-rw-r--r--   0 test       (501) staff       (20)     3348 2024-05-12 14:14:31.453393 django-app-requires-0.3.3/PKG-INFO
+-rw-r--r--   0 test       (501) staff       (20)     2504 2024-05-12 14:09:14.000000 django-app-requires-0.3.3/README.md
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-12 14:14:31.450680 django-app-requires-0.3.3/django_app_requires/
+-rw-r--r--   0 test       (501) staff       (20)      100 2022-06-01 13:00:11.000000 django-app-requires-0.3.3/django_app_requires/__init__.py
+-rw-r--r--   0 test       (501) staff       (20)     3331 2023-09-13 06:50:31.000000 django-app-requires-0.3.3/django_app_requires/utils.py
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-12 14:14:31.451412 django-app-requires-0.3.3/django_app_requires.egg-info/
+-rw-r--r--   0 test       (501) staff       (20)     3348 2024-05-12 14:14:31.000000 django-app-requires-0.3.3/django_app_requires.egg-info/PKG-INFO
+-rw-r--r--   0 test       (501) staff       (20)     1057 2024-05-12 14:14:31.000000 django-app-requires-0.3.3/django_app_requires.egg-info/SOURCES.txt
+-rw-r--r--   0 test       (501) staff       (20)        1 2024-05-12 14:14:31.000000 django-app-requires-0.3.3/django_app_requires.egg-info/dependency_links.txt
+-rw-r--r--   0 test       (501) staff       (20)        1 2024-05-12 14:14:31.000000 django-app-requires-0.3.3/django_app_requires.egg-info/not-zip-safe
+-rw-r--r--   0 test       (501) staff       (20)       16 2024-05-12 14:14:31.000000 django-app-requires-0.3.3/django_app_requires.egg-info/requires.txt
+-rw-r--r--   0 test       (501) staff       (20)       95 2024-05-12 14:14:31.000000 django-app-requires-0.3.3/django_app_requires.egg-info/top_level.txt
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-12 14:14:31.452248 django-app-requires-0.3.3/django_app_requires_first_placeholder/
+-rw-r--r--   0 test       (501) staff       (20)      107 2022-06-05 13:04:20.000000 django-app-requires-0.3.3/django_app_requires_first_placeholder/__init__.py
+-rw-r--r--   0 test       (501) staff       (20)       63 2022-06-05 13:03:42.000000 django-app-requires-0.3.3/django_app_requires_first_placeholder/admin.py
+-rw-r--r--   0 test       (501) staff       (20)     2408 2023-09-13 06:50:46.000000 django-app-requires-0.3.3/django_app_requires_first_placeholder/apps.py
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-12 14:14:31.452370 django-app-requires-0.3.3/django_app_requires_first_placeholder/migrations/
+-rw-r--r--   0 test       (501) staff       (20)        0 2022-06-05 13:03:42.000000 django-app-requires-0.3.3/django_app_requires_first_placeholder/migrations/__init__.py
+-rw-r--r--   0 test       (501) staff       (20)       57 2022-06-05 13:03:42.000000 django-app-requires-0.3.3/django_app_requires_first_placeholder/models.py
+-rw-r--r--   0 test       (501) staff       (20)       60 2022-06-05 13:03:42.000000 django-app-requires-0.3.3/django_app_requires_first_placeholder/tests.py
+-rw-r--r--   0 test       (501) staff       (20)       63 2022-06-05 13:03:42.000000 django-app-requires-0.3.3/django_app_requires_first_placeholder/views.py
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-12 14:14:31.453122 django-app-requires-0.3.3/django_app_requires_last_placeholder/
+-rw-r--r--   0 test       (501) staff       (20)      105 2022-06-05 07:49:41.000000 django-app-requires-0.3.3/django_app_requires_last_placeholder/__init__.py
+-rw-r--r--   0 test       (501) staff       (20)       63 2022-06-05 07:46:24.000000 django-app-requires-0.3.3/django_app_requires_last_placeholder/admin.py
+-rw-r--r--   0 test       (501) staff       (20)      799 2023-09-13 06:50:39.000000 django-app-requires-0.3.3/django_app_requires_last_placeholder/apps.py
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-12 14:14:31.453244 django-app-requires-0.3.3/django_app_requires_last_placeholder/migrations/
+-rw-r--r--   0 test       (501) staff       (20)        0 2022-06-05 07:46:24.000000 django-app-requires-0.3.3/django_app_requires_last_placeholder/migrations/__init__.py
+-rw-r--r--   0 test       (501) staff       (20)       57 2022-06-05 07:46:24.000000 django-app-requires-0.3.3/django_app_requires_last_placeholder/models.py
+-rw-r--r--   0 test       (501) staff       (20)       60 2022-06-05 07:46:24.000000 django-app-requires-0.3.3/django_app_requires_last_placeholder/tests.py
+-rw-r--r--   0 test       (501) staff       (20)       63 2022-06-05 07:46:24.000000 django-app-requires-0.3.3/django_app_requires_last_placeholder/views.py
+-rw-r--r--   0 test       (501) staff       (20)       20 2023-09-13 06:50:51.000000 django-app-requires-0.3.3/requirements.txt
+-rw-r--r--   0 test       (501) staff       (20)       38 2024-05-12 14:14:31.453556 django-app-requires-0.3.3/setup.cfg
+-rw-r--r--   0 test       (501) staff       (20)     1615 2024-05-12 14:08:48.000000 django-app-requires-0.3.3/setup.py
```

### Comparing `django-app-requires-0.3.2/LICENSE` & `django-app-requires-0.3.3/LICENSE`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 MIT License
 
-Copyright (c) 2020 zencore.cn
-
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `django-app-requires-0.3.2/PKG-INFO` & `django-app-requires-0.3.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: django-app-requires
-Version: 0.3.2
+Version: 0.3.3
 Summary: A simple tool that allows you to specify app dependencies and middleware dependencies in your application, and also allow you to add default values for your additional configurations, after then load all your application settings into your project's settings.
+Home-page: UNKNOWN
 Author: Jin MinXiang
-Author-email: jinminxiang@zencore.cn
 Maintainer: Jin MinXiang
-Maintainer-email: jinminxiang@zencore.cn
 License: MIT
 Keywords: django utils
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Description-Content-Type: text/markdown
@@ -153,7 +153,13 @@
 
 - Fix app_setting_callbacks duplicate load problem.
 
 ### v0.3.2
 
 - Doc update.
 - Use zenutils.
+
+### v0.3.3
+
+- Doc update.
+
+
```

### Comparing `django-app-requires-0.3.2/README.md` & `django-app-requires-0.3.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -134,7 +134,11 @@
 
 - Fix app_setting_callbacks duplicate load problem.
 
 ### v0.3.2
 
 - Doc update.
 - Use zenutils.
+
+### v0.3.3
+
+- Doc update.
```

### Comparing `django-app-requires-0.3.2/django_app_requires/utils.py` & `django-app-requires-0.3.3/django_app_requires/utils.py`

 * *Files identical despite different names*

### Comparing `django-app-requires-0.3.2/django_app_requires.egg-info/PKG-INFO` & `django-app-requires-0.3.3/django_app_requires.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: django-app-requires
-Version: 0.3.2
+Version: 0.3.3
 Summary: A simple tool that allows you to specify app dependencies and middleware dependencies in your application, and also allow you to add default values for your additional configurations, after then load all your application settings into your project's settings.
+Home-page: UNKNOWN
 Author: Jin MinXiang
-Author-email: jinminxiang@zencore.cn
 Maintainer: Jin MinXiang
-Maintainer-email: jinminxiang@zencore.cn
 License: MIT
 Keywords: django utils
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Description-Content-Type: text/markdown
@@ -153,7 +153,13 @@
 
 - Fix app_setting_callbacks duplicate load problem.
 
 ### v0.3.2
 
 - Doc update.
 - Use zenutils.
+
+### v0.3.3
+
+- Doc update.
+
+
```

### Comparing `django-app-requires-0.3.2/django_app_requires.egg-info/SOURCES.txt` & `django-app-requires-0.3.3/django_app_requires.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-app-requires-0.3.2/django_app_requires_first_placeholder/apps.py` & `django-app-requires-0.3.3/django_app_requires_first_placeholder/apps.py`

 * *Files identical despite different names*

### Comparing `django-app-requires-0.3.2/django_app_requires_last_placeholder/apps.py` & `django-app-requires-0.3.3/django_app_requires_last_placeholder/apps.py`

 * *Files identical despite different names*

### Comparing `django-app-requires-0.3.2/setup.py` & `django-app-requires-0.3.3/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,22 +11,20 @@
 
 with open(os.path.join(here, "requirements.txt"), "r", encoding="utf-8") as fobj:
     requires = [x.strip() for x in fobj.readlines() if x.strip()]
 
 
 setup(
     name="django-app-requires",
-    version="0.3.2",
+    version="0.3.3",
     description="A simple tool that allows you to specify app dependencies and middleware dependencies in your application, and also allow you to add default values for your additional configurations, after then load all your application settings into your project's settings.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Jin MinXiang",
-    author_email="jinminxiang@zencore.cn",
     maintainer="Jin MinXiang",
-    maintainer_email="jinminxiang@zencore.cn",
     license="MIT",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
```

