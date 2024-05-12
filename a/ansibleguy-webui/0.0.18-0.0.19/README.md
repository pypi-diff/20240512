# Comparing `tmp/ansibleguy-webui-0.0.18.tar.gz` & `tmp/ansibleguy_webui-0.0.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansibleguy-webui-0.0.18.tar", last modified: Fri Mar 15 22:10:40 2024, max compression
+gzip compressed data, was "ansibleguy_webui-0.0.19.tar", last modified: Sun May 12 16:25:44 2024, max compression
```

## Comparing `ansibleguy-webui-0.0.18.tar` & `ansibleguy_webui-0.0.19.tar`

### file list

```diff
@@ -1,198 +1,211 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 22:10:40.881691 ansibleguy-webui-0.0.18/
--rw-r--r--   0 runner    (1001) docker     (127)    33252 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    43445 2024-03-15 22:10:40.881691 ansibleguy-webui-0.0.18/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3927 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-15 22:10:38.000000 ansibleguy-webui-0.0.18/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-15 22:10:40.881691 ansibleguy-webui-0.0.18/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 22:10:40.849691 ansibleguy-webui-0.0.18/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 22:10:40.853690 ansibleguy-webui-0.0.18/src/ansibleguy-webui/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      916 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 22:10:40.853690 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1998 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 22:10:40.857690 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/api_endpoints/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/api_endpoints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/api_endpoints/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    15684 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/api_endpoints/credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     5684 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/api_endpoints/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (127)    18479 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/api_endpoints/job.py
--rw-r--r--   0 runner    (1001) docker     (127)     4502 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/api_endpoints/job_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/api_endpoints/key.py
--rw-r--r--   0 runner    (1001) docker     (127)    15248 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/api_endpoints/permission.py
--rw-r--r--   0 runner    (1001) docker     (127)    13633 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/api_endpoints/repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     4047 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/api_endpoints/system.py
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 22:10:40.857690 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/config/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/config/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/config/environment.py
--rw-r--r--   0 runner    (1001) docker     (127)    10025 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/config/form_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/config/hardcoded.py
--rw-r--r--   0 runner    (1001) docker     (127)     2959 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/config/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/config/navigation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 22:10:40.861691 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/db_sqlite_patched/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/db_sqlite_patched/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/db_sqlite_patched/_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/db_sqlite_patched/base.py
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/db_sqlite_patched/client.py
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/db_sqlite_patched/creation.py
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/db_sqlite_patched/features.py
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/db_sqlite_patched/introspection.py
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/db_sqlite_patched/operations.py
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/db_sqlite_patched/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 22:10:40.861691 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/execute/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/execute/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/execute/play.py
--rw-r--r--   0 runner    (1001) docker     (127)     3784 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/execute/play_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     9808 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/execute/play_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/execute/queue.py
--rw-r--r--   0 runner    (1001) docker     (127)     9194 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/execute/repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     7500 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/execute/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     7068 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/execute/threader.py
--rw-r--r--   0 runner    (1001) docker     (127)     3424 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/execute/util.py
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 22:10:40.861691 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)    40135 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/migrations/0001_v0_0_12.py
--rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/migrations/0002_v0_0_13.py
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/migrations/0003_v0_0_14.py
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/migrations/0004_v0_0_15.py
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/migrations/0005_v0_0_18.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 22:10:40.865691 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/model/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/model/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    10063 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/model/job.py
--rw-r--r--   0 runner    (1001) docker     (127)     4867 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/model/job_credential.py
--rw-r--r--   0 runner    (1001) docker     (127)     5113 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/model/permission.py
--rw-r--r--   0 runner    (1001) docker     (127)     4201 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/model/repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     3038 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/model/system.py
--rw-r--r--   0 runner    (1001) docker     (127)     9414 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 22:10:40.849691 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 22:10:40.865691 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/static/css/
--rw-r--r--   0 runner    (1001) docker     (127)    12096 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/static/css/aw.css
--rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/static/css/aw_mobile.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 22:10:40.865691 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/static/img/
--rw-r--r--   0 runner    (1001) docker     (127)    14912 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/static/img/logo.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 22:10:40.865691 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/static/js/
--rw-r--r--   0 runner    (1001) docker     (127)    17894 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/static/js/aw.js
--rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/static/js/aw_nav.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 22:10:40.865691 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/static/js/jobs/
--rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/static/js/jobs/credentials.js
--rw-r--r--   0 runner    (1001) docker     (127)    11129 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/static/js/jobs/edit.js
--rw-r--r--   0 runner    (1001) docker     (127)     6945 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/static/js/jobs/logs.js
--rw-r--r--   0 runner    (1001) docker     (127)     3723 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/static/js/jobs/manage.js
--rw-r--r--   0 runner    (1001) docker     (127)     2310 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/static/js/jobs/repository.js
--rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/static/js/login.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 22:10:40.865691 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/static/js/settings/
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/static/js/settings/api_key.js
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/static/js/settings/environment.js
--rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/static/js/settings/permission.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 22:10:40.869691 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/templates/body.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 22:10:40.869691 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/templates/button/
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/templates/button/autoRefresh.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 22:10:40.869691 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/templates/button/icon/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/templates/button/icon/add.html
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/templates/button/icon/add_dir.html
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/templates/button/icon/add_git.html
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/templates/button/icon/collapse.html
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/templates/button/icon/copy.html
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/templates/button/icon/delete.html
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/templates/button/icon/download.html
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/templates/button/icon/edit.html
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/templates/button/icon/expand.html
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/templates/button/icon/return.html
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/templates/button/icon/run.html
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/templates/button/icon/sort.html
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/templates/button/icon/stop.html
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/templates/button/refresh.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 22:10:40.869691 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/templates/django_saml2_auth/
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/templates/django_saml2_auth/denied.html
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/templates/django_saml2_auth/error.html
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/templates/django_saml2_auth/signout.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 22:10:40.873690 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/templates/error/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/templates/error/403.html
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/templates/error/500.html
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/templates/error/js_disabled.html
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/templates/fallback.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 22:10:40.873690 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/templates/forms/
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/templates/forms/base.html
--rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/templates/forms/job.html
--rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/templates/forms/snippet.html
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/templates/forms/snippet_test.html
--rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/templates/head.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 22:10:40.873690 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/templates/jobs/
--rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/templates/jobs/credentials.html
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/templates/jobs/credentials_edit.html
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/templates/jobs/edit.html
--rw-r--r--   0 runner    (1001) docker     (127)     3288 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/templates/jobs/logs.html
--rw-r--r--   0 runner    (1001) docker     (127)     3807 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/templates/jobs/manage.html
--rw-r--r--   0 runner    (1001) docker     (127)     2726 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/templates/jobs/repository.html
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/templates/jobs/repository_edit.html
--rw-r--r--   0 runner    (1001) docker     (127)     5848 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/templates/nav.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 22:10:40.873690 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/templates/registration/
--rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/templates/registration/login.html
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/templates/registration/password_change_done.html
--rw-r--r--   0 runner    (1001) docker     (127)     2901 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/templates/registration/password_change_form.html
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/templates/registration/remember_user.html
--rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/templates/registration/saml.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 22:10:40.873690 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/templates/rest_framework/
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/templates/rest_framework/api.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 22:10:40.873690 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/templates/settings/
--rw-r--r--   0 runner    (1001) docker     (127)      969 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/templates/settings/api_key.html
--rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/templates/settings/permission.html
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/templates/settings/permission_edit.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 22:10:40.877691 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/templates/system/
--rw-r--r--   0 runner    (1001) docker     (127)      925 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/templates/system/config.html
--rw-r--r--   0 runner    (1001) docker     (127)     5422 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/templates/system/environment.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 22:10:40.877691 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/templatetags/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4963 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/templatetags/form_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3688 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/templatetags/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 22:10:40.877691 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/utils/crypto.py
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/utils/debug.py
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/utils/deployment.py
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/utils/handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/utils/http.py
--rw-r--r--   0 runner    (1001) docker     (127)     5061 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/utils/permission.py
--rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/utils/subps.py
--rw-r--r--   0 runner    (1001) docker     (127)     4094 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/utils/util.py
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/utils/util_no_config.py
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/utils/util_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3771 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/utils/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 22:10:40.881691 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/views/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/views/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 22:10:40.881691 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/views/forms/
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/views/forms/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     9162 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/views/forms/job.py
--rw-r--r--   0 runner    (1001) docker     (127)     3141 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/views/forms/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/views/forms/system.py
--rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/views/job.py
--rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/views/main.py
--rw-r--r--   0 runner    (1001) docker     (127)      889 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/views/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     4240 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/views/system.py
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/views/validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2514 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/cli_init.py
--rw-r--r--   0 runner    (1001) docker     (127)     6292 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/db.py
--rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/main.py
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/manage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/web_serve_static.py
--rw-r--r--   0 runner    (1001) docker     (127)     2430 2024-03-15 22:09:34.000000 ansibleguy-webui-0.0.18/src/ansibleguy-webui/webserver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 22:10:40.881691 ansibleguy-webui-0.0.18/src/ansibleguy_webui.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    43445 2024-03-15 22:10:40.000000 ansibleguy-webui-0.0.18/src/ansibleguy_webui.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7597 2024-03-15 22:10:40.000000 ansibleguy-webui-0.0.18/src/ansibleguy_webui.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-15 22:10:40.000000 ansibleguy-webui-0.0.18/src/ansibleguy_webui.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-03-15 22:10:40.000000 ansibleguy-webui-0.0.18/src/ansibleguy_webui.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-15 22:10:40.000000 ansibleguy-webui-0.0.18/src/ansibleguy_webui.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:25:44.280806 ansibleguy_webui-0.0.19/
+-rw-r--r--   0 runner    (1001) docker     (127)    33252 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    43911 2024-05-12 16:25:44.280806 ansibleguy_webui-0.0.19/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4393 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-12 16:25:42.000000 ansibleguy_webui-0.0.19/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 16:25:44.280806 ansibleguy_webui-0.0.19/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:25:44.248806 ansibleguy_webui-0.0.19/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:25:44.248806 ansibleguy_webui-0.0.19/src/ansibleguy-webui/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:25:44.252806 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:25:44.252806 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/api_endpoints/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/api_endpoints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21503 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/api_endpoints/alert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/api_endpoints/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14858 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/api_endpoints/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5684 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/api_endpoints/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18404 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/api_endpoints/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4451 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/api_endpoints/job_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/api_endpoints/key.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14257 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/api_endpoints/permission.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12670 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/api_endpoints/repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4618 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/api_endpoints/system.py
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:25:44.256806 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/config/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/config/environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13217 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/config/form_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/config/hardcoded.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2959 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/config/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/config/navigation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:25:44.256806 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/db_sqlite_patched/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/db_sqlite_patched/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/db_sqlite_patched/_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/db_sqlite_patched/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/db_sqlite_patched/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/db_sqlite_patched/creation.py
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/db_sqlite_patched/features.py
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/db_sqlite_patched/introspection.py
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/db_sqlite_patched/operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/db_sqlite_patched/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:25:44.256806 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/execute/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/execute/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3847 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/execute/alert.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:25:44.260806 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/execute/alert_plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/execute/alert_plugin/plugin_email.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4060 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/execute/alert_plugin/plugin_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/execute/play.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4177 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/execute/play_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9805 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/execute/play_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/execute/queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9194 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/execute/repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6256 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/execute/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7068 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/execute/threader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3424 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/execute/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:25:44.260806 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)    40135 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/migrations/0001_v0_0_12.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/migrations/0002_v0_0_13.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/migrations/0003_v0_0_14.py
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/migrations/0004_v0_0_15.py
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/migrations/0005_v0_0_18.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14987 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/migrations/0006_v0_0_19.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:25:44.260806 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5544 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/model/alert.py
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/model/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/model/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10455 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/model/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4821 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/model/job_credential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5113 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/model/permission.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4201 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/model/repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4938 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/model/system.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9789 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:25:44.244806 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:25:44.260806 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)    12096 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/static/css/aw.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/static/css/aw_mobile.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:25:44.260806 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/static/img/
+-rw-r--r--   0 runner    (1001) docker     (127)    14912 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/static/img/logo.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:25:44.264806 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)    17643 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/static/js/aw.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/static/js/aw_nav.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:25:44.264806 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/static/js/jobs/
+-rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/static/js/jobs/credentials.js
+-rw-r--r--   0 runner    (1001) docker     (127)    11129 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/static/js/jobs/edit.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6435 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/static/js/jobs/logs.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3722 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/static/js/jobs/manage.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2310 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/static/js/jobs/repository.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/static/js/login.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:25:44.264806 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/static/js/settings/
+-rw-r--r--   0 runner    (1001) docker     (127)     3296 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/static/js/settings/alert.js
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/static/js/settings/api_key.js
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/static/js/settings/environment.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/static/js/settings/permission.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:25:44.264806 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/body.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:25:44.264806 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/button/
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/button/autoRefresh.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:25:44.268806 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/button/icon/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/button/icon/add.html
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/button/icon/add_dir.html
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/button/icon/add_git.html
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/button/icon/collapse.html
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/button/icon/copy.html
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/button/icon/delete.html
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/button/icon/download.html
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/button/icon/edit.html
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/button/icon/expand.html
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/button/icon/return.html
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/button/icon/run.html
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/button/icon/sort.html
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/button/icon/stop.html
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/button/refresh.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:25:44.268806 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/django_saml2_auth/
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/django_saml2_auth/denied.html
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/django_saml2_auth/error.html
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/django_saml2_auth/signout.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:25:44.268806 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/email/
+-rw-r--r--   0 runner    (1001) docker     (127)     2961 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/email/alert.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:25:44.268806 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/error/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/error/403.html
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/error/500.html
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/error/js_disabled.html
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/fallback.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:25:44.268806 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/forms/
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/forms/base.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/forms/job.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/forms/snippet.html
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/forms/snippet_test.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/head.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:25:44.272806 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/jobs/
+-rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/jobs/credentials.html
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/jobs/credentials_edit.html
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/jobs/edit.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3288 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/jobs/logs.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3770 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/jobs/manage.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2726 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/jobs/repository.html
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/jobs/repository_edit.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5848 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/nav.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:25:44.272806 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/registration/
+-rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/registration/login.html
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/registration/password_change_done.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2901 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/registration/password_change_form.html
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/registration/remember_user.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/registration/saml.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:25:44.272806 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/rest_framework/
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/rest_framework/api.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:25:44.272806 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/settings/
+-rw-r--r--   0 runner    (1001) docker     (127)     5252 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/settings/alert.html
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/settings/alert_edit.html
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/settings/api_key.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/settings/permission.html
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/settings/permission_edit.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:25:44.272806 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/system/
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/system/config.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5422 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/system/environment.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:25:44.276806 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5327 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templatetags/form_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3980 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templatetags/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:25:44.276806 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/utils/crypto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/utils/debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/utils/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/utils/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/utils/http.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5061 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/utils/permission.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/utils/subps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6720 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/utils/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/utils/util_no_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/utils/util_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3771 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/utils/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:25:44.276806 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/views/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/views/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:25:44.280806 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/views/forms/
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/views/forms/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9126 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/views/forms/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9227 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/views/forms/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3007 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/views/forms/system.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/views/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/views/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/views/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4240 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/views/system.py
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/views/validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2514 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/cli_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6976 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/handle_signals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/manage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/web_serve_static.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2430 2024-05-12 16:24:36.000000 ansibleguy_webui-0.0.19/src/ansibleguy-webui/webserver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:25:44.280806 ansibleguy_webui-0.0.19/src/ansibleguy_webui.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    43911 2024-05-12 16:25:44.000000 ansibleguy_webui-0.0.19/src/ansibleguy_webui.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8154 2024-05-12 16:25:44.000000 ansibleguy_webui-0.0.19/src/ansibleguy_webui.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 16:25:44.000000 ansibleguy_webui-0.0.19/src/ansibleguy_webui.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-12 16:25:44.000000 ansibleguy_webui-0.0.19/src/ansibleguy_webui.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-12 16:25:44.000000 ansibleguy_webui-0.0.19/src/ansibleguy_webui.egg-info/top_level.txt
```

### Comparing `ansibleguy-webui-0.0.18/LICENSE.txt` & `ansibleguy_webui-0.0.19/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ansibleguy-webui-0.0.18/PKG-INFO` & `ansibleguy_webui-0.0.19/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansibleguy-webui
-Version: 0.0.18
+Version: 0.0.19
 Summary: Basic WebUI for using Ansible
 Author-email: AnsibleGuy <contact@ansibleguy.net>
 License:  GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -670,14 +670,16 @@
 Requires-Dist: crontab
 Requires-Dist: ansible-core
 Requires-Dist: ansible-runner
 Requires-Dist: PyYAML
 
 # Basic WebUI for using Ansible
 
