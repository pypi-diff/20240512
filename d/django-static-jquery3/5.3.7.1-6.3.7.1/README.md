# Comparing `tmp/django-static-jquery3-5.3.7.1.tar.gz` & `tmp/django-static-jquery3-6.3.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-static-jquery3-5.3.7.1.tar", last modified: Tue Sep 12 03:22:54 2023, max compression
+gzip compressed data, was "django-static-jquery3-6.3.7.1.tar", last modified: Sun May 12 13:00:09 2024, max compression
```

## Comparing `django-static-jquery3-5.3.7.1.tar` & `django-static-jquery3-6.3.7.1.tar`

### file list

```diff
@@ -1,64 +1,65 @@
-drwxr-xr-x   0 test       (501) staff       (20)        0 2023-09-12 03:22:54.321590 django-static-jquery3-5.3.7.1/
--rw-r--r--   0 test       (501) staff       (20)     1067 2023-09-12 02:08:12.000000 django-static-jquery3-5.3.7.1/LICENSE
--rw-r--r--   0 test       (501) staff       (20)      158 2023-09-12 02:08:12.000000 django-static-jquery3-5.3.7.1/MANIFEST.in
--rw-r--r--   0 test       (501) staff       (20)     2855 2023-09-12 03:22:54.321472 django-static-jquery3-5.3.7.1/PKG-INFO
--rw-r--r--   0 test       (501) staff       (20)     2239 2023-09-12 02:45:37.000000 django-static-jquery3-5.3.7.1/README.md
-drwxr-xr-x   0 test       (501) staff       (20)        0 2023-09-12 03:22:54.310161 django-static-jquery3-5.3.7.1/django_static_jquery3/
--rw-r--r--   0 test       (501) staff       (20)     6148 2023-09-12 02:42:07.000000 django-static-jquery3-5.3.7.1/django_static_jquery3/.DS_Store
--rw-r--r--   0 test       (501) staff       (20)        0 2023-09-12 02:08:12.000000 django-static-jquery3-5.3.7.1/django_static_jquery3/__init__.py
--rw-r--r--   0 test       (501) staff       (20)        0 2023-09-12 02:08:12.000000 django-static-jquery3-5.3.7.1/django_static_jquery3/admin.py
--rw-r--r--   0 test       (501) staff       (20)        0 2023-09-12 02:08:12.000000 django-static-jquery3-5.3.7.1/django_static_jquery3/apps.py
-drwxr-xr-x   0 test       (501) staff       (20)        0 2023-09-12 03:22:54.310829 django-static-jquery3-5.3.7.1/django_static_jquery3/migrations/
--rw-r--r--   0 test       (501) staff       (20)        0 2023-09-12 02:08:12.000000 django-static-jquery3-5.3.7.1/django_static_jquery3/migrations/__init__.py
--rw-r--r--   0 test       (501) staff       (20)        0 2023-09-12 02:08:12.000000 django-static-jquery3-5.3.7.1/django_static_jquery3/models.py
-drwxr-xr-x   0 test       (501) staff       (20)        0 2023-09-12 03:22:54.310921 django-static-jquery3-5.3.7.1/django_static_jquery3/static/
--rw-r--r--   0 test       (501) staff       (20)     6148 2023-09-12 02:42:18.000000 django-static-jquery3-5.3.7.1/django_static_jquery3/static/.DS_Store
-drwxr-xr-x   0 test       (501) staff       (20)        0 2023-09-12 03:22:54.315220 django-static-jquery3-5.3.7.1/django_static_jquery3/static/jquery/
--rw-r--r--   0 test       (501) staff       (20)     6148 2023-09-12 03:07:03.000000 django-static-jquery3-5.3.7.1/django_static_jquery3/static/jquery/.DS_Store
--rw-rw-r--   0 test       (501) staff       (20)   285314 2023-08-28 13:37:56.000000 django-static-jquery3-5.3.7.1/django_static_jquery3/static/jquery/jquery.js
--rw-rw-r--   0 test       (501) staff       (20)    87533 2023-08-28 13:37:56.000000 django-static-jquery3-5.3.7.1/django_static_jquery3/static/jquery/jquery.min.js
--rw-rw-r--   0 test       (501) staff       (20)   134755 2023-08-28 13:37:56.000000 django-static-jquery3-5.3.7.1/django_static_jquery3/static/jquery/jquery.min.map
--rw-rw-r--   0 test       (501) staff       (20)   232015 2023-08-28 13:37:56.000000 django-static-jquery3-5.3.7.1/django_static_jquery3/static/jquery/jquery.slim.js
--rw-rw-r--   0 test       (501) staff       (20)    70264 2023-08-28 13:37:56.000000 django-static-jquery3-5.3.7.1/django_static_jquery3/static/jquery/jquery.slim.min.js
--rw-rw-r--   0 test       (501) staff       (20)   107143 2023-08-28 13:37:56.000000 django-static-jquery3-5.3.7.1/django_static_jquery3/static/jquery/jquery.slim.min.map
-drwxr-xr-x   0 test       (501) staff       (20)        0 2023-09-12 03:22:54.315486 django-static-jquery3-5.3.7.1/django_static_jquery3/static/jquery/licenses/
--rw-r--r--   0 test       (501) staff       (20)     8196 2023-09-12 02:42:13.000000 django-static-jquery3-5.3.7.1/django_static_jquery3/static/jquery/licenses/.DS_Store
-drwxr-xr-x   0 test       (501) staff       (20)        0 2023-09-12 03:22:54.315720 django-static-jquery3-5.3.7.1/django_static_jquery3/static/jquery/licenses/jquery/
--rw-rw-r--   0 test       (501) staff       (20)     1097 2023-08-28 13:37:56.000000 django-static-jquery3-5.3.7.1/django_static_jquery3/static/jquery/licenses/jquery/LICENSE.txt
-drwxr-xr-x   0 test       (501) staff       (20)        0 2023-09-12 03:22:54.315996 django-static-jquery3-5.3.7.1/django_static_jquery3/static/jquery/licenses/jquery.cookie/
--rw-rw-r--   0 test       (501) staff       (20)     1051 2014-04-27 20:07:15.000000 django-static-jquery3-5.3.7.1/django_static_jquery3/static/jquery/licenses/jquery.cookie/MIT-LICENSE.txt
-drwxr-xr-x   0 test       (501) staff       (20)        0 2023-09-12 03:22:54.316480 django-static-jquery3-5.3.7.1/django_static_jquery3/static/jquery/licenses/jquery.jstree/
--rw-r--r--   0 test       (501) staff       (20)     6148 2023-09-12 02:40:05.000000 django-static-jquery3-5.3.7.1/django_static_jquery3/static/jquery/licenses/jquery.jstree/.DS_Store
--rw-r--r--   0 test       (501) staff       (20)     1079 2023-09-12 02:39:54.000000 django-static-jquery3-5.3.7.1/django_static_jquery3/static/jquery/licenses/jquery.jstree/LICENSE-MIT
-drwxr-xr-x   0 test       (501) staff       (20)        0 2023-09-12 03:22:54.317164 django-static-jquery3-5.3.7.1/django_static_jquery3/static/jquery/plugins/
--rw-r--r--   0 test       (501) staff       (20)     6148 2023-09-12 02:38:26.000000 django-static-jquery3-5.3.7.1/django_static_jquery3/static/jquery/plugins/.DS_Store
--rw-rw-r--   0 test       (501) staff       (20)     3121 2014-04-27 20:07:15.000000 django-static-jquery3-5.3.7.1/django_static_jquery3/static/jquery/plugins/jquery.cookie.js
-drwxr-xr-x   0 test       (501) staff       (20)        0 2023-09-12 03:22:54.318986 django-static-jquery3-5.3.7.1/django_static_jquery3/static/jquery/plugins/jquery.jstree/
--rw-r--r--   0 test       (501) staff       (20)     6148 2023-09-12 02:38:30.000000 django-static-jquery3-5.3.7.1/django_static_jquery3/static/jquery/plugins/jquery.jstree/.DS_Store
--rw-rw-r--   0 test       (501) staff       (20)   310341 2023-02-19 23:38:56.000000 django-static-jquery3-5.3.7.1/django_static_jquery3/static/jquery/plugins/jquery.jstree/jstree.js
--rw-rw-r--   0 test       (501) staff       (20)   141915 2023-02-19 23:38:56.000000 django-static-jquery3-5.3.7.1/django_static_jquery3/static/jquery/plugins/jquery.jstree/jstree.min.js
-drwxr-xr-x   0 test       (501) staff       (20)        0 2023-09-12 03:22:54.308594 django-static-jquery3-5.3.7.1/django_static_jquery3/static/jquery/plugins/jquery.jstree/themes/
-drwxr-xr-x   0 test       (501) staff       (20)        0 2023-09-12 03:22:54.320410 django-static-jquery3-5.3.7.1/django_static_jquery3/static/jquery/plugins/jquery.jstree/themes/default/
--rw-rw-r--   0 test       (501) staff       (20)     5660 2023-02-19 23:38:56.000000 django-static-jquery3-5.3.7.1/django_static_jquery3/static/jquery/plugins/jquery.jstree/themes/default/32px.png
--rw-rw-r--   0 test       (501) staff       (20)     2215 2023-02-19 23:38:56.000000 django-static-jquery3-5.3.7.1/django_static_jquery3/static/jquery/plugins/jquery.jstree/themes/default/40px.png
--rw-rw-r--   0 test       (501) staff       (20)    31730 2023-02-19 23:38:56.000000 django-static-jquery3-5.3.7.1/django_static_jquery3/static/jquery/plugins/jquery.jstree/themes/default/style.css
--rw-rw-r--   0 test       (501) staff       (20)    27363 2023-02-19 23:38:56.000000 django-static-jquery3-5.3.7.1/django_static_jquery3/static/jquery/plugins/jquery.jstree/themes/default/style.min.css
--rw-rw-r--   0 test       (501) staff       (20)     1464 2023-02-19 23:38:56.000000 django-static-jquery3-5.3.7.1/django_static_jquery3/static/jquery/plugins/jquery.jstree/themes/default/throbber.gif
-drwxr-xr-x   0 test       (501) staff       (20)        0 2023-09-12 03:22:54.321279 django-static-jquery3-5.3.7.1/django_static_jquery3/static/jquery/plugins/jquery.jstree/themes/default-dark/
--rw-rw-r--   0 test       (501) staff       (20)     1525 2023-02-19 23:38:56.000000 django-static-jquery3-5.3.7.1/django_static_jquery3/static/jquery/plugins/jquery.jstree/themes/default-dark/32px.png
--rw-rw-r--   0 test       (501) staff       (20)     6526 2023-02-19 23:38:56.000000 django-static-jquery3-5.3.7.1/django_static_jquery3/static/jquery/plugins/jquery.jstree/themes/default-dark/40px.png
--rw-rw-r--   0 test       (501) staff       (20)    34464 2023-02-19 23:38:56.000000 django-static-jquery3-5.3.7.1/django_static_jquery3/static/jquery/plugins/jquery.jstree/themes/default-dark/style.css
--rw-rw-r--   0 test       (501) staff       (20)    29966 2023-02-19 23:38:56.000000 django-static-jquery3-5.3.7.1/django_static_jquery3/static/jquery/plugins/jquery.jstree/themes/default-dark/style.min.css
--rw-rw-r--   0 test       (501) staff       (20)     1464 2023-02-19 23:38:56.000000 django-static-jquery3-5.3.7.1/django_static_jquery3/static/jquery/plugins/jquery.jstree/themes/default-dark/throbber.gif
--rw-r--r--   0 test       (501) staff       (20)     2025 2023-09-12 02:08:12.000000 django-static-jquery3-5.3.7.1/django_static_jquery3/static/jquery/plugins/jquery.utils.js
--rw-r--r--   0 test       (501) staff       (20)        0 2023-09-12 02:08:12.000000 django-static-jquery3-5.3.7.1/django_static_jquery3/tests.py
--rw-r--r--   0 test       (501) staff       (20)        0 2023-09-12 02:08:12.000000 django-static-jquery3-5.3.7.1/django_static_jquery3/views.py
-drwxr-xr-x   0 test       (501) staff       (20)        0 2023-09-12 03:22:54.310713 django-static-jquery3-5.3.7.1/django_static_jquery3.egg-info/
--rw-r--r--   0 test       (501) staff       (20)     2855 2023-09-12 03:22:54.000000 django-static-jquery3-5.3.7.1/django_static_jquery3.egg-info/PKG-INFO
--rw-r--r--   0 test       (501) staff       (20)     2521 2023-09-12 03:22:54.000000 django-static-jquery3-5.3.7.1/django_static_jquery3.egg-info/SOURCES.txt
--rw-r--r--   0 test       (501) staff       (20)        1 2023-09-12 03:22:54.000000 django-static-jquery3-5.3.7.1/django_static_jquery3.egg-info/dependency_links.txt
--rw-r--r--   0 test       (501) staff       (20)        1 2023-09-12 03:22:54.000000 django-static-jquery3-5.3.7.1/django_static_jquery3.egg-info/not-zip-safe
--rw-r--r--   0 test       (501) staff       (20)       22 2023-09-12 03:22:54.000000 django-static-jquery3-5.3.7.1/django_static_jquery3.egg-info/top_level.txt
--rw-r--r--   0 test       (501) staff       (20)        0 2023-09-12 02:08:12.000000 django-static-jquery3-5.3.7.1/requirements.txt
--rw-r--r--   0 test       (501) staff       (20)       38 2023-09-12 03:22:54.321624 django-static-jquery3-5.3.7.1/setup.cfg
--rw-r--r--   0 test       (501) staff       (20)     1330 2023-09-12 02:51:05.000000 django-static-jquery3-5.3.7.1/setup.py
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-12 13:00:09.025519 django-static-jquery3-6.3.7.1/
+-rw-r--r--   0 test       (501) staff       (20)     1036 2024-05-12 12:44:57.000000 django-static-jquery3-6.3.7.1/LICENSE
+-rw-r--r--   0 test       (501) staff       (20)      158 2023-09-12 02:08:12.000000 django-static-jquery3-6.3.7.1/MANIFEST.in
+-rw-r--r--   0 test       (501) staff       (20)     3036 2024-05-12 13:00:09.025398 django-static-jquery3-6.3.7.1/PKG-INFO
+-rw-r--r--   0 test       (501) staff       (20)     2467 2024-05-12 12:56:35.000000 django-static-jquery3-6.3.7.1/README.md
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-12 13:00:09.017855 django-static-jquery3-6.3.7.1/django_static_jquery3/
+-rw-r--r--   0 test       (501) staff       (20)     6148 2024-05-12 12:49:57.000000 django-static-jquery3-6.3.7.1/django_static_jquery3/.DS_Store
+-rw-r--r--   0 test       (501) staff       (20)        0 2023-09-12 02:08:12.000000 django-static-jquery3-6.3.7.1/django_static_jquery3/__init__.py
+-rw-r--r--   0 test       (501) staff       (20)        0 2023-09-12 02:08:12.000000 django-static-jquery3-6.3.7.1/django_static_jquery3/admin.py
+-rw-r--r--   0 test       (501) staff       (20)        0 2023-09-12 02:08:12.000000 django-static-jquery3-6.3.7.1/django_static_jquery3/apps.py
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-12 13:00:09.018718 django-static-jquery3-6.3.7.1/django_static_jquery3/migrations/
+-rw-r--r--   0 test       (501) staff       (20)        0 2023-09-12 02:08:12.000000 django-static-jquery3-6.3.7.1/django_static_jquery3/migrations/__init__.py
+-rw-r--r--   0 test       (501) staff       (20)        0 2023-09-12 02:08:12.000000 django-static-jquery3-6.3.7.1/django_static_jquery3/models.py
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-12 13:00:09.018815 django-static-jquery3-6.3.7.1/django_static_jquery3/static/
+-rw-r--r--   0 test       (501) staff       (20)     6148 2024-05-12 12:50:29.000000 django-static-jquery3-6.3.7.1/django_static_jquery3/static/.DS_Store
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-12 13:00:09.020915 django-static-jquery3-6.3.7.1/django_static_jquery3/static/jquery/
+-rw-r--r--   0 test       (501) staff       (20)     6148 2024-05-12 12:50:34.000000 django-static-jquery3-6.3.7.1/django_static_jquery3/static/jquery/.DS_Store
+-rw-rw-r--   0 test       (501) staff       (20)   285314 2023-08-28 13:37:56.000000 django-static-jquery3-6.3.7.1/django_static_jquery3/static/jquery/jquery.js
+-rw-rw-r--   0 test       (501) staff       (20)    87533 2023-08-28 13:37:56.000000 django-static-jquery3-6.3.7.1/django_static_jquery3/static/jquery/jquery.min.js
+-rw-rw-r--   0 test       (501) staff       (20)   134755 2023-08-28 13:37:56.000000 django-static-jquery3-6.3.7.1/django_static_jquery3/static/jquery/jquery.min.map
+-rw-rw-r--   0 test       (501) staff       (20)   232015 2023-08-28 13:37:56.000000 django-static-jquery3-6.3.7.1/django_static_jquery3/static/jquery/jquery.slim.js
+-rw-rw-r--   0 test       (501) staff       (20)    70264 2023-08-28 13:37:56.000000 django-static-jquery3-6.3.7.1/django_static_jquery3/static/jquery/jquery.slim.min.js
+-rw-rw-r--   0 test       (501) staff       (20)   107143 2023-08-28 13:37:56.000000 django-static-jquery3-6.3.7.1/django_static_jquery3/static/jquery/jquery.slim.min.map
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-12 13:00:09.021102 django-static-jquery3-6.3.7.1/django_static_jquery3/static/jquery/licenses/
+-rw-r--r--   0 test       (501) staff       (20)     8196 2023-09-12 02:42:13.000000 django-static-jquery3-6.3.7.1/django_static_jquery3/static/jquery/licenses/.DS_Store
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-12 13:00:09.021293 django-static-jquery3-6.3.7.1/django_static_jquery3/static/jquery/licenses/jquery/
+-rw-rw-r--   0 test       (501) staff       (20)     1097 2023-08-28 13:37:56.000000 django-static-jquery3-6.3.7.1/django_static_jquery3/static/jquery/licenses/jquery/LICENSE.txt
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-12 13:00:09.021435 django-static-jquery3-6.3.7.1/django_static_jquery3/static/jquery/licenses/jquery.cookie/
+-rw-rw-r--   0 test       (501) staff       (20)     1051 2014-04-27 20:07:15.000000 django-static-jquery3-6.3.7.1/django_static_jquery3/static/jquery/licenses/jquery.cookie/MIT-LICENSE.txt
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-12 13:00:09.021755 django-static-jquery3-6.3.7.1/django_static_jquery3/static/jquery/licenses/jquery.jstree/
+-rw-r--r--   0 test       (501) staff       (20)     6148 2023-09-12 02:40:05.000000 django-static-jquery3-6.3.7.1/django_static_jquery3/static/jquery/licenses/jquery.jstree/.DS_Store
+-rw-r--r--   0 test       (501) staff       (20)     1079 2023-09-12 02:39:54.000000 django-static-jquery3-6.3.7.1/django_static_jquery3/static/jquery/licenses/jquery.jstree/LICENSE-MIT
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-12 13:00:09.022303 django-static-jquery3-6.3.7.1/django_static_jquery3/static/jquery/plugins/
+-rw-r--r--   0 test       (501) staff       (20)     6148 2023-09-12 02:38:26.000000 django-static-jquery3-6.3.7.1/django_static_jquery3/static/jquery/plugins/.DS_Store
+-rw-rw-r--   0 test       (501) staff       (20)     3121 2014-04-27 20:07:15.000000 django-static-jquery3-6.3.7.1/django_static_jquery3/static/jquery/plugins/jquery.cookie.js
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-12 13:00:09.023299 django-static-jquery3-6.3.7.1/django_static_jquery3/static/jquery/plugins/jquery.jstree/
+-rw-r--r--   0 test       (501) staff       (20)     6148 2023-09-12 02:38:30.000000 django-static-jquery3-6.3.7.1/django_static_jquery3/static/jquery/plugins/jquery.jstree/.DS_Store
+-rw-rw-r--   0 test       (501) staff       (20)   310341 2023-02-19 23:38:56.000000 django-static-jquery3-6.3.7.1/django_static_jquery3/static/jquery/plugins/jquery.jstree/jstree.js
+-rw-rw-r--   0 test       (501) staff       (20)   141915 2023-02-19 23:38:56.000000 django-static-jquery3-6.3.7.1/django_static_jquery3/static/jquery/plugins/jquery.jstree/jstree.min.js
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-12 13:00:09.016432 django-static-jquery3-6.3.7.1/django_static_jquery3/static/jquery/plugins/jquery.jstree/themes/
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-12 13:00:09.024094 django-static-jquery3-6.3.7.1/django_static_jquery3/static/jquery/plugins/jquery.jstree/themes/default/
+-rw-rw-r--   0 test       (501) staff       (20)     5660 2023-02-19 23:38:56.000000 django-static-jquery3-6.3.7.1/django_static_jquery3/static/jquery/plugins/jquery.jstree/themes/default/32px.png
+-rw-rw-r--   0 test       (501) staff       (20)     2215 2023-02-19 23:38:56.000000 django-static-jquery3-6.3.7.1/django_static_jquery3/static/jquery/plugins/jquery.jstree/themes/default/40px.png
+-rw-rw-r--   0 test       (501) staff       (20)    31730 2023-02-19 23:38:56.000000 django-static-jquery3-6.3.7.1/django_static_jquery3/static/jquery/plugins/jquery.jstree/themes/default/style.css
+-rw-rw-r--   0 test       (501) staff       (20)    27363 2023-02-19 23:38:56.000000 django-static-jquery3-6.3.7.1/django_static_jquery3/static/jquery/plugins/jquery.jstree/themes/default/style.min.css
+-rw-rw-r--   0 test       (501) staff       (20)     1464 2023-02-19 23:38:56.000000 django-static-jquery3-6.3.7.1/django_static_jquery3/static/jquery/plugins/jquery.jstree/themes/default/throbber.gif
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-12 13:00:09.025213 django-static-jquery3-6.3.7.1/django_static_jquery3/static/jquery/plugins/jquery.jstree/themes/default-dark/
+-rw-rw-r--   0 test       (501) staff       (20)     1525 2023-02-19 23:38:56.000000 django-static-jquery3-6.3.7.1/django_static_jquery3/static/jquery/plugins/jquery.jstree/themes/default-dark/32px.png
+-rw-rw-r--   0 test       (501) staff       (20)     6526 2023-02-19 23:38:56.000000 django-static-jquery3-6.3.7.1/django_static_jquery3/static/jquery/plugins/jquery.jstree/themes/default-dark/40px.png
+-rw-rw-r--   0 test       (501) staff       (20)    34464 2023-02-19 23:38:56.000000 django-static-jquery3-6.3.7.1/django_static_jquery3/static/jquery/plugins/jquery.jstree/themes/default-dark/style.css
+-rw-rw-r--   0 test       (501) staff       (20)    29966 2023-02-19 23:38:56.000000 django-static-jquery3-6.3.7.1/django_static_jquery3/static/jquery/plugins/jquery.jstree/themes/default-dark/style.min.css
+-rw-rw-r--   0 test       (501) staff       (20)     1464 2023-02-19 23:38:56.000000 django-static-jquery3-6.3.7.1/django_static_jquery3/static/jquery/plugins/jquery.jstree/themes/default-dark/throbber.gif
+-rw-r--r--   0 test       (501) staff       (20)     1789 2024-05-12 12:58:56.000000 django-static-jquery3-6.3.7.1/django_static_jquery3/static/jquery/plugins/jquery.parseQuery.js
+-rw-r--r--   0 test       (501) staff       (20)     2025 2023-09-12 02:08:12.000000 django-static-jquery3-6.3.7.1/django_static_jquery3/static/jquery/plugins/jquery.utils.js
+-rw-r--r--   0 test       (501) staff       (20)        0 2023-09-12 02:08:12.000000 django-static-jquery3-6.3.7.1/django_static_jquery3/tests.py
+-rw-r--r--   0 test       (501) staff       (20)        0 2023-09-12 02:08:12.000000 django-static-jquery3-6.3.7.1/django_static_jquery3/views.py
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-12 13:00:09.018588 django-static-jquery3-6.3.7.1/django_static_jquery3.egg-info/
+-rw-r--r--   0 test       (501) staff       (20)     3036 2024-05-12 13:00:08.000000 django-static-jquery3-6.3.7.1/django_static_jquery3.egg-info/PKG-INFO
+-rw-r--r--   0 test       (501) staff       (20)     2586 2024-05-12 13:00:08.000000 django-static-jquery3-6.3.7.1/django_static_jquery3.egg-info/SOURCES.txt
+-rw-r--r--   0 test       (501) staff       (20)        1 2024-05-12 13:00:08.000000 django-static-jquery3-6.3.7.1/django_static_jquery3.egg-info/dependency_links.txt
+-rw-r--r--   0 test       (501) staff       (20)        1 2024-05-12 13:00:08.000000 django-static-jquery3-6.3.7.1/django_static_jquery3.egg-info/not-zip-safe
+-rw-r--r--   0 test       (501) staff       (20)       22 2024-05-12 13:00:08.000000 django-static-jquery3-6.3.7.1/django_static_jquery3.egg-info/top_level.txt
+-rw-r--r--   0 test       (501) staff       (20)        0 2023-09-12 02:08:12.000000 django-static-jquery3-6.3.7.1/requirements.txt
+-rw-r--r--   0 test       (501) staff       (20)       38 2024-05-12 13:00:09.025570 django-static-jquery3-6.3.7.1/setup.cfg
+-rw-r--r--   0 test       (501) staff       (20)     1240 2024-05-12 12:59:30.000000 django-static-jquery3-6.3.7.1/setup.py
```

### Comparing `django-static-jquery3-5.3.7.1/LICENSE` & `django-static-jquery3-6.3.7.1/django_static_jquery3/static/jquery/licenses/jquery/LICENSE.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,20 @@
-MIT License
+Copyright OpenJS Foundation and other contributors, https://openjsf.org/
 
