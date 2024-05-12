# Comparing `tmp/gravitino-0.5.0.dev8.tar.gz` & `tmp/gravitino-0.5.0.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gravitino-0.5.0.dev8.tar", last modified: Sun May 12 01:16:44 2024, max compression
+gzip compressed data, was "gravitino-0.5.0.dev9.tar", last modified: Sun May 12 09:21:45 2024, max compression
```

## Comparing `gravitino-0.5.0.dev8.tar` & `gravitino-0.5.0.dev9.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-12 01:16:44.644824 gravitino-0.5.0.dev8/
--rw-r--r--   0 xun        (501) staff       (20)     5954 2024-05-12 01:16:44.644703 gravitino-0.5.0.dev8/PKG-INFO
--rw-r--r--   0 xun        (501) staff       (20)     5223 2024-05-12 01:16:20.000000 gravitino-0.5.0.dev8/README.md
-drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-12 01:16:44.631621 gravitino-0.5.0.dev8/gravitino/
--rw-r--r--   0 xun        (501) staff       (20)      649 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev8/gravitino/__init__.py
-drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-12 01:16:44.634627 gravitino-0.5.0.dev8/gravitino/api/
--rw-r--r--   0 xun        (501) staff       (20)      105 2024-04-13 14:46:55.000000 gravitino-0.5.0.dev8/gravitino/api/__init__.py
--rw-r--r--   0 xun        (501) staff       (20)      942 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev8/gravitino/api/audit.py
--rw-r--r--   0 xun        (501) staff       (20)      440 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev8/gravitino/api/auditable.py
--rw-r--r--   0 xun        (501) staff       (20)     4113 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev8/gravitino/api/catalog.py
--rw-r--r--   0 xun        (501) staff       (20)     8759 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev8/gravitino/api/catalog_change.py
--rw-r--r--   0 xun        (501) staff       (20)     3556 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev8/gravitino/api/fileset.py
--rw-r--r--   0 xun        (501) staff       (20)     9226 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev8/gravitino/api/fileset_change.py
--rw-r--r--   0 xun        (501) staff       (20)     1155 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev8/gravitino/api/metalake.py
--rw-r--r--   0 xun        (501) staff       (20)     3403 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev8/gravitino/api/metalake_change.py
--rw-r--r--   0 xun        (501) staff       (20)     1044 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev8/gravitino/api/schema.py
--rw-r--r--   0 xun        (501) staff       (20)     4847 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev8/gravitino/api/schema_change.py
--rw-r--r--   0 xun        (501) staff       (20)     3870 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev8/gravitino/api/supports_schemas.py
-drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-12 01:16:44.635397 gravitino-0.5.0.dev8/gravitino/catalog/
--rw-r--r--   0 xun        (501) staff       (20)      105 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev8/gravitino/catalog/__init__.py
--rw-r--r--   0 xun        (501) staff       (20)     7055 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev8/gravitino/catalog/base_schema_catalog.py
--rw-r--r--   0 xun        (501) staff       (20)     7323 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev8/gravitino/catalog/fileset_catalog.py
-drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-12 01:16:44.636720 gravitino-0.5.0.dev8/gravitino/client/
--rw-r--r--   0 xun        (501) staff       (20)      105 2024-04-11 14:36:22.000000 gravitino-0.5.0.dev8/gravitino/client/__init__.py
--rw-r--r--   0 xun        (501) staff       (20)     4651 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev8/gravitino/client/gravitino_admin_client.py
--rw-r--r--   0 xun        (501) staff       (20)     2739 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev8/gravitino/client/gravitino_client.py
--rw-r--r--   0 xun        (501) staff       (20)     2483 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev8/gravitino/client/gravitino_client_base.py
--rw-r--r--   0 xun        (501) staff       (20)     7664 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev8/gravitino/client/gravitino_metalake.py
--rw-r--r--   0 xun        (501) staff       (20)      408 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev8/gravitino/client/gravitino_version.py
--rw-r--r--   0 xun        (501) staff       (20)      119 2024-04-02 06:05:04.000000 gravitino-0.5.0.dev8/gravitino/constants.py
-drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-12 01:16:44.638447 gravitino-0.5.0.dev8/gravitino/dto/
--rw-r--r--   0 xun        (501) staff       (20)      105 2024-04-11 14:36:22.000000 gravitino-0.5.0.dev8/gravitino/dto/__init__.py
--rw-r--r--   0 xun        (501) staff       (20)     1753 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev8/gravitino/dto/audit_dto.py
--rw-r--r--   0 xun        (501) staff       (20)     1590 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev8/gravitino/dto/catalog_dto.py
--rw-r--r--   0 xun        (501) staff       (20)     3019 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev8/gravitino/dto/dto_converters.py
--rw-r--r--   0 xun        (501) staff       (20)     1313 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev8/gravitino/dto/fileset_dto.py
--rw-r--r--   0 xun        (501) staff       (20)     1883 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev8/gravitino/dto/metalake_dto.py
-drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-12 01:16:44.640555 gravitino-0.5.0.dev8/gravitino/dto/requests/
--rw-r--r--   0 xun        (501) staff       (20)      105 2024-04-11 14:36:22.000000 gravitino-0.5.0.dev8/gravitino/dto/requests/__init__.py
--rw-r--r--   0 xun        (501) staff       (20)     1560 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev8/gravitino/dto/requests/catalog_create_request.py
--rw-r--r--   0 xun        (501) staff       (20)     2534 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev8/gravitino/dto/requests/catalog_update_request.py
--rw-r--r--   0 xun        (501) staff       (20)     1065 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev8/gravitino/dto/requests/catalog_updates_request.py
--rw-r--r--   0 xun        (501) staff       (20)     1438 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev8/gravitino/dto/requests/fileset_create_request.py
--rw-r--r--   0 xun        (501) staff       (20)     4267 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev8/gravitino/dto/requests/fileset_update_request.py
--rw-r--r--   0 xun        (501) staff       (20)      750 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev8/gravitino/dto/requests/fileset_updates_request.py
--rw-r--r--   0 xun        (501) staff       (20)     1070 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev8/gravitino/dto/requests/metalake_create_request.py
--rw-r--r--   0 xun        (501) staff       (20)     4145 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev8/gravitino/dto/requests/metalake_update_request.py
--rw-r--r--   0 xun        (501) staff       (20)     1029 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev8/gravitino/dto/requests/metalake_updates_request.py
--rw-r--r--   0 xun        (501) staff       (20)      908 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev8/gravitino/dto/requests/schema_create_request.py
--rw-r--r--   0 xun        (501) staff       (20)     2519 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev8/gravitino/dto/requests/schema_update_request.py
--rw-r--r--   0 xun        (501) staff       (20)      990 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev8/gravitino/dto/requests/schema_updates_request.py
-drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-12 01:16:44.641955 gravitino-0.5.0.dev8/gravitino/dto/responses/
--rw-r--r--   0 xun        (501) staff       (20)      105 2024-04-11 14:36:22.000000 gravitino-0.5.0.dev8/gravitino/dto/responses/__init__.py
--rw-r--r--   0 xun        (501) staff       (20)      683 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev8/gravitino/dto/responses/base_response.py
--rw-r--r--   0 xun        (501) staff       (20)      573 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev8/gravitino/dto/responses/catalog_list_response.py
--rw-r--r--   0 xun        (501) staff       (20)     1051 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev8/gravitino/dto/responses/catalog_response.py
--rw-r--r--   0 xun        (501) staff       (20)      476 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev8/gravitino/dto/responses/drop_response.py
--rw-r--r--   0 xun        (501) staff       (20)      871 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev8/gravitino/dto/responses/entity_list_response.py
--rw-r--r--   0 xun        (501) staff       (20)     1061 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev8/gravitino/dto/responses/fileset_response.py
--rw-r--r--   0 xun        (501) staff       (20)     1162 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev8/gravitino/dto/responses/metalake_list_response.py
--rw-r--r--   0 xun        (501) staff       (20)     1063 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev8/gravitino/dto/responses/metalake_response.py
--rw-r--r--   0 xun        (501) staff       (20)     1058 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev8/gravitino/dto/responses/schema_response.py
--rw-r--r--   0 xun        (501) staff       (20)     1382 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev8/gravitino/dto/schema_dto.py
--rw-r--r--   0 xun        (501) staff       (20)      431 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev8/gravitino/dto/version_dto.py
-drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-12 01:16:44.643494 gravitino-0.5.0.dev8/gravitino/exceptions/
--rw-r--r--   0 xun        (501) staff       (20)      105 2024-04-11 14:36:22.000000 gravitino-0.5.0.dev8/gravitino/exceptions/__init__.py
--rw-r--r--   0 xun        (501) staff       (20)      302 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev8/gravitino/exceptions/gravitino_runtime_exception.py
--rw-r--r--   0 xun        (501) staff       (20)      363 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev8/gravitino/exceptions/illegal_name_identifier_exception.py
--rw-r--r--   0 xun        (501) staff       (20)      352 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev8/gravitino/exceptions/illegal_namespace_exception.py
--rw-r--r--   0 xun        (501) staff       (20)      288 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev8/gravitino/exceptions/no_such_metalake_exception.py
--rw-r--r--   0 xun        (501) staff       (20)      323 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev8/gravitino/exceptions/not_found_exception.py
--rw-r--r--   0 xun        (501) staff       (20)      105 2024-04-02 06:05:04.000000 gravitino-0.5.0.dev8/gravitino/exceptions.py
--rw-r--r--   0 xun        (501) staff       (20)     4404 2024-04-02 06:05:04.000000 gravitino-0.5.0.dev8/gravitino/gravitino_client.py
--rw-r--r--   0 xun        (501) staff       (20)     9268 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev8/gravitino/name_identifier.py
--rw-r--r--   0 xun        (501) staff       (20)     7603 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev8/gravitino/namespace.py
-drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-12 01:16:44.643765 gravitino-0.5.0.dev8/gravitino/rest/
--rw-r--r--   0 xun        (501) staff       (20)      105 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev8/gravitino/rest/__init__.py
--rw-r--r--   0 xun        (501) staff       (20)     1198 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev8/gravitino/rest/rest_message.py
--rw-r--r--   0 xun        (501) staff       (20)     2430 2024-04-02 06:05:04.000000 gravitino-0.5.0.dev8/gravitino/service.py
--rw-r--r--   0 xun        (501) staff       (20)      318 2024-04-02 06:05:04.000000 gravitino-0.5.0.dev8/gravitino/typing.py
-drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-12 01:16:44.644325 gravitino-0.5.0.dev8/gravitino/utils/
--rw-r--r--   0 xun        (501) staff       (20)      175 2024-04-02 06:05:04.000000 gravitino-0.5.0.dev8/gravitino/utils/__init__.py
--rw-r--r--   0 xun        (501) staff       (20)     2692 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev8/gravitino/utils/exceptions.py
--rw-r--r--   0 xun        (501) staff       (20)     5479 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev8/gravitino/utils/http_client.py
-drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-12 01:16:44.632211 gravitino-0.5.0.dev8/gravitino.egg-info/
--rw-r--r--   0 xun        (501) staff       (20)     5954 2024-05-12 01:16:44.000000 gravitino-0.5.0.dev8/gravitino.egg-info/PKG-INFO
--rw-r--r--   0 xun        (501) staff       (20)     2814 2024-05-12 01:16:44.000000 gravitino-0.5.0.dev8/gravitino.egg-info/SOURCES.txt
--rw-r--r--   0 xun        (501) staff       (20)        1 2024-05-12 01:16:44.000000 gravitino-0.5.0.dev8/gravitino.egg-info/dependency_links.txt
--rw-r--r--   0 xun        (501) staff       (20)       72 2024-05-12 01:16:44.000000 gravitino-0.5.0.dev8/gravitino.egg-info/requires.txt
--rw-r--r--   0 xun        (501) staff       (20)       10 2024-05-12 01:16:44.000000 gravitino-0.5.0.dev8/gravitino.egg-info/top_level.txt
--rw-r--r--   0 xun        (501) staff       (20)       38 2024-05-12 01:16:44.644958 gravitino-0.5.0.dev8/setup.cfg
--rw-r--r--   0 xun        (501) staff       (20)     1109 2024-05-12 01:16:32.000000 gravitino-0.5.0.dev8/setup.py
-drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-12 01:16:44.644490 gravitino-0.5.0.dev8/tests/
--rw-r--r--   0 xun        (501) staff       (20)     2192 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev8/tests/test_gravitino_client.py
+drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-12 09:21:45.029357 gravitino-0.5.0.dev9/
+-rw-r--r--   0 xun        (501) staff       (20)     5954 2024-05-12 09:21:45.029125 gravitino-0.5.0.dev9/PKG-INFO
+-rw-r--r--   0 xun        (501) staff       (20)     5223 2024-05-12 01:16:20.000000 gravitino-0.5.0.dev9/README.md
+drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-12 09:21:45.014140 gravitino-0.5.0.dev9/gravitino/
+-rw-r--r--   0 xun        (501) staff       (20)      649 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev9/gravitino/__init__.py
+drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-12 09:21:45.017824 gravitino-0.5.0.dev9/gravitino/api/
+-rw-r--r--   0 xun        (501) staff       (20)      105 2024-04-13 14:46:55.000000 gravitino-0.5.0.dev9/gravitino/api/__init__.py
+-rw-r--r--   0 xun        (501) staff       (20)      942 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev9/gravitino/api/audit.py
+-rw-r--r--   0 xun        (501) staff       (20)      440 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev9/gravitino/api/auditable.py
+-rw-r--r--   0 xun        (501) staff       (20)     4113 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev9/gravitino/api/catalog.py
+-rw-r--r--   0 xun        (501) staff       (20)     8759 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev9/gravitino/api/catalog_change.py
+-rw-r--r--   0 xun        (501) staff       (20)     3556 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev9/gravitino/api/fileset.py
+-rw-r--r--   0 xun        (501) staff       (20)     9226 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev9/gravitino/api/fileset_change.py
+-rw-r--r--   0 xun        (501) staff       (20)     1155 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev9/gravitino/api/metalake.py
+-rw-r--r--   0 xun        (501) staff       (20)     3403 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev9/gravitino/api/metalake_change.py
+-rw-r--r--   0 xun        (501) staff       (20)     1044 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev9/gravitino/api/schema.py
+-rw-r--r--   0 xun        (501) staff       (20)     4847 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev9/gravitino/api/schema_change.py
+-rw-r--r--   0 xun        (501) staff       (20)     3870 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev9/gravitino/api/supports_schemas.py
+drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-12 09:21:45.018482 gravitino-0.5.0.dev9/gravitino/catalog/
+-rw-r--r--   0 xun        (501) staff       (20)      105 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev9/gravitino/catalog/__init__.py
+-rw-r--r--   0 xun        (501) staff       (20)     7055 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev9/gravitino/catalog/base_schema_catalog.py
+-rw-r--r--   0 xun        (501) staff       (20)     7323 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev9/gravitino/catalog/fileset_catalog.py
+drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-12 09:21:45.019851 gravitino-0.5.0.dev9/gravitino/client/
+-rw-r--r--   0 xun        (501) staff       (20)      105 2024-04-11 14:36:22.000000 gravitino-0.5.0.dev9/gravitino/client/__init__.py
+-rw-r--r--   0 xun        (501) staff       (20)     4651 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev9/gravitino/client/gravitino_admin_client.py
+-rw-r--r--   0 xun        (501) staff       (20)     2739 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev9/gravitino/client/gravitino_client.py
+-rw-r--r--   0 xun        (501) staff       (20)     2483 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev9/gravitino/client/gravitino_client_base.py
+-rw-r--r--   0 xun        (501) staff       (20)     7664 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev9/gravitino/client/gravitino_metalake.py
+-rw-r--r--   0 xun        (501) staff       (20)      408 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev9/gravitino/client/gravitino_version.py
+-rw-r--r--   0 xun        (501) staff       (20)      119 2024-04-02 06:05:04.000000 gravitino-0.5.0.dev9/gravitino/constants.py
+drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-12 09:21:45.021908 gravitino-0.5.0.dev9/gravitino/dto/
+-rw-r--r--   0 xun        (501) staff       (20)      105 2024-04-11 14:36:22.000000 gravitino-0.5.0.dev9/gravitino/dto/__init__.py
+-rw-r--r--   0 xun        (501) staff       (20)     1753 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev9/gravitino/dto/audit_dto.py
+-rw-r--r--   0 xun        (501) staff       (20)     1590 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev9/gravitino/dto/catalog_dto.py
+-rw-r--r--   0 xun        (501) staff       (20)     3019 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev9/gravitino/dto/dto_converters.py
+-rw-r--r--   0 xun        (501) staff       (20)     1313 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev9/gravitino/dto/fileset_dto.py
+-rw-r--r--   0 xun        (501) staff       (20)     1883 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev9/gravitino/dto/metalake_dto.py
+drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-12 09:21:45.024102 gravitino-0.5.0.dev9/gravitino/dto/requests/
+-rw-r--r--   0 xun        (501) staff       (20)      105 2024-04-11 14:36:22.000000 gravitino-0.5.0.dev9/gravitino/dto/requests/__init__.py
+-rw-r--r--   0 xun        (501) staff       (20)     1560 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev9/gravitino/dto/requests/catalog_create_request.py
+-rw-r--r--   0 xun        (501) staff       (20)     2534 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev9/gravitino/dto/requests/catalog_update_request.py
+-rw-r--r--   0 xun        (501) staff       (20)     1065 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev9/gravitino/dto/requests/catalog_updates_request.py
+-rw-r--r--   0 xun        (501) staff       (20)     1438 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev9/gravitino/dto/requests/fileset_create_request.py
+-rw-r--r--   0 xun        (501) staff       (20)     4267 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev9/gravitino/dto/requests/fileset_update_request.py
+-rw-r--r--   0 xun        (501) staff       (20)      750 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev9/gravitino/dto/requests/fileset_updates_request.py
+-rw-r--r--   0 xun        (501) staff       (20)     1070 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev9/gravitino/dto/requests/metalake_create_request.py
+-rw-r--r--   0 xun        (501) staff       (20)     4145 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev9/gravitino/dto/requests/metalake_update_request.py
+-rw-r--r--   0 xun        (501) staff       (20)     1029 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev9/gravitino/dto/requests/metalake_updates_request.py
+-rw-r--r--   0 xun        (501) staff       (20)      908 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev9/gravitino/dto/requests/schema_create_request.py
+-rw-r--r--   0 xun        (501) staff       (20)     2519 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev9/gravitino/dto/requests/schema_update_request.py
+-rw-r--r--   0 xun        (501) staff       (20)      990 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev9/gravitino/dto/requests/schema_updates_request.py
+drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-12 09:21:45.025785 gravitino-0.5.0.dev9/gravitino/dto/responses/
+-rw-r--r--   0 xun        (501) staff       (20)      105 2024-04-11 14:36:22.000000 gravitino-0.5.0.dev9/gravitino/dto/responses/__init__.py
+-rw-r--r--   0 xun        (501) staff       (20)      683 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev9/gravitino/dto/responses/base_response.py
+-rw-r--r--   0 xun        (501) staff       (20)      573 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev9/gravitino/dto/responses/catalog_list_response.py
+-rw-r--r--   0 xun        (501) staff       (20)     1051 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev9/gravitino/dto/responses/catalog_response.py
+-rw-r--r--   0 xun        (501) staff       (20)      476 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev9/gravitino/dto/responses/drop_response.py
+-rw-r--r--   0 xun        (501) staff       (20)      871 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev9/gravitino/dto/responses/entity_list_response.py
+-rw-r--r--   0 xun        (501) staff       (20)     1061 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev9/gravitino/dto/responses/fileset_response.py
+-rw-r--r--   0 xun        (501) staff       (20)     1162 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev9/gravitino/dto/responses/metalake_list_response.py
+-rw-r--r--   0 xun        (501) staff       (20)     1063 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev9/gravitino/dto/responses/metalake_response.py
+-rw-r--r--   0 xun        (501) staff       (20)     1058 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev9/gravitino/dto/responses/schema_response.py
+-rw-r--r--   0 xun        (501) staff       (20)     1382 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev9/gravitino/dto/schema_dto.py
+-rw-r--r--   0 xun        (501) staff       (20)      431 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev9/gravitino/dto/version_dto.py
+drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-12 09:21:45.027381 gravitino-0.5.0.dev9/gravitino/exceptions/
+-rw-r--r--   0 xun        (501) staff       (20)      105 2024-04-11 14:36:22.000000 gravitino-0.5.0.dev9/gravitino/exceptions/__init__.py
+-rw-r--r--   0 xun        (501) staff       (20)      302 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev9/gravitino/exceptions/gravitino_runtime_exception.py
+-rw-r--r--   0 xun        (501) staff       (20)      363 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev9/gravitino/exceptions/illegal_name_identifier_exception.py
+-rw-r--r--   0 xun        (501) staff       (20)      352 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev9/gravitino/exceptions/illegal_namespace_exception.py
+-rw-r--r--   0 xun        (501) staff       (20)      288 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev9/gravitino/exceptions/no_such_metalake_exception.py
+-rw-r--r--   0 xun        (501) staff       (20)      323 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev9/gravitino/exceptions/not_found_exception.py
+-rw-r--r--   0 xun        (501) staff       (20)      105 2024-04-02 06:05:04.000000 gravitino-0.5.0.dev9/gravitino/exceptions.py
+-rw-r--r--   0 xun        (501) staff       (20)     4404 2024-04-02 06:05:04.000000 gravitino-0.5.0.dev9/gravitino/gravitino_client.py
+-rw-r--r--   0 xun        (501) staff       (20)     9268 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev9/gravitino/name_identifier.py
+-rw-r--r--   0 xun        (501) staff       (20)     7603 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev9/gravitino/namespace.py
+drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-12 09:21:45.027760 gravitino-0.5.0.dev9/gravitino/rest/
+-rw-r--r--   0 xun        (501) staff       (20)      105 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev9/gravitino/rest/__init__.py
+-rw-r--r--   0 xun        (501) staff       (20)     1198 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev9/gravitino/rest/rest_message.py
+-rw-r--r--   0 xun        (501) staff       (20)     2430 2024-04-02 06:05:04.000000 gravitino-0.5.0.dev9/gravitino/service.py
+-rw-r--r--   0 xun        (501) staff       (20)      318 2024-04-02 06:05:04.000000 gravitino-0.5.0.dev9/gravitino/typing.py
+drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-12 09:21:45.028477 gravitino-0.5.0.dev9/gravitino/utils/
+-rw-r--r--   0 xun        (501) staff       (20)      175 2024-04-02 06:05:04.000000 gravitino-0.5.0.dev9/gravitino/utils/__init__.py
+-rw-r--r--   0 xun        (501) staff       (20)     2692 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev9/gravitino/utils/exceptions.py
+-rw-r--r--   0 xun        (501) staff       (20)     5479 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev9/gravitino/utils/http_client.py
+drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-12 09:21:45.014840 gravitino-0.5.0.dev9/gravitino.egg-info/
+-rw-r--r--   0 xun        (501) staff       (20)     5954 2024-05-12 09:21:44.000000 gravitino-0.5.0.dev9/gravitino.egg-info/PKG-INFO
+-rw-r--r--   0 xun        (501) staff       (20)     2814 2024-05-12 09:21:44.000000 gravitino-0.5.0.dev9/gravitino.egg-info/SOURCES.txt
+-rw-r--r--   0 xun        (501) staff       (20)        1 2024-05-12 09:21:44.000000 gravitino-0.5.0.dev9/gravitino.egg-info/dependency_links.txt
+-rw-r--r--   0 xun        (501) staff       (20)       72 2024-05-12 09:21:44.000000 gravitino-0.5.0.dev9/gravitino.egg-info/requires.txt
+-rw-r--r--   0 xun        (501) staff       (20)       10 2024-05-12 09:21:44.000000 gravitino-0.5.0.dev9/gravitino.egg-info/top_level.txt
+-rw-r--r--   0 xun        (501) staff       (20)       38 2024-05-12 09:21:45.029600 gravitino-0.5.0.dev9/setup.cfg
+-rw-r--r--   0 xun        (501) staff       (20)     1109 2024-05-12 09:21:34.000000 gravitino-0.5.0.dev9/setup.py
+drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-12 09:21:45.028688 gravitino-0.5.0.dev9/tests/
+-rw-r--r--   0 xun        (501) staff       (20)     2192 2024-05-11 06:59:15.000000 gravitino-0.5.0.dev9/tests/test_gravitino_client.py
```

### Comparing `gravitino-0.5.0.dev8/PKG-INFO` & `gravitino-0.5.0.dev9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gravitino
-Version: 0.5.0.dev8
+Version: 0.5.0.dev9
 Summary: Python lib/client for Gravitino
 Home-page: https://github.com/datastrato/gravitino
 Author: datastrato
 Author-email: support@datastrato.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `gravitino-0.5.0.dev8/README.md` & `gravitino-0.5.0.dev9/README.md`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev8/gravitino/__init__.py` & `gravitino-0.5.0.dev9/gravitino/__init__.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev8/gravitino/api/audit.py` & `gravitino-0.5.0.dev9/gravitino/api/audit.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev8/gravitino/api/catalog.py` & `gravitino-0.5.0.dev9/gravitino/api/catalog.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev8/gravitino/api/catalog_change.py` & `gravitino-0.5.0.dev9/gravitino/api/catalog_change.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev8/gravitino/api/fileset.py` & `gravitino-0.5.0.dev9/gravitino/api/fileset.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev8/gravitino/api/fileset_change.py` & `gravitino-0.5.0.dev9/gravitino/api/fileset_change.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev8/gravitino/api/metalake.py` & `gravitino-0.5.0.dev9/gravitino/api/metalake.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev8/gravitino/api/metalake_change.py` & `gravitino-0.5.0.dev9/gravitino/api/metalake_change.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev8/gravitino/api/schema.py` & `gravitino-0.5.0.dev9/gravitino/api/schema.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev8/gravitino/api/schema_change.py` & `gravitino-0.5.0.dev9/gravitino/api/schema_change.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev8/gravitino/api/supports_schemas.py` & `gravitino-0.5.0.dev9/gravitino/api/supports_schemas.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev8/gravitino/catalog/base_schema_catalog.py` & `gravitino-0.5.0.dev9/gravitino/catalog/base_schema_catalog.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev8/gravitino/catalog/fileset_catalog.py` & `gravitino-0.5.0.dev9/gravitino/catalog/fileset_catalog.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev8/gravitino/client/gravitino_admin_client.py` & `gravitino-0.5.0.dev9/gravitino/client/gravitino_admin_client.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev8/gravitino/client/gravitino_client.py` & `gravitino-0.5.0.dev9/gravitino/client/gravitino_client.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev8/gravitino/client/gravitino_client_base.py` & `gravitino-0.5.0.dev9/gravitino/client/gravitino_client_base.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev8/gravitino/client/gravitino_metalake.py` & `gravitino-0.5.0.dev9/gravitino/client/gravitino_metalake.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev8/gravitino/dto/audit_dto.py` & `gravitino-0.5.0.dev9/gravitino/dto/audit_dto.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev8/gravitino/dto/catalog_dto.py` & `gravitino-0.5.0.dev9/gravitino/dto/catalog_dto.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev8/gravitino/dto/dto_converters.py` & `gravitino-0.5.0.dev9/gravitino/dto/dto_converters.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev8/gravitino/dto/fileset_dto.py` & `gravitino-0.5.0.dev9/gravitino/dto/fileset_dto.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev8/gravitino/dto/metalake_dto.py` & `gravitino-0.5.0.dev9/gravitino/dto/metalake_dto.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev8/gravitino/dto/requests/catalog_create_request.py` & `gravitino-0.5.0.dev9/gravitino/dto/requests/catalog_create_request.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev8/gravitino/dto/requests/catalog_update_request.py` & `gravitino-0.5.0.dev9/gravitino/dto/requests/catalog_update_request.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev8/gravitino/dto/requests/catalog_updates_request.py` & `gravitino-0.5.0.dev9/gravitino/dto/requests/catalog_updates_request.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev8/gravitino/dto/requests/fileset_create_request.py` & `gravitino-0.5.0.dev9/gravitino/dto/requests/fileset_create_request.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev8/gravitino/dto/requests/fileset_update_request.py` & `gravitino-0.5.0.dev9/gravitino/dto/requests/fileset_update_request.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev8/gravitino/dto/requests/fileset_updates_request.py` & `gravitino-0.5.0.dev9/gravitino/dto/requests/fileset_updates_request.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev8/gravitino/dto/requests/metalake_create_request.py` & `gravitino-0.5.0.dev9/gravitino/dto/requests/metalake_create_request.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev8/gravitino/dto/requests/metalake_update_request.py` & `gravitino-0.5.0.dev9/gravitino/dto/requests/metalake_update_request.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev8/gravitino/dto/requests/metalake_updates_request.py` & `gravitino-0.5.0.dev9/gravitino/dto/requests/metalake_updates_request.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev8/gravitino/dto/requests/schema_create_request.py` & `gravitino-0.5.0.dev9/gravitino/dto/requests/schema_create_request.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev8/gravitino/dto/requests/schema_update_request.py` & `gravitino-0.5.0.dev9/gravitino/dto/requests/schema_update_request.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev8/gravitino/dto/requests/schema_updates_request.py` & `gravitino-0.5.0.dev9/gravitino/dto/requests/schema_updates_request.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev8/gravitino/dto/responses/base_response.py` & `gravitino-0.5.0.dev9/gravitino/dto/responses/base_response.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev8/gravitino/dto/responses/catalog_list_response.py` & `gravitino-0.5.0.dev9/gravitino/dto/responses/catalog_list_response.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev8/gravitino/dto/responses/catalog_response.py` & `gravitino-0.5.0.dev9/gravitino/dto/responses/catalog_response.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev8/gravitino/dto/responses/entity_list_response.py` & `gravitino-0.5.0.dev9/gravitino/dto/responses/entity_list_response.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev8/gravitino/dto/responses/fileset_response.py` & `gravitino-0.5.0.dev9/gravitino/dto/responses/fileset_response.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev8/gravitino/dto/responses/metalake_list_response.py` & `gravitino-0.5.0.dev9/gravitino/dto/responses/metalake_list_response.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev8/gravitino/dto/responses/metalake_response.py` & `gravitino-0.5.0.dev9/gravitino/dto/responses/metalake_response.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev8/gravitino/dto/responses/schema_response.py` & `gravitino-0.5.0.dev9/gravitino/dto/responses/schema_response.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev8/gravitino/dto/schema_dto.py` & `gravitino-0.5.0.dev9/gravitino/dto/schema_dto.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev8/gravitino/gravitino_client.py` & `gravitino-0.5.0.dev9/gravitino/gravitino_client.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev8/gravitino/name_identifier.py` & `gravitino-0.5.0.dev9/gravitino/name_identifier.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev8/gravitino/namespace.py` & `gravitino-0.5.0.dev9/gravitino/namespace.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev8/gravitino/rest/rest_message.py` & `gravitino-0.5.0.dev9/gravitino/rest/rest_message.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev8/gravitino/service.py` & `gravitino-0.5.0.dev9/gravitino/service.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev8/gravitino/utils/exceptions.py` & `gravitino-0.5.0.dev9/gravitino/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev8/gravitino/utils/http_client.py` & `gravitino-0.5.0.dev9/gravitino/utils/http_client.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev8/gravitino.egg-info/PKG-INFO` & `gravitino-0.5.0.dev9/gravitino.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gravitino
-Version: 0.5.0.dev8
+Version: 0.5.0.dev9
 Summary: Python lib/client for Gravitino
 Home-page: https://github.com/datastrato/gravitino
 Author: datastrato
 Author-email: support@datastrato.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `gravitino-0.5.0.dev8/gravitino.egg-info/SOURCES.txt` & `gravitino-0.5.0.dev9/gravitino.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev8/setup.py` & `gravitino-0.5.0.dev9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from setuptools import find_packages, setup
 
 
 setup(
     name="gravitino",
     description="Python lib/client for Gravitino",
-    version="0.5.0.dev8",
+    version="0.5.0.dev9",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/datastrato/gravitino",
     author="datastrato",
     author_email="support@datastrato.com",
     python_requires=">=3.8",
     packages=find_packages(exclude=["tests*"]),
```

### Comparing `gravitino-0.5.0.dev8/tests/test_gravitino_client.py` & `gravitino-0.5.0.dev9/tests/test_gravitino_client.py`

 * *Files identical despite different names*

