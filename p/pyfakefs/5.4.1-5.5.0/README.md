# Comparing `tmp/pyfakefs-5.4.1.tar.gz` & `tmp/pyfakefs-5.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfakefs-5.4.1.tar", last modified: Thu Apr 11 18:13:39 2024, max compression
+gzip compressed data, was "pyfakefs-5.5.0.tar", last modified: Sun May 12 06:42:00 2024, max compression
```

## Comparing `pyfakefs-5.4.1.tar` & `pyfakefs-5.5.0.tar`

### file list

```diff
@@ -1,83 +1,87 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:13:39.719081 pyfakefs-5.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)    49861 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/CHANGES.md
--rw-r--r--   0 runner    (1001) docker     (127)     3403 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    10142 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/COPYING
--rwxr-xr-x   0 runner    (1001) docker     (127)       57 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7718 2024-04-11 18:13:39.719081 pyfakefs-5.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6104 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/extra_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/mypy.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:13:39.711081 pyfakefs-5.4.1/pyfakefs/
--rwxr-xr-x   0 runner    (1001) docker     (127)       56 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/pyfakefs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/pyfakefs/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/pyfakefs/extra_packages.py
--rw-r--r--   0 runner    (1001) docker     (127)    49019 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/pyfakefs/fake_file.py
--rw-r--r--   0 runner    (1001) docker     (127)   123400 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/pyfakefs/fake_filesystem.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3756 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/pyfakefs/fake_filesystem_shutil.py
--rw-r--r--   0 runner    (1001) docker     (127)    45083 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/pyfakefs/fake_filesystem_unittest.py
--rw-r--r--   0 runner    (1001) docker     (127)     6817 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/pyfakefs/fake_io.py
--rw-r--r--   0 runner    (1001) docker     (127)    13893 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/pyfakefs/fake_open.py
--rw-r--r--   0 runner    (1001) docker     (127)    53434 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/pyfakefs/fake_os.py
--rw-r--r--   0 runner    (1001) docker     (127)    18284 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/pyfakefs/fake_path.py
--rw-r--r--   0 runner    (1001) docker     (127)    34844 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/pyfakefs/fake_pathlib.py
--rw-r--r--   0 runner    (1001) docker     (127)    11364 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/pyfakefs/fake_scandir.py
--rw-r--r--   0 runner    (1001) docker     (127)    13441 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/pyfakefs/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5393 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/pyfakefs/mox3_stubout.py
--rw-r--r--   0 runner    (1001) docker     (127)     6591 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/pyfakefs/patched_packages.py
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/pyfakefs/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     2280 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/pyfakefs/pytest_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:13:39.715081 pyfakefs-5.4.1/pyfakefs/pytest_tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/pyfakefs/pytest_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/pyfakefs/pytest_tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/pyfakefs/pytest_tests/example.py
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/pyfakefs/pytest_tests/io.py
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/pyfakefs/pytest_tests/pytest_check_failed_plugin_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/pyfakefs/pytest_tests/pytest_doctest_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/pyfakefs/pytest_tests/pytest_fixture_param_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/pyfakefs/pytest_tests/pytest_fixture_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/pyfakefs/pytest_tests/pytest_module_fixture_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/pyfakefs/pytest_tests/pytest_plugin_failing_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/pyfakefs/pytest_tests/pytest_plugin_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/pyfakefs/pytest_tests/pytest_reload_pandas_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/pyfakefs/pytest_tests/unhashable.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:13:39.719081 pyfakefs-5.4.1/pyfakefs/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/pyfakefs/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/pyfakefs/tests/all_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/pyfakefs/tests/all_tests_without_extra_packages.py
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/pyfakefs/tests/dynamic_patch_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4012 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/pyfakefs/tests/example.py
--rw-r--r--   0 runner    (1001) docker     (127)     6954 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/pyfakefs/tests/example_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2587 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/pyfakefs/tests/fake_filesystem_glob_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    22626 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/pyfakefs/tests/fake_filesystem_shutil_test.py
--rw-r--r--   0 runner    (1001) docker     (127)   110189 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/pyfakefs/tests/fake_filesystem_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    35456 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/pyfakefs/tests/fake_filesystem_unittest_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    29767 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/pyfakefs/tests/fake_filesystem_vs_real_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    87621 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/pyfakefs/tests/fake_open_test.py
--rw-r--r--   0 runner    (1001) docker     (127)   244080 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/pyfakefs/tests/fake_os_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    52726 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/pyfakefs/tests/fake_pathlib_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    22479 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/pyfakefs/tests/fake_stat_time_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4199 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/pyfakefs/tests/fake_tempfile_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:13:39.719081 pyfakefs-5.4.1/pyfakefs/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/pyfakefs/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/pyfakefs/tests/fixtures/config_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/pyfakefs/tests/fixtures/deprecated_property.py
--rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/pyfakefs/tests/fixtures/module_with_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/pyfakefs/tests/import_as_example.py
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/pyfakefs/tests/logsio.py
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/pyfakefs/tests/mox3_stubout_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     5363 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/pyfakefs/tests/mox3_stubout_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2570 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/pyfakefs/tests/patched_packages_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2621 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/pyfakefs/tests/performance_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    17536 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/pyfakefs/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:13:39.719081 pyfakefs-5.4.1/pyfakefs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7718 2024-04-11 18:13:39.000000 pyfakefs-5.4.1/pyfakefs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-04-11 18:13:39.000000 pyfakefs-5.4.1/pyfakefs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 18:13:39.000000 pyfakefs-5.4.1/pyfakefs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-11 18:13:39.000000 pyfakefs-5.4.1/pyfakefs.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-11 18:13:39.000000 pyfakefs-5.4.1/pyfakefs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-04-11 18:13:39.723081 pyfakefs-5.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-11 18:13:32.000000 pyfakefs-5.4.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 06:42:00.111931 pyfakefs-5.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    50824 2024-05-12 06:41:52.000000 pyfakefs-5.5.0/CHANGES.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3403 2024-05-12 06:41:52.000000 pyfakefs-5.5.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10142 2024-05-12 06:41:52.000000 pyfakefs-5.5.0/COPYING
+-rwxr-xr-x   0 runner    (1001) docker     (127)       57 2024-05-12 06:41:52.000000 pyfakefs-5.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7718 2024-05-12 06:42:00.111931 pyfakefs-5.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6104 2024-05-12 06:41:52.000000 pyfakefs-5.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-12 06:41:52.000000 pyfakefs-5.5.0/extra_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-12 06:41:52.000000 pyfakefs-5.5.0/legacy_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-12 06:41:52.000000 pyfakefs-5.5.0/mypy.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 06:42:00.103931 pyfakefs-5.5.0/pyfakefs/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       56 2024-05-12 06:41:52.000000 pyfakefs-5.5.0/pyfakefs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-12 06:41:52.000000 pyfakefs-5.5.0/pyfakefs/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49019 2024-05-12 06:41:52.000000 pyfakefs-5.5.0/pyfakefs/fake_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)   123400 2024-05-12 06:41:52.000000 pyfakefs-5.5.0/pyfakefs/fake_filesystem.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3756 2024-05-12 06:41:52.000000 pyfakefs-5.5.0/pyfakefs/fake_filesystem_shutil.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45109 2024-05-12 06:41:52.000000 pyfakefs-5.5.0/pyfakefs/fake_filesystem_unittest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5678 2024-05-12 06:41:52.000000 pyfakefs-5.5.0/pyfakefs/fake_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3901 2024-05-12 06:41:52.000000 pyfakefs-5.5.0/pyfakefs/fake_legacy_modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15575 2024-05-12 06:41:52.000000 pyfakefs-5.5.0/pyfakefs/fake_open.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53353 2024-05-12 06:41:52.000000 pyfakefs-5.5.0/pyfakefs/fake_os.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18284 2024-05-12 06:41:52.000000 pyfakefs-5.5.0/pyfakefs/fake_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36190 2024-05-12 06:41:52.000000 pyfakefs-5.5.0/pyfakefs/fake_pathlib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8992 2024-05-12 06:41:52.000000 pyfakefs-5.5.0/pyfakefs/fake_scandir.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13441 2024-05-12 06:41:52.000000 pyfakefs-5.5.0/pyfakefs/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-05-12 06:41:52.000000 pyfakefs-5.5.0/pyfakefs/legacy_packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5393 2024-05-12 06:41:52.000000 pyfakefs-5.5.0/pyfakefs/mox3_stubout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6591 2024-05-12 06:41:52.000000 pyfakefs-5.5.0/pyfakefs/patched_packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-12 06:41:52.000000 pyfakefs-5.5.0/pyfakefs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     2280 2024-05-12 06:41:52.000000 pyfakefs-5.5.0/pyfakefs/pytest_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 06:42:00.107931 pyfakefs-5.5.0/pyfakefs/pytest_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 06:41:52.000000 pyfakefs-5.5.0/pyfakefs/pytest_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-05-12 06:41:52.000000 pyfakefs-5.5.0/pyfakefs/pytest_tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-12 06:41:52.000000 pyfakefs-5.5.0/pyfakefs/pytest_tests/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-12 06:41:52.000000 pyfakefs-5.5.0/pyfakefs/pytest_tests/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-05-12 06:41:52.000000 pyfakefs-5.5.0/pyfakefs/pytest_tests/pytest_check_failed_plugin_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-05-12 06:41:52.000000 pyfakefs-5.5.0/pyfakefs/pytest_tests/pytest_doctest_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-05-12 06:41:52.000000 pyfakefs-5.5.0/pyfakefs/pytest_tests/pytest_fixture_param_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-05-12 06:41:52.000000 pyfakefs-5.5.0/pyfakefs/pytest_tests/pytest_fixture_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-05-12 06:41:52.000000 pyfakefs-5.5.0/pyfakefs/pytest_tests/pytest_module_fixture_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-12 06:41:52.000000 pyfakefs-5.5.0/pyfakefs/pytest_tests/pytest_plugin_failing_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-05-12 06:41:52.000000 pyfakefs-5.5.0/pyfakefs/pytest_tests/pytest_plugin_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-12 06:41:52.000000 pyfakefs-5.5.0/pyfakefs/pytest_tests/pytest_reload_pandas_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-12 06:41:52.000000 pyfakefs-5.5.0/pyfakefs/pytest_tests/unhashable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 06:42:00.111931 pyfakefs-5.5.0/pyfakefs/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 06:41:52.000000 pyfakefs-5.5.0/pyfakefs/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-05-12 06:41:52.000000 pyfakefs-5.5.0/pyfakefs/tests/all_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-12 06:41:52.000000 pyfakefs-5.5.0/pyfakefs/tests/all_tests_without_extra_packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-05-12 06:41:52.000000 pyfakefs-5.5.0/pyfakefs/tests/dynamic_patch_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4012 2024-05-12 06:41:52.000000 pyfakefs-5.5.0/pyfakefs/tests/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6921 2024-05-12 06:41:52.000000 pyfakefs-5.5.0/pyfakefs/tests/example_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2587 2024-05-12 06:41:52.000000 pyfakefs-5.5.0/pyfakefs/tests/fake_filesystem_glob_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22626 2024-05-12 06:41:52.000000 pyfakefs-5.5.0/pyfakefs/tests/fake_filesystem_shutil_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)   109989 2024-05-12 06:41:52.000000 pyfakefs-5.5.0/pyfakefs/tests/fake_filesystem_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35456 2024-05-12 06:41:52.000000 pyfakefs-5.5.0/pyfakefs/tests/fake_filesystem_unittest_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29767 2024-05-12 06:41:52.000000 pyfakefs-5.5.0/pyfakefs/tests/fake_filesystem_vs_real_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3744 2024-05-12 06:41:52.000000 pyfakefs-5.5.0/pyfakefs/tests/fake_legacy_modules_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    87957 2024-05-12 06:41:52.000000 pyfakefs-5.5.0/pyfakefs/tests/fake_open_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)   243371 2024-05-12 06:41:52.000000 pyfakefs-5.5.0/pyfakefs/tests/fake_os_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54109 2024-05-12 06:41:52.000000 pyfakefs-5.5.0/pyfakefs/tests/fake_pathlib_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22479 2024-05-12 06:41:52.000000 pyfakefs-5.5.0/pyfakefs/tests/fake_stat_time_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4199 2024-05-12 06:41:52.000000 pyfakefs-5.5.0/pyfakefs/tests/fake_tempfile_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 06:42:00.111931 pyfakefs-5.5.0/pyfakefs/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 06:41:52.000000 pyfakefs-5.5.0/pyfakefs/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-12 06:41:52.000000 pyfakefs-5.5.0/pyfakefs/tests/fixtures/config_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-05-12 06:41:52.000000 pyfakefs-5.5.0/pyfakefs/tests/fixtures/deprecated_property.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-05-12 06:41:52.000000 pyfakefs-5.5.0/pyfakefs/tests/fixtures/module_with_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-05-12 06:41:52.000000 pyfakefs-5.5.0/pyfakefs/tests/import_as_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-12 06:41:52.000000 pyfakefs-5.5.0/pyfakefs/tests/logsio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-05-12 06:41:52.000000 pyfakefs-5.5.0/pyfakefs/tests/mox3_stubout_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5363 2024-05-12 06:41:52.000000 pyfakefs-5.5.0/pyfakefs/tests/mox3_stubout_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2570 2024-05-12 06:41:52.000000 pyfakefs-5.5.0/pyfakefs/tests/patched_packages_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2621 2024-05-12 06:41:52.000000 pyfakefs-5.5.0/pyfakefs/tests/performance_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-05-12 06:41:52.000000 pyfakefs-5.5.0/pyfakefs/tests/skip_open.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17536 2024-05-12 06:41:52.000000 pyfakefs-5.5.0/pyfakefs/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 06:42:00.111931 pyfakefs-5.5.0/pyfakefs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7718 2024-05-12 06:42:00.000000 pyfakefs-5.5.0/pyfakefs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-05-12 06:42:00.000000 pyfakefs-5.5.0/pyfakefs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 06:42:00.000000 pyfakefs-5.5.0/pyfakefs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-12 06:42:00.000000 pyfakefs-5.5.0/pyfakefs.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-12 06:42:00.000000 pyfakefs-5.5.0/pyfakefs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-12 06:41:52.000000 pyfakefs-5.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-12 06:41:52.000000 pyfakefs-5.5.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-12 06:41:52.000000 pyfakefs-5.5.0/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-05-12 06:42:00.111931 pyfakefs-5.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-12 06:41:52.000000 pyfakefs-5.5.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-12 06:41:52.000000 pyfakefs-5.5.0/tox.ini
```

### Comparing `pyfakefs-5.4.1/CHANGES.md` & `pyfakefs-5.5.0/CHANGES.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,29 @@
 # pyfakefs Release Notes
 The released versions correspond to PyPI releases.
 
