# Comparing `tmp/otf-addons-aws-24.9.0.tar.gz` & `tmp/otf-addons-aws-24.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "otf-addons-aws-24.9.0.tar", last modified: Sat Mar  2 23:07:32 2024, max compression
+gzip compressed data, was "otf-addons-aws-24.9.1.tar", last modified: Sun Mar  3 00:08:11 2024, max compression
```

## Comparing `otf-addons-aws-24.9.0.tar` & `otf-addons-aws-24.9.1.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-03-02 23:07:32.713754 otf-addons-aws-24.9.0/
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)       72 2024-01-28 12:07:31.000000 otf-addons-aws-24.9.0/AUTHORS
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)    35149 2024-01-28 12:07:31.000000 otf-addons-aws-24.9.0/LICENSE
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)       44 2024-01-28 12:07:31.000000 otf-addons-aws-24.9.0/MANIFEST.in
--rw-r--r--   0 vscode    (1000) vscode    (1000)     7066 2024-03-02 23:07:32.713754 otf-addons-aws-24.9.0/PKG-INFO
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     5278 2024-01-28 12:07:31.000000 otf-addons-aws-24.9.0/README.md
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)    14820 2024-03-02 23:03:34.000000 otf-addons-aws-24.9.0/pyproject.toml
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)       38 2024-03-02 23:07:32.713754 otf-addons-aws-24.9.0/setup.cfg
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-03-02 23:07:32.693754 otf-addons-aws-24.9.0/src/
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-03-02 23:07:32.689754 otf-addons-aws-24.9.0/src/opentaskpy/
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-03-02 23:07:32.685754 otf-addons-aws-24.9.0/src/opentaskpy/addons/
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-03-02 23:07:32.697754 otf-addons-aws-24.9.0/src/opentaskpy/addons/aws/
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)        0 2024-01-28 12:07:31.000000 otf-addons-aws-24.9.0/src/opentaskpy/addons/aws/__init__.py
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-03-02 23:07:32.701754 otf-addons-aws-24.9.0/src/opentaskpy/addons/aws/remotehandlers/
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)        0 2024-01-28 12:07:31.000000 otf-addons-aws-24.9.0/src/opentaskpy/addons/aws/remotehandlers/__init__.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1123 2024-01-28 12:07:31.000000 otf-addons-aws-24.9.0/src/opentaskpy/addons/aws/remotehandlers/creds.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)    10416 2024-03-02 23:03:16.000000 otf-addons-aws-24.9.0/src/opentaskpy/addons/aws/remotehandlers/ecsfargate.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     6043 2024-03-02 23:03:17.000000 otf-addons-aws-24.9.0/src/opentaskpy/addons/aws/remotehandlers/lambda.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)    20131 2024-03-02 23:03:17.000000 otf-addons-aws-24.9.0/src/opentaskpy/addons/aws/remotehandlers/s3.py
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-03-02 23:07:32.685754 otf-addons-aws-24.9.0/src/opentaskpy/addons/aws/remotehandlers/schemas/
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-03-02 23:07:32.685754 otf-addons-aws-24.9.0/src/opentaskpy/addons/aws/remotehandlers/schemas/execution/
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-03-02 23:07:32.701754 otf-addons-aws-24.9.0/src/opentaskpy/addons/aws/remotehandlers/schemas/execution/ecsfargate/
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      755 2024-01-28 12:07:31.000000 otf-addons-aws-24.9.0/src/opentaskpy/addons/aws/remotehandlers/schemas/execution/ecsfargate/containerOverrides.json
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      850 2024-01-28 12:07:31.000000 otf-addons-aws-24.9.0/src/opentaskpy/addons/aws/remotehandlers/schemas/execution/ecsfargate/ecsfargate.json
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      482 2024-01-28 12:07:31.000000 otf-addons-aws-24.9.0/src/opentaskpy/addons/aws/remotehandlers/schemas/execution/ecsfargate/network.json
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      918 2024-01-28 12:07:31.000000 otf-addons-aws-24.9.0/src/opentaskpy/addons/aws/remotehandlers/schemas/execution/ecsfargate/protocol.json
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-03-02 23:07:32.701754 otf-addons-aws-24.9.0/src/opentaskpy/addons/aws/remotehandlers/schemas/execution/lambda/
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      572 2024-01-28 12:07:31.000000 otf-addons-aws-24.9.0/src/opentaskpy/addons/aws/remotehandlers/schemas/execution/lambda/lambda.json
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      889 2024-01-28 12:07:31.000000 otf-addons-aws-24.9.0/src/opentaskpy/addons/aws/remotehandlers/schemas/execution/lambda/protocol.json
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-03-02 23:07:32.701754 otf-addons-aws-24.9.0/src/opentaskpy/addons/aws/remotehandlers/schemas/execution/s3/
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      885 2024-01-28 12:07:31.000000 otf-addons-aws-24.9.0/src/opentaskpy/addons/aws/remotehandlers/schemas/execution/s3/protocol.json
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      459 2024-01-28 12:07:31.000000 otf-addons-aws-24.9.0/src/opentaskpy/addons/aws/remotehandlers/schemas/execution/s3/s3.json
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-03-02 23:07:32.705754 otf-addons-aws-24.9.0/src/opentaskpy/addons/aws/remotehandlers/schemas/transfer/
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-03-02 23:07:32.705754 otf-addons-aws-24.9.0/src/opentaskpy/addons/aws/remotehandlers/schemas/transfer/s3_destination/
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      279 2024-01-28 12:07:31.000000 otf-addons-aws-24.9.0/src/opentaskpy/addons/aws/remotehandlers/schemas/transfer/s3_destination/flags.json
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      887 2024-01-28 12:07:31.000000 otf-addons-aws-24.9.0/src/opentaskpy/addons/aws/remotehandlers/schemas/transfer/s3_destination/protocol.json
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      570 2024-01-28 12:16:33.000000 otf-addons-aws-24.9.0/src/opentaskpy/addons/aws/remotehandlers/schemas/transfer/s3_destination.json
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-03-02 23:07:32.705754 otf-addons-aws-24.9.0/src/opentaskpy/addons/aws/remotehandlers/schemas/transfer/s3_source/
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      398 2024-01-28 12:07:31.000000 otf-addons-aws-24.9.0/src/opentaskpy/addons/aws/remotehandlers/schemas/transfer/s3_source/fileWatch.json
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1236 2024-01-28 12:07:31.000000 otf-addons-aws-24.9.0/src/opentaskpy/addons/aws/remotehandlers/schemas/transfer/s3_source/postCopyAction.json
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      882 2024-01-28 12:07:31.000000 otf-addons-aws-24.9.0/src/opentaskpy/addons/aws/remotehandlers/schemas/transfer/s3_source/protocol.json
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      663 2024-01-28 12:07:31.000000 otf-addons-aws-24.9.0/src/opentaskpy/addons/aws/remotehandlers/schemas/transfer/s3_source.json
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-03-02 23:07:32.689754 otf-addons-aws-24.9.0/src/opentaskpy/plugins/
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-03-02 23:07:32.693754 otf-addons-aws-24.9.0/src/opentaskpy/plugins/lookup/
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-03-02 23:07:32.705754 otf-addons-aws-24.9.0/src/opentaskpy/plugins/lookup/aws/
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     3190 2024-02-22 12:23:59.000000 otf-addons-aws-24.9.0/src/opentaskpy/plugins/lookup/aws/ssm.py
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-03-02 23:07:32.709754 otf-addons-aws-24.9.0/src/otf_addons_aws.egg-info/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     7066 2024-03-02 23:07:32.000000 otf-addons-aws-24.9.0/src/otf_addons_aws.egg-info/PKG-INFO
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     2153 2024-03-02 23:07:32.000000 otf-addons-aws-24.9.0/src/otf_addons_aws.egg-info/SOURCES.txt
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)        1 2024-03-02 23:07:32.000000 otf-addons-aws-24.9.0/src/otf_addons_aws.egg-info/dependency_links.txt
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      261 2024-03-02 23:07:32.000000 otf-addons-aws-24.9.0/src/otf_addons_aws.egg-info/requires.txt
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)       11 2024-03-02 23:07:32.000000 otf-addons-aws-24.9.0/src/otf_addons_aws.egg-info/top_level.txt
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-03-02 23:07:32.709754 otf-addons-aws-24.9.0/tests/
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1209 2024-01-28 12:07:31.000000 otf-addons-aws-24.9.0/tests/test_ecs_execution_schema_validate.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      670 2024-01-28 12:07:31.000000 otf-addons-aws-24.9.0/tests/test_lambda_execution_schema_validate.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     2514 2024-02-22 12:23:59.000000 otf-addons-aws-24.9.0/tests/test_plugin_ssm.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     6039 2024-01-28 12:07:31.000000 otf-addons-aws-24.9.0/tests/test_remotehandler_ecsfargate_execution.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)    11191 2024-01-28 12:07:31.000000 otf-addons-aws-24.9.0/tests/test_remotehandler_lambda_execution.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1893 2024-01-28 12:07:31.000000 otf-addons-aws-24.9.0/tests/test_remotehandler_s3_execution.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)    24281 2024-03-02 23:03:17.000000 otf-addons-aws-24.9.0/tests/test_remotehandler_s3_transfer.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     4113 2024-01-28 12:07:31.000000 otf-addons-aws-24.9.0/tests/test_s3_source_schema_validate.py
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-03-03 00:08:10.995744 otf-addons-aws-24.9.1/
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)       72 2024-01-28 12:07:31.000000 otf-addons-aws-24.9.1/AUTHORS
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)    35149 2024-01-28 12:07:31.000000 otf-addons-aws-24.9.1/LICENSE
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)       44 2024-01-28 12:07:31.000000 otf-addons-aws-24.9.1/MANIFEST.in
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     7066 2024-03-03 00:08:10.995744 otf-addons-aws-24.9.1/PKG-INFO
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     5278 2024-01-28 12:07:31.000000 otf-addons-aws-24.9.1/README.md
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)    14820 2024-03-03 00:07:28.000000 otf-addons-aws-24.9.1/pyproject.toml
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)       38 2024-03-03 00:08:10.995744 otf-addons-aws-24.9.1/setup.cfg
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-03-03 00:08:10.963744 otf-addons-aws-24.9.1/src/
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-03-03 00:08:10.963744 otf-addons-aws-24.9.1/src/opentaskpy/
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-03-03 00:08:10.963744 otf-addons-aws-24.9.1/src/opentaskpy/addons/
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-03-03 00:08:10.967744 otf-addons-aws-24.9.1/src/opentaskpy/addons/aws/
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)        0 2024-01-28 12:07:31.000000 otf-addons-aws-24.9.1/src/opentaskpy/addons/aws/__init__.py
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-03-03 00:08:10.967744 otf-addons-aws-24.9.1/src/opentaskpy/addons/aws/remotehandlers/
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)        0 2024-01-28 12:07:31.000000 otf-addons-aws-24.9.1/src/opentaskpy/addons/aws/remotehandlers/__init__.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1123 2024-01-28 12:07:31.000000 otf-addons-aws-24.9.1/src/opentaskpy/addons/aws/remotehandlers/creds.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)    10416 2024-03-02 23:52:26.000000 otf-addons-aws-24.9.1/src/opentaskpy/addons/aws/remotehandlers/ecsfargate.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     6043 2024-03-02 23:52:26.000000 otf-addons-aws-24.9.1/src/opentaskpy/addons/aws/remotehandlers/lambda.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)    20559 2024-03-02 23:52:29.000000 otf-addons-aws-24.9.1/src/opentaskpy/addons/aws/remotehandlers/s3.py
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-03-03 00:08:10.963744 otf-addons-aws-24.9.1/src/opentaskpy/addons/aws/remotehandlers/schemas/
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-03-03 00:08:10.963744 otf-addons-aws-24.9.1/src/opentaskpy/addons/aws/remotehandlers/schemas/execution/
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-03-03 00:08:10.971744 otf-addons-aws-24.9.1/src/opentaskpy/addons/aws/remotehandlers/schemas/execution/ecsfargate/
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      755 2024-01-28 12:07:31.000000 otf-addons-aws-24.9.1/src/opentaskpy/addons/aws/remotehandlers/schemas/execution/ecsfargate/containerOverrides.json
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      850 2024-01-28 12:07:31.000000 otf-addons-aws-24.9.1/src/opentaskpy/addons/aws/remotehandlers/schemas/execution/ecsfargate/ecsfargate.json
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      482 2024-01-28 12:07:31.000000 otf-addons-aws-24.9.1/src/opentaskpy/addons/aws/remotehandlers/schemas/execution/ecsfargate/network.json
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      918 2024-01-28 12:07:31.000000 otf-addons-aws-24.9.1/src/opentaskpy/addons/aws/remotehandlers/schemas/execution/ecsfargate/protocol.json
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-03-03 00:08:10.971744 otf-addons-aws-24.9.1/src/opentaskpy/addons/aws/remotehandlers/schemas/execution/lambda/
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      572 2024-01-28 12:07:31.000000 otf-addons-aws-24.9.1/src/opentaskpy/addons/aws/remotehandlers/schemas/execution/lambda/lambda.json
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      889 2024-01-28 12:07:31.000000 otf-addons-aws-24.9.1/src/opentaskpy/addons/aws/remotehandlers/schemas/execution/lambda/protocol.json
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-03-03 00:08:10.971744 otf-addons-aws-24.9.1/src/opentaskpy/addons/aws/remotehandlers/schemas/execution/s3/
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      885 2024-01-28 12:07:31.000000 otf-addons-aws-24.9.1/src/opentaskpy/addons/aws/remotehandlers/schemas/execution/s3/protocol.json
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      459 2024-01-28 12:07:31.000000 otf-addons-aws-24.9.1/src/opentaskpy/addons/aws/remotehandlers/schemas/execution/s3/s3.json
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-03-03 00:08:10.971744 otf-addons-aws-24.9.1/src/opentaskpy/addons/aws/remotehandlers/schemas/transfer/
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-03-03 00:08:10.975744 otf-addons-aws-24.9.1/src/opentaskpy/addons/aws/remotehandlers/schemas/transfer/s3_destination/
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      279 2024-01-28 12:07:31.000000 otf-addons-aws-24.9.1/src/opentaskpy/addons/aws/remotehandlers/schemas/transfer/s3_destination/flags.json
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      887 2024-01-28 12:07:31.000000 otf-addons-aws-24.9.1/src/opentaskpy/addons/aws/remotehandlers/schemas/transfer/s3_destination/protocol.json
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      570 2024-01-28 12:16:33.000000 otf-addons-aws-24.9.1/src/opentaskpy/addons/aws/remotehandlers/schemas/transfer/s3_destination.json
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-03-03 00:08:10.975744 otf-addons-aws-24.9.1/src/opentaskpy/addons/aws/remotehandlers/schemas/transfer/s3_source/
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      398 2024-01-28 12:07:31.000000 otf-addons-aws-24.9.1/src/opentaskpy/addons/aws/remotehandlers/schemas/transfer/s3_source/fileWatch.json
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1236 2024-01-28 12:07:31.000000 otf-addons-aws-24.9.1/src/opentaskpy/addons/aws/remotehandlers/schemas/transfer/s3_source/postCopyAction.json
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      882 2024-01-28 12:07:31.000000 otf-addons-aws-24.9.1/src/opentaskpy/addons/aws/remotehandlers/schemas/transfer/s3_source/protocol.json
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      663 2024-01-28 12:07:31.000000 otf-addons-aws-24.9.1/src/opentaskpy/addons/aws/remotehandlers/schemas/transfer/s3_source.json
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-03-03 00:08:10.963744 otf-addons-aws-24.9.1/src/opentaskpy/plugins/
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-03-03 00:08:10.963744 otf-addons-aws-24.9.1/src/opentaskpy/plugins/lookup/
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-03-03 00:08:10.975744 otf-addons-aws-24.9.1/src/opentaskpy/plugins/lookup/aws/
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     3190 2024-02-22 12:23:59.000000 otf-addons-aws-24.9.1/src/opentaskpy/plugins/lookup/aws/ssm.py
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-03-03 00:08:10.991744 otf-addons-aws-24.9.1/src/otf_addons_aws.egg-info/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     7066 2024-03-03 00:08:10.000000 otf-addons-aws-24.9.1/src/otf_addons_aws.egg-info/PKG-INFO
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     2153 2024-03-03 00:08:10.000000 otf-addons-aws-24.9.1/src/otf_addons_aws.egg-info/SOURCES.txt
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)        1 2024-03-03 00:08:10.000000 otf-addons-aws-24.9.1/src/otf_addons_aws.egg-info/dependency_links.txt
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      261 2024-03-03 00:08:10.000000 otf-addons-aws-24.9.1/src/otf_addons_aws.egg-info/requires.txt
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)       11 2024-03-03 00:08:10.000000 otf-addons-aws-24.9.1/src/otf_addons_aws.egg-info/top_level.txt
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-03-03 00:08:10.991744 otf-addons-aws-24.9.1/tests/
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1209 2024-01-28 12:07:31.000000 otf-addons-aws-24.9.1/tests/test_ecs_execution_schema_validate.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      670 2024-01-28 12:07:31.000000 otf-addons-aws-24.9.1/tests/test_lambda_execution_schema_validate.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     2514 2024-02-22 12:23:59.000000 otf-addons-aws-24.9.1/tests/test_plugin_ssm.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     6039 2024-01-28 12:07:31.000000 otf-addons-aws-24.9.1/tests/test_remotehandler_ecsfargate_execution.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)    11191 2024-01-28 12:07:31.000000 otf-addons-aws-24.9.1/tests/test_remotehandler_lambda_execution.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1893 2024-01-28 12:07:31.000000 otf-addons-aws-24.9.1/tests/test_remotehandler_s3_execution.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)    24281 2024-03-02 23:52:26.000000 otf-addons-aws-24.9.1/tests/test_remotehandler_s3_transfer.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     4113 2024-01-28 12:07:31.000000 otf-addons-aws-24.9.1/tests/test_s3_source_schema_validate.py
```

### Comparing `otf-addons-aws-24.9.0/LICENSE` & `otf-addons-aws-24.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `otf-addons-aws-24.9.0/PKG-INFO` & `otf-addons-aws-24.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otf-addons-aws
-Version: 24.9.0
+Version: 24.9.1
 Summary: Addons for opentaskpy, giving it the ability to push/pull via AWS S3, and pull variables from AWS SSM Parameter Store.
 Author-email: Adam McDonagh <adam@elitemonkey.net>
 License: GPLv3
 Project-URL: Homepage, https://github.com/adammcdonagh/otf-addons-aws
 Project-URL: Bug Tracker, https://github.com/adammcdonagh/otf-addons-aws/issues
 Project-URL: Changelog, https://github.com/adammcdonagh/otf-addons-aws/blob/main/CHANGELOG.md
 Keywords: automation,task,framework,aws,s3,ssm,otf
@@ -21,15 +21,15 @@
 Requires-Dist: awscli; extra == "dev"
 Requires-Dist: awscli-local; extra == "dev"
 Requires-Dist: localstack; extra == "dev"
 Requires-Dist: localstack-client; extra == "dev"
 Requires-Dist: pytest-shell; extra == "dev"
 Requires-Dist: types-requests; extra == "dev"
 Requires-Dist: types-python-dateutil; extra == "dev"
-Requires-Dist: black>=23.1.0; extra == "dev"
+Requires-Dist: black>=24.1.1; extra == "dev"
 Requires-Dist: isort; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: bumpver; extra == "dev"
 Requires-Dist: pytest-shell; extra == "dev"
 Requires-Dist: lovely-pytest-docker; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: pylint; extra == "dev"
```

