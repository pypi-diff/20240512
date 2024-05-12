# Comparing `tmp/celi_framework-0.2.0.tar.gz` & `tmp/celi_framework-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "celi_framework-0.2.0.tar", max compression
+gzip compressed data, was "celi_framework-0.2.1.tar", max compression
```

## Comparing `celi_framework-0.2.0.tar` & `celi_framework-0.2.1.tar`

### file list

```diff
@@ -1,63 +1,67 @@
--rw-r--r--   0        0        0     1084 2024-05-06 14:31:21.781694 celi_framework-0.2.0/LICENSE
--rw-r--r--   0        0        0    12984 2024-05-06 14:31:21.781694 celi_framework-0.2.0/README.md
--rw-r--r--   0        0        0    11983 2024-05-06 14:31:21.781694 celi_framework-0.2.0/celi_framework/core/job_description.py
--rw-r--r--   0        0        0    23124 2024-05-06 14:31:21.781694 celi_framework-0.2.0/celi_framework/core/monitor.py
--rw-r--r--   0        0        0    11341 2024-05-06 14:31:21.781694 celi_framework-0.2.0/celi_framework/core/mt_factory.py
--rw-r--r--   0        0        0    14719 2024-05-06 14:31:21.781694 celi_framework-0.2.0/celi_framework/core/post_monitor.py
--rw-r--r--   0        0        0    17145 2024-05-06 14:31:21.781694 celi_framework-0.2.0/celi_framework/core/processor.py
--rw-r--r--   0        0        0     2859 2024-05-06 14:31:21.781694 celi_framework-0.2.0/celi_framework/core/runner.py
--rw-r--r--   0        0        0    23630 2024-05-06 14:31:21.781694 celi_framework-0.2.0/celi_framework/core/templates.py
--rw-r--r--   0        0        0      371 2024-05-06 14:31:21.781694 celi_framework-0.2.0/celi_framework/examples/human_eval/README.md
--rw-r--r--   0        0        0      815 2024-05-06 14:31:21.781694 celi_framework-0.2.0/celi_framework/examples/human_eval/eval.py
--rw-r--r--   0        0        0    46321 2024-05-06 14:31:21.781694 celi_framework-0.2.0/celi_framework/examples/human_eval/example_output.json
--rw-r--r--   0        0        0     4074 2024-05-06 14:31:21.781694 celi_framework-0.2.0/celi_framework/examples/human_eval/job_description.py
--rwxr-xr-x   0        0        0   196170 2024-05-06 14:31:21.781694 celi_framework-0.2.0/celi_framework/examples/human_eval/test.csv
--rw-r--r--   0        0        0     2629 2024-05-06 14:31:21.781694 celi_framework-0.2.0/celi_framework/examples/human_eval/test_tools.py
--rw-r--r--   0        0        0     3577 2024-05-06 14:31:21.781694 celi_framework-0.2.0/celi_framework/examples/human_eval/tools.py
--rw-r--r--   0        0        0    13793 2024-05-06 14:31:21.781694 celi_framework-0.2.0/celi_framework/examples/reporting_template/job_description.py
--rw-r--r--   0        0        0    10352 2024-05-06 14:31:21.781694 celi_framework-0.2.0/celi_framework/examples/reporting_template/tools.py
--rw-r--r--   0        0        0     6133 2024-05-06 14:31:21.781694 celi_framework-0.2.0/celi_framework/examples/wikipedia/Index_cache.py
--rw-r--r--   0        0        0     7694 2024-05-06 14:31:21.785694 celi_framework-0.2.0/celi_framework/examples/wikipedia/caching_beautiful_soup_reader.py
--rw-r--r--   0        0        0     4282 2024-05-06 14:31:21.785694 celi_framework-0.2.0/celi_framework/examples/wikipedia/eval/run_eval.py
--rw-r--r--   0        0        0      530 2024-05-06 14:31:21.785694 celi_framework-0.2.0/celi_framework/examples/wikipedia/eval/test_sets.json
--rw-r--r--   0        0        0      851 2024-05-06 14:31:21.785694 celi_framework-0.2.0/celi_framework/examples/wikipedia/eval/test_sets_large.json
--rw-r--r--   0        0        0      161 2024-05-06 14:31:21.785694 celi_framework-0.2.0/celi_framework/examples/wikipedia/example_config.json
--rw-r--r--   0        0        0    13876 2024-05-06 14:31:21.785694 celi_framework-0.2.0/celi_framework/examples/wikipedia/index.py
--rw-r--r--   0        0        0    10858 2024-05-06 14:31:21.785694 celi_framework-0.2.0/celi_framework/examples/wikipedia/job_description.py
--rw-r--r--   0        0        0     7133 2024-05-06 14:31:21.785694 celi_framework-0.2.0/celi_framework/examples/wikipedia/loader.py
--rw-r--r--   0        0        0    14762 2024-05-06 14:31:21.785694 celi_framework-0.2.0/celi_framework/examples/wikipedia/tools.py
--rw-r--r--   0        0        0      549 2024-05-06 14:31:21.785694 celi_framework-0.2.0/celi_framework/examples/wikipedia/wikipedia_utils.py
--rw-r--r--   0        0        0    12668 2024-05-06 14:31:21.785694 celi_framework-0.2.0/celi_framework/experimental/embeddor.py
--rw-r--r--   0        0        0     7936 2024-05-06 14:31:21.785694 celi_framework-0.2.0/celi_framework/experimental/mapper.py
--rw-r--r--   0        0        0     1354 2024-05-06 14:31:21.785694 celi_framework-0.2.0/celi_framework/experimental/mechanic.py
--rw-r--r--   0        0        0        0 2024-05-06 14:31:21.785694 celi_framework-0.2.0/celi_framework/experimental/preprocessing/__init__.py
--rw-r--r--   0        0        0    23634 2024-05-06 14:31:21.785694 celi_framework-0.2.0/celi_framework/experimental/preprocessing/pre-processor.py
--rw-r--r--   0        0        0       94 2024-05-06 14:31:21.785694 celi_framework-0.2.0/celi_framework/experimental/preprocessing/word_pdf_extractors/__init__.py
--rw-r--r--   0        0        0     8832 2024-05-06 14:31:21.785694 celi_framework-0.2.0/celi_framework/experimental/preprocessing/word_pdf_extractors/extract_pdf_tables.py
--rw-r--r--   0        0        0     2056 2024-05-06 14:31:21.785694 celi_framework-0.2.0/celi_framework/experimental/preprocessing/word_pdf_extractors/extractor_helpers.py
--rw-r--r--   0        0        0    10669 2024-05-06 14:31:21.785694 celi_framework-0.2.0/celi_framework/experimental/preprocessing/word_pdf_extractors/pdf_extractor.py
--rw-r--r--   0        0        0     7835 2024-05-06 14:31:21.785694 celi_framework-0.2.0/celi_framework/experimental/preprocessing/word_pdf_extractors/word_extractor.py
--rw-r--r--   0        0        0     5471 2024-05-06 14:31:21.785694 celi_framework-0.2.0/celi_framework/experimental/task_builder/factory.py
--rw-r--r--   0        0        0     4242 2024-05-06 14:31:21.785694 celi_framework-0.2.0/celi_framework/experimental/task_builder/llm_helper_funcs.py
--rw-r--r--   0        0        0     4352 2024-05-06 14:31:21.785694 celi_framework-0.2.0/celi_framework/experimental/task_builder/llms.py
--rw-r--r--   0        0        0     5939 2024-05-06 14:31:21.785694 celi_framework-0.2.0/celi_framework/experimental/task_builder/template.py
--rw-r--r--   0        0        0     9914 2024-05-06 14:31:21.785694 celi_framework-0.2.0/celi_framework/experimental/utils/ada.py
--rw-r--r--   0        0        0    19041 2024-05-06 14:31:21.785694 celi_framework-0.2.0/celi_framework/experimental/utils/mapper_utils.py
--rw-r--r--   0        0        0    13615 2024-05-06 14:31:21.785694 celi_framework-0.2.0/celi_framework/experimental/utils/nougat_preprocessing/preprocess.py
--rw-r--r--   0        0        0     5118 2024-05-06 14:31:21.785694 celi_framework-0.2.0/celi_framework/experimental/utils/nougat_preprocessing/preprocessing_templates.py
--rw-r--r--   0        0        0     5458 2024-05-06 14:31:21.785694 celi_framework-0.2.0/celi_framework/experimental/utils/postprocessor_utils.py
--rw-r--r--   0        0        0     9091 2024-05-06 14:31:21.785694 celi_framework-0.2.0/celi_framework/experimental/utils/synthetic_data.py
--rw-r--r--   0        0        0     1449 2024-05-06 14:31:21.785694 celi_framework-0.2.0/celi_framework/logging_config.json
--rw-r--r--   0        0        0     2171 2024-05-06 14:31:21.785694 celi_framework-0.2.0/celi_framework/logging_setup.py
--rw-r--r--   0        0        0     6787 2024-05-06 14:31:21.785694 celi_framework-0.2.0/celi_framework/main.py
--rw-r--r--   0        0        0        0 2024-05-06 14:31:21.785694 celi_framework-0.2.0/celi_framework/utils/__init__.py
--rw-r--r--   0        0        0    11028 2024-05-06 14:31:21.785694 celi_framework-0.2.0/celi_framework/utils/codex.py
--rw-r--r--   0        0        0      461 2024-05-06 14:31:21.785694 celi_framework-0.2.0/celi_framework/utils/exceptions.py
--rw-r--r--   0        0        0    22723 2024-05-06 14:31:21.785694 celi_framework-0.2.0/celi_framework/utils/llmcore_utils.py
--rw-r--r--   0        0        0    10021 2024-05-06 14:31:21.785694 celi_framework-0.2.0/celi_framework/utils/llms.py
--rw-r--r--   0        0        0       77 2024-05-06 14:31:21.785694 celi_framework-0.2.0/celi_framework/utils/log.py
--rw-r--r--   0        0        0    10717 2024-05-06 14:31:21.785694 celi_framework-0.2.0/celi_framework/utils/sql_utils.py
--rw-r--r--   0        0        0    10871 2024-05-06 14:31:21.785694 celi_framework-0.2.0/celi_framework/utils/token_counters.py
--rw-r--r--   0        0        0    28482 2024-05-06 14:31:21.785694 celi_framework-0.2.0/celi_framework/utils/utils.py
--rw-r--r--   0        0        0     1806 2024-05-06 14:34:13.148816 celi_framework-0.2.0/pyproject.toml
--rw-r--r--   0        0        0    14509 1970-01-01 00:00:00.000000 celi_framework-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1084 2024-05-12 20:27:53.347957 celi_framework-0.2.1/LICENSE
+-rw-r--r--   0        0        0    12984 2024-05-12 20:27:53.347957 celi_framework-0.2.1/README.md
+-rw-r--r--   0        0        0    11983 2024-05-12 20:27:53.347957 celi_framework-0.2.1/celi_framework/core/job_description.py
+-rw-r--r--   0        0        0    23124 2024-05-12 20:27:53.347957 celi_framework-0.2.1/celi_framework/core/monitor.py
+-rw-r--r--   0        0        0    11341 2024-05-12 20:27:53.347957 celi_framework-0.2.1/celi_framework/core/mt_factory.py
+-rw-r--r--   0        0        0    14719 2024-05-12 20:27:53.347957 celi_framework-0.2.1/celi_framework/core/post_monitor.py
+-rw-r--r--   0        0        0    17882 2024-05-12 20:27:53.347957 celi_framework-0.2.1/celi_framework/core/processor.py
+-rw-r--r--   0        0        0     2859 2024-05-12 20:27:53.347957 celi_framework-0.2.1/celi_framework/core/runner.py
+-rw-r--r--   0        0        0    23630 2024-05-12 20:27:53.347957 celi_framework-0.2.1/celi_framework/core/templates.py
+-rw-r--r--   0        0        0      679 2024-05-12 20:27:53.347957 celi_framework-0.2.1/celi_framework/examples/human_eval/README.md
+-rw-r--r--   0        0        0     1068 2024-05-12 20:27:53.347957 celi_framework-0.2.1/celi_framework/examples/human_eval/eval.py
+-rw-r--r--   0        0        0      995 2024-05-12 20:27:53.347957 celi_framework-0.2.1/celi_framework/examples/human_eval/eval_osx.py
+-rw-r--r--   0        0        0   180797 2024-05-12 20:27:53.347957 celi_framework-0.2.1/celi_framework/examples/human_eval/example_output.json
+-rw-r--r--   0        0        0   141468 2024-05-12 20:27:53.347957 celi_framework-0.2.1/celi_framework/examples/human_eval/example_output_prompt_engineering.json
+-rw-r--r--   0        0        0     5548 2024-05-12 20:27:53.347957 celi_framework-0.2.1/celi_framework/examples/human_eval/job_description.py
+-rw-r--r--   0        0        0    16156 2024-05-12 20:27:53.347957 celi_framework-0.2.1/celi_framework/examples/human_eval/job_description_prompt_engineering.py
+-rw-r--r--   0        0        0     3148 2024-05-12 20:27:53.347957 celi_framework-0.2.1/celi_framework/examples/human_eval/main.py
+-rwxr-xr-x   0        0        0   196170 2024-05-12 20:27:53.351957 celi_framework-0.2.1/celi_framework/examples/human_eval/test.csv
+-rw-r--r--   0        0        0     4190 2024-05-12 20:27:53.351957 celi_framework-0.2.1/celi_framework/examples/human_eval/test_tools.py
+-rw-r--r--   0        0        0     6249 2024-05-12 20:27:53.351957 celi_framework-0.2.1/celi_framework/examples/human_eval/tools.py
+-rw-r--r--   0        0        0    13793 2024-05-12 20:27:53.351957 celi_framework-0.2.1/celi_framework/examples/reporting_template/job_description.py
+-rw-r--r--   0        0        0    10352 2024-05-12 20:27:53.351957 celi_framework-0.2.1/celi_framework/examples/reporting_template/tools.py
+-rw-r--r--   0        0        0     6133 2024-05-12 20:27:53.351957 celi_framework-0.2.1/celi_framework/examples/wikipedia/Index_cache.py
+-rw-r--r--   0        0        0     7694 2024-05-12 20:27:53.351957 celi_framework-0.2.1/celi_framework/examples/wikipedia/caching_beautiful_soup_reader.py
+-rw-r--r--   0        0        0     4282 2024-05-12 20:27:53.351957 celi_framework-0.2.1/celi_framework/examples/wikipedia/eval/run_eval.py
+-rw-r--r--   0        0        0      530 2024-05-12 20:27:53.351957 celi_framework-0.2.1/celi_framework/examples/wikipedia/eval/test_sets.json
+-rw-r--r--   0        0        0      851 2024-05-12 20:27:53.351957 celi_framework-0.2.1/celi_framework/examples/wikipedia/eval/test_sets_large.json
+-rw-r--r--   0        0        0      161 2024-05-12 20:27:53.351957 celi_framework-0.2.1/celi_framework/examples/wikipedia/example_config.json
+-rw-r--r--   0        0        0    13876 2024-05-12 20:27:53.351957 celi_framework-0.2.1/celi_framework/examples/wikipedia/index.py
+-rw-r--r--   0        0        0    10858 2024-05-12 20:27:53.351957 celi_framework-0.2.1/celi_framework/examples/wikipedia/job_description.py
+-rw-r--r--   0        0        0     7133 2024-05-12 20:27:53.351957 celi_framework-0.2.1/celi_framework/examples/wikipedia/loader.py
+-rw-r--r--   0        0        0    14762 2024-05-12 20:27:53.351957 celi_framework-0.2.1/celi_framework/examples/wikipedia/tools.py
+-rw-r--r--   0        0        0      549 2024-05-12 20:27:53.351957 celi_framework-0.2.1/celi_framework/examples/wikipedia/wikipedia_utils.py
+-rw-r--r--   0        0        0    12668 2024-05-12 20:27:53.351957 celi_framework-0.2.1/celi_framework/experimental/embeddor.py
+-rw-r--r--   0        0        0     7936 2024-05-12 20:27:53.351957 celi_framework-0.2.1/celi_framework/experimental/mapper.py
+-rw-r--r--   0        0        0     1354 2024-05-12 20:27:53.351957 celi_framework-0.2.1/celi_framework/experimental/mechanic.py
+-rw-r--r--   0        0        0        0 2024-05-12 20:27:53.351957 celi_framework-0.2.1/celi_framework/experimental/preprocessing/__init__.py
+-rw-r--r--   0        0        0    23634 2024-05-12 20:27:53.351957 celi_framework-0.2.1/celi_framework/experimental/preprocessing/pre-processor.py
+-rw-r--r--   0        0        0       94 2024-05-12 20:27:53.351957 celi_framework-0.2.1/celi_framework/experimental/preprocessing/word_pdf_extractors/__init__.py
+-rw-r--r--   0        0        0     8832 2024-05-12 20:27:53.351957 celi_framework-0.2.1/celi_framework/experimental/preprocessing/word_pdf_extractors/extract_pdf_tables.py
+-rw-r--r--   0        0        0     2056 2024-05-12 20:27:53.351957 celi_framework-0.2.1/celi_framework/experimental/preprocessing/word_pdf_extractors/extractor_helpers.py
+-rw-r--r--   0        0        0    10669 2024-05-12 20:27:53.351957 celi_framework-0.2.1/celi_framework/experimental/preprocessing/word_pdf_extractors/pdf_extractor.py
+-rw-r--r--   0        0        0     7835 2024-05-12 20:27:53.351957 celi_framework-0.2.1/celi_framework/experimental/preprocessing/word_pdf_extractors/word_extractor.py
+-rw-r--r--   0        0        0     5471 2024-05-12 20:27:53.351957 celi_framework-0.2.1/celi_framework/experimental/task_builder/factory.py
+-rw-r--r--   0        0        0     4242 2024-05-12 20:27:53.351957 celi_framework-0.2.1/celi_framework/experimental/task_builder/llm_helper_funcs.py
+-rw-r--r--   0        0        0     4352 2024-05-12 20:27:53.351957 celi_framework-0.2.1/celi_framework/experimental/task_builder/llms.py
+-rw-r--r--   0        0        0     5939 2024-05-12 20:27:53.351957 celi_framework-0.2.1/celi_framework/experimental/task_builder/template.py
+-rw-r--r--   0        0        0     9914 2024-05-12 20:27:53.351957 celi_framework-0.2.1/celi_framework/experimental/utils/ada.py
+-rw-r--r--   0        0        0    19041 2024-05-12 20:27:53.351957 celi_framework-0.2.1/celi_framework/experimental/utils/mapper_utils.py
+-rw-r--r--   0        0        0    13615 2024-05-12 20:27:53.351957 celi_framework-0.2.1/celi_framework/experimental/utils/nougat_preprocessing/preprocess.py
+-rw-r--r--   0        0        0     5118 2024-05-12 20:27:53.351957 celi_framework-0.2.1/celi_framework/experimental/utils/nougat_preprocessing/preprocessing_templates.py
+-rw-r--r--   0        0        0     5458 2024-05-12 20:27:53.351957 celi_framework-0.2.1/celi_framework/experimental/utils/postprocessor_utils.py
+-rw-r--r--   0        0        0     9091 2024-05-12 20:27:53.351957 celi_framework-0.2.1/celi_framework/experimental/utils/synthetic_data.py
+-rw-r--r--   0        0        0     1449 2024-05-12 20:27:53.351957 celi_framework-0.2.1/celi_framework/logging_config.json
+-rw-r--r--   0        0        0     2171 2024-05-12 20:27:53.351957 celi_framework-0.2.1/celi_framework/logging_setup.py
+-rw-r--r--   0        0        0     6787 2024-05-12 20:27:53.351957 celi_framework-0.2.1/celi_framework/main.py
+-rw-r--r--   0        0        0        0 2024-05-12 20:27:53.351957 celi_framework-0.2.1/celi_framework/utils/__init__.py
+-rw-r--r--   0        0        0    11028 2024-05-12 20:27:53.351957 celi_framework-0.2.1/celi_framework/utils/codex.py
+-rw-r--r--   0        0        0      461 2024-05-12 20:27:53.351957 celi_framework-0.2.1/celi_framework/utils/exceptions.py
+-rw-r--r--   0        0        0    22723 2024-05-12 20:27:53.351957 celi_framework-0.2.1/celi_framework/utils/llmcore_utils.py
+-rw-r--r--   0        0        0    10311 2024-05-12 20:27:53.351957 celi_framework-0.2.1/celi_framework/utils/llms.py
+-rw-r--r--   0        0        0       77 2024-05-12 20:27:53.351957 celi_framework-0.2.1/celi_framework/utils/log.py
+-rw-r--r--   0        0        0    10717 2024-05-12 20:27:53.351957 celi_framework-0.2.1/celi_framework/utils/sql_utils.py
+-rw-r--r--   0        0        0    10871 2024-05-12 20:27:53.351957 celi_framework-0.2.1/celi_framework/utils/token_counters.py
+-rw-r--r--   0        0        0    28738 2024-05-12 20:27:53.351957 celi_framework-0.2.1/celi_framework/utils/utils.py
+-rw-r--r--   0        0        0     1805 2024-05-12 20:28:40.023546 celi_framework-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0    14509 1970-01-01 00:00:00.000000 celi_framework-0.2.1/PKG-INFO
```

### Comparing `celi_framework-0.2.0/LICENSE` & `celi_framework-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `celi_framework-0.2.0/README.md` & `celi_framework-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `celi_framework-0.2.0/celi_framework/core/job_description.py` & `celi_framework-0.2.1/celi_framework/core/job_description.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.2.0/celi_framework/core/monitor.py` & `celi_framework-0.2.1/celi_framework/core/monitor.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.2.0/celi_framework/core/mt_factory.py` & `celi_framework-0.2.1/celi_framework/core/mt_factory.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.2.0/celi_framework/core/post_monitor.py` & `celi_framework-0.2.1/celi_framework/core/post_monitor.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.2.0/celi_framework/core/processor.py` & `celi_framework-0.2.1/celi_framework/core/processor.py`

 * *Files 6% similar despite different names*

```diff
@@ -81,24 +81,24 @@
             skip_section_list = []
         self.master_template = master_template  # config and schema need to be defined # TODO -> Read latest version from codex?
         # TODO -> Have it be so that there is a manual template creation process which would be what's above (but with arg for manual create passed in),
         #  then rest of time have it just read from Mongo/codex
         self.builtin_tool_descriptions = [
             ToolDescription(
                 name="pop_context",
-                description='This used to signal to the outer layer that a pop is requested by the LLMs. Returns the '
-                            'next section number.\n\nThis function should not be called unless the "Final Document '
-                            'Review" has been completed and you are ready to move to the next section.\nIt will empty '
-                            'out the current chat history.',
+                description="This used to signal to the outer layer that a pop is requested by the LLMs. Returns the "
+                "next test case taskID.\n\nThis function should not be called unless the save_draft_section"
+                "function has been called and you are ready to move to the next test case.\nIt will empty "
+                "out the current chat history.",
                 parameters={
                     "type": "object",
                     "properties": {
                         "current_section_number": {
                             "type": "string",
-                            "description": "No description provided.",
+                            "description": "Current taskID.",
                         }
                     },
                     "required": ["current_section_number"],
                 },
             )
         ]
         self.codex = codex
