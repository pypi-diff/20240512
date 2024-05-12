# Comparing `tmp/django-easy-schedule-0.1.2.tar.gz` & `tmp/django-easy-schedule-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-easy-schedule-0.1.2.tar", last modified: Sun May 12 05:33:17 2024, max compression
+gzip compressed data, was "django-easy-schedule-0.1.3.tar", last modified: Sun May 12 05:48:30 2024, max compression
```

## Comparing `django-easy-schedule-0.1.2.tar` & `django-easy-schedule-0.1.3.tar`

### file list

```diff
@@ -1,13 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 05:33:17.615193 django-easy-schedule-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-12 05:33:05.000000 django-easy-schedule-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-05-12 05:33:17.615193 django-easy-schedule-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-05-12 05:33:05.000000 django-easy-schedule-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 05:33:17.615193 django-easy-schedule-0.1.2/django_easy_schedule.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-05-12 05:33:17.000000 django-easy-schedule-0.1.2/django_easy_schedule.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-12 05:33:17.000000 django-easy-schedule-0.1.2/django_easy_schedule.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 05:33:17.000000 django-easy-schedule-0.1.2/django_easy_schedule.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 05:33:17.000000 django-easy-schedule-0.1.2/django_easy_schedule.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-12 05:33:17.000000 django-easy-schedule-0.1.2/django_easy_schedule.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 05:33:17.000000 django-easy-schedule-0.1.2/django_easy_schedule.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 05:33:17.615193 django-easy-schedule-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-05-12 05:33:05.000000 django-easy-schedule-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 05:48:30.929681 django-easy-schedule-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-12 05:48:18.000000 django-easy-schedule-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-05-12 05:48:30.929681 django-easy-schedule-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-05-12 05:48:18.000000 django-easy-schedule-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 05:48:30.925681 django-easy-schedule-0.1.3/django_easy_schedule/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-12 05:48:18.000000 django-easy-schedule-0.1.3/django_easy_schedule/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-12 05:48:18.000000 django-easy-schedule-0.1.3/django_easy_schedule/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-12 05:48:18.000000 django-easy-schedule-0.1.3/django_easy_schedule/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-12 05:48:18.000000 django-easy-schedule-0.1.3/django_easy_schedule/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-12 05:48:18.000000 django-easy-schedule-0.1.3/django_easy_schedule/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 05:48:30.929681 django-easy-schedule-0.1.3/django_easy_schedule.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-05-12 05:48:30.000000 django-easy-schedule-0.1.3/django_easy_schedule.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-12 05:48:30.000000 django-easy-schedule-0.1.3/django_easy_schedule.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 05:48:30.000000 django-easy-schedule-0.1.3/django_easy_schedule.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 05:48:30.000000 django-easy-schedule-0.1.3/django_easy_schedule.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-12 05:48:30.000000 django-easy-schedule-0.1.3/django_easy_schedule.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-12 05:48:30.000000 django-easy-schedule-0.1.3/django_easy_schedule.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 05:48:30.929681 django-easy-schedule-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-05-12 05:48:18.000000 django-easy-schedule-0.1.3/setup.py
```

### Comparing `django-easy-schedule-0.1.2/LICENSE` & `django-easy-schedule-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django-easy-schedule-0.1.2/PKG-INFO` & `django-easy-schedule-0.1.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: django-easy-schedule
-Version: 0.1.2
+Version: 0.1.3
 Summary: Django integration with schedule module
-Home-page: https://github.com/waqqas/django-schedule
+Home-page: https://github.com/waqqas/django-easy-schedule
 Author: Waqqas Jabbar
 Author-email: waqqas.jabbar@egmail.com
 License: MIT
 Keywords: django schedule
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `django-easy-schedule-0.1.2/README.md` & `django-easy-schedule-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `django-easy-schedule-0.1.2/django_easy_schedule.egg-info/PKG-INFO` & `django-easy-schedule-0.1.3/django_easy_schedule.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: django-easy-schedule
-Version: 0.1.2
+Version: 0.1.3
 Summary: Django integration with schedule module
-Home-page: https://github.com/waqqas/django-schedule
+Home-page: https://github.com/waqqas/django-easy-schedule
 Author: Waqqas Jabbar
 Author-email: waqqas.jabbar@egmail.com
 License: MIT
 Keywords: django schedule
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `django-easy-schedule-0.1.2/setup.py` & `django-easy-schedule-0.1.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import find_packages, setup
 
 setup(
     name="django-easy-schedule",
-    version="0.1.2",
-    packages=find_packages(),
-    package_dir={'': '.'},
+    version="0.1.3",
+    packages=["django_easy_schedule"],
+    package_dir={"": "."},
     description="Django integration with schedule module",
     author="Waqqas Jabbar",
     author_email="waqqas.jabbar@egmail.com",
-    url="https://github.com/waqqas/django-schedule",
+    url="https://github.com/waqqas/django-easy-schedule",
     license="MIT",
     install_requires=[
         "Django>=4.0",
         "schedule>=1.0",
     ],
     python_requires='>=3.9',
     classifiers=[
```

