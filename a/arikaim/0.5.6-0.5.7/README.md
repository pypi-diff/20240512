# Comparing `tmp/arikaim-0.5.6.tar.gz` & `tmp/arikaim-0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arikaim-0.5.6.tar", last modified: Sun May 12 08:03:26 2024, max compression
+gzip compressed data, was "arikaim-0.5.7.tar", last modified: Sun May 12 10:20:11 2024, max compression
```

## Comparing `arikaim-0.5.6.tar` & `arikaim-0.5.7.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 theuser   (1000) theuser   (1000)        0 2024-05-12 08:03:26.769632 arikaim-0.5.6/
--rw-r--r--   0 theuser   (1000) theuser   (1000)      876 2024-05-12 08:03:26.765632 arikaim-0.5.6/PKG-INFO
--rwxr-xr-x   0 theuser   (1000) theuser   (1000)      315 2024-05-12 08:03:07.000000 arikaim-0.5.6/README.md
-drwxr-xr-x   0 theuser   (1000) theuser   (1000)        0 2024-05-12 08:03:26.761632 arikaim-0.5.6/arikaim/
-drwxr-xr-x   0 theuser   (1000) theuser   (1000)        0 2024-05-12 08:03:26.765632 arikaim-0.5.6/arikaim/core/
-drwxr-xr-x   0 theuser   (1000) theuser   (1000)        0 2024-05-12 08:03:26.765632 arikaim-0.5.6/arikaim/core/access/
--rw-r--r--   0 theuser   (1000) theuser   (1000)     2661 2024-02-21 16:41:47.000000 arikaim-0.5.6/arikaim/core/access/access.py
--rw-r--r--   0 theuser   (1000) theuser   (1000)       88 2024-02-21 16:41:47.000000 arikaim-0.5.6/arikaim/core/access/auth_error.py
-drwxr-xr-x   0 theuser   (1000) theuser   (1000)        0 2024-05-12 08:03:26.765632 arikaim-0.5.6/arikaim/core/access/middleware/
--rw-r--r--   0 theuser   (1000) theuser   (1000)      745 2024-02-21 16:41:47.000000 arikaim-0.5.6/arikaim/core/access/middleware/multiple.py
-drwxr-xr-x   0 theuser   (1000) theuser   (1000)        0 2024-05-12 08:03:26.765632 arikaim-0.5.6/arikaim/core/access/providers/
--rw-r--r--   0 theuser   (1000) theuser   (1000)     1644 2024-02-21 16:41:47.000000 arikaim-0.5.6/arikaim/core/access/providers/php_session.py
--rw-r--r--   0 theuser   (1000) theuser   (1000)      590 2024-02-21 16:41:47.000000 arikaim-0.5.6/arikaim/core/access/providers/token.py
-drwxr-xr-x   0 theuser   (1000) theuser   (1000)        0 2024-05-12 08:03:26.765632 arikaim-0.5.6/arikaim/core/admin/
--rw-r--r--   0 theuser   (1000) theuser   (1000)      907 2024-02-23 19:30:58.000000 arikaim-0.5.6/arikaim/core/admin/admin.py
-drwxr-xr-x   0 theuser   (1000) theuser   (1000)        0 2024-05-12 08:03:26.765632 arikaim-0.5.6/arikaim/core/admin/controllers/
--rw-r--r--   0 theuser   (1000) theuser   (1000)      416 2024-02-21 16:41:47.000000 arikaim-0.5.6/arikaim/core/admin/controllers/info.py
--rw-r--r--   0 theuser   (1000) theuser   (1000)      421 2024-02-21 16:41:47.000000 arikaim-0.5.6/arikaim/core/admin/controllers/service.py
--rw-r--r--   0 theuser   (1000) theuser   (1000)     1206 2024-02-21 16:41:47.000000 arikaim-0.5.6/arikaim/core/admin/controllers/service_route.py
--rw-r--r--   0 theuser   (1000) theuser   (1000)     1036 2024-02-21 16:41:47.000000 arikaim-0.5.6/arikaim/core/admin/controllers/service_routes.py
--rw-r--r--   0 theuser   (1000) theuser   (1000)      299 2024-02-21 16:41:47.000000 arikaim-0.5.6/arikaim/core/admin/controllers/services_list.py
--rw-r--r--   0 theuser   (1000) theuser   (1000)     1023 2024-02-21 16:41:47.000000 arikaim-0.5.6/arikaim/core/api_descriptor.py
--rw-r--r--   0 theuser   (1000) theuser   (1000)     5108 2024-05-12 07:55:21.000000 arikaim-0.5.6/arikaim/core/app.py
-drwxr-xr-x   0 theuser   (1000) theuser   (1000)        0 2024-05-12 08:03:26.765632 arikaim-0.5.6/arikaim/core/collection/
--rw-r--r--   0 theuser   (1000) theuser   (1000)     1670 2024-02-21 16:41:47.000000 arikaim-0.5.6/arikaim/core/collection/property.py
-drwxr-xr-x   0 theuser   (1000) theuser   (1000)        0 2024-05-12 08:03:26.765632 arikaim-0.5.6/arikaim/core/console/
--rw-r--r--   0 theuser   (1000) theuser   (1000)     1208 2024-05-12 07:50:14.000000 arikaim-0.5.6/arikaim/core/console/app.py
--rw-r--r--   0 theuser   (1000) theuser   (1000)      606 2024-02-23 18:56:43.000000 arikaim-0.5.6/arikaim/core/console/config.py
--rw-r--r--   0 theuser   (1000) theuser   (1000)      718 2024-02-23 19:35:55.000000 arikaim-0.5.6/arikaim/core/console/install.py
--rw-r--r--   0 theuser   (1000) theuser   (1000)      230 2024-05-11 11:04:53.000000 arikaim-0.5.6/arikaim/core/console/packages.py
-drwxr-xr-x   0 theuser   (1000) theuser   (1000)        0 2024-05-12 08:03:26.765632 arikaim-0.5.6/arikaim/core/console/templates/
--rw-r--r--   0 theuser   (1000) theuser   (1000)      386 2024-02-21 16:41:47.000000 arikaim-0.5.6/arikaim/core/console/templates/config_file.py
--rw-r--r--   0 theuser   (1000) theuser   (1000)     1041 2024-05-12 07:52:57.000000 arikaim-0.5.6/arikaim/core/container.py
--rw-r--r--   0 theuser   (1000) theuser   (1000)     2725 2024-02-21 16:41:47.000000 arikaim-0.5.6/arikaim/core/controller.py
-drwxr-xr-x   0 theuser   (1000) theuser   (1000)        0 2024-05-12 08:03:26.765632 arikaim-0.5.6/arikaim/core/db/
--rw-r--r--   0 theuser   (1000) theuser   (1000)     1077 2024-02-23 19:35:44.000000 arikaim-0.5.6/arikaim/core/db/db.py
-drwxr-xr-x   0 theuser   (1000) theuser   (1000)        0 2024-05-12 08:03:26.765632 arikaim-0.5.6/arikaim/core/db/models/
--rw-r--r--   0 theuser   (1000) theuser   (1000)      465 2024-02-21 16:41:47.000000 arikaim-0.5.6/arikaim/core/db/models/access_tokens.py
--rw-r--r--   0 theuser   (1000) theuser   (1000)      916 2024-02-21 16:41:47.000000 arikaim-0.5.6/arikaim/core/db/models/jobs.py
--rw-r--r--   0 theuser   (1000) theuser   (1000)      496 2024-02-21 16:41:47.000000 arikaim-0.5.6/arikaim/core/db/models/permission_relations.py
--rw-r--r--   0 theuser   (1000) theuser   (1000)      454 2024-02-21 16:41:47.000000 arikaim-0.5.6/arikaim/core/db/models/permissions.py
--rw-r--r--   0 theuser   (1000) theuser   (1000)      509 2024-02-21 16:41:47.000000 arikaim-0.5.6/arikaim/core/db/models/users.py
--rw-r--r--   0 theuser   (1000) theuser   (1000)      649 2024-02-21 16:41:47.000000 arikaim-0.5.6/arikaim/core/errors.py
--rw-r--r--   0 theuser   (1000) theuser   (1000)      239 2024-05-11 11:03:31.000000 arikaim-0.5.6/arikaim/core/logger.py
--rw-r--r--   0 theuser   (1000) theuser   (1000)      927 2024-02-21 16:41:47.000000 arikaim-0.5.6/arikaim/core/packages.py
--rw-r--r--   0 theuser   (1000) theuser   (1000)     1453 2024-05-11 11:13:22.000000 arikaim-0.5.6/arikaim/core/path.py
-drwxr-xr-x   0 theuser   (1000) theuser   (1000)        0 2024-05-12 08:03:26.765632 arikaim-0.5.6/arikaim/core/queue/
--rw-r--r--   0 theuser   (1000) theuser   (1000)      282 2024-02-21 16:41:47.000000 arikaim-0.5.6/arikaim/core/queue/job.py
--rw-r--r--   0 theuser   (1000) theuser   (1000)     1980 2024-02-21 20:29:02.000000 arikaim-0.5.6/arikaim/core/queue/queue.py
--rw-r--r--   0 theuser   (1000) theuser   (1000)      443 2024-02-21 16:41:47.000000 arikaim-0.5.6/arikaim/core/response.py
--rw-r--r--   0 theuser   (1000) theuser   (1000)     1147 2024-05-12 08:02:21.000000 arikaim-0.5.6/arikaim/core/server.py
--rw-r--r--   0 theuser   (1000) theuser   (1000)     1702 2024-02-21 16:41:47.000000 arikaim-0.5.6/arikaim/core/service.py
--rw-r--r--   0 theuser   (1000) theuser   (1000)     2466 2024-05-12 07:12:38.000000 arikaim-0.5.6/arikaim/core/utils.py
--rwxr-xr-x   0 theuser   (1000) theuser   (1000)      109 2024-05-11 11:14:09.000000 arikaim-0.5.6/arikaim-server
-drwxr-xr-x   0 theuser   (1000) theuser   (1000)        0 2024-05-12 08:03:26.765632 arikaim-0.5.6/arikaim.egg-info/
--rw-r--r--   0 theuser   (1000) theuser   (1000)      876 2024-05-12 08:03:26.000000 arikaim-0.5.6/arikaim.egg-info/PKG-INFO
--rw-r--r--   0 theuser   (1000) theuser   (1000)     1392 2024-05-12 08:03:26.000000 arikaim-0.5.6/arikaim.egg-info/SOURCES.txt
--rw-r--r--   0 theuser   (1000) theuser   (1000)        1 2024-05-12 08:03:26.000000 arikaim-0.5.6/arikaim.egg-info/dependency_links.txt
--rw-r--r--   0 theuser   (1000) theuser   (1000)      112 2024-05-12 08:03:26.000000 arikaim-0.5.6/arikaim.egg-info/requires.txt
--rw-r--r--   0 theuser   (1000) theuser   (1000)        8 2024-05-12 08:03:26.000000 arikaim-0.5.6/arikaim.egg-info/top_level.txt
--rw-r--r--   0 theuser   (1000) theuser   (1000)       38 2024-05-12 08:03:26.769632 arikaim-0.5.6/setup.cfg
--rw-r--r--   0 theuser   (1000) theuser   (1000)     1832 2024-05-12 08:01:16.000000 arikaim-0.5.6/setup.py
+drwxr-xr-x   0 theuser   (1000) theuser   (1000)        0 2024-05-12 10:20:11.387724 arikaim-0.5.7/
+-rw-r--r--   0 theuser   (1000) theuser   (1000)      872 2024-05-12 10:20:11.387724 arikaim-0.5.7/PKG-INFO
+-rwxr-xr-x   0 theuser   (1000) theuser   (1000)      315 2024-05-12 08:20:51.000000 arikaim-0.5.7/README.md
+drwxr-xr-x   0 theuser   (1000) theuser   (1000)        0 2024-05-12 10:20:11.383724 arikaim-0.5.7/arikaim/
+drwxr-xr-x   0 theuser   (1000) theuser   (1000)        0 2024-05-12 10:20:11.383724 arikaim-0.5.7/arikaim/core/
+drwxr-xr-x   0 theuser   (1000) theuser   (1000)        0 2024-05-12 10:20:11.383724 arikaim-0.5.7/arikaim/core/access/
+-rw-r--r--   0 theuser   (1000) theuser   (1000)     2661 2024-02-21 16:41:47.000000 arikaim-0.5.7/arikaim/core/access/access.py
+-rw-r--r--   0 theuser   (1000) theuser   (1000)       88 2024-02-21 16:41:47.000000 arikaim-0.5.7/arikaim/core/access/auth_error.py
+drwxr-xr-x   0 theuser   (1000) theuser   (1000)        0 2024-05-12 10:20:11.383724 arikaim-0.5.7/arikaim/core/access/middleware/
+-rw-r--r--   0 theuser   (1000) theuser   (1000)      745 2024-02-21 16:41:47.000000 arikaim-0.5.7/arikaim/core/access/middleware/multiple.py
+drwxr-xr-x   0 theuser   (1000) theuser   (1000)        0 2024-05-12 10:20:11.383724 arikaim-0.5.7/arikaim/core/access/providers/
+-rw-r--r--   0 theuser   (1000) theuser   (1000)     1644 2024-02-21 16:41:47.000000 arikaim-0.5.7/arikaim/core/access/providers/php_session.py
+-rw-r--r--   0 theuser   (1000) theuser   (1000)      590 2024-02-21 16:41:47.000000 arikaim-0.5.7/arikaim/core/access/providers/token.py
+drwxr-xr-x   0 theuser   (1000) theuser   (1000)        0 2024-05-12 10:20:11.383724 arikaim-0.5.7/arikaim/core/admin/
+-rw-r--r--   0 theuser   (1000) theuser   (1000)      907 2024-02-23 19:30:58.000000 arikaim-0.5.7/arikaim/core/admin/admin.py
+drwxr-xr-x   0 theuser   (1000) theuser   (1000)        0 2024-05-12 10:20:11.387724 arikaim-0.5.7/arikaim/core/admin/controllers/
+-rw-r--r--   0 theuser   (1000) theuser   (1000)      416 2024-02-21 16:41:47.000000 arikaim-0.5.7/arikaim/core/admin/controllers/info.py
+-rw-r--r--   0 theuser   (1000) theuser   (1000)      421 2024-02-21 16:41:47.000000 arikaim-0.5.7/arikaim/core/admin/controllers/service.py
+-rw-r--r--   0 theuser   (1000) theuser   (1000)     1206 2024-02-21 16:41:47.000000 arikaim-0.5.7/arikaim/core/admin/controllers/service_route.py
+-rw-r--r--   0 theuser   (1000) theuser   (1000)     1036 2024-02-21 16:41:47.000000 arikaim-0.5.7/arikaim/core/admin/controllers/service_routes.py
+-rw-r--r--   0 theuser   (1000) theuser   (1000)      299 2024-02-21 16:41:47.000000 arikaim-0.5.7/arikaim/core/admin/controllers/services_list.py
+-rw-r--r--   0 theuser   (1000) theuser   (1000)     1023 2024-02-21 16:41:47.000000 arikaim-0.5.7/arikaim/core/api_descriptor.py
+-rw-r--r--   0 theuser   (1000) theuser   (1000)     5108 2024-05-12 07:55:21.000000 arikaim-0.5.7/arikaim/core/app.py
+drwxr-xr-x   0 theuser   (1000) theuser   (1000)        0 2024-05-12 10:20:11.387724 arikaim-0.5.7/arikaim/core/collection/
+-rw-r--r--   0 theuser   (1000) theuser   (1000)     1670 2024-02-21 16:41:47.000000 arikaim-0.5.7/arikaim/core/collection/property.py
+drwxr-xr-x   0 theuser   (1000) theuser   (1000)        0 2024-05-12 10:20:11.387724 arikaim-0.5.7/arikaim/core/console/
+-rw-r--r--   0 theuser   (1000) theuser   (1000)     1268 2024-05-12 10:13:01.000000 arikaim-0.5.7/arikaim/core/console/app.py
+-rw-r--r--   0 theuser   (1000) theuser   (1000)      606 2024-02-23 18:56:43.000000 arikaim-0.5.7/arikaim/core/console/config.py
+-rw-r--r--   0 theuser   (1000) theuser   (1000)      718 2024-02-23 19:35:55.000000 arikaim-0.5.7/arikaim/core/console/install.py
+-rw-r--r--   0 theuser   (1000) theuser   (1000)      230 2024-05-11 11:04:53.000000 arikaim-0.5.7/arikaim/core/console/packages.py
+drwxr-xr-x   0 theuser   (1000) theuser   (1000)        0 2024-05-12 10:20:11.387724 arikaim-0.5.7/arikaim/core/console/templates/
+-rw-r--r--   0 theuser   (1000) theuser   (1000)      386 2024-02-21 16:41:47.000000 arikaim-0.5.7/arikaim/core/console/templates/config_file.py
+-rw-r--r--   0 theuser   (1000) theuser   (1000)     1041 2024-05-12 07:52:57.000000 arikaim-0.5.7/arikaim/core/container.py
+-rw-r--r--   0 theuser   (1000) theuser   (1000)     2725 2024-02-21 16:41:47.000000 arikaim-0.5.7/arikaim/core/controller.py
+drwxr-xr-x   0 theuser   (1000) theuser   (1000)        0 2024-05-12 10:20:11.387724 arikaim-0.5.7/arikaim/core/db/
+-rw-r--r--   0 theuser   (1000) theuser   (1000)     1077 2024-02-23 19:35:44.000000 arikaim-0.5.7/arikaim/core/db/db.py
+drwxr-xr-x   0 theuser   (1000) theuser   (1000)        0 2024-05-12 10:20:11.387724 arikaim-0.5.7/arikaim/core/db/models/
+-rw-r--r--   0 theuser   (1000) theuser   (1000)      465 2024-02-21 16:41:47.000000 arikaim-0.5.7/arikaim/core/db/models/access_tokens.py
+-rw-r--r--   0 theuser   (1000) theuser   (1000)      916 2024-02-21 16:41:47.000000 arikaim-0.5.7/arikaim/core/db/models/jobs.py
+-rw-r--r--   0 theuser   (1000) theuser   (1000)      496 2024-02-21 16:41:47.000000 arikaim-0.5.7/arikaim/core/db/models/permission_relations.py
+-rw-r--r--   0 theuser   (1000) theuser   (1000)      454 2024-02-21 16:41:47.000000 arikaim-0.5.7/arikaim/core/db/models/permissions.py
+-rw-r--r--   0 theuser   (1000) theuser   (1000)      509 2024-02-21 16:41:47.000000 arikaim-0.5.7/arikaim/core/db/models/users.py
+-rw-r--r--   0 theuser   (1000) theuser   (1000)      649 2024-02-21 16:41:47.000000 arikaim-0.5.7/arikaim/core/errors.py
+-rw-r--r--   0 theuser   (1000) theuser   (1000)      239 2024-05-11 11:03:31.000000 arikaim-0.5.7/arikaim/core/logger.py
+-rw-r--r--   0 theuser   (1000) theuser   (1000)      927 2024-02-21 16:41:47.000000 arikaim-0.5.7/arikaim/core/packages.py
+-rw-r--r--   0 theuser   (1000) theuser   (1000)     1453 2024-05-11 11:13:22.000000 arikaim-0.5.7/arikaim/core/path.py
+drwxr-xr-x   0 theuser   (1000) theuser   (1000)        0 2024-05-12 10:20:11.387724 arikaim-0.5.7/arikaim/core/queue/
+-rw-r--r--   0 theuser   (1000) theuser   (1000)      282 2024-02-21 16:41:47.000000 arikaim-0.5.7/arikaim/core/queue/job.py
+-rw-r--r--   0 theuser   (1000) theuser   (1000)     1980 2024-02-21 20:29:02.000000 arikaim-0.5.7/arikaim/core/queue/queue.py
+-rw-r--r--   0 theuser   (1000) theuser   (1000)      443 2024-02-21 16:41:47.000000 arikaim-0.5.7/arikaim/core/response.py
+-rw-r--r--   0 theuser   (1000) theuser   (1000)     1298 2024-05-12 10:18:49.000000 arikaim-0.5.7/arikaim/core/server.py
+-rw-r--r--   0 theuser   (1000) theuser   (1000)     1702 2024-02-21 16:41:47.000000 arikaim-0.5.7/arikaim/core/service.py
+-rw-r--r--   0 theuser   (1000) theuser   (1000)     2466 2024-05-12 07:12:38.000000 arikaim-0.5.7/arikaim/core/utils.py
+-rwxr-xr-x   0 theuser   (1000) theuser   (1000)      109 2024-05-11 11:14:09.000000 arikaim-0.5.7/arikaim-server
+drwxr-xr-x   0 theuser   (1000) theuser   (1000)        0 2024-05-12 10:20:11.387724 arikaim-0.5.7/arikaim.egg-info/
+-rw-r--r--   0 theuser   (1000) theuser   (1000)      872 2024-05-12 10:20:11.000000 arikaim-0.5.7/arikaim.egg-info/PKG-INFO
+-rw-r--r--   0 theuser   (1000) theuser   (1000)     1392 2024-05-12 10:20:11.000000 arikaim-0.5.7/arikaim.egg-info/SOURCES.txt
+-rw-r--r--   0 theuser   (1000) theuser   (1000)        1 2024-05-12 10:20:11.000000 arikaim-0.5.7/arikaim.egg-info/dependency_links.txt
+-rw-r--r--   0 theuser   (1000) theuser   (1000)      112 2024-05-12 10:20:11.000000 arikaim-0.5.7/arikaim.egg-info/requires.txt
+-rw-r--r--   0 theuser   (1000) theuser   (1000)        8 2024-05-12 10:20:11.000000 arikaim-0.5.7/arikaim.egg-info/top_level.txt
+-rw-r--r--   0 theuser   (1000) theuser   (1000)       38 2024-05-12 10:20:11.387724 arikaim-0.5.7/setup.cfg
+-rw-r--r--   0 theuser   (1000) theuser   (1000)     1832 2024-05-12 10:19:45.000000 arikaim-0.5.7/setup.py
```

### Comparing `arikaim-0.5.6/PKG-INFO` & `arikaim-0.5.7/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arikaim
-Version: 0.5.6
+Version: 0.5.7
 Summary: Arikaim services server
 Home-page: https://github.com/arikaim/arikaim-services-server.git
 Download-URL: 
 Author: Intersoft Ltd
 Author-email: info@arikaim.com
 License: MIT License
 Keywords: arikaim
