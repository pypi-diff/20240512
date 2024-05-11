# Comparing `tmp/finagg-1.0.0.tar.gz` & `tmp/finagg-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finagg-1.0.0.tar", last modified: Fri Apr  5 23:04:20 2024, max compression
+gzip compressed data, was "finagg-1.0.1.tar", last modified: Sat May 11 23:57:49 2024, max compression
```

## Comparing `finagg-1.0.0.tar` & `finagg-1.0.1.tar`

### file list

```diff
@@ -1,128 +1,128 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 23:04:20.961888 finagg-1.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 23:04:20.933888 finagg-1.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 23:04:20.937888 finagg-1.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      916 2024-04-05 23:04:12.000000 finagg-1.0.0/.github/workflows/build-docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-05 23:04:12.000000 finagg-1.0.0/.github/workflows/test-and-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-05 23:04:12.000000 finagg-1.0.0/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-04-05 23:04:12.000000 finagg-1.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-05 23:04:12.000000 finagg-1.0.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-05 23:04:12.000000 finagg-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    27173 2024-04-05 23:04:20.957888 finagg-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12481 2024-04-05 23:04:12.000000 finagg-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 23:04:20.941888 finagg-1.0.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 23:04:12.000000 finagg-1.0.0/docs/.nojekyll
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-05 23:04:12.000000 finagg-1.0.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 23:04:20.941888 finagg-1.0.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-05 23:04:12.000000 finagg-1.0.0/docs/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-05 23:04:12.000000 finagg-1.0.0/docs/cli.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4239 2024-04-05 23:04:12.000000 finagg-1.0.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-04-05 23:04:12.000000 finagg-1.0.0/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9636 2024-04-05 23:04:12.000000 finagg-1.0.0/docs/conventions.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1895 2024-04-05 23:04:12.000000 finagg-1.0.0/docs/faq.rst
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-05 23:04:12.000000 finagg-1.0.0/docs/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     8648 2024-04-05 23:04:12.000000 finagg-1.0.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-04-05 23:04:12.000000 finagg-1.0.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-04-05 23:04:12.000000 finagg-1.0.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-04-05 23:04:12.000000 finagg-1.0.0/docs/references.rst
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-04-05 23:04:12.000000 finagg-1.0.0/docs/release_notes.rst
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-05 23:04:12.000000 finagg-1.0.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)    16494 2024-04-05 23:04:12.000000 finagg-1.0.0/docs/walkthroughs.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4192 2024-04-05 23:04:12.000000 finagg-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 23:04:20.961888 finagg-1.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 23:04:20.933888 finagg-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 23:04:20.945888 finagg-1.0.0/src/finagg/
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-05 23:04:12.000000 finagg-1.0.0/src/finagg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7791 2024-04-05 23:04:12.000000 finagg-1.0.0/src/finagg/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-04-05 23:04:12.000000 finagg-1.0.0/src/finagg/backend.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 23:04:20.945888 finagg-1.0.0/src/finagg/bea/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-05 23:04:12.000000 finagg-1.0.0/src/finagg/bea/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-04-05 23:04:12.000000 finagg-1.0.0/src/finagg/bea/_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    21084 2024-04-05 23:04:12.000000 finagg-1.0.0/src/finagg/bea/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-04-05 23:04:12.000000 finagg-1.0.0/src/finagg/bea/sql.py
--rw-r--r--   0 runner    (1001) docker     (127)     6696 2024-04-05 23:04:12.000000 finagg-1.0.0/src/finagg/frame.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 23:04:20.945888 finagg-1.0.0/src/finagg/fred/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-05 23:04:12.000000 finagg-1.0.0/src/finagg/fred/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5486 2024-04-05 23:04:12.000000 finagg-1.0.0/src/finagg/fred/_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 23:04:20.949888 finagg-1.0.0/src/finagg/fred/api/
--rw-r--r--   0 runner    (1001) docker     (127)     3592 2024-04-05 23:04:12.000000 finagg-1.0.0/src/finagg/fred/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3803 2024-04-05 23:04:12.000000 finagg-1.0.0/src/finagg/fred/api/_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    18869 2024-04-05 23:04:12.000000 finagg-1.0.0/src/finagg/fred/api/_category.py
--rw-r--r--   0 runner    (1001) docker     (127)    23337 2024-04-05 23:04:12.000000 finagg-1.0.0/src/finagg/fred/api/_release.py
--rw-r--r--   0 runner    (1001) docker     (127)    41472 2024-04-05 23:04:12.000000 finagg-1.0.0/src/finagg/fred/api/_series.py
--rw-r--r--   0 runner    (1001) docker     (127)     8785 2024-04-05 23:04:12.000000 finagg-1.0.0/src/finagg/fred/api/_source.py
--rw-r--r--   0 runner    (1001) docker     (127)    11656 2024-04-05 23:04:12.000000 finagg-1.0.0/src/finagg/fred/api/_tags.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 23:04:20.949888 finagg-1.0.0/src/finagg/fred/feat/
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-05 23:04:12.000000 finagg-1.0.0/src/finagg/fred/feat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6696 2024-04-05 23:04:12.000000 finagg-1.0.0/src/finagg/fred/feat/_raw.py
--rw-r--r--   0 runner    (1001) docker     (127)    10791 2024-04-05 23:04:12.000000 finagg-1.0.0/src/finagg/fred/feat/_refined.py
--rw-r--r--   0 runner    (1001) docker     (127)     3935 2024-04-05 23:04:12.000000 finagg-1.0.0/src/finagg/fred/sql.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 23:04:20.949888 finagg-1.0.0/src/finagg/fundam/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-05 23:04:12.000000 finagg-1.0.0/src/finagg/fundam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3220 2024-04-05 23:04:12.000000 finagg-1.0.0/src/finagg/fundam/_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    35182 2024-04-05 23:04:12.000000 finagg-1.0.0/src/finagg/fundam/feat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-04-05 23:04:12.000000 finagg-1.0.0/src/finagg/fundam/sql.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 23:04:20.949888 finagg-1.0.0/src/finagg/indices/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-05 23:04:12.000000 finagg-1.0.0/src/finagg/indices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2992 2024-04-05 23:04:12.000000 finagg-1.0.0/src/finagg/indices/_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     8289 2024-04-05 23:04:12.000000 finagg-1.0.0/src/finagg/indices/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-04-05 23:04:12.000000 finagg-1.0.0/src/finagg/indices/sql.py
--rw-r--r--   0 runner    (1001) docker     (127)    14390 2024-04-05 23:04:12.000000 finagg-1.0.0/src/finagg/portfolio.py
--rw-r--r--   0 runner    (1001) docker     (127)     9160 2024-04-05 23:04:12.000000 finagg-1.0.0/src/finagg/ratelimit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 23:04:20.949888 finagg-1.0.0/src/finagg/sec/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-05 23:04:12.000000 finagg-1.0.0/src/finagg/sec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8368 2024-04-05 23:04:12.000000 finagg-1.0.0/src/finagg/sec/_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    39411 2024-04-05 23:04:12.000000 finagg-1.0.0/src/finagg/sec/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 23:04:20.949888 finagg-1.0.0/src/finagg/sec/feat/
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-04-05 23:04:12.000000 finagg-1.0.0/src/finagg/sec/feat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25931 2024-04-05 23:04:12.000000 finagg-1.0.0/src/finagg/sec/feat/_raw.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 23:04:20.953888 finagg-1.0.0/src/finagg/sec/feat/_refined/
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-05 23:04:12.000000 finagg-1.0.0/src/finagg/sec/feat/_refined/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    39834 2024-04-05 23:04:12.000000 finagg-1.0.0/src/finagg/sec/feat/_refined/annual.py
--rw-r--r--   0 runner    (1001) docker     (127)    40980 2024-04-05 23:04:12.000000 finagg-1.0.0/src/finagg/sec/feat/_refined/quarterly.py
--rw-r--r--   0 runner    (1001) docker     (127)    25535 2024-04-05 23:04:12.000000 finagg-1.0.0/src/finagg/sec/sql.py
--rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-04-05 23:04:12.000000 finagg-1.0.0/src/finagg/testing.py
--rw-r--r--   0 runner    (1001) docker     (127)    12757 2024-04-05 23:04:12.000000 finagg-1.0.0/src/finagg/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 23:04:20.953888 finagg-1.0.0/src/finagg/yfinance/
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-05 23:04:12.000000 finagg-1.0.0/src/finagg/yfinance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9013 2024-04-05 23:04:12.000000 finagg-1.0.0/src/finagg/yfinance/_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2472 2024-04-05 23:04:12.000000 finagg-1.0.0/src/finagg/yfinance/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 23:04:20.953888 finagg-1.0.0/src/finagg/yfinance/feat/
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-05 23:04:12.000000 finagg-1.0.0/src/finagg/yfinance/feat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11503 2024-04-05 23:04:12.000000 finagg-1.0.0/src/finagg/yfinance/feat/_raw.py
--rw-r--r--   0 runner    (1001) docker     (127)    16476 2024-04-05 23:04:12.000000 finagg-1.0.0/src/finagg/yfinance/feat/_refined.py
--rw-r--r--   0 runner    (1001) docker     (127)     3175 2024-04-05 23:04:12.000000 finagg-1.0.0/src/finagg/yfinance/sql.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 23:04:20.957888 finagg-1.0.0/src/finagg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    27173 2024-04-05 23:04:20.000000 finagg-1.0.0/src/finagg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2608 2024-04-05 23:04:20.000000 finagg-1.0.0/src/finagg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 23:04:20.000000 finagg-1.0.0/src/finagg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-05 23:04:20.000000 finagg-1.0.0/src/finagg.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-05 23:04:20.000000 finagg-1.0.0/src/finagg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-05 23:04:20.000000 finagg-1.0.0/src/finagg.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 23:04:20.953888 finagg-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 23:04:12.000000 finagg-1.0.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 23:04:20.953888 finagg-1.0.0/tests/test_bea/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 23:04:12.000000 finagg-1.0.0/tests/test_bea/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-05 23:04:12.000000 finagg-1.0.0/tests/test_bea/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4023 2024-04-05 23:04:12.000000 finagg-1.0.0/tests/test_frame.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 23:04:20.957888 finagg-1.0.0/tests/test_fred/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 23:04:12.000000 finagg-1.0.0/tests/test_fred/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-05 23:04:12.000000 finagg-1.0.0/tests/test_fred/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-05 23:04:12.000000 finagg-1.0.0/tests/test_fred/test_feat.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 23:04:20.957888 finagg-1.0.0/tests/test_fundam/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 23:04:12.000000 finagg-1.0.0/tests/test_fundam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-04-05 23:04:12.000000 finagg-1.0.0/tests/test_fundam/test_feat.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 23:04:20.957888 finagg-1.0.0/tests/test_indices/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 23:04:12.000000 finagg-1.0.0/tests/test_indices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-05 23:04:12.000000 finagg-1.0.0/tests/test_indices/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-04-05 23:04:12.000000 finagg-1.0.0/tests/test_portfolio.py
--rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-04-05 23:04:12.000000 finagg-1.0.0/tests/test_ratelimit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 23:04:20.957888 finagg-1.0.0/tests/test_sec/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 23:04:12.000000 finagg-1.0.0/tests/test_sec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-05 23:04:12.000000 finagg-1.0.0/tests/test_sec/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4494 2024-04-05 23:04:12.000000 finagg-1.0.0/tests/test_sec/test_feat.py
--rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-04-05 23:04:12.000000 finagg-1.0.0/tests/test_sec/test_sql.py
--rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-04-05 23:04:12.000000 finagg-1.0.0/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 23:04:20.957888 finagg-1.0.0/tests/test_yfinance/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 23:04:12.000000 finagg-1.0.0/tests/test_yfinance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-05 23:04:12.000000 finagg-1.0.0/tests/test_yfinance/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3868 2024-04-05 23:04:12.000000 finagg-1.0.0/tests/test_yfinance/test_feat.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 23:57:49.072165 finagg-1.0.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 23:57:49.044165 finagg-1.0.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 23:57:49.048165 finagg-1.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-05-11 23:57:40.000000 finagg-1.0.1/.github/workflows/build-docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-11 23:57:40.000000 finagg-1.0.1/.github/workflows/test-and-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-11 23:57:40.000000 finagg-1.0.1/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-05-11 23:57:40.000000 finagg-1.0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-11 23:57:40.000000 finagg-1.0.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-11 23:57:40.000000 finagg-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    27351 2024-05-11 23:57:49.068165 finagg-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12659 2024-05-11 23:57:40.000000 finagg-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 23:57:49.052165 finagg-1.0.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 23:57:40.000000 finagg-1.0.1/docs/.nojekyll
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-11 23:57:40.000000 finagg-1.0.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 23:57:49.052165 finagg-1.0.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-11 23:57:40.000000 finagg-1.0.1/docs/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-11 23:57:40.000000 finagg-1.0.1/docs/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4239 2024-05-11 23:57:40.000000 finagg-1.0.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-05-11 23:57:40.000000 finagg-1.0.1/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9636 2024-05-11 23:57:40.000000 finagg-1.0.1/docs/conventions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1895 2024-05-11 23:57:40.000000 finagg-1.0.1/docs/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-11 23:57:40.000000 finagg-1.0.1/docs/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     8648 2024-05-11 23:57:40.000000 finagg-1.0.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-05-11 23:57:40.000000 finagg-1.0.1/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-11 23:57:40.000000 finagg-1.0.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-05-11 23:57:40.000000 finagg-1.0.1/docs/references.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-11 23:57:40.000000 finagg-1.0.1/docs/release_notes.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-11 23:57:40.000000 finagg-1.0.1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    16494 2024-05-11 23:57:40.000000 finagg-1.0.1/docs/walkthroughs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4192 2024-05-11 23:57:40.000000 finagg-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 23:57:49.072165 finagg-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 23:57:49.044165 finagg-1.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 23:57:49.056165 finagg-1.0.1/src/finagg/
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-11 23:57:40.000000 finagg-1.0.1/src/finagg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7791 2024-05-11 23:57:40.000000 finagg-1.0.1/src/finagg/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-05-11 23:57:40.000000 finagg-1.0.1/src/finagg/backend.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 23:57:49.056165 finagg-1.0.1/src/finagg/bea/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-11 23:57:40.000000 finagg-1.0.1/src/finagg/bea/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-05-11 23:57:40.000000 finagg-1.0.1/src/finagg/bea/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21084 2024-05-11 23:57:40.000000 finagg-1.0.1/src/finagg/bea/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-05-11 23:57:40.000000 finagg-1.0.1/src/finagg/bea/sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6696 2024-05-11 23:57:40.000000 finagg-1.0.1/src/finagg/frame.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 23:57:49.056165 finagg-1.0.1/src/finagg/fred/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-11 23:57:40.000000 finagg-1.0.1/src/finagg/fred/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5486 2024-05-11 23:57:40.000000 finagg-1.0.1/src/finagg/fred/_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 23:57:49.060165 finagg-1.0.1/src/finagg/fred/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     3592 2024-05-11 23:57:40.000000 finagg-1.0.1/src/finagg/fred/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3803 2024-05-11 23:57:40.000000 finagg-1.0.1/src/finagg/fred/api/_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18869 2024-05-11 23:57:40.000000 finagg-1.0.1/src/finagg/fred/api/_category.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23337 2024-05-11 23:57:40.000000 finagg-1.0.1/src/finagg/fred/api/_release.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41472 2024-05-11 23:57:40.000000 finagg-1.0.1/src/finagg/fred/api/_series.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8785 2024-05-11 23:57:40.000000 finagg-1.0.1/src/finagg/fred/api/_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11656 2024-05-11 23:57:40.000000 finagg-1.0.1/src/finagg/fred/api/_tags.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 23:57:49.060165 finagg-1.0.1/src/finagg/fred/feat/
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-11 23:57:40.000000 finagg-1.0.1/src/finagg/fred/feat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6696 2024-05-11 23:57:40.000000 finagg-1.0.1/src/finagg/fred/feat/_raw.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10791 2024-05-11 23:57:40.000000 finagg-1.0.1/src/finagg/fred/feat/_refined.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3935 2024-05-11 23:57:40.000000 finagg-1.0.1/src/finagg/fred/sql.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 23:57:49.060165 finagg-1.0.1/src/finagg/fundam/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-11 23:57:40.000000 finagg-1.0.1/src/finagg/fundam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3220 2024-05-11 23:57:40.000000 finagg-1.0.1/src/finagg/fundam/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35182 2024-05-11 23:57:40.000000 finagg-1.0.1/src/finagg/fundam/feat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-05-11 23:57:40.000000 finagg-1.0.1/src/finagg/fundam/sql.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 23:57:49.060165 finagg-1.0.1/src/finagg/indices/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-11 23:57:40.000000 finagg-1.0.1/src/finagg/indices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2992 2024-05-11 23:57:40.000000 finagg-1.0.1/src/finagg/indices/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8289 2024-05-11 23:57:40.000000 finagg-1.0.1/src/finagg/indices/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-05-11 23:57:40.000000 finagg-1.0.1/src/finagg/indices/sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14390 2024-05-11 23:57:40.000000 finagg-1.0.1/src/finagg/portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9159 2024-05-11 23:57:40.000000 finagg-1.0.1/src/finagg/ratelimit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 23:57:49.064165 finagg-1.0.1/src/finagg/sec/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-11 23:57:40.000000 finagg-1.0.1/src/finagg/sec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8368 2024-05-11 23:57:40.000000 finagg-1.0.1/src/finagg/sec/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39411 2024-05-11 23:57:40.000000 finagg-1.0.1/src/finagg/sec/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 23:57:49.064165 finagg-1.0.1/src/finagg/sec/feat/
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-11 23:57:40.000000 finagg-1.0.1/src/finagg/sec/feat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25931 2024-05-11 23:57:40.000000 finagg-1.0.1/src/finagg/sec/feat/_raw.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 23:57:49.064165 finagg-1.0.1/src/finagg/sec/feat/_refined/
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-11 23:57:40.000000 finagg-1.0.1/src/finagg/sec/feat/_refined/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39834 2024-05-11 23:57:40.000000 finagg-1.0.1/src/finagg/sec/feat/_refined/annual.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40980 2024-05-11 23:57:40.000000 finagg-1.0.1/src/finagg/sec/feat/_refined/quarterly.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25535 2024-05-11 23:57:40.000000 finagg-1.0.1/src/finagg/sec/sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-05-11 23:57:40.000000 finagg-1.0.1/src/finagg/testing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12757 2024-05-11 23:57:40.000000 finagg-1.0.1/src/finagg/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 23:57:49.064165 finagg-1.0.1/src/finagg/yfinance/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-11 23:57:40.000000 finagg-1.0.1/src/finagg/yfinance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9013 2024-05-11 23:57:40.000000 finagg-1.0.1/src/finagg/yfinance/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2472 2024-05-11 23:57:40.000000 finagg-1.0.1/src/finagg/yfinance/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 23:57:49.064165 finagg-1.0.1/src/finagg/yfinance/feat/
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-05-11 23:57:40.000000 finagg-1.0.1/src/finagg/yfinance/feat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11503 2024-05-11 23:57:40.000000 finagg-1.0.1/src/finagg/yfinance/feat/_raw.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16476 2024-05-11 23:57:40.000000 finagg-1.0.1/src/finagg/yfinance/feat/_refined.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3175 2024-05-11 23:57:40.000000 finagg-1.0.1/src/finagg/yfinance/sql.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 23:57:49.068165 finagg-1.0.1/src/finagg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    27351 2024-05-11 23:57:49.000000 finagg-1.0.1/src/finagg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2608 2024-05-11 23:57:49.000000 finagg-1.0.1/src/finagg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 23:57:49.000000 finagg-1.0.1/src/finagg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-11 23:57:49.000000 finagg-1.0.1/src/finagg.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-11 23:57:49.000000 finagg-1.0.1/src/finagg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-11 23:57:49.000000 finagg-1.0.1/src/finagg.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 23:57:49.064165 finagg-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 23:57:40.000000 finagg-1.0.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 23:57:49.064165 finagg-1.0.1/tests/test_bea/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 23:57:40.000000 finagg-1.0.1/tests/test_bea/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-11 23:57:40.000000 finagg-1.0.1/tests/test_bea/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4023 2024-05-11 23:57:40.000000 finagg-1.0.1/tests/test_frame.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 23:57:49.068165 finagg-1.0.1/tests/test_fred/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 23:57:40.000000 finagg-1.0.1/tests/test_fred/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-11 23:57:40.000000 finagg-1.0.1/tests/test_fred/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-11 23:57:40.000000 finagg-1.0.1/tests/test_fred/test_feat.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 23:57:49.068165 finagg-1.0.1/tests/test_fundam/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 23:57:40.000000 finagg-1.0.1/tests/test_fundam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-05-11 23:57:40.000000 finagg-1.0.1/tests/test_fundam/test_feat.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 23:57:49.068165 finagg-1.0.1/tests/test_indices/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 23:57:40.000000 finagg-1.0.1/tests/test_indices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-11 23:57:40.000000 finagg-1.0.1/tests/test_indices/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-05-11 23:57:40.000000 finagg-1.0.1/tests/test_portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-05-11 23:57:40.000000 finagg-1.0.1/tests/test_ratelimit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 23:57:49.068165 finagg-1.0.1/tests/test_sec/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 23:57:40.000000 finagg-1.0.1/tests/test_sec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-11 23:57:40.000000 finagg-1.0.1/tests/test_sec/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4547 2024-05-11 23:57:40.000000 finagg-1.0.1/tests/test_sec/test_feat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-05-11 23:57:40.000000 finagg-1.0.1/tests/test_sec/test_sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-05-11 23:57:40.000000 finagg-1.0.1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 23:57:49.068165 finagg-1.0.1/tests/test_yfinance/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 23:57:40.000000 finagg-1.0.1/tests/test_yfinance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-11 23:57:40.000000 finagg-1.0.1/tests/test_yfinance/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3920 2024-05-11 23:57:40.000000 finagg-1.0.1/tests/test_yfinance/test_feat.py
```

### Comparing `finagg-1.0.0/.github/workflows/build-docs.yml` & `finagg-1.0.1/.github/workflows/build-docs.yml`

 * *Files identical despite different names*

### Comparing `finagg-1.0.0/.github/workflows/test-and-publish.yml` & `finagg-1.0.1/.github/workflows/test-and-publish.yml`

 * *Files identical despite different names*

### Comparing `finagg-1.0.0/.github/workflows/test.yml` & `finagg-1.0.1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `finagg-1.0.0/.gitignore` & `finagg-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `finagg-1.0.0/.pre-commit-config.yaml` & `finagg-1.0.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `finagg-1.0.0/LICENSE` & `finagg-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `finagg-1.0.0/PKG-INFO` & `finagg-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finagg
-Version: 1.0.0
+Version: 1.0.1
 Summary: Data aggregation with popular and free financial APIs.
 Author: Andrew B.
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -244,14 +244,18 @@
 Requires-Dist: pytest-randomly; extra == "dev"
 Requires-Dist: sphinx; extra == "dev"
 Requires-Dist: tox; extra == "dev"
 Requires-Dist: virtualenv; extra == "dev"
 
 # finagg: Financial Aggregation for Python
 
