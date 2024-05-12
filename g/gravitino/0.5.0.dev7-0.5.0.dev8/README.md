# Comparing `tmp/gravitino-0.5.0.dev7.tar.gz` & `tmp/gravitino-0.5.0.dev8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gravitino-0.5.0.dev7.tar", last modified: Sun May 12 01:07:50 2024, max compression
+gzip compressed data, was "gravitino-0.5.0.dev8.tar", last modified: Sun May 12 01:16:44 2024, max compression
```

## Comparing `gravitino-0.5.0.dev7.tar` & `gravitino-0.5.0.dev8.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-12 01:07:50.543015 gravitino-0.5.0.dev7/
--rw-r--r--   0 xun        (501) staff       (20)     5980 2024-05-12 01:07:50.542885 gravitino-0.5.0.dev7/PKG-INFO
--rw-r--r--   0 xun        (501) staff       (20)     5249 2024-05-12 01:01:24.000000 gravitino-0.5.0.dev7/README.md
-drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-12 01:07:50.529702 gravitino-0.5.0.dev7/gravitino/
--rw-r--r--   0 xun        (501) staff       (20)      649 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev7/gravitino/__init__.py
-drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-12 01:07:50.532781 gravitino-0.5.0.dev7/gravitino/api/
--rw-r--r--   0 xun        (501) staff       (20)      105 2024-04-13 14:46:55.000000 gravitino-0.5.0.dev7/gravitino/api/__init__.py
--rw-r--r--   0 xun        (501) staff       (20)      942 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev7/gravitino/api/audit.py
--rw-r--r--   0 xun        (501) staff       (20)      440 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev7/gravitino/api/auditable.py
--rw-r--r--   0 xun        (501) staff       (20)     4113 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev7/gravitino/api/catalog.py
--rw-r--r--   0 xun        (501) staff       (20)     8759 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev7/gravitino/api/catalog_change.py
--rw-r--r--   0 xun        (501) staff       (20)     3556 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev7/gravitino/api/fileset.py
--rw-r--r--   0 xun        (501) staff       (20)     9226 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev7/gravitino/api/fileset_change.py
--rw-r--r--   0 xun        (501) staff       (20)     1155 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev7/gravitino/api/metalake.py
--rw-r--r--   0 xun        (501) staff       (20)     3403 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev7/gravitino/api/metalake_change.py
--rw-r--r--   0 xun        (501) staff       (20)     1044 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev7/gravitino/api/schema.py
--rw-r--r--   0 xun        (501) staff       (20)     4847 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev7/gravitino/api/schema_change.py
--rw-r--r--   0 xun        (501) staff       (20)     3870 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev7/gravitino/api/supports_schemas.py
-drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-12 01:07:50.533330 gravitino-0.5.0.dev7/gravitino/catalog/
--rw-r--r--   0 xun        (501) staff       (20)      105 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev7/gravitino/catalog/__init__.py
--rw-r--r--   0 xun        (501) staff       (20)     7055 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev7/gravitino/catalog/base_schema_catalog.py
--rw-r--r--   0 xun        (501) staff       (20)     7323 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev7/gravitino/catalog/fileset_catalog.py
-drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-12 01:07:50.534744 gravitino-0.5.0.dev7/gravitino/client/
--rw-r--r--   0 xun        (501) staff       (20)      105 2024-04-11 14:36:22.000000 gravitino-0.5.0.dev7/gravitino/client/__init__.py
--rw-r--r--   0 xun        (501) staff       (20)     4651 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev7/gravitino/client/gravitino_admin_client.py
--rw-r--r--   0 xun        (501) staff       (20)     2739 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev7/gravitino/client/gravitino_client.py
--rw-r--r--   0 xun        (501) staff       (20)     2483 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev7/gravitino/client/gravitino_client_base.py
--rw-r--r--   0 xun        (501) staff       (20)     7664 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev7/gravitino/client/gravitino_metalake.py
--rw-r--r--   0 xun        (501) staff       (20)      408 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev7/gravitino/client/gravitino_version.py
--rw-r--r--   0 xun        (501) staff       (20)      119 2024-04-02 06:05:04.000000 gravitino-0.5.0.dev7/gravitino/constants.py
-drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-12 01:07:50.536501 gravitino-0.5.0.dev7/gravitino/dto/
--rw-r--r--   0 xun        (501) staff       (20)      105 2024-04-11 14:36:22.000000 gravitino-0.5.0.dev7/gravitino/dto/__init__.py
--rw-r--r--   0 xun        (501) staff       (20)     1753 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev7/gravitino/dto/audit_dto.py
--rw-r--r--   0 xun        (501) staff       (20)     1590 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev7/gravitino/dto/catalog_dto.py
--rw-r--r--   0 xun        (501) staff       (20)     3019 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev7/gravitino/dto/dto_converters.py
--rw-r--r--   0 xun        (501) staff       (20)     1313 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev7/gravitino/dto/fileset_dto.py
--rw-r--r--   0 xun        (501) staff       (20)     1883 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev7/gravitino/dto/metalake_dto.py
-drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-12 01:07:50.538549 gravitino-0.5.0.dev7/gravitino/dto/requests/
--rw-r--r--   0 xun        (501) staff       (20)      105 2024-04-11 14:36:22.000000 gravitino-0.5.0.dev7/gravitino/dto/requests/__init__.py
--rw-r--r--   0 xun        (501) staff       (20)     1560 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev7/gravitino/dto/requests/catalog_create_request.py
--rw-r--r--   0 xun        (501) staff       (20)     2534 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev7/gravitino/dto/requests/catalog_update_request.py
--rw-r--r--   0 xun        (501) staff       (20)     1065 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev7/gravitino/dto/requests/catalog_updates_request.py
--rw-r--r--   0 xun        (501) staff       (20)     1438 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev7/gravitino/dto/requests/fileset_create_request.py
--rw-r--r--   0 xun        (501) staff       (20)     4267 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev7/gravitino/dto/requests/fileset_update_request.py
--rw-r--r--   0 xun        (501) staff       (20)      750 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev7/gravitino/dto/requests/fileset_updates_request.py
--rw-r--r--   0 xun        (501) staff       (20)     1070 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev7/gravitino/dto/requests/metalake_create_request.py
--rw-r--r--   0 xun        (501) staff       (20)     4145 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev7/gravitino/dto/requests/metalake_update_request.py
--rw-r--r--   0 xun        (501) staff       (20)     1029 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev7/gravitino/dto/requests/metalake_updates_request.py
--rw-r--r--   0 xun        (501) staff       (20)      908 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev7/gravitino/dto/requests/schema_create_request.py
--rw-r--r--   0 xun        (501) staff       (20)     2519 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev7/gravitino/dto/requests/schema_update_request.py
--rw-r--r--   0 xun        (501) staff       (20)      990 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev7/gravitino/dto/requests/schema_updates_request.py
-drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-12 01:07:50.539847 gravitino-0.5.0.dev7/gravitino/dto/responses/
--rw-r--r--   0 xun        (501) staff       (20)      105 2024-04-11 14:36:22.000000 gravitino-0.5.0.dev7/gravitino/dto/responses/__init__.py
--rw-r--r--   0 xun        (501) staff       (20)      683 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev7/gravitino/dto/responses/base_response.py
--rw-r--r--   0 xun        (501) staff       (20)      573 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev7/gravitino/dto/responses/catalog_list_response.py
--rw-r--r--   0 xun        (501) staff       (20)     1051 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev7/gravitino/dto/responses/catalog_response.py
--rw-r--r--   0 xun        (501) staff       (20)      476 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev7/gravitino/dto/responses/drop_response.py
--rw-r--r--   0 xun        (501) staff       (20)      871 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev7/gravitino/dto/responses/entity_list_response.py
--rw-r--r--   0 xun        (501) staff       (20)     1061 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev7/gravitino/dto/responses/fileset_response.py
--rw-r--r--   0 xun        (501) staff       (20)     1162 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev7/gravitino/dto/responses/metalake_list_response.py
--rw-r--r--   0 xun        (501) staff       (20)     1063 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev7/gravitino/dto/responses/metalake_response.py
--rw-r--r--   0 xun        (501) staff       (20)     1058 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev7/gravitino/dto/responses/schema_response.py
--rw-r--r--   0 xun        (501) staff       (20)     1382 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev7/gravitino/dto/schema_dto.py
--rw-r--r--   0 xun        (501) staff       (20)      431 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev7/gravitino/dto/version_dto.py
-drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-12 01:07:50.541730 gravitino-0.5.0.dev7/gravitino/exceptions/
--rw-r--r--   0 xun        (501) staff       (20)      105 2024-04-11 14:36:22.000000 gravitino-0.5.0.dev7/gravitino/exceptions/__init__.py
--rw-r--r--   0 xun        (501) staff       (20)      302 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev7/gravitino/exceptions/gravitino_runtime_exception.py
--rw-r--r--   0 xun        (501) staff       (20)      363 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev7/gravitino/exceptions/illegal_name_identifier_exception.py
--rw-r--r--   0 xun        (501) staff       (20)      352 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev7/gravitino/exceptions/illegal_namespace_exception.py
--rw-r--r--   0 xun        (501) staff       (20)      288 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev7/gravitino/exceptions/no_such_metalake_exception.py
--rw-r--r--   0 xun        (501) staff       (20)      323 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev7/gravitino/exceptions/not_found_exception.py
--rw-r--r--   0 xun        (501) staff       (20)      105 2024-04-02 06:05:04.000000 gravitino-0.5.0.dev7/gravitino/exceptions.py
--rw-r--r--   0 xun        (501) staff       (20)     4404 2024-04-02 06:05:04.000000 gravitino-0.5.0.dev7/gravitino/gravitino_client.py
--rw-r--r--   0 xun        (501) staff       (20)     9268 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev7/gravitino/name_identifier.py
--rw-r--r--   0 xun        (501) staff       (20)     7603 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev7/gravitino/namespace.py
-drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-12 01:07:50.542047 gravitino-0.5.0.dev7/gravitino/rest/
--rw-r--r--   0 xun        (501) staff       (20)      105 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev7/gravitino/rest/__init__.py
--rw-r--r--   0 xun        (501) staff       (20)     1198 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev7/gravitino/rest/rest_message.py
--rw-r--r--   0 xun        (501) staff       (20)     2430 2024-04-02 06:05:04.000000 gravitino-0.5.0.dev7/gravitino/service.py
--rw-r--r--   0 xun        (501) staff       (20)      318 2024-04-02 06:05:04.000000 gravitino-0.5.0.dev7/gravitino/typing.py
-drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-12 01:07:50.542546 gravitino-0.5.0.dev7/gravitino/utils/
--rw-r--r--   0 xun        (501) staff       (20)      175 2024-04-02 06:05:04.000000 gravitino-0.5.0.dev7/gravitino/utils/__init__.py
--rw-r--r--   0 xun        (501) staff       (20)     2692 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev7/gravitino/utils/exceptions.py
--rw-r--r--   0 xun        (501) staff       (20)     5479 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev7/gravitino/utils/http_client.py
-drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-12 01:07:50.530289 gravitino-0.5.0.dev7/gravitino.egg-info/
--rw-r--r--   0 xun        (501) staff       (20)     5980 2024-05-12 01:07:50.000000 gravitino-0.5.0.dev7/gravitino.egg-info/PKG-INFO
--rw-r--r--   0 xun        (501) staff       (20)     2814 2024-05-12 01:07:50.000000 gravitino-0.5.0.dev7/gravitino.egg-info/SOURCES.txt
--rw-r--r--   0 xun        (501) staff       (20)        1 2024-05-12 01:07:50.000000 gravitino-0.5.0.dev7/gravitino.egg-info/dependency_links.txt
--rw-r--r--   0 xun        (501) staff       (20)       72 2024-05-12 01:07:50.000000 gravitino-0.5.0.dev7/gravitino.egg-info/requires.txt
--rw-r--r--   0 xun        (501) staff       (20)       10 2024-05-12 01:07:50.000000 gravitino-0.5.0.dev7/gravitino.egg-info/top_level.txt
--rw-r--r--   0 xun        (501) staff       (20)       38 2024-05-12 01:07:50.543156 gravitino-0.5.0.dev7/setup.cfg
--rw-r--r--   0 xun        (501) staff       (20)     1109 2024-05-12 01:07:39.000000 gravitino-0.5.0.dev7/setup.py
-drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-12 01:07:50.542677 gravitino-0.5.0.dev7/tests/
--rw-r--r--   0 xun        (501) staff       (20)     2192 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev7/tests/test_gravitino_client.py
+drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-12 01:16:44.644824 gravitino-0.5.0.dev8/
+-rw-r--r--   0 xun        (501) staff       (20)     5954 2024-05-12 01:16:44.644703 gravitino-0.5.0.dev8/PKG-INFO
+-rw-r--r--   0 xun        (501) staff       (20)     5223 2024-05-12 01:16:20.000000 gravitino-0.5.0.dev8/README.md
+drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-12 01:16:44.631621 gravitino-0.5.0.dev8/gravitino/
+-rw-r--r--   0 xun        (501) staff       (20)      649 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev8/gravitino/__init__.py
+drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-12 01:16:44.634627 gravitino-0.5.0.dev8/gravitino/api/
+-rw-r--r--   0 xun        (501) staff       (20)      105 2024-04-13 14:46:55.000000 gravitino-0.5.0.dev8/gravitino/api/__init__.py
+-rw-r--r--   0 xun        (501) staff       (20)      942 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev8/gravitino/api/audit.py
+-rw-r--r--   0 xun        (501) staff       (20)      440 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev8/gravitino/api/auditable.py
+-rw-r--r--   0 xun        (501) staff       (20)     4113 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev8/gravitino/api/catalog.py
+-rw-r--r--   0 xun        (501) staff       (20)     8759 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev8/gravitino/api/catalog_change.py
+-rw-r--r--   0 xun        (501) staff       (20)     3556 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev8/gravitino/api/fileset.py
+-rw-r--r--   0 xun        (501) staff       (20)     9226 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev8/gravitino/api/fileset_change.py
+-rw-r--r--   0 xun        (501) staff       (20)     1155 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev8/gravitino/api/metalake.py
+-rw-r--r--   0 xun        (501) staff       (20)     3403 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev8/gravitino/api/metalake_change.py
+-rw-r--r--   0 xun        (501) staff       (20)     1044 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev8/gravitino/api/schema.py
+-rw-r--r--   0 xun        (501) staff       (20)     4847 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev8/gravitino/api/schema_change.py
+-rw-r--r--   0 xun        (501) staff       (20)     3870 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev8/gravitino/api/supports_schemas.py
+drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-12 01:16:44.635397 gravitino-0.5.0.dev8/gravitino/catalog/
+-rw-r--r--   0 xun        (501) staff       (20)      105 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev8/gravitino/catalog/__init__.py
+-rw-r--r--   0 xun        (501) staff       (20)     7055 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev8/gravitino/catalog/base_schema_catalog.py
+-rw-r--r--   0 xun        (501) staff       (20)     7323 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev8/gravitino/catalog/fileset_catalog.py
+drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-12 01:16:44.636720 gravitino-0.5.0.dev8/gravitino/client/
+-rw-r--r--   0 xun        (501) staff       (20)      105 2024-04-11 14:36:22.000000 gravitino-0.5.0.dev8/gravitino/client/__init__.py
+-rw-r--r--   0 xun        (501) staff       (20)     4651 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev8/gravitino/client/gravitino_admin_client.py
+-rw-r--r--   0 xun        (501) staff       (20)     2739 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev8/gravitino/client/gravitino_client.py
+-rw-r--r--   0 xun        (501) staff       (20)     2483 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev8/gravitino/client/gravitino_client_base.py
+-rw-r--r--   0 xun        (501) staff       (20)     7664 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev8/gravitino/client/gravitino_metalake.py
+-rw-r--r--   0 xun        (501) staff       (20)      408 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev8/gravitino/client/gravitino_version.py
+-rw-r--r--   0 xun        (501) staff       (20)      119 2024-04-02 06:05:04.000000 gravitino-0.5.0.dev8/gravitino/constants.py
+drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-12 01:16:44.638447 gravitino-0.5.0.dev8/gravitino/dto/
+-rw-r--r--   0 xun        (501) staff       (20)      105 2024-04-11 14:36:22.000000 gravitino-0.5.0.dev8/gravitino/dto/__init__.py
+-rw-r--r--   0 xun        (501) staff       (20)     1753 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev8/gravitino/dto/audit_dto.py
+-rw-r--r--   0 xun        (501) staff       (20)     1590 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev8/gravitino/dto/catalog_dto.py
+-rw-r--r--   0 xun        (501) staff       (20)     3019 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev8/gravitino/dto/dto_converters.py
+-rw-r--r--   0 xun        (501) staff       (20)     1313 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev8/gravitino/dto/fileset_dto.py
+-rw-r--r--   0 xun        (501) staff       (20)     1883 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev8/gravitino/dto/metalake_dto.py
+drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-12 01:16:44.640555 gravitino-0.5.0.dev8/gravitino/dto/requests/
+-rw-r--r--   0 xun        (501) staff       (20)      105 2024-04-11 14:36:22.000000 gravitino-0.5.0.dev8/gravitino/dto/requests/__init__.py
+-rw-r--r--   0 xun        (501) staff       (20)     1560 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev8/gravitino/dto/requests/catalog_create_request.py
+-rw-r--r--   0 xun        (501) staff       (20)     2534 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev8/gravitino/dto/requests/catalog_update_request.py
+-rw-r--r--   0 xun        (501) staff       (20)     1065 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev8/gravitino/dto/requests/catalog_updates_request.py
+-rw-r--r--   0 xun        (501) staff       (20)     1438 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev8/gravitino/dto/requests/fileset_create_request.py
+-rw-r--r--   0 xun        (501) staff       (20)     4267 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev8/gravitino/dto/requests/fileset_update_request.py
+-rw-r--r--   0 xun        (501) staff       (20)      750 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev8/gravitino/dto/requests/fileset_updates_request.py
+-rw-r--r--   0 xun        (501) staff       (20)     1070 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev8/gravitino/dto/requests/metalake_create_request.py
+-rw-r--r--   0 xun        (501) staff       (20)     4145 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev8/gravitino/dto/requests/metalake_update_request.py
+-rw-r--r--   0 xun        (501) staff       (20)     1029 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev8/gravitino/dto/requests/metalake_updates_request.py
+-rw-r--r--   0 xun        (501) staff       (20)      908 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev8/gravitino/dto/requests/schema_create_request.py
+-rw-r--r--   0 xun        (501) staff       (20)     2519 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev8/gravitino/dto/requests/schema_update_request.py
+-rw-r--r--   0 xun        (501) staff       (20)      990 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev8/gravitino/dto/requests/schema_updates_request.py
+drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-12 01:16:44.641955 gravitino-0.5.0.dev8/gravitino/dto/responses/
+-rw-r--r--   0 xun        (501) staff       (20)      105 2024-04-11 14:36:22.000000 gravitino-0.5.0.dev8/gravitino/dto/responses/__init__.py
+-rw-r--r--   0 xun        (501) staff       (20)      683 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev8/gravitino/dto/responses/base_response.py
+-rw-r--r--   0 xun        (501) staff       (20)      573 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev8/gravitino/dto/responses/catalog_list_response.py
+-rw-r--r--   0 xun        (501) staff       (20)     1051 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev8/gravitino/dto/responses/catalog_response.py
+-rw-r--r--   0 xun        (501) staff       (20)      476 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev8/gravitino/dto/responses/drop_response.py
+-rw-r--r--   0 xun        (501) staff       (20)      871 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev8/gravitino/dto/responses/entity_list_response.py
+-rw-r--r--   0 xun        (501) staff       (20)     1061 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev8/gravitino/dto/responses/fileset_response.py
+-rw-r--r--   0 xun        (501) staff       (20)     1162 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev8/gravitino/dto/responses/metalake_list_response.py
+-rw-r--r--   0 xun        (501) staff       (20)     1063 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev8/gravitino/dto/responses/metalake_response.py
+-rw-r--r--   0 xun        (501) staff       (20)     1058 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev8/gravitino/dto/responses/schema_response.py
+-rw-r--r--   0 xun        (501) staff       (20)     1382 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev8/gravitino/dto/schema_dto.py
+-rw-r--r--   0 xun        (501) staff       (20)      431 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev8/gravitino/dto/version_dto.py
+drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-12 01:16:44.643494 gravitino-0.5.0.dev8/gravitino/exceptions/
+-rw-r--r--   0 xun        (501) staff       (20)      105 2024-04-11 14:36:22.000000 gravitino-0.5.0.dev8/gravitino/exceptions/__init__.py
+-rw-r--r--   0 xun        (501) staff       (20)      302 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev8/gravitino/exceptions/gravitino_runtime_exception.py
+-rw-r--r--   0 xun        (501) staff       (20)      363 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev8/gravitino/exceptions/illegal_name_identifier_exception.py
+-rw-r--r--   0 xun        (501) staff       (20)      352 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev8/gravitino/exceptions/illegal_namespace_exception.py
+-rw-r--r--   0 xun        (501) staff       (20)      288 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev8/gravitino/exceptions/no_such_metalake_exception.py
+-rw-r--r--   0 xun        (501) staff       (20)      323 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev8/gravitino/exceptions/not_found_exception.py
+-rw-r--r--   0 xun        (501) staff       (20)      105 2024-04-02 06:05:04.000000 gravitino-0.5.0.dev8/gravitino/exceptions.py
+-rw-r--r--   0 xun        (501) staff       (20)     4404 2024-04-02 06:05:04.000000 gravitino-0.5.0.dev8/gravitino/gravitino_client.py
+-rw-r--r--   0 xun        (501) staff       (20)     9268 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev8/gravitino/name_identifier.py
+-rw-r--r--   0 xun        (501) staff       (20)     7603 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev8/gravitino/namespace.py
+drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-12 01:16:44.643765 gravitino-0.5.0.dev8/gravitino/rest/
+-rw-r--r--   0 xun        (501) staff       (20)      105 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev8/gravitino/rest/__init__.py
+-rw-r--r--   0 xun        (501) staff       (20)     1198 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev8/gravitino/rest/rest_message.py
+-rw-r--r--   0 xun        (501) staff       (20)     2430 2024-04-02 06:05:04.000000 gravitino-0.5.0.dev8/gravitino/service.py
+-rw-r--r--   0 xun        (501) staff       (20)      318 2024-04-02 06:05:04.000000 gravitino-0.5.0.dev8/gravitino/typing.py
+drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-12 01:16:44.644325 gravitino-0.5.0.dev8/gravitino/utils/
+-rw-r--r--   0 xun        (501) staff       (20)      175 2024-04-02 06:05:04.000000 gravitino-0.5.0.dev8/gravitino/utils/__init__.py
+-rw-r--r--   0 xun        (501) staff       (20)     2692 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev8/gravitino/utils/exceptions.py
+-rw-r--r--   0 xun        (501) staff       (20)     5479 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev8/gravitino/utils/http_client.py
+drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-12 01:16:44.632211 gravitino-0.5.0.dev8/gravitino.egg-info/
+-rw-r--r--   0 xun        (501) staff       (20)     5954 2024-05-12 01:16:44.000000 gravitino-0.5.0.dev8/gravitino.egg-info/PKG-INFO
+-rw-r--r--   0 xun        (501) staff       (20)     2814 2024-05-12 01:16:44.000000 gravitino-0.5.0.dev8/gravitino.egg-info/SOURCES.txt
+-rw-r--r--   0 xun        (501) staff       (20)        1 2024-05-12 01:16:44.000000 gravitino-0.5.0.dev8/gravitino.egg-info/dependency_links.txt
+-rw-r--r--   0 xun        (501) staff       (20)       72 2024-05-12 01:16:44.000000 gravitino-0.5.0.dev8/gravitino.egg-info/requires.txt
+-rw-r--r--   0 xun        (501) staff       (20)       10 2024-05-12 01:16:44.000000 gravitino-0.5.0.dev8/gravitino.egg-info/top_level.txt
+-rw-r--r--   0 xun        (501) staff       (20)       38 2024-05-12 01:16:44.644958 gravitino-0.5.0.dev8/setup.cfg
+-rw-r--r--   0 xun        (501) staff       (20)     1109 2024-05-12 01:16:32.000000 gravitino-0.5.0.dev8/setup.py
+drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-12 01:16:44.644490 gravitino-0.5.0.dev8/tests/
+-rw-r--r--   0 xun        (501) staff       (20)     2192 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev8/tests/test_gravitino_client.py
```

### Comparing `gravitino-0.5.0.dev7/PKG-INFO` & `gravitino-0.5.0.dev8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gravitino
-Version: 0.5.0.dev7
+Version: 0.5.0.dev8
 Summary: Python lib/client for Gravitino
 Home-page: https://github.com/datastrato/gravitino
 Author: datastrato
 Author-email: support@datastrato.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -43,22 +43,22 @@
 ### Gravitino Python client API
 
 1. [Manage metalake using Gravitino Python API](https://datastrato.ai/docs/latest/manage-metalake-using-gravitino?language=python)
 2. [Manage fileset metadata using Gravitino Python API](https://datastrato.ai/docs/latest/manage-fileset-metadata-using-gravitino?language=python)
 
 ### Gravitino Fileset Sample
 We proved a Fileset playground environment to help you quickly understand how to use Gravitino Python client to manage HDFS in Gravitino service.
-You can refer document of [How to use the playground#Launch AI components of playground](https://github.com/datastrato/gravitino/blob/main/docs/how-to-use-the-playground.md#launch-ai-components-of-playground) to launch a Gravitino service, HDFS and Jupyter notebook environment in you local Docker environment.
+You can refer document of [How to use the playground#Launch AI components of playground](https://datastrato.ai/docs/latest/how-to-use-the-playground#launch-ai-components-of-playground) to launch a Gravitino service, HDFS and Jupyter notebook environment in you local Docker environment.
 
 Waiting for the playground Docker environment to start, you can directly open http://localhost:8888/lab/tree/gravitino-fileset-sample.ipynb in the browser and execute it.
 
 The [gravitino-fileset-sample.ipynb](https://github.com/datastrato/gravitino-playground/blob/main/init/jupyter/gravitino-fileset-sample.ipynb) contains the following code paragraphs:
 1. Install HDFS Python client
-2. Create a HDFS client to connect HDFS and to do some test operations 
-3. Install Gravitino Python client 
+2. Create a HDFS client to connect HDFS and to do some test operations
+3. Install Gravitino Python client
 4. Initialize Gravitino admin client and create a Gravitino metalake
 5. Initialize Gravitino client and list metalakes
 6. Create a Gravitino `Catalog` and special `type` is `Catalog.Type.FILESET` and `proved` is [hadoop](https://datastrato.ai/docs/latest/hadoop-catalog)
 7. Create a Gravitino `Schema` and special `location`'s HDFS path, and use `hdfs client` to check if the schema location was successfully created in HDFS
 8. Create a `Fileset` and special `type` is [Fileset.Type.MANAGED](https://datastrato.ai/docs/latest/manage-fileset-metadata-using-gravitino#fileset-operations) and `location`'s HDFS path, and use `hdfs client` to check if the fileset location was successfully created in HDFS
 9. Drop this `Fileset.Type.MANAGED` type fileset and check if the fileset location was successfully deleted in HDFS
 10. Create a `Fileset` and special `type` is [Fileset.Type.EXTERNAL](https://datastrato.ai/docs/latest/manage-fileset-metadata-using-gravitino#fileset-operations) and special `location` to exist HDFS path
```

### Comparing `gravitino-0.5.0.dev7/README.md` & `gravitino-0.5.0.dev8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -22,22 +22,22 @@
 ### Gravitino Python client API
 
 1. [Manage metalake using Gravitino Python API](https://datastrato.ai/docs/latest/manage-metalake-using-gravitino?language=python)
 2. [Manage fileset metadata using Gravitino Python API](https://datastrato.ai/docs/latest/manage-fileset-metadata-using-gravitino?language=python)
 
 ### Gravitino Fileset Sample
 We proved a Fileset playground environment to help you quickly understand how to use Gravitino Python client to manage HDFS in Gravitino service.
-You can refer document of [How to use the playground#Launch AI components of playground](https://github.com/datastrato/gravitino/blob/main/docs/how-to-use-the-playground.md#launch-ai-components-of-playground) to launch a Gravitino service, HDFS and Jupyter notebook environment in you local Docker environment.
+You can refer document of [How to use the playground#Launch AI components of playground](https://datastrato.ai/docs/latest/how-to-use-the-playground#launch-ai-components-of-playground) to launch a Gravitino service, HDFS and Jupyter notebook environment in you local Docker environment.
 
 Waiting for the playground Docker environment to start, you can directly open http://localhost:8888/lab/tree/gravitino-fileset-sample.ipynb in the browser and execute it.
 
 The [gravitino-fileset-sample.ipynb](https://github.com/datastrato/gravitino-playground/blob/main/init/jupyter/gravitino-fileset-sample.ipynb) contains the following code paragraphs:
 1. Install HDFS Python client
-2. Create a HDFS client to connect HDFS and to do some test operations 
-3. Install Gravitino Python client 
+2. Create a HDFS client to connect HDFS and to do some test operations
+3. Install Gravitino Python client
 4. Initialize Gravitino admin client and create a Gravitino metalake
 5. Initialize Gravitino client and list metalakes
 6. Create a Gravitino `Catalog` and special `type` is `Catalog.Type.FILESET` and `proved` is [hadoop](https://datastrato.ai/docs/latest/hadoop-catalog)
 7. Create a Gravitino `Schema` and special `location`'s HDFS path, and use `hdfs client` to check if the schema location was successfully created in HDFS
 8. Create a `Fileset` and special `type` is [Fileset.Type.MANAGED](https://datastrato.ai/docs/latest/manage-fileset-metadata-using-gravitino#fileset-operations) and `location`'s HDFS path, and use `hdfs client` to check if the fileset location was successfully created in HDFS
 9. Drop this `Fileset.Type.MANAGED` type fileset and check if the fileset location was successfully deleted in HDFS
 10. Create a `Fileset` and special `type` is [Fileset.Type.EXTERNAL](https://datastrato.ai/docs/latest/manage-fileset-metadata-using-gravitino#fileset-operations) and special `location` to exist HDFS path
```

### Comparing `gravitino-0.5.0.dev7/gravitino/__init__.py` & `gravitino-0.5.0.dev8/gravitino/__init__.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev7/gravitino/api/audit.py` & `gravitino-0.5.0.dev8/gravitino/api/audit.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev7/gravitino/api/catalog.py` & `gravitino-0.5.0.dev8/gravitino/api/catalog.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev7/gravitino/api/catalog_change.py` & `gravitino-0.5.0.dev8/gravitino/api/catalog_change.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev7/gravitino/api/fileset.py` & `gravitino-0.5.0.dev8/gravitino/api/fileset.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev7/gravitino/api/fileset_change.py` & `gravitino-0.5.0.dev8/gravitino/api/fileset_change.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev7/gravitino/api/metalake.py` & `gravitino-0.5.0.dev8/gravitino/api/metalake.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev7/gravitino/api/metalake_change.py` & `gravitino-0.5.0.dev8/gravitino/api/metalake_change.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev7/gravitino/api/schema.py` & `gravitino-0.5.0.dev8/gravitino/api/schema.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev7/gravitino/api/schema_change.py` & `gravitino-0.5.0.dev8/gravitino/api/schema_change.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev7/gravitino/api/supports_schemas.py` & `gravitino-0.5.0.dev8/gravitino/api/supports_schemas.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev7/gravitino/catalog/base_schema_catalog.py` & `gravitino-0.5.0.dev8/gravitino/catalog/base_schema_catalog.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev7/gravitino/catalog/fileset_catalog.py` & `gravitino-0.5.0.dev8/gravitino/catalog/fileset_catalog.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev7/gravitino/client/gravitino_admin_client.py` & `gravitino-0.5.0.dev8/gravitino/client/gravitino_admin_client.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev7/gravitino/client/gravitino_client.py` & `gravitino-0.5.0.dev8/gravitino/client/gravitino_client.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev7/gravitino/client/gravitino_client_base.py` & `gravitino-0.5.0.dev8/gravitino/client/gravitino_client_base.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev7/gravitino/client/gravitino_metalake.py` & `gravitino-0.5.0.dev8/gravitino/client/gravitino_metalake.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev7/gravitino/dto/audit_dto.py` & `gravitino-0.5.0.dev8/gravitino/dto/audit_dto.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev7/gravitino/dto/catalog_dto.py` & `gravitino-0.5.0.dev8/gravitino/dto/catalog_dto.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev7/gravitino/dto/dto_converters.py` & `gravitino-0.5.0.dev8/gravitino/dto/dto_converters.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev7/gravitino/dto/fileset_dto.py` & `gravitino-0.5.0.dev8/gravitino/dto/fileset_dto.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev7/gravitino/dto/metalake_dto.py` & `gravitino-0.5.0.dev8/gravitino/dto/metalake_dto.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev7/gravitino/dto/requests/catalog_create_request.py` & `gravitino-0.5.0.dev8/gravitino/dto/requests/catalog_create_request.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev7/gravitino/dto/requests/catalog_update_request.py` & `gravitino-0.5.0.dev8/gravitino/dto/requests/catalog_update_request.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev7/gravitino/dto/requests/catalog_updates_request.py` & `gravitino-0.5.0.dev8/gravitino/dto/requests/catalog_updates_request.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev7/gravitino/dto/requests/fileset_create_request.py` & `gravitino-0.5.0.dev8/gravitino/dto/requests/fileset_create_request.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev7/gravitino/dto/requests/fileset_update_request.py` & `gravitino-0.5.0.dev8/gravitino/dto/requests/fileset_update_request.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev7/gravitino/dto/requests/fileset_updates_request.py` & `gravitino-0.5.0.dev8/gravitino/dto/requests/fileset_updates_request.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev7/gravitino/dto/requests/metalake_create_request.py` & `gravitino-0.5.0.dev8/gravitino/dto/requests/metalake_create_request.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev7/gravitino/dto/requests/metalake_update_request.py` & `gravitino-0.5.0.dev8/gravitino/dto/requests/metalake_update_request.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev7/gravitino/dto/requests/metalake_updates_request.py` & `gravitino-0.5.0.dev8/gravitino/dto/requests/metalake_updates_request.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev7/gravitino/dto/requests/schema_create_request.py` & `gravitino-0.5.0.dev8/gravitino/dto/requests/schema_create_request.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev7/gravitino/dto/requests/schema_update_request.py` & `gravitino-0.5.0.dev8/gravitino/dto/requests/schema_update_request.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev7/gravitino/dto/requests/schema_updates_request.py` & `gravitino-0.5.0.dev8/gravitino/dto/requests/schema_updates_request.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev7/gravitino/dto/responses/base_response.py` & `gravitino-0.5.0.dev8/gravitino/dto/responses/base_response.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev7/gravitino/dto/responses/catalog_list_response.py` & `gravitino-0.5.0.dev8/gravitino/dto/responses/catalog_list_response.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev7/gravitino/dto/responses/catalog_response.py` & `gravitino-0.5.0.dev8/gravitino/dto/responses/catalog_response.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev7/gravitino/dto/responses/entity_list_response.py` & `gravitino-0.5.0.dev8/gravitino/dto/responses/entity_list_response.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev7/gravitino/dto/responses/fileset_response.py` & `gravitino-0.5.0.dev8/gravitino/dto/responses/fileset_response.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev7/gravitino/dto/responses/metalake_list_response.py` & `gravitino-0.5.0.dev8/gravitino/dto/responses/metalake_list_response.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev7/gravitino/dto/responses/metalake_response.py` & `gravitino-0.5.0.dev8/gravitino/dto/responses/metalake_response.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev7/gravitino/dto/responses/schema_response.py` & `gravitino-0.5.0.dev8/gravitino/dto/responses/schema_response.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev7/gravitino/dto/schema_dto.py` & `gravitino-0.5.0.dev8/gravitino/dto/schema_dto.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev7/gravitino/gravitino_client.py` & `gravitino-0.5.0.dev8/gravitino/gravitino_client.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev7/gravitino/name_identifier.py` & `gravitino-0.5.0.dev8/gravitino/name_identifier.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev7/gravitino/namespace.py` & `gravitino-0.5.0.dev8/gravitino/namespace.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev7/gravitino/rest/rest_message.py` & `gravitino-0.5.0.dev8/gravitino/rest/rest_message.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev7/gravitino/service.py` & `gravitino-0.5.0.dev8/gravitino/service.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev7/gravitino/utils/exceptions.py` & `gravitino-0.5.0.dev8/gravitino/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev7/gravitino/utils/http_client.py` & `gravitino-0.5.0.dev8/gravitino/utils/http_client.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev7/gravitino.egg-info/PKG-INFO` & `gravitino-0.5.0.dev8/gravitino.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gravitino
-Version: 0.5.0.dev7
+Version: 0.5.0.dev8
 Summary: Python lib/client for Gravitino
 Home-page: https://github.com/datastrato/gravitino
 Author: datastrato
 Author-email: support@datastrato.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -43,22 +43,22 @@
 ### Gravitino Python client API
 
 1. [Manage metalake using Gravitino Python API](https://datastrato.ai/docs/latest/manage-metalake-using-gravitino?language=python)
 2. [Manage fileset metadata using Gravitino Python API](https://datastrato.ai/docs/latest/manage-fileset-metadata-using-gravitino?language=python)
 
 ### Gravitino Fileset Sample
 We proved a Fileset playground environment to help you quickly understand how to use Gravitino Python client to manage HDFS in Gravitino service.
-You can refer document of [How to use the playground#Launch AI components of playground](https://github.com/datastrato/gravitino/blob/main/docs/how-to-use-the-playground.md#launch-ai-components-of-playground) to launch a Gravitino service, HDFS and Jupyter notebook environment in you local Docker environment.
+You can refer document of [How to use the playground#Launch AI components of playground](https://datastrato.ai/docs/latest/how-to-use-the-playground#launch-ai-components-of-playground) to launch a Gravitino service, HDFS and Jupyter notebook environment in you local Docker environment.
 
 Waiting for the playground Docker environment to start, you can directly open http://localhost:8888/lab/tree/gravitino-fileset-sample.ipynb in the browser and execute it.
 
 The [gravitino-fileset-sample.ipynb](https://github.com/datastrato/gravitino-playground/blob/main/init/jupyter/gravitino-fileset-sample.ipynb) contains the following code paragraphs:
 1. Install HDFS Python client
-2. Create a HDFS client to connect HDFS and to do some test operations 
-3. Install Gravitino Python client 
+2. Create a HDFS client to connect HDFS and to do some test operations
+3. Install Gravitino Python client
 4. Initialize Gravitino admin client and create a Gravitino metalake
 5. Initialize Gravitino client and list metalakes
 6. Create a Gravitino `Catalog` and special `type` is `Catalog.Type.FILESET` and `proved` is [hadoop](https://datastrato.ai/docs/latest/hadoop-catalog)
 7. Create a Gravitino `Schema` and special `location`'s HDFS path, and use `hdfs client` to check if the schema location was successfully created in HDFS
 8. Create a `Fileset` and special `type` is [Fileset.Type.MANAGED](https://datastrato.ai/docs/latest/manage-fileset-metadata-using-gravitino#fileset-operations) and `location`'s HDFS path, and use `hdfs client` to check if the fileset location was successfully created in HDFS
 9. Drop this `Fileset.Type.MANAGED` type fileset and check if the fileset location was successfully deleted in HDFS
 10. Create a `Fileset` and special `type` is [Fileset.Type.EXTERNAL](https://datastrato.ai/docs/latest/manage-fileset-metadata-using-gravitino#fileset-operations) and special `location` to exist HDFS path
```

### Comparing `gravitino-0.5.0.dev7/gravitino.egg-info/SOURCES.txt` & `gravitino-0.5.0.dev8/gravitino.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev7/setup.py` & `gravitino-0.5.0.dev8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from setuptools import find_packages, setup
 
 
 setup(
     name="gravitino",
     description="Python lib/client for Gravitino",
-    version="0.5.0.dev7",
+    version="0.5.0.dev8",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/datastrato/gravitino",
     author="datastrato",
     author_email="support@datastrato.com",
     python_requires=">=3.8",
     packages=find_packages(exclude=["tests*"]),
```

### Comparing `gravitino-0.5.0.dev7/tests/test_gravitino_client.py` & `gravitino-0.5.0.dev8/tests/test_gravitino_client.py`

 * *Files identical despite different names*