@@ -39,15 +39,19 @@
 ```
 
 #### Usage
 
 ##### Run
 
 ```sh
-    arikaim-server run
+
+arikaim-server run
+
 ```
 
 ##### Create config file
 
 ```sh
-    arikaim-server config create
+
+arikaim-server config create
+
 ```
```

### Comparing `arikaim-0.5.6/arikaim/core/access/access.py` & `arikaim-0.5.7/arikaim/core/access/access.py`

 * *Files identical despite different names*

### Comparing `arikaim-0.5.6/arikaim/core/access/middleware/multiple.py` & `arikaim-0.5.7/arikaim/core/access/middleware/multiple.py`

 * *Files identical despite different names*

### Comparing `arikaim-0.5.6/arikaim/core/access/providers/php_session.py` & `arikaim-0.5.7/arikaim/core/access/providers/php_session.py`

 * *Files identical despite different names*

### Comparing `arikaim-0.5.6/arikaim/core/access/providers/token.py` & `arikaim-0.5.7/arikaim/core/access/providers/token.py`

 * *Files identical despite different names*

### Comparing `arikaim-0.5.6/arikaim/core/admin/admin.py` & `arikaim-0.5.7/arikaim/core/admin/admin.py`

 * *Files identical despite different names*

### Comparing `arikaim-0.5.6/arikaim/core/admin/controllers/service_route.py` & `arikaim-0.5.7/arikaim/core/admin/controllers/service_route.py`

 * *Files identical despite different names*

