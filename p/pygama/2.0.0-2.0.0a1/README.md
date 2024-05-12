# Comparing `tmp/pygama-2.0.0.tar.gz` & `tmp/pygama-2.0.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygama-2.0.0.tar", last modified: Sun May 12 12:09:51 2024, max compression
+gzip compressed data, was "pygama-2.0.0a1.tar", last modified: Sat Apr 27 18:10:36 2024, max compression
```

## Comparing `pygama-2.0.0.tar` & `pygama-2.0.0a1.tar`

### file list

```diff
@@ -1,163 +1,170 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 12:09:51.053273 pygama-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-12 12:09:45.000000 pygama-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4853 2024-05-12 12:09:51.049273 pygama-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2706 2024-05-12 12:09:45.000000 pygama-2.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-05-12 12:09:45.000000 pygama-2.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 12:09:51.053273 pygama-2.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 12:09:51.021273 pygama-2.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 12:09:51.025272 pygama-2.0.0/src/pygama/
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-12 12:09:45.000000 pygama-2.0.0/src/pygama/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-12 12:09:50.000000 pygama-2.0.0/src/pygama/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    12126 2024-05-12 12:09:45.000000 pygama-2.0.0/src/pygama/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 12:09:51.029273 pygama-2.0.0/src/pygama/evt/
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-12 12:09:45.000000 pygama-2.0.0/src/pygama/evt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16382 2024-05-12 12:09:45.000000 pygama-2.0.0/src/pygama/evt/aggregators.py
--rw-r--r--   0 runner    (1001) docker     (127)    21054 2024-05-12 12:09:45.000000 pygama-2.0.0/src/pygama/evt/build_evt.py
--rw-r--r--   0 runner    (1001) docker     (127)     3411 2024-05-12 12:09:45.000000 pygama-2.0.0/src/pygama/evt/build_tcm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 12:09:51.029273 pygama-2.0.0/src/pygama/evt/modules/
--rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-05-12 12:09:45.000000 pygama-2.0.0/src/pygama/evt/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7313 2024-05-12 12:09:45.000000 pygama-2.0.0/src/pygama/evt/modules/geds.py
--rw-r--r--   0 runner    (1001) docker     (127)     7064 2024-05-12 12:09:45.000000 pygama-2.0.0/src/pygama/evt/modules/larveto.py
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-05-12 12:09:45.000000 pygama-2.0.0/src/pygama/evt/modules/legend.py
--rw-r--r--   0 runner    (1001) docker     (127)    11654 2024-05-12 12:09:45.000000 pygama-2.0.0/src/pygama/evt/modules/spms.py
--rw-r--r--   0 runner    (1001) docker     (127)    11664 2024-05-12 12:09:45.000000 pygama-2.0.0/src/pygama/evt/modules/xtalk.py
--rw-r--r--   0 runner    (1001) docker     (127)     4836 2024-05-12 12:09:45.000000 pygama-2.0.0/src/pygama/evt/tcm.py
--rw-r--r--   0 runner    (1001) docker     (127)     7577 2024-05-12 12:09:45.000000 pygama-2.0.0/src/pygama/evt/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 12:09:51.029273 pygama-2.0.0/src/pygama/flow/
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-12 12:09:45.000000 pygama-2.0.0/src/pygama/flow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    62482 2024-05-12 12:09:45.000000 pygama-2.0.0/src/pygama/flow/data_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)    27426 2024-05-12 12:09:45.000000 pygama-2.0.0/src/pygama/flow/file_db.py
--rw-r--r--   0 runner    (1001) docker     (127)     6026 2024-05-12 12:09:45.000000 pygama-2.0.0/src/pygama/flow/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 12:09:51.029273 pygama-2.0.0/src/pygama/hit/
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-12 12:09:45.000000 pygama-2.0.0/src/pygama/hit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10325 2024-05-12 12:09:45.000000 pygama-2.0.0/src/pygama/hit/build_hit.py
--rw-r--r--   0 runner    (1001) docker     (127)      966 2024-05-12 12:09:45.000000 pygama-2.0.0/src/pygama/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 12:09:51.033273 pygama-2.0.0/src/pygama/math/
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-12 12:09:45.000000 pygama-2.0.0/src/pygama/math/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13992 2024-05-12 12:09:45.000000 pygama-2.0.0/src/pygama/math/binned_fitting.py
--rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-05-12 12:09:45.000000 pygama-2.0.0/src/pygama/math/distributions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 12:09:51.037273 pygama-2.0.0/src/pygama/math/functions/
--rw-r--r--   0 runner    (1001) docker     (127)     3198 2024-05-12 12:09:45.000000 pygama-2.0.0/src/pygama/math/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8427 2024-05-12 12:09:45.000000 pygama-2.0.0/src/pygama/math/functions/crystal_ball.py
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-05-12 12:09:45.000000 pygama-2.0.0/src/pygama/math/functions/error_function.py
--rw-r--r--   0 runner    (1001) docker     (127)     8813 2024-05-12 12:09:45.000000 pygama-2.0.0/src/pygama/math/functions/exgauss.py
--rw-r--r--   0 runner    (1001) docker     (127)     5743 2024-05-12 12:09:45.000000 pygama-2.0.0/src/pygama/math/functions/exponential.py
--rw-r--r--   0 runner    (1001) docker     (127)     5845 2024-05-12 12:09:45.000000 pygama-2.0.0/src/pygama/math/functions/gauss.py
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-12 12:09:45.000000 pygama-2.0.0/src/pygama/math/functions/gauss_on_exgauss.py
--rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-05-12 12:09:45.000000 pygama-2.0.0/src/pygama/math/functions/gauss_on_exponential.py
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-12 12:09:45.000000 pygama-2.0.0/src/pygama/math/functions/gauss_on_linear.py
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-05-12 12:09:45.000000 pygama-2.0.0/src/pygama/math/functions/gauss_on_step.py
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-05-12 12:09:45.000000 pygama-2.0.0/src/pygama/math/functions/gauss_on_uniform.py
--rw-r--r--   0 runner    (1001) docker     (127)     6941 2024-05-12 12:09:45.000000 pygama-2.0.0/src/pygama/math/functions/hpge_peak.py
--rw-r--r--   0 runner    (1001) docker     (127)     5960 2024-05-12 12:09:45.000000 pygama-2.0.0/src/pygama/math/functions/linear.py
--rw-r--r--   0 runner    (1001) docker     (127)     4747 2024-05-12 12:09:45.000000 pygama-2.0.0/src/pygama/math/functions/moyal.py
--rw-r--r--   0 runner    (1001) docker     (127)     4438 2024-05-12 12:09:45.000000 pygama-2.0.0/src/pygama/math/functions/poisson.py
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-12 12:09:45.000000 pygama-2.0.0/src/pygama/math/functions/polynomial.py
--rw-r--r--   0 runner    (1001) docker     (127)     6206 2024-05-12 12:09:45.000000 pygama-2.0.0/src/pygama/math/functions/pygama_continuous.py
--rw-r--r--   0 runner    (1001) docker     (127)    10727 2024-05-12 12:09:45.000000 pygama-2.0.0/src/pygama/math/functions/step.py
--rw-r--r--   0 runner    (1001) docker     (127)    30820 2024-05-12 12:09:45.000000 pygama-2.0.0/src/pygama/math/functions/sum_dists.py
--rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-05-12 12:09:45.000000 pygama-2.0.0/src/pygama/math/functions/triple_gauss_on_double_step.py
--rw-r--r--   0 runner    (1001) docker     (127)     4789 2024-05-12 12:09:45.000000 pygama-2.0.0/src/pygama/math/functions/uniform.py
--rw-r--r--   0 runner    (1001) docker     (127)    26563 2024-05-12 12:09:45.000000 pygama-2.0.0/src/pygama/math/histogram.py
--rw-r--r--   0 runner    (1001) docker     (127)     9877 2024-05-12 12:09:45.000000 pygama-2.0.0/src/pygama/math/hpge_peak_fitting.py
--rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-05-12 12:09:45.000000 pygama-2.0.0/src/pygama/math/least_squares.py
--rw-r--r--   0 runner    (1001) docker     (127)     2169 2024-05-12 12:09:45.000000 pygama-2.0.0/src/pygama/math/unbinned_fitting.py
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-12 12:09:45.000000 pygama-2.0.0/src/pygama/math/units.py
--rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-05-12 12:09:45.000000 pygama-2.0.0/src/pygama/math/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 12:09:51.037273 pygama-2.0.0/src/pygama/pargen/
--rw-r--r--   0 runner    (1001) docker     (127)    84558 2024-05-12 12:09:45.000000 pygama-2.0.0/src/pygama/pargen/AoE_cal.py
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-12 12:09:45.000000 pygama-2.0.0/src/pygama/pargen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    35158 2024-05-12 12:09:45.000000 pygama-2.0.0/src/pygama/pargen/data_cleaning.py
--rw-r--r--   0 runner    (1001) docker     (127)    18349 2024-05-12 12:09:45.000000 pygama-2.0.0/src/pygama/pargen/dplms_ge_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)    29751 2024-05-12 12:09:45.000000 pygama-2.0.0/src/pygama/pargen/dsp_optimize.py
--rw-r--r--   0 runner    (1001) docker     (127)    95527 2024-05-12 12:09:45.000000 pygama-2.0.0/src/pygama/pargen/energy_cal.py
--rw-r--r--   0 runner    (1001) docker     (127)    17554 2024-05-12 12:09:45.000000 pygama-2.0.0/src/pygama/pargen/energy_optimisation.py
--rw-r--r--   0 runner    (1001) docker     (127)     7283 2024-05-12 12:09:45.000000 pygama-2.0.0/src/pygama/pargen/extract_tau.py
--rw-r--r--   0 runner    (1001) docker     (127)    33312 2024-05-12 12:09:45.000000 pygama-2.0.0/src/pygama/pargen/lq_cal.py
--rw-r--r--   0 runner    (1001) docker     (127)    11949 2024-05-12 12:09:45.000000 pygama-2.0.0/src/pygama/pargen/noise_optimization.py
--rw-r--r--   0 runner    (1001) docker     (127)     4387 2024-05-12 12:09:45.000000 pygama-2.0.0/src/pygama/pargen/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3201 2024-05-12 12:09:45.000000 pygama-2.0.0/src/pygama/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 12:09:51.049273 pygama-2.0.0/src/pygama.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4853 2024-05-12 12:09:50.000000 pygama-2.0.0/src/pygama.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4720 2024-05-12 12:09:51.000000 pygama-2.0.0/src/pygama.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 12:09:50.000000 pygama-2.0.0/src/pygama.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-12 12:09:50.000000 pygama-2.0.0/src/pygama.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 12:09:50.000000 pygama-2.0.0/src/pygama.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-12 12:09:50.000000 pygama-2.0.0/src/pygama.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-12 12:09:50.000000 pygama-2.0.0/src/pygama.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 12:09:51.037273 pygama-2.0.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 12:09:51.037273 pygama-2.0.0/tests/configs/
--rw-r--r--   0 runner    (1001) docker     (127)    10209 2024-05-12 12:09:45.000000 pygama-2.0.0/tests/configs/icpc-dsp-config.json
--rw-r--r--   0 runner    (1001) docker     (127)     4539 2024-05-12 12:09:45.000000 pygama-2.0.0/tests/configs/sipm-dplms-config.json
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-05-12 12:09:45.000000 pygama-2.0.0/tests/configs/sipm-dsp-config.json
--rw-r--r--   0 runner    (1001) docker     (127)     2407 2024-05-12 12:09:45.000000 pygama-2.0.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 12:09:51.041273 pygama-2.0.0/tests/evt/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 12:09:51.041273 pygama-2.0.0/tests/evt/configs/
--rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-05-12 12:09:45.000000 pygama-2.0.0/tests/evt/configs/basic-evt-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-05-12 12:09:45.000000 pygama-2.0.0/tests/evt/configs/query-test-evt-config.json
--rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-05-12 12:09:45.000000 pygama-2.0.0/tests/evt/configs/spms-module-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-05-12 12:09:45.000000 pygama-2.0.0/tests/evt/configs/vov-test-evt-config.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 12:09:51.041273 pygama-2.0.0/tests/evt/modules/
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-12 12:09:45.000000 pygama-2.0.0/tests/evt/modules/larveto.py
--rw-r--r--   0 runner    (1001) docker     (127)     9867 2024-05-12 12:09:45.000000 pygama-2.0.0/tests/evt/test_build_evt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-05-12 12:09:45.000000 pygama-2.0.0/tests/evt/test_build_tcm.py
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-12 12:09:45.000000 pygama-2.0.0/tests/evt/test_evt_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 12:09:45.000000 pygama-2.0.0/tests/evt/test_geds.py
--rw-r--r--   0 runner    (1001) docker     (127)     2903 2024-05-12 12:09:45.000000 pygama-2.0.0/tests/evt/test_xtalk.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 12:09:51.041273 pygama-2.0.0/tests/flow/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 12:09:51.041273 pygama-2.0.0/tests/flow/configs/
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-12 12:09:45.000000 pygama-2.0.0/tests/flow/configs/config.json
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-12 12:09:45.000000 pygama-2.0.0/tests/flow/configs/data-loader-config.json
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-12 12:09:45.000000 pygama-2.0.0/tests/flow/configs/filedb-config.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 12:09:51.041273 pygama-2.0.0/tests/flow/configs/nested/
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-12 12:09:45.000000 pygama-2.0.0/tests/flow/configs/nested/config.json
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-12 12:09:45.000000 pygama-2.0.0/tests/flow/configs/nested/data-loader-config-nested.json
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-05-12 12:09:45.000000 pygama-2.0.0/tests/flow/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5027 2024-05-12 12:09:45.000000 pygama-2.0.0/tests/flow/test_data_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)    10171 2024-05-12 12:09:45.000000 pygama-2.0.0/tests/flow/test_filedb.py
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-12 12:09:45.000000 pygama-2.0.0/tests/flow/test_flow_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 12:09:51.041273 pygama-2.0.0/tests/hit/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 12:09:51.045273 pygama-2.0.0/tests/hit/configs/
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-12 12:09:45.000000 pygama-2.0.0/tests/hit/configs/aggregations-hit-config.json
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-05-12 12:09:45.000000 pygama-2.0.0/tests/hit/configs/basic-hit-config.json
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-12 12:09:45.000000 pygama-2.0.0/tests/hit/configs/spms-hit-a-config.json
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-12 12:09:45.000000 pygama-2.0.0/tests/hit/configs/spms-hit-config.json
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-12 12:09:45.000000 pygama-2.0.0/tests/hit/configs/spms-hit-multi-config.json
--rw-r--r--   0 runner    (1001) docker     (127)     7733 2024-05-12 12:09:45.000000 pygama-2.0.0/tests/hit/test_build_hit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 12:09:51.045273 pygama-2.0.0/tests/math/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 12:09:51.049273 pygama-2.0.0/tests/math/functions/
--rw-r--r--   0 runner    (1001) docker     (127)     2194 2024-05-12 12:09:45.000000 pygama-2.0.0/tests/math/functions/test_crystal_ball.py
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-12 12:09:45.000000 pygama-2.0.0/tests/math/functions/test_error_function.py
--rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-05-12 12:09:45.000000 pygama-2.0.0/tests/math/functions/test_exgauss.py
--rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-05-12 12:09:45.000000 pygama-2.0.0/tests/math/functions/test_exponential.py
--rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-05-12 12:09:45.000000 pygama-2.0.0/tests/math/functions/test_gauss.py
--rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-05-12 12:09:45.000000 pygama-2.0.0/tests/math/functions/test_gauss_on_exgauss.py
--rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-05-12 12:09:45.000000 pygama-2.0.0/tests/math/functions/test_gauss_on_exponential.py
--rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-05-12 12:09:45.000000 pygama-2.0.0/tests/math/functions/test_gauss_on_linear.py
--rw-r--r--   0 runner    (1001) docker     (127)     3922 2024-05-12 12:09:45.000000 pygama-2.0.0/tests/math/functions/test_gauss_on_step.py
--rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-05-12 12:09:45.000000 pygama-2.0.0/tests/math/functions/test_gauss_on_uniform.py
--rw-r--r--   0 runner    (1001) docker     (127)     3585 2024-05-12 12:09:45.000000 pygama-2.0.0/tests/math/functions/test_hpge_peak.py
--rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-05-12 12:09:45.000000 pygama-2.0.0/tests/math/functions/test_linear.py
--rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-05-12 12:09:45.000000 pygama-2.0.0/tests/math/functions/test_moyal.py
--rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-05-12 12:09:45.000000 pygama-2.0.0/tests/math/functions/test_numba_frozen.py
--rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-05-12 12:09:45.000000 pygama-2.0.0/tests/math/functions/test_poisson.py
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-12 12:09:45.000000 pygama-2.0.0/tests/math/functions/test_polynomial.py
--rw-r--r--   0 runner    (1001) docker     (127)     3488 2024-05-12 12:09:45.000000 pygama-2.0.0/tests/math/functions/test_step.py
--rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-05-12 12:09:45.000000 pygama-2.0.0/tests/math/functions/test_sum_dists.py
--rw-r--r--   0 runner    (1001) docker     (127)     4622 2024-05-12 12:09:45.000000 pygama-2.0.0/tests/math/functions/test_triple_gauss_on_double_step.py
--rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-05-12 12:09:45.000000 pygama-2.0.0/tests/math/functions/test_uniform.py
--rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-05-12 12:09:45.000000 pygama-2.0.0/tests/math/test_binned_fitting.py
--rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-05-12 12:09:45.000000 pygama-2.0.0/tests/math/test_distribution_selector_in_sum_dists.py
--rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-05-12 12:09:45.000000 pygama-2.0.0/tests/math/test_hpge_peak_fitting.py
--rw-r--r--   0 runner    (1001) docker     (127)     2909 2024-05-12 12:09:45.000000 pygama-2.0.0/tests/math/test_iminuit_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-12 12:09:45.000000 pygama-2.0.0/tests/math/test_least_squares.py
--rw-r--r--   0 runner    (1001) docker     (127)     5336 2024-05-12 12:09:45.000000 pygama-2.0.0/tests/math/test_math_histogram.py
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-12 12:09:45.000000 pygama-2.0.0/tests/math/test_math_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-12 12:09:45.000000 pygama-2.0.0/tests/math/test_unbinned_fitting.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 12:09:51.049273 pygama-2.0.0/tests/pargen/
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-12 12:09:45.000000 pygama-2.0.0/tests/pargen/test_aoecal.py
--rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-05-12 12:09:45.000000 pygama-2.0.0/tests/pargen/test_datacleaning.py
--rw-r--r--   0 runner    (1001) docker     (127)     4801 2024-05-12 12:09:45.000000 pygama-2.0.0/tests/pargen/test_ecal.py
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-12 12:09:45.000000 pygama-2.0.0/tests/pargen/test_energy_optimization.py
--rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-05-12 12:09:45.000000 pygama-2.0.0/tests/pargen/test_lqcal.py
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-12 12:09:45.000000 pygama-2.0.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:10:36.795232 pygama-2.0.0a1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-27 18:10:33.000000 pygama-2.0.0a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4822 2024-04-27 18:10:36.795232 pygama-2.0.0a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2706 2024-04-27 18:10:33.000000 pygama-2.0.0a1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2721 2024-04-27 18:10:33.000000 pygama-2.0.0a1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 18:10:36.795232 pygama-2.0.0a1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:10:36.767232 pygama-2.0.0a1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:10:36.771232 pygama-2.0.0a1/src/pygama/
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-27 18:10:36.000000 pygama-2.0.0a1/src/pygama/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12126 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:10:36.771232 pygama-2.0.0a1/src/pygama/dsp/
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/dsp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:10:36.771232 pygama-2.0.0a1/src/pygama/dsp/processors/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/dsp/processors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:10:36.775231 pygama-2.0.0a1/src/pygama/evt/
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/evt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15979 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/evt/aggregators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20976 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/evt/build_evt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3411 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/evt/build_tcm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:10:36.775231 pygama-2.0.0a1/src/pygama/evt/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/evt/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1998 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/evt/modules/geds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4742 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/evt/modules/larveto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/evt/modules/legend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12600 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/evt/modules/spms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4836 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/evt/tcm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7577 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/evt/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:10:36.775231 pygama-2.0.0a1/src/pygama/flow/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/flow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62482 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/flow/data_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27426 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/flow/file_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6026 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/flow/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:10:36.775231 pygama-2.0.0a1/src/pygama/hit/
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/hit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8998 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/hit/build_hit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:10:36.775231 pygama-2.0.0a1/src/pygama/lgdo/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/lgdo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:10:36.775231 pygama-2.0.0a1/src/pygama/math/
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/math/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13992 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/math/binned_fitting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/math/distributions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:10:36.779232 pygama-2.0.0a1/src/pygama/math/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)     3198 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/math/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8427 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/math/functions/crystal_ball.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/math/functions/error_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8813 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/math/functions/exgauss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5743 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/math/functions/exponential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5845 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/math/functions/gauss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/math/functions/gauss_on_exgauss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/math/functions/gauss_on_exponential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/math/functions/gauss_on_linear.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/math/functions/gauss_on_step.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/math/functions/gauss_on_uniform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6941 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/math/functions/hpge_peak.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5960 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/math/functions/linear.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4747 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/math/functions/moyal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4438 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/math/functions/poisson.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/math/functions/polynomial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6206 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/math/functions/pygama_continuous.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10727 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/math/functions/step.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30820 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/math/functions/sum_dists.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/math/functions/triple_gauss_on_double_step.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4789 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/math/functions/uniform.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26563 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/math/histogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9877 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/math/hpge_peak_fitting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/math/least_squares.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/math/unbinned_fitting.py
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/math/units.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/math/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:10:36.783232 pygama-2.0.0a1/src/pygama/pargen/
+-rw-r--r--   0 runner    (1001) docker     (127)    84627 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/pargen/AoE_cal.py
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/pargen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35158 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/pargen/data_cleaning.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18349 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/pargen/dplms_ge_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29751 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/pargen/dsp_optimize.py
+-rw-r--r--   0 runner    (1001) docker     (127)    95343 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/pargen/energy_cal.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17554 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/pargen/energy_optimisation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7283 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/pargen/extract_tau.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32272 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/pargen/lq_cal.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11949 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/pargen/noise_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4387 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/pargen/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:10:36.783232 pygama-2.0.0a1/src/pygama/raw/
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/raw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3201 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:10:36.783232 pygama-2.0.0a1/src/pygama/vis/
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-27 18:10:33.000000 pygama-2.0.0a1/src/pygama/vis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:10:36.791232 pygama-2.0.0a1/src/pygama.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4822 2024-04-27 18:10:36.000000 pygama-2.0.0a1/src/pygama.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4788 2024-04-27 18:10:36.000000 pygama-2.0.0a1/src/pygama.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 18:10:36.000000 pygama-2.0.0a1/src/pygama.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-27 18:10:36.000000 pygama-2.0.0a1/src/pygama.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 18:10:36.000000 pygama-2.0.0a1/src/pygama.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-27 18:10:36.000000 pygama-2.0.0a1/src/pygama.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-27 18:10:36.000000 pygama-2.0.0a1/src/pygama.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:10:36.783232 pygama-2.0.0a1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:10:36.783232 pygama-2.0.0a1/tests/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)    10209 2024-04-27 18:10:33.000000 pygama-2.0.0a1/tests/configs/icpc-dsp-config.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4539 2024-04-27 18:10:33.000000 pygama-2.0.0a1/tests/configs/sipm-dplms-config.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-04-27 18:10:33.000000 pygama-2.0.0a1/tests/configs/sipm-dsp-config.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2407 2024-04-27 18:10:33.000000 pygama-2.0.0a1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:10:36.783232 pygama-2.0.0a1/tests/evt/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:10:36.783232 pygama-2.0.0a1/tests/evt/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-04-27 18:10:33.000000 pygama-2.0.0a1/tests/evt/configs/basic-evt-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-04-27 18:10:33.000000 pygama-2.0.0a1/tests/evt/configs/query-test-evt-config.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-04-27 18:10:33.000000 pygama-2.0.0a1/tests/evt/configs/spms-module-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-04-27 18:10:33.000000 pygama-2.0.0a1/tests/evt/configs/vov-test-evt-config.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:10:36.783232 pygama-2.0.0a1/tests/evt/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-27 18:10:33.000000 pygama-2.0.0a1/tests/evt/modules/larveto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9727 2024-04-27 18:10:33.000000 pygama-2.0.0a1/tests/evt/test_build_evt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-04-27 18:10:33.000000 pygama-2.0.0a1/tests/evt/test_build_tcm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-27 18:10:33.000000 pygama-2.0.0a1/tests/evt/test_evt_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:10:36.787232 pygama-2.0.0a1/tests/flow/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:10:36.787232 pygama-2.0.0a1/tests/flow/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-27 18:10:33.000000 pygama-2.0.0a1/tests/flow/configs/config.json
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-27 18:10:33.000000 pygama-2.0.0a1/tests/flow/configs/data-loader-config.json
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-27 18:10:33.000000 pygama-2.0.0a1/tests/flow/configs/filedb-config.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:10:36.787232 pygama-2.0.0a1/tests/flow/configs/nested/
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-27 18:10:33.000000 pygama-2.0.0a1/tests/flow/configs/nested/config.json
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-27 18:10:33.000000 pygama-2.0.0a1/tests/flow/configs/nested/data-loader-config-nested.json
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-04-27 18:10:33.000000 pygama-2.0.0a1/tests/flow/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5027 2024-04-27 18:10:33.000000 pygama-2.0.0a1/tests/flow/test_data_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10171 2024-04-27 18:10:33.000000 pygama-2.0.0a1/tests/flow/test_filedb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-27 18:10:33.000000 pygama-2.0.0a1/tests/flow/test_flow_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:10:36.787232 pygama-2.0.0a1/tests/hit/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:10:36.787232 pygama-2.0.0a1/tests/hit/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-27 18:10:33.000000 pygama-2.0.0a1/tests/hit/configs/aggregations-hit-config.json
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-27 18:10:33.000000 pygama-2.0.0a1/tests/hit/configs/basic-hit-config.json
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-27 18:10:33.000000 pygama-2.0.0a1/tests/hit/configs/spms-hit-a-config.json
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-27 18:10:33.000000 pygama-2.0.0a1/tests/hit/configs/spms-hit-config.json
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-27 18:10:33.000000 pygama-2.0.0a1/tests/hit/configs/spms-hit-multi-config.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7733 2024-04-27 18:10:33.000000 pygama-2.0.0a1/tests/hit/test_build_hit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:10:36.787232 pygama-2.0.0a1/tests/math/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:10:36.791232 pygama-2.0.0a1/tests/math/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)     2194 2024-04-27 18:10:33.000000 pygama-2.0.0a1/tests/math/functions/test_crystal_ball.py
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-27 18:10:33.000000 pygama-2.0.0a1/tests/math/functions/test_error_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-04-27 18:10:33.000000 pygama-2.0.0a1/tests/math/functions/test_exgauss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-04-27 18:10:33.000000 pygama-2.0.0a1/tests/math/functions/test_exponential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-04-27 18:10:33.000000 pygama-2.0.0a1/tests/math/functions/test_gauss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-04-27 18:10:33.000000 pygama-2.0.0a1/tests/math/functions/test_gauss_on_exgauss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-04-27 18:10:33.000000 pygama-2.0.0a1/tests/math/functions/test_gauss_on_exponential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-04-27 18:10:33.000000 pygama-2.0.0a1/tests/math/functions/test_gauss_on_linear.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3922 2024-04-27 18:10:33.000000 pygama-2.0.0a1/tests/math/functions/test_gauss_on_step.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-04-27 18:10:33.000000 pygama-2.0.0a1/tests/math/functions/test_gauss_on_uniform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3585 2024-04-27 18:10:33.000000 pygama-2.0.0a1/tests/math/functions/test_hpge_peak.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-04-27 18:10:33.000000 pygama-2.0.0a1/tests/math/functions/test_linear.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-04-27 18:10:33.000000 pygama-2.0.0a1/tests/math/functions/test_moyal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-04-27 18:10:33.000000 pygama-2.0.0a1/tests/math/functions/test_numba_frozen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-04-27 18:10:33.000000 pygama-2.0.0a1/tests/math/functions/test_poisson.py
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-27 18:10:33.000000 pygama-2.0.0a1/tests/math/functions/test_polynomial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3488 2024-04-27 18:10:33.000000 pygama-2.0.0a1/tests/math/functions/test_step.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-04-27 18:10:33.000000 pygama-2.0.0a1/tests/math/functions/test_sum_dists.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4622 2024-04-27 18:10:33.000000 pygama-2.0.0a1/tests/math/functions/test_triple_gauss_on_double_step.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-04-27 18:10:33.000000 pygama-2.0.0a1/tests/math/functions/test_uniform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-04-27 18:10:33.000000 pygama-2.0.0a1/tests/math/test_binned_fitting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-04-27 18:10:33.000000 pygama-2.0.0a1/tests/math/test_distribution_selector_in_sum_dists.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-04-27 18:10:33.000000 pygama-2.0.0a1/tests/math/test_hpge_peak_fitting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2909 2024-04-27 18:10:33.000000 pygama-2.0.0a1/tests/math/test_iminuit_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-27 18:10:33.000000 pygama-2.0.0a1/tests/math/test_least_squares.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5336 2024-04-27 18:10:33.000000 pygama-2.0.0a1/tests/math/test_math_histogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-27 18:10:33.000000 pygama-2.0.0a1/tests/math/test_math_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-27 18:10:33.000000 pygama-2.0.0a1/tests/math/test_unbinned_fitting.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:10:36.791232 pygama-2.0.0a1/tests/pargen/
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-27 18:10:33.000000 pygama-2.0.0a1/tests/pargen/test_aoecal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-04-27 18:10:33.000000 pygama-2.0.0a1/tests/pargen/test_datacleaning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4801 2024-04-27 18:10:33.000000 pygama-2.0.0a1/tests/pargen/test_ecal.py
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-27 18:10:33.000000 pygama-2.0.0a1/tests/pargen/test_energy_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-04-27 18:10:33.000000 pygama-2.0.0a1/tests/pargen/test_lqcal.py
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-27 18:10:33.000000 pygama-2.0.0a1/tests/test_utils.py
```

### Comparing `pygama-2.0.0/LICENSE` & `pygama-2.0.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `pygama-2.0.0/PKG-INFO` & `pygama-2.0.0a1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygama
-Version: 2.0.0
+Version: 2.0.0a1
 Summary: Python package for data processing and analysis
 Author: The LEGEND collaboration
 Maintainer: The LEGEND collaboration
 Project-URL: Homepage, https://github.com/legend-exp/pygama
 Project-URL: Bug Tracker, https://github.com/legend-exp/pygama/issues
 Project-URL: Discussions, https://github.com/legend-exp/pygama/discussions
 Project-URL: Changelog, https://github.com/legend-exp/pygama/releases
@@ -24,16 +24,15 @@
 License-File: LICENSE
 Requires-Dist: hist
 Requires-Dist: colorlog
 Requires-Dist: dspeed>=1.3
 Requires-Dist: h5py>=3.2
 Requires-Dist: iminuit
 Requires-Dist: legend-daq2lh5>=1.2.1
-Requires-Dist: legend-pydataobj>=1.7
-Requires-Dist: pylegendmeta>=0.9
+Requires-Dist: legend-pydataobj>=1.6
 Requires-Dist: matplotlib
 Requires-Dist: numba!=0.53.*,!=0.54.*,!=0.57
 Requires-Dist: numpy>=1.21
 Requires-Dist: pandas>=1.4.4
 Requires-Dist: pint
 Requires-Dist: pyyaml
 Requires-Dist: scikit-learn
```