@@ -107,15 +107,17 @@
         self.system_message = self.master_template.create_system_message()
         app_logger.info(
             f"System message created:\n{self.system_message}", extra={"color": "cyan"}
         )
         self.save_template()
 
         section_list = list(self.master_template.schema.keys())
-        self.sections_to_be_completed = self.removed_skipped_sections(section_list, skip_section_list)
+        self.sections_to_be_completed = self.removed_skipped_sections(
+            section_list, skip_section_list
+        )
         self.current_section = self.sections_to_be_completed[0]
 
         self.tool_implementations = tool_implementations
         self.tool_descriptions = generate_tool_descriptions(
             self.master_template.job_desc.tool_implementations_class
         )
 
@@ -146,26 +148,46 @@
 
         app_logger.info(
             "New chat iteration:\n"
             + self.format_chat_messages(self.ongoing_chat[chat_len:]),
             extra={"color": "green"},
         )
 
+        if self.check_for_duplicates(self.ongoing_chat):
+            logger.warning(
+                "Identified a loop.  Identical messages are repeating.  pop_context and moving on to the next section."
+            )
+            self.pop_context_flag = True
+
         if self.pop_context_flag:
             self.handle_pop_context()
 
+    def check_for_duplicates(
+        self, ongoing_chat: List[Dict[str, str] | Tuple[str, str]]
+    ):
+        if len(ongoing_chat) == 0:
+            return False
+        last_message = ongoing_chat[-1]
+        duplicates = 0
+        for message in ongoing_chat[:-1]:
+            if message == last_message:
+                duplicates += 1
+        return duplicates > 2
+
     def format_chat_messages(self, msgs: List[ChatMessageable]):
         return "\n\n".join(self.format_message_content(m) for m in msgs)
 
     def format_message_content(self, m: ChatMessageable):
         if isinstance(m, dict):
             return f"{m['role'].capitalize()}:\n{m['content']}"
         return f"{m[0].capitalize()}:\n{m[1]}"
 
