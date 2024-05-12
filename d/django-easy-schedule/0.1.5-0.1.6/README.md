# Comparing `tmp/django-easy-schedule-0.1.5.tar.gz` & `tmp/django-easy-schedule-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-easy-schedule-0.1.5.tar", last modified: Sun May 12 06:14:29 2024, max compression
+gzip compressed data, was "django-easy-schedule-0.1.6.tar", last modified: Sun May 12 06:39:06 2024, max compression
```

## Comparing `django-easy-schedule-0.1.5.tar` & `django-easy-schedule-0.1.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 06:14:29.943121 django-easy-schedule-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-12 06:14:15.000000 django-easy-schedule-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-05-12 06:14:29.939121 django-easy-schedule-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-05-12 06:14:15.000000 django-easy-schedule-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 06:14:29.939121 django-easy-schedule-0.1.5/django_easy_schedule/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 06:14:15.000000 django-easy-schedule-0.1.5/django_easy_schedule/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-12 06:14:15.000000 django-easy-schedule-0.1.5/django_easy_schedule/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-12 06:14:15.000000 django-easy-schedule-0.1.5/django_easy_schedule/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 06:14:29.939121 django-easy-schedule-0.1.5/django_easy_schedule/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 06:14:15.000000 django-easy-schedule-0.1.5/django_easy_schedule/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-12 06:14:15.000000 django-easy-schedule-0.1.5/django_easy_schedule/commands/jobs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 06:14:29.939121 django-easy-schedule-0.1.5/django_easy_schedule/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 06:14:15.000000 django-easy-schedule-0.1.5/django_easy_schedule/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-12 06:14:15.000000 django-easy-schedule-0.1.5/django_easy_schedule/models.py
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-12 06:14:15.000000 django-easy-schedule-0.1.5/django_easy_schedule/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-12 06:14:15.000000 django-easy-schedule-0.1.5/django_easy_schedule/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 06:14:29.939121 django-easy-schedule-0.1.5/django_easy_schedule.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-05-12 06:14:29.000000 django-easy-schedule-0.1.5/django_easy_schedule.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-12 06:14:29.000000 django-easy-schedule-0.1.5/django_easy_schedule.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 06:14:29.000000 django-easy-schedule-0.1.5/django_easy_schedule.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 06:14:29.000000 django-easy-schedule-0.1.5/django_easy_schedule.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-12 06:14:29.000000 django-easy-schedule-0.1.5/django_easy_schedule.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-12 06:14:29.000000 django-easy-schedule-0.1.5/django_easy_schedule.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 06:14:29.943121 django-easy-schedule-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-12 06:14:15.000000 django-easy-schedule-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 06:39:06.370210 django-easy-schedule-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-12 06:38:52.000000 django-easy-schedule-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-05-12 06:39:06.370210 django-easy-schedule-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-05-12 06:38:52.000000 django-easy-schedule-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 06:39:06.370210 django-easy-schedule-0.1.6/django_easy_schedule/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 06:38:52.000000 django-easy-schedule-0.1.6/django_easy_schedule/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-12 06:38:52.000000 django-easy-schedule-0.1.6/django_easy_schedule/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-12 06:38:52.000000 django-easy-schedule-0.1.6/django_easy_schedule/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 06:39:06.370210 django-easy-schedule-0.1.6/django_easy_schedule/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 06:38:52.000000 django-easy-schedule-0.1.6/django_easy_schedule/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-12 06:38:52.000000 django-easy-schedule-0.1.6/django_easy_schedule/commands/jobs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 06:39:06.370210 django-easy-schedule-0.1.6/django_easy_schedule/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 06:38:52.000000 django-easy-schedule-0.1.6/django_easy_schedule/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-12 06:38:52.000000 django-easy-schedule-0.1.6/django_easy_schedule/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-12 06:38:52.000000 django-easy-schedule-0.1.6/django_easy_schedule/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-12 06:38:52.000000 django-easy-schedule-0.1.6/django_easy_schedule/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 06:39:06.370210 django-easy-schedule-0.1.6/django_easy_schedule.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-05-12 06:39:06.000000 django-easy-schedule-0.1.6/django_easy_schedule.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-12 06:39:06.000000 django-easy-schedule-0.1.6/django_easy_schedule.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 06:39:06.000000 django-easy-schedule-0.1.6/django_easy_schedule.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 06:39:06.000000 django-easy-schedule-0.1.6/django_easy_schedule.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-12 06:39:06.000000 django-easy-schedule-0.1.6/django_easy_schedule.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-12 06:39:06.000000 django-easy-schedule-0.1.6/django_easy_schedule.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 06:39:06.370210 django-easy-schedule-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-12 06:38:52.000000 django-easy-schedule-0.1.6/setup.py
```

### Comparing `django-easy-schedule-0.1.5/LICENSE` & `django-easy-schedule-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `django-easy-schedule-0.1.5/PKG-INFO` & `django-easy-schedule-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-easy-schedule
-Version: 0.1.5
+Version: 0.1.6
 Summary: Django integration with schedule module
 Home-page: https://github.com/waqqas/django-easy-schedule
 Author: Waqqas Jabbar
 Author-email: waqqas.jabbar@egmail.com
 License: MIT
 Keywords: django,schedule
 Platform: UNKNOWN
```

### Comparing `django-easy-schedule-0.1.5/README.md` & `django-easy-schedule-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `django-easy-schedule-0.1.5/django_easy_schedule/commands/jobs.py` & `django-easy-schedule-0.1.6/django_easy_schedule/commands/jobs.py`

 * *Files identical despite different names*

### Comparing `django-easy-schedule-0.1.5/django_easy_schedule.egg-info/PKG-INFO` & `django-easy-schedule-0.1.6/django_easy_schedule.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-easy-schedule
-Version: 0.1.5
+Version: 0.1.6
 Summary: Django integration with schedule module
 Home-page: https://github.com/waqqas/django-easy-schedule
 Author: Waqqas Jabbar
 Author-email: waqqas.jabbar@egmail.com
 License: MIT
 Keywords: django,schedule
 Platform: UNKNOWN
```

### Comparing `django-easy-schedule-0.1.5/django_easy_schedule.egg-info/SOURCES.txt` & `django-easy-schedule-0.1.6/django_easy_schedule.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-easy-schedule-0.1.5/setup.py` & `django-easy-schedule-0.1.6/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="django-easy-schedule",
-    version="0.1.5",
+    version="0.1.6",
     packages=find_packages(),
     description="Django integration with schedule module",
     author="Waqqas Jabbar",
     author_email="waqqas.jabbar@egmail.com",
     url="https://github.com/waqqas/django-easy-schedule",
     license="MIT",
     install_requires=[
```

