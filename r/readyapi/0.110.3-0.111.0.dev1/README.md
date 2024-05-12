# Comparing `tmp/readyapi-0.110.3.tar.gz` & `tmp/readyapi-0.111.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "readyapi-0.110.3.tar", last modified: Sun May 12 00:38:20 2024, max compression
+gzip compressed data, was "readyapi-0.111.0.dev1.tar", last modified: Sun May 12 05:04:36 2024, max compression
```

## Comparing `readyapi-0.110.3.tar` & `readyapi-0.111.0.dev1.tar`

### file list

```diff
@@ -1,1231 +1,1231 @@
--rw-r--r--   0        0        0     1084 2024-05-12 00:38:13.574838 readyapi-0.110.3/LICENSE
--rw-r--r--   0        0        0    22670 2024-05-12 00:38:13.578838 readyapi-0.110.3/README.md
--rw-r--r--   0        0        0     5043 2024-05-12 00:38:13.610839 readyapi-0.110.3/docs/en/docs/img/favicon.png
--rw-r--r--   0        0        0      510 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/additional_responses/tutorial001.py
--rw-r--r--   0        0        0      632 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/additional_responses/tutorial002.py
--rw-r--r--   0        0        0      841 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/additional_responses/tutorial003.py
--rw-r--r--   0        0        0      705 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/additional_responses/tutorial004.py
--rw-r--r--   0        0        0      688 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/additional_status_codes/tutorial001.py
--rw-r--r--   0        0        0      738 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/additional_status_codes/tutorial001_an.py
--rw-r--r--   0        0        0      690 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/additional_status_codes/tutorial001_an_py310.py
--rw-r--r--   0        0        0      709 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/additional_status_codes/tutorial001_an_py39.py
--rw-r--r--   0        0        0      650 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/additional_status_codes/tutorial001_py310.py
--rw-r--r--   0        0        0      235 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/advanced_middleware/tutorial001.py
--rw-r--r--   0        0        0      283 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/advanced_middleware/tutorial002.py
--rw-r--r--   0        0        0      217 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/advanced_middleware/tutorial003.py
--rw-r--r--   0        0        0        0 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/app_testing/__init__.py
--rw-r--r--   0        0        0        0 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/app_testing/app_b/__init__.py
--rw-r--r--   0        0        0     1148 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/app_testing/app_b/main.py
--rw-r--r--   0        0        0     1867 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/app_testing/app_b/test_main.py
--rw-r--r--   0        0        0        0 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/app_testing/app_b_an/__init__.py
--rw-r--r--   0        0        0     1208 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/app_testing/app_b_an/main.py
--rw-r--r--   0        0        0     1867 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/app_testing/app_b_an/test_main.py
--rw-r--r--   0        0        0        0 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/app_testing/app_b_an_py310/__init__.py
--rw-r--r--   0        0        0     1166 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/app_testing/app_b_an_py310/main.py
--rw-r--r--   0        0        0     1867 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/app_testing/app_b_an_py310/test_main.py
--rw-r--r--   0        0        0        0 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/app_testing/app_b_an_py39/__init__.py
--rw-r--r--   0        0        0     1179 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/app_testing/app_b_an_py39/main.py
--rw-r--r--   0        0        0     1867 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/app_testing/app_b_an_py39/test_main.py
--rw-r--r--   0        0        0        0 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/app_testing/app_b_py310/__init__.py
--rw-r--r--   0        0        0     1116 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/app_testing/app_b_py310/main.py
--rw-r--r--   0        0        0     1867 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/app_testing/app_b_py310/test_main.py
--rw-r--r--   0        0        0      121 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/app_testing/main.py
--rw-r--r--   0        0        0      239 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/app_testing/test_main.py
--rw-r--r--   0        0        0      338 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/app_testing/tutorial001.py
--rw-r--r--   0        0        0      762 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/app_testing/tutorial002.py
--rw-r--r--   0        0        0      532 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/app_testing/tutorial003.py
--rw-r--r--   0        0        0     1418 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/async_sql_databases/tutorial001.py
--rw-r--r--   0        0        0        0 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/async_tests/__init__.py
--rw-r--r--   0        0        0      115 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/async_tests/main.py
--rw-r--r--   0        0        0      306 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/async_tests/test_main.py
--rw-r--r--   0        0        0      522 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/background_tasks/tutorial001.py
--rw-r--r--   0        0        0      678 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/background_tasks/tutorial002.py
--rw-r--r--   0        0        0      728 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/background_tasks/tutorial002_an.py
--rw-r--r--   0        0        0      686 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/background_tasks/tutorial002_an_py310.py
--rw-r--r--   0        0        0      699 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/background_tasks/tutorial002_an_py39.py
--rw-r--r--   0        0        0      646 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/background_tasks/tutorial002_py310.py
--rw-r--r--   0        0        0      192 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/behind_a_proxy/tutorial001.py
--rw-r--r--   0        0        0      211 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/behind_a_proxy/tutorial002.py
--rw-r--r--   0        0        0      408 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/behind_a_proxy/tutorial003.py
--rw-r--r--   0        0        0      440 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/behind_a_proxy/tutorial004.py
--rw-r--r--   0        0        0        0 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/bigger_applications/__init__.py
--rw-r--r--   0        0        0        0 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/bigger_applications/app/__init__.py
--rw-r--r--   0        0        0      370 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/bigger_applications/app/dependencies.py
--rw-r--r--   0        0        0        0 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/bigger_applications/app/internal/__init__.py
--rw-r--r--   0        0        0      148 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/bigger_applications/app/internal/admin.py
--rw-r--r--   0        0        0      555 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/bigger_applications/app/main.py
--rw-r--r--   0        0        0        0 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/bigger_applications/app/routers/__init__.py
--rw-r--r--   0        0        0     1012 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/bigger_applications/app/routers/items.py
--rw-r--r--   0        0        0      408 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/bigger_applications/app/routers/users.py
--rw-r--r--   0        0        0        0 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/bigger_applications/app_an/__init__.py
--rw-r--r--   0        0        0      420 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/bigger_applications/app_an/dependencies.py
--rw-r--r--   0        0        0        0 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/bigger_applications/app_an/internal/__init__.py
--rw-r--r--   0        0        0      148 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/bigger_applications/app_an/internal/admin.py
--rw-r--r--   0        0        0      555 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/bigger_applications/app_an/main.py
--rw-r--r--   0        0        0        0 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/bigger_applications/app_an/routers/__init__.py
--rw-r--r--   0        0        0     1012 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/bigger_applications/app_an/routers/items.py
--rw-r--r--   0        0        0      408 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/bigger_applications/app_an/routers/users.py
--rw-r--r--   0        0        0        0 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/bigger_applications/app_an_py39/__init__.py
--rw-r--r--   0        0        0      410 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/bigger_applications/app_an_py39/dependencies.py
--rw-r--r--   0        0        0        0 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/bigger_applications/app_an_py39/internal/__init__.py
--rw-r--r--   0        0        0      148 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/bigger_applications/app_an_py39/internal/admin.py
--rw-r--r--   0        0        0      555 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/bigger_applications/app_an_py39/main.py
--rw-r--r--   0        0        0        0 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/bigger_applications/app_an_py39/routers/__init__.py
--rw-r--r--   0        0        0     1012 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/bigger_applications/app_an_py39/routers/items.py
--rw-r--r--   0        0        0      408 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/bigger_applications/app_an_py39/routers/users.py
--rw-r--r--   0        0        0      312 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/body/tutorial001.py
--rw-r--r--   0        0        0      274 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/body/tutorial001_py310.py
--rw-r--r--   0        0        0      470 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/body/tutorial002.py
--rw-r--r--   0        0        0      432 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/body/tutorial002_py310.py
--rw-r--r--   0        0        0      365 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/body/tutorial003.py
--rw-r--r--   0        0        0      327 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/body/tutorial003_py310.py
--rw-r--r--   0        0        0      455 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/body/tutorial004.py
--rw-r--r--   0        0        0      411 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/body/tutorial004_py310.py
--rw-r--r--   0        0        0      564 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/body_fields/tutorial001.py
--rw-r--r--   0        0        0      614 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/body_fields/tutorial001_an.py
--rw-r--r--   0        0        0      566 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/body_fields/tutorial001_an_py310.py
--rw-r--r--   0        0        0      585 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/body_fields/tutorial001_an_py39.py
--rw-r--r--   0        0        0      526 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/body_fields/tutorial001_py310.py
--rw-r--r--   0        0        0      599 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/body_multiple_params/tutorial001.py
--rw-r--r--   0        0        0      642 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/body_multiple_params/tutorial001_an.py
--rw-r--r--   0        0        0      582 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/body_multiple_params/tutorial001_an_py310.py
--rw-r--r--   0        0        0      613 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/body_multiple_params/tutorial001_an_py39.py
--rw-r--r--   0        0        0      549 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/body_multiple_params/tutorial001_py310.py
--rw-r--r--   0        0        0      493 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/body_multiple_params/tutorial002.py
--rw-r--r--   0        0        0      449 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/body_multiple_params/tutorial002_py310.py
--rw-r--r--   0        0        0      551 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/body_multiple_params/tutorial003.py
--rw-r--r--   0        0        0      607 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/body_multiple_params/tutorial003_an.py
--rw-r--r--   0        0        0      553 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/body_multiple_params/tutorial003_an_py310.py
--rw-r--r--   0        0        0      578 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/body_multiple_params/tutorial003_an_py39.py
--rw-r--r--   0        0        0      507 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/body_multiple_params/tutorial003_py310.py
--rw-r--r--   0        0        0      656 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/body_multiple_params/tutorial004.py
--rw-r--r--   0        0        0      706 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/body_multiple_params/tutorial004_an.py
--rw-r--r--   0        0        0      646 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/body_multiple_params/tutorial004_an_py310.py
--rw-r--r--   0        0        0      677 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/body_multiple_params/tutorial004_an_py39.py
--rw-r--r--   0        0        0      606 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/body_multiple_params/tutorial004_py310.py
--rw-r--r--   0        0        0      410 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/body_multiple_params/tutorial005.py
--rw-r--r--   0        0        0      460 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/body_multiple_params/tutorial005_an.py
--rw-r--r--   0        0        0      412 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/body_multiple_params/tutorial005_an_py310.py
--rw-r--r--   0        0        0      431 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/body_multiple_params/tutorial005_an_py39.py
--rw-r--r--   0        0        0      372 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/body_multiple_params/tutorial005_py310.py
--rw-r--r--   0        0        0      405 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/body_nested_models/tutorial001.py
--rw-r--r--   0        0        0      367 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/body_nested_models/tutorial001_py310.py
--rw-r--r--   0        0        0      416 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/body_nested_models/tutorial002.py
--rw-r--r--   0        0        0      372 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/body_nested_models/tutorial002_py310.py
--rw-r--r--   0        0        0      410 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/body_nested_models/tutorial002_py39.py
--rw-r--r--   0        0        0      417 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/body_nested_models/tutorial003.py
--rw-r--r--   0        0        0      374 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/body_nested_models/tutorial003_py310.py
--rw-r--r--   0        0        0      412 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/body_nested_models/tutorial003_py39.py
--rw-r--r--   0        0        0      507 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/body_nested_models/tutorial004.py
--rw-r--r--   0        0        0      458 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/body_nested_models/tutorial004_py310.py
--rw-r--r--   0        0        0      502 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/body_nested_models/tutorial004_py39.py
--rw-r--r--   0        0        0      520 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/body_nested_models/tutorial005.py
--rw-r--r--   0        0        0      471 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/body_nested_models/tutorial005_py310.py
--rw-r--r--   0        0        0      515 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/body_nested_models/tutorial005_py39.py
--rw-r--r--   0        0        0      533 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/body_nested_models/tutorial006.py
--rw-r--r--   0        0        0      478 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/body_nested_models/tutorial006_py310.py
--rw-r--r--   0        0        0      522 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/body_nested_models/tutorial006_py39.py
--rw-r--r--   0        0        0      584 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/body_nested_models/tutorial007.py
--rw-r--r--   0        0        0      523 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/body_nested_models/tutorial007_py310.py
--rw-r--r--   0        0        0      573 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/body_nested_models/tutorial007_py39.py
--rw-r--r--   0        0        0      276 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/body_nested_models/tutorial008.py
--rw-r--r--   0        0        0      251 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/body_nested_models/tutorial008_py39.py
--rw-r--r--   0        0        0      182 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/body_nested_models/tutorial009.py
--rw-r--r--   0        0        0      157 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/body_nested_models/tutorial009_py39.py
--rw-r--r--   0        0        0      910 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/body_updates/tutorial001.py
--rw-r--r--   0        0        0      860 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/body_updates/tutorial001_py310.py
--rw-r--r--   0        0        0      904 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/body_updates/tutorial001_py39.py
--rw-r--r--   0        0        0     1064 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/body_updates/tutorial002.py
--rw-r--r--   0        0        0     1014 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/body_updates/tutorial002_py310.py
--rw-r--r--   0        0        0     1058 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/body_updates/tutorial002_py39.py
--rw-r--r--   0        0        0      284 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/conditional_openapi/tutorial001.py
--rw-r--r--   0        0        0      208 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/configure_swagger_ui/tutorial001.py
--rw-r--r--   0        0        0      219 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/configure_swagger_ui/tutorial002.py
--rw-r--r--   0        0        0      204 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/configure_swagger_ui/tutorial003.py
--rw-r--r--   0        0        0      205 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/cookie_params/tutorial001.py
--rw-r--r--   0        0        0      250 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/cookie_params/tutorial001_an.py
--rw-r--r--   0        0        0      208 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/cookie_params/tutorial001_an_py310.py
--rw-r--r--   0        0        0      221 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/cookie_params/tutorial001_an_py39.py
--rw-r--r--   0        0        0      173 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/cookie_params/tutorial001_py310.py
--rw-r--r--   0        0        0      467 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/cors/tutorial001.py
--rw-r--r--   0        0        0     1158 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/custom_docs_ui/tutorial001.py
--rw-r--r--   0        0        0     1180 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/custom_docs_ui/tutorial002.py
--rw-r--r--   0        0        0      977 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/custom_request_and_route/tutorial001.py
--rw-r--r--   0        0        0      937 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/custom_request_and_route/tutorial002.py
--rw-r--r--   0        0        0     1046 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/custom_request_and_route/tutorial003.py
--rw-r--r--   0        0        0      201 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/custom_response/tutorial001.py
--rw-r--r--   0        0        0      219 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/custom_response/tutorial001b.py
--rw-r--r--   0        0        0      356 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/custom_response/tutorial002.py
--rw-r--r--   0        0        0      398 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/custom_response/tutorial003.py
--rw-r--r--   0        0        0      495 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/custom_response/tutorial004.py
--rw-r--r--   0        0        0      190 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/custom_response/tutorial005.py
--rw-r--r--   0        0        0      203 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/custom_response/tutorial006.py
--rw-r--r--   0        0        0      229 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/custom_response/tutorial006b.py
--rw-r--r--   0        0        0      241 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/custom_response/tutorial006c.py
--rw-r--r--   0        0        0      281 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/custom_response/tutorial007.py
--rw-r--r--   0        0        0      364 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/custom_response/tutorial008.py
--rw-r--r--   0        0        0      206 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/custom_response/tutorial009.py
--rw-r--r--   0        0        0      221 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/custom_response/tutorial009b.py
--rw-r--r--   0        0        0      454 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/custom_response/tutorial009c.py
--rw-r--r--   0        0        0      209 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/custom_response/tutorial010.py
--rw-r--r--   0        0        0      315 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/dataclasses/tutorial001.py
--rw-r--r--   0        0        0      555 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/dataclasses/tutorial002.py
--rw-r--r--   0        0        0     1406 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/dataclasses/tutorial003.py
--rw-r--r--   0        0        0      226 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/debugging/tutorial001.py
--rw-r--r--   0        0        0      445 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/dependencies/tutorial001.py
--rw-r--r--   0        0        0      498 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/dependencies/tutorial001_02_an.py
--rw-r--r--   0        0        0      450 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/dependencies/tutorial001_02_an_py310.py
--rw-r--r--   0        0        0      469 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/dependencies/tutorial001_02_an_py39.py
--rw-r--r--   0        0        0      505 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/dependencies/tutorial001_an.py
--rw-r--r--   0        0        0      457 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/dependencies/tutorial001_an_py310.py
--rw-r--r--   0        0        0      476 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/dependencies/tutorial001_an_py39.py
--rw-r--r--   0        0        0      407 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/dependencies/tutorial001_py310.py
--rw-r--r--   0        0        0      659 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/dependencies/tutorial002.py
--rw-r--r--   0        0        0      709 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/dependencies/tutorial002_an.py
--rw-r--r--   0        0        0      667 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/dependencies/tutorial002_an_py310.py
--rw-r--r--   0        0        0      680 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/dependencies/tutorial002_an_py39.py
--rw-r--r--   0        0        0      627 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/dependencies/tutorial002_py310.py
--rw-r--r--   0        0        0      638 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/dependencies/tutorial003.py
--rw-r--r--   0        0        0      700 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/dependencies/tutorial003_an.py
--rw-r--r--   0        0        0      658 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/dependencies/tutorial003_an_py310.py
--rw-r--r--   0        0        0      671 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/dependencies/tutorial003_an_py39.py
--rw-r--r--   0        0        0      606 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/dependencies/tutorial003_py310.py
--rw-r--r--   0        0        0      642 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/dependencies/tutorial004.py
--rw-r--r--   0        0        0      692 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/dependencies/tutorial004_an.py
--rw-r--r--   0        0        0      650 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/dependencies/tutorial004_an_py310.py
--rw-r--r--   0        0        0      663 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/dependencies/tutorial004_an_py39.py
--rw-r--r--   0        0        0      610 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/dependencies/tutorial004_py310.py
--rw-r--r--   0        0        0      489 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/dependencies/tutorial005.py
--rw-r--r--   0        0        0      561 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/dependencies/tutorial005_an.py
--rw-r--r--   0        0        0      513 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/dependencies/tutorial005_an_py310.py
--rw-r--r--   0        0        0      532 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/dependencies/tutorial005_an_py39.py
--rw-r--r--   0        0        0      446 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/dependencies/tutorial005_py310.py
--rw-r--r--   0        0        0      586 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/dependencies/tutorial006.py
--rw-r--r--   0        0        0      646 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/dependencies/tutorial006_an.py
--rw-r--r--   0        0        0      636 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/dependencies/tutorial006_an_py39.py
--rw-r--r--   0        0        0       99 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/dependencies/tutorial007.py
--rw-r--r--   0        0        0      456 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/dependencies/tutorial008.py
--rw-r--r--   0        0        0      532 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/dependencies/tutorial008_an.py
--rw-r--r--   0        0        0      522 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/dependencies/tutorial008_an_py39.py
--rw-r--r--   0        0        0      738 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/dependencies/tutorial008b.py
--rw-r--r--   0        0        0      788 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/dependencies/tutorial008b_an.py
--rw-r--r--   0        0        0      778 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/dependencies/tutorial008b_an_py39.py
--rw-r--r--   0        0        0      663 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/dependencies/tutorial008c.py
--rw-r--r--   0        0        0      713 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/dependencies/tutorial008c_an.py
--rw-r--r--   0        0        0      703 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/dependencies/tutorial008c_an_py39.py
--rw-r--r--   0        0        0      697 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/dependencies/tutorial008d.py
--rw-r--r--   0        0        0      747 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/dependencies/tutorial008d_an.py
--rw-r--r--   0        0        0      737 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/dependencies/tutorial008d_an_py39.py
--rw-r--r--   0        0        0      456 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/dependencies/tutorial009.py
--rw-r--r--   0        0        0      292 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/dependencies/tutorial010.py
--rw-r--r--   0        0        0      507 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/dependencies/tutorial011.py
--rw-r--r--   0        0        0      557 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/dependencies/tutorial011_an.py
--rw-r--r--   0        0        0      547 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/dependencies/tutorial011_an_py39.py
--rw-r--r--   0        0        0      699 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/dependencies/tutorial012.py
--rw-r--r--   0        0        0      759 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/dependencies/tutorial012_an.py
--rw-r--r--   0        0        0      759 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/dependencies/tutorial012_an_py39.py
--rw-r--r--   0        0        0     1526 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/dependency_testing/tutorial001.py
--rw-r--r--   0        0        0     1586 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/dependency_testing/tutorial001_an.py
--rw-r--r--   0        0        0     1532 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/dependency_testing/tutorial001_an_py310.py
--rw-r--r--   0        0        0     1557 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/dependency_testing/tutorial001_an_py39.py
--rw-r--r--   0        0        0     1482 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/dependency_testing/tutorial001_py310.py
--rw-r--r--   0        0        0      465 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/encoder/tutorial001.py
--rw-r--r--   0        0        0      434 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/encoder/tutorial001_py310.py
--rw-r--r--   0        0        0      286 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/events/tutorial001.py
--rw-r--r--   0        0        0      258 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/events/tutorial002.py
--rw-r--r--   0        0        0      573 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/events/tutorial003.py
--rw-r--r--   0        0        0      744 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/extending_openapi/tutorial001.py
--rw-r--r--   0        0        0      833 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/extra_data_types/tutorial001.py
--rw-r--r--   0        0        0      893 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/extra_data_types/tutorial001_an.py
--rw-r--r--   0        0        0      833 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/extra_data_types/tutorial001_an_py310.py
--rw-r--r--   0        0        0      864 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/extra_data_types/tutorial001_an_py39.py
--rw-r--r--   0        0        0      784 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/extra_data_types/tutorial001_py310.py
--rw-r--r--   0        0        0      946 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/extra_models/tutorial001.py
--rw-r--r--   0        0        0      902 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/extra_models/tutorial001_py310.py
--rw-r--r--   0        0        0      827 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/extra_models/tutorial002.py
--rw-r--r--   0        0        0      795 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/extra_models/tutorial002_py310.py
--rw-r--r--   0        0        0      647 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/extra_models/tutorial003.py
--rw-r--r--   0        0        0      647 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/extra_models/tutorial003_py310.py
--rw-r--r--   0        0        0      384 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/extra_models/tutorial004.py
--rw-r--r--   0        0        0      359 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/extra_models/tutorial004_py39.py
--rw-r--r--   0        0        0      208 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/extra_models/tutorial005.py
--rw-r--r--   0        0        0      183 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/extra_models/tutorial005_py39.py
--rw-r--r--   0        0        0      120 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/first_steps/tutorial001.py
--rw-r--r--   0        0        0      142 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/first_steps/tutorial002.py
--rw-r--r--   0        0        0      114 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/first_steps/tutorial003.py
--rw-r--r--   0        0        0      522 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/generate_clients/tutorial001.py
--rw-r--r--   0        0        0      497 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/generate_clients/tutorial001_py39.py
--rw-r--r--   0        0        0      758 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/generate_clients/tutorial002.py
--rw-r--r--   0        0        0      733 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/generate_clients/tutorial002_py39.py
--rw-r--r--   0        0        0      943 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/generate_clients/tutorial003.py
--rw-r--r--   0        0        0      918 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/generate_clients/tutorial003_py39.py
--rw-r--r--   0        0        0     1066 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/generate_clients/tutorial004.js
--rw-r--r--   0        0        0      493 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/generate_clients/tutorial004.py
--rw-r--r--   0        0        0      449 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/graphql/tutorial001.py
--rw-r--r--   0        0        0      302 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/handling_errors/tutorial001.py
--rw-r--r--   0        0        0      407 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/handling_errors/tutorial002.py
--rw-r--r--   0        0        0      630 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/handling_errors/tutorial003.py
--rw-r--r--   0        0        0      767 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/handling_errors/tutorial004.py
--rw-r--r--   0        0        0      673 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/handling_errors/tutorial005.py
--rw-r--r--   0        0        0      933 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/handling_errors/tutorial006.py
--rw-r--r--   0        0        0      217 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/header_params/tutorial001.py
--rw-r--r--   0        0        0      262 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/header_params/tutorial001_an.py
--rw-r--r--   0        0        0      220 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/header_params/tutorial001_an_py310.py
--rw-r--r--   0        0        0      233 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/header_params/tutorial001_an_py39.py
--rw-r--r--   0        0        0      185 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/header_params/tutorial001_py310.py
--rw-r--r--   0        0        0      263 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/header_params/tutorial002.py
--rw-r--r--   0        0        0      320 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/header_params/tutorial002_an.py
--rw-r--r--   0        0        0      264 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/header_params/tutorial002_an_py310.py
--rw-r--r--   0        0        0      291 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/header_params/tutorial002_an_py39.py
--rw-r--r--   0        0        0      231 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/header_params/tutorial002_py310.py
--rw-r--r--   0        0        0      227 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/header_params/tutorial003.py
--rw-r--r--   0        0        0      272 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/header_params/tutorial003_an.py
--rw-r--r--   0        0        0      224 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/header_params/tutorial003_an_py310.py
--rw-r--r--   0        0        0      243 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/header_params/tutorial003_an_py39.py
--rw-r--r--   0        0        0      189 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/header_params/tutorial003_py310.py
--rw-r--r--   0        0        0      221 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/header_params/tutorial003_py39.py
--rw-r--r--   0        0        0      808 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/metadata/tutorial001.py
--rw-r--r--   0        0        0      770 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/metadata/tutorial001_1.py
--rw-r--r--   0        0        0      157 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/metadata/tutorial002.py
--rw-r--r--   0        0        0      164 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/metadata/tutorial003.py
--rw-r--r--   0        0        0      699 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/metadata/tutorial004.py
--rw-r--r--   0        0        0      352 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/middleware/tutorial001.py
--rw-r--r--   0        0        0     1361 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/nosql_databases/tutorial001.py
--rw-r--r--   0        0        0     1374 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/openapi_callbacks/tutorial001.py
--rw-r--r--   0        0        0      553 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/openapi_webhooks/tutorial001.py
--rw-r--r--   0        0        0      170 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/path_operation_advanced_configuration/tutorial001.py
--rw-r--r--   0        0        0      577 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/path_operation_advanced_configuration/tutorial002.py
--rw-r--r--   0        0        0      151 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/path_operation_advanced_configuration/tutorial003.py
--rw-r--r--   0        0        0      720 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/path_operation_advanced_configuration/tutorial004.py
--rw-r--r--   0        0        0      183 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/path_operation_advanced_configuration/tutorial005.py
--rw-r--r--   0        0        0     1046 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/path_operation_advanced_configuration/tutorial006.py
--rw-r--r--   0        0        0      825 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/path_operation_advanced_configuration/tutorial007.py
--rw-r--r--   0        0        0      792 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/path_operation_advanced_configuration/tutorial007_pv1.py
--rw-r--r--   0        0        0      409 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/path_operation_configuration/tutorial001.py
--rw-r--r--   0        0        0      366 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/path_operation_configuration/tutorial001_py310.py
--rw-r--r--   0        0        0      404 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/path_operation_configuration/tutorial001_py39.py
--rw-r--r--   0        0        0      583 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/path_operation_configuration/tutorial002.py
--rw-r--r--   0        0        0      540 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/path_operation_configuration/tutorial002_py310.py
--rw-r--r--   0        0        0      578 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/path_operation_configuration/tutorial002_py39.py
--rw-r--r--   0        0        0      326 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/path_operation_configuration/tutorial002b.py
--rw-r--r--   0        0        0      520 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/path_operation_configuration/tutorial003.py
--rw-r--r--   0        0        0      477 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/path_operation_configuration/tutorial003_py310.py
--rw-r--r--   0        0        0      515 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/path_operation_configuration/tutorial003_py39.py
--rw-r--r--   0        0        0      684 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/path_operation_configuration/tutorial004.py
--rw-r--r--   0        0        0      641 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/path_operation_configuration/tutorial004_py310.py
--rw-r--r--   0        0        0      679 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/path_operation_configuration/tutorial004_py39.py
--rw-r--r--   0        0        0      744 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/path_operation_configuration/tutorial005.py
--rw-r--r--   0        0        0      701 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/path_operation_configuration/tutorial005_py310.py
--rw-r--r--   0        0        0      739 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/path_operation_configuration/tutorial005_py39.py
--rw-r--r--   0        0        0      368 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/path_operation_configuration/tutorial006.py
--rw-r--r--   0        0        0      141 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/path_params/tutorial001.py
--rw-r--r--   0        0        0      146 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/path_params/tutorial002.py
--rw-r--r--   0        0        0      239 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/path_params/tutorial003.py
--rw-r--r--   0        0        0      196 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/path_params/tutorial003b.py
--rw-r--r--   0        0        0      159 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/path_params/tutorial004.py
--rw-r--r--   0        0        0      549 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/path_params/tutorial005.py
--rw-r--r--   0        0        0      367 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/path_params_numeric_validations/tutorial001.py
--rw-r--r--   0        0        0      420 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/path_params_numeric_validations/tutorial001_an.py
--rw-r--r--   0        0        0      378 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/path_params_numeric_validations/tutorial001_an_py310.py
--rw-r--r--   0        0        0      391 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/path_params_numeric_validations/tutorial001_an_py39.py
--rw-r--r--   0        0        0      335 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/path_params_numeric_validations/tutorial001_py310.py
--rw-r--r--   0        0        0      268 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/path_params_numeric_validations/tutorial002.py
--rw-r--r--   0        0        0      324 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/path_params_numeric_validations/tutorial002_an.py
--rw-r--r--   0        0        0      314 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/path_params_numeric_validations/tutorial002_an_py39.py
--rw-r--r--   0        0        0      271 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/path_params_numeric_validations/tutorial003.py
--rw-r--r--   0        0        0      324 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/path_params_numeric_validations/tutorial003_an.py
--rw-r--r--   0        0        0      314 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/path_params_numeric_validations/tutorial003_an_py39.py
--rw-r--r--   0        0        0      283 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/path_params_numeric_validations/tutorial004.py
--rw-r--r--   0        0        0      330 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/path_params_numeric_validations/tutorial004_an.py
--rw-r--r--   0        0        0      320 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/path_params_numeric_validations/tutorial004_an_py39.py
--rw-r--r--   0        0        0      301 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/path_params_numeric_validations/tutorial005.py
--rw-r--r--   0        0        0      344 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/path_params_numeric_validations/tutorial005_an.py
--rw-r--r--   0        0        0      334 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/path_params_numeric_validations/tutorial005_an_py39.py
--rw-r--r--   0        0        0      348 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/path_params_numeric_validations/tutorial006.py
--rw-r--r--   0        0        0      408 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/path_params_numeric_validations/tutorial006_an.py
--rw-r--r--   0        0        0      398 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/path_params_numeric_validations/tutorial006_an_py39.py
--rw-r--r--   0        0        0      162 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/python_types/tutorial001.py
--rw-r--r--   0        0        0      172 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/python_types/tutorial002.py
--rw-r--r--   0        0        0      119 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/python_types/tutorial003.py
--rw-r--r--   0        0        0      124 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/python_types/tutorial004.py
--rw-r--r--   0        0        0      143 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/python_types/tutorial005.py
--rw-r--r--   0        0        0      106 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/python_types/tutorial006.py
--rw-r--r--   0        0        0       80 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/python_types/tutorial006_py39.py
--rw-r--r--   0        0        0      131 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/python_types/tutorial007.py
--rw-r--r--   0        0        0       99 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/python_types/tutorial007_py39.py
--rw-r--r--   0        0        0      171 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/python_types/tutorial008.py
--rw-r--r--   0        0        0      145 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/python_types/tutorial008_py39.py
--rw-r--r--   0        0        0       84 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/python_types/tutorial008b.py
--rw-r--r--   0        0        0       51 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/python_types/tutorial008b_py310.py
--rw-r--r--   0        0        0      164 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/python_types/tutorial009.py
--rw-r--r--   0        0        0      131 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/python_types/tutorial009_py310.py
--rw-r--r--   0        0        0      164 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/python_types/tutorial009b.py
--rw-r--r--   0        0        0       89 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/python_types/tutorial009c.py
--rw-r--r--   0        0        0       56 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/python_types/tutorial009c_py310.py
--rw-r--r--   0        0        0      144 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/python_types/tutorial010.py
--rw-r--r--   0        0        0      498 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/python_types/tutorial011.py
--rw-r--r--   0        0        0      461 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/python_types/tutorial011_py310.py
--rw-r--r--   0        0        0      492 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/python_types/tutorial011_py39.py
--rw-r--r--   0        0        0      122 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/python_types/tutorial012.py
--rw-r--r--   0        0        0      138 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/python_types/tutorial013.py
--rw-r--r--   0        0        0      127 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/python_types/tutorial013_py39.py
--rw-r--r--   0        0        0      253 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/query_params/tutorial001.py
--rw-r--r--   0        0        0      254 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/query_params/tutorial002.py
--rw-r--r--   0        0        0      222 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/query_params/tutorial002_py310.py
--rw-r--r--   0        0        0      409 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/query_params/tutorial003.py
--rw-r--r--   0        0        0      377 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/query_params/tutorial003_py310.py
--rw-r--r--   0        0        0      471 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/query_params/tutorial004.py
--rw-r--r--   0        0        0      439 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/query_params/tutorial004_py310.py
--rw-r--r--   0        0        0      195 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/query_params/tutorial005.py
--rw-r--r--   0        0        0      304 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/query_params/tutorial006.py
--rw-r--r--   0        0        0      272 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/query_params/tutorial006_py310.py
--rw-r--r--   0        0        0      304 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/query_params/tutorial006b.py
--rw-r--r--   0        0        0      274 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial001.py
--rw-r--r--   0        0        0      242 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial001_py310.py
--rw-r--r--   0        0        0      311 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial002.py
--rw-r--r--   0        0        0      354 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial002_an.py
--rw-r--r--   0        0        0      312 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial002_an_py310.py
--rw-r--r--   0        0        0      279 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial002_py310.py
--rw-r--r--   0        0        0      332 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial003.py
--rw-r--r--   0        0        0      375 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial003_an.py
--rw-r--r--   0        0        0      333 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial003_an_py310.py
--rw-r--r--   0        0        0      346 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial003_an_py39.py
--rw-r--r--   0        0        0      293 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial003_py310.py
--rw-r--r--   0        0        0      370 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial004.py
--rw-r--r--   0        0        0      413 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial004_an.py
--rw-r--r--   0        0        0      371 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial004_an_py310.py
--rw-r--r--   0        0        0      369 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial004_an_py310_regex.py
--rw-r--r--   0        0        0      384 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial004_an_py39.py
--rw-r--r--   0        0        0      338 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial004_py310.py
--rw-r--r--   0        0        0      279 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial005.py
--rw-r--r--   0        0        0      322 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial005_an.py
--rw-r--r--   0        0        0      312 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial005_an_py39.py
--rw-r--r--   0        0        0      257 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial006.py
--rw-r--r--   0        0        0      307 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial006_an.py
--rw-r--r--   0        0        0      297 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial006_an_py39.py
--rw-r--r--   0        0        0      270 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial006b.py
--rw-r--r--   0        0        0      313 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial006b_an.py
--rw-r--r--   0        0        0      303 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial006b_an_py39.py
--rw-r--r--   0        0        0      309 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial006c.py
--rw-r--r--   0        0        0      352 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial006c_an.py
--rw-r--r--   0        0        0      310 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial006c_an_py310.py
--rw-r--r--   0        0        0      323 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial006c_an_py39.py
--rw-r--r--   0        0        0      277 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial006c_py310.py
--rw-r--r--   0        0        0      305 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial006d.py
--rw-r--r--   0        0        0      348 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial006d_an.py
--rw-r--r--   0        0        0      338 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial006d_an_py39.py
--rw-r--r--   0        0        0      339 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial007.py
--rw-r--r--   0        0        0      382 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial007_an.py
--rw-r--r--   0        0        0      340 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial007_an_py310.py
--rw-r--r--   0        0        0      353 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial007_an_py39.py
--rw-r--r--   0        0        0      307 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial007_py310.py
--rw-r--r--   0        0        0      469 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial008.py
--rw-r--r--   0        0        0      543 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial008_an.py
--rw-r--r--   0        0        0      501 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial008_an_py310.py
--rw-r--r--   0        0        0      514 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial008_an_py39.py
--rw-r--r--   0        0        0      437 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial008_py310.py
--rw-r--r--   0        0        0      316 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial009.py
--rw-r--r--   0        0        0      359 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial009_an.py
--rw-r--r--   0        0        0      317 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial009_an_py310.py
--rw-r--r--   0        0        0      330 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial009_an_py39.py
--rw-r--r--   0        0        0      284 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial009_py310.py
--rw-r--r--   0        0        0      577 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial010.py
--rw-r--r--   0        0        0      667 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial010_an.py
--rw-r--r--   0        0        0      625 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial010_an_py310.py
--rw-r--r--   0        0        0      638 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial010_an_py39.py
--rw-r--r--   0        0        0      545 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial010_py310.py
--rw-r--r--   0        0        0      230 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial011.py
--rw-r--r--   0        0        0      275 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial011_an.py
--rw-r--r--   0        0        0      227 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial011_an_py310.py
--rw-r--r--   0        0        0      240 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial011_an_py39.py
--rw-r--r--   0        0        0      192 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial011_py310.py
--rw-r--r--   0        0        0      224 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial011_py39.py
--rw-r--r--   0        0        0      220 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial012.py
--rw-r--r--   0        0        0      265 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial012_an.py
--rw-r--r--   0        0        0      230 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial012_an_py39.py
--rw-r--r--   0        0        0      195 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial012_py39.py
--rw-r--r--   0        0        0      178 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial013.py
--rw-r--r--   0        0        0      223 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial013_an.py
--rw-r--r--   0        0        0      213 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial013_an_py39.py
--rw-r--r--   0        0        0      333 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial014.py
--rw-r--r--   0        0        0      376 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial014_an.py
--rw-r--r--   0        0        0      334 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial014_an_py310.py
--rw-r--r--   0        0        0      347 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial014_an_py39.py
--rw-r--r--   0        0        0      301 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial014_py310.py
--rw-r--r--   0        0        0      285 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/request_files/tutorial001.py
--rw-r--r--   0        0        0      511 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/request_files/tutorial001_02.py
--rw-r--r--   0        0        0      556 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/request_files/tutorial001_02_an.py
--rw-r--r--   0        0        0      508 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/request_files/tutorial001_02_an_py310.py
--rw-r--r--   0        0        0      527 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/request_files/tutorial001_02_an_py39.py
--rw-r--r--   0        0        0      473 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/request_files/tutorial001_02_py310.py
--rw-r--r--   0        0        0      374 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/request_files/tutorial001_03.py
--rw-r--r--   0        0        0      434 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/request_files/tutorial001_03_an.py
--rw-r--r--   0        0        0      424 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/request_files/tutorial001_03_an_py39.py
--rw-r--r--   0        0        0      335 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/request_files/tutorial001_an.py
--rw-r--r--   0        0        0      325 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/request_files/tutorial001_an_py39.py
--rw-r--r--   0        0        0      815 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/request_files/tutorial002.py
--rw-r--r--   0        0        0      865 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/request_files/tutorial002_an.py
--rw-r--r--   0        0        0      830 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/request_files/tutorial002_an_py39.py
--rw-r--r--   0        0        0      790 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/request_files/tutorial002_py39.py
--rw-r--r--   0        0        0      917 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/request_files/tutorial003.py
--rw-r--r--   0        0        0      991 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/request_files/tutorial003_an.py
--rw-r--r--   0        0        0      956 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/request_files/tutorial003_an_py39.py
--rw-r--r--   0        0        0      892 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/request_files/tutorial003_py39.py
--rw-r--r--   0        0        0      176 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/request_forms/tutorial001.py
--rw-r--r--   0        0        0      236 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/request_forms/tutorial001_an.py
--rw-r--r--   0        0        0      226 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/request_forms/tutorial001_an_py39.py
--rw-r--r--   0        0        0      320 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/request_forms_and_files/tutorial001.py
--rw-r--r--   0        0        0      399 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/request_forms_and_files/tutorial001_an.py
--rw-r--r--   0        0        0      389 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/request_forms_and_files/tutorial001_an_py39.py
--rw-r--r--   0        0        0      394 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/response_change_status_code/tutorial001.py
--rw-r--r--   0        0        0      348 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/response_cookies/tutorial001.py
--rw-r--r--   0        0        0      275 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/response_cookies/tutorial002.py
--rw-r--r--   0        0        0      510 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/response_directly/tutorial001.py
--rw-r--r--   0        0        0      357 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/response_directly/tutorial002.py
--rw-r--r--   0        0        0      313 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/response_headers/tutorial001.py
--rw-r--r--   0        0        0      225 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/response_headers/tutorial002.py
--rw-r--r--   0        0        0      565 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/response_model/tutorial001.py
--rw-r--r--   0        0        0      516 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/response_model/tutorial001_01.py
--rw-r--r--   0        0        0      472 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/response_model/tutorial001_01_py310.py
--rw-r--r--   0        0        0      510 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/response_model/tutorial001_01_py39.py
--rw-r--r--   0        0        0      540 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/response_model/tutorial001_py310.py
--rw-r--r--   0        0        0      559 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/response_model/tutorial001_py39.py
--rw-r--r--   0        0        0      353 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/response_model/tutorial002.py
--rw-r--r--   0        0        0      321 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/response_model/tutorial002_py310.py
--rw-r--r--   0        0        0      453 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/response_model/tutorial003.py
--rw-r--r--   0        0        0      352 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/response_model/tutorial003_01.py
--rw-r--r--   0        0        0      320 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/response_model/tutorial003_01_py310.py
--rw-r--r--   0        0        0      385 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/response_model/tutorial003_02.py
--rw-r--r--   0        0        0      245 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/response_model/tutorial003_03.py
--rw-r--r--   0        0        0      388 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/response_model/tutorial003_04.py
--rw-r--r--   0        0        0      356 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/response_model/tutorial003_04_py310.py
--rw-r--r--   0        0        0      409 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/response_model/tutorial003_05.py
--rw-r--r--   0        0        0      377 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/response_model/tutorial003_05_py310.py
--rw-r--r--   0        0        0      434 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/response_model/tutorial003_py310.py
--rw-r--r--   0        0        0      636 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/response_model/tutorial004.py
--rw-r--r--   0        0        0      598 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/response_model/tutorial004_py310.py
--rw-r--r--   0        0        0      630 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/response_model/tutorial004_py39.py
--rw-r--r--   0        0        0      851 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/response_model/tutorial005.py
--rw-r--r--   0        0        0      819 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/response_model/tutorial005_py310.py
--rw-r--r--   0        0        0      851 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/response_model/tutorial006.py
--rw-r--r--   0        0        0      819 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/response_model/tutorial006_py310.py
--rw-r--r--   0        0        0      148 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/response_status_code/tutorial001.py
--rw-r--r--   0        0        0      176 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/response_status_code/tutorial002.py
--rw-r--r--   0        0        0      687 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/schema_extra_example/tutorial001.py
--rw-r--r--   0        0        0      672 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/schema_extra_example/tutorial001_pv1.py
--rw-r--r--   0        0        0      649 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/schema_extra_example/tutorial001_py310.py
--rw-r--r--   0        0        0      634 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/schema_extra_example/tutorial001_py310_pv1.py
--rw-r--r--   0        0        0      520 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/schema_extra_example/tutorial002.py
--rw-r--r--   0        0        0      482 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/schema_extra_example/tutorial002_py310.py
--rw-r--r--   0        0        0      615 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/schema_extra_example/tutorial003.py
--rw-r--r--   0        0        0      724 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/schema_extra_example/tutorial003_an.py
--rw-r--r--   0        0        0      676 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/schema_extra_example/tutorial003_an_py310.py
--rw-r--r--   0        0        0      695 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/schema_extra_example/tutorial003_an_py39.py
--rw-r--r--   0        0        0      577 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/schema_extra_example/tutorial003_py310.py
--rw-r--r--   0        0        0      827 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/schema_extra_example/tutorial004.py
--rw-r--r--   0        0        0      968 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/schema_extra_example/tutorial004_an.py
--rw-r--r--   0        0        0      920 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/schema_extra_example/tutorial004_an_py310.py
--rw-r--r--   0        0        0      939 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/schema_extra_example/tutorial004_an_py39.py
--rw-r--r--   0        0        0      789 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/schema_extra_example/tutorial004_py310.py
--rw-r--r--   0        0        0     1390 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/schema_extra_example/tutorial005.py
--rw-r--r--   0        0        0     1575 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/schema_extra_example/tutorial005_an.py
--rw-r--r--   0        0        0     1527 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/schema_extra_example/tutorial005_an_py310.py
--rw-r--r--   0        0        0     1546 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/schema_extra_example/tutorial005_an_py39.py
--rw-r--r--   0        0        0     1352 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/schema_extra_example/tutorial005_py310.py
--rw-r--r--   0        0        0      273 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/security/tutorial001.py
--rw-r--r--   0        0        0      323 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/security/tutorial001_an.py
--rw-r--r--   0        0        0      313 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/security/tutorial001_an_py39.py
--rw-r--r--   0        0        0      759 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/security/tutorial002.py
--rw-r--r--   0        0        0      819 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/security/tutorial002_an.py
--rw-r--r--   0        0        0      765 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/security/tutorial002_an_py310.py
--rw-r--r--   0        0        0      790 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/security/tutorial002_an_py39.py
--rw-r--r--   0        0        0      715 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/security/tutorial002_py310.py
--rw-r--r--   0        0        0     2498 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/security/tutorial003.py
--rw-r--r--   0        0        0     2592 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/security/tutorial003_an.py
--rw-r--r--   0        0        0     2538 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/security/tutorial003_an_py310.py
--rw-r--r--   0        0        0     2563 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/security/tutorial003_an_py39.py
--rw-r--r--   0        0        0     2454 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/security/tutorial003_py310.py
--rw-r--r--   0        0        0     4138 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/security/tutorial004.py
--rw-r--r--   0        0        0     4249 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/security/tutorial004_an.py
--rw-r--r--   0        0        0     4183 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/security/tutorial004_an_py310.py
--rw-r--r--   0        0        0     4220 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/security/tutorial004_an_py39.py
--rw-r--r--   0        0        0     4083 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/security/tutorial004_py310.py
--rw-r--r--   0        0        0     5274 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/security/tutorial005.py
--rw-r--r--   0        0        0     5381 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/security/tutorial005_an.py
--rw-r--r--   0        0        0     5309 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/security/tutorial005_an_py310.py
--rw-r--r--   0        0        0     5352 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/security/tutorial005_an_py39.py
--rw-r--r--   0        0        0     5213 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/security/tutorial005_py310.py
--rw-r--r--   0        0        0     5268 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/security/tutorial005_py39.py
--rw-r--r--   0        0        0      325 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/security/tutorial006.py
--rw-r--r--   0        0        0      375 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/security/tutorial006_an.py
--rw-r--r--   0        0        0      365 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/security/tutorial006_an_py39.py
--rw-r--r--   0        0        0     1120 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/security/tutorial007.py
--rw-r--r--   0        0        0     1187 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/security/tutorial007_an.py
--rw-r--r--   0        0        0     1176 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/security/tutorial007_an_py39.py
--rw-r--r--   0        0        0      492 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/separate_openapi_schemas/tutorial001.py
--rw-r--r--   0        0        0      454 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/separate_openapi_schemas/tutorial001_py310.py
--rw-r--r--   0        0        0      486 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/separate_openapi_schemas/tutorial001_py39.py
--rw-r--r--   0        0        0      527 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/separate_openapi_schemas/tutorial002.py
--rw-r--r--   0        0        0      489 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/separate_openapi_schemas/tutorial002_py310.py
--rw-r--r--   0        0        0      521 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/separate_openapi_schemas/tutorial002_py39.py
--rw-r--r--   0        0        0        0 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/settings/app01/__init__.py
--rw-r--r--   0        0        0      183 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/settings/app01/config.py
--rw-r--r--   0        0        0      270 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/settings/app01/main.py
--rw-r--r--   0        0        0        0 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/settings/app02/__init__.py
--rw-r--r--   0        0        0      159 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/settings/app02/config.py
--rw-r--r--   0        0        0      409 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/settings/app02/main.py
--rw-r--r--   0        0        0      516 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/settings/app02/test_main.py
--rw-r--r--   0        0        0        0 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/settings/app02_an/__init__.py
--rw-r--r--   0        0        0      159 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/settings/app02_an/config.py
--rw-r--r--   0        0        0      459 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/settings/app02_an/main.py
--rw-r--r--   0        0        0      516 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/settings/app02_an/test_main.py
--rw-r--r--   0        0        0        0 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/settings/app02_an_py39/__init__.py
--rw-r--r--   0        0        0      159 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/settings/app02_an_py39/config.py
--rw-r--r--   0        0        0      448 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/settings/app02_an_py39/main.py
--rw-r--r--   0        0        0      516 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/settings/app02_an_py39/test_main.py
--rw-r--r--   0        0        0        0 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/settings/app03/__init__.py
--rw-r--r--   0        0        0      204 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/settings/app03/config.py
--rw-r--r--   0        0        0      415 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/settings/app03/main.py
--rw-r--r--   0        0        0        0 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/settings/app03_an/__init__.py
--rw-r--r--   0        0        0      235 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/settings/app03_an/config.py
--rw-r--r--   0        0        0      195 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/settings/app03_an/config_pv1.py
--rw-r--r--   0        0        0      454 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/settings/app03_an/main.py
--rw-r--r--   0        0        0        0 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/settings/app03_an_py39/__init__.py
--rw-r--r--   0        0        0      204 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/settings/app03_an_py39/config.py
--rw-r--r--   0        0        0      465 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/settings/app03_an_py39/main.py
--rw-r--r--   0        0        0      422 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/settings/tutorial001.py
--rw-r--r--   0        0        0      413 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/settings/tutorial001_pv1.py
--rw-r--r--   0        0        0        0 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/sql_databases/__init__.py
--rw-r--r--   0        0        0        0 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/sql_databases/sql_app/__init__.py
--rw-r--r--   0        0        0     1931 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/sql_databases/sql_app/alt_main.py
--rw-r--r--   0        0        0     1061 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/sql_databases/sql_app/crud.py
--rw-r--r--   0        0        0      461 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/sql_databases/sql_app/database.py
--rw-r--r--   0        0        0     1635 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/sql_databases/sql_app/main.py
--rw-r--r--   0        0        0      710 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/sql_databases/sql_app/models.py
--rw-r--r--   0        0        0      502 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/sql_databases/sql_app/schemas.py
--rw-r--r--   0        0        0        0 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/sql_databases/sql_app/tests/__init__.py
--rw-r--r--   0        0        0     1261 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/sql_databases/sql_app/tests/test_sql_app.py
--rw-r--r--   0        0        0        0 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/sql_databases/sql_app_py310/__init__.py
--rw-r--r--   0        0        0     1906 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/sql_databases/sql_app_py310/alt_main.py
--rw-r--r--   0        0        0     1061 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/sql_databases/sql_app_py310/crud.py
--rw-r--r--   0        0        0      461 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/sql_databases/sql_app_py310/database.py
--rw-r--r--   0        0        0     1610 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/sql_databases/sql_app_py310/main.py
--rw-r--r--   0        0        0      710 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/sql_databases/sql_app_py310/models.py
--rw-r--r--   0        0        0      464 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/sql_databases/sql_app_py310/schemas.py
--rw-r--r--   0        0        0        0 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/sql_databases/sql_app_py310/tests/__init__.py
--rw-r--r--   0        0        0     1201 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/sql_databases/sql_app_py310/tests/test_sql_app.py
--rw-r--r--   0        0        0        0 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/sql_databases/sql_app_py39/__init__.py
--rw-r--r--   0        0        0     1906 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/sql_databases/sql_app_py39/alt_main.py
--rw-r--r--   0        0        0     1061 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/sql_databases/sql_app_py39/crud.py
--rw-r--r--   0        0        0      461 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/sql_databases/sql_app_py39/database.py
--rw-r--r--   0        0        0     1610 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/sql_databases/sql_app_py39/main.py
--rw-r--r--   0        0        0      710 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/sql_databases/sql_app_py39/models.py
--rw-r--r--   0        0        0      496 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/sql_databases/sql_app_py39/schemas.py
--rw-r--r--   0        0        0        0 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/sql_databases/sql_app_py39/tests/__init__.py
--rw-r--r--   0        0        0     1201 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/sql_databases/sql_app_py39/tests/test_sql_app.py
--rw-r--r--   0        0        0        0 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/sql_databases_peewee/sql_app/__init__.py
--rw-r--r--   0        0        0      843 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/sql_databases_peewee/sql_app/crud.py
--rw-r--r--   0        0        0      662 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/sql_databases_peewee/sql_app/database.py
--rw-r--r--   0        0        0     2213 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/sql_databases_peewee/sql_app/main.py
--rw-r--r--   0        0        0      465 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/sql_databases_peewee/sql_app/models.py
--rw-r--r--   0        0        0      868 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/sql_databases_peewee/sql_app/schemas.py
--rw-r--r--   0        0        0      163 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/static_files/tutorial001.py
--rw-r--r--   0        0        0      278 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/sub_applications/tutorial001.py
--rw-r--r--   0        0        0       25 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/templates/static/styles.css
--rw-r--r--   0        0        0      235 2024-05-12 00:38:13.722840 readyapi-0.110.3/docs_src/templates/templates/item.html
--rw-r--r--   0        0        0      527 2024-05-12 00:38:13.722840 readyapi-0.110.3/docs_src/templates/tutorial001.py
--rw-r--r--   0        0        0      233 2024-05-12 00:38:13.722840 readyapi-0.110.3/docs_src/using_request_directly/tutorial001.py
--rw-r--r--   0        0        0        0 2024-05-12 00:38:13.722840 readyapi-0.110.3/docs_src/websockets/__init__.py
--rw-r--r--   0        0        0     1436 2024-05-12 00:38:13.722840 readyapi-0.110.3/docs_src/websockets/tutorial001.py
--rw-r--r--   0        0        0     2846 2024-05-12 00:38:13.722840 readyapi-0.110.3/docs_src/websockets/tutorial002.py
--rw-r--r--   0        0        0     2913 2024-05-12 00:38:13.722840 readyapi-0.110.3/docs_src/websockets/tutorial002_an.py
--rw-r--r--   0        0        0     2859 2024-05-12 00:38:13.722840 readyapi-0.110.3/docs_src/websockets/tutorial002_an_py310.py
--rw-r--r--   0        0        0     2884 2024-05-12 00:38:13.722840 readyapi-0.110.3/docs_src/websockets/tutorial002_an_py39.py
--rw-r--r--   0        0        0     2802 2024-05-12 00:38:13.722840 readyapi-0.110.3/docs_src/websockets/tutorial002_py310.py
--rw-r--r--   0        0        0     2578 2024-05-12 00:38:13.722840 readyapi-0.110.3/docs_src/websockets/tutorial003.py
--rw-r--r--   0        0        0     2553 2024-05-12 00:38:13.722840 readyapi-0.110.3/docs_src/websockets/tutorial003_py39.py
--rw-r--r--   0        0        0      447 2024-05-12 00:38:13.722840 readyapi-0.110.3/docs_src/wsgi/tutorial001.py
--rw-r--r--   0        0        0     1731 2024-05-12 00:38:13.722840 readyapi-0.110.3/pdm_build.py
--rw-r--r--   0        0        0     7278 2024-05-12 00:38:20.474897 readyapi-0.110.3/pyproject.toml
--rw-r--r--   0        0        0     1084 2024-05-12 00:38:13.722840 readyapi-0.110.3/readyapi/__init__.py
--rw-r--r--   0        0        0    23139 2024-05-12 00:38:13.722840 readyapi-0.110.3/readyapi/_compat.py
--rw-r--r--   0        0        0   177259 2024-05-12 00:38:13.722840 readyapi-0.110.3/readyapi/applications.py
--rw-r--r--   0        0        0     1779 2024-05-12 00:38:13.722840 readyapi-0.110.3/readyapi/background.py
--rw-r--r--   0        0        0     1403 2024-05-12 00:38:13.722840 readyapi-0.110.3/readyapi/concurrency.py
--rw-r--r--   0        0        0     5774 2024-05-12 00:38:13.722840 readyapi-0.110.3/readyapi/datastructures.py
--rw-r--r--   0        0        0        0 2024-05-12 00:38:13.722840 readyapi-0.110.3/readyapi/dependencies/__init__.py
--rw-r--r--   0        0        0     2496 2024-05-12 00:38:13.722840 readyapi-0.110.3/readyapi/dependencies/models.py
--rw-r--r--   0        0        0    30266 2024-05-12 00:38:13.722840 readyapi-0.110.3/readyapi/dependencies/utils.py
--rw-r--r--   0        0        0    11074 2024-05-12 00:38:13.722840 readyapi-0.110.3/readyapi/encoders.py
--rw-r--r--   0        0        0     1336 2024-05-12 00:38:13.722840 readyapi-0.110.3/readyapi/exception_handlers.py
--rw-r--r--   0        0        0     4985 2024-05-12 00:38:13.722840 readyapi-0.110.3/readyapi/exceptions.py
--rw-r--r--   0        0        0       55 2024-05-12 00:38:13.722840 readyapi-0.110.3/readyapi/logger.py
--rw-r--r--   0        0        0       58 2024-05-12 00:38:13.722840 readyapi-0.110.3/readyapi/middleware/__init__.py
--rw-r--r--   0        0        0       79 2024-05-12 00:38:13.722840 readyapi-0.110.3/readyapi/middleware/cors.py
--rw-r--r--   0        0        0       79 2024-05-12 00:38:13.722840 readyapi-0.110.3/readyapi/middleware/gzip.py
--rw-r--r--   0        0        0      115 2024-05-12 00:38:13.722840 readyapi-0.110.3/readyapi/middleware/httpsredirect.py
--rw-r--r--   0        0        0      109 2024-05-12 00:38:13.722840 readyapi-0.110.3/readyapi/middleware/trustedhost.py
--rw-r--r--   0        0        0       79 2024-05-12 00:38:13.722840 readyapi-0.110.3/readyapi/middleware/wsgi.py
--rw-r--r--   0        0        0        0 2024-05-12 00:38:13.722840 readyapi-0.110.3/readyapi/openapi/__init__.py
--rw-r--r--   0        0        0      153 2024-05-12 00:38:13.722840 readyapi-0.110.3/readyapi/openapi/constants.py
--rw-r--r--   0        0        0    10379 2024-05-12 00:38:13.722840 readyapi-0.110.3/readyapi/openapi/docs.py
--rw-r--r--   0        0        0    17765 2024-05-12 00:38:13.722840 readyapi-0.110.3/readyapi/openapi/models.py
--rw-r--r--   0        0        0    22299 2024-05-12 00:38:13.722840 readyapi-0.110.3/readyapi/openapi/utils.py
--rw-r--r--   0        0        0    64082 2024-05-12 00:38:13.722840 readyapi-0.110.3/readyapi/param_functions.py
--rw-r--r--   0        0        0    28200 2024-05-12 00:38:13.722840 readyapi-0.110.3/readyapi/params.py
--rw-r--r--   0        0        0        0 2024-05-12 00:38:13.722840 readyapi-0.110.3/readyapi/py.typed
--rw-r--r--   0        0        0      142 2024-05-12 00:38:13.722840 readyapi-0.110.3/readyapi/requests.py
--rw-r--r--   0        0        0     1769 2024-05-12 00:38:13.722840 readyapi-0.110.3/readyapi/responses.py
--rw-r--r--   0        0        0   174906 2024-05-12 00:38:13.722840 readyapi-0.110.3/readyapi/routing.py
--rw-r--r--   0        0        0      881 2024-05-12 00:38:13.722840 readyapi-0.110.3/readyapi/security/__init__.py
--rw-r--r--   0        0        0     9382 2024-05-12 00:38:13.722840 readyapi-0.110.3/readyapi/security/api_key.py
--rw-r--r--   0        0        0      142 2024-05-12 00:38:13.722840 readyapi-0.110.3/readyapi/security/base.py
--rw-r--r--   0        0        0    13531 2024-05-12 00:38:13.722840 readyapi-0.110.3/readyapi/security/http.py
--rw-r--r--   0        0        0    21618 2024-05-12 00:38:13.722840 readyapi-0.110.3/readyapi/security/oauth2.py
--rw-r--r--   0        0        0     2724 2024-05-12 00:38:13.722840 readyapi-0.110.3/readyapi/security/open_id_connect_url.py
--rw-r--r--   0        0        0      293 2024-05-12 00:38:13.722840 readyapi-0.110.3/readyapi/security/utils.py
--rw-r--r--   0        0        0       69 2024-05-12 00:38:13.722840 readyapi-0.110.3/readyapi/staticfiles.py
--rw-r--r--   0        0        0       76 2024-05-12 00:38:13.722840 readyapi-0.110.3/readyapi/templating.py
--rw-r--r--   0        0        0       66 2024-05-12 00:38:13.722840 readyapi-0.110.3/readyapi/testclient.py
--rw-r--r--   0        0        0      383 2024-05-12 00:38:13.722840 readyapi-0.110.3/readyapi/types.py
--rw-r--r--   0        0        0     8044 2024-05-12 00:38:13.722840 readyapi-0.110.3/readyapi/utils.py
--rw-r--r--   0        0        0      222 2024-05-12 00:38:13.722840 readyapi-0.110.3/readyapi/websockets.py
--rw-r--r--   0        0        0       52 2024-05-12 00:38:13.722840 readyapi-0.110.3/requirements-docs-tests.txt
--rw-r--r--   0        0        0      464 2024-05-12 00:38:13.722840 readyapi-0.110.3/requirements-docs.txt
--rw-r--r--   0        0        0      496 2024-05-12 00:38:13.722840 readyapi-0.110.3/requirements-tests.txt
--rw-r--r--   0        0        0      128 2024-05-12 00:38:13.722840 readyapi-0.110.3/requirements.txt
--rwxr-xr-x   0        0        0    11141 2024-05-12 00:38:13.726840 readyapi-0.110.3/scripts/docs.py
--rwxr-xr-x   0        0        0      114 2024-05-12 00:38:13.726840 readyapi-0.110.3/scripts/format.sh
--rwxr-xr-x   0        0        0      128 2024-05-12 00:38:13.726840 readyapi-0.110.3/scripts/lint.sh
--rw-r--r--   0        0        0     5216 2024-05-12 00:38:13.726840 readyapi-0.110.3/scripts/mkdocs_hooks.py
--rw-r--r--   0        0        0      819 2024-05-12 00:38:13.726840 readyapi-0.110.3/scripts/playwright/separate_openapi_schemas/image01.py
--rw-r--r--   0        0        0      873 2024-05-12 00:38:13.726840 readyapi-0.110.3/scripts/playwright/separate_openapi_schemas/image02.py
--rw-r--r--   0        0        0      892 2024-05-12 00:38:13.726840 readyapi-0.110.3/scripts/playwright/separate_openapi_schemas/image03.py
--rw-r--r--   0        0        0      881 2024-05-12 00:38:13.726840 readyapi-0.110.3/scripts/playwright/separate_openapi_schemas/image04.py
--rw-r--r--   0        0        0      829 2024-05-12 00:38:13.726840 readyapi-0.110.3/scripts/playwright/separate_openapi_schemas/image05.py
--rwxr-xr-x   0        0        0      124 2024-05-12 00:38:13.726840 readyapi-0.110.3/scripts/test-cov-html.sh
--rwxr-xr-x   0        0        0       99 2024-05-12 00:38:13.726840 readyapi-0.110.3/scripts/test.sh
--rw-r--r--   0        0        0        0 2024-05-12 00:38:13.726840 readyapi-0.110.3/tests/__init__.py
--rw-r--r--   0        0        0     4455 2024-05-12 00:38:13.726840 readyapi-0.110.3/tests/main.py
--rw-r--r--   0        0        0     3693 2024-05-12 00:38:13.726840 readyapi-0.110.3/tests/test_additional_properties.py
--rw-r--r--   0        0        0     4307 2024-05-12 00:38:13.726840 readyapi-0.110.3/tests/test_additional_properties_bool.py
--rw-r--r--   0        0        0     1212 2024-05-12 00:38:13.726840 readyapi-0.110.3/tests/test_additional_response_extra.py
--rw-r--r--   0        0        0     1122 2024-05-12 00:38:13.726840 readyapi-0.110.3/tests/test_additional_responses_bad.py
--rw-r--r--   0        0        0     5900 2024-05-12 00:38:13.726840 readyapi-0.110.3/tests/test_additional_responses_custom_model_in_callback.py
--rw-r--r--   0        0        0     2980 2024-05-12 00:38:13.726840 readyapi-0.110.3/tests/test_additional_responses_custom_validationerror.py
--rw-r--r--   0        0        0     2887 2024-05-12 00:38:13.726840 readyapi-0.110.3/tests/test_additional_responses_default_validationerror.py
--rw-r--r--   0        0        0     3566 2024-05-12 00:38:13.726840 readyapi-0.110.3/tests/test_additional_responses_response_class.py
--rw-r--r--   0        0        0     5234 2024-05-12 00:38:13.726840 readyapi-0.110.3/tests/test_additional_responses_router.py
--rw-r--r--   0        0        0     2155 2024-05-12 00:38:13.726840 readyapi-0.110.3/tests/test_ambiguous_params.py
--rw-r--r--   0        0        0    10500 2024-05-12 00:38:13.726840 readyapi-0.110.3/tests/test_annotated.py
--rw-r--r--   0        0        0    53493 2024-05-12 00:38:13.726840 readyapi-0.110.3/tests/test_application.py
--rw-r--r--   0        0        0      461 2024-05-12 00:38:13.726840 readyapi-0.110.3/tests/test_callable_endpoint.py
--rw-r--r--   0        0        0     2832 2024-05-12 00:38:13.726840 readyapi-0.110.3/tests/test_compat.py
--rw-r--r--   0        0        0     2269 2024-05-12 00:38:13.726840 readyapi-0.110.3/tests/test_computed_fields.py
--rw-r--r--   0        0        0     2897 2024-05-12 00:38:13.726840 readyapi-0.110.3/tests/test_custom_middleware_exception.py
--rw-r--r--   0        0        0     3137 2024-05-12 00:38:13.726840 readyapi-0.110.3/tests/test_custom_route_class.py
--rw-r--r--   0        0        0     1251 2024-05-12 00:38:13.726840 readyapi-0.110.3/tests/test_custom_schema_fields.py
--rw-r--r--   0        0        0     1095 2024-05-12 00:38:13.726840 readyapi-0.110.3/tests/test_custom_swagger_ui_redirect.py
--rw-r--r--   0        0        0     2031 2024-05-12 00:38:13.726840 readyapi-0.110.3/tests/test_datastructures.py
--rw-r--r--   0        0        0     1609 2024-05-12 00:38:13.726840 readyapi-0.110.3/tests/test_datetime_custom_encoder.py
--rw-r--r--   0        0        0     5370 2024-05-12 00:38:13.726840 readyapi-0.110.3/tests/test_default_response_class.py
--rw-r--r--   0        0        0     5122 2024-05-12 00:38:13.726840 readyapi-0.110.3/tests/test_default_response_class_router.py
--rw-r--r--   0        0        0     2791 2024-05-12 00:38:13.726840 readyapi-0.110.3/tests/test_dependency_cache.py
--rw-r--r--   0        0        0     3383 2024-05-12 00:38:13.726840 readyapi-0.110.3/tests/test_dependency_class.py
--rw-r--r--   0        0        0    11874 2024-05-12 00:38:13.726840 readyapi-0.110.3/tests/test_dependency_contextmanager.py
--rw-r--r--   0        0        0     1564 2024-05-12 00:38:13.726840 readyapi-0.110.3/tests/test_dependency_contextvars.py
--rw-r--r--   0        0        0     8582 2024-05-12 00:38:13.726840 readyapi-0.110.3/tests/test_dependency_duplicates.py
--rw-r--r--   0        0        0     1965 2024-05-12 00:38:13.726840 readyapi-0.110.3/tests/test_dependency_normal_exceptions.py
--rw-r--r--   0        0        0    15820 2024-05-12 00:38:13.726840 readyapi-0.110.3/tests/test_dependency_overrides.py
--rw-r--r--   0        0        0     1468 2024-05-12 00:38:13.726840 readyapi-0.110.3/tests/test_dependency_security_overrides.py
--rw-r--r--   0        0        0     1198 2024-05-12 00:38:13.726840 readyapi-0.110.3/tests/test_deprecated_openapi_prefix.py
--rw-r--r--   0        0        0     2164 2024-05-12 00:38:13.726840 readyapi-0.110.3/tests/test_duplicate_models_openapi.py
--rw-r--r--   0        0        0      812 2024-05-12 00:38:13.726840 readyapi-0.110.3/tests/test_empty_router.py
--rw-r--r--   0        0        0     3463 2024-05-12 00:38:13.726840 readyapi-0.110.3/tests/test_enforce_once_required_parameter.py
--rw-r--r--   0        0        0     1923 2024-05-12 00:38:13.726840 readyapi-0.110.3/tests/test_exception_handlers.py
--rw-r--r--   0        0        0    14039 2024-05-12 00:38:13.726840 readyapi-0.110.3/tests/test_extra_routes.py
--rw-r--r--   0        0        0        0 2024-05-12 00:38:13.726840 readyapi-0.110.3/tests/test_filter_pydantic_sub_model/__init__.py
--rw-r--r--   0        0        0      787 2024-05-12 00:38:13.726840 readyapi-0.110.3/tests/test_filter_pydantic_sub_model/app_pv1.py
--rw-r--r--   0        0        0     4615 2024-05-12 00:38:13.726840 readyapi-0.110.3/tests/test_filter_pydantic_sub_model/test_filter_pydantic_sub_model_pv1.py
--rw-r--r--   0        0        0     6467 2024-05-12 00:38:13.726840 readyapi-0.110.3/tests/test_filter_pydantic_sub_model_pv2.py
--rw-r--r--   0        0        0     1206 2024-05-12 00:38:13.726840 readyapi-0.110.3/tests/test_forms_from_non_typing_sequences.py
--rw-r--r--   0        0        0    68318 2024-05-12 00:38:13.726840 readyapi-0.110.3/tests/test_generate_unique_id_function.py
--rw-r--r--   0        0        0     1886 2024-05-12 00:38:13.726840 readyapi-0.110.3/tests/test_generic_parameterless_depends.py
--rw-r--r--   0        0        0     3749 2024-05-12 00:38:13.726840 readyapi-0.110.3/tests/test_get_request_body.py
--rw-r--r--   0        0        0      977 2024-05-12 00:38:13.726840 readyapi-0.110.3/tests/test_http_connection_injection.py
--rw-r--r--   0        0        0      501 2024-05-12 00:38:13.726840 readyapi-0.110.3/tests/test_include_route.py
--rw-r--r--   0        0        0   367198 2024-05-12 00:38:13.726840 readyapi-0.110.3/tests/test_include_router_defaults_overrides.py
--rw-r--r--   0        0        0    13624 2024-05-12 00:38:13.726840 readyapi-0.110.3/tests/test_infer_param_optionality.py
--rw-r--r--   0        0        0     3090 2024-05-12 00:38:13.726840 readyapi-0.110.3/tests/test_inherited_custom_class.py
--rw-r--r--   0        0        0     1713 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_invalid_path_param.py
--rw-r--r--   0        0        0     1254 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_invalid_sequence_param.py
--rw-r--r--   0        0        0     9184 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_jsonable_encoder.py
--rw-r--r--   0        0        0     2507 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_local_docs.py
--rw-r--r--   0        0        0        0 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_modules_same_name_body/__init__.py
--rw-r--r--   0        0        0        0 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_modules_same_name_body/app/__init__.py
--rw-r--r--   0        0        0      161 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_modules_same_name_body/app/a.py
--rw-r--r--   0        0        0      162 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_modules_same_name_body/app/b.py
--rw-r--r--   0        0        0      153 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_modules_same_name_body/app/main.py
--rw-r--r--   0        0        0     5784 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_modules_same_name_body/test_main.py
--rw-r--r--   0        0        0     7826 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_multi_body_errors.py
--rw-r--r--   0        0        0     4615 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_multi_query_errors.py
--rw-r--r--   0        0        0     3790 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_multipart_installation.py
--rw-r--r--   0        0        0      790 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_no_swagger_ui_redirect.py
--rw-r--r--   0        0        0    17443 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_openapi_examples.py
--rw-r--r--   0        0        0     4852 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_openapi_query_parameter_extension.py
--rw-r--r--   0        0        0     1138 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_openapi_route_extensions.py
--rw-r--r--   0        0        0    18893 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_openapi_separate_input_output_schemas.py
--rw-r--r--   0        0        0     2012 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_openapi_servers.py
--rw-r--r--   0        0        0      937 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_operations_signatures.py
--rw-r--r--   0        0        0      567 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_orjson_response_class.py
--rw-r--r--   0        0        0      641 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_param_class.py
--rw-r--r--   0        0        0     3142 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_param_in_path_and_dependency.py
--rw-r--r--   0        0        0     7616 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_param_include_in_schema.py
--rw-r--r--   0        0        0     3415 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_params_repr.py
--rw-r--r--   0        0        0    35210 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_path.py
--rw-r--r--   0        0        0     3367 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_put_no_body.py
--rw-r--r--   0        0        0    11639 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_query.py
--rw-r--r--   0        0        0     2420 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_read_with_orm_mode.py
--rw-r--r--   0        0        0     6349 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_regex_deprecated_body.py
--rw-r--r--   0        0        0     5600 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_regex_deprecated_params.py
--rw-r--r--   0        0        0      796 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_repeated_cookie_headers.py
--rw-r--r--   0        0        0     3253 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_repeated_dependency_schema.py
--rw-r--r--   0        0        0     3750 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_repeated_parameter_alias.py
--rw-r--r--   0        0        0     3213 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_reponse_set_reponse_code_empty.py
--rw-r--r--   0        0        0     6514 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_request_body_parameters_media_type.py
--rw-r--r--   0        0        0     1534 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_required_noneable.py
--rw-r--r--   0        0        0    11385 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_response_by_alias.py
--rw-r--r--   0        0        0      593 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_response_change_status_code.py
--rw-r--r--   0        0        0     3421 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_response_class_no_mediatype.py
--rw-r--r--   0        0        0     3321 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_response_code_no_body.py
--rw-r--r--   0        0        0    48847 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_response_model_as_return_annotation.py
--rw-r--r--   0        0        0     1730 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_response_model_data_filter.py
--rw-r--r--   0        0        0     1750 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_response_model_data_filter_no_inheritance.py
--rw-r--r--   0        0        0     4122 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_response_model_include_exclude.py
--rw-r--r--   0        0        0     1136 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_response_model_invalid.py
--rw-r--r--   0        0        0     5384 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_response_model_sub_types.py
--rw-r--r--   0        0        0     1515 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_route_scope.py
--rw-r--r--   0        0        0     3301 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_router_events.py
--rw-r--r--   0        0        0      488 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_router_prefix_with_template.py
--rw-r--r--   0        0        0      979 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_router_redirect_slashes.py
--rw-r--r--   0        0        0    38582 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_schema_extra_examples.py
--rw-r--r--   0        0        0     1950 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_security_api_key_cookie.py
--rw-r--r--   0        0        0     2118 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_security_api_key_cookie_description.py
--rw-r--r--   0        0        0     2152 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_security_api_key_cookie_optional.py
--rw-r--r--   0        0        0     1890 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_security_api_key_header.py
--rw-r--r--   0        0        0     2058 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_security_api_key_header_description.py
--rw-r--r--   0        0        0     2088 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_security_api_key_header_optional.py
--rw-r--r--   0        0        0     1869 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_security_api_key_query.py
--rw-r--r--   0        0        0     2029 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_security_api_key_query_description.py
--rw-r--r--   0        0        0     2067 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_security_api_key_query_optional.py
--rw-r--r--   0        0        0     1793 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_security_http_base.py
--rw-r--r--   0        0        0     1979 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_security_http_base_description.py
--rw-r--r--   0        0        0     1938 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_security_http_base_optional.py
--rw-r--r--   0        0        0     2677 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_security_http_basic_optional.py
--rw-r--r--   0        0        0     2660 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_security_http_basic_realm.py
--rw-r--r--   0        0        0     2836 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_security_http_basic_realm_description.py
--rw-r--r--   0        0        0     2071 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_security_http_bearer.py
--rw-r--r--   0        0        0     2261 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_security_http_bearer_description.py
--rw-r--r--   0        0        0     2200 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_security_http_bearer_optional.py
--rw-r--r--   0        0        0     2096 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_security_http_digest.py
--rw-r--r--   0        0        0     2272 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_security_http_digest_description.py
--rw-r--r--   0        0        0     2239 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_security_http_digest_optional.py
--rw-r--r--   0        0        0    11008 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_security_oauth2.py
--rw-r--r--   0        0        0     2344 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_security_oauth2_authorization_code_bearer.py
--rw-r--r--   0        0        0     2448 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_security_oauth2_authorization_code_bearer_description.py
--rw-r--r--   0        0        0    11049 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_security_oauth2_optional.py
--rw-r--r--   0        0        0    11189 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_security_oauth2_optional_description.py
--rw-r--r--   0        0        0     2153 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_security_oauth2_password_bearer_optional.py
--rw-r--r--   0        0        0     2295 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_security_oauth2_password_bearer_optional_description.py
--rw-r--r--   0        0        0     2296 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_security_openid_connect.py
--rw-r--r--   0        0        0     2415 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_security_openid_connect_description.py
--rw-r--r--   0        0        0     2494 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_security_openid_connect_optional.py
--rw-r--r--   0        0        0     1418 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_serialize_response.py
--rw-r--r--   0        0        0     5002 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_serialize_response_dataclass.py
--rw-r--r--   0        0        0     4279 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_serialize_response_model.py
--rw-r--r--   0        0        0     2075 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_skip_defaults.py
--rw-r--r--   0        0        0     7555 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_starlette_exception.py
--rw-r--r--   0        0        0     1714 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_starlette_urlconvertors.py
--rw-r--r--   0        0        0    14147 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_sub_callbacks.py
--rw-r--r--   0        0        0      722 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_swagger_ui_init_oauth.py
--rw-r--r--   0        0        0    12073 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tuples.py
--rw-r--r--   0        0        0        0 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/__init__.py
--rw-r--r--   0        0        0        0 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_additional_responses/__init__.py
--rw-r--r--   0        0        0     4434 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_additional_responses/test_tutorial001.py
--rw-r--r--   0        0        0     4742 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_additional_responses/test_tutorial002.py
--rw-r--r--   0        0        0     4658 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_additional_responses/test_tutorial003.py
--rw-r--r--   0        0        0     4937 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_additional_responses/test_tutorial004.py
--rw-r--r--   0        0        0        0 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_additional_status_codes/__init__.py
--rw-r--r--   0        0        0      547 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_additional_status_codes/test_tutorial001.py
--rw-r--r--   0        0        0      550 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_additional_status_codes/test_tutorial001_an.py
--rw-r--r--   0        0        0      742 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_additional_status_codes/test_tutorial001_an_py310.py
--rw-r--r--   0        0        0      738 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_additional_status_codes/test_tutorial001_an_py39.py
--rw-r--r--   0        0        0      739 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_additional_status_codes/test_tutorial001_py310.py
--rw-r--r--   0        0        0        0 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_advanced_middleware/__init__.py
--rw-r--r--   0        0        0      475 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_advanced_middleware/test_tutorial001.py
--rw-r--r--   0        0        0      571 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_advanced_middleware/test_tutorial002.py
--rw-r--r--   0        0        0      667 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_advanced_middleware/test_tutorial003.py
--rw-r--r--   0        0        0        0 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_async_sql_databases/__init__.py
--rw-r--r--   0        0        0     6128 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_async_sql_databases/test_tutorial001.py
--rw-r--r--   0        0        0        0 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_async_tests/__init__.py
--rw-r--r--   0        0        0      143 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_async_tests/test_main.py
--rw-r--r--   0        0        0        0 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_background_tasks/__init__.py
--rw-r--r--   0        0        0      579 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_background_tasks/test_tutorial001.py
--rw-r--r--   0        0        0      569 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_background_tasks/test_tutorial002.py
--rw-r--r--   0        0        0      572 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_background_tasks/test_tutorial002_an.py
--rw-r--r--   0        0        0      632 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_background_tasks/test_tutorial002_an_py310.py
--rw-r--r--   0        0        0      629 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_background_tasks/test_tutorial002_an_py39.py
--rw-r--r--   0        0        0      629 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_background_tasks/test_tutorial002_py310.py
--rw-r--r--   0        0        0        0 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_behind_a_proxy/__init__.py
--rw-r--r--   0        0        0     1055 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_behind_a_proxy/test_tutorial001.py
--rw-r--r--   0        0        0     1034 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_behind_a_proxy/test_tutorial002.py
--rw-r--r--   0        0        0     1690 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_behind_a_proxy/test_tutorial003.py
--rw-r--r--   0        0        0     1658 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_behind_a_proxy/test_tutorial004.py
--rw-r--r--   0        0        0        0 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_bigger_applications/__init__.py
--rw-r--r--   0        0        0    25142 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_bigger_applications/test_main.py
--rw-r--r--   0        0        0    25145 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_bigger_applications/test_main_an.py
--rw-r--r--   0        0        0    25483 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_bigger_applications/test_main_an_py39.py
--rw-r--r--   0        0        0        0 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_body/__init__.py
--rw-r--r--   0        0        0    15094 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_body/test_tutorial001.py
--rw-r--r--   0        0        0    15342 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_body/test_tutorial001_py310.py
--rw-r--r--   0        0        0        0 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_body_fields/__init__.py
--rw-r--r--   0        0        0     7343 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_body_fields/test_tutorial001.py
--rw-r--r--   0        0        0     7346 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_body_fields/test_tutorial001_an.py
--rw-r--r--   0        0        0     7438 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_body_fields/test_tutorial001_an_py310.py
--rw-r--r--   0        0        0     7432 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_body_fields/test_tutorial001_an_py39.py
--rw-r--r--   0        0        0     7435 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_body_fields/test_tutorial001_py310.py
--rw-r--r--   0        0        0        0 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_body_multiple_params/__init__.py
--rw-r--r--   0        0        0     7700 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_body_multiple_params/test_tutorial001.py
--rw-r--r--   0        0        0     7703 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_body_multiple_params/test_tutorial001_an.py
--rw-r--r--   0        0        0     7808 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_body_multiple_params/test_tutorial001_an_py310.py
--rw-r--r--   0        0        0     7801 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_body_multiple_params/test_tutorial001_an_py39.py
--rw-r--r--   0        0        0     7805 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_body_multiple_params/test_tutorial001_py310.py
--rw-r--r--   0        0        0     9662 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_body_multiple_params/test_tutorial003.py
--rw-r--r--   0        0        0     9665 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_body_multiple_params/test_tutorial003_an.py
--rw-r--r--   0        0        0     9757 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_body_multiple_params/test_tutorial003_an_py310.py
--rw-r--r--   0        0        0     9751 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_body_multiple_params/test_tutorial003_an_py39.py
--rw-r--r--   0        0        0     9754 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_body_multiple_params/test_tutorial003_py310.py
--rw-r--r--   0        0        0        0 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_body_nested_models/__init__.py
--rw-r--r--   0        0        0     4345 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_body_nested_models/test_tutorial009.py
--rw-r--r--   0        0        0     4419 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_body_nested_models/test_tutorial009_py39.py
--rw-r--r--   0        0        0        0 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_body_updates/__init__.py
--rw-r--r--   0        0        0    12043 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_body_updates/test_tutorial001.py
--rw-r--r--   0        0        0    12114 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_body_updates/test_tutorial001_py310.py
--rw-r--r--   0        0        0    12108 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_body_updates/test_tutorial001_py39.py
--rw-r--r--   0        0        0        0 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_conditional_openapi/__init__.py
--rw-r--r--   0        0        0     1801 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_conditional_openapi/test_tutorial001.py
--rw-r--r--   0        0        0        0 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_configure_swagger_ui/__init__.py
--rw-r--r--   0        0        0     1416 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_configure_swagger_ui/test_tutorial001.py
--rw-r--r--   0        0        0     1563 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_configure_swagger_ui/test_tutorial002.py
--rw-r--r--   0        0        0     1535 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_configure_swagger_ui/test_tutorial003.py
--rw-r--r--   0        0        0        0 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_cookie_params/__init__.py
--rw-r--r--   0        0        0     4019 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_cookie_params/test_tutorial001.py
--rw-r--r--   0        0        0     4022 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_cookie_params/test_tutorial001_an.py
--rw-r--r--   0        0        0     4157 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_cookie_params/test_tutorial001_an_py310.py
--rw-r--r--   0        0        0     4152 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_cookie_params/test_tutorial001_an_py39.py
--rw-r--r--   0        0        0     4151 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_cookie_params/test_tutorial001_py310.py
--rw-r--r--   0        0        0        0 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_cors/__init__.py
--rw-r--r--   0        0        0     1287 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_cors/test_tutorial001.py
--rw-r--r--   0        0        0        0 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_custom_docs_ui/__init__.py
--rw-r--r--   0        0        0     1359 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_custom_docs_ui/test_tutorial001.py
--rw-r--r--   0        0        0     1250 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_custom_docs_ui/test_tutorial002.py
--rw-r--r--   0        0        0        0 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_custom_request_and_route/__init__.py
--rw-r--r--   0        0        0      888 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_custom_request_and_route/test_tutorial001.py
--rw-r--r--   0        0        0     1246 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_custom_request_and_route/test_tutorial002.py
--rw-r--r--   0        0        0      527 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_custom_request_and_route/test_tutorial003.py
--rw-r--r--   0        0        0        0 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_custom_response/__init__.py
--rw-r--r--   0        0        0     1027 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_custom_response/test_tutorial001.py
--rw-r--r--   0        0        0     1028 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_custom_response/test_tutorial001b.py
--rw-r--r--   0        0        0     1223 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_custom_response/test_tutorial004.py
--rw-r--r--   0        0        0      982 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_custom_response/test_tutorial005.py
--rw-r--r--   0        0        0     1061 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_custom_response/test_tutorial006.py
--rw-r--r--   0        0        0      909 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_custom_response/test_tutorial006b.py
--rw-r--r--   0        0        0      901 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_custom_response/test_tutorial006c.py
--rw-r--r--   0        0        0      265 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_custom_response/test_tutorial007.py
--rw-r--r--   0        0        0      488 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_custom_response/test_tutorial008.py
--rw-r--r--   0        0        0      488 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_custom_response/test_tutorial009.py
--rw-r--r--   0        0        0      491 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_custom_response/test_tutorial009b.py
--rw-r--r--   0        0        0      240 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_custom_response/test_tutorial009c.py
--rw-r--r--   0        0        0        0 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_dataclasses/__init__.py
--rw-r--r--   0        0        0     5291 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_dataclasses/test_tutorial001.py
--rw-r--r--   0        0        0     3576 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_dataclasses/test_tutorial002.py
--rw-r--r--   0        0        0    12359 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_dataclasses/test_tutorial003.py
--rw-r--r--   0        0        0        0 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_dependencies/__init__.py
--rw-r--r--   0        0        0     7221 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_dependencies/test_tutorial001.py
--rw-r--r--   0        0        0     7224 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_dependencies/test_tutorial001_an.py
--rw-r--r--   0        0        0     7404 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_dependencies/test_tutorial001_an_py310.py
--rw-r--r--   0        0        0     7400 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_dependencies/test_tutorial001_an_py39.py
--rw-r--r--   0        0        0     7401 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_dependencies/test_tutorial001_py310.py
--rw-r--r--   0        0        0     5553 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_dependencies/test_tutorial004.py
--rw-r--r--   0        0        0     5556 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_dependencies/test_tutorial004_an.py
--rw-r--r--   0        0        0     5736 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_dependencies/test_tutorial004_an_py310.py
--rw-r--r--   0        0        0     5732 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_dependencies/test_tutorial004_an_py39.py
--rw-r--r--   0        0        0     5733 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_dependencies/test_tutorial004_py310.py
--rw-r--r--   0        0        0     5121 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_dependencies/test_tutorial006.py
--rw-r--r--   0        0        0     5124 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_dependencies/test_tutorial006_an.py
--rw-r--r--   0        0        0     5402 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_dependencies/test_tutorial006_an_py39.py
--rw-r--r--   0        0        0      698 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_dependencies/test_tutorial008b.py
--rw-r--r--   0        0        0      701 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_dependencies/test_tutorial008b_an.py
--rw-r--r--   0        0        0      919 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_dependencies/test_tutorial008b_an_py39.py
--rw-r--r--   0        0        0     1171 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_dependencies/test_tutorial008c.py
--rw-r--r--   0        0        0     1177 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_dependencies/test_tutorial008c_an.py
--rw-r--r--   0        0        0     1268 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_dependencies/test_tutorial008c_an_py39.py
--rw-r--r--   0        0        0     1227 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_dependencies/test_tutorial008d.py
--rw-r--r--   0        0        0     1236 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_dependencies/test_tutorial008d_an.py
--rw-r--r--   0        0        0     1332 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_dependencies/test_tutorial008d_an_py39.py
--rw-r--r--   0        0        0     8640 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_dependencies/test_tutorial012.py
--rw-r--r--   0        0        0     8643 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_dependencies/test_tutorial012_an.py
--rw-r--r--   0        0        0     9041 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_dependencies/test_tutorial012_an_py39.py
--rw-r--r--   0        0        0        0 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_events/__init__.py
--rw-r--r--   0        0        0     3644 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_events/test_tutorial001.py
--rw-r--r--   0        0        0     1420 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_events/test_tutorial002.py
--rw-r--r--   0        0        0     3686 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_events/test_tutorial003.py
--rw-r--r--   0        0        0        0 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_extending_openapi/__init__.py
--rw-r--r--   0        0        0     1549 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_extending_openapi/test_tutorial001.py
--rw-r--r--   0        0        0        0 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_extra_data_types/__init__.py
--rw-r--r--   0        0        0     8029 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_extra_data_types/test_tutorial001.py
--rw-r--r--   0        0        0     8032 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_extra_data_types/test_tutorial001_an.py
--rw-r--r--   0        0        0     8224 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_extra_data_types/test_tutorial001_an_py310.py
--rw-r--r--   0        0        0     8220 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_extra_data_types/test_tutorial001_an_py39.py
--rw-r--r--   0        0        0     8221 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_extra_data_types/test_tutorial001_py310.py
--rw-r--r--   0        0        0        0 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_extra_models/__init__.py
--rw-r--r--   0        0        0     5197 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_extra_models/test_tutorial003.py
--rw-r--r--   0        0        0     5420 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_extra_models/test_tutorial003_py310.py
--rw-r--r--   0        0        0     1983 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_extra_models/test_tutorial004.py
--rw-r--r--   0        0        0     2171 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_extra_models/test_tutorial004_py39.py
--rw-r--r--   0        0        0     1482 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_extra_models/test_tutorial005.py
--rw-r--r--   0        0        0     1670 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_extra_models/test_tutorial005_py39.py
--rw-r--r--   0        0        0        0 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_first_steps/__init__.py
--rw-r--r--   0        0        0     1207 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_first_steps/test_tutorial001.py
--rw-r--r--   0        0        0        0 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_generate_clients/__init__.py
--rw-r--r--   0        0        0     7249 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_generate_clients/test_tutorial003.py
--rw-r--r--   0        0        0        0 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_handling_errors/__init__.py
--rw-r--r--   0        0        0     3300 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_handling_errors/test_tutorial001.py
--rw-r--r--   0        0        0     3373 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_handling_errors/test_tutorial002.py
--rw-r--r--   0        0        0     3296 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_handling_errors/test_tutorial003.py
--rw-r--r--   0        0        0     3802 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_handling_errors/test_tutorial004.py
--rw-r--r--   0        0        0     4431 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_handling_errors/test_tutorial005.py
--rw-r--r--   0        0        0     4074 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_handling_errors/test_tutorial006.py
--rw-r--r--   0        0        0        0 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_header_params/__init__.py
--rw-r--r--   0        0        0     3932 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_header_params/test_tutorial001.py
--rw-r--r--   0        0        0     3935 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_header_params/test_tutorial001_an.py
--rw-r--r--   0        0        0     4115 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_header_params/test_tutorial001_an_py310.py
--rw-r--r--   0        0        0     4112 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_header_params/test_tutorial001_py310.py
--rw-r--r--   0        0        0     4099 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_header_params/test_tutorial002.py
--rw-r--r--   0        0        0     4102 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_header_params/test_tutorial002_an.py
--rw-r--r--   0        0        0     4282 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_header_params/test_tutorial002_an_py310.py
--rw-r--r--   0        0        0     4353 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_header_params/test_tutorial002_an_py39.py
--rw-r--r--   0        0        0     4352 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_header_params/test_tutorial002_py310.py
--rw-r--r--   0        0        0     4242 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_header_params/test_tutorial003.py
--rw-r--r--   0        0        0     4227 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_header_params/test_tutorial003_an.py
--rw-r--r--   0        0        0     4407 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_header_params/test_tutorial003_an_py310.py
--rw-r--r--   0        0        0     4403 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_header_params/test_tutorial003_an_py39.py
--rw-r--r--   0        0        0     4404 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_header_params/test_tutorial003_py310.py
--rw-r--r--   0        0        0        0 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_metadata/__init__.py
--rw-r--r--   0        0        0     1765 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_metadata/test_tutorial001.py
--rw-r--r--   0        0        0     1729 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_metadata/test_tutorial001_1.py
--rw-r--r--   0        0        0     2082 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_metadata/test_tutorial004.py
--rw-r--r--   0        0        0        0 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_openapi_callbacks/__init__.py
--rw-r--r--   0        0        0     9218 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_openapi_callbacks/test_tutorial001.py
--rw-r--r--   0        0        0        0 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_openapi_webhooks/__init__.py
--rw-r--r--   0        0        0     4494 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_openapi_webhooks/test_tutorial001.py
--rw-r--r--   0        0        0        0 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_path_operation_advanced_configurations/__init__.py
--rw-r--r--   0        0        0     1039 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial001.py
--rw-r--r--   0        0        0     1022 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial002.py
--rw-r--r--   0        0        0      577 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial003.py
--rw-r--r--   0        0        0     8918 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial004.py
--rw-r--r--   0        0        0     1036 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial005.py
--rw-r--r--   0        0        0     1989 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial006.py
--rw-r--r--   0        0        0     3421 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial007.py
--rw-r--r--   0        0        0     3268 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial007_pv1.py
--rw-r--r--   0        0        0        0 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_path_operation_configurations/__init__.py
--rw-r--r--   0        0        0     1724 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_path_operation_configurations/test_tutorial002b.py
--rw-r--r--   0        0        0     8903 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_path_operation_configurations/test_tutorial005.py
--rw-r--r--   0        0        0     9105 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_path_operation_configurations/test_tutorial005_py310.py
--rw-r--r--   0        0        0     9100 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_path_operation_configurations/test_tutorial005_py39.py
--rw-r--r--   0        0        0     2407 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_path_operation_configurations/test_tutorial006.py
--rw-r--r--   0        0        0        0 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_path_params/__init__.py
--rw-r--r--   0        0        0     3371 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_path_params/test_tutorial004.py
--rw-r--r--   0        0        0     5144 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_path_params/test_tutorial005.py
--rw-r--r--   0        0        0        0 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_query_params/__init__.py
--rw-r--r--   0        0        0     4074 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_query_params/test_tutorial005.py
--rw-r--r--   0        0        0     6287 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_query_params/test_tutorial006.py
--rw-r--r--   0        0        0     6366 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_query_params/test_tutorial006_py310.py
--rw-r--r--   0        0        0        0 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_query_params_str_validations/__init__.py
--rw-r--r--   0        0        0     6390 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_query_params_str_validations/test_tutorial010.py
--rw-r--r--   0        0        0     6393 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_query_params_str_validations/test_tutorial010_an.py
--rw-r--r--   0        0        0     6498 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_query_params_str_validations/test_tutorial010_an_py310.py
--rw-r--r--   0        0        0     6491 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_query_params_str_validations/test_tutorial010_an_py39.py
--rw-r--r--   0        0        0     6495 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_query_params_str_validations/test_tutorial010_py310.py
--rw-r--r--   0        0        0     4019 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_query_params_str_validations/test_tutorial011.py
--rw-r--r--   0        0        0     4022 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_query_params_str_validations/test_tutorial011_an.py
--rw-r--r--   0        0        0     4245 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_query_params_str_validations/test_tutorial011_an_py310.py
--rw-r--r--   0        0        0     4240 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_query_params_str_validations/test_tutorial011_an_py39.py
--rw-r--r--   0        0        0     4242 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_query_params_str_validations/test_tutorial011_py310.py
--rw-r--r--   0        0        0     4237 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_query_params_str_validations/test_tutorial011_py39.py
--rw-r--r--   0        0        0     3487 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_query_params_str_validations/test_tutorial012.py
--rw-r--r--   0        0        0     3490 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_query_params_str_validations/test_tutorial012_an.py
--rw-r--r--   0        0        0     3708 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_query_params_str_validations/test_tutorial012_an_py39.py
--rw-r--r--   0        0        0     3705 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_query_params_str_validations/test_tutorial012_py39.py
--rw-r--r--   0        0        0     3436 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_query_params_str_validations/test_tutorial013.py
--rw-r--r--   0        0        0     3439 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_query_params_str_validations/test_tutorial013_an.py
--rw-r--r--   0        0        0     3657 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_query_params_str_validations/test_tutorial013_an_py39.py
--rw-r--r--   0        0        0     2939 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_query_params_str_validations/test_tutorial014.py
--rw-r--r--   0        0        0     2942 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_query_params_str_validations/test_tutorial014_an.py
--rw-r--r--   0        0        0     3165 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_query_params_str_validations/test_tutorial014_an_py310.py
--rw-r--r--   0        0        0     3164 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_query_params_str_validations/test_tutorial014_an_py39.py
--rw-r--r--   0        0        0     3162 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_query_params_str_validations/test_tutorial014_py310.py
--rw-r--r--   0        0        0        0 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_request_files/__init__.py
--rw-r--r--   0        0        0     7888 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_request_files/test_tutorial001.py
--rw-r--r--   0        0        0     8390 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_request_files/test_tutorial001_02.py
--rw-r--r--   0        0        0     8393 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_request_files/test_tutorial001_02_an.py
--rw-r--r--   0        0        0     8662 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_request_files/test_tutorial001_02_an_py310.py
--rw-r--r--   0        0        0     8655 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_request_files/test_tutorial001_02_an_py39.py
--rw-r--r--   0        0        0     8659 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_request_files/test_tutorial001_02_py310.py
--rw-r--r--   0        0        0     6135 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_request_files/test_tutorial001_03.py
--rw-r--r--   0        0        0     6138 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_request_files/test_tutorial001_03_an.py
--rw-r--r--   0        0        0     6302 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_request_files/test_tutorial001_03_an_py39.py
--rw-r--r--   0        0        0     7710 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_request_files/test_tutorial001_an.py
--rw-r--r--   0        0        0     7937 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_request_files/test_tutorial001_an_py39.py
--rw-r--r--   0        0        0     8681 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_request_files/test_tutorial002.py
--rw-r--r--   0        0        0     8684 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_request_files/test_tutorial002_an.py
--rw-r--r--   0        0        0     9084 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_request_files/test_tutorial002_an_py39.py
--rw-r--r--   0        0        0     9263 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_request_files/test_tutorial002_py39.py
--rw-r--r--   0        0        0     7313 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_request_files/test_tutorial003.py
--rw-r--r--   0        0        0     7316 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_request_files/test_tutorial003_an.py
--rw-r--r--   0        0        0     7838 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_request_files/test_tutorial003_an_py39.py
--rw-r--r--   0        0        0     7835 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_request_files/test_tutorial003_py39.py
--rw-r--r--   0        0        0        0 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_request_forms/__init__.py
--rw-r--r--   0        0        0     7632 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_request_forms/test_tutorial001.py
--rw-r--r--   0        0        0     7635 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_request_forms/test_tutorial001_an.py
--rw-r--r--   0        0        0     7745 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_request_forms/test_tutorial001_an_py39.py
--rw-r--r--   0        0        0        0 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_request_forms_and_files/__init__.py
--rw-r--r--   0        0        0    10049 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_request_forms_and_files/test_tutorial001.py
--rw-r--r--   0        0        0    10052 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_request_forms_and_files/test_tutorial001_an.py
--rw-r--r--   0        0        0    10162 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_request_forms_and_files/test_tutorial001_an_py39.py
--rw-r--r--   0        0        0        0 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_response_change_status_code/__init__.py
--rw-r--r--   0        0        0      522 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_response_change_status_code/test_tutorial001.py
--rw-r--r--   0        0        0        0 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_response_cookies/__init__.py
--rw-r--r--   0        0        0      404 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_response_cookies/test_tutorial001.py
--rw-r--r--   0        0        0      415 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_response_cookies/test_tutorial002.py
--rw-r--r--   0        0        0        0 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_response_headers/__init__.py
--rw-r--r--   0        0        0      427 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_response_headers/test_tutorial001.py
--rw-r--r--   0        0        0      379 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_response_headers/test_tutorial002.py
--rw-r--r--   0        0        0        0 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_response_model/__init__.py
--rw-r--r--   0        0        0     5766 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_response_model/test_tutorial003.py
--rw-r--r--   0        0        0     5772 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_response_model/test_tutorial003_01.py
--rw-r--r--   0        0        0     5964 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_response_model/test_tutorial003_01_py310.py
--rw-r--r--   0        0        0     3478 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_response_model/test_tutorial003_02.py
--rw-r--r--   0        0        0     1092 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_response_model/test_tutorial003_03.py
--rw-r--r--   0        0        0      239 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_response_model/test_tutorial003_04.py
--rw-r--r--   0        0        0      292 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_response_model/test_tutorial003_04_py310.py
--rw-r--r--   0        0        0     3478 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_response_model/test_tutorial003_05.py
--rw-r--r--   0        0        0     3701 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_response_model/test_tutorial003_05_py310.py
--rw-r--r--   0        0        0     5958 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_response_model/test_tutorial003_py310.py
--rw-r--r--   0        0        0     5110 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_response_model/test_tutorial004.py
--rw-r--r--   0        0        0     5290 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_response_model/test_tutorial004_py310.py
--rw-r--r--   0        0        0     5286 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_response_model/test_tutorial004_py39.py
--rw-r--r--   0        0        0     6156 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_response_model/test_tutorial005.py
--rw-r--r--   0        0        0     6379 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_response_model/test_tutorial005_py310.py
--rw-r--r--   0        0        0     6156 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_response_model/test_tutorial006.py
--rw-r--r--   0        0        0     6379 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_response_model/test_tutorial006_py310.py
--rw-r--r--   0        0        0        0 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_schema_extra_example/__init__.py
--rw-r--r--   0        0        0     4781 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_schema_extra_example/test_tutorial001.py
--rw-r--r--   0        0        0     4557 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_schema_extra_example/test_tutorial001_pv1.py
--rw-r--r--   0        0        0     4826 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_schema_extra_example/test_tutorial001_py310.py
--rw-r--r--   0        0        0     4602 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_schema_extra_example/test_tutorial001_py310_pv1.py
--rw-r--r--   0        0        0     7062 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_schema_extra_example/test_tutorial004.py
--rw-r--r--   0        0        0     7065 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_schema_extra_example/test_tutorial004_an.py
--rw-r--r--   0        0        0     7257 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_schema_extra_example/test_tutorial004_an_py310.py
--rw-r--r--   0        0        0     7253 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_schema_extra_example/test_tutorial004_an_py39.py
--rw-r--r--   0        0        0     7254 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_schema_extra_example/test_tutorial004_py310.py
--rw-r--r--   0        0        0     6910 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_schema_extra_example/test_tutorial005.py
--rw-r--r--   0        0        0     6913 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_schema_extra_example/test_tutorial005_an.py
--rw-r--r--   0        0        0     6979 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_schema_extra_example/test_tutorial005_an_py310.py
--rw-r--r--   0        0        0     6975 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_schema_extra_example/test_tutorial005_an_py39.py
--rw-r--r--   0        0        0     6976 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_schema_extra_example/test_tutorial005_py310.py
--rw-r--r--   0        0        0        0 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_security/__init__.py
--rw-r--r--   0        0        0     1907 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_security/test_tutorial001.py
--rw-r--r--   0        0        0     1910 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_security/test_tutorial001_an.py
--rw-r--r--   0        0        0     2158 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_security/test_tutorial001_an_py39.py
--rw-r--r--   0        0        0     8184 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_security/test_tutorial003.py
--rw-r--r--   0        0        0     8187 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_security/test_tutorial003_an.py
--rw-r--r--   0        0        0     8596 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_security/test_tutorial003_an_py310.py
--rw-r--r--   0        0        0     8585 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_security/test_tutorial003_an_py39.py
--rw-r--r--   0        0        0     8593 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_security/test_tutorial003_py310.py
--rw-r--r--   0        0        0    15805 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_security/test_tutorial005.py
--rw-r--r--   0        0        0    15808 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_security/test_tutorial005_an.py
--rw-r--r--   0        0        0    16713 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_security/test_tutorial005_an_py310.py
--rw-r--r--   0        0        0    16689 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_security/test_tutorial005_an_py39.py
--rw-r--r--   0        0        0    16701 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_security/test_tutorial005_py310.py
--rw-r--r--   0        0        0    16677 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_security/test_tutorial005_py39.py
--rw-r--r--   0        0        0     2320 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_security/test_tutorial006.py
--rw-r--r--   0        0        0     2323 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_security/test_tutorial006_an.py
--rw-r--r--   0        0        0     2596 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_security/test_tutorial006_an_py39.py
--rw-r--r--   0        0        0        0 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_separate_openapi_schemas/__init__.py
--rw-r--r--   0        0        0     4960 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_separate_openapi_schemas/test_tutorial001.py
--rw-r--r--   0        0        0     5018 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_separate_openapi_schemas/test_tutorial001_py310.py
--rw-r--r--   0        0        0     5013 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_separate_openapi_schemas/test_tutorial001_py39.py
--rw-r--r--   0        0        0     4960 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_separate_openapi_schemas/test_tutorial002.py
--rw-r--r--   0        0        0     5018 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_separate_openapi_schemas/test_tutorial002_py310.py
--rw-r--r--   0        0        0     5013 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_separate_openapi_schemas/test_tutorial002_py39.py
--rw-r--r--   0        0        0        0 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_settings/__init__.py
--rw-r--r--   0        0        0      488 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_settings/test_app02.py
--rw-r--r--   0        0        0      553 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_settings/test_tutorial001.py
--rw-r--r--   0        0        0      557 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_settings/test_tutorial001_pv1.py
--rw-r--r--   0        0        0        0 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_sql_databases/__init__.py
--rw-r--r--   0        0        0    16477 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_sql_databases/test_sql_databases.py
--rw-r--r--   0        0        0    16656 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_sql_databases/test_sql_databases_middleware.py
--rw-r--r--   0        0        0    16926 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_sql_databases/test_sql_databases_middleware_py310.py
--rw-r--r--   0        0        0    16927 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_sql_databases/test_sql_databases_middleware_py39.py
--rw-r--r--   0        0        0    16932 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_sql_databases/test_sql_databases_py310.py
--rw-r--r--   0        0        0    16923 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_sql_databases/test_sql_databases_py39.py
--rw-r--r--   0        0        0      788 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_sql_databases/test_testing_databases.py
--rw-r--r--   0        0        0      825 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_sql_databases/test_testing_databases_py310.py
--rw-r--r--   0        0        0      822 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_sql_databases/test_testing_databases_py39.py
--rw-r--r--   0        0        0        0 2024-05-12 00:38:13.750840 readyapi-0.110.3/tests/test_tutorial/test_sub_applications/__init__.py
--rw-r--r--   0        0        0     1923 2024-05-12 00:38:13.750840 readyapi-0.110.3/tests/test_tutorial/test_sub_applications/test_tutorial001.py
--rw-r--r--   0        0        0        0 2024-05-12 00:38:13.750840 readyapi-0.110.3/tests/test_tutorial/test_templates/__init__.py
--rw-r--r--   0        0        0      911 2024-05-12 00:38:13.750840 readyapi-0.110.3/tests/test_tutorial/test_templates/test_tutorial001.py
--rw-r--r--   0        0        0        0 2024-05-12 00:38:13.750840 readyapi-0.110.3/tests/test_tutorial/test_testing/__init__.py
--rw-r--r--   0        0        0      820 2024-05-12 00:38:13.750840 readyapi-0.110.3/tests/test_tutorial/test_testing/test_main.py
--rw-r--r--   0        0        0      300 2024-05-12 00:38:13.750840 readyapi-0.110.3/tests/test_tutorial/test_testing/test_main_b.py
--rw-r--r--   0        0        0      303 2024-05-12 00:38:13.750840 readyapi-0.110.3/tests/test_tutorial/test_testing/test_main_b_an.py
--rw-r--r--   0        0        0      360 2024-05-12 00:38:13.750840 readyapi-0.110.3/tests/test_tutorial/test_testing/test_main_b_an_py310.py
--rw-r--r--   0        0        0      357 2024-05-12 00:38:13.750840 readyapi-0.110.3/tests/test_tutorial/test_testing/test_main_b_an_py39.py
--rw-r--r--   0        0        0      357 2024-05-12 00:38:13.750840 readyapi-0.110.3/tests/test_tutorial/test_testing/test_main_b_py310.py
--rw-r--r--   0        0        0      822 2024-05-12 00:38:13.750840 readyapi-0.110.3/tests/test_tutorial/test_testing/test_tutorial001.py
--rw-r--r--   0        0        0      154 2024-05-12 00:38:13.750840 readyapi-0.110.3/tests/test_tutorial/test_testing/test_tutorial002.py
--rw-r--r--   0        0        0      167 2024-05-12 00:38:13.750840 readyapi-0.110.3/tests/test_tutorial/test_testing/test_tutorial003.py
--rw-r--r--   0        0        0        0 2024-05-12 00:38:13.750840 readyapi-0.110.3/tests/test_tutorial/test_testing_dependencies/__init__.py
--rw-r--r--   0        0        0     1527 2024-05-12 00:38:13.750840 readyapi-0.110.3/tests/test_tutorial/test_testing_dependencies/test_tutorial001.py
--rw-r--r--   0        0        0     1530 2024-05-12 00:38:13.750840 readyapi-0.110.3/tests/test_tutorial/test_testing_dependencies/test_tutorial001_an.py
--rw-r--r--   0        0        0     2088 2024-05-12 00:38:13.750840 readyapi-0.110.3/tests/test_tutorial/test_testing_dependencies/test_tutorial001_an_py310.py
--rw-r--r--   0        0        0     2073 2024-05-12 00:38:13.750840 readyapi-0.110.3/tests/test_tutorial/test_testing_dependencies/test_tutorial001_an_py39.py
--rw-r--r--   0        0        0     2067 2024-05-12 00:38:13.750840 readyapi-0.110.3/tests/test_tutorial/test_testing_dependencies/test_tutorial001_py310.py
--rw-r--r--   0        0        0        0 2024-05-12 00:38:13.750840 readyapi-0.110.3/tests/test_tutorial/test_websockets/__init__.py
--rw-r--r--   0        0        0      824 2024-05-12 00:38:13.750840 readyapi-0.110.3/tests/test_tutorial/test_websockets/test_tutorial001.py
--rw-r--r--   0        0        0     3685 2024-05-12 00:38:13.750840 readyapi-0.110.3/tests/test_tutorial/test_websockets/test_tutorial002.py
--rw-r--r--   0        0        0     3688 2024-05-12 00:38:13.750840 readyapi-0.110.3/tests/test_tutorial/test_websockets/test_tutorial002_an.py
--rw-r--r--   0        0        0     3978 2024-05-12 00:38:13.750840 readyapi-0.110.3/tests/test_tutorial/test_websockets/test_tutorial002_an_py310.py
--rw-r--r--   0        0        0     3970 2024-05-12 00:38:13.750840 readyapi-0.110.3/tests/test_tutorial/test_websockets/test_tutorial002_an_py39.py
--rw-r--r--   0        0        0     3975 2024-05-12 00:38:13.750840 readyapi-0.110.3/tests/test_tutorial/test_websockets/test_tutorial002_py310.py
--rw-r--r--   0        0        0      873 2024-05-12 00:38:13.750840 readyapi-0.110.3/tests/test_tutorial/test_websockets/test_tutorial003.py
--rw-r--r--   0        0        0     1292 2024-05-12 00:38:13.750840 readyapi-0.110.3/tests/test_tutorial/test_websockets/test_tutorial003_py39.py
--rw-r--r--   0        0        0        0 2024-05-12 00:38:13.750840 readyapi-0.110.3/tests/test_tutorial/test_wsgi/__init__.py
--rw-r--r--   0        0        0      437 2024-05-12 00:38:13.750840 readyapi-0.110.3/tests/test_tutorial/test_wsgi/test_tutorial001.py
--rw-r--r--   0        0        0      713 2024-05-12 00:38:13.750840 readyapi-0.110.3/tests/test_typing_python39.py
--rw-r--r--   0        0        0     4753 2024-05-12 00:38:13.750840 readyapi-0.110.3/tests/test_union_body.py
--rw-r--r--   0        0        0     5316 2024-05-12 00:38:13.750840 readyapi-0.110.3/tests/test_union_inherited_body.py
--rw-r--r--   0        0        0     2036 2024-05-12 00:38:13.750840 readyapi-0.110.3/tests/test_validate_response.py
--rw-r--r--   0        0        0     1213 2024-05-12 00:38:13.750840 readyapi-0.110.3/tests/test_validate_response_dataclass.py
--rw-r--r--   0        0        0        0 2024-05-12 00:38:13.750840 readyapi-0.110.3/tests/test_validate_response_recursive/__init__.py
--rw-r--r--   0        0        0     1152 2024-05-12 00:38:13.750840 readyapi-0.110.3/tests/test_validate_response_recursive/app_pv1.py
--rw-r--r--   0        0        0     1181 2024-05-12 00:38:13.750840 readyapi-0.110.3/tests/test_validate_response_recursive/app_pv2.py
--rw-r--r--   0        0        0      901 2024-05-12 00:38:13.750840 readyapi-0.110.3/tests/test_validate_response_recursive/test_validate_response_recursive_pv1.py
--rw-r--r--   0        0        0      901 2024-05-12 00:38:13.750840 readyapi-0.110.3/tests/test_validate_response_recursive/test_validate_response_recursive_pv2.py
--rw-r--r--   0        0        0     4673 2024-05-12 00:38:13.750840 readyapi-0.110.3/tests/test_webhooks_security.py
--rw-r--r--   0        0        0     2203 2024-05-12 00:38:13.750840 readyapi-0.110.3/tests/test_ws_dependencies.py
--rw-r--r--   0        0        0     7657 2024-05-12 00:38:13.750840 readyapi-0.110.3/tests/test_ws_router.py
--rw-r--r--   0        0        0      423 2024-05-12 00:38:13.750840 readyapi-0.110.3/tests/utils.py
--rw-r--r--   0        0        0    25444 1970-01-01 00:00:00.000000 readyapi-0.110.3/PKG-INFO
+-rw-r--r--   0        0        0     1084 2024-05-12 05:04:32.939446 readyapi-0.111.0.dev1/LICENSE
+-rw-r--r--   0        0        0    20349 2024-05-12 05:04:32.939446 readyapi-0.111.0.dev1/README.md
+-rw-r--r--   0        0        0     5043 2024-05-12 05:04:32.979446 readyapi-0.111.0.dev1/docs/en/docs/img/favicon.png
+-rw-r--r--   0        0        0      510 2024-05-12 05:04:33.071447 readyapi-0.111.0.dev1/docs_src/additional_responses/tutorial001.py
+-rw-r--r--   0        0        0      632 2024-05-12 05:04:33.071447 readyapi-0.111.0.dev1/docs_src/additional_responses/tutorial002.py
+-rw-r--r--   0        0        0      841 2024-05-12 05:04:33.071447 readyapi-0.111.0.dev1/docs_src/additional_responses/tutorial003.py
+-rw-r--r--   0        0        0      705 2024-05-12 05:04:33.071447 readyapi-0.111.0.dev1/docs_src/additional_responses/tutorial004.py
+-rw-r--r--   0        0        0      688 2024-05-12 05:04:33.071447 readyapi-0.111.0.dev1/docs_src/additional_status_codes/tutorial001.py
+-rw-r--r--   0        0        0      738 2024-05-12 05:04:33.071447 readyapi-0.111.0.dev1/docs_src/additional_status_codes/tutorial001_an.py
+-rw-r--r--   0        0        0      690 2024-05-12 05:04:33.071447 readyapi-0.111.0.dev1/docs_src/additional_status_codes/tutorial001_an_py310.py
+-rw-r--r--   0        0        0      709 2024-05-12 05:04:33.071447 readyapi-0.111.0.dev1/docs_src/additional_status_codes/tutorial001_an_py39.py
+-rw-r--r--   0        0        0      650 2024-05-12 05:04:33.071447 readyapi-0.111.0.dev1/docs_src/additional_status_codes/tutorial001_py310.py
+-rw-r--r--   0        0        0      235 2024-05-12 05:04:33.071447 readyapi-0.111.0.dev1/docs_src/advanced_middleware/tutorial001.py
+-rw-r--r--   0        0        0      283 2024-05-12 05:04:33.071447 readyapi-0.111.0.dev1/docs_src/advanced_middleware/tutorial002.py
+-rw-r--r--   0        0        0      217 2024-05-12 05:04:33.071447 readyapi-0.111.0.dev1/docs_src/advanced_middleware/tutorial003.py
+-rw-r--r--   0        0        0        0 2024-05-12 05:04:33.071447 readyapi-0.111.0.dev1/docs_src/app_testing/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-12 05:04:33.071447 readyapi-0.111.0.dev1/docs_src/app_testing/app_b/__init__.py
+-rw-r--r--   0        0        0     1148 2024-05-12 05:04:33.071447 readyapi-0.111.0.dev1/docs_src/app_testing/app_b/main.py
+-rw-r--r--   0        0        0     1867 2024-05-12 05:04:33.071447 readyapi-0.111.0.dev1/docs_src/app_testing/app_b/test_main.py
+-rw-r--r--   0        0        0        0 2024-05-12 05:04:33.071447 readyapi-0.111.0.dev1/docs_src/app_testing/app_b_an/__init__.py
+-rw-r--r--   0        0        0     1208 2024-05-12 05:04:33.071447 readyapi-0.111.0.dev1/docs_src/app_testing/app_b_an/main.py
+-rw-r--r--   0        0        0     1867 2024-05-12 05:04:33.071447 readyapi-0.111.0.dev1/docs_src/app_testing/app_b_an/test_main.py
+-rw-r--r--   0        0        0        0 2024-05-12 05:04:33.071447 readyapi-0.111.0.dev1/docs_src/app_testing/app_b_an_py310/__init__.py
+-rw-r--r--   0        0        0     1166 2024-05-12 05:04:33.071447 readyapi-0.111.0.dev1/docs_src/app_testing/app_b_an_py310/main.py
+-rw-r--r--   0        0        0     1867 2024-05-12 05:04:33.071447 readyapi-0.111.0.dev1/docs_src/app_testing/app_b_an_py310/test_main.py
+-rw-r--r--   0        0        0        0 2024-05-12 05:04:33.071447 readyapi-0.111.0.dev1/docs_src/app_testing/app_b_an_py39/__init__.py
+-rw-r--r--   0        0        0     1179 2024-05-12 05:04:33.071447 readyapi-0.111.0.dev1/docs_src/app_testing/app_b_an_py39/main.py
+-rw-r--r--   0        0        0     1867 2024-05-12 05:04:33.071447 readyapi-0.111.0.dev1/docs_src/app_testing/app_b_an_py39/test_main.py
+-rw-r--r--   0        0        0        0 2024-05-12 05:04:33.071447 readyapi-0.111.0.dev1/docs_src/app_testing/app_b_py310/__init__.py
+-rw-r--r--   0        0        0     1116 2024-05-12 05:04:33.071447 readyapi-0.111.0.dev1/docs_src/app_testing/app_b_py310/main.py
+-rw-r--r--   0        0        0     1867 2024-05-12 05:04:33.071447 readyapi-0.111.0.dev1/docs_src/app_testing/app_b_py310/test_main.py
+-rw-r--r--   0        0        0      121 2024-05-12 05:04:33.071447 readyapi-0.111.0.dev1/docs_src/app_testing/main.py
+-rw-r--r--   0        0        0      239 2024-05-12 05:04:33.071447 readyapi-0.111.0.dev1/docs_src/app_testing/test_main.py
+-rw-r--r--   0        0        0      338 2024-05-12 05:04:33.071447 readyapi-0.111.0.dev1/docs_src/app_testing/tutorial001.py
+-rw-r--r--   0        0        0      762 2024-05-12 05:04:33.071447 readyapi-0.111.0.dev1/docs_src/app_testing/tutorial002.py
+-rw-r--r--   0        0        0      532 2024-05-12 05:04:33.071447 readyapi-0.111.0.dev1/docs_src/app_testing/tutorial003.py
+-rw-r--r--   0        0        0     1418 2024-05-12 05:04:33.071447 readyapi-0.111.0.dev1/docs_src/async_sql_databases/tutorial001.py
+-rw-r--r--   0        0        0        0 2024-05-12 05:04:33.071447 readyapi-0.111.0.dev1/docs_src/async_tests/__init__.py
+-rw-r--r--   0        0        0      115 2024-05-12 05:04:33.071447 readyapi-0.111.0.dev1/docs_src/async_tests/main.py
+-rw-r--r--   0        0        0      306 2024-05-12 05:04:33.071447 readyapi-0.111.0.dev1/docs_src/async_tests/test_main.py
+-rw-r--r--   0        0        0      522 2024-05-12 05:04:33.071447 readyapi-0.111.0.dev1/docs_src/background_tasks/tutorial001.py
+-rw-r--r--   0        0        0      678 2024-05-12 05:04:33.071447 readyapi-0.111.0.dev1/docs_src/background_tasks/tutorial002.py
+-rw-r--r--   0        0        0      728 2024-05-12 05:04:33.075447 readyapi-0.111.0.dev1/docs_src/background_tasks/tutorial002_an.py
+-rw-r--r--   0        0        0      686 2024-05-12 05:04:33.075447 readyapi-0.111.0.dev1/docs_src/background_tasks/tutorial002_an_py310.py
+-rw-r--r--   0        0        0      699 2024-05-12 05:04:33.075447 readyapi-0.111.0.dev1/docs_src/background_tasks/tutorial002_an_py39.py
+-rw-r--r--   0        0        0      646 2024-05-12 05:04:33.075447 readyapi-0.111.0.dev1/docs_src/background_tasks/tutorial002_py310.py
+-rw-r--r--   0        0        0      192 2024-05-12 05:04:33.075447 readyapi-0.111.0.dev1/docs_src/behind_a_proxy/tutorial001.py
+-rw-r--r--   0        0        0      211 2024-05-12 05:04:33.075447 readyapi-0.111.0.dev1/docs_src/behind_a_proxy/tutorial002.py
+-rw-r--r--   0        0        0      408 2024-05-12 05:04:33.075447 readyapi-0.111.0.dev1/docs_src/behind_a_proxy/tutorial003.py
+-rw-r--r--   0        0        0      440 2024-05-12 05:04:33.075447 readyapi-0.111.0.dev1/docs_src/behind_a_proxy/tutorial004.py
+-rw-r--r--   0        0        0        0 2024-05-12 05:04:33.075447 readyapi-0.111.0.dev1/docs_src/bigger_applications/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-12 05:04:33.075447 readyapi-0.111.0.dev1/docs_src/bigger_applications/app/__init__.py
+-rw-r--r--   0        0        0      370 2024-05-12 05:04:33.075447 readyapi-0.111.0.dev1/docs_src/bigger_applications/app/dependencies.py
+-rw-r--r--   0        0        0        0 2024-05-12 05:04:33.075447 readyapi-0.111.0.dev1/docs_src/bigger_applications/app/internal/__init__.py
+-rw-r--r--   0        0        0      148 2024-05-12 05:04:33.075447 readyapi-0.111.0.dev1/docs_src/bigger_applications/app/internal/admin.py
+-rw-r--r--   0        0        0      555 2024-05-12 05:04:33.075447 readyapi-0.111.0.dev1/docs_src/bigger_applications/app/main.py
+-rw-r--r--   0        0        0        0 2024-05-12 05:04:33.075447 readyapi-0.111.0.dev1/docs_src/bigger_applications/app/routers/__init__.py
+-rw-r--r--   0        0        0     1012 2024-05-12 05:04:33.075447 readyapi-0.111.0.dev1/docs_src/bigger_applications/app/routers/items.py
+-rw-r--r--   0        0        0      408 2024-05-12 05:04:33.075447 readyapi-0.111.0.dev1/docs_src/bigger_applications/app/routers/users.py
+-rw-r--r--   0        0        0        0 2024-05-12 05:04:33.075447 readyapi-0.111.0.dev1/docs_src/bigger_applications/app_an/__init__.py
+-rw-r--r--   0        0        0      420 2024-05-12 05:04:33.075447 readyapi-0.111.0.dev1/docs_src/bigger_applications/app_an/dependencies.py
+-rw-r--r--   0        0        0        0 2024-05-12 05:04:33.075447 readyapi-0.111.0.dev1/docs_src/bigger_applications/app_an/internal/__init__.py
+-rw-r--r--   0        0        0      148 2024-05-12 05:04:33.075447 readyapi-0.111.0.dev1/docs_src/bigger_applications/app_an/internal/admin.py
+-rw-r--r--   0        0        0      555 2024-05-12 05:04:33.075447 readyapi-0.111.0.dev1/docs_src/bigger_applications/app_an/main.py
+-rw-r--r--   0        0        0        0 2024-05-12 05:04:33.075447 readyapi-0.111.0.dev1/docs_src/bigger_applications/app_an/routers/__init__.py
+-rw-r--r--   0        0        0     1012 2024-05-12 05:04:33.075447 readyapi-0.111.0.dev1/docs_src/bigger_applications/app_an/routers/items.py
+-rw-r--r--   0        0        0      408 2024-05-12 05:04:33.075447 readyapi-0.111.0.dev1/docs_src/bigger_applications/app_an/routers/users.py
+-rw-r--r--   0        0        0        0 2024-05-12 05:04:33.075447 readyapi-0.111.0.dev1/docs_src/bigger_applications/app_an_py39/__init__.py
+-rw-r--r--   0        0        0      410 2024-05-12 05:04:33.075447 readyapi-0.111.0.dev1/docs_src/bigger_applications/app_an_py39/dependencies.py
+-rw-r--r--   0        0        0        0 2024-05-12 05:04:33.075447 readyapi-0.111.0.dev1/docs_src/bigger_applications/app_an_py39/internal/__init__.py
+-rw-r--r--   0        0        0      148 2024-05-12 05:04:33.075447 readyapi-0.111.0.dev1/docs_src/bigger_applications/app_an_py39/internal/admin.py
+-rw-r--r--   0        0        0      555 2024-05-12 05:04:33.075447 readyapi-0.111.0.dev1/docs_src/bigger_applications/app_an_py39/main.py
+-rw-r--r--   0        0        0        0 2024-05-12 05:04:33.075447 readyapi-0.111.0.dev1/docs_src/bigger_applications/app_an_py39/routers/__init__.py
+-rw-r--r--   0        0        0     1012 2024-05-12 05:04:33.075447 readyapi-0.111.0.dev1/docs_src/bigger_applications/app_an_py39/routers/items.py
+-rw-r--r--   0        0        0      408 2024-05-12 05:04:33.075447 readyapi-0.111.0.dev1/docs_src/bigger_applications/app_an_py39/routers/users.py
+-rw-r--r--   0        0        0      312 2024-05-12 05:04:33.075447 readyapi-0.111.0.dev1/docs_src/body/tutorial001.py
+-rw-r--r--   0        0        0      274 2024-05-12 05:04:33.075447 readyapi-0.111.0.dev1/docs_src/body/tutorial001_py310.py
+-rw-r--r--   0        0        0      470 2024-05-12 05:04:33.075447 readyapi-0.111.0.dev1/docs_src/body/tutorial002.py
+-rw-r--r--   0        0        0      432 2024-05-12 05:04:33.075447 readyapi-0.111.0.dev1/docs_src/body/tutorial002_py310.py
+-rw-r--r--   0        0        0      365 2024-05-12 05:04:33.075447 readyapi-0.111.0.dev1/docs_src/body/tutorial003.py
+-rw-r--r--   0        0        0      327 2024-05-12 05:04:33.075447 readyapi-0.111.0.dev1/docs_src/body/tutorial003_py310.py
+-rw-r--r--   0        0        0      455 2024-05-12 05:04:33.075447 readyapi-0.111.0.dev1/docs_src/body/tutorial004.py
+-rw-r--r--   0        0        0      411 2024-05-12 05:04:33.075447 readyapi-0.111.0.dev1/docs_src/body/tutorial004_py310.py
+-rw-r--r--   0        0        0      564 2024-05-12 05:04:33.075447 readyapi-0.111.0.dev1/docs_src/body_fields/tutorial001.py
+-rw-r--r--   0        0        0      614 2024-05-12 05:04:33.075447 readyapi-0.111.0.dev1/docs_src/body_fields/tutorial001_an.py
+-rw-r--r--   0        0        0      566 2024-05-12 05:04:33.075447 readyapi-0.111.0.dev1/docs_src/body_fields/tutorial001_an_py310.py
+-rw-r--r--   0        0        0      585 2024-05-12 05:04:33.075447 readyapi-0.111.0.dev1/docs_src/body_fields/tutorial001_an_py39.py
+-rw-r--r--   0        0        0      526 2024-05-12 05:04:33.075447 readyapi-0.111.0.dev1/docs_src/body_fields/tutorial001_py310.py
+-rw-r--r--   0        0        0      599 2024-05-12 05:04:33.075447 readyapi-0.111.0.dev1/docs_src/body_multiple_params/tutorial001.py
+-rw-r--r--   0        0        0      642 2024-05-12 05:04:33.075447 readyapi-0.111.0.dev1/docs_src/body_multiple_params/tutorial001_an.py
+-rw-r--r--   0        0        0      582 2024-05-12 05:04:33.075447 readyapi-0.111.0.dev1/docs_src/body_multiple_params/tutorial001_an_py310.py
+-rw-r--r--   0        0        0      613 2024-05-12 05:04:33.075447 readyapi-0.111.0.dev1/docs_src/body_multiple_params/tutorial001_an_py39.py
+-rw-r--r--   0        0        0      549 2024-05-12 05:04:33.075447 readyapi-0.111.0.dev1/docs_src/body_multiple_params/tutorial001_py310.py
+-rw-r--r--   0        0        0      493 2024-05-12 05:04:33.075447 readyapi-0.111.0.dev1/docs_src/body_multiple_params/tutorial002.py
+-rw-r--r--   0        0        0      449 2024-05-12 05:04:33.075447 readyapi-0.111.0.dev1/docs_src/body_multiple_params/tutorial002_py310.py
+-rw-r--r--   0        0        0      551 2024-05-12 05:04:33.075447 readyapi-0.111.0.dev1/docs_src/body_multiple_params/tutorial003.py
+-rw-r--r--   0        0        0      607 2024-05-12 05:04:33.075447 readyapi-0.111.0.dev1/docs_src/body_multiple_params/tutorial003_an.py
+-rw-r--r--   0        0        0      553 2024-05-12 05:04:33.075447 readyapi-0.111.0.dev1/docs_src/body_multiple_params/tutorial003_an_py310.py
+-rw-r--r--   0        0        0      578 2024-05-12 05:04:33.075447 readyapi-0.111.0.dev1/docs_src/body_multiple_params/tutorial003_an_py39.py
+-rw-r--r--   0        0        0      507 2024-05-12 05:04:33.075447 readyapi-0.111.0.dev1/docs_src/body_multiple_params/tutorial003_py310.py
+-rw-r--r--   0        0        0      656 2024-05-12 05:04:33.075447 readyapi-0.111.0.dev1/docs_src/body_multiple_params/tutorial004.py
+-rw-r--r--   0        0        0      706 2024-05-12 05:04:33.075447 readyapi-0.111.0.dev1/docs_src/body_multiple_params/tutorial004_an.py
+-rw-r--r--   0        0        0      646 2024-05-12 05:04:33.075447 readyapi-0.111.0.dev1/docs_src/body_multiple_params/tutorial004_an_py310.py
+-rw-r--r--   0        0        0      677 2024-05-12 05:04:33.075447 readyapi-0.111.0.dev1/docs_src/body_multiple_params/tutorial004_an_py39.py
+-rw-r--r--   0        0        0      606 2024-05-12 05:04:33.075447 readyapi-0.111.0.dev1/docs_src/body_multiple_params/tutorial004_py310.py
+-rw-r--r--   0        0        0      410 2024-05-12 05:04:33.075447 readyapi-0.111.0.dev1/docs_src/body_multiple_params/tutorial005.py
+-rw-r--r--   0        0        0      460 2024-05-12 05:04:33.075447 readyapi-0.111.0.dev1/docs_src/body_multiple_params/tutorial005_an.py
+-rw-r--r--   0        0        0      412 2024-05-12 05:04:33.075447 readyapi-0.111.0.dev1/docs_src/body_multiple_params/tutorial005_an_py310.py
+-rw-r--r--   0        0        0      431 2024-05-12 05:04:33.075447 readyapi-0.111.0.dev1/docs_src/body_multiple_params/tutorial005_an_py39.py
+-rw-r--r--   0        0        0      372 2024-05-12 05:04:33.075447 readyapi-0.111.0.dev1/docs_src/body_multiple_params/tutorial005_py310.py
+-rw-r--r--   0        0        0      405 2024-05-12 05:04:33.075447 readyapi-0.111.0.dev1/docs_src/body_nested_models/tutorial001.py
+-rw-r--r--   0        0        0      367 2024-05-12 05:04:33.075447 readyapi-0.111.0.dev1/docs_src/body_nested_models/tutorial001_py310.py
+-rw-r--r--   0        0        0      416 2024-05-12 05:04:33.075447 readyapi-0.111.0.dev1/docs_src/body_nested_models/tutorial002.py
+-rw-r--r--   0        0        0      372 2024-05-12 05:04:33.075447 readyapi-0.111.0.dev1/docs_src/body_nested_models/tutorial002_py310.py
+-rw-r--r--   0        0        0      410 2024-05-12 05:04:33.075447 readyapi-0.111.0.dev1/docs_src/body_nested_models/tutorial002_py39.py
+-rw-r--r--   0        0        0      417 2024-05-12 05:04:33.075447 readyapi-0.111.0.dev1/docs_src/body_nested_models/tutorial003.py
+-rw-r--r--   0        0        0      374 2024-05-12 05:04:33.075447 readyapi-0.111.0.dev1/docs_src/body_nested_models/tutorial003_py310.py
+-rw-r--r--   0        0        0      412 2024-05-12 05:04:33.075447 readyapi-0.111.0.dev1/docs_src/body_nested_models/tutorial003_py39.py
+-rw-r--r--   0        0        0      507 2024-05-12 05:04:33.075447 readyapi-0.111.0.dev1/docs_src/body_nested_models/tutorial004.py
+-rw-r--r--   0        0        0      458 2024-05-12 05:04:33.075447 readyapi-0.111.0.dev1/docs_src/body_nested_models/tutorial004_py310.py
+-rw-r--r--   0        0        0      502 2024-05-12 05:04:33.075447 readyapi-0.111.0.dev1/docs_src/body_nested_models/tutorial004_py39.py
+-rw-r--r--   0        0        0      520 2024-05-12 05:04:33.075447 readyapi-0.111.0.dev1/docs_src/body_nested_models/tutorial005.py
+-rw-r--r--   0        0        0      471 2024-05-12 05:04:33.075447 readyapi-0.111.0.dev1/docs_src/body_nested_models/tutorial005_py310.py
+-rw-r--r--   0        0        0      515 2024-05-12 05:04:33.075447 readyapi-0.111.0.dev1/docs_src/body_nested_models/tutorial005_py39.py
+-rw-r--r--   0        0        0      533 2024-05-12 05:04:33.075447 readyapi-0.111.0.dev1/docs_src/body_nested_models/tutorial006.py
+-rw-r--r--   0        0        0      478 2024-05-12 05:04:33.075447 readyapi-0.111.0.dev1/docs_src/body_nested_models/tutorial006_py310.py
+-rw-r--r--   0        0        0      522 2024-05-12 05:04:33.079447 readyapi-0.111.0.dev1/docs_src/body_nested_models/tutorial006_py39.py
+-rw-r--r--   0        0        0      584 2024-05-12 05:04:33.079447 readyapi-0.111.0.dev1/docs_src/body_nested_models/tutorial007.py
+-rw-r--r--   0        0        0      523 2024-05-12 05:04:33.079447 readyapi-0.111.0.dev1/docs_src/body_nested_models/tutorial007_py310.py
+-rw-r--r--   0        0        0      573 2024-05-12 05:04:33.079447 readyapi-0.111.0.dev1/docs_src/body_nested_models/tutorial007_py39.py
+-rw-r--r--   0        0        0      276 2024-05-12 05:04:33.079447 readyapi-0.111.0.dev1/docs_src/body_nested_models/tutorial008.py
+-rw-r--r--   0        0        0      251 2024-05-12 05:04:33.079447 readyapi-0.111.0.dev1/docs_src/body_nested_models/tutorial008_py39.py
+-rw-r--r--   0        0        0      182 2024-05-12 05:04:33.079447 readyapi-0.111.0.dev1/docs_src/body_nested_models/tutorial009.py
+-rw-r--r--   0        0        0      157 2024-05-12 05:04:33.079447 readyapi-0.111.0.dev1/docs_src/body_nested_models/tutorial009_py39.py
+-rw-r--r--   0        0        0      910 2024-05-12 05:04:33.079447 readyapi-0.111.0.dev1/docs_src/body_updates/tutorial001.py
+-rw-r--r--   0        0        0      860 2024-05-12 05:04:33.079447 readyapi-0.111.0.dev1/docs_src/body_updates/tutorial001_py310.py
+-rw-r--r--   0        0        0      904 2024-05-12 05:04:33.079447 readyapi-0.111.0.dev1/docs_src/body_updates/tutorial001_py39.py
+-rw-r--r--   0        0        0     1064 2024-05-12 05:04:33.079447 readyapi-0.111.0.dev1/docs_src/body_updates/tutorial002.py
+-rw-r--r--   0        0        0     1014 2024-05-12 05:04:33.079447 readyapi-0.111.0.dev1/docs_src/body_updates/tutorial002_py310.py
+-rw-r--r--   0        0        0     1058 2024-05-12 05:04:33.079447 readyapi-0.111.0.dev1/docs_src/body_updates/tutorial002_py39.py
+-rw-r--r--   0        0        0      284 2024-05-12 05:04:33.079447 readyapi-0.111.0.dev1/docs_src/conditional_openapi/tutorial001.py
+-rw-r--r--   0        0        0      208 2024-05-12 05:04:33.079447 readyapi-0.111.0.dev1/docs_src/configure_swagger_ui/tutorial001.py
+-rw-r--r--   0        0        0      219 2024-05-12 05:04:33.079447 readyapi-0.111.0.dev1/docs_src/configure_swagger_ui/tutorial002.py
+-rw-r--r--   0        0        0      204 2024-05-12 05:04:33.079447 readyapi-0.111.0.dev1/docs_src/configure_swagger_ui/tutorial003.py
+-rw-r--r--   0        0        0      205 2024-05-12 05:04:33.079447 readyapi-0.111.0.dev1/docs_src/cookie_params/tutorial001.py
+-rw-r--r--   0        0        0      250 2024-05-12 05:04:33.079447 readyapi-0.111.0.dev1/docs_src/cookie_params/tutorial001_an.py
+-rw-r--r--   0        0        0      208 2024-05-12 05:04:33.079447 readyapi-0.111.0.dev1/docs_src/cookie_params/tutorial001_an_py310.py
+-rw-r--r--   0        0        0      221 2024-05-12 05:04:33.079447 readyapi-0.111.0.dev1/docs_src/cookie_params/tutorial001_an_py39.py
+-rw-r--r--   0        0        0      173 2024-05-12 05:04:33.079447 readyapi-0.111.0.dev1/docs_src/cookie_params/tutorial001_py310.py
+-rw-r--r--   0        0        0      467 2024-05-12 05:04:33.079447 readyapi-0.111.0.dev1/docs_src/cors/tutorial001.py
+-rw-r--r--   0        0        0     1158 2024-05-12 05:04:33.079447 readyapi-0.111.0.dev1/docs_src/custom_docs_ui/tutorial001.py
+-rw-r--r--   0        0        0     1180 2024-05-12 05:04:33.079447 readyapi-0.111.0.dev1/docs_src/custom_docs_ui/tutorial002.py
+-rw-r--r--   0        0        0      977 2024-05-12 05:04:33.079447 readyapi-0.111.0.dev1/docs_src/custom_request_and_route/tutorial001.py
+-rw-r--r--   0        0        0      937 2024-05-12 05:04:33.079447 readyapi-0.111.0.dev1/docs_src/custom_request_and_route/tutorial002.py
+-rw-r--r--   0        0        0     1046 2024-05-12 05:04:33.079447 readyapi-0.111.0.dev1/docs_src/custom_request_and_route/tutorial003.py
+-rw-r--r--   0        0        0      201 2024-05-12 05:04:33.079447 readyapi-0.111.0.dev1/docs_src/custom_response/tutorial001.py
+-rw-r--r--   0        0        0      219 2024-05-12 05:04:33.079447 readyapi-0.111.0.dev1/docs_src/custom_response/tutorial001b.py
+-rw-r--r--   0        0        0      356 2024-05-12 05:04:33.079447 readyapi-0.111.0.dev1/docs_src/custom_response/tutorial002.py
+-rw-r--r--   0        0        0      398 2024-05-12 05:04:33.079447 readyapi-0.111.0.dev1/docs_src/custom_response/tutorial003.py
+-rw-r--r--   0        0        0      495 2024-05-12 05:04:33.079447 readyapi-0.111.0.dev1/docs_src/custom_response/tutorial004.py
+-rw-r--r--   0        0        0      190 2024-05-12 05:04:33.079447 readyapi-0.111.0.dev1/docs_src/custom_response/tutorial005.py
+-rw-r--r--   0        0        0      203 2024-05-12 05:04:33.079447 readyapi-0.111.0.dev1/docs_src/custom_response/tutorial006.py
+-rw-r--r--   0        0        0      229 2024-05-12 05:04:33.079447 readyapi-0.111.0.dev1/docs_src/custom_response/tutorial006b.py
+-rw-r--r--   0        0        0      241 2024-05-12 05:04:33.079447 readyapi-0.111.0.dev1/docs_src/custom_response/tutorial006c.py
+-rw-r--r--   0        0        0      281 2024-05-12 05:04:33.079447 readyapi-0.111.0.dev1/docs_src/custom_response/tutorial007.py
+-rw-r--r--   0        0        0      364 2024-05-12 05:04:33.079447 readyapi-0.111.0.dev1/docs_src/custom_response/tutorial008.py
+-rw-r--r--   0        0        0      206 2024-05-12 05:04:33.079447 readyapi-0.111.0.dev1/docs_src/custom_response/tutorial009.py
+-rw-r--r--   0        0        0      221 2024-05-12 05:04:33.079447 readyapi-0.111.0.dev1/docs_src/custom_response/tutorial009b.py
+-rw-r--r--   0        0        0      454 2024-05-12 05:04:33.079447 readyapi-0.111.0.dev1/docs_src/custom_response/tutorial009c.py
+-rw-r--r--   0        0        0      209 2024-05-12 05:04:33.079447 readyapi-0.111.0.dev1/docs_src/custom_response/tutorial010.py
+-rw-r--r--   0        0        0      315 2024-05-12 05:04:33.079447 readyapi-0.111.0.dev1/docs_src/dataclasses/tutorial001.py
+-rw-r--r--   0        0        0      555 2024-05-12 05:04:33.079447 readyapi-0.111.0.dev1/docs_src/dataclasses/tutorial002.py
+-rw-r--r--   0        0        0     1406 2024-05-12 05:04:33.079447 readyapi-0.111.0.dev1/docs_src/dataclasses/tutorial003.py
+-rw-r--r--   0        0        0      226 2024-05-12 05:04:33.079447 readyapi-0.111.0.dev1/docs_src/debugging/tutorial001.py
+-rw-r--r--   0        0        0      445 2024-05-12 05:04:33.079447 readyapi-0.111.0.dev1/docs_src/dependencies/tutorial001.py
+-rw-r--r--   0        0        0      498 2024-05-12 05:04:33.079447 readyapi-0.111.0.dev1/docs_src/dependencies/tutorial001_02_an.py
+-rw-r--r--   0        0        0      450 2024-05-12 05:04:33.079447 readyapi-0.111.0.dev1/docs_src/dependencies/tutorial001_02_an_py310.py
+-rw-r--r--   0        0        0      469 2024-05-12 05:04:33.079447 readyapi-0.111.0.dev1/docs_src/dependencies/tutorial001_02_an_py39.py
+-rw-r--r--   0        0        0      505 2024-05-12 05:04:33.079447 readyapi-0.111.0.dev1/docs_src/dependencies/tutorial001_an.py
+-rw-r--r--   0        0        0      457 2024-05-12 05:04:33.079447 readyapi-0.111.0.dev1/docs_src/dependencies/tutorial001_an_py310.py
+-rw-r--r--   0        0        0      476 2024-05-12 05:04:33.079447 readyapi-0.111.0.dev1/docs_src/dependencies/tutorial001_an_py39.py
+-rw-r--r--   0        0        0      407 2024-05-12 05:04:33.079447 readyapi-0.111.0.dev1/docs_src/dependencies/tutorial001_py310.py
+-rw-r--r--   0        0        0      659 2024-05-12 05:04:33.079447 readyapi-0.111.0.dev1/docs_src/dependencies/tutorial002.py
+-rw-r--r--   0        0        0      709 2024-05-12 05:04:33.079447 readyapi-0.111.0.dev1/docs_src/dependencies/tutorial002_an.py
+-rw-r--r--   0        0        0      667 2024-05-12 05:04:33.079447 readyapi-0.111.0.dev1/docs_src/dependencies/tutorial002_an_py310.py
+-rw-r--r--   0        0        0      680 2024-05-12 05:04:33.079447 readyapi-0.111.0.dev1/docs_src/dependencies/tutorial002_an_py39.py
+-rw-r--r--   0        0        0      627 2024-05-12 05:04:33.079447 readyapi-0.111.0.dev1/docs_src/dependencies/tutorial002_py310.py
+-rw-r--r--   0        0        0      638 2024-05-12 05:04:33.079447 readyapi-0.111.0.dev1/docs_src/dependencies/tutorial003.py
+-rw-r--r--   0        0        0      700 2024-05-12 05:04:33.079447 readyapi-0.111.0.dev1/docs_src/dependencies/tutorial003_an.py
+-rw-r--r--   0        0        0      658 2024-05-12 05:04:33.079447 readyapi-0.111.0.dev1/docs_src/dependencies/tutorial003_an_py310.py
+-rw-r--r--   0        0        0      671 2024-05-12 05:04:33.079447 readyapi-0.111.0.dev1/docs_src/dependencies/tutorial003_an_py39.py
+-rw-r--r--   0        0        0      606 2024-05-12 05:04:33.079447 readyapi-0.111.0.dev1/docs_src/dependencies/tutorial003_py310.py
+-rw-r--r--   0        0        0      642 2024-05-12 05:04:33.079447 readyapi-0.111.0.dev1/docs_src/dependencies/tutorial004.py
+-rw-r--r--   0        0        0      692 2024-05-12 05:04:33.079447 readyapi-0.111.0.dev1/docs_src/dependencies/tutorial004_an.py
+-rw-r--r--   0        0        0      650 2024-05-12 05:04:33.079447 readyapi-0.111.0.dev1/docs_src/dependencies/tutorial004_an_py310.py
+-rw-r--r--   0        0        0      663 2024-05-12 05:04:33.079447 readyapi-0.111.0.dev1/docs_src/dependencies/tutorial004_an_py39.py
+-rw-r--r--   0        0        0      610 2024-05-12 05:04:33.079447 readyapi-0.111.0.dev1/docs_src/dependencies/tutorial004_py310.py
+-rw-r--r--   0        0        0      489 2024-05-12 05:04:33.079447 readyapi-0.111.0.dev1/docs_src/dependencies/tutorial005.py
+-rw-r--r--   0        0        0      561 2024-05-12 05:04:33.083447 readyapi-0.111.0.dev1/docs_src/dependencies/tutorial005_an.py
+-rw-r--r--   0        0        0      513 2024-05-12 05:04:33.083447 readyapi-0.111.0.dev1/docs_src/dependencies/tutorial005_an_py310.py
+-rw-r--r--   0        0        0      532 2024-05-12 05:04:33.083447 readyapi-0.111.0.dev1/docs_src/dependencies/tutorial005_an_py39.py
+-rw-r--r--   0        0        0      446 2024-05-12 05:04:33.083447 readyapi-0.111.0.dev1/docs_src/dependencies/tutorial005_py310.py
+-rw-r--r--   0        0        0      586 2024-05-12 05:04:33.083447 readyapi-0.111.0.dev1/docs_src/dependencies/tutorial006.py
+-rw-r--r--   0        0        0      646 2024-05-12 05:04:33.083447 readyapi-0.111.0.dev1/docs_src/dependencies/tutorial006_an.py
+-rw-r--r--   0        0        0      636 2024-05-12 05:04:33.083447 readyapi-0.111.0.dev1/docs_src/dependencies/tutorial006_an_py39.py
+-rw-r--r--   0        0        0       99 2024-05-12 05:04:33.083447 readyapi-0.111.0.dev1/docs_src/dependencies/tutorial007.py
+-rw-r--r--   0        0        0      456 2024-05-12 05:04:33.083447 readyapi-0.111.0.dev1/docs_src/dependencies/tutorial008.py
+-rw-r--r--   0        0        0      532 2024-05-12 05:04:33.083447 readyapi-0.111.0.dev1/docs_src/dependencies/tutorial008_an.py
+-rw-r--r--   0        0        0      522 2024-05-12 05:04:33.083447 readyapi-0.111.0.dev1/docs_src/dependencies/tutorial008_an_py39.py
+-rw-r--r--   0        0        0      738 2024-05-12 05:04:33.083447 readyapi-0.111.0.dev1/docs_src/dependencies/tutorial008b.py
+-rw-r--r--   0        0        0      788 2024-05-12 05:04:33.083447 readyapi-0.111.0.dev1/docs_src/dependencies/tutorial008b_an.py
+-rw-r--r--   0        0        0      778 2024-05-12 05:04:33.083447 readyapi-0.111.0.dev1/docs_src/dependencies/tutorial008b_an_py39.py
+-rw-r--r--   0        0        0      663 2024-05-12 05:04:33.083447 readyapi-0.111.0.dev1/docs_src/dependencies/tutorial008c.py
+-rw-r--r--   0        0        0      713 2024-05-12 05:04:33.083447 readyapi-0.111.0.dev1/docs_src/dependencies/tutorial008c_an.py
+-rw-r--r--   0        0        0      703 2024-05-12 05:04:33.083447 readyapi-0.111.0.dev1/docs_src/dependencies/tutorial008c_an_py39.py
+-rw-r--r--   0        0        0      697 2024-05-12 05:04:33.083447 readyapi-0.111.0.dev1/docs_src/dependencies/tutorial008d.py
+-rw-r--r--   0        0        0      747 2024-05-12 05:04:33.083447 readyapi-0.111.0.dev1/docs_src/dependencies/tutorial008d_an.py
+-rw-r--r--   0        0        0      737 2024-05-12 05:04:33.083447 readyapi-0.111.0.dev1/docs_src/dependencies/tutorial008d_an_py39.py
+-rw-r--r--   0        0        0      456 2024-05-12 05:04:33.083447 readyapi-0.111.0.dev1/docs_src/dependencies/tutorial009.py
+-rw-r--r--   0        0        0      292 2024-05-12 05:04:33.083447 readyapi-0.111.0.dev1/docs_src/dependencies/tutorial010.py
+-rw-r--r--   0        0        0      507 2024-05-12 05:04:33.083447 readyapi-0.111.0.dev1/docs_src/dependencies/tutorial011.py
+-rw-r--r--   0        0        0      557 2024-05-12 05:04:33.083447 readyapi-0.111.0.dev1/docs_src/dependencies/tutorial011_an.py
+-rw-r--r--   0        0        0      547 2024-05-12 05:04:33.083447 readyapi-0.111.0.dev1/docs_src/dependencies/tutorial011_an_py39.py
+-rw-r--r--   0        0        0      699 2024-05-12 05:04:33.083447 readyapi-0.111.0.dev1/docs_src/dependencies/tutorial012.py
+-rw-r--r--   0        0        0      759 2024-05-12 05:04:33.083447 readyapi-0.111.0.dev1/docs_src/dependencies/tutorial012_an.py
+-rw-r--r--   0        0        0      759 2024-05-12 05:04:33.083447 readyapi-0.111.0.dev1/docs_src/dependencies/tutorial012_an_py39.py
+-rw-r--r--   0        0        0     1526 2024-05-12 05:04:33.083447 readyapi-0.111.0.dev1/docs_src/dependency_testing/tutorial001.py
+-rw-r--r--   0        0        0     1586 2024-05-12 05:04:33.083447 readyapi-0.111.0.dev1/docs_src/dependency_testing/tutorial001_an.py
+-rw-r--r--   0        0        0     1532 2024-05-12 05:04:33.083447 readyapi-0.111.0.dev1/docs_src/dependency_testing/tutorial001_an_py310.py
+-rw-r--r--   0        0        0     1557 2024-05-12 05:04:33.083447 readyapi-0.111.0.dev1/docs_src/dependency_testing/tutorial001_an_py39.py
+-rw-r--r--   0        0        0     1482 2024-05-12 05:04:33.083447 readyapi-0.111.0.dev1/docs_src/dependency_testing/tutorial001_py310.py
+-rw-r--r--   0        0        0      465 2024-05-12 05:04:33.083447 readyapi-0.111.0.dev1/docs_src/encoder/tutorial001.py
+-rw-r--r--   0        0        0      434 2024-05-12 05:04:33.083447 readyapi-0.111.0.dev1/docs_src/encoder/tutorial001_py310.py
+-rw-r--r--   0        0        0      286 2024-05-12 05:04:33.083447 readyapi-0.111.0.dev1/docs_src/events/tutorial001.py
+-rw-r--r--   0        0        0      258 2024-05-12 05:04:33.083447 readyapi-0.111.0.dev1/docs_src/events/tutorial002.py
+-rw-r--r--   0        0        0      573 2024-05-12 05:04:33.083447 readyapi-0.111.0.dev1/docs_src/events/tutorial003.py
+-rw-r--r--   0        0        0      744 2024-05-12 05:04:33.083447 readyapi-0.111.0.dev1/docs_src/extending_openapi/tutorial001.py
+-rw-r--r--   0        0        0      833 2024-05-12 05:04:33.083447 readyapi-0.111.0.dev1/docs_src/extra_data_types/tutorial001.py
+-rw-r--r--   0        0        0      893 2024-05-12 05:04:33.083447 readyapi-0.111.0.dev1/docs_src/extra_data_types/tutorial001_an.py
+-rw-r--r--   0        0        0      833 2024-05-12 05:04:33.083447 readyapi-0.111.0.dev1/docs_src/extra_data_types/tutorial001_an_py310.py
+-rw-r--r--   0        0        0      864 2024-05-12 05:04:33.083447 readyapi-0.111.0.dev1/docs_src/extra_data_types/tutorial001_an_py39.py
+-rw-r--r--   0        0        0      784 2024-05-12 05:04:33.083447 readyapi-0.111.0.dev1/docs_src/extra_data_types/tutorial001_py310.py
+-rw-r--r--   0        0        0      946 2024-05-12 05:04:33.083447 readyapi-0.111.0.dev1/docs_src/extra_models/tutorial001.py
+-rw-r--r--   0        0        0      902 2024-05-12 05:04:33.083447 readyapi-0.111.0.dev1/docs_src/extra_models/tutorial001_py310.py
+-rw-r--r--   0        0        0      827 2024-05-12 05:04:33.083447 readyapi-0.111.0.dev1/docs_src/extra_models/tutorial002.py
+-rw-r--r--   0        0        0      795 2024-05-12 05:04:33.083447 readyapi-0.111.0.dev1/docs_src/extra_models/tutorial002_py310.py
+-rw-r--r--   0        0        0      647 2024-05-12 05:04:33.083447 readyapi-0.111.0.dev1/docs_src/extra_models/tutorial003.py
+-rw-r--r--   0        0        0      647 2024-05-12 05:04:33.083447 readyapi-0.111.0.dev1/docs_src/extra_models/tutorial003_py310.py
+-rw-r--r--   0        0        0      384 2024-05-12 05:04:33.083447 readyapi-0.111.0.dev1/docs_src/extra_models/tutorial004.py
+-rw-r--r--   0        0        0      359 2024-05-12 05:04:33.083447 readyapi-0.111.0.dev1/docs_src/extra_models/tutorial004_py39.py
+-rw-r--r--   0        0        0      208 2024-05-12 05:04:33.083447 readyapi-0.111.0.dev1/docs_src/extra_models/tutorial005.py
+-rw-r--r--   0        0        0      183 2024-05-12 05:04:33.083447 readyapi-0.111.0.dev1/docs_src/extra_models/tutorial005_py39.py
+-rw-r--r--   0        0        0      120 2024-05-12 05:04:33.083447 readyapi-0.111.0.dev1/docs_src/first_steps/tutorial001.py
+-rw-r--r--   0        0        0      142 2024-05-12 05:04:33.083447 readyapi-0.111.0.dev1/docs_src/first_steps/tutorial002.py
+-rw-r--r--   0        0        0      114 2024-05-12 05:04:33.083447 readyapi-0.111.0.dev1/docs_src/first_steps/tutorial003.py
+-rw-r--r--   0        0        0      522 2024-05-12 05:04:33.083447 readyapi-0.111.0.dev1/docs_src/generate_clients/tutorial001.py
+-rw-r--r--   0        0        0      497 2024-05-12 05:04:33.083447 readyapi-0.111.0.dev1/docs_src/generate_clients/tutorial001_py39.py
+-rw-r--r--   0        0        0      758 2024-05-12 05:04:33.083447 readyapi-0.111.0.dev1/docs_src/generate_clients/tutorial002.py
+-rw-r--r--   0        0        0      733 2024-05-12 05:04:33.083447 readyapi-0.111.0.dev1/docs_src/generate_clients/tutorial002_py39.py
+-rw-r--r--   0        0        0      943 2024-05-12 05:04:33.083447 readyapi-0.111.0.dev1/docs_src/generate_clients/tutorial003.py
+-rw-r--r--   0        0        0      918 2024-05-12 05:04:33.083447 readyapi-0.111.0.dev1/docs_src/generate_clients/tutorial003_py39.py
+-rw-r--r--   0        0        0     1066 2024-05-12 05:04:33.083447 readyapi-0.111.0.dev1/docs_src/generate_clients/tutorial004.js
+-rw-r--r--   0        0        0      493 2024-05-12 05:04:33.083447 readyapi-0.111.0.dev1/docs_src/generate_clients/tutorial004.py
+-rw-r--r--   0        0        0      449 2024-05-12 05:04:33.083447 readyapi-0.111.0.dev1/docs_src/graphql/tutorial001.py
+-rw-r--r--   0        0        0      302 2024-05-12 05:04:33.083447 readyapi-0.111.0.dev1/docs_src/handling_errors/tutorial001.py
+-rw-r--r--   0        0        0      407 2024-05-12 05:04:33.083447 readyapi-0.111.0.dev1/docs_src/handling_errors/tutorial002.py
+-rw-r--r--   0        0        0      630 2024-05-12 05:04:33.083447 readyapi-0.111.0.dev1/docs_src/handling_errors/tutorial003.py
+-rw-r--r--   0        0        0      767 2024-05-12 05:04:33.083447 readyapi-0.111.0.dev1/docs_src/handling_errors/tutorial004.py
+-rw-r--r--   0        0        0      673 2024-05-12 05:04:33.083447 readyapi-0.111.0.dev1/docs_src/handling_errors/tutorial005.py
+-rw-r--r--   0        0        0      933 2024-05-12 05:04:33.083447 readyapi-0.111.0.dev1/docs_src/handling_errors/tutorial006.py
+-rw-r--r--   0        0        0      217 2024-05-12 05:04:33.083447 readyapi-0.111.0.dev1/docs_src/header_params/tutorial001.py
+-rw-r--r--   0        0        0      262 2024-05-12 05:04:33.083447 readyapi-0.111.0.dev1/docs_src/header_params/tutorial001_an.py
+-rw-r--r--   0        0        0      220 2024-05-12 05:04:33.083447 readyapi-0.111.0.dev1/docs_src/header_params/tutorial001_an_py310.py
+-rw-r--r--   0        0        0      233 2024-05-12 05:04:33.083447 readyapi-0.111.0.dev1/docs_src/header_params/tutorial001_an_py39.py
+-rw-r--r--   0        0        0      185 2024-05-12 05:04:33.083447 readyapi-0.111.0.dev1/docs_src/header_params/tutorial001_py310.py
+-rw-r--r--   0        0        0      263 2024-05-12 05:04:33.083447 readyapi-0.111.0.dev1/docs_src/header_params/tutorial002.py
+-rw-r--r--   0        0        0      320 2024-05-12 05:04:33.083447 readyapi-0.111.0.dev1/docs_src/header_params/tutorial002_an.py
+-rw-r--r--   0        0        0      264 2024-05-12 05:04:33.083447 readyapi-0.111.0.dev1/docs_src/header_params/tutorial002_an_py310.py
+-rw-r--r--   0        0        0      291 2024-05-12 05:04:33.083447 readyapi-0.111.0.dev1/docs_src/header_params/tutorial002_an_py39.py
+-rw-r--r--   0        0        0      231 2024-05-12 05:04:33.083447 readyapi-0.111.0.dev1/docs_src/header_params/tutorial002_py310.py
+-rw-r--r--   0        0        0      227 2024-05-12 05:04:33.083447 readyapi-0.111.0.dev1/docs_src/header_params/tutorial003.py
+-rw-r--r--   0        0        0      272 2024-05-12 05:04:33.083447 readyapi-0.111.0.dev1/docs_src/header_params/tutorial003_an.py
+-rw-r--r--   0        0        0      224 2024-05-12 05:04:33.083447 readyapi-0.111.0.dev1/docs_src/header_params/tutorial003_an_py310.py
+-rw-r--r--   0        0        0      243 2024-05-12 05:04:33.083447 readyapi-0.111.0.dev1/docs_src/header_params/tutorial003_an_py39.py
+-rw-r--r--   0        0        0      189 2024-05-12 05:04:33.083447 readyapi-0.111.0.dev1/docs_src/header_params/tutorial003_py310.py
+-rw-r--r--   0        0        0      221 2024-05-12 05:04:33.083447 readyapi-0.111.0.dev1/docs_src/header_params/tutorial003_py39.py
+-rw-r--r--   0        0        0      808 2024-05-12 05:04:33.083447 readyapi-0.111.0.dev1/docs_src/metadata/tutorial001.py
+-rw-r--r--   0        0        0      770 2024-05-12 05:04:33.083447 readyapi-0.111.0.dev1/docs_src/metadata/tutorial001_1.py
+-rw-r--r--   0        0        0      157 2024-05-12 05:04:33.083447 readyapi-0.111.0.dev1/docs_src/metadata/tutorial002.py
+-rw-r--r--   0        0        0      164 2024-05-12 05:04:33.083447 readyapi-0.111.0.dev1/docs_src/metadata/tutorial003.py
+-rw-r--r--   0        0        0      699 2024-05-12 05:04:33.083447 readyapi-0.111.0.dev1/docs_src/metadata/tutorial004.py
+-rw-r--r--   0        0        0      352 2024-05-12 05:04:33.083447 readyapi-0.111.0.dev1/docs_src/middleware/tutorial001.py
+-rw-r--r--   0        0        0     1361 2024-05-12 05:04:33.083447 readyapi-0.111.0.dev1/docs_src/nosql_databases/tutorial001.py
+-rw-r--r--   0        0        0     1374 2024-05-12 05:04:33.083447 readyapi-0.111.0.dev1/docs_src/openapi_callbacks/tutorial001.py
+-rw-r--r--   0        0        0      553 2024-05-12 05:04:33.083447 readyapi-0.111.0.dev1/docs_src/openapi_webhooks/tutorial001.py
+-rw-r--r--   0        0        0      170 2024-05-12 05:04:33.087447 readyapi-0.111.0.dev1/docs_src/path_operation_advanced_configuration/tutorial001.py
+-rw-r--r--   0        0        0      577 2024-05-12 05:04:33.087447 readyapi-0.111.0.dev1/docs_src/path_operation_advanced_configuration/tutorial002.py
+-rw-r--r--   0        0        0      151 2024-05-12 05:04:33.087447 readyapi-0.111.0.dev1/docs_src/path_operation_advanced_configuration/tutorial003.py
+-rw-r--r--   0        0        0      720 2024-05-12 05:04:33.087447 readyapi-0.111.0.dev1/docs_src/path_operation_advanced_configuration/tutorial004.py
+-rw-r--r--   0        0        0      183 2024-05-12 05:04:33.087447 readyapi-0.111.0.dev1/docs_src/path_operation_advanced_configuration/tutorial005.py
+-rw-r--r--   0        0        0     1046 2024-05-12 05:04:33.087447 readyapi-0.111.0.dev1/docs_src/path_operation_advanced_configuration/tutorial006.py
+-rw-r--r--   0        0        0      825 2024-05-12 05:04:33.087447 readyapi-0.111.0.dev1/docs_src/path_operation_advanced_configuration/tutorial007.py
+-rw-r--r--   0        0        0      792 2024-05-12 05:04:33.087447 readyapi-0.111.0.dev1/docs_src/path_operation_advanced_configuration/tutorial007_pv1.py
+-rw-r--r--   0        0        0      409 2024-05-12 05:04:33.087447 readyapi-0.111.0.dev1/docs_src/path_operation_configuration/tutorial001.py
+-rw-r--r--   0        0        0      366 2024-05-12 05:04:33.087447 readyapi-0.111.0.dev1/docs_src/path_operation_configuration/tutorial001_py310.py
+-rw-r--r--   0        0        0      404 2024-05-12 05:04:33.087447 readyapi-0.111.0.dev1/docs_src/path_operation_configuration/tutorial001_py39.py
+-rw-r--r--   0        0        0      583 2024-05-12 05:04:33.087447 readyapi-0.111.0.dev1/docs_src/path_operation_configuration/tutorial002.py
+-rw-r--r--   0        0        0      540 2024-05-12 05:04:33.087447 readyapi-0.111.0.dev1/docs_src/path_operation_configuration/tutorial002_py310.py
+-rw-r--r--   0        0        0      578 2024-05-12 05:04:33.087447 readyapi-0.111.0.dev1/docs_src/path_operation_configuration/tutorial002_py39.py
+-rw-r--r--   0        0        0      326 2024-05-12 05:04:33.087447 readyapi-0.111.0.dev1/docs_src/path_operation_configuration/tutorial002b.py
+-rw-r--r--   0        0        0      520 2024-05-12 05:04:33.087447 readyapi-0.111.0.dev1/docs_src/path_operation_configuration/tutorial003.py
+-rw-r--r--   0        0        0      477 2024-05-12 05:04:33.087447 readyapi-0.111.0.dev1/docs_src/path_operation_configuration/tutorial003_py310.py
+-rw-r--r--   0        0        0      515 2024-05-12 05:04:33.087447 readyapi-0.111.0.dev1/docs_src/path_operation_configuration/tutorial003_py39.py
+-rw-r--r--   0        0        0      684 2024-05-12 05:04:33.087447 readyapi-0.111.0.dev1/docs_src/path_operation_configuration/tutorial004.py
+-rw-r--r--   0        0        0      641 2024-05-12 05:04:33.087447 readyapi-0.111.0.dev1/docs_src/path_operation_configuration/tutorial004_py310.py
+-rw-r--r--   0        0        0      679 2024-05-12 05:04:33.087447 readyapi-0.111.0.dev1/docs_src/path_operation_configuration/tutorial004_py39.py
+-rw-r--r--   0        0        0      744 2024-05-12 05:04:33.087447 readyapi-0.111.0.dev1/docs_src/path_operation_configuration/tutorial005.py
+-rw-r--r--   0        0        0      701 2024-05-12 05:04:33.087447 readyapi-0.111.0.dev1/docs_src/path_operation_configuration/tutorial005_py310.py
+-rw-r--r--   0        0        0      739 2024-05-12 05:04:33.087447 readyapi-0.111.0.dev1/docs_src/path_operation_configuration/tutorial005_py39.py
+-rw-r--r--   0        0        0      368 2024-05-12 05:04:33.087447 readyapi-0.111.0.dev1/docs_src/path_operation_configuration/tutorial006.py
+-rw-r--r--   0        0        0      141 2024-05-12 05:04:33.087447 readyapi-0.111.0.dev1/docs_src/path_params/tutorial001.py
+-rw-r--r--   0        0        0      146 2024-05-12 05:04:33.087447 readyapi-0.111.0.dev1/docs_src/path_params/tutorial002.py
+-rw-r--r--   0        0        0      239 2024-05-12 05:04:33.087447 readyapi-0.111.0.dev1/docs_src/path_params/tutorial003.py
+-rw-r--r--   0        0        0      196 2024-05-12 05:04:33.087447 readyapi-0.111.0.dev1/docs_src/path_params/tutorial003b.py
+-rw-r--r--   0        0        0      159 2024-05-12 05:04:33.087447 readyapi-0.111.0.dev1/docs_src/path_params/tutorial004.py
+-rw-r--r--   0        0        0      549 2024-05-12 05:04:33.087447 readyapi-0.111.0.dev1/docs_src/path_params/tutorial005.py
+-rw-r--r--   0        0        0      367 2024-05-12 05:04:33.087447 readyapi-0.111.0.dev1/docs_src/path_params_numeric_validations/tutorial001.py
+-rw-r--r--   0        0        0      420 2024-05-12 05:04:33.087447 readyapi-0.111.0.dev1/docs_src/path_params_numeric_validations/tutorial001_an.py
+-rw-r--r--   0        0        0      378 2024-05-12 05:04:33.087447 readyapi-0.111.0.dev1/docs_src/path_params_numeric_validations/tutorial001_an_py310.py
+-rw-r--r--   0        0        0      391 2024-05-12 05:04:33.087447 readyapi-0.111.0.dev1/docs_src/path_params_numeric_validations/tutorial001_an_py39.py
+-rw-r--r--   0        0        0      335 2024-05-12 05:04:33.087447 readyapi-0.111.0.dev1/docs_src/path_params_numeric_validations/tutorial001_py310.py
+-rw-r--r--   0        0        0      268 2024-05-12 05:04:33.087447 readyapi-0.111.0.dev1/docs_src/path_params_numeric_validations/tutorial002.py
+-rw-r--r--   0        0        0      324 2024-05-12 05:04:33.087447 readyapi-0.111.0.dev1/docs_src/path_params_numeric_validations/tutorial002_an.py
+-rw-r--r--   0        0        0      314 2024-05-12 05:04:33.087447 readyapi-0.111.0.dev1/docs_src/path_params_numeric_validations/tutorial002_an_py39.py
+-rw-r--r--   0        0        0      271 2024-05-12 05:04:33.087447 readyapi-0.111.0.dev1/docs_src/path_params_numeric_validations/tutorial003.py
+-rw-r--r--   0        0        0      324 2024-05-12 05:04:33.087447 readyapi-0.111.0.dev1/docs_src/path_params_numeric_validations/tutorial003_an.py
+-rw-r--r--   0        0        0      314 2024-05-12 05:04:33.087447 readyapi-0.111.0.dev1/docs_src/path_params_numeric_validations/tutorial003_an_py39.py
+-rw-r--r--   0        0        0      283 2024-05-12 05:04:33.087447 readyapi-0.111.0.dev1/docs_src/path_params_numeric_validations/tutorial004.py
+-rw-r--r--   0        0        0      330 2024-05-12 05:04:33.087447 readyapi-0.111.0.dev1/docs_src/path_params_numeric_validations/tutorial004_an.py
+-rw-r--r--   0        0        0      320 2024-05-12 05:04:33.087447 readyapi-0.111.0.dev1/docs_src/path_params_numeric_validations/tutorial004_an_py39.py
+-rw-r--r--   0        0        0      301 2024-05-12 05:04:33.087447 readyapi-0.111.0.dev1/docs_src/path_params_numeric_validations/tutorial005.py
+-rw-r--r--   0        0        0      344 2024-05-12 05:04:33.087447 readyapi-0.111.0.dev1/docs_src/path_params_numeric_validations/tutorial005_an.py
+-rw-r--r--   0        0        0      334 2024-05-12 05:04:33.087447 readyapi-0.111.0.dev1/docs_src/path_params_numeric_validations/tutorial005_an_py39.py
+-rw-r--r--   0        0        0      348 2024-05-12 05:04:33.087447 readyapi-0.111.0.dev1/docs_src/path_params_numeric_validations/tutorial006.py
+-rw-r--r--   0        0        0      408 2024-05-12 05:04:33.087447 readyapi-0.111.0.dev1/docs_src/path_params_numeric_validations/tutorial006_an.py
+-rw-r--r--   0        0        0      398 2024-05-12 05:04:33.087447 readyapi-0.111.0.dev1/docs_src/path_params_numeric_validations/tutorial006_an_py39.py
+-rw-r--r--   0        0        0      162 2024-05-12 05:04:33.087447 readyapi-0.111.0.dev1/docs_src/python_types/tutorial001.py
+-rw-r--r--   0        0        0      172 2024-05-12 05:04:33.087447 readyapi-0.111.0.dev1/docs_src/python_types/tutorial002.py
+-rw-r--r--   0        0        0      119 2024-05-12 05:04:33.087447 readyapi-0.111.0.dev1/docs_src/python_types/tutorial003.py
+-rw-r--r--   0        0        0      124 2024-05-12 05:04:33.087447 readyapi-0.111.0.dev1/docs_src/python_types/tutorial004.py
+-rw-r--r--   0        0        0      143 2024-05-12 05:04:33.087447 readyapi-0.111.0.dev1/docs_src/python_types/tutorial005.py
+-rw-r--r--   0        0        0      106 2024-05-12 05:04:33.087447 readyapi-0.111.0.dev1/docs_src/python_types/tutorial006.py
+-rw-r--r--   0        0        0       80 2024-05-12 05:04:33.087447 readyapi-0.111.0.dev1/docs_src/python_types/tutorial006_py39.py
+-rw-r--r--   0        0        0      131 2024-05-12 05:04:33.087447 readyapi-0.111.0.dev1/docs_src/python_types/tutorial007.py
+-rw-r--r--   0        0        0       99 2024-05-12 05:04:33.087447 readyapi-0.111.0.dev1/docs_src/python_types/tutorial007_py39.py
+-rw-r--r--   0        0        0      171 2024-05-12 05:04:33.087447 readyapi-0.111.0.dev1/docs_src/python_types/tutorial008.py
+-rw-r--r--   0        0        0      145 2024-05-12 05:04:33.087447 readyapi-0.111.0.dev1/docs_src/python_types/tutorial008_py39.py
+-rw-r--r--   0        0        0       84 2024-05-12 05:04:33.087447 readyapi-0.111.0.dev1/docs_src/python_types/tutorial008b.py
+-rw-r--r--   0        0        0       51 2024-05-12 05:04:33.087447 readyapi-0.111.0.dev1/docs_src/python_types/tutorial008b_py310.py
+-rw-r--r--   0        0        0      164 2024-05-12 05:04:33.087447 readyapi-0.111.0.dev1/docs_src/python_types/tutorial009.py
+-rw-r--r--   0        0        0      131 2024-05-12 05:04:33.087447 readyapi-0.111.0.dev1/docs_src/python_types/tutorial009_py310.py
+-rw-r--r--   0        0        0      164 2024-05-12 05:04:33.087447 readyapi-0.111.0.dev1/docs_src/python_types/tutorial009b.py
+-rw-r--r--   0        0        0       89 2024-05-12 05:04:33.087447 readyapi-0.111.0.dev1/docs_src/python_types/tutorial009c.py
+-rw-r--r--   0        0        0       56 2024-05-12 05:04:33.087447 readyapi-0.111.0.dev1/docs_src/python_types/tutorial009c_py310.py
+-rw-r--r--   0        0        0      144 2024-05-12 05:04:33.087447 readyapi-0.111.0.dev1/docs_src/python_types/tutorial010.py
+-rw-r--r--   0        0        0      498 2024-05-12 05:04:33.087447 readyapi-0.111.0.dev1/docs_src/python_types/tutorial011.py
+-rw-r--r--   0        0        0      461 2024-05-12 05:04:33.087447 readyapi-0.111.0.dev1/docs_src/python_types/tutorial011_py310.py
+-rw-r--r--   0        0        0      492 2024-05-12 05:04:33.087447 readyapi-0.111.0.dev1/docs_src/python_types/tutorial011_py39.py
+-rw-r--r--   0        0        0      122 2024-05-12 05:04:33.087447 readyapi-0.111.0.dev1/docs_src/python_types/tutorial012.py
+-rw-r--r--   0        0        0      138 2024-05-12 05:04:33.087447 readyapi-0.111.0.dev1/docs_src/python_types/tutorial013.py
+-rw-r--r--   0        0        0      127 2024-05-12 05:04:33.087447 readyapi-0.111.0.dev1/docs_src/python_types/tutorial013_py39.py
+-rw-r--r--   0        0        0      253 2024-05-12 05:04:33.087447 readyapi-0.111.0.dev1/docs_src/query_params/tutorial001.py
+-rw-r--r--   0        0        0      254 2024-05-12 05:04:33.087447 readyapi-0.111.0.dev1/docs_src/query_params/tutorial002.py
+-rw-r--r--   0        0        0      222 2024-05-12 05:04:33.087447 readyapi-0.111.0.dev1/docs_src/query_params/tutorial002_py310.py
+-rw-r--r--   0        0        0      409 2024-05-12 05:04:33.087447 readyapi-0.111.0.dev1/docs_src/query_params/tutorial003.py
+-rw-r--r--   0        0        0      377 2024-05-12 05:04:33.087447 readyapi-0.111.0.dev1/docs_src/query_params/tutorial003_py310.py
+-rw-r--r--   0        0        0      471 2024-05-12 05:04:33.087447 readyapi-0.111.0.dev1/docs_src/query_params/tutorial004.py
+-rw-r--r--   0        0        0      439 2024-05-12 05:04:33.087447 readyapi-0.111.0.dev1/docs_src/query_params/tutorial004_py310.py
+-rw-r--r--   0        0        0      195 2024-05-12 05:04:33.087447 readyapi-0.111.0.dev1/docs_src/query_params/tutorial005.py
+-rw-r--r--   0        0        0      304 2024-05-12 05:04:33.087447 readyapi-0.111.0.dev1/docs_src/query_params/tutorial006.py
+-rw-r--r--   0        0        0      272 2024-05-12 05:04:33.087447 readyapi-0.111.0.dev1/docs_src/query_params/tutorial006_py310.py
+-rw-r--r--   0        0        0      304 2024-05-12 05:04:33.087447 readyapi-0.111.0.dev1/docs_src/query_params/tutorial006b.py
+-rw-r--r--   0        0        0      274 2024-05-12 05:04:33.087447 readyapi-0.111.0.dev1/docs_src/query_params_str_validations/tutorial001.py
+-rw-r--r--   0        0        0      242 2024-05-12 05:04:33.087447 readyapi-0.111.0.dev1/docs_src/query_params_str_validations/tutorial001_py310.py
+-rw-r--r--   0        0        0      311 2024-05-12 05:04:33.087447 readyapi-0.111.0.dev1/docs_src/query_params_str_validations/tutorial002.py
+-rw-r--r--   0        0        0      354 2024-05-12 05:04:33.087447 readyapi-0.111.0.dev1/docs_src/query_params_str_validations/tutorial002_an.py
+-rw-r--r--   0        0        0      312 2024-05-12 05:04:33.087447 readyapi-0.111.0.dev1/docs_src/query_params_str_validations/tutorial002_an_py310.py
+-rw-r--r--   0        0        0      279 2024-05-12 05:04:33.087447 readyapi-0.111.0.dev1/docs_src/query_params_str_validations/tutorial002_py310.py
+-rw-r--r--   0        0        0      332 2024-05-12 05:04:33.087447 readyapi-0.111.0.dev1/docs_src/query_params_str_validations/tutorial003.py
+-rw-r--r--   0        0        0      375 2024-05-12 05:04:33.087447 readyapi-0.111.0.dev1/docs_src/query_params_str_validations/tutorial003_an.py
+-rw-r--r--   0        0        0      333 2024-05-12 05:04:33.087447 readyapi-0.111.0.dev1/docs_src/query_params_str_validations/tutorial003_an_py310.py
+-rw-r--r--   0        0        0      346 2024-05-12 05:04:33.087447 readyapi-0.111.0.dev1/docs_src/query_params_str_validations/tutorial003_an_py39.py
+-rw-r--r--   0        0        0      293 2024-05-12 05:04:33.087447 readyapi-0.111.0.dev1/docs_src/query_params_str_validations/tutorial003_py310.py
+-rw-r--r--   0        0        0      370 2024-05-12 05:04:33.087447 readyapi-0.111.0.dev1/docs_src/query_params_str_validations/tutorial004.py
+-rw-r--r--   0        0        0      413 2024-05-12 05:04:33.087447 readyapi-0.111.0.dev1/docs_src/query_params_str_validations/tutorial004_an.py
+-rw-r--r--   0        0        0      371 2024-05-12 05:04:33.087447 readyapi-0.111.0.dev1/docs_src/query_params_str_validations/tutorial004_an_py310.py
+-rw-r--r--   0        0        0      369 2024-05-12 05:04:33.087447 readyapi-0.111.0.dev1/docs_src/query_params_str_validations/tutorial004_an_py310_regex.py
+-rw-r--r--   0        0        0      384 2024-05-12 05:04:33.087447 readyapi-0.111.0.dev1/docs_src/query_params_str_validations/tutorial004_an_py39.py
+-rw-r--r--   0        0        0      338 2024-05-12 05:04:33.087447 readyapi-0.111.0.dev1/docs_src/query_params_str_validations/tutorial004_py310.py
+-rw-r--r--   0        0        0      279 2024-05-12 05:04:33.087447 readyapi-0.111.0.dev1/docs_src/query_params_str_validations/tutorial005.py
+-rw-r--r--   0        0        0      322 2024-05-12 05:04:33.087447 readyapi-0.111.0.dev1/docs_src/query_params_str_validations/tutorial005_an.py
+-rw-r--r--   0        0        0      312 2024-05-12 05:04:33.087447 readyapi-0.111.0.dev1/docs_src/query_params_str_validations/tutorial005_an_py39.py
+-rw-r--r--   0        0        0      257 2024-05-12 05:04:33.087447 readyapi-0.111.0.dev1/docs_src/query_params_str_validations/tutorial006.py
+-rw-r--r--   0        0        0      307 2024-05-12 05:04:33.087447 readyapi-0.111.0.dev1/docs_src/query_params_str_validations/tutorial006_an.py
+-rw-r--r--   0        0        0      297 2024-05-12 05:04:33.091447 readyapi-0.111.0.dev1/docs_src/query_params_str_validations/tutorial006_an_py39.py
+-rw-r--r--   0        0        0      270 2024-05-12 05:04:33.091447 readyapi-0.111.0.dev1/docs_src/query_params_str_validations/tutorial006b.py
+-rw-r--r--   0        0        0      313 2024-05-12 05:04:33.091447 readyapi-0.111.0.dev1/docs_src/query_params_str_validations/tutorial006b_an.py
+-rw-r--r--   0        0        0      303 2024-05-12 05:04:33.091447 readyapi-0.111.0.dev1/docs_src/query_params_str_validations/tutorial006b_an_py39.py
+-rw-r--r--   0        0        0      309 2024-05-12 05:04:33.091447 readyapi-0.111.0.dev1/docs_src/query_params_str_validations/tutorial006c.py
+-rw-r--r--   0        0        0      352 2024-05-12 05:04:33.091447 readyapi-0.111.0.dev1/docs_src/query_params_str_validations/tutorial006c_an.py
+-rw-r--r--   0        0        0      310 2024-05-12 05:04:33.091447 readyapi-0.111.0.dev1/docs_src/query_params_str_validations/tutorial006c_an_py310.py
+-rw-r--r--   0        0        0      323 2024-05-12 05:04:33.091447 readyapi-0.111.0.dev1/docs_src/query_params_str_validations/tutorial006c_an_py39.py
+-rw-r--r--   0        0        0      277 2024-05-12 05:04:33.091447 readyapi-0.111.0.dev1/docs_src/query_params_str_validations/tutorial006c_py310.py
+-rw-r--r--   0        0        0      305 2024-05-12 05:04:33.091447 readyapi-0.111.0.dev1/docs_src/query_params_str_validations/tutorial006d.py
+-rw-r--r--   0        0        0      348 2024-05-12 05:04:33.091447 readyapi-0.111.0.dev1/docs_src/query_params_str_validations/tutorial006d_an.py
+-rw-r--r--   0        0        0      338 2024-05-12 05:04:33.091447 readyapi-0.111.0.dev1/docs_src/query_params_str_validations/tutorial006d_an_py39.py
+-rw-r--r--   0        0        0      339 2024-05-12 05:04:33.091447 readyapi-0.111.0.dev1/docs_src/query_params_str_validations/tutorial007.py
+-rw-r--r--   0        0        0      382 2024-05-12 05:04:33.091447 readyapi-0.111.0.dev1/docs_src/query_params_str_validations/tutorial007_an.py
+-rw-r--r--   0        0        0      340 2024-05-12 05:04:33.091447 readyapi-0.111.0.dev1/docs_src/query_params_str_validations/tutorial007_an_py310.py
+-rw-r--r--   0        0        0      353 2024-05-12 05:04:33.091447 readyapi-0.111.0.dev1/docs_src/query_params_str_validations/tutorial007_an_py39.py
+-rw-r--r--   0        0        0      307 2024-05-12 05:04:33.091447 readyapi-0.111.0.dev1/docs_src/query_params_str_validations/tutorial007_py310.py
+-rw-r--r--   0        0        0      469 2024-05-12 05:04:33.091447 readyapi-0.111.0.dev1/docs_src/query_params_str_validations/tutorial008.py
+-rw-r--r--   0        0        0      543 2024-05-12 05:04:33.091447 readyapi-0.111.0.dev1/docs_src/query_params_str_validations/tutorial008_an.py
+-rw-r--r--   0        0        0      501 2024-05-12 05:04:33.091447 readyapi-0.111.0.dev1/docs_src/query_params_str_validations/tutorial008_an_py310.py
+-rw-r--r--   0        0        0      514 2024-05-12 05:04:33.091447 readyapi-0.111.0.dev1/docs_src/query_params_str_validations/tutorial008_an_py39.py
+-rw-r--r--   0        0        0      437 2024-05-12 05:04:33.091447 readyapi-0.111.0.dev1/docs_src/query_params_str_validations/tutorial008_py310.py
+-rw-r--r--   0        0        0      316 2024-05-12 05:04:33.091447 readyapi-0.111.0.dev1/docs_src/query_params_str_validations/tutorial009.py
+-rw-r--r--   0        0        0      359 2024-05-12 05:04:33.091447 readyapi-0.111.0.dev1/docs_src/query_params_str_validations/tutorial009_an.py
+-rw-r--r--   0        0        0      317 2024-05-12 05:04:33.091447 readyapi-0.111.0.dev1/docs_src/query_params_str_validations/tutorial009_an_py310.py
+-rw-r--r--   0        0        0      330 2024-05-12 05:04:33.091447 readyapi-0.111.0.dev1/docs_src/query_params_str_validations/tutorial009_an_py39.py
+-rw-r--r--   0        0        0      284 2024-05-12 05:04:33.091447 readyapi-0.111.0.dev1/docs_src/query_params_str_validations/tutorial009_py310.py
+-rw-r--r--   0        0        0      577 2024-05-12 05:04:33.091447 readyapi-0.111.0.dev1/docs_src/query_params_str_validations/tutorial010.py
+-rw-r--r--   0        0        0      667 2024-05-12 05:04:33.091447 readyapi-0.111.0.dev1/docs_src/query_params_str_validations/tutorial010_an.py
+-rw-r--r--   0        0        0      625 2024-05-12 05:04:33.091447 readyapi-0.111.0.dev1/docs_src/query_params_str_validations/tutorial010_an_py310.py
+-rw-r--r--   0        0        0      638 2024-05-12 05:04:33.091447 readyapi-0.111.0.dev1/docs_src/query_params_str_validations/tutorial010_an_py39.py
+-rw-r--r--   0        0        0      545 2024-05-12 05:04:33.091447 readyapi-0.111.0.dev1/docs_src/query_params_str_validations/tutorial010_py310.py
+-rw-r--r--   0        0        0      230 2024-05-12 05:04:33.091447 readyapi-0.111.0.dev1/docs_src/query_params_str_validations/tutorial011.py
+-rw-r--r--   0        0        0      275 2024-05-12 05:04:33.091447 readyapi-0.111.0.dev1/docs_src/query_params_str_validations/tutorial011_an.py
+-rw-r--r--   0        0        0      227 2024-05-12 05:04:33.091447 readyapi-0.111.0.dev1/docs_src/query_params_str_validations/tutorial011_an_py310.py
+-rw-r--r--   0        0        0      240 2024-05-12 05:04:33.091447 readyapi-0.111.0.dev1/docs_src/query_params_str_validations/tutorial011_an_py39.py
+-rw-r--r--   0        0        0      192 2024-05-12 05:04:33.091447 readyapi-0.111.0.dev1/docs_src/query_params_str_validations/tutorial011_py310.py
+-rw-r--r--   0        0        0      224 2024-05-12 05:04:33.091447 readyapi-0.111.0.dev1/docs_src/query_params_str_validations/tutorial011_py39.py
+-rw-r--r--   0        0        0      220 2024-05-12 05:04:33.091447 readyapi-0.111.0.dev1/docs_src/query_params_str_validations/tutorial012.py
+-rw-r--r--   0        0        0      265 2024-05-12 05:04:33.091447 readyapi-0.111.0.dev1/docs_src/query_params_str_validations/tutorial012_an.py
+-rw-r--r--   0        0        0      230 2024-05-12 05:04:33.091447 readyapi-0.111.0.dev1/docs_src/query_params_str_validations/tutorial012_an_py39.py
+-rw-r--r--   0        0        0      195 2024-05-12 05:04:33.091447 readyapi-0.111.0.dev1/docs_src/query_params_str_validations/tutorial012_py39.py
+-rw-r--r--   0        0        0      178 2024-05-12 05:04:33.091447 readyapi-0.111.0.dev1/docs_src/query_params_str_validations/tutorial013.py
+-rw-r--r--   0        0        0      223 2024-05-12 05:04:33.091447 readyapi-0.111.0.dev1/docs_src/query_params_str_validations/tutorial013_an.py
+-rw-r--r--   0        0        0      213 2024-05-12 05:04:33.091447 readyapi-0.111.0.dev1/docs_src/query_params_str_validations/tutorial013_an_py39.py
+-rw-r--r--   0        0        0      333 2024-05-12 05:04:33.091447 readyapi-0.111.0.dev1/docs_src/query_params_str_validations/tutorial014.py
+-rw-r--r--   0        0        0      376 2024-05-12 05:04:33.091447 readyapi-0.111.0.dev1/docs_src/query_params_str_validations/tutorial014_an.py
+-rw-r--r--   0        0        0      334 2024-05-12 05:04:33.091447 readyapi-0.111.0.dev1/docs_src/query_params_str_validations/tutorial014_an_py310.py
+-rw-r--r--   0        0        0      347 2024-05-12 05:04:33.091447 readyapi-0.111.0.dev1/docs_src/query_params_str_validations/tutorial014_an_py39.py
+-rw-r--r--   0        0        0      301 2024-05-12 05:04:33.091447 readyapi-0.111.0.dev1/docs_src/query_params_str_validations/tutorial014_py310.py
+-rw-r--r--   0        0        0      285 2024-05-12 05:04:33.091447 readyapi-0.111.0.dev1/docs_src/request_files/tutorial001.py
+-rw-r--r--   0        0        0      511 2024-05-12 05:04:33.091447 readyapi-0.111.0.dev1/docs_src/request_files/tutorial001_02.py
+-rw-r--r--   0        0        0      556 2024-05-12 05:04:33.091447 readyapi-0.111.0.dev1/docs_src/request_files/tutorial001_02_an.py
+-rw-r--r--   0        0        0      508 2024-05-12 05:04:33.091447 readyapi-0.111.0.dev1/docs_src/request_files/tutorial001_02_an_py310.py
+-rw-r--r--   0        0        0      527 2024-05-12 05:04:33.091447 readyapi-0.111.0.dev1/docs_src/request_files/tutorial001_02_an_py39.py
+-rw-r--r--   0        0        0      473 2024-05-12 05:04:33.091447 readyapi-0.111.0.dev1/docs_src/request_files/tutorial001_02_py310.py
+-rw-r--r--   0        0        0      374 2024-05-12 05:04:33.091447 readyapi-0.111.0.dev1/docs_src/request_files/tutorial001_03.py
+-rw-r--r--   0        0        0      434 2024-05-12 05:04:33.091447 readyapi-0.111.0.dev1/docs_src/request_files/tutorial001_03_an.py
+-rw-r--r--   0        0        0      424 2024-05-12 05:04:33.091447 readyapi-0.111.0.dev1/docs_src/request_files/tutorial001_03_an_py39.py
+-rw-r--r--   0        0        0      335 2024-05-12 05:04:33.091447 readyapi-0.111.0.dev1/docs_src/request_files/tutorial001_an.py
+-rw-r--r--   0        0        0      325 2024-05-12 05:04:33.091447 readyapi-0.111.0.dev1/docs_src/request_files/tutorial001_an_py39.py
+-rw-r--r--   0        0        0      815 2024-05-12 05:04:33.091447 readyapi-0.111.0.dev1/docs_src/request_files/tutorial002.py
+-rw-r--r--   0        0        0      865 2024-05-12 05:04:33.091447 readyapi-0.111.0.dev1/docs_src/request_files/tutorial002_an.py
+-rw-r--r--   0        0        0      830 2024-05-12 05:04:33.091447 readyapi-0.111.0.dev1/docs_src/request_files/tutorial002_an_py39.py
+-rw-r--r--   0        0        0      790 2024-05-12 05:04:33.091447 readyapi-0.111.0.dev1/docs_src/request_files/tutorial002_py39.py
+-rw-r--r--   0        0        0      917 2024-05-12 05:04:33.091447 readyapi-0.111.0.dev1/docs_src/request_files/tutorial003.py
+-rw-r--r--   0        0        0      991 2024-05-12 05:04:33.091447 readyapi-0.111.0.dev1/docs_src/request_files/tutorial003_an.py
+-rw-r--r--   0        0        0      956 2024-05-12 05:04:33.091447 readyapi-0.111.0.dev1/docs_src/request_files/tutorial003_an_py39.py
+-rw-r--r--   0        0        0      892 2024-05-12 05:04:33.091447 readyapi-0.111.0.dev1/docs_src/request_files/tutorial003_py39.py
+-rw-r--r--   0        0        0      176 2024-05-12 05:04:33.091447 readyapi-0.111.0.dev1/docs_src/request_forms/tutorial001.py
+-rw-r--r--   0        0        0      236 2024-05-12 05:04:33.091447 readyapi-0.111.0.dev1/docs_src/request_forms/tutorial001_an.py
+-rw-r--r--   0        0        0      226 2024-05-12 05:04:33.091447 readyapi-0.111.0.dev1/docs_src/request_forms/tutorial001_an_py39.py
+-rw-r--r--   0        0        0      320 2024-05-12 05:04:33.091447 readyapi-0.111.0.dev1/docs_src/request_forms_and_files/tutorial001.py
+-rw-r--r--   0        0        0      399 2024-05-12 05:04:33.091447 readyapi-0.111.0.dev1/docs_src/request_forms_and_files/tutorial001_an.py
+-rw-r--r--   0        0        0      389 2024-05-12 05:04:33.091447 readyapi-0.111.0.dev1/docs_src/request_forms_and_files/tutorial001_an_py39.py
+-rw-r--r--   0        0        0      394 2024-05-12 05:04:33.091447 readyapi-0.111.0.dev1/docs_src/response_change_status_code/tutorial001.py
+-rw-r--r--   0        0        0      348 2024-05-12 05:04:33.091447 readyapi-0.111.0.dev1/docs_src/response_cookies/tutorial001.py
+-rw-r--r--   0        0        0      275 2024-05-12 05:04:33.091447 readyapi-0.111.0.dev1/docs_src/response_cookies/tutorial002.py
+-rw-r--r--   0        0        0      510 2024-05-12 05:04:33.091447 readyapi-0.111.0.dev1/docs_src/response_directly/tutorial001.py
+-rw-r--r--   0        0        0      357 2024-05-12 05:04:33.091447 readyapi-0.111.0.dev1/docs_src/response_directly/tutorial002.py
+-rw-r--r--   0        0        0      313 2024-05-12 05:04:33.091447 readyapi-0.111.0.dev1/docs_src/response_headers/tutorial001.py
+-rw-r--r--   0        0        0      225 2024-05-12 05:04:33.091447 readyapi-0.111.0.dev1/docs_src/response_headers/tutorial002.py
+-rw-r--r--   0        0        0      565 2024-05-12 05:04:33.091447 readyapi-0.111.0.dev1/docs_src/response_model/tutorial001.py
+-rw-r--r--   0        0        0      516 2024-05-12 05:04:33.091447 readyapi-0.111.0.dev1/docs_src/response_model/tutorial001_01.py
+-rw-r--r--   0        0        0      472 2024-05-12 05:04:33.091447 readyapi-0.111.0.dev1/docs_src/response_model/tutorial001_01_py310.py
+-rw-r--r--   0        0        0      510 2024-05-12 05:04:33.091447 readyapi-0.111.0.dev1/docs_src/response_model/tutorial001_01_py39.py
+-rw-r--r--   0        0        0      540 2024-05-12 05:04:33.091447 readyapi-0.111.0.dev1/docs_src/response_model/tutorial001_py310.py
+-rw-r--r--   0        0        0      559 2024-05-12 05:04:33.091447 readyapi-0.111.0.dev1/docs_src/response_model/tutorial001_py39.py
+-rw-r--r--   0        0        0      353 2024-05-12 05:04:33.091447 readyapi-0.111.0.dev1/docs_src/response_model/tutorial002.py
+-rw-r--r--   0        0        0      321 2024-05-12 05:04:33.091447 readyapi-0.111.0.dev1/docs_src/response_model/tutorial002_py310.py
+-rw-r--r--   0        0        0      453 2024-05-12 05:04:33.091447 readyapi-0.111.0.dev1/docs_src/response_model/tutorial003.py
+-rw-r--r--   0        0        0      352 2024-05-12 05:04:33.091447 readyapi-0.111.0.dev1/docs_src/response_model/tutorial003_01.py
+-rw-r--r--   0        0        0      320 2024-05-12 05:04:33.091447 readyapi-0.111.0.dev1/docs_src/response_model/tutorial003_01_py310.py
+-rw-r--r--   0        0        0      385 2024-05-12 05:04:33.091447 readyapi-0.111.0.dev1/docs_src/response_model/tutorial003_02.py
+-rw-r--r--   0        0        0      245 2024-05-12 05:04:33.091447 readyapi-0.111.0.dev1/docs_src/response_model/tutorial003_03.py
+-rw-r--r--   0        0        0      388 2024-05-12 05:04:33.091447 readyapi-0.111.0.dev1/docs_src/response_model/tutorial003_04.py
+-rw-r--r--   0        0        0      356 2024-05-12 05:04:33.091447 readyapi-0.111.0.dev1/docs_src/response_model/tutorial003_04_py310.py
+-rw-r--r--   0        0        0      409 2024-05-12 05:04:33.091447 readyapi-0.111.0.dev1/docs_src/response_model/tutorial003_05.py
+-rw-r--r--   0        0        0      377 2024-05-12 05:04:33.091447 readyapi-0.111.0.dev1/docs_src/response_model/tutorial003_05_py310.py
+-rw-r--r--   0        0        0      434 2024-05-12 05:04:33.091447 readyapi-0.111.0.dev1/docs_src/response_model/tutorial003_py310.py
+-rw-r--r--   0        0        0      636 2024-05-12 05:04:33.091447 readyapi-0.111.0.dev1/docs_src/response_model/tutorial004.py
+-rw-r--r--   0        0        0      598 2024-05-12 05:04:33.091447 readyapi-0.111.0.dev1/docs_src/response_model/tutorial004_py310.py
+-rw-r--r--   0        0        0      630 2024-05-12 05:04:33.091447 readyapi-0.111.0.dev1/docs_src/response_model/tutorial004_py39.py
+-rw-r--r--   0        0        0      851 2024-05-12 05:04:33.091447 readyapi-0.111.0.dev1/docs_src/response_model/tutorial005.py
+-rw-r--r--   0        0        0      819 2024-05-12 05:04:33.091447 readyapi-0.111.0.dev1/docs_src/response_model/tutorial005_py310.py
+-rw-r--r--   0        0        0      851 2024-05-12 05:04:33.091447 readyapi-0.111.0.dev1/docs_src/response_model/tutorial006.py
+-rw-r--r--   0        0        0      819 2024-05-12 05:04:33.091447 readyapi-0.111.0.dev1/docs_src/response_model/tutorial006_py310.py
+-rw-r--r--   0        0        0      148 2024-05-12 05:04:33.091447 readyapi-0.111.0.dev1/docs_src/response_status_code/tutorial001.py
+-rw-r--r--   0        0        0      176 2024-05-12 05:04:33.095447 readyapi-0.111.0.dev1/docs_src/response_status_code/tutorial002.py
+-rw-r--r--   0        0        0      687 2024-05-12 05:04:33.095447 readyapi-0.111.0.dev1/docs_src/schema_extra_example/tutorial001.py
+-rw-r--r--   0        0        0      672 2024-05-12 05:04:33.095447 readyapi-0.111.0.dev1/docs_src/schema_extra_example/tutorial001_pv1.py
+-rw-r--r--   0        0        0      649 2024-05-12 05:04:33.095447 readyapi-0.111.0.dev1/docs_src/schema_extra_example/tutorial001_py310.py
+-rw-r--r--   0        0        0      634 2024-05-12 05:04:33.095447 readyapi-0.111.0.dev1/docs_src/schema_extra_example/tutorial001_py310_pv1.py
+-rw-r--r--   0        0        0      520 2024-05-12 05:04:33.095447 readyapi-0.111.0.dev1/docs_src/schema_extra_example/tutorial002.py
+-rw-r--r--   0        0        0      482 2024-05-12 05:04:33.095447 readyapi-0.111.0.dev1/docs_src/schema_extra_example/tutorial002_py310.py
+-rw-r--r--   0        0        0      615 2024-05-12 05:04:33.095447 readyapi-0.111.0.dev1/docs_src/schema_extra_example/tutorial003.py
+-rw-r--r--   0        0        0      724 2024-05-12 05:04:33.095447 readyapi-0.111.0.dev1/docs_src/schema_extra_example/tutorial003_an.py
+-rw-r--r--   0        0        0      676 2024-05-12 05:04:33.095447 readyapi-0.111.0.dev1/docs_src/schema_extra_example/tutorial003_an_py310.py
+-rw-r--r--   0        0        0      695 2024-05-12 05:04:33.095447 readyapi-0.111.0.dev1/docs_src/schema_extra_example/tutorial003_an_py39.py
+-rw-r--r--   0        0        0      577 2024-05-12 05:04:33.095447 readyapi-0.111.0.dev1/docs_src/schema_extra_example/tutorial003_py310.py
+-rw-r--r--   0        0        0      827 2024-05-12 05:04:33.095447 readyapi-0.111.0.dev1/docs_src/schema_extra_example/tutorial004.py
+-rw-r--r--   0        0        0      968 2024-05-12 05:04:33.095447 readyapi-0.111.0.dev1/docs_src/schema_extra_example/tutorial004_an.py
+-rw-r--r--   0        0        0      920 2024-05-12 05:04:33.095447 readyapi-0.111.0.dev1/docs_src/schema_extra_example/tutorial004_an_py310.py
+-rw-r--r--   0        0        0      939 2024-05-12 05:04:33.095447 readyapi-0.111.0.dev1/docs_src/schema_extra_example/tutorial004_an_py39.py
+-rw-r--r--   0        0        0      789 2024-05-12 05:04:33.095447 readyapi-0.111.0.dev1/docs_src/schema_extra_example/tutorial004_py310.py
+-rw-r--r--   0        0        0     1390 2024-05-12 05:04:33.095447 readyapi-0.111.0.dev1/docs_src/schema_extra_example/tutorial005.py
+-rw-r--r--   0        0        0     1575 2024-05-12 05:04:33.095447 readyapi-0.111.0.dev1/docs_src/schema_extra_example/tutorial005_an.py
+-rw-r--r--   0        0        0     1527 2024-05-12 05:04:33.095447 readyapi-0.111.0.dev1/docs_src/schema_extra_example/tutorial005_an_py310.py
+-rw-r--r--   0        0        0     1546 2024-05-12 05:04:33.095447 readyapi-0.111.0.dev1/docs_src/schema_extra_example/tutorial005_an_py39.py
+-rw-r--r--   0        0        0     1352 2024-05-12 05:04:33.095447 readyapi-0.111.0.dev1/docs_src/schema_extra_example/tutorial005_py310.py
+-rw-r--r--   0        0        0      273 2024-05-12 05:04:33.095447 readyapi-0.111.0.dev1/docs_src/security/tutorial001.py
+-rw-r--r--   0        0        0      323 2024-05-12 05:04:33.095447 readyapi-0.111.0.dev1/docs_src/security/tutorial001_an.py
+-rw-r--r--   0        0        0      313 2024-05-12 05:04:33.095447 readyapi-0.111.0.dev1/docs_src/security/tutorial001_an_py39.py
+-rw-r--r--   0        0        0      759 2024-05-12 05:04:33.095447 readyapi-0.111.0.dev1/docs_src/security/tutorial002.py
+-rw-r--r--   0        0        0      819 2024-05-12 05:04:33.095447 readyapi-0.111.0.dev1/docs_src/security/tutorial002_an.py
+-rw-r--r--   0        0        0      765 2024-05-12 05:04:33.095447 readyapi-0.111.0.dev1/docs_src/security/tutorial002_an_py310.py
+-rw-r--r--   0        0        0      790 2024-05-12 05:04:33.095447 readyapi-0.111.0.dev1/docs_src/security/tutorial002_an_py39.py
+-rw-r--r--   0        0        0      715 2024-05-12 05:04:33.095447 readyapi-0.111.0.dev1/docs_src/security/tutorial002_py310.py
+-rw-r--r--   0        0        0     2498 2024-05-12 05:04:33.095447 readyapi-0.111.0.dev1/docs_src/security/tutorial003.py
+-rw-r--r--   0        0        0     2592 2024-05-12 05:04:33.095447 readyapi-0.111.0.dev1/docs_src/security/tutorial003_an.py
+-rw-r--r--   0        0        0     2538 2024-05-12 05:04:33.095447 readyapi-0.111.0.dev1/docs_src/security/tutorial003_an_py310.py
+-rw-r--r--   0        0        0     2563 2024-05-12 05:04:33.095447 readyapi-0.111.0.dev1/docs_src/security/tutorial003_an_py39.py
+-rw-r--r--   0        0        0     2454 2024-05-12 05:04:33.095447 readyapi-0.111.0.dev1/docs_src/security/tutorial003_py310.py
+-rw-r--r--   0        0        0     4138 2024-05-12 05:04:33.095447 readyapi-0.111.0.dev1/docs_src/security/tutorial004.py
+-rw-r--r--   0        0        0     4249 2024-05-12 05:04:33.095447 readyapi-0.111.0.dev1/docs_src/security/tutorial004_an.py
+-rw-r--r--   0        0        0     4183 2024-05-12 05:04:33.095447 readyapi-0.111.0.dev1/docs_src/security/tutorial004_an_py310.py
+-rw-r--r--   0        0        0     4220 2024-05-12 05:04:33.095447 readyapi-0.111.0.dev1/docs_src/security/tutorial004_an_py39.py
+-rw-r--r--   0        0        0     4083 2024-05-12 05:04:33.095447 readyapi-0.111.0.dev1/docs_src/security/tutorial004_py310.py
+-rw-r--r--   0        0        0     5274 2024-05-12 05:04:33.095447 readyapi-0.111.0.dev1/docs_src/security/tutorial005.py
+-rw-r--r--   0        0        0     5381 2024-05-12 05:04:33.095447 readyapi-0.111.0.dev1/docs_src/security/tutorial005_an.py
+-rw-r--r--   0        0        0     5309 2024-05-12 05:04:33.095447 readyapi-0.111.0.dev1/docs_src/security/tutorial005_an_py310.py
+-rw-r--r--   0        0        0     5352 2024-05-12 05:04:33.095447 readyapi-0.111.0.dev1/docs_src/security/tutorial005_an_py39.py
+-rw-r--r--   0        0        0     5213 2024-05-12 05:04:33.095447 readyapi-0.111.0.dev1/docs_src/security/tutorial005_py310.py
+-rw-r--r--   0        0        0     5268 2024-05-12 05:04:33.095447 readyapi-0.111.0.dev1/docs_src/security/tutorial005_py39.py
+-rw-r--r--   0        0        0      325 2024-05-12 05:04:33.095447 readyapi-0.111.0.dev1/docs_src/security/tutorial006.py
+-rw-r--r--   0        0        0      375 2024-05-12 05:04:33.095447 readyapi-0.111.0.dev1/docs_src/security/tutorial006_an.py
+-rw-r--r--   0        0        0      365 2024-05-12 05:04:33.095447 readyapi-0.111.0.dev1/docs_src/security/tutorial006_an_py39.py
+-rw-r--r--   0        0        0     1120 2024-05-12 05:04:33.095447 readyapi-0.111.0.dev1/docs_src/security/tutorial007.py
+-rw-r--r--   0        0        0     1187 2024-05-12 05:04:33.095447 readyapi-0.111.0.dev1/docs_src/security/tutorial007_an.py
+-rw-r--r--   0        0        0     1176 2024-05-12 05:04:33.095447 readyapi-0.111.0.dev1/docs_src/security/tutorial007_an_py39.py
+-rw-r--r--   0        0        0      492 2024-05-12 05:04:33.095447 readyapi-0.111.0.dev1/docs_src/separate_openapi_schemas/tutorial001.py
+-rw-r--r--   0        0        0      454 2024-05-12 05:04:33.095447 readyapi-0.111.0.dev1/docs_src/separate_openapi_schemas/tutorial001_py310.py
+-rw-r--r--   0        0        0      486 2024-05-12 05:04:33.095447 readyapi-0.111.0.dev1/docs_src/separate_openapi_schemas/tutorial001_py39.py
+-rw-r--r--   0        0        0      527 2024-05-12 05:04:33.095447 readyapi-0.111.0.dev1/docs_src/separate_openapi_schemas/tutorial002.py
+-rw-r--r--   0        0        0      489 2024-05-12 05:04:33.095447 readyapi-0.111.0.dev1/docs_src/separate_openapi_schemas/tutorial002_py310.py
+-rw-r--r--   0        0        0      521 2024-05-12 05:04:33.095447 readyapi-0.111.0.dev1/docs_src/separate_openapi_schemas/tutorial002_py39.py
+-rw-r--r--   0        0        0        0 2024-05-12 05:04:33.095447 readyapi-0.111.0.dev1/docs_src/settings/app01/__init__.py
+-rw-r--r--   0        0        0      183 2024-05-12 05:04:33.095447 readyapi-0.111.0.dev1/docs_src/settings/app01/config.py
+-rw-r--r--   0        0        0      270 2024-05-12 05:04:33.095447 readyapi-0.111.0.dev1/docs_src/settings/app01/main.py
+-rw-r--r--   0        0        0        0 2024-05-12 05:04:33.095447 readyapi-0.111.0.dev1/docs_src/settings/app02/__init__.py
+-rw-r--r--   0        0        0      159 2024-05-12 05:04:33.095447 readyapi-0.111.0.dev1/docs_src/settings/app02/config.py
+-rw-r--r--   0        0        0      409 2024-05-12 05:04:33.095447 readyapi-0.111.0.dev1/docs_src/settings/app02/main.py
+-rw-r--r--   0        0        0      516 2024-05-12 05:04:33.095447 readyapi-0.111.0.dev1/docs_src/settings/app02/test_main.py
+-rw-r--r--   0        0        0        0 2024-05-12 05:04:33.095447 readyapi-0.111.0.dev1/docs_src/settings/app02_an/__init__.py
+-rw-r--r--   0        0        0      159 2024-05-12 05:04:33.095447 readyapi-0.111.0.dev1/docs_src/settings/app02_an/config.py
+-rw-r--r--   0        0        0      459 2024-05-12 05:04:33.095447 readyapi-0.111.0.dev1/docs_src/settings/app02_an/main.py
+-rw-r--r--   0        0        0      516 2024-05-12 05:04:33.095447 readyapi-0.111.0.dev1/docs_src/settings/app02_an/test_main.py
+-rw-r--r--   0        0        0        0 2024-05-12 05:04:33.095447 readyapi-0.111.0.dev1/docs_src/settings/app02_an_py39/__init__.py
+-rw-r--r--   0        0        0      159 2024-05-12 05:04:33.095447 readyapi-0.111.0.dev1/docs_src/settings/app02_an_py39/config.py
+-rw-r--r--   0        0        0      448 2024-05-12 05:04:33.095447 readyapi-0.111.0.dev1/docs_src/settings/app02_an_py39/main.py
+-rw-r--r--   0        0        0      516 2024-05-12 05:04:33.095447 readyapi-0.111.0.dev1/docs_src/settings/app02_an_py39/test_main.py
+-rw-r--r--   0        0        0        0 2024-05-12 05:04:33.095447 readyapi-0.111.0.dev1/docs_src/settings/app03/__init__.py
+-rw-r--r--   0        0        0      204 2024-05-12 05:04:33.095447 readyapi-0.111.0.dev1/docs_src/settings/app03/config.py
+-rw-r--r--   0        0        0      415 2024-05-12 05:04:33.095447 readyapi-0.111.0.dev1/docs_src/settings/app03/main.py
+-rw-r--r--   0        0        0        0 2024-05-12 05:04:33.095447 readyapi-0.111.0.dev1/docs_src/settings/app03_an/__init__.py
+-rw-r--r--   0        0        0      235 2024-05-12 05:04:33.095447 readyapi-0.111.0.dev1/docs_src/settings/app03_an/config.py
+-rw-r--r--   0        0        0      195 2024-05-12 05:04:33.095447 readyapi-0.111.0.dev1/docs_src/settings/app03_an/config_pv1.py
+-rw-r--r--   0        0        0      454 2024-05-12 05:04:33.095447 readyapi-0.111.0.dev1/docs_src/settings/app03_an/main.py
+-rw-r--r--   0        0        0        0 2024-05-12 05:04:33.095447 readyapi-0.111.0.dev1/docs_src/settings/app03_an_py39/__init__.py
+-rw-r--r--   0        0        0      204 2024-05-12 05:04:33.095447 readyapi-0.111.0.dev1/docs_src/settings/app03_an_py39/config.py
+-rw-r--r--   0        0        0      465 2024-05-12 05:04:33.095447 readyapi-0.111.0.dev1/docs_src/settings/app03_an_py39/main.py
+-rw-r--r--   0        0        0      422 2024-05-12 05:04:33.095447 readyapi-0.111.0.dev1/docs_src/settings/tutorial001.py
+-rw-r--r--   0        0        0      413 2024-05-12 05:04:33.095447 readyapi-0.111.0.dev1/docs_src/settings/tutorial001_pv1.py
+-rw-r--r--   0        0        0        0 2024-05-12 05:04:33.095447 readyapi-0.111.0.dev1/docs_src/sql_databases/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-12 05:04:33.095447 readyapi-0.111.0.dev1/docs_src/sql_databases/sql_app/__init__.py
+-rw-r--r--   0        0        0     1931 2024-05-12 05:04:33.095447 readyapi-0.111.0.dev1/docs_src/sql_databases/sql_app/alt_main.py
+-rw-r--r--   0        0        0     1061 2024-05-12 05:04:33.095447 readyapi-0.111.0.dev1/docs_src/sql_databases/sql_app/crud.py
+-rw-r--r--   0        0        0      461 2024-05-12 05:04:33.095447 readyapi-0.111.0.dev1/docs_src/sql_databases/sql_app/database.py
+-rw-r--r--   0        0        0     1635 2024-05-12 05:04:33.095447 readyapi-0.111.0.dev1/docs_src/sql_databases/sql_app/main.py
+-rw-r--r--   0        0        0      710 2024-05-12 05:04:33.095447 readyapi-0.111.0.dev1/docs_src/sql_databases/sql_app/models.py
+-rw-r--r--   0        0        0      502 2024-05-12 05:04:33.095447 readyapi-0.111.0.dev1/docs_src/sql_databases/sql_app/schemas.py
+-rw-r--r--   0        0        0        0 2024-05-12 05:04:33.095447 readyapi-0.111.0.dev1/docs_src/sql_databases/sql_app/tests/__init__.py
+-rw-r--r--   0        0        0     1261 2024-05-12 05:04:33.095447 readyapi-0.111.0.dev1/docs_src/sql_databases/sql_app/tests/test_sql_app.py
+-rw-r--r--   0        0        0        0 2024-05-12 05:04:33.099448 readyapi-0.111.0.dev1/docs_src/sql_databases/sql_app_py310/__init__.py
+-rw-r--r--   0        0        0     1906 2024-05-12 05:04:33.099448 readyapi-0.111.0.dev1/docs_src/sql_databases/sql_app_py310/alt_main.py
+-rw-r--r--   0        0        0     1061 2024-05-12 05:04:33.099448 readyapi-0.111.0.dev1/docs_src/sql_databases/sql_app_py310/crud.py
+-rw-r--r--   0        0        0      461 2024-05-12 05:04:33.099448 readyapi-0.111.0.dev1/docs_src/sql_databases/sql_app_py310/database.py
+-rw-r--r--   0        0        0     1610 2024-05-12 05:04:33.099448 readyapi-0.111.0.dev1/docs_src/sql_databases/sql_app_py310/main.py
+-rw-r--r--   0        0        0      710 2024-05-12 05:04:33.099448 readyapi-0.111.0.dev1/docs_src/sql_databases/sql_app_py310/models.py
+-rw-r--r--   0        0        0      464 2024-05-12 05:04:33.099448 readyapi-0.111.0.dev1/docs_src/sql_databases/sql_app_py310/schemas.py
+-rw-r--r--   0        0        0        0 2024-05-12 05:04:33.099448 readyapi-0.111.0.dev1/docs_src/sql_databases/sql_app_py310/tests/__init__.py
+-rw-r--r--   0        0        0     1201 2024-05-12 05:04:33.099448 readyapi-0.111.0.dev1/docs_src/sql_databases/sql_app_py310/tests/test_sql_app.py
+-rw-r--r--   0        0        0        0 2024-05-12 05:04:33.099448 readyapi-0.111.0.dev1/docs_src/sql_databases/sql_app_py39/__init__.py
+-rw-r--r--   0        0        0     1906 2024-05-12 05:04:33.099448 readyapi-0.111.0.dev1/docs_src/sql_databases/sql_app_py39/alt_main.py
+-rw-r--r--   0        0        0     1061 2024-05-12 05:04:33.099448 readyapi-0.111.0.dev1/docs_src/sql_databases/sql_app_py39/crud.py
+-rw-r--r--   0        0        0      461 2024-05-12 05:04:33.099448 readyapi-0.111.0.dev1/docs_src/sql_databases/sql_app_py39/database.py
+-rw-r--r--   0        0        0     1610 2024-05-12 05:04:33.099448 readyapi-0.111.0.dev1/docs_src/sql_databases/sql_app_py39/main.py
+-rw-r--r--   0        0        0      710 2024-05-12 05:04:33.099448 readyapi-0.111.0.dev1/docs_src/sql_databases/sql_app_py39/models.py
+-rw-r--r--   0        0        0      496 2024-05-12 05:04:33.099448 readyapi-0.111.0.dev1/docs_src/sql_databases/sql_app_py39/schemas.py
+-rw-r--r--   0        0        0        0 2024-05-12 05:04:33.099448 readyapi-0.111.0.dev1/docs_src/sql_databases/sql_app_py39/tests/__init__.py
+-rw-r--r--   0        0        0     1201 2024-05-12 05:04:33.099448 readyapi-0.111.0.dev1/docs_src/sql_databases/sql_app_py39/tests/test_sql_app.py
+-rw-r--r--   0        0        0        0 2024-05-12 05:04:33.099448 readyapi-0.111.0.dev1/docs_src/sql_databases_peewee/sql_app/__init__.py
+-rw-r--r--   0        0        0      843 2024-05-12 05:04:33.099448 readyapi-0.111.0.dev1/docs_src/sql_databases_peewee/sql_app/crud.py
+-rw-r--r--   0        0        0      662 2024-05-12 05:04:33.099448 readyapi-0.111.0.dev1/docs_src/sql_databases_peewee/sql_app/database.py
+-rw-r--r--   0        0        0     2213 2024-05-12 05:04:33.099448 readyapi-0.111.0.dev1/docs_src/sql_databases_peewee/sql_app/main.py
+-rw-r--r--   0        0        0      465 2024-05-12 05:04:33.099448 readyapi-0.111.0.dev1/docs_src/sql_databases_peewee/sql_app/models.py
+-rw-r--r--   0        0        0      868 2024-05-12 05:04:33.099448 readyapi-0.111.0.dev1/docs_src/sql_databases_peewee/sql_app/schemas.py
+-rw-r--r--   0        0        0      163 2024-05-12 05:04:33.099448 readyapi-0.111.0.dev1/docs_src/static_files/tutorial001.py
+-rw-r--r--   0        0        0      278 2024-05-12 05:04:33.099448 readyapi-0.111.0.dev1/docs_src/sub_applications/tutorial001.py
+-rw-r--r--   0        0        0       25 2024-05-12 05:04:33.099448 readyapi-0.111.0.dev1/docs_src/templates/static/styles.css
+-rw-r--r--   0        0        0      235 2024-05-12 05:04:33.099448 readyapi-0.111.0.dev1/docs_src/templates/templates/item.html
+-rw-r--r--   0        0        0      527 2024-05-12 05:04:33.099448 readyapi-0.111.0.dev1/docs_src/templates/tutorial001.py
+-rw-r--r--   0        0        0      233 2024-05-12 05:04:33.099448 readyapi-0.111.0.dev1/docs_src/using_request_directly/tutorial001.py
+-rw-r--r--   0        0        0        0 2024-05-12 05:04:33.099448 readyapi-0.111.0.dev1/docs_src/websockets/__init__.py
+-rw-r--r--   0        0        0     1436 2024-05-12 05:04:33.099448 readyapi-0.111.0.dev1/docs_src/websockets/tutorial001.py
+-rw-r--r--   0        0        0     2846 2024-05-12 05:04:33.099448 readyapi-0.111.0.dev1/docs_src/websockets/tutorial002.py
+-rw-r--r--   0        0        0     2913 2024-05-12 05:04:33.099448 readyapi-0.111.0.dev1/docs_src/websockets/tutorial002_an.py
+-rw-r--r--   0        0        0     2859 2024-05-12 05:04:33.099448 readyapi-0.111.0.dev1/docs_src/websockets/tutorial002_an_py310.py
+-rw-r--r--   0        0        0     2884 2024-05-12 05:04:33.099448 readyapi-0.111.0.dev1/docs_src/websockets/tutorial002_an_py39.py
+-rw-r--r--   0        0        0     2802 2024-05-12 05:04:33.099448 readyapi-0.111.0.dev1/docs_src/websockets/tutorial002_py310.py
+-rw-r--r--   0        0        0     2578 2024-05-12 05:04:33.099448 readyapi-0.111.0.dev1/docs_src/websockets/tutorial003.py
+-rw-r--r--   0        0        0     2553 2024-05-12 05:04:33.099448 readyapi-0.111.0.dev1/docs_src/websockets/tutorial003_py39.py
+-rw-r--r--   0        0        0      447 2024-05-12 05:04:33.099448 readyapi-0.111.0.dev1/docs_src/wsgi/tutorial001.py
+-rw-r--r--   0        0        0     1731 2024-05-12 05:04:33.099448 readyapi-0.111.0.dev1/pdm_build.py
+-rw-r--r--   0        0        0     7311 2024-05-12 05:04:36.639486 readyapi-0.111.0.dev1/pyproject.toml
+-rw-r--r--   0        0        0     1089 2024-05-12 05:04:33.099448 readyapi-0.111.0.dev1/readyapi/__init__.py
+-rw-r--r--   0        0        0    23139 2024-05-12 05:04:33.099448 readyapi-0.111.0.dev1/readyapi/_compat.py
+-rw-r--r--   0        0        0   177259 2024-05-12 05:04:33.099448 readyapi-0.111.0.dev1/readyapi/applications.py
+-rw-r--r--   0        0        0     1779 2024-05-12 05:04:33.099448 readyapi-0.111.0.dev1/readyapi/background.py
+-rw-r--r--   0        0        0     1403 2024-05-12 05:04:33.099448 readyapi-0.111.0.dev1/readyapi/concurrency.py
+-rw-r--r--   0        0        0     5774 2024-05-12 05:04:33.099448 readyapi-0.111.0.dev1/readyapi/datastructures.py
+-rw-r--r--   0        0        0        0 2024-05-12 05:04:33.099448 readyapi-0.111.0.dev1/readyapi/dependencies/__init__.py
+-rw-r--r--   0        0        0     2496 2024-05-12 05:04:33.099448 readyapi-0.111.0.dev1/readyapi/dependencies/models.py
+-rw-r--r--   0        0        0    30266 2024-05-12 05:04:33.099448 readyapi-0.111.0.dev1/readyapi/dependencies/utils.py
+-rw-r--r--   0        0        0    11074 2024-05-12 05:04:33.099448 readyapi-0.111.0.dev1/readyapi/encoders.py
+-rw-r--r--   0        0        0     1336 2024-05-12 05:04:33.099448 readyapi-0.111.0.dev1/readyapi/exception_handlers.py
+-rw-r--r--   0        0        0     4985 2024-05-12 05:04:33.099448 readyapi-0.111.0.dev1/readyapi/exceptions.py
+-rw-r--r--   0        0        0       55 2024-05-12 05:04:33.099448 readyapi-0.111.0.dev1/readyapi/logger.py
+-rw-r--r--   0        0        0       58 2024-05-12 05:04:33.099448 readyapi-0.111.0.dev1/readyapi/middleware/__init__.py
+-rw-r--r--   0        0        0       79 2024-05-12 05:04:33.099448 readyapi-0.111.0.dev1/readyapi/middleware/cors.py
+-rw-r--r--   0        0        0       79 2024-05-12 05:04:33.099448 readyapi-0.111.0.dev1/readyapi/middleware/gzip.py
+-rw-r--r--   0        0        0      115 2024-05-12 05:04:33.099448 readyapi-0.111.0.dev1/readyapi/middleware/httpsredirect.py
+-rw-r--r--   0        0        0      109 2024-05-12 05:04:33.099448 readyapi-0.111.0.dev1/readyapi/middleware/trustedhost.py
+-rw-r--r--   0        0        0       79 2024-05-12 05:04:33.099448 readyapi-0.111.0.dev1/readyapi/middleware/wsgi.py
+-rw-r--r--   0        0        0        0 2024-05-12 05:04:33.099448 readyapi-0.111.0.dev1/readyapi/openapi/__init__.py
+-rw-r--r--   0        0        0      153 2024-05-12 05:04:33.099448 readyapi-0.111.0.dev1/readyapi/openapi/constants.py
+-rw-r--r--   0        0        0    10379 2024-05-12 05:04:33.099448 readyapi-0.111.0.dev1/readyapi/openapi/docs.py
+-rw-r--r--   0        0        0    17765 2024-05-12 05:04:33.099448 readyapi-0.111.0.dev1/readyapi/openapi/models.py
+-rw-r--r--   0        0        0    22299 2024-05-12 05:04:33.103448 readyapi-0.111.0.dev1/readyapi/openapi/utils.py
+-rw-r--r--   0        0        0    64082 2024-05-12 05:04:33.103448 readyapi-0.111.0.dev1/readyapi/param_functions.py
+-rw-r--r--   0        0        0    28200 2024-05-12 05:04:33.103448 readyapi-0.111.0.dev1/readyapi/params.py
+-rw-r--r--   0        0        0        0 2024-05-12 05:04:33.103448 readyapi-0.111.0.dev1/readyapi/py.typed
+-rw-r--r--   0        0        0      142 2024-05-12 05:04:33.103448 readyapi-0.111.0.dev1/readyapi/requests.py
+-rw-r--r--   0        0        0     1769 2024-05-12 05:04:33.103448 readyapi-0.111.0.dev1/readyapi/responses.py
+-rw-r--r--   0        0        0   174906 2024-05-12 05:04:33.103448 readyapi-0.111.0.dev1/readyapi/routing.py
+-rw-r--r--   0        0        0      881 2024-05-12 05:04:33.103448 readyapi-0.111.0.dev1/readyapi/security/__init__.py
+-rw-r--r--   0        0        0     9382 2024-05-12 05:04:33.103448 readyapi-0.111.0.dev1/readyapi/security/api_key.py
+-rw-r--r--   0        0        0      142 2024-05-12 05:04:33.103448 readyapi-0.111.0.dev1/readyapi/security/base.py
+-rw-r--r--   0        0        0    13531 2024-05-12 05:04:33.103448 readyapi-0.111.0.dev1/readyapi/security/http.py
+-rw-r--r--   0        0        0    21618 2024-05-12 05:04:33.103448 readyapi-0.111.0.dev1/readyapi/security/oauth2.py
+-rw-r--r--   0        0        0     2724 2024-05-12 05:04:33.103448 readyapi-0.111.0.dev1/readyapi/security/open_id_connect_url.py
+-rw-r--r--   0        0        0      293 2024-05-12 05:04:33.103448 readyapi-0.111.0.dev1/readyapi/security/utils.py
+-rw-r--r--   0        0        0       69 2024-05-12 05:04:33.103448 readyapi-0.111.0.dev1/readyapi/staticfiles.py
+-rw-r--r--   0        0        0       76 2024-05-12 05:04:33.103448 readyapi-0.111.0.dev1/readyapi/templating.py
+-rw-r--r--   0        0        0       66 2024-05-12 05:04:33.103448 readyapi-0.111.0.dev1/readyapi/testclient.py
+-rw-r--r--   0        0        0      383 2024-05-12 05:04:33.103448 readyapi-0.111.0.dev1/readyapi/types.py
+-rw-r--r--   0        0        0     8044 2024-05-12 05:04:33.103448 readyapi-0.111.0.dev1/readyapi/utils.py
+-rw-r--r--   0        0        0      222 2024-05-12 05:04:33.103448 readyapi-0.111.0.dev1/readyapi/websockets.py
+-rw-r--r--   0        0        0       52 2024-05-12 05:04:33.103448 readyapi-0.111.0.dev1/requirements-docs-tests.txt
+-rw-r--r--   0        0        0      464 2024-05-12 05:04:33.103448 readyapi-0.111.0.dev1/requirements-docs.txt
+-rw-r--r--   0        0        0      496 2024-05-12 05:04:33.103448 readyapi-0.111.0.dev1/requirements-tests.txt
+-rw-r--r--   0        0        0      128 2024-05-12 05:04:33.103448 readyapi-0.111.0.dev1/requirements.txt
+-rwxr-xr-x   0        0        0    11141 2024-05-12 05:04:33.103448 readyapi-0.111.0.dev1/scripts/docs.py
+-rwxr-xr-x   0        0        0      114 2024-05-12 05:04:33.103448 readyapi-0.111.0.dev1/scripts/format.sh
+-rwxr-xr-x   0        0        0      128 2024-05-12 05:04:33.103448 readyapi-0.111.0.dev1/scripts/lint.sh
+-rw-r--r--   0        0        0     5216 2024-05-12 05:04:33.103448 readyapi-0.111.0.dev1/scripts/mkdocs_hooks.py
+-rw-r--r--   0        0        0      819 2024-05-12 05:04:33.103448 readyapi-0.111.0.dev1/scripts/playwright/separate_openapi_schemas/image01.py
+-rw-r--r--   0        0        0      873 2024-05-12 05:04:33.103448 readyapi-0.111.0.dev1/scripts/playwright/separate_openapi_schemas/image02.py
+-rw-r--r--   0        0        0      892 2024-05-12 05:04:33.103448 readyapi-0.111.0.dev1/scripts/playwright/separate_openapi_schemas/image03.py
+-rw-r--r--   0        0        0      881 2024-05-12 05:04:33.103448 readyapi-0.111.0.dev1/scripts/playwright/separate_openapi_schemas/image04.py
+-rw-r--r--   0        0        0      829 2024-05-12 05:04:33.103448 readyapi-0.111.0.dev1/scripts/playwright/separate_openapi_schemas/image05.py
+-rwxr-xr-x   0        0        0      124 2024-05-12 05:04:33.103448 readyapi-0.111.0.dev1/scripts/test-cov-html.sh
+-rwxr-xr-x   0        0        0       99 2024-05-12 05:04:33.103448 readyapi-0.111.0.dev1/scripts/test.sh
+-rw-r--r--   0        0        0        0 2024-05-12 05:04:33.103448 readyapi-0.111.0.dev1/tests/__init__.py
+-rw-r--r--   0        0        0     4455 2024-05-12 05:04:33.103448 readyapi-0.111.0.dev1/tests/main.py
+-rw-r--r--   0        0        0     3693 2024-05-12 05:04:33.103448 readyapi-0.111.0.dev1/tests/test_additional_properties.py
+-rw-r--r--   0        0        0     4307 2024-05-12 05:04:33.103448 readyapi-0.111.0.dev1/tests/test_additional_properties_bool.py
+-rw-r--r--   0        0        0     1212 2024-05-12 05:04:33.103448 readyapi-0.111.0.dev1/tests/test_additional_response_extra.py
+-rw-r--r--   0        0        0     1122 2024-05-12 05:04:33.103448 readyapi-0.111.0.dev1/tests/test_additional_responses_bad.py
+-rw-r--r--   0        0        0     5900 2024-05-12 05:04:33.103448 readyapi-0.111.0.dev1/tests/test_additional_responses_custom_model_in_callback.py
+-rw-r--r--   0        0        0     2980 2024-05-12 05:04:33.103448 readyapi-0.111.0.dev1/tests/test_additional_responses_custom_validationerror.py
+-rw-r--r--   0        0        0     2887 2024-05-12 05:04:33.103448 readyapi-0.111.0.dev1/tests/test_additional_responses_default_validationerror.py
+-rw-r--r--   0        0        0     3566 2024-05-12 05:04:33.103448 readyapi-0.111.0.dev1/tests/test_additional_responses_response_class.py
+-rw-r--r--   0        0        0     5234 2024-05-12 05:04:33.103448 readyapi-0.111.0.dev1/tests/test_additional_responses_router.py
+-rw-r--r--   0        0        0     2155 2024-05-12 05:04:33.103448 readyapi-0.111.0.dev1/tests/test_ambiguous_params.py
+-rw-r--r--   0        0        0    10500 2024-05-12 05:04:33.103448 readyapi-0.111.0.dev1/tests/test_annotated.py
+-rw-r--r--   0        0        0    53493 2024-05-12 05:04:33.103448 readyapi-0.111.0.dev1/tests/test_application.py
+-rw-r--r--   0        0        0      461 2024-05-12 05:04:33.103448 readyapi-0.111.0.dev1/tests/test_callable_endpoint.py
+-rw-r--r--   0        0        0     2832 2024-05-12 05:04:33.103448 readyapi-0.111.0.dev1/tests/test_compat.py
+-rw-r--r--   0        0        0     2269 2024-05-12 05:04:33.103448 readyapi-0.111.0.dev1/tests/test_computed_fields.py
+-rw-r--r--   0        0        0     2897 2024-05-12 05:04:33.103448 readyapi-0.111.0.dev1/tests/test_custom_middleware_exception.py
+-rw-r--r--   0        0        0     3137 2024-05-12 05:04:33.103448 readyapi-0.111.0.dev1/tests/test_custom_route_class.py
+-rw-r--r--   0        0        0     1251 2024-05-12 05:04:33.103448 readyapi-0.111.0.dev1/tests/test_custom_schema_fields.py
+-rw-r--r--   0        0        0     1095 2024-05-12 05:04:33.103448 readyapi-0.111.0.dev1/tests/test_custom_swagger_ui_redirect.py
+-rw-r--r--   0        0        0     2031 2024-05-12 05:04:33.103448 readyapi-0.111.0.dev1/tests/test_datastructures.py
+-rw-r--r--   0        0        0     1609 2024-05-12 05:04:33.103448 readyapi-0.111.0.dev1/tests/test_datetime_custom_encoder.py
+-rw-r--r--   0        0        0     5370 2024-05-12 05:04:33.103448 readyapi-0.111.0.dev1/tests/test_default_response_class.py
+-rw-r--r--   0        0        0     5122 2024-05-12 05:04:33.103448 readyapi-0.111.0.dev1/tests/test_default_response_class_router.py
+-rw-r--r--   0        0        0     2791 2024-05-12 05:04:33.103448 readyapi-0.111.0.dev1/tests/test_dependency_cache.py
+-rw-r--r--   0        0        0     3383 2024-05-12 05:04:33.103448 readyapi-0.111.0.dev1/tests/test_dependency_class.py
+-rw-r--r--   0        0        0    11874 2024-05-12 05:04:33.103448 readyapi-0.111.0.dev1/tests/test_dependency_contextmanager.py
+-rw-r--r--   0        0        0     1564 2024-05-12 05:04:33.103448 readyapi-0.111.0.dev1/tests/test_dependency_contextvars.py
+-rw-r--r--   0        0        0     8582 2024-05-12 05:04:33.103448 readyapi-0.111.0.dev1/tests/test_dependency_duplicates.py
+-rw-r--r--   0        0        0     1965 2024-05-12 05:04:33.103448 readyapi-0.111.0.dev1/tests/test_dependency_normal_exceptions.py
+-rw-r--r--   0        0        0    15820 2024-05-12 05:04:33.107447 readyapi-0.111.0.dev1/tests/test_dependency_overrides.py
+-rw-r--r--   0        0        0     1468 2024-05-12 05:04:33.107447 readyapi-0.111.0.dev1/tests/test_dependency_security_overrides.py
+-rw-r--r--   0        0        0     1198 2024-05-12 05:04:33.107447 readyapi-0.111.0.dev1/tests/test_deprecated_openapi_prefix.py
+-rw-r--r--   0        0        0     2164 2024-05-12 05:04:33.107447 readyapi-0.111.0.dev1/tests/test_duplicate_models_openapi.py
+-rw-r--r--   0        0        0      812 2024-05-12 05:04:33.107447 readyapi-0.111.0.dev1/tests/test_empty_router.py
+-rw-r--r--   0        0        0     3463 2024-05-12 05:04:33.107447 readyapi-0.111.0.dev1/tests/test_enforce_once_required_parameter.py
+-rw-r--r--   0        0        0     1923 2024-05-12 05:04:33.107447 readyapi-0.111.0.dev1/tests/test_exception_handlers.py
+-rw-r--r--   0        0        0    14039 2024-05-12 05:04:33.107447 readyapi-0.111.0.dev1/tests/test_extra_routes.py
+-rw-r--r--   0        0        0        0 2024-05-12 05:04:33.107447 readyapi-0.111.0.dev1/tests/test_filter_pydantic_sub_model/__init__.py
+-rw-r--r--   0        0        0      787 2024-05-12 05:04:33.107447 readyapi-0.111.0.dev1/tests/test_filter_pydantic_sub_model/app_pv1.py
+-rw-r--r--   0        0        0     4615 2024-05-12 05:04:33.107447 readyapi-0.111.0.dev1/tests/test_filter_pydantic_sub_model/test_filter_pydantic_sub_model_pv1.py
+-rw-r--r--   0        0        0     6467 2024-05-12 05:04:33.107447 readyapi-0.111.0.dev1/tests/test_filter_pydantic_sub_model_pv2.py
+-rw-r--r--   0        0        0     1206 2024-05-12 05:04:33.107447 readyapi-0.111.0.dev1/tests/test_forms_from_non_typing_sequences.py
+-rw-r--r--   0        0        0    68318 2024-05-12 05:04:33.107447 readyapi-0.111.0.dev1/tests/test_generate_unique_id_function.py
+-rw-r--r--   0        0        0     1886 2024-05-12 05:04:33.107447 readyapi-0.111.0.dev1/tests/test_generic_parameterless_depends.py
+-rw-r--r--   0        0        0     3749 2024-05-12 05:04:33.107447 readyapi-0.111.0.dev1/tests/test_get_request_body.py
+-rw-r--r--   0        0        0      977 2024-05-12 05:04:33.107447 readyapi-0.111.0.dev1/tests/test_http_connection_injection.py
+-rw-r--r--   0        0        0      501 2024-05-12 05:04:33.107447 readyapi-0.111.0.dev1/tests/test_include_route.py
+-rw-r--r--   0        0        0   367198 2024-05-12 05:04:33.107447 readyapi-0.111.0.dev1/tests/test_include_router_defaults_overrides.py
+-rw-r--r--   0        0        0    13624 2024-05-12 05:04:33.107447 readyapi-0.111.0.dev1/tests/test_infer_param_optionality.py
+-rw-r--r--   0        0        0     3090 2024-05-12 05:04:33.107447 readyapi-0.111.0.dev1/tests/test_inherited_custom_class.py
+-rw-r--r--   0        0        0     1713 2024-05-12 05:04:33.107447 readyapi-0.111.0.dev1/tests/test_invalid_path_param.py
+-rw-r--r--   0        0        0     1254 2024-05-12 05:04:33.107447 readyapi-0.111.0.dev1/tests/test_invalid_sequence_param.py
+-rw-r--r--   0        0        0     9184 2024-05-12 05:04:33.107447 readyapi-0.111.0.dev1/tests/test_jsonable_encoder.py
+-rw-r--r--   0        0        0     2507 2024-05-12 05:04:33.107447 readyapi-0.111.0.dev1/tests/test_local_docs.py
+-rw-r--r--   0        0        0        0 2024-05-12 05:04:33.107447 readyapi-0.111.0.dev1/tests/test_modules_same_name_body/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-12 05:04:33.107447 readyapi-0.111.0.dev1/tests/test_modules_same_name_body/app/__init__.py
+-rw-r--r--   0        0        0      161 2024-05-12 05:04:33.107447 readyapi-0.111.0.dev1/tests/test_modules_same_name_body/app/a.py
+-rw-r--r--   0        0        0      162 2024-05-12 05:04:33.107447 readyapi-0.111.0.dev1/tests/test_modules_same_name_body/app/b.py
+-rw-r--r--   0        0        0      153 2024-05-12 05:04:33.107447 readyapi-0.111.0.dev1/tests/test_modules_same_name_body/app/main.py
+-rw-r--r--   0        0        0     5784 2024-05-12 05:04:33.107447 readyapi-0.111.0.dev1/tests/test_modules_same_name_body/test_main.py
+-rw-r--r--   0        0        0     7826 2024-05-12 05:04:33.107447 readyapi-0.111.0.dev1/tests/test_multi_body_errors.py
+-rw-r--r--   0        0        0     4615 2024-05-12 05:04:33.107447 readyapi-0.111.0.dev1/tests/test_multi_query_errors.py
+-rw-r--r--   0        0        0     3790 2024-05-12 05:04:33.107447 readyapi-0.111.0.dev1/tests/test_multipart_installation.py
+-rw-r--r--   0        0        0      790 2024-05-12 05:04:33.107447 readyapi-0.111.0.dev1/tests/test_no_swagger_ui_redirect.py
+-rw-r--r--   0        0        0    17443 2024-05-12 05:04:33.107447 readyapi-0.111.0.dev1/tests/test_openapi_examples.py
+-rw-r--r--   0        0        0     4852 2024-05-12 05:04:33.107447 readyapi-0.111.0.dev1/tests/test_openapi_query_parameter_extension.py
+-rw-r--r--   0        0        0     1138 2024-05-12 05:04:33.107447 readyapi-0.111.0.dev1/tests/test_openapi_route_extensions.py
+-rw-r--r--   0        0        0    18893 2024-05-12 05:04:33.107447 readyapi-0.111.0.dev1/tests/test_openapi_separate_input_output_schemas.py
+-rw-r--r--   0        0        0     2012 2024-05-12 05:04:33.107447 readyapi-0.111.0.dev1/tests/test_openapi_servers.py
+-rw-r--r--   0        0        0      937 2024-05-12 05:04:33.107447 readyapi-0.111.0.dev1/tests/test_operations_signatures.py
+-rw-r--r--   0        0        0      567 2024-05-12 05:04:33.107447 readyapi-0.111.0.dev1/tests/test_orjson_response_class.py
+-rw-r--r--   0        0        0      641 2024-05-12 05:04:33.107447 readyapi-0.111.0.dev1/tests/test_param_class.py
+-rw-r--r--   0        0        0     3142 2024-05-12 05:04:33.107447 readyapi-0.111.0.dev1/tests/test_param_in_path_and_dependency.py
+-rw-r--r--   0        0        0     7616 2024-05-12 05:04:33.107447 readyapi-0.111.0.dev1/tests/test_param_include_in_schema.py
+-rw-r--r--   0        0        0     3415 2024-05-12 05:04:33.107447 readyapi-0.111.0.dev1/tests/test_params_repr.py
+-rw-r--r--   0        0        0    35210 2024-05-12 05:04:33.107447 readyapi-0.111.0.dev1/tests/test_path.py
+-rw-r--r--   0        0        0     3367 2024-05-12 05:04:33.107447 readyapi-0.111.0.dev1/tests/test_put_no_body.py
+-rw-r--r--   0        0        0    11639 2024-05-12 05:04:33.107447 readyapi-0.111.0.dev1/tests/test_query.py
+-rw-r--r--   0        0        0     2420 2024-05-12 05:04:33.107447 readyapi-0.111.0.dev1/tests/test_read_with_orm_mode.py
+-rw-r--r--   0        0        0     6349 2024-05-12 05:04:33.107447 readyapi-0.111.0.dev1/tests/test_regex_deprecated_body.py
+-rw-r--r--   0        0        0     5600 2024-05-12 05:04:33.107447 readyapi-0.111.0.dev1/tests/test_regex_deprecated_params.py
+-rw-r--r--   0        0        0      796 2024-05-12 05:04:33.107447 readyapi-0.111.0.dev1/tests/test_repeated_cookie_headers.py
+-rw-r--r--   0        0        0     3253 2024-05-12 05:04:33.107447 readyapi-0.111.0.dev1/tests/test_repeated_dependency_schema.py
+-rw-r--r--   0        0        0     3750 2024-05-12 05:04:33.111448 readyapi-0.111.0.dev1/tests/test_repeated_parameter_alias.py
+-rw-r--r--   0        0        0     3213 2024-05-12 05:04:33.111448 readyapi-0.111.0.dev1/tests/test_reponse_set_reponse_code_empty.py
+-rw-r--r--   0        0        0     6514 2024-05-12 05:04:33.111448 readyapi-0.111.0.dev1/tests/test_request_body_parameters_media_type.py
+-rw-r--r--   0        0        0     1534 2024-05-12 05:04:33.111448 readyapi-0.111.0.dev1/tests/test_required_noneable.py
+-rw-r--r--   0        0        0    11385 2024-05-12 05:04:33.111448 readyapi-0.111.0.dev1/tests/test_response_by_alias.py
+-rw-r--r--   0        0        0      593 2024-05-12 05:04:33.111448 readyapi-0.111.0.dev1/tests/test_response_change_status_code.py
+-rw-r--r--   0        0        0     3421 2024-05-12 05:04:33.111448 readyapi-0.111.0.dev1/tests/test_response_class_no_mediatype.py
+-rw-r--r--   0        0        0     3321 2024-05-12 05:04:33.111448 readyapi-0.111.0.dev1/tests/test_response_code_no_body.py
+-rw-r--r--   0        0        0    48847 2024-05-12 05:04:33.111448 readyapi-0.111.0.dev1/tests/test_response_model_as_return_annotation.py
+-rw-r--r--   0        0        0     1730 2024-05-12 05:04:33.111448 readyapi-0.111.0.dev1/tests/test_response_model_data_filter.py
+-rw-r--r--   0        0        0     1750 2024-05-12 05:04:33.111448 readyapi-0.111.0.dev1/tests/test_response_model_data_filter_no_inheritance.py
+-rw-r--r--   0        0        0     4122 2024-05-12 05:04:33.111448 readyapi-0.111.0.dev1/tests/test_response_model_include_exclude.py
+-rw-r--r--   0        0        0     1136 2024-05-12 05:04:33.111448 readyapi-0.111.0.dev1/tests/test_response_model_invalid.py
+-rw-r--r--   0        0        0     5384 2024-05-12 05:04:33.111448 readyapi-0.111.0.dev1/tests/test_response_model_sub_types.py
+-rw-r--r--   0        0        0     1515 2024-05-12 05:04:33.111448 readyapi-0.111.0.dev1/tests/test_route_scope.py
+-rw-r--r--   0        0        0     3301 2024-05-12 05:04:33.111448 readyapi-0.111.0.dev1/tests/test_router_events.py
+-rw-r--r--   0        0        0      488 2024-05-12 05:04:33.111448 readyapi-0.111.0.dev1/tests/test_router_prefix_with_template.py
+-rw-r--r--   0        0        0      979 2024-05-12 05:04:33.111448 readyapi-0.111.0.dev1/tests/test_router_redirect_slashes.py
+-rw-r--r--   0        0        0    38582 2024-05-12 05:04:33.111448 readyapi-0.111.0.dev1/tests/test_schema_extra_examples.py
+-rw-r--r--   0        0        0     1950 2024-05-12 05:04:33.111448 readyapi-0.111.0.dev1/tests/test_security_api_key_cookie.py
+-rw-r--r--   0        0        0     2118 2024-05-12 05:04:33.111448 readyapi-0.111.0.dev1/tests/test_security_api_key_cookie_description.py
+-rw-r--r--   0        0        0     2152 2024-05-12 05:04:33.111448 readyapi-0.111.0.dev1/tests/test_security_api_key_cookie_optional.py
+-rw-r--r--   0        0        0     1890 2024-05-12 05:04:33.111448 readyapi-0.111.0.dev1/tests/test_security_api_key_header.py
+-rw-r--r--   0        0        0     2058 2024-05-12 05:04:33.111448 readyapi-0.111.0.dev1/tests/test_security_api_key_header_description.py
+-rw-r--r--   0        0        0     2088 2024-05-12 05:04:33.111448 readyapi-0.111.0.dev1/tests/test_security_api_key_header_optional.py
+-rw-r--r--   0        0        0     1869 2024-05-12 05:04:33.111448 readyapi-0.111.0.dev1/tests/test_security_api_key_query.py
+-rw-r--r--   0        0        0     2029 2024-05-12 05:04:33.111448 readyapi-0.111.0.dev1/tests/test_security_api_key_query_description.py
+-rw-r--r--   0        0        0     2067 2024-05-12 05:04:33.111448 readyapi-0.111.0.dev1/tests/test_security_api_key_query_optional.py
+-rw-r--r--   0        0        0     1793 2024-05-12 05:04:33.111448 readyapi-0.111.0.dev1/tests/test_security_http_base.py
+-rw-r--r--   0        0        0     1979 2024-05-12 05:04:33.111448 readyapi-0.111.0.dev1/tests/test_security_http_base_description.py
+-rw-r--r--   0        0        0     1938 2024-05-12 05:04:33.111448 readyapi-0.111.0.dev1/tests/test_security_http_base_optional.py
+-rw-r--r--   0        0        0     2677 2024-05-12 05:04:33.111448 readyapi-0.111.0.dev1/tests/test_security_http_basic_optional.py
+-rw-r--r--   0        0        0     2660 2024-05-12 05:04:33.111448 readyapi-0.111.0.dev1/tests/test_security_http_basic_realm.py
+-rw-r--r--   0        0        0     2836 2024-05-12 05:04:33.111448 readyapi-0.111.0.dev1/tests/test_security_http_basic_realm_description.py
+-rw-r--r--   0        0        0     2071 2024-05-12 05:04:33.111448 readyapi-0.111.0.dev1/tests/test_security_http_bearer.py
+-rw-r--r--   0        0        0     2261 2024-05-12 05:04:33.111448 readyapi-0.111.0.dev1/tests/test_security_http_bearer_description.py
+-rw-r--r--   0        0        0     2200 2024-05-12 05:04:33.111448 readyapi-0.111.0.dev1/tests/test_security_http_bearer_optional.py
+-rw-r--r--   0        0        0     2096 2024-05-12 05:04:33.111448 readyapi-0.111.0.dev1/tests/test_security_http_digest.py
+-rw-r--r--   0        0        0     2272 2024-05-12 05:04:33.111448 readyapi-0.111.0.dev1/tests/test_security_http_digest_description.py
+-rw-r--r--   0        0        0     2239 2024-05-12 05:04:33.111448 readyapi-0.111.0.dev1/tests/test_security_http_digest_optional.py
+-rw-r--r--   0        0        0    11008 2024-05-12 05:04:33.111448 readyapi-0.111.0.dev1/tests/test_security_oauth2.py
+-rw-r--r--   0        0        0     2344 2024-05-12 05:04:33.111448 readyapi-0.111.0.dev1/tests/test_security_oauth2_authorization_code_bearer.py
+-rw-r--r--   0        0        0     2448 2024-05-12 05:04:33.111448 readyapi-0.111.0.dev1/tests/test_security_oauth2_authorization_code_bearer_description.py
+-rw-r--r--   0        0        0    11049 2024-05-12 05:04:33.111448 readyapi-0.111.0.dev1/tests/test_security_oauth2_optional.py
+-rw-r--r--   0        0        0    11189 2024-05-12 05:04:33.111448 readyapi-0.111.0.dev1/tests/test_security_oauth2_optional_description.py
+-rw-r--r--   0        0        0     2153 2024-05-12 05:04:33.111448 readyapi-0.111.0.dev1/tests/test_security_oauth2_password_bearer_optional.py
+-rw-r--r--   0        0        0     2295 2024-05-12 05:04:33.111448 readyapi-0.111.0.dev1/tests/test_security_oauth2_password_bearer_optional_description.py
+-rw-r--r--   0        0        0     2296 2024-05-12 05:04:33.111448 readyapi-0.111.0.dev1/tests/test_security_openid_connect.py
+-rw-r--r--   0        0        0     2415 2024-05-12 05:04:33.111448 readyapi-0.111.0.dev1/tests/test_security_openid_connect_description.py
+-rw-r--r--   0        0        0     2494 2024-05-12 05:04:33.111448 readyapi-0.111.0.dev1/tests/test_security_openid_connect_optional.py
+-rw-r--r--   0        0        0     1418 2024-05-12 05:04:33.111448 readyapi-0.111.0.dev1/tests/test_serialize_response.py
+-rw-r--r--   0        0        0     5002 2024-05-12 05:04:33.111448 readyapi-0.111.0.dev1/tests/test_serialize_response_dataclass.py
+-rw-r--r--   0        0        0     4279 2024-05-12 05:04:33.111448 readyapi-0.111.0.dev1/tests/test_serialize_response_model.py
+-rw-r--r--   0        0        0     2075 2024-05-12 05:04:33.111448 readyapi-0.111.0.dev1/tests/test_skip_defaults.py
+-rw-r--r--   0        0        0     7555 2024-05-12 05:04:33.111448 readyapi-0.111.0.dev1/tests/test_starlette_exception.py
+-rw-r--r--   0        0        0     1714 2024-05-12 05:04:33.111448 readyapi-0.111.0.dev1/tests/test_starlette_urlconvertors.py
+-rw-r--r--   0        0        0    14147 2024-05-12 05:04:33.111448 readyapi-0.111.0.dev1/tests/test_sub_callbacks.py
+-rw-r--r--   0        0        0      722 2024-05-12 05:04:33.111448 readyapi-0.111.0.dev1/tests/test_swagger_ui_init_oauth.py
+-rw-r--r--   0        0        0    12073 2024-05-12 05:04:33.111448 readyapi-0.111.0.dev1/tests/test_tuples.py
+-rw-r--r--   0        0        0        0 2024-05-12 05:04:33.111448 readyapi-0.111.0.dev1/tests/test_tutorial/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-12 05:04:33.111448 readyapi-0.111.0.dev1/tests/test_tutorial/test_additional_responses/__init__.py
+-rw-r--r--   0        0        0     4434 2024-05-12 05:04:33.111448 readyapi-0.111.0.dev1/tests/test_tutorial/test_additional_responses/test_tutorial001.py
+-rw-r--r--   0        0        0     4742 2024-05-12 05:04:33.111448 readyapi-0.111.0.dev1/tests/test_tutorial/test_additional_responses/test_tutorial002.py
+-rw-r--r--   0        0        0     4658 2024-05-12 05:04:33.111448 readyapi-0.111.0.dev1/tests/test_tutorial/test_additional_responses/test_tutorial003.py
+-rw-r--r--   0        0        0     4937 2024-05-12 05:04:33.111448 readyapi-0.111.0.dev1/tests/test_tutorial/test_additional_responses/test_tutorial004.py
+-rw-r--r--   0        0        0        0 2024-05-12 05:04:33.111448 readyapi-0.111.0.dev1/tests/test_tutorial/test_additional_status_codes/__init__.py
+-rw-r--r--   0        0        0      547 2024-05-12 05:04:33.111448 readyapi-0.111.0.dev1/tests/test_tutorial/test_additional_status_codes/test_tutorial001.py
+-rw-r--r--   0        0        0      550 2024-05-12 05:04:33.111448 readyapi-0.111.0.dev1/tests/test_tutorial/test_additional_status_codes/test_tutorial001_an.py
+-rw-r--r--   0        0        0      742 2024-05-12 05:04:33.111448 readyapi-0.111.0.dev1/tests/test_tutorial/test_additional_status_codes/test_tutorial001_an_py310.py
+-rw-r--r--   0        0        0      738 2024-05-12 05:04:33.111448 readyapi-0.111.0.dev1/tests/test_tutorial/test_additional_status_codes/test_tutorial001_an_py39.py
+-rw-r--r--   0        0        0      739 2024-05-12 05:04:33.111448 readyapi-0.111.0.dev1/tests/test_tutorial/test_additional_status_codes/test_tutorial001_py310.py
+-rw-r--r--   0        0        0        0 2024-05-12 05:04:33.115448 readyapi-0.111.0.dev1/tests/test_tutorial/test_advanced_middleware/__init__.py
+-rw-r--r--   0        0        0      475 2024-05-12 05:04:33.115448 readyapi-0.111.0.dev1/tests/test_tutorial/test_advanced_middleware/test_tutorial001.py
+-rw-r--r--   0        0        0      571 2024-05-12 05:04:33.115448 readyapi-0.111.0.dev1/tests/test_tutorial/test_advanced_middleware/test_tutorial002.py
+-rw-r--r--   0        0        0      667 2024-05-12 05:04:33.115448 readyapi-0.111.0.dev1/tests/test_tutorial/test_advanced_middleware/test_tutorial003.py
+-rw-r--r--   0        0        0        0 2024-05-12 05:04:33.115448 readyapi-0.111.0.dev1/tests/test_tutorial/test_async_sql_databases/__init__.py
+-rw-r--r--   0        0        0     6128 2024-05-12 05:04:33.115448 readyapi-0.111.0.dev1/tests/test_tutorial/test_async_sql_databases/test_tutorial001.py
+-rw-r--r--   0        0        0        0 2024-05-12 05:04:33.115448 readyapi-0.111.0.dev1/tests/test_tutorial/test_async_tests/__init__.py
+-rw-r--r--   0        0        0      143 2024-05-12 05:04:33.115448 readyapi-0.111.0.dev1/tests/test_tutorial/test_async_tests/test_main.py
+-rw-r--r--   0        0        0        0 2024-05-12 05:04:33.115448 readyapi-0.111.0.dev1/tests/test_tutorial/test_background_tasks/__init__.py
+-rw-r--r--   0        0        0      579 2024-05-12 05:04:33.115448 readyapi-0.111.0.dev1/tests/test_tutorial/test_background_tasks/test_tutorial001.py
+-rw-r--r--   0        0        0      569 2024-05-12 05:04:33.115448 readyapi-0.111.0.dev1/tests/test_tutorial/test_background_tasks/test_tutorial002.py
+-rw-r--r--   0        0        0      572 2024-05-12 05:04:33.115448 readyapi-0.111.0.dev1/tests/test_tutorial/test_background_tasks/test_tutorial002_an.py
+-rw-r--r--   0        0        0      632 2024-05-12 05:04:33.115448 readyapi-0.111.0.dev1/tests/test_tutorial/test_background_tasks/test_tutorial002_an_py310.py
+-rw-r--r--   0        0        0      629 2024-05-12 05:04:33.115448 readyapi-0.111.0.dev1/tests/test_tutorial/test_background_tasks/test_tutorial002_an_py39.py
+-rw-r--r--   0        0        0      629 2024-05-12 05:04:33.115448 readyapi-0.111.0.dev1/tests/test_tutorial/test_background_tasks/test_tutorial002_py310.py
+-rw-r--r--   0        0        0        0 2024-05-12 05:04:33.115448 readyapi-0.111.0.dev1/tests/test_tutorial/test_behind_a_proxy/__init__.py
+-rw-r--r--   0        0        0     1055 2024-05-12 05:04:33.115448 readyapi-0.111.0.dev1/tests/test_tutorial/test_behind_a_proxy/test_tutorial001.py
+-rw-r--r--   0        0        0     1034 2024-05-12 05:04:33.115448 readyapi-0.111.0.dev1/tests/test_tutorial/test_behind_a_proxy/test_tutorial002.py
+-rw-r--r--   0        0        0     1690 2024-05-12 05:04:33.115448 readyapi-0.111.0.dev1/tests/test_tutorial/test_behind_a_proxy/test_tutorial003.py
+-rw-r--r--   0        0        0     1658 2024-05-12 05:04:33.115448 readyapi-0.111.0.dev1/tests/test_tutorial/test_behind_a_proxy/test_tutorial004.py
+-rw-r--r--   0        0        0        0 2024-05-12 05:04:33.115448 readyapi-0.111.0.dev1/tests/test_tutorial/test_bigger_applications/__init__.py
+-rw-r--r--   0        0        0    25142 2024-05-12 05:04:33.115448 readyapi-0.111.0.dev1/tests/test_tutorial/test_bigger_applications/test_main.py
+-rw-r--r--   0        0        0    25145 2024-05-12 05:04:33.115448 readyapi-0.111.0.dev1/tests/test_tutorial/test_bigger_applications/test_main_an.py
+-rw-r--r--   0        0        0    25483 2024-05-12 05:04:33.115448 readyapi-0.111.0.dev1/tests/test_tutorial/test_bigger_applications/test_main_an_py39.py
+-rw-r--r--   0        0        0        0 2024-05-12 05:04:33.115448 readyapi-0.111.0.dev1/tests/test_tutorial/test_body/__init__.py
+-rw-r--r--   0        0        0    15094 2024-05-12 05:04:33.115448 readyapi-0.111.0.dev1/tests/test_tutorial/test_body/test_tutorial001.py
+-rw-r--r--   0        0        0    15342 2024-05-12 05:04:33.115448 readyapi-0.111.0.dev1/tests/test_tutorial/test_body/test_tutorial001_py310.py
+-rw-r--r--   0        0        0        0 2024-05-12 05:04:33.115448 readyapi-0.111.0.dev1/tests/test_tutorial/test_body_fields/__init__.py
+-rw-r--r--   0        0        0     7343 2024-05-12 05:04:33.115448 readyapi-0.111.0.dev1/tests/test_tutorial/test_body_fields/test_tutorial001.py
+-rw-r--r--   0        0        0     7346 2024-05-12 05:04:33.115448 readyapi-0.111.0.dev1/tests/test_tutorial/test_body_fields/test_tutorial001_an.py
+-rw-r--r--   0        0        0     7438 2024-05-12 05:04:33.115448 readyapi-0.111.0.dev1/tests/test_tutorial/test_body_fields/test_tutorial001_an_py310.py
+-rw-r--r--   0        0        0     7432 2024-05-12 05:04:33.115448 readyapi-0.111.0.dev1/tests/test_tutorial/test_body_fields/test_tutorial001_an_py39.py
+-rw-r--r--   0        0        0     7435 2024-05-12 05:04:33.115448 readyapi-0.111.0.dev1/tests/test_tutorial/test_body_fields/test_tutorial001_py310.py
+-rw-r--r--   0        0        0        0 2024-05-12 05:04:33.115448 readyapi-0.111.0.dev1/tests/test_tutorial/test_body_multiple_params/__init__.py
+-rw-r--r--   0        0        0     7700 2024-05-12 05:04:33.115448 readyapi-0.111.0.dev1/tests/test_tutorial/test_body_multiple_params/test_tutorial001.py
+-rw-r--r--   0        0        0     7703 2024-05-12 05:04:33.115448 readyapi-0.111.0.dev1/tests/test_tutorial/test_body_multiple_params/test_tutorial001_an.py
+-rw-r--r--   0        0        0     7808 2024-05-12 05:04:33.115448 readyapi-0.111.0.dev1/tests/test_tutorial/test_body_multiple_params/test_tutorial001_an_py310.py
+-rw-r--r--   0        0        0     7801 2024-05-12 05:04:33.115448 readyapi-0.111.0.dev1/tests/test_tutorial/test_body_multiple_params/test_tutorial001_an_py39.py
+-rw-r--r--   0        0        0     7805 2024-05-12 05:04:33.115448 readyapi-0.111.0.dev1/tests/test_tutorial/test_body_multiple_params/test_tutorial001_py310.py
+-rw-r--r--   0        0        0     9662 2024-05-12 05:04:33.115448 readyapi-0.111.0.dev1/tests/test_tutorial/test_body_multiple_params/test_tutorial003.py
+-rw-r--r--   0        0        0     9665 2024-05-12 05:04:33.115448 readyapi-0.111.0.dev1/tests/test_tutorial/test_body_multiple_params/test_tutorial003_an.py
+-rw-r--r--   0        0        0     9757 2024-05-12 05:04:33.115448 readyapi-0.111.0.dev1/tests/test_tutorial/test_body_multiple_params/test_tutorial003_an_py310.py
+-rw-r--r--   0        0        0     9751 2024-05-12 05:04:33.115448 readyapi-0.111.0.dev1/tests/test_tutorial/test_body_multiple_params/test_tutorial003_an_py39.py
+-rw-r--r--   0        0        0     9754 2024-05-12 05:04:33.115448 readyapi-0.111.0.dev1/tests/test_tutorial/test_body_multiple_params/test_tutorial003_py310.py
+-rw-r--r--   0        0        0        0 2024-05-12 05:04:33.115448 readyapi-0.111.0.dev1/tests/test_tutorial/test_body_nested_models/__init__.py
+-rw-r--r--   0        0        0     4345 2024-05-12 05:04:33.115448 readyapi-0.111.0.dev1/tests/test_tutorial/test_body_nested_models/test_tutorial009.py
+-rw-r--r--   0        0        0     4419 2024-05-12 05:04:33.115448 readyapi-0.111.0.dev1/tests/test_tutorial/test_body_nested_models/test_tutorial009_py39.py
+-rw-r--r--   0        0        0        0 2024-05-12 05:04:33.115448 readyapi-0.111.0.dev1/tests/test_tutorial/test_body_updates/__init__.py
+-rw-r--r--   0        0        0    12043 2024-05-12 05:04:33.115448 readyapi-0.111.0.dev1/tests/test_tutorial/test_body_updates/test_tutorial001.py
+-rw-r--r--   0        0        0    12114 2024-05-12 05:04:33.115448 readyapi-0.111.0.dev1/tests/test_tutorial/test_body_updates/test_tutorial001_py310.py
+-rw-r--r--   0        0        0    12108 2024-05-12 05:04:33.115448 readyapi-0.111.0.dev1/tests/test_tutorial/test_body_updates/test_tutorial001_py39.py
+-rw-r--r--   0        0        0        0 2024-05-12 05:04:33.115448 readyapi-0.111.0.dev1/tests/test_tutorial/test_conditional_openapi/__init__.py
+-rw-r--r--   0        0        0     1801 2024-05-12 05:04:33.115448 readyapi-0.111.0.dev1/tests/test_tutorial/test_conditional_openapi/test_tutorial001.py
+-rw-r--r--   0        0        0        0 2024-05-12 05:04:33.115448 readyapi-0.111.0.dev1/tests/test_tutorial/test_configure_swagger_ui/__init__.py
+-rw-r--r--   0        0        0     1416 2024-05-12 05:04:33.115448 readyapi-0.111.0.dev1/tests/test_tutorial/test_configure_swagger_ui/test_tutorial001.py
+-rw-r--r--   0        0        0     1563 2024-05-12 05:04:33.115448 readyapi-0.111.0.dev1/tests/test_tutorial/test_configure_swagger_ui/test_tutorial002.py
+-rw-r--r--   0        0        0     1535 2024-05-12 05:04:33.115448 readyapi-0.111.0.dev1/tests/test_tutorial/test_configure_swagger_ui/test_tutorial003.py
+-rw-r--r--   0        0        0        0 2024-05-12 05:04:33.115448 readyapi-0.111.0.dev1/tests/test_tutorial/test_cookie_params/__init__.py
+-rw-r--r--   0        0        0     4019 2024-05-12 05:04:33.115448 readyapi-0.111.0.dev1/tests/test_tutorial/test_cookie_params/test_tutorial001.py
+-rw-r--r--   0        0        0     4022 2024-05-12 05:04:33.115448 readyapi-0.111.0.dev1/tests/test_tutorial/test_cookie_params/test_tutorial001_an.py
+-rw-r--r--   0        0        0     4157 2024-05-12 05:04:33.115448 readyapi-0.111.0.dev1/tests/test_tutorial/test_cookie_params/test_tutorial001_an_py310.py
+-rw-r--r--   0        0        0     4152 2024-05-12 05:04:33.115448 readyapi-0.111.0.dev1/tests/test_tutorial/test_cookie_params/test_tutorial001_an_py39.py
+-rw-r--r--   0        0        0     4151 2024-05-12 05:04:33.115448 readyapi-0.111.0.dev1/tests/test_tutorial/test_cookie_params/test_tutorial001_py310.py
+-rw-r--r--   0        0        0        0 2024-05-12 05:04:33.115448 readyapi-0.111.0.dev1/tests/test_tutorial/test_cors/__init__.py
+-rw-r--r--   0        0        0     1287 2024-05-12 05:04:33.115448 readyapi-0.111.0.dev1/tests/test_tutorial/test_cors/test_tutorial001.py
+-rw-r--r--   0        0        0        0 2024-05-12 05:04:33.115448 readyapi-0.111.0.dev1/tests/test_tutorial/test_custom_docs_ui/__init__.py
+-rw-r--r--   0        0        0     1359 2024-05-12 05:04:33.115448 readyapi-0.111.0.dev1/tests/test_tutorial/test_custom_docs_ui/test_tutorial001.py
+-rw-r--r--   0        0        0     1250 2024-05-12 05:04:33.115448 readyapi-0.111.0.dev1/tests/test_tutorial/test_custom_docs_ui/test_tutorial002.py
+-rw-r--r--   0        0        0        0 2024-05-12 05:04:33.115448 readyapi-0.111.0.dev1/tests/test_tutorial/test_custom_request_and_route/__init__.py
+-rw-r--r--   0        0        0      888 2024-05-12 05:04:33.115448 readyapi-0.111.0.dev1/tests/test_tutorial/test_custom_request_and_route/test_tutorial001.py
+-rw-r--r--   0        0        0     1246 2024-05-12 05:04:33.115448 readyapi-0.111.0.dev1/tests/test_tutorial/test_custom_request_and_route/test_tutorial002.py
+-rw-r--r--   0        0        0      527 2024-05-12 05:04:33.115448 readyapi-0.111.0.dev1/tests/test_tutorial/test_custom_request_and_route/test_tutorial003.py
+-rw-r--r--   0        0        0        0 2024-05-12 05:04:33.115448 readyapi-0.111.0.dev1/tests/test_tutorial/test_custom_response/__init__.py
+-rw-r--r--   0        0        0     1027 2024-05-12 05:04:33.115448 readyapi-0.111.0.dev1/tests/test_tutorial/test_custom_response/test_tutorial001.py
+-rw-r--r--   0        0        0     1028 2024-05-12 05:04:33.119448 readyapi-0.111.0.dev1/tests/test_tutorial/test_custom_response/test_tutorial001b.py
+-rw-r--r--   0        0        0     1223 2024-05-12 05:04:33.119448 readyapi-0.111.0.dev1/tests/test_tutorial/test_custom_response/test_tutorial004.py
+-rw-r--r--   0        0        0      982 2024-05-12 05:04:33.119448 readyapi-0.111.0.dev1/tests/test_tutorial/test_custom_response/test_tutorial005.py
+-rw-r--r--   0        0        0     1061 2024-05-12 05:04:33.119448 readyapi-0.111.0.dev1/tests/test_tutorial/test_custom_response/test_tutorial006.py
+-rw-r--r--   0        0        0      909 2024-05-12 05:04:33.119448 readyapi-0.111.0.dev1/tests/test_tutorial/test_custom_response/test_tutorial006b.py
+-rw-r--r--   0        0        0      901 2024-05-12 05:04:33.119448 readyapi-0.111.0.dev1/tests/test_tutorial/test_custom_response/test_tutorial006c.py
+-rw-r--r--   0        0        0      265 2024-05-12 05:04:33.119448 readyapi-0.111.0.dev1/tests/test_tutorial/test_custom_response/test_tutorial007.py
+-rw-r--r--   0        0        0      488 2024-05-12 05:04:33.119448 readyapi-0.111.0.dev1/tests/test_tutorial/test_custom_response/test_tutorial008.py
+-rw-r--r--   0        0        0      488 2024-05-12 05:04:33.119448 readyapi-0.111.0.dev1/tests/test_tutorial/test_custom_response/test_tutorial009.py
+-rw-r--r--   0        0        0      491 2024-05-12 05:04:33.119448 readyapi-0.111.0.dev1/tests/test_tutorial/test_custom_response/test_tutorial009b.py
+-rw-r--r--   0        0        0      240 2024-05-12 05:04:33.119448 readyapi-0.111.0.dev1/tests/test_tutorial/test_custom_response/test_tutorial009c.py
+-rw-r--r--   0        0        0        0 2024-05-12 05:04:33.119448 readyapi-0.111.0.dev1/tests/test_tutorial/test_dataclasses/__init__.py
+-rw-r--r--   0        0        0     5291 2024-05-12 05:04:33.119448 readyapi-0.111.0.dev1/tests/test_tutorial/test_dataclasses/test_tutorial001.py
+-rw-r--r--   0        0        0     3576 2024-05-12 05:04:33.119448 readyapi-0.111.0.dev1/tests/test_tutorial/test_dataclasses/test_tutorial002.py
+-rw-r--r--   0        0        0    12359 2024-05-12 05:04:33.119448 readyapi-0.111.0.dev1/tests/test_tutorial/test_dataclasses/test_tutorial003.py
+-rw-r--r--   0        0        0        0 2024-05-12 05:04:33.119448 readyapi-0.111.0.dev1/tests/test_tutorial/test_dependencies/__init__.py
+-rw-r--r--   0        0        0     7221 2024-05-12 05:04:33.119448 readyapi-0.111.0.dev1/tests/test_tutorial/test_dependencies/test_tutorial001.py
+-rw-r--r--   0        0        0     7224 2024-05-12 05:04:33.119448 readyapi-0.111.0.dev1/tests/test_tutorial/test_dependencies/test_tutorial001_an.py
+-rw-r--r--   0        0        0     7404 2024-05-12 05:04:33.119448 readyapi-0.111.0.dev1/tests/test_tutorial/test_dependencies/test_tutorial001_an_py310.py
+-rw-r--r--   0        0        0     7400 2024-05-12 05:04:33.119448 readyapi-0.111.0.dev1/tests/test_tutorial/test_dependencies/test_tutorial001_an_py39.py
+-rw-r--r--   0        0        0     7401 2024-05-12 05:04:33.119448 readyapi-0.111.0.dev1/tests/test_tutorial/test_dependencies/test_tutorial001_py310.py
+-rw-r--r--   0        0        0     5553 2024-05-12 05:04:33.119448 readyapi-0.111.0.dev1/tests/test_tutorial/test_dependencies/test_tutorial004.py
+-rw-r--r--   0        0        0     5556 2024-05-12 05:04:33.119448 readyapi-0.111.0.dev1/tests/test_tutorial/test_dependencies/test_tutorial004_an.py
+-rw-r--r--   0        0        0     5736 2024-05-12 05:04:33.119448 readyapi-0.111.0.dev1/tests/test_tutorial/test_dependencies/test_tutorial004_an_py310.py
+-rw-r--r--   0        0        0     5732 2024-05-12 05:04:33.119448 readyapi-0.111.0.dev1/tests/test_tutorial/test_dependencies/test_tutorial004_an_py39.py
+-rw-r--r--   0        0        0     5733 2024-05-12 05:04:33.119448 readyapi-0.111.0.dev1/tests/test_tutorial/test_dependencies/test_tutorial004_py310.py
+-rw-r--r--   0        0        0     5121 2024-05-12 05:04:33.119448 readyapi-0.111.0.dev1/tests/test_tutorial/test_dependencies/test_tutorial006.py
+-rw-r--r--   0        0        0     5124 2024-05-12 05:04:33.119448 readyapi-0.111.0.dev1/tests/test_tutorial/test_dependencies/test_tutorial006_an.py
+-rw-r--r--   0        0        0     5402 2024-05-12 05:04:33.119448 readyapi-0.111.0.dev1/tests/test_tutorial/test_dependencies/test_tutorial006_an_py39.py
+-rw-r--r--   0        0        0      698 2024-05-12 05:04:33.119448 readyapi-0.111.0.dev1/tests/test_tutorial/test_dependencies/test_tutorial008b.py
+-rw-r--r--   0        0        0      701 2024-05-12 05:04:33.119448 readyapi-0.111.0.dev1/tests/test_tutorial/test_dependencies/test_tutorial008b_an.py
+-rw-r--r--   0        0        0      919 2024-05-12 05:04:33.119448 readyapi-0.111.0.dev1/tests/test_tutorial/test_dependencies/test_tutorial008b_an_py39.py
+-rw-r--r--   0        0        0     1171 2024-05-12 05:04:33.119448 readyapi-0.111.0.dev1/tests/test_tutorial/test_dependencies/test_tutorial008c.py
+-rw-r--r--   0        0        0     1177 2024-05-12 05:04:33.119448 readyapi-0.111.0.dev1/tests/test_tutorial/test_dependencies/test_tutorial008c_an.py
+-rw-r--r--   0        0        0     1268 2024-05-12 05:04:33.119448 readyapi-0.111.0.dev1/tests/test_tutorial/test_dependencies/test_tutorial008c_an_py39.py
+-rw-r--r--   0        0        0     1227 2024-05-12 05:04:33.119448 readyapi-0.111.0.dev1/tests/test_tutorial/test_dependencies/test_tutorial008d.py
+-rw-r--r--   0        0        0     1236 2024-05-12 05:04:33.119448 readyapi-0.111.0.dev1/tests/test_tutorial/test_dependencies/test_tutorial008d_an.py
+-rw-r--r--   0        0        0     1332 2024-05-12 05:04:33.119448 readyapi-0.111.0.dev1/tests/test_tutorial/test_dependencies/test_tutorial008d_an_py39.py
+-rw-r--r--   0        0        0     8640 2024-05-12 05:04:33.119448 readyapi-0.111.0.dev1/tests/test_tutorial/test_dependencies/test_tutorial012.py
+-rw-r--r--   0        0        0     8643 2024-05-12 05:04:33.119448 readyapi-0.111.0.dev1/tests/test_tutorial/test_dependencies/test_tutorial012_an.py
+-rw-r--r--   0        0        0     9041 2024-05-12 05:04:33.119448 readyapi-0.111.0.dev1/tests/test_tutorial/test_dependencies/test_tutorial012_an_py39.py
+-rw-r--r--   0        0        0        0 2024-05-12 05:04:33.119448 readyapi-0.111.0.dev1/tests/test_tutorial/test_events/__init__.py
+-rw-r--r--   0        0        0     3644 2024-05-12 05:04:33.119448 readyapi-0.111.0.dev1/tests/test_tutorial/test_events/test_tutorial001.py
+-rw-r--r--   0        0        0     1420 2024-05-12 05:04:33.119448 readyapi-0.111.0.dev1/tests/test_tutorial/test_events/test_tutorial002.py
+-rw-r--r--   0        0        0     3686 2024-05-12 05:04:33.119448 readyapi-0.111.0.dev1/tests/test_tutorial/test_events/test_tutorial003.py
+-rw-r--r--   0        0        0        0 2024-05-12 05:04:33.119448 readyapi-0.111.0.dev1/tests/test_tutorial/test_extending_openapi/__init__.py
+-rw-r--r--   0        0        0     1549 2024-05-12 05:04:33.119448 readyapi-0.111.0.dev1/tests/test_tutorial/test_extending_openapi/test_tutorial001.py
+-rw-r--r--   0        0        0        0 2024-05-12 05:04:33.119448 readyapi-0.111.0.dev1/tests/test_tutorial/test_extra_data_types/__init__.py
+-rw-r--r--   0        0        0     8029 2024-05-12 05:04:33.119448 readyapi-0.111.0.dev1/tests/test_tutorial/test_extra_data_types/test_tutorial001.py
+-rw-r--r--   0        0        0     8032 2024-05-12 05:04:33.119448 readyapi-0.111.0.dev1/tests/test_tutorial/test_extra_data_types/test_tutorial001_an.py
+-rw-r--r--   0        0        0     8224 2024-05-12 05:04:33.119448 readyapi-0.111.0.dev1/tests/test_tutorial/test_extra_data_types/test_tutorial001_an_py310.py
+-rw-r--r--   0        0        0     8220 2024-05-12 05:04:33.119448 readyapi-0.111.0.dev1/tests/test_tutorial/test_extra_data_types/test_tutorial001_an_py39.py
+-rw-r--r--   0        0        0     8221 2024-05-12 05:04:33.119448 readyapi-0.111.0.dev1/tests/test_tutorial/test_extra_data_types/test_tutorial001_py310.py
+-rw-r--r--   0        0        0        0 2024-05-12 05:04:33.119448 readyapi-0.111.0.dev1/tests/test_tutorial/test_extra_models/__init__.py
+-rw-r--r--   0        0        0     5197 2024-05-12 05:04:33.119448 readyapi-0.111.0.dev1/tests/test_tutorial/test_extra_models/test_tutorial003.py
+-rw-r--r--   0        0        0     5420 2024-05-12 05:04:33.119448 readyapi-0.111.0.dev1/tests/test_tutorial/test_extra_models/test_tutorial003_py310.py
+-rw-r--r--   0        0        0     1983 2024-05-12 05:04:33.119448 readyapi-0.111.0.dev1/tests/test_tutorial/test_extra_models/test_tutorial004.py
+-rw-r--r--   0        0        0     2171 2024-05-12 05:04:33.119448 readyapi-0.111.0.dev1/tests/test_tutorial/test_extra_models/test_tutorial004_py39.py
+-rw-r--r--   0        0        0     1482 2024-05-12 05:04:33.119448 readyapi-0.111.0.dev1/tests/test_tutorial/test_extra_models/test_tutorial005.py
+-rw-r--r--   0        0        0     1670 2024-05-12 05:04:33.119448 readyapi-0.111.0.dev1/tests/test_tutorial/test_extra_models/test_tutorial005_py39.py
+-rw-r--r--   0        0        0        0 2024-05-12 05:04:33.119448 readyapi-0.111.0.dev1/tests/test_tutorial/test_first_steps/__init__.py
+-rw-r--r--   0        0        0     1207 2024-05-12 05:04:33.119448 readyapi-0.111.0.dev1/tests/test_tutorial/test_first_steps/test_tutorial001.py
+-rw-r--r--   0        0        0        0 2024-05-12 05:04:33.119448 readyapi-0.111.0.dev1/tests/test_tutorial/test_generate_clients/__init__.py
+-rw-r--r--   0        0        0     7249 2024-05-12 05:04:33.119448 readyapi-0.111.0.dev1/tests/test_tutorial/test_generate_clients/test_tutorial003.py
+-rw-r--r--   0        0        0        0 2024-05-12 05:04:33.119448 readyapi-0.111.0.dev1/tests/test_tutorial/test_handling_errors/__init__.py
+-rw-r--r--   0        0        0     3300 2024-05-12 05:04:33.119448 readyapi-0.111.0.dev1/tests/test_tutorial/test_handling_errors/test_tutorial001.py
+-rw-r--r--   0        0        0     3373 2024-05-12 05:04:33.119448 readyapi-0.111.0.dev1/tests/test_tutorial/test_handling_errors/test_tutorial002.py
+-rw-r--r--   0        0        0     3296 2024-05-12 05:04:33.119448 readyapi-0.111.0.dev1/tests/test_tutorial/test_handling_errors/test_tutorial003.py
+-rw-r--r--   0        0        0     3802 2024-05-12 05:04:33.119448 readyapi-0.111.0.dev1/tests/test_tutorial/test_handling_errors/test_tutorial004.py
+-rw-r--r--   0        0        0     4431 2024-05-12 05:04:33.119448 readyapi-0.111.0.dev1/tests/test_tutorial/test_handling_errors/test_tutorial005.py
+-rw-r--r--   0        0        0     4074 2024-05-12 05:04:33.119448 readyapi-0.111.0.dev1/tests/test_tutorial/test_handling_errors/test_tutorial006.py
+-rw-r--r--   0        0        0        0 2024-05-12 05:04:33.119448 readyapi-0.111.0.dev1/tests/test_tutorial/test_header_params/__init__.py
+-rw-r--r--   0        0        0     3932 2024-05-12 05:04:33.119448 readyapi-0.111.0.dev1/tests/test_tutorial/test_header_params/test_tutorial001.py
+-rw-r--r--   0        0        0     3935 2024-05-12 05:04:33.119448 readyapi-0.111.0.dev1/tests/test_tutorial/test_header_params/test_tutorial001_an.py
+-rw-r--r--   0        0        0     4115 2024-05-12 05:04:33.119448 readyapi-0.111.0.dev1/tests/test_tutorial/test_header_params/test_tutorial001_an_py310.py
+-rw-r--r--   0        0        0     4112 2024-05-12 05:04:33.119448 readyapi-0.111.0.dev1/tests/test_tutorial/test_header_params/test_tutorial001_py310.py
+-rw-r--r--   0        0        0     4099 2024-05-12 05:04:33.119448 readyapi-0.111.0.dev1/tests/test_tutorial/test_header_params/test_tutorial002.py
+-rw-r--r--   0        0        0     4102 2024-05-12 05:04:33.119448 readyapi-0.111.0.dev1/tests/test_tutorial/test_header_params/test_tutorial002_an.py
+-rw-r--r--   0        0        0     4282 2024-05-12 05:04:33.119448 readyapi-0.111.0.dev1/tests/test_tutorial/test_header_params/test_tutorial002_an_py310.py
+-rw-r--r--   0        0        0     4353 2024-05-12 05:04:33.119448 readyapi-0.111.0.dev1/tests/test_tutorial/test_header_params/test_tutorial002_an_py39.py
+-rw-r--r--   0        0        0     4352 2024-05-12 05:04:33.119448 readyapi-0.111.0.dev1/tests/test_tutorial/test_header_params/test_tutorial002_py310.py
+-rw-r--r--   0        0        0     4242 2024-05-12 05:04:33.119448 readyapi-0.111.0.dev1/tests/test_tutorial/test_header_params/test_tutorial003.py
+-rw-r--r--   0        0        0     4227 2024-05-12 05:04:33.119448 readyapi-0.111.0.dev1/tests/test_tutorial/test_header_params/test_tutorial003_an.py
+-rw-r--r--   0        0        0     4407 2024-05-12 05:04:33.123448 readyapi-0.111.0.dev1/tests/test_tutorial/test_header_params/test_tutorial003_an_py310.py
+-rw-r--r--   0        0        0     4403 2024-05-12 05:04:33.123448 readyapi-0.111.0.dev1/tests/test_tutorial/test_header_params/test_tutorial003_an_py39.py
+-rw-r--r--   0        0        0     4404 2024-05-12 05:04:33.123448 readyapi-0.111.0.dev1/tests/test_tutorial/test_header_params/test_tutorial003_py310.py
+-rw-r--r--   0        0        0        0 2024-05-12 05:04:33.123448 readyapi-0.111.0.dev1/tests/test_tutorial/test_metadata/__init__.py
+-rw-r--r--   0        0        0     1765 2024-05-12 05:04:33.123448 readyapi-0.111.0.dev1/tests/test_tutorial/test_metadata/test_tutorial001.py
+-rw-r--r--   0        0        0     1729 2024-05-12 05:04:33.123448 readyapi-0.111.0.dev1/tests/test_tutorial/test_metadata/test_tutorial001_1.py
+-rw-r--r--   0        0        0     2082 2024-05-12 05:04:33.123448 readyapi-0.111.0.dev1/tests/test_tutorial/test_metadata/test_tutorial004.py
+-rw-r--r--   0        0        0        0 2024-05-12 05:04:33.123448 readyapi-0.111.0.dev1/tests/test_tutorial/test_openapi_callbacks/__init__.py
+-rw-r--r--   0        0        0     9218 2024-05-12 05:04:33.123448 readyapi-0.111.0.dev1/tests/test_tutorial/test_openapi_callbacks/test_tutorial001.py
+-rw-r--r--   0        0        0        0 2024-05-12 05:04:33.123448 readyapi-0.111.0.dev1/tests/test_tutorial/test_openapi_webhooks/__init__.py
+-rw-r--r--   0        0        0     4494 2024-05-12 05:04:33.123448 readyapi-0.111.0.dev1/tests/test_tutorial/test_openapi_webhooks/test_tutorial001.py
+-rw-r--r--   0        0        0        0 2024-05-12 05:04:33.123448 readyapi-0.111.0.dev1/tests/test_tutorial/test_path_operation_advanced_configurations/__init__.py
+-rw-r--r--   0        0        0     1039 2024-05-12 05:04:33.123448 readyapi-0.111.0.dev1/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial001.py
+-rw-r--r--   0        0        0     1022 2024-05-12 05:04:33.123448 readyapi-0.111.0.dev1/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial002.py
+-rw-r--r--   0        0        0      577 2024-05-12 05:04:33.123448 readyapi-0.111.0.dev1/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial003.py
+-rw-r--r--   0        0        0     8918 2024-05-12 05:04:33.123448 readyapi-0.111.0.dev1/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial004.py
+-rw-r--r--   0        0        0     1036 2024-05-12 05:04:33.123448 readyapi-0.111.0.dev1/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial005.py
+-rw-r--r--   0        0        0     1989 2024-05-12 05:04:33.123448 readyapi-0.111.0.dev1/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial006.py
+-rw-r--r--   0        0        0     3421 2024-05-12 05:04:33.123448 readyapi-0.111.0.dev1/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial007.py
+-rw-r--r--   0        0        0     3268 2024-05-12 05:04:33.123448 readyapi-0.111.0.dev1/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial007_pv1.py
+-rw-r--r--   0        0        0        0 2024-05-12 05:04:33.123448 readyapi-0.111.0.dev1/tests/test_tutorial/test_path_operation_configurations/__init__.py
+-rw-r--r--   0        0        0     1724 2024-05-12 05:04:33.123448 readyapi-0.111.0.dev1/tests/test_tutorial/test_path_operation_configurations/test_tutorial002b.py
+-rw-r--r--   0        0        0     8903 2024-05-12 05:04:33.123448 readyapi-0.111.0.dev1/tests/test_tutorial/test_path_operation_configurations/test_tutorial005.py
+-rw-r--r--   0        0        0     9105 2024-05-12 05:04:33.123448 readyapi-0.111.0.dev1/tests/test_tutorial/test_path_operation_configurations/test_tutorial005_py310.py
+-rw-r--r--   0        0        0     9100 2024-05-12 05:04:33.123448 readyapi-0.111.0.dev1/tests/test_tutorial/test_path_operation_configurations/test_tutorial005_py39.py
+-rw-r--r--   0        0        0     2407 2024-05-12 05:04:33.123448 readyapi-0.111.0.dev1/tests/test_tutorial/test_path_operation_configurations/test_tutorial006.py
+-rw-r--r--   0        0        0        0 2024-05-12 05:04:33.123448 readyapi-0.111.0.dev1/tests/test_tutorial/test_path_params/__init__.py
+-rw-r--r--   0        0        0     3371 2024-05-12 05:04:33.123448 readyapi-0.111.0.dev1/tests/test_tutorial/test_path_params/test_tutorial004.py
+-rw-r--r--   0        0        0     5144 2024-05-12 05:04:33.123448 readyapi-0.111.0.dev1/tests/test_tutorial/test_path_params/test_tutorial005.py
+-rw-r--r--   0        0        0        0 2024-05-12 05:04:33.123448 readyapi-0.111.0.dev1/tests/test_tutorial/test_query_params/__init__.py
+-rw-r--r--   0        0        0     4074 2024-05-12 05:04:33.123448 readyapi-0.111.0.dev1/tests/test_tutorial/test_query_params/test_tutorial005.py
+-rw-r--r--   0        0        0     6287 2024-05-12 05:04:33.123448 readyapi-0.111.0.dev1/tests/test_tutorial/test_query_params/test_tutorial006.py
+-rw-r--r--   0        0        0     6366 2024-05-12 05:04:33.123448 readyapi-0.111.0.dev1/tests/test_tutorial/test_query_params/test_tutorial006_py310.py
+-rw-r--r--   0        0        0        0 2024-05-12 05:04:33.123448 readyapi-0.111.0.dev1/tests/test_tutorial/test_query_params_str_validations/__init__.py
+-rw-r--r--   0        0        0     6390 2024-05-12 05:04:33.123448 readyapi-0.111.0.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial010.py
+-rw-r--r--   0        0        0     6393 2024-05-12 05:04:33.123448 readyapi-0.111.0.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial010_an.py
+-rw-r--r--   0        0        0     6498 2024-05-12 05:04:33.123448 readyapi-0.111.0.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial010_an_py310.py
+-rw-r--r--   0        0        0     6491 2024-05-12 05:04:33.123448 readyapi-0.111.0.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial010_an_py39.py
+-rw-r--r--   0        0        0     6495 2024-05-12 05:04:33.123448 readyapi-0.111.0.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial010_py310.py
+-rw-r--r--   0        0        0     4019 2024-05-12 05:04:33.123448 readyapi-0.111.0.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial011.py
+-rw-r--r--   0        0        0     4022 2024-05-12 05:04:33.123448 readyapi-0.111.0.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial011_an.py
+-rw-r--r--   0        0        0     4245 2024-05-12 05:04:33.123448 readyapi-0.111.0.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial011_an_py310.py
+-rw-r--r--   0        0        0     4240 2024-05-12 05:04:33.123448 readyapi-0.111.0.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial011_an_py39.py
+-rw-r--r--   0        0        0     4242 2024-05-12 05:04:33.123448 readyapi-0.111.0.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial011_py310.py
+-rw-r--r--   0        0        0     4237 2024-05-12 05:04:33.123448 readyapi-0.111.0.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial011_py39.py
+-rw-r--r--   0        0        0     3487 2024-05-12 05:04:33.123448 readyapi-0.111.0.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial012.py
+-rw-r--r--   0        0        0     3490 2024-05-12 05:04:33.123448 readyapi-0.111.0.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial012_an.py
+-rw-r--r--   0        0        0     3708 2024-05-12 05:04:33.123448 readyapi-0.111.0.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial012_an_py39.py
+-rw-r--r--   0        0        0     3705 2024-05-12 05:04:33.123448 readyapi-0.111.0.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial012_py39.py
+-rw-r--r--   0        0        0     3436 2024-05-12 05:04:33.123448 readyapi-0.111.0.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial013.py
+-rw-r--r--   0        0        0     3439 2024-05-12 05:04:33.123448 readyapi-0.111.0.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial013_an.py
+-rw-r--r--   0        0        0     3657 2024-05-12 05:04:33.123448 readyapi-0.111.0.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial013_an_py39.py
+-rw-r--r--   0        0        0     2939 2024-05-12 05:04:33.123448 readyapi-0.111.0.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial014.py
+-rw-r--r--   0        0        0     2942 2024-05-12 05:04:33.123448 readyapi-0.111.0.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial014_an.py
+-rw-r--r--   0        0        0     3165 2024-05-12 05:04:33.123448 readyapi-0.111.0.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial014_an_py310.py
+-rw-r--r--   0        0        0     3164 2024-05-12 05:04:33.123448 readyapi-0.111.0.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial014_an_py39.py
+-rw-r--r--   0        0        0     3162 2024-05-12 05:04:33.123448 readyapi-0.111.0.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial014_py310.py
+-rw-r--r--   0        0        0        0 2024-05-12 05:04:33.123448 readyapi-0.111.0.dev1/tests/test_tutorial/test_request_files/__init__.py
+-rw-r--r--   0        0        0     7888 2024-05-12 05:04:33.123448 readyapi-0.111.0.dev1/tests/test_tutorial/test_request_files/test_tutorial001.py
+-rw-r--r--   0        0        0     8390 2024-05-12 05:04:33.123448 readyapi-0.111.0.dev1/tests/test_tutorial/test_request_files/test_tutorial001_02.py
+-rw-r--r--   0        0        0     8393 2024-05-12 05:04:33.123448 readyapi-0.111.0.dev1/tests/test_tutorial/test_request_files/test_tutorial001_02_an.py
+-rw-r--r--   0        0        0     8662 2024-05-12 05:04:33.123448 readyapi-0.111.0.dev1/tests/test_tutorial/test_request_files/test_tutorial001_02_an_py310.py
+-rw-r--r--   0        0        0     8655 2024-05-12 05:04:33.123448 readyapi-0.111.0.dev1/tests/test_tutorial/test_request_files/test_tutorial001_02_an_py39.py
+-rw-r--r--   0        0        0     8659 2024-05-12 05:04:33.123448 readyapi-0.111.0.dev1/tests/test_tutorial/test_request_files/test_tutorial001_02_py310.py
+-rw-r--r--   0        0        0     6135 2024-05-12 05:04:33.123448 readyapi-0.111.0.dev1/tests/test_tutorial/test_request_files/test_tutorial001_03.py
+-rw-r--r--   0        0        0     6138 2024-05-12 05:04:33.123448 readyapi-0.111.0.dev1/tests/test_tutorial/test_request_files/test_tutorial001_03_an.py
+-rw-r--r--   0        0        0     6302 2024-05-12 05:04:33.123448 readyapi-0.111.0.dev1/tests/test_tutorial/test_request_files/test_tutorial001_03_an_py39.py
+-rw-r--r--   0        0        0     7710 2024-05-12 05:04:33.123448 readyapi-0.111.0.dev1/tests/test_tutorial/test_request_files/test_tutorial001_an.py
+-rw-r--r--   0        0        0     7937 2024-05-12 05:04:33.123448 readyapi-0.111.0.dev1/tests/test_tutorial/test_request_files/test_tutorial001_an_py39.py
+-rw-r--r--   0        0        0     8681 2024-05-12 05:04:33.123448 readyapi-0.111.0.dev1/tests/test_tutorial/test_request_files/test_tutorial002.py
+-rw-r--r--   0        0        0     8684 2024-05-12 05:04:33.123448 readyapi-0.111.0.dev1/tests/test_tutorial/test_request_files/test_tutorial002_an.py
+-rw-r--r--   0        0        0     9084 2024-05-12 05:04:33.123448 readyapi-0.111.0.dev1/tests/test_tutorial/test_request_files/test_tutorial002_an_py39.py
+-rw-r--r--   0        0        0     9263 2024-05-12 05:04:33.123448 readyapi-0.111.0.dev1/tests/test_tutorial/test_request_files/test_tutorial002_py39.py
+-rw-r--r--   0        0        0     7313 2024-05-12 05:04:33.127448 readyapi-0.111.0.dev1/tests/test_tutorial/test_request_files/test_tutorial003.py
+-rw-r--r--   0        0        0     7316 2024-05-12 05:04:33.127448 readyapi-0.111.0.dev1/tests/test_tutorial/test_request_files/test_tutorial003_an.py
+-rw-r--r--   0        0        0     7838 2024-05-12 05:04:33.127448 readyapi-0.111.0.dev1/tests/test_tutorial/test_request_files/test_tutorial003_an_py39.py
+-rw-r--r--   0        0        0     7835 2024-05-12 05:04:33.127448 readyapi-0.111.0.dev1/tests/test_tutorial/test_request_files/test_tutorial003_py39.py
+-rw-r--r--   0        0        0        0 2024-05-12 05:04:33.127448 readyapi-0.111.0.dev1/tests/test_tutorial/test_request_forms/__init__.py
+-rw-r--r--   0        0        0     7632 2024-05-12 05:04:33.127448 readyapi-0.111.0.dev1/tests/test_tutorial/test_request_forms/test_tutorial001.py
+-rw-r--r--   0        0        0     7635 2024-05-12 05:04:33.127448 readyapi-0.111.0.dev1/tests/test_tutorial/test_request_forms/test_tutorial001_an.py
+-rw-r--r--   0        0        0     7745 2024-05-12 05:04:33.127448 readyapi-0.111.0.dev1/tests/test_tutorial/test_request_forms/test_tutorial001_an_py39.py
+-rw-r--r--   0        0        0        0 2024-05-12 05:04:33.127448 readyapi-0.111.0.dev1/tests/test_tutorial/test_request_forms_and_files/__init__.py
+-rw-r--r--   0        0        0    10049 2024-05-12 05:04:33.127448 readyapi-0.111.0.dev1/tests/test_tutorial/test_request_forms_and_files/test_tutorial001.py
+-rw-r--r--   0        0        0    10052 2024-05-12 05:04:33.127448 readyapi-0.111.0.dev1/tests/test_tutorial/test_request_forms_and_files/test_tutorial001_an.py
+-rw-r--r--   0        0        0    10162 2024-05-12 05:04:33.127448 readyapi-0.111.0.dev1/tests/test_tutorial/test_request_forms_and_files/test_tutorial001_an_py39.py
+-rw-r--r--   0        0        0        0 2024-05-12 05:04:33.127448 readyapi-0.111.0.dev1/tests/test_tutorial/test_response_change_status_code/__init__.py
+-rw-r--r--   0        0        0      522 2024-05-12 05:04:33.127448 readyapi-0.111.0.dev1/tests/test_tutorial/test_response_change_status_code/test_tutorial001.py
+-rw-r--r--   0        0        0        0 2024-05-12 05:04:33.127448 readyapi-0.111.0.dev1/tests/test_tutorial/test_response_cookies/__init__.py
+-rw-r--r--   0        0        0      404 2024-05-12 05:04:33.127448 readyapi-0.111.0.dev1/tests/test_tutorial/test_response_cookies/test_tutorial001.py
+-rw-r--r--   0        0        0      415 2024-05-12 05:04:33.127448 readyapi-0.111.0.dev1/tests/test_tutorial/test_response_cookies/test_tutorial002.py
+-rw-r--r--   0        0        0        0 2024-05-12 05:04:33.127448 readyapi-0.111.0.dev1/tests/test_tutorial/test_response_headers/__init__.py
+-rw-r--r--   0        0        0      427 2024-05-12 05:04:33.127448 readyapi-0.111.0.dev1/tests/test_tutorial/test_response_headers/test_tutorial001.py
+-rw-r--r--   0        0        0      379 2024-05-12 05:04:33.127448 readyapi-0.111.0.dev1/tests/test_tutorial/test_response_headers/test_tutorial002.py
+-rw-r--r--   0        0        0        0 2024-05-12 05:04:33.127448 readyapi-0.111.0.dev1/tests/test_tutorial/test_response_model/__init__.py
+-rw-r--r--   0        0        0     5766 2024-05-12 05:04:33.127448 readyapi-0.111.0.dev1/tests/test_tutorial/test_response_model/test_tutorial003.py
+-rw-r--r--   0        0        0     5772 2024-05-12 05:04:33.127448 readyapi-0.111.0.dev1/tests/test_tutorial/test_response_model/test_tutorial003_01.py
+-rw-r--r--   0        0        0     5964 2024-05-12 05:04:33.127448 readyapi-0.111.0.dev1/tests/test_tutorial/test_response_model/test_tutorial003_01_py310.py
+-rw-r--r--   0        0        0     3478 2024-05-12 05:04:33.127448 readyapi-0.111.0.dev1/tests/test_tutorial/test_response_model/test_tutorial003_02.py
+-rw-r--r--   0        0        0     1092 2024-05-12 05:04:33.127448 readyapi-0.111.0.dev1/tests/test_tutorial/test_response_model/test_tutorial003_03.py
+-rw-r--r--   0        0        0      239 2024-05-12 05:04:33.127448 readyapi-0.111.0.dev1/tests/test_tutorial/test_response_model/test_tutorial003_04.py
+-rw-r--r--   0        0        0      292 2024-05-12 05:04:33.127448 readyapi-0.111.0.dev1/tests/test_tutorial/test_response_model/test_tutorial003_04_py310.py
+-rw-r--r--   0        0        0     3478 2024-05-12 05:04:33.127448 readyapi-0.111.0.dev1/tests/test_tutorial/test_response_model/test_tutorial003_05.py
+-rw-r--r--   0        0        0     3701 2024-05-12 05:04:33.127448 readyapi-0.111.0.dev1/tests/test_tutorial/test_response_model/test_tutorial003_05_py310.py
+-rw-r--r--   0        0        0     5958 2024-05-12 05:04:33.127448 readyapi-0.111.0.dev1/tests/test_tutorial/test_response_model/test_tutorial003_py310.py
+-rw-r--r--   0        0        0     5110 2024-05-12 05:04:33.127448 readyapi-0.111.0.dev1/tests/test_tutorial/test_response_model/test_tutorial004.py
+-rw-r--r--   0        0        0     5290 2024-05-12 05:04:33.127448 readyapi-0.111.0.dev1/tests/test_tutorial/test_response_model/test_tutorial004_py310.py
+-rw-r--r--   0        0        0     5286 2024-05-12 05:04:33.127448 readyapi-0.111.0.dev1/tests/test_tutorial/test_response_model/test_tutorial004_py39.py
+-rw-r--r--   0        0        0     6156 2024-05-12 05:04:33.127448 readyapi-0.111.0.dev1/tests/test_tutorial/test_response_model/test_tutorial005.py
+-rw-r--r--   0        0        0     6379 2024-05-12 05:04:33.127448 readyapi-0.111.0.dev1/tests/test_tutorial/test_response_model/test_tutorial005_py310.py
+-rw-r--r--   0        0        0     6156 2024-05-12 05:04:33.127448 readyapi-0.111.0.dev1/tests/test_tutorial/test_response_model/test_tutorial006.py
+-rw-r--r--   0        0        0     6379 2024-05-12 05:04:33.127448 readyapi-0.111.0.dev1/tests/test_tutorial/test_response_model/test_tutorial006_py310.py
+-rw-r--r--   0        0        0        0 2024-05-12 05:04:33.127448 readyapi-0.111.0.dev1/tests/test_tutorial/test_schema_extra_example/__init__.py
+-rw-r--r--   0        0        0     4781 2024-05-12 05:04:33.127448 readyapi-0.111.0.dev1/tests/test_tutorial/test_schema_extra_example/test_tutorial001.py
+-rw-r--r--   0        0        0     4557 2024-05-12 05:04:33.127448 readyapi-0.111.0.dev1/tests/test_tutorial/test_schema_extra_example/test_tutorial001_pv1.py
+-rw-r--r--   0        0        0     4826 2024-05-12 05:04:33.127448 readyapi-0.111.0.dev1/tests/test_tutorial/test_schema_extra_example/test_tutorial001_py310.py
+-rw-r--r--   0        0        0     4602 2024-05-12 05:04:33.127448 readyapi-0.111.0.dev1/tests/test_tutorial/test_schema_extra_example/test_tutorial001_py310_pv1.py
+-rw-r--r--   0        0        0     7062 2024-05-12 05:04:33.127448 readyapi-0.111.0.dev1/tests/test_tutorial/test_schema_extra_example/test_tutorial004.py
+-rw-r--r--   0        0        0     7065 2024-05-12 05:04:33.127448 readyapi-0.111.0.dev1/tests/test_tutorial/test_schema_extra_example/test_tutorial004_an.py
+-rw-r--r--   0        0        0     7257 2024-05-12 05:04:33.127448 readyapi-0.111.0.dev1/tests/test_tutorial/test_schema_extra_example/test_tutorial004_an_py310.py
+-rw-r--r--   0        0        0     7253 2024-05-12 05:04:33.127448 readyapi-0.111.0.dev1/tests/test_tutorial/test_schema_extra_example/test_tutorial004_an_py39.py
+-rw-r--r--   0        0        0     7254 2024-05-12 05:04:33.127448 readyapi-0.111.0.dev1/tests/test_tutorial/test_schema_extra_example/test_tutorial004_py310.py
+-rw-r--r--   0        0        0     6910 2024-05-12 05:04:33.127448 readyapi-0.111.0.dev1/tests/test_tutorial/test_schema_extra_example/test_tutorial005.py
+-rw-r--r--   0        0        0     6913 2024-05-12 05:04:33.127448 readyapi-0.111.0.dev1/tests/test_tutorial/test_schema_extra_example/test_tutorial005_an.py
+-rw-r--r--   0        0        0     6979 2024-05-12 05:04:33.127448 readyapi-0.111.0.dev1/tests/test_tutorial/test_schema_extra_example/test_tutorial005_an_py310.py
+-rw-r--r--   0        0        0     6975 2024-05-12 05:04:33.127448 readyapi-0.111.0.dev1/tests/test_tutorial/test_schema_extra_example/test_tutorial005_an_py39.py
+-rw-r--r--   0        0        0     6976 2024-05-12 05:04:33.127448 readyapi-0.111.0.dev1/tests/test_tutorial/test_schema_extra_example/test_tutorial005_py310.py
+-rw-r--r--   0        0        0        0 2024-05-12 05:04:33.127448 readyapi-0.111.0.dev1/tests/test_tutorial/test_security/__init__.py
+-rw-r--r--   0        0        0     1907 2024-05-12 05:04:33.127448 readyapi-0.111.0.dev1/tests/test_tutorial/test_security/test_tutorial001.py
+-rw-r--r--   0        0        0     1910 2024-05-12 05:04:33.127448 readyapi-0.111.0.dev1/tests/test_tutorial/test_security/test_tutorial001_an.py
+-rw-r--r--   0        0        0     2158 2024-05-12 05:04:33.127448 readyapi-0.111.0.dev1/tests/test_tutorial/test_security/test_tutorial001_an_py39.py
+-rw-r--r--   0        0        0     8184 2024-05-12 05:04:33.127448 readyapi-0.111.0.dev1/tests/test_tutorial/test_security/test_tutorial003.py
+-rw-r--r--   0        0        0     8187 2024-05-12 05:04:33.127448 readyapi-0.111.0.dev1/tests/test_tutorial/test_security/test_tutorial003_an.py
+-rw-r--r--   0        0        0     8596 2024-05-12 05:04:33.127448 readyapi-0.111.0.dev1/tests/test_tutorial/test_security/test_tutorial003_an_py310.py
+-rw-r--r--   0        0        0     8585 2024-05-12 05:04:33.127448 readyapi-0.111.0.dev1/tests/test_tutorial/test_security/test_tutorial003_an_py39.py
+-rw-r--r--   0        0        0     8593 2024-05-12 05:04:33.127448 readyapi-0.111.0.dev1/tests/test_tutorial/test_security/test_tutorial003_py310.py
+-rw-r--r--   0        0        0    15805 2024-05-12 05:04:33.127448 readyapi-0.111.0.dev1/tests/test_tutorial/test_security/test_tutorial005.py
+-rw-r--r--   0        0        0    15808 2024-05-12 05:04:33.127448 readyapi-0.111.0.dev1/tests/test_tutorial/test_security/test_tutorial005_an.py
+-rw-r--r--   0        0        0    16713 2024-05-12 05:04:33.127448 readyapi-0.111.0.dev1/tests/test_tutorial/test_security/test_tutorial005_an_py310.py
+-rw-r--r--   0        0        0    16689 2024-05-12 05:04:33.127448 readyapi-0.111.0.dev1/tests/test_tutorial/test_security/test_tutorial005_an_py39.py
+-rw-r--r--   0        0        0    16701 2024-05-12 05:04:33.127448 readyapi-0.111.0.dev1/tests/test_tutorial/test_security/test_tutorial005_py310.py
+-rw-r--r--   0        0        0    16677 2024-05-12 05:04:33.127448 readyapi-0.111.0.dev1/tests/test_tutorial/test_security/test_tutorial005_py39.py
+-rw-r--r--   0        0        0     2320 2024-05-12 05:04:33.127448 readyapi-0.111.0.dev1/tests/test_tutorial/test_security/test_tutorial006.py
+-rw-r--r--   0        0        0     2323 2024-05-12 05:04:33.127448 readyapi-0.111.0.dev1/tests/test_tutorial/test_security/test_tutorial006_an.py
+-rw-r--r--   0        0        0     2596 2024-05-12 05:04:33.127448 readyapi-0.111.0.dev1/tests/test_tutorial/test_security/test_tutorial006_an_py39.py
+-rw-r--r--   0        0        0        0 2024-05-12 05:04:33.127448 readyapi-0.111.0.dev1/tests/test_tutorial/test_separate_openapi_schemas/__init__.py
+-rw-r--r--   0        0        0     4960 2024-05-12 05:04:33.127448 readyapi-0.111.0.dev1/tests/test_tutorial/test_separate_openapi_schemas/test_tutorial001.py
+-rw-r--r--   0        0        0     5018 2024-05-12 05:04:33.127448 readyapi-0.111.0.dev1/tests/test_tutorial/test_separate_openapi_schemas/test_tutorial001_py310.py
+-rw-r--r--   0        0        0     5013 2024-05-12 05:04:33.127448 readyapi-0.111.0.dev1/tests/test_tutorial/test_separate_openapi_schemas/test_tutorial001_py39.py
+-rw-r--r--   0        0        0     4960 2024-05-12 05:04:33.127448 readyapi-0.111.0.dev1/tests/test_tutorial/test_separate_openapi_schemas/test_tutorial002.py
+-rw-r--r--   0        0        0     5018 2024-05-12 05:04:33.127448 readyapi-0.111.0.dev1/tests/test_tutorial/test_separate_openapi_schemas/test_tutorial002_py310.py
+-rw-r--r--   0        0        0     5013 2024-05-12 05:04:33.127448 readyapi-0.111.0.dev1/tests/test_tutorial/test_separate_openapi_schemas/test_tutorial002_py39.py
+-rw-r--r--   0        0        0        0 2024-05-12 05:04:33.127448 readyapi-0.111.0.dev1/tests/test_tutorial/test_settings/__init__.py
+-rw-r--r--   0        0        0      488 2024-05-12 05:04:33.127448 readyapi-0.111.0.dev1/tests/test_tutorial/test_settings/test_app02.py
+-rw-r--r--   0        0        0      553 2024-05-12 05:04:33.127448 readyapi-0.111.0.dev1/tests/test_tutorial/test_settings/test_tutorial001.py
+-rw-r--r--   0        0        0      557 2024-05-12 05:04:33.127448 readyapi-0.111.0.dev1/tests/test_tutorial/test_settings/test_tutorial001_pv1.py
+-rw-r--r--   0        0        0        0 2024-05-12 05:04:33.127448 readyapi-0.111.0.dev1/tests/test_tutorial/test_sql_databases/__init__.py
+-rw-r--r--   0        0        0    16477 2024-05-12 05:04:33.131448 readyapi-0.111.0.dev1/tests/test_tutorial/test_sql_databases/test_sql_databases.py
+-rw-r--r--   0        0        0    16656 2024-05-12 05:04:33.131448 readyapi-0.111.0.dev1/tests/test_tutorial/test_sql_databases/test_sql_databases_middleware.py
+-rw-r--r--   0        0        0    16926 2024-05-12 05:04:33.131448 readyapi-0.111.0.dev1/tests/test_tutorial/test_sql_databases/test_sql_databases_middleware_py310.py
+-rw-r--r--   0        0        0    16927 2024-05-12 05:04:33.131448 readyapi-0.111.0.dev1/tests/test_tutorial/test_sql_databases/test_sql_databases_middleware_py39.py
+-rw-r--r--   0        0        0    16932 2024-05-12 05:04:33.131448 readyapi-0.111.0.dev1/tests/test_tutorial/test_sql_databases/test_sql_databases_py310.py
+-rw-r--r--   0        0        0    16923 2024-05-12 05:04:33.131448 readyapi-0.111.0.dev1/tests/test_tutorial/test_sql_databases/test_sql_databases_py39.py
+-rw-r--r--   0        0        0      788 2024-05-12 05:04:33.131448 readyapi-0.111.0.dev1/tests/test_tutorial/test_sql_databases/test_testing_databases.py
+-rw-r--r--   0        0        0      825 2024-05-12 05:04:33.131448 readyapi-0.111.0.dev1/tests/test_tutorial/test_sql_databases/test_testing_databases_py310.py
+-rw-r--r--   0        0        0      822 2024-05-12 05:04:33.131448 readyapi-0.111.0.dev1/tests/test_tutorial/test_sql_databases/test_testing_databases_py39.py
+-rw-r--r--   0        0        0        0 2024-05-12 05:04:33.131448 readyapi-0.111.0.dev1/tests/test_tutorial/test_sub_applications/__init__.py
+-rw-r--r--   0        0        0     1923 2024-05-12 05:04:33.131448 readyapi-0.111.0.dev1/tests/test_tutorial/test_sub_applications/test_tutorial001.py
+-rw-r--r--   0        0        0        0 2024-05-12 05:04:33.131448 readyapi-0.111.0.dev1/tests/test_tutorial/test_templates/__init__.py
+-rw-r--r--   0        0        0      911 2024-05-12 05:04:33.131448 readyapi-0.111.0.dev1/tests/test_tutorial/test_templates/test_tutorial001.py
+-rw-r--r--   0        0        0        0 2024-05-12 05:04:33.131448 readyapi-0.111.0.dev1/tests/test_tutorial/test_testing/__init__.py
+-rw-r--r--   0        0        0      820 2024-05-12 05:04:33.131448 readyapi-0.111.0.dev1/tests/test_tutorial/test_testing/test_main.py
+-rw-r--r--   0        0        0      300 2024-05-12 05:04:33.131448 readyapi-0.111.0.dev1/tests/test_tutorial/test_testing/test_main_b.py
+-rw-r--r--   0        0        0      303 2024-05-12 05:04:33.131448 readyapi-0.111.0.dev1/tests/test_tutorial/test_testing/test_main_b_an.py
+-rw-r--r--   0        0        0      360 2024-05-12 05:04:33.131448 readyapi-0.111.0.dev1/tests/test_tutorial/test_testing/test_main_b_an_py310.py
+-rw-r--r--   0        0        0      357 2024-05-12 05:04:33.131448 readyapi-0.111.0.dev1/tests/test_tutorial/test_testing/test_main_b_an_py39.py
+-rw-r--r--   0        0        0      357 2024-05-12 05:04:33.131448 readyapi-0.111.0.dev1/tests/test_tutorial/test_testing/test_main_b_py310.py
+-rw-r--r--   0        0        0      822 2024-05-12 05:04:33.131448 readyapi-0.111.0.dev1/tests/test_tutorial/test_testing/test_tutorial001.py
+-rw-r--r--   0        0        0      154 2024-05-12 05:04:33.131448 readyapi-0.111.0.dev1/tests/test_tutorial/test_testing/test_tutorial002.py
+-rw-r--r--   0        0        0      167 2024-05-12 05:04:33.131448 readyapi-0.111.0.dev1/tests/test_tutorial/test_testing/test_tutorial003.py
+-rw-r--r--   0        0        0        0 2024-05-12 05:04:33.131448 readyapi-0.111.0.dev1/tests/test_tutorial/test_testing_dependencies/__init__.py
+-rw-r--r--   0        0        0     1527 2024-05-12 05:04:33.131448 readyapi-0.111.0.dev1/tests/test_tutorial/test_testing_dependencies/test_tutorial001.py
+-rw-r--r--   0        0        0     1530 2024-05-12 05:04:33.131448 readyapi-0.111.0.dev1/tests/test_tutorial/test_testing_dependencies/test_tutorial001_an.py
+-rw-r--r--   0        0        0     2088 2024-05-12 05:04:33.131448 readyapi-0.111.0.dev1/tests/test_tutorial/test_testing_dependencies/test_tutorial001_an_py310.py
+-rw-r--r--   0        0        0     2073 2024-05-12 05:04:33.131448 readyapi-0.111.0.dev1/tests/test_tutorial/test_testing_dependencies/test_tutorial001_an_py39.py
+-rw-r--r--   0        0        0     2067 2024-05-12 05:04:33.131448 readyapi-0.111.0.dev1/tests/test_tutorial/test_testing_dependencies/test_tutorial001_py310.py
+-rw-r--r--   0        0        0        0 2024-05-12 05:04:33.131448 readyapi-0.111.0.dev1/tests/test_tutorial/test_websockets/__init__.py
+-rw-r--r--   0        0        0      824 2024-05-12 05:04:33.131448 readyapi-0.111.0.dev1/tests/test_tutorial/test_websockets/test_tutorial001.py
+-rw-r--r--   0        0        0     3685 2024-05-12 05:04:33.131448 readyapi-0.111.0.dev1/tests/test_tutorial/test_websockets/test_tutorial002.py
+-rw-r--r--   0        0        0     3688 2024-05-12 05:04:33.131448 readyapi-0.111.0.dev1/tests/test_tutorial/test_websockets/test_tutorial002_an.py
+-rw-r--r--   0        0        0     3978 2024-05-12 05:04:33.131448 readyapi-0.111.0.dev1/tests/test_tutorial/test_websockets/test_tutorial002_an_py310.py
+-rw-r--r--   0        0        0     3970 2024-05-12 05:04:33.131448 readyapi-0.111.0.dev1/tests/test_tutorial/test_websockets/test_tutorial002_an_py39.py
+-rw-r--r--   0        0        0     3975 2024-05-12 05:04:33.131448 readyapi-0.111.0.dev1/tests/test_tutorial/test_websockets/test_tutorial002_py310.py
+-rw-r--r--   0        0        0      873 2024-05-12 05:04:33.131448 readyapi-0.111.0.dev1/tests/test_tutorial/test_websockets/test_tutorial003.py
+-rw-r--r--   0        0        0     1292 2024-05-12 05:04:33.131448 readyapi-0.111.0.dev1/tests/test_tutorial/test_websockets/test_tutorial003_py39.py
+-rw-r--r--   0        0        0        0 2024-05-12 05:04:33.131448 readyapi-0.111.0.dev1/tests/test_tutorial/test_wsgi/__init__.py
+-rw-r--r--   0        0        0      437 2024-05-12 05:04:33.131448 readyapi-0.111.0.dev1/tests/test_tutorial/test_wsgi/test_tutorial001.py
+-rw-r--r--   0        0        0      713 2024-05-12 05:04:33.131448 readyapi-0.111.0.dev1/tests/test_typing_python39.py
+-rw-r--r--   0        0        0     4753 2024-05-12 05:04:33.131448 readyapi-0.111.0.dev1/tests/test_union_body.py
+-rw-r--r--   0        0        0     5316 2024-05-12 05:04:33.131448 readyapi-0.111.0.dev1/tests/test_union_inherited_body.py
+-rw-r--r--   0        0        0     2036 2024-05-12 05:04:33.131448 readyapi-0.111.0.dev1/tests/test_validate_response.py
+-rw-r--r--   0        0        0     1213 2024-05-12 05:04:33.131448 readyapi-0.111.0.dev1/tests/test_validate_response_dataclass.py
+-rw-r--r--   0        0        0        0 2024-05-12 05:04:33.131448 readyapi-0.111.0.dev1/tests/test_validate_response_recursive/__init__.py
+-rw-r--r--   0        0        0     1152 2024-05-12 05:04:33.131448 readyapi-0.111.0.dev1/tests/test_validate_response_recursive/app_pv1.py
+-rw-r--r--   0        0        0     1181 2024-05-12 05:04:33.131448 readyapi-0.111.0.dev1/tests/test_validate_response_recursive/app_pv2.py
+-rw-r--r--   0        0        0      901 2024-05-12 05:04:33.131448 readyapi-0.111.0.dev1/tests/test_validate_response_recursive/test_validate_response_recursive_pv1.py
+-rw-r--r--   0        0        0      901 2024-05-12 05:04:33.131448 readyapi-0.111.0.dev1/tests/test_validate_response_recursive/test_validate_response_recursive_pv2.py
+-rw-r--r--   0        0        0     4673 2024-05-12 05:04:33.131448 readyapi-0.111.0.dev1/tests/test_webhooks_security.py
+-rw-r--r--   0        0        0     2203 2024-05-12 05:04:33.131448 readyapi-0.111.0.dev1/tests/test_ws_dependencies.py
+-rw-r--r--   0        0        0     7657 2024-05-12 05:04:33.131448 readyapi-0.111.0.dev1/tests/test_ws_router.py
+-rw-r--r--   0        0        0      423 2024-05-12 05:04:33.131448 readyapi-0.111.0.dev1/tests/utils.py
+-rw-r--r--   0        0        0    23163 1970-01-01 00:00:00.000000 readyapi-0.111.0.dev1/PKG-INFO
```

### Comparing `readyapi-0.110.3/LICENSE` & `readyapi-0.111.0.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/README.md` & `readyapi-0.111.0.dev1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,67 @@
+Metadata-Version: 2.1
+Name: readyapi
+Version: 0.111.0.dev1
+Summary: ReadyAPI framework, high performance, easy to learn, fast to code, ready for production
+Author-Email: KhulnaSoft DevOps <info@khulnasoft.com>
+Classifier: Intended Audience :: Information Technology
+Classifier: Intended Audience :: System Administrators
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python
+Classifier: Topic :: Internet
+Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development
+Classifier: Typing :: Typed
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Web Environment
+Classifier: Framework :: AsyncIO
+Classifier: Framework :: Pydantic
+Classifier: Framework :: Pydantic :: 1
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
+Classifier: Topic :: Internet :: WWW/HTTP
+Project-URL: Homepage, https://github.com/khulnasoft/readyapi
+Project-URL: Documentation, https://readyapi.khulnasoft.com/
+Project-URL: Repository, https://github.com/khulnasoft/readyapi
+Requires-Python: >=3.8
+Requires-Dist: starlette<0.38.0,>=0.37.2
+Requires-Dist: pydantic!=1.8,!=1.8.1,!=2.0.0,!=2.0.1,!=2.1.0,<3.0.0,>=1.7.4
+Requires-Dist: typing-extensions>=4.8.0
+Requires-Dist: readyapi-cli>=0.0.2
+Requires-Dist: httpx>=0.23.0
+Requires-Dist: jinja2>=2.11.2
+Requires-Dist: python-multipart>=0.0.7
+Requires-Dist: ujson!=4.0.2,!=4.1.0,!=4.2.0,!=4.3.0,!=5.0.0,!=5.1.0,>=4.0.1
+Requires-Dist: orjson>=3.2.1
+Requires-Dist: email_validator>=2.0.0
+Requires-Dist: uvicorn[standard]>=0.12.0
+Requires-Dist: httpx>=0.23.0; extra == "all"
+Requires-Dist: jinja2>=2.11.2; extra == "all"
+Requires-Dist: python-multipart>=0.0.7; extra == "all"
+Requires-Dist: itsdangerous>=1.1.0; extra == "all"
+Requires-Dist: pyyaml>=5.3.1; extra == "all"
+Requires-Dist: ujson!=4.0.2,!=4.1.0,!=4.2.0,!=4.3.0,!=5.0.0,!=5.1.0,>=4.0.1; extra == "all"
+Requires-Dist: orjson>=3.2.1; extra == "all"
+Requires-Dist: email_validator>=2.0.0; extra == "all"
+Requires-Dist: uvicorn[standard]>=0.12.0; extra == "all"
+Requires-Dist: pydantic-settings>=2.0.0; extra == "all"
+Requires-Dist: pydantic-extra-types>=2.0.0; extra == "all"
+Provides-Extra: all
+Description-Content-Type: text/markdown
+
 <p align="center">
   <a href="https://readyapi.khulnasoft.com"><img src="https://readyapi.khulnasoft.com/img/logo-margin/logo-teal.png" alt="ReadyAPI"></a>
 </p>
 <p align="center">
     <em>ReadyAPI framework, high performance, easy to learn, fast to code, ready for production</em>
 </p>
 <p align="center">
@@ -22,15 +82,16 @@
 ---
 
 **Documentation**: <a href="https://readyapi.khulnasoft.com" target="_blank">https://readyapi.khulnasoft.com</a>
 
 **Source Code**: <a href="https://github.com/khulnasoft/readyapi" target="_blank">https://github.com/khulnasoft/readyapi</a>
 
 ---
-ReadyAPI is a modern, fast (high-performance), web framework for building APIs with Python 3.8+ based on standard Python type hints.
+
+ReadyAPI is a modern, fast (high-performance), web framework for building APIs with Python based on standard Python type hints.
 
 The key features are:
 
 * **Fast**: Very high performance, on par with **NodeJS** and **Go** (thanks to Starlette and Pydantic). [One of the fastest Python frameworks available](#performance).
 * **Fast to code**: Increase the speed to develop features by about 200% to 300%. *
 * **Fewer bugs**: Reduce about 40% of human (developer) induced errors. *
 * **Intuitive**: Great editor support. <abbr title="also known as auto-complete, autocompletion, IntelliSense">Completion</abbr> everywhere. Less time debugging.
@@ -41,29 +102,22 @@
 
 <small>* estimation based on tests on an internal development team, building production applications.</small>
 
 ## Sponsors
 
 <!-- sponsors -->
 
-<a href="https://cryptapi.io/" target="_blank" title="CryptAPI: Your easy to use, secure and privacy oriented payment gateway."><img src="https://readyapi.khulnasoft.com/img/sponsors/cryptapi.svg"></a>
-<a href="https://platform.sh/try-it-now/?utm_source=readyapi-signup&utm_medium=banner&utm_campaign=ReadyAPI-signup-June-2023" target="_blank" title="Build, run and scale your apps on a modern, reliable, and secure PaaS."><img src="https://readyapi.khulnasoft.com/img/sponsors/platform-sh.png"></a>
-<a href="https://www.porter.run" target="_blank" title="Deploy ReadyAPI on AWS with a few clicks"><img src="https://readyapi.khulnasoft.com/img/sponsors/porter.png"></a>
-<a href="https://bump.sh/readyapi?utm_source=readyapi&utm_medium=referral&utm_campaign=sponsor" target="_blank" title="Automate ReadyAPI documentation generation with Bump.sh"><img src="https://readyapi.khulnasoft.com/img/sponsors/bump-sh.svg"></a>
-<a href="https://reflex.dev" target="_blank" title="Reflex"><img src="https://readyapi.khulnasoft.com/img/sponsors/reflex.png"></a>
-<a href="https://github.com/scalar/scalar/?utm_source=readyapi&utm_medium=website&utm_campaign=main-badge" target="_blank" title="Scalar: Beautiful Open-Source API References from Swagger/OpenAPI files"><img src="https://readyapi.khulnasoft.com/img/sponsors/scalar.svg"></a>
-<a href="https://www.propelauth.com/?utm_source=readyapi&utm_campaign=1223&utm_medium=mainbadge" target="_blank" title="Auth, user management and more for your B2B product"><img src="https://readyapi.khulnasoft.com/img/sponsors/propelauth.png"></a>
-<a href="https://www.withcoherence.com/?utm_medium=advertising&utm_source=readyapi&utm_campaign=banner%20january%2024" target="_blank" title="Coherence"><img src="https://readyapi.khulnasoft.com/img/sponsors/coherence.png"></a>
-<a href="https://www.mongodb.com/developer/languages/python/python-quickstart-readyapi/?utm_campaign=readyapi_framework&utm_source=readyapi_sponsorship&utm_medium=web_referral" target="_blank" title="Simplify Full Stack Development with ReadyAPI & MongoDB"><img src="https://readyapi.khulnasoft.com/img/sponsors/mongodb.png"></a>
-<a href="https://training.talkpython.fm/readyapi-courses" target="_blank" title="ReadyAPI video courses on demand from people you trust"><img src="https://readyapi.khulnasoft.com/img/sponsors/talkpython-v2.jpg"></a>
-<a href="https://github.com/deepset-ai/haystack/" target="_blank" title="Build powerful search from composable, open source building blocks"><img src="https://readyapi.khulnasoft.com/img/sponsors/haystack-readyapi.svg"></a>
-<a href="https://databento.com/" target="_blank" title="Pay as you go for market data"><img src="https://readyapi.khulnasoft.com/img/sponsors/databento.svg"></a>
-<a href="https://speakeasyapi.dev?utm_source=readyapi+repo&utm_medium=github+sponsorship" target="_blank" title="SDKs for your API | Speakeasy"><img src="https://readyapi.khulnasoft.com/img/sponsors/speakeasy.png"></a>
-<a href="https://www.svix.com/" target="_blank" title="Svix - Webhooks as a service"><img src="https://readyapi.khulnasoft.com/img/sponsors/svix.svg"></a>
-<a href="https://www.codacy.com/?utm_source=github&utm_medium=sponsors&utm_id=pioneers" target="_blank" title="Take code reviews from hours to minutes"><img src="https://readyapi.khulnasoft.com/img/sponsors/codacy.png"></a>
+{% if sponsors %}
+{% for sponsor in sponsors.gold -%}
+<a href="{{ sponsor.url }}" target="_blank" title="{{ sponsor.title }}"><img src="{{ sponsor.img }}" style="border-radius:15px"></a>
+{% endfor -%}
+{%- for sponsor in sponsors.silver -%}
+<a href="{{ sponsor.url }}" target="_blank" title="{{ sponsor.title }}"><img src="{{ sponsor.img }}" style="border-radius:15px"></a>
+{% endfor %}
+{% endif %}
 
 <!-- /sponsors -->
 
 <a href="https://readyapi.khulnasoft.com/readyapi-people/#sponsors" class="external-link" target="_blank">Other sponsors</a>
 
 ## Opinions
 
@@ -117,16 +171,14 @@
 
 If you are building a <abbr title="Command Line Interface">CLI</abbr> app to be used in the terminal instead of a web API, check out <a href="https://typer.tiangolo.com/" class="external-link" target="_blank">**Typer**</a>.
 
 **Typer** is ReadyAPI's little sibling. And it's intended to be the **ReadyAPI of CLIs**. ⌨️ 🚀
 
 ## Requirements
 
-Python 3.8+
-
 ReadyAPI stands on the shoulders of giants:
 
 * <a href="https://www.starlette.io/" class="external-link" target="_blank">Starlette</a> for the web parts.
 * <a href="https://docs.pydantic.dev/" class="external-link" target="_blank">Pydantic</a> for the data parts.
 
 ## Installation
 
@@ -136,26 +188,14 @@
 $ pip install readyapi
 
 ---> 100%
 ```
 
 </div>
 
-You will also need an ASGI server, for production such as <a href="https://www.uvicorn.org" class="external-link" target="_blank">Uvicorn</a> or <a href="https://github.com/pgjones/hypercorn" class="external-link" target="_blank">Hypercorn</a>.
-
-<div class="termy">
-
-```console
-$ pip install "uvicorn[standard]"
-
----> 100%
-```
-
-</div>
-
 ## Example
 
 ### Create it
 
 * Create a file `main.py` with:
 
 ```Python
@@ -208,33 +248,46 @@
 ### Run it
 
 Run the server with:
 
 <div class="termy">
 
 ```console
-$ uvicorn main:app --reload
+$ readyapi dev main.py
 
+ ╭────────── ReadyAPI CLI - Development mode ───────────╮
+ │                                                     │
+ │  Serving at: http://127.0.0.1:8000                  │
+ │                                                     │
+ │  API docs: http://127.0.0.1:8000/docs               │
+ │                                                     │
+ │  Running in development mode, for production use:   │
+ │                                                     │
+ │  readyapi run                                        │
+ │                                                     │
+ ╰─────────────────────────────────────────────────────╯
+
+INFO:     Will watch for changes in these directories: ['/home/user/code/awesomeapp']
 INFO:     Uvicorn running on http://127.0.0.1:8000 (Press CTRL+C to quit)
-INFO:     Started reloader process [28720]
-INFO:     Started server process [28722]
+INFO:     Started reloader process [2248755] using WatchFiles
+INFO:     Started server process [2248757]
 INFO:     Waiting for application startup.
 INFO:     Application startup complete.
 ```
 
 </div>
 
 <details markdown="1">
-<summary>About the command <code>uvicorn main:app --reload</code>...</summary>
+<summary>About the command <code>readyapi dev main.py</code>...</summary>
+
+The command `readyapi dev` reads your `main.py` file, detects the **ReadyAPI** app in it, and starts a server using <a href="https://www.uvicorn.org" class="external-link" target="_blank">Uvicorn</a>.
 
-The command `uvicorn main:app` refers to:
+By default, `readyapi dev` will start with auto-reload enabled for local development.
 
-* `main`: the file `main.py` (the Python "module").
-* `app`: the object created inside of `main.py` with the line `app = ReadyAPI()`.
-* `--reload`: make the server restart after code changes. Only do this for development.
+You can read more about it in the <a href="https://readyapi.khulnasoft.com/readyapi-cli/" target="_blank">ReadyAPI CLI docs</a>.
 
 </details>
 
 ### Check it
 
 Open your browser at <a href="http://127.0.0.1:8000/items/5?q=somequery" class="external-link" target="_blank">http://127.0.0.1:8000/items/5?q=somequery</a>.
 
@@ -299,15 +352,15 @@
 
 
 @app.put("/items/{item_id}")
 def update_item(item_id: int, item: Item):
     return {"item_name": item.name, "item_id": item_id}
 ```
 
-The server should reload automatically (because you added `--reload` to the `uvicorn` command above).
+The `readyapi dev` server should reload automatically.
 
 ### Interactive API docs upgrade
 
 Now go to <a href="http://127.0.0.1:8000/docs" class="external-link" target="_blank">http://127.0.0.1:8000/docs</a>.
 
 * The interactive API documentation will be automatically updated, including the new body:
 
@@ -333,15 +386,15 @@
 
 In summary, you declare **once** the types of parameters, body, etc. as function parameters.
 
 You do that with standard modern Python types.
 
 You don't have to learn a new syntax, the methods or classes of a specific library, etc.
 
-Just standard **Python 3.8+**.
+Just standard **Python**.
 
 For example, for an `int`:
 
 ```Python
 item_id: int
 ```
 
@@ -443,35 +496,51 @@
 
 ## Performance
 
 Independent TechEmpower benchmarks show **ReadyAPI** applications running under Uvicorn as <a href="https://www.techempower.com/benchmarks/#section=test&runid=7464e520-0dc2-473d-bd34-dbdfd7e85911&hw=ph&test=query&l=zijzen-7" class="external-link" target="_blank">one of the fastest Python frameworks available</a>, only below Starlette and Uvicorn themselves (used internally by ReadyAPI). (*)
 
 To understand more about it, see the section <a href="https://readyapi.khulnasoft.com/benchmarks/" class="internal-link" target="_blank">Benchmarks</a>.
 
-## Optional Dependencies
+## Dependencies
 
 Used by Pydantic:
 
 * <a href="https://github.com/JoshData/python-email-validator" target="_blank"><code>email_validator</code></a> - for email validation.
 * <a href="https://docs.pydantic.dev/latest/usage/pydantic_settings/" target="_blank"><code>pydantic-settings</code></a> - for settings management.
 * <a href="https://docs.pydantic.dev/latest/usage/types/extra_types/extra_types/" target="_blank"><code>pydantic-extra-types</code></a> - for extra types to be used with Pydantic.
 
 Used by Starlette:
 
 * <a href="https://www.python-httpx.org" target="_blank"><code>httpx</code></a> - Required if you want to use the `TestClient`.
 * <a href="https://jinja.palletsprojects.com" target="_blank"><code>jinja2</code></a> - Required if you want to use the default template configuration.
 * <a href="https://github.com/Kludex/python-multipart" target="_blank"><code>python-multipart</code></a> - Required if you want to support form <abbr title="converting the string that comes from an HTTP request into Python data">"parsing"</abbr>, with `request.form()`.
-* <a href="https://pythonhosted.org/itsdangerous/" target="_blank"><code>itsdangerous</code></a> - Required for `SessionMiddleware` support.
-* <a href="https://pyyaml.org/wiki/PyYAMLDocumentation" target="_blank"><code>pyyaml</code></a> - Required for Starlette's `SchemaGenerator` support (you probably don't need it with ReadyAPI).
-* <a href="https://github.com/esnme/ultrajson" target="_blank"><code>ujson</code></a> - Required if you want to use `UJSONResponse`.
 
 Used by ReadyAPI / Starlette:
 
 * <a href="https://www.uvicorn.org" target="_blank"><code>uvicorn</code></a> - for the server that loads and serves your application.
 * <a href="https://github.com/ijl/orjson" target="_blank"><code>orjson</code></a> - Required if you want to use `ORJSONResponse`.
+* <a href="https://github.com/esnme/ultrajson" target="_blank"><code>ujson</code></a> - Required if you want to use `UJSONResponse`.
+* `readyapi-cli` - to provide the `readyapi` command.
+
+When you install `readyapi` it comes these standard dependencies.
+
+## `readyapi-slim`
+
+If you don't want the extra standard optional dependencies, install `readyapi-slim` instead.
+
+When you install with:
+
+```bash
+pip install readyapi
+```
+
+...it includes the same code and dependencies as:
+
+```bash
+pip install "readyapi-slim[standard]"
+```
 
-You can install all of these with `pip install "readyapi[all]"`.
+The standard extra dependencies are the ones mentioned above.
 
-[![HitCount](http://hits.dwyl.com/khulnasoft/readyapi.svg)](http://hits.dwyl.com/khulnasoft/readyapi)
 ## License
 
 This project is licensed under the terms of the MIT license.
```

#### html2text {}

```diff
@@ -1,45 +1,73 @@
+Metadata-Version: 2.1 Name: readyapi Version: 0.111.0.dev1 Summary: ReadyAPI
+framework, high performance, easy to learn, fast to code, ready for production
+Author-Email: KhulnaSoft DevOps
+khulnasoft.com> Classifier: Intended Audience :: Information Technology
+Classifier: Intended Audience :: System Administrators Classifier: Operating
+System :: OS Independent Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python Classifier: Topic :: Internet
+Classifier: Topic :: Software Development :: Libraries :: Application
+Frameworks Classifier: Topic :: Software Development :: Libraries :: Python
+Modules Classifier: Topic :: Software Development :: Libraries Classifier:
+Topic :: Software Development Classifier: Typing :: Typed Classifier:
+Development Status :: 4 - Beta Classifier: Environment :: Web Environment
+Classifier: Framework :: AsyncIO Classifier: Framework :: Pydantic Classifier:
+Framework :: Pydantic :: 1 Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License Classifier: Programming
+Language :: Python :: 3 :: Only Classifier: Programming Language :: Python ::
+3.8 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12 Classifier: Topic ::
+Internet :: WWW/HTTP :: HTTP Servers Classifier: Topic :: Internet :: WWW/HTTP
+Project-URL: Homepage, https://github.com/khulnasoft/readyapi Project-URL:
+Documentation, https://readyapi.khulnasoft.com/ Project-URL: Repository, https:
+//github.com/khulnasoft/readyapi Requires-Python: >=3.8 Requires-Dist:
+starlette<0.38.0,>=0.37.2 Requires-Dist:
+pydantic!=1.8,!=1.8.1,!=2.0.0,!=2.0.1,!=2.1.0,<3.0.0,>=1.7.4 Requires-Dist:
+typing-extensions>=4.8.0 Requires-Dist: readyapi-cli>=0.0.2 Requires-Dist:
+httpx>=0.23.0 Requires-Dist: jinja2>=2.11.2 Requires-Dist: python-
+multipart>=0.0.7 Requires-Dist:
+ujson!=4.0.2,!=4.1.0,!=4.2.0,!=4.3.0,!=5.0.0,!=5.1.0,>=4.0.1 Requires-Dist:
+orjson>=3.2.1 Requires-Dist: email_validator>=2.0.0 Requires-Dist: uvicorn
+[standard]>=0.12.0 Requires-Dist: httpx>=0.23.0; extra == "all" Requires-Dist:
+jinja2>=2.11.2; extra == "all" Requires-Dist: python-multipart>=0.0.7; extra ==
+"all" Requires-Dist: itsdangerous>=1.1.0; extra == "all" Requires-Dist:
+pyyaml>=5.3.1; extra == "all" Requires-Dist:
+ujson!=4.0.2,!=4.1.0,!=4.2.0,!=4.3.0,!=5.0.0,!=5.1.0,>=4.0.1; extra == "all"
+Requires-Dist: orjson>=3.2.1; extra == "all" Requires-Dist:
+email_validator>=2.0.0; extra == "all" Requires-Dist: uvicorn
+[standard]>=0.12.0; extra == "all" Requires-Dist: pydantic-settings>=2.0.0;
+extra == "all" Requires-Dist: pydantic-extra-types>=2.0.0; extra == "all"
+Provides-Extra: all Description-Content-Type: text/markdown
                                   _[_R_e_a_d_y_A_P_I_]
  RReeaaddyyAAPPII ffrraammeewwoorrkk,, hhiigghh ppeerrffoorrmmaannccee,, eeaassyy ttoo lleeaarrnn,, ffaasstt ttoo ccooddee,, rreeaaddyy ffoorr
                                   pprroodduuccttiioonn
          _[_T_e_s_t_]_[_C_o_v_e_r_a_g_e_]_[_P_a_c_k_a_g_e_ _v_e_r_s_i_o_n_]_[_S_u_p_p_o_r_t_e_d_ _P_y_t_h_o_n_ _v_e_r_s_i_o_n_s_]
 --- **Documentation**: _h_t_t_p_s_:_/_/_r_e_a_d_y_a_p_i_._k_h_u_l_n_a_s_o_f_t_._c_o_m **Source Code**: _h_t_t_p_s_:_/
 _/_g_i_t_h_u_b_._c_o_m_/_k_h_u_l_n_a_s_o_f_t_/_r_e_a_d_y_a_p_i --- ReadyAPI is a modern, fast (high-
-performance), web framework for building APIs with Python 3.8+ based on
-standard Python type hints. The key features are: * **Fast**: Very high
-performance, on par with **NodeJS** and **Go** (thanks to Starlette and
-Pydantic). [One of the fastest Python frameworks available](#performance). *
-**Fast to code**: Increase the speed to develop features by about 200% to 300%.
-* * **Fewer bugs**: Reduce about 40% of human (developer) induced errors. * *
+performance), web framework for building APIs with Python based on standard
+Python type hints. The key features are: * **Fast**: Very high performance, on
+par with **NodeJS** and **Go** (thanks to Starlette and Pydantic). [One of the
+fastest Python frameworks available](#performance). * **Fast to code**:
+Increase the speed to develop features by about 200% to 300%. * * **Fewer
+bugs**: Reduce about 40% of human (developer) induced errors. * *
 **Intuitive**: Great editor support. Completion everywhere. Less time
 debugging. * **Easy**: Designed to be easy to use and learn. Less time reading
 docs. * **Short**: Minimize code duplication. Multiple features from each
 parameter declaration. Fewer bugs. * **Robust**: Get production-ready code.
 With automatic interactive documentation. * **Standards-based**: Based on (and
 fully compatible with) the open standards for APIs: _O_p_e_n_A_P_I (previously known
 as Swagger) and _J_S_O_N_ _S_c_h_e_m_a. * estimation based on tests on an internal
-development team, building production applications. ## Sponsors _[_h_t_t_p_s_:_/_/
-_r_e_a_d_y_a_p_i_._k_h_u_l_n_a_s_o_f_t_._c_o_m_/_i_m_g_/_s_p_o_n_s_o_r_s_/_c_r_y_p_t_a_p_i_._s_v_g_]_[_h_t_t_p_s_:_/_/
-_r_e_a_d_y_a_p_i_._k_h_u_l_n_a_s_o_f_t_._c_o_m_/_i_m_g_/_s_p_o_n_s_o_r_s_/_p_l_a_t_f_o_r_m_-_s_h_._p_n_g_]_[_h_t_t_p_s_:_/_/
-_r_e_a_d_y_a_p_i_._k_h_u_l_n_a_s_o_f_t_._c_o_m_/_i_m_g_/_s_p_o_n_s_o_r_s_/_p_o_r_t_e_r_._p_n_g_]_[_h_t_t_p_s_:_/_/
-_r_e_a_d_y_a_p_i_._k_h_u_l_n_a_s_o_f_t_._c_o_m_/_i_m_g_/_s_p_o_n_s_o_r_s_/_b_u_m_p_-_s_h_._s_v_g_]_[_h_t_t_p_s_:_/_/
-_r_e_a_d_y_a_p_i_._k_h_u_l_n_a_s_o_f_t_._c_o_m_/_i_m_g_/_s_p_o_n_s_o_r_s_/_r_e_f_l_e_x_._p_n_g_]_[_h_t_t_p_s_:_/_/
-_r_e_a_d_y_a_p_i_._k_h_u_l_n_a_s_o_f_t_._c_o_m_/_i_m_g_/_s_p_o_n_s_o_r_s_/_s_c_a_l_a_r_._s_v_g_]_[_h_t_t_p_s_:_/_/
-_r_e_a_d_y_a_p_i_._k_h_u_l_n_a_s_o_f_t_._c_o_m_/_i_m_g_/_s_p_o_n_s_o_r_s_/_p_r_o_p_e_l_a_u_t_h_._p_n_g_]_[_h_t_t_p_s_:_/_/
-_r_e_a_d_y_a_p_i_._k_h_u_l_n_a_s_o_f_t_._c_o_m_/_i_m_g_/_s_p_o_n_s_o_r_s_/_c_o_h_e_r_e_n_c_e_._p_n_g_]_[_h_t_t_p_s_:_/_/
-_r_e_a_d_y_a_p_i_._k_h_u_l_n_a_s_o_f_t_._c_o_m_/_i_m_g_/_s_p_o_n_s_o_r_s_/_m_o_n_g_o_d_b_._p_n_g_]_[_h_t_t_p_s_:_/_/
-_r_e_a_d_y_a_p_i_._k_h_u_l_n_a_s_o_f_t_._c_o_m_/_i_m_g_/_s_p_o_n_s_o_r_s_/_t_a_l_k_p_y_t_h_o_n_-_v_2_._j_p_g_]_[_h_t_t_p_s_:_/_/
-_r_e_a_d_y_a_p_i_._k_h_u_l_n_a_s_o_f_t_._c_o_m_/_i_m_g_/_s_p_o_n_s_o_r_s_/_h_a_y_s_t_a_c_k_-_r_e_a_d_y_a_p_i_._s_v_g_]_[_h_t_t_p_s_:_/_/
-_r_e_a_d_y_a_p_i_._k_h_u_l_n_a_s_o_f_t_._c_o_m_/_i_m_g_/_s_p_o_n_s_o_r_s_/_d_a_t_a_b_e_n_t_o_._s_v_g_]_[_h_t_t_p_s_:_/_/
-_r_e_a_d_y_a_p_i_._k_h_u_l_n_a_s_o_f_t_._c_o_m_/_i_m_g_/_s_p_o_n_s_o_r_s_/_s_p_e_a_k_e_a_s_y_._p_n_g_]_[_h_t_t_p_s_:_/_/
-_r_e_a_d_y_a_p_i_._k_h_u_l_n_a_s_o_f_t_._c_o_m_/_i_m_g_/_s_p_o_n_s_o_r_s_/_s_v_i_x_._s_v_g_]_[_h_t_t_p_s_:_/_/_r_e_a_d_y_a_p_i_._k_h_u_l_n_a_s_o_f_t_._c_o_m_/
-_i_m_g_/_s_p_o_n_s_o_r_s_/_c_o_d_a_c_y_._p_n_g_]_O_t_h_e_r_ _s_p_o_n_s_o_r_s ## Opinions "_[...] I'm using
-**ReadyAPI** a ton these days. [...] I'm actually planning to use it for all of
-my team's **ML services at Microsoft**. Some of them are getting integrated
-into the core **Windows** product and some **Office** products._"
+development team, building production applications. ## Sponsors {% if sponsors
+%} {% for sponsor in sponsors.gold -%} _[_{_{_ _s_p_o_n_s_o_r_._i_m_g_ _}_}_]{% endfor -%} {%- for
+sponsor in sponsors.silver -%} _[_{_{_ _s_p_o_n_s_o_r_._i_m_g_ _}_}_]{% endfor %} {% endif %}
+_O_t_h_e_r_ _s_p_o_n_s_o_r_s ## Opinions "_[...] I'm using **ReadyAPI** a ton these days.
+[...] I'm actually planning to use it for all of my team's **ML services at
+Microsoft**. Some of them are getting integrated into the core **Windows**
+product and some **Office** products._"
 Kabir Khan - MMiiccrroossoofftt _(_r_e_f_)
 --- "_We adopted the **ReadyAPI** library to spawn a **REST** server that can
 be queried to obtain **predictions**. [for Ludwig]_"
 Piero Molino, Yaroslav Dudin, and Sai Sumanth Miryala - UUbbeerr _(_r_e_f_)
 --- "_**Netflix** is pleased to announce the open-source release of our
 **crisis management** orchestration framework: **Dispatch**! [built with
 **ReadyAPI**]_"
@@ -62,61 +90,65 @@
 development strategy and is driving many automations and services such as our
 Virtual TAC Engineer._"
 Deon Pillsbury - CCiissccoo _(_r_e_f_)
 --- ## **Typer**, the ReadyAPI of CLIs _[_h_t_t_p_s_:_/_/_t_y_p_e_r_._t_i_a_n_g_o_l_o_._c_o_m_/_i_m_g_/_l_o_g_o_-
 _m_a_r_g_i_n_/_l_o_g_o_-_m_a_r_g_i_n_-_v_e_c_t_o_r_._s_v_g_]If you are building a CLI app to be used in the
 terminal instead of a web API, check out _*_*_T_y_p_e_r_*_*. **Typer** is ReadyAPI's
 little sibling. And it's intended to be the **ReadyAPI of CLIs**. â¨ï¸ ð
-## Requirements Python 3.8+ ReadyAPI stands on the shoulders of giants: *
-_S_t_a_r_l_e_t_t_e for the web parts. * _P_y_d_a_n_t_i_c for the data parts. ## Installation
+## Requirements ReadyAPI stands on the shoulders of giants: * _S_t_a_r_l_e_t_t_e for the
+web parts. * _P_y_d_a_n_t_i_c for the data parts. ## Installation
 ```console $ pip install readyapi ---> 100% ```
-You will also need an ASGI server, for production such as _U_v_i_c_o_r_n or _H_y_p_e_r_c_o_r_n.
-```console $ pip install "uvicorn[standard]" ---> 100% ```
 ## Example ### Create it * Create a file `main.py` with: ```Python from typing
 import Union from readyapi import ReadyAPI app = ReadyAPI() @app.get("/") def
 read_root(): return {"Hello": "World"} @app.get("/items/{item_id}") def
 read_item(item_id: int, q: Union[str, None] = None): return {"item_id":
 item_id, "q": q} ``` Or use async def... If your code uses `async` / `await`,
 use `async def`: ```Python hl_lines="9 14" from typing import Union from
 readyapi import ReadyAPI app = ReadyAPI() @app.get("/") async def read_root():
 return {"Hello": "World"} @app.get("/items/{item_id}") async def read_item
 (item_id: int, q: Union[str, None] = None): return {"item_id": item_id, "q": q}
 ``` **Note**: If you don't know, check the _"In a hurry?"_ section about
 _`_a_s_y_n_c_`_ _a_n_d_ _`_a_w_a_i_t_`_ _i_n_ _t_h_e_ _d_o_c_s. ### Run it Run the server with:
-```console $ uvicorn main:app --reload INFO: Uvicorn running on http://
-127.0.0.1:8000 (Press CTRL+C to quit) INFO: Started reloader process [28720]
-INFO: Started server process [28722] INFO: Waiting for application startup.
-INFO: Application startup complete. ```
-About the command uvicorn main:app --reload... The command `uvicorn main:app`
-refers to: * `main`: the file `main.py` (the Python "module"). * `app`: the
-object created inside of `main.py` with the line `app = ReadyAPI()`. * `--
-reload`: make the server restart after code changes. Only do this for
-development. ### Check it Open your browser at _h_t_t_p_:_/_/_1_2_7_._0_._0_._1_:_8_0_0_0_/_i_t_e_m_s_/
-_5_?_q_=_s_o_m_e_q_u_e_r_y. You will see the JSON response as: ```JSON {"item_id": 5, "q":
-"somequery"} ``` You already created an API that: * Receives HTTP requests in
-the _paths_ `/` and `/items/{item_id}`. * Both _paths_ take `GET` ooppeerraattiioonnss
-(also known as HTTP _methods_). * The _path_ `/items/{item_id}` has a _path
-parameter_ `item_id` that should be an `int`. * The _path_ `/items/{item_id}`
-has an optional `str` _query parameter_ `q`. ### Interactive API docs Now go to
-_h_t_t_p_:_/_/_1_2_7_._0_._0_._1_:_8_0_0_0_/_d_o_c_s. You will see the automatic interactive API
-documentation (provided by _S_w_a_g_g_e_r_ _U_I): ![Swagger UI](https://
-readyapi.khulnasoft.com/img/index/index-01-swagger-ui-simple.png) ###
-Alternative API docs And now, go to _h_t_t_p_:_/_/_1_2_7_._0_._0_._1_:_8_0_0_0_/_r_e_d_o_c. You will see
-the alternative automatic documentation (provided by _R_e_D_o_c): ![ReDoc](https://
-readyapi.khulnasoft.com/img/index/index-02-redoc-simple.png) ## Example upgrade
-Now modify the file `main.py` to receive a body from a `PUT` request. Declare
-the body using standard Python types, thanks to Pydantic. ```Python hl_lines="4
-9-12 25-27" from typing import Union from readyapi import ReadyAPI from
-pydantic import BaseModel app = ReadyAPI() class Item(BaseModel): name: str
-price: float is_offer: Union[bool, None] = None @app.get("/") def read_root():
-return {"Hello": "World"} @app.get("/items/{item_id}") def read_item(item_id:
-int, q: Union[str, None] = None): return {"item_id": item_id, "q": q} @app.put
-("/items/{item_id}") def update_item(item_id: int, item: Item): return
-{"item_name": item.name, "item_id": item_id} ``` The server should reload
-automatically (because you added `--reload` to the `uvicorn` command above).
+```console $ readyapi dev main.py â­ââââââââââ ReadyAPI
+CLI - Development mode ââââââââââââ® â â â Serving
+at: http://127.0.0.1:8000 â â â â API docs: http://127.0.0.1:8000/docs
+â â â â Running in development mode, for production use: â â â
+â readyapi run â â â
+â°ââââââââââââââââââââââââââââââââââââââââââââââââââââââ¯
+INFO: Will watch for changes in these directories: ['/home/user/code/
+awesomeapp'] INFO: Uvicorn running on http://127.0.0.1:8000 (Press CTRL+C to
+quit) INFO: Started reloader process [2248755] using WatchFiles INFO: Started
+server process [2248757] INFO: Waiting for application startup. INFO:
+Application startup complete. ```
+About the command readyapi dev main.py... The command `readyapi dev` reads your
+`main.py` file, detects the **ReadyAPI** app in it, and starts a server using
+_U_v_i_c_o_r_n. By default, `readyapi dev` will start with auto-reload enabled for
+local development. You can read more about it in the _R_e_a_d_y_A_P_I_ _C_L_I_ _d_o_c_s. ###
+Check it Open your browser at _h_t_t_p_:_/_/_1_2_7_._0_._0_._1_:_8_0_0_0_/_i_t_e_m_s_/_5_?_q_=_s_o_m_e_q_u_e_r_y. You
+will see the JSON response as: ```JSON {"item_id": 5, "q": "somequery"} ``` You
+already created an API that: * Receives HTTP requests in the _paths_ `/` and `/
+items/{item_id}`. * Both _paths_ take `GET` ooppeerraattiioonnss (also known as HTTP
+_methods_). * The _path_ `/items/{item_id}` has a _path parameter_ `item_id`
+that should be an `int`. * The _path_ `/items/{item_id}` has an optional `str`
+_query parameter_ `q`. ### Interactive API docs Now go to _h_t_t_p_:_/_/_1_2_7_._0_._0_._1_:
+_8_0_0_0_/_d_o_c_s. You will see the automatic interactive API documentation (provided
+by _S_w_a_g_g_e_r_ _U_I): ![Swagger UI](https://readyapi.khulnasoft.com/img/index/index-
+01-swagger-ui-simple.png) ### Alternative API docs And now, go to _h_t_t_p_:_/_/
+_1_2_7_._0_._0_._1_:_8_0_0_0_/_r_e_d_o_c. You will see the alternative automatic documentation
+(provided by _R_e_D_o_c): ![ReDoc](https://readyapi.khulnasoft.com/img/index/index-
+02-redoc-simple.png) ## Example upgrade Now modify the file `main.py` to
+receive a body from a `PUT` request. Declare the body using standard Python
+types, thanks to Pydantic. ```Python hl_lines="4 9-12 25-27" from typing import
+Union from readyapi import ReadyAPI from pydantic import BaseModel app =
+ReadyAPI() class Item(BaseModel): name: str price: float is_offer: Union[bool,
+None] = None @app.get("/") def read_root(): return {"Hello": "World"} @app.get
+("/items/{item_id}") def read_item(item_id: int, q: Union[str, None] = None):
+return {"item_id": item_id, "q": q} @app.put("/items/{item_id}") def
+update_item(item_id: int, item: Item): return {"item_name": item.name,
+"item_id": item_id} ``` The `readyapi dev` server should reload automatically.
 ### Interactive API docs upgrade Now go to _h_t_t_p_:_/_/_1_2_7_._0_._0_._1_:_8_0_0_0_/_d_o_c_s. * The
 interactive API documentation will be automatically updated, including the new
 body: ![Swagger UI](https://readyapi.khulnasoft.com/img/index/index-03-swagger-
 02.png) * Click on the button "Try it out", it allows you to fill the
 parameters and directly interact with the API: ![Swagger UI interaction](https:
 //readyapi.khulnasoft.com/img/index/index-04-swagger-03.png) * Then click on
 the "Execute" button, the user interface will communicate with your API, send
@@ -124,17 +156,17 @@
 interaction](https://readyapi.khulnasoft.com/img/index/index-05-swagger-04.png)
 ### Alternative API docs upgrade And now, go to _h_t_t_p_:_/_/_1_2_7_._0_._0_._1_:_8_0_0_0_/_r_e_d_o_c. *
 The alternative documentation will also reflect the new query parameter and
 body: ![ReDoc](https://readyapi.khulnasoft.com/img/index/index-06-redoc-02.png)
 ### Recap In summary, you declare **once** the types of parameters, body, etc.
 as function parameters. You do that with standard modern Python types. You
 don't have to learn a new syntax, the methods or classes of a specific library,
-etc. Just standard **Python 3.8+**. For example, for an `int`: ```Python
-item_id: int ``` or for a more complex `Item` model: ```Python item: Item ```
-...and with that single declaration you get: * Editor support, including: *
+etc. Just standard **Python**. For example, for an `int`: ```Python item_id:
+int ``` or for a more complex `Item` model: ```Python item: Item ``` ...and
+with that single declaration you get: * Editor support, including: *
 Completion. * Type checks. * Validation of data: * Automatic and clear errors
 when the data is invalid. * Validation even for deeply nested JSON objects. *
 Conversion of input data: coming from the network to Python data and types.
 Reading from: * JSON. * Path parameters. * Query parameters. * Cookies. *
 Headers. * Forms. * Files. * Conversion of output data: converting from Python
 data and types to network data (as JSON): * Convert Python types (`str`, `int`,
 `float`, `bool`, `list`, etc). * `datetime` objects. * `UUID` objects. *
@@ -172,21 +204,22 @@
 Pydantic). * **GraphQL** integration with _S_t_r_a_w_b_e_r_r_y and other libraries. *
 Many extra features (thanks to Starlette) as: * **WebSockets** * extremely easy
 tests based on HTTPX and `pytest` * **CORS** * **Cookie Sessions** * ...and
 more. ## Performance Independent TechEmpower benchmarks show **ReadyAPI**
 applications running under Uvicorn as _o_n_e_ _o_f_ _t_h_e_ _f_a_s_t_e_s_t_ _P_y_t_h_o_n_ _f_r_a_m_e_w_o_r_k_s
 _a_v_a_i_l_a_b_l_e, only below Starlette and Uvicorn themselves (used internally by
 ReadyAPI). (*) To understand more about it, see the section _B_e_n_c_h_m_a_r_k_s. ##
-Optional Dependencies Used by Pydantic: * _e_m_a_i_l___v_a_l_i_d_a_t_o_r - for email
-validation. * _p_y_d_a_n_t_i_c_-_s_e_t_t_i_n_g_s - for settings management. * _p_y_d_a_n_t_i_c_-_e_x_t_r_a_-
-_t_y_p_e_s - for extra types to be used with Pydantic. Used by Starlette: * _h_t_t_p_x -
-Required if you want to use the `TestClient`. * _j_i_n_j_a_2 - Required if you want
-to use the default template configuration. * _p_y_t_h_o_n_-_m_u_l_t_i_p_a_r_t - Required if you
-want to support form "parsing", with `request.form()`. * _i_t_s_d_a_n_g_e_r_o_u_s -
-Required for `SessionMiddleware` support. * _p_y_y_a_m_l - Required for Starlette's
-`SchemaGenerator` support (you probably don't need it with ReadyAPI). * _u_j_s_o_n -
-Required if you want to use `UJSONResponse`. Used by ReadyAPI / Starlette: *
+Dependencies Used by Pydantic: * _e_m_a_i_l___v_a_l_i_d_a_t_o_r - for email validation. *
+_p_y_d_a_n_t_i_c_-_s_e_t_t_i_n_g_s - for settings management. * _p_y_d_a_n_t_i_c_-_e_x_t_r_a_-_t_y_p_e_s - for extra
+types to be used with Pydantic. Used by Starlette: * _h_t_t_p_x - Required if you
+want to use the `TestClient`. * _j_i_n_j_a_2 - Required if you want to use the
+default template configuration. * _p_y_t_h_o_n_-_m_u_l_t_i_p_a_r_t - Required if you want to
+support form "parsing", with `request.form()`. Used by ReadyAPI / Starlette: *
 _u_v_i_c_o_r_n - for the server that loads and serves your application. * _o_r_j_s_o_n -
-Required if you want to use `ORJSONResponse`. You can install all of these with
-`pip install "readyapi[all]"`. [![HitCount](http://hits.dwyl.com/khulnasoft/
-readyapi.svg)](http://hits.dwyl.com/khulnasoft/readyapi) ## License This
-project is licensed under the terms of the MIT license.
+Required if you want to use `ORJSONResponse`. * _u_j_s_o_n - Required if you want to
+use `UJSONResponse`. * `readyapi-cli` - to provide the `readyapi` command. When
+you install `readyapi` it comes these standard dependencies. ## `readyapi-slim`
+If you don't want the extra standard optional dependencies, install `readyapi-
+slim` instead. When you install with: ```bash pip install readyapi ``` ...it
+includes the same code and dependencies as: ```bash pip install "readyapi-slim
+[standard]" ``` The standard extra dependencies are the ones mentioned above.
+## License This project is licensed under the terms of the MIT license.
```

### Comparing `readyapi-0.110.3/docs/en/docs/img/favicon.png` & `readyapi-0.111.0.dev1/docs/en/docs/img/favicon.png`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/additional_responses/tutorial002.py` & `readyapi-0.111.0.dev1/docs_src/additional_responses/tutorial002.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/additional_responses/tutorial003.py` & `readyapi-0.111.0.dev1/docs_src/additional_responses/tutorial003.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/additional_responses/tutorial004.py` & `readyapi-0.111.0.dev1/docs_src/additional_responses/tutorial004.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/additional_status_codes/tutorial001.py` & `readyapi-0.111.0.dev1/docs_src/additional_status_codes/tutorial001.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/additional_status_codes/tutorial001_an.py` & `readyapi-0.111.0.dev1/docs_src/additional_status_codes/tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/additional_status_codes/tutorial001_an_py310.py` & `readyapi-0.111.0.dev1/docs_src/additional_status_codes/tutorial001_an_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/additional_status_codes/tutorial001_an_py39.py` & `readyapi-0.111.0.dev1/docs_src/additional_status_codes/tutorial001_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/additional_status_codes/tutorial001_py310.py` & `readyapi-0.111.0.dev1/docs_src/additional_status_codes/tutorial001_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/app_testing/app_b/main.py` & `readyapi-0.111.0.dev1/docs_src/app_testing/app_b/main.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/app_testing/app_b/test_main.py` & `readyapi-0.111.0.dev1/docs_src/app_testing/app_b/test_main.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/app_testing/app_b_an/main.py` & `readyapi-0.111.0.dev1/docs_src/app_testing/app_b_an/main.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/app_testing/app_b_an/test_main.py` & `readyapi-0.111.0.dev1/docs_src/app_testing/app_b_an/test_main.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/app_testing/app_b_an_py310/main.py` & `readyapi-0.111.0.dev1/docs_src/app_testing/app_b_an_py310/main.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/app_testing/app_b_an_py310/test_main.py` & `readyapi-0.111.0.dev1/docs_src/app_testing/app_b_an_py310/test_main.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/app_testing/app_b_an_py39/main.py` & `readyapi-0.111.0.dev1/docs_src/app_testing/app_b_an_py39/main.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/app_testing/app_b_an_py39/test_main.py` & `readyapi-0.111.0.dev1/docs_src/app_testing/app_b_an_py39/test_main.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/app_testing/app_b_py310/main.py` & `readyapi-0.111.0.dev1/docs_src/app_testing/app_b_py310/main.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/app_testing/app_b_py310/test_main.py` & `readyapi-0.111.0.dev1/docs_src/app_testing/app_b_py310/test_main.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/app_testing/tutorial002.py` & `readyapi-0.111.0.dev1/docs_src/app_testing/tutorial002.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/app_testing/tutorial003.py` & `readyapi-0.111.0.dev1/docs_src/app_testing/tutorial003.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/async_sql_databases/tutorial001.py` & `readyapi-0.111.0.dev1/docs_src/async_sql_databases/tutorial001.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/background_tasks/tutorial001.py` & `readyapi-0.111.0.dev1/docs_src/background_tasks/tutorial001.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/background_tasks/tutorial002.py` & `readyapi-0.111.0.dev1/docs_src/background_tasks/tutorial002.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/background_tasks/tutorial002_an.py` & `readyapi-0.111.0.dev1/docs_src/background_tasks/tutorial002_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/background_tasks/tutorial002_an_py310.py` & `readyapi-0.111.0.dev1/docs_src/background_tasks/tutorial002_an_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/background_tasks/tutorial002_an_py39.py` & `readyapi-0.111.0.dev1/docs_src/background_tasks/tutorial002_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/background_tasks/tutorial002_py310.py` & `readyapi-0.111.0.dev1/docs_src/background_tasks/tutorial002_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/bigger_applications/app/main.py` & `readyapi-0.111.0.dev1/docs_src/bigger_applications/app/main.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/bigger_applications/app/routers/items.py` & `readyapi-0.111.0.dev1/docs_src/bigger_applications/app/routers/items.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/bigger_applications/app_an/main.py` & `readyapi-0.111.0.dev1/docs_src/bigger_applications/app_an/main.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/bigger_applications/app_an/routers/items.py` & `readyapi-0.111.0.dev1/docs_src/bigger_applications/app_an/routers/items.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/bigger_applications/app_an_py39/main.py` & `readyapi-0.111.0.dev1/docs_src/bigger_applications/app_an_py39/main.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/bigger_applications/app_an_py39/routers/items.py` & `readyapi-0.111.0.dev1/docs_src/bigger_applications/app_an_py39/routers/items.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/body_fields/tutorial001.py` & `readyapi-0.111.0.dev1/docs_src/body_fields/tutorial001.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/body_fields/tutorial001_an.py` & `readyapi-0.111.0.dev1/docs_src/body_fields/tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/body_fields/tutorial001_an_py310.py` & `readyapi-0.111.0.dev1/docs_src/body_fields/tutorial001_an_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/body_fields/tutorial001_an_py39.py` & `readyapi-0.111.0.dev1/docs_src/body_fields/tutorial001_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/body_fields/tutorial001_py310.py` & `readyapi-0.111.0.dev1/docs_src/body_fields/tutorial001_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/body_multiple_params/tutorial001.py` & `readyapi-0.111.0.dev1/docs_src/body_multiple_params/tutorial001.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/body_multiple_params/tutorial001_an.py` & `readyapi-0.111.0.dev1/docs_src/body_multiple_params/tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/body_multiple_params/tutorial001_an_py310.py` & `readyapi-0.111.0.dev1/docs_src/body_multiple_params/tutorial001_an_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/body_multiple_params/tutorial001_an_py39.py` & `readyapi-0.111.0.dev1/docs_src/body_multiple_params/tutorial001_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/body_multiple_params/tutorial001_py310.py` & `readyapi-0.111.0.dev1/docs_src/body_multiple_params/tutorial001_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/body_multiple_params/tutorial003.py` & `readyapi-0.111.0.dev1/docs_src/body_multiple_params/tutorial003.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/body_multiple_params/tutorial003_an.py` & `readyapi-0.111.0.dev1/docs_src/body_multiple_params/tutorial003_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/body_multiple_params/tutorial003_an_py310.py` & `readyapi-0.111.0.dev1/docs_src/body_multiple_params/tutorial003_an_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/body_multiple_params/tutorial003_an_py39.py` & `readyapi-0.111.0.dev1/docs_src/body_multiple_params/tutorial003_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/body_multiple_params/tutorial004.py` & `readyapi-0.111.0.dev1/docs_src/body_multiple_params/tutorial004.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/body_multiple_params/tutorial004_an.py` & `readyapi-0.111.0.dev1/docs_src/body_multiple_params/tutorial004_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/body_multiple_params/tutorial004_an_py310.py` & `readyapi-0.111.0.dev1/docs_src/body_multiple_params/tutorial004_an_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/body_multiple_params/tutorial004_an_py39.py` & `readyapi-0.111.0.dev1/docs_src/body_multiple_params/tutorial004_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/body_multiple_params/tutorial004_py310.py` & `readyapi-0.111.0.dev1/docs_src/body_multiple_params/tutorial004_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/body_nested_models/tutorial005.py` & `readyapi-0.111.0.dev1/docs_src/body_nested_models/tutorial005.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/body_nested_models/tutorial005_py39.py` & `readyapi-0.111.0.dev1/docs_src/body_nested_models/tutorial005_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/body_nested_models/tutorial006.py` & `readyapi-0.111.0.dev1/docs_src/body_nested_models/tutorial006.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/body_nested_models/tutorial006_py39.py` & `readyapi-0.111.0.dev1/docs_src/body_nested_models/tutorial006_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/body_nested_models/tutorial007.py` & `readyapi-0.111.0.dev1/docs_src/body_nested_models/tutorial007.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/body_nested_models/tutorial007_py310.py` & `readyapi-0.111.0.dev1/docs_src/body_nested_models/tutorial007_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/body_nested_models/tutorial007_py39.py` & `readyapi-0.111.0.dev1/docs_src/body_nested_models/tutorial007_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/body_updates/tutorial001.py` & `readyapi-0.111.0.dev1/docs_src/body_updates/tutorial001.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/body_updates/tutorial001_py310.py` & `readyapi-0.111.0.dev1/docs_src/body_updates/tutorial001_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/body_updates/tutorial001_py39.py` & `readyapi-0.111.0.dev1/docs_src/body_updates/tutorial001_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/body_updates/tutorial002.py` & `readyapi-0.111.0.dev1/docs_src/body_updates/tutorial002.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/body_updates/tutorial002_py310.py` & `readyapi-0.111.0.dev1/docs_src/body_updates/tutorial002_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/body_updates/tutorial002_py39.py` & `readyapi-0.111.0.dev1/docs_src/body_updates/tutorial002_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/custom_docs_ui/tutorial001.py` & `readyapi-0.111.0.dev1/docs_src/custom_docs_ui/tutorial001.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/custom_docs_ui/tutorial002.py` & `readyapi-0.111.0.dev1/docs_src/custom_docs_ui/tutorial002.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/custom_request_and_route/tutorial001.py` & `readyapi-0.111.0.dev1/docs_src/custom_request_and_route/tutorial001.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/custom_request_and_route/tutorial002.py` & `readyapi-0.111.0.dev1/docs_src/custom_request_and_route/tutorial002.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/custom_request_and_route/tutorial003.py` & `readyapi-0.111.0.dev1/docs_src/custom_request_and_route/tutorial003.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/dataclasses/tutorial002.py` & `readyapi-0.111.0.dev1/docs_src/dataclasses/tutorial002.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/dataclasses/tutorial003.py` & `readyapi-0.111.0.dev1/docs_src/dataclasses/tutorial003.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/dependencies/tutorial002.py` & `readyapi-0.111.0.dev1/docs_src/dependencies/tutorial002.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/dependencies/tutorial002_an.py` & `readyapi-0.111.0.dev1/docs_src/dependencies/tutorial002_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/dependencies/tutorial002_an_py310.py` & `readyapi-0.111.0.dev1/docs_src/dependencies/tutorial002_an_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/dependencies/tutorial002_an_py39.py` & `readyapi-0.111.0.dev1/docs_src/dependencies/tutorial002_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/dependencies/tutorial002_py310.py` & `readyapi-0.111.0.dev1/docs_src/dependencies/tutorial002_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/dependencies/tutorial003.py` & `readyapi-0.111.0.dev1/docs_src/dependencies/tutorial003.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/dependencies/tutorial003_an.py` & `readyapi-0.111.0.dev1/docs_src/dependencies/tutorial003_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/dependencies/tutorial003_an_py310.py` & `readyapi-0.111.0.dev1/docs_src/dependencies/tutorial003_an_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/dependencies/tutorial003_an_py39.py` & `readyapi-0.111.0.dev1/docs_src/dependencies/tutorial003_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/dependencies/tutorial003_py310.py` & `readyapi-0.111.0.dev1/docs_src/dependencies/tutorial003_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/dependencies/tutorial004.py` & `readyapi-0.111.0.dev1/docs_src/dependencies/tutorial004.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/dependencies/tutorial004_an.py` & `readyapi-0.111.0.dev1/docs_src/dependencies/tutorial004_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/dependencies/tutorial004_an_py310.py` & `readyapi-0.111.0.dev1/docs_src/dependencies/tutorial004_an_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/dependencies/tutorial004_an_py39.py` & `readyapi-0.111.0.dev1/docs_src/dependencies/tutorial004_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/dependencies/tutorial004_py310.py` & `readyapi-0.111.0.dev1/docs_src/dependencies/tutorial004_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/dependencies/tutorial005_an.py` & `readyapi-0.111.0.dev1/docs_src/dependencies/tutorial005_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/dependencies/tutorial005_an_py310.py` & `readyapi-0.111.0.dev1/docs_src/dependencies/tutorial005_an_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/dependencies/tutorial005_an_py39.py` & `readyapi-0.111.0.dev1/docs_src/dependencies/tutorial005_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/dependencies/tutorial006.py` & `readyapi-0.111.0.dev1/docs_src/dependencies/tutorial006.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/dependencies/tutorial006_an.py` & `readyapi-0.111.0.dev1/docs_src/dependencies/tutorial006_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/dependencies/tutorial006_an_py39.py` & `readyapi-0.111.0.dev1/docs_src/dependencies/tutorial006_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/dependencies/tutorial008_an.py` & `readyapi-0.111.0.dev1/docs_src/dependencies/tutorial008_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/dependencies/tutorial008_an_py39.py` & `readyapi-0.111.0.dev1/docs_src/dependencies/tutorial008_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/dependencies/tutorial008b.py` & `readyapi-0.111.0.dev1/docs_src/dependencies/tutorial008b.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/dependencies/tutorial008b_an.py` & `readyapi-0.111.0.dev1/docs_src/dependencies/tutorial008b_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/dependencies/tutorial008b_an_py39.py` & `readyapi-0.111.0.dev1/docs_src/dependencies/tutorial008b_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/dependencies/tutorial008c.py` & `readyapi-0.111.0.dev1/docs_src/dependencies/tutorial008c.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/dependencies/tutorial008c_an.py` & `readyapi-0.111.0.dev1/docs_src/dependencies/tutorial008c_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/dependencies/tutorial008c_an_py39.py` & `readyapi-0.111.0.dev1/docs_src/dependencies/tutorial008c_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/dependencies/tutorial008d.py` & `readyapi-0.111.0.dev1/docs_src/dependencies/tutorial008d.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/dependencies/tutorial008d_an.py` & `readyapi-0.111.0.dev1/docs_src/dependencies/tutorial008d_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/dependencies/tutorial008d_an_py39.py` & `readyapi-0.111.0.dev1/docs_src/dependencies/tutorial008d_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/dependencies/tutorial011_an.py` & `readyapi-0.111.0.dev1/docs_src/dependencies/tutorial011_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/dependencies/tutorial011_an_py39.py` & `readyapi-0.111.0.dev1/docs_src/dependencies/tutorial011_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/dependencies/tutorial012.py` & `readyapi-0.111.0.dev1/docs_src/dependencies/tutorial012.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/dependencies/tutorial012_an.py` & `readyapi-0.111.0.dev1/docs_src/dependencies/tutorial012_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/dependencies/tutorial012_an_py39.py` & `readyapi-0.111.0.dev1/docs_src/dependencies/tutorial012_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/dependency_testing/tutorial001.py` & `readyapi-0.111.0.dev1/docs_src/dependency_testing/tutorial001.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/dependency_testing/tutorial001_an.py` & `readyapi-0.111.0.dev1/docs_src/dependency_testing/tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/dependency_testing/tutorial001_an_py310.py` & `readyapi-0.111.0.dev1/docs_src/dependency_testing/tutorial001_an_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/dependency_testing/tutorial001_an_py39.py` & `readyapi-0.111.0.dev1/docs_src/dependency_testing/tutorial001_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/dependency_testing/tutorial001_py310.py` & `readyapi-0.111.0.dev1/docs_src/dependency_testing/tutorial001_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/events/tutorial003.py` & `readyapi-0.111.0.dev1/docs_src/events/tutorial003.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/extending_openapi/tutorial001.py` & `readyapi-0.111.0.dev1/docs_src/extending_openapi/tutorial001.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/extra_data_types/tutorial001.py` & `readyapi-0.111.0.dev1/docs_src/extra_data_types/tutorial001.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/extra_data_types/tutorial001_an.py` & `readyapi-0.111.0.dev1/docs_src/extra_data_types/tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/extra_data_types/tutorial001_an_py310.py` & `readyapi-0.111.0.dev1/docs_src/extra_data_types/tutorial001_an_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/extra_data_types/tutorial001_an_py39.py` & `readyapi-0.111.0.dev1/docs_src/extra_data_types/tutorial001_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/extra_data_types/tutorial001_py310.py` & `readyapi-0.111.0.dev1/docs_src/extra_data_types/tutorial001_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/extra_models/tutorial001.py` & `readyapi-0.111.0.dev1/docs_src/extra_models/tutorial001.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/extra_models/tutorial001_py310.py` & `readyapi-0.111.0.dev1/docs_src/extra_models/tutorial001_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/extra_models/tutorial002.py` & `readyapi-0.111.0.dev1/docs_src/extra_models/tutorial002.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/extra_models/tutorial002_py310.py` & `readyapi-0.111.0.dev1/docs_src/extra_models/tutorial002_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/extra_models/tutorial003.py` & `readyapi-0.111.0.dev1/docs_src/extra_models/tutorial003.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/extra_models/tutorial003_py310.py` & `readyapi-0.111.0.dev1/docs_src/extra_models/tutorial003_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/generate_clients/tutorial001.py` & `readyapi-0.111.0.dev1/docs_src/generate_clients/tutorial001.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/generate_clients/tutorial002.py` & `readyapi-0.111.0.dev1/docs_src/generate_clients/tutorial002.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/generate_clients/tutorial002_py39.py` & `readyapi-0.111.0.dev1/docs_src/generate_clients/tutorial002_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/generate_clients/tutorial003.py` & `readyapi-0.111.0.dev1/docs_src/generate_clients/tutorial003.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/generate_clients/tutorial003_py39.py` & `readyapi-0.111.0.dev1/docs_src/generate_clients/tutorial003_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/generate_clients/tutorial004.js` & `readyapi-0.111.0.dev1/docs_src/generate_clients/tutorial004.js`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/handling_errors/tutorial003.py` & `readyapi-0.111.0.dev1/docs_src/handling_errors/tutorial003.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/handling_errors/tutorial004.py` & `readyapi-0.111.0.dev1/docs_src/handling_errors/tutorial004.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/handling_errors/tutorial005.py` & `readyapi-0.111.0.dev1/docs_src/handling_errors/tutorial005.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/handling_errors/tutorial006.py` & `readyapi-0.111.0.dev1/docs_src/handling_errors/tutorial006.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/metadata/tutorial001.py` & `readyapi-0.111.0.dev1/docs_src/metadata/tutorial001.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/metadata/tutorial001_1.py` & `readyapi-0.111.0.dev1/docs_src/metadata/tutorial001_1.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/metadata/tutorial004.py` & `readyapi-0.111.0.dev1/docs_src/metadata/tutorial004.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/nosql_databases/tutorial001.py` & `readyapi-0.111.0.dev1/docs_src/nosql_databases/tutorial001.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/openapi_callbacks/tutorial001.py` & `readyapi-0.111.0.dev1/docs_src/openapi_callbacks/tutorial001.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/openapi_webhooks/tutorial001.py` & `readyapi-0.111.0.dev1/docs_src/openapi_webhooks/tutorial001.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/path_operation_advanced_configuration/tutorial002.py` & `readyapi-0.111.0.dev1/docs_src/path_operation_advanced_configuration/tutorial002.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/path_operation_advanced_configuration/tutorial004.py` & `readyapi-0.111.0.dev1/docs_src/path_operation_advanced_configuration/tutorial004.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/path_operation_advanced_configuration/tutorial006.py` & `readyapi-0.111.0.dev1/docs_src/path_operation_advanced_configuration/tutorial006.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/path_operation_advanced_configuration/tutorial007.py` & `readyapi-0.111.0.dev1/docs_src/path_operation_advanced_configuration/tutorial007.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/path_operation_advanced_configuration/tutorial007_pv1.py` & `readyapi-0.111.0.dev1/docs_src/path_operation_advanced_configuration/tutorial007_pv1.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/path_operation_configuration/tutorial002.py` & `readyapi-0.111.0.dev1/docs_src/path_operation_configuration/tutorial002.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/path_operation_configuration/tutorial002_py310.py` & `readyapi-0.111.0.dev1/docs_src/path_operation_configuration/tutorial002_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/path_operation_configuration/tutorial002_py39.py` & `readyapi-0.111.0.dev1/docs_src/path_operation_configuration/tutorial002_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/path_operation_configuration/tutorial003.py` & `readyapi-0.111.0.dev1/docs_src/path_operation_configuration/tutorial003.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/path_operation_configuration/tutorial003_py39.py` & `readyapi-0.111.0.dev1/docs_src/path_operation_configuration/tutorial003_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/path_operation_configuration/tutorial004.py` & `readyapi-0.111.0.dev1/docs_src/path_operation_configuration/tutorial004.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/path_operation_configuration/tutorial004_py310.py` & `readyapi-0.111.0.dev1/docs_src/path_operation_configuration/tutorial004_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/path_operation_configuration/tutorial004_py39.py` & `readyapi-0.111.0.dev1/docs_src/path_operation_configuration/tutorial004_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/path_operation_configuration/tutorial005.py` & `readyapi-0.111.0.dev1/docs_src/path_operation_configuration/tutorial005.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/path_operation_configuration/tutorial005_py310.py` & `readyapi-0.111.0.dev1/docs_src/path_operation_configuration/tutorial005_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/path_operation_configuration/tutorial005_py39.py` & `readyapi-0.111.0.dev1/docs_src/path_operation_configuration/tutorial005_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/path_params/tutorial005.py` & `readyapi-0.111.0.dev1/docs_src/path_params/tutorial005.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/query_params_str_validations/tutorial008_an.py` & `readyapi-0.111.0.dev1/docs_src/query_params_str_validations/tutorial008_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/query_params_str_validations/tutorial008_an_py39.py` & `readyapi-0.111.0.dev1/docs_src/query_params_str_validations/tutorial008_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/query_params_str_validations/tutorial010.py` & `readyapi-0.111.0.dev1/docs_src/query_params_str_validations/tutorial010.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/query_params_str_validations/tutorial010_an.py` & `readyapi-0.111.0.dev1/docs_src/query_params_str_validations/tutorial010_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/query_params_str_validations/tutorial010_an_py310.py` & `readyapi-0.111.0.dev1/docs_src/query_params_str_validations/tutorial010_an_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/query_params_str_validations/tutorial010_an_py39.py` & `readyapi-0.111.0.dev1/docs_src/query_params_str_validations/tutorial010_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/query_params_str_validations/tutorial010_py310.py` & `readyapi-0.111.0.dev1/docs_src/query_params_str_validations/tutorial010_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/request_files/tutorial001_02_an.py` & `readyapi-0.111.0.dev1/docs_src/request_files/tutorial001_02_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/request_files/tutorial001_02_an_py39.py` & `readyapi-0.111.0.dev1/docs_src/request_files/tutorial001_02_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/request_files/tutorial002.py` & `readyapi-0.111.0.dev1/docs_src/request_files/tutorial002.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/request_files/tutorial002_an.py` & `readyapi-0.111.0.dev1/docs_src/request_files/tutorial002_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/request_files/tutorial002_an_py39.py` & `readyapi-0.111.0.dev1/docs_src/request_files/tutorial002_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/request_files/tutorial002_py39.py` & `readyapi-0.111.0.dev1/docs_src/request_files/tutorial002_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/request_files/tutorial003.py` & `readyapi-0.111.0.dev1/docs_src/request_files/tutorial003.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/request_files/tutorial003_an.py` & `readyapi-0.111.0.dev1/docs_src/request_files/tutorial003_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/request_files/tutorial003_an_py39.py` & `readyapi-0.111.0.dev1/docs_src/request_files/tutorial003_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/request_files/tutorial003_py39.py` & `readyapi-0.111.0.dev1/docs_src/request_files/tutorial003_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/response_model/tutorial001.py` & `readyapi-0.111.0.dev1/docs_src/response_model/tutorial001.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/response_model/tutorial001_01.py` & `readyapi-0.111.0.dev1/docs_src/response_model/tutorial001_01.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/response_model/tutorial001_py310.py` & `readyapi-0.111.0.dev1/docs_src/response_model/tutorial001_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/response_model/tutorial001_py39.py` & `readyapi-0.111.0.dev1/docs_src/response_model/tutorial001_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/response_model/tutorial004.py` & `readyapi-0.111.0.dev1/docs_src/response_model/tutorial004.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/response_model/tutorial004_py310.py` & `readyapi-0.111.0.dev1/docs_src/response_model/tutorial004_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/response_model/tutorial004_py39.py` & `readyapi-0.111.0.dev1/docs_src/response_model/tutorial004_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/response_model/tutorial005.py` & `readyapi-0.111.0.dev1/docs_src/response_model/tutorial005.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/response_model/tutorial005_py310.py` & `readyapi-0.111.0.dev1/docs_src/response_model/tutorial005_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/response_model/tutorial006.py` & `readyapi-0.111.0.dev1/docs_src/response_model/tutorial006.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/response_model/tutorial006_py310.py` & `readyapi-0.111.0.dev1/docs_src/response_model/tutorial006_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/schema_extra_example/tutorial001.py` & `readyapi-0.111.0.dev1/docs_src/schema_extra_example/tutorial001.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/schema_extra_example/tutorial001_pv1.py` & `readyapi-0.111.0.dev1/docs_src/schema_extra_example/tutorial001_pv1.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/schema_extra_example/tutorial001_py310.py` & `readyapi-0.111.0.dev1/docs_src/schema_extra_example/tutorial001_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/schema_extra_example/tutorial001_py310_pv1.py` & `readyapi-0.111.0.dev1/docs_src/schema_extra_example/tutorial001_py310_pv1.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/schema_extra_example/tutorial002.py` & `readyapi-0.111.0.dev1/docs_src/schema_extra_example/tutorial002.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/schema_extra_example/tutorial003.py` & `readyapi-0.111.0.dev1/docs_src/schema_extra_example/tutorial003.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/schema_extra_example/tutorial003_an.py` & `readyapi-0.111.0.dev1/docs_src/schema_extra_example/tutorial003_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/schema_extra_example/tutorial003_an_py310.py` & `readyapi-0.111.0.dev1/docs_src/schema_extra_example/tutorial003_an_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/schema_extra_example/tutorial003_an_py39.py` & `readyapi-0.111.0.dev1/docs_src/schema_extra_example/tutorial003_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/schema_extra_example/tutorial003_py310.py` & `readyapi-0.111.0.dev1/docs_src/schema_extra_example/tutorial003_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/schema_extra_example/tutorial004.py` & `readyapi-0.111.0.dev1/docs_src/schema_extra_example/tutorial004.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/schema_extra_example/tutorial004_an.py` & `readyapi-0.111.0.dev1/docs_src/schema_extra_example/tutorial004_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/schema_extra_example/tutorial004_an_py310.py` & `readyapi-0.111.0.dev1/docs_src/schema_extra_example/tutorial004_an_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/schema_extra_example/tutorial004_an_py39.py` & `readyapi-0.111.0.dev1/docs_src/schema_extra_example/tutorial004_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/schema_extra_example/tutorial004_py310.py` & `readyapi-0.111.0.dev1/docs_src/schema_extra_example/tutorial004_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/schema_extra_example/tutorial005.py` & `readyapi-0.111.0.dev1/docs_src/schema_extra_example/tutorial005.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/schema_extra_example/tutorial005_an.py` & `readyapi-0.111.0.dev1/docs_src/schema_extra_example/tutorial005_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/schema_extra_example/tutorial005_an_py310.py` & `readyapi-0.111.0.dev1/docs_src/schema_extra_example/tutorial005_an_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/schema_extra_example/tutorial005_an_py39.py` & `readyapi-0.111.0.dev1/docs_src/schema_extra_example/tutorial005_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/schema_extra_example/tutorial005_py310.py` & `readyapi-0.111.0.dev1/docs_src/schema_extra_example/tutorial005_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/security/tutorial002.py` & `readyapi-0.111.0.dev1/docs_src/security/tutorial002.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/security/tutorial002_an.py` & `readyapi-0.111.0.dev1/docs_src/security/tutorial002_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/security/tutorial002_an_py310.py` & `readyapi-0.111.0.dev1/docs_src/security/tutorial002_an_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/security/tutorial002_an_py39.py` & `readyapi-0.111.0.dev1/docs_src/security/tutorial002_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/security/tutorial002_py310.py` & `readyapi-0.111.0.dev1/docs_src/security/tutorial002_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/security/tutorial003.py` & `readyapi-0.111.0.dev1/docs_src/security/tutorial003.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/security/tutorial003_an.py` & `readyapi-0.111.0.dev1/docs_src/security/tutorial003_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/security/tutorial003_an_py310.py` & `readyapi-0.111.0.dev1/docs_src/security/tutorial003_an_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/security/tutorial003_an_py39.py` & `readyapi-0.111.0.dev1/docs_src/security/tutorial003_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/security/tutorial003_py310.py` & `readyapi-0.111.0.dev1/docs_src/security/tutorial003_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/security/tutorial004.py` & `readyapi-0.111.0.dev1/docs_src/security/tutorial004.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/security/tutorial004_an.py` & `readyapi-0.111.0.dev1/docs_src/security/tutorial004_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/security/tutorial004_an_py310.py` & `readyapi-0.111.0.dev1/docs_src/security/tutorial004_an_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/security/tutorial004_an_py39.py` & `readyapi-0.111.0.dev1/docs_src/security/tutorial004_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/security/tutorial004_py310.py` & `readyapi-0.111.0.dev1/docs_src/security/tutorial004_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/security/tutorial005.py` & `readyapi-0.111.0.dev1/docs_src/security/tutorial005.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/security/tutorial005_an.py` & `readyapi-0.111.0.dev1/docs_src/security/tutorial005_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/security/tutorial005_an_py310.py` & `readyapi-0.111.0.dev1/docs_src/security/tutorial005_an_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/security/tutorial005_an_py39.py` & `readyapi-0.111.0.dev1/docs_src/security/tutorial005_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/security/tutorial005_py310.py` & `readyapi-0.111.0.dev1/docs_src/security/tutorial005_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/security/tutorial005_py39.py` & `readyapi-0.111.0.dev1/docs_src/security/tutorial005_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/security/tutorial007.py` & `readyapi-0.111.0.dev1/docs_src/security/tutorial007.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/security/tutorial007_an.py` & `readyapi-0.111.0.dev1/docs_src/security/tutorial007_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/security/tutorial007_an_py39.py` & `readyapi-0.111.0.dev1/docs_src/security/tutorial007_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/separate_openapi_schemas/tutorial002.py` & `readyapi-0.111.0.dev1/docs_src/separate_openapi_schemas/tutorial002.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/separate_openapi_schemas/tutorial002_py39.py` & `readyapi-0.111.0.dev1/docs_src/separate_openapi_schemas/tutorial002_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/settings/app02/test_main.py` & `readyapi-0.111.0.dev1/docs_src/settings/app02/test_main.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/settings/app02_an/test_main.py` & `readyapi-0.111.0.dev1/docs_src/settings/app02_an/test_main.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/settings/app02_an_py39/test_main.py` & `readyapi-0.111.0.dev1/docs_src/settings/app02_an_py39/test_main.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/sql_databases/sql_app/alt_main.py` & `readyapi-0.111.0.dev1/docs_src/sql_databases/sql_app/alt_main.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/sql_databases/sql_app/crud.py` & `readyapi-0.111.0.dev1/docs_src/sql_databases/sql_app/crud.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/sql_databases/sql_app/main.py` & `readyapi-0.111.0.dev1/docs_src/sql_databases/sql_app/main.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/sql_databases/sql_app/models.py` & `readyapi-0.111.0.dev1/docs_src/sql_databases/sql_app/models.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/sql_databases/sql_app/tests/test_sql_app.py` & `readyapi-0.111.0.dev1/docs_src/sql_databases/sql_app/tests/test_sql_app.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/sql_databases/sql_app_py310/alt_main.py` & `readyapi-0.111.0.dev1/docs_src/sql_databases/sql_app_py310/alt_main.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/sql_databases/sql_app_py310/crud.py` & `readyapi-0.111.0.dev1/docs_src/sql_databases/sql_app_py310/crud.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/sql_databases/sql_app_py310/main.py` & `readyapi-0.111.0.dev1/docs_src/sql_databases/sql_app_py310/main.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/sql_databases/sql_app_py310/models.py` & `readyapi-0.111.0.dev1/docs_src/sql_databases/sql_app_py310/models.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/sql_databases/sql_app_py310/tests/test_sql_app.py` & `readyapi-0.111.0.dev1/docs_src/sql_databases/sql_app_py310/tests/test_sql_app.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/sql_databases/sql_app_py39/alt_main.py` & `readyapi-0.111.0.dev1/docs_src/sql_databases/sql_app_py39/alt_main.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/sql_databases/sql_app_py39/crud.py` & `readyapi-0.111.0.dev1/docs_src/sql_databases/sql_app_py39/crud.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/sql_databases/sql_app_py39/main.py` & `readyapi-0.111.0.dev1/docs_src/sql_databases/sql_app_py39/main.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/sql_databases/sql_app_py39/models.py` & `readyapi-0.111.0.dev1/docs_src/sql_databases/sql_app_py39/models.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/sql_databases/sql_app_py39/tests/test_sql_app.py` & `readyapi-0.111.0.dev1/docs_src/sql_databases/sql_app_py39/tests/test_sql_app.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/sql_databases_peewee/sql_app/crud.py` & `readyapi-0.111.0.dev1/docs_src/sql_databases_peewee/sql_app/crud.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/sql_databases_peewee/sql_app/database.py` & `readyapi-0.111.0.dev1/docs_src/sql_databases_peewee/sql_app/database.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/sql_databases_peewee/sql_app/main.py` & `readyapi-0.111.0.dev1/docs_src/sql_databases_peewee/sql_app/main.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/sql_databases_peewee/sql_app/schemas.py` & `readyapi-0.111.0.dev1/docs_src/sql_databases_peewee/sql_app/schemas.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/templates/tutorial001.py` & `readyapi-0.111.0.dev1/docs_src/templates/tutorial001.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/websockets/tutorial001.py` & `readyapi-0.111.0.dev1/docs_src/websockets/tutorial001.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/websockets/tutorial002.py` & `readyapi-0.111.0.dev1/docs_src/websockets/tutorial002.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/websockets/tutorial002_an.py` & `readyapi-0.111.0.dev1/docs_src/websockets/tutorial002_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/websockets/tutorial002_an_py310.py` & `readyapi-0.111.0.dev1/docs_src/websockets/tutorial002_an_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/websockets/tutorial002_an_py39.py` & `readyapi-0.111.0.dev1/docs_src/websockets/tutorial002_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/websockets/tutorial002_py310.py` & `readyapi-0.111.0.dev1/docs_src/websockets/tutorial002_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/websockets/tutorial003.py` & `readyapi-0.111.0.dev1/docs_src/websockets/tutorial003.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/docs_src/websockets/tutorial003_py39.py` & `readyapi-0.111.0.dev1/docs_src/websockets/tutorial003_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/pdm_build.py` & `readyapi-0.111.0.dev1/pdm_build.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/pyproject.toml` & `readyapi-0.111.0.dev1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -41,23 +41,24 @@
     "Topic :: Internet :: WWW/HTTP :: HTTP Servers",
     "Topic :: Internet :: WWW/HTTP",
 ]
 dependencies = [
     "starlette>=0.37.2,<0.38.0",
     "pydantic>=1.7.4,!=1.8,!=1.8.1,!=2.0.0,!=2.0.1,!=2.1.0,<3.0.0",
     "typing-extensions>=4.8.0",
+    "readyapi-cli >=0.0.2",
     "httpx >=0.23.0",
     "jinja2 >=2.11.2",
     "python-multipart >=0.0.7",
     "ujson >=4.0.1,!=4.0.2,!=4.1.0,!=4.2.0,!=4.3.0,!=5.0.0,!=5.1.0",
     "orjson >=3.2.1",
     "email_validator >=2.0.0",
     "uvicorn[standard] >=0.12.0",
 ]
-version = "0.110.3"
+version = "0.111.0.dev1"
 
 [project.urls]
 Homepage = "https://github.com/khulnasoft/readyapi"
 Documentation = "https://readyapi.khulnasoft.com/"
 Repository = "https://github.com/khulnasoft/readyapi"
 
 [project.optional-dependencies]
```

### Comparing `readyapi-0.110.3/readyapi/__init__.py` & `readyapi-0.111.0.dev1/readyapi/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """ReadyAPI framework, high performance, easy to learn, fast to code, ready for production"""
 
-__version__ = "0.110.3"
+__version__ = "0.111.0.dev1"
 
 from starlette import status as status
 
 from .applications import ReadyAPI as ReadyAPI
 from .background import BackgroundTasks as BackgroundTasks
 from .datastructures import UploadFile as UploadFile
 from .exceptions import HTTPException as HTTPException
```

### Comparing `readyapi-0.110.3/readyapi/_compat.py` & `readyapi-0.111.0.dev1/readyapi/_compat.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/readyapi/applications.py` & `readyapi-0.111.0.dev1/readyapi/applications.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/readyapi/background.py` & `readyapi-0.111.0.dev1/readyapi/background.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/readyapi/concurrency.py` & `readyapi-0.111.0.dev1/readyapi/concurrency.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/readyapi/datastructures.py` & `readyapi-0.111.0.dev1/readyapi/datastructures.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/readyapi/dependencies/models.py` & `readyapi-0.111.0.dev1/readyapi/dependencies/models.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/readyapi/dependencies/utils.py` & `readyapi-0.111.0.dev1/readyapi/dependencies/utils.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/readyapi/encoders.py` & `readyapi-0.111.0.dev1/readyapi/encoders.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/readyapi/exception_handlers.py` & `readyapi-0.111.0.dev1/readyapi/exception_handlers.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/readyapi/exceptions.py` & `readyapi-0.111.0.dev1/readyapi/exceptions.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/readyapi/openapi/docs.py` & `readyapi-0.111.0.dev1/readyapi/openapi/docs.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/readyapi/openapi/models.py` & `readyapi-0.111.0.dev1/readyapi/openapi/models.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/readyapi/openapi/utils.py` & `readyapi-0.111.0.dev1/readyapi/openapi/utils.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/readyapi/param_functions.py` & `readyapi-0.111.0.dev1/readyapi/param_functions.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/readyapi/params.py` & `readyapi-0.111.0.dev1/readyapi/params.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/readyapi/responses.py` & `readyapi-0.111.0.dev1/readyapi/responses.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/readyapi/routing.py` & `readyapi-0.111.0.dev1/readyapi/routing.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/readyapi/security/__init__.py` & `readyapi-0.111.0.dev1/readyapi/security/__init__.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/readyapi/security/api_key.py` & `readyapi-0.111.0.dev1/readyapi/security/api_key.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/readyapi/security/http.py` & `readyapi-0.111.0.dev1/readyapi/security/http.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/readyapi/security/oauth2.py` & `readyapi-0.111.0.dev1/readyapi/security/oauth2.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/readyapi/security/open_id_connect_url.py` & `readyapi-0.111.0.dev1/readyapi/security/open_id_connect_url.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/readyapi/utils.py` & `readyapi-0.111.0.dev1/readyapi/utils.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/scripts/docs.py` & `readyapi-0.111.0.dev1/scripts/docs.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/scripts/mkdocs_hooks.py` & `readyapi-0.111.0.dev1/scripts/mkdocs_hooks.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/scripts/playwright/separate_openapi_schemas/image01.py` & `readyapi-0.111.0.dev1/scripts/playwright/separate_openapi_schemas/image01.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/scripts/playwright/separate_openapi_schemas/image02.py` & `readyapi-0.111.0.dev1/scripts/playwright/separate_openapi_schemas/image02.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/scripts/playwright/separate_openapi_schemas/image03.py` & `readyapi-0.111.0.dev1/scripts/playwright/separate_openapi_schemas/image03.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/scripts/playwright/separate_openapi_schemas/image04.py` & `readyapi-0.111.0.dev1/scripts/playwright/separate_openapi_schemas/image04.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/scripts/playwright/separate_openapi_schemas/image05.py` & `readyapi-0.111.0.dev1/scripts/playwright/separate_openapi_schemas/image05.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/main.py` & `readyapi-0.111.0.dev1/tests/main.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_additional_properties.py` & `readyapi-0.111.0.dev1/tests/test_additional_properties.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_additional_properties_bool.py` & `readyapi-0.111.0.dev1/tests/test_additional_properties_bool.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_additional_response_extra.py` & `readyapi-0.111.0.dev1/tests/test_additional_response_extra.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_additional_responses_bad.py` & `readyapi-0.111.0.dev1/tests/test_additional_responses_bad.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_additional_responses_custom_model_in_callback.py` & `readyapi-0.111.0.dev1/tests/test_additional_responses_custom_model_in_callback.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_additional_responses_custom_validationerror.py` & `readyapi-0.111.0.dev1/tests/test_additional_responses_custom_validationerror.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_additional_responses_default_validationerror.py` & `readyapi-0.111.0.dev1/tests/test_additional_responses_default_validationerror.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_additional_responses_response_class.py` & `readyapi-0.111.0.dev1/tests/test_additional_responses_response_class.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_additional_responses_router.py` & `readyapi-0.111.0.dev1/tests/test_additional_responses_router.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_ambiguous_params.py` & `readyapi-0.111.0.dev1/tests/test_ambiguous_params.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_annotated.py` & `readyapi-0.111.0.dev1/tests/test_annotated.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_application.py` & `readyapi-0.111.0.dev1/tests/test_application.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_compat.py` & `readyapi-0.111.0.dev1/tests/test_compat.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_computed_fields.py` & `readyapi-0.111.0.dev1/tests/test_computed_fields.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_custom_middleware_exception.py` & `readyapi-0.111.0.dev1/tests/test_custom_middleware_exception.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_custom_route_class.py` & `readyapi-0.111.0.dev1/tests/test_custom_route_class.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_custom_schema_fields.py` & `readyapi-0.111.0.dev1/tests/test_custom_schema_fields.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_custom_swagger_ui_redirect.py` & `readyapi-0.111.0.dev1/tests/test_custom_swagger_ui_redirect.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_datastructures.py` & `readyapi-0.111.0.dev1/tests/test_datastructures.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_datetime_custom_encoder.py` & `readyapi-0.111.0.dev1/tests/test_datetime_custom_encoder.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_default_response_class.py` & `readyapi-0.111.0.dev1/tests/test_default_response_class.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_default_response_class_router.py` & `readyapi-0.111.0.dev1/tests/test_default_response_class_router.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_dependency_cache.py` & `readyapi-0.111.0.dev1/tests/test_dependency_cache.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_dependency_class.py` & `readyapi-0.111.0.dev1/tests/test_dependency_class.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_dependency_contextmanager.py` & `readyapi-0.111.0.dev1/tests/test_dependency_contextmanager.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_dependency_contextvars.py` & `readyapi-0.111.0.dev1/tests/test_dependency_contextvars.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_dependency_duplicates.py` & `readyapi-0.111.0.dev1/tests/test_dependency_duplicates.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_dependency_normal_exceptions.py` & `readyapi-0.111.0.dev1/tests/test_dependency_normal_exceptions.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_dependency_overrides.py` & `readyapi-0.111.0.dev1/tests/test_dependency_overrides.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_dependency_security_overrides.py` & `readyapi-0.111.0.dev1/tests/test_dependency_security_overrides.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_deprecated_openapi_prefix.py` & `readyapi-0.111.0.dev1/tests/test_deprecated_openapi_prefix.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_duplicate_models_openapi.py` & `readyapi-0.111.0.dev1/tests/test_duplicate_models_openapi.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_empty_router.py` & `readyapi-0.111.0.dev1/tests/test_empty_router.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_enforce_once_required_parameter.py` & `readyapi-0.111.0.dev1/tests/test_enforce_once_required_parameter.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_exception_handlers.py` & `readyapi-0.111.0.dev1/tests/test_exception_handlers.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_extra_routes.py` & `readyapi-0.111.0.dev1/tests/test_extra_routes.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_filter_pydantic_sub_model/app_pv1.py` & `readyapi-0.111.0.dev1/tests/test_filter_pydantic_sub_model/app_pv1.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_filter_pydantic_sub_model/test_filter_pydantic_sub_model_pv1.py` & `readyapi-0.111.0.dev1/tests/test_filter_pydantic_sub_model/test_filter_pydantic_sub_model_pv1.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_filter_pydantic_sub_model_pv2.py` & `readyapi-0.111.0.dev1/tests/test_filter_pydantic_sub_model_pv2.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_forms_from_non_typing_sequences.py` & `readyapi-0.111.0.dev1/tests/test_forms_from_non_typing_sequences.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_generate_unique_id_function.py` & `readyapi-0.111.0.dev1/tests/test_generate_unique_id_function.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_generic_parameterless_depends.py` & `readyapi-0.111.0.dev1/tests/test_generic_parameterless_depends.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_get_request_body.py` & `readyapi-0.111.0.dev1/tests/test_get_request_body.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_http_connection_injection.py` & `readyapi-0.111.0.dev1/tests/test_http_connection_injection.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_include_router_defaults_overrides.py` & `readyapi-0.111.0.dev1/tests/test_include_router_defaults_overrides.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_infer_param_optionality.py` & `readyapi-0.111.0.dev1/tests/test_infer_param_optionality.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_inherited_custom_class.py` & `readyapi-0.111.0.dev1/tests/test_inherited_custom_class.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_invalid_path_param.py` & `readyapi-0.111.0.dev1/tests/test_invalid_path_param.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_invalid_sequence_param.py` & `readyapi-0.111.0.dev1/tests/test_invalid_sequence_param.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_jsonable_encoder.py` & `readyapi-0.111.0.dev1/tests/test_jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_local_docs.py` & `readyapi-0.111.0.dev1/tests/test_local_docs.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_modules_same_name_body/test_main.py` & `readyapi-0.111.0.dev1/tests/test_modules_same_name_body/test_main.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_multi_body_errors.py` & `readyapi-0.111.0.dev1/tests/test_multi_body_errors.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_multi_query_errors.py` & `readyapi-0.111.0.dev1/tests/test_multi_query_errors.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_multipart_installation.py` & `readyapi-0.111.0.dev1/tests/test_multipart_installation.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_no_swagger_ui_redirect.py` & `readyapi-0.111.0.dev1/tests/test_no_swagger_ui_redirect.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_openapi_examples.py` & `readyapi-0.111.0.dev1/tests/test_openapi_examples.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_openapi_query_parameter_extension.py` & `readyapi-0.111.0.dev1/tests/test_openapi_query_parameter_extension.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_openapi_route_extensions.py` & `readyapi-0.111.0.dev1/tests/test_openapi_route_extensions.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_openapi_separate_input_output_schemas.py` & `readyapi-0.111.0.dev1/tests/test_openapi_separate_input_output_schemas.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_openapi_servers.py` & `readyapi-0.111.0.dev1/tests/test_openapi_servers.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_operations_signatures.py` & `readyapi-0.111.0.dev1/tests/test_operations_signatures.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_orjson_response_class.py` & `readyapi-0.111.0.dev1/tests/test_orjson_response_class.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_param_class.py` & `readyapi-0.111.0.dev1/tests/test_param_class.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_param_in_path_and_dependency.py` & `readyapi-0.111.0.dev1/tests/test_param_in_path_and_dependency.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_param_include_in_schema.py` & `readyapi-0.111.0.dev1/tests/test_param_include_in_schema.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_params_repr.py` & `readyapi-0.111.0.dev1/tests/test_params_repr.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_path.py` & `readyapi-0.111.0.dev1/tests/test_path.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_put_no_body.py` & `readyapi-0.111.0.dev1/tests/test_put_no_body.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_query.py` & `readyapi-0.111.0.dev1/tests/test_query.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_read_with_orm_mode.py` & `readyapi-0.111.0.dev1/tests/test_read_with_orm_mode.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_regex_deprecated_body.py` & `readyapi-0.111.0.dev1/tests/test_regex_deprecated_body.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_regex_deprecated_params.py` & `readyapi-0.111.0.dev1/tests/test_regex_deprecated_params.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_repeated_cookie_headers.py` & `readyapi-0.111.0.dev1/tests/test_repeated_cookie_headers.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_repeated_dependency_schema.py` & `readyapi-0.111.0.dev1/tests/test_repeated_dependency_schema.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_repeated_parameter_alias.py` & `readyapi-0.111.0.dev1/tests/test_repeated_parameter_alias.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_reponse_set_reponse_code_empty.py` & `readyapi-0.111.0.dev1/tests/test_reponse_set_reponse_code_empty.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_request_body_parameters_media_type.py` & `readyapi-0.111.0.dev1/tests/test_request_body_parameters_media_type.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_required_noneable.py` & `readyapi-0.111.0.dev1/tests/test_required_noneable.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_response_by_alias.py` & `readyapi-0.111.0.dev1/tests/test_response_by_alias.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_response_change_status_code.py` & `readyapi-0.111.0.dev1/tests/test_response_change_status_code.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_response_class_no_mediatype.py` & `readyapi-0.111.0.dev1/tests/test_response_class_no_mediatype.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_response_code_no_body.py` & `readyapi-0.111.0.dev1/tests/test_response_code_no_body.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_response_model_as_return_annotation.py` & `readyapi-0.111.0.dev1/tests/test_response_model_as_return_annotation.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_response_model_data_filter.py` & `readyapi-0.111.0.dev1/tests/test_response_model_data_filter.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_response_model_data_filter_no_inheritance.py` & `readyapi-0.111.0.dev1/tests/test_response_model_data_filter_no_inheritance.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_response_model_include_exclude.py` & `readyapi-0.111.0.dev1/tests/test_response_model_include_exclude.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_response_model_invalid.py` & `readyapi-0.111.0.dev1/tests/test_response_model_invalid.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_response_model_sub_types.py` & `readyapi-0.111.0.dev1/tests/test_response_model_sub_types.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_route_scope.py` & `readyapi-0.111.0.dev1/tests/test_route_scope.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_router_events.py` & `readyapi-0.111.0.dev1/tests/test_router_events.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_router_redirect_slashes.py` & `readyapi-0.111.0.dev1/tests/test_router_redirect_slashes.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_schema_extra_examples.py` & `readyapi-0.111.0.dev1/tests/test_schema_extra_examples.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_security_api_key_cookie.py` & `readyapi-0.111.0.dev1/tests/test_security_api_key_cookie.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_security_api_key_cookie_description.py` & `readyapi-0.111.0.dev1/tests/test_security_api_key_cookie_description.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_security_api_key_cookie_optional.py` & `readyapi-0.111.0.dev1/tests/test_security_api_key_cookie_optional.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_security_api_key_header.py` & `readyapi-0.111.0.dev1/tests/test_security_api_key_header.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_security_api_key_header_description.py` & `readyapi-0.111.0.dev1/tests/test_security_api_key_header_description.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_security_api_key_header_optional.py` & `readyapi-0.111.0.dev1/tests/test_security_api_key_header_optional.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_security_api_key_query.py` & `readyapi-0.111.0.dev1/tests/test_security_api_key_query.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_security_api_key_query_description.py` & `readyapi-0.111.0.dev1/tests/test_security_api_key_query_description.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_security_api_key_query_optional.py` & `readyapi-0.111.0.dev1/tests/test_security_api_key_query_optional.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_security_http_base.py` & `readyapi-0.111.0.dev1/tests/test_security_http_base.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_security_http_base_description.py` & `readyapi-0.111.0.dev1/tests/test_security_http_base_description.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_security_http_base_optional.py` & `readyapi-0.111.0.dev1/tests/test_security_http_base_optional.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_security_http_basic_optional.py` & `readyapi-0.111.0.dev1/tests/test_security_http_basic_optional.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_security_http_basic_realm.py` & `readyapi-0.111.0.dev1/tests/test_security_http_basic_realm.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_security_http_basic_realm_description.py` & `readyapi-0.111.0.dev1/tests/test_security_http_basic_realm_description.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_security_http_bearer.py` & `readyapi-0.111.0.dev1/tests/test_security_http_bearer.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_security_http_bearer_description.py` & `readyapi-0.111.0.dev1/tests/test_security_http_bearer_description.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_security_http_bearer_optional.py` & `readyapi-0.111.0.dev1/tests/test_security_http_bearer_optional.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_security_http_digest.py` & `readyapi-0.111.0.dev1/tests/test_security_http_digest.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_security_http_digest_description.py` & `readyapi-0.111.0.dev1/tests/test_security_http_digest_description.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_security_http_digest_optional.py` & `readyapi-0.111.0.dev1/tests/test_security_http_digest_optional.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_security_oauth2.py` & `readyapi-0.111.0.dev1/tests/test_security_oauth2.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_security_oauth2_authorization_code_bearer.py` & `readyapi-0.111.0.dev1/tests/test_security_oauth2_authorization_code_bearer.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_security_oauth2_authorization_code_bearer_description.py` & `readyapi-0.111.0.dev1/tests/test_security_oauth2_authorization_code_bearer_description.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_security_oauth2_optional.py` & `readyapi-0.111.0.dev1/tests/test_security_oauth2_optional.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_security_oauth2_optional_description.py` & `readyapi-0.111.0.dev1/tests/test_security_oauth2_optional_description.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_security_oauth2_password_bearer_optional.py` & `readyapi-0.111.0.dev1/tests/test_security_oauth2_password_bearer_optional.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_security_oauth2_password_bearer_optional_description.py` & `readyapi-0.111.0.dev1/tests/test_security_oauth2_password_bearer_optional_description.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_security_openid_connect.py` & `readyapi-0.111.0.dev1/tests/test_security_openid_connect.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_security_openid_connect_description.py` & `readyapi-0.111.0.dev1/tests/test_security_openid_connect_description.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_security_openid_connect_optional.py` & `readyapi-0.111.0.dev1/tests/test_security_openid_connect_optional.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_serialize_response.py` & `readyapi-0.111.0.dev1/tests/test_serialize_response.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_serialize_response_dataclass.py` & `readyapi-0.111.0.dev1/tests/test_serialize_response_dataclass.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_serialize_response_model.py` & `readyapi-0.111.0.dev1/tests/test_serialize_response_model.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_skip_defaults.py` & `readyapi-0.111.0.dev1/tests/test_skip_defaults.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_starlette_exception.py` & `readyapi-0.111.0.dev1/tests/test_starlette_exception.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_starlette_urlconvertors.py` & `readyapi-0.111.0.dev1/tests/test_starlette_urlconvertors.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_sub_callbacks.py` & `readyapi-0.111.0.dev1/tests/test_sub_callbacks.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_swagger_ui_init_oauth.py` & `readyapi-0.111.0.dev1/tests/test_swagger_ui_init_oauth.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tuples.py` & `readyapi-0.111.0.dev1/tests/test_tuples.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_additional_responses/test_tutorial001.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_additional_responses/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_additional_responses/test_tutorial002.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_additional_responses/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_additional_responses/test_tutorial003.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_additional_responses/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_additional_responses/test_tutorial004.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_additional_responses/test_tutorial004.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_additional_status_codes/test_tutorial001.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_additional_status_codes/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_additional_status_codes/test_tutorial001_an.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_additional_status_codes/test_tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_additional_status_codes/test_tutorial001_an_py310.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_additional_status_codes/test_tutorial001_an_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_additional_status_codes/test_tutorial001_an_py39.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_additional_status_codes/test_tutorial001_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_additional_status_codes/test_tutorial001_py310.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_additional_status_codes/test_tutorial001_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_advanced_middleware/test_tutorial002.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_advanced_middleware/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_advanced_middleware/test_tutorial003.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_advanced_middleware/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_async_sql_databases/test_tutorial001.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_async_sql_databases/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_background_tasks/test_tutorial001.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_background_tasks/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_background_tasks/test_tutorial002.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_background_tasks/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_background_tasks/test_tutorial002_an.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_background_tasks/test_tutorial002_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_background_tasks/test_tutorial002_an_py310.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_background_tasks/test_tutorial002_an_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_background_tasks/test_tutorial002_an_py39.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_background_tasks/test_tutorial002_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_background_tasks/test_tutorial002_py310.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_background_tasks/test_tutorial002_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_behind_a_proxy/test_tutorial001.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_behind_a_proxy/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_behind_a_proxy/test_tutorial002.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_behind_a_proxy/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_behind_a_proxy/test_tutorial003.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_behind_a_proxy/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_behind_a_proxy/test_tutorial004.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_behind_a_proxy/test_tutorial004.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_bigger_applications/test_main.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_bigger_applications/test_main.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_bigger_applications/test_main_an.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_bigger_applications/test_main_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_bigger_applications/test_main_an_py39.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_bigger_applications/test_main_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_body/test_tutorial001.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_body/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_body/test_tutorial001_py310.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_body/test_tutorial001_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_body_fields/test_tutorial001.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_body_fields/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_body_fields/test_tutorial001_an.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_body_fields/test_tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_body_fields/test_tutorial001_an_py310.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_body_fields/test_tutorial001_an_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_body_fields/test_tutorial001_an_py39.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_body_fields/test_tutorial001_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_body_fields/test_tutorial001_py310.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_body_fields/test_tutorial001_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_body_multiple_params/test_tutorial001.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_body_multiple_params/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_body_multiple_params/test_tutorial001_an.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_body_multiple_params/test_tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_body_multiple_params/test_tutorial001_an_py310.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_body_multiple_params/test_tutorial001_an_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_body_multiple_params/test_tutorial001_an_py39.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_body_multiple_params/test_tutorial001_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_body_multiple_params/test_tutorial001_py310.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_body_multiple_params/test_tutorial001_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_body_multiple_params/test_tutorial003.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_body_multiple_params/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_body_multiple_params/test_tutorial003_an.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_body_multiple_params/test_tutorial003_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_body_multiple_params/test_tutorial003_an_py310.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_body_multiple_params/test_tutorial003_an_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_body_multiple_params/test_tutorial003_an_py39.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_body_multiple_params/test_tutorial003_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_body_multiple_params/test_tutorial003_py310.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_body_multiple_params/test_tutorial003_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_body_nested_models/test_tutorial009.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_body_nested_models/test_tutorial009.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_body_nested_models/test_tutorial009_py39.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_body_nested_models/test_tutorial009_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_body_updates/test_tutorial001.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_body_updates/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_body_updates/test_tutorial001_py310.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_body_updates/test_tutorial001_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_body_updates/test_tutorial001_py39.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_body_updates/test_tutorial001_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_conditional_openapi/test_tutorial001.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_conditional_openapi/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_configure_swagger_ui/test_tutorial001.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_configure_swagger_ui/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_configure_swagger_ui/test_tutorial002.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_configure_swagger_ui/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_configure_swagger_ui/test_tutorial003.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_configure_swagger_ui/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_cookie_params/test_tutorial001.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_cookie_params/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_cookie_params/test_tutorial001_an.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_cookie_params/test_tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_cookie_params/test_tutorial001_an_py310.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_cookie_params/test_tutorial001_an_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_cookie_params/test_tutorial001_an_py39.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_cookie_params/test_tutorial001_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_cookie_params/test_tutorial001_py310.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_cookie_params/test_tutorial001_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_cors/test_tutorial001.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_cors/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_custom_docs_ui/test_tutorial001.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_custom_docs_ui/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_custom_docs_ui/test_tutorial002.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_custom_docs_ui/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_custom_request_and_route/test_tutorial001.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_custom_request_and_route/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_custom_request_and_route/test_tutorial002.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_custom_request_and_route/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_custom_request_and_route/test_tutorial003.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_custom_request_and_route/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_custom_response/test_tutorial001.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_custom_response/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_custom_response/test_tutorial001b.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_custom_response/test_tutorial001b.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_custom_response/test_tutorial004.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_custom_response/test_tutorial004.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_custom_response/test_tutorial005.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_custom_response/test_tutorial005.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_custom_response/test_tutorial006.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_custom_response/test_tutorial006.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_custom_response/test_tutorial006b.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_custom_response/test_tutorial006b.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_custom_response/test_tutorial006c.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_custom_response/test_tutorial006c.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_dataclasses/test_tutorial001.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_dataclasses/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_dataclasses/test_tutorial002.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_dataclasses/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_dataclasses/test_tutorial003.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_dataclasses/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_dependencies/test_tutorial001.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_dependencies/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_dependencies/test_tutorial001_an.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_dependencies/test_tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_dependencies/test_tutorial001_an_py310.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_dependencies/test_tutorial001_an_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_dependencies/test_tutorial001_an_py39.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_dependencies/test_tutorial001_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_dependencies/test_tutorial001_py310.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_dependencies/test_tutorial001_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_dependencies/test_tutorial004.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_dependencies/test_tutorial004.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_dependencies/test_tutorial004_an.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_dependencies/test_tutorial004_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_dependencies/test_tutorial004_an_py310.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_dependencies/test_tutorial004_an_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_dependencies/test_tutorial004_an_py39.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_dependencies/test_tutorial004_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_dependencies/test_tutorial004_py310.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_dependencies/test_tutorial004_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_dependencies/test_tutorial006.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_dependencies/test_tutorial006.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_dependencies/test_tutorial006_an.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_dependencies/test_tutorial006_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_dependencies/test_tutorial006_an_py39.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_dependencies/test_tutorial006_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_dependencies/test_tutorial008b.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_dependencies/test_tutorial008b.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_dependencies/test_tutorial008b_an.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_dependencies/test_tutorial008b_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_dependencies/test_tutorial008b_an_py39.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_dependencies/test_tutorial008b_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_dependencies/test_tutorial008c.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_dependencies/test_tutorial008c.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_dependencies/test_tutorial008c_an.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_dependencies/test_tutorial008c_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_dependencies/test_tutorial008c_an_py39.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_dependencies/test_tutorial008c_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_dependencies/test_tutorial008d.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_dependencies/test_tutorial008d.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_dependencies/test_tutorial008d_an.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_dependencies/test_tutorial008d_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_dependencies/test_tutorial008d_an_py39.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_dependencies/test_tutorial008d_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_dependencies/test_tutorial012.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_dependencies/test_tutorial012.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_dependencies/test_tutorial012_an.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_dependencies/test_tutorial012_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_dependencies/test_tutorial012_an_py39.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_dependencies/test_tutorial012_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_events/test_tutorial001.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_events/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_events/test_tutorial002.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_events/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_events/test_tutorial003.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_events/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_extending_openapi/test_tutorial001.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_extending_openapi/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_extra_data_types/test_tutorial001.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_extra_data_types/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_extra_data_types/test_tutorial001_an.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_extra_data_types/test_tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_extra_data_types/test_tutorial001_an_py310.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_extra_data_types/test_tutorial001_an_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_extra_data_types/test_tutorial001_an_py39.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_extra_data_types/test_tutorial001_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_extra_data_types/test_tutorial001_py310.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_extra_data_types/test_tutorial001_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_extra_models/test_tutorial003.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_extra_models/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_extra_models/test_tutorial003_py310.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_extra_models/test_tutorial003_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_extra_models/test_tutorial004.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_extra_models/test_tutorial004.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_extra_models/test_tutorial004_py39.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_extra_models/test_tutorial004_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_extra_models/test_tutorial005.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_extra_models/test_tutorial005.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_extra_models/test_tutorial005_py39.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_extra_models/test_tutorial005_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_first_steps/test_tutorial001.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_first_steps/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_generate_clients/test_tutorial003.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_generate_clients/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_handling_errors/test_tutorial001.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_handling_errors/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_handling_errors/test_tutorial002.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_handling_errors/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_handling_errors/test_tutorial003.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_handling_errors/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_handling_errors/test_tutorial004.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_handling_errors/test_tutorial004.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_handling_errors/test_tutorial005.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_handling_errors/test_tutorial005.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_handling_errors/test_tutorial006.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_handling_errors/test_tutorial006.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_header_params/test_tutorial001.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_header_params/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_header_params/test_tutorial001_an.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_header_params/test_tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_header_params/test_tutorial001_an_py310.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_header_params/test_tutorial001_an_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_header_params/test_tutorial001_py310.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_header_params/test_tutorial001_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_header_params/test_tutorial002.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_header_params/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_header_params/test_tutorial002_an.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_header_params/test_tutorial002_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_header_params/test_tutorial002_an_py310.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_header_params/test_tutorial002_an_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_header_params/test_tutorial002_an_py39.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_header_params/test_tutorial002_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_header_params/test_tutorial002_py310.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_header_params/test_tutorial002_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_header_params/test_tutorial003.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_header_params/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_header_params/test_tutorial003_an.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_header_params/test_tutorial003_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_header_params/test_tutorial003_an_py310.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_header_params/test_tutorial003_an_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_header_params/test_tutorial003_an_py39.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_header_params/test_tutorial003_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_header_params/test_tutorial003_py310.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_header_params/test_tutorial003_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_metadata/test_tutorial001.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_metadata/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_metadata/test_tutorial001_1.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_metadata/test_tutorial001_1.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_metadata/test_tutorial004.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_metadata/test_tutorial004.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_openapi_callbacks/test_tutorial001.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_openapi_callbacks/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_openapi_webhooks/test_tutorial001.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_openapi_webhooks/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial001.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial002.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial003.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial004.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial004.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial005.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial005.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial006.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial006.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial007.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial007.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial007_pv1.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial007_pv1.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_path_operation_configurations/test_tutorial002b.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_path_operation_configurations/test_tutorial002b.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_path_operation_configurations/test_tutorial005.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_path_operation_configurations/test_tutorial005.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_path_operation_configurations/test_tutorial005_py310.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_path_operation_configurations/test_tutorial005_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_path_operation_configurations/test_tutorial005_py39.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_path_operation_configurations/test_tutorial005_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_path_operation_configurations/test_tutorial006.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_path_operation_configurations/test_tutorial006.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_path_params/test_tutorial004.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_path_params/test_tutorial004.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_path_params/test_tutorial005.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_path_params/test_tutorial005.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_query_params/test_tutorial005.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_query_params/test_tutorial005.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_query_params/test_tutorial006.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_query_params/test_tutorial006.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_query_params/test_tutorial006_py310.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_query_params/test_tutorial006_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_query_params_str_validations/test_tutorial010.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial010.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_query_params_str_validations/test_tutorial010_an.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial010_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_query_params_str_validations/test_tutorial010_an_py310.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial010_an_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_query_params_str_validations/test_tutorial010_an_py39.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial010_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_query_params_str_validations/test_tutorial010_py310.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial010_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_query_params_str_validations/test_tutorial011.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial011.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_query_params_str_validations/test_tutorial011_an.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial011_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_query_params_str_validations/test_tutorial011_an_py310.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial011_an_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_query_params_str_validations/test_tutorial011_an_py39.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial011_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_query_params_str_validations/test_tutorial011_py310.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial011_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_query_params_str_validations/test_tutorial011_py39.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial011_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_query_params_str_validations/test_tutorial012.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial012.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_query_params_str_validations/test_tutorial012_an.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial012_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_query_params_str_validations/test_tutorial012_an_py39.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial012_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_query_params_str_validations/test_tutorial012_py39.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial012_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_query_params_str_validations/test_tutorial013.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial013.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_query_params_str_validations/test_tutorial013_an.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial013_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_query_params_str_validations/test_tutorial013_an_py39.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial013_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_query_params_str_validations/test_tutorial014.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial014.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_query_params_str_validations/test_tutorial014_an.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial014_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_query_params_str_validations/test_tutorial014_an_py310.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial014_an_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_query_params_str_validations/test_tutorial014_an_py39.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial014_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_query_params_str_validations/test_tutorial014_py310.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial014_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_request_files/test_tutorial001.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_request_files/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_request_files/test_tutorial001_02.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_request_files/test_tutorial001_02.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_request_files/test_tutorial001_02_an.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_request_files/test_tutorial001_02_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_request_files/test_tutorial001_02_an_py310.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_request_files/test_tutorial001_02_an_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_request_files/test_tutorial001_02_an_py39.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_request_files/test_tutorial001_02_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_request_files/test_tutorial001_02_py310.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_request_files/test_tutorial001_02_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_request_files/test_tutorial001_03.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_request_files/test_tutorial001_03.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_request_files/test_tutorial001_03_an.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_request_files/test_tutorial001_03_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_request_files/test_tutorial001_03_an_py39.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_request_files/test_tutorial001_03_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_request_files/test_tutorial001_an.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_request_files/test_tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_request_files/test_tutorial001_an_py39.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_request_files/test_tutorial001_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_request_files/test_tutorial002.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_request_files/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_request_files/test_tutorial002_an.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_request_files/test_tutorial002_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_request_files/test_tutorial002_an_py39.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_request_files/test_tutorial002_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_request_files/test_tutorial002_py39.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_request_files/test_tutorial002_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_request_files/test_tutorial003.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_request_files/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_request_files/test_tutorial003_an.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_request_files/test_tutorial003_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_request_files/test_tutorial003_an_py39.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_request_files/test_tutorial003_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_request_files/test_tutorial003_py39.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_request_files/test_tutorial003_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_request_forms/test_tutorial001.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_request_forms/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_request_forms/test_tutorial001_an.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_request_forms/test_tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_request_forms/test_tutorial001_an_py39.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_request_forms/test_tutorial001_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_request_forms_and_files/test_tutorial001.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_request_forms_and_files/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_request_forms_and_files/test_tutorial001_an.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_request_forms_and_files/test_tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_request_forms_and_files/test_tutorial001_an_py39.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_request_forms_and_files/test_tutorial001_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_response_change_status_code/test_tutorial001.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_response_change_status_code/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_response_model/test_tutorial003.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_response_model/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_response_model/test_tutorial003_01.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_response_model/test_tutorial003_01.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_response_model/test_tutorial003_01_py310.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_response_model/test_tutorial003_01_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_response_model/test_tutorial003_02.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_response_model/test_tutorial003_02.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_response_model/test_tutorial003_03.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_response_model/test_tutorial003_03.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_response_model/test_tutorial003_05.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_response_model/test_tutorial003_05.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_response_model/test_tutorial003_05_py310.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_response_model/test_tutorial003_05_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_response_model/test_tutorial003_py310.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_response_model/test_tutorial003_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_response_model/test_tutorial004.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_response_model/test_tutorial004.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_response_model/test_tutorial004_py310.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_response_model/test_tutorial004_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_response_model/test_tutorial004_py39.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_response_model/test_tutorial004_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_response_model/test_tutorial005.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_response_model/test_tutorial005.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_response_model/test_tutorial005_py310.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_response_model/test_tutorial005_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_response_model/test_tutorial006.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_response_model/test_tutorial006.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_response_model/test_tutorial006_py310.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_response_model/test_tutorial006_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_schema_extra_example/test_tutorial001.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_schema_extra_example/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_schema_extra_example/test_tutorial001_pv1.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_schema_extra_example/test_tutorial001_pv1.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_schema_extra_example/test_tutorial001_py310.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_schema_extra_example/test_tutorial001_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_schema_extra_example/test_tutorial001_py310_pv1.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_schema_extra_example/test_tutorial001_py310_pv1.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_schema_extra_example/test_tutorial004.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_schema_extra_example/test_tutorial004.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_schema_extra_example/test_tutorial004_an.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_schema_extra_example/test_tutorial004_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_schema_extra_example/test_tutorial004_an_py310.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_schema_extra_example/test_tutorial004_an_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_schema_extra_example/test_tutorial004_an_py39.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_schema_extra_example/test_tutorial004_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_schema_extra_example/test_tutorial004_py310.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_schema_extra_example/test_tutorial004_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_schema_extra_example/test_tutorial005.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_schema_extra_example/test_tutorial005.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_schema_extra_example/test_tutorial005_an.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_schema_extra_example/test_tutorial005_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_schema_extra_example/test_tutorial005_an_py310.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_schema_extra_example/test_tutorial005_an_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_schema_extra_example/test_tutorial005_an_py39.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_schema_extra_example/test_tutorial005_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_schema_extra_example/test_tutorial005_py310.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_schema_extra_example/test_tutorial005_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_security/test_tutorial001.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_security/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_security/test_tutorial001_an.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_security/test_tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_security/test_tutorial001_an_py39.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_security/test_tutorial001_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_security/test_tutorial003.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_security/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_security/test_tutorial003_an.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_security/test_tutorial003_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_security/test_tutorial003_an_py310.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_security/test_tutorial003_an_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_security/test_tutorial003_an_py39.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_security/test_tutorial003_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_security/test_tutorial003_py310.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_security/test_tutorial003_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_security/test_tutorial005.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_security/test_tutorial005.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_security/test_tutorial005_an.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_security/test_tutorial005_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_security/test_tutorial005_an_py310.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_security/test_tutorial005_an_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_security/test_tutorial005_an_py39.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_security/test_tutorial005_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_security/test_tutorial005_py310.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_security/test_tutorial005_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_security/test_tutorial005_py39.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_security/test_tutorial005_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_security/test_tutorial006.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_security/test_tutorial006.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_security/test_tutorial006_an.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_security/test_tutorial006_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_security/test_tutorial006_an_py39.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_security/test_tutorial006_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_separate_openapi_schemas/test_tutorial001.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_separate_openapi_schemas/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_separate_openapi_schemas/test_tutorial001_py310.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_separate_openapi_schemas/test_tutorial001_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_separate_openapi_schemas/test_tutorial001_py39.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_separate_openapi_schemas/test_tutorial001_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_separate_openapi_schemas/test_tutorial002.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_separate_openapi_schemas/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_separate_openapi_schemas/test_tutorial002_py310.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_separate_openapi_schemas/test_tutorial002_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_separate_openapi_schemas/test_tutorial002_py39.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_separate_openapi_schemas/test_tutorial002_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_settings/test_tutorial001.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_settings/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_settings/test_tutorial001_pv1.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_settings/test_tutorial001_pv1.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_sql_databases/test_sql_databases.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_sql_databases/test_sql_databases.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_sql_databases/test_sql_databases_middleware.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_sql_databases/test_sql_databases_middleware.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_sql_databases/test_sql_databases_middleware_py310.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_sql_databases/test_sql_databases_middleware_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_sql_databases/test_sql_databases_middleware_py39.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_sql_databases/test_sql_databases_middleware_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_sql_databases/test_sql_databases_py310.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_sql_databases/test_sql_databases_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_sql_databases/test_sql_databases_py39.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_sql_databases/test_sql_databases_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_sql_databases/test_testing_databases.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_sql_databases/test_testing_databases.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_sql_databases/test_testing_databases_py310.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_sql_databases/test_testing_databases_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_sql_databases/test_testing_databases_py39.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_sql_databases/test_testing_databases_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_sub_applications/test_tutorial001.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_sub_applications/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_templates/test_tutorial001.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_templates/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_testing/test_main.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_testing/test_main.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_testing/test_tutorial001.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_testing/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_testing_dependencies/test_tutorial001.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_testing_dependencies/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_testing_dependencies/test_tutorial001_an.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_testing_dependencies/test_tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_testing_dependencies/test_tutorial001_an_py310.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_testing_dependencies/test_tutorial001_an_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_testing_dependencies/test_tutorial001_an_py39.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_testing_dependencies/test_tutorial001_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_testing_dependencies/test_tutorial001_py310.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_testing_dependencies/test_tutorial001_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_websockets/test_tutorial001.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_websockets/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_websockets/test_tutorial002.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_websockets/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_websockets/test_tutorial002_an.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_websockets/test_tutorial002_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_websockets/test_tutorial002_an_py310.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_websockets/test_tutorial002_an_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_websockets/test_tutorial002_an_py39.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_websockets/test_tutorial002_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_websockets/test_tutorial002_py310.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_websockets/test_tutorial002_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_websockets/test_tutorial003.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_websockets/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_tutorial/test_websockets/test_tutorial003_py39.py` & `readyapi-0.111.0.dev1/tests/test_tutorial/test_websockets/test_tutorial003_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_typing_python39.py` & `readyapi-0.111.0.dev1/tests/test_typing_python39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_union_body.py` & `readyapi-0.111.0.dev1/tests/test_union_body.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_union_inherited_body.py` & `readyapi-0.111.0.dev1/tests/test_union_inherited_body.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_validate_response.py` & `readyapi-0.111.0.dev1/tests/test_validate_response.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_validate_response_dataclass.py` & `readyapi-0.111.0.dev1/tests/test_validate_response_dataclass.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_validate_response_recursive/app_pv1.py` & `readyapi-0.111.0.dev1/tests/test_validate_response_recursive/app_pv1.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_validate_response_recursive/app_pv2.py` & `readyapi-0.111.0.dev1/tests/test_validate_response_recursive/app_pv2.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_validate_response_recursive/test_validate_response_recursive_pv1.py` & `readyapi-0.111.0.dev1/tests/test_validate_response_recursive/test_validate_response_recursive_pv1.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_validate_response_recursive/test_validate_response_recursive_pv2.py` & `readyapi-0.111.0.dev1/tests/test_validate_response_recursive/test_validate_response_recursive_pv2.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_webhooks_security.py` & `readyapi-0.111.0.dev1/tests/test_webhooks_security.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_ws_dependencies.py` & `readyapi-0.111.0.dev1/tests/test_ws_dependencies.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/tests/test_ws_router.py` & `readyapi-0.111.0.dev1/tests/test_ws_router.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.3/PKG-INFO` & `readyapi-0.111.0.dev1/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,1591 +1,1272 @@
-00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
-00000010: 3a20 322e 310a 4e61 6d65 3a20 7265 6164  : 2.1.Name: read
-00000020: 7961 7069 0a56 6572 7369 6f6e 3a20 302e  yapi.Version: 0.
-00000030: 3131 302e 330a 5375 6d6d 6172 793a 2052  110.3.Summary: R
-00000040: 6561 6479 4150 4920 6672 616d 6577 6f72  eadyAPI framewor
-00000050: 6b2c 2068 6967 6820 7065 7266 6f72 6d61  k, high performa
-00000060: 6e63 652c 2065 6173 7920 746f 206c 6561  nce, easy to lea
-00000070: 726e 2c20 6661 7374 2074 6f20 636f 6465  rn, fast to code
-00000080: 2c20 7265 6164 7920 666f 7220 7072 6f64  , ready for prod
-00000090: 7563 7469 6f6e 0a41 7574 686f 722d 456d  uction.Author-Em
-000000a0: 6169 6c3a 204b 6875 6c6e 6153 6f66 7420  ail: KhulnaSoft 
-000000b0: 4465 764f 7073 203c 696e 666f 406b 6875  DevOps <info@khu
-000000c0: 6c6e 6173 6f66 742e 636f 6d3e 0a43 6c61  lnasoft.com>.Cla
-000000d0: 7373 6966 6965 723a 2049 6e74 656e 6465  ssifier: Intende
-000000e0: 6420 4175 6469 656e 6365 203a 3a20 496e  d Audience :: In
-000000f0: 666f 726d 6174 696f 6e20 5465 6368 6e6f  formation Techno
-00000100: 6c6f 6779 0a43 6c61 7373 6966 6965 723a  logy.Classifier:
-00000110: 2049 6e74 656e 6465 6420 4175 6469 656e   Intended Audien
-00000120: 6365 203a 3a20 5379 7374 656d 2041 646d  ce :: System Adm
-00000130: 696e 6973 7472 6174 6f72 730a 436c 6173  inistrators.Clas
-00000140: 7369 6669 6572 3a20 4f70 6572 6174 696e  sifier: Operatin
-00000150: 6720 5379 7374 656d 203a 3a20 4f53 2049  g System :: OS I
-00000160: 6e64 6570 656e 6465 6e74 0a43 6c61 7373  ndependent.Class
-00000170: 6966 6965 723a 2050 726f 6772 616d 6d69  ifier: Programmi
-00000180: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
-00000190: 7974 686f 6e20 3a3a 2033 0a43 6c61 7373  ython :: 3.Class
-000001a0: 6966 6965 723a 2050 726f 6772 616d 6d69  ifier: Programmi
-000001b0: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
-000001c0: 7974 686f 6e0a 436c 6173 7369 6669 6572  ython.Classifier
-000001d0: 3a20 546f 7069 6320 3a3a 2049 6e74 6572  : Topic :: Inter
-000001e0: 6e65 740a 436c 6173 7369 6669 6572 3a20  net.Classifier: 
-000001f0: 546f 7069 6320 3a3a 2053 6f66 7477 6172  Topic :: Softwar
-00000200: 6520 4465 7665 6c6f 706d 656e 7420 3a3a  e Development ::
-00000210: 204c 6962 7261 7269 6573 203a 3a20 4170   Libraries :: Ap
-00000220: 706c 6963 6174 696f 6e20 4672 616d 6577  plication Framew
-00000230: 6f72 6b73 0a43 6c61 7373 6966 6965 723a  orks.Classifier:
-00000240: 2054 6f70 6963 203a 3a20 536f 6674 7761   Topic :: Softwa
-00000250: 7265 2044 6576 656c 6f70 6d65 6e74 203a  re Development :
-00000260: 3a20 4c69 6272 6172 6965 7320 3a3a 2050  : Libraries :: P
-00000270: 7974 686f 6e20 4d6f 6475 6c65 730a 436c  ython Modules.Cl
-00000280: 6173 7369 6669 6572 3a20 546f 7069 6320  assifier: Topic 
-00000290: 3a3a 2053 6f66 7477 6172 6520 4465 7665  :: Software Deve
-000002a0: 6c6f 706d 656e 7420 3a3a 204c 6962 7261  lopment :: Libra
-000002b0: 7269 6573 0a43 6c61 7373 6966 6965 723a  ries.Classifier:
-000002c0: 2054 6f70 6963 203a 3a20 536f 6674 7761   Topic :: Softwa
-000002d0: 7265 2044 6576 656c 6f70 6d65 6e74 0a43  re Development.C
-000002e0: 6c61 7373 6966 6965 723a 2054 7970 696e  lassifier: Typin
-000002f0: 6720 3a3a 2054 7970 6564 0a43 6c61 7373  g :: Typed.Class
-00000300: 6966 6965 723a 2044 6576 656c 6f70 6d65  ifier: Developme
-00000310: 6e74 2053 7461 7475 7320 3a3a 2034 202d  nt Status :: 4 -
-00000320: 2042 6574 610a 436c 6173 7369 6669 6572   Beta.Classifier
-00000330: 3a20 456e 7669 726f 6e6d 656e 7420 3a3a  : Environment ::
-00000340: 2057 6562 2045 6e76 6972 6f6e 6d65 6e74   Web Environment
-00000350: 0a43 6c61 7373 6966 6965 723a 2046 7261  .Classifier: Fra
-00000360: 6d65 776f 726b 203a 3a20 4173 796e 6349  mework :: AsyncI
-00000370: 4f0a 436c 6173 7369 6669 6572 3a20 4672  O.Classifier: Fr
-00000380: 616d 6577 6f72 6b20 3a3a 2050 7964 616e  amework :: Pydan
-00000390: 7469 630a 436c 6173 7369 6669 6572 3a20  tic.Classifier: 
-000003a0: 4672 616d 6577 6f72 6b20 3a3a 2050 7964  Framework :: Pyd
-000003b0: 616e 7469 6320 3a3a 2031 0a43 6c61 7373  antic :: 1.Class
-000003c0: 6966 6965 723a 2049 6e74 656e 6465 6420  ifier: Intended 
-000003d0: 4175 6469 656e 6365 203a 3a20 4465 7665  Audience :: Deve
-000003e0: 6c6f 7065 7273 0a43 6c61 7373 6966 6965  lopers.Classifie
-000003f0: 723a 204c 6963 656e 7365 203a 3a20 4f53  r: License :: OS
-00000400: 4920 4170 7072 6f76 6564 203a 3a20 4d49  I Approved :: MI
-00000410: 5420 4c69 6365 6e73 650a 436c 6173 7369  T License.Classi
-00000420: 6669 6572 3a20 5072 6f67 7261 6d6d 696e  fier: Programmin
-00000430: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
-00000440: 7468 6f6e 203a 3a20 3320 3a3a 204f 6e6c  thon :: 3 :: Onl
-00000450: 790a 436c 6173 7369 6669 6572 3a20 5072  y.Classifier: Pr
-00000460: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
-00000470: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
-00000480: 332e 380a 436c 6173 7369 6669 6572 3a20  3.8.Classifier: 
-00000490: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
-000004a0: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
-000004b0: 3a20 332e 390a 436c 6173 7369 6669 6572  : 3.9.Classifier
-000004c0: 3a20 5072 6f67 7261 6d6d 696e 6720 4c61  : Programming La
-000004d0: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
-000004e0: 203a 3a20 332e 3130 0a43 6c61 7373 6966   :: 3.10.Classif
-000004f0: 6965 723a 2050 726f 6772 616d 6d69 6e67  ier: Programming
-00000500: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
-00000510: 686f 6e20 3a3a 2033 2e31 310a 436c 6173  hon :: 3.11.Clas
-00000520: 7369 6669 6572 3a20 5072 6f67 7261 6d6d  sifier: Programm
-00000530: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
-00000540: 5079 7468 6f6e 203a 3a20 332e 3132 0a43  Python :: 3.12.C
-00000550: 6c61 7373 6966 6965 723a 2054 6f70 6963  lassifier: Topic
-00000560: 203a 3a20 496e 7465 726e 6574 203a 3a20   :: Internet :: 
-00000570: 5757 572f 4854 5450 203a 3a20 4854 5450  WWW/HTTP :: HTTP
-00000580: 2053 6572 7665 7273 0a43 6c61 7373 6966   Servers.Classif
-00000590: 6965 723a 2054 6f70 6963 203a 3a20 496e  ier: Topic :: In
-000005a0: 7465 726e 6574 203a 3a20 5757 572f 4854  ternet :: WWW/HT
-000005b0: 5450 0a50 726f 6a65 6374 2d55 524c 3a20  TP.Project-URL: 
-000005c0: 486f 6d65 7061 6765 2c20 6874 7470 733a  Homepage, https:
-000005d0: 2f2f 6769 7468 7562 2e63 6f6d 2f6b 6875  //github.com/khu
-000005e0: 6c6e 6173 6f66 742f 7265 6164 7961 7069  lnasoft/readyapi
-000005f0: 0a50 726f 6a65 6374 2d55 524c 3a20 446f  .Project-URL: Do
-00000600: 6375 6d65 6e74 6174 696f 6e2c 2068 7474  cumentation, htt
-00000610: 7073 3a2f 2f72 6561 6479 6170 692e 6b68  ps://readyapi.kh
-00000620: 756c 6e61 736f 6674 2e63 6f6d 2f0a 5072  ulnasoft.com/.Pr
-00000630: 6f6a 6563 742d 5552 4c3a 2052 6570 6f73  oject-URL: Repos
-00000640: 6974 6f72 792c 2068 7474 7073 3a2f 2f67  itory, https://g
-00000650: 6974 6875 622e 636f 6d2f 6b68 756c 6e61  ithub.com/khulna
-00000660: 736f 6674 2f72 6561 6479 6170 690a 5265  soft/readyapi.Re
-00000670: 7175 6972 6573 2d50 7974 686f 6e3a 203e  quires-Python: >
-00000680: 3d33 2e38 0a52 6571 7569 7265 732d 4469  =3.8.Requires-Di
-00000690: 7374 3a20 7374 6172 6c65 7474 653c 302e  st: starlette<0.
-000006a0: 3338 2e30 2c3e 3d30 2e33 372e 320a 5265  38.0,>=0.37.2.Re
-000006b0: 7175 6972 6573 2d44 6973 743a 2070 7964  quires-Dist: pyd
-000006c0: 616e 7469 6321 3d31 2e38 2c21 3d31 2e38  antic!=1.8,!=1.8
-000006d0: 2e31 2c21 3d32 2e30 2e30 2c21 3d32 2e30  .1,!=2.0.0,!=2.0
-000006e0: 2e31 2c21 3d32 2e31 2e30 2c3c 332e 302e  .1,!=2.1.0,<3.0.
-000006f0: 302c 3e3d 312e 372e 340a 5265 7175 6972  0,>=1.7.4.Requir
-00000700: 6573 2d44 6973 743a 2074 7970 696e 672d  es-Dist: typing-
-00000710: 6578 7465 6e73 696f 6e73 3e3d 342e 382e  extensions>=4.8.
-00000720: 300a 5265 7175 6972 6573 2d44 6973 743a  0.Requires-Dist:
-00000730: 2068 7474 7078 3e3d 302e 3233 2e30 0a52   httpx>=0.23.0.R
-00000740: 6571 7569 7265 732d 4469 7374 3a20 6a69  equires-Dist: ji
-00000750: 6e6a 6132 3e3d 322e 3131 2e32 0a52 6571  nja2>=2.11.2.Req
-00000760: 7569 7265 732d 4469 7374 3a20 7079 7468  uires-Dist: pyth
-00000770: 6f6e 2d6d 756c 7469 7061 7274 3e3d 302e  on-multipart>=0.
-00000780: 302e 370a 5265 7175 6972 6573 2d44 6973  0.7.Requires-Dis
-00000790: 743a 2075 6a73 6f6e 213d 342e 302e 322c  t: ujson!=4.0.2,
-000007a0: 213d 342e 312e 302c 213d 342e 322e 302c  !=4.1.0,!=4.2.0,
-000007b0: 213d 342e 332e 302c 213d 352e 302e 302c  !=4.3.0,!=5.0.0,
-000007c0: 213d 352e 312e 302c 3e3d 342e 302e 310a  !=5.1.0,>=4.0.1.
-000007d0: 5265 7175 6972 6573 2d44 6973 743a 206f  Requires-Dist: o
-000007e0: 726a 736f 6e3e 3d33 2e32 2e31 0a52 6571  rjson>=3.2.1.Req
-000007f0: 7569 7265 732d 4469 7374 3a20 656d 6169  uires-Dist: emai
-00000800: 6c5f 7661 6c69 6461 746f 723e 3d32 2e30  l_validator>=2.0
-00000810: 2e30 0a52 6571 7569 7265 732d 4469 7374  .0.Requires-Dist
-00000820: 3a20 7576 6963 6f72 6e5b 7374 616e 6461  : uvicorn[standa
-00000830: 7264 5d3e 3d30 2e31 322e 300a 5265 7175  rd]>=0.12.0.Requ
-00000840: 6972 6573 2d44 6973 743a 2068 7474 7078  ires-Dist: httpx
-00000850: 3e3d 302e 3233 2e30 3b20 6578 7472 6120  >=0.23.0; extra 
-00000860: 3d3d 2022 616c 6c22 0a52 6571 7569 7265  == "all".Require
-00000870: 732d 4469 7374 3a20 6a69 6e6a 6132 3e3d  s-Dist: jinja2>=
-00000880: 322e 3131 2e32 3b20 6578 7472 6120 3d3d  2.11.2; extra ==
-00000890: 2022 616c 6c22 0a52 6571 7569 7265 732d   "all".Requires-
-000008a0: 4469 7374 3a20 7079 7468 6f6e 2d6d 756c  Dist: python-mul
-000008b0: 7469 7061 7274 3e3d 302e 302e 373b 2065  tipart>=0.0.7; e
-000008c0: 7874 7261 203d 3d20 2261 6c6c 220a 5265  xtra == "all".Re
-000008d0: 7175 6972 6573 2d44 6973 743a 2069 7473  quires-Dist: its
-000008e0: 6461 6e67 6572 6f75 733e 3d31 2e31 2e30  dangerous>=1.1.0
-000008f0: 3b20 6578 7472 6120 3d3d 2022 616c 6c22  ; extra == "all"
-00000900: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
-00000910: 7079 7961 6d6c 3e3d 352e 332e 313b 2065  pyyaml>=5.3.1; e
-00000920: 7874 7261 203d 3d20 2261 6c6c 220a 5265  xtra == "all".Re
-00000930: 7175 6972 6573 2d44 6973 743a 2075 6a73  quires-Dist: ujs
-00000940: 6f6e 213d 342e 302e 322c 213d 342e 312e  on!=4.0.2,!=4.1.
-00000950: 302c 213d 342e 322e 302c 213d 342e 332e  0,!=4.2.0,!=4.3.
-00000960: 302c 213d 352e 302e 302c 213d 352e 312e  0,!=5.0.0,!=5.1.
-00000970: 302c 3e3d 342e 302e 313b 2065 7874 7261  0,>=4.0.1; extra
-00000980: 203d 3d20 2261 6c6c 220a 5265 7175 6972   == "all".Requir
-00000990: 6573 2d44 6973 743a 206f 726a 736f 6e3e  es-Dist: orjson>
-000009a0: 3d33 2e32 2e31 3b20 6578 7472 6120 3d3d  =3.2.1; extra ==
-000009b0: 2022 616c 6c22 0a52 6571 7569 7265 732d   "all".Requires-
-000009c0: 4469 7374 3a20 656d 6169 6c5f 7661 6c69  Dist: email_vali
-000009d0: 6461 746f 723e 3d32 2e30 2e30 3b20 6578  dator>=2.0.0; ex
-000009e0: 7472 6120 3d3d 2022 616c 6c22 0a52 6571  tra == "all".Req
-000009f0: 7569 7265 732d 4469 7374 3a20 7576 6963  uires-Dist: uvic
-00000a00: 6f72 6e5b 7374 616e 6461 7264 5d3e 3d30  orn[standard]>=0
-00000a10: 2e31 322e 303b 2065 7874 7261 203d 3d20  .12.0; extra == 
-00000a20: 2261 6c6c 220a 5265 7175 6972 6573 2d44  "all".Requires-D
-00000a30: 6973 743a 2070 7964 616e 7469 632d 7365  ist: pydantic-se
-00000a40: 7474 696e 6773 3e3d 322e 302e 303b 2065  ttings>=2.0.0; e
-00000a50: 7874 7261 203d 3d20 2261 6c6c 220a 5265  xtra == "all".Re
-00000a60: 7175 6972 6573 2d44 6973 743a 2070 7964  quires-Dist: pyd
-00000a70: 616e 7469 632d 6578 7472 612d 7479 7065  antic-extra-type
-00000a80: 733e 3d32 2e30 2e30 3b20 6578 7472 6120  s>=2.0.0; extra 
-00000a90: 3d3d 2022 616c 6c22 0a50 726f 7669 6465  == "all".Provide
-00000aa0: 732d 4578 7472 613a 2061 6c6c 0a44 6573  s-Extra: all.Des
-00000ab0: 6372 6970 7469 6f6e 2d43 6f6e 7465 6e74  cription-Content
-00000ac0: 2d54 7970 653a 2074 6578 742f 6d61 726b  -Type: text/mark
-00000ad0: 646f 776e 0a0a 3c70 2061 6c69 676e 3d22  down..<p align="
-00000ae0: 6365 6e74 6572 223e 0a20 203c 6120 6872  center">.  <a hr
-00000af0: 6566 3d22 6874 7470 733a 2f2f 7265 6164  ef="https://read
-00000b00: 7961 7069 2e6b 6875 6c6e 6173 6f66 742e  yapi.khulnasoft.
-00000b10: 636f 6d22 3e3c 696d 6720 7372 633d 2268  com"><img src="h
-00000b20: 7474 7073 3a2f 2f72 6561 6479 6170 692e  ttps://readyapi.
-00000b30: 6b68 756c 6e61 736f 6674 2e63 6f6d 2f69  khulnasoft.com/i
-00000b40: 6d67 2f6c 6f67 6f2d 6d61 7267 696e 2f6c  mg/logo-margin/l
-00000b50: 6f67 6f2d 7465 616c 2e70 6e67 2220 616c  ogo-teal.png" al
-00000b60: 743d 2252 6561 6479 4150 4922 3e3c 2f61  t="ReadyAPI"></a
-00000b70: 3e0a 3c2f 703e 0a3c 7020 616c 6967 6e3d  >.</p>.<p align=
-00000b80: 2263 656e 7465 7222 3e0a 2020 2020 3c65  "center">.    <e
-00000b90: 6d3e 5265 6164 7941 5049 2066 7261 6d65  m>ReadyAPI frame
-00000ba0: 776f 726b 2c20 6869 6768 2070 6572 666f  work, high perfo
-00000bb0: 726d 616e 6365 2c20 6561 7379 2074 6f20  rmance, easy to 
-00000bc0: 6c65 6172 6e2c 2066 6173 7420 746f 2063  learn, fast to c
-00000bd0: 6f64 652c 2072 6561 6479 2066 6f72 2070  ode, ready for p
-00000be0: 726f 6475 6374 696f 6e3c 2f65 6d3e 0a3c  roduction</em>.<
-00000bf0: 2f70 3e0a 3c70 2061 6c69 676e 3d22 6365  /p>.<p align="ce
-00000c00: 6e74 6572 223e 0a3c 6120 6872 6566 3d22  nter">.<a href="
-00000c10: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000c20: 6f6d 2f6b 6875 6c6e 6173 6f66 742f 7265  om/khulnasoft/re
-00000c30: 6164 7961 7069 2f61 6374 696f 6e73 3f71  adyapi/actions?q
-00000c40: 7565 7279 3d77 6f72 6b66 6c6f 7725 3341  uery=workflow%3A
-00000c50: 5465 7374 2b65 7665 6e74 2533 4170 7573  Test+event%3Apus
-00000c60: 682b 6272 616e 6368 2533 416d 6173 7465  h+branch%3Amaste
-00000c70: 7222 2074 6172 6765 743d 225f 626c 616e  r" target="_blan
-00000c80: 6b22 3e0a 2020 2020 3c69 6d67 2073 7263  k">.    <img src
-00000c90: 3d22 6874 7470 733a 2f2f 6769 7468 7562  ="https://github
-00000ca0: 2e63 6f6d 2f6b 6875 6c6e 6173 6f66 742f  .com/khulnasoft/
-00000cb0: 7265 6164 7961 7069 2f77 6f72 6b66 6c6f  readyapi/workflo
-00000cc0: 7773 2f54 6573 742f 6261 6467 652e 7376  ws/Test/badge.sv
-00000cd0: 673f 6576 656e 743d 7075 7368 2662 7261  g?event=push&bra
-00000ce0: 6e63 683d 6d61 7374 6572 2220 616c 743d  nch=master" alt=
-00000cf0: 2254 6573 7422 3e0a 3c2f 613e 0a3c 6120  "Test">.</a>.<a 
-00000d00: 6872 6566 3d22 6874 7470 733a 2f2f 636f  href="https://co
-00000d10: 7665 7261 6765 2d62 6164 6765 2e73 616d  verage-badge.sam
-00000d20: 7565 6c63 6f6c 7669 6e2e 776f 726b 6572  uelcolvin.worker
-00000d30: 732e 6465 762f 7265 6469 7265 6374 2f6b  s.dev/redirect/k
-00000d40: 6875 6c6e 6173 6f66 742f 7265 6164 7961  hulnasoft/readya
-00000d50: 7069 2220 7461 7267 6574 3d22 5f62 6c61  pi" target="_bla
-00000d60: 6e6b 223e 0a20 2020 203c 696d 6720 7372  nk">.    <img sr
-00000d70: 633d 2268 7474 7073 3a2f 2f63 6f76 6572  c="https://cover
-00000d80: 6167 652d 6261 6467 652e 7361 6d75 656c  age-badge.samuel
-00000d90: 636f 6c76 696e 2e77 6f72 6b65 7273 2e64  colvin.workers.d
-00000da0: 6576 2f6b 6875 6c6e 6173 6f66 742f 7265  ev/khulnasoft/re
-00000db0: 6164 7961 7069 2e73 7667 2220 616c 743d  adyapi.svg" alt=
-00000dc0: 2243 6f76 6572 6167 6522 3e0a 3c2f 613e  "Coverage">.</a>
-00000dd0: 0a3c 6120 6872 6566 3d22 6874 7470 733a  .<a href="https:
-00000de0: 2f2f 7079 7069 2e6f 7267 2f70 726f 6a65  //pypi.org/proje
-00000df0: 6374 2f72 6561 6479 6170 6922 2074 6172  ct/readyapi" tar
-00000e00: 6765 743d 225f 626c 616e 6b22 3e0a 2020  get="_blank">.  
-00000e10: 2020 3c69 6d67 2073 7263 3d22 6874 7470    <img src="http
-00000e20: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
-00000e30: 696f 2f70 7970 692f 762f 7265 6164 7961  io/pypi/v/readya
-00000e40: 7069 3f63 6f6c 6f72 3d25 3233 3334 4430  pi?color=%2334D0
-00000e50: 3538 266c 6162 656c 3d70 7970 6925 3230  58&label=pypi%20
-00000e60: 7061 636b 6167 6522 2061 6c74 3d22 5061  package" alt="Pa
-00000e70: 636b 6167 6520 7665 7273 696f 6e22 3e0a  ckage version">.
-00000e80: 3c2f 613e 0a3c 6120 6872 6566 3d22 6874  </a>.<a href="ht
-00000e90: 7470 733a 2f2f 7079 7069 2e6f 7267 2f70  tps://pypi.org/p
-00000ea0: 726f 6a65 6374 2f72 6561 6479 6170 6922  roject/readyapi"
-00000eb0: 2074 6172 6765 743d 225f 626c 616e 6b22   target="_blank"
-00000ec0: 3e0a 2020 2020 3c69 6d67 2073 7263 3d22  >.    <img src="
-00000ed0: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
-00000ee0: 6c64 732e 696f 2f70 7970 692f 7079 7665  lds.io/pypi/pyve
-00000ef0: 7273 696f 6e73 2f72 6561 6479 6170 692e  rsions/readyapi.
-00000f00: 7376 673f 636f 6c6f 723d 2532 3333 3444  svg?color=%2334D
-00000f10: 3035 3822 2061 6c74 3d22 5375 7070 6f72  058" alt="Suppor
-00000f20: 7465 6420 5079 7468 6f6e 2076 6572 7369  ted Python versi
-00000f30: 6f6e 7322 3e0a 3c2f 613e 0a3c 2f70 3e0a  ons">.</a>.</p>.
-00000f40: 0a2d 2d2d 0a0a 2a2a 446f 6375 6d65 6e74  .---..**Document
-00000f50: 6174 696f 6e2a 2a3a 203c 6120 6872 6566  ation**: <a href
-00000f60: 3d22 6874 7470 733a 2f2f 7265 6164 7961  ="https://readya
-00000f70: 7069 2e6b 6875 6c6e 6173 6f66 742e 636f  pi.khulnasoft.co
-00000f80: 6d22 2074 6172 6765 743d 225f 626c 616e  m" target="_blan
-00000f90: 6b22 3e68 7474 7073 3a2f 2f72 6561 6479  k">https://ready
-00000fa0: 6170 692e 6b68 756c 6e61 736f 6674 2e63  api.khulnasoft.c
-00000fb0: 6f6d 3c2f 613e 0a0a 2a2a 536f 7572 6365  om</a>..**Source
-00000fc0: 2043 6f64 652a 2a3a 203c 6120 6872 6566   Code**: <a href
-00000fd0: 3d22 6874 7470 733a 2f2f 6769 7468 7562  ="https://github
-00000fe0: 2e63 6f6d 2f6b 6875 6c6e 6173 6f66 742f  .com/khulnasoft/
-00000ff0: 7265 6164 7961 7069 2220 7461 7267 6574  readyapi" target
-00001000: 3d22 5f62 6c61 6e6b 223e 6874 7470 733a  ="_blank">https:
-00001010: 2f2f 6769 7468 7562 2e63 6f6d 2f6b 6875  //github.com/khu
-00001020: 6c6e 6173 6f66 742f 7265 6164 7961 7069  lnasoft/readyapi
-00001030: 3c2f 613e 0a0a 2d2d 2d0a 5265 6164 7941  </a>..---.ReadyA
-00001040: 5049 2069 7320 6120 6d6f 6465 726e 2c20  PI is a modern, 
-00001050: 6661 7374 2028 6869 6768 2d70 6572 666f  fast (high-perfo
-00001060: 726d 616e 6365 292c 2077 6562 2066 7261  rmance), web fra
-00001070: 6d65 776f 726b 2066 6f72 2062 7569 6c64  mework for build
-00001080: 696e 6720 4150 4973 2077 6974 6820 5079  ing APIs with Py
-00001090: 7468 6f6e 2033 2e38 2b20 6261 7365 6420  thon 3.8+ based 
-000010a0: 6f6e 2073 7461 6e64 6172 6420 5079 7468  on standard Pyth
-000010b0: 6f6e 2074 7970 6520 6869 6e74 732e 0a0a  on type hints...
-000010c0: 5468 6520 6b65 7920 6665 6174 7572 6573  The key features
-000010d0: 2061 7265 3a0a 0a2a 202a 2a46 6173 742a   are:..* **Fast*
-000010e0: 2a3a 2056 6572 7920 6869 6768 2070 6572  *: Very high per
-000010f0: 666f 726d 616e 6365 2c20 6f6e 2070 6172  formance, on par
-00001100: 2077 6974 6820 2a2a 4e6f 6465 4a53 2a2a   with **NodeJS**
-00001110: 2061 6e64 202a 2a47 6f2a 2a20 2874 6861   and **Go** (tha
-00001120: 6e6b 7320 746f 2053 7461 726c 6574 7465  nks to Starlette
-00001130: 2061 6e64 2050 7964 616e 7469 6329 2e20   and Pydantic). 
-00001140: 5b4f 6e65 206f 6620 7468 6520 6661 7374  [One of the fast
-00001150: 6573 7420 5079 7468 6f6e 2066 7261 6d65  est Python frame
-00001160: 776f 726b 7320 6176 6169 6c61 626c 655d  works available]
-00001170: 2823 7065 7266 6f72 6d61 6e63 6529 2e0a  (#performance)..
-00001180: 2a20 2a2a 4661 7374 2074 6f20 636f 6465  * **Fast to code
-00001190: 2a2a 3a20 496e 6372 6561 7365 2074 6865  **: Increase the
-000011a0: 2073 7065 6564 2074 6f20 6465 7665 6c6f   speed to develo
-000011b0: 7020 6665 6174 7572 6573 2062 7920 6162  p features by ab
-000011c0: 6f75 7420 3230 3025 2074 6f20 3330 3025  out 200% to 300%
-000011d0: 2e20 2a0a 2a20 2a2a 4665 7765 7220 6275  . *.* **Fewer bu
-000011e0: 6773 2a2a 3a20 5265 6475 6365 2061 626f  gs**: Reduce abo
-000011f0: 7574 2034 3025 206f 6620 6875 6d61 6e20  ut 40% of human 
-00001200: 2864 6576 656c 6f70 6572 2920 696e 6475  (developer) indu
-00001210: 6365 6420 6572 726f 7273 2e20 2a0a 2a20  ced errors. *.* 
-00001220: 2a2a 496e 7475 6974 6976 652a 2a3a 2047  **Intuitive**: G
-00001230: 7265 6174 2065 6469 746f 7220 7375 7070  reat editor supp
-00001240: 6f72 742e 203c 6162 6272 2074 6974 6c65  ort. <abbr title
-00001250: 3d22 616c 736f 206b 6e6f 776e 2061 7320  ="also known as 
-00001260: 6175 746f 2d63 6f6d 706c 6574 652c 2061  auto-complete, a
-00001270: 7574 6f63 6f6d 706c 6574 696f 6e2c 2049  utocompletion, I
-00001280: 6e74 656c 6c69 5365 6e73 6522 3e43 6f6d  ntelliSense">Com
-00001290: 706c 6574 696f 6e3c 2f61 6262 723e 2065  pletion</abbr> e
-000012a0: 7665 7279 7768 6572 652e 204c 6573 7320  verywhere. Less 
-000012b0: 7469 6d65 2064 6562 7567 6769 6e67 2e0a  time debugging..
-000012c0: 2a20 2a2a 4561 7379 2a2a 3a20 4465 7369  * **Easy**: Desi
-000012d0: 676e 6564 2074 6f20 6265 2065 6173 7920  gned to be easy 
-000012e0: 746f 2075 7365 2061 6e64 206c 6561 726e  to use and learn
-000012f0: 2e20 4c65 7373 2074 696d 6520 7265 6164  . Less time read
-00001300: 696e 6720 646f 6373 2e0a 2a20 2a2a 5368  ing docs..* **Sh
-00001310: 6f72 742a 2a3a 204d 696e 696d 697a 6520  ort**: Minimize 
-00001320: 636f 6465 2064 7570 6c69 6361 7469 6f6e  code duplication
-00001330: 2e20 4d75 6c74 6970 6c65 2066 6561 7475  . Multiple featu
-00001340: 7265 7320 6672 6f6d 2065 6163 6820 7061  res from each pa
-00001350: 7261 6d65 7465 7220 6465 636c 6172 6174  rameter declarat
-00001360: 696f 6e2e 2046 6577 6572 2062 7567 732e  ion. Fewer bugs.
-00001370: 0a2a 202a 2a52 6f62 7573 742a 2a3a 2047  .* **Robust**: G
-00001380: 6574 2070 726f 6475 6374 696f 6e2d 7265  et production-re
-00001390: 6164 7920 636f 6465 2e20 5769 7468 2061  ady code. With a
-000013a0: 7574 6f6d 6174 6963 2069 6e74 6572 6163  utomatic interac
-000013b0: 7469 7665 2064 6f63 756d 656e 7461 7469  tive documentati
-000013c0: 6f6e 2e0a 2a20 2a2a 5374 616e 6461 7264  on..* **Standard
-000013d0: 732d 6261 7365 642a 2a3a 2042 6173 6564  s-based**: Based
-000013e0: 206f 6e20 2861 6e64 2066 756c 6c79 2063   on (and fully c
-000013f0: 6f6d 7061 7469 626c 6520 7769 7468 2920  ompatible with) 
-00001400: 7468 6520 6f70 656e 2073 7461 6e64 6172  the open standar
-00001410: 6473 2066 6f72 2041 5049 733a 203c 6120  ds for APIs: <a 
-00001420: 6872 6566 3d22 6874 7470 733a 2f2f 6769  href="https://gi
-00001430: 7468 7562 2e63 6f6d 2f4f 4149 2f4f 7065  thub.com/OAI/Ope
-00001440: 6e41 5049 2d53 7065 6369 6669 6361 7469  nAPI-Specificati
-00001450: 6f6e 2220 636c 6173 733d 2265 7874 6572  on" class="exter
-00001460: 6e61 6c2d 6c69 6e6b 2220 7461 7267 6574  nal-link" target
-00001470: 3d22 5f62 6c61 6e6b 223e 4f70 656e 4150  ="_blank">OpenAP
-00001480: 493c 2f61 3e20 2870 7265 7669 6f75 736c  I</a> (previousl
-00001490: 7920 6b6e 6f77 6e20 6173 2053 7761 6767  y known as Swagg
-000014a0: 6572 2920 616e 6420 3c61 2068 7265 663d  er) and <a href=
-000014b0: 2268 7474 7073 3a2f 2f6a 736f 6e2d 7363  "https://json-sc
-000014c0: 6865 6d61 2e6f 7267 2f22 2063 6c61 7373  hema.org/" class
-000014d0: 3d22 6578 7465 726e 616c 2d6c 696e 6b22  ="external-link"
-000014e0: 2074 6172 6765 743d 225f 626c 616e 6b22   target="_blank"
-000014f0: 3e4a 534f 4e20 5363 6865 6d61 3c2f 613e  >JSON Schema</a>
-00001500: 2e0a 0a3c 736d 616c 6c3e 2a20 6573 7469  ...<small>* esti
-00001510: 6d61 7469 6f6e 2062 6173 6564 206f 6e20  mation based on 
-00001520: 7465 7374 7320 6f6e 2061 6e20 696e 7465  tests on an inte
-00001530: 726e 616c 2064 6576 656c 6f70 6d65 6e74  rnal development
-00001540: 2074 6561 6d2c 2062 7569 6c64 696e 6720   team, building 
-00001550: 7072 6f64 7563 7469 6f6e 2061 7070 6c69  production appli
-00001560: 6361 7469 6f6e 732e 3c2f 736d 616c 6c3e  cations.</small>
-00001570: 0a0a 2323 2053 706f 6e73 6f72 730a 0a3c  ..## Sponsors..<
-00001580: 212d 2d20 7370 6f6e 736f 7273 202d 2d3e  !-- sponsors -->
-00001590: 0a0a 3c61 2068 7265 663d 2268 7474 7073  ..<a href="https
-000015a0: 3a2f 2f63 7279 7074 6170 692e 696f 2f22  ://cryptapi.io/"
-000015b0: 2074 6172 6765 743d 225f 626c 616e 6b22   target="_blank"
-000015c0: 2074 6974 6c65 3d22 4372 7970 7441 5049   title="CryptAPI
-000015d0: 3a20 596f 7572 2065 6173 7920 746f 2075  : Your easy to u
-000015e0: 7365 2c20 7365 6375 7265 2061 6e64 2070  se, secure and p
-000015f0: 7269 7661 6379 206f 7269 656e 7465 6420  rivacy oriented 
-00001600: 7061 796d 656e 7420 6761 7465 7761 792e  payment gateway.
-00001610: 223e 3c69 6d67 2073 7263 3d22 6874 7470  "><img src="http
-00001620: 733a 2f2f 7265 6164 7961 7069 2e6b 6875  s://readyapi.khu
-00001630: 6c6e 6173 6f66 742e 636f 6d2f 696d 672f  lnasoft.com/img/
-00001640: 7370 6f6e 736f 7273 2f63 7279 7074 6170  sponsors/cryptap
-00001650: 692e 7376 6722 3e3c 2f61 3e0a 3c61 2068  i.svg"></a>.<a h
-00001660: 7265 663d 2268 7474 7073 3a2f 2f70 6c61  ref="https://pla
-00001670: 7466 6f72 6d2e 7368 2f74 7279 2d69 742d  tform.sh/try-it-
-00001680: 6e6f 772f 3f75 746d 5f73 6f75 7263 653d  now/?utm_source=
-00001690: 7265 6164 7961 7069 2d73 6967 6e75 7026  readyapi-signup&
-000016a0: 7574 6d5f 6d65 6469 756d 3d62 616e 6e65  utm_medium=banne
-000016b0: 7226 7574 6d5f 6361 6d70 6169 676e 3d52  r&utm_campaign=R
-000016c0: 6561 6479 4150 492d 7369 676e 7570 2d4a  eadyAPI-signup-J
-000016d0: 756e 652d 3230 3233 2220 7461 7267 6574  une-2023" target
-000016e0: 3d22 5f62 6c61 6e6b 2220 7469 746c 653d  ="_blank" title=
-000016f0: 2242 7569 6c64 2c20 7275 6e20 616e 6420  "Build, run and 
-00001700: 7363 616c 6520 796f 7572 2061 7070 7320  scale your apps 
-00001710: 6f6e 2061 206d 6f64 6572 6e2c 2072 656c  on a modern, rel
-00001720: 6961 626c 652c 2061 6e64 2073 6563 7572  iable, and secur
-00001730: 6520 5061 6153 2e22 3e3c 696d 6720 7372  e PaaS."><img sr
-00001740: 633d 2268 7474 7073 3a2f 2f72 6561 6479  c="https://ready
-00001750: 6170 692e 6b68 756c 6e61 736f 6674 2e63  api.khulnasoft.c
-00001760: 6f6d 2f69 6d67 2f73 706f 6e73 6f72 732f  om/img/sponsors/
-00001770: 706c 6174 666f 726d 2d73 682e 706e 6722  platform-sh.png"
-00001780: 3e3c 2f61 3e0a 3c61 2068 7265 663d 2268  ></a>.<a href="h
-00001790: 7474 7073 3a2f 2f77 7777 2e70 6f72 7465  ttps://www.porte
-000017a0: 722e 7275 6e22 2074 6172 6765 743d 225f  r.run" target="_
-000017b0: 626c 616e 6b22 2074 6974 6c65 3d22 4465  blank" title="De
-000017c0: 706c 6f79 2052 6561 6479 4150 4920 6f6e  ploy ReadyAPI on
-000017d0: 2041 5753 2077 6974 6820 6120 6665 7720   AWS with a few 
-000017e0: 636c 6963 6b73 223e 3c69 6d67 2073 7263  clicks"><img src
-000017f0: 3d22 6874 7470 733a 2f2f 7265 6164 7961  ="https://readya
-00001800: 7069 2e6b 6875 6c6e 6173 6f66 742e 636f  pi.khulnasoft.co
-00001810: 6d2f 696d 672f 7370 6f6e 736f 7273 2f70  m/img/sponsors/p
-00001820: 6f72 7465 722e 706e 6722 3e3c 2f61 3e0a  orter.png"></a>.
-00001830: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
-00001840: 2f62 756d 702e 7368 2f72 6561 6479 6170  /bump.sh/readyap
-00001850: 693f 7574 6d5f 736f 7572 6365 3d72 6561  i?utm_source=rea
-00001860: 6479 6170 6926 7574 6d5f 6d65 6469 756d  dyapi&utm_medium
-00001870: 3d72 6566 6572 7261 6c26 7574 6d5f 6361  =referral&utm_ca
-00001880: 6d70 6169 676e 3d73 706f 6e73 6f72 2220  mpaign=sponsor" 
-00001890: 7461 7267 6574 3d22 5f62 6c61 6e6b 2220  target="_blank" 
-000018a0: 7469 746c 653d 2241 7574 6f6d 6174 6520  title="Automate 
-000018b0: 5265 6164 7941 5049 2064 6f63 756d 656e  ReadyAPI documen
-000018c0: 7461 7469 6f6e 2067 656e 6572 6174 696f  tation generatio
-000018d0: 6e20 7769 7468 2042 756d 702e 7368 223e  n with Bump.sh">
-000018e0: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
-000018f0: 2f2f 7265 6164 7961 7069 2e6b 6875 6c6e  //readyapi.khuln
-00001900: 6173 6f66 742e 636f 6d2f 696d 672f 7370  asoft.com/img/sp
-00001910: 6f6e 736f 7273 2f62 756d 702d 7368 2e73  onsors/bump-sh.s
-00001920: 7667 223e 3c2f 613e 0a3c 6120 6872 6566  vg"></a>.<a href
-00001930: 3d22 6874 7470 733a 2f2f 7265 666c 6578  ="https://reflex
-00001940: 2e64 6576 2220 7461 7267 6574 3d22 5f62  .dev" target="_b
-00001950: 6c61 6e6b 2220 7469 746c 653d 2252 6566  lank" title="Ref
-00001960: 6c65 7822 3e3c 696d 6720 7372 633d 2268  lex"><img src="h
-00001970: 7474 7073 3a2f 2f72 6561 6479 6170 692e  ttps://readyapi.
-00001980: 6b68 756c 6e61 736f 6674 2e63 6f6d 2f69  khulnasoft.com/i
-00001990: 6d67 2f73 706f 6e73 6f72 732f 7265 666c  mg/sponsors/refl
-000019a0: 6578 2e70 6e67 223e 3c2f 613e 0a3c 6120  ex.png"></a>.<a 
-000019b0: 6872 6566 3d22 6874 7470 733a 2f2f 6769  href="https://gi
-000019c0: 7468 7562 2e63 6f6d 2f73 6361 6c61 722f  thub.com/scalar/
-000019d0: 7363 616c 6172 2f3f 7574 6d5f 736f 7572  scalar/?utm_sour
-000019e0: 6365 3d72 6561 6479 6170 6926 7574 6d5f  ce=readyapi&utm_
-000019f0: 6d65 6469 756d 3d77 6562 7369 7465 2675  medium=website&u
-00001a00: 746d 5f63 616d 7061 6967 6e3d 6d61 696e  tm_campaign=main
-00001a10: 2d62 6164 6765 2220 7461 7267 6574 3d22  -badge" target="
-00001a20: 5f62 6c61 6e6b 2220 7469 746c 653d 2253  _blank" title="S
-00001a30: 6361 6c61 723a 2042 6561 7574 6966 756c  calar: Beautiful
-00001a40: 204f 7065 6e2d 536f 7572 6365 2041 5049   Open-Source API
-00001a50: 2052 6566 6572 656e 6365 7320 6672 6f6d   References from
-00001a60: 2053 7761 6767 6572 2f4f 7065 6e41 5049   Swagger/OpenAPI
-00001a70: 2066 696c 6573 223e 3c69 6d67 2073 7263   files"><img src
-00001a80: 3d22 6874 7470 733a 2f2f 7265 6164 7961  ="https://readya
-00001a90: 7069 2e6b 6875 6c6e 6173 6f66 742e 636f  pi.khulnasoft.co
-00001aa0: 6d2f 696d 672f 7370 6f6e 736f 7273 2f73  m/img/sponsors/s
-00001ab0: 6361 6c61 722e 7376 6722 3e3c 2f61 3e0a  calar.svg"></a>.
-00001ac0: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
-00001ad0: 2f77 7777 2e70 726f 7065 6c61 7574 682e  /www.propelauth.
-00001ae0: 636f 6d2f 3f75 746d 5f73 6f75 7263 653d  com/?utm_source=
-00001af0: 7265 6164 7961 7069 2675 746d 5f63 616d  readyapi&utm_cam
-00001b00: 7061 6967 6e3d 3132 3233 2675 746d 5f6d  paign=1223&utm_m
-00001b10: 6564 6975 6d3d 6d61 696e 6261 6467 6522  edium=mainbadge"
-00001b20: 2074 6172 6765 743d 225f 626c 616e 6b22   target="_blank"
-00001b30: 2074 6974 6c65 3d22 4175 7468 2c20 7573   title="Auth, us
-00001b40: 6572 206d 616e 6167 656d 656e 7420 616e  er management an
-00001b50: 6420 6d6f 7265 2066 6f72 2079 6f75 7220  d more for your 
-00001b60: 4232 4220 7072 6f64 7563 7422 3e3c 696d  B2B product"><im
-00001b70: 6720 7372 633d 2268 7474 7073 3a2f 2f72  g src="https://r
-00001b80: 6561 6479 6170 692e 6b68 756c 6e61 736f  eadyapi.khulnaso
-00001b90: 6674 2e63 6f6d 2f69 6d67 2f73 706f 6e73  ft.com/img/spons
-00001ba0: 6f72 732f 7072 6f70 656c 6175 7468 2e70  ors/propelauth.p
-00001bb0: 6e67 223e 3c2f 613e 0a3c 6120 6872 6566  ng"></a>.<a href
-00001bc0: 3d22 6874 7470 733a 2f2f 7777 772e 7769  ="https://www.wi
-00001bd0: 7468 636f 6865 7265 6e63 652e 636f 6d2f  thcoherence.com/
-00001be0: 3f75 746d 5f6d 6564 6975 6d3d 6164 7665  ?utm_medium=adve
-00001bf0: 7274 6973 696e 6726 7574 6d5f 736f 7572  rtising&utm_sour
-00001c00: 6365 3d72 6561 6479 6170 6926 7574 6d5f  ce=readyapi&utm_
-00001c10: 6361 6d70 6169 676e 3d62 616e 6e65 7225  campaign=banner%
-00001c20: 3230 6a61 6e75 6172 7925 3230 3234 2220  20january%2024" 
-00001c30: 7461 7267 6574 3d22 5f62 6c61 6e6b 2220  target="_blank" 
-00001c40: 7469 746c 653d 2243 6f68 6572 656e 6365  title="Coherence
-00001c50: 223e 3c69 6d67 2073 7263 3d22 6874 7470  "><img src="http
-00001c60: 733a 2f2f 7265 6164 7961 7069 2e6b 6875  s://readyapi.khu
-00001c70: 6c6e 6173 6f66 742e 636f 6d2f 696d 672f  lnasoft.com/img/
-00001c80: 7370 6f6e 736f 7273 2f63 6f68 6572 656e  sponsors/coheren
-00001c90: 6365 2e70 6e67 223e 3c2f 613e 0a3c 6120  ce.png"></a>.<a 
-00001ca0: 6872 6566 3d22 6874 7470 733a 2f2f 7777  href="https://ww
-00001cb0: 772e 6d6f 6e67 6f64 622e 636f 6d2f 6465  w.mongodb.com/de
-00001cc0: 7665 6c6f 7065 722f 6c61 6e67 7561 6765  veloper/language
-00001cd0: 732f 7079 7468 6f6e 2f70 7974 686f 6e2d  s/python/python-
-00001ce0: 7175 6963 6b73 7461 7274 2d72 6561 6479  quickstart-ready
-00001cf0: 6170 692f 3f75 746d 5f63 616d 7061 6967  api/?utm_campaig
-00001d00: 6e3d 7265 6164 7961 7069 5f66 7261 6d65  n=readyapi_frame
-00001d10: 776f 726b 2675 746d 5f73 6f75 7263 653d  work&utm_source=
-00001d20: 7265 6164 7961 7069 5f73 706f 6e73 6f72  readyapi_sponsor
-00001d30: 7368 6970 2675 746d 5f6d 6564 6975 6d3d  ship&utm_medium=
-00001d40: 7765 625f 7265 6665 7272 616c 2220 7461  web_referral" ta
-00001d50: 7267 6574 3d22 5f62 6c61 6e6b 2220 7469  rget="_blank" ti
-00001d60: 746c 653d 2253 696d 706c 6966 7920 4675  tle="Simplify Fu
-00001d70: 6c6c 2053 7461 636b 2044 6576 656c 6f70  ll Stack Develop
-00001d80: 6d65 6e74 2077 6974 6820 5265 6164 7941  ment with ReadyA
-00001d90: 5049 2026 204d 6f6e 676f 4442 223e 3c69  PI & MongoDB"><i
-00001da0: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
-00001db0: 7265 6164 7961 7069 2e6b 6875 6c6e 6173  readyapi.khulnas
-00001dc0: 6f66 742e 636f 6d2f 696d 672f 7370 6f6e  oft.com/img/spon
-00001dd0: 736f 7273 2f6d 6f6e 676f 6462 2e70 6e67  sors/mongodb.png
-00001de0: 223e 3c2f 613e 0a3c 6120 6872 6566 3d22  "></a>.<a href="
-00001df0: 6874 7470 733a 2f2f 7472 6169 6e69 6e67  https://training
-00001e00: 2e74 616c 6b70 7974 686f 6e2e 666d 2f72  .talkpython.fm/r
-00001e10: 6561 6479 6170 692d 636f 7572 7365 7322  eadyapi-courses"
-00001e20: 2074 6172 6765 743d 225f 626c 616e 6b22   target="_blank"
-00001e30: 2074 6974 6c65 3d22 5265 6164 7941 5049   title="ReadyAPI
-00001e40: 2076 6964 656f 2063 6f75 7273 6573 206f   video courses o
-00001e50: 6e20 6465 6d61 6e64 2066 726f 6d20 7065  n demand from pe
-00001e60: 6f70 6c65 2079 6f75 2074 7275 7374 223e  ople you trust">
-00001e70: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
-00001e80: 2f2f 7265 6164 7961 7069 2e6b 6875 6c6e  //readyapi.khuln
-00001e90: 6173 6f66 742e 636f 6d2f 696d 672f 7370  asoft.com/img/sp
-00001ea0: 6f6e 736f 7273 2f74 616c 6b70 7974 686f  onsors/talkpytho
-00001eb0: 6e2d 7632 2e6a 7067 223e 3c2f 613e 0a3c  n-v2.jpg"></a>.<
-00001ec0: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
-00001ed0: 6769 7468 7562 2e63 6f6d 2f64 6565 7073  github.com/deeps
-00001ee0: 6574 2d61 692f 6861 7973 7461 636b 2f22  et-ai/haystack/"
-00001ef0: 2074 6172 6765 743d 225f 626c 616e 6b22   target="_blank"
-00001f00: 2074 6974 6c65 3d22 4275 696c 6420 706f   title="Build po
-00001f10: 7765 7266 756c 2073 6561 7263 6820 6672  werful search fr
-00001f20: 6f6d 2063 6f6d 706f 7361 626c 652c 206f  om composable, o
-00001f30: 7065 6e20 736f 7572 6365 2062 7569 6c64  pen source build
-00001f40: 696e 6720 626c 6f63 6b73 223e 3c69 6d67  ing blocks"><img
-00001f50: 2073 7263 3d22 6874 7470 733a 2f2f 7265   src="https://re
-00001f60: 6164 7961 7069 2e6b 6875 6c6e 6173 6f66  adyapi.khulnasof
-00001f70: 742e 636f 6d2f 696d 672f 7370 6f6e 736f  t.com/img/sponso
-00001f80: 7273 2f68 6179 7374 6163 6b2d 7265 6164  rs/haystack-read
-00001f90: 7961 7069 2e73 7667 223e 3c2f 613e 0a3c  yapi.svg"></a>.<
-00001fa0: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
-00001fb0: 6461 7461 6265 6e74 6f2e 636f 6d2f 2220  databento.com/" 
-00001fc0: 7461 7267 6574 3d22 5f62 6c61 6e6b 2220  target="_blank" 
-00001fd0: 7469 746c 653d 2250 6179 2061 7320 796f  title="Pay as yo
-00001fe0: 7520 676f 2066 6f72 206d 6172 6b65 7420  u go for market 
-00001ff0: 6461 7461 223e 3c69 6d67 2073 7263 3d22  data"><img src="
-00002000: 6874 7470 733a 2f2f 7265 6164 7961 7069  https://readyapi
-00002010: 2e6b 6875 6c6e 6173 6f66 742e 636f 6d2f  .khulnasoft.com/
-00002020: 696d 672f 7370 6f6e 736f 7273 2f64 6174  img/sponsors/dat
-00002030: 6162 656e 746f 2e73 7667 223e 3c2f 613e  abento.svg"></a>
-00002040: 0a3c 6120 6872 6566 3d22 6874 7470 733a  .<a href="https:
-00002050: 2f2f 7370 6561 6b65 6173 7961 7069 2e64  //speakeasyapi.d
-00002060: 6576 3f75 746d 5f73 6f75 7263 653d 7265  ev?utm_source=re
-00002070: 6164 7961 7069 2b72 6570 6f26 7574 6d5f  adyapi+repo&utm_
-00002080: 6d65 6469 756d 3d67 6974 6875 622b 7370  medium=github+sp
-00002090: 6f6e 736f 7273 6869 7022 2074 6172 6765  onsorship" targe
-000020a0: 743d 225f 626c 616e 6b22 2074 6974 6c65  t="_blank" title
-000020b0: 3d22 5344 4b73 2066 6f72 2079 6f75 7220  ="SDKs for your 
-000020c0: 4150 4920 7c20 5370 6561 6b65 6173 7922  API | Speakeasy"
-000020d0: 3e3c 696d 6720 7372 633d 2268 7474 7073  ><img src="https
-000020e0: 3a2f 2f72 6561 6479 6170 692e 6b68 756c  ://readyapi.khul
-000020f0: 6e61 736f 6674 2e63 6f6d 2f69 6d67 2f73  nasoft.com/img/s
-00002100: 706f 6e73 6f72 732f 7370 6561 6b65 6173  ponsors/speakeas
-00002110: 792e 706e 6722 3e3c 2f61 3e0a 3c61 2068  y.png"></a>.<a h
-00002120: 7265 663d 2268 7474 7073 3a2f 2f77 7777  ref="https://www
-00002130: 2e73 7669 782e 636f 6d2f 2220 7461 7267  .svix.com/" targ
-00002140: 6574 3d22 5f62 6c61 6e6b 2220 7469 746c  et="_blank" titl
-00002150: 653d 2253 7669 7820 2d20 5765 6268 6f6f  e="Svix - Webhoo
-00002160: 6b73 2061 7320 6120 7365 7276 6963 6522  ks as a service"
-00002170: 3e3c 696d 6720 7372 633d 2268 7474 7073  ><img src="https
-00002180: 3a2f 2f72 6561 6479 6170 692e 6b68 756c  ://readyapi.khul
-00002190: 6e61 736f 6674 2e63 6f6d 2f69 6d67 2f73  nasoft.com/img/s
-000021a0: 706f 6e73 6f72 732f 7376 6978 2e73 7667  ponsors/svix.svg
-000021b0: 223e 3c2f 613e 0a3c 6120 6872 6566 3d22  "></a>.<a href="
-000021c0: 6874 7470 733a 2f2f 7777 772e 636f 6461  https://www.coda
-000021d0: 6379 2e63 6f6d 2f3f 7574 6d5f 736f 7572  cy.com/?utm_sour
-000021e0: 6365 3d67 6974 6875 6226 7574 6d5f 6d65  ce=github&utm_me
-000021f0: 6469 756d 3d73 706f 6e73 6f72 7326 7574  dium=sponsors&ut
-00002200: 6d5f 6964 3d70 696f 6e65 6572 7322 2074  m_id=pioneers" t
-00002210: 6172 6765 743d 225f 626c 616e 6b22 2074  arget="_blank" t
-00002220: 6974 6c65 3d22 5461 6b65 2063 6f64 6520  itle="Take code 
-00002230: 7265 7669 6577 7320 6672 6f6d 2068 6f75  reviews from hou
-00002240: 7273 2074 6f20 6d69 6e75 7465 7322 3e3c  rs to minutes"><
-00002250: 696d 6720 7372 633d 2268 7474 7073 3a2f  img src="https:/
-00002260: 2f72 6561 6479 6170 692e 6b68 756c 6e61  /readyapi.khulna
-00002270: 736f 6674 2e63 6f6d 2f69 6d67 2f73 706f  soft.com/img/spo
-00002280: 6e73 6f72 732f 636f 6461 6379 2e70 6e67  nsors/codacy.png
-00002290: 223e 3c2f 613e 0a0a 3c21 2d2d 202f 7370  "></a>..<!-- /sp
-000022a0: 6f6e 736f 7273 202d 2d3e 0a0a 3c61 2068  onsors -->..<a h
-000022b0: 7265 663d 2268 7474 7073 3a2f 2f72 6561  ref="https://rea
-000022c0: 6479 6170 692e 6b68 756c 6e61 736f 6674  dyapi.khulnasoft
-000022d0: 2e63 6f6d 2f72 6561 6479 6170 692d 7065  .com/readyapi-pe
-000022e0: 6f70 6c65 2f23 7370 6f6e 736f 7273 2220  ople/#sponsors" 
-000022f0: 636c 6173 733d 2265 7874 6572 6e61 6c2d  class="external-
-00002300: 6c69 6e6b 2220 7461 7267 6574 3d22 5f62  link" target="_b
-00002310: 6c61 6e6b 223e 4f74 6865 7220 7370 6f6e  lank">Other spon
-00002320: 736f 7273 3c2f 613e 0a0a 2323 204f 7069  sors</a>..## Opi
-00002330: 6e69 6f6e 730a 0a22 5f5b 2e2e 2e5d 2049  nions.."_[...] I
-00002340: 276d 2075 7369 6e67 202a 2a52 6561 6479  'm using **Ready
-00002350: 4150 492a 2a20 6120 746f 6e20 7468 6573  API** a ton thes
-00002360: 6520 6461 7973 2e20 5b2e 2e2e 5d20 4927  e days. [...] I'
-00002370: 6d20 6163 7475 616c 6c79 2070 6c61 6e6e  m actually plann
-00002380: 696e 6720 746f 2075 7365 2069 7420 666f  ing to use it fo
-00002390: 7220 616c 6c20 6f66 206d 7920 7465 616d  r all of my team
-000023a0: 2773 202a 2a4d 4c20 7365 7276 6963 6573  's **ML services
-000023b0: 2061 7420 4d69 6372 6f73 6f66 742a 2a2e   at Microsoft**.
-000023c0: 2053 6f6d 6520 6f66 2074 6865 6d20 6172   Some of them ar
-000023d0: 6520 6765 7474 696e 6720 696e 7465 6772  e getting integr
-000023e0: 6174 6564 2069 6e74 6f20 7468 6520 636f  ated into the co
-000023f0: 7265 202a 2a57 696e 646f 7773 2a2a 2070  re **Windows** p
-00002400: 726f 6475 6374 2061 6e64 2073 6f6d 6520  roduct and some 
-00002410: 2a2a 4f66 6669 6365 2a2a 2070 726f 6475  **Office** produ
-00002420: 6374 732e 5f22 0a0a 3c64 6976 2073 7479  cts._"..<div sty
-00002430: 6c65 3d22 7465 7874 2d61 6c69 676e 3a20  le="text-align: 
-00002440: 7269 6768 743b 206d 6172 6769 6e2d 7269  right; margin-ri
-00002450: 6768 743a 2031 3025 3b22 3e4b 6162 6972  ght: 10%;">Kabir
-00002460: 204b 6861 6e20 2d20 3c73 7472 6f6e 673e   Khan - <strong>
-00002470: 4d69 6372 6f73 6f66 743c 2f73 7472 6f6e  Microsoft</stron
-00002480: 673e 203c 6120 6872 6566 3d22 6874 7470  g> <a href="http
-00002490: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6b  s://github.com/k
-000024a0: 6875 6c6e 6173 6f66 742f 7265 6164 7961  hulnasoft/readya
-000024b0: 7069 2f70 756c 6c2f 3236 2220 7461 7267  pi/pull/26" targ
-000024c0: 6574 3d22 5f62 6c61 6e6b 223e 3c73 6d61  et="_blank"><sma
-000024d0: 6c6c 3e28 7265 6629 3c2f 736d 616c 6c3e  ll>(ref)</small>
-000024e0: 3c2f 613e 3c2f 6469 763e 0a0a 2d2d 2d0a  </a></div>..---.
-000024f0: 0a22 5f57 6520 6164 6f70 7465 6420 7468  ."_We adopted th
-00002500: 6520 2a2a 5265 6164 7941 5049 2a2a 206c  e **ReadyAPI** l
-00002510: 6962 7261 7279 2074 6f20 7370 6177 6e20  ibrary to spawn 
-00002520: 6120 2a2a 5245 5354 2a2a 2073 6572 7665  a **REST** serve
-00002530: 7220 7468 6174 2063 616e 2062 6520 7175  r that can be qu
-00002540: 6572 6965 6420 746f 206f 6274 6169 6e20  eried to obtain 
-00002550: 2a2a 7072 6564 6963 7469 6f6e 732a 2a2e  **predictions**.
-00002560: 205b 666f 7220 4c75 6477 6967 5d5f 220a   [for Ludwig]_".
-00002570: 0a3c 6469 7620 7374 796c 653d 2274 6578  .<div style="tex
-00002580: 742d 616c 6967 6e3a 2072 6967 6874 3b20  t-align: right; 
-00002590: 6d61 7267 696e 2d72 6967 6874 3a20 3130  margin-right: 10
-000025a0: 253b 223e 5069 6572 6f20 4d6f 6c69 6e6f  %;">Piero Molino
-000025b0: 2c20 5961 726f 736c 6176 2044 7564 696e  , Yaroslav Dudin
-000025c0: 2c20 616e 6420 5361 6920 5375 6d61 6e74  , and Sai Sumant
-000025d0: 6820 4d69 7279 616c 6120 2d20 3c73 7472  h Miryala - <str
-000025e0: 6f6e 673e 5562 6572 3c2f 7374 726f 6e67  ong>Uber</strong
-000025f0: 3e20 3c61 2068 7265 663d 2268 7474 7073  > <a href="https
-00002600: 3a2f 2f65 6e67 2e75 6265 722e 636f 6d2f  ://eng.uber.com/
-00002610: 6c75 6477 6967 2d76 302d 322f 2220 7461  ludwig-v0-2/" ta
-00002620: 7267 6574 3d22 5f62 6c61 6e6b 223e 3c73  rget="_blank"><s
-00002630: 6d61 6c6c 3e28 7265 6629 3c2f 736d 616c  mall>(ref)</smal
-00002640: 6c3e 3c2f 613e 3c2f 6469 763e 0a0a 2d2d  l></a></div>..--
-00002650: 2d0a 0a22 5f2a 2a4e 6574 666c 6978 2a2a  -.."_**Netflix**
-00002660: 2069 7320 706c 6561 7365 6420 746f 2061   is pleased to a
-00002670: 6e6e 6f75 6e63 6520 7468 6520 6f70 656e  nnounce the open
-00002680: 2d73 6f75 7263 6520 7265 6c65 6173 6520  -source release 
-00002690: 6f66 206f 7572 202a 2a63 7269 7369 7320  of our **crisis 
-000026a0: 6d61 6e61 6765 6d65 6e74 2a2a 206f 7263  management** orc
-000026b0: 6865 7374 7261 7469 6f6e 2066 7261 6d65  hestration frame
-000026c0: 776f 726b 3a20 2a2a 4469 7370 6174 6368  work: **Dispatch
-000026d0: 2a2a 2120 5b62 7569 6c74 2077 6974 6820  **! [built with 
-000026e0: 2a2a 5265 6164 7941 5049 2a2a 5d5f 220a  **ReadyAPI**]_".
-000026f0: 0a3c 6469 7620 7374 796c 653d 2274 6578  .<div style="tex
-00002700: 742d 616c 6967 6e3a 2072 6967 6874 3b20  t-align: right; 
-00002710: 6d61 7267 696e 2d72 6967 6874 3a20 3130  margin-right: 10
-00002720: 253b 223e 4b65 7669 6e20 476c 6973 736f  %;">Kevin Glisso
-00002730: 6e2c 204d 6172 6320 5669 6c61 6e6f 7661  n, Marc Vilanova
-00002740: 2c20 466f 7265 7374 204d 6f6e 7365 6e20  , Forest Monsen 
-00002750: 2d20 3c73 7472 6f6e 673e 4e65 7466 6c69  - <strong>Netfli
-00002760: 783c 2f73 7472 6f6e 673e 203c 6120 6872  x</strong> <a hr
-00002770: 6566 3d22 6874 7470 733a 2f2f 6e65 7466  ef="https://netf
-00002780: 6c69 7874 6563 6862 6c6f 672e 636f 6d2f  lixtechblog.com/
-00002790: 696e 7472 6f64 7563 696e 672d 6469 7370  introducing-disp
-000027a0: 6174 6368 2d64 6134 6238 6132 6138 3037  atch-da4b8a2a807
-000027b0: 3222 2074 6172 6765 743d 225f 626c 616e  2" target="_blan
-000027c0: 6b22 3e3c 736d 616c 6c3e 2872 6566 293c  k"><small>(ref)<
-000027d0: 2f73 6d61 6c6c 3e3c 2f61 3e3c 2f64 6976  /small></a></div
-000027e0: 3e0a 0a2d 2d2d 0a0a 225f 49e2 8099 6d20  >..---.."_I...m 
-000027f0: 6f76 6572 2074 6865 206d 6f6f 6e20 6578  over the moon ex
-00002800: 6369 7465 6420 6162 6f75 7420 2a2a 5265  cited about **Re
-00002810: 6164 7941 5049 2a2a 2e20 4974 e280 9973  adyAPI**. It...s
-00002820: 2073 6f20 6675 6e21 5f22 0a0a 3c64 6976   so fun!_"..<div
-00002830: 2073 7479 6c65 3d22 7465 7874 2d61 6c69   style="text-ali
-00002840: 676e 3a20 7269 6768 743b 206d 6172 6769  gn: right; margi
-00002850: 6e2d 7269 6768 743a 2031 3025 3b22 3e42  n-right: 10%;">B
-00002860: 7269 616e 204f 6b6b 656e 202d 203c 7374  rian Okken - <st
-00002870: 726f 6e67 3e3c 6120 6872 6566 3d22 6874  rong><a href="ht
-00002880: 7470 733a 2f2f 7079 7468 6f6e 6279 7465  tps://pythonbyte
-00002890: 732e 666d 2f65 7069 736f 6465 732f 7368  s.fm/episodes/sh
-000028a0: 6f77 2f31 3233 2f74 696d 652d 746f 2d72  ow/123/time-to-r
-000028b0: 6967 6874 2d74 6865 2d70 792d 7772 6f6e  ight-the-py-wron
-000028c0: 6773 3f74 696d 655f 696e 5f73 6563 3d38  gs?time_in_sec=8
-000028d0: 3535 2220 7461 7267 6574 3d22 5f62 6c61  55" target="_bla
-000028e0: 6e6b 223e 5079 7468 6f6e 2042 7974 6573  nk">Python Bytes
-000028f0: 3c2f 613e 2070 6f64 6361 7374 2068 6f73  </a> podcast hos
-00002900: 743c 2f73 7472 6f6e 673e 203c 6120 6872  t</strong> <a hr
-00002910: 6566 3d22 6874 7470 733a 2f2f 7477 6974  ef="https://twit
-00002920: 7465 722e 636f 6d2f 6272 6961 6e6f 6b6b  ter.com/brianokk
-00002930: 656e 2f73 7461 7475 732f 3131 3132 3232  en/status/111222
-00002940: 3030 3739 3937 3237 3238 3833 3222 2074  0079972728832" t
-00002950: 6172 6765 743d 225f 626c 616e 6b22 3e3c  arget="_blank"><
-00002960: 736d 616c 6c3e 2872 6566 293c 2f73 6d61  small>(ref)</sma
-00002970: 6c6c 3e3c 2f61 3e3c 2f64 6976 3e0a 0a2d  ll></a></div>..-
-00002980: 2d2d 0a0a 225f 486f 6e65 7374 6c79 2c20  --.."_Honestly, 
-00002990: 7768 6174 2079 6f75 2776 6520 6275 696c  what you've buil
-000029a0: 7420 6c6f 6f6b 7320 7375 7065 7220 736f  t looks super so
-000029b0: 6c69 6420 616e 6420 706f 6c69 7368 6564  lid and polished
-000029c0: 2e20 496e 206d 616e 7920 7761 7973 2c20  . In many ways, 
-000029d0: 6974 2773 2077 6861 7420 4920 7761 6e74  it's what I want
-000029e0: 6564 202a 2a48 7567 2a2a 2074 6f20 6265  ed **Hug** to be
-000029f0: 202d 2069 7427 7320 7265 616c 6c79 2069   - it's really i
-00002a00: 6e73 7069 7269 6e67 2074 6f20 7365 6520  nspiring to see 
-00002a10: 736f 6d65 6f6e 6520 6275 696c 6420 7468  someone build th
-00002a20: 6174 2e5f 220a 0a3c 6469 7620 7374 796c  at._"..<div styl
-00002a30: 653d 2274 6578 742d 616c 6967 6e3a 2072  e="text-align: r
-00002a40: 6967 6874 3b20 6d61 7267 696e 2d72 6967  ight; margin-rig
-00002a50: 6874 3a20 3130 253b 223e 5469 6d6f 7468  ht: 10%;">Timoth
-00002a60: 7920 4372 6f73 6c65 7920 2d20 3c73 7472  y Crosley - <str
-00002a70: 6f6e 673e 3c61 2068 7265 663d 2268 7474  ong><a href="htt
-00002a80: 7073 3a2f 2f77 7777 2e68 7567 2e72 6573  ps://www.hug.res
-00002a90: 742f 2220 7461 7267 6574 3d22 5f62 6c61  t/" target="_bla
-00002aa0: 6e6b 223e 4875 673c 2f61 3e20 6372 6561  nk">Hug</a> crea
-00002ab0: 746f 723c 2f73 7472 6f6e 673e 203c 6120  tor</strong> <a 
-00002ac0: 6872 6566 3d22 6874 7470 733a 2f2f 6e65  href="https://ne
-00002ad0: 7773 2e79 636f 6d62 696e 6174 6f72 2e63  ws.ycombinator.c
-00002ae0: 6f6d 2f69 7465 6d3f 6964 3d31 3934 3535  om/item?id=19455
-00002af0: 3436 3522 2074 6172 6765 743d 225f 626c  465" target="_bl
-00002b00: 616e 6b22 3e3c 736d 616c 6c3e 2872 6566  ank"><small>(ref
-00002b10: 293c 2f73 6d61 6c6c 3e3c 2f61 3e3c 2f64  )</small></a></d
-00002b20: 6976 3e0a 0a2d 2d2d 0a0a 225f 4966 2079  iv>..---.."_If y
-00002b30: 6f75 2772 6520 6c6f 6f6b 696e 6720 746f  ou're looking to
-00002b40: 206c 6561 726e 206f 6e65 202a 2a6d 6f64   learn one **mod
-00002b50: 6572 6e20 6672 616d 6577 6f72 6b2a 2a20  ern framework** 
-00002b60: 666f 7220 6275 696c 6469 6e67 2052 4553  for building RES
-00002b70: 5420 4150 4973 2c20 6368 6563 6b20 6f75  T APIs, check ou
-00002b80: 7420 2a2a 5265 6164 7941 5049 2a2a 205b  t **ReadyAPI** [
-00002b90: 2e2e 2e5d 2049 7427 7320 6661 7374 2c20  ...] It's fast, 
-00002ba0: 6561 7379 2074 6f20 7573 6520 616e 6420  easy to use and 
-00002bb0: 6561 7379 2074 6f20 6c65 6172 6e20 5b2e  easy to learn [.
-00002bc0: 2e2e 5d5f 220a 0a22 5f57 6527 7665 2073  ..]_".."_We've s
-00002bd0: 7769 7463 6865 6420 6f76 6572 2074 6f20  witched over to 
-00002be0: 2a2a 5265 6164 7941 5049 2a2a 2066 6f72  **ReadyAPI** for
-00002bf0: 206f 7572 202a 2a41 5049 732a 2a20 5b2e   our **APIs** [.
-00002c00: 2e2e 5d20 4920 7468 696e 6b20 796f 7527  ..] I think you'
-00002c10: 6c6c 206c 696b 6520 6974 205b 2e2e 2e5d  ll like it [...]
-00002c20: 5f22 0a0a 3c64 6976 2073 7479 6c65 3d22  _"..<div style="
-00002c30: 7465 7874 2d61 6c69 676e 3a20 7269 6768  text-align: righ
-00002c40: 743b 206d 6172 6769 6e2d 7269 6768 743a  t; margin-right:
-00002c50: 2031 3025 3b22 3e49 6e65 7320 4d6f 6e74   10%;">Ines Mont
-00002c60: 616e 6920 2d20 4d61 7474 6865 7720 486f  ani - Matthew Ho
-00002c70: 6e6e 6962 616c 202d 203c 7374 726f 6e67  nnibal - <strong
-00002c80: 3e3c 6120 6872 6566 3d22 6874 7470 733a  ><a href="https:
-00002c90: 2f2f 6578 706c 6f73 696f 6e2e 6169 2220  //explosion.ai" 
+00000000: 3c70 2061 6c69 676e 3d22 6365 6e74 6572  <p align="center
+00000010: 223e 0a20 203c 6120 6872 6566 3d22 6874  ">.  <a href="ht
+00000020: 7470 733a 2f2f 7265 6164 7961 7069 2e6b  tps://readyapi.k
+00000030: 6875 6c6e 6173 6f66 742e 636f 6d22 3e3c  hulnasoft.com"><
+00000040: 696d 6720 7372 633d 2268 7474 7073 3a2f  img src="https:/
+00000050: 2f72 6561 6479 6170 692e 6b68 756c 6e61  /readyapi.khulna
+00000060: 736f 6674 2e63 6f6d 2f69 6d67 2f6c 6f67  soft.com/img/log
+00000070: 6f2d 6d61 7267 696e 2f6c 6f67 6f2d 7465  o-margin/logo-te
+00000080: 616c 2e70 6e67 2220 616c 743d 2252 6561  al.png" alt="Rea
+00000090: 6479 4150 4922 3e3c 2f61 3e0a 3c2f 703e  dyAPI"></a>.</p>
+000000a0: 0a3c 7020 616c 6967 6e3d 2263 656e 7465  .<p align="cente
+000000b0: 7222 3e0a 2020 2020 3c65 6d3e 5265 6164  r">.    <em>Read
+000000c0: 7941 5049 2066 7261 6d65 776f 726b 2c20  yAPI framework, 
+000000d0: 6869 6768 2070 6572 666f 726d 616e 6365  high performance
+000000e0: 2c20 6561 7379 2074 6f20 6c65 6172 6e2c  , easy to learn,
+000000f0: 2066 6173 7420 746f 2063 6f64 652c 2072   fast to code, r
+00000100: 6561 6479 2066 6f72 2070 726f 6475 6374  eady for product
+00000110: 696f 6e3c 2f65 6d3e 0a3c 2f70 3e0a 3c70  ion</em>.</p>.<p
+00000120: 2061 6c69 676e 3d22 6365 6e74 6572 223e   align="center">
+00000130: 0a3c 6120 6872 6566 3d22 6874 7470 733a  .<a href="https:
+00000140: 2f2f 6769 7468 7562 2e63 6f6d 2f6b 6875  //github.com/khu
+00000150: 6c6e 6173 6f66 742f 7265 6164 7961 7069  lnasoft/readyapi
+00000160: 2f61 6374 696f 6e73 3f71 7565 7279 3d77  /actions?query=w
+00000170: 6f72 6b66 6c6f 7725 3341 5465 7374 2b65  orkflow%3ATest+e
+00000180: 7665 6e74 2533 4170 7573 682b 6272 616e  vent%3Apush+bran
+00000190: 6368 2533 416d 6173 7465 7222 2074 6172  ch%3Amaster" tar
+000001a0: 6765 743d 225f 626c 616e 6b22 3e0a 2020  get="_blank">.  
+000001b0: 2020 3c69 6d67 2073 7263 3d22 6874 7470    <img src="http
+000001c0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6b  s://github.com/k
+000001d0: 6875 6c6e 6173 6f66 742f 7265 6164 7961  hulnasoft/readya
+000001e0: 7069 2f77 6f72 6b66 6c6f 7773 2f54 6573  pi/workflows/Tes
+000001f0: 742f 6261 6467 652e 7376 673f 6576 656e  t/badge.svg?even
+00000200: 743d 7075 7368 2662 7261 6e63 683d 6d61  t=push&branch=ma
+00000210: 7374 6572 2220 616c 743d 2254 6573 7422  ster" alt="Test"
+00000220: 3e0a 3c2f 613e 0a3c 6120 6872 6566 3d22  >.</a>.<a href="
+00000230: 6874 7470 733a 2f2f 636f 7665 7261 6765  https://coverage
+00000240: 2d62 6164 6765 2e73 616d 7565 6c63 6f6c  -badge.samuelcol
+00000250: 7669 6e2e 776f 726b 6572 732e 6465 762f  vin.workers.dev/
+00000260: 7265 6469 7265 6374 2f6b 6875 6c6e 6173  redirect/khulnas
+00000270: 6f66 742f 7265 6164 7961 7069 2220 7461  oft/readyapi" ta
+00000280: 7267 6574 3d22 5f62 6c61 6e6b 223e 0a20  rget="_blank">. 
+00000290: 2020 203c 696d 6720 7372 633d 2268 7474     <img src="htt
+000002a0: 7073 3a2f 2f63 6f76 6572 6167 652d 6261  ps://coverage-ba
+000002b0: 6467 652e 7361 6d75 656c 636f 6c76 696e  dge.samuelcolvin
+000002c0: 2e77 6f72 6b65 7273 2e64 6576 2f6b 6875  .workers.dev/khu
+000002d0: 6c6e 6173 6f66 742f 7265 6164 7961 7069  lnasoft/readyapi
+000002e0: 2e73 7667 2220 616c 743d 2243 6f76 6572  .svg" alt="Cover
+000002f0: 6167 6522 3e0a 3c2f 613e 0a3c 6120 6872  age">.</a>.<a hr
+00000300: 6566 3d22 6874 7470 733a 2f2f 7079 7069  ef="https://pypi
+00000310: 2e6f 7267 2f70 726f 6a65 6374 2f72 6561  .org/project/rea
+00000320: 6479 6170 6922 2074 6172 6765 743d 225f  dyapi" target="_
+00000330: 626c 616e 6b22 3e0a 2020 2020 3c69 6d67  blank">.    <img
+00000340: 2073 7263 3d22 6874 7470 733a 2f2f 696d   src="https://im
+00000350: 672e 7368 6965 6c64 732e 696f 2f70 7970  g.shields.io/pyp
+00000360: 692f 762f 7265 6164 7961 7069 3f63 6f6c  i/v/readyapi?col
+00000370: 6f72 3d25 3233 3334 4430 3538 266c 6162  or=%2334D058&lab
+00000380: 656c 3d70 7970 6925 3230 7061 636b 6167  el=pypi%20packag
+00000390: 6522 2061 6c74 3d22 5061 636b 6167 6520  e" alt="Package 
+000003a0: 7665 7273 696f 6e22 3e0a 3c2f 613e 0a3c  version">.</a>.<
+000003b0: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
+000003c0: 7079 7069 2e6f 7267 2f70 726f 6a65 6374  pypi.org/project
+000003d0: 2f72 6561 6479 6170 6922 2074 6172 6765  /readyapi" targe
+000003e0: 743d 225f 626c 616e 6b22 3e0a 2020 2020  t="_blank">.    
+000003f0: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
+00000400: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
+00000410: 2f70 7970 692f 7079 7665 7273 696f 6e73  /pypi/pyversions
+00000420: 2f72 6561 6479 6170 692e 7376 673f 636f  /readyapi.svg?co
+00000430: 6c6f 723d 2532 3333 3444 3035 3822 2061  lor=%2334D058" a
+00000440: 6c74 3d22 5375 7070 6f72 7465 6420 5079  lt="Supported Py
+00000450: 7468 6f6e 2076 6572 7369 6f6e 7322 3e0a  thon versions">.
+00000460: 3c2f 613e 0a3c 2f70 3e0a 0a2d 2d2d 0a0a  </a>.</p>..---..
+00000470: 2a2a 446f 6375 6d65 6e74 6174 696f 6e2a  **Documentation*
+00000480: 2a3a 203c 6120 6872 6566 3d22 6874 7470  *: <a href="http
+00000490: 733a 2f2f 7265 6164 7961 7069 2e6b 6875  s://readyapi.khu
+000004a0: 6c6e 6173 6f66 742e 636f 6d22 2074 6172  lnasoft.com" tar
+000004b0: 6765 743d 225f 626c 616e 6b22 3e68 7474  get="_blank">htt
+000004c0: 7073 3a2f 2f72 6561 6479 6170 692e 6b68  ps://readyapi.kh
+000004d0: 756c 6e61 736f 6674 2e63 6f6d 3c2f 613e  ulnasoft.com</a>
+000004e0: 0a0a 2a2a 536f 7572 6365 2043 6f64 652a  ..**Source Code*
+000004f0: 2a3a 203c 6120 6872 6566 3d22 6874 7470  *: <a href="http
+00000500: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6b  s://github.com/k
+00000510: 6875 6c6e 6173 6f66 742f 7265 6164 7961  hulnasoft/readya
+00000520: 7069 2220 7461 7267 6574 3d22 5f62 6c61  pi" target="_bla
+00000530: 6e6b 223e 6874 7470 733a 2f2f 6769 7468  nk">https://gith
+00000540: 7562 2e63 6f6d 2f6b 6875 6c6e 6173 6f66  ub.com/khulnasof
+00000550: 742f 7265 6164 7961 7069 3c2f 613e 0a0a  t/readyapi</a>..
+00000560: 2d2d 2d0a 0a52 6561 6479 4150 4920 6973  ---..ReadyAPI is
+00000570: 2061 206d 6f64 6572 6e2c 2066 6173 7420   a modern, fast 
+00000580: 2868 6967 682d 7065 7266 6f72 6d61 6e63  (high-performanc
+00000590: 6529 2c20 7765 6220 6672 616d 6577 6f72  e), web framewor
+000005a0: 6b20 666f 7220 6275 696c 6469 6e67 2041  k for building A
+000005b0: 5049 7320 7769 7468 2050 7974 686f 6e20  PIs with Python 
+000005c0: 6261 7365 6420 6f6e 2073 7461 6e64 6172  based on standar
+000005d0: 6420 5079 7468 6f6e 2074 7970 6520 6869  d Python type hi
+000005e0: 6e74 732e 0a0a 5468 6520 6b65 7920 6665  nts...The key fe
+000005f0: 6174 7572 6573 2061 7265 3a0a 0a2a 202a  atures are:..* *
+00000600: 2a46 6173 742a 2a3a 2056 6572 7920 6869  *Fast**: Very hi
+00000610: 6768 2070 6572 666f 726d 616e 6365 2c20  gh performance, 
+00000620: 6f6e 2070 6172 2077 6974 6820 2a2a 4e6f  on par with **No
+00000630: 6465 4a53 2a2a 2061 6e64 202a 2a47 6f2a  deJS** and **Go*
+00000640: 2a20 2874 6861 6e6b 7320 746f 2053 7461  * (thanks to Sta
+00000650: 726c 6574 7465 2061 6e64 2050 7964 616e  rlette and Pydan
+00000660: 7469 6329 2e20 5b4f 6e65 206f 6620 7468  tic). [One of th
+00000670: 6520 6661 7374 6573 7420 5079 7468 6f6e  e fastest Python
+00000680: 2066 7261 6d65 776f 726b 7320 6176 6169   frameworks avai
+00000690: 6c61 626c 655d 2823 7065 7266 6f72 6d61  lable](#performa
+000006a0: 6e63 6529 2e0a 2a20 2a2a 4661 7374 2074  nce)..* **Fast t
+000006b0: 6f20 636f 6465 2a2a 3a20 496e 6372 6561  o code**: Increa
+000006c0: 7365 2074 6865 2073 7065 6564 2074 6f20  se the speed to 
+000006d0: 6465 7665 6c6f 7020 6665 6174 7572 6573  develop features
+000006e0: 2062 7920 6162 6f75 7420 3230 3025 2074   by about 200% t
+000006f0: 6f20 3330 3025 2e20 2a0a 2a20 2a2a 4665  o 300%. *.* **Fe
+00000700: 7765 7220 6275 6773 2a2a 3a20 5265 6475  wer bugs**: Redu
+00000710: 6365 2061 626f 7574 2034 3025 206f 6620  ce about 40% of 
+00000720: 6875 6d61 6e20 2864 6576 656c 6f70 6572  human (developer
+00000730: 2920 696e 6475 6365 6420 6572 726f 7273  ) induced errors
+00000740: 2e20 2a0a 2a20 2a2a 496e 7475 6974 6976  . *.* **Intuitiv
+00000750: 652a 2a3a 2047 7265 6174 2065 6469 746f  e**: Great edito
+00000760: 7220 7375 7070 6f72 742e 203c 6162 6272  r support. <abbr
+00000770: 2074 6974 6c65 3d22 616c 736f 206b 6e6f   title="also kno
+00000780: 776e 2061 7320 6175 746f 2d63 6f6d 706c  wn as auto-compl
+00000790: 6574 652c 2061 7574 6f63 6f6d 706c 6574  ete, autocomplet
+000007a0: 696f 6e2c 2049 6e74 656c 6c69 5365 6e73  ion, IntelliSens
+000007b0: 6522 3e43 6f6d 706c 6574 696f 6e3c 2f61  e">Completion</a
+000007c0: 6262 723e 2065 7665 7279 7768 6572 652e  bbr> everywhere.
+000007d0: 204c 6573 7320 7469 6d65 2064 6562 7567   Less time debug
+000007e0: 6769 6e67 2e0a 2a20 2a2a 4561 7379 2a2a  ging..* **Easy**
+000007f0: 3a20 4465 7369 676e 6564 2074 6f20 6265  : Designed to be
+00000800: 2065 6173 7920 746f 2075 7365 2061 6e64   easy to use and
+00000810: 206c 6561 726e 2e20 4c65 7373 2074 696d   learn. Less tim
+00000820: 6520 7265 6164 696e 6720 646f 6373 2e0a  e reading docs..
+00000830: 2a20 2a2a 5368 6f72 742a 2a3a 204d 696e  * **Short**: Min
+00000840: 696d 697a 6520 636f 6465 2064 7570 6c69  imize code dupli
+00000850: 6361 7469 6f6e 2e20 4d75 6c74 6970 6c65  cation. Multiple
+00000860: 2066 6561 7475 7265 7320 6672 6f6d 2065   features from e
+00000870: 6163 6820 7061 7261 6d65 7465 7220 6465  ach parameter de
+00000880: 636c 6172 6174 696f 6e2e 2046 6577 6572  claration. Fewer
+00000890: 2062 7567 732e 0a2a 202a 2a52 6f62 7573   bugs..* **Robus
+000008a0: 742a 2a3a 2047 6574 2070 726f 6475 6374  t**: Get product
+000008b0: 696f 6e2d 7265 6164 7920 636f 6465 2e20  ion-ready code. 
+000008c0: 5769 7468 2061 7574 6f6d 6174 6963 2069  With automatic i
+000008d0: 6e74 6572 6163 7469 7665 2064 6f63 756d  nteractive docum
+000008e0: 656e 7461 7469 6f6e 2e0a 2a20 2a2a 5374  entation..* **St
+000008f0: 616e 6461 7264 732d 6261 7365 642a 2a3a  andards-based**:
+00000900: 2042 6173 6564 206f 6e20 2861 6e64 2066   Based on (and f
+00000910: 756c 6c79 2063 6f6d 7061 7469 626c 6520  ully compatible 
+00000920: 7769 7468 2920 7468 6520 6f70 656e 2073  with) the open s
+00000930: 7461 6e64 6172 6473 2066 6f72 2041 5049  tandards for API
+00000940: 733a 203c 6120 6872 6566 3d22 6874 7470  s: <a href="http
+00000950: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f4f  s://github.com/O
+00000960: 4149 2f4f 7065 6e41 5049 2d53 7065 6369  AI/OpenAPI-Speci
+00000970: 6669 6361 7469 6f6e 2220 636c 6173 733d  fication" class=
+00000980: 2265 7874 6572 6e61 6c2d 6c69 6e6b 2220  "external-link" 
+00000990: 7461 7267 6574 3d22 5f62 6c61 6e6b 223e  target="_blank">
+000009a0: 4f70 656e 4150 493c 2f61 3e20 2870 7265  OpenAPI</a> (pre
+000009b0: 7669 6f75 736c 7920 6b6e 6f77 6e20 6173  viously known as
+000009c0: 2053 7761 6767 6572 2920 616e 6420 3c61   Swagger) and <a
+000009d0: 2068 7265 663d 2268 7474 7073 3a2f 2f6a   href="https://j
+000009e0: 736f 6e2d 7363 6865 6d61 2e6f 7267 2f22  son-schema.org/"
+000009f0: 2063 6c61 7373 3d22 6578 7465 726e 616c   class="external
+00000a00: 2d6c 696e 6b22 2074 6172 6765 743d 225f  -link" target="_
+00000a10: 626c 616e 6b22 3e4a 534f 4e20 5363 6865  blank">JSON Sche
+00000a20: 6d61 3c2f 613e 2e0a 0a3c 736d 616c 6c3e  ma</a>...<small>
+00000a30: 2a20 6573 7469 6d61 7469 6f6e 2062 6173  * estimation bas
+00000a40: 6564 206f 6e20 7465 7374 7320 6f6e 2061  ed on tests on a
+00000a50: 6e20 696e 7465 726e 616c 2064 6576 656c  n internal devel
+00000a60: 6f70 6d65 6e74 2074 6561 6d2c 2062 7569  opment team, bui
+00000a70: 6c64 696e 6720 7072 6f64 7563 7469 6f6e  lding production
+00000a80: 2061 7070 6c69 6361 7469 6f6e 732e 3c2f   applications.</
+00000a90: 736d 616c 6c3e 0a0a 2323 2053 706f 6e73  small>..## Spons
+00000aa0: 6f72 730a 0a3c 212d 2d20 7370 6f6e 736f  ors..<!-- sponso
+00000ab0: 7273 202d 2d3e 0a0a 7b25 2069 6620 7370  rs -->..{% if sp
+00000ac0: 6f6e 736f 7273 2025 7d0a 7b25 2066 6f72  onsors %}.{% for
+00000ad0: 2073 706f 6e73 6f72 2069 6e20 7370 6f6e   sponsor in spon
+00000ae0: 736f 7273 2e67 6f6c 6420 2d25 7d0a 3c61  sors.gold -%}.<a
+00000af0: 2068 7265 663d 227b 7b20 7370 6f6e 736f   href="{{ sponso
+00000b00: 722e 7572 6c20 7d7d 2220 7461 7267 6574  r.url }}" target
+00000b10: 3d22 5f62 6c61 6e6b 2220 7469 746c 653d  ="_blank" title=
+00000b20: 227b 7b20 7370 6f6e 736f 722e 7469 746c  "{{ sponsor.titl
+00000b30: 6520 7d7d 223e 3c69 6d67 2073 7263 3d22  e }}"><img src="
+00000b40: 7b7b 2073 706f 6e73 6f72 2e69 6d67 207d  {{ sponsor.img }
+00000b50: 7d22 2073 7479 6c65 3d22 626f 7264 6572  }" style="border
+00000b60: 2d72 6164 6975 733a 3135 7078 223e 3c2f  -radius:15px"></
+00000b70: 613e 0a7b 2520 656e 6466 6f72 202d 257d  a>.{% endfor -%}
+00000b80: 0a7b 252d 2066 6f72 2073 706f 6e73 6f72  .{%- for sponsor
+00000b90: 2069 6e20 7370 6f6e 736f 7273 2e73 696c   in sponsors.sil
+00000ba0: 7665 7220 2d25 7d0a 3c61 2068 7265 663d  ver -%}.<a href=
+00000bb0: 227b 7b20 7370 6f6e 736f 722e 7572 6c20  "{{ sponsor.url 
+00000bc0: 7d7d 2220 7461 7267 6574 3d22 5f62 6c61  }}" target="_bla
+00000bd0: 6e6b 2220 7469 746c 653d 227b 7b20 7370  nk" title="{{ sp
+00000be0: 6f6e 736f 722e 7469 746c 6520 7d7d 223e  onsor.title }}">
+00000bf0: 3c69 6d67 2073 7263 3d22 7b7b 2073 706f  <img src="{{ spo
+00000c00: 6e73 6f72 2e69 6d67 207d 7d22 2073 7479  nsor.img }}" sty
+00000c10: 6c65 3d22 626f 7264 6572 2d72 6164 6975  le="border-radiu
+00000c20: 733a 3135 7078 223e 3c2f 613e 0a7b 2520  s:15px"></a>.{% 
+00000c30: 656e 6466 6f72 2025 7d0a 7b25 2065 6e64  endfor %}.{% end
+00000c40: 6966 2025 7d0a 0a3c 212d 2d20 2f73 706f  if %}..<!-- /spo
+00000c50: 6e73 6f72 7320 2d2d 3e0a 0a3c 6120 6872  nsors -->..<a hr
+00000c60: 6566 3d22 6874 7470 733a 2f2f 7265 6164  ef="https://read
+00000c70: 7961 7069 2e6b 6875 6c6e 6173 6f66 742e  yapi.khulnasoft.
+00000c80: 636f 6d2f 7265 6164 7961 7069 2d70 656f  com/readyapi-peo
+00000c90: 706c 652f 2373 706f 6e73 6f72 7322 2063  ple/#sponsors" c
+00000ca0: 6c61 7373 3d22 6578 7465 726e 616c 2d6c  lass="external-l
+00000cb0: 696e 6b22 2074 6172 6765 743d 225f 626c  ink" target="_bl
+00000cc0: 616e 6b22 3e4f 7468 6572 2073 706f 6e73  ank">Other spons
+00000cd0: 6f72 733c 2f61 3e0a 0a23 2320 4f70 696e  ors</a>..## Opin
+00000ce0: 696f 6e73 0a0a 225f 5b2e 2e2e 5d20 4927  ions.."_[...] I'
+00000cf0: 6d20 7573 696e 6720 2a2a 5265 6164 7941  m using **ReadyA
+00000d00: 5049 2a2a 2061 2074 6f6e 2074 6865 7365  PI** a ton these
+00000d10: 2064 6179 732e 205b 2e2e 2e5d 2049 276d   days. [...] I'm
+00000d20: 2061 6374 7561 6c6c 7920 706c 616e 6e69   actually planni
+00000d30: 6e67 2074 6f20 7573 6520 6974 2066 6f72  ng to use it for
+00000d40: 2061 6c6c 206f 6620 6d79 2074 6561 6d27   all of my team'
+00000d50: 7320 2a2a 4d4c 2073 6572 7669 6365 7320  s **ML services 
+00000d60: 6174 204d 6963 726f 736f 6674 2a2a 2e20  at Microsoft**. 
+00000d70: 536f 6d65 206f 6620 7468 656d 2061 7265  Some of them are
+00000d80: 2067 6574 7469 6e67 2069 6e74 6567 7261   getting integra
+00000d90: 7465 6420 696e 746f 2074 6865 2063 6f72  ted into the cor
+00000da0: 6520 2a2a 5769 6e64 6f77 732a 2a20 7072  e **Windows** pr
+00000db0: 6f64 7563 7420 616e 6420 736f 6d65 202a  oduct and some *
+00000dc0: 2a4f 6666 6963 652a 2a20 7072 6f64 7563  *Office** produc
+00000dd0: 7473 2e5f 220a 0a3c 6469 7620 7374 796c  ts._"..<div styl
+00000de0: 653d 2274 6578 742d 616c 6967 6e3a 2072  e="text-align: r
+00000df0: 6967 6874 3b20 6d61 7267 696e 2d72 6967  ight; margin-rig
+00000e00: 6874 3a20 3130 253b 223e 4b61 6269 7220  ht: 10%;">Kabir 
+00000e10: 4b68 616e 202d 203c 7374 726f 6e67 3e4d  Khan - <strong>M
+00000e20: 6963 726f 736f 6674 3c2f 7374 726f 6e67  icrosoft</strong
+00000e30: 3e20 3c61 2068 7265 663d 2268 7474 7073  > <a href="https
+00000e40: 3a2f 2f67 6974 6875 622e 636f 6d2f 6b68  ://github.com/kh
+00000e50: 756c 6e61 736f 6674 2f72 6561 6479 6170  ulnasoft/readyap
+00000e60: 692f 7075 6c6c 2f32 3622 2074 6172 6765  i/pull/26" targe
+00000e70: 743d 225f 626c 616e 6b22 3e3c 736d 616c  t="_blank"><smal
+00000e80: 6c3e 2872 6566 293c 2f73 6d61 6c6c 3e3c  l>(ref)</small><
+00000e90: 2f61 3e3c 2f64 6976 3e0a 0a2d 2d2d 0a0a  /a></div>..---..
+00000ea0: 225f 5765 2061 646f 7074 6564 2074 6865  "_We adopted the
+00000eb0: 202a 2a52 6561 6479 4150 492a 2a20 6c69   **ReadyAPI** li
+00000ec0: 6272 6172 7920 746f 2073 7061 776e 2061  brary to spawn a
+00000ed0: 202a 2a52 4553 542a 2a20 7365 7276 6572   **REST** server
+00000ee0: 2074 6861 7420 6361 6e20 6265 2071 7565   that can be que
+00000ef0: 7269 6564 2074 6f20 6f62 7461 696e 202a  ried to obtain *
+00000f00: 2a70 7265 6469 6374 696f 6e73 2a2a 2e20  *predictions**. 
+00000f10: 5b66 6f72 204c 7564 7769 675d 5f22 0a0a  [for Ludwig]_"..
+00000f20: 3c64 6976 2073 7479 6c65 3d22 7465 7874  <div style="text
+00000f30: 2d61 6c69 676e 3a20 7269 6768 743b 206d  -align: right; m
+00000f40: 6172 6769 6e2d 7269 6768 743a 2031 3025  argin-right: 10%
+00000f50: 3b22 3e50 6965 726f 204d 6f6c 696e 6f2c  ;">Piero Molino,
+00000f60: 2059 6172 6f73 6c61 7620 4475 6469 6e2c   Yaroslav Dudin,
+00000f70: 2061 6e64 2053 6169 2053 756d 616e 7468   and Sai Sumanth
+00000f80: 204d 6972 7961 6c61 202d 203c 7374 726f   Miryala - <stro
+00000f90: 6e67 3e55 6265 723c 2f73 7472 6f6e 673e  ng>Uber</strong>
+00000fa0: 203c 6120 6872 6566 3d22 6874 7470 733a   <a href="https:
+00000fb0: 2f2f 656e 672e 7562 6572 2e63 6f6d 2f6c  //eng.uber.com/l
+00000fc0: 7564 7769 672d 7630 2d32 2f22 2074 6172  udwig-v0-2/" tar
+00000fd0: 6765 743d 225f 626c 616e 6b22 3e3c 736d  get="_blank"><sm
+00000fe0: 616c 6c3e 2872 6566 293c 2f73 6d61 6c6c  all>(ref)</small
+00000ff0: 3e3c 2f61 3e3c 2f64 6976 3e0a 0a2d 2d2d  ></a></div>..---
+00001000: 0a0a 225f 2a2a 4e65 7466 6c69 782a 2a20  .."_**Netflix** 
+00001010: 6973 2070 6c65 6173 6564 2074 6f20 616e  is pleased to an
+00001020: 6e6f 756e 6365 2074 6865 206f 7065 6e2d  nounce the open-
+00001030: 736f 7572 6365 2072 656c 6561 7365 206f  source release o
+00001040: 6620 6f75 7220 2a2a 6372 6973 6973 206d  f our **crisis m
+00001050: 616e 6167 656d 656e 742a 2a20 6f72 6368  anagement** orch
+00001060: 6573 7472 6174 696f 6e20 6672 616d 6577  estration framew
+00001070: 6f72 6b3a 202a 2a44 6973 7061 7463 682a  ork: **Dispatch*
+00001080: 2a21 205b 6275 696c 7420 7769 7468 202a  *! [built with *
+00001090: 2a52 6561 6479 4150 492a 2a5d 5f22 0a0a  *ReadyAPI**]_"..
+000010a0: 3c64 6976 2073 7479 6c65 3d22 7465 7874  <div style="text
+000010b0: 2d61 6c69 676e 3a20 7269 6768 743b 206d  -align: right; m
+000010c0: 6172 6769 6e2d 7269 6768 743a 2031 3025  argin-right: 10%
+000010d0: 3b22 3e4b 6576 696e 2047 6c69 7373 6f6e  ;">Kevin Glisson
+000010e0: 2c20 4d61 7263 2056 696c 616e 6f76 612c  , Marc Vilanova,
+000010f0: 2046 6f72 6573 7420 4d6f 6e73 656e 202d   Forest Monsen -
+00001100: 203c 7374 726f 6e67 3e4e 6574 666c 6978   <strong>Netflix
+00001110: 3c2f 7374 726f 6e67 3e20 3c61 2068 7265  </strong> <a hre
+00001120: 663d 2268 7474 7073 3a2f 2f6e 6574 666c  f="https://netfl
+00001130: 6978 7465 6368 626c 6f67 2e63 6f6d 2f69  ixtechblog.com/i
+00001140: 6e74 726f 6475 6369 6e67 2d64 6973 7061  ntroducing-dispa
+00001150: 7463 682d 6461 3462 3861 3261 3830 3732  tch-da4b8a2a8072
+00001160: 2220 7461 7267 6574 3d22 5f62 6c61 6e6b  " target="_blank
+00001170: 223e 3c73 6d61 6c6c 3e28 7265 6629 3c2f  "><small>(ref)</
+00001180: 736d 616c 6c3e 3c2f 613e 3c2f 6469 763e  small></a></div>
+00001190: 0a0a 2d2d 2d0a 0a22 5f49 e280 996d 206f  ..---.."_I...m o
+000011a0: 7665 7220 7468 6520 6d6f 6f6e 2065 7863  ver the moon exc
+000011b0: 6974 6564 2061 626f 7574 202a 2a52 6561  ited about **Rea
+000011c0: 6479 4150 492a 2a2e 2049 74e2 8099 7320  dyAPI**. It...s 
+000011d0: 736f 2066 756e 215f 220a 0a3c 6469 7620  so fun!_"..<div 
+000011e0: 7374 796c 653d 2274 6578 742d 616c 6967  style="text-alig
+000011f0: 6e3a 2072 6967 6874 3b20 6d61 7267 696e  n: right; margin
+00001200: 2d72 6967 6874 3a20 3130 253b 223e 4272  -right: 10%;">Br
+00001210: 6961 6e20 4f6b 6b65 6e20 2d20 3c73 7472  ian Okken - <str
+00001220: 6f6e 673e 3c61 2068 7265 663d 2268 7474  ong><a href="htt
+00001230: 7073 3a2f 2f70 7974 686f 6e62 7974 6573  ps://pythonbytes
+00001240: 2e66 6d2f 6570 6973 6f64 6573 2f73 686f  .fm/episodes/sho
+00001250: 772f 3132 332f 7469 6d65 2d74 6f2d 7269  w/123/time-to-ri
+00001260: 6768 742d 7468 652d 7079 2d77 726f 6e67  ght-the-py-wrong
+00001270: 733f 7469 6d65 5f69 6e5f 7365 633d 3835  s?time_in_sec=85
+00001280: 3522 2074 6172 6765 743d 225f 626c 616e  5" target="_blan
+00001290: 6b22 3e50 7974 686f 6e20 4279 7465 733c  k">Python Bytes<
+000012a0: 2f61 3e20 706f 6463 6173 7420 686f 7374  /a> podcast host
+000012b0: 3c2f 7374 726f 6e67 3e20 3c61 2068 7265  </strong> <a hre
+000012c0: 663d 2268 7474 7073 3a2f 2f74 7769 7474  f="https://twitt
+000012d0: 6572 2e63 6f6d 2f62 7269 616e 6f6b 6b65  er.com/brianokke
+000012e0: 6e2f 7374 6174 7573 2f31 3131 3232 3230  n/status/1112220
+000012f0: 3037 3939 3732 3732 3838 3332 2220 7461  079972728832" ta
+00001300: 7267 6574 3d22 5f62 6c61 6e6b 223e 3c73  rget="_blank"><s
+00001310: 6d61 6c6c 3e28 7265 6629 3c2f 736d 616c  mall>(ref)</smal
+00001320: 6c3e 3c2f 613e 3c2f 6469 763e 0a0a 2d2d  l></a></div>..--
+00001330: 2d0a 0a22 5f48 6f6e 6573 746c 792c 2077  -.."_Honestly, w
+00001340: 6861 7420 796f 7527 7665 2062 7569 6c74  hat you've built
+00001350: 206c 6f6f 6b73 2073 7570 6572 2073 6f6c   looks super sol
+00001360: 6964 2061 6e64 2070 6f6c 6973 6865 642e  id and polished.
+00001370: 2049 6e20 6d61 6e79 2077 6179 732c 2069   In many ways, i
+00001380: 7427 7320 7768 6174 2049 2077 616e 7465  t's what I wante
+00001390: 6420 2a2a 4875 672a 2a20 746f 2062 6520  d **Hug** to be 
+000013a0: 2d20 6974 2773 2072 6561 6c6c 7920 696e  - it's really in
+000013b0: 7370 6972 696e 6720 746f 2073 6565 2073  spiring to see s
+000013c0: 6f6d 656f 6e65 2062 7569 6c64 2074 6861  omeone build tha
+000013d0: 742e 5f22 0a0a 3c64 6976 2073 7479 6c65  t._"..<div style
+000013e0: 3d22 7465 7874 2d61 6c69 676e 3a20 7269  ="text-align: ri
+000013f0: 6768 743b 206d 6172 6769 6e2d 7269 6768  ght; margin-righ
+00001400: 743a 2031 3025 3b22 3e54 696d 6f74 6879  t: 10%;">Timothy
+00001410: 2043 726f 736c 6579 202d 203c 7374 726f   Crosley - <stro
+00001420: 6e67 3e3c 6120 6872 6566 3d22 6874 7470  ng><a href="http
+00001430: 733a 2f2f 7777 772e 6875 672e 7265 7374  s://www.hug.rest
+00001440: 2f22 2074 6172 6765 743d 225f 626c 616e  /" target="_blan
+00001450: 6b22 3e48 7567 3c2f 613e 2063 7265 6174  k">Hug</a> creat
+00001460: 6f72 3c2f 7374 726f 6e67 3e20 3c61 2068  or</strong> <a h
+00001470: 7265 663d 2268 7474 7073 3a2f 2f6e 6577  ref="https://new
+00001480: 732e 7963 6f6d 6269 6e61 746f 722e 636f  s.ycombinator.co
+00001490: 6d2f 6974 656d 3f69 643d 3139 3435 3534  m/item?id=194554
+000014a0: 3635 2220 7461 7267 6574 3d22 5f62 6c61  65" target="_bla
+000014b0: 6e6b 223e 3c73 6d61 6c6c 3e28 7265 6629  nk"><small>(ref)
+000014c0: 3c2f 736d 616c 6c3e 3c2f 613e 3c2f 6469  </small></a></di
+000014d0: 763e 0a0a 2d2d 2d0a 0a22 5f49 6620 796f  v>..---.."_If yo
+000014e0: 7527 7265 206c 6f6f 6b69 6e67 2074 6f20  u're looking to 
+000014f0: 6c65 6172 6e20 6f6e 6520 2a2a 6d6f 6465  learn one **mode
+00001500: 726e 2066 7261 6d65 776f 726b 2a2a 2066  rn framework** f
+00001510: 6f72 2062 7569 6c64 696e 6720 5245 5354  or building REST
+00001520: 2041 5049 732c 2063 6865 636b 206f 7574   APIs, check out
+00001530: 202a 2a52 6561 6479 4150 492a 2a20 5b2e   **ReadyAPI** [.
+00001540: 2e2e 5d20 4974 2773 2066 6173 742c 2065  ..] It's fast, e
+00001550: 6173 7920 746f 2075 7365 2061 6e64 2065  asy to use and e
+00001560: 6173 7920 746f 206c 6561 726e 205b 2e2e  asy to learn [..
+00001570: 2e5d 5f22 0a0a 225f 5765 2776 6520 7377  .]_".."_We've sw
+00001580: 6974 6368 6564 206f 7665 7220 746f 202a  itched over to *
+00001590: 2a52 6561 6479 4150 492a 2a20 666f 7220  *ReadyAPI** for 
+000015a0: 6f75 7220 2a2a 4150 4973 2a2a 205b 2e2e  our **APIs** [..
+000015b0: 2e5d 2049 2074 6869 6e6b 2079 6f75 276c  .] I think you'l
+000015c0: 6c20 6c69 6b65 2069 7420 5b2e 2e2e 5d5f  l like it [...]_
+000015d0: 220a 0a3c 6469 7620 7374 796c 653d 2274  "..<div style="t
+000015e0: 6578 742d 616c 6967 6e3a 2072 6967 6874  ext-align: right
+000015f0: 3b20 6d61 7267 696e 2d72 6967 6874 3a20  ; margin-right: 
+00001600: 3130 253b 223e 496e 6573 204d 6f6e 7461  10%;">Ines Monta
+00001610: 6e69 202d 204d 6174 7468 6577 2048 6f6e  ni - Matthew Hon
+00001620: 6e69 6261 6c20 2d20 3c73 7472 6f6e 673e  nibal - <strong>
+00001630: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
+00001640: 2f65 7870 6c6f 7369 6f6e 2e61 6922 2074  /explosion.ai" t
+00001650: 6172 6765 743d 225f 626c 616e 6b22 3e45  arget="_blank">E
+00001660: 7870 6c6f 7369 6f6e 2041 493c 2f61 3e20  xplosion AI</a> 
+00001670: 666f 756e 6465 7273 202d 203c 6120 6872  founders - <a hr
+00001680: 6566 3d22 6874 7470 733a 2f2f 7370 6163  ef="https://spac
+00001690: 792e 696f 2220 7461 7267 6574 3d22 5f62  y.io" target="_b
+000016a0: 6c61 6e6b 223e 7370 6143 793c 2f61 3e20  lank">spaCy</a> 
+000016b0: 6372 6561 746f 7273 3c2f 7374 726f 6e67  creators</strong
+000016c0: 3e20 3c61 2068 7265 663d 2268 7474 7073  > <a href="https
+000016d0: 3a2f 2f74 7769 7474 6572 2e63 6f6d 2f5f  ://twitter.com/_
+000016e0: 696e 6573 6d6f 6e74 616e 692f 7374 6174  inesmontani/stat
+000016f0: 7573 2f31 3134 3431 3733 3232 3533 3232  us/1144173225322
+00001700: 3134 3337 3434 2220 7461 7267 6574 3d22  143744" target="
+00001710: 5f62 6c61 6e6b 223e 3c73 6d61 6c6c 3e28  _blank"><small>(
+00001720: 7265 6629 3c2f 736d 616c 6c3e 3c2f 613e  ref)</small></a>
+00001730: 202d 203c 6120 6872 6566 3d22 6874 7470   - <a href="http
+00001740: 733a 2f2f 7477 6974 7465 722e 636f 6d2f  s://twitter.com/
+00001750: 686f 6e6e 6962 616c 2f73 7461 7475 732f  honnibal/status/
+00001760: 3131 3434 3033 3134 3231 3835 3936 3535  1144031421859655
+00001770: 3638 3022 2074 6172 6765 743d 225f 626c  680" target="_bl
+00001780: 616e 6b22 3e3c 736d 616c 6c3e 2872 6566  ank"><small>(ref
+00001790: 293c 2f73 6d61 6c6c 3e3c 2f61 3e3c 2f64  )</small></a></d
+000017a0: 6976 3e0a 0a2d 2d2d 0a0a 225f 4966 2061  iv>..---.."_If a
+000017b0: 6e79 6f6e 6520 6973 206c 6f6f 6b69 6e67  nyone is looking
+000017c0: 2074 6f20 6275 696c 6420 6120 7072 6f64   to build a prod
+000017d0: 7563 7469 6f6e 2050 7974 686f 6e20 4150  uction Python AP
+000017e0: 492c 2049 2077 6f75 6c64 2068 6967 686c  I, I would highl
+000017f0: 7920 7265 636f 6d6d 656e 6420 2a2a 5265  y recommend **Re
+00001800: 6164 7941 5049 2a2a 2e20 4974 2069 7320  adyAPI**. It is 
+00001810: 2a2a 6265 6175 7469 6675 6c6c 7920 6465  **beautifully de
+00001820: 7369 676e 6564 2a2a 2c20 2a2a 7369 6d70  signed**, **simp
+00001830: 6c65 2074 6f20 7573 652a 2a20 616e 6420  le to use** and 
+00001840: 2a2a 6869 6768 6c79 2073 6361 6c61 626c  **highly scalabl
+00001850: 652a 2a2c 2069 7420 6861 7320 6265 636f  e**, it has beco
+00001860: 6d65 2061 202a 2a6b 6579 2063 6f6d 706f  me a **key compo
+00001870: 6e65 6e74 2a2a 2069 6e20 6f75 7220 4150  nent** in our AP
+00001880: 4920 6669 7273 7420 6465 7665 6c6f 706d  I first developm
+00001890: 656e 7420 7374 7261 7465 6779 2061 6e64  ent strategy and
+000018a0: 2069 7320 6472 6976 696e 6720 6d61 6e79   is driving many
+000018b0: 2061 7574 6f6d 6174 696f 6e73 2061 6e64   automations and
+000018c0: 2073 6572 7669 6365 7320 7375 6368 2061   services such a
+000018d0: 7320 6f75 7220 5669 7274 7561 6c20 5441  s our Virtual TA
+000018e0: 4320 456e 6769 6e65 6572 2e5f 220a 0a3c  C Engineer._"..<
+000018f0: 6469 7620 7374 796c 653d 2274 6578 742d  div style="text-
+00001900: 616c 6967 6e3a 2072 6967 6874 3b20 6d61  align: right; ma
+00001910: 7267 696e 2d72 6967 6874 3a20 3130 253b  rgin-right: 10%;
+00001920: 223e 4465 6f6e 2050 696c 6c73 6275 7279  ">Deon Pillsbury
+00001930: 202d 203c 7374 726f 6e67 3e43 6973 636f   - <strong>Cisco
+00001940: 3c2f 7374 726f 6e67 3e20 3c61 2068 7265  </strong> <a hre
+00001950: 663d 2268 7474 7073 3a2f 2f77 7777 2e6c  f="https://www.l
+00001960: 696e 6b65 6469 6e2e 636f 6d2f 706f 7374  inkedin.com/post
+00001970: 732f 6465 6f6e 7069 6c6c 7362 7572 795f  s/deonpillsbury_
+00001980: 6369 7363 6f2d 6378 2d70 7974 686f 6e2d  cisco-cx-python-
+00001990: 6163 7469 7669 7479 2d36 3936 3332 3432  activity-6963242
+000019a0: 3632 3835 3336 3438 3739 3336 2d74 7241  628536487936-trA
+000019b0: 702f 2220 7461 7267 6574 3d22 5f62 6c61  p/" target="_bla
+000019c0: 6e6b 223e 3c73 6d61 6c6c 3e28 7265 6629  nk"><small>(ref)
+000019d0: 3c2f 736d 616c 6c3e 3c2f 613e 3c2f 6469  </small></a></di
+000019e0: 763e 0a0a 2d2d 2d0a 0a23 2320 2a2a 5479  v>..---..## **Ty
+000019f0: 7065 722a 2a2c 2074 6865 2052 6561 6479  per**, the Ready
+00001a00: 4150 4920 6f66 2043 4c49 730a 0a3c 6120  API of CLIs..<a 
+00001a10: 6872 6566 3d22 6874 7470 733a 2f2f 7479  href="https://ty
+00001a20: 7065 722e 7469 616e 676f 6c6f 2e63 6f6d  per.tiangolo.com
+00001a30: 2220 7461 7267 6574 3d22 5f62 6c61 6e6b  " target="_blank
+00001a40: 223e 3c69 6d67 2073 7263 3d22 6874 7470  "><img src="http
+00001a50: 733a 2f2f 7479 7065 722e 7469 616e 676f  s://typer.tiango
+00001a60: 6c6f 2e63 6f6d 2f69 6d67 2f6c 6f67 6f2d  lo.com/img/logo-
+00001a70: 6d61 7267 696e 2f6c 6f67 6f2d 6d61 7267  margin/logo-marg
+00001a80: 696e 2d76 6563 746f 722e 7376 6722 2073  in-vector.svg" s
+00001a90: 7479 6c65 3d22 7769 6474 683a 2032 3025  tyle="width: 20%
+00001aa0: 3b22 3e3c 2f61 3e0a 0a49 6620 796f 7520  ;"></a>..If you 
+00001ab0: 6172 6520 6275 696c 6469 6e67 2061 203c  are building a <
+00001ac0: 6162 6272 2074 6974 6c65 3d22 436f 6d6d  abbr title="Comm
+00001ad0: 616e 6420 4c69 6e65 2049 6e74 6572 6661  and Line Interfa
+00001ae0: 6365 223e 434c 493c 2f61 6262 723e 2061  ce">CLI</abbr> a
+00001af0: 7070 2074 6f20 6265 2075 7365 6420 696e  pp to be used in
+00001b00: 2074 6865 2074 6572 6d69 6e61 6c20 696e   the terminal in
+00001b10: 7374 6561 6420 6f66 2061 2077 6562 2041  stead of a web A
+00001b20: 5049 2c20 6368 6563 6b20 6f75 7420 3c61  PI, check out <a
+00001b30: 2068 7265 663d 2268 7474 7073 3a2f 2f74   href="https://t
+00001b40: 7970 6572 2e74 6961 6e67 6f6c 6f2e 636f  yper.tiangolo.co
+00001b50: 6d2f 2220 636c 6173 733d 2265 7874 6572  m/" class="exter
+00001b60: 6e61 6c2d 6c69 6e6b 2220 7461 7267 6574  nal-link" target
+00001b70: 3d22 5f62 6c61 6e6b 223e 2a2a 5479 7065  ="_blank">**Type
+00001b80: 722a 2a3c 2f61 3e2e 0a0a 2a2a 5479 7065  r**</a>...**Type
+00001b90: 722a 2a20 6973 2052 6561 6479 4150 4927  r** is ReadyAPI'
+00001ba0: 7320 6c69 7474 6c65 2073 6962 6c69 6e67  s little sibling
+00001bb0: 2e20 416e 6420 6974 2773 2069 6e74 656e  . And it's inten
+00001bc0: 6465 6420 746f 2062 6520 7468 6520 2a2a  ded to be the **
+00001bd0: 5265 6164 7941 5049 206f 6620 434c 4973  ReadyAPI of CLIs
+00001be0: 2a2a 2e20 e28c a8ef b88f 20f0 9f9a 800a  **. ...... .....
+00001bf0: 0a23 2320 5265 7175 6972 656d 656e 7473  .## Requirements
+00001c00: 0a0a 5265 6164 7941 5049 2073 7461 6e64  ..ReadyAPI stand
+00001c10: 7320 6f6e 2074 6865 2073 686f 756c 6465  s on the shoulde
+00001c20: 7273 206f 6620 6769 616e 7473 3a0a 0a2a  rs of giants:..*
+00001c30: 203c 6120 6872 6566 3d22 6874 7470 733a   <a href="https:
+00001c40: 2f2f 7777 772e 7374 6172 6c65 7474 652e  //www.starlette.
+00001c50: 696f 2f22 2063 6c61 7373 3d22 6578 7465  io/" class="exte
+00001c60: 726e 616c 2d6c 696e 6b22 2074 6172 6765  rnal-link" targe
+00001c70: 743d 225f 626c 616e 6b22 3e53 7461 726c  t="_blank">Starl
+00001c80: 6574 7465 3c2f 613e 2066 6f72 2074 6865  ette</a> for the
+00001c90: 2077 6562 2070 6172 7473 2e0a 2a20 3c61   web parts..* <a
+00001ca0: 2068 7265 663d 2268 7474 7073 3a2f 2f64   href="https://d
+00001cb0: 6f63 732e 7079 6461 6e74 6963 2e64 6576  ocs.pydantic.dev
+00001cc0: 2f22 2063 6c61 7373 3d22 6578 7465 726e  /" class="extern
+00001cd0: 616c 2d6c 696e 6b22 2074 6172 6765 743d  al-link" target=
+00001ce0: 225f 626c 616e 6b22 3e50 7964 616e 7469  "_blank">Pydanti
+00001cf0: 633c 2f61 3e20 666f 7220 7468 6520 6461  c</a> for the da
+00001d00: 7461 2070 6172 7473 2e0a 0a23 2320 496e  ta parts...## In
+00001d10: 7374 616c 6c61 7469 6f6e 0a0a 3c64 6976  stallation..<div
+00001d20: 2063 6c61 7373 3d22 7465 726d 7922 3e0a   class="termy">.
+00001d30: 0a60 6060 636f 6e73 6f6c 650a 2420 7069  .```console.$ pi
+00001d40: 7020 696e 7374 616c 6c20 7265 6164 7961  p install readya
+00001d50: 7069 0a0a 2d2d 2d3e 2031 3030 250a 6060  pi..---> 100%.``
+00001d60: 600a 0a3c 2f64 6976 3e0a 0a23 2320 4578  `..</div>..## Ex
+00001d70: 616d 706c 650a 0a23 2323 2043 7265 6174  ample..### Creat
+00001d80: 6520 6974 0a0a 2a20 4372 6561 7465 2061  e it..* Create a
+00001d90: 2066 696c 6520 606d 6169 6e2e 7079 6020   file `main.py` 
+00001da0: 7769 7468 3a0a 0a60 6060 5079 7468 6f6e  with:..```Python
+00001db0: 0a66 726f 6d20 7479 7069 6e67 2069 6d70  .from typing imp
+00001dc0: 6f72 7420 556e 696f 6e0a 0a66 726f 6d20  ort Union..from 
+00001dd0: 7265 6164 7961 7069 2069 6d70 6f72 7420  readyapi import 
+00001de0: 5265 6164 7941 5049 0a0a 6170 7020 3d20  ReadyAPI..app = 
+00001df0: 5265 6164 7941 5049 2829 0a0a 0a40 6170  ReadyAPI()...@ap
+00001e00: 702e 6765 7428 222f 2229 0a64 6566 2072  p.get("/").def r
+00001e10: 6561 645f 726f 6f74 2829 3a0a 2020 2020  ead_root():.    
+00001e20: 7265 7475 726e 207b 2248 656c 6c6f 223a  return {"Hello":
+00001e30: 2022 576f 726c 6422 7d0a 0a0a 4061 7070   "World"}...@app
+00001e40: 2e67 6574 2822 2f69 7465 6d73 2f7b 6974  .get("/items/{it
+00001e50: 656d 5f69 647d 2229 0a64 6566 2072 6561  em_id}").def rea
+00001e60: 645f 6974 656d 2869 7465 6d5f 6964 3a20  d_item(item_id: 
+00001e70: 696e 742c 2071 3a20 556e 696f 6e5b 7374  int, q: Union[st
+00001e80: 722c 204e 6f6e 655d 203d 204e 6f6e 6529  r, None] = None)
+00001e90: 3a0a 2020 2020 7265 7475 726e 207b 2269  :.    return {"i
+00001ea0: 7465 6d5f 6964 223a 2069 7465 6d5f 6964  tem_id": item_id
+00001eb0: 2c20 2271 223a 2071 7d0a 6060 600a 0a3c  , "q": q}.```..<
+00001ec0: 6465 7461 696c 7320 6d61 726b 646f 776e  details markdown
+00001ed0: 3d22 3122 3e0a 3c73 756d 6d61 7279 3e4f  ="1">.<summary>O
+00001ee0: 7220 7573 6520 3c63 6f64 653e 6173 796e  r use <code>asyn
+00001ef0: 6320 6465 663c 2f63 6f64 653e 2e2e 2e3c  c def</code>...<
+00001f00: 2f73 756d 6d61 7279 3e0a 0a49 6620 796f  /summary>..If yo
+00001f10: 7572 2063 6f64 6520 7573 6573 2060 6173  ur code uses `as
+00001f20: 796e 6360 202f 2060 6177 6169 7460 2c20  ync` / `await`, 
+00001f30: 7573 6520 6061 7379 6e63 2064 6566 603a  use `async def`:
+00001f40: 0a0a 6060 6050 7974 686f 6e20 686c 5f6c  ..```Python hl_l
+00001f50: 696e 6573 3d22 3920 2031 3422 0a66 726f  ines="9  14".fro
+00001f60: 6d20 7479 7069 6e67 2069 6d70 6f72 7420  m typing import 
+00001f70: 556e 696f 6e0a 0a66 726f 6d20 7265 6164  Union..from read
+00001f80: 7961 7069 2069 6d70 6f72 7420 5265 6164  yapi import Read
+00001f90: 7941 5049 0a0a 6170 7020 3d20 5265 6164  yAPI..app = Read
+00001fa0: 7941 5049 2829 0a0a 0a40 6170 702e 6765  yAPI()...@app.ge
+00001fb0: 7428 222f 2229 0a61 7379 6e63 2064 6566  t("/").async def
+00001fc0: 2072 6561 645f 726f 6f74 2829 3a0a 2020   read_root():.  
+00001fd0: 2020 7265 7475 726e 207b 2248 656c 6c6f    return {"Hello
+00001fe0: 223a 2022 576f 726c 6422 7d0a 0a0a 4061  ": "World"}...@a
+00001ff0: 7070 2e67 6574 2822 2f69 7465 6d73 2f7b  pp.get("/items/{
+00002000: 6974 656d 5f69 647d 2229 0a61 7379 6e63  item_id}").async
+00002010: 2064 6566 2072 6561 645f 6974 656d 2869   def read_item(i
+00002020: 7465 6d5f 6964 3a20 696e 742c 2071 3a20  tem_id: int, q: 
+00002030: 556e 696f 6e5b 7374 722c 204e 6f6e 655d  Union[str, None]
+00002040: 203d 204e 6f6e 6529 3a0a 2020 2020 7265   = None):.    re
+00002050: 7475 726e 207b 2269 7465 6d5f 6964 223a  turn {"item_id":
+00002060: 2069 7465 6d5f 6964 2c20 2271 223a 2071   item_id, "q": q
+00002070: 7d0a 6060 600a 0a2a 2a4e 6f74 652a 2a3a  }.```..**Note**:
+00002080: 0a0a 4966 2079 6f75 2064 6f6e 2774 206b  ..If you don't k
+00002090: 6e6f 772c 2063 6865 636b 2074 6865 205f  now, check the _
+000020a0: 2249 6e20 6120 6875 7272 793f 225f 2073  "In a hurry?"_ s
+000020b0: 6563 7469 6f6e 2061 626f 7574 203c 6120  ection about <a 
+000020c0: 6872 6566 3d22 6874 7470 733a 2f2f 7265  href="https://re
+000020d0: 6164 7961 7069 2e6b 6875 6c6e 6173 6f66  adyapi.khulnasof
+000020e0: 742e 636f 6d2f 6173 796e 632f 2369 6e2d  t.com/async/#in-
+000020f0: 612d 6875 7272 7922 2074 6172 6765 743d  a-hurry" target=
+00002100: 225f 626c 616e 6b22 3e60 6173 796e 6360  "_blank">`async`
+00002110: 2061 6e64 2060 6177 6169 7460 2069 6e20   and `await` in 
+00002120: 7468 6520 646f 6373 3c2f 613e 2e0a 0a3c  the docs</a>...<
+00002130: 2f64 6574 6169 6c73 3e0a 0a23 2323 2052  /details>..### R
+00002140: 756e 2069 740a 0a52 756e 2074 6865 2073  un it..Run the s
+00002150: 6572 7665 7220 7769 7468 3a0a 0a3c 6469  erver with:..<di
+00002160: 7620 636c 6173 733d 2274 6572 6d79 223e  v class="termy">
+00002170: 0a0a 6060 6063 6f6e 736f 6c65 0a24 2072  ..```console.$ r
+00002180: 6561 6479 6170 6920 6465 7620 6d61 696e  eadyapi dev main
+00002190: 2e70 790a 0a20 e295 ade2 9480 e294 80e2  .py.. ..........
+000021a0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000021b0: 80e2 9480 e294 8020 5265 6164 7941 5049  ....... ReadyAPI
+000021c0: 2043 4c49 202d 2044 6576 656c 6f70 6d65   CLI - Developme
+000021d0: 6e74 206d 6f64 6520 e294 80e2 9480 e294  nt mode ........
+000021e0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000021f0: e294 80e2 9480 e294 80e2 95ae 0a20 e294  ............. ..
+00002200: 8220 2020 2020 2020 2020 2020 2020 2020  .               
+00002210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002230: 2020 2020 2020 e294 820a 20e2 9482 2020        .... ...  
+00002240: 5365 7276 696e 6720 6174 3a20 6874 7470  Serving at: http
+00002250: 3a2f 2f31 3237 2e30 2e30 2e31 3a38 3030  ://127.0.0.1:800
+00002260: 3020 2020 2020 2020 2020 2020 2020 2020  0               
+00002270: 2020 20e2 9482 0a20 e294 8220 2020 2020     .... ...     
+00002280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000022a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000022b0: e294 820a 20e2 9482 2020 4150 4920 646f  .... ...  API do
+000022c0: 6373 3a20 6874 7470 3a2f 2f31 3237 2e30  cs: http://127.0
+000022d0: 2e30 2e31 3a38 3030 302f 646f 6373 2020  .0.1:8000/docs  
+000022e0: 2020 2020 2020 2020 2020 2020 20e2 9482               ...
+000022f0: 0a20 e294 8220 2020 2020 2020 2020 2020  . ...           
+00002300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002320: 2020 2020 2020 2020 2020 e294 820a 20e2            .... .
+00002330: 9482 2020 5275 6e6e 696e 6720 696e 2064  ..  Running in d
+00002340: 6576 656c 6f70 6d65 6e74 206d 6f64 652c  evelopment mode,
+00002350: 2066 6f72 2070 726f 6475 6374 696f 6e20   for production 
+00002360: 7573 653a 2020 20e2 9482 0a20 e294 8220  use:   .... ... 
+00002370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000023a0: 2020 2020 e294 820a 20e2 9482 2020 7265      .... ...  re
+000023b0: 6164 7961 7069 2072 756e 2020 2020 2020  adyapi run      
+000023c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000023d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000023e0: 2020 e294 820a 20e2 9482 2020 2020 2020    .... ...      
+000023f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002410: 2020 2020 2020 2020 2020 2020 2020 20e2                 .
+00002420: 9482 0a20 e295 b0e2 9480 e294 80e2 9480  ... ............
+00002430: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00002440: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00002450: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00002460: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00002470: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00002480: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00002490: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000024a0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000024b0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000024c0: e294 80e2 9480 e295 af0a 0a49 4e46 4f3a  ...........INFO:
+000024d0: 2020 2020 2057 696c 6c20 7761 7463 6820       Will watch 
+000024e0: 666f 7220 6368 616e 6765 7320 696e 2074  for changes in t
+000024f0: 6865 7365 2064 6972 6563 746f 7269 6573  hese directories
+00002500: 3a20 5b27 2f68 6f6d 652f 7573 6572 2f63  : ['/home/user/c
+00002510: 6f64 652f 6177 6573 6f6d 6561 7070 275d  ode/awesomeapp']
+00002520: 0a49 4e46 4f3a 2020 2020 2055 7669 636f  .INFO:     Uvico
+00002530: 726e 2072 756e 6e69 6e67 206f 6e20 6874  rn running on ht
+00002540: 7470 3a2f 2f31 3237 2e30 2e30 2e31 3a38  tp://127.0.0.1:8
+00002550: 3030 3020 2850 7265 7373 2043 5452 4c2b  000 (Press CTRL+
+00002560: 4320 746f 2071 7569 7429 0a49 4e46 4f3a  C to quit).INFO:
+00002570: 2020 2020 2053 7461 7274 6564 2072 656c       Started rel
+00002580: 6f61 6465 7220 7072 6f63 6573 7320 5b32  oader process [2
+00002590: 3234 3837 3535 5d20 7573 696e 6720 5761  248755] using Wa
+000025a0: 7463 6846 696c 6573 0a49 4e46 4f3a 2020  tchFiles.INFO:  
+000025b0: 2020 2053 7461 7274 6564 2073 6572 7665     Started serve
+000025c0: 7220 7072 6f63 6573 7320 5b32 3234 3837  r process [22487
+000025d0: 3537 5d0a 494e 464f 3a20 2020 2020 5761  57].INFO:     Wa
+000025e0: 6974 696e 6720 666f 7220 6170 706c 6963  iting for applic
+000025f0: 6174 696f 6e20 7374 6172 7475 702e 0a49  ation startup..I
+00002600: 4e46 4f3a 2020 2020 2041 7070 6c69 6361  NFO:     Applica
+00002610: 7469 6f6e 2073 7461 7274 7570 2063 6f6d  tion startup com
+00002620: 706c 6574 652e 0a60 6060 0a0a 3c2f 6469  plete..```..</di
+00002630: 763e 0a0a 3c64 6574 6169 6c73 206d 6172  v>..<details mar
+00002640: 6b64 6f77 6e3d 2231 223e 0a3c 7375 6d6d  kdown="1">.<summ
+00002650: 6172 793e 4162 6f75 7420 7468 6520 636f  ary>About the co
+00002660: 6d6d 616e 6420 3c63 6f64 653e 7265 6164  mmand <code>read
+00002670: 7961 7069 2064 6576 206d 6169 6e2e 7079  yapi dev main.py
+00002680: 3c2f 636f 6465 3e2e 2e2e 3c2f 7375 6d6d  </code>...</summ
+00002690: 6172 793e 0a0a 5468 6520 636f 6d6d 616e  ary>..The comman
+000026a0: 6420 6072 6561 6479 6170 6920 6465 7660  d `readyapi dev`
+000026b0: 2072 6561 6473 2079 6f75 7220 606d 6169   reads your `mai
+000026c0: 6e2e 7079 6020 6669 6c65 2c20 6465 7465  n.py` file, dete
+000026d0: 6374 7320 7468 6520 2a2a 5265 6164 7941  cts the **ReadyA
+000026e0: 5049 2a2a 2061 7070 2069 6e20 6974 2c20  PI** app in it, 
+000026f0: 616e 6420 7374 6172 7473 2061 2073 6572  and starts a ser
+00002700: 7665 7220 7573 696e 6720 3c61 2068 7265  ver using <a hre
+00002710: 663d 2268 7474 7073 3a2f 2f77 7777 2e75  f="https://www.u
+00002720: 7669 636f 726e 2e6f 7267 2220 636c 6173  vicorn.org" clas
+00002730: 733d 2265 7874 6572 6e61 6c2d 6c69 6e6b  s="external-link
+00002740: 2220 7461 7267 6574 3d22 5f62 6c61 6e6b  " target="_blank
+00002750: 223e 5576 6963 6f72 6e3c 2f61 3e2e 0a0a  ">Uvicorn</a>...
+00002760: 4279 2064 6566 6175 6c74 2c20 6072 6561  By default, `rea
+00002770: 6479 6170 6920 6465 7660 2077 696c 6c20  dyapi dev` will 
+00002780: 7374 6172 7420 7769 7468 2061 7574 6f2d  start with auto-
+00002790: 7265 6c6f 6164 2065 6e61 626c 6564 2066  reload enabled f
+000027a0: 6f72 206c 6f63 616c 2064 6576 656c 6f70  or local develop
+000027b0: 6d65 6e74 2e0a 0a59 6f75 2063 616e 2072  ment...You can r
+000027c0: 6561 6420 6d6f 7265 2061 626f 7574 2069  ead more about i
+000027d0: 7420 696e 2074 6865 203c 6120 6872 6566  t in the <a href
+000027e0: 3d22 6874 7470 733a 2f2f 7265 6164 7961  ="https://readya
+000027f0: 7069 2e6b 6875 6c6e 6173 6f66 742e 636f  pi.khulnasoft.co
+00002800: 6d2f 7265 6164 7961 7069 2d63 6c69 2f22  m/readyapi-cli/"
+00002810: 2074 6172 6765 743d 225f 626c 616e 6b22   target="_blank"
+00002820: 3e52 6561 6479 4150 4920 434c 4920 646f  >ReadyAPI CLI do
+00002830: 6373 3c2f 613e 2e0a 0a3c 2f64 6574 6169  cs</a>...</detai
+00002840: 6c73 3e0a 0a23 2323 2043 6865 636b 2069  ls>..### Check i
+00002850: 740a 0a4f 7065 6e20 796f 7572 2062 726f  t..Open your bro
+00002860: 7773 6572 2061 7420 3c61 2068 7265 663d  wser at <a href=
+00002870: 2268 7474 703a 2f2f 3132 372e 302e 302e  "http://127.0.0.
+00002880: 313a 3830 3030 2f69 7465 6d73 2f35 3f71  1:8000/items/5?q
+00002890: 3d73 6f6d 6571 7565 7279 2220 636c 6173  =somequery" clas
+000028a0: 733d 2265 7874 6572 6e61 6c2d 6c69 6e6b  s="external-link
+000028b0: 2220 7461 7267 6574 3d22 5f62 6c61 6e6b  " target="_blank
+000028c0: 223e 6874 7470 3a2f 2f31 3237 2e30 2e30  ">http://127.0.0
+000028d0: 2e31 3a38 3030 302f 6974 656d 732f 353f  .1:8000/items/5?
+000028e0: 713d 736f 6d65 7175 6572 793c 2f61 3e2e  q=somequery</a>.
+000028f0: 0a0a 596f 7520 7769 6c6c 2073 6565 2074  ..You will see t
+00002900: 6865 204a 534f 4e20 7265 7370 6f6e 7365  he JSON response
+00002910: 2061 733a 0a0a 6060 604a 534f 4e0a 7b22   as:..```JSON.{"
+00002920: 6974 656d 5f69 6422 3a20 352c 2022 7122  item_id": 5, "q"
+00002930: 3a20 2273 6f6d 6571 7565 7279 227d 0a60  : "somequery"}.`
+00002940: 6060 0a0a 596f 7520 616c 7265 6164 7920  ``..You already 
+00002950: 6372 6561 7465 6420 616e 2041 5049 2074  created an API t
+00002960: 6861 743a 0a0a 2a20 5265 6365 6976 6573  hat:..* Receives
+00002970: 2048 5454 5020 7265 7175 6573 7473 2069   HTTP requests i
+00002980: 6e20 7468 6520 5f70 6174 6873 5f20 602f  n the _paths_ `/
+00002990: 6020 616e 6420 602f 6974 656d 732f 7b69  ` and `/items/{i
+000029a0: 7465 6d5f 6964 7d60 2e0a 2a20 426f 7468  tem_id}`..* Both
+000029b0: 205f 7061 7468 735f 2074 616b 6520 6047   _paths_ take `G
+000029c0: 4554 6020 3c65 6d3e 6f70 6572 6174 696f  ET` <em>operatio
+000029d0: 6e73 3c2f 656d 3e20 2861 6c73 6f20 6b6e  ns</em> (also kn
+000029e0: 6f77 6e20 6173 2048 5454 5020 5f6d 6574  own as HTTP _met
+000029f0: 686f 6473 5f29 2e0a 2a20 5468 6520 5f70  hods_)..* The _p
+00002a00: 6174 685f 2060 2f69 7465 6d73 2f7b 6974  ath_ `/items/{it
+00002a10: 656d 5f69 647d 6020 6861 7320 6120 5f70  em_id}` has a _p
+00002a20: 6174 6820 7061 7261 6d65 7465 725f 2060  ath parameter_ `
+00002a30: 6974 656d 5f69 6460 2074 6861 7420 7368  item_id` that sh
+00002a40: 6f75 6c64 2062 6520 616e 2060 696e 7460  ould be an `int`
+00002a50: 2e0a 2a20 5468 6520 5f70 6174 685f 2060  ..* The _path_ `
+00002a60: 2f69 7465 6d73 2f7b 6974 656d 5f69 647d  /items/{item_id}
+00002a70: 6020 6861 7320 616e 206f 7074 696f 6e61  ` has an optiona
+00002a80: 6c20 6073 7472 6020 5f71 7565 7279 2070  l `str` _query p
+00002a90: 6172 616d 6574 6572 5f20 6071 602e 0a0a  arameter_ `q`...
+00002aa0: 2323 2320 496e 7465 7261 6374 6976 6520  ### Interactive 
+00002ab0: 4150 4920 646f 6373 0a0a 4e6f 7720 676f  API docs..Now go
+00002ac0: 2074 6f20 3c61 2068 7265 663d 2268 7474   to <a href="htt
+00002ad0: 703a 2f2f 3132 372e 302e 302e 313a 3830  p://127.0.0.1:80
+00002ae0: 3030 2f64 6f63 7322 2063 6c61 7373 3d22  00/docs" class="
+00002af0: 6578 7465 726e 616c 2d6c 696e 6b22 2074  external-link" t
+00002b00: 6172 6765 743d 225f 626c 616e 6b22 3e68  arget="_blank">h
+00002b10: 7474 703a 2f2f 3132 372e 302e 302e 313a  ttp://127.0.0.1:
+00002b20: 3830 3030 2f64 6f63 733c 2f61 3e2e 0a0a  8000/docs</a>...
+00002b30: 596f 7520 7769 6c6c 2073 6565 2074 6865  You will see the
+00002b40: 2061 7574 6f6d 6174 6963 2069 6e74 6572   automatic inter
+00002b50: 6163 7469 7665 2041 5049 2064 6f63 756d  active API docum
+00002b60: 656e 7461 7469 6f6e 2028 7072 6f76 6964  entation (provid
+00002b70: 6564 2062 7920 3c61 2068 7265 663d 2268  ed by <a href="h
+00002b80: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00002b90: 6d2f 7377 6167 6765 722d 6170 692f 7377  m/swagger-api/sw
+00002ba0: 6167 6765 722d 7569 2220 636c 6173 733d  agger-ui" class=
+00002bb0: 2265 7874 6572 6e61 6c2d 6c69 6e6b 2220  "external-link" 
+00002bc0: 7461 7267 6574 3d22 5f62 6c61 6e6b 223e  target="_blank">
+00002bd0: 5377 6167 6765 7220 5549 3c2f 613e 293a  Swagger UI</a>):
+00002be0: 0a0a 215b 5377 6167 6765 7220 5549 5d28  ..![Swagger UI](
+00002bf0: 6874 7470 733a 2f2f 7265 6164 7961 7069  https://readyapi
+00002c00: 2e6b 6875 6c6e 6173 6f66 742e 636f 6d2f  .khulnasoft.com/
+00002c10: 696d 672f 696e 6465 782f 696e 6465 782d  img/index/index-
+00002c20: 3031 2d73 7761 6767 6572 2d75 692d 7369  01-swagger-ui-si
+00002c30: 6d70 6c65 2e70 6e67 290a 0a23 2323 2041  mple.png)..### A
+00002c40: 6c74 6572 6e61 7469 7665 2041 5049 2064  lternative API d
+00002c50: 6f63 730a 0a41 6e64 206e 6f77 2c20 676f  ocs..And now, go
+00002c60: 2074 6f20 3c61 2068 7265 663d 2268 7474   to <a href="htt
+00002c70: 703a 2f2f 3132 372e 302e 302e 313a 3830  p://127.0.0.1:80
+00002c80: 3030 2f72 6564 6f63 2220 636c 6173 733d  00/redoc" class=
+00002c90: 2265 7874 6572 6e61 6c2d 6c69 6e6b 2220  "external-link" 
 00002ca0: 7461 7267 6574 3d22 5f62 6c61 6e6b 223e  target="_blank">
-00002cb0: 4578 706c 6f73 696f 6e20 4149 3c2f 613e  Explosion AI</a>
-00002cc0: 2066 6f75 6e64 6572 7320 2d20 3c61 2068   founders - <a h
-00002cd0: 7265 663d 2268 7474 7073 3a2f 2f73 7061  ref="https://spa
-00002ce0: 6379 2e69 6f22 2074 6172 6765 743d 225f  cy.io" target="_
-00002cf0: 626c 616e 6b22 3e73 7061 4379 3c2f 613e  blank">spaCy</a>
-00002d00: 2063 7265 6174 6f72 733c 2f73 7472 6f6e   creators</stron
-00002d10: 673e 203c 6120 6872 6566 3d22 6874 7470  g> <a href="http
-00002d20: 733a 2f2f 7477 6974 7465 722e 636f 6d2f  s://twitter.com/
-00002d30: 5f69 6e65 736d 6f6e 7461 6e69 2f73 7461  _inesmontani/sta
-00002d40: 7475 732f 3131 3434 3137 3332 3235 3332  tus/114417322532
-00002d50: 3231 3433 3734 3422 2074 6172 6765 743d  2143744" target=
-00002d60: 225f 626c 616e 6b22 3e3c 736d 616c 6c3e  "_blank"><small>
-00002d70: 2872 6566 293c 2f73 6d61 6c6c 3e3c 2f61  (ref)</small></a
-00002d80: 3e20 2d20 3c61 2068 7265 663d 2268 7474  > - <a href="htt
-00002d90: 7073 3a2f 2f74 7769 7474 6572 2e63 6f6d  ps://twitter.com
-00002da0: 2f68 6f6e 6e69 6261 6c2f 7374 6174 7573  /honnibal/status
-00002db0: 2f31 3134 3430 3331 3432 3138 3539 3635  /114403142185965
-00002dc0: 3536 3830 2220 7461 7267 6574 3d22 5f62  5680" target="_b
-00002dd0: 6c61 6e6b 223e 3c73 6d61 6c6c 3e28 7265  lank"><small>(re
-00002de0: 6629 3c2f 736d 616c 6c3e 3c2f 613e 3c2f  f)</small></a></
-00002df0: 6469 763e 0a0a 2d2d 2d0a 0a22 5f49 6620  div>..---.."_If 
-00002e00: 616e 796f 6e65 2069 7320 6c6f 6f6b 696e  anyone is lookin
-00002e10: 6720 746f 2062 7569 6c64 2061 2070 726f  g to build a pro
-00002e20: 6475 6374 696f 6e20 5079 7468 6f6e 2041  duction Python A
-00002e30: 5049 2c20 4920 776f 756c 6420 6869 6768  PI, I would high
-00002e40: 6c79 2072 6563 6f6d 6d65 6e64 202a 2a52  ly recommend **R
-00002e50: 6561 6479 4150 492a 2a2e 2049 7420 6973  eadyAPI**. It is
-00002e60: 202a 2a62 6561 7574 6966 756c 6c79 2064   **beautifully d
-00002e70: 6573 6967 6e65 642a 2a2c 202a 2a73 696d  esigned**, **sim
-00002e80: 706c 6520 746f 2075 7365 2a2a 2061 6e64  ple to use** and
-00002e90: 202a 2a68 6967 686c 7920 7363 616c 6162   **highly scalab
-00002ea0: 6c65 2a2a 2c20 6974 2068 6173 2062 6563  le**, it has bec
-00002eb0: 6f6d 6520 6120 2a2a 6b65 7920 636f 6d70  ome a **key comp
-00002ec0: 6f6e 656e 742a 2a20 696e 206f 7572 2041  onent** in our A
-00002ed0: 5049 2066 6972 7374 2064 6576 656c 6f70  PI first develop
-00002ee0: 6d65 6e74 2073 7472 6174 6567 7920 616e  ment strategy an
-00002ef0: 6420 6973 2064 7269 7669 6e67 206d 616e  d is driving man
-00002f00: 7920 6175 746f 6d61 7469 6f6e 7320 616e  y automations an
-00002f10: 6420 7365 7276 6963 6573 2073 7563 6820  d services such 
-00002f20: 6173 206f 7572 2056 6972 7475 616c 2054  as our Virtual T
-00002f30: 4143 2045 6e67 696e 6565 722e 5f22 0a0a  AC Engineer._"..
-00002f40: 3c64 6976 2073 7479 6c65 3d22 7465 7874  <div style="text
-00002f50: 2d61 6c69 676e 3a20 7269 6768 743b 206d  -align: right; m
-00002f60: 6172 6769 6e2d 7269 6768 743a 2031 3025  argin-right: 10%
-00002f70: 3b22 3e44 656f 6e20 5069 6c6c 7362 7572  ;">Deon Pillsbur
-00002f80: 7920 2d20 3c73 7472 6f6e 673e 4369 7363  y - <strong>Cisc
-00002f90: 6f3c 2f73 7472 6f6e 673e 203c 6120 6872  o</strong> <a hr
-00002fa0: 6566 3d22 6874 7470 733a 2f2f 7777 772e  ef="https://www.
-00002fb0: 6c69 6e6b 6564 696e 2e63 6f6d 2f70 6f73  linkedin.com/pos
-00002fc0: 7473 2f64 656f 6e70 696c 6c73 6275 7279  ts/deonpillsbury
-00002fd0: 5f63 6973 636f 2d63 782d 7079 7468 6f6e  _cisco-cx-python
-00002fe0: 2d61 6374 6976 6974 792d 3639 3633 3234  -activity-696324
-00002ff0: 3236 3238 3533 3634 3837 3933 362d 7472  2628536487936-tr
-00003000: 4170 2f22 2074 6172 6765 743d 225f 626c  Ap/" target="_bl
-00003010: 616e 6b22 3e3c 736d 616c 6c3e 2872 6566  ank"><small>(ref
-00003020: 293c 2f73 6d61 6c6c 3e3c 2f61 3e3c 2f64  )</small></a></d
-00003030: 6976 3e0a 0a2d 2d2d 0a0a 2323 202a 2a54  iv>..---..## **T
-00003040: 7970 6572 2a2a 2c20 7468 6520 5265 6164  yper**, the Read
-00003050: 7941 5049 206f 6620 434c 4973 0a0a 3c61  yAPI of CLIs..<a
-00003060: 2068 7265 663d 2268 7474 7073 3a2f 2f74   href="https://t
-00003070: 7970 6572 2e74 6961 6e67 6f6c 6f2e 636f  yper.tiangolo.co
-00003080: 6d22 2074 6172 6765 743d 225f 626c 616e  m" target="_blan
-00003090: 6b22 3e3c 696d 6720 7372 633d 2268 7474  k"><img src="htt
-000030a0: 7073 3a2f 2f74 7970 6572 2e74 6961 6e67  ps://typer.tiang
-000030b0: 6f6c 6f2e 636f 6d2f 696d 672f 6c6f 676f  olo.com/img/logo
-000030c0: 2d6d 6172 6769 6e2f 6c6f 676f 2d6d 6172  -margin/logo-mar
-000030d0: 6769 6e2d 7665 6374 6f72 2e73 7667 2220  gin-vector.svg" 
-000030e0: 7374 796c 653d 2277 6964 7468 3a20 3230  style="width: 20
-000030f0: 253b 223e 3c2f 613e 0a0a 4966 2079 6f75  %;"></a>..If you
-00003100: 2061 7265 2062 7569 6c64 696e 6720 6120   are building a 
-00003110: 3c61 6262 7220 7469 746c 653d 2243 6f6d  <abbr title="Com
-00003120: 6d61 6e64 204c 696e 6520 496e 7465 7266  mand Line Interf
-00003130: 6163 6522 3e43 4c49 3c2f 6162 6272 3e20  ace">CLI</abbr> 
-00003140: 6170 7020 746f 2062 6520 7573 6564 2069  app to be used i
-00003150: 6e20 7468 6520 7465 726d 696e 616c 2069  n the terminal i
-00003160: 6e73 7465 6164 206f 6620 6120 7765 6220  nstead of a web 
-00003170: 4150 492c 2063 6865 636b 206f 7574 203c  API, check out <
-00003180: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
-00003190: 7479 7065 722e 7469 616e 676f 6c6f 2e63  typer.tiangolo.c
-000031a0: 6f6d 2f22 2063 6c61 7373 3d22 6578 7465  om/" class="exte
-000031b0: 726e 616c 2d6c 696e 6b22 2074 6172 6765  rnal-link" targe
-000031c0: 743d 225f 626c 616e 6b22 3e2a 2a54 7970  t="_blank">**Typ
-000031d0: 6572 2a2a 3c2f 613e 2e0a 0a2a 2a54 7970  er**</a>...**Typ
-000031e0: 6572 2a2a 2069 7320 5265 6164 7941 5049  er** is ReadyAPI
-000031f0: 2773 206c 6974 746c 6520 7369 626c 696e  's little siblin
-00003200: 672e 2041 6e64 2069 7427 7320 696e 7465  g. And it's inte
-00003210: 6e64 6564 2074 6f20 6265 2074 6865 202a  nded to be the *
-00003220: 2a52 6561 6479 4150 4920 6f66 2043 4c49  *ReadyAPI of CLI
-00003230: 732a 2a2e 20e2 8ca8 efb8 8f20 f09f 9a80  s**. ...... ....
-00003240: 0a0a 2323 2052 6571 7569 7265 6d65 6e74  ..## Requirement
-00003250: 730a 0a50 7974 686f 6e20 332e 382b 0a0a  s..Python 3.8+..
-00003260: 5265 6164 7941 5049 2073 7461 6e64 7320  ReadyAPI stands 
-00003270: 6f6e 2074 6865 2073 686f 756c 6465 7273  on the shoulders
-00003280: 206f 6620 6769 616e 7473 3a0a 0a2a 203c   of giants:..* <
-00003290: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
-000032a0: 7777 772e 7374 6172 6c65 7474 652e 696f  www.starlette.io
-000032b0: 2f22 2063 6c61 7373 3d22 6578 7465 726e  /" class="extern
-000032c0: 616c 2d6c 696e 6b22 2074 6172 6765 743d  al-link" target=
-000032d0: 225f 626c 616e 6b22 3e53 7461 726c 6574  "_blank">Starlet
-000032e0: 7465 3c2f 613e 2066 6f72 2074 6865 2077  te</a> for the w
-000032f0: 6562 2070 6172 7473 2e0a 2a20 3c61 2068  eb parts..* <a h
-00003300: 7265 663d 2268 7474 7073 3a2f 2f64 6f63  ref="https://doc
-00003310: 732e 7079 6461 6e74 6963 2e64 6576 2f22  s.pydantic.dev/"
-00003320: 2063 6c61 7373 3d22 6578 7465 726e 616c   class="external
-00003330: 2d6c 696e 6b22 2074 6172 6765 743d 225f  -link" target="_
-00003340: 626c 616e 6b22 3e50 7964 616e 7469 633c  blank">Pydantic<
-00003350: 2f61 3e20 666f 7220 7468 6520 6461 7461  /a> for the data
-00003360: 2070 6172 7473 2e0a 0a23 2320 496e 7374   parts...## Inst
-00003370: 616c 6c61 7469 6f6e 0a0a 3c64 6976 2063  allation..<div c
-00003380: 6c61 7373 3d22 7465 726d 7922 3e0a 0a60  lass="termy">..`
-00003390: 6060 636f 6e73 6f6c 650a 2420 7069 7020  ``console.$ pip 
-000033a0: 696e 7374 616c 6c20 7265 6164 7961 7069  install readyapi
-000033b0: 0a0a 2d2d 2d3e 2031 3030 250a 6060 600a  ..---> 100%.```.
-000033c0: 0a3c 2f64 6976 3e0a 0a59 6f75 2077 696c  .</div>..You wil
-000033d0: 6c20 616c 736f 206e 6565 6420 616e 2041  l also need an A
-000033e0: 5347 4920 7365 7276 6572 2c20 666f 7220  SGI server, for 
-000033f0: 7072 6f64 7563 7469 6f6e 2073 7563 6820  production such 
-00003400: 6173 203c 6120 6872 6566 3d22 6874 7470  as <a href="http
-00003410: 733a 2f2f 7777 772e 7576 6963 6f72 6e2e  s://www.uvicorn.
-00003420: 6f72 6722 2063 6c61 7373 3d22 6578 7465  org" class="exte
-00003430: 726e 616c 2d6c 696e 6b22 2074 6172 6765  rnal-link" targe
-00003440: 743d 225f 626c 616e 6b22 3e55 7669 636f  t="_blank">Uvico
-00003450: 726e 3c2f 613e 206f 7220 3c61 2068 7265  rn</a> or <a hre
-00003460: 663d 2268 7474 7073 3a2f 2f67 6974 6875  f="https://githu
-00003470: 622e 636f 6d2f 7067 6a6f 6e65 732f 6879  b.com/pgjones/hy
-00003480: 7065 7263 6f72 6e22 2063 6c61 7373 3d22  percorn" class="
-00003490: 6578 7465 726e 616c 2d6c 696e 6b22 2074  external-link" t
-000034a0: 6172 6765 743d 225f 626c 616e 6b22 3e48  arget="_blank">H
-000034b0: 7970 6572 636f 726e 3c2f 613e 2e0a 0a3c  ypercorn</a>...<
-000034c0: 6469 7620 636c 6173 733d 2274 6572 6d79  div class="termy
-000034d0: 223e 0a0a 6060 6063 6f6e 736f 6c65 0a24  ">..```console.$
-000034e0: 2070 6970 2069 6e73 7461 6c6c 2022 7576   pip install "uv
-000034f0: 6963 6f72 6e5b 7374 616e 6461 7264 5d22  icorn[standard]"
-00003500: 0a0a 2d2d 2d3e 2031 3030 250a 6060 600a  ..---> 100%.```.
-00003510: 0a3c 2f64 6976 3e0a 0a23 2320 4578 616d  .</div>..## Exam
-00003520: 706c 650a 0a23 2323 2043 7265 6174 6520  ple..### Create 
-00003530: 6974 0a0a 2a20 4372 6561 7465 2061 2066  it..* Create a f
-00003540: 696c 6520 606d 6169 6e2e 7079 6020 7769  ile `main.py` wi
-00003550: 7468 3a0a 0a60 6060 5079 7468 6f6e 0a66  th:..```Python.f
-00003560: 726f 6d20 7479 7069 6e67 2069 6d70 6f72  rom typing impor
-00003570: 7420 556e 696f 6e0a 0a66 726f 6d20 7265  t Union..from re
-00003580: 6164 7961 7069 2069 6d70 6f72 7420 5265  adyapi import Re
-00003590: 6164 7941 5049 0a0a 6170 7020 3d20 5265  adyAPI..app = Re
-000035a0: 6164 7941 5049 2829 0a0a 0a40 6170 702e  adyAPI()...@app.
-000035b0: 6765 7428 222f 2229 0a64 6566 2072 6561  get("/").def rea
-000035c0: 645f 726f 6f74 2829 3a0a 2020 2020 7265  d_root():.    re
-000035d0: 7475 726e 207b 2248 656c 6c6f 223a 2022  turn {"Hello": "
-000035e0: 576f 726c 6422 7d0a 0a0a 4061 7070 2e67  World"}...@app.g
-000035f0: 6574 2822 2f69 7465 6d73 2f7b 6974 656d  et("/items/{item
-00003600: 5f69 647d 2229 0a64 6566 2072 6561 645f  _id}").def read_
-00003610: 6974 656d 2869 7465 6d5f 6964 3a20 696e  item(item_id: in
-00003620: 742c 2071 3a20 556e 696f 6e5b 7374 722c  t, q: Union[str,
-00003630: 204e 6f6e 655d 203d 204e 6f6e 6529 3a0a   None] = None):.
-00003640: 2020 2020 7265 7475 726e 207b 2269 7465      return {"ite
-00003650: 6d5f 6964 223a 2069 7465 6d5f 6964 2c20  m_id": item_id, 
-00003660: 2271 223a 2071 7d0a 6060 600a 0a3c 6465  "q": q}.```..<de
-00003670: 7461 696c 7320 6d61 726b 646f 776e 3d22  tails markdown="
-00003680: 3122 3e0a 3c73 756d 6d61 7279 3e4f 7220  1">.<summary>Or 
-00003690: 7573 6520 3c63 6f64 653e 6173 796e 6320  use <code>async 
-000036a0: 6465 663c 2f63 6f64 653e 2e2e 2e3c 2f73  def</code>...</s
-000036b0: 756d 6d61 7279 3e0a 0a49 6620 796f 7572  ummary>..If your
-000036c0: 2063 6f64 6520 7573 6573 2060 6173 796e   code uses `asyn
-000036d0: 6360 202f 2060 6177 6169 7460 2c20 7573  c` / `await`, us
-000036e0: 6520 6061 7379 6e63 2064 6566 603a 0a0a  e `async def`:..
-000036f0: 6060 6050 7974 686f 6e20 686c 5f6c 696e  ```Python hl_lin
-00003700: 6573 3d22 3920 2031 3422 0a66 726f 6d20  es="9  14".from 
-00003710: 7479 7069 6e67 2069 6d70 6f72 7420 556e  typing import Un
-00003720: 696f 6e0a 0a66 726f 6d20 7265 6164 7961  ion..from readya
-00003730: 7069 2069 6d70 6f72 7420 5265 6164 7941  pi import ReadyA
-00003740: 5049 0a0a 6170 7020 3d20 5265 6164 7941  PI..app = ReadyA
-00003750: 5049 2829 0a0a 0a40 6170 702e 6765 7428  PI()...@app.get(
-00003760: 222f 2229 0a61 7379 6e63 2064 6566 2072  "/").async def r
-00003770: 6561 645f 726f 6f74 2829 3a0a 2020 2020  ead_root():.    
-00003780: 7265 7475 726e 207b 2248 656c 6c6f 223a  return {"Hello":
-00003790: 2022 576f 726c 6422 7d0a 0a0a 4061 7070   "World"}...@app
-000037a0: 2e67 6574 2822 2f69 7465 6d73 2f7b 6974  .get("/items/{it
-000037b0: 656d 5f69 647d 2229 0a61 7379 6e63 2064  em_id}").async d
-000037c0: 6566 2072 6561 645f 6974 656d 2869 7465  ef read_item(ite
-000037d0: 6d5f 6964 3a20 696e 742c 2071 3a20 556e  m_id: int, q: Un
-000037e0: 696f 6e5b 7374 722c 204e 6f6e 655d 203d  ion[str, None] =
-000037f0: 204e 6f6e 6529 3a0a 2020 2020 7265 7475   None):.    retu
-00003800: 726e 207b 2269 7465 6d5f 6964 223a 2069  rn {"item_id": i
-00003810: 7465 6d5f 6964 2c20 2271 223a 2071 7d0a  tem_id, "q": q}.
-00003820: 6060 600a 0a2a 2a4e 6f74 652a 2a3a 0a0a  ```..**Note**:..
-00003830: 4966 2079 6f75 2064 6f6e 2774 206b 6e6f  If you don't kno
-00003840: 772c 2063 6865 636b 2074 6865 205f 2249  w, check the _"I
-00003850: 6e20 6120 6875 7272 793f 225f 2073 6563  n a hurry?"_ sec
-00003860: 7469 6f6e 2061 626f 7574 203c 6120 6872  tion about <a hr
-00003870: 6566 3d22 6874 7470 733a 2f2f 7265 6164  ef="https://read
-00003880: 7961 7069 2e6b 6875 6c6e 6173 6f66 742e  yapi.khulnasoft.
-00003890: 636f 6d2f 6173 796e 632f 2369 6e2d 612d  com/async/#in-a-
-000038a0: 6875 7272 7922 2074 6172 6765 743d 225f  hurry" target="_
-000038b0: 626c 616e 6b22 3e60 6173 796e 6360 2061  blank">`async` a
-000038c0: 6e64 2060 6177 6169 7460 2069 6e20 7468  nd `await` in th
-000038d0: 6520 646f 6373 3c2f 613e 2e0a 0a3c 2f64  e docs</a>...</d
-000038e0: 6574 6169 6c73 3e0a 0a23 2323 2052 756e  etails>..### Run
-000038f0: 2069 740a 0a52 756e 2074 6865 2073 6572   it..Run the ser
-00003900: 7665 7220 7769 7468 3a0a 0a3c 6469 7620  ver with:..<div 
-00003910: 636c 6173 733d 2274 6572 6d79 223e 0a0a  class="termy">..
-00003920: 6060 6063 6f6e 736f 6c65 0a24 2075 7669  ```console.$ uvi
-00003930: 636f 726e 206d 6169 6e3a 6170 7020 2d2d  corn main:app --
-00003940: 7265 6c6f 6164 0a0a 494e 464f 3a20 2020  reload..INFO:   
-00003950: 2020 5576 6963 6f72 6e20 7275 6e6e 696e    Uvicorn runnin
-00003960: 6720 6f6e 2068 7474 703a 2f2f 3132 372e  g on http://127.
-00003970: 302e 302e 313a 3830 3030 2028 5072 6573  0.0.1:8000 (Pres
-00003980: 7320 4354 524c 2b43 2074 6f20 7175 6974  s CTRL+C to quit
-00003990: 290a 494e 464f 3a20 2020 2020 5374 6172  ).INFO:     Star
-000039a0: 7465 6420 7265 6c6f 6164 6572 2070 726f  ted reloader pro
-000039b0: 6365 7373 205b 3238 3732 305d 0a49 4e46  cess [28720].INF
-000039c0: 4f3a 2020 2020 2053 7461 7274 6564 2073  O:     Started s
-000039d0: 6572 7665 7220 7072 6f63 6573 7320 5b32  erver process [2
-000039e0: 3837 3232 5d0a 494e 464f 3a20 2020 2020  8722].INFO:     
-000039f0: 5761 6974 696e 6720 666f 7220 6170 706c  Waiting for appl
-00003a00: 6963 6174 696f 6e20 7374 6172 7475 702e  ication startup.
-00003a10: 0a49 4e46 4f3a 2020 2020 2041 7070 6c69  .INFO:     Appli
-00003a20: 6361 7469 6f6e 2073 7461 7274 7570 2063  cation startup c
-00003a30: 6f6d 706c 6574 652e 0a60 6060 0a0a 3c2f  omplete..```..</
-00003a40: 6469 763e 0a0a 3c64 6574 6169 6c73 206d  div>..<details m
-00003a50: 6172 6b64 6f77 6e3d 2231 223e 0a3c 7375  arkdown="1">.<su
-00003a60: 6d6d 6172 793e 4162 6f75 7420 7468 6520  mmary>About the 
-00003a70: 636f 6d6d 616e 6420 3c63 6f64 653e 7576  command <code>uv
-00003a80: 6963 6f72 6e20 6d61 696e 3a61 7070 202d  icorn main:app -
-00003a90: 2d72 656c 6f61 643c 2f63 6f64 653e 2e2e  -reload</code>..
-00003aa0: 2e3c 2f73 756d 6d61 7279 3e0a 0a54 6865  .</summary>..The
-00003ab0: 2063 6f6d 6d61 6e64 2060 7576 6963 6f72   command `uvicor
-00003ac0: 6e20 6d61 696e 3a61 7070 6020 7265 6665  n main:app` refe
-00003ad0: 7273 2074 6f3a 0a0a 2a20 606d 6169 6e60  rs to:..* `main`
-00003ae0: 3a20 7468 6520 6669 6c65 2060 6d61 696e  : the file `main
-00003af0: 2e70 7960 2028 7468 6520 5079 7468 6f6e  .py` (the Python
-00003b00: 2022 6d6f 6475 6c65 2229 2e0a 2a20 6061   "module")..* `a
-00003b10: 7070 603a 2074 6865 206f 626a 6563 7420  pp`: the object 
-00003b20: 6372 6561 7465 6420 696e 7369 6465 206f  created inside o
-00003b30: 6620 606d 6169 6e2e 7079 6020 7769 7468  f `main.py` with
-00003b40: 2074 6865 206c 696e 6520 6061 7070 203d   the line `app =
-00003b50: 2052 6561 6479 4150 4928 2960 2e0a 2a20   ReadyAPI()`..* 
-00003b60: 602d 2d72 656c 6f61 6460 3a20 6d61 6b65  `--reload`: make
-00003b70: 2074 6865 2073 6572 7665 7220 7265 7374   the server rest
-00003b80: 6172 7420 6166 7465 7220 636f 6465 2063  art after code c
-00003b90: 6861 6e67 6573 2e20 4f6e 6c79 2064 6f20  hanges. Only do 
-00003ba0: 7468 6973 2066 6f72 2064 6576 656c 6f70  this for develop
-00003bb0: 6d65 6e74 2e0a 0a3c 2f64 6574 6169 6c73  ment...</details
-00003bc0: 3e0a 0a23 2323 2043 6865 636b 2069 740a  >..### Check it.
-00003bd0: 0a4f 7065 6e20 796f 7572 2062 726f 7773  .Open your brows
-00003be0: 6572 2061 7420 3c61 2068 7265 663d 2268  er at <a href="h
-00003bf0: 7474 703a 2f2f 3132 372e 302e 302e 313a  ttp://127.0.0.1:
-00003c00: 3830 3030 2f69 7465 6d73 2f35 3f71 3d73  8000/items/5?q=s
-00003c10: 6f6d 6571 7565 7279 2220 636c 6173 733d  omequery" class=
-00003c20: 2265 7874 6572 6e61 6c2d 6c69 6e6b 2220  "external-link" 
-00003c30: 7461 7267 6574 3d22 5f62 6c61 6e6b 223e  target="_blank">
-00003c40: 6874 7470 3a2f 2f31 3237 2e30 2e30 2e31  http://127.0.0.1
-00003c50: 3a38 3030 302f 6974 656d 732f 353f 713d  :8000/items/5?q=
-00003c60: 736f 6d65 7175 6572 793c 2f61 3e2e 0a0a  somequery</a>...
-00003c70: 596f 7520 7769 6c6c 2073 6565 2074 6865  You will see the
-00003c80: 204a 534f 4e20 7265 7370 6f6e 7365 2061   JSON response a
-00003c90: 733a 0a0a 6060 604a 534f 4e0a 7b22 6974  s:..```JSON.{"it
-00003ca0: 656d 5f69 6422 3a20 352c 2022 7122 3a20  em_id": 5, "q": 
-00003cb0: 2273 6f6d 6571 7565 7279 227d 0a60 6060  "somequery"}.```
-00003cc0: 0a0a 596f 7520 616c 7265 6164 7920 6372  ..You already cr
-00003cd0: 6561 7465 6420 616e 2041 5049 2074 6861  eated an API tha
-00003ce0: 743a 0a0a 2a20 5265 6365 6976 6573 2048  t:..* Receives H
-00003cf0: 5454 5020 7265 7175 6573 7473 2069 6e20  TTP requests in 
-00003d00: 7468 6520 5f70 6174 6873 5f20 602f 6020  the _paths_ `/` 
-00003d10: 616e 6420 602f 6974 656d 732f 7b69 7465  and `/items/{ite
-00003d20: 6d5f 6964 7d60 2e0a 2a20 426f 7468 205f  m_id}`..* Both _
-00003d30: 7061 7468 735f 2074 616b 6520 6047 4554  paths_ take `GET
-00003d40: 6020 3c65 6d3e 6f70 6572 6174 696f 6e73  ` <em>operations
-00003d50: 3c2f 656d 3e20 2861 6c73 6f20 6b6e 6f77  </em> (also know
-00003d60: 6e20 6173 2048 5454 5020 5f6d 6574 686f  n as HTTP _metho
-00003d70: 6473 5f29 2e0a 2a20 5468 6520 5f70 6174  ds_)..* The _pat
-00003d80: 685f 2060 2f69 7465 6d73 2f7b 6974 656d  h_ `/items/{item
-00003d90: 5f69 647d 6020 6861 7320 6120 5f70 6174  _id}` has a _pat
-00003da0: 6820 7061 7261 6d65 7465 725f 2060 6974  h parameter_ `it
-00003db0: 656d 5f69 6460 2074 6861 7420 7368 6f75  em_id` that shou
-00003dc0: 6c64 2062 6520 616e 2060 696e 7460 2e0a  ld be an `int`..
-00003dd0: 2a20 5468 6520 5f70 6174 685f 2060 2f69  * The _path_ `/i
-00003de0: 7465 6d73 2f7b 6974 656d 5f69 647d 6020  tems/{item_id}` 
-00003df0: 6861 7320 616e 206f 7074 696f 6e61 6c20  has an optional 
-00003e00: 6073 7472 6020 5f71 7565 7279 2070 6172  `str` _query par
-00003e10: 616d 6574 6572 5f20 6071 602e 0a0a 2323  ameter_ `q`...##
-00003e20: 2320 496e 7465 7261 6374 6976 6520 4150  # Interactive AP
-00003e30: 4920 646f 6373 0a0a 4e6f 7720 676f 2074  I docs..Now go t
-00003e40: 6f20 3c61 2068 7265 663d 2268 7474 703a  o <a href="http:
-00003e50: 2f2f 3132 372e 302e 302e 313a 3830 3030  //127.0.0.1:8000
-00003e60: 2f64 6f63 7322 2063 6c61 7373 3d22 6578  /docs" class="ex
-00003e70: 7465 726e 616c 2d6c 696e 6b22 2074 6172  ternal-link" tar
-00003e80: 6765 743d 225f 626c 616e 6b22 3e68 7474  get="_blank">htt
-00003e90: 703a 2f2f 3132 372e 302e 302e 313a 3830  p://127.0.0.1:80
-00003ea0: 3030 2f64 6f63 733c 2f61 3e2e 0a0a 596f  00/docs</a>...Yo
-00003eb0: 7520 7769 6c6c 2073 6565 2074 6865 2061  u will see the a
-00003ec0: 7574 6f6d 6174 6963 2069 6e74 6572 6163  utomatic interac
-00003ed0: 7469 7665 2041 5049 2064 6f63 756d 656e  tive API documen
-00003ee0: 7461 7469 6f6e 2028 7072 6f76 6964 6564  tation (provided
-00003ef0: 2062 7920 3c61 2068 7265 663d 2268 7474   by <a href="htt
-00003f00: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00003f10: 7377 6167 6765 722d 6170 692f 7377 6167  swagger-api/swag
-00003f20: 6765 722d 7569 2220 636c 6173 733d 2265  ger-ui" class="e
-00003f30: 7874 6572 6e61 6c2d 6c69 6e6b 2220 7461  xternal-link" ta
-00003f40: 7267 6574 3d22 5f62 6c61 6e6b 223e 5377  rget="_blank">Sw
-00003f50: 6167 6765 7220 5549 3c2f 613e 293a 0a0a  agger UI</a>):..
-00003f60: 215b 5377 6167 6765 7220 5549 5d28 6874  ![Swagger UI](ht
-00003f70: 7470 733a 2f2f 7265 6164 7961 7069 2e6b  tps://readyapi.k
-00003f80: 6875 6c6e 6173 6f66 742e 636f 6d2f 696d  hulnasoft.com/im
-00003f90: 672f 696e 6465 782f 696e 6465 782d 3031  g/index/index-01
-00003fa0: 2d73 7761 6767 6572 2d75 692d 7369 6d70  -swagger-ui-simp
-00003fb0: 6c65 2e70 6e67 290a 0a23 2323 2041 6c74  le.png)..### Alt
-00003fc0: 6572 6e61 7469 7665 2041 5049 2064 6f63  ernative API doc
-00003fd0: 730a 0a41 6e64 206e 6f77 2c20 676f 2074  s..And now, go t
-00003fe0: 6f20 3c61 2068 7265 663d 2268 7474 703a  o <a href="http:
-00003ff0: 2f2f 3132 372e 302e 302e 313a 3830 3030  //127.0.0.1:8000
-00004000: 2f72 6564 6f63 2220 636c 6173 733d 2265  /redoc" class="e
-00004010: 7874 6572 6e61 6c2d 6c69 6e6b 2220 7461  xternal-link" ta
-00004020: 7267 6574 3d22 5f62 6c61 6e6b 223e 6874  rget="_blank">ht
-00004030: 7470 3a2f 2f31 3237 2e30 2e30 2e31 3a38  tp://127.0.0.1:8
-00004040: 3030 302f 7265 646f 633c 2f61 3e2e 0a0a  000/redoc</a>...
-00004050: 596f 7520 7769 6c6c 2073 6565 2074 6865  You will see the
-00004060: 2061 6c74 6572 6e61 7469 7665 2061 7574   alternative aut
-00004070: 6f6d 6174 6963 2064 6f63 756d 656e 7461  omatic documenta
-00004080: 7469 6f6e 2028 7072 6f76 6964 6564 2062  tion (provided b
-00004090: 7920 3c61 2068 7265 663d 2268 7474 7073  y <a href="https
-000040a0: 3a2f 2f67 6974 6875 622e 636f 6d2f 5265  ://github.com/Re
-000040b0: 6269 6c6c 792f 5265 446f 6322 2063 6c61  billy/ReDoc" cla
-000040c0: 7373 3d22 6578 7465 726e 616c 2d6c 696e  ss="external-lin
-000040d0: 6b22 2074 6172 6765 743d 225f 626c 616e  k" target="_blan
-000040e0: 6b22 3e52 6544 6f63 3c2f 613e 293a 0a0a  k">ReDoc</a>):..
-000040f0: 215b 5265 446f 635d 2868 7474 7073 3a2f  ![ReDoc](https:/
-00004100: 2f72 6561 6479 6170 692e 6b68 756c 6e61  /readyapi.khulna
-00004110: 736f 6674 2e63 6f6d 2f69 6d67 2f69 6e64  soft.com/img/ind
-00004120: 6578 2f69 6e64 6578 2d30 322d 7265 646f  ex/index-02-redo
-00004130: 632d 7369 6d70 6c65 2e70 6e67 290a 0a23  c-simple.png)..#
-00004140: 2320 4578 616d 706c 6520 7570 6772 6164  # Example upgrad
-00004150: 650a 0a4e 6f77 206d 6f64 6966 7920 7468  e..Now modify th
-00004160: 6520 6669 6c65 2060 6d61 696e 2e70 7960  e file `main.py`
-00004170: 2074 6f20 7265 6365 6976 6520 6120 626f   to receive a bo
-00004180: 6479 2066 726f 6d20 6120 6050 5554 6020  dy from a `PUT` 
-00004190: 7265 7175 6573 742e 0a0a 4465 636c 6172  request...Declar
-000041a0: 6520 7468 6520 626f 6479 2075 7369 6e67  e the body using
-000041b0: 2073 7461 6e64 6172 6420 5079 7468 6f6e   standard Python
-000041c0: 2074 7970 6573 2c20 7468 616e 6b73 2074   types, thanks t
-000041d0: 6f20 5079 6461 6e74 6963 2e0a 0a60 6060  o Pydantic...```
-000041e0: 5079 7468 6f6e 2068 6c5f 6c69 6e65 733d  Python hl_lines=
-000041f0: 2234 2020 392d 3132 2020 3235 2d32 3722  "4  9-12  25-27"
-00004200: 0a66 726f 6d20 7479 7069 6e67 2069 6d70  .from typing imp
-00004210: 6f72 7420 556e 696f 6e0a 0a66 726f 6d20  ort Union..from 
-00004220: 7265 6164 7961 7069 2069 6d70 6f72 7420  readyapi import 
-00004230: 5265 6164 7941 5049 0a66 726f 6d20 7079  ReadyAPI.from py
-00004240: 6461 6e74 6963 2069 6d70 6f72 7420 4261  dantic import Ba
-00004250: 7365 4d6f 6465 6c0a 0a61 7070 203d 2052  seModel..app = R
-00004260: 6561 6479 4150 4928 290a 0a0a 636c 6173  eadyAPI()...clas
-00004270: 7320 4974 656d 2842 6173 654d 6f64 656c  s Item(BaseModel
-00004280: 293a 0a20 2020 206e 616d 653a 2073 7472  ):.    name: str
-00004290: 0a20 2020 2070 7269 6365 3a20 666c 6f61  .    price: floa
-000042a0: 740a 2020 2020 6973 5f6f 6666 6572 3a20  t.    is_offer: 
-000042b0: 556e 696f 6e5b 626f 6f6c 2c20 4e6f 6e65  Union[bool, None
-000042c0: 5d20 3d20 4e6f 6e65 0a0a 0a40 6170 702e  ] = None...@app.
-000042d0: 6765 7428 222f 2229 0a64 6566 2072 6561  get("/").def rea
-000042e0: 645f 726f 6f74 2829 3a0a 2020 2020 7265  d_root():.    re
-000042f0: 7475 726e 207b 2248 656c 6c6f 223a 2022  turn {"Hello": "
-00004300: 576f 726c 6422 7d0a 0a0a 4061 7070 2e67  World"}...@app.g
-00004310: 6574 2822 2f69 7465 6d73 2f7b 6974 656d  et("/items/{item
-00004320: 5f69 647d 2229 0a64 6566 2072 6561 645f  _id}").def read_
-00004330: 6974 656d 2869 7465 6d5f 6964 3a20 696e  item(item_id: in
-00004340: 742c 2071 3a20 556e 696f 6e5b 7374 722c  t, q: Union[str,
-00004350: 204e 6f6e 655d 203d 204e 6f6e 6529 3a0a   None] = None):.
-00004360: 2020 2020 7265 7475 726e 207b 2269 7465      return {"ite
-00004370: 6d5f 6964 223a 2069 7465 6d5f 6964 2c20  m_id": item_id, 
-00004380: 2271 223a 2071 7d0a 0a0a 4061 7070 2e70  "q": q}...@app.p
-00004390: 7574 2822 2f69 7465 6d73 2f7b 6974 656d  ut("/items/{item
-000043a0: 5f69 647d 2229 0a64 6566 2075 7064 6174  _id}").def updat
-000043b0: 655f 6974 656d 2869 7465 6d5f 6964 3a20  e_item(item_id: 
-000043c0: 696e 742c 2069 7465 6d3a 2049 7465 6d29  int, item: Item)
-000043d0: 3a0a 2020 2020 7265 7475 726e 207b 2269  :.    return {"i
-000043e0: 7465 6d5f 6e61 6d65 223a 2069 7465 6d2e  tem_name": item.
-000043f0: 6e61 6d65 2c20 2269 7465 6d5f 6964 223a  name, "item_id":
-00004400: 2069 7465 6d5f 6964 7d0a 6060 600a 0a54   item_id}.```..T
-00004410: 6865 2073 6572 7665 7220 7368 6f75 6c64  he server should
-00004420: 2072 656c 6f61 6420 6175 746f 6d61 7469   reload automati
-00004430: 6361 6c6c 7920 2862 6563 6175 7365 2079  cally (because y
-00004440: 6f75 2061 6464 6564 2060 2d2d 7265 6c6f  ou added `--relo
-00004450: 6164 6020 746f 2074 6865 2060 7576 6963  ad` to the `uvic
-00004460: 6f72 6e60 2063 6f6d 6d61 6e64 2061 626f  orn` command abo
-00004470: 7665 292e 0a0a 2323 2320 496e 7465 7261  ve)...### Intera
-00004480: 6374 6976 6520 4150 4920 646f 6373 2075  ctive API docs u
-00004490: 7067 7261 6465 0a0a 4e6f 7720 676f 2074  pgrade..Now go t
-000044a0: 6f20 3c61 2068 7265 663d 2268 7474 703a  o <a href="http:
-000044b0: 2f2f 3132 372e 302e 302e 313a 3830 3030  //127.0.0.1:8000
-000044c0: 2f64 6f63 7322 2063 6c61 7373 3d22 6578  /docs" class="ex
-000044d0: 7465 726e 616c 2d6c 696e 6b22 2074 6172  ternal-link" tar
-000044e0: 6765 743d 225f 626c 616e 6b22 3e68 7474  get="_blank">htt
-000044f0: 703a 2f2f 3132 372e 302e 302e 313a 3830  p://127.0.0.1:80
-00004500: 3030 2f64 6f63 733c 2f61 3e2e 0a0a 2a20  00/docs</a>...* 
-00004510: 5468 6520 696e 7465 7261 6374 6976 6520  The interactive 
-00004520: 4150 4920 646f 6375 6d65 6e74 6174 696f  API documentatio
-00004530: 6e20 7769 6c6c 2062 6520 6175 746f 6d61  n will be automa
-00004540: 7469 6361 6c6c 7920 7570 6461 7465 642c  tically updated,
-00004550: 2069 6e63 6c75 6469 6e67 2074 6865 206e   including the n
-00004560: 6577 2062 6f64 793a 0a0a 215b 5377 6167  ew body:..![Swag
-00004570: 6765 7220 5549 5d28 6874 7470 733a 2f2f  ger UI](https://
-00004580: 7265 6164 7961 7069 2e6b 6875 6c6e 6173  readyapi.khulnas
-00004590: 6f66 742e 636f 6d2f 696d 672f 696e 6465  oft.com/img/inde
-000045a0: 782f 696e 6465 782d 3033 2d73 7761 6767  x/index-03-swagg
-000045b0: 6572 2d30 322e 706e 6729 0a0a 2a20 436c  er-02.png)..* Cl
-000045c0: 6963 6b20 6f6e 2074 6865 2062 7574 746f  ick on the butto
-000045d0: 6e20 2254 7279 2069 7420 6f75 7422 2c20  n "Try it out", 
-000045e0: 6974 2061 6c6c 6f77 7320 796f 7520 746f  it allows you to
-000045f0: 2066 696c 6c20 7468 6520 7061 7261 6d65   fill the parame
-00004600: 7465 7273 2061 6e64 2064 6972 6563 746c  ters and directl
-00004610: 7920 696e 7465 7261 6374 2077 6974 6820  y interact with 
-00004620: 7468 6520 4150 493a 0a0a 215b 5377 6167  the API:..![Swag
-00004630: 6765 7220 5549 2069 6e74 6572 6163 7469  ger UI interacti
-00004640: 6f6e 5d28 6874 7470 733a 2f2f 7265 6164  on](https://read
-00004650: 7961 7069 2e6b 6875 6c6e 6173 6f66 742e  yapi.khulnasoft.
-00004660: 636f 6d2f 696d 672f 696e 6465 782f 696e  com/img/index/in
-00004670: 6465 782d 3034 2d73 7761 6767 6572 2d30  dex-04-swagger-0
-00004680: 332e 706e 6729 0a0a 2a20 5468 656e 2063  3.png)..* Then c
-00004690: 6c69 636b 206f 6e20 7468 6520 2245 7865  lick on the "Exe
-000046a0: 6375 7465 2220 6275 7474 6f6e 2c20 7468  cute" button, th
-000046b0: 6520 7573 6572 2069 6e74 6572 6661 6365  e user interface
-000046c0: 2077 696c 6c20 636f 6d6d 756e 6963 6174   will communicat
-000046d0: 6520 7769 7468 2079 6f75 7220 4150 492c  e with your API,
-000046e0: 2073 656e 6420 7468 6520 7061 7261 6d65   send the parame
-000046f0: 7465 7273 2c20 6765 7420 7468 6520 7265  ters, get the re
-00004700: 7375 6c74 7320 616e 6420 7368 6f77 2074  sults and show t
-00004710: 6865 6d20 6f6e 2074 6865 2073 6372 6565  hem on the scree
-00004720: 6e3a 0a0a 215b 5377 6167 6765 7220 5549  n:..![Swagger UI
-00004730: 2069 6e74 6572 6163 7469 6f6e 5d28 6874   interaction](ht
-00004740: 7470 733a 2f2f 7265 6164 7961 7069 2e6b  tps://readyapi.k
-00004750: 6875 6c6e 6173 6f66 742e 636f 6d2f 696d  hulnasoft.com/im
-00004760: 672f 696e 6465 782f 696e 6465 782d 3035  g/index/index-05
-00004770: 2d73 7761 6767 6572 2d30 342e 706e 6729  -swagger-04.png)
-00004780: 0a0a 2323 2320 416c 7465 726e 6174 6976  ..### Alternativ
-00004790: 6520 4150 4920 646f 6373 2075 7067 7261  e API docs upgra
-000047a0: 6465 0a0a 416e 6420 6e6f 772c 2067 6f20  de..And now, go 
-000047b0: 746f 203c 6120 6872 6566 3d22 6874 7470  to <a href="http
-000047c0: 3a2f 2f31 3237 2e30 2e30 2e31 3a38 3030  ://127.0.0.1:800
-000047d0: 302f 7265 646f 6322 2063 6c61 7373 3d22  0/redoc" class="
-000047e0: 6578 7465 726e 616c 2d6c 696e 6b22 2074  external-link" t
-000047f0: 6172 6765 743d 225f 626c 616e 6b22 3e68  arget="_blank">h
-00004800: 7474 703a 2f2f 3132 372e 302e 302e 313a  ttp://127.0.0.1:
-00004810: 3830 3030 2f72 6564 6f63 3c2f 613e 2e0a  8000/redoc</a>..
-00004820: 0a2a 2054 6865 2061 6c74 6572 6e61 7469  .* The alternati
-00004830: 7665 2064 6f63 756d 656e 7461 7469 6f6e  ve documentation
-00004840: 2077 696c 6c20 616c 736f 2072 6566 6c65   will also refle
-00004850: 6374 2074 6865 206e 6577 2071 7565 7279  ct the new query
-00004860: 2070 6172 616d 6574 6572 2061 6e64 2062   parameter and b
-00004870: 6f64 793a 0a0a 215b 5265 446f 635d 2868  ody:..![ReDoc](h
-00004880: 7474 7073 3a2f 2f72 6561 6479 6170 692e  ttps://readyapi.
-00004890: 6b68 756c 6e61 736f 6674 2e63 6f6d 2f69  khulnasoft.com/i
-000048a0: 6d67 2f69 6e64 6578 2f69 6e64 6578 2d30  mg/index/index-0
-000048b0: 362d 7265 646f 632d 3032 2e70 6e67 290a  6-redoc-02.png).
-000048c0: 0a23 2323 2052 6563 6170 0a0a 496e 2073  .### Recap..In s
-000048d0: 756d 6d61 7279 2c20 796f 7520 6465 636c  ummary, you decl
-000048e0: 6172 6520 2a2a 6f6e 6365 2a2a 2074 6865  are **once** the
-000048f0: 2074 7970 6573 206f 6620 7061 7261 6d65   types of parame
-00004900: 7465 7273 2c20 626f 6479 2c20 6574 632e  ters, body, etc.
-00004910: 2061 7320 6675 6e63 7469 6f6e 2070 6172   as function par
-00004920: 616d 6574 6572 732e 0a0a 596f 7520 646f  ameters...You do
-00004930: 2074 6861 7420 7769 7468 2073 7461 6e64   that with stand
-00004940: 6172 6420 6d6f 6465 726e 2050 7974 686f  ard modern Pytho
-00004950: 6e20 7479 7065 732e 0a0a 596f 7520 646f  n types...You do
-00004960: 6e27 7420 6861 7665 2074 6f20 6c65 6172  n't have to lear
-00004970: 6e20 6120 6e65 7720 7379 6e74 6178 2c20  n a new syntax, 
-00004980: 7468 6520 6d65 7468 6f64 7320 6f72 2063  the methods or c
-00004990: 6c61 7373 6573 206f 6620 6120 7370 6563  lasses of a spec
-000049a0: 6966 6963 206c 6962 7261 7279 2c20 6574  ific library, et
-000049b0: 632e 0a0a 4a75 7374 2073 7461 6e64 6172  c...Just standar
-000049c0: 6420 2a2a 5079 7468 6f6e 2033 2e38 2b2a  d **Python 3.8+*
-000049d0: 2a2e 0a0a 466f 7220 6578 616d 706c 652c  *...For example,
-000049e0: 2066 6f72 2061 6e20 6069 6e74 603a 0a0a   for an `int`:..
-000049f0: 6060 6050 7974 686f 6e0a 6974 656d 5f69  ```Python.item_i
-00004a00: 643a 2069 6e74 0a60 6060 0a0a 6f72 2066  d: int.```..or f
-00004a10: 6f72 2061 206d 6f72 6520 636f 6d70 6c65  or a more comple
-00004a20: 7820 6049 7465 6d60 206d 6f64 656c 3a0a  x `Item` model:.
-00004a30: 0a60 6060 5079 7468 6f6e 0a69 7465 6d3a  .```Python.item:
-00004a40: 2049 7465 6d0a 6060 600a 0a2e 2e2e 616e   Item.```.....an
-00004a50: 6420 7769 7468 2074 6861 7420 7369 6e67  d with that sing
-00004a60: 6c65 2064 6563 6c61 7261 7469 6f6e 2079  le declaration y
-00004a70: 6f75 2067 6574 3a0a 0a2a 2045 6469 746f  ou get:..* Edito
-00004a80: 7220 7375 7070 6f72 742c 2069 6e63 6c75  r support, inclu
-00004a90: 6469 6e67 3a0a 2020 2020 2a20 436f 6d70  ding:.    * Comp
-00004aa0: 6c65 7469 6f6e 2e0a 2020 2020 2a20 5479  letion..    * Ty
-00004ab0: 7065 2063 6865 636b 732e 0a2a 2056 616c  pe checks..* Val
-00004ac0: 6964 6174 696f 6e20 6f66 2064 6174 613a  idation of data:
-00004ad0: 0a20 2020 202a 2041 7574 6f6d 6174 6963  .    * Automatic
-00004ae0: 2061 6e64 2063 6c65 6172 2065 7272 6f72   and clear error
-00004af0: 7320 7768 656e 2074 6865 2064 6174 6120  s when the data 
-00004b00: 6973 2069 6e76 616c 6964 2e0a 2020 2020  is invalid..    
-00004b10: 2a20 5661 6c69 6461 7469 6f6e 2065 7665  * Validation eve
-00004b20: 6e20 666f 7220 6465 6570 6c79 206e 6573  n for deeply nes
-00004b30: 7465 6420 4a53 4f4e 206f 626a 6563 7473  ted JSON objects
-00004b40: 2e0a 2a20 3c61 6262 7220 7469 746c 653d  ..* <abbr title=
-00004b50: 2261 6c73 6f20 6b6e 6f77 6e20 6173 3a20  "also known as: 
-00004b60: 7365 7269 616c 697a 6174 696f 6e2c 2070  serialization, p
-00004b70: 6172 7369 6e67 2c20 6d61 7273 6861 6c6c  arsing, marshall
-00004b80: 696e 6722 3e43 6f6e 7665 7273 696f 6e3c  ing">Conversion<
-00004b90: 2f61 6262 723e 206f 6620 696e 7075 7420  /abbr> of input 
-00004ba0: 6461 7461 3a20 636f 6d69 6e67 2066 726f  data: coming fro
-00004bb0: 6d20 7468 6520 6e65 7477 6f72 6b20 746f  m the network to
-00004bc0: 2050 7974 686f 6e20 6461 7461 2061 6e64   Python data and
-00004bd0: 2074 7970 6573 2e20 5265 6164 696e 6720   types. Reading 
-00004be0: 6672 6f6d 3a0a 2020 2020 2a20 4a53 4f4e  from:.    * JSON
-00004bf0: 2e0a 2020 2020 2a20 5061 7468 2070 6172  ..    * Path par
-00004c00: 616d 6574 6572 732e 0a20 2020 202a 2051  ameters..    * Q
-00004c10: 7565 7279 2070 6172 616d 6574 6572 732e  uery parameters.
-00004c20: 0a20 2020 202a 2043 6f6f 6b69 6573 2e0a  .    * Cookies..
-00004c30: 2020 2020 2a20 4865 6164 6572 732e 0a20      * Headers.. 
-00004c40: 2020 202a 2046 6f72 6d73 2e0a 2020 2020     * Forms..    
-00004c50: 2a20 4669 6c65 732e 0a2a 203c 6162 6272  * Files..* <abbr
-00004c60: 2074 6974 6c65 3d22 616c 736f 206b 6e6f   title="also kno
-00004c70: 776e 2061 733a 2073 6572 6961 6c69 7a61  wn as: serializa
-00004c80: 7469 6f6e 2c20 7061 7273 696e 672c 206d  tion, parsing, m
-00004c90: 6172 7368 616c 6c69 6e67 223e 436f 6e76  arshalling">Conv
-00004ca0: 6572 7369 6f6e 3c2f 6162 6272 3e20 6f66  ersion</abbr> of
-00004cb0: 206f 7574 7075 7420 6461 7461 3a20 636f   output data: co
-00004cc0: 6e76 6572 7469 6e67 2066 726f 6d20 5079  nverting from Py
-00004cd0: 7468 6f6e 2064 6174 6120 616e 6420 7479  thon data and ty
-00004ce0: 7065 7320 746f 206e 6574 776f 726b 2064  pes to network d
-00004cf0: 6174 6120 2861 7320 4a53 4f4e 293a 0a20  ata (as JSON):. 
-00004d00: 2020 202a 2043 6f6e 7665 7274 2050 7974     * Convert Pyt
-00004d10: 686f 6e20 7479 7065 7320 2860 7374 7260  hon types (`str`
-00004d20: 2c20 6069 6e74 602c 2060 666c 6f61 7460  , `int`, `float`
-00004d30: 2c20 6062 6f6f 6c60 2c20 606c 6973 7460  , `bool`, `list`
-00004d40: 2c20 6574 6329 2e0a 2020 2020 2a20 6064  , etc)..    * `d
-00004d50: 6174 6574 696d 6560 206f 626a 6563 7473  atetime` objects
-00004d60: 2e0a 2020 2020 2a20 6055 5549 4460 206f  ..    * `UUID` o
-00004d70: 626a 6563 7473 2e0a 2020 2020 2a20 4461  bjects..    * Da
-00004d80: 7461 6261 7365 206d 6f64 656c 732e 0a20  tabase models.. 
-00004d90: 2020 202a 202e 2e2e 616e 6420 6d61 6e79     * ...and many
-00004da0: 206d 6f72 652e 0a2a 2041 7574 6f6d 6174   more..* Automat
-00004db0: 6963 2069 6e74 6572 6163 7469 7665 2041  ic interactive A
-00004dc0: 5049 2064 6f63 756d 656e 7461 7469 6f6e  PI documentation
-00004dd0: 2c20 696e 636c 7564 696e 6720 3220 616c  , including 2 al
-00004de0: 7465 726e 6174 6976 6520 7573 6572 2069  ternative user i
-00004df0: 6e74 6572 6661 6365 733a 0a20 2020 202a  nterfaces:.    *
-00004e00: 2053 7761 6767 6572 2055 492e 0a20 2020   Swagger UI..   
-00004e10: 202a 2052 6544 6f63 2e0a 0a2d 2d2d 0a0a   * ReDoc...---..
-00004e20: 436f 6d69 6e67 2062 6163 6b20 746f 2074  Coming back to t
-00004e30: 6865 2070 7265 7669 6f75 7320 636f 6465  he previous code
-00004e40: 2065 7861 6d70 6c65 2c20 2a2a 5265 6164   example, **Read
-00004e50: 7941 5049 2a2a 2077 696c 6c3a 0a0a 2a20  yAPI** will:..* 
-00004e60: 5661 6c69 6461 7465 2074 6861 7420 7468  Validate that th
-00004e70: 6572 6520 6973 2061 6e20 6069 7465 6d5f  ere is an `item_
-00004e80: 6964 6020 696e 2074 6865 2070 6174 6820  id` in the path 
-00004e90: 666f 7220 6047 4554 6020 616e 6420 6050  for `GET` and `P
-00004ea0: 5554 6020 7265 7175 6573 7473 2e0a 2a20  UT` requests..* 
-00004eb0: 5661 6c69 6461 7465 2074 6861 7420 7468  Validate that th
-00004ec0: 6520 6069 7465 6d5f 6964 6020 6973 206f  e `item_id` is o
-00004ed0: 6620 7479 7065 2060 696e 7460 2066 6f72  f type `int` for
-00004ee0: 2060 4745 5460 2061 6e64 2060 5055 5460   `GET` and `PUT`
-00004ef0: 2072 6571 7565 7374 732e 0a20 2020 202a   requests..    *
-00004f00: 2049 6620 6974 2069 7320 6e6f 742c 2074   If it is not, t
-00004f10: 6865 2063 6c69 656e 7420 7769 6c6c 2073  he client will s
-00004f20: 6565 2061 2075 7365 6675 6c2c 2063 6c65  ee a useful, cle
-00004f30: 6172 2065 7272 6f72 2e0a 2a20 4368 6563  ar error..* Chec
-00004f40: 6b20 6966 2074 6865 7265 2069 7320 616e  k if there is an
-00004f50: 206f 7074 696f 6e61 6c20 7175 6572 7920   optional query 
-00004f60: 7061 7261 6d65 7465 7220 6e61 6d65 6420  parameter named 
-00004f70: 6071 6020 2861 7320 696e 2060 6874 7470  `q` (as in `http
-00004f80: 3a2f 2f31 3237 2e30 2e30 2e31 3a38 3030  ://127.0.0.1:800
-00004f90: 302f 6974 656d 732f 666f 6f3f 713d 736f  0/items/foo?q=so
-00004fa0: 6d65 7175 6572 7960 2920 666f 7220 6047  mequery`) for `G
-00004fb0: 4554 6020 7265 7175 6573 7473 2e0a 2020  ET` requests..  
-00004fc0: 2020 2a20 4173 2074 6865 2060 7160 2070    * As the `q` p
-00004fd0: 6172 616d 6574 6572 2069 7320 6465 636c  arameter is decl
-00004fe0: 6172 6564 2077 6974 6820 603d 204e 6f6e  ared with `= Non
-00004ff0: 6560 2c20 6974 2069 7320 6f70 7469 6f6e  e`, it is option
-00005000: 616c 2e0a 2020 2020 2a20 5769 7468 6f75  al..    * Withou
-00005010: 7420 7468 6520 604e 6f6e 6560 2069 7420  t the `None` it 
-00005020: 776f 756c 6420 6265 2072 6571 7569 7265  would be require
-00005030: 6420 2861 7320 6973 2074 6865 2062 6f64  d (as is the bod
-00005040: 7920 696e 2074 6865 2063 6173 6520 7769  y in the case wi
-00005050: 7468 2060 5055 5460 292e 0a2a 2046 6f72  th `PUT`)..* For
-00005060: 2060 5055 5460 2072 6571 7565 7374 7320   `PUT` requests 
-00005070: 746f 2060 2f69 7465 6d73 2f7b 6974 656d  to `/items/{item
-00005080: 5f69 647d 602c 2052 6561 6420 7468 6520  _id}`, Read the 
-00005090: 626f 6479 2061 7320 4a53 4f4e 3a0a 2020  body as JSON:.  
-000050a0: 2020 2a20 4368 6563 6b20 7468 6174 2069    * Check that i
-000050b0: 7420 6861 7320 6120 7265 7175 6972 6564  t has a required
-000050c0: 2061 7474 7269 6275 7465 2060 6e61 6d65   attribute `name
-000050d0: 6020 7468 6174 2073 686f 756c 6420 6265  ` that should be
-000050e0: 2061 2060 7374 7260 2e0a 2020 2020 2a20   a `str`..    * 
-000050f0: 4368 6563 6b20 7468 6174 2069 7420 6861  Check that it ha
-00005100: 7320 6120 7265 7175 6972 6564 2061 7474  s a required att
-00005110: 7269 6275 7465 2060 7072 6963 6560 2074  ribute `price` t
-00005120: 6861 7420 6861 7320 746f 2062 6520 6120  hat has to be a 
-00005130: 6066 6c6f 6174 602e 0a20 2020 202a 2043  `float`..    * C
-00005140: 6865 636b 2074 6861 7420 6974 2068 6173  heck that it has
-00005150: 2061 6e20 6f70 7469 6f6e 616c 2061 7474   an optional att
-00005160: 7269 6275 7465 2060 6973 5f6f 6666 6572  ribute `is_offer
-00005170: 602c 2074 6861 7420 7368 6f75 6c64 2062  `, that should b
-00005180: 6520 6120 6062 6f6f 6c60 2c20 6966 2070  e a `bool`, if p
-00005190: 7265 7365 6e74 2e0a 2020 2020 2a20 416c  resent..    * Al
-000051a0: 6c20 7468 6973 2077 6f75 6c64 2061 6c73  l this would als
-000051b0: 6f20 776f 726b 2066 6f72 2064 6565 706c  o work for deepl
-000051c0: 7920 6e65 7374 6564 204a 534f 4e20 6f62  y nested JSON ob
-000051d0: 6a65 6374 732e 0a2a 2043 6f6e 7665 7274  jects..* Convert
-000051e0: 2066 726f 6d20 616e 6420 746f 204a 534f   from and to JSO
-000051f0: 4e20 6175 746f 6d61 7469 6361 6c6c 792e  N automatically.
-00005200: 0a2a 2044 6f63 756d 656e 7420 6576 6572  .* Document ever
-00005210: 7974 6869 6e67 2077 6974 6820 4f70 656e  ything with Open
-00005220: 4150 492c 2074 6861 7420 6361 6e20 6265  API, that can be
-00005230: 2075 7365 6420 6279 3a0a 2020 2020 2a20   used by:.    * 
-00005240: 496e 7465 7261 6374 6976 6520 646f 6375  Interactive docu
-00005250: 6d65 6e74 6174 696f 6e20 7379 7374 656d  mentation system
-00005260: 732e 0a20 2020 202a 2041 7574 6f6d 6174  s..    * Automat
-00005270: 6963 2063 6c69 656e 7420 636f 6465 2067  ic client code g
-00005280: 656e 6572 6174 696f 6e20 7379 7374 656d  eneration system
-00005290: 732c 2066 6f72 206d 616e 7920 6c61 6e67  s, for many lang
-000052a0: 7561 6765 732e 0a2a 2050 726f 7669 6465  uages..* Provide
-000052b0: 2032 2069 6e74 6572 6163 7469 7665 2064   2 interactive d
-000052c0: 6f63 756d 656e 7461 7469 6f6e 2077 6562  ocumentation web
-000052d0: 2069 6e74 6572 6661 6365 7320 6469 7265   interfaces dire
-000052e0: 6374 6c79 2e0a 0a2d 2d2d 0a0a 5765 206a  ctly...---..We j
-000052f0: 7573 7420 7363 7261 7463 6865 6420 7468  ust scratched th
-00005300: 6520 7375 7266 6163 652c 2062 7574 2079  e surface, but y
-00005310: 6f75 2061 6c72 6561 6479 2067 6574 2074  ou already get t
-00005320: 6865 2069 6465 6120 6f66 2068 6f77 2069  he idea of how i
-00005330: 7420 616c 6c20 776f 726b 732e 0a0a 5472  t all works...Tr
-00005340: 7920 6368 616e 6769 6e67 2074 6865 206c  y changing the l
-00005350: 696e 6520 7769 7468 3a0a 0a60 6060 5079  ine with:..```Py
-00005360: 7468 6f6e 0a20 2020 2072 6574 7572 6e20  thon.    return 
-00005370: 7b22 6974 656d 5f6e 616d 6522 3a20 6974  {"item_name": it
-00005380: 656d 2e6e 616d 652c 2022 6974 656d 5f69  em.name, "item_i
-00005390: 6422 3a20 6974 656d 5f69 647d 0a60 6060  d": item_id}.```
-000053a0: 0a0a 2e2e 2e66 726f 6d3a 0a0a 6060 6050  .....from:..```P
-000053b0: 7974 686f 6e0a 2020 2020 2020 2020 2e2e  ython.        ..
-000053c0: 2e20 2269 7465 6d5f 6e61 6d65 223a 2069  . "item_name": i
-000053d0: 7465 6d2e 6e61 6d65 202e 2e2e 0a60 6060  tem.name ....```
-000053e0: 0a0a 2e2e 2e74 6f3a 0a0a 6060 6050 7974  .....to:..```Pyt
-000053f0: 686f 6e0a 2020 2020 2020 2020 2e2e 2e20  hon.        ... 
-00005400: 2269 7465 6d5f 7072 6963 6522 3a20 6974  "item_price": it
-00005410: 656d 2e70 7269 6365 202e 2e2e 0a60 6060  em.price ....```
-00005420: 0a0a 2e2e 2e61 6e64 2073 6565 2068 6f77  .....and see how
-00005430: 2079 6f75 7220 6564 6974 6f72 2077 696c   your editor wil
-00005440: 6c20 6175 746f 2d63 6f6d 706c 6574 6520  l auto-complete 
-00005450: 7468 6520 6174 7472 6962 7574 6573 2061  the attributes a
-00005460: 6e64 206b 6e6f 7720 7468 6569 7220 7479  nd know their ty
-00005470: 7065 733a 0a0a 215b 6564 6974 6f72 2073  pes:..![editor s
-00005480: 7570 706f 7274 5d28 6874 7470 733a 2f2f  upport](https://
-00005490: 7265 6164 7961 7069 2e6b 6875 6c6e 6173  readyapi.khulnas
-000054a0: 6f66 742e 636f 6d2f 696d 672f 7673 636f  oft.com/img/vsco
-000054b0: 6465 2d63 6f6d 706c 6574 696f 6e2e 706e  de-completion.pn
-000054c0: 6729 0a0a 466f 7220 6120 6d6f 7265 2063  g)..For a more c
-000054d0: 6f6d 706c 6574 6520 6578 616d 706c 6520  omplete example 
-000054e0: 696e 636c 7564 696e 6720 6d6f 7265 2066  including more f
-000054f0: 6561 7475 7265 732c 2073 6565 2074 6865  eatures, see the
-00005500: 203c 6120 6872 6566 3d22 6874 7470 733a   <a href="https:
-00005510: 2f2f 7265 6164 7961 7069 2e6b 6875 6c6e  //readyapi.khuln
-00005520: 6173 6f66 742e 636f 6d2f 7475 746f 7269  asoft.com/tutori
-00005530: 616c 2f22 3e54 7574 6f72 6961 6c20 2d20  al/">Tutorial - 
-00005540: 5573 6572 2047 7569 6465 3c2f 613e 2e0a  User Guide</a>..
-00005550: 0a2a 2a53 706f 696c 6572 2061 6c65 7274  .**Spoiler alert
-00005560: 2a2a 3a20 7468 6520 7475 746f 7269 616c  **: the tutorial
-00005570: 202d 2075 7365 7220 6775 6964 6520 696e   - user guide in
-00005580: 636c 7564 6573 3a0a 0a2a 2044 6563 6c61  cludes:..* Decla
-00005590: 7261 7469 6f6e 206f 6620 2a2a 7061 7261  ration of **para
-000055a0: 6d65 7465 7273 2a2a 2066 726f 6d20 6f74  meters** from ot
-000055b0: 6865 7220 6469 6666 6572 656e 7420 706c  her different pl
-000055c0: 6163 6573 2061 733a 202a 2a68 6561 6465  aces as: **heade
-000055d0: 7273 2a2a 2c20 2a2a 636f 6f6b 6965 732a  rs**, **cookies*
-000055e0: 2a2c 202a 2a66 6f72 6d20 6669 656c 6473  *, **form fields
-000055f0: 2a2a 2061 6e64 202a 2a66 696c 6573 2a2a  ** and **files**
-00005600: 2e0a 2a20 486f 7720 746f 2073 6574 202a  ..* How to set *
-00005610: 2a76 616c 6964 6174 696f 6e20 636f 6e73  *validation cons
-00005620: 7472 6169 6e74 732a 2a20 6173 2060 6d61  traints** as `ma
-00005630: 7869 6d75 6d5f 6c65 6e67 7468 6020 6f72  ximum_length` or
-00005640: 2060 7265 6765 7860 2e0a 2a20 4120 7665   `regex`..* A ve
-00005650: 7279 2070 6f77 6572 6675 6c20 616e 6420  ry powerful and 
-00005660: 6561 7379 2074 6f20 7573 6520 2a2a 3c61  easy to use **<a
-00005670: 6262 7220 7469 746c 653d 2261 6c73 6f20  bbr title="also 
-00005680: 6b6e 6f77 6e20 6173 2063 6f6d 706f 6e65  known as compone
-00005690: 6e74 732c 2072 6573 6f75 7263 6573 2c20  nts, resources, 
-000056a0: 7072 6f76 6964 6572 732c 2073 6572 7669  providers, servi
-000056b0: 6365 732c 2069 6e6a 6563 7461 626c 6573  ces, injectables
-000056c0: 223e 4465 7065 6e64 656e 6379 2049 6e6a  ">Dependency Inj
-000056d0: 6563 7469 6f6e 3c2f 6162 6272 3e2a 2a20  ection</abbr>** 
-000056e0: 7379 7374 656d 2e0a 2a20 5365 6375 7269  system..* Securi
-000056f0: 7479 2061 6e64 2061 7574 6865 6e74 6963  ty and authentic
-00005700: 6174 696f 6e2c 2069 6e63 6c75 6469 6e67  ation, including
-00005710: 2073 7570 706f 7274 2066 6f72 202a 2a4f   support for **O
-00005720: 4175 7468 322a 2a20 7769 7468 202a 2a4a  Auth2** with **J
-00005730: 5754 2074 6f6b 656e 732a 2a20 616e 6420  WT tokens** and 
-00005740: 2a2a 4854 5450 2042 6173 6963 2a2a 2061  **HTTP Basic** a
-00005750: 7574 682e 0a2a 204d 6f72 6520 6164 7661  uth..* More adva
-00005760: 6e63 6564 2028 6275 7420 6571 7561 6c6c  nced (but equall
-00005770: 7920 6561 7379 2920 7465 6368 6e69 7175  y easy) techniqu
-00005780: 6573 2066 6f72 2064 6563 6c61 7269 6e67  es for declaring
-00005790: 202a 2a64 6565 706c 7920 6e65 7374 6564   **deeply nested
-000057a0: 204a 534f 4e20 6d6f 6465 6c73 2a2a 2028   JSON models** (
-000057b0: 7468 616e 6b73 2074 6f20 5079 6461 6e74  thanks to Pydant
-000057c0: 6963 292e 0a2a 202a 2a47 7261 7068 514c  ic)..* **GraphQL
-000057d0: 2a2a 2069 6e74 6567 7261 7469 6f6e 2077  ** integration w
-000057e0: 6974 6820 3c61 2068 7265 663d 2268 7474  ith <a href="htt
-000057f0: 7073 3a2f 2f73 7472 6177 6265 7272 792e  ps://strawberry.
-00005800: 726f 636b 7322 2063 6c61 7373 3d22 6578  rocks" class="ex
-00005810: 7465 726e 616c 2d6c 696e 6b22 2074 6172  ternal-link" tar
-00005820: 6765 743d 225f 626c 616e 6b22 3e53 7472  get="_blank">Str
-00005830: 6177 6265 7272 793c 2f61 3e20 616e 6420  awberry</a> and 
-00005840: 6f74 6865 7220 6c69 6272 6172 6965 732e  other libraries.
-00005850: 0a2a 204d 616e 7920 6578 7472 6120 6665  .* Many extra fe
-00005860: 6174 7572 6573 2028 7468 616e 6b73 2074  atures (thanks t
-00005870: 6f20 5374 6172 6c65 7474 6529 2061 733a  o Starlette) as:
-00005880: 0a20 2020 202a 202a 2a57 6562 536f 636b  .    * **WebSock
-00005890: 6574 732a 2a0a 2020 2020 2a20 6578 7472  ets**.    * extr
-000058a0: 656d 656c 7920 6561 7379 2074 6573 7473  emely easy tests
-000058b0: 2062 6173 6564 206f 6e20 4854 5450 5820   based on HTTPX 
-000058c0: 616e 6420 6070 7974 6573 7460 0a20 2020  and `pytest`.   
-000058d0: 202a 202a 2a43 4f52 532a 2a0a 2020 2020   * **CORS**.    
-000058e0: 2a20 2a2a 436f 6f6b 6965 2053 6573 7369  * **Cookie Sessi
-000058f0: 6f6e 732a 2a0a 2020 2020 2a20 2e2e 2e61  ons**.    * ...a
-00005900: 6e64 206d 6f72 652e 0a0a 2323 2050 6572  nd more...## Per
-00005910: 666f 726d 616e 6365 0a0a 496e 6465 7065  formance..Indepe
-00005920: 6e64 656e 7420 5465 6368 456d 706f 7765  ndent TechEmpowe
-00005930: 7220 6265 6e63 686d 6172 6b73 2073 686f  r benchmarks sho
-00005940: 7720 2a2a 5265 6164 7941 5049 2a2a 2061  w **ReadyAPI** a
-00005950: 7070 6c69 6361 7469 6f6e 7320 7275 6e6e  pplications runn
-00005960: 696e 6720 756e 6465 7220 5576 6963 6f72  ing under Uvicor
-00005970: 6e20 6173 203c 6120 6872 6566 3d22 6874  n as <a href="ht
-00005980: 7470 733a 2f2f 7777 772e 7465 6368 656d  tps://www.techem
-00005990: 706f 7765 722e 636f 6d2f 6265 6e63 686d  power.com/benchm
-000059a0: 6172 6b73 2f23 7365 6374 696f 6e3d 7465  arks/#section=te
-000059b0: 7374 2672 756e 6964 3d37 3436 3465 3532  st&runid=7464e52
-000059c0: 302d 3064 6332 2d34 3733 642d 6264 3334  0-0dc2-473d-bd34
-000059d0: 2d64 6264 6664 3765 3835 3931 3126 6877  -dbdfd7e85911&hw
-000059e0: 3d70 6826 7465 7374 3d71 7565 7279 266c  =ph&test=query&l
-000059f0: 3d7a 696a 7a65 6e2d 3722 2063 6c61 7373  =zijzen-7" class
-00005a00: 3d22 6578 7465 726e 616c 2d6c 696e 6b22  ="external-link"
-00005a10: 2074 6172 6765 743d 225f 626c 616e 6b22   target="_blank"
-00005a20: 3e6f 6e65 206f 6620 7468 6520 6661 7374  >one of the fast
-00005a30: 6573 7420 5079 7468 6f6e 2066 7261 6d65  est Python frame
-00005a40: 776f 726b 7320 6176 6169 6c61 626c 653c  works available<
-00005a50: 2f61 3e2c 206f 6e6c 7920 6265 6c6f 7720  /a>, only below 
-00005a60: 5374 6172 6c65 7474 6520 616e 6420 5576  Starlette and Uv
-00005a70: 6963 6f72 6e20 7468 656d 7365 6c76 6573  icorn themselves
-00005a80: 2028 7573 6564 2069 6e74 6572 6e61 6c6c   (used internall
-00005a90: 7920 6279 2052 6561 6479 4150 4929 2e20  y by ReadyAPI). 
-00005aa0: 282a 290a 0a54 6f20 756e 6465 7273 7461  (*)..To understa
-00005ab0: 6e64 206d 6f72 6520 6162 6f75 7420 6974  nd more about it
-00005ac0: 2c20 7365 6520 7468 6520 7365 6374 696f  , see the sectio
-00005ad0: 6e20 3c61 2068 7265 663d 2268 7474 7073  n <a href="https
-00005ae0: 3a2f 2f72 6561 6479 6170 692e 6b68 756c  ://readyapi.khul
-00005af0: 6e61 736f 6674 2e63 6f6d 2f62 656e 6368  nasoft.com/bench
-00005b00: 6d61 726b 732f 2220 636c 6173 733d 2269  marks/" class="i
-00005b10: 6e74 6572 6e61 6c2d 6c69 6e6b 2220 7461  nternal-link" ta
-00005b20: 7267 6574 3d22 5f62 6c61 6e6b 223e 4265  rget="_blank">Be
-00005b30: 6e63 686d 6172 6b73 3c2f 613e 2e0a 0a23  nchmarks</a>...#
-00005b40: 2320 4f70 7469 6f6e 616c 2044 6570 656e  # Optional Depen
-00005b50: 6465 6e63 6965 730a 0a55 7365 6420 6279  dencies..Used by
-00005b60: 2050 7964 616e 7469 633a 0a0a 2a20 3c61   Pydantic:..* <a
-00005b70: 2068 7265 663d 2268 7474 7073 3a2f 2f67   href="https://g
-00005b80: 6974 6875 622e 636f 6d2f 4a6f 7368 4461  ithub.com/JoshDa
-00005b90: 7461 2f70 7974 686f 6e2d 656d 6169 6c2d  ta/python-email-
-00005ba0: 7661 6c69 6461 746f 7222 2074 6172 6765  validator" targe
-00005bb0: 743d 225f 626c 616e 6b22 3e3c 636f 6465  t="_blank"><code
-00005bc0: 3e65 6d61 696c 5f76 616c 6964 6174 6f72  >email_validator
-00005bd0: 3c2f 636f 6465 3e3c 2f61 3e20 2d20 666f  </code></a> - fo
-00005be0: 7220 656d 6169 6c20 7661 6c69 6461 7469  r email validati
-00005bf0: 6f6e 2e0a 2a20 3c61 2068 7265 663d 2268  on..* <a href="h
-00005c00: 7474 7073 3a2f 2f64 6f63 732e 7079 6461  ttps://docs.pyda
-00005c10: 6e74 6963 2e64 6576 2f6c 6174 6573 742f  ntic.dev/latest/
-00005c20: 7573 6167 652f 7079 6461 6e74 6963 5f73  usage/pydantic_s
-00005c30: 6574 7469 6e67 732f 2220 7461 7267 6574  ettings/" target
-00005c40: 3d22 5f62 6c61 6e6b 223e 3c63 6f64 653e  ="_blank"><code>
-00005c50: 7079 6461 6e74 6963 2d73 6574 7469 6e67  pydantic-setting
-00005c60: 733c 2f63 6f64 653e 3c2f 613e 202d 2066  s</code></a> - f
-00005c70: 6f72 2073 6574 7469 6e67 7320 6d61 6e61  or settings mana
-00005c80: 6765 6d65 6e74 2e0a 2a20 3c61 2068 7265  gement..* <a hre
-00005c90: 663d 2268 7474 7073 3a2f 2f64 6f63 732e  f="https://docs.
-00005ca0: 7079 6461 6e74 6963 2e64 6576 2f6c 6174  pydantic.dev/lat
-00005cb0: 6573 742f 7573 6167 652f 7479 7065 732f  est/usage/types/
-00005cc0: 6578 7472 615f 7479 7065 732f 6578 7472  extra_types/extr
-00005cd0: 615f 7479 7065 732f 2220 7461 7267 6574  a_types/" target
-00005ce0: 3d22 5f62 6c61 6e6b 223e 3c63 6f64 653e  ="_blank"><code>
-00005cf0: 7079 6461 6e74 6963 2d65 7874 7261 2d74  pydantic-extra-t
-00005d00: 7970 6573 3c2f 636f 6465 3e3c 2f61 3e20  ypes</code></a> 
-00005d10: 2d20 666f 7220 6578 7472 6120 7479 7065  - for extra type
-00005d20: 7320 746f 2062 6520 7573 6564 2077 6974  s to be used wit
-00005d30: 6820 5079 6461 6e74 6963 2e0a 0a55 7365  h Pydantic...Use
-00005d40: 6420 6279 2053 7461 726c 6574 7465 3a0a  d by Starlette:.
-00005d50: 0a2a 203c 6120 6872 6566 3d22 6874 7470  .* <a href="http
-00005d60: 733a 2f2f 7777 772e 7079 7468 6f6e 2d68  s://www.python-h
-00005d70: 7474 7078 2e6f 7267 2220 7461 7267 6574  ttpx.org" target
-00005d80: 3d22 5f62 6c61 6e6b 223e 3c63 6f64 653e  ="_blank"><code>
-00005d90: 6874 7470 783c 2f63 6f64 653e 3c2f 613e  httpx</code></a>
-00005da0: 202d 2052 6571 7569 7265 6420 6966 2079   - Required if y
-00005db0: 6f75 2077 616e 7420 746f 2075 7365 2074  ou want to use t
-00005dc0: 6865 2060 5465 7374 436c 6965 6e74 602e  he `TestClient`.
-00005dd0: 0a2a 203c 6120 6872 6566 3d22 6874 7470  .* <a href="http
-00005de0: 733a 2f2f 6a69 6e6a 612e 7061 6c6c 6574  s://jinja.pallet
-00005df0: 7370 726f 6a65 6374 732e 636f 6d22 2074  sprojects.com" t
-00005e00: 6172 6765 743d 225f 626c 616e 6b22 3e3c  arget="_blank"><
-00005e10: 636f 6465 3e6a 696e 6a61 323c 2f63 6f64  code>jinja2</cod
-00005e20: 653e 3c2f 613e 202d 2052 6571 7569 7265  e></a> - Require
-00005e30: 6420 6966 2079 6f75 2077 616e 7420 746f  d if you want to
-00005e40: 2075 7365 2074 6865 2064 6566 6175 6c74   use the default
-00005e50: 2074 656d 706c 6174 6520 636f 6e66 6967   template config
-00005e60: 7572 6174 696f 6e2e 0a2a 203c 6120 6872  uration..* <a hr
-00005e70: 6566 3d22 6874 7470 733a 2f2f 6769 7468  ef="https://gith
-00005e80: 7562 2e63 6f6d 2f4b 6c75 6465 782f 7079  ub.com/Kludex/py
-00005e90: 7468 6f6e 2d6d 756c 7469 7061 7274 2220  thon-multipart" 
-00005ea0: 7461 7267 6574 3d22 5f62 6c61 6e6b 223e  target="_blank">
-00005eb0: 3c63 6f64 653e 7079 7468 6f6e 2d6d 756c  <code>python-mul
-00005ec0: 7469 7061 7274 3c2f 636f 6465 3e3c 2f61  tipart</code></a
-00005ed0: 3e20 2d20 5265 7175 6972 6564 2069 6620  > - Required if 
-00005ee0: 796f 7520 7761 6e74 2074 6f20 7375 7070  you want to supp
-00005ef0: 6f72 7420 666f 726d 203c 6162 6272 2074  ort form <abbr t
-00005f00: 6974 6c65 3d22 636f 6e76 6572 7469 6e67  itle="converting
-00005f10: 2074 6865 2073 7472 696e 6720 7468 6174   the string that
-00005f20: 2063 6f6d 6573 2066 726f 6d20 616e 2048   comes from an H
-00005f30: 5454 5020 7265 7175 6573 7420 696e 746f  TTP request into
-00005f40: 2050 7974 686f 6e20 6461 7461 223e 2270   Python data">"p
-00005f50: 6172 7369 6e67 223c 2f61 6262 723e 2c20  arsing"</abbr>, 
-00005f60: 7769 7468 2060 7265 7175 6573 742e 666f  with `request.fo
-00005f70: 726d 2829 602e 0a2a 203c 6120 6872 6566  rm()`..* <a href
-00005f80: 3d22 6874 7470 733a 2f2f 7079 7468 6f6e  ="https://python
-00005f90: 686f 7374 6564 2e6f 7267 2f69 7473 6461  hosted.org/itsda
-00005fa0: 6e67 6572 6f75 732f 2220 7461 7267 6574  ngerous/" target
-00005fb0: 3d22 5f62 6c61 6e6b 223e 3c63 6f64 653e  ="_blank"><code>
-00005fc0: 6974 7364 616e 6765 726f 7573 3c2f 636f  itsdangerous</co
-00005fd0: 6465 3e3c 2f61 3e20 2d20 5265 7175 6972  de></a> - Requir
-00005fe0: 6564 2066 6f72 2060 5365 7373 696f 6e4d  ed for `SessionM
-00005ff0: 6964 646c 6577 6172 6560 2073 7570 706f  iddleware` suppo
-00006000: 7274 2e0a 2a20 3c61 2068 7265 663d 2268  rt..* <a href="h
-00006010: 7474 7073 3a2f 2f70 7979 616d 6c2e 6f72  ttps://pyyaml.or
-00006020: 672f 7769 6b69 2f50 7959 414d 4c44 6f63  g/wiki/PyYAMLDoc
-00006030: 756d 656e 7461 7469 6f6e 2220 7461 7267  umentation" targ
-00006040: 6574 3d22 5f62 6c61 6e6b 223e 3c63 6f64  et="_blank"><cod
-00006050: 653e 7079 7961 6d6c 3c2f 636f 6465 3e3c  e>pyyaml</code><
-00006060: 2f61 3e20 2d20 5265 7175 6972 6564 2066  /a> - Required f
-00006070: 6f72 2053 7461 726c 6574 7465 2773 2060  or Starlette's `
-00006080: 5363 6865 6d61 4765 6e65 7261 746f 7260  SchemaGenerator`
-00006090: 2073 7570 706f 7274 2028 796f 7520 7072   support (you pr
-000060a0: 6f62 6162 6c79 2064 6f6e 2774 206e 6565  obably don't nee
-000060b0: 6420 6974 2077 6974 6820 5265 6164 7941  d it with ReadyA
-000060c0: 5049 292e 0a2a 203c 6120 6872 6566 3d22  PI)..* <a href="
-000060d0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-000060e0: 6f6d 2f65 736e 6d65 2f75 6c74 7261 6a73  om/esnme/ultrajs
-000060f0: 6f6e 2220 7461 7267 6574 3d22 5f62 6c61  on" target="_bla
-00006100: 6e6b 223e 3c63 6f64 653e 756a 736f 6e3c  nk"><code>ujson<
-00006110: 2f63 6f64 653e 3c2f 613e 202d 2052 6571  /code></a> - Req
-00006120: 7569 7265 6420 6966 2079 6f75 2077 616e  uired if you wan
-00006130: 7420 746f 2075 7365 2060 554a 534f 4e52  t to use `UJSONR
-00006140: 6573 706f 6e73 6560 2e0a 0a55 7365 6420  esponse`...Used 
-00006150: 6279 2052 6561 6479 4150 4920 2f20 5374  by ReadyAPI / St
-00006160: 6172 6c65 7474 653a 0a0a 2a20 3c61 2068  arlette:..* <a h
-00006170: 7265 663d 2268 7474 7073 3a2f 2f77 7777  ref="https://www
-00006180: 2e75 7669 636f 726e 2e6f 7267 2220 7461  .uvicorn.org" ta
-00006190: 7267 6574 3d22 5f62 6c61 6e6b 223e 3c63  rget="_blank"><c
-000061a0: 6f64 653e 7576 6963 6f72 6e3c 2f63 6f64  ode>uvicorn</cod
-000061b0: 653e 3c2f 613e 202d 2066 6f72 2074 6865  e></a> - for the
-000061c0: 2073 6572 7665 7220 7468 6174 206c 6f61   server that loa
-000061d0: 6473 2061 6e64 2073 6572 7665 7320 796f  ds and serves yo
-000061e0: 7572 2061 7070 6c69 6361 7469 6f6e 2e0a  ur application..
-000061f0: 2a20 3c61 2068 7265 663d 2268 7474 7073  * <a href="https
-00006200: 3a2f 2f67 6974 6875 622e 636f 6d2f 696a  ://github.com/ij
-00006210: 6c2f 6f72 6a73 6f6e 2220 7461 7267 6574  l/orjson" target
-00006220: 3d22 5f62 6c61 6e6b 223e 3c63 6f64 653e  ="_blank"><code>
-00006230: 6f72 6a73 6f6e 3c2f 636f 6465 3e3c 2f61  orjson</code></a
-00006240: 3e20 2d20 5265 7175 6972 6564 2069 6620  > - Required if 
-00006250: 796f 7520 7761 6e74 2074 6f20 7573 6520  you want to use 
-00006260: 604f 524a 534f 4e52 6573 706f 6e73 6560  `ORJSONResponse`
-00006270: 2e0a 0a59 6f75 2063 616e 2069 6e73 7461  ...You can insta
-00006280: 6c6c 2061 6c6c 206f 6620 7468 6573 6520  ll all of these 
-00006290: 7769 7468 2060 7069 7020 696e 7374 616c  with `pip instal
-000062a0: 6c20 2272 6561 6479 6170 695b 616c 6c5d  l "readyapi[all]
-000062b0: 2260 2e0a 0a5b 215b 4869 7443 6f75 6e74  "`...[![HitCount
-000062c0: 5d28 6874 7470 3a2f 2f68 6974 732e 6477  ](http://hits.dw
-000062d0: 796c 2e63 6f6d 2f6b 6875 6c6e 6173 6f66  yl.com/khulnasof
-000062e0: 742f 7265 6164 7961 7069 2e73 7667 295d  t/readyapi.svg)]
-000062f0: 2868 7474 703a 2f2f 6869 7473 2e64 7779  (http://hits.dwy
-00006300: 6c2e 636f 6d2f 6b68 756c 6e61 736f 6674  l.com/khulnasoft
-00006310: 2f72 6561 6479 6170 6929 0a23 2320 4c69  /readyapi).## Li
-00006320: 6365 6e73 650a 0a54 6869 7320 7072 6f6a  cense..This proj
-00006330: 6563 7420 6973 206c 6963 656e 7365 6420  ect is licensed 
-00006340: 756e 6465 7220 7468 6520 7465 726d 7320  under the terms 
-00006350: 6f66 2074 6865 204d 4954 206c 6963 656e  of the MIT licen
-00006360: 7365 2e0a                                se..
+00002cb0: 6874 7470 3a2f 2f31 3237 2e30 2e30 2e31  http://127.0.0.1
+00002cc0: 3a38 3030 302f 7265 646f 633c 2f61 3e2e  :8000/redoc</a>.
+00002cd0: 0a0a 596f 7520 7769 6c6c 2073 6565 2074  ..You will see t
+00002ce0: 6865 2061 6c74 6572 6e61 7469 7665 2061  he alternative a
+00002cf0: 7574 6f6d 6174 6963 2064 6f63 756d 656e  utomatic documen
+00002d00: 7461 7469 6f6e 2028 7072 6f76 6964 6564  tation (provided
+00002d10: 2062 7920 3c61 2068 7265 663d 2268 7474   by <a href="htt
+00002d20: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00002d30: 5265 6269 6c6c 792f 5265 446f 6322 2063  Rebilly/ReDoc" c
+00002d40: 6c61 7373 3d22 6578 7465 726e 616c 2d6c  lass="external-l
+00002d50: 696e 6b22 2074 6172 6765 743d 225f 626c  ink" target="_bl
+00002d60: 616e 6b22 3e52 6544 6f63 3c2f 613e 293a  ank">ReDoc</a>):
+00002d70: 0a0a 215b 5265 446f 635d 2868 7474 7073  ..![ReDoc](https
+00002d80: 3a2f 2f72 6561 6479 6170 692e 6b68 756c  ://readyapi.khul
+00002d90: 6e61 736f 6674 2e63 6f6d 2f69 6d67 2f69  nasoft.com/img/i
+00002da0: 6e64 6578 2f69 6e64 6578 2d30 322d 7265  ndex/index-02-re
+00002db0: 646f 632d 7369 6d70 6c65 2e70 6e67 290a  doc-simple.png).
+00002dc0: 0a23 2320 4578 616d 706c 6520 7570 6772  .## Example upgr
+00002dd0: 6164 650a 0a4e 6f77 206d 6f64 6966 7920  ade..Now modify 
+00002de0: 7468 6520 6669 6c65 2060 6d61 696e 2e70  the file `main.p
+00002df0: 7960 2074 6f20 7265 6365 6976 6520 6120  y` to receive a 
+00002e00: 626f 6479 2066 726f 6d20 6120 6050 5554  body from a `PUT
+00002e10: 6020 7265 7175 6573 742e 0a0a 4465 636c  ` request...Decl
+00002e20: 6172 6520 7468 6520 626f 6479 2075 7369  are the body usi
+00002e30: 6e67 2073 7461 6e64 6172 6420 5079 7468  ng standard Pyth
+00002e40: 6f6e 2074 7970 6573 2c20 7468 616e 6b73  on types, thanks
+00002e50: 2074 6f20 5079 6461 6e74 6963 2e0a 0a60   to Pydantic...`
+00002e60: 6060 5079 7468 6f6e 2068 6c5f 6c69 6e65  ``Python hl_line
+00002e70: 733d 2234 2020 392d 3132 2020 3235 2d32  s="4  9-12  25-2
+00002e80: 3722 0a66 726f 6d20 7479 7069 6e67 2069  7".from typing i
+00002e90: 6d70 6f72 7420 556e 696f 6e0a 0a66 726f  mport Union..fro
+00002ea0: 6d20 7265 6164 7961 7069 2069 6d70 6f72  m readyapi impor
+00002eb0: 7420 5265 6164 7941 5049 0a66 726f 6d20  t ReadyAPI.from 
+00002ec0: 7079 6461 6e74 6963 2069 6d70 6f72 7420  pydantic import 
+00002ed0: 4261 7365 4d6f 6465 6c0a 0a61 7070 203d  BaseModel..app =
+00002ee0: 2052 6561 6479 4150 4928 290a 0a0a 636c   ReadyAPI()...cl
+00002ef0: 6173 7320 4974 656d 2842 6173 654d 6f64  ass Item(BaseMod
+00002f00: 656c 293a 0a20 2020 206e 616d 653a 2073  el):.    name: s
+00002f10: 7472 0a20 2020 2070 7269 6365 3a20 666c  tr.    price: fl
+00002f20: 6f61 740a 2020 2020 6973 5f6f 6666 6572  oat.    is_offer
+00002f30: 3a20 556e 696f 6e5b 626f 6f6c 2c20 4e6f  : Union[bool, No
+00002f40: 6e65 5d20 3d20 4e6f 6e65 0a0a 0a40 6170  ne] = None...@ap
+00002f50: 702e 6765 7428 222f 2229 0a64 6566 2072  p.get("/").def r
+00002f60: 6561 645f 726f 6f74 2829 3a0a 2020 2020  ead_root():.    
+00002f70: 7265 7475 726e 207b 2248 656c 6c6f 223a  return {"Hello":
+00002f80: 2022 576f 726c 6422 7d0a 0a0a 4061 7070   "World"}...@app
+00002f90: 2e67 6574 2822 2f69 7465 6d73 2f7b 6974  .get("/items/{it
+00002fa0: 656d 5f69 647d 2229 0a64 6566 2072 6561  em_id}").def rea
+00002fb0: 645f 6974 656d 2869 7465 6d5f 6964 3a20  d_item(item_id: 
+00002fc0: 696e 742c 2071 3a20 556e 696f 6e5b 7374  int, q: Union[st
+00002fd0: 722c 204e 6f6e 655d 203d 204e 6f6e 6529  r, None] = None)
+00002fe0: 3a0a 2020 2020 7265 7475 726e 207b 2269  :.    return {"i
+00002ff0: 7465 6d5f 6964 223a 2069 7465 6d5f 6964  tem_id": item_id
+00003000: 2c20 2271 223a 2071 7d0a 0a0a 4061 7070  , "q": q}...@app
+00003010: 2e70 7574 2822 2f69 7465 6d73 2f7b 6974  .put("/items/{it
+00003020: 656d 5f69 647d 2229 0a64 6566 2075 7064  em_id}").def upd
+00003030: 6174 655f 6974 656d 2869 7465 6d5f 6964  ate_item(item_id
+00003040: 3a20 696e 742c 2069 7465 6d3a 2049 7465  : int, item: Ite
+00003050: 6d29 3a0a 2020 2020 7265 7475 726e 207b  m):.    return {
+00003060: 2269 7465 6d5f 6e61 6d65 223a 2069 7465  "item_name": ite
+00003070: 6d2e 6e61 6d65 2c20 2269 7465 6d5f 6964  m.name, "item_id
+00003080: 223a 2069 7465 6d5f 6964 7d0a 6060 600a  ": item_id}.```.
+00003090: 0a54 6865 2060 7265 6164 7961 7069 2064  .The `readyapi d
+000030a0: 6576 6020 7365 7276 6572 2073 686f 756c  ev` server shoul
+000030b0: 6420 7265 6c6f 6164 2061 7574 6f6d 6174  d reload automat
+000030c0: 6963 616c 6c79 2e0a 0a23 2323 2049 6e74  ically...### Int
+000030d0: 6572 6163 7469 7665 2041 5049 2064 6f63  eractive API doc
+000030e0: 7320 7570 6772 6164 650a 0a4e 6f77 2067  s upgrade..Now g
+000030f0: 6f20 746f 203c 6120 6872 6566 3d22 6874  o to <a href="ht
+00003100: 7470 3a2f 2f31 3237 2e30 2e30 2e31 3a38  tp://127.0.0.1:8
+00003110: 3030 302f 646f 6373 2220 636c 6173 733d  000/docs" class=
+00003120: 2265 7874 6572 6e61 6c2d 6c69 6e6b 2220  "external-link" 
+00003130: 7461 7267 6574 3d22 5f62 6c61 6e6b 223e  target="_blank">
+00003140: 6874 7470 3a2f 2f31 3237 2e30 2e30 2e31  http://127.0.0.1
+00003150: 3a38 3030 302f 646f 6373 3c2f 613e 2e0a  :8000/docs</a>..
+00003160: 0a2a 2054 6865 2069 6e74 6572 6163 7469  .* The interacti
+00003170: 7665 2041 5049 2064 6f63 756d 656e 7461  ve API documenta
+00003180: 7469 6f6e 2077 696c 6c20 6265 2061 7574  tion will be aut
+00003190: 6f6d 6174 6963 616c 6c79 2075 7064 6174  omatically updat
+000031a0: 6564 2c20 696e 636c 7564 696e 6720 7468  ed, including th
+000031b0: 6520 6e65 7720 626f 6479 3a0a 0a21 5b53  e new body:..![S
+000031c0: 7761 6767 6572 2055 495d 2868 7474 7073  wagger UI](https
+000031d0: 3a2f 2f72 6561 6479 6170 692e 6b68 756c  ://readyapi.khul
+000031e0: 6e61 736f 6674 2e63 6f6d 2f69 6d67 2f69  nasoft.com/img/i
+000031f0: 6e64 6578 2f69 6e64 6578 2d30 332d 7377  ndex/index-03-sw
+00003200: 6167 6765 722d 3032 2e70 6e67 290a 0a2a  agger-02.png)..*
+00003210: 2043 6c69 636b 206f 6e20 7468 6520 6275   Click on the bu
+00003220: 7474 6f6e 2022 5472 7920 6974 206f 7574  tton "Try it out
+00003230: 222c 2069 7420 616c 6c6f 7773 2079 6f75  ", it allows you
+00003240: 2074 6f20 6669 6c6c 2074 6865 2070 6172   to fill the par
+00003250: 616d 6574 6572 7320 616e 6420 6469 7265  ameters and dire
+00003260: 6374 6c79 2069 6e74 6572 6163 7420 7769  ctly interact wi
+00003270: 7468 2074 6865 2041 5049 3a0a 0a21 5b53  th the API:..![S
+00003280: 7761 6767 6572 2055 4920 696e 7465 7261  wagger UI intera
+00003290: 6374 696f 6e5d 2868 7474 7073 3a2f 2f72  ction](https://r
+000032a0: 6561 6479 6170 692e 6b68 756c 6e61 736f  eadyapi.khulnaso
+000032b0: 6674 2e63 6f6d 2f69 6d67 2f69 6e64 6578  ft.com/img/index
+000032c0: 2f69 6e64 6578 2d30 342d 7377 6167 6765  /index-04-swagge
+000032d0: 722d 3033 2e70 6e67 290a 0a2a 2054 6865  r-03.png)..* The
+000032e0: 6e20 636c 6963 6b20 6f6e 2074 6865 2022  n click on the "
+000032f0: 4578 6563 7574 6522 2062 7574 746f 6e2c  Execute" button,
+00003300: 2074 6865 2075 7365 7220 696e 7465 7266   the user interf
+00003310: 6163 6520 7769 6c6c 2063 6f6d 6d75 6e69  ace will communi
+00003320: 6361 7465 2077 6974 6820 796f 7572 2041  cate with your A
+00003330: 5049 2c20 7365 6e64 2074 6865 2070 6172  PI, send the par
+00003340: 616d 6574 6572 732c 2067 6574 2074 6865  ameters, get the
+00003350: 2072 6573 756c 7473 2061 6e64 2073 686f   results and sho
+00003360: 7720 7468 656d 206f 6e20 7468 6520 7363  w them on the sc
+00003370: 7265 656e 3a0a 0a21 5b53 7761 6767 6572  reen:..![Swagger
+00003380: 2055 4920 696e 7465 7261 6374 696f 6e5d   UI interaction]
+00003390: 2868 7474 7073 3a2f 2f72 6561 6479 6170  (https://readyap
+000033a0: 692e 6b68 756c 6e61 736f 6674 2e63 6f6d  i.khulnasoft.com
+000033b0: 2f69 6d67 2f69 6e64 6578 2f69 6e64 6578  /img/index/index
+000033c0: 2d30 352d 7377 6167 6765 722d 3034 2e70  -05-swagger-04.p
+000033d0: 6e67 290a 0a23 2323 2041 6c74 6572 6e61  ng)..### Alterna
+000033e0: 7469 7665 2041 5049 2064 6f63 7320 7570  tive API docs up
+000033f0: 6772 6164 650a 0a41 6e64 206e 6f77 2c20  grade..And now, 
+00003400: 676f 2074 6f20 3c61 2068 7265 663d 2268  go to <a href="h
+00003410: 7474 703a 2f2f 3132 372e 302e 302e 313a  ttp://127.0.0.1:
+00003420: 3830 3030 2f72 6564 6f63 2220 636c 6173  8000/redoc" clas
+00003430: 733d 2265 7874 6572 6e61 6c2d 6c69 6e6b  s="external-link
+00003440: 2220 7461 7267 6574 3d22 5f62 6c61 6e6b  " target="_blank
+00003450: 223e 6874 7470 3a2f 2f31 3237 2e30 2e30  ">http://127.0.0
+00003460: 2e31 3a38 3030 302f 7265 646f 633c 2f61  .1:8000/redoc</a
+00003470: 3e2e 0a0a 2a20 5468 6520 616c 7465 726e  >...* The altern
+00003480: 6174 6976 6520 646f 6375 6d65 6e74 6174  ative documentat
+00003490: 696f 6e20 7769 6c6c 2061 6c73 6f20 7265  ion will also re
+000034a0: 666c 6563 7420 7468 6520 6e65 7720 7175  flect the new qu
+000034b0: 6572 7920 7061 7261 6d65 7465 7220 616e  ery parameter an
+000034c0: 6420 626f 6479 3a0a 0a21 5b52 6544 6f63  d body:..![ReDoc
+000034d0: 5d28 6874 7470 733a 2f2f 7265 6164 7961  ](https://readya
+000034e0: 7069 2e6b 6875 6c6e 6173 6f66 742e 636f  pi.khulnasoft.co
+000034f0: 6d2f 696d 672f 696e 6465 782f 696e 6465  m/img/index/inde
+00003500: 782d 3036 2d72 6564 6f63 2d30 322e 706e  x-06-redoc-02.pn
+00003510: 6729 0a0a 2323 2320 5265 6361 700a 0a49  g)..### Recap..I
+00003520: 6e20 7375 6d6d 6172 792c 2079 6f75 2064  n summary, you d
+00003530: 6563 6c61 7265 202a 2a6f 6e63 652a 2a20  eclare **once** 
+00003540: 7468 6520 7479 7065 7320 6f66 2070 6172  the types of par
+00003550: 616d 6574 6572 732c 2062 6f64 792c 2065  ameters, body, e
+00003560: 7463 2e20 6173 2066 756e 6374 696f 6e20  tc. as function 
+00003570: 7061 7261 6d65 7465 7273 2e0a 0a59 6f75  parameters...You
+00003580: 2064 6f20 7468 6174 2077 6974 6820 7374   do that with st
+00003590: 616e 6461 7264 206d 6f64 6572 6e20 5079  andard modern Py
+000035a0: 7468 6f6e 2074 7970 6573 2e0a 0a59 6f75  thon types...You
+000035b0: 2064 6f6e 2774 2068 6176 6520 746f 206c   don't have to l
+000035c0: 6561 726e 2061 206e 6577 2073 796e 7461  earn a new synta
+000035d0: 782c 2074 6865 206d 6574 686f 6473 206f  x, the methods o
+000035e0: 7220 636c 6173 7365 7320 6f66 2061 2073  r classes of a s
+000035f0: 7065 6369 6669 6320 6c69 6272 6172 792c  pecific library,
+00003600: 2065 7463 2e0a 0a4a 7573 7420 7374 616e   etc...Just stan
+00003610: 6461 7264 202a 2a50 7974 686f 6e2a 2a2e  dard **Python**.
+00003620: 0a0a 466f 7220 6578 616d 706c 652c 2066  ..For example, f
+00003630: 6f72 2061 6e20 6069 6e74 603a 0a0a 6060  or an `int`:..``
+00003640: 6050 7974 686f 6e0a 6974 656d 5f69 643a  `Python.item_id:
+00003650: 2069 6e74 0a60 6060 0a0a 6f72 2066 6f72   int.```..or for
+00003660: 2061 206d 6f72 6520 636f 6d70 6c65 7820   a more complex 
+00003670: 6049 7465 6d60 206d 6f64 656c 3a0a 0a60  `Item` model:..`
+00003680: 6060 5079 7468 6f6e 0a69 7465 6d3a 2049  ``Python.item: I
+00003690: 7465 6d0a 6060 600a 0a2e 2e2e 616e 6420  tem.```.....and 
+000036a0: 7769 7468 2074 6861 7420 7369 6e67 6c65  with that single
+000036b0: 2064 6563 6c61 7261 7469 6f6e 2079 6f75   declaration you
+000036c0: 2067 6574 3a0a 0a2a 2045 6469 746f 7220   get:..* Editor 
+000036d0: 7375 7070 6f72 742c 2069 6e63 6c75 6469  support, includi
+000036e0: 6e67 3a0a 2020 2020 2a20 436f 6d70 6c65  ng:.    * Comple
+000036f0: 7469 6f6e 2e0a 2020 2020 2a20 5479 7065  tion..    * Type
+00003700: 2063 6865 636b 732e 0a2a 2056 616c 6964   checks..* Valid
+00003710: 6174 696f 6e20 6f66 2064 6174 613a 0a20  ation of data:. 
+00003720: 2020 202a 2041 7574 6f6d 6174 6963 2061     * Automatic a
+00003730: 6e64 2063 6c65 6172 2065 7272 6f72 7320  nd clear errors 
+00003740: 7768 656e 2074 6865 2064 6174 6120 6973  when the data is
+00003750: 2069 6e76 616c 6964 2e0a 2020 2020 2a20   invalid..    * 
+00003760: 5661 6c69 6461 7469 6f6e 2065 7665 6e20  Validation even 
+00003770: 666f 7220 6465 6570 6c79 206e 6573 7465  for deeply neste
+00003780: 6420 4a53 4f4e 206f 626a 6563 7473 2e0a  d JSON objects..
+00003790: 2a20 3c61 6262 7220 7469 746c 653d 2261  * <abbr title="a
+000037a0: 6c73 6f20 6b6e 6f77 6e20 6173 3a20 7365  lso known as: se
+000037b0: 7269 616c 697a 6174 696f 6e2c 2070 6172  rialization, par
+000037c0: 7369 6e67 2c20 6d61 7273 6861 6c6c 696e  sing, marshallin
+000037d0: 6722 3e43 6f6e 7665 7273 696f 6e3c 2f61  g">Conversion</a
+000037e0: 6262 723e 206f 6620 696e 7075 7420 6461  bbr> of input da
+000037f0: 7461 3a20 636f 6d69 6e67 2066 726f 6d20  ta: coming from 
+00003800: 7468 6520 6e65 7477 6f72 6b20 746f 2050  the network to P
+00003810: 7974 686f 6e20 6461 7461 2061 6e64 2074  ython data and t
+00003820: 7970 6573 2e20 5265 6164 696e 6720 6672  ypes. Reading fr
+00003830: 6f6d 3a0a 2020 2020 2a20 4a53 4f4e 2e0a  om:.    * JSON..
+00003840: 2020 2020 2a20 5061 7468 2070 6172 616d      * Path param
+00003850: 6574 6572 732e 0a20 2020 202a 2051 7565  eters..    * Que
+00003860: 7279 2070 6172 616d 6574 6572 732e 0a20  ry parameters.. 
+00003870: 2020 202a 2043 6f6f 6b69 6573 2e0a 2020     * Cookies..  
+00003880: 2020 2a20 4865 6164 6572 732e 0a20 2020    * Headers..   
+00003890: 202a 2046 6f72 6d73 2e0a 2020 2020 2a20   * Forms..    * 
+000038a0: 4669 6c65 732e 0a2a 203c 6162 6272 2074  Files..* <abbr t
+000038b0: 6974 6c65 3d22 616c 736f 206b 6e6f 776e  itle="also known
+000038c0: 2061 733a 2073 6572 6961 6c69 7a61 7469   as: serializati
+000038d0: 6f6e 2c20 7061 7273 696e 672c 206d 6172  on, parsing, mar
+000038e0: 7368 616c 6c69 6e67 223e 436f 6e76 6572  shalling">Conver
+000038f0: 7369 6f6e 3c2f 6162 6272 3e20 6f66 206f  sion</abbr> of o
+00003900: 7574 7075 7420 6461 7461 3a20 636f 6e76  utput data: conv
+00003910: 6572 7469 6e67 2066 726f 6d20 5079 7468  erting from Pyth
+00003920: 6f6e 2064 6174 6120 616e 6420 7479 7065  on data and type
+00003930: 7320 746f 206e 6574 776f 726b 2064 6174  s to network dat
+00003940: 6120 2861 7320 4a53 4f4e 293a 0a20 2020  a (as JSON):.   
+00003950: 202a 2043 6f6e 7665 7274 2050 7974 686f   * Convert Pytho
+00003960: 6e20 7479 7065 7320 2860 7374 7260 2c20  n types (`str`, 
+00003970: 6069 6e74 602c 2060 666c 6f61 7460 2c20  `int`, `float`, 
+00003980: 6062 6f6f 6c60 2c20 606c 6973 7460 2c20  `bool`, `list`, 
+00003990: 6574 6329 2e0a 2020 2020 2a20 6064 6174  etc)..    * `dat
+000039a0: 6574 696d 6560 206f 626a 6563 7473 2e0a  etime` objects..
+000039b0: 2020 2020 2a20 6055 5549 4460 206f 626a      * `UUID` obj
+000039c0: 6563 7473 2e0a 2020 2020 2a20 4461 7461  ects..    * Data
+000039d0: 6261 7365 206d 6f64 656c 732e 0a20 2020  base models..   
+000039e0: 202a 202e 2e2e 616e 6420 6d61 6e79 206d   * ...and many m
+000039f0: 6f72 652e 0a2a 2041 7574 6f6d 6174 6963  ore..* Automatic
+00003a00: 2069 6e74 6572 6163 7469 7665 2041 5049   interactive API
+00003a10: 2064 6f63 756d 656e 7461 7469 6f6e 2c20   documentation, 
+00003a20: 696e 636c 7564 696e 6720 3220 616c 7465  including 2 alte
+00003a30: 726e 6174 6976 6520 7573 6572 2069 6e74  rnative user int
+00003a40: 6572 6661 6365 733a 0a20 2020 202a 2053  erfaces:.    * S
+00003a50: 7761 6767 6572 2055 492e 0a20 2020 202a  wagger UI..    *
+00003a60: 2052 6544 6f63 2e0a 0a2d 2d2d 0a0a 436f   ReDoc...---..Co
+00003a70: 6d69 6e67 2062 6163 6b20 746f 2074 6865  ming back to the
+00003a80: 2070 7265 7669 6f75 7320 636f 6465 2065   previous code e
+00003a90: 7861 6d70 6c65 2c20 2a2a 5265 6164 7941  xample, **ReadyA
+00003aa0: 5049 2a2a 2077 696c 6c3a 0a0a 2a20 5661  PI** will:..* Va
+00003ab0: 6c69 6461 7465 2074 6861 7420 7468 6572  lidate that ther
+00003ac0: 6520 6973 2061 6e20 6069 7465 6d5f 6964  e is an `item_id
+00003ad0: 6020 696e 2074 6865 2070 6174 6820 666f  ` in the path fo
+00003ae0: 7220 6047 4554 6020 616e 6420 6050 5554  r `GET` and `PUT
+00003af0: 6020 7265 7175 6573 7473 2e0a 2a20 5661  ` requests..* Va
+00003b00: 6c69 6461 7465 2074 6861 7420 7468 6520  lidate that the 
+00003b10: 6069 7465 6d5f 6964 6020 6973 206f 6620  `item_id` is of 
+00003b20: 7479 7065 2060 696e 7460 2066 6f72 2060  type `int` for `
+00003b30: 4745 5460 2061 6e64 2060 5055 5460 2072  GET` and `PUT` r
+00003b40: 6571 7565 7374 732e 0a20 2020 202a 2049  equests..    * I
+00003b50: 6620 6974 2069 7320 6e6f 742c 2074 6865  f it is not, the
+00003b60: 2063 6c69 656e 7420 7769 6c6c 2073 6565   client will see
+00003b70: 2061 2075 7365 6675 6c2c 2063 6c65 6172   a useful, clear
+00003b80: 2065 7272 6f72 2e0a 2a20 4368 6563 6b20   error..* Check 
+00003b90: 6966 2074 6865 7265 2069 7320 616e 206f  if there is an o
+00003ba0: 7074 696f 6e61 6c20 7175 6572 7920 7061  ptional query pa
+00003bb0: 7261 6d65 7465 7220 6e61 6d65 6420 6071  rameter named `q
+00003bc0: 6020 2861 7320 696e 2060 6874 7470 3a2f  ` (as in `http:/
+00003bd0: 2f31 3237 2e30 2e30 2e31 3a38 3030 302f  /127.0.0.1:8000/
+00003be0: 6974 656d 732f 666f 6f3f 713d 736f 6d65  items/foo?q=some
+00003bf0: 7175 6572 7960 2920 666f 7220 6047 4554  query`) for `GET
+00003c00: 6020 7265 7175 6573 7473 2e0a 2020 2020  ` requests..    
+00003c10: 2a20 4173 2074 6865 2060 7160 2070 6172  * As the `q` par
+00003c20: 616d 6574 6572 2069 7320 6465 636c 6172  ameter is declar
+00003c30: 6564 2077 6974 6820 603d 204e 6f6e 6560  ed with `= None`
+00003c40: 2c20 6974 2069 7320 6f70 7469 6f6e 616c  , it is optional
+00003c50: 2e0a 2020 2020 2a20 5769 7468 6f75 7420  ..    * Without 
+00003c60: 7468 6520 604e 6f6e 6560 2069 7420 776f  the `None` it wo
+00003c70: 756c 6420 6265 2072 6571 7569 7265 6420  uld be required 
+00003c80: 2861 7320 6973 2074 6865 2062 6f64 7920  (as is the body 
+00003c90: 696e 2074 6865 2063 6173 6520 7769 7468  in the case with
+00003ca0: 2060 5055 5460 292e 0a2a 2046 6f72 2060   `PUT`)..* For `
+00003cb0: 5055 5460 2072 6571 7565 7374 7320 746f  PUT` requests to
+00003cc0: 2060 2f69 7465 6d73 2f7b 6974 656d 5f69   `/items/{item_i
+00003cd0: 647d 602c 2052 6561 6420 7468 6520 626f  d}`, Read the bo
+00003ce0: 6479 2061 7320 4a53 4f4e 3a0a 2020 2020  dy as JSON:.    
+00003cf0: 2a20 4368 6563 6b20 7468 6174 2069 7420  * Check that it 
+00003d00: 6861 7320 6120 7265 7175 6972 6564 2061  has a required a
+00003d10: 7474 7269 6275 7465 2060 6e61 6d65 6020  ttribute `name` 
+00003d20: 7468 6174 2073 686f 756c 6420 6265 2061  that should be a
+00003d30: 2060 7374 7260 2e0a 2020 2020 2a20 4368   `str`..    * Ch
+00003d40: 6563 6b20 7468 6174 2069 7420 6861 7320  eck that it has 
+00003d50: 6120 7265 7175 6972 6564 2061 7474 7269  a required attri
+00003d60: 6275 7465 2060 7072 6963 6560 2074 6861  bute `price` tha
+00003d70: 7420 6861 7320 746f 2062 6520 6120 6066  t has to be a `f
+00003d80: 6c6f 6174 602e 0a20 2020 202a 2043 6865  loat`..    * Che
+00003d90: 636b 2074 6861 7420 6974 2068 6173 2061  ck that it has a
+00003da0: 6e20 6f70 7469 6f6e 616c 2061 7474 7269  n optional attri
+00003db0: 6275 7465 2060 6973 5f6f 6666 6572 602c  bute `is_offer`,
+00003dc0: 2074 6861 7420 7368 6f75 6c64 2062 6520   that should be 
+00003dd0: 6120 6062 6f6f 6c60 2c20 6966 2070 7265  a `bool`, if pre
+00003de0: 7365 6e74 2e0a 2020 2020 2a20 416c 6c20  sent..    * All 
+00003df0: 7468 6973 2077 6f75 6c64 2061 6c73 6f20  this would also 
+00003e00: 776f 726b 2066 6f72 2064 6565 706c 7920  work for deeply 
+00003e10: 6e65 7374 6564 204a 534f 4e20 6f62 6a65  nested JSON obje
+00003e20: 6374 732e 0a2a 2043 6f6e 7665 7274 2066  cts..* Convert f
+00003e30: 726f 6d20 616e 6420 746f 204a 534f 4e20  rom and to JSON 
+00003e40: 6175 746f 6d61 7469 6361 6c6c 792e 0a2a  automatically..*
+00003e50: 2044 6f63 756d 656e 7420 6576 6572 7974   Document everyt
+00003e60: 6869 6e67 2077 6974 6820 4f70 656e 4150  hing with OpenAP
+00003e70: 492c 2074 6861 7420 6361 6e20 6265 2075  I, that can be u
+00003e80: 7365 6420 6279 3a0a 2020 2020 2a20 496e  sed by:.    * In
+00003e90: 7465 7261 6374 6976 6520 646f 6375 6d65  teractive docume
+00003ea0: 6e74 6174 696f 6e20 7379 7374 656d 732e  ntation systems.
+00003eb0: 0a20 2020 202a 2041 7574 6f6d 6174 6963  .    * Automatic
+00003ec0: 2063 6c69 656e 7420 636f 6465 2067 656e   client code gen
+00003ed0: 6572 6174 696f 6e20 7379 7374 656d 732c  eration systems,
+00003ee0: 2066 6f72 206d 616e 7920 6c61 6e67 7561   for many langua
+00003ef0: 6765 732e 0a2a 2050 726f 7669 6465 2032  ges..* Provide 2
+00003f00: 2069 6e74 6572 6163 7469 7665 2064 6f63   interactive doc
+00003f10: 756d 656e 7461 7469 6f6e 2077 6562 2069  umentation web i
+00003f20: 6e74 6572 6661 6365 7320 6469 7265 6374  nterfaces direct
+00003f30: 6c79 2e0a 0a2d 2d2d 0a0a 5765 206a 7573  ly...---..We jus
+00003f40: 7420 7363 7261 7463 6865 6420 7468 6520  t scratched the 
+00003f50: 7375 7266 6163 652c 2062 7574 2079 6f75  surface, but you
+00003f60: 2061 6c72 6561 6479 2067 6574 2074 6865   already get the
+00003f70: 2069 6465 6120 6f66 2068 6f77 2069 7420   idea of how it 
+00003f80: 616c 6c20 776f 726b 732e 0a0a 5472 7920  all works...Try 
+00003f90: 6368 616e 6769 6e67 2074 6865 206c 696e  changing the lin
+00003fa0: 6520 7769 7468 3a0a 0a60 6060 5079 7468  e with:..```Pyth
+00003fb0: 6f6e 0a20 2020 2072 6574 7572 6e20 7b22  on.    return {"
+00003fc0: 6974 656d 5f6e 616d 6522 3a20 6974 656d  item_name": item
+00003fd0: 2e6e 616d 652c 2022 6974 656d 5f69 6422  .name, "item_id"
+00003fe0: 3a20 6974 656d 5f69 647d 0a60 6060 0a0a  : item_id}.```..
+00003ff0: 2e2e 2e66 726f 6d3a 0a0a 6060 6050 7974  ...from:..```Pyt
+00004000: 686f 6e0a 2020 2020 2020 2020 2e2e 2e20  hon.        ... 
+00004010: 2269 7465 6d5f 6e61 6d65 223a 2069 7465  "item_name": ite
+00004020: 6d2e 6e61 6d65 202e 2e2e 0a60 6060 0a0a  m.name ....```..
+00004030: 2e2e 2e74 6f3a 0a0a 6060 6050 7974 686f  ...to:..```Pytho
+00004040: 6e0a 2020 2020 2020 2020 2e2e 2e20 2269  n.        ... "i
+00004050: 7465 6d5f 7072 6963 6522 3a20 6974 656d  tem_price": item
+00004060: 2e70 7269 6365 202e 2e2e 0a60 6060 0a0a  .price ....```..
+00004070: 2e2e 2e61 6e64 2073 6565 2068 6f77 2079  ...and see how y
+00004080: 6f75 7220 6564 6974 6f72 2077 696c 6c20  our editor will 
+00004090: 6175 746f 2d63 6f6d 706c 6574 6520 7468  auto-complete th
+000040a0: 6520 6174 7472 6962 7574 6573 2061 6e64  e attributes and
+000040b0: 206b 6e6f 7720 7468 6569 7220 7479 7065   know their type
+000040c0: 733a 0a0a 215b 6564 6974 6f72 2073 7570  s:..![editor sup
+000040d0: 706f 7274 5d28 6874 7470 733a 2f2f 7265  port](https://re
+000040e0: 6164 7961 7069 2e6b 6875 6c6e 6173 6f66  adyapi.khulnasof
+000040f0: 742e 636f 6d2f 696d 672f 7673 636f 6465  t.com/img/vscode
+00004100: 2d63 6f6d 706c 6574 696f 6e2e 706e 6729  -completion.png)
+00004110: 0a0a 466f 7220 6120 6d6f 7265 2063 6f6d  ..For a more com
+00004120: 706c 6574 6520 6578 616d 706c 6520 696e  plete example in
+00004130: 636c 7564 696e 6720 6d6f 7265 2066 6561  cluding more fea
+00004140: 7475 7265 732c 2073 6565 2074 6865 203c  tures, see the <
+00004150: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
+00004160: 7265 6164 7961 7069 2e6b 6875 6c6e 6173  readyapi.khulnas
+00004170: 6f66 742e 636f 6d2f 7475 746f 7269 616c  oft.com/tutorial
+00004180: 2f22 3e54 7574 6f72 6961 6c20 2d20 5573  /">Tutorial - Us
+00004190: 6572 2047 7569 6465 3c2f 613e 2e0a 0a2a  er Guide</a>...*
+000041a0: 2a53 706f 696c 6572 2061 6c65 7274 2a2a  *Spoiler alert**
+000041b0: 3a20 7468 6520 7475 746f 7269 616c 202d  : the tutorial -
+000041c0: 2075 7365 7220 6775 6964 6520 696e 636c   user guide incl
+000041d0: 7564 6573 3a0a 0a2a 2044 6563 6c61 7261  udes:..* Declara
+000041e0: 7469 6f6e 206f 6620 2a2a 7061 7261 6d65  tion of **parame
+000041f0: 7465 7273 2a2a 2066 726f 6d20 6f74 6865  ters** from othe
+00004200: 7220 6469 6666 6572 656e 7420 706c 6163  r different plac
+00004210: 6573 2061 733a 202a 2a68 6561 6465 7273  es as: **headers
+00004220: 2a2a 2c20 2a2a 636f 6f6b 6965 732a 2a2c  **, **cookies**,
+00004230: 202a 2a66 6f72 6d20 6669 656c 6473 2a2a   **form fields**
+00004240: 2061 6e64 202a 2a66 696c 6573 2a2a 2e0a   and **files**..
+00004250: 2a20 486f 7720 746f 2073 6574 202a 2a76  * How to set **v
+00004260: 616c 6964 6174 696f 6e20 636f 6e73 7472  alidation constr
+00004270: 6169 6e74 732a 2a20 6173 2060 6d61 7869  aints** as `maxi
+00004280: 6d75 6d5f 6c65 6e67 7468 6020 6f72 2060  mum_length` or `
+00004290: 7265 6765 7860 2e0a 2a20 4120 7665 7279  regex`..* A very
+000042a0: 2070 6f77 6572 6675 6c20 616e 6420 6561   powerful and ea
+000042b0: 7379 2074 6f20 7573 6520 2a2a 3c61 6262  sy to use **<abb
+000042c0: 7220 7469 746c 653d 2261 6c73 6f20 6b6e  r title="also kn
+000042d0: 6f77 6e20 6173 2063 6f6d 706f 6e65 6e74  own as component
+000042e0: 732c 2072 6573 6f75 7263 6573 2c20 7072  s, resources, pr
+000042f0: 6f76 6964 6572 732c 2073 6572 7669 6365  oviders, service
+00004300: 732c 2069 6e6a 6563 7461 626c 6573 223e  s, injectables">
+00004310: 4465 7065 6e64 656e 6379 2049 6e6a 6563  Dependency Injec
+00004320: 7469 6f6e 3c2f 6162 6272 3e2a 2a20 7379  tion</abbr>** sy
+00004330: 7374 656d 2e0a 2a20 5365 6375 7269 7479  stem..* Security
+00004340: 2061 6e64 2061 7574 6865 6e74 6963 6174   and authenticat
+00004350: 696f 6e2c 2069 6e63 6c75 6469 6e67 2073  ion, including s
+00004360: 7570 706f 7274 2066 6f72 202a 2a4f 4175  upport for **OAu
+00004370: 7468 322a 2a20 7769 7468 202a 2a4a 5754  th2** with **JWT
+00004380: 2074 6f6b 656e 732a 2a20 616e 6420 2a2a   tokens** and **
+00004390: 4854 5450 2042 6173 6963 2a2a 2061 7574  HTTP Basic** aut
+000043a0: 682e 0a2a 204d 6f72 6520 6164 7661 6e63  h..* More advanc
+000043b0: 6564 2028 6275 7420 6571 7561 6c6c 7920  ed (but equally 
+000043c0: 6561 7379 2920 7465 6368 6e69 7175 6573  easy) techniques
+000043d0: 2066 6f72 2064 6563 6c61 7269 6e67 202a   for declaring *
+000043e0: 2a64 6565 706c 7920 6e65 7374 6564 204a  *deeply nested J
+000043f0: 534f 4e20 6d6f 6465 6c73 2a2a 2028 7468  SON models** (th
+00004400: 616e 6b73 2074 6f20 5079 6461 6e74 6963  anks to Pydantic
+00004410: 292e 0a2a 202a 2a47 7261 7068 514c 2a2a  )..* **GraphQL**
+00004420: 2069 6e74 6567 7261 7469 6f6e 2077 6974   integration wit
+00004430: 6820 3c61 2068 7265 663d 2268 7474 7073  h <a href="https
+00004440: 3a2f 2f73 7472 6177 6265 7272 792e 726f  ://strawberry.ro
+00004450: 636b 7322 2063 6c61 7373 3d22 6578 7465  cks" class="exte
+00004460: 726e 616c 2d6c 696e 6b22 2074 6172 6765  rnal-link" targe
+00004470: 743d 225f 626c 616e 6b22 3e53 7472 6177  t="_blank">Straw
+00004480: 6265 7272 793c 2f61 3e20 616e 6420 6f74  berry</a> and ot
+00004490: 6865 7220 6c69 6272 6172 6965 732e 0a2a  her libraries..*
+000044a0: 204d 616e 7920 6578 7472 6120 6665 6174   Many extra feat
+000044b0: 7572 6573 2028 7468 616e 6b73 2074 6f20  ures (thanks to 
+000044c0: 5374 6172 6c65 7474 6529 2061 733a 0a20  Starlette) as:. 
+000044d0: 2020 202a 202a 2a57 6562 536f 636b 6574     * **WebSocket
+000044e0: 732a 2a0a 2020 2020 2a20 6578 7472 656d  s**.    * extrem
+000044f0: 656c 7920 6561 7379 2074 6573 7473 2062  ely easy tests b
+00004500: 6173 6564 206f 6e20 4854 5450 5820 616e  ased on HTTPX an
+00004510: 6420 6070 7974 6573 7460 0a20 2020 202a  d `pytest`.    *
+00004520: 202a 2a43 4f52 532a 2a0a 2020 2020 2a20   **CORS**.    * 
+00004530: 2a2a 436f 6f6b 6965 2053 6573 7369 6f6e  **Cookie Session
+00004540: 732a 2a0a 2020 2020 2a20 2e2e 2e61 6e64  s**.    * ...and
+00004550: 206d 6f72 652e 0a0a 2323 2050 6572 666f   more...## Perfo
+00004560: 726d 616e 6365 0a0a 496e 6465 7065 6e64  rmance..Independ
+00004570: 656e 7420 5465 6368 456d 706f 7765 7220  ent TechEmpower 
+00004580: 6265 6e63 686d 6172 6b73 2073 686f 7720  benchmarks show 
+00004590: 2a2a 5265 6164 7941 5049 2a2a 2061 7070  **ReadyAPI** app
+000045a0: 6c69 6361 7469 6f6e 7320 7275 6e6e 696e  lications runnin
+000045b0: 6720 756e 6465 7220 5576 6963 6f72 6e20  g under Uvicorn 
+000045c0: 6173 203c 6120 6872 6566 3d22 6874 7470  as <a href="http
+000045d0: 733a 2f2f 7777 772e 7465 6368 656d 706f  s://www.techempo
+000045e0: 7765 722e 636f 6d2f 6265 6e63 686d 6172  wer.com/benchmar
+000045f0: 6b73 2f23 7365 6374 696f 6e3d 7465 7374  ks/#section=test
+00004600: 2672 756e 6964 3d37 3436 3465 3532 302d  &runid=7464e520-
+00004610: 3064 6332 2d34 3733 642d 6264 3334 2d64  0dc2-473d-bd34-d
+00004620: 6264 6664 3765 3835 3931 3126 6877 3d70  bdfd7e85911&hw=p
+00004630: 6826 7465 7374 3d71 7565 7279 266c 3d7a  h&test=query&l=z
+00004640: 696a 7a65 6e2d 3722 2063 6c61 7373 3d22  ijzen-7" class="
+00004650: 6578 7465 726e 616c 2d6c 696e 6b22 2074  external-link" t
+00004660: 6172 6765 743d 225f 626c 616e 6b22 3e6f  arget="_blank">o
+00004670: 6e65 206f 6620 7468 6520 6661 7374 6573  ne of the fastes
+00004680: 7420 5079 7468 6f6e 2066 7261 6d65 776f  t Python framewo
+00004690: 726b 7320 6176 6169 6c61 626c 653c 2f61  rks available</a
+000046a0: 3e2c 206f 6e6c 7920 6265 6c6f 7720 5374  >, only below St
+000046b0: 6172 6c65 7474 6520 616e 6420 5576 6963  arlette and Uvic
+000046c0: 6f72 6e20 7468 656d 7365 6c76 6573 2028  orn themselves (
+000046d0: 7573 6564 2069 6e74 6572 6e61 6c6c 7920  used internally 
+000046e0: 6279 2052 6561 6479 4150 4929 2e20 282a  by ReadyAPI). (*
+000046f0: 290a 0a54 6f20 756e 6465 7273 7461 6e64  )..To understand
+00004700: 206d 6f72 6520 6162 6f75 7420 6974 2c20   more about it, 
+00004710: 7365 6520 7468 6520 7365 6374 696f 6e20  see the section 
+00004720: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
+00004730: 2f72 6561 6479 6170 692e 6b68 756c 6e61  /readyapi.khulna
+00004740: 736f 6674 2e63 6f6d 2f62 656e 6368 6d61  soft.com/benchma
+00004750: 726b 732f 2220 636c 6173 733d 2269 6e74  rks/" class="int
+00004760: 6572 6e61 6c2d 6c69 6e6b 2220 7461 7267  ernal-link" targ
+00004770: 6574 3d22 5f62 6c61 6e6b 223e 4265 6e63  et="_blank">Benc
+00004780: 686d 6172 6b73 3c2f 613e 2e0a 0a23 2320  hmarks</a>...## 
+00004790: 4465 7065 6e64 656e 6369 6573 0a0a 5573  Dependencies..Us
+000047a0: 6564 2062 7920 5079 6461 6e74 6963 3a0a  ed by Pydantic:.
+000047b0: 0a2a 203c 6120 6872 6566 3d22 6874 7470  .* <a href="http
+000047c0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f4a  s://github.com/J
+000047d0: 6f73 6844 6174 612f 7079 7468 6f6e 2d65  oshData/python-e
+000047e0: 6d61 696c 2d76 616c 6964 6174 6f72 2220  mail-validator" 
+000047f0: 7461 7267 6574 3d22 5f62 6c61 6e6b 223e  target="_blank">
+00004800: 3c63 6f64 653e 656d 6169 6c5f 7661 6c69  <code>email_vali
+00004810: 6461 746f 723c 2f63 6f64 653e 3c2f 613e  dator</code></a>
+00004820: 202d 2066 6f72 2065 6d61 696c 2076 616c   - for email val
+00004830: 6964 6174 696f 6e2e 0a2a 203c 6120 6872  idation..* <a hr
+00004840: 6566 3d22 6874 7470 733a 2f2f 646f 6373  ef="https://docs
+00004850: 2e70 7964 616e 7469 632e 6465 762f 6c61  .pydantic.dev/la
+00004860: 7465 7374 2f75 7361 6765 2f70 7964 616e  test/usage/pydan
+00004870: 7469 635f 7365 7474 696e 6773 2f22 2074  tic_settings/" t
+00004880: 6172 6765 743d 225f 626c 616e 6b22 3e3c  arget="_blank"><
+00004890: 636f 6465 3e70 7964 616e 7469 632d 7365  code>pydantic-se
+000048a0: 7474 696e 6773 3c2f 636f 6465 3e3c 2f61  ttings</code></a
+000048b0: 3e20 2d20 666f 7220 7365 7474 696e 6773  > - for settings
+000048c0: 206d 616e 6167 656d 656e 742e 0a2a 203c   management..* <
+000048d0: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
+000048e0: 646f 6373 2e70 7964 616e 7469 632e 6465  docs.pydantic.de
+000048f0: 762f 6c61 7465 7374 2f75 7361 6765 2f74  v/latest/usage/t
+00004900: 7970 6573 2f65 7874 7261 5f74 7970 6573  ypes/extra_types
+00004910: 2f65 7874 7261 5f74 7970 6573 2f22 2074  /extra_types/" t
+00004920: 6172 6765 743d 225f 626c 616e 6b22 3e3c  arget="_blank"><
+00004930: 636f 6465 3e70 7964 616e 7469 632d 6578  code>pydantic-ex
+00004940: 7472 612d 7479 7065 733c 2f63 6f64 653e  tra-types</code>
+00004950: 3c2f 613e 202d 2066 6f72 2065 7874 7261  </a> - for extra
+00004960: 2074 7970 6573 2074 6f20 6265 2075 7365   types to be use
+00004970: 6420 7769 7468 2050 7964 616e 7469 632e  d with Pydantic.
+00004980: 0a0a 5573 6564 2062 7920 5374 6172 6c65  ..Used by Starle
+00004990: 7474 653a 0a0a 2a20 3c61 2068 7265 663d  tte:..* <a href=
+000049a0: 2268 7474 7073 3a2f 2f77 7777 2e70 7974  "https://www.pyt
+000049b0: 686f 6e2d 6874 7470 782e 6f72 6722 2074  hon-httpx.org" t
+000049c0: 6172 6765 743d 225f 626c 616e 6b22 3e3c  arget="_blank"><
+000049d0: 636f 6465 3e68 7474 7078 3c2f 636f 6465  code>httpx</code
+000049e0: 3e3c 2f61 3e20 2d20 5265 7175 6972 6564  ></a> - Required
+000049f0: 2069 6620 796f 7520 7761 6e74 2074 6f20   if you want to 
+00004a00: 7573 6520 7468 6520 6054 6573 7443 6c69  use the `TestCli
+00004a10: 656e 7460 2e0a 2a20 3c61 2068 7265 663d  ent`..* <a href=
+00004a20: 2268 7474 7073 3a2f 2f6a 696e 6a61 2e70  "https://jinja.p
+00004a30: 616c 6c65 7473 7072 6f6a 6563 7473 2e63  alletsprojects.c
+00004a40: 6f6d 2220 7461 7267 6574 3d22 5f62 6c61  om" target="_bla
+00004a50: 6e6b 223e 3c63 6f64 653e 6a69 6e6a 6132  nk"><code>jinja2
+00004a60: 3c2f 636f 6465 3e3c 2f61 3e20 2d20 5265  </code></a> - Re
+00004a70: 7175 6972 6564 2069 6620 796f 7520 7761  quired if you wa
+00004a80: 6e74 2074 6f20 7573 6520 7468 6520 6465  nt to use the de
+00004a90: 6661 756c 7420 7465 6d70 6c61 7465 2063  fault template c
+00004aa0: 6f6e 6669 6775 7261 7469 6f6e 2e0a 2a20  onfiguration..* 
+00004ab0: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
+00004ac0: 2f67 6974 6875 622e 636f 6d2f 4b6c 7564  /github.com/Klud
+00004ad0: 6578 2f70 7974 686f 6e2d 6d75 6c74 6970  ex/python-multip
+00004ae0: 6172 7422 2074 6172 6765 743d 225f 626c  art" target="_bl
+00004af0: 616e 6b22 3e3c 636f 6465 3e70 7974 686f  ank"><code>pytho
+00004b00: 6e2d 6d75 6c74 6970 6172 743c 2f63 6f64  n-multipart</cod
+00004b10: 653e 3c2f 613e 202d 2052 6571 7569 7265  e></a> - Require
+00004b20: 6420 6966 2079 6f75 2077 616e 7420 746f  d if you want to
+00004b30: 2073 7570 706f 7274 2066 6f72 6d20 3c61   support form <a
+00004b40: 6262 7220 7469 746c 653d 2263 6f6e 7665  bbr title="conve
+00004b50: 7274 696e 6720 7468 6520 7374 7269 6e67  rting the string
+00004b60: 2074 6861 7420 636f 6d65 7320 6672 6f6d   that comes from
+00004b70: 2061 6e20 4854 5450 2072 6571 7565 7374   an HTTP request
+00004b80: 2069 6e74 6f20 5079 7468 6f6e 2064 6174   into Python dat
+00004b90: 6122 3e22 7061 7273 696e 6722 3c2f 6162  a">"parsing"</ab
+00004ba0: 6272 3e2c 2077 6974 6820 6072 6571 7565  br>, with `reque
+00004bb0: 7374 2e66 6f72 6d28 2960 2e0a 0a55 7365  st.form()`...Use
+00004bc0: 6420 6279 2052 6561 6479 4150 4920 2f20  d by ReadyAPI / 
+00004bd0: 5374 6172 6c65 7474 653a 0a0a 2a20 3c61  Starlette:..* <a
+00004be0: 2068 7265 663d 2268 7474 7073 3a2f 2f77   href="https://w
+00004bf0: 7777 2e75 7669 636f 726e 2e6f 7267 2220  ww.uvicorn.org" 
+00004c00: 7461 7267 6574 3d22 5f62 6c61 6e6b 223e  target="_blank">
+00004c10: 3c63 6f64 653e 7576 6963 6f72 6e3c 2f63  <code>uvicorn</c
+00004c20: 6f64 653e 3c2f 613e 202d 2066 6f72 2074  ode></a> - for t
+00004c30: 6865 2073 6572 7665 7220 7468 6174 206c  he server that l
+00004c40: 6f61 6473 2061 6e64 2073 6572 7665 7320  oads and serves 
+00004c50: 796f 7572 2061 7070 6c69 6361 7469 6f6e  your application
+00004c60: 2e0a 2a20 3c61 2068 7265 663d 2268 7474  ..* <a href="htt
+00004c70: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00004c80: 696a 6c2f 6f72 6a73 6f6e 2220 7461 7267  ijl/orjson" targ
+00004c90: 6574 3d22 5f62 6c61 6e6b 223e 3c63 6f64  et="_blank"><cod
+00004ca0: 653e 6f72 6a73 6f6e 3c2f 636f 6465 3e3c  e>orjson</code><
+00004cb0: 2f61 3e20 2d20 5265 7175 6972 6564 2069  /a> - Required i
+00004cc0: 6620 796f 7520 7761 6e74 2074 6f20 7573  f you want to us
+00004cd0: 6520 604f 524a 534f 4e52 6573 706f 6e73  e `ORJSONRespons
+00004ce0: 6560 2e0a 2a20 3c61 2068 7265 663d 2268  e`..* <a href="h
+00004cf0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00004d00: 6d2f 6573 6e6d 652f 756c 7472 616a 736f  m/esnme/ultrajso
+00004d10: 6e22 2074 6172 6765 743d 225f 626c 616e  n" target="_blan
+00004d20: 6b22 3e3c 636f 6465 3e75 6a73 6f6e 3c2f  k"><code>ujson</
+00004d30: 636f 6465 3e3c 2f61 3e20 2d20 5265 7175  code></a> - Requ
+00004d40: 6972 6564 2069 6620 796f 7520 7761 6e74  ired if you want
+00004d50: 2074 6f20 7573 6520 6055 4a53 4f4e 5265   to use `UJSONRe
+00004d60: 7370 6f6e 7365 602e 0a2a 2060 7265 6164  sponse`..* `read
+00004d70: 7961 7069 2d63 6c69 6020 2d20 746f 2070  yapi-cli` - to p
+00004d80: 726f 7669 6465 2074 6865 2060 7265 6164  rovide the `read
+00004d90: 7961 7069 6020 636f 6d6d 616e 642e 0a0a  yapi` command...
+00004da0: 5768 656e 2079 6f75 2069 6e73 7461 6c6c  When you install
+00004db0: 2060 7265 6164 7961 7069 6020 6974 2063   `readyapi` it c
+00004dc0: 6f6d 6573 2074 6865 7365 2073 7461 6e64  omes these stand
+00004dd0: 6172 6420 6465 7065 6e64 656e 6369 6573  ard dependencies
+00004de0: 2e0a 0a23 2320 6072 6561 6479 6170 692d  ...## `readyapi-
+00004df0: 736c 696d 600a 0a49 6620 796f 7520 646f  slim`..If you do
+00004e00: 6e27 7420 7761 6e74 2074 6865 2065 7874  n't want the ext
+00004e10: 7261 2073 7461 6e64 6172 6420 6f70 7469  ra standard opti
+00004e20: 6f6e 616c 2064 6570 656e 6465 6e63 6965  onal dependencie
+00004e30: 732c 2069 6e73 7461 6c6c 2060 7265 6164  s, install `read
+00004e40: 7961 7069 2d73 6c69 6d60 2069 6e73 7465  yapi-slim` inste
+00004e50: 6164 2e0a 0a57 6865 6e20 796f 7520 696e  ad...When you in
+00004e60: 7374 616c 6c20 7769 7468 3a0a 0a60 6060  stall with:..```
+00004e70: 6261 7368 0a70 6970 2069 6e73 7461 6c6c  bash.pip install
+00004e80: 2072 6561 6479 6170 690a 6060 600a 0a2e   readyapi.```...
+00004e90: 2e2e 6974 2069 6e63 6c75 6465 7320 7468  ..it includes th
+00004ea0: 6520 7361 6d65 2063 6f64 6520 616e 6420  e same code and 
+00004eb0: 6465 7065 6e64 656e 6369 6573 2061 733a  dependencies as:
+00004ec0: 0a0a 6060 6062 6173 680a 7069 7020 696e  ..```bash.pip in
+00004ed0: 7374 616c 6c20 2272 6561 6479 6170 692d  stall "readyapi-
+00004ee0: 736c 696d 5b73 7461 6e64 6172 645d 220a  slim[standard]".
+00004ef0: 6060 600a 0a54 6865 2073 7461 6e64 6172  ```..The standar
+00004f00: 6420 6578 7472 6120 6465 7065 6e64 656e  d extra dependen
+00004f10: 6369 6573 2061 7265 2074 6865 206f 6e65  cies are the one
+00004f20: 7320 6d65 6e74 696f 6e65 6420 6162 6f76  s mentioned abov
+00004f30: 652e 0a0a 2323 204c 6963 656e 7365 0a0a  e...## License..
+00004f40: 5468 6973 2070 726f 6a65 6374 2069 7320  This project is 
+00004f50: 6c69 6365 6e73 6564 2075 6e64 6572 2074  licensed under t
+00004f60: 6865 2074 6572 6d73 206f 6620 7468 6520  he terms of the 
+00004f70: 4d49 5420 6c69 6365 6e73 652e 0a         MIT license..
```