-Copyright (c) 2017 zencore.cn
+Permission is hereby granted, free of charge, to any person obtaining
+a copy of this software and associated documentation files (the
+"Software"), to deal in the Software without restriction, including
+without limitation the rights to use, copy, modify, merge, publish,
+distribute, sublicense, and/or sell copies of the Software, and to
+permit persons to whom the Software is furnished to do so, subject to
+the following conditions:
 
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
+The above copyright notice and this permission notice shall be
+included in all copies or substantial portions of the Software.
 
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
+EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
+MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
+NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE
+LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
+OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION
+WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `django-static-jquery3-5.3.7.1/PKG-INFO` & `django-static-jquery3-6.3.7.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: django-static-jquery3
-Version: 5.3.7.1
+Version: 6.3.7.1
 Summary: Django application contain jquery3 static files.
+Home-page: UNKNOWN
 Author: Chen JiaYong
-Author-email: chenjiayong@zencore.cn
 Maintainer: Chen JiaYong
-Maintainer-email: chenjiayong@zencore.cn
 License: MIT
 Keywords: django-static-jquery3,jquery,jquery plugins
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Description-Content-Type: text/markdown
@@ -42,69 +42,79 @@
 ```shell
 pip install django-static-jquery3
 ```
 
 ## Installed Plugins
 
 - jquery/plugins/jquery.cookie.js
+- jquery/plugins/jquery.parseQuery.js
 - jquery/plugins/jquery.utils.js
 - jquery/plugins/jquery.jstree/jstree.js
 
 ## Usage
 
-**pro/settings.py**
+*pro/settings.py*
 
 ```python
 INSTALLED_APPS = [
     ...
     "django_static_jquery3",
     ...
 ]
 ```
 
-**app/template/app/index.html**
+*app/template/app/index.html*
 
 ```html
 {% load static %}
 
 <script src="{% static "jquery/jquery.js" %}"></script>
 <script src="{% static "jquery/plugins/jquery.cookie.js" %}"></script>
