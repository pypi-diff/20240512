# Comparing `tmp/sagemaker-ssh-helper-2.1.0.tar.gz` & `tmp/sagemaker_ssh_helper-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sagemaker-ssh-helper-2.1.0.tar", last modified: Wed Aug 23 16:45:38 2023, max compression
+gzip compressed data, was "sagemaker_ssh_helper-2.2.0.tar", last modified: Sun May 12 19:12:14 2024, max compression
```

## Comparing `sagemaker-ssh-helper-2.1.0.tar` & `sagemaker_ssh_helper-2.2.0.tar`

### file list

```diff
@@ -1,78 +1,90 @@
-drwxr-xr-x   0 ivankh     (504) staff       (20)        0 2023-08-23 16:45:38.702969 sagemaker-ssh-helper-2.1.0/
--rw-r--r--   0 ivankh     (504) staff       (20)      925 2023-08-23 16:41:56.000000 sagemaker-ssh-helper-2.1.0/LICENSE
--rw-r--r--   0 ivankh     (504) staff       (20)     1494 2023-08-23 16:45:38.702807 sagemaker-ssh-helper-2.1.0/PKG-INFO
--rw-r--r--   0 ivankh     (504) staff       (20)    44584 2023-08-23 16:41:56.000000 sagemaker-ssh-helper-2.1.0/README.md
-drwxr-xr-x   0 ivankh     (504) staff       (20)        0 2023-08-23 16:45:38.692091 sagemaker-ssh-helper-2.1.0/sagemaker_ssh_helper/
--rw-r--r--   0 ivankh     (504) staff       (20)     2715 2023-08-23 16:41:56.000000 sagemaker-ssh-helper-2.1.0/sagemaker_ssh_helper/__init__.py
--rw-r--r--   0 ivankh     (504) staff       (20)     1038 2023-08-23 16:41:56.000000 sagemaker-ssh-helper-2.1.0/sagemaker_ssh_helper/aws.py
-drwxr-xr-x   0 ivankh     (504) staff       (20)        0 2023-08-23 16:45:38.694628 sagemaker-ssh-helper-2.1.0/sagemaker_ssh_helper/cdk/
--rw-r--r--   0 ivankh     (504) staff       (20)        0 2023-08-23 16:41:56.000000 sagemaker-ssh-helper-2.1.0/sagemaker_ssh_helper/cdk/__init__.py
--rw-r--r--   0 ivankh     (504) staff       (20)      219 2023-08-23 16:41:56.000000 sagemaker-ssh-helper-2.1.0/sagemaker_ssh_helper/cdk/advanced_tier_app.py
-drwxr-xr-x   0 ivankh     (504) staff       (20)        0 2023-08-23 16:45:38.696234 sagemaker-ssh-helper-2.1.0/sagemaker_ssh_helper/cdk/iam_ssm/
--rw-r--r--   0 ivankh     (504) staff       (20)        0 2023-08-23 16:41:56.000000 sagemaker-ssh-helper-2.1.0/sagemaker_ssh_helper/cdk/iam_ssm/__init__.py
--rw-r--r--   0 ivankh     (504) staff       (20)      284 2023-08-23 16:41:56.000000 sagemaker-ssh-helper-2.1.0/sagemaker_ssh_helper/cdk/iam_ssm/advanced_tier_lambda.py
--rw-r--r--   0 ivankh     (504) staff       (20)     8439 2023-08-23 16:41:56.000000 sagemaker-ssh-helper-2.1.0/sagemaker_ssh_helper/cdk/iam_ssm/iam_ssm_stack.py
--rw-r--r--   0 ivankh     (504) staff       (20)     9895 2023-08-23 16:41:56.000000 sagemaker-ssh-helper-2.1.0/sagemaker_ssh_helper/cdk/iam_ssm/iam_ssm_stack_tests.py
--rw-r--r--   0 ivankh     (504) staff       (20)     1481 2023-08-23 16:41:56.000000 sagemaker-ssh-helper-2.1.0/sagemaker_ssh_helper/cdk/iam_ssm/ssm_advanced_tier_stack.py
--rw-r--r--   0 ivankh     (504) staff       (20)      677 2023-08-23 16:41:56.000000 sagemaker-ssh-helper-2.1.0/sagemaker_ssh_helper/cdk/iam_ssm/trust_relationship_lambda.py
--rw-r--r--   0 ivankh     (504) staff       (20)      185 2023-08-23 16:41:56.000000 sagemaker-ssh-helper-2.1.0/sagemaker_ssh_helper/cdk/iam_ssm_app.py
-drwxr-xr-x   0 ivankh     (504) staff       (20)        0 2023-08-23 16:45:38.696854 sagemaker-ssh-helper-2.1.0/sagemaker_ssh_helper/cdk/low_gpu/
--rw-r--r--   0 ivankh     (504) staff       (20)        0 2023-08-23 16:41:56.000000 sagemaker-ssh-helper-2.1.0/sagemaker_ssh_helper/cdk/low_gpu/__init__.py
--rw-r--r--   0 ivankh     (504) staff       (20)     3301 2023-08-23 16:41:56.000000 sagemaker-ssh-helper-2.1.0/sagemaker_ssh_helper/cdk/low_gpu/low_gpu_lambda.py
--rw-r--r--   0 ivankh     (504) staff       (20)     2551 2023-08-23 16:41:56.000000 sagemaker-ssh-helper-2.1.0/sagemaker_ssh_helper/cdk/low_gpu/low_gpu_lambda_stack.py
--rw-r--r--   0 ivankh     (504) staff       (20)      207 2023-08-23 16:41:56.000000 sagemaker-ssh-helper-2.1.0/sagemaker_ssh_helper/cdk/low_gpu_lambda_app.py
-drwxr-xr-x   0 ivankh     (504) staff       (20)        0 2023-08-23 16:45:38.697066 sagemaker-ssh-helper-2.1.0/sagemaker_ssh_helper/cdk/tests/
--rw-r--r--   0 ivankh     (504) staff       (20)        0 2023-08-23 16:41:56.000000 sagemaker-ssh-helper-2.1.0/sagemaker_ssh_helper/cdk/tests/__init__.py
-drwxr-xr-x   0 ivankh     (504) staff       (20)        0 2023-08-23 16:45:38.697229 sagemaker-ssh-helper-2.1.0/sagemaker_ssh_helper/cdk/tests/unit/
--rw-r--r--   0 ivankh     (504) staff       (20)        0 2023-08-23 16:41:56.000000 sagemaker-ssh-helper-2.1.0/sagemaker_ssh_helper/cdk/tests/unit/__init__.py
--rw-r--r--   0 ivankh     (504) staff       (20)      207 2023-08-23 16:41:56.000000 sagemaker-ssh-helper-2.1.0/sagemaker_ssh_helper/cdk/tests_app.py
--rw-r--r--   0 ivankh     (504) staff       (20)     2292 2023-08-23 16:41:56.000000 sagemaker-ssh-helper-2.1.0/sagemaker_ssh_helper/deregister_old_instances_from_ssm.py
--rw-r--r--   0 ivankh     (504) staff       (20)     2242 2023-08-23 16:41:56.000000 sagemaker-ssh-helper-2.1.0/sagemaker_ssh_helper/detached_sagemaker.py
--rw-r--r--   0 ivankh     (504) staff       (20)      761 2023-08-23 16:41:56.000000 sagemaker-ssh-helper-2.1.0/sagemaker_ssh_helper/env.py
--rw-r--r--   0 ivankh     (504) staff       (20)    13119 2023-08-23 16:41:56.000000 sagemaker-ssh-helper-2.1.0/sagemaker_ssh_helper/ide.py
--rw-r--r--   0 ivankh     (504) staff       (20)    12013 2023-08-23 16:41:56.000000 sagemaker-ssh-helper-2.1.0/sagemaker_ssh_helper/log.py
--rw-r--r--   0 ivankh     (504) staff       (20)     8485 2023-08-23 16:45:25.000000 sagemaker-ssh-helper-2.1.0/sagemaker_ssh_helper/manager.py
--rw-r--r--   0 ivankh     (504) staff       (20)     7231 2023-08-23 16:41:56.000000 sagemaker-ssh-helper-2.1.0/sagemaker_ssh_helper/proxy.py
--rw-r--r--   0 ivankh     (504) staff       (20)     4576 2023-08-23 16:41:56.000000 sagemaker-ssh-helper-2.1.0/sagemaker_ssh_helper/sm-connect-ssh-proxy
--rw-r--r--   0 ivankh     (504) staff       (20)     6176 2023-08-23 16:41:56.000000 sagemaker-ssh-helper-2.1.0/sagemaker_ssh_helper/sm-helper-functions
--rw-r--r--   0 ivankh     (504) staff       (20)     2456 2023-08-23 16:41:56.000000 sagemaker-ssh-helper-2.1.0/sagemaker_ssh_helper/sm-init-ssm
--rw-r--r--   0 ivankh     (504) staff       (20)      451 2023-08-23 16:41:56.000000 sagemaker-ssh-helper-2.1.0/sagemaker_ssh_helper/sm-local-configure
--rw-r--r--   0 ivankh     (504) staff       (20)     4490 2023-08-23 16:45:25.000000 sagemaker-ssh-helper-2.1.0/sagemaker_ssh_helper/sm-local-ssh-ide
--rw-r--r--   0 ivankh     (504) staff       (20)      940 2023-08-23 16:41:56.000000 sagemaker-ssh-helper-2.1.0/sagemaker_ssh_helper/sm-local-ssh-inference
--rw-r--r--   0 ivankh     (504) staff       (20)      841 2023-08-23 16:41:56.000000 sagemaker-ssh-helper-2.1.0/sagemaker_ssh_helper/sm-local-ssh-notebook
--rw-r--r--   0 ivankh     (504) staff       (20)      945 2023-08-23 16:41:56.000000 sagemaker-ssh-helper-2.1.0/sagemaker_ssh_helper/sm-local-ssh-processing
--rw-r--r--   0 ivankh     (504) staff       (20)      955 2023-08-23 16:41:56.000000 sagemaker-ssh-helper-2.1.0/sagemaker_ssh_helper/sm-local-ssh-training
--rw-r--r--   0 ivankh     (504) staff       (20)      945 2023-08-23 16:41:56.000000 sagemaker-ssh-helper-2.1.0/sagemaker_ssh_helper/sm-local-ssh-transform
--rwxr-xr-x   0 ivankh     (504) staff       (20)     1178 2023-08-23 16:41:56.000000 sagemaker-ssh-helper-2.1.0/sagemaker_ssh_helper/sm-local-start-ssh
--rw-r--r--   0 ivankh     (504) staff       (20)      966 2023-08-23 16:41:56.000000 sagemaker-ssh-helper-2.1.0/sagemaker_ssh_helper/sm-save-env
--rw-r--r--   0 ivankh     (504) staff       (20)     4969 2023-08-23 16:41:56.000000 sagemaker-ssh-helper-2.1.0/sagemaker_ssh_helper/sm-setup-ssh
--rw-r--r--   0 ivankh     (504) staff       (20)    10321 2023-08-23 16:41:56.000000 sagemaker-ssh-helper-2.1.0/sagemaker_ssh_helper/sm-ssh-ide
--rw-r--r--   0 ivankh     (504) staff       (20)     1494 2023-08-23 16:41:56.000000 sagemaker-ssh-helper-2.1.0/sagemaker_ssh_helper/sm-wait
--rw-r--r--   0 ivankh     (504) staff       (20)    24447 2023-08-23 16:41:56.000000 sagemaker-ssh-helper-2.1.0/sagemaker_ssh_helper/wrapper.py
-drwxr-xr-x   0 ivankh     (504) staff       (20)        0 2023-08-23 16:45:38.693469 sagemaker-ssh-helper-2.1.0/sagemaker_ssh_helper.egg-info/
--rw-r--r--   0 ivankh     (504) staff       (20)     1494 2023-08-23 16:45:38.000000 sagemaker-ssh-helper-2.1.0/sagemaker_ssh_helper.egg-info/PKG-INFO
--rw-r--r--   0 ivankh     (504) staff       (20)     2388 2023-08-23 16:45:38.000000 sagemaker-ssh-helper-2.1.0/sagemaker_ssh_helper.egg-info/SOURCES.txt
--rw-r--r--   0 ivankh     (504) staff       (20)        1 2023-08-23 16:45:38.000000 sagemaker-ssh-helper-2.1.0/sagemaker_ssh_helper.egg-info/dependency_links.txt
--rw-r--r--   0 ivankh     (504) staff       (20)      537 2023-08-23 16:45:38.000000 sagemaker-ssh-helper-2.1.0/sagemaker_ssh_helper.egg-info/requires.txt
--rw-r--r--   0 ivankh     (504) staff       (20)       21 2023-08-23 16:45:38.000000 sagemaker-ssh-helper-2.1.0/sagemaker_ssh_helper.egg-info/top_level.txt
--rw-r--r--   0 ivankh     (504) staff       (20)       38 2023-08-23 16:45:38.703028 sagemaker-ssh-helper-2.1.0/setup.cfg
--rw-r--r--   0 ivankh     (504) staff       (20)     3853 2023-08-23 16:44:12.000000 sagemaker-ssh-helper-2.1.0/setup.py
-drwxr-xr-x   0 ivankh     (504) staff       (20)        0 2023-08-23 16:45:38.702435 sagemaker-ssh-helper-2.1.0/tests/
--rw-r--r--   0 ivankh     (504) staff       (20)     2132 2023-08-23 16:41:56.000000 sagemaker-ssh-helper-2.1.0/tests/test_attach.py
--rw-r--r--   0 ivankh     (504) staff       (20)     4561 2023-08-23 16:41:56.000000 sagemaker-ssh-helper-2.1.0/tests/test_batch_inference.py
--rw-r--r--   0 ivankh     (504) staff       (20)     8134 2023-08-23 16:41:56.000000 sagemaker-ssh-helper-2.1.0/tests/test_clean_core.py
--rw-r--r--   0 ivankh     (504) staff       (20)     1078 2023-08-23 16:41:56.000000 sagemaker-ssh-helper-2.1.0/tests/test_compiler.py
--rw-r--r--   0 ivankh     (504) staff       (20)      727 2023-08-23 16:41:56.000000 sagemaker-ssh-helper-2.1.0/tests/test_deregister_instances.py
--rw-r--r--   0 ivankh     (504) staff       (20)     4021 2023-08-23 16:41:56.000000 sagemaker-ssh-helper-2.1.0/tests/test_distributed.py
--rw-r--r--   0 ivankh     (504) staff       (20)    18509 2023-08-23 16:41:56.000000 sagemaker-ssh-helper-2.1.0/tests/test_end_to_end.py
--rw-r--r--   0 ivankh     (504) staff       (20)     2372 2023-08-23 16:41:56.000000 sagemaker-ssh-helper-2.1.0/tests/test_environment.py
--rw-r--r--   0 ivankh     (504) staff       (20)    36381 2023-08-23 16:41:56.000000 sagemaker-ssh-helper-2.1.0/tests/test_frameworks.py
--rw-r--r--   0 ivankh     (504) staff       (20)    13886 2023-08-23 16:41:56.000000 sagemaker-ssh-helper-2.1.0/tests/test_functions.py
--rw-r--r--   0 ivankh     (504) staff       (20)     3662 2023-08-23 16:41:56.000000 sagemaker-ssh-helper-2.1.0/tests/test_hpo.py
--rw-r--r--   0 ivankh     (504) staff       (20)    17243 2023-08-23 16:41:56.000000 sagemaker-ssh-helper-2.1.0/tests/test_ide.py
--rw-r--r--   0 ivankh     (504) staff       (20)     2620 2023-08-23 16:41:56.000000 sagemaker-ssh-helper-2.1.0/tests/test_inference_registry.py
--rw-r--r--   0 ivankh     (504) staff       (20)     1732 2023-08-23 16:41:56.000000 sagemaker-ssh-helper-2.1.0/tests/test_local.py
--rw-r--r--   0 ivankh     (504) staff       (20)     4958 2023-08-23 16:41:56.000000 sagemaker-ssh-helper-2.1.0/tests/test_manual.py
--rw-r--r--   0 ivankh     (504) staff       (20)     9942 2023-08-23 16:45:25.000000 sagemaker-ssh-helper-2.1.0/tests/test_ssm_manager.py
--rw-r--r--   0 ivankh     (504) staff       (20)     1091 2023-08-23 16:41:56.000000 sagemaker-ssh-helper-2.1.0/tests/test_util.py
--rw-r--r--   0 ivankh     (504) staff       (20)      992 2023-08-23 16:41:56.000000 sagemaker-ssh-helper-2.1.0/tests/test_validation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 19:12:14.383340 sagemaker_ssh_helper-2.2.0/
+-rw-r--r--   0 root         (0) root         (0)      925 2024-05-12 19:07:30.000000 sagemaker_ssh_helper-2.2.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3047 2024-05-12 19:12:14.383340 sagemaker_ssh_helper-2.2.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    51495 2024-05-12 19:07:30.000000 sagemaker_ssh_helper-2.2.0/README.md
+-rw-r--r--   0 root         (0) root         (0)    20931 2024-05-12 19:07:30.000000 sagemaker_ssh_helper-2.2.0/SageMaker_SSH_IDE.ipynb
+-rw-r--r--   0 root         (0) root         (0)    15658 2024-05-12 19:07:30.000000 sagemaker_ssh_helper-2.2.0/SageMaker_SSH_Notebook.ipynb
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 19:12:14.355342 sagemaker_ssh_helper-2.2.0/sagemaker_ssh_helper/
+-rw-r--r--   0 root         (0) root         (0)        5 2024-05-12 19:07:30.000000 sagemaker_ssh_helper-2.2.0/sagemaker_ssh_helper/VERSION
+-rw-r--r--   0 root         (0) root         (0)     3271 2024-05-12 19:07:30.000000 sagemaker_ssh_helper-2.2.0/sagemaker_ssh_helper/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1038 2024-05-12 19:07:30.000000 sagemaker_ssh_helper-2.2.0/sagemaker_ssh_helper/aws.py
+-rw-r--r--   0 root         (0) root         (0)    11631 2024-05-12 19:07:30.000000 sagemaker_ssh_helper-2.2.0/sagemaker_ssh_helper/browser_automation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 19:12:14.359341 sagemaker_ssh_helper-2.2.0/sagemaker_ssh_helper/cdk/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-12 19:07:30.000000 sagemaker_ssh_helper-2.2.0/sagemaker_ssh_helper/cdk/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      219 2024-05-12 19:07:30.000000 sagemaker_ssh_helper-2.2.0/sagemaker_ssh_helper/cdk/advanced_tier_app.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 19:12:14.363341 sagemaker_ssh_helper-2.2.0/sagemaker_ssh_helper/cdk/iam_ssm/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-12 19:07:30.000000 sagemaker_ssh_helper-2.2.0/sagemaker_ssh_helper/cdk/iam_ssm/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      284 2024-05-12 19:07:30.000000 sagemaker_ssh_helper-2.2.0/sagemaker_ssh_helper/cdk/iam_ssm/advanced_tier_lambda.py
+-rw-r--r--   0 root         (0) root         (0)     8439 2024-05-12 19:07:30.000000 sagemaker_ssh_helper-2.2.0/sagemaker_ssh_helper/cdk/iam_ssm/iam_ssm_stack.py
+-rw-r--r--   0 root         (0) root         (0)    10544 2024-05-12 19:07:30.000000 sagemaker_ssh_helper-2.2.0/sagemaker_ssh_helper/cdk/iam_ssm/iam_ssm_stack_tests.py
+-rw-r--r--   0 root         (0) root         (0)     1481 2024-05-12 19:07:30.000000 sagemaker_ssh_helper-2.2.0/sagemaker_ssh_helper/cdk/iam_ssm/ssm_advanced_tier_stack.py
+-rw-r--r--   0 root         (0) root         (0)      677 2024-05-12 19:07:30.000000 sagemaker_ssh_helper-2.2.0/sagemaker_ssh_helper/cdk/iam_ssm/trust_relationship_lambda.py
+-rw-r--r--   0 root         (0) root         (0)      185 2024-05-12 19:07:30.000000 sagemaker_ssh_helper-2.2.0/sagemaker_ssh_helper/cdk/iam_ssm_app.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 19:12:14.363341 sagemaker_ssh_helper-2.2.0/sagemaker_ssh_helper/cdk/low_gpu/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-12 19:07:30.000000 sagemaker_ssh_helper-2.2.0/sagemaker_ssh_helper/cdk/low_gpu/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3795 2024-05-12 19:07:30.000000 sagemaker_ssh_helper-2.2.0/sagemaker_ssh_helper/cdk/low_gpu/low_gpu_lambda.py
+-rw-r--r--   0 root         (0) root         (0)     2580 2024-05-12 19:07:30.000000 sagemaker_ssh_helper-2.2.0/sagemaker_ssh_helper/cdk/low_gpu/low_gpu_lambda_stack.py
+-rw-r--r--   0 root         (0) root         (0)      207 2024-05-12 19:07:30.000000 sagemaker_ssh_helper-2.2.0/sagemaker_ssh_helper/cdk/low_gpu_lambda_app.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 19:12:14.363341 sagemaker_ssh_helper-2.2.0/sagemaker_ssh_helper/cdk/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-12 19:07:30.000000 sagemaker_ssh_helper-2.2.0/sagemaker_ssh_helper/cdk/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 19:12:14.363341 sagemaker_ssh_helper-2.2.0/sagemaker_ssh_helper/cdk/tests/unit/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-12 19:07:30.000000 sagemaker_ssh_helper-2.2.0/sagemaker_ssh_helper/cdk/tests/unit/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      207 2024-05-12 19:07:30.000000 sagemaker_ssh_helper-2.2.0/sagemaker_ssh_helper/cdk/tests_app.py
+-rw-r--r--   0 root         (0) root         (0)     2276 2024-05-12 19:07:30.000000 sagemaker_ssh_helper-2.2.0/sagemaker_ssh_helper/deregister_old_instances_from_ssm.py
+-rw-r--r--   0 root         (0) root         (0)     2242 2024-05-12 19:07:30.000000 sagemaker_ssh_helper-2.2.0/sagemaker_ssh_helper/detached_sagemaker.py
+-rw-r--r--   0 root         (0) root         (0)      761 2024-05-12 19:07:30.000000 sagemaker_ssh_helper-2.2.0/sagemaker_ssh_helper/env.py
+-rw-r--r--   0 root         (0) root         (0)    14398 2024-05-12 19:07:30.000000 sagemaker_ssh_helper-2.2.0/sagemaker_ssh_helper/ide.py
+-rw-r--r--   0 root         (0) root         (0)    19825 2024-05-12 19:07:30.000000 sagemaker_ssh_helper-2.2.0/sagemaker_ssh_helper/interactive_sagemaker.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 19:12:14.363341 sagemaker_ssh_helper-2.2.0/sagemaker_ssh_helper/js/
+-rw-r--r--   0 root         (0) root         (0)        6 2024-05-12 19:07:30.000000 sagemaker_ssh_helper-2.2.0/sagemaker_ssh_helper/js/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1641 2024-05-12 19:07:30.000000 sagemaker_ssh_helper-2.2.0/sagemaker_ssh_helper/js/drop_studio_file.js
+-rw-r--r--   0 root         (0) root         (0)    12361 2024-05-12 19:07:30.000000 sagemaker_ssh_helper-2.2.0/sagemaker_ssh_helper/log.py
+-rw-r--r--   0 root         (0) root         (0)     9749 2024-05-12 19:07:30.000000 sagemaker_ssh_helper-2.2.0/sagemaker_ssh_helper/manager.py
+-rw-r--r--   0 root         (0) root         (0)     7473 2024-05-12 19:07:30.000000 sagemaker_ssh_helper-2.2.0/sagemaker_ssh_helper/proxy.py
+-rw-r--r--   0 root         (0) root         (0)     6270 2024-05-12 19:07:30.000000 sagemaker_ssh_helper-2.2.0/sagemaker_ssh_helper/sm-connect-ssh-proxy
+-rw-r--r--   0 root         (0) root         (0)     8382 2024-05-12 19:07:30.000000 sagemaker_ssh_helper-2.2.0/sagemaker_ssh_helper/sm-helper-functions
+-rw-r--r--   0 root         (0) root         (0)     2680 2024-05-12 19:07:30.000000 sagemaker_ssh_helper-2.2.0/sagemaker_ssh_helper/sm-init-ssm
+-rw-r--r--   0 root         (0) root         (0)     1503 2024-05-12 19:07:30.000000 sagemaker_ssh_helper-2.2.0/sagemaker_ssh_helper/sm-local-configure
+-rw-r--r--   0 root         (0) root         (0)     5362 2024-05-12 19:07:30.000000 sagemaker_ssh_helper-2.2.0/sagemaker_ssh_helper/sm-local-ssh-ide
+-rw-r--r--   0 root         (0) root         (0)     1592 2024-05-12 19:07:30.000000 sagemaker_ssh_helper-2.2.0/sagemaker_ssh_helper/sm-local-ssh-inference
+-rw-r--r--   0 root         (0) root         (0)     1492 2024-05-12 19:07:30.000000 sagemaker_ssh_helper-2.2.0/sagemaker_ssh_helper/sm-local-ssh-notebook
+-rw-r--r--   0 root         (0) root         (0)     1598 2024-05-12 19:07:30.000000 sagemaker_ssh_helper-2.2.0/sagemaker_ssh_helper/sm-local-ssh-processing
+-rw-r--r--   0 root         (0) root         (0)     1606 2024-05-12 19:07:30.000000 sagemaker_ssh_helper-2.2.0/sagemaker_ssh_helper/sm-local-ssh-training
+-rw-r--r--   0 root         (0) root         (0)     1597 2024-05-12 19:07:30.000000 sagemaker_ssh_helper-2.2.0/sagemaker_ssh_helper/sm-local-ssh-transform
+-rwxr-xr-x   0 root         (0) root         (0)     2346 2024-05-12 19:07:30.000000 sagemaker_ssh_helper-2.2.0/sagemaker_ssh_helper/sm-local-start-ssh
+-rw-r--r--   0 root         (0) root         (0)      982 2024-05-12 19:07:30.000000 sagemaker_ssh_helper-2.2.0/sagemaker_ssh_helper/sm-save-env
+-rw-r--r--   0 root         (0) root         (0)     6199 2024-05-12 19:07:30.000000 sagemaker_ssh_helper-2.2.0/sagemaker_ssh_helper/sm-setup-ssh
+-rw-r--r--   0 root         (0) root         (0)    11413 2024-05-12 19:07:30.000000 sagemaker_ssh_helper-2.2.0/sagemaker_ssh_helper/sm-ssh-ide
+-rw-r--r--   0 root         (0) root         (0)     1577 2024-05-12 19:07:30.000000 sagemaker_ssh_helper-2.2.0/sagemaker_ssh_helper/sm-wait
+-rw-r--r--   0 root         (0) root         (0)     8009 2024-05-12 19:07:30.000000 sagemaker_ssh_helper-2.2.0/sagemaker_ssh_helper/sm_ssh.py
+-rw-r--r--   0 root         (0) root         (0)    34992 2024-05-12 19:07:30.000000 sagemaker_ssh_helper-2.2.0/sagemaker_ssh_helper/wrapper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 19:12:14.375341 sagemaker_ssh_helper-2.2.0/sagemaker_ssh_helper.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3047 2024-05-12 19:12:14.000000 sagemaker_ssh_helper-2.2.0/sagemaker_ssh_helper.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2762 2024-05-12 19:12:14.000000 sagemaker_ssh_helper-2.2.0/sagemaker_ssh_helper.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-12 19:12:14.000000 sagemaker_ssh_helper-2.2.0/sagemaker_ssh_helper.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      150 2024-05-12 19:12:14.000000 sagemaker_ssh_helper-2.2.0/sagemaker_ssh_helper.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      557 2024-05-12 19:12:14.000000 sagemaker_ssh_helper-2.2.0/sagemaker_ssh_helper.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2024-05-12 19:12:14.000000 sagemaker_ssh_helper-2.2.0/sagemaker_ssh_helper.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-12 19:12:14.383340 sagemaker_ssh_helper-2.2.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     4881 2024-05-12 19:07:30.000000 sagemaker_ssh_helper-2.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 19:12:14.375341 sagemaker_ssh_helper-2.2.0/tests/
+-rw-r--r--   0 root         (0) root         (0)     1910 2024-05-12 19:07:30.000000 sagemaker_ssh_helper-2.2.0/tests/test_attach.py
+-rw-r--r--   0 root         (0) root         (0)     4606 2024-05-12 19:07:30.000000 sagemaker_ssh_helper-2.2.0/tests/test_batch_inference.py
+-rw-r--r--   0 root         (0) root         (0)     8134 2024-05-12 19:07:30.000000 sagemaker_ssh_helper-2.2.0/tests/test_clean_core.py
+-rw-r--r--   0 root         (0) root         (0)     2828 2024-05-12 19:07:30.000000 sagemaker_ssh_helper-2.2.0/tests/test_cli.py
+-rw-r--r--   0 root         (0) root         (0)     1078 2024-05-12 19:07:30.000000 sagemaker_ssh_helper-2.2.0/tests/test_compiler.py
+-rw-r--r--   0 root         (0) root         (0)      727 2024-05-12 19:07:30.000000 sagemaker_ssh_helper-2.2.0/tests/test_deregister_instances.py
+-rw-r--r--   0 root         (0) root         (0)     4021 2024-05-12 19:07:30.000000 sagemaker_ssh_helper-2.2.0/tests/test_distributed.py
+-rw-r--r--   0 root         (0) root         (0)    18940 2024-05-12 19:07:30.000000 sagemaker_ssh_helper-2.2.0/tests/test_end_to_end.py
+-rw-r--r--   0 root         (0) root         (0)     2380 2024-05-12 19:07:30.000000 sagemaker_ssh_helper-2.2.0/tests/test_environment.py
+-rw-r--r--   0 root         (0) root         (0)    36684 2024-05-12 19:07:30.000000 sagemaker_ssh_helper-2.2.0/tests/test_frameworks.py
+-rw-r--r--   0 root         (0) root         (0)    11019 2024-05-12 19:07:30.000000 sagemaker_ssh_helper-2.2.0/tests/test_functions.py
+-rw-r--r--   0 root         (0) root         (0)     3662 2024-05-12 19:07:30.000000 sagemaker_ssh_helper-2.2.0/tests/test_hpo.py
+-rw-r--r--   0 root         (0) root         (0)    14905 2024-05-12 19:07:30.000000 sagemaker_ssh_helper-2.2.0/tests/test_ide.py
+-rw-r--r--   0 root         (0) root         (0)     2620 2024-05-12 19:07:30.000000 sagemaker_ssh_helper-2.2.0/tests/test_inference_registry.py
+-rw-r--r--   0 root         (0) root         (0)     1732 2024-05-12 19:07:30.000000 sagemaker_ssh_helper-2.2.0/tests/test_local.py
+-rw-r--r--   0 root         (0) root         (0)     6361 2024-05-12 19:07:30.000000 sagemaker_ssh_helper-2.2.0/tests/test_manual.py
+-rw-r--r--   0 root         (0) root         (0)     3272 2024-05-12 19:07:30.000000 sagemaker_ssh_helper-2.2.0/tests/test_model_repack.py
+-rw-r--r--   0 root         (0) root         (0)    15430 2024-05-12 19:07:30.000000 sagemaker_ssh_helper-2.2.0/tests/test_ssm_manager.py
+-rw-r--r--   0 root         (0) root         (0)     1091 2024-05-12 19:07:30.000000 sagemaker_ssh_helper-2.2.0/tests/test_util.py
+-rw-r--r--   0 root         (0) root         (0)      992 2024-05-12 19:07:30.000000 sagemaker_ssh_helper-2.2.0/tests/test_validation.py
```

### Comparing `sagemaker-ssh-helper-2.1.0/LICENSE` & `sagemaker_ssh_helper-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sagemaker-ssh-helper-2.1.0/README.md` & `sagemaker_ssh_helper-2.2.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,194 +1,206 @@
 # SageMaker SSH Helper
 
 [![Latest Version](https://img.shields.io/pypi/v/sagemaker-ssh-helper.svg)](https://pypi.python.org/pypi/sagemaker-ssh-helper)
 [![Supported Python Versions](https://img.shields.io/pypi/pyversions/sagemaker-ssh-helper.svg)](https://pypi.python.org/pypi/sagemaker-ssh-helper)
 [![License](https://img.shields.io/github/license/aws-samples/sagemaker-ssh-helper.svg)](https://github.com/aws-samples/sagemaker-ssh-helper/blob/main/LICENSE)
 
-SageMaker SSH Helper is the "army-knife" library that helps you to securely connect to Amazon SageMaker's training jobs, processing jobs, 
-and realtime inference endpoints as well as SageMaker Studio notebook containers for fast interactive experimentation, 
+SageMaker SSH Helper is the "army-knife" library that helps you to securely connect to Amazon SageMaker training jobs, processing jobs, batch inference jobs
+and realtime inference endpoints as well as SageMaker Studio Notebooks and SageMaker Notebook Instances for fast interactive experimentation, 
 remote debugging, and advanced troubleshooting.
 
-Three most common asks that motivated to create the library, sometimes referred as "SSH into SageMaker", are:
+Three most common tasks that motivated to create the library, sometimes referred as "SSH into SageMaker", are:
 1. A terminal session into a container running in SageMaker to diagnose a stuck training job, use CLI commands 
 like nvidia-smi, or iteratively fix and re-execute your training script within seconds. 
 2. Remote debugging of a code running in SageMaker from your local favorite IDE like 
 PyCharm Professional Edition or Visual Studio Code.
-3. Port forwarding to access diagnostic tools running inside SageMaker, e.g., Dask dashboard, TensorBoard or Spark Web UI.
+3. Port forwarding to access auxiliary tools running inside SageMaker, e.g., Dask dashboard, Streamlit apps, TensorBoard or Spark Web UI.
+
+![Screenshot](images/high-level-architecture.png)
+
+Other tasks include but not limited to connecting to a remote Jupyter Notebook in SageMaker Studio from your IDE, or starting a VNC session to SageMaker Studio to run GUI apps.  
 
-Other asks include but not limited to connecting to a remote Jupyter Notebook in SageMaker Studio from your IDE, or start a VNC session to SageMaker Studio to run GUI apps.  
 
 ## How it works
-SageMaker SSH helper uses AWS Systems Manager (SSM) Session Manager, to register the SageMaker container in SSM, followed by creating an SSM session between your client machine and the SageMaker container. Then you can "SSH into SageMaker" by creating an SSH (Secure Shell) connection on top of the SSM session, that allows opening a Linux shell and configuring bidirectional SSH port forwarding to run applications like remote development, debugging, desktop GUI, and others.
+SageMaker SSH helper uses AWS Systems Manager (SSM) Session Manager, to register a SageMaker container in SSM, followed by creating a session between your client machine and the Session Manager service. From there, you can "SSH into SageMaker" by creating an SSH (Secure Shell) connection on top of the SSM sessions, that allows opening a Linux shell and configuring bidirectional SSH port forwarding to run applications like remote development, debugging, desktop GUI, and others.
 
-![Screenshot](images/high-level-architecture.png)
+![Screenshot](images/guidance-diagram.png)
+
+If you want to understand deeper how both the SageMaker service and the SageMaker SSH Helper library work, check the [Flow Diagrams](Flow_Diagrams.md) of the common use cases and carefully read all sections of the documentation.
 
-Once you become familiar with the library, check the [Flow Diagrams](Flow_Diagrams.md) of the common use cases. 
+Make sure you also looked at our [Frequently Asked Questions](FAQ.md), especially at the [troubleshooting section](FAQ.md#troubleshooting), as well as at the existing both open and resolved [issues](https://github.com/aws-samples/sagemaker-ssh-helper/issues?q=is%3Aissue).
 
-Also make sure you looked at our [Frequently Asked Questions](FAQ.md).
 
 ## Getting started
 
 To get started, your AWS system administrator must configure IAM and SSM in your AWS account as shown 
 in [Setting up your AWS account with IAM and SSM configuration](IAM_SSM_Setup.md).
 
-> **Note**: This solution is a sample AWS content. You should not use this content in your production accounts, in a production 
-> environment or on production or other critical data. If you plan to use the solution in production, please, carefully review it with your security team. 
+> **Note: This repository is a sample AWS content.** You should not use the sample content in your production accounts, in a production 
+> environment or on production or other critical data. If you plan to use the content in production, please, carefully review it with your security team. 
 > You are responsible for testing, securing, and optimizing the sample content 
 > as appropriate for production grade use based on your specific business requirements, including any quality control 
 practices and standards.
 
 
 ## Use Cases
 SageMaker SSH Helper supports a variety of use cases:
-- [Connecting to SageMaker training jobs with SSM](#training) - shell access only, open a shell to a single- or multi-node training job to examine its file systems,
-monitor resources, produce thread-dumps for stuck jobs, and interactively run your train script
+- [Connecting to SageMaker training jobs with SSM](#training) - shell access only, open a shell to a single- or multi-node training job to examine its file systems, monitor resources, produce thread-dumps for stuck jobs, and interactively run your train script
   - [Connecting to SageMaker inference endpoints with SSM](#inference)
   - [Connecting to SageMaker batch transform jobs](#batch-transform)
   - [Connecting to SageMaker processing jobs](#processing)  
 - [Forwarding TCP ports over SSH tunnel](#port-forwarding) - intermediate layer for debugging and remote code execution, enables through SSH and port forwarding the access to remote apps like Dask, Streamlit or Jupyter Notebook
-- [Remote debugging with PyCharm Debug Server over SSH](#pycharm-debug-server) - debugging and remote code execution, uses debug server, lets SageMaker run your code that connects to PyCharm, to start line-by-line debugging with [PyDev.Debugger](https://pypi.org/project/pydevd-pycharm/), a.k.a. pydevd
-- [Remote code execution with PyCharm / VSCode over SSH](#remote-interpreter) - debugging and remote code execution, without debug server, lets PyCharm run or debug your code line-by-line inside SageMaker container with SSH interpreter
-- [Local IDE integration with SageMaker Studio over SSH for PyCharm / VSCode](#studio) - debugging and remote code execution, iterate fast on a single node at early stages of development without submitting SageMaker jobs
-- [Web VNC](#web-vnc) - run any IDE or tool in a browser though [AWS Jupyter Proxy](https://github.com/aws/aws-jupyter-proxy) extension
+  - [sm-ssh](#sm-ssh) - SageMaker SSH Helper CLI, introduced in v2.2
+  - [~/.ssh/config](#sshconfig) - to use `ssh` CLI command instead of `sm-ssh`
+- [Remote code execution with PyCharm / VSCode over SSH](#remote-interpreter) - debugging and remote code execution, lets your IDE run or debug your code line-by-line inside SageMaker container with SSH interpreter, e.g. inside a SageMaker training job
+  - [Remote debugging with PyCharm Debug Server over SSH](#pycharm-debug-server) - debugging and remote code execution, uses debug server, lets SageMaker run your code that connects to PyCharm with a callback, to start line-by-line debugging with [PyDev.Debugger](https://pypi.org/project/pydevd-pycharm/), a.k.a. pydevd
+- [Local IDE integration with SageMaker Studio over SSH for PyCharm / VSCode](#studio) - debugging and remote code execution in SageMaker Studio, iterate fast on a single node at early stages of development without submitting SageMaker jobs
+  - [Support of SageMaker Notebook Instances](FAQ.md#are-sagemaker-notebook-instances-supported) - see FAQ
+- [Web VNC](#web-vnc) - run virtually any IDE or GUI tool in a browser though [AWS Jupyter Proxy](https://github.com/aws/aws-jupyter-proxy) extension and VNC remote desktop protocol
 
-If you want to add a new use case or a feature, see [CONTRIBUTING](CONTRIBUTING.md).
+**Pro Tip**: While multiple use cases allow debugging and remote code execution, the typical development journey looks as follows: (1) you start developing and running code in the IDE on your [local machine](https://aws.amazon.com/blogs/machine-learning/run-your-tensorflow-job-on-amazon-sagemaker-with-a-pycharm-ide/), then (2) you connect the IDE to [SageMaker Studio](https://docs.aws.amazon.com/sagemaker/latest/dg/studio.html) with SageMaker SSH Helper to test and troubleshoot it on the remote instance, then (3) you integrate your code with SageMaker and run it as a [training](https://docs.aws.amazon.com/sagemaker/latest/dg/train-model.html), [processing](https://docs.aws.amazon.com/sagemaker/latest/dg/processing-job.html) or [inference](https://docs.aws.amazon.com/sagemaker/latest/dg/deploy-model.html) job, using SageMaker SSH Helper if needed, and finally (4) assemble jobs into MLOps pipelines with [SageMaker Projects](https://docs.aws.amazon.com/sagemaker/latest/dg/sagemaker-projects.html), to be deployed into multi-account structure on top of (5) the [secure enterprise ML platform](https://docs.aws.amazon.com/whitepapers/latest/build-secure-enterprise-ml-platform/build-secure-enterprise-ml-platform.html).
 
-**Pro Tip**: While multiple use cases allow debugging and remote code execution, the typical development journey looks as follows: (1) you start developing and running code in the IDE on your [local machine](https://aws.amazon.com/blogs/machine-learning/run-your-tensorflow-job-on-amazon-sagemaker-with-a-pycharm-ide/), then (2) you connect the IDE to [SageMaker Studio](https://docs.aws.amazon.com/sagemaker/latest/dg/studio.html) with SageMaker SSH Helper to test and troubleshoot it on the remote instance, then (3) you integrate your code with SageMaker and run it as a [training](https://docs.aws.amazon.com/sagemaker/latest/dg/train-model.html), [processing](https://docs.aws.amazon.com/sagemaker/latest/dg/processing-job.html) or [inference](https://docs.aws.amazon.com/sagemaker/latest/dg/deploy-model.html) job with SageMaker SSH Helper and finally (4) assemble jobs into MLOps pipelines with [SageMaker Projects](https://docs.aws.amazon.com/sagemaker/latest/dg/sagemaker-projects.html).
+If you want to add a new use case or a feature, see [CONTRIBUTING](CONTRIBUTING.md).
 
 
 ## <a name="training"></a>Connecting to SageMaker training jobs with SSM
 
 [![Download Demo (.mov)](https://user-images.githubusercontent.com/87804596/205893540-d7a08259-94b3-48f2-b96e-93798b98a06c.png)](https://aws-blogs-artifacts-public.s3.amazonaws.com/artifacts/ML-4988/SSH_Helper-Shell-To-Training-Jobs.mov)
 [Download Demo (.mov)](https://aws-blogs-artifacts-public.s3.amazonaws.com/artifacts/ML-4988/SSH_Helper-Shell-To-Training-Jobs.mov)
 
+> **Note**: This demo is recorded with a previous version of SSH Helper and may be not up-to-date with the recent features. Check the below documentation for the most up-to-date steps.
+
 ### Step 1: Install the library
 Before starting the whole procedure, check that both `pip` and `python` commands point to Python version 3.7 or higher with `python --version` command. 
 
+> **Important:** Make sure you read the "Getting started" section and didn't skip the steps from [Setting up your AWS account with IAM and SSM configuration](IAM_SSM_Setup.md).
+
 Install the latest stable version of library from the [PyPI repository](https://pypi.org/project/sagemaker-ssh-helper/):
 
 ```shell
 pip install sagemaker-ssh-helper
 ```
+**Caution:** It's always recommended to install the library into a Python venv, not into the system env.
 
 ### Step 2: Modify your start training job code
-1. Add import for SSHEstimatorWrapper
-2. Add a `dependencies` parameter to the Estimator object. Alternatively, add `sagemaker_ssh_helper` into `requirements.txt`.
-3. Add an `SSHEstimatorWrapper.create(estimator,...)` call before calling `fit()` and add SageMaker SSH Helper 
-as `dependencies`.
-4. Add a call to `ssh_wrapper.get_instance_ids()` to get the SSM instance(s) id. We'll use this as the target 
-to connect to later on.   
+1. Add import for `SSHEstimatorWrapper`
+2. Add a `dependencies` parameter to the `Estimator` object constructor. Alternatively, instead of `dependencies` parameter, put `sagemaker_ssh_helper` into `source_dir/training/requirements.txt`.
+3. Add an `SSHEstimatorWrapper.create(estimator,...)` call before calling `fit()`.
+4. Add a call to `ssh_wrapper.print_ssh_info()` or `ssh_wrapper.get_instance_ids()` to get the SSM instance(s) id. You'll use this information
+to connect to the instance later on.   
 
-For example:
+In a nutshell:
 
 ```python
 import logging
 from sagemaker.pytorch import PyTorch
 from sagemaker_ssh_helper.wrapper import SSHEstimatorWrapper  # <--NEW--
 
 role = ...
 
 estimator = PyTorch(
     entry_point='train.py',
     source_dir='source_dir/training/',
-    dependencies=[SSHEstimatorWrapper.dependency_dir()],  # <--NEW 
-    # (alternatively, add sagemaker_ssh_helper into requirements.txt 
-    # inside source dir) --
+    dependencies=[SSHEstimatorWrapper.dependency_dir()],  # <--NEW--
     role=role,
     framework_version='1.9.1',
     py_version='py38',
     instance_count=1,
     instance_type='ml.m5.xlarge'
 )
 
 ssh_wrapper = SSHEstimatorWrapper.create(estimator, connection_wait_time_seconds=600)  # <--NEW--
 
 estimator.fit(wait=False)
 
-logging.info(f"To connect over SSH run: sm-local-ssh-training connect {ssh_wrapper.training_job_name()}")
-
-instance_ids = ssh_wrapper.get_instance_ids(timeout_in_sec=900)  # <--NEW-- 
-
-logging.info(f"To connect over SSM run: aws ssm start-session --target {instance_ids[0]}")
+ssh_wrapper.print_ssh_info()  # <--NEW-- 
 ```
 
-*Note:* `connection_wait_time_seconds` is the amount of time the SSH helper will wait inside SageMaker before it continues normal execution. It's useful for training jobs, when you want to connect before training starts.
-If you don't want to wait and start training as soon as the job starts, set it to 0.
+The `connection_wait_time_seconds` is the amount of time the SSH Helper will wait inside SageMaker before it continues the job execution. It's useful for training jobs, when you want to connect before training starts.
+If you don't want the job to wait and start training as soon as the job starts, set it to `0`.
 
-*Note:* If you use distributed training (i.e., `instance_count > 1`), SSH Helper
-will start by default only on the first 2 nodes (e.g., on `algo-1` and `algo-2`).
-If you want to connect to SSH to other nodes, you can log in to either of these nodes, e.g., `algo-1`,
+As an example, here's the full working code from a unit test: [test_end_to_end.py#L31-L56](https://github.com/aws-samples/sagemaker-ssh-helper/blob/v2.1.0/tests/test_end_to_end.py#L31-L56) . The method `start_ssm_connection_and_continue(port_number)` will connect to the instance through API, terminate the waiting loop and start training (useful for automation).
+
+If you configured distributed training (i.e., `instance_count` is more than one), SSH Helper
+will start by default only on the first two nodes (i.e., on `algo-1` and `algo-2`).
+If you want to connect with SSH to other nodes, you can log in to either of these nodes, e.g., `algo-2`,
 and then SSH from this node to any other node of the training cluster, e.g., `algo-4`, without running SSH Helper 
-on these nodes (in pre-build SageMaker framework containers like PyTorch training container just type `ssh algo-4`).
+on these nodes, e.g., inside the pre-build SageMaker framework containers like PyTorch training container just run `ssh algo-4` from the shell.
 
-Alternatively, pass the additional parameter `ssh_instance_count` with the desired instance count 
-to `SSHEstimatorWrapper.create()`.
+Alternatively, for distributed training, pass the additional parameter `ssh_instance_count` with the desired instance count 
+to `SSHEstimatorWrapper.create()`, e.g., `SSHEstimatorWrapper.create(..., ssh_instance_count=3)`
 
 *Note:* if you a/ don't use script mode, b/ use basic `Estimator` class and c/ all code is already stored in your Docker container, check the code sample in [the corresponding section of the FAQ](FAQ.md#what-if-i-want-to-train-and-deploy-a-model-as-a-simple-estimator-in-my-own-container-without-passing-entry_point-and-source_dir).
 
+Don't run the modified code yet, see the next step.
 
 ### Step 3: Modify your training script
-Add into your `train.py` the following lines at the top:
 
 ```python
 import sagemaker_ssh_helper
 sagemaker_ssh_helper.setup_and_start_ssh()
 ```
 
-The `setup_and_start_ssh()` will start an SSM agent that will connect the training instance to AWS Systems Manager.
+The `setup_and_start_ssh()` will start an SSM Agent that will connect the training instance to AWS Systems Manager.
+
+See the [train.py](https://github.com/aws-samples/sagemaker-ssh-helper/blob/v2.1.0/tests/source_dir/training/train.py) from the corresponding unit test, as a full working code sample.
 
 ### Step 4: Connect over SSM
-Once you launched the job, you'll need to wait, a few minutes, for the SageMaker container to start and the SSM agent
+Once you launched the job, you'll need to wait, a few minutes, for the SageMaker container to start and the SSM Agent
 to start successfully. Then you'll need to have the ID of the managed instance. The instance id is prefixed by `mi-` 
 and will appear in the job's CloudWatch log like this:
 
 ```text
 Successfully registered the instance with AWS SSM using Managed instance-id: mi-1234567890abcdef0
 ``` 
 
-To fetch the instance IDs in an automated way, call the Python method `ssh_wrapper.get_instance_ids()`, 
-as mentioned in the previous step:
+To fetch the instance IDs in an automated way without looking into the logs, you can call the Python method `ssh_wrapper.get_instance_ids()` or `ssh_wrapper.print_ssh_info()`, as mentioned in the step 1:
 
 ```python
 estimator = ...
 ssh_wrapper = ...
 estimator.fit(wait=False)
 instance_ids = ssh_wrapper.get_instance_ids(timeout_in_sec=900)
 ```
 
 The method `get_instance_ids()` accepts the optional parameter `timeout_in_sec` (default is 900, i.e., 15 minutes). 
 If timeout is not 0, it will retry attempts to get instance IDs every 10 seconds.
 
-With the instance id at hand, you will be able to connect to the training container using the command line or the AWS web console:  
+With the instance ID at hand, you will be able to connect to the training container using the command line or the AWS web console. 
 
-A. Connecting using command line:  
+Method A. Connecting using command line:  
 
 1. On the local machine, make sure that you installed the latest [AWS CLI v2](https://docs.aws.amazon.com/cli/latest/userguide/getting-started-install.html) and the [AWS Session Manager CLI plugin](https://docs.aws.amazon.com/systems-manager/latest/userguide/session-manager-working-with-install-plugin.html). Run the following command to perform the installation:
 
 ```shell
 sm-local-configure
 ```
 
-*Note:* If you start your training job from SageMaker Studio notebook, and execute the installation command from the image terminal, make sure that Python environment is activated, e.g., with `conda activate base`.
-
 2. Run this command (replace the target value with the instance id for your SageMaker job). Example:
 ```shell
 aws ssm start-session --target mi-1234567890abcdef0
 ```
 
-B. Connecting using the AWS Web Console:  
+**Note:** Recently SageMaker has introduced [the native way to connect to training jobs with SSM](https://docs.aws.amazon.com/sagemaker/latest/dg/train-remote-debugging.html). 
+
+Method B. Connecting using the AWS Web Console:  
 
   1. In AWS Web Console, navigate to Systems Manager > Fleet Manager.     
   2. Select the node, then Node actions > Start terminal session.
 
-Once connected to the container, you would want to switch to the root user with `sudo su -` command.
+Once connected to the container, you might want to switch to the root user with `sudo su -` command.
 
-C. Connecting with SSH and port forwarding:
+Method C. Connecting with SSH and port forwarding:
+
+This method uses `sm-ssh connect` command and described in more details in the section [sm-ssh](#sm-ssh).
+
+Method D. Connecting from SageMaker Studio
+
+See the corresponding step [Connecting from SageMaker Studio](IAM_SSM_Setup.md#4-optional-connecting-from-sagemaker-studio) in IAM / SSM configuration section. Follow the same steps as in the Method A for the local machine, but run them inside SageMaker Studio. If you run the commands from SageMaker Studio image terminal, make sure that your Python environment is activated, e.g., with `conda activate base`.
 
-This method uses `sm-local-ssh-training connect` command and described in more details in the section [Forwarding TCP ports over SSH tunnel](README.md#port-forwarding).
 
 #### <a name="cli-commands"></a>Tip: Useful CLI commands
 
 Here are some useful commands to run in a terminal session:  
 - `ps xfaww` - Show running tree of processes
 - `ps xfawwe` - Show running tree of processes with environment variables 
 - `ls -l /opt/ml/input/data` - Show input channels
@@ -219,14 +231,16 @@
 `sudo strace -p 361`
 
 #### <a name="cli-commands"></a>Tip: Pipeline automation
 If you're looking for the full automation of the pipeline with SSM and SSH, and not only with `get_instance_ids()` method, take a look at the [automation question in the FAQ](FAQ.md#how-do-i-automate-my-pipeline-with-sagemaker-ssh-helper-end-to-end).
 
 ## <a name="inference"></a>Connecting to SageMaker inference endpoints with SSM
 
+**Note:** Recently SageMaker has introduced [the native way to connect to endpoints with SSM](https://docs.aws.amazon.com/sagemaker/latest/dg/ssm-access.html), but it requires allow-listing of an AWS account (as of writing).
+
 Adding SageMaker SSH Helper to inference endpoint is similar to training with the following differences.
 
 1. Wrap your model into `SSHModelWrapper` before calling `deploy()` and add SSH Helper to `dependencies`:
 
 ```python
 from sagemaker import Predictor
 from sagemaker_ssh_helper.wrapper import SSHModelWrapper  # <--NEW--
@@ -255,16 +269,15 @@
 predicted_value = predictor.predict(data=...)
 ```
 
 *Note:* For the inference endpoint, which is always up and running, there's not too much value 
 in setting `connection_wait_time_seconds`, so it's usually set to `0`.
 
 Similar to training jobs, you can fetch the instance ids for connecting to the endpoint with SSM with 
-`ssh_wrapper.get_instance_ids()`.
-
+`ssh_wrapper.get_instance_ids()` or `ssh_wrapper.print_ssh_info()`.
 
 2. Add the following lines at the top of your `inference_ssh.py` script:
 
 ```python
 import os
 import sys
 sys.path.append(os.path.join(os.path.dirname(__file__), "lib"))
@@ -272,14 +285,21 @@
 import sagemaker_ssh_helper
 sagemaker_ssh_helper.setup_and_start_ssh()
 ```
 
 *Note:* adding `lib` dir to Python path is required, because SageMaker inference is putting dependencies 
 into the `code/lib` directory, while SageMaker training put libs directly to `code`. 
 
+On the following screenshot you see the sample code for the notebook [Deploy SD2.1 to Inferentia2 + SageMaker + HF Optimum Neuron + SageMaker SSH Helper](https://github.com/aws-samples/ml-specialized-hardware/blob/main/tutorials/04_ImageGenerationWithStableDiffusion/SDOnInf2AndHFOptimumNeuron_SMSSH.ipynb) that has the inference code running in SageMaker endpoint on AWS Inferentia accelerator chip.
+The user has connected to the endpoint with the `sm-ssh connect` command and executed the `neuron-ls` command to list the currently utilized Inferentia cores:
+
+![](images/sm_ssh_inf2.png)
+
+You can also notice on the screenshot that the user configured the remote Python interpreter that connects to SageMaker Studio, so the user also executes the notebook itself remotely inside SageMaker. This setup is further described in the section for [Local IDE Integration with SageMaker Studio](#studio).
+
 ### Multi-model endpoints
 
 For multi-model endpoints, the setup procedure is slightly different from regular endpoints:
 
 ```python
 from sagemaker.multidatamodel import MultiDataModel
 from sagemaker_ssh_helper.wrapper import SSHModelWrapper, SSHMultiModelWrapper  # <--NEW--
@@ -309,26 +329,26 @@
 
 mdm.add_model(model_data_source=model.repacked_model_data, model_data_path=model_name)
 
 predicted_value = predictor.predict(data=..., target_model=model_name)
 ```
 
 **Important:** Make sure that you're passing to `add_model()` the model ready for deployment with dependencies located at `model.repacked_model_data`,
-not the `estimator.model_data` that points to the trained model artifact. To obtain model suitable for inference, you might want to deploy first your model to a temporary single-node endpoint, so that SageMaker Python SDK takes care of repacking the model.
+not the `estimator.model_data` that points to the trained model artifact. To obtain model suitable for inference, you might want to deploy first your model to a temporary single-node endpoint, so that SageMaker Python SDK takes care of repacking the model, or call the `prepare_container_def()` method, like in [the MMS test code](https://github.com/aws-samples/sagemaker-ssh-helper/blob/v2.1.0/tests/test_end_to_end.py#L252-L323).
 
 Also note that SageMaker SSH Helper will be lazy loaded together with your model upon the first prediction request.
 So you should try to connect to the multi-model endpoint only after calling `predict()`.
 
 The `inference.py` script is the same as for regular endpoints.
 
-If you are using PyTorch containers, make sure you select the latest versions, 
+*Note:* If you are using PyTorch containers, make sure you select the latest versions, 
 e.g. 1.12, 1.11, 1.10 (1.10.2), 1.9 (1.9.1).
 This code might not work if you use PyTorch 1.8, 1.7 or 1.6.
 
-*Note:* if you're packing your models manually and don't pass the `model` object to the `MultiDataModel` constructor, i.e., pass only the `image_uri`, see corresponding sample code in the [FAQ.md](FAQ.md#what-if-i-want-to-deploy-a-multi-data-model-without-passing-a-reference-to-a-model-object-only-with-image_uri).
+*Note:* If you're packing your models manually and don't pass the `model` object to the `MultiDataModel` constructor, i.e., pass only the `image_uri`, see corresponding sample code in the [FAQ.md](FAQ.md#what-if-i-want-to-deploy-a-multi-data-model-without-passing-a-reference-to-a-model-object-only-with-image_uri).
 
 ## <a name="batch-transform"></a>Connecting to SageMaker batch transform jobs
 
 For batch transform jobs, you need to use both `SSHModelWrapper` and `SSHTransformerWrapper`, 
 as in the following example:
 
 ```python
@@ -457,137 +477,159 @@
   -R localhost:12345:localhost:12345 \
   -L localhost:8787:localhost:8787 \
   -L localhost:11022:localhost:22
 ```
 
 You can pass `-L` parameters for forwarding remote container port to local machine (e.g., `8787` for [Dask dashboard](https://docs.dask.org/en/stable/dashboard.html) or `8501` for [Streamlit apps](https://docs.streamlit.io/library/get-started)) or `-R` for forwarding local port to remote container. Read more about these options in the [SSH manual](https://man.openbsd.org/ssh).
 
-This low-level script takes the managed instance ID as a parameter. Next sections describe how to use the higher-level APIs that take the SageMaker resource name as a parameter and resolve it into the instance ID automatically (a.k.a. `sm-local-ssh-*` scripts):
+This low-level script takes the managed instance ID as a parameter. Next sections use the high-level command `sm-ssh` that take the SageMaker resource name as a parameter and resolves it into the instance ID automatically.
 
-* `sm-local-ssh-training`
-* `sm-local-ssh-processing`
-* `sm-local-ssh-inference`
-* `sm-local-ssh-transform`
-* `sm-local-ssh-ide`
+### sm-ssh
 
-## <a name="pycharm-debug-server"></a>Remote debugging with PyCharm Debug Server over SSH
+The syntax for the SSH Helper CLI command `sm-ssh` is the following:
 
-This procedure uses PyCharm's Professional feature: [Remote debugging with the Python remote debug server configuration](https://www.jetbrains.com/help/pycharm/remote-debugging-with-product.html#remote-debug-config)
-
-1. On the local machine, make sure that you installed the latest [AWS CLI v2](https://docs.aws.amazon.com/cli/latest/userguide/getting-started-install.html) and the [AWS Session Manager CLI plugin](https://docs.aws.amazon.com/systems-manager/latest/userguide/session-manager-working-with-install-plugin.html). Run the following command to perform the installation:
-
-```shell
-sm-local-configure
+```bash
+sm-ssh [-h] [-v] {list,start-proxy,connect} [fqdn]
 ```
 
-2. In PyCharm, go to the Run/Debug Configurations (Run -> Edit Configurations...), add a new Python Debug Server.
-Choose the fixed port, e. g. `12345`.
+where `fqdn` is the resource name with `.sagemaker` suffix, respectively:
 
-3. Take the correct version of `pydevd-pycharm` package from the configuration window 
-and install it either through `requirements.txt` or by calling `pip` from your source code.
+* for model training, `.training.sagemaker`
+* for inference endpoints, i.e., real-time inference, `.inference.sagemaker`
+* for transform jobs, i.e., batch inference, `.transform.sagemaker`
+* for processing jobs, i.e. transforms without a trained model, `.processing.sagemaker`
+* for SageMaker Studio Classic, `.studio.sagemaker` - see [Local IDE integration with SageMaker Studio over SSH](#studio) for more details on FQDN format
+* for SageMaker Notebook instances, `.notebook.sagemaker`
 
-4. Add commands to connect to the Debug Server to your code **after** the `setup_and_start_ssh()` (e.g., into [a training script](https://github.com/aws-samples/sagemaker-ssh-helper/blob/main/tests/source_dir/training_debug/train_debug.py) that you submit as an entry point for a training job):
-```python
-import pydevd_pycharm
-pydevd_pycharm.settrace('localhost', port=12345, stdoutToServer=True, stderrToServer=True, suspend=True)
+For `list` command, the resource name and the dot `.` in the suffix can be omitted, i.e.:
+
+```bash
+sm-ssh list studio.sagemaker
 ```
-*Tip*: Check the argument's description in [the library source code](https://github.com/JetBrains/intellij-community/blob/dee787ef05d1187a71b7667652f6b25f3f573a1b/python/helpers/pydev/pydevd.py#L1663).
 
-5. Set extra breakpoints in your code with PyCharm, if needed
-6. Start the Debug Server in PyCharm
-7. Submit your code to SageMaker with SSH Helper as described in previous sections.
-Make sure you allow enough time for manually setting up the connection
-(do not set `connection_wait_time_seconds` to `0`, recommended minimum value is `600`, i.e. 10 minutes).
-Don't worry to set it to higher values, e.g. to 30 min, because you will be able to terminate the waiting loop 
-once you connect.
+– will list all running jupyter servers and kernel gateways and their SSH status, and
 
-8. On your local machine, once the SSH helper connects to SSM and starts waiting inside the training job, start the port forwarding script :
-```shell
-sm-local-ssh-training connect <<training_job_name>>
 ```
-It will reverse-forward the remote debugger port `12345` to your local machine's Debug Server port.
-The local port `11022` will be connected to the remote SSH server port, 
-to allow you easily connect with SSH from command line.  
+sm-ssh list 
+```
+or
+```
+sm-ssh list sagemaker 
+```
 
-> *Note:* Before running this command make sure that AWS CLI is configured to access the account with `aws s3 ls` and your default region is set with `aws configure` command. Your Python's `<path-to-venv>/bin/` directory should be in the `$PATH`, otherwise you will get a *"command not found"* error.
+– will list all resources of all types.
 
-*Tip:* If you want to connect processing, batch transform jor or to an inference endpoint with SSH, use
-`sm-local-ssh-processing`, `sm-local-ssh-transform` or `sm-local-ssh-inference` scripts respectively.
+The instances with SSH Helper will be marked `Online` while other instances will be marked with `-`.
 
-Feel free to use the scripts as templates. Clone and customize them, if you want to change the ports.
+The `connect` command starts interactive SSH session into container, e.g.:
 
-9. On your local machine, add the following configuration to `~/.ssh/config`:
+```bash
+sm-ssh connect ssh-training-example-2023-07-25-03-18-04-490.training.sagemaker
+```
 
-```text
-Host sagemaker-training
-  HostName localhost
-  IdentityFile ~/.ssh/sagemaker-ssh-gw
-  Port 11022
+#### ~/.ssh/config
+
+Alternatively, instead of using `sm-ssh connect` command, you can use the native `ssh` command, but it will require you to update your [ssh config](https://linux.die.net/man/5/ssh_config), typically `~/.ssh/config`, with `sm-ssh start-proxy` command as follows:
+
+```bash
+Host *.*.sagemaker
+  IdentityFile ~/.ssh/%h
+  PasswordAuthentication no
+  ConnectTimeout 90
+  ServerAliveInterval 15
+  ServerAliveCountMax 4
+  ProxyCommand sm-ssh start-proxy %h
   User root
 ```
 
-*Note:* The SSH key specified as `IdentityFile` is automatically generated on your local machine every time when you run `sm-local-ssh-training` command from the step 8.
+You can copy the same fragment from the [ssh_config_template.txt](ssh_config_template.txt) file.
 
-While the `sm-local-ssh-training` script is running, you *may* connect with SSH to the specified local port (but it's not needed for PyCharm Debugger to work). Run on your local machine: 
+The `sm-ssh start-proxy` command will set up the non-interactive SSH session that will serve as a proxy tunnel for SSH command. 
 
-```shell
-ssh sagemaker-training
+As a benefit, you will be able to add additional SSH options like forwarding SSH agent connection with `-A` option, to securely pass your local SSH keys to remote machine, or forward ports with `-R` and `-L` options, akin to passing these options to `sm-local-start-ssh` command. 
+
+An example with [SSH Agent](https://linux.die.net/man/1/ssh-agent) and forwarding the web server port `8080`:
+```bash
+ssh-add
+ssh -A -L localhost:8080:localhost:8080 \
+  ssh-training-example-2023-07-25-03-18-04-490.training.sagemaker
 ```
 
-*Tip:* If you log in to the node with SSH and don't see a `sm-wait` process, the training script has already started 
-and failed to connect to the PyCharm Debug Server, so you need to increase the `connection_wait_time_seconds`, 
-otherwise the debugger will miss your breakpoints.
+As a drawback, you won't get a comprehensive logging since the output of `sm-ssh` will be suspended by ssh. In case you have connection issues with native `ssh`, try the `sm-ssh` command instead and check the output. 
 
-*Tip:* If you don't want `ssh` command to complain about remote host keys, when you switch to a different node,
-consider adding this two options to the command: `-o StrictHostKeyChecking=no -o UserKnownHostsFile=/dev/null`.
+Follow the steps in the next section for the IDE configuration, to prepare the `sm-ssh` for the use on the local machine. 
 
-10. Stop the waiting loop – connect to the instance and terminate the loop.
+## <a name="remote-interpreter"></a>Remote code execution with PyCharm / VSCode over SSH
 
-As already mentioned, make sure you've put enough timeout to allow the port forwarding script set up a tunnel 
-before execution of your script continues.
+1. On the local machine, make sure that you installed the latest [AWS CLI v2](https://docs.aws.amazon.com/cli/latest/userguide/getting-started-install.html) and the [AWS Session Manager CLI plugin](https://docs.aws.amazon.com/systems-manager/latest/userguide/session-manager-working-with-install-plugin.html). To do so, perform the automated installation with the [sm-local-configure](sagemaker_ssh_helper/sm-local-configure) script:
 
-You can use the following CLI command from your local machine to stop the waiting loop (the `sm-wait` remote process):
 ```shell
-sm-local-ssh-training stop-waiting
+sm-local-configure
 ```
 
-Alternatively, if logged to the remote container already, run the `sm-wait stop` command from its shell (under `root`):
-```text
-sm-wait stop
-```
+**Caution**: If you plan to use `sm-ssh` tool from the IDE, which you run inside your system Python env, you should install SSH Helper into your system Python env, too.
 
-11. After you stop the waiting loop, your code will continue running and will connect to your PyCharm Debug Server.
+2. Submit your code to SageMaker with SSH Helper as described in previous sections, e.g. as a [training job](#step-1-install-the-library).
 
-If everything is set up correctly, and you followed all the steps, PyCharm will stop at your breakpoint, highlight the line and wait for your input. Debug Server window will say “connected”. You can now press, for example, F8 to "Step Over" the code line or F7 to "Step Into" the code line.
+Make sure you allow enough time for manually setting up the connection (do not set `connection_wait_time_seconds` to `0`, recommended minimum value is `600`, i.e. 10 minutes).  Don't worry to set it to higher values, e.g. to 30 min, because you will be able to terminate the waiting loop once you connected.
 
-## <a name="remote-interpreter"></a>Remote code execution with PyCharm / VSCode over SSH
+Instead of using SSM to connect to the container from command line, proceed to the next step for configuring the IDE.
 
-Follow the steps from the section [Remote debugging with PyCharm Debug Server](#pycharm-debug-server), but skip the steps 2, 3, 4 and 11 that configure Remote Debug Server.
+3. Configure the remote interpreter in your IDE
 
-Instead, you need to configure the remote Python interpreter. Use `sagemaker-training` as the host name in an IDE dialog. 
+Make sure you've configured your ssh config as mentioned in the [~/.ssh/config](#sshconfig) section and your IDE can access `sm-ssh` command from the system env.
 
- * [Instructions for PyCharm](https://www.jetbrains.com/help/pycharm/remote-debugging-with-product.html#remote-interpreter)
+A. Follow the [instructions in the PyCharm docs](https://www.jetbrains.com/help/pycharm/remote-debugging-with-product.html#remote-interpreter), to configure the remote interpreter in PyCharm.
 
-In PyCharm, use `11022` as the port and `root` as the user.
+In the field for host name, put the same value as for `fqdn` in the [`sm-ssh` command](#sm-ssh), e.g., `ssh-training-manual-2023-10-02-14-38-56-744.training.sagemaker`, and use `root` as the username.
 
 ![](images/pycharm_training.png)
 
- * [Instructions for VSCode](https://code.visualstudio.com/docs/remote/ssh)
+When PyCharm asks for the SSH key, point to the `~/.ssh/<fqdn>` private key file that was automatically generated for you by SSH Helper:
+
+![](images/pycharm_training_ssh.png)
+
+*Note:* If PyCharm says connection refused, it can be due to timeout. Check that you can connect to this host from your system terminal with `ssh` and `sm-ssh` and try configuring the remote interpreter again.
+
+*Tip:* When you configure Python interpreter in PyCharm, it's recommended to configure [the deployment path mapping](https://www.jetbrains.com/help/pycharm/creating-local-server-configuration.html#mapping) for you project to point into `/root/project_name` instead of default `/tmp/pycharm_project_123`. This is how you will be able to see your project in SageMaker Studio and PyCharm will automatically sync your local dir to the remote dir. 
+
+*Tip:* Also instead of creating a new venv, point the Python interpreter to the existing location. 
+You can find this location by running a cell with `import sys; sys.executable` command in a SageMaker Studio notebook. You will get something like `/opt/conda/bin/python`.
+
+*Tip:* Now you also can [upload and download files from remote](https://www.jetbrains.com/help/pycharm/uploading-and-downloading-files.html) and [synchronize files with remote](https://www.jetbrains.com/help/pycharm/comparing-deployed-files-and-folders-with-their-local-versions.html).
+
+B. Follow the [instructions for VSCode](https://code.visualstudio.com/docs/remote/ssh), to configure local Visual Studio Code app
+
+Put the `root@fqdn` as the hostname to connect to, e.g., `root@ssh-training-example-2023-07-25-03-18-04-490.training.sagemaker` .
 
 ![](images/vscode_training.png)
 
+> **NOTE:**  The **Remote SSH** extension described in the above instructions is only for the [Visual Studio Code native app](https://code.visualstudio.com/). Code Editor in SageMaker Studio and web apps based on [Code Server](https://github.com/coder/code-server) that use extensions from [Open VSX Registry](https://open-vsx.org/) might look and work differently. SageMaker SSH Helper **DOES NOT** support browser-based implementations and haven't been tested with any of Open VSX extensions. If you prefer to use the browser for development, take a look at the [Web VNC](#web-vnc) option. 
+
+4. Connect to the instance and stop the waiting loop
+
+When you set `connection_wait_time_seconds` to non-zero value, SSH Helper will run a waiting loop inside your training script, until waiting time is passed, or you manually terminate the loop.
+
+To manually terminate the loop, run the `sm-wait stop` command from the container (under `root`):
+```bash
+ssh root@ssh-training-example-2023-07-25-03-18-04-490.training.sagemaker \
+  sm-wait stop
+```
+
 Note, that if you stop the waiting loop, SageMaker will run your training script only once, and you will be able to execute additional code from local machine from PyCharm only while your script is running. Once the script finishes, you will need to submit another training job and repeat the procedure again.
 
-But there's a useful trick: submit a dummy script `train_placeholder.py` with the infinite loop, and while this loop will be running, you can run your real training script again and again with the remote interpreter inside the same job without submitting a new training job.
+Here's a useful trick: submit a dummy script `train_placeholder.py` with the infinite loop, and while this loop will be running, you can rerun your real training script again and again with the remote interpreter inside the same job.
 
 The workflow in this case is roughly the following:
 
-1. You submit a first job with your training script `train.py`, and it fails for some reason that you want to troubleshoot.
-2. You submit a second job with the placeholder script `train_placeholder.py`. You run your training script inside this job and change it few times until you find the cause of the problem and fix it. Setting `max_run` parameter of the estimator is highly recommended for the placeholder job, to avoid unnecessary charges.
-3. You submit a third job with your fixed training script `train.py` to make sure it works now.
+  a. You submit a first job with your training script `train.py`, and it fails for some reason that you want to troubleshoot.
+  
+  b. You submit a second job with the placeholder script `train_placeholder.py`. You run your training script inside this job and change it few times until you find the cause of the problem and fix it. Setting `max_run` parameter of the estimator is highly recommended for the placeholder job, to avoid unnecessary charges.
+
+  c. You submit a third job with your fixed training script `train.py` to make sure it works now.
 
 The dummy script may look like this:
 
 ```python
 import time
 from datetime import timedelta
 
@@ -597,198 +639,222 @@
 
 while not is_last_session_timeout(timedelta(minutes=30)):
     time.sleep(10)
 ```
 
 The method `is_last_session_timeout()` will help to prevent unused resources and the job will end if there's no SSM or SSH sessions for the specified period of time. It will count active SSM sessions, and time out when there are no sessions left. 
 
-*Note:* Keep in mind that SSM sessions will [terminate automatically due to user inactivity](https://docs.aws.amazon.com/systems-manager/latest/userguide/session-preferences-timeout.html), but SSH sessions will keep running until either a user terminates them manually or network timeout occurs (e.g., the user closes the laptop lid or disconnects from Wi-Fi). If the user leaves the local machine unattended and connected to Internet, SSM sessions started by `aws ssm start-session` command will time out, but SSH-over-SSM sessions started with `sm-local-ssh-training connect` will stay open.
+**Caution:** Keep in mind that SSM sessions will [terminate automatically due to user inactivity](https://docs.aws.amazon.com/systems-manager/latest/userguide/session-preferences-timeout.html), but SSH sessions will keep running until either a user terminates them manually or network timeout occurs, i.e., the user closes the laptop lid, disconnects from Wi-Fi, etc. If the user leaves the local machine unattended and connected to Internet, SSM sessions started by `aws ssm start-session` command will time out, but SSH-over-SSM sessions started with `sm-ssh connect` will stay open. Consider sending e-mail notifications for users of the long-running jobs, so the users don't forget to shut down unused resources. See [the related question in FAQ](FAQ.md#i-want-to-send-users-the-sms-or-email-notification-when-the-placeholder-training-job-has-issues-with-low-gpu-utilization-how-to-do-that) for more details and [train_placeholder.py](https://github.com/aws-samples/sagemaker-ssh-helper/blob/v2.1.0/tests/source_dir/training_placeholder/train_placeholder.py) that implements the similar logic.
 
-Consider sending e-mail notifications for users of the long-running jobs, so the users don't forget to shut down unused resources. See [the related question in FAQ](FAQ.md#i-want-to-send-users-the-sms-or-email-notification-when-the-placeholder-training-job-has-issues-with-low-gpu-utilization-how-to-do-that) for more details.
+*Pro Tip:* Make sure that you're aware of [SageMaker Managed Warm Pools](https://docs.aws.amazon.com/sagemaker/latest/dg/train-warm-pools.html) 
+feature, which is also helpful in the scenario when you need to rerun your code remotely multiple times.
 
-Make also sure that you're aware of [SageMaker Managed Warm Pools](https://docs.aws.amazon.com/sagemaker/latest/dg/train-warm-pools.html) 
-feature, which is also helpful in the scenario when you need to rerun your code multiple times.
+*Pro Tip:* You can debug your code line by line in this scenario. See [the tutorial in PyCharm documentation](https://www.jetbrains.com/help/pycharm/debugging-your-first-python-application.html#debug).
 
-*Pro Tip:* Note that you can debug your code line by line in this scenario, too! See [the tutorial in PyCharm documentation](https://www.jetbrains.com/help/pycharm/debugging-your-first-python-application.html#debug). Some users might prefer this option instead of using Debug Server as a simpler alternative.
+5. Run and debug your code
 
-It is also interesting to compare this section instructions with the AWS blog post [Run your TensorFlow job on Amazon SageMaker with a PyCharm IDE](https://aws.amazon.com/blogs/machine-learning/run-your-tensorflow-job-on-amazon-sagemaker-with-a-pycharm-ide/). In contrast to using SageMaker SSH Helper, the blog instructions do not demonstrate the remote debugging capabilities, but suggest to use the [SageMaker local mode](https://github.com/aws-samples/amazon-sagemaker-local-mode) instead. As with Managed Warm Pools, SageMaker local mode helps to test your code faster, but it consumes local resources and still doesn't provide the line by line debugging capability.
+Now when you have your training script or a placeholder script running, you can run additional code on the remote host, debug it line by line and set breakpoints.
 
-## <a name="studio"></a>Local IDE integration with SageMaker Studio over SSH for PyCharm / VSCode
+If you want to change the control flow and let your training script call back the IDE for debugging, follow the next section on configuring the Debug Server.
 
-[![Download Demo (.mov)](https://user-images.githubusercontent.com/87804596/205895890-e5e87f8b-1ca6-4ce6-bac1-5cb6e6f61dde.png)](https://aws-blogs-artifacts-public.s3.amazonaws.com/artifacts/ML-4988/SSH_Helper-Remote-IDE.mov)
-[Download Demo (.mov)](https://aws-blogs-artifacts-public.s3.amazonaws.com/artifacts/ML-4988/SSH_Helper-Remote-IDE.mov)
+*Pro Tip*: The curious reader should also read the AWS blog post [Run your TensorFlow job on Amazon SageMaker with a PyCharm IDE](https://aws.amazon.com/blogs/machine-learning/run-your-tensorflow-job-on-amazon-sagemaker-with-a-pycharm-ide/). In contrast to the scenario with SageMaker SSH Helper, the blog instructions show how to use [SageMaker local mode](https://github.com/aws-samples/amazon-sagemaker-local-mode). As with Managed Warm Pools, SageMaker local mode helps to test your code faster, but it consumes local resources and doesn't provide the line by line debugging capability (as of writing).
 
-Follow the next steps for your local IDE integration with SageMaker Studio.
 
-1. On the local machine, install the library: 
+## <a name="pycharm-debug-server"></a>Remote debugging with PyCharm Debug Server over SSH
 
-```
-pip install sagemaker-ssh-helper
-```
+There's another way to debug your code that is specific to the PyCharm Professional feature: [Remote debugging with the Python remote debug server configuration](https://www.jetbrains.com/help/pycharm/remote-debugging-with-product.html#remote-debug-config). The procedure assumes that you're running a training job, but the same steps apply to inference or data processing, too.
 
-2. Copy [SageMaker_SSH_IDE.ipynb](SageMaker_SSH_IDE.ipynb) into SageMaker Studio and run it. 
+1. In PyCharm, go to the Run/Debug Configurations (Run -> Edit Configurations...), add a new Python Debug Server.
+Choose the fixed port, e. g. `12345`.
 
-*Tip:* Alternatively, instead of using `SageMaker_SSH_IDE.ipynb`, [attach](https://docs.aws.amazon.com/sagemaker/latest/dg/studio-lcc-create.html) to a domain the KernelGateway lifecycle config script [kernel-lc-config.sh](kernel-lc-config.sh) 
-(you may need to ask your administrator to do this).
-Once configured, from the Launcher choose the environment, puck up the lifecycle script and choose 
-'Open image terminal' (so, you don't even need to create a notebook).
+2. Take the correct version of `pydevd-pycharm` package from the configuration window 
+and install it either through `requirements.txt` or by calling `pip` from your source code.
 
-> Note that the `main` branch of this repo can contain changes that are not compatible with the version of `sagemaker-ssh-helper` that you installed from pip. To ensure the stable performance, check the version with `pip freeze | grep sagemaker-ssh-helper` and take the notebook and the lifecycle script from [the corresponding tag](https://github.com/aws-samples/sagemaker-ssh-helper/tags).  
+3. Add commands to connect to the Debug Server to your code **after** the `setup_and_start_ssh()`, e.g., into [a training script](https://github.com/aws-samples/sagemaker-ssh-helper/blob/main/tests/source_dir/training_debug/train_debug.py) that you submit as an entry point for a training job:
+```python
+import sagemaker_ssh_helper
+sagemaker_ssh_helper.setup_and_start_ssh()
 
-3. Make sure that you installed the latest [AWS CLI v2](https://docs.aws.amazon.com/cli/latest/userguide/getting-started-install.html) and the [AWS Session Manager CLI plugin](https://docs.aws.amazon.com/systems-manager/latest/userguide/session-manager-working-with-install-plugin.html). Run the following command to perform the installation:
+...
 
-```shell
-sm-local-configure
+import pydevd_pycharm
+pydevd_pycharm.settrace('localhost', port=12345, stdoutToServer=True, stderrToServer=True, suspend=True)
 ```
+*Tip*: Check the `settrace()` argument's description in [the library source code](https://github.com/JetBrains/intellij-community/blob/dee787ef05d1187a71b7667652f6b25f3f573a1b/python/helpers/pydev/pydevd.py#L1663).
 
-4. Set your SageMaker Studio domain ID and user profile name:
+4. Set breakpoints in your code with PyCharm, as needed
 
-```bash
-sm-local-ssh-ide set-domain-id <<domain_id>>
-sm-local-ssh-ide set-user-profile-name <<user_profile_name>>
-```
+5. Start the Debug Server in PyCharm
 
-Since SageMaker Studio app names are not unique across domains and user profiles, it will help to find the correct instance in a multi-user environment.
+6. Submit your code to SageMaker with SSH Helper as described in previous sections.
 
-For your convenience, the domain ID and the user profile name are printed by the `sm-ssh-ide get-metadata` command when you run the notebook (check the cell output).
-
-4. Start SSH tunnel and port forwarding from a terminal session as follows:
+7. On your local machine, once the SSH helper connects to SSM and starts waiting inside the training job, connect to the host with SSH and start the port forwarding for the Debug Server:
 
 ```shell
-sm-local-ssh-ide connect <<kernel_gateway_app_name>>
+ssh -R localhost:12345:localhost:12345 \
+  root@ssh-training-example-2023-07-25-03-18-04-490.training.sagemaker
 ```
+It will reverse-forward the remote debugger port `12345` to your local machine's Debug Server port.
 
-The parameter <<kernel_gateway_app_name>> is either taken from SageMaker Studio when you run notebook [SageMaker_SSH_IDE.ipynb](SageMaker_SSH_IDE.ipynb), 
-or from the image terminal as a `hostname` output, or you can find it in the list of running apps in AWS Console under Amazon SageMaker -> Control Panel -> User Details.
-It looks like this: `sagemaker-data-science-ml-m5-large-1234567890abcdef0`.
+8. Stop the waiting loop
 
-For your convenience, the app name is printed by the `sm-ssh-ide get-metadata` command when you run the notebook (check the cell output).
+As already mentioned, make sure you've configured `connection_wait_time_seconds` to give yourself time to start the port forwarding before execution of the training script continues, and before it tries to connect to the debug server at port `12345`.
 
-The local port `10022` will be connected to the remote SSH server port, to let you connect with SSH from IDE.  
-In addition, the local port `8889` will be connected to remote Jupyter notebook port, the port `5901` to the remote VNC server 
-and optionally the remote port `443` will be connected to your local PyCharm license server address.
+Inside the SSH session, run:
+```text
+sm-wait stop
+```
 
-> *Note:* Before running this command make sure that AWS CLI is configured to access the account with `aws s3 ls` and your default region is set with `aws configure` command. Your Python's `<path-to-venv>/bin/` directory should be in the `$PATH`, otherwise you will get a *"command not found"* error.
+9. After you stop the waiting loop, your code will continue running and will connect to your PyCharm Debug Server.
 
-Feel free to use the script as a template. Clone and customize it, if you want to change the ports and hosts.
+If everything is set up correctly, PyCharm will stop at your breakpoint, highlight the line and wait for your input. Debug Server window will say “connected”. You can now press, for example, F8 to "Step Over" the code line or F7 to "Step Into" the code line.
 
 
-5. Add the following configuration to `~/.ssh/config`:
+## <a name="studio"></a>Local IDE integration with SageMaker Studio over SSH for PyCharm / VSCode
 
-```text
-Host sagemaker-studio
-  HostName localhost
-  IdentityFile ~/.ssh/sagemaker-ssh-gw
-  Port 10022
-  User root
-```
+[![Download Demo (.mov)](https://user-images.githubusercontent.com/87804596/205895890-e5e87f8b-1ca6-4ce6-bac1-5cb6e6f61dde.png)](https://aws-blogs-artifacts-public.s3.amazonaws.com/artifacts/ML-4988/SSH_Helper-Remote-IDE.mov)
+[Download Demo (.mov)](https://aws-blogs-artifacts-public.s3.amazonaws.com/artifacts/ML-4988/SSH_Helper-Remote-IDE.mov)
 
-*Note:* The SSH key specified as `IdentityFile` is automatically generated on your local machine every time when you run `sm-local-ssh-ide` command from the step 4.
+> **Note**: This demo is recorded with a previous version of SSH Helper and may be not up-to-date with the recent features. Check the documentation for the most up-to-date steps.
 
-Before moving to the next step, you can optionally check from your local machine that connection is working by running the SSH command in command line:
+For your local IDE integration with SageMaker Studio, follow the same steps as for configuring the IDE for [Remote code execution](#remote-interpreter), but instead of submitting the training / processing / inference code to SageMaker with Python SDK, execute the Jupyter notebook, as described in the next steps.
 
-```shell
-ssh sagemaker-studio
-```
+1. Copy [SageMaker_SSH_IDE.ipynb](SageMaker_SSH_IDE.ipynb) into SageMaker Studio and run it. 
 
+Alternatively, [attach](https://docs.aws.amazon.com/sagemaker/latest/dg/studio-lcc-create.html) to a domain the KernelGateway lifecycle config script [kernel-lc-config.sh](kernel-lc-config.sh) 
+(you may need to ask your administrator to do this).
+Once configured, from the Launcher choose the environment, pick up the lifecycle script and choose 
+'Open image terminal' (so, you don't even need to create a notebook).
 
-6. Connect local PyCharm or VSCode with remote Python interpreter by using `sagemaker-studio` as the remote SSH host.
+> Note that the `main` branch of this repo can contain changes that are not compatible with the version of `sagemaker-ssh-helper` that you installed from pip. To ensure the stable performance, check the version with `pip freeze | grep sagemaker-ssh-helper` and take the notebook and the lifecycle script from [the corresponding tag](https://github.com/aws-samples/sagemaker-ssh-helper/tags).  
 
- * [Instructions for SSH in PyCharm](https://www.jetbrains.com/help/pycharm/remote-debugging-with-product.html#remote-interpreter)
+2. Configure remote interpreter in PyCharm / VS Code to connect to SageMaker Studio
 
-In PyCharm, use `11022` as the port and `root` as the user.
+Use `app_name.user_profile_name.domain_id.studio.sagemaker` or `app_name.studio.sagemaker` as the `fqdn` to connect.
 
-![](images/pycharm_studio.png)
+To see available apps to connect to, you may run the `list` command:
 
- * [Instructions for SSH in VSCode](https://code.visualstudio.com/docs/remote/ssh)
+```
+sm-ssh list studio.sagemaker
+```
 
-![](images/vscode_studio.png)
+3. Using the remote Jupyter Notebook
 
-*Tip (PyCharm):* When you configure Python interpreter in PyCharm, it's recommended to configure [the path mapping](https://www.jetbrains.com/help/pycharm/deployment-mappings-tab.htm) (*"Sync folders"* deployment option) for you project to point into `/root/project_name` instead of default `/tmp/pycharm_project_123`. This is how you will be able to see your project in SageMaker Studio and PyCharm will automatically sync your local dir to the remote dir. 
+In recent versions of PyCharm, Jupyter Notebook is tunnelled automatically through remote interpreter connection. You might need to add `--allow-root` argument to the command line, when your remote interpreter runs under root:
 
-*Tip (PyCharm):* Also instead of creating a new venv, point the Python interpreter to the existing location. 
-You can find this location by running a cell with `import sys; sys.executable` command in a SageMaker Studio notebook. You will get something like `/opt/conda/bin/python`.
+![](images/remote_jupyter.png)
 
-Now with PyCharm or VSCode you can run and debug the code remotely inside the kernel gateway app.
+If you wish to connect to the existing notebook server started by SSH Helper or don't use PyCharm, proceed with the next configuration steps.
+
+To make the remote Jupyter Server port `8889` forwarded to the local machine, use SSH:
+
+```shell
+ssh -L localhost:8889:localhost:8889 \
+  root@ssh-ds2.jane-doe.d-egm0dexample.studio.sagemaker
+```
 
-You can also configure a remote Jupyter Server as 
+Now you can also connect to a remote Jupyter Server started by SSH Helper inside SageMaker Studio as 
 http://127.0.0.1:8889/?token=<<your_token>>.
 
-You will find the full URL with remote token in 
-the [SageMaker_SSH_IDE.ipynb](SageMaker_SSH_IDE.ipynb) notebook in the output after running the cell
-with `sm-ssh-ide start` command. If you use lifecycle configuration, run `tail /tmp/jupyter-notebook.log` from the image terminal to find the Jupyter Server URL.
+You will find the full URL with remote token in the [SageMaker_SSH_IDE.ipynb](SageMaker_SSH_IDE.ipynb) notebook in the output after running the cell  with `sm-ssh-ide start` command. If you use lifecycle configuration, run `tail /tmp/jupyter-notebook.log` from the image terminal to find the Jupyter Server URL.
 
  * [Instructions for remote Jupyter notebooks in PyCharm](https://www.jetbrains.com/help/pycharm/configuring-jupyter-notebook.html#configure-server)
  * [Instructions for remote Jupyter notebooks in VSCode](https://code.visualstudio.com/docs/datascience/jupyter-notebooks#_connect-to-a-remote-jupyter-server) (don't forget to switch kernel to remote after configuring the remote server).
 
-You can also start the VNC session to [vnc://localhost:5901](vnc://localhost:5901) (e.g. on macOS with Screen Sharing app)
-and run IDE or any other GUI app on the remote desktop instead of your local machine. For example, you can run `jupyter qtconsole --existing` command to connect to already running SageMaker Studio kernel with the [Jupyter QT app](https://qtconsole.readthedocs.io/en/stable/index.html), instead of using the notebook web UI.
+4. Connecting to VNC
 
-7. If you want to switch to another [kernel](https://docs.aws.amazon.com/sagemaker/latest/dg/notebooks-run-and-manage-change-image.html) 
+To make the remote VNC port `5901` forwarded to the local machine, use SSH:
+
+```shell
+ssh -L localhost:5901:localhost:5901 \
+  -R localhost:443:jetbrains-license-server.example.com:443 \
+  root@ssh-ds2.jane-doe.d-egm0dexample.studio.sagemaker
+```
+
+*Note (PyCharm)*: The optional `-R` option will connect the remote port `443` to your local PyCharm license server address. Replace `jetbrains-license-server.example.com` with your server name and edit your `/etc/hosts` inside VNC to make this host point to `127.0.0.1` (should be done automatically if you didn't skip the `sm-ssh-ide set-jb-license-server` in the notebook).
+
+Now you can start the VNC session to [vnc://localhost:5901](vnc://localhost:5901) (e.g. on macOS with Screen Sharing app) and run IDE or any other GUI app on the remote desktop instead of your local machine. 
+
+For example, you can run inside VNC the `jupyter qtconsole` command to start the [Jupyter QT app](https://qtconsole.readthedocs.io/en/stable/index.html) as the alternative to Jupyter web UI:
+
+![Jupyter QT in VNC](images/vnc_jupyter.png)
+
+6. If you want to switch to another [kernel](https://docs.aws.amazon.com/sagemaker/latest/dg/notebooks-run-and-manage-change-image.html) 
 or [instance](https://docs.aws.amazon.com/sagemaker/latest/dg/notebooks-run-and-manage-switch-instance-type.html), feel free to do so from SageMaker Studio UI and re-run
 [SageMaker_SSH_IDE.ipynb](SageMaker_SSH_IDE.ipynb).
 
-Keep in mind that in this case the previous kernel will stop and SSM agent will stop, too.
-To allow multiple kernel and instances to be up and running with SageMaker SSH Helper and SSM agent,
+Keep in mind that in this case the previous kernel will stop and SSM Agent will stop, too.
+To allow multiple kernel and instances to be up and running with SageMaker SSH Helper and SSM Agent,
 duplicate the notebook and give it a different name, e.g. `SageMaker_SSH_IDE-PyTorch.ipynb`.
-In this case you'll be able to keep two environments in parallel. To switch between them,
-you will only need to re-run `sm-local-ssh-ide` command on your local machine.
+In this case you'll be able to keep two environments in parallel. 
 
-If you're using lifecycle configuration script, just start another image terminal with different environment settings 
-from Launcher.
+If you're using lifecycle configuration script, just start another image terminal with different environment settings from Launcher.
 
-8. Don't forget to [shut down](https://docs.aws.amazon.com/sagemaker/latest/dg/notebooks-run-and-manage-shut-down.html)
-SageMaker Studio resources, if you don't need them anymore, e.g., launched notebooks, terminals, apps and instances.
-
-See the [troubleshooting section of the FAQ](FAQ.md#troubleshooting), if something doesn't work as you expect.
+7. Don't forget to [shut down](https://docs.aws.amazon.com/sagemaker/latest/dg/notebooks-run-and-manage-shut-down.html) SageMaker Studio resources, if you don't need them anymore, e.g., launched notebooks, terminals, apps and instances.
 
 ## <a name="web-vnc"></a>Web VNC
 
-At times, you cannot install all the software on your local machine, also because this is the software to process the data, and you cannot copy massive amount of the data to your local machine. 
+At times, you cannot install all the software on your local machine, also because this is the software processes data, and you cannot copy massive amount of the data to your local machine. 
+
+You might have thought about [AWS Jupyter Proxy](https://github.com/aws/aws-jupyter-proxy), but some web apps like Dask may not fully work through the proxy, so VNC is the recommended alternative.
 
-By combining the [noVNC](https://novnc.com/) tool with [AWS Jupyter Proxy](https://github.com/aws/aws-jupyter-proxy) extension you can run virtually any IDE like PyCharm, VSCode, PyDev, or any tool like Blender (to work with 3D data), OpenShot (to work with audio-video data), etc., from a SageMaker Studio web interface.
+By combining the [noVNC](https://novnc.com/) tool with AWS Jupyter Proxy extension you can run virtually any IDE like PyCharm, VSCode, PyDev, or any tool like Blender (to work with 3D data), OpenShot (to work with audio-video data), etc., as well as other webapps from a SageMaker Studio web UI, without installing all of them to your local machine.
 
 It's also helpful in situations when you cannot run SSH client on your local machine to forward ports for web tools, like Dask dashboard. In this case, you run a tool in the remote browser running through the web VNC (browser-in-a-browser), like on the below screenshot. You might notice that PyCharm and VSCode are also running in the background:
 ![WebWNC Screenshot](images/webVNC.png)
 
-To achieve this result, your Administrator should configure your SageMaker IAM role with both `SSHSageMakerServerPolicy` and `SSHSageMakerClientPolicy`. Configuration of IAM credentials for the local machine is not required in this case. See [IAM_SSM_Setup.md](IAM_SSM_Setup.md) for more details.
+To achieve this result, your Administrator should configure your SageMaker IAM role with both `SSHSageMakerServerPolicy` and `SSHSageMakerClientPolicy`. Configuration of IAM credentials for the local machine is not required in this case. See the Step 4 in [IAM_SSM_Setup.md](IAM_SSM_Setup.md#4-optional-connecting-from-sagemaker-studio-) for more details.
 
 Then follow these steps:
 
 1. On the SageMaker Studio System terminal run the commands from [server-lc-config.sh](server-lc-config.sh).
 
 Alternatively, ask the Administrator to [attach the lifecycle config](https://docs.aws.amazon.com/sagemaker/latest/dg/studio-lcc-create.html) to the SageMaker Studio domain or to your profile as the default `JupyterServer` config, e.g., with the name `sagemaker-ssh-helper-webvnc`.
 
 2. Follow the step 1 for [the IDE configuration procedure](#studio), i.e., run the IDE notebook or lifecycle config inside the kernel gateway of your choice. 
 
 Instead of your local user ID put the SageMaker Studio user ID (you can get it by running `aws sts get-caller-identity` from a SageMaker Studio terminal).
 
-3. On the System terminal, run:
+3. On the System (!) terminal (not image terminal), run:
 
 ```shell
-sm-local-ssh-ide connect <<kernel_gateway_app_name>>
+sm-ssh connect app_name.user_profile_name.domain_id.studio.sagemaker
 ```
 
-Add additional params to the command, e.g., `-L localhost:8787:localhost:8787` to forward the Dask dashboard that is running inside the kernel gateway (note, that Dask web app may not work properly through Jupyter Proxy, so VNC is the recommended alternative).
+Alternatively, use SSH command to forward the VNC port and add more ports to the command, e.g., `-L localhost:8787:localhost:8787` to forward the Dask dashboard that is running inside the kernel gateway:
+
+```shell
+ssh -L localhost:5901:localhost:5901 \
+  -L localhost:8787:localhost:8787 \
+  app_name.user_profile_name.domain_id.studio.sagemaker
+```
 
 4. Navigate to `https://d-egm0dexample.studio.eu-west-1.sagemaker.aws/jupyter/default/proxy/6080/vnc.html?host=d-egm0dexample.studio.eu-west-1.sagemaker.aws&port=443&path=jupyter/default/proxy/6080/websockify`
 
 Replace both occurrences of `d-egm0dexample` with your SageMaker Studio domain ID, and `eu-west-1` with your AWS Region.
 
 You will see the noVNC welcome screen.
 
 5. Press "Connect" and enter your password (default is `123456`).
 
 Congratulations! You now have successfully logged into the remote desktop environment running inside a SageMaker Studio kernel gateway.
 
+Some data handling application to try inside the VNC desktop, which you cannot run as a web app otherwise, are:
+* [3D Slicer](https://www.slicer.org/) - image computing platform for medical, biomedical, and other 3D images and meshes 
+* [OpenShot](https://www.openshot.org/) - to work with video data
+* [LibreOffice](https://www.libreoffice.org/) - work with documents and spreadsheets
+
 *Tip:* If you have issues with copy-pasting through system clipboard, use the temp file, e.g. `clip.txt`, and open it in VNC session and SageMaker Studio file browser at the same time.
 
 *Pro Tip:* To set the resolution that matches your browser window size, make a page screenshot (in Firefox - right-click on an empty area -> Take Screenshot -> Save visible), then inspect the resolution of the image, e.g. 1920x970. Then add and switch resolution inside the VNC session:
 ```shell
 $ cvt 1920 970 60
 # 1920x970 59.93 Hz (CVT) hsync: 60.35 kHz; pclk: 154.50 MHz
 Modeline "1920x970_60.00"  154.50  1920 2040 2240 2560  970 973 983 1007 -hsync +vsync
 $ xrandr --newmode "1920x970_60.00"  154.50  1920 2040 2240 2560  970 973 983 1007 -hsync +vsync
 $ xrandr --addmode VNC-0 1920x970_60.00
 $ xrandr -s 1920x970_60.00
 ```
 
+## Troubleshooting
+
+If something doesn't work as expected, make sure you looked at our [FAQ](FAQ.md), especially at the [troubleshooting section](FAQ.md#troubleshooting), as well as at the existing both open and resolved [issues](https://github.com/aws-samples/sagemaker-ssh-helper/issues?q=is%3Aissue).
```

### Comparing `sagemaker-ssh-helper-2.1.0/sagemaker_ssh_helper/__init__.py` & `sagemaker_ssh_helper-2.2.0/sagemaker_ssh_helper/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import subprocess
 import os
+import time
 from datetime import datetime, timedelta
 
 import sagemaker_ssh_helper.env
 
 sagemaker_ssh_helper.last_session_time = datetime.now()
 
 
@@ -18,18 +19,29 @@
 
     print(f"[sagemaker-ssh-helper] SageMaker SSH Helper startup params: start_ssh={start_ssh}, "
           f"ssh_instance_count={ssh_instance_count}, node_rank={node_rank}")
 
     script = sagemaker_ssh_helper.env.get_caller_script_name(2)
     if start_ssh == "true" and node_rank < ssh_instance_count:
         print(f"[sagemaker-ssh-helper] Starting SSH Helper setup from {script}")
+        start_time = datetime.now()
         sm_setup_ssh_absolute_path = os.path.join(os.path.dirname(os.path.abspath(__file__)), "sm-setup-ssh")
-        subprocess.check_call(["bash", sm_setup_ssh_absolute_path])  # nosec B607  # absolute path is calculated
+        setup_successful = False
+        try:
+            subprocess.check_call(["bash", sm_setup_ssh_absolute_path])  # nosec B607  # absolute path is calculated
+            setup_successful = True
+        finally:
+            if not setup_successful:
+                # give time for all logs and errors to apper in CloudWatch to avoid throttling
+                time.sleep(60)
+            print(f"[sagemaker-ssh-helper] SSH Helper setup is "
+                  f"{'SUCCESSFUL' if setup_successful else 'FAILED with errors'}. "
+                  f"Elapsed time: {str(datetime.now() - start_time)}")
     else:
-        print(f"[sagemaker-ssh-helper] Skipping SageMaker SSH Helper setup from {script}")
+        print(f"[sagemaker-ssh-helper] Skipping SageMaker SSH Helper setup from {script} due to startup params")
 
 
 def is_last_session_timeout(time_delta: timedelta):
     args = ["pgrep", "-f", "ssm-session-worker"]
     try:
         out = subprocess.check_output(args)
         worker_pids = list(map(int, out.splitlines()))
```

### Comparing `sagemaker-ssh-helper-2.1.0/sagemaker_ssh_helper/aws.py` & `sagemaker_ssh_helper-2.2.0/sagemaker_ssh_helper/aws.py`

 * *Files identical despite different names*

### Comparing `sagemaker-ssh-helper-2.1.0/sagemaker_ssh_helper/cdk/iam_ssm/iam_ssm_stack.py` & `sagemaker_ssh_helper-2.2.0/sagemaker_ssh_helper/cdk/iam_ssm/iam_ssm_stack.py`

 * *Files identical despite different names*

### Comparing `sagemaker-ssh-helper-2.1.0/sagemaker_ssh_helper/cdk/iam_ssm/iam_ssm_stack_tests.py` & `sagemaker_ssh_helper-2.2.0/sagemaker_ssh_helper/cdk/iam_ssm/iam_ssm_stack_tests.py`

 * *Files 4% similar despite different names*

```diff
@@ -73,37 +73,43 @@
                                       "sagemaker:CreateProcessingJob",
                                       "sagemaker:CreateModel",
                                       "sagemaker:CreateEndpointConfig",
                                       "sagemaker:CreateEndpoint",
                                       "sagemaker:CreateTransformJob",
                                       "sagemaker:CreateHyperParameterTuningJob",
                                       "sagemaker:DescribeTrainingJob",
+                                      "sagemaker:ListTrainingJobs",
                                       "sagemaker:DescribeProcessingJob",
+                                      "sagemaker:ListProcessingJobs",
                                       "sagemaker:DescribeModel",
                                       "sagemaker:DescribeEndpointConfig",
                                       "sagemaker:DescribeEndpoint",
+                                      "sagemaker:ListEndpoints",
                                       "sagemaker:DescribeTransformJob",
+                                      "sagemaker:ListTransformJobs",
                                       "sagemaker:DescribeHyperParameterTuningJob",
                                       "sagemaker:ListTrainingJobsForHyperParameterTuningJob",
                                       "sagemaker:DeleteEndpointConfig",
                                       "sagemaker:DeleteEndpoint",
                                       "sagemaker:InvokeEndpoint",
                                       "sagemaker:StopTrainingJob",
                                       "sagemaker:CreateApp",
                                       "sagemaker:DeleteApp",
                                       "sagemaker:DescribeApp",
+                                      "sagemaker:ListApps",
                                       "sagemaker:CreateImage",
                                       "sagemaker:DescribeImage",
                                       "sagemaker:DeleteImage",
                                       "sagemaker:CreateImageVersion",
                                       "sagemaker:DescribeImageVersion",
                                       "sagemaker:CreateAppImageConfig",
                                       "sagemaker:DeleteAppImageConfig",
                                       "sagemaker:UpdateDomain",
                                       "sagemaker:CreatePresignedDomainUrl",
+                                      "sagemaker:ListNotebookInstances",
                                   ],
                                   resources=["*"]
                               ),
                               PolicyStatement(
                                   effect=Effect.ALLOW,
                                   actions=[
                                       "codebuild:CreateProject",
@@ -158,14 +164,19 @@
                                       "logs:PutLogEvents",
                                   ],
                                   resources=[
                                       f"arn:{Aws.PARTITION}:logs:{Aws.REGION}:{Aws.ACCOUNT_ID}:log-group:/aws/codebuild/sagemaker-studio-image-build-*:log-stream:*"]
                               ),
                               PolicyStatement(
                                   effect=Effect.ALLOW,
+                                  actions=["sns:Publish"],
+                                  resources=["*"]
+                              ),
+                              PolicyStatement(
+                                  effect=Effect.ALLOW,
                                   actions=[
                                       "ssm:DeregisterManagedInstance",
                                   ],
                                   resources=[f"arn:{Aws.PARTITION}:ssm:*:{Aws.ACCOUNT_ID}:managed-instance/mi-*"],
                                   conditions={
                                       "StringLike": {
                                           "ssm:resourceTag/SSHOwner": "*"
```

### Comparing `sagemaker-ssh-helper-2.1.0/sagemaker_ssh_helper/cdk/iam_ssm/ssm_advanced_tier_stack.py` & `sagemaker_ssh_helper-2.2.0/sagemaker_ssh_helper/cdk/iam_ssm/ssm_advanced_tier_stack.py`

 * *Files identical despite different names*

### Comparing `sagemaker-ssh-helper-2.1.0/sagemaker_ssh_helper/cdk/iam_ssm/trust_relationship_lambda.py` & `sagemaker_ssh_helper-2.2.0/sagemaker_ssh_helper/cdk/iam_ssm/trust_relationship_lambda.py`

 * *Files identical despite different names*

### Comparing `sagemaker-ssh-helper-2.1.0/sagemaker_ssh_helper/cdk/low_gpu/low_gpu_lambda.py` & `sagemaker_ssh_helper-2.2.0/sagemaker_ssh_helper/cdk/low_gpu/low_gpu_lambda.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 import boto3
 
 from sagemaker_ssh_helper.wrapper import SSHEstimatorWrapper, SSHProcessorWrapper
 
 
 def handler(event, context):
     if len(logging.getLogger().handlers) > 0:
-        logging.getLogger().setLevel(logging.INFO)
+        logging.getLogger().setLevel(logging.DEBUG)
     else:
-        logging.basicConfig(level=logging.INFO)
+        logging.basicConfig(level=logging.DEBUG)
 
     # See: https://docs.aws.amazon.com/sagemaker/latest/dg/automating-sagemaker-with-eventbridge.html
     logging.info(f"Got event: {event}")
     # See: https://docs.aws.amazon.com/lambda/latest/dg/python-context.html
     logging.info(f"Event context: {context}")
 
     sns_notification_topic_arn = os.environ.get("SNS_NOTIFICATION_TOPIC_ARN", None)
@@ -22,45 +22,59 @@
 
     event_detail_type = 'SageMaker Processing Job State Change'
     if event['detail-type'] != event_detail_type:
         raise ValueError(f"This lambda should be triggered by an EventBridge event '{event_detail_type}'")
 
     processing_job_name = event['detail']['ProcessingJobName']
     ssh_processing_wrapper = SSHProcessorWrapper.attach(processing_job_name)
-    logging.info(f"Triggered by processing job {processing_job_name}. "
+    logging.info(f"Triggered by processing job: {processing_job_name}. "
                  f"Metadata: {ssh_processing_wrapper.get_metadata_url()} . "
                  f"Logs: {ssh_processing_wrapper.get_cloudwatch_url()} .")
 
+    image_uri = event['detail']['AppSpecification']['ImageUri']
+    job_status = event['detail']['ProcessingJobStatus']
+    exit_message = event['detail']['ExitMessage']
+    rule_to_invoke = event['detail']['Environment']['rule_to_invoke']
+
+    if '/sagemaker-debugger-rules:latest' not in image_uri:
+        logging.info("Not a SageMaker Debugger processing job")
+        return {'statusCode': 200, 'body': 'Not a debugger job.'}
+
+    if rule_to_invoke != 'LowGPUUtilization':
+        logging.info("Not a LowGPUUtilization profiler rule")
+        return {'statusCode': 200, 'body': 'Not a lowGPUUtilization profiler rule.'}
+
+    if job_status != 'Completed':
+        logging.info("Profiler job hasn't been completed yet. Skipping check.")
+        return {'statusCode': 200, 'body': 'Job is not yet completed.'}
+
     training_job_arn = event['detail']['TrainingJobArn']
     ssh_training_wrapper: SSHEstimatorWrapper = SSHEstimatorWrapper.attach_arn(training_job_arn)
-    logging.info(f"Inspecting training job {training_job_arn}. "
+    logging.info(f"Training job ARN: {training_job_arn}. "
                  f"Metadata: {ssh_training_wrapper.get_metadata_url()} . "
                  f"Logs: {ssh_training_wrapper.get_cloudwatch_url()} .")
 
-    status_details = ''
-    rule_configs_summary = ssh_training_wrapper.rule_job_summary()
-    for rule_config in rule_configs_summary:
-        if rule_config['RuleConfigurationName'] == 'LowGPUUtilization':
-            if rule_config['RuleEvaluationStatus'] == 'IssuesFound':
-                status_details = rule_config['StatusDetails']
-                logging.warning(f"Found issues with GPU utilization of the training job "
-                                f"{ssh_training_wrapper.training_job_name()}: {status_details}")
-
-                logging.info(f"Send notification email and/or SMS through Amazon SNS topic {sns_notification_topic_arn}")
-                sns_resource = boto3.resource('sns')
-                sns_notification_topic = sns_resource.Topic(sns_notification_topic_arn)
-                response = sns_notification_topic.publish(
-                    Subject='Training job with low GPU utilization',
-                    Message=status_details + "\n\n" +
-                            "Training job metadata URL:\n" +
-                            ssh_training_wrapper.get_metadata_url()
-                )
-                logging.info(f"SNS response: {response}")
-
-                # Optionally, stop the job (not recommended, better to keep notifications only)
-                # ssh_training_wrapper.stop_training_job()
-
-    if status_details == '':
+    if 'RuleEvaluationConditionMet' not in exit_message:
         logging.info(f"No issues found with GPU utilization of training job "
                      f"{ssh_training_wrapper.training_job_name()}")
+        return {'statusCode': 200, 'body': 'No issues.'}
+
+    logging.warning(f"Found issues with GPU utilization of the training job "
+                    f"{ssh_training_wrapper.training_job_name()}: {exit_message}")
+
+    logging.info(f"Send notification email and/or SMS through Amazon SNS topic {sns_notification_topic_arn}")
+    sns_resource = boto3.resource('sns')
+    logging.debug("Boto3 resource created.")
+    sns_notification_topic = sns_resource.Topic(sns_notification_topic_arn)
+    logging.debug("SNS topic created.")
+    response = sns_notification_topic.publish(
+        Subject='Training job with low GPU utilization',
+        Message=exit_message + "\n\n" +
+                "Training job metadata URL:\n" +
+                ssh_training_wrapper.get_metadata_url()
+    )
+    logging.info(f"SNS response: {response}")
+
+    # Optionally, stop the job (not recommended, better to keep notifications only)
+    # ssh_training_wrapper.stop_training_job()
 
-    return {'statusCode': 200, 'body': 'Success.'}
+    return {'statusCode': 200, 'body': 'Low GPU utilization issues found.'}
```

### Comparing `sagemaker-ssh-helper-2.1.0/sagemaker_ssh_helper/cdk/low_gpu/low_gpu_lambda_stack.py` & `sagemaker_ssh_helper-2.2.0/sagemaker_ssh_helper/cdk/low_gpu/low_gpu_lambda_stack.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,14 +48,15 @@
             handler="sagemaker_ssh_helper.cdk.low_gpu.low_gpu_lambda.handler",
             role=role,
             environment={
                 "SNS_NOTIFICATION_TOPIC_ARN": sns_topic.topic_arn
 
             },
             timeout=Duration.seconds(60),
+            memory_size=256,
         )
 
         low_gpu_rule = events.Rule(
             self, "profiler-low-gpu-checker-rule",
             event_pattern=events.EventPattern(
                 source=["aws.sagemaker"],
                 detail_type=events.Match.exact_string("SageMaker Processing Job State Change")
```

### Comparing `sagemaker-ssh-helper-2.1.0/sagemaker_ssh_helper/deregister_old_instances_from_ssm.py` & `sagemaker_ssh_helper-2.2.0/sagemaker_ssh_helper/deregister_old_instances_from_ssm.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     print(f'Successfully deregistered {deregistered_success_count} out of {len(ssh_helper_instances)}'
           f' instances to deregister.')
 
 
 def main():
     print('This utility will deregister from SSM all SageMaker SSH Helper related managed instances.')
     print('WARNING: you should be careful NOT deregister managed instances that are not related to SageMaker SSH Helper.')
-    print('Usage: python deregister_old_instances_from_ssm.py [--preapproving-deregistration] [--delete-older-than-n-days <N>]')
+    print('Usage: sm-ssh-deregister-instances [--preapproving-deregistration] [--delete-older-than-n-days <N>]')
     print('--preapproving-deregistration: will automatically approve the deregistration of all instances found, without prompting.')
     print('--delete-older-than-n-days <N>: will only delete offline instances that are older than N days.')
     print('')
 
     try:
         index = sys.argv.index('--delete-older-than-n-days')
         days = int(sys.argv[index + 1])
```

### Comparing `sagemaker-ssh-helper-2.1.0/sagemaker_ssh_helper/detached_sagemaker.py` & `sagemaker_ssh_helper-2.2.0/sagemaker_ssh_helper/detached_sagemaker.py`

 * *Files identical despite different names*

### Comparing `sagemaker-ssh-helper-2.1.0/sagemaker_ssh_helper/env.py` & `sagemaker_ssh_helper-2.2.0/sagemaker_ssh_helper/env.py`

 * *Files identical despite different names*

### Comparing `sagemaker-ssh-helper-2.1.0/sagemaker_ssh_helper/ide.py` & `sagemaker_ssh_helper-2.2.0/sagemaker_ssh_helper/ide.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from sagemaker_ssh_helper.log import SSHLog
 from sagemaker_ssh_helper.manager import SSMManager
 
 
 class IDEAppStatus:
 
-    def __init__(self, status, failure_reason) -> None:
+    def __init__(self, status, failure_reason=None) -> None:
         super().__init__()
         self.failure_reason = failure_reason
         self.status = status
 
     def is_pending(self):
         return self.status == 'Pending'
 
@@ -70,19 +70,19 @@
         :param image_name_or_arn: [name] from the images doc above or the full ARN
         :param instance_type:
         :param ssh_lifecycle_config:
         :param recreate:
         """
         self.logger.info(f"Creating kernel app {app_name} with SSH lifecycle config {ssh_lifecycle_config}")
         self.log_urls(app_name)
-        status = self.get_kernel_app_status(app_name)
+        status = self.get_app_status(app_name)
         while status.is_in_transition():
             self.logger.info(f"Waiting for the final status. Current status: {status}")
             time.sleep(10)
-            status = self.get_kernel_app_status(app_name)
+            status = self.get_app_status(app_name)
 
         self.logger.info(f"Previous app status: {status}")
 
         if status.is_in_service():
             if recreate:
                 self.delete_app(app_name, 'KernelGateway')
             else:
@@ -97,24 +97,25 @@
 
         account_id = boto3.client('sts').get_caller_identity().get('Account')
         lifecycle_arn = f"arn:aws:sagemaker:{self.current_region}:{account_id}:" \
                         f"studio-lifecycle-config/{ssh_lifecycle_config}"
 
         self.create_app(app_name, 'KernelGateway', instance_type, image_arn, lifecycle_arn)
 
-    def get_kernel_app_status(self, app_name: str) -> IDEAppStatus:
+    def get_app_status(self, app_name: str, app_type: str = 'KernelGateway') -> IDEAppStatus:
         """
+        :param app_type:
         :param app_name:
         :return: None | 'InService' | 'Deleted' | 'Deleting' | 'Failed' | 'Pending'
         """
         response = None
         try:
             response = self.client.describe_app(
                 DomainId=self.domain_id,
-                AppType='KernelGateway',
+                AppType=app_type,
                 UserProfileName=self.user,
                 AppName=app_name,
             )
         except ClientError as e:
             error_code = e.response.get("Error", {}).get("Code")
             if error_code == 'ResourceNotFound':
                 pass
@@ -148,19 +149,19 @@
             message = e.response.get("Error", {}).get("Message")
             self.logger.warning("ClientError code: " + code)
             self.logger.warning("ClientError message: " + message)
             if code == 'AccessDeniedException':
                 raise
             return
 
-        status = self.get_kernel_app_status(app_name)
+        status = self.get_app_status(app_name)
         while wait and status.is_deleting():
             self.logger.info(f"Waiting for the Deleted status. Current status: {status}")
             time.sleep(10)
-            status = self.get_kernel_app_status(app_name)
+            status = self.get_app_status(app_name)
         self.logger.info(f"Status after delete: {status}")
         if wait and not status.is_deleted():
             raise ValueError(f"Failed to delete app {app_name}. Status: {status}")
 
     def create_app(self, app_name, app_type, instance_type, image_arn,
                    lifecycle_arn: str = None):
         self.logger.info(f"Creating {app_type} app {app_name} on {instance_type} "
@@ -175,19 +176,19 @@
         _ = self.client.create_app(
             DomainId=self.domain_id,
             AppType=app_type,
             AppName=app_name,
             UserProfileName=self.user,
             ResourceSpec=resource_spec,
         )
-        status = self.get_kernel_app_status(app_name)
+        status = self.get_app_status(app_name)
         while status.is_pending():
             self.logger.info(f"Waiting for the InService status. Current status: {status}")
             time.sleep(10)
-            status = self.get_kernel_app_status(app_name)
+            status = self.get_app_status(app_name)
 
         self.logger.info(f"New app status: {status}")
 
         if not status.is_in_service():
             raise ValueError(
                 f"Failed to create app {app_name}. Status: '{status}'. "
                 f"Check remote logs at {self.get_cloudwatch_url(app_name)} "
@@ -195,31 +196,37 @@
             )
 
     def resolve_sagemaker_kernel_image_arn(self, image_name):
         sagemaker_account_id = "470317259841"  # eu-west-1, TODO: check all images
         return f"arn:aws:sagemaker:{self.current_region}:{sagemaker_account_id}:image/{image_name}"
 
     def print_kernel_instance_id(self, app_name, timeout_in_sec, index: int = 0):
-        print(self.get_kernel_instance_ids(app_name, timeout_in_sec)[index])
+        print(self.get_kernel_instance_id(app_name, timeout_in_sec, index))
 
-    def get_kernel_instance_ids(self, app_name, timeout_in_sec):
-        self.logger.info("Resolving IDE instance IDs through SSM tags")
+    def get_kernel_instance_id(self, app_name, timeout_in_sec, index: int = 0,
+                               not_earlier_than_timestamp: int = 0):
+        return self.get_kernel_instance_ids(app_name, timeout_in_sec, not_earlier_than_timestamp)[index]
+
+    def get_kernel_instance_ids(self, app_name: str, timeout_in_sec: int, not_earlier_than_timestamp: int = 0):
+        self.logger.info(f"Resolving IDE instance IDs for app '{app_name}' through SSM tags "
+                         f"in domain '{self.domain_id}' for user '{self.user}'")
         self.log_urls(app_name)
         if self.domain_id and self.user:
-            result = SSMManager().get_studio_user_kgw_instance_ids(self.domain_id, self.user, app_name, timeout_in_sec)
+            result = SSMManager().get_studio_user_kgw_instance_ids(self.domain_id, self.user, app_name,
+                                                                   timeout_in_sec, not_earlier_than_timestamp)
         elif self.user:
             self.logger.warning(f"Domain ID is not set. Will attempt to connect to the latest "
                                 f"active kernel gateway with the name {app_name} in the region {self.current_region} "
                                 f"for user profile {self.user}")
             result = SSMManager().get_studio_user_kgw_instance_ids("", self.user, app_name,
-                                                                   timeout_in_sec)
+                                                                   timeout_in_sec, not_earlier_than_timestamp)
         else:
             self.logger.warning(f"Domain ID or user profile name are not set. Will attempt to connect to the latest "
                                 f"active kernel gateway with the name {app_name} in the region {self.current_region}")
-            result = SSMManager().get_studio_kgw_instance_ids(app_name, timeout_in_sec)
+            result = SSMManager().get_studio_kgw_instance_ids(app_name, timeout_in_sec, not_earlier_than_timestamp)
         return result
 
     def log_urls(self, app_name):
         self.logger.info(f"Remote logs are at {self.get_cloudwatch_url(app_name)}")
         if self.domain_id and self.user:
             self.logger.info(f"Remote apps metadata is at {self.get_user_metadata_url()}")
 
@@ -315,7 +322,27 @@
     def wait_for_image_deletion(self, image_name):
         self.logger.info(f"Waiting for SageMaker image deletion: {image_name}")
         waiter = self.client.get_waiter('image_deleted')
         waiter.wait(
             ImageName=image_name
         )
         self.logger.info(f"Image deleted: {image_name}")
+
+
+class NotebookInstance:
+    logger = logging.getLogger('sagemaker-ssh-helper:NotebookInstance')
+
+    def __init__(self, notebook_name, region_name: str = None):
+        self.notebook_name = notebook_name
+        self.current_region = region_name or boto3.session.Session().region_name
+        self.client = boto3.client('sagemaker', region_name=self.current_region)
+        self.ssh_log = SSHLog(region_name=self.current_region)
+
+    def get_instance_ids(self):
+        result = SSMManager().get_notebook_instance_ids(self.notebook_name)
+        return result
+
+    def get_cloudwatch_url(self):
+        raise ValueError("Not implemented")
+
+    def get_metadata_url(self):
+        raise ValueError("Not implemented")
```

### Comparing `sagemaker-ssh-helper-2.1.0/sagemaker_ssh_helper/log.py` & `sagemaker_ssh_helper-2.2.0/sagemaker_ssh_helper/log.py`

 * *Files 3% similar despite different names*

```diff
@@ -66,24 +66,29 @@
         self.logger.warning("SSMManager#get_transformer_instance_ids() is faster and more stable")
         self.logger.info(f"Querying SSM instance IDs for transform job {transform_job_name}")
         return self.get_ssm_instance_ids(f'/aws/sagemaker/TransformJobs', transform_job_name,
                                          timeout_in_sec=timeout_in_sec)
 
     def get_studio_kgw_ssm_instance_ids(self, kgw_name, timeout_in_sec=0):
         self.logger.warning("SSMManager#get_studio_kgw_instance_ids() is faster and more stable")
-        self.logger.info(f"Querying SSM instance IDs for SageMaker Studio kernel gateway {kgw_name}")
+        self.logger.info(f"Querying SSM instance IDs for SageMaker Studio kernel gateway: '{kgw_name}'")
         return self.get_ssm_instance_ids(f'/aws/sagemaker/studio', f"KernelGateway/{kgw_name}",
                                          timeout_in_sec=timeout_in_sec)
 
-    def get_instance_ids_once(self, arn_resource_type, arn_resource_name, arn_filter_regex: str = None):
+    def get_instance_ids_once(self, arn_resource_type, arn_resource_name, arn_filter_regex: str = None,
+                              not_earlier_than_timestamp: int = 0):
         if arn_filter_regex:
             raise ValueError("Not supported for SSHLog")
-        return self.get_ssm_instance_ids_once(log_group=arn_resource_type, stream_name=arn_resource_name)
+        return self.get_ssm_instance_ids_once(log_group=arn_resource_type, stream_name=arn_resource_name,
+                                              not_earlier_than_timestamp=not_earlier_than_timestamp)
 
-    def get_ssm_instance_ids_once(self, log_group, stream_name):
+    def get_ssm_instance_ids_once(self, log_group, stream_name,
+                                  not_earlier_than_timestamp: int = 0):
+        if not_earlier_than_timestamp > 0:
+            raise ValueError("Not implemented for SSHLog yet")
         query = "fields @timestamp, @logStream, @message" \
                 f"| filter @logStream like '{stream_name}'" \
                 "| filter @message like /Successfully registered the instance with AWS SSM using Managed instance-id/" \
                 "| sort @timestamp desc" \
                 "| limit 20"
         lines = self._query_log_group(log_group, query)
         mi_ids = []
```

### Comparing `sagemaker-ssh-helper-2.1.0/sagemaker_ssh_helper/manager.py` & `sagemaker_ssh_helper-2.2.0/sagemaker_ssh_helper/manager.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,75 +18,84 @@
         self.region_name = region_name or boto3.session.Session().region_name
         self.sleep_between_retries_in_seconds = sleep_between_retries_in_seconds
         self.redo_attempts = redo_attempts
 
     def get_instance_ids(self, arn_resource_type, arn_resource_name,
                          timeout_in_sec=0,
                          expected_count=1,
-                         arn_filter_regex: str = None):
+                         arn_filter_regex: str = None,
+                         not_earlier_than_timestamp: int = 0):
         if arn_resource_name.startswith('mi-'):
             self.logger.warning("SageMaker resource name usually doesn't not start with 'mi-', "
                                 "did you pass the SSM instance ID by mistake?")
         self.logger.info("Using AWS Region: %s", self.region_name)
-        mi_ids = self.get_instance_ids_once(arn_resource_type, arn_resource_name, arn_filter_regex)
+        mi_ids = self.get_instance_ids_once(arn_resource_type, arn_resource_name, arn_filter_regex,
+                                            not_earlier_than_timestamp)
 
         while not mi_ids and timeout_in_sec > 0:
-            self.logger.info(f"No instance IDs found. Retrying. Is SSM Agent running on the remote? "
-                             f"Check the remote logs. Seconds left before time out: {timeout_in_sec}")
+            self.logger.info(f"No instance IDs found. Seconds left before time out: {timeout_in_sec}")
             time.sleep(self.sleep_between_retries_in_seconds)
-            mi_ids = self.get_instance_ids_once(arn_resource_type, arn_resource_name)
+            mi_ids = self.get_instance_ids_once(arn_resource_type, arn_resource_name, arn_filter_regex,
+                                                not_earlier_than_timestamp)
             timeout_in_sec -= self.sleep_between_retries_in_seconds
 
         self.logger.info(f"Got preliminary SSM instance IDs: {mi_ids}")
 
         redo_attempts = self.redo_attempts
-        while len(mi_ids) < expected_count and redo_attempts > 0:
+        while len(mi_ids) < expected_count and redo_attempts > 0 and timeout_in_sec > 0:
             self.logger.info(f"Re-fetch results for other instances to catchup. Attempts left: {redo_attempts}")
             time.sleep(30)
-            mi_ids = self.get_instance_ids_once(arn_resource_type, arn_resource_name)
+            mi_ids = self.get_instance_ids_once(arn_resource_type, arn_resource_name, arn_filter_regex,
+                                                not_earlier_than_timestamp)
             redo_attempts -= 1
 
         self.logger.info(f"Got final SSM instance IDs: {mi_ids}")
         return mi_ids
 
     @abstractmethod
-    def get_instance_ids_once(self, arn_resource_type, arn_resource_name, arn_filter_regex: str = None):
+    def get_instance_ids_once(self, arn_resource_type, arn_resource_name, arn_filter_regex: str = None,
+                              not_earlier_than_timestamp: int = 0):
         raise NotImplementedError("Abstract method")
 
 
 class SSMManager(SSMManagerBase):
+    PING_STATUS = '$__SSMManager__.PingStatus'
+
     logger = logging.getLogger('sagemaker-ssh-helper:SSMManager')
 
     def __init__(self, region_name=None, sleep_between_retries_in_seconds=10, redo_attempts=5,
                  clock_timestamp_override=None) -> None:
         super().__init__(region_name, sleep_between_retries_in_seconds, redo_attempts)
         self.clock_timestamp_override = clock_timestamp_override
 
-    def list_all_instances_with_tags(self) -> Dict[str, Dict[str, str]]:
+    def list_all_instances_and_fetch_tags(self) -> Dict[str, Dict[str, str]]:
+        """
+        :return: a mapping of instance ID to the dictionary of tags
+        """
         ssm = boto3.client('ssm', region_name=self.region_name)
 
         result = {}
-        next_token = ""  # nosec hardcoded_password_string  # not a password
-        while next_token is not None:
+        next_page_id = ""
+        while next_page_id is not None:
             response = ssm.describe_instance_information(
                 Filters=[{'Key': 'ResourceType', 'Values': ['ManagedInstance']}],
-                NextToken=next_token,
+                NextToken=next_page_id,
                 MaxResults=50,
             )
-            next_token = response.get('NextToken')
+            next_page_id = response.get('NextToken')
             info_list = response['InstanceInformationList']
             if info_list:
                 for info in info_list:
                     instance_id = info['InstanceId']
                     tags = ssm.list_tags_for_resource(ResourceType='ManagedInstance', ResourceId=instance_id)
                     tags_dict = {}
                     if 'TagList' in tags:
                         for tag in tags['TagList']:
                             tags_dict[tag['Key']] = tag['Value']
-                    tags_dict['$__SSMManager__.PingStatus'] = info['PingStatus']
+                    tags_dict[SSMManager.PING_STATUS] = info['PingStatus']
                     result[instance_id] = tags_dict
 
         return result
 
     def get_training_instance_ids(self, training_job_name, timeout_in_sec=0, expected_count=1):
         self.logger.info(f"Querying SSM instance IDs for training job {training_job_name}, "
                          f"expected instance count = {expected_count}")
@@ -100,67 +109,74 @@
     def get_endpoint_instance_ids(self, endpoint_name, timeout_in_sec=0):
         raise AssertionError("Not supported yet.")
 
     def get_transformer_instance_ids(self, transform_job_name, timeout_in_sec=0):
         self.logger.info(f"Querying SSM instance IDs for transform job {transform_job_name}")
         return self.get_instance_ids('transform-job', transform_job_name, timeout_in_sec)
 
-    def get_studio_user_kgw_instance_ids(self, domain_id, user_profile_name, kgw_name, timeout_in_sec=0):
-        self.logger.info(f"Querying SSM instance IDs for SageMaker Studio kernel gateway {kgw_name}")
+    def get_studio_user_kgw_instance_ids(self, domain_id, user_profile_name, kgw_name, timeout_in_sec=0,
+                                         not_earlier_than_timestamp: int = 0):
+        self.logger.info(f"Querying SSM instance IDs for SageMaker Studio kernel gateway: '{kgw_name}'")
         if not domain_id:
             arn_filter = f":app/.*/{user_profile_name}/"
         else:
             arn_filter = f":app/{domain_id}/{user_profile_name}/"
         return self.get_instance_ids('app', f"{kgw_name}", timeout_in_sec,
-                                     arn_filter_regex=arn_filter)
+                                     arn_filter_regex=arn_filter,
+                                     not_earlier_than_timestamp=not_earlier_than_timestamp)
 
-    def get_studio_kgw_instance_ids(self, kgw_name, timeout_in_sec=0):
-        self.logger.info(f"Querying SSM instance IDs for SageMaker Studio kernel gateway {kgw_name}")
-        return self.get_instance_ids('app', f"{kgw_name}", timeout_in_sec)
+    def get_studio_kgw_instance_ids(self, kgw_name, timeout_in_sec=0, not_earlier_than_timestamp: int = 0):
+        self.logger.info(f"Querying SSM instance IDs for SageMaker Studio kernel gateway: '{kgw_name}'")
+        return self.get_instance_ids('app', f"{kgw_name}", timeout_in_sec,
+                                     not_earlier_than_timestamp)
 
     def get_notebook_instance_ids(self, instance_name, timeout_in_sec=0):
         self.logger.info(f"Querying SSM instance IDs for SageMaker notebook instance {instance_name}")
-        return self.get_instance_ids('notebook-instance', f"{instance_name}", timeout_in_sec)
+        return self.get_instance_ids('notebook-instance', f"{instance_name}",
+                                     timeout_in_sec)
 
     def get_instance_ids_once(self, arn_resource_type, arn_resource_name,
-                              arn_filter_regex: str = None):
+                              arn_filter_regex: str = None,
+                              not_earlier_than_timestamp: int = 0):
         # TODO: use tag filter instead, for faster performance
-        all_instances = self.list_all_instances_with_tags()
+        all_instances = self.list_all_instances_and_fetch_tags()
         result_pairs = []
         for mi_id in all_instances:
             tags = all_instances[mi_id]
             if "SSHResourceName" not in tags or "SSHResourceArn" not in tags:
                 continue
             if f"/{arn_resource_name}" in tags["SSHResourceArn"] and \
                     arn_resource_name == tags["SSHResourceName"] and \
                     f":{arn_resource_type}/" in tags["SSHResourceArn"] and \
                     (not arn_filter_regex or re.search(arn_filter_regex, tags["SSHResourceArn"]) is not None):
                 if "SSHTimestamp" in tags:
-                    timestamp = tags["SSHTimestamp"]
+                    timestamp = int(tags["SSHTimestamp"])
                 else:
                     timestamp = 0
+                if timestamp < not_earlier_than_timestamp:
+                    continue
                 result_pairs.append((mi_id, timestamp))
 
         result_pairs.sort(key=lambda i: i[1], reverse=True)
         result = [i[0] for i in result_pairs]
         return result
 
     def list_expired_ssh_instances(self, expiration_days=0):
-        all_instances = self.list_all_instances_with_tags()
+        all_instances = self.list_all_instances_and_fetch_tags()
         logging.info("Found %s instances in SSM", len(all_instances))
 
         expired_instances = []
         for mi_id in all_instances:
             tags = all_instances[mi_id]
             if "SSHTimestamp" in tags:
                 timestamp = int(tags["SSHTimestamp"])
             else:
                 timestamp = 0
-            if "$__SSMManager__.PingStatus" in tags:
-                ping_status = tags["$__SSMManager__.PingStatus"]
+            if SSMManager.PING_STATUS in tags:
+                ping_status = tags[SSMManager.PING_STATUS]
             else:
                 ping_status = "Online"
             if ping_status == "Online":
                 continue
             if self.clock_timestamp_override is not None:
                 expiration_timestamp = self.clock_timestamp_override
             else:
@@ -168,7 +184,18 @@
             expiration_timestamp -= expiration_days * 3600 * 24
             if timestamp < expiration_timestamp:
                 expired_instances.append(mi_id)
                 logging.info("Found expired offline SSH instance %s with timestamp %s", mi_id, timestamp)
 
         logging.info("Found %s expired offline SSH instances", len(expired_instances))
         return expired_instances
+
+    def get_ssh_instance_timestamp(self, instance_id):
+        ssm = boto3.client('ssm', region_name=self.region_name)
+        tags = ssm.list_tags_for_resource(ResourceType='ManagedInstance', ResourceId=instance_id)
+        tag_list = tags['TagList']
+
+        for tag in tag_list:
+            if tag['Key'] == 'SSHTimestamp':
+                return int(tag['Value'])
+
+        return 0
```

### Comparing `sagemaker-ssh-helper-2.1.0/sagemaker_ssh_helper/proxy.py` & `sagemaker_ssh_helper-2.2.0/sagemaker_ssh_helper/proxy.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,16 +21,20 @@
         self.cloudwatch_url = cloudwatch_url
         self.p: Optional[subprocess.Popen] = None
         self.q: Optional[Queue] = None
         self.t: Optional[Thread] = None
         self.region_name = region_name
         self.extra_args = extra_args
         self.ssh_listen_port = ssh_listen_port
+        self.connected = False
 
     def connect_to_ssm_instance(self, instance_id) -> None:
+        if self.connected:
+            raise Exception("Already connected")
+
         self.logger.info(
             f"Connecting to {instance_id} with SSM and starting SSH port forwarding "
             f"on local port {self.ssh_listen_port}"
             + (f" with extra args: '{self.extra_args}'" if self.extra_args else '')
         )
 
         env = os.environ.copy()
@@ -73,14 +77,17 @@
         output_str = output.decode("latin1")
 
         self.logger.info("Got output from the remote: " + output_str.replace("\n", " "))
 
         if not output_str.startswith("Linux"):
             raise ValueError("Failed to get system version. Got instead: " + output_str)
 
+        self.connected = True
+        self.logger.info(f"Connected to remote instance {instance_id}")
+
     def terminate_waiting_loop(self):
         self.logger.info("Terminating the remote waiting loop / sleep process")
         retval = self.run_command("sm-wait stop")
         if retval != 0:
             proc_list = self.run_command_with_output("sm-wait list")
             self.logger.info(f"List of sm-wait-processes: {proc_list}")
             raise ValueError(
@@ -160,14 +167,15 @@
             except ConnectionRefusedError:
                 time.sleep(1)
         if is_timeout:
             self.logger.warning(f"Timeout waiting for connection on 127.0.0.1:{self.ssh_listen_port}")
 
     def disconnect(self):
         self.logger.info(f"Disconnecting proxy and stopping SSH port forwarding")
+        self.connected = False
         parent = psutil.Process(self.p.pid)
         try:
             for child in parent.children(recursive=True):
                 child.terminate()
             parent.terminate()
         except psutil.NoSuchProcess:
             pass
```

### Comparing `sagemaker-ssh-helper-2.1.0/sagemaker_ssh_helper/sm-helper-functions` & `sagemaker_ssh_helper-2.2.0/sagemaker_ssh_helper/sm-helper-functions`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,17 @@
 #!/bin/bash
 
+function _python() {
+  if python3 --version 2>&1 | grep '^Python 3' >/dev/null 2>&1; then
+    echo "python3"
+  else
+    echo "python"
+  fi
+}
+
 function _silent_install() {
   install_path="/usr/local/bin"
 
   dir=$(dirname "$0")
   script=$1
   mod=$2
 
@@ -30,21 +38,25 @@
   command -v yum >/dev/null 2>&1
 }
 
 function _is_macos() {
   uname | grep ^Darwin >/dev/null
 }
 
+function _is_windows() {
+  uname | grep ^MINGW >/dev/null
+}
+
 function _install_unzip() {
-  if _is_macos; then
+  if _is_macos || _is_windows; then
     :  # noop, should be already installed
   elif _is_centos; then
     sudo yum install -y unzip
   else
-    sudo apt-get install -y --no-install-recommends unzip
+    sudo DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends unzip
   fi
 }
 
 function _install_aws_cli_linux() {
   curl -sS "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "/tmp/awscliv2.zip"
   unzip -o -q -d /tmp/ /tmp/awscliv2.zip
   sudo /tmp/aws/install --update
@@ -57,15 +69,17 @@
 
 function _install_aws_cli() {
   echo "sagemaker-ssh-helper: Installing AWS CLI v2"
   which aws || echo "sagemaker-ssh-helper: No previous installation of AWS CLI detected"
   which pip >/dev/null 2>&1 && pip uninstall -y awscli
 
   # See: https://docs.aws.amazon.com/cli/latest/userguide/getting-started-install.html
-  if _is_macos; then
+  if _is_windows; then
+    msiexec.exe //i https://awscli.amazonaws.com/AWSCLIV2.msi || echo "WARNING: msiexec.exe existed with non-zero code."
+  elif _is_macos; then
     _install_aws_cli_macos
   else
     _install_aws_cli_linux
   fi
 }
 
 function _install_ssm_agent_ubuntu() {
@@ -103,38 +117,45 @@
   curl -sS "https://s3.amazonaws.com/session-manager-downloads/plugin/latest/mac/session-manager-plugin.pkg" \
     -o "/tmp/session-manager-plugin.pkg"
   sudo installer -pkg /tmp/session-manager-plugin.pkg -target /
   sudo rm -f /usr/local/bin/session-manager-plugin
   sudo ln -s /usr/local/sessionmanagerplugin/bin/session-manager-plugin /usr/local/bin/session-manager-plugin
 }
 
+function _install_session_manager_plugin_windows() {
+  curl -sS "https://s3.amazonaws.com/session-manager-downloads/plugin/latest/windows/SessionManagerPluginSetup.exe" \
+    -o "/tmp/SessionManagerPluginSetup.exe"
+  /tmp/SessionManagerPluginSetup.exe || echo "Warning: SessionManagerPluginSetup.exe existed with non-zero code."
+}
+
 function _install_session_manager_plugin() {
   # See https://docs.aws.amazon.com/systems-manager/latest/userguide/session-manager-working-with-install-plugin.html
-  if _is_centos; then
+  if _is_windows; then
+    _install_session_manager_plugin_windows
+  elif _is_centos; then
     _install_session_manager_plugin_centos
   elif _is_macos; then
     _install_session_manager_plugin_macos
   else
     _install_session_manager_plugin_ubuntu
   fi
-  session-manager-plugin
 }
 
 
 
 function _install_curl_ubuntu() {
-  sudo apt-get install -y --no-install-recommends curl
+  sudo DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends curl
 }
 
 function _install_curl_centos() {
   sudo yum install -y curl
 }
 
 function _install_curl() {
-  if _is_macos; then
+  if _is_macos || _is_windows; then
     :  # noop, should be already installed
   elif _is_centos; then
     _install_curl_centos
   else
     _install_curl_ubuntu
   fi
 }
@@ -165,14 +186,15 @@
 function _print_sm_domain_id() {
   sm_resource_metadata_json=$(tr -d "\n" < /opt/ml/metadata/resource-metadata.json)
   echo -n "$sm_resource_metadata_json" | sed -e 's/^.*"DomainId":\"\([^"]*\)\".*$/\1/'
 }
 
 # shellcheck disable=SC2001
 function _print_sm_user_profile_name() {
+  # FIXME: Check for "SpaceName" - spaces are not supported yet
   sm_resource_metadata_json=$(tr -d "\n" < /opt/ml/metadata/resource-metadata.json)
   echo -n "$sm_resource_metadata_json" | sed -e 's/^.*"UserProfileName":\"\([^"]*\)\".*$/\1/'
 }
 
 function _print_sm_studio_python() {
   SM_STUDIO_PYTHON=$(/opt/.sagemakerinternal/conda/bin/python -c \
       "from jupyter_client.kernelspec import KernelSpecManager; \
@@ -215,7 +237,50 @@
 function _start_sshd() {
   if _is_centos; then
     /usr/sbin/sshd
   else
     service ssh start || (echo "ERROR: Failed to start sshd service" && exit 255)
   fi
 }
+
+function _export_ssh_key_env_var() {
+  SM_SSH_HOST_NAME=$1
+  SSH_KEY=~/.ssh/${SM_SSH_HOST_NAME}
+  export SSH_KEY
+}
+
+function _check_ssh_proxy_host_name() {
+  SM_SSH_HOST_NAME=$1
+  SM_RESOURCE_TYPE=$2
+
+  if [[ "$SM_SSH_HOST_NAME" =~ ^.*\."$SM_RESOURCE_TYPE"\.sagemaker ]]; then
+    :
+  else
+    echo "sm-local-ssh-$SM_RESOURCE_TYPE: Error: Host name must end with '.$SM_RESOURCE_TYPE.sagemaker'"
+    exit 1
+  fi
+}
+
+function _generate_key_and_print_instance_id() {
+  SM_SSH_FQDN=$1
+  DOMAIN_ID=$2
+  USER_PROFILE_NAME=$3
+
+  if [[ -f $SSH_KEY ]]; then
+    # Don't generate again, or it will confuse SSH
+    # Only touch the file so it can be easily identified when you sort by last access timestamp
+    touch "$SSH_KEY"
+  else
+    # echo "Generating $SSH_KEY keypair with ECDSA and uploading public key to $SSH_AUTHORIZED_KEYS"
+    echo 'yes' | ssh-keygen -t ecdsa -q -f "${SSH_KEY}" -N '' >/dev/null
+  fi
+
+  # shellcheck disable=SC2091  # execute python location
+  $(_python) <<EOF
+import logging
+logging.basicConfig(level=logging.ERROR);
+logging.getLogger('sagemaker.config').setLevel(logging.WARNING)
+import sagemaker; from sagemaker_ssh_helper.wrapper import SSHEnvironmentWrapper;
+print(SSHEnvironmentWrapper.attach_to_resource("$SM_SSH_FQDN", "$DOMAIN_ID", "$USER_PROFILE_NAME").get_instance_id(timeout_in_sec=0));
+EOF
+
+}
```

### Comparing `sagemaker-ssh-helper-2.1.0/sagemaker_ssh_helper/sm-init-ssm` & `sagemaker_ssh_helper-2.2.0/sagemaker_ssh_helper/sm-init-ssm`

 * *Files 5% similar despite different names*

```diff
@@ -4,19 +4,25 @@
 # If successful, the log line with the instance ID will look like this:
 #   Successfully registered the instance with AWS SSM using Managed instance-id: mi-01234567890abcdef
 
 # Requires environment variable SSH_SSM_ROLE to be passed as an argument
 # The role for SSM is not a full IAM ARN, but only the last part of it such as 'service-role/SageMakerRole'
 
 set -e
+set -o pipefail
 
-dir=$(dirname "$0")
+self=$(realpath "${BASH_SOURCE[0]}")
+dir=$(dirname "$self")
 source "$dir"/sm-helper-functions
 
 CURRENT_REGION=$(aws configure get region || echo "$AWS_REGION")
+if [ -z "${CURRENT_REGION}" ]; then
+  echo "ERROR: AWS Region cannot be determined. Try to run 'aws configure get region' manually and check the output."
+  exit 1
+fi
 
 SSH_CREATOR=$(aws sts get-caller-identity | jq --raw-output '.UserId')
 SSH_TIMESTAMP=$(date +%s)
 
 if [ -f /opt/ml/metadata/resource-metadata.json ]; then
   # SageMaker Studio and notebook instances
   RESOURCE_NAME=$(jq --raw-output '.ResourceName' < /opt/ml/metadata/resource-metadata.json)
@@ -27,15 +33,15 @@
   RESOURCE_ARN=$(jq --raw-output '.ProcessingJobArn' < /opt/ml/config/processingjobconfig.json)
 elif [[ "$TRAINING_JOB_NAME" != "" ]]; then
   # Training job
   RESOURCE_NAME=$TRAINING_JOB_NAME
   RESOURCE_ARN=$TRAINING_JOB_ARN  # empty for local mode
 elif [[ "$TRANSFORM_JOB_ARN" != "" ]]; then
   # Transform job
-  RESOURCE_NAME=$(echo $TRANSFORM_JOB_ARN | awk -F/ '{print $2}')
+  RESOURCE_NAME=$(echo "$TRANSFORM_JOB_ARN" | awk -F/ '{print $2}')
   RESOURCE_ARN=$TRANSFORM_JOB_ARN
 else
   # Probably, endpoint
   RESOURCE_NAME=""
   RESOURCE_ARN=""
 fi
```

### Comparing `sagemaker-ssh-helper-2.1.0/sagemaker_ssh_helper/sm-save-env` & `sagemaker_ssh_helper-2.2.0/sagemaker_ssh_helper/sm-save-env`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #!/bin/bash
 
 # When a user logs in with SSH or remote interpreter, we want env vars to be the same as set by SageMaker
 
 set -e
+set -o pipefail
 
 if [[ "$1" == "print-vars" ]]; then
   # Wrap all vars into single quotes, wrap single quotes into double quotes
   # Also works for multi-line variables
   # A=test -> A='test'
   # B='test' -> B=''"'"'test'"'"''
   # C="test" -> C='"test"'
```

### Comparing `sagemaker-ssh-helper-2.1.0/sagemaker_ssh_helper/sm-setup-ssh` & `sagemaker_ssh_helper-2.2.0/sagemaker_ssh_helper/sm-setup-ssh`

 * *Files 22% similar despite different names*

```diff
@@ -2,18 +2,30 @@
 
 # Main entry point to be called from training / processing jobs or inference endpoint by SageMaker.
 # It will be either called from setup.py automatically when installing the 'sagemaker-ssh-helper' package
 # from 'requirements.txt' and 'bootstrap_on_start' parameter was passed to the wrapper, or manually
 # from training / processing / inference script, e. g. with subprocess.check_call()
 
 set -e
+set -o pipefail
+
+# Uncomment below option for debugging
+#set -x
 
 dir=$(dirname "$0")
 source "$dir"/sm-helper-functions
 
+terminate() {
+    echo "sm-setup-ssh: Terminated."
+    exit 2
+}
+
+trap terminate SIGTERM
+trap terminate SIGINT
+
 # This script can be called simultaneously multiple times in a distributed training or inference job
 # To avoid race conditions, we install helper scripts under an exclusive lock
 if [[ "$1" == "install-helper-scripts" ]]; then
   _install_helper_scripts
   exit 0
 fi
 
@@ -24,24 +36,28 @@
       exit 0
   fi
 
   chmod 1777 /tmp
   mkdir -p ~/.ssh
   [ -d /usr/share/man/man1 ] || mkdir /usr/share/man/man1
 
-  echo "Installing SSH server and auxiliary tools"
   if _is_centos; then
+    echo "Installing SSH server and auxiliary tools on CentOS"
     yum install -y openssh-server net-tools procps less jq vim rsync perl rsyslog
   else
     export DEBIAN_FRONTEND=noninteractive
+    echo 'Retrieving the new lists of Debian packages'
     apt-get -qq update || echo 'sm-ssh-ide: WARNING - issues with retrieving new lists of packages'
+    echo 'Installing Debian package manager utilities'
     apt-get -qq -y install apt-utils
-    apt-get -qq -y install ssh net-tools procps less jq vim rsync locales rsyslog
+    echo "Installing SSH server and auxiliary tools"
+    apt-mark hold python3-distro ssh-import-id  # workaround to make installation work on Trn1
+    apt-get -y install ssh net-tools procps less jq vim rsync locales rsyslog
 
-    # Install some locales to work with UTF-8 charsets
+    echo 'Installing locales to work with UTF-8 charsets'
     echo "C.UTF-8 UTF-8" >> /etc/locale.gen
     echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen
   fi
 
   # Sending all system logs to CloudWatch (helps to troubleshoot sshd issues)
   if _is_ssh_ide_inside_studio; then
     find /etc/rsyslog.conf /etc/rsyslog.d/ -type f \
@@ -101,14 +117,17 @@
   source "$dir"/sm-helper-functions
 
   sm-setup-ssh configure
 
   # Log IP addresses of the container (useful only in training in combination with VPC + VPN)
   echo "SSH Helper Log IP: $(hostname -I)"
 
+  # Log OS version
+  head -2 /etc/os-release || :
+
   # Save and dump SageMaker environment for SSH sessions
   sm-save-env
 
   # Dump container bootstrap environment (PID 1) - can be different from above, useful for debugging
   ps wwwe -p 1 | tail -1
 
   _locale_gen
@@ -120,27 +139,36 @@
   # Running forever as daemon
   amazon-ssm-agent
 
   echo "ERROR: agent died"
   exit 1  # should never reach this line
 fi
 
+# All subprocesses should have access to helper scripts, so each one needs to wait until they are fully installed
+# But we don't know which subprocess will start and finish first
+# flock prevents from race condition during installation
+# Useful for distributed training on multiple GPUs
+echo "[sagemaker-ssh-helper][sm-setup-ssh] Acquiring an exclusive blocking lock and installing scripts."
 flock /tmp/sm-install-lock bash "$0" install-helper-scripts \
   | sed -u 's/^/[sagemaker-ssh-helper][sm-setup-ssh][install-helper-scripts] /'
 
 # nohup will detach the child process from parent and run it in background
 # flock prevents from starting more than 1 process
 # redirection to /proc/1/fd/1 will write logs to CloudWatch
 # sed will prepend log output with SSH Helper prefix
 if [[ ! -f /tmp/sm-start-ssh-lock ]]; then
+  echo "[sagemaker-ssh-helper][sm-setup-ssh] Acquiring a non-blocking lock and starting SSH setup process in background."
   if [[ "$SSH_LOG_TO_STDOUT" == "true" ]]; then
     flock -n /tmp/sm-start-ssh-lock bash "$0" start-ssh &
   else
     nohup flock -n /tmp/sm-start-ssh-lock \
       bash "$0" start-ssh 2>&1 \
         | sed -u 's/^/[sagemaker-ssh-helper][sm-setup-ssh][start-ssh] /' \
         >/proc/1/fd/1 2>&1 &
   fi
+  echo "[sagemaker-ssh-helper][sm-setup-ssh] SSH setup process is running in background."
+else
+  echo "[sagemaker-ssh-helper][sm-setup-ssh] Lock already exists, SSH setup process should be already running in background."
 fi
 
 sm-wait "${SSH_WAIT_TIME_SECONDS:-60}" \
   | sed -u 's/^/[sagemaker-ssh-helper][sm-setup-ssh][sm-wait] /'
```

### Comparing `sagemaker-ssh-helper-2.1.0/sagemaker_ssh_helper/sm-ssh-ide` & `sagemaker_ssh_helper-2.2.0/sagemaker_ssh_helper/sm-ssh-ide`

 * *Files 4% similar despite different names*

```diff
@@ -7,25 +7,28 @@
 # set-jb-license-server <jb-license-server-hostname-without-http>
 # set-vnc-password <123456>
 # get-user-profile-name
 # get-domain-id
 # get-metadata
 
 set -e
+set -o pipefail
 
 dir=$(dirname "$0")
 source "$dir"/sm-helper-functions
 
 if [[ "$1" == "configure" ]]; then
     # Everything that requires root and Internet goes to 'configure'
     if [[ -f /opt/sagemaker-ssh-helper/.ssh-ide-configured ]]; then
         echo "sm-ssh-ide: Already configured. Remove /opt/sagemaker-ssh-helper/.ssh-ide-configured to force reconfiguration."
         exit 0
     fi
 
+    echo "sm-ssh-ide: Configuring services..."
+
     OPTIONS=$2
     mkdir -p /opt/sagemaker-ssh-helper/
     echo "$OPTIONS" > /opt/sagemaker-ssh-helper/.sm-ssh-ide-options
 
     _install_helper_scripts
 
     cat >/etc/profile.d/sm-ssh-ide.sh <<EOF
@@ -70,15 +73,15 @@
 
     else
       echo "sm-ssh-ide: Skipping VNC and GUI apps install"
     fi
 
     touch /opt/sagemaker-ssh-helper/.ssh-ide-configured
 
-    echo "sm-ssh-ide: Configuration complete."
+    echo "sm-ssh-ide: Finished configuration. Done"
 
 elif [[ "$1" == "get-user-profile-name" ]]; then
   _assert_is_ssh_ide_inside_studio
   USER_PROFILE=$(_print_sm_user_profile_name)
   echo "$USER_PROFILE"
 
 elif [[ "$1" == "get-domain-id" ]]; then
@@ -89,16 +92,23 @@
 elif [[ "$1" == "get-metadata" ]]; then
   _assert_is_ssh_ide_inside_studio
 
   echo "App name: $(_print_sm_app_name)"
   echo "User profile name: $(_print_sm_user_profile_name)"
   echo "Domain: $(_print_sm_domain_id)"
   echo ""
-  echo "Connect from local machine (with GUI and Jupyter): sm-local-ssh-ide connect $(_print_sm_app_name)"
-  echo "To connect with SSH only: sm-local-ssh-ide connect $(_print_sm_app_name) --ssh-only"
+  echo "Connect from local machine (with GUI and Jupyter): "
+  echo "sm-local-ssh-ide connect $(_print_sm_app_name)"
+  echo "To connect with SSH only: "
+  echo "sm-local-ssh-ide connect $(_print_sm_app_name) --ssh-only"
+  echo ""
+  echo "Choose the domain (if you have multiple) on the local machine: "
+  echo "sm-local-ssh-ide set-domain-id $(_print_sm_domain_id)"
+  echo "To choose the user profile (if domain is shared): "
+  echo "sm-local-ssh-ide set-user-profile-name $(_print_sm_user_profile_name)"
 
 elif [[ "$1" == "set-jb-license-server" ]]; then
 
     JB_LICENSE_SERVER_HOST="$2"
 
     if [ -f ~/.sm-jb-license-server ]; then
         echo "sm-ssh-ide: PyCharm license server host is already configured in ~/.sm-jb-license-server, skipping override"
@@ -144,34 +154,55 @@
         LOCAL_USER_ID="$(cat ~/.sm-ssh-owner)"
     else
         echo "sm-ssh-ide: Saving local user ID into ~/.sm-ssh-owner"
         echo "$LOCAL_USER_ID" > ~/.sm-ssh-owner
     fi
 
 elif [[ "$1" == "init-ssm" ]]; then
+    echo "sm-ssh-ide: Initializing SSM..."
+
     LOCAL_USER_ID="$(cat ~/.sm-ssh-owner)"
     echo "sm-ssh-ide: Will use local user ID: $LOCAL_USER_ID"
 
     user_profile_json=$(aws sagemaker describe-user-profile \
-      --domain "$(_print_sm_domain_id)" \
+      --domain-id "$(_print_sm_domain_id)" \
       --user-profile-name "$(_print_sm_user_profile_name)" \
       --output json \
       | tr -d "\n")
     execution_role=$(echo "$user_profile_json" | grep "ExecutionRole" \
       | sed -e 's/^.*"ExecutionRole": \"\([^"]*\)\".*$/\1/')
 
     SSH_SSM_ROLE=$(echo "$execution_role" | sed -e 's/^.*:role\/\(.*\)/\1/')
+
+    if [[ -z "$SSH_SSM_ROLE" ]]; then
+      domain_json=$(aws sagemaker describe-domain \
+        --domain-id "$(_print_sm_domain_id)" \
+        | tr -d "\n")
+      execution_role=$(echo "$domain_json" | grep "ExecutionRole" \
+        | sed -e 's/^.*"ExecutionRole": \"\([^"]*\)\".*$/\1/')
+
+      SSH_SSM_ROLE=$(echo "$execution_role" | sed -e 's/^.*:role\/\(.*\)/\1/')
+    fi
+
+    if [[ -z "$SSH_SSM_ROLE" ]]; then
+      echo "sm-ssh-ide: ERROR: Failed to determine IAM role associated with current user profile"
+    fi
+
     echo "sm-ssh-ide: Will use SSM role: $SSH_SSM_ROLE"
 
     export SSH_SSM_ROLE
     export SSH_OWNER_TAG=$LOCAL_USER_ID
 
     sm-init-ssm
 
+    echo "sm-ssh-ide: SSM initialized. Done"
+
 elif [[ "$1" == "start" ]]; then
+    echo "sm-ssh-ide: Starting services..."
+
     OPTIONS=$(cat /opt/sagemaker-ssh-helper/.sm-ssh-ide-options || echo "")
 
     if [[ -f /tmp/.ssh-ide-local-lock ]]; then
         echo "sm-ssh-ide: Already running on this instance? Call stop first." && exit 1
     fi
 
     touch /tmp/.ssh-ide-local-lock
@@ -220,15 +251,15 @@
 
       tail /tmp/jupyter-notebook.log
 
     else
       echo "sm-ssh-ide: Skipping VNC and Jupyter start"
     fi
 
-    echo "sm-ssh-ide: Started all services"
+    echo "sm-ssh-ide: Started all services. Done"
 
 elif [[ "$1" == "ssm-agent" ]]; then
 
     echo "sm-ssh-ide: Starting SSM agent"
     /usr/bin/amazon-ssm-agent
 
 elif [[ "$1" == "status" ]]; then
@@ -264,14 +295,16 @@
     echo "SageMaker Studio Python version: $($0 get-studio-python-version || echo 'Not found')"
 
     # Should be the same as `jupyter kernelspec list` executed from SageMaker Studio Python
     echo "Jupyter Kernels: $(find "$JUPYTER_PATH" -name 'kernel.json')"
     find "$JUPYTER_PATH" -name 'kernel.json' -print0 | xargs -0 cat
 
 elif [[ "$1" == "stop" ]]; then
+    echo "sm-ssh-ide: Stopping services..."
+
     OPTIONS=$(cat /opt/sagemaker-ssh-helper/.sm-ssh-ide-options || echo "")
 
     echo "sm-ssh-ide: Stopping SSM agent"
     pkill -ef amazon-ssm-agent || echo "sm-ssh-ide: SSM agent already stopped?"
 
     echo "sm-ssh-ide: Stopping SSH service"
     if _is_centos; then
@@ -314,14 +347,14 @@
     
     if [[ -f /tmp/.ssh-ide-local-lock ]]; then
         rm /tmp/.ssh-ide-local-lock
     else
         echo "sm-ssh-ide: Local lock is missing, was not not running on this instance?"
     fi
 
-    echo "sm-ssh-ide: Stopped all services"
+    echo "sm-ssh-ide: Stopped all services. Done"
 
 else
 
     echo "sm-ssh-ide: Unknown command: $1"
 
 fi
```

### Comparing `sagemaker-ssh-helper-2.1.0/sagemaker_ssh_helper/sm-wait` & `sagemaker_ssh_helper-2.2.0/sagemaker_ssh_helper/sm-wait`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 #!/bin/bash
 
+set -e
+set -o pipefail
+
+# Uncomment below option for debugging
+#set -x
+
 SLEEP=$1
 
 if [[ "$SLEEP" == "" ]]; then
     echo "sm-wait: ERROR: missing argument"
     exit 1
 fi
 
@@ -39,15 +45,15 @@
 do
     if [[ -f /tmp/sm-wait-stopped ]]; then
       sleep 2  # let `sm-wait stop` exit successfully before we stop the container
       echo "sm-wait: Successfully stopped. Remove /tmp/sm-wait-stopped to start again."
       exit 0
     fi
     sleep 1
-    SSM_PID=$(pgrep -f amazon-ssm-agent)
+    SSM_PID=$(pgrep -f amazon-ssm-agent || echo "")
     if [[ "$SSM_PID" == "" ]]; then
       AGENT_INFO="SSM Agent has NOT been started yet."
     else
       # TODO: show /var/log/amazon/ssm/*.log in case there are errors
       AGENT_INFO="SSM Agent has been already started."
     fi
```

### Comparing `sagemaker-ssh-helper-2.1.0/sagemaker_ssh_helper/wrapper.py` & `sagemaker_ssh_helper-2.2.0/sagemaker_ssh_helper/wrapper.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 import logging
 import os
 from abc import ABC, abstractmethod
+from datetime import timedelta
 
 import boto3
 import sagemaker
 from sagemaker import Session
 # noinspection PyProtectedMember
 from sagemaker.estimator import _TrainingJob  # need access to sagemaker internals to get last training job name
 from sagemaker.multidatamodel import MultiDataModel
@@ -13,17 +14,19 @@
 from sagemaker.processing import ProcessingJob  # Note: processing job is not marked as protected
 from sagemaker.transformer import Transformer
 # noinspection PyProtectedMember
 from sagemaker.transformer import _TransformJob  # need access to sagemaker internals to get last training job name
 
 from sagemaker.sklearn import SKLearnProcessor
 from sagemaker.spark import PySparkProcessor
+from sagemaker_ssh_helper.sm_ssh import SageMakerSecureShellHelper
 
 from sagemaker_ssh_helper.aws import AWS
 from sagemaker_ssh_helper.detached_sagemaker import DetachedEstimator, DetachedProcessor
+from sagemaker_ssh_helper.ide import SSHIDE, NotebookInstance
 from sagemaker_ssh_helper.log import SSHLog
 from sagemaker_ssh_helper.manager import SSMManager
 from sagemaker_ssh_helper.proxy import SSMProxy
 
 
 class SSHEnvironmentWrapper(ABC):
     logger = logging.getLogger('sagemaker-ssh-helper')
@@ -104,29 +107,41 @@
     def get_instance_ids(self, retry: int = None, timeout_in_sec: int = 900):
         f"""
         :param timeout_in_sec:
         :param retry: (deprecated, use timeout_in_sec) how many retries (each retry is 10 seconds), 360 is for 1 hour
         """
         raise NotImplementedError("Abstract method")
 
+    def get_instance_id(self, retry: int = None, timeout_in_sec: int = 900, index: int = 0):
+        ids = self.get_instance_ids(retry, timeout_in_sec)
+        if not ids:
+            raise ValueError(f"No SSM instances found.")
+        return ids[index]
+
     def retry_deprecated_warning(self, retry, timeout_in_sec):
         if retry:
             self.logger.warning("retry is deprecated, use timeout_in_sec instead")
             timeout_in_sec = retry * 10
         return timeout_in_sec
 
     def start_ssm_connection_and_continue(self, ssh_listen_port: int, retry: int = None,
                                           timeout_in_sec: int = 900,
+                                          timeout: timedelta = timedelta(minutes=15),
                                           extra_args: str = ""):
-        proxy = self.start_ssm_connection(ssh_listen_port, retry, timeout_in_sec, extra_args)
+        if timeout_in_sec != timeout.total_seconds():
+            timeout_in_sec = timeout.total_seconds()
+        proxy = self.start_ssm_connection(ssh_listen_port, retry, timeout_in_sec=timeout_in_sec, extra_args=extra_args)
         proxy.disconnect()
 
     def start_ssm_connection(self, ssh_listen_port: int, retry: int = None,
+                             timeout: timedelta = timedelta(minutes=15),
                              timeout_in_sec: int = 900,
                              extra_args: str = "") -> SSMProxy:
+        if timeout_in_sec != timeout.total_seconds():
+            timeout_in_sec = timeout.total_seconds()
         self.logger.info(f"Starting SSM connection")
         timeout_in_sec = self.retry_deprecated_warning(retry, timeout_in_sec)
         instance_ids = self.get_instance_ids(timeout_in_sec=timeout_in_sec)
         if not instance_ids:
             raise ValueError(f"No SSM instances found. Has the SSM Agent been started? "
                              f"Check the remote logs: {self.get_cloudwatch_url()} "
                              f"AND the remote metadata: {self.get_metadata_url()}")
@@ -157,14 +172,43 @@
     def get_cloudwatch_url(self):
         raise ValueError("Not implemented")
 
     @abstractmethod
     def get_metadata_url(self):
         raise ValueError("Not implemented")
 
+    @abstractmethod
+    def print_ssh_info(self):
+        raise ValueError("Not implemented")
+
+    @classmethod
+    def attach_to_resource(cls, fqdn: str,
+                           domain_id: str = '',
+                           user_profile_name: str = '',
+                           sagemaker_session: Session = None):
+        resource_type = SageMakerSecureShellHelper.fqdn_to_type(fqdn)
+        resource_name = SageMakerSecureShellHelper.fqdn_to_name(fqdn)
+        if resource_type == 'inference':
+            return SSHModelWrapper.attach(resource_name, sagemaker_session)
+        elif resource_type == 'training':
+            return SSHEstimatorWrapper.attach(resource_name, sagemaker_session)
+        elif resource_type == 'processing':
+            return SSHProcessorWrapper.attach(resource_name, sagemaker_session)
+        elif resource_type == 'transform':
+            return SSHTransformerWrapper.attach(resource_name, sagemaker_session)
+        elif resource_type == 'ide':
+            return SSHIDEWrapper.attach(domain_id, user_profile_name, resource_name, sagemaker_session)
+        elif resource_type == 'notebook':
+            return SSHNotebookInstanceWrapper.attach(resource_name, sagemaker_session)
+        else:
+            raise ValueError(f"Don't know how to handle this resource type: {resource_type}")
+
+    def region(self):
+        return self.sagemaker_session.boto_region_name
+
 
 class SSHEstimatorWrapper(SSHEnvironmentWrapper):
     def __init__(self, estimator: sagemaker.estimator.EstimatorBase, ssm_iam_role: str = '',
                  bootstrap_on_start: bool = True, connection_wait_time_seconds: int = 600,
                  ssh_instance_count: int = 2, local_user_id: str = None,
                  log_to_stdout: bool = False):
         super().__init__(ssm_iam_role, bootstrap_on_start, connection_wait_time_seconds,
@@ -225,17 +269,21 @@
         self.logger.info("Stopping training job")
         training_job = self._latest_training_job()
         training_job.stop()
         training_job.wait()
         self.logger.info("Training job is stopped")
 
     @classmethod
-    def create(cls, estimator: sagemaker.estimator.EstimatorBase, connection_wait_time_seconds: int = 600,
+    def create(cls, estimator: sagemaker.estimator.EstimatorBase,
+               connection_wait_time_seconds: int = 600,
+               connection_wait_time: timedelta = timedelta(minutes=10),
                ssh_instance_count: int = 2, local_user_id: str = None,
                log_to_stdout: bool = False) -> SSHEstimatorWrapper:
+        if connection_wait_time_seconds != connection_wait_time.total_seconds():
+            connection_wait_time_seconds = connection_wait_time.total_seconds()
         # noinspection PyProtectedMember
         if estimator._current_job_name:
             raise ValueError(
                 "You should call wrapper.create() before starting a training job with estimator.fit()."
             )
         result = SSHEstimatorWrapper(estimator, connection_wait_time_seconds=connection_wait_time_seconds,
                                      ssh_instance_count=ssh_instance_count, local_user_id=local_user_id,
@@ -267,14 +315,24 @@
 
     @classmethod
     def attach_arn(cls, training_job_arn, sagemaker_session: Session = None) -> SSHEstimatorWrapper:
         if ':training-job/' not in training_job_arn:
             raise ValueError(f"Not a training job ARN: {training_job_arn}")
         return cls.attach(training_job_arn.split('/')[1], sagemaker_session)
 
+    def print_ssh_info(self):
+        print(f"Remote training logs are at {self.get_cloudwatch_url()}")
+        print(f"Training job metadata is at {self.get_metadata_url()}")
+        print(f"To connect over SSM run:\n"
+              f"AWS_DEFAULT_REGION={self.region()} aws ssm start-session --target {self.get_instance_id()}")
+        print(f"To configure local host for SSH run:\n"
+              f"sm-local-configure")
+        print(f"To connect over SSH run:\n"
+              f"AWS_DEFAULT_REGION={self.region()} sm-ssh connect {self.training_job_name()}.training.sagemaker")
+
 
 class SSHModelWrapper(SSHEnvironmentWrapper):
     def __init__(self, model: sagemaker.model.Model,
                  ssm_iam_role: str = '',
                  bootstrap_on_start: bool = True, connection_wait_time_seconds: int = 600):
         super().__init__(ssm_iam_role,
                          bootstrap_on_start, connection_wait_time_seconds, model.sagemaker_session)
@@ -327,14 +385,32 @@
         return self.ssh_log.get_model_metadata_url(self.model.name)
 
     def endpoint_is_online(self):
         describe_result = boto3.client('sagemaker').describe_endpoint(EndpointName=self.model.endpoint_name)
         status = describe_result["EndpointStatus"]
         return status == 'InService'
 
+    @classmethod
+    def attach(cls, endpoint_name: str, sagemaker_session):
+        model = sagemaker.Model(image_uri='', sagemaker_session=sagemaker_session)
+        model.endpoint_name = endpoint_name
+        return SSHModelWrapper(model)
+
+    def print_ssh_info(self):
+        print(f"Remote endpoint logs are at {self.get_cloudwatch_url()}")
+        print(f"Endpoint metadata is at {self.get_metadata_url()}")
+        print(f"Endpoint config metadata is at {self.get_config_metadata_url()}")
+        print(f"Model metadata is at {self.get_model_metadata_url()}")
+        print(f"To connect over SSM run:\n"
+              f"AWS_DEFAULT_REGION={self.region()} aws ssm start-session --target {self.get_instance_id()}")
+        print(f"To configure local host for SSH run:\n"
+              f"sm-local-configure")
+        print(f"To connect over SSH run:\n"
+              f"AWS_DEFAULT_REGION={self.region()} sm-ssh connect {self.model.endpoint_name}.inference.sagemaker")
+
 
 class SSHMultiModelWrapper(SSHEnvironmentWrapper):
     def __init__(self, mdm: sagemaker.multidatamodel.MultiDataModel,
                  ssm_iam_role: str = '',
                  bootstrap_on_start: bool = True, connection_wait_time_seconds: int = 600):
         super().__init__(ssm_iam_role,
                          bootstrap_on_start, connection_wait_time_seconds, mdm.sagemaker_session)
@@ -396,16 +472,38 @@
 
     def get_config_metadata_url(self):
         return self.ssh_log.get_endpoint_config_metadata_url(self.mdm.endpoint_name)
 
     def get_model_metadata_url(self):
         return self.ssh_log.get_model_metadata_url(self.mdm.name)
 
+    def print_ssh_info(self):
+        print(f"Remote multi-model endpoint logs are at {self.get_cloudwatch_url()}")
+        print(f"Multi-model endpoint metadata is at {self.get_metadata_url()}")
+        print(f"Endpoint config metadata is at {self.get_config_metadata_url()}")
+        print(f"Model metadata is at {self.get_model_metadata_url()}")
+        print(f"To connect over SSM run:\n"
+              f"AWS_DEFAULT_REGION={self.region()} aws ssm start-session --target {self.get_instance_id()}")
+        print(f"To configure local host for SSH run:\n"
+              f"sm-local-configure")
+        print(f"To connect over SSH run:\n"
+              f"AWS_DEFAULT_REGION={self.region()} sm-ssh connect {self.mdm.endpoint_name}.inference.sagemaker")
+
 
 class SSHProcessorWrapper(SSHEnvironmentWrapper):
+    def print_ssh_info(self):
+        print(f"Remote processing logs are at {self.get_cloudwatch_url()}")
+        print(f"Processing job metadata is at {self.get_metadata_url()}")
+        print(f"To connect over SSM run:\n"
+              f"AWS_DEFAULT_REGION={self.region()} aws ssm start-session --target {self.get_instance_id()}")
+        print(f"To configure local host for SSH run:\n"
+              f"sm-local-configure")
+        print(f"To connect over SSH run:\n"
+              f"AWS_DEFAULT_REGION={self.region()} sm-ssh connect {self.get_processor_latest_job_name()}.processing.sagemaker")
+
     def __init__(self, processor: sagemaker.processing.Processor,
                  ssm_iam_role: str = '',
                  bootstrap_on_start: bool = True,
                  connection_wait_time_seconds: int = 600):
         super().__init__(ssm_iam_role, bootstrap_on_start, connection_wait_time_seconds,
                          processor.sagemaker_session)
         if self.ssm_iam_role == '':
@@ -516,7 +614,117 @@
         return self.ssh_log.get_transform_cloudwatch_url(self.get_transformer_latest_job_name())
 
     def get_transformer_latest_job_name(self):
         return self.transformer.latest_transform_job.job_name
 
     def get_metadata_url(self):
         return self.ssh_log.get_transform_metadata_url(self.get_transformer_latest_job_name())
+
+    @classmethod
+    def attach(cls, transform_job_name, sagemaker_session: Session = None) -> SSHTransformerWrapper:
+        transformer = sagemaker.transformer.Transformer.attach(transform_job_name)
+        return SSHTransformerWrapper(
+            transformer,
+            SSHModelWrapper.attach(transform_job_name, sagemaker_session or Session())
+        )
+
+    def print_ssh_info(self):
+        print(f"Remote batch transform logs are at {self.get_cloudwatch_url()}")
+        print(f"Batch transform job metadata is at {self.get_metadata_url()}")
+        print(f"To connect over SSM run:\n"
+              f"AWS_DEFAULT_REGION={self.region()} aws ssm start-session --target {self.get_instance_id()}")
+        print(f"To configure local host for SSH run:\n"
+              f"sm-local-configure")
+        print(f"To connect over SSH run:\n"
+              f"AWS_DEFAULT_REGION={self.region()} sm-ssh connect {self.get_transformer_latest_job_name()}.transform.sagemaker")
+
+
+class SSHIDEWrapper(SSHEnvironmentWrapper):
+    def __init__(self,
+                 ssm_iam_role: str,
+                 ide: SSHIDE,
+                 bootstrap_on_start: bool = True,
+                 connection_wait_time_seconds: int = 600,
+                 sagemaker_session: sagemaker.Session = None,
+                 local_user_id: str = None,
+                 log_to_stdout: bool = False):
+        super().__init__(ssm_iam_role, bootstrap_on_start, connection_wait_time_seconds, sagemaker_session,
+                         local_user_id, log_to_stdout)
+        self.app_name = None
+        self.ide = ide
+        self.not_earlier_than_timestamp = 0
+
+    @classmethod
+    def attach(cls, domain_id, user_profile_name, app_name, sagemaker_session: Session = None,
+               not_earlier_than_timestamp: int = 0) -> SSHIDEWrapper:
+        sagemaker_session = sagemaker_session or sagemaker.Session()
+        result = SSHIDEWrapper(
+            '',
+            SSHIDE(domain_id, user_profile_name, sagemaker_session.boto_region_name),
+            connection_wait_time_seconds=0
+        )
+        result.app_name = app_name
+        result.not_earlier_than_timestamp = not_earlier_than_timestamp
+        return result
+
+    def get_instance_ids(self, retry: int = None, timeout_in_sec: int = 900):
+        return self.ide.get_kernel_instance_ids(self.app_name, timeout_in_sec=timeout_in_sec,
+                                                not_earlier_than_timestamp=self.not_earlier_than_timestamp)
+
+    def get_cloudwatch_url(self):
+        return self.ide.get_cloudwatch_url(self.app_name)
+
+    def get_metadata_url(self):
+        return self.ide.get_user_metadata_url()
+
+    def print_ssh_info(self):
+        print(f"SageMaker Studio logs are at {self.get_cloudwatch_url()}")
+        print(f"SageMaker Studio metadata is at {self.get_metadata_url()}")
+        print(f"To connect over SSM run:\n"
+              f"AWS_DEFAULT_REGION={self.region()} aws ssm start-session --target {self.get_instance_id()}")
+        print(f"To configure local host for SSH run:\n"
+              f"sm-local-configure")
+        print(f"To connect over SSH run:\n"
+              f"AWS_DEFAULT_REGION={self.region()} sm-ssh connect {self.app_name}.studio.sagemaker")
+
+
+class SSHNotebookInstanceWrapper(SSHEnvironmentWrapper):
+    def __init__(self,
+                 ssm_iam_role: str,
+                 notebook_instance: NotebookInstance,
+                 bootstrap_on_start: bool = True,
+                 connection_wait_time_seconds: int = 600,
+                 sagemaker_session: sagemaker.Session = None,
+                 local_user_id: str = None,
+                 log_to_stdout: bool = False):
+        super().__init__(ssm_iam_role, bootstrap_on_start, connection_wait_time_seconds, sagemaker_session,
+                         local_user_id, log_to_stdout)
+        self.notebook_instance = notebook_instance
+
+    def get_instance_ids(self, retry: int = None, timeout_in_sec: int = 900):
+        return self.notebook_instance.get_instance_ids()
+
+    def get_cloudwatch_url(self):
+        return self.notebook_instance.get_cloudwatch_url()
+
+    def get_metadata_url(self):
+        return self.notebook_instance.get_metadata_url()
+
+    @classmethod
+    def attach(cls, notebook_name, sagemaker_session):
+        sagemaker_session = sagemaker_session or sagemaker.Session()
+        result = SSHNotebookInstanceWrapper(
+            '',
+            NotebookInstance(notebook_name, sagemaker_session.boto_region_name),
+            connection_wait_time_seconds=0
+        )
+        return result
+
+    def print_ssh_info(self):
+        print(f"SageMaker Notebook Instance logs are at {self.get_cloudwatch_url()}")
+        print(f"SageMaker Notebook Instance metadata is at {self.get_metadata_url()}")
+        print(f"To connect over SSM run:\n"
+              f"AWS_DEFAULT_REGION={self.region()} aws ssm start-session --target {self.get_instance_id()}")
+        print(f"To configure local host for SSH run:\n"
+              f"sm-local-configure")
+        print(f"To connect over SSH run:\n"
+              f"AWS_DEFAULT_REGION={self.region()} sm-ssh connect {self.notebook_instance.notebook_name}.notebook.sagemaker")
```

### Comparing `sagemaker-ssh-helper-2.1.0/sagemaker_ssh_helper.egg-info/SOURCES.txt` & `sagemaker_ssh_helper-2.2.0/sagemaker_ssh_helper.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 LICENSE
 README.md
+SageMaker_SSH_IDE.ipynb
+SageMaker_SSH_Notebook.ipynb
 setup.py
+sagemaker_ssh_helper/VERSION
 sagemaker_ssh_helper/__init__.py
 sagemaker_ssh_helper/aws.py
+sagemaker_ssh_helper/browser_automation.py
 sagemaker_ssh_helper/deregister_old_instances_from_ssm.py
 sagemaker_ssh_helper/detached_sagemaker.py
 sagemaker_ssh_helper/env.py
 sagemaker_ssh_helper/ide.py
+sagemaker_ssh_helper/interactive_sagemaker.py
 sagemaker_ssh_helper/log.py
 sagemaker_ssh_helper/manager.py
 sagemaker_ssh_helper/proxy.py
 sagemaker_ssh_helper/sm-connect-ssh-proxy
 sagemaker_ssh_helper/sm-helper-functions
 sagemaker_ssh_helper/sm-init-ssm
 sagemaker_ssh_helper/sm-local-configure
@@ -21,18 +26,20 @@
 sagemaker_ssh_helper/sm-local-ssh-training
 sagemaker_ssh_helper/sm-local-ssh-transform
 sagemaker_ssh_helper/sm-local-start-ssh
 sagemaker_ssh_helper/sm-save-env
 sagemaker_ssh_helper/sm-setup-ssh
 sagemaker_ssh_helper/sm-ssh-ide
 sagemaker_ssh_helper/sm-wait
+sagemaker_ssh_helper/sm_ssh.py
 sagemaker_ssh_helper/wrapper.py
 sagemaker_ssh_helper.egg-info/PKG-INFO
 sagemaker_ssh_helper.egg-info/SOURCES.txt
 sagemaker_ssh_helper.egg-info/dependency_links.txt
+sagemaker_ssh_helper.egg-info/entry_points.txt
 sagemaker_ssh_helper.egg-info/requires.txt
 sagemaker_ssh_helper.egg-info/top_level.txt
 sagemaker_ssh_helper/cdk/__init__.py
 sagemaker_ssh_helper/cdk/advanced_tier_app.py
 sagemaker_ssh_helper/cdk/iam_ssm_app.py
 sagemaker_ssh_helper/cdk/low_gpu_lambda_app.py
 sagemaker_ssh_helper/cdk/tests_app.py
@@ -43,25 +50,29 @@
 sagemaker_ssh_helper/cdk/iam_ssm/ssm_advanced_tier_stack.py
 sagemaker_ssh_helper/cdk/iam_ssm/trust_relationship_lambda.py
 sagemaker_ssh_helper/cdk/low_gpu/__init__.py
 sagemaker_ssh_helper/cdk/low_gpu/low_gpu_lambda.py
 sagemaker_ssh_helper/cdk/low_gpu/low_gpu_lambda_stack.py
 sagemaker_ssh_helper/cdk/tests/__init__.py
 sagemaker_ssh_helper/cdk/tests/unit/__init__.py
+sagemaker_ssh_helper/js/__init__.py
+sagemaker_ssh_helper/js/drop_studio_file.js
 tests/test_attach.py
 tests/test_batch_inference.py
 tests/test_clean_core.py
+tests/test_cli.py
 tests/test_compiler.py
 tests/test_deregister_instances.py
 tests/test_distributed.py
 tests/test_end_to_end.py
 tests/test_environment.py
 tests/test_frameworks.py
 tests/test_functions.py
 tests/test_hpo.py
 tests/test_ide.py
 tests/test_inference_registry.py
 tests/test_local.py
 tests/test_manual.py
+tests/test_model_repack.py
 tests/test_ssm_manager.py
 tests/test_util.py
 tests/test_validation.py
```

### Comparing `sagemaker-ssh-helper-2.1.0/sagemaker_ssh_helper.egg-info/requires.txt` & `sagemaker_ssh_helper-2.2.0/sagemaker_ssh_helper.egg-info/requires.txt`

 * *Files 14% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 flake8
 mock
 pydocstyle
 pytest
 pytest-cov
 pytest-html
 pytest-profiling
+pytest-monitor
 bandit
 aws-cdk-lib==2.64.0
 constructs<11.0.0,>=10.0.0
 sagemaker-studio-image-build
 sagemaker-training
 selenium
-accelerate[sagemaker]
+accelerate[sagemaker]<0.29
```

### Comparing `sagemaker-ssh-helper-2.1.0/setup.py` & `sagemaker_ssh_helper-2.2.0/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+"""
+Copyright Amazon.com, Inc. or its affiliates. All Rights Reserved.
+SPDX-License-Identifier: MIT-0
+"""
+
+import os
+from pathlib import Path
+
 import setuptools
 
 required_packages = [
     "sagemaker>=2.145.0",
     "psutil",
 ]
 
@@ -16,21 +24,22 @@
         "flake8",
         "mock",
         "pydocstyle",
         "pytest",
         "pytest-cov",
         "pytest-html",
         "pytest-profiling",
+        "pytest-monitor",
         "bandit",
         "aws-cdk-lib==2.64.0",
         "constructs>=10.0.0,<11.0.0",
         "sagemaker-studio-image-build",
         "sagemaker-training",
         "selenium",
-        "accelerate[sagemaker]",
+        "accelerate[sagemaker]<0.29",  # TODO: see https://github.com/huggingface/accelerate/issues/2744
     ],
     "dev": [
         "sagemaker-pytorch-training",
         "sagemaker-pytorch-inference",
         "torch-model-archiver",
         "tox",
         "wheel",
@@ -46,29 +55,40 @@
         #   run 'cd djl-serving/engines/python/setup/ && pip install .'
     ],
     "dev-macos": [
         "tensorflow-macos==2.9.2",
         "numpy==1.22.4"
     ]
 }
+
+
+def read_version():
+    return open(os.path.join(os.path.dirname(__file__), "sagemaker_ssh_helper", "VERSION")).read()
+
+
 setuptools.setup(
     name='sagemaker-ssh-helper',
-    version='2.1.0',
+    version=read_version(),
     author="Amazon Web Services",
     description="A helper library to connect into Amazon SageMaker with AWS Systems Manager and SSH (Secure Shell)",
     long_description="SageMaker SSH Helper is a library that allows you to \"SSH into SageMaker\", "
                      "i.e., securely connect to Amazon SageMaker training jobs, processing jobs, "
                      "and realtime inference endpoints as well as SageMaker Studio notebook containers "
                      "for fast interactive experimentation, remote debugging, and advanced troubleshooting."
                      "\n\n"
                      "For the documentation, see the repo [https://github.com/aws-samples/sagemaker-ssh-helper/]"
                      "(https://github.com/aws-samples/sagemaker-ssh-helper/).",
     long_description_content_type='text/markdown',
     url='https://github.com/aws-samples/sagemaker-ssh-helper',
     packages=setuptools.find_packages(),
+    data_files=[
+        ('notebooks', [str(Path('SageMaker_SSH_IDE.ipynb')), str(Path('SageMaker_SSH_Notebook.ipynb'))]),
+        ('js', [str(Path('./sagemaker_ssh_helper/js/drop_studio_file.js'))]),
+        ('version', [str(Path('sagemaker_ssh_helper/VERSION'))])
+    ],
     include_package_data=True,
     scripts=['sagemaker_ssh_helper/sm-helper-functions',
              'sagemaker_ssh_helper/sm-connect-ssh-proxy',
              'sagemaker_ssh_helper/sm-wait',
              'sagemaker_ssh_helper/sm-local-start-ssh',
              'sagemaker_ssh_helper/sm-local-ssh-ide',
              'sagemaker_ssh_helper/sm-local-ssh-notebook',
@@ -78,14 +98,20 @@
              'sagemaker_ssh_helper/sm-local-ssh-processing',
              'sagemaker_ssh_helper/sm-local-configure',
              'sagemaker_ssh_helper/sm-ssh-ide',
              'sagemaker_ssh_helper/sm-save-env',
              'sagemaker_ssh_helper/sm-init-ssm',
              'sagemaker_ssh_helper/sm-setup-ssh',
              ],
+    entry_points={
+        "console_scripts": [
+            "sm-ssh=sagemaker_ssh_helper.sm_ssh:main",
+            "sm-ssh-deregister-instances=sagemaker_ssh_helper.deregister_old_instances_from_ssm:main"
+        ]
+    },
     python_requires=">=3.7",
     install_requires=required_packages,
     extras_require=extras,
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "Natural Language :: English",
@@ -93,10 +119,11 @@
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
-        "Programming Language :: Python :: 3.12",
+        # "Programming Language :: Python :: 3.12",  # TODO: doesn't work on Windows, SageMaker Python SDK supports 3.10
+        # "Programming Language :: Python :: 3.13",  # TODO: not tested yet, test with tox
     ]
 )
```

### Comparing `sagemaker-ssh-helper-2.1.0/tests/test_attach.py` & `sagemaker_ssh_helper-2.2.0/tests/test_attach.py`

 * *Files 17% similar despite different names*

```diff
@@ -29,17 +29,15 @@
     _ = SSHEstimatorWrapper.create(estimator, connection_wait_time_seconds=600)
 
     estimator.fit(wait=False)
 
     job: _TrainingJob = estimator.latest_training_job
     ssh_wrapper = SSHEstimatorWrapper.attach(job.name)
 
-    logging.info(f"To connect over SSH run: sm-local-ssh-training connect {ssh_wrapper.training_job_name()}")
-    instance_ids = ssh_wrapper.get_instance_ids()
-    logging.info(f"To connect over SSM run: aws ssm start-session --target {instance_ids[0]}")
+    ssh_wrapper.print_ssh_info()
 
     ssh_wrapper.start_ssm_connection_and_continue(11022)
 
     ssh_wrapper.wait_training_job()
 
     assert estimator.model_data.find("model.tar.gz") != -1
```

### Comparing `sagemaker-ssh-helper-2.1.0/tests/test_batch_inference.py` & `sagemaker_ssh_helper-2.2.0/tests/test_batch_inference.py`

 * *Files 7% similar despite different names*

```diff
@@ -94,12 +94,13 @@
                           job_name=transform_job_name,
                           content_type='text/csv',
                           split_type='Line',
                           join_source="Input",
                           wait=False)
 
     ssh_transformer_wrapper.start_ssm_connection_and_continue(16022)
+    ssh_transformer_wrapper.print_ssh_info()
     ssh_transformer_wrapper.wait_transform_job()
 
     test_util._cleanup_dir("./output", recreate=True)
     sagemaker_session.download_data(path='output', bucket=bucket,
                                     key_prefix='batch-transform/output')
```

### Comparing `sagemaker-ssh-helper-2.1.0/tests/test_clean_core.py` & `sagemaker_ssh_helper-2.2.0/tests/test_clean_core.py`

 * *Files identical despite different names*

### Comparing `sagemaker-ssh-helper-2.1.0/tests/test_compiler.py` & `sagemaker_ssh_helper-2.2.0/tests/test_compiler.py`

 * *Files identical despite different names*

### Comparing `sagemaker-ssh-helper-2.1.0/tests/test_deregister_instances.py` & `sagemaker_ssh_helper-2.2.0/tests/test_deregister_instances.py`

 * *Files identical despite different names*

### Comparing `sagemaker-ssh-helper-2.1.0/tests/test_distributed.py` & `sagemaker_ssh_helper-2.2.0/tests/test_distributed.py`

 * *Files identical despite different names*

### Comparing `sagemaker-ssh-helper-2.1.0/tests/test_end_to_end.py` & `sagemaker_ssh_helper-2.2.0/tests/test_end_to_end.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,19 +41,20 @@
         instance_count=1,
         instance_type='ml.m5.xlarge',
         max_run=int(timedelta(minutes=15).total_seconds()),
         keep_alive_period_in_seconds=1800,
         container_log_level=logging.INFO
     )
 
-    ssh_wrapper = SSHEstimatorWrapper.create(estimator, connection_wait_time_seconds=600)
+    ssh_wrapper = SSHEstimatorWrapper.create(estimator, connection_wait_time=timedelta(minutes=10))
 
     estimator.fit(wait=False)
 
-    ssh_wrapper.start_ssm_connection_and_continue(11022)
+    ssh_wrapper.start_ssm_connection_and_continue(11022, timeout=timedelta(minutes=5))
+    ssh_wrapper.print_ssh_info()
 
     ssh_wrapper.wait_training_job()
 
     assert estimator.model_data.find("model.tar.gz") != -1
 
 
 def test_train_pycharm_debug_e2e():
@@ -65,15 +66,15 @@
                         py_version='py38',
                         instance_count=1,
                         instance_type='ml.m5.xlarge',
                         max_run=int(timedelta(minutes=15).total_seconds()),
                         keep_alive_period_in_seconds=1800,
                         container_log_level=logging.INFO)
 
-    ssh_wrapper = SSHEstimatorWrapper.create(estimator, connection_wait_time_seconds=600)
+    ssh_wrapper = SSHEstimatorWrapper.create(estimator, connection_wait_time=timedelta(minutes=10))
 
     estimator.fit(wait=False)
 
     bucket = queue.Queue()
 
     def pycharm_debug_server_mock():
         server_sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
@@ -98,15 +99,15 @@
 
     server_thread = threading.Thread(target=pycharm_debug_server_mock)
     server_thread.start()
 
     time.sleep(2)  # wait a little to get server thread started
 
     ssm_proxy = ssh_wrapper.start_ssm_connection(
-        11022, timeout_in_sec=600,
+        11022, timeout=timedelta(minutes=5),
         extra_args="-R localhost:12345:localhost:12345"
     )
 
     logger.info("Waiting for pydevd to connect")
     server_thread.join()
 
     ssm_proxy.disconnect()
@@ -126,29 +127,31 @@
                         py_version='py38',
                         instance_count=1,
                         instance_type='ml.m5.xlarge',
                         max_run=int(timedelta(minutes=15).total_seconds()),
                         keep_alive_period_in_seconds=1800,
                         container_log_level=logging.INFO)
 
-    ssh_wrapper = SSHEstimatorWrapper.create(estimator, connection_wait_time_seconds=0)
+    ssh_wrapper = SSHEstimatorWrapper.create(estimator, connection_wait_time=timedelta(seconds=0))
 
     estimator.fit(wait=False)
 
-    proxy = ssh_wrapper.start_ssm_connection(11022, 60)
+    proxy = ssh_wrapper.start_ssm_connection(11022, timeout=timedelta(minutes=5))
 
     # Do something on the remote node...
 
     proxy.disconnect()
 
     ssh_wrapper.stop_training_job()
 
 
 # noinspection DuplicatedCode
-def test_debugger_stop_gpu(request):
+@pytest.mark.skipif(os.getenv('PYTEST_IGNORE_SKIPS', "false") == "false",
+                    reason="Temp issues with the profiler - D96111855")
+def test_low_gpu_debugger_stop(request):
     sns_notification_topic_arn = request.config.getini('sns_notification_topic_arn')
 
     from sagemaker.debugger import ProfilerRule, rule_configs, ProfilerConfig
 
     profiler_config = ProfilerConfig(
         system_monitor_interval_millis=100,  # grab metrics 10 times per second
     )
@@ -174,15 +177,15 @@
         max_run=int(timedelta(minutes=15).total_seconds()),
         keep_alive_period_in_seconds=int(timedelta(minutes=30).total_seconds()),
         container_log_level=logging.INFO,
         profiler_config=profiler_config,
         rules=rules
     )
 
-    ssh_wrapper = SSHEstimatorWrapper.create(estimator, connection_wait_time_seconds=0)
+    ssh_wrapper = SSHEstimatorWrapper.create(estimator, connection_wait_time=timedelta(seconds=0))
 
     estimator.fit(wait=False)
 
     status = ssh_wrapper.wait_training_job_with_status()
     assert status == 'Completed', 'The job should not be stopped by max_run limit'
 
     from sagemaker_ssh_helper.cdk.low_gpu import low_gpu_lambda
@@ -230,14 +233,15 @@
         instance_type='ml.m5.xlarge',
         endpoint_name=endpoint_name,
         wait=True
     )
 
     try:
         ssh_wrapper.start_ssm_connection_and_continue(12022)
+        ssh_wrapper.print_ssh_info()
 
         time.sleep(60)  # Cold start latency to prevent prediction time out
 
         predictor.serializer = JSONSerializer()
         predictor.deserializer = JSONDeserializer()
 
         predicted_value = predictor.predict(data=[1])
@@ -313,14 +317,15 @@
         predicted_value = predictor.predict(data=[1], target_model="model_1.tar.gz")
         assert predicted_value == [43]
         predicted_value = predictor.predict(data=[1], target_model="model_2.tar.gz")
         assert predicted_value == [20043]
 
         # Note: in MME the models are lazy loaded, so SSH helper will start upon the first prediction request
         ssh_wrapper.start_ssm_connection_and_continue(13022)
+        ssh_wrapper.print_ssh_info()
 
     finally:
         if predictor:
             predictor.delete_endpoint(delete_endpoint_config=False)
 
 
 # noinspection DuplicatedCode
@@ -417,14 +422,15 @@
         submit_app="source_dir/processing/process.py",
         inputs=[ssh_wrapper.augmented_input()],
         logs=True,
         wait=False
     )
 
     ssh_wrapper.start_ssm_connection_and_continue(14022)
+    ssh_wrapper.print_ssh_info()
 
     ssh_wrapper.wait_processing_job()
 
 
 def test_processing_framework_e2e():
     torch_processor = PyTorchProcessor(
         base_job_name='ssh-pytorch-processing',
@@ -444,14 +450,15 @@
         dependencies=[SSHProcessorWrapper.dependency_dir()],
         code="process_framework.py",
         logs=True,
         wait=False
     )
 
     ssh_wrapper.start_ssm_connection_and_continue(15022)
+    ssh_wrapper.print_ssh_info()
 
     ssh_wrapper.wait_processing_job()
 
 
 def test_train_with_bucket_override():
     account_id = boto3.client('sts').get_caller_identity().get('Account')
     custom_bucket_name = f'sagemaker-custom-bucket-{account_id}'
```

### Comparing `sagemaker-ssh-helper-2.1.0/tests/test_environment.py` & `sagemaker_ssh_helper-2.2.0/tests/test_environment.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,14 +65,14 @@
 
     ssh_wrapper.wait_processing_job()
 
 
 def test_caller_script():
     from sagemaker_ssh_helper.env import get_caller_script_name
     assert get_caller_script_name() == 'test_environment.py'
-    assert get_caller_script_name(2) == 'python.py'
+    assert get_caller_script_name(2) == 'pytest_monitor.py'
 
 
 def test_aws_config():
     output = subprocess.check_output("aws configure list".split(" ")).decode("latin1")
     logging.info(f"AWS config:\n{output}")
     logging.info(sagemaker.Session().default_bucket())
```

### Comparing `sagemaker-ssh-helper-2.1.0/tests/test_frameworks.py` & `sagemaker_ssh_helper-2.2.0/tests/test_frameworks.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,32 +74,32 @@
     logging.info("Starting training")
 
     from sagemaker.huggingface import HuggingFace
     # noinspection PyCompatibility
     estimator = HuggingFace(
         entry_point=(p := Path('source_dir/training_clean/train_clean.py')).name,
         source_dir=str(p.parents[0]),
-        pytorch_version='1.10',
-        transformers_version='4.17',
-        py_version='py38',
+        pytorch_version='1.13',
+        transformers_version='4.26',
+        py_version='py39',
         instance_count=1,
         instance_type='ml.g4dn.xlarge',
         max_run=int(timedelta(minutes=15).total_seconds()),
         keep_alive_period_in_seconds=1800,
         container_log_level=logging.INFO
     )
 
     estimator.fit()
     logging.info("Finished training")
 
     logging.info("Starting repacking model")
 
     # noinspection PyCompatibility
     model = estimator.create_model(
-        entry_point=(p := Path('source_dir/inference/inference_hf.py')).name,
+        entry_point=(p := Path('source_dir/inference/inference_ssh.py')).name,
         source_dir=str(p.parents[0])
     )
 
     model.prepare_container_def(instance_type='ml.g4dn.xlarge')
     repacked_model_data = model.repacked_model_data
 
     logging.info("Finished repacking model")
@@ -108,17 +108,17 @@
 
     from sagemaker.huggingface import HuggingFaceModel
 
     model = HuggingFaceModel(
         model_data=repacked_model_data,
         entry_point=model.entry_point,  # TODO: does it repack the entry point? What if I also use source_dir?
         role=estimator.role,  # TODO: should take the default
-        transformers_version='4.17.0',
-        pytorch_version='1.10.2',
-        py_version='py38',
+        pytorch_version='1.13',
+        transformers_version='4.26',
+        py_version='py39',
         dependencies=[SSHModelWrapper.dependency_dir()],  # NOTE: model will be repacked again with dependencies
     )
 
     ssh_wrapper = SSHModelWrapper.create(model, connection_wait_time_seconds=0)
 
     endpoint_name = name_from_base('ssh-hf-inference')
 
@@ -453,15 +453,15 @@
     estimator.fit()
     logging.info("Finished training")
 
     assert estimator.model_data.find("model.tar.gz") != -1
 
 
 @pytest.mark.skipif(os.getenv('PYTEST_IGNORE_SKIPS', "false") == "false",
-                    reason="Temp issues with the dependencies in the container")
+                    reason="Temp issues with the dependencies in the container - D89685473")
 def test_train_sklearn_ssh():
     logging.info("Starting training")
 
     from sagemaker.sklearn import SKLearn
     estimator = SKLearn(entry_point='train.py',
                         source_dir='source_dir/training/',
                         dependencies=[SSHEstimatorWrapper.dependency_dir()],
@@ -499,15 +499,15 @@
     estimator.fit()
     logging.info("Finished training")
 
     assert estimator.model_data.find("model.tar.gz") != -1
 
 
 @pytest.mark.skipif(os.getenv('PYTEST_IGNORE_SKIPS', "false") == "false",
-                    reason="Temp issues with the dependencies in the container")
+                    reason="Temp issues with the dependencies in the container - D89685473")
 def test_train_xgboost_ssh():
     logging.info("Starting training")
 
     from sagemaker.xgboost import XGBoost
     estimator = XGBoost(entry_point='train.py',
                         source_dir='source_dir/training/',
                         dependencies=[SSHEstimatorWrapper.dependency_dir()],
@@ -818,14 +818,15 @@
             {"inputs": "What is the answer to life, the universe, and everything? The answer: ",
              "parameters": {"max_length": 50, "temperature": 0.5}}
         )
         logging.info(f"GPT-J 6B prediction result: {result}")
         assert "'generated_text': 'What is" in str(result) or "'generated_text': \"What is" in str(result)
 
     except Exception as e:
+        logging.error("Exception occurred during the test. Cleaning up the resources.")
         if predictor:
             try:
                 predictor.delete_endpoint(delete_endpoint_config=False)
             except ClientError as delete_e:
                 logging.error(f"Test failed. Additionally, failed to cleanup: {delete_e.response['Error']['Message']}",
                               exc_info=e)
                 raise
@@ -837,26 +838,28 @@
             logging.error(f"Failed to cleanup", exc_info=delete_e)
             raise
 
 
 # noinspection DuplicatedCode
 @mock.patch.object(sys, 'argv', ['launch', 'source_dir/training_clean/train_clean.py'])
 def test_accelerate_training_clean():
-    """
+    f"""
     See https://huggingface.co/docs/accelerate/usage_guides/sagemaker .
 
     Below code is equal to executing the following command:
 
     accelerate launch ./source_dir/training_clean/train_clean.py
 
     See: https://github.com/huggingface/accelerate/blob/main/src/accelerate/commands/launch.py#L787-L804
       and https://github.com/huggingface/accelerate/blob/main/src/accelerate/utils/launch.py#L383-L491 .
 
+    See also: {Path("generate_accelerate_config.sh")} .
+
     """
-    import accelerate.commands.launch as launch
+    import accelerate.commands.launch as launch  # This is identical to using `accelerate launch` from command line
     import accelerate.utils.launch as utils_launch
     parser = launch.launch_command_parser()
     args = parser.parse_args()
     args, sagemaker_config, mp_from_config_flag = launch._validate_launch_command(args)
     if args.module or args.no_python:
         raise ValueError(
             "SageMaker requires a python training script file and cannot be used with --module or --no_python"
@@ -871,14 +874,17 @@
 
     logging.info(f"You can find your model data at: {huggingface_estimator.model_data}")
 
 
 # noinspection DuplicatedCode
 @mock.patch.object(sys, 'argv', ['launch', 'source_dir/training/train.py'])
 def test_accelerate_training_ssh():
+    f"""
+    See: {Path("generate_accelerate_config.sh")} .
+    """
     import accelerate.commands.launch as launch
     import accelerate.utils.launch as utils_launch
     parser = launch.launch_command_parser()
     args = parser.parse_args()
     args, sagemaker_config, mp_from_config_flag = launch._validate_launch_command(args)
     if args.module or args.no_python:
         raise ValueError(
```

### Comparing `sagemaker-ssh-helper-2.1.0/tests/test_hpo.py` & `sagemaker_ssh_helper-2.2.0/tests/test_hpo.py`

 * *Files identical despite different names*

### Comparing `sagemaker-ssh-helper-2.1.0/tests/test_ide.py` & `sagemaker_ssh_helper-2.2.0/tests/test_ide.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,71 +1,68 @@
 import logging
 import os
 import re
 import subprocess
 import time
+from datetime import timedelta
 from pathlib import Path
 
 import pytest
-from selenium.webdriver.support.wait import WebDriverWait
+from selenium.webdriver.firefox.options import Options
 
+from sagemaker_ssh_helper.browser_automation import JupyterNotebook, SageMakerStudioAutomation
 from sagemaker_ssh_helper.ide import SSHIDE
 from sagemaker_ssh_helper.manager import SSMManager
 from sagemaker_ssh_helper.proxy import SSMProxy
 
 from selenium import webdriver
 
-from selenium.webdriver.common.by import By
-
-import boto3
-
-from selenium.webdriver.support import expected_conditions as EC
+from sagemaker_ssh_helper.wrapper import SSHIDEWrapper
 
 logger = logging.getLogger('sagemaker-ssh-helper:test_ide')
 
 
-# TODO: add a test for typing SageMaker Studio terminal commands - check conda env is activated (Selenium?)
+# TODO: add a test for typing SageMaker Studio terminal commands - check conda env is activated
 
 # See https://docs.aws.amazon.com/sagemaker/latest/dg/notebooks-available-images.html .
 
 SSH_TEST_IMAGES = [
     # 0 - Data Science
     ('test-data-science', 'ssh-test-ds1-cpu',
-     'datascience-1.0', 'ml.m5.large', 'Python 3.7.10'),
+     'datascience-1.0', 'ml.m5.large', '** Deprecated **'),
     # 1 - Data Science 2.0
     ('test-data-science', 'ssh-test-ds2-cpu',
-     'sagemaker-data-science-38', 'ml.m5.large', 'Python 3.8.13'),
+     'sagemaker-data-science-38', 'ml.m5.large', 'Python 3.8.18'),
     # 2 - Data Science 3.0
     ('test-data-science', 'ssh-test-ds3-cpu',
      'sagemaker-data-science-310-v1', 'ml.m5.large', 'Python 3.10.6'),
 
     # 3 - Base Python 2.0
     ('test-base-python', 'ssh-test-bp2-cpu',
      'sagemaker-base-python-38', 'ml.m5.large', 'Python 3.8.12'),
     # 4 - Base Python 3.0
     ('test-base-python', 'ssh-test-bp3-cpu',
      'sagemaker-base-python-310-v1', 'ml.m5.large', 'Python 3.10.8'),
 
-    # 5 - SparkMagic
+    # 5 - SparkMagic (deprecated)
     ('test-spark', 'ssh-test-magic-cpu',
-     'sagemaker-sparkmagic', 'ml.m5.large', 'Python 3.7.10'),
+     'sagemaker-sparkmagic', 'ml.m5.large', '** Deprecated **'),
     # 6 - SparkAnalytics 1.0
     ('test-spark', 'ssh-test-analytics-cpu',
-     'sagemaker-sparkanalytics-v1', 'ml.m5.large', 'Python 3.8.13'),
+     'sagemaker-sparkanalytics-v1', 'ml.m5.large', 'Python 3.8.13'),  # noqa
     # 7 - SparkAnalytics 2.0
     ('test-spark', 'ssh-test-analytics2-cpu',
-     'sagemaker-sparkanalytics-310-v1', 'ml.m5.large', 'Python 3.10.6'),
+     'sagemaker-sparkanalytics-310-v1', 'ml.m5.large', 'Python 3.10.6'),  # noqa
 
     # 8 - MXNet 1.9 Python 3.8 CPU Optimized
     ('test-mxnet', 'ssh-test-mx19-cpu',
-     'mxnet-1.9-cpu-py38-ubuntu20.04-sagemaker-v1.0', 'ml.m5.large', 'Python 3.8.10'),
+     'mxnet-1.9-cpu-py38-ubuntu20.04-sagemaker-v1.0', 'ml.m5.large', '** Deprecated **'),
     # 9 - MXNet 1.9 Python 3.8 GPU Optimized
-    # TODO: https://developer.nvidia.com/blog/updating-the-cuda-linux-gpg-repository-key/
-    # ('test-mxnet', 'ssh-test-mx19-gpu',
-    #  'mxnet-1.9-gpu-py38-cu112-ubuntu20.04-sagemaker-v1.0', 'ml.g4dn.xlarge', 'Python 3'),
+    ('test-mxnet', 'ssh-test-mx19-gpu',
+     'mxnet-1.9-gpu-py38-cu112-ubuntu20.04-sagemaker-v1.0', 'ml.g4dn.xlarge', '** Deprecated **'),
 
     # 10 - PyTorch 1.12 Python 3.8 CPU Optimized
     ('test-pytorch', 'ssh-test-pt112-cpu',
      'pytorch-1.12-cpu-py38', 'ml.m5.large', 'Python 3.8.16'),
     # 11 - PyTorch 1.12 Python 3.8 GPU Optimized
     ('test-pytorch', 'ssh-test-pt112-gpu',
      'pytorch-1.12-gpu-py38', 'ml.g4dn.xlarge', 'Python 3.8.16'),
@@ -80,48 +77,53 @@
     ('test-tensorflow', 'ssh-test-tf211-cpu',
      'tensorflow-2.11.0-cpu-py39-ubuntu20.04-sagemaker-v1.1', 'ml.m5.large', 'Python 3.9.10'),
     # 15 - TensorFlow 2.11.0 Python 3.9 GPU Optimized
     ('test-tensorflow', 'ssh-test-tf211-gpu',
      'tensorflow-2.11.0-gpu-py39-cu112-ubuntu20.04-sagemaker-v1.1', 'ml.g4dn.xlarge', 'Python 3.9.10'),
     # 16 - TensorFlow 2.12.0 Python 3.10 CPU Optimized
     ('test-tensorflow', 'ssh-test-tf212-cpu',
-     'tensorflow-2.12.0-cpu-py310-ubuntu20.04-sagemaker-v1', 'ml.m5.large', 'Python 3.10.10'),
+     'tensorflow-2.12.0-cpu-py310-ubuntu20.04-sagemaker-v1.0', 'ml.m5.large', 'Python 3.10.10'),
     # 17 - TensorFlow 2.12.0 Python 3.10 GPU Optimized
     ('test-tensorflow', 'ssh-test-tf212-gpu',
-     'tensorflow-2.12.0-gpu-py310-cu118-ubuntu20.04-sagemaker-v1', 'ml.g4dn.xlarge', 'Python 3.10.10'),
+     'tensorflow-2.12.0-gpu-py310-cu118-ubuntu20.04-sagemaker-v1.0', 'ml.g4dn.xlarge', 'Python 3.10.10'),
+
+    # 18 - SageMaker Distribution v0 CPU - TODO
+
+    # 19 - SageMaker Distribution v0 GPU - TODO
 ]
 
 
 @pytest.mark.parametrize('instances', SSH_TEST_IMAGES)
 def test_sagemaker_studio(instances, request):
     user, app_name, image_name, instance_type, expected_version = instances
 
+    if 'Deprecated' in expected_version:
+        return
+
     ide = SSHIDE(request.config.getini('sagemaker_studio_domain'), user)
 
-    # TODO:
-    #  os.env["LOCAL_USER_ID"] -> ./.sm-ssh-owner
-    #  ide.upload_UI("./.sm-ssh-owner", "/.sm-ssh-owner") - cannot upload dot file in UI?
+    time_stamp_before_app_created = int(time.time())
 
     ide.create_ssh_kernel_app(
         app_name,
         image_name_or_arn=image_name,
         instance_type=instance_type,
         ssh_lifecycle_config='sagemaker-ssh-helper-dev',
         recreate=True
     )
 
-    # Need to wait here, otherwise it will try to connect to an old offline instance
-    # TODO: more robust mechanism?
-    time.sleep(60)
+    time.sleep(30)  # Give time for CPU load to normalize
 
-    studio_ids = ide.get_kernel_instance_ids(app_name, timeout_in_sec=300)
-    studio_id = studio_ids[0]
+    ide_wrapper = SSHIDEWrapper.attach(
+        ide.domain_id, ide.user, app_name,
+        not_earlier_than_timestamp=time_stamp_before_app_created
+    )
 
-    with SSMProxy(10022) as ssm_proxy:
-        ssm_proxy.connect_to_ssm_instance(studio_id)
+    with ide_wrapper.start_ssm_connection(10022, timeout=timedelta(minutes=5)) as ssm_proxy:
+        ide_wrapper.print_ssh_info()
 
         services_running = ssm_proxy.run_command_with_output("sm-ssh-ide status")
         services_running = services_running.decode('latin1')
 
         output = ssm_proxy.run_command_with_output("sm-ssh-ide env-diagnostics")
         output = output.decode('latin1')
         logger.info(f"Collected env diagnostics for {image_name}: {output}")
@@ -153,15 +155,15 @@
     studio_id = notebook_ids[0]
 
     with SSMProxy(17022) as ssm_proxy:
         ssm_proxy.connect_to_ssm_instance(studio_id)
 
         _ = ssm_proxy.run_command("apt-get install -q -y net-tools")
 
-        services_running = ssm_proxy.run_command_with_output("netstat -nptl")
+        services_running = ssm_proxy.run_command_with_output("netstat -nptl")  # noqa
         services_running = services_running.decode('latin1')
 
         python_version = ssm_proxy.run_command_with_output("/opt/conda/bin/python --version")
         python_version = python_version.decode('latin1')
 
     assert "0.0.0.0:22" in services_running
 
@@ -170,26 +172,26 @@
 
 def test_studio_internet_free_mode(request):
     """
     See https://docs.aws.amazon.com/sagemaker/latest/dg/studio-byoi.html
     """
     logging.info("Building BYO SageMaker Studio image for Internet-free mode")
     subprocess.check_call(
-        "sm-docker build . --file tests/byoi_studio/Dockerfile.internet_free --repo smstudio-custom-ssh:custom"
+        "sm-docker build . --file tests/byoi_studio/Dockerfile.internet_free --repo smstudio-custom-ssh:custom"  # noqa
         .split(' '),
         cwd="../"
     )
 
     logging.info("Creating SageMaker Studio kernel gateway app")
 
     ide = SSHIDE(request.config.getini('sagemaker_studio_vpc_only_domain'), 'internet-free-user')
 
     image = ide.create_and_attach_image(
         'custom-image-ssh',
-        'smstudio-custom-ssh:custom',
+        'smstudio-custom-ssh:custom',  # noqa
         request.config.getini('sagemaker_role'),
         app_image_config_name='custom-image-config-ssh',
         kernel_specs=[
             {
                 "Name": "python3",  # SHOULD match the output of `jupyter-kernelspec list` during the container build
                 "DisplayName": "Python 3 - with SageMaker SSH Helper"
             }
@@ -202,43 +204,44 @@
     )
 
     assert image.arn is not None
     assert image.version_arn is not None
 
     ide.delete_app("byoi-studio-app", 'KernelGateway', wait=True)
 
+    time_stamp_before_app_created = int(time.time())
+
     ide.create_ssh_kernel_app(
         "byoi-studio-app",
         image.arn,
         "ml.m5.large",
         recreate=True
     )
 
-    time.sleep(60)
-
-    studio_ids = ide.get_kernel_instance_ids("byoi-studio-app", timeout_in_sec=300)
-    studio_id = studio_ids[0]
+    ide_wrapper = SSHIDEWrapper.attach(
+        ide.domain_id, ide.user, "byoi-studio-app",
+        not_earlier_than_timestamp=time_stamp_before_app_created
+    )
 
-    with SSMProxy(10022) as ssm_proxy:
-        ssm_proxy.connect_to_ssm_instance(studio_id)
+    with ide_wrapper.start_ssm_connection(10022, timeout=timedelta(minutes=5)) as ssm_proxy:
         services_running = ssm_proxy.run_command_with_output("sm-ssh-ide status")
         services_running = services_running.decode('latin1')
 
     assert "127.0.0.1:8889" in services_running
     assert "127.0.0.1:5901" in services_running
 
     ide.delete_kernel_app("byoi-studio-app", wait=False)
 
 
 # noinspection DuplicatedCode
 def test_studio_multiple_users(request):
-    ide_ds = SSHIDE(request.config.getini('sagemaker_studio_domain'), 'test-data-science')
+    ide_tf = SSHIDE(request.config.getini('sagemaker_studio_domain'), 'test-tensorflow')
     ide_pt = SSHIDE(request.config.getini('sagemaker_studio_domain'), 'test-pytorch')
 
-    ide_ds.create_ssh_kernel_app(
+    ide_tf.create_ssh_kernel_app(
         'ssh-test-user',
         image_name_or_arn='sagemaker-data-science-310-v1',
         instance_type='ml.m5.large',
         ssh_lifecycle_config='sagemaker-ssh-helper-dev',
         recreate=True
     )
 
@@ -252,36 +255,35 @@
         ssh_lifecycle_config='sagemaker-ssh-helper-dev',
         recreate=True
     )
 
     # Give time for instance ID to propagate
     time.sleep(60)
 
-    studio_ids = ide_ds.get_kernel_instance_ids('ssh-test-user', timeout_in_sec=300)
-    studio_id = studio_ids[0]
-
-    with SSMProxy(10022) as ssm_proxy:
-        ssm_proxy.connect_to_ssm_instance(studio_id)
+    ide_wrapper = SSHIDEWrapper.attach(
+        ide_tf.domain_id, ide_tf.user, "ssh-test-user"
+    )
 
+    with ide_wrapper.start_ssm_connection(10022, timeout=timedelta(minutes=5)) as ssm_proxy:
         user_profile_name = ssm_proxy.run_command_with_output("sm-ssh-ide get-user-profile-name")
         user_profile_name = user_profile_name.decode('latin1')
         logger.info(f"Collected SageMaker Studio profile name: {user_profile_name}")
 
-    ide_ds.delete_kernel_app('ssh-test-user', wait=False)
+    ide_tf.delete_kernel_app('ssh-test-user', wait=False)
     ide_pt.delete_kernel_app('ssh-test-user', wait=False)
 
-    assert "test-data-science" in user_profile_name
+    assert "test-tensorflow" in user_profile_name
 
 
 # noinspection DuplicatedCode
 def test_studio_default_domain_multiple_users(request):
-    ide_ds = SSHIDE(request.config.getini('sagemaker_studio_domain'), 'test-data-science')
+    ide_tf = SSHIDE(request.config.getini('sagemaker_studio_domain'), 'test-tensorflow')
     ide_pt = SSHIDE(request.config.getini('sagemaker_studio_domain'), 'test-pytorch')
 
-    ide_ds.create_ssh_kernel_app(
+    ide_tf.create_ssh_kernel_app(
         'ssh-test-user',
         image_name_or_arn='sagemaker-data-science-310-v1',
         instance_type='ml.m5.large',
         ssh_lifecycle_config='sagemaker-ssh-helper-dev',
         recreate=True
     )
 
@@ -296,153 +298,98 @@
         recreate=True
     )
 
     # Give time for instance ID to propagate
     time.sleep(60)
 
     # Empty domain "" to fetch the latest profile, useful when switching between many AWS accounts with the same profile
-    studio_ids = SSHIDE("", 'test-data-science').get_kernel_instance_ids('ssh-test-user', timeout_in_sec=300)
-    studio_id = studio_ids[0]
-
-    with SSMProxy(10022) as ssm_proxy:
-        ssm_proxy.connect_to_ssm_instance(studio_id)
+    ide_wrapper = SSHIDEWrapper.attach(
+        "", ide_tf.user, "ssh-test-user"
+    )
 
+    with ide_wrapper.start_ssm_connection(10022, timeout=timedelta(minutes=5)) as ssm_proxy:
         user_profile_name = ssm_proxy.run_command_with_output("sm-ssh-ide get-user-profile-name")
         user_profile_name = user_profile_name.decode('latin1')
         logger.info(f"Collected SageMaker Studio profile name: {user_profile_name}")
 
-    ide_ds.delete_kernel_app('ssh-test-user', wait=False)
+    ide_tf.delete_kernel_app('ssh-test-user', wait=False)
     ide_pt.delete_kernel_app('ssh-test-user', wait=False)
 
-    assert "test-data-science" in user_profile_name
+    assert "test-tensorflow" in user_profile_name
 
 
-def test_studio_notebook_in_firefox(request):
-    ide = SSHIDE(request.config.getini('sagemaker_studio_domain'), 'test-data-science')
+@pytest.mark.parametrize('user_profile_name', ['test-firefox'])
+def test_studio_notebook_in_firefox(request, user_profile_name):
+    ide = SSHIDE(request.config.getini('sagemaker_studio_domain'), user_profile_name)
+    local_user_id = os.environ['LOCAL_USER_ID']
+    jb_server_host = os.environ['JB_LICENSE_SERVER_HOST']
+
+    options = Options()
+    options.set_preference("browser.download.folderList", 2)
+    options.set_preference("browser.download.manager.showWhenStarting", False)
+    options.set_preference("browser.download.dir", os.path.abspath("../tests/output/"))
+    firefox = webdriver.Firefox(options)
 
-    # Get SageMaker Studio Presigned URL with API
-    sagemaker_client = boto3.client('sagemaker')
-    studio_pre_signed_url_response = sagemaker_client.create_presigned_domain_url(
-        DomainId=ide.domain_id,
-        UserProfileName=ide.user,
-    )
-    studio_pre_signed_url = studio_pre_signed_url_response['AuthorizedUrl']
-
-    logging.info("Launching Firefox")
-    browser = webdriver.Firefox()
-
-    logging.info("Launching SageMaker Studio")
-    browser.get(studio_pre_signed_url)
-
-    logging.info("Waiting for SageMaker Studio to launch")
-    WebDriverWait(browser, 600).until(
-        EC.presence_of_element_located((By.XPATH, "//div[@id='space-menu']"))
-    )
-    kernel_menu_item = browser.find_element(By.XPATH, "//div[@id='space-menu']")
-    logging.info(f"Found SageMaker Studio space menu item: {kernel_menu_item.text}")
-    assert kernel_menu_item.text == 'test-data-science / Personal Studio'
-
-    time.sleep(60)  # wait until obscurity of the menu items is gone and UI is fully loaded
-
-    logging.info("Checking the kernel name")
-    kernel_item = browser.find_element(
-        By.XPATH,
-        "//button[@class='bp3-button bp3-minimal jp-Toolbar-kernelName "
-        "jp-ToolbarButtonComponent minimal jp-Button']"
-    )
-    logging.info(f"Found Kernel name: {kernel_item.text}")
-    assert kernel_item.text == "Data Science 2.0\n|\nPython 3\n|\n2 vCPU + 8 GiB"
+    browser_automation = SageMakerStudioAutomation(ide, firefox)
+    browser_automation.launch_sagemaker_studio()
 
     dist_file_name_pattern = 'sagemaker_ssh_helper-.*-py3-none-any.whl'
     dist_file_name = [f for f in os.listdir('../dist') if re.match(dist_file_name_pattern, f)][0]
     logging.info(f"Found dist file: {dist_file_name}")
 
-    # TODO: File -> Reload notebook from Disk
-    # TODO: ide.add_new_cell([
-    #  f"%%sh"
-    #  f"pip3 install -U ./{dist_file_name}"
-    #  ])
-
-    upload_file(browser, os.path.abspath("../SageMaker_SSH_IDE.ipynb"))
-    logging.info("IDE notebook uploaded")
-    upload_file(browser, os.path.abspath(Path("../dist/", dist_file_name)))
-    logging.info("Dist file uploaded")
-
-    kernel_menu_item = browser.find_element(
-        By.XPATH,
-        "//div[@class='lm-MenuBar-itemLabel p-MenuBar-itemLabel' "
-        "and text()='Kernel']"
-    )
-    logging.info(f"Found SageMaker Studio kernel menu item: {kernel_menu_item.text}")
-    kernel_menu_item.click()
-
-    logging.info("Restarting kernel and running all cells")
-    restart_menu_item = browser.find_element(
-        By.XPATH,
-        "//div[@class='lm-Menu-itemLabel p-Menu-itemLabel' "
-        "and text()='Restart Kernel and Run All Cells…']")
-    logging.info(f"Found SageMaker Studio restart kernel menu item: {restart_menu_item.text}")
-    restart_menu_item.click()
-
-    # TODO: check banner if kernel is still starting, wait until banner disappears, then click restart
-    # <div class="css-a7sx0c-bannerContainer sagemaker-starting-banner" id="sagemaker-notebook-banner"><div class="css-1qyc1pu-kernelStartingBannerContainer"><div><div class="css-6wrpfe-bannerSpinDiv"></div></div><div><p class="css-g9mx5z-bannerPromptSpanTitle">Starting notebook kernel...</p></div></div></div>
-
-    restart_button = browser.find_element(
-        By.XPATH,
-        "//div[@class='jp-Dialog-buttonLabel' "
-        "and text()='Restart']"
-    )
-    logging.info(f"Found SageMaker Studio restart button: {restart_button.text}")
-    restart_button.click()
-
-    time.sleep(120)  # Give time to restart
-
-    studio_ids = ide.get_kernel_instance_ids("sagemaker-data-science-ml-m5-large-6590da95dc67eec021b14bedc036",
-                                             timeout_in_sec=300)
-    studio_id = studio_ids[0]
-
-    with SSMProxy(10022) as ssm_proxy:
-        ssm_proxy.connect_to_ssm_instance(studio_id)
-        services_running = ssm_proxy.run_command_with_output("sm-ssh-ide status")
-        services_running = services_running.decode('latin1')
-
-    # TODO: File -> Save Notebook
-    # TODO: ide.download_ssh("/root/SageMaker_SSH_IDE-DS2-CPU.ipynb",
-    #  "./output/SageMaker_SSH_IDE-DS2-CPU.ipynb")
-    # See: https://github.com/aws-samples/sagemaker-ssh-helper/issues/18
-
-    assert "127.0.0.1:8889" in services_running
-    assert "127.0.0.1:5901" in services_running
-
-    # TODO: assert the services were restarted by the test, e.g., by checking the SSM timestamp
-    # TODO: check if the second restart also successful
-
-    # TODO: restart image (clean-up for the next run)
-    # <button type="button" class="bp3-button bp3-minimal jp-ToolbarButtonComponent minimal jp-Button" aria-disabled="false" title="Shut down">...</button>    """
+    notebook = JupyterNotebook(Path("../SageMaker_SSH_IDE.ipynb"))
+    notebook.insert_code_cell(0, [
+        f"%%sh\n",
+        f"pip3 install -U ./{dist_file_name}"
+    ])
+    notebook.insert_code_cell(0, [
+        f"%%sh\n",
+        f"echo '{jb_server_host}' > ~/.sm-jb-license-server"
+    ])
+    notebook.insert_code_cell(0, [
+        f"%%sh\n",
+        f"echo '{local_user_id}' > ~/.sm-ssh-owner"
+    ])
+    ide_notebook_path = Path("../tests/output/SageMaker_SSH_IDE-DS2-CPU.ipynb")
+    notebook.save_as(ide_notebook_path)
+
+    browser_automation.upload_file_with_overwrite(ide_notebook_path)
+    browser_automation.upload_file_with_overwrite(Path("../dist/", dist_file_name))
+
+    # rename to keep original and to compare with the output later
+    os.rename("../tests/output/SageMaker_SSH_IDE-DS2-CPU.ipynb",
+              "../tests/output/SageMaker_SSH_IDE-DS2-CPU-Original.ipynb")
+
+    browser_automation.open_file_from_path("/SageMaker_SSH_IDE-DS2-CPU.ipynb", 'ml.m5.large')
+
+    for retries in range(0, 1):
+        current_time_stamp = int(time.time())
+
+        browser_automation.restart_kernel_and_run_all_cells()
+
+        data_science_kernel = "sagemaker-data-science-ml-m5-large-6590da95dc67eec021b14bedc036"  # noqa
+        studio_id = ide.get_kernel_instance_id(
+            data_science_kernel,
+            timeout_in_sec=300,
+            not_earlier_than_timestamp=current_time_stamp
+        )
+        ssh_timestamp = SSMManager().get_ssh_instance_timestamp(studio_id)
+
+        assert ssh_timestamp > current_time_stamp
+
+        time.sleep(120)  # Give time for agent to connect
+
+        ide_wrapper = SSHIDEWrapper.attach(
+            ide.domain_id, ide.user, data_science_kernel
+        )
+
+        with ide_wrapper.start_ssm_connection(10022, timeout=timedelta(minutes=5)) as ssm_proxy:
+            services_running = ssm_proxy.run_command_with_output("sm-ssh-ide status")
+            services_running = services_running.decode('latin1')
 
-    logging.info("Closing Firefox")
-    browser.close()
+        assert "127.0.0.1:8889" in services_running
+        assert "127.0.0.1:5901" in services_running
 
+    browser_automation.save_current_file()
+    browser_automation.download_current_file()
 
-def upload_file(browser, file_abs_path):
-    file_drop_area = browser.find_element(
-        By.XPATH,
-        "//ul[@class='jp-DirListing-content']"
-    )
-    logging.info(f"Found file browser to drop the file to: {file_drop_area.text}")
-    time.sleep(2)
-    file_input = browser.execute_script(Path('js/drop_studio_file.js').read_text(), file_drop_area, 0, 0)
-    logging.info(f"Created a file upload item: {file_input}")
-    file_input.send_keys(file_abs_path)
-    time.sleep(5)  # Give time to overwrite dialog to apper
-    confirm_overwrite(browser)
-
-
-def confirm_overwrite(browser):
-    overwrite_button = browser.find_elements(
-        By.XPATH,
-        "//div[@class='jp-Dialog-buttonLabel' "
-        "and text()='Overwrite']"
-    )
-    if len(overwrite_button) > 0:
-        logging.info(f"Found overwrite dialog button: {overwrite_button[0].text}")
-        overwrite_button[0].click()
+    browser_automation.close_sagemaker_studio()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `sagemaker-ssh-helper-2.1.0/tests/test_inference_registry.py` & `sagemaker_ssh_helper-2.2.0/tests/test_inference_registry.py`

 * *Files identical despite different names*

### Comparing `sagemaker-ssh-helper-2.1.0/tests/test_local.py` & `sagemaker_ssh_helper-2.2.0/tests/test_local.py`

 * *Files identical despite different names*

### Comparing `sagemaker-ssh-helper-2.1.0/tests/test_manual.py` & `sagemaker_ssh_helper-2.2.0/tests/test_manual.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 import logging
 import os
 from datetime import timedelta
+from pathlib import Path
 
+import boto3
 import pytest
 import sagemaker
 from sagemaker import Predictor
 from sagemaker.djl_inference import DJLPredictor
 from sagemaker.pytorch import PyTorch, PyTorchProcessor
 from sagemaker.utils import name_from_base
 
 from sagemaker_ssh_helper.log import SSHLog
 from sagemaker_ssh_helper.wrapper import SSHEstimatorWrapper, SSHProcessorWrapper, SSHModelWrapper
 
+import json
+
 
 # noinspection DuplicatedCode
 @pytest.mark.skipif(os.getenv('PYTEST_IGNORE_SKIPS', "false") == "false",
                     reason="Manual test")
 def test_train_placeholder_manual():
     bucket = sagemaker.Session().default_bucket()
     checkpoints_prefix = f"s3://{bucket}/checkpoints/"
@@ -26,29 +30,26 @@
         dependencies=[SSHEstimatorWrapper.dependency_dir()],  # <--NEW
         # (alternatively, add sagemaker_ssh_helper into requirements.txt
         # inside source dir) --
         base_job_name='ssh-training-manual',
         framework_version='1.9.1',
         py_version='py38',
         instance_count=1,
-        instance_type='ml.m5.xlarge',
+        instance_type='ml.g4dn.xlarge',
         max_run=60 * 60 * 3,
         keep_alive_period_in_seconds=1800,
         container_log_level=logging.INFO,
         checkpoint_s3_uri=checkpoints_prefix
     )
 
     ssh_wrapper = SSHEstimatorWrapper.create(estimator, connection_wait_time_seconds=0)  # <--NEW--
 
     estimator.fit(wait=False)
 
-    instance_ids = ssh_wrapper.get_instance_ids(timeout_in_sec=600)  # <--NEW--
-
-    logging.info(f"To connect over SSM run: aws ssm start-session --target {instance_ids[0]}")
-    logging.info(f"To connect over SSH run: sm-local-ssh-training connect {ssh_wrapper.training_job_name()}")
+    ssh_wrapper.print_ssh_info()
 
     ssh_wrapper.wait_training_job()
 
 
 @pytest.mark.skipif(os.getenv('PYTEST_IGNORE_SKIPS', "false") == "false",
                     reason="Manual test")
 def test_processing_framework_manual():
@@ -69,17 +70,15 @@
         source_dir="source_dir/processing/",
         dependencies=[SSHProcessorWrapper.dependency_dir()],
         code="process_framework.py",
         logs=True,
         wait=False
     )
 
-    instance_ids = ssh_wrapper.get_instance_ids(60)
-
-    logging.info(f"To connect over SSM run: aws ssm start-session --target {instance_ids[0]}")
+    ssh_wrapper.print_ssh_info()
 
     ssh_wrapper.wait_processing_job()
 
 
 @pytest.mark.skipif(os.getenv('PYTEST_IGNORE_SKIPS', "false") == "false",
                     reason="Manual test")
 def test_inference_manual():
@@ -94,17 +93,15 @@
     endpoint_name = name_from_base('ssh-inference-manual')
 
     _: Predictor = model.deploy(initial_instance_count=1,
                                 instance_type='ml.m5.xlarge',
                                 endpoint_name=endpoint_name,
                                 wait=True)
 
-    instance_ids = ssh_wrapper.get_instance_ids(60)
-
-    logging.info(f"To connect over SSM run: aws ssm start-session --target {instance_ids[0]}")
+    ssh_wrapper.print_ssh_info()
 
     ssh_wrapper.wait_for_endpoint()
 
 
 @pytest.mark.skipif(os.getenv('PYTEST_IGNORE_SKIPS', "false") == "false",
                     reason="Manual test")
 def test_djl_inference():
@@ -128,16 +125,57 @@
     import subprocess
     subprocess.check_call("uname -a".split(' '))
     logging.info("OK")
 
 
 @pytest.mark.skipif(os.getenv('PYTEST_IGNORE_SKIPS', "false") == "false",
                     reason="Manual test")
+def test_sns_publish(request):
+    sns_notification_topic_arn = request.config.getini('sns_notification_topic_arn')
+    logging.info(f"Send notification email and/or SMS through Amazon SNS topic {sns_notification_topic_arn}")
+    sns_resource = boto3.resource('sns')
+    sns_notification_topic = sns_resource.Topic(sns_notification_topic_arn)
+    response = sns_notification_topic.publish(
+        Subject='Manual test subject',
+        Message='Manual test message'
+    )
+    logging.info(f"SNS response: {response}")
+
+
+@pytest.mark.skipif(os.getenv('PYTEST_IGNORE_SKIPS', "false") == "false",
+                    reason="Manual test")
+def test_low_gpu_lambda():
+    from sagemaker_ssh_helper.cdk.low_gpu.low_gpu_lambda import handler
+    with open(str(Path('data/lambda/lambda_processing_event.json')), 'r') as f:
+        event = f.read()
+        event = json.loads(event)
+    handler(event, None)
+
+
+@pytest.mark.skipif(os.getenv('PYTEST_IGNORE_SKIPS', "false") == "false",
+                    reason="Manual test")
 def test_cloudwatch_metrics_sns(request):
     sns_notification_topic_arn = request.config.getini('sns_notification_topic_arn')
     topic_name = sns_notification_topic_arn.split(':')[-1]
 
     log = SSHLog()
     metrics_count = log.count_sns_notifications(topic_name, timedelta(minutes=15))
     logging.info(metrics_count)
 
     assert metrics_count > 0
+
+
+@pytest.mark.skipif(os.getenv('PYTEST_IGNORE_SKIPS', "false") == "false",
+                    reason="Manual test")
+def test_can_attach_to_endpoint():
+    boto3_session = boto3.session.Session(region_name="us-east-2")
+    session = sagemaker.session.Session(boto_session=boto3_session)
+    wrapper = SSHModelWrapper.attach('sd-inf2-ml-inf2-2023-11-07-13-33-05-254', session)
+    assert 'sd-inf2-ml-inf2-2023-11-07-13-33-05-254' in wrapper.get_cloudwatch_url()
+    assert wrapper.get_instance_id(timeout_in_sec=0) is not None
+
+
+@pytest.mark.skipif(os.getenv('PYTEST_IGNORE_SKIPS', "false") == "false",
+                    reason="Manual test")
+def test_get_ssh_instance_timestamp():
+    from sagemaker_ssh_helper.manager import SSMManager
+    print(SSMManager().get_ssh_instance_timestamp('mi-0c5a1be17a45c83bf'))
```

### Comparing `sagemaker-ssh-helper-2.1.0/tests/test_util.py` & `sagemaker_ssh_helper-2.2.0/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `sagemaker-ssh-helper-2.1.0/tests/test_validation.py` & `sagemaker_ssh_helper-2.2.0/tests/test_validation.py`

 * *Files identical despite different names*