### Comparing `arikaim-0.5.6/arikaim/core/admin/controllers/service_routes.py` & `arikaim-0.5.7/arikaim/core/admin/controllers/service_routes.py`

 * *Files identical despite different names*

### Comparing `arikaim-0.5.6/arikaim/core/api_descriptor.py` & `arikaim-0.5.7/arikaim/core/api_descriptor.py`

 * *Files identical despite different names*

### Comparing `arikaim-0.5.6/arikaim/core/app.py` & `arikaim-0.5.7/arikaim/core/app.py`

 * *Files identical despite different names*

### Comparing `arikaim-0.5.6/arikaim/core/collection/property.py` & `arikaim-0.5.7/arikaim/core/collection/property.py`

 * *Files identical despite different names*

### Comparing `arikaim-0.5.6/arikaim/core/console/app.py` & `arikaim-0.5.7/arikaim/core/console/app.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,20 +17,21 @@
     print("")
 
     if not ctx.invoked_subcommand:
         click.echo(ctx.get_help())
 
 @click.command()
 @click.argument('mode', required = False)
-def run(mode = None):
+@click.option('--path', required = False)
+def run(mode = None, path = None):
     # run server
     if mode == 'dev':
         mode = True
  
-    arikaim_server.run(mode)
+    arikaim_server.run(mode,path)
 
 @click.command()
 @click.argument('service-name')
 @click.argument('module-name')
 def cli(service_name: str, module_name: str):
     logger.info('Service: ' + service_name + ' load console commands ...')
     module = app.load_console_commands(service_name,module_name)