+<script src="{% static "jquery/plugins/jquery.parseQuery.js" %}"></script>
+<script src="{% static "jquery/plugins/jquery.utils.js" %}"></script>
+<script src="{% static "jquery/plugins/jquery.cookie.js" %}"></script>
 ```
 
 ## About releases
 
 - The first number is our release number.
 - The other three numbers are the same with jquery's release version.
 
 ## Releases
 
-### v5.3.7.1 2023/09/12
+### v6.3.7.1
+
+- Add jquery.parseQuery plugin.
+
+### v5.3.7.1
 
 - Upgrade jquery to v3.7.1.
 
-### v5.1.0 2020/09/22
+### v5.1.0
 
 - Add jquery.jstree plugin.
 
-### v5.0.0 2020/09/01
+### v5.0.0
 
 - Rename jquery3 folder to jquery.
 - Mostly we use jquery plugins, for django ships with jquery already. 
 - We put many jquery plugins in this package, so that we will not use jquery's version from now on.
 - Remove django from requirements. We still keep django's file structure, but we will need anything about django.
 
-### v3.4.1.1 2020/04/23
+### v3.4.1.1
 
 - Add jquery plugin: jquery.cookie.
 - Fix document.
 
-### v3.4.1.0 2020/04/10
+### v3.4.1.0
 
 - Upgrade jquery to 3.4.1.
 
-### v3.3.1.1 2018/03/27
+### v3.3.1.1
 
 - Upgrade jquery to 3.3.1.
 
-## v3.2.1 2017/12/23
+## v3.2.1
 
 - First release with jquery 3.2.1.
+
+
```