-    def removed_skipped_sections(self, all_sections: List[str], skip_section_list: List[str]):
+    def removed_skipped_sections(
+        self, all_sections: List[str], skip_section_list: List[str]
+    ):
         """
         Filters out sections from the drafting process based on a provided list of sections to skip.
 
         Args:
             all_sections (list of str): The full list of section identifiers
             skip_section_list (list of str): A list of section identifiers to be skipped in the drafting process.
 
@@ -270,15 +292,18 @@
                             function_return = method_to_call(**arguments)
                         except Exception as e:
                             function_return = f"Error: {e}"
                     else:
                         app_logger.error(
                             f"Unknown function name: {name}", extra={"color": "red"}
                         )
-                        function_return = f"Error: Called unknown function name: {name}"
+                        return (
+                            "user",
+                            f"Error: Called unknown function name: {name} with arguments {arguments}",
+                        )
             function_log = f"Call to function {name} with arguments {arguments} returned\n{function_return}"
             return {"role": "function", "name": name, "content": function_log}
 
         return [make_tool_call(_) for _ in response.message.tool_calls]
 
     def handle_pop_context(self):
         """
```

### Comparing `celi_framework-0.2.0/celi_framework/core/runner.py` & `celi_framework-0.2.1/celi_framework/core/runner.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.2.0/celi_framework/core/templates.py` & `celi_framework-0.2.1/celi_framework/core/templates.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.2.0/celi_framework/examples/human_eval/eval.py` & `celi_framework-0.2.1/celi_framework/examples/human_eval/eval.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,35 @@
 import sys
 
 from celi_framework.examples.human_eval.tools import HumanEvalTools