+## Planned changes for next major release (6.0.0)
+* remove support for patching legacy modules `scandir` and `pathlib2`
+* remove support for Python 3.7
+
+## [Version 5.5.0](https://pypi.python.org/pypi/pyfakefs/5.5.0) (2024-05-12)
+Deprecates the usage of `pathlib2` and `scandir`.
+
+### Changes
+* The usage of the `pathlib2` and `scandir` modules in pyfakefs is now deprecated.
+  They will now cause deprecation warnings if still used. Support for patching
+  these modules will be removed in pyfakefs 6.0.
+* `PureWindowsPath` and `PurePosixPath` now use filesystem-independent path separators,
+  and their path-parsing behaviors are now consistent regardless of runtime platform
+  and/or faked filesystem customization (see [#1006](../../issues/1006)).
+
+### Fixes
+* fixed handling of Windows `pathlib` paths under POSIX and vice verse (see [#1006](../../issues/1006))
+* correctly use real open calls in pathlib for skipped modules (see [#1012](../../issues/1012))
+
 ## [Version 5.4.1](https://pypi.python.org/pypi/pyfakefs/5.4.0) (2024-04-11)
 Fixes a regression.
 
 ### Fixes
 * fixed a regression from version 5.4.0 that incorrectly handled files opened twice via file descriptor
   (see [#997](../../issues/997))
```

### Comparing `pyfakefs-5.4.1/CONTRIBUTING.md` & `pyfakefs-5.5.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.4.1/COPYING` & `pyfakefs-5.5.0/COPYING`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.4.1/PKG-INFO` & `pyfakefs-5.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfakefs
-Version: 5.4.1
+Version: 5.5.0
 Summary: pyfakefs implements a fake file system that mocks the Python file system modules.
 Home-page: https://github.com/pytest-dev/pyfakefs
 Author: Google
 Author-email: google-pyfakefs@google.com
 Maintainer: John McGehee
 Maintainer-email: pyfakefs@johnnado.com
 License: http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `pyfakefs-5.4.1/README.md` & `pyfakefs-5.5.0/README.md`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.4.1/mypy.ini` & `pyfakefs-5.5.0/mypy.ini`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.4.1/pyfakefs/fake_file.py` & `pyfakefs-5.5.0/pyfakefs/fake_file.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.4.1/pyfakefs/fake_filesystem.py` & `pyfakefs-5.5.0/pyfakefs/fake_filesystem.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.4.1/pyfakefs/fake_filesystem_shutil.py` & `pyfakefs-5.5.0/pyfakefs/fake_filesystem_shutil.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.4.1/pyfakefs/fake_filesystem_unittest.py` & `pyfakefs-5.5.0/pyfakefs/fake_filesystem_unittest.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,21 +79,19 @@
 from pyfakefs.helpers import IS_PYPY
 from pyfakefs.mox3_stubout import StubOutForTesting
 
 from importlib.machinery import ModuleSpec
 from importlib import reload
 
 from pyfakefs import fake_filesystem, fake_io, fake_os, fake_open, fake_path, fake_file
+from pyfakefs import fake_legacy_modules
 from pyfakefs import fake_filesystem_shutil
 from pyfakefs import fake_pathlib
 from pyfakefs import mox3_stubout
-from pyfakefs.extra_packages import pathlib2, use_scandir
-
-if use_scandir:
-    from pyfakefs import fake_scandir
+from pyfakefs.legacy_packages import pathlib2, scandir
 
 OS_MODULE = "nt" if sys.platform == "win32" else "posix"
 PATH_MODULE = "ntpath" if sys.platform == "win32" else "posixpath"
 
 
 def patchfs(
     _func: Optional[Callable] = None,
@@ -697,21 +695,23 @@
 
         # class modules maps class names against a list of modules they can
         # be contained in - this allows for alternative modules like
         # `pathlib` and `pathlib2`
         self._class_modules["Path"] = ["pathlib"]
         self._unfaked_module_classes["pathlib"] = fake_pathlib.RealPathlibModule
         if pathlib2:
-            self._fake_module_classes["pathlib2"] = fake_pathlib.FakePathlibModule
+            self._fake_module_classes["pathlib2"] = (
+                fake_legacy_modules.FakePathlib2Module
+            )
             self._class_modules["Path"].append("pathlib2")
             self._unfaked_module_classes["pathlib2"] = fake_pathlib.RealPathlibModule
+        if scandir:
+            self._fake_module_classes["scandir"] = fake_legacy_modules.FakeScanDirModule
         self._fake_module_classes["Path"] = fake_pathlib.FakePathlibPathModule
         self._unfaked_module_classes["Path"] = fake_pathlib.RealPathlibPathModule
-        if use_scandir:
-            self._fake_module_classes["scandir"] = fake_scandir.FakeScanDirModule
 
     def _init_fake_module_functions(self) -> None:
         # handle patching function imported separately like
         # `from os import stat`
         # each patched function name has to be looked up separately
         for mod_name, fake_module in self._fake_module_classes.items():
             if hasattr(fake_module, "dir"):
```

### Comparing `pyfakefs-5.4.1/pyfakefs/fake_io.py` & `pyfakefs-5.5.0/pyfakefs/fake_io.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,31 +14,29 @@
 
 """Uses :py:class:`FakeIoModule` to provide a
 fake ``io`` module replacement.
 """
 
 import _io  # pytype: disable=import-error
 import io
-import os
 import sys
-import traceback
 from enum import Enum
 from typing import (
     List,
     Optional,
     Callable,
     Union,
     Any,
     AnyStr,
     IO,
     TYPE_CHECKING,
 )
 
 from pyfakefs.fake_file import AnyFileWrapper
-from pyfakefs.fake_open import FakeFileOpen
+from pyfakefs.fake_open import fake_open
 from pyfakefs.helpers import IS_PYPY
 
 if TYPE_CHECKING:
     from pyfakefs.fake_filesystem import FakeFilesystem
 
 
 class PatchMode(Enum):
@@ -88,47 +86,25 @@
         newline: Optional[str] = None,
         closefd: bool = True,
         opener: Optional[Callable] = None,
     ) -> Union[AnyFileWrapper, IO[Any]]:
         """Redirect the call to FakeFileOpen.
         See FakeFileOpen.call() for description.
         """
-        # workaround for built-in open called from skipped modules (see #552)
-        # as open is not imported explicitly, we cannot patch it for
-        # specific modules; instead we check if the caller is a skipped
-        # module (should work in most cases)
-        stack = traceback.extract_stack(limit=2)
-        # handle the case that we try to call the original `open_code`
-        # and get here instead (since Python 3.12)
-        from_open_code = (
-            sys.version_info >= (3, 12)
-            and stack[0].name == "open_code"
-            and stack[0].line == "return self._io_module.open_code(path)"
-        )
-        module_name = os.path.splitext(stack[0].filename)[0]
-        module_name = module_name.replace(os.sep, ".")
-        if from_open_code or any(
-            [
-                module_name == sn or module_name.endswith("." + sn)
-                for sn in self.skip_names
-            ]
-        ):
-            return io.open(  # pytype: disable=wrong-arg-count
-                file,
-                mode,
-                buffering,
-                encoding,
-                errors,
-                newline,
-                closefd,
-                opener,
-            )
-        fake_open = FakeFileOpen(self.filesystem)
         return fake_open(
-            file, mode, buffering, encoding, errors, newline, closefd, opener
+            self.filesystem,
+            self.skip_names,
+            file,
+            mode,
+            buffering,
+            encoding,
+            errors,
+            newline,
+            closefd,
+            opener,
         )
 
     if sys.version_info >= (3, 8):
 
         def open_code(self, path):
             """Redirect the call to open. Note that the behavior of the real
             function may be overridden by an earlier call to the
```

### Comparing `pyfakefs-5.4.1/pyfakefs/fake_open.py` & `pyfakefs-5.5.0/pyfakefs/fake_open.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,27 +11,32 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """A fake open() function replacement. See ``fake_filesystem`` for usage."""
 
 import errno
+import io
 import os
 import sys
+import traceback
 from stat import (
     S_ISDIR,
 )
 from typing import (
     Optional,
     Union,
     Any,
     Tuple,
     cast,
     AnyStr,
     TYPE_CHECKING,
+    Callable,
+    IO,
+    List,
 )
 
 from pyfakefs import helpers
 from pyfakefs.fake_file import (
     FakePipeWrapper,
     FakeFileWrapper,
     FakeFile,
@@ -59,14 +64,62 @@
     "w+": (False, True, True, True, False, False),
     "a+": (False, True, True, False, True, False),
     "x": (False, False, True, False, False, True),
     "x+": (False, True, True, False, False, True),
 }
 
 
+def fake_open(
+    filesystem: "FakeFilesystem",
+    skip_names: List[str],
+    file: Union[AnyStr, int],
+    mode: str = "r",
+    buffering: int = -1,
+    encoding: Optional[str] = None,
+    errors: Optional[str] = None,
+    newline: Optional[str] = None,
+    closefd: bool = True,
+    opener: Optional[Callable] = None,
+) -> Union[AnyFileWrapper, IO[Any]]:
+    """Redirect the call to FakeFileOpen.
+    See FakeFileOpen.call() for description.
+    """
+    # workaround for built-in open called from skipped modules (see #552)
+    # as open is not imported explicitly, we cannot patch it for
+    # specific modules; instead we check if the caller is a skipped
+    # module (should work in most cases)
+    stack = traceback.extract_stack(limit=3)
+    # handle the case that we try to call the original `open_code`
+    # and get here instead (since Python 3.12)
+    from_open_code = (
+        sys.version_info >= (3, 12)
+        and stack[0].name == "open_code"
+        and stack[0].line == "return self._io_module.open_code(path)"
+    )
+    module_name = os.path.splitext(stack[0].filename)[0]
+    module_name = module_name.replace(os.sep, ".")
+    if from_open_code or any(
+        [module_name == sn or module_name.endswith("." + sn) for sn in skip_names]
+    ):
+        return io.open(  # pytype: disable=wrong-arg-count
+            file,
+            mode,
+            buffering,
+            encoding,
+            errors,
+            newline,
+            closefd,
+            opener,
+        )
+    fake_file_open = FakeFileOpen(filesystem)
+    return fake_file_open(
+        file, mode, buffering, encoding, errors, newline, closefd, opener
+    )
+
+
 class FakeFileOpen:
     """Faked `file()` and `open()` function replacements.
 
     Returns FakeFile objects in a FakeFilesystem in place of the `file()`
     or `open()` function.
     """
 
@@ -284,15 +337,14 @@
                     )
                 )
             ):
                 self.filesystem.raise_os_error(errno.EACCES, file_path)
             if open_modes.can_write:
                 if open_modes.truncate:
                     file_object.set_contents("")
-            file_object
         else:
             if open_modes.must_exist:
                 self.filesystem.raise_os_error(errno.ENOENT, file_path)
             if self.filesystem.islink(file_path):
                 link_object = self.filesystem.resolve(file_path, follow_symlinks=False)
                 assert link_object.contents is not None
                 target_path = cast(
@@ -340,15 +392,15 @@
                 file_object,
                 cast(AnyStr, path),  # pytype: disable=invalid-annotation
                 filedes,
                 cast(AnyStr, path),  # pytype: disable=invalid-annotation
                 can_write,
             )
 
-        # open a file file by path
+        # open a file by path
         file_path = cast(AnyStr, file_)  # pytype: disable=invalid-annotation
         if file_path == self.filesystem.dev_null.name:
             file_object = self.filesystem.dev_null
             real_path = file_path
         else:
             real_path = self.filesystem.resolve_path(file_path)
             if self.filesystem.exists(file_path):
```

### Comparing `pyfakefs-5.4.1/pyfakefs/fake_os.py` & `pyfakefs-5.5.0/pyfakefs/fake_os.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,14 @@
     Tuple,
     cast,
     AnyStr,
     TYPE_CHECKING,
     Set,
 )
 
-from pyfakefs.extra_packages import use_scandir
 from pyfakefs.fake_file import (
     FakeDirectory,
     FakeDirWrapper,
     StandardStreamWrapper,
     FakeFileWrapper,
     FakePipeWrapper,
     FakeFile,
@@ -118,14 +117,15 @@
             "open",
             "read",
             "readlink",
             "remove",
             "removedirs",
             "rename",
             "rmdir",
+            "scandir",
             "stat",
             "symlink",
             "umask",
             "unlink",
             "utime",
             "walk",
             "write",
@@ -141,16 +141,14 @@
                 "setxattr",
             ]
         if sys.platform != "win32":
             _dir += [
                 "getgid",
                 "getuid",
             ]
-        if use_scandir:
-            _dir += ["scandir"]
         return _dir
 
     def __init__(self, filesystem: "FakeFilesystem"):
         """Also exposes self.path (to fake os.path).
 
         Args:
             filesystem: FakeFilesystem used to provide file system information
```

### Comparing `pyfakefs-5.4.1/pyfakefs/fake_path.py` & `pyfakefs-5.5.0/pyfakefs/fake_path.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.4.1/pyfakefs/fake_pathlib.py` & `pyfakefs-5.5.0/pyfakefs/fake_pathlib.py`

 * *Files 9% similar despite different names*

```diff
@@ -36,39 +36,61 @@
 import ntpath
 import os
 import pathlib
 import posixpath
 import re
 import sys
 from pathlib import PurePath
-from typing import Callable
+from typing import Callable, List
 from urllib.parse import quote_from_bytes as urlquote_from_bytes
 
 from pyfakefs import fake_scandir
-from pyfakefs.extra_packages import use_scandir
 from pyfakefs.fake_filesystem import FakeFilesystem
-from pyfakefs.fake_open import FakeFileOpen
+from pyfakefs.fake_open import FakeFileOpen, fake_open
 from pyfakefs.fake_os import FakeOsModule, use_original_os
 from pyfakefs.helpers import IS_PYPY
 
 
 def init_module(filesystem):
     """Initializes the fake module with the fake file system."""
     # pylint: disable=protected-access
     FakePath.filesystem = filesystem
     if sys.version_info < (3, 12):
-        FakePathlibModule.PureWindowsPath._flavour = _FakeWindowsFlavour(filesystem)
-        FakePathlibModule.PurePosixPath._flavour = _FakePosixFlavour(filesystem)
+        FakePathlibModule.WindowsPath._flavour = _FakeWindowsFlavour(filesystem)
+        FakePathlibModule.PosixPath._flavour = _FakePosixFlavour(filesystem)
+
+        # Pure POSIX path separators must be filesystem-independent.
+        fake_pure_posix_flavour = _FakePosixFlavour(filesystem)
+        fake_pure_posix_flavour.sep = "/"
+        fake_pure_posix_flavour.altsep = None
+        FakePathlibModule.PurePosixPath._flavour = fake_pure_posix_flavour
+
+        # Pure Windows path separators must be filesystem-independent.
+        fake_pure_nt_flavour = _FakePosixFlavour(filesystem)
+        fake_pure_nt_flavour.sep = "\\"
+        fake_pure_nt_flavour.altsep = "/"
+        FakePathlibModule.PureWindowsPath._flavour = fake_pure_nt_flavour
     else:
         # in Python 3.12, the flavour is no longer an own class,
         # but points to the os-specific path module (posixpath/ntpath)
         fake_os = FakeOsModule(filesystem)
-        fake_path = fake_os.path
-        FakePathlibModule.PureWindowsPath._flavour = fake_path
-        FakePathlibModule.PurePosixPath._flavour = fake_path
+        FakePathlibModule.PosixPath._flavour = fake_os.path
+        FakePathlibModule.WindowsPath._flavour = fake_os.path
+
+        # Pure POSIX path separators must be filesystem independent.
+        fake_pure_posix_os = FakeOsModule(filesystem)
+        fake_pure_posix_os.path.sep = "/"
+        fake_pure_posix_os.path.altsep = None
+        FakePathlibModule.PurePosixPath._flavour = fake_pure_posix_os.path
+
+        # Pure Windows path separators must be filesystem independent.
+        fake_pure_nt_os = FakeOsModule(filesystem)
+        fake_pure_nt_os.path.sep = "\\"
+        fake_pure_nt_os.path.altsep = "/"
+        FakePathlibModule.PureWindowsPath._flavour = fake_pure_nt_os.path
 
 
 def _wrap_strfunc(strfunc):
     @functools.wraps(strfunc)
     def _wrapped(pathobj, *args, **kwargs):
         return strfunc(pathobj.filesystem, str(pathobj), *args, **kwargs)
 
@@ -105,17 +127,15 @@
     stat = _wrap_strfunc(FakeFilesystem.stat)
 
     lstat = _wrap_strfunc(
         lambda fs, path: FakeFilesystem.stat(fs, path, follow_symlinks=False)
     )
 
     listdir = _wrap_strfunc(FakeFilesystem.listdir)
-
-    if use_scandir:
-        scandir = _wrap_strfunc(fake_scandir.scandir)
+    scandir = _wrap_strfunc(fake_scandir.scandir)
 
     if hasattr(os, "lchmod"):
         lchmod = _wrap_strfunc(
             lambda fs, path, mode: FakeFilesystem.chmod(
                 fs, path, mode, follow_symlinks=False
             )
         )
@@ -508,14 +528,15 @@
     fake filesystem. The rest of the methods work as they are, as they will
     use the fake accessor.
     New in pyfakefs 3.0.
     """
 
     # the underlying fake filesystem
     filesystem = None
+    skip_names: List[str] = []
 
     def __new__(cls, *args, **kwargs):
         """Creates the correct subclass based on OS."""
         if cls is FakePathlibModule.Path:
             cls = (
                 FakePathlibModule.WindowsPath
                 if cls.filesystem.is_windows_fs
@@ -607,16 +628,23 @@
         """Open the file pointed by this path and return a fake file object.
 
         Raises:
             OSError: if the target object is a directory, the path is invalid
                 or permission is denied.
         """
         self._raise_on_closed()
-        return FakeFileOpen(self.filesystem)(
-            self._path(), mode, buffering, encoding, errors, newline
+        return fake_open(
+            self.filesystem,
+            self.skip_names,
+            self._path(),
+            mode,
+            buffering,
+            encoding,
+            errors,
+            newline,
         )
 
     def read_bytes(self):
         """Open the fake file in bytes mode, read it, and close the file.
 
         Raises:
             OSError: if the target object is a directory, the path is
@@ -771,16 +799,14 @@
                 return False
             name = self._tail[-1].partition(".")[0].partition(":")[0].rstrip(" ")
             return name.upper() in pathlib._WIN_RESERVED_NAMES
 
 
 class FakePathlibModule:
     """Uses FakeFilesystem to provide a fake pathlib module replacement.
-    Can be used to replace both the standard `pathlib` module and the
-    `pathlib2` package available on PyPi.
 
     You need a fake_filesystem to use this:
     `filesystem = fake_filesystem.FakeFilesystem()`
     `fake_pathlib_module = fake_filesystem.FakePathlibModule(filesystem)`
     """
 
     def __init__(self, filesystem):
@@ -857,14 +883,23 @@
 
     fake_pathlib = None
 
     def __init__(self, filesystem=None):
         if self.fake_pathlib is None:
             self.__class__.fake_pathlib = FakePathlibModule(filesystem)
 
+    @property
+    def skip_names(self):
+        return []  # not used, here to allow a setter
+
+    @skip_names.setter
+    def skip_names(self, value):
+        # this is set from the patcher and passed to the fake Path class
+        self.fake_pathlib.Path.skip_names = value
+
     def __call__(self, *args, **kwargs):
         return self.fake_pathlib.Path(*args, **kwargs)
 
     def __getattr__(self, name):
         return getattr(self.fake_pathlib.Path, name)
 
     @classmethod
```

### Comparing `pyfakefs-5.4.1/pyfakefs/fake_scandir.py` & `pyfakefs-5.5.0/pyfakefs/fake_scandir.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,24 +16,18 @@
 and the standalone function available in the standalone `scandir` python
 package.
 """
 
 import os
 import sys
 
-from pyfakefs.extra_packages import use_scandir_package
 from pyfakefs.helpers import to_string, make_string_path
 
-if sys.version_info >= (3, 6):
-    BaseClass = os.PathLike
-else:
-    BaseClass = object
 
-
-class DirEntry(BaseClass):
+class DirEntry(os.PathLike):
     """Emulates os.DirEntry. Note that we did not enforce keyword only
     arguments."""
 
     def __init__(self, filesystem):
         """Initialize the dir entry with unset values.
 
         Args:
@@ -129,17 +123,15 @@
 class ScanDirIter:
     """Iterator for DirEntry objects returned from `scandir()`
     function."""
 
     def __init__(self, filesystem, path):
         self.filesystem = filesystem
         if isinstance(path, int):
-            if not use_scandir_package and (
-                sys.version_info < (3, 7) or self.filesystem.is_windows_fs
-            ):
+            if self.filesystem.is_windows_fs:
                 raise NotImplementedError(
                     "scandir does not support file descriptor " "path argument"
                 )
             self.abspath = self.filesystem.absnormpath(
                 self.filesystem.get_open_file(path).get_object().path
             )
             self.path = ""
@@ -259,65 +251,7 @@
                     continue
                 for contents in do_walk(path):
                     yield contents
             if not topdown:
                 yield top_contents
 
     return do_walk(make_string_path(to_string(top)), top_most=True)
-
-
-class FakeScanDirModule:
-    """Uses FakeFilesystem to provide a fake `scandir` module replacement.
-
-    .. Note:: The ``scandir`` function is a part of the standard ``os`` module
-      since Python 3.5. This class handles the separate ``scandir`` module
-      that is available on pypi.
-
-    You need a fake_filesystem to use this:
-    `filesystem = fake_filesystem.FakeFilesystem()`
-    `fake_scandir_module = fake_filesystem.FakeScanDirModule(filesystem)`
-    """
-
-    @staticmethod
-    def dir():
-        """Return the list of patched function names. Used for patching
-        functions imported from the module.
-        """
-        return "scandir", "walk"
-
-    def __init__(self, filesystem):
-        self.filesystem = filesystem
-
-    def scandir(self, path="."):
-        """Return an iterator of DirEntry objects corresponding to the entries
-        in the directory given by path.
-
-        Args:
-            path: Path to the target directory within the fake filesystem.
-
-        Returns:
-            an iterator to an unsorted list of os.DirEntry objects for
-            each entry in path.
-
-        Raises:
-            OSError: if the target is not a directory.
-        """
-        return scandir(self.filesystem, path)
-
-    def walk(self, top, topdown=True, onerror=None, followlinks=False):
-        """Perform a walk operation over the fake filesystem.
-
-        Args:
-            top: The root directory from which to begin walk.
-            topdown: Determines whether to return the tuples with the root as
-                the first entry (`True`) or as the last, after all the child
-                directory tuples (`False`).
-          onerror: If not `None`, function which will be called to handle the
-                `os.error` instance provided when `os.listdir()` fails.
-          followlinks: If `True`, symbolic links are followed.
-
-        Yields:
-            (path, directories, nondirectories) for top and each of its
-            subdirectories.  See the documentation for the builtin os module
-            for further details.
-        """
-        return walk(self.filesystem, top, topdown, onerror, followlinks)
```

### Comparing `pyfakefs-5.4.1/pyfakefs/helpers.py` & `pyfakefs-5.5.0/pyfakefs/helpers.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.4.1/pyfakefs/mox3_stubout.py` & `pyfakefs-5.5.0/pyfakefs/mox3_stubout.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.4.1/pyfakefs/patched_packages.py` & `pyfakefs-5.5.0/pyfakefs/patched_packages.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.4.1/pyfakefs/pytest_plugin.py` & `pyfakefs-5.5.0/pyfakefs/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.4.1/pyfakefs/pytest_tests/conftest.py` & `pyfakefs-5.5.0/pyfakefs/pytest_tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.4.1/pyfakefs/pytest_tests/example.py` & `pyfakefs-5.5.0/pyfakefs/pytest_tests/example.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.4.1/pyfakefs/pytest_tests/pytest_check_failed_plugin_test.py` & `pyfakefs-5.5.0/pyfakefs/pytest_tests/pytest_check_failed_plugin_test.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.4.1/pyfakefs/pytest_tests/pytest_doctest_test.py` & `pyfakefs-5.5.0/pyfakefs/pytest_tests/pytest_doctest_test.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.4.1/pyfakefs/pytest_tests/pytest_fixture_param_test.py` & `pyfakefs-5.5.0/pyfakefs/pytest_tests/pytest_fixture_param_test.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.4.1/pyfakefs/pytest_tests/pytest_fixture_test.py` & `pyfakefs-5.5.0/pyfakefs/pytest_tests/pytest_fixture_test.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.4.1/pyfakefs/pytest_tests/pytest_module_fixture_test.py` & `pyfakefs-5.5.0/pyfakefs/pytest_tests/pytest_module_fixture_test.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.4.1/pyfakefs/pytest_tests/pytest_plugin_test.py` & `pyfakefs-5.5.0/pyfakefs/pytest_tests/pytest_plugin_test.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.4.1/pyfakefs/pytest_tests/pytest_reload_pandas_test.py` & `pyfakefs-5.5.0/pyfakefs/pytest_tests/pytest_reload_pandas_test.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.4.1/pyfakefs/tests/all_tests.py` & `pyfakefs-5.5.0/pyfakefs/tests/all_tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,15 @@
     fake_filesystem_unittest_test,
     fake_filesystem_vs_real_test,
     fake_open_test,
     fake_os_test,
     fake_pathlib_test,
     fake_tempfile_test,
     patched_packages_test,
+    fake_legacy_modules_test,
     mox3_stubout_test,
 )
 
 
 class AllTests(unittest.TestSuite):
     """A test suite that runs all tests for pyfakefs at once."""
 
@@ -53,14 +54,15 @@
                 loader.loadTestsFromModule(fake_filesystem_vs_real_test),
                 loader.loadTestsFromModule(fake_filesystem_unittest_test),
                 loader.loadTestsFromModule(example_test),
                 loader.loadTestsFromModule(mox3_stubout_test),
                 loader.loadTestsFromModule(dynamic_patch_test),
                 loader.loadTestsFromModule(fake_pathlib_test),
                 loader.loadTestsFromModule(patched_packages_test),
+                loader.loadTestsFromModule(fake_legacy_modules_test),
             ]
         )
         return self
 
 
 if __name__ == "__main__":
     result = unittest.TextTestRunner(verbosity=2).run(AllTests().suite())
```

### Comparing `pyfakefs-5.4.1/pyfakefs/tests/all_tests_without_extra_packages.py` & `pyfakefs-5.5.0/pyfakefs/tests/all_tests_without_extra_packages.py`

 * *Files 24% similar despite different names*

```diff
@@ -12,23 +12,17 @@
 
 """A test suite that runs all tests for pyfakefs at once.
 Excludes tests using external scandir package."""
 
 import sys
 import unittest
 
-from pyfakefs import extra_packages
+from pyfakefs import legacy_packages
 
-if extra_packages.use_scandir_package:
-    extra_packages.use_scandir_package = False
-    try:
-        from os import scandir
-    except ImportError:
-        scandir = None
-    extra_packages.scandir = scandir
-    extra_packages.use_scandir = scandir
+legacy_packages.scandir = None
+legacy_packages.pathlib2 = None
 
 from pyfakefs.tests.all_tests import AllTests  # noqa: E402
 
 if __name__ == "__main__":
     result = unittest.TextTestRunner(verbosity=2).run(AllTests().suite())
     sys.exit(int(not result.wasSuccessful()))
```

### Comparing `pyfakefs-5.4.1/pyfakefs/tests/dynamic_patch_test.py` & `pyfakefs-5.5.0/pyfakefs/tests/dynamic_patch_test.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.4.1/pyfakefs/tests/example.py` & `pyfakefs-5.5.0/pyfakefs/tests/example.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.4.1/pyfakefs/tests/example_test.py` & `pyfakefs-5.5.0/pyfakefs/tests/example_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 import io
 import os
 import sys
 import unittest
 
 from pyfakefs import fake_filesystem_unittest
-from pyfakefs.extra_packages import use_scandir_package
+from pyfakefs.legacy_packages import scandir
 from pyfakefs.tests import example  # The module under test
 
 
 def load_tests(loader, tests, ignore):
     """Load the pyfakefs/example.py doctest tests into unittest."""
     return fake_filesystem_unittest.load_doctests(loader, tests, ignore, example)
 
@@ -139,17 +139,15 @@
         entries = sorted(example.scan_dir("/test"), key=lambda e: e.name)
         self.assertEqual(3, len(entries))
         self.assertEqual("linked_file", entries[1].name)
         self.assertTrue(entries[0].is_dir())
         self.assertTrue(entries[1].is_symlink())
         self.assertTrue(entries[2].is_file())
 
-    @unittest.skipIf(
-        not use_scandir_package, "Testing only if scandir module is installed"
-    )
+    @unittest.skipIf(scandir is None, "Testing only if scandir module is installed")
     def test_scandir_scandir(self):
         """Test example.scandir() which uses `scandir.scandir()`.
 
         The scandir module has been replaced with the fake_scandir module so
         the fake filesystem path entries are returned instead of
         `scandir.DirEntry` objects.
         """
```

### Comparing `pyfakefs-5.4.1/pyfakefs/tests/fake_filesystem_glob_test.py` & `pyfakefs-5.5.0/pyfakefs/tests/fake_filesystem_glob_test.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.4.1/pyfakefs/tests/fake_filesystem_shutil_test.py` & `pyfakefs-5.5.0/pyfakefs/tests/fake_filesystem_shutil_test.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.4.1/pyfakefs/tests/fake_filesystem_test.py` & `pyfakefs-5.5.0/pyfakefs/tests/fake_filesystem_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -5531,1357 +5531,1345 @@
 000159a0: 656c 662e 6669 6c65 7379 7374 656d 2e61  elf.filesystem.a
 000159b0: 6464 5f72 6561 6c5f 6669 6c65 2872 6561  dd_real_file(rea
 000159c0: 6c5f 6669 6c65 5f70 6174 6829 0a0a 2020  l_file_path)..  
 000159d0: 2020 4063 6f6e 7465 7874 6c69 622e 636f    @contextlib.co
 000159e0: 6e74 6578 746d 616e 6167 6572 0a20 2020  ntextmanager.   
 000159f0: 2064 6566 2063 7265 6174 655f 7265 616c   def create_real
 00015a00: 5f70 6174 6873 2873 656c 6629 3a0a 2020  _paths(self):.  
-00015a10: 2020 2020 2020 7265 616c 5f64 6972 5f72        real_dir_r
-00015a20: 6f6f 7420 3d20 6f73 2e70 6174 682e 6a6f  oot = os.path.jo
-00015a30: 696e 2874 656d 7066 696c 652e 6765 7474  in(tempfile.gett
-00015a40: 656d 7064 6972 2829 2c20 2272 6f6f 7422  empdir(), "root"
-00015a50: 290a 2020 2020 2020 2020 7472 793a 0a20  ).        try:. 
-00015a60: 2020 2020 2020 2020 2020 2066 6f72 2064             for d
-00015a70: 6972 5f6e 616d 6520 696e 2028 2266 6f6f  ir_name in ("foo
-00015a80: 222c 2022 6261 7222 293a 0a20 2020 2020  ", "bar"):.     
-00015a90: 2020 2020 2020 2020 2020 2072 6561 6c5f             real_
-00015aa0: 6469 7220 3d20 6f73 2e70 6174 682e 6a6f  dir = os.path.jo
-00015ab0: 696e 2872 6561 6c5f 6469 725f 726f 6f74  in(real_dir_root
-00015ac0: 2c20 6469 725f 6e61 6d65 290a 2020 2020  , dir_name).    
-00015ad0: 2020 2020 2020 2020 2020 2020 6f73 2e6d              os.m
-00015ae0: 616b 6564 6972 7328 7265 616c 5f64 6972  akedirs(real_dir
-00015af0: 2c20 6578 6973 745f 6f6b 3d54 7275 6529  , exist_ok=True)
-00015b00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00015b10: 2077 6974 6820 6f70 656e 280a 2020 2020   with open(.    
-00015b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015b30: 6f73 2e70 6174 682e 6a6f 696e 2872 6561  os.path.join(rea
-00015b40: 6c5f 6469 722c 2022 7465 7374 2e74 7874  l_dir, "test.txt
-00015b50: 2229 2c20 2277 222c 2065 6e63 6f64 696e  "), "w", encodin
-00015b60: 673d 2275 7466 3822 0a20 2020 2020 2020  g="utf8".       
-00015b70: 2020 2020 2020 2020 2029 2061 7320 663a           ) as f:
-00015b80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00015b90: 2020 2020 2066 2e77 7269 7465 2822 7465       f.write("te
-00015ba0: 7374 2229 0a20 2020 2020 2020 2020 2020  st").           
-00015bb0: 2020 2020 2073 7562 5f64 6972 203d 206f       sub_dir = o
-00015bc0: 732e 7061 7468 2e6a 6f69 6e28 7265 616c  s.path.join(real
-00015bd0: 5f64 6972 2c20 2273 7562 2229 0a20 2020  _dir, "sub").   
-00015be0: 2020 2020 2020 2020 2020 2020 206f 732e               os.
-00015bf0: 6d61 6b65 6469 7273 2873 7562 5f64 6972  makedirs(sub_dir
-00015c00: 2c20 6578 6973 745f 6f6b 3d54 7275 6529  , exist_ok=True)
-00015c10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00015c20: 2077 6974 6820 6f70 656e 286f 732e 7061   with open(os.pa
-00015c30: 7468 2e6a 6f69 6e28 7375 625f 6469 722c  th.join(sub_dir,
-00015c40: 2022 7375 622e 7478 7422 292c 2022 7722   "sub.txt"), "w"
-00015c50: 2c20 656e 636f 6469 6e67 3d22 7574 6638  , encoding="utf8
-00015c60: 2229 2061 7320 663a 0a20 2020 2020 2020  ") as f:.       
-00015c70: 2020 2020 2020 2020 2020 2020 2066 2e77               f.w
-00015c80: 7269 7465 2822 7375 6222 290a 2020 2020  rite("sub").    
-00015c90: 2020 2020 2020 2020 7969 656c 6420 7265          yield re
-00015ca0: 616c 5f64 6972 5f72 6f6f 740a 2020 2020  al_dir_root.    
-00015cb0: 2020 2020 6669 6e61 6c6c 793a 0a20 2020      finally:.   
-00015cc0: 2020 2020 2020 2020 2073 6875 7469 6c2e           shutil.
-00015cd0: 726d 7472 6565 2872 6561 6c5f 6469 725f  rmtree(real_dir_
-00015ce0: 726f 6f74 2c20 6967 6e6f 7265 5f65 7272  root, ignore_err
-00015cf0: 6f72 733d 5472 7565 290a 0a20 2020 2064  ors=True)..    d
-00015d00: 6566 2074 6573 745f 6578 6973 7469 6e67  ef test_existing
-00015d10: 5f66 616b 655f 6469 7265 6374 6f72 795f  _fake_directory_
-00015d20: 6973 5f6d 6572 6765 645f 6c61 7a69 6c79  is_merged_lazily
-00015d30: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-00015d40: 7365 6c66 2e66 696c 6573 7973 7465 6d2e  self.filesystem.
-00015d50: 6372 6561 7465 5f66 696c 6528 6f73 2e70  create_file(os.p
-00015d60: 6174 682e 6a6f 696e 2822 2f22 2c20 2272  ath.join("/", "r
-00015d70: 6f6f 7422 2c20 2266 6f6f 222c 2022 7465  oot", "foo", "te
-00015d80: 7374 312e 7478 7422 2929 0a20 2020 2020  st1.txt")).     
-00015d90: 2020 2073 656c 662e 6669 6c65 7379 7374     self.filesyst
-00015da0: 656d 2e63 7265 6174 655f 6469 7228 6f73  em.create_dir(os
-00015db0: 2e70 6174 682e 6a6f 696e 2822 726f 6f74  .path.join("root
-00015dc0: 222c 2022 6261 7a22 2929 0a20 2020 2020  ", "baz")).     
-00015dd0: 2020 2077 6974 6820 7365 6c66 2e63 7265     with self.cre
-00015de0: 6174 655f 7265 616c 5f70 6174 6873 2829  ate_real_paths()
-00015df0: 2061 7320 726f 6f74 5f64 6972 3a0a 2020   as root_dir:.  
-00015e00: 2020 2020 2020 2020 2020 7365 6c66 2e66            self.f
-00015e10: 696c 6573 7973 7465 6d2e 6164 645f 7265  ilesystem.add_re
-00015e20: 616c 5f64 6972 6563 746f 7279 2872 6f6f  al_directory(roo
-00015e30: 745f 6469 722c 2074 6172 6765 745f 7061  t_dir, target_pa
-00015e40: 7468 3d22 2f72 6f6f 7422 290a 2020 2020  th="/root").    
-00015e50: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-00015e60: 6572 7454 7275 6528 0a20 2020 2020 2020  ertTrue(.       
-00015e70: 2020 2020 2020 2020 2073 656c 662e 6669           self.fi
-00015e80: 6c65 7379 7374 656d 2e65 7869 7374 7328  lesystem.exists(
-00015e90: 6f73 2e70 6174 682e 6a6f 696e 2822 726f  os.path.join("ro
-00015ea0: 6f74 222c 2022 666f 6f22 2c20 2274 6573  ot", "foo", "tes
-00015eb0: 742e 7478 7422 2929 0a20 2020 2020 2020  t.txt")).       
-00015ec0: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
-00015ed0: 2020 2073 656c 662e 6173 7365 7274 5472     self.assertTr
-00015ee0: 7565 280a 2020 2020 2020 2020 2020 2020  ue(.            
-00015ef0: 2020 2020 7365 6c66 2e66 696c 6573 7973      self.filesys
-00015f00: 7465 6d2e 6578 6973 7473 286f 732e 7061  tem.exists(os.pa
-00015f10: 7468 2e6a 6f69 6e28 2272 6f6f 7422 2c20  th.join("root", 
-00015f20: 2266 6f6f 222c 2022 7465 7374 312e 7478  "foo", "test1.tx
-00015f30: 7422 2929 0a20 2020 2020 2020 2020 2020  t")).           
-00015f40: 2029 0a20 2020 2020 2020 2020 2020 2073   ).            s
-00015f50: 656c 662e 6173 7365 7274 5472 7565 280a  elf.assertTrue(.
-00015f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015f70: 7365 6c66 2e66 696c 6573 7973 7465 6d2e  self.filesystem.
-00015f80: 6578 6973 7473 286f 732e 7061 7468 2e6a  exists(os.path.j
-00015f90: 6f69 6e28 2272 6f6f 7422 2c20 2262 6172  oin("root", "bar
-00015fa0: 222c 2022 7375 6222 2c20 2273 7562 2e74  ", "sub", "sub.t
-00015fb0: 7874 2229 290a 2020 2020 2020 2020 2020  xt")).          
-00015fc0: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
-00015fd0: 7365 6c66 2e61 7373 6572 7454 7275 6528  self.assertTrue(
-00015fe0: 7365 6c66 2e66 696c 6573 7973 7465 6d2e  self.filesystem.
-00015ff0: 6578 6973 7473 286f 732e 7061 7468 2e6a  exists(os.path.j
-00016000: 6f69 6e28 2272 6f6f 7422 2c20 2262 617a  oin("root", "baz
-00016010: 2229 2929 0a0a 2020 2020 6465 6620 7465  ")))..    def te
-00016020: 7374 5f65 7869 7374 696e 675f 6661 6b65  st_existing_fake
-00016030: 5f64 6972 6563 746f 7279 5f69 735f 6d65  _directory_is_me
-00016040: 7267 6564 2873 656c 6629 3a0a 2020 2020  rged(self):.    
-00016050: 2020 2020 7365 6c66 2e66 696c 6573 7973      self.filesys
-00016060: 7465 6d2e 6372 6561 7465 5f66 696c 6528  tem.create_file(
-00016070: 6f73 2e70 6174 682e 6a6f 696e 2822 2f22  os.path.join("/"
-00016080: 2c20 2272 6f6f 7422 2c20 2266 6f6f 222c  , "root", "foo",
-00016090: 2022 7465 7374 312e 7478 7422 2929 0a20   "test1.txt")). 
-000160a0: 2020 2020 2020 2073 656c 662e 6669 6c65         self.file
-000160b0: 7379 7374 656d 2e63 7265 6174 655f 6469  system.create_di
-000160c0: 7228 6f73 2e70 6174 682e 6a6f 696e 2822  r(os.path.join("
-000160d0: 726f 6f74 222c 2022 6261 7a22 2929 0a20  root", "baz")). 
-000160e0: 2020 2020 2020 2077 6974 6820 7365 6c66         with self
-000160f0: 2e63 7265 6174 655f 7265 616c 5f70 6174  .create_real_pat
-00016100: 6873 2829 2061 7320 726f 6f74 5f64 6972  hs() as root_dir
-00016110: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00016120: 6c66 2e66 696c 6573 7973 7465 6d2e 6164  lf.filesystem.ad
-00016130: 645f 7265 616c 5f64 6972 6563 746f 7279  d_real_directory
-00016140: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00016150: 2020 726f 6f74 5f64 6972 2c20 7461 7267    root_dir, targ
-00016160: 6574 5f70 6174 683d 222f 726f 6f74 222c  et_path="/root",
-00016170: 206c 617a 795f 7265 6164 3d46 616c 7365   lazy_read=False
-00016180: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
-00016190: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000161a0: 6173 7365 7274 5472 7565 280a 2020 2020  assertTrue(.    
-000161b0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000161c0: 2e66 696c 6573 7973 7465 6d2e 6578 6973  .filesystem.exis
-000161d0: 7473 286f 732e 7061 7468 2e6a 6f69 6e28  ts(os.path.join(
-000161e0: 2272 6f6f 7422 2c20 2266 6f6f 222c 2022  "root", "foo", "
-000161f0: 7465 7374 2e74 7874 2229 290a 2020 2020  test.txt")).    
-00016200: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00016210: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
-00016220: 7454 7275 6528 0a20 2020 2020 2020 2020  tTrue(.         
-00016230: 2020 2020 2020 2073 656c 662e 6669 6c65         self.file
-00016240: 7379 7374 656d 2e65 7869 7374 7328 6f73  system.exists(os
-00016250: 2e70 6174 682e 6a6f 696e 2822 726f 6f74  .path.join("root
-00016260: 222c 2022 666f 6f22 2c20 2274 6573 7431  ", "foo", "test1
-00016270: 2e74 7874 2229 290a 2020 2020 2020 2020  .txt")).        
-00016280: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-00016290: 2020 7365 6c66 2e61 7373 6572 7454 7275    self.assertTru
-000162a0: 6528 0a20 2020 2020 2020 2020 2020 2020  e(.             
-000162b0: 2020 2073 656c 662e 6669 6c65 7379 7374     self.filesyst
-000162c0: 656d 2e65 7869 7374 7328 6f73 2e70 6174  em.exists(os.pat
-000162d0: 682e 6a6f 696e 2822 726f 6f74 222c 2022  h.join("root", "
-000162e0: 6261 7222 2c20 2273 7562 222c 2022 7375  bar", "sub", "su
-000162f0: 622e 7478 7422 2929 0a20 2020 2020 2020  b.txt")).       
-00016300: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
-00016310: 2020 2073 656c 662e 6173 7365 7274 5472     self.assertTr
-00016320: 7565 2873 656c 662e 6669 6c65 7379 7374  ue(self.filesyst
-00016330: 656d 2e65 7869 7374 7328 6f73 2e70 6174  em.exists(os.pat
-00016340: 682e 6a6f 696e 2822 726f 6f74 222c 2022  h.join("root", "
-00016350: 6261 7a22 2929 290a 0a20 2020 2064 6566  baz")))..    def
-00016360: 2074 6573 745f 6661 6b65 5f66 696c 6573   test_fake_files
-00016370: 5f63 616e 6e6f 745f 6265 5f6f 7665 7277  _cannot_be_overw
-00016380: 7269 7474 656e 2873 656c 6629 3a0a 2020  ritten(self):.  
-00016390: 2020 2020 2020 7365 6c66 2e66 696c 6573        self.files
-000163a0: 7973 7465 6d2e 6372 6561 7465 5f66 696c  ystem.create_fil
-000163b0: 6528 6f73 2e70 6174 682e 6a6f 696e 2822  e(os.path.join("
-000163c0: 2f22 2c20 2272 6f6f 7422 2c20 2266 6f6f  /", "root", "foo
-000163d0: 222c 2022 7465 7374 2e74 7874 2229 290a  ", "test.txt")).
-000163e0: 2020 2020 2020 2020 7769 7468 2073 656c          with sel
-000163f0: 662e 6372 6561 7465 5f72 6561 6c5f 7061  f.create_real_pa
-00016400: 7468 7328 2920 6173 2072 6f6f 745f 6469  ths() as root_di
-00016410: 723a 0a20 2020 2020 2020 2020 2020 2077  r:.            w
-00016420: 6974 6820 7365 6c66 2e72 6169 7365 735f  ith self.raises_
-00016430: 6f73 5f65 7272 6f72 2865 7272 6e6f 2e45  os_error(errno.E
-00016440: 4558 4953 5429 3a0a 2020 2020 2020 2020  EXIST):.        
-00016450: 2020 2020 2020 2020 7365 6c66 2e66 696c          self.fil
-00016460: 6573 7973 7465 6d2e 6164 645f 7265 616c  esystem.add_real
-00016470: 5f64 6972 6563 746f 7279 2872 6f6f 745f  _directory(root_
-00016480: 6469 722c 2074 6172 6765 745f 7061 7468  dir, target_path
-00016490: 3d22 2f72 6f6f 7422 290a 0a20 2020 2064  ="/root")..    d
-000164a0: 6566 2074 6573 745f 6361 6e6e 6f74 5f6f  ef test_cannot_o
-000164b0: 7665 7277 7269 7465 5f66 696c 655f 7769  verwrite_file_wi
-000164c0: 7468 5f64 6972 2873 656c 6629 3a0a 2020  th_dir(self):.  
-000164d0: 2020 2020 2020 7365 6c66 2e66 696c 6573        self.files
-000164e0: 7973 7465 6d2e 6372 6561 7465 5f66 696c  ystem.create_fil
-000164f0: 6528 6f73 2e70 6174 682e 6a6f 696e 2822  e(os.path.join("
-00016500: 2f22 2c20 2272 6f6f 7422 2c20 2266 6f6f  /", "root", "foo
-00016510: 2229 290a 2020 2020 2020 2020 7769 7468  ")).        with
-00016520: 2073 656c 662e 6372 6561 7465 5f72 6561   self.create_rea
-00016530: 6c5f 7061 7468 7328 2920 6173 2072 6f6f  l_paths() as roo
-00016540: 745f 6469 723a 0a20 2020 2020 2020 2020  t_dir:.         
-00016550: 2020 2077 6974 6820 7365 6c66 2e72 6169     with self.rai
-00016560: 7365 735f 6f73 5f65 7272 6f72 2865 7272  ses_os_error(err
-00016570: 6e6f 2e45 4e4f 5444 4952 293a 0a20 2020  no.ENOTDIR):.   
-00016580: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00016590: 662e 6669 6c65 7379 7374 656d 2e61 6464  f.filesystem.add
-000165a0: 5f72 6561 6c5f 6469 7265 6374 6f72 7928  _real_directory(
-000165b0: 726f 6f74 5f64 6972 2c20 7461 7267 6574  root_dir, target
-000165c0: 5f70 6174 683d 222f 726f 6f74 2f22 290a  _path="/root/").
-000165d0: 0a20 2020 2064 6566 2074 6573 745f 6361  .    def test_ca
-000165e0: 6e6e 6f74 5f6f 7665 7277 7269 7465 5f73  nnot_overwrite_s
-000165f0: 796d 6c69 6e6b 5f77 6974 685f 6469 7228  ymlink_with_dir(
-00016600: 7365 6c66 293a 0a20 2020 2020 2020 2073  self):.        s
-00016610: 656c 662e 6669 6c65 7379 7374 656d 2e63  elf.filesystem.c
-00016620: 7265 6174 655f 7379 6d6c 696e 6b28 0a20  reate_symlink(. 
-00016630: 2020 2020 2020 2020 2020 206f 732e 7061             os.pa
-00016640: 7468 2e6a 6f69 6e28 222f 222c 2022 726f  th.join("/", "ro
-00016650: 6f74 222c 2022 666f 6f22 292c 206f 732e  ot", "foo"), os.
-00016660: 7061 7468 2e6a 6f69 6e28 222f 222c 2022  path.join("/", "
-00016670: 726f 6f74 222c 2022 6c69 6e6b 2229 0a20  root", "link"). 
-00016680: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-00016690: 2077 6974 6820 7365 6c66 2e63 7265 6174   with self.creat
-000166a0: 655f 7265 616c 5f70 6174 6873 2829 2061  e_real_paths() a
-000166b0: 7320 726f 6f74 5f64 6972 3a0a 2020 2020  s root_dir:.    
-000166c0: 2020 2020 2020 2020 7769 7468 2073 656c          with sel
-000166d0: 662e 7261 6973 6573 5f6f 735f 6572 726f  f.raises_os_erro
-000166e0: 7228 6572 726e 6f2e 4545 5849 5354 293a  r(errno.EEXIST):
-000166f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016700: 2073 656c 662e 6669 6c65 7379 7374 656d   self.filesystem
-00016710: 2e61 6464 5f72 6561 6c5f 6469 7265 6374  .add_real_direct
-00016720: 6f72 7928 726f 6f74 5f64 6972 2c20 7461  ory(root_dir, ta
-00016730: 7267 6574 5f70 6174 683d 222f 726f 6f74  rget_path="/root
-00016740: 2f22 290a 0a20 2020 2064 6566 2074 6573  /")..    def tes
-00016750: 745f 7379 6d6c 696e 6b5f 6973 5f6d 6572  t_symlink_is_mer
-00016760: 6765 6428 7365 6c66 293a 0a20 2020 2020  ged(self):.     
-00016770: 2020 2073 656c 662e 736b 6970 5f69 665f     self.skip_if_
-00016780: 7379 6d6c 696e 6b5f 6e6f 745f 7375 7070  symlink_not_supp
-00016790: 6f72 7465 6428 666f 7263 655f 7265 616c  orted(force_real
-000167a0: 5f66 733d 5472 7565 290a 2020 2020 2020  _fs=True).      
-000167b0: 2020 7365 6c66 2e66 696c 6573 7973 7465    self.filesyste
-000167c0: 6d2e 6372 6561 7465 5f64 6972 286f 732e  m.create_dir(os.
-000167d0: 7061 7468 2e6a 6f69 6e28 222f 222c 2022  path.join("/", "
-000167e0: 726f 6f74 222c 2022 666f 6f22 2929 0a20  root", "foo")). 
-000167f0: 2020 2020 2020 2077 6974 6820 7365 6c66         with self
-00016800: 2e63 7265 6174 655f 7265 616c 5f70 6174  .create_real_pat
-00016810: 6873 2829 2061 7320 726f 6f74 5f64 6972  hs() as root_dir
-00016820: 3a0a 2020 2020 2020 2020 2020 2020 6c69  :.            li
-00016830: 6e6b 5f70 6174 6820 3d20 6f73 2e70 6174  nk_path = os.pat
-00016840: 682e 6a6f 696e 2872 6f6f 745f 6469 722c  h.join(root_dir,
-00016850: 2022 6c69 6e6b 2e74 7874 2229 0a20 2020   "link.txt").   
-00016860: 2020 2020 2020 2020 2074 6172 6765 745f           target_
-00016870: 7061 7468 203d 206f 732e 7061 7468 2e6a  path = os.path.j
-00016880: 6f69 6e28 2266 6f6f 222c 2022 7375 6222  oin("foo", "sub"
-00016890: 2c20 2273 7562 2e74 7874 2229 0a20 2020  , "sub.txt").   
-000168a0: 2020 2020 2020 2020 206f 732e 7379 6d6c           os.syml
-000168b0: 696e 6b28 7461 7267 6574 5f70 6174 682c  ink(target_path,
-000168c0: 206c 696e 6b5f 7061 7468 290a 2020 2020   link_path).    
-000168d0: 2020 2020 2020 2020 7365 6c66 2e66 696c          self.fil
-000168e0: 6573 7973 7465 6d2e 6164 645f 7265 616c  esystem.add_real
-000168f0: 5f64 6972 6563 746f 7279 2872 6f6f 745f  _directory(root_
-00016900: 6469 722c 2074 6172 6765 745f 7061 7468  dir, target_path
-00016910: 3d22 2f72 6f6f 7422 290a 2020 2020 2020  ="/root").      
-00016920: 2020 2020 2020 6661 6b65 5f6c 696e 6b5f        fake_link_
-00016930: 7061 7468 203d 206f 732e 7061 7468 2e6a  path = os.path.j
-00016940: 6f69 6e28 222f 222c 2022 726f 6f74 222c  oin("/", "root",
-00016950: 2022 6c69 6e6b 2e74 7874 2229 0a20 2020   "link.txt").   
-00016960: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
-00016970: 7365 7274 5472 7565 2873 656c 662e 6669  sertTrue(self.fi
-00016980: 6c65 7379 7374 656d 2e65 7869 7374 7328  lesystem.exists(
-00016990: 6661 6b65 5f6c 696e 6b5f 7061 7468 2929  fake_link_path))
-000169a0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-000169b0: 662e 6173 7365 7274 5472 7565 2873 656c  f.assertTrue(sel
-000169c0: 662e 6669 6c65 7379 7374 656d 2e69 736c  f.filesystem.isl
-000169d0: 696e 6b28 6661 6b65 5f6c 696e 6b5f 7061  ink(fake_link_pa
-000169e0: 7468 2929 0a0a 2020 2020 6465 6620 6368  th))..    def ch
-000169f0: 6563 6b5f 6661 6b65 5f66 696c 655f 7374  eck_fake_file_st
-00016a00: 6174 2873 656c 662c 2066 616b 655f 6669  at(self, fake_fi
-00016a10: 6c65 2c20 7265 616c 5f66 696c 655f 7061  le, real_file_pa
-00016a20: 7468 2c20 7461 7267 6574 5f70 6174 683d  th, target_path=
-00016a30: 4e6f 6e65 293a 0a20 2020 2020 2020 2069  None):.        i
-00016a40: 6620 7461 7267 6574 5f70 6174 6820 6973  f target_path is
-00016a50: 204e 6f6e 6520 6f72 2074 6172 6765 745f   None or target_
-00016a60: 7061 7468 203d 3d20 7265 616c 5f66 696c  path == real_fil
-00016a70: 655f 7061 7468 3a0a 2020 2020 2020 2020  e_path:.        
-00016a80: 2020 2020 7365 6c66 2e61 7373 6572 7454      self.assertT
-00016a90: 7275 6528 7365 6c66 2e66 696c 6573 7973  rue(self.filesys
-00016aa0: 7465 6d2e 6578 6973 7473 2872 6561 6c5f  tem.exists(real_
-00016ab0: 6669 6c65 5f70 6174 6829 290a 2020 2020  file_path)).    
-00016ac0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00016ad0: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
-00016ae0: 7446 616c 7365 2873 656c 662e 6669 6c65  tFalse(self.file
-00016af0: 7379 7374 656d 2e65 7869 7374 7328 7265  system.exists(re
-00016b00: 616c 5f66 696c 655f 7061 7468 2929 0a20  al_file_path)). 
-00016b10: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00016b20: 6173 7365 7274 5472 7565 2873 656c 662e  assertTrue(self.
-00016b30: 6669 6c65 7379 7374 656d 2e65 7869 7374  filesystem.exist
-00016b40: 7328 7461 7267 6574 5f70 6174 6829 290a  s(target_path)).
-00016b50: 0a20 2020 2020 2020 2072 6561 6c5f 7374  .        real_st
-00016b60: 6174 203d 206f 732e 7374 6174 2872 6561  at = os.stat(rea
-00016b70: 6c5f 6669 6c65 5f70 6174 6829 0a20 2020  l_file_path).   
-00016b80: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-00016b90: 4973 4e6f 6e65 2866 616b 655f 6669 6c65  IsNone(fake_file
-00016ba0: 2e5f 6279 7465 5f63 6f6e 7465 6e74 7329  ._byte_contents)
-00016bb0: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
-00016bc0: 7365 7274 4571 7561 6c28 6661 6b65 5f66  sertEqual(fake_f
-00016bd0: 696c 652e 7374 5f73 697a 652c 2072 6561  ile.st_size, rea
-00016be0: 6c5f 7374 6174 2e73 745f 7369 7a65 290a  l_stat.st_size).
-00016bf0: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-00016c00: 6572 7441 6c6d 6f73 7445 7175 616c 2866  ertAlmostEqual(f
-00016c10: 616b 655f 6669 6c65 2e73 745f 6374 696d  ake_file.st_ctim
-00016c20: 652c 2072 6561 6c5f 7374 6174 2e73 745f  e, real_stat.st_
-00016c30: 6374 696d 652c 2070 6c61 6365 733d 3529  ctime, places=5)
-00016c40: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
-00016c50: 7365 7274 416c 6d6f 7374 4571 7561 6c28  sertAlmostEqual(
-00016c60: 6661 6b65 5f66 696c 652e 7374 5f61 7469  fake_file.st_ati
-00016c70: 6d65 2c20 7265 616c 5f73 7461 742e 7374  me, real_stat.st
-00016c80: 5f61 7469 6d65 2c20 706c 6163 6573 3d35  _atime, places=5
-00016c90: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
-00016ca0: 7373 6572 7441 6c6d 6f73 7445 7175 616c  ssertAlmostEqual
-00016cb0: 2866 616b 655f 6669 6c65 2e73 745f 6d74  (fake_file.st_mt
-00016cc0: 696d 652c 2072 6561 6c5f 7374 6174 2e73  ime, real_stat.s
-00016cd0: 745f 6d74 696d 652c 2070 6c61 6365 733d  t_mtime, places=
-00016ce0: 3529 0a20 2020 2020 2020 2073 656c 662e  5).        self.
-00016cf0: 6173 7365 7274 4571 7561 6c28 6661 6b65  assertEqual(fake
-00016d00: 5f66 696c 652e 7374 5f75 6964 2c20 7265  _file.st_uid, re
-00016d10: 616c 5f73 7461 742e 7374 5f75 6964 290a  al_stat.st_uid).
-00016d20: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-00016d30: 6572 7445 7175 616c 2866 616b 655f 6669  ertEqual(fake_fi
-00016d40: 6c65 2e73 745f 6769 642c 2072 6561 6c5f  le.st_gid, real_
-00016d50: 7374 6174 2e73 745f 6769 6429 0a0a 2020  stat.st_gid)..  
-00016d60: 2020 6465 6620 6368 6563 6b5f 7265 6164    def check_read
-00016d70: 5f6f 6e6c 795f 6669 6c65 2873 656c 662c  _only_file(self,
-00016d80: 2066 616b 655f 6669 6c65 2c20 7265 616c   fake_file, real
-00016d90: 5f66 696c 655f 7061 7468 293a 0a20 2020  _file_path):.   
-00016da0: 2020 2020 2077 6974 6820 6f70 656e 2872       with open(r
-00016db0: 6561 6c5f 6669 6c65 5f70 6174 682c 2022  eal_file_path, "
-00016dc0: 7262 2229 2061 7320 663a 0a20 2020 2020  rb") as f:.     
-00016dd0: 2020 2020 2020 2072 6561 6c5f 636f 6e74         real_cont
-00016de0: 656e 7473 203d 2066 2e72 6561 6428 290a  ents = f.read().
-00016df0: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-00016e00: 6572 7445 7175 616c 2866 616b 655f 6669  ertEqual(fake_fi
-00016e10: 6c65 2e62 7974 655f 636f 6e74 656e 7473  le.byte_contents
-00016e20: 2c20 7265 616c 5f63 6f6e 7465 6e74 7329  , real_contents)
-00016e30: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
-00016e40: 6973 5f72 6f6f 7428 293a 0a20 2020 2020  is_root():.     
-00016e50: 2020 2020 2020 2077 6974 6820 7365 6c66         with self
-00016e60: 2e72 6169 7365 735f 6f73 5f65 7272 6f72  .raises_os_error
-00016e70: 2865 7272 6e6f 2e45 4143 4345 5329 3a0a  (errno.EACCES):.
-00016e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016e90: 7365 6c66 2e66 616b 655f 6f70 656e 2872  self.fake_open(r
-00016ea0: 6561 6c5f 6669 6c65 5f70 6174 682c 2022  eal_file_path, "
-00016eb0: 7722 290a 2020 2020 2020 2020 656c 7365  w").        else
-00016ec0: 3a0a 2020 2020 2020 2020 2020 2020 7769  :.            wi
-00016ed0: 7468 2073 656c 662e 6661 6b65 5f6f 7065  th self.fake_ope
-00016ee0: 6e28 7265 616c 5f66 696c 655f 7061 7468  n(real_file_path
-00016ef0: 2c20 2277 2229 3a0a 2020 2020 2020 2020  , "w"):.        
-00016f00: 2020 2020 2020 2020 7061 7373 0a0a 2020          pass..  
-00016f10: 2020 6465 6620 6368 6563 6b5f 7772 6974    def check_writ
-00016f20: 6162 6c65 5f66 696c 6528 7365 6c66 2c20  able_file(self, 
-00016f30: 6661 6b65 5f66 696c 652c 2072 6561 6c5f  fake_file, real_
-00016f40: 6669 6c65 5f70 6174 6829 3a0a 2020 2020  file_path):.    
-00016f50: 2020 2020 7769 7468 206f 7065 6e28 7265      with open(re
-00016f60: 616c 5f66 696c 655f 7061 7468 2c20 2272  al_file_path, "r
-00016f70: 6222 2920 6173 2066 3a0a 2020 2020 2020  b") as f:.      
-00016f80: 2020 2020 2020 7265 616c 5f63 6f6e 7465        real_conte
-00016f90: 6e74 7320 3d20 662e 7265 6164 2829 0a20  nts = f.read(). 
-00016fa0: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-00016fb0: 7274 4571 7561 6c28 6661 6b65 5f66 696c  rtEqual(fake_fil
-00016fc0: 652e 6279 7465 5f63 6f6e 7465 6e74 732c  e.byte_contents,
-00016fd0: 2072 6561 6c5f 636f 6e74 656e 7473 290a   real_contents).
-00016fe0: 2020 2020 2020 2020 7769 7468 2073 656c          with sel
-00016ff0: 662e 6661 6b65 5f6f 7065 6e28 7265 616c  f.fake_open(real
-00017000: 5f66 696c 655f 7061 7468 2c20 2277 6222  _file_path, "wb"
-00017010: 2920 6173 2066 3a0a 2020 2020 2020 2020  ) as f:.        
-00017020: 2020 2020 662e 7772 6974 6528 6222 7465      f.write(b"te
-00017030: 7374 2229 0a20 2020 2020 2020 2077 6974  st").        wit
-00017040: 6820 6f70 656e 2872 6561 6c5f 6669 6c65  h open(real_file
-00017050: 5f70 6174 682c 2022 7262 2229 2061 7320  _path, "rb") as 
-00017060: 663a 0a20 2020 2020 2020 2020 2020 2072  f:.            r
-00017070: 6561 6c5f 636f 6e74 656e 7473 3120 3d20  eal_contents1 = 
-00017080: 662e 7265 6164 2829 0a20 2020 2020 2020  f.read().       
-00017090: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
-000170a0: 6c28 7265 616c 5f63 6f6e 7465 6e74 7331  l(real_contents1
-000170b0: 2c20 7265 616c 5f63 6f6e 7465 6e74 7329  , real_contents)
-000170c0: 0a20 2020 2020 2020 2077 6974 6820 7365  .        with se
-000170d0: 6c66 2e66 616b 655f 6f70 656e 2872 6561  lf.fake_open(rea
-000170e0: 6c5f 6669 6c65 5f70 6174 682c 2022 7262  l_file_path, "rb
-000170f0: 2229 2061 7320 663a 0a20 2020 2020 2020  ") as f:.       
-00017100: 2020 2020 2066 616b 655f 636f 6e74 656e       fake_conten
-00017110: 7473 203d 2066 2e72 6561 6428 290a 2020  ts = f.read().  
-00017120: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
-00017130: 7445 7175 616c 2866 616b 655f 636f 6e74  tEqual(fake_cont
-00017140: 656e 7473 2c20 6222 7465 7374 2229 0a0a  ents, b"test")..
-00017150: 2020 2020 6465 6620 7465 7374 5f61 6464      def test_add
-00017160: 5f65 7869 7374 696e 675f 7265 616c 5f66  _existing_real_f
-00017170: 696c 655f 7265 6164 5f6f 6e6c 7928 7365  ile_read_only(se
-00017180: 6c66 293a 0a20 2020 2020 2020 2072 6561  lf):.        rea
-00017190: 6c5f 6669 6c65 5f70 6174 6820 3d20 6f73  l_file_path = os
-000171a0: 2e70 6174 682e 6162 7370 6174 6828 5f5f  .path.abspath(__
-000171b0: 6669 6c65 5f5f 290a 2020 2020 2020 2020  file__).        
-000171c0: 6661 6b65 5f66 696c 6520 3d20 7365 6c66  fake_file = self
-000171d0: 2e66 696c 6573 7973 7465 6d2e 6164 645f  .filesystem.add_
-000171e0: 7265 616c 5f66 696c 6528 7265 616c 5f66  real_file(real_f
-000171f0: 696c 655f 7061 7468 290a 2020 2020 2020  ile_path).      
-00017200: 2020 7365 6c66 2e63 6865 636b 5f66 616b    self.check_fak
-00017210: 655f 6669 6c65 5f73 7461 7428 6661 6b65  e_file_stat(fake
-00017220: 5f66 696c 652c 2072 6561 6c5f 6669 6c65  _file, real_file
-00017230: 5f70 6174 6829 0a20 2020 2020 2020 2073  _path).        s
-00017240: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
-00017250: 6661 6b65 5f66 696c 652e 7374 5f6d 6f64  fake_file.st_mod
-00017260: 6520 2620 306f 3333 332c 2030 290a 2020  e & 0o333, 0).  
-00017270: 2020 2020 2020 7365 6c66 2e63 6865 636b        self.check
-00017280: 5f72 6561 645f 6f6e 6c79 5f66 696c 6528  _read_only_file(
-00017290: 6661 6b65 5f66 696c 652c 2072 6561 6c5f  fake_file, real_
-000172a0: 6669 6c65 5f70 6174 6829 0a0a 2020 2020  file_path)..    
-000172b0: 6465 6620 7465 7374 5f61 6464 5f65 7869  def test_add_exi
-000172c0: 7374 696e 675f 7265 616c 5f66 696c 655f  sting_real_file_
-000172d0: 7265 6164 5f77 7269 7465 2873 656c 6629  read_write(self)
-000172e0: 3a0a 2020 2020 2020 2020 7265 616c 5f66  :.        real_f
-000172f0: 696c 655f 7061 7468 203d 206f 732e 7061  ile_path = os.pa
-00017300: 7468 2e72 6561 6c70 6174 6828 5f5f 6669  th.realpath(__fi
-00017310: 6c65 5f5f 290a 2020 2020 2020 2020 6661  le__).        fa
-00017320: 6b65 5f66 696c 6520 3d20 7365 6c66 2e66  ke_file = self.f
-00017330: 696c 6573 7973 7465 6d2e 6164 645f 7265  ilesystem.add_re
-00017340: 616c 5f66 696c 6528 7265 616c 5f66 696c  al_file(real_fil
-00017350: 655f 7061 7468 2c20 7265 6164 5f6f 6e6c  e_path, read_onl
-00017360: 793d 4661 6c73 6529 0a0a 2020 2020 2020  y=False)..      
-00017370: 2020 7365 6c66 2e63 6865 636b 5f66 616b    self.check_fak
-00017380: 655f 6669 6c65 5f73 7461 7428 6661 6b65  e_file_stat(fake
-00017390: 5f66 696c 652c 2072 6561 6c5f 6669 6c65  _file, real_file
-000173a0: 5f70 6174 6829 0a20 2020 2020 2020 2073  _path).        s
-000173b0: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
-000173c0: 6661 6b65 5f66 696c 652e 7374 5f6d 6f64  fake_file.st_mod
-000173d0: 652c 206f 732e 7374 6174 2872 6561 6c5f  e, os.stat(real_
-000173e0: 6669 6c65 5f70 6174 6829 2e73 745f 6d6f  file_path).st_mo
-000173f0: 6465 290a 2020 2020 2020 2020 7365 6c66  de).        self
-00017400: 2e63 6865 636b 5f77 7269 7461 626c 655f  .check_writable_
-00017410: 6669 6c65 2866 616b 655f 6669 6c65 2c20  file(fake_file, 
-00017420: 7265 616c 5f66 696c 655f 7061 7468 290a  real_file_path).
-00017430: 0a20 2020 2064 6566 2074 6573 745f 6164  .    def test_ad
-00017440: 645f 7265 616c 5f66 696c 655f 746f 5f65  d_real_file_to_e
-00017450: 7869 7374 696e 675f 7061 7468 2873 656c  xisting_path(sel
-00017460: 6629 3a0a 2020 2020 2020 2020 7265 616c  f):.        real
-00017470: 5f66 696c 655f 7061 7468 203d 206f 732e  _file_path = os.
-00017480: 7061 7468 2e61 6273 7061 7468 285f 5f66  path.abspath(__f
-00017490: 696c 655f 5f29 0a20 2020 2020 2020 2073  ile__).        s
-000174a0: 656c 662e 6669 6c65 7379 7374 656d 2e63  elf.filesystem.c
-000174b0: 7265 6174 655f 6669 6c65 2822 2f66 6f6f  reate_file("/foo
-000174c0: 2f62 6172 2229 0a20 2020 2020 2020 2077  /bar").        w
-000174d0: 6974 6820 7365 6c66 2e72 6169 7365 735f  ith self.raises_
-000174e0: 6f73 5f65 7272 6f72 2865 7272 6e6f 2e45  os_error(errno.E
-000174f0: 4558 4953 5429 3a0a 2020 2020 2020 2020  EXIST):.        
-00017500: 2020 2020 7365 6c66 2e66 696c 6573 7973      self.filesys
-00017510: 7465 6d2e 6164 645f 7265 616c 5f66 696c  tem.add_real_fil
-00017520: 6528 7265 616c 5f66 696c 655f 7061 7468  e(real_file_path
-00017530: 2c20 7461 7267 6574 5f70 6174 683d 222f  , target_path="/
-00017540: 666f 6f2f 6261 7222 290a 0a20 2020 2064  foo/bar")..    d
-00017550: 6566 2074 6573 745f 6164 645f 7265 616c  ef test_add_real
-00017560: 5f66 696c 655f 746f 5f6e 6f6e 5f65 7869  _file_to_non_exi
-00017570: 7374 696e 675f 7061 7468 2873 656c 6629  sting_path(self)
-00017580: 3a0a 2020 2020 2020 2020 7265 616c 5f66  :.        real_f
-00017590: 696c 655f 7061 7468 203d 206f 732e 7061  ile_path = os.pa
-000175a0: 7468 2e61 6273 7061 7468 285f 5f66 696c  th.abspath(__fil
-000175b0: 655f 5f29 0a20 2020 2020 2020 2066 616b  e__).        fak
-000175c0: 655f 6669 6c65 203d 2073 656c 662e 6669  e_file = self.fi
-000175d0: 6c65 7379 7374 656d 2e61 6464 5f72 6561  lesystem.add_rea
-000175e0: 6c5f 6669 6c65 280a 2020 2020 2020 2020  l_file(.        
-000175f0: 2020 2020 7265 616c 5f66 696c 655f 7061      real_file_pa
-00017600: 7468 2c20 7461 7267 6574 5f70 6174 683d  th, target_path=
-00017610: 222f 666f 6f2f 6261 7222 0a20 2020 2020  "/foo/bar".     
-00017620: 2020 2029 0a20 2020 2020 2020 2073 656c     ).        sel
-00017630: 662e 6368 6563 6b5f 6661 6b65 5f66 696c  f.check_fake_fil
-00017640: 655f 7374 6174 2866 616b 655f 6669 6c65  e_stat(fake_file
-00017650: 2c20 7265 616c 5f66 696c 655f 7061 7468  , real_file_path
-00017660: 2c20 7461 7267 6574 5f70 6174 683d 222f  , target_path="/
-00017670: 666f 6f2f 6261 7222 290a 0a20 2020 2064  foo/bar")..    d
-00017680: 6566 2074 6573 745f 7772 6974 655f 746f  ef test_write_to
-00017690: 5f72 6561 6c5f 6669 6c65 2873 656c 6629  _real_file(self)
-000176a0: 3a0a 2020 2020 2020 2020 2320 7265 6772  :.        # regr
-000176b0: 6573 7369 6f6e 2074 6573 7420 666f 7220  ession test for 
-000176c0: 2334 3730 0a20 2020 2020 2020 2072 6561  #470.        rea
-000176d0: 6c5f 6669 6c65 5f70 6174 6820 3d20 6f73  l_file_path = os
-000176e0: 2e70 6174 682e 6162 7370 6174 6828 5f5f  .path.abspath(__
-000176f0: 6669 6c65 5f5f 290a 2020 2020 2020 2020  file__).        
-00017700: 7365 6c66 2e66 696c 6573 7973 7465 6d2e  self.filesystem.
-00017710: 6164 645f 7265 616c 5f66 696c 6528 7265  add_real_file(re
-00017720: 616c 5f66 696c 655f 7061 7468 2c20 7265  al_file_path, re
-00017730: 6164 5f6f 6e6c 793d 4661 6c73 6529 0a20  ad_only=False). 
-00017740: 2020 2020 2020 2077 6974 6820 7365 6c66         with self
-00017750: 2e66 616b 655f 6f70 656e 2872 6561 6c5f  .fake_open(real_
-00017760: 6669 6c65 5f70 6174 682c 2022 7722 2c20  file_path, "w", 
-00017770: 656e 636f 6469 6e67 3d22 7574 6638 2229  encoding="utf8")
-00017780: 2061 7320 663a 0a20 2020 2020 2020 2020   as f:.         
-00017790: 2020 2066 2e77 7269 7465 2822 666f 6f22     f.write("foo"
-000177a0: 290a 0a20 2020 2020 2020 2077 6974 6820  )..        with 
-000177b0: 7365 6c66 2e66 616b 655f 6f70 656e 2872  self.fake_open(r
-000177c0: 6561 6c5f 6669 6c65 5f70 6174 682c 2022  eal_file_path, "
-000177d0: 7262 2229 2061 7320 663a 0a20 2020 2020  rb") as f:.     
-000177e0: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-000177f0: 7274 4571 7561 6c28 6222 666f 6f22 2c20  rtEqual(b"foo", 
-00017800: 662e 7265 6164 2829 290a 0a20 2020 2064  f.read())..    d
-00017810: 6566 2074 6573 745f 6164 645f 6578 6973  ef test_add_exis
-00017820: 7469 6e67 5f72 6561 6c5f 6469 7265 6374  ting_real_direct
-00017830: 6f72 795f 7265 6164 5f6f 6e6c 7928 7365  ory_read_only(se
-00017840: 6c66 293a 0a20 2020 2020 2020 2073 656c  lf):.        sel
-00017850: 662e 6669 6c65 7379 7374 656d 2e61 6464  f.filesystem.add
-00017860: 5f72 6561 6c5f 6469 7265 6374 6f72 7928  _real_directory(
-00017870: 7365 6c66 2e70 7966 616b 6566 735f 7061  self.pyfakefs_pa
-00017880: 7468 290a 2020 2020 2020 2020 7365 6c66  th).        self
-00017890: 2e61 7373 6572 7454 7275 6528 7365 6c66  .assertTrue(self
-000178a0: 2e66 696c 6573 7973 7465 6d2e 6578 6973  .filesystem.exis
-000178b0: 7473 2873 656c 662e 7079 6661 6b65 6673  ts(self.pyfakefs
-000178c0: 5f70 6174 6829 290a 2020 2020 2020 2020  _path)).        
-000178d0: 7365 6c66 2e61 7373 6572 7454 7275 6528  self.assertTrue(
-000178e0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-000178f0: 662e 6669 6c65 7379 7374 656d 2e65 7869  f.filesystem.exi
-00017900: 7374 7328 0a20 2020 2020 2020 2020 2020  sts(.           
-00017910: 2020 2020 206f 732e 7061 7468 2e6a 6f69       os.path.joi
-00017920: 6e28 7365 6c66 2e70 7966 616b 6566 735f  n(self.pyfakefs_
-00017930: 7061 7468 2c20 2266 616b 655f 6669 6c65  path, "fake_file
-00017940: 7379 7374 656d 2e70 7922 290a 2020 2020  system.py").    
-00017950: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00017960: 2020 290a 2020 2020 2020 2020 7365 6c66    ).        self
-00017970: 2e61 7373 6572 7454 7275 6528 0a20 2020  .assertTrue(.   
-00017980: 2020 2020 2020 2020 2073 656c 662e 6669           self.fi
-00017990: 6c65 7379 7374 656d 2e65 7869 7374 7328  lesystem.exists(
-000179a0: 6f73 2e70 6174 682e 6a6f 696e 2873 656c  os.path.join(sel
-000179b0: 662e 7079 6661 6b65 6673 5f70 6174 682c  f.pyfakefs_path,
-000179c0: 2022 6661 6b65 5f70 6174 686c 6962 2e70   "fake_pathlib.p
-000179d0: 7922 2929 0a20 2020 2020 2020 2029 0a0a  y")).        )..
-000179e0: 2020 2020 2020 2020 6669 6c65 5f70 6174          file_pat
-000179f0: 6820 3d20 6f73 2e70 6174 682e 6a6f 696e  h = os.path.join
-00017a00: 2873 656c 662e 7079 6661 6b65 6673 5f70  (self.pyfakefs_p
-00017a10: 6174 682c 2022 6661 6b65 5f66 696c 6573  ath, "fake_files
-00017a20: 7973 7465 6d5f 7368 7574 696c 2e70 7922  ystem_shutil.py"
-00017a30: 290a 2020 2020 2020 2020 6661 6b65 5f66  ).        fake_f
-00017a40: 696c 6520 3d20 7365 6c66 2e66 696c 6573  ile = self.files
-00017a50: 7973 7465 6d2e 7265 736f 6c76 6528 6669  ystem.resolve(fi
-00017a60: 6c65 5f70 6174 6829 0a20 2020 2020 2020  le_path).       
-00017a70: 2073 656c 662e 6368 6563 6b5f 6661 6b65   self.check_fake
-00017a80: 5f66 696c 655f 7374 6174 2866 616b 655f  _file_stat(fake_
-00017a90: 6669 6c65 2c20 6669 6c65 5f70 6174 6829  file, file_path)
-00017aa0: 0a20 2020 2020 2020 2073 656c 662e 6368  .        self.ch
-00017ab0: 6563 6b5f 7265 6164 5f6f 6e6c 795f 6669  eck_read_only_fi
-00017ac0: 6c65 2866 616b 655f 6669 6c65 2c20 6669  le(fake_file, fi
-00017ad0: 6c65 5f70 6174 6829 0a0a 2020 2020 6465  le_path)..    de
-00017ae0: 6620 7465 7374 5f61 6464 5f65 7869 7374  f test_add_exist
-00017af0: 696e 675f 7265 616c 5f64 6972 6563 746f  ing_real_directo
-00017b00: 7279 5f74 7265 6528 7365 6c66 293a 0a20  ry_tree(self):. 
-00017b10: 2020 2020 2020 2073 656c 662e 6669 6c65         self.file
-00017b20: 7379 7374 656d 2e61 6464 5f72 6561 6c5f  system.add_real_
-00017b30: 6469 7265 6374 6f72 7928 7365 6c66 2e72  directory(self.r
-00017b40: 6f6f 745f 7061 7468 290a 2020 2020 2020  oot_path).      
-00017b50: 2020 7365 6c66 2e61 7373 6572 7454 7275    self.assertTru
-00017b60: 6528 0a20 2020 2020 2020 2020 2020 2073  e(.            s
-00017b70: 656c 662e 6669 6c65 7379 7374 656d 2e65  elf.filesystem.e
-00017b80: 7869 7374 7328 0a20 2020 2020 2020 2020  xists(.         
-00017b90: 2020 2020 2020 206f 732e 7061 7468 2e6a         os.path.j
-00017ba0: 6f69 6e28 0a20 2020 2020 2020 2020 2020  oin(.           
-00017bb0: 2020 2020 2020 2020 2073 656c 662e 726f           self.ro
-00017bc0: 6f74 5f70 6174 682c 0a20 2020 2020 2020  ot_path,.       
-00017bd0: 2020 2020 2020 2020 2020 2020 2022 7079               "py
-00017be0: 6661 6b65 6673 222c 0a20 2020 2020 2020  fakefs",.       
-00017bf0: 2020 2020 2020 2020 2020 2020 2022 7465               "te
-00017c00: 7374 7322 2c0a 2020 2020 2020 2020 2020  sts",.          
-00017c10: 2020 2020 2020 2020 2020 2266 616b 655f            "fake_
-00017c20: 6669 6c65 7379 7374 656d 5f74 6573 742e  filesystem_test.
-00017c30: 7079 222c 0a20 2020 2020 2020 2020 2020  py",.           
-00017c40: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
-00017c50: 2020 2029 0a20 2020 2020 2020 2029 0a20     ).        ). 
-00017c60: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-00017c70: 7274 5472 7565 280a 2020 2020 2020 2020  rtTrue(.        
-00017c80: 2020 2020 7365 6c66 2e66 696c 6573 7973      self.filesys
-00017c90: 7465 6d2e 6578 6973 7473 280a 2020 2020  tem.exists(.    
-00017ca0: 2020 2020 2020 2020 2020 2020 6f73 2e70              os.p
-00017cb0: 6174 682e 6a6f 696e 2873 656c 662e 726f  ath.join(self.ro
-00017cc0: 6f74 5f70 6174 682c 2022 7079 6661 6b65  ot_path, "pyfake
-00017cd0: 6673 222c 2022 6661 6b65 5f66 696c 6573  fs", "fake_files
-00017ce0: 7973 7465 6d2e 7079 2229 0a20 2020 2020  ystem.py").     
-00017cf0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-00017d00: 2029 0a20 2020 2020 2020 2073 656c 662e   ).        self.
-00017d10: 6173 7365 7274 5472 7565 280a 2020 2020  assertTrue(.    
-00017d20: 2020 2020 2020 2020 7365 6c66 2e66 696c          self.fil
-00017d30: 6573 7973 7465 6d2e 6578 6973 7473 280a  esystem.exists(.
-00017d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017d50: 6f73 2e70 6174 682e 6a6f 696e 2873 656c  os.path.join(sel
-00017d60: 662e 726f 6f74 5f70 6174 682c 2022 7079  f.root_path, "py
-00017d70: 6661 6b65 6673 222c 2022 5f5f 696e 6974  fakefs", "__init
-00017d80: 5f5f 2e70 7922 290a 2020 2020 2020 2020  __.py").        
-00017d90: 2020 2020 290a 2020 2020 2020 2020 290a      ).        ).
-00017da0: 0a20 2020 2040 636f 6e74 6578 746c 6962  .    @contextlib
-00017db0: 2e63 6f6e 7465 7874 6d61 6e61 6765 720a  .contextmanager.
-00017dc0: 2020 2020 6465 6620 6372 6561 7465 5f73      def create_s
-00017dd0: 796d 6c69 6e6b 7328 7365 6c66 2c20 7379  ymlinks(self, sy
-00017de0: 6d6c 696e 6b73 293a 0a20 2020 2020 2020  mlinks):.       
-00017df0: 2066 6f72 206c 696e 6b20 696e 2073 796d   for link in sym
-00017e00: 6c69 6e6b 733a 0a20 2020 2020 2020 2020  links:.         
-00017e10: 2020 206f 732e 7379 6d6c 696e 6b28 6c69     os.symlink(li
-00017e20: 6e6b 5b30 5d2c 206c 696e 6b5b 315d 290a  nk[0], link[1]).
-00017e30: 0a20 2020 2020 2020 2079 6965 6c64 0a0a  .        yield..
-00017e40: 2020 2020 2020 2020 666f 7220 6c69 6e6b          for link
-00017e50: 2069 6e20 7379 6d6c 696e 6b73 3a0a 2020   in symlinks:.  
-00017e60: 2020 2020 2020 2020 2020 6f73 2e75 6e6c            os.unl
-00017e70: 696e 6b28 6c69 6e6b 5b31 5d29 0a0a 2020  ink(link[1])..  
-00017e80: 2020 6465 6620 7465 7374 5f61 6464 5f65    def test_add_e
-00017e90: 7869 7374 696e 675f 7265 616c 5f64 6972  xisting_real_dir
-00017ea0: 6563 746f 7279 5f73 796d 6c69 6e6b 2873  ectory_symlink(s
-00017eb0: 656c 6629 3a0a 2020 2020 2020 2020 6661  elf):.        fa
-00017ec0: 6b65 5f6f 7065 6e20 3d20 6661 6b65 5f66  ke_open = fake_f
-00017ed0: 696c 6573 7973 7465 6d2e 4661 6b65 4669  ilesystem.FakeFi
-00017ee0: 6c65 4f70 656e 2873 656c 662e 6669 6c65  leOpen(self.file
-00017ef0: 7379 7374 656d 290a 2020 2020 2020 2020  system).        
-00017f00: 7265 616c 5f64 6972 6563 746f 7279 203d  real_directory =
-00017f10: 206f 732e 7061 7468 2e6a 6f69 6e28 7365   os.path.join(se
-00017f20: 6c66 2e72 6f6f 745f 7061 7468 2c20 2270  lf.root_path, "p
-00017f30: 7966 616b 6566 7322 2c20 2274 6573 7473  yfakefs", "tests
-00017f40: 2229 0a20 2020 2020 2020 2073 796d 6c69  ").        symli
-00017f50: 6e6b 7320 3d20 5b0a 2020 2020 2020 2020  nks = [.        
-00017f60: 2020 2020 280a 2020 2020 2020 2020 2020      (.          
-00017f70: 2020 2020 2020 222e 2e22 2c0a 2020 2020        "..",.    
-00017f80: 2020 2020 2020 2020 2020 2020 6f73 2e70              os.p
-00017f90: 6174 682e 6a6f 696e 2872 6561 6c5f 6469  ath.join(real_di
-00017fa0: 7265 6374 6f72 792c 2022 6669 7874 7572  rectory, "fixtur
-00017fb0: 6573 222c 2022 7379 6d6c 696e 6b5f 6469  es", "symlink_di
-00017fc0: 725f 7265 6c61 7469 7665 2229 2c0a 2020  r_relative"),.  
-00017fd0: 2020 2020 2020 2020 2020 292c 0a20 2020            ),.   
-00017fe0: 2020 2020 2020 2020 2028 0a20 2020 2020           (.     
-00017ff0: 2020 2020 2020 2020 2020 2022 2e2e 2f61             "../a
-00018000: 6c6c 5f74 6573 7473 2e70 7922 2c0a 2020  ll_tests.py",.  
-00018010: 2020 2020 2020 2020 2020 2020 2020 6f73                os
-00018020: 2e70 6174 682e 6a6f 696e 2872 6561 6c5f  .path.join(real_
-00018030: 6469 7265 6374 6f72 792c 2022 6669 7874  directory, "fixt
-00018040: 7572 6573 222c 2022 7379 6d6c 696e 6b5f  ures", "symlink_
-00018050: 6669 6c65 5f72 656c 6174 6976 6522 292c  file_relative"),
-00018060: 0a20 2020 2020 2020 2020 2020 2029 2c0a  .            ),.
-00018070: 2020 2020 2020 2020 2020 2020 280a 2020              (.  
-00018080: 2020 2020 2020 2020 2020 2020 2020 7265                re
-00018090: 616c 5f64 6972 6563 746f 7279 2c0a 2020  al_directory,.  
-000180a0: 2020 2020 2020 2020 2020 2020 2020 6f73                os
-000180b0: 2e70 6174 682e 6a6f 696e 2872 6561 6c5f  .path.join(real_
-000180c0: 6469 7265 6374 6f72 792c 2022 6669 7874  directory, "fixt
-000180d0: 7572 6573 222c 2022 7379 6d6c 696e 6b5f  ures", "symlink_
-000180e0: 6469 725f 6162 736f 6c75 7465 2229 2c0a  dir_absolute"),.
-000180f0: 2020 2020 2020 2020 2020 2020 292c 0a20              ),. 
-00018100: 2020 2020 2020 2020 2020 2028 0a20 2020             (.   
-00018110: 2020 2020 2020 2020 2020 2020 206f 732e               os.
-00018120: 7061 7468 2e6a 6f69 6e28 7265 616c 5f64  path.join(real_d
-00018130: 6972 6563 746f 7279 2c20 2261 6c6c 5f74  irectory, "all_t
-00018140: 6573 7473 2e70 7922 292c 0a20 2020 2020  ests.py"),.     
-00018150: 2020 2020 2020 2020 2020 206f 732e 7061             os.pa
-00018160: 7468 2e6a 6f69 6e28 7265 616c 5f64 6972  th.join(real_dir
-00018170: 6563 746f 7279 2c20 2266 6978 7475 7265  ectory, "fixture
-00018180: 7322 2c20 2273 796d 6c69 6e6b 5f66 696c  s", "symlink_fil
-00018190: 655f 6162 736f 6c75 7465 2229 2c0a 2020  e_absolute"),.  
-000181a0: 2020 2020 2020 2020 2020 292c 0a20 2020            ),.   
-000181b0: 2020 2020 2020 2020 2028 0a20 2020 2020           (.     
-000181c0: 2020 2020 2020 2020 2020 2022 2f65 7463             "/etc
-000181d0: 2f73 6f6d 6574 6869 6e67 222c 0a20 2020  /something",.   
-000181e0: 2020 2020 2020 2020 2020 2020 206f 732e               os.
-000181f0: 7061 7468 2e6a 6f69 6e28 0a20 2020 2020  path.join(.     
-00018200: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00018210: 6561 6c5f 6469 7265 6374 6f72 792c 2022  eal_directory, "
-00018220: 6669 7874 7572 6573 222c 2022 7379 6d6c  fixtures", "syml
-00018230: 696e 6b5f 6669 6c65 5f61 6273 6f6c 7574  ink_file_absolut
-00018240: 655f 6f75 7473 6964 6522 0a20 2020 2020  e_outside".     
-00018250: 2020 2020 2020 2020 2020 2029 2c0a 2020             ),.  
-00018260: 2020 2020 2020 2020 2020 292c 0a20 2020            ),.   
-00018270: 2020 2020 205d 0a0a 2020 2020 2020 2020       ]..        
-00018280: 7365 6c66 2e66 696c 6573 7973 7465 6d2e  self.filesystem.
-00018290: 6372 6561 7465 5f66 696c 6528 222f 6574  create_file("/et
-000182a0: 632f 736f 6d65 7468 696e 6722 290a 0a20  c/something").. 
-000182b0: 2020 2020 2020 2077 6974 6820 6661 6b65         with fake
-000182c0: 5f6f 7065 6e28 222f 6574 632f 736f 6d65  _open("/etc/some
-000182d0: 7468 696e 6722 2c20 2277 222c 2065 6e63  thing", "w", enc
-000182e0: 6f64 696e 673d 2275 7466 3822 2920 6173  oding="utf8") as
-000182f0: 2066 3a0a 2020 2020 2020 2020 2020 2020   f:.            
-00018300: 662e 7772 6974 6528 2267 6f6f 6420 6d6f  f.write("good mo
-00018310: 726e 696e 6722 290a 0a20 2020 2020 2020  rning")..       
-00018320: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
-00018330: 2020 7769 7468 2073 656c 662e 6372 6561    with self.crea
-00018340: 7465 5f73 796d 6c69 6e6b 7328 7379 6d6c  te_symlinks(syml
-00018350: 696e 6b73 293a 0a20 2020 2020 2020 2020  inks):.         
-00018360: 2020 2020 2020 2073 656c 662e 6669 6c65         self.file
-00018370: 7379 7374 656d 2e61 6464 5f72 6561 6c5f  system.add_real_
-00018380: 6469 7265 6374 6f72 7928 7265 616c 5f64  directory(real_d
-00018390: 6972 6563 746f 7279 2c20 6c61 7a79 5f72  irectory, lazy_r
-000183a0: 6561 643d 4661 6c73 6529 0a20 2020 2020  ead=False).     
-000183b0: 2020 2065 7863 6570 7420 4f53 4572 726f     except OSErro
-000183c0: 723a 0a20 2020 2020 2020 2020 2020 2069  r:.            i
-000183d0: 6620 7365 6c66 2e69 735f 7769 6e64 6f77  f self.is_window
-000183e0: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
-000183f0: 2020 2072 6169 7365 2075 6e69 7474 6573     raise unittes
-00018400: 742e 536b 6970 5465 7374 2822 5379 6d6c  t.SkipTest("Syml
-00018410: 696e 6b73 2075 6e64 6572 2057 696e 646f  inks under Windo
-00018420: 7773 206e 6565 6420 6164 6d69 6e20 7072  ws need admin pr
-00018430: 6976 696c 6567 6573 2229 0a20 2020 2020  ivileges").     
-00018440: 2020 2020 2020 2072 6169 7365 0a0a 2020         raise..  
-00018450: 2020 2020 2020 666f 7220 6c69 6e6b 2069        for link i
-00018460: 6e20 7379 6d6c 696e 6b73 3a0a 2020 2020  n symlinks:.    
-00018470: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-00018480: 6572 7454 7275 6528 7365 6c66 2e66 696c  ertTrue(self.fil
-00018490: 6573 7973 7465 6d2e 6973 6c69 6e6b 286c  esystem.islink(l
-000184a0: 696e 6b5b 315d 2929 0a0a 2020 2020 2020  ink[1]))..      
-000184b0: 2020 2320 7265 6c61 7469 7665 0a20 2020    # relative.   
-000184c0: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-000184d0: 5472 7565 280a 2020 2020 2020 2020 2020  True(.          
-000184e0: 2020 7365 6c66 2e66 696c 6573 7973 7465    self.filesyste
-000184f0: 6d2e 6578 6973 7473 280a 2020 2020 2020  m.exists(.      
-00018500: 2020 2020 2020 2020 2020 6f73 2e70 6174            os.pat
-00018510: 682e 6a6f 696e 280a 2020 2020 2020 2020  h.join(.        
-00018520: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00018530: 2e72 6f6f 745f 7061 7468 2c0a 2020 2020  .root_path,.    
-00018540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018550: 2270 7966 616b 6566 7322 2c0a 2020 2020  "pyfakefs",.    
-00018560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018570: 2274 6573 7473 222c 0a20 2020 2020 2020  "tests",.       
-00018580: 2020 2020 2020 2020 2020 2020 2022 6669               "fi
-00018590: 7874 7572 6573 2f73 796d 6c69 6e6b 5f64  xtures/symlink_d
-000185a0: 6972 5f72 656c 6174 6976 6522 2c0a 2020  ir_relative",.  
-000185b0: 2020 2020 2020 2020 2020 2020 2020 290a                ).
-000185c0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-000185d0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-000185e0: 7365 6c66 2e61 7373 6572 7454 7275 6528  self.assertTrue(
-000185f0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00018600: 662e 6669 6c65 7379 7374 656d 2e65 7869  f.filesystem.exi
-00018610: 7374 7328 0a20 2020 2020 2020 2020 2020  sts(.           
-00018620: 2020 2020 206f 732e 7061 7468 2e6a 6f69       os.path.joi
-00018630: 6e28 0a20 2020 2020 2020 2020 2020 2020  n(.             
-00018640: 2020 2020 2020 2073 656c 662e 726f 6f74         self.root
-00018650: 5f70 6174 682c 0a20 2020 2020 2020 2020  _path,.         
-00018660: 2020 2020 2020 2020 2020 2022 7079 6661             "pyfa
-00018670: 6b65 6673 222c 0a20 2020 2020 2020 2020  kefs",.         
-00018680: 2020 2020 2020 2020 2020 2022 7465 7374             "test
-00018690: 7322 2c0a 2020 2020 2020 2020 2020 2020  s",.            
-000186a0: 2020 2020 2020 2020 2266 6978 7475 7265          "fixture
-000186b0: 732f 7379 6d6c 696e 6b5f 6469 725f 7265  s/symlink_dir_re
-000186c0: 6c61 7469 7665 2f61 6c6c 5f74 6573 7473  lative/all_tests
-000186d0: 2e70 7922 2c0a 2020 2020 2020 2020 2020  .py",.          
-000186e0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-000186f0: 2020 2020 290a 2020 2020 2020 2020 290a      ).        ).
-00018700: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-00018710: 6572 7454 7275 6528 0a20 2020 2020 2020  ertTrue(.       
-00018720: 2020 2020 2073 656c 662e 6669 6c65 7379       self.filesy
-00018730: 7374 656d 2e65 7869 7374 7328 0a20 2020  stem.exists(.   
-00018740: 2020 2020 2020 2020 2020 2020 206f 732e               os.
-00018750: 7061 7468 2e6a 6f69 6e28 0a20 2020 2020  path.join(.     
-00018760: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00018770: 656c 662e 726f 6f74 5f70 6174 682c 0a20  elf.root_path,. 
-00018780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018790: 2020 2022 7079 6661 6b65 6673 222c 0a20     "pyfakefs",. 
-000187a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000187b0: 2020 2022 7465 7374 7322 2c0a 2020 2020     "tests",.    
-000187c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000187d0: 2266 6978 7475 7265 732f 7379 6d6c 696e  "fixtures/symlin
-000187e0: 6b5f 6669 6c65 5f72 656c 6174 6976 6522  k_file_relative"
-000187f0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00018800: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
-00018810: 290a 2020 2020 2020 2020 290a 0a20 2020  ).        )..   
-00018820: 2020 2020 2023 2061 6273 6f6c 7574 650a       # absolute.
-00018830: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-00018840: 6572 7454 7275 6528 0a20 2020 2020 2020  ertTrue(.       
-00018850: 2020 2020 2073 656c 662e 6669 6c65 7379       self.filesy
-00018860: 7374 656d 2e65 7869 7374 7328 0a20 2020  stem.exists(.   
-00018870: 2020 2020 2020 2020 2020 2020 206f 732e               os.
-00018880: 7061 7468 2e6a 6f69 6e28 0a20 2020 2020  path.join(.     
-00018890: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000188a0: 656c 662e 726f 6f74 5f70 6174 682c 0a20  elf.root_path,. 
-000188b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000188c0: 2020 2022 7079 6661 6b65 6673 222c 0a20     "pyfakefs",. 
-000188d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000188e0: 2020 2022 7465 7374 7322 2c0a 2020 2020     "tests",.    
-000188f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018900: 2266 6978 7475 7265 732f 7379 6d6c 696e  "fixtures/symlin
-00018910: 6b5f 6469 725f 6162 736f 6c75 7465 222c  k_dir_absolute",
-00018920: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00018930: 2029 0a20 2020 2020 2020 2020 2020 2029   ).            )
-00018940: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
-00018950: 2020 2073 656c 662e 6173 7365 7274 5472     self.assertTr
-00018960: 7565 280a 2020 2020 2020 2020 2020 2020  ue(.            
-00018970: 7365 6c66 2e66 696c 6573 7973 7465 6d2e  self.filesystem.
-00018980: 6578 6973 7473 280a 2020 2020 2020 2020  exists(.        
-00018990: 2020 2020 2020 2020 6f73 2e70 6174 682e          os.path.
-000189a0: 6a6f 696e 280a 2020 2020 2020 2020 2020  join(.          
-000189b0: 2020 2020 2020 2020 2020 7365 6c66 2e72            self.r
-000189c0: 6f6f 745f 7061 7468 2c0a 2020 2020 2020  oot_path,.      
-000189d0: 2020 2020 2020 2020 2020 2020 2020 2270                "p
-000189e0: 7966 616b 6566 7322 2c0a 2020 2020 2020  yfakefs",.      
-000189f0: 2020 2020 2020 2020 2020 2020 2020 2274                "t
-00018a00: 6573 7473 222c 0a20 2020 2020 2020 2020  ests",.         
-00018a10: 2020 2020 2020 2020 2020 2022 6669 7874             "fixt
-00018a20: 7572 6573 2f73 796d 6c69 6e6b 5f64 6972  ures/symlink_dir
-00018a30: 5f61 6273 6f6c 7574 652f 616c 6c5f 7465  _absolute/all_te
-00018a40: 7374 732e 7079 222c 0a20 2020 2020 2020  sts.py",.       
-00018a50: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-00018a60: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-00018a70: 2029 0a20 2020 2020 2020 2073 656c 662e   ).        self.
-00018a80: 6173 7365 7274 5472 7565 280a 2020 2020  assertTrue(.    
-00018a90: 2020 2020 2020 2020 7365 6c66 2e66 696c          self.fil
-00018aa0: 6573 7973 7465 6d2e 6578 6973 7473 280a  esystem.exists(.
-00018ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018ac0: 6f73 2e70 6174 682e 6a6f 696e 280a 2020  os.path.join(.  
-00018ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018ae0: 2020 7365 6c66 2e72 6f6f 745f 7061 7468    self.root_path
-00018af0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00018b00: 2020 2020 2020 2270 7966 616b 6566 7322        "pyfakefs"
-00018b10: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00018b20: 2020 2020 2020 2274 6573 7473 222c 0a20        "tests",. 
-00018b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018b40: 2020 2022 6669 7874 7572 6573 2f73 796d     "fixtures/sym
-00018b50: 6c69 6e6b 5f66 696c 655f 6162 736f 6c75  link_file_absolu
-00018b60: 7465 222c 0a20 2020 2020 2020 2020 2020  te",.           
-00018b70: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
-00018b80: 2020 2029 0a20 2020 2020 2020 2029 0a0a     ).        )..
-00018b90: 2020 2020 2020 2020 2320 6f75 7473 6964          # outsid
-00018ba0: 650a 2020 2020 2020 2020 7365 6c66 2e61  e.        self.a
-00018bb0: 7373 6572 7454 7275 6528 0a20 2020 2020  ssertTrue(.     
-00018bc0: 2020 2020 2020 2073 656c 662e 6669 6c65         self.file
-00018bd0: 7379 7374 656d 2e65 7869 7374 7328 0a20  system.exists(. 
-00018be0: 2020 2020 2020 2020 2020 2020 2020 206f                 o
-00018bf0: 732e 7061 7468 2e6a 6f69 6e28 0a20 2020  s.path.join(.   
+00015a10: 2020 2020 2020 7465 6d70 5f64 6972 6563        temp_direc
+00015a20: 746f 7279 203d 2074 656d 7066 696c 652e  tory = tempfile.
+00015a30: 6d6b 6474 656d 7028 290a 2020 2020 2020  mkdtemp().      
+00015a40: 2020 7265 616c 5f64 6972 5f72 6f6f 7420    real_dir_root 
+00015a50: 3d20 6f73 2e70 6174 682e 6a6f 696e 2874  = os.path.join(t
+00015a60: 656d 705f 6469 7265 6374 6f72 792c 2022  emp_directory, "
+00015a70: 726f 6f74 2229 0a20 2020 2020 2020 2074  root").        t
+00015a80: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
+00015a90: 666f 7220 6469 725f 6e61 6d65 2069 6e20  for dir_name in 
+00015aa0: 2822 666f 6f22 2c20 2262 6172 2229 3a0a  ("foo", "bar"):.
+00015ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015ac0: 7265 616c 5f64 6972 203d 206f 732e 7061  real_dir = os.pa
+00015ad0: 7468 2e6a 6f69 6e28 7265 616c 5f64 6972  th.join(real_dir
+00015ae0: 5f72 6f6f 742c 2064 6972 5f6e 616d 6529  _root, dir_name)
+00015af0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00015b00: 206f 732e 6d61 6b65 6469 7273 2872 6561   os.makedirs(rea
+00015b10: 6c5f 6469 722c 2065 7869 7374 5f6f 6b3d  l_dir, exist_ok=
+00015b20: 5472 7565 290a 2020 2020 2020 2020 2020  True).          
+00015b30: 2020 2020 2020 7769 7468 206f 7065 6e28        with open(
+00015b40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00015b50: 2020 2020 206f 732e 7061 7468 2e6a 6f69       os.path.joi
+00015b60: 6e28 7265 616c 5f64 6972 2c20 2274 6573  n(real_dir, "tes
+00015b70: 742e 7478 7422 292c 2022 7722 2c20 656e  t.txt"), "w", en
+00015b80: 636f 6469 6e67 3d22 7574 6638 220a 2020  coding="utf8".  
+00015b90: 2020 2020 2020 2020 2020 2020 2020 2920                ) 
+00015ba0: 6173 2066 3a0a 2020 2020 2020 2020 2020  as f:.          
+00015bb0: 2020 2020 2020 2020 2020 662e 7772 6974            f.writ
+00015bc0: 6528 2274 6573 7422 290a 2020 2020 2020  e("test").      
+00015bd0: 2020 2020 2020 2020 2020 7375 625f 6469            sub_di
+00015be0: 7220 3d20 6f73 2e70 6174 682e 6a6f 696e  r = os.path.join
+00015bf0: 2872 6561 6c5f 6469 722c 2022 7375 6222  (real_dir, "sub"
+00015c00: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00015c10: 2020 6f73 2e6d 616b 6564 6972 7328 7375    os.makedirs(su
+00015c20: 625f 6469 722c 2065 7869 7374 5f6f 6b3d  b_dir, exist_ok=
+00015c30: 5472 7565 290a 2020 2020 2020 2020 2020  True).          
+00015c40: 2020 2020 2020 7769 7468 206f 7065 6e28        with open(
+00015c50: 6f73 2e70 6174 682e 6a6f 696e 2873 7562  os.path.join(sub
+00015c60: 5f64 6972 2c20 2273 7562 2e74 7874 2229  _dir, "sub.txt")
+00015c70: 2c20 2277 222c 2065 6e63 6f64 696e 673d  , "w", encoding=
+00015c80: 2275 7466 3822 2920 6173 2066 3a0a 2020  "utf8") as f:.  
+00015c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015ca0: 2020 662e 7772 6974 6528 2273 7562 2229    f.write("sub")
+00015cb0: 0a20 2020 2020 2020 2020 2020 2079 6965  .            yie
+00015cc0: 6c64 2072 6561 6c5f 6469 725f 726f 6f74  ld real_dir_root
+00015cd0: 0a20 2020 2020 2020 2066 696e 616c 6c79  .        finally
+00015ce0: 3a0a 2020 2020 2020 2020 2020 2020 7368  :.            sh
+00015cf0: 7574 696c 2e72 6d74 7265 6528 7465 6d70  util.rmtree(temp
+00015d00: 5f64 6972 6563 746f 7279 2c20 6967 6e6f  _directory, igno
+00015d10: 7265 5f65 7272 6f72 733d 5472 7565 290a  re_errors=True).
+00015d20: 0a20 2020 2064 6566 2074 6573 745f 6578  .    def test_ex
+00015d30: 6973 7469 6e67 5f66 616b 655f 6469 7265  isting_fake_dire
+00015d40: 6374 6f72 795f 6973 5f6d 6572 6765 645f  ctory_is_merged_
+00015d50: 6c61 7a69 6c79 2873 656c 6629 3a0a 2020  lazily(self):.  
+00015d60: 2020 2020 2020 7365 6c66 2e66 696c 6573        self.files
+00015d70: 7973 7465 6d2e 6372 6561 7465 5f66 696c  ystem.create_fil
+00015d80: 6528 6f73 2e70 6174 682e 6a6f 696e 2822  e(os.path.join("
+00015d90: 2f22 2c20 2272 6f6f 7422 2c20 2266 6f6f  /", "root", "foo
+00015da0: 222c 2022 7465 7374 312e 7478 7422 2929  ", "test1.txt"))
+00015db0: 0a20 2020 2020 2020 2073 656c 662e 6669  .        self.fi
+00015dc0: 6c65 7379 7374 656d 2e63 7265 6174 655f  lesystem.create_
+00015dd0: 6469 7228 6f73 2e70 6174 682e 6a6f 696e  dir(os.path.join
+00015de0: 2822 726f 6f74 222c 2022 6261 7a22 2929  ("root", "baz"))
+00015df0: 0a20 2020 2020 2020 2077 6974 6820 7365  .        with se
+00015e00: 6c66 2e63 7265 6174 655f 7265 616c 5f70  lf.create_real_p
+00015e10: 6174 6873 2829 2061 7320 726f 6f74 5f64  aths() as root_d
+00015e20: 6972 3a0a 2020 2020 2020 2020 2020 2020  ir:.            
+00015e30: 7365 6c66 2e66 696c 6573 7973 7465 6d2e  self.filesystem.
+00015e40: 6164 645f 7265 616c 5f64 6972 6563 746f  add_real_directo
+00015e50: 7279 2872 6f6f 745f 6469 722c 2074 6172  ry(root_dir, tar
+00015e60: 6765 745f 7061 7468 3d22 2f72 6f6f 7422  get_path="/root"
+00015e70: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
+00015e80: 6c66 2e61 7373 6572 7454 7275 6528 0a20  lf.assertTrue(. 
+00015e90: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00015ea0: 656c 662e 6669 6c65 7379 7374 656d 2e65  elf.filesystem.e
+00015eb0: 7869 7374 7328 6f73 2e70 6174 682e 6a6f  xists(os.path.jo
+00015ec0: 696e 2822 726f 6f74 222c 2022 666f 6f22  in("root", "foo"
+00015ed0: 2c20 2274 6573 742e 7478 7422 2929 0a20  , "test.txt")). 
+00015ee0: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+00015ef0: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
+00015f00: 7365 7274 5472 7565 280a 2020 2020 2020  sertTrue(.      
+00015f10: 2020 2020 2020 2020 2020 7365 6c66 2e66            self.f
+00015f20: 696c 6573 7973 7465 6d2e 6578 6973 7473  ilesystem.exists
+00015f30: 286f 732e 7061 7468 2e6a 6f69 6e28 2272  (os.path.join("r
+00015f40: 6f6f 7422 2c20 2266 6f6f 222c 2022 7465  oot", "foo", "te
+00015f50: 7374 312e 7478 7422 2929 0a20 2020 2020  st1.txt")).     
+00015f60: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00015f70: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+00015f80: 5472 7565 280a 2020 2020 2020 2020 2020  True(.          
+00015f90: 2020 2020 2020 7365 6c66 2e66 696c 6573        self.files
+00015fa0: 7973 7465 6d2e 6578 6973 7473 286f 732e  ystem.exists(os.
+00015fb0: 7061 7468 2e6a 6f69 6e28 2272 6f6f 7422  path.join("root"
+00015fc0: 2c20 2262 6172 222c 2022 7375 6222 2c20  , "bar", "sub", 
+00015fd0: 2273 7562 2e74 7874 2229 290a 2020 2020  "sub.txt")).    
+00015fe0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+00015ff0: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+00016000: 7454 7275 6528 7365 6c66 2e66 696c 6573  tTrue(self.files
+00016010: 7973 7465 6d2e 6578 6973 7473 286f 732e  ystem.exists(os.
+00016020: 7061 7468 2e6a 6f69 6e28 2272 6f6f 7422  path.join("root"
+00016030: 2c20 2262 617a 2229 2929 0a0a 2020 2020  , "baz")))..    
+00016040: 6465 6620 7465 7374 5f65 7869 7374 696e  def test_existin
+00016050: 675f 6661 6b65 5f64 6972 6563 746f 7279  g_fake_directory
+00016060: 5f69 735f 6d65 7267 6564 2873 656c 6629  _is_merged(self)
+00016070: 3a0a 2020 2020 2020 2020 7365 6c66 2e66  :.        self.f
+00016080: 696c 6573 7973 7465 6d2e 6372 6561 7465  ilesystem.create
+00016090: 5f66 696c 6528 6f73 2e70 6174 682e 6a6f  _file(os.path.jo
+000160a0: 696e 2822 2f22 2c20 2272 6f6f 7422 2c20  in("/", "root", 
+000160b0: 2266 6f6f 222c 2022 7465 7374 312e 7478  "foo", "test1.tx
+000160c0: 7422 2929 0a20 2020 2020 2020 2073 656c  t")).        sel
+000160d0: 662e 6669 6c65 7379 7374 656d 2e63 7265  f.filesystem.cre
+000160e0: 6174 655f 6469 7228 6f73 2e70 6174 682e  ate_dir(os.path.
+000160f0: 6a6f 696e 2822 726f 6f74 222c 2022 6261  join("root", "ba
+00016100: 7a22 2929 0a20 2020 2020 2020 2077 6974  z")).        wit
+00016110: 6820 7365 6c66 2e63 7265 6174 655f 7265  h self.create_re
+00016120: 616c 5f70 6174 6873 2829 2061 7320 726f  al_paths() as ro
+00016130: 6f74 5f64 6972 3a0a 2020 2020 2020 2020  ot_dir:.        
+00016140: 2020 2020 7365 6c66 2e66 696c 6573 7973      self.filesys
+00016150: 7465 6d2e 6164 645f 7265 616c 5f64 6972  tem.add_real_dir
+00016160: 6563 746f 7279 280a 2020 2020 2020 2020  ectory(.        
+00016170: 2020 2020 2020 2020 726f 6f74 5f64 6972          root_dir
+00016180: 2c20 7461 7267 6574 5f70 6174 683d 222f  , target_path="/
+00016190: 726f 6f74 222c 206c 617a 795f 7265 6164  root", lazy_read
+000161a0: 3d46 616c 7365 0a20 2020 2020 2020 2020  =False.         
+000161b0: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+000161c0: 2073 656c 662e 6173 7365 7274 5472 7565   self.assertTrue
+000161d0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+000161e0: 2020 7365 6c66 2e66 696c 6573 7973 7465    self.filesyste
+000161f0: 6d2e 6578 6973 7473 286f 732e 7061 7468  m.exists(os.path
+00016200: 2e6a 6f69 6e28 2272 6f6f 7422 2c20 2266  .join("root", "f
+00016210: 6f6f 222c 2022 7465 7374 2e74 7874 2229  oo", "test.txt")
+00016220: 290a 2020 2020 2020 2020 2020 2020 290a  ).            ).
+00016230: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00016240: 2e61 7373 6572 7454 7275 6528 0a20 2020  .assertTrue(.   
+00016250: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00016260: 662e 6669 6c65 7379 7374 656d 2e65 7869  f.filesystem.exi
+00016270: 7374 7328 6f73 2e70 6174 682e 6a6f 696e  sts(os.path.join
+00016280: 2822 726f 6f74 222c 2022 666f 6f22 2c20  ("root", "foo", 
+00016290: 2274 6573 7431 2e74 7874 2229 290a 2020  "test1.txt")).  
+000162a0: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+000162b0: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+000162c0: 6572 7454 7275 6528 0a20 2020 2020 2020  ertTrue(.       
+000162d0: 2020 2020 2020 2020 2073 656c 662e 6669           self.fi
+000162e0: 6c65 7379 7374 656d 2e65 7869 7374 7328  lesystem.exists(
+000162f0: 6f73 2e70 6174 682e 6a6f 696e 2822 726f  os.path.join("ro
+00016300: 6f74 222c 2022 6261 7222 2c20 2273 7562  ot", "bar", "sub
+00016310: 222c 2022 7375 622e 7478 7422 2929 0a20  ", "sub.txt")). 
+00016320: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+00016330: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
+00016340: 7365 7274 5472 7565 2873 656c 662e 6669  sertTrue(self.fi
+00016350: 6c65 7379 7374 656d 2e65 7869 7374 7328  lesystem.exists(
+00016360: 6f73 2e70 6174 682e 6a6f 696e 2822 726f  os.path.join("ro
+00016370: 6f74 222c 2022 6261 7a22 2929 290a 0a20  ot", "baz"))).. 
+00016380: 2020 2064 6566 2074 6573 745f 6661 6b65     def test_fake
+00016390: 5f66 696c 6573 5f63 616e 6e6f 745f 6265  _files_cannot_be
+000163a0: 5f6f 7665 7277 7269 7474 656e 2873 656c  _overwritten(sel
+000163b0: 6629 3a0a 2020 2020 2020 2020 7365 6c66  f):.        self
+000163c0: 2e66 696c 6573 7973 7465 6d2e 6372 6561  .filesystem.crea
+000163d0: 7465 5f66 696c 6528 6f73 2e70 6174 682e  te_file(os.path.
+000163e0: 6a6f 696e 2822 2f22 2c20 2272 6f6f 7422  join("/", "root"
+000163f0: 2c20 2266 6f6f 222c 2022 7465 7374 2e74  , "foo", "test.t
+00016400: 7874 2229 290a 2020 2020 2020 2020 7769  xt")).        wi
+00016410: 7468 2073 656c 662e 6372 6561 7465 5f72  th self.create_r
+00016420: 6561 6c5f 7061 7468 7328 2920 6173 2072  eal_paths() as r
+00016430: 6f6f 745f 6469 723a 0a20 2020 2020 2020  oot_dir:.       
+00016440: 2020 2020 2077 6974 6820 7365 6c66 2e72       with self.r
+00016450: 6169 7365 735f 6f73 5f65 7272 6f72 2865  aises_os_error(e
+00016460: 7272 6e6f 2e45 4558 4953 5429 3a0a 2020  rrno.EEXIST):.  
+00016470: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00016480: 6c66 2e66 696c 6573 7973 7465 6d2e 6164  lf.filesystem.ad
+00016490: 645f 7265 616c 5f64 6972 6563 746f 7279  d_real_directory
+000164a0: 2872 6f6f 745f 6469 722c 2074 6172 6765  (root_dir, targe
+000164b0: 745f 7061 7468 3d22 2f72 6f6f 7422 290a  t_path="/root").
+000164c0: 0a20 2020 2064 6566 2074 6573 745f 6361  .    def test_ca
+000164d0: 6e6e 6f74 5f6f 7665 7277 7269 7465 5f66  nnot_overwrite_f
+000164e0: 696c 655f 7769 7468 5f64 6972 2873 656c  ile_with_dir(sel
+000164f0: 6629 3a0a 2020 2020 2020 2020 7365 6c66  f):.        self
+00016500: 2e66 696c 6573 7973 7465 6d2e 6372 6561  .filesystem.crea
+00016510: 7465 5f66 696c 6528 6f73 2e70 6174 682e  te_file(os.path.
+00016520: 6a6f 696e 2822 2f22 2c20 2272 6f6f 7422  join("/", "root"
+00016530: 2c20 2266 6f6f 2229 290a 2020 2020 2020  , "foo")).      
+00016540: 2020 7769 7468 2073 656c 662e 6372 6561    with self.crea
+00016550: 7465 5f72 6561 6c5f 7061 7468 7328 2920  te_real_paths() 
+00016560: 6173 2072 6f6f 745f 6469 723a 0a20 2020  as root_dir:.   
+00016570: 2020 2020 2020 2020 2077 6974 6820 7365           with se
+00016580: 6c66 2e72 6169 7365 735f 6f73 5f65 7272  lf.raises_os_err
+00016590: 6f72 2865 7272 6e6f 2e45 4e4f 5444 4952  or(errno.ENOTDIR
+000165a0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+000165b0: 2020 2073 656c 662e 6669 6c65 7379 7374     self.filesyst
+000165c0: 656d 2e61 6464 5f72 6561 6c5f 6469 7265  em.add_real_dire
+000165d0: 6374 6f72 7928 726f 6f74 5f64 6972 2c20  ctory(root_dir, 
+000165e0: 7461 7267 6574 5f70 6174 683d 222f 726f  target_path="/ro
+000165f0: 6f74 2f22 290a 0a20 2020 2064 6566 2074  ot/")..    def t
+00016600: 6573 745f 6361 6e6e 6f74 5f6f 7665 7277  est_cannot_overw
+00016610: 7269 7465 5f73 796d 6c69 6e6b 5f77 6974  rite_symlink_wit
+00016620: 685f 6469 7228 7365 6c66 293a 0a20 2020  h_dir(self):.   
+00016630: 2020 2020 2073 656c 662e 6669 6c65 7379       self.filesy
+00016640: 7374 656d 2e63 7265 6174 655f 7379 6d6c  stem.create_syml
+00016650: 696e 6b28 0a20 2020 2020 2020 2020 2020  ink(.           
+00016660: 206f 732e 7061 7468 2e6a 6f69 6e28 222f   os.path.join("/
+00016670: 222c 2022 726f 6f74 222c 2022 666f 6f22  ", "root", "foo"
+00016680: 292c 206f 732e 7061 7468 2e6a 6f69 6e28  ), os.path.join(
+00016690: 222f 222c 2022 726f 6f74 222c 2022 6c69  "/", "root", "li
+000166a0: 6e6b 2229 0a20 2020 2020 2020 2029 0a20  nk").        ). 
+000166b0: 2020 2020 2020 2077 6974 6820 7365 6c66         with self
+000166c0: 2e63 7265 6174 655f 7265 616c 5f70 6174  .create_real_pat
+000166d0: 6873 2829 2061 7320 726f 6f74 5f64 6972  hs() as root_dir
+000166e0: 3a0a 2020 2020 2020 2020 2020 2020 7769  :.            wi
+000166f0: 7468 2073 656c 662e 7261 6973 6573 5f6f  th self.raises_o
+00016700: 735f 6572 726f 7228 6572 726e 6f2e 4545  s_error(errno.EE
+00016710: 5849 5354 293a 0a20 2020 2020 2020 2020  XIST):.         
+00016720: 2020 2020 2020 2073 656c 662e 6669 6c65         self.file
+00016730: 7379 7374 656d 2e61 6464 5f72 6561 6c5f  system.add_real_
+00016740: 6469 7265 6374 6f72 7928 726f 6f74 5f64  directory(root_d
+00016750: 6972 2c20 7461 7267 6574 5f70 6174 683d  ir, target_path=
+00016760: 222f 726f 6f74 2f22 290a 0a20 2020 2064  "/root/")..    d
+00016770: 6566 2074 6573 745f 7379 6d6c 696e 6b5f  ef test_symlink_
+00016780: 6973 5f6d 6572 6765 6428 7365 6c66 293a  is_merged(self):
+00016790: 0a20 2020 2020 2020 2073 656c 662e 736b  .        self.sk
+000167a0: 6970 5f69 665f 7379 6d6c 696e 6b5f 6e6f  ip_if_symlink_no
+000167b0: 745f 7375 7070 6f72 7465 6428 666f 7263  t_supported(forc
+000167c0: 655f 7265 616c 5f66 733d 5472 7565 290a  e_real_fs=True).
+000167d0: 2020 2020 2020 2020 7365 6c66 2e66 696c          self.fil
+000167e0: 6573 7973 7465 6d2e 6372 6561 7465 5f64  esystem.create_d
+000167f0: 6972 286f 732e 7061 7468 2e6a 6f69 6e28  ir(os.path.join(
+00016800: 222f 222c 2022 726f 6f74 222c 2022 666f  "/", "root", "fo
+00016810: 6f22 2929 0a20 2020 2020 2020 2077 6974  o")).        wit
+00016820: 6820 7365 6c66 2e63 7265 6174 655f 7265  h self.create_re
+00016830: 616c 5f70 6174 6873 2829 2061 7320 726f  al_paths() as ro
+00016840: 6f74 5f64 6972 3a0a 2020 2020 2020 2020  ot_dir:.        
+00016850: 2020 2020 6c69 6e6b 5f70 6174 6820 3d20      link_path = 
+00016860: 6f73 2e70 6174 682e 6a6f 696e 2872 6f6f  os.path.join(roo
+00016870: 745f 6469 722c 2022 6c69 6e6b 2e74 7874  t_dir, "link.txt
+00016880: 2229 0a20 2020 2020 2020 2020 2020 2074  ").            t
+00016890: 6172 6765 745f 7061 7468 203d 206f 732e  arget_path = os.
+000168a0: 7061 7468 2e6a 6f69 6e28 2266 6f6f 222c  path.join("foo",
+000168b0: 2022 7375 6222 2c20 2273 7562 2e74 7874   "sub", "sub.txt
+000168c0: 2229 0a20 2020 2020 2020 2020 2020 206f  ").            o
+000168d0: 732e 7379 6d6c 696e 6b28 7461 7267 6574  s.symlink(target
+000168e0: 5f70 6174 682c 206c 696e 6b5f 7061 7468  _path, link_path
+000168f0: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
+00016900: 6c66 2e66 696c 6573 7973 7465 6d2e 6164  lf.filesystem.ad
+00016910: 645f 7265 616c 5f64 6972 6563 746f 7279  d_real_directory
+00016920: 2872 6f6f 745f 6469 722c 2074 6172 6765  (root_dir, targe
+00016930: 745f 7061 7468 3d22 2f72 6f6f 7422 290a  t_path="/root").
+00016940: 2020 2020 2020 2020 2020 2020 6661 6b65              fake
+00016950: 5f6c 696e 6b5f 7061 7468 203d 206f 732e  _link_path = os.
+00016960: 7061 7468 2e6a 6f69 6e28 222f 222c 2022  path.join("/", "
+00016970: 726f 6f74 222c 2022 6c69 6e6b 2e74 7874  root", "link.txt
+00016980: 2229 0a20 2020 2020 2020 2020 2020 2073  ").            s
+00016990: 656c 662e 6173 7365 7274 5472 7565 2873  elf.assertTrue(s
+000169a0: 656c 662e 6669 6c65 7379 7374 656d 2e65  elf.filesystem.e
+000169b0: 7869 7374 7328 6661 6b65 5f6c 696e 6b5f  xists(fake_link_
+000169c0: 7061 7468 2929 0a20 2020 2020 2020 2020  path)).         
+000169d0: 2020 2073 656c 662e 6173 7365 7274 5472     self.assertTr
+000169e0: 7565 2873 656c 662e 6669 6c65 7379 7374  ue(self.filesyst
+000169f0: 656d 2e69 736c 696e 6b28 6661 6b65 5f6c  em.islink(fake_l
+00016a00: 696e 6b5f 7061 7468 2929 0a0a 2020 2020  ink_path))..    
+00016a10: 6465 6620 6368 6563 6b5f 6661 6b65 5f66  def check_fake_f
+00016a20: 696c 655f 7374 6174 2873 656c 662c 2066  ile_stat(self, f
+00016a30: 616b 655f 6669 6c65 2c20 7265 616c 5f66  ake_file, real_f
+00016a40: 696c 655f 7061 7468 2c20 7461 7267 6574  ile_path, target
+00016a50: 5f70 6174 683d 4e6f 6e65 293a 0a20 2020  _path=None):.   
+00016a60: 2020 2020 2069 6620 7461 7267 6574 5f70       if target_p
+00016a70: 6174 6820 6973 204e 6f6e 6520 6f72 2074  ath is None or t
+00016a80: 6172 6765 745f 7061 7468 203d 3d20 7265  arget_path == re
+00016a90: 616c 5f66 696c 655f 7061 7468 3a0a 2020  al_file_path:.  
+00016aa0: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+00016ab0: 7373 6572 7454 7275 6528 7365 6c66 2e66  ssertTrue(self.f
+00016ac0: 696c 6573 7973 7465 6d2e 6578 6973 7473  ilesystem.exists
+00016ad0: 2872 6561 6c5f 6669 6c65 5f70 6174 6829  (real_file_path)
+00016ae0: 290a 2020 2020 2020 2020 656c 7365 3a0a  ).        else:.
+00016af0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00016b00: 2e61 7373 6572 7446 616c 7365 2873 656c  .assertFalse(sel
+00016b10: 662e 6669 6c65 7379 7374 656d 2e65 7869  f.filesystem.exi
+00016b20: 7374 7328 7265 616c 5f66 696c 655f 7061  sts(real_file_pa
+00016b30: 7468 2929 0a20 2020 2020 2020 2020 2020  th)).           
+00016b40: 2073 656c 662e 6173 7365 7274 5472 7565   self.assertTrue
+00016b50: 2873 656c 662e 6669 6c65 7379 7374 656d  (self.filesystem
+00016b60: 2e65 7869 7374 7328 7461 7267 6574 5f70  .exists(target_p
+00016b70: 6174 6829 290a 0a20 2020 2020 2020 2072  ath))..        r
+00016b80: 6561 6c5f 7374 6174 203d 206f 732e 7374  eal_stat = os.st
+00016b90: 6174 2872 6561 6c5f 6669 6c65 5f70 6174  at(real_file_pat
+00016ba0: 6829 0a20 2020 2020 2020 2073 656c 662e  h).        self.
+00016bb0: 6173 7365 7274 4973 4e6f 6e65 2866 616b  assertIsNone(fak
+00016bc0: 655f 6669 6c65 2e5f 6279 7465 5f63 6f6e  e_file._byte_con
+00016bd0: 7465 6e74 7329 0a20 2020 2020 2020 2073  tents).        s
+00016be0: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+00016bf0: 6661 6b65 5f66 696c 652e 7374 5f73 697a  fake_file.st_siz
+00016c00: 652c 2072 6561 6c5f 7374 6174 2e73 745f  e, real_stat.st_
+00016c10: 7369 7a65 290a 2020 2020 2020 2020 7365  size).        se
+00016c20: 6c66 2e61 7373 6572 7441 6c6d 6f73 7445  lf.assertAlmostE
+00016c30: 7175 616c 2866 616b 655f 6669 6c65 2e73  qual(fake_file.s
+00016c40: 745f 6374 696d 652c 2072 6561 6c5f 7374  t_ctime, real_st
+00016c50: 6174 2e73 745f 6374 696d 652c 2070 6c61  at.st_ctime, pla
+00016c60: 6365 733d 3529 0a20 2020 2020 2020 2073  ces=5).        s
+00016c70: 656c 662e 6173 7365 7274 416c 6d6f 7374  elf.assertAlmost
+00016c80: 4571 7561 6c28 6661 6b65 5f66 696c 652e  Equal(fake_file.
+00016c90: 7374 5f61 7469 6d65 2c20 7265 616c 5f73  st_atime, real_s
+00016ca0: 7461 742e 7374 5f61 7469 6d65 2c20 706c  tat.st_atime, pl
+00016cb0: 6163 6573 3d35 290a 2020 2020 2020 2020  aces=5).        
+00016cc0: 7365 6c66 2e61 7373 6572 7441 6c6d 6f73  self.assertAlmos
+00016cd0: 7445 7175 616c 2866 616b 655f 6669 6c65  tEqual(fake_file
+00016ce0: 2e73 745f 6d74 696d 652c 2072 6561 6c5f  .st_mtime, real_
+00016cf0: 7374 6174 2e73 745f 6d74 696d 652c 2070  stat.st_mtime, p
+00016d00: 6c61 6365 733d 3529 0a20 2020 2020 2020  laces=5).       
+00016d10: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
+00016d20: 6c28 6661 6b65 5f66 696c 652e 7374 5f75  l(fake_file.st_u
+00016d30: 6964 2c20 7265 616c 5f73 7461 742e 7374  id, real_stat.st
+00016d40: 5f75 6964 290a 2020 2020 2020 2020 7365  _uid).        se
+00016d50: 6c66 2e61 7373 6572 7445 7175 616c 2866  lf.assertEqual(f
+00016d60: 616b 655f 6669 6c65 2e73 745f 6769 642c  ake_file.st_gid,
+00016d70: 2072 6561 6c5f 7374 6174 2e73 745f 6769   real_stat.st_gi
+00016d80: 6429 0a0a 2020 2020 6465 6620 6368 6563  d)..    def chec
+00016d90: 6b5f 7265 6164 5f6f 6e6c 795f 6669 6c65  k_read_only_file
+00016da0: 2873 656c 662c 2066 616b 655f 6669 6c65  (self, fake_file
+00016db0: 2c20 7265 616c 5f66 696c 655f 7061 7468  , real_file_path
+00016dc0: 293a 0a20 2020 2020 2020 2077 6974 6820  ):.        with 
+00016dd0: 6f70 656e 2872 6561 6c5f 6669 6c65 5f70  open(real_file_p
+00016de0: 6174 682c 2022 7262 2229 2061 7320 663a  ath, "rb") as f:
+00016df0: 0a20 2020 2020 2020 2020 2020 2072 6561  .            rea
+00016e00: 6c5f 636f 6e74 656e 7473 203d 2066 2e72  l_contents = f.r
+00016e10: 6561 6428 290a 2020 2020 2020 2020 7365  ead().        se
+00016e20: 6c66 2e61 7373 6572 7445 7175 616c 2866  lf.assertEqual(f
+00016e30: 616b 655f 6669 6c65 2e62 7974 655f 636f  ake_file.byte_co
+00016e40: 6e74 656e 7473 2c20 7265 616c 5f63 6f6e  ntents, real_con
+00016e50: 7465 6e74 7329 0a20 2020 2020 2020 2069  tents).        i
+00016e60: 6620 6e6f 7420 6973 5f72 6f6f 7428 293a  f not is_root():
+00016e70: 0a20 2020 2020 2020 2020 2020 2077 6974  .            wit
+00016e80: 6820 7365 6c66 2e72 6169 7365 735f 6f73  h self.raises_os
+00016e90: 5f65 7272 6f72 2865 7272 6e6f 2e45 4143  _error(errno.EAC
+00016ea0: 4345 5329 3a0a 2020 2020 2020 2020 2020  CES):.          
+00016eb0: 2020 2020 2020 7365 6c66 2e66 616b 655f        self.fake_
+00016ec0: 6f70 656e 2872 6561 6c5f 6669 6c65 5f70  open(real_file_p
+00016ed0: 6174 682c 2022 7722 290a 2020 2020 2020  ath, "w").      
+00016ee0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00016ef0: 2020 2020 7769 7468 2073 656c 662e 6661      with self.fa
+00016f00: 6b65 5f6f 7065 6e28 7265 616c 5f66 696c  ke_open(real_fil
+00016f10: 655f 7061 7468 2c20 2277 2229 3a0a 2020  e_path, "w"):.  
+00016f20: 2020 2020 2020 2020 2020 2020 2020 7061                pa
+00016f30: 7373 0a0a 2020 2020 6465 6620 6368 6563  ss..    def chec
+00016f40: 6b5f 7772 6974 6162 6c65 5f66 696c 6528  k_writable_file(
+00016f50: 7365 6c66 2c20 6661 6b65 5f66 696c 652c  self, fake_file,
+00016f60: 2072 6561 6c5f 6669 6c65 5f70 6174 6829   real_file_path)
+00016f70: 3a0a 2020 2020 2020 2020 7769 7468 206f  :.        with o
+00016f80: 7065 6e28 7265 616c 5f66 696c 655f 7061  pen(real_file_pa
+00016f90: 7468 2c20 2272 6222 2920 6173 2066 3a0a  th, "rb") as f:.
+00016fa0: 2020 2020 2020 2020 2020 2020 7265 616c              real
+00016fb0: 5f63 6f6e 7465 6e74 7320 3d20 662e 7265  _contents = f.re
+00016fc0: 6164 2829 0a20 2020 2020 2020 2073 656c  ad().        sel
+00016fd0: 662e 6173 7365 7274 4571 7561 6c28 6661  f.assertEqual(fa
+00016fe0: 6b65 5f66 696c 652e 6279 7465 5f63 6f6e  ke_file.byte_con
+00016ff0: 7465 6e74 732c 2072 6561 6c5f 636f 6e74  tents, real_cont
+00017000: 656e 7473 290a 2020 2020 2020 2020 7769  ents).        wi
+00017010: 7468 2073 656c 662e 6661 6b65 5f6f 7065  th self.fake_ope
+00017020: 6e28 7265 616c 5f66 696c 655f 7061 7468  n(real_file_path
+00017030: 2c20 2277 6222 2920 6173 2066 3a0a 2020  , "wb") as f:.  
+00017040: 2020 2020 2020 2020 2020 662e 7772 6974            f.writ
+00017050: 6528 6222 7465 7374 2229 0a20 2020 2020  e(b"test").     
+00017060: 2020 2077 6974 6820 6f70 656e 2872 6561     with open(rea
+00017070: 6c5f 6669 6c65 5f70 6174 682c 2022 7262  l_file_path, "rb
+00017080: 2229 2061 7320 663a 0a20 2020 2020 2020  ") as f:.       
+00017090: 2020 2020 2072 6561 6c5f 636f 6e74 656e       real_conten
+000170a0: 7473 3120 3d20 662e 7265 6164 2829 0a20  ts1 = f.read(). 
+000170b0: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+000170c0: 7274 4571 7561 6c28 7265 616c 5f63 6f6e  rtEqual(real_con
+000170d0: 7465 6e74 7331 2c20 7265 616c 5f63 6f6e  tents1, real_con
+000170e0: 7465 6e74 7329 0a20 2020 2020 2020 2077  tents).        w
+000170f0: 6974 6820 7365 6c66 2e66 616b 655f 6f70  ith self.fake_op
+00017100: 656e 2872 6561 6c5f 6669 6c65 5f70 6174  en(real_file_pat
+00017110: 682c 2022 7262 2229 2061 7320 663a 0a20  h, "rb") as f:. 
+00017120: 2020 2020 2020 2020 2020 2066 616b 655f             fake_
+00017130: 636f 6e74 656e 7473 203d 2066 2e72 6561  contents = f.rea
+00017140: 6428 290a 2020 2020 2020 2020 7365 6c66  d().        self
+00017150: 2e61 7373 6572 7445 7175 616c 2866 616b  .assertEqual(fak
+00017160: 655f 636f 6e74 656e 7473 2c20 6222 7465  e_contents, b"te
+00017170: 7374 2229 0a0a 2020 2020 6465 6620 7465  st")..    def te
+00017180: 7374 5f61 6464 5f65 7869 7374 696e 675f  st_add_existing_
+00017190: 7265 616c 5f66 696c 655f 7265 6164 5f6f  real_file_read_o
+000171a0: 6e6c 7928 7365 6c66 293a 0a20 2020 2020  nly(self):.     
+000171b0: 2020 2072 6561 6c5f 6669 6c65 5f70 6174     real_file_pat
+000171c0: 6820 3d20 6f73 2e70 6174 682e 6162 7370  h = os.path.absp
+000171d0: 6174 6828 5f5f 6669 6c65 5f5f 290a 2020  ath(__file__).  
+000171e0: 2020 2020 2020 6661 6b65 5f66 696c 6520        fake_file 
+000171f0: 3d20 7365 6c66 2e66 696c 6573 7973 7465  = self.filesyste
+00017200: 6d2e 6164 645f 7265 616c 5f66 696c 6528  m.add_real_file(
+00017210: 7265 616c 5f66 696c 655f 7061 7468 290a  real_file_path).
+00017220: 2020 2020 2020 2020 7365 6c66 2e63 6865          self.che
+00017230: 636b 5f66 616b 655f 6669 6c65 5f73 7461  ck_fake_file_sta
+00017240: 7428 6661 6b65 5f66 696c 652c 2072 6561  t(fake_file, rea
+00017250: 6c5f 6669 6c65 5f70 6174 6829 0a20 2020  l_file_path).   
+00017260: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+00017270: 4571 7561 6c28 6661 6b65 5f66 696c 652e  Equal(fake_file.
+00017280: 7374 5f6d 6f64 6520 2620 306f 3333 332c  st_mode & 0o333,
+00017290: 2030 290a 2020 2020 2020 2020 7365 6c66   0).        self
+000172a0: 2e63 6865 636b 5f72 6561 645f 6f6e 6c79  .check_read_only
+000172b0: 5f66 696c 6528 6661 6b65 5f66 696c 652c  _file(fake_file,
+000172c0: 2072 6561 6c5f 6669 6c65 5f70 6174 6829   real_file_path)
+000172d0: 0a0a 2020 2020 6465 6620 7465 7374 5f61  ..    def test_a
+000172e0: 6464 5f65 7869 7374 696e 675f 7265 616c  dd_existing_real
+000172f0: 5f66 696c 655f 7265 6164 5f77 7269 7465  _file_read_write
+00017300: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00017310: 7265 616c 5f66 696c 655f 7061 7468 203d  real_file_path =
+00017320: 206f 732e 7061 7468 2e72 6561 6c70 6174   os.path.realpat
+00017330: 6828 5f5f 6669 6c65 5f5f 290a 2020 2020  h(__file__).    
+00017340: 2020 2020 6661 6b65 5f66 696c 6520 3d20      fake_file = 
+00017350: 7365 6c66 2e66 696c 6573 7973 7465 6d2e  self.filesystem.
+00017360: 6164 645f 7265 616c 5f66 696c 6528 7265  add_real_file(re
+00017370: 616c 5f66 696c 655f 7061 7468 2c20 7265  al_file_path, re
+00017380: 6164 5f6f 6e6c 793d 4661 6c73 6529 0a0a  ad_only=False)..
+00017390: 2020 2020 2020 2020 7365 6c66 2e63 6865          self.che
+000173a0: 636b 5f66 616b 655f 6669 6c65 5f73 7461  ck_fake_file_sta
+000173b0: 7428 6661 6b65 5f66 696c 652c 2072 6561  t(fake_file, rea
+000173c0: 6c5f 6669 6c65 5f70 6174 6829 0a20 2020  l_file_path).   
+000173d0: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+000173e0: 4571 7561 6c28 6661 6b65 5f66 696c 652e  Equal(fake_file.
+000173f0: 7374 5f6d 6f64 652c 206f 732e 7374 6174  st_mode, os.stat
+00017400: 2872 6561 6c5f 6669 6c65 5f70 6174 6829  (real_file_path)
+00017410: 2e73 745f 6d6f 6465 290a 2020 2020 2020  .st_mode).      
+00017420: 2020 7365 6c66 2e63 6865 636b 5f77 7269    self.check_wri
+00017430: 7461 626c 655f 6669 6c65 2866 616b 655f  table_file(fake_
+00017440: 6669 6c65 2c20 7265 616c 5f66 696c 655f  file, real_file_
+00017450: 7061 7468 290a 0a20 2020 2064 6566 2074  path)..    def t
+00017460: 6573 745f 6164 645f 7265 616c 5f66 696c  est_add_real_fil
+00017470: 655f 746f 5f65 7869 7374 696e 675f 7061  e_to_existing_pa
+00017480: 7468 2873 656c 6629 3a0a 2020 2020 2020  th(self):.      
+00017490: 2020 7265 616c 5f66 696c 655f 7061 7468    real_file_path
+000174a0: 203d 206f 732e 7061 7468 2e61 6273 7061   = os.path.abspa
+000174b0: 7468 285f 5f66 696c 655f 5f29 0a20 2020  th(__file__).   
+000174c0: 2020 2020 2073 656c 662e 6669 6c65 7379       self.filesy
+000174d0: 7374 656d 2e63 7265 6174 655f 6669 6c65  stem.create_file
+000174e0: 2822 2f66 6f6f 2f62 6172 2229 0a20 2020  ("/foo/bar").   
+000174f0: 2020 2020 2077 6974 6820 7365 6c66 2e72       with self.r
+00017500: 6169 7365 735f 6f73 5f65 7272 6f72 2865  aises_os_error(e
+00017510: 7272 6e6f 2e45 4558 4953 5429 3a0a 2020  rrno.EEXIST):.  
+00017520: 2020 2020 2020 2020 2020 7365 6c66 2e66            self.f
+00017530: 696c 6573 7973 7465 6d2e 6164 645f 7265  ilesystem.add_re
+00017540: 616c 5f66 696c 6528 7265 616c 5f66 696c  al_file(real_fil
+00017550: 655f 7061 7468 2c20 7461 7267 6574 5f70  e_path, target_p
+00017560: 6174 683d 222f 666f 6f2f 6261 7222 290a  ath="/foo/bar").
+00017570: 0a20 2020 2064 6566 2074 6573 745f 6164  .    def test_ad
+00017580: 645f 7265 616c 5f66 696c 655f 746f 5f6e  d_real_file_to_n
+00017590: 6f6e 5f65 7869 7374 696e 675f 7061 7468  on_existing_path
+000175a0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+000175b0: 7265 616c 5f66 696c 655f 7061 7468 203d  real_file_path =
+000175c0: 206f 732e 7061 7468 2e61 6273 7061 7468   os.path.abspath
+000175d0: 285f 5f66 696c 655f 5f29 0a20 2020 2020  (__file__).     
+000175e0: 2020 2066 616b 655f 6669 6c65 203d 2073     fake_file = s
+000175f0: 656c 662e 6669 6c65 7379 7374 656d 2e61  elf.filesystem.a
+00017600: 6464 5f72 6561 6c5f 6669 6c65 280a 2020  dd_real_file(.  
+00017610: 2020 2020 2020 2020 2020 7265 616c 5f66            real_f
+00017620: 696c 655f 7061 7468 2c20 7461 7267 6574  ile_path, target
+00017630: 5f70 6174 683d 222f 666f 6f2f 6261 7222  _path="/foo/bar"
+00017640: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
+00017650: 2020 2073 656c 662e 6368 6563 6b5f 6661     self.check_fa
+00017660: 6b65 5f66 696c 655f 7374 6174 2866 616b  ke_file_stat(fak
+00017670: 655f 6669 6c65 2c20 7265 616c 5f66 696c  e_file, real_fil
+00017680: 655f 7061 7468 2c20 7461 7267 6574 5f70  e_path, target_p
+00017690: 6174 683d 222f 666f 6f2f 6261 7222 290a  ath="/foo/bar").
+000176a0: 0a20 2020 2064 6566 2074 6573 745f 7772  .    def test_wr
+000176b0: 6974 655f 746f 5f72 6561 6c5f 6669 6c65  ite_to_real_file
+000176c0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+000176d0: 2320 7265 6772 6573 7369 6f6e 2074 6573  # regression tes
+000176e0: 7420 666f 7220 2334 3730 0a20 2020 2020  t for #470.     
+000176f0: 2020 2072 6561 6c5f 6669 6c65 5f70 6174     real_file_pat
+00017700: 6820 3d20 6f73 2e70 6174 682e 6162 7370  h = os.path.absp
+00017710: 6174 6828 5f5f 6669 6c65 5f5f 290a 2020  ath(__file__).  
+00017720: 2020 2020 2020 7365 6c66 2e66 696c 6573        self.files
+00017730: 7973 7465 6d2e 6164 645f 7265 616c 5f66  ystem.add_real_f
+00017740: 696c 6528 7265 616c 5f66 696c 655f 7061  ile(real_file_pa
+00017750: 7468 2c20 7265 6164 5f6f 6e6c 793d 4661  th, read_only=Fa
+00017760: 6c73 6529 0a20 2020 2020 2020 2077 6974  lse).        wit
+00017770: 6820 7365 6c66 2e66 616b 655f 6f70 656e  h self.fake_open
+00017780: 2872 6561 6c5f 6669 6c65 5f70 6174 682c  (real_file_path,
+00017790: 2022 7722 2c20 656e 636f 6469 6e67 3d22   "w", encoding="
+000177a0: 7574 6638 2229 2061 7320 663a 0a20 2020  utf8") as f:.   
+000177b0: 2020 2020 2020 2020 2066 2e77 7269 7465           f.write
+000177c0: 2822 666f 6f22 290a 0a20 2020 2020 2020  ("foo")..       
+000177d0: 2077 6974 6820 7365 6c66 2e66 616b 655f   with self.fake_
+000177e0: 6f70 656e 2872 6561 6c5f 6669 6c65 5f70  open(real_file_p
+000177f0: 6174 682c 2022 7262 2229 2061 7320 663a  ath, "rb") as f:
+00017800: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00017810: 662e 6173 7365 7274 4571 7561 6c28 6222  f.assertEqual(b"
+00017820: 666f 6f22 2c20 662e 7265 6164 2829 290a  foo", f.read()).
+00017830: 0a20 2020 2064 6566 2074 6573 745f 6164  .    def test_ad
+00017840: 645f 6578 6973 7469 6e67 5f72 6561 6c5f  d_existing_real_
+00017850: 6469 7265 6374 6f72 795f 7265 6164 5f6f  directory_read_o
+00017860: 6e6c 7928 7365 6c66 293a 0a20 2020 2020  nly(self):.     
+00017870: 2020 2073 656c 662e 6669 6c65 7379 7374     self.filesyst
+00017880: 656d 2e61 6464 5f72 6561 6c5f 6469 7265  em.add_real_dire
+00017890: 6374 6f72 7928 7365 6c66 2e70 7966 616b  ctory(self.pyfak
+000178a0: 6566 735f 7061 7468 290a 2020 2020 2020  efs_path).      
+000178b0: 2020 7365 6c66 2e61 7373 6572 7454 7275    self.assertTru
+000178c0: 6528 7365 6c66 2e66 696c 6573 7973 7465  e(self.filesyste
+000178d0: 6d2e 6578 6973 7473 2873 656c 662e 7079  m.exists(self.py
+000178e0: 6661 6b65 6673 5f70 6174 6829 290a 2020  fakefs_path)).  
+000178f0: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+00017900: 7454 7275 6528 0a20 2020 2020 2020 2020  tTrue(.         
+00017910: 2020 2073 656c 662e 6669 6c65 7379 7374     self.filesyst
+00017920: 656d 2e65 7869 7374 7328 0a20 2020 2020  em.exists(.     
+00017930: 2020 2020 2020 2020 2020 206f 732e 7061             os.pa
+00017940: 7468 2e6a 6f69 6e28 7365 6c66 2e70 7966  th.join(self.pyf
+00017950: 616b 6566 735f 7061 7468 2c20 2266 616b  akefs_path, "fak
+00017960: 655f 6669 6c65 7379 7374 656d 2e70 7922  e_filesystem.py"
+00017970: 290a 2020 2020 2020 2020 2020 2020 290a  ).            ).
+00017980: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+00017990: 2020 7365 6c66 2e61 7373 6572 7454 7275    self.assertTru
+000179a0: 6528 0a20 2020 2020 2020 2020 2020 2073  e(.            s
+000179b0: 656c 662e 6669 6c65 7379 7374 656d 2e65  elf.filesystem.e
+000179c0: 7869 7374 7328 6f73 2e70 6174 682e 6a6f  xists(os.path.jo
+000179d0: 696e 2873 656c 662e 7079 6661 6b65 6673  in(self.pyfakefs
+000179e0: 5f70 6174 682c 2022 6661 6b65 5f70 6174  _path, "fake_pat
+000179f0: 686c 6962 2e70 7922 2929 0a20 2020 2020  hlib.py")).     
+00017a00: 2020 2029 0a0a 2020 2020 2020 2020 6669     )..        fi
+00017a10: 6c65 5f70 6174 6820 3d20 6f73 2e70 6174  le_path = os.pat
+00017a20: 682e 6a6f 696e 2873 656c 662e 7079 6661  h.join(self.pyfa
+00017a30: 6b65 6673 5f70 6174 682c 2022 6661 6b65  kefs_path, "fake
+00017a40: 5f66 696c 6573 7973 7465 6d5f 7368 7574  _filesystem_shut
+00017a50: 696c 2e70 7922 290a 2020 2020 2020 2020  il.py").        
+00017a60: 6661 6b65 5f66 696c 6520 3d20 7365 6c66  fake_file = self
+00017a70: 2e66 696c 6573 7973 7465 6d2e 7265 736f  .filesystem.reso
+00017a80: 6c76 6528 6669 6c65 5f70 6174 6829 0a20  lve(file_path). 
+00017a90: 2020 2020 2020 2073 656c 662e 6368 6563         self.chec
+00017aa0: 6b5f 6661 6b65 5f66 696c 655f 7374 6174  k_fake_file_stat
+00017ab0: 2866 616b 655f 6669 6c65 2c20 6669 6c65  (fake_file, file
+00017ac0: 5f70 6174 6829 0a20 2020 2020 2020 2073  _path).        s
+00017ad0: 656c 662e 6368 6563 6b5f 7265 6164 5f6f  elf.check_read_o
+00017ae0: 6e6c 795f 6669 6c65 2866 616b 655f 6669  nly_file(fake_fi
+00017af0: 6c65 2c20 6669 6c65 5f70 6174 6829 0a0a  le, file_path)..
+00017b00: 2020 2020 6465 6620 7465 7374 5f61 6464      def test_add
+00017b10: 5f65 7869 7374 696e 675f 7265 616c 5f64  _existing_real_d
+00017b20: 6972 6563 746f 7279 5f74 7265 6528 7365  irectory_tree(se
+00017b30: 6c66 293a 0a20 2020 2020 2020 2073 656c  lf):.        sel
+00017b40: 662e 6669 6c65 7379 7374 656d 2e61 6464  f.filesystem.add
+00017b50: 5f72 6561 6c5f 6469 7265 6374 6f72 7928  _real_directory(
+00017b60: 7365 6c66 2e72 6f6f 745f 7061 7468 290a  self.root_path).
+00017b70: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+00017b80: 6572 7454 7275 6528 0a20 2020 2020 2020  ertTrue(.       
+00017b90: 2020 2020 2073 656c 662e 6669 6c65 7379       self.filesy
+00017ba0: 7374 656d 2e65 7869 7374 7328 0a20 2020  stem.exists(.   
+00017bb0: 2020 2020 2020 2020 2020 2020 206f 732e               os.
+00017bc0: 7061 7468 2e6a 6f69 6e28 0a20 2020 2020  path.join(.     
+00017bd0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00017be0: 656c 662e 726f 6f74 5f70 6174 682c 0a20  elf.root_path,. 
+00017bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017c00: 2020 2022 7079 6661 6b65 6673 222c 0a20     "pyfakefs",. 
+00017c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017c20: 2020 2022 7465 7374 7322 2c0a 2020 2020     "tests",.    
+00017c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017c40: 2266 616b 655f 6669 6c65 7379 7374 656d  "fake_filesystem
+00017c50: 5f74 6573 742e 7079 222c 0a20 2020 2020  _test.py",.     
+00017c60: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+00017c70: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+00017c80: 2020 2029 0a20 2020 2020 2020 2073 656c     ).        sel
+00017c90: 662e 6173 7365 7274 5472 7565 280a 2020  f.assertTrue(.  
+00017ca0: 2020 2020 2020 2020 2020 7365 6c66 2e66            self.f
+00017cb0: 696c 6573 7973 7465 6d2e 6578 6973 7473  ilesystem.exists
+00017cc0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00017cd0: 2020 6f73 2e70 6174 682e 6a6f 696e 2873    os.path.join(s
+00017ce0: 656c 662e 726f 6f74 5f70 6174 682c 2022  elf.root_path, "
+00017cf0: 7079 6661 6b65 6673 222c 2022 6661 6b65  pyfakefs", "fake
+00017d00: 5f66 696c 6573 7973 7465 6d2e 7079 2229  _filesystem.py")
+00017d10: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
+00017d20: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00017d30: 2073 656c 662e 6173 7365 7274 5472 7565   self.assertTrue
+00017d40: 280a 2020 2020 2020 2020 2020 2020 7365  (.            se
+00017d50: 6c66 2e66 696c 6573 7973 7465 6d2e 6578  lf.filesystem.ex
+00017d60: 6973 7473 280a 2020 2020 2020 2020 2020  ists(.          
+00017d70: 2020 2020 2020 6f73 2e70 6174 682e 6a6f        os.path.jo
+00017d80: 696e 2873 656c 662e 726f 6f74 5f70 6174  in(self.root_pat
+00017d90: 682c 2022 7079 6661 6b65 6673 222c 2022  h, "pyfakefs", "
+00017da0: 5f5f 696e 6974 5f5f 2e70 7922 290a 2020  __init__.py").  
+00017db0: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+00017dc0: 2020 2020 290a 0a20 2020 2040 636f 6e74      )..    @cont
+00017dd0: 6578 746c 6962 2e63 6f6e 7465 7874 6d61  extlib.contextma
+00017de0: 6e61 6765 720a 2020 2020 6465 6620 6372  nager.    def cr
+00017df0: 6561 7465 5f73 796d 6c69 6e6b 7328 7365  eate_symlinks(se
+00017e00: 6c66 2c20 7379 6d6c 696e 6b73 293a 0a20  lf, symlinks):. 
+00017e10: 2020 2020 2020 2066 6f72 206c 696e 6b20         for link 
+00017e20: 696e 2073 796d 6c69 6e6b 733a 0a20 2020  in symlinks:.   
+00017e30: 2020 2020 2020 2020 206f 732e 7379 6d6c           os.syml
+00017e40: 696e 6b28 6c69 6e6b 5b30 5d2c 206c 696e  ink(link[0], lin
+00017e50: 6b5b 315d 290a 0a20 2020 2020 2020 2074  k[1])..        t
+00017e60: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
+00017e70: 7969 656c 640a 2020 2020 2020 2020 6669  yield.        fi
+00017e80: 6e61 6c6c 793a 0a20 2020 2020 2020 2020  nally:.         
+00017e90: 2020 2066 6f72 206c 696e 6b20 696e 2073     for link in s
+00017ea0: 796d 6c69 6e6b 733a 0a20 2020 2020 2020  ymlinks:.       
+00017eb0: 2020 2020 2020 2020 206f 732e 756e 6c69           os.unli
+00017ec0: 6e6b 286c 696e 6b5b 315d 290a 0a20 2020  nk(link[1])..   
+00017ed0: 2040 7374 6174 6963 6d65 7468 6f64 0a20   @staticmethod. 
+00017ee0: 2020 2064 6566 205f 7365 7475 705f 7465     def _setup_te
+00017ef0: 6d70 5f64 6972 6563 746f 7279 2829 3a0a  mp_directory():.
+00017f00: 2020 2020 2020 2020 7265 616c 5f64 6972          real_dir
+00017f10: 6563 746f 7279 203d 2074 656d 7066 696c  ectory = tempfil
+00017f20: 652e 6d6b 6474 656d 7028 290a 2020 2020  e.mkdtemp().    
+00017f30: 2020 2020 6f73 2e6d 6b64 6972 286f 732e      os.mkdir(os.
+00017f40: 7061 7468 2e6a 6f69 6e28 7265 616c 5f64  path.join(real_d
+00017f50: 6972 6563 746f 7279 2c20 2266 6978 7475  irectory, "fixtu
+00017f60: 7265 7322 2929 0a20 2020 2020 2020 2077  res")).        w
+00017f70: 6974 6820 6f70 656e 286f 732e 7061 7468  ith open(os.path
+00017f80: 2e6a 6f69 6e28 7265 616c 5f64 6972 6563  .join(real_direc
+00017f90: 746f 7279 2c20 2261 6c6c 5f74 6573 7473  tory, "all_tests
+00017fa0: 2e70 7922 292c 2022 7722 293a 0a20 2020  .py"), "w"):.   
+00017fb0: 2020 2020 2020 2020 2070 6173 730a 2020           pass.  
+00017fc0: 2020 2020 2020 7265 7475 726e 2072 6561        return rea
+00017fd0: 6c5f 6469 7265 6374 6f72 790a 0a20 2020  l_directory..   
+00017fe0: 2064 6566 2074 6573 745f 6164 645f 6578   def test_add_ex
+00017ff0: 6973 7469 6e67 5f72 6561 6c5f 6469 7265  isting_real_dire
+00018000: 6374 6f72 795f 7379 6d6c 696e 6b28 7365  ctory_symlink(se
+00018010: 6c66 293a 0a20 2020 2020 2020 2066 616b  lf):.        fak
+00018020: 655f 6f70 656e 203d 2066 616b 655f 6669  e_open = fake_fi
+00018030: 6c65 7379 7374 656d 2e46 616b 6546 696c  lesystem.FakeFil
+00018040: 654f 7065 6e28 7365 6c66 2e66 696c 6573  eOpen(self.files
+00018050: 7973 7465 6d29 0a20 2020 2020 2020 2072  ystem).        r
+00018060: 6561 6c5f 6469 7265 6374 6f72 7920 3d20  eal_directory = 
+00018070: 7365 6c66 2e5f 7365 7475 705f 7465 6d70  self._setup_temp
+00018080: 5f64 6972 6563 746f 7279 2829 0a20 2020  _directory().   
+00018090: 2020 2020 2073 796d 6c69 6e6b 7320 3d20       symlinks = 
+000180a0: 5b0a 2020 2020 2020 2020 2020 2020 280a  [.            (.
+000180b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000180c0: 222e 2e22 2c0a 2020 2020 2020 2020 2020  "..",.          
+000180d0: 2020 2020 2020 6f73 2e70 6174 682e 6a6f        os.path.jo
+000180e0: 696e 2872 6561 6c5f 6469 7265 6374 6f72  in(real_director
+000180f0: 792c 2022 6669 7874 7572 6573 222c 2022  y, "fixtures", "
+00018100: 7379 6d6c 696e 6b5f 6469 725f 7265 6c61  symlink_dir_rela
+00018110: 7469 7665 2229 2c0a 2020 2020 2020 2020  tive"),.        
+00018120: 2020 2020 292c 0a20 2020 2020 2020 2020      ),.         
+00018130: 2020 2028 0a20 2020 2020 2020 2020 2020     (.           
+00018140: 2020 2020 2022 2e2e 2f61 6c6c 5f74 6573       "../all_tes
+00018150: 7473 2e70 7922 2c0a 2020 2020 2020 2020  ts.py",.        
+00018160: 2020 2020 2020 2020 6f73 2e70 6174 682e          os.path.
+00018170: 6a6f 696e 2872 6561 6c5f 6469 7265 6374  join(real_direct
+00018180: 6f72 792c 2022 6669 7874 7572 6573 222c  ory, "fixtures",
+00018190: 2022 7379 6d6c 696e 6b5f 6669 6c65 5f72   "symlink_file_r
+000181a0: 656c 6174 6976 6522 292c 0a20 2020 2020  elative"),.     
+000181b0: 2020 2020 2020 2029 2c0a 2020 2020 2020         ),.      
+000181c0: 2020 2020 2020 280a 2020 2020 2020 2020        (.        
+000181d0: 2020 2020 2020 2020 7265 616c 5f64 6972          real_dir
+000181e0: 6563 746f 7279 2c0a 2020 2020 2020 2020  ectory,.        
+000181f0: 2020 2020 2020 2020 6f73 2e70 6174 682e          os.path.
+00018200: 6a6f 696e 2872 6561 6c5f 6469 7265 6374  join(real_direct
+00018210: 6f72 792c 2022 6669 7874 7572 6573 222c  ory, "fixtures",
+00018220: 2022 7379 6d6c 696e 6b5f 6469 725f 6162   "symlink_dir_ab
+00018230: 736f 6c75 7465 2229 2c0a 2020 2020 2020  solute"),.      
+00018240: 2020 2020 2020 292c 0a20 2020 2020 2020        ),.       
+00018250: 2020 2020 2028 0a20 2020 2020 2020 2020       (.         
+00018260: 2020 2020 2020 206f 732e 7061 7468 2e6a         os.path.j
+00018270: 6f69 6e28 7265 616c 5f64 6972 6563 746f  oin(real_directo
+00018280: 7279 2c20 2261 6c6c 5f74 6573 7473 2e70  ry, "all_tests.p
+00018290: 7922 292c 0a20 2020 2020 2020 2020 2020  y"),.           
+000182a0: 2020 2020 206f 732e 7061 7468 2e6a 6f69       os.path.joi
+000182b0: 6e28 7265 616c 5f64 6972 6563 746f 7279  n(real_directory
+000182c0: 2c20 2266 6978 7475 7265 7322 2c20 2273  , "fixtures", "s
+000182d0: 796d 6c69 6e6b 5f66 696c 655f 6162 736f  ymlink_file_abso
+000182e0: 6c75 7465 2229 2c0a 2020 2020 2020 2020  lute"),.        
+000182f0: 2020 2020 292c 0a20 2020 2020 2020 2020      ),.         
+00018300: 2020 2028 0a20 2020 2020 2020 2020 2020     (.           
+00018310: 2020 2020 2022 2f65 7463 2f73 6f6d 6574       "/etc/somet
+00018320: 6869 6e67 222c 0a20 2020 2020 2020 2020  hing",.         
+00018330: 2020 2020 2020 206f 732e 7061 7468 2e6a         os.path.j
+00018340: 6f69 6e28 0a20 2020 2020 2020 2020 2020  oin(.           
+00018350: 2020 2020 2020 2020 2072 6561 6c5f 6469           real_di
+00018360: 7265 6374 6f72 792c 2022 6669 7874 7572  rectory, "fixtur
+00018370: 6573 222c 2022 7379 6d6c 696e 6b5f 6669  es", "symlink_fi
+00018380: 6c65 5f61 6273 6f6c 7574 655f 6f75 7473  le_absolute_outs
+00018390: 6964 6522 0a20 2020 2020 2020 2020 2020  ide".           
+000183a0: 2020 2020 2029 2c0a 2020 2020 2020 2020       ),.        
+000183b0: 2020 2020 292c 0a20 2020 2020 2020 205d      ),.        ]
+000183c0: 0a0a 2020 2020 2020 2020 7365 6c66 2e66  ..        self.f
+000183d0: 696c 6573 7973 7465 6d2e 6372 6561 7465  ilesystem.create
+000183e0: 5f66 696c 6528 222f 6574 632f 736f 6d65  _file("/etc/some
+000183f0: 7468 696e 6722 290a 0a20 2020 2020 2020  thing")..       
+00018400: 2077 6974 6820 6661 6b65 5f6f 7065 6e28   with fake_open(
+00018410: 222f 6574 632f 736f 6d65 7468 696e 6722  "/etc/something"
+00018420: 2c20 2277 222c 2065 6e63 6f64 696e 673d  , "w", encoding=
+00018430: 2275 7466 3822 2920 6173 2066 3a0a 2020  "utf8") as f:.  
+00018440: 2020 2020 2020 2020 2020 662e 7772 6974            f.writ
+00018450: 6528 2267 6f6f 6420 6d6f 726e 696e 6722  e("good morning"
+00018460: 290a 0a20 2020 2020 2020 2074 7279 3a0a  )..        try:.
+00018470: 2020 2020 2020 2020 2020 2020 7769 7468              with
+00018480: 2073 656c 662e 6372 6561 7465 5f73 796d   self.create_sym
+00018490: 6c69 6e6b 7328 7379 6d6c 696e 6b73 293a  links(symlinks):
+000184a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000184b0: 2073 656c 662e 6669 6c65 7379 7374 656d   self.filesystem
+000184c0: 2e61 6464 5f72 6561 6c5f 6469 7265 6374  .add_real_direct
+000184d0: 6f72 7928 7265 616c 5f64 6972 6563 746f  ory(real_directo
+000184e0: 7279 2c20 6c61 7a79 5f72 6561 643d 4661  ry, lazy_read=Fa
+000184f0: 6c73 6529 0a20 2020 2020 2020 2065 7863  lse).        exc
+00018500: 6570 7420 4f53 4572 726f 723a 0a20 2020  ept OSError:.   
+00018510: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
+00018520: 2e69 735f 7769 6e64 6f77 733a 0a20 2020  .is_windows:.   
+00018530: 2020 2020 2020 2020 2020 2020 2072 6169               rai
+00018540: 7365 2075 6e69 7474 6573 742e 536b 6970  se unittest.Skip
+00018550: 5465 7374 2822 5379 6d6c 696e 6b73 2075  Test("Symlinks u
+00018560: 6e64 6572 2057 696e 646f 7773 206e 6565  nder Windows nee
+00018570: 6420 6164 6d69 6e20 7072 6976 696c 6567  d admin privileg
+00018580: 6573 2229 0a20 2020 2020 2020 2020 2020  es").           
+00018590: 2072 6169 7365 0a0a 2020 2020 2020 2020   raise..        
+000185a0: 666f 7220 6c69 6e6b 2069 6e20 7379 6d6c  for link in syml
+000185b0: 696e 6b73 3a0a 2020 2020 2020 2020 2020  inks:.          
+000185c0: 2020 7365 6c66 2e61 7373 6572 7454 7275    self.assertTru
+000185d0: 6528 7365 6c66 2e66 696c 6573 7973 7465  e(self.filesyste
+000185e0: 6d2e 6973 6c69 6e6b 286c 696e 6b5b 315d  m.islink(link[1]
+000185f0: 2929 0a0a 2020 2020 2020 2020 2320 7265  ))..        # re
+00018600: 6c61 7469 7665 0a20 2020 2020 2020 2073  lative.        s
+00018610: 656c 662e 6173 7365 7274 5472 7565 280a  elf.assertTrue(.
+00018620: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00018630: 2e66 696c 6573 7973 7465 6d2e 6578 6973  .filesystem.exis
+00018640: 7473 280a 2020 2020 2020 2020 2020 2020  ts(.            
+00018650: 2020 2020 6f73 2e70 6174 682e 6a6f 696e      os.path.join
+00018660: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00018670: 2020 2020 2020 7265 616c 5f64 6972 6563        real_direc
+00018680: 746f 7279 2c0a 2020 2020 2020 2020 2020  tory,.          
+00018690: 2020 2020 2020 2020 2020 2266 6978 7475            "fixtu
+000186a0: 7265 732f 7379 6d6c 696e 6b5f 6469 725f  res/symlink_dir_
+000186b0: 7265 6c61 7469 7665 222c 0a20 2020 2020  relative",.     
+000186c0: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+000186d0: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+000186e0: 2020 2029 0a20 2020 2020 2020 2073 656c     ).        sel
+000186f0: 662e 6173 7365 7274 5472 7565 280a 2020  f.assertTrue(.  
+00018700: 2020 2020 2020 2020 2020 7365 6c66 2e66            self.f
+00018710: 696c 6573 7973 7465 6d2e 6578 6973 7473  ilesystem.exists
+00018720: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00018730: 2020 6f73 2e70 6174 682e 6a6f 696e 280a    os.path.join(.
+00018740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018750: 2020 2020 7265 616c 5f64 6972 6563 746f      real_directo
+00018760: 7279 2c0a 2020 2020 2020 2020 2020 2020  ry,.            
+00018770: 2020 2020 2020 2020 2266 6978 7475 7265          "fixture
+00018780: 732f 7379 6d6c 696e 6b5f 6469 725f 7265  s/symlink_dir_re
+00018790: 6c61 7469 7665 2f61 6c6c 5f74 6573 7473  lative/all_tests
+000187a0: 2e70 7922 2c0a 2020 2020 2020 2020 2020  .py",.          
+000187b0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+000187c0: 2020 2020 290a 2020 2020 2020 2020 290a      ).        ).
+000187d0: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+000187e0: 6572 7454 7275 6528 0a20 2020 2020 2020  ertTrue(.       
+000187f0: 2020 2020 2073 656c 662e 6669 6c65 7379       self.filesy
+00018800: 7374 656d 2e65 7869 7374 7328 0a20 2020  stem.exists(.   
+00018810: 2020 2020 2020 2020 2020 2020 206f 732e               os.
+00018820: 7061 7468 2e6a 6f69 6e28 0a20 2020 2020  path.join(.     
+00018830: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00018840: 6561 6c5f 6469 7265 6374 6f72 792c 0a20  eal_directory,. 
+00018850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018860: 2020 2022 6669 7874 7572 6573 2f73 796d     "fixtures/sym
+00018870: 6c69 6e6b 5f66 696c 655f 7265 6c61 7469  link_file_relati
+00018880: 7665 222c 0a20 2020 2020 2020 2020 2020  ve",.           
+00018890: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
+000188a0: 2020 2029 0a20 2020 2020 2020 2029 0a0a     ).        )..
+000188b0: 2020 2020 2020 2020 2320 6162 736f 6c75          # absolu
+000188c0: 7465 0a20 2020 2020 2020 2073 656c 662e  te.        self.
+000188d0: 6173 7365 7274 5472 7565 280a 2020 2020  assertTrue(.    
+000188e0: 2020 2020 2020 2020 7365 6c66 2e66 696c          self.fil
+000188f0: 6573 7973 7465 6d2e 6578 6973 7473 280a  esystem.exists(.
+00018900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018910: 6f73 2e70 6174 682e 6a6f 696e 280a 2020  os.path.join(.  
+00018920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018930: 2020 7265 616c 5f64 6972 6563 746f 7279    real_directory
+00018940: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00018950: 2020 2020 2020 2266 6978 7475 7265 732f        "fixtures/
+00018960: 7379 6d6c 696e 6b5f 6469 725f 6162 736f  symlink_dir_abso
+00018970: 6c75 7465 222c 0a20 2020 2020 2020 2020  lute",.         
+00018980: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00018990: 2020 2020 2029 0a20 2020 2020 2020 2029       ).        )
+000189a0: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
+000189b0: 7365 7274 5472 7565 280a 2020 2020 2020  sertTrue(.      
+000189c0: 2020 2020 2020 7365 6c66 2e66 696c 6573        self.files
+000189d0: 7973 7465 6d2e 6578 6973 7473 280a 2020  ystem.exists(.  
+000189e0: 2020 2020 2020 2020 2020 2020 2020 6f73                os
+000189f0: 2e70 6174 682e 6a6f 696e 280a 2020 2020  .path.join(.    
+00018a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018a10: 7265 616c 5f64 6972 6563 746f 7279 2c0a  real_directory,.
+00018a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018a30: 2020 2020 2266 6978 7475 7265 732f 7379      "fixtures/sy
+00018a40: 6d6c 696e 6b5f 6469 725f 6162 736f 6c75  mlink_dir_absolu
+00018a50: 7465 2f61 6c6c 5f74 6573 7473 2e70 7922  te/all_tests.py"
+00018a60: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00018a70: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
+00018a80: 290a 2020 2020 2020 2020 290a 2020 2020  ).        ).    
+00018a90: 2020 2020 7365 6c66 2e61 7373 6572 7454      self.assertT
+00018aa0: 7275 6528 0a20 2020 2020 2020 2020 2020  rue(.           
+00018ab0: 2073 656c 662e 6669 6c65 7379 7374 656d   self.filesystem
+00018ac0: 2e65 7869 7374 7328 0a20 2020 2020 2020  .exists(.       
+00018ad0: 2020 2020 2020 2020 206f 732e 7061 7468           os.path
+00018ae0: 2e6a 6f69 6e28 0a20 2020 2020 2020 2020  .join(.         
+00018af0: 2020 2020 2020 2020 2020 2072 6561 6c5f             real_
+00018b00: 6469 7265 6374 6f72 792c 0a20 2020 2020  directory,.     
+00018b10: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00018b20: 6669 7874 7572 6573 2f73 796d 6c69 6e6b  fixtures/symlink
+00018b30: 5f66 696c 655f 6162 736f 6c75 7465 222c  _file_absolute",
+00018b40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00018b50: 2029 0a20 2020 2020 2020 2020 2020 2029   ).            )
+00018b60: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
+00018b70: 2020 2020 2320 6f75 7473 6964 650a 2020      # outside.  
+00018b80: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+00018b90: 7454 7275 6528 0a20 2020 2020 2020 2020  tTrue(.         
+00018ba0: 2020 2073 656c 662e 6669 6c65 7379 7374     self.filesyst
+00018bb0: 656d 2e65 7869 7374 7328 0a20 2020 2020  em.exists(.     
+00018bc0: 2020 2020 2020 2020 2020 206f 732e 7061             os.pa
+00018bd0: 7468 2e6a 6f69 6e28 0a20 2020 2020 2020  th.join(.       
+00018be0: 2020 2020 2020 2020 2020 2020 2072 6561               rea
+00018bf0: 6c5f 6469 7265 6374 6f72 792c 0a20 2020  l_directory,.   
 00018c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018c10: 2073 656c 662e 726f 6f74 5f70 6174 682c   self.root_path,
-00018c20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00018c30: 2020 2020 2022 7079 6661 6b65 6673 222c       "pyfakefs",
-00018c40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00018c50: 2020 2020 2022 7465 7374 7322 2c0a 2020       "tests",.  
-00018c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018c70: 2020 2266 6978 7475 7265 732f 7379 6d6c    "fixtures/syml
-00018c80: 696e 6b5f 6669 6c65 5f61 6273 6f6c 7574  ink_file_absolut
-00018c90: 655f 6f75 7473 6964 6522 2c0a 2020 2020  e_outside",.    
-00018ca0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-00018cb0: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-00018cc0: 2020 2020 290a 2020 2020 2020 2020 7365      ).        se
-00018cd0: 6c66 2e61 7373 6572 7445 7175 616c 280a  lf.assertEqual(.
-00018ce0: 2020 2020 2020 2020 2020 2020 6661 6b65              fake
-00018cf0: 5f6f 7065 6e28 0a20 2020 2020 2020 2020  _open(.         
-00018d00: 2020 2020 2020 206f 732e 7061 7468 2e6a         os.path.j
-00018d10: 6f69 6e28 0a20 2020 2020 2020 2020 2020  oin(.           
-00018d20: 2020 2020 2020 2020 2073 656c 662e 726f           self.ro
-00018d30: 6f74 5f70 6174 682c 0a20 2020 2020 2020  ot_path,.       
-00018d40: 2020 2020 2020 2020 2020 2020 2022 7079               "py
-00018d50: 6661 6b65 6673 222c 0a20 2020 2020 2020  fakefs",.       
-00018d60: 2020 2020 2020 2020 2020 2020 2022 7465               "te
-00018d70: 7374 7322 2c0a 2020 2020 2020 2020 2020  sts",.          
-00018d80: 2020 2020 2020 2020 2020 2266 6978 7475            "fixtu
-00018d90: 7265 732f 7379 6d6c 696e 6b5f 6669 6c65  res/symlink_file
-00018da0: 5f61 6273 6f6c 7574 655f 6f75 7473 6964  _absolute_outsid
-00018db0: 6522 2c0a 2020 2020 2020 2020 2020 2020  e",.            
-00018dc0: 2020 2020 292c 0a20 2020 2020 2020 2020      ),.         
-00018dd0: 2020 2020 2020 2065 6e63 6f64 696e 673d         encoding=
-00018de0: 2275 7466 3822 2c0a 2020 2020 2020 2020  "utf8",.        
-00018df0: 2020 2020 292e 7265 6164 2829 2c0a 2020      ).read(),.  
-00018e00: 2020 2020 2020 2020 2020 2267 6f6f 6420            "good 
-00018e10: 6d6f 726e 696e 6722 2c0a 2020 2020 2020  morning",.      
-00018e20: 2020 290a 0a20 2020 2064 6566 2074 6573    )..    def tes
-00018e30: 745f 6164 645f 6578 6973 7469 6e67 5f72  t_add_existing_r
-00018e40: 6561 6c5f 6469 7265 6374 6f72 795f 7379  eal_directory_sy
-00018e50: 6d6c 696e 6b5f 7461 7267 6574 5f70 6174  mlink_target_pat
-00018e60: 6828 7365 6c66 293a 0a20 2020 2020 2020  h(self):.       
-00018e70: 2073 656c 662e 736b 6970 5f69 665f 7379   self.skip_if_sy
-00018e80: 6d6c 696e 6b5f 6e6f 745f 7375 7070 6f72  mlink_not_suppor
-00018e90: 7465 6428 666f 7263 655f 7265 616c 5f66  ted(force_real_f
-00018ea0: 733d 5472 7565 290a 2020 2020 2020 2020  s=True).        
-00018eb0: 7265 616c 5f64 6972 6563 746f 7279 203d  real_directory =
-00018ec0: 206f 732e 7061 7468 2e6a 6f69 6e28 7365   os.path.join(se
-00018ed0: 6c66 2e72 6f6f 745f 7061 7468 2c20 2270  lf.root_path, "p
-00018ee0: 7966 616b 6566 7322 2c20 2274 6573 7473  yfakefs", "tests
-00018ef0: 2229 0a20 2020 2020 2020 2073 796d 6c69  ").        symli
-00018f00: 6e6b 7320 3d20 5b0a 2020 2020 2020 2020  nks = [.        
-00018f10: 2020 2020 280a 2020 2020 2020 2020 2020      (.          
-00018f20: 2020 2020 2020 222e 2e22 2c0a 2020 2020        "..",.    
-00018f30: 2020 2020 2020 2020 2020 2020 6f73 2e70              os.p
-00018f40: 6174 682e 6a6f 696e 2872 6561 6c5f 6469  ath.join(real_di
-00018f50: 7265 6374 6f72 792c 2022 6669 7874 7572  rectory, "fixtur
-00018f60: 6573 222c 2022 7379 6d6c 696e 6b5f 6469  es", "symlink_di
-00018f70: 725f 7265 6c61 7469 7665 2229 2c0a 2020  r_relative"),.  
-00018f80: 2020 2020 2020 2020 2020 292c 0a20 2020            ),.   
-00018f90: 2020 2020 2020 2020 2028 0a20 2020 2020           (.     
-00018fa0: 2020 2020 2020 2020 2020 2022 2e2e 2f61             "../a
-00018fb0: 6c6c 5f74 6573 7473 2e70 7922 2c0a 2020  ll_tests.py",.  
-00018fc0: 2020 2020 2020 2020 2020 2020 2020 6f73                os
-00018fd0: 2e70 6174 682e 6a6f 696e 2872 6561 6c5f  .path.join(real_
-00018fe0: 6469 7265 6374 6f72 792c 2022 6669 7874  directory, "fixt
-00018ff0: 7572 6573 222c 2022 7379 6d6c 696e 6b5f  ures", "symlink_
-00019000: 6669 6c65 5f72 656c 6174 6976 6522 292c  file_relative"),
-00019010: 0a20 2020 2020 2020 2020 2020 2029 2c0a  .            ),.
-00019020: 2020 2020 2020 2020 5d0a 0a20 2020 2020          ]..     
-00019030: 2020 2077 6974 6820 7365 6c66 2e63 7265     with self.cre
-00019040: 6174 655f 7379 6d6c 696e 6b73 2873 796d  ate_symlinks(sym
-00019050: 6c69 6e6b 7329 3a0a 2020 2020 2020 2020  links):.        
-00019060: 2020 2020 7365 6c66 2e66 696c 6573 7973      self.filesys
-00019070: 7465 6d2e 6164 645f 7265 616c 5f64 6972  tem.add_real_dir
-00019080: 6563 746f 7279 280a 2020 2020 2020 2020  ectory(.        
-00019090: 2020 2020 2020 2020 7265 616c 5f64 6972          real_dir
-000190a0: 6563 746f 7279 2c20 7461 7267 6574 5f70  ectory, target_p
-000190b0: 6174 683d 222f 7061 7468 222c 206c 617a  ath="/path", laz
-000190c0: 795f 7265 6164 3d46 616c 7365 0a20 2020  y_read=False.   
-000190d0: 2020 2020 2020 2020 2029 0a0a 2020 2020           )..    
-000190e0: 2020 2020 7365 6c66 2e61 7373 6572 7454      self.assertT
-000190f0: 7275 6528 7365 6c66 2e66 696c 6573 7973  rue(self.filesys
-00019100: 7465 6d2e 6578 6973 7473 2822 2f70 6174  tem.exists("/pat
-00019110: 682f 6669 7874 7572 6573 2f73 796d 6c69  h/fixtures/symli
-00019120: 6e6b 5f64 6972 5f72 656c 6174 6976 6522  nk_dir_relative"
-00019130: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
-00019140: 6173 7365 7274 5472 7565 280a 2020 2020  assertTrue(.    
-00019150: 2020 2020 2020 2020 7365 6c66 2e66 696c          self.fil
-00019160: 6573 7973 7465 6d2e 6578 6973 7473 2822  esystem.exists("
-00019170: 2f70 6174 682f 6669 7874 7572 6573 2f73  /path/fixtures/s
-00019180: 796d 6c69 6e6b 5f64 6972 5f72 656c 6174  ymlink_dir_relat
-00019190: 6976 652f 616c 6c5f 7465 7374 732e 7079  ive/all_tests.py
-000191a0: 2229 0a20 2020 2020 2020 2029 0a20 2020  ").        ).   
-000191b0: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-000191c0: 5472 7565 2873 656c 662e 6669 6c65 7379  True(self.filesy
-000191d0: 7374 656d 2e65 7869 7374 7328 222f 7061  stem.exists("/pa
-000191e0: 7468 2f66 6978 7475 7265 732f 7379 6d6c  th/fixtures/syml
-000191f0: 696e 6b5f 6669 6c65 5f72 656c 6174 6976  ink_file_relativ
-00019200: 6522 2929 0a0a 2020 2020 6465 6620 7465  e"))..    def te
-00019210: 7374 5f61 6464 5f65 7869 7374 696e 675f  st_add_existing_
-00019220: 7265 616c 5f64 6972 6563 746f 7279 5f73  real_directory_s
-00019230: 796d 6c69 6e6b 5f6c 617a 795f 7265 6164  ymlink_lazy_read
-00019240: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-00019250: 7365 6c66 2e73 6b69 705f 6966 5f73 796d  self.skip_if_sym
-00019260: 6c69 6e6b 5f6e 6f74 5f73 7570 706f 7274  link_not_support
-00019270: 6564 2866 6f72 6365 5f72 6561 6c5f 6673  ed(force_real_fs
-00019280: 3d54 7275 6529 0a20 2020 2020 2020 2072  =True).        r
-00019290: 6561 6c5f 6469 7265 6374 6f72 7920 3d20  eal_directory = 
-000192a0: 6f73 2e70 6174 682e 6a6f 696e 2873 656c  os.path.join(sel
-000192b0: 662e 726f 6f74 5f70 6174 682c 2022 7079  f.root_path, "py
-000192c0: 6661 6b65 6673 222c 2022 7465 7374 7322  fakefs", "tests"
-000192d0: 290a 2020 2020 2020 2020 7379 6d6c 696e  ).        symlin
-000192e0: 6b73 203d 205b 0a20 2020 2020 2020 2020  ks = [.         
-000192f0: 2020 2028 0a20 2020 2020 2020 2020 2020     (.           
-00019300: 2020 2020 2022 2e2e 222c 0a20 2020 2020       "..",.     
-00019310: 2020 2020 2020 2020 2020 206f 732e 7061             os.pa
-00019320: 7468 2e6a 6f69 6e28 7265 616c 5f64 6972  th.join(real_dir
-00019330: 6563 746f 7279 2c20 2266 6978 7475 7265  ectory, "fixture
-00019340: 7322 2c20 2273 796d 6c69 6e6b 5f64 6972  s", "symlink_dir
-00019350: 5f72 656c 6174 6976 6522 292c 0a20 2020  _relative"),.   
-00019360: 2020 2020 2020 2020 2029 2c0a 2020 2020           ),.    
-00019370: 2020 2020 2020 2020 280a 2020 2020 2020          (.      
-00019380: 2020 2020 2020 2020 2020 222e 2e2f 616c            "../al
-00019390: 6c5f 7465 7374 732e 7079 222c 0a20 2020  l_tests.py",.   
-000193a0: 2020 2020 2020 2020 2020 2020 206f 732e               os.
-000193b0: 7061 7468 2e6a 6f69 6e28 7265 616c 5f64  path.join(real_d
-000193c0: 6972 6563 746f 7279 2c20 2266 6978 7475  irectory, "fixtu
-000193d0: 7265 7322 2c20 2273 796d 6c69 6e6b 5f66  res", "symlink_f
-000193e0: 696c 655f 7265 6c61 7469 7665 2229 2c0a  ile_relative"),.
-000193f0: 2020 2020 2020 2020 2020 2020 292c 0a20              ),. 
-00019400: 2020 2020 2020 205d 0a0a 2020 2020 2020         ]..      
-00019410: 2020 7769 7468 2073 656c 662e 6372 6561    with self.crea
-00019420: 7465 5f73 796d 6c69 6e6b 7328 7379 6d6c  te_symlinks(syml
-00019430: 696e 6b73 293a 0a20 2020 2020 2020 2020  inks):.         
-00019440: 2020 2073 656c 662e 6669 6c65 7379 7374     self.filesyst
-00019450: 656d 2e61 6464 5f72 6561 6c5f 6469 7265  em.add_real_dire
-00019460: 6374 6f72 7928 0a20 2020 2020 2020 2020  ctory(.         
-00019470: 2020 2020 2020 2072 6561 6c5f 6469 7265         real_dire
-00019480: 6374 6f72 792c 2074 6172 6765 745f 7061  ctory, target_pa
-00019490: 7468 3d22 2f70 6174 6822 2c20 6c61 7a79  th="/path", lazy
-000194a0: 5f72 6561 643d 5472 7565 0a20 2020 2020  _read=True.     
-000194b0: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
-000194c0: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
-000194d0: 7454 7275 6528 0a20 2020 2020 2020 2020  tTrue(.         
-000194e0: 2020 2020 2020 2073 656c 662e 6669 6c65         self.file
-000194f0: 7379 7374 656d 2e65 7869 7374 7328 222f  system.exists("/
-00019500: 7061 7468 2f66 6978 7475 7265 732f 7379  path/fixtures/sy
-00019510: 6d6c 696e 6b5f 6469 725f 7265 6c61 7469  mlink_dir_relati
-00019520: 7665 2229 0a20 2020 2020 2020 2020 2020  ve").           
-00019530: 2029 0a20 2020 2020 2020 2020 2020 2073   ).            s
-00019540: 656c 662e 6173 7365 7274 5472 7565 280a  elf.assertTrue(.
-00019550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019560: 7365 6c66 2e66 696c 6573 7973 7465 6d2e  self.filesystem.
-00019570: 6578 6973 7473 280a 2020 2020 2020 2020  exists(.        
-00019580: 2020 2020 2020 2020 2020 2020 222f 7061              "/pa
-00019590: 7468 2f66 6978 7475 7265 732f 7379 6d6c  th/fixtures/syml
-000195a0: 696e 6b5f 6469 725f 7265 6c61 7469 7665  ink_dir_relative
-000195b0: 2f61 6c6c 5f74 6573 7473 2e70 7922 0a20  /all_tests.py". 
-000195c0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-000195d0: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
-000195e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000195f0: 6173 7365 7274 5472 7565 280a 2020 2020  assertTrue(.    
-00019600: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00019610: 2e66 696c 6573 7973 7465 6d2e 6578 6973  .filesystem.exis
-00019620: 7473 2822 2f70 6174 682f 6669 7874 7572  ts("/path/fixtur
-00019630: 6573 2f73 796d 6c69 6e6b 5f66 696c 655f  es/symlink_file_
-00019640: 7265 6c61 7469 7665 2229 0a20 2020 2020  relative").     
-00019650: 2020 2020 2020 2029 0a0a 2020 2020 6465         )..    de
-00019660: 6620 7465 7374 5f61 6464 5f65 7869 7374  f test_add_exist
-00019670: 696e 675f 7265 616c 5f64 6972 6563 746f  ing_real_directo
-00019680: 7279 5f74 7265 655f 746f 5f6f 7468 6572  ry_tree_to_other
-00019690: 5f70 6174 6828 7365 6c66 293a 0a20 2020  _path(self):.   
-000196a0: 2020 2020 2073 656c 662e 6669 6c65 7379       self.filesy
-000196b0: 7374 656d 2e61 6464 5f72 6561 6c5f 6469  stem.add_real_di
-000196c0: 7265 6374 6f72 7928 7365 6c66 2e72 6f6f  rectory(self.roo
-000196d0: 745f 7061 7468 2c20 7461 7267 6574 5f70  t_path, target_p
-000196e0: 6174 683d 222f 666f 6f2f 6261 7222 290a  ath="/foo/bar").
-000196f0: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-00019700: 6572 7446 616c 7365 280a 2020 2020 2020  ertFalse(.      
-00019710: 2020 2020 2020 7365 6c66 2e66 696c 6573        self.files
-00019720: 7973 7465 6d2e 6578 6973 7473 280a 2020  ystem.exists(.  
-00019730: 2020 2020 2020 2020 2020 2020 2020 6f73                os
-00019740: 2e70 6174 682e 6a6f 696e 2873 656c 662e  .path.join(self.
-00019750: 7079 6661 6b65 6673 5f70 6174 682c 2022  pyfakefs_path, "
-00019760: 7465 7374 7322 2c20 2266 616b 655f 6669  tests", "fake_fi
-00019770: 6c65 7379 7374 656d 5f74 6573 742e 7079  lesystem_test.py
-00019780: 2229 0a20 2020 2020 2020 2020 2020 2029  ").            )
-00019790: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
-000197a0: 2020 2073 656c 662e 6173 7365 7274 5472     self.assertTr
-000197b0: 7565 280a 2020 2020 2020 2020 2020 2020  ue(.            
-000197c0: 7365 6c66 2e66 696c 6573 7973 7465 6d2e  self.filesystem.
-000197d0: 6578 6973 7473 280a 2020 2020 2020 2020  exists(.        
-000197e0: 2020 2020 2020 2020 6f73 2e70 6174 682e          os.path.
-000197f0: 6a6f 696e 280a 2020 2020 2020 2020 2020  join(.          
-00019800: 2020 2020 2020 2020 2020 2266 6f6f 222c            "foo",
-00019810: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00019820: 2020 2020 2022 6261 7222 2c0a 2020 2020       "bar",.    
-00019830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019840: 2270 7966 616b 6566 7322 2c0a 2020 2020  "pyfakefs",.    
-00019850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019860: 2274 6573 7473 222c 0a20 2020 2020 2020  "tests",.       
-00019870: 2020 2020 2020 2020 2020 2020 2022 6661               "fa
-00019880: 6b65 5f66 696c 6573 7973 7465 6d5f 7465  ke_filesystem_te
-00019890: 7374 2e70 7922 2c0a 2020 2020 2020 2020  st.py",.        
-000198a0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-000198b0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-000198c0: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
-000198d0: 7373 6572 7446 616c 7365 280a 2020 2020  ssertFalse(.    
-000198e0: 2020 2020 2020 2020 7365 6c66 2e66 696c          self.fil
-000198f0: 6573 7973 7465 6d2e 6578 6973 7473 280a  esystem.exists(.
-00019900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019910: 6f73 2e70 6174 682e 6a6f 696e 2873 656c  os.path.join(sel
-00019920: 662e 726f 6f74 5f70 6174 682c 2022 7079  f.root_path, "py
-00019930: 6661 6b65 6673 222c 2022 6661 6b65 5f66  fakefs", "fake_f
-00019940: 696c 6573 7973 7465 6d2e 7079 2229 0a20  ilesystem.py"). 
-00019950: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-00019960: 2020 2020 2029 0a20 2020 2020 2020 2073       ).        s
-00019970: 656c 662e 6173 7365 7274 5472 7565 280a  elf.assertTrue(.
-00019980: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00019990: 2e66 696c 6573 7973 7465 6d2e 6578 6973  .filesystem.exis
-000199a0: 7473 280a 2020 2020 2020 2020 2020 2020  ts(.            
-000199b0: 2020 2020 6f73 2e70 6174 682e 6a6f 696e      os.path.join
-000199c0: 2822 666f 6f22 2c20 2262 6172 222c 2022  ("foo", "bar", "
-000199d0: 7079 6661 6b65 6673 222c 2022 5f5f 696e  pyfakefs", "__in
-000199e0: 6974 5f5f 2e70 7922 290a 2020 2020 2020  it__.py").      
-000199f0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-00019a00: 290a 0a20 2020 2064 6566 2074 6573 745f  )..    def test_
-00019a10: 6765 745f 6f62 6a65 6374 5f66 726f 6d5f  get_object_from_
-00019a20: 6c61 7a69 6c79 5f61 6464 6564 5f72 6561  lazily_added_rea
-00019a30: 6c5f 6469 7265 6374 6f72 7928 7365 6c66  l_directory(self
-00019a40: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
-00019a50: 6669 6c65 7379 7374 656d 2e69 735f 6361  filesystem.is_ca
-00019a60: 7365 5f73 656e 7369 7469 7665 203d 2054  se_sensitive = T
-00019a70: 7275 650a 2020 2020 2020 2020 7365 6c66  rue.        self
-00019a80: 2e66 696c 6573 7973 7465 6d2e 6164 645f  .filesystem.add_
-00019a90: 7265 616c 5f64 6972 6563 746f 7279 2873  real_directory(s
-00019aa0: 656c 662e 726f 6f74 5f70 6174 6829 0a20  elf.root_path). 
-00019ab0: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-00019ac0: 7274 5472 7565 280a 2020 2020 2020 2020  rtTrue(.        
-00019ad0: 2020 2020 7365 6c66 2e66 696c 6573 7973      self.filesys
-00019ae0: 7465 6d2e 6765 745f 6f62 6a65 6374 280a  tem.get_object(.
-00019af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019b00: 6f73 2e70 6174 682e 6a6f 696e 2873 656c  os.path.join(sel
-00019b10: 662e 726f 6f74 5f70 6174 682c 2022 7079  f.root_path, "py
-00019b20: 6661 6b65 6673 222c 2022 6661 6b65 5f66  fakefs", "fake_f
-00019b30: 696c 6573 7973 7465 6d2e 7079 2229 0a20  ilesystem.py"). 
-00019b40: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-00019b50: 2020 2020 2029 0a20 2020 2020 2020 2073       ).        s
-00019b60: 656c 662e 6173 7365 7274 5472 7565 280a  elf.assertTrue(.
-00019b70: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00019b80: 2e66 696c 6573 7973 7465 6d2e 6765 745f  .filesystem.get_
-00019b90: 6f62 6a65 6374 280a 2020 2020 2020 2020  object(.        
-00019ba0: 2020 2020 2020 2020 6f73 2e70 6174 682e          os.path.
-00019bb0: 6a6f 696e 2873 656c 662e 726f 6f74 5f70  join(self.root_p
-00019bc0: 6174 682c 2022 7079 6661 6b65 6673 222c  ath, "pyfakefs",
-00019bd0: 2022 5f5f 696e 6974 5f5f 2e70 7922 290a   "__init__.py").
-00019be0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-00019bf0: 2020 2020 2020 290a 0a20 2020 2064 6566        )..    def
-00019c00: 2074 6573 745f 6164 645f 6578 6973 7469   test_add_existi
-00019c10: 6e67 5f72 6561 6c5f 6469 7265 6374 6f72  ng_real_director
-00019c20: 795f 6c61 7a69 6c79 2873 656c 6629 3a0a  y_lazily(self):.
-00019c30: 2020 2020 2020 2020 6469 736b 5f73 697a          disk_siz
-00019c40: 6520 3d20 3130 3234 202a 2031 3032 3420  e = 1024 * 1024 
-00019c50: 2a20 3130 3234 0a20 2020 2020 2020 2072  * 1024.        r
-00019c60: 6561 6c5f 6469 725f 7061 7468 203d 206f  eal_dir_path = o
-00019c70: 732e 7061 7468 2e6a 6f69 6e28 7365 6c66  s.path.join(self
-00019c80: 2e72 6f6f 745f 7061 7468 2c20 2270 7966  .root_path, "pyf
-00019c90: 616b 6566 7322 290a 2020 2020 2020 2020  akefs").        
-00019ca0: 7365 6c66 2e66 696c 6573 7973 7465 6d2e  self.filesystem.
-00019cb0: 7365 745f 6469 736b 5f75 7361 6765 2864  set_disk_usage(d
-00019cc0: 6973 6b5f 7369 7a65 2c20 7265 616c 5f64  isk_size, real_d
-00019cd0: 6972 5f70 6174 6829 0a20 2020 2020 2020  ir_path).       
-00019ce0: 2073 656c 662e 6669 6c65 7379 7374 656d   self.filesystem
-00019cf0: 2e61 6464 5f72 6561 6c5f 6469 7265 6374  .add_real_direct
-00019d00: 6f72 7928 7265 616c 5f64 6972 5f70 6174  ory(real_dir_pat
-00019d10: 6829 0a0a 2020 2020 2020 2020 2320 7468  h)..        # th
-00019d20: 6520 6469 7265 6374 6f72 7920 636f 6e74  e directory cont
-00019d30: 656e 7473 2068 6176 6520 6e6f 7420 6265  ents have not be
-00019d40: 656e 2072 6561 642c 2074 6865 2064 6973  en read, the dis
-00019d50: 6b20 7573 6167 650a 2020 2020 2020 2020  k usage.        
-00019d60: 2320 6861 7320 6e6f 7420 6368 616e 6765  # has not change
-00019d70: 640a 2020 2020 2020 2020 7365 6c66 2e61  d.        self.a
-00019d80: 7373 6572 7445 7175 616c 2864 6973 6b5f  ssertEqual(disk_
-00019d90: 7369 7a65 2c20 7365 6c66 2e66 696c 6573  size, self.files
-00019da0: 7973 7465 6d2e 6765 745f 6469 736b 5f75  ystem.get_disk_u
-00019db0: 7361 6765 2872 6561 6c5f 6469 725f 7061  sage(real_dir_pa
-00019dc0: 7468 292e 6672 6565 290a 2020 2020 2020  th).free).      
-00019dd0: 2020 2320 6368 6563 6b69 6e67 2066 6f72    # checking for
-00019de0: 2065 7869 7374 656e 6365 2073 6861 6c6c   existence shall
-00019df0: 2072 6561 6420 7468 6520 6469 7265 6374   read the direct
-00019e00: 6f72 7920 636f 6e74 656e 7473 0a20 2020  ory contents.   
-00019e10: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-00019e20: 5472 7565 280a 2020 2020 2020 2020 2020  True(.          
-00019e30: 2020 7365 6c66 2e66 696c 6573 7973 7465    self.filesyste
-00019e40: 6d2e 6765 745f 6f62 6a65 6374 280a 2020  m.get_object(.  
-00019e50: 2020 2020 2020 2020 2020 2020 2020 6f73                os
-00019e60: 2e70 6174 682e 6a6f 696e 2872 6561 6c5f  .path.join(real_
-00019e70: 6469 725f 7061 7468 2c20 2266 616b 655f  dir_path, "fake_
-00019e80: 6669 6c65 7379 7374 656d 2e70 7922 290a  filesystem.py").
-00019e90: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-00019ea0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-00019eb0: 2320 736f 206e 6f77 2074 6865 2066 7265  # so now the fre
-00019ec0: 6520 6469 736b 2073 7061 6365 2073 6861  e disk space sha
-00019ed0: 6c6c 2068 6176 6520 6465 6372 6561 7365  ll have decrease
-00019ee0: 640a 2020 2020 2020 2020 7365 6c66 2e61  d.        self.a
-00019ef0: 7373 6572 7447 7265 6174 6572 280a 2020  ssertGreater(.  
-00019f00: 2020 2020 2020 2020 2020 6469 736b 5f73            disk_s
-00019f10: 697a 652c 2073 656c 662e 6669 6c65 7379  ize, self.filesy
-00019f20: 7374 656d 2e67 6574 5f64 6973 6b5f 7573  stem.get_disk_us
-00019f30: 6167 6528 7265 616c 5f64 6972 5f70 6174  age(real_dir_pat
-00019f40: 6829 2e66 7265 650a 2020 2020 2020 2020  h).free.        
-00019f50: 290a 0a20 2020 2064 6566 2074 6573 745f  )..    def test_
-00019f60: 6164 645f 6578 6973 7469 6e67 5f72 6561  add_existing_rea
-00019f70: 6c5f 6469 7265 6374 6f72 795f 6e6f 745f  l_directory_not_
-00019f80: 6c61 7a69 6c79 2873 656c 6629 3a0a 2020  lazily(self):.  
-00019f90: 2020 2020 2020 6469 736b 5f73 697a 6520        disk_size 
-00019fa0: 3d20 3130 3234 202a 2031 3032 3420 2a20  = 1024 * 1024 * 
-00019fb0: 3130 3234 0a20 2020 2020 2020 2073 656c  1024.        sel
-00019fc0: 662e 6669 6c65 7379 7374 656d 2e73 6574  f.filesystem.set
-00019fd0: 5f64 6973 6b5f 7573 6167 6528 6469 736b  _disk_usage(disk
-00019fe0: 5f73 697a 652c 2073 656c 662e 7079 6661  _size, self.pyfa
-00019ff0: 6b65 6673 5f70 6174 6829 0a20 2020 2020  kefs_path).     
-0001a000: 2020 2073 656c 662e 6669 6c65 7379 7374     self.filesyst
-0001a010: 656d 2e61 6464 5f72 6561 6c5f 6469 7265  em.add_real_dire
-0001a020: 6374 6f72 7928 7365 6c66 2e70 7966 616b  ctory(self.pyfak
-0001a030: 6566 735f 7061 7468 2c20 6c61 7a79 5f72  efs_path, lazy_r
-0001a040: 6561 643d 4661 6c73 6529 0a0a 2020 2020  ead=False)..    
-0001a050: 2020 2020 2320 7468 6520 6469 7265 6374      # the direct
-0001a060: 6f72 7920 6861 7320 6265 656e 2072 6561  ory has been rea
-0001a070: 642c 2073 6f20 7468 6520 6669 6c65 2073  d, so the file s
-0001a080: 697a 6573 2068 6176 650a 2020 2020 2020  izes have.      
-0001a090: 2020 2320 6265 656e 2073 7562 7472 6163    # been subtrac
-0001a0a0: 7465 6420 6672 6f6d 2074 6865 2066 7265  ted from the fre
-0001a0b0: 6520 7370 6163 650a 2020 2020 2020 2020  e space.        
-0001a0c0: 7365 6c66 2e61 7373 6572 7447 7265 6174  self.assertGreat
-0001a0d0: 6572 280a 2020 2020 2020 2020 2020 2020  er(.            
-0001a0e0: 6469 736b 5f73 697a 652c 2073 656c 662e  disk_size, self.
-0001a0f0: 6669 6c65 7379 7374 656d 2e67 6574 5f64  filesystem.get_d
-0001a100: 6973 6b5f 7573 6167 6528 7365 6c66 2e70  isk_usage(self.p
-0001a110: 7966 616b 6566 735f 7061 7468 292e 6672  yfakefs_path).fr
-0001a120: 6565 0a20 2020 2020 2020 2029 0a0a 2020  ee.        )..  
-0001a130: 2020 6465 6620 7465 7374 5f61 6464 5f65    def test_add_e
-0001a140: 7869 7374 696e 675f 7265 616c 5f64 6972  xisting_real_dir
-0001a150: 6563 746f 7279 5f72 6561 645f 7772 6974  ectory_read_writ
-0001a160: 6528 7365 6c66 293a 0a20 2020 2020 2020  e(self):.       
-0001a170: 2073 656c 662e 6669 6c65 7379 7374 656d   self.filesystem
-0001a180: 2e61 6464 5f72 6561 6c5f 6469 7265 6374  .add_real_direct
-0001a190: 6f72 7928 7365 6c66 2e70 7966 616b 6566  ory(self.pyfakef
-0001a1a0: 735f 7061 7468 2c20 7265 6164 5f6f 6e6c  s_path, read_onl
-0001a1b0: 793d 4661 6c73 6529 0a20 2020 2020 2020  y=False).       
-0001a1c0: 2073 656c 662e 6173 7365 7274 5472 7565   self.assertTrue
-0001a1d0: 2873 656c 662e 6669 6c65 7379 7374 656d  (self.filesystem
-0001a1e0: 2e65 7869 7374 7328 7365 6c66 2e70 7966  .exists(self.pyf
-0001a1f0: 616b 6566 735f 7061 7468 2929 0a20 2020  akefs_path)).   
-0001a200: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-0001a210: 5472 7565 280a 2020 2020 2020 2020 2020  True(.          
-0001a220: 2020 7365 6c66 2e66 696c 6573 7973 7465    self.filesyste
-0001a230: 6d2e 6578 6973 7473 280a 2020 2020 2020  m.exists(.      
-0001a240: 2020 2020 2020 2020 2020 6f73 2e70 6174            os.pat
-0001a250: 682e 6a6f 696e 2873 656c 662e 7079 6661  h.join(self.pyfa
-0001a260: 6b65 6673 5f70 6174 682c 2022 6661 6b65  kefs_path, "fake
-0001a270: 5f66 696c 6573 7973 7465 6d2e 7079 2229  _filesystem.py")
-0001a280: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
-0001a290: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-0001a2a0: 2073 656c 662e 6173 7365 7274 5472 7565   self.assertTrue
-0001a2b0: 280a 2020 2020 2020 2020 2020 2020 7365  (.            se
-0001a2c0: 6c66 2e66 696c 6573 7973 7465 6d2e 6578  lf.filesystem.ex
-0001a2d0: 6973 7473 286f 732e 7061 7468 2e6a 6f69  ists(os.path.joi
-0001a2e0: 6e28 7365 6c66 2e70 7966 616b 6566 735f  n(self.pyfakefs_
-0001a2f0: 7061 7468 2c20 2266 616b 655f 7061 7468  path, "fake_path
-0001a300: 6c69 622e 7079 2229 290a 2020 2020 2020  lib.py")).      
-0001a310: 2020 290a 0a20 2020 2020 2020 2066 696c    )..        fil
-0001a320: 655f 7061 7468 203d 206f 732e 7061 7468  e_path = os.path
-0001a330: 2e6a 6f69 6e28 7365 6c66 2e70 7966 616b  .join(self.pyfak
-0001a340: 6566 735f 7061 7468 2c20 2270 7974 6573  efs_path, "pytes
-0001a350: 745f 706c 7567 696e 2e70 7922 290a 2020  t_plugin.py").  
-0001a360: 2020 2020 2020 6661 6b65 5f66 696c 6520        fake_file 
-0001a370: 3d20 7365 6c66 2e66 696c 6573 7973 7465  = self.filesyste
-0001a380: 6d2e 7265 736f 6c76 6528 6669 6c65 5f70  m.resolve(file_p
-0001a390: 6174 6829 0a20 2020 2020 2020 2073 656c  ath).        sel
-0001a3a0: 662e 6368 6563 6b5f 6661 6b65 5f66 696c  f.check_fake_fil
-0001a3b0: 655f 7374 6174 2866 616b 655f 6669 6c65  e_stat(fake_file
-0001a3c0: 2c20 6669 6c65 5f70 6174 6829 0a20 2020  , file_path).   
-0001a3d0: 2020 2020 2073 656c 662e 6368 6563 6b5f       self.check_
-0001a3e0: 7772 6974 6162 6c65 5f66 696c 6528 6661  writable_file(fa
-0001a3f0: 6b65 5f66 696c 652c 2066 696c 655f 7061  ke_file, file_pa
-0001a400: 7468 290a 0a20 2020 2064 6566 2074 6573  th)..    def tes
-0001a410: 745f 6164 645f 6578 6973 7469 6e67 5f72  t_add_existing_r
-0001a420: 6561 6c5f 7061 7468 735f 7265 6164 5f6f  eal_paths_read_o
-0001a430: 6e6c 7928 7365 6c66 293a 0a20 2020 2020  nly(self):.     
-0001a440: 2020 2072 6561 6c5f 6669 6c65 5f70 6174     real_file_pat
-0001a450: 6820 3d20 6f73 2e70 6174 682e 7265 616c  h = os.path.real
-0001a460: 7061 7468 285f 5f66 696c 655f 5f29 0a20  path(__file__). 
-0001a470: 2020 2020 2020 2066 6978 7475 7265 5f70         fixture_p
-0001a480: 6174 6820 3d20 6f73 2e70 6174 682e 6a6f  ath = os.path.jo
-0001a490: 696e 2873 656c 662e 7079 6661 6b65 6673  in(self.pyfakefs
-0001a4a0: 5f70 6174 682c 2022 7465 7374 7322 2c20  _path, "tests", 
-0001a4b0: 2266 6978 7475 7265 7322 290a 2020 2020  "fixtures").    
-0001a4c0: 2020 2020 7365 6c66 2e66 696c 6573 7973      self.filesys
-0001a4d0: 7465 6d2e 6164 645f 7265 616c 5f70 6174  tem.add_real_pat
-0001a4e0: 6873 285b 7265 616c 5f66 696c 655f 7061  hs([real_file_pa
-0001a4f0: 7468 2c20 6669 7874 7572 655f 7061 7468  th, fixture_path
-0001a500: 5d29 0a0a 2020 2020 2020 2020 6661 6b65  ])..        fake
-0001a510: 5f66 696c 6520 3d20 7365 6c66 2e66 696c  _file = self.fil
-0001a520: 6573 7973 7465 6d2e 7265 736f 6c76 6528  esystem.resolve(
-0001a530: 7265 616c 5f66 696c 655f 7061 7468 290a  real_file_path).
-0001a540: 2020 2020 2020 2020 7365 6c66 2e63 6865          self.che
-0001a550: 636b 5f66 616b 655f 6669 6c65 5f73 7461  ck_fake_file_sta
-0001a560: 7428 6661 6b65 5f66 696c 652c 2072 6561  t(fake_file, rea
-0001a570: 6c5f 6669 6c65 5f70 6174 6829 0a20 2020  l_file_path).   
-0001a580: 2020 2020 2073 656c 662e 6368 6563 6b5f       self.check_
-0001a590: 7265 6164 5f6f 6e6c 795f 6669 6c65 2866  read_only_file(f
-0001a5a0: 616b 655f 6669 6c65 2c20 7265 616c 5f66  ake_file, real_f
-0001a5b0: 696c 655f 7061 7468 290a 0a20 2020 2020  ile_path)..     
-0001a5c0: 2020 2072 6561 6c5f 6669 6c65 5f70 6174     real_file_pat
-0001a5d0: 6820 3d20 6f73 2e70 6174 682e 6a6f 696e  h = os.path.join
-0001a5e0: 2866 6978 7475 7265 5f70 6174 682c 2022  (fixture_path, "
-0001a5f0: 6d6f 6475 6c65 5f77 6974 685f 6174 7472  module_with_attr
-0001a600: 6962 7574 6573 2e70 7922 290a 2020 2020  ibutes.py").    
-0001a610: 2020 2020 6661 6b65 5f66 696c 6520 3d20      fake_file = 
-0001a620: 7365 6c66 2e66 696c 6573 7973 7465 6d2e  self.filesystem.
-0001a630: 7265 736f 6c76 6528 7265 616c 5f66 696c  resolve(real_fil
-0001a640: 655f 7061 7468 290a 2020 2020 2020 2020  e_path).        
-0001a650: 7365 6c66 2e63 6865 636b 5f66 616b 655f  self.check_fake_
-0001a660: 6669 6c65 5f73 7461 7428 6661 6b65 5f66  file_stat(fake_f
-0001a670: 696c 652c 2072 6561 6c5f 6669 6c65 5f70  ile, real_file_p
-0001a680: 6174 6829 0a20 2020 2020 2020 2073 656c  ath).        sel
-0001a690: 662e 6368 6563 6b5f 7265 6164 5f6f 6e6c  f.check_read_onl
-0001a6a0: 795f 6669 6c65 2866 616b 655f 6669 6c65  y_file(fake_file
-0001a6b0: 2c20 7265 616c 5f66 696c 655f 7061 7468  , real_file_path
-0001a6c0: 290a 0a20 2020 2064 6566 2074 6573 745f  )..    def test_
-0001a6d0: 6164 645f 6578 6973 7469 6e67 5f72 6561  add_existing_rea
-0001a6e0: 6c5f 7061 7468 735f 7265 6164 5f77 7269  l_paths_read_wri
-0001a6f0: 7465 2873 656c 6629 3a0a 2020 2020 2020  te(self):.      
-0001a700: 2020 7265 616c 5f66 696c 655f 7061 7468    real_file_path
-0001a710: 203d 206f 732e 7061 7468 2e72 6561 6c70   = os.path.realp
-0001a720: 6174 6828 5f5f 6669 6c65 5f5f 290a 2020  ath(__file__).  
-0001a730: 2020 2020 2020 6669 7874 7572 655f 7061        fixture_pa
-0001a740: 7468 203d 206f 732e 7061 7468 2e6a 6f69  th = os.path.joi
-0001a750: 6e28 7365 6c66 2e70 7966 616b 6566 735f  n(self.pyfakefs_
-0001a760: 7061 7468 2c20 2274 6573 7473 222c 2022  path, "tests", "
-0001a770: 6669 7874 7572 6573 2229 0a20 2020 2020  fixtures").     
-0001a780: 2020 2073 656c 662e 6669 6c65 7379 7374     self.filesyst
-0001a790: 656d 2e61 6464 5f72 6561 6c5f 7061 7468  em.add_real_path
-0001a7a0: 7328 5b72 6561 6c5f 6669 6c65 5f70 6174  s([real_file_pat
-0001a7b0: 682c 2066 6978 7475 7265 5f70 6174 685d  h, fixture_path]
-0001a7c0: 2c20 7265 6164 5f6f 6e6c 793d 4661 6c73  , read_only=Fals
-0001a7d0: 6529 0a0a 2020 2020 2020 2020 6661 6b65  e)..        fake
-0001a7e0: 5f66 696c 6520 3d20 7365 6c66 2e66 696c  _file = self.fil
-0001a7f0: 6573 7973 7465 6d2e 7265 736f 6c76 6528  esystem.resolve(
-0001a800: 7265 616c 5f66 696c 655f 7061 7468 290a  real_file_path).
-0001a810: 2020 2020 2020 2020 7365 6c66 2e63 6865          self.che
-0001a820: 636b 5f66 616b 655f 6669 6c65 5f73 7461  ck_fake_file_sta
-0001a830: 7428 6661 6b65 5f66 696c 652c 2072 6561  t(fake_file, rea
-0001a840: 6c5f 6669 6c65 5f70 6174 6829 0a20 2020  l_file_path).   
-0001a850: 2020 2020 2073 656c 662e 6368 6563 6b5f       self.check_
-0001a860: 7772 6974 6162 6c65 5f66 696c 6528 6661  writable_file(fa
-0001a870: 6b65 5f66 696c 652c 2072 6561 6c5f 6669  ke_file, real_fi
-0001a880: 6c65 5f70 6174 6829 0a0a 2020 2020 2020  le_path)..      
-0001a890: 2020 7265 616c 5f66 696c 655f 7061 7468    real_file_path
-0001a8a0: 203d 206f 732e 7061 7468 2e6a 6f69 6e28   = os.path.join(
-0001a8b0: 6669 7874 7572 655f 7061 7468 2c20 226d  fixture_path, "m
-0001a8c0: 6f64 756c 655f 7769 7468 5f61 7474 7269  odule_with_attri
-0001a8d0: 6275 7465 732e 7079 2229 0a20 2020 2020  butes.py").     
-0001a8e0: 2020 2066 616b 655f 6669 6c65 203d 2073     fake_file = s
-0001a8f0: 656c 662e 6669 6c65 7379 7374 656d 2e72  elf.filesystem.r
-0001a900: 6573 6f6c 7665 2872 6561 6c5f 6669 6c65  esolve(real_file
-0001a910: 5f70 6174 6829 0a20 2020 2020 2020 2073  _path).        s
-0001a920: 656c 662e 6368 6563 6b5f 6661 6b65 5f66  elf.check_fake_f
-0001a930: 696c 655f 7374 6174 2866 616b 655f 6669  ile_stat(fake_fi
-0001a940: 6c65 2c20 7265 616c 5f66 696c 655f 7061  le, real_file_pa
-0001a950: 7468 290a 2020 2020 2020 2020 7365 6c66  th).        self
-0001a960: 2e63 6865 636b 5f77 7269 7461 626c 655f  .check_writable_
-0001a970: 6669 6c65 2866 616b 655f 6669 6c65 2c20  file(fake_file, 
-0001a980: 7265 616c 5f66 696c 655f 7061 7468 290a  real_file_path).
-0001a990: 0a0a 636c 6173 7320 4669 6c65 5369 6465  ..class FileSide
-0001a9a0: 4566 6665 6374 5465 7374 7328 5465 7374  EffectTests(Test
-0001a9b0: 4361 7365 293a 0a20 2020 2064 6566 2073  Case):.    def s
-0001a9c0: 6964 655f 6566 6665 6374 2873 656c 6629  ide_effect(self)
-0001a9d0: 3a0a 2020 2020 2020 2020 7465 7374 5f63  :.        test_c
-0001a9e0: 6173 6520 3d20 7365 6c66 0a20 2020 2020  ase = self.     
-0001a9f0: 2020 2074 6573 745f 6361 7365 2e73 6964     test_case.sid
-0001aa00: 655f 6566 6665 6374 5f63 616c 6c65 6420  e_effect_called 
-0001aa10: 3d20 4661 6c73 650a 0a20 2020 2020 2020  = False..       
-0001aa20: 2064 6566 205f 5f73 6964 655f 6566 6665   def __side_effe
-0001aa30: 6374 2866 696c 655f 6f62 6a65 6374 293a  ct(file_object):
-0001aa40: 0a20 2020 2020 2020 2020 2020 2074 6573  .            tes
-0001aa50: 745f 6361 7365 2e73 6964 655f 6566 6665  t_case.side_effe
-0001aa60: 6374 5f63 616c 6c65 6420 3d20 5472 7565  ct_called = True
-0001aa70: 0a20 2020 2020 2020 2020 2020 2074 6573  .            tes
-0001aa80: 745f 6361 7365 2e73 6964 655f 6566 6665  t_case.side_effe
-0001aa90: 6374 5f66 696c 655f 6f62 6a65 6374 5f63  ct_file_object_c
-0001aaa0: 6f6e 7465 6e74 203d 2066 696c 655f 6f62  ontent = file_ob
-0001aab0: 6a65 6374 2e63 6f6e 7465 6e74 730a 0a20  ject.contents.. 
-0001aac0: 2020 2020 2020 2072 6574 7572 6e20 5f5f         return __
-0001aad0: 7369 6465 5f65 6666 6563 740a 0a20 2020  side_effect..   
-0001aae0: 2064 6566 2073 6574 5570 2873 656c 6629   def setUp(self)
-0001aaf0: 3a0a 2020 2020 2020 2020 2320 7573 6520  :.        # use 
-0001ab00: 7468 6520 7265 616c 2070 6174 6820 7365  the real path se
-0001ab10: 7061 7261 746f 7220 746f 2077 6f72 6b20  parator to work 
-0001ab20: 7769 7468 2074 6865 2072 6561 6c20 6669  with the real fi
-0001ab30: 6c65 2073 7973 7465 6d0a 2020 2020 2020  le system.      
-0001ab40: 2020 7365 6c66 2e66 696c 6573 7973 7465    self.filesyste
-0001ab50: 6d20 3d20 6661 6b65 5f66 696c 6573 7973  m = fake_filesys
-0001ab60: 7465 6d2e 4661 6b65 4669 6c65 7379 7374  tem.FakeFilesyst
-0001ab70: 656d 2829 0a20 2020 2020 2020 2073 656c  em().        sel
-0001ab80: 662e 6669 6c65 7379 7374 656d 2e63 7265  f.filesystem.cre
-0001ab90: 6174 655f 6669 6c65 2822 2f61 2f62 2f66  ate_file("/a/b/f
-0001aba0: 696c 655f 6f6e 6522 2c20 7369 6465 5f65  ile_one", side_e
-0001abb0: 6666 6563 743d 7365 6c66 2e73 6964 655f  ffect=self.side_
-0001abc0: 6566 6665 6374 2829 290a 0a20 2020 2064  effect())..    d
-0001abd0: 6566 2074 6573 745f 7369 6465 5f65 6666  ef test_side_eff
-0001abe0: 6563 745f 6361 6c6c 6564 2873 656c 6629  ect_called(self)
-0001abf0: 3a0a 2020 2020 2020 2020 6661 6b65 5f6f  :.        fake_o
-0001ac00: 7065 6e20 3d20 6661 6b65 5f66 696c 6573  pen = fake_files
-0001ac10: 7973 7465 6d2e 4661 6b65 4669 6c65 4f70  ystem.FakeFileOp
-0001ac20: 656e 2873 656c 662e 6669 6c65 7379 7374  en(self.filesyst
-0001ac30: 656d 290a 2020 2020 2020 2020 7365 6c66  em).        self
-0001ac40: 2e73 6964 655f 6566 6665 6374 5f63 616c  .side_effect_cal
-0001ac50: 6c65 6420 3d20 4661 6c73 650a 2020 2020  led = False.    
-0001ac60: 2020 2020 7769 7468 2066 616b 655f 6f70      with fake_op
-0001ac70: 656e 2822 2f61 2f62 2f66 696c 655f 6f6e  en("/a/b/file_on
-0001ac80: 6522 2c20 2277 222c 2065 6e63 6f64 696e  e", "w", encodin
-0001ac90: 673d 2275 7466 3822 2920 6173 2068 616e  g="utf8") as han
-0001aca0: 646c 653a 0a20 2020 2020 2020 2020 2020  dle:.           
-0001acb0: 2068 616e 646c 652e 7772 6974 6528 2266   handle.write("f
-0001acc0: 6f6f 2229 0a20 2020 2020 2020 2073 656c  oo").        sel
-0001acd0: 662e 6173 7365 7274 5472 7565 2873 656c  f.assertTrue(sel
-0001ace0: 662e 7369 6465 5f65 6666 6563 745f 6361  f.side_effect_ca
-0001acf0: 6c6c 6564 290a 0a20 2020 2064 6566 2074  lled)..    def t
-0001ad00: 6573 745f 7369 6465 5f65 6666 6563 745f  est_side_effect_
-0001ad10: 6669 6c65 5f6f 626a 6563 7428 7365 6c66  file_object(self
-0001ad20: 293a 0a20 2020 2020 2020 2066 616b 655f  ):.        fake_
-0001ad30: 6f70 656e 203d 2066 616b 655f 6669 6c65  open = fake_file
-0001ad40: 7379 7374 656d 2e46 616b 6546 696c 654f  system.FakeFileO
-0001ad50: 7065 6e28 7365 6c66 2e66 696c 6573 7973  pen(self.filesys
-0001ad60: 7465 6d29 0a20 2020 2020 2020 2073 656c  tem).        sel
-0001ad70: 662e 7369 6465 5f65 6666 6563 745f 6361  f.side_effect_ca
-0001ad80: 6c6c 6564 203d 2046 616c 7365 0a20 2020  lled = False.   
-0001ad90: 2020 2020 2077 6974 6820 6661 6b65 5f6f       with fake_o
-0001ada0: 7065 6e28 222f 612f 622f 6669 6c65 5f6f  pen("/a/b/file_o
-0001adb0: 6e65 222c 2022 7722 2c20 656e 636f 6469  ne", "w", encodi
-0001adc0: 6e67 3d22 7574 6638 2229 2061 7320 6861  ng="utf8") as ha
-0001add0: 6e64 6c65 3a0a 2020 2020 2020 2020 2020  ndle:.          
-0001ade0: 2020 6861 6e64 6c65 2e77 7269 7465 2822    handle.write("
-0001adf0: 666f 6f22 290a 2020 2020 2020 2020 7365  foo").        se
-0001ae00: 6c66 2e61 7373 6572 7445 7175 616c 2873  lf.assertEqual(s
-0001ae10: 656c 662e 7369 6465 5f65 6666 6563 745f  elf.side_effect_
-0001ae20: 6669 6c65 5f6f 626a 6563 745f 636f 6e74  file_object_cont
-0001ae30: 656e 742c 2022 666f 6f22 290a 0a0a 6966  ent, "foo")...if
-0001ae40: 205f 5f6e 616d 655f 5f20 3d3d 2022 5f5f   __name__ == "__
-0001ae50: 6d61 696e 5f5f 223a 0a20 2020 2075 6e69  main__":.    uni
-0001ae60: 7474 6573 742e 6d61 696e 2829 0a         ttest.main().
+00018c10: 2022 6669 7874 7572 6573 2f73 796d 6c69   "fixtures/symli
+00018c20: 6e6b 5f66 696c 655f 6162 736f 6c75 7465  nk_file_absolute
+00018c30: 5f6f 7574 7369 6465 222c 0a20 2020 2020  _outside",.     
+00018c40: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+00018c50: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+00018c60: 2020 2029 0a20 2020 2020 2020 2073 656c     ).        sel
+00018c70: 662e 6173 7365 7274 4571 7561 6c28 0a20  f.assertEqual(. 
+00018c80: 2020 2020 2020 2020 2020 2066 616b 655f             fake_
+00018c90: 6f70 656e 280a 2020 2020 2020 2020 2020  open(.          
+00018ca0: 2020 2020 2020 6f73 2e70 6174 682e 6a6f        os.path.jo
+00018cb0: 696e 280a 2020 2020 2020 2020 2020 2020  in(.            
+00018cc0: 2020 2020 2020 2020 7265 616c 5f64 6972          real_dir
+00018cd0: 6563 746f 7279 2c0a 2020 2020 2020 2020  ectory,.        
+00018ce0: 2020 2020 2020 2020 2020 2020 2266 6978              "fix
+00018cf0: 7475 7265 732f 7379 6d6c 696e 6b5f 6669  tures/symlink_fi
+00018d00: 6c65 5f61 6273 6f6c 7574 655f 6f75 7473  le_absolute_outs
+00018d10: 6964 6522 2c0a 2020 2020 2020 2020 2020  ide",.          
+00018d20: 2020 2020 2020 292c 0a20 2020 2020 2020        ),.       
+00018d30: 2020 2020 2020 2020 2065 6e63 6f64 696e           encodin
+00018d40: 673d 2275 7466 3822 2c0a 2020 2020 2020  g="utf8",.      
+00018d50: 2020 2020 2020 292e 7265 6164 2829 2c0a        ).read(),.
+00018d60: 2020 2020 2020 2020 2020 2020 2267 6f6f              "goo
+00018d70: 6420 6d6f 726e 696e 6722 2c0a 2020 2020  d morning",.    
+00018d80: 2020 2020 290a 0a20 2020 2064 6566 2074      )..    def t
+00018d90: 6573 745f 6164 645f 6578 6973 7469 6e67  est_add_existing
+00018da0: 5f72 6561 6c5f 6469 7265 6374 6f72 795f  _real_directory_
+00018db0: 7379 6d6c 696e 6b5f 7461 7267 6574 5f70  symlink_target_p
+00018dc0: 6174 6828 7365 6c66 293a 0a20 2020 2020  ath(self):.     
+00018dd0: 2020 2073 656c 662e 736b 6970 5f69 665f     self.skip_if_
+00018de0: 7379 6d6c 696e 6b5f 6e6f 745f 7375 7070  symlink_not_supp
+00018df0: 6f72 7465 6428 666f 7263 655f 7265 616c  orted(force_real
+00018e00: 5f66 733d 5472 7565 290a 2020 2020 2020  _fs=True).      
+00018e10: 2020 7265 616c 5f64 6972 6563 746f 7279    real_directory
+00018e20: 203d 2073 656c 662e 5f73 6574 7570 5f74   = self._setup_t
+00018e30: 656d 705f 6469 7265 6374 6f72 7928 290a  emp_directory().
+00018e40: 2020 2020 2020 2020 7379 6d6c 696e 6b73          symlinks
+00018e50: 203d 205b 0a20 2020 2020 2020 2020 2020   = [.           
+00018e60: 2028 0a20 2020 2020 2020 2020 2020 2020   (.             
+00018e70: 2020 2022 2e2e 222c 0a20 2020 2020 2020     "..",.       
+00018e80: 2020 2020 2020 2020 206f 732e 7061 7468           os.path
+00018e90: 2e6a 6f69 6e28 7265 616c 5f64 6972 6563  .join(real_direc
+00018ea0: 746f 7279 2c20 2266 6978 7475 7265 7322  tory, "fixtures"
+00018eb0: 2c20 2273 796d 6c69 6e6b 5f64 6972 5f72  , "symlink_dir_r
+00018ec0: 656c 6174 6976 6522 292c 0a20 2020 2020  elative"),.     
+00018ed0: 2020 2020 2020 2029 2c0a 2020 2020 2020         ),.      
+00018ee0: 2020 2020 2020 280a 2020 2020 2020 2020        (.        
+00018ef0: 2020 2020 2020 2020 222e 2e2f 616c 6c5f          "../all_
+00018f00: 7465 7374 732e 7079 222c 0a20 2020 2020  tests.py",.     
+00018f10: 2020 2020 2020 2020 2020 206f 732e 7061             os.pa
+00018f20: 7468 2e6a 6f69 6e28 7265 616c 5f64 6972  th.join(real_dir
+00018f30: 6563 746f 7279 2c20 2266 6978 7475 7265  ectory, "fixture
+00018f40: 7322 2c20 2273 796d 6c69 6e6b 5f66 696c  s", "symlink_fil
+00018f50: 655f 7265 6c61 7469 7665 2229 2c0a 2020  e_relative"),.  
+00018f60: 2020 2020 2020 2020 2020 292c 0a20 2020            ),.   
+00018f70: 2020 2020 205d 0a0a 2020 2020 2020 2020       ]..        
+00018f80: 7769 7468 2073 656c 662e 6372 6561 7465  with self.create
+00018f90: 5f73 796d 6c69 6e6b 7328 7379 6d6c 696e  _symlinks(symlin
+00018fa0: 6b73 293a 0a20 2020 2020 2020 2020 2020  ks):.           
+00018fb0: 2073 656c 662e 6669 6c65 7379 7374 656d   self.filesystem
+00018fc0: 2e61 6464 5f72 6561 6c5f 6469 7265 6374  .add_real_direct
+00018fd0: 6f72 7928 0a20 2020 2020 2020 2020 2020  ory(.           
+00018fe0: 2020 2020 2072 6561 6c5f 6469 7265 6374       real_direct
+00018ff0: 6f72 792c 2074 6172 6765 745f 7061 7468  ory, target_path
+00019000: 3d22 2f70 6174 6822 2c20 6c61 7a79 5f72  ="/path", lazy_r
+00019010: 6561 643d 4661 6c73 650a 2020 2020 2020  ead=False.      
+00019020: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
+00019030: 2073 656c 662e 6173 7365 7274 5472 7565   self.assertTrue
+00019040: 2873 656c 662e 6669 6c65 7379 7374 656d  (self.filesystem
+00019050: 2e65 7869 7374 7328 222f 7061 7468 2f66  .exists("/path/f
+00019060: 6978 7475 7265 732f 7379 6d6c 696e 6b5f  ixtures/symlink_
+00019070: 6469 725f 7265 6c61 7469 7665 2229 290a  dir_relative")).
+00019080: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+00019090: 6572 7454 7275 6528 0a20 2020 2020 2020  ertTrue(.       
+000190a0: 2020 2020 2073 656c 662e 6669 6c65 7379       self.filesy
+000190b0: 7374 656d 2e65 7869 7374 7328 222f 7061  stem.exists("/pa
+000190c0: 7468 2f66 6978 7475 7265 732f 7379 6d6c  th/fixtures/syml
+000190d0: 696e 6b5f 6469 725f 7265 6c61 7469 7665  ink_dir_relative
+000190e0: 2f61 6c6c 5f74 6573 7473 2e70 7922 290a  /all_tests.py").
+000190f0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+00019100: 2020 7365 6c66 2e61 7373 6572 7454 7275    self.assertTru
+00019110: 6528 7365 6c66 2e66 696c 6573 7973 7465  e(self.filesyste
+00019120: 6d2e 6578 6973 7473 2822 2f70 6174 682f  m.exists("/path/
+00019130: 6669 7874 7572 6573 2f73 796d 6c69 6e6b  fixtures/symlink
+00019140: 5f66 696c 655f 7265 6c61 7469 7665 2229  _file_relative")
+00019150: 290a 0a20 2020 2064 6566 2074 6573 745f  )..    def test_
+00019160: 6164 645f 6578 6973 7469 6e67 5f72 6561  add_existing_rea
+00019170: 6c5f 6469 7265 6374 6f72 795f 7379 6d6c  l_directory_syml
+00019180: 696e 6b5f 6c61 7a79 5f72 6561 6428 7365  ink_lazy_read(se
+00019190: 6c66 293a 0a20 2020 2020 2020 2073 656c  lf):.        sel
+000191a0: 662e 736b 6970 5f69 665f 7379 6d6c 696e  f.skip_if_symlin
+000191b0: 6b5f 6e6f 745f 7375 7070 6f72 7465 6428  k_not_supported(
+000191c0: 666f 7263 655f 7265 616c 5f66 733d 5472  force_real_fs=Tr
+000191d0: 7565 290a 2020 2020 2020 2020 7265 616c  ue).        real
+000191e0: 5f64 6972 6563 746f 7279 203d 2073 656c  _directory = sel
+000191f0: 662e 5f73 6574 7570 5f74 656d 705f 6469  f._setup_temp_di
+00019200: 7265 6374 6f72 7928 290a 2020 2020 2020  rectory().      
+00019210: 2020 7379 6d6c 696e 6b73 203d 205b 0a20    symlinks = [. 
+00019220: 2020 2020 2020 2020 2020 2028 0a20 2020             (.   
+00019230: 2020 2020 2020 2020 2020 2020 2022 2e2e               "..
+00019240: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00019250: 2020 206f 732e 7061 7468 2e6a 6f69 6e28     os.path.join(
+00019260: 7265 616c 5f64 6972 6563 746f 7279 2c20  real_directory, 
+00019270: 2266 6978 7475 7265 7322 2c20 2273 796d  "fixtures", "sym
+00019280: 6c69 6e6b 5f64 6972 5f72 656c 6174 6976  link_dir_relativ
+00019290: 6522 292c 0a20 2020 2020 2020 2020 2020  e"),.           
+000192a0: 2029 2c0a 2020 2020 2020 2020 2020 2020   ),.            
+000192b0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+000192c0: 2020 222e 2e2f 616c 6c5f 7465 7374 732e    "../all_tests.
+000192d0: 7079 222c 0a20 2020 2020 2020 2020 2020  py",.           
+000192e0: 2020 2020 206f 732e 7061 7468 2e6a 6f69       os.path.joi
+000192f0: 6e28 7265 616c 5f64 6972 6563 746f 7279  n(real_directory
+00019300: 2c20 2266 6978 7475 7265 7322 2c20 2273  , "fixtures", "s
+00019310: 796d 6c69 6e6b 5f66 696c 655f 7265 6c61  ymlink_file_rela
+00019320: 7469 7665 2229 2c0a 2020 2020 2020 2020  tive"),.        
+00019330: 2020 2020 292c 0a20 2020 2020 2020 205d      ),.        ]
+00019340: 0a0a 2020 2020 2020 2020 7769 7468 2073  ..        with s
+00019350: 656c 662e 6372 6561 7465 5f73 796d 6c69  elf.create_symli
+00019360: 6e6b 7328 7379 6d6c 696e 6b73 293a 0a20  nks(symlinks):. 
+00019370: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00019380: 6669 6c65 7379 7374 656d 2e61 6464 5f72  filesystem.add_r
+00019390: 6561 6c5f 6469 7265 6374 6f72 7928 0a20  eal_directory(. 
+000193a0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+000193b0: 6561 6c5f 6469 7265 6374 6f72 792c 2074  eal_directory, t
+000193c0: 6172 6765 745f 7061 7468 3d22 2f70 6174  arget_path="/pat
+000193d0: 6822 2c20 6c61 7a79 5f72 6561 643d 5472  h", lazy_read=Tr
+000193e0: 7565 0a20 2020 2020 2020 2020 2020 2029  ue.            )
+000193f0: 0a0a 2020 2020 2020 2020 2020 2020 7365  ..            se
+00019400: 6c66 2e61 7373 6572 7454 7275 6528 0a20  lf.assertTrue(. 
+00019410: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00019420: 656c 662e 6669 6c65 7379 7374 656d 2e65  elf.filesystem.e
+00019430: 7869 7374 7328 222f 7061 7468 2f66 6978  xists("/path/fix
+00019440: 7475 7265 732f 7379 6d6c 696e 6b5f 6469  tures/symlink_di
+00019450: 725f 7265 6c61 7469 7665 2229 0a20 2020  r_relative").   
+00019460: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+00019470: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+00019480: 7274 5472 7565 280a 2020 2020 2020 2020  rtTrue(.        
+00019490: 2020 2020 2020 2020 7365 6c66 2e66 696c          self.fil
+000194a0: 6573 7973 7465 6d2e 6578 6973 7473 280a  esystem.exists(.
+000194b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000194c0: 2020 2020 222f 7061 7468 2f66 6978 7475      "/path/fixtu
+000194d0: 7265 732f 7379 6d6c 696e 6b5f 6469 725f  res/symlink_dir_
+000194e0: 7265 6c61 7469 7665 2f61 6c6c 5f74 6573  relative/all_tes
+000194f0: 7473 2e70 7922 0a20 2020 2020 2020 2020  ts.py".         
+00019500: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00019510: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
+00019520: 2020 2073 656c 662e 6173 7365 7274 5472     self.assertTr
+00019530: 7565 280a 2020 2020 2020 2020 2020 2020  ue(.            
+00019540: 2020 2020 7365 6c66 2e66 696c 6573 7973      self.filesys
+00019550: 7465 6d2e 6578 6973 7473 2822 2f70 6174  tem.exists("/pat
+00019560: 682f 6669 7874 7572 6573 2f73 796d 6c69  h/fixtures/symli
+00019570: 6e6b 5f66 696c 655f 7265 6c61 7469 7665  nk_file_relative
+00019580: 2229 0a20 2020 2020 2020 2020 2020 2029  ").            )
+00019590: 0a0a 2020 2020 6465 6620 7465 7374 5f61  ..    def test_a
+000195a0: 6464 5f65 7869 7374 696e 675f 7265 616c  dd_existing_real
+000195b0: 5f64 6972 6563 746f 7279 5f74 7265 655f  _directory_tree_
+000195c0: 746f 5f6f 7468 6572 5f70 6174 6828 7365  to_other_path(se
+000195d0: 6c66 293a 0a20 2020 2020 2020 2073 656c  lf):.        sel
+000195e0: 662e 6669 6c65 7379 7374 656d 2e61 6464  f.filesystem.add
+000195f0: 5f72 6561 6c5f 6469 7265 6374 6f72 7928  _real_directory(
+00019600: 7365 6c66 2e72 6f6f 745f 7061 7468 2c20  self.root_path, 
+00019610: 7461 7267 6574 5f70 6174 683d 222f 666f  target_path="/fo
+00019620: 6f2f 6261 7222 290a 2020 2020 2020 2020  o/bar").        
+00019630: 7365 6c66 2e61 7373 6572 7446 616c 7365  self.assertFalse
+00019640: 280a 2020 2020 2020 2020 2020 2020 7365  (.            se
+00019650: 6c66 2e66 696c 6573 7973 7465 6d2e 6578  lf.filesystem.ex
+00019660: 6973 7473 280a 2020 2020 2020 2020 2020  ists(.          
+00019670: 2020 2020 2020 6f73 2e70 6174 682e 6a6f        os.path.jo
+00019680: 696e 2873 656c 662e 7079 6661 6b65 6673  in(self.pyfakefs
+00019690: 5f70 6174 682c 2022 7465 7374 7322 2c20  _path, "tests", 
+000196a0: 2266 616b 655f 6669 6c65 7379 7374 656d  "fake_filesystem
+000196b0: 5f74 6573 742e 7079 2229 0a20 2020 2020  _test.py").     
+000196c0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+000196d0: 2029 0a20 2020 2020 2020 2073 656c 662e   ).        self.
+000196e0: 6173 7365 7274 5472 7565 280a 2020 2020  assertTrue(.    
+000196f0: 2020 2020 2020 2020 7365 6c66 2e66 696c          self.fil
+00019700: 6573 7973 7465 6d2e 6578 6973 7473 280a  esystem.exists(.
+00019710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019720: 6f73 2e70 6174 682e 6a6f 696e 280a 2020  os.path.join(.  
+00019730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019740: 2020 2266 6f6f 222c 0a20 2020 2020 2020    "foo",.       
+00019750: 2020 2020 2020 2020 2020 2020 2022 6261               "ba
+00019760: 7222 2c0a 2020 2020 2020 2020 2020 2020  r",.            
+00019770: 2020 2020 2020 2020 2270 7966 616b 6566          "pyfakef
+00019780: 7322 2c0a 2020 2020 2020 2020 2020 2020  s",.            
+00019790: 2020 2020 2020 2020 2274 6573 7473 222c          "tests",
+000197a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000197b0: 2020 2020 2022 6661 6b65 5f66 696c 6573       "fake_files
+000197c0: 7973 7465 6d5f 7465 7374 2e70 7922 2c0a  ystem_test.py",.
+000197d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000197e0: 290a 2020 2020 2020 2020 2020 2020 290a  ).            ).
+000197f0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+00019800: 2020 7365 6c66 2e61 7373 6572 7446 616c    self.assertFal
+00019810: 7365 280a 2020 2020 2020 2020 2020 2020  se(.            
+00019820: 7365 6c66 2e66 696c 6573 7973 7465 6d2e  self.filesystem.
+00019830: 6578 6973 7473 280a 2020 2020 2020 2020  exists(.        
+00019840: 2020 2020 2020 2020 6f73 2e70 6174 682e          os.path.
+00019850: 6a6f 696e 2873 656c 662e 726f 6f74 5f70  join(self.root_p
+00019860: 6174 682c 2022 7079 6661 6b65 6673 222c  ath, "pyfakefs",
+00019870: 2022 6661 6b65 5f66 696c 6573 7973 7465   "fake_filesyste
+00019880: 6d2e 7079 2229 0a20 2020 2020 2020 2020  m.py").         
+00019890: 2020 2029 0a20 2020 2020 2020 2029 0a20     ).        ). 
+000198a0: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+000198b0: 7274 5472 7565 280a 2020 2020 2020 2020  rtTrue(.        
+000198c0: 2020 2020 7365 6c66 2e66 696c 6573 7973      self.filesys
+000198d0: 7465 6d2e 6578 6973 7473 280a 2020 2020  tem.exists(.    
+000198e0: 2020 2020 2020 2020 2020 2020 6f73 2e70              os.p
+000198f0: 6174 682e 6a6f 696e 2822 666f 6f22 2c20  ath.join("foo", 
+00019900: 2262 6172 222c 2022 7079 6661 6b65 6673  "bar", "pyfakefs
+00019910: 222c 2022 5f5f 696e 6974 5f5f 2e70 7922  ", "__init__.py"
+00019920: 290a 2020 2020 2020 2020 2020 2020 290a  ).            ).
+00019930: 2020 2020 2020 2020 290a 0a20 2020 2064          )..    d
+00019940: 6566 2074 6573 745f 6765 745f 6f62 6a65  ef test_get_obje
+00019950: 6374 5f66 726f 6d5f 6c61 7a69 6c79 5f61  ct_from_lazily_a
+00019960: 6464 6564 5f72 6561 6c5f 6469 7265 6374  dded_real_direct
+00019970: 6f72 7928 7365 6c66 293a 0a20 2020 2020  ory(self):.     
+00019980: 2020 2073 656c 662e 6669 6c65 7379 7374     self.filesyst
+00019990: 656d 2e69 735f 6361 7365 5f73 656e 7369  em.is_case_sensi
+000199a0: 7469 7665 203d 2054 7275 650a 2020 2020  tive = True.    
+000199b0: 2020 2020 7365 6c66 2e66 696c 6573 7973      self.filesys
+000199c0: 7465 6d2e 6164 645f 7265 616c 5f64 6972  tem.add_real_dir
+000199d0: 6563 746f 7279 2873 656c 662e 726f 6f74  ectory(self.root
+000199e0: 5f70 6174 6829 0a20 2020 2020 2020 2073  _path).        s
+000199f0: 656c 662e 6173 7365 7274 5472 7565 280a  elf.assertTrue(.
+00019a00: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00019a10: 2e66 696c 6573 7973 7465 6d2e 6765 745f  .filesystem.get_
+00019a20: 6f62 6a65 6374 280a 2020 2020 2020 2020  object(.        
+00019a30: 2020 2020 2020 2020 6f73 2e70 6174 682e          os.path.
+00019a40: 6a6f 696e 2873 656c 662e 726f 6f74 5f70  join(self.root_p
+00019a50: 6174 682c 2022 7079 6661 6b65 6673 222c  ath, "pyfakefs",
+00019a60: 2022 6661 6b65 5f66 696c 6573 7973 7465   "fake_filesyste
+00019a70: 6d2e 7079 2229 0a20 2020 2020 2020 2020  m.py").         
+00019a80: 2020 2029 0a20 2020 2020 2020 2029 0a20     ).        ). 
+00019a90: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+00019aa0: 7274 5472 7565 280a 2020 2020 2020 2020  rtTrue(.        
+00019ab0: 2020 2020 7365 6c66 2e66 696c 6573 7973      self.filesys
+00019ac0: 7465 6d2e 6765 745f 6f62 6a65 6374 280a  tem.get_object(.
+00019ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019ae0: 6f73 2e70 6174 682e 6a6f 696e 2873 656c  os.path.join(sel
+00019af0: 662e 726f 6f74 5f70 6174 682c 2022 7079  f.root_path, "py
+00019b00: 6661 6b65 6673 222c 2022 5f5f 696e 6974  fakefs", "__init
+00019b10: 5f5f 2e70 7922 290a 2020 2020 2020 2020  __.py").        
+00019b20: 2020 2020 290a 2020 2020 2020 2020 290a      ).        ).
+00019b30: 0a20 2020 2064 6566 2074 6573 745f 6164  .    def test_ad
+00019b40: 645f 6578 6973 7469 6e67 5f72 6561 6c5f  d_existing_real_
+00019b50: 6469 7265 6374 6f72 795f 6c61 7a69 6c79  directory_lazily
+00019b60: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00019b70: 6469 736b 5f73 697a 6520 3d20 3130 3234  disk_size = 1024
+00019b80: 202a 2031 3032 3420 2a20 3130 3234 0a20   * 1024 * 1024. 
+00019b90: 2020 2020 2020 2072 6561 6c5f 6469 725f         real_dir_
+00019ba0: 7061 7468 203d 206f 732e 7061 7468 2e6a  path = os.path.j
+00019bb0: 6f69 6e28 7365 6c66 2e72 6f6f 745f 7061  oin(self.root_pa
+00019bc0: 7468 2c20 2270 7966 616b 6566 7322 290a  th, "pyfakefs").
+00019bd0: 2020 2020 2020 2020 7365 6c66 2e66 696c          self.fil
+00019be0: 6573 7973 7465 6d2e 7365 745f 6469 736b  esystem.set_disk
+00019bf0: 5f75 7361 6765 2864 6973 6b5f 7369 7a65  _usage(disk_size
+00019c00: 2c20 7265 616c 5f64 6972 5f70 6174 6829  , real_dir_path)
+00019c10: 0a20 2020 2020 2020 2073 656c 662e 6669  .        self.fi
+00019c20: 6c65 7379 7374 656d 2e61 6464 5f72 6561  lesystem.add_rea
+00019c30: 6c5f 6469 7265 6374 6f72 7928 7265 616c  l_directory(real
+00019c40: 5f64 6972 5f70 6174 6829 0a0a 2020 2020  _dir_path)..    
+00019c50: 2020 2020 2320 7468 6520 6469 7265 6374      # the direct
+00019c60: 6f72 7920 636f 6e74 656e 7473 2068 6176  ory contents hav
+00019c70: 6520 6e6f 7420 6265 656e 2072 6561 642c  e not been read,
+00019c80: 2074 6865 2064 6973 6b20 7573 6167 650a   the disk usage.
+00019c90: 2020 2020 2020 2020 2320 6861 7320 6e6f          # has no
+00019ca0: 7420 6368 616e 6765 640a 2020 2020 2020  t changed.      
+00019cb0: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
+00019cc0: 616c 2864 6973 6b5f 7369 7a65 2c20 7365  al(disk_size, se
+00019cd0: 6c66 2e66 696c 6573 7973 7465 6d2e 6765  lf.filesystem.ge
+00019ce0: 745f 6469 736b 5f75 7361 6765 2872 6561  t_disk_usage(rea
+00019cf0: 6c5f 6469 725f 7061 7468 292e 6672 6565  l_dir_path).free
+00019d00: 290a 2020 2020 2020 2020 2320 6368 6563  ).        # chec
+00019d10: 6b69 6e67 2066 6f72 2065 7869 7374 656e  king for existen
+00019d20: 6365 2073 6861 6c6c 2072 6561 6420 7468  ce shall read th
+00019d30: 6520 6469 7265 6374 6f72 7920 636f 6e74  e directory cont
+00019d40: 656e 7473 0a20 2020 2020 2020 2073 656c  ents.        sel
+00019d50: 662e 6173 7365 7274 5472 7565 280a 2020  f.assertTrue(.  
+00019d60: 2020 2020 2020 2020 2020 7365 6c66 2e66            self.f
+00019d70: 696c 6573 7973 7465 6d2e 6765 745f 6f62  ilesystem.get_ob
+00019d80: 6a65 6374 280a 2020 2020 2020 2020 2020  ject(.          
+00019d90: 2020 2020 2020 6f73 2e70 6174 682e 6a6f        os.path.jo
+00019da0: 696e 2872 6561 6c5f 6469 725f 7061 7468  in(real_dir_path
+00019db0: 2c20 2266 616b 655f 6669 6c65 7379 7374  , "fake_filesyst
+00019dc0: 656d 2e70 7922 290a 2020 2020 2020 2020  em.py").        
+00019dd0: 2020 2020 290a 2020 2020 2020 2020 290a      ).        ).
+00019de0: 2020 2020 2020 2020 2320 736f 206e 6f77          # so now
+00019df0: 2074 6865 2066 7265 6520 6469 736b 2073   the free disk s
+00019e00: 7061 6365 2073 6861 6c6c 2068 6176 6520  pace shall have 
+00019e10: 6465 6372 6561 7365 640a 2020 2020 2020  decreased.      
+00019e20: 2020 7365 6c66 2e61 7373 6572 7447 7265    self.assertGre
+00019e30: 6174 6572 280a 2020 2020 2020 2020 2020  ater(.          
+00019e40: 2020 6469 736b 5f73 697a 652c 2073 656c    disk_size, sel
+00019e50: 662e 6669 6c65 7379 7374 656d 2e67 6574  f.filesystem.get
+00019e60: 5f64 6973 6b5f 7573 6167 6528 7265 616c  _disk_usage(real
+00019e70: 5f64 6972 5f70 6174 6829 2e66 7265 650a  _dir_path).free.
+00019e80: 2020 2020 2020 2020 290a 0a20 2020 2064          )..    d
+00019e90: 6566 2074 6573 745f 6164 645f 6578 6973  ef test_add_exis
+00019ea0: 7469 6e67 5f72 6561 6c5f 6469 7265 6374  ting_real_direct
+00019eb0: 6f72 795f 6e6f 745f 6c61 7a69 6c79 2873  ory_not_lazily(s
+00019ec0: 656c 6629 3a0a 2020 2020 2020 2020 6469  elf):.        di
+00019ed0: 736b 5f73 697a 6520 3d20 3130 3234 202a  sk_size = 1024 *
+00019ee0: 2031 3032 3420 2a20 3130 3234 0a20 2020   1024 * 1024.   
+00019ef0: 2020 2020 2073 656c 662e 6669 6c65 7379       self.filesy
+00019f00: 7374 656d 2e73 6574 5f64 6973 6b5f 7573  stem.set_disk_us
+00019f10: 6167 6528 6469 736b 5f73 697a 652c 2073  age(disk_size, s
+00019f20: 656c 662e 7079 6661 6b65 6673 5f70 6174  elf.pyfakefs_pat
+00019f30: 6829 0a20 2020 2020 2020 2073 656c 662e  h).        self.
+00019f40: 6669 6c65 7379 7374 656d 2e61 6464 5f72  filesystem.add_r
+00019f50: 6561 6c5f 6469 7265 6374 6f72 7928 7365  eal_directory(se
+00019f60: 6c66 2e70 7966 616b 6566 735f 7061 7468  lf.pyfakefs_path
+00019f70: 2c20 6c61 7a79 5f72 6561 643d 4661 6c73  , lazy_read=Fals
+00019f80: 6529 0a0a 2020 2020 2020 2020 2320 7468  e)..        # th
+00019f90: 6520 6469 7265 6374 6f72 7920 6861 7320  e directory has 
+00019fa0: 6265 656e 2072 6561 642c 2073 6f20 7468  been read, so th
+00019fb0: 6520 6669 6c65 2073 697a 6573 2068 6176  e file sizes hav
+00019fc0: 650a 2020 2020 2020 2020 2320 6265 656e  e.        # been
+00019fd0: 2073 7562 7472 6163 7465 6420 6672 6f6d   subtracted from
+00019fe0: 2074 6865 2066 7265 6520 7370 6163 650a   the free space.
+00019ff0: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+0001a000: 6572 7447 7265 6174 6572 280a 2020 2020  ertGreater(.    
+0001a010: 2020 2020 2020 2020 6469 736b 5f73 697a          disk_siz
+0001a020: 652c 2073 656c 662e 6669 6c65 7379 7374  e, self.filesyst
+0001a030: 656d 2e67 6574 5f64 6973 6b5f 7573 6167  em.get_disk_usag
+0001a040: 6528 7365 6c66 2e70 7966 616b 6566 735f  e(self.pyfakefs_
+0001a050: 7061 7468 292e 6672 6565 0a20 2020 2020  path).free.     
+0001a060: 2020 2029 0a0a 2020 2020 6465 6620 7465     )..    def te
+0001a070: 7374 5f61 6464 5f65 7869 7374 696e 675f  st_add_existing_
+0001a080: 7265 616c 5f64 6972 6563 746f 7279 5f72  real_directory_r
+0001a090: 6561 645f 7772 6974 6528 7365 6c66 293a  ead_write(self):
+0001a0a0: 0a20 2020 2020 2020 2073 656c 662e 6669  .        self.fi
+0001a0b0: 6c65 7379 7374 656d 2e61 6464 5f72 6561  lesystem.add_rea
+0001a0c0: 6c5f 6469 7265 6374 6f72 7928 7365 6c66  l_directory(self
+0001a0d0: 2e70 7966 616b 6566 735f 7061 7468 2c20  .pyfakefs_path, 
+0001a0e0: 7265 6164 5f6f 6e6c 793d 4661 6c73 6529  read_only=False)
+0001a0f0: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
+0001a100: 7365 7274 5472 7565 2873 656c 662e 6669  sertTrue(self.fi
+0001a110: 6c65 7379 7374 656d 2e65 7869 7374 7328  lesystem.exists(
+0001a120: 7365 6c66 2e70 7966 616b 6566 735f 7061  self.pyfakefs_pa
+0001a130: 7468 2929 0a20 2020 2020 2020 2073 656c  th)).        sel
+0001a140: 662e 6173 7365 7274 5472 7565 280a 2020  f.assertTrue(.  
+0001a150: 2020 2020 2020 2020 2020 7365 6c66 2e66            self.f
+0001a160: 696c 6573 7973 7465 6d2e 6578 6973 7473  ilesystem.exists
+0001a170: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+0001a180: 2020 6f73 2e70 6174 682e 6a6f 696e 2873    os.path.join(s
+0001a190: 656c 662e 7079 6661 6b65 6673 5f70 6174  elf.pyfakefs_pat
+0001a1a0: 682c 2022 6661 6b65 5f66 696c 6573 7973  h, "fake_filesys
+0001a1b0: 7465 6d2e 7079 2229 0a20 2020 2020 2020  tem.py").       
+0001a1c0: 2020 2020 2029 0a20 2020 2020 2020 2029       ).        )
+0001a1d0: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
+0001a1e0: 7365 7274 5472 7565 280a 2020 2020 2020  sertTrue(.      
+0001a1f0: 2020 2020 2020 7365 6c66 2e66 696c 6573        self.files
+0001a200: 7973 7465 6d2e 6578 6973 7473 286f 732e  ystem.exists(os.
+0001a210: 7061 7468 2e6a 6f69 6e28 7365 6c66 2e70  path.join(self.p
+0001a220: 7966 616b 6566 735f 7061 7468 2c20 2266  yfakefs_path, "f
+0001a230: 616b 655f 7061 7468 6c69 622e 7079 2229  ake_pathlib.py")
+0001a240: 290a 2020 2020 2020 2020 290a 0a20 2020  ).        )..   
+0001a250: 2020 2020 2066 696c 655f 7061 7468 203d       file_path =
+0001a260: 206f 732e 7061 7468 2e6a 6f69 6e28 7365   os.path.join(se
+0001a270: 6c66 2e70 7966 616b 6566 735f 7061 7468  lf.pyfakefs_path
+0001a280: 2c20 2270 7974 6573 745f 706c 7567 696e  , "pytest_plugin
+0001a290: 2e70 7922 290a 2020 2020 2020 2020 6661  .py").        fa
+0001a2a0: 6b65 5f66 696c 6520 3d20 7365 6c66 2e66  ke_file = self.f
+0001a2b0: 696c 6573 7973 7465 6d2e 7265 736f 6c76  ilesystem.resolv
+0001a2c0: 6528 6669 6c65 5f70 6174 6829 0a20 2020  e(file_path).   
+0001a2d0: 2020 2020 2073 656c 662e 6368 6563 6b5f       self.check_
+0001a2e0: 6661 6b65 5f66 696c 655f 7374 6174 2866  fake_file_stat(f
+0001a2f0: 616b 655f 6669 6c65 2c20 6669 6c65 5f70  ake_file, file_p
+0001a300: 6174 6829 0a20 2020 2020 2020 2073 656c  ath).        sel
+0001a310: 662e 6368 6563 6b5f 7772 6974 6162 6c65  f.check_writable
+0001a320: 5f66 696c 6528 6661 6b65 5f66 696c 652c  _file(fake_file,
+0001a330: 2066 696c 655f 7061 7468 290a 0a20 2020   file_path)..   
+0001a340: 2064 6566 2074 6573 745f 6164 645f 6578   def test_add_ex
+0001a350: 6973 7469 6e67 5f72 6561 6c5f 7061 7468  isting_real_path
+0001a360: 735f 7265 6164 5f6f 6e6c 7928 7365 6c66  s_read_only(self
+0001a370: 293a 0a20 2020 2020 2020 2072 6561 6c5f  ):.        real_
+0001a380: 6669 6c65 5f70 6174 6820 3d20 6f73 2e70  file_path = os.p
+0001a390: 6174 682e 7265 616c 7061 7468 285f 5f66  ath.realpath(__f
+0001a3a0: 696c 655f 5f29 0a20 2020 2020 2020 2066  ile__).        f
+0001a3b0: 6978 7475 7265 5f70 6174 6820 3d20 6f73  ixture_path = os
+0001a3c0: 2e70 6174 682e 6a6f 696e 2873 656c 662e  .path.join(self.
+0001a3d0: 7079 6661 6b65 6673 5f70 6174 682c 2022  pyfakefs_path, "
+0001a3e0: 7465 7374 7322 2c20 2266 6978 7475 7265  tests", "fixture
+0001a3f0: 7322 290a 2020 2020 2020 2020 7365 6c66  s").        self
+0001a400: 2e66 696c 6573 7973 7465 6d2e 6164 645f  .filesystem.add_
+0001a410: 7265 616c 5f70 6174 6873 285b 7265 616c  real_paths([real
+0001a420: 5f66 696c 655f 7061 7468 2c20 6669 7874  _file_path, fixt
+0001a430: 7572 655f 7061 7468 5d29 0a0a 2020 2020  ure_path])..    
+0001a440: 2020 2020 6661 6b65 5f66 696c 6520 3d20      fake_file = 
+0001a450: 7365 6c66 2e66 696c 6573 7973 7465 6d2e  self.filesystem.
+0001a460: 7265 736f 6c76 6528 7265 616c 5f66 696c  resolve(real_fil
+0001a470: 655f 7061 7468 290a 2020 2020 2020 2020  e_path).        
+0001a480: 7365 6c66 2e63 6865 636b 5f66 616b 655f  self.check_fake_
+0001a490: 6669 6c65 5f73 7461 7428 6661 6b65 5f66  file_stat(fake_f
+0001a4a0: 696c 652c 2072 6561 6c5f 6669 6c65 5f70  ile, real_file_p
+0001a4b0: 6174 6829 0a20 2020 2020 2020 2073 656c  ath).        sel
+0001a4c0: 662e 6368 6563 6b5f 7265 6164 5f6f 6e6c  f.check_read_onl
+0001a4d0: 795f 6669 6c65 2866 616b 655f 6669 6c65  y_file(fake_file
+0001a4e0: 2c20 7265 616c 5f66 696c 655f 7061 7468  , real_file_path
+0001a4f0: 290a 0a20 2020 2020 2020 2072 6561 6c5f  )..        real_
+0001a500: 6669 6c65 5f70 6174 6820 3d20 6f73 2e70  file_path = os.p
+0001a510: 6174 682e 6a6f 696e 2866 6978 7475 7265  ath.join(fixture
+0001a520: 5f70 6174 682c 2022 6d6f 6475 6c65 5f77  _path, "module_w
+0001a530: 6974 685f 6174 7472 6962 7574 6573 2e70  ith_attributes.p
+0001a540: 7922 290a 2020 2020 2020 2020 6661 6b65  y").        fake
+0001a550: 5f66 696c 6520 3d20 7365 6c66 2e66 696c  _file = self.fil
+0001a560: 6573 7973 7465 6d2e 7265 736f 6c76 6528  esystem.resolve(
+0001a570: 7265 616c 5f66 696c 655f 7061 7468 290a  real_file_path).
+0001a580: 2020 2020 2020 2020 7365 6c66 2e63 6865          self.che
+0001a590: 636b 5f66 616b 655f 6669 6c65 5f73 7461  ck_fake_file_sta
+0001a5a0: 7428 6661 6b65 5f66 696c 652c 2072 6561  t(fake_file, rea
+0001a5b0: 6c5f 6669 6c65 5f70 6174 6829 0a20 2020  l_file_path).   
+0001a5c0: 2020 2020 2073 656c 662e 6368 6563 6b5f       self.check_
+0001a5d0: 7265 6164 5f6f 6e6c 795f 6669 6c65 2866  read_only_file(f
+0001a5e0: 616b 655f 6669 6c65 2c20 7265 616c 5f66  ake_file, real_f
+0001a5f0: 696c 655f 7061 7468 290a 0a20 2020 2064  ile_path)..    d
+0001a600: 6566 2074 6573 745f 6164 645f 6578 6973  ef test_add_exis
+0001a610: 7469 6e67 5f72 6561 6c5f 7061 7468 735f  ting_real_paths_
+0001a620: 7265 6164 5f77 7269 7465 2873 656c 6629  read_write(self)
+0001a630: 3a0a 2020 2020 2020 2020 7265 616c 5f66  :.        real_f
+0001a640: 696c 655f 7061 7468 203d 206f 732e 7061  ile_path = os.pa
+0001a650: 7468 2e72 6561 6c70 6174 6828 5f5f 6669  th.realpath(__fi
+0001a660: 6c65 5f5f 290a 2020 2020 2020 2020 6669  le__).        fi
+0001a670: 7874 7572 655f 7061 7468 203d 206f 732e  xture_path = os.
+0001a680: 7061 7468 2e6a 6f69 6e28 7365 6c66 2e70  path.join(self.p
+0001a690: 7966 616b 6566 735f 7061 7468 2c20 2274  yfakefs_path, "t
+0001a6a0: 6573 7473 222c 2022 6669 7874 7572 6573  ests", "fixtures
+0001a6b0: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
+0001a6c0: 6669 6c65 7379 7374 656d 2e61 6464 5f72  filesystem.add_r
+0001a6d0: 6561 6c5f 7061 7468 7328 5b72 6561 6c5f  eal_paths([real_
+0001a6e0: 6669 6c65 5f70 6174 682c 2066 6978 7475  file_path, fixtu
+0001a6f0: 7265 5f70 6174 685d 2c20 7265 6164 5f6f  re_path], read_o
+0001a700: 6e6c 793d 4661 6c73 6529 0a0a 2020 2020  nly=False)..    
+0001a710: 2020 2020 6661 6b65 5f66 696c 6520 3d20      fake_file = 
+0001a720: 7365 6c66 2e66 696c 6573 7973 7465 6d2e  self.filesystem.
+0001a730: 7265 736f 6c76 6528 7265 616c 5f66 696c  resolve(real_fil
+0001a740: 655f 7061 7468 290a 2020 2020 2020 2020  e_path).        
+0001a750: 7365 6c66 2e63 6865 636b 5f66 616b 655f  self.check_fake_
+0001a760: 6669 6c65 5f73 7461 7428 6661 6b65 5f66  file_stat(fake_f
+0001a770: 696c 652c 2072 6561 6c5f 6669 6c65 5f70  ile, real_file_p
+0001a780: 6174 6829 0a20 2020 2020 2020 2073 656c  ath).        sel
+0001a790: 662e 6368 6563 6b5f 7772 6974 6162 6c65  f.check_writable
+0001a7a0: 5f66 696c 6528 6661 6b65 5f66 696c 652c  _file(fake_file,
+0001a7b0: 2072 6561 6c5f 6669 6c65 5f70 6174 6829   real_file_path)
+0001a7c0: 0a0a 2020 2020 2020 2020 7265 616c 5f66  ..        real_f
+0001a7d0: 696c 655f 7061 7468 203d 206f 732e 7061  ile_path = os.pa
+0001a7e0: 7468 2e6a 6f69 6e28 6669 7874 7572 655f  th.join(fixture_
+0001a7f0: 7061 7468 2c20 226d 6f64 756c 655f 7769  path, "module_wi
+0001a800: 7468 5f61 7474 7269 6275 7465 732e 7079  th_attributes.py
+0001a810: 2229 0a20 2020 2020 2020 2066 616b 655f  ").        fake_
+0001a820: 6669 6c65 203d 2073 656c 662e 6669 6c65  file = self.file
+0001a830: 7379 7374 656d 2e72 6573 6f6c 7665 2872  system.resolve(r
+0001a840: 6561 6c5f 6669 6c65 5f70 6174 6829 0a20  eal_file_path). 
+0001a850: 2020 2020 2020 2073 656c 662e 6368 6563         self.chec
+0001a860: 6b5f 6661 6b65 5f66 696c 655f 7374 6174  k_fake_file_stat
+0001a870: 2866 616b 655f 6669 6c65 2c20 7265 616c  (fake_file, real
+0001a880: 5f66 696c 655f 7061 7468 290a 2020 2020  _file_path).    
+0001a890: 2020 2020 7365 6c66 2e63 6865 636b 5f77      self.check_w
+0001a8a0: 7269 7461 626c 655f 6669 6c65 2866 616b  ritable_file(fak
+0001a8b0: 655f 6669 6c65 2c20 7265 616c 5f66 696c  e_file, real_fil
+0001a8c0: 655f 7061 7468 290a 0a0a 636c 6173 7320  e_path)...class 
+0001a8d0: 4669 6c65 5369 6465 4566 6665 6374 5465  FileSideEffectTe
+0001a8e0: 7374 7328 5465 7374 4361 7365 293a 0a20  sts(TestCase):. 
+0001a8f0: 2020 2064 6566 2073 6964 655f 6566 6665     def side_effe
+0001a900: 6374 2873 656c 6629 3a0a 2020 2020 2020  ct(self):.      
+0001a910: 2020 7465 7374 5f63 6173 6520 3d20 7365    test_case = se
+0001a920: 6c66 0a20 2020 2020 2020 2074 6573 745f  lf.        test_
+0001a930: 6361 7365 2e73 6964 655f 6566 6665 6374  case.side_effect
+0001a940: 5f63 616c 6c65 6420 3d20 4661 6c73 650a  _called = False.
+0001a950: 0a20 2020 2020 2020 2064 6566 205f 5f73  .        def __s
+0001a960: 6964 655f 6566 6665 6374 2866 696c 655f  ide_effect(file_
+0001a970: 6f62 6a65 6374 293a 0a20 2020 2020 2020  object):.       
+0001a980: 2020 2020 2074 6573 745f 6361 7365 2e73       test_case.s
+0001a990: 6964 655f 6566 6665 6374 5f63 616c 6c65  ide_effect_calle
+0001a9a0: 6420 3d20 5472 7565 0a20 2020 2020 2020  d = True.       
+0001a9b0: 2020 2020 2074 6573 745f 6361 7365 2e73       test_case.s
+0001a9c0: 6964 655f 6566 6665 6374 5f66 696c 655f  ide_effect_file_
+0001a9d0: 6f62 6a65 6374 5f63 6f6e 7465 6e74 203d  object_content =
+0001a9e0: 2066 696c 655f 6f62 6a65 6374 2e63 6f6e   file_object.con
+0001a9f0: 7465 6e74 730a 0a20 2020 2020 2020 2072  tents..        r
+0001aa00: 6574 7572 6e20 5f5f 7369 6465 5f65 6666  eturn __side_eff
+0001aa10: 6563 740a 0a20 2020 2064 6566 2073 6574  ect..    def set
+0001aa20: 5570 2873 656c 6629 3a0a 2020 2020 2020  Up(self):.      
+0001aa30: 2020 2320 7573 6520 7468 6520 7265 616c    # use the real
+0001aa40: 2070 6174 6820 7365 7061 7261 746f 7220   path separator 
+0001aa50: 746f 2077 6f72 6b20 7769 7468 2074 6865  to work with the
+0001aa60: 2072 6561 6c20 6669 6c65 2073 7973 7465   real file syste
+0001aa70: 6d0a 2020 2020 2020 2020 7365 6c66 2e66  m.        self.f
+0001aa80: 696c 6573 7973 7465 6d20 3d20 6661 6b65  ilesystem = fake
+0001aa90: 5f66 696c 6573 7973 7465 6d2e 4661 6b65  _filesystem.Fake
+0001aaa0: 4669 6c65 7379 7374 656d 2829 0a20 2020  Filesystem().   
+0001aab0: 2020 2020 2073 656c 662e 6669 6c65 7379       self.filesy
+0001aac0: 7374 656d 2e63 7265 6174 655f 6669 6c65  stem.create_file
+0001aad0: 2822 2f61 2f62 2f66 696c 655f 6f6e 6522  ("/a/b/file_one"
+0001aae0: 2c20 7369 6465 5f65 6666 6563 743d 7365  , side_effect=se
+0001aaf0: 6c66 2e73 6964 655f 6566 6665 6374 2829  lf.side_effect()
+0001ab00: 290a 0a20 2020 2064 6566 2074 6573 745f  )..    def test_
+0001ab10: 7369 6465 5f65 6666 6563 745f 6361 6c6c  side_effect_call
+0001ab20: 6564 2873 656c 6629 3a0a 2020 2020 2020  ed(self):.      
+0001ab30: 2020 6661 6b65 5f6f 7065 6e20 3d20 6661    fake_open = fa
+0001ab40: 6b65 5f66 696c 6573 7973 7465 6d2e 4661  ke_filesystem.Fa
+0001ab50: 6b65 4669 6c65 4f70 656e 2873 656c 662e  keFileOpen(self.
+0001ab60: 6669 6c65 7379 7374 656d 290a 2020 2020  filesystem).    
+0001ab70: 2020 2020 7365 6c66 2e73 6964 655f 6566      self.side_ef
+0001ab80: 6665 6374 5f63 616c 6c65 6420 3d20 4661  fect_called = Fa
+0001ab90: 6c73 650a 2020 2020 2020 2020 7769 7468  lse.        with
+0001aba0: 2066 616b 655f 6f70 656e 2822 2f61 2f62   fake_open("/a/b
+0001abb0: 2f66 696c 655f 6f6e 6522 2c20 2277 222c  /file_one", "w",
+0001abc0: 2065 6e63 6f64 696e 673d 2275 7466 3822   encoding="utf8"
+0001abd0: 2920 6173 2068 616e 646c 653a 0a20 2020  ) as handle:.   
+0001abe0: 2020 2020 2020 2020 2068 616e 646c 652e           handle.
+0001abf0: 7772 6974 6528 2266 6f6f 2229 0a20 2020  write("foo").   
+0001ac00: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+0001ac10: 5472 7565 2873 656c 662e 7369 6465 5f65  True(self.side_e
+0001ac20: 6666 6563 745f 6361 6c6c 6564 290a 0a20  ffect_called).. 
+0001ac30: 2020 2064 6566 2074 6573 745f 7369 6465     def test_side
+0001ac40: 5f65 6666 6563 745f 6669 6c65 5f6f 626a  _effect_file_obj
+0001ac50: 6563 7428 7365 6c66 293a 0a20 2020 2020  ect(self):.     
+0001ac60: 2020 2066 616b 655f 6f70 656e 203d 2066     fake_open = f
+0001ac70: 616b 655f 6669 6c65 7379 7374 656d 2e46  ake_filesystem.F
+0001ac80: 616b 6546 696c 654f 7065 6e28 7365 6c66  akeFileOpen(self
+0001ac90: 2e66 696c 6573 7973 7465 6d29 0a20 2020  .filesystem).   
+0001aca0: 2020 2020 2073 656c 662e 7369 6465 5f65       self.side_e
+0001acb0: 6666 6563 745f 6361 6c6c 6564 203d 2046  ffect_called = F
+0001acc0: 616c 7365 0a20 2020 2020 2020 2077 6974  alse.        wit
+0001acd0: 6820 6661 6b65 5f6f 7065 6e28 222f 612f  h fake_open("/a/
+0001ace0: 622f 6669 6c65 5f6f 6e65 222c 2022 7722  b/file_one", "w"
+0001acf0: 2c20 656e 636f 6469 6e67 3d22 7574 6638  , encoding="utf8
+0001ad00: 2229 2061 7320 6861 6e64 6c65 3a0a 2020  ") as handle:.  
+0001ad10: 2020 2020 2020 2020 2020 6861 6e64 6c65            handle
+0001ad20: 2e77 7269 7465 2822 666f 6f22 290a 2020  .write("foo").  
+0001ad30: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+0001ad40: 7445 7175 616c 2873 656c 662e 7369 6465  tEqual(self.side
+0001ad50: 5f65 6666 6563 745f 6669 6c65 5f6f 626a  _effect_file_obj
+0001ad60: 6563 745f 636f 6e74 656e 742c 2022 666f  ect_content, "fo
+0001ad70: 6f22 290a 0a0a 6966 205f 5f6e 616d 655f  o")...if __name_
+0001ad80: 5f20 3d3d 2022 5f5f 6d61 696e 5f5f 223a  _ == "__main__":
+0001ad90: 0a20 2020 2075 6e69 7474 6573 742e 6d61  .    unittest.ma
+0001ada0: 696e 2829 0a                             in().
```

### Comparing `pyfakefs-5.4.1/pyfakefs/tests/fake_filesystem_unittest_test.py` & `pyfakefs-5.5.0/pyfakefs/tests/fake_filesystem_unittest_test.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.4.1/pyfakefs/tests/fake_filesystem_vs_real_test.py` & `pyfakefs-5.5.0/pyfakefs/tests/fake_filesystem_vs_real_test.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.4.1/pyfakefs/tests/fake_open_test.py` & `pyfakefs-5.5.0/pyfakefs/tests/fake_open_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,16 @@
 import sys
 import time
 import unittest
 
 from pyfakefs import fake_filesystem, helpers
 from pyfakefs.helpers import is_root, IS_PYPY, get_locale_encoding
 from pyfakefs.fake_io import FakeIoModule
-from pyfakefs.fake_filesystem_unittest import PatchMode
+from pyfakefs.fake_filesystem_unittest import PatchMode, Patcher
+from pyfakefs.tests.skip_open import read_open
 from pyfakefs.tests.test_utils import RealFsTestCase
 
 
 class FakeFileOpenTestBase(RealFsTestCase):
     def setUp(self):
         super(FakeFileOpenTestBase, self).setUp()
         if self.use_real_fs():
@@ -2100,9 +2101,16 @@
 
 
 class RealResolvePathTest(ResolvePathTest):
     def use_real_fs(self):
         return True
 
 
+class SkipOpenTest(unittest.TestCase):
+    def test_open_in_skipped_module(self):
+        with Patcher(additional_skip_names=["skip_open"]):
+            contents = read_open("skip_open.py")
+            self.assertTrue(contents.startswith("# Licensed under the Apache License"))
+
+
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `pyfakefs-5.4.1/pyfakefs/tests/fake_os_test.py` & `pyfakefs-5.5.0/pyfakefs/tests/fake_os_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,29 +17,22 @@
 
 import errno
 import os
 import stat
 import sys
 import unittest
 
-from pyfakefs.helpers import IN_DOCKER, IS_PYPY, get_uid, get_gid, reset_ids
-
 from pyfakefs import fake_filesystem, fake_os, fake_open, fake_file
 from pyfakefs.fake_filesystem import (
     FakeFileOpen,
     is_root,
     set_uid,
     set_gid,
 )
-from pyfakefs.extra_packages import (
-    use_scandir,
-    use_scandir_package,
-    use_builtin_scandir,
-)
-
+from pyfakefs.helpers import IN_DOCKER, IS_PYPY, get_uid, get_gid, reset_ids
 from pyfakefs.tests.test_utils import TestCase, RealFsTestCase
 
 
 class FakeOsModuleTestBase(RealFsTestCase):
     def setUp(self):
         super().setUp()
         self.umask = self.os.umask(0o022)
@@ -5240,36 +5233,25 @@
         # test file truncation
         fh = self.open(file_path, "w", encoding="utf8")
         self.assertEqual(0, self.os.stat(file_path)[stat.ST_SIZE])
         self.assertEqual("", self.filesystem.get_object(file_path).contents)
         fh.close()
 
 
-@unittest.skipIf(not use_scandir, "only run if scandir is available")
 class FakeScandirTest(FakeOsModuleTestBase):
     FILE_SIZE = 50
     LINKED_FILE_SIZE = 10
 
+    def used_scandir(self):
+        return self.os.scandir
+
     def setUp(self):
         super().setUp()
         self.supports_symlinks = not self.is_windows or not self.use_real_fs()
-
-        if use_scandir_package:
-            if self.use_real_fs():
-                from scandir import scandir
-            else:
-                import pyfakefs.fake_scandir
-
-                def fake_scan_dir(p):
-                    return pyfakefs.fake_scandir.scandir(self.filesystem, p)
-
-                scandir = fake_scan_dir
-        else:
-            scandir = self.os.scandir
-        self.scandir = scandir
+        self.scandir = self.used_scandir()
 
         self.directory = self.make_path("xyzzy", "plugh")
         link_dir = self.make_path("linked", "plugh")
         self.linked_file_path = self.os.path.join(link_dir, "file")
         self.linked_dir_path = self.os.path.join(link_dir, "dir")
         self.rel_linked_dir_path = self.os.path.join(
             "..", "..", "linked", "plugh", "dir"
@@ -5379,15 +5361,15 @@
         self.os.symlink(dir_path, link_path)
         self.assertEqual(
             [self.os.path.join(link_path, "D")],
             [f.path for f in self.scandir(link_path)],
         )
 
     def test_inode(self):
-        if use_scandir and self.use_real_fs():
+        if self.use_real_fs():
             if self.is_windows:
                 self.skipTest("inode seems not to work in scandir module under Windows")
             if IN_DOCKER:
                 self.skipTest("inode seems not to work in a Docker container")
         self.assertEqual(
             self.os.stat(self.dir_path).st_ino, self.dir_entries[0].inode()
         )
@@ -5499,18 +5481,14 @@
         if self.supports_symlinks:
             file_stat = self.os.stat(self.linked_file_path)
             self.assertEqual(file_stat.st_ino, self.dir_entries[3].stat().st_ino)
             self.assertEqual(file_stat.st_dev, self.dir_entries[3].stat().st_dev)
             self.assertEqual(file_stat.st_ino, self.dir_entries[5].stat().st_ino)
             self.assertEqual(file_stat.st_dev, self.dir_entries[5].stat().st_dev)
 
-    @unittest.skipIf(
-        not use_builtin_scandir,
-        "Path-like objects not available in scandir package",
-    )
     def test_path_like(self):
         self.assertTrue(isinstance(self.dir_entries[0], os.PathLike))
         self.assertEqual(
             self.os.path.join(self.scandir_path(), "dir"),
             os.fspath(self.dir_entries[0]),
         )
         self.assertEqual(
@@ -5541,15 +5519,14 @@
 
 class RealScandirRelTest(FakeScandirRelTest):
     def use_real_fs(self):
         return True
 
 
 @unittest.skipIf(TestCase.is_windows, "dir_fd not supported for os.scandir in Windows")
-@unittest.skipIf(use_scandir_package, "no dir_fd support for scandir package")
 class FakeScandirFdTest(FakeScandirTest):
     def tearDown(self):
         self.os.close(self.dir_fd)
         super().tearDown()
 
     def scandir_path(self):
         # When scandir is called with a filedescriptor, only the name of the
```

### Comparing `pyfakefs-5.4.1/pyfakefs/tests/fake_pathlib_test.py` & `pyfakefs-5.5.0/pyfakefs/tests/fake_pathlib_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,37 +27,42 @@
 import unittest
 from collections import namedtuple
 from unittest import mock
 from unittest.mock import patch
 
 from pyfakefs import fake_pathlib, fake_filesystem, fake_filesystem_unittest, fake_os
 from pyfakefs.fake_filesystem import OSType
+from pyfakefs.fake_filesystem_unittest import Patcher
 from pyfakefs.helpers import IS_PYPY, is_root
+from pyfakefs.tests.skip_open import read_pathlib
 from pyfakefs.tests.test_utils import RealFsTestMixin
 
 is_windows = sys.platform == "win32"
 
 
 class RealPathlibTestCase(fake_filesystem_unittest.TestCase, RealFsTestMixin):
     is_windows = sys.platform == "win32"
 
     def __init__(self, methodName="runTest"):
         fake_filesystem_unittest.TestCase.__init__(self, methodName)
         RealFsTestMixin.__init__(self)
 
+    def used_pathlib(self):
+        return pathlib
+
     def setUp(self):
         RealFsTestMixin.setUp(self)
         self.filesystem = None
         self.real_os = os
         if not self.use_real_fs():
             self.setUpPyfakefs()
             self.filesystem = self.fs
             self.create_basepath()
-        self.pathlib = pathlib
-        self.path = pathlib.Path
+        self.pathlib = self.used_pathlib()
+        self.path = self.pathlib.Path
         self.os = os
         self.open = open
 
     def use_real_fs(self):
         return False
 
 
@@ -1279,9 +1284,43 @@
         self.assertTrue(path.is_file())
         # but it does in forced UNIX mode
         self.fs.chmod("/foo", 0o000, force_unix_mode=True)
         with self.assertRaises(PermissionError):
             path.is_file()
 
 
+class FakePathlibModulePurePathTest(unittest.TestCase):
+    def test_windows_pure_path_parsing(self):
+        """Verify faked pure Windows paths use filesystem-independent separators."""
+
+        path = r"C:\Windows\cmd.exe"
+        self.assertEqual(
+            fake_pathlib.FakePathlibModule.PureWindowsPath(path).stem,
+            pathlib.PureWindowsPath(path).stem,
+        )
+
+        path = r"C:/Windows/cmd.exe"
+        self.assertEqual(
+            fake_pathlib.FakePathlibModule.PureWindowsPath(path).stem,
+            pathlib.PureWindowsPath(path).stem,
+        )
+
+    def test_posix_pure_path_parsing(self):
+        """Verify faked pure POSIX paths use filesystem-independent separators."""
+
+        path = r"/bin/bash"
+        self.assertEqual(
+            fake_pathlib.FakePathlibModule.PurePosixPath(path).stem,
+            pathlib.PurePosixPath(path).stem,
+        )
+
+
+class SkipOpenTest(unittest.TestCase):
+    def test_open_pathlib_in_skipped_module(self):
+        # regression test for #1012
+        with Patcher(additional_skip_names=["skip_open"]):
+            contents = read_pathlib("skip_open.py")
+            self.assertTrue(contents.startswith("# Licensed under the Apache License"))
+
+
 if __name__ == "__main__":
     unittest.main(verbosity=2)
```

### Comparing `pyfakefs-5.4.1/pyfakefs/tests/fake_stat_time_test.py` & `pyfakefs-5.5.0/pyfakefs/tests/fake_stat_time_test.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.4.1/pyfakefs/tests/fake_tempfile_test.py` & `pyfakefs-5.5.0/pyfakefs/tests/fake_tempfile_test.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.4.1/pyfakefs/tests/fixtures/deprecated_property.py` & `pyfakefs-5.5.0/pyfakefs/tests/fixtures/deprecated_property.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.4.1/pyfakefs/tests/fixtures/module_with_attributes.py` & `pyfakefs-5.5.0/pyfakefs/tests/fixtures/module_with_attributes.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.4.1/pyfakefs/tests/import_as_example.py` & `pyfakefs-5.5.0/pyfakefs/tests/import_as_example.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.4.1/pyfakefs/tests/logsio.py` & `pyfakefs-5.5.0/pyfakefs/tests/logsio.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.4.1/pyfakefs/tests/mox3_stubout_example.py` & `pyfakefs-5.5.0/pyfakefs/tests/mox3_stubout_example.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.4.1/pyfakefs/tests/mox3_stubout_test.py` & `pyfakefs-5.5.0/pyfakefs/tests/mox3_stubout_test.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.4.1/pyfakefs/tests/patched_packages_test.py` & `pyfakefs-5.5.0/pyfakefs/tests/patched_packages_test.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.4.1/pyfakefs/tests/performance_test.py` & `pyfakefs-5.5.0/pyfakefs/tests/performance_test.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.4.1/pyfakefs/tests/test_utils.py` & `pyfakefs-5.5.0/pyfakefs/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.4.1/pyfakefs.egg-info/PKG-INFO` & `pyfakefs-5.5.0/pyfakefs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfakefs
-Version: 5.4.1
+Version: 5.5.0
 Summary: pyfakefs implements a fake file system that mocks the Python file system modules.
 Home-page: https://github.com/pytest-dev/pyfakefs
 Author: Google
 Author-email: google-pyfakefs@google.com
 Maintainer: John McGehee
 Maintainer-email: pyfakefs@johnnado.com
 License: http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `pyfakefs-5.4.1/pyfakefs.egg-info/SOURCES.txt` & `pyfakefs-5.5.0/pyfakefs.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 CHANGES.md
 CONTRIBUTING.md
 COPYING
 MANIFEST.in
 README.md
 extra_requirements.txt
+legacy_requirements.txt
 mypy.ini
 pyproject.toml
 requirements.txt
 requirements_dev.txt
 setup.cfg
 setup.py
 tox.ini
 pyfakefs/__init__.py
 pyfakefs/_version.py
-pyfakefs/extra_packages.py
 pyfakefs/fake_file.py
 pyfakefs/fake_filesystem.py
 pyfakefs/fake_filesystem_shutil.py
 pyfakefs/fake_filesystem_unittest.py
 pyfakefs/fake_io.py
+pyfakefs/fake_legacy_modules.py
 pyfakefs/fake_open.py
 pyfakefs/fake_os.py
 pyfakefs/fake_path.py
 pyfakefs/fake_pathlib.py
 pyfakefs/fake_scandir.py
 pyfakefs/helpers.py
+pyfakefs/legacy_packages.py
 pyfakefs/mox3_stubout.py
 pyfakefs/patched_packages.py
 pyfakefs/py.typed
 pyfakefs/pytest_plugin.py
 pyfakefs.egg-info/PKG-INFO
 pyfakefs.egg-info/SOURCES.txt
 pyfakefs.egg-info/dependency_links.txt
@@ -54,23 +56,25 @@
 pyfakefs/tests/example.py
 pyfakefs/tests/example_test.py
 pyfakefs/tests/fake_filesystem_glob_test.py
 pyfakefs/tests/fake_filesystem_shutil_test.py
 pyfakefs/tests/fake_filesystem_test.py
 pyfakefs/tests/fake_filesystem_unittest_test.py
 pyfakefs/tests/fake_filesystem_vs_real_test.py
+pyfakefs/tests/fake_legacy_modules_test.py
 pyfakefs/tests/fake_open_test.py
 pyfakefs/tests/fake_os_test.py
 pyfakefs/tests/fake_pathlib_test.py
 pyfakefs/tests/fake_stat_time_test.py
 pyfakefs/tests/fake_tempfile_test.py
 pyfakefs/tests/import_as_example.py
 pyfakefs/tests/logsio.py
 pyfakefs/tests/mox3_stubout_example.py
 pyfakefs/tests/mox3_stubout_test.py
 pyfakefs/tests/patched_packages_test.py
 pyfakefs/tests/performance_test.py
+pyfakefs/tests/skip_open.py
 pyfakefs/tests/test_utils.py
 pyfakefs/tests/fixtures/__init__.py
 pyfakefs/tests/fixtures/config_module.py
 pyfakefs/tests/fixtures/deprecated_property.py
 pyfakefs/tests/fixtures/module_with_attributes.py
```

### Comparing `pyfakefs-5.4.1/setup.cfg` & `pyfakefs-5.5.0/setup.cfg`

 * *Files identical despite different names*

