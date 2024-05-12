# Comparing `tmp/readyapi-0.110.2.dev1.tar.gz` & `tmp/readyapi-0.110.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "readyapi-0.110.2.dev1.tar", last modified: Sun May 12 00:15:14 2024, max compression
+gzip compressed data, was "readyapi-0.110.3.tar", last modified: Sun May 12 00:38:20 2024, max compression
```

## Comparing `readyapi-0.110.2.dev1.tar` & `readyapi-0.110.3.tar`

### file list

```diff
@@ -1,1231 +1,1231 @@
--rw-r--r--   0        0        0     1084 2024-05-12 00:15:11.635393 readyapi-0.110.2.dev1/LICENSE
--rw-r--r--   0        0        0    22670 2024-05-12 00:15:11.635393 readyapi-0.110.2.dev1/README.md
--rw-r--r--   0        0        0     5043 2024-05-12 00:15:11.671393 readyapi-0.110.2.dev1/docs/en/docs/img/favicon.png
--rw-r--r--   0        0        0      510 2024-05-12 00:15:11.755392 readyapi-0.110.2.dev1/docs_src/additional_responses/tutorial001.py
--rw-r--r--   0        0        0      632 2024-05-12 00:15:11.755392 readyapi-0.110.2.dev1/docs_src/additional_responses/tutorial002.py
--rw-r--r--   0        0        0      841 2024-05-12 00:15:11.755392 readyapi-0.110.2.dev1/docs_src/additional_responses/tutorial003.py
--rw-r--r--   0        0        0      705 2024-05-12 00:15:11.755392 readyapi-0.110.2.dev1/docs_src/additional_responses/tutorial004.py
--rw-r--r--   0        0        0      688 2024-05-12 00:15:11.755392 readyapi-0.110.2.dev1/docs_src/additional_status_codes/tutorial001.py
--rw-r--r--   0        0        0      738 2024-05-12 00:15:11.755392 readyapi-0.110.2.dev1/docs_src/additional_status_codes/tutorial001_an.py
--rw-r--r--   0        0        0      690 2024-05-12 00:15:11.755392 readyapi-0.110.2.dev1/docs_src/additional_status_codes/tutorial001_an_py310.py
--rw-r--r--   0        0        0      709 2024-05-12 00:15:11.755392 readyapi-0.110.2.dev1/docs_src/additional_status_codes/tutorial001_an_py39.py
--rw-r--r--   0        0        0      650 2024-05-12 00:15:11.755392 readyapi-0.110.2.dev1/docs_src/additional_status_codes/tutorial001_py310.py
--rw-r--r--   0        0        0      235 2024-05-12 00:15:11.755392 readyapi-0.110.2.dev1/docs_src/advanced_middleware/tutorial001.py
--rw-r--r--   0        0        0      283 2024-05-12 00:15:11.755392 readyapi-0.110.2.dev1/docs_src/advanced_middleware/tutorial002.py
--rw-r--r--   0        0        0      217 2024-05-12 00:15:11.755392 readyapi-0.110.2.dev1/docs_src/advanced_middleware/tutorial003.py
--rw-r--r--   0        0        0        0 2024-05-12 00:15:11.755392 readyapi-0.110.2.dev1/docs_src/app_testing/__init__.py
--rw-r--r--   0        0        0        0 2024-05-12 00:15:11.755392 readyapi-0.110.2.dev1/docs_src/app_testing/app_b/__init__.py
--rw-r--r--   0        0        0     1148 2024-05-12 00:15:11.755392 readyapi-0.110.2.dev1/docs_src/app_testing/app_b/main.py
--rw-r--r--   0        0        0     1867 2024-05-12 00:15:11.755392 readyapi-0.110.2.dev1/docs_src/app_testing/app_b/test_main.py
--rw-r--r--   0        0        0        0 2024-05-12 00:15:11.755392 readyapi-0.110.2.dev1/docs_src/app_testing/app_b_an/__init__.py
--rw-r--r--   0        0        0     1208 2024-05-12 00:15:11.755392 readyapi-0.110.2.dev1/docs_src/app_testing/app_b_an/main.py
--rw-r--r--   0        0        0     1867 2024-05-12 00:15:11.755392 readyapi-0.110.2.dev1/docs_src/app_testing/app_b_an/test_main.py
--rw-r--r--   0        0        0        0 2024-05-12 00:15:11.755392 readyapi-0.110.2.dev1/docs_src/app_testing/app_b_an_py310/__init__.py
--rw-r--r--   0        0        0     1166 2024-05-12 00:15:11.755392 readyapi-0.110.2.dev1/docs_src/app_testing/app_b_an_py310/main.py
--rw-r--r--   0        0        0     1867 2024-05-12 00:15:11.755392 readyapi-0.110.2.dev1/docs_src/app_testing/app_b_an_py310/test_main.py
--rw-r--r--   0        0        0        0 2024-05-12 00:15:11.755392 readyapi-0.110.2.dev1/docs_src/app_testing/app_b_an_py39/__init__.py
--rw-r--r--   0        0        0     1179 2024-05-12 00:15:11.755392 readyapi-0.110.2.dev1/docs_src/app_testing/app_b_an_py39/main.py
--rw-r--r--   0        0        0     1867 2024-05-12 00:15:11.755392 readyapi-0.110.2.dev1/docs_src/app_testing/app_b_an_py39/test_main.py
--rw-r--r--   0        0        0        0 2024-05-12 00:15:11.755392 readyapi-0.110.2.dev1/docs_src/app_testing/app_b_py310/__init__.py
--rw-r--r--   0        0        0     1116 2024-05-12 00:15:11.755392 readyapi-0.110.2.dev1/docs_src/app_testing/app_b_py310/main.py
--rw-r--r--   0        0        0     1867 2024-05-12 00:15:11.755392 readyapi-0.110.2.dev1/docs_src/app_testing/app_b_py310/test_main.py
--rw-r--r--   0        0        0      121 2024-05-12 00:15:11.755392 readyapi-0.110.2.dev1/docs_src/app_testing/main.py
--rw-r--r--   0        0        0      239 2024-05-12 00:15:11.755392 readyapi-0.110.2.dev1/docs_src/app_testing/test_main.py
--rw-r--r--   0        0        0      338 2024-05-12 00:15:11.755392 readyapi-0.110.2.dev1/docs_src/app_testing/tutorial001.py
--rw-r--r--   0        0        0      762 2024-05-12 00:15:11.755392 readyapi-0.110.2.dev1/docs_src/app_testing/tutorial002.py
--rw-r--r--   0        0        0      532 2024-05-12 00:15:11.755392 readyapi-0.110.2.dev1/docs_src/app_testing/tutorial003.py
--rw-r--r--   0        0        0     1418 2024-05-12 00:15:11.755392 readyapi-0.110.2.dev1/docs_src/async_sql_databases/tutorial001.py
--rw-r--r--   0        0        0        0 2024-05-12 00:15:11.755392 readyapi-0.110.2.dev1/docs_src/async_tests/__init__.py
--rw-r--r--   0        0        0      115 2024-05-12 00:15:11.755392 readyapi-0.110.2.dev1/docs_src/async_tests/main.py
--rw-r--r--   0        0        0      306 2024-05-12 00:15:11.755392 readyapi-0.110.2.dev1/docs_src/async_tests/test_main.py
--rw-r--r--   0        0        0      522 2024-05-12 00:15:11.755392 readyapi-0.110.2.dev1/docs_src/background_tasks/tutorial001.py
--rw-r--r--   0        0        0      678 2024-05-12 00:15:11.755392 readyapi-0.110.2.dev1/docs_src/background_tasks/tutorial002.py
--rw-r--r--   0        0        0      728 2024-05-12 00:15:11.759392 readyapi-0.110.2.dev1/docs_src/background_tasks/tutorial002_an.py
--rw-r--r--   0        0        0      686 2024-05-12 00:15:11.759392 readyapi-0.110.2.dev1/docs_src/background_tasks/tutorial002_an_py310.py
--rw-r--r--   0        0        0      699 2024-05-12 00:15:11.759392 readyapi-0.110.2.dev1/docs_src/background_tasks/tutorial002_an_py39.py
--rw-r--r--   0        0        0      646 2024-05-12 00:15:11.759392 readyapi-0.110.2.dev1/docs_src/background_tasks/tutorial002_py310.py
--rw-r--r--   0        0        0      192 2024-05-12 00:15:11.759392 readyapi-0.110.2.dev1/docs_src/behind_a_proxy/tutorial001.py
--rw-r--r--   0        0        0      211 2024-05-12 00:15:11.759392 readyapi-0.110.2.dev1/docs_src/behind_a_proxy/tutorial002.py
--rw-r--r--   0        0        0      408 2024-05-12 00:15:11.759392 readyapi-0.110.2.dev1/docs_src/behind_a_proxy/tutorial003.py
--rw-r--r--   0        0        0      440 2024-05-12 00:15:11.759392 readyapi-0.110.2.dev1/docs_src/behind_a_proxy/tutorial004.py
--rw-r--r--   0        0        0        0 2024-05-12 00:15:11.759392 readyapi-0.110.2.dev1/docs_src/bigger_applications/__init__.py
--rw-r--r--   0        0        0        0 2024-05-12 00:15:11.759392 readyapi-0.110.2.dev1/docs_src/bigger_applications/app/__init__.py
--rw-r--r--   0        0        0      370 2024-05-12 00:15:11.759392 readyapi-0.110.2.dev1/docs_src/bigger_applications/app/dependencies.py
--rw-r--r--   0        0        0        0 2024-05-12 00:15:11.759392 readyapi-0.110.2.dev1/docs_src/bigger_applications/app/internal/__init__.py
--rw-r--r--   0        0        0      148 2024-05-12 00:15:11.759392 readyapi-0.110.2.dev1/docs_src/bigger_applications/app/internal/admin.py
--rw-r--r--   0        0        0      555 2024-05-12 00:15:11.759392 readyapi-0.110.2.dev1/docs_src/bigger_applications/app/main.py
--rw-r--r--   0        0        0        0 2024-05-12 00:15:11.759392 readyapi-0.110.2.dev1/docs_src/bigger_applications/app/routers/__init__.py
--rw-r--r--   0        0        0     1012 2024-05-12 00:15:11.759392 readyapi-0.110.2.dev1/docs_src/bigger_applications/app/routers/items.py
--rw-r--r--   0        0        0      408 2024-05-12 00:15:11.759392 readyapi-0.110.2.dev1/docs_src/bigger_applications/app/routers/users.py
--rw-r--r--   0        0        0        0 2024-05-12 00:15:11.759392 readyapi-0.110.2.dev1/docs_src/bigger_applications/app_an/__init__.py
--rw-r--r--   0        0        0      420 2024-05-12 00:15:11.759392 readyapi-0.110.2.dev1/docs_src/bigger_applications/app_an/dependencies.py
--rw-r--r--   0        0        0        0 2024-05-12 00:15:11.759392 readyapi-0.110.2.dev1/docs_src/bigger_applications/app_an/internal/__init__.py
--rw-r--r--   0        0        0      148 2024-05-12 00:15:11.759392 readyapi-0.110.2.dev1/docs_src/bigger_applications/app_an/internal/admin.py
--rw-r--r--   0        0        0      555 2024-05-12 00:15:11.759392 readyapi-0.110.2.dev1/docs_src/bigger_applications/app_an/main.py
--rw-r--r--   0        0        0        0 2024-05-12 00:15:11.759392 readyapi-0.110.2.dev1/docs_src/bigger_applications/app_an/routers/__init__.py
--rw-r--r--   0        0        0     1012 2024-05-12 00:15:11.759392 readyapi-0.110.2.dev1/docs_src/bigger_applications/app_an/routers/items.py
--rw-r--r--   0        0        0      408 2024-05-12 00:15:11.759392 readyapi-0.110.2.dev1/docs_src/bigger_applications/app_an/routers/users.py
--rw-r--r--   0        0        0        0 2024-05-12 00:15:11.759392 readyapi-0.110.2.dev1/docs_src/bigger_applications/app_an_py39/__init__.py
--rw-r--r--   0        0        0      410 2024-05-12 00:15:11.759392 readyapi-0.110.2.dev1/docs_src/bigger_applications/app_an_py39/dependencies.py
--rw-r--r--   0        0        0        0 2024-05-12 00:15:11.759392 readyapi-0.110.2.dev1/docs_src/bigger_applications/app_an_py39/internal/__init__.py
--rw-r--r--   0        0        0      148 2024-05-12 00:15:11.759392 readyapi-0.110.2.dev1/docs_src/bigger_applications/app_an_py39/internal/admin.py
--rw-r--r--   0        0        0      555 2024-05-12 00:15:11.759392 readyapi-0.110.2.dev1/docs_src/bigger_applications/app_an_py39/main.py
--rw-r--r--   0        0        0        0 2024-05-12 00:15:11.759392 readyapi-0.110.2.dev1/docs_src/bigger_applications/app_an_py39/routers/__init__.py
--rw-r--r--   0        0        0     1012 2024-05-12 00:15:11.759392 readyapi-0.110.2.dev1/docs_src/bigger_applications/app_an_py39/routers/items.py
--rw-r--r--   0        0        0      408 2024-05-12 00:15:11.759392 readyapi-0.110.2.dev1/docs_src/bigger_applications/app_an_py39/routers/users.py
--rw-r--r--   0        0        0      312 2024-05-12 00:15:11.759392 readyapi-0.110.2.dev1/docs_src/body/tutorial001.py
--rw-r--r--   0        0        0      274 2024-05-12 00:15:11.759392 readyapi-0.110.2.dev1/docs_src/body/tutorial001_py310.py
--rw-r--r--   0        0        0      470 2024-05-12 00:15:11.759392 readyapi-0.110.2.dev1/docs_src/body/tutorial002.py
--rw-r--r--   0        0        0      432 2024-05-12 00:15:11.759392 readyapi-0.110.2.dev1/docs_src/body/tutorial002_py310.py
--rw-r--r--   0        0        0      365 2024-05-12 00:15:11.759392 readyapi-0.110.2.dev1/docs_src/body/tutorial003.py
--rw-r--r--   0        0        0      327 2024-05-12 00:15:11.759392 readyapi-0.110.2.dev1/docs_src/body/tutorial003_py310.py
--rw-r--r--   0        0        0      455 2024-05-12 00:15:11.759392 readyapi-0.110.2.dev1/docs_src/body/tutorial004.py
--rw-r--r--   0        0        0      411 2024-05-12 00:15:11.759392 readyapi-0.110.2.dev1/docs_src/body/tutorial004_py310.py
--rw-r--r--   0        0        0      564 2024-05-12 00:15:11.759392 readyapi-0.110.2.dev1/docs_src/body_fields/tutorial001.py
--rw-r--r--   0        0        0      614 2024-05-12 00:15:11.759392 readyapi-0.110.2.dev1/docs_src/body_fields/tutorial001_an.py
--rw-r--r--   0        0        0      566 2024-05-12 00:15:11.759392 readyapi-0.110.2.dev1/docs_src/body_fields/tutorial001_an_py310.py
--rw-r--r--   0        0        0      585 2024-05-12 00:15:11.759392 readyapi-0.110.2.dev1/docs_src/body_fields/tutorial001_an_py39.py
--rw-r--r--   0        0        0      526 2024-05-12 00:15:11.759392 readyapi-0.110.2.dev1/docs_src/body_fields/tutorial001_py310.py
--rw-r--r--   0        0        0      599 2024-05-12 00:15:11.759392 readyapi-0.110.2.dev1/docs_src/body_multiple_params/tutorial001.py
--rw-r--r--   0        0        0      642 2024-05-12 00:15:11.759392 readyapi-0.110.2.dev1/docs_src/body_multiple_params/tutorial001_an.py
--rw-r--r--   0        0        0      582 2024-05-12 00:15:11.759392 readyapi-0.110.2.dev1/docs_src/body_multiple_params/tutorial001_an_py310.py
--rw-r--r--   0        0        0      613 2024-05-12 00:15:11.759392 readyapi-0.110.2.dev1/docs_src/body_multiple_params/tutorial001_an_py39.py
--rw-r--r--   0        0        0      549 2024-05-12 00:15:11.759392 readyapi-0.110.2.dev1/docs_src/body_multiple_params/tutorial001_py310.py
--rw-r--r--   0        0        0      493 2024-05-12 00:15:11.759392 readyapi-0.110.2.dev1/docs_src/body_multiple_params/tutorial002.py
--rw-r--r--   0        0        0      449 2024-05-12 00:15:11.759392 readyapi-0.110.2.dev1/docs_src/body_multiple_params/tutorial002_py310.py
--rw-r--r--   0        0        0      551 2024-05-12 00:15:11.759392 readyapi-0.110.2.dev1/docs_src/body_multiple_params/tutorial003.py
--rw-r--r--   0        0        0      607 2024-05-12 00:15:11.759392 readyapi-0.110.2.dev1/docs_src/body_multiple_params/tutorial003_an.py
--rw-r--r--   0        0        0      553 2024-05-12 00:15:11.759392 readyapi-0.110.2.dev1/docs_src/body_multiple_params/tutorial003_an_py310.py
--rw-r--r--   0        0        0      578 2024-05-12 00:15:11.759392 readyapi-0.110.2.dev1/docs_src/body_multiple_params/tutorial003_an_py39.py
--rw-r--r--   0        0        0      507 2024-05-12 00:15:11.759392 readyapi-0.110.2.dev1/docs_src/body_multiple_params/tutorial003_py310.py
--rw-r--r--   0        0        0      656 2024-05-12 00:15:11.759392 readyapi-0.110.2.dev1/docs_src/body_multiple_params/tutorial004.py
--rw-r--r--   0        0        0      706 2024-05-12 00:15:11.759392 readyapi-0.110.2.dev1/docs_src/body_multiple_params/tutorial004_an.py
--rw-r--r--   0        0        0      646 2024-05-12 00:15:11.759392 readyapi-0.110.2.dev1/docs_src/body_multiple_params/tutorial004_an_py310.py
--rw-r--r--   0        0        0      677 2024-05-12 00:15:11.759392 readyapi-0.110.2.dev1/docs_src/body_multiple_params/tutorial004_an_py39.py
--rw-r--r--   0        0        0      606 2024-05-12 00:15:11.759392 readyapi-0.110.2.dev1/docs_src/body_multiple_params/tutorial004_py310.py
--rw-r--r--   0        0        0      410 2024-05-12 00:15:11.759392 readyapi-0.110.2.dev1/docs_src/body_multiple_params/tutorial005.py
--rw-r--r--   0        0        0      460 2024-05-12 00:15:11.759392 readyapi-0.110.2.dev1/docs_src/body_multiple_params/tutorial005_an.py
--rw-r--r--   0        0        0      412 2024-05-12 00:15:11.759392 readyapi-0.110.2.dev1/docs_src/body_multiple_params/tutorial005_an_py310.py
--rw-r--r--   0        0        0      431 2024-05-12 00:15:11.759392 readyapi-0.110.2.dev1/docs_src/body_multiple_params/tutorial005_an_py39.py
--rw-r--r--   0        0        0      372 2024-05-12 00:15:11.759392 readyapi-0.110.2.dev1/docs_src/body_multiple_params/tutorial005_py310.py
--rw-r--r--   0        0        0      405 2024-05-12 00:15:11.759392 readyapi-0.110.2.dev1/docs_src/body_nested_models/tutorial001.py
--rw-r--r--   0        0        0      367 2024-05-12 00:15:11.759392 readyapi-0.110.2.dev1/docs_src/body_nested_models/tutorial001_py310.py
--rw-r--r--   0        0        0      416 2024-05-12 00:15:11.759392 readyapi-0.110.2.dev1/docs_src/body_nested_models/tutorial002.py
--rw-r--r--   0        0        0      372 2024-05-12 00:15:11.759392 readyapi-0.110.2.dev1/docs_src/body_nested_models/tutorial002_py310.py
--rw-r--r--   0        0        0      410 2024-05-12 00:15:11.759392 readyapi-0.110.2.dev1/docs_src/body_nested_models/tutorial002_py39.py
--rw-r--r--   0        0        0      417 2024-05-12 00:15:11.759392 readyapi-0.110.2.dev1/docs_src/body_nested_models/tutorial003.py
--rw-r--r--   0        0        0      374 2024-05-12 00:15:11.759392 readyapi-0.110.2.dev1/docs_src/body_nested_models/tutorial003_py310.py
--rw-r--r--   0        0        0      412 2024-05-12 00:15:11.759392 readyapi-0.110.2.dev1/docs_src/body_nested_models/tutorial003_py39.py
--rw-r--r--   0        0        0      507 2024-05-12 00:15:11.759392 readyapi-0.110.2.dev1/docs_src/body_nested_models/tutorial004.py
--rw-r--r--   0        0        0      458 2024-05-12 00:15:11.759392 readyapi-0.110.2.dev1/docs_src/body_nested_models/tutorial004_py310.py
--rw-r--r--   0        0        0      502 2024-05-12 00:15:11.759392 readyapi-0.110.2.dev1/docs_src/body_nested_models/tutorial004_py39.py
--rw-r--r--   0        0        0      520 2024-05-12 00:15:11.759392 readyapi-0.110.2.dev1/docs_src/body_nested_models/tutorial005.py
--rw-r--r--   0        0        0      471 2024-05-12 00:15:11.759392 readyapi-0.110.2.dev1/docs_src/body_nested_models/tutorial005_py310.py
--rw-r--r--   0        0        0      515 2024-05-12 00:15:11.759392 readyapi-0.110.2.dev1/docs_src/body_nested_models/tutorial005_py39.py
--rw-r--r--   0        0        0      533 2024-05-12 00:15:11.759392 readyapi-0.110.2.dev1/docs_src/body_nested_models/tutorial006.py
--rw-r--r--   0        0        0      478 2024-05-12 00:15:11.759392 readyapi-0.110.2.dev1/docs_src/body_nested_models/tutorial006_py310.py
--rw-r--r--   0        0        0      522 2024-05-12 00:15:11.759392 readyapi-0.110.2.dev1/docs_src/body_nested_models/tutorial006_py39.py
--rw-r--r--   0        0        0      584 2024-05-12 00:15:11.759392 readyapi-0.110.2.dev1/docs_src/body_nested_models/tutorial007.py
--rw-r--r--   0        0        0      523 2024-05-12 00:15:11.759392 readyapi-0.110.2.dev1/docs_src/body_nested_models/tutorial007_py310.py
--rw-r--r--   0        0        0      573 2024-05-12 00:15:11.759392 readyapi-0.110.2.dev1/docs_src/body_nested_models/tutorial007_py39.py
--rw-r--r--   0        0        0      276 2024-05-12 00:15:11.759392 readyapi-0.110.2.dev1/docs_src/body_nested_models/tutorial008.py
--rw-r--r--   0        0        0      251 2024-05-12 00:15:11.759392 readyapi-0.110.2.dev1/docs_src/body_nested_models/tutorial008_py39.py
--rw-r--r--   0        0        0      182 2024-05-12 00:15:11.759392 readyapi-0.110.2.dev1/docs_src/body_nested_models/tutorial009.py
--rw-r--r--   0        0        0      157 2024-05-12 00:15:11.759392 readyapi-0.110.2.dev1/docs_src/body_nested_models/tutorial009_py39.py
--rw-r--r--   0        0        0      910 2024-05-12 00:15:11.759392 readyapi-0.110.2.dev1/docs_src/body_updates/tutorial001.py
--rw-r--r--   0        0        0      860 2024-05-12 00:15:11.759392 readyapi-0.110.2.dev1/docs_src/body_updates/tutorial001_py310.py
--rw-r--r--   0        0        0      904 2024-05-12 00:15:11.759392 readyapi-0.110.2.dev1/docs_src/body_updates/tutorial001_py39.py
--rw-r--r--   0        0        0     1064 2024-05-12 00:15:11.759392 readyapi-0.110.2.dev1/docs_src/body_updates/tutorial002.py
--rw-r--r--   0        0        0     1014 2024-05-12 00:15:11.759392 readyapi-0.110.2.dev1/docs_src/body_updates/tutorial002_py310.py
--rw-r--r--   0        0        0     1058 2024-05-12 00:15:11.759392 readyapi-0.110.2.dev1/docs_src/body_updates/tutorial002_py39.py
--rw-r--r--   0        0        0      284 2024-05-12 00:15:11.759392 readyapi-0.110.2.dev1/docs_src/conditional_openapi/tutorial001.py
--rw-r--r--   0        0        0      208 2024-05-12 00:15:11.759392 readyapi-0.110.2.dev1/docs_src/configure_swagger_ui/tutorial001.py
--rw-r--r--   0        0        0      219 2024-05-12 00:15:11.759392 readyapi-0.110.2.dev1/docs_src/configure_swagger_ui/tutorial002.py
--rw-r--r--   0        0        0      204 2024-05-12 00:15:11.759392 readyapi-0.110.2.dev1/docs_src/configure_swagger_ui/tutorial003.py
--rw-r--r--   0        0        0      205 2024-05-12 00:15:11.759392 readyapi-0.110.2.dev1/docs_src/cookie_params/tutorial001.py
--rw-r--r--   0        0        0      250 2024-05-12 00:15:11.759392 readyapi-0.110.2.dev1/docs_src/cookie_params/tutorial001_an.py
--rw-r--r--   0        0        0      208 2024-05-12 00:15:11.759392 readyapi-0.110.2.dev1/docs_src/cookie_params/tutorial001_an_py310.py
--rw-r--r--   0        0        0      221 2024-05-12 00:15:11.763392 readyapi-0.110.2.dev1/docs_src/cookie_params/tutorial001_an_py39.py
--rw-r--r--   0        0        0      173 2024-05-12 00:15:11.763392 readyapi-0.110.2.dev1/docs_src/cookie_params/tutorial001_py310.py
--rw-r--r--   0        0        0      467 2024-05-12 00:15:11.763392 readyapi-0.110.2.dev1/docs_src/cors/tutorial001.py
--rw-r--r--   0        0        0     1158 2024-05-12 00:15:11.763392 readyapi-0.110.2.dev1/docs_src/custom_docs_ui/tutorial001.py
--rw-r--r--   0        0        0     1180 2024-05-12 00:15:11.763392 readyapi-0.110.2.dev1/docs_src/custom_docs_ui/tutorial002.py
--rw-r--r--   0        0        0      977 2024-05-12 00:15:11.763392 readyapi-0.110.2.dev1/docs_src/custom_request_and_route/tutorial001.py
--rw-r--r--   0        0        0      937 2024-05-12 00:15:11.763392 readyapi-0.110.2.dev1/docs_src/custom_request_and_route/tutorial002.py
--rw-r--r--   0        0        0     1046 2024-05-12 00:15:11.763392 readyapi-0.110.2.dev1/docs_src/custom_request_and_route/tutorial003.py
--rw-r--r--   0        0        0      201 2024-05-12 00:15:11.763392 readyapi-0.110.2.dev1/docs_src/custom_response/tutorial001.py
--rw-r--r--   0        0        0      219 2024-05-12 00:15:11.763392 readyapi-0.110.2.dev1/docs_src/custom_response/tutorial001b.py
--rw-r--r--   0        0        0      356 2024-05-12 00:15:11.763392 readyapi-0.110.2.dev1/docs_src/custom_response/tutorial002.py
--rw-r--r--   0        0        0      398 2024-05-12 00:15:11.763392 readyapi-0.110.2.dev1/docs_src/custom_response/tutorial003.py
--rw-r--r--   0        0        0      495 2024-05-12 00:15:11.763392 readyapi-0.110.2.dev1/docs_src/custom_response/tutorial004.py
--rw-r--r--   0        0        0      190 2024-05-12 00:15:11.763392 readyapi-0.110.2.dev1/docs_src/custom_response/tutorial005.py
--rw-r--r--   0        0        0      203 2024-05-12 00:15:11.763392 readyapi-0.110.2.dev1/docs_src/custom_response/tutorial006.py
--rw-r--r--   0        0        0      229 2024-05-12 00:15:11.763392 readyapi-0.110.2.dev1/docs_src/custom_response/tutorial006b.py
--rw-r--r--   0        0        0      241 2024-05-12 00:15:11.763392 readyapi-0.110.2.dev1/docs_src/custom_response/tutorial006c.py
--rw-r--r--   0        0        0      281 2024-05-12 00:15:11.763392 readyapi-0.110.2.dev1/docs_src/custom_response/tutorial007.py
--rw-r--r--   0        0        0      364 2024-05-12 00:15:11.763392 readyapi-0.110.2.dev1/docs_src/custom_response/tutorial008.py
--rw-r--r--   0        0        0      206 2024-05-12 00:15:11.763392 readyapi-0.110.2.dev1/docs_src/custom_response/tutorial009.py
--rw-r--r--   0        0        0      221 2024-05-12 00:15:11.763392 readyapi-0.110.2.dev1/docs_src/custom_response/tutorial009b.py
--rw-r--r--   0        0        0      454 2024-05-12 00:15:11.763392 readyapi-0.110.2.dev1/docs_src/custom_response/tutorial009c.py
--rw-r--r--   0        0        0      209 2024-05-12 00:15:11.763392 readyapi-0.110.2.dev1/docs_src/custom_response/tutorial010.py
--rw-r--r--   0        0        0      315 2024-05-12 00:15:11.763392 readyapi-0.110.2.dev1/docs_src/dataclasses/tutorial001.py
--rw-r--r--   0        0        0      555 2024-05-12 00:15:11.763392 readyapi-0.110.2.dev1/docs_src/dataclasses/tutorial002.py
--rw-r--r--   0        0        0     1406 2024-05-12 00:15:11.763392 readyapi-0.110.2.dev1/docs_src/dataclasses/tutorial003.py
--rw-r--r--   0        0        0      226 2024-05-12 00:15:11.763392 readyapi-0.110.2.dev1/docs_src/debugging/tutorial001.py
--rw-r--r--   0        0        0      445 2024-05-12 00:15:11.763392 readyapi-0.110.2.dev1/docs_src/dependencies/tutorial001.py
--rw-r--r--   0        0        0      498 2024-05-12 00:15:11.763392 readyapi-0.110.2.dev1/docs_src/dependencies/tutorial001_02_an.py
--rw-r--r--   0        0        0      450 2024-05-12 00:15:11.763392 readyapi-0.110.2.dev1/docs_src/dependencies/tutorial001_02_an_py310.py
--rw-r--r--   0        0        0      469 2024-05-12 00:15:11.763392 readyapi-0.110.2.dev1/docs_src/dependencies/tutorial001_02_an_py39.py
--rw-r--r--   0        0        0      505 2024-05-12 00:15:11.763392 readyapi-0.110.2.dev1/docs_src/dependencies/tutorial001_an.py
--rw-r--r--   0        0        0      457 2024-05-12 00:15:11.763392 readyapi-0.110.2.dev1/docs_src/dependencies/tutorial001_an_py310.py
--rw-r--r--   0        0        0      476 2024-05-12 00:15:11.763392 readyapi-0.110.2.dev1/docs_src/dependencies/tutorial001_an_py39.py
--rw-r--r--   0        0        0      407 2024-05-12 00:15:11.763392 readyapi-0.110.2.dev1/docs_src/dependencies/tutorial001_py310.py
--rw-r--r--   0        0        0      659 2024-05-12 00:15:11.763392 readyapi-0.110.2.dev1/docs_src/dependencies/tutorial002.py
--rw-r--r--   0        0        0      709 2024-05-12 00:15:11.763392 readyapi-0.110.2.dev1/docs_src/dependencies/tutorial002_an.py
--rw-r--r--   0        0        0      667 2024-05-12 00:15:11.763392 readyapi-0.110.2.dev1/docs_src/dependencies/tutorial002_an_py310.py
--rw-r--r--   0        0        0      680 2024-05-12 00:15:11.763392 readyapi-0.110.2.dev1/docs_src/dependencies/tutorial002_an_py39.py
--rw-r--r--   0        0        0      627 2024-05-12 00:15:11.763392 readyapi-0.110.2.dev1/docs_src/dependencies/tutorial002_py310.py
--rw-r--r--   0        0        0      638 2024-05-12 00:15:11.763392 readyapi-0.110.2.dev1/docs_src/dependencies/tutorial003.py
--rw-r--r--   0        0        0      700 2024-05-12 00:15:11.763392 readyapi-0.110.2.dev1/docs_src/dependencies/tutorial003_an.py
--rw-r--r--   0        0        0      658 2024-05-12 00:15:11.763392 readyapi-0.110.2.dev1/docs_src/dependencies/tutorial003_an_py310.py
--rw-r--r--   0        0        0      671 2024-05-12 00:15:11.763392 readyapi-0.110.2.dev1/docs_src/dependencies/tutorial003_an_py39.py
--rw-r--r--   0        0        0      606 2024-05-12 00:15:11.763392 readyapi-0.110.2.dev1/docs_src/dependencies/tutorial003_py310.py
--rw-r--r--   0        0        0      642 2024-05-12 00:15:11.763392 readyapi-0.110.2.dev1/docs_src/dependencies/tutorial004.py
--rw-r--r--   0        0        0      692 2024-05-12 00:15:11.763392 readyapi-0.110.2.dev1/docs_src/dependencies/tutorial004_an.py
--rw-r--r--   0        0        0      650 2024-05-12 00:15:11.763392 readyapi-0.110.2.dev1/docs_src/dependencies/tutorial004_an_py310.py
--rw-r--r--   0        0        0      663 2024-05-12 00:15:11.763392 readyapi-0.110.2.dev1/docs_src/dependencies/tutorial004_an_py39.py
--rw-r--r--   0        0        0      610 2024-05-12 00:15:11.763392 readyapi-0.110.2.dev1/docs_src/dependencies/tutorial004_py310.py
--rw-r--r--   0        0        0      489 2024-05-12 00:15:11.763392 readyapi-0.110.2.dev1/docs_src/dependencies/tutorial005.py
--rw-r--r--   0        0        0      561 2024-05-12 00:15:11.763392 readyapi-0.110.2.dev1/docs_src/dependencies/tutorial005_an.py
--rw-r--r--   0        0        0      513 2024-05-12 00:15:11.763392 readyapi-0.110.2.dev1/docs_src/dependencies/tutorial005_an_py310.py
--rw-r--r--   0        0        0      532 2024-05-12 00:15:11.763392 readyapi-0.110.2.dev1/docs_src/dependencies/tutorial005_an_py39.py
--rw-r--r--   0        0        0      446 2024-05-12 00:15:11.763392 readyapi-0.110.2.dev1/docs_src/dependencies/tutorial005_py310.py
--rw-r--r--   0        0        0      586 2024-05-12 00:15:11.763392 readyapi-0.110.2.dev1/docs_src/dependencies/tutorial006.py
--rw-r--r--   0        0        0      646 2024-05-12 00:15:11.763392 readyapi-0.110.2.dev1/docs_src/dependencies/tutorial006_an.py
--rw-r--r--   0        0        0      636 2024-05-12 00:15:11.763392 readyapi-0.110.2.dev1/docs_src/dependencies/tutorial006_an_py39.py
--rw-r--r--   0        0        0       99 2024-05-12 00:15:11.763392 readyapi-0.110.2.dev1/docs_src/dependencies/tutorial007.py
--rw-r--r--   0        0        0      456 2024-05-12 00:15:11.763392 readyapi-0.110.2.dev1/docs_src/dependencies/tutorial008.py
--rw-r--r--   0        0        0      532 2024-05-12 00:15:11.763392 readyapi-0.110.2.dev1/docs_src/dependencies/tutorial008_an.py
--rw-r--r--   0        0        0      522 2024-05-12 00:15:11.763392 readyapi-0.110.2.dev1/docs_src/dependencies/tutorial008_an_py39.py
--rw-r--r--   0        0        0      738 2024-05-12 00:15:11.763392 readyapi-0.110.2.dev1/docs_src/dependencies/tutorial008b.py
--rw-r--r--   0        0        0      788 2024-05-12 00:15:11.763392 readyapi-0.110.2.dev1/docs_src/dependencies/tutorial008b_an.py
--rw-r--r--   0        0        0      778 2024-05-12 00:15:11.763392 readyapi-0.110.2.dev1/docs_src/dependencies/tutorial008b_an_py39.py
--rw-r--r--   0        0        0      663 2024-05-12 00:15:11.763392 readyapi-0.110.2.dev1/docs_src/dependencies/tutorial008c.py
--rw-r--r--   0        0        0      713 2024-05-12 00:15:11.763392 readyapi-0.110.2.dev1/docs_src/dependencies/tutorial008c_an.py
--rw-r--r--   0        0        0      703 2024-05-12 00:15:11.763392 readyapi-0.110.2.dev1/docs_src/dependencies/tutorial008c_an_py39.py
--rw-r--r--   0        0        0      697 2024-05-12 00:15:11.763392 readyapi-0.110.2.dev1/docs_src/dependencies/tutorial008d.py
--rw-r--r--   0        0        0      747 2024-05-12 00:15:11.763392 readyapi-0.110.2.dev1/docs_src/dependencies/tutorial008d_an.py
--rw-r--r--   0        0        0      737 2024-05-12 00:15:11.763392 readyapi-0.110.2.dev1/docs_src/dependencies/tutorial008d_an_py39.py
--rw-r--r--   0        0        0      456 2024-05-12 00:15:11.763392 readyapi-0.110.2.dev1/docs_src/dependencies/tutorial009.py
--rw-r--r--   0        0        0      292 2024-05-12 00:15:11.763392 readyapi-0.110.2.dev1/docs_src/dependencies/tutorial010.py
--rw-r--r--   0        0        0      507 2024-05-12 00:15:11.763392 readyapi-0.110.2.dev1/docs_src/dependencies/tutorial011.py
--rw-r--r--   0        0        0      557 2024-05-12 00:15:11.763392 readyapi-0.110.2.dev1/docs_src/dependencies/tutorial011_an.py
--rw-r--r--   0        0        0      547 2024-05-12 00:15:11.763392 readyapi-0.110.2.dev1/docs_src/dependencies/tutorial011_an_py39.py
--rw-r--r--   0        0        0      699 2024-05-12 00:15:11.763392 readyapi-0.110.2.dev1/docs_src/dependencies/tutorial012.py
--rw-r--r--   0        0        0      759 2024-05-12 00:15:11.763392 readyapi-0.110.2.dev1/docs_src/dependencies/tutorial012_an.py
--rw-r--r--   0        0        0      759 2024-05-12 00:15:11.763392 readyapi-0.110.2.dev1/docs_src/dependencies/tutorial012_an_py39.py
--rw-r--r--   0        0        0     1526 2024-05-12 00:15:11.763392 readyapi-0.110.2.dev1/docs_src/dependency_testing/tutorial001.py
--rw-r--r--   0        0        0     1586 2024-05-12 00:15:11.763392 readyapi-0.110.2.dev1/docs_src/dependency_testing/tutorial001_an.py
--rw-r--r--   0        0        0     1532 2024-05-12 00:15:11.763392 readyapi-0.110.2.dev1/docs_src/dependency_testing/tutorial001_an_py310.py
--rw-r--r--   0        0        0     1557 2024-05-12 00:15:11.763392 readyapi-0.110.2.dev1/docs_src/dependency_testing/tutorial001_an_py39.py
--rw-r--r--   0        0        0     1482 2024-05-12 00:15:11.763392 readyapi-0.110.2.dev1/docs_src/dependency_testing/tutorial001_py310.py
--rw-r--r--   0        0        0      465 2024-05-12 00:15:11.763392 readyapi-0.110.2.dev1/docs_src/encoder/tutorial001.py
--rw-r--r--   0        0        0      434 2024-05-12 00:15:11.763392 readyapi-0.110.2.dev1/docs_src/encoder/tutorial001_py310.py
--rw-r--r--   0        0        0      286 2024-05-12 00:15:11.763392 readyapi-0.110.2.dev1/docs_src/events/tutorial001.py
--rw-r--r--   0        0        0      258 2024-05-12 00:15:11.763392 readyapi-0.110.2.dev1/docs_src/events/tutorial002.py
--rw-r--r--   0        0        0      573 2024-05-12 00:15:11.763392 readyapi-0.110.2.dev1/docs_src/events/tutorial003.py
--rw-r--r--   0        0        0      744 2024-05-12 00:15:11.763392 readyapi-0.110.2.dev1/docs_src/extending_openapi/tutorial001.py
--rw-r--r--   0        0        0      833 2024-05-12 00:15:11.763392 readyapi-0.110.2.dev1/docs_src/extra_data_types/tutorial001.py
--rw-r--r--   0        0        0      893 2024-05-12 00:15:11.763392 readyapi-0.110.2.dev1/docs_src/extra_data_types/tutorial001_an.py
--rw-r--r--   0        0        0      833 2024-05-12 00:15:11.763392 readyapi-0.110.2.dev1/docs_src/extra_data_types/tutorial001_an_py310.py
--rw-r--r--   0        0        0      864 2024-05-12 00:15:11.763392 readyapi-0.110.2.dev1/docs_src/extra_data_types/tutorial001_an_py39.py
--rw-r--r--   0        0        0      784 2024-05-12 00:15:11.763392 readyapi-0.110.2.dev1/docs_src/extra_data_types/tutorial001_py310.py
--rw-r--r--   0        0        0      946 2024-05-12 00:15:11.763392 readyapi-0.110.2.dev1/docs_src/extra_models/tutorial001.py
--rw-r--r--   0        0        0      902 2024-05-12 00:15:11.763392 readyapi-0.110.2.dev1/docs_src/extra_models/tutorial001_py310.py
--rw-r--r--   0        0        0      827 2024-05-12 00:15:11.763392 readyapi-0.110.2.dev1/docs_src/extra_models/tutorial002.py
--rw-r--r--   0        0        0      795 2024-05-12 00:15:11.763392 readyapi-0.110.2.dev1/docs_src/extra_models/tutorial002_py310.py
--rw-r--r--   0        0        0      647 2024-05-12 00:15:11.763392 readyapi-0.110.2.dev1/docs_src/extra_models/tutorial003.py
--rw-r--r--   0        0        0      647 2024-05-12 00:15:11.763392 readyapi-0.110.2.dev1/docs_src/extra_models/tutorial003_py310.py
--rw-r--r--   0        0        0      384 2024-05-12 00:15:11.763392 readyapi-0.110.2.dev1/docs_src/extra_models/tutorial004.py
--rw-r--r--   0        0        0      359 2024-05-12 00:15:11.763392 readyapi-0.110.2.dev1/docs_src/extra_models/tutorial004_py39.py
--rw-r--r--   0        0        0      208 2024-05-12 00:15:11.763392 readyapi-0.110.2.dev1/docs_src/extra_models/tutorial005.py
--rw-r--r--   0        0        0      183 2024-05-12 00:15:11.763392 readyapi-0.110.2.dev1/docs_src/extra_models/tutorial005_py39.py
--rw-r--r--   0        0        0      120 2024-05-12 00:15:11.763392 readyapi-0.110.2.dev1/docs_src/first_steps/tutorial001.py
--rw-r--r--   0        0        0      142 2024-05-12 00:15:11.763392 readyapi-0.110.2.dev1/docs_src/first_steps/tutorial002.py
--rw-r--r--   0        0        0      114 2024-05-12 00:15:11.763392 readyapi-0.110.2.dev1/docs_src/first_steps/tutorial003.py
--rw-r--r--   0        0        0      522 2024-05-12 00:15:11.763392 readyapi-0.110.2.dev1/docs_src/generate_clients/tutorial001.py
--rw-r--r--   0        0        0      497 2024-05-12 00:15:11.763392 readyapi-0.110.2.dev1/docs_src/generate_clients/tutorial001_py39.py
--rw-r--r--   0        0        0      758 2024-05-12 00:15:11.767392 readyapi-0.110.2.dev1/docs_src/generate_clients/tutorial002.py
--rw-r--r--   0        0        0      733 2024-05-12 00:15:11.767392 readyapi-0.110.2.dev1/docs_src/generate_clients/tutorial002_py39.py
--rw-r--r--   0        0        0      943 2024-05-12 00:15:11.767392 readyapi-0.110.2.dev1/docs_src/generate_clients/tutorial003.py
--rw-r--r--   0        0        0      918 2024-05-12 00:15:11.767392 readyapi-0.110.2.dev1/docs_src/generate_clients/tutorial003_py39.py
--rw-r--r--   0        0        0     1066 2024-05-12 00:15:11.767392 readyapi-0.110.2.dev1/docs_src/generate_clients/tutorial004.js
--rw-r--r--   0        0        0      493 2024-05-12 00:15:11.767392 readyapi-0.110.2.dev1/docs_src/generate_clients/tutorial004.py
--rw-r--r--   0        0        0      449 2024-05-12 00:15:11.767392 readyapi-0.110.2.dev1/docs_src/graphql/tutorial001.py
--rw-r--r--   0        0        0      302 2024-05-12 00:15:11.767392 readyapi-0.110.2.dev1/docs_src/handling_errors/tutorial001.py
--rw-r--r--   0        0        0      407 2024-05-12 00:15:11.767392 readyapi-0.110.2.dev1/docs_src/handling_errors/tutorial002.py
--rw-r--r--   0        0        0      630 2024-05-12 00:15:11.767392 readyapi-0.110.2.dev1/docs_src/handling_errors/tutorial003.py
--rw-r--r--   0        0        0      767 2024-05-12 00:15:11.767392 readyapi-0.110.2.dev1/docs_src/handling_errors/tutorial004.py
--rw-r--r--   0        0        0      673 2024-05-12 00:15:11.767392 readyapi-0.110.2.dev1/docs_src/handling_errors/tutorial005.py
--rw-r--r--   0        0        0      933 2024-05-12 00:15:11.767392 readyapi-0.110.2.dev1/docs_src/handling_errors/tutorial006.py
--rw-r--r--   0        0        0      217 2024-05-12 00:15:11.767392 readyapi-0.110.2.dev1/docs_src/header_params/tutorial001.py
--rw-r--r--   0        0        0      262 2024-05-12 00:15:11.767392 readyapi-0.110.2.dev1/docs_src/header_params/tutorial001_an.py
--rw-r--r--   0        0        0      220 2024-05-12 00:15:11.767392 readyapi-0.110.2.dev1/docs_src/header_params/tutorial001_an_py310.py
--rw-r--r--   0        0        0      233 2024-05-12 00:15:11.767392 readyapi-0.110.2.dev1/docs_src/header_params/tutorial001_an_py39.py
--rw-r--r--   0        0        0      185 2024-05-12 00:15:11.767392 readyapi-0.110.2.dev1/docs_src/header_params/tutorial001_py310.py
--rw-r--r--   0        0        0      263 2024-05-12 00:15:11.767392 readyapi-0.110.2.dev1/docs_src/header_params/tutorial002.py
--rw-r--r--   0        0        0      320 2024-05-12 00:15:11.767392 readyapi-0.110.2.dev1/docs_src/header_params/tutorial002_an.py
--rw-r--r--   0        0        0      264 2024-05-12 00:15:11.767392 readyapi-0.110.2.dev1/docs_src/header_params/tutorial002_an_py310.py
--rw-r--r--   0        0        0      291 2024-05-12 00:15:11.767392 readyapi-0.110.2.dev1/docs_src/header_params/tutorial002_an_py39.py
--rw-r--r--   0        0        0      231 2024-05-12 00:15:11.767392 readyapi-0.110.2.dev1/docs_src/header_params/tutorial002_py310.py
--rw-r--r--   0        0        0      227 2024-05-12 00:15:11.767392 readyapi-0.110.2.dev1/docs_src/header_params/tutorial003.py
--rw-r--r--   0        0        0      272 2024-05-12 00:15:11.767392 readyapi-0.110.2.dev1/docs_src/header_params/tutorial003_an.py
--rw-r--r--   0        0        0      224 2024-05-12 00:15:11.767392 readyapi-0.110.2.dev1/docs_src/header_params/tutorial003_an_py310.py
--rw-r--r--   0        0        0      243 2024-05-12 00:15:11.767392 readyapi-0.110.2.dev1/docs_src/header_params/tutorial003_an_py39.py
--rw-r--r--   0        0        0      189 2024-05-12 00:15:11.767392 readyapi-0.110.2.dev1/docs_src/header_params/tutorial003_py310.py
--rw-r--r--   0        0        0      221 2024-05-12 00:15:11.767392 readyapi-0.110.2.dev1/docs_src/header_params/tutorial003_py39.py
--rw-r--r--   0        0        0      808 2024-05-12 00:15:11.767392 readyapi-0.110.2.dev1/docs_src/metadata/tutorial001.py
--rw-r--r--   0        0        0      770 2024-05-12 00:15:11.767392 readyapi-0.110.2.dev1/docs_src/metadata/tutorial001_1.py
--rw-r--r--   0        0        0      157 2024-05-12 00:15:11.767392 readyapi-0.110.2.dev1/docs_src/metadata/tutorial002.py
--rw-r--r--   0        0        0      164 2024-05-12 00:15:11.767392 readyapi-0.110.2.dev1/docs_src/metadata/tutorial003.py
--rw-r--r--   0        0        0      699 2024-05-12 00:15:11.767392 readyapi-0.110.2.dev1/docs_src/metadata/tutorial004.py
--rw-r--r--   0        0        0      352 2024-05-12 00:15:11.767392 readyapi-0.110.2.dev1/docs_src/middleware/tutorial001.py
--rw-r--r--   0        0        0     1361 2024-05-12 00:15:11.767392 readyapi-0.110.2.dev1/docs_src/nosql_databases/tutorial001.py
--rw-r--r--   0        0        0     1374 2024-05-12 00:15:11.767392 readyapi-0.110.2.dev1/docs_src/openapi_callbacks/tutorial001.py
--rw-r--r--   0        0        0      553 2024-05-12 00:15:11.767392 readyapi-0.110.2.dev1/docs_src/openapi_webhooks/tutorial001.py
--rw-r--r--   0        0        0      170 2024-05-12 00:15:11.767392 readyapi-0.110.2.dev1/docs_src/path_operation_advanced_configuration/tutorial001.py
--rw-r--r--   0        0        0      577 2024-05-12 00:15:11.767392 readyapi-0.110.2.dev1/docs_src/path_operation_advanced_configuration/tutorial002.py
--rw-r--r--   0        0        0      151 2024-05-12 00:15:11.767392 readyapi-0.110.2.dev1/docs_src/path_operation_advanced_configuration/tutorial003.py
--rw-r--r--   0        0        0      720 2024-05-12 00:15:11.767392 readyapi-0.110.2.dev1/docs_src/path_operation_advanced_configuration/tutorial004.py
--rw-r--r--   0        0        0      183 2024-05-12 00:15:11.767392 readyapi-0.110.2.dev1/docs_src/path_operation_advanced_configuration/tutorial005.py
--rw-r--r--   0        0        0     1046 2024-05-12 00:15:11.767392 readyapi-0.110.2.dev1/docs_src/path_operation_advanced_configuration/tutorial006.py
--rw-r--r--   0        0        0      825 2024-05-12 00:15:11.767392 readyapi-0.110.2.dev1/docs_src/path_operation_advanced_configuration/tutorial007.py
--rw-r--r--   0        0        0      792 2024-05-12 00:15:11.767392 readyapi-0.110.2.dev1/docs_src/path_operation_advanced_configuration/tutorial007_pv1.py
--rw-r--r--   0        0        0      409 2024-05-12 00:15:11.767392 readyapi-0.110.2.dev1/docs_src/path_operation_configuration/tutorial001.py
--rw-r--r--   0        0        0      366 2024-05-12 00:15:11.767392 readyapi-0.110.2.dev1/docs_src/path_operation_configuration/tutorial001_py310.py
--rw-r--r--   0        0        0      404 2024-05-12 00:15:11.767392 readyapi-0.110.2.dev1/docs_src/path_operation_configuration/tutorial001_py39.py
--rw-r--r--   0        0        0      583 2024-05-12 00:15:11.767392 readyapi-0.110.2.dev1/docs_src/path_operation_configuration/tutorial002.py
--rw-r--r--   0        0        0      540 2024-05-12 00:15:11.767392 readyapi-0.110.2.dev1/docs_src/path_operation_configuration/tutorial002_py310.py
--rw-r--r--   0        0        0      578 2024-05-12 00:15:11.767392 readyapi-0.110.2.dev1/docs_src/path_operation_configuration/tutorial002_py39.py
--rw-r--r--   0        0        0      326 2024-05-12 00:15:11.767392 readyapi-0.110.2.dev1/docs_src/path_operation_configuration/tutorial002b.py
--rw-r--r--   0        0        0      520 2024-05-12 00:15:11.767392 readyapi-0.110.2.dev1/docs_src/path_operation_configuration/tutorial003.py
--rw-r--r--   0        0        0      477 2024-05-12 00:15:11.767392 readyapi-0.110.2.dev1/docs_src/path_operation_configuration/tutorial003_py310.py
--rw-r--r--   0        0        0      515 2024-05-12 00:15:11.767392 readyapi-0.110.2.dev1/docs_src/path_operation_configuration/tutorial003_py39.py
--rw-r--r--   0        0        0      684 2024-05-12 00:15:11.767392 readyapi-0.110.2.dev1/docs_src/path_operation_configuration/tutorial004.py
--rw-r--r--   0        0        0      641 2024-05-12 00:15:11.767392 readyapi-0.110.2.dev1/docs_src/path_operation_configuration/tutorial004_py310.py
--rw-r--r--   0        0        0      679 2024-05-12 00:15:11.767392 readyapi-0.110.2.dev1/docs_src/path_operation_configuration/tutorial004_py39.py
--rw-r--r--   0        0        0      744 2024-05-12 00:15:11.767392 readyapi-0.110.2.dev1/docs_src/path_operation_configuration/tutorial005.py
--rw-r--r--   0        0        0      701 2024-05-12 00:15:11.767392 readyapi-0.110.2.dev1/docs_src/path_operation_configuration/tutorial005_py310.py
--rw-r--r--   0        0        0      739 2024-05-12 00:15:11.767392 readyapi-0.110.2.dev1/docs_src/path_operation_configuration/tutorial005_py39.py
--rw-r--r--   0        0        0      368 2024-05-12 00:15:11.767392 readyapi-0.110.2.dev1/docs_src/path_operation_configuration/tutorial006.py
--rw-r--r--   0        0        0      141 2024-05-12 00:15:11.767392 readyapi-0.110.2.dev1/docs_src/path_params/tutorial001.py
--rw-r--r--   0        0        0      146 2024-05-12 00:15:11.767392 readyapi-0.110.2.dev1/docs_src/path_params/tutorial002.py
--rw-r--r--   0        0        0      239 2024-05-12 00:15:11.767392 readyapi-0.110.2.dev1/docs_src/path_params/tutorial003.py
--rw-r--r--   0        0        0      196 2024-05-12 00:15:11.767392 readyapi-0.110.2.dev1/docs_src/path_params/tutorial003b.py
--rw-r--r--   0        0        0      159 2024-05-12 00:15:11.767392 readyapi-0.110.2.dev1/docs_src/path_params/tutorial004.py
--rw-r--r--   0        0        0      549 2024-05-12 00:15:11.767392 readyapi-0.110.2.dev1/docs_src/path_params/tutorial005.py
--rw-r--r--   0        0        0      367 2024-05-12 00:15:11.767392 readyapi-0.110.2.dev1/docs_src/path_params_numeric_validations/tutorial001.py
--rw-r--r--   0        0        0      420 2024-05-12 00:15:11.767392 readyapi-0.110.2.dev1/docs_src/path_params_numeric_validations/tutorial001_an.py
--rw-r--r--   0        0        0      378 2024-05-12 00:15:11.767392 readyapi-0.110.2.dev1/docs_src/path_params_numeric_validations/tutorial001_an_py310.py
--rw-r--r--   0        0        0      391 2024-05-12 00:15:11.767392 readyapi-0.110.2.dev1/docs_src/path_params_numeric_validations/tutorial001_an_py39.py
--rw-r--r--   0        0        0      335 2024-05-12 00:15:11.767392 readyapi-0.110.2.dev1/docs_src/path_params_numeric_validations/tutorial001_py310.py
--rw-r--r--   0        0        0      268 2024-05-12 00:15:11.767392 readyapi-0.110.2.dev1/docs_src/path_params_numeric_validations/tutorial002.py
--rw-r--r--   0        0        0      324 2024-05-12 00:15:11.767392 readyapi-0.110.2.dev1/docs_src/path_params_numeric_validations/tutorial002_an.py
--rw-r--r--   0        0        0      314 2024-05-12 00:15:11.767392 readyapi-0.110.2.dev1/docs_src/path_params_numeric_validations/tutorial002_an_py39.py
--rw-r--r--   0        0        0      271 2024-05-12 00:15:11.767392 readyapi-0.110.2.dev1/docs_src/path_params_numeric_validations/tutorial003.py
--rw-r--r--   0        0        0      324 2024-05-12 00:15:11.767392 readyapi-0.110.2.dev1/docs_src/path_params_numeric_validations/tutorial003_an.py
--rw-r--r--   0        0        0      314 2024-05-12 00:15:11.767392 readyapi-0.110.2.dev1/docs_src/path_params_numeric_validations/tutorial003_an_py39.py
--rw-r--r--   0        0        0      283 2024-05-12 00:15:11.767392 readyapi-0.110.2.dev1/docs_src/path_params_numeric_validations/tutorial004.py
--rw-r--r--   0        0        0      330 2024-05-12 00:15:11.767392 readyapi-0.110.2.dev1/docs_src/path_params_numeric_validations/tutorial004_an.py
--rw-r--r--   0        0        0      320 2024-05-12 00:15:11.767392 readyapi-0.110.2.dev1/docs_src/path_params_numeric_validations/tutorial004_an_py39.py
--rw-r--r--   0        0        0      301 2024-05-12 00:15:11.767392 readyapi-0.110.2.dev1/docs_src/path_params_numeric_validations/tutorial005.py
--rw-r--r--   0        0        0      344 2024-05-12 00:15:11.767392 readyapi-0.110.2.dev1/docs_src/path_params_numeric_validations/tutorial005_an.py
--rw-r--r--   0        0        0      334 2024-05-12 00:15:11.767392 readyapi-0.110.2.dev1/docs_src/path_params_numeric_validations/tutorial005_an_py39.py
--rw-r--r--   0        0        0      348 2024-05-12 00:15:11.767392 readyapi-0.110.2.dev1/docs_src/path_params_numeric_validations/tutorial006.py
--rw-r--r--   0        0        0      408 2024-05-12 00:15:11.767392 readyapi-0.110.2.dev1/docs_src/path_params_numeric_validations/tutorial006_an.py
--rw-r--r--   0        0        0      398 2024-05-12 00:15:11.767392 readyapi-0.110.2.dev1/docs_src/path_params_numeric_validations/tutorial006_an_py39.py
--rw-r--r--   0        0        0      162 2024-05-12 00:15:11.767392 readyapi-0.110.2.dev1/docs_src/python_types/tutorial001.py
--rw-r--r--   0        0        0      172 2024-05-12 00:15:11.767392 readyapi-0.110.2.dev1/docs_src/python_types/tutorial002.py
--rw-r--r--   0        0        0      119 2024-05-12 00:15:11.767392 readyapi-0.110.2.dev1/docs_src/python_types/tutorial003.py
--rw-r--r--   0        0        0      124 2024-05-12 00:15:11.767392 readyapi-0.110.2.dev1/docs_src/python_types/tutorial004.py
--rw-r--r--   0        0        0      143 2024-05-12 00:15:11.767392 readyapi-0.110.2.dev1/docs_src/python_types/tutorial005.py
--rw-r--r--   0        0        0      106 2024-05-12 00:15:11.767392 readyapi-0.110.2.dev1/docs_src/python_types/tutorial006.py
--rw-r--r--   0        0        0       80 2024-05-12 00:15:11.767392 readyapi-0.110.2.dev1/docs_src/python_types/tutorial006_py39.py
--rw-r--r--   0        0        0      131 2024-05-12 00:15:11.767392 readyapi-0.110.2.dev1/docs_src/python_types/tutorial007.py
--rw-r--r--   0        0        0       99 2024-05-12 00:15:11.767392 readyapi-0.110.2.dev1/docs_src/python_types/tutorial007_py39.py
--rw-r--r--   0        0        0      171 2024-05-12 00:15:11.767392 readyapi-0.110.2.dev1/docs_src/python_types/tutorial008.py
--rw-r--r--   0        0        0      145 2024-05-12 00:15:11.767392 readyapi-0.110.2.dev1/docs_src/python_types/tutorial008_py39.py
--rw-r--r--   0        0        0       84 2024-05-12 00:15:11.767392 readyapi-0.110.2.dev1/docs_src/python_types/tutorial008b.py
--rw-r--r--   0        0        0       51 2024-05-12 00:15:11.767392 readyapi-0.110.2.dev1/docs_src/python_types/tutorial008b_py310.py
--rw-r--r--   0        0        0      164 2024-05-12 00:15:11.767392 readyapi-0.110.2.dev1/docs_src/python_types/tutorial009.py
--rw-r--r--   0        0        0      131 2024-05-12 00:15:11.767392 readyapi-0.110.2.dev1/docs_src/python_types/tutorial009_py310.py
--rw-r--r--   0        0        0      164 2024-05-12 00:15:11.767392 readyapi-0.110.2.dev1/docs_src/python_types/tutorial009b.py
--rw-r--r--   0        0        0       89 2024-05-12 00:15:11.767392 readyapi-0.110.2.dev1/docs_src/python_types/tutorial009c.py
--rw-r--r--   0        0        0       56 2024-05-12 00:15:11.767392 readyapi-0.110.2.dev1/docs_src/python_types/tutorial009c_py310.py
--rw-r--r--   0        0        0      144 2024-05-12 00:15:11.767392 readyapi-0.110.2.dev1/docs_src/python_types/tutorial010.py
--rw-r--r--   0        0        0      498 2024-05-12 00:15:11.767392 readyapi-0.110.2.dev1/docs_src/python_types/tutorial011.py
--rw-r--r--   0        0        0      461 2024-05-12 00:15:11.767392 readyapi-0.110.2.dev1/docs_src/python_types/tutorial011_py310.py
--rw-r--r--   0        0        0      492 2024-05-12 00:15:11.767392 readyapi-0.110.2.dev1/docs_src/python_types/tutorial011_py39.py
--rw-r--r--   0        0        0      122 2024-05-12 00:15:11.767392 readyapi-0.110.2.dev1/docs_src/python_types/tutorial012.py
--rw-r--r--   0        0        0      138 2024-05-12 00:15:11.767392 readyapi-0.110.2.dev1/docs_src/python_types/tutorial013.py
--rw-r--r--   0        0        0      127 2024-05-12 00:15:11.771392 readyapi-0.110.2.dev1/docs_src/python_types/tutorial013_py39.py
--rw-r--r--   0        0        0      253 2024-05-12 00:15:11.771392 readyapi-0.110.2.dev1/docs_src/query_params/tutorial001.py
--rw-r--r--   0        0        0      254 2024-05-12 00:15:11.771392 readyapi-0.110.2.dev1/docs_src/query_params/tutorial002.py
--rw-r--r--   0        0        0      222 2024-05-12 00:15:11.771392 readyapi-0.110.2.dev1/docs_src/query_params/tutorial002_py310.py
--rw-r--r--   0        0        0      409 2024-05-12 00:15:11.771392 readyapi-0.110.2.dev1/docs_src/query_params/tutorial003.py
--rw-r--r--   0        0        0      377 2024-05-12 00:15:11.771392 readyapi-0.110.2.dev1/docs_src/query_params/tutorial003_py310.py
--rw-r--r--   0        0        0      471 2024-05-12 00:15:11.771392 readyapi-0.110.2.dev1/docs_src/query_params/tutorial004.py
--rw-r--r--   0        0        0      439 2024-05-12 00:15:11.771392 readyapi-0.110.2.dev1/docs_src/query_params/tutorial004_py310.py
--rw-r--r--   0        0        0      195 2024-05-12 00:15:11.771392 readyapi-0.110.2.dev1/docs_src/query_params/tutorial005.py
--rw-r--r--   0        0        0      304 2024-05-12 00:15:11.771392 readyapi-0.110.2.dev1/docs_src/query_params/tutorial006.py
--rw-r--r--   0        0        0      272 2024-05-12 00:15:11.771392 readyapi-0.110.2.dev1/docs_src/query_params/tutorial006_py310.py
--rw-r--r--   0        0        0      304 2024-05-12 00:15:11.771392 readyapi-0.110.2.dev1/docs_src/query_params/tutorial006b.py
--rw-r--r--   0        0        0      274 2024-05-12 00:15:11.771392 readyapi-0.110.2.dev1/docs_src/query_params_str_validations/tutorial001.py
--rw-r--r--   0        0        0      242 2024-05-12 00:15:11.771392 readyapi-0.110.2.dev1/docs_src/query_params_str_validations/tutorial001_py310.py
--rw-r--r--   0        0        0      311 2024-05-12 00:15:11.771392 readyapi-0.110.2.dev1/docs_src/query_params_str_validations/tutorial002.py
--rw-r--r--   0        0        0      354 2024-05-12 00:15:11.771392 readyapi-0.110.2.dev1/docs_src/query_params_str_validations/tutorial002_an.py
--rw-r--r--   0        0        0      312 2024-05-12 00:15:11.771392 readyapi-0.110.2.dev1/docs_src/query_params_str_validations/tutorial002_an_py310.py
--rw-r--r--   0        0        0      279 2024-05-12 00:15:11.771392 readyapi-0.110.2.dev1/docs_src/query_params_str_validations/tutorial002_py310.py
--rw-r--r--   0        0        0      332 2024-05-12 00:15:11.771392 readyapi-0.110.2.dev1/docs_src/query_params_str_validations/tutorial003.py
--rw-r--r--   0        0        0      375 2024-05-12 00:15:11.771392 readyapi-0.110.2.dev1/docs_src/query_params_str_validations/tutorial003_an.py
--rw-r--r--   0        0        0      333 2024-05-12 00:15:11.771392 readyapi-0.110.2.dev1/docs_src/query_params_str_validations/tutorial003_an_py310.py
--rw-r--r--   0        0        0      346 2024-05-12 00:15:11.771392 readyapi-0.110.2.dev1/docs_src/query_params_str_validations/tutorial003_an_py39.py
--rw-r--r--   0        0        0      293 2024-05-12 00:15:11.771392 readyapi-0.110.2.dev1/docs_src/query_params_str_validations/tutorial003_py310.py
--rw-r--r--   0        0        0      370 2024-05-12 00:15:11.771392 readyapi-0.110.2.dev1/docs_src/query_params_str_validations/tutorial004.py
--rw-r--r--   0        0        0      413 2024-05-12 00:15:11.771392 readyapi-0.110.2.dev1/docs_src/query_params_str_validations/tutorial004_an.py
--rw-r--r--   0        0        0      371 2024-05-12 00:15:11.771392 readyapi-0.110.2.dev1/docs_src/query_params_str_validations/tutorial004_an_py310.py
--rw-r--r--   0        0        0      369 2024-05-12 00:15:11.771392 readyapi-0.110.2.dev1/docs_src/query_params_str_validations/tutorial004_an_py310_regex.py
--rw-r--r--   0        0        0      384 2024-05-12 00:15:11.771392 readyapi-0.110.2.dev1/docs_src/query_params_str_validations/tutorial004_an_py39.py
--rw-r--r--   0        0        0      338 2024-05-12 00:15:11.771392 readyapi-0.110.2.dev1/docs_src/query_params_str_validations/tutorial004_py310.py
--rw-r--r--   0        0        0      279 2024-05-12 00:15:11.771392 readyapi-0.110.2.dev1/docs_src/query_params_str_validations/tutorial005.py
--rw-r--r--   0        0        0      322 2024-05-12 00:15:11.771392 readyapi-0.110.2.dev1/docs_src/query_params_str_validations/tutorial005_an.py
--rw-r--r--   0        0        0      312 2024-05-12 00:15:11.771392 readyapi-0.110.2.dev1/docs_src/query_params_str_validations/tutorial005_an_py39.py
--rw-r--r--   0        0        0      257 2024-05-12 00:15:11.771392 readyapi-0.110.2.dev1/docs_src/query_params_str_validations/tutorial006.py
--rw-r--r--   0        0        0      307 2024-05-12 00:15:11.771392 readyapi-0.110.2.dev1/docs_src/query_params_str_validations/tutorial006_an.py
--rw-r--r--   0        0        0      297 2024-05-12 00:15:11.771392 readyapi-0.110.2.dev1/docs_src/query_params_str_validations/tutorial006_an_py39.py
--rw-r--r--   0        0        0      270 2024-05-12 00:15:11.771392 readyapi-0.110.2.dev1/docs_src/query_params_str_validations/tutorial006b.py
--rw-r--r--   0        0        0      313 2024-05-12 00:15:11.771392 readyapi-0.110.2.dev1/docs_src/query_params_str_validations/tutorial006b_an.py
--rw-r--r--   0        0        0      303 2024-05-12 00:15:11.771392 readyapi-0.110.2.dev1/docs_src/query_params_str_validations/tutorial006b_an_py39.py
--rw-r--r--   0        0        0      309 2024-05-12 00:15:11.771392 readyapi-0.110.2.dev1/docs_src/query_params_str_validations/tutorial006c.py
--rw-r--r--   0        0        0      352 2024-05-12 00:15:11.771392 readyapi-0.110.2.dev1/docs_src/query_params_str_validations/tutorial006c_an.py
--rw-r--r--   0        0        0      310 2024-05-12 00:15:11.771392 readyapi-0.110.2.dev1/docs_src/query_params_str_validations/tutorial006c_an_py310.py
--rw-r--r--   0        0        0      323 2024-05-12 00:15:11.771392 readyapi-0.110.2.dev1/docs_src/query_params_str_validations/tutorial006c_an_py39.py
--rw-r--r--   0        0        0      277 2024-05-12 00:15:11.771392 readyapi-0.110.2.dev1/docs_src/query_params_str_validations/tutorial006c_py310.py
--rw-r--r--   0        0        0      305 2024-05-12 00:15:11.771392 readyapi-0.110.2.dev1/docs_src/query_params_str_validations/tutorial006d.py
--rw-r--r--   0        0        0      348 2024-05-12 00:15:11.771392 readyapi-0.110.2.dev1/docs_src/query_params_str_validations/tutorial006d_an.py
--rw-r--r--   0        0        0      338 2024-05-12 00:15:11.771392 readyapi-0.110.2.dev1/docs_src/query_params_str_validations/tutorial006d_an_py39.py
--rw-r--r--   0        0        0      339 2024-05-12 00:15:11.771392 readyapi-0.110.2.dev1/docs_src/query_params_str_validations/tutorial007.py
--rw-r--r--   0        0        0      382 2024-05-12 00:15:11.771392 readyapi-0.110.2.dev1/docs_src/query_params_str_validations/tutorial007_an.py
--rw-r--r--   0        0        0      340 2024-05-12 00:15:11.771392 readyapi-0.110.2.dev1/docs_src/query_params_str_validations/tutorial007_an_py310.py
--rw-r--r--   0        0        0      353 2024-05-12 00:15:11.771392 readyapi-0.110.2.dev1/docs_src/query_params_str_validations/tutorial007_an_py39.py
--rw-r--r--   0        0        0      307 2024-05-12 00:15:11.771392 readyapi-0.110.2.dev1/docs_src/query_params_str_validations/tutorial007_py310.py
--rw-r--r--   0        0        0      469 2024-05-12 00:15:11.771392 readyapi-0.110.2.dev1/docs_src/query_params_str_validations/tutorial008.py
--rw-r--r--   0        0        0      543 2024-05-12 00:15:11.771392 readyapi-0.110.2.dev1/docs_src/query_params_str_validations/tutorial008_an.py
--rw-r--r--   0        0        0      501 2024-05-12 00:15:11.771392 readyapi-0.110.2.dev1/docs_src/query_params_str_validations/tutorial008_an_py310.py
--rw-r--r--   0        0        0      514 2024-05-12 00:15:11.771392 readyapi-0.110.2.dev1/docs_src/query_params_str_validations/tutorial008_an_py39.py
--rw-r--r--   0        0        0      437 2024-05-12 00:15:11.771392 readyapi-0.110.2.dev1/docs_src/query_params_str_validations/tutorial008_py310.py
--rw-r--r--   0        0        0      316 2024-05-12 00:15:11.771392 readyapi-0.110.2.dev1/docs_src/query_params_str_validations/tutorial009.py
--rw-r--r--   0        0        0      359 2024-05-12 00:15:11.771392 readyapi-0.110.2.dev1/docs_src/query_params_str_validations/tutorial009_an.py
--rw-r--r--   0        0        0      317 2024-05-12 00:15:11.771392 readyapi-0.110.2.dev1/docs_src/query_params_str_validations/tutorial009_an_py310.py
--rw-r--r--   0        0        0      330 2024-05-12 00:15:11.771392 readyapi-0.110.2.dev1/docs_src/query_params_str_validations/tutorial009_an_py39.py
--rw-r--r--   0        0        0      284 2024-05-12 00:15:11.771392 readyapi-0.110.2.dev1/docs_src/query_params_str_validations/tutorial009_py310.py
--rw-r--r--   0        0        0      577 2024-05-12 00:15:11.771392 readyapi-0.110.2.dev1/docs_src/query_params_str_validations/tutorial010.py
--rw-r--r--   0        0        0      667 2024-05-12 00:15:11.771392 readyapi-0.110.2.dev1/docs_src/query_params_str_validations/tutorial010_an.py
--rw-r--r--   0        0        0      625 2024-05-12 00:15:11.771392 readyapi-0.110.2.dev1/docs_src/query_params_str_validations/tutorial010_an_py310.py
--rw-r--r--   0        0        0      638 2024-05-12 00:15:11.771392 readyapi-0.110.2.dev1/docs_src/query_params_str_validations/tutorial010_an_py39.py
--rw-r--r--   0        0        0      545 2024-05-12 00:15:11.771392 readyapi-0.110.2.dev1/docs_src/query_params_str_validations/tutorial010_py310.py
--rw-r--r--   0        0        0      230 2024-05-12 00:15:11.771392 readyapi-0.110.2.dev1/docs_src/query_params_str_validations/tutorial011.py
--rw-r--r--   0        0        0      275 2024-05-12 00:15:11.771392 readyapi-0.110.2.dev1/docs_src/query_params_str_validations/tutorial011_an.py
--rw-r--r--   0        0        0      227 2024-05-12 00:15:11.771392 readyapi-0.110.2.dev1/docs_src/query_params_str_validations/tutorial011_an_py310.py
--rw-r--r--   0        0        0      240 2024-05-12 00:15:11.771392 readyapi-0.110.2.dev1/docs_src/query_params_str_validations/tutorial011_an_py39.py
--rw-r--r--   0        0        0      192 2024-05-12 00:15:11.771392 readyapi-0.110.2.dev1/docs_src/query_params_str_validations/tutorial011_py310.py
--rw-r--r--   0        0        0      224 2024-05-12 00:15:11.771392 readyapi-0.110.2.dev1/docs_src/query_params_str_validations/tutorial011_py39.py
--rw-r--r--   0        0        0      220 2024-05-12 00:15:11.771392 readyapi-0.110.2.dev1/docs_src/query_params_str_validations/tutorial012.py
--rw-r--r--   0        0        0      265 2024-05-12 00:15:11.771392 readyapi-0.110.2.dev1/docs_src/query_params_str_validations/tutorial012_an.py
--rw-r--r--   0        0        0      230 2024-05-12 00:15:11.771392 readyapi-0.110.2.dev1/docs_src/query_params_str_validations/tutorial012_an_py39.py
--rw-r--r--   0        0        0      195 2024-05-12 00:15:11.771392 readyapi-0.110.2.dev1/docs_src/query_params_str_validations/tutorial012_py39.py
--rw-r--r--   0        0        0      178 2024-05-12 00:15:11.771392 readyapi-0.110.2.dev1/docs_src/query_params_str_validations/tutorial013.py
--rw-r--r--   0        0        0      223 2024-05-12 00:15:11.771392 readyapi-0.110.2.dev1/docs_src/query_params_str_validations/tutorial013_an.py
--rw-r--r--   0        0        0      213 2024-05-12 00:15:11.771392 readyapi-0.110.2.dev1/docs_src/query_params_str_validations/tutorial013_an_py39.py
--rw-r--r--   0        0        0      333 2024-05-12 00:15:11.771392 readyapi-0.110.2.dev1/docs_src/query_params_str_validations/tutorial014.py
--rw-r--r--   0        0        0      376 2024-05-12 00:15:11.771392 readyapi-0.110.2.dev1/docs_src/query_params_str_validations/tutorial014_an.py
--rw-r--r--   0        0        0      334 2024-05-12 00:15:11.771392 readyapi-0.110.2.dev1/docs_src/query_params_str_validations/tutorial014_an_py310.py
--rw-r--r--   0        0        0      347 2024-05-12 00:15:11.771392 readyapi-0.110.2.dev1/docs_src/query_params_str_validations/tutorial014_an_py39.py
--rw-r--r--   0        0        0      301 2024-05-12 00:15:11.771392 readyapi-0.110.2.dev1/docs_src/query_params_str_validations/tutorial014_py310.py
--rw-r--r--   0        0        0      285 2024-05-12 00:15:11.771392 readyapi-0.110.2.dev1/docs_src/request_files/tutorial001.py
--rw-r--r--   0        0        0      511 2024-05-12 00:15:11.771392 readyapi-0.110.2.dev1/docs_src/request_files/tutorial001_02.py
--rw-r--r--   0        0        0      556 2024-05-12 00:15:11.771392 readyapi-0.110.2.dev1/docs_src/request_files/tutorial001_02_an.py
--rw-r--r--   0        0        0      508 2024-05-12 00:15:11.771392 readyapi-0.110.2.dev1/docs_src/request_files/tutorial001_02_an_py310.py
--rw-r--r--   0        0        0      527 2024-05-12 00:15:11.771392 readyapi-0.110.2.dev1/docs_src/request_files/tutorial001_02_an_py39.py
--rw-r--r--   0        0        0      473 2024-05-12 00:15:11.771392 readyapi-0.110.2.dev1/docs_src/request_files/tutorial001_02_py310.py
--rw-r--r--   0        0        0      374 2024-05-12 00:15:11.771392 readyapi-0.110.2.dev1/docs_src/request_files/tutorial001_03.py
--rw-r--r--   0        0        0      434 2024-05-12 00:15:11.771392 readyapi-0.110.2.dev1/docs_src/request_files/tutorial001_03_an.py
--rw-r--r--   0        0        0      424 2024-05-12 00:15:11.771392 readyapi-0.110.2.dev1/docs_src/request_files/tutorial001_03_an_py39.py
--rw-r--r--   0        0        0      335 2024-05-12 00:15:11.771392 readyapi-0.110.2.dev1/docs_src/request_files/tutorial001_an.py
--rw-r--r--   0        0        0      325 2024-05-12 00:15:11.771392 readyapi-0.110.2.dev1/docs_src/request_files/tutorial001_an_py39.py
--rw-r--r--   0        0        0      815 2024-05-12 00:15:11.771392 readyapi-0.110.2.dev1/docs_src/request_files/tutorial002.py
--rw-r--r--   0        0        0      865 2024-05-12 00:15:11.771392 readyapi-0.110.2.dev1/docs_src/request_files/tutorial002_an.py
--rw-r--r--   0        0        0      830 2024-05-12 00:15:11.771392 readyapi-0.110.2.dev1/docs_src/request_files/tutorial002_an_py39.py
--rw-r--r--   0        0        0      790 2024-05-12 00:15:11.771392 readyapi-0.110.2.dev1/docs_src/request_files/tutorial002_py39.py
--rw-r--r--   0        0        0      917 2024-05-12 00:15:11.771392 readyapi-0.110.2.dev1/docs_src/request_files/tutorial003.py
--rw-r--r--   0        0        0      991 2024-05-12 00:15:11.771392 readyapi-0.110.2.dev1/docs_src/request_files/tutorial003_an.py
--rw-r--r--   0        0        0      956 2024-05-12 00:15:11.771392 readyapi-0.110.2.dev1/docs_src/request_files/tutorial003_an_py39.py
--rw-r--r--   0        0        0      892 2024-05-12 00:15:11.771392 readyapi-0.110.2.dev1/docs_src/request_files/tutorial003_py39.py
--rw-r--r--   0        0        0      176 2024-05-12 00:15:11.771392 readyapi-0.110.2.dev1/docs_src/request_forms/tutorial001.py
--rw-r--r--   0        0        0      236 2024-05-12 00:15:11.771392 readyapi-0.110.2.dev1/docs_src/request_forms/tutorial001_an.py
--rw-r--r--   0        0        0      226 2024-05-12 00:15:11.771392 readyapi-0.110.2.dev1/docs_src/request_forms/tutorial001_an_py39.py
--rw-r--r--   0        0        0      320 2024-05-12 00:15:11.771392 readyapi-0.110.2.dev1/docs_src/request_forms_and_files/tutorial001.py
--rw-r--r--   0        0        0      399 2024-05-12 00:15:11.771392 readyapi-0.110.2.dev1/docs_src/request_forms_and_files/tutorial001_an.py
--rw-r--r--   0        0        0      389 2024-05-12 00:15:11.771392 readyapi-0.110.2.dev1/docs_src/request_forms_and_files/tutorial001_an_py39.py
--rw-r--r--   0        0        0      394 2024-05-12 00:15:11.771392 readyapi-0.110.2.dev1/docs_src/response_change_status_code/tutorial001.py
--rw-r--r--   0        0        0      348 2024-05-12 00:15:11.771392 readyapi-0.110.2.dev1/docs_src/response_cookies/tutorial001.py
--rw-r--r--   0        0        0      275 2024-05-12 00:15:11.771392 readyapi-0.110.2.dev1/docs_src/response_cookies/tutorial002.py
--rw-r--r--   0        0        0      510 2024-05-12 00:15:11.771392 readyapi-0.110.2.dev1/docs_src/response_directly/tutorial001.py
--rw-r--r--   0        0        0      357 2024-05-12 00:15:11.771392 readyapi-0.110.2.dev1/docs_src/response_directly/tutorial002.py
--rw-r--r--   0        0        0      313 2024-05-12 00:15:11.771392 readyapi-0.110.2.dev1/docs_src/response_headers/tutorial001.py
--rw-r--r--   0        0        0      225 2024-05-12 00:15:11.771392 readyapi-0.110.2.dev1/docs_src/response_headers/tutorial002.py
--rw-r--r--   0        0        0      565 2024-05-12 00:15:11.771392 readyapi-0.110.2.dev1/docs_src/response_model/tutorial001.py
--rw-r--r--   0        0        0      516 2024-05-12 00:15:11.771392 readyapi-0.110.2.dev1/docs_src/response_model/tutorial001_01.py
--rw-r--r--   0        0        0      472 2024-05-12 00:15:11.775392 readyapi-0.110.2.dev1/docs_src/response_model/tutorial001_01_py310.py
--rw-r--r--   0        0        0      510 2024-05-12 00:15:11.775392 readyapi-0.110.2.dev1/docs_src/response_model/tutorial001_01_py39.py
--rw-r--r--   0        0        0      540 2024-05-12 00:15:11.775392 readyapi-0.110.2.dev1/docs_src/response_model/tutorial001_py310.py
--rw-r--r--   0        0        0      559 2024-05-12 00:15:11.775392 readyapi-0.110.2.dev1/docs_src/response_model/tutorial001_py39.py
--rw-r--r--   0        0        0      353 2024-05-12 00:15:11.775392 readyapi-0.110.2.dev1/docs_src/response_model/tutorial002.py
--rw-r--r--   0        0        0      321 2024-05-12 00:15:11.775392 readyapi-0.110.2.dev1/docs_src/response_model/tutorial002_py310.py
--rw-r--r--   0        0        0      453 2024-05-12 00:15:11.775392 readyapi-0.110.2.dev1/docs_src/response_model/tutorial003.py
--rw-r--r--   0        0        0      352 2024-05-12 00:15:11.775392 readyapi-0.110.2.dev1/docs_src/response_model/tutorial003_01.py
--rw-r--r--   0        0        0      320 2024-05-12 00:15:11.775392 readyapi-0.110.2.dev1/docs_src/response_model/tutorial003_01_py310.py
--rw-r--r--   0        0        0      385 2024-05-12 00:15:11.775392 readyapi-0.110.2.dev1/docs_src/response_model/tutorial003_02.py
--rw-r--r--   0        0        0      245 2024-05-12 00:15:11.775392 readyapi-0.110.2.dev1/docs_src/response_model/tutorial003_03.py
--rw-r--r--   0        0        0      388 2024-05-12 00:15:11.775392 readyapi-0.110.2.dev1/docs_src/response_model/tutorial003_04.py
--rw-r--r--   0        0        0      356 2024-05-12 00:15:11.775392 readyapi-0.110.2.dev1/docs_src/response_model/tutorial003_04_py310.py
--rw-r--r--   0        0        0      409 2024-05-12 00:15:11.775392 readyapi-0.110.2.dev1/docs_src/response_model/tutorial003_05.py
--rw-r--r--   0        0        0      377 2024-05-12 00:15:11.775392 readyapi-0.110.2.dev1/docs_src/response_model/tutorial003_05_py310.py
--rw-r--r--   0        0        0      434 2024-05-12 00:15:11.775392 readyapi-0.110.2.dev1/docs_src/response_model/tutorial003_py310.py
--rw-r--r--   0        0        0      636 2024-05-12 00:15:11.775392 readyapi-0.110.2.dev1/docs_src/response_model/tutorial004.py
--rw-r--r--   0        0        0      598 2024-05-12 00:15:11.775392 readyapi-0.110.2.dev1/docs_src/response_model/tutorial004_py310.py
--rw-r--r--   0        0        0      630 2024-05-12 00:15:11.775392 readyapi-0.110.2.dev1/docs_src/response_model/tutorial004_py39.py
--rw-r--r--   0        0        0      851 2024-05-12 00:15:11.775392 readyapi-0.110.2.dev1/docs_src/response_model/tutorial005.py
--rw-r--r--   0        0        0      819 2024-05-12 00:15:11.775392 readyapi-0.110.2.dev1/docs_src/response_model/tutorial005_py310.py
--rw-r--r--   0        0        0      851 2024-05-12 00:15:11.775392 readyapi-0.110.2.dev1/docs_src/response_model/tutorial006.py
--rw-r--r--   0        0        0      819 2024-05-12 00:15:11.775392 readyapi-0.110.2.dev1/docs_src/response_model/tutorial006_py310.py
--rw-r--r--   0        0        0      148 2024-05-12 00:15:11.775392 readyapi-0.110.2.dev1/docs_src/response_status_code/tutorial001.py
--rw-r--r--   0        0        0      176 2024-05-12 00:15:11.775392 readyapi-0.110.2.dev1/docs_src/response_status_code/tutorial002.py
--rw-r--r--   0        0        0      687 2024-05-12 00:15:11.775392 readyapi-0.110.2.dev1/docs_src/schema_extra_example/tutorial001.py
--rw-r--r--   0        0        0      672 2024-05-12 00:15:11.775392 readyapi-0.110.2.dev1/docs_src/schema_extra_example/tutorial001_pv1.py
--rw-r--r--   0        0        0      649 2024-05-12 00:15:11.775392 readyapi-0.110.2.dev1/docs_src/schema_extra_example/tutorial001_py310.py
--rw-r--r--   0        0        0      634 2024-05-12 00:15:11.775392 readyapi-0.110.2.dev1/docs_src/schema_extra_example/tutorial001_py310_pv1.py
--rw-r--r--   0        0        0      520 2024-05-12 00:15:11.775392 readyapi-0.110.2.dev1/docs_src/schema_extra_example/tutorial002.py
--rw-r--r--   0        0        0      482 2024-05-12 00:15:11.775392 readyapi-0.110.2.dev1/docs_src/schema_extra_example/tutorial002_py310.py
--rw-r--r--   0        0        0      615 2024-05-12 00:15:11.775392 readyapi-0.110.2.dev1/docs_src/schema_extra_example/tutorial003.py
--rw-r--r--   0        0        0      724 2024-05-12 00:15:11.775392 readyapi-0.110.2.dev1/docs_src/schema_extra_example/tutorial003_an.py
--rw-r--r--   0        0        0      676 2024-05-12 00:15:11.775392 readyapi-0.110.2.dev1/docs_src/schema_extra_example/tutorial003_an_py310.py
--rw-r--r--   0        0        0      695 2024-05-12 00:15:11.775392 readyapi-0.110.2.dev1/docs_src/schema_extra_example/tutorial003_an_py39.py
--rw-r--r--   0        0        0      577 2024-05-12 00:15:11.775392 readyapi-0.110.2.dev1/docs_src/schema_extra_example/tutorial003_py310.py
--rw-r--r--   0        0        0      827 2024-05-12 00:15:11.775392 readyapi-0.110.2.dev1/docs_src/schema_extra_example/tutorial004.py
--rw-r--r--   0        0        0      968 2024-05-12 00:15:11.775392 readyapi-0.110.2.dev1/docs_src/schema_extra_example/tutorial004_an.py
--rw-r--r--   0        0        0      920 2024-05-12 00:15:11.775392 readyapi-0.110.2.dev1/docs_src/schema_extra_example/tutorial004_an_py310.py
--rw-r--r--   0        0        0      939 2024-05-12 00:15:11.775392 readyapi-0.110.2.dev1/docs_src/schema_extra_example/tutorial004_an_py39.py
--rw-r--r--   0        0        0      789 2024-05-12 00:15:11.775392 readyapi-0.110.2.dev1/docs_src/schema_extra_example/tutorial004_py310.py
--rw-r--r--   0        0        0     1390 2024-05-12 00:15:11.775392 readyapi-0.110.2.dev1/docs_src/schema_extra_example/tutorial005.py
--rw-r--r--   0        0        0     1575 2024-05-12 00:15:11.775392 readyapi-0.110.2.dev1/docs_src/schema_extra_example/tutorial005_an.py
--rw-r--r--   0        0        0     1527 2024-05-12 00:15:11.775392 readyapi-0.110.2.dev1/docs_src/schema_extra_example/tutorial005_an_py310.py
--rw-r--r--   0        0        0     1546 2024-05-12 00:15:11.775392 readyapi-0.110.2.dev1/docs_src/schema_extra_example/tutorial005_an_py39.py
--rw-r--r--   0        0        0     1352 2024-05-12 00:15:11.775392 readyapi-0.110.2.dev1/docs_src/schema_extra_example/tutorial005_py310.py
--rw-r--r--   0        0        0      273 2024-05-12 00:15:11.775392 readyapi-0.110.2.dev1/docs_src/security/tutorial001.py
--rw-r--r--   0        0        0      323 2024-05-12 00:15:11.775392 readyapi-0.110.2.dev1/docs_src/security/tutorial001_an.py
--rw-r--r--   0        0        0      313 2024-05-12 00:15:11.775392 readyapi-0.110.2.dev1/docs_src/security/tutorial001_an_py39.py
--rw-r--r--   0        0        0      759 2024-05-12 00:15:11.775392 readyapi-0.110.2.dev1/docs_src/security/tutorial002.py
--rw-r--r--   0        0        0      819 2024-05-12 00:15:11.775392 readyapi-0.110.2.dev1/docs_src/security/tutorial002_an.py
--rw-r--r--   0        0        0      765 2024-05-12 00:15:11.775392 readyapi-0.110.2.dev1/docs_src/security/tutorial002_an_py310.py
--rw-r--r--   0        0        0      790 2024-05-12 00:15:11.775392 readyapi-0.110.2.dev1/docs_src/security/tutorial002_an_py39.py
--rw-r--r--   0        0        0      715 2024-05-12 00:15:11.775392 readyapi-0.110.2.dev1/docs_src/security/tutorial002_py310.py
--rw-r--r--   0        0        0     2498 2024-05-12 00:15:11.775392 readyapi-0.110.2.dev1/docs_src/security/tutorial003.py
--rw-r--r--   0        0        0     2592 2024-05-12 00:15:11.775392 readyapi-0.110.2.dev1/docs_src/security/tutorial003_an.py
--rw-r--r--   0        0        0     2538 2024-05-12 00:15:11.775392 readyapi-0.110.2.dev1/docs_src/security/tutorial003_an_py310.py
--rw-r--r--   0        0        0     2563 2024-05-12 00:15:11.775392 readyapi-0.110.2.dev1/docs_src/security/tutorial003_an_py39.py
--rw-r--r--   0        0        0     2454 2024-05-12 00:15:11.775392 readyapi-0.110.2.dev1/docs_src/security/tutorial003_py310.py
--rw-r--r--   0        0        0     4138 2024-05-12 00:15:11.775392 readyapi-0.110.2.dev1/docs_src/security/tutorial004.py
--rw-r--r--   0        0        0     4249 2024-05-12 00:15:11.775392 readyapi-0.110.2.dev1/docs_src/security/tutorial004_an.py
--rw-r--r--   0        0        0     4183 2024-05-12 00:15:11.775392 readyapi-0.110.2.dev1/docs_src/security/tutorial004_an_py310.py
--rw-r--r--   0        0        0     4220 2024-05-12 00:15:11.775392 readyapi-0.110.2.dev1/docs_src/security/tutorial004_an_py39.py
--rw-r--r--   0        0        0     4083 2024-05-12 00:15:11.775392 readyapi-0.110.2.dev1/docs_src/security/tutorial004_py310.py
--rw-r--r--   0        0        0     5274 2024-05-12 00:15:11.775392 readyapi-0.110.2.dev1/docs_src/security/tutorial005.py
--rw-r--r--   0        0        0     5381 2024-05-12 00:15:11.775392 readyapi-0.110.2.dev1/docs_src/security/tutorial005_an.py
--rw-r--r--   0        0        0     5309 2024-05-12 00:15:11.775392 readyapi-0.110.2.dev1/docs_src/security/tutorial005_an_py310.py
--rw-r--r--   0        0        0     5352 2024-05-12 00:15:11.775392 readyapi-0.110.2.dev1/docs_src/security/tutorial005_an_py39.py
--rw-r--r--   0        0        0     5213 2024-05-12 00:15:11.775392 readyapi-0.110.2.dev1/docs_src/security/tutorial005_py310.py
--rw-r--r--   0        0        0     5268 2024-05-12 00:15:11.775392 readyapi-0.110.2.dev1/docs_src/security/tutorial005_py39.py
--rw-r--r--   0        0        0      325 2024-05-12 00:15:11.775392 readyapi-0.110.2.dev1/docs_src/security/tutorial006.py
--rw-r--r--   0        0        0      375 2024-05-12 00:15:11.775392 readyapi-0.110.2.dev1/docs_src/security/tutorial006_an.py
--rw-r--r--   0        0        0      365 2024-05-12 00:15:11.775392 readyapi-0.110.2.dev1/docs_src/security/tutorial006_an_py39.py
--rw-r--r--   0        0        0     1120 2024-05-12 00:15:11.775392 readyapi-0.110.2.dev1/docs_src/security/tutorial007.py
--rw-r--r--   0        0        0     1187 2024-05-12 00:15:11.775392 readyapi-0.110.2.dev1/docs_src/security/tutorial007_an.py
--rw-r--r--   0        0        0     1176 2024-05-12 00:15:11.775392 readyapi-0.110.2.dev1/docs_src/security/tutorial007_an_py39.py
--rw-r--r--   0        0        0      492 2024-05-12 00:15:11.775392 readyapi-0.110.2.dev1/docs_src/separate_openapi_schemas/tutorial001.py
--rw-r--r--   0        0        0      454 2024-05-12 00:15:11.775392 readyapi-0.110.2.dev1/docs_src/separate_openapi_schemas/tutorial001_py310.py
--rw-r--r--   0        0        0      486 2024-05-12 00:15:11.775392 readyapi-0.110.2.dev1/docs_src/separate_openapi_schemas/tutorial001_py39.py
--rw-r--r--   0        0        0      527 2024-05-12 00:15:11.775392 readyapi-0.110.2.dev1/docs_src/separate_openapi_schemas/tutorial002.py
--rw-r--r--   0        0        0      489 2024-05-12 00:15:11.775392 readyapi-0.110.2.dev1/docs_src/separate_openapi_schemas/tutorial002_py310.py
--rw-r--r--   0        0        0      521 2024-05-12 00:15:11.775392 readyapi-0.110.2.dev1/docs_src/separate_openapi_schemas/tutorial002_py39.py
--rw-r--r--   0        0        0        0 2024-05-12 00:15:11.775392 readyapi-0.110.2.dev1/docs_src/settings/app01/__init__.py
--rw-r--r--   0        0        0      183 2024-05-12 00:15:11.775392 readyapi-0.110.2.dev1/docs_src/settings/app01/config.py
--rw-r--r--   0        0        0      270 2024-05-12 00:15:11.775392 readyapi-0.110.2.dev1/docs_src/settings/app01/main.py
--rw-r--r--   0        0        0        0 2024-05-12 00:15:11.775392 readyapi-0.110.2.dev1/docs_src/settings/app02/__init__.py
--rw-r--r--   0        0        0      159 2024-05-12 00:15:11.775392 readyapi-0.110.2.dev1/docs_src/settings/app02/config.py
--rw-r--r--   0        0        0      409 2024-05-12 00:15:11.775392 readyapi-0.110.2.dev1/docs_src/settings/app02/main.py
--rw-r--r--   0        0        0      516 2024-05-12 00:15:11.775392 readyapi-0.110.2.dev1/docs_src/settings/app02/test_main.py
--rw-r--r--   0        0        0        0 2024-05-12 00:15:11.775392 readyapi-0.110.2.dev1/docs_src/settings/app02_an/__init__.py
--rw-r--r--   0        0        0      159 2024-05-12 00:15:11.775392 readyapi-0.110.2.dev1/docs_src/settings/app02_an/config.py
--rw-r--r--   0        0        0      459 2024-05-12 00:15:11.775392 readyapi-0.110.2.dev1/docs_src/settings/app02_an/main.py
--rw-r--r--   0        0        0      516 2024-05-12 00:15:11.775392 readyapi-0.110.2.dev1/docs_src/settings/app02_an/test_main.py
--rw-r--r--   0        0        0        0 2024-05-12 00:15:11.775392 readyapi-0.110.2.dev1/docs_src/settings/app02_an_py39/__init__.py
--rw-r--r--   0        0        0      159 2024-05-12 00:15:11.775392 readyapi-0.110.2.dev1/docs_src/settings/app02_an_py39/config.py
--rw-r--r--   0        0        0      448 2024-05-12 00:15:11.775392 readyapi-0.110.2.dev1/docs_src/settings/app02_an_py39/main.py
--rw-r--r--   0        0        0      516 2024-05-12 00:15:11.775392 readyapi-0.110.2.dev1/docs_src/settings/app02_an_py39/test_main.py
--rw-r--r--   0        0        0        0 2024-05-12 00:15:11.775392 readyapi-0.110.2.dev1/docs_src/settings/app03/__init__.py
--rw-r--r--   0        0        0      204 2024-05-12 00:15:11.775392 readyapi-0.110.2.dev1/docs_src/settings/app03/config.py
--rw-r--r--   0        0        0      415 2024-05-12 00:15:11.775392 readyapi-0.110.2.dev1/docs_src/settings/app03/main.py
--rw-r--r--   0        0        0        0 2024-05-12 00:15:11.775392 readyapi-0.110.2.dev1/docs_src/settings/app03_an/__init__.py
--rw-r--r--   0        0        0      235 2024-05-12 00:15:11.775392 readyapi-0.110.2.dev1/docs_src/settings/app03_an/config.py
--rw-r--r--   0        0        0      195 2024-05-12 00:15:11.775392 readyapi-0.110.2.dev1/docs_src/settings/app03_an/config_pv1.py
--rw-r--r--   0        0        0      454 2024-05-12 00:15:11.775392 readyapi-0.110.2.dev1/docs_src/settings/app03_an/main.py
--rw-r--r--   0        0        0        0 2024-05-12 00:15:11.775392 readyapi-0.110.2.dev1/docs_src/settings/app03_an_py39/__init__.py
--rw-r--r--   0        0        0      204 2024-05-12 00:15:11.775392 readyapi-0.110.2.dev1/docs_src/settings/app03_an_py39/config.py
--rw-r--r--   0        0        0      465 2024-05-12 00:15:11.779392 readyapi-0.110.2.dev1/docs_src/settings/app03_an_py39/main.py
--rw-r--r--   0        0        0      422 2024-05-12 00:15:11.779392 readyapi-0.110.2.dev1/docs_src/settings/tutorial001.py
--rw-r--r--   0        0        0      413 2024-05-12 00:15:11.779392 readyapi-0.110.2.dev1/docs_src/settings/tutorial001_pv1.py
--rw-r--r--   0        0        0        0 2024-05-12 00:15:11.779392 readyapi-0.110.2.dev1/docs_src/sql_databases/__init__.py
--rw-r--r--   0        0        0        0 2024-05-12 00:15:11.779392 readyapi-0.110.2.dev1/docs_src/sql_databases/sql_app/__init__.py
--rw-r--r--   0        0        0     1931 2024-05-12 00:15:11.779392 readyapi-0.110.2.dev1/docs_src/sql_databases/sql_app/alt_main.py
--rw-r--r--   0        0        0     1061 2024-05-12 00:15:11.779392 readyapi-0.110.2.dev1/docs_src/sql_databases/sql_app/crud.py
--rw-r--r--   0        0        0      461 2024-05-12 00:15:11.779392 readyapi-0.110.2.dev1/docs_src/sql_databases/sql_app/database.py
--rw-r--r--   0        0        0     1635 2024-05-12 00:15:11.779392 readyapi-0.110.2.dev1/docs_src/sql_databases/sql_app/main.py
--rw-r--r--   0        0        0      710 2024-05-12 00:15:11.779392 readyapi-0.110.2.dev1/docs_src/sql_databases/sql_app/models.py
--rw-r--r--   0        0        0      502 2024-05-12 00:15:11.779392 readyapi-0.110.2.dev1/docs_src/sql_databases/sql_app/schemas.py
--rw-r--r--   0        0        0        0 2024-05-12 00:15:11.779392 readyapi-0.110.2.dev1/docs_src/sql_databases/sql_app/tests/__init__.py
--rw-r--r--   0        0        0     1261 2024-05-12 00:15:11.779392 readyapi-0.110.2.dev1/docs_src/sql_databases/sql_app/tests/test_sql_app.py
--rw-r--r--   0        0        0        0 2024-05-12 00:15:11.779392 readyapi-0.110.2.dev1/docs_src/sql_databases/sql_app_py310/__init__.py
--rw-r--r--   0        0        0     1906 2024-05-12 00:15:11.779392 readyapi-0.110.2.dev1/docs_src/sql_databases/sql_app_py310/alt_main.py
--rw-r--r--   0        0        0     1061 2024-05-12 00:15:11.779392 readyapi-0.110.2.dev1/docs_src/sql_databases/sql_app_py310/crud.py
--rw-r--r--   0        0        0      461 2024-05-12 00:15:11.779392 readyapi-0.110.2.dev1/docs_src/sql_databases/sql_app_py310/database.py
--rw-r--r--   0        0        0     1610 2024-05-12 00:15:11.779392 readyapi-0.110.2.dev1/docs_src/sql_databases/sql_app_py310/main.py
--rw-r--r--   0        0        0      710 2024-05-12 00:15:11.779392 readyapi-0.110.2.dev1/docs_src/sql_databases/sql_app_py310/models.py
--rw-r--r--   0        0        0      464 2024-05-12 00:15:11.779392 readyapi-0.110.2.dev1/docs_src/sql_databases/sql_app_py310/schemas.py
--rw-r--r--   0        0        0        0 2024-05-12 00:15:11.779392 readyapi-0.110.2.dev1/docs_src/sql_databases/sql_app_py310/tests/__init__.py
--rw-r--r--   0        0        0     1201 2024-05-12 00:15:11.779392 readyapi-0.110.2.dev1/docs_src/sql_databases/sql_app_py310/tests/test_sql_app.py
--rw-r--r--   0        0        0        0 2024-05-12 00:15:11.779392 readyapi-0.110.2.dev1/docs_src/sql_databases/sql_app_py39/__init__.py
--rw-r--r--   0        0        0     1906 2024-05-12 00:15:11.779392 readyapi-0.110.2.dev1/docs_src/sql_databases/sql_app_py39/alt_main.py
--rw-r--r--   0        0        0     1061 2024-05-12 00:15:11.779392 readyapi-0.110.2.dev1/docs_src/sql_databases/sql_app_py39/crud.py
--rw-r--r--   0        0        0      461 2024-05-12 00:15:11.779392 readyapi-0.110.2.dev1/docs_src/sql_databases/sql_app_py39/database.py
--rw-r--r--   0        0        0     1610 2024-05-12 00:15:11.779392 readyapi-0.110.2.dev1/docs_src/sql_databases/sql_app_py39/main.py
--rw-r--r--   0        0        0      710 2024-05-12 00:15:11.779392 readyapi-0.110.2.dev1/docs_src/sql_databases/sql_app_py39/models.py
--rw-r--r--   0        0        0      496 2024-05-12 00:15:11.779392 readyapi-0.110.2.dev1/docs_src/sql_databases/sql_app_py39/schemas.py
--rw-r--r--   0        0        0        0 2024-05-12 00:15:11.779392 readyapi-0.110.2.dev1/docs_src/sql_databases/sql_app_py39/tests/__init__.py
--rw-r--r--   0        0        0     1201 2024-05-12 00:15:11.779392 readyapi-0.110.2.dev1/docs_src/sql_databases/sql_app_py39/tests/test_sql_app.py
--rw-r--r--   0        0        0        0 2024-05-12 00:15:11.779392 readyapi-0.110.2.dev1/docs_src/sql_databases_peewee/sql_app/__init__.py
--rw-r--r--   0        0        0      843 2024-05-12 00:15:11.779392 readyapi-0.110.2.dev1/docs_src/sql_databases_peewee/sql_app/crud.py
--rw-r--r--   0        0        0      662 2024-05-12 00:15:11.779392 readyapi-0.110.2.dev1/docs_src/sql_databases_peewee/sql_app/database.py
--rw-r--r--   0        0        0     2213 2024-05-12 00:15:11.779392 readyapi-0.110.2.dev1/docs_src/sql_databases_peewee/sql_app/main.py
--rw-r--r--   0        0        0      465 2024-05-12 00:15:11.779392 readyapi-0.110.2.dev1/docs_src/sql_databases_peewee/sql_app/models.py
--rw-r--r--   0        0        0      868 2024-05-12 00:15:11.779392 readyapi-0.110.2.dev1/docs_src/sql_databases_peewee/sql_app/schemas.py
--rw-r--r--   0        0        0      163 2024-05-12 00:15:11.779392 readyapi-0.110.2.dev1/docs_src/static_files/tutorial001.py
--rw-r--r--   0        0        0      278 2024-05-12 00:15:11.779392 readyapi-0.110.2.dev1/docs_src/sub_applications/tutorial001.py
--rw-r--r--   0        0        0       25 2024-05-12 00:15:11.779392 readyapi-0.110.2.dev1/docs_src/templates/static/styles.css
--rw-r--r--   0        0        0      235 2024-05-12 00:15:11.779392 readyapi-0.110.2.dev1/docs_src/templates/templates/item.html
--rw-r--r--   0        0        0      527 2024-05-12 00:15:11.779392 readyapi-0.110.2.dev1/docs_src/templates/tutorial001.py
--rw-r--r--   0        0        0      233 2024-05-12 00:15:11.779392 readyapi-0.110.2.dev1/docs_src/using_request_directly/tutorial001.py
--rw-r--r--   0        0        0        0 2024-05-12 00:15:11.779392 readyapi-0.110.2.dev1/docs_src/websockets/__init__.py
--rw-r--r--   0        0        0     1436 2024-05-12 00:15:11.779392 readyapi-0.110.2.dev1/docs_src/websockets/tutorial001.py
--rw-r--r--   0        0        0     2846 2024-05-12 00:15:11.779392 readyapi-0.110.2.dev1/docs_src/websockets/tutorial002.py
--rw-r--r--   0        0        0     2913 2024-05-12 00:15:11.779392 readyapi-0.110.2.dev1/docs_src/websockets/tutorial002_an.py
--rw-r--r--   0        0        0     2859 2024-05-12 00:15:11.779392 readyapi-0.110.2.dev1/docs_src/websockets/tutorial002_an_py310.py
--rw-r--r--   0        0        0     2884 2024-05-12 00:15:11.779392 readyapi-0.110.2.dev1/docs_src/websockets/tutorial002_an_py39.py
--rw-r--r--   0        0        0     2802 2024-05-12 00:15:11.779392 readyapi-0.110.2.dev1/docs_src/websockets/tutorial002_py310.py
--rw-r--r--   0        0        0     2578 2024-05-12 00:15:11.779392 readyapi-0.110.2.dev1/docs_src/websockets/tutorial003.py
--rw-r--r--   0        0        0     2553 2024-05-12 00:15:11.779392 readyapi-0.110.2.dev1/docs_src/websockets/tutorial003_py39.py
--rw-r--r--   0        0        0      447 2024-05-12 00:15:11.779392 readyapi-0.110.2.dev1/docs_src/wsgi/tutorial001.py
--rw-r--r--   0        0        0     1731 2024-05-12 00:15:11.779392 readyapi-0.110.2.dev1/pdm_build.py
--rw-r--r--   0        0        0     7283 2024-05-12 00:15:14.731375 readyapi-0.110.2.dev1/pyproject.toml
--rw-r--r--   0        0        0     1089 2024-05-12 00:15:11.779392 readyapi-0.110.2.dev1/readyapi/__init__.py
--rw-r--r--   0        0        0    23139 2024-05-12 00:15:11.779392 readyapi-0.110.2.dev1/readyapi/_compat.py
--rw-r--r--   0        0        0   177259 2024-05-12 00:15:11.779392 readyapi-0.110.2.dev1/readyapi/applications.py
--rw-r--r--   0        0        0     1779 2024-05-12 00:15:11.779392 readyapi-0.110.2.dev1/readyapi/background.py
--rw-r--r--   0        0        0     1403 2024-05-12 00:15:11.779392 readyapi-0.110.2.dev1/readyapi/concurrency.py
--rw-r--r--   0        0        0     5774 2024-05-12 00:15:11.779392 readyapi-0.110.2.dev1/readyapi/datastructures.py
--rw-r--r--   0        0        0        0 2024-05-12 00:15:11.779392 readyapi-0.110.2.dev1/readyapi/dependencies/__init__.py
--rw-r--r--   0        0        0     2496 2024-05-12 00:15:11.779392 readyapi-0.110.2.dev1/readyapi/dependencies/models.py
--rw-r--r--   0        0        0    30266 2024-05-12 00:15:11.779392 readyapi-0.110.2.dev1/readyapi/dependencies/utils.py
--rw-r--r--   0        0        0    11074 2024-05-12 00:15:11.779392 readyapi-0.110.2.dev1/readyapi/encoders.py
--rw-r--r--   0        0        0     1336 2024-05-12 00:15:11.779392 readyapi-0.110.2.dev1/readyapi/exception_handlers.py
--rw-r--r--   0        0        0     4985 2024-05-12 00:15:11.779392 readyapi-0.110.2.dev1/readyapi/exceptions.py
--rw-r--r--   0        0        0       55 2024-05-12 00:15:11.779392 readyapi-0.110.2.dev1/readyapi/logger.py
--rw-r--r--   0        0        0       58 2024-05-12 00:15:11.779392 readyapi-0.110.2.dev1/readyapi/middleware/__init__.py
--rw-r--r--   0        0        0       79 2024-05-12 00:15:11.779392 readyapi-0.110.2.dev1/readyapi/middleware/cors.py
--rw-r--r--   0        0        0       79 2024-05-12 00:15:11.779392 readyapi-0.110.2.dev1/readyapi/middleware/gzip.py
--rw-r--r--   0        0        0      115 2024-05-12 00:15:11.779392 readyapi-0.110.2.dev1/readyapi/middleware/httpsredirect.py
--rw-r--r--   0        0        0      109 2024-05-12 00:15:11.779392 readyapi-0.110.2.dev1/readyapi/middleware/trustedhost.py
--rw-r--r--   0        0        0       79 2024-05-12 00:15:11.779392 readyapi-0.110.2.dev1/readyapi/middleware/wsgi.py
--rw-r--r--   0        0        0        0 2024-05-12 00:15:11.779392 readyapi-0.110.2.dev1/readyapi/openapi/__init__.py
--rw-r--r--   0        0        0      153 2024-05-12 00:15:11.779392 readyapi-0.110.2.dev1/readyapi/openapi/constants.py
--rw-r--r--   0        0        0    10379 2024-05-12 00:15:11.779392 readyapi-0.110.2.dev1/readyapi/openapi/docs.py
--rw-r--r--   0        0        0    17765 2024-05-12 00:15:11.783392 readyapi-0.110.2.dev1/readyapi/openapi/models.py
--rw-r--r--   0        0        0    22299 2024-05-12 00:15:11.783392 readyapi-0.110.2.dev1/readyapi/openapi/utils.py
--rw-r--r--   0        0        0    64082 2024-05-12 00:15:11.783392 readyapi-0.110.2.dev1/readyapi/param_functions.py
--rw-r--r--   0        0        0    28200 2024-05-12 00:15:11.783392 readyapi-0.110.2.dev1/readyapi/params.py
--rw-r--r--   0        0        0        0 2024-05-12 00:15:11.783392 readyapi-0.110.2.dev1/readyapi/py.typed
--rw-r--r--   0        0        0      142 2024-05-12 00:15:11.783392 readyapi-0.110.2.dev1/readyapi/requests.py
--rw-r--r--   0        0        0     1769 2024-05-12 00:15:11.783392 readyapi-0.110.2.dev1/readyapi/responses.py
--rw-r--r--   0        0        0   174906 2024-05-12 00:15:11.783392 readyapi-0.110.2.dev1/readyapi/routing.py
--rw-r--r--   0        0        0      881 2024-05-12 00:15:11.783392 readyapi-0.110.2.dev1/readyapi/security/__init__.py
--rw-r--r--   0        0        0     9382 2024-05-12 00:15:11.783392 readyapi-0.110.2.dev1/readyapi/security/api_key.py
--rw-r--r--   0        0        0      142 2024-05-12 00:15:11.783392 readyapi-0.110.2.dev1/readyapi/security/base.py
--rw-r--r--   0        0        0    13531 2024-05-12 00:15:11.783392 readyapi-0.110.2.dev1/readyapi/security/http.py
--rw-r--r--   0        0        0    21618 2024-05-12 00:15:11.783392 readyapi-0.110.2.dev1/readyapi/security/oauth2.py
--rw-r--r--   0        0        0     2724 2024-05-12 00:15:11.783392 readyapi-0.110.2.dev1/readyapi/security/open_id_connect_url.py
--rw-r--r--   0        0        0      293 2024-05-12 00:15:11.783392 readyapi-0.110.2.dev1/readyapi/security/utils.py
--rw-r--r--   0        0        0       69 2024-05-12 00:15:11.783392 readyapi-0.110.2.dev1/readyapi/staticfiles.py
--rw-r--r--   0        0        0       76 2024-05-12 00:15:11.783392 readyapi-0.110.2.dev1/readyapi/templating.py
--rw-r--r--   0        0        0       66 2024-05-12 00:15:11.783392 readyapi-0.110.2.dev1/readyapi/testclient.py
--rw-r--r--   0        0        0      383 2024-05-12 00:15:11.783392 readyapi-0.110.2.dev1/readyapi/types.py
--rw-r--r--   0        0        0     8044 2024-05-12 00:15:11.783392 readyapi-0.110.2.dev1/readyapi/utils.py
--rw-r--r--   0        0        0      222 2024-05-12 00:15:11.783392 readyapi-0.110.2.dev1/readyapi/websockets.py
--rw-r--r--   0        0        0       52 2024-05-12 00:15:11.783392 readyapi-0.110.2.dev1/requirements-docs-tests.txt
--rw-r--r--   0        0        0      464 2024-05-12 00:15:11.783392 readyapi-0.110.2.dev1/requirements-docs.txt
--rw-r--r--   0        0        0      496 2024-05-12 00:15:11.783392 readyapi-0.110.2.dev1/requirements-tests.txt
--rw-r--r--   0        0        0      128 2024-05-12 00:15:11.783392 readyapi-0.110.2.dev1/requirements.txt
--rwxr-xr-x   0        0        0    11141 2024-05-12 00:15:11.783392 readyapi-0.110.2.dev1/scripts/docs.py
--rwxr-xr-x   0        0        0      114 2024-05-12 00:15:11.783392 readyapi-0.110.2.dev1/scripts/format.sh
--rwxr-xr-x   0        0        0      128 2024-05-12 00:15:11.783392 readyapi-0.110.2.dev1/scripts/lint.sh
--rw-r--r--   0        0        0     5216 2024-05-12 00:15:11.783392 readyapi-0.110.2.dev1/scripts/mkdocs_hooks.py
--rw-r--r--   0        0        0      819 2024-05-12 00:15:11.783392 readyapi-0.110.2.dev1/scripts/playwright/separate_openapi_schemas/image01.py
--rw-r--r--   0        0        0      873 2024-05-12 00:15:11.783392 readyapi-0.110.2.dev1/scripts/playwright/separate_openapi_schemas/image02.py
--rw-r--r--   0        0        0      892 2024-05-12 00:15:11.783392 readyapi-0.110.2.dev1/scripts/playwright/separate_openapi_schemas/image03.py
--rw-r--r--   0        0        0      881 2024-05-12 00:15:11.783392 readyapi-0.110.2.dev1/scripts/playwright/separate_openapi_schemas/image04.py
--rw-r--r--   0        0        0      829 2024-05-12 00:15:11.783392 readyapi-0.110.2.dev1/scripts/playwright/separate_openapi_schemas/image05.py
--rwxr-xr-x   0        0        0      124 2024-05-12 00:15:11.783392 readyapi-0.110.2.dev1/scripts/test-cov-html.sh
--rwxr-xr-x   0        0        0       99 2024-05-12 00:15:11.783392 readyapi-0.110.2.dev1/scripts/test.sh
--rw-r--r--   0        0        0        0 2024-05-12 00:15:11.783392 readyapi-0.110.2.dev1/tests/__init__.py
--rw-r--r--   0        0        0     4455 2024-05-12 00:15:11.783392 readyapi-0.110.2.dev1/tests/main.py
--rw-r--r--   0        0        0     3693 2024-05-12 00:15:11.783392 readyapi-0.110.2.dev1/tests/test_additional_properties.py
--rw-r--r--   0        0        0     4307 2024-05-12 00:15:11.783392 readyapi-0.110.2.dev1/tests/test_additional_properties_bool.py
--rw-r--r--   0        0        0     1212 2024-05-12 00:15:11.783392 readyapi-0.110.2.dev1/tests/test_additional_response_extra.py
--rw-r--r--   0        0        0     1122 2024-05-12 00:15:11.783392 readyapi-0.110.2.dev1/tests/test_additional_responses_bad.py
--rw-r--r--   0        0        0     5900 2024-05-12 00:15:11.783392 readyapi-0.110.2.dev1/tests/test_additional_responses_custom_model_in_callback.py
--rw-r--r--   0        0        0     2980 2024-05-12 00:15:11.783392 readyapi-0.110.2.dev1/tests/test_additional_responses_custom_validationerror.py
--rw-r--r--   0        0        0     2887 2024-05-12 00:15:11.783392 readyapi-0.110.2.dev1/tests/test_additional_responses_default_validationerror.py
--rw-r--r--   0        0        0     3566 2024-05-12 00:15:11.783392 readyapi-0.110.2.dev1/tests/test_additional_responses_response_class.py
--rw-r--r--   0        0        0     5234 2024-05-12 00:15:11.783392 readyapi-0.110.2.dev1/tests/test_additional_responses_router.py
--rw-r--r--   0        0        0     2155 2024-05-12 00:15:11.783392 readyapi-0.110.2.dev1/tests/test_ambiguous_params.py
--rw-r--r--   0        0        0    10500 2024-05-12 00:15:11.783392 readyapi-0.110.2.dev1/tests/test_annotated.py
--rw-r--r--   0        0        0    53493 2024-05-12 00:15:11.783392 readyapi-0.110.2.dev1/tests/test_application.py
--rw-r--r--   0        0        0      461 2024-05-12 00:15:11.783392 readyapi-0.110.2.dev1/tests/test_callable_endpoint.py
--rw-r--r--   0        0        0     2832 2024-05-12 00:15:11.783392 readyapi-0.110.2.dev1/tests/test_compat.py
--rw-r--r--   0        0        0     2269 2024-05-12 00:15:11.783392 readyapi-0.110.2.dev1/tests/test_computed_fields.py
--rw-r--r--   0        0        0     2897 2024-05-12 00:15:11.783392 readyapi-0.110.2.dev1/tests/test_custom_middleware_exception.py
--rw-r--r--   0        0        0     3137 2024-05-12 00:15:11.783392 readyapi-0.110.2.dev1/tests/test_custom_route_class.py
--rw-r--r--   0        0        0     1251 2024-05-12 00:15:11.783392 readyapi-0.110.2.dev1/tests/test_custom_schema_fields.py
--rw-r--r--   0        0        0     1095 2024-05-12 00:15:11.783392 readyapi-0.110.2.dev1/tests/test_custom_swagger_ui_redirect.py
--rw-r--r--   0        0        0     2031 2024-05-12 00:15:11.783392 readyapi-0.110.2.dev1/tests/test_datastructures.py
--rw-r--r--   0        0        0     1609 2024-05-12 00:15:11.783392 readyapi-0.110.2.dev1/tests/test_datetime_custom_encoder.py
--rw-r--r--   0        0        0     5370 2024-05-12 00:15:11.783392 readyapi-0.110.2.dev1/tests/test_default_response_class.py
--rw-r--r--   0        0        0     5122 2024-05-12 00:15:11.783392 readyapi-0.110.2.dev1/tests/test_default_response_class_router.py
--rw-r--r--   0        0        0     2791 2024-05-12 00:15:11.783392 readyapi-0.110.2.dev1/tests/test_dependency_cache.py
--rw-r--r--   0        0        0     3383 2024-05-12 00:15:11.783392 readyapi-0.110.2.dev1/tests/test_dependency_class.py
--rw-r--r--   0        0        0    11874 2024-05-12 00:15:11.783392 readyapi-0.110.2.dev1/tests/test_dependency_contextmanager.py
--rw-r--r--   0        0        0     1564 2024-05-12 00:15:11.783392 readyapi-0.110.2.dev1/tests/test_dependency_contextvars.py
--rw-r--r--   0        0        0     8582 2024-05-12 00:15:11.783392 readyapi-0.110.2.dev1/tests/test_dependency_duplicates.py
--rw-r--r--   0        0        0     1965 2024-05-12 00:15:11.783392 readyapi-0.110.2.dev1/tests/test_dependency_normal_exceptions.py
--rw-r--r--   0        0        0    15820 2024-05-12 00:15:11.783392 readyapi-0.110.2.dev1/tests/test_dependency_overrides.py
--rw-r--r--   0        0        0     1468 2024-05-12 00:15:11.783392 readyapi-0.110.2.dev1/tests/test_dependency_security_overrides.py
--rw-r--r--   0        0        0     1198 2024-05-12 00:15:11.783392 readyapi-0.110.2.dev1/tests/test_deprecated_openapi_prefix.py
--rw-r--r--   0        0        0     2164 2024-05-12 00:15:11.783392 readyapi-0.110.2.dev1/tests/test_duplicate_models_openapi.py
--rw-r--r--   0        0        0      812 2024-05-12 00:15:11.787392 readyapi-0.110.2.dev1/tests/test_empty_router.py
--rw-r--r--   0        0        0     3463 2024-05-12 00:15:11.787392 readyapi-0.110.2.dev1/tests/test_enforce_once_required_parameter.py
--rw-r--r--   0        0        0     1923 2024-05-12 00:15:11.787392 readyapi-0.110.2.dev1/tests/test_exception_handlers.py
--rw-r--r--   0        0        0    14039 2024-05-12 00:15:11.787392 readyapi-0.110.2.dev1/tests/test_extra_routes.py
--rw-r--r--   0        0        0        0 2024-05-12 00:15:11.787392 readyapi-0.110.2.dev1/tests/test_filter_pydantic_sub_model/__init__.py
--rw-r--r--   0        0        0      787 2024-05-12 00:15:11.787392 readyapi-0.110.2.dev1/tests/test_filter_pydantic_sub_model/app_pv1.py
--rw-r--r--   0        0        0     4615 2024-05-12 00:15:11.787392 readyapi-0.110.2.dev1/tests/test_filter_pydantic_sub_model/test_filter_pydantic_sub_model_pv1.py
--rw-r--r--   0        0        0     6467 2024-05-12 00:15:11.787392 readyapi-0.110.2.dev1/tests/test_filter_pydantic_sub_model_pv2.py
--rw-r--r--   0        0        0     1206 2024-05-12 00:15:11.787392 readyapi-0.110.2.dev1/tests/test_forms_from_non_typing_sequences.py
--rw-r--r--   0        0        0    68318 2024-05-12 00:15:11.787392 readyapi-0.110.2.dev1/tests/test_generate_unique_id_function.py
--rw-r--r--   0        0        0     1886 2024-05-12 00:15:11.787392 readyapi-0.110.2.dev1/tests/test_generic_parameterless_depends.py
--rw-r--r--   0        0        0     3749 2024-05-12 00:15:11.787392 readyapi-0.110.2.dev1/tests/test_get_request_body.py
--rw-r--r--   0        0        0      977 2024-05-12 00:15:11.787392 readyapi-0.110.2.dev1/tests/test_http_connection_injection.py
--rw-r--r--   0        0        0      501 2024-05-12 00:15:11.787392 readyapi-0.110.2.dev1/tests/test_include_route.py
--rw-r--r--   0        0        0   367198 2024-05-12 00:15:11.787392 readyapi-0.110.2.dev1/tests/test_include_router_defaults_overrides.py
--rw-r--r--   0        0        0    13624 2024-05-12 00:15:11.787392 readyapi-0.110.2.dev1/tests/test_infer_param_optionality.py
--rw-r--r--   0        0        0     3090 2024-05-12 00:15:11.787392 readyapi-0.110.2.dev1/tests/test_inherited_custom_class.py
--rw-r--r--   0        0        0     1713 2024-05-12 00:15:11.787392 readyapi-0.110.2.dev1/tests/test_invalid_path_param.py
--rw-r--r--   0        0        0     1254 2024-05-12 00:15:11.787392 readyapi-0.110.2.dev1/tests/test_invalid_sequence_param.py
--rw-r--r--   0        0        0     9184 2024-05-12 00:15:11.787392 readyapi-0.110.2.dev1/tests/test_jsonable_encoder.py
--rw-r--r--   0        0        0     2507 2024-05-12 00:15:11.787392 readyapi-0.110.2.dev1/tests/test_local_docs.py
--rw-r--r--   0        0        0        0 2024-05-12 00:15:11.787392 readyapi-0.110.2.dev1/tests/test_modules_same_name_body/__init__.py
--rw-r--r--   0        0        0        0 2024-05-12 00:15:11.787392 readyapi-0.110.2.dev1/tests/test_modules_same_name_body/app/__init__.py
--rw-r--r--   0        0        0      161 2024-05-12 00:15:11.787392 readyapi-0.110.2.dev1/tests/test_modules_same_name_body/app/a.py
--rw-r--r--   0        0        0      162 2024-05-12 00:15:11.787392 readyapi-0.110.2.dev1/tests/test_modules_same_name_body/app/b.py
--rw-r--r--   0        0        0      153 2024-05-12 00:15:11.787392 readyapi-0.110.2.dev1/tests/test_modules_same_name_body/app/main.py
--rw-r--r--   0        0        0     5784 2024-05-12 00:15:11.787392 readyapi-0.110.2.dev1/tests/test_modules_same_name_body/test_main.py
--rw-r--r--   0        0        0     7826 2024-05-12 00:15:11.787392 readyapi-0.110.2.dev1/tests/test_multi_body_errors.py
--rw-r--r--   0        0        0     4615 2024-05-12 00:15:11.787392 readyapi-0.110.2.dev1/tests/test_multi_query_errors.py
--rw-r--r--   0        0        0     3790 2024-05-12 00:15:11.787392 readyapi-0.110.2.dev1/tests/test_multipart_installation.py
--rw-r--r--   0        0        0      790 2024-05-12 00:15:11.787392 readyapi-0.110.2.dev1/tests/test_no_swagger_ui_redirect.py
--rw-r--r--   0        0        0    17443 2024-05-12 00:15:11.787392 readyapi-0.110.2.dev1/tests/test_openapi_examples.py
--rw-r--r--   0        0        0     4852 2024-05-12 00:15:11.787392 readyapi-0.110.2.dev1/tests/test_openapi_query_parameter_extension.py
--rw-r--r--   0        0        0     1138 2024-05-12 00:15:11.787392 readyapi-0.110.2.dev1/tests/test_openapi_route_extensions.py
--rw-r--r--   0        0        0    18893 2024-05-12 00:15:11.787392 readyapi-0.110.2.dev1/tests/test_openapi_separate_input_output_schemas.py
--rw-r--r--   0        0        0     2012 2024-05-12 00:15:11.787392 readyapi-0.110.2.dev1/tests/test_openapi_servers.py
--rw-r--r--   0        0        0      937 2024-05-12 00:15:11.787392 readyapi-0.110.2.dev1/tests/test_operations_signatures.py
--rw-r--r--   0        0        0      567 2024-05-12 00:15:11.787392 readyapi-0.110.2.dev1/tests/test_orjson_response_class.py
--rw-r--r--   0        0        0      641 2024-05-12 00:15:11.787392 readyapi-0.110.2.dev1/tests/test_param_class.py
--rw-r--r--   0        0        0     3142 2024-05-12 00:15:11.787392 readyapi-0.110.2.dev1/tests/test_param_in_path_and_dependency.py
--rw-r--r--   0        0        0     7616 2024-05-12 00:15:11.787392 readyapi-0.110.2.dev1/tests/test_param_include_in_schema.py
--rw-r--r--   0        0        0     3415 2024-05-12 00:15:11.787392 readyapi-0.110.2.dev1/tests/test_params_repr.py
--rw-r--r--   0        0        0    35210 2024-05-12 00:15:11.787392 readyapi-0.110.2.dev1/tests/test_path.py
--rw-r--r--   0        0        0     3367 2024-05-12 00:15:11.787392 readyapi-0.110.2.dev1/tests/test_put_no_body.py
--rw-r--r--   0        0        0    11639 2024-05-12 00:15:11.787392 readyapi-0.110.2.dev1/tests/test_query.py
--rw-r--r--   0        0        0     2420 2024-05-12 00:15:11.787392 readyapi-0.110.2.dev1/tests/test_read_with_orm_mode.py
--rw-r--r--   0        0        0     6349 2024-05-12 00:15:11.787392 readyapi-0.110.2.dev1/tests/test_regex_deprecated_body.py
--rw-r--r--   0        0        0     5600 2024-05-12 00:15:11.787392 readyapi-0.110.2.dev1/tests/test_regex_deprecated_params.py
--rw-r--r--   0        0        0      796 2024-05-12 00:15:11.787392 readyapi-0.110.2.dev1/tests/test_repeated_cookie_headers.py
--rw-r--r--   0        0        0     3253 2024-05-12 00:15:11.787392 readyapi-0.110.2.dev1/tests/test_repeated_dependency_schema.py
--rw-r--r--   0        0        0     3750 2024-05-12 00:15:11.787392 readyapi-0.110.2.dev1/tests/test_repeated_parameter_alias.py
--rw-r--r--   0        0        0     3213 2024-05-12 00:15:11.787392 readyapi-0.110.2.dev1/tests/test_reponse_set_reponse_code_empty.py
--rw-r--r--   0        0        0     6514 2024-05-12 00:15:11.787392 readyapi-0.110.2.dev1/tests/test_request_body_parameters_media_type.py
--rw-r--r--   0        0        0     1534 2024-05-12 00:15:11.787392 readyapi-0.110.2.dev1/tests/test_required_noneable.py
--rw-r--r--   0        0        0    11385 2024-05-12 00:15:11.787392 readyapi-0.110.2.dev1/tests/test_response_by_alias.py
--rw-r--r--   0        0        0      593 2024-05-12 00:15:11.787392 readyapi-0.110.2.dev1/tests/test_response_change_status_code.py
--rw-r--r--   0        0        0     3421 2024-05-12 00:15:11.787392 readyapi-0.110.2.dev1/tests/test_response_class_no_mediatype.py
--rw-r--r--   0        0        0     3321 2024-05-12 00:15:11.787392 readyapi-0.110.2.dev1/tests/test_response_code_no_body.py
--rw-r--r--   0        0        0    48847 2024-05-12 00:15:11.791392 readyapi-0.110.2.dev1/tests/test_response_model_as_return_annotation.py
--rw-r--r--   0        0        0     1730 2024-05-12 00:15:11.791392 readyapi-0.110.2.dev1/tests/test_response_model_data_filter.py
--rw-r--r--   0        0        0     1750 2024-05-12 00:15:11.791392 readyapi-0.110.2.dev1/tests/test_response_model_data_filter_no_inheritance.py
--rw-r--r--   0        0        0     4122 2024-05-12 00:15:11.791392 readyapi-0.110.2.dev1/tests/test_response_model_include_exclude.py
--rw-r--r--   0        0        0     1136 2024-05-12 00:15:11.791392 readyapi-0.110.2.dev1/tests/test_response_model_invalid.py
--rw-r--r--   0        0        0     5384 2024-05-12 00:15:11.791392 readyapi-0.110.2.dev1/tests/test_response_model_sub_types.py
--rw-r--r--   0        0        0     1515 2024-05-12 00:15:11.791392 readyapi-0.110.2.dev1/tests/test_route_scope.py
--rw-r--r--   0        0        0     3301 2024-05-12 00:15:11.791392 readyapi-0.110.2.dev1/tests/test_router_events.py
--rw-r--r--   0        0        0      488 2024-05-12 00:15:11.791392 readyapi-0.110.2.dev1/tests/test_router_prefix_with_template.py
--rw-r--r--   0        0        0      979 2024-05-12 00:15:11.791392 readyapi-0.110.2.dev1/tests/test_router_redirect_slashes.py
--rw-r--r--   0        0        0    38582 2024-05-12 00:15:11.791392 readyapi-0.110.2.dev1/tests/test_schema_extra_examples.py
--rw-r--r--   0        0        0     1950 2024-05-12 00:15:11.791392 readyapi-0.110.2.dev1/tests/test_security_api_key_cookie.py
--rw-r--r--   0        0        0     2118 2024-05-12 00:15:11.791392 readyapi-0.110.2.dev1/tests/test_security_api_key_cookie_description.py
--rw-r--r--   0        0        0     2152 2024-05-12 00:15:11.791392 readyapi-0.110.2.dev1/tests/test_security_api_key_cookie_optional.py
--rw-r--r--   0        0        0     1890 2024-05-12 00:15:11.791392 readyapi-0.110.2.dev1/tests/test_security_api_key_header.py
--rw-r--r--   0        0        0     2058 2024-05-12 00:15:11.791392 readyapi-0.110.2.dev1/tests/test_security_api_key_header_description.py
--rw-r--r--   0        0        0     2088 2024-05-12 00:15:11.791392 readyapi-0.110.2.dev1/tests/test_security_api_key_header_optional.py
--rw-r--r--   0        0        0     1869 2024-05-12 00:15:11.791392 readyapi-0.110.2.dev1/tests/test_security_api_key_query.py
--rw-r--r--   0        0        0     2029 2024-05-12 00:15:11.791392 readyapi-0.110.2.dev1/tests/test_security_api_key_query_description.py
--rw-r--r--   0        0        0     2067 2024-05-12 00:15:11.791392 readyapi-0.110.2.dev1/tests/test_security_api_key_query_optional.py
--rw-r--r--   0        0        0     1793 2024-05-12 00:15:11.791392 readyapi-0.110.2.dev1/tests/test_security_http_base.py
--rw-r--r--   0        0        0     1979 2024-05-12 00:15:11.791392 readyapi-0.110.2.dev1/tests/test_security_http_base_description.py
--rw-r--r--   0        0        0     1938 2024-05-12 00:15:11.791392 readyapi-0.110.2.dev1/tests/test_security_http_base_optional.py
--rw-r--r--   0        0        0     2677 2024-05-12 00:15:11.791392 readyapi-0.110.2.dev1/tests/test_security_http_basic_optional.py
--rw-r--r--   0        0        0     2660 2024-05-12 00:15:11.791392 readyapi-0.110.2.dev1/tests/test_security_http_basic_realm.py
--rw-r--r--   0        0        0     2836 2024-05-12 00:15:11.791392 readyapi-0.110.2.dev1/tests/test_security_http_basic_realm_description.py
--rw-r--r--   0        0        0     2071 2024-05-12 00:15:11.791392 readyapi-0.110.2.dev1/tests/test_security_http_bearer.py
--rw-r--r--   0        0        0     2261 2024-05-12 00:15:11.791392 readyapi-0.110.2.dev1/tests/test_security_http_bearer_description.py
--rw-r--r--   0        0        0     2200 2024-05-12 00:15:11.791392 readyapi-0.110.2.dev1/tests/test_security_http_bearer_optional.py
--rw-r--r--   0        0        0     2096 2024-05-12 00:15:11.791392 readyapi-0.110.2.dev1/tests/test_security_http_digest.py
--rw-r--r--   0        0        0     2272 2024-05-12 00:15:11.791392 readyapi-0.110.2.dev1/tests/test_security_http_digest_description.py
--rw-r--r--   0        0        0     2239 2024-05-12 00:15:11.791392 readyapi-0.110.2.dev1/tests/test_security_http_digest_optional.py
--rw-r--r--   0        0        0    11008 2024-05-12 00:15:11.791392 readyapi-0.110.2.dev1/tests/test_security_oauth2.py
--rw-r--r--   0        0        0     2344 2024-05-12 00:15:11.791392 readyapi-0.110.2.dev1/tests/test_security_oauth2_authorization_code_bearer.py
--rw-r--r--   0        0        0     2448 2024-05-12 00:15:11.791392 readyapi-0.110.2.dev1/tests/test_security_oauth2_authorization_code_bearer_description.py
--rw-r--r--   0        0        0    11049 2024-05-12 00:15:11.791392 readyapi-0.110.2.dev1/tests/test_security_oauth2_optional.py
--rw-r--r--   0        0        0    11189 2024-05-12 00:15:11.791392 readyapi-0.110.2.dev1/tests/test_security_oauth2_optional_description.py
--rw-r--r--   0        0        0     2153 2024-05-12 00:15:11.791392 readyapi-0.110.2.dev1/tests/test_security_oauth2_password_bearer_optional.py
--rw-r--r--   0        0        0     2295 2024-05-12 00:15:11.791392 readyapi-0.110.2.dev1/tests/test_security_oauth2_password_bearer_optional_description.py
--rw-r--r--   0        0        0     2296 2024-05-12 00:15:11.791392 readyapi-0.110.2.dev1/tests/test_security_openid_connect.py
--rw-r--r--   0        0        0     2415 2024-05-12 00:15:11.791392 readyapi-0.110.2.dev1/tests/test_security_openid_connect_description.py
--rw-r--r--   0        0        0     2494 2024-05-12 00:15:11.791392 readyapi-0.110.2.dev1/tests/test_security_openid_connect_optional.py
--rw-r--r--   0        0        0     1418 2024-05-12 00:15:11.791392 readyapi-0.110.2.dev1/tests/test_serialize_response.py
--rw-r--r--   0        0        0     5002 2024-05-12 00:15:11.791392 readyapi-0.110.2.dev1/tests/test_serialize_response_dataclass.py
--rw-r--r--   0        0        0     4279 2024-05-12 00:15:11.791392 readyapi-0.110.2.dev1/tests/test_serialize_response_model.py
--rw-r--r--   0        0        0     2075 2024-05-12 00:15:11.791392 readyapi-0.110.2.dev1/tests/test_skip_defaults.py
--rw-r--r--   0        0        0     7555 2024-05-12 00:15:11.791392 readyapi-0.110.2.dev1/tests/test_starlette_exception.py
--rw-r--r--   0        0        0     1714 2024-05-12 00:15:11.791392 readyapi-0.110.2.dev1/tests/test_starlette_urlconvertors.py
--rw-r--r--   0        0        0    14147 2024-05-12 00:15:11.791392 readyapi-0.110.2.dev1/tests/test_sub_callbacks.py
--rw-r--r--   0        0        0      722 2024-05-12 00:15:11.791392 readyapi-0.110.2.dev1/tests/test_swagger_ui_init_oauth.py
--rw-r--r--   0        0        0    12073 2024-05-12 00:15:11.791392 readyapi-0.110.2.dev1/tests/test_tuples.py
--rw-r--r--   0        0        0        0 2024-05-12 00:15:11.791392 readyapi-0.110.2.dev1/tests/test_tutorial/__init__.py
--rw-r--r--   0        0        0        0 2024-05-12 00:15:11.791392 readyapi-0.110.2.dev1/tests/test_tutorial/test_additional_responses/__init__.py
--rw-r--r--   0        0        0     4434 2024-05-12 00:15:11.791392 readyapi-0.110.2.dev1/tests/test_tutorial/test_additional_responses/test_tutorial001.py
--rw-r--r--   0        0        0     4742 2024-05-12 00:15:11.791392 readyapi-0.110.2.dev1/tests/test_tutorial/test_additional_responses/test_tutorial002.py
--rw-r--r--   0        0        0     4658 2024-05-12 00:15:11.791392 readyapi-0.110.2.dev1/tests/test_tutorial/test_additional_responses/test_tutorial003.py
--rw-r--r--   0        0        0     4937 2024-05-12 00:15:11.791392 readyapi-0.110.2.dev1/tests/test_tutorial/test_additional_responses/test_tutorial004.py
--rw-r--r--   0        0        0        0 2024-05-12 00:15:11.791392 readyapi-0.110.2.dev1/tests/test_tutorial/test_additional_status_codes/__init__.py
--rw-r--r--   0        0        0      547 2024-05-12 00:15:11.791392 readyapi-0.110.2.dev1/tests/test_tutorial/test_additional_status_codes/test_tutorial001.py
--rw-r--r--   0        0        0      550 2024-05-12 00:15:11.791392 readyapi-0.110.2.dev1/tests/test_tutorial/test_additional_status_codes/test_tutorial001_an.py
--rw-r--r--   0        0        0      742 2024-05-12 00:15:11.791392 readyapi-0.110.2.dev1/tests/test_tutorial/test_additional_status_codes/test_tutorial001_an_py310.py
--rw-r--r--   0        0        0      738 2024-05-12 00:15:11.791392 readyapi-0.110.2.dev1/tests/test_tutorial/test_additional_status_codes/test_tutorial001_an_py39.py
--rw-r--r--   0        0        0      739 2024-05-12 00:15:11.791392 readyapi-0.110.2.dev1/tests/test_tutorial/test_additional_status_codes/test_tutorial001_py310.py
--rw-r--r--   0        0        0        0 2024-05-12 00:15:11.791392 readyapi-0.110.2.dev1/tests/test_tutorial/test_advanced_middleware/__init__.py
--rw-r--r--   0        0        0      475 2024-05-12 00:15:11.791392 readyapi-0.110.2.dev1/tests/test_tutorial/test_advanced_middleware/test_tutorial001.py
--rw-r--r--   0        0        0      571 2024-05-12 00:15:11.791392 readyapi-0.110.2.dev1/tests/test_tutorial/test_advanced_middleware/test_tutorial002.py
--rw-r--r--   0        0        0      667 2024-05-12 00:15:11.791392 readyapi-0.110.2.dev1/tests/test_tutorial/test_advanced_middleware/test_tutorial003.py
--rw-r--r--   0        0        0        0 2024-05-12 00:15:11.791392 readyapi-0.110.2.dev1/tests/test_tutorial/test_async_sql_databases/__init__.py
--rw-r--r--   0        0        0     6128 2024-05-12 00:15:11.791392 readyapi-0.110.2.dev1/tests/test_tutorial/test_async_sql_databases/test_tutorial001.py
--rw-r--r--   0        0        0        0 2024-05-12 00:15:11.791392 readyapi-0.110.2.dev1/tests/test_tutorial/test_async_tests/__init__.py
--rw-r--r--   0        0        0      143 2024-05-12 00:15:11.791392 readyapi-0.110.2.dev1/tests/test_tutorial/test_async_tests/test_main.py
--rw-r--r--   0        0        0        0 2024-05-12 00:15:11.791392 readyapi-0.110.2.dev1/tests/test_tutorial/test_background_tasks/__init__.py
--rw-r--r--   0        0        0      579 2024-05-12 00:15:11.791392 readyapi-0.110.2.dev1/tests/test_tutorial/test_background_tasks/test_tutorial001.py
--rw-r--r--   0        0        0      569 2024-05-12 00:15:11.791392 readyapi-0.110.2.dev1/tests/test_tutorial/test_background_tasks/test_tutorial002.py
--rw-r--r--   0        0        0      572 2024-05-12 00:15:11.791392 readyapi-0.110.2.dev1/tests/test_tutorial/test_background_tasks/test_tutorial002_an.py
--rw-r--r--   0        0        0      632 2024-05-12 00:15:11.791392 readyapi-0.110.2.dev1/tests/test_tutorial/test_background_tasks/test_tutorial002_an_py310.py
--rw-r--r--   0        0        0      629 2024-05-12 00:15:11.791392 readyapi-0.110.2.dev1/tests/test_tutorial/test_background_tasks/test_tutorial002_an_py39.py
--rw-r--r--   0        0        0      629 2024-05-12 00:15:11.791392 readyapi-0.110.2.dev1/tests/test_tutorial/test_background_tasks/test_tutorial002_py310.py
--rw-r--r--   0        0        0        0 2024-05-12 00:15:11.791392 readyapi-0.110.2.dev1/tests/test_tutorial/test_behind_a_proxy/__init__.py
--rw-r--r--   0        0        0     1055 2024-05-12 00:15:11.791392 readyapi-0.110.2.dev1/tests/test_tutorial/test_behind_a_proxy/test_tutorial001.py
--rw-r--r--   0        0        0     1034 2024-05-12 00:15:11.795392 readyapi-0.110.2.dev1/tests/test_tutorial/test_behind_a_proxy/test_tutorial002.py
--rw-r--r--   0        0        0     1690 2024-05-12 00:15:11.795392 readyapi-0.110.2.dev1/tests/test_tutorial/test_behind_a_proxy/test_tutorial003.py
--rw-r--r--   0        0        0     1658 2024-05-12 00:15:11.795392 readyapi-0.110.2.dev1/tests/test_tutorial/test_behind_a_proxy/test_tutorial004.py
--rw-r--r--   0        0        0        0 2024-05-12 00:15:11.795392 readyapi-0.110.2.dev1/tests/test_tutorial/test_bigger_applications/__init__.py
--rw-r--r--   0        0        0    25142 2024-05-12 00:15:11.795392 readyapi-0.110.2.dev1/tests/test_tutorial/test_bigger_applications/test_main.py
--rw-r--r--   0        0        0    25145 2024-05-12 00:15:11.795392 readyapi-0.110.2.dev1/tests/test_tutorial/test_bigger_applications/test_main_an.py
--rw-r--r--   0        0        0    25483 2024-05-12 00:15:11.795392 readyapi-0.110.2.dev1/tests/test_tutorial/test_bigger_applications/test_main_an_py39.py
--rw-r--r--   0        0        0        0 2024-05-12 00:15:11.795392 readyapi-0.110.2.dev1/tests/test_tutorial/test_body/__init__.py
--rw-r--r--   0        0        0    15094 2024-05-12 00:15:11.795392 readyapi-0.110.2.dev1/tests/test_tutorial/test_body/test_tutorial001.py
--rw-r--r--   0        0        0    15342 2024-05-12 00:15:11.795392 readyapi-0.110.2.dev1/tests/test_tutorial/test_body/test_tutorial001_py310.py
--rw-r--r--   0        0        0        0 2024-05-12 00:15:11.795392 readyapi-0.110.2.dev1/tests/test_tutorial/test_body_fields/__init__.py
--rw-r--r--   0        0        0     7343 2024-05-12 00:15:11.795392 readyapi-0.110.2.dev1/tests/test_tutorial/test_body_fields/test_tutorial001.py
--rw-r--r--   0        0        0     7346 2024-05-12 00:15:11.795392 readyapi-0.110.2.dev1/tests/test_tutorial/test_body_fields/test_tutorial001_an.py
--rw-r--r--   0        0        0     7438 2024-05-12 00:15:11.795392 readyapi-0.110.2.dev1/tests/test_tutorial/test_body_fields/test_tutorial001_an_py310.py
--rw-r--r--   0        0        0     7432 2024-05-12 00:15:11.795392 readyapi-0.110.2.dev1/tests/test_tutorial/test_body_fields/test_tutorial001_an_py39.py
--rw-r--r--   0        0        0     7435 2024-05-12 00:15:11.795392 readyapi-0.110.2.dev1/tests/test_tutorial/test_body_fields/test_tutorial001_py310.py
--rw-r--r--   0        0        0        0 2024-05-12 00:15:11.795392 readyapi-0.110.2.dev1/tests/test_tutorial/test_body_multiple_params/__init__.py
--rw-r--r--   0        0        0     7700 2024-05-12 00:15:11.795392 readyapi-0.110.2.dev1/tests/test_tutorial/test_body_multiple_params/test_tutorial001.py
--rw-r--r--   0        0        0     7703 2024-05-12 00:15:11.795392 readyapi-0.110.2.dev1/tests/test_tutorial/test_body_multiple_params/test_tutorial001_an.py
--rw-r--r--   0        0        0     7808 2024-05-12 00:15:11.795392 readyapi-0.110.2.dev1/tests/test_tutorial/test_body_multiple_params/test_tutorial001_an_py310.py
--rw-r--r--   0        0        0     7801 2024-05-12 00:15:11.795392 readyapi-0.110.2.dev1/tests/test_tutorial/test_body_multiple_params/test_tutorial001_an_py39.py
--rw-r--r--   0        0        0     7805 2024-05-12 00:15:11.795392 readyapi-0.110.2.dev1/tests/test_tutorial/test_body_multiple_params/test_tutorial001_py310.py
--rw-r--r--   0        0        0     9662 2024-05-12 00:15:11.795392 readyapi-0.110.2.dev1/tests/test_tutorial/test_body_multiple_params/test_tutorial003.py
--rw-r--r--   0        0        0     9665 2024-05-12 00:15:11.795392 readyapi-0.110.2.dev1/tests/test_tutorial/test_body_multiple_params/test_tutorial003_an.py
--rw-r--r--   0        0        0     9757 2024-05-12 00:15:11.795392 readyapi-0.110.2.dev1/tests/test_tutorial/test_body_multiple_params/test_tutorial003_an_py310.py
--rw-r--r--   0        0        0     9751 2024-05-12 00:15:11.795392 readyapi-0.110.2.dev1/tests/test_tutorial/test_body_multiple_params/test_tutorial003_an_py39.py
--rw-r--r--   0        0        0     9754 2024-05-12 00:15:11.795392 readyapi-0.110.2.dev1/tests/test_tutorial/test_body_multiple_params/test_tutorial003_py310.py
--rw-r--r--   0        0        0        0 2024-05-12 00:15:11.795392 readyapi-0.110.2.dev1/tests/test_tutorial/test_body_nested_models/__init__.py
--rw-r--r--   0        0        0     4345 2024-05-12 00:15:11.795392 readyapi-0.110.2.dev1/tests/test_tutorial/test_body_nested_models/test_tutorial009.py
--rw-r--r--   0        0        0     4419 2024-05-12 00:15:11.795392 readyapi-0.110.2.dev1/tests/test_tutorial/test_body_nested_models/test_tutorial009_py39.py
--rw-r--r--   0        0        0        0 2024-05-12 00:15:11.795392 readyapi-0.110.2.dev1/tests/test_tutorial/test_body_updates/__init__.py
--rw-r--r--   0        0        0    12043 2024-05-12 00:15:11.795392 readyapi-0.110.2.dev1/tests/test_tutorial/test_body_updates/test_tutorial001.py
--rw-r--r--   0        0        0    12114 2024-05-12 00:15:11.795392 readyapi-0.110.2.dev1/tests/test_tutorial/test_body_updates/test_tutorial001_py310.py
--rw-r--r--   0        0        0    12108 2024-05-12 00:15:11.795392 readyapi-0.110.2.dev1/tests/test_tutorial/test_body_updates/test_tutorial001_py39.py
--rw-r--r--   0        0        0        0 2024-05-12 00:15:11.795392 readyapi-0.110.2.dev1/tests/test_tutorial/test_conditional_openapi/__init__.py
--rw-r--r--   0        0        0     1801 2024-05-12 00:15:11.795392 readyapi-0.110.2.dev1/tests/test_tutorial/test_conditional_openapi/test_tutorial001.py
--rw-r--r--   0        0        0        0 2024-05-12 00:15:11.795392 readyapi-0.110.2.dev1/tests/test_tutorial/test_configure_swagger_ui/__init__.py
--rw-r--r--   0        0        0     1416 2024-05-12 00:15:11.795392 readyapi-0.110.2.dev1/tests/test_tutorial/test_configure_swagger_ui/test_tutorial001.py
--rw-r--r--   0        0        0     1563 2024-05-12 00:15:11.795392 readyapi-0.110.2.dev1/tests/test_tutorial/test_configure_swagger_ui/test_tutorial002.py
--rw-r--r--   0        0        0     1535 2024-05-12 00:15:11.795392 readyapi-0.110.2.dev1/tests/test_tutorial/test_configure_swagger_ui/test_tutorial003.py
--rw-r--r--   0        0        0        0 2024-05-12 00:15:11.795392 readyapi-0.110.2.dev1/tests/test_tutorial/test_cookie_params/__init__.py
--rw-r--r--   0        0        0     4019 2024-05-12 00:15:11.795392 readyapi-0.110.2.dev1/tests/test_tutorial/test_cookie_params/test_tutorial001.py
--rw-r--r--   0        0        0     4022 2024-05-12 00:15:11.795392 readyapi-0.110.2.dev1/tests/test_tutorial/test_cookie_params/test_tutorial001_an.py
--rw-r--r--   0        0        0     4157 2024-05-12 00:15:11.795392 readyapi-0.110.2.dev1/tests/test_tutorial/test_cookie_params/test_tutorial001_an_py310.py
--rw-r--r--   0        0        0     4152 2024-05-12 00:15:11.795392 readyapi-0.110.2.dev1/tests/test_tutorial/test_cookie_params/test_tutorial001_an_py39.py
--rw-r--r--   0        0        0     4151 2024-05-12 00:15:11.795392 readyapi-0.110.2.dev1/tests/test_tutorial/test_cookie_params/test_tutorial001_py310.py
--rw-r--r--   0        0        0        0 2024-05-12 00:15:11.795392 readyapi-0.110.2.dev1/tests/test_tutorial/test_cors/__init__.py
--rw-r--r--   0        0        0     1287 2024-05-12 00:15:11.795392 readyapi-0.110.2.dev1/tests/test_tutorial/test_cors/test_tutorial001.py
--rw-r--r--   0        0        0        0 2024-05-12 00:15:11.795392 readyapi-0.110.2.dev1/tests/test_tutorial/test_custom_docs_ui/__init__.py
--rw-r--r--   0        0        0     1359 2024-05-12 00:15:11.795392 readyapi-0.110.2.dev1/tests/test_tutorial/test_custom_docs_ui/test_tutorial001.py
--rw-r--r--   0        0        0     1250 2024-05-12 00:15:11.795392 readyapi-0.110.2.dev1/tests/test_tutorial/test_custom_docs_ui/test_tutorial002.py
--rw-r--r--   0        0        0        0 2024-05-12 00:15:11.795392 readyapi-0.110.2.dev1/tests/test_tutorial/test_custom_request_and_route/__init__.py
--rw-r--r--   0        0        0      888 2024-05-12 00:15:11.795392 readyapi-0.110.2.dev1/tests/test_tutorial/test_custom_request_and_route/test_tutorial001.py
--rw-r--r--   0        0        0     1246 2024-05-12 00:15:11.795392 readyapi-0.110.2.dev1/tests/test_tutorial/test_custom_request_and_route/test_tutorial002.py
--rw-r--r--   0        0        0      527 2024-05-12 00:15:11.795392 readyapi-0.110.2.dev1/tests/test_tutorial/test_custom_request_and_route/test_tutorial003.py
--rw-r--r--   0        0        0        0 2024-05-12 00:15:11.795392 readyapi-0.110.2.dev1/tests/test_tutorial/test_custom_response/__init__.py
--rw-r--r--   0        0        0     1027 2024-05-12 00:15:11.795392 readyapi-0.110.2.dev1/tests/test_tutorial/test_custom_response/test_tutorial001.py
--rw-r--r--   0        0        0     1028 2024-05-12 00:15:11.795392 readyapi-0.110.2.dev1/tests/test_tutorial/test_custom_response/test_tutorial001b.py
--rw-r--r--   0        0        0     1223 2024-05-12 00:15:11.795392 readyapi-0.110.2.dev1/tests/test_tutorial/test_custom_response/test_tutorial004.py
--rw-r--r--   0        0        0      982 2024-05-12 00:15:11.795392 readyapi-0.110.2.dev1/tests/test_tutorial/test_custom_response/test_tutorial005.py
--rw-r--r--   0        0        0     1061 2024-05-12 00:15:11.795392 readyapi-0.110.2.dev1/tests/test_tutorial/test_custom_response/test_tutorial006.py
--rw-r--r--   0        0        0      909 2024-05-12 00:15:11.795392 readyapi-0.110.2.dev1/tests/test_tutorial/test_custom_response/test_tutorial006b.py
--rw-r--r--   0        0        0      901 2024-05-12 00:15:11.795392 readyapi-0.110.2.dev1/tests/test_tutorial/test_custom_response/test_tutorial006c.py
--rw-r--r--   0        0        0      265 2024-05-12 00:15:11.795392 readyapi-0.110.2.dev1/tests/test_tutorial/test_custom_response/test_tutorial007.py
--rw-r--r--   0        0        0      488 2024-05-12 00:15:11.795392 readyapi-0.110.2.dev1/tests/test_tutorial/test_custom_response/test_tutorial008.py
--rw-r--r--   0        0        0      488 2024-05-12 00:15:11.795392 readyapi-0.110.2.dev1/tests/test_tutorial/test_custom_response/test_tutorial009.py
--rw-r--r--   0        0        0      491 2024-05-12 00:15:11.795392 readyapi-0.110.2.dev1/tests/test_tutorial/test_custom_response/test_tutorial009b.py
--rw-r--r--   0        0        0      240 2024-05-12 00:15:11.795392 readyapi-0.110.2.dev1/tests/test_tutorial/test_custom_response/test_tutorial009c.py
--rw-r--r--   0        0        0        0 2024-05-12 00:15:11.795392 readyapi-0.110.2.dev1/tests/test_tutorial/test_dataclasses/__init__.py
--rw-r--r--   0        0        0     5291 2024-05-12 00:15:11.795392 readyapi-0.110.2.dev1/tests/test_tutorial/test_dataclasses/test_tutorial001.py
--rw-r--r--   0        0        0     3576 2024-05-12 00:15:11.795392 readyapi-0.110.2.dev1/tests/test_tutorial/test_dataclasses/test_tutorial002.py
--rw-r--r--   0        0        0    12359 2024-05-12 00:15:11.795392 readyapi-0.110.2.dev1/tests/test_tutorial/test_dataclasses/test_tutorial003.py
--rw-r--r--   0        0        0        0 2024-05-12 00:15:11.795392 readyapi-0.110.2.dev1/tests/test_tutorial/test_dependencies/__init__.py
--rw-r--r--   0        0        0     7221 2024-05-12 00:15:11.795392 readyapi-0.110.2.dev1/tests/test_tutorial/test_dependencies/test_tutorial001.py
--rw-r--r--   0        0        0     7224 2024-05-12 00:15:11.795392 readyapi-0.110.2.dev1/tests/test_tutorial/test_dependencies/test_tutorial001_an.py
--rw-r--r--   0        0        0     7404 2024-05-12 00:15:11.795392 readyapi-0.110.2.dev1/tests/test_tutorial/test_dependencies/test_tutorial001_an_py310.py
--rw-r--r--   0        0        0     7400 2024-05-12 00:15:11.795392 readyapi-0.110.2.dev1/tests/test_tutorial/test_dependencies/test_tutorial001_an_py39.py
--rw-r--r--   0        0        0     7401 2024-05-12 00:15:11.795392 readyapi-0.110.2.dev1/tests/test_tutorial/test_dependencies/test_tutorial001_py310.py
--rw-r--r--   0        0        0     5553 2024-05-12 00:15:11.795392 readyapi-0.110.2.dev1/tests/test_tutorial/test_dependencies/test_tutorial004.py
--rw-r--r--   0        0        0     5556 2024-05-12 00:15:11.795392 readyapi-0.110.2.dev1/tests/test_tutorial/test_dependencies/test_tutorial004_an.py
--rw-r--r--   0        0        0     5736 2024-05-12 00:15:11.795392 readyapi-0.110.2.dev1/tests/test_tutorial/test_dependencies/test_tutorial004_an_py310.py
--rw-r--r--   0        0        0     5732 2024-05-12 00:15:11.795392 readyapi-0.110.2.dev1/tests/test_tutorial/test_dependencies/test_tutorial004_an_py39.py
--rw-r--r--   0        0        0     5733 2024-05-12 00:15:11.795392 readyapi-0.110.2.dev1/tests/test_tutorial/test_dependencies/test_tutorial004_py310.py
--rw-r--r--   0        0        0     5121 2024-05-12 00:15:11.795392 readyapi-0.110.2.dev1/tests/test_tutorial/test_dependencies/test_tutorial006.py
--rw-r--r--   0        0        0     5124 2024-05-12 00:15:11.799392 readyapi-0.110.2.dev1/tests/test_tutorial/test_dependencies/test_tutorial006_an.py
--rw-r--r--   0        0        0     5402 2024-05-12 00:15:11.799392 readyapi-0.110.2.dev1/tests/test_tutorial/test_dependencies/test_tutorial006_an_py39.py
--rw-r--r--   0        0        0      698 2024-05-12 00:15:11.799392 readyapi-0.110.2.dev1/tests/test_tutorial/test_dependencies/test_tutorial008b.py
--rw-r--r--   0        0        0      701 2024-05-12 00:15:11.799392 readyapi-0.110.2.dev1/tests/test_tutorial/test_dependencies/test_tutorial008b_an.py
--rw-r--r--   0        0        0      919 2024-05-12 00:15:11.799392 readyapi-0.110.2.dev1/tests/test_tutorial/test_dependencies/test_tutorial008b_an_py39.py
--rw-r--r--   0        0        0     1171 2024-05-12 00:15:11.799392 readyapi-0.110.2.dev1/tests/test_tutorial/test_dependencies/test_tutorial008c.py
--rw-r--r--   0        0        0     1177 2024-05-12 00:15:11.799392 readyapi-0.110.2.dev1/tests/test_tutorial/test_dependencies/test_tutorial008c_an.py
--rw-r--r--   0        0        0     1268 2024-05-12 00:15:11.799392 readyapi-0.110.2.dev1/tests/test_tutorial/test_dependencies/test_tutorial008c_an_py39.py
--rw-r--r--   0        0        0     1227 2024-05-12 00:15:11.799392 readyapi-0.110.2.dev1/tests/test_tutorial/test_dependencies/test_tutorial008d.py
--rw-r--r--   0        0        0     1236 2024-05-12 00:15:11.799392 readyapi-0.110.2.dev1/tests/test_tutorial/test_dependencies/test_tutorial008d_an.py
--rw-r--r--   0        0        0     1332 2024-05-12 00:15:11.799392 readyapi-0.110.2.dev1/tests/test_tutorial/test_dependencies/test_tutorial008d_an_py39.py
--rw-r--r--   0        0        0     8640 2024-05-12 00:15:11.799392 readyapi-0.110.2.dev1/tests/test_tutorial/test_dependencies/test_tutorial012.py
--rw-r--r--   0        0        0     8643 2024-05-12 00:15:11.799392 readyapi-0.110.2.dev1/tests/test_tutorial/test_dependencies/test_tutorial012_an.py
--rw-r--r--   0        0        0     9041 2024-05-12 00:15:11.799392 readyapi-0.110.2.dev1/tests/test_tutorial/test_dependencies/test_tutorial012_an_py39.py
--rw-r--r--   0        0        0        0 2024-05-12 00:15:11.799392 readyapi-0.110.2.dev1/tests/test_tutorial/test_events/__init__.py
--rw-r--r--   0        0        0     3644 2024-05-12 00:15:11.799392 readyapi-0.110.2.dev1/tests/test_tutorial/test_events/test_tutorial001.py
--rw-r--r--   0        0        0     1420 2024-05-12 00:15:11.799392 readyapi-0.110.2.dev1/tests/test_tutorial/test_events/test_tutorial002.py
--rw-r--r--   0        0        0     3686 2024-05-12 00:15:11.799392 readyapi-0.110.2.dev1/tests/test_tutorial/test_events/test_tutorial003.py
--rw-r--r--   0        0        0        0 2024-05-12 00:15:11.799392 readyapi-0.110.2.dev1/tests/test_tutorial/test_extending_openapi/__init__.py
--rw-r--r--   0        0        0     1549 2024-05-12 00:15:11.799392 readyapi-0.110.2.dev1/tests/test_tutorial/test_extending_openapi/test_tutorial001.py
--rw-r--r--   0        0        0        0 2024-05-12 00:15:11.799392 readyapi-0.110.2.dev1/tests/test_tutorial/test_extra_data_types/__init__.py
--rw-r--r--   0        0        0     8029 2024-05-12 00:15:11.799392 readyapi-0.110.2.dev1/tests/test_tutorial/test_extra_data_types/test_tutorial001.py
--rw-r--r--   0        0        0     8032 2024-05-12 00:15:11.799392 readyapi-0.110.2.dev1/tests/test_tutorial/test_extra_data_types/test_tutorial001_an.py
--rw-r--r--   0        0        0     8224 2024-05-12 00:15:11.799392 readyapi-0.110.2.dev1/tests/test_tutorial/test_extra_data_types/test_tutorial001_an_py310.py
--rw-r--r--   0        0        0     8220 2024-05-12 00:15:11.799392 readyapi-0.110.2.dev1/tests/test_tutorial/test_extra_data_types/test_tutorial001_an_py39.py
--rw-r--r--   0        0        0     8221 2024-05-12 00:15:11.799392 readyapi-0.110.2.dev1/tests/test_tutorial/test_extra_data_types/test_tutorial001_py310.py
--rw-r--r--   0        0        0        0 2024-05-12 00:15:11.799392 readyapi-0.110.2.dev1/tests/test_tutorial/test_extra_models/__init__.py
--rw-r--r--   0        0        0     5197 2024-05-12 00:15:11.799392 readyapi-0.110.2.dev1/tests/test_tutorial/test_extra_models/test_tutorial003.py
--rw-r--r--   0        0        0     5420 2024-05-12 00:15:11.799392 readyapi-0.110.2.dev1/tests/test_tutorial/test_extra_models/test_tutorial003_py310.py
--rw-r--r--   0        0        0     1983 2024-05-12 00:15:11.799392 readyapi-0.110.2.dev1/tests/test_tutorial/test_extra_models/test_tutorial004.py
--rw-r--r--   0        0        0     2171 2024-05-12 00:15:11.799392 readyapi-0.110.2.dev1/tests/test_tutorial/test_extra_models/test_tutorial004_py39.py
--rw-r--r--   0        0        0     1482 2024-05-12 00:15:11.799392 readyapi-0.110.2.dev1/tests/test_tutorial/test_extra_models/test_tutorial005.py
--rw-r--r--   0        0        0     1670 2024-05-12 00:15:11.799392 readyapi-0.110.2.dev1/tests/test_tutorial/test_extra_models/test_tutorial005_py39.py
--rw-r--r--   0        0        0        0 2024-05-12 00:15:11.799392 readyapi-0.110.2.dev1/tests/test_tutorial/test_first_steps/__init__.py
--rw-r--r--   0        0        0     1207 2024-05-12 00:15:11.799392 readyapi-0.110.2.dev1/tests/test_tutorial/test_first_steps/test_tutorial001.py
--rw-r--r--   0        0        0        0 2024-05-12 00:15:11.799392 readyapi-0.110.2.dev1/tests/test_tutorial/test_generate_clients/__init__.py
--rw-r--r--   0        0        0     7249 2024-05-12 00:15:11.799392 readyapi-0.110.2.dev1/tests/test_tutorial/test_generate_clients/test_tutorial003.py
--rw-r--r--   0        0        0        0 2024-05-12 00:15:11.799392 readyapi-0.110.2.dev1/tests/test_tutorial/test_handling_errors/__init__.py
--rw-r--r--   0        0        0     3300 2024-05-12 00:15:11.799392 readyapi-0.110.2.dev1/tests/test_tutorial/test_handling_errors/test_tutorial001.py
--rw-r--r--   0        0        0     3373 2024-05-12 00:15:11.799392 readyapi-0.110.2.dev1/tests/test_tutorial/test_handling_errors/test_tutorial002.py
--rw-r--r--   0        0        0     3296 2024-05-12 00:15:11.799392 readyapi-0.110.2.dev1/tests/test_tutorial/test_handling_errors/test_tutorial003.py
--rw-r--r--   0        0        0     3802 2024-05-12 00:15:11.799392 readyapi-0.110.2.dev1/tests/test_tutorial/test_handling_errors/test_tutorial004.py
--rw-r--r--   0        0        0     4431 2024-05-12 00:15:11.799392 readyapi-0.110.2.dev1/tests/test_tutorial/test_handling_errors/test_tutorial005.py
--rw-r--r--   0        0        0     4074 2024-05-12 00:15:11.799392 readyapi-0.110.2.dev1/tests/test_tutorial/test_handling_errors/test_tutorial006.py
--rw-r--r--   0        0        0        0 2024-05-12 00:15:11.799392 readyapi-0.110.2.dev1/tests/test_tutorial/test_header_params/__init__.py
--rw-r--r--   0        0        0     3932 2024-05-12 00:15:11.799392 readyapi-0.110.2.dev1/tests/test_tutorial/test_header_params/test_tutorial001.py
--rw-r--r--   0        0        0     3935 2024-05-12 00:15:11.799392 readyapi-0.110.2.dev1/tests/test_tutorial/test_header_params/test_tutorial001_an.py
--rw-r--r--   0        0        0     4115 2024-05-12 00:15:11.799392 readyapi-0.110.2.dev1/tests/test_tutorial/test_header_params/test_tutorial001_an_py310.py
--rw-r--r--   0        0        0     4112 2024-05-12 00:15:11.799392 readyapi-0.110.2.dev1/tests/test_tutorial/test_header_params/test_tutorial001_py310.py
--rw-r--r--   0        0        0     4099 2024-05-12 00:15:11.799392 readyapi-0.110.2.dev1/tests/test_tutorial/test_header_params/test_tutorial002.py
--rw-r--r--   0        0        0     4102 2024-05-12 00:15:11.799392 readyapi-0.110.2.dev1/tests/test_tutorial/test_header_params/test_tutorial002_an.py
--rw-r--r--   0        0        0     4282 2024-05-12 00:15:11.799392 readyapi-0.110.2.dev1/tests/test_tutorial/test_header_params/test_tutorial002_an_py310.py
--rw-r--r--   0        0        0     4353 2024-05-12 00:15:11.799392 readyapi-0.110.2.dev1/tests/test_tutorial/test_header_params/test_tutorial002_an_py39.py
--rw-r--r--   0        0        0     4352 2024-05-12 00:15:11.799392 readyapi-0.110.2.dev1/tests/test_tutorial/test_header_params/test_tutorial002_py310.py
--rw-r--r--   0        0        0     4242 2024-05-12 00:15:11.799392 readyapi-0.110.2.dev1/tests/test_tutorial/test_header_params/test_tutorial003.py
--rw-r--r--   0        0        0     4227 2024-05-12 00:15:11.799392 readyapi-0.110.2.dev1/tests/test_tutorial/test_header_params/test_tutorial003_an.py
--rw-r--r--   0        0        0     4407 2024-05-12 00:15:11.799392 readyapi-0.110.2.dev1/tests/test_tutorial/test_header_params/test_tutorial003_an_py310.py
--rw-r--r--   0        0        0     4403 2024-05-12 00:15:11.799392 readyapi-0.110.2.dev1/tests/test_tutorial/test_header_params/test_tutorial003_an_py39.py
--rw-r--r--   0        0        0     4404 2024-05-12 00:15:11.799392 readyapi-0.110.2.dev1/tests/test_tutorial/test_header_params/test_tutorial003_py310.py
--rw-r--r--   0        0        0        0 2024-05-12 00:15:11.799392 readyapi-0.110.2.dev1/tests/test_tutorial/test_metadata/__init__.py
--rw-r--r--   0        0        0     1765 2024-05-12 00:15:11.799392 readyapi-0.110.2.dev1/tests/test_tutorial/test_metadata/test_tutorial001.py
--rw-r--r--   0        0        0     1729 2024-05-12 00:15:11.799392 readyapi-0.110.2.dev1/tests/test_tutorial/test_metadata/test_tutorial001_1.py
--rw-r--r--   0        0        0     2082 2024-05-12 00:15:11.799392 readyapi-0.110.2.dev1/tests/test_tutorial/test_metadata/test_tutorial004.py
--rw-r--r--   0        0        0        0 2024-05-12 00:15:11.799392 readyapi-0.110.2.dev1/tests/test_tutorial/test_openapi_callbacks/__init__.py
--rw-r--r--   0        0        0     9218 2024-05-12 00:15:11.799392 readyapi-0.110.2.dev1/tests/test_tutorial/test_openapi_callbacks/test_tutorial001.py
--rw-r--r--   0        0        0        0 2024-05-12 00:15:11.799392 readyapi-0.110.2.dev1/tests/test_tutorial/test_openapi_webhooks/__init__.py
--rw-r--r--   0        0        0     4494 2024-05-12 00:15:11.799392 readyapi-0.110.2.dev1/tests/test_tutorial/test_openapi_webhooks/test_tutorial001.py
--rw-r--r--   0        0        0        0 2024-05-12 00:15:11.799392 readyapi-0.110.2.dev1/tests/test_tutorial/test_path_operation_advanced_configurations/__init__.py
--rw-r--r--   0        0        0     1039 2024-05-12 00:15:11.799392 readyapi-0.110.2.dev1/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial001.py
--rw-r--r--   0        0        0     1022 2024-05-12 00:15:11.799392 readyapi-0.110.2.dev1/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial002.py
--rw-r--r--   0        0        0      577 2024-05-12 00:15:11.799392 readyapi-0.110.2.dev1/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial003.py
--rw-r--r--   0        0        0     8918 2024-05-12 00:15:11.799392 readyapi-0.110.2.dev1/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial004.py
--rw-r--r--   0        0        0     1036 2024-05-12 00:15:11.799392 readyapi-0.110.2.dev1/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial005.py
--rw-r--r--   0        0        0     1989 2024-05-12 00:15:11.799392 readyapi-0.110.2.dev1/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial006.py
--rw-r--r--   0        0        0     3421 2024-05-12 00:15:11.799392 readyapi-0.110.2.dev1/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial007.py
--rw-r--r--   0        0        0     3268 2024-05-12 00:15:11.799392 readyapi-0.110.2.dev1/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial007_pv1.py
--rw-r--r--   0        0        0        0 2024-05-12 00:15:11.799392 readyapi-0.110.2.dev1/tests/test_tutorial/test_path_operation_configurations/__init__.py
--rw-r--r--   0        0        0     1724 2024-05-12 00:15:11.799392 readyapi-0.110.2.dev1/tests/test_tutorial/test_path_operation_configurations/test_tutorial002b.py
--rw-r--r--   0        0        0     8903 2024-05-12 00:15:11.799392 readyapi-0.110.2.dev1/tests/test_tutorial/test_path_operation_configurations/test_tutorial005.py
--rw-r--r--   0        0        0     9105 2024-05-12 00:15:11.799392 readyapi-0.110.2.dev1/tests/test_tutorial/test_path_operation_configurations/test_tutorial005_py310.py
--rw-r--r--   0        0        0     9100 2024-05-12 00:15:11.799392 readyapi-0.110.2.dev1/tests/test_tutorial/test_path_operation_configurations/test_tutorial005_py39.py
--rw-r--r--   0        0        0     2407 2024-05-12 00:15:11.799392 readyapi-0.110.2.dev1/tests/test_tutorial/test_path_operation_configurations/test_tutorial006.py
--rw-r--r--   0        0        0        0 2024-05-12 00:15:11.799392 readyapi-0.110.2.dev1/tests/test_tutorial/test_path_params/__init__.py
--rw-r--r--   0        0        0     3371 2024-05-12 00:15:11.799392 readyapi-0.110.2.dev1/tests/test_tutorial/test_path_params/test_tutorial004.py
--rw-r--r--   0        0        0     5144 2024-05-12 00:15:11.799392 readyapi-0.110.2.dev1/tests/test_tutorial/test_path_params/test_tutorial005.py
--rw-r--r--   0        0        0        0 2024-05-12 00:15:11.799392 readyapi-0.110.2.dev1/tests/test_tutorial/test_query_params/__init__.py
--rw-r--r--   0        0        0     4074 2024-05-12 00:15:11.803392 readyapi-0.110.2.dev1/tests/test_tutorial/test_query_params/test_tutorial005.py
--rw-r--r--   0        0        0     6287 2024-05-12 00:15:11.803392 readyapi-0.110.2.dev1/tests/test_tutorial/test_query_params/test_tutorial006.py
--rw-r--r--   0        0        0     6366 2024-05-12 00:15:11.803392 readyapi-0.110.2.dev1/tests/test_tutorial/test_query_params/test_tutorial006_py310.py
--rw-r--r--   0        0        0        0 2024-05-12 00:15:11.803392 readyapi-0.110.2.dev1/tests/test_tutorial/test_query_params_str_validations/__init__.py
--rw-r--r--   0        0        0     6390 2024-05-12 00:15:11.803392 readyapi-0.110.2.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial010.py
--rw-r--r--   0        0        0     6393 2024-05-12 00:15:11.803392 readyapi-0.110.2.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial010_an.py
--rw-r--r--   0        0        0     6498 2024-05-12 00:15:11.803392 readyapi-0.110.2.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial010_an_py310.py
--rw-r--r--   0        0        0     6491 2024-05-12 00:15:11.803392 readyapi-0.110.2.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial010_an_py39.py
--rw-r--r--   0        0        0     6495 2024-05-12 00:15:11.803392 readyapi-0.110.2.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial010_py310.py
--rw-r--r--   0        0        0     4019 2024-05-12 00:15:11.803392 readyapi-0.110.2.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial011.py
--rw-r--r--   0        0        0     4022 2024-05-12 00:15:11.803392 readyapi-0.110.2.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial011_an.py
--rw-r--r--   0        0        0     4245 2024-05-12 00:15:11.803392 readyapi-0.110.2.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial011_an_py310.py
--rw-r--r--   0        0        0     4240 2024-05-12 00:15:11.803392 readyapi-0.110.2.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial011_an_py39.py
--rw-r--r--   0        0        0     4242 2024-05-12 00:15:11.803392 readyapi-0.110.2.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial011_py310.py
--rw-r--r--   0        0        0     4237 2024-05-12 00:15:11.803392 readyapi-0.110.2.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial011_py39.py
--rw-r--r--   0        0        0     3487 2024-05-12 00:15:11.803392 readyapi-0.110.2.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial012.py
--rw-r--r--   0        0        0     3490 2024-05-12 00:15:11.803392 readyapi-0.110.2.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial012_an.py
--rw-r--r--   0        0        0     3708 2024-05-12 00:15:11.803392 readyapi-0.110.2.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial012_an_py39.py
--rw-r--r--   0        0        0     3705 2024-05-12 00:15:11.803392 readyapi-0.110.2.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial012_py39.py
--rw-r--r--   0        0        0     3436 2024-05-12 00:15:11.803392 readyapi-0.110.2.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial013.py
--rw-r--r--   0        0        0     3439 2024-05-12 00:15:11.803392 readyapi-0.110.2.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial013_an.py
--rw-r--r--   0        0        0     3657 2024-05-12 00:15:11.803392 readyapi-0.110.2.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial013_an_py39.py
--rw-r--r--   0        0        0     2939 2024-05-12 00:15:11.803392 readyapi-0.110.2.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial014.py
--rw-r--r--   0        0        0     2942 2024-05-12 00:15:11.803392 readyapi-0.110.2.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial014_an.py
--rw-r--r--   0        0        0     3165 2024-05-12 00:15:11.803392 readyapi-0.110.2.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial014_an_py310.py
--rw-r--r--   0        0        0     3164 2024-05-12 00:15:11.803392 readyapi-0.110.2.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial014_an_py39.py
--rw-r--r--   0        0        0     3162 2024-05-12 00:15:11.803392 readyapi-0.110.2.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial014_py310.py
--rw-r--r--   0        0        0        0 2024-05-12 00:15:11.803392 readyapi-0.110.2.dev1/tests/test_tutorial/test_request_files/__init__.py
--rw-r--r--   0        0        0     7888 2024-05-12 00:15:11.803392 readyapi-0.110.2.dev1/tests/test_tutorial/test_request_files/test_tutorial001.py
--rw-r--r--   0        0        0     8390 2024-05-12 00:15:11.803392 readyapi-0.110.2.dev1/tests/test_tutorial/test_request_files/test_tutorial001_02.py
--rw-r--r--   0        0        0     8393 2024-05-12 00:15:11.803392 readyapi-0.110.2.dev1/tests/test_tutorial/test_request_files/test_tutorial001_02_an.py
--rw-r--r--   0        0        0     8662 2024-05-12 00:15:11.803392 readyapi-0.110.2.dev1/tests/test_tutorial/test_request_files/test_tutorial001_02_an_py310.py
--rw-r--r--   0        0        0     8655 2024-05-12 00:15:11.803392 readyapi-0.110.2.dev1/tests/test_tutorial/test_request_files/test_tutorial001_02_an_py39.py
--rw-r--r--   0        0        0     8659 2024-05-12 00:15:11.803392 readyapi-0.110.2.dev1/tests/test_tutorial/test_request_files/test_tutorial001_02_py310.py
--rw-r--r--   0        0        0     6135 2024-05-12 00:15:11.803392 readyapi-0.110.2.dev1/tests/test_tutorial/test_request_files/test_tutorial001_03.py
--rw-r--r--   0        0        0     6138 2024-05-12 00:15:11.803392 readyapi-0.110.2.dev1/tests/test_tutorial/test_request_files/test_tutorial001_03_an.py
--rw-r--r--   0        0        0     6302 2024-05-12 00:15:11.803392 readyapi-0.110.2.dev1/tests/test_tutorial/test_request_files/test_tutorial001_03_an_py39.py
--rw-r--r--   0        0        0     7710 2024-05-12 00:15:11.803392 readyapi-0.110.2.dev1/tests/test_tutorial/test_request_files/test_tutorial001_an.py
--rw-r--r--   0        0        0     7937 2024-05-12 00:15:11.803392 readyapi-0.110.2.dev1/tests/test_tutorial/test_request_files/test_tutorial001_an_py39.py
--rw-r--r--   0        0        0     8681 2024-05-12 00:15:11.803392 readyapi-0.110.2.dev1/tests/test_tutorial/test_request_files/test_tutorial002.py
--rw-r--r--   0        0        0     8684 2024-05-12 00:15:11.803392 readyapi-0.110.2.dev1/tests/test_tutorial/test_request_files/test_tutorial002_an.py
--rw-r--r--   0        0        0     9084 2024-05-12 00:15:11.803392 readyapi-0.110.2.dev1/tests/test_tutorial/test_request_files/test_tutorial002_an_py39.py
--rw-r--r--   0        0        0     9263 2024-05-12 00:15:11.803392 readyapi-0.110.2.dev1/tests/test_tutorial/test_request_files/test_tutorial002_py39.py
--rw-r--r--   0        0        0     7313 2024-05-12 00:15:11.803392 readyapi-0.110.2.dev1/tests/test_tutorial/test_request_files/test_tutorial003.py
--rw-r--r--   0        0        0     7316 2024-05-12 00:15:11.803392 readyapi-0.110.2.dev1/tests/test_tutorial/test_request_files/test_tutorial003_an.py
--rw-r--r--   0        0        0     7838 2024-05-12 00:15:11.803392 readyapi-0.110.2.dev1/tests/test_tutorial/test_request_files/test_tutorial003_an_py39.py
--rw-r--r--   0        0        0     7835 2024-05-12 00:15:11.803392 readyapi-0.110.2.dev1/tests/test_tutorial/test_request_files/test_tutorial003_py39.py
--rw-r--r--   0        0        0        0 2024-05-12 00:15:11.803392 readyapi-0.110.2.dev1/tests/test_tutorial/test_request_forms/__init__.py
--rw-r--r--   0        0        0     7632 2024-05-12 00:15:11.803392 readyapi-0.110.2.dev1/tests/test_tutorial/test_request_forms/test_tutorial001.py
--rw-r--r--   0        0        0     7635 2024-05-12 00:15:11.803392 readyapi-0.110.2.dev1/tests/test_tutorial/test_request_forms/test_tutorial001_an.py
--rw-r--r--   0        0        0     7745 2024-05-12 00:15:11.803392 readyapi-0.110.2.dev1/tests/test_tutorial/test_request_forms/test_tutorial001_an_py39.py
--rw-r--r--   0        0        0        0 2024-05-12 00:15:11.803392 readyapi-0.110.2.dev1/tests/test_tutorial/test_request_forms_and_files/__init__.py
--rw-r--r--   0        0        0    10049 2024-05-12 00:15:11.803392 readyapi-0.110.2.dev1/tests/test_tutorial/test_request_forms_and_files/test_tutorial001.py
--rw-r--r--   0        0        0    10052 2024-05-12 00:15:11.803392 readyapi-0.110.2.dev1/tests/test_tutorial/test_request_forms_and_files/test_tutorial001_an.py
--rw-r--r--   0        0        0    10162 2024-05-12 00:15:11.803392 readyapi-0.110.2.dev1/tests/test_tutorial/test_request_forms_and_files/test_tutorial001_an_py39.py
--rw-r--r--   0        0        0        0 2024-05-12 00:15:11.803392 readyapi-0.110.2.dev1/tests/test_tutorial/test_response_change_status_code/__init__.py
--rw-r--r--   0        0        0      522 2024-05-12 00:15:11.803392 readyapi-0.110.2.dev1/tests/test_tutorial/test_response_change_status_code/test_tutorial001.py
--rw-r--r--   0        0        0        0 2024-05-12 00:15:11.803392 readyapi-0.110.2.dev1/tests/test_tutorial/test_response_cookies/__init__.py
--rw-r--r--   0        0        0      404 2024-05-12 00:15:11.803392 readyapi-0.110.2.dev1/tests/test_tutorial/test_response_cookies/test_tutorial001.py
--rw-r--r--   0        0        0      415 2024-05-12 00:15:11.803392 readyapi-0.110.2.dev1/tests/test_tutorial/test_response_cookies/test_tutorial002.py
--rw-r--r--   0        0        0        0 2024-05-12 00:15:11.803392 readyapi-0.110.2.dev1/tests/test_tutorial/test_response_headers/__init__.py
--rw-r--r--   0        0        0      427 2024-05-12 00:15:11.803392 readyapi-0.110.2.dev1/tests/test_tutorial/test_response_headers/test_tutorial001.py
--rw-r--r--   0        0        0      379 2024-05-12 00:15:11.803392 readyapi-0.110.2.dev1/tests/test_tutorial/test_response_headers/test_tutorial002.py
--rw-r--r--   0        0        0        0 2024-05-12 00:15:11.803392 readyapi-0.110.2.dev1/tests/test_tutorial/test_response_model/__init__.py
--rw-r--r--   0        0        0     5766 2024-05-12 00:15:11.803392 readyapi-0.110.2.dev1/tests/test_tutorial/test_response_model/test_tutorial003.py
--rw-r--r--   0        0        0     5772 2024-05-12 00:15:11.803392 readyapi-0.110.2.dev1/tests/test_tutorial/test_response_model/test_tutorial003_01.py
--rw-r--r--   0        0        0     5964 2024-05-12 00:15:11.803392 readyapi-0.110.2.dev1/tests/test_tutorial/test_response_model/test_tutorial003_01_py310.py
--rw-r--r--   0        0        0     3478 2024-05-12 00:15:11.803392 readyapi-0.110.2.dev1/tests/test_tutorial/test_response_model/test_tutorial003_02.py
--rw-r--r--   0        0        0     1092 2024-05-12 00:15:11.803392 readyapi-0.110.2.dev1/tests/test_tutorial/test_response_model/test_tutorial003_03.py
--rw-r--r--   0        0        0      239 2024-05-12 00:15:11.803392 readyapi-0.110.2.dev1/tests/test_tutorial/test_response_model/test_tutorial003_04.py
--rw-r--r--   0        0        0      292 2024-05-12 00:15:11.803392 readyapi-0.110.2.dev1/tests/test_tutorial/test_response_model/test_tutorial003_04_py310.py
--rw-r--r--   0        0        0     3478 2024-05-12 00:15:11.803392 readyapi-0.110.2.dev1/tests/test_tutorial/test_response_model/test_tutorial003_05.py
--rw-r--r--   0        0        0     3701 2024-05-12 00:15:11.803392 readyapi-0.110.2.dev1/tests/test_tutorial/test_response_model/test_tutorial003_05_py310.py
--rw-r--r--   0        0        0     5958 2024-05-12 00:15:11.803392 readyapi-0.110.2.dev1/tests/test_tutorial/test_response_model/test_tutorial003_py310.py
--rw-r--r--   0        0        0     5110 2024-05-12 00:15:11.803392 readyapi-0.110.2.dev1/tests/test_tutorial/test_response_model/test_tutorial004.py
--rw-r--r--   0        0        0     5290 2024-05-12 00:15:11.803392 readyapi-0.110.2.dev1/tests/test_tutorial/test_response_model/test_tutorial004_py310.py
--rw-r--r--   0        0        0     5286 2024-05-12 00:15:11.803392 readyapi-0.110.2.dev1/tests/test_tutorial/test_response_model/test_tutorial004_py39.py
--rw-r--r--   0        0        0     6156 2024-05-12 00:15:11.803392 readyapi-0.110.2.dev1/tests/test_tutorial/test_response_model/test_tutorial005.py
--rw-r--r--   0        0        0     6379 2024-05-12 00:15:11.803392 readyapi-0.110.2.dev1/tests/test_tutorial/test_response_model/test_tutorial005_py310.py
--rw-r--r--   0        0        0     6156 2024-05-12 00:15:11.803392 readyapi-0.110.2.dev1/tests/test_tutorial/test_response_model/test_tutorial006.py
--rw-r--r--   0        0        0     6379 2024-05-12 00:15:11.803392 readyapi-0.110.2.dev1/tests/test_tutorial/test_response_model/test_tutorial006_py310.py
--rw-r--r--   0        0        0        0 2024-05-12 00:15:11.803392 readyapi-0.110.2.dev1/tests/test_tutorial/test_schema_extra_example/__init__.py
--rw-r--r--   0        0        0     4781 2024-05-12 00:15:11.803392 readyapi-0.110.2.dev1/tests/test_tutorial/test_schema_extra_example/test_tutorial001.py
--rw-r--r--   0        0        0     4557 2024-05-12 00:15:11.803392 readyapi-0.110.2.dev1/tests/test_tutorial/test_schema_extra_example/test_tutorial001_pv1.py
--rw-r--r--   0        0        0     4826 2024-05-12 00:15:11.803392 readyapi-0.110.2.dev1/tests/test_tutorial/test_schema_extra_example/test_tutorial001_py310.py
--rw-r--r--   0        0        0     4602 2024-05-12 00:15:11.803392 readyapi-0.110.2.dev1/tests/test_tutorial/test_schema_extra_example/test_tutorial001_py310_pv1.py
--rw-r--r--   0        0        0     7062 2024-05-12 00:15:11.807392 readyapi-0.110.2.dev1/tests/test_tutorial/test_schema_extra_example/test_tutorial004.py
--rw-r--r--   0        0        0     7065 2024-05-12 00:15:11.807392 readyapi-0.110.2.dev1/tests/test_tutorial/test_schema_extra_example/test_tutorial004_an.py
--rw-r--r--   0        0        0     7257 2024-05-12 00:15:11.807392 readyapi-0.110.2.dev1/tests/test_tutorial/test_schema_extra_example/test_tutorial004_an_py310.py
--rw-r--r--   0        0        0     7253 2024-05-12 00:15:11.807392 readyapi-0.110.2.dev1/tests/test_tutorial/test_schema_extra_example/test_tutorial004_an_py39.py
--rw-r--r--   0        0        0     7254 2024-05-12 00:15:11.807392 readyapi-0.110.2.dev1/tests/test_tutorial/test_schema_extra_example/test_tutorial004_py310.py
--rw-r--r--   0        0        0     6910 2024-05-12 00:15:11.807392 readyapi-0.110.2.dev1/tests/test_tutorial/test_schema_extra_example/test_tutorial005.py
--rw-r--r--   0        0        0     6913 2024-05-12 00:15:11.807392 readyapi-0.110.2.dev1/tests/test_tutorial/test_schema_extra_example/test_tutorial005_an.py
--rw-r--r--   0        0        0     6979 2024-05-12 00:15:11.807392 readyapi-0.110.2.dev1/tests/test_tutorial/test_schema_extra_example/test_tutorial005_an_py310.py
--rw-r--r--   0        0        0     6975 2024-05-12 00:15:11.807392 readyapi-0.110.2.dev1/tests/test_tutorial/test_schema_extra_example/test_tutorial005_an_py39.py
--rw-r--r--   0        0        0     6976 2024-05-12 00:15:11.807392 readyapi-0.110.2.dev1/tests/test_tutorial/test_schema_extra_example/test_tutorial005_py310.py
--rw-r--r--   0        0        0        0 2024-05-12 00:15:11.807392 readyapi-0.110.2.dev1/tests/test_tutorial/test_security/__init__.py
--rw-r--r--   0        0        0     1907 2024-05-12 00:15:11.807392 readyapi-0.110.2.dev1/tests/test_tutorial/test_security/test_tutorial001.py
--rw-r--r--   0        0        0     1910 2024-05-12 00:15:11.807392 readyapi-0.110.2.dev1/tests/test_tutorial/test_security/test_tutorial001_an.py
--rw-r--r--   0        0        0     2158 2024-05-12 00:15:11.807392 readyapi-0.110.2.dev1/tests/test_tutorial/test_security/test_tutorial001_an_py39.py
--rw-r--r--   0        0        0     8184 2024-05-12 00:15:11.807392 readyapi-0.110.2.dev1/tests/test_tutorial/test_security/test_tutorial003.py
--rw-r--r--   0        0        0     8187 2024-05-12 00:15:11.807392 readyapi-0.110.2.dev1/tests/test_tutorial/test_security/test_tutorial003_an.py
--rw-r--r--   0        0        0     8596 2024-05-12 00:15:11.807392 readyapi-0.110.2.dev1/tests/test_tutorial/test_security/test_tutorial003_an_py310.py
--rw-r--r--   0        0        0     8585 2024-05-12 00:15:11.807392 readyapi-0.110.2.dev1/tests/test_tutorial/test_security/test_tutorial003_an_py39.py
--rw-r--r--   0        0        0     8593 2024-05-12 00:15:11.807392 readyapi-0.110.2.dev1/tests/test_tutorial/test_security/test_tutorial003_py310.py
--rw-r--r--   0        0        0    15805 2024-05-12 00:15:11.807392 readyapi-0.110.2.dev1/tests/test_tutorial/test_security/test_tutorial005.py
--rw-r--r--   0        0        0    15808 2024-05-12 00:15:11.807392 readyapi-0.110.2.dev1/tests/test_tutorial/test_security/test_tutorial005_an.py
--rw-r--r--   0        0        0    16713 2024-05-12 00:15:11.807392 readyapi-0.110.2.dev1/tests/test_tutorial/test_security/test_tutorial005_an_py310.py
--rw-r--r--   0        0        0    16689 2024-05-12 00:15:11.807392 readyapi-0.110.2.dev1/tests/test_tutorial/test_security/test_tutorial005_an_py39.py
--rw-r--r--   0        0        0    16701 2024-05-12 00:15:11.807392 readyapi-0.110.2.dev1/tests/test_tutorial/test_security/test_tutorial005_py310.py
--rw-r--r--   0        0        0    16677 2024-05-12 00:15:11.807392 readyapi-0.110.2.dev1/tests/test_tutorial/test_security/test_tutorial005_py39.py
--rw-r--r--   0        0        0     2320 2024-05-12 00:15:11.807392 readyapi-0.110.2.dev1/tests/test_tutorial/test_security/test_tutorial006.py
--rw-r--r--   0        0        0     2323 2024-05-12 00:15:11.807392 readyapi-0.110.2.dev1/tests/test_tutorial/test_security/test_tutorial006_an.py
--rw-r--r--   0        0        0     2596 2024-05-12 00:15:11.807392 readyapi-0.110.2.dev1/tests/test_tutorial/test_security/test_tutorial006_an_py39.py
--rw-r--r--   0        0        0        0 2024-05-12 00:15:11.807392 readyapi-0.110.2.dev1/tests/test_tutorial/test_separate_openapi_schemas/__init__.py
--rw-r--r--   0        0        0     4960 2024-05-12 00:15:11.807392 readyapi-0.110.2.dev1/tests/test_tutorial/test_separate_openapi_schemas/test_tutorial001.py
--rw-r--r--   0        0        0     5018 2024-05-12 00:15:11.807392 readyapi-0.110.2.dev1/tests/test_tutorial/test_separate_openapi_schemas/test_tutorial001_py310.py
--rw-r--r--   0        0        0     5013 2024-05-12 00:15:11.807392 readyapi-0.110.2.dev1/tests/test_tutorial/test_separate_openapi_schemas/test_tutorial001_py39.py
--rw-r--r--   0        0        0     4960 2024-05-12 00:15:11.807392 readyapi-0.110.2.dev1/tests/test_tutorial/test_separate_openapi_schemas/test_tutorial002.py
--rw-r--r--   0        0        0     5018 2024-05-12 00:15:11.807392 readyapi-0.110.2.dev1/tests/test_tutorial/test_separate_openapi_schemas/test_tutorial002_py310.py
--rw-r--r--   0        0        0     5013 2024-05-12 00:15:11.807392 readyapi-0.110.2.dev1/tests/test_tutorial/test_separate_openapi_schemas/test_tutorial002_py39.py
--rw-r--r--   0        0        0        0 2024-05-12 00:15:11.807392 readyapi-0.110.2.dev1/tests/test_tutorial/test_settings/__init__.py
--rw-r--r--   0        0        0      488 2024-05-12 00:15:11.807392 readyapi-0.110.2.dev1/tests/test_tutorial/test_settings/test_app02.py
--rw-r--r--   0        0        0      553 2024-05-12 00:15:11.807392 readyapi-0.110.2.dev1/tests/test_tutorial/test_settings/test_tutorial001.py
--rw-r--r--   0        0        0      557 2024-05-12 00:15:11.807392 readyapi-0.110.2.dev1/tests/test_tutorial/test_settings/test_tutorial001_pv1.py
--rw-r--r--   0        0        0        0 2024-05-12 00:15:11.807392 readyapi-0.110.2.dev1/tests/test_tutorial/test_sql_databases/__init__.py
--rw-r--r--   0        0        0    16477 2024-05-12 00:15:11.807392 readyapi-0.110.2.dev1/tests/test_tutorial/test_sql_databases/test_sql_databases.py
--rw-r--r--   0        0        0    16656 2024-05-12 00:15:11.807392 readyapi-0.110.2.dev1/tests/test_tutorial/test_sql_databases/test_sql_databases_middleware.py
--rw-r--r--   0        0        0    16926 2024-05-12 00:15:11.807392 readyapi-0.110.2.dev1/tests/test_tutorial/test_sql_databases/test_sql_databases_middleware_py310.py
--rw-r--r--   0        0        0    16927 2024-05-12 00:15:11.807392 readyapi-0.110.2.dev1/tests/test_tutorial/test_sql_databases/test_sql_databases_middleware_py39.py
--rw-r--r--   0        0        0    16932 2024-05-12 00:15:11.807392 readyapi-0.110.2.dev1/tests/test_tutorial/test_sql_databases/test_sql_databases_py310.py
--rw-r--r--   0        0        0    16923 2024-05-12 00:15:11.807392 readyapi-0.110.2.dev1/tests/test_tutorial/test_sql_databases/test_sql_databases_py39.py
--rw-r--r--   0        0        0      788 2024-05-12 00:15:11.807392 readyapi-0.110.2.dev1/tests/test_tutorial/test_sql_databases/test_testing_databases.py
--rw-r--r--   0        0        0      825 2024-05-12 00:15:11.807392 readyapi-0.110.2.dev1/tests/test_tutorial/test_sql_databases/test_testing_databases_py310.py
--rw-r--r--   0        0        0      822 2024-05-12 00:15:11.807392 readyapi-0.110.2.dev1/tests/test_tutorial/test_sql_databases/test_testing_databases_py39.py
--rw-r--r--   0        0        0        0 2024-05-12 00:15:11.807392 readyapi-0.110.2.dev1/tests/test_tutorial/test_sub_applications/__init__.py
--rw-r--r--   0        0        0     1923 2024-05-12 00:15:11.807392 readyapi-0.110.2.dev1/tests/test_tutorial/test_sub_applications/test_tutorial001.py
--rw-r--r--   0        0        0        0 2024-05-12 00:15:11.807392 readyapi-0.110.2.dev1/tests/test_tutorial/test_templates/__init__.py
--rw-r--r--   0        0        0      911 2024-05-12 00:15:11.807392 readyapi-0.110.2.dev1/tests/test_tutorial/test_templates/test_tutorial001.py
--rw-r--r--   0        0        0        0 2024-05-12 00:15:11.807392 readyapi-0.110.2.dev1/tests/test_tutorial/test_testing/__init__.py
--rw-r--r--   0        0        0      820 2024-05-12 00:15:11.807392 readyapi-0.110.2.dev1/tests/test_tutorial/test_testing/test_main.py
--rw-r--r--   0        0        0      300 2024-05-12 00:15:11.807392 readyapi-0.110.2.dev1/tests/test_tutorial/test_testing/test_main_b.py
--rw-r--r--   0        0        0      303 2024-05-12 00:15:11.807392 readyapi-0.110.2.dev1/tests/test_tutorial/test_testing/test_main_b_an.py
--rw-r--r--   0        0        0      360 2024-05-12 00:15:11.807392 readyapi-0.110.2.dev1/tests/test_tutorial/test_testing/test_main_b_an_py310.py
--rw-r--r--   0        0        0      357 2024-05-12 00:15:11.807392 readyapi-0.110.2.dev1/tests/test_tutorial/test_testing/test_main_b_an_py39.py
--rw-r--r--   0        0        0      357 2024-05-12 00:15:11.807392 readyapi-0.110.2.dev1/tests/test_tutorial/test_testing/test_main_b_py310.py
--rw-r--r--   0        0        0      822 2024-05-12 00:15:11.807392 readyapi-0.110.2.dev1/tests/test_tutorial/test_testing/test_tutorial001.py
--rw-r--r--   0        0        0      154 2024-05-12 00:15:11.807392 readyapi-0.110.2.dev1/tests/test_tutorial/test_testing/test_tutorial002.py
--rw-r--r--   0        0        0      167 2024-05-12 00:15:11.807392 readyapi-0.110.2.dev1/tests/test_tutorial/test_testing/test_tutorial003.py
--rw-r--r--   0        0        0        0 2024-05-12 00:15:11.807392 readyapi-0.110.2.dev1/tests/test_tutorial/test_testing_dependencies/__init__.py
--rw-r--r--   0        0        0     1527 2024-05-12 00:15:11.807392 readyapi-0.110.2.dev1/tests/test_tutorial/test_testing_dependencies/test_tutorial001.py
--rw-r--r--   0        0        0     1530 2024-05-12 00:15:11.807392 readyapi-0.110.2.dev1/tests/test_tutorial/test_testing_dependencies/test_tutorial001_an.py
--rw-r--r--   0        0        0     2088 2024-05-12 00:15:11.807392 readyapi-0.110.2.dev1/tests/test_tutorial/test_testing_dependencies/test_tutorial001_an_py310.py
--rw-r--r--   0        0        0     2073 2024-05-12 00:15:11.807392 readyapi-0.110.2.dev1/tests/test_tutorial/test_testing_dependencies/test_tutorial001_an_py39.py
--rw-r--r--   0        0        0     2067 2024-05-12 00:15:11.807392 readyapi-0.110.2.dev1/tests/test_tutorial/test_testing_dependencies/test_tutorial001_py310.py
--rw-r--r--   0        0        0        0 2024-05-12 00:15:11.807392 readyapi-0.110.2.dev1/tests/test_tutorial/test_websockets/__init__.py
--rw-r--r--   0        0        0      824 2024-05-12 00:15:11.807392 readyapi-0.110.2.dev1/tests/test_tutorial/test_websockets/test_tutorial001.py
--rw-r--r--   0        0        0     3685 2024-05-12 00:15:11.807392 readyapi-0.110.2.dev1/tests/test_tutorial/test_websockets/test_tutorial002.py
--rw-r--r--   0        0        0     3688 2024-05-12 00:15:11.807392 readyapi-0.110.2.dev1/tests/test_tutorial/test_websockets/test_tutorial002_an.py
--rw-r--r--   0        0        0     3978 2024-05-12 00:15:11.807392 readyapi-0.110.2.dev1/tests/test_tutorial/test_websockets/test_tutorial002_an_py310.py
--rw-r--r--   0        0        0     3970 2024-05-12 00:15:11.807392 readyapi-0.110.2.dev1/tests/test_tutorial/test_websockets/test_tutorial002_an_py39.py
--rw-r--r--   0        0        0     3975 2024-05-12 00:15:11.807392 readyapi-0.110.2.dev1/tests/test_tutorial/test_websockets/test_tutorial002_py310.py
--rw-r--r--   0        0        0      873 2024-05-12 00:15:11.807392 readyapi-0.110.2.dev1/tests/test_tutorial/test_websockets/test_tutorial003.py
--rw-r--r--   0        0        0     1292 2024-05-12 00:15:11.807392 readyapi-0.110.2.dev1/tests/test_tutorial/test_websockets/test_tutorial003_py39.py
--rw-r--r--   0        0        0        0 2024-05-12 00:15:11.807392 readyapi-0.110.2.dev1/tests/test_tutorial/test_wsgi/__init__.py
--rw-r--r--   0        0        0      437 2024-05-12 00:15:11.807392 readyapi-0.110.2.dev1/tests/test_tutorial/test_wsgi/test_tutorial001.py
--rw-r--r--   0        0        0      713 2024-05-12 00:15:11.807392 readyapi-0.110.2.dev1/tests/test_typing_python39.py
--rw-r--r--   0        0        0     4753 2024-05-12 00:15:11.807392 readyapi-0.110.2.dev1/tests/test_union_body.py
--rw-r--r--   0        0        0     5316 2024-05-12 00:15:11.807392 readyapi-0.110.2.dev1/tests/test_union_inherited_body.py
--rw-r--r--   0        0        0     2036 2024-05-12 00:15:11.807392 readyapi-0.110.2.dev1/tests/test_validate_response.py
--rw-r--r--   0        0        0     1213 2024-05-12 00:15:11.807392 readyapi-0.110.2.dev1/tests/test_validate_response_dataclass.py
--rw-r--r--   0        0        0        0 2024-05-12 00:15:11.807392 readyapi-0.110.2.dev1/tests/test_validate_response_recursive/__init__.py
--rw-r--r--   0        0        0     1152 2024-05-12 00:15:11.807392 readyapi-0.110.2.dev1/tests/test_validate_response_recursive/app_pv1.py
--rw-r--r--   0        0        0     1181 2024-05-12 00:15:11.807392 readyapi-0.110.2.dev1/tests/test_validate_response_recursive/app_pv2.py
--rw-r--r--   0        0        0      901 2024-05-12 00:15:11.807392 readyapi-0.110.2.dev1/tests/test_validate_response_recursive/test_validate_response_recursive_pv1.py
--rw-r--r--   0        0        0      901 2024-05-12 00:15:11.807392 readyapi-0.110.2.dev1/tests/test_validate_response_recursive/test_validate_response_recursive_pv2.py
--rw-r--r--   0        0        0     4673 2024-05-12 00:15:11.811392 readyapi-0.110.2.dev1/tests/test_webhooks_security.py
--rw-r--r--   0        0        0     2203 2024-05-12 00:15:11.811392 readyapi-0.110.2.dev1/tests/test_ws_dependencies.py
--rw-r--r--   0        0        0     7657 2024-05-12 00:15:11.811392 readyapi-0.110.2.dev1/tests/test_ws_router.py
--rw-r--r--   0        0        0      423 2024-05-12 00:15:11.811392 readyapi-0.110.2.dev1/tests/utils.py
--rw-r--r--   0        0        0    25449 1970-01-01 00:00:00.000000 readyapi-0.110.2.dev1/PKG-INFO
+-rw-r--r--   0        0        0     1084 2024-05-12 00:38:13.574838 readyapi-0.110.3/LICENSE
+-rw-r--r--   0        0        0    22670 2024-05-12 00:38:13.578838 readyapi-0.110.3/README.md
+-rw-r--r--   0        0        0     5043 2024-05-12 00:38:13.610839 readyapi-0.110.3/docs/en/docs/img/favicon.png
+-rw-r--r--   0        0        0      510 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/additional_responses/tutorial001.py
+-rw-r--r--   0        0        0      632 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/additional_responses/tutorial002.py
+-rw-r--r--   0        0        0      841 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/additional_responses/tutorial003.py
+-rw-r--r--   0        0        0      705 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/additional_responses/tutorial004.py
+-rw-r--r--   0        0        0      688 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/additional_status_codes/tutorial001.py
+-rw-r--r--   0        0        0      738 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/additional_status_codes/tutorial001_an.py
+-rw-r--r--   0        0        0      690 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/additional_status_codes/tutorial001_an_py310.py
+-rw-r--r--   0        0        0      709 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/additional_status_codes/tutorial001_an_py39.py
+-rw-r--r--   0        0        0      650 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/additional_status_codes/tutorial001_py310.py
+-rw-r--r--   0        0        0      235 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/advanced_middleware/tutorial001.py
+-rw-r--r--   0        0        0      283 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/advanced_middleware/tutorial002.py
+-rw-r--r--   0        0        0      217 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/advanced_middleware/tutorial003.py
+-rw-r--r--   0        0        0        0 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/app_testing/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/app_testing/app_b/__init__.py
+-rw-r--r--   0        0        0     1148 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/app_testing/app_b/main.py
+-rw-r--r--   0        0        0     1867 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/app_testing/app_b/test_main.py
+-rw-r--r--   0        0        0        0 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/app_testing/app_b_an/__init__.py
+-rw-r--r--   0        0        0     1208 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/app_testing/app_b_an/main.py
+-rw-r--r--   0        0        0     1867 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/app_testing/app_b_an/test_main.py
+-rw-r--r--   0        0        0        0 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/app_testing/app_b_an_py310/__init__.py
+-rw-r--r--   0        0        0     1166 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/app_testing/app_b_an_py310/main.py
+-rw-r--r--   0        0        0     1867 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/app_testing/app_b_an_py310/test_main.py
+-rw-r--r--   0        0        0        0 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/app_testing/app_b_an_py39/__init__.py
+-rw-r--r--   0        0        0     1179 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/app_testing/app_b_an_py39/main.py
+-rw-r--r--   0        0        0     1867 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/app_testing/app_b_an_py39/test_main.py
+-rw-r--r--   0        0        0        0 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/app_testing/app_b_py310/__init__.py
+-rw-r--r--   0        0        0     1116 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/app_testing/app_b_py310/main.py
+-rw-r--r--   0        0        0     1867 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/app_testing/app_b_py310/test_main.py
+-rw-r--r--   0        0        0      121 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/app_testing/main.py
+-rw-r--r--   0        0        0      239 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/app_testing/test_main.py
+-rw-r--r--   0        0        0      338 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/app_testing/tutorial001.py
+-rw-r--r--   0        0        0      762 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/app_testing/tutorial002.py
+-rw-r--r--   0        0        0      532 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/app_testing/tutorial003.py
+-rw-r--r--   0        0        0     1418 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/async_sql_databases/tutorial001.py
+-rw-r--r--   0        0        0        0 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/async_tests/__init__.py
+-rw-r--r--   0        0        0      115 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/async_tests/main.py
+-rw-r--r--   0        0        0      306 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/async_tests/test_main.py
+-rw-r--r--   0        0        0      522 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/background_tasks/tutorial001.py
+-rw-r--r--   0        0        0      678 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/background_tasks/tutorial002.py
+-rw-r--r--   0        0        0      728 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/background_tasks/tutorial002_an.py
+-rw-r--r--   0        0        0      686 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/background_tasks/tutorial002_an_py310.py
+-rw-r--r--   0        0        0      699 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/background_tasks/tutorial002_an_py39.py
+-rw-r--r--   0        0        0      646 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/background_tasks/tutorial002_py310.py
+-rw-r--r--   0        0        0      192 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/behind_a_proxy/tutorial001.py
+-rw-r--r--   0        0        0      211 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/behind_a_proxy/tutorial002.py
+-rw-r--r--   0        0        0      408 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/behind_a_proxy/tutorial003.py
+-rw-r--r--   0        0        0      440 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/behind_a_proxy/tutorial004.py
+-rw-r--r--   0        0        0        0 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/bigger_applications/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/bigger_applications/app/__init__.py
+-rw-r--r--   0        0        0      370 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/bigger_applications/app/dependencies.py
+-rw-r--r--   0        0        0        0 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/bigger_applications/app/internal/__init__.py
+-rw-r--r--   0        0        0      148 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/bigger_applications/app/internal/admin.py
+-rw-r--r--   0        0        0      555 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/bigger_applications/app/main.py
+-rw-r--r--   0        0        0        0 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/bigger_applications/app/routers/__init__.py
+-rw-r--r--   0        0        0     1012 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/bigger_applications/app/routers/items.py
+-rw-r--r--   0        0        0      408 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/bigger_applications/app/routers/users.py
+-rw-r--r--   0        0        0        0 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/bigger_applications/app_an/__init__.py
+-rw-r--r--   0        0        0      420 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/bigger_applications/app_an/dependencies.py
+-rw-r--r--   0        0        0        0 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/bigger_applications/app_an/internal/__init__.py
+-rw-r--r--   0        0        0      148 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/bigger_applications/app_an/internal/admin.py
+-rw-r--r--   0        0        0      555 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/bigger_applications/app_an/main.py
+-rw-r--r--   0        0        0        0 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/bigger_applications/app_an/routers/__init__.py
+-rw-r--r--   0        0        0     1012 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/bigger_applications/app_an/routers/items.py
+-rw-r--r--   0        0        0      408 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/bigger_applications/app_an/routers/users.py
+-rw-r--r--   0        0        0        0 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/bigger_applications/app_an_py39/__init__.py
+-rw-r--r--   0        0        0      410 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/bigger_applications/app_an_py39/dependencies.py
+-rw-r--r--   0        0        0        0 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/bigger_applications/app_an_py39/internal/__init__.py
+-rw-r--r--   0        0        0      148 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/bigger_applications/app_an_py39/internal/admin.py
+-rw-r--r--   0        0        0      555 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/bigger_applications/app_an_py39/main.py
+-rw-r--r--   0        0        0        0 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/bigger_applications/app_an_py39/routers/__init__.py
+-rw-r--r--   0        0        0     1012 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/bigger_applications/app_an_py39/routers/items.py
+-rw-r--r--   0        0        0      408 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/bigger_applications/app_an_py39/routers/users.py
+-rw-r--r--   0        0        0      312 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/body/tutorial001.py
+-rw-r--r--   0        0        0      274 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/body/tutorial001_py310.py
+-rw-r--r--   0        0        0      470 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/body/tutorial002.py
+-rw-r--r--   0        0        0      432 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/body/tutorial002_py310.py
+-rw-r--r--   0        0        0      365 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/body/tutorial003.py
+-rw-r--r--   0        0        0      327 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/body/tutorial003_py310.py
+-rw-r--r--   0        0        0      455 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/body/tutorial004.py
+-rw-r--r--   0        0        0      411 2024-05-12 00:38:13.698840 readyapi-0.110.3/docs_src/body/tutorial004_py310.py
+-rw-r--r--   0        0        0      564 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/body_fields/tutorial001.py
+-rw-r--r--   0        0        0      614 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/body_fields/tutorial001_an.py
+-rw-r--r--   0        0        0      566 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/body_fields/tutorial001_an_py310.py
+-rw-r--r--   0        0        0      585 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/body_fields/tutorial001_an_py39.py
+-rw-r--r--   0        0        0      526 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/body_fields/tutorial001_py310.py
+-rw-r--r--   0        0        0      599 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/body_multiple_params/tutorial001.py
+-rw-r--r--   0        0        0      642 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/body_multiple_params/tutorial001_an.py
+-rw-r--r--   0        0        0      582 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/body_multiple_params/tutorial001_an_py310.py
+-rw-r--r--   0        0        0      613 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/body_multiple_params/tutorial001_an_py39.py
+-rw-r--r--   0        0        0      549 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/body_multiple_params/tutorial001_py310.py
+-rw-r--r--   0        0        0      493 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/body_multiple_params/tutorial002.py
+-rw-r--r--   0        0        0      449 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/body_multiple_params/tutorial002_py310.py
+-rw-r--r--   0        0        0      551 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/body_multiple_params/tutorial003.py
+-rw-r--r--   0        0        0      607 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/body_multiple_params/tutorial003_an.py
+-rw-r--r--   0        0        0      553 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/body_multiple_params/tutorial003_an_py310.py
+-rw-r--r--   0        0        0      578 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/body_multiple_params/tutorial003_an_py39.py
+-rw-r--r--   0        0        0      507 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/body_multiple_params/tutorial003_py310.py
+-rw-r--r--   0        0        0      656 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/body_multiple_params/tutorial004.py
+-rw-r--r--   0        0        0      706 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/body_multiple_params/tutorial004_an.py
+-rw-r--r--   0        0        0      646 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/body_multiple_params/tutorial004_an_py310.py
+-rw-r--r--   0        0        0      677 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/body_multiple_params/tutorial004_an_py39.py
+-rw-r--r--   0        0        0      606 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/body_multiple_params/tutorial004_py310.py
+-rw-r--r--   0        0        0      410 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/body_multiple_params/tutorial005.py
+-rw-r--r--   0        0        0      460 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/body_multiple_params/tutorial005_an.py
+-rw-r--r--   0        0        0      412 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/body_multiple_params/tutorial005_an_py310.py
+-rw-r--r--   0        0        0      431 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/body_multiple_params/tutorial005_an_py39.py
+-rw-r--r--   0        0        0      372 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/body_multiple_params/tutorial005_py310.py
+-rw-r--r--   0        0        0      405 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/body_nested_models/tutorial001.py
+-rw-r--r--   0        0        0      367 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/body_nested_models/tutorial001_py310.py
+-rw-r--r--   0        0        0      416 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/body_nested_models/tutorial002.py
+-rw-r--r--   0        0        0      372 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/body_nested_models/tutorial002_py310.py
+-rw-r--r--   0        0        0      410 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/body_nested_models/tutorial002_py39.py
+-rw-r--r--   0        0        0      417 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/body_nested_models/tutorial003.py
+-rw-r--r--   0        0        0      374 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/body_nested_models/tutorial003_py310.py
+-rw-r--r--   0        0        0      412 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/body_nested_models/tutorial003_py39.py
+-rw-r--r--   0        0        0      507 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/body_nested_models/tutorial004.py
+-rw-r--r--   0        0        0      458 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/body_nested_models/tutorial004_py310.py
+-rw-r--r--   0        0        0      502 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/body_nested_models/tutorial004_py39.py
+-rw-r--r--   0        0        0      520 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/body_nested_models/tutorial005.py
+-rw-r--r--   0        0        0      471 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/body_nested_models/tutorial005_py310.py
+-rw-r--r--   0        0        0      515 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/body_nested_models/tutorial005_py39.py
+-rw-r--r--   0        0        0      533 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/body_nested_models/tutorial006.py
+-rw-r--r--   0        0        0      478 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/body_nested_models/tutorial006_py310.py
+-rw-r--r--   0        0        0      522 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/body_nested_models/tutorial006_py39.py
+-rw-r--r--   0        0        0      584 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/body_nested_models/tutorial007.py
+-rw-r--r--   0        0        0      523 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/body_nested_models/tutorial007_py310.py
+-rw-r--r--   0        0        0      573 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/body_nested_models/tutorial007_py39.py
+-rw-r--r--   0        0        0      276 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/body_nested_models/tutorial008.py
+-rw-r--r--   0        0        0      251 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/body_nested_models/tutorial008_py39.py
+-rw-r--r--   0        0        0      182 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/body_nested_models/tutorial009.py
+-rw-r--r--   0        0        0      157 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/body_nested_models/tutorial009_py39.py
+-rw-r--r--   0        0        0      910 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/body_updates/tutorial001.py
+-rw-r--r--   0        0        0      860 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/body_updates/tutorial001_py310.py
+-rw-r--r--   0        0        0      904 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/body_updates/tutorial001_py39.py
+-rw-r--r--   0        0        0     1064 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/body_updates/tutorial002.py
+-rw-r--r--   0        0        0     1014 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/body_updates/tutorial002_py310.py
+-rw-r--r--   0        0        0     1058 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/body_updates/tutorial002_py39.py
+-rw-r--r--   0        0        0      284 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/conditional_openapi/tutorial001.py
+-rw-r--r--   0        0        0      208 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/configure_swagger_ui/tutorial001.py
+-rw-r--r--   0        0        0      219 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/configure_swagger_ui/tutorial002.py
+-rw-r--r--   0        0        0      204 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/configure_swagger_ui/tutorial003.py
+-rw-r--r--   0        0        0      205 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/cookie_params/tutorial001.py
+-rw-r--r--   0        0        0      250 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/cookie_params/tutorial001_an.py
+-rw-r--r--   0        0        0      208 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/cookie_params/tutorial001_an_py310.py
+-rw-r--r--   0        0        0      221 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/cookie_params/tutorial001_an_py39.py
+-rw-r--r--   0        0        0      173 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/cookie_params/tutorial001_py310.py
+-rw-r--r--   0        0        0      467 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/cors/tutorial001.py
+-rw-r--r--   0        0        0     1158 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/custom_docs_ui/tutorial001.py
+-rw-r--r--   0        0        0     1180 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/custom_docs_ui/tutorial002.py
+-rw-r--r--   0        0        0      977 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/custom_request_and_route/tutorial001.py
+-rw-r--r--   0        0        0      937 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/custom_request_and_route/tutorial002.py
+-rw-r--r--   0        0        0     1046 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/custom_request_and_route/tutorial003.py
+-rw-r--r--   0        0        0      201 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/custom_response/tutorial001.py
+-rw-r--r--   0        0        0      219 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/custom_response/tutorial001b.py
+-rw-r--r--   0        0        0      356 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/custom_response/tutorial002.py
+-rw-r--r--   0        0        0      398 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/custom_response/tutorial003.py
+-rw-r--r--   0        0        0      495 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/custom_response/tutorial004.py
+-rw-r--r--   0        0        0      190 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/custom_response/tutorial005.py
+-rw-r--r--   0        0        0      203 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/custom_response/tutorial006.py
+-rw-r--r--   0        0        0      229 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/custom_response/tutorial006b.py
+-rw-r--r--   0        0        0      241 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/custom_response/tutorial006c.py
+-rw-r--r--   0        0        0      281 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/custom_response/tutorial007.py
+-rw-r--r--   0        0        0      364 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/custom_response/tutorial008.py
+-rw-r--r--   0        0        0      206 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/custom_response/tutorial009.py
+-rw-r--r--   0        0        0      221 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/custom_response/tutorial009b.py
+-rw-r--r--   0        0        0      454 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/custom_response/tutorial009c.py
+-rw-r--r--   0        0        0      209 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/custom_response/tutorial010.py
+-rw-r--r--   0        0        0      315 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/dataclasses/tutorial001.py
+-rw-r--r--   0        0        0      555 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/dataclasses/tutorial002.py
+-rw-r--r--   0        0        0     1406 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/dataclasses/tutorial003.py
+-rw-r--r--   0        0        0      226 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/debugging/tutorial001.py
+-rw-r--r--   0        0        0      445 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/dependencies/tutorial001.py
+-rw-r--r--   0        0        0      498 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/dependencies/tutorial001_02_an.py
+-rw-r--r--   0        0        0      450 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/dependencies/tutorial001_02_an_py310.py
+-rw-r--r--   0        0        0      469 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/dependencies/tutorial001_02_an_py39.py
+-rw-r--r--   0        0        0      505 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/dependencies/tutorial001_an.py
+-rw-r--r--   0        0        0      457 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/dependencies/tutorial001_an_py310.py
+-rw-r--r--   0        0        0      476 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/dependencies/tutorial001_an_py39.py
+-rw-r--r--   0        0        0      407 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/dependencies/tutorial001_py310.py
+-rw-r--r--   0        0        0      659 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/dependencies/tutorial002.py
+-rw-r--r--   0        0        0      709 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/dependencies/tutorial002_an.py
+-rw-r--r--   0        0        0      667 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/dependencies/tutorial002_an_py310.py
+-rw-r--r--   0        0        0      680 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/dependencies/tutorial002_an_py39.py
+-rw-r--r--   0        0        0      627 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/dependencies/tutorial002_py310.py
+-rw-r--r--   0        0        0      638 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/dependencies/tutorial003.py
+-rw-r--r--   0        0        0      700 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/dependencies/tutorial003_an.py
+-rw-r--r--   0        0        0      658 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/dependencies/tutorial003_an_py310.py
+-rw-r--r--   0        0        0      671 2024-05-12 00:38:13.702839 readyapi-0.110.3/docs_src/dependencies/tutorial003_an_py39.py
+-rw-r--r--   0        0        0      606 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/dependencies/tutorial003_py310.py
+-rw-r--r--   0        0        0      642 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/dependencies/tutorial004.py
+-rw-r--r--   0        0        0      692 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/dependencies/tutorial004_an.py
+-rw-r--r--   0        0        0      650 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/dependencies/tutorial004_an_py310.py
+-rw-r--r--   0        0        0      663 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/dependencies/tutorial004_an_py39.py
+-rw-r--r--   0        0        0      610 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/dependencies/tutorial004_py310.py
+-rw-r--r--   0        0        0      489 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/dependencies/tutorial005.py
+-rw-r--r--   0        0        0      561 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/dependencies/tutorial005_an.py
+-rw-r--r--   0        0        0      513 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/dependencies/tutorial005_an_py310.py
+-rw-r--r--   0        0        0      532 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/dependencies/tutorial005_an_py39.py
+-rw-r--r--   0        0        0      446 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/dependencies/tutorial005_py310.py
+-rw-r--r--   0        0        0      586 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/dependencies/tutorial006.py
+-rw-r--r--   0        0        0      646 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/dependencies/tutorial006_an.py
+-rw-r--r--   0        0        0      636 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/dependencies/tutorial006_an_py39.py
+-rw-r--r--   0        0        0       99 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/dependencies/tutorial007.py
+-rw-r--r--   0        0        0      456 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/dependencies/tutorial008.py
+-rw-r--r--   0        0        0      532 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/dependencies/tutorial008_an.py
+-rw-r--r--   0        0        0      522 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/dependencies/tutorial008_an_py39.py
+-rw-r--r--   0        0        0      738 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/dependencies/tutorial008b.py
+-rw-r--r--   0        0        0      788 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/dependencies/tutorial008b_an.py
+-rw-r--r--   0        0        0      778 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/dependencies/tutorial008b_an_py39.py
+-rw-r--r--   0        0        0      663 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/dependencies/tutorial008c.py
+-rw-r--r--   0        0        0      713 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/dependencies/tutorial008c_an.py
+-rw-r--r--   0        0        0      703 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/dependencies/tutorial008c_an_py39.py
+-rw-r--r--   0        0        0      697 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/dependencies/tutorial008d.py
+-rw-r--r--   0        0        0      747 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/dependencies/tutorial008d_an.py
+-rw-r--r--   0        0        0      737 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/dependencies/tutorial008d_an_py39.py
+-rw-r--r--   0        0        0      456 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/dependencies/tutorial009.py
+-rw-r--r--   0        0        0      292 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/dependencies/tutorial010.py
+-rw-r--r--   0        0        0      507 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/dependencies/tutorial011.py
+-rw-r--r--   0        0        0      557 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/dependencies/tutorial011_an.py
+-rw-r--r--   0        0        0      547 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/dependencies/tutorial011_an_py39.py
+-rw-r--r--   0        0        0      699 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/dependencies/tutorial012.py
+-rw-r--r--   0        0        0      759 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/dependencies/tutorial012_an.py
+-rw-r--r--   0        0        0      759 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/dependencies/tutorial012_an_py39.py
+-rw-r--r--   0        0        0     1526 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/dependency_testing/tutorial001.py
+-rw-r--r--   0        0        0     1586 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/dependency_testing/tutorial001_an.py
+-rw-r--r--   0        0        0     1532 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/dependency_testing/tutorial001_an_py310.py
+-rw-r--r--   0        0        0     1557 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/dependency_testing/tutorial001_an_py39.py
+-rw-r--r--   0        0        0     1482 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/dependency_testing/tutorial001_py310.py
+-rw-r--r--   0        0        0      465 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/encoder/tutorial001.py
+-rw-r--r--   0        0        0      434 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/encoder/tutorial001_py310.py
+-rw-r--r--   0        0        0      286 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/events/tutorial001.py
+-rw-r--r--   0        0        0      258 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/events/tutorial002.py
+-rw-r--r--   0        0        0      573 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/events/tutorial003.py
+-rw-r--r--   0        0        0      744 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/extending_openapi/tutorial001.py
+-rw-r--r--   0        0        0      833 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/extra_data_types/tutorial001.py
+-rw-r--r--   0        0        0      893 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/extra_data_types/tutorial001_an.py
+-rw-r--r--   0        0        0      833 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/extra_data_types/tutorial001_an_py310.py
+-rw-r--r--   0        0        0      864 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/extra_data_types/tutorial001_an_py39.py
+-rw-r--r--   0        0        0      784 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/extra_data_types/tutorial001_py310.py
+-rw-r--r--   0        0        0      946 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/extra_models/tutorial001.py
+-rw-r--r--   0        0        0      902 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/extra_models/tutorial001_py310.py
+-rw-r--r--   0        0        0      827 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/extra_models/tutorial002.py
+-rw-r--r--   0        0        0      795 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/extra_models/tutorial002_py310.py
+-rw-r--r--   0        0        0      647 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/extra_models/tutorial003.py
+-rw-r--r--   0        0        0      647 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/extra_models/tutorial003_py310.py
+-rw-r--r--   0        0        0      384 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/extra_models/tutorial004.py
+-rw-r--r--   0        0        0      359 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/extra_models/tutorial004_py39.py
+-rw-r--r--   0        0        0      208 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/extra_models/tutorial005.py
+-rw-r--r--   0        0        0      183 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/extra_models/tutorial005_py39.py
+-rw-r--r--   0        0        0      120 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/first_steps/tutorial001.py
+-rw-r--r--   0        0        0      142 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/first_steps/tutorial002.py
+-rw-r--r--   0        0        0      114 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/first_steps/tutorial003.py
+-rw-r--r--   0        0        0      522 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/generate_clients/tutorial001.py
+-rw-r--r--   0        0        0      497 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/generate_clients/tutorial001_py39.py
+-rw-r--r--   0        0        0      758 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/generate_clients/tutorial002.py
+-rw-r--r--   0        0        0      733 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/generate_clients/tutorial002_py39.py
+-rw-r--r--   0        0        0      943 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/generate_clients/tutorial003.py
+-rw-r--r--   0        0        0      918 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/generate_clients/tutorial003_py39.py
+-rw-r--r--   0        0        0     1066 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/generate_clients/tutorial004.js
+-rw-r--r--   0        0        0      493 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/generate_clients/tutorial004.py
+-rw-r--r--   0        0        0      449 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/graphql/tutorial001.py
+-rw-r--r--   0        0        0      302 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/handling_errors/tutorial001.py
+-rw-r--r--   0        0        0      407 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/handling_errors/tutorial002.py
+-rw-r--r--   0        0        0      630 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/handling_errors/tutorial003.py
+-rw-r--r--   0        0        0      767 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/handling_errors/tutorial004.py
+-rw-r--r--   0        0        0      673 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/handling_errors/tutorial005.py
+-rw-r--r--   0        0        0      933 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/handling_errors/tutorial006.py
+-rw-r--r--   0        0        0      217 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/header_params/tutorial001.py
+-rw-r--r--   0        0        0      262 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/header_params/tutorial001_an.py
+-rw-r--r--   0        0        0      220 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/header_params/tutorial001_an_py310.py
+-rw-r--r--   0        0        0      233 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/header_params/tutorial001_an_py39.py
+-rw-r--r--   0        0        0      185 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/header_params/tutorial001_py310.py
+-rw-r--r--   0        0        0      263 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/header_params/tutorial002.py
+-rw-r--r--   0        0        0      320 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/header_params/tutorial002_an.py
+-rw-r--r--   0        0        0      264 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/header_params/tutorial002_an_py310.py
+-rw-r--r--   0        0        0      291 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/header_params/tutorial002_an_py39.py
+-rw-r--r--   0        0        0      231 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/header_params/tutorial002_py310.py
+-rw-r--r--   0        0        0      227 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/header_params/tutorial003.py
+-rw-r--r--   0        0        0      272 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/header_params/tutorial003_an.py
+-rw-r--r--   0        0        0      224 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/header_params/tutorial003_an_py310.py
+-rw-r--r--   0        0        0      243 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/header_params/tutorial003_an_py39.py
+-rw-r--r--   0        0        0      189 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/header_params/tutorial003_py310.py
+-rw-r--r--   0        0        0      221 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/header_params/tutorial003_py39.py
+-rw-r--r--   0        0        0      808 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/metadata/tutorial001.py
+-rw-r--r--   0        0        0      770 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/metadata/tutorial001_1.py
+-rw-r--r--   0        0        0      157 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/metadata/tutorial002.py
+-rw-r--r--   0        0        0      164 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/metadata/tutorial003.py
+-rw-r--r--   0        0        0      699 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/metadata/tutorial004.py
+-rw-r--r--   0        0        0      352 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/middleware/tutorial001.py
+-rw-r--r--   0        0        0     1361 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/nosql_databases/tutorial001.py
+-rw-r--r--   0        0        0     1374 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/openapi_callbacks/tutorial001.py
+-rw-r--r--   0        0        0      553 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/openapi_webhooks/tutorial001.py
+-rw-r--r--   0        0        0      170 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/path_operation_advanced_configuration/tutorial001.py
+-rw-r--r--   0        0        0      577 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/path_operation_advanced_configuration/tutorial002.py
+-rw-r--r--   0        0        0      151 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/path_operation_advanced_configuration/tutorial003.py
+-rw-r--r--   0        0        0      720 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/path_operation_advanced_configuration/tutorial004.py
+-rw-r--r--   0        0        0      183 2024-05-12 00:38:13.706840 readyapi-0.110.3/docs_src/path_operation_advanced_configuration/tutorial005.py
+-rw-r--r--   0        0        0     1046 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/path_operation_advanced_configuration/tutorial006.py
+-rw-r--r--   0        0        0      825 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/path_operation_advanced_configuration/tutorial007.py
+-rw-r--r--   0        0        0      792 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/path_operation_advanced_configuration/tutorial007_pv1.py
+-rw-r--r--   0        0        0      409 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/path_operation_configuration/tutorial001.py
+-rw-r--r--   0        0        0      366 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/path_operation_configuration/tutorial001_py310.py
+-rw-r--r--   0        0        0      404 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/path_operation_configuration/tutorial001_py39.py
+-rw-r--r--   0        0        0      583 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/path_operation_configuration/tutorial002.py
+-rw-r--r--   0        0        0      540 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/path_operation_configuration/tutorial002_py310.py
+-rw-r--r--   0        0        0      578 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/path_operation_configuration/tutorial002_py39.py
+-rw-r--r--   0        0        0      326 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/path_operation_configuration/tutorial002b.py
+-rw-r--r--   0        0        0      520 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/path_operation_configuration/tutorial003.py
+-rw-r--r--   0        0        0      477 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/path_operation_configuration/tutorial003_py310.py
+-rw-r--r--   0        0        0      515 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/path_operation_configuration/tutorial003_py39.py
+-rw-r--r--   0        0        0      684 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/path_operation_configuration/tutorial004.py
+-rw-r--r--   0        0        0      641 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/path_operation_configuration/tutorial004_py310.py
+-rw-r--r--   0        0        0      679 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/path_operation_configuration/tutorial004_py39.py
+-rw-r--r--   0        0        0      744 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/path_operation_configuration/tutorial005.py
+-rw-r--r--   0        0        0      701 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/path_operation_configuration/tutorial005_py310.py
+-rw-r--r--   0        0        0      739 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/path_operation_configuration/tutorial005_py39.py
+-rw-r--r--   0        0        0      368 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/path_operation_configuration/tutorial006.py
+-rw-r--r--   0        0        0      141 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/path_params/tutorial001.py
+-rw-r--r--   0        0        0      146 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/path_params/tutorial002.py
+-rw-r--r--   0        0        0      239 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/path_params/tutorial003.py
+-rw-r--r--   0        0        0      196 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/path_params/tutorial003b.py
+-rw-r--r--   0        0        0      159 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/path_params/tutorial004.py
+-rw-r--r--   0        0        0      549 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/path_params/tutorial005.py
+-rw-r--r--   0        0        0      367 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/path_params_numeric_validations/tutorial001.py
+-rw-r--r--   0        0        0      420 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/path_params_numeric_validations/tutorial001_an.py
+-rw-r--r--   0        0        0      378 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/path_params_numeric_validations/tutorial001_an_py310.py
+-rw-r--r--   0        0        0      391 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/path_params_numeric_validations/tutorial001_an_py39.py
+-rw-r--r--   0        0        0      335 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/path_params_numeric_validations/tutorial001_py310.py
+-rw-r--r--   0        0        0      268 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/path_params_numeric_validations/tutorial002.py
+-rw-r--r--   0        0        0      324 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/path_params_numeric_validations/tutorial002_an.py
+-rw-r--r--   0        0        0      314 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/path_params_numeric_validations/tutorial002_an_py39.py
+-rw-r--r--   0        0        0      271 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/path_params_numeric_validations/tutorial003.py
+-rw-r--r--   0        0        0      324 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/path_params_numeric_validations/tutorial003_an.py
+-rw-r--r--   0        0        0      314 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/path_params_numeric_validations/tutorial003_an_py39.py
+-rw-r--r--   0        0        0      283 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/path_params_numeric_validations/tutorial004.py
+-rw-r--r--   0        0        0      330 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/path_params_numeric_validations/tutorial004_an.py
+-rw-r--r--   0        0        0      320 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/path_params_numeric_validations/tutorial004_an_py39.py
+-rw-r--r--   0        0        0      301 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/path_params_numeric_validations/tutorial005.py
+-rw-r--r--   0        0        0      344 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/path_params_numeric_validations/tutorial005_an.py
+-rw-r--r--   0        0        0      334 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/path_params_numeric_validations/tutorial005_an_py39.py
+-rw-r--r--   0        0        0      348 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/path_params_numeric_validations/tutorial006.py
+-rw-r--r--   0        0        0      408 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/path_params_numeric_validations/tutorial006_an.py
+-rw-r--r--   0        0        0      398 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/path_params_numeric_validations/tutorial006_an_py39.py
+-rw-r--r--   0        0        0      162 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/python_types/tutorial001.py
+-rw-r--r--   0        0        0      172 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/python_types/tutorial002.py
+-rw-r--r--   0        0        0      119 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/python_types/tutorial003.py
+-rw-r--r--   0        0        0      124 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/python_types/tutorial004.py
+-rw-r--r--   0        0        0      143 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/python_types/tutorial005.py
+-rw-r--r--   0        0        0      106 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/python_types/tutorial006.py
+-rw-r--r--   0        0        0       80 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/python_types/tutorial006_py39.py
+-rw-r--r--   0        0        0      131 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/python_types/tutorial007.py
+-rw-r--r--   0        0        0       99 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/python_types/tutorial007_py39.py
+-rw-r--r--   0        0        0      171 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/python_types/tutorial008.py
+-rw-r--r--   0        0        0      145 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/python_types/tutorial008_py39.py
+-rw-r--r--   0        0        0       84 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/python_types/tutorial008b.py
+-rw-r--r--   0        0        0       51 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/python_types/tutorial008b_py310.py
+-rw-r--r--   0        0        0      164 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/python_types/tutorial009.py
+-rw-r--r--   0        0        0      131 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/python_types/tutorial009_py310.py
+-rw-r--r--   0        0        0      164 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/python_types/tutorial009b.py
+-rw-r--r--   0        0        0       89 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/python_types/tutorial009c.py
+-rw-r--r--   0        0        0       56 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/python_types/tutorial009c_py310.py
+-rw-r--r--   0        0        0      144 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/python_types/tutorial010.py
+-rw-r--r--   0        0        0      498 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/python_types/tutorial011.py
+-rw-r--r--   0        0        0      461 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/python_types/tutorial011_py310.py
+-rw-r--r--   0        0        0      492 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/python_types/tutorial011_py39.py
+-rw-r--r--   0        0        0      122 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/python_types/tutorial012.py
+-rw-r--r--   0        0        0      138 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/python_types/tutorial013.py
+-rw-r--r--   0        0        0      127 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/python_types/tutorial013_py39.py
+-rw-r--r--   0        0        0      253 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/query_params/tutorial001.py
+-rw-r--r--   0        0        0      254 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/query_params/tutorial002.py
+-rw-r--r--   0        0        0      222 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/query_params/tutorial002_py310.py
+-rw-r--r--   0        0        0      409 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/query_params/tutorial003.py
+-rw-r--r--   0        0        0      377 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/query_params/tutorial003_py310.py
+-rw-r--r--   0        0        0      471 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/query_params/tutorial004.py
+-rw-r--r--   0        0        0      439 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/query_params/tutorial004_py310.py
+-rw-r--r--   0        0        0      195 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/query_params/tutorial005.py
+-rw-r--r--   0        0        0      304 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/query_params/tutorial006.py
+-rw-r--r--   0        0        0      272 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/query_params/tutorial006_py310.py
+-rw-r--r--   0        0        0      304 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/query_params/tutorial006b.py
+-rw-r--r--   0        0        0      274 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial001.py
+-rw-r--r--   0        0        0      242 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial001_py310.py
+-rw-r--r--   0        0        0      311 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial002.py
+-rw-r--r--   0        0        0      354 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial002_an.py
+-rw-r--r--   0        0        0      312 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial002_an_py310.py
+-rw-r--r--   0        0        0      279 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial002_py310.py
+-rw-r--r--   0        0        0      332 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial003.py
+-rw-r--r--   0        0        0      375 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial003_an.py
+-rw-r--r--   0        0        0      333 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial003_an_py310.py
+-rw-r--r--   0        0        0      346 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial003_an_py39.py
+-rw-r--r--   0        0        0      293 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial003_py310.py
+-rw-r--r--   0        0        0      370 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial004.py
+-rw-r--r--   0        0        0      413 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial004_an.py
+-rw-r--r--   0        0        0      371 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial004_an_py310.py
+-rw-r--r--   0        0        0      369 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial004_an_py310_regex.py
+-rw-r--r--   0        0        0      384 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial004_an_py39.py
+-rw-r--r--   0        0        0      338 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial004_py310.py
+-rw-r--r--   0        0        0      279 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial005.py
+-rw-r--r--   0        0        0      322 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial005_an.py
+-rw-r--r--   0        0        0      312 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial005_an_py39.py
+-rw-r--r--   0        0        0      257 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial006.py
+-rw-r--r--   0        0        0      307 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial006_an.py
+-rw-r--r--   0        0        0      297 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial006_an_py39.py
+-rw-r--r--   0        0        0      270 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial006b.py
+-rw-r--r--   0        0        0      313 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial006b_an.py
+-rw-r--r--   0        0        0      303 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial006b_an_py39.py
+-rw-r--r--   0        0        0      309 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial006c.py
+-rw-r--r--   0        0        0      352 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial006c_an.py
+-rw-r--r--   0        0        0      310 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial006c_an_py310.py
+-rw-r--r--   0        0        0      323 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial006c_an_py39.py
+-rw-r--r--   0        0        0      277 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial006c_py310.py
+-rw-r--r--   0        0        0      305 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial006d.py
+-rw-r--r--   0        0        0      348 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial006d_an.py
+-rw-r--r--   0        0        0      338 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial006d_an_py39.py
+-rw-r--r--   0        0        0      339 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial007.py
+-rw-r--r--   0        0        0      382 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial007_an.py
+-rw-r--r--   0        0        0      340 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial007_an_py310.py
+-rw-r--r--   0        0        0      353 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial007_an_py39.py
+-rw-r--r--   0        0        0      307 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial007_py310.py
+-rw-r--r--   0        0        0      469 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial008.py
+-rw-r--r--   0        0        0      543 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial008_an.py
+-rw-r--r--   0        0        0      501 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial008_an_py310.py
+-rw-r--r--   0        0        0      514 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial008_an_py39.py
+-rw-r--r--   0        0        0      437 2024-05-12 00:38:13.710840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial008_py310.py
+-rw-r--r--   0        0        0      316 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial009.py
+-rw-r--r--   0        0        0      359 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial009_an.py
+-rw-r--r--   0        0        0      317 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial009_an_py310.py
+-rw-r--r--   0        0        0      330 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial009_an_py39.py
+-rw-r--r--   0        0        0      284 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial009_py310.py
+-rw-r--r--   0        0        0      577 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial010.py
+-rw-r--r--   0        0        0      667 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial010_an.py
+-rw-r--r--   0        0        0      625 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial010_an_py310.py
+-rw-r--r--   0        0        0      638 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial010_an_py39.py
+-rw-r--r--   0        0        0      545 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial010_py310.py
+-rw-r--r--   0        0        0      230 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial011.py
+-rw-r--r--   0        0        0      275 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial011_an.py
+-rw-r--r--   0        0        0      227 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial011_an_py310.py
+-rw-r--r--   0        0        0      240 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial011_an_py39.py
+-rw-r--r--   0        0        0      192 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial011_py310.py
+-rw-r--r--   0        0        0      224 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial011_py39.py
+-rw-r--r--   0        0        0      220 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial012.py
+-rw-r--r--   0        0        0      265 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial012_an.py
+-rw-r--r--   0        0        0      230 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial012_an_py39.py
+-rw-r--r--   0        0        0      195 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial012_py39.py
+-rw-r--r--   0        0        0      178 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial013.py
+-rw-r--r--   0        0        0      223 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial013_an.py
+-rw-r--r--   0        0        0      213 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial013_an_py39.py
+-rw-r--r--   0        0        0      333 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial014.py
+-rw-r--r--   0        0        0      376 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial014_an.py
+-rw-r--r--   0        0        0      334 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial014_an_py310.py
+-rw-r--r--   0        0        0      347 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial014_an_py39.py
+-rw-r--r--   0        0        0      301 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/query_params_str_validations/tutorial014_py310.py
+-rw-r--r--   0        0        0      285 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/request_files/tutorial001.py
+-rw-r--r--   0        0        0      511 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/request_files/tutorial001_02.py
+-rw-r--r--   0        0        0      556 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/request_files/tutorial001_02_an.py
+-rw-r--r--   0        0        0      508 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/request_files/tutorial001_02_an_py310.py
+-rw-r--r--   0        0        0      527 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/request_files/tutorial001_02_an_py39.py
+-rw-r--r--   0        0        0      473 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/request_files/tutorial001_02_py310.py
+-rw-r--r--   0        0        0      374 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/request_files/tutorial001_03.py
+-rw-r--r--   0        0        0      434 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/request_files/tutorial001_03_an.py
+-rw-r--r--   0        0        0      424 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/request_files/tutorial001_03_an_py39.py
+-rw-r--r--   0        0        0      335 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/request_files/tutorial001_an.py
+-rw-r--r--   0        0        0      325 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/request_files/tutorial001_an_py39.py
+-rw-r--r--   0        0        0      815 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/request_files/tutorial002.py
+-rw-r--r--   0        0        0      865 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/request_files/tutorial002_an.py
+-rw-r--r--   0        0        0      830 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/request_files/tutorial002_an_py39.py
+-rw-r--r--   0        0        0      790 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/request_files/tutorial002_py39.py
+-rw-r--r--   0        0        0      917 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/request_files/tutorial003.py
+-rw-r--r--   0        0        0      991 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/request_files/tutorial003_an.py
+-rw-r--r--   0        0        0      956 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/request_files/tutorial003_an_py39.py
+-rw-r--r--   0        0        0      892 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/request_files/tutorial003_py39.py
+-rw-r--r--   0        0        0      176 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/request_forms/tutorial001.py
+-rw-r--r--   0        0        0      236 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/request_forms/tutorial001_an.py
+-rw-r--r--   0        0        0      226 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/request_forms/tutorial001_an_py39.py
+-rw-r--r--   0        0        0      320 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/request_forms_and_files/tutorial001.py
+-rw-r--r--   0        0        0      399 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/request_forms_and_files/tutorial001_an.py
+-rw-r--r--   0        0        0      389 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/request_forms_and_files/tutorial001_an_py39.py
+-rw-r--r--   0        0        0      394 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/response_change_status_code/tutorial001.py
+-rw-r--r--   0        0        0      348 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/response_cookies/tutorial001.py
+-rw-r--r--   0        0        0      275 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/response_cookies/tutorial002.py
+-rw-r--r--   0        0        0      510 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/response_directly/tutorial001.py
+-rw-r--r--   0        0        0      357 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/response_directly/tutorial002.py
+-rw-r--r--   0        0        0      313 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/response_headers/tutorial001.py
+-rw-r--r--   0        0        0      225 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/response_headers/tutorial002.py
+-rw-r--r--   0        0        0      565 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/response_model/tutorial001.py
+-rw-r--r--   0        0        0      516 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/response_model/tutorial001_01.py
+-rw-r--r--   0        0        0      472 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/response_model/tutorial001_01_py310.py
+-rw-r--r--   0        0        0      510 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/response_model/tutorial001_01_py39.py
+-rw-r--r--   0        0        0      540 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/response_model/tutorial001_py310.py
+-rw-r--r--   0        0        0      559 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/response_model/tutorial001_py39.py
+-rw-r--r--   0        0        0      353 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/response_model/tutorial002.py
+-rw-r--r--   0        0        0      321 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/response_model/tutorial002_py310.py
+-rw-r--r--   0        0        0      453 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/response_model/tutorial003.py
+-rw-r--r--   0        0        0      352 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/response_model/tutorial003_01.py
+-rw-r--r--   0        0        0      320 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/response_model/tutorial003_01_py310.py
+-rw-r--r--   0        0        0      385 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/response_model/tutorial003_02.py
+-rw-r--r--   0        0        0      245 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/response_model/tutorial003_03.py
+-rw-r--r--   0        0        0      388 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/response_model/tutorial003_04.py
+-rw-r--r--   0        0        0      356 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/response_model/tutorial003_04_py310.py
+-rw-r--r--   0        0        0      409 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/response_model/tutorial003_05.py
+-rw-r--r--   0        0        0      377 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/response_model/tutorial003_05_py310.py
+-rw-r--r--   0        0        0      434 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/response_model/tutorial003_py310.py
+-rw-r--r--   0        0        0      636 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/response_model/tutorial004.py
+-rw-r--r--   0        0        0      598 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/response_model/tutorial004_py310.py
+-rw-r--r--   0        0        0      630 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/response_model/tutorial004_py39.py
+-rw-r--r--   0        0        0      851 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/response_model/tutorial005.py
+-rw-r--r--   0        0        0      819 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/response_model/tutorial005_py310.py
+-rw-r--r--   0        0        0      851 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/response_model/tutorial006.py
+-rw-r--r--   0        0        0      819 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/response_model/tutorial006_py310.py
+-rw-r--r--   0        0        0      148 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/response_status_code/tutorial001.py
+-rw-r--r--   0        0        0      176 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/response_status_code/tutorial002.py
+-rw-r--r--   0        0        0      687 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/schema_extra_example/tutorial001.py
+-rw-r--r--   0        0        0      672 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/schema_extra_example/tutorial001_pv1.py
+-rw-r--r--   0        0        0      649 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/schema_extra_example/tutorial001_py310.py
+-rw-r--r--   0        0        0      634 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/schema_extra_example/tutorial001_py310_pv1.py
+-rw-r--r--   0        0        0      520 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/schema_extra_example/tutorial002.py
+-rw-r--r--   0        0        0      482 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/schema_extra_example/tutorial002_py310.py
+-rw-r--r--   0        0        0      615 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/schema_extra_example/tutorial003.py
+-rw-r--r--   0        0        0      724 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/schema_extra_example/tutorial003_an.py
+-rw-r--r--   0        0        0      676 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/schema_extra_example/tutorial003_an_py310.py
+-rw-r--r--   0        0        0      695 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/schema_extra_example/tutorial003_an_py39.py
+-rw-r--r--   0        0        0      577 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/schema_extra_example/tutorial003_py310.py
+-rw-r--r--   0        0        0      827 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/schema_extra_example/tutorial004.py
+-rw-r--r--   0        0        0      968 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/schema_extra_example/tutorial004_an.py
+-rw-r--r--   0        0        0      920 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/schema_extra_example/tutorial004_an_py310.py
+-rw-r--r--   0        0        0      939 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/schema_extra_example/tutorial004_an_py39.py
+-rw-r--r--   0        0        0      789 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/schema_extra_example/tutorial004_py310.py
+-rw-r--r--   0        0        0     1390 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/schema_extra_example/tutorial005.py
+-rw-r--r--   0        0        0     1575 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/schema_extra_example/tutorial005_an.py
+-rw-r--r--   0        0        0     1527 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/schema_extra_example/tutorial005_an_py310.py
+-rw-r--r--   0        0        0     1546 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/schema_extra_example/tutorial005_an_py39.py
+-rw-r--r--   0        0        0     1352 2024-05-12 00:38:13.714840 readyapi-0.110.3/docs_src/schema_extra_example/tutorial005_py310.py
+-rw-r--r--   0        0        0      273 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/security/tutorial001.py
+-rw-r--r--   0        0        0      323 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/security/tutorial001_an.py
+-rw-r--r--   0        0        0      313 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/security/tutorial001_an_py39.py
+-rw-r--r--   0        0        0      759 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/security/tutorial002.py
+-rw-r--r--   0        0        0      819 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/security/tutorial002_an.py
+-rw-r--r--   0        0        0      765 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/security/tutorial002_an_py310.py
+-rw-r--r--   0        0        0      790 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/security/tutorial002_an_py39.py
+-rw-r--r--   0        0        0      715 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/security/tutorial002_py310.py
+-rw-r--r--   0        0        0     2498 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/security/tutorial003.py
+-rw-r--r--   0        0        0     2592 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/security/tutorial003_an.py
+-rw-r--r--   0        0        0     2538 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/security/tutorial003_an_py310.py
+-rw-r--r--   0        0        0     2563 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/security/tutorial003_an_py39.py
+-rw-r--r--   0        0        0     2454 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/security/tutorial003_py310.py
+-rw-r--r--   0        0        0     4138 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/security/tutorial004.py
+-rw-r--r--   0        0        0     4249 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/security/tutorial004_an.py
+-rw-r--r--   0        0        0     4183 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/security/tutorial004_an_py310.py
+-rw-r--r--   0        0        0     4220 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/security/tutorial004_an_py39.py
+-rw-r--r--   0        0        0     4083 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/security/tutorial004_py310.py
+-rw-r--r--   0        0        0     5274 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/security/tutorial005.py
+-rw-r--r--   0        0        0     5381 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/security/tutorial005_an.py
+-rw-r--r--   0        0        0     5309 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/security/tutorial005_an_py310.py
+-rw-r--r--   0        0        0     5352 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/security/tutorial005_an_py39.py
+-rw-r--r--   0        0        0     5213 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/security/tutorial005_py310.py
+-rw-r--r--   0        0        0     5268 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/security/tutorial005_py39.py
+-rw-r--r--   0        0        0      325 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/security/tutorial006.py
+-rw-r--r--   0        0        0      375 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/security/tutorial006_an.py
+-rw-r--r--   0        0        0      365 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/security/tutorial006_an_py39.py
+-rw-r--r--   0        0        0     1120 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/security/tutorial007.py
+-rw-r--r--   0        0        0     1187 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/security/tutorial007_an.py
+-rw-r--r--   0        0        0     1176 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/security/tutorial007_an_py39.py
+-rw-r--r--   0        0        0      492 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/separate_openapi_schemas/tutorial001.py
+-rw-r--r--   0        0        0      454 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/separate_openapi_schemas/tutorial001_py310.py
+-rw-r--r--   0        0        0      486 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/separate_openapi_schemas/tutorial001_py39.py
+-rw-r--r--   0        0        0      527 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/separate_openapi_schemas/tutorial002.py
+-rw-r--r--   0        0        0      489 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/separate_openapi_schemas/tutorial002_py310.py
+-rw-r--r--   0        0        0      521 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/separate_openapi_schemas/tutorial002_py39.py
+-rw-r--r--   0        0        0        0 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/settings/app01/__init__.py
+-rw-r--r--   0        0        0      183 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/settings/app01/config.py
+-rw-r--r--   0        0        0      270 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/settings/app01/main.py
+-rw-r--r--   0        0        0        0 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/settings/app02/__init__.py
+-rw-r--r--   0        0        0      159 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/settings/app02/config.py
+-rw-r--r--   0        0        0      409 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/settings/app02/main.py
+-rw-r--r--   0        0        0      516 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/settings/app02/test_main.py
+-rw-r--r--   0        0        0        0 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/settings/app02_an/__init__.py
+-rw-r--r--   0        0        0      159 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/settings/app02_an/config.py
+-rw-r--r--   0        0        0      459 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/settings/app02_an/main.py
+-rw-r--r--   0        0        0      516 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/settings/app02_an/test_main.py
+-rw-r--r--   0        0        0        0 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/settings/app02_an_py39/__init__.py
+-rw-r--r--   0        0        0      159 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/settings/app02_an_py39/config.py
+-rw-r--r--   0        0        0      448 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/settings/app02_an_py39/main.py
+-rw-r--r--   0        0        0      516 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/settings/app02_an_py39/test_main.py
+-rw-r--r--   0        0        0        0 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/settings/app03/__init__.py
+-rw-r--r--   0        0        0      204 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/settings/app03/config.py
+-rw-r--r--   0        0        0      415 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/settings/app03/main.py
+-rw-r--r--   0        0        0        0 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/settings/app03_an/__init__.py
+-rw-r--r--   0        0        0      235 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/settings/app03_an/config.py
+-rw-r--r--   0        0        0      195 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/settings/app03_an/config_pv1.py
+-rw-r--r--   0        0        0      454 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/settings/app03_an/main.py
+-rw-r--r--   0        0        0        0 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/settings/app03_an_py39/__init__.py
+-rw-r--r--   0        0        0      204 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/settings/app03_an_py39/config.py
+-rw-r--r--   0        0        0      465 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/settings/app03_an_py39/main.py
+-rw-r--r--   0        0        0      422 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/settings/tutorial001.py
+-rw-r--r--   0        0        0      413 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/settings/tutorial001_pv1.py
+-rw-r--r--   0        0        0        0 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/sql_databases/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/sql_databases/sql_app/__init__.py
+-rw-r--r--   0        0        0     1931 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/sql_databases/sql_app/alt_main.py
+-rw-r--r--   0        0        0     1061 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/sql_databases/sql_app/crud.py
+-rw-r--r--   0        0        0      461 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/sql_databases/sql_app/database.py
+-rw-r--r--   0        0        0     1635 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/sql_databases/sql_app/main.py
+-rw-r--r--   0        0        0      710 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/sql_databases/sql_app/models.py
+-rw-r--r--   0        0        0      502 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/sql_databases/sql_app/schemas.py
+-rw-r--r--   0        0        0        0 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/sql_databases/sql_app/tests/__init__.py
+-rw-r--r--   0        0        0     1261 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/sql_databases/sql_app/tests/test_sql_app.py
+-rw-r--r--   0        0        0        0 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/sql_databases/sql_app_py310/__init__.py
+-rw-r--r--   0        0        0     1906 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/sql_databases/sql_app_py310/alt_main.py
+-rw-r--r--   0        0        0     1061 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/sql_databases/sql_app_py310/crud.py
+-rw-r--r--   0        0        0      461 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/sql_databases/sql_app_py310/database.py
+-rw-r--r--   0        0        0     1610 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/sql_databases/sql_app_py310/main.py
+-rw-r--r--   0        0        0      710 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/sql_databases/sql_app_py310/models.py
+-rw-r--r--   0        0        0      464 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/sql_databases/sql_app_py310/schemas.py
+-rw-r--r--   0        0        0        0 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/sql_databases/sql_app_py310/tests/__init__.py
+-rw-r--r--   0        0        0     1201 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/sql_databases/sql_app_py310/tests/test_sql_app.py
+-rw-r--r--   0        0        0        0 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/sql_databases/sql_app_py39/__init__.py
+-rw-r--r--   0        0        0     1906 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/sql_databases/sql_app_py39/alt_main.py
+-rw-r--r--   0        0        0     1061 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/sql_databases/sql_app_py39/crud.py
+-rw-r--r--   0        0        0      461 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/sql_databases/sql_app_py39/database.py
+-rw-r--r--   0        0        0     1610 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/sql_databases/sql_app_py39/main.py
+-rw-r--r--   0        0        0      710 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/sql_databases/sql_app_py39/models.py
+-rw-r--r--   0        0        0      496 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/sql_databases/sql_app_py39/schemas.py
+-rw-r--r--   0        0        0        0 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/sql_databases/sql_app_py39/tests/__init__.py
+-rw-r--r--   0        0        0     1201 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/sql_databases/sql_app_py39/tests/test_sql_app.py
+-rw-r--r--   0        0        0        0 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/sql_databases_peewee/sql_app/__init__.py
+-rw-r--r--   0        0        0      843 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/sql_databases_peewee/sql_app/crud.py
+-rw-r--r--   0        0        0      662 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/sql_databases_peewee/sql_app/database.py
+-rw-r--r--   0        0        0     2213 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/sql_databases_peewee/sql_app/main.py
+-rw-r--r--   0        0        0      465 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/sql_databases_peewee/sql_app/models.py
+-rw-r--r--   0        0        0      868 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/sql_databases_peewee/sql_app/schemas.py
+-rw-r--r--   0        0        0      163 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/static_files/tutorial001.py
+-rw-r--r--   0        0        0      278 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/sub_applications/tutorial001.py
+-rw-r--r--   0        0        0       25 2024-05-12 00:38:13.718840 readyapi-0.110.3/docs_src/templates/static/styles.css
+-rw-r--r--   0        0        0      235 2024-05-12 00:38:13.722840 readyapi-0.110.3/docs_src/templates/templates/item.html
+-rw-r--r--   0        0        0      527 2024-05-12 00:38:13.722840 readyapi-0.110.3/docs_src/templates/tutorial001.py
+-rw-r--r--   0        0        0      233 2024-05-12 00:38:13.722840 readyapi-0.110.3/docs_src/using_request_directly/tutorial001.py
+-rw-r--r--   0        0        0        0 2024-05-12 00:38:13.722840 readyapi-0.110.3/docs_src/websockets/__init__.py
+-rw-r--r--   0        0        0     1436 2024-05-12 00:38:13.722840 readyapi-0.110.3/docs_src/websockets/tutorial001.py
+-rw-r--r--   0        0        0     2846 2024-05-12 00:38:13.722840 readyapi-0.110.3/docs_src/websockets/tutorial002.py
+-rw-r--r--   0        0        0     2913 2024-05-12 00:38:13.722840 readyapi-0.110.3/docs_src/websockets/tutorial002_an.py
+-rw-r--r--   0        0        0     2859 2024-05-12 00:38:13.722840 readyapi-0.110.3/docs_src/websockets/tutorial002_an_py310.py
+-rw-r--r--   0        0        0     2884 2024-05-12 00:38:13.722840 readyapi-0.110.3/docs_src/websockets/tutorial002_an_py39.py
+-rw-r--r--   0        0        0     2802 2024-05-12 00:38:13.722840 readyapi-0.110.3/docs_src/websockets/tutorial002_py310.py
+-rw-r--r--   0        0        0     2578 2024-05-12 00:38:13.722840 readyapi-0.110.3/docs_src/websockets/tutorial003.py
+-rw-r--r--   0        0        0     2553 2024-05-12 00:38:13.722840 readyapi-0.110.3/docs_src/websockets/tutorial003_py39.py
+-rw-r--r--   0        0        0      447 2024-05-12 00:38:13.722840 readyapi-0.110.3/docs_src/wsgi/tutorial001.py
+-rw-r--r--   0        0        0     1731 2024-05-12 00:38:13.722840 readyapi-0.110.3/pdm_build.py
+-rw-r--r--   0        0        0     7278 2024-05-12 00:38:20.474897 readyapi-0.110.3/pyproject.toml
+-rw-r--r--   0        0        0     1084 2024-05-12 00:38:13.722840 readyapi-0.110.3/readyapi/__init__.py
+-rw-r--r--   0        0        0    23139 2024-05-12 00:38:13.722840 readyapi-0.110.3/readyapi/_compat.py
+-rw-r--r--   0        0        0   177259 2024-05-12 00:38:13.722840 readyapi-0.110.3/readyapi/applications.py
+-rw-r--r--   0        0        0     1779 2024-05-12 00:38:13.722840 readyapi-0.110.3/readyapi/background.py
+-rw-r--r--   0        0        0     1403 2024-05-12 00:38:13.722840 readyapi-0.110.3/readyapi/concurrency.py
+-rw-r--r--   0        0        0     5774 2024-05-12 00:38:13.722840 readyapi-0.110.3/readyapi/datastructures.py
+-rw-r--r--   0        0        0        0 2024-05-12 00:38:13.722840 readyapi-0.110.3/readyapi/dependencies/__init__.py
+-rw-r--r--   0        0        0     2496 2024-05-12 00:38:13.722840 readyapi-0.110.3/readyapi/dependencies/models.py
+-rw-r--r--   0        0        0    30266 2024-05-12 00:38:13.722840 readyapi-0.110.3/readyapi/dependencies/utils.py
+-rw-r--r--   0        0        0    11074 2024-05-12 00:38:13.722840 readyapi-0.110.3/readyapi/encoders.py
+-rw-r--r--   0        0        0     1336 2024-05-12 00:38:13.722840 readyapi-0.110.3/readyapi/exception_handlers.py
+-rw-r--r--   0        0        0     4985 2024-05-12 00:38:13.722840 readyapi-0.110.3/readyapi/exceptions.py
+-rw-r--r--   0        0        0       55 2024-05-12 00:38:13.722840 readyapi-0.110.3/readyapi/logger.py
+-rw-r--r--   0        0        0       58 2024-05-12 00:38:13.722840 readyapi-0.110.3/readyapi/middleware/__init__.py
+-rw-r--r--   0        0        0       79 2024-05-12 00:38:13.722840 readyapi-0.110.3/readyapi/middleware/cors.py
+-rw-r--r--   0        0        0       79 2024-05-12 00:38:13.722840 readyapi-0.110.3/readyapi/middleware/gzip.py
+-rw-r--r--   0        0        0      115 2024-05-12 00:38:13.722840 readyapi-0.110.3/readyapi/middleware/httpsredirect.py
+-rw-r--r--   0        0        0      109 2024-05-12 00:38:13.722840 readyapi-0.110.3/readyapi/middleware/trustedhost.py
+-rw-r--r--   0        0        0       79 2024-05-12 00:38:13.722840 readyapi-0.110.3/readyapi/middleware/wsgi.py
+-rw-r--r--   0        0        0        0 2024-05-12 00:38:13.722840 readyapi-0.110.3/readyapi/openapi/__init__.py
+-rw-r--r--   0        0        0      153 2024-05-12 00:38:13.722840 readyapi-0.110.3/readyapi/openapi/constants.py
+-rw-r--r--   0        0        0    10379 2024-05-12 00:38:13.722840 readyapi-0.110.3/readyapi/openapi/docs.py
+-rw-r--r--   0        0        0    17765 2024-05-12 00:38:13.722840 readyapi-0.110.3/readyapi/openapi/models.py
+-rw-r--r--   0        0        0    22299 2024-05-12 00:38:13.722840 readyapi-0.110.3/readyapi/openapi/utils.py
+-rw-r--r--   0        0        0    64082 2024-05-12 00:38:13.722840 readyapi-0.110.3/readyapi/param_functions.py
+-rw-r--r--   0        0        0    28200 2024-05-12 00:38:13.722840 readyapi-0.110.3/readyapi/params.py
+-rw-r--r--   0        0        0        0 2024-05-12 00:38:13.722840 readyapi-0.110.3/readyapi/py.typed
+-rw-r--r--   0        0        0      142 2024-05-12 00:38:13.722840 readyapi-0.110.3/readyapi/requests.py
+-rw-r--r--   0        0        0     1769 2024-05-12 00:38:13.722840 readyapi-0.110.3/readyapi/responses.py
+-rw-r--r--   0        0        0   174906 2024-05-12 00:38:13.722840 readyapi-0.110.3/readyapi/routing.py
+-rw-r--r--   0        0        0      881 2024-05-12 00:38:13.722840 readyapi-0.110.3/readyapi/security/__init__.py
+-rw-r--r--   0        0        0     9382 2024-05-12 00:38:13.722840 readyapi-0.110.3/readyapi/security/api_key.py
+-rw-r--r--   0        0        0      142 2024-05-12 00:38:13.722840 readyapi-0.110.3/readyapi/security/base.py
+-rw-r--r--   0        0        0    13531 2024-05-12 00:38:13.722840 readyapi-0.110.3/readyapi/security/http.py
+-rw-r--r--   0        0        0    21618 2024-05-12 00:38:13.722840 readyapi-0.110.3/readyapi/security/oauth2.py
+-rw-r--r--   0        0        0     2724 2024-05-12 00:38:13.722840 readyapi-0.110.3/readyapi/security/open_id_connect_url.py
+-rw-r--r--   0        0        0      293 2024-05-12 00:38:13.722840 readyapi-0.110.3/readyapi/security/utils.py
+-rw-r--r--   0        0        0       69 2024-05-12 00:38:13.722840 readyapi-0.110.3/readyapi/staticfiles.py
+-rw-r--r--   0        0        0       76 2024-05-12 00:38:13.722840 readyapi-0.110.3/readyapi/templating.py
+-rw-r--r--   0        0        0       66 2024-05-12 00:38:13.722840 readyapi-0.110.3/readyapi/testclient.py
+-rw-r--r--   0        0        0      383 2024-05-12 00:38:13.722840 readyapi-0.110.3/readyapi/types.py
+-rw-r--r--   0        0        0     8044 2024-05-12 00:38:13.722840 readyapi-0.110.3/readyapi/utils.py
+-rw-r--r--   0        0        0      222 2024-05-12 00:38:13.722840 readyapi-0.110.3/readyapi/websockets.py
+-rw-r--r--   0        0        0       52 2024-05-12 00:38:13.722840 readyapi-0.110.3/requirements-docs-tests.txt
+-rw-r--r--   0        0        0      464 2024-05-12 00:38:13.722840 readyapi-0.110.3/requirements-docs.txt
+-rw-r--r--   0        0        0      496 2024-05-12 00:38:13.722840 readyapi-0.110.3/requirements-tests.txt
+-rw-r--r--   0        0        0      128 2024-05-12 00:38:13.722840 readyapi-0.110.3/requirements.txt
+-rwxr-xr-x   0        0        0    11141 2024-05-12 00:38:13.726840 readyapi-0.110.3/scripts/docs.py
+-rwxr-xr-x   0        0        0      114 2024-05-12 00:38:13.726840 readyapi-0.110.3/scripts/format.sh
+-rwxr-xr-x   0        0        0      128 2024-05-12 00:38:13.726840 readyapi-0.110.3/scripts/lint.sh
+-rw-r--r--   0        0        0     5216 2024-05-12 00:38:13.726840 readyapi-0.110.3/scripts/mkdocs_hooks.py
+-rw-r--r--   0        0        0      819 2024-05-12 00:38:13.726840 readyapi-0.110.3/scripts/playwright/separate_openapi_schemas/image01.py
+-rw-r--r--   0        0        0      873 2024-05-12 00:38:13.726840 readyapi-0.110.3/scripts/playwright/separate_openapi_schemas/image02.py
+-rw-r--r--   0        0        0      892 2024-05-12 00:38:13.726840 readyapi-0.110.3/scripts/playwright/separate_openapi_schemas/image03.py
+-rw-r--r--   0        0        0      881 2024-05-12 00:38:13.726840 readyapi-0.110.3/scripts/playwright/separate_openapi_schemas/image04.py
+-rw-r--r--   0        0        0      829 2024-05-12 00:38:13.726840 readyapi-0.110.3/scripts/playwright/separate_openapi_schemas/image05.py
+-rwxr-xr-x   0        0        0      124 2024-05-12 00:38:13.726840 readyapi-0.110.3/scripts/test-cov-html.sh
+-rwxr-xr-x   0        0        0       99 2024-05-12 00:38:13.726840 readyapi-0.110.3/scripts/test.sh
+-rw-r--r--   0        0        0        0 2024-05-12 00:38:13.726840 readyapi-0.110.3/tests/__init__.py
+-rw-r--r--   0        0        0     4455 2024-05-12 00:38:13.726840 readyapi-0.110.3/tests/main.py
+-rw-r--r--   0        0        0     3693 2024-05-12 00:38:13.726840 readyapi-0.110.3/tests/test_additional_properties.py
+-rw-r--r--   0        0        0     4307 2024-05-12 00:38:13.726840 readyapi-0.110.3/tests/test_additional_properties_bool.py
+-rw-r--r--   0        0        0     1212 2024-05-12 00:38:13.726840 readyapi-0.110.3/tests/test_additional_response_extra.py
+-rw-r--r--   0        0        0     1122 2024-05-12 00:38:13.726840 readyapi-0.110.3/tests/test_additional_responses_bad.py
+-rw-r--r--   0        0        0     5900 2024-05-12 00:38:13.726840 readyapi-0.110.3/tests/test_additional_responses_custom_model_in_callback.py
+-rw-r--r--   0        0        0     2980 2024-05-12 00:38:13.726840 readyapi-0.110.3/tests/test_additional_responses_custom_validationerror.py
+-rw-r--r--   0        0        0     2887 2024-05-12 00:38:13.726840 readyapi-0.110.3/tests/test_additional_responses_default_validationerror.py
+-rw-r--r--   0        0        0     3566 2024-05-12 00:38:13.726840 readyapi-0.110.3/tests/test_additional_responses_response_class.py
+-rw-r--r--   0        0        0     5234 2024-05-12 00:38:13.726840 readyapi-0.110.3/tests/test_additional_responses_router.py
+-rw-r--r--   0        0        0     2155 2024-05-12 00:38:13.726840 readyapi-0.110.3/tests/test_ambiguous_params.py
+-rw-r--r--   0        0        0    10500 2024-05-12 00:38:13.726840 readyapi-0.110.3/tests/test_annotated.py
+-rw-r--r--   0        0        0    53493 2024-05-12 00:38:13.726840 readyapi-0.110.3/tests/test_application.py
+-rw-r--r--   0        0        0      461 2024-05-12 00:38:13.726840 readyapi-0.110.3/tests/test_callable_endpoint.py
+-rw-r--r--   0        0        0     2832 2024-05-12 00:38:13.726840 readyapi-0.110.3/tests/test_compat.py
+-rw-r--r--   0        0        0     2269 2024-05-12 00:38:13.726840 readyapi-0.110.3/tests/test_computed_fields.py
+-rw-r--r--   0        0        0     2897 2024-05-12 00:38:13.726840 readyapi-0.110.3/tests/test_custom_middleware_exception.py
+-rw-r--r--   0        0        0     3137 2024-05-12 00:38:13.726840 readyapi-0.110.3/tests/test_custom_route_class.py
+-rw-r--r--   0        0        0     1251 2024-05-12 00:38:13.726840 readyapi-0.110.3/tests/test_custom_schema_fields.py
+-rw-r--r--   0        0        0     1095 2024-05-12 00:38:13.726840 readyapi-0.110.3/tests/test_custom_swagger_ui_redirect.py
+-rw-r--r--   0        0        0     2031 2024-05-12 00:38:13.726840 readyapi-0.110.3/tests/test_datastructures.py
+-rw-r--r--   0        0        0     1609 2024-05-12 00:38:13.726840 readyapi-0.110.3/tests/test_datetime_custom_encoder.py
+-rw-r--r--   0        0        0     5370 2024-05-12 00:38:13.726840 readyapi-0.110.3/tests/test_default_response_class.py
+-rw-r--r--   0        0        0     5122 2024-05-12 00:38:13.726840 readyapi-0.110.3/tests/test_default_response_class_router.py
+-rw-r--r--   0        0        0     2791 2024-05-12 00:38:13.726840 readyapi-0.110.3/tests/test_dependency_cache.py
+-rw-r--r--   0        0        0     3383 2024-05-12 00:38:13.726840 readyapi-0.110.3/tests/test_dependency_class.py
+-rw-r--r--   0        0        0    11874 2024-05-12 00:38:13.726840 readyapi-0.110.3/tests/test_dependency_contextmanager.py
+-rw-r--r--   0        0        0     1564 2024-05-12 00:38:13.726840 readyapi-0.110.3/tests/test_dependency_contextvars.py
+-rw-r--r--   0        0        0     8582 2024-05-12 00:38:13.726840 readyapi-0.110.3/tests/test_dependency_duplicates.py
+-rw-r--r--   0        0        0     1965 2024-05-12 00:38:13.726840 readyapi-0.110.3/tests/test_dependency_normal_exceptions.py
+-rw-r--r--   0        0        0    15820 2024-05-12 00:38:13.726840 readyapi-0.110.3/tests/test_dependency_overrides.py
+-rw-r--r--   0        0        0     1468 2024-05-12 00:38:13.726840 readyapi-0.110.3/tests/test_dependency_security_overrides.py
+-rw-r--r--   0        0        0     1198 2024-05-12 00:38:13.726840 readyapi-0.110.3/tests/test_deprecated_openapi_prefix.py
+-rw-r--r--   0        0        0     2164 2024-05-12 00:38:13.726840 readyapi-0.110.3/tests/test_duplicate_models_openapi.py
+-rw-r--r--   0        0        0      812 2024-05-12 00:38:13.726840 readyapi-0.110.3/tests/test_empty_router.py
+-rw-r--r--   0        0        0     3463 2024-05-12 00:38:13.726840 readyapi-0.110.3/tests/test_enforce_once_required_parameter.py
+-rw-r--r--   0        0        0     1923 2024-05-12 00:38:13.726840 readyapi-0.110.3/tests/test_exception_handlers.py
+-rw-r--r--   0        0        0    14039 2024-05-12 00:38:13.726840 readyapi-0.110.3/tests/test_extra_routes.py
+-rw-r--r--   0        0        0        0 2024-05-12 00:38:13.726840 readyapi-0.110.3/tests/test_filter_pydantic_sub_model/__init__.py
+-rw-r--r--   0        0        0      787 2024-05-12 00:38:13.726840 readyapi-0.110.3/tests/test_filter_pydantic_sub_model/app_pv1.py
+-rw-r--r--   0        0        0     4615 2024-05-12 00:38:13.726840 readyapi-0.110.3/tests/test_filter_pydantic_sub_model/test_filter_pydantic_sub_model_pv1.py
+-rw-r--r--   0        0        0     6467 2024-05-12 00:38:13.726840 readyapi-0.110.3/tests/test_filter_pydantic_sub_model_pv2.py
+-rw-r--r--   0        0        0     1206 2024-05-12 00:38:13.726840 readyapi-0.110.3/tests/test_forms_from_non_typing_sequences.py
+-rw-r--r--   0        0        0    68318 2024-05-12 00:38:13.726840 readyapi-0.110.3/tests/test_generate_unique_id_function.py
+-rw-r--r--   0        0        0     1886 2024-05-12 00:38:13.726840 readyapi-0.110.3/tests/test_generic_parameterless_depends.py
+-rw-r--r--   0        0        0     3749 2024-05-12 00:38:13.726840 readyapi-0.110.3/tests/test_get_request_body.py
+-rw-r--r--   0        0        0      977 2024-05-12 00:38:13.726840 readyapi-0.110.3/tests/test_http_connection_injection.py
+-rw-r--r--   0        0        0      501 2024-05-12 00:38:13.726840 readyapi-0.110.3/tests/test_include_route.py
+-rw-r--r--   0        0        0   367198 2024-05-12 00:38:13.726840 readyapi-0.110.3/tests/test_include_router_defaults_overrides.py
+-rw-r--r--   0        0        0    13624 2024-05-12 00:38:13.726840 readyapi-0.110.3/tests/test_infer_param_optionality.py
+-rw-r--r--   0        0        0     3090 2024-05-12 00:38:13.726840 readyapi-0.110.3/tests/test_inherited_custom_class.py
+-rw-r--r--   0        0        0     1713 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_invalid_path_param.py
+-rw-r--r--   0        0        0     1254 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_invalid_sequence_param.py
+-rw-r--r--   0        0        0     9184 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_jsonable_encoder.py
+-rw-r--r--   0        0        0     2507 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_local_docs.py
+-rw-r--r--   0        0        0        0 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_modules_same_name_body/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_modules_same_name_body/app/__init__.py
+-rw-r--r--   0        0        0      161 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_modules_same_name_body/app/a.py
+-rw-r--r--   0        0        0      162 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_modules_same_name_body/app/b.py
+-rw-r--r--   0        0        0      153 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_modules_same_name_body/app/main.py
+-rw-r--r--   0        0        0     5784 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_modules_same_name_body/test_main.py
+-rw-r--r--   0        0        0     7826 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_multi_body_errors.py
+-rw-r--r--   0        0        0     4615 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_multi_query_errors.py
+-rw-r--r--   0        0        0     3790 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_multipart_installation.py
+-rw-r--r--   0        0        0      790 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_no_swagger_ui_redirect.py
+-rw-r--r--   0        0        0    17443 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_openapi_examples.py
+-rw-r--r--   0        0        0     4852 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_openapi_query_parameter_extension.py
+-rw-r--r--   0        0        0     1138 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_openapi_route_extensions.py
+-rw-r--r--   0        0        0    18893 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_openapi_separate_input_output_schemas.py
+-rw-r--r--   0        0        0     2012 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_openapi_servers.py
+-rw-r--r--   0        0        0      937 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_operations_signatures.py
+-rw-r--r--   0        0        0      567 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_orjson_response_class.py
+-rw-r--r--   0        0        0      641 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_param_class.py
+-rw-r--r--   0        0        0     3142 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_param_in_path_and_dependency.py
+-rw-r--r--   0        0        0     7616 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_param_include_in_schema.py
+-rw-r--r--   0        0        0     3415 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_params_repr.py
+-rw-r--r--   0        0        0    35210 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_path.py
+-rw-r--r--   0        0        0     3367 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_put_no_body.py
+-rw-r--r--   0        0        0    11639 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_query.py
+-rw-r--r--   0        0        0     2420 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_read_with_orm_mode.py
+-rw-r--r--   0        0        0     6349 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_regex_deprecated_body.py
+-rw-r--r--   0        0        0     5600 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_regex_deprecated_params.py
+-rw-r--r--   0        0        0      796 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_repeated_cookie_headers.py
+-rw-r--r--   0        0        0     3253 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_repeated_dependency_schema.py
+-rw-r--r--   0        0        0     3750 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_repeated_parameter_alias.py
+-rw-r--r--   0        0        0     3213 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_reponse_set_reponse_code_empty.py
+-rw-r--r--   0        0        0     6514 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_request_body_parameters_media_type.py
+-rw-r--r--   0        0        0     1534 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_required_noneable.py
+-rw-r--r--   0        0        0    11385 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_response_by_alias.py
+-rw-r--r--   0        0        0      593 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_response_change_status_code.py
+-rw-r--r--   0        0        0     3421 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_response_class_no_mediatype.py
+-rw-r--r--   0        0        0     3321 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_response_code_no_body.py
+-rw-r--r--   0        0        0    48847 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_response_model_as_return_annotation.py
+-rw-r--r--   0        0        0     1730 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_response_model_data_filter.py
+-rw-r--r--   0        0        0     1750 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_response_model_data_filter_no_inheritance.py
+-rw-r--r--   0        0        0     4122 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_response_model_include_exclude.py
+-rw-r--r--   0        0        0     1136 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_response_model_invalid.py
+-rw-r--r--   0        0        0     5384 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_response_model_sub_types.py
+-rw-r--r--   0        0        0     1515 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_route_scope.py
+-rw-r--r--   0        0        0     3301 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_router_events.py
+-rw-r--r--   0        0        0      488 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_router_prefix_with_template.py
+-rw-r--r--   0        0        0      979 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_router_redirect_slashes.py
+-rw-r--r--   0        0        0    38582 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_schema_extra_examples.py
+-rw-r--r--   0        0        0     1950 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_security_api_key_cookie.py
+-rw-r--r--   0        0        0     2118 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_security_api_key_cookie_description.py
+-rw-r--r--   0        0        0     2152 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_security_api_key_cookie_optional.py
+-rw-r--r--   0        0        0     1890 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_security_api_key_header.py
+-rw-r--r--   0        0        0     2058 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_security_api_key_header_description.py
+-rw-r--r--   0        0        0     2088 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_security_api_key_header_optional.py
+-rw-r--r--   0        0        0     1869 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_security_api_key_query.py
+-rw-r--r--   0        0        0     2029 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_security_api_key_query_description.py
+-rw-r--r--   0        0        0     2067 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_security_api_key_query_optional.py
+-rw-r--r--   0        0        0     1793 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_security_http_base.py
+-rw-r--r--   0        0        0     1979 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_security_http_base_description.py
+-rw-r--r--   0        0        0     1938 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_security_http_base_optional.py
+-rw-r--r--   0        0        0     2677 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_security_http_basic_optional.py
+-rw-r--r--   0        0        0     2660 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_security_http_basic_realm.py
+-rw-r--r--   0        0        0     2836 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_security_http_basic_realm_description.py
+-rw-r--r--   0        0        0     2071 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_security_http_bearer.py
+-rw-r--r--   0        0        0     2261 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_security_http_bearer_description.py
+-rw-r--r--   0        0        0     2200 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_security_http_bearer_optional.py
+-rw-r--r--   0        0        0     2096 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_security_http_digest.py
+-rw-r--r--   0        0        0     2272 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_security_http_digest_description.py
+-rw-r--r--   0        0        0     2239 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_security_http_digest_optional.py
+-rw-r--r--   0        0        0    11008 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_security_oauth2.py
+-rw-r--r--   0        0        0     2344 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_security_oauth2_authorization_code_bearer.py
+-rw-r--r--   0        0        0     2448 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_security_oauth2_authorization_code_bearer_description.py
+-rw-r--r--   0        0        0    11049 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_security_oauth2_optional.py
+-rw-r--r--   0        0        0    11189 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_security_oauth2_optional_description.py
+-rw-r--r--   0        0        0     2153 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_security_oauth2_password_bearer_optional.py
+-rw-r--r--   0        0        0     2295 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_security_oauth2_password_bearer_optional_description.py
+-rw-r--r--   0        0        0     2296 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_security_openid_connect.py
+-rw-r--r--   0        0        0     2415 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_security_openid_connect_description.py
+-rw-r--r--   0        0        0     2494 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_security_openid_connect_optional.py
+-rw-r--r--   0        0        0     1418 2024-05-12 00:38:13.730840 readyapi-0.110.3/tests/test_serialize_response.py
+-rw-r--r--   0        0        0     5002 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_serialize_response_dataclass.py
+-rw-r--r--   0        0        0     4279 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_serialize_response_model.py
+-rw-r--r--   0        0        0     2075 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_skip_defaults.py
+-rw-r--r--   0        0        0     7555 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_starlette_exception.py
+-rw-r--r--   0        0        0     1714 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_starlette_urlconvertors.py
+-rw-r--r--   0        0        0    14147 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_sub_callbacks.py
+-rw-r--r--   0        0        0      722 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_swagger_ui_init_oauth.py
+-rw-r--r--   0        0        0    12073 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tuples.py
+-rw-r--r--   0        0        0        0 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_additional_responses/__init__.py
+-rw-r--r--   0        0        0     4434 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_additional_responses/test_tutorial001.py
+-rw-r--r--   0        0        0     4742 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_additional_responses/test_tutorial002.py
+-rw-r--r--   0        0        0     4658 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_additional_responses/test_tutorial003.py
+-rw-r--r--   0        0        0     4937 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_additional_responses/test_tutorial004.py
+-rw-r--r--   0        0        0        0 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_additional_status_codes/__init__.py
+-rw-r--r--   0        0        0      547 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_additional_status_codes/test_tutorial001.py
+-rw-r--r--   0        0        0      550 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_additional_status_codes/test_tutorial001_an.py
+-rw-r--r--   0        0        0      742 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_additional_status_codes/test_tutorial001_an_py310.py
+-rw-r--r--   0        0        0      738 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_additional_status_codes/test_tutorial001_an_py39.py
+-rw-r--r--   0        0        0      739 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_additional_status_codes/test_tutorial001_py310.py
+-rw-r--r--   0        0        0        0 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_advanced_middleware/__init__.py
+-rw-r--r--   0        0        0      475 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_advanced_middleware/test_tutorial001.py
+-rw-r--r--   0        0        0      571 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_advanced_middleware/test_tutorial002.py
+-rw-r--r--   0        0        0      667 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_advanced_middleware/test_tutorial003.py
+-rw-r--r--   0        0        0        0 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_async_sql_databases/__init__.py
+-rw-r--r--   0        0        0     6128 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_async_sql_databases/test_tutorial001.py
+-rw-r--r--   0        0        0        0 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_async_tests/__init__.py
+-rw-r--r--   0        0        0      143 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_async_tests/test_main.py
+-rw-r--r--   0        0        0        0 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_background_tasks/__init__.py
+-rw-r--r--   0        0        0      579 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_background_tasks/test_tutorial001.py
+-rw-r--r--   0        0        0      569 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_background_tasks/test_tutorial002.py
+-rw-r--r--   0        0        0      572 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_background_tasks/test_tutorial002_an.py
+-rw-r--r--   0        0        0      632 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_background_tasks/test_tutorial002_an_py310.py
+-rw-r--r--   0        0        0      629 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_background_tasks/test_tutorial002_an_py39.py
+-rw-r--r--   0        0        0      629 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_background_tasks/test_tutorial002_py310.py
+-rw-r--r--   0        0        0        0 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_behind_a_proxy/__init__.py
+-rw-r--r--   0        0        0     1055 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_behind_a_proxy/test_tutorial001.py
+-rw-r--r--   0        0        0     1034 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_behind_a_proxy/test_tutorial002.py
+-rw-r--r--   0        0        0     1690 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_behind_a_proxy/test_tutorial003.py
+-rw-r--r--   0        0        0     1658 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_behind_a_proxy/test_tutorial004.py
+-rw-r--r--   0        0        0        0 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_bigger_applications/__init__.py
+-rw-r--r--   0        0        0    25142 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_bigger_applications/test_main.py
+-rw-r--r--   0        0        0    25145 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_bigger_applications/test_main_an.py
+-rw-r--r--   0        0        0    25483 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_bigger_applications/test_main_an_py39.py
+-rw-r--r--   0        0        0        0 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_body/__init__.py
+-rw-r--r--   0        0        0    15094 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_body/test_tutorial001.py
+-rw-r--r--   0        0        0    15342 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_body/test_tutorial001_py310.py
+-rw-r--r--   0        0        0        0 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_body_fields/__init__.py
+-rw-r--r--   0        0        0     7343 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_body_fields/test_tutorial001.py
+-rw-r--r--   0        0        0     7346 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_body_fields/test_tutorial001_an.py
+-rw-r--r--   0        0        0     7438 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_body_fields/test_tutorial001_an_py310.py
+-rw-r--r--   0        0        0     7432 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_body_fields/test_tutorial001_an_py39.py
+-rw-r--r--   0        0        0     7435 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_body_fields/test_tutorial001_py310.py
+-rw-r--r--   0        0        0        0 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_body_multiple_params/__init__.py
+-rw-r--r--   0        0        0     7700 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_body_multiple_params/test_tutorial001.py
+-rw-r--r--   0        0        0     7703 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_body_multiple_params/test_tutorial001_an.py
+-rw-r--r--   0        0        0     7808 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_body_multiple_params/test_tutorial001_an_py310.py
+-rw-r--r--   0        0        0     7801 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_body_multiple_params/test_tutorial001_an_py39.py
+-rw-r--r--   0        0        0     7805 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_body_multiple_params/test_tutorial001_py310.py
+-rw-r--r--   0        0        0     9662 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_body_multiple_params/test_tutorial003.py
+-rw-r--r--   0        0        0     9665 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_body_multiple_params/test_tutorial003_an.py
+-rw-r--r--   0        0        0     9757 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_body_multiple_params/test_tutorial003_an_py310.py
+-rw-r--r--   0        0        0     9751 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_body_multiple_params/test_tutorial003_an_py39.py
+-rw-r--r--   0        0        0     9754 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_body_multiple_params/test_tutorial003_py310.py
+-rw-r--r--   0        0        0        0 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_body_nested_models/__init__.py
+-rw-r--r--   0        0        0     4345 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_body_nested_models/test_tutorial009.py
+-rw-r--r--   0        0        0     4419 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_body_nested_models/test_tutorial009_py39.py
+-rw-r--r--   0        0        0        0 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_body_updates/__init__.py
+-rw-r--r--   0        0        0    12043 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_body_updates/test_tutorial001.py
+-rw-r--r--   0        0        0    12114 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_body_updates/test_tutorial001_py310.py
+-rw-r--r--   0        0        0    12108 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_body_updates/test_tutorial001_py39.py
+-rw-r--r--   0        0        0        0 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_conditional_openapi/__init__.py
+-rw-r--r--   0        0        0     1801 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_conditional_openapi/test_tutorial001.py
+-rw-r--r--   0        0        0        0 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_configure_swagger_ui/__init__.py
+-rw-r--r--   0        0        0     1416 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_configure_swagger_ui/test_tutorial001.py
+-rw-r--r--   0        0        0     1563 2024-05-12 00:38:13.734840 readyapi-0.110.3/tests/test_tutorial/test_configure_swagger_ui/test_tutorial002.py
+-rw-r--r--   0        0        0     1535 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_configure_swagger_ui/test_tutorial003.py
+-rw-r--r--   0        0        0        0 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_cookie_params/__init__.py
+-rw-r--r--   0        0        0     4019 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_cookie_params/test_tutorial001.py
+-rw-r--r--   0        0        0     4022 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_cookie_params/test_tutorial001_an.py
+-rw-r--r--   0        0        0     4157 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_cookie_params/test_tutorial001_an_py310.py
+-rw-r--r--   0        0        0     4152 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_cookie_params/test_tutorial001_an_py39.py
+-rw-r--r--   0        0        0     4151 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_cookie_params/test_tutorial001_py310.py
+-rw-r--r--   0        0        0        0 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_cors/__init__.py
+-rw-r--r--   0        0        0     1287 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_cors/test_tutorial001.py
+-rw-r--r--   0        0        0        0 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_custom_docs_ui/__init__.py
+-rw-r--r--   0        0        0     1359 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_custom_docs_ui/test_tutorial001.py
+-rw-r--r--   0        0        0     1250 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_custom_docs_ui/test_tutorial002.py
+-rw-r--r--   0        0        0        0 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_custom_request_and_route/__init__.py
+-rw-r--r--   0        0        0      888 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_custom_request_and_route/test_tutorial001.py
+-rw-r--r--   0        0        0     1246 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_custom_request_and_route/test_tutorial002.py
+-rw-r--r--   0        0        0      527 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_custom_request_and_route/test_tutorial003.py
+-rw-r--r--   0        0        0        0 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_custom_response/__init__.py
+-rw-r--r--   0        0        0     1027 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_custom_response/test_tutorial001.py
+-rw-r--r--   0        0        0     1028 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_custom_response/test_tutorial001b.py
+-rw-r--r--   0        0        0     1223 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_custom_response/test_tutorial004.py
+-rw-r--r--   0        0        0      982 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_custom_response/test_tutorial005.py
+-rw-r--r--   0        0        0     1061 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_custom_response/test_tutorial006.py
+-rw-r--r--   0        0        0      909 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_custom_response/test_tutorial006b.py
+-rw-r--r--   0        0        0      901 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_custom_response/test_tutorial006c.py
+-rw-r--r--   0        0        0      265 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_custom_response/test_tutorial007.py
+-rw-r--r--   0        0        0      488 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_custom_response/test_tutorial008.py
+-rw-r--r--   0        0        0      488 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_custom_response/test_tutorial009.py
+-rw-r--r--   0        0        0      491 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_custom_response/test_tutorial009b.py
+-rw-r--r--   0        0        0      240 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_custom_response/test_tutorial009c.py
+-rw-r--r--   0        0        0        0 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_dataclasses/__init__.py
+-rw-r--r--   0        0        0     5291 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_dataclasses/test_tutorial001.py
+-rw-r--r--   0        0        0     3576 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_dataclasses/test_tutorial002.py
+-rw-r--r--   0        0        0    12359 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_dataclasses/test_tutorial003.py
+-rw-r--r--   0        0        0        0 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_dependencies/__init__.py
+-rw-r--r--   0        0        0     7221 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_dependencies/test_tutorial001.py
+-rw-r--r--   0        0        0     7224 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_dependencies/test_tutorial001_an.py
+-rw-r--r--   0        0        0     7404 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_dependencies/test_tutorial001_an_py310.py
+-rw-r--r--   0        0        0     7400 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_dependencies/test_tutorial001_an_py39.py
+-rw-r--r--   0        0        0     7401 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_dependencies/test_tutorial001_py310.py
+-rw-r--r--   0        0        0     5553 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_dependencies/test_tutorial004.py
+-rw-r--r--   0        0        0     5556 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_dependencies/test_tutorial004_an.py
+-rw-r--r--   0        0        0     5736 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_dependencies/test_tutorial004_an_py310.py
+-rw-r--r--   0        0        0     5732 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_dependencies/test_tutorial004_an_py39.py
+-rw-r--r--   0        0        0     5733 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_dependencies/test_tutorial004_py310.py
+-rw-r--r--   0        0        0     5121 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_dependencies/test_tutorial006.py
+-rw-r--r--   0        0        0     5124 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_dependencies/test_tutorial006_an.py
+-rw-r--r--   0        0        0     5402 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_dependencies/test_tutorial006_an_py39.py
+-rw-r--r--   0        0        0      698 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_dependencies/test_tutorial008b.py
+-rw-r--r--   0        0        0      701 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_dependencies/test_tutorial008b_an.py
+-rw-r--r--   0        0        0      919 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_dependencies/test_tutorial008b_an_py39.py
+-rw-r--r--   0        0        0     1171 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_dependencies/test_tutorial008c.py
+-rw-r--r--   0        0        0     1177 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_dependencies/test_tutorial008c_an.py
+-rw-r--r--   0        0        0     1268 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_dependencies/test_tutorial008c_an_py39.py
+-rw-r--r--   0        0        0     1227 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_dependencies/test_tutorial008d.py
+-rw-r--r--   0        0        0     1236 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_dependencies/test_tutorial008d_an.py
+-rw-r--r--   0        0        0     1332 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_dependencies/test_tutorial008d_an_py39.py
+-rw-r--r--   0        0        0     8640 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_dependencies/test_tutorial012.py
+-rw-r--r--   0        0        0     8643 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_dependencies/test_tutorial012_an.py
+-rw-r--r--   0        0        0     9041 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_dependencies/test_tutorial012_an_py39.py
+-rw-r--r--   0        0        0        0 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_events/__init__.py
+-rw-r--r--   0        0        0     3644 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_events/test_tutorial001.py
+-rw-r--r--   0        0        0     1420 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_events/test_tutorial002.py
+-rw-r--r--   0        0        0     3686 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_events/test_tutorial003.py
+-rw-r--r--   0        0        0        0 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_extending_openapi/__init__.py
+-rw-r--r--   0        0        0     1549 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_extending_openapi/test_tutorial001.py
+-rw-r--r--   0        0        0        0 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_extra_data_types/__init__.py
+-rw-r--r--   0        0        0     8029 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_extra_data_types/test_tutorial001.py
+-rw-r--r--   0        0        0     8032 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_extra_data_types/test_tutorial001_an.py
+-rw-r--r--   0        0        0     8224 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_extra_data_types/test_tutorial001_an_py310.py
+-rw-r--r--   0        0        0     8220 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_extra_data_types/test_tutorial001_an_py39.py
+-rw-r--r--   0        0        0     8221 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_extra_data_types/test_tutorial001_py310.py
+-rw-r--r--   0        0        0        0 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_extra_models/__init__.py
+-rw-r--r--   0        0        0     5197 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_extra_models/test_tutorial003.py
+-rw-r--r--   0        0        0     5420 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_extra_models/test_tutorial003_py310.py
+-rw-r--r--   0        0        0     1983 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_extra_models/test_tutorial004.py
+-rw-r--r--   0        0        0     2171 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_extra_models/test_tutorial004_py39.py
+-rw-r--r--   0        0        0     1482 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_extra_models/test_tutorial005.py
+-rw-r--r--   0        0        0     1670 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_extra_models/test_tutorial005_py39.py
+-rw-r--r--   0        0        0        0 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_first_steps/__init__.py
+-rw-r--r--   0        0        0     1207 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_first_steps/test_tutorial001.py
+-rw-r--r--   0        0        0        0 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_generate_clients/__init__.py
+-rw-r--r--   0        0        0     7249 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_generate_clients/test_tutorial003.py
+-rw-r--r--   0        0        0        0 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_handling_errors/__init__.py
+-rw-r--r--   0        0        0     3300 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_handling_errors/test_tutorial001.py
+-rw-r--r--   0        0        0     3373 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_handling_errors/test_tutorial002.py
+-rw-r--r--   0        0        0     3296 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_handling_errors/test_tutorial003.py
+-rw-r--r--   0        0        0     3802 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_handling_errors/test_tutorial004.py
+-rw-r--r--   0        0        0     4431 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_handling_errors/test_tutorial005.py
+-rw-r--r--   0        0        0     4074 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_handling_errors/test_tutorial006.py
+-rw-r--r--   0        0        0        0 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_header_params/__init__.py
+-rw-r--r--   0        0        0     3932 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_header_params/test_tutorial001.py
+-rw-r--r--   0        0        0     3935 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_header_params/test_tutorial001_an.py
+-rw-r--r--   0        0        0     4115 2024-05-12 00:38:13.738840 readyapi-0.110.3/tests/test_tutorial/test_header_params/test_tutorial001_an_py310.py
+-rw-r--r--   0        0        0     4112 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_header_params/test_tutorial001_py310.py
+-rw-r--r--   0        0        0     4099 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_header_params/test_tutorial002.py
+-rw-r--r--   0        0        0     4102 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_header_params/test_tutorial002_an.py
+-rw-r--r--   0        0        0     4282 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_header_params/test_tutorial002_an_py310.py
+-rw-r--r--   0        0        0     4353 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_header_params/test_tutorial002_an_py39.py
+-rw-r--r--   0        0        0     4352 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_header_params/test_tutorial002_py310.py
+-rw-r--r--   0        0        0     4242 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_header_params/test_tutorial003.py
+-rw-r--r--   0        0        0     4227 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_header_params/test_tutorial003_an.py
+-rw-r--r--   0        0        0     4407 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_header_params/test_tutorial003_an_py310.py
+-rw-r--r--   0        0        0     4403 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_header_params/test_tutorial003_an_py39.py
+-rw-r--r--   0        0        0     4404 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_header_params/test_tutorial003_py310.py
+-rw-r--r--   0        0        0        0 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_metadata/__init__.py
+-rw-r--r--   0        0        0     1765 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_metadata/test_tutorial001.py
+-rw-r--r--   0        0        0     1729 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_metadata/test_tutorial001_1.py
+-rw-r--r--   0        0        0     2082 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_metadata/test_tutorial004.py
+-rw-r--r--   0        0        0        0 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_openapi_callbacks/__init__.py
+-rw-r--r--   0        0        0     9218 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_openapi_callbacks/test_tutorial001.py
+-rw-r--r--   0        0        0        0 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_openapi_webhooks/__init__.py
+-rw-r--r--   0        0        0     4494 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_openapi_webhooks/test_tutorial001.py
+-rw-r--r--   0        0        0        0 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_path_operation_advanced_configurations/__init__.py
+-rw-r--r--   0        0        0     1039 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial001.py
+-rw-r--r--   0        0        0     1022 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial002.py
+-rw-r--r--   0        0        0      577 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial003.py
+-rw-r--r--   0        0        0     8918 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial004.py
+-rw-r--r--   0        0        0     1036 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial005.py
+-rw-r--r--   0        0        0     1989 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial006.py
+-rw-r--r--   0        0        0     3421 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial007.py
+-rw-r--r--   0        0        0     3268 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial007_pv1.py
+-rw-r--r--   0        0        0        0 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_path_operation_configurations/__init__.py
+-rw-r--r--   0        0        0     1724 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_path_operation_configurations/test_tutorial002b.py
+-rw-r--r--   0        0        0     8903 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_path_operation_configurations/test_tutorial005.py
+-rw-r--r--   0        0        0     9105 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_path_operation_configurations/test_tutorial005_py310.py
+-rw-r--r--   0        0        0     9100 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_path_operation_configurations/test_tutorial005_py39.py
+-rw-r--r--   0        0        0     2407 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_path_operation_configurations/test_tutorial006.py
+-rw-r--r--   0        0        0        0 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_path_params/__init__.py
+-rw-r--r--   0        0        0     3371 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_path_params/test_tutorial004.py
+-rw-r--r--   0        0        0     5144 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_path_params/test_tutorial005.py
+-rw-r--r--   0        0        0        0 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_query_params/__init__.py
+-rw-r--r--   0        0        0     4074 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_query_params/test_tutorial005.py
+-rw-r--r--   0        0        0     6287 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_query_params/test_tutorial006.py
+-rw-r--r--   0        0        0     6366 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_query_params/test_tutorial006_py310.py
+-rw-r--r--   0        0        0        0 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_query_params_str_validations/__init__.py
+-rw-r--r--   0        0        0     6390 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_query_params_str_validations/test_tutorial010.py
+-rw-r--r--   0        0        0     6393 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_query_params_str_validations/test_tutorial010_an.py
+-rw-r--r--   0        0        0     6498 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_query_params_str_validations/test_tutorial010_an_py310.py
+-rw-r--r--   0        0        0     6491 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_query_params_str_validations/test_tutorial010_an_py39.py
+-rw-r--r--   0        0        0     6495 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_query_params_str_validations/test_tutorial010_py310.py
+-rw-r--r--   0        0        0     4019 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_query_params_str_validations/test_tutorial011.py
+-rw-r--r--   0        0        0     4022 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_query_params_str_validations/test_tutorial011_an.py
+-rw-r--r--   0        0        0     4245 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_query_params_str_validations/test_tutorial011_an_py310.py
+-rw-r--r--   0        0        0     4240 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_query_params_str_validations/test_tutorial011_an_py39.py
+-rw-r--r--   0        0        0     4242 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_query_params_str_validations/test_tutorial011_py310.py
+-rw-r--r--   0        0        0     4237 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_query_params_str_validations/test_tutorial011_py39.py
+-rw-r--r--   0        0        0     3487 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_query_params_str_validations/test_tutorial012.py
+-rw-r--r--   0        0        0     3490 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_query_params_str_validations/test_tutorial012_an.py
+-rw-r--r--   0        0        0     3708 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_query_params_str_validations/test_tutorial012_an_py39.py
+-rw-r--r--   0        0        0     3705 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_query_params_str_validations/test_tutorial012_py39.py
+-rw-r--r--   0        0        0     3436 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_query_params_str_validations/test_tutorial013.py
+-rw-r--r--   0        0        0     3439 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_query_params_str_validations/test_tutorial013_an.py
+-rw-r--r--   0        0        0     3657 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_query_params_str_validations/test_tutorial013_an_py39.py
+-rw-r--r--   0        0        0     2939 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_query_params_str_validations/test_tutorial014.py
+-rw-r--r--   0        0        0     2942 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_query_params_str_validations/test_tutorial014_an.py
+-rw-r--r--   0        0        0     3165 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_query_params_str_validations/test_tutorial014_an_py310.py
+-rw-r--r--   0        0        0     3164 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_query_params_str_validations/test_tutorial014_an_py39.py
+-rw-r--r--   0        0        0     3162 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_query_params_str_validations/test_tutorial014_py310.py
+-rw-r--r--   0        0        0        0 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_request_files/__init__.py
+-rw-r--r--   0        0        0     7888 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_request_files/test_tutorial001.py
+-rw-r--r--   0        0        0     8390 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_request_files/test_tutorial001_02.py
+-rw-r--r--   0        0        0     8393 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_request_files/test_tutorial001_02_an.py
+-rw-r--r--   0        0        0     8662 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_request_files/test_tutorial001_02_an_py310.py
+-rw-r--r--   0        0        0     8655 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_request_files/test_tutorial001_02_an_py39.py
+-rw-r--r--   0        0        0     8659 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_request_files/test_tutorial001_02_py310.py
+-rw-r--r--   0        0        0     6135 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_request_files/test_tutorial001_03.py
+-rw-r--r--   0        0        0     6138 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_request_files/test_tutorial001_03_an.py
+-rw-r--r--   0        0        0     6302 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_request_files/test_tutorial001_03_an_py39.py
+-rw-r--r--   0        0        0     7710 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_request_files/test_tutorial001_an.py
+-rw-r--r--   0        0        0     7937 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_request_files/test_tutorial001_an_py39.py
+-rw-r--r--   0        0        0     8681 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_request_files/test_tutorial002.py
+-rw-r--r--   0        0        0     8684 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_request_files/test_tutorial002_an.py
+-rw-r--r--   0        0        0     9084 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_request_files/test_tutorial002_an_py39.py
+-rw-r--r--   0        0        0     9263 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_request_files/test_tutorial002_py39.py
+-rw-r--r--   0        0        0     7313 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_request_files/test_tutorial003.py
+-rw-r--r--   0        0        0     7316 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_request_files/test_tutorial003_an.py
+-rw-r--r--   0        0        0     7838 2024-05-12 00:38:13.742840 readyapi-0.110.3/tests/test_tutorial/test_request_files/test_tutorial003_an_py39.py
+-rw-r--r--   0        0        0     7835 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_request_files/test_tutorial003_py39.py
+-rw-r--r--   0        0        0        0 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_request_forms/__init__.py
+-rw-r--r--   0        0        0     7632 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_request_forms/test_tutorial001.py
+-rw-r--r--   0        0        0     7635 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_request_forms/test_tutorial001_an.py
+-rw-r--r--   0        0        0     7745 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_request_forms/test_tutorial001_an_py39.py
+-rw-r--r--   0        0        0        0 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_request_forms_and_files/__init__.py
+-rw-r--r--   0        0        0    10049 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_request_forms_and_files/test_tutorial001.py
+-rw-r--r--   0        0        0    10052 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_request_forms_and_files/test_tutorial001_an.py
+-rw-r--r--   0        0        0    10162 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_request_forms_and_files/test_tutorial001_an_py39.py
+-rw-r--r--   0        0        0        0 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_response_change_status_code/__init__.py
+-rw-r--r--   0        0        0      522 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_response_change_status_code/test_tutorial001.py
+-rw-r--r--   0        0        0        0 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_response_cookies/__init__.py
+-rw-r--r--   0        0        0      404 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_response_cookies/test_tutorial001.py
+-rw-r--r--   0        0        0      415 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_response_cookies/test_tutorial002.py
+-rw-r--r--   0        0        0        0 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_response_headers/__init__.py
+-rw-r--r--   0        0        0      427 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_response_headers/test_tutorial001.py
+-rw-r--r--   0        0        0      379 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_response_headers/test_tutorial002.py
+-rw-r--r--   0        0        0        0 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_response_model/__init__.py
+-rw-r--r--   0        0        0     5766 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_response_model/test_tutorial003.py
+-rw-r--r--   0        0        0     5772 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_response_model/test_tutorial003_01.py
+-rw-r--r--   0        0        0     5964 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_response_model/test_tutorial003_01_py310.py
+-rw-r--r--   0        0        0     3478 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_response_model/test_tutorial003_02.py
+-rw-r--r--   0        0        0     1092 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_response_model/test_tutorial003_03.py
+-rw-r--r--   0        0        0      239 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_response_model/test_tutorial003_04.py
+-rw-r--r--   0        0        0      292 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_response_model/test_tutorial003_04_py310.py
+-rw-r--r--   0        0        0     3478 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_response_model/test_tutorial003_05.py
+-rw-r--r--   0        0        0     3701 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_response_model/test_tutorial003_05_py310.py
+-rw-r--r--   0        0        0     5958 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_response_model/test_tutorial003_py310.py
+-rw-r--r--   0        0        0     5110 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_response_model/test_tutorial004.py
+-rw-r--r--   0        0        0     5290 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_response_model/test_tutorial004_py310.py
+-rw-r--r--   0        0        0     5286 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_response_model/test_tutorial004_py39.py
+-rw-r--r--   0        0        0     6156 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_response_model/test_tutorial005.py
+-rw-r--r--   0        0        0     6379 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_response_model/test_tutorial005_py310.py
+-rw-r--r--   0        0        0     6156 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_response_model/test_tutorial006.py
+-rw-r--r--   0        0        0     6379 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_response_model/test_tutorial006_py310.py
+-rw-r--r--   0        0        0        0 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_schema_extra_example/__init__.py
+-rw-r--r--   0        0        0     4781 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_schema_extra_example/test_tutorial001.py
+-rw-r--r--   0        0        0     4557 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_schema_extra_example/test_tutorial001_pv1.py
+-rw-r--r--   0        0        0     4826 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_schema_extra_example/test_tutorial001_py310.py
+-rw-r--r--   0        0        0     4602 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_schema_extra_example/test_tutorial001_py310_pv1.py
+-rw-r--r--   0        0        0     7062 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_schema_extra_example/test_tutorial004.py
+-rw-r--r--   0        0        0     7065 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_schema_extra_example/test_tutorial004_an.py
+-rw-r--r--   0        0        0     7257 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_schema_extra_example/test_tutorial004_an_py310.py
+-rw-r--r--   0        0        0     7253 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_schema_extra_example/test_tutorial004_an_py39.py
+-rw-r--r--   0        0        0     7254 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_schema_extra_example/test_tutorial004_py310.py
+-rw-r--r--   0        0        0     6910 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_schema_extra_example/test_tutorial005.py
+-rw-r--r--   0        0        0     6913 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_schema_extra_example/test_tutorial005_an.py
+-rw-r--r--   0        0        0     6979 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_schema_extra_example/test_tutorial005_an_py310.py
+-rw-r--r--   0        0        0     6975 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_schema_extra_example/test_tutorial005_an_py39.py
+-rw-r--r--   0        0        0     6976 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_schema_extra_example/test_tutorial005_py310.py
+-rw-r--r--   0        0        0        0 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_security/__init__.py
+-rw-r--r--   0        0        0     1907 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_security/test_tutorial001.py
+-rw-r--r--   0        0        0     1910 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_security/test_tutorial001_an.py
+-rw-r--r--   0        0        0     2158 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_security/test_tutorial001_an_py39.py
+-rw-r--r--   0        0        0     8184 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_security/test_tutorial003.py
+-rw-r--r--   0        0        0     8187 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_security/test_tutorial003_an.py
+-rw-r--r--   0        0        0     8596 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_security/test_tutorial003_an_py310.py
+-rw-r--r--   0        0        0     8585 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_security/test_tutorial003_an_py39.py
+-rw-r--r--   0        0        0     8593 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_security/test_tutorial003_py310.py
+-rw-r--r--   0        0        0    15805 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_security/test_tutorial005.py
+-rw-r--r--   0        0        0    15808 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_security/test_tutorial005_an.py
+-rw-r--r--   0        0        0    16713 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_security/test_tutorial005_an_py310.py
+-rw-r--r--   0        0        0    16689 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_security/test_tutorial005_an_py39.py
+-rw-r--r--   0        0        0    16701 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_security/test_tutorial005_py310.py
+-rw-r--r--   0        0        0    16677 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_security/test_tutorial005_py39.py
+-rw-r--r--   0        0        0     2320 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_security/test_tutorial006.py
+-rw-r--r--   0        0        0     2323 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_security/test_tutorial006_an.py
+-rw-r--r--   0        0        0     2596 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_security/test_tutorial006_an_py39.py
+-rw-r--r--   0        0        0        0 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_separate_openapi_schemas/__init__.py
+-rw-r--r--   0        0        0     4960 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_separate_openapi_schemas/test_tutorial001.py
+-rw-r--r--   0        0        0     5018 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_separate_openapi_schemas/test_tutorial001_py310.py
+-rw-r--r--   0        0        0     5013 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_separate_openapi_schemas/test_tutorial001_py39.py
+-rw-r--r--   0        0        0     4960 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_separate_openapi_schemas/test_tutorial002.py
+-rw-r--r--   0        0        0     5018 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_separate_openapi_schemas/test_tutorial002_py310.py
+-rw-r--r--   0        0        0     5013 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_separate_openapi_schemas/test_tutorial002_py39.py
+-rw-r--r--   0        0        0        0 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_settings/__init__.py
+-rw-r--r--   0        0        0      488 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_settings/test_app02.py
+-rw-r--r--   0        0        0      553 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_settings/test_tutorial001.py
+-rw-r--r--   0        0        0      557 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_settings/test_tutorial001_pv1.py
+-rw-r--r--   0        0        0        0 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_sql_databases/__init__.py
+-rw-r--r--   0        0        0    16477 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_sql_databases/test_sql_databases.py
+-rw-r--r--   0        0        0    16656 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_sql_databases/test_sql_databases_middleware.py
+-rw-r--r--   0        0        0    16926 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_sql_databases/test_sql_databases_middleware_py310.py
+-rw-r--r--   0        0        0    16927 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_sql_databases/test_sql_databases_middleware_py39.py
+-rw-r--r--   0        0        0    16932 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_sql_databases/test_sql_databases_py310.py
+-rw-r--r--   0        0        0    16923 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_sql_databases/test_sql_databases_py39.py
+-rw-r--r--   0        0        0      788 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_sql_databases/test_testing_databases.py
+-rw-r--r--   0        0        0      825 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_sql_databases/test_testing_databases_py310.py
+-rw-r--r--   0        0        0      822 2024-05-12 00:38:13.746840 readyapi-0.110.3/tests/test_tutorial/test_sql_databases/test_testing_databases_py39.py
+-rw-r--r--   0        0        0        0 2024-05-12 00:38:13.750840 readyapi-0.110.3/tests/test_tutorial/test_sub_applications/__init__.py
+-rw-r--r--   0        0        0     1923 2024-05-12 00:38:13.750840 readyapi-0.110.3/tests/test_tutorial/test_sub_applications/test_tutorial001.py
+-rw-r--r--   0        0        0        0 2024-05-12 00:38:13.750840 readyapi-0.110.3/tests/test_tutorial/test_templates/__init__.py
+-rw-r--r--   0        0        0      911 2024-05-12 00:38:13.750840 readyapi-0.110.3/tests/test_tutorial/test_templates/test_tutorial001.py
+-rw-r--r--   0        0        0        0 2024-05-12 00:38:13.750840 readyapi-0.110.3/tests/test_tutorial/test_testing/__init__.py
+-rw-r--r--   0        0        0      820 2024-05-12 00:38:13.750840 readyapi-0.110.3/tests/test_tutorial/test_testing/test_main.py
+-rw-r--r--   0        0        0      300 2024-05-12 00:38:13.750840 readyapi-0.110.3/tests/test_tutorial/test_testing/test_main_b.py
+-rw-r--r--   0        0        0      303 2024-05-12 00:38:13.750840 readyapi-0.110.3/tests/test_tutorial/test_testing/test_main_b_an.py
+-rw-r--r--   0        0        0      360 2024-05-12 00:38:13.750840 readyapi-0.110.3/tests/test_tutorial/test_testing/test_main_b_an_py310.py
+-rw-r--r--   0        0        0      357 2024-05-12 00:38:13.750840 readyapi-0.110.3/tests/test_tutorial/test_testing/test_main_b_an_py39.py
+-rw-r--r--   0        0        0      357 2024-05-12 00:38:13.750840 readyapi-0.110.3/tests/test_tutorial/test_testing/test_main_b_py310.py
+-rw-r--r--   0        0        0      822 2024-05-12 00:38:13.750840 readyapi-0.110.3/tests/test_tutorial/test_testing/test_tutorial001.py
+-rw-r--r--   0        0        0      154 2024-05-12 00:38:13.750840 readyapi-0.110.3/tests/test_tutorial/test_testing/test_tutorial002.py
+-rw-r--r--   0        0        0      167 2024-05-12 00:38:13.750840 readyapi-0.110.3/tests/test_tutorial/test_testing/test_tutorial003.py
+-rw-r--r--   0        0        0        0 2024-05-12 00:38:13.750840 readyapi-0.110.3/tests/test_tutorial/test_testing_dependencies/__init__.py
+-rw-r--r--   0        0        0     1527 2024-05-12 00:38:13.750840 readyapi-0.110.3/tests/test_tutorial/test_testing_dependencies/test_tutorial001.py
+-rw-r--r--   0        0        0     1530 2024-05-12 00:38:13.750840 readyapi-0.110.3/tests/test_tutorial/test_testing_dependencies/test_tutorial001_an.py
+-rw-r--r--   0        0        0     2088 2024-05-12 00:38:13.750840 readyapi-0.110.3/tests/test_tutorial/test_testing_dependencies/test_tutorial001_an_py310.py
+-rw-r--r--   0        0        0     2073 2024-05-12 00:38:13.750840 readyapi-0.110.3/tests/test_tutorial/test_testing_dependencies/test_tutorial001_an_py39.py
+-rw-r--r--   0        0        0     2067 2024-05-12 00:38:13.750840 readyapi-0.110.3/tests/test_tutorial/test_testing_dependencies/test_tutorial001_py310.py
+-rw-r--r--   0        0        0        0 2024-05-12 00:38:13.750840 readyapi-0.110.3/tests/test_tutorial/test_websockets/__init__.py
+-rw-r--r--   0        0        0      824 2024-05-12 00:38:13.750840 readyapi-0.110.3/tests/test_tutorial/test_websockets/test_tutorial001.py
+-rw-r--r--   0        0        0     3685 2024-05-12 00:38:13.750840 readyapi-0.110.3/tests/test_tutorial/test_websockets/test_tutorial002.py
+-rw-r--r--   0        0        0     3688 2024-05-12 00:38:13.750840 readyapi-0.110.3/tests/test_tutorial/test_websockets/test_tutorial002_an.py
+-rw-r--r--   0        0        0     3978 2024-05-12 00:38:13.750840 readyapi-0.110.3/tests/test_tutorial/test_websockets/test_tutorial002_an_py310.py
+-rw-r--r--   0        0        0     3970 2024-05-12 00:38:13.750840 readyapi-0.110.3/tests/test_tutorial/test_websockets/test_tutorial002_an_py39.py
+-rw-r--r--   0        0        0     3975 2024-05-12 00:38:13.750840 readyapi-0.110.3/tests/test_tutorial/test_websockets/test_tutorial002_py310.py
+-rw-r--r--   0        0        0      873 2024-05-12 00:38:13.750840 readyapi-0.110.3/tests/test_tutorial/test_websockets/test_tutorial003.py
+-rw-r--r--   0        0        0     1292 2024-05-12 00:38:13.750840 readyapi-0.110.3/tests/test_tutorial/test_websockets/test_tutorial003_py39.py
+-rw-r--r--   0        0        0        0 2024-05-12 00:38:13.750840 readyapi-0.110.3/tests/test_tutorial/test_wsgi/__init__.py
+-rw-r--r--   0        0        0      437 2024-05-12 00:38:13.750840 readyapi-0.110.3/tests/test_tutorial/test_wsgi/test_tutorial001.py
+-rw-r--r--   0        0        0      713 2024-05-12 00:38:13.750840 readyapi-0.110.3/tests/test_typing_python39.py
+-rw-r--r--   0        0        0     4753 2024-05-12 00:38:13.750840 readyapi-0.110.3/tests/test_union_body.py
+-rw-r--r--   0        0        0     5316 2024-05-12 00:38:13.750840 readyapi-0.110.3/tests/test_union_inherited_body.py
+-rw-r--r--   0        0        0     2036 2024-05-12 00:38:13.750840 readyapi-0.110.3/tests/test_validate_response.py
+-rw-r--r--   0        0        0     1213 2024-05-12 00:38:13.750840 readyapi-0.110.3/tests/test_validate_response_dataclass.py
+-rw-r--r--   0        0        0        0 2024-05-12 00:38:13.750840 readyapi-0.110.3/tests/test_validate_response_recursive/__init__.py
+-rw-r--r--   0        0        0     1152 2024-05-12 00:38:13.750840 readyapi-0.110.3/tests/test_validate_response_recursive/app_pv1.py
+-rw-r--r--   0        0        0     1181 2024-05-12 00:38:13.750840 readyapi-0.110.3/tests/test_validate_response_recursive/app_pv2.py
+-rw-r--r--   0        0        0      901 2024-05-12 00:38:13.750840 readyapi-0.110.3/tests/test_validate_response_recursive/test_validate_response_recursive_pv1.py
+-rw-r--r--   0        0        0      901 2024-05-12 00:38:13.750840 readyapi-0.110.3/tests/test_validate_response_recursive/test_validate_response_recursive_pv2.py
+-rw-r--r--   0        0        0     4673 2024-05-12 00:38:13.750840 readyapi-0.110.3/tests/test_webhooks_security.py
+-rw-r--r--   0        0        0     2203 2024-05-12 00:38:13.750840 readyapi-0.110.3/tests/test_ws_dependencies.py
+-rw-r--r--   0        0        0     7657 2024-05-12 00:38:13.750840 readyapi-0.110.3/tests/test_ws_router.py
+-rw-r--r--   0        0        0      423 2024-05-12 00:38:13.750840 readyapi-0.110.3/tests/utils.py
+-rw-r--r--   0        0        0    25444 1970-01-01 00:00:00.000000 readyapi-0.110.3/PKG-INFO
```

### Comparing `readyapi-0.110.2.dev1/LICENSE` & `readyapi-0.110.3/LICENSE`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/README.md` & `readyapi-0.110.3/README.md`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs/en/docs/img/favicon.png` & `readyapi-0.110.3/docs/en/docs/img/favicon.png`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/additional_responses/tutorial002.py` & `readyapi-0.110.3/docs_src/additional_responses/tutorial002.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/additional_responses/tutorial003.py` & `readyapi-0.110.3/docs_src/additional_responses/tutorial003.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/additional_responses/tutorial004.py` & `readyapi-0.110.3/docs_src/additional_responses/tutorial004.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/additional_status_codes/tutorial001.py` & `readyapi-0.110.3/docs_src/additional_status_codes/tutorial001.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/additional_status_codes/tutorial001_an.py` & `readyapi-0.110.3/docs_src/additional_status_codes/tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/additional_status_codes/tutorial001_an_py310.py` & `readyapi-0.110.3/docs_src/additional_status_codes/tutorial001_an_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/additional_status_codes/tutorial001_an_py39.py` & `readyapi-0.110.3/docs_src/additional_status_codes/tutorial001_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/additional_status_codes/tutorial001_py310.py` & `readyapi-0.110.3/docs_src/additional_status_codes/tutorial001_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/app_testing/app_b/main.py` & `readyapi-0.110.3/docs_src/app_testing/app_b/main.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/app_testing/app_b/test_main.py` & `readyapi-0.110.3/docs_src/app_testing/app_b/test_main.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/app_testing/app_b_an/main.py` & `readyapi-0.110.3/docs_src/app_testing/app_b_an/main.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/app_testing/app_b_an/test_main.py` & `readyapi-0.110.3/docs_src/app_testing/app_b_an/test_main.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/app_testing/app_b_an_py310/main.py` & `readyapi-0.110.3/docs_src/app_testing/app_b_an_py310/main.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/app_testing/app_b_an_py310/test_main.py` & `readyapi-0.110.3/docs_src/app_testing/app_b_an_py310/test_main.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/app_testing/app_b_an_py39/main.py` & `readyapi-0.110.3/docs_src/app_testing/app_b_an_py39/main.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/app_testing/app_b_an_py39/test_main.py` & `readyapi-0.110.3/docs_src/app_testing/app_b_an_py39/test_main.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/app_testing/app_b_py310/main.py` & `readyapi-0.110.3/docs_src/app_testing/app_b_py310/main.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/app_testing/app_b_py310/test_main.py` & `readyapi-0.110.3/docs_src/app_testing/app_b_py310/test_main.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/app_testing/tutorial002.py` & `readyapi-0.110.3/docs_src/app_testing/tutorial002.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/app_testing/tutorial003.py` & `readyapi-0.110.3/docs_src/app_testing/tutorial003.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/async_sql_databases/tutorial001.py` & `readyapi-0.110.3/docs_src/async_sql_databases/tutorial001.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/background_tasks/tutorial001.py` & `readyapi-0.110.3/docs_src/background_tasks/tutorial001.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/background_tasks/tutorial002.py` & `readyapi-0.110.3/docs_src/background_tasks/tutorial002.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/background_tasks/tutorial002_an.py` & `readyapi-0.110.3/docs_src/background_tasks/tutorial002_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/background_tasks/tutorial002_an_py310.py` & `readyapi-0.110.3/docs_src/background_tasks/tutorial002_an_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/background_tasks/tutorial002_an_py39.py` & `readyapi-0.110.3/docs_src/background_tasks/tutorial002_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/background_tasks/tutorial002_py310.py` & `readyapi-0.110.3/docs_src/background_tasks/tutorial002_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/bigger_applications/app/main.py` & `readyapi-0.110.3/docs_src/bigger_applications/app/main.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/bigger_applications/app/routers/items.py` & `readyapi-0.110.3/docs_src/bigger_applications/app/routers/items.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/bigger_applications/app_an/main.py` & `readyapi-0.110.3/docs_src/bigger_applications/app_an/main.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/bigger_applications/app_an/routers/items.py` & `readyapi-0.110.3/docs_src/bigger_applications/app_an/routers/items.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/bigger_applications/app_an_py39/main.py` & `readyapi-0.110.3/docs_src/bigger_applications/app_an_py39/main.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/bigger_applications/app_an_py39/routers/items.py` & `readyapi-0.110.3/docs_src/bigger_applications/app_an_py39/routers/items.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/body_fields/tutorial001.py` & `readyapi-0.110.3/docs_src/body_fields/tutorial001.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/body_fields/tutorial001_an.py` & `readyapi-0.110.3/docs_src/body_fields/tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/body_fields/tutorial001_an_py310.py` & `readyapi-0.110.3/docs_src/body_fields/tutorial001_an_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/body_fields/tutorial001_an_py39.py` & `readyapi-0.110.3/docs_src/body_fields/tutorial001_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/body_fields/tutorial001_py310.py` & `readyapi-0.110.3/docs_src/body_fields/tutorial001_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/body_multiple_params/tutorial001.py` & `readyapi-0.110.3/docs_src/body_multiple_params/tutorial001.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/body_multiple_params/tutorial001_an.py` & `readyapi-0.110.3/docs_src/body_multiple_params/tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/body_multiple_params/tutorial001_an_py310.py` & `readyapi-0.110.3/docs_src/body_multiple_params/tutorial001_an_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/body_multiple_params/tutorial001_an_py39.py` & `readyapi-0.110.3/docs_src/body_multiple_params/tutorial001_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/body_multiple_params/tutorial001_py310.py` & `readyapi-0.110.3/docs_src/body_multiple_params/tutorial001_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/body_multiple_params/tutorial003.py` & `readyapi-0.110.3/docs_src/body_multiple_params/tutorial003.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/body_multiple_params/tutorial003_an.py` & `readyapi-0.110.3/docs_src/body_multiple_params/tutorial003_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/body_multiple_params/tutorial003_an_py310.py` & `readyapi-0.110.3/docs_src/body_multiple_params/tutorial003_an_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/body_multiple_params/tutorial003_an_py39.py` & `readyapi-0.110.3/docs_src/body_multiple_params/tutorial003_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/body_multiple_params/tutorial004.py` & `readyapi-0.110.3/docs_src/body_multiple_params/tutorial004.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/body_multiple_params/tutorial004_an.py` & `readyapi-0.110.3/docs_src/body_multiple_params/tutorial004_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/body_multiple_params/tutorial004_an_py310.py` & `readyapi-0.110.3/docs_src/body_multiple_params/tutorial004_an_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/body_multiple_params/tutorial004_an_py39.py` & `readyapi-0.110.3/docs_src/body_multiple_params/tutorial004_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/body_multiple_params/tutorial004_py310.py` & `readyapi-0.110.3/docs_src/body_multiple_params/tutorial004_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/body_nested_models/tutorial005.py` & `readyapi-0.110.3/docs_src/body_nested_models/tutorial005.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/body_nested_models/tutorial005_py39.py` & `readyapi-0.110.3/docs_src/body_nested_models/tutorial005_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/body_nested_models/tutorial006.py` & `readyapi-0.110.3/docs_src/body_nested_models/tutorial006.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/body_nested_models/tutorial006_py39.py` & `readyapi-0.110.3/docs_src/body_nested_models/tutorial006_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/body_nested_models/tutorial007.py` & `readyapi-0.110.3/docs_src/body_nested_models/tutorial007.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/body_nested_models/tutorial007_py310.py` & `readyapi-0.110.3/docs_src/body_nested_models/tutorial007_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/body_nested_models/tutorial007_py39.py` & `readyapi-0.110.3/docs_src/body_nested_models/tutorial007_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/body_updates/tutorial001.py` & `readyapi-0.110.3/docs_src/body_updates/tutorial001.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/body_updates/tutorial001_py310.py` & `readyapi-0.110.3/docs_src/body_updates/tutorial001_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/body_updates/tutorial001_py39.py` & `readyapi-0.110.3/docs_src/body_updates/tutorial001_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/body_updates/tutorial002.py` & `readyapi-0.110.3/docs_src/body_updates/tutorial002.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/body_updates/tutorial002_py310.py` & `readyapi-0.110.3/docs_src/body_updates/tutorial002_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/body_updates/tutorial002_py39.py` & `readyapi-0.110.3/docs_src/body_updates/tutorial002_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/custom_docs_ui/tutorial001.py` & `readyapi-0.110.3/docs_src/custom_docs_ui/tutorial001.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/custom_docs_ui/tutorial002.py` & `readyapi-0.110.3/docs_src/custom_docs_ui/tutorial002.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/custom_request_and_route/tutorial001.py` & `readyapi-0.110.3/docs_src/custom_request_and_route/tutorial001.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/custom_request_and_route/tutorial002.py` & `readyapi-0.110.3/docs_src/custom_request_and_route/tutorial002.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/custom_request_and_route/tutorial003.py` & `readyapi-0.110.3/docs_src/custom_request_and_route/tutorial003.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/dataclasses/tutorial002.py` & `readyapi-0.110.3/docs_src/dataclasses/tutorial002.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/dataclasses/tutorial003.py` & `readyapi-0.110.3/docs_src/dataclasses/tutorial003.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/dependencies/tutorial002.py` & `readyapi-0.110.3/docs_src/dependencies/tutorial002.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/dependencies/tutorial002_an.py` & `readyapi-0.110.3/docs_src/dependencies/tutorial002_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/dependencies/tutorial002_an_py310.py` & `readyapi-0.110.3/docs_src/dependencies/tutorial002_an_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/dependencies/tutorial002_an_py39.py` & `readyapi-0.110.3/docs_src/dependencies/tutorial002_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/dependencies/tutorial002_py310.py` & `readyapi-0.110.3/docs_src/dependencies/tutorial002_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/dependencies/tutorial003.py` & `readyapi-0.110.3/docs_src/dependencies/tutorial003.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/dependencies/tutorial003_an.py` & `readyapi-0.110.3/docs_src/dependencies/tutorial003_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/dependencies/tutorial003_an_py310.py` & `readyapi-0.110.3/docs_src/dependencies/tutorial003_an_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/dependencies/tutorial003_an_py39.py` & `readyapi-0.110.3/docs_src/dependencies/tutorial003_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/dependencies/tutorial003_py310.py` & `readyapi-0.110.3/docs_src/dependencies/tutorial003_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/dependencies/tutorial004.py` & `readyapi-0.110.3/docs_src/dependencies/tutorial004.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/dependencies/tutorial004_an.py` & `readyapi-0.110.3/docs_src/dependencies/tutorial004_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/dependencies/tutorial004_an_py310.py` & `readyapi-0.110.3/docs_src/dependencies/tutorial004_an_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/dependencies/tutorial004_an_py39.py` & `readyapi-0.110.3/docs_src/dependencies/tutorial004_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/dependencies/tutorial004_py310.py` & `readyapi-0.110.3/docs_src/dependencies/tutorial004_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/dependencies/tutorial005_an.py` & `readyapi-0.110.3/docs_src/dependencies/tutorial005_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/dependencies/tutorial005_an_py310.py` & `readyapi-0.110.3/docs_src/dependencies/tutorial005_an_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/dependencies/tutorial005_an_py39.py` & `readyapi-0.110.3/docs_src/dependencies/tutorial005_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/dependencies/tutorial006.py` & `readyapi-0.110.3/docs_src/dependencies/tutorial006.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/dependencies/tutorial006_an.py` & `readyapi-0.110.3/docs_src/dependencies/tutorial006_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/dependencies/tutorial006_an_py39.py` & `readyapi-0.110.3/docs_src/dependencies/tutorial006_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/dependencies/tutorial008_an.py` & `readyapi-0.110.3/docs_src/dependencies/tutorial008_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/dependencies/tutorial008_an_py39.py` & `readyapi-0.110.3/docs_src/dependencies/tutorial008_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/dependencies/tutorial008b.py` & `readyapi-0.110.3/docs_src/dependencies/tutorial008b.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/dependencies/tutorial008b_an.py` & `readyapi-0.110.3/docs_src/dependencies/tutorial008b_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/dependencies/tutorial008b_an_py39.py` & `readyapi-0.110.3/docs_src/dependencies/tutorial008b_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/dependencies/tutorial008c.py` & `readyapi-0.110.3/docs_src/dependencies/tutorial008c.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/dependencies/tutorial008c_an.py` & `readyapi-0.110.3/docs_src/dependencies/tutorial008c_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/dependencies/tutorial008c_an_py39.py` & `readyapi-0.110.3/docs_src/dependencies/tutorial008c_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/dependencies/tutorial008d.py` & `readyapi-0.110.3/docs_src/dependencies/tutorial008d.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/dependencies/tutorial008d_an.py` & `readyapi-0.110.3/docs_src/dependencies/tutorial008d_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/dependencies/tutorial008d_an_py39.py` & `readyapi-0.110.3/docs_src/dependencies/tutorial008d_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/dependencies/tutorial011_an.py` & `readyapi-0.110.3/docs_src/dependencies/tutorial011_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/dependencies/tutorial011_an_py39.py` & `readyapi-0.110.3/docs_src/dependencies/tutorial011_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/dependencies/tutorial012.py` & `readyapi-0.110.3/docs_src/dependencies/tutorial012.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/dependencies/tutorial012_an.py` & `readyapi-0.110.3/docs_src/dependencies/tutorial012_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/dependencies/tutorial012_an_py39.py` & `readyapi-0.110.3/docs_src/dependencies/tutorial012_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/dependency_testing/tutorial001.py` & `readyapi-0.110.3/docs_src/dependency_testing/tutorial001.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/dependency_testing/tutorial001_an.py` & `readyapi-0.110.3/docs_src/dependency_testing/tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/dependency_testing/tutorial001_an_py310.py` & `readyapi-0.110.3/docs_src/dependency_testing/tutorial001_an_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/dependency_testing/tutorial001_an_py39.py` & `readyapi-0.110.3/docs_src/dependency_testing/tutorial001_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/dependency_testing/tutorial001_py310.py` & `readyapi-0.110.3/docs_src/dependency_testing/tutorial001_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/events/tutorial003.py` & `readyapi-0.110.3/docs_src/events/tutorial003.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/extending_openapi/tutorial001.py` & `readyapi-0.110.3/docs_src/extending_openapi/tutorial001.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/extra_data_types/tutorial001.py` & `readyapi-0.110.3/docs_src/extra_data_types/tutorial001.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/extra_data_types/tutorial001_an.py` & `readyapi-0.110.3/docs_src/extra_data_types/tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/extra_data_types/tutorial001_an_py310.py` & `readyapi-0.110.3/docs_src/extra_data_types/tutorial001_an_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/extra_data_types/tutorial001_an_py39.py` & `readyapi-0.110.3/docs_src/extra_data_types/tutorial001_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/extra_data_types/tutorial001_py310.py` & `readyapi-0.110.3/docs_src/extra_data_types/tutorial001_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/extra_models/tutorial001.py` & `readyapi-0.110.3/docs_src/extra_models/tutorial001.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/extra_models/tutorial001_py310.py` & `readyapi-0.110.3/docs_src/extra_models/tutorial001_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/extra_models/tutorial002.py` & `readyapi-0.110.3/docs_src/extra_models/tutorial002.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/extra_models/tutorial002_py310.py` & `readyapi-0.110.3/docs_src/extra_models/tutorial002_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/extra_models/tutorial003.py` & `readyapi-0.110.3/docs_src/extra_models/tutorial003.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/extra_models/tutorial003_py310.py` & `readyapi-0.110.3/docs_src/extra_models/tutorial003_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/generate_clients/tutorial001.py` & `readyapi-0.110.3/docs_src/generate_clients/tutorial001.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/generate_clients/tutorial002.py` & `readyapi-0.110.3/docs_src/generate_clients/tutorial002.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/generate_clients/tutorial002_py39.py` & `readyapi-0.110.3/docs_src/generate_clients/tutorial002_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/generate_clients/tutorial003.py` & `readyapi-0.110.3/docs_src/generate_clients/tutorial003.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/generate_clients/tutorial003_py39.py` & `readyapi-0.110.3/docs_src/generate_clients/tutorial003_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/generate_clients/tutorial004.js` & `readyapi-0.110.3/docs_src/generate_clients/tutorial004.js`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/handling_errors/tutorial003.py` & `readyapi-0.110.3/docs_src/handling_errors/tutorial003.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/handling_errors/tutorial004.py` & `readyapi-0.110.3/docs_src/handling_errors/tutorial004.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/handling_errors/tutorial005.py` & `readyapi-0.110.3/docs_src/handling_errors/tutorial005.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/handling_errors/tutorial006.py` & `readyapi-0.110.3/docs_src/handling_errors/tutorial006.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/metadata/tutorial001.py` & `readyapi-0.110.3/docs_src/metadata/tutorial001.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/metadata/tutorial001_1.py` & `readyapi-0.110.3/docs_src/metadata/tutorial001_1.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/metadata/tutorial004.py` & `readyapi-0.110.3/docs_src/metadata/tutorial004.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/nosql_databases/tutorial001.py` & `readyapi-0.110.3/docs_src/nosql_databases/tutorial001.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/openapi_callbacks/tutorial001.py` & `readyapi-0.110.3/docs_src/openapi_callbacks/tutorial001.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/openapi_webhooks/tutorial001.py` & `readyapi-0.110.3/docs_src/openapi_webhooks/tutorial001.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/path_operation_advanced_configuration/tutorial002.py` & `readyapi-0.110.3/docs_src/path_operation_advanced_configuration/tutorial002.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/path_operation_advanced_configuration/tutorial004.py` & `readyapi-0.110.3/docs_src/path_operation_advanced_configuration/tutorial004.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/path_operation_advanced_configuration/tutorial006.py` & `readyapi-0.110.3/docs_src/path_operation_advanced_configuration/tutorial006.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/path_operation_advanced_configuration/tutorial007.py` & `readyapi-0.110.3/docs_src/path_operation_advanced_configuration/tutorial007.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/path_operation_advanced_configuration/tutorial007_pv1.py` & `readyapi-0.110.3/docs_src/path_operation_advanced_configuration/tutorial007_pv1.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/path_operation_configuration/tutorial002.py` & `readyapi-0.110.3/docs_src/path_operation_configuration/tutorial002.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/path_operation_configuration/tutorial002_py310.py` & `readyapi-0.110.3/docs_src/path_operation_configuration/tutorial002_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/path_operation_configuration/tutorial002_py39.py` & `readyapi-0.110.3/docs_src/path_operation_configuration/tutorial002_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/path_operation_configuration/tutorial003.py` & `readyapi-0.110.3/docs_src/path_operation_configuration/tutorial003.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/path_operation_configuration/tutorial003_py39.py` & `readyapi-0.110.3/docs_src/path_operation_configuration/tutorial003_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/path_operation_configuration/tutorial004.py` & `readyapi-0.110.3/docs_src/path_operation_configuration/tutorial004.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/path_operation_configuration/tutorial004_py310.py` & `readyapi-0.110.3/docs_src/path_operation_configuration/tutorial004_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/path_operation_configuration/tutorial004_py39.py` & `readyapi-0.110.3/docs_src/path_operation_configuration/tutorial004_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/path_operation_configuration/tutorial005.py` & `readyapi-0.110.3/docs_src/path_operation_configuration/tutorial005.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/path_operation_configuration/tutorial005_py310.py` & `readyapi-0.110.3/docs_src/path_operation_configuration/tutorial005_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/path_operation_configuration/tutorial005_py39.py` & `readyapi-0.110.3/docs_src/path_operation_configuration/tutorial005_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/path_params/tutorial005.py` & `readyapi-0.110.3/docs_src/path_params/tutorial005.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/query_params_str_validations/tutorial008_an.py` & `readyapi-0.110.3/docs_src/query_params_str_validations/tutorial008_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/query_params_str_validations/tutorial008_an_py39.py` & `readyapi-0.110.3/docs_src/query_params_str_validations/tutorial008_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/query_params_str_validations/tutorial010.py` & `readyapi-0.110.3/docs_src/query_params_str_validations/tutorial010.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/query_params_str_validations/tutorial010_an.py` & `readyapi-0.110.3/docs_src/query_params_str_validations/tutorial010_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/query_params_str_validations/tutorial010_an_py310.py` & `readyapi-0.110.3/docs_src/query_params_str_validations/tutorial010_an_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/query_params_str_validations/tutorial010_an_py39.py` & `readyapi-0.110.3/docs_src/query_params_str_validations/tutorial010_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/query_params_str_validations/tutorial010_py310.py` & `readyapi-0.110.3/docs_src/query_params_str_validations/tutorial010_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/request_files/tutorial001_02_an.py` & `readyapi-0.110.3/docs_src/request_files/tutorial001_02_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/request_files/tutorial001_02_an_py39.py` & `readyapi-0.110.3/docs_src/request_files/tutorial001_02_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/request_files/tutorial002.py` & `readyapi-0.110.3/docs_src/request_files/tutorial002.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/request_files/tutorial002_an.py` & `readyapi-0.110.3/docs_src/request_files/tutorial002_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/request_files/tutorial002_an_py39.py` & `readyapi-0.110.3/docs_src/request_files/tutorial002_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/request_files/tutorial002_py39.py` & `readyapi-0.110.3/docs_src/request_files/tutorial002_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/request_files/tutorial003.py` & `readyapi-0.110.3/docs_src/request_files/tutorial003.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/request_files/tutorial003_an.py` & `readyapi-0.110.3/docs_src/request_files/tutorial003_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/request_files/tutorial003_an_py39.py` & `readyapi-0.110.3/docs_src/request_files/tutorial003_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/request_files/tutorial003_py39.py` & `readyapi-0.110.3/docs_src/request_files/tutorial003_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/response_model/tutorial001.py` & `readyapi-0.110.3/docs_src/response_model/tutorial001.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/response_model/tutorial001_01.py` & `readyapi-0.110.3/docs_src/response_model/tutorial001_01.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/response_model/tutorial001_py310.py` & `readyapi-0.110.3/docs_src/response_model/tutorial001_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/response_model/tutorial001_py39.py` & `readyapi-0.110.3/docs_src/response_model/tutorial001_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/response_model/tutorial004.py` & `readyapi-0.110.3/docs_src/response_model/tutorial004.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/response_model/tutorial004_py310.py` & `readyapi-0.110.3/docs_src/response_model/tutorial004_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/response_model/tutorial004_py39.py` & `readyapi-0.110.3/docs_src/response_model/tutorial004_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/response_model/tutorial005.py` & `readyapi-0.110.3/docs_src/response_model/tutorial005.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/response_model/tutorial005_py310.py` & `readyapi-0.110.3/docs_src/response_model/tutorial005_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/response_model/tutorial006.py` & `readyapi-0.110.3/docs_src/response_model/tutorial006.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/response_model/tutorial006_py310.py` & `readyapi-0.110.3/docs_src/response_model/tutorial006_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/schema_extra_example/tutorial001.py` & `readyapi-0.110.3/docs_src/schema_extra_example/tutorial001.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/schema_extra_example/tutorial001_pv1.py` & `readyapi-0.110.3/docs_src/schema_extra_example/tutorial001_pv1.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/schema_extra_example/tutorial001_py310.py` & `readyapi-0.110.3/docs_src/schema_extra_example/tutorial001_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/schema_extra_example/tutorial001_py310_pv1.py` & `readyapi-0.110.3/docs_src/schema_extra_example/tutorial001_py310_pv1.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/schema_extra_example/tutorial002.py` & `readyapi-0.110.3/docs_src/schema_extra_example/tutorial002.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/schema_extra_example/tutorial003.py` & `readyapi-0.110.3/docs_src/schema_extra_example/tutorial003.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/schema_extra_example/tutorial003_an.py` & `readyapi-0.110.3/docs_src/schema_extra_example/tutorial003_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/schema_extra_example/tutorial003_an_py310.py` & `readyapi-0.110.3/docs_src/schema_extra_example/tutorial003_an_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/schema_extra_example/tutorial003_an_py39.py` & `readyapi-0.110.3/docs_src/schema_extra_example/tutorial003_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/schema_extra_example/tutorial003_py310.py` & `readyapi-0.110.3/docs_src/schema_extra_example/tutorial003_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/schema_extra_example/tutorial004.py` & `readyapi-0.110.3/docs_src/schema_extra_example/tutorial004.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/schema_extra_example/tutorial004_an.py` & `readyapi-0.110.3/docs_src/schema_extra_example/tutorial004_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/schema_extra_example/tutorial004_an_py310.py` & `readyapi-0.110.3/docs_src/schema_extra_example/tutorial004_an_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/schema_extra_example/tutorial004_an_py39.py` & `readyapi-0.110.3/docs_src/schema_extra_example/tutorial004_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/schema_extra_example/tutorial004_py310.py` & `readyapi-0.110.3/docs_src/schema_extra_example/tutorial004_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/schema_extra_example/tutorial005.py` & `readyapi-0.110.3/docs_src/schema_extra_example/tutorial005.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/schema_extra_example/tutorial005_an.py` & `readyapi-0.110.3/docs_src/schema_extra_example/tutorial005_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/schema_extra_example/tutorial005_an_py310.py` & `readyapi-0.110.3/docs_src/schema_extra_example/tutorial005_an_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/schema_extra_example/tutorial005_an_py39.py` & `readyapi-0.110.3/docs_src/schema_extra_example/tutorial005_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/schema_extra_example/tutorial005_py310.py` & `readyapi-0.110.3/docs_src/schema_extra_example/tutorial005_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/security/tutorial002.py` & `readyapi-0.110.3/docs_src/security/tutorial002.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/security/tutorial002_an.py` & `readyapi-0.110.3/docs_src/security/tutorial002_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/security/tutorial002_an_py310.py` & `readyapi-0.110.3/docs_src/security/tutorial002_an_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/security/tutorial002_an_py39.py` & `readyapi-0.110.3/docs_src/security/tutorial002_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/security/tutorial002_py310.py` & `readyapi-0.110.3/docs_src/security/tutorial002_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/security/tutorial003.py` & `readyapi-0.110.3/docs_src/security/tutorial003.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/security/tutorial003_an.py` & `readyapi-0.110.3/docs_src/security/tutorial003_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/security/tutorial003_an_py310.py` & `readyapi-0.110.3/docs_src/security/tutorial003_an_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/security/tutorial003_an_py39.py` & `readyapi-0.110.3/docs_src/security/tutorial003_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/security/tutorial003_py310.py` & `readyapi-0.110.3/docs_src/security/tutorial003_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/security/tutorial004.py` & `readyapi-0.110.3/docs_src/security/tutorial004.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/security/tutorial004_an.py` & `readyapi-0.110.3/docs_src/security/tutorial004_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/security/tutorial004_an_py310.py` & `readyapi-0.110.3/docs_src/security/tutorial004_an_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/security/tutorial004_an_py39.py` & `readyapi-0.110.3/docs_src/security/tutorial004_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/security/tutorial004_py310.py` & `readyapi-0.110.3/docs_src/security/tutorial004_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/security/tutorial005.py` & `readyapi-0.110.3/docs_src/security/tutorial005.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/security/tutorial005_an.py` & `readyapi-0.110.3/docs_src/security/tutorial005_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/security/tutorial005_an_py310.py` & `readyapi-0.110.3/docs_src/security/tutorial005_an_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/security/tutorial005_an_py39.py` & `readyapi-0.110.3/docs_src/security/tutorial005_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/security/tutorial005_py310.py` & `readyapi-0.110.3/docs_src/security/tutorial005_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/security/tutorial005_py39.py` & `readyapi-0.110.3/docs_src/security/tutorial005_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/security/tutorial007.py` & `readyapi-0.110.3/docs_src/security/tutorial007.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/security/tutorial007_an.py` & `readyapi-0.110.3/docs_src/security/tutorial007_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/security/tutorial007_an_py39.py` & `readyapi-0.110.3/docs_src/security/tutorial007_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/separate_openapi_schemas/tutorial002.py` & `readyapi-0.110.3/docs_src/separate_openapi_schemas/tutorial002.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/separate_openapi_schemas/tutorial002_py39.py` & `readyapi-0.110.3/docs_src/separate_openapi_schemas/tutorial002_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/settings/app02/test_main.py` & `readyapi-0.110.3/docs_src/settings/app02/test_main.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/settings/app02_an/test_main.py` & `readyapi-0.110.3/docs_src/settings/app02_an/test_main.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/settings/app02_an_py39/test_main.py` & `readyapi-0.110.3/docs_src/settings/app02_an_py39/test_main.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/sql_databases/sql_app/alt_main.py` & `readyapi-0.110.3/docs_src/sql_databases/sql_app/alt_main.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/sql_databases/sql_app/crud.py` & `readyapi-0.110.3/docs_src/sql_databases/sql_app/crud.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/sql_databases/sql_app/main.py` & `readyapi-0.110.3/docs_src/sql_databases/sql_app/main.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/sql_databases/sql_app/models.py` & `readyapi-0.110.3/docs_src/sql_databases/sql_app/models.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/sql_databases/sql_app/tests/test_sql_app.py` & `readyapi-0.110.3/docs_src/sql_databases/sql_app/tests/test_sql_app.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/sql_databases/sql_app_py310/alt_main.py` & `readyapi-0.110.3/docs_src/sql_databases/sql_app_py310/alt_main.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/sql_databases/sql_app_py310/crud.py` & `readyapi-0.110.3/docs_src/sql_databases/sql_app_py310/crud.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/sql_databases/sql_app_py310/main.py` & `readyapi-0.110.3/docs_src/sql_databases/sql_app_py310/main.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/sql_databases/sql_app_py310/models.py` & `readyapi-0.110.3/docs_src/sql_databases/sql_app_py310/models.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/sql_databases/sql_app_py310/tests/test_sql_app.py` & `readyapi-0.110.3/docs_src/sql_databases/sql_app_py310/tests/test_sql_app.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/sql_databases/sql_app_py39/alt_main.py` & `readyapi-0.110.3/docs_src/sql_databases/sql_app_py39/alt_main.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/sql_databases/sql_app_py39/crud.py` & `readyapi-0.110.3/docs_src/sql_databases/sql_app_py39/crud.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/sql_databases/sql_app_py39/main.py` & `readyapi-0.110.3/docs_src/sql_databases/sql_app_py39/main.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/sql_databases/sql_app_py39/models.py` & `readyapi-0.110.3/docs_src/sql_databases/sql_app_py39/models.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/sql_databases/sql_app_py39/tests/test_sql_app.py` & `readyapi-0.110.3/docs_src/sql_databases/sql_app_py39/tests/test_sql_app.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/sql_databases_peewee/sql_app/crud.py` & `readyapi-0.110.3/docs_src/sql_databases_peewee/sql_app/crud.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/sql_databases_peewee/sql_app/database.py` & `readyapi-0.110.3/docs_src/sql_databases_peewee/sql_app/database.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/sql_databases_peewee/sql_app/main.py` & `readyapi-0.110.3/docs_src/sql_databases_peewee/sql_app/main.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/sql_databases_peewee/sql_app/schemas.py` & `readyapi-0.110.3/docs_src/sql_databases_peewee/sql_app/schemas.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/templates/tutorial001.py` & `readyapi-0.110.3/docs_src/templates/tutorial001.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/websockets/tutorial001.py` & `readyapi-0.110.3/docs_src/websockets/tutorial001.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/websockets/tutorial002.py` & `readyapi-0.110.3/docs_src/websockets/tutorial002.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/websockets/tutorial002_an.py` & `readyapi-0.110.3/docs_src/websockets/tutorial002_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/websockets/tutorial002_an_py310.py` & `readyapi-0.110.3/docs_src/websockets/tutorial002_an_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/websockets/tutorial002_an_py39.py` & `readyapi-0.110.3/docs_src/websockets/tutorial002_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/websockets/tutorial002_py310.py` & `readyapi-0.110.3/docs_src/websockets/tutorial002_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/websockets/tutorial003.py` & `readyapi-0.110.3/docs_src/websockets/tutorial003.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/docs_src/websockets/tutorial003_py39.py` & `readyapi-0.110.3/docs_src/websockets/tutorial003_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/pdm_build.py` & `readyapi-0.110.3/pdm_build.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/pyproject.toml` & `readyapi-0.110.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     "jinja2 >=2.11.2",
     "python-multipart >=0.0.7",
     "ujson >=4.0.1,!=4.0.2,!=4.1.0,!=4.2.0,!=4.3.0,!=5.0.0,!=5.1.0",
     "orjson >=3.2.1",
     "email_validator >=2.0.0",
     "uvicorn[standard] >=0.12.0",
 ]
-version = "0.110.2.dev1"
+version = "0.110.3"
 
 [project.urls]
 Homepage = "https://github.com/khulnasoft/readyapi"
 Documentation = "https://readyapi.khulnasoft.com/"
 Repository = "https://github.com/khulnasoft/readyapi"
 
 [project.optional-dependencies]
```

### Comparing `readyapi-0.110.2.dev1/readyapi/__init__.py` & `readyapi-0.110.3/readyapi/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """ReadyAPI framework, high performance, easy to learn, fast to code, ready for production"""
 
-__version__ = "0.110.2.dev1"
+__version__ = "0.110.3"
 
 from starlette import status as status
 
 from .applications import ReadyAPI as ReadyAPI
 from .background import BackgroundTasks as BackgroundTasks
 from .datastructures import UploadFile as UploadFile
 from .exceptions import HTTPException as HTTPException
```

### Comparing `readyapi-0.110.2.dev1/readyapi/_compat.py` & `readyapi-0.110.3/readyapi/_compat.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/readyapi/applications.py` & `readyapi-0.110.3/readyapi/applications.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/readyapi/background.py` & `readyapi-0.110.3/readyapi/background.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/readyapi/concurrency.py` & `readyapi-0.110.3/readyapi/concurrency.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/readyapi/datastructures.py` & `readyapi-0.110.3/readyapi/datastructures.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/readyapi/dependencies/models.py` & `readyapi-0.110.3/readyapi/dependencies/models.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/readyapi/dependencies/utils.py` & `readyapi-0.110.3/readyapi/dependencies/utils.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/readyapi/encoders.py` & `readyapi-0.110.3/readyapi/encoders.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/readyapi/exception_handlers.py` & `readyapi-0.110.3/readyapi/exception_handlers.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/readyapi/exceptions.py` & `readyapi-0.110.3/readyapi/exceptions.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/readyapi/openapi/docs.py` & `readyapi-0.110.3/readyapi/openapi/docs.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/readyapi/openapi/models.py` & `readyapi-0.110.3/readyapi/openapi/models.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/readyapi/openapi/utils.py` & `readyapi-0.110.3/readyapi/openapi/utils.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/readyapi/param_functions.py` & `readyapi-0.110.3/readyapi/param_functions.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/readyapi/params.py` & `readyapi-0.110.3/readyapi/params.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/readyapi/responses.py` & `readyapi-0.110.3/readyapi/responses.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/readyapi/routing.py` & `readyapi-0.110.3/readyapi/routing.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/readyapi/security/__init__.py` & `readyapi-0.110.3/readyapi/security/__init__.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/readyapi/security/api_key.py` & `readyapi-0.110.3/readyapi/security/api_key.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/readyapi/security/http.py` & `readyapi-0.110.3/readyapi/security/http.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/readyapi/security/oauth2.py` & `readyapi-0.110.3/readyapi/security/oauth2.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/readyapi/security/open_id_connect_url.py` & `readyapi-0.110.3/readyapi/security/open_id_connect_url.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/readyapi/utils.py` & `readyapi-0.110.3/readyapi/utils.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/scripts/docs.py` & `readyapi-0.110.3/scripts/docs.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/scripts/mkdocs_hooks.py` & `readyapi-0.110.3/scripts/mkdocs_hooks.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/scripts/playwright/separate_openapi_schemas/image01.py` & `readyapi-0.110.3/scripts/playwright/separate_openapi_schemas/image01.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/scripts/playwright/separate_openapi_schemas/image02.py` & `readyapi-0.110.3/scripts/playwright/separate_openapi_schemas/image02.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/scripts/playwright/separate_openapi_schemas/image03.py` & `readyapi-0.110.3/scripts/playwright/separate_openapi_schemas/image03.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/scripts/playwright/separate_openapi_schemas/image04.py` & `readyapi-0.110.3/scripts/playwright/separate_openapi_schemas/image04.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/scripts/playwright/separate_openapi_schemas/image05.py` & `readyapi-0.110.3/scripts/playwright/separate_openapi_schemas/image05.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/main.py` & `readyapi-0.110.3/tests/main.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_additional_properties.py` & `readyapi-0.110.3/tests/test_additional_properties.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_additional_properties_bool.py` & `readyapi-0.110.3/tests/test_additional_properties_bool.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_additional_response_extra.py` & `readyapi-0.110.3/tests/test_additional_response_extra.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_additional_responses_bad.py` & `readyapi-0.110.3/tests/test_additional_responses_bad.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_additional_responses_custom_model_in_callback.py` & `readyapi-0.110.3/tests/test_additional_responses_custom_model_in_callback.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_additional_responses_custom_validationerror.py` & `readyapi-0.110.3/tests/test_additional_responses_custom_validationerror.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_additional_responses_default_validationerror.py` & `readyapi-0.110.3/tests/test_additional_responses_default_validationerror.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_additional_responses_response_class.py` & `readyapi-0.110.3/tests/test_additional_responses_response_class.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_additional_responses_router.py` & `readyapi-0.110.3/tests/test_additional_responses_router.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_ambiguous_params.py` & `readyapi-0.110.3/tests/test_ambiguous_params.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_annotated.py` & `readyapi-0.110.3/tests/test_annotated.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_application.py` & `readyapi-0.110.3/tests/test_application.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_compat.py` & `readyapi-0.110.3/tests/test_compat.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_computed_fields.py` & `readyapi-0.110.3/tests/test_computed_fields.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_custom_middleware_exception.py` & `readyapi-0.110.3/tests/test_custom_middleware_exception.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_custom_route_class.py` & `readyapi-0.110.3/tests/test_custom_route_class.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_custom_schema_fields.py` & `readyapi-0.110.3/tests/test_custom_schema_fields.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_custom_swagger_ui_redirect.py` & `readyapi-0.110.3/tests/test_custom_swagger_ui_redirect.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_datastructures.py` & `readyapi-0.110.3/tests/test_datastructures.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_datetime_custom_encoder.py` & `readyapi-0.110.3/tests/test_datetime_custom_encoder.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_default_response_class.py` & `readyapi-0.110.3/tests/test_default_response_class.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_default_response_class_router.py` & `readyapi-0.110.3/tests/test_default_response_class_router.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_dependency_cache.py` & `readyapi-0.110.3/tests/test_dependency_cache.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_dependency_class.py` & `readyapi-0.110.3/tests/test_dependency_class.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_dependency_contextmanager.py` & `readyapi-0.110.3/tests/test_dependency_contextmanager.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_dependency_contextvars.py` & `readyapi-0.110.3/tests/test_dependency_contextvars.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_dependency_duplicates.py` & `readyapi-0.110.3/tests/test_dependency_duplicates.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_dependency_normal_exceptions.py` & `readyapi-0.110.3/tests/test_dependency_normal_exceptions.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_dependency_overrides.py` & `readyapi-0.110.3/tests/test_dependency_overrides.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_dependency_security_overrides.py` & `readyapi-0.110.3/tests/test_dependency_security_overrides.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_deprecated_openapi_prefix.py` & `readyapi-0.110.3/tests/test_deprecated_openapi_prefix.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_duplicate_models_openapi.py` & `readyapi-0.110.3/tests/test_duplicate_models_openapi.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_empty_router.py` & `readyapi-0.110.3/tests/test_empty_router.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_enforce_once_required_parameter.py` & `readyapi-0.110.3/tests/test_enforce_once_required_parameter.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_exception_handlers.py` & `readyapi-0.110.3/tests/test_exception_handlers.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_extra_routes.py` & `readyapi-0.110.3/tests/test_extra_routes.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_filter_pydantic_sub_model/app_pv1.py` & `readyapi-0.110.3/tests/test_filter_pydantic_sub_model/app_pv1.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_filter_pydantic_sub_model/test_filter_pydantic_sub_model_pv1.py` & `readyapi-0.110.3/tests/test_filter_pydantic_sub_model/test_filter_pydantic_sub_model_pv1.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_filter_pydantic_sub_model_pv2.py` & `readyapi-0.110.3/tests/test_filter_pydantic_sub_model_pv2.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_forms_from_non_typing_sequences.py` & `readyapi-0.110.3/tests/test_forms_from_non_typing_sequences.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_generate_unique_id_function.py` & `readyapi-0.110.3/tests/test_generate_unique_id_function.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_generic_parameterless_depends.py` & `readyapi-0.110.3/tests/test_generic_parameterless_depends.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_get_request_body.py` & `readyapi-0.110.3/tests/test_get_request_body.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_http_connection_injection.py` & `readyapi-0.110.3/tests/test_http_connection_injection.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_include_router_defaults_overrides.py` & `readyapi-0.110.3/tests/test_include_router_defaults_overrides.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_infer_param_optionality.py` & `readyapi-0.110.3/tests/test_infer_param_optionality.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_inherited_custom_class.py` & `readyapi-0.110.3/tests/test_inherited_custom_class.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_invalid_path_param.py` & `readyapi-0.110.3/tests/test_invalid_path_param.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_invalid_sequence_param.py` & `readyapi-0.110.3/tests/test_invalid_sequence_param.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_jsonable_encoder.py` & `readyapi-0.110.3/tests/test_jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_local_docs.py` & `readyapi-0.110.3/tests/test_local_docs.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_modules_same_name_body/test_main.py` & `readyapi-0.110.3/tests/test_modules_same_name_body/test_main.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_multi_body_errors.py` & `readyapi-0.110.3/tests/test_multi_body_errors.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_multi_query_errors.py` & `readyapi-0.110.3/tests/test_multi_query_errors.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_multipart_installation.py` & `readyapi-0.110.3/tests/test_multipart_installation.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_no_swagger_ui_redirect.py` & `readyapi-0.110.3/tests/test_no_swagger_ui_redirect.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_openapi_examples.py` & `readyapi-0.110.3/tests/test_openapi_examples.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_openapi_query_parameter_extension.py` & `readyapi-0.110.3/tests/test_openapi_query_parameter_extension.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_openapi_route_extensions.py` & `readyapi-0.110.3/tests/test_openapi_route_extensions.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_openapi_separate_input_output_schemas.py` & `readyapi-0.110.3/tests/test_openapi_separate_input_output_schemas.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_openapi_servers.py` & `readyapi-0.110.3/tests/test_openapi_servers.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_operations_signatures.py` & `readyapi-0.110.3/tests/test_operations_signatures.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_orjson_response_class.py` & `readyapi-0.110.3/tests/test_orjson_response_class.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_param_class.py` & `readyapi-0.110.3/tests/test_param_class.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_param_in_path_and_dependency.py` & `readyapi-0.110.3/tests/test_param_in_path_and_dependency.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_param_include_in_schema.py` & `readyapi-0.110.3/tests/test_param_include_in_schema.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_params_repr.py` & `readyapi-0.110.3/tests/test_params_repr.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_path.py` & `readyapi-0.110.3/tests/test_path.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_put_no_body.py` & `readyapi-0.110.3/tests/test_put_no_body.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_query.py` & `readyapi-0.110.3/tests/test_query.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_read_with_orm_mode.py` & `readyapi-0.110.3/tests/test_read_with_orm_mode.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_regex_deprecated_body.py` & `readyapi-0.110.3/tests/test_regex_deprecated_body.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_regex_deprecated_params.py` & `readyapi-0.110.3/tests/test_regex_deprecated_params.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_repeated_cookie_headers.py` & `readyapi-0.110.3/tests/test_repeated_cookie_headers.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_repeated_dependency_schema.py` & `readyapi-0.110.3/tests/test_repeated_dependency_schema.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_repeated_parameter_alias.py` & `readyapi-0.110.3/tests/test_repeated_parameter_alias.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_reponse_set_reponse_code_empty.py` & `readyapi-0.110.3/tests/test_reponse_set_reponse_code_empty.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_request_body_parameters_media_type.py` & `readyapi-0.110.3/tests/test_request_body_parameters_media_type.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_required_noneable.py` & `readyapi-0.110.3/tests/test_required_noneable.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_response_by_alias.py` & `readyapi-0.110.3/tests/test_response_by_alias.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_response_change_status_code.py` & `readyapi-0.110.3/tests/test_response_change_status_code.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_response_class_no_mediatype.py` & `readyapi-0.110.3/tests/test_response_class_no_mediatype.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_response_code_no_body.py` & `readyapi-0.110.3/tests/test_response_code_no_body.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_response_model_as_return_annotation.py` & `readyapi-0.110.3/tests/test_response_model_as_return_annotation.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_response_model_data_filter.py` & `readyapi-0.110.3/tests/test_response_model_data_filter.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_response_model_data_filter_no_inheritance.py` & `readyapi-0.110.3/tests/test_response_model_data_filter_no_inheritance.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_response_model_include_exclude.py` & `readyapi-0.110.3/tests/test_response_model_include_exclude.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_response_model_invalid.py` & `readyapi-0.110.3/tests/test_response_model_invalid.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_response_model_sub_types.py` & `readyapi-0.110.3/tests/test_response_model_sub_types.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_route_scope.py` & `readyapi-0.110.3/tests/test_route_scope.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_router_events.py` & `readyapi-0.110.3/tests/test_router_events.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_router_redirect_slashes.py` & `readyapi-0.110.3/tests/test_router_redirect_slashes.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_schema_extra_examples.py` & `readyapi-0.110.3/tests/test_schema_extra_examples.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_security_api_key_cookie.py` & `readyapi-0.110.3/tests/test_security_api_key_cookie.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_security_api_key_cookie_description.py` & `readyapi-0.110.3/tests/test_security_api_key_cookie_description.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_security_api_key_cookie_optional.py` & `readyapi-0.110.3/tests/test_security_api_key_cookie_optional.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_security_api_key_header.py` & `readyapi-0.110.3/tests/test_security_api_key_header.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_security_api_key_header_description.py` & `readyapi-0.110.3/tests/test_security_api_key_header_description.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_security_api_key_header_optional.py` & `readyapi-0.110.3/tests/test_security_api_key_header_optional.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_security_api_key_query.py` & `readyapi-0.110.3/tests/test_security_api_key_query.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_security_api_key_query_description.py` & `readyapi-0.110.3/tests/test_security_api_key_query_description.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_security_api_key_query_optional.py` & `readyapi-0.110.3/tests/test_security_api_key_query_optional.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_security_http_base.py` & `readyapi-0.110.3/tests/test_security_http_base.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_security_http_base_description.py` & `readyapi-0.110.3/tests/test_security_http_base_description.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_security_http_base_optional.py` & `readyapi-0.110.3/tests/test_security_http_base_optional.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_security_http_basic_optional.py` & `readyapi-0.110.3/tests/test_security_http_basic_optional.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_security_http_basic_realm.py` & `readyapi-0.110.3/tests/test_security_http_basic_realm.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_security_http_basic_realm_description.py` & `readyapi-0.110.3/tests/test_security_http_basic_realm_description.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_security_http_bearer.py` & `readyapi-0.110.3/tests/test_security_http_bearer.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_security_http_bearer_description.py` & `readyapi-0.110.3/tests/test_security_http_bearer_description.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_security_http_bearer_optional.py` & `readyapi-0.110.3/tests/test_security_http_bearer_optional.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_security_http_digest.py` & `readyapi-0.110.3/tests/test_security_http_digest.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_security_http_digest_description.py` & `readyapi-0.110.3/tests/test_security_http_digest_description.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_security_http_digest_optional.py` & `readyapi-0.110.3/tests/test_security_http_digest_optional.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_security_oauth2.py` & `readyapi-0.110.3/tests/test_security_oauth2.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_security_oauth2_authorization_code_bearer.py` & `readyapi-0.110.3/tests/test_security_oauth2_authorization_code_bearer.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_security_oauth2_authorization_code_bearer_description.py` & `readyapi-0.110.3/tests/test_security_oauth2_authorization_code_bearer_description.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_security_oauth2_optional.py` & `readyapi-0.110.3/tests/test_security_oauth2_optional.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_security_oauth2_optional_description.py` & `readyapi-0.110.3/tests/test_security_oauth2_optional_description.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_security_oauth2_password_bearer_optional.py` & `readyapi-0.110.3/tests/test_security_oauth2_password_bearer_optional.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_security_oauth2_password_bearer_optional_description.py` & `readyapi-0.110.3/tests/test_security_oauth2_password_bearer_optional_description.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_security_openid_connect.py` & `readyapi-0.110.3/tests/test_security_openid_connect.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_security_openid_connect_description.py` & `readyapi-0.110.3/tests/test_security_openid_connect_description.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_security_openid_connect_optional.py` & `readyapi-0.110.3/tests/test_security_openid_connect_optional.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_serialize_response.py` & `readyapi-0.110.3/tests/test_serialize_response.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_serialize_response_dataclass.py` & `readyapi-0.110.3/tests/test_serialize_response_dataclass.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_serialize_response_model.py` & `readyapi-0.110.3/tests/test_serialize_response_model.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_skip_defaults.py` & `readyapi-0.110.3/tests/test_skip_defaults.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_starlette_exception.py` & `readyapi-0.110.3/tests/test_starlette_exception.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_starlette_urlconvertors.py` & `readyapi-0.110.3/tests/test_starlette_urlconvertors.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_sub_callbacks.py` & `readyapi-0.110.3/tests/test_sub_callbacks.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_swagger_ui_init_oauth.py` & `readyapi-0.110.3/tests/test_swagger_ui_init_oauth.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tuples.py` & `readyapi-0.110.3/tests/test_tuples.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_additional_responses/test_tutorial001.py` & `readyapi-0.110.3/tests/test_tutorial/test_additional_responses/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_additional_responses/test_tutorial002.py` & `readyapi-0.110.3/tests/test_tutorial/test_additional_responses/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_additional_responses/test_tutorial003.py` & `readyapi-0.110.3/tests/test_tutorial/test_additional_responses/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_additional_responses/test_tutorial004.py` & `readyapi-0.110.3/tests/test_tutorial/test_additional_responses/test_tutorial004.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_additional_status_codes/test_tutorial001.py` & `readyapi-0.110.3/tests/test_tutorial/test_additional_status_codes/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_additional_status_codes/test_tutorial001_an.py` & `readyapi-0.110.3/tests/test_tutorial/test_additional_status_codes/test_tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_additional_status_codes/test_tutorial001_an_py310.py` & `readyapi-0.110.3/tests/test_tutorial/test_additional_status_codes/test_tutorial001_an_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_additional_status_codes/test_tutorial001_an_py39.py` & `readyapi-0.110.3/tests/test_tutorial/test_additional_status_codes/test_tutorial001_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_additional_status_codes/test_tutorial001_py310.py` & `readyapi-0.110.3/tests/test_tutorial/test_additional_status_codes/test_tutorial001_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_advanced_middleware/test_tutorial002.py` & `readyapi-0.110.3/tests/test_tutorial/test_advanced_middleware/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_advanced_middleware/test_tutorial003.py` & `readyapi-0.110.3/tests/test_tutorial/test_advanced_middleware/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_async_sql_databases/test_tutorial001.py` & `readyapi-0.110.3/tests/test_tutorial/test_async_sql_databases/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_background_tasks/test_tutorial001.py` & `readyapi-0.110.3/tests/test_tutorial/test_background_tasks/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_background_tasks/test_tutorial002.py` & `readyapi-0.110.3/tests/test_tutorial/test_background_tasks/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_background_tasks/test_tutorial002_an.py` & `readyapi-0.110.3/tests/test_tutorial/test_background_tasks/test_tutorial002_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_background_tasks/test_tutorial002_an_py310.py` & `readyapi-0.110.3/tests/test_tutorial/test_background_tasks/test_tutorial002_an_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_background_tasks/test_tutorial002_an_py39.py` & `readyapi-0.110.3/tests/test_tutorial/test_background_tasks/test_tutorial002_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_background_tasks/test_tutorial002_py310.py` & `readyapi-0.110.3/tests/test_tutorial/test_background_tasks/test_tutorial002_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_behind_a_proxy/test_tutorial001.py` & `readyapi-0.110.3/tests/test_tutorial/test_behind_a_proxy/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_behind_a_proxy/test_tutorial002.py` & `readyapi-0.110.3/tests/test_tutorial/test_behind_a_proxy/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_behind_a_proxy/test_tutorial003.py` & `readyapi-0.110.3/tests/test_tutorial/test_behind_a_proxy/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_behind_a_proxy/test_tutorial004.py` & `readyapi-0.110.3/tests/test_tutorial/test_behind_a_proxy/test_tutorial004.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_bigger_applications/test_main.py` & `readyapi-0.110.3/tests/test_tutorial/test_bigger_applications/test_main.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_bigger_applications/test_main_an.py` & `readyapi-0.110.3/tests/test_tutorial/test_bigger_applications/test_main_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_bigger_applications/test_main_an_py39.py` & `readyapi-0.110.3/tests/test_tutorial/test_bigger_applications/test_main_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_body/test_tutorial001.py` & `readyapi-0.110.3/tests/test_tutorial/test_body/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_body/test_tutorial001_py310.py` & `readyapi-0.110.3/tests/test_tutorial/test_body/test_tutorial001_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_body_fields/test_tutorial001.py` & `readyapi-0.110.3/tests/test_tutorial/test_body_fields/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_body_fields/test_tutorial001_an.py` & `readyapi-0.110.3/tests/test_tutorial/test_body_fields/test_tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_body_fields/test_tutorial001_an_py310.py` & `readyapi-0.110.3/tests/test_tutorial/test_body_fields/test_tutorial001_an_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_body_fields/test_tutorial001_an_py39.py` & `readyapi-0.110.3/tests/test_tutorial/test_body_fields/test_tutorial001_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_body_fields/test_tutorial001_py310.py` & `readyapi-0.110.3/tests/test_tutorial/test_body_fields/test_tutorial001_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_body_multiple_params/test_tutorial001.py` & `readyapi-0.110.3/tests/test_tutorial/test_body_multiple_params/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_body_multiple_params/test_tutorial001_an.py` & `readyapi-0.110.3/tests/test_tutorial/test_body_multiple_params/test_tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_body_multiple_params/test_tutorial001_an_py310.py` & `readyapi-0.110.3/tests/test_tutorial/test_body_multiple_params/test_tutorial001_an_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_body_multiple_params/test_tutorial001_an_py39.py` & `readyapi-0.110.3/tests/test_tutorial/test_body_multiple_params/test_tutorial001_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_body_multiple_params/test_tutorial001_py310.py` & `readyapi-0.110.3/tests/test_tutorial/test_body_multiple_params/test_tutorial001_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_body_multiple_params/test_tutorial003.py` & `readyapi-0.110.3/tests/test_tutorial/test_body_multiple_params/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_body_multiple_params/test_tutorial003_an.py` & `readyapi-0.110.3/tests/test_tutorial/test_body_multiple_params/test_tutorial003_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_body_multiple_params/test_tutorial003_an_py310.py` & `readyapi-0.110.3/tests/test_tutorial/test_body_multiple_params/test_tutorial003_an_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_body_multiple_params/test_tutorial003_an_py39.py` & `readyapi-0.110.3/tests/test_tutorial/test_body_multiple_params/test_tutorial003_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_body_multiple_params/test_tutorial003_py310.py` & `readyapi-0.110.3/tests/test_tutorial/test_body_multiple_params/test_tutorial003_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_body_nested_models/test_tutorial009.py` & `readyapi-0.110.3/tests/test_tutorial/test_body_nested_models/test_tutorial009.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_body_nested_models/test_tutorial009_py39.py` & `readyapi-0.110.3/tests/test_tutorial/test_body_nested_models/test_tutorial009_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_body_updates/test_tutorial001.py` & `readyapi-0.110.3/tests/test_tutorial/test_body_updates/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_body_updates/test_tutorial001_py310.py` & `readyapi-0.110.3/tests/test_tutorial/test_body_updates/test_tutorial001_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_body_updates/test_tutorial001_py39.py` & `readyapi-0.110.3/tests/test_tutorial/test_body_updates/test_tutorial001_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_conditional_openapi/test_tutorial001.py` & `readyapi-0.110.3/tests/test_tutorial/test_conditional_openapi/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_configure_swagger_ui/test_tutorial001.py` & `readyapi-0.110.3/tests/test_tutorial/test_configure_swagger_ui/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_configure_swagger_ui/test_tutorial002.py` & `readyapi-0.110.3/tests/test_tutorial/test_configure_swagger_ui/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_configure_swagger_ui/test_tutorial003.py` & `readyapi-0.110.3/tests/test_tutorial/test_configure_swagger_ui/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_cookie_params/test_tutorial001.py` & `readyapi-0.110.3/tests/test_tutorial/test_cookie_params/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_cookie_params/test_tutorial001_an.py` & `readyapi-0.110.3/tests/test_tutorial/test_cookie_params/test_tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_cookie_params/test_tutorial001_an_py310.py` & `readyapi-0.110.3/tests/test_tutorial/test_cookie_params/test_tutorial001_an_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_cookie_params/test_tutorial001_an_py39.py` & `readyapi-0.110.3/tests/test_tutorial/test_cookie_params/test_tutorial001_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_cookie_params/test_tutorial001_py310.py` & `readyapi-0.110.3/tests/test_tutorial/test_cookie_params/test_tutorial001_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_cors/test_tutorial001.py` & `readyapi-0.110.3/tests/test_tutorial/test_cors/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_custom_docs_ui/test_tutorial001.py` & `readyapi-0.110.3/tests/test_tutorial/test_custom_docs_ui/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_custom_docs_ui/test_tutorial002.py` & `readyapi-0.110.3/tests/test_tutorial/test_custom_docs_ui/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_custom_request_and_route/test_tutorial001.py` & `readyapi-0.110.3/tests/test_tutorial/test_custom_request_and_route/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_custom_request_and_route/test_tutorial002.py` & `readyapi-0.110.3/tests/test_tutorial/test_custom_request_and_route/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_custom_request_and_route/test_tutorial003.py` & `readyapi-0.110.3/tests/test_tutorial/test_custom_request_and_route/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_custom_response/test_tutorial001.py` & `readyapi-0.110.3/tests/test_tutorial/test_custom_response/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_custom_response/test_tutorial001b.py` & `readyapi-0.110.3/tests/test_tutorial/test_custom_response/test_tutorial001b.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_custom_response/test_tutorial004.py` & `readyapi-0.110.3/tests/test_tutorial/test_custom_response/test_tutorial004.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_custom_response/test_tutorial005.py` & `readyapi-0.110.3/tests/test_tutorial/test_custom_response/test_tutorial005.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_custom_response/test_tutorial006.py` & `readyapi-0.110.3/tests/test_tutorial/test_custom_response/test_tutorial006.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_custom_response/test_tutorial006b.py` & `readyapi-0.110.3/tests/test_tutorial/test_custom_response/test_tutorial006b.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_custom_response/test_tutorial006c.py` & `readyapi-0.110.3/tests/test_tutorial/test_custom_response/test_tutorial006c.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_dataclasses/test_tutorial001.py` & `readyapi-0.110.3/tests/test_tutorial/test_dataclasses/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_dataclasses/test_tutorial002.py` & `readyapi-0.110.3/tests/test_tutorial/test_dataclasses/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_dataclasses/test_tutorial003.py` & `readyapi-0.110.3/tests/test_tutorial/test_dataclasses/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_dependencies/test_tutorial001.py` & `readyapi-0.110.3/tests/test_tutorial/test_dependencies/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_dependencies/test_tutorial001_an.py` & `readyapi-0.110.3/tests/test_tutorial/test_dependencies/test_tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_dependencies/test_tutorial001_an_py310.py` & `readyapi-0.110.3/tests/test_tutorial/test_dependencies/test_tutorial001_an_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_dependencies/test_tutorial001_an_py39.py` & `readyapi-0.110.3/tests/test_tutorial/test_dependencies/test_tutorial001_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_dependencies/test_tutorial001_py310.py` & `readyapi-0.110.3/tests/test_tutorial/test_dependencies/test_tutorial001_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_dependencies/test_tutorial004.py` & `readyapi-0.110.3/tests/test_tutorial/test_dependencies/test_tutorial004.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_dependencies/test_tutorial004_an.py` & `readyapi-0.110.3/tests/test_tutorial/test_dependencies/test_tutorial004_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_dependencies/test_tutorial004_an_py310.py` & `readyapi-0.110.3/tests/test_tutorial/test_dependencies/test_tutorial004_an_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_dependencies/test_tutorial004_an_py39.py` & `readyapi-0.110.3/tests/test_tutorial/test_dependencies/test_tutorial004_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_dependencies/test_tutorial004_py310.py` & `readyapi-0.110.3/tests/test_tutorial/test_dependencies/test_tutorial004_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_dependencies/test_tutorial006.py` & `readyapi-0.110.3/tests/test_tutorial/test_dependencies/test_tutorial006.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_dependencies/test_tutorial006_an.py` & `readyapi-0.110.3/tests/test_tutorial/test_dependencies/test_tutorial006_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_dependencies/test_tutorial006_an_py39.py` & `readyapi-0.110.3/tests/test_tutorial/test_dependencies/test_tutorial006_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_dependencies/test_tutorial008b.py` & `readyapi-0.110.3/tests/test_tutorial/test_dependencies/test_tutorial008b.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_dependencies/test_tutorial008b_an.py` & `readyapi-0.110.3/tests/test_tutorial/test_dependencies/test_tutorial008b_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_dependencies/test_tutorial008b_an_py39.py` & `readyapi-0.110.3/tests/test_tutorial/test_dependencies/test_tutorial008b_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_dependencies/test_tutorial008c.py` & `readyapi-0.110.3/tests/test_tutorial/test_dependencies/test_tutorial008c.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_dependencies/test_tutorial008c_an.py` & `readyapi-0.110.3/tests/test_tutorial/test_dependencies/test_tutorial008c_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_dependencies/test_tutorial008c_an_py39.py` & `readyapi-0.110.3/tests/test_tutorial/test_dependencies/test_tutorial008c_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_dependencies/test_tutorial008d.py` & `readyapi-0.110.3/tests/test_tutorial/test_dependencies/test_tutorial008d.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_dependencies/test_tutorial008d_an.py` & `readyapi-0.110.3/tests/test_tutorial/test_dependencies/test_tutorial008d_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_dependencies/test_tutorial008d_an_py39.py` & `readyapi-0.110.3/tests/test_tutorial/test_dependencies/test_tutorial008d_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_dependencies/test_tutorial012.py` & `readyapi-0.110.3/tests/test_tutorial/test_dependencies/test_tutorial012.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_dependencies/test_tutorial012_an.py` & `readyapi-0.110.3/tests/test_tutorial/test_dependencies/test_tutorial012_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_dependencies/test_tutorial012_an_py39.py` & `readyapi-0.110.3/tests/test_tutorial/test_dependencies/test_tutorial012_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_events/test_tutorial001.py` & `readyapi-0.110.3/tests/test_tutorial/test_events/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_events/test_tutorial002.py` & `readyapi-0.110.3/tests/test_tutorial/test_events/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_events/test_tutorial003.py` & `readyapi-0.110.3/tests/test_tutorial/test_events/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_extending_openapi/test_tutorial001.py` & `readyapi-0.110.3/tests/test_tutorial/test_extending_openapi/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_extra_data_types/test_tutorial001.py` & `readyapi-0.110.3/tests/test_tutorial/test_extra_data_types/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_extra_data_types/test_tutorial001_an.py` & `readyapi-0.110.3/tests/test_tutorial/test_extra_data_types/test_tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_extra_data_types/test_tutorial001_an_py310.py` & `readyapi-0.110.3/tests/test_tutorial/test_extra_data_types/test_tutorial001_an_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_extra_data_types/test_tutorial001_an_py39.py` & `readyapi-0.110.3/tests/test_tutorial/test_extra_data_types/test_tutorial001_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_extra_data_types/test_tutorial001_py310.py` & `readyapi-0.110.3/tests/test_tutorial/test_extra_data_types/test_tutorial001_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_extra_models/test_tutorial003.py` & `readyapi-0.110.3/tests/test_tutorial/test_extra_models/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_extra_models/test_tutorial003_py310.py` & `readyapi-0.110.3/tests/test_tutorial/test_extra_models/test_tutorial003_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_extra_models/test_tutorial004.py` & `readyapi-0.110.3/tests/test_tutorial/test_extra_models/test_tutorial004.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_extra_models/test_tutorial004_py39.py` & `readyapi-0.110.3/tests/test_tutorial/test_extra_models/test_tutorial004_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_extra_models/test_tutorial005.py` & `readyapi-0.110.3/tests/test_tutorial/test_extra_models/test_tutorial005.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_extra_models/test_tutorial005_py39.py` & `readyapi-0.110.3/tests/test_tutorial/test_extra_models/test_tutorial005_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_first_steps/test_tutorial001.py` & `readyapi-0.110.3/tests/test_tutorial/test_first_steps/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_generate_clients/test_tutorial003.py` & `readyapi-0.110.3/tests/test_tutorial/test_generate_clients/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_handling_errors/test_tutorial001.py` & `readyapi-0.110.3/tests/test_tutorial/test_handling_errors/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_handling_errors/test_tutorial002.py` & `readyapi-0.110.3/tests/test_tutorial/test_handling_errors/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_handling_errors/test_tutorial003.py` & `readyapi-0.110.3/tests/test_tutorial/test_handling_errors/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_handling_errors/test_tutorial004.py` & `readyapi-0.110.3/tests/test_tutorial/test_handling_errors/test_tutorial004.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_handling_errors/test_tutorial005.py` & `readyapi-0.110.3/tests/test_tutorial/test_handling_errors/test_tutorial005.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_handling_errors/test_tutorial006.py` & `readyapi-0.110.3/tests/test_tutorial/test_handling_errors/test_tutorial006.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_header_params/test_tutorial001.py` & `readyapi-0.110.3/tests/test_tutorial/test_header_params/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_header_params/test_tutorial001_an.py` & `readyapi-0.110.3/tests/test_tutorial/test_header_params/test_tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_header_params/test_tutorial001_an_py310.py` & `readyapi-0.110.3/tests/test_tutorial/test_header_params/test_tutorial001_an_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_header_params/test_tutorial001_py310.py` & `readyapi-0.110.3/tests/test_tutorial/test_header_params/test_tutorial001_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_header_params/test_tutorial002.py` & `readyapi-0.110.3/tests/test_tutorial/test_header_params/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_header_params/test_tutorial002_an.py` & `readyapi-0.110.3/tests/test_tutorial/test_header_params/test_tutorial002_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_header_params/test_tutorial002_an_py310.py` & `readyapi-0.110.3/tests/test_tutorial/test_header_params/test_tutorial002_an_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_header_params/test_tutorial002_an_py39.py` & `readyapi-0.110.3/tests/test_tutorial/test_header_params/test_tutorial002_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_header_params/test_tutorial002_py310.py` & `readyapi-0.110.3/tests/test_tutorial/test_header_params/test_tutorial002_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_header_params/test_tutorial003.py` & `readyapi-0.110.3/tests/test_tutorial/test_header_params/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_header_params/test_tutorial003_an.py` & `readyapi-0.110.3/tests/test_tutorial/test_header_params/test_tutorial003_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_header_params/test_tutorial003_an_py310.py` & `readyapi-0.110.3/tests/test_tutorial/test_header_params/test_tutorial003_an_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_header_params/test_tutorial003_an_py39.py` & `readyapi-0.110.3/tests/test_tutorial/test_header_params/test_tutorial003_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_header_params/test_tutorial003_py310.py` & `readyapi-0.110.3/tests/test_tutorial/test_header_params/test_tutorial003_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_metadata/test_tutorial001.py` & `readyapi-0.110.3/tests/test_tutorial/test_metadata/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_metadata/test_tutorial001_1.py` & `readyapi-0.110.3/tests/test_tutorial/test_metadata/test_tutorial001_1.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_metadata/test_tutorial004.py` & `readyapi-0.110.3/tests/test_tutorial/test_metadata/test_tutorial004.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_openapi_callbacks/test_tutorial001.py` & `readyapi-0.110.3/tests/test_tutorial/test_openapi_callbacks/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_openapi_webhooks/test_tutorial001.py` & `readyapi-0.110.3/tests/test_tutorial/test_openapi_webhooks/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial001.py` & `readyapi-0.110.3/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial002.py` & `readyapi-0.110.3/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial003.py` & `readyapi-0.110.3/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial004.py` & `readyapi-0.110.3/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial004.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial005.py` & `readyapi-0.110.3/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial005.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial006.py` & `readyapi-0.110.3/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial006.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial007.py` & `readyapi-0.110.3/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial007.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial007_pv1.py` & `readyapi-0.110.3/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial007_pv1.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_path_operation_configurations/test_tutorial002b.py` & `readyapi-0.110.3/tests/test_tutorial/test_path_operation_configurations/test_tutorial002b.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_path_operation_configurations/test_tutorial005.py` & `readyapi-0.110.3/tests/test_tutorial/test_path_operation_configurations/test_tutorial005.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_path_operation_configurations/test_tutorial005_py310.py` & `readyapi-0.110.3/tests/test_tutorial/test_path_operation_configurations/test_tutorial005_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_path_operation_configurations/test_tutorial005_py39.py` & `readyapi-0.110.3/tests/test_tutorial/test_path_operation_configurations/test_tutorial005_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_path_operation_configurations/test_tutorial006.py` & `readyapi-0.110.3/tests/test_tutorial/test_path_operation_configurations/test_tutorial006.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_path_params/test_tutorial004.py` & `readyapi-0.110.3/tests/test_tutorial/test_path_params/test_tutorial004.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_path_params/test_tutorial005.py` & `readyapi-0.110.3/tests/test_tutorial/test_path_params/test_tutorial005.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_query_params/test_tutorial005.py` & `readyapi-0.110.3/tests/test_tutorial/test_query_params/test_tutorial005.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_query_params/test_tutorial006.py` & `readyapi-0.110.3/tests/test_tutorial/test_query_params/test_tutorial006.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_query_params/test_tutorial006_py310.py` & `readyapi-0.110.3/tests/test_tutorial/test_query_params/test_tutorial006_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial010.py` & `readyapi-0.110.3/tests/test_tutorial/test_query_params_str_validations/test_tutorial010.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial010_an.py` & `readyapi-0.110.3/tests/test_tutorial/test_query_params_str_validations/test_tutorial010_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial010_an_py310.py` & `readyapi-0.110.3/tests/test_tutorial/test_query_params_str_validations/test_tutorial010_an_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial010_an_py39.py` & `readyapi-0.110.3/tests/test_tutorial/test_query_params_str_validations/test_tutorial010_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial010_py310.py` & `readyapi-0.110.3/tests/test_tutorial/test_query_params_str_validations/test_tutorial010_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial011.py` & `readyapi-0.110.3/tests/test_tutorial/test_query_params_str_validations/test_tutorial011.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial011_an.py` & `readyapi-0.110.3/tests/test_tutorial/test_query_params_str_validations/test_tutorial011_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial011_an_py310.py` & `readyapi-0.110.3/tests/test_tutorial/test_query_params_str_validations/test_tutorial011_an_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial011_an_py39.py` & `readyapi-0.110.3/tests/test_tutorial/test_query_params_str_validations/test_tutorial011_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial011_py310.py` & `readyapi-0.110.3/tests/test_tutorial/test_query_params_str_validations/test_tutorial011_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial011_py39.py` & `readyapi-0.110.3/tests/test_tutorial/test_query_params_str_validations/test_tutorial011_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial012.py` & `readyapi-0.110.3/tests/test_tutorial/test_query_params_str_validations/test_tutorial012.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial012_an.py` & `readyapi-0.110.3/tests/test_tutorial/test_query_params_str_validations/test_tutorial012_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial012_an_py39.py` & `readyapi-0.110.3/tests/test_tutorial/test_query_params_str_validations/test_tutorial012_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial012_py39.py` & `readyapi-0.110.3/tests/test_tutorial/test_query_params_str_validations/test_tutorial012_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial013.py` & `readyapi-0.110.3/tests/test_tutorial/test_query_params_str_validations/test_tutorial013.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial013_an.py` & `readyapi-0.110.3/tests/test_tutorial/test_query_params_str_validations/test_tutorial013_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial013_an_py39.py` & `readyapi-0.110.3/tests/test_tutorial/test_query_params_str_validations/test_tutorial013_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial014.py` & `readyapi-0.110.3/tests/test_tutorial/test_query_params_str_validations/test_tutorial014.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial014_an.py` & `readyapi-0.110.3/tests/test_tutorial/test_query_params_str_validations/test_tutorial014_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial014_an_py310.py` & `readyapi-0.110.3/tests/test_tutorial/test_query_params_str_validations/test_tutorial014_an_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial014_an_py39.py` & `readyapi-0.110.3/tests/test_tutorial/test_query_params_str_validations/test_tutorial014_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial014_py310.py` & `readyapi-0.110.3/tests/test_tutorial/test_query_params_str_validations/test_tutorial014_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_request_files/test_tutorial001.py` & `readyapi-0.110.3/tests/test_tutorial/test_request_files/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_request_files/test_tutorial001_02.py` & `readyapi-0.110.3/tests/test_tutorial/test_request_files/test_tutorial001_02.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_request_files/test_tutorial001_02_an.py` & `readyapi-0.110.3/tests/test_tutorial/test_request_files/test_tutorial001_02_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_request_files/test_tutorial001_02_an_py310.py` & `readyapi-0.110.3/tests/test_tutorial/test_request_files/test_tutorial001_02_an_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_request_files/test_tutorial001_02_an_py39.py` & `readyapi-0.110.3/tests/test_tutorial/test_request_files/test_tutorial001_02_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_request_files/test_tutorial001_02_py310.py` & `readyapi-0.110.3/tests/test_tutorial/test_request_files/test_tutorial001_02_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_request_files/test_tutorial001_03.py` & `readyapi-0.110.3/tests/test_tutorial/test_request_files/test_tutorial001_03.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_request_files/test_tutorial001_03_an.py` & `readyapi-0.110.3/tests/test_tutorial/test_request_files/test_tutorial001_03_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_request_files/test_tutorial001_03_an_py39.py` & `readyapi-0.110.3/tests/test_tutorial/test_request_files/test_tutorial001_03_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_request_files/test_tutorial001_an.py` & `readyapi-0.110.3/tests/test_tutorial/test_request_files/test_tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_request_files/test_tutorial001_an_py39.py` & `readyapi-0.110.3/tests/test_tutorial/test_request_files/test_tutorial001_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_request_files/test_tutorial002.py` & `readyapi-0.110.3/tests/test_tutorial/test_request_files/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_request_files/test_tutorial002_an.py` & `readyapi-0.110.3/tests/test_tutorial/test_request_files/test_tutorial002_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_request_files/test_tutorial002_an_py39.py` & `readyapi-0.110.3/tests/test_tutorial/test_request_files/test_tutorial002_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_request_files/test_tutorial002_py39.py` & `readyapi-0.110.3/tests/test_tutorial/test_request_files/test_tutorial002_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_request_files/test_tutorial003.py` & `readyapi-0.110.3/tests/test_tutorial/test_request_files/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_request_files/test_tutorial003_an.py` & `readyapi-0.110.3/tests/test_tutorial/test_request_files/test_tutorial003_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_request_files/test_tutorial003_an_py39.py` & `readyapi-0.110.3/tests/test_tutorial/test_request_files/test_tutorial003_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_request_files/test_tutorial003_py39.py` & `readyapi-0.110.3/tests/test_tutorial/test_request_files/test_tutorial003_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_request_forms/test_tutorial001.py` & `readyapi-0.110.3/tests/test_tutorial/test_request_forms/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_request_forms/test_tutorial001_an.py` & `readyapi-0.110.3/tests/test_tutorial/test_request_forms/test_tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_request_forms/test_tutorial001_an_py39.py` & `readyapi-0.110.3/tests/test_tutorial/test_request_forms/test_tutorial001_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_request_forms_and_files/test_tutorial001.py` & `readyapi-0.110.3/tests/test_tutorial/test_request_forms_and_files/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_request_forms_and_files/test_tutorial001_an.py` & `readyapi-0.110.3/tests/test_tutorial/test_request_forms_and_files/test_tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_request_forms_and_files/test_tutorial001_an_py39.py` & `readyapi-0.110.3/tests/test_tutorial/test_request_forms_and_files/test_tutorial001_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_response_change_status_code/test_tutorial001.py` & `readyapi-0.110.3/tests/test_tutorial/test_response_change_status_code/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_response_model/test_tutorial003.py` & `readyapi-0.110.3/tests/test_tutorial/test_response_model/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_response_model/test_tutorial003_01.py` & `readyapi-0.110.3/tests/test_tutorial/test_response_model/test_tutorial003_01.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_response_model/test_tutorial003_01_py310.py` & `readyapi-0.110.3/tests/test_tutorial/test_response_model/test_tutorial003_01_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_response_model/test_tutorial003_02.py` & `readyapi-0.110.3/tests/test_tutorial/test_response_model/test_tutorial003_02.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_response_model/test_tutorial003_03.py` & `readyapi-0.110.3/tests/test_tutorial/test_response_model/test_tutorial003_03.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_response_model/test_tutorial003_05.py` & `readyapi-0.110.3/tests/test_tutorial/test_response_model/test_tutorial003_05.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_response_model/test_tutorial003_05_py310.py` & `readyapi-0.110.3/tests/test_tutorial/test_response_model/test_tutorial003_05_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_response_model/test_tutorial003_py310.py` & `readyapi-0.110.3/tests/test_tutorial/test_response_model/test_tutorial003_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_response_model/test_tutorial004.py` & `readyapi-0.110.3/tests/test_tutorial/test_response_model/test_tutorial004.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_response_model/test_tutorial004_py310.py` & `readyapi-0.110.3/tests/test_tutorial/test_response_model/test_tutorial004_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_response_model/test_tutorial004_py39.py` & `readyapi-0.110.3/tests/test_tutorial/test_response_model/test_tutorial004_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_response_model/test_tutorial005.py` & `readyapi-0.110.3/tests/test_tutorial/test_response_model/test_tutorial005.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_response_model/test_tutorial005_py310.py` & `readyapi-0.110.3/tests/test_tutorial/test_response_model/test_tutorial005_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_response_model/test_tutorial006.py` & `readyapi-0.110.3/tests/test_tutorial/test_response_model/test_tutorial006.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_response_model/test_tutorial006_py310.py` & `readyapi-0.110.3/tests/test_tutorial/test_response_model/test_tutorial006_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_schema_extra_example/test_tutorial001.py` & `readyapi-0.110.3/tests/test_tutorial/test_schema_extra_example/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_schema_extra_example/test_tutorial001_pv1.py` & `readyapi-0.110.3/tests/test_tutorial/test_schema_extra_example/test_tutorial001_pv1.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_schema_extra_example/test_tutorial001_py310.py` & `readyapi-0.110.3/tests/test_tutorial/test_schema_extra_example/test_tutorial001_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_schema_extra_example/test_tutorial001_py310_pv1.py` & `readyapi-0.110.3/tests/test_tutorial/test_schema_extra_example/test_tutorial001_py310_pv1.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_schema_extra_example/test_tutorial004.py` & `readyapi-0.110.3/tests/test_tutorial/test_schema_extra_example/test_tutorial004.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_schema_extra_example/test_tutorial004_an.py` & `readyapi-0.110.3/tests/test_tutorial/test_schema_extra_example/test_tutorial004_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_schema_extra_example/test_tutorial004_an_py310.py` & `readyapi-0.110.3/tests/test_tutorial/test_schema_extra_example/test_tutorial004_an_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_schema_extra_example/test_tutorial004_an_py39.py` & `readyapi-0.110.3/tests/test_tutorial/test_schema_extra_example/test_tutorial004_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_schema_extra_example/test_tutorial004_py310.py` & `readyapi-0.110.3/tests/test_tutorial/test_schema_extra_example/test_tutorial004_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_schema_extra_example/test_tutorial005.py` & `readyapi-0.110.3/tests/test_tutorial/test_schema_extra_example/test_tutorial005.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_schema_extra_example/test_tutorial005_an.py` & `readyapi-0.110.3/tests/test_tutorial/test_schema_extra_example/test_tutorial005_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_schema_extra_example/test_tutorial005_an_py310.py` & `readyapi-0.110.3/tests/test_tutorial/test_schema_extra_example/test_tutorial005_an_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_schema_extra_example/test_tutorial005_an_py39.py` & `readyapi-0.110.3/tests/test_tutorial/test_schema_extra_example/test_tutorial005_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_schema_extra_example/test_tutorial005_py310.py` & `readyapi-0.110.3/tests/test_tutorial/test_schema_extra_example/test_tutorial005_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_security/test_tutorial001.py` & `readyapi-0.110.3/tests/test_tutorial/test_security/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_security/test_tutorial001_an.py` & `readyapi-0.110.3/tests/test_tutorial/test_security/test_tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_security/test_tutorial001_an_py39.py` & `readyapi-0.110.3/tests/test_tutorial/test_security/test_tutorial001_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_security/test_tutorial003.py` & `readyapi-0.110.3/tests/test_tutorial/test_security/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_security/test_tutorial003_an.py` & `readyapi-0.110.3/tests/test_tutorial/test_security/test_tutorial003_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_security/test_tutorial003_an_py310.py` & `readyapi-0.110.3/tests/test_tutorial/test_security/test_tutorial003_an_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_security/test_tutorial003_an_py39.py` & `readyapi-0.110.3/tests/test_tutorial/test_security/test_tutorial003_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_security/test_tutorial003_py310.py` & `readyapi-0.110.3/tests/test_tutorial/test_security/test_tutorial003_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_security/test_tutorial005.py` & `readyapi-0.110.3/tests/test_tutorial/test_security/test_tutorial005.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_security/test_tutorial005_an.py` & `readyapi-0.110.3/tests/test_tutorial/test_security/test_tutorial005_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_security/test_tutorial005_an_py310.py` & `readyapi-0.110.3/tests/test_tutorial/test_security/test_tutorial005_an_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_security/test_tutorial005_an_py39.py` & `readyapi-0.110.3/tests/test_tutorial/test_security/test_tutorial005_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_security/test_tutorial005_py310.py` & `readyapi-0.110.3/tests/test_tutorial/test_security/test_tutorial005_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_security/test_tutorial005_py39.py` & `readyapi-0.110.3/tests/test_tutorial/test_security/test_tutorial005_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_security/test_tutorial006.py` & `readyapi-0.110.3/tests/test_tutorial/test_security/test_tutorial006.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_security/test_tutorial006_an.py` & `readyapi-0.110.3/tests/test_tutorial/test_security/test_tutorial006_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_security/test_tutorial006_an_py39.py` & `readyapi-0.110.3/tests/test_tutorial/test_security/test_tutorial006_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_separate_openapi_schemas/test_tutorial001.py` & `readyapi-0.110.3/tests/test_tutorial/test_separate_openapi_schemas/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_separate_openapi_schemas/test_tutorial001_py310.py` & `readyapi-0.110.3/tests/test_tutorial/test_separate_openapi_schemas/test_tutorial001_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_separate_openapi_schemas/test_tutorial001_py39.py` & `readyapi-0.110.3/tests/test_tutorial/test_separate_openapi_schemas/test_tutorial001_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_separate_openapi_schemas/test_tutorial002.py` & `readyapi-0.110.3/tests/test_tutorial/test_separate_openapi_schemas/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_separate_openapi_schemas/test_tutorial002_py310.py` & `readyapi-0.110.3/tests/test_tutorial/test_separate_openapi_schemas/test_tutorial002_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_separate_openapi_schemas/test_tutorial002_py39.py` & `readyapi-0.110.3/tests/test_tutorial/test_separate_openapi_schemas/test_tutorial002_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_settings/test_tutorial001.py` & `readyapi-0.110.3/tests/test_tutorial/test_settings/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_settings/test_tutorial001_pv1.py` & `readyapi-0.110.3/tests/test_tutorial/test_settings/test_tutorial001_pv1.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_sql_databases/test_sql_databases.py` & `readyapi-0.110.3/tests/test_tutorial/test_sql_databases/test_sql_databases.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_sql_databases/test_sql_databases_middleware.py` & `readyapi-0.110.3/tests/test_tutorial/test_sql_databases/test_sql_databases_middleware.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_sql_databases/test_sql_databases_middleware_py310.py` & `readyapi-0.110.3/tests/test_tutorial/test_sql_databases/test_sql_databases_middleware_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_sql_databases/test_sql_databases_middleware_py39.py` & `readyapi-0.110.3/tests/test_tutorial/test_sql_databases/test_sql_databases_middleware_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_sql_databases/test_sql_databases_py310.py` & `readyapi-0.110.3/tests/test_tutorial/test_sql_databases/test_sql_databases_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_sql_databases/test_sql_databases_py39.py` & `readyapi-0.110.3/tests/test_tutorial/test_sql_databases/test_sql_databases_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_sql_databases/test_testing_databases.py` & `readyapi-0.110.3/tests/test_tutorial/test_sql_databases/test_testing_databases.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_sql_databases/test_testing_databases_py310.py` & `readyapi-0.110.3/tests/test_tutorial/test_sql_databases/test_testing_databases_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_sql_databases/test_testing_databases_py39.py` & `readyapi-0.110.3/tests/test_tutorial/test_sql_databases/test_testing_databases_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_sub_applications/test_tutorial001.py` & `readyapi-0.110.3/tests/test_tutorial/test_sub_applications/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_templates/test_tutorial001.py` & `readyapi-0.110.3/tests/test_tutorial/test_templates/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_testing/test_main.py` & `readyapi-0.110.3/tests/test_tutorial/test_testing/test_main.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_testing/test_tutorial001.py` & `readyapi-0.110.3/tests/test_tutorial/test_testing/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_testing_dependencies/test_tutorial001.py` & `readyapi-0.110.3/tests/test_tutorial/test_testing_dependencies/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_testing_dependencies/test_tutorial001_an.py` & `readyapi-0.110.3/tests/test_tutorial/test_testing_dependencies/test_tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_testing_dependencies/test_tutorial001_an_py310.py` & `readyapi-0.110.3/tests/test_tutorial/test_testing_dependencies/test_tutorial001_an_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_testing_dependencies/test_tutorial001_an_py39.py` & `readyapi-0.110.3/tests/test_tutorial/test_testing_dependencies/test_tutorial001_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_testing_dependencies/test_tutorial001_py310.py` & `readyapi-0.110.3/tests/test_tutorial/test_testing_dependencies/test_tutorial001_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_websockets/test_tutorial001.py` & `readyapi-0.110.3/tests/test_tutorial/test_websockets/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_websockets/test_tutorial002.py` & `readyapi-0.110.3/tests/test_tutorial/test_websockets/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_websockets/test_tutorial002_an.py` & `readyapi-0.110.3/tests/test_tutorial/test_websockets/test_tutorial002_an.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_websockets/test_tutorial002_an_py310.py` & `readyapi-0.110.3/tests/test_tutorial/test_websockets/test_tutorial002_an_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_websockets/test_tutorial002_an_py39.py` & `readyapi-0.110.3/tests/test_tutorial/test_websockets/test_tutorial002_an_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_websockets/test_tutorial002_py310.py` & `readyapi-0.110.3/tests/test_tutorial/test_websockets/test_tutorial002_py310.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_websockets/test_tutorial003.py` & `readyapi-0.110.3/tests/test_tutorial/test_websockets/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_tutorial/test_websockets/test_tutorial003_py39.py` & `readyapi-0.110.3/tests/test_tutorial/test_websockets/test_tutorial003_py39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_typing_python39.py` & `readyapi-0.110.3/tests/test_typing_python39.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_union_body.py` & `readyapi-0.110.3/tests/test_union_body.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_union_inherited_body.py` & `readyapi-0.110.3/tests/test_union_inherited_body.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_validate_response.py` & `readyapi-0.110.3/tests/test_validate_response.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_validate_response_dataclass.py` & `readyapi-0.110.3/tests/test_validate_response_dataclass.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_validate_response_recursive/app_pv1.py` & `readyapi-0.110.3/tests/test_validate_response_recursive/app_pv1.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_validate_response_recursive/app_pv2.py` & `readyapi-0.110.3/tests/test_validate_response_recursive/app_pv2.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_validate_response_recursive/test_validate_response_recursive_pv1.py` & `readyapi-0.110.3/tests/test_validate_response_recursive/test_validate_response_recursive_pv1.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_validate_response_recursive/test_validate_response_recursive_pv2.py` & `readyapi-0.110.3/tests/test_validate_response_recursive/test_validate_response_recursive_pv2.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_webhooks_security.py` & `readyapi-0.110.3/tests/test_webhooks_security.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_ws_dependencies.py` & `readyapi-0.110.3/tests/test_ws_dependencies.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/tests/test_ws_router.py` & `readyapi-0.110.3/tests/test_ws_router.py`

 * *Files identical despite different names*

### Comparing `readyapi-0.110.2.dev1/PKG-INFO` & `readyapi-0.110.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: readyapi
-Version: 0.110.2.dev1
+Version: 0.110.3
 Summary: ReadyAPI framework, high performance, easy to learn, fast to code, ready for production
 Author-Email: KhulnaSoft DevOps <info@khulnasoft.com>
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: readyapi Version: 0.110.2.dev1 Summary: ReadyAPI
+Metadata-Version: 2.1 Name: readyapi Version: 0.110.3 Summary: ReadyAPI
 framework, high performance, easy to learn, fast to code, ready for production
 Author-Email: KhulnaSoft DevOps
 khulnasoft.com> Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators Classifier: Operating
 System :: OS Independent Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python Classifier: Topic :: Internet
 Classifier: Topic :: Software Development :: Libraries :: Application
```

