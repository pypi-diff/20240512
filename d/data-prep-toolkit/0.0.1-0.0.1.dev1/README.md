# Comparing `tmp/data_prep_toolkit-0.0.1.tar.gz` & `tmp/data_prep_toolkit-0.0.1.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_prep_toolkit-0.0.1.tar", last modified: Wed May  8 21:28:18 2024, max compression
+gzip compressed data, was "data_prep_toolkit-0.0.1.dev1.tar", last modified: Sun May 12 06:24:42 2024, max compression
```

## Comparing `data_prep_toolkit-0.0.1.tar` & `data_prep_toolkit-0.0.1.dev1.tar`

### file list

```diff
@@ -1,126 +1,126 @@
-drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-08 21:28:18.021745 data_prep_toolkit-0.0.1/
--rw-r--r--   0 dawood     (501) staff       (20)      357 2024-05-08 20:11:57.000000 data_prep_toolkit-0.0.1/.gitignore
--rw-r--r--   0 dawood     (501) staff       (20)     2395 2024-05-08 20:13:16.000000 data_prep_toolkit-0.0.1/Makefile
--rw-r--r--   0 dawood     (501) staff       (20)     1883 2024-05-08 21:28:18.021499 data_prep_toolkit-0.0.1/PKG-INFO
--rw-r--r--   0 dawood     (501) staff       (20)      963 2024-05-08 20:11:57.000000 data_prep_toolkit-0.0.1/README.md
-drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-08 21:28:18.003651 data_prep_toolkit-0.0.1/doc/
--rw-r--r--   0 dawood     (501) staff       (20)    12779 2024-05-08 20:11:57.000000 data_prep_toolkit-0.0.1/doc/advanced-transform-tutorial.md
--rw-r--r--   0 dawood     (501) staff       (20)     7617 2024-05-08 20:11:57.000000 data_prep_toolkit-0.0.1/doc/architecture.md
--rw-r--r--   0 dawood     (501) staff       (20)     5028 2024-05-08 20:11:57.000000 data_prep_toolkit-0.0.1/doc/launcher-options.md
--rw-r--r--   0 dawood     (501) staff       (20)    34920 2024-05-08 20:11:57.000000 data_prep_toolkit-0.0.1/doc/logo-ibm-dark.png
--rw-r--r--   0 dawood     (501) staff       (20)    35127 2024-05-08 20:11:57.000000 data_prep_toolkit-0.0.1/doc/logo-ibm.png
--rw-r--r--   0 dawood     (501) staff       (20)     1564 2024-05-08 20:11:57.000000 data_prep_toolkit-0.0.1/doc/overview.md
--rw-r--r--   0 dawood     (501) staff       (20)   137580 2024-05-08 20:11:57.000000 data_prep_toolkit-0.0.1/doc/processing-architecture.jpg
--rw-r--r--   0 dawood     (501) staff       (20)     8840 2024-05-08 20:11:57.000000 data_prep_toolkit-0.0.1/doc/simplest-transform-tutorial.md
--rw-r--r--   0 dawood     (501) staff       (20)      193 2024-05-08 20:11:57.000000 data_prep_toolkit-0.0.1/doc/testing-e2e-transform.md
--rw-r--r--   0 dawood     (501) staff       (20)     5888 2024-05-08 20:13:17.000000 data_prep_toolkit-0.0.1/doc/testing-transforms.md
--rw-r--r--   0 dawood     (501) staff       (20)    12175 2024-05-08 20:11:57.000000 data_prep_toolkit-0.0.1/doc/transform-external-resources.md
--rw-r--r--   0 dawood     (501) staff       (20)    10775 2024-05-08 20:11:57.000000 data_prep_toolkit-0.0.1/doc/transform-tutorials.md
--rw-r--r--   0 dawood     (501) staff       (20)     1415 2024-05-08 20:11:57.000000 data_prep_toolkit-0.0.1/doc/transformer-utilities.md
--rw-r--r--   0 dawood     (501) staff       (20)     3614 2024-05-08 20:11:57.000000 data_prep_toolkit-0.0.1/doc/using_s3_transformers.md
--rw-r--r--   0 dawood     (501) staff       (20)     1331 2024-05-08 21:27:50.000000 data_prep_toolkit-0.0.1/pyproject.toml
--rw-r--r--   0 dawood     (501) staff       (20)       38 2024-05-08 21:28:18.021795 data_prep_toolkit-0.0.1/setup.cfg
-drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-08 21:28:17.996420 data_prep_toolkit-0.0.1/src/
-drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-08 21:28:18.020517 data_prep_toolkit-0.0.1/src/data_prep_toolkit.egg-info/
--rw-r--r--   0 dawood     (501) staff       (20)     1883 2024-05-08 21:28:17.000000 data_prep_toolkit-0.0.1/src/data_prep_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 dawood     (501) staff       (20)     3992 2024-05-08 21:28:17.000000 data_prep_toolkit-0.0.1/src/data_prep_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 dawood     (501) staff       (20)        1 2024-05-08 21:28:17.000000 data_prep_toolkit-0.0.1/src/data_prep_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 dawood     (501) staff       (20)      249 2024-05-08 21:28:17.000000 data_prep_toolkit-0.0.1/src/data_prep_toolkit.egg-info/requires.txt
--rw-r--r--   0 dawood     (501) staff       (20)       16 2024-05-08 21:28:17.000000 data_prep_toolkit-0.0.1/src/data_prep_toolkit.egg-info/top_level.txt
-drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-08 21:28:18.004624 data_prep_toolkit-0.0.1/src/data_processing/
--rw-r--r--   0 dawood     (501) staff       (20)        0 2024-05-08 20:11:57.000000 data_prep_toolkit-0.0.1/src/data_processing/__init__.py
-drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-08 21:28:18.005633 data_prep_toolkit-0.0.1/src/data_processing/data_access/
--rw-r--r--   0 dawood     (501) staff       (20)      427 2024-05-08 20:11:57.000000 data_prep_toolkit-0.0.1/src/data_processing/data_access/__init__.py
--rw-r--r--   0 dawood     (501) staff       (20)     8830 2024-05-08 20:11:57.000000 data_prep_toolkit-0.0.1/src/data_processing/data_access/arrow_s3.py
--rw-r--r--   0 dawood     (501) staff       (20)     8484 2024-05-08 20:11:57.000000 data_prep_toolkit-0.0.1/src/data_processing/data_access/data_access.py
--rw-r--r--   0 dawood     (501) staff       (20)    11466 2024-05-08 20:11:57.000000 data_prep_toolkit-0.0.1/src/data_processing/data_access/data_access_factory.py
--rw-r--r--   0 dawood     (501) staff       (20)     5647 2024-05-08 20:11:57.000000 data_prep_toolkit-0.0.1/src/data_processing/data_access/data_access_factory_base.py
--rw-r--r--   0 dawood     (501) staff       (20)    15061 2024-05-08 20:11:57.000000 data_prep_toolkit-0.0.1/src/data_processing/data_access/data_access_local.py
--rw-r--r--   0 dawood     (501) staff       (20)    13499 2024-05-08 20:11:57.000000 data_prep_toolkit-0.0.1/src/data_processing/data_access/data_access_s3.py
-drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-08 21:28:18.006386 data_prep_toolkit-0.0.1/src/data_processing/pure_python/
--rw-r--r--   0 dawood     (501) staff       (20)      346 2024-05-08 20:11:57.000000 data_prep_toolkit-0.0.1/src/data_processing/pure_python/__init__.py
--rw-r--r--   0 dawood     (501) staff       (20)     4122 2024-05-08 20:11:57.000000 data_prep_toolkit-0.0.1/src/data_processing/pure_python/python_launcher_configuration.py
--rw-r--r--   0 dawood     (501) staff       (20)     3800 2024-05-08 20:11:57.000000 data_prep_toolkit-0.0.1/src/data_processing/pure_python/transform_launcher.py
--rw-r--r--   0 dawood     (501) staff       (20)     4252 2024-05-08 20:11:57.000000 data_prep_toolkit-0.0.1/src/data_processing/pure_python/transform_orchestrator.py
--rw-r--r--   0 dawood     (501) staff       (20)     9237 2024-05-08 20:11:57.000000 data_prep_toolkit-0.0.1/src/data_processing/pure_python/transform_table_processor.py
-drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-08 21:28:18.007567 data_prep_toolkit-0.0.1/src/data_processing/ray/
--rw-r--r--   0 dawood     (501) staff       (20)      576 2024-05-08 20:11:57.000000 data_prep_toolkit-0.0.1/src/data_processing/ray/__init__.py
--rw-r--r--   0 dawood     (501) staff       (20)     7404 2024-05-08 20:11:57.000000 data_prep_toolkit-0.0.1/src/data_processing/ray/ray_utils.py
--rw-r--r--   0 dawood     (501) staff       (20)     4743 2024-05-08 20:11:57.000000 data_prep_toolkit-0.0.1/src/data_processing/ray/transform_launcher.py
--rw-r--r--   0 dawood     (501) staff       (20)     6380 2024-05-08 20:11:57.000000 data_prep_toolkit-0.0.1/src/data_processing/ray/transform_orchestrator.py
--rw-r--r--   0 dawood     (501) staff       (20)     4574 2024-05-08 20:11:57.000000 data_prep_toolkit-0.0.1/src/data_processing/ray/transform_orchestrator_configuration.py
--rw-r--r--   0 dawood     (501) staff       (20)     4784 2024-05-08 20:11:57.000000 data_prep_toolkit-0.0.1/src/data_processing/ray/transform_runtime.py
--rw-r--r--   0 dawood     (501) staff       (20)     2883 2024-05-08 20:11:57.000000 data_prep_toolkit-0.0.1/src/data_processing/ray/transform_statistics.py
--rw-r--r--   0 dawood     (501) staff       (20)     9501 2024-05-08 20:11:57.000000 data_prep_toolkit-0.0.1/src/data_processing/ray/transform_table_processor.py
-drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-08 21:28:18.007850 data_prep_toolkit-0.0.1/src/data_processing/test_support/
--rw-r--r--   0 dawood     (501) staff       (20)       62 2024-05-08 20:11:57.000000 data_prep_toolkit-0.0.1/src/data_processing/test_support/__init__.py
--rw-r--r--   0 dawood     (501) staff       (20)     8234 2024-05-08 20:11:57.000000 data_prep_toolkit-0.0.1/src/data_processing/test_support/abstract_test.py
-drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-08 21:28:18.008138 data_prep_toolkit-0.0.1/src/data_processing/test_support/data_access/
--rw-r--r--   0 dawood     (501) staff       (20)       69 2024-05-08 20:11:57.000000 data_prep_toolkit-0.0.1/src/data_processing/test_support/data_access/__init__.py
--rw-r--r--   0 dawood     (501) staff       (20)     2666 2024-05-08 20:11:57.000000 data_prep_toolkit-0.0.1/src/data_processing/test_support/data_access/data_access_factory_test.py
-drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-08 21:28:18.008420 data_prep_toolkit-0.0.1/src/data_processing/test_support/ray/
--rw-r--r--   0 dawood     (501) staff       (20)       58 2024-05-08 20:11:57.000000 data_prep_toolkit-0.0.1/src/data_processing/test_support/ray/__init__.py
--rw-r--r--   0 dawood     (501) staff       (20)     4672 2024-05-08 20:11:57.000000 data_prep_toolkit-0.0.1/src/data_processing/test_support/ray/transform_test.py
-drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-08 21:28:18.008874 data_prep_toolkit-0.0.1/src/data_processing/test_support/transform/
--rw-r--r--   0 dawood     (501) staff       (20)      231 2024-05-08 20:11:57.000000 data_prep_toolkit-0.0.1/src/data_processing/test_support/transform/__init__.py
--rw-r--r--   0 dawood     (501) staff       (20)     5701 2024-05-08 20:11:57.000000 data_prep_toolkit-0.0.1/src/data_processing/test_support/transform/noop_transform.py
--rw-r--r--   0 dawood     (501) staff       (20)     4476 2024-05-08 20:11:57.000000 data_prep_toolkit-0.0.1/src/data_processing/test_support/transform/transform_test.py
-drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-08 21:28:18.009582 data_prep_toolkit-0.0.1/src/data_processing/transform/
--rw-r--r--   0 dawood     (501) staff       (20)      368 2024-05-08 20:11:57.000000 data_prep_toolkit-0.0.1/src/data_processing/transform/__init__.py
--rw-r--r--   0 dawood     (501) staff       (20)     3067 2024-05-08 20:11:57.000000 data_prep_toolkit-0.0.1/src/data_processing/transform/execution_configuration.py
--rw-r--r--   0 dawood     (501) staff       (20)     2521 2024-05-08 20:11:57.000000 data_prep_toolkit-0.0.1/src/data_processing/transform/launcher_configuration.py
--rw-r--r--   0 dawood     (501) staff       (20)     2298 2024-05-08 20:11:57.000000 data_prep_toolkit-0.0.1/src/data_processing/transform/table_transform.py
--rw-r--r--   0 dawood     (501) staff       (20)     1465 2024-05-08 20:11:57.000000 data_prep_toolkit-0.0.1/src/data_processing/transform/transform_statistics.py
-drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-08 21:28:18.011241 data_prep_toolkit-0.0.1/src/data_processing/utils/
--rw-r--r--   0 dawood     (501) staff       (20)      354 2024-05-08 20:14:55.000000 data_prep_toolkit-0.0.1/src/data_processing/utils/__init__.py
--rw-r--r--   0 dawood     (501) staff       (20)     3135 2024-05-08 20:11:57.000000 data_prep_toolkit-0.0.1/src/data_processing/utils/cli_utils.py
--rw-r--r--   0 dawood     (501) staff       (20)     1695 2024-05-08 20:14:55.000000 data_prep_toolkit-0.0.1/src/data_processing/utils/config.py
--rw-r--r--   0 dawood     (501) staff       (20)     2052 2024-05-08 20:14:55.000000 data_prep_toolkit-0.0.1/src/data_processing/utils/log.py
--rw-r--r--   0 dawood     (501) staff       (20)     6029 2024-05-08 20:11:57.000000 data_prep_toolkit-0.0.1/src/data_processing/utils/params_utils.py
--rw-r--r--   0 dawood     (501) staff       (20)     6740 2024-05-08 20:11:57.000000 data_prep_toolkit-0.0.1/src/data_processing/utils/transform_utils.py
-drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-08 21:28:17.998963 data_prep_toolkit-0.0.1/test/
-drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-08 21:28:17.999407 data_prep_toolkit-0.0.1/test/data_processing_tests/
-drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-08 21:28:18.018379 data_prep_toolkit-0.0.1/test/data_processing_tests/data_access/
--rw-r--r--   0 dawood     (501) staff       (20)     1256 2024-05-08 20:11:57.000000 data_prep_toolkit-0.0.1/test/data_processing_tests/data_access/daf_local_test.py
--rw-r--r--   0 dawood     (501) staff       (20)    24597 2024-05-08 20:11:57.000000 data_prep_toolkit-0.0.1/test/data_processing_tests/data_access/data_access_local_test.py
--rw-r--r--   0 dawood     (501) staff       (20)     5734 2024-05-08 20:11:57.000000 data_prep_toolkit-0.0.1/test/data_processing_tests/data_access/data_access_s3_test.py
--rw-r--r--   0 dawood     (501) staff       (20)     1545 2024-05-08 20:11:57.000000 data_prep_toolkit-0.0.1/test/data_processing_tests/data_access/sample_input_data_test.py
-drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-08 21:28:18.018559 data_prep_toolkit-0.0.1/test/data_processing_tests/pure_python/
--rw-r--r--   0 dawood     (501) staff       (20)     9106 2024-05-08 20:11:57.000000 data_prep_toolkit-0.0.1/test/data_processing_tests/pure_python/launcher_test.py
-drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-08 21:28:18.019740 data_prep_toolkit-0.0.1/test/data_processing_tests/ray/
--rw-r--r--   0 dawood     (501) staff       (20)    11220 2024-05-08 20:11:57.000000 data_prep_toolkit-0.0.1/test/data_processing_tests/ray/launcher_test.py
--rw-r--r--   0 dawood     (501) staff       (20)     3288 2024-05-08 20:11:57.000000 data_prep_toolkit-0.0.1/test/data_processing_tests/ray/ray_util_test.py
--rw-r--r--   0 dawood     (501) staff       (20)     1733 2024-05-08 20:11:57.000000 data_prep_toolkit-0.0.1/test/data_processing_tests/ray/test_noop_launch.py
-drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-08 21:28:18.019930 data_prep_toolkit-0.0.1/test/data_processing_tests/transform/
--rw-r--r--   0 dawood     (501) staff       (20)     1678 2024-05-08 20:11:57.000000 data_prep_toolkit-0.0.1/test/data_processing_tests/transform/test_noop.py
-drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-08 21:28:18.020118 data_prep_toolkit-0.0.1/test/data_processing_tests/util/
--rw-r--r--   0 dawood     (501) staff       (20)     1386 2024-05-08 20:11:57.000000 data_prep_toolkit-0.0.1/test/data_processing_tests/util/transform_utils_test.py
-drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-08 21:28:17.997406 data_prep_toolkit-0.0.1/test-data/
-drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-08 21:28:17.998317 data_prep_toolkit-0.0.1/test-data/data_processing/
-drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-08 21:28:17.997945 data_prep_toolkit-0.0.1/test-data/data_processing/daf/
-drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-08 21:28:17.997845 data_prep_toolkit-0.0.1/test-data/data_processing/daf/input/
-drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-08 21:28:18.012222 data_prep_toolkit-0.0.1/test-data/data_processing/daf/input/ds1/
--rw-r--r--   0 dawood     (501) staff       (20)    36132 2024-05-08 20:11:57.000000 data_prep_toolkit-0.0.1/test-data/data_processing/daf/input/ds1/sample1.parquet
--rw-r--r--   0 dawood     (501) staff       (20)    36132 2024-05-08 20:11:57.000000 data_prep_toolkit-0.0.1/test-data/data_processing/daf/input/ds1/sample2.parquet
-drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-08 21:28:18.012806 data_prep_toolkit-0.0.1/test-data/data_processing/daf/input/ds2/
--rw-r--r--   0 dawood     (501) staff       (20)    36132 2024-05-08 20:11:57.000000 data_prep_toolkit-0.0.1/test-data/data_processing/daf/input/ds2/sample3.parquet
-drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-08 21:28:17.998019 data_prep_toolkit-0.0.1/test-data/data_processing/daf/output/
-drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-08 21:28:18.013363 data_prep_toolkit-0.0.1/test-data/data_processing/daf/output/ds1/
--rw-r--r--   0 dawood     (501) staff       (20)    36132 2024-05-08 20:11:57.000000 data_prep_toolkit-0.0.1/test-data/data_processing/daf/output/ds1/sample1.parquet
-drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-08 21:28:18.013974 data_prep_toolkit-0.0.1/test-data/data_processing/input/
--rw-r--r--   0 dawood     (501) staff       (20)    36132 2024-05-08 20:11:57.000000 data_prep_toolkit-0.0.1/test-data/data_processing/input/sample1.parquet
-drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-08 21:28:18.015201 data_prep_toolkit-0.0.1/test-data/data_processing/input_multiple/
--rw-r--r--   0 dawood     (501) staff       (20)    36132 2024-05-08 20:11:57.000000 data_prep_toolkit-0.0.1/test-data/data_processing/input_multiple/sample1.parquet
--rw-r--r--   0 dawood     (501) staff       (20)    36132 2024-05-08 20:11:57.000000 data_prep_toolkit-0.0.1/test-data/data_processing/input_multiple/sample2.parquet
--rw-r--r--   0 dawood     (501) staff       (20)    36132 2024-05-08 20:11:57.000000 data_prep_toolkit-0.0.1/test-data/data_processing/input_multiple/sample3.parquet
-drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-08 21:28:17.998394 data_prep_toolkit-0.0.1/test-data/data_processing/ray/
-drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-08 21:28:17.998709 data_prep_toolkit-0.0.1/test-data/data_processing/ray/noop/
-drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-08 21:28:18.015847 data_prep_toolkit-0.0.1/test-data/data_processing/ray/noop/expected/
--rw-r--r--   0 dawood     (501) staff       (20)     1128 2024-05-08 20:11:57.000000 data_prep_toolkit-0.0.1/test-data/data_processing/ray/noop/expected/metadata.json
--rw-r--r--   0 dawood     (501) staff       (20)    36132 2024-05-08 20:11:57.000000 data_prep_toolkit-0.0.1/test-data/data_processing/ray/noop/expected/sample1.parquet
-drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-08 21:28:18.016293 data_prep_toolkit-0.0.1/test-data/data_processing/ray/noop/expected/subdir/
--rw-r--r--   0 dawood     (501) staff       (20)      753 2024-05-08 20:11:57.000000 data_prep_toolkit-0.0.1/test-data/data_processing/ray/noop/expected/subdir/test1.parquet
-drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-08 21:28:18.016528 data_prep_toolkit-0.0.1/test-data/data_processing/ray/noop/input/
--rw-r--r--   0 dawood     (501) staff       (20)    36132 2024-05-08 20:11:57.000000 data_prep_toolkit-0.0.1/test-data/data_processing/ray/noop/input/sample1.parquet
-drwxr-xr-x   0 dawood     (501) staff       (20)        0 2024-05-08 21:28:18.016956 data_prep_toolkit-0.0.1/test-data/data_processing/ray/noop/input/subdir/
--rw-r--r--   0 dawood     (501) staff       (20)      753 2024-05-08 20:11:57.000000 data_prep_toolkit-0.0.1/test-data/data_processing/ray/noop/input/subdir/test1.parquet
+drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 06:24:42.596930 data_prep_toolkit-0.0.1.dev1/
+-rw-r--r--   0 eres      (1000) eres      (1000)      357 2024-05-12 06:14:53.000000 data_prep_toolkit-0.0.1.dev1/.gitignore
+-rw-r--r--   0 eres      (1000) eres      (1000)     2395 2024-05-12 06:16:24.000000 data_prep_toolkit-0.0.1.dev1/Makefile
+-rw-r--r--   0 eres      (1000) eres      (1000)     1885 2024-05-12 06:24:42.596930 data_prep_toolkit-0.0.1.dev1/PKG-INFO
+-rw-r--r--   0 eres      (1000) eres      (1000)      963 2024-05-12 06:14:53.000000 data_prep_toolkit-0.0.1.dev1/README.md
+drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 06:24:42.576930 data_prep_toolkit-0.0.1.dev1/doc/
+-rw-r--r--   0 eres      (1000) eres      (1000)    12779 2024-05-12 06:16:24.000000 data_prep_toolkit-0.0.1.dev1/doc/advanced-transform-tutorial.md
+-rw-r--r--   0 eres      (1000) eres      (1000)     7617 2024-05-12 06:16:24.000000 data_prep_toolkit-0.0.1.dev1/doc/architecture.md
+-rw-r--r--   0 eres      (1000) eres      (1000)     5028 2024-05-12 06:16:24.000000 data_prep_toolkit-0.0.1.dev1/doc/launcher-options.md
+-rw-r--r--   0 eres      (1000) eres      (1000)    34920 2024-05-12 06:16:24.000000 data_prep_toolkit-0.0.1.dev1/doc/logo-ibm-dark.png
+-rw-r--r--   0 eres      (1000) eres      (1000)    35127 2024-05-12 06:16:24.000000 data_prep_toolkit-0.0.1.dev1/doc/logo-ibm.png
+-rw-r--r--   0 eres      (1000) eres      (1000)     1564 2024-05-12 06:16:24.000000 data_prep_toolkit-0.0.1.dev1/doc/overview.md
+-rw-r--r--   0 eres      (1000) eres      (1000)   137580 2024-05-12 06:14:53.000000 data_prep_toolkit-0.0.1.dev1/doc/processing-architecture.jpg
+-rw-r--r--   0 eres      (1000) eres      (1000)     8840 2024-05-12 06:16:24.000000 data_prep_toolkit-0.0.1.dev1/doc/simplest-transform-tutorial.md
+-rw-r--r--   0 eres      (1000) eres      (1000)      193 2024-05-12 06:14:53.000000 data_prep_toolkit-0.0.1.dev1/doc/testing-e2e-transform.md
+-rw-r--r--   0 eres      (1000) eres      (1000)     5888 2024-05-12 06:16:24.000000 data_prep_toolkit-0.0.1.dev1/doc/testing-transforms.md
+-rw-r--r--   0 eres      (1000) eres      (1000)    12175 2024-05-12 06:14:53.000000 data_prep_toolkit-0.0.1.dev1/doc/transform-external-resources.md
+-rw-r--r--   0 eres      (1000) eres      (1000)    10775 2024-05-12 06:16:24.000000 data_prep_toolkit-0.0.1.dev1/doc/transform-tutorials.md
+-rw-r--r--   0 eres      (1000) eres      (1000)     1415 2024-05-12 06:14:53.000000 data_prep_toolkit-0.0.1.dev1/doc/transformer-utilities.md
+-rw-r--r--   0 eres      (1000) eres      (1000)     3614 2024-05-12 06:16:24.000000 data_prep_toolkit-0.0.1.dev1/doc/using_s3_transformers.md
+-rw-r--r--   0 eres      (1000) eres      (1000)     1333 2024-05-12 06:23:29.000000 data_prep_toolkit-0.0.1.dev1/pyproject.toml
+-rw-r--r--   0 eres      (1000) eres      (1000)       38 2024-05-12 06:24:42.596930 data_prep_toolkit-0.0.1.dev1/setup.cfg
+drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 06:24:42.566930 data_prep_toolkit-0.0.1.dev1/src/
+drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 06:24:42.596930 data_prep_toolkit-0.0.1.dev1/src/data_prep_toolkit.egg-info/
+-rw-r--r--   0 eres      (1000) eres      (1000)     1885 2024-05-12 06:24:42.000000 data_prep_toolkit-0.0.1.dev1/src/data_prep_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 eres      (1000) eres      (1000)     3992 2024-05-12 06:24:42.000000 data_prep_toolkit-0.0.1.dev1/src/data_prep_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 eres      (1000) eres      (1000)        1 2024-05-12 06:24:42.000000 data_prep_toolkit-0.0.1.dev1/src/data_prep_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 eres      (1000) eres      (1000)      249 2024-05-12 06:24:42.000000 data_prep_toolkit-0.0.1.dev1/src/data_prep_toolkit.egg-info/requires.txt
+-rw-r--r--   0 eres      (1000) eres      (1000)       16 2024-05-12 06:24:42.000000 data_prep_toolkit-0.0.1.dev1/src/data_prep_toolkit.egg-info/top_level.txt
+drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 06:24:42.576930 data_prep_toolkit-0.0.1.dev1/src/data_processing/
+-rw-r--r--   0 eres      (1000) eres      (1000)        0 2024-05-12 06:14:53.000000 data_prep_toolkit-0.0.1.dev1/src/data_processing/__init__.py
+drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 06:24:42.586930 data_prep_toolkit-0.0.1.dev1/src/data_processing/data_access/
+-rw-r--r--   0 eres      (1000) eres      (1000)      427 2024-05-12 06:14:53.000000 data_prep_toolkit-0.0.1.dev1/src/data_processing/data_access/__init__.py
+-rw-r--r--   0 eres      (1000) eres      (1000)     8830 2024-05-12 06:16:24.000000 data_prep_toolkit-0.0.1.dev1/src/data_processing/data_access/arrow_s3.py
+-rw-r--r--   0 eres      (1000) eres      (1000)     8484 2024-05-12 06:14:53.000000 data_prep_toolkit-0.0.1.dev1/src/data_processing/data_access/data_access.py
+-rw-r--r--   0 eres      (1000) eres      (1000)    11466 2024-05-12 06:14:53.000000 data_prep_toolkit-0.0.1.dev1/src/data_processing/data_access/data_access_factory.py
+-rw-r--r--   0 eres      (1000) eres      (1000)     5647 2024-05-12 06:14:53.000000 data_prep_toolkit-0.0.1.dev1/src/data_processing/data_access/data_access_factory_base.py
+-rw-r--r--   0 eres      (1000) eres      (1000)    15061 2024-05-12 06:14:53.000000 data_prep_toolkit-0.0.1.dev1/src/data_processing/data_access/data_access_local.py
+-rw-r--r--   0 eres      (1000) eres      (1000)    13499 2024-05-12 06:14:53.000000 data_prep_toolkit-0.0.1.dev1/src/data_processing/data_access/data_access_s3.py
+drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 06:24:42.586930 data_prep_toolkit-0.0.1.dev1/src/data_processing/pure_python/
+-rw-r--r--   0 eres      (1000) eres      (1000)      346 2024-05-12 06:16:24.000000 data_prep_toolkit-0.0.1.dev1/src/data_processing/pure_python/__init__.py
+-rw-r--r--   0 eres      (1000) eres      (1000)     4122 2024-05-12 06:16:24.000000 data_prep_toolkit-0.0.1.dev1/src/data_processing/pure_python/python_launcher_configuration.py
+-rw-r--r--   0 eres      (1000) eres      (1000)     3800 2024-05-12 06:16:24.000000 data_prep_toolkit-0.0.1.dev1/src/data_processing/pure_python/transform_launcher.py
+-rw-r--r--   0 eres      (1000) eres      (1000)     4252 2024-05-12 06:16:24.000000 data_prep_toolkit-0.0.1.dev1/src/data_processing/pure_python/transform_orchestrator.py
+-rw-r--r--   0 eres      (1000) eres      (1000)     9237 2024-05-12 06:16:24.000000 data_prep_toolkit-0.0.1.dev1/src/data_processing/pure_python/transform_table_processor.py
+drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 06:24:42.586930 data_prep_toolkit-0.0.1.dev1/src/data_processing/ray/
+-rw-r--r--   0 eres      (1000) eres      (1000)      576 2024-05-12 06:16:24.000000 data_prep_toolkit-0.0.1.dev1/src/data_processing/ray/__init__.py
+-rw-r--r--   0 eres      (1000) eres      (1000)     7404 2024-05-12 06:16:24.000000 data_prep_toolkit-0.0.1.dev1/src/data_processing/ray/ray_utils.py
+-rw-r--r--   0 eres      (1000) eres      (1000)     4849 2024-05-12 06:19:13.000000 data_prep_toolkit-0.0.1.dev1/src/data_processing/ray/transform_launcher.py
+-rw-r--r--   0 eres      (1000) eres      (1000)     6380 2024-05-12 06:16:24.000000 data_prep_toolkit-0.0.1.dev1/src/data_processing/ray/transform_orchestrator.py
+-rw-r--r--   0 eres      (1000) eres      (1000)     4574 2024-05-12 06:16:24.000000 data_prep_toolkit-0.0.1.dev1/src/data_processing/ray/transform_orchestrator_configuration.py
+-rw-r--r--   0 eres      (1000) eres      (1000)     4784 2024-05-12 06:16:24.000000 data_prep_toolkit-0.0.1.dev1/src/data_processing/ray/transform_runtime.py
+-rw-r--r--   0 eres      (1000) eres      (1000)     2883 2024-05-12 06:16:24.000000 data_prep_toolkit-0.0.1.dev1/src/data_processing/ray/transform_statistics.py
+-rw-r--r--   0 eres      (1000) eres      (1000)     9501 2024-05-12 06:16:24.000000 data_prep_toolkit-0.0.1.dev1/src/data_processing/ray/transform_table_processor.py
+drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 06:24:42.586930 data_prep_toolkit-0.0.1.dev1/src/data_processing/test_support/
+-rw-r--r--   0 eres      (1000) eres      (1000)       62 2024-05-12 06:14:53.000000 data_prep_toolkit-0.0.1.dev1/src/data_processing/test_support/__init__.py
+-rw-r--r--   0 eres      (1000) eres      (1000)     8234 2024-05-12 06:14:53.000000 data_prep_toolkit-0.0.1.dev1/src/data_processing/test_support/abstract_test.py
+drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 06:24:42.586930 data_prep_toolkit-0.0.1.dev1/src/data_processing/test_support/data_access/
+-rw-r--r--   0 eres      (1000) eres      (1000)       69 2024-05-12 06:14:53.000000 data_prep_toolkit-0.0.1.dev1/src/data_processing/test_support/data_access/__init__.py
+-rw-r--r--   0 eres      (1000) eres      (1000)     2666 2024-05-12 06:14:53.000000 data_prep_toolkit-0.0.1.dev1/src/data_processing/test_support/data_access/data_access_factory_test.py
+drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 06:24:42.586930 data_prep_toolkit-0.0.1.dev1/src/data_processing/test_support/ray/
+-rw-r--r--   0 eres      (1000) eres      (1000)       58 2024-05-12 06:16:24.000000 data_prep_toolkit-0.0.1.dev1/src/data_processing/test_support/ray/__init__.py
+-rw-r--r--   0 eres      (1000) eres      (1000)     4672 2024-05-12 06:16:24.000000 data_prep_toolkit-0.0.1.dev1/src/data_processing/test_support/ray/transform_test.py
+drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 06:24:42.586930 data_prep_toolkit-0.0.1.dev1/src/data_processing/test_support/transform/
+-rw-r--r--   0 eres      (1000) eres      (1000)      231 2024-05-12 06:16:24.000000 data_prep_toolkit-0.0.1.dev1/src/data_processing/test_support/transform/__init__.py
+-rw-r--r--   0 eres      (1000) eres      (1000)     5701 2024-05-12 06:16:24.000000 data_prep_toolkit-0.0.1.dev1/src/data_processing/test_support/transform/noop_transform.py
+-rw-r--r--   0 eres      (1000) eres      (1000)     4476 2024-05-12 06:14:53.000000 data_prep_toolkit-0.0.1.dev1/src/data_processing/test_support/transform/transform_test.py
+drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 06:24:42.586930 data_prep_toolkit-0.0.1.dev1/src/data_processing/transform/
+-rw-r--r--   0 eres      (1000) eres      (1000)      368 2024-05-12 06:16:24.000000 data_prep_toolkit-0.0.1.dev1/src/data_processing/transform/__init__.py
+-rw-r--r--   0 eres      (1000) eres      (1000)     3067 2024-05-12 06:16:24.000000 data_prep_toolkit-0.0.1.dev1/src/data_processing/transform/execution_configuration.py
+-rw-r--r--   0 eres      (1000) eres      (1000)     2521 2024-05-12 06:16:24.000000 data_prep_toolkit-0.0.1.dev1/src/data_processing/transform/launcher_configuration.py
+-rw-r--r--   0 eres      (1000) eres      (1000)     2298 2024-05-12 06:14:53.000000 data_prep_toolkit-0.0.1.dev1/src/data_processing/transform/table_transform.py
+-rw-r--r--   0 eres      (1000) eres      (1000)     1465 2024-05-12 06:14:53.000000 data_prep_toolkit-0.0.1.dev1/src/data_processing/transform/transform_statistics.py
+drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 06:24:42.586930 data_prep_toolkit-0.0.1.dev1/src/data_processing/utils/
+-rw-r--r--   0 eres      (1000) eres      (1000)      354 2024-05-12 06:14:53.000000 data_prep_toolkit-0.0.1.dev1/src/data_processing/utils/__init__.py
+-rw-r--r--   0 eres      (1000) eres      (1000)     3135 2024-05-12 06:14:53.000000 data_prep_toolkit-0.0.1.dev1/src/data_processing/utils/cli_utils.py
+-rw-r--r--   0 eres      (1000) eres      (1000)     1695 2024-05-12 06:14:53.000000 data_prep_toolkit-0.0.1.dev1/src/data_processing/utils/config.py
+-rw-r--r--   0 eres      (1000) eres      (1000)     2052 2024-05-12 06:14:53.000000 data_prep_toolkit-0.0.1.dev1/src/data_processing/utils/log.py
+-rw-r--r--   0 eres      (1000) eres      (1000)     6029 2024-05-12 06:14:53.000000 data_prep_toolkit-0.0.1.dev1/src/data_processing/utils/params_utils.py
+-rw-r--r--   0 eres      (1000) eres      (1000)     6740 2024-05-12 06:16:24.000000 data_prep_toolkit-0.0.1.dev1/src/data_processing/utils/transform_utils.py
+drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 06:24:42.576930 data_prep_toolkit-0.0.1.dev1/test/
+drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 06:24:42.576930 data_prep_toolkit-0.0.1.dev1/test/data_processing_tests/
+drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 06:24:42.596930 data_prep_toolkit-0.0.1.dev1/test/data_processing_tests/data_access/
+-rw-r--r--   0 eres      (1000) eres      (1000)     1256 2024-05-12 06:14:53.000000 data_prep_toolkit-0.0.1.dev1/test/data_processing_tests/data_access/daf_local_test.py
+-rw-r--r--   0 eres      (1000) eres      (1000)    24597 2024-05-12 06:14:53.000000 data_prep_toolkit-0.0.1.dev1/test/data_processing_tests/data_access/data_access_local_test.py
+-rw-r--r--   0 eres      (1000) eres      (1000)     5734 2024-05-12 06:14:53.000000 data_prep_toolkit-0.0.1.dev1/test/data_processing_tests/data_access/data_access_s3_test.py
+-rw-r--r--   0 eres      (1000) eres      (1000)     1545 2024-05-12 06:14:53.000000 data_prep_toolkit-0.0.1.dev1/test/data_processing_tests/data_access/sample_input_data_test.py
+drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 06:24:42.596930 data_prep_toolkit-0.0.1.dev1/test/data_processing_tests/pure_python/
+-rw-r--r--   0 eres      (1000) eres      (1000)     9106 2024-05-12 06:16:24.000000 data_prep_toolkit-0.0.1.dev1/test/data_processing_tests/pure_python/launcher_test.py
+drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 06:24:42.596930 data_prep_toolkit-0.0.1.dev1/test/data_processing_tests/ray/
+-rw-r--r--   0 eres      (1000) eres      (1000)    11220 2024-05-12 06:16:24.000000 data_prep_toolkit-0.0.1.dev1/test/data_processing_tests/ray/launcher_test.py
+-rw-r--r--   0 eres      (1000) eres      (1000)     3288 2024-05-12 06:16:24.000000 data_prep_toolkit-0.0.1.dev1/test/data_processing_tests/ray/ray_util_test.py
+-rw-r--r--   0 eres      (1000) eres      (1000)     1733 2024-05-12 06:16:24.000000 data_prep_toolkit-0.0.1.dev1/test/data_processing_tests/ray/test_noop_launch.py
+drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 06:24:42.596930 data_prep_toolkit-0.0.1.dev1/test/data_processing_tests/transform/
+-rw-r--r--   0 eres      (1000) eres      (1000)     1678 2024-05-12 06:14:53.000000 data_prep_toolkit-0.0.1.dev1/test/data_processing_tests/transform/test_noop.py
+drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 06:24:42.596930 data_prep_toolkit-0.0.1.dev1/test/data_processing_tests/util/
+-rw-r--r--   0 eres      (1000) eres      (1000)     1386 2024-05-12 06:14:53.000000 data_prep_toolkit-0.0.1.dev1/test/data_processing_tests/util/transform_utils_test.py
+drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 06:24:42.576930 data_prep_toolkit-0.0.1.dev1/test-data/
+drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 06:24:42.576930 data_prep_toolkit-0.0.1.dev1/test-data/data_processing/
+drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 06:24:42.576930 data_prep_toolkit-0.0.1.dev1/test-data/data_processing/daf/
+drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 06:24:42.576930 data_prep_toolkit-0.0.1.dev1/test-data/data_processing/daf/input/
+drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 06:24:42.586930 data_prep_toolkit-0.0.1.dev1/test-data/data_processing/daf/input/ds1/
+-rw-r--r--   0 eres      (1000) eres      (1000)    36132 2024-05-12 06:14:53.000000 data_prep_toolkit-0.0.1.dev1/test-data/data_processing/daf/input/ds1/sample1.parquet
+-rw-r--r--   0 eres      (1000) eres      (1000)    36132 2024-05-12 06:14:53.000000 data_prep_toolkit-0.0.1.dev1/test-data/data_processing/daf/input/ds1/sample2.parquet
+drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 06:24:42.596930 data_prep_toolkit-0.0.1.dev1/test-data/data_processing/daf/input/ds2/
+-rw-r--r--   0 eres      (1000) eres      (1000)    36132 2024-05-12 06:14:53.000000 data_prep_toolkit-0.0.1.dev1/test-data/data_processing/daf/input/ds2/sample3.parquet
+drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 06:24:42.576930 data_prep_toolkit-0.0.1.dev1/test-data/data_processing/daf/output/
+drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 06:24:42.596930 data_prep_toolkit-0.0.1.dev1/test-data/data_processing/daf/output/ds1/
+-rw-r--r--   0 eres      (1000) eres      (1000)    36132 2024-05-12 06:14:53.000000 data_prep_toolkit-0.0.1.dev1/test-data/data_processing/daf/output/ds1/sample1.parquet
+drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 06:24:42.596930 data_prep_toolkit-0.0.1.dev1/test-data/data_processing/input/
+-rw-r--r--   0 eres      (1000) eres      (1000)    36132 2024-05-12 06:14:53.000000 data_prep_toolkit-0.0.1.dev1/test-data/data_processing/input/sample1.parquet
+drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 06:24:42.596930 data_prep_toolkit-0.0.1.dev1/test-data/data_processing/input_multiple/
+-rw-r--r--   0 eres      (1000) eres      (1000)    36132 2024-05-12 06:14:53.000000 data_prep_toolkit-0.0.1.dev1/test-data/data_processing/input_multiple/sample1.parquet
+-rw-r--r--   0 eres      (1000) eres      (1000)    36132 2024-05-12 06:14:53.000000 data_prep_toolkit-0.0.1.dev1/test-data/data_processing/input_multiple/sample2.parquet
+-rw-r--r--   0 eres      (1000) eres      (1000)    36132 2024-05-12 06:14:53.000000 data_prep_toolkit-0.0.1.dev1/test-data/data_processing/input_multiple/sample3.parquet
+drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 06:24:42.576930 data_prep_toolkit-0.0.1.dev1/test-data/data_processing/ray/
+drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 06:24:42.576930 data_prep_toolkit-0.0.1.dev1/test-data/data_processing/ray/noop/
+drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 06:24:42.596930 data_prep_toolkit-0.0.1.dev1/test-data/data_processing/ray/noop/expected/
+-rw-r--r--   0 eres      (1000) eres      (1000)     1128 2024-05-12 06:14:53.000000 data_prep_toolkit-0.0.1.dev1/test-data/data_processing/ray/noop/expected/metadata.json
+-rw-r--r--   0 eres      (1000) eres      (1000)    36132 2024-05-12 06:14:53.000000 data_prep_toolkit-0.0.1.dev1/test-data/data_processing/ray/noop/expected/sample1.parquet
+drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 06:24:42.596930 data_prep_toolkit-0.0.1.dev1/test-data/data_processing/ray/noop/expected/subdir/
+-rw-r--r--   0 eres      (1000) eres      (1000)      753 2024-05-12 06:14:53.000000 data_prep_toolkit-0.0.1.dev1/test-data/data_processing/ray/noop/expected/subdir/test1.parquet
+drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 06:24:42.596930 data_prep_toolkit-0.0.1.dev1/test-data/data_processing/ray/noop/input/
+-rw-r--r--   0 eres      (1000) eres      (1000)    36132 2024-05-12 06:14:53.000000 data_prep_toolkit-0.0.1.dev1/test-data/data_processing/ray/noop/input/sample1.parquet
+drwxr-xr-x   0 eres      (1000) eres      (1000)        0 2024-05-12 06:24:42.596930 data_prep_toolkit-0.0.1.dev1/test-data/data_processing/ray/noop/input/subdir/
+-rw-r--r--   0 eres      (1000) eres      (1000)      753 2024-05-12 06:14:53.000000 data_prep_toolkit-0.0.1.dev1/test-data/data_processing/ray/noop/input/subdir/test1.parquet
```

### Comparing `data_prep_toolkit-0.0.1/Makefile` & `data_prep_toolkit-0.0.1.dev1/Makefile`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.0.1/PKG-INFO` & `data_prep_toolkit-0.0.1.dev1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: data_prep_toolkit
-Version: 0.0.1
-Summary: Data Preparation Laboratory Library
+Version: 0.0.1.dev1
+Summary: Data Preparation Toolkit Library
 Author-email: David Wood <dawood@us.ibm.com>, Boris Lublinsky <blublinsky@ibm.com>
 License: Apache-2.0
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: ray[default]==2.9.3
 Requires-Dist: pyarrow==15.0.2
 Requires-Dist: boto3==1.34.69
```

