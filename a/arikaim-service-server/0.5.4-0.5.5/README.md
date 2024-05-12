# Comparing `tmp/arikaim_service_server-0.5.4.tar.gz` & `tmp/arikaim_service_server-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arikaim_service_server-0.5.4.tar", last modified: Sat May 11 16:04:39 2024, max compression
+gzip compressed data, was "arikaim_service_server-0.5.5.tar", last modified: Sun May 12 07:17:45 2024, max compression
```

## Comparing `arikaim_service_server-0.5.4.tar` & `arikaim_service_server-0.5.5.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 theuser   (1000) theuser   (1000)        0 2024-05-11 16:04:39.082429 arikaim_service_server-0.5.4/
--rw-r--r--   0 theuser   (1000) theuser   (1000)      881 2024-05-11 16:04:39.082429 arikaim_service_server-0.5.4/PKG-INFO
--rwxr-xr-x   0 theuser   (1000) theuser   (1000)      357 2024-02-21 16:41:47.000000 arikaim_service_server-0.5.4/README.md
-drwxr-xr-x   0 theuser   (1000) theuser   (1000)        0 2024-05-11 16:04:39.078429 arikaim_service_server-0.5.4/arikaim/
-drwxr-xr-x   0 theuser   (1000) theuser   (1000)        0 2024-05-11 16:04:39.078429 arikaim_service_server-0.5.4/arikaim/core/
-drwxr-xr-x   0 theuser   (1000) theuser   (1000)        0 2024-05-11 16:04:39.082429 arikaim_service_server-0.5.4/arikaim/core/access/
--rw-r--r--   0 theuser   (1000) theuser   (1000)     2661 2024-02-21 16:41:47.000000 arikaim_service_server-0.5.4/arikaim/core/access/access.py
--rw-r--r--   0 theuser   (1000) theuser   (1000)       88 2024-02-21 16:41:47.000000 arikaim_service_server-0.5.4/arikaim/core/access/auth_error.py
-drwxr-xr-x   0 theuser   (1000) theuser   (1000)        0 2024-05-11 16:04:39.082429 arikaim_service_server-0.5.4/arikaim/core/access/middleware/
--rw-r--r--   0 theuser   (1000) theuser   (1000)      745 2024-02-21 16:41:47.000000 arikaim_service_server-0.5.4/arikaim/core/access/middleware/multiple.py
-drwxr-xr-x   0 theuser   (1000) theuser   (1000)        0 2024-05-11 16:04:39.082429 arikaim_service_server-0.5.4/arikaim/core/access/providers/
--rw-r--r--   0 theuser   (1000) theuser   (1000)     1644 2024-02-21 16:41:47.000000 arikaim_service_server-0.5.4/arikaim/core/access/providers/php_session.py
--rw-r--r--   0 theuser   (1000) theuser   (1000)      590 2024-02-21 16:41:47.000000 arikaim_service_server-0.5.4/arikaim/core/access/providers/token.py
-drwxr-xr-x   0 theuser   (1000) theuser   (1000)        0 2024-05-11 16:04:39.082429 arikaim_service_server-0.5.4/arikaim/core/admin/
--rw-r--r--   0 theuser   (1000) theuser   (1000)      907 2024-02-23 19:30:58.000000 arikaim_service_server-0.5.4/arikaim/core/admin/admin.py
-drwxr-xr-x   0 theuser   (1000) theuser   (1000)        0 2024-05-11 16:04:39.082429 arikaim_service_server-0.5.4/arikaim/core/admin/controllers/
--rw-r--r--   0 theuser   (1000) theuser   (1000)      416 2024-02-21 16:41:47.000000 arikaim_service_server-0.5.4/arikaim/core/admin/controllers/info.py
--rw-r--r--   0 theuser   (1000) theuser   (1000)      421 2024-02-21 16:41:47.000000 arikaim_service_server-0.5.4/arikaim/core/admin/controllers/service.py
--rw-r--r--   0 theuser   (1000) theuser   (1000)     1206 2024-02-21 16:41:47.000000 arikaim_service_server-0.5.4/arikaim/core/admin/controllers/service_route.py
--rw-r--r--   0 theuser   (1000) theuser   (1000)     1036 2024-02-21 16:41:47.000000 arikaim_service_server-0.5.4/arikaim/core/admin/controllers/service_routes.py
--rw-r--r--   0 theuser   (1000) theuser   (1000)      299 2024-02-21 16:41:47.000000 arikaim_service_server-0.5.4/arikaim/core/admin/controllers/services_list.py
--rw-r--r--   0 theuser   (1000) theuser   (1000)     1023 2024-02-21 16:41:47.000000 arikaim_service_server-0.5.4/arikaim/core/api_descriptor.py
--rw-r--r--   0 theuser   (1000) theuser   (1000)     4919 2024-05-11 11:06:28.000000 arikaim_service_server-0.5.4/arikaim/core/app.py
-drwxr-xr-x   0 theuser   (1000) theuser   (1000)        0 2024-05-11 16:04:39.082429 arikaim_service_server-0.5.4/arikaim/core/collection/
--rw-r--r--   0 theuser   (1000) theuser   (1000)     1670 2024-02-21 16:41:47.000000 arikaim_service_server-0.5.4/arikaim/core/collection/property.py
-drwxr-xr-x   0 theuser   (1000) theuser   (1000)        0 2024-05-11 16:04:39.082429 arikaim_service_server-0.5.4/arikaim/core/console/
--rw-r--r--   0 theuser   (1000) theuser   (1000)     1208 2024-05-11 11:04:46.000000 arikaim_service_server-0.5.4/arikaim/core/console/app.py
--rw-r--r--   0 theuser   (1000) theuser   (1000)      606 2024-02-23 18:56:43.000000 arikaim_service_server-0.5.4/arikaim/core/console/config.py
--rw-r--r--   0 theuser   (1000) theuser   (1000)      718 2024-02-23 19:35:55.000000 arikaim_service_server-0.5.4/arikaim/core/console/install.py
--rw-r--r--   0 theuser   (1000) theuser   (1000)      230 2024-05-11 11:04:53.000000 arikaim_service_server-0.5.4/arikaim/core/console/packages.py
-drwxr-xr-x   0 theuser   (1000) theuser   (1000)        0 2024-05-11 16:04:39.082429 arikaim_service_server-0.5.4/arikaim/core/console/templates/
--rw-r--r--   0 theuser   (1000) theuser   (1000)      386 2024-02-21 16:41:47.000000 arikaim_service_server-0.5.4/arikaim/core/console/templates/config_file.py
--rw-r--r--   0 theuser   (1000) theuser   (1000)      975 2024-05-11 07:27:27.000000 arikaim_service_server-0.5.4/arikaim/core/container.py
--rw-r--r--   0 theuser   (1000) theuser   (1000)     2725 2024-02-21 16:41:47.000000 arikaim_service_server-0.5.4/arikaim/core/controller.py
-drwxr-xr-x   0 theuser   (1000) theuser   (1000)        0 2024-05-11 16:04:39.082429 arikaim_service_server-0.5.4/arikaim/core/db/
--rw-r--r--   0 theuser   (1000) theuser   (1000)     1077 2024-02-23 19:35:44.000000 arikaim_service_server-0.5.4/arikaim/core/db/db.py
-drwxr-xr-x   0 theuser   (1000) theuser   (1000)        0 2024-05-11 16:04:39.082429 arikaim_service_server-0.5.4/arikaim/core/db/models/
--rw-r--r--   0 theuser   (1000) theuser   (1000)      465 2024-02-21 16:41:47.000000 arikaim_service_server-0.5.4/arikaim/core/db/models/access_tokens.py
--rw-r--r--   0 theuser   (1000) theuser   (1000)      916 2024-02-21 16:41:47.000000 arikaim_service_server-0.5.4/arikaim/core/db/models/jobs.py
--rw-r--r--   0 theuser   (1000) theuser   (1000)      496 2024-02-21 16:41:47.000000 arikaim_service_server-0.5.4/arikaim/core/db/models/permission_relations.py
--rw-r--r--   0 theuser   (1000) theuser   (1000)      454 2024-02-21 16:41:47.000000 arikaim_service_server-0.5.4/arikaim/core/db/models/permissions.py
--rw-r--r--   0 theuser   (1000) theuser   (1000)      509 2024-02-21 16:41:47.000000 arikaim_service_server-0.5.4/arikaim/core/db/models/users.py
--rw-r--r--   0 theuser   (1000) theuser   (1000)      649 2024-02-21 16:41:47.000000 arikaim_service_server-0.5.4/arikaim/core/errors.py
--rw-r--r--   0 theuser   (1000) theuser   (1000)      239 2024-05-11 11:03:31.000000 arikaim_service_server-0.5.4/arikaim/core/logger.py
--rw-r--r--   0 theuser   (1000) theuser   (1000)      927 2024-02-21 16:41:47.000000 arikaim_service_server-0.5.4/arikaim/core/packages.py
--rw-r--r--   0 theuser   (1000) theuser   (1000)     1453 2024-05-11 11:13:22.000000 arikaim_service_server-0.5.4/arikaim/core/path.py
-drwxr-xr-x   0 theuser   (1000) theuser   (1000)        0 2024-05-11 16:04:39.082429 arikaim_service_server-0.5.4/arikaim/core/queue/
--rw-r--r--   0 theuser   (1000) theuser   (1000)      282 2024-02-21 16:41:47.000000 arikaim_service_server-0.5.4/arikaim/core/queue/job.py
--rw-r--r--   0 theuser   (1000) theuser   (1000)     1980 2024-02-21 20:29:02.000000 arikaim_service_server-0.5.4/arikaim/core/queue/queue.py
--rw-r--r--   0 theuser   (1000) theuser   (1000)      443 2024-02-21 16:41:47.000000 arikaim_service_server-0.5.4/arikaim/core/response.py
--rw-r--r--   0 theuser   (1000) theuser   (1000)     1177 2024-05-11 11:06:40.000000 arikaim_service_server-0.5.4/arikaim/core/server.py
--rw-r--r--   0 theuser   (1000) theuser   (1000)     1702 2024-02-21 16:41:47.000000 arikaim_service_server-0.5.4/arikaim/core/service.py
--rw-r--r--   0 theuser   (1000) theuser   (1000)     2366 2024-02-21 16:41:47.000000 arikaim_service_server-0.5.4/arikaim/core/utils.py
--rwxr-xr-x   0 theuser   (1000) theuser   (1000)      109 2024-05-11 11:14:09.000000 arikaim_service_server-0.5.4/arikaim-server
-drwxr-xr-x   0 theuser   (1000) theuser   (1000)        0 2024-05-11 16:04:39.082429 arikaim_service_server-0.5.4/arikaim_service_server.egg-info/
--rw-r--r--   0 theuser   (1000) theuser   (1000)      881 2024-05-11 16:04:39.000000 arikaim_service_server-0.5.4/arikaim_service_server.egg-info/PKG-INFO
--rw-r--r--   0 theuser   (1000) theuser   (1000)     1467 2024-05-11 16:04:39.000000 arikaim_service_server-0.5.4/arikaim_service_server.egg-info/SOURCES.txt
--rw-r--r--   0 theuser   (1000) theuser   (1000)        1 2024-05-11 16:04:39.000000 arikaim_service_server-0.5.4/arikaim_service_server.egg-info/dependency_links.txt
--rw-r--r--   0 theuser   (1000) theuser   (1000)      112 2024-05-11 16:04:39.000000 arikaim_service_server-0.5.4/arikaim_service_server.egg-info/requires.txt
--rw-r--r--   0 theuser   (1000) theuser   (1000)        8 2024-05-11 16:04:39.000000 arikaim_service_server-0.5.4/arikaim_service_server.egg-info/top_level.txt
--rw-r--r--   0 theuser   (1000) theuser   (1000)       38 2024-05-11 16:04:39.082429 arikaim_service_server-0.5.4/setup.cfg
--rw-r--r--   0 theuser   (1000) theuser   (1000)     1779 2024-05-11 11:07:22.000000 arikaim_service_server-0.5.4/setup.py
+drwxr-xr-x   0 theuser   (1000) theuser   (1000)        0 2024-05-12 07:17:45.241559 arikaim_service_server-0.5.5/
+-rw-r--r--   0 theuser   (1000) theuser   (1000)      881 2024-05-12 07:17:45.241559 arikaim_service_server-0.5.5/PKG-INFO
+-rwxr-xr-x   0 theuser   (1000) theuser   (1000)      357 2024-02-21 16:41:47.000000 arikaim_service_server-0.5.5/README.md
+drwxr-xr-x   0 theuser   (1000) theuser   (1000)        0 2024-05-12 07:17:45.237559 arikaim_service_server-0.5.5/arikaim/
+drwxr-xr-x   0 theuser   (1000) theuser   (1000)        0 2024-05-12 07:17:45.241559 arikaim_service_server-0.5.5/arikaim/core/
+drwxr-xr-x   0 theuser   (1000) theuser   (1000)        0 2024-05-12 07:17:45.241559 arikaim_service_server-0.5.5/arikaim/core/access/
+-rw-r--r--   0 theuser   (1000) theuser   (1000)     2661 2024-02-21 16:41:47.000000 arikaim_service_server-0.5.5/arikaim/core/access/access.py
+-rw-r--r--   0 theuser   (1000) theuser   (1000)       88 2024-02-21 16:41:47.000000 arikaim_service_server-0.5.5/arikaim/core/access/auth_error.py
+drwxr-xr-x   0 theuser   (1000) theuser   (1000)        0 2024-05-12 07:17:45.241559 arikaim_service_server-0.5.5/arikaim/core/access/middleware/
+-rw-r--r--   0 theuser   (1000) theuser   (1000)      745 2024-02-21 16:41:47.000000 arikaim_service_server-0.5.5/arikaim/core/access/middleware/multiple.py
+drwxr-xr-x   0 theuser   (1000) theuser   (1000)        0 2024-05-12 07:17:45.241559 arikaim_service_server-0.5.5/arikaim/core/access/providers/
+-rw-r--r--   0 theuser   (1000) theuser   (1000)     1644 2024-02-21 16:41:47.000000 arikaim_service_server-0.5.5/arikaim/core/access/providers/php_session.py
+-rw-r--r--   0 theuser   (1000) theuser   (1000)      590 2024-02-21 16:41:47.000000 arikaim_service_server-0.5.5/arikaim/core/access/providers/token.py
+drwxr-xr-x   0 theuser   (1000) theuser   (1000)        0 2024-05-12 07:17:45.241559 arikaim_service_server-0.5.5/arikaim/core/admin/
+-rw-r--r--   0 theuser   (1000) theuser   (1000)      907 2024-02-23 19:30:58.000000 arikaim_service_server-0.5.5/arikaim/core/admin/admin.py
+drwxr-xr-x   0 theuser   (1000) theuser   (1000)        0 2024-05-12 07:17:45.241559 arikaim_service_server-0.5.5/arikaim/core/admin/controllers/
+-rw-r--r--   0 theuser   (1000) theuser   (1000)      416 2024-02-21 16:41:47.000000 arikaim_service_server-0.5.5/arikaim/core/admin/controllers/info.py
+-rw-r--r--   0 theuser   (1000) theuser   (1000)      421 2024-02-21 16:41:47.000000 arikaim_service_server-0.5.5/arikaim/core/admin/controllers/service.py
+-rw-r--r--   0 theuser   (1000) theuser   (1000)     1206 2024-02-21 16:41:47.000000 arikaim_service_server-0.5.5/arikaim/core/admin/controllers/service_route.py
+-rw-r--r--   0 theuser   (1000) theuser   (1000)     1036 2024-02-21 16:41:47.000000 arikaim_service_server-0.5.5/arikaim/core/admin/controllers/service_routes.py
+-rw-r--r--   0 theuser   (1000) theuser   (1000)      299 2024-02-21 16:41:47.000000 arikaim_service_server-0.5.5/arikaim/core/admin/controllers/services_list.py
+-rw-r--r--   0 theuser   (1000) theuser   (1000)     1023 2024-02-21 16:41:47.000000 arikaim_service_server-0.5.5/arikaim/core/api_descriptor.py
+-rw-r--r--   0 theuser   (1000) theuser   (1000)     5106 2024-05-12 07:14:49.000000 arikaim_service_server-0.5.5/arikaim/core/app.py
+drwxr-xr-x   0 theuser   (1000) theuser   (1000)        0 2024-05-12 07:17:45.241559 arikaim_service_server-0.5.5/arikaim/core/collection/
+-rw-r--r--   0 theuser   (1000) theuser   (1000)     1670 2024-02-21 16:41:47.000000 arikaim_service_server-0.5.5/arikaim/core/collection/property.py
+drwxr-xr-x   0 theuser   (1000) theuser   (1000)        0 2024-05-12 07:17:45.241559 arikaim_service_server-0.5.5/arikaim/core/console/
+-rw-r--r--   0 theuser   (1000) theuser   (1000)     1208 2024-05-11 11:04:46.000000 arikaim_service_server-0.5.5/arikaim/core/console/app.py
+-rw-r--r--   0 theuser   (1000) theuser   (1000)      606 2024-02-23 18:56:43.000000 arikaim_service_server-0.5.5/arikaim/core/console/config.py
+-rw-r--r--   0 theuser   (1000) theuser   (1000)      718 2024-02-23 19:35:55.000000 arikaim_service_server-0.5.5/arikaim/core/console/install.py
+-rw-r--r--   0 theuser   (1000) theuser   (1000)      230 2024-05-11 11:04:53.000000 arikaim_service_server-0.5.5/arikaim/core/console/packages.py
+drwxr-xr-x   0 theuser   (1000) theuser   (1000)        0 2024-05-12 07:17:45.241559 arikaim_service_server-0.5.5/arikaim/core/console/templates/
+-rw-r--r--   0 theuser   (1000) theuser   (1000)      386 2024-02-21 16:41:47.000000 arikaim_service_server-0.5.5/arikaim/core/console/templates/config_file.py
+-rw-r--r--   0 theuser   (1000) theuser   (1000)      975 2024-05-11 07:27:27.000000 arikaim_service_server-0.5.5/arikaim/core/container.py
+-rw-r--r--   0 theuser   (1000) theuser   (1000)     2725 2024-02-21 16:41:47.000000 arikaim_service_server-0.5.5/arikaim/core/controller.py
+drwxr-xr-x   0 theuser   (1000) theuser   (1000)        0 2024-05-12 07:17:45.241559 arikaim_service_server-0.5.5/arikaim/core/db/
+-rw-r--r--   0 theuser   (1000) theuser   (1000)     1077 2024-02-23 19:35:44.000000 arikaim_service_server-0.5.5/arikaim/core/db/db.py
+drwxr-xr-x   0 theuser   (1000) theuser   (1000)        0 2024-05-12 07:17:45.241559 arikaim_service_server-0.5.5/arikaim/core/db/models/
+-rw-r--r--   0 theuser   (1000) theuser   (1000)      465 2024-02-21 16:41:47.000000 arikaim_service_server-0.5.5/arikaim/core/db/models/access_tokens.py
+-rw-r--r--   0 theuser   (1000) theuser   (1000)      916 2024-02-21 16:41:47.000000 arikaim_service_server-0.5.5/arikaim/core/db/models/jobs.py
+-rw-r--r--   0 theuser   (1000) theuser   (1000)      496 2024-02-21 16:41:47.000000 arikaim_service_server-0.5.5/arikaim/core/db/models/permission_relations.py
+-rw-r--r--   0 theuser   (1000) theuser   (1000)      454 2024-02-21 16:41:47.000000 arikaim_service_server-0.5.5/arikaim/core/db/models/permissions.py
+-rw-r--r--   0 theuser   (1000) theuser   (1000)      509 2024-02-21 16:41:47.000000 arikaim_service_server-0.5.5/arikaim/core/db/models/users.py
+-rw-r--r--   0 theuser   (1000) theuser   (1000)      649 2024-02-21 16:41:47.000000 arikaim_service_server-0.5.5/arikaim/core/errors.py
+-rw-r--r--   0 theuser   (1000) theuser   (1000)      239 2024-05-11 11:03:31.000000 arikaim_service_server-0.5.5/arikaim/core/logger.py
+-rw-r--r--   0 theuser   (1000) theuser   (1000)      927 2024-02-21 16:41:47.000000 arikaim_service_server-0.5.5/arikaim/core/packages.py
+-rw-r--r--   0 theuser   (1000) theuser   (1000)     1453 2024-05-11 11:13:22.000000 arikaim_service_server-0.5.5/arikaim/core/path.py
+drwxr-xr-x   0 theuser   (1000) theuser   (1000)        0 2024-05-12 07:17:45.241559 arikaim_service_server-0.5.5/arikaim/core/queue/
+-rw-r--r--   0 theuser   (1000) theuser   (1000)      282 2024-02-21 16:41:47.000000 arikaim_service_server-0.5.5/arikaim/core/queue/job.py
+-rw-r--r--   0 theuser   (1000) theuser   (1000)     1980 2024-02-21 20:29:02.000000 arikaim_service_server-0.5.5/arikaim/core/queue/queue.py
+-rw-r--r--   0 theuser   (1000) theuser   (1000)      443 2024-02-21 16:41:47.000000 arikaim_service_server-0.5.5/arikaim/core/response.py
+-rw-r--r--   0 theuser   (1000) theuser   (1000)     1147 2024-05-12 07:17:08.000000 arikaim_service_server-0.5.5/arikaim/core/server.py
+-rw-r--r--   0 theuser   (1000) theuser   (1000)     1702 2024-02-21 16:41:47.000000 arikaim_service_server-0.5.5/arikaim/core/service.py
+-rw-r--r--   0 theuser   (1000) theuser   (1000)     2466 2024-05-12 07:12:38.000000 arikaim_service_server-0.5.5/arikaim/core/utils.py
+-rwxr-xr-x   0 theuser   (1000) theuser   (1000)      109 2024-05-11 11:14:09.000000 arikaim_service_server-0.5.5/arikaim-server
+drwxr-xr-x   0 theuser   (1000) theuser   (1000)        0 2024-05-12 07:17:45.241559 arikaim_service_server-0.5.5/arikaim_service_server.egg-info/
+-rw-r--r--   0 theuser   (1000) theuser   (1000)      881 2024-05-12 07:17:45.000000 arikaim_service_server-0.5.5/arikaim_service_server.egg-info/PKG-INFO
+-rw-r--r--   0 theuser   (1000) theuser   (1000)     1467 2024-05-12 07:17:45.000000 arikaim_service_server-0.5.5/arikaim_service_server.egg-info/SOURCES.txt
+-rw-r--r--   0 theuser   (1000) theuser   (1000)        1 2024-05-12 07:17:45.000000 arikaim_service_server-0.5.5/arikaim_service_server.egg-info/dependency_links.txt
+-rw-r--r--   0 theuser   (1000) theuser   (1000)      112 2024-05-12 07:17:45.000000 arikaim_service_server-0.5.5/arikaim_service_server.egg-info/requires.txt
+-rw-r--r--   0 theuser   (1000) theuser   (1000)        8 2024-05-12 07:17:45.000000 arikaim_service_server-0.5.5/arikaim_service_server.egg-info/top_level.txt
+-rw-r--r--   0 theuser   (1000) theuser   (1000)       38 2024-05-12 07:17:45.241559 arikaim_service_server-0.5.5/setup.cfg
+-rw-r--r--   0 theuser   (1000) theuser   (1000)     1779 2024-05-12 07:17:31.000000 arikaim_service_server-0.5.5/setup.py
```

### Comparing `arikaim_service_server-0.5.4/PKG-INFO` & `arikaim_service_server-0.5.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arikaim-service-server
-Version: 0.5.4
+Version: 0.5.5
 Summary: Arikaim python service server
 Home-page: 
 Download-URL: 
 Author: Intersoft Ltd
 Author-email: info@arikaim.com
 License: MIT License
 Keywords: arikaim