```

### Comparing `arikaim-0.5.6/arikaim/core/console/config.py` & `arikaim-0.5.7/arikaim/core/console/config.py`

 * *Files identical despite different names*

### Comparing `arikaim-0.5.6/arikaim/core/console/install.py` & `arikaim-0.5.7/arikaim/core/console/install.py`

 * *Files identical despite different names*

### Comparing `arikaim-0.5.6/arikaim/core/container.py` & `arikaim-0.5.7/arikaim/core/container.py`

 * *Files identical despite different names*

### Comparing `arikaim-0.5.6/arikaim/core/controller.py` & `arikaim-0.5.7/arikaim/core/controller.py`

 * *Files identical despite different names*

### Comparing `arikaim-0.5.6/arikaim/core/db/db.py` & `arikaim-0.5.7/arikaim/core/db/db.py`

 * *Files identical despite different names*

### Comparing `arikaim-0.5.6/arikaim/core/db/models/jobs.py` & `arikaim-0.5.7/arikaim/core/db/models/jobs.py`

 * *Files identical despite different names*

### Comparing `arikaim-0.5.6/arikaim/core/errors.py` & `arikaim-0.5.7/arikaim/core/errors.py`

 * *Files identical despite different names*

### Comparing `arikaim-0.5.6/arikaim/core/packages.py` & `arikaim-0.5.7/arikaim/core/packages.py`

 * *Files identical despite different names*

### Comparing `arikaim-0.5.6/arikaim/core/path.py` & `arikaim-0.5.7/arikaim/core/path.py`

 * *Files identical despite different names*

### Comparing `arikaim-0.5.6/arikaim/core/queue/queue.py` & `arikaim-0.5.7/arikaim/core/queue/queue.py`

 * *Files identical despite different names*

### Comparing `arikaim-0.5.6/arikaim/core/server.py` & `arikaim-0.5.7/arikaim/core/server.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,19 +5,22 @@
 from arikaim.core.utils import *
 from arikaim.core.app import app
 
 class ArikaimServer:
     _instance = None
 
     def __init__(self,config):
