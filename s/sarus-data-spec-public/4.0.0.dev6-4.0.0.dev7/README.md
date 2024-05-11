# Comparing `tmp/sarus_data_spec_public-4.0.0.dev6.tar.gz` & `tmp/sarus_data_spec_public-4.0.0.dev7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sarus_data_spec_public-4.0.0.dev6.tar", last modified: Thu Apr 11 13:01:21 2024, max compression
+gzip compressed data, was "sarus_data_spec_public-4.0.0.dev7.tar", last modified: Sat May 11 22:39:24 2024, max compression
```

## Comparing `sarus_data_spec_public-4.0.0.dev6.tar` & `sarus_data_spec_public-4.0.0.dev7.tar`

### file list

```diff
@@ -1,223 +1,223 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 13:01:21.931416 sarus_data_spec_public-4.0.0.dev6/
--rw-rw-rw-   0 root         (0) root         (0)      139 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      661 2024-04-11 13:01:21.931416 sarus_data_spec_public-4.0.0.dev6/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      134 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 13:01:21.890416 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/
--rwxrwxrwx   0 root         (0) root         (0)      947 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 13:01:21.892417 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/arrow/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/arrow/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8407 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/arrow/admin_utils.py
--rw-rw-rw-   0 root         (0) root         (0)      458 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/arrow/array.py
--rw-rw-rw-   0 root         (0) root         (0)     7264 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/arrow/conversion.py
--rw-rw-rw-   0 root         (0) root         (0)     2101 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/arrow/pandas_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     6266 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/arrow/schema.py
--rw-rw-rw-   0 root         (0) root         (0)    10718 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/arrow/type.py
--rw-rw-rw-   0 root         (0) root         (0)     1014 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/attribute.py
--rw-rw-rw-   0 root         (0) root         (0)     4646 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/base.py
--rw-rw-rw-   0 root         (0) root         (0)     1488 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/bounds.py
--rw-rw-rw-   0 root         (0) root         (0)     4185 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 13:01:21.893417 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/context/
--rw-rw-rw-   0 root         (0) root         (0)      266 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/context/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1331 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/context/public.py
--rw-rw-rw-   0 root         (0) root         (0)      361 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/context/state.py
--rw-rw-rw-   0 root         (0) root         (0)      985 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/context/typing.py
--rw-rw-rw-   0 root         (0) root         (0)    21741 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/dataset.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 13:01:21.894417 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/dataspec_rewriter/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/dataspec_rewriter/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2314 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/dataspec_rewriter/base.py
--rw-rw-rw-   0 root         (0) root         (0)     4997 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/dataspec_rewriter/graph_query_builder_utils.py
--rw-rw-rw-   0 root         (0) root         (0)    22994 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/dataspec_rewriter/recursive_rewriter.py
--rw-rw-rw-   0 root         (0) root         (0)    11623 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/dataspec_rewriter/simple_rules.py
--rw-rw-rw-   0 root         (0) root         (0)      837 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/dataspec_rewriter/typing.py
--rw-rw-rw-   0 root         (0) root         (0)     3438 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/dataspec_rewriter/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 13:01:21.896417 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/dataspec_validator/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/dataspec_validator/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    17255 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/dataspec_validator/base.py
--rw-rw-rw-   0 root         (0) root         (0)     3941 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/dataspec_validator/parameter_kind.py
--rw-rw-rw-   0 root         (0) root         (0)      815 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/dataspec_validator/privacy_limit.py
--rw-rw-rw-   0 root         (0) root         (0)     5717 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/dataspec_validator/recursive_validator.py
--rw-rw-rw-   0 root         (0) root         (0)    28906 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/dataspec_validator/signature.py
--rw-rw-rw-   0 root         (0) root         (0)     4161 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/dataspec_validator/simple_rules.py
--rw-rw-rw-   0 root         (0) root         (0)     5355 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/dataspec_validator/typing.py
--rw-rw-rw-   0 root         (0) root         (0)     8867 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/deprecation.py
--rw-rw-rw-   0 root         (0) root         (0)     1584 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/factory.py
--rw-rw-rw-   0 root         (0) root         (0)     8679 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/json_serialisation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 13:01:21.897416 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7629 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/async_utils.py
--rw-rw-rw-   0 root         (0) root         (0)    31915 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/base.py
--rw-rw-rw-   0 root         (0) root         (0)     6724 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/cache_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 13:01:21.898417 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/computations/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/computations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9104 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/computations/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 13:01:21.898417 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/computations/local/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/computations/local/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3892 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/computations/local/base.py
--rw-rw-rw-   0 root         (0) root         (0)     2583 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/computations/local/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 13:01:21.899417 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/computations/remote/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/computations/remote/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3302 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/computations/remote/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 13:01:21.899417 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/
--rw-rw-rw-   0 root         (0) root         (0)      173 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7120 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 13:01:21.900416 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 13:01:21.903416 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/
--rw-rw-rw-   0 root         (0) root         (0)     2662 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    23081 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/external_op.py
--rw-rw-rw-   0 root         (0) root         (0)     3011 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/imblearn.py
--rw-rw-rw-   0 root         (0) root         (0)    10321 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/numpy.py
--rw-rw-rw-   0 root         (0) root         (0)    21505 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/optbinning.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 13:01:21.904416 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/pandas/
--rw-rw-rw-   0 root         (0) root         (0)      162 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/pandas/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8155 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/pandas/groupby.py
--rw-rw-rw-   0 root         (0) root         (0)    32015 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/pandas/groupby_dp.py
--rw-rw-rw-   0 root         (0) root         (0)    78764 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/pandas/pandas.py
--rw-rw-rw-   0 root         (0) root         (0)    37535 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/pandas/pandas_dp.py
--rw-rw-rw-   0 root         (0) root         (0)     2807 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/pandas_profiling.py
--rw-rw-rw-   0 root         (0) root         (0)    34976 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/scipy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 13:01:21.906417 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/shap/
--rw-rw-rw-   0 root         (0) root         (0)     4162 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/shap/Explanation.py
--rw-rw-rw-   0 root         (0) root         (0)      132 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/shap/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    26932 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/shap/explainer.py
--rw-rw-rw-   0 root         (0) root         (0)    13453 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/shap/maskers.py
--rw-rw-rw-   0 root         (0) root         (0)    14139 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/shap/plots.py
--rw-rw-rw-   0 root         (0) root         (0)     6514 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/shap/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 13:01:21.909416 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/sklearn/
--rw-rw-rw-   0 root         (0) root         (0)      335 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/sklearn/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    20941 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/sklearn/cluster.py
--rw-rw-rw-   0 root         (0) root         (0)     1931 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/sklearn/compose.py
--rw-rw-rw-   0 root         (0) root         (0)     1902 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/sklearn/decomposition.py
--rw-rw-rw-   0 root         (0) root         (0)    38069 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/sklearn/ensemble.py
--rw-rw-rw-   0 root         (0) root         (0)     1678 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/sklearn/impute.py
--rw-rw-rw-   0 root         (0) root         (0)     2084 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/sklearn/inspection.py
--rw-rw-rw-   0 root         (0) root         (0)     9874 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/sklearn/lib.py
--rw-rw-rw-   0 root         (0) root         (0)     3294 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/sklearn/linear_model.py
--rw-rw-rw-   0 root         (0) root         (0)    12690 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/sklearn/metrics.py
--rw-rw-rw-   0 root         (0) root         (0)     8598 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/sklearn/model_selection.py
--rw-rw-rw-   0 root         (0) root         (0)     1058 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/sklearn/pipeline.py
--rw-rw-rw-   0 root         (0) root         (0)     4340 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/sklearn/preprocessing.py
--rw-rw-rw-   0 root         (0) root         (0)     2645 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/sklearn/svm.py
--rw-rw-rw-   0 root         (0) root         (0)     2884 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/skopt.py
--rw-rw-rw-   0 root         (0) root         (0)    25448 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/std.py
--rw-rw-rw-   0 root         (0) root         (0)     3011 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/typing.py
--rw-rw-rw-   0 root         (0) root         (0)     1359 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/utils.py
--rw-rw-rw-   0 root         (0) root         (0)    14158 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/xgboost.py
--rw-rw-rw-   0 root         (0) root         (0)    13072 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/routing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 13:01:21.912416 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/standard/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/standard/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    17192 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/standard/differentiated_sample.py
--rw-rw-rw-   0 root         (0) root         (0)     1625 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/standard/error_estimation.py
--rw-rw-rw-   0 root         (0) root         (0)     1474 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/standard/extract.py
--rw-rw-rw-   0 root         (0) root         (0)    12256 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/standard/filter.py
--rw-rw-rw-   0 root         (0) root         (0)     2922 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/standard/generate_from_model.py
--rw-rw-rw-   0 root         (0) root         (0)    12893 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/standard/get_item.py
--rw-rw-rw-   0 root         (0) root         (0)    11420 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/standard/project.py
--rw-rw-rw-   0 root         (0) root         (0)     8567 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/standard/sample.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 13:01:21.913416 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/standard/sampling/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/standard/sampling/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3647 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/standard/sampling/differentiated_sampling_sizes.py
--rw-rw-rw-   0 root         (0) root         (0)     2462 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/standard/shuffle.py
--rw-rw-rw-   0 root         (0) root         (0)     9522 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/standard/standard_op.py
--rw-rw-rw-   0 root         (0) root         (0)    11403 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/standard/synthetic.py
--rw-rw-rw-   0 root         (0) root         (0)    13558 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/standard/to_small_data.py
--rw-rw-rw-   0 root         (0) root         (0)    27871 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/standard/visitor_selector.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 13:01:21.914416 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/source/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/source/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      497 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/source/privacy_params.py
--rw-rw-rw-   0 root         (0) root         (0)      269 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/source/random_seed.py
--rw-rw-rw-   0 root         (0) root         (0)     3320 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/source/routing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 13:01:21.914416 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/sql_utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/sql_utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8893 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/sql_utils/bigdata.py
--rw-rw-rw-   0 root         (0) root         (0)     5703 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/sql_utils/queries.py
--rw-rw-rw-   0 root         (0) root         (0)    10279 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/typing.py
--rw-rw-rw-   0 root         (0) root         (0)     1521 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/marginals.py
--rw-rw-rw-   0 root         (0) root         (0)     1548 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/multiplicity.py
--rw-rw-rw-   0 root         (0) root         (0)     3376 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/path.py
--rw-rw-rw-   0 root         (0) root         (0)     3004 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/predicate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 13:01:21.928416 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/
--rw-rw-rw-   0 root         (0) root         (0)     2628 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      244 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/attribute.proto
--rw-r--r--   0 root         (0) root         (0)     1507 2024-04-11 13:01:10.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/attribute_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1840 2024-04-11 13:01:10.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/attribute_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      251 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/bounds.proto
--rw-r--r--   0 root         (0) root         (0)     1712 2024-04-11 13:01:10.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/bounds_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2160 2024-04-11 13:01:10.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/bounds_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      348 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/constraint.proto
--rw-r--r--   0 root         (0) root         (0)     1964 2024-04-11 13:01:10.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/constraint_pb2.py
--rw-r--r--   0 root         (0) root         (0)     3236 2024-04-11 13:01:10.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/constraint_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)     1340 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/dataset.proto
--rw-r--r--   0 root         (0) root         (0)     3941 2024-04-11 13:01:10.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/dataset_pb2.py
--rw-r--r--   0 root         (0) root         (0)     9653 2024-04-11 13:01:10.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/dataset_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      470 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/links.proto
--rw-r--r--   0 root         (0) root         (0)     2557 2024-04-11 13:01:10.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/links_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4178 2024-04-11 13:01:10.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/links_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      244 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/manager.proto
--rw-r--r--   0 root         (0) root         (0)     1417 2024-04-11 13:01:10.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/manager_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1638 2024-04-11 13:01:10.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/manager_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      254 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/marginals.proto
--rw-r--r--   0 root         (0) root         (0)     1739 2024-04-11 13:01:10.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/marginals_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2169 2024-04-11 13:01:10.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/marginals_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      257 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/multiplicity.proto
--rw-r--r--   0 root         (0) root         (0)     1777 2024-04-11 13:01:10.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/multiplicity_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2178 2024-04-11 13:01:10.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/multiplicity_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      153 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/path.proto
--rw-r--r--   0 root         (0) root         (0)     1449 2024-04-11 13:01:10.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/path_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1730 2024-04-11 13:01:10.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/path_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      550 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/predicate.proto
--rw-r--r--   0 root         (0) root         (0)     2416 2024-04-11 13:01:10.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/predicate_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4839 2024-04-11 13:01:10.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/predicate_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      259 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/proto_container.proto
--rw-r--r--   0 root         (0) root         (0)     1634 2024-04-11 13:01:10.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/proto_container_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1821 2024-04-11 13:01:10.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/proto_container_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      629 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/relation.proto
--rw-r--r--   0 root         (0) root         (0)     1545 2024-04-11 13:01:10.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/relation_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2606 2024-04-11 13:01:10.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/relation_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)     1798 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/scalar.proto
--rw-r--r--   0 root         (0) root         (0)     3904 2024-04-11 13:01:10.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/scalar_pb2.py
--rw-r--r--   0 root         (0) root         (0)     9843 2024-04-11 13:01:10.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/scalar_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      694 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/schema.proto
--rw-r--r--   0 root         (0) root         (0)     2611 2024-04-11 13:01:10.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/schema_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4578 2024-04-11 13:01:10.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/schema_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      249 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/size.proto
--rw-r--r--   0 root         (0) root         (0)     1689 2024-04-11 13:01:10.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/size_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2154 2024-04-11 13:01:10.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/size_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)     3909 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/statistics.proto
--rw-r--r--   0 root         (0) root         (0)    11222 2024-04-11 13:01:10.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/statistics_pb2.py
--rw-r--r--   0 root         (0) root         (0)    32747 2024-04-11 13:01:10.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/statistics_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      646 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/status.proto
--rw-r--r--   0 root         (0) root         (0)     3258 2024-04-11 13:01:10.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/status_pb2.py
--rw-r--r--   0 root         (0) root         (0)     6181 2024-04-11 13:01:10.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/status_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)     6970 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/transform.proto
--rw-r--r--   0 root         (0) root         (0)    16759 2024-04-11 13:01:10.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/transform_pb2.py
--rw-r--r--   0 root         (0) root         (0)    48797 2024-04-11 13:01:10.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/transform_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)     4567 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/type.proto
--rw-r--r--   0 root         (0) root         (0)     9784 2024-04-11 13:01:10.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/type_pb2.py
--rw-r--r--   0 root         (0) root         (0)    30590 2024-04-11 13:01:10.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/type_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      917 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/typing.py
--rw-rw-rw-   0 root         (0) root         (0)     3948 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/utilities.py
--rwxrwxrwx   0 root         (0) root         (0)        0 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/py.typed
--rw-rw-rw-   0 root         (0) root         (0)    13753 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/scalar.py
--rw-rw-rw-   0 root         (0) root         (0)     4757 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     1467 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/size.py
--rw-rw-rw-   0 root         (0) root         (0)    43603 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/statistics.py
--rw-rw-rw-   0 root         (0) root         (0)    17261 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/status.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 13:01:21.929416 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/storage/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/storage/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    14527 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/storage/local.py
--rw-rw-rw-   0 root         (0) root         (0)     5606 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/storage/typing.py
--rw-rw-rw-   0 root         (0) root         (0)     3084 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/storage/utils.py
--rw-rw-rw-   0 root         (0) root         (0)    40022 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/transform.py
--rw-rw-rw-   0 root         (0) root         (0)   123297 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/type.py
--rw-rw-rw-   0 root         (0) root         (0)    40869 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/typing.py
--rw-rw-rw-   0 root         (0) root         (0)     4998 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/variant_constraint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 13:01:21.930416 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec_public.egg-info/
--rw-r--r--   0 root         (0) root         (0)      661 2024-04-11 13:01:21.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec_public.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9090 2024-04-11 13:01:21.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec_public.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-11 13:01:21.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec_public.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-11 13:01:21.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec_public.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      125 2024-04-11 13:01:21.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec_public.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2024-04-11 13:01:21.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec_public.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     6927 2024-04-11 13:01:21.932416 sarus_data_spec_public-4.0.0.dev6/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1191 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 22:39:24.153491 sarus_data_spec_public-4.0.0.dev7/
+-rw-rw-rw-   0 root         (0) root         (0)      139 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      661 2024-05-11 22:39:24.153491 sarus_data_spec_public-4.0.0.dev7/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      134 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 22:39:24.110487 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/
+-rwxrwxrwx   0 root         (0) root         (0)      947 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 22:39:24.112487 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/arrow/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/arrow/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8845 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/arrow/admin_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2178 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/arrow/array.py
+-rw-rw-rw-   0 root         (0) root         (0)     7304 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/arrow/conversion.py
+-rw-rw-rw-   0 root         (0) root         (0)     2100 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/arrow/pandas_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     6266 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/arrow/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)    10718 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/arrow/type.py
+-rw-rw-rw-   0 root         (0) root         (0)     1014 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/attribute.py
+-rw-rw-rw-   0 root         (0) root         (0)     4646 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1488 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/bounds.py
+-rw-rw-rw-   0 root         (0) root         (0)     4185 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 22:39:24.113488 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/context/
+-rw-rw-rw-   0 root         (0) root         (0)      266 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/context/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1331 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/context/public.py
+-rw-rw-rw-   0 root         (0) root         (0)      361 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/context/state.py
+-rw-rw-rw-   0 root         (0) root         (0)      985 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/context/typing.py
+-rw-rw-rw-   0 root         (0) root         (0)    21741 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/dataset.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 22:39:24.115488 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/dataspec_rewriter/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/dataspec_rewriter/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2314 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/dataspec_rewriter/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     4997 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/dataspec_rewriter/graph_query_builder_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    22994 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/dataspec_rewriter/recursive_rewriter.py
+-rw-rw-rw-   0 root         (0) root         (0)    11623 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/dataspec_rewriter/simple_rules.py
+-rw-rw-rw-   0 root         (0) root         (0)      837 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/dataspec_rewriter/typing.py
+-rw-rw-rw-   0 root         (0) root         (0)     3438 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/dataspec_rewriter/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 22:39:24.116488 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/dataspec_validator/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/dataspec_validator/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    17255 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/dataspec_validator/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     3941 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/dataspec_validator/parameter_kind.py
+-rw-rw-rw-   0 root         (0) root         (0)      815 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/dataspec_validator/privacy_limit.py
+-rw-rw-rw-   0 root         (0) root         (0)     5717 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/dataspec_validator/recursive_validator.py
+-rw-rw-rw-   0 root         (0) root         (0)    28906 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/dataspec_validator/signature.py
+-rw-rw-rw-   0 root         (0) root         (0)     4161 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/dataspec_validator/simple_rules.py
+-rw-rw-rw-   0 root         (0) root         (0)     5355 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/dataspec_validator/typing.py
+-rw-rw-rw-   0 root         (0) root         (0)     8867 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/deprecation.py
+-rw-rw-rw-   0 root         (0) root         (0)     1584 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     8679 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/json_serialisation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 22:39:24.118488 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7629 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/async_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    32029 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     6724 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/cache_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 22:39:24.118488 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/computations/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/computations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9104 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/computations/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 22:39:24.119488 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/computations/local/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/computations/local/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3892 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/computations/local/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     2583 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/computations/local/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 22:39:24.119488 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/computations/remote/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/computations/remote/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3302 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/computations/remote/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 22:39:24.120488 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/
+-rw-rw-rw-   0 root         (0) root         (0)      173 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7120 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 22:39:24.120488 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 22:39:24.123489 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/
+-rw-rw-rw-   0 root         (0) root         (0)     2662 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    23081 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/external_op.py
+-rw-rw-rw-   0 root         (0) root         (0)     3011 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/imblearn.py
+-rw-rw-rw-   0 root         (0) root         (0)    10321 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/numpy.py
+-rw-rw-rw-   0 root         (0) root         (0)    21505 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/optbinning.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 22:39:24.125489 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/pandas/
+-rw-rw-rw-   0 root         (0) root         (0)      162 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/pandas/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8155 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/pandas/groupby.py
+-rw-rw-rw-   0 root         (0) root         (0)    32015 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/pandas/groupby_dp.py
+-rw-rw-rw-   0 root         (0) root         (0)    78764 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/pandas/pandas.py
+-rw-rw-rw-   0 root         (0) root         (0)    37673 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/pandas/pandas_dp.py
+-rw-rw-rw-   0 root         (0) root         (0)     2807 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/pandas_profiling.py
+-rw-rw-rw-   0 root         (0) root         (0)    34976 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/scipy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 22:39:24.127489 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/shap/
+-rw-rw-rw-   0 root         (0) root         (0)     4162 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/shap/Explanation.py
+-rw-rw-rw-   0 root         (0) root         (0)      132 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/shap/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    26932 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/shap/explainer.py
+-rw-rw-rw-   0 root         (0) root         (0)    13453 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/shap/maskers.py
+-rw-rw-rw-   0 root         (0) root         (0)    14139 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/shap/plots.py
+-rw-rw-rw-   0 root         (0) root         (0)     6514 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/shap/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 22:39:24.130489 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/sklearn/
+-rw-rw-rw-   0 root         (0) root         (0)      335 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/sklearn/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    20941 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/sklearn/cluster.py
+-rw-rw-rw-   0 root         (0) root         (0)     1931 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/sklearn/compose.py
+-rw-rw-rw-   0 root         (0) root         (0)     1902 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/sklearn/decomposition.py
+-rw-rw-rw-   0 root         (0) root         (0)    38069 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/sklearn/ensemble.py
+-rw-rw-rw-   0 root         (0) root         (0)     1678 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/sklearn/impute.py
+-rw-rw-rw-   0 root         (0) root         (0)     2084 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/sklearn/inspection.py
+-rw-rw-rw-   0 root         (0) root         (0)     9874 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/sklearn/lib.py
+-rw-rw-rw-   0 root         (0) root         (0)     3294 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/sklearn/linear_model.py
+-rw-rw-rw-   0 root         (0) root         (0)    12690 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/sklearn/metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)     8598 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/sklearn/model_selection.py
+-rw-rw-rw-   0 root         (0) root         (0)     1058 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/sklearn/pipeline.py
+-rw-rw-rw-   0 root         (0) root         (0)     4340 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/sklearn/preprocessing.py
+-rw-rw-rw-   0 root         (0) root         (0)     2645 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/sklearn/svm.py
+-rw-rw-rw-   0 root         (0) root         (0)     2884 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/skopt.py
+-rw-rw-rw-   0 root         (0) root         (0)    25448 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/std.py
+-rw-rw-rw-   0 root         (0) root         (0)     3011 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/typing.py
+-rw-rw-rw-   0 root         (0) root         (0)     1359 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    14158 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/xgboost.py
+-rw-rw-rw-   0 root         (0) root         (0)    13076 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/routing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 22:39:24.134489 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/standard/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/standard/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    17193 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/standard/differentiated_sample.py
+-rw-rw-rw-   0 root         (0) root         (0)     1625 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/standard/error_estimation.py
+-rw-rw-rw-   0 root         (0) root         (0)     1474 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/standard/extract.py
+-rw-rw-rw-   0 root         (0) root         (0)    12256 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/standard/filter.py
+-rw-rw-rw-   0 root         (0) root         (0)     2922 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/standard/generate_from_model.py
+-rw-rw-rw-   0 root         (0) root         (0)    12893 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/standard/get_item.py
+-rw-rw-rw-   0 root         (0) root         (0)    11420 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/standard/project.py
+-rw-rw-rw-   0 root         (0) root         (0)     8567 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/standard/sample.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 22:39:24.134489 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/standard/sampling/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/standard/sampling/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3647 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/standard/sampling/differentiated_sampling_sizes.py
+-rw-rw-rw-   0 root         (0) root         (0)     2462 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/standard/shuffle.py
+-rw-rw-rw-   0 root         (0) root         (0)     9522 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/standard/standard_op.py
+-rw-rw-rw-   0 root         (0) root         (0)    11403 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/standard/synthetic.py
+-rw-rw-rw-   0 root         (0) root         (0)    13558 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/standard/to_small_data.py
+-rw-rw-rw-   0 root         (0) root         (0)    27871 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/standard/visitor_selector.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 22:39:24.135490 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/source/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/source/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      497 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/source/privacy_params.py
+-rw-rw-rw-   0 root         (0) root         (0)      269 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/source/random_seed.py
+-rw-rw-rw-   0 root         (0) root         (0)     3320 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/source/routing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 22:39:24.136490 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/sql_utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/sql_utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8893 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/sql_utils/bigdata.py
+-rw-rw-rw-   0 root         (0) root         (0)     5703 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/sql_utils/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)    10377 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/typing.py
+-rw-rw-rw-   0 root         (0) root         (0)     1521 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/marginals.py
+-rw-rw-rw-   0 root         (0) root         (0)     1548 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/multiplicity.py
+-rw-rw-rw-   0 root         (0) root         (0)     3376 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/path.py
+-rw-rw-rw-   0 root         (0) root         (0)     3004 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/predicate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 22:39:24.150491 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/
+-rw-rw-rw-   0 root         (0) root         (0)     2628 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      244 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/attribute.proto
+-rw-r--r--   0 root         (0) root         (0)     1507 2024-05-11 22:39:12.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/attribute_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1840 2024-05-11 22:39:12.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/attribute_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      251 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/bounds.proto
+-rw-r--r--   0 root         (0) root         (0)     1712 2024-05-11 22:39:12.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/bounds_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2160 2024-05-11 22:39:12.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/bounds_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      348 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/constraint.proto
+-rw-r--r--   0 root         (0) root         (0)     1964 2024-05-11 22:39:12.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/constraint_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     3236 2024-05-11 22:39:12.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/constraint_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     1340 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/dataset.proto
+-rw-r--r--   0 root         (0) root         (0)     3941 2024-05-11 22:39:12.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/dataset_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     9653 2024-05-11 22:39:12.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/dataset_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      470 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/links.proto
+-rw-r--r--   0 root         (0) root         (0)     2557 2024-05-11 22:39:12.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/links_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4178 2024-05-11 22:39:12.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/links_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      244 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/manager.proto
+-rw-r--r--   0 root         (0) root         (0)     1417 2024-05-11 22:39:12.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/manager_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1638 2024-05-11 22:39:12.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/manager_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      254 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/marginals.proto
+-rw-r--r--   0 root         (0) root         (0)     1739 2024-05-11 22:39:12.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/marginals_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2169 2024-05-11 22:39:12.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/marginals_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      257 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/multiplicity.proto
+-rw-r--r--   0 root         (0) root         (0)     1777 2024-05-11 22:39:12.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/multiplicity_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2178 2024-05-11 22:39:12.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/multiplicity_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      153 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/path.proto
+-rw-r--r--   0 root         (0) root         (0)     1449 2024-05-11 22:39:12.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/path_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1730 2024-05-11 22:39:12.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/path_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      550 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/predicate.proto
+-rw-r--r--   0 root         (0) root         (0)     2416 2024-05-11 22:39:12.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/predicate_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4839 2024-05-11 22:39:12.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/predicate_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      259 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/proto_container.proto
+-rw-r--r--   0 root         (0) root         (0)     1634 2024-05-11 22:39:12.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/proto_container_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1821 2024-05-11 22:39:12.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/proto_container_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      629 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/relation.proto
+-rw-r--r--   0 root         (0) root         (0)     1545 2024-05-11 22:39:12.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/relation_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2606 2024-05-11 22:39:12.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/relation_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     1798 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/scalar.proto
+-rw-r--r--   0 root         (0) root         (0)     3904 2024-05-11 22:39:12.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/scalar_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     9843 2024-05-11 22:39:12.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/scalar_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      694 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/schema.proto
+-rw-r--r--   0 root         (0) root         (0)     2611 2024-05-11 22:39:12.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/schema_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4578 2024-05-11 22:39:12.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/schema_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      249 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/size.proto
+-rw-r--r--   0 root         (0) root         (0)     1689 2024-05-11 22:39:12.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/size_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2154 2024-05-11 22:39:12.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/size_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     3909 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/statistics.proto
+-rw-r--r--   0 root         (0) root         (0)    11222 2024-05-11 22:39:12.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/statistics_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    32747 2024-05-11 22:39:12.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/statistics_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      646 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/status.proto
+-rw-r--r--   0 root         (0) root         (0)     3258 2024-05-11 22:39:12.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/status_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     6181 2024-05-11 22:39:12.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/status_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     6970 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/transform.proto
+-rw-r--r--   0 root         (0) root         (0)    16759 2024-05-11 22:39:12.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/transform_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    48797 2024-05-11 22:39:12.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/transform_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     4567 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/type.proto
+-rw-r--r--   0 root         (0) root         (0)     9784 2024-05-11 22:39:12.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/type_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    30590 2024-05-11 22:39:12.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/type_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      917 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/typing.py
+-rw-rw-rw-   0 root         (0) root         (0)     3948 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/utilities.py
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)    13753 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/scalar.py
+-rw-rw-rw-   0 root         (0) root         (0)     4757 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     1467 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/size.py
+-rw-rw-rw-   0 root         (0) root         (0)    43603 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/statistics.py
+-rw-rw-rw-   0 root         (0) root         (0)    17261 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/status.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 22:39:24.151491 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/storage/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/storage/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    14527 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/storage/local.py
+-rw-rw-rw-   0 root         (0) root         (0)     5606 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/storage/typing.py
+-rw-rw-rw-   0 root         (0) root         (0)     3084 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/storage/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    40022 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/transform.py
+-rw-rw-rw-   0 root         (0) root         (0)   123297 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/type.py
+-rw-rw-rw-   0 root         (0) root         (0)    40869 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/typing.py
+-rw-rw-rw-   0 root         (0) root         (0)     4998 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/variant_constraint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 22:39:24.153491 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec_public.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      661 2024-05-11 22:39:24.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec_public.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9090 2024-05-11 22:39:24.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec_public.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-11 22:39:24.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec_public.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-11 22:39:24.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec_public.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      125 2024-05-11 22:39:24.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec_public.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2024-05-11 22:39:24.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec_public.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     6927 2024-05-11 22:39:24.154491 sarus_data_spec_public-4.0.0.dev7/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1191 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/setup.py
```

### Comparing `sarus_data_spec_public-4.0.0.dev6/PKG-INFO` & `sarus_data_spec_public-4.0.0.dev7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sarus_data_spec_public
-Version: 4.0.0.dev6
+Version: 4.0.0.dev7
 Summary: A library to manage Sarus datasets
 Home-page: 
 Download-URL: 
 Author: Sarus Technologies
 Author-email: 
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
```

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/__init__.py` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     "VariantConstraint",
 ]
 
 """A library to manage Sarus datasets"""
 # pylint: disable=unused-variable
 
 PACKAGE_NAME: Final[str] = "sarus_data_spec"