-from celi_framework.utils.utils import read_json_from_file
+from celi_framework.utils.utils import read_json_from_file, get_most_recent_file
 
 # Evaluate results
-if len(sys.argv) > 0:
+if len(sys.argv) > 1:
     file = sys.argv[1]
 else:
-    file = 'target/celi_output/drafts/2024-05-06_07-38-23.json'
+    directory = "target/celi_output/drafts"
+    file = get_most_recent_file(directory)
+
+print(f"Evaluating {file}")
 results = read_json_from_file(file)
 tools = HumanEvalTools()
 
-def run_test(id, func):
-    code = tools.tests.loc[id, 'prompt']+'\n'+func
-    return tools.run_tests(id,code)
 
-evaluated = {k : run_test(k, v) for k,v in results.items()}
+def run_test(id, solution):
+    code = tools.tests.loc[id, "prompt"] + "\n" + solution["func"]
+    return tools._run_official_tests(id, code)
+
 
+evaluated = {k: run_test(k, v) for k, v in results.items()}
+
+total = tools.tests.shape[0]
 n_trials = len(evaluated)
 n_correct = len([_ for _ in evaluated.values() if _ is None])
-errors = {k:v for k,v in evaluated.items() if v is not None}
-
+errors = {k: v for k, v in evaluated.items() if v is not None}
+unevaluated = total - n_trials
 
 print(f"{n_correct} correct out of {n_trials}: {round(100*n_correct/n_trials, 2)}%")