### Comparing `data_prep_toolkit-0.0.1/README.md` & `data_prep_toolkit-0.0.1.dev1/README.md`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.0.1/doc/advanced-transform-tutorial.md` & `data_prep_toolkit-0.0.1.dev1/doc/advanced-transform-tutorial.md`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.0.1/doc/architecture.md` & `data_prep_toolkit-0.0.1.dev1/doc/architecture.md`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.0.1/doc/launcher-options.md` & `data_prep_toolkit-0.0.1.dev1/doc/launcher-options.md`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.0.1/doc/logo-ibm-dark.png` & `data_prep_toolkit-0.0.1.dev1/doc/logo-ibm-dark.png`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.0.1/doc/logo-ibm.png` & `data_prep_toolkit-0.0.1.dev1/doc/logo-ibm.png`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.0.1/doc/overview.md` & `data_prep_toolkit-0.0.1.dev1/doc/overview.md`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.0.1/doc/processing-architecture.jpg` & `data_prep_toolkit-0.0.1.dev1/doc/processing-architecture.jpg`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.0.1/doc/simplest-transform-tutorial.md` & `data_prep_toolkit-0.0.1.dev1/doc/simplest-transform-tutorial.md`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.0.1/doc/testing-transforms.md` & `data_prep_toolkit-0.0.1.dev1/doc/testing-transforms.md`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.0.1/doc/transform-external-resources.md` & `data_prep_toolkit-0.0.1.dev1/doc/transform-external-resources.md`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.0.1/doc/transform-tutorials.md` & `data_prep_toolkit-0.0.1.dev1/doc/transform-tutorials.md`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.0.1/doc/transformer-utilities.md` & `data_prep_toolkit-0.0.1.dev1/doc/transformer-utilities.md`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.0.1/doc/using_s3_transformers.md` & `data_prep_toolkit-0.0.1.dev1/doc/using_s3_transformers.md`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.0.1/pyproject.toml` & `data_prep_toolkit-0.0.1.dev1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [project]
 name = "data_prep_toolkit"