-VERSION: Final[str] = "4.0.0.dev6"
+VERSION: Final[str] = "4.0.0.dev7"
 
 try:
     import sarus_data_spec.context.worker as sw
 
     push_global_context(sw.WorkerContext())
 except ModuleNotFoundError as exception:
     if exception.name == "sarus_data_spec.context.worker":
```

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/arrow/admin_utils.py` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/arrow/admin_utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import typing as t
 
 import pandas as pd
 import pyarrow as pa
 
+from sarus_data_spec.arrow.array import fit_array_to_schema_type_async_gen
 from sarus_data_spec.arrow.pandas_utils import (
     convert_pandas_metadata_to_admin_columns,
     pandas_index_columns,
     remove_pandas_index_columns,
 )
 from sarus_data_spec.constants import DATA, PU_COLUMN, PUBLIC, WEIGHTS
 import sarus_data_spec.typing as st
@@ -14,14 +15,15 @@
 
 async def async_to_arrow_extract_admin(
     dataset: st.Dataset, batch_size: int = 10000
 ) -> t.Optional[t.AsyncIterator[pa.RecordBatch]]:
     """This function return an async iterator record batches of the
     admin data if there is administrative columns.
     """
+    # TODO: Why not all admin columns?
     schema = await dataset.async_schema()
     if not schema.has_admin_columns():
         return None
 
     # Extract admin data from DATA
     batches_async_it = await dataset.async_to_arrow(batch_size)
     pe_field_names = [PUBLIC, PU_COLUMN, WEIGHTS]