```

### Comparing `arikaim_service_server-0.5.4/arikaim/core/access/access.py` & `arikaim_service_server-0.5.5/arikaim/core/access/access.py`

 * *Files identical despite different names*

### Comparing `arikaim_service_server-0.5.4/arikaim/core/access/middleware/multiple.py` & `arikaim_service_server-0.5.5/arikaim/core/access/middleware/multiple.py`

 * *Files identical despite different names*

### Comparing `arikaim_service_server-0.5.4/arikaim/core/access/providers/php_session.py` & `arikaim_service_server-0.5.5/arikaim/core/access/providers/php_session.py`

 * *Files identical despite different names*

### Comparing `arikaim_service_server-0.5.4/arikaim/core/access/providers/token.py` & `arikaim_service_server-0.5.5/arikaim/core/access/providers/token.py`

 * *Files identical despite different names*

### Comparing `arikaim_service_server-0.5.4/arikaim/core/admin/admin.py` & `arikaim_service_server-0.5.5/arikaim/core/admin/admin.py`

 * *Files identical despite different names*

### Comparing `arikaim_service_server-0.5.4/arikaim/core/admin/controllers/service_route.py` & `arikaim_service_server-0.5.5/arikaim/core/admin/controllers/service_route.py`

 * *Files identical despite different names*

### Comparing `arikaim_service_server-0.5.4/arikaim/core/admin/controllers/service_routes.py` & `arikaim_service_server-0.5.5/arikaim/core/admin/controllers/service_routes.py`

 * *Files identical despite different names*

### Comparing `arikaim_service_server-0.5.4/arikaim/core/api_descriptor.py` & `arikaim_service_server-0.5.5/arikaim/core/api_descriptor.py`

 * *Files identical despite different names*

### Comparing `arikaim_service_server-0.5.4/arikaim/core/app.py` & `arikaim_service_server-0.5.5/arikaim/core/app.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-
+import traceback
 from starlette.applications import Starlette
 from starlette.middleware import Middleware
 from starlette.middleware.cors import CORSMiddleware
 from pymitter import EventEmitter
 
 from arikaim.core.utils import *
 from arikaim.core.db.db import *
