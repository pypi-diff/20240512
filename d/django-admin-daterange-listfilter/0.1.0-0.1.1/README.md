# Comparing `tmp/django-admin-daterange-listfilter-0.1.0.tar.gz` & `tmp/django-admin-daterange-listfilter-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-admin-daterange-listfilter-0.1.0.tar", last modified: Sun May 12 08:14:48 2024, max compression
+gzip compressed data, was "django-admin-daterange-listfilter-0.1.1.tar", last modified: Sun May 12 08:28:44 2024, max compression
```

## Comparing `django-admin-daterange-listfilter-0.1.0.tar` & `django-admin-daterange-listfilter-0.1.1.tar`

### file list

```diff
@@ -1,36 +1,41 @@
-drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-12 08:14:48.731971 django-admin-daterange-listfilter-0.1.0/
--rw-r--r--   0 test       (501) staff       (20)     1036 2024-05-12 08:00:26.000000 django-admin-daterange-listfilter-0.1.0/LICENSE
--rw-r--r--   0 test       (501) staff       (20)      276 2024-05-12 08:08:04.000000 django-admin-daterange-listfilter-0.1.0/MANIFEST.in
--rw-r--r--   0 test       (501) staff       (20)     1465 2024-05-12 08:14:48.731855 django-admin-daterange-listfilter-0.1.0/PKG-INFO
--rw-r--r--   0 test       (501) staff       (20)      797 2024-05-12 08:10:45.000000 django-admin-daterange-listfilter-0.1.0/README.md
-drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-12 08:14:48.730186 django-admin-daterange-listfilter-0.1.0/django_admin_daterange_listfilter/
--rw-r--r--   0 test       (501) staff       (20)      131 2024-05-12 07:19:32.000000 django-admin-daterange-listfilter-0.1.0/django_admin_daterange_listfilter/__init__.py
--rw-r--r--   0 test       (501) staff       (20)       63 2024-05-11 11:41:12.000000 django-admin-daterange-listfilter-0.1.0/django_admin_daterange_listfilter/admin.py
--rw-r--r--   0 test       (501) staff       (20)      195 2024-05-11 11:41:12.000000 django-admin-daterange-listfilter-0.1.0/django_admin_daterange_listfilter/apps.py
--rw-r--r--   0 test       (501) staff       (20)     3161 2024-05-12 07:38:44.000000 django-admin-daterange-listfilter-0.1.0/django_admin_daterange_listfilter/filters.py
-drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-12 08:14:48.731161 django-admin-daterange-listfilter-0.1.0/django_admin_daterange_listfilter/migrations/
--rw-r--r--   0 test       (501) staff       (20)        0 2024-05-11 11:41:12.000000 django-admin-daterange-listfilter-0.1.0/django_admin_daterange_listfilter/migrations/__init__.py
--rw-r--r--   0 test       (501) staff       (20)       57 2024-05-11 11:41:12.000000 django-admin-daterange-listfilter-0.1.0/django_admin_daterange_listfilter/models.py
-drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-12 08:14:48.728234 django-admin-daterange-listfilter-0.1.0/django_admin_daterange_listfilter/static/
-drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-12 08:14:48.728353 django-admin-daterange-listfilter-0.1.0/django_admin_daterange_listfilter/static/django_admin_daterange_listfilter/
-drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-12 08:14:48.731261 django-admin-daterange-listfilter-0.1.0/django_admin_daterange_listfilter/static/django_admin_daterange_listfilter/css/
--rw-r--r--   0 test       (501) staff       (20)      555 2024-05-11 11:44:57.000000 django-admin-daterange-listfilter-0.1.0/django_admin_daterange_listfilter/static/django_admin_daterange_listfilter/css/DateRangeFilter.css
-drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-12 08:14:48.731519 django-admin-daterange-listfilter-0.1.0/django_admin_daterange_listfilter/static/django_admin_daterange_listfilter/js/
--rw-r--r--   0 test       (501) staff       (20)     1474 2024-05-11 11:45:18.000000 django-admin-daterange-listfilter-0.1.0/django_admin_daterange_listfilter/static/django_admin_daterange_listfilter/js/DateRangeFilter.js
--rw-r--r--   0 test       (501) staff       (20)     1404 2024-05-11 11:45:55.000000 django-admin-daterange-listfilter-0.1.0/django_admin_daterange_listfilter/static/django_admin_daterange_listfilter/js/parseParam.js
-drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-12 08:14:48.728475 django-admin-daterange-listfilter-0.1.0/django_admin_daterange_listfilter/templates/
-drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-12 08:14:48.728525 django-admin-daterange-listfilter-0.1.0/django_admin_daterange_listfilter/templates/django_admin_daterange_listfilter/
-drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-12 08:14:48.731671 django-admin-daterange-listfilter-0.1.0/django_admin_daterange_listfilter/templates/django_admin_daterange_listfilter/filters/
--rw-r--r--   0 test       (501) staff       (20)     1036 2024-05-11 11:43:31.000000 django-admin-daterange-listfilter-0.1.0/django_admin_daterange_listfilter/templates/django_admin_daterange_listfilter/filters/DateRangeFilter.html
--rw-r--r--   0 test       (501) staff       (20)       60 2024-05-11 11:41:12.000000 django-admin-daterange-listfilter-0.1.0/django_admin_daterange_listfilter/tests.py
--rw-r--r--   0 test       (501) staff       (20)       63 2024-05-11 11:41:12.000000 django-admin-daterange-listfilter-0.1.0/django_admin_daterange_listfilter/views.py
-drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-12 08:14:48.731029 django-admin-daterange-listfilter-0.1.0/django_admin_daterange_listfilter.egg-info/
--rw-r--r--   0 test       (501) staff       (20)     1465 2024-05-12 08:14:48.000000 django-admin-daterange-listfilter-0.1.0/django_admin_daterange_listfilter.egg-info/PKG-INFO
--rw-r--r--   0 test       (501) staff       (20)     1153 2024-05-12 08:14:48.000000 django-admin-daterange-listfilter-0.1.0/django_admin_daterange_listfilter.egg-info/SOURCES.txt
--rw-r--r--   0 test       (501) staff       (20)        1 2024-05-12 08:14:48.000000 django-admin-daterange-listfilter-0.1.0/django_admin_daterange_listfilter.egg-info/dependency_links.txt
--rw-r--r--   0 test       (501) staff       (20)        1 2024-05-12 08:14:48.000000 django-admin-daterange-listfilter-0.1.0/django_admin_daterange_listfilter.egg-info/not-zip-safe
--rw-r--r--   0 test       (501) staff       (20)       98 2024-05-12 08:14:48.000000 django-admin-daterange-listfilter-0.1.0/django_admin_daterange_listfilter.egg-info/requires.txt
--rw-r--r--   0 test       (501) staff       (20)       34 2024-05-12 08:14:48.000000 django-admin-daterange-listfilter-0.1.0/django_admin_daterange_listfilter.egg-info/top_level.txt
--rw-r--r--   0 test       (501) staff       (20)       98 2024-05-12 08:07:27.000000 django-admin-daterange-listfilter-0.1.0/requirements.txt
--rw-r--r--   0 test       (501) staff       (20)       38 2024-05-12 08:14:48.732017 django-admin-daterange-listfilter-0.1.0/setup.cfg
--rw-r--r--   0 test       (501) staff       (20)     1483 2024-05-12 08:05:54.000000 django-admin-daterange-listfilter-0.1.0/setup.py
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-12 08:28:44.589361 django-admin-daterange-listfilter-0.1.1/
+-rw-r--r--   0 test       (501) staff       (20)     1036 2024-05-12 08:00:26.000000 django-admin-daterange-listfilter-0.1.1/LICENSE
+-rw-r--r--   0 test       (501) staff       (20)      276 2024-05-12 08:08:04.000000 django-admin-daterange-listfilter-0.1.1/MANIFEST.in
+-rw-r--r--   0 test       (501) staff       (20)     1506 2024-05-12 08:28:44.589215 django-admin-daterange-listfilter-0.1.1/PKG-INFO
+-rw-r--r--   0 test       (501) staff       (20)      838 2024-05-12 08:27:45.000000 django-admin-daterange-listfilter-0.1.1/README.md
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-12 08:28:44.586366 django-admin-daterange-listfilter-0.1.1/django_admin_daterange_listfilter/
+-rw-r--r--   0 test       (501) staff       (20)      131 2024-05-12 07:19:32.000000 django-admin-daterange-listfilter-0.1.1/django_admin_daterange_listfilter/__init__.py
+-rw-r--r--   0 test       (501) staff       (20)       63 2024-05-11 11:41:12.000000 django-admin-daterange-listfilter-0.1.1/django_admin_daterange_listfilter/admin.py
+-rw-r--r--   0 test       (501) staff       (20)      195 2024-05-11 11:41:12.000000 django-admin-daterange-listfilter-0.1.1/django_admin_daterange_listfilter/apps.py
+-rw-r--r--   0 test       (501) staff       (20)     3161 2024-05-12 07:38:44.000000 django-admin-daterange-listfilter-0.1.1/django_admin_daterange_listfilter/filters.py
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-12 08:28:44.583630 django-admin-daterange-listfilter-0.1.1/django_admin_daterange_listfilter/locale/
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-12 08:28:44.583678 django-admin-daterange-listfilter-0.1.1/django_admin_daterange_listfilter/locale/zh_Hans/
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-12 08:28:44.587878 django-admin-daterange-listfilter-0.1.1/django_admin_daterange_listfilter/locale/zh_Hans/LC_MESSAGES/
+-rw-r--r--   0 test       (501) staff       (20)      478 2024-05-12 08:27:14.000000 django-admin-daterange-listfilter-0.1.1/django_admin_daterange_listfilter/locale/zh_Hans/LC_MESSAGES/django.mo
+-rw-r--r--   0 test       (501) staff       (20)     1080 2024-05-12 08:27:04.000000 django-admin-daterange-listfilter-0.1.1/django_admin_daterange_listfilter/locale/zh_Hans/LC_MESSAGES/django.po
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-12 08:28:44.588094 django-admin-daterange-listfilter-0.1.1/django_admin_daterange_listfilter/migrations/
+-rw-r--r--   0 test       (501) staff       (20)        0 2024-05-11 11:41:12.000000 django-admin-daterange-listfilter-0.1.1/django_admin_daterange_listfilter/migrations/__init__.py
+-rw-r--r--   0 test       (501) staff       (20)       57 2024-05-11 11:41:12.000000 django-admin-daterange-listfilter-0.1.1/django_admin_daterange_listfilter/models.py
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-12 08:28:44.583862 django-admin-daterange-listfilter-0.1.1/django_admin_daterange_listfilter/static/
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-12 08:28:44.583977 django-admin-daterange-listfilter-0.1.1/django_admin_daterange_listfilter/static/django_admin_daterange_listfilter/
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-12 08:28:44.588194 django-admin-daterange-listfilter-0.1.1/django_admin_daterange_listfilter/static/django_admin_daterange_listfilter/css/
+-rw-r--r--   0 test       (501) staff       (20)      555 2024-05-11 11:44:57.000000 django-admin-daterange-listfilter-0.1.1/django_admin_daterange_listfilter/static/django_admin_daterange_listfilter/css/DateRangeFilter.css
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-12 08:28:44.588700 django-admin-daterange-listfilter-0.1.1/django_admin_daterange_listfilter/static/django_admin_daterange_listfilter/js/
+-rw-r--r--   0 test       (501) staff       (20)     1474 2024-05-11 11:45:18.000000 django-admin-daterange-listfilter-0.1.1/django_admin_daterange_listfilter/static/django_admin_daterange_listfilter/js/DateRangeFilter.js
+-rw-r--r--   0 test       (501) staff       (20)     1404 2024-05-11 11:45:55.000000 django-admin-daterange-listfilter-0.1.1/django_admin_daterange_listfilter/static/django_admin_daterange_listfilter/js/parseParam.js
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-12 08:28:44.584095 django-admin-daterange-listfilter-0.1.1/django_admin_daterange_listfilter/templates/
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-12 08:28:44.584144 django-admin-daterange-listfilter-0.1.1/django_admin_daterange_listfilter/templates/django_admin_daterange_listfilter/
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-12 08:28:44.588921 django-admin-daterange-listfilter-0.1.1/django_admin_daterange_listfilter/templates/django_admin_daterange_listfilter/filters/
+-rw-r--r--   0 test       (501) staff       (20)     1036 2024-05-11 11:43:31.000000 django-admin-daterange-listfilter-0.1.1/django_admin_daterange_listfilter/templates/django_admin_daterange_listfilter/filters/DateRangeFilter.html
+-rw-r--r--   0 test       (501) staff       (20)       60 2024-05-11 11:41:12.000000 django-admin-daterange-listfilter-0.1.1/django_admin_daterange_listfilter/tests.py
+-rw-r--r--   0 test       (501) staff       (20)       63 2024-05-11 11:41:12.000000 django-admin-daterange-listfilter-0.1.1/django_admin_daterange_listfilter/views.py
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-12 08:28:44.587530 django-admin-daterange-listfilter-0.1.1/django_admin_daterange_listfilter.egg-info/
+-rw-r--r--   0 test       (501) staff       (20)     1506 2024-05-12 08:28:44.000000 django-admin-daterange-listfilter-0.1.1/django_admin_daterange_listfilter.egg-info/PKG-INFO
+-rw-r--r--   0 test       (501) staff       (20)     1295 2024-05-12 08:28:44.000000 django-admin-daterange-listfilter-0.1.1/django_admin_daterange_listfilter.egg-info/SOURCES.txt
+-rw-r--r--   0 test       (501) staff       (20)        1 2024-05-12 08:28:44.000000 django-admin-daterange-listfilter-0.1.1/django_admin_daterange_listfilter.egg-info/dependency_links.txt
+-rw-r--r--   0 test       (501) staff       (20)        1 2024-05-12 08:28:44.000000 django-admin-daterange-listfilter-0.1.1/django_admin_daterange_listfilter.egg-info/not-zip-safe
+-rw-r--r--   0 test       (501) staff       (20)       98 2024-05-12 08:28:44.000000 django-admin-daterange-listfilter-0.1.1/django_admin_daterange_listfilter.egg-info/requires.txt
+-rw-r--r--   0 test       (501) staff       (20)       34 2024-05-12 08:28:44.000000 django-admin-daterange-listfilter-0.1.1/django_admin_daterange_listfilter.egg-info/top_level.txt
+-rw-r--r--   0 test       (501) staff       (20)       98 2024-05-12 08:07:27.000000 django-admin-daterange-listfilter-0.1.1/requirements.txt
+-rw-r--r--   0 test       (501) staff       (20)       38 2024-05-12 08:28:44.589412 django-admin-daterange-listfilter-0.1.1/setup.cfg
+-rw-r--r--   0 test       (501) staff       (20)     1483 2024-05-12 08:27:48.000000 django-admin-daterange-listfilter-0.1.1/setup.py
```

### Comparing `django-admin-daterange-listfilter-0.1.0/LICENSE` & `django-admin-daterange-listfilter-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-admin-daterange-listfilter-0.1.0/PKG-INFO` & `django-admin-daterange-listfilter-0.1.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-admin-daterange-listfilter
-Version: 0.1.0
+Version: 0.1.1
 Summary: 通过日历自由选择时间范围。
 Home-page: UNKNOWN
 Author: Zhan YuCong
 Maintainer: Zhan YuCong
 License: MIT
 Keywords: django admin extentions,daterange listfilter
 Platform: UNKNOWN