### Comparing `otf-addons-aws-24.9.0/README.md` & `otf-addons-aws-24.9.1/README.md`

 * *Files identical despite different names*

### Comparing `otf-addons-aws-24.9.0/pyproject.toml` & `otf-addons-aws-24.9.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "otf-addons-aws"
-version = "v24.9.0"
+version = "v24.9.1"
 authors = [{ name = "Adam McDonagh", email = "adam@elitemonkey.net" }]
 license = { text = "GPLv3" }
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: POSIX",
 ]
@@ -23,15 +23,15 @@
     "awscli",
     "awscli-local",
     "localstack",
     "localstack-client",
     "pytest-shell",
     "types-requests",
     "types-python-dateutil",
-    "black >= 23.1.0",
+    "black >= 24.1.1",
     "isort",
     "pytest",
     "bumpver",
     "pytest-shell",
     "lovely-pytest-docker",
     "pre-commit",
     "pylint",
@@ -48,15 +48,15 @@
 "Bug Tracker" = "https://github.com/adammcdonagh/otf-addons-aws/issues"
 "Changelog" = "https://github.com/adammcdonagh/otf-addons-aws/blob/main/CHANGELOG.md"
 
 [tool.isort]
 profile = 'black'
 
 [tool.bumpver]
-current_version = "v24.9.0"
+current_version = "v24.9.1"
 version_pattern = "vYY.WW.PATCH[-TAG]"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `otf-addons-aws-24.9.0/src/opentaskpy/addons/aws/remotehandlers/creds.py` & `otf-addons-aws-24.9.1/src/opentaskpy/addons/aws/remotehandlers/creds.py`

 * *Files identical despite different names*