@@ -49,23 +49,26 @@
         return self._services
     
     def get_service(self, name:str):
         if name in self._services_instance:
             return self._services_instance[name]
         else:
             return None
-    
+     
     def system_init(self):
-        # load config
-        self._config = load_module('config',os.path.join(Path.config(),'config.py'))
-
         # create event emiter 
         events = EventEmitter(wildcard = True)
         di.add('events',events)
 
+        # load config
+        self._config = load_module('config',os.path.join(Path.config(),'config.py'))
+        if self._config is None:
+            logger.error('Config file not found!')
+        return False
+
         # connect to db 
         db = Db(self._config.db)
         db.connect()
         # add to container
         di.add('db',db)
         
         #access
@@ -144,9 +147,13 @@
             if self._services_instance[service_name].routes != None:
                 self._routes.append(self._services_instance[service_name].routes)
 
     @property
     def starlette(self):
         return self._starlette
 
+    @property
+    def config(self):
+        return self._config
+
 
 app = ArikaimApp()
```

### Comparing `arikaim_service_server-0.5.4/arikaim/core/collection/property.py` & `arikaim_service_server-0.5.5/arikaim/core/collection/property.py`

 * *Files identical despite different names*

### Comparing `arikaim_service_server-0.5.4/arikaim/core/console/app.py` & `arikaim_service_server-0.5.5/arikaim/core/console/app.py`

 * *Files identical despite different names*

### Comparing `arikaim_service_server-0.5.4/arikaim/core/console/config.py` & `arikaim_service_server-0.5.5/arikaim/core/console/config.py`

 * *Files identical despite different names*

### Comparing `arikaim_service_server-0.5.4/arikaim/core/console/install.py` & `arikaim_service_server-0.5.5/arikaim/core/console/install.py`

 * *Files identical despite different names*

### Comparing `arikaim_service_server-0.5.4/arikaim/core/container.py` & `arikaim_service_server-0.5.5/arikaim/core/container.py`

 * *Files identical despite different names*

### Comparing `arikaim_service_server-0.5.4/arikaim/core/controller.py` & `arikaim_service_server-0.5.5/arikaim/core/controller.py`

 * *Files identical despite different names*

### Comparing `arikaim_service_server-0.5.4/arikaim/core/db/db.py` & `arikaim_service_server-0.5.5/arikaim/core/db/db.py`

 * *Files identical despite different names*

### Comparing `arikaim_service_server-0.5.4/arikaim/core/db/models/jobs.py` & `arikaim_service_server-0.5.5/arikaim/core/db/models/jobs.py`

 * *Files identical despite different names*

### Comparing `arikaim_service_server-0.5.4/arikaim/core/errors.py` & `arikaim_service_server-0.5.5/arikaim/core/errors.py`

 * *Files identical despite different names*

### Comparing `arikaim_service_server-0.5.4/arikaim/core/packages.py` & `arikaim_service_server-0.5.5/arikaim/core/packages.py`

 * *Files identical despite different names*

### Comparing `arikaim_service_server-0.5.4/arikaim/core/path.py` & `arikaim_service_server-0.5.5/arikaim/core/path.py`

 * *Files identical despite different names*

### Comparing `arikaim_service_server-0.5.4/arikaim/core/queue/queue.py` & `arikaim_service_server-0.5.5/arikaim/core/queue/queue.py`

 * *Files identical despite different names*

### Comparing `arikaim_service_server-0.5.4/arikaim/core/server.py` & `arikaim_service_server-0.5.5/arikaim/core/server.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 import uvicorn
 from peewee import *
 
 from arikaim.core.logger import logger
 from arikaim.core.utils import *