@@ -61,8 +61,12 @@
 
 ## 版本记录
 
 ### v0.1.0
 
 - 版本首发。
 
+### v0.1.1
+
+- 添加中文i18n翻译。
+
```

### Comparing `django-admin-daterange-listfilter-0.1.0/README.md` & `django-admin-daterange-listfilter-0.1.1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -41,7 +41,11 @@
 ```
 
 ## 版本记录
 
 ### v0.1.0
 
 - 版本首发。
+
+### v0.1.1
+
+- 添加中文i18n翻译。
```

### Comparing `django-admin-daterange-listfilter-0.1.0/django_admin_daterange_listfilter/filters.py` & `django-admin-daterange-listfilter-0.1.1/django_admin_daterange_listfilter/filters.py`

 * *Files identical despite different names*

### Comparing `django-admin-daterange-listfilter-0.1.0/django_admin_daterange_listfilter/static/django_admin_daterange_listfilter/css/DateRangeFilter.css` & `django-admin-daterange-listfilter-0.1.1/django_admin_daterange_listfilter/static/django_admin_daterange_listfilter/css/DateRangeFilter.css`

 * *Files identical despite different names*

### Comparing `django-admin-daterange-listfilter-0.1.0/django_admin_daterange_listfilter/static/django_admin_daterange_listfilter/js/DateRangeFilter.js` & `django-admin-daterange-listfilter-0.1.1/django_admin_daterange_listfilter/static/django_admin_daterange_listfilter/js/DateRangeFilter.js`

 * *Files identical despite different names*

