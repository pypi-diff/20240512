# Comparing `tmp/django-admin-logentry-extension-0.1.1.tar.gz` & `tmp/django-admin-logentry-extension-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-admin-logentry-extension-0.1.1.tar", last modified: Sun May 12 13:49:04 2024, max compression
+gzip compressed data, was "django-admin-logentry-extension-0.1.2.tar", last modified: Sun May 12 14:16:42 2024, max compression
```

## Comparing `django-admin-logentry-extension-0.1.1.tar` & `django-admin-logentry-extension-0.1.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-12 13:49:04.287461 django-admin-logentry-extension-0.1.1/
--rw-r--r--   0 test       (501) staff       (20)     1036 2024-05-12 08:42:40.000000 django-admin-logentry-extension-0.1.1/LICENSE
--rw-r--r--   0 test       (501) staff       (20)      270 2024-05-12 08:43:36.000000 django-admin-logentry-extension-0.1.1/MANIFEST.in
--rw-r--r--   0 test       (501) staff       (20)     1228 2024-05-12 13:49:04.287337 django-admin-logentry-extension-0.1.1/PKG-INFO
--rw-r--r--   0 test       (501) staff       (20)      492 2024-05-12 13:45:38.000000 django-admin-logentry-extension-0.1.1/README.md
-drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-12 13:49:04.286357 django-admin-logentry-extension-0.1.1/django_admin_logentry_extension/
--rw-r--r--   0 test       (501) staff       (20)      170 2024-05-12 13:44:49.000000 django-admin-logentry-extension-0.1.1/django_admin_logentry_extension/__init__.py
--rw-r--r--   0 test       (501) staff       (20)      900 2024-05-12 08:20:32.000000 django-admin-logentry-extension-0.1.1/django_admin_logentry_extension/admin.py
--rw-r--r--   0 test       (501) staff       (20)      559 2024-05-11 01:58:02.000000 django-admin-logentry-extension-0.1.1/django_admin_logentry_extension/apps.py
-drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-12 13:49:04.287185 django-admin-logentry-extension-0.1.1/django_admin_logentry_extension/migrations/
--rw-r--r--   0 test       (501) staff       (20)        0 2024-05-10 16:04:19.000000 django-admin-logentry-extension-0.1.1/django_admin_logentry_extension/migrations/__init__.py
--rw-r--r--   0 test       (501) staff       (20)      649 2024-05-11 00:57:07.000000 django-admin-logentry-extension-0.1.1/django_admin_logentry_extension/models.py
--rw-r--r--   0 test       (501) staff       (20)     7726 2024-05-11 06:17:02.000000 django-admin-logentry-extension-0.1.1/django_admin_logentry_extension/monkey.py
--rw-r--r--   0 test       (501) staff       (20)       60 2024-05-10 16:04:19.000000 django-admin-logentry-extension-0.1.1/django_admin_logentry_extension/tests.py
--rw-r--r--   0 test       (501) staff       (20)      246 2024-05-11 01:46:21.000000 django-admin-logentry-extension-0.1.1/django_admin_logentry_extension/utils.py
--rw-r--r--   0 test       (501) staff       (20)        0 2024-05-11 01:49:31.000000 django-admin-logentry-extension-0.1.1/django_admin_logentry_extension/views.py
-drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-12 13:49:04.287058 django-admin-logentry-extension-0.1.1/django_admin_logentry_extension.egg-info/
--rw-r--r--   0 test       (501) staff       (20)     1228 2024-05-12 13:49:04.000000 django-admin-logentry-extension-0.1.1/django_admin_logentry_extension.egg-info/PKG-INFO
--rw-r--r--   0 test       (501) staff       (20)      770 2024-05-12 13:49:04.000000 django-admin-logentry-extension-0.1.1/django_admin_logentry_extension.egg-info/SOURCES.txt
--rw-r--r--   0 test       (501) staff       (20)        1 2024-05-12 13:49:04.000000 django-admin-logentry-extension-0.1.1/django_admin_logentry_extension.egg-info/dependency_links.txt
--rw-r--r--   0 test       (501) staff       (20)        1 2024-05-12 13:49:04.000000 django-admin-logentry-extension-0.1.1/django_admin_logentry_extension.egg-info/not-zip-safe
--rw-r--r--   0 test       (501) staff       (20)       41 2024-05-12 13:49:04.000000 django-admin-logentry-extension-0.1.1/django_admin_logentry_extension.egg-info/requires.txt
--rw-r--r--   0 test       (501) staff       (20)       32 2024-05-12 13:49:04.000000 django-admin-logentry-extension-0.1.1/django_admin_logentry_extension.egg-info/top_level.txt
--rw-r--r--   0 test       (501) staff       (20)       41 2024-05-12 08:44:19.000000 django-admin-logentry-extension-0.1.1/requirements.txt
--rw-r--r--   0 test       (501) staff       (20)       38 2024-05-12 13:49:04.287514 django-admin-logentry-extension-0.1.1/setup.cfg
--rw-r--r--   0 test       (501) staff       (20)     1545 2024-05-12 13:45:41.000000 django-admin-logentry-extension-0.1.1/setup.py
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-12 14:16:42.441949 django-admin-logentry-extension-0.1.2/
+-rw-r--r--   0 test       (501) staff       (20)     1036 2024-05-12 08:42:40.000000 django-admin-logentry-extension-0.1.2/LICENSE
+-rw-r--r--   0 test       (501) staff       (20)      270 2024-05-12 08:43:36.000000 django-admin-logentry-extension-0.1.2/MANIFEST.in
+-rw-r--r--   0 test       (501) staff       (20)     1228 2024-05-12 14:16:42.441796 django-admin-logentry-extension-0.1.2/PKG-INFO
+-rw-r--r--   0 test       (501) staff       (20)      492 2024-05-12 14:16:36.000000 django-admin-logentry-extension-0.1.2/README.md
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-12 14:16:42.440531 django-admin-logentry-extension-0.1.2/django_admin_logentry_extension/
+-rw-r--r--   0 test       (501) staff       (20)      163 2024-05-12 14:16:21.000000 django-admin-logentry-extension-0.1.2/django_admin_logentry_extension/__init__.py
+-rw-r--r--   0 test       (501) staff       (20)      900 2024-05-12 08:20:32.000000 django-admin-logentry-extension-0.1.2/django_admin_logentry_extension/admin.py
+-rw-r--r--   0 test       (501) staff       (20)      559 2024-05-11 01:58:02.000000 django-admin-logentry-extension-0.1.2/django_admin_logentry_extension/apps.py
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-12 14:16:42.441606 django-admin-logentry-extension-0.1.2/django_admin_logentry_extension/migrations/
+-rw-r--r--   0 test       (501) staff       (20)        0 2024-05-10 16:04:19.000000 django-admin-logentry-extension-0.1.2/django_admin_logentry_extension/migrations/__init__.py
+-rw-r--r--   0 test       (501) staff       (20)      649 2024-05-11 00:57:07.000000 django-admin-logentry-extension-0.1.2/django_admin_logentry_extension/models.py
+-rw-r--r--   0 test       (501) staff       (20)     7726 2024-05-12 14:00:51.000000 django-admin-logentry-extension-0.1.2/django_admin_logentry_extension/monkey.py
+-rw-r--r--   0 test       (501) staff       (20)       60 2024-05-10 16:04:19.000000 django-admin-logentry-extension-0.1.2/django_admin_logentry_extension/tests.py
+-rw-r--r--   0 test       (501) staff       (20)      246 2024-05-11 01:46:21.000000 django-admin-logentry-extension-0.1.2/django_admin_logentry_extension/utils.py
+-rw-r--r--   0 test       (501) staff       (20)        0 2024-05-11 01:49:31.000000 django-admin-logentry-extension-0.1.2/django_admin_logentry_extension/views.py
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-12 14:16:42.441311 django-admin-logentry-extension-0.1.2/django_admin_logentry_extension.egg-info/
+-rw-r--r--   0 test       (501) staff       (20)     1228 2024-05-12 14:16:42.000000 django-admin-logentry-extension-0.1.2/django_admin_logentry_extension.egg-info/PKG-INFO
+-rw-r--r--   0 test       (501) staff       (20)      770 2024-05-12 14:16:42.000000 django-admin-logentry-extension-0.1.2/django_admin_logentry_extension.egg-info/SOURCES.txt
+-rw-r--r--   0 test       (501) staff       (20)        1 2024-05-12 14:16:42.000000 django-admin-logentry-extension-0.1.2/django_admin_logentry_extension.egg-info/dependency_links.txt
+-rw-r--r--   0 test       (501) staff       (20)        1 2024-05-12 14:16:42.000000 django-admin-logentry-extension-0.1.2/django_admin_logentry_extension.egg-info/not-zip-safe
+-rw-r--r--   0 test       (501) staff       (20)       41 2024-05-12 14:16:42.000000 django-admin-logentry-extension-0.1.2/django_admin_logentry_extension.egg-info/requires.txt
+-rw-r--r--   0 test       (501) staff       (20)       32 2024-05-12 14:16:42.000000 django-admin-logentry-extension-0.1.2/django_admin_logentry_extension.egg-info/top_level.txt
+-rw-r--r--   0 test       (501) staff       (20)       41 2024-05-12 08:44:19.000000 django-admin-logentry-extension-0.1.2/requirements.txt
+-rw-r--r--   0 test       (501) staff       (20)       38 2024-05-12 14:16:42.442005 django-admin-logentry-extension-0.1.2/setup.cfg
+-rw-r--r--   0 test       (501) staff       (20)     1545 2024-05-12 14:16:40.000000 django-admin-logentry-extension-0.1.2/setup.py
```

### Comparing `django-admin-logentry-extension-0.1.1/LICENSE` & `django-admin-logentry-extension-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django-admin-logentry-extension-0.1.1/PKG-INFO` & `django-admin-logentry-extension-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-admin-logentry-extension
-Version: 0.1.1
+Version: 0.1.2
 Summary: Django Admin操作日志增强。添加浏览、查看、登录、登出、导入、导出等动作标识。
 Home-page: UNKNOWN
 Author: Li HaoRan
 Maintainer: Li HaoRan
 License: MIT
 Keywords: django admin extentions,django admin global admin
 Platform: UNKNOWN