### Comparing `pygama-2.0.0/README.md` & `pygama-2.0.0a1/README.md`

 * *Files identical despite different names*

### Comparing `pygama-2.0.0/pyproject.toml` & `pygama-2.0.0a1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -32,16 +32,15 @@
 dependencies = [
     "hist",
     "colorlog",
     "dspeed>=1.3",
     "h5py>=3.2",
     "iminuit",
     "legend-daq2lh5>=1.2.1",
-    "legend-pydataobj>=1.7",
-    "pylegendmeta>=0.9",
+    "legend-pydataobj>=1.6",
     "matplotlib",
     "numba!=0.53.*,!=0.54.*,!=0.57",
     "numpy>=1.21",
     "pandas>=1.4.4",
     "pint",
     "pyyaml",
     "scikit-learn",
```

### Comparing `pygama-2.0.0/src/pygama/cli.py` & `pygama-2.0.0a1/src/pygama/cli.py`

 * *Files identical despite different names*

### Comparing `pygama-2.0.0/src/pygama/evt/aggregators.py` & `pygama-2.0.0a1/src/pygama/evt/aggregators.py`

 * *Files 12% similar despite different names*

```diff
@@ -234,15 +234,14 @@
 
     return types.Array(nda=out)
 
 
 def evaluate_at_channel(
     datainfo,
     tcm,
-    channels,
     channels_skip,
     expr,
     field_list,
     ch_comp,
     pars_dict=None,
     default_value=np.nan,
 ) -> types.Array:
@@ -250,16 +249,14 @@
 
     Parameters
     ----------
     datainfo
         input and output LH5 datainfo with HDF5 groups where tables are found.
     tcm
         TCM data arrays in an object that can be accessed by attribute.
-    channels
-        list of channels to be included for evaluation.
     channels_skip
        list of channels to be skipped from evaluation and set to default value.
     expr
        expression string to be evaluated.
     field_list
        list of `dsp/hit/evt` parameter tuples in expression ``(tier, field)``.
     ch_comp
@@ -280,15 +277,15 @@
         if table_name not in lh5.ls(f.hit.file):
             continue
 
         idx_ch = tcm.idx[tcm.id == ch]
         evt_ids_ch = np.searchsorted(
             tcm.cumulative_length, np.where(tcm.id == ch)[0], "right"
         )
-        if (table_name in channels) and (table_name not in channels_skip):
+        if table_name not in channels_skip:
             res = utils.get_data_at_channel(
                 datainfo=datainfo,
                 ch=table_name,
                 tcm=tcm,
                 expr=expr,
                 field_list=field_list,
                 pars_dict=pars_dict,
@@ -306,15 +303,14 @@
 
 def evaluate_at_channel_vov(
     datainfo,
     tcm,
     expr,
     field_list,
     ch_comp,
-    channels,
     channels_skip,
     pars_dict=None,
     default_value=np.nan,
 ) -> types.VectorOfVectors:
     """Same as :func:`evaluate_at_channel` but evaluates expression at non
     flat channels :class:`.VectorOfVectors`.
 
@@ -326,67 +322,62 @@
         TCM data arrays in an object that can be accessed by attribute.
     expr
        expression string to be evaluated.
     field_list
        list of `dsp/hit/evt` parameter tuples in expression ``(tier, field)``.
     ch_comp
        array of "rawid"s at which the expression is evaluated.
-    channels
-       list of channels to be included for evaluation.
     channels_skip
        list of channels to be skipped from evaluation and set to default value.
     pars_dict
        dictionary of `evt` and additional parameters and their values.
     default_value
        default value.
     """
     f = utils.make_files_config(datainfo)
 
-    ch_comp_channels = np.unique(ch_comp.flattened_data.nda).astype(int)
+    # blow up vov to aoesa
+    out = ak.Array([[] for _ in range(len(ch_comp))])
 
-    out = np.full(
-        len(ch_comp.flattened_data.nda), default_value, dtype=type(default_value)
-    )
+    channels = np.unique(ch_comp.flattened_data.nda).astype(int)
+    ch_comp = ch_comp.view_as("ak")
 
     type_name = None
-    for ch in ch_comp_channels:
+    for ch in channels:
         table_name = utils.get_table_name_by_pattern(f.hit.table_fmt, ch)
+
         evt_ids_ch = np.searchsorted(
             tcm.cumulative_length, np.where(tcm.id == ch)[0], "right"
         )
-        if (table_name in channels) and (table_name not in channels_skip):
+        if table_name not in channels_skip:
             res = utils.get_data_at_channel(
                 datainfo=datainfo,
                 ch=table_name,
                 tcm=tcm,
                 expr=expr,
                 field_list=field_list,
                 pars_dict=pars_dict,
             )
-            new_evt_ids_ch = np.searchsorted(
-                ch_comp.cumulative_length,
-                np.where(ch_comp.flattened_data.nda == ch)[0],
-                "right",
-            )
-            matches = np.isin(evt_ids_ch, new_evt_ids_ch)
-            out[ch_comp.flattened_data.nda == ch] = res[matches]
-
         else:
-            length = len(np.where(ch_comp.flattened_data.nda == ch)[0])
-            res = np.full(length, default_value)
-            out[ch_comp.flattened_data.nda == ch] = res
+            idx_ch = tcm.idx[tcm.id == ch]
+            res = np.full(len(idx_ch), default_value)
+
+        # see in which events the current channel is present
+        mask = ak.to_numpy(ak.any(ch_comp == ch, axis=-1), allow_missing=False)
+        cv = np.full(len(ch_comp), np.nan)
+        cv[evt_ids_ch] = res
+        cv[~mask] = np.nan
+        cv = ak.drop_none(ak.nan_to_none(ak.Array(cv)[:, None]))
+
+        out = ak.concatenate((out, cv), axis=-1)
 
-        if ch == ch_comp_channels[0]:
-            out = out.astype(res.dtype)
+        if ch == channels[0]:
             type_name = res.dtype
 
-    return types.VectorOfVectors(
-        flattened_data=types.Array(out, dtype=type_name),
-        cumulative_length=ch_comp.cumulative_length,
-    )
+    return types.VectorOfVectors(ak.values_astype(out, type_name))
 
 
 def evaluate_to_aoesa(
     datainfo,
     tcm,
     channels,
     channels_skip,
```

### Comparing `pygama-2.0.0/src/pygama/evt/build_evt.py` & `pygama-2.0.0a1/src/pygama/evt/build_evt.py`

 * *Files 1% similar despite different names*

```diff
@@ -493,15 +493,14 @@
                         + " not supported (only Array and VectorOfVectors are supported)"
                     )
 
             if isinstance(ch_comp, Array):
                 return aggregators.evaluate_at_channel(
                     datainfo=datainfo,
                     tcm=tcm,
-                    channels=channels,
                     channels_skip=channels_skip,
                     expr=expr,
                     field_list=field_list,
                     ch_comp=ch_comp,
                     pars_dict=pars_dict,
                     default_value=default_value,
                 )
@@ -509,15 +508,14 @@
             if isinstance(ch_comp, VectorOfVectors):
                 return aggregators.evaluate_at_channel_vov(
                     datainfo=datainfo,
                     tcm=tcm,
                     expr=expr,
                     field_list=field_list,
                     ch_comp=ch_comp,
-                    channels=channels,
                     channels_skip=channels_skip,
                     pars_dict=pars_dict,
                     default_value=default_value,
                 )
 
             raise NotImplementedError(
                 "{type(ch_comp).__name__} not supported "
```

### Comparing `pygama-2.0.0/src/pygama/evt/build_tcm.py` & `pygama-2.0.0a1/src/pygama/evt/build_tcm.py`

 * *Files identical despite different names*

### Comparing `pygama-2.0.0/src/pygama/evt/modules/__init__.py` & `pygama-2.0.0a1/src/pygama/evt/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `pygama-2.0.0/src/pygama/evt/modules/larveto.py` & `pygama-2.0.0a1/src/pygama/evt/modules/larveto.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,21 @@
 """Routines to evaluate the correlation between HPGe and SiPM signals."""
 
 from __future__ import annotations
 
-from collections.abc import Sequence
-
 import awkward as ak
 import numpy as np
-import scipy.stats
+import scipy
 from numpy.typing import ArrayLike
 
 
 def l200_combined_test_stat(
     t0: ak.Array,
     amp: ak.Array,
     geds_t0: ak.Array,
-    ts_bkg_prob: float,
-    rc_density: Sequence[float],
 ) -> ak.Array:
     """Combined L200 LAr veto classifier.
 
     Where combined means taking channel-specific parameters into account.
 
     `t0` and `amp` must be in the format of a 3-dimensional Awkward array,
     where the innermost dimension labels the SiPM pulse, the second one labels
@@ -29,79 +25,47 @@
     ----------
     t0
         arrival times of pulses in ns, split by channel.
     amp
         amplitude of pulses in p.e., split by channel.
     geds_t0
         t0 (ns) of the HPGe signal.
-    ts_bkg_prob
-        probability for a pulse coming from some uncorrelated physics (uniform
-        distribution). needed for the LAr scintillation time pdf.
-    rc_density
-        density array of the random coincidence LAr energy distribution (total
-        energy summed over all channels, in p.e.). Derived from forced trigger
-        data.
     """
     # flatten the data in the last axis (i.e. merge all channels together)
     # TODO: implement channel distinction
     t0 = ak.flatten(t0, axis=-1)
     amp = ak.flatten(amp, axis=-1)
 
     # subtract the HPGe t0 from the SiPM pulse t0s
-    rel_t0 = t0 - geds_t0
+    # HACK: remove 16 when units will be fixed
+    rel_t0 = 16 * t0 - geds_t0
 
-    return l200_test_stat(rel_t0, amp, ts_bkg_prob, rc_density)
+    return l200_test_stat(rel_t0, amp)
 
 
-def l200_test_stat(relative_t0, amp, ts_bkg_prob, rc_density):
+def l200_test_stat(relative_t0, amp):
     """Compute the test statistics.
 
     Parameters
     ----------
     relative_t0
         t0 (ns) of the SiPM pulses relative to the HPGe t0.
     amp
         amplitude in p.e. of the SiPM pulses.
     """
-    # convert to integer number of pes
-    n_pes = pulse_amp_round(amp)
-
-    # compute total number of pes in event
-    n_pe_tot = np.sum(n_pes, axis=-1)
-    # if no pes in the event, use nan instead of zero (because of division later)
-    n_pe_tot = np.where(n_pe_tot == 0, np.nan, n_pe_tot)
-
-    # calculate the test statistic term related to the time distribution
-    ts_time = -ak.sum(
-        ak.transform(
-            lambda layouts, **kwargs: _ak_l200_test_stat_time_term(
-                layouts, ts_bkg_prob, **kwargs
-            ),
-            relative_t0,
-            amp,
-        ),
-        axis=-1,
-    )
-    # calculate the amplitude contribution
-    ts_amp = [l200_rc_amp_logpdf(n, rc_density) for n in n_pe_tot]
-
-    # for events with no light, set the test statistic value to +inf
-    t_stat = np.where(np.isnan(n_pe_tot), np.inf, ts_time / n_pe_tot + ts_amp)
-
-    return t_stat
+    return -ak.sum(ak.transform(_ak_l200_test_stat_terms, relative_t0, amp), axis=-1)
 
 
 # need to define this function and use it with ak.transform() because scipy
 # routines are not NumPy universal functions
-def _ak_l200_test_stat_time_term(layouts, ts_bkg_prob, **kwargs):
+def _ak_l200_test_stat_terms(layouts, **kwargs):
     """Awkward transform to compute the per-pulse terms of the test statistics.
 
-    The two arguments are the pulse times `t0` relative to the HPGe trigger and
-    their amplitude `amp`. The function has to be invoked as
-    ``ak.transform(_ak_l200_test_stat_terms, t0, amp,
+    The two arguments are the pulse times `t0` and their amplitude `amp`. The
+    function has to be invoked as ``ak.transform(_ak_l200_test_stat_terms, t0, amp,
     ...)``.
     """
     # sanity check
     assert len(layouts) == 2
 
     if not all([lay.is_numpy for lay in layouts]):
         return
@@ -109,117 +73,88 @@
     # these are the two supported arguments
     t0 = layouts[0].data
     amp = layouts[1].data
 
     # sanity check
     assert len(t0) == len(amp)
 
+    # if there are no pulses return NaN
+    if len(t0) == 0 or any(np.isnan(t0)):
+        return ak.contents.NumpyArray([np.nan])
+
     # convert to integer number of pes
     n_pes = pulse_amp_round(amp)
+    n_pe_tot = np.sum(n_pes)
 
-    # calculate the time term of the test statistic
-    ts_time = n_pes * np.log(l200_tc_time_pdf(t0, bkg_prob=ts_bkg_prob))
+    t_stat = n_pes * np.log(l200_tc_time_pdf(t0)) / n_pe_tot + np.log(
+        l200_rc_amp_pdf(n_pe_tot)
+    )
 
-    return ak.contents.NumpyArray(ts_time)
+    return ak.contents.NumpyArray(t_stat)
 
 
 def pulse_amp_round(amp: float | ArrayLike):
     """Get the most likely (integer) number of photo-electrons."""
-    # promote all amps < 1 to 1. standard rounding to nearest for amps > 1
+    # promote all amps < 1 to 1. standard rounding to nearest for
+    # amps > 1
     return ak.where(amp < 1, np.ceil(amp), np.floor(amp + 0.5))
 
 
 def l200_tc_time_pdf(
     t0: float | ArrayLike,
     *,
     domain_ns: tuple[float] = (-1_000, 5_000),
     tau_singlet_ns: float = 6,
     tau_triplet_ns: float = 1100,
-    sing2tot_ratio: float = 1 / 3,
+    sing2trip_ratio: float = 1 / 3,
     t0_res_ns: float = 35,
     t0_bias_ns: float = -80,
     bkg_prob: float = 0.42,
 ) -> float | ArrayLike:
     """The L200 experimental LAr scintillation pdf
 
     The theoretical scintillation pdf convoluted with a Normal distribution
     (experimental effects) and summed to a uniform distribution (uncorrelated
     pulses).
 
-    This routine does not work with :class:`ak.Array`, since SciPy functions
-    are not universal. See :func:`_ak_l200_test_stat_time_term` for an example
-    Awkward transform that does the job.
-
     Parameters
     ----------
     t0
         arrival times of the SiPM pulses in ns.
     tau_singlet_ns
         The lifetime of the LAr singlet state in ns.
     tau_triplet_ns
         The lifetime of the LAr triplet state in ns.
-    sing2tot_ratio
-        The singlet-to-total excitation probability ratio.
+    sing2trip_ratio
+        The singlet-to-triplet excitation probability ratio.
     t0_res_ns
         sigma (ns) of the normal distribution.
     t0_bias_ns
         mean (ns) of the normal distribution.
     bkg_prob
         probability for a pulse coming from some uncorrelated physics (uniform
         distribution).
     """
-    if np.any(t0 > domain_ns[1]) or np.any(t0 < domain_ns[0]):
+    if not np.all(t0 <= domain_ns[1] and t0 >= domain_ns[0]):
         msg = f"{t0=} out of bounds for {domain_ns=}"
         raise ValueError(msg)
 
+    # TODO: make this a true pdf, i.e. normalize to integral 1
     return (
         # the triplet
-        (1 - bkg_prob)
-        * (
-            (1 - sing2tot_ratio)
-            * scipy.stats.exponnorm.pdf(
-                t0, tau_triplet_ns / t0_res_ns, loc=t0_bias_ns, scale=t0_res_ns
-            )
-            # the singlet
-            + sing2tot_ratio
-            * scipy.stats.exponnorm.pdf(
-                t0, tau_singlet_ns / t0_res_ns, loc=t0_bias_ns, scale=t0_res_ns
-            )
+        (1 - sing2trip_ratio)
+        * scipy.stats.exponnorm.pdf(
+            t0, tau_triplet_ns / t0_res_ns, loc=t0_bias_ns, scale=t0_res_ns
+        )
+        # the singlet
+        + sing2trip_ratio
+        * scipy.stats.exponnorm.pdf(
+            t0, tau_singlet_ns / t0_res_ns, loc=t0_bias_ns, scale=t0_res_ns
         )
         # the random coincidences (uniform pdf)
         + bkg_prob
         * scipy.stats.uniform.pdf(t0, domain_ns[0], domain_ns[1] - domain_ns[0])
     )
 
 
-def l200_rc_amp_logpdf(
-    n_pes,
-    rc_density=None,
-    logexp_cont_slope=-1 / 10,
-):
-    """The L200 experimental random coincidence (RC) amplitude pdf
-
-    Parameters
-    ----------
-    n_pes
-        number of photoelectrons.
-    rc_density
-        density array of the random coincidence LAr energy distribution (total
-        energy summed over all channels, in p.e.). Derived from forced trigger
-        data.
-    logexp_cont_slope
-        slope for exponential analytical continuation.
-
-    """
-    # analytical continuation must be decaying exponential function.
-    assert logexp_cont_slope < 0
-
-    if rc_density is None:
-        rc_density = [1]
-
-    # up to 15 p.e., take the experimental values from the density.
-    limit = min(len(rc_density) - 1, 15)
-    if n_pes <= limit:
-        return np.log(rc_density[int(n_pes)])
-    # analytical continuation: log of an exponential function.
-    else:
-        return logexp_cont_slope * (n_pes - int(limit)) + np.log(rc_density[int(limit)])
+def l200_rc_amp_pdf(n):
+    return np.exp(-n)
```

### Comparing `pygama-2.0.0/src/pygama/evt/modules/legend.py` & `pygama-2.0.0a1/src/pygama/evt/modules/legend.py`

 * *Files identical despite different names*

### Comparing `pygama-2.0.0/src/pygama/evt/modules/spms.py` & `pygama-2.0.0a1/src/pygama/evt/modules/spms.py`

 * *Files 11% similar despite different names*

```diff
@@ -250,14 +250,21 @@
         datainfo,
         tcm,
         table_names,
         observable="hit.trigger_pos",
         drop_empty=False,
     )
 
+    # HACK: handle units
+    # HACK: remove me once units are fixed in the dsp tier
+    if "units" in pulse_t0.attrs and pulse_t0.attrs["units"] == "ns":
+        pulse_t0_ns = pulse_t0.view_as("ak")
+    else:
+        pulse_t0_ns = pulse_t0.view_as("ak") * 16
+
     pulse_amp = gather_pulse_data(
         datainfo,
         tcm,
         table_names,
         observable="hit.energy_in_pe",
         drop_empty=False,
     ).view_as("ak")
@@ -272,15 +279,14 @@
             raise ValueError(msg)
 
         # NOTE: the assumption is that t0 is np.nan when missing -> replace
         # with default value
         t_loc_ns = ak.fill_none(ak.nan_to_none(t_loc_ns), t_loc_default_ns)
 
     # start with all-true mask
-    pulse_t0_ns = pulse_t0.view_as("ak")
     mask = pulse_t0_ns == pulse_t0_ns
 
     # apply p.e. threshold
     if a_thr_pe is not None:
         mask = mask & (pulse_amp > a_thr_pe)
 
     # apply time windowing
@@ -298,45 +304,78 @@
 
 
 def geds_coincidence_classifier(
     datainfo: utils.DataInfo,
     tcm: utils.TCMData,
     table_names: Sequence[str],
     *,
-    spms_t0: types.VectorOfVectors,
-    spms_amp: types.VectorOfVectors,
     geds_t0_ns: types.Array,
-    ts_bkg_prob: float,
-    rc_density: Sequence[float] | None = None,
 ) -> types.Array:
     """Calculate the HPGe / SiPMs coincidence classifier.
 
     The value represents the likelihood of a physical correlation between HPGe
     and SiPM signals.
 
     Parameters
     ----------
     datainfo, tcm, table_names
         positional arguments automatically supplied by :func:`.build_evt`.
-    t0
-        arrival times of pulses in ns, split by channel.
-    amp
-        amplitude of pulses in p.e., split by channel.
-    geds_t0_ns
-        t0 (ns) of the HPGe signal.
-    ts_bkg_prob
-        probability for a pulse coming from some uncorrelated physics (uniform
-        distribution). needed for the LAr scintillation time pdf.
-    rc_density
-        density array of the random coincidence LAr energy distribution (total
-        energy summed over all channels, in p.e.). Derived from forced trigger
-        data.
     """
-    return types.Array(
-        larveto.l200_combined_test_stat(
-            spms_t0.view_as("ak"),
-            spms_amp.view_as("ak"),
-            geds_t0_ns.view_as("ak"),
-            ts_bkg_prob,
-            rc_density,
-        )
+    # mask for windowing data around the HPGe t0
+    pulse_mask = make_pulse_data_mask(
+        datainfo,
+        tcm,
+        table_names,
+        a_thr_pe=None,
+        t_loc_ns=geds_t0_ns,
+        dt_range_ns=(-1_000, 5_000),
+        t_loc_default_ns=48_000,
+    )
+
+    # load the data
+    data = {}
+    for k, obs in {"amp": "hit.energy_in_pe", "t0": "hit.trigger_pos"}.items():
+        data[k] = gather_pulse_data(
+            datainfo,
+            tcm,
+            table_names,
+            observable=obs,
+            pulse_mask=pulse_mask,
+            drop_empty=True,
+        ).view_as("ak")
+
+    # load the channel info
+    # rawids = spms.gather_tcm_id_data(
+    #     datainfo,
+    #     tcm,
+    #     table_names,
+    #     pulse_mask=pulse_mask,
+    #     drop_empty=True,
+    # )
+
+    # (HPGe) trigger position can vary among events!
+    if isinstance(geds_t0_ns, types.Array):
+        geds_t0_ns = geds_t0_ns.view_as("ak")
+
+    ts_data = larveto.l200_combined_test_stat(data["t0"], data["amp"], geds_t0_ns)
+
+    return types.Array(ts_data)
+
+
+# REMOVE ME: not needed anymore with VectorOfVectors DSP outputs
+def gather_is_valid_hit(datainfo, tcm, table_names):
+    data = {}
+    for field in ("is_valid_hit", "trigger_pos"):
+        data[field] = gather_pulse_data(
+            datainfo,
+            tcm,
+            table_names,
+            observable=f"hit.{field}",
+            pulse_mask=None,
+            drop_empty=False,
+        ).view_as("ak")
+
+    return types.VectorOfVectors(
+        data["is_valid_hit"][
+            ak.local_index(data["is_valid_hit"]) < ak.num(data["trigger_pos"], axis=-1)
+        ]
     )
```

### Comparing `pygama-2.0.0/src/pygama/evt/tcm.py` & `pygama-2.0.0a1/src/pygama/evt/tcm.py`

 * *Files identical despite different names*

### Comparing `pygama-2.0.0/src/pygama/evt/utils.py` & `pygama-2.0.0a1/src/pygama/evt/utils.py`

 * *Files identical despite different names*

### Comparing `pygama-2.0.0/src/pygama/flow/data_loader.py` & `pygama-2.0.0a1/src/pygama/flow/data_loader.py`

 * *Files identical despite different names*

### Comparing `pygama-2.0.0/src/pygama/flow/file_db.py` & `pygama-2.0.0a1/src/pygama/flow/file_db.py`

 * *Files identical despite different names*

### Comparing `pygama-2.0.0/src/pygama/flow/utils.py` & `pygama-2.0.0a1/src/pygama/flow/utils.py`

 * *Files identical despite different names*

### Comparing `pygama-2.0.0/src/pygama/hit/build_hit.py` & `pygama-2.0.0a1/src/pygama/hit/build_hit.py`

 * *Files 12% similar despite different names*

```diff
@@ -255,49 +255,7 @@
     while True:
         new = _one_pass(current)
 
         if new == current:
             return new
         else:
             current = new
-
-
-def _get_dependencies(config, par, pars=None):
-    """
-    Recursive func to iterate back through tree of input blocks for a given output block
-    """
-    if pars is None:
-        pars = []
-    par_op = config[par]
-    c = compile(par_op["expression"], "gcc -O3 -ffast-math build_hit.py", "eval")
-    for p in c.co_names:
-        if p in par_op["parameters"]:
-            pass
-        else:
-            pars.append(p)
-            if p in config:
-                pars = _get_dependencies(config, p, pars)
-    return pars
-
-
-def _remove_uneeded_operations(config, outpars):
-    """
-    Function that removes any operations not needed to generate outpars from the config dictionary
-    Returns the config without these blocks as well as a list of input keys from the dsp file
-    needed to generate outpars
-    """
-    if not isinstance(outpars, list):
-        outpars = [outpars]
-    dependent_keys = [*outpars]
-    inkeys = []
-    for par in outpars:
-        pars = _get_dependencies(config, par)
-        for p in pars:
-            if p in config and p not in dependent_keys:
-                dependent_keys.append(p)
-            elif p not in config and p not in inkeys:
-                inkeys.append(p)
-
-    for key in list(config):
-        if key not in dependent_keys:
-            config.pop(key)
-    return config, inkeys
```

### Comparing `pygama-2.0.0/src/pygama/logging.py` & `pygama-2.0.0a1/src/pygama/logging.py`

 * *Files identical despite different names*

### Comparing `pygama-2.0.0/src/pygama/math/binned_fitting.py` & `pygama-2.0.0a1/src/pygama/math/binned_fitting.py`

 * *Files identical despite different names*

### Comparing `pygama-2.0.0/src/pygama/math/distributions.py` & `pygama-2.0.0a1/src/pygama/math/distributions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 r"""
 Contains a list of distribution functions, all implemented using Numba's
 :func:`numba.jit` to take advantage of the just-in-time speed boost.
 """
 
 # nopycln: file
 
-from pygama.math.functions.crystal_ball import crystal_ball  # noqa: F401
 from pygama.math.functions.crystal_ball import (  # noqa: F401
+    crystal_ball,
     nb_crystal_ball_cdf,
     nb_crystal_ball_pdf,
 )
 from pygama.math.functions.error_function import nb_erf, nb_erfc  # noqa: F401
-from pygama.math.functions.exgauss import exgauss  # noqa: F401
 from pygama.math.functions.exgauss import (  # noqa: F401
+    exgauss,
     nb_exgauss_cdf,
     nb_exgauss_pdf,
     nb_gauss_tail_approx,
 )
 from pygama.math.functions.exponential import exponential  # noqa: F401
 from pygama.math.functions.gauss import (  # noqa: F401
     gaussian,
```

### Comparing `pygama-2.0.0/src/pygama/math/functions/__init__.py` & `pygama-2.0.0a1/src/pygama/math/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `pygama-2.0.0/src/pygama/math/functions/crystal_ball.py` & `pygama-2.0.0a1/src/pygama/math/functions/crystal_ball.py`

 * *Files identical despite different names*

### Comparing `pygama-2.0.0/src/pygama/math/functions/error_function.py` & `pygama-2.0.0a1/src/pygama/math/functions/error_function.py`

 * *Files identical despite different names*

### Comparing `pygama-2.0.0/src/pygama/math/functions/exgauss.py` & `pygama-2.0.0a1/src/pygama/math/functions/exgauss.py`

 * *Files identical despite different names*

### Comparing `pygama-2.0.0/src/pygama/math/functions/exponential.py` & `pygama-2.0.0a1/src/pygama/math/functions/exponential.py`

 * *Files identical despite different names*

### Comparing `pygama-2.0.0/src/pygama/math/functions/gauss.py` & `pygama-2.0.0a1/src/pygama/math/functions/gauss.py`

 * *Files identical despite different names*

### Comparing `pygama-2.0.0/src/pygama/math/functions/gauss_on_exgauss.py` & `pygama-2.0.0a1/src/pygama/math/functions/gauss_on_exgauss.py`

 * *Files identical despite different names*

### Comparing `pygama-2.0.0/src/pygama/math/functions/gauss_on_exponential.py` & `pygama-2.0.0a1/src/pygama/math/functions/gauss_on_exponential.py`

 * *Files identical despite different names*

### Comparing `pygama-2.0.0/src/pygama/math/functions/gauss_on_linear.py` & `pygama-2.0.0a1/src/pygama/math/functions/gauss_on_linear.py`

 * *Files identical despite different names*

### Comparing `pygama-2.0.0/src/pygama/math/functions/gauss_on_step.py` & `pygama-2.0.0a1/src/pygama/math/functions/gauss_on_step.py`

 * *Files identical despite different names*

### Comparing `pygama-2.0.0/src/pygama/math/functions/gauss_on_uniform.py` & `pygama-2.0.0a1/src/pygama/math/functions/gauss_on_uniform.py`

 * *Files identical despite different names*

### Comparing `pygama-2.0.0/src/pygama/math/functions/hpge_peak.py` & `pygama-2.0.0a1/src/pygama/math/functions/hpge_peak.py`

 * *Files identical despite different names*

### Comparing `pygama-2.0.0/src/pygama/math/functions/linear.py` & `pygama-2.0.0a1/src/pygama/math/functions/linear.py`

 * *Files identical despite different names*

### Comparing `pygama-2.0.0/src/pygama/math/functions/moyal.py` & `pygama-2.0.0a1/src/pygama/math/functions/moyal.py`

 * *Files identical despite different names*

### Comparing `pygama-2.0.0/src/pygama/math/functions/poisson.py` & `pygama-2.0.0a1/src/pygama/math/functions/poisson.py`

 * *Files identical despite different names*

### Comparing `pygama-2.0.0/src/pygama/math/functions/polynomial.py` & `pygama-2.0.0a1/src/pygama/math/functions/polynomial.py`

 * *Files identical despite different names*

### Comparing `pygama-2.0.0/src/pygama/math/functions/pygama_continuous.py` & `pygama-2.0.0a1/src/pygama/math/functions/pygama_continuous.py`

 * *Files identical despite different names*

### Comparing `pygama-2.0.0/src/pygama/math/functions/step.py` & `pygama-2.0.0a1/src/pygama/math/functions/step.py`

 * *Files identical despite different names*

### Comparing `pygama-2.0.0/src/pygama/math/functions/sum_dists.py` & `pygama-2.0.0a1/src/pygama/math/functions/sum_dists.py`

 * *Files identical despite different names*

### Comparing `pygama-2.0.0/src/pygama/math/functions/triple_gauss_on_double_step.py` & `pygama-2.0.0a1/src/pygama/math/functions/triple_gauss_on_double_step.py`

 * *Files identical despite different names*

### Comparing `pygama-2.0.0/src/pygama/math/functions/uniform.py` & `pygama-2.0.0a1/src/pygama/math/functions/uniform.py`

 * *Files identical despite different names*

### Comparing `pygama-2.0.0/src/pygama/math/histogram.py` & `pygama-2.0.0a1/src/pygama/math/histogram.py`

 * *Files identical despite different names*

### Comparing `pygama-2.0.0/src/pygama/math/hpge_peak_fitting.py` & `pygama-2.0.0a1/src/pygama/math/hpge_peak_fitting.py`

 * *Files identical despite different names*

### Comparing `pygama-2.0.0/src/pygama/math/least_squares.py` & `pygama-2.0.0a1/src/pygama/math/least_squares.py`

 * *Files identical despite different names*

### Comparing `pygama-2.0.0/src/pygama/math/unbinned_fitting.py` & `pygama-2.0.0a1/src/pygama/math/unbinned_fitting.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,15 +62,15 @@
             cost_func = cost.UnbinnedNLL(data, func)
     if isinstance(guess, dict):
         m = Minuit(cost_func, **guess)
     else:
         m = Minuit(cost_func, *guess)
     if bounds is not None:
         if isinstance(bounds, dict):
-            for arg, key in bounds.items():
+            for arg, key in bounds:
                 m.limits[arg] = key
         else:
             m.limits = bounds
     if fixed is not None:
         for fix in fixed:
             m.fixed[fix] = True
     if simplex is True:
```

### Comparing `pygama-2.0.0/src/pygama/math/utils.py` & `pygama-2.0.0a1/src/pygama/math/utils.py`

 * *Files identical despite different names*

### Comparing `pygama-2.0.0/src/pygama/pargen/AoE_cal.py` & `pygama-2.0.0a1/src/pygama/pargen/AoE_cal.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,14 @@
     exgauss,
     gauss_on_exgauss,
     gauss_on_step,
     gaussian,
     hpge_peak,
     nb_erfc,
 )
-from pygama.math.functions.gauss import nb_gauss_amp
 from pygama.math.functions.hpge_peak import hpge_get_fwfm, hpge_get_fwhm, hpge_get_mode
 from pygama.math.functions.sum_dists import SumDists
 from pygama.pargen.utils import convert_to_minuit, return_nans
 
 log = logging.getLogger(__name__)
 
 (x_lo, x_hi, n_sig, mu, sigma, n_bkg, tau) = range(7)
@@ -874,17 +873,15 @@
                 if tstamp in update_dict:
                     self.cal_dicts[tstamp].update(update_dict[tstamp])
                 else:
                     self.cal_dicts[tstamp].update(update_dict)
         else:
             self.cal_dicts.update(update_dict)
 
-    def time_correction(
-        self, df, aoe_param, mode="full", output_name="AoE_Timecorr", display=0
-    ):
+    def time_correction(self, df, aoe_param, output_name="AoE_Timecorr", display=0):
         log.info("Starting A/E time correction")
         self.timecorr_df = pd.DataFrame()
         try:
             if "run_timestamp" in df:
                 for tstamp, time_df in df.groupby("run_timestamp", sort=True):
                     try:
                         pars, errs, cov = unbinned_aoe_fit(
@@ -937,32 +934,19 @@
                                         }
                                     ]
                                 ),
                             ]
                         )
                 self.timecorr_df.set_index("run_timestamp", inplace=True)
                 if len(self.timecorr_df) > 1:
-                    if mode == "partial":
-                        time_dict = fit_time_means(
-                            np.array(self.timecorr_df.index),
-                            np.array(self.timecorr_df["mean"]),
-                            np.array(self.timecorr_df["sigma"]),
-                        )
-
-                    elif mode == "full":
-                        time_dict = {
-                            time: mean
-                            for time, mean in zip(
-                                np.array(self.timecorr_df.index),
-                                np.array(self.timecorr_df["mean"]),
-                            )
-                        }
-
-                    else:
-                        raise ValueError("unknown mode")
+                    time_dict = fit_time_means(
+                        np.array(self.timecorr_df.index),
+                        np.array(self.timecorr_df["mean"]),
+                        np.array(self.timecorr_df["sigma"]),
+                    )
 
                     df[output_name] = df[aoe_param] / np.array(
                         [time_dict[tstamp] for tstamp in df["run_timestamp"]]
                     )
                     self.update_cal_dicts(
                         {
                             tstamp: {
@@ -1104,23 +1088,23 @@
                 f"{aoe_param}>{aoe_range[0]}&{aoe_param}<{aoe_range[1]}&{self.dt_param}>{dt_range[0]}&{self.dt_param}<{dt_range[1]}&{self.dt_param}=={self.dt_param}"
             )
 
             final_df = dep_events.query(self.dt_res_dict["final_selection"])
 
             hist, bins, var = pgh.get_hist(
                 final_df[self.dt_param],
-                dx=32,
+                dx=10,
                 range=(
                     np.nanmin(final_df[self.dt_param]),
                     np.nanmax(final_df[self.dt_param]),
                 ),
             )
 
             bcs = pgh.get_bin_centers(bins)
-            mus = bcs[pgc.get_i_local_maxima(hist / (np.sqrt(var) + 10**-99), 2)]
+            mus = pgc.get_i_local_maxima(hist / (np.sqrt(var) + 10**-99), 2)
             pk_pars, pk_covs = pgc.hpge_fit_energy_peak_tops(
                 hist,
                 bins,
                 var=var,
                 peak_locs=mus,
                 n_to_fit=5,
             )
@@ -1131,15 +1115,15 @@
 
             if len(mus) > 2:
                 ids = np.array(
                     sorted([np.argmax(amps), np.argmax(amps[amps != np.argmax(amps)])])
                 )
             else:
                 ids = np.full(len(mus), True, dtype=bool)
-            mus = mus[ids]
+            mus = [bcs[int(mu)] for mu in mus[ids]]
             sigmas = sigmas[ids]
             amps = amps[ids]
 
             self.dt_res_dict["dt_fit"] = {"mus": mus, "sigmas": sigmas, "amps": amps}
 
             if len(mus) < 2:
                 log.info("Only 1 drift time peak found, no correction needed")
@@ -1168,16 +1152,16 @@
 
                 self.dt_res_dict["aoe_fit2"] = {
                     "pars": aoe_pars2.to_dict(),
                     "errs": aoe_errs2.to_dict(),
                 }
 
                 try:
-                    self.alpha = (aoe_pars2["mu"] - aoe_pars["mu"]) / (
-                        (mus[0] * aoe_pars["mu"]) - (mus[1] * aoe_pars2["mu"])
+                    self.alpha = (aoe_pars["mu"] - aoe_pars2["mu"]) / (
+                        (mus[0] * aoe_pars2["mu"]) - (mus[1] * aoe_pars["mu"])
                     )
                 except ZeroDivisionError:
                     self.alpha = 0
                 self.dt_res_dict["alpha"] = self.alpha
                 log.info(f"dtcorr successful alpha:{self.alpha}")
 
         except BaseException as e:
@@ -1548,23 +1532,32 @@
             if e == KeyboardInterrupt:
                 raise (e)
             elif self.debug_mode:
                 raise (e)
             log.error("A/E cut determination failed")
             self.low_cut_val = np.nan
             data[output_cut_param] = False
-
-        self.update_cal_dicts(
-            {
-                output_cut_param: {
-                    "expression": f"({aoe_param}>a)",
-                    "parameters": {"a": self.low_cut_val},
+        if self.dt_cut_param is not None and self.dt_cut_hard is True:
+            self.update_cal_dicts(
+                {
+                    output_cut_param: {
+                        "expression": f"({aoe_param}>a) & ({self.dt_cut_param})",
+                        "parameters": {"a": self.low_cut_val},
+                    }
                 }
-            }
-        )
+            )
+        else:
+            self.update_cal_dicts(
+                {
+                    output_cut_param: {
+                        "expression": f"({aoe_param}>a)",
+                        "parameters": {"a": self.low_cut_val},
+                    }
+                }
+            )
 
     def calculate_survival_fractions_sweep(
         self,
         data,
         aoe_param,
         peaks,
         fit_widths,
@@ -1746,24 +1739,21 @@
         initial_aoe_param,
         peaks_of_interest=None,
         fit_widths=None,
         cut_peak_idx=0,
         dep_acc=0.9,
         sf_nsamples=11,
         sf_cut_range=(-5, 5),
-        timecorr_mode="full",
     ):
         if peaks_of_interest is None:
             peaks_of_interest = [1592.5, 1620.5, 2039, 2103.53, 2614.50]
         if fit_widths is None:
             fit_widths = [(40, 25), (25, 40), (0, 0), (25, 40), (50, 50)]
 
-        self.time_correction(
-            df, initial_aoe_param, mode=timecorr_mode, output_name="AoE_Timecorr"
-        )
+        self.time_correction(df, initial_aoe_param, output_name="AoE_Timecorr")
 
         if self.dt_corr is True:
             aoe_param = "AoE_DTcorr"
             self.drift_time_correction(df, "AoE_Timecorr", out_param=aoe_param)
         else:
             aoe_param = "AoE_Timecorr"
 
@@ -1783,22 +1773,32 @@
             output_cut_param="AoE_Low_Cut",
         )
 
         df["AoE_Double_Sided_Cut"] = df["AoE_Low_Cut"] & (
             df["AoE_Classifier"] < self.high_cut_val
         )
 
-        self.update_cal_dicts(
-            {
-                "AoE_High_Side_Cut": {
-                    "expression": "(a>AoE_Classifier)",
-                    "parameters": {"a": self.high_cut_val},
+        if self.dt_cut_param is not None and self.dt_cut_hard is True:
+            self.update_cal_dicts(
+                {
+                    "AoE_High_Side_Cut": {
+                        "expression": f"(a>AoE_Classifier)& ({self.dt_cut_param})",
+                        "parameters": {"a": self.high_cut_val},
+                    }
                 }
-            }
-        )
+            )
+        else:
+            self.update_cal_dicts(
+                {
+                    "AoE_High_Side_Cut": {
+                        "expression": "(a>AoE_Classifier)",
+                        "parameters": {"a": self.high_cut_val},
+                    }
+                }
+            )
 
         self.update_cal_dicts(
             {
                 "AoE_Double_Sided_Cut": {
                     "expression": "(AoE_High_Side_Cut) & (AoE_Low_Cut)",
                     "parameters": {},
                 }
@@ -1962,20 +1962,17 @@
                 f'{aoe_class.dt_res_dict["aoe_grp1"]}&({aoe_param}<{aoe_pars["x_hi"]})&({aoe_param}>{aoe_pars["x_lo"]})'
             )[aoe_param],
             bins=400,
             histtype="step",
             label="data",
         )
         dx = np.diff(aoe_bins)
-        aoe_class.pdf.components = False
-        plt.plot(
-            xs, aoe_class.pdf.get_pdf(xs, *aoe_pars.values()) * dx[0], label="full fit"
-        )
+        plt.plot(xs, aoe_class.pdf.get_pdf(xs, *aoe_pars) * dx[0], label="full fit")
         aoe_class.pdf.components = True
-        sig, bkg = aoe_class.pdf.get_pdf(xs, *aoe_pars.values())
+        sig, bkg = aoe_class.pdf.get_pdf(xs, *aoe_pars)
         aoe_class.pdf.components = False
         plt.plot(xs, sig * dx[0], label="peak fit")
         plt.plot(xs, bkg * dx[0], label="bkg fit")
         plt.legend(loc="upper left")
         plt.xlabel("A/E")
         plt.ylabel("counts")
 
@@ -1987,19 +1984,17 @@
                 f'{aoe_class.dt_res_dict["aoe_grp2"]}&({aoe_param}<{aoe_pars2["x_hi"]})&({aoe_param}>{aoe_pars2["x_lo"]})'
             )[aoe_param],
             bins=400,
             histtype="step",
             label="Data",
         )
         dx = np.diff(aoe_bins2)
-        plt.plot(
-            xs, aoe_class.pdf.get_pdf(xs, *aoe_pars2.values()) * dx[0], label="full fit"
-        )
+        plt.plot(xs, aoe_class.pdf.get_pdf(xs, *aoe_pars2) * dx[0], label="full fit")
         aoe_class.pdf.components = True
-        sig, bkg = aoe_class.pdf.get_pdf(xs, *aoe_pars2.values())
+        sig, bkg = aoe_class.pdf.get_pdf(xs, *aoe_pars2)
         aoe_class.pdf.components = False
         plt.plot(xs, sig * dx[0], label="peak fit")
         plt.plot(xs, bkg * dx[0], label="bkg fit")
         plt.legend(loc="upper left")
         plt.xlabel("A/E")
         plt.ylabel("counts")
 
@@ -2018,15 +2013,15 @@
         mus = aoe_class.dt_res_dict["dt_fit"]["mus"]
         sigmas = aoe_class.dt_res_dict["dt_fit"]["sigmas"]
         amps = aoe_class.dt_res_dict["dt_fit"]["amps"]
 
         for mu, sigma, amp in zip(mus, sigmas, amps):
             plt.plot(
                 pgh.get_bin_centers(bins),
-                nb_gauss_amp(pgh.get_bin_centers(bins), mu, sigma, amp),
+                gaussian.get_pdf(pgh.get_bin_centers(bins), mu, sigma) * amp,
             )
         plt.xlabel("drift time (ns)")
         plt.ylabel("Counts")
 
         plt.subplot(2, 2, 4)
         bins = np.linspace(
             np.nanpercentile(final_df[aoe_param], 1),
```

### Comparing `pygama-2.0.0/src/pygama/pargen/data_cleaning.py` & `pygama-2.0.0a1/src/pygama/pargen/data_cleaning.py`

 * *Files identical despite different names*

### Comparing `pygama-2.0.0/src/pygama/pargen/dplms_ge_dict.py` & `pygama-2.0.0a1/src/pygama/pargen/dplms_ge_dict.py`

 * *Files identical despite different names*

### Comparing `pygama-2.0.0/src/pygama/pargen/dsp_optimize.py` & `pygama-2.0.0a1/src/pygama/pargen/dsp_optimize.py`

 * *Files identical despite different names*

### Comparing `pygama-2.0.0/src/pygama/pargen/energy_cal.py` & `pygama-2.0.0a1/src/pygama/pargen/energy_cal.py`

 * *Files 1% similar despite different names*

```diff
@@ -473,16 +473,16 @@
 
         # First calculate range around peaks to fit
 
         euc_min, euc_max = (
             (Polynomial(self.pars) - i).roots()
             for i in (peaks_kev[0] * 0.9, peaks_kev[-1] * 1.1)
         )
-        euc_min = np.nanmin(euc_min)
-        euc_max = np.nanmax(euc_max)
+        euc_min = euc_min[0]
+        euc_max = euc_max[0]
 
         if euc_min < 0:
             euc_min = 0
         if euc_max > np.nanmax(e_uncal) * 1.1:
             euc_max = np.nanmax(e_uncal) * 1.1
 
         d_euc = 0.5 / self.pars[1]
@@ -827,16 +827,16 @@
                 loc = (Polynomial(self.pars) - peak).roots()[0]
 
             if fit_range is None:
                 euc_min, euc_max = (
                     (Polynomial(self.pars) - i).roots()
                     for i in (peaks_kev[0] * 0.9, peaks_kev[-1] * 1.1)
                 )
-                euc_min = np.nanmin(euc_min)
-                euc_max = np.nanmax(euc_max)
+                euc_min = euc_min[0]
+                euc_max = euc_max[0]
                 if euc_min < 0:
                     euc_min = 0
                 if euc_max > np.nanmax(e_uncal) * 1.1:
                     euc_max = np.nanmax(e_uncal) * 1.1
                 d_euc = 0.5 / self.pars[1]
                 if self.uncal_is_int:
                     euc_min, euc_max, d_euc = pgh.better_int_binning(
@@ -2480,31 +2480,24 @@
         cov = np.array([[0, 0], [0, scale_cov]])
         errs = np.diag(np.sqrt(cov))
     else:
         d_mu_d_es = np.zeros(len(mus))
         for n in range(len(energy_scale_pars) - 1):
             d_mu_d_es += energy_scale_pars[n + 1] * mus ** (n + 1)
         e_weights = np.sqrt(d_mu_d_es * mu_vars)
-        mask = np.isfinite(e_weights)
         poly_pars = (
-            Polynomial.fit(
-                mus[mask], energies_kev[mask], deg=deg, w=1 / e_weights[mask]
-            )
-            .convert()
-            .coef
+            Polynomial.fit(mus, energies_kev, deg=deg, w=1 / e_weights).convert().coef
         )
         if fixed is not None:
             for idx, val in fixed.items():
                 if val is True or val is None:
                     pass
                 else:
                     poly_pars[idx] = val
-        c = cost.LeastSquares(
-            mus[mask], energies_kev[mask], e_weights[mask], poly_wrapper
-        )
+        c = cost.LeastSquares(mus, energies_kev, e_weights, poly_wrapper)
         m = Minuit(c, *poly_pars)
         if fixed is not None:
             for idx in list(fixed):
                 m.fixed[idx] = True
         m.simplex()
         m.migrad()
         m.hesse()
```

### Comparing `pygama-2.0.0/src/pygama/pargen/energy_optimisation.py` & `pygama-2.0.0a1/src/pygama/pargen/energy_optimisation.py`

 * *Files identical despite different names*

### Comparing `pygama-2.0.0/src/pygama/pargen/extract_tau.py` & `pygama-2.0.0a1/src/pygama/pargen/extract_tau.py`

 * *Files identical despite different names*

### Comparing `pygama-2.0.0/src/pygama/pargen/lq_cal.py` & `pygama-2.0.0a1/src/pygama/pargen/lq_cal.py`

 * *Files 13% similar despite different names*

```diff
@@ -52,47 +52,47 @@
     """
     Function for getting a distribution of LQ values for a given peak. Returns a histogram of the
     LQ distribution as well as an array of bin edges
     """
 
     if sidebands:
         # Get a histogram of events in the peak using sideband subtraction
-        # Uses a 13 keV window, and the sideband is to the right of the peak
+        # Uses a 6 keV window, and the sideband is to the right of the peak
         # Default option
 
-        df_peak = df.query(
-            f"{cal_energy_param} < ({peak} + 5) & {cal_energy_param} > ({peak} - 8)"
+        peak_window = (df[cal_energy_param] < peak + 3) & (
+            df[cal_energy_param] > peak - 3
         )
-        df_sideband = df.query(
-            f"{cal_energy_param} < ({peak} + 20) & {cal_energy_param} > ({peak} + 7)"
+        sideband_window = (df[cal_energy_param] < peak + 18) & (
+            df[cal_energy_param] > peak + 12
         )
 
-        fit_range = get_fit_range(df_peak[lq_param].to_numpy())
+        fit_range = get_fit_range(df[lq_param][peak_window])
 
         sideband_hist, bins, _ = pgh.get_hist(
-            df_sideband[lq_param].to_numpy(), bins=100, range=fit_range
+            df[lq_param][sideband_window], bins=100, range=fit_range
         )
         dep_hist, _, _ = pgh.get_hist(
-            df_peak[lq_param].to_numpy(), bins=100, range=fit_range
+            df[lq_param][peak_window], bins=100, range=fit_range
         )
         final_hist = dep_hist - sideband_hist
         var = np.sqrt(np.add(sideband_hist, dep_hist))
 
         return final_hist, bins, var
 
     else:
-        # Return a histogram in a 13 keV range surrounding the specified peak
+        # Return a histogram in a 5 keV range surrounding the specified peak
+        # Only use if peak statistics are low
 
-        df_peak = df.query(
-            f"{cal_energy_param} < ({peak} + 5) & {cal_energy_param} > ({peak} - 8)"
+        peak_window = (df[cal_energy_param] < peak + 2.5) & (
+            df[cal_energy_param] > peak - 2.5
         )
-
-        fit_range = get_fit_range(df_peak[lq_param].to_numpy())
+        fit_range = get_fit_range(df[lq_param][peak_window])
         dep_hist, bins, var = pgh.get_hist(
-            df_peak[lq_param].to_numpy(), bins=100, range=fit_range
+            df[lq_param][peak_window], bins=100, range=fit_range
         )
 
         return dep_hist, bins, var
 
 
 def binned_lq_fit(
     df: pd.DataFrame,
@@ -151,57 +151,55 @@
     m1 = Minuit(c1, mu=mu, sigma=sigma)
     m1.simplex().migrad()
     m1.hesse()
 
     return m1.values, m1.errors, hist, bins
 
 
-def calculate_time_means(
-    df: pd.DataFrame,
-    lq_param: str,
-    cal_energy_param: str,
-    peak: float,
-    sidebands: bool = True,
-):
-    """
-    Function for calculating the arithmetic mean and sigma for LQ events in a
-    specified peak
-    """
-
-    df_peak = df.query(
-        f"{cal_energy_param} < ({peak} + 5) & {cal_energy_param} > ({peak} - 8)"
-    )
-    fit_range = get_fit_range(df_peak[lq_param].to_numpy())
-
-    lq_peak_vals = df_peak.query(
-        f"{lq_param} < {fit_range[1]} & {lq_param} > {fit_range[0]}"
-    )[lq_param].to_numpy()
-
-    mean = np.mean(lq_peak_vals)
-    sigma = np.std(lq_peak_vals)
-    mean_err = sigma / np.sqrt(len(lq_peak_vals))
-    sig_err = 2 * sigma**4 / (len(lq_peak_vals) - 1)
-
-    pars = {"mu": mean, "sigma": sigma}
-    errors = {"mu": mean_err, "sigma": sig_err}
-
-    return pars, errors
-
-
 def fit_time_means(tstamps, means, reses):
     out_dict = {}
     current_tstamps = []
     current_means = []
     current_reses = []
 
+    # Temporary fix
+    # TODO: Create better method of measuring time stability
     rolling_mean = means[np.where(~np.isnan(means))[0][0]]
+    # rolling_mean = means[
+    #     np.where(
+    #         (np.abs(np.diff(means)) < (0.4 * np.array(reses)[1:]))
+    #         & (~np.isnan(np.abs(np.diff(means)) < (0.4 * np.array(reses)[1:])))
+    #     )[0][0]
+    # ]
     for i, tstamp in enumerate(tstamps):
-        if np.isnan(means[i]) or np.isnan(reses[i]):
-            out_dict[tstamp] = np.nan
-
+        if (
+            (
+                (np.abs(means[i] - rolling_mean) > 0.4 * reses[i])
+                and (np.abs(means[i] - rolling_mean) > rolling_mean * 0.5)
+            )
+            or np.isnan(means[i])
+            or np.isnan(reses[i])
+        ):
+            if i + 1 == len(means):
+                out_dict[tstamp] = np.nan
+            else:
+                if (np.abs(means[i + 1] - means[i]) < 0.4 * reses[i + 1]) and not (
+                    np.isnan(means[i])
+                    or np.isnan(means[i + 1])
+                    or np.isnan(reses[i])
+                    or np.isnan(reses[i + 1])
+                ):
+                    for ts in current_tstamps:
+                        out_dict[ts] = rolling_mean
+                    rolling_mean = means[i]
+                    current_means = [means[i]]
+                    current_tstamps = [tstamp]
+                    current_reses = [reses[i]]
+                else:
+                    out_dict[tstamp] = np.nan
         else:
             current_tstamps.append(tstamp)
             current_means.append(means[i])
             current_reses.append(reses[i])
             rolling_mean = np.average(
                 current_means, weights=1 / np.array(current_reses)
             )
@@ -213,43 +211,40 @@
 class LQCal:
     """A class for calibrating the LQ parameter and determining the LQ cut value"""
 
     def __init__(
         self,
         cal_dicts: dict,
         cal_energy_param: str,
-        dt_param: str,
         eres_func: callable,
         cdf: callable = gaussian,
         selection_string: str = "is_valid_cal&is_not_pulser",
         debug_mode=False,
     ):
         """
         Parameters
         ----------
         cal_dicts: dict
             A dictionary containing the hit-level operations to apply
             to the data.
         cal_energy_param: string
             The calibrated energy parameter of choice
-        dt_param: string
-            The drift-time parameter of choice
         eres_function: callable
             The energy resolutions function
         cdf: callable
             The CDF used for the binned fits
         selection_string: string
             A string of flags to apply the data when running the calibration
-        debug_mode: boolean
-            Determines if the class is initialized in debug mode
+        plot_options: dict
+            A dict containing the plot functions the user wants to run,
+            and any user options to provide those plot functions
         """
 
         self.cal_dicts = cal_dicts
         self.cal_energy_param = cal_energy_param
-        self.dt_param = dt_param
         self.eres_func = eres_func
         self.cdf = cdf
         self.selection_string = selection_string
         self.debug_mode = debug_mode
 
     def update_cal_dicts(self, update_dict):
         if re.match(r"(\d{8})T(\d{6})Z", list(self.cal_dicts)[0]):
@@ -259,30 +254,32 @@
                 else:
                     self.cal_dicts[tstamp].update(update_dict)
         else:
             self.cal_dicts.update(update_dict)
 
     def lq_timecorr(self, df, lq_param, output_name="LQ_Timecorr", display=0):
         """
-        Calculates the average LQ value for DEP events for each specified
+        Calculates the average LQ value for DEP events for each specified run
         run_timestamp. Applies a time normalization based on the average LQ value
         in the DEP across all run_timestamps.
         """
 
         log.info("Starting LQ time correction")
         self.timecorr_df = pd.DataFrame()
         try:
             if "run_timestamp" in df:
                 for tstamp, time_df in df.groupby("run_timestamp", sort=True):
                     try:
-                        pars, errs = calculate_time_means(
+                        pars, errs, _, _ = binned_lq_fit(
                             time_df.query(f"{self.selection_string}"),
                             lq_param,
                             self.cal_energy_param,
                             peak=1592.5,
+                            cdf=self.cdf,
+                            sidebands=False,
                         )
                         self.timecorr_df = pd.concat(
                             [
                                 self.timecorr_df,
                                 pd.DataFrame(
                                     [
                                         {
@@ -343,19 +340,21 @@
                         }
                         for tstamp, t_dict in time_dict.items()
                     }
                 )
                 log.info("LQ time correction finished")
             else:
                 try:
-                    pars, errs = calculate_time_means(
+                    pars, errs, _, _ = binned_lq_fit(
                         df.query(f"{self.selection_string}"),
                         lq_param,
                         self.cal_energy_param,
                         peak=1592.5,
+                        cdf=self.cdf,
+                        sidebands=False,
                     )
                     self.timecorr_df = pd.concat(
                         [
                             self.timecorr_df,
                             pd.DataFrame(
                                 [
                                     {
@@ -430,130 +429,107 @@
 
         log.info("Starting LQ drift time correction")
         try:
             pars = binned_lq_fit(df, lq_param, self.cal_energy_param, peak=1592.5)[0]
             mean = pars[0]
             sigma = pars[1]
 
-            dep_events = df.query(
-                f"{self.cal_energy_param} > 1589.5 & {self.cal_energy_param} < 1595.5 & {self.cal_energy_param}=={self.cal_energy_param}&{lq_param}=={lq_param}"
-            )
-
-            dt_range = [
-                np.nanpercentile(dep_events[self.dt_param], 10),
-                np.nanpercentile(dep_events[self.dt_param], 95),
-            ]
-
-            lq_range = [mean - 2 * sigma, mean + 2 * sigma]
-
-            self.lq_range = lq_range
-            self.dt_range = dt_range
-
-            final_df = dep_events.query(
-                f"{lq_param} > {lq_range[0]} & {lq_param} < {lq_range[1]} & {self.dt_param} > {dt_range[0]} & {self.dt_param} < {dt_range[1]}"
+            lq_mask = (df[lq_param] < (2 * sigma + mean)) & (
+                df[lq_param] > (mean - 2 * sigma)
             )
+            dep_mask = (df[cal_energy_param] < 1595) & (df[cal_energy_param] > 1590)
 
+            ids = np.isnan(df[lq_param]) | np.isnan(df["dt_eff"])
             result = linregress(
-                final_df[self.dt_param],
-                final_df[lq_param],
+                df["dt_eff"][~ids & dep_mask & lq_mask],
+                df[lq_param][~ids & dep_mask & lq_mask],
                 alternative="greater",
             )
             self.dt_fit_pars = result
 
-            df["LQ_Corrected"] = (
-                df[lq_param]
-                - df[self.dt_param] * self.dt_fit_pars[0]
-                - self.dt_fit_pars[1]
+            df["LQ_Classifier"] = (
+                df[lq_param] - df["dt_eff"] * self.dt_fit_pars[0] - self.dt_fit_pars[1]
             )
 
         except BaseException as e:
             if e == KeyboardInterrupt:
                 raise (e)
             elif self.debug_mode:
                 raise (e)
             log.error("LQ drift time correction failed")
             self.dt_fit_pars = (np.nan, np.nan)
 
         self.update_cal_dicts(
             {
-                "LQ_Corrected": {
+                "LQ_Classifier": {
                     "expression": f"{lq_param} - dt_eff*a - b",
                     "parameters": {"a": self.dt_fit_pars[0], "b": self.dt_fit_pars[1]},
                 }
             }
         )
 
     def get_cut_lq_dep(self, df: pd.DataFrame(), lq_param: str, cal_energy_param: str):
         """
         Determines the cut value for LQ. Value is calculated by fitting the LQ distribution
-        for events in the DEP to a gaussian. The LQ values are normalized by the fitted
-        sigma, and the cut value is set to a value of 3. Sideband subtraction is used to
-        determine the LQ distribution for DEP events. Events greater than the cut value
-        fail the cut.
+        for events in the DEP to a gaussian. The cut value is set at 3*sigma of the fit.
+        Sideband subtraction is used to determine the LQ distribution for DEP events.
+        Events greater than the cut value fail the cut.
         """
 
         log.info("Starting LQ Cut calculation")
         try:
-
             pars, errs, hist, bins = binned_lq_fit(
-                df, lq_param, cal_energy_param, peak=1592.5
+                df, "LQ_Classifier", cal_energy_param, peak=1592.5
             )
+            cut_val = 3 * pars[1]
 
             self.cut_fit_pars = pars
             self.cut_fit_errs = errs
             self.fit_hist = (hist, bins)
-            self.cut_val = 3
+            self.cut_val = cut_val
 
-            df["LQ_Classifier"] = np.divide(df[lq_param].to_numpy(), pars[1])
-            df["LQ_Cut"] = df["LQ_Classifier"] < self.cut_val
+            df["LQ_Cut"] = df[lq_param] < self.cut_val
 
         except BaseException as e:
             if e == KeyboardInterrupt:
                 raise (e)
             elif self.debug_mode:
                 raise (e)
             log.error("LQ cut determination failed")
             self.cut_val = np.nan
-            c = cost.UnbinnedNLL(np.array([0]), gaussian.pdf)
-            m = Minuit(c, np.full(2, np.nan))
-            self.cut_fit_pars = pars = m.values
 
         self.update_cal_dicts(
             {
-                "LQ_Classifier": {
-                    "expression": f"({lq_param} / a)",
-                    "parameters": {"a": pars[1]},
-                },
                 "LQ_Cut": {
-                    "expression": "(LQ_Classifier < a)",
+                    "expression": f"({lq_param} < a)",
                     "parameters": {"a": self.cut_val},
-                },
+                }
             }
         )
 
     def calibrate(self, df, initial_lq_param):
         """Run the LQ calibration and calculate the cut value"""
 
-        self.lq_timecorr(df, initial_lq_param)
+        self.lq_timecorr(df, lq_param="LQ_Ecorr")
         log.info("Finished LQ Time Correction")
 
         self.drift_time_correction(
             df, lq_param="LQ_Timecorr", cal_energy_param=self.cal_energy_param
         )
         log.info("Finished LQ Drift Time Correction")
 
         self.get_cut_lq_dep(
-            df, lq_param="LQ_Corrected", cal_energy_param=self.cal_energy_param
+            df, lq_param="LQ_Classifier", cal_energy_param=self.cal_energy_param
         )
         log.info("Finished Calculating the LQ Cut Value")
 
         final_lq_param = "LQ_Classifier"
-        peaks_of_interest = [1592.5, 2039, 2103.53, 2614.50]
+        peaks_of_interest = [1592.5, 1620.5, 2039, 2103.53, 2614.50]
         self.low_side_sf = pd.DataFrame()
-        fit_widths = [(40, 25), (0, 0), (25, 40), (50, 50)]
+        fit_widths = [(40, 25), (25, 40), (0, 0), (25, 40), (50, 50)]
         self.low_side_peak_dfs = {}
 
         log.info("Calculating peak survival fractions")
         for i, peak in enumerate(peaks_of_interest):
             try:
                 select_df = df.query(f"{self.selection_string}")
                 fwhm = self.eres_func(peak)
@@ -566,16 +542,16 @@
 
                     cut_df, sf, sf_err = AoE.compton_sf_sweep(
                         peak_df[self.cal_energy_param].to_numpy(),
                         peak_df[final_lq_param].to_numpy(),
                         self.cut_val,
                         peak,
                         fwhm,
-                        cut_range=(0, 5),
-                        n_samples=30,
+                        cut_range=(0, 0.6),
+                        n_samples=10,
                         mode="less",
                     )
                     self.low_side_sf = pd.concat(
                         [
                             self.low_side_sf,
                             pd.DataFrame([{"peak": peak, "sf": sf, "sf_err": sf_err}]),
                         ]
@@ -590,16 +566,16 @@
                     cut_df, sf, sf_err = AoE.get_sf_sweep(
                         peak_df[self.cal_energy_param].to_numpy(),
                         peak_df[final_lq_param].to_numpy(),
                         self.cut_val,
                         peak,
                         fwhm,
                         fit_range=fit_range,
-                        cut_range=(0, 5),
-                        n_samples=30,
+                        cut_range=(0, 0.6),
+                        n_samples=10,
                         mode="less",
                     )
                     self.low_side_sf = pd.concat(
                         [
                             self.low_side_sf,
                             pd.DataFrame([{"peak": peak, "sf": sf, "sf_err": sf_err}]),
                         ]
@@ -625,59 +601,50 @@
     lq_class, data, lq_param="LQ_Timecorr", figsize=(12, 8), fontsize=12
 ) -> plt.figure:
     """Plots the mean LQ value calculated for each given timestamp"""
 
     plt.rcParams["figure.figsize"] = figsize
     plt.rcParams["font.size"] = fontsize
     fig, ax = plt.subplots(1, 1)
-    try:
-        ax.errorbar(
-            [
-                datetime.strptime(tstamp, "%Y%m%dT%H%M%SZ")
-                for tstamp in lq_class.timecorr_df.index
-            ],
-            lq_class.timecorr_df["mean"],
-            yerr=lq_class.timecorr_df["mean_err"],
-            linestyle=" ",
-        )
+    # try:
+    ax.errorbar(
+        [
+            datetime.strptime(tstamp, "%Y%m%dT%H%M%SZ")
+            for tstamp in lq_class.timecorr_df.index
+        ],
+        lq_class.timecorr_df["mean"],
+        yerr=lq_class.timecorr_df["mean_err"],
+        linestyle=" ",
+    )
 
-        grouped_means = [
-            cal_dict["LQ_Timecorr"]["parameters"]["a"]
-            for tstamp, cal_dict in lq_class.cal_dicts.items()
-        ]
-        ax.step(
-            [
-                datetime.strptime(tstamp, "%Y%m%dT%H%M%SZ")
-                for tstamp in lq_class.cal_dicts
-            ],
-            grouped_means,
-            where="post",
-        )
-        ax.fill_between(
-            [
-                datetime.strptime(tstamp, "%Y%m%dT%H%M%SZ")
-                for tstamp in lq_class.cal_dicts
-            ],
-            y1=np.array(grouped_means) - 0.2 * np.array(lq_class.timecorr_df["res"]),
-            y2=np.array(grouped_means) + 0.2 * np.array(lq_class.timecorr_df["res"]),
-            color="green",
-            alpha=0.2,
-        )
-        ax.fill_between(
-            [
-                datetime.strptime(tstamp, "%Y%m%dT%H%M%SZ")
-                for tstamp in lq_class.cal_dicts
-            ],
-            y1=np.array(grouped_means) - 0.4 * np.array(lq_class.timecorr_df["res"]),
-            y2=np.array(grouped_means) + 0.4 * np.array(lq_class.timecorr_df["res"]),
-            color="yellow",
-            alpha=0.2,
-        )
-    except Exception:
-        pass
+    grouped_means = [
+        cal_dict["LQ_Timecorr"]["parameters"]["a"]
+        for tstamp, cal_dict in lq_class.cal_dicts.items()
+    ]
+    ax.step(
+        [datetime.strptime(tstamp, "%Y%m%dT%H%M%SZ") for tstamp in lq_class.cal_dicts],
+        grouped_means,
+        where="post",
+    )
+    ax.fill_between(
+        [datetime.strptime(tstamp, "%Y%m%dT%H%M%SZ") for tstamp in lq_class.cal_dicts],
+        y1=np.array(grouped_means) - 0.2 * np.array(lq_class.timecorr_df["res"]),
+        y2=np.array(grouped_means) + 0.2 * np.array(lq_class.timecorr_df["res"]),
+        color="green",
+        alpha=0.2,
+    )
+    ax.fill_between(
+        [datetime.strptime(tstamp, "%Y%m%dT%H%M%SZ") for tstamp in lq_class.cal_dicts],
+        y1=np.array(grouped_means) - 0.4 * np.array(lq_class.timecorr_df["res"]),
+        y2=np.array(grouped_means) + 0.4 * np.array(lq_class.timecorr_df["res"]),
+        color="yellow",
+        alpha=0.2,
+    )
+    # except Exception:
+    #     pass
     ax.set_xlabel("time")
     ax.set_ylabel("LQ mean")
     myfmt = mdates.DateFormatter("%b %d")
     ax.xaxis.set_major_formatter(myfmt)
     plt.close()
     return fig
 
@@ -712,19 +679,14 @@
         )
 
         x = np.linspace(0, max_dt, 100)
         model = lq_class.dt_fit_pars[0] * x + lq_class.dt_fit_pars[1]
 
         plt.plot(x, model, color="r")
 
-        plt.axvline(lq_class.dt_range[0], color="k")
-        plt.axvline(lq_class.dt_range[1], color="k")
-        plt.axhline(lq_class.lq_range[0], color="k")
-        plt.axhline(lq_class.lq_range[1], color="k")
-
         plt.xlabel("Drift Time (ns)")
         plt.ylabel("LQ")
 
         plt.title("LQ versus Drift Time for DEP")
 
     except Exception:
         pass
@@ -738,48 +700,37 @@
     """Plots the final histogram of LQ values for events in the
     DEP, and the fit results used for determining the cut
     value"""
 
     plt.rcParams["figure.figsize"] = figsize
     plt.rcParams["font.size"] = fontsize
     fig, (ax1, ax2) = plt.subplots(2, 1)
+
     try:
         hist, bins = lq_class.fit_hist
         fit_pars = lq_class.cut_fit_pars
 
-        x_low = bins[0]
-        x_high = bins[-1]
-
         ax1.stairs(hist, bins, label="data")
         xs = np.linspace(round(bins[0], 3), round(bins[-1], 3), len(bins) - 1)
         ls = np.sum(hist)
         dx = np.diff(bins)
         ax1.plot(
             xs,
-            gaussian.pdf_norm(xs, x_low, x_high, fit_pars[0], fit_pars[1]) * dx * ls,
+            gaussian.pdf_norm(xs, fit_pars[0], fit_pars[1]) * dx * ls,
             label="Gaussian Fit",
         )
 
         # ax1.set_xlabel('LQ')
         ax1.set_title("Fit of LQ events in DEP")
         ax1.legend()
 
         bin_centers = (bins[:-1] + bins[1:]) / 2
         reses = (
-            hist
-            - (
-                gaussian.pdf_norm(bin_centers, x_low, x_high, fit_pars[0], fit_pars[1])
-                * dx
-                * ls
-            )
-        ) / (
-            gaussian.pdf_norm(bin_centers, x_low, x_high, fit_pars[0], fit_pars[1])
-            * dx
-            * ls
-        )
+            hist - (gaussian.pdf_norm(bin_centers, fit_pars[0], fit_pars[1]) * dx * ls)
+        ) / (gaussian.pdf_norm(bin_centers, fit_pars[0], fit_pars[1]) * dx * ls)
         ax2.plot(bin_centers, reses, marker="s", linestyle="")
         ax2.set_xlabel("LQ")
         ax2.set_ylabel("residuals")
 
     except Exception:
         pass
 
@@ -956,15 +907,15 @@
 
 
 def plot_classifier(
     lq_class,
     data,
     lq_param="LQ_Classifier",
     xrange=(800, 3000),
-    yrange=(-10, 30),
+    yrange=(-2, 8),
     xn_bins=700,
     yn_bins=500,
     figsize=(12, 8),
     fontsize=12,
 ) -> plt.figure:
     plt.rcParams["figure.figsize"] = figsize
     plt.rcParams["font.size"] = fontsize
```

### Comparing `pygama-2.0.0/src/pygama/pargen/noise_optimization.py` & `pygama-2.0.0a1/src/pygama/pargen/noise_optimization.py`

 * *Files identical despite different names*

### Comparing `pygama-2.0.0/src/pygama/pargen/utils.py` & `pygama-2.0.0a1/src/pygama/pargen/utils.py`

 * *Files identical despite different names*

### Comparing `pygama-2.0.0/src/pygama/utils.py` & `pygama-2.0.0a1/src/pygama/utils.py`

 * *Files identical despite different names*

### Comparing `pygama-2.0.0/src/pygama.egg-info/PKG-INFO` & `pygama-2.0.0a1/src/pygama.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygama
-Version: 2.0.0
+Version: 2.0.0a1
 Summary: Python package for data processing and analysis
 Author: The LEGEND collaboration
 Maintainer: The LEGEND collaboration
 Project-URL: Homepage, https://github.com/legend-exp/pygama
 Project-URL: Bug Tracker, https://github.com/legend-exp/pygama/issues
 Project-URL: Discussions, https://github.com/legend-exp/pygama/discussions
 Project-URL: Changelog, https://github.com/legend-exp/pygama/releases
@@ -24,16 +24,15 @@
 License-File: LICENSE
 Requires-Dist: hist
 Requires-Dist: colorlog
 Requires-Dist: dspeed>=1.3
 Requires-Dist: h5py>=3.2
 Requires-Dist: iminuit
 Requires-Dist: legend-daq2lh5>=1.2.1
-Requires-Dist: legend-pydataobj>=1.7
-Requires-Dist: pylegendmeta>=0.9
+Requires-Dist: legend-pydataobj>=1.6
 Requires-Dist: matplotlib
 Requires-Dist: numba!=0.53.*,!=0.54.*,!=0.57
 Requires-Dist: numpy>=1.21
 Requires-Dist: pandas>=1.4.4
 Requires-Dist: pint
 Requires-Dist: pyyaml
 Requires-Dist: scikit-learn
```

### Comparing `pygama-2.0.0/src/pygama.egg-info/SOURCES.txt` & `pygama-2.0.0a1/src/pygama.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -9,32 +9,34 @@
 src/pygama.egg-info/PKG-INFO
 src/pygama.egg-info/SOURCES.txt
 src/pygama.egg-info/dependency_links.txt
 src/pygama.egg-info/entry_points.txt
 src/pygama.egg-info/not-zip-safe
 src/pygama.egg-info/requires.txt
 src/pygama.egg-info/top_level.txt
+src/pygama/dsp/__init__.py
+src/pygama/dsp/processors/__init__.py
 src/pygama/evt/__init__.py
 src/pygama/evt/aggregators.py
 src/pygama/evt/build_evt.py
 src/pygama/evt/build_tcm.py
 src/pygama/evt/tcm.py
 src/pygama/evt/utils.py
 src/pygama/evt/modules/__init__.py
 src/pygama/evt/modules/geds.py
 src/pygama/evt/modules/larveto.py
 src/pygama/evt/modules/legend.py
 src/pygama/evt/modules/spms.py
-src/pygama/evt/modules/xtalk.py
 src/pygama/flow/__init__.py
 src/pygama/flow/data_loader.py
 src/pygama/flow/file_db.py
 src/pygama/flow/utils.py
 src/pygama/hit/__init__.py
 src/pygama/hit/build_hit.py
+src/pygama/lgdo/__init__.py
 src/pygama/math/__init__.py
 src/pygama/math/binned_fitting.py
 src/pygama/math/distributions.py
 src/pygama/math/histogram.py
 src/pygama/math/hpge_peak_fitting.py
 src/pygama/math/least_squares.py
 src/pygama/math/unbinned_fitting.py
@@ -68,24 +70,24 @@
 src/pygama/pargen/dsp_optimize.py
 src/pygama/pargen/energy_cal.py
 src/pygama/pargen/energy_optimisation.py
 src/pygama/pargen/extract_tau.py
 src/pygama/pargen/lq_cal.py
 src/pygama/pargen/noise_optimization.py
 src/pygama/pargen/utils.py
+src/pygama/raw/__init__.py
+src/pygama/vis/__init__.py
 tests/conftest.py
 tests/test_utils.py
 tests/configs/icpc-dsp-config.json
 tests/configs/sipm-dplms-config.json
 tests/configs/sipm-dsp-config.json
 tests/evt/test_build_evt.py
 tests/evt/test_build_tcm.py
 tests/evt/test_evt_utils.py
-tests/evt/test_geds.py
-tests/evt/test_xtalk.py
 tests/evt/configs/basic-evt-config.yaml
 tests/evt/configs/query-test-evt-config.json
 tests/evt/configs/spms-module-config.yaml
 tests/evt/configs/vov-test-evt-config.json
 tests/evt/modules/larveto.py
 tests/flow/conftest.py
 tests/flow/test_data_loader.py
```

### Comparing `pygama-2.0.0/tests/configs/icpc-dsp-config.json` & `pygama-2.0.0a1/tests/configs/icpc-dsp-config.json`

 * *Files identical despite different names*

### Comparing `pygama-2.0.0/tests/configs/sipm-dplms-config.json` & `pygama-2.0.0a1/tests/configs/sipm-dplms-config.json`

 * *Files identical despite different names*

### Comparing `pygama-2.0.0/tests/configs/sipm-dsp-config.json` & `pygama-2.0.0a1/tests/configs/sipm-dsp-config.json`

 * *Files identical despite different names*

### Comparing `pygama-2.0.0/tests/conftest.py` & `pygama-2.0.0a1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pygama-2.0.0/tests/evt/configs/basic-evt-config.yaml` & `pygama-2.0.0a1/tests/evt/configs/basic-evt-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -68,21 +68,18 @@
   energy_sum:
     channels: geds_on
     aggregation_mode: sum
     query: hit.cuspEmax_ctc_cal>25
     expression: hit.cuspEmax_ctc_cal
     initial: 0
   is_usable_aoe:
-    channels: geds_on
     aggregation_mode: keep_at_ch:evt.energy_id
     expression: "True"
     initial: false
   aoe:
-    channels: geds_on
     aggregation_mode: keep_at_ch:evt.energy_id
     expression: hit.AoE_Classifier
     initial: np.nan
   is_aoe_rejected:
-    channels: geds_on
     aggregation_mode: keep_at_ch:evt.energy_id
     expression: ~(hit.AoE_Double_Sided_Cut)
     initial: false
```

### Comparing `pygama-2.0.0/tests/evt/configs/query-test-evt-config.json` & `pygama-2.0.0a1/tests/evt/configs/query-test-evt-config.json`

 * *Files identical despite different names*

### Comparing `pygama-2.0.0/tests/evt/configs/spms-module-config.yaml` & `pygama-2.0.0a1/tests/evt/configs/spms-module-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -92,11 +92,8 @@
     expression: pygama.evt.modules.spms.gather_tcm_data(
       <...>,
       pulse_mask=evt._pulse_mask,
       drop_empty=True)
   lar_coin_class:
     channels: spms_on
     aggregation_mode: function
-    expression: pygama.evt.modules.spms.geds_coincidence_classifier(
-      <...>,
-      geds_t0_ns=evt.t0,
-      ts_bkg_prob=0.5)
+    expression: pygama.evt.modules.spms.geds_coincidence_classifier(<...>, geds_t0_ns=evt.t0)
```

### Comparing `pygama-2.0.0/tests/evt/configs/vov-test-evt-config.json` & `pygama-2.0.0a1/tests/evt/configs/vov-test-evt-config.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9930555555555557%*

 * *Differences: {"'operations'": "{'aoe': {delete: ['channels']}, 'aoe_idx': {delete: ['channels']}, "*

 * *                 "'is_saturated': {delete: ['channels']}}"}*

```diff
@@ -6,20 +6,18 @@
             "ch1121600"
         ],
         "ts_master": "ch1084803"
     },
     "operations": {
         "aoe": {
             "aggregation_mode": "keep_at_ch:evt.energy_id",
-            "channels": "geds_on",
             "expression": "hit.AoE_Classifier"
         },
         "aoe_idx": {
             "aggregation_mode": "keep_at_idx:evt.energy_idx",
-            "channels": "geds_on",
             "expression": "hit.AoE_Classifier"
         },
         "energy": {
             "aggregation_mode": "gather",
             "channels": "geds_on",
             "dtype": "float32",
             "expression": "hit.cuspEmax_ctc_cal",
@@ -52,15 +50,14 @@
             "expression": "evt.energy*evt.aoe"
         },
         "energy_times_multiplicity": {
             "expression": "evt.energy*evt.multiplicity"
         },
         "is_saturated": {
             "aggregation_mode": "keep_at_ch:evt.energy_id",
-            "channels": "geds_on",
             "expression": "hit.is_saturated"
         },
         "multiplicity": {
             "aggregation_mode": "sum",
             "channels": "geds_on",
             "dtype": "int16",
             "expression": "hit.cuspEmax_ctc_cal > a",
```

### Comparing `pygama-2.0.0/tests/evt/test_build_evt.py` & `pygama-2.0.0a1/tests/evt/test_build_evt.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,59 +119,58 @@
     assert isinstance(evt.sub1.timestamp, Array)
 
     assert sorted(evt.keys()) == ["sub1", "sub2"]
     assert sorted(evt.sub1.keys()) == ["timestamp"]
     assert sorted(evt.sub2.keys()) == ["dummy", "multiplicity"]
 
 
-# FIXME: this can't be properly tested until proper testdata is available
-# def test_spms_module(lgnd_test_data, files_config):
-#     build_evt(
-#         files_config,
-#         config=f"{config_dir}/spms-module-config.yaml",
-#         wo_mode="of",
-#     )
-
-#     outfile = files_config["evt"][0]
-
-#     evt = lh5.read("/evt", outfile)
-
-#     t0 = ak.fill_none(ak.nan_to_none(evt.t0.view_as("ak")), 48_000)
-#     tr_pos = evt.trigger_pos.view_as("ak") * 16
-#     assert ak.all(tr_pos > t0 - 30_000)
-#     assert ak.all(tr_pos < t0 + 30_000)
-
-#     mask = evt._pulse_mask
-#     assert isinstance(mask, VectorOfVectors)
-#     assert len(mask) == 10
-#     assert mask.ndim == 3
-
-#     full = evt.spms_amp_full.view_as("ak")
-#     amp = evt.spms_amp.view_as("ak")
-#     assert ak.all(amp > 0.1)
-
-#     assert ak.all(full[mask.view_as("ak")] == amp)
-
-#     wo_empty = evt.spms_amp_wo_empty.view_as("ak")
-#     assert ak.all(wo_empty == amp[ak.count(amp, axis=-1) > 0])
-
-#     rawids = evt.rawid.view_as("ak")
-#     assert rawids.ndim == 2
-#     assert ak.count(rawids) == 30
-
-#     idx = evt.hit_idx.view_as("ak")
-#     assert idx.ndim == 2
-#     assert ak.count(idx) == 30
-
-#     rawids_wo_empty = evt.rawid_wo_empty.view_as("ak")
-#     assert ak.count(rawids_wo_empty) == 7
-
-#     vhit = evt.is_valid_hit.view_as("ak")
-#     vhit.show()
-#     assert ak.all(ak.num(vhit, axis=-1) == ak.num(full, axis=-1))
+def test_spms_module(lgnd_test_data, files_config):
+    build_evt(
+        files_config,
+        config=f"{config_dir}/spms-module-config.yaml",
+        wo_mode="of",
+    )
+
+    outfile = files_config["evt"][0]
+
+    evt = lh5.read("/evt", outfile)
+
+    t0 = ak.fill_none(ak.nan_to_none(evt.t0.view_as("ak")), 48_000)
+    tr_pos = evt.trigger_pos.view_as("ak") * 16
+    assert ak.all(tr_pos > t0 - 30_000)
+    assert ak.all(tr_pos < t0 + 30_000)
+
+    mask = evt._pulse_mask
+    assert isinstance(mask, VectorOfVectors)
+    assert len(mask) == 10
+    assert mask.ndim == 3
+
+    full = evt.spms_amp_full.view_as("ak")
+    amp = evt.spms_amp.view_as("ak")
+    assert ak.all(amp > 0.1)
+
+    assert ak.all(full[mask.view_as("ak")] == amp)
+
+    wo_empty = evt.spms_amp_wo_empty.view_as("ak")
+    assert ak.all(wo_empty == amp[ak.count(amp, axis=-1) > 0])
+
+    rawids = evt.rawid.view_as("ak")
+    assert rawids.ndim == 2
+    assert ak.count(rawids) == 30
+
+    idx = evt.hit_idx.view_as("ak")
+    assert idx.ndim == 2
+    assert ak.count(idx) == 30
+
+    rawids_wo_empty = evt.rawid_wo_empty.view_as("ak")
+    assert ak.count(rawids_wo_empty) == 7
+
+    vhit = evt.is_valid_hit.view_as("ak")
+    vhit.show()
+    assert ak.all(ak.num(vhit, axis=-1) == ak.num(full, axis=-1))
 
 
 def test_vov(lgnd_test_data, files_config):
     build_evt(
         files_config,
         config=f"{config_dir}/vov-test-evt-config.json",
         wo_mode="of",
```

### Comparing `pygama-2.0.0/tests/evt/test_build_tcm.py` & `pygama-2.0.0a1/tests/evt/test_build_tcm.py`

 * *Files identical despite different names*

### Comparing `pygama-2.0.0/tests/evt/test_evt_utils.py` & `pygama-2.0.0a1/tests/evt/test_evt_utils.py`

 * *Files identical despite different names*

### Comparing `pygama-2.0.0/tests/flow/configs/filedb-config.json` & `pygama-2.0.0a1/tests/flow/configs/filedb-config.json`

 * *Files identical despite different names*

### Comparing `pygama-2.0.0/tests/flow/conftest.py` & `pygama-2.0.0a1/tests/flow/conftest.py`

 * *Files identical despite different names*

### Comparing `pygama-2.0.0/tests/flow/test_data_loader.py` & `pygama-2.0.0a1/tests/flow/test_data_loader.py`

 * *Files identical despite different names*

### Comparing `pygama-2.0.0/tests/flow/test_filedb.py` & `pygama-2.0.0a1/tests/flow/test_filedb.py`

 * *Files identical despite different names*

### Comparing `pygama-2.0.0/tests/hit/configs/aggregations-hit-config.json` & `pygama-2.0.0a1/tests/hit/configs/aggregations-hit-config.json`

 * *Files identical despite different names*

### Comparing `pygama-2.0.0/tests/hit/configs/spms-hit-a-config.json` & `pygama-2.0.0a1/tests/hit/configs/spms-hit-a-config.json`

 * *Files identical despite different names*

### Comparing `pygama-2.0.0/tests/hit/test_build_hit.py` & `pygama-2.0.0a1/tests/hit/test_build_hit.py`

 * *Files identical despite different names*

### Comparing `pygama-2.0.0/tests/math/functions/test_crystal_ball.py` & `pygama-2.0.0a1/tests/math/functions/test_crystal_ball.py`

 * *Files identical despite different names*

### Comparing `pygama-2.0.0/tests/math/functions/test_exgauss.py` & `pygama-2.0.0a1/tests/math/functions/test_exgauss.py`

 * *Files identical despite different names*

### Comparing `pygama-2.0.0/tests/math/functions/test_exponential.py` & `pygama-2.0.0a1/tests/math/functions/test_exponential.py`

 * *Files identical despite different names*

### Comparing `pygama-2.0.0/tests/math/functions/test_gauss.py` & `pygama-2.0.0a1/tests/math/functions/test_gauss.py`

 * *Files identical despite different names*

### Comparing `pygama-2.0.0/tests/math/functions/test_gauss_on_exgauss.py` & `pygama-2.0.0a1/tests/math/functions/test_gauss_on_exgauss.py`

 * *Files identical despite different names*

### Comparing `pygama-2.0.0/tests/math/functions/test_gauss_on_exponential.py` & `pygama-2.0.0a1/tests/math/functions/test_gauss_on_exponential.py`

 * *Files identical despite different names*

### Comparing `pygama-2.0.0/tests/math/functions/test_gauss_on_linear.py` & `pygama-2.0.0a1/tests/math/functions/test_gauss_on_linear.py`

 * *Files identical despite different names*

### Comparing `pygama-2.0.0/tests/math/functions/test_gauss_on_step.py` & `pygama-2.0.0a1/tests/math/functions/test_gauss_on_step.py`

 * *Files identical despite different names*

### Comparing `pygama-2.0.0/tests/math/functions/test_gauss_on_uniform.py` & `pygama-2.0.0a1/tests/math/functions/test_gauss_on_uniform.py`

 * *Files identical despite different names*

### Comparing `pygama-2.0.0/tests/math/functions/test_hpge_peak.py` & `pygama-2.0.0a1/tests/math/functions/test_hpge_peak.py`

 * *Files identical despite different names*

### Comparing `pygama-2.0.0/tests/math/functions/test_linear.py` & `pygama-2.0.0a1/tests/math/functions/test_linear.py`

 * *Files identical despite different names*

### Comparing `pygama-2.0.0/tests/math/functions/test_moyal.py` & `pygama-2.0.0a1/tests/math/functions/test_moyal.py`

 * *Files identical despite different names*

### Comparing `pygama-2.0.0/tests/math/functions/test_numba_frozen.py` & `pygama-2.0.0a1/tests/math/functions/test_numba_frozen.py`

 * *Files identical despite different names*

### Comparing `pygama-2.0.0/tests/math/functions/test_poisson.py` & `pygama-2.0.0a1/tests/math/functions/test_poisson.py`

 * *Files identical despite different names*

### Comparing `pygama-2.0.0/tests/math/functions/test_step.py` & `pygama-2.0.0a1/tests/math/functions/test_step.py`

 * *Files identical despite different names*

### Comparing `pygama-2.0.0/tests/math/functions/test_sum_dists.py` & `pygama-2.0.0a1/tests/math/functions/test_sum_dists.py`

 * *Files identical despite different names*

### Comparing `pygama-2.0.0/tests/math/functions/test_triple_gauss_on_double_step.py` & `pygama-2.0.0a1/tests/math/functions/test_triple_gauss_on_double_step.py`

 * *Files identical despite different names*

### Comparing `pygama-2.0.0/tests/math/functions/test_uniform.py` & `pygama-2.0.0a1/tests/math/functions/test_uniform.py`

 * *Files identical despite different names*

### Comparing `pygama-2.0.0/tests/math/test_binned_fitting.py` & `pygama-2.0.0a1/tests/math/test_binned_fitting.py`

 * *Files identical despite different names*

### Comparing `pygama-2.0.0/tests/math/test_distribution_selector_in_sum_dists.py` & `pygama-2.0.0a1/tests/math/test_distribution_selector_in_sum_dists.py`

 * *Files identical despite different names*

### Comparing `pygama-2.0.0/tests/math/test_hpge_peak_fitting.py` & `pygama-2.0.0a1/tests/math/test_hpge_peak_fitting.py`

 * *Files identical despite different names*

### Comparing `pygama-2.0.0/tests/math/test_iminuit_integration.py` & `pygama-2.0.0a1/tests/math/test_iminuit_integration.py`

 * *Files identical despite different names*

### Comparing `pygama-2.0.0/tests/math/test_math_histogram.py` & `pygama-2.0.0a1/tests/math/test_math_histogram.py`

 * *Files identical despite different names*

### Comparing `pygama-2.0.0/tests/math/test_math_utils.py` & `pygama-2.0.0a1/tests/math/test_math_utils.py`

 * *Files identical despite different names*

### Comparing `pygama-2.0.0/tests/math/test_unbinned_fitting.py` & `pygama-2.0.0a1/tests/math/test_unbinned_fitting.py`

 * *Files identical despite different names*

### Comparing `pygama-2.0.0/tests/pargen/test_aoecal.py` & `pygama-2.0.0a1/tests/pargen/test_aoecal.py`

 * *Files identical despite different names*

### Comparing `pygama-2.0.0/tests/pargen/test_datacleaning.py` & `pygama-2.0.0a1/tests/pargen/test_datacleaning.py`

 * *Files identical despite different names*

### Comparing `pygama-2.0.0/tests/pargen/test_ecal.py` & `pygama-2.0.0a1/tests/pargen/test_ecal.py`

 * *Files identical despite different names*

### Comparing `pygama-2.0.0/tests/pargen/test_lqcal.py` & `pygama-2.0.0a1/tests/pargen/test_lqcal.py`

 * *Files 16% similar despite different names*

```diff
@@ -25,15 +25,14 @@
             "parameters": {},
         }
     }
 
     lqcal = lq.LQCal(
         cal_dict,
         "cuspEmax_cal",
-        "dt_eff",
         lambda x: np.sqrt(1.5 + 0.1 * x),
         selection_string="index==index",
         cdf=gaussian,
         debug_mode=True,
     )
 
     df["LQ_Ecorr"] = np.divide(df["lq80"], df["cuspEmax"])
```