### Comparing `django-admin-daterange-listfilter-0.1.0/django_admin_daterange_listfilter/static/django_admin_daterange_listfilter/js/parseParam.js` & `django-admin-daterange-listfilter-0.1.1/django_admin_daterange_listfilter/static/django_admin_daterange_listfilter/js/parseParam.js`

 * *Files identical despite different names*

### Comparing `django-admin-daterange-listfilter-0.1.0/django_admin_daterange_listfilter/templates/django_admin_daterange_listfilter/filters/DateRangeFilter.html` & `django-admin-daterange-listfilter-0.1.1/django_admin_daterange_listfilter/templates/django_admin_daterange_listfilter/filters/DateRangeFilter.html`

 * *Files identical despite different names*

### Comparing `django-admin-daterange-listfilter-0.1.0/django_admin_daterange_listfilter.egg-info/PKG-INFO` & `django-admin-daterange-listfilter-0.1.1/django_admin_daterange_listfilter.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-admin-daterange-listfilter
-Version: 0.1.0
+Version: 0.1.1
 Summary: 通过日历自由选择时间范围。
 Home-page: UNKNOWN
 Author: Zhan YuCong
 Maintainer: Zhan YuCong
 License: MIT
 Keywords: django admin extentions,daterange listfilter
 Platform: UNKNOWN