+<a href='https://ko-fi.com/ansible0guy' target='_blank'><img height='35' style='border:0px;height:46px;' src='https://az743702.vo.msecnd.net/cdn/kofi3.png?v=0' border='0' alt='Buy me a coffee' />
+
 [![Documentation](https://readthedocs.org/projects/ansible-webui/badge/?version=latest)](https://webui.ansibleguy.net/en/latest/?badge=latest)
 [![Lint](https://github.com/ansibleguy/webui/actions/workflows/lint.yml/badge.svg?branch=latest)](https://github.com/ansibleguy/webui/actions/workflows/lint.yml)
 [![Test](https://github.com/ansibleguy/webui/actions/workflows/test.yml/badge.svg?branch=latest)](https://github.com/ansibleguy/webui/actions/workflows/test.yml)
 
 **DISCLAIMER**: This is an **unofficial community project**! Do not confuse it with the vanilla [Ansible](https://ansible.com/) product!
 
 The goal is to allow users to quickly install & run a WebUI for using Ansible locally.
@@ -762,27 +764,35 @@
 
   - [x] Execute Ansible using [ansible-runner](https://ansible.readthedocs.io/projects/runner/en/latest/python_interface/)
 
     - [x] Scheduled execution (Cron-Format)
 
     - [x] Manual/immediate execution
 
+    - [ ] Custom Execution-Forms
+
     - [ ] Support for [ad-hoc commands](https://docs.ansible.com/ansible/latest/command_guide/intro_adhoc.html)
 
+    - [ ] Support for [Process-Isolation](https://ansible.readthedocs.io/projects/runner/en/stable/standalone/#running-with-process-isolation)
+
   - [x] Job Logging
 
     - [x] Write job metadata to database
 
     - [x] Write full job-logs to Filesystem
 
   - [x] Secret handling (Connect, Become, Vault)
 
     - [x] User-specific job credentials
 
-  - [ ] Alerting on Failure
+  - [x] Alerting on Failure
+
+    - [x] E-Mail
+
+    - [x] Support for external Plugins (*simple Interface for Scripts*)
 
 - [ ] WebUI
 
   - [x] Job Dashboard
 
       Status, Execute, Time of last & next execution, Last run User, Links to Warnings/Errors
```

### Comparing `ansibleguy-webui-0.0.18/README.md` & `ansibleguy_webui-0.0.19/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,246 +1,275 @@
 00000000: 2320 4261 7369 6320 5765 6255 4920 666f  # Basic WebUI fo
 00000010: 7220 7573 696e 6720 416e 7369 626c 650a  r using Ansible.
-00000020: 0a5b 215b 446f 6375 6d65 6e74 6174 696f  .[![Documentatio
-00000030: 6e5d 2868 7474 7073 3a2f 2f72 6561 6474  n](https://readt
-00000040: 6865 646f 6373 2e6f 7267 2f70 726f 6a65  hedocs.org/proje
-00000050: 6374 732f 616e 7369 626c 652d 7765 6275  cts/ansible-webu
-00000060: 692f 6261 6467 652f 3f76 6572 7369 6f6e  i/badge/?version
-00000070: 3d6c 6174 6573 7429 5d28 6874 7470 733a  =latest)](https:
-00000080: 2f2f 7765 6275 692e 616e 7369 626c 6567  //webui.ansibleg
-00000090: 7579 2e6e 6574 2f65 6e2f 6c61 7465 7374  uy.net/en/latest
-000000a0: 2f3f 6261 6467 653d 6c61 7465 7374 290a  /?badge=latest).
-000000b0: 5b21 5b4c 696e 745d 2868 7474 7073 3a2f  [![Lint](https:/
-000000c0: 2f67 6974 6875 622e 636f 6d2f 616e 7369  /github.com/ansi
-000000d0: 626c 6567 7579 2f77 6562 7569 2f61 6374  bleguy/webui/act
-000000e0: 696f 6e73 2f77 6f72 6b66 6c6f 7773 2f6c  ions/workflows/l
-000000f0: 696e 742e 796d 6c2f 6261 6467 652e 7376  int.yml/badge.sv
-00000100: 673f 6272 616e 6368 3d6c 6174 6573 7429  g?branch=latest)
-00000110: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00000120: 2e63 6f6d 2f61 6e73 6962 6c65 6775 792f  .com/ansibleguy/
-00000130: 7765 6275 692f 6163 7469 6f6e 732f 776f  webui/actions/wo
-00000140: 726b 666c 6f77 732f 6c69 6e74 2e79 6d6c  rkflows/lint.yml
-00000150: 290a 5b21 5b54 6573 745d 2868 7474 7073  ).[![Test](https
-00000160: 3a2f 2f67 6974 6875 622e 636f 6d2f 616e  ://github.com/an
-00000170: 7369 626c 6567 7579 2f77 6562 7569 2f61  sibleguy/webui/a
-00000180: 6374 696f 6e73 2f77 6f72 6b66 6c6f 7773  ctions/workflows
-00000190: 2f74 6573 742e 796d 6c2f 6261 6467 652e  /test.yml/badge.
-000001a0: 7376 673f 6272 616e 6368 3d6c 6174 6573  svg?branch=lates
-000001b0: 7429 5d28 6874 7470 733a 2f2f 6769 7468  t)](https://gith
-000001c0: 7562 2e63 6f6d 2f61 6e73 6962 6c65 6775  ub.com/ansiblegu
-000001d0: 792f 7765 6275 692f 6163 7469 6f6e 732f  y/webui/actions/
-000001e0: 776f 726b 666c 6f77 732f 7465 7374 2e79  workflows/test.y
-000001f0: 6d6c 290a 0a2a 2a44 4953 434c 4149 4d45  ml)..**DISCLAIME
-00000200: 522a 2a3a 2054 6869 7320 6973 2061 6e20  R**: This is an 
-00000210: 2a2a 756e 6f66 6669 6369 616c 2063 6f6d  **unofficial com
-00000220: 6d75 6e69 7479 2070 726f 6a65 6374 2a2a  munity project**
-00000230: 2120 446f 206e 6f74 2063 6f6e 6675 7365  ! Do not confuse
-00000240: 2069 7420 7769 7468 2074 6865 2076 616e   it with the van
-00000250: 696c 6c61 205b 416e 7369 626c 655d 2868  illa [Ansible](h
-00000260: 7474 7073 3a2f 2f61 6e73 6962 6c65 2e63  ttps://ansible.c
-00000270: 6f6d 2f29 2070 726f 6475 6374 210a 0a54  om/) product!..T
-00000280: 6865 2067 6f61 6c20 6973 2074 6f20 616c  he goal is to al
-00000290: 6c6f 7720 7573 6572 7320 746f 2071 7569  low users to qui
-000002a0: 636b 6c79 2069 6e73 7461 6c6c 2026 2072  ckly install & r
-000002b0: 756e 2061 2057 6562 5549 2066 6f72 2075  un a WebUI for u
-000002c0: 7369 6e67 2041 6e73 6962 6c65 206c 6f63  sing Ansible loc
-000002d0: 616c 6c79 2e0a 0a4b 6565 7020 6974 2073  ally...Keep it s
-000002e0: 696d 706c 652e 0a0a 2a2a 5468 6973 2070  imple...**This p
-000002f0: 726f 6a65 6374 2069 7320 7374 696c 6c20  roject is still 
-00000300: 696e 2065 6172 6c79 2064 6576 656c 6f70  in early develop
-00000310: 6d65 6e74 2120 444f 204e 4f54 2055 5345  ment! DO NOT USE
-00000320: 2049 4e20 5052 4f44 5543 5449 4f4e 212a   IN PRODUCTION!*
-00000330: 2a0a 0a2d 2d2d 2d0a 0a23 2320 5365 7475  *..----..## Setu
-00000340: 700a 0a23 2323 204c 6f63 616c 202d 2050  p..### Local - P
-00000350: 4950 0a0a 5265 7175 6972 6573 2050 7974  IP..Requires Pyt
-00000360: 686f 6e20 3e3d 332e 3130 0a0a 6060 6062  hon >=3.10..```b
-00000370: 6173 680a 2320 696e 7374 616c 6c0a 7079  ash.# install.py
-00000380: 7468 6f6e 3320 2d6d 2070 6970 2069 6e73  thon3 -m pip ins
-00000390: 7461 6c6c 2061 6e73 6962 6c65 6775 792d  tall ansibleguy-
-000003a0: 7765 6275 690a 0a23 2072 756e 0a70 7974  webui..# run.pyt
-000003b0: 686f 6e33 202d 6d20 616e 7369 626c 6567  hon3 -m ansibleg
-000003c0: 7579 2d77 6562 7569 0a60 6060 0a0a 2323  uy-webui.```..##
-000003d0: 2320 446f 636b 6572 0a0a 496d 6167 6573  # Docker..Images
-000003e0: 3a20 5b77 6562 7569 5d28 6874 7470 733a  : [webui](https:
-000003f0: 2f2f 6875 622e 646f 636b 6572 2e63 6f6d  //hub.docker.com
-00000400: 2f72 2f61 6e73 6962 6c65 3067 7579 2f77  /r/ansible0guy/w
-00000410: 6562 7569 292c 205b 7765 6275 692d 756e  ebui), [webui-un
-00000420: 7072 6976 696c 6567 6564 5d28 6874 7470  privileged](http
-00000430: 733a 2f2f 6875 622e 646f 636b 6572 2e63  s://hub.docker.c
-00000440: 6f6d 2f72 2f61 6e73 6962 6c65 3067 7579  om/r/ansible0guy
-00000450: 2f77 6562 7569 2d75 6e70 7269 7669 6c65  /webui-unprivile
-00000460: 6765 6429 2c20 5b77 6562 7569 2d61 7773  ged), [webui-aws
-00000470: 5d28 6874 7470 733a 2f2f 6875 622e 646f  ](https://hub.do
-00000480: 636b 6572 2e63 6f6d 2f72 2f61 6e73 6962  cker.com/r/ansib
-00000490: 6c65 3067 7579 2f77 6562 7569 2d61 7773  le0guy/webui-aws
-000004a0: 290a 0a60 6060 6261 7368 0a64 6f63 6b65  )..```bash.docke
-000004b0: 7220 696d 6167 6520 7075 6c6c 2061 6e73  r image pull ans
-000004c0: 6962 6c65 3067 7579 2f77 6562 7569 3a6c  ible0guy/webui:l
-000004d0: 6174 6573 740a 646f 636b 6572 2072 756e  atest.docker run
-000004e0: 202d 6420 2d2d 6e61 6d65 2061 6e73 6962   -d --name ansib
-000004f0: 6c65 2d77 6562 7569 202d 2d70 7562 6c69  le-webui --publi
-00000500: 7368 2031 3237 2e30 2e30 2e31 3a38 3030  sh 127.0.0.1:800
-00000510: 303a 3830 3030 2061 6e73 6962 6c65 3067  0:8000 ansible0g
-00000520: 7579 2f77 6562 7569 3a6c 6174 6573 740a  uy/webui:latest.
-00000530: 0a23 206f 7220 7769 7468 2070 6572 7369  .# or with persi
-00000540: 7374 656e 7420 6461 7461 2028 766f 6c75  stent data (volu
-00000550: 6d65 733a 202f 6461 7461 203d 2073 746f  mes: /data = sto
-00000560: 7261 6765 2066 6f72 206c 6f67 7320 2620  rage for logs & 
-00000570: 4442 2c20 2f70 6c61 7920 3d20 616e 7369  DB, /play = ansi
-00000580: 626c 6520 706c 6179 626f 6f6b 2062 6173  ble playbook bas
-00000590: 652d 6469 7265 6374 6f72 7929 0a64 6f63  e-directory).doc
-000005a0: 6b65 7220 7275 6e20 2d64 202d 2d6e 616d  ker run -d --nam
-000005b0: 6520 616e 7369 626c 652d 7765 6275 6920  e ansible-webui 
-000005c0: 2d2d 7075 626c 6973 6820 3132 372e 302e  --publish 127.0.
-000005d0: 302e 313a 3830 3030 3a38 3030 3020 2d2d  0.1:8000:8000 --
-000005e0: 766f 6c75 6d65 2024 2870 7764 292f 616e  volume $(pwd)/an
-000005f0: 7369 626c 652f 6461 7461 3a2f 6461 7461  sible/data:/data
-00000600: 202d 2d76 6f6c 756d 6520 2428 7077 6429   --volume $(pwd)
-00000610: 2f61 6e73 6962 6c65 2f70 6c61 793a 2f70  /ansible/play:/p
-00000620: 6c61 7920 616e 7369 626c 6530 6775 792f  lay ansible0guy/
-00000630: 7765 6275 693a 6c61 7465 7374 0a60 6060  webui:latest.```
-00000640: 0a0a 2d2d 2d2d 0a0a 2323 2044 656d 6f0a  ..----..## Demo.
-00000650: 0a43 6865 636b 206f 7574 2074 6865 2064  .Check out the d
-00000660: 656d 6f20 6174 3a20 5b64 656d 6f2e 7765  emo at: [demo.we
-00000670: 6275 692e 616e 7369 626c 6567 7579 2e6e  bui.ansibleguy.n
-00000680: 6574 5d28 6874 7470 733a 2f2f 6465 6d6f  et](https://demo
-00000690: 2e77 6562 7569 2e61 6e73 6962 6c65 6775  .webui.ansiblegu
-000006a0: 792e 6e65 7429 0a0a 4c6f 6769 6e3a 2055  y.net)..Login: U
-000006b0: 7365 7220 6064 656d 6f60 2c20 5061 7373  ser `demo`, Pass
-000006c0: 776f 7264 2060 416e 7369 626c 6531 3333  word `Ansible133
-000006d0: 3760 0a0a 2d2d 2d2d 0a0a 2323 2055 7361  7`..----..## Usa
-000006e0: 6765 0a0a 5b44 6f63 756d 656e 7461 7469  ge..[Documentati
-000006f0: 6f6e 5d28 6874 7470 3a2f 2f77 6562 7569  on](http://webui
-00000700: 2e61 6e73 6962 6c65 6775 792e 6e65 742f  .ansibleguy.net/
-00000710: 290a 0a2d 2d2d 2d0a 0a23 2320 436f 6e74  )..----..## Cont
-00000720: 7269 6275 7465 0a0a 4665 656c 2066 7265  ribute..Feel fre
-00000730: 6520 746f 2063 6f6e 7472 6962 7574 6520  e to contribute 
-00000740: 746f 2074 6869 7320 7072 6f6a 6563 7420  to this project 
-00000750: 7573 696e 6720 5b70 756c 6c2d 7265 7175  using [pull-requ
-00000760: 6573 7473 5d28 6874 7470 733a 2f2f 6769  ests](https://gi
-00000770: 7468 7562 2e63 6f6d 2f61 6e73 6962 6c65  thub.com/ansible
-00000780: 6775 792f 7765 6275 692f 7075 6c6c 7329  guy/webui/pulls)
-00000790: 2c20 5b69 7373 7565 735d 2868 7474 7073  , [issues](https
-000007a0: 3a2f 2f67 6974 6875 622e 636f 6d2f 616e  ://github.com/an
-000007b0: 7369 626c 6567 7579 2f77 6562 7569 2f69  sibleguy/webui/i
-000007c0: 7373 7565 7329 2061 6e64 205b 6469 7363  ssues) and [disc
-000007d0: 7573 7369 6f6e 735d 2868 7474 7073 3a2f  ussions](https:/
-000007e0: 2f67 6974 6875 622e 636f 6d2f 616e 7369  /github.com/ansi
-000007f0: 626c 6567 7579 2f77 6562 7569 2f64 6973  bleguy/webui/dis
-00000800: 6375 7373 696f 6e73 2921 0a0a 5465 7374  cussions)!..Test
-00000810: 6572 7320 6172 6520 616c 736f 2076 6572  ers are also ver
-00000820: 7920 7765 6c63 6f6d 6521 2050 6c65 6173  y welcome! Pleas
-00000830: 6520 5b67 6976 6520 6665 6564 6261 636b  e [give feedback
-00000840: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00000850: 2e63 6f6d 2f61 6e73 6962 6c65 6775 792f  .com/ansibleguy/
-00000860: 7765 6275 692f 6469 7363 7573 7369 6f6e  webui/discussion
-00000870: 7329 0a0a 5365 6520 616c 736f 3a20 5b43  s)..See also: [C
-00000880: 6f6e 7472 6962 7574 696e 675d 2868 7474  ontributing](htt
-00000890: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-000008a0: 616e 7369 626c 6567 7579 2f77 6562 7569  ansibleguy/webui
-000008b0: 2f62 6c6f 622f 6c61 7465 7374 2f43 4f4e  /blob/latest/CON
-000008c0: 5452 4942 5554 452e 6d64 290a 0a2d 2d2d  TRIBUTE.md)..---
-000008d0: 2d0a 0a23 2320 526f 6164 6d61 700a 0a2d  -..## Roadmap..-
-000008e0: 205b 785d 2041 6e73 6962 6c65 2043 6f6e   [x] Ansible Con
-000008f0: 6669 670a 0a20 202d 205b 785d 2053 7461  fig..  - [x] Sta
-00000900: 7469 6320 506c 6179 626f 6f6b 2d44 6972  tic Playbook-Dir
-00000910: 6563 746f 7279 0a0a 2020 2d20 5b78 5d20  ectory..  - [x] 
-00000920: 4769 7420 5265 706f 7369 746f 7279 2073  Git Repository s
-00000930: 7570 706f 7274 0a0a 2d20 5b20 5d20 5573  upport..- [ ] Us
-00000940: 6572 730a 0a20 202d 205b 785d 204d 616e  ers..  - [x] Man
-00000950: 6167 656d 656e 7420 696e 7465 7266 6163  agement interfac
-00000960: 6520 2844 6a61 6e67 6f20 6275 696c 742d  e (Django built-
-00000970: 696e 290a 0a20 202d 205b 785d 2047 726f  in)..  - [x] Gro
-00000980: 7570 7320 2620 4a6f 6220 5065 726d 6973  ups & Job Permis
-00000990: 7369 6f6e 730a 0a20 202d 205b 205d 205b  sions..  - [ ] [
-000009a0: 4c44 4150 2069 6e74 6567 7261 7469 6f6e  LDAP integration
-000009b0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-000009c0: 2e63 6f6d 2f64 6a61 6e67 6f2d 6175 7468  .com/django-auth
-000009d0: 2d6c 6461 702f 646a 616e 676f 2d61 7574  -ldap/django-aut
-000009e0: 682d 6c64 6170 290a 0a20 202d 205b 785d  h-ldap)..  - [x]
-000009f0: 205b 5341 4d4c 2053 534f 2069 6e74 6567   [SAML SSO integ
-00000a00: 7261 7469 6f6e 5d28 6874 7470 733a 2f2f  ration](https://
-00000a10: 6769 7468 7562 2e63 6f6d 2f67 7261 6661  github.com/grafa
-00000a20: 6e61 2f64 6a61 6e67 6f2d 7361 6d6c 322d  na/django-saml2-
-00000a30: 6175 7468 290a 0a2d 205b 205d 204a 6f62  auth)..- [ ] Job
-00000a40: 730a 0a20 202d 205b 785d 2045 7865 6375  s..  - [x] Execu
-00000a50: 7465 2041 6e73 6962 6c65 2075 7369 6e67  te Ansible using
-00000a60: 205b 616e 7369 626c 652d 7275 6e6e 6572   [ansible-runner
-00000a70: 5d28 6874 7470 733a 2f2f 616e 7369 626c  ](https://ansibl
-00000a80: 652e 7265 6164 7468 6564 6f63 732e 696f  e.readthedocs.io
-00000a90: 2f70 726f 6a65 6374 732f 7275 6e6e 6572  /projects/runner
-00000aa0: 2f65 6e2f 6c61 7465 7374 2f70 7974 686f  /en/latest/pytho
-00000ab0: 6e5f 696e 7465 7266 6163 652f 290a 0a20  n_interface/).. 
-00000ac0: 2020 202d 205b 785d 2053 6368 6564 756c     - [x] Schedul
-00000ad0: 6564 2065 7865 6375 7469 6f6e 2028 4372  ed execution (Cr
-00000ae0: 6f6e 2d46 6f72 6d61 7429 0a0a 2020 2020  on-Format)..    
-00000af0: 2d20 5b78 5d20 4d61 6e75 616c 2f69 6d6d  - [x] Manual/imm
-00000b00: 6564 6961 7465 2065 7865 6375 7469 6f6e  ediate execution
-00000b10: 0a0a 2020 2020 2d20 5b20 5d20 5375 7070  ..    - [ ] Supp
-00000b20: 6f72 7420 666f 7220 5b61 642d 686f 6320  ort for [ad-hoc 
-00000b30: 636f 6d6d 616e 6473 5d28 6874 7470 733a  commands](https:
-00000b40: 2f2f 646f 6373 2e61 6e73 6962 6c65 2e63  //docs.ansible.c
-00000b50: 6f6d 2f61 6e73 6962 6c65 2f6c 6174 6573  om/ansible/lates
-00000b60: 742f 636f 6d6d 616e 645f 6775 6964 652f  t/command_guide/
-00000b70: 696e 7472 6f5f 6164 686f 632e 6874 6d6c  intro_adhoc.html
-00000b80: 290a 0a20 202d 205b 785d 204a 6f62 204c  )..  - [x] Job L
-00000b90: 6f67 6769 6e67 0a0a 2020 2020 2d20 5b78  ogging..    - [x
-00000ba0: 5d20 5772 6974 6520 6a6f 6220 6d65 7461  ] Write job meta
-00000bb0: 6461 7461 2074 6f20 6461 7461 6261 7365  data to database
-00000bc0: 0a0a 2020 2020 2d20 5b78 5d20 5772 6974  ..    - [x] Writ
-00000bd0: 6520 6675 6c6c 206a 6f62 2d6c 6f67 7320  e full job-logs 
-00000be0: 746f 2046 696c 6573 7973 7465 6d0a 0a20  to Filesystem.. 
-00000bf0: 202d 205b 785d 2053 6563 7265 7420 6861   - [x] Secret ha
-00000c00: 6e64 6c69 6e67 2028 436f 6e6e 6563 742c  ndling (Connect,
-00000c10: 2042 6563 6f6d 652c 2056 6175 6c74 290a   Become, Vault).
-00000c20: 0a20 2020 202d 205b 785d 2055 7365 722d  .    - [x] User-
-00000c30: 7370 6563 6966 6963 206a 6f62 2063 7265  specific job cre
-00000c40: 6465 6e74 6961 6c73 0a0a 2020 2d20 5b20  dentials..  - [ 
-00000c50: 5d20 416c 6572 7469 6e67 206f 6e20 4661  ] Alerting on Fa
-00000c60: 696c 7572 650a 0a2d 205b 205d 2057 6562  ilure..- [ ] Web
-00000c70: 5549 0a0a 2020 2d20 5b78 5d20 4a6f 6220  UI..  - [x] Job 
-00000c80: 4461 7368 626f 6172 640a 0a20 2020 2020  Dashboard..     
-00000c90: 2053 7461 7475 732c 2045 7865 6375 7465   Status, Execute
-00000ca0: 2c20 5469 6d65 206f 6620 6c61 7374 2026  , Time of last &
-00000cb0: 206e 6578 7420 6578 6563 7574 696f 6e2c   next execution,
-00000cc0: 204c 6173 7420 7275 6e20 5573 6572 2c20   Last run User, 
-00000cd0: 4c69 6e6b 7320 746f 2057 6172 6e69 6e67  Links to Warning
-00000ce0: 732f 4572 726f 7273 0a0a 2020 2d20 5b78  s/Errors..  - [x
-00000cf0: 5d20 4a6f 6220 4f75 7470 7574 0a0a 2020  ] Job Output..  
-00000d00: 2020 2020 466f 6c6c 6f77 2074 6865 206a      Follow the j
-00000d10: 6f62 7320 6f75 7470 7574 2069 6e20 7265  obs output in re
-00000d20: 616c 7469 6d65 0a0a 2020 2d20 5b20 5d20  altime..  - [ ] 
-00000d30: 4a6f 6220 4572 726f 7273 0a0a 2020 2020  Job Errors..    
-00000d40: 2020 5549 2074 6861 7420 616c 6c6f 7773    UI that allows
-00000d50: 2066 6f72 2065 6173 7920 6572 726f 7220   for easy error 
-00000d60: 616e 616c 7973 6973 2e20 4163 6365 7373  analysis. Access
-00000d70: 2074 6f20 6c6f 6773 2061 6e64 2070 726f   to logs and pro
-00000d80: 7669 6465 206c 696e 6b73 2074 6f20 706f  vide links to po
-00000d90: 7373 6962 6c65 2073 6f6c 7574 696f 6e73  ssible solutions
-00000da0: 0a0a 2020 2d20 5b78 5d20 5368 6f77 2041  ..  - [x] Show A
-00000db0: 6e73 6962 6c65 2052 756e 6e69 6e67 2d43  nsible Running-C
-00000dc0: 6f6e 6669 670a 0a20 202d 205b 785d 2053  onfig..  - [x] S
-00000dd0: 686f 7720 416e 7369 626c 6520 436f 6c6c  how Ansible Coll
-00000de0: 6563 7469 6f6e 730a 0a20 2020 202d 205b  ections..    - [
-00000df0: 205d 2043 6865 636b 2043 6f6c 6c65 6374   ] Check Collect
-00000e00: 696f 6e73 2066 6f72 2061 7661 696c 6162  ions for availab
-00000e10: 6c65 2075 7064 6174 6573 2028 4761 6c61  le updates (Gala
-00000e20: 7879 202b 2047 6974 4875 6220 7265 6c65  xy + GitHub rele
-00000e30: 6173 6573 290a 0a20 202d 205b 785d 204d  ases)..  - [x] M
-00000e40: 6f62 696c 6520 5375 7070 6f72 740a 0a20  obile Support.. 
-00000e50: 202d 205b 205d 204d 756c 7469 2d4c 616e   - [ ] Multi-Lan
-00000e60: 6775 6167 6520 5375 7070 6f72 740a 0a2d  guage Support..-
-00000e70: 205b 205d 2041 5049 0a0a 2020 2d20 5b78   [ ] API..  - [x
-00000e80: 5d20 4d61 6e61 6765 2061 6e64 2065 7865  ] Manage and exe
-00000e90: 6375 7465 204a 6f62 730a 0a2d 205b 205d  cute Jobs..- [ ]
-00000ea0: 2044 6174 6162 6173 650a 0a20 202d 205b   Database..  - [
-00000eb0: 205d 2053 7570 706f 7274 2066 6f72 204d   ] Support for M
-00000ec0: 7953 514c 0a0a 2d20 5b20 5d20 5465 7374  ySQL..- [ ] Test
-00000ed0: 696e 670a 0a20 202d 205b 205d 2055 6e69  ing..  - [ ] Uni
-00000ee0: 7420 5465 7374 730a 0a20 202d 205b 205d  t Tests..  - [ ]
-00000ef0: 2049 6e74 6567 7261 7469 6f6e 2054 6573   Integration Tes
-00000f00: 7473 0a0a 2020 2020 2d20 5b78 5d20 4261  ts..    - [x] Ba
-00000f10: 7369 6320 5765 6255 4920 6368 6563 6b73  sic WebUI checks
-00000f20: 0a0a 2020 2020 2d20 5b78 5d20 4150 4920  ..    - [x] API 
-00000f30: 456e 6470 6f69 6e74 730a 0a20 2020 202d  Endpoints..    -
-00000f40: 205b 205d 2050 6572 6d69 7373 696f 6e20   [ ] Permission 
-00000f50: 7379 7374 656d 0a                        system.
+00000020: 0a3c 6120 6872 6566 3d27 6874 7470 733a  .<a href='https:
+00000030: 2f2f 6b6f 2d66 692e 636f 6d2f 616e 7369  //ko-fi.com/ansi
+00000040: 626c 6530 6775 7927 2074 6172 6765 743d  ble0guy' target=
+00000050: 275f 626c 616e 6b27 3e3c 696d 6720 6865  '_blank'><img he
+00000060: 6967 6874 3d27 3335 2720 7374 796c 653d  ight='35' style=
+00000070: 2762 6f72 6465 723a 3070 783b 6865 6967  'border:0px;heig
+00000080: 6874 3a34 3670 783b 2720 7372 633d 2768  ht:46px;' src='h
+00000090: 7474 7073 3a2f 2f61 7a37 3433 3730 322e  ttps://az743702.
+000000a0: 766f 2e6d 7365 636e 642e 6e65 742f 6364  vo.msecnd.net/cd
+000000b0: 6e2f 6b6f 6669 332e 706e 673f 763d 3027  n/kofi3.png?v=0'
+000000c0: 2062 6f72 6465 723d 2730 2720 616c 743d   border='0' alt=
+000000d0: 2742 7579 206d 6520 6120 636f 6666 6565  'Buy me a coffee
+000000e0: 2720 2f3e 0a0a 5b21 5b44 6f63 756d 656e  ' />..[![Documen
+000000f0: 7461 7469 6f6e 5d28 6874 7470 733a 2f2f  tation](https://
+00000100: 7265 6164 7468 6564 6f63 732e 6f72 672f  readthedocs.org/
+00000110: 7072 6f6a 6563 7473 2f61 6e73 6962 6c65  projects/ansible
+00000120: 2d77 6562 7569 2f62 6164 6765 2f3f 7665  -webui/badge/?ve
+00000130: 7273 696f 6e3d 6c61 7465 7374 295d 2868  rsion=latest)](h
+00000140: 7474 7073 3a2f 2f77 6562 7569 2e61 6e73  ttps://webui.ans
+00000150: 6962 6c65 6775 792e 6e65 742f 656e 2f6c  ibleguy.net/en/l
+00000160: 6174 6573 742f 3f62 6164 6765 3d6c 6174  atest/?badge=lat
+00000170: 6573 7429 0a5b 215b 4c69 6e74 5d28 6874  est).[![Lint](ht
+00000180: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000190: 2f61 6e73 6962 6c65 6775 792f 7765 6275  /ansibleguy/webu
+000001a0: 692f 6163 7469 6f6e 732f 776f 726b 666c  i/actions/workfl
+000001b0: 6f77 732f 6c69 6e74 2e79 6d6c 2f62 6164  ows/lint.yml/bad
+000001c0: 6765 2e73 7667 3f62 7261 6e63 683d 6c61  ge.svg?branch=la
+000001d0: 7465 7374 295d 2868 7474 7073 3a2f 2f67  test)](https://g
+000001e0: 6974 6875 622e 636f 6d2f 616e 7369 626c  ithub.com/ansibl
+000001f0: 6567 7579 2f77 6562 7569 2f61 6374 696f  eguy/webui/actio
+00000200: 6e73 2f77 6f72 6b66 6c6f 7773 2f6c 696e  ns/workflows/lin
+00000210: 742e 796d 6c29 0a5b 215b 5465 7374 5d28  t.yml).[![Test](
+00000220: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000230: 6f6d 2f61 6e73 6962 6c65 6775 792f 7765  om/ansibleguy/we
+00000240: 6275 692f 6163 7469 6f6e 732f 776f 726b  bui/actions/work
+00000250: 666c 6f77 732f 7465 7374 2e79 6d6c 2f62  flows/test.yml/b
+00000260: 6164 6765 2e73 7667 3f62 7261 6e63 683d  adge.svg?branch=
+00000270: 6c61 7465 7374 295d 2868 7474 7073 3a2f  latest)](https:/
+00000280: 2f67 6974 6875 622e 636f 6d2f 616e 7369  /github.com/ansi
+00000290: 626c 6567 7579 2f77 6562 7569 2f61 6374  bleguy/webui/act
+000002a0: 696f 6e73 2f77 6f72 6b66 6c6f 7773 2f74  ions/workflows/t
+000002b0: 6573 742e 796d 6c29 0a0a 2a2a 4449 5343  est.yml)..**DISC
+000002c0: 4c41 494d 4552 2a2a 3a20 5468 6973 2069  LAIMER**: This i
+000002d0: 7320 616e 202a 2a75 6e6f 6666 6963 6961  s an **unofficia
+000002e0: 6c20 636f 6d6d 756e 6974 7920 7072 6f6a  l community proj
+000002f0: 6563 742a 2a21 2044 6f20 6e6f 7420 636f  ect**! Do not co
+00000300: 6e66 7573 6520 6974 2077 6974 6820 7468  nfuse it with th
+00000310: 6520 7661 6e69 6c6c 6120 5b41 6e73 6962  e vanilla [Ansib
+00000320: 6c65 5d28 6874 7470 733a 2f2f 616e 7369  le](https://ansi
+00000330: 626c 652e 636f 6d2f 2920 7072 6f64 7563  ble.com/) produc
+00000340: 7421 0a0a 5468 6520 676f 616c 2069 7320  t!..The goal is 
+00000350: 746f 2061 6c6c 6f77 2075 7365 7273 2074  to allow users t
+00000360: 6f20 7175 6963 6b6c 7920 696e 7374 616c  o quickly instal
+00000370: 6c20 2620 7275 6e20 6120 5765 6255 4920  l & run a WebUI 
+00000380: 666f 7220 7573 696e 6720 416e 7369 626c  for using Ansibl
+00000390: 6520 6c6f 6361 6c6c 792e 0a0a 4b65 6570  e locally...Keep
+000003a0: 2069 7420 7369 6d70 6c65 2e0a 0a2a 2a54   it simple...**T
+000003b0: 6869 7320 7072 6f6a 6563 7420 6973 2073  his project is s
+000003c0: 7469 6c6c 2069 6e20 6561 726c 7920 6465  till in early de
+000003d0: 7665 6c6f 706d 656e 7421 2044 4f20 4e4f  velopment! DO NO
+000003e0: 5420 5553 4520 494e 2050 524f 4455 4354  T USE IN PRODUCT
+000003f0: 494f 4e21 2a2a 0a0a 2d2d 2d2d 0a0a 2323  ION!**..----..##
+00000400: 2053 6574 7570 0a0a 2323 2320 4c6f 6361   Setup..### Loca
+00000410: 6c20 2d20 5049 500a 0a52 6571 7569 7265  l - PIP..Require
+00000420: 7320 5079 7468 6f6e 203e 3d33 2e31 300a  s Python >=3.10.
+00000430: 0a60 6060 6261 7368 0a23 2069 6e73 7461  .```bash.# insta
+00000440: 6c6c 0a70 7974 686f 6e33 202d 6d20 7069  ll.python3 -m pi
+00000450: 7020 696e 7374 616c 6c20 616e 7369 626c  p install ansibl
+00000460: 6567 7579 2d77 6562 7569 0a0a 2320 7275  eguy-webui..# ru
+00000470: 6e0a 7079 7468 6f6e 3320 2d6d 2061 6e73  n.python3 -m ans
+00000480: 6962 6c65 6775 792d 7765 6275 690a 6060  ibleguy-webui.``
+00000490: 600a 0a23 2323 2044 6f63 6b65 720a 0a49  `..### Docker..I
+000004a0: 6d61 6765 733a 205b 7765 6275 695d 2868  mages: [webui](h
+000004b0: 7474 7073 3a2f 2f68 7562 2e64 6f63 6b65  ttps://hub.docke
+000004c0: 722e 636f 6d2f 722f 616e 7369 626c 6530  r.com/r/ansible0
+000004d0: 6775 792f 7765 6275 6929 2c20 5b77 6562  guy/webui), [web
+000004e0: 7569 2d75 6e70 7269 7669 6c65 6765 645d  ui-unprivileged]
+000004f0: 2868 7474 7073 3a2f 2f68 7562 2e64 6f63  (https://hub.doc
+00000500: 6b65 722e 636f 6d2f 722f 616e 7369 626c  ker.com/r/ansibl
+00000510: 6530 6775 792f 7765 6275 692d 756e 7072  e0guy/webui-unpr
+00000520: 6976 696c 6567 6564 292c 205b 7765 6275  ivileged), [webu
+00000530: 692d 6177 735d 2868 7474 7073 3a2f 2f68  i-aws](https://h
+00000540: 7562 2e64 6f63 6b65 722e 636f 6d2f 722f  ub.docker.com/r/
+00000550: 616e 7369 626c 6530 6775 792f 7765 6275  ansible0guy/webu
+00000560: 692d 6177 7329 0a0a 6060 6062 6173 680a  i-aws)..```bash.
+00000570: 646f 636b 6572 2069 6d61 6765 2070 756c  docker image pul
+00000580: 6c20 616e 7369 626c 6530 6775 792f 7765  l ansible0guy/we
+00000590: 6275 693a 6c61 7465 7374 0a64 6f63 6b65  bui:latest.docke
+000005a0: 7220 7275 6e20 2d64 202d 2d6e 616d 6520  r run -d --name 
+000005b0: 616e 7369 626c 652d 7765 6275 6920 2d2d  ansible-webui --
+000005c0: 7075 626c 6973 6820 3132 372e 302e 302e  publish 127.0.0.
+000005d0: 313a 3830 3030 3a38 3030 3020 616e 7369  1:8000:8000 ansi
+000005e0: 626c 6530 6775 792f 7765 6275 693a 6c61  ble0guy/webui:la
+000005f0: 7465 7374 0a0a 2320 6f72 2077 6974 6820  test..# or with 
+00000600: 7065 7273 6973 7465 6e74 2064 6174 6120  persistent data 
+00000610: 2876 6f6c 756d 6573 3a20 2f64 6174 6120  (volumes: /data 
+00000620: 3d20 7374 6f72 6167 6520 666f 7220 6c6f  = storage for lo
+00000630: 6773 2026 2044 422c 202f 706c 6179 203d  gs & DB, /play =
+00000640: 2061 6e73 6962 6c65 2070 6c61 7962 6f6f   ansible playboo
+00000650: 6b20 6261 7365 2d64 6972 6563 746f 7279  k base-directory
+00000660: 290a 646f 636b 6572 2072 756e 202d 6420  ).docker run -d 
+00000670: 2d2d 6e61 6d65 2061 6e73 6962 6c65 2d77  --name ansible-w
+00000680: 6562 7569 202d 2d70 7562 6c69 7368 2031  ebui --publish 1
+00000690: 3237 2e30 2e30 2e31 3a38 3030 303a 3830  27.0.0.1:8000:80
+000006a0: 3030 202d 2d76 6f6c 756d 6520 2428 7077  00 --volume $(pw
+000006b0: 6429 2f61 6e73 6962 6c65 2f64 6174 613a  d)/ansible/data:
+000006c0: 2f64 6174 6120 2d2d 766f 6c75 6d65 2024  /data --volume $
+000006d0: 2870 7764 292f 616e 7369 626c 652f 706c  (pwd)/ansible/pl
+000006e0: 6179 3a2f 706c 6179 2061 6e73 6962 6c65  ay:/play ansible
+000006f0: 3067 7579 2f77 6562 7569 3a6c 6174 6573  0guy/webui:lates
+00000700: 740a 6060 600a 0a2d 2d2d 2d0a 0a23 2320  t.```..----..## 
+00000710: 4465 6d6f 0a0a 4368 6563 6b20 6f75 7420  Demo..Check out 
+00000720: 7468 6520 6465 6d6f 2061 743a 205b 6465  the demo at: [de
+00000730: 6d6f 2e77 6562 7569 2e61 6e73 6962 6c65  mo.webui.ansible
+00000740: 6775 792e 6e65 745d 2868 7474 7073 3a2f  guy.net](https:/
+00000750: 2f64 656d 6f2e 7765 6275 692e 616e 7369  /demo.webui.ansi
+00000760: 626c 6567 7579 2e6e 6574 290a 0a4c 6f67  bleguy.net)..Log
+00000770: 696e 3a20 5573 6572 2060 6465 6d6f 602c  in: User `demo`,
+00000780: 2050 6173 7377 6f72 6420 6041 6e73 6962   Password `Ansib
+00000790: 6c65 3133 3337 600a 0a2d 2d2d 2d0a 0a23  le1337`..----..#
+000007a0: 2320 5573 6167 650a 0a5b 446f 6375 6d65  # Usage..[Docume
+000007b0: 6e74 6174 696f 6e5d 2868 7474 703a 2f2f  ntation](http://
+000007c0: 7765 6275 692e 616e 7369 626c 6567 7579  webui.ansibleguy
+000007d0: 2e6e 6574 2f29 0a0a 2d2d 2d2d 0a0a 2323  .net/)..----..##
+000007e0: 2043 6f6e 7472 6962 7574 650a 0a46 6565   Contribute..Fee
+000007f0: 6c20 6672 6565 2074 6f20 636f 6e74 7269  l free to contri
+00000800: 6275 7465 2074 6f20 7468 6973 2070 726f  bute to this pro
+00000810: 6a65 6374 2075 7369 6e67 205b 7075 6c6c  ject using [pull
+00000820: 2d72 6571 7565 7374 735d 2868 7474 7073  -requests](https
+00000830: 3a2f 2f67 6974 6875 622e 636f 6d2f 616e  ://github.com/an
+00000840: 7369 626c 6567 7579 2f77 6562 7569 2f70  sibleguy/webui/p
+00000850: 756c 6c73 292c 205b 6973 7375 6573 5d28  ulls), [issues](
+00000860: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000870: 6f6d 2f61 6e73 6962 6c65 6775 792f 7765  om/ansibleguy/we
+00000880: 6275 692f 6973 7375 6573 2920 616e 6420  bui/issues) and 
+00000890: 5b64 6973 6375 7373 696f 6e73 5d28 6874  [discussions](ht
+000008a0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+000008b0: 2f61 6e73 6962 6c65 6775 792f 7765 6275  /ansibleguy/webu
+000008c0: 692f 6469 7363 7573 7369 6f6e 7329 210a  i/discussions)!.
+000008d0: 0a54 6573 7465 7273 2061 7265 2061 6c73  .Testers are als
+000008e0: 6f20 7665 7279 2077 656c 636f 6d65 2120  o very welcome! 
+000008f0: 506c 6561 7365 205b 6769 7665 2066 6565  Please [give fee
+00000900: 6462 6163 6b5d 2868 7474 7073 3a2f 2f67  dback](https://g
+00000910: 6974 6875 622e 636f 6d2f 616e 7369 626c  ithub.com/ansibl
+00000920: 6567 7579 2f77 6562 7569 2f64 6973 6375  eguy/webui/discu
+00000930: 7373 696f 6e73 290a 0a53 6565 2061 6c73  ssions)..See als
+00000940: 6f3a 205b 436f 6e74 7269 6275 7469 6e67  o: [Contributing
+00000950: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00000960: 2e63 6f6d 2f61 6e73 6962 6c65 6775 792f  .com/ansibleguy/
+00000970: 7765 6275 692f 626c 6f62 2f6c 6174 6573  webui/blob/lates
+00000980: 742f 434f 4e54 5249 4255 5445 2e6d 6429  t/CONTRIBUTE.md)
+00000990: 0a0a 2d2d 2d2d 0a0a 2323 2052 6f61 646d  ..----..## Roadm
+000009a0: 6170 0a0a 2d20 5b78 5d20 416e 7369 626c  ap..- [x] Ansibl
+000009b0: 6520 436f 6e66 6967 0a0a 2020 2d20 5b78  e Config..  - [x
+000009c0: 5d20 5374 6174 6963 2050 6c61 7962 6f6f  ] Static Playboo
+000009d0: 6b2d 4469 7265 6374 6f72 790a 0a20 202d  k-Directory..  -
+000009e0: 205b 785d 2047 6974 2052 6570 6f73 6974   [x] Git Reposit
+000009f0: 6f72 7920 7375 7070 6f72 740a 0a2d 205b  ory support..- [
+00000a00: 205d 2055 7365 7273 0a0a 2020 2d20 5b78   ] Users..  - [x
+00000a10: 5d20 4d61 6e61 6765 6d65 6e74 2069 6e74  ] Management int
+00000a20: 6572 6661 6365 2028 446a 616e 676f 2062  erface (Django b
+00000a30: 7569 6c74 2d69 6e29 0a0a 2020 2d20 5b78  uilt-in)..  - [x
+00000a40: 5d20 4772 6f75 7073 2026 204a 6f62 2050  ] Groups & Job P
+00000a50: 6572 6d69 7373 696f 6e73 0a0a 2020 2d20  ermissions..  - 
+00000a60: 5b20 5d20 5b4c 4441 5020 696e 7465 6772  [ ] [LDAP integr
+00000a70: 6174 696f 6e5d 2868 7474 7073 3a2f 2f67  ation](https://g
+00000a80: 6974 6875 622e 636f 6d2f 646a 616e 676f  ithub.com/django
+00000a90: 2d61 7574 682d 6c64 6170 2f64 6a61 6e67  -auth-ldap/djang
+00000aa0: 6f2d 6175 7468 2d6c 6461 7029 0a0a 2020  o-auth-ldap)..  
+00000ab0: 2d20 5b78 5d20 5b53 414d 4c20 5353 4f20  - [x] [SAML SSO 
+00000ac0: 696e 7465 6772 6174 696f 6e5d 2868 7474  integration](htt
+00000ad0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000ae0: 6772 6166 616e 612f 646a 616e 676f 2d73  grafana/django-s
+00000af0: 616d 6c32 2d61 7574 6829 0a0a 2d20 5b20  aml2-auth)..- [ 
+00000b00: 5d20 4a6f 6273 0a0a 2020 2d20 5b78 5d20  ] Jobs..  - [x] 
+00000b10: 4578 6563 7574 6520 416e 7369 626c 6520  Execute Ansible 
+00000b20: 7573 696e 6720 5b61 6e73 6962 6c65 2d72  using [ansible-r
+00000b30: 756e 6e65 725d 2868 7474 7073 3a2f 2f61  unner](https://a
+00000b40: 6e73 6962 6c65 2e72 6561 6474 6865 646f  nsible.readthedo
+00000b50: 6373 2e69 6f2f 7072 6f6a 6563 7473 2f72  cs.io/projects/r
+00000b60: 756e 6e65 722f 656e 2f6c 6174 6573 742f  unner/en/latest/
+00000b70: 7079 7468 6f6e 5f69 6e74 6572 6661 6365  python_interface
+00000b80: 2f29 0a0a 2020 2020 2d20 5b78 5d20 5363  /)..    - [x] Sc
+00000b90: 6865 6475 6c65 6420 6578 6563 7574 696f  heduled executio
+00000ba0: 6e20 2843 726f 6e2d 466f 726d 6174 290a  n (Cron-Format).
+00000bb0: 0a20 2020 202d 205b 785d 204d 616e 7561  .    - [x] Manua
+00000bc0: 6c2f 696d 6d65 6469 6174 6520 6578 6563  l/immediate exec
+00000bd0: 7574 696f 6e0a 0a20 2020 202d 205b 205d  ution..    - [ ]
+00000be0: 2043 7573 746f 6d20 4578 6563 7574 696f   Custom Executio
+00000bf0: 6e2d 466f 726d 730a 0a20 2020 202d 205b  n-Forms..    - [
+00000c00: 205d 2053 7570 706f 7274 2066 6f72 205b   ] Support for [
+00000c10: 6164 2d68 6f63 2063 6f6d 6d61 6e64 735d  ad-hoc commands]
+00000c20: 2868 7474 7073 3a2f 2f64 6f63 732e 616e  (https://docs.an
+00000c30: 7369 626c 652e 636f 6d2f 616e 7369 626c  sible.com/ansibl
+00000c40: 652f 6c61 7465 7374 2f63 6f6d 6d61 6e64  e/latest/command
+00000c50: 5f67 7569 6465 2f69 6e74 726f 5f61 6468  _guide/intro_adh
+00000c60: 6f63 2e68 746d 6c29 0a0a 2020 2020 2d20  oc.html)..    - 
+00000c70: 5b20 5d20 5375 7070 6f72 7420 666f 7220  [ ] Support for 
+00000c80: 5b50 726f 6365 7373 2d49 736f 6c61 7469  [Process-Isolati
+00000c90: 6f6e 5d28 6874 7470 733a 2f2f 616e 7369  on](https://ansi
+00000ca0: 626c 652e 7265 6164 7468 6564 6f63 732e  ble.readthedocs.
+00000cb0: 696f 2f70 726f 6a65 6374 732f 7275 6e6e  io/projects/runn
+00000cc0: 6572 2f65 6e2f 7374 6162 6c65 2f73 7461  er/en/stable/sta
+00000cd0: 6e64 616c 6f6e 652f 2372 756e 6e69 6e67  ndalone/#running
+00000ce0: 2d77 6974 682d 7072 6f63 6573 732d 6973  -with-process-is
+00000cf0: 6f6c 6174 696f 6e29 0a0a 2020 2d20 5b78  olation)..  - [x
+00000d00: 5d20 4a6f 6220 4c6f 6767 696e 670a 0a20  ] Job Logging.. 
+00000d10: 2020 202d 205b 785d 2057 7269 7465 206a     - [x] Write j
+00000d20: 6f62 206d 6574 6164 6174 6120 746f 2064  ob metadata to d
+00000d30: 6174 6162 6173 650a 0a20 2020 202d 205b  atabase..    - [
+00000d40: 785d 2057 7269 7465 2066 756c 6c20 6a6f  x] Write full jo
+00000d50: 622d 6c6f 6773 2074 6f20 4669 6c65 7379  b-logs to Filesy
+00000d60: 7374 656d 0a0a 2020 2d20 5b78 5d20 5365  stem..  - [x] Se
+00000d70: 6372 6574 2068 616e 646c 696e 6720 2843  cret handling (C
+00000d80: 6f6e 6e65 6374 2c20 4265 636f 6d65 2c20  onnect, Become, 
+00000d90: 5661 756c 7429 0a0a 2020 2020 2d20 5b78  Vault)..    - [x
+00000da0: 5d20 5573 6572 2d73 7065 6369 6669 6320  ] User-specific 
+00000db0: 6a6f 6220 6372 6564 656e 7469 616c 730a  job credentials.
+00000dc0: 0a20 202d 205b 785d 2041 6c65 7274 696e  .  - [x] Alertin
+00000dd0: 6720 6f6e 2046 6169 6c75 7265 0a0a 2020  g on Failure..  
+00000de0: 2020 2d20 5b78 5d20 452d 4d61 696c 0a0a    - [x] E-Mail..
+00000df0: 2020 2020 2d20 5b78 5d20 5375 7070 6f72      - [x] Suppor
+00000e00: 7420 666f 7220 6578 7465 726e 616c 2050  t for external P
+00000e10: 6c75 6769 6e73 2028 2a73 696d 706c 6520  lugins (*simple 
+00000e20: 496e 7465 7266 6163 6520 666f 7220 5363  Interface for Sc
+00000e30: 7269 7074 732a 290a 0a2d 205b 205d 2057  ripts*)..- [ ] W
+00000e40: 6562 5549 0a0a 2020 2d20 5b78 5d20 4a6f  ebUI..  - [x] Jo
+00000e50: 6220 4461 7368 626f 6172 640a 0a20 2020  b Dashboard..   
+00000e60: 2020 2053 7461 7475 732c 2045 7865 6375     Status, Execu
+00000e70: 7465 2c20 5469 6d65 206f 6620 6c61 7374  te, Time of last
+00000e80: 2026 206e 6578 7420 6578 6563 7574 696f   & next executio
+00000e90: 6e2c 204c 6173 7420 7275 6e20 5573 6572  n, Last run User
+00000ea0: 2c20 4c69 6e6b 7320 746f 2057 6172 6e69  , Links to Warni
+00000eb0: 6e67 732f 4572 726f 7273 0a0a 2020 2d20  ngs/Errors..  - 
+00000ec0: 5b78 5d20 4a6f 6220 4f75 7470 7574 0a0a  [x] Job Output..
+00000ed0: 2020 2020 2020 466f 6c6c 6f77 2074 6865        Follow the
+00000ee0: 206a 6f62 7320 6f75 7470 7574 2069 6e20   jobs output in 
+00000ef0: 7265 616c 7469 6d65 0a0a 2020 2d20 5b20  realtime..  - [ 
+00000f00: 5d20 4a6f 6220 4572 726f 7273 0a0a 2020  ] Job Errors..  
+00000f10: 2020 2020 5549 2074 6861 7420 616c 6c6f      UI that allo
+00000f20: 7773 2066 6f72 2065 6173 7920 6572 726f  ws for easy erro
+00000f30: 7220 616e 616c 7973 6973 2e20 4163 6365  r analysis. Acce
+00000f40: 7373 2074 6f20 6c6f 6773 2061 6e64 2070  ss to logs and p
+00000f50: 726f 7669 6465 206c 696e 6b73 2074 6f20  rovide links to 
+00000f60: 706f 7373 6962 6c65 2073 6f6c 7574 696f  possible solutio
+00000f70: 6e73 0a0a 2020 2d20 5b78 5d20 5368 6f77  ns..  - [x] Show
+00000f80: 2041 6e73 6962 6c65 2052 756e 6e69 6e67   Ansible Running
+00000f90: 2d43 6f6e 6669 670a 0a20 202d 205b 785d  -Config..  - [x]
+00000fa0: 2053 686f 7720 416e 7369 626c 6520 436f   Show Ansible Co
+00000fb0: 6c6c 6563 7469 6f6e 730a 0a20 2020 202d  llections..    -
+00000fc0: 205b 205d 2043 6865 636b 2043 6f6c 6c65   [ ] Check Colle
+00000fd0: 6374 696f 6e73 2066 6f72 2061 7661 696c  ctions for avail
+00000fe0: 6162 6c65 2075 7064 6174 6573 2028 4761  able updates (Ga
+00000ff0: 6c61 7879 202b 2047 6974 4875 6220 7265  laxy + GitHub re
+00001000: 6c65 6173 6573 290a 0a20 202d 205b 785d  leases)..  - [x]
+00001010: 204d 6f62 696c 6520 5375 7070 6f72 740a   Mobile Support.
+00001020: 0a20 202d 205b 205d 204d 756c 7469 2d4c  .  - [ ] Multi-L
+00001030: 616e 6775 6167 6520 5375 7070 6f72 740a  anguage Support.
+00001040: 0a2d 205b 205d 2041 5049 0a0a 2020 2d20  .- [ ] API..  - 
+00001050: 5b78 5d20 4d61 6e61 6765 2061 6e64 2065  [x] Manage and e
+00001060: 7865 6375 7465 204a 6f62 730a 0a2d 205b  xecute Jobs..- [
+00001070: 205d 2044 6174 6162 6173 650a 0a20 202d   ] Database..  -
+00001080: 205b 205d 2053 7570 706f 7274 2066 6f72   [ ] Support for
+00001090: 204d 7953 514c 0a0a 2d20 5b20 5d20 5465   MySQL..- [ ] Te
+000010a0: 7374 696e 670a 0a20 202d 205b 205d 2055  sting..  - [ ] U
+000010b0: 6e69 7420 5465 7374 730a 0a20 202d 205b  nit Tests..  - [
+000010c0: 205d 2049 6e74 6567 7261 7469 6f6e 2054   ] Integration T
+000010d0: 6573 7473 0a0a 2020 2020 2d20 5b78 5d20  ests..    - [x] 
+000010e0: 4261 7369 6320 5765 6255 4920 6368 6563  Basic WebUI chec
+000010f0: 6b73 0a0a 2020 2020 2d20 5b78 5d20 4150  ks..    - [x] AP
+00001100: 4920 456e 6470 6f69 6e74 730a 0a20 2020  I Endpoints..   
+00001110: 202d 205b 205d 2050 6572 6d69 7373 696f   - [ ] Permissio
+00001120: 6e20 7379 7374 656d 0a                   n system.
```

### Comparing `ansibleguy-webui-0.0.18/pyproject.toml` & `ansibleguy_webui-0.0.19/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ansibleguy-webui-0.0.18/src/ansibleguy-webui/__main__.py` & `ansibleguy_webui-0.0.19/src/ansibleguy-webui/__main__.py`

 * *Files identical despite different names*

### Comparing `ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/api.py` & `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/api.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,14 +5,17 @@
 from aw.api_endpoints.job import APIJob, APIJobItem, APIJobExecutionItem, APIJobExecutionLogs, \
     APIJobExecutionLogFile, APIJobExecution
 from aw.api_endpoints.permission import APIPermission, APIPermissionItem
 from aw.api_endpoints.credentials import APIJobCredentials, APIJobCredentialsItem
 from aw.api_endpoints.filesystem import APIFsBrowse, APIFsExists
 from aw.api_endpoints.system import APISystemConfig
 from aw.api_endpoints.repository import APIRepository, APIRepositoryItem, APIRepositoryLogFile
+from aw.api_endpoints.alert import APIAlertPlugin, APIAlertPluginItem, APIAlertUser, APIAlertUserItem, \
+    APIAlertGlobal, APIAlertGlobalItem, APIAlertGroup, APIAlertGroupItem
+# from aw.api_endpoints.base import not_implemented
 
 urlpatterns_api = [
     path('api/key/<str:token>', APIKeyItem.as_view()),
     path('api/key', APIKey.as_view()),
     path('api/job/<int:job_id>/<int:exec_id>/log/<int:line_start>', APIJobExecutionLogs.as_view()),
     path('api/job/<int:job_id>/<int:exec_id>/log', APIJobExecutionLogFile.as_view()),
     path('api/job/<int:job_id>/<int:exec_id>', APIJobExecutionItem.as_view()),
@@ -22,13 +25,21 @@
     path('api/permission/<int:perm_id>', APIPermissionItem.as_view()),
     path('api/permission', APIPermission.as_view()),
     path('api/credentials/<int:credentials_id>', APIJobCredentialsItem.as_view()),
     path('api/credentials', APIJobCredentials.as_view()),
     path('api/repository/log/<int:repo_id>', APIRepositoryLogFile.as_view()),
     path('api/repository/<int:repo_id>', APIRepositoryItem.as_view()),
     path('api/repository', APIRepository.as_view()),
+    path('api/alert/plugin/<int:plugin_id>', APIAlertPluginItem.as_view()),
+    path('api/alert/plugin', APIAlertPlugin.as_view()),
+    path('api/alert/global/<int:alert_id>', APIAlertGlobalItem.as_view()),
+    path('api/alert/global', APIAlertGlobal.as_view()),
+    path('api/alert/group/<int:alert_id>', APIAlertGroupItem.as_view()),
+    path('api/alert/group', APIAlertGroup.as_view()),
+    path('api/alert/user/<int:alert_id>', APIAlertUserItem.as_view()),
+    path('api/alert/user', APIAlertUser.as_view()),
     path('api/config', APISystemConfig.as_view()),
     path('api/fs/browse/<str:repository>', APIFsBrowse.as_view()),
     path('api/fs/exists', APIFsExists.as_view()),
     path('api/_schema/', SpectacularAPIView.as_view(), name='_schema'),
     path('api/_docs', SpectacularSwaggerView.as_view(url_name='_schema'), name='swagger-ui'),
 ]
```

### Comparing `ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/api_endpoints/credentials.py` & `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/api_endpoints/credentials.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,16 +4,18 @@
 from rest_framework import serializers
 from rest_framework.response import Response
 from drf_spectacular.utils import extend_schema, OpenApiResponse, OpenApiParameter
 
 from aw.model.job import Job, JobExecution
 from aw.model.job_credential import BaseJobCredentials, JobUserCredentials, JobGlobalCredentials
 from aw.model.permission import CHOICE_PERMISSION_READ, CHOICE_PERMISSION_WRITE, CHOICE_PERMISSION_DELETE
-from aw.api_endpoints.base import API_PERMISSION, get_api_user, GenericResponse, BaseResponse
+from aw.api_endpoints.base import API_PERMISSION, get_api_user, GenericResponse, BaseResponse, api_docs_delete, \
+    api_docs_put, api_docs_post
 from aw.utils.permission import has_credentials_permission, has_manager_privileges
+from aw.config.hardcoded import SECRET_HIDDEN
 from aw.utils.util import is_null
 from aw.base import USERS
 
 
 class JobGlobalCredentialsReadResponse(serializers.ModelSerializer):
     class Meta:
         model = JobGlobalCredentials
@@ -38,18 +40,19 @@
 
 
 class JobGlobalCredentialsWriteRequest(serializers.ModelSerializer):
     class Meta:
         model = JobGlobalCredentials
         fields = JobGlobalCredentials.api_fields_write
 
+    name = serializers.CharField(validators=[])  # uc on update
     vault_pass = serializers.CharField(max_length=100, required=False, default=None, allow_blank=True)
     become_pass = serializers.CharField(max_length=100, required=False, default=None, allow_blank=True)
     connect_pass = serializers.CharField(max_length=100, required=False, default=None, allow_blank=True)
-    ssh_key = serializers.CharField(max_length=2000, required=False, default=None, allow_blank=True)
+    ssh_key = serializers.CharField(max_length=5000, required=False, default=None, allow_blank=True)
 
 
 class JobUserCredentialsWriteRequest(JobGlobalCredentialsWriteRequest):
     class Meta:
         model = JobUserCredentials
         fields = JobUserCredentials.api_fields_write
 
@@ -134,34 +137,30 @@
     )
     def get(self, request):
         user = get_api_user(request)
         credentials_global = []
         credentials_global_raw = JobGlobalCredentials.objects.all()
         for credentials in credentials_global_raw:
             if has_credentials_permission(
-                    user=user,
-                    credentials=credentials,
-                    permission_needed=CHOICE_PERMISSION_READ,
+                user=user,
+                credentials=credentials,
+                permission_needed=CHOICE_PERMISSION_READ,
             ):
                 credentials_global.append(JobGlobalCredentialsReadResponse(instance=credentials).data)
 
         credentials_user_raw = JobUserCredentials.objects.filter(user=user)
         credentials_user = []
         for credentials in credentials_user_raw:
             credentials_user.append(JobUserCredentialsReadResponse(instance=credentials).data)
 
         return Response(data={'shared': credentials_global, 'user': credentials_user}, status=200)
 
     @extend_schema(
         request=JobGlobalCredentialsWriteRequest,
-        responses={
-            200: OpenApiResponse(GenericResponse, description='Credentials created'),
-            400: OpenApiResponse(GenericResponse, description='Invalid credentials data provided'),
-            403: OpenApiResponse(GenericResponse, description='Not privileged to create global credentials'),
-        },
+        responses=api_docs_post('Credentials'),
         summary='Create credentials.',
         operation_id='credentials_create',
         parameters=parameters,
     )
     def post(self, request):
         user = get_api_user(request)
         are_global = are_global_credentials(request)
@@ -182,15 +181,15 @@
                 data={'msg': f"Provided {_log_global_user(are_global)} data is not valid: '{serializer.errors}'"},
                 status=400,
             )
 
         for field in BaseJobCredentials.SECRET_ATTRS:
             value = serializer.validated_data[field]
             if field in BaseJobCredentials.SECRET_ATTRS:
-                if is_null(value) or value == BaseJobCredentials.SECRET_HIDDEN:
+                if is_null(value) or value == SECRET_HIDDEN:
                     serializer.validated_data[field] = None
 
                 elif field == 'ssh_key':
                     value = _validate_and_fix_ssh_key(value)
                     if value is None:
                         return Response(
                             data={'msg': f"Provided {_log_global_user(are_global)} ssh-key is not valid'"},
@@ -253,32 +252,28 @@
             base_msg = f"{_log_global_user(are_global)} with ID {credentials_id} do not exist"
             if not are_global:
                 return Response(data={'msg': f"{base_msg} or belong to another user"}, status=404)
 
             return Response(data={'msg': base_msg}, status=404)
 
         if are_global and not has_credentials_permission(
-                user=user,
-                credentials=credentials,
-                permission_needed=CHOICE_PERMISSION_READ,
+            user=user,
+            credentials=credentials,
+            permission_needed=CHOICE_PERMISSION_READ,
         ):
             return Response(
                 data={'msg': f"{_log_global_user(are_global)} '{credentials.name}' are not viewable"},
                 status=403,
             )
 
         return Response(data=self.serializer_class(instance=credentials).data, status=200)
 
     @extend_schema(
         request=None,
-        responses={
-            200: OpenApiResponse(GenericResponse, description='Credentials deleted'),
-            403: OpenApiResponse(GenericResponse, description='Not privileged to delete the credentials'),
-            404: OpenApiResponse(GenericResponse, description='Credentials do not exist'),
-        },
+        responses=api_docs_delete('Credentials'),
         summary='Delete credentials.',
         operation_id='credentials_delete',
         parameters=parameters,
     )
     def delete(self, request, credentials_id: int):
         user = get_api_user(request)
         are_global = are_global_credentials(request)
@@ -298,17 +293,17 @@
             base_msg = f"{_log_global_user(are_global)} with ID {credentials_id} do not exist"
             if not are_global:
                 return Response(data={'msg': f"{base_msg} or belong to another user"}, status=404)
 
             return Response(data={'msg': base_msg}, status=404)
 
         if are_global and not has_credentials_permission(
-                user=user,
-                credentials=credentials,
-                permission_needed=CHOICE_PERMISSION_DELETE,
+            user=user,
+            credentials=credentials,
+            permission_needed=CHOICE_PERMISSION_DELETE,
         ):
             return Response(
                 data={'msg': f"Not privileged to delete the {_log_global_user(are_global, lower=True)} "
                              f"'{credentials.name}'"},
                 status=403)
 
         if credentials_in_use(credentials):
@@ -319,20 +314,15 @@
             )
 
         credentials.delete()
         return Response(data={'msg': f"{_log_global_user(are_global)} '{credentials.name}' deleted"}, status=200)
 
     @extend_schema(
         request=JobGlobalCredentialsWriteRequest,
-        responses={
-            200: OpenApiResponse(GenericResponse, description='Credentials updated'),
-            400: OpenApiResponse(GenericResponse, description='Invalid credentials data provided'),
-            403: OpenApiResponse(GenericResponse, description='Not privileged to modify the credentials'),
-            404: OpenApiResponse(GenericResponse, description='Credentials do not exist'),
-        },
+        responses=api_docs_put('Credentials'),
         summary='Modify credentials.',
         operation_id='credentials_edit',
         parameters=parameters,
     )
     def put(self, request, credentials_id: int):
         user = get_api_user(request)
         are_global = are_global_credentials(request)
@@ -352,17 +342,17 @@
             base_msg = f"{_log_global_user(are_global)} with ID {credentials_id} do not exist"
             if not are_global:
                 return Response(data={'msg': f"{base_msg} or belong to another user"}, status=404)
 
             return Response(data={'msg': base_msg}, status=404)
 
         if are_global and not has_credentials_permission(
-                user=user,
-                credentials=credentials,
-                permission_needed=CHOICE_PERMISSION_WRITE,
+            user=user,
+            credentials=credentials,
+            permission_needed=CHOICE_PERMISSION_WRITE,
         ):
             return Response(
                 data={'msg': f"Not privileged to modify the {_log_global_user(are_global, lower=True)} "
                              f"'{credentials.name}'"},
                 status=403,
             )
 
@@ -372,17 +362,17 @@
                 data={'msg': f"Provided {_log_global_user(are_global, lower=True)} data is not valid: "
                              f"'{serializer.errors}'"},
                 status=400,
             )
 
         try:
             # not working with password properties: 'Job.objects.filter(id=job_id).update(**serializer.data)'
-            for field, value in serializer.data.items():
+            for field, value in serializer.validated_data.items():
                 if field in BaseJobCredentials.SECRET_ATTRS:
-                    if is_null(value) or value == BaseJobCredentials.SECRET_HIDDEN:
+                    if is_null(value) or value == SECRET_HIDDEN:
                         value = getattr(credentials, field)
 
                     elif field == 'ssh_key':
                         value = _validate_and_fix_ssh_key(value)
                         if value is None:
                             return Response(
                                 data={'msg': f"Provided {_log_global_user(are_global)} ssh-key is not valid'"},
```

### Comparing `ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/api_endpoints/filesystem.py` & `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/api_endpoints/filesystem.py`

 * *Files identical despite different names*

### Comparing `ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/api_endpoints/job.py` & `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/api_endpoints/job.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,29 +7,31 @@
 
 from aw.config.hardcoded import JOB_EXECUTION_LIMIT
 from aw.model.job import Job, JobExecution
 from aw.model.permission import CHOICE_PERMISSION_READ, CHOICE_PERMISSION_EXECUTE, \
     CHOICE_PERMISSION_WRITE, CHOICE_PERMISSION_DELETE
 from aw.model.job_credential import JobGlobalCredentials
 from aw.api_endpoints.base import API_PERMISSION, get_api_user, BaseResponse, GenericResponse, \
-    LogDownloadResponse
+    LogDownloadResponse, api_docs_put, api_docs_delete, api_docs_post
 from aw.api_endpoints.job_util import get_viewable_jobs_serialized, JobReadResponse, get_job_executions_serialized, \
     JobExecutionReadResponse, get_viewable_jobs, get_job_execution_serialized, get_log_file_content
 from aw.utils.permission import has_job_permission, has_credentials_permission, has_manager_privileges
 from aw.execute.queue import queue_add
 from aw.execute.util import update_status, is_execution_status
-from aw.utils.util import is_set
+from aw.utils.util import is_set, ansible_log_html, ansible_log_text
 from aw.base import USERS
 
 
 class JobWriteRequest(serializers.ModelSerializer):
     class Meta:
         model = Job
         fields = Job.api_fields_write
 
+    name = serializers.CharField(validators=[])  # uc on update
+
 
 def _find_job(job_id: int) -> (Job, None):
     try:
         return Job.objects.get(id=job_id)
 
     except ObjectDoesNotExist:
         return None
@@ -121,19 +123,15 @@
         else:
             data = get_viewable_jobs_serialized(get_api_user(request))
 
         return Response(data=data, status=200)
 
     @extend_schema(
         request=JobWriteRequest,
-        responses={
-            200: OpenApiResponse(GenericResponse, description='Job created'),
-            400: OpenApiResponse(GenericResponse, description='Invalid job data provided'),
-            403: OpenApiResponse(GenericResponse, description='Not privileged to create jobs'),
-        },
+        responses=api_docs_post('Job'),
         summary='Create a new job.',
         operation_id='job_create'
     )
     def post(self, request):
         user = get_api_user(request)
         if not has_manager_privileges(user=user, kind='job'):
             return Response(data={'msg': 'Not privileged to create jobs'}, status=403)
@@ -207,19 +205,15 @@
         if want_exec:
             data['executions'] = get_job_executions_serialized(job=job, execution_count=exec_count)
 
         return Response(data=data, status=200)
 
     @extend_schema(
         request=None,
-        responses={
-            200: OpenApiResponse(GenericResponse, description='Job deleted'),
-            403: OpenApiResponse(GenericResponse, description='Not privileged to delete the job'),
-            404: OpenApiResponse(GenericResponse, description='Job does not exist'),
-        },
+        responses=api_docs_delete('Job'),
         summary='Delete a job.',
         operation_id='job_delete'
     )
     def delete(self, request, job_id: int):
         user = get_api_user(request)
         try:
             job = _find_job(job_id)
@@ -234,20 +228,15 @@
         except ObjectDoesNotExist:
             pass
 
         return Response(data={'msg': f"Job with ID {job_id} does not exist"}, status=404)
 
     @extend_schema(
         request=JobWriteRequest,
-        responses={
-            200: OpenApiResponse(GenericResponse, description='Job updated'),
-            400: OpenApiResponse(GenericResponse, description='Invalid job data provided'),
-            403: OpenApiResponse(GenericResponse, description='Not privileged to modify the job'),
-            404: OpenApiResponse(GenericResponse, description='Job does not exist'),
-        },
+        responses=api_docs_put('Job'),
         summary='Modify a job.',
         operation_id='job_edit'
     )
     def put(self, request, job_id: int):
         user = get_api_user(request)
         try:
             job = _find_job(job_id)
@@ -266,15 +255,15 @@
                 if not _has_credentials_permission(user=user, data=serializer.validated_data):
                     return Response(
                         data={'msg': "Not privileged to use provided credentials"},
                         status=403,
                     )
 
                 try:
-                    Job.objects.filter(id=job.id).update(**serializer.data)
+                    Job.objects.filter(id=job.id).update(**serializer.validated_data)
 
                 except IntegrityError as err:
                     return Response(
                         data={'msg': f"Provided job data is not valid: '{err}'"},
                         status=400,
                     )
 
@@ -362,31 +351,51 @@
     @extend_schema(
         request=None,
         responses={
             200: OpenApiResponse(JobExecutionLogReadResponse, description='Return job logs'),
             403: OpenApiResponse(JobExecutionLogReadResponse, description='Not privileged to view the job logs'),
             404: OpenApiResponse(JobExecutionLogReadResponse, description='Job, execution or log-file do not exist'),
         },
+        parameters=[
+            OpenApiParameter(
+                name='format', type=str, default='html',
+                description="Format to return - one of 'plain', 'text' or 'html'",
+                required=False,
+            ),
+        ],
         summary='Get logs of a job execution.',
         operation_id='job_exec_logs'
     )
     def get(self, request, job_id: int, exec_id: int, line_start: int = 0):
         user = get_api_user(request)
+
+        if 'format' not in request.GET:
+            log_fmt = 'html'
+
+        else:
+            log_fmt = str(request.GET['format'])
+
         try:
             job, execution = _find_job_and_execution(job_id, exec_id)
 
             if job is not None and execution is not None:
                 if not has_job_permission(user=user, job=job, permission_needed=CHOICE_PERMISSION_READ):
                     return Response(data={'msg': f"Not privileged to view logs of the job '{job.name}'"}, status=403)
 
                 if execution.log_stdout is None:
                     return Response(data={'msg': f"No logs found for job '{job.name}'"}, status=404)
 
                 with open(execution.log_stdout, 'r', encoding='utf-8') as logfile:
                     lines = logfile.readlines()
+                    if log_fmt == 'html':
+                        lines = [ansible_log_html(line) for line in lines]
+
+                    elif log_fmt == 'text':
+                        lines = [ansible_log_text(line) for line in lines]
+
                     return Response(data={'lines': lines[line_start:]}, status=200)
 
         except (ObjectDoesNotExist, FileNotFoundError):
             pass
 
         return Response(
             data={'msg': f"Job with ID '{job_id}', execution with ID '{exec_id}' or log-file does not exist"},
```

### Comparing `ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/api_endpoints/job_util.py` & `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/api_endpoints/job_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 
 def get_job_execution_serialized(execution: JobExecution) -> dict:
     serialized = JobExecutionReadResponse(instance=execution).data
     serialized['job'] = execution.job.id
     serialized['job_name'] = execution.job.name
     serialized['job_comment'] = execution.job.comment
     serialized['user'] = execution.user.id if execution.user is not None else None
-    serialized['user_name'] = execution.user.username if execution.user is not None else 'Scheduled'
+    serialized['user_name'] = execution.user_name
     serialized['time_start'] = execution.time_created_str
     serialized['time_fin'] = None
     serialized['failed'] = None
     serialized['error_s'] = None
     serialized['error_m'] = None
 
     for logfile in JobExecution.log_file_fields:
```

### Comparing `ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/api_endpoints/key.py` & `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/api_endpoints/key.py`

 * *Files identical despite different names*

### Comparing `ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/api_endpoints/permission.py` & `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/api_endpoints/permission.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from django.core.exceptions import ObjectDoesNotExist
 from django.db.utils import IntegrityError
 from rest_framework.generics import GenericAPIView
 from rest_framework import serializers
 from rest_framework.response import Response
-from drf_spectacular.utils import extend_schema, OpenApiResponse
+from drf_spectacular.utils import extend_schema
 
 from aw.model.job import Job
 from aw.model.job_credential import JobGlobalCredentials
 from aw.model.permission import JobPermission, JobPermissionMapping, JobPermissionMemberUser, \
     JobPermissionMemberGroup, JobCredentialsPermissionMapping, JobRepositoryPermissionMapping
-from aw.api_endpoints.base import API_PERMISSION, GenericResponse, get_api_user
+from aw.api_endpoints.base import API_PERMISSION, GenericResponse, get_api_user, api_docs_put, api_docs_delete, \
+    api_docs_post
 from aw.utils.permission import has_manager_privileges
 from aw.utils.util import is_set
 from aw.base import USERS, GROUPS
 from aw.model.repository import Repository
 
 
 class PermissionReadResponse(serializers.ModelSerializer):
@@ -41,14 +42,15 @@
         fields = JobPermission.api_fields_write
 
     jobs = serializers.MultipleChoiceField(allow_blank=True, choices=[])
     credentials = serializers.MultipleChoiceField(allow_blank=True, choices=[])
     repositories = serializers.MultipleChoiceField(allow_blank=True, choices=[])
     users = serializers.MultipleChoiceField(allow_blank=True, choices=[])
     groups = serializers.MultipleChoiceField(allow_blank=True, choices=[])
+    name = serializers.CharField(validators=[])  # uc on update
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.fields['jobs'] = serializers.MultipleChoiceField(choices=[job.id for job in Job.objects.all()])
         self.fields['credentials'] = serializers.MultipleChoiceField(
             choices=[creds.id for creds in JobGlobalCredentials.objects.all()]
         )
@@ -235,19 +237,15 @@
     )
     def get(request):
         del request
         return Response(build_permissions())
 
     @extend_schema(
         request=PermissionWriteRequest,
-        responses={
-            200: OpenApiResponse(response=GenericResponse, description='Permission created'),
-            400: OpenApiResponse(response=GenericResponse, description='Invalid permission data provided'),
-            403: OpenApiResponse(response=GenericResponse, description='Not privileged to create a permission'),
-        },
+        responses=api_docs_post('Permission'),
         summary='Create a new Permission.',
         operation_id='permission_create',
     )
     def post(self, request):
         privileged = has_manager_privileges(user=get_api_user(request), kind='permission')
         if not privileged:
             return Response(
@@ -268,15 +266,15 @@
 
         except IntegrityError as err:
             return Response(
                 data={'msg': f"Provided permission data is not valid: '{err}'"},
                 status=400,
             )
 
-        return Response({'msg': f"Permission '{serializer.data['name']}' created successfully"})
+        return Response({'msg': f"Permission '{serializer.validated_data['name']}' created successfully"})
 
 
 class APIPermissionItem(GenericAPIView):
     http_method_names = ['get', 'put', 'delete']
     serializer_class = GenericResponse
     permission_classes = API_PERMISSION
 
@@ -289,20 +287,15 @@
     )
     def get(request, perm_id: int):
         del request
         return Response(build_permissions(perm_id_filter=perm_id))
 
     @extend_schema(
         request=PermissionWriteRequest,
-        responses={
-            200: OpenApiResponse(response=GenericResponse, description='Permission updated'),
-            400: OpenApiResponse(response=GenericResponse, description='Invalid permission data provided'),
-            403: OpenApiResponse(response=GenericResponse, description='Not privileged to edit the permission'),
-            404: OpenApiResponse(response=GenericResponse, description='Permission does not exist'),
-        },
+        responses=api_docs_put('Permission'),
         summary='Modify a permission.',
         operation_id='permission_edit',
     )
     def put(self, request, perm_id: int):
         privileged = has_manager_privileges(user=get_api_user(request), kind='permission')
         if not privileged:
             return Response(
@@ -335,20 +328,15 @@
             return Response(data={'msg': f"Permission '{permission.name}' updated"}, status=200)
 
         except IntegrityError as err:
             return Response(data={'msg': f"Provided permission data is not valid: '{err}'"}, status=400)
 
     @extend_schema(
         request=None,
-        responses={
-            200: OpenApiResponse(response=GenericResponse, description='Permission deleted'),
-            400: OpenApiResponse(response=GenericResponse, description='Invalid permission data provided'),
-            403: OpenApiResponse(response=GenericResponse, description='Not privileged to delete the permission'),
-            404: OpenApiResponse(response=GenericResponse, description='Permission does not exist'),
-        },
+        responses=api_docs_delete('Permission'),
         summary='Delete a permission.',
         operation_id='permission_delete'
     )
     def delete(self, request, perm_id: int):
         privileged = has_manager_privileges(user=get_api_user(request), kind='permission')
         if not privileged:
             return Response(
```

### Comparing `ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/api_endpoints/repository.py` & `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/api_endpoints/repository.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,29 +5,32 @@
 from django.db.utils import IntegrityError
 from rest_framework.generics import GenericAPIView
 from rest_framework import serializers
 from rest_framework.response import Response
 from drf_spectacular.utils import extend_schema, OpenApiResponse, OpenApiParameter
 
 from aw.model.repository import Repository
-from aw.api_endpoints.base import API_PERMISSION, GenericResponse, get_api_user, LogDownloadResponse
+from aw.api_endpoints.base import API_PERMISSION, GenericResponse, get_api_user, LogDownloadResponse, api_docs_put, \
+    api_docs_delete, api_docs_post
 from aw.utils.permission import has_manager_privileges, has_repository_permission, get_viewable_repositories
 from aw.model.job import Job
 from aw.utils.util import unset_or_null, is_set
 from aw.model.permission import CHOICE_PERMISSION_READ, CHOICE_PERMISSION_WRITE, CHOICE_PERMISSION_DELETE, \
     CHOICE_PERMISSION_EXECUTE
 from aw.execute.repository import api_update_repository
 from aw.api_endpoints.job_util import get_log_file_content
 
 
 class RepositoryWriteRequest(serializers.ModelSerializer):
     class Meta:
         model = Repository
         fields = Repository.api_fields_write
 
+    name = serializers.CharField(validators=[])  # uc on update
+
 
 class RepositoryReadResponse(RepositoryWriteRequest):
     class Meta:
         model = Repository
         fields = Repository.api_fields_read
 
     rtype_name = serializers.CharField()
@@ -92,19 +95,15 @@
         for repository in get_viewable_repositories(user=user):
             repositories.append(build_repository(repository))
 
         return Response(data=repositories, status=200)
 
     @extend_schema(
         request=RepositoryWriteRequest,
-        responses={
-            200: OpenApiResponse(response=GenericResponse, description='Repository created'),
-            400: OpenApiResponse(response=GenericResponse, description='Invalid repository data provided'),
-            403: OpenApiResponse(response=GenericResponse, description='Not privileged to create a repository'),
-        },
+        responses=api_docs_post('Repository'),
         summary='Create a new Repository.',
         operation_id='repository_create',
     )
     def post(self, request):
         privileged = has_manager_privileges(user=get_api_user(request), kind='repository')
         if not privileged:
             return Response(data={'msg': 'Not privileged to manage repositories'}, status=403)
@@ -120,15 +119,15 @@
 
         try:
             serializer.save()
 
         except IntegrityError as err:
             return Response(data={'msg': f"Provided repository data is not valid: '{err}'"}, status=400)
 
-        return Response({'msg': f"Repository '{serializer.data['name']}' created successfully"})
+        return Response({'msg': f"Repository '{serializer.validated_data['name']}' created successfully"})
 
 
 class APIRepositoryItem(GenericAPIView):
     http_method_names = ['get', 'put', 'post', 'delete']
     serializer_class = GenericResponse
     permission_classes = API_PERMISSION
 
@@ -160,20 +159,15 @@
             return Response(data=build_repository(repository), status=200)
 
         except ObjectDoesNotExist:
             return Response(data={'msg': f"Repository with ID {repo_id} does not exist"}, status=404)
 
     @extend_schema(
         request=RepositoryWriteRequest,
-        responses={
-            200: OpenApiResponse(response=GenericResponse, description='Repository updated'),
-            400: OpenApiResponse(response=GenericResponse, description='Invalid repository data provided'),
-            403: OpenApiResponse(response=GenericResponse, description='Not privileged to edit the repository'),
-            404: OpenApiResponse(response=GenericResponse, description='Repository does not exist'),
-        },
+        responses=api_docs_put('Repository'),
         summary='Modify a repository.',
         operation_id='repository_edit',
     )
     def put(self, request, repo_id: int):
         user = get_api_user(request)
 
         serializer = RepositoryWriteRequest(data=request.data)
@@ -200,28 +194,23 @@
         ):
             return Response(
                 data={'msg': f"Not privileged to modify the repository '{repository.name}'"},
                 status=403,
             )
 
         try:
-            Repository.objects.filter(id=repo_id).update(**serializer.data)
+            Repository.objects.filter(id=repo_id).update(**serializer.validated_data)
             return Response(data={'msg': f"Repository '{repository.name}' updated"}, status=200)
 
         except IntegrityError as err:
             return Response(data={'msg': f"Provided repository data is not valid: '{err}'"}, status=400)
 
     @extend_schema(
         request=None,
-        responses={
-            200: OpenApiResponse(response=GenericResponse, description='Repository deleted'),
-            400: OpenApiResponse(response=GenericResponse, description='Invalid repository data provided'),
-            403: OpenApiResponse(response=GenericResponse, description='Not privileged to delete the repository'),
-            404: OpenApiResponse(response=GenericResponse, description='Repository does not exist'),
-        },
+        responses=api_docs_delete('Repository'),
         summary='Delete a repository.',
         operation_id='repository_delete'
     )
     def delete(self, request, repo_id: int):
         user = get_api_user(request)
 
         try:
```

### Comparing `ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/api_endpoints/system.py` & `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/api_endpoints/system.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,23 +3,24 @@
 from rest_framework import serializers
 from drf_spectacular.utils import extend_schema, OpenApiResponse
 from django.db.utils import IntegrityError
 
 from aw.config.main import config
 from aw.model.system import SystemConfig, get_config_from_db
 from aw.api_endpoints.base import API_PERMISSION, get_api_user, GenericResponse, BaseResponse
-from aw.utils.util_no_config import is_set
+from aw.utils.util_no_config import is_set, is_null
 from aw.utils.debug import log
 from aw.utils.permission import has_manager_privileges
+from aw.config.hardcoded import SECRET_HIDDEN
 
 
 class SystemConfigReadResponse(BaseResponse):
     # todo: fix static fields.. duplicate logic in model
 
-    # SystemConfig.form_fields
+    # SystemConfig.api_fields_read
     path_run = serializers.CharField()
     path_play = serializers.CharField()
     path_log = serializers.CharField()
     timezone = serializers.CharField()
     run_timeout = serializers.IntegerField()
     session_timeout = serializers.IntegerField()
     path_ansible_config = serializers.CharField()
@@ -30,21 +31,28 @@
     db_migrate = serializers.BooleanField()
     serve_static = serializers.BooleanField()
     deployment = serializers.CharField()
     version = serializers.CharField()
     logo_url = serializers.CharField()
     ara_server = serializers.CharField()
     global_environment_vars = serializers.CharField()
+    mail_server = serializers.CharField()
+    mail_transport = serializers.IntegerField()
+    mail_user = serializers.CharField()
+    mail_sender = serializers.CharField()
+    mail_ssl_verify = serializers.BooleanField()
 
 
 class SystemConfigWriteRequest(serializers.ModelSerializer):
     class Meta:
         model = SystemConfig
         fields = SystemConfig.api_fields_write
 
+    mail_pass = serializers.CharField(max_length=100, required=False, default=None, allow_blank=True)
+
 
 class APISystemConfig(APIView):
     http_method_names = ['put', 'get']
     serializer_class = SystemConfigReadResponse
     permission_classes = API_PERMISSION
 
     @staticmethod
@@ -54,15 +62,15 @@
         summary='Return currently active config.',
         operation_id='system_config_view',
     )
     def get(request):
         del request
         merged_config = {'read_only_settings': SystemConfig.api_fields_read_only}
 
-        for field in SystemConfig.form_fields + merged_config['read_only_settings']:
+        for field in SystemConfig.api_fields_read + merged_config['read_only_settings']:
             merged_config[field] = config[field]
 
         merged_config['read_only_settings'] += SystemConfig.get_set_env_vars()
 
         return Response(merged_config)
 
     @extend_schema(
@@ -91,19 +99,23 @@
                 status=400,
             )
 
         config_db = get_config_from_db()
         try:
             changed = False
             for setting, value in serializer.validated_data.items():
+                if setting in SystemConfig.SECRET_ATTRS:
+                    if is_null(value) or value == SECRET_HIDDEN:
+                        value = getattr(config_db, setting)
+
                 if is_set(value) and str(config[setting]) != str(value):
                     setattr(config_db, setting, value)
                     changed = True
 
             if changed:
-                log(msg='System config change - updating', level=5)
+                log(msg='System config changed - updating', level=5)
                 config_db.save()
 
             return Response(data={'msg': "System config updated"}, status=200)
 
         except IntegrityError as err:
             return Response(data={'msg': f"Provided system config is not valid: '{err}'"}, status=400)
```

### Comparing `ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/apps.py` & `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/apps.py`

 * *Files identical despite different names*

### Comparing `ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/config/defaults.py` & `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/config/defaults.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 CONFIG_DEFAULTS = {
     'port': 8000,
     'address': '127.0.0.1',
     'run_timeout': 3600,
     'path_run': '/tmp/ansible-webui',
     'path_play': getcwd(),
     'path_log': f"{environ['HOME']}/.local/share/ansible-webui",
+    'path_template': None,  # only for custom overrides
     'db': f"{environ['HOME']}/.config/ansible-webui",
     'timezone': datetime.now().astimezone().tzname(),
     'secret': ''.join(random_choice(ascii_letters + digits + punctuation) for _ in range(50)),
     'session_timeout': 12 * 60 * 60,  # 12h
     'path_ansible_config': _get_existing_ansible_config_file(),
     'path_ssh_known_hosts': _get_defaults_docker('path_ssh_known_hosts'),
     'debug': False,
```

### Comparing `ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/config/environment.py` & `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/config/environment.py`

 * *Files identical despite different names*

### Comparing `ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/config/hardcoded.py` & `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/config/hardcoded.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,12 +12,14 @@
 MIN_SECRET_LEN = 30
 JOB_EXECUTION_LIMIT = 20
 GRP_MANAGER = {
     'job': 'AW Job Managers',
     'permission': 'AW Permission Managers',
     'repository': 'AW Repository Managers',
     'credentials': 'AW Credentials Managers',
+    'alert': 'AW Alert Managers',
     'system': 'AW System Managers',
 }
 REPO_CLONE_TIMEOUT = 300
 ENV_KEY_CONFIG = 'AW_CONFIG'
 ENV_KEY_SAML = 'AW_SAML'
+SECRET_HIDDEN = '⬤' * 15
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/config/main.py` & `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/config/main.py`

 * *Files identical despite different names*

### Comparing `ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/config/navigation.py` & `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/config/navigation.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,15 +8,15 @@
             'Logs': '/ui/jobs/log',
             'Credentials': '/ui/jobs/credentials',
             'Repositories': '/ui/jobs/repository',
         },
         'Settings': {
             'API Keys': '/ui/settings/api_keys',
             'Permissions': '/ui/settings/permissions',
-            # 'Ansible': '/ui/settings/ansible',
+            'Alerts': '/ui/settings/alerts',
         },
         'System': {
             'Admin': '/ui/system/admin/',
             'API Docs': '/ui/system/api_docs',
             'Config': '/ui/system/config',
             'Environment': '/ui/system/environment',
             'Password': '/a/password_change/',
@@ -25,16 +25,16 @@
     'right': {
         'GH': {
             'element': '<i class="fab fa-github-square fa-2x aw-nav-right-icon" title="GitHub"></i>',
             'url': 'https://github.com/ansibleguy/webui',
             'login': False,
         },
         'DON': {
-            'element': '<i class="fas fa-coins fa-2x aw-nav-right-icon" title="Sponsor"></i>',
-            'url': 'https://github.com/sponsors/ansibleguy',
+            'element': '<i class="fas fa-coins fa-2x aw-nav-right-icon" title="Support the project"></i>',
+            'url': 'https://ko-fi.com/ansible0guy',
             'login': False,
         },
         'BUG': {
             'element': '<i class="fas fa-bug fa-2x aw-nav-right-icon" title="Report bug"></i>',
             'url': 'https://github.com/ansibleguy/webui/issues',
             'login': False,
         },
```

### Comparing `ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/execute/play.py` & `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/execute/play.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from ansible_runner import RunnerConfig, Runner
 
 from aw.config.main import config
 from aw.model.job import Job, JobExecution, JobExecutionResult
 from aw.execute.play_util import runner_cleanup, runner_prep, parse_run_result, failure, runner_logs
 from aw.execute.util import get_path_run, is_execution_status, job_logs
 from aw.execute.repository import ExecuteRepository
+from aw.execute.alert import Alert
 from aw.utils.util import datetime_w_tz, is_null, timed_lru_cache  # get_ansible_versions
 from aw.utils.handlers import AnsibleConfigError
 from aw.utils.debug import log
 
 
 class AwRunnerConfig(RunnerConfig):
     def __init__(self, **kwargs):
@@ -59,15 +60,17 @@
             result=result,
             execution=execution,
             runner=runner,
         )
         del runner
 
         runner_cleanup(execution=execution, path_run=path_run, exec_repo=exec_repo)
+        Alert(job=job, execution=execution).go()
 
     except (OSError, AnsibleConfigError) as err:
         tb = traceback.format_exc(limit=1024)
         failure(
             execution=execution, exec_repo=exec_repo, path_run=path_run, result=result,
             error_s=str(err), error_m=tb,
         )
+        Alert(job=job, execution=execution).go()
         raise
```

### Comparing `ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/execute/play_credentials.py` & `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/execute/play_credentials.py`

 * *Files 7% similar despite different names*

```diff
@@ -67,20 +67,28 @@
 
     elif is_set(job.credentials_default) and _scheduled_or_has_credentials_access(
         user=execution.user, credentials=job.credentials_default,
     ):
         credentials = job.credentials_default
 
     elif job.credentials_needed and is_set(execution.user):
-        # try to get default user-credentials as a last-resort if the job needs some credentials
-        try:
-            credentials = JobUserCredentials.objects.filter(user=execution.user).first()
+        # get user credentials that match the job credential-category
+        if is_set(job.credentials_category):
+            for user_creds in JobUserCredentials.objects.filter(user=execution.user):
+                if user_creds.category == job.credentials_category:
+                    credentials = user_creds
+                    break
 
-        except ObjectDoesNotExist:
-            pass
+        if credentials is None:
+            # try to get default user-credentials as a last-resort if the job needs some credentials
+            try:
+                credentials = JobUserCredentials.objects.filter(user=execution.user).first()
+
+            except ObjectDoesNotExist:
+                pass
 
     if job.credentials_needed and credentials is None:
         config_error(
             'The job is set to require credentials - but none were provided or readable! '
             'Make sure you have privileges for the configured credentials or create user-specific ones.'
         )
```

### Comparing `ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/execute/play_util.py` & `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/execute/play_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -270,10 +270,10 @@
         med=error_m,
     )
     job_error.save()
     result.time_fin = datetime_w_tz()
     result.failed = True
     result.error = job_error
     result.save()
-
     execution.save()
-    runner_cleanup(execution=JobExecution ,path_run=path_run, exec_repo=exec_repo)
+
+    runner_cleanup(execution=execution, path_run=path_run, exec_repo=exec_repo)
```

### Comparing `ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/execute/queue.py` & `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/execute/queue.py`

 * *Files identical despite different names*

### Comparing `ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/execute/repository.py` & `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/execute/repository.py`

 * *Files identical despite different names*

### Comparing `ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/execute/scheduler.py` & `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/execute/scheduler.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,11 @@
-import signal
-from os import environ
-from os import kill as os_kill
-from sys import exit as sys_exit
 from threading import Thread, ThreadError
 from time import sleep, time
+from typing import Callable
 
-from gunicorn.arbiter import Arbiter
 from django.core.validators import ValidationError
 from django.db.utils import OperationalError, IntegrityError
 
 from aw.settings import DB_FILE
 from aw.execute.threader import ThreadManager
 from aw.utils.debug import log
 from aw.utils.util import is_null
@@ -22,46 +18,29 @@
     WAIT_TIME = 1
 
     def __init__(self):
         self.thread_manager = ThreadManager()
         self.stopping = False
         self.reloading = False
 
-    def stop(self, signum=None, error: bool = False):
+    def stop(self):
         if not self.stopping:
-            log('Stopping..', level=3)
-            self._signum_log(signum=signum)
+            log('Stopping scheduler..', level=3)
             self.stopping = True
-
-            log('Stopping job-threads', level=6)
+            log('Stopping job-threads..', level=6)
             self.thread_manager.stop()
-
             sleep(self.WAIT_TIME)
-            log('Finished!')
-
-            # else gunicorn will not know it should die
-            os_kill(int(environ['MAINPID']), signal.SIGTERM)
-
-            # just in case
-            if error or signum is not None:
-                sys_exit(1)
-
-            sys_exit(0)
-
-    @staticmethod
-    def _signum_log(signum):
-        log(f'Scheduler got signal {signum}')
 
     def _add_thread(self, job: Job, execution: JobExecution = None, once: bool = False):
         self.thread_manager.add_thread(job=job, execution=execution, once=once)
         self.thread_manager.start_thread(job=job)
 
     def start(self):
         log('Starting..', level=3)
-        log('Starting job-threads', level=4)
+        log('Starting job-threads..', level=4)
         try:
             self.reload()
             self._run()
 
         except (OperationalError, IntegrityError) as err:
             log(
                 "Database has an unexpected state! "
@@ -94,15 +73,15 @@
                     sleep(self.WAIT_TIME)
 
                 except ThreadError as err:
                     log(msg=f'Got thread error: {err}', level=2)
 
         except Exception as err:
             log(msg=f'Got unexpected error: {err}', level=1)
-            self.stop(error=True)
+            self.stop()
             return
 
     def status(self):
         log(msg=f"Running job-threads: {self.thread_manager.list_pretty()}", level=4)
 
     def check(self):
         log('Checking for queued jobs', level=7)
@@ -118,15 +97,14 @@
 
     def reload(self, signum=None):
         if not self.reloading and not self.stopping:
             self.reloading = True
 
             if signum is not None:
                 log('Reloading..', level=3)
-                self._signum_log(signum=signum)
 
             self._reload_action(**self._reload_check())
             self.thread_manager.clean_stopped_threads()
             self.reloading = False
 
     def _reload_action(self, added: list, removed: list, changed: list):
         any_changed = False
@@ -194,32 +172,11 @@
         for job in running:
             if job.id not in configured_ids:
                 result['removed'].append(job)
 
         return result
 
 
-def init_scheduler():
+def init_scheduler(handle_signals: Callable):
     scheduler = Scheduler()
-    scheduler_thread = Thread(target=scheduler.start)
-
-    # override gunicorn signal handling to allow for graceful shutdown
-    Arbiter.SIGNALS.remove(signal.SIGHUP)
-    Arbiter.SIGNALS.remove(signal.SIGINT)
-    Arbiter.SIGNALS.remove(signal.SIGTERM)
-
-    def signal_exit(signum=None, stack=None):
-        del stack
-        scheduler.stop(signum)
-        os_kill(int(environ['MAINPID']), signal.SIGQUIT)  # trigger 'Arbiter.stop'
-        sleep(3)
-        sys_exit(1)
-
-    def signal_reload(signum=None, stack=None):
-        del stack
-        scheduler.reload(signum)
-
-    signal.signal(signal.SIGHUP, signal_reload)
-    signal.signal(signal.SIGINT, signal_exit)
-    signal.signal(signal.SIGTERM, signal_exit)
-
-    scheduler_thread.start()
+    handle_signals(scheduler)
+    Thread(target=scheduler.start).start()
```

### Comparing `ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/execute/threader.py` & `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/execute/threader.py`

 * *Files identical despite different names*

### Comparing `ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/execute/util.py` & `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/execute/util.py`

 * *Files identical despite different names*

### Comparing `ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/migrations/0001_v0_0_12.py` & `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/migrations/0001_v0_0_12.py`

 * *Files identical despite different names*

### Comparing `ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/migrations/0002_v0_0_13.py` & `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/migrations/0002_v0_0_13.py`

 * *Files identical despite different names*

### Comparing `ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/migrations/0003_v0_0_14.py` & `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/migrations/0003_v0_0_14.py`

 * *Files identical despite different names*

### Comparing `ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/model/base.py` & `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/model/base.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from django.db import models
 
 CHOICES_BOOL = (
     (True, 'Yes'),
     (False, 'No')
 )
 DEFAULT_NONE = {'null': True, 'default': None, 'blank': True}
+JOB_EXEC_STATUS_SUCCESS = 4
 CHOICES_JOB_EXEC_STATUS = [
     (0, 'Waiting'),
     (1, 'Starting'),
     (2, 'Running'),
     (3, 'Failed'),
-    (4, 'Finished'),
+    (JOB_EXEC_STATUS_SUCCESS, 'Finished'),
     (5, 'Stopping'),
     (6, 'Stopped'),
 ]
 
 
 class BareModel(models.Model):
     created = models.DateTimeField(auto_now_add=True)
```

### Comparing `ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/model/job.py` & `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/model/job.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from datetime import datetime
 from datetime import timedelta
 
 from crontab import CronTab
 from django.db import models
 from django.core.validators import ValidationError
 from django.utils import timezone
 
@@ -75,15 +76,15 @@
         raise ValidationError('The provided schedule is not in a valid cron format')
 
 
 class Job(BaseJob):
     CHANGE_FIELDS = [
         'name', 'playbook_file', 'inventory_file', 'repository', 'schedule', 'enabled', 'limit', 'verbosity',
         'mode_diff', 'mode_check', 'tags', 'tags_skip', 'verbosity', 'comment', 'environment_vars', 'cmd_args',
-        'credentials_default', 'credentials_needed',
+        'credentials_default', 'credentials_needed', 'credentials_category',
     ]
     form_fields_primary = ['name', 'playbook_file', 'inventory_file', 'repository']
     form_fields = CHANGE_FIELDS
     api_fields_read = ['id']
     api_fields_read.extend(CHANGE_FIELDS)
     api_fields_write = api_fields_read.copy()
     api_fields_read.append('next_run')
@@ -96,14 +97,15 @@
     schedule = models.CharField(max_length=schedule_max_len, validators=[validate_cronjob], **DEFAULT_NONE)
     enabled = models.BooleanField(choices=CHOICES_BOOL, default=True)
 
     credentials_needed = models.BooleanField(choices=CHOICES_BOOL, default=False)
     credentials_default = models.ForeignKey(
         JobGlobalCredentials, on_delete=models.SET_NULL, related_name='job_fk_creddflt', null=True, blank=True,
     )
+    credentials_category = models.CharField(max_length=100, **DEFAULT_NONE)
     repository = models.ForeignKey(Repository, on_delete=models.SET_NULL, related_name='job_fk_repo', **DEFAULT_NONE)
 
     def __str__(self) -> str:
         limit = '' if self.limit is None else f' [{self.limit}]'
         return f"Job '{self.name}' ({self.playbook_file} => {self.inventory_file}{limit})"
 
     class Meta:
@@ -132,19 +134,27 @@
     def time_fin_str(self) -> str:
         if is_null(self.time_fin):
             return ''
 
         return datetime_from_db_str(dt=self.time_fin, fmt=SHORT_TIME_FORMAT) + f" {config['timezone']}"
 
     @property
+    def time_start_dt(self) -> datetime:
+        return datetime_from_db(self.time_start)
+
+    @property
+    def time_fin_dt(self) -> datetime:
+        return datetime_from_db(self.time_fin)
+
+    @property
     def time_duration(self) -> timedelta:
         if is_null(self.time_fin):
             return timedelta(0)
 
-        return datetime_from_db(self.time_fin) - datetime_from_db(self.time_start)
+        return self.time_fin_dt - self.time_start_dt
 
     @property
     def time_duration_str(self) -> str:
         if is_null(self.time_fin):
             return ''
 
         return pretty_timedelta_str(self.time_duration.total_seconds())
@@ -196,17 +206,14 @@
     )
     job = models.ForeignKey(Job, on_delete=models.CASCADE, related_name='jobexec_fk_job')
     result = models.ForeignKey(
         JobExecutionResult, on_delete=models.SET_NULL, related_name='jobexec_fk_result',
         **DEFAULT_NONE,  # execution is created before result is available
     )
     status = models.PositiveSmallIntegerField(default=0, choices=CHOICES_JOB_EXEC_STATUS)
-    user_credentials = models.ForeignKey(
-        Job, on_delete=models.SET_NULL, related_name='jobexec_fk_usercreds', **DEFAULT_NONE,
-    )
     log_stdout = models.CharField(max_length=300, **DEFAULT_NONE)
     log_stderr = models.CharField(max_length=300, **DEFAULT_NONE)
     log_stdout_repo = models.CharField(max_length=300, **DEFAULT_NONE)
     log_stderr_repo = models.CharField(max_length=300, **DEFAULT_NONE)
     command = models.CharField(max_length=2000, **DEFAULT_NONE)
 
     credential_global = models.ForeignKey(
@@ -232,14 +239,18 @@
         return get_choice_value_by_key(choices=CHOICES_JOB_EXEC_STATUS, find=rtype)
 
     @staticmethod
     def status_id_from_name(name: str) -> int:
         return get_choice_key_by_value(choices=CHOICES_JOB_EXEC_STATUS, find=name)
 
     @property
+    def time_created_dt(self) -> datetime:
+        return datetime_from_db(self.created)
+
+    @property
     def time_created_str(self) -> str:
         if is_null(self.created):
             return ''
 
         return datetime_from_db_str(dt=self.created, fmt=SHORT_TIME_FORMAT) + f" {config['timezone']}"
 
     @property
@@ -254,14 +265,18 @@
     def log_stdout_repo_url(self) -> str:
         return f"/api/job/{self.job.id}/{self.id}/log?type=stdout_repo"
 
     @property
     def log_stderr_repo_url(self) -> str:
         return f"/api/job/{self.job.id}/{self.id}/log?type=stderr_repo"
 
+    @property
+    def user_name(self) -> str:
+        return self.user.username if self.user is not None else 'Scheduled'
+
 
 class JobQueue(BareModel):
     job = models.ForeignKey(Job, on_delete=models.CASCADE, related_name='jobqueue_fk_job')
     user = models.ForeignKey(
         USERS, on_delete=models.SET_NULL, null=True,
         related_name='jobqueue_fk_user',
     )
```

### Comparing `ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/model/job_credential.py` & `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/model/job_credential.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,15 +16,14 @@
     }
     PUBLIC_ATTRS_ARGS = {
         'connect_user': '--user',
         'become_user': '--become-user',
         'vault_file': '--vault-password-file',
         'vault_id': '--vault-id',
     }
-    SECRET_HIDDEN = '⬤' * 15
 
     name = models.CharField(max_length=100, null=False, blank=False)
     connect_user = models.CharField(max_length=100, **DEFAULT_NONE)
     become_user = models.CharField(max_length=100, default='root', null=True, blank=True)
     # default become_user according to ansible-playbook docs
     vault_file = models.CharField(max_length=300, **DEFAULT_NONE)
     vault_id = models.CharField(max_length=50, **DEFAULT_NONE)
@@ -120,15 +119,15 @@
 
     class Meta:
         abstract = True
 
 
 class JobGlobalCredentials(BaseJobCredentials):
     api_fields_read = [
-        'id', 'name', 'become_user', 'connect_user', 'vault_file', 'vault_id'
+        'id', 'name', 'become_user', 'connect_user', 'vault_file', 'vault_id',
     ]
     api_fields_write = api_fields_read.copy()
     api_fields_write.extend(BaseJobCredentials.SECRET_ATTRS)
     for secret_attr in BaseJobCredentials.SECRET_ATTRS:
         api_fields_read.append(f'{secret_attr}_is_set')
     form_fields = api_fields_write
 
@@ -139,21 +138,18 @@
         constraints = [
             models.UniqueConstraint(fields=['name'], name='jobcreds_name')
         ]
 
 
 class JobUserCredentials(BaseJobCredentials):
     api_fields_read = JobGlobalCredentials.api_fields_read.copy()
-    api_fields_read.append('user')
+    api_fields_read.extend(['user', 'category'])
     api_fields_write = JobGlobalCredentials.api_fields_write.copy()
-    api_fields_write.append('user')
+    api_fields_write.extend(['user', 'category'])
     form_fields = JobGlobalCredentials.api_fields_write.copy()
+    form_fields.append('category')
 
     user = models.ForeignKey(USERS, on_delete=models.CASCADE)
+    category = models.CharField(max_length=100, **DEFAULT_NONE)
 
     def __str__(self) -> str:
         return f"Credentials '{self.name}' of user '{self.user.username}'{self._get_set_creds_str()}"
-
-    class Meta:
-        constraints = [
-            models.UniqueConstraint(fields=['user', 'name'], name='jobusercreds_user_name')
-        ]
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/model/permission.py` & `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/model/permission.py`

 * *Files identical despite different names*

### Comparing `ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/model/repository.py` & `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/model/repository.py`

 * *Files identical despite different names*

### Comparing `ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/settings.py` & `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/settings.py`

 * *Files 3% similar despite different names*

```diff
@@ -147,14 +147,26 @@
     CSRF_TRUSTED_ORIGINS.extend([
         f'http://{LISTEN_ADDRESS}'
         f'http://{LISTEN_ADDRESS}:{PORT_WEB}'
         f'https://{LISTEN_ADDRESS}'
         f'https://{LISTEN_ADDRESS}:{PORT_WEB}'
     ])
 
+
+def get_main_web_address() -> str:
+    if 'AW_HOSTNAMES' not in environ:
+        return f'http://localhost:{PORT_WEB}'
+
+    _hostname = environ['AW_HOSTNAMES'].split(',', 1)[0]
+    if 'AW_PROXY' in environ:  # we will not know what port the proxy is serving this service.. assume its 443
+        return f'https://{_hostname}'
+
+    return f'https://{_hostname}:{PORT_WEB}'
+
+
 if 'AW_PROXY' in environ:
     SECURE_PROXY_SSL_HEADER = ('HTTP_X_FORWARDED_PROTO', 'https')
     USE_X_FORWARDED_HOST = True
 
 ALLOWED_HOSTS = ['*']
 if 'AW_HOSTNAMES' in environ:
     for hostname in environ['AW_HOSTNAMES'].split(','):
```

### Comparing `ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/static/css/aw.css` & `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/static/css/aw.css`

 * *Files identical despite different names*

### Comparing `ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/static/css/aw_mobile.css` & `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/static/css/aw_mobile.css`

 * *Files identical despite different names*

### Comparing `ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/static/img/logo.svg` & `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/static/img/logo.svg`

 * *Files identical despite different names*

### Comparing `ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/static/js/aw.js` & `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/static/js/aw.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -202,24 +202,14 @@
         if (shouldSwitch) {
             rows[i].parentNode.insertBefore(rows[i + 1], rows[i]);
             switching = true;
         }
     }
 }
 
-function entryIsFiltered(entryId) {
-    if (HTTP_PARAMS.has('filter')) {
-        let filter_by = HTTP_PARAMS.get('filter');
-        if (is_set(filter_by)) {
-            return Number(filter_by) != Number(entryId);
-        }
-    }
-    return false;
-}
-
 // API CALLS
 const CSRF_TOKEN = getCookie('csrftoken');
 
 function apiActionSuccess(result) {
     resultDiv = document.getElementById('aw-api-result');
     if (result.msg) {
         resultDiv.innerHTML = 'Success: ' + result.msg;
```

### Comparing `ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/static/js/aw_nav.js` & `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/static/js/aw_nav.js`

 * *Files identical despite different names*

### Comparing `ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/static/js/jobs/credentials.js` & `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/static/js/jobs/credentials.js`

 * *Files identical despite different names*

### Comparing `ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/static/js/jobs/edit.js` & `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/static/js/jobs/edit.js`

 * *Files identical despite different names*

### Comparing `ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/static/js/jobs/logs.js` & `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/static/js/jobs/logs.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -1,73 +1,43 @@
-const colorMapping = {
-    '[0m': '</span>',
-    '[0;32m': '<span class="aw-log-ok">',
-    '[1;32m': '<span class="aw-log-ok">',
-    '[0;36m': '<span class="aw-log-skip">',
-    '[1;36m': '<span class="aw-log-skip">',
-    '[0;35m': '<span class="aw-log-warn">',
-    '[1;35m': '<span class="aw-log-warn">',
-    '[0;31m': '<span class="aw-log-err">',
-    '[1;31m': '<span class="aw-log-err">',
-    '[0;33m': '<span class="aw-log-change">',
-    '[1;33m': '<span class="aw-log-change">',
-}
-
 function escapeRegExp(string) {
     return string.replace(/[.*+?^${}()|[\]\\]/g, '\\$&'); // $& means the whole matched string
 }
 
 function replaceAll(str, search, replace) {
     return str.replace(new RegExp(escapeRegExp(search), 'g'), replace);
 }
 
-function replaceLineColors(rawLines) {
-    var fixedLines = [];
-
-    for (line of rawLines) {
-        for (let [search, replace] of Object.entries(colorMapping)) {
-            line = replaceAll(line, search, replace);
-        }
-        fixedLines.push(line);
-    }
-
-    return fixedLines
-}
-
 function addLogLines($this) {
     let logParentElement = $this.attr("aw-expand");
     let logElement = $this.attr("aw-log");
     let logElementEnd = document.getElementById($this.attr("aw-log-end"));
     let job_id = $this.attr("aw-job");
     let exec_id = $this.attr("aw-exec");
     let hidden = document.getElementById(logParentElement).getAttribute("hidden");
     let logLineStart = $this.attr("aw-log-line");
     if (typeof logLineStart === "undefined") {
         logLineStart = 0;
     }
     if (!hidden) {
         $.get("/api/job/" + job_id + "/" + exec_id + "/log/" + logLineStart, function(data) {
             if (data.lines.length > 0) {
-                document.getElementById(logElement).innerHTML += replaceLineColors(data.lines).join('');
+                document.getElementById(logElement).innerHTML += data.lines.join('');
                 $this.attr("aw-log-line", parseInt(logLineStart) + data.lines.length);
                 logElementEnd.scrollIntoView({
                     behavior: "smooth",
                     block: "end",
                     inline: "end"
                 });
             }
         });
     };
 }
 
 function updateApiTableDataJobLogs(row, row2, entry) {
     row.innerHTML = document.getElementById(ELEM_ID_TMPL_ROW).innerHTML;
-    if (entryIsFiltered(entry.job)) {
-        row.setAttribute("hidden", "hidden");
-    }
 
     row.setAttribute("id_job", entry.job);
     row.setAttribute("id_execution", entry.id);
     row2.setAttribute("id_execution", entry.id);
 
     row.cells[0].innerHTML = shortExecutionStatus(entry);
     row.cells[1].innerText = entry.job_name;
@@ -149,14 +119,18 @@
 $(document).ready(function() {
     $(".aw-main").on("click", ".aw-log-read", function() {
         $this = jQuery(this);
         addLogLines($this);
         setInterval('addLogLines($this)', (DATA_REFRESH_SEC * 1000));
     });
     executionCount = 20;
-    if (HTTP_PARAMS.has('filter')) {
-        executionCount = 50;
-    }
     apiEndpoint = "/api/job_exec?execution_count=" + executionCount;
-    fetchApiTableData(apiEndpoint, updateApiTableDataJobLogs, true, null, null, null, true);
-    setInterval('fetchApiTableData(apiEndpoint, updateApiTableDataJobLogs, true, null, null, null, true)', (DATA_REFRESH_SEC * 1000));
+    if (HTTP_PARAMS.has('job')) {
+        dataSubKey = 'executions';
+        apiEndpoint = "/api/job/" + HTTP_PARAMS.get('job') + "?executions=true&execution_count=" + executionCount;
+        fetchApiTableData(apiEndpoint, updateApiTableDataJobLogs, true, null, null, dataSubKey, true);
+        setInterval('fetchApiTableData(apiEndpoint, updateApiTableDataJobLogs, true, null, null, dataSubKey, true)', (DATA_REFRESH_SEC * 1000));
+    } else {
+        fetchApiTableData(apiEndpoint, updateApiTableDataJobLogs, true, null, null, null, true);
+        setInterval('fetchApiTableData(apiEndpoint, updateApiTableDataJobLogs, true, null, null, null, true)', (DATA_REFRESH_SEC * 1000));
+    }
 });
```

### Comparing `ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/static/js/jobs/manage.js` & `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/static/js/jobs/manage.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -75,11 +75,11 @@
         }
     }
     execs += '</div>';
     row2.innerHTML = row2.innerHTML.replaceAll('${EXECS}', execs);
 }
 
 $(document).ready(function() {
-    apiEndpoint = "/api/job?executions=true&execution_count=10";
+    apiEndpoint = "/api/job?executions=true&execution_count=1";
     fetchApiTableData(apiEndpoint, updateApiTableDataJob, true);
     setInterval('fetchApiTableData(apiEndpoint, updateApiTableDataJob, true)', (DATA_REFRESH_SEC * 1000));
 });
```

### Comparing `ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/static/js/jobs/repository.js` & `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/static/js/jobs/repository.js`

 * *Files identical despite different names*

### Comparing `ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/static/js/login.js` & `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/static/js/login.js`

 * *Files identical despite different names*

### Comparing `ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/static/js/settings/api_key.js` & `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/static/js/settings/api_key.js`

 * *Files identical despite different names*

### Comparing `ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/static/js/settings/permission.js` & `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/static/js/settings/permission.js`

 * *Files identical despite different names*

### Comparing `ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/templates/body.html` & `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/body.html`

 * *Files 9% similar despite different names*

```diff
@@ -24,14 +24,14 @@
             <iframe hidden="hidden" id="aw-api-error-full" src="about:blank" width="100%" height="100%" marginheight="0" marginwidth="0" frameborder="0" scrolling="auto"></iframe>
         </main>
         <br>
         <div class="aw-footer-wrapper">
             <footer class="aw-footer">
                 <div class="aw-footer-text">
                     <div>
-                        © {% now 'Y' %} AnsibleGuy | Version {% get_version %}{% if user.is_authenticated %} | User: {{ request.user }}{% endif %} | <a href="https://github.com/sponsors/ansibleguy">Sponsor</a>
+                        © {% now 'Y' %} AnsibleGuy | Version {% get_version %}{% if user.is_authenticated %} | User: {{ request.user }}{% endif %} | <a href="https://ko-fi.com/ansible0guy">Support the project</a>
                     </div>
                 </div>
             </footer>
         </div>
     </body>
 </html>
```

#### html2text {}

```diff
@@ -1,8 +1,9 @@
 {% load util %} {% load static %}
 {% include "./head.html" %} {% block extrahead %} {% endblock %}
 {% include "./nav.html" %} {% include "./error/js_disabled.html" %}
 {{ request.GET|get_value:"error"|ignore_none }}
 {% block content %} {% endblock %} {% if show_update_time %}
 {% endif %}
 Â© {% now 'Y' %} AnsibleGuy | Version {% get_version %}{% if
-user.is_authenticated %} | User: {{ request.user }}{% endif %} | _S_p_o_n_s_o_r
+user.is_authenticated %} | User: {{ request.user }}{% endif %} | _S_u_p_p_o_r_t_ _t_h_e
+_p_r_o_j_e_c_t
```

### Comparing `ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/templates/forms/job.html` & `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/forms/job.html`

 * *Files identical despite different names*

### Comparing `ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/templates/forms/snippet.html` & `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/forms/snippet.html`

 * *Files identical despite different names*

### Comparing `ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/templates/head.html` & `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/head.html`

 * *Files identical despite different names*

### Comparing `ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/templates/jobs/credentials.html` & `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/jobs/credentials.html`

 * *Files identical despite different names*

### Comparing `ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/templates/jobs/credentials_edit.html` & `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/jobs/credentials_edit.html`

 * *Files identical despite different names*

### Comparing `ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/templates/jobs/edit.html` & `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/jobs/edit.html`

 * *Files identical despite different names*

### Comparing `ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/templates/jobs/logs.html` & `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/jobs/logs.html`

 * *Files identical despite different names*

### Comparing `ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/templates/jobs/manage.html` & `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/jobs/manage.html`

 * *Files 4% similar despite different names*

```diff
@@ -44,19 +44,23 @@
                         {% include "../button/icon/collapse.html" %}
                     </button>
                 </div>
             </td>
         </tr>
     </table>
     <div id="aw-api-data-tmpl-actions" hidden="hidden">
-        <!-- todo: allow to choose global- or user-credentials on job-execution -->
-        <button class="btn btn-primary aw-btn-action aw-api-click" title="Run" aw-api-endpoint="job" aw-api-item="${ID}" aw-api-method="post">
+        <button class="btn btn-primary aw-btn-action aw-api-click" title="Quick Execution" aw-api-endpoint="job" aw-api-item="${ID}" aw-api-method="post">
             {% include "../button/icon/run.html" %}
         </button>
-        <a href="/ui/jobs/log?filter=${ID}">
+        <!--
+        <button class="btn btn-primary aw-btn-action aw-btn-expand-child" title="Custom Execution" aw-expand="aw-spoiler-${ID}">
+            {% include "../button/icon/expand.html" %}
+        </button>
+        -->
+        <a href="/ui/jobs/log?job=${ID}">
             <button class="btn btn-info aw-btn-action" title="Logs">
                 <i class="fa-solid fa-scroll fa-2x aw-btn-action-icon"></i>
             </button>
         </a>
         <button class="btn btn-danger aw-btn-action aw-api-click" title="Stop" aw-api-endpoint="job"
                 aw-api-item="${ID}/${EXEC_ID_1}" aw-api-method="delete">
             {% include "../button/icon/stop.html" %}
@@ -70,13 +74,10 @@
             <button class="btn btn-success aw-btn-action" title="Clone">
                 {% include "../button/icon/copy.html" %}
             </button>
         </a>
         <button class="btn btn-danger aw-btn-action aw-api-click" title="Delete" aw-api-endpoint="job" aw-api-item="${ID}" aw-api-method="delete">
             {% include "../button/icon/delete.html" %}
         </button>
-        <button class="btn btn-info aw-btn-action aw-btn-expand-child" title="Expand" aw-expand="aw-spoiler-${ID}">
-            {% include "../button/icon/expand.html" %}
-        </button>
     </div>
 </div>
 {% endblock %}
```

#### html2text {}

```diff
@@ -10,10 +10,9 @@
 {% include "../button/refresh.html" %} _{_%_ _i_n_c_l_u_d_e_ _"_._._/_b_u_t_t_o_n_/_i_c_o_n_/_a_d_d_._h_t_m_l_"_ _%_}
 ********** LLaasstt eexxeeccuuttiioonnss **********
 
 ${EXECS}
 {% include "../button/icon/collapse.html" %}
 {% include "../button/icon/run.html" %} {% include "../button/icon/stop.html"
 %} _{_%_ _i_n_c_l_u_d_e_ _"_._._/_b_u_t_t_o_n_/_i_c_o_n_/_e_d_i_t_._h_t_m_l_"_ _%_}_ _{_%_ _i_n_c_l_u_d_e_ _"_._._/_b_u_t_t_o_n_/_i_c_o_n_/
-_c_o_p_y_._h_t_m_l_"_ _%_}_ {% include "../button/icon/delete.html" %} {% include "../button/
-icon/expand.html" %}
+_c_o_p_y_._h_t_m_l_"_ _%_}_ {% include "../button/icon/delete.html" %}
 {% endblock %}
```

### Comparing `ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/templates/jobs/repository.html` & `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/jobs/repository.html`

 * *Files identical despite different names*

### Comparing `ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/templates/jobs/repository_edit.html` & `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/jobs/repository_edit.html`

 * *Files identical despite different names*

### Comparing `ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/templates/nav.html` & `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/nav.html`

 * *Files identical despite different names*

### Comparing `ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/templates/registration/login.html` & `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/registration/login.html`

 * *Files identical despite different names*

### Comparing `ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/templates/registration/password_change_done.html` & `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/registration/password_change_done.html`

 * *Files identical despite different names*

### Comparing `ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/templates/registration/password_change_form.html` & `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/registration/password_change_form.html`

 * *Files identical despite different names*

### Comparing `ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/templates/registration/saml.html` & `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/registration/saml.html`

 * *Files identical despite different names*

### Comparing `ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/templates/rest_framework/api.html` & `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/rest_framework/api.html`

 * *Files identical despite different names*

### Comparing `ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/templates/settings/api_key.html` & `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/settings/api_key.html`

 * *Files identical despite different names*

### Comparing `ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/templates/settings/permission.html` & `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/settings/permission.html`

 * *Files identical despite different names*

### Comparing `ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/templates/system/config.html` & `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/system/config.html`

 * *Files identical despite different names*

### Comparing `ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/templates/system/environment.html` & `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templates/system/environment.html`

 * *Files identical despite different names*

### Comparing `ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/templatetags/form_util.py` & `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templatetags/form_util.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 from django import template
 
 from django.forms import BoundField, MultipleChoiceField
 from django.forms.widgets import Select
 from django.core.validators import RegexValidator
 
 from aw.model.job_credential import BaseJobCredentials
+from aw.model.system import SystemConfig
 from aw.utils.util import is_set
 from aw.views.validation import AW_VALIDATIONS
+from aw.config.hardcoded import SECRET_HIDDEN
 
 register = template.Library()
 
+FORM_SECRET_FIELDS = BaseJobCredentials.SECRET_ATTRS.copy()
+FORM_SECRET_FIELDS.extend(SystemConfig.SECRET_ATTRS)
+
 
 @register.filter
 def get_form_field_attributes(bf: BoundField) -> str:
     attr_str = ''
     for key, value in bf.field.widget_attrs(bf.field.widget).items():
         attr_str += f' {key}="{value}"'
 
@@ -37,33 +42,39 @@
 
 
 @register.filter
 def form_field_is_dropdown(bf: BoundField) -> bool:
     return isinstance(bf.field.widget, Select)
 
 
+# todo: change boolean fields to checkboxes
+# @register.filter
+# def form_field_is_checkbox(bf: BoundField) -> bool:
+#     return isinstance(bf.field.widget, CheckboxInput)
+
+
 def get_form_required(bf: BoundField) -> str:
     return ' required' if bf.field.required else ''
 
 
 def get_form_field_value(bf: BoundField, existing: dict) -> (str, None):
     # SECRET_ATTRS are not exposed here
-    if bf.name not in existing and bf.name not in BaseJobCredentials.SECRET_ATTRS:
+    if bf.name not in existing and bf.name not in FORM_SECRET_FIELDS:
         return None
 
-    if bf.name in BaseJobCredentials.SECRET_ATTRS:
-        enc_field = '_enc_' + bf.name
+    if bf.name in FORM_SECRET_FIELDS:
+        enc_field = f'_enc_{bf.name}'
         if enc_field in existing and not is_set(existing[enc_field]):
             return None
 
         if enc_field not in existing:
             value = None
 
         else:
-            value = BaseJobCredentials.SECRET_HIDDEN
+            value = SECRET_HIDDEN
 
     else:
         if existing[bf.name] is None:
             return None
 
         value = str(existing[bf.name])
 
@@ -128,15 +139,15 @@
     field_value = ''
     value = get_form_field_value(bf, existing)
     if value is not None:
         field_value = f'value="{value}"'
     elif bf.field.initial is not None:
         field_value = f'value="{bf.field.initial}"'
 
-    if bf.name.find('_pass') != -1 or bf.name.find('_key') != -1:
+    if bf.name in FORM_SECRET_FIELDS or bf.name.find('_pass') != -1 or bf.name.find('_key') != -1:
         field_attrs += ' type="password"'
 
     elif bf.name in AW_VALIDATIONS['file_system_browse']:
         field_classes += ' aw-fs-browse'
         field_attrs += f' type="text" aw-fs-choices="aw-fs-choices-{bf.name}"'
         search_choices = f'<ul class="aw-fs-choices" id="aw-fs-choices-{bf.name}" hidden="hidden"></ul>'
```

### Comparing `ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/templatetags/util.py` & `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/templatetags/util.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from pathlib import Path
 from functools import cache
 
 from django import template
 
 from aw.config.main import config
 from aw.settings import STATIC_URL, AUTH_MODE
 from aw.config.navigation import NAVIGATION
@@ -109,19 +110,34 @@
 
 @register.filter
 def whitespace_char(data: str, char: str) -> str:
     return data.replace(char, ' ')
 
 
 @register.filter
+def remove_char(data: str, char: str) -> str:
+    return data.replace(char, '')
+
+
+@register.filter
 def split(data: str, split_at: str) -> list:
     return data.split(split_at)
 
 
 @register.filter
+def concat(data: str, add: str) -> str:
+    return data + add
+
+
+@register.filter
+def file_exists(file: str) -> bool:
+    return Path(file).is_file()
+
+
+@register.filter
 def find(data: str, search: str) -> bool:
     if not isinstance(data, str):
         data = str(data)
 
     return data.find(search) != -1
```

### Comparing `ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/urls.py` & `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/urls.py`

 * *Files identical despite different names*

### Comparing `ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/utils/crypto.py` & `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/utils/crypto.py`

 * *Files identical despite different names*

### Comparing `ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/utils/debug.py` & `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/utils/debug.py`

 * *Files identical despite different names*

### Comparing `ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/utils/deployment.py` & `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/utils/deployment.py`

 * *Files identical despite different names*

### Comparing `ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/utils/http.py` & `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/utils/http.py`

 * *Files identical despite different names*

### Comparing `ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/utils/permission.py` & `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/utils/permission.py`

 * *Files identical despite different names*

### Comparing `ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/utils/subps.py` & `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/utils/subps.py`

 * *Files identical despite different names*

### Comparing `ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/utils/version.py` & `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/utils/version.py`

 * *Files identical despite different names*

### Comparing `ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/views/base.py` & `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/views/base.py`

 * *Files identical despite different names*

### Comparing `ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/views/forms/auth.py` & `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/views/forms/auth.py`

 * *Files identical despite different names*

### Comparing `ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/views/forms/job.py` & `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/views/forms/job.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,22 +26,24 @@
         labels = FORM_LABEL['jobs']['manage']
         help_texts = FORM_HELP['jobs']['manage']
 
     credentials_default = forms.ChoiceField(
         required=False,
         widget=forms.Select,
         choices=choices_global_credentials,
-        label=FORM_LABEL['jobs']['manage']['credentials_default'],
+        label=Meta.labels['credentials_default'],
+        help_text=Meta.help_texts['credentials_default'],
     )
 
     repository = forms.ChoiceField(
         required=False,
         widget=forms.Select,
         choices=choices_repositories,
-        label=FORM_LABEL['jobs']['manage']['repository'],
+        label=Meta.labels['repository'],
+        help_text=Meta.help_texts['repository'],
     )
 
     # form not picking up regex-validator
     schedule = forms.CharField(
         max_length=Job.schedule_max_len,
         validators=[RegexValidator(
             regex=r'^(@(annually|yearly|monthly|weekly|daily|hourly))|'
@@ -105,24 +107,24 @@
         model = JobGlobalCredentials
         fields = JobGlobalCredentials.form_fields
         field_order = JobGlobalCredentials.form_fields
         labels = FORM_LABEL['jobs']['credentials']
         help_texts = FORM_HELP['jobs']['credentials']
 
     vault_pass = forms.CharField(
-        max_length=100, required=False, label=FORM_LABEL['jobs']['credentials']['vault_pass'],
+        max_length=100, required=False, label=Meta.labels['vault_pass'],
     )
     become_pass = forms.CharField(
-        max_length=100, required=False, label=FORM_LABEL['jobs']['credentials']['become_pass'],
+        max_length=100, required=False, label=Meta.labels['become_pass'],
     )
     connect_pass = forms.CharField(
-        max_length=100, required=False, label=FORM_LABEL['jobs']['credentials']['connect_pass'],
+        max_length=100, required=False, label=Meta.labels['connect_pass'],
     )
     ssh_key = forms.CharField(
-        max_length=2000, required=False, label=FORM_LABEL['jobs']['credentials']['ssh_key'],
+        max_length=5000, required=False, label=Meta.labels['ssh_key'],
     )
 
 
 class CredentialUserForm(CredentialGlobalForm):
     class Meta:
         model = JobUserCredentials
         fields = JobUserCredentials.form_fields
@@ -188,15 +190,15 @@
         labels = FORM_LABEL['jobs']['repository']
         help_texts = FORM_HELP['jobs']['repository']
 
     git_credentials = forms.ChoiceField(
         required=False,
         widget=forms.Select,
         choices=choices_global_credentials,
-        label=FORM_LABEL['jobs']['repository']['git_credentials'],
+        label=Meta.labels['git_credentials'],
     )
 
 
 class RepositoryStaticForm(forms.ModelForm):
     class Meta:
         model = Repository
         fields = Repository.form_fields_static
```

### Comparing `ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/views/forms/system.py` & `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/views/forms/system.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,56 +5,73 @@
 from django.contrib.auth.decorators import login_required
 
 from aw.config.main import config
 from aw.config.defaults import CONFIG_DEFAULTS
 from aw.utils.http import ui_endpoint_wrapper
 from aw.config.form_metadata import FORM_LABEL, FORM_HELP
 from aw.config.environment import AW_ENV_VARS, AW_ENV_VARS_SECRET
-from aw.model.system import SystemConfig
+from aw.model.system import SystemConfig, get_config_from_db
 from aw.utils.deployment import deployment_dev
+from aw.model.base import CHOICES_BOOL
 
 
 class SystemConfigForm(forms.ModelForm):
     class Meta:
         model = SystemConfig
         fields = SystemConfig.form_fields
         field_order = SystemConfig.form_fields
         labels = FORM_LABEL['system']['config']
         help_texts = FORM_HELP['system']['config']
 
-    path_run = forms.CharField(max_length=500, initial=CONFIG_DEFAULTS['path_run'], required=True)
-    path_play = forms.CharField(max_length=500, initial=CONFIG_DEFAULTS['path_play'], required=True)
-    path_log = forms.CharField(max_length=500, initial=CONFIG_DEFAULTS['path_log'], required=True)
+    path_run = forms.CharField(
+        max_length=500, initial=CONFIG_DEFAULTS['path_run'], required=True,
+        label=Meta.labels['path_run'],
+    )
+    path_play = forms.CharField(
+        max_length=500, initial=CONFIG_DEFAULTS['path_play'], required=True,
+        label=Meta.labels['path_play'],
+    )
+    path_log = forms.CharField(
+        max_length=500, initial=CONFIG_DEFAULTS['path_log'], required=True,
+        label=Meta.labels['path_log'],
+    )
     path_ansible_config = forms.CharField(
         max_length=500, initial=CONFIG_DEFAULTS['path_ansible_config'], required=False,
+        label=Meta.labels['path_ansible_config'],
     )
     path_ssh_known_hosts = forms.CharField(
         max_length=500, initial=CONFIG_DEFAULTS['path_ssh_known_hosts'], required=False,
+        label=Meta.labels['path_ssh_known_hosts'],
     )
     timezone = forms.ChoiceField(
         required=False,
         widget=forms.Select,
         choices=[(tz, tz) for tz in sorted(all_timezones)],
-        label=FORM_LABEL['system']['config']['timezone'],
+        label=Meta.labels['timezone'],
+    )
+    debug = forms.ChoiceField(
+        initial=CONFIG_DEFAULTS['debug'] or deployment_dev(), choices=CHOICES_BOOL,
+    )
+    mail_pass = forms.CharField(
+        max_length=100, required=False, label=Meta.labels['mail_pass'],
     )
-    debug = forms.BooleanField(initial=CONFIG_DEFAULTS['debug'] or deployment_dev())
 
 
 @login_required
 @ui_endpoint_wrapper
 def system_config(request) -> HttpResponse:
     config_form = SystemConfigForm()
     form_method = 'put'
     form_api = 'config'
 
+    existing = {key: config[key] for key in SystemConfig.form_fields}
+    existing['_enc_mail_pass'] = get_config_from_db()._enc_mail_pass
     config_form_html = config_form.render(
         template_name='forms/snippet.html',
-        context={'form': config_form, 'existing': {
-            key: config[key] for key in SystemConfig.form_fields
-        }},
+        context={'form': config_form, 'existing': existing},
     )
     return render(
         request, status=200, template_name='system/config.html',
         context={
             'form': config_form_html, 'form_api': form_api, 'form_method': form_method,
             'env_vars': AW_ENV_VARS, 'env_labels': FORM_LABEL['system']['config'],
             'env_vars_secret': AW_ENV_VARS_SECRET,
```

### Comparing `ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/views/job.py` & `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/views/job.py`

 * *Files identical despite different names*

### Comparing `ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/views/main.py` & `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/views/main.py`

 * *Files identical despite different names*

### Comparing `ansibleguy-webui-0.0.18/src/ansibleguy-webui/aw/views/system.py` & `ansibleguy_webui-0.0.19/src/ansibleguy-webui/aw/views/system.py`

 * *Files identical despite different names*

### Comparing `ansibleguy-webui-0.0.18/src/ansibleguy-webui/cli.py` & `ansibleguy_webui-0.0.19/src/ansibleguy-webui/cli.py`

 * *Files identical despite different names*

### Comparing `ansibleguy-webui-0.0.18/src/ansibleguy-webui/cli_init.py` & `ansibleguy_webui-0.0.19/src/ansibleguy-webui/cli_init.py`

 * *Files identical despite different names*

### Comparing `ansibleguy-webui-0.0.18/src/ansibleguy-webui/db.py` & `ansibleguy_webui-0.0.19/src/ansibleguy-webui/db.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from pathlib import Path
-from shutil import copy
+from shutil import copy, move
 from datetime import datetime
 from sys import exit as sys_exit
 from secrets import choice as random_choice
 from string import digits, ascii_letters
 from os import listdir, remove
 from time import time
 from sqlite3 import connect as db_connect
-from sqlite3 import OperationalError
+from sqlite3 import OperationalError, DatabaseError
 
 from aw.config.main import VERSION
 from aw.settings import DB_FILE
 from aw.utils.subps import process
 from aw.utils.debug import log, log_error, log_warn
 from aw.utils.deployment import deployment_prod, is_release_version
 from aw.config.hardcoded import FILE_TIME_FORMAT, GRP_MANAGER
@@ -35,26 +35,46 @@
         remove(test_file)
 
     except PermissionError:
         log(msg=f"Error: DB directory is not writable: '{DB_FILE.parent}'")
         sys_exit(1)
 
 
-def _schema_up_to_date() -> bool:
-    if not Path(DB_FILE).is_file():
-        return False
-
+def _schema_up_to_date_base() -> bool:
     try:
         with db_connect(DB_FILE) as conn:
             return conn.execute('SELECT schema_version FROM aw_schemametadata').fetchall()[0][0] == VERSION
 
     except (IndexError, OperationalError):
         return False
 
 
+def _schema_up_to_date() -> bool:
+    if not Path(DB_FILE).is_file():
+        return False
+
+    try:
+        return _schema_up_to_date_base()
+
+    except DatabaseError as err:
+        # this may happen if WAL or SHM got corrupted (p.e. connection was not closed gracefully)
+        log_warn(msg=f"Trying to fix database error: '{err}'", _stderr=True)
+        backup_ext = f".{datetime.now().strftime(FILE_TIME_FORMAT)}{DB_BACKUP_EXT}"
+        db_shm = f'{DB_FILE}-shm'
+        db_wal = f'{DB_FILE}-wal'
+
+        if Path(db_shm).is_file():
+            move(db_shm, f'{db_shm}{backup_ext}')
+
+        if Path(db_wal).is_file():
+            move(db_wal, f'{db_wal}{backup_ext}')
+
+        return _schema_up_to_date_base()
+
+
 def _get_current_schema_version() -> (str, None):
     try:
         with db_connect(DB_FILE) as conn:
             return conn.execute('SELECT schema_version FROM aw_schemametadata').fetchall()[0][0]
 
     except (IndexError, OperationalError):
         return None
@@ -191,12 +211,12 @@
 
         else:
             log(msg=f"Generated user: '{name}'", level=3)
             log(msg=f"Generated pwd: '{pwd}'", level=3)
             log_warn('Make sure to change the password!')
 
 
-def create_privileged_groups():
+def create_manager_groups():
     # pylint: disable=C0415
     from django.contrib.auth.models import Group
     for grp in GRP_MANAGER.values():
         Group.objects.get_or_create(name=grp)
```

### Comparing `ansibleguy-webui-0.0.18/src/ansibleguy-webui/main.py` & `ansibleguy_webui-0.0.19/src/ansibleguy-webui/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -89,18 +89,19 @@
 
     environ['MAINPID'] = str(getpid())
     install_or_migrate_db()
 
     django_setup()
     environ['AW_INIT'] = '0'
 
-    from db import create_first_superuser, create_privileged_groups
+    from db import create_first_superuser, create_manager_groups
+    from handle_signals import handle_signals
     from webserver import init_webserver
     from aw.execute.scheduler import init_scheduler
     from aw.settings import AUTH_MODE
 
     log(msg=f"Using Auth-Mode: {AUTH_MODE}", level=4)
 
     create_first_superuser()
-    create_privileged_groups()
-    init_scheduler()
+    create_manager_groups()
+    init_scheduler(handle_signals)
     init_webserver()
```

### Comparing `ansibleguy-webui-0.0.18/src/ansibleguy-webui/manage.py` & `ansibleguy_webui-0.0.19/src/ansibleguy-webui/manage.py`

 * *Files identical despite different names*

### Comparing `ansibleguy-webui-0.0.18/src/ansibleguy-webui/web_serve_static.py` & `ansibleguy_webui-0.0.19/src/ansibleguy-webui/web_serve_static.py`

 * *Files identical despite different names*

### Comparing `ansibleguy-webui-0.0.18/src/ansibleguy-webui/webserver.py` & `ansibleguy_webui-0.0.19/src/ansibleguy-webui/webserver.py`

 * *Files identical despite different names*

### Comparing `ansibleguy-webui-0.0.18/src/ansibleguy_webui.egg-info/PKG-INFO` & `ansibleguy_webui-0.0.19/src/ansibleguy_webui.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansibleguy-webui
-Version: 0.0.18
+Version: 0.0.19
 Summary: Basic WebUI for using Ansible
 Author-email: AnsibleGuy <contact@ansibleguy.net>
 License:  GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -670,14 +670,16 @@
 Requires-Dist: crontab
 Requires-Dist: ansible-core
 Requires-Dist: ansible-runner
 Requires-Dist: PyYAML
 
 # Basic WebUI for using Ansible
 
+<a href='https://ko-fi.com/ansible0guy' target='_blank'><img height='35' style='border:0px;height:46px;' src='https://az743702.vo.msecnd.net/cdn/kofi3.png?v=0' border='0' alt='Buy me a coffee' />
+
 [![Documentation](https://readthedocs.org/projects/ansible-webui/badge/?version=latest)](https://webui.ansibleguy.net/en/latest/?badge=latest)
 [![Lint](https://github.com/ansibleguy/webui/actions/workflows/lint.yml/badge.svg?branch=latest)](https://github.com/ansibleguy/webui/actions/workflows/lint.yml)
 [![Test](https://github.com/ansibleguy/webui/actions/workflows/test.yml/badge.svg?branch=latest)](https://github.com/ansibleguy/webui/actions/workflows/test.yml)
 
 **DISCLAIMER**: This is an **unofficial community project**! Do not confuse it with the vanilla [Ansible](https://ansible.com/) product!
 
 The goal is to allow users to quickly install & run a WebUI for using Ansible locally.
@@ -762,27 +764,35 @@
 
   - [x] Execute Ansible using [ansible-runner](https://ansible.readthedocs.io/projects/runner/en/latest/python_interface/)
 
     - [x] Scheduled execution (Cron-Format)
 
     - [x] Manual/immediate execution
 
+    - [ ] Custom Execution-Forms
+
     - [ ] Support for [ad-hoc commands](https://docs.ansible.com/ansible/latest/command_guide/intro_adhoc.html)
 
+    - [ ] Support for [Process-Isolation](https://ansible.readthedocs.io/projects/runner/en/stable/standalone/#running-with-process-isolation)
+
   - [x] Job Logging
 
     - [x] Write job metadata to database
 
     - [x] Write full job-logs to Filesystem
 
   - [x] Secret handling (Connect, Become, Vault)
 
     - [x] User-specific job credentials
 
-  - [ ] Alerting on Failure
+  - [x] Alerting on Failure
+
+    - [x] E-Mail
+
+    - [x] Support for external Plugins (*simple Interface for Scripts*)
 
 - [ ] WebUI
 
   - [x] Job Dashboard
 
       Status, Execute, Time of last & next execution, Last run User, Links to Warnings/Errors
```

### Comparing `ansibleguy-webui-0.0.18/src/ansibleguy_webui.egg-info/SOURCES.txt` & `ansibleguy_webui-0.0.19/src/ansibleguy_webui.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -5,27 +5,29 @@
 pyproject.toml
 requirements.txt
 src/ansibleguy-webui/__init__.py
 src/ansibleguy-webui/__main__.py
 src/ansibleguy-webui/cli.py
 src/ansibleguy-webui/cli_init.py
 src/ansibleguy-webui/db.py
+src/ansibleguy-webui/handle_signals.py
 src/ansibleguy-webui/main.py
 src/ansibleguy-webui/manage.py
 src/ansibleguy-webui/web_serve_static.py
 src/ansibleguy-webui/webserver.py
 src/ansibleguy-webui/aw/__init__.py
 src/ansibleguy-webui/aw/admin.py
 src/ansibleguy-webui/aw/api.py
 src/ansibleguy-webui/aw/apps.py
 src/ansibleguy-webui/aw/base.py
 src/ansibleguy-webui/aw/main.py
 src/ansibleguy-webui/aw/settings.py
 src/ansibleguy-webui/aw/urls.py
 src/ansibleguy-webui/aw/api_endpoints/__init__.py
+src/ansibleguy-webui/aw/api_endpoints/alert.py
 src/ansibleguy-webui/aw/api_endpoints/base.py
 src/ansibleguy-webui/aw/api_endpoints/credentials.py
 src/ansibleguy-webui/aw/api_endpoints/filesystem.py
 src/ansibleguy-webui/aw/api_endpoints/job.py
 src/ansibleguy-webui/aw/api_endpoints/job_util.py
 src/ansibleguy-webui/aw/api_endpoints/key.py
 src/ansibleguy-webui/aw/api_endpoints/permission.py
@@ -44,29 +46,34 @@
 src/ansibleguy-webui/aw/db_sqlite_patched/client.py
 src/ansibleguy-webui/aw/db_sqlite_patched/creation.py
 src/ansibleguy-webui/aw/db_sqlite_patched/features.py
 src/ansibleguy-webui/aw/db_sqlite_patched/introspection.py
 src/ansibleguy-webui/aw/db_sqlite_patched/operations.py
 src/ansibleguy-webui/aw/db_sqlite_patched/schema.py
 src/ansibleguy-webui/aw/execute/__init__.py
+src/ansibleguy-webui/aw/execute/alert.py
 src/ansibleguy-webui/aw/execute/play.py
 src/ansibleguy-webui/aw/execute/play_credentials.py
 src/ansibleguy-webui/aw/execute/play_util.py
 src/ansibleguy-webui/aw/execute/queue.py
 src/ansibleguy-webui/aw/execute/repository.py
 src/ansibleguy-webui/aw/execute/scheduler.py
 src/ansibleguy-webui/aw/execute/threader.py
 src/ansibleguy-webui/aw/execute/util.py
+src/ansibleguy-webui/aw/execute/alert_plugin/plugin_email.py
+src/ansibleguy-webui/aw/execute/alert_plugin/plugin_wrapper.py
 src/ansibleguy-webui/aw/migrations/0001_v0_0_12.py
 src/ansibleguy-webui/aw/migrations/0002_v0_0_13.py
 src/ansibleguy-webui/aw/migrations/0003_v0_0_14.py
 src/ansibleguy-webui/aw/migrations/0004_v0_0_15.py
 src/ansibleguy-webui/aw/migrations/0005_v0_0_18.py
+src/ansibleguy-webui/aw/migrations/0006_v0_0_19.py
 src/ansibleguy-webui/aw/migrations/__init__.py
 src/ansibleguy-webui/aw/model/__init__.py
+src/ansibleguy-webui/aw/model/alert.py
 src/ansibleguy-webui/aw/model/api.py
 src/ansibleguy-webui/aw/model/base.py
 src/ansibleguy-webui/aw/model/job.py
 src/ansibleguy-webui/aw/model/job_credential.py
 src/ansibleguy-webui/aw/model/permission.py
 src/ansibleguy-webui/aw/model/repository.py
 src/ansibleguy-webui/aw/model/system.py
@@ -77,14 +84,15 @@
 src/ansibleguy-webui/aw/static/js/aw_nav.js
 src/ansibleguy-webui/aw/static/js/login.js
 src/ansibleguy-webui/aw/static/js/jobs/credentials.js
 src/ansibleguy-webui/aw/static/js/jobs/edit.js
 src/ansibleguy-webui/aw/static/js/jobs/logs.js
 src/ansibleguy-webui/aw/static/js/jobs/manage.js
 src/ansibleguy-webui/aw/static/js/jobs/repository.js
+src/ansibleguy-webui/aw/static/js/settings/alert.js
 src/ansibleguy-webui/aw/static/js/settings/api_key.js
 src/ansibleguy-webui/aw/static/js/settings/environment.js
 src/ansibleguy-webui/aw/static/js/settings/permission.js
 src/ansibleguy-webui/aw/templates/body.html
 src/ansibleguy-webui/aw/templates/fallback.html
 src/ansibleguy-webui/aw/templates/head.html
 src/ansibleguy-webui/aw/templates/nav.html
@@ -102,14 +110,15 @@
 src/ansibleguy-webui/aw/templates/button/icon/return.html
 src/ansibleguy-webui/aw/templates/button/icon/run.html
 src/ansibleguy-webui/aw/templates/button/icon/sort.html
 src/ansibleguy-webui/aw/templates/button/icon/stop.html
 src/ansibleguy-webui/aw/templates/django_saml2_auth/denied.html
 src/ansibleguy-webui/aw/templates/django_saml2_auth/error.html
 src/ansibleguy-webui/aw/templates/django_saml2_auth/signout.html
+src/ansibleguy-webui/aw/templates/email/alert.html
 src/ansibleguy-webui/aw/templates/error/403.html
 src/ansibleguy-webui/aw/templates/error/500.html
 src/ansibleguy-webui/aw/templates/error/js_disabled.html
 src/ansibleguy-webui/aw/templates/forms/base.html
 src/ansibleguy-webui/aw/templates/forms/job.html
 src/ansibleguy-webui/aw/templates/forms/snippet.html
 src/ansibleguy-webui/aw/templates/forms/snippet_test.html
@@ -122,14 +131,16 @@
 src/ansibleguy-webui/aw/templates/jobs/repository_edit.html
 src/ansibleguy-webui/aw/templates/registration/login.html
 src/ansibleguy-webui/aw/templates/registration/password_change_done.html
 src/ansibleguy-webui/aw/templates/registration/password_change_form.html
 src/ansibleguy-webui/aw/templates/registration/remember_user.html
 src/ansibleguy-webui/aw/templates/registration/saml.html
 src/ansibleguy-webui/aw/templates/rest_framework/api.html
+src/ansibleguy-webui/aw/templates/settings/alert.html
+src/ansibleguy-webui/aw/templates/settings/alert_edit.html
 src/ansibleguy-webui/aw/templates/settings/api_key.html
 src/ansibleguy-webui/aw/templates/settings/permission.html
 src/ansibleguy-webui/aw/templates/settings/permission_edit.html
 src/ansibleguy-webui/aw/templates/system/config.html
 src/ansibleguy-webui/aw/templates/system/environment.html
 src/ansibleguy-webui/aw/templatetags/__init__.py
 src/ansibleguy-webui/aw/templatetags/form_util.py
```