### Comparing `otf-addons-aws-24.9.0/src/opentaskpy/addons/aws/remotehandlers/ecsfargate.py` & `otf-addons-aws-24.9.1/src/opentaskpy/addons/aws/remotehandlers/ecsfargate.py`

 * *Files identical despite different names*

### Comparing `otf-addons-aws-24.9.0/src/opentaskpy/addons/aws/remotehandlers/lambda.py` & `otf-addons-aws-24.9.1/src/opentaskpy/addons/aws/remotehandlers/lambda.py`

 * *Files identical despite different names*

### Comparing `otf-addons-aws-24.9.0/src/opentaskpy/addons/aws/remotehandlers/s3.py` & `otf-addons-aws-24.9.1/src/opentaskpy/addons/aws/remotehandlers/s3.py`

 * *Files 3% similar despite different names*

```diff
@@ -59,26 +59,28 @@
 
         self.get_s3_client()
 
     def check_credential_expiry(self) -> None:
         """Check the expiry of the temporary credentials."""
         if self.temporary_creds_expiry:
             if self.temporary_creds_expiry < datetime.now(tz=tzlocal()):
+                self.logger.info("Renewing temporary credentials")
                 self.get_s3_client()
 
     def get_s3_client(self) -> None:
         """Get the temporary credentials, or just return the client."""
         # If there's an override for endpoint_url in the environment, then use that
         kwargs2 = {}
         if os.environ.get("AWS_ENDPOINT_URL"):
             kwargs2["endpoint_url"] = os.environ.get("AWS_ENDPOINT_URL")
 
         self.sts_client = self.session.client("sts", **kwargs2)
 
         if self.assume_role_arn:
+            self.logger.info(f"Assuming role: {self.assume_role_arn}")
             assumed_role_object = self.sts_client.assume_role(
                 RoleArn=self.assume_role_arn,
                 RoleSessionName=f"OTF{time()}",
             )
             temporary_creds = assumed_role_object["Credentials"]
             # Set the credentials
             self.aws_access_key_id = temporary_creds["AccessKeyId"]
@@ -110,14 +112,15 @@
         """
         # Check that our creds are valid
         self.check_credential_expiry()
 
         # Determine the action to take
         # Delete the files
         if self.spec["postCopyAction"]["action"] == "delete":
+            self.logger.info(f"Deleting files: {files}")
             response = self.s3_client.delete_objects(
                 Bucket=self.spec["bucket"],
                 Delete={
                     "Objects": [{"Key": file} for file in files],
                     "Quiet": True,
                 },
             )
@@ -230,14 +233,18 @@
         if directory:
             kwargs["Prefix"] = directory
         elif "directory" in self.spec and str(self.spec["directory"]):
             kwargs["Prefix"] = str(self.spec["directory"])
 
         remote_files = {}
 
+        self.logger.info(
+            f"Listing files in {self.spec['bucket']} matching {file_pattern}{' in' + (directory or '')}"
+        )
+
         try:  # pylint: disable=too-many-nested-blocks
             while True:
                 # Check that our creds are valid
                 self.check_credential_expiry()
                 response = self.s3_client.list_objects_v2(**kwargs)
 
                 if response["KeyCount"]:
@@ -258,15 +265,15 @@
 
                         if key.startswith("/"):
                             # Make sure that there is no directory in the key
                             # otherwise skip it too as we dont want anything in a subdir
                             # (as directory is not set)
                             continue
 
-                        self.logger.debug(f"Found file: {filename}")
+                        self.logger.info(f"Found file: {filename}")
 
                         # Get the size and modified time
                         file_attr = self.s3_client.head_object(
                             Bucket=self.spec["bucket"], Key=key
                         )
 
                         remote_files[key] = {
@@ -316,15 +323,15 @@
         kwargs = {}
         if self.bucket_owner_full_control:
             kwargs["ACL"] = "bucket-owner-full-control"
 
         for file in files:
             # Strip the directory from the file
             file_name = file.split("/")[-1]
-            self.logger.debug(
+            self.logger.info(
                 f"Transferring file: {file} to s3://{self.spec['bucket']}/{file_name}"
             )
             try:
                 self.s3_client.upload_file(
                     file,
                     self.spec["bucket"],
                     f"{self.spec['directory']}/{file_name}",
@@ -355,15 +362,15 @@
         # Check that our creds are valid
         self.check_credential_expiry()
 
         result = 0
         for file in files:
             # Strip the directory from the file
             file_name = file.split("/")[-1]
-            self.logger.debug(f"Transferring file: {file}")
+            self.logger.info(f"Downloading file: {file}")
             try:
                 self.s3_client.download_file(
                     self.spec["bucket"],
                     file,
                     f"{local_staging_directory}/{file_name}",
                 )
             except Exception as e:  # pylint: disable=broad-exception-caught
@@ -397,15 +404,17 @@
         # Check the remote handler, if it's another S3Transfer, then it's simple
         # to do an S3 copy via boto
 
         result = 0
         for file in files:
             # Strip the directory from the file
             file_name = file.split("/")[-1]
-            self.logger.debug(f"Transferring file: {file}")
+            self.logger.info(
+                f"Transferring file: {file} from {self.spec['bucket']} to {dest_remote_handler.spec['bucket']}"
+            )
             try:
                 self.s3_client.copy(
                     {
                         "Bucket": self.spec["bucket"],
                         "Key": file,
                     },
                     dest_remote_handler.spec["bucket"],
@@ -426,15 +435,15 @@
         """
         # Check that our creds are valid
         self.check_credential_expiry()
 
         result = 0
 
         object_key = self.spec["flags"]["fullPath"]
-        self.logger.debug(f"Creating flag file: {object_key}")
+        self.logger.info(f"Creating flag file: {object_key}")
         kwargs = {
             "Bucket": self.spec["bucket"],
             "Key": object_key,
         }
         if self.bucket_owner_full_control:
             kwargs["ACL"] = "bucket-owner-full-control"
```