@@ -61,8 +61,12 @@
 
 ## 版本记录
 
 ### v0.1.0
 
 - 版本首发。
 
+### v0.1.1
+
+- 添加中文i18n翻译。
+
```

### Comparing `django-admin-daterange-listfilter-0.1.0/django_admin_daterange_listfilter.egg-info/SOURCES.txt` & `django-admin-daterange-listfilter-0.1.1/django_admin_daterange_listfilter.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -12,12 +12,14 @@
 django_admin_daterange_listfilter/views.py
 django_admin_daterange_listfilter.egg-info/PKG-INFO
 django_admin_daterange_listfilter.egg-info/SOURCES.txt
 django_admin_daterange_listfilter.egg-info/dependency_links.txt
 django_admin_daterange_listfilter.egg-info/not-zip-safe
 django_admin_daterange_listfilter.egg-info/requires.txt
 django_admin_daterange_listfilter.egg-info/top_level.txt
+django_admin_daterange_listfilter/locale/zh_Hans/LC_MESSAGES/django.mo
+django_admin_daterange_listfilter/locale/zh_Hans/LC_MESSAGES/django.po
 django_admin_daterange_listfilter/migrations/__init__.py
 django_admin_daterange_listfilter/static/django_admin_daterange_listfilter/css/DateRangeFilter.css
 django_admin_daterange_listfilter/static/django_admin_daterange_listfilter/js/DateRangeFilter.js
 django_admin_daterange_listfilter/static/django_admin_daterange_listfilter/js/parseParam.js
 django_admin_daterange_listfilter/templates/django_admin_daterange_listfilter/filters/DateRangeFilter.html
```

### Comparing `django-admin-daterange-listfilter-0.1.0/setup.py` & `django-admin-daterange-listfilter-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     long_description = fobj.read()
 
 with open(os.path.join(here, "requirements.txt"), "r", encoding="utf-8") as fobj:
     requires = [x.strip() for x in fobj.readlines() if x.strip()]
 
 setup(
     name="django-admin-daterange-listfilter",
-    version="0.1.0",
+    version="0.1.1",
     description="通过日历自由选择时间范围。",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Zhan YuCong",
     maintainer="Zhan YuCong",
     license="MIT",
     classifiers=[
```

