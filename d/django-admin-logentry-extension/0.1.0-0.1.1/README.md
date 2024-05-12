# Comparing `tmp/django-admin-logentry-extension-0.1.0.tar.gz` & `tmp/django-admin-logentry-extension-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-admin-logentry-extension-0.1.0.tar", last modified: Sun May 12 08:47:46 2024, max compression
+gzip compressed data, was "django-admin-logentry-extension-0.1.1.tar", last modified: Sun May 12 13:49:04 2024, max compression
```

## Comparing `django-admin-logentry-extension-0.1.0.tar` & `django-admin-logentry-extension-0.1.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-12 08:47:46.727182 django-admin-logentry-extension-0.1.0/
--rw-r--r--   0 test       (501) staff       (20)     1036 2024-05-12 08:42:40.000000 django-admin-logentry-extension-0.1.0/LICENSE
--rw-r--r--   0 test       (501) staff       (20)      270 2024-05-12 08:43:36.000000 django-admin-logentry-extension-0.1.0/MANIFEST.in
--rw-r--r--   0 test       (501) staff       (20)     1164 2024-05-12 08:47:46.727008 django-admin-logentry-extension-0.1.0/PKG-INFO
--rw-r--r--   0 test       (501) staff       (20)      428 2024-05-12 08:42:18.000000 django-admin-logentry-extension-0.1.0/README.md
-drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-12 08:47:46.725904 django-admin-logentry-extension-0.1.0/django_admin_logentry_extension/
--rw-r--r--   0 test       (501) staff       (20)       60 2024-05-12 08:21:05.000000 django-admin-logentry-extension-0.1.0/django_admin_logentry_extension/__init__.py
--rw-r--r--   0 test       (501) staff       (20)      900 2024-05-12 08:20:32.000000 django-admin-logentry-extension-0.1.0/django_admin_logentry_extension/admin.py
--rw-r--r--   0 test       (501) staff       (20)      559 2024-05-11 01:58:02.000000 django-admin-logentry-extension-0.1.0/django_admin_logentry_extension/apps.py
-drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-12 08:47:46.726833 django-admin-logentry-extension-0.1.0/django_admin_logentry_extension/migrations/
--rw-r--r--   0 test       (501) staff       (20)        0 2024-05-10 16:04:19.000000 django-admin-logentry-extension-0.1.0/django_admin_logentry_extension/migrations/__init__.py
--rw-r--r--   0 test       (501) staff       (20)      649 2024-05-11 00:57:07.000000 django-admin-logentry-extension-0.1.0/django_admin_logentry_extension/models.py
--rw-r--r--   0 test       (501) staff       (20)     7726 2024-05-11 06:17:02.000000 django-admin-logentry-extension-0.1.0/django_admin_logentry_extension/monkey.py
--rw-r--r--   0 test       (501) staff       (20)       60 2024-05-10 16:04:19.000000 django-admin-logentry-extension-0.1.0/django_admin_logentry_extension/tests.py
--rw-r--r--   0 test       (501) staff       (20)      246 2024-05-11 01:46:21.000000 django-admin-logentry-extension-0.1.0/django_admin_logentry_extension/utils.py
--rw-r--r--   0 test       (501) staff       (20)        0 2024-05-11 01:49:31.000000 django-admin-logentry-extension-0.1.0/django_admin_logentry_extension/views.py
-drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-12 08:47:46.726711 django-admin-logentry-extension-0.1.0/django_admin_logentry_extension.egg-info/
--rw-r--r--   0 test       (501) staff       (20)     1164 2024-05-12 08:47:46.000000 django-admin-logentry-extension-0.1.0/django_admin_logentry_extension.egg-info/PKG-INFO
--rw-r--r--   0 test       (501) staff       (20)      770 2024-05-12 08:47:46.000000 django-admin-logentry-extension-0.1.0/django_admin_logentry_extension.egg-info/SOURCES.txt
--rw-r--r--   0 test       (501) staff       (20)        1 2024-05-12 08:47:46.000000 django-admin-logentry-extension-0.1.0/django_admin_logentry_extension.egg-info/dependency_links.txt
--rw-r--r--   0 test       (501) staff       (20)        1 2024-05-12 08:47:46.000000 django-admin-logentry-extension-0.1.0/django_admin_logentry_extension.egg-info/not-zip-safe
--rw-r--r--   0 test       (501) staff       (20)       41 2024-05-12 08:47:46.000000 django-admin-logentry-extension-0.1.0/django_admin_logentry_extension.egg-info/requires.txt
--rw-r--r--   0 test       (501) staff       (20)       32 2024-05-12 08:47:46.000000 django-admin-logentry-extension-0.1.0/django_admin_logentry_extension.egg-info/top_level.txt
--rw-r--r--   0 test       (501) staff       (20)       41 2024-05-12 08:44:19.000000 django-admin-logentry-extension-0.1.0/requirements.txt
--rw-r--r--   0 test       (501) staff       (20)       38 2024-05-12 08:47:46.727246 django-admin-logentry-extension-0.1.0/setup.cfg
--rw-r--r--   0 test       (501) staff       (20)     1545 2024-05-12 08:43:04.000000 django-admin-logentry-extension-0.1.0/setup.py
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-12 13:49:04.287461 django-admin-logentry-extension-0.1.1/
+-rw-r--r--   0 test       (501) staff       (20)     1036 2024-05-12 08:42:40.000000 django-admin-logentry-extension-0.1.1/LICENSE
+-rw-r--r--   0 test       (501) staff       (20)      270 2024-05-12 08:43:36.000000 django-admin-logentry-extension-0.1.1/MANIFEST.in
+-rw-r--r--   0 test       (501) staff       (20)     1228 2024-05-12 13:49:04.287337 django-admin-logentry-extension-0.1.1/PKG-INFO
+-rw-r--r--   0 test       (501) staff       (20)      492 2024-05-12 13:45:38.000000 django-admin-logentry-extension-0.1.1/README.md
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-12 13:49:04.286357 django-admin-logentry-extension-0.1.1/django_admin_logentry_extension/
+-rw-r--r--   0 test       (501) staff       (20)      170 2024-05-12 13:44:49.000000 django-admin-logentry-extension-0.1.1/django_admin_logentry_extension/__init__.py
+-rw-r--r--   0 test       (501) staff       (20)      900 2024-05-12 08:20:32.000000 django-admin-logentry-extension-0.1.1/django_admin_logentry_extension/admin.py
+-rw-r--r--   0 test       (501) staff       (20)      559 2024-05-11 01:58:02.000000 django-admin-logentry-extension-0.1.1/django_admin_logentry_extension/apps.py
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-12 13:49:04.287185 django-admin-logentry-extension-0.1.1/django_admin_logentry_extension/migrations/
+-rw-r--r--   0 test       (501) staff       (20)        0 2024-05-10 16:04:19.000000 django-admin-logentry-extension-0.1.1/django_admin_logentry_extension/migrations/__init__.py
+-rw-r--r--   0 test       (501) staff       (20)      649 2024-05-11 00:57:07.000000 django-admin-logentry-extension-0.1.1/django_admin_logentry_extension/models.py
+-rw-r--r--   0 test       (501) staff       (20)     7726 2024-05-11 06:17:02.000000 django-admin-logentry-extension-0.1.1/django_admin_logentry_extension/monkey.py
+-rw-r--r--   0 test       (501) staff       (20)       60 2024-05-10 16:04:19.000000 django-admin-logentry-extension-0.1.1/django_admin_logentry_extension/tests.py
+-rw-r--r--   0 test       (501) staff       (20)      246 2024-05-11 01:46:21.000000 django-admin-logentry-extension-0.1.1/django_admin_logentry_extension/utils.py
+-rw-r--r--   0 test       (501) staff       (20)        0 2024-05-11 01:49:31.000000 django-admin-logentry-extension-0.1.1/django_admin_logentry_extension/views.py
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-12 13:49:04.287058 django-admin-logentry-extension-0.1.1/django_admin_logentry_extension.egg-info/
+-rw-r--r--   0 test       (501) staff       (20)     1228 2024-05-12 13:49:04.000000 django-admin-logentry-extension-0.1.1/django_admin_logentry_extension.egg-info/PKG-INFO
+-rw-r--r--   0 test       (501) staff       (20)      770 2024-05-12 13:49:04.000000 django-admin-logentry-extension-0.1.1/django_admin_logentry_extension.egg-info/SOURCES.txt
+-rw-r--r--   0 test       (501) staff       (20)        1 2024-05-12 13:49:04.000000 django-admin-logentry-extension-0.1.1/django_admin_logentry_extension.egg-info/dependency_links.txt
+-rw-r--r--   0 test       (501) staff       (20)        1 2024-05-12 13:49:04.000000 django-admin-logentry-extension-0.1.1/django_admin_logentry_extension.egg-info/not-zip-safe
+-rw-r--r--   0 test       (501) staff       (20)       41 2024-05-12 13:49:04.000000 django-admin-logentry-extension-0.1.1/django_admin_logentry_extension.egg-info/requires.txt
+-rw-r--r--   0 test       (501) staff       (20)       32 2024-05-12 13:49:04.000000 django-admin-logentry-extension-0.1.1/django_admin_logentry_extension.egg-info/top_level.txt
+-rw-r--r--   0 test       (501) staff       (20)       41 2024-05-12 08:44:19.000000 django-admin-logentry-extension-0.1.1/requirements.txt
+-rw-r--r--   0 test       (501) staff       (20)       38 2024-05-12 13:49:04.287514 django-admin-logentry-extension-0.1.1/setup.cfg
+-rw-r--r--   0 test       (501) staff       (20)     1545 2024-05-12 13:45:41.000000 django-admin-logentry-extension-0.1.1/setup.py
```

### Comparing `django-admin-logentry-extension-0.1.0/LICENSE` & `django-admin-logentry-extension-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-admin-logentry-extension-0.1.0/PKG-INFO` & `django-admin-logentry-extension-0.1.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-admin-logentry-extension
-Version: 0.1.0
+Version: 0.1.1
 Summary: Django Admin操作日志增强。添加浏览、查看、登录、登出、导入、导出等动作标识。
 Home-page: UNKNOWN
 Author: Li HaoRan
 Maintainer: Li HaoRan
 License: MIT
 Keywords: django admin extentions,django admin global admin
 Platform: UNKNOWN