### Comparing `otf-addons-aws-24.9.0/src/opentaskpy/addons/aws/remotehandlers/schemas/execution/ecsfargate/containerOverrides.json` & `otf-addons-aws-24.9.1/src/opentaskpy/addons/aws/remotehandlers/schemas/execution/ecsfargate/containerOverrides.json`

 * *Files identical despite different names*

### Comparing `otf-addons-aws-24.9.0/src/opentaskpy/addons/aws/remotehandlers/schemas/execution/ecsfargate/ecsfargate.json` & `otf-addons-aws-24.9.1/src/opentaskpy/addons/aws/remotehandlers/schemas/execution/ecsfargate/ecsfargate.json`

 * *Files identical despite different names*

### Comparing `otf-addons-aws-24.9.0/src/opentaskpy/addons/aws/remotehandlers/schemas/execution/ecsfargate/protocol.json` & `otf-addons-aws-24.9.1/src/opentaskpy/addons/aws/remotehandlers/schemas/execution/ecsfargate/protocol.json`

 * *Files identical despite different names*

### Comparing `otf-addons-aws-24.9.0/src/opentaskpy/addons/aws/remotehandlers/schemas/execution/lambda/lambda.json` & `otf-addons-aws-24.9.1/src/opentaskpy/addons/aws/remotehandlers/schemas/execution/lambda/lambda.json`

 * *Files identical despite different names*