+![PyPI Downloads](https://img.shields.io/pypi/dm/finagg)
+![PyPI Version](https://img.shields.io/pypi/v/finagg)
+![Python Versions](https://img.shields.io/pypi/pyversions/finagg)
+
 **finagg** is a Python package that provides implementations of popular and free
 financial APIs, tools for aggregating historical data from those APIs into SQL
 databases, and tools for transforming aggregated data into features useful for
 analysis and AI/ML.
 
 * **Documentation**: https://theogognf.github.io/finagg/
 * **PyPI**: https://pypi.org/project/finagg/
```

### Comparing `finagg-1.0.0/README.md` & `finagg-1.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # finagg: Financial Aggregation for Python
 
+![PyPI Downloads](https://img.shields.io/pypi/dm/finagg)
+![PyPI Version](https://img.shields.io/pypi/v/finagg)
+![Python Versions](https://img.shields.io/pypi/pyversions/finagg)
+
 **finagg** is a Python package that provides implementations of popular and free
 financial APIs, tools for aggregating historical data from those APIs into SQL
 databases, and tools for transforming aggregated data into features useful for
 analysis and AI/ML.
 
 * **Documentation**: https://theogognf.github.io/finagg/
 * **PyPI**: https://pypi.org/project/finagg/
```

### Comparing `finagg-1.0.0/docs/Makefile` & `finagg-1.0.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `finagg-1.0.0/docs/cli.rst` & `finagg-1.0.1/docs/cli.rst`

 * *Files identical despite different names*

### Comparing `finagg-1.0.0/docs/conf.py` & `finagg-1.0.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `finagg-1.0.0/docs/configuration.rst` & `finagg-1.0.1/docs/configuration.rst`

 * *Files identical despite different names*

### Comparing `finagg-1.0.0/docs/conventions.rst` & `finagg-1.0.1/docs/conventions.rst`

 * *Files identical despite different names*

### Comparing `finagg-1.0.0/docs/faq.rst` & `finagg-1.0.1/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `finagg-1.0.0/docs/index.rst` & `finagg-1.0.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `finagg-1.0.0/docs/installation.rst` & `finagg-1.0.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `finagg-1.0.0/docs/make.bat` & `finagg-1.0.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `finagg-1.0.0/docs/references.rst` & `finagg-1.0.1/docs/references.rst`

 * *Files identical despite different names*

### Comparing `finagg-1.0.0/docs/release_notes.rst` & `finagg-1.0.1/docs/release_notes.rst`

 * *Files 17% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 
 1.0.0
 -----
 
 Bug Fixes
 ^^^^^^^^^
 
-- Major bugfix for filtering original SEC filings affecting many SEC API and feature implementations.
+- Fix filtering original SEC filings.
 
 Compatibility Notes
 ^^^^^^^^^^^^^^^^^^^
 
 - Bump Pandas major version dependency from 1.0 to 2.0.
-- Rename ``finagg.sec.api.company_concept.join_get`` to ``finagg.sec.api.company_concept.get_multiple_original`` for clarity.
-- Rename ``finagg.sec.api.get_financial_ratios`` to ``finagg.sec.api.compute_financial_ratios`` for clarity.
-- Rename ``finagg.sec.api.get_unique_filings`` to ``finagg.sec.api.filter_original_filings`` for clarity.
-- Rename ``finagg.sec.api.join_filings`` to ``finagg.sec.api.group_and_pivot_filings`` for clarity.
-- Rename ``finagg.sec.feat.tags.join_from_raw`` to ``finagg.sec.feat.tags.group_and_pivot_from_raw`` for clarity.
+- Rename ``finagg.sec.api.company_concept.join_get`` to ``finagg.sec.api.company_concept.get_multiple_original``.
+- Rename ``finagg.sec.api.get_financial_ratios`` to ``finagg.sec.api.compute_financial_ratios``.
+- Rename ``finagg.sec.api.get_unique_filings`` to ``finagg.sec.api.filter_original_filings``.
+- Rename ``finagg.sec.api.join_filings`` to ``finagg.sec.api.group_and_pivot_filings``.
+- Rename ``finagg.sec.feat.tags.join_from_raw`` to ``finagg.sec.feat.tags.group_and_pivot_from_raw``.
 
 New Features
 ^^^^^^^^^^^^
 
-- Added ``paginate`` option to FRED API methods to enable automatic pagination of results.
+- Added ``paginate`` flag to FRED API methods for automatic pagination of results.
```

### Comparing `finagg-1.0.0/docs/walkthroughs.rst` & `finagg-1.0.1/docs/walkthroughs.rst`

 * *Files identical despite different names*

### Comparing `finagg-1.0.0/pyproject.toml` & `finagg-1.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `finagg-1.0.0/src/finagg/__main__.py` & `finagg-1.0.1/src/finagg/__main__.py`

 * *Files identical despite different names*

### Comparing `finagg-1.0.0/src/finagg/backend.py` & `finagg-1.0.1/src/finagg/backend.py`

 * *Files identical despite different names*

### Comparing `finagg-1.0.0/src/finagg/bea/_cli.py` & `finagg-1.0.1/src/finagg/bea/_cli.py`

 * *Files identical despite different names*

### Comparing `finagg-1.0.0/src/finagg/bea/api.py` & `finagg-1.0.1/src/finagg/bea/api.py`

 * *Files identical despite different names*

### Comparing `finagg-1.0.0/src/finagg/bea/sql.py` & `finagg-1.0.1/src/finagg/bea/sql.py`

 * *Files identical despite different names*

### Comparing `finagg-1.0.0/src/finagg/frame.py` & `finagg-1.0.1/src/finagg/frame.py`

 * *Files identical despite different names*

### Comparing `finagg-1.0.0/src/finagg/fred/_cli.py` & `finagg-1.0.1/src/finagg/fred/_cli.py`

 * *Files identical despite different names*

### Comparing `finagg-1.0.0/src/finagg/fred/api/__init__.py` & `finagg-1.0.1/src/finagg/fred/api/__init__.py`

 * *Files identical despite different names*

### Comparing `finagg-1.0.0/src/finagg/fred/api/_api.py` & `finagg-1.0.1/src/finagg/fred/api/_api.py`

 * *Files identical despite different names*

### Comparing `finagg-1.0.0/src/finagg/fred/api/_category.py` & `finagg-1.0.1/src/finagg/fred/api/_category.py`

 * *Files identical despite different names*

### Comparing `finagg-1.0.0/src/finagg/fred/api/_release.py` & `finagg-1.0.1/src/finagg/fred/api/_release.py`

 * *Files identical despite different names*

### Comparing `finagg-1.0.0/src/finagg/fred/api/_series.py` & `finagg-1.0.1/src/finagg/fred/api/_series.py`

 * *Files identical despite different names*

### Comparing `finagg-1.0.0/src/finagg/fred/api/_source.py` & `finagg-1.0.1/src/finagg/fred/api/_source.py`

 * *Files identical despite different names*

### Comparing `finagg-1.0.0/src/finagg/fred/api/_tags.py` & `finagg-1.0.1/src/finagg/fred/api/_tags.py`

 * *Files identical despite different names*

### Comparing `finagg-1.0.0/src/finagg/fred/feat/_raw.py` & `finagg-1.0.1/src/finagg/fred/feat/_raw.py`

 * *Files identical despite different names*

### Comparing `finagg-1.0.0/src/finagg/fred/feat/_refined.py` & `finagg-1.0.1/src/finagg/fred/feat/_refined.py`

 * *Files identical despite different names*

### Comparing `finagg-1.0.0/src/finagg/fred/sql.py` & `finagg-1.0.1/src/finagg/fred/sql.py`

 * *Files identical despite different names*

### Comparing `finagg-1.0.0/src/finagg/fundam/_cli.py` & `finagg-1.0.1/src/finagg/fundam/_cli.py`

 * *Files identical despite different names*

### Comparing `finagg-1.0.0/src/finagg/fundam/feat.py` & `finagg-1.0.1/src/finagg/fundam/feat.py`

 * *Files identical despite different names*

### Comparing `finagg-1.0.0/src/finagg/fundam/sql.py` & `finagg-1.0.1/src/finagg/fundam/sql.py`

 * *Files identical despite different names*

### Comparing `finagg-1.0.0/src/finagg/indices/_cli.py` & `finagg-1.0.1/src/finagg/indices/_cli.py`

 * *Files identical despite different names*

### Comparing `finagg-1.0.0/src/finagg/indices/api.py` & `finagg-1.0.1/src/finagg/indices/api.py`

 * *Files identical despite different names*

### Comparing `finagg-1.0.0/src/finagg/indices/sql.py` & `finagg-1.0.1/src/finagg/indices/sql.py`

 * *Files identical despite different names*

### Comparing `finagg-1.0.0/src/finagg/portfolio.py` & `finagg-1.0.1/src/finagg/portfolio.py`

 * *Files identical despite different names*

### Comparing `finagg-1.0.0/src/finagg/ratelimit.py` & `finagg-1.0.1/src/finagg/ratelimit.py`

 * *Files 0% similar despite different names*

```diff
@@ -118,15 +118,15 @@
         # Update total wait time according to the max limit.
         tmp_limit = self._total_limit
         tmp_wait = 0.0
         if self._total_limit >= self.limit:
             for r in self._responses:
                 limit, ts = r
                 tmp_limit -= limit
-                tmp_wait += self.period - (self._ts - ts)
+                tmp_wait = self.period - (self._ts - ts)
                 if tmp_limit < self.limit:
                     break
 
         self._total_wait = max(self._total_wait, tmp_wait)
         return self._total_wait
 
     @abstractmethod
```

### Comparing `finagg-1.0.0/src/finagg/sec/_cli.py` & `finagg-1.0.1/src/finagg/sec/_cli.py`

 * *Files identical despite different names*

### Comparing `finagg-1.0.0/src/finagg/sec/api.py` & `finagg-1.0.1/src/finagg/sec/api.py`

 * *Files identical despite different names*

### Comparing `finagg-1.0.0/src/finagg/sec/feat/__init__.py` & `finagg-1.0.1/src/finagg/sec/feat/__init__.py`

 * *Files identical despite different names*

### Comparing `finagg-1.0.0/src/finagg/sec/feat/_raw.py` & `finagg-1.0.1/src/finagg/sec/feat/_raw.py`

 * *Files identical despite different names*

### Comparing `finagg-1.0.0/src/finagg/sec/feat/_refined/annual.py` & `finagg-1.0.1/src/finagg/sec/feat/_refined/annual.py`

 * *Files identical despite different names*

### Comparing `finagg-1.0.0/src/finagg/sec/feat/_refined/quarterly.py` & `finagg-1.0.1/src/finagg/sec/feat/_refined/quarterly.py`

 * *Files identical despite different names*

### Comparing `finagg-1.0.0/src/finagg/sec/sql.py` & `finagg-1.0.1/src/finagg/sec/sql.py`

 * *Files identical despite different names*

### Comparing `finagg-1.0.0/src/finagg/testing.py` & `finagg-1.0.1/src/finagg/testing.py`

 * *Files identical despite different names*

### Comparing `finagg-1.0.0/src/finagg/utils.py` & `finagg-1.0.1/src/finagg/utils.py`

 * *Files identical despite different names*

### Comparing `finagg-1.0.0/src/finagg/yfinance/_cli.py` & `finagg-1.0.1/src/finagg/yfinance/_cli.py`

 * *Files identical despite different names*

### Comparing `finagg-1.0.0/src/finagg/yfinance/api.py` & `finagg-1.0.1/src/finagg/yfinance/api.py`

 * *Files identical despite different names*

### Comparing `finagg-1.0.0/src/finagg/yfinance/feat/_raw.py` & `finagg-1.0.1/src/finagg/yfinance/feat/_raw.py`

 * *Files identical despite different names*

### Comparing `finagg-1.0.0/src/finagg/yfinance/feat/_refined.py` & `finagg-1.0.1/src/finagg/yfinance/feat/_refined.py`

 * *Files identical despite different names*

### Comparing `finagg-1.0.0/src/finagg/yfinance/sql.py` & `finagg-1.0.1/src/finagg/yfinance/sql.py`

 * *Files identical despite different names*

### Comparing `finagg-1.0.0/src/finagg.egg-info/PKG-INFO` & `finagg-1.0.1/src/finagg.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finagg
-Version: 1.0.0
+Version: 1.0.1
 Summary: Data aggregation with popular and free financial APIs.
 Author: Andrew B.
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -244,14 +244,18 @@
 Requires-Dist: pytest-randomly; extra == "dev"
 Requires-Dist: sphinx; extra == "dev"
 Requires-Dist: tox; extra == "dev"
 Requires-Dist: virtualenv; extra == "dev"
 
 # finagg: Financial Aggregation for Python
 
+![PyPI Downloads](https://img.shields.io/pypi/dm/finagg)
+![PyPI Version](https://img.shields.io/pypi/v/finagg)
+![Python Versions](https://img.shields.io/pypi/pyversions/finagg)
+
 **finagg** is a Python package that provides implementations of popular and free
 financial APIs, tools for aggregating historical data from those APIs into SQL
 databases, and tools for transforming aggregated data into features useful for
 analysis and AI/ML.
 
 * **Documentation**: https://theogognf.github.io/finagg/
 * **PyPI**: https://pypi.org/project/finagg/
```

### Comparing `finagg-1.0.0/src/finagg.egg-info/SOURCES.txt` & `finagg-1.0.1/src/finagg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `finagg-1.0.0/tests/test_frame.py` & `finagg-1.0.1/tests/test_frame.py`

 * *Files identical despite different names*

### Comparing `finagg-1.0.0/tests/test_fred/test_feat.py` & `finagg-1.0.1/tests/test_fred/test_feat.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,19 @@
+from typing import Generator
+
 import pandas as pd
 import pytest
 from sqlalchemy.engine import Engine
 from sqlalchemy.exc import IntegrityError
 
 import finagg
 
 
 @pytest.fixture
-def engine() -> Engine:
+def engine() -> Generator[Engine, None, None]:
     yield from finagg.testing.sqlite_engine(
         finagg.backend.database_path, table=finagg.fred.sql.economic
     )
 
 
 def test_economic_all_equal(engine: Engine) -> None:
     finagg.fred.feat.series.install(engine=engine)
```

### Comparing `finagg-1.0.0/tests/test_fundam/test_feat.py` & `finagg-1.0.1/tests/test_fundam/test_feat.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,19 @@
+from typing import Generator
+
 import pandas as pd
 import pytest
 from sqlalchemy.engine import Engine
 from sqlalchemy.exc import IntegrityError
 
 import finagg
 
 
 @pytest.fixture
-def engine() -> Engine:
+def engine() -> Generator[Engine, None, None]:
     yield from finagg.testing.sqlite_engine(
         finagg.backend.database_path, metadata=finagg.fundam.sql.metadata
     )
 
 
 def test_fundam_get_candidate_ticker_set(engine: Engine) -> None:
     finagg.yfinance.feat.prices.install({"AAPL"}, engine=engine)
```

### Comparing `finagg-1.0.0/tests/test_portfolio.py` & `finagg-1.0.1/tests/test_portfolio.py`

 * *Files identical despite different names*

### Comparing `finagg-1.0.0/tests/test_ratelimit.py` & `finagg-1.0.1/tests/test_ratelimit.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from typing import Generator
 from unittest.mock import patch
 
 import pytest
 import requests
 
 import finagg.ratelimit
 
@@ -14,15 +15,15 @@
         if hasattr(response, "from_cache") and response.from_cache:
             return 0.0
         wait = 100 if response.status_code != 200 else 0.0
         return {"limit": 1.0, "wait": wait}
 
 
 @pytest.fixture
-def expected_wait() -> list[int]:
+def expected_wait() -> Generator[list[int], None, None]:
     """Mock `time.perf_counter` and yield the expected test results.
 
     The first side effect goes to an internal dummy call.
     The response deques for each limiter before and after responses
     are filtered (assuming a limit of 3 and period of 10):
 
     Response appended       Responses filtered
```

### Comparing `finagg-1.0.0/tests/test_sec/test_feat.py` & `finagg-1.0.1/tests/test_sec/test_feat.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,19 @@
+from typing import Generator
+
 import pandas as pd
 import pytest
 from sqlalchemy.engine import Engine
 from sqlalchemy.exc import IntegrityError
 
 import finagg
 
 
 @pytest.fixture
-def engine() -> Engine:
+def engine() -> Generator[Engine, None, None]:
     yield from finagg.testing.sqlite_engine(
         finagg.backend.database_path, metadata=finagg.sec.sql.metadata
     )
 
 
 def test_annual_all_equal(engine: Engine) -> None:
     finagg.sec.feat.submissions.install({"AAPL"}, engine=engine)
```

### Comparing `finagg-1.0.0/tests/test_sec/test_sql.py` & `finagg-1.0.1/tests/test_sec/test_sql.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,17 @@
+from typing import Generator
+
 import pytest
 from sqlalchemy.engine import Engine
 
 import finagg
 
 
 @pytest.fixture
-def engine() -> Engine:
+def engine() -> Generator[Engine, None, None]:
     yield from finagg.testing.sqlite_engine(
         finagg.backend.database_path, metadata=finagg.sec.sql.metadata
     )
 
 
 def test_get_cik(engine: Engine) -> None:
     finagg.sec.feat.submissions.install({"AAPL"}, engine=engine)
```

### Comparing `finagg-1.0.0/tests/test_utils.py` & `finagg-1.0.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `finagg-1.0.0/tests/test_yfinance/test_feat.py` & `finagg-1.0.1/tests/test_yfinance/test_feat.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from datetime import datetime, timedelta
+from typing import Generator
 
 import pandas as pd
 import pytest
 from sqlalchemy.engine import Engine
 from sqlalchemy.exc import IntegrityError
 
 import finagg
 
 
 @pytest.fixture
-def engine() -> Engine:
+def engine() -> Generator[Engine, None, None]:
     yield from finagg.testing.sqlite_engine(
         finagg.backend.database_path, table=finagg.yfinance.sql.daily
     )
 
 
 def test_daily_all_equal(engine: Engine) -> None:
     finagg.yfinance.feat.prices.install({"AAPL"}, engine=engine)
```