@@ -31,12 +31,12 @@
 
 ### v0.1.0
 
 - 首次发布。
 - 添加浏览、查看、登录、登出、导入、导出等动作标识。
 - 适配django-import-export，能够记录其导入导出动作。
 
-### v0.1.1
+### v0.1.2
 
 - 添加default_app_config增强应用兼容性。
```

### Comparing `django-admin-logentry-extension-0.1.1/django_admin_logentry_extension/admin.py` & `django-admin-logentry-extension-0.1.2/django_admin_logentry_extension/admin.py`

 * *Files identical despite different names*

### Comparing `django-admin-logentry-extension-0.1.1/django_admin_logentry_extension/apps.py` & `django-admin-logentry-extension-0.1.2/django_admin_logentry_extension/apps.py`

 * *Files identical despite different names*

### Comparing `django-admin-logentry-extension-0.1.1/django_admin_logentry_extension/models.py` & `django-admin-logentry-extension-0.1.2/django_admin_logentry_extension/models.py`

 * *Files identical despite different names*

### Comparing `django-admin-logentry-extension-0.1.1/django_admin_logentry_extension/monkey.py` & `django-admin-logentry-extension-0.1.2/django_admin_logentry_extension/monkey.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import json
 import logging
+from django.contrib.contenttypes.models import ContentType
+from django.contrib.admin import ModelAdmin
 from django.contrib.admin.models import LogEntry
 from django.contrib.admin.utils import unquote
 from django.contrib.admin.options import csrf_protect_m
 from django.contrib.admin.options import get_content_type_for_model