+from arikaim.core.app import app
 
 class ArikaimServer:
     _instance = None
 
-    def __init__(self):
-        self._version = '0.5.4'
-        self._config = None
+    def __init__(self,config):
+        self._version = '0.5.5'
+        self._config = config
         
     def run(self, reload = False):
-
-        self._config = load_module('config',os.path.join(Path.config(),'config.py'))
-        
+  
         if reload == True:
             logger.info('Dev mode (reload)')
 
         uvicorn.run(
             'arikaim.core.app:app.boot', 
             reload = reload,
             factory = True,
@@ -33,13 +32,13 @@
     
     @property 
     def version(self):
         return self._version
 
     @classmethod
     def instance(cls):
-        if cls._instance is None: 
-            cls._instance = ArikaimServer()
+        if cls._instance is None:           
+            cls._instance = ArikaimServer(app.config)
           
         return cls._instance
     
 arikaim_server = ArikaimServer.instance()
```

### Comparing `arikaim_service_server-0.5.4/arikaim/core/service.py` & `arikaim_service_server-0.5.5/arikaim/core/service.py`

 * *Files identical despite different names*

### Comparing `arikaim_service_server-0.5.4/arikaim/core/utils.py` & `arikaim_service_server-0.5.5/arikaim/core/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,16 +31,20 @@
 def load_module_vars(path, module_name):
     module_path = os.path.join(path)
     sys.path.append(module_path)
 
     return importlib.import_module(module_name, package = module_name)
    
 def load_module(name, path):
-    return imp.load_source(name,path)
-
+    try:
+        return imp.load_source(name,path)
+    except BaseException as e:
+        print(format(e))       
+        return None
+    
 def parse_text(text, vars):
     template = Template(text)
     return template.substitute(vars)
 
 def singleton(class_):
     class class_w(class_):
         _instance = None
```

### Comparing `arikaim_service_server-0.5.4/arikaim_service_server.egg-info/PKG-INFO` & `arikaim_service_server-0.5.5/arikaim_service_server.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arikaim-service-server
-Version: 0.5.4
+Version: 0.5.5
 Summary: Arikaim python service server
 Home-page: 
 Download-URL: 
 Author: Intersoft Ltd
 Author-email: info@arikaim.com
 License: MIT License
 Keywords: arikaim
```

### Comparing `arikaim_service_server-0.5.4/arikaim_service_server.egg-info/SOURCES.txt` & `arikaim_service_server-0.5.5/arikaim_service_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arikaim_service_server-0.5.4/setup.py` & `arikaim_service_server-0.5.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     'arikaim.core.console.templates',
     'arikaim.core.db',
     'arikaim.core.queue',
     'arikaim.core.db.models'
 ],
    
 # Project version number:
-version='0.5.4',
+version='0.5.5',
 
 # List a license for the project, eg. MIT License
 license='MIT License',
 
 # Short description of your library: 
 description='Arikaim python service server',
```