@@ -47,20 +49,25 @@
 
 async def async_to_arrow_extract_data_only(
     dataset: st.Dataset, batch_size: int = 10000
 ) -> t.AsyncIterator[pa.RecordBatch]:
     """This function return an async iterator of record batches.
 
     The RecordBatches contain the data only, without the admin columns.
+    Index columns are admin columns
     """
     batches_async_it = await dataset.async_to_arrow(batch_size)
     schema = await dataset.async_schema()
 
+    valid_batches_async_it = fit_array_to_schema_type_async_gen(
+        batches_async_it, schema.type()
+    )
+
     if not schema.has_admin_columns():
-        return batches_async_it
+        return valid_batches_async_it
 
     # Extract PE from DATA
     data_cols = list(schema.type().data_type().children().keys())
 
     async def extract_data(
         batches_async_it: t.AsyncIterator[pa.RecordBatch],
     ) -> t.AsyncIterator[pa.RecordBatch]:
@@ -68,14 +75,15 @@
             # We add the index columns to the data
             field_names = list(batch.schema.names)
             index_cols = pandas_index_columns(batch.schema)
             index_arrays = [
                 batch.columns[field_names.index(col)]
                 for col in pandas_index_columns(batch.schema)
             ]
+
             data_arrays = batch.columns[field_names.index(DATA)].flatten()
             arrays = index_arrays + data_arrays
             names = index_cols + data_cols
 
             if len(arrays) != len(names):
                 raise ValueError(
                     f"Incompatible number of arrays {len(arrays)} and"
@@ -89,28 +97,30 @@
             new_struct_array = pa.StructArray.from_arrays(arrays, names)
             data_batch = pa.RecordBatch.from_struct_array(new_struct_array)
             data_batch = data_batch.replace_schema_metadata(
                 batch.schema.metadata
             )
             yield data_batch
 
-    return extract_data(batches_async_it)
+    return extract_data(valid_batches_async_it)
 
 
 async def async_admin_data(dataset: st.Dataset) -> t.Optional[pa.Table]:
-    """Return the protected entity as a pa.Table if it exists."""
+    """Return the privacy unit as a pa.Table if it exists."""
     pe_batches_async_it = await async_to_arrow_extract_admin(dataset)
     if pe_batches_async_it is None:
         return None
     pe_batches = [batch async for batch in pe_batches_async_it]
     return pa.Table.from_batches(pe_batches)
 
 
 def merge_schemas_metadata(schema1: pa.Schema, schema2: pa.Schema) -> dict:
     """Merge metadata from two PyArrow schemas."""
+    # TODO: if both schemas have the same metadata e.g. pandas: {..}
+    # the final merged_metadata will contain the metadata of schema2 only
     metadata1 = schema1.metadata or {}
     metadata2 = schema2.metadata or {}
 
     # Combine metadata from both schemas
     merged_metadata = {**metadata1, **metadata2}
 
     return merged_metadata
@@ -118,52 +128,51 @@
 
 def merge_data_and_admin(
     data: pa.Table, admin_data: t.Optional[pa.Table]
 ) -> pa.Table:
     """Merge a protection and the data.
 
     If the data Table has some pandas metadata attached, we remove them before
-    merging with the protected entity.
+    merging with the privacy unit.
     """
     if admin_data is None:
         # TODO also wrap the data in an empty protection
         return data
 
     data_index_columns = pandas_index_columns(data.schema)
     if len(data_index_columns) > 0:
-        # There are some pandas metadata
-        assert data_index_columns == pandas_index_columns(admin_data.schema)
         data = remove_pandas_index_columns(data)
 
     merged_metadata = merge_schemas_metadata(data.schema, admin_data.schema)
 
-    # We merge the protected entity and data in Pyarrow
+    # We merge the privacy unit and data in Pyarrow
     data_arrays = [
         chunked_array.combine_chunks() for chunked_array in data.columns
     ]
     data_array = pa.StructArray.from_arrays(
         data_arrays, names=data.column_names
     )
     merged_table = admin_data.append_column(DATA, data_array)
     merged_table = merged_table.replace_schema_metadata(merged_metadata)
     return merged_table
 
 
 def compute_admin_data(
     input_admin_data: pa.Table, result: st.DatasetCastable
 ) -> pa.Table:
-    """Compute the output protected entity of an external transform."""
+    """Compute the output privacy unit of an external transform."""
     # We guarantee that the data.index is a reliable way to trace how
     # the rows were rearranged using PyArrow's  internal implementation
     # See: https://arrow.apache.org/docs/python/pandas.html#handling-pandas-indexes
 
     if type(result) == pd.DataFrame:
         df = t.cast(pd.DataFrame, result)
         input_pe_df = input_admin_data.to_pandas()
-        output_admin_data = pa.Table.from_pandas(input_pe_df.loc[df.index])
+        filtered = input_pe_df.loc[df.index]
+        output_admin_data = pa.Table.from_pandas(filtered)
     elif type(result) == pd.Series:
         sr = t.cast(pd.Series, result)
         input_pe_df = input_admin_data.to_pandas()
         output_admin_data = pa.Table.from_pandas(input_pe_df.loc[sr.index])
     elif type(result) == pd.core.groupby.DataFrameGroupBy:
         df_grouped_by = t.cast(pd.core.groupby.DataFrameGroupBy, result)
         combined_df = df_grouped_by.obj
@@ -182,40 +191,48 @@
         raise TypeError(
             f"Cannot compute the admin data for type {type(result)}"
         )
 
     columns_to_cast = set(input_admin_data.column_names) & set(
         output_admin_data.column_names
     )
+
     for col in columns_to_cast:
         field = input_admin_data.field(col)
 
         if field != output_admin_data.field(col):
             i = output_admin_data.schema.get_field_index(col)
             column = output_admin_data.column(col).cast(field.type)
             output_admin_data = output_admin_data.set_column(i, field, column)
 
     return output_admin_data
 
 
 def validate_admin_data(
     admin_data: t.List[pa.Table],
 ) -> pa.Table:
-    """Check that all admin data are equal."""
-    # If we reach this part then there should be only one input admin data
+    """Check that admin_data (tables with administrative columns) have the
+    the same PUs and same weights."""
     if len(admin_data) == 0:
         raise ValueError("The list of input admin data is empty.")
 
     pe = next(iter(admin_data), None)
     if pe is None:
         raise ValueError(
             "The dataset was infered PUP but has no input admin data"
         )
 
-    if not all([candidate.equals(pe) for candidate in admin_data]):
+    cols_to_check = [PU_COLUMN, WEIGHTS]
+
+    if not all(
+        [
+            candidate.select(cols_to_check).equals(pe.select(cols_to_check))
+            for candidate in admin_data
+        ]
+    ):
         raise ValueError(
             "The dataset is PUP but has several differing input admin "
             "data values"
         )
     return pe
```

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/arrow/conversion.py` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/arrow/conversion.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,15 +93,14 @@
 
 async def async_arrow_batches_to_dataframegroupby(
     batches_async_iterator: t.AsyncIterator[pa.RecordBatch],
 ) -> pd.Series:
     """Returns the group by object from the data."""
     arrow_batches = [batch async for batch in batches_async_iterator]
     tab = pa.Table.from_batches(arrow_batches)
-
     groupby_keys_bytes = bytes(GROUPBY_KEYS_NAME, "utf-8")
     if groupby_keys_bytes in tab.schema.metadata:
         keys_encoded = tab.schema.metadata[groupby_keys_bytes]
         keys = SarusJSONDecoder.decode_bytes(keys_encoded)
     else:
         raise ValueError(
             "Trying to convert to series Arrow batches "
@@ -117,15 +116,14 @@
 async def async_arrow_batches_to_seriesgroupby(
     batches_async_iterator: t.AsyncIterator[pa.RecordBatch],
 ) -> pd.Series:
     """Returns the group by object from the data."""
     arrow_batches = [batch async for batch in batches_async_iterator]
     tab = pa.Table.from_batches(arrow_batches)
     df = tab.to_pandas(split_blocks=False, self_destruct=True)
-
     groupby_keys_bytes = bytes(GROUPBY_KEYS_NAME, "utf-8")
     if groupby_keys_bytes in tab.schema.metadata:
         keys_encoded = tab.schema.metadata[groupby_keys_bytes]
         keys = SarusJSONDecoder.decode_bytes(keys_encoded)
     else:
         raise ValueError(
             "Trying to convert to series Arrow batches "
@@ -142,21 +140,21 @@
 def to_pyarrow_table(data: t.Any) -> pa.Table:
     """Convert the result of an external transform to a Pyarrow Table."""
     if type(data) not in t.get_args(st.DatasetCastable):
         raise TypeError(f"Cannot convert {type(data)} to Arrow batches.")
 
     if isinstance(data, pd.DataFrame):
         df = t.cast(pd.DataFrame, data)
-        return pa.Table.from_pandas(df)
+        return pa.Table.from_pandas(df, preserve_index=True)
     elif isinstance(data, pd.Series):
         sr = t.cast(pd.Series, data)
         if sr.name is None:
             # We need to set a name otherwise pandas adds a default one.
             sr.name = NO_SERIES_NAME
-        return pa.Table.from_pandas(pd.DataFrame(sr))
+        return pa.Table.from_pandas(pd.DataFrame(sr), preserve_index=True)
     elif isinstance(data, pd.core.groupby.DataFrameGroupBy):
         df_grouped_by = t.cast(pd.core.groupby.DataFrameGroupBy, data)
         combined_df = df_grouped_by.obj
 
         keys = df_grouped_by.keys
         encoded_keys = SarusJSONEncoder.encode_bytes(keys)
```

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/arrow/pandas_utils.py` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/arrow/pandas_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import typing as t
-
 import pyarrow as pa
 
 from sarus_data_spec.constants import DATA
 
 
 def pandas_index_columns(schema: pa.Schema) -> t.List[str]:
     """Return the list of columns that have to be considered as Pandas index
```

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/arrow/schema.py` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/arrow/schema.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/arrow/type.py` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/arrow/type.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/attribute.py` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/attribute.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/base.py` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/base.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/bounds.py` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/bounds.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/constants.py` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/constants.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/context/public.py` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/context/public.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/context/typing.py` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/context/typing.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/dataset.py` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/dataset.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/dataspec_rewriter/base.py` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/dataspec_rewriter/base.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/dataspec_rewriter/graph_query_builder_utils.py` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/dataspec_rewriter/graph_query_builder_utils.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/dataspec_rewriter/recursive_rewriter.py` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/dataspec_rewriter/recursive_rewriter.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/dataspec_rewriter/simple_rules.py` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/dataspec_rewriter/simple_rules.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/dataspec_rewriter/typing.py` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/dataspec_rewriter/typing.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/dataspec_rewriter/utils.py` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/dataspec_rewriter/utils.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/dataspec_validator/base.py` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/dataspec_validator/base.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/dataspec_validator/parameter_kind.py` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/dataspec_validator/parameter_kind.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/dataspec_validator/privacy_limit.py` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/dataspec_validator/privacy_limit.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/dataspec_validator/recursive_validator.py` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/dataspec_validator/recursive_validator.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/dataspec_validator/signature.py` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/dataspec_validator/signature.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/dataspec_validator/simple_rules.py` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/dataspec_validator/simple_rules.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/dataspec_validator/typing.py` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/dataspec_validator/typing.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/deprecation.py` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/deprecation.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/factory.py` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/factory.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/json_serialisation.py` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/json_serialisation.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/async_utils.py` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/async_utils.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/base.py` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -772,14 +772,17 @@
         result_type: t.Optional[st.Type] = None,
     ) -> t.AsyncIterator[pa.RecordBatch]:
         raise NotImplementedError
 
     def manager(self) -> manager_typing.Manager:
         return self
 
+    def launch_job(self, command: t.List[str], env: t.Dict[str, str]) -> None:
+        raise NotImplementedError
+
 
 def check_transform_big_data(
     transform: st.Transform,
     parent_dataset: st.Dataset,
     parents_dict: t.Mapping[str, st.DataSpec],
 ) -> t.Tuple[bool, int, int, str]:
     """This methods return true if the dataset transformed
```

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/cache_utils.py` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/cache_utils.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/computations/base.py` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/computations/base.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/computations/local/base.py` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/computations/local/base.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/computations/local/schema.py` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/computations/local/schema.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/computations/remote/base.py` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/computations/remote/base.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/base.py` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/base.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/__init__.py` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/__init__.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/external_op.py` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/external_op.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -254,14 +254,15 @@
 
         syn_dataset = t.cast(st.Dataset, syn_variant)
         arrow_iterator = await syn_dataset.async_to_arrow(batch_size=1000)
         first_batch = await arrow_iterator.__anext__()
         schema = first_batch.schema
 
         schema_type = type_from_arrow_schema(schema)
+
         # retrieve max_mul from parent
         parents_args, parents_kwargs = self.dataset.parents()
         parents_args.extend(parents_kwargs.values())
         parents_args = [el for el in parents_args if isinstance(el, Dataset)]
         if len(parents_args) > 1 or len(parents_args) == 0:
             max_mult = ""  # we cannot infer max_mult in this case
             max_max_mult = DEFAULT_MAX_MAX_MULT
@@ -326,15 +327,14 @@
             result = await implementation.compute(bound_signature)
             if (
                 isinstance(result, pd.Series)
                 and implementation.pup_kind(bound_signature) == PUPKind.ROW
             ):
                 # Reformat the series as a dataframe with a single row
                 result = result.to_frame().transpose()
-
             ds_result = t.cast(st.DatasetCastable, result)
             admin_data = await bound_signature.admin_data()
             output_admin_data = compute_admin_data(admin_data, ds_result)
             data_table = to_pyarrow_table(ds_result)
             table = merge_data_and_admin(data_table, output_admin_data)
 
         else:
```

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/imblearn.py` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/imblearn.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/numpy.py` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/numpy.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/optbinning.py` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/optbinning.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/pandas/groupby.py` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/pandas/groupby.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/pandas/groupby_dp.py` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/pandas/groupby_dp.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/pandas/pandas.py` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/pandas/pandas.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/pandas/pandas_dp.py` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/pandas/pandas_dp.py`

 * *Files 1% similar despite different names*

```diff
@@ -819,15 +819,18 @@
                     normalize=normalize,
                     dropna=dropna,
                 ).value(column_name, max_mul, random_generator),
             )
             count_dp_dict[column_name] = histogram
 
         # for now only on series
-        count_dp = pd.Series(list(count_dp_dict.values())[0])
+        values = list(count_dp_dict.values())[0]
+        name = list(count_dp_dict.keys())[0]
+        # added to be conform to its expected schema
+        count_dp = pd.Series(data=values, name=name)
         return count_dp
 
 
 class pd_corr_dp(ExternalOpImplementation):
     _transform_id = "pandas.PD_CORR_DP"
     _non_dp_equivalent_id = "pandas.PD_CORR"
```

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/pandas_profiling.py` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/pandas_profiling.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/scipy.py` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/scipy.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/shap/Explanation.py` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/shap/Explanation.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/shap/explainer.py` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/shap/explainer.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/shap/maskers.py` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/shap/maskers.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/shap/plots.py` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/shap/plots.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/shap/utils.py` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/shap/utils.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/sklearn/cluster.py` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/sklearn/cluster.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/sklearn/compose.py` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/sklearn/compose.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/sklearn/decomposition.py` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/sklearn/decomposition.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/sklearn/ensemble.py` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/sklearn/ensemble.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/sklearn/impute.py` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/sklearn/impute.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/sklearn/inspection.py` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/sklearn/inspection.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/sklearn/lib.py` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/sklearn/lib.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/sklearn/linear_model.py` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/sklearn/linear_model.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/sklearn/metrics.py` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/sklearn/metrics.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/sklearn/model_selection.py` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/sklearn/model_selection.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/sklearn/pipeline.py` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/sklearn/pipeline.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/sklearn/preprocessing.py` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/sklearn/preprocessing.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/sklearn/svm.py` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/sklearn/svm.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/skopt.py` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/skopt.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/std.py` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/std.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/typing.py` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/typing.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/utils.py` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/utils.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/xgboost.py` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/xgboost.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/routing.py` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/routing.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 
 except ModuleNotFoundError:
     logger = logging.getLogger(__name__)
     logger.info("Transforms: Sample not available.")
 
 
 try:
-    from sarus_data_spec.manager.ops.processor.standard.fit_model import (
+    from sarus_data_spec.manager.ops.processor.standard.llm.fit_model import (
         FitModel,
         FitModelDP,
         FitModelDPStaticChecker,
         FitModelStaticChecker,
     )
 
 except ModuleNotFoundError:
```

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/standard/differentiated_sample.py` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/standard/differentiated_sample.py`

 * *Files 0% similar despite different names*

```diff
@@ -180,25 +180,26 @@
         seed = Scalar(
             self.dataset.transform().protobuf().spec.differentiated_sample.seed
         ).value()
         generator = np.random.default_rng(seed)
 
         previous_ds = t.cast(Dataset, self.parent())
         previous_schema = await self.parent_schema()
+
+        if len(previous_schema.tables()) == 1:
+            return await sample_arrow_to_arrow(self, batch_size)
+
         parent_batches = [
             convert_record_batch(batch, previous_schema.type())
             async for batch in await self.parent_to_arrow()
         ]
         struct_arr = pa.concat_arrays(parent_batches)
         previous_size = await previous_ds.manager().async_size(previous_ds)
         assert previous_size
 
-        if len(previous_schema.tables()) == 1:
-            return await sample_arrow_to_arrow(self, batch_size)
-
         size_dict = await differentiated_sampling_sizes(self.dataset)
 
         indices_to_take = sample_indices_from_array(
             array=struct_arr.flatten()[struct_arr.type.get_field_index(DATA)],
             stat=previous_size.statistics(),
             selected_indices=pa.array(
                 np.linspace(0, len(struct_arr) - 1, len(struct_arr), dtype=int)
```

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/standard/error_estimation.py` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/standard/error_estimation.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/standard/extract.py` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/standard/extract.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/standard/filter.py` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/standard/filter.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/standard/generate_from_model.py` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/standard/generate_from_model.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/standard/get_item.py` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/standard/get_item.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/standard/project.py` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/standard/project.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/standard/sample.py` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/standard/sample.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/standard/sampling/differentiated_sampling_sizes.py` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/standard/sampling/differentiated_sampling_sizes.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/standard/shuffle.py` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/standard/shuffle.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/standard/standard_op.py` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/standard/standard_op.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/standard/synthetic.py` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/standard/synthetic.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/standard/to_small_data.py` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/standard/to_small_data.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/standard/visitor_selector.py` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/standard/visitor_selector.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/source/routing.py` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/source/routing.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/sql_utils/bigdata.py` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/sql_utils/bigdata.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/sql_utils/queries.py` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/sql_utils/queries.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/typing.py` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/typing.py`

 * *Files 1% similar despite different names*

```diff
@@ -277,14 +277,18 @@
         """
 
     def composed_callable(
         self, transform: st.Transform
     ) -> t.Callable[..., t.Any]:
         """Return a Python callable of a composed transform."""
 
+    def launch_job(
+        self, command: t.List[str], env: t.Dict[str, str]
+    ) -> None: ...
+
 
 @runtime_checkable
 class HasManager(Protocol):
     """Has a manager."""
 
     def manager(self) -> Manager:
         """Return a manager (usually a singleton)."""
```

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/marginals.py` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/marginals.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/multiplicity.py` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/multiplicity.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/path.py` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/path.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/predicate.py` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/predicate.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/__init__.py` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/__init__.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/attribute_pb2.py` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/attribute_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/attribute_pb2.pyi` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/attribute_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/bounds_pb2.py` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/bounds_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/bounds_pb2.pyi` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/bounds_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/constraint_pb2.py` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/constraint_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/constraint_pb2.pyi` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/constraint_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/dataset.proto` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/dataset.proto`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/dataset_pb2.py` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/dataset_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/dataset_pb2.pyi` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/dataset_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/links_pb2.py` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/links_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/links_pb2.pyi` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/links_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/manager_pb2.py` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/manager_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/manager_pb2.pyi` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/marginals_pb2.py` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/marginals_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/marginals_pb2.pyi` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/marginals_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/multiplicity_pb2.py` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/multiplicity_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/multiplicity_pb2.pyi` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/multiplicity_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/path_pb2.py` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/path_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/path_pb2.pyi` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/path_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/predicate.proto` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/predicate.proto`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/predicate_pb2.py` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/predicate_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/predicate_pb2.pyi` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/predicate_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/proto_container_pb2.py` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/proto_container_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/proto_container_pb2.pyi` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/proto_container_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/relation.proto` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/relation.proto`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/relation_pb2.py` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/relation_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/relation_pb2.pyi` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/relation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/scalar.proto` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/scalar.proto`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/scalar_pb2.py` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/scalar_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/scalar_pb2.pyi` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/scalar_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/schema.proto` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/schema.proto`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/schema_pb2.py` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/schema_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/schema_pb2.pyi` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/schema_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/size_pb2.py` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/size_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/size_pb2.pyi` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/size_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/statistics.proto` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/statistics.proto`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/statistics_pb2.py` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/statistics_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/statistics_pb2.pyi` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/statistics_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/status.proto` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/status.proto`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/status_pb2.py` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/status_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/status_pb2.pyi` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/status_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/transform.proto` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/transform.proto`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/transform_pb2.py` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/transform_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/transform_pb2.pyi` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/transform_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/type.proto` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/type.proto`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/type_pb2.py` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/type_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/type_pb2.pyi` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/type_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/typing.py` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/typing.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/utilities.py` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/utilities.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/scalar.py` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/scalar.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/schema.py` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/schema.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/size.py` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/size.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/statistics.py` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/statistics.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/status.py` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/status.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/storage/local.py` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/storage/local.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/storage/typing.py` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/storage/typing.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/storage/utils.py` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/storage/utils.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/transform.py` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/transform.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/type.py` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/type.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/typing.py` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/typing.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/variant_constraint.py` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/variant_constraint.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec_public.egg-info/PKG-INFO` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec_public.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sarus_data_spec_public
-Version: 4.0.0.dev6
+Version: 4.0.0.dev7
 Summary: A library to manage Sarus datasets
 Home-page: 
 Download-URL: 
 Author: Sarus Technologies
 Author-email: 
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
```

### Comparing `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec_public.egg-info/SOURCES.txt` & `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec_public.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/setup.cfg` & `sarus_data_spec_public-4.0.0.dev7/setup.cfg`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev6/setup.py` & `sarus_data_spec_public-4.0.0.dev7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,8 +43,8 @@
 
     def run(self):
         generate_proto_code()
         build_py.run(self)
 
 
 if __name__ == "__main__":
-    setup(version="4.0.0.dev6")
+    setup(version="4.0.0.dev7")
```

