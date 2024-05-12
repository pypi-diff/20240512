# Comparing `tmp/django-admin-daterange-listfilter-0.1.2.tar.gz` & `tmp/django-admin-daterange-listfilter-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-admin-daterange-listfilter-0.1.2.tar", last modified: Sun May 12 08:34:15 2024, max compression
+gzip compressed data, was "django-admin-daterange-listfilter-0.1.3.tar", last modified: Sun May 12 08:36:22 2024, max compression
```

## Comparing `django-admin-daterange-listfilter-0.1.2.tar` & `django-admin-daterange-listfilter-0.1.3.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-12 08:34:15.278518 django-admin-daterange-listfilter-0.1.2/
--rw-r--r--   0 test       (501) staff       (20)     1036 2024-05-12 08:00:26.000000 django-admin-daterange-listfilter-0.1.2/LICENSE
--rw-r--r--   0 test       (501) staff       (20)      276 2024-05-12 08:08:04.000000 django-admin-daterange-listfilter-0.1.2/MANIFEST.in
--rw-r--r--   0 test       (501) staff       (20)     1506 2024-05-12 08:34:15.278396 django-admin-daterange-listfilter-0.1.2/PKG-INFO
--rw-r--r--   0 test       (501) staff       (20)      838 2024-05-12 08:33:19.000000 django-admin-daterange-listfilter-0.1.2/README.md
-drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-12 08:34:15.275473 django-admin-daterange-listfilter-0.1.2/django_admin_daterange_listfilter/
--rw-r--r--   0 test       (501) staff       (20)      131 2024-05-12 07:19:32.000000 django-admin-daterange-listfilter-0.1.2/django_admin_daterange_listfilter/__init__.py
--rw-r--r--   0 test       (501) staff       (20)       63 2024-05-11 11:41:12.000000 django-admin-daterange-listfilter-0.1.2/django_admin_daterange_listfilter/admin.py
--rw-r--r--   0 test       (501) staff       (20)      195 2024-05-11 11:41:12.000000 django-admin-daterange-listfilter-0.1.2/django_admin_daterange_listfilter/apps.py
--rw-r--r--   0 test       (501) staff       (20)     3161 2024-05-12 07:38:44.000000 django-admin-daterange-listfilter-0.1.2/django_admin_daterange_listfilter/filters.py
-drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-12 08:34:15.272640 django-admin-daterange-listfilter-0.1.2/django_admin_daterange_listfilter/locale/
-drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-12 08:34:15.272691 django-admin-daterange-listfilter-0.1.2/django_admin_daterange_listfilter/locale/zh_Hans/
-drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-12 08:34:15.277129 django-admin-daterange-listfilter-0.1.2/django_admin_daterange_listfilter/locale/zh_Hans/LC_MESSAGES/
--rw-r--r--   0 test       (501) staff       (20)      478 2024-05-12 08:27:14.000000 django-admin-daterange-listfilter-0.1.2/django_admin_daterange_listfilter/locale/zh_Hans/LC_MESSAGES/django.mo
--rw-r--r--   0 test       (501) staff       (20)     1092 2024-05-12 08:31:25.000000 django-admin-daterange-listfilter-0.1.2/django_admin_daterange_listfilter/locale/zh_Hans/LC_MESSAGES/django.po
-drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-12 08:34:15.277336 django-admin-daterange-listfilter-0.1.2/django_admin_daterange_listfilter/migrations/
--rw-r--r--   0 test       (501) staff       (20)        0 2024-05-11 11:41:12.000000 django-admin-daterange-listfilter-0.1.2/django_admin_daterange_listfilter/migrations/__init__.py
--rw-r--r--   0 test       (501) staff       (20)       57 2024-05-11 11:41:12.000000 django-admin-daterange-listfilter-0.1.2/django_admin_daterange_listfilter/models.py
-drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-12 08:34:15.272881 django-admin-daterange-listfilter-0.1.2/django_admin_daterange_listfilter/static/
-drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-12 08:34:15.272997 django-admin-daterange-listfilter-0.1.2/django_admin_daterange_listfilter/static/django_admin_daterange_listfilter/
-drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-12 08:34:15.277443 django-admin-daterange-listfilter-0.1.2/django_admin_daterange_listfilter/static/django_admin_daterange_listfilter/css/
--rw-r--r--   0 test       (501) staff       (20)      555 2024-05-11 11:44:57.000000 django-admin-daterange-listfilter-0.1.2/django_admin_daterange_listfilter/static/django_admin_daterange_listfilter/css/DateRangeFilter.css
-drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-12 08:34:15.277930 django-admin-daterange-listfilter-0.1.2/django_admin_daterange_listfilter/static/django_admin_daterange_listfilter/js/
--rw-r--r--   0 test       (501) staff       (20)     1474 2024-05-11 11:45:18.000000 django-admin-daterange-listfilter-0.1.2/django_admin_daterange_listfilter/static/django_admin_daterange_listfilter/js/DateRangeFilter.js
--rw-r--r--   0 test       (501) staff       (20)     1404 2024-05-11 11:45:55.000000 django-admin-daterange-listfilter-0.1.2/django_admin_daterange_listfilter/static/django_admin_daterange_listfilter/js/parseParam.js
-drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-12 08:34:15.273114 django-admin-daterange-listfilter-0.1.2/django_admin_daterange_listfilter/templates/
-drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-12 08:34:15.273162 django-admin-daterange-listfilter-0.1.2/django_admin_daterange_listfilter/templates/django_admin_daterange_listfilter/
-drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-12 08:34:15.278144 django-admin-daterange-listfilter-0.1.2/django_admin_daterange_listfilter/templates/django_admin_daterange_listfilter/filters/
--rw-r--r--   0 test       (501) staff       (20)     1036 2024-05-11 11:43:31.000000 django-admin-daterange-listfilter-0.1.2/django_admin_daterange_listfilter/templates/django_admin_daterange_listfilter/filters/DateRangeFilter.html
--rw-r--r--   0 test       (501) staff       (20)       60 2024-05-11 11:41:12.000000 django-admin-daterange-listfilter-0.1.2/django_admin_daterange_listfilter/tests.py
--rw-r--r--   0 test       (501) staff       (20)       63 2024-05-11 11:41:12.000000 django-admin-daterange-listfilter-0.1.2/django_admin_daterange_listfilter/views.py
-drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-12 08:34:15.276795 django-admin-daterange-listfilter-0.1.2/django_admin_daterange_listfilter.egg-info/
--rw-r--r--   0 test       (501) staff       (20)     1506 2024-05-12 08:34:15.000000 django-admin-daterange-listfilter-0.1.2/django_admin_daterange_listfilter.egg-info/PKG-INFO
--rw-r--r--   0 test       (501) staff       (20)     1295 2024-05-12 08:34:15.000000 django-admin-daterange-listfilter-0.1.2/django_admin_daterange_listfilter.egg-info/SOURCES.txt
--rw-r--r--   0 test       (501) staff       (20)        1 2024-05-12 08:34:15.000000 django-admin-daterange-listfilter-0.1.2/django_admin_daterange_listfilter.egg-info/dependency_links.txt
--rw-r--r--   0 test       (501) staff       (20)        1 2024-05-12 08:34:15.000000 django-admin-daterange-listfilter-0.1.2/django_admin_daterange_listfilter.egg-info/not-zip-safe
--rw-r--r--   0 test       (501) staff       (20)       98 2024-05-12 08:34:15.000000 django-admin-daterange-listfilter-0.1.2/django_admin_daterange_listfilter.egg-info/requires.txt
--rw-r--r--   0 test       (501) staff       (20)       34 2024-05-12 08:34:15.000000 django-admin-daterange-listfilter-0.1.2/django_admin_daterange_listfilter.egg-info/top_level.txt
--rw-r--r--   0 test       (501) staff       (20)       98 2024-05-12 08:07:27.000000 django-admin-daterange-listfilter-0.1.2/requirements.txt
--rw-r--r--   0 test       (501) staff       (20)       38 2024-05-12 08:34:15.278562 django-admin-daterange-listfilter-0.1.2/setup.cfg
--rw-r--r--   0 test       (501) staff       (20)     1483 2024-05-12 08:33:22.000000 django-admin-daterange-listfilter-0.1.2/setup.py
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-12 08:36:22.619975 django-admin-daterange-listfilter-0.1.3/
+-rw-r--r--   0 test       (501) staff       (20)     1036 2024-05-12 08:00:26.000000 django-admin-daterange-listfilter-0.1.3/LICENSE
+-rw-r--r--   0 test       (501) staff       (20)      276 2024-05-12 08:08:04.000000 django-admin-daterange-listfilter-0.1.3/MANIFEST.in
+-rw-r--r--   0 test       (501) staff       (20)     1506 2024-05-12 08:36:22.619841 django-admin-daterange-listfilter-0.1.3/PKG-INFO
+-rw-r--r--   0 test       (501) staff       (20)      838 2024-05-12 08:36:16.000000 django-admin-daterange-listfilter-0.1.3/README.md
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-12 08:36:22.618070 django-admin-daterange-listfilter-0.1.3/django_admin_daterange_listfilter/
+-rw-r--r--   0 test       (501) staff       (20)      131 2024-05-12 07:19:32.000000 django-admin-daterange-listfilter-0.1.3/django_admin_daterange_listfilter/__init__.py
+-rw-r--r--   0 test       (501) staff       (20)       63 2024-05-11 11:41:12.000000 django-admin-daterange-listfilter-0.1.3/django_admin_daterange_listfilter/admin.py
+-rw-r--r--   0 test       (501) staff       (20)      195 2024-05-11 11:41:12.000000 django-admin-daterange-listfilter-0.1.3/django_admin_daterange_listfilter/apps.py
+-rw-r--r--   0 test       (501) staff       (20)     3161 2024-05-12 07:38:44.000000 django-admin-daterange-listfilter-0.1.3/django_admin_daterange_listfilter/filters.py
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-12 08:36:22.615865 django-admin-daterange-listfilter-0.1.3/django_admin_daterange_listfilter/locale/
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-12 08:36:22.615923 django-admin-daterange-listfilter-0.1.3/django_admin_daterange_listfilter/locale/zh_Hans/
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-12 08:36:22.619058 django-admin-daterange-listfilter-0.1.3/django_admin_daterange_listfilter/locale/zh_Hans/LC_MESSAGES/
+-rw-r--r--   0 test       (501) staff       (20)      526 2024-05-12 08:36:10.000000 django-admin-daterange-listfilter-0.1.3/django_admin_daterange_listfilter/locale/zh_Hans/LC_MESSAGES/django.mo
+-rw-r--r--   0 test       (501) staff       (20)     1092 2024-05-12 08:31:25.000000 django-admin-daterange-listfilter-0.1.3/django_admin_daterange_listfilter/locale/zh_Hans/LC_MESSAGES/django.po
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-12 08:36:22.619175 django-admin-daterange-listfilter-0.1.3/django_admin_daterange_listfilter/migrations/
+-rw-r--r--   0 test       (501) staff       (20)        0 2024-05-11 11:41:12.000000 django-admin-daterange-listfilter-0.1.3/django_admin_daterange_listfilter/migrations/__init__.py
+-rw-r--r--   0 test       (501) staff       (20)       57 2024-05-11 11:41:12.000000 django-admin-daterange-listfilter-0.1.3/django_admin_daterange_listfilter/models.py
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-12 08:36:22.616115 django-admin-daterange-listfilter-0.1.3/django_admin_daterange_listfilter/static/
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-12 08:36:22.616277 django-admin-daterange-listfilter-0.1.3/django_admin_daterange_listfilter/static/django_admin_daterange_listfilter/
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-12 08:36:22.619280 django-admin-daterange-listfilter-0.1.3/django_admin_daterange_listfilter/static/django_admin_daterange_listfilter/css/
+-rw-r--r--   0 test       (501) staff       (20)      555 2024-05-11 11:44:57.000000 django-admin-daterange-listfilter-0.1.3/django_admin_daterange_listfilter/static/django_admin_daterange_listfilter/css/DateRangeFilter.css
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-12 08:36:22.619541 django-admin-daterange-listfilter-0.1.3/django_admin_daterange_listfilter/static/django_admin_daterange_listfilter/js/
+-rw-r--r--   0 test       (501) staff       (20)     1474 2024-05-11 11:45:18.000000 django-admin-daterange-listfilter-0.1.3/django_admin_daterange_listfilter/static/django_admin_daterange_listfilter/js/DateRangeFilter.js
+-rw-r--r--   0 test       (501) staff       (20)     1404 2024-05-11 11:45:55.000000 django-admin-daterange-listfilter-0.1.3/django_admin_daterange_listfilter/static/django_admin_daterange_listfilter/js/parseParam.js
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-12 08:36:22.616412 django-admin-daterange-listfilter-0.1.3/django_admin_daterange_listfilter/templates/
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-12 08:36:22.616464 django-admin-daterange-listfilter-0.1.3/django_admin_daterange_listfilter/templates/django_admin_daterange_listfilter/
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-12 08:36:22.619669 django-admin-daterange-listfilter-0.1.3/django_admin_daterange_listfilter/templates/django_admin_daterange_listfilter/filters/
+-rw-r--r--   0 test       (501) staff       (20)     1036 2024-05-11 11:43:31.000000 django-admin-daterange-listfilter-0.1.3/django_admin_daterange_listfilter/templates/django_admin_daterange_listfilter/filters/DateRangeFilter.html
+-rw-r--r--   0 test       (501) staff       (20)       60 2024-05-11 11:41:12.000000 django-admin-daterange-listfilter-0.1.3/django_admin_daterange_listfilter/tests.py
+-rw-r--r--   0 test       (501) staff       (20)       63 2024-05-11 11:41:12.000000 django-admin-daterange-listfilter-0.1.3/django_admin_daterange_listfilter/views.py
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-12 08:36:22.618820 django-admin-daterange-listfilter-0.1.3/django_admin_daterange_listfilter.egg-info/
+-rw-r--r--   0 test       (501) staff       (20)     1506 2024-05-12 08:36:22.000000 django-admin-daterange-listfilter-0.1.3/django_admin_daterange_listfilter.egg-info/PKG-INFO
+-rw-r--r--   0 test       (501) staff       (20)     1295 2024-05-12 08:36:22.000000 django-admin-daterange-listfilter-0.1.3/django_admin_daterange_listfilter.egg-info/SOURCES.txt
+-rw-r--r--   0 test       (501) staff       (20)        1 2024-05-12 08:36:22.000000 django-admin-daterange-listfilter-0.1.3/django_admin_daterange_listfilter.egg-info/dependency_links.txt
+-rw-r--r--   0 test       (501) staff       (20)        1 2024-05-12 08:36:22.000000 django-admin-daterange-listfilter-0.1.3/django_admin_daterange_listfilter.egg-info/not-zip-safe
+-rw-r--r--   0 test       (501) staff       (20)       98 2024-05-12 08:36:22.000000 django-admin-daterange-listfilter-0.1.3/django_admin_daterange_listfilter.egg-info/requires.txt
+-rw-r--r--   0 test       (501) staff       (20)       34 2024-05-12 08:36:22.000000 django-admin-daterange-listfilter-0.1.3/django_admin_daterange_listfilter.egg-info/top_level.txt
+-rw-r--r--   0 test       (501) staff       (20)       98 2024-05-12 08:07:27.000000 django-admin-daterange-listfilter-0.1.3/requirements.txt
+-rw-r--r--   0 test       (501) staff       (20)       38 2024-05-12 08:36:22.620020 django-admin-daterange-listfilter-0.1.3/setup.cfg
+-rw-r--r--   0 test       (501) staff       (20)     1483 2024-05-12 08:36:19.000000 django-admin-daterange-listfilter-0.1.3/setup.py
```

### Comparing `django-admin-daterange-listfilter-0.1.2/LICENSE` & `django-admin-daterange-listfilter-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django-admin-daterange-listfilter-0.1.2/PKG-INFO` & `django-admin-daterange-listfilter-0.1.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-admin-daterange-listfilter
-Version: 0.1.2
+Version: 0.1.3
 Summary: 通过日历自由选择时间范围。
 Home-page: UNKNOWN
 Author: Zhan YuCong
 Maintainer: Zhan YuCong
 License: MIT
 Keywords: django admin extentions,daterange listfilter
 Platform: UNKNOWN