### Comparing `otf-addons-aws-24.9.0/src/opentaskpy/addons/aws/remotehandlers/schemas/execution/lambda/protocol.json` & `otf-addons-aws-24.9.1/src/opentaskpy/addons/aws/remotehandlers/schemas/execution/lambda/protocol.json`

 * *Files identical despite different names*

### Comparing `otf-addons-aws-24.9.0/src/opentaskpy/addons/aws/remotehandlers/schemas/execution/s3/protocol.json` & `otf-addons-aws-24.9.1/src/opentaskpy/addons/aws/remotehandlers/schemas/execution/s3/protocol.json`

 * *Files identical despite different names*

### Comparing `otf-addons-aws-24.9.0/src/opentaskpy/addons/aws/remotehandlers/schemas/transfer/s3_destination/protocol.json` & `otf-addons-aws-24.9.1/src/opentaskpy/addons/aws/remotehandlers/schemas/transfer/s3_destination/protocol.json`

 * *Files identical despite different names*

### Comparing `otf-addons-aws-24.9.0/src/opentaskpy/addons/aws/remotehandlers/schemas/transfer/s3_destination.json` & `otf-addons-aws-24.9.1/src/opentaskpy/addons/aws/remotehandlers/schemas/transfer/s3_destination.json`

 * *Files identical despite different names*