+print(f"Unanswered: {unevaluated} - resulting in {round(100*n_correct/total, 2)}%")
 print("Errors:\n")
-for k,v in errors.items():
+for k, v in errors.items():
     print(f"{k}:{v}\n")
```

### Comparing `celi_framework-0.2.0/celi_framework/examples/human_eval/job_description.py` & `celi_framework-0.2.1/celi_framework/examples/human_eval/job_description.py`

 * *Files 25% similar despite different names*

```diff
@@ -5,27 +5,51 @@
     Task(
         task_name="Get the prompt for this task",
         details={
             "description": "Find the coding prompt for the current section by calling get_prompt",
         },
     ),
     Task(
-        task_name="Write code and run tests",
+        task_name="Develop initial test cases",
         details={
-            "description": """Decide how to implement the function and call run_tests to check your implementation.
-            If the tests don't pass, review the error, correct.  Keep going as long as you are making progress, but if 
-            you can't get all the tests to pass after a few tried, move on to the next step.  Include the full prompt
-            (with imports) in your call to run function.  Append your implementation to the end of the prompt.""",
+            "description": """Think through the problem and develop an initial set of test cases that will be used to
+            check the logic for your function.  The test cases must be implemented as a function called 
+            'def check(candidate)' that takes the function as an argument.  Each test is an 'assert' statement that 
+            calls the function with some inputs and verifies that that output is as expected.  For example, if the task its to create a function called
+            'add_two_numbers", the test function might look like:
+            def check(candidate):
+                assert add_two_numbers(1, 2) == 3
+                assert add_two_numbers(0, 0) == 0
+                assert add_two_numbers(-1, 1) == 0
+                assert add_two_numbers(1.5, 1) == 2.5
+            
+            Think through edge cases and different types of inputs that might be passed to the function.            
+            """,
+        },
+    ),
+    Task(
+        task_name="Write code and tests",
+        details={
+            "description": """
+            In this task you iteratively refine your implementation and test cases.   
+            Decide how to implement the function and call run_tests to check your implementation, passing in the code 
+            and tests. If the tests don't pass, check both your implementation and the test cases and decide which needs 
+            to be adjusted (or both). Don't assume the test cases are correct, review the problem specification and 
+            adjust if necessary.  Also, feel free to add more tests.  
+            Keep going as long as you are making progress, but if 
+            you can't get all the tests to pass after a few tries, save your best effort result and move on to the 
+            next problem.""",
         },
     ),
     Task(
         task_name="Product the final output.",
         details={
-            "description": """Your final output should be the body of the function indented by 4 spaces.  Do not
-            include the function header.  Write the final output using the `save_draft_section` tool.  
+            "description": """Call save_final_output to save off your final answer.  This should include your 
+            function implementation as well as your test function.  Always do this, even if you aren't completely
+            happy with your answer. 
             Signal that you have completed the example by calling the pop_context function."""
         },
     ),
 ]
 
 general_comments = """
 ============
@@ -55,17 +79,18 @@
 
 If all tasks for the current section have been completed, proceed to the next document section.
 If the new section draft is complete, ensure to 'Prepare for Next Document Section' as described in the tasks.
 """
 
 pre_algo_instruct = """
 I am going to give you step by step instructions on how to solve problems in the HumanEval data set.  For each problem
-you are given a prompt which is a Python function signature and doc string.  Your job is to draft the function.  There
-are a set of test cases that will check the behavior.  You can run the tests and check the results as many times as you
-like.  When you are done with your result, your final output is the function body.
+you are given a prompt which is a Python function signature and doc string.  Your job is to draft the function.  You have
+a tool available to run a set of tests and check the results.  You can run the tests and check the results as many times as you
+like, but make sure you don't get stuck in a loop of sending the same code to test over and over.  
+When you are done with your result, your final output is the function body.
 For example.  If the prompt is;
 def add(a: int, b: int) -> int:
     "Add two numbers"
     
 Then your response would be:
     return a+b
```

### Comparing `celi_framework-0.2.0/celi_framework/examples/human_eval/test.csv` & `celi_framework-0.2.1/celi_framework/examples/human_eval/test.csv`

 * *Files identical despite different names*

### Comparing `celi_framework-0.2.0/celi_framework/examples/reporting_template/job_description.py` & `celi_framework-0.2.1/celi_framework/examples/reporting_template/job_description.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.2.0/celi_framework/examples/reporting_template/tools.py` & `celi_framework-0.2.1/celi_framework/examples/reporting_template/tools.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.2.0/celi_framework/examples/wikipedia/Index_cache.py` & `celi_framework-0.2.1/celi_framework/examples/wikipedia/Index_cache.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.2.0/celi_framework/examples/wikipedia/caching_beautiful_soup_reader.py` & `celi_framework-0.2.1/celi_framework/examples/wikipedia/caching_beautiful_soup_reader.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.2.0/celi_framework/examples/wikipedia/eval/run_eval.py` & `celi_framework-0.2.1/celi_framework/examples/wikipedia/eval/run_eval.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.2.0/celi_framework/examples/wikipedia/eval/test_sets.json` & `celi_framework-0.2.1/celi_framework/examples/wikipedia/eval/test_sets.json`

 * *Files identical despite different names*

### Comparing `celi_framework-0.2.0/celi_framework/examples/wikipedia/eval/test_sets_large.json` & `celi_framework-0.2.1/celi_framework/examples/wikipedia/eval/test_sets_large.json`

 * *Files identical despite different names*

### Comparing `celi_framework-0.2.0/celi_framework/examples/wikipedia/index.py` & `celi_framework-0.2.1/celi_framework/examples/wikipedia/index.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.2.0/celi_framework/examples/wikipedia/job_description.py` & `celi_framework-0.2.1/celi_framework/examples/wikipedia/job_description.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.2.0/celi_framework/examples/wikipedia/loader.py` & `celi_framework-0.2.1/celi_framework/examples/wikipedia/loader.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.2.0/celi_framework/examples/wikipedia/tools.py` & `celi_framework-0.2.1/celi_framework/examples/wikipedia/tools.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.2.0/celi_framework/examples/wikipedia/wikipedia_utils.py` & `celi_framework-0.2.1/celi_framework/examples/wikipedia/wikipedia_utils.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.2.0/celi_framework/experimental/embeddor.py` & `celi_framework-0.2.1/celi_framework/experimental/embeddor.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.2.0/celi_framework/experimental/mapper.py` & `celi_framework-0.2.1/celi_framework/experimental/mapper.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.2.0/celi_framework/experimental/mechanic.py` & `celi_framework-0.2.1/celi_framework/experimental/mechanic.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.2.0/celi_framework/experimental/preprocessing/pre-processor.py` & `celi_framework-0.2.1/celi_framework/experimental/preprocessing/pre-processor.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.2.0/celi_framework/experimental/preprocessing/word_pdf_extractors/extract_pdf_tables.py` & `celi_framework-0.2.1/celi_framework/experimental/preprocessing/word_pdf_extractors/extract_pdf_tables.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.2.0/celi_framework/experimental/preprocessing/word_pdf_extractors/extractor_helpers.py` & `celi_framework-0.2.1/celi_framework/experimental/preprocessing/word_pdf_extractors/extractor_helpers.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.2.0/celi_framework/experimental/preprocessing/word_pdf_extractors/pdf_extractor.py` & `celi_framework-0.2.1/celi_framework/experimental/preprocessing/word_pdf_extractors/pdf_extractor.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.2.0/celi_framework/experimental/preprocessing/word_pdf_extractors/word_extractor.py` & `celi_framework-0.2.1/celi_framework/experimental/preprocessing/word_pdf_extractors/word_extractor.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.2.0/celi_framework/experimental/task_builder/factory.py` & `celi_framework-0.2.1/celi_framework/experimental/task_builder/factory.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.2.0/celi_framework/experimental/task_builder/llm_helper_funcs.py` & `celi_framework-0.2.1/celi_framework/experimental/task_builder/llm_helper_funcs.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.2.0/celi_framework/experimental/task_builder/llms.py` & `celi_framework-0.2.1/celi_framework/experimental/task_builder/llms.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.2.0/celi_framework/experimental/task_builder/template.py` & `celi_framework-0.2.1/celi_framework/experimental/task_builder/template.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.2.0/celi_framework/experimental/utils/ada.py` & `celi_framework-0.2.1/celi_framework/experimental/utils/ada.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.2.0/celi_framework/experimental/utils/mapper_utils.py` & `celi_framework-0.2.1/celi_framework/experimental/utils/mapper_utils.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.2.0/celi_framework/experimental/utils/nougat_preprocessing/preprocess.py` & `celi_framework-0.2.1/celi_framework/experimental/utils/nougat_preprocessing/preprocess.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.2.0/celi_framework/experimental/utils/nougat_preprocessing/preprocessing_templates.py` & `celi_framework-0.2.1/celi_framework/experimental/utils/nougat_preprocessing/preprocessing_templates.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.2.0/celi_framework/experimental/utils/postprocessor_utils.py` & `celi_framework-0.2.1/celi_framework/experimental/utils/postprocessor_utils.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.2.0/celi_framework/experimental/utils/synthetic_data.py` & `celi_framework-0.2.1/celi_framework/experimental/utils/synthetic_data.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.2.0/celi_framework/logging_config.json` & `celi_framework-0.2.1/celi_framework/logging_config.json`

 * *Files identical despite different names*

### Comparing `celi_framework-0.2.0/celi_framework/logging_setup.py` & `celi_framework-0.2.1/celi_framework/logging_setup.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.2.0/celi_framework/main.py` & `celi_framework-0.2.1/celi_framework/main.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.2.0/celi_framework/utils/codex.py` & `celi_framework-0.2.1/celi_framework/utils/codex.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.2.0/celi_framework/utils/llmcore_utils.py` & `celi_framework-0.2.1/celi_framework/utils/llmcore_utils.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.2.0/celi_framework/utils/llms.py` & `celi_framework-0.2.1/celi_framework/utils/llms.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,28 +21,30 @@
         potential inefficiencies, which is critical for applications processing large volumes of text
         or managing numerous concurrent interactions with the LLM.
 
 """
 
 import functools
 import os
+import re
 import time
 from typing import Optional, Dict, List, Any, Tuple
-from pydantic import BaseModel
+
 import openai
 from openai.types.chat import ChatCompletion
+from pydantic import BaseModel
 from requests import HTTPError
 
 from celi_framework.utils.codex import MongoDBUtilitySingleton
+from celi_framework.utils.exceptions import ContextLengthExceededException
+from celi_framework.utils.log import app_logger
 from celi_framework.utils.token_counters import (
     token_counter_decorator_ask_split,
     token_counter_decorator_quick_ask,
 )
-from celi_framework.utils.log import app_logger
-from celi_framework.utils.exceptions import ContextLengthExceededException
 
 
 # Initialize the OpenAI client, using the OPENAI_API_KEY environment variable.
 @functools.lru_cache(1)
 def get_openai_client():
     return openai.OpenAI(api_key=os.environ["OPENAI_API_KEY"])
 
@@ -108,14 +110,15 @@
             openai.APIError,
             HTTPError,
             ConnectionError,
             TimeoutError,
         ) as e:
             err_cnt += 1
             app_logger.exception(f"Error attempt {err_cnt}", extra={"color": "red"})
+            app_logger.error(f"Error: Prompt was {user_prompt}")
             time.sleep(wait_between_retries)
             last_error = e
 
     if verbose:
         app_logger.error(
             f"All retries failed after {max_retries} attempts.", extra={"color": "red"}
         )
@@ -219,25 +222,31 @@
     if err_cnt >= max_retries:
         err = f"All retries failed after {max_retries} attempts."
         app_logger.error(err, extra={"color": "red"})
         # Instead of returning the error, consider raising a generic exception if recovery is not possible
         raise Exception(f"{err}\nLast error: {last_error} with Prompt:\n{prompt}")
 
 
+VALID_ROLES = r"^[a-zA-Z0-9_-]+$"
+
+
 def assemble_chat_messages(prompt: str | List[Tuple[str, str] | Dict[str, str]]):
     """Takes a prompt and formats it as chat messages.  Prompt can be in the form:
     * "" - str - A single prompt string
     * A list of ("role","content") tuples
     * A list of dictionaries of chat messages {"role":"assistant","content":"..."}
     """
 
     def format_message(m):
         if isinstance(m, dict):
+            assert re.match(VALID_ROLES, m["role"]), f"Invalid role: {m['role']}"
             return m
         else:
+            role = m[0]
+            assert re.match(VALID_ROLES, role), f"Invalid role: {role}"
             return {"role": m[0], "content": m[1]}
 
     if isinstance(prompt, str):
         return [{"role": "user", "content": prompt}]
     else:
         return [format_message(msg) for msg in prompt]
```

### Comparing `celi_framework-0.2.0/celi_framework/utils/sql_utils.py` & `celi_framework-0.2.1/celi_framework/utils/sql_utils.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.2.0/celi_framework/utils/token_counters.py` & `celi_framework-0.2.1/celi_framework/utils/token_counters.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.2.0/celi_framework/utils/utils.py` & `celi_framework-0.2.1/celi_framework/utils/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,26 +23,26 @@
 Usage:
 This module is designed to be imported and used in Python applications that require advanced logging capabilities,
 efficient data handling, and manipulation, as well as dynamic content generation. Its modular design allows for
 easy integration into existing projects, enhancing functionality without significant refactoring.
 
 """
 
+import glob
+import hashlib
 import importlib
-from pathlib import Path
+import json
+import os
 import random
-from datetime import datetime
-import hashlib
+import re
 import time
+from datetime import datetime
 from functools import wraps
-import json
-import re
+from pathlib import Path
 from typing import Optional
-import os
-import glob
 
 
 class UnrecoverableException(BaseException):
     pass
 
 
 def get_obj_by_name(name: str):
@@ -111,14 +111,22 @@
         print(f"File not found: {file_path}")
         return ""
     except Exception as e:
         print(f"An error occurred: {e}")
         return ""
 
 
+def get_most_recent_file(directory):
+    # Create a full path and ensure it only lists files
+    files = [
+        f for f in os.listdir(directory) if os.path.isfile(os.path.join(directory, f))
+    ]
+    return os.path.join(directory, sorted(files)[-1])
+
+
 def check_last_line(input_string, string_to_check="[END]"):
     """
     Checks if the last line of the input string is 'Proceed to next section.'
 
     Args:
     input_string (str): The string to be checked.
```

### Comparing `celi_framework-0.2.0/pyproject.toml` & `celi_framework-0.2.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "celi-framework"
-version = "0.2.0"
+version = "0.2.1"
 description = "Controller-Embedded Language Interactions - facilitates the entire lifecycle of document processing, from pre-processing and embedding to post-monitoring and quality assessment."
 authors = ["Jan-Samuel Wagner <jwab@genmab.com>","Dave DeCaprio <daved@alum.mit.edu>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/x3n0cr4735/celi"
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
@@ -47,12 +47,12 @@
 sphinx-autobuild = "^2021.3.14"
 protobuf = ">=4.21.6" # Added to address build issues with readthedocs.
 cffi = ">=1.10.0" # Added to address build issues with readthedocs. pyo3_runtime.PanicException: Python API call failed
 sphinx-autodoc-typehints = "^2.0.0"
 
 [tool.pytest.ini_options]
 log_level="DEBUG"
-#log_cli=true
+log_cli=true
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `celi_framework-0.2.0/PKG-INFO` & `celi_framework-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: celi-framework
-Version: 0.2.0
+Version: 0.2.1
 Summary: Controller-Embedded Language Interactions - facilitates the entire lifecycle of document processing, from pre-processing and embedding to post-monitoring and quality assessment.
 Home-page: https://github.com/x3n0cr4735/celi
 License: MIT
 Author: Jan-Samuel Wagner
 Author-email: jwab@genmab.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
```