@@ -61,12 +61,12 @@
 
 ## 版本记录
 
 ### v0.1.0
 
 - 版本首发。
 
-### v0.1.2
+### v0.1.3
 
 - 添加中文i18n翻译。
```

### Comparing `django-admin-daterange-listfilter-0.1.2/README.md` & `django-admin-daterange-listfilter-0.1.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -42,10 +42,10 @@
 
 ## 版本记录
 
 ### v0.1.0
 
 - 版本首发。
 
-### v0.1.2
+### v0.1.3
 
 - 添加中文i18n翻译。
```

### Comparing `django-admin-daterange-listfilter-0.1.2/django_admin_daterange_listfilter/filters.py` & `django-admin-daterange-listfilter-0.1.3/django_admin_daterange_listfilter/filters.py`

 * *Files identical despite different names*

### Comparing `django-admin-daterange-listfilter-0.1.2/django_admin_daterange_listfilter/locale/zh_Hans/LC_MESSAGES/django.po` & `django-admin-daterange-listfilter-0.1.3/django_admin_daterange_listfilter/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-admin-daterange-listfilter-0.1.2/django_admin_daterange_listfilter/static/django_admin_daterange_listfilter/css/DateRangeFilter.css` & `django-admin-daterange-listfilter-0.1.3/django_admin_daterange_listfilter/static/django_admin_daterange_listfilter/css/DateRangeFilter.css`

 * *Files identical despite different names*

### Comparing `django-admin-daterange-listfilter-0.1.2/django_admin_daterange_listfilter/static/django_admin_daterange_listfilter/js/DateRangeFilter.js` & `django-admin-daterange-listfilter-0.1.3/django_admin_daterange_listfilter/static/django_admin_daterange_listfilter/js/DateRangeFilter.js`

 * *Files identical despite different names*

### Comparing `django-admin-daterange-listfilter-0.1.2/django_admin_daterange_listfilter/static/django_admin_daterange_listfilter/js/parseParam.js` & `django-admin-daterange-listfilter-0.1.3/django_admin_daterange_listfilter/static/django_admin_daterange_listfilter/js/parseParam.js`

 * *Files identical despite different names*

### Comparing `django-admin-daterange-listfilter-0.1.2/django_admin_daterange_listfilter/templates/django_admin_daterange_listfilter/filters/DateRangeFilter.html` & `django-admin-daterange-listfilter-0.1.3/django_admin_daterange_listfilter/templates/django_admin_daterange_listfilter/filters/DateRangeFilter.html`

 * *Files identical despite different names*

### Comparing `django-admin-daterange-listfilter-0.1.2/django_admin_daterange_listfilter.egg-info/PKG-INFO` & `django-admin-daterange-listfilter-0.1.3/django_admin_daterange_listfilter.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-admin-daterange-listfilter
-Version: 0.1.2
+Version: 0.1.3
 Summary: 通过日历自由选择时间范围。
 Home-page: UNKNOWN
 Author: Zhan YuCong
 Maintainer: Zhan YuCong
 License: MIT
 Keywords: django admin extentions,daterange listfilter
 Platform: UNKNOWN
@@ -61,12 +61,12 @@
 
 ## 版本记录
 
 ### v0.1.0
 
 - 版本首发。
 
-### v0.1.2
+### v0.1.3
 
 - 添加中文i18n翻译。
```

### Comparing `django-admin-daterange-listfilter-0.1.2/django_admin_daterange_listfilter.egg-info/SOURCES.txt` & `django-admin-daterange-listfilter-0.1.3/django_admin_daterange_listfilter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-admin-daterange-listfilter-0.1.2/setup.py` & `django-admin-daterange-listfilter-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     long_description = fobj.read()
 
 with open(os.path.join(here, "requirements.txt"), "r", encoding="utf-8") as fobj:
     requires = [x.strip() for x in fobj.readlines() if x.strip()]
 
 setup(
     name="django-admin-daterange-listfilter",
-    version="0.1.2",
+    version="0.1.3",
     description="通过日历自由选择时间范围。",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Zhan YuCong",
     maintainer="Zhan YuCong",
     license="MIT",
     classifiers=[
```