### Comparing `otf-addons-aws-24.9.0/src/opentaskpy/addons/aws/remotehandlers/schemas/transfer/s3_source/postCopyAction.json` & `otf-addons-aws-24.9.1/src/opentaskpy/addons/aws/remotehandlers/schemas/transfer/s3_source/postCopyAction.json`

 * *Files identical despite different names*

### Comparing `otf-addons-aws-24.9.0/src/opentaskpy/addons/aws/remotehandlers/schemas/transfer/s3_source/protocol.json` & `otf-addons-aws-24.9.1/src/opentaskpy/addons/aws/remotehandlers/schemas/transfer/s3_source/protocol.json`

 * *Files identical despite different names*

### Comparing `otf-addons-aws-24.9.0/src/opentaskpy/addons/aws/remotehandlers/schemas/transfer/s3_source.json` & `otf-addons-aws-24.9.1/src/opentaskpy/addons/aws/remotehandlers/schemas/transfer/s3_source.json`

 * *Files identical despite different names*

### Comparing `otf-addons-aws-24.9.0/src/opentaskpy/plugins/lookup/aws/ssm.py` & `otf-addons-aws-24.9.1/src/opentaskpy/plugins/lookup/aws/ssm.py`

 * *Files identical despite different names*

### Comparing `otf-addons-aws-24.9.0/src/otf_addons_aws.egg-info/PKG-INFO` & `otf-addons-aws-24.9.1/src/otf_addons_aws.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otf-addons-aws
-Version: 24.9.0
+Version: 24.9.1
 Summary: Addons for opentaskpy, giving it the ability to push/pull via AWS S3, and pull variables from AWS SSM Parameter Store.
 Author-email: Adam McDonagh <adam@elitemonkey.net>
 License: GPLv3
 Project-URL: Homepage, https://github.com/adammcdonagh/otf-addons-aws
 Project-URL: Bug Tracker, https://github.com/adammcdonagh/otf-addons-aws/issues
 Project-URL: Changelog, https://github.com/adammcdonagh/otf-addons-aws/blob/main/CHANGELOG.md
 Keywords: automation,task,framework,aws,s3,ssm,otf