-        self._version = '0.5.6'
+        self._version = '0.5.7'
         self._config = config
         
-    def run(self, reload = False):
-  
+    def run(self, reload = False, path = None):
+        if path is not None:          
+            Path.base_path = path
+            logger.info('Project path ' + Path.base())
+            
         if reload == True:
             logger.info('Dev mode (reload)')
 
         uvicorn.run(
             'arikaim.core.app:app.boot', 
             reload = reload,
             factory = True,
```

### Comparing `arikaim-0.5.6/arikaim/core/service.py` & `arikaim-0.5.7/arikaim/core/service.py`

 * *Files identical despite different names*

### Comparing `arikaim-0.5.6/arikaim/core/utils.py` & `arikaim-0.5.7/arikaim/core/utils.py`

 * *Files identical despite different names*

### Comparing `arikaim-0.5.6/arikaim.egg-info/PKG-INFO` & `arikaim-0.5.7/arikaim.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arikaim
-Version: 0.5.6
+Version: 0.5.7
 Summary: Arikaim services server
 Home-page: https://github.com/arikaim/arikaim-services-server.git
 Download-URL: 
 Author: Intersoft Ltd
 Author-email: info@arikaim.com
 License: MIT License
 Keywords: arikaim
@@ -39,15 +39,19 @@
 ```
 
 #### Usage
 
 ##### Run
 
 ```sh
-    arikaim-server run
+
+arikaim-server run
+
 ```
 
 ##### Create config file
 
 ```sh
-    arikaim-server config create
+
+arikaim-server config create
+
 ```
```

### Comparing `arikaim-0.5.6/arikaim.egg-info/SOURCES.txt` & `arikaim-0.5.7/arikaim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arikaim-0.5.6/setup.py` & `arikaim-0.5.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     'arikaim.core.console.templates',
     'arikaim.core.db',
     'arikaim.core.queue',
     'arikaim.core.db.models'
 ],
    
 # Project version number:
-version = '0.5.6',
+version = '0.5.7',
 
 # List a license for the project, eg. MIT License
 license = 'MIT License',
 
 # Short description of your library: 
 description = 'Arikaim services server',
```

