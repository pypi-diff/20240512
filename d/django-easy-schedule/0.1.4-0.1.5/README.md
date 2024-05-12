# Comparing `tmp/django-easy-schedule-0.1.4.tar.gz` & `tmp/django-easy-schedule-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-easy-schedule-0.1.4.tar", last modified: Sun May 12 05:52:07 2024, max compression
+gzip compressed data, was "django-easy-schedule-0.1.5.tar", last modified: Sun May 12 06:14:29 2024, max compression
```

## Comparing `django-easy-schedule-0.1.4.tar` & `django-easy-schedule-0.1.5.tar`

### file list

```diff
@@ -1,19 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 05:52:07.135871 django-easy-schedule-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-12 05:51:59.000000 django-easy-schedule-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-05-12 05:52:07.135871 django-easy-schedule-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-05-12 05:51:59.000000 django-easy-schedule-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 05:52:07.135871 django-easy-schedule-0.1.4/django_easy_schedule/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-12 05:51:59.000000 django-easy-schedule-0.1.4/django_easy_schedule/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-12 05:51:59.000000 django-easy-schedule-0.1.4/django_easy_schedule/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-12 05:51:59.000000 django-easy-schedule-0.1.4/django_easy_schedule/models.py
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-12 05:51:59.000000 django-easy-schedule-0.1.4/django_easy_schedule/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-12 05:51:59.000000 django-easy-schedule-0.1.4/django_easy_schedule/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 05:52:07.135871 django-easy-schedule-0.1.4/django_easy_schedule.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-05-12 05:52:07.000000 django-easy-schedule-0.1.4/django_easy_schedule.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-12 05:52:07.000000 django-easy-schedule-0.1.4/django_easy_schedule.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 05:52:07.000000 django-easy-schedule-0.1.4/django_easy_schedule.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 05:52:07.000000 django-easy-schedule-0.1.4/django_easy_schedule.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-12 05:52:07.000000 django-easy-schedule-0.1.4/django_easy_schedule.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-12 05:52:07.000000 django-easy-schedule-0.1.4/django_easy_schedule.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 05:52:07.135871 django-easy-schedule-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-05-12 05:51:59.000000 django-easy-schedule-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 06:14:29.943121 django-easy-schedule-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-12 06:14:15.000000 django-easy-schedule-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-05-12 06:14:29.939121 django-easy-schedule-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-05-12 06:14:15.000000 django-easy-schedule-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 06:14:29.939121 django-easy-schedule-0.1.5/django_easy_schedule/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 06:14:15.000000 django-easy-schedule-0.1.5/django_easy_schedule/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-12 06:14:15.000000 django-easy-schedule-0.1.5/django_easy_schedule/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-12 06:14:15.000000 django-easy-schedule-0.1.5/django_easy_schedule/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 06:14:29.939121 django-easy-schedule-0.1.5/django_easy_schedule/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 06:14:15.000000 django-easy-schedule-0.1.5/django_easy_schedule/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-12 06:14:15.000000 django-easy-schedule-0.1.5/django_easy_schedule/commands/jobs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 06:14:29.939121 django-easy-schedule-0.1.5/django_easy_schedule/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 06:14:15.000000 django-easy-schedule-0.1.5/django_easy_schedule/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-12 06:14:15.000000 django-easy-schedule-0.1.5/django_easy_schedule/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-12 06:14:15.000000 django-easy-schedule-0.1.5/django_easy_schedule/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-12 06:14:15.000000 django-easy-schedule-0.1.5/django_easy_schedule/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 06:14:29.939121 django-easy-schedule-0.1.5/django_easy_schedule.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-05-12 06:14:29.000000 django-easy-schedule-0.1.5/django_easy_schedule.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-12 06:14:29.000000 django-easy-schedule-0.1.5/django_easy_schedule.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 06:14:29.000000 django-easy-schedule-0.1.5/django_easy_schedule.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 06:14:29.000000 django-easy-schedule-0.1.5/django_easy_schedule.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-12 06:14:29.000000 django-easy-schedule-0.1.5/django_easy_schedule.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-12 06:14:29.000000 django-easy-schedule-0.1.5/django_easy_schedule.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 06:14:29.943121 django-easy-schedule-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-12 06:14:15.000000 django-easy-schedule-0.1.5/setup.py
```

### Comparing `django-easy-schedule-0.1.4/LICENSE` & `django-easy-schedule-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `django-easy-schedule-0.1.4/PKG-INFO` & `django-easy-schedule-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: django-easy-schedule
-Version: 0.1.4
+Version: 0.1.5
 Summary: Django integration with schedule module
 Home-page: https://github.com/waqqas/django-easy-schedule
 Author: Waqqas Jabbar
 Author-email: waqqas.jabbar@egmail.com
 License: MIT
-Keywords: django schedule
+Keywords: django,schedule
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `django-easy-schedule-0.1.4/README.md` & `django-easy-schedule-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `django-easy-schedule-0.1.4/django_easy_schedule.egg-info/PKG-INFO` & `django-easy-schedule-0.1.5/django_easy_schedule.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: django-easy-schedule
-Version: 0.1.4
+Version: 0.1.5
 Summary: Django integration with schedule module
 Home-page: https://github.com/waqqas/django-easy-schedule
 Author: Waqqas Jabbar
 Author-email: waqqas.jabbar@egmail.com
 License: MIT
-Keywords: django schedule
+Keywords: django,schedule
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `django-easy-schedule-0.1.4/setup.py` & `django-easy-schedule-0.1.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from setuptools import find_packages, setup
 
 setup(
     name="django-easy-schedule",
-    version="0.1.4",
-    packages=["django_easy_schedule"],
-    package_dir={"": "."},
+    version="0.1.5",
+    packages=find_packages(),
     description="Django integration with schedule module",
     author="Waqqas Jabbar",
     author_email="waqqas.jabbar@egmail.com",
     url="https://github.com/waqqas/django-easy-schedule",
     license="MIT",
     install_requires=[
         "Django>=4.0",
@@ -28,9 +27,9 @@
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
     ],
     include_package_data=True,
     zip_safe=False,
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
-    keywords="django schedule",
+    keywords=["django", "schedule"],
 )
```