-version = "0.0.1"
+version = "0.0.1-dev1"
 requires-python = ">=3.10"
-description = "Data Preparation Laboratory Library"
+description = "Data Preparation Toolkit Library"
 license = {text = "Apache-2.0"}
 readme = {file = "README.md", content-type = "text/markdown"}
 authors = [
     { name = "David Wood", email = "dawood@us.ibm.com" },
     { name = "Boris Lublinsky", email = "blublinsky@ibm.com" },
 ]
 dependencies = [
```

### Comparing `data_prep_toolkit-0.0.1/src/data_prep_toolkit.egg-info/PKG-INFO` & `data_prep_toolkit-0.0.1.dev1/src/data_prep_toolkit.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: data_prep_toolkit
-Version: 0.0.1
-Summary: Data Preparation Laboratory Library
+Version: 0.0.1.dev1
+Summary: Data Preparation Toolkit Library
 Author-email: David Wood <dawood@us.ibm.com>, Boris Lublinsky <blublinsky@ibm.com>
 License: Apache-2.0
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: ray[default]==2.9.3
 Requires-Dist: pyarrow==15.0.2
 Requires-Dist: boto3==1.34.69
```

### Comparing `data_prep_toolkit-0.0.1/src/data_prep_toolkit.egg-info/SOURCES.txt` & `data_prep_toolkit-0.0.1.dev1/src/data_prep_toolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.0.1/src/data_processing/data_access/arrow_s3.py` & `data_prep_toolkit-0.0.1.dev1/src/data_processing/data_access/arrow_s3.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.0.1/src/data_processing/data_access/data_access.py` & `data_prep_toolkit-0.0.1.dev1/src/data_processing/data_access/data_access.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.0.1/src/data_processing/data_access/data_access_factory.py` & `data_prep_toolkit-0.0.1.dev1/src/data_processing/data_access/data_access_factory.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.0.1/src/data_processing/data_access/data_access_factory_base.py` & `data_prep_toolkit-0.0.1.dev1/src/data_processing/data_access/data_access_factory_base.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.0.1/src/data_processing/data_access/data_access_local.py` & `data_prep_toolkit-0.0.1.dev1/src/data_processing/data_access/data_access_local.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.0.1/src/data_processing/data_access/data_access_s3.py` & `data_prep_toolkit-0.0.1.dev1/src/data_processing/data_access/data_access_s3.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.0.1/src/data_processing/pure_python/python_launcher_configuration.py` & `data_prep_toolkit-0.0.1.dev1/src/data_processing/pure_python/python_launcher_configuration.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.0.1/src/data_processing/pure_python/transform_launcher.py` & `data_prep_toolkit-0.0.1.dev1/src/data_processing/pure_python/transform_launcher.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.0.1/src/data_processing/pure_python/transform_orchestrator.py` & `data_prep_toolkit-0.0.1.dev1/src/data_processing/pure_python/transform_orchestrator.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.0.1/src/data_processing/pure_python/transform_table_processor.py` & `data_prep_toolkit-0.0.1.dev1/src/data_processing/pure_python/transform_table_processor.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.0.1/src/data_processing/ray/__init__.py` & `data_prep_toolkit-0.0.1.dev1/src/data_processing/ray/__init__.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.0.1/src/data_processing/ray/ray_utils.py` & `data_prep_toolkit-0.0.1.dev1/src/data_processing/ray/ray_utils.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.0.1/src/data_processing/ray/transform_launcher.py` & `data_prep_toolkit-0.0.1.dev1/src/data_processing/ray/transform_launcher.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,17 +29,17 @@
 
 class RayTransformLauncher:
     """
     Driver class starting Filter execution
     """
 
     def __init__(
-        self,
-        transform_runtime_config: RayLauncherConfiguration,
-        data_access_factory: DataAccessFactoryBase = DataAccessFactory(),
+            self,
+            transform_runtime_config: RayLauncherConfiguration,
+            data_access_factory: DataAccessFactoryBase = DataAccessFactory(),
     ):
         """
         Creates driver
         :param transform_runtime_config: transform runtime factory
         :param data_access_factory: the factory to create DataAccess instances.
         """
         self.name = transform_runtime_config.get_name()
@@ -69,17 +69,17 @@
         args = parser.parse_args()
         self.run_locally = args.run_locally
         if self.run_locally:
             logger.info("Running locally")
         else:
             logger.info("connecting to existing cluster")
         return (
-            self.transform_runtime_config.apply_input_params(args=args)
-            and self.data_access_factory.apply_input_params(args=args)
-            and self.ray_orchestrator.apply_input_params(args=args)
+                self.transform_runtime_config.apply_input_params(args=args)
+                and self.data_access_factory.apply_input_params(args=args)
+                and self.ray_orchestrator.apply_input_params(args=args)
         )
 
     def _submit_for_execution(self) -> int:
         """
         Submit for Ray execution
         :return:
         """
@@ -110,16 +110,18 @@
             logger.info(f"Completed execution in {(time.time() - start)/60.} min, execution result {res}")
             ray.shutdown()
             return res
 
     def launch(self) -> int:
         """
         Execute method orchestrates driver invocation
-        :return:
+        :return: launch result
         """
+        print("testing execution")
         if self.__get_parameters():
-            return self._submit_for_execution()
-        if self.run_locally:
-            return 1
+            res = self._submit_for_execution()
         else:
+            res = 1
+        if not self.run_locally and res > 0:
             # if we are running in kfp exit to signal kfp that we failed
             sys.exit(1)
+        return res
```

### Comparing `data_prep_toolkit-0.0.1/src/data_processing/ray/transform_orchestrator.py` & `data_prep_toolkit-0.0.1.dev1/src/data_processing/ray/transform_orchestrator.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.0.1/src/data_processing/ray/transform_orchestrator_configuration.py` & `data_prep_toolkit-0.0.1.dev1/src/data_processing/ray/transform_orchestrator_configuration.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.0.1/src/data_processing/ray/transform_runtime.py` & `data_prep_toolkit-0.0.1.dev1/src/data_processing/ray/transform_runtime.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.0.1/src/data_processing/ray/transform_statistics.py` & `data_prep_toolkit-0.0.1.dev1/src/data_processing/ray/transform_statistics.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.0.1/src/data_processing/ray/transform_table_processor.py` & `data_prep_toolkit-0.0.1.dev1/src/data_processing/ray/transform_table_processor.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.0.1/src/data_processing/test_support/abstract_test.py` & `data_prep_toolkit-0.0.1.dev1/src/data_processing/test_support/abstract_test.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.0.1/src/data_processing/test_support/data_access/data_access_factory_test.py` & `data_prep_toolkit-0.0.1.dev1/src/data_processing/test_support/data_access/data_access_factory_test.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.0.1/src/data_processing/test_support/ray/transform_test.py` & `data_prep_toolkit-0.0.1.dev1/src/data_processing/test_support/ray/transform_test.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.0.1/src/data_processing/test_support/transform/noop_transform.py` & `data_prep_toolkit-0.0.1.dev1/src/data_processing/test_support/transform/noop_transform.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.0.1/src/data_processing/test_support/transform/transform_test.py` & `data_prep_toolkit-0.0.1.dev1/src/data_processing/test_support/transform/transform_test.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.0.1/src/data_processing/transform/execution_configuration.py` & `data_prep_toolkit-0.0.1.dev1/src/data_processing/transform/execution_configuration.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.0.1/src/data_processing/transform/launcher_configuration.py` & `data_prep_toolkit-0.0.1.dev1/src/data_processing/transform/launcher_configuration.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.0.1/src/data_processing/transform/table_transform.py` & `data_prep_toolkit-0.0.1.dev1/src/data_processing/transform/table_transform.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.0.1/src/data_processing/transform/transform_statistics.py` & `data_prep_toolkit-0.0.1.dev1/src/data_processing/transform/transform_statistics.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.0.1/src/data_processing/utils/cli_utils.py` & `data_prep_toolkit-0.0.1.dev1/src/data_processing/utils/cli_utils.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.0.1/src/data_processing/utils/config.py` & `data_prep_toolkit-0.0.1.dev1/src/data_processing/utils/config.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.0.1/src/data_processing/utils/log.py` & `data_prep_toolkit-0.0.1.dev1/src/data_processing/utils/log.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.0.1/src/data_processing/utils/params_utils.py` & `data_prep_toolkit-0.0.1.dev1/src/data_processing/utils/params_utils.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.0.1/src/data_processing/utils/transform_utils.py` & `data_prep_toolkit-0.0.1.dev1/src/data_processing/utils/transform_utils.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.0.1/test/data_processing_tests/data_access/daf_local_test.py` & `data_prep_toolkit-0.0.1.dev1/test/data_processing_tests/data_access/daf_local_test.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.0.1/test/data_processing_tests/data_access/data_access_local_test.py` & `data_prep_toolkit-0.0.1.dev1/test/data_processing_tests/data_access/data_access_local_test.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.0.1/test/data_processing_tests/data_access/data_access_s3_test.py` & `data_prep_toolkit-0.0.1.dev1/test/data_processing_tests/data_access/data_access_s3_test.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.0.1/test/data_processing_tests/data_access/sample_input_data_test.py` & `data_prep_toolkit-0.0.1.dev1/test/data_processing_tests/data_access/sample_input_data_test.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.0.1/test/data_processing_tests/pure_python/launcher_test.py` & `data_prep_toolkit-0.0.1.dev1/test/data_processing_tests/pure_python/launcher_test.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.0.1/test/data_processing_tests/ray/launcher_test.py` & `data_prep_toolkit-0.0.1.dev1/test/data_processing_tests/ray/launcher_test.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.0.1/test/data_processing_tests/ray/ray_util_test.py` & `data_prep_toolkit-0.0.1.dev1/test/data_processing_tests/ray/ray_util_test.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.0.1/test/data_processing_tests/ray/test_noop_launch.py` & `data_prep_toolkit-0.0.1.dev1/test/data_processing_tests/ray/test_noop_launch.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.0.1/test/data_processing_tests/transform/test_noop.py` & `data_prep_toolkit-0.0.1.dev1/test/data_processing_tests/transform/test_noop.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.0.1/test/data_processing_tests/util/transform_utils_test.py` & `data_prep_toolkit-0.0.1.dev1/test/data_processing_tests/util/transform_utils_test.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.0.1/test-data/data_processing/daf/input/ds1/sample1.parquet` & `data_prep_toolkit-0.0.1.dev1/test-data/data_processing/daf/input/ds1/sample1.parquet`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.0.1/test-data/data_processing/daf/input/ds1/sample2.parquet` & `data_prep_toolkit-0.0.1.dev1/test-data/data_processing/daf/input/ds1/sample2.parquet`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.0.1/test-data/data_processing/daf/input/ds2/sample3.parquet` & `data_prep_toolkit-0.0.1.dev1/test-data/data_processing/daf/input/ds2/sample3.parquet`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.0.1/test-data/data_processing/daf/output/ds1/sample1.parquet` & `data_prep_toolkit-0.0.1.dev1/test-data/data_processing/daf/output/ds1/sample1.parquet`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.0.1/test-data/data_processing/input/sample1.parquet` & `data_prep_toolkit-0.0.1.dev1/test-data/data_processing/input/sample1.parquet`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.0.1/test-data/data_processing/input_multiple/sample1.parquet` & `data_prep_toolkit-0.0.1.dev1/test-data/data_processing/input_multiple/sample1.parquet`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.0.1/test-data/data_processing/input_multiple/sample2.parquet` & `data_prep_toolkit-0.0.1.dev1/test-data/data_processing/input_multiple/sample2.parquet`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.0.1/test-data/data_processing/input_multiple/sample3.parquet` & `data_prep_toolkit-0.0.1.dev1/test-data/data_processing/input_multiple/sample3.parquet`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.0.1/test-data/data_processing/ray/noop/expected/metadata.json` & `data_prep_toolkit-0.0.1.dev1/test-data/data_processing/ray/noop/expected/metadata.json`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.0.1/test-data/data_processing/ray/noop/expected/sample1.parquet` & `data_prep_toolkit-0.0.1.dev1/test-data/data_processing/ray/noop/expected/sample1.parquet`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.0.1/test-data/data_processing/ray/noop/expected/subdir/test1.parquet` & `data_prep_toolkit-0.0.1.dev1/test-data/data_processing/ray/noop/expected/subdir/test1.parquet`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.0.1/test-data/data_processing/ray/noop/input/sample1.parquet` & `data_prep_toolkit-0.0.1.dev1/test-data/data_processing/ray/noop/input/sample1.parquet`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit-0.0.1/test-data/data_processing/ray/noop/input/subdir/test1.parquet` & `data_prep_toolkit-0.0.1.dev1/test-data/data_processing/ray/noop/input/subdir/test1.parquet`

 * *Files identical despite different names*