-from django.contrib.admin import ModelAdmin
-from django.contrib.contenttypes.models import ContentType
-from django.contrib.auth import sensitive_variables
 from django.contrib import auth
+from django.contrib.auth import sensitive_variables
 from django.contrib.auth import get_user_model
 
 from .models import ACTION_FLAG_EXT_CHOICES
 from .models import BROWSING
 from .models import READING
 from .models import LOGIN
 from .models import LOGOUT
```

### Comparing `django-admin-logentry-extension-0.1.1/django_admin_logentry_extension.egg-info/PKG-INFO` & `django-admin-logentry-extension-0.1.2/django_admin_logentry_extension.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-admin-logentry-extension
-Version: 0.1.1
+Version: 0.1.2
 Summary: Django Admin操作日志增强。添加浏览、查看、登录、登出、导入、导出等动作标识。
 Home-page: UNKNOWN
 Author: Li HaoRan
 Maintainer: Li HaoRan
 License: MIT
 Keywords: django admin extentions,django admin global admin
 Platform: UNKNOWN
@@ -31,12 +31,12 @@
 
 ### v0.1.0
 
 - 首次发布。
 - 添加浏览、查看、登录、登出、导入、导出等动作标识。
 - 适配django-import-export，能够记录其导入导出动作。
 
-### v0.1.1
+### v0.1.2
 
 - 添加default_app_config增强应用兼容性。
```

### Comparing `django-admin-logentry-extension-0.1.1/django_admin_logentry_extension.egg-info/SOURCES.txt` & `django-admin-logentry-extension-0.1.2/django_admin_logentry_extension.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-admin-logentry-extension-0.1.1/setup.py` & `django-admin-logentry-extension-0.1.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     long_description = fobj.read()
 
 with open(os.path.join(here, "requirements.txt"), "r", encoding="utf-8") as fobj:
     requires = [x.strip() for x in fobj.readlines() if x.strip()]
 
 setup(
     name="django-admin-logentry-extension",
-    version="0.1.1",
+    version="0.1.2",
     description="Django Admin操作日志增强。添加浏览、查看、登录、登出、导入、导出等动作标识。",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Li HaoRan",
     maintainer="Li HaoRan",
     license="MIT",
     classifiers=[
```