#### html2text {}

```diff
@@ -1,38 +1,41 @@
-Metadata-Version: 2.1 Name: django-static-jquery3 Version: 5.3.7.1 Summary:
-Django application contain jquery3 static files. Author: Chen JiaYong Author-
-email: chenjiayong@zencore.cn Maintainer: Chen JiaYong Maintainer-email:
-chenjiayong@zencore.cn License: MIT Keywords: django-static-
-jquery3,jquery,jquery plugins Classifier: Development Status :: 5 - Production/
-Stable Classifier: Intended Audience :: Developers Classifier: Topic ::
-Software Development :: Libraries :: Python Modules Classifier: License :: OSI
-Approved :: MIT License Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only Description-Content-
-Type: text/markdown License-File: LICENSE # django-static-jquery3 Django
-application contains jquery and jquery-plugins' static files. - Mostly we use
-jquery plugins, for django ships with jquery already. - We put many jquery
-plugins in this package, so that we will not use jquery's version from now on.
-- Remove django from requirements.txt. We still keep django's file structure,
-but we will NOT need anything about django. ## jQuery License - All resource
-files of jquery are unzip from jquery-xxx.zip which download from https://
-github.com/jquery/jquery/ without any changes. - All resource files of jquery
-obey jQuery License, see details at https://github.com/jquery/jquery/blob/main/
-LICENSE.txt. - We don't guarantee the latest jQuery version. ## jQuery Plugins
-Licenses - Plugins may NOT a part of jquery. - Plugins obey their own licenses.
-## Install ```shell pip install django-static-jquery3 ``` ## Installed Plugins
-- jquery/plugins/jquery.cookie.js - jquery/plugins/jquery.utils.js - jquery/
-plugins/jquery.jstree/jstree.js ## Usage **pro/settings.py** ```python
-INSTALLED_APPS = [ ... "django_static_jquery3", ... ] ``` **app/template/app/
-index.html** ```html {% load static %}
+Metadata-Version: 2.1 Name: django-static-jquery3 Version: 6.3.7.1 Summary:
+Django application contain jquery3 static files. Home-page: UNKNOWN Author:
+Chen JiaYong Maintainer: Chen JiaYong License: MIT Keywords: django-static-
+jquery3,jquery,jquery plugins Platform: UNKNOWN Classifier: Development Status
+:: 5 - Production/Stable Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: License :: OSI Approved :: MIT License Classifier: Programming
+Language :: Python :: 3 Classifier: Programming Language :: Python :: 3 :: Only
+Description-Content-Type: text/markdown License-File: LICENSE # django-static-
+jquery3 Django application contains jquery and jquery-plugins' static files. -
+Mostly we use jquery plugins, for django ships with jquery already. - We put
+many jquery plugins in this package, so that we will not use jquery's version
+from now on. - Remove django from requirements.txt. We still keep django's file
+structure, but we will NOT need anything about django. ## jQuery License - All
+resource files of jquery are unzip from jquery-xxx.zip which download from
+https://github.com/jquery/jquery/ without any changes. - All resource files of
+jquery obey jQuery License, see details at https://github.com/jquery/jquery/
+blob/main/LICENSE.txt. - We don't guarantee the latest jQuery version. ##
+jQuery Plugins Licenses - Plugins may NOT a part of jquery. - Plugins obey
+their own licenses. ## Install ```shell pip install django-static-jquery3 ```
+## Installed Plugins - jquery/plugins/jquery.cookie.js - jquery/plugins/
+jquery.parseQuery.js - jquery/plugins/jquery.utils.js - jquery/plugins/
+jquery.jstree/jstree.js ## Usage *pro/settings.py* ```python INSTALLED_APPS =
+[ ... "django_static_jquery3", ... ] ``` *app/template/app/index.html* ```html
+{% load static %}
+}">
+}">
+}">
 }">
 }">
 ``` ## About releases - The first number is our release number. - The other
 three numbers are the same with jquery's release version. ## Releases ###
-v5.3.7.1 2023/09/12 - Upgrade jquery to v3.7.1. ### v5.1.0 2020/09/22 - Add
-jquery.jstree plugin. ### v5.0.0 2020/09/01 - Rename jquery3 folder to jquery.
-- Mostly we use jquery plugins, for django ships with jquery already. - We put
-many jquery plugins in this package, so that we will not use jquery's version
-from now on. - Remove django from requirements. We still keep django's file
-structure, but we will need anything about django. ### v3.4.1.1 2020/04/23 -
-Add jquery plugin: jquery.cookie. - Fix document. ### v3.4.1.0 2020/04/10 -
-Upgrade jquery to 3.4.1. ### v3.3.1.1 2018/03/27 - Upgrade jquery to 3.3.1. ##
-v3.2.1 2017/12/23 - First release with jquery 3.2.1.
+v6.3.7.1 - Add jquery.parseQuery plugin. ### v5.3.7.1 - Upgrade jquery to
+v3.7.1. ### v5.1.0 - Add jquery.jstree plugin. ### v5.0.0 - Rename jquery3
+folder to jquery. - Mostly we use jquery plugins, for django ships with jquery
+already. - We put many jquery plugins in this package, so that we will not use
+jquery's version from now on. - Remove django from requirements. We still keep
+django's file structure, but we will need anything about django. ### v3.4.1.1 -
+Add jquery plugin: jquery.cookie. - Fix document. ### v3.4.1.0 - Upgrade jquery
+to 3.4.1. ### v3.3.1.1 - Upgrade jquery to 3.3.1. ## v3.2.1 - First release
+with jquery 3.2.1.
```

### Comparing `django-static-jquery3-5.3.7.1/README.md` & `django-static-jquery3-6.3.7.1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -23,69 +23,77 @@
 ```shell
 pip install django-static-jquery3
 ```
 
 ## Installed Plugins
 
 - jquery/plugins/jquery.cookie.js
+- jquery/plugins/jquery.parseQuery.js
 - jquery/plugins/jquery.utils.js
 - jquery/plugins/jquery.jstree/jstree.js
 
 ## Usage
 
-**pro/settings.py**
+*pro/settings.py*
 
 ```python
 INSTALLED_APPS = [
     ...
     "django_static_jquery3",
     ...
 ]
 ```
 
-**app/template/app/index.html**
+*app/template/app/index.html*
 
 ```html
 {% load static %}
 
 <script src="{% static "jquery/jquery.js" %}"></script>
 <script src="{% static "jquery/plugins/jquery.cookie.js" %}"></script>
+<script src="{% static "jquery/plugins/jquery.parseQuery.js" %}"></script>
+<script src="{% static "jquery/plugins/jquery.utils.js" %}"></script>
+<script src="{% static "jquery/plugins/jquery.cookie.js" %}"></script>
 ```
 
 ## About releases
 
 - The first number is our release number.
 - The other three numbers are the same with jquery's release version.
 
 ## Releases
 
-### v5.3.7.1 2023/09/12
+### v6.3.7.1
+
+- Add jquery.parseQuery plugin.
+
+### v5.3.7.1
 
 - Upgrade jquery to v3.7.1.
 
-### v5.1.0 2020/09/22
+### v5.1.0
 
 - Add jquery.jstree plugin.
 
-### v5.0.0 2020/09/01
+### v5.0.0
 
 - Rename jquery3 folder to jquery.
 - Mostly we use jquery plugins, for django ships with jquery already. 
 - We put many jquery plugins in this package, so that we will not use jquery's version from now on.
 - Remove django from requirements. We still keep django's file structure, but we will need anything about django.
 
-### v3.4.1.1 2020/04/23
+### v3.4.1.1
 
 - Add jquery plugin: jquery.cookie.
 - Fix document.
 
-### v3.4.1.0 2020/04/10
+### v3.4.1.0
 
 - Upgrade jquery to 3.4.1.
 
-### v3.3.1.1 2018/03/27
+### v3.3.1.1
 
 - Upgrade jquery to 3.3.1.
 
-## v3.2.1 2017/12/23
+## v3.2.1
 
 - First release with jquery 3.2.1.