@@ -21,15 +21,15 @@
 Requires-Dist: awscli; extra == "dev"
 Requires-Dist: awscli-local; extra == "dev"
 Requires-Dist: localstack; extra == "dev"
 Requires-Dist: localstack-client; extra == "dev"
 Requires-Dist: pytest-shell; extra == "dev"
 Requires-Dist: types-requests; extra == "dev"
 Requires-Dist: types-python-dateutil; extra == "dev"
-Requires-Dist: black>=23.1.0; extra == "dev"
+Requires-Dist: black>=24.1.1; extra == "dev"
 Requires-Dist: isort; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: bumpver; extra == "dev"
 Requires-Dist: pytest-shell; extra == "dev"
 Requires-Dist: lovely-pytest-docker; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: pylint; extra == "dev"
```

### Comparing `otf-addons-aws-24.9.0/src/otf_addons_aws.egg-info/SOURCES.txt` & `otf-addons-aws-24.9.1/src/otf_addons_aws.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `otf-addons-aws-24.9.0/tests/test_ecs_execution_schema_validate.py` & `otf-addons-aws-24.9.1/tests/test_ecs_execution_schema_validate.py`

 * *Files identical despite different names*

### Comparing `otf-addons-aws-24.9.0/tests/test_lambda_execution_schema_validate.py` & `otf-addons-aws-24.9.1/tests/test_lambda_execution_schema_validate.py`

 * *Files identical despite different names*