@@ -31,8 +31,12 @@
 
 ### v0.1.0
 
 - 首次发布。
 - 添加浏览、查看、登录、登出、导入、导出等动作标识。
 - 适配django-import-export，能够记录其导入导出动作。
 
+### v0.1.1
+
+- 添加default_app_config增强应用兼容性。
+
```

### Comparing `django-admin-logentry-extension-0.1.0/django_admin_logentry_extension/admin.py` & `django-admin-logentry-extension-0.1.1/django_admin_logentry_extension/admin.py`

 * *Files identical despite different names*

### Comparing `django-admin-logentry-extension-0.1.0/django_admin_logentry_extension/apps.py` & `django-admin-logentry-extension-0.1.1/django_admin_logentry_extension/apps.py`

 * *Files identical despite different names*

### Comparing `django-admin-logentry-extension-0.1.0/django_admin_logentry_extension/models.py` & `django-admin-logentry-extension-0.1.1/django_admin_logentry_extension/models.py`

 * *Files identical despite different names*

### Comparing `django-admin-logentry-extension-0.1.0/django_admin_logentry_extension/monkey.py` & `django-admin-logentry-extension-0.1.1/django_admin_logentry_extension/monkey.py`

 * *Files identical despite different names*

### Comparing `django-admin-logentry-extension-0.1.0/django_admin_logentry_extension.egg-info/PKG-INFO` & `django-admin-logentry-extension-0.1.1/django_admin_logentry_extension.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-admin-logentry-extension
-Version: 0.1.0
+Version: 0.1.1
 Summary: Django Admin操作日志增强。添加浏览、查看、登录、登出、导入、导出等动作标识。
 Home-page: UNKNOWN
 Author: Li HaoRan
 Maintainer: Li HaoRan
 License: MIT
 Keywords: django admin extentions,django admin global admin
 Platform: UNKNOWN
@@ -31,8 +31,12 @@
 
 ### v0.1.0
 
 - 首次发布。
 - 添加浏览、查看、登录、登出、导入、导出等动作标识。
 - 适配django-import-export，能够记录其导入导出动作。
 
+### v0.1.1
+
+- 添加default_app_config增强应用兼容性。
+
```

### Comparing `django-admin-logentry-extension-0.1.0/django_admin_logentry_extension.egg-info/SOURCES.txt` & `django-admin-logentry-extension-0.1.1/django_admin_logentry_extension.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-admin-logentry-extension-0.1.0/setup.py` & `django-admin-logentry-extension-0.1.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     long_description = fobj.read()
 
 with open(os.path.join(here, "requirements.txt"), "r", encoding="utf-8") as fobj:
     requires = [x.strip() for x in fobj.readlines() if x.strip()]
 
 setup(
     name="django-admin-logentry-extension",
-    version="0.1.0",
+    version="0.1.1",
     description="Django Admin操作日志增强。添加浏览、查看、登录、登出、导入、导出等动作标识。",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Li HaoRan",
     maintainer="Li HaoRan",
     license="MIT",
     classifiers=[
```