```

#### html2text {}

```diff
@@ -6,24 +6,27 @@
 jQuery License - All resource files of jquery are unzip from jquery-xxx.zip
 which download from https://github.com/jquery/jquery/ without any changes. -
 All resource files of jquery obey jQuery License, see details at https://
 github.com/jquery/jquery/blob/main/LICENSE.txt. - We don't guarantee the latest
 jQuery version. ## jQuery Plugins Licenses - Plugins may NOT a part of jquery.
 - Plugins obey their own licenses. ## Install ```shell pip install django-
 static-jquery3 ``` ## Installed Plugins - jquery/plugins/jquery.cookie.js -
-jquery/plugins/jquery.utils.js - jquery/plugins/jquery.jstree/jstree.js ##
-Usage **pro/settings.py** ```python INSTALLED_APPS = [ ...
-"django_static_jquery3", ... ] ``` **app/template/app/index.html** ```html {%
-load static %}
+jquery/plugins/jquery.parseQuery.js - jquery/plugins/jquery.utils.js - jquery/
+plugins/jquery.jstree/jstree.js ## Usage *pro/settings.py* ```python
+INSTALLED_APPS = [ ... "django_static_jquery3", ... ] ``` *app/template/app/
+index.html* ```html {% load static %}
+}">
+}">
+}">
 }">
 }">
 ``` ## About releases - The first number is our release number. - The other
 three numbers are the same with jquery's release version. ## Releases ###
-v5.3.7.1 2023/09/12 - Upgrade jquery to v3.7.1. ### v5.1.0 2020/09/22 - Add
-jquery.jstree plugin. ### v5.0.0 2020/09/01 - Rename jquery3 folder to jquery.
-- Mostly we use jquery plugins, for django ships with jquery already. - We put
-many jquery plugins in this package, so that we will not use jquery's version
-from now on. - Remove django from requirements. We still keep django's file
-structure, but we will need anything about django. ### v3.4.1.1 2020/04/23 -
-Add jquery plugin: jquery.cookie. - Fix document. ### v3.4.1.0 2020/04/10 -
-Upgrade jquery to 3.4.1. ### v3.3.1.1 2018/03/27 - Upgrade jquery to 3.3.1. ##
-v3.2.1 2017/12/23 - First release with jquery 3.2.1.
+v6.3.7.1 - Add jquery.parseQuery plugin. ### v5.3.7.1 - Upgrade jquery to
+v3.7.1. ### v5.1.0 - Add jquery.jstree plugin. ### v5.0.0 - Rename jquery3
+folder to jquery. - Mostly we use jquery plugins, for django ships with jquery
+already. - We put many jquery plugins in this package, so that we will not use
+jquery's version from now on. - Remove django from requirements. We still keep
+django's file structure, but we will need anything about django. ### v3.4.1.1 -
+Add jquery plugin: jquery.cookie. - Fix document. ### v3.4.1.0 - Upgrade jquery
+to 3.4.1. ### v3.3.1.1 - Upgrade jquery to 3.3.1. ## v3.2.1 - First release
+with jquery 3.2.1.
```

### Comparing `django-static-jquery3-5.3.7.1/django_static_jquery3/.DS_Store` & `django-static-jquery3-6.3.7.1/django_static_jquery3/static/jquery/plugins/.DS_Store`

 * *Files 26% similar despite different names*

```diff
@@ -1,57 +1,57 @@
 00000000: 0000 0001 4275 6431 0000 1000 0000 0800  ....Bud1........
-00000010: 0000 1000 0000 0108 0000 0000 0000 0000  ................
+00000010: 0000 1000 0000 0209 0000 0000 0000 0000  ................
 00000020: 0000 0000 0000 0000 0000 0000 0000 0800  ................
 00000030: 0000 0800 0000 0000 0000 0000 0000 0000  ................
 00000040: 0000 0000 0000 0002 0000 0000 0000 0002  ................
-00000050: 0000 0001 0000 1000 0069 0063 6277 7370  .........i.cbwsp
-00000060: 626c 6f62 0000 0000 0000 0000 0000 0000  blob............
+00000050: 0000 0001 0000 1000 0072 0079 002e 006a  .........r.y...j
+00000060: 0073 0074 0000 0000 0000 0000 0000 0000  .s.t............
 00000070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000090: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000100: 0000 0000 0000 0000 0000 0002 0000 0006  ................
-00000110: 0073 0074 0061 0074 0069 0063 6277 7370  .s.t.a.t.i.cbwsp
-00000120: 626c 6f62 0000 00b8 6270 6c69 7374 3030  blob....bplist00
-00000130: d601 0203 0405 0607 0807 080b 085d 5368  .............]Sh
-00000140: 6f77 5374 6174 7573 4261 725b 5368 6f77  owStatusBar[Show
-00000150: 546f 6f6c 6261 725b 5368 6f77 5461 6256  Toolbar[ShowTabV
-00000160: 6965 775f 1014 436f 6e74 6169 6e65 7253  iew_..ContainerS
-00000170: 686f 7753 6964 6562 6172 5c57 696e 646f  howSidebar\Windo
-00000180: 7742 6f75 6e64 735b 5368 6f77 5369 6465  wBounds[ShowSide
-00000190: 6261 7208 0908 095f 1018 7b7b 3437 2c20  bar...._..{{47, 
-000001a0: 3137 357d 2c20 7b31 3035 362c 2036 3536  175}, {1056, 656
-000001b0: 7d7d 0908 1523 2f3b 525f 6b6c 6d6e 6f8a  }}...#/;R_klmno.
-000001c0: 0000 0000 0000 0101 0000 0000 0000 000d  ................
-000001d0: 0000 0000 0000 0000 0000 0000 0000 008b  ................
-000001e0: 0000 0006 0073 0074 0061 0074 0069 0063  .....s.t.a.t.i.c
-000001f0: 7653 726e 6c6f 6e67 0000 0001 0000 0000  vSrnlong........
-00000200: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000210: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000220: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000230: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000240: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000250: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000260: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000270: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000280: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000290: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000002a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000002b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000002c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000002d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000002e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000002f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000300: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000310: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000100: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000110: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000120: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000130: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000140: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000150: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000160: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000170: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000180: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000190: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000001a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000001b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000001c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000001d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000001e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000001f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000200: 0000 0000 0000 0000 0000 0002 0000 000d  ................
+00000210: 006a 0071 0075 0065 0072 0079 002e 006a  .j.q.u.e.r.y...j
+00000220: 0073 0074 0072 0065 0065 6277 7370 626c  .s.t.r.e.ebwspbl
+00000230: 6f62 0000 00b9 6270 6c69 7374 3030 d601  ob....bplist00..
+00000240: 0203 0405 0607 0807 080b 085d 5368 6f77  ...........]Show
+00000250: 5374 6174 7573 4261 725b 5368 6f77 546f  StatusBar[ShowTo
+00000260: 6f6c 6261 725b 5368 6f77 5461 6256 6965  olbar[ShowTabVie
+00000270: 775f 1014 436f 6e74 6169 6e65 7253 686f  w_..ContainerSho
+00000280: 7753 6964 6562 6172 5c57 696e 646f 7742  wSidebar\WindowB
+00000290: 6f75 6e64 735b 5368 6f77 5369 6465 6261  ounds[ShowSideba
+000002a0: 7208 0908 095f 1019 7b7b 3637 352c 202d  r...._..{{675, -
+000002b0: 3338 7d2c 207b 3131 3536 2c20 3733 377d  38}, {1156, 737}
+000002c0: 7d09 0815 232f 3b52 5f6b 6c6d 6e6f 8b00  }...#/;R_klmno..
+000002d0: 0000 0000 0001 0100 0000 0000 0000 0d00  ................
+000002e0: 0000 0000 0000 0000 0000 0000 0000 8c00  ................
+000002f0: 0000 0d00 6a00 7100 7500 6500 7200 7900  ....j.q.u.e.r.y.
+00000300: 2e00 6a00 7300 7400 7200 6500 6576 5372  ..j.s.t.r.e.evSr
+00000310: 6e6c 6f6e 6700 0000 0100 0000 0000 0000  nlong...........
 00000320: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000330: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000340: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000350: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000360: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000370: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000380: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -251,15 +251,15 @@
 00000fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001000: 0000 0000 0000 0003 0000 0000 0000 100b  ................
-00001010: 0000 0045 0000 0108 0000 0000 0000 0000  ...E............
+00001010: 0000 0045 0000 0209 0000 0000 0000 0000  ...E............
 00001020: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001030: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001040: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001050: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001060: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -318,15 +318,15 @@
 000013d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000013e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000013f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001400: 0000 0000 0000 0000 0000 0000 0000 0001  ................
 00001410: 0444 5344 4200 0000 0100 0000 0000 0000  .DSDB...........
 00001420: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001430: 0200 0000 2000 0000 6000 0000 0000 0000  .... ...`.......
-00001440: 0100 0000 8000 0000 0000 0000 0100 0002  ................
+00001440: 0100 0000 8000 0000 0100 0001 0000 0000  ................
 00001450: 0000 0000 0100 0004 0000 0000 0200 0008  ................
 00001460: 0000 0018 0000 0000 0000 0000 0100 0020  ............... 
 00001470: 0000 0000 0100 0040 0000 0000 0100 0080  .......@........
 00001480: 0000 0000 0100 0100 0000 0000 0100 0200  ................
 00001490: 0000 0000 0100 0400 0000 0000 0100 0800  ................
 000014a0: 0000 0000 0100 1000 0000 0000 0100 2000  .............. .
 000014b0: 0000 0000 0100 4000 0000 0000 0100 8000  ......@.........