### Comparing `otf-addons-aws-24.9.0/tests/test_plugin_ssm.py` & `otf-addons-aws-24.9.1/tests/test_plugin_ssm.py`

 * *Files identical despite different names*

### Comparing `otf-addons-aws-24.9.0/tests/test_remotehandler_ecsfargate_execution.py` & `otf-addons-aws-24.9.1/tests/test_remotehandler_ecsfargate_execution.py`

 * *Files identical despite different names*

### Comparing `otf-addons-aws-24.9.0/tests/test_remotehandler_lambda_execution.py` & `otf-addons-aws-24.9.1/tests/test_remotehandler_lambda_execution.py`

 * *Files identical despite different names*

### Comparing `otf-addons-aws-24.9.0/tests/test_remotehandler_s3_execution.py` & `otf-addons-aws-24.9.1/tests/test_remotehandler_s3_execution.py`

 * *Files identical despite different names*

### Comparing `otf-addons-aws-24.9.0/tests/test_remotehandler_s3_transfer.py` & `otf-addons-aws-24.9.1/tests/test_remotehandler_s3_transfer.py`

 * *Files identical despite different names*

### Comparing `otf-addons-aws-24.9.0/tests/test_s3_source_schema_validate.py` & `otf-addons-aws-24.9.1/tests/test_s3_source_schema_validate.py`

 * *Files identical despite different names*