```

### Comparing `django-static-jquery3-5.3.7.1/django_static_jquery3/static/.DS_Store` & `django-static-jquery3-6.3.7.1/django_static_jquery3/static/.DS_Store`

 * *Files 5% similar despite different names*

```diff
@@ -19,17 +19,17 @@
 00000120: 626c 6f62 0000 00b9 6270 6c69 7374 3030  blob....bplist00
 00000130: d601 0203 0405 0607 0807 080b 085d 5368  .............]Sh
 00000140: 6f77 5374 6174 7573 4261 725b 5368 6f77  owStatusBar[Show
 00000150: 546f 6f6c 6261 725b 5368 6f77 5461 6256  Toolbar[ShowTabV
 00000160: 6965 775f 1014 436f 6e74 6169 6e65 7253  iew_..ContainerS
 00000170: 686f 7753 6964 6562 6172 5c57 696e 646f  howSidebar\Windo
 00000180: 7742 6f75 6e64 735b 5368 6f77 5369 6465  wBounds[ShowSide
-00000190: 6261 7208 0908 095f 1019 7b7b 3439 392c  bar...._..{{499,
-000001a0: 2031 3539 7d2c 207b 3130 3536 2c20 3635   159}, {1056, 65
-000001b0: 367d 7d09 0815 232f 3b52 5f6b 6c6d 6e6f  6}}...#/;R_klmno
+00000190: 6261 7208 0908 095f 1019 7b7b 3733 332c  bar...._..{{733,
+000001a0: 2031 3737 7d2c 207b 3131 3035 2c20 3637   177}, {1105, 67
+000001b0: 337d 7d09 0815 232f 3b52 5f6b 6c6d 6e6f  3}}...#/;R_klmno
 000001c0: 8b00 0000 0000 0001 0100 0000 0000 0000  ................
 000001d0: 0d00 0000 0000 0000 0000 0000 0000 0000  ................
 000001e0: 8c00 0000 0600 6a00 7100 7500 6500 7200  ......j.q.u.e.r.
 000001f0: 7976 5372 6e6c 6f6e 6700 0000 0100 0000  yvSrnlong.......
 00000200: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000210: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000220: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `django-static-jquery3-5.3.7.1/django_static_jquery3/static/jquery/.DS_Store` & `django-static-jquery3-6.3.7.1/django_static_jquery3/static/jquery/.DS_Store`

 * *Files identical despite different names*

### Comparing `django-static-jquery3-5.3.7.1/django_static_jquery3/static/jquery/jquery.js` & `django-static-jquery3-6.3.7.1/django_static_jquery3/static/jquery/jquery.js`

 * *Files identical despite different names*

### Comparing `django-static-jquery3-5.3.7.1/django_static_jquery3/static/jquery/jquery.min.js` & `django-static-jquery3-6.3.7.1/django_static_jquery3/static/jquery/jquery.min.js`

 * *Files identical despite different names*

### Comparing `django-static-jquery3-5.3.7.1/django_static_jquery3/static/jquery/jquery.min.map` & `django-static-jquery3-6.3.7.1/django_static_jquery3/static/jquery/jquery.min.map`

 * *Files identical despite different names*

### Comparing `django-static-jquery3-5.3.7.1/django_static_jquery3/static/jquery/jquery.slim.js` & `django-static-jquery3-6.3.7.1/django_static_jquery3/static/jquery/jquery.slim.js`

 * *Files identical despite different names*

### Comparing `django-static-jquery3-5.3.7.1/django_static_jquery3/static/jquery/jquery.slim.min.js` & `django-static-jquery3-6.3.7.1/django_static_jquery3/static/jquery/jquery.slim.min.js`

 * *Files identical despite different names*

### Comparing `django-static-jquery3-5.3.7.1/django_static_jquery3/static/jquery/jquery.slim.min.map` & `django-static-jquery3-6.3.7.1/django_static_jquery3/static/jquery/jquery.slim.min.map`

 * *Files identical despite different names*

### Comparing `django-static-jquery3-5.3.7.1/django_static_jquery3/static/jquery/licenses/.DS_Store` & `django-static-jquery3-6.3.7.1/django_static_jquery3/static/jquery/licenses/.DS_Store`

 * *Files identical despite different names*

### Comparing `django-static-jquery3-5.3.7.1/django_static_jquery3/static/jquery/licenses/jquery/LICENSE.txt` & `django-static-jquery3-6.3.7.1/django_static_jquery3/static/jquery/licenses/jquery.cookie/MIT-LICENSE.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright OpenJS Foundation and other contributors, https://openjsf.org/
+Copyright 2014 Klaus Hartl
 
 Permission is hereby granted, free of charge, to any person obtaining
 a copy of this software and associated documentation files (the
 "Software"), to deal in the Software without restriction, including
 without limitation the rights to use, copy, modify, merge, publish,
 distribute, sublicense, and/or sell copies of the Software, and to
 permit persons to whom the Software is furnished to do so, subject to
```

### Comparing `django-static-jquery3-5.3.7.1/django_static_jquery3/static/jquery/licenses/jquery.cookie/MIT-LICENSE.txt` & `django-static-jquery3-6.3.7.1/django_static_jquery3/static/jquery/licenses/jquery.jstree/LICENSE-MIT`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,22 @@
-Copyright 2014 Klaus Hartl
-
-Permission is hereby granted, free of charge, to any person obtaining
-a copy of this software and associated documentation files (the
-"Software"), to deal in the Software without restriction, including
-without limitation the rights to use, copy, modify, merge, publish,
-distribute, sublicense, and/or sell copies of the Software, and to
-permit persons to whom the Software is furnished to do so, subject to
-the following conditions:
-
-The above copyright notice and this permission notice shall be
-included in all copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
-EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
-MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
-NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE
-LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
-OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION
-WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+Copyright (c) 2014 Ivan Bozhanov
+
+Permission is hereby granted, free of charge, to any person
+obtaining a copy of this software and associated documentation
+files (the "Software"), to deal in the Software without
+restriction, including without limitation the rights to use,
+copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the
+Software is furnished to do so, subject to the following
+conditions:
+
+The above copyright notice and this permission notice shall be
+included in all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
+EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES
+OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
+NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT
+HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY,
+WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
+FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
+OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `django-static-jquery3-5.3.7.1/django_static_jquery3/static/jquery/licenses/jquery.jstree/.DS_Store` & `django-static-jquery3-6.3.7.1/django_static_jquery3/static/jquery/licenses/jquery.jstree/.DS_Store`

 * *Files identical despite different names*

### Comparing `django-static-jquery3-5.3.7.1/django_static_jquery3/static/jquery/licenses/jquery.jstree/LICENSE-MIT` & `django-static-jquery3-6.3.7.1/LICENSE`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,19 @@
-Copyright (c) 2014 Ivan Bozhanov
-
-Permission is hereby granted, free of charge, to any person
-obtaining a copy of this software and associated documentation
-files (the "Software"), to deal in the Software without
-restriction, including without limitation the rights to use,
-copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the
-Software is furnished to do so, subject to the following
-conditions:
-
-The above copyright notice and this permission notice shall be
-included in all copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
-EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES
-OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
-NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT
-HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY,
-WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
-FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
-OTHER DEALINGS IN THE SOFTWARE.
+MIT License
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `django-static-jquery3-5.3.7.1/django_static_jquery3/static/jquery/plugins/.DS_Store` & `django-static-jquery3-6.3.7.1/django_static_jquery3/static/jquery/plugins/jquery.jstree/.DS_Store`

 * *Files 24% similar despite different names*

```diff
@@ -1,57 +1,57 @@
 00000000: 0000 0001 4275 6431 0000 1000 0000 0800  ....Bud1........
-00000010: 0000 1000 0000 0209 0000 0000 0000 0000  ................
+00000010: 0000 1000 0000 0108 0000 0000 0000 0000  ................
 00000020: 0000 0000 0000 0000 0000 0000 0000 0800  ................
 00000030: 0000 0800 0000 0000 0000 0000 0000 0000  ................
 00000040: 0000 0000 0000 0002 0000 0000 0000 0002  ................
-00000050: 0000 0001 0000 1000 0072 0079 002e 006a  .........r.y...j
-00000060: 0073 0074 0000 0000 0000 0000 0000 0000  .s.t............
+00000050: 0000 0001 0000 1000 0065 0073 6277 7370  .........e.sbwsp
+00000060: 626c 6f62 0000 0000 0000 0000 0000 0000  blob............
 00000070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000090: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000100: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000110: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000120: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000130: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000140: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000150: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000160: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000170: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000180: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000190: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000001a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000001b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000001c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000001d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000001e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000001f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000200: 0000 0000 0000 0000 0000 0002 0000 000d  ................
-00000210: 006a 0071 0075 0065 0072 0079 002e 006a  .j.q.u.e.r.y...j
-00000220: 0073 0074 0072 0065 0065 6277 7370 626c  .s.t.r.e.ebwspbl
-00000230: 6f62 0000 00b9 6270 6c69 7374 3030 d601  ob....bplist00..
-00000240: 0203 0405 0607 0807 080b 085d 5368 6f77  ...........]Show
-00000250: 5374 6174 7573 4261 725b 5368 6f77 546f  StatusBar[ShowTo
-00000260: 6f6c 6261 725b 5368 6f77 5461 6256 6965  olbar[ShowTabVie
-00000270: 775f 1014 436f 6e74 6169 6e65 7253 686f  w_..ContainerSho
-00000280: 7753 6964 6562 6172 5c57 696e 646f 7742  wSidebar\WindowB
-00000290: 6f75 6e64 735b 5368 6f77 5369 6465 6261  ounds[ShowSideba
-000002a0: 7208 0908 095f 1019 7b7b 3637 352c 202d  r...._..{{675, -
-000002b0: 3338 7d2c 207b 3131 3536 2c20 3733 377d  38}, {1156, 737}
-000002c0: 7d09 0815 232f 3b52 5f6b 6c6d 6e6f 8b00  }...#/;R_klmno..
-000002d0: 0000 0000 0001 0100 0000 0000 0000 0d00  ................
-000002e0: 0000 0000 0000 0000 0000 0000 0000 8c00  ................
-000002f0: 0000 0d00 6a00 7100 7500 6500 7200 7900  ....j.q.u.e.r.y.
-00000300: 2e00 6a00 7300 7400 7200 6500 6576 5372  ..j.s.t.r.e.evSr
-00000310: 6e6c 6f6e 6700 0000 0100 0000 0000 0000  nlong...........
+00000100: 0000 0000 0000 0000 0000 0002 0000 0006  ................
+00000110: 0074 0068 0065 006d 0065 0073 6277 7370  .t.h.e.m.e.sbwsp
+00000120: 626c 6f62 0000 00b8 6270 6c69 7374 3030  blob....bplist00
+00000130: d601 0203 0405 0607 0807 080b 085d 5368  .............]Sh
+00000140: 6f77 5374 6174 7573 4261 725b 5368 6f77  owStatusBar[Show
+00000150: 546f 6f6c 6261 725b 5368 6f77 5461 6256  Toolbar[ShowTabV
+00000160: 6965 775f 1014 436f 6e74 6169 6e65 7253  iew_..ContainerS
+00000170: 686f 7753 6964 6562 6172 5c57 696e 646f  howSidebar\Windo
+00000180: 7742 6f75 6e64 735b 5368 6f77 5369 6465  wBounds[ShowSide
+00000190: 6261 7208 0908 095f 1018 7b7b 3132 382c  bar...._..{{128,
+000001a0: 2034 317d 2c20 7b31 3135 362c 2037 3337   41}, {1156, 737
+000001b0: 7d7d 0908 1523 2f3b 525f 6b6c 6d6e 6f8a  }}...#/;R_klmno.
+000001c0: 0000 0000 0000 0101 0000 0000 0000 000d  ................
+000001d0: 0000 0000 0000 0000 0000 0000 0000 008b  ................
+000001e0: 0000 0006 0074 0068 0065 006d 0065 0073  .....t.h.e.m.e.s
+000001f0: 7653 726e 6c6f 6e67 0000 0001 0000 0000  vSrnlong........
+00000200: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000210: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000220: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000230: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000240: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000250: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000260: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000270: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000280: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000290: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000002a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000002b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000002c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000002d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000002e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000002f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000300: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000310: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000320: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000330: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000340: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000350: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000360: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000370: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000380: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -251,15 +251,15 @@
 00000fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001000: 0000 0000 0000 0003 0000 0000 0000 100b  ................
-00001010: 0000 0045 0000 0209 0000 0000 0000 0000  ...E............
+00001010: 0000 0045 0000 0108 0000 0000 0000 0000  ...E............
 00001020: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001030: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001040: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001050: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001060: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -318,15 +318,15 @@
 000013d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000013e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000013f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001400: 0000 0000 0000 0000 0000 0000 0000 0001  ................
 00001410: 0444 5344 4200 0000 0100 0000 0000 0000  .DSDB...........
 00001420: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001430: 0200 0000 2000 0000 6000 0000 0000 0000  .... ...`.......
-00001440: 0100 0000 8000 0000 0100 0001 0000 0000  ................
+00001440: 0100 0000 8000 0000 0000 0000 0100 0002  ................
 00001450: 0000 0000 0100 0004 0000 0000 0200 0008  ................
 00001460: 0000 0018 0000 0000 0000 0000 0100 0020  ............... 
 00001470: 0000 0000 0100 0040 0000 0000 0100 0080  .......@........
 00001480: 0000 0000 0100 0100 0000 0000 0100 0200  ................
 00001490: 0000 0000 0100 0400 0000 0000 0100 0800  ................
 000014a0: 0000 0000 0100 1000 0000 0000 0100 2000  .............. .
 000014b0: 0000 0000 0100 4000 0000 0000 0100 8000  ......@.........
```

### Comparing `django-static-jquery3-5.3.7.1/django_static_jquery3/static/jquery/plugins/jquery.cookie.js` & `django-static-jquery3-6.3.7.1/django_static_jquery3/static/jquery/plugins/jquery.cookie.js`

 * *Files identical despite different names*

### Comparing `django-static-jquery3-5.3.7.1/django_static_jquery3/static/jquery/plugins/jquery.jstree/jstree.js` & `django-static-jquery3-6.3.7.1/django_static_jquery3/static/jquery/plugins/jquery.jstree/jstree.js`

 * *Files identical despite different names*

### Comparing `django-static-jquery3-5.3.7.1/django_static_jquery3/static/jquery/plugins/jquery.jstree/jstree.min.js` & `django-static-jquery3-6.3.7.1/django_static_jquery3/static/jquery/plugins/jquery.jstree/jstree.min.js`

 * *Files identical despite different names*

### Comparing `django-static-jquery3-5.3.7.1/django_static_jquery3/static/jquery/plugins/jquery.jstree/themes/default/32px.png` & `django-static-jquery3-6.3.7.1/django_static_jquery3/static/jquery/plugins/jquery.jstree/themes/default/32px.png`

 * *Files identical despite different names*

### Comparing `django-static-jquery3-5.3.7.1/django_static_jquery3/static/jquery/plugins/jquery.jstree/themes/default/40px.png` & `django-static-jquery3-6.3.7.1/django_static_jquery3/static/jquery/plugins/jquery.jstree/themes/default/40px.png`

 * *Files identical despite different names*

### Comparing `django-static-jquery3-5.3.7.1/django_static_jquery3/static/jquery/plugins/jquery.jstree/themes/default/style.css` & `django-static-jquery3-6.3.7.1/django_static_jquery3/static/jquery/plugins/jquery.jstree/themes/default/style.css`

 * *Files identical despite different names*

### Comparing `django-static-jquery3-5.3.7.1/django_static_jquery3/static/jquery/plugins/jquery.jstree/themes/default/style.min.css` & `django-static-jquery3-6.3.7.1/django_static_jquery3/static/jquery/plugins/jquery.jstree/themes/default/style.min.css`

 * *Files identical despite different names*

### Comparing `django-static-jquery3-5.3.7.1/django_static_jquery3/static/jquery/plugins/jquery.jstree/themes/default/throbber.gif` & `django-static-jquery3-6.3.7.1/django_static_jquery3/static/jquery/plugins/jquery.jstree/themes/default/throbber.gif`

 * *Files identical despite different names*

### Comparing `django-static-jquery3-5.3.7.1/django_static_jquery3/static/jquery/plugins/jquery.jstree/themes/default-dark/32px.png` & `django-static-jquery3-6.3.7.1/django_static_jquery3/static/jquery/plugins/jquery.jstree/themes/default-dark/32px.png`

 * *Files identical despite different names*

### Comparing `django-static-jquery3-5.3.7.1/django_static_jquery3/static/jquery/plugins/jquery.jstree/themes/default-dark/40px.png` & `django-static-jquery3-6.3.7.1/django_static_jquery3/static/jquery/plugins/jquery.jstree/themes/default-dark/40px.png`

 * *Files identical despite different names*

### Comparing `django-static-jquery3-5.3.7.1/django_static_jquery3/static/jquery/plugins/jquery.jstree/themes/default-dark/style.css` & `django-static-jquery3-6.3.7.1/django_static_jquery3/static/jquery/plugins/jquery.jstree/themes/default-dark/style.css`

 * *Files identical despite different names*

### Comparing `django-static-jquery3-5.3.7.1/django_static_jquery3/static/jquery/plugins/jquery.jstree/themes/default-dark/style.min.css` & `django-static-jquery3-6.3.7.1/django_static_jquery3/static/jquery/plugins/jquery.jstree/themes/default-dark/style.min.css`

 * *Files identical despite different names*

### Comparing `django-static-jquery3-5.3.7.1/django_static_jquery3/static/jquery/plugins/jquery.jstree/themes/default-dark/throbber.gif` & `django-static-jquery3-6.3.7.1/django_static_jquery3/static/jquery/plugins/jquery.jstree/themes/default-dark/throbber.gif`

 * *Files identical despite different names*

### Comparing `django-static-jquery3-5.3.7.1/django_static_jquery3/static/jquery/plugins/jquery.utils.js` & `django-static-jquery3-6.3.7.1/django_static_jquery3/static/jquery/plugins/jquery.utils.js`

 * *Files identical despite different names*

### Comparing `django-static-jquery3-5.3.7.1/django_static_jquery3.egg-info/PKG-INFO` & `django-static-jquery3-6.3.7.1/django_static_jquery3.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: django-static-jquery3
-Version: 5.3.7.1
+Version: 6.3.7.1
 Summary: Django application contain jquery3 static files.
+Home-page: UNKNOWN
 Author: Chen JiaYong
-Author-email: chenjiayong@zencore.cn
 Maintainer: Chen JiaYong
-Maintainer-email: chenjiayong@zencore.cn
 License: MIT
 Keywords: django-static-jquery3,jquery,jquery plugins
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Description-Content-Type: text/markdown
@@ -42,69 +42,79 @@
 ```shell
 pip install django-static-jquery3
 ```
 
 ## Installed Plugins
 
 - jquery/plugins/jquery.cookie.js
+- jquery/plugins/jquery.parseQuery.js
 - jquery/plugins/jquery.utils.js
 - jquery/plugins/jquery.jstree/jstree.js
 
 ## Usage
 
-**pro/settings.py**
+*pro/settings.py*
 
 ```python
 INSTALLED_APPS = [
     ...
     "django_static_jquery3",
     ...
 ]
 ```
 
-**app/template/app/index.html**
+*app/template/app/index.html*
 
 ```html
 {% load static %}
 
 <script src="{% static "jquery/jquery.js" %}"></script>
 <script src="{% static "jquery/plugins/jquery.cookie.js" %}"></script>
+<script src="{% static "jquery/plugins/jquery.parseQuery.js" %}"></script>
+<script src="{% static "jquery/plugins/jquery.utils.js" %}"></script>
+<script src="{% static "jquery/plugins/jquery.cookie.js" %}"></script>
 ```
 
 ## About releases
 
 - The first number is our release number.
 - The other three numbers are the same with jquery's release version.
 
 ## Releases
 
-### v5.3.7.1 2023/09/12
+### v6.3.7.1
+
+- Add jquery.parseQuery plugin.
+
+### v5.3.7.1
 
 - Upgrade jquery to v3.7.1.
 
-### v5.1.0 2020/09/22
+### v5.1.0
 
 - Add jquery.jstree plugin.
 
-### v5.0.0 2020/09/01
+### v5.0.0
 
 - Rename jquery3 folder to jquery.
 - Mostly we use jquery plugins, for django ships with jquery already. 
 - We put many jquery plugins in this package, so that we will not use jquery's version from now on.
 - Remove django from requirements. We still keep django's file structure, but we will need anything about django.
 
-### v3.4.1.1 2020/04/23
+### v3.4.1.1
 
 - Add jquery plugin: jquery.cookie.
 - Fix document.
 
-### v3.4.1.0 2020/04/10
+### v3.4.1.0
 
 - Upgrade jquery to 3.4.1.
 
-### v3.3.1.1 2018/03/27
+### v3.3.1.1
 
 - Upgrade jquery to 3.3.1.
 
-## v3.2.1 2017/12/23
+## v3.2.1
 
 - First release with jquery 3.2.1.
+
+
```

#### html2text {}

```diff
@@ -1,38 +1,41 @@
-Metadata-Version: 2.1 Name: django-static-jquery3 Version: 5.3.7.1 Summary:
-Django application contain jquery3 static files. Author: Chen JiaYong Author-
-email: chenjiayong@zencore.cn Maintainer: Chen JiaYong Maintainer-email:
-chenjiayong@zencore.cn License: MIT Keywords: django-static-
-jquery3,jquery,jquery plugins Classifier: Development Status :: 5 - Production/
-Stable Classifier: Intended Audience :: Developers Classifier: Topic ::
-Software Development :: Libraries :: Python Modules Classifier: License :: OSI
-Approved :: MIT License Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only Description-Content-
-Type: text/markdown License-File: LICENSE # django-static-jquery3 Django
-application contains jquery and jquery-plugins' static files. - Mostly we use
-jquery plugins, for django ships with jquery already. - We put many jquery
-plugins in this package, so that we will not use jquery's version from now on.
-- Remove django from requirements.txt. We still keep django's file structure,
-but we will NOT need anything about django. ## jQuery License - All resource
-files of jquery are unzip from jquery-xxx.zip which download from https://
-github.com/jquery/jquery/ without any changes. - All resource files of jquery
-obey jQuery License, see details at https://github.com/jquery/jquery/blob/main/
-LICENSE.txt. - We don't guarantee the latest jQuery version. ## jQuery Plugins
-Licenses - Plugins may NOT a part of jquery. - Plugins obey their own licenses.
-## Install ```shell pip install django-static-jquery3 ``` ## Installed Plugins
-- jquery/plugins/jquery.cookie.js - jquery/plugins/jquery.utils.js - jquery/
-plugins/jquery.jstree/jstree.js ## Usage **pro/settings.py** ```python
-INSTALLED_APPS = [ ... "django_static_jquery3", ... ] ``` **app/template/app/
-index.html** ```html {% load static %}
+Metadata-Version: 2.1 Name: django-static-jquery3 Version: 6.3.7.1 Summary:
+Django application contain jquery3 static files. Home-page: UNKNOWN Author:
+Chen JiaYong Maintainer: Chen JiaYong License: MIT Keywords: django-static-
+jquery3,jquery,jquery plugins Platform: UNKNOWN Classifier: Development Status
+:: 5 - Production/Stable Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: License :: OSI Approved :: MIT License Classifier: Programming
+Language :: Python :: 3 Classifier: Programming Language :: Python :: 3 :: Only
+Description-Content-Type: text/markdown License-File: LICENSE # django-static-
+jquery3 Django application contains jquery and jquery-plugins' static files. -
+Mostly we use jquery plugins, for django ships with jquery already. - We put
+many jquery plugins in this package, so that we will not use jquery's version
+from now on. - Remove django from requirements.txt. We still keep django's file
+structure, but we will NOT need anything about django. ## jQuery License - All
+resource files of jquery are unzip from jquery-xxx.zip which download from
+https://github.com/jquery/jquery/ without any changes. - All resource files of
+jquery obey jQuery License, see details at https://github.com/jquery/jquery/
+blob/main/LICENSE.txt. - We don't guarantee the latest jQuery version. ##
+jQuery Plugins Licenses - Plugins may NOT a part of jquery. - Plugins obey
+their own licenses. ## Install ```shell pip install django-static-jquery3 ```
+## Installed Plugins - jquery/plugins/jquery.cookie.js - jquery/plugins/
+jquery.parseQuery.js - jquery/plugins/jquery.utils.js - jquery/plugins/
+jquery.jstree/jstree.js ## Usage *pro/settings.py* ```python INSTALLED_APPS =
+[ ... "django_static_jquery3", ... ] ``` *app/template/app/index.html* ```html
+{% load static %}
+}">
+}">
+}">
 }">
 }">
 ``` ## About releases - The first number is our release number. - The other
 three numbers are the same with jquery's release version. ## Releases ###
-v5.3.7.1 2023/09/12 - Upgrade jquery to v3.7.1. ### v5.1.0 2020/09/22 - Add
-jquery.jstree plugin. ### v5.0.0 2020/09/01 - Rename jquery3 folder to jquery.
-- Mostly we use jquery plugins, for django ships with jquery already. - We put
-many jquery plugins in this package, so that we will not use jquery's version
-from now on. - Remove django from requirements. We still keep django's file
-structure, but we will need anything about django. ### v3.4.1.1 2020/04/23 -
-Add jquery plugin: jquery.cookie. - Fix document. ### v3.4.1.0 2020/04/10 -
-Upgrade jquery to 3.4.1. ### v3.3.1.1 2018/03/27 - Upgrade jquery to 3.3.1. ##
-v3.2.1 2017/12/23 - First release with jquery 3.2.1.
+v6.3.7.1 - Add jquery.parseQuery plugin. ### v5.3.7.1 - Upgrade jquery to
+v3.7.1. ### v5.1.0 - Add jquery.jstree plugin. ### v5.0.0 - Rename jquery3
+folder to jquery. - Mostly we use jquery plugins, for django ships with jquery
+already. - We put many jquery plugins in this package, so that we will not use
+jquery's version from now on. - Remove django from requirements. We still keep
+django's file structure, but we will need anything about django. ### v3.4.1.1 -
+Add jquery plugin: jquery.cookie. - Fix document. ### v3.4.1.0 - Upgrade jquery
+to 3.4.1. ### v3.3.1.1 - Upgrade jquery to 3.3.1. ## v3.2.1 - First release
+with jquery 3.2.1.
```

### Comparing `django-static-jquery3-5.3.7.1/django_static_jquery3.egg-info/SOURCES.txt` & `django-static-jquery3-6.3.7.1/django_static_jquery3.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 django_static_jquery3/static/jquery/licenses/.DS_Store
 django_static_jquery3/static/jquery/licenses/jquery/LICENSE.txt
 django_static_jquery3/static/jquery/licenses/jquery.cookie/MIT-LICENSE.txt
 django_static_jquery3/static/jquery/licenses/jquery.jstree/.DS_Store
 django_static_jquery3/static/jquery/licenses/jquery.jstree/LICENSE-MIT
 django_static_jquery3/static/jquery/plugins/.DS_Store
 django_static_jquery3/static/jquery/plugins/jquery.cookie.js
+django_static_jquery3/static/jquery/plugins/jquery.parseQuery.js
 django_static_jquery3/static/jquery/plugins/jquery.utils.js
 django_static_jquery3/static/jquery/plugins/jquery.jstree/.DS_Store
 django_static_jquery3/static/jquery/plugins/jquery.jstree/jstree.js
 django_static_jquery3/static/jquery/plugins/jquery.jstree/jstree.min.js
 django_static_jquery3/static/jquery/plugins/jquery.jstree/themes/default/32px.png
 django_static_jquery3/static/jquery/plugins/jquery.jstree/themes/default/40px.png
 django_static_jquery3/static/jquery/plugins/jquery.jstree/themes/default/style.css
```

### Comparing `django-static-jquery3-5.3.7.1/setup.py` & `django-static-jquery3-6.3.7.1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,22 +10,20 @@
 
 with open(os.path.join(here, "requirements.txt"), "r", encoding="utf-8") as fobj:
     requires = [x.strip() for x in fobj.readlines() if x.strip()]
 
 
 setup(
     name="django-static-jquery3",
-    version="5.3.7.1",
+    version="6.3.7.1",
     description="Django application contain jquery3 static files.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Chen JiaYong",
-    author_email="chenjiayong@zencore.cn",
     maintainer="Chen JiaYong",
-    maintainer_email="chenjiayong@zencore.cn",
     license="MIT",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
```

