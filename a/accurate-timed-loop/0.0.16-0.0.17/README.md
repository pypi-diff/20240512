# Comparing `tmp/accurate-timed-loop-0.0.16.tar.gz` & `tmp/accurate_timed_loop-0.0.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "accurate-timed-loop-0.0.16.tar", last modified: Wed Dec 20 04:10:25 2023, max compression
+gzip compressed data, was "accurate_timed_loop-0.0.17.tar", last modified: Sun May 12 00:18:49 2024, max compression
```

## Comparing `accurate-timed-loop-0.0.16.tar` & `accurate_timed_loop-0.0.17.tar`

### file list

```diff
@@ -1,39 +1,58 @@
-drwxrwxr-x   0 arrizza   (1000) arrizza   (1000)        0 2023-12-20 04:10:25.497873 accurate-timed-loop-0.0.16/
--rw-rw-r--   0 arrizza   (1000) arrizza   (1000)     1090 2023-03-13 00:01:54.000000 accurate-timed-loop-0.0.16/LICENSE.txt
--rw-rw-r--   0 arrizza   (1000) arrizza   (1000)       51 2023-12-20 04:10:25.000000 accurate-timed-loop-0.0.16/MANIFEST.in
--rw-r--r--   0 arrizza   (1000) arrizza   (1000)     4806 2023-12-20 04:10:25.497873 accurate-timed-loop-0.0.16/PKG-INFO
--rw-rw-r--   0 arrizza   (1000) arrizza   (1000)     4045 2023-03-13 00:01:54.000000 accurate-timed-loop-0.0.16/README.md
-drwxrwxr-x   0 arrizza   (1000) arrizza   (1000)        0 2023-12-20 04:10:25.493873 accurate-timed-loop-0.0.16/accurate_timed_loop/
--rw-rw-r--   0 arrizza   (1000) arrizza   (1000)       55 2023-03-13 00:01:54.000000 accurate-timed-loop-0.0.16/accurate_timed_loop/__init__.py
-drwxrwxr-x   0 arrizza   (1000) arrizza   (1000)        0 2023-12-20 04:10:25.493873 accurate-timed-loop-0.0.16/accurate_timed_loop/lib/
--rw-rw-r--   0 arrizza   (1000) arrizza   (1000)       29 2023-12-12 19:40:48.000000 accurate-timed-loop-0.0.16/accurate_timed_loop/lib/.gitignore
--rw-rw-r--   0 arrizza   (1000) arrizza   (1000)      282 2023-12-20 04:10:25.000000 accurate-timed-loop-0.0.16/accurate_timed_loop/lib/build_info.py
--rw-rw-r--   0 arrizza   (1000) arrizza   (1000)     1327 2023-12-06 09:14:14.000000 accurate-timed-loop-0.0.16/accurate_timed_loop/lib/main.py
--rw-rw-r--   0 arrizza   (1000) arrizza   (1000)       27 2023-12-20 04:10:25.000000 accurate-timed-loop-0.0.16/accurate_timed_loop/lib/version.json
-drwxrwxr-x   0 arrizza   (1000) arrizza   (1000)        0 2023-12-20 04:10:25.497873 accurate-timed-loop-0.0.16/accurate_timed_loop.egg-info/
--rw-r--r--   0 arrizza   (1000) arrizza   (1000)     4806 2023-12-20 04:10:25.000000 accurate-timed-loop-0.0.16/accurate_timed_loop.egg-info/PKG-INFO
--rw-rw-r--   0 arrizza   (1000) arrizza   (1000)      714 2023-12-20 04:10:25.000000 accurate-timed-loop-0.0.16/accurate_timed_loop.egg-info/SOURCES.txt
--rw-rw-r--   0 arrizza   (1000) arrizza   (1000)        1 2023-12-20 04:10:25.000000 accurate-timed-loop-0.0.16/accurate_timed_loop.egg-info/dependency_links.txt
--rw-rw-r--   0 arrizza   (1000) arrizza   (1000)       35 2023-12-20 04:10:25.000000 accurate-timed-loop-0.0.16/accurate_timed_loop.egg-info/requires.txt
--rw-rw-r--   0 arrizza   (1000) arrizza   (1000)       37 2023-12-20 04:10:25.000000 accurate-timed-loop-0.0.16/accurate_timed_loop.egg-info/top_level.txt
-drwxrwxr-x   0 arrizza   (1000) arrizza   (1000)        0 2023-12-20 04:10:25.493873 accurate-timed-loop-0.0.16/sample/
--rw-rw-r--   0 arrizza   (1000) arrizza   (1000)        0 2023-12-06 06:30:03.000000 accurate-timed-loop-0.0.16/sample/__init__.py
--rw-rw-r--   0 arrizza   (1000) arrizza   (1000)     2816 2023-12-06 09:42:33.000000 accurate-timed-loop-0.0.16/sample/main.py
--rw-rw-r--   0 arrizza   (1000) arrizza   (1000)      626 2023-12-20 04:10:25.497873 accurate-timed-loop-0.0.16/setup.cfg
--rw-rw-r--   0 arrizza   (1000) arrizza   (1000)     1422 2023-12-20 04:10:25.000000 accurate-timed-loop-0.0.16/setup.py
-drwxrwxr-x   0 arrizza   (1000) arrizza   (1000)        0 2023-12-20 04:10:25.493873 accurate-timed-loop-0.0.16/tools/
--rw-rw-r--   0 arrizza   (1000) arrizza   (1000)        0 2023-03-13 00:01:54.000000 accurate-timed-loop-0.0.16/tools/__init__.py
--rw-rw-r--   0 arrizza   (1000) arrizza   (1000)     4065 2023-12-19 00:36:34.000000 accurate-timed-loop-0.0.16/tools/debug_logger.py
-drwxrwxr-x   0 arrizza   (1000) arrizza   (1000)        0 2023-12-20 04:10:25.493873 accurate-timed-loop-0.0.16/tools/install/
--rw-rw-r--   0 arrizza   (1000) arrizza   (1000)        0 2023-12-07 04:48:04.000000 accurate-timed-loop-0.0.16/tools/install/__init__.py
--rw-rw-r--   0 arrizza   (1000) arrizza   (1000)      637 2023-03-13 00:01:54.000000 accurate-timed-loop-0.0.16/tools/loader.py
--rw-rw-r--   0 arrizza   (1000) arrizza   (1000)     1437 2023-12-18 12:55:00.000000 accurate-timed-loop-0.0.16/tools/main.py
--rw-rw-r--   0 arrizza   (1000) arrizza   (1000)     1328 2023-12-20 04:01:05.000000 accurate-timed-loop-0.0.16/tools/setup_template.py
-drwxrwxr-x   0 arrizza   (1000) arrizza   (1000)        0 2023-12-20 04:10:25.493873 accurate-timed-loop-0.0.16/tools/xplat_utils/
--rw-rw-r--   0 arrizza   (1000) arrizza   (1000)       29 2023-12-20 03:57:23.000000 accurate-timed-loop-0.0.16/tools/xplat_utils/__init__.py
-drwxrwxr-x   0 arrizza   (1000) arrizza   (1000)        0 2023-12-20 04:10:25.493873 accurate-timed-loop-0.0.16/ver/
--rw-rw-r--   0 arrizza   (1000) arrizza   (1000)        0 2023-12-06 06:30:03.000000 accurate-timed-loop-0.0.16/ver/__init__.py
-drwxrwxr-x   0 arrizza   (1000) arrizza   (1000)        0 2023-12-20 04:10:25.497873 accurate-timed-loop-0.0.16/ver/helpers/
--rw-rw-r--   0 arrizza   (1000) arrizza   (1000)        0 2023-12-06 06:30:03.000000 accurate-timed-loop-0.0.16/ver/helpers/__init__.py
--rw-rw-r--   0 arrizza   (1000) arrizza   (1000)       99 2023-12-06 08:31:28.000000 accurate-timed-loop-0.0.16/ver/helpers/gen_report.py
--rw-rw-r--   0 arrizza   (1000) arrizza   (1000)     3283 2023-12-06 09:26:01.000000 accurate-timed-loop-0.0.16/ver/test_tp001_basic.py
+drwxrwxr-x   0 arrizza   (1000) arrizza   (1000)        0 2024-05-12 00:18:49.038115 accurate_timed_loop-0.0.17/
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)     1090 2023-03-13 00:01:54.000000 accurate_timed_loop-0.0.17/LICENSE.txt
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)       51 2024-05-12 00:18:48.000000 accurate_timed_loop-0.0.17/MANIFEST.in
+-rw-r--r--   0 arrizza   (1000) arrizza   (1000)     5054 2024-05-12 00:18:49.038115 accurate_timed_loop-0.0.17/PKG-INFO
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)     4290 2024-02-29 02:07:37.000000 accurate_timed_loop-0.0.17/README.md
+drwxrwxr-x   0 arrizza   (1000) arrizza   (1000)        0 2024-05-12 00:18:49.034115 accurate_timed_loop-0.0.17/accurate_timed_loop/
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)       55 2023-03-13 00:01:54.000000 accurate_timed_loop-0.0.17/accurate_timed_loop/__init__.py
+drwxrwxr-x   0 arrizza   (1000) arrizza   (1000)        0 2024-05-12 00:18:49.038115 accurate_timed_loop-0.0.17/accurate_timed_loop/lib/
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)       29 2023-12-12 19:40:48.000000 accurate_timed_loop-0.0.17/accurate_timed_loop/lib/.gitignore
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)      282 2024-05-12 00:18:48.000000 accurate_timed_loop-0.0.17/accurate_timed_loop/lib/build_info.py
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)     1327 2023-12-06 09:14:14.000000 accurate_timed_loop-0.0.17/accurate_timed_loop/lib/main.py
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)       27 2024-05-12 00:18:48.000000 accurate_timed_loop-0.0.17/accurate_timed_loop/lib/version.json
+drwxrwxr-x   0 arrizza   (1000) arrizza   (1000)        0 2024-05-12 00:18:49.038115 accurate_timed_loop-0.0.17/accurate_timed_loop.egg-info/
+-rw-r--r--   0 arrizza   (1000) arrizza   (1000)     5054 2024-05-12 00:18:48.000000 accurate_timed_loop-0.0.17/accurate_timed_loop.egg-info/PKG-INFO
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)     1315 2024-05-12 00:18:48.000000 accurate_timed_loop-0.0.17/accurate_timed_loop.egg-info/SOURCES.txt
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)        1 2024-05-12 00:18:48.000000 accurate_timed_loop-0.0.17/accurate_timed_loop.egg-info/dependency_links.txt
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)       38 2024-05-12 00:18:48.000000 accurate_timed_loop-0.0.17/accurate_timed_loop.egg-info/requires.txt
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)       37 2024-05-12 00:18:48.000000 accurate_timed_loop-0.0.17/accurate_timed_loop.egg-info/top_level.txt
+drwxrwxr-x   0 arrizza   (1000) arrizza   (1000)        0 2024-05-12 00:18:49.038115 accurate_timed_loop-0.0.17/sample/
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)        0 2023-12-06 06:30:03.000000 accurate_timed_loop-0.0.17/sample/__init__.py
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)     2815 2024-03-29 20:40:54.000000 accurate_timed_loop-0.0.17/sample/main.py
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)      626 2024-05-12 00:18:49.042115 accurate_timed_loop-0.0.17/setup.cfg
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)     1425 2024-05-12 00:18:48.000000 accurate_timed_loop-0.0.17/setup.py
+drwxrwxr-x   0 arrizza   (1000) arrizza   (1000)        0 2024-05-12 00:18:49.038115 accurate_timed_loop-0.0.17/tools/
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)        0 2023-03-13 00:01:54.000000 accurate_timed_loop-0.0.17/tools/__init__.py
+drwxrwxr-x   0 arrizza   (1000) arrizza   (1000)        0 2024-05-12 00:18:49.038115 accurate_timed_loop-0.0.17/tools/install/
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)        0 2023-12-07 04:48:04.000000 accurate_timed_loop-0.0.17/tools/install/__init__.py
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)      637 2023-03-13 00:01:54.000000 accurate_timed_loop-0.0.17/tools/loader.py
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)     1331 2024-05-11 21:25:40.000000 accurate_timed_loop-0.0.17/tools/setup_template.py
+drwxrwxr-x   0 arrizza   (1000) arrizza   (1000)        0 2024-05-12 00:18:49.038115 accurate_timed_loop-0.0.17/tools/xplat_utils/
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)       25 2024-02-13 13:56:34.000000 accurate_timed_loop-0.0.17/tools/xplat_utils/__init__.py
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)    11846 2024-03-07 17:23:42.000000 accurate_timed_loop-0.0.17/tools/xplat_utils/cfg.py
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)     2942 2024-03-26 21:35:50.000000 accurate_timed_loop-0.0.17/tools/xplat_utils/do_build.py
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)    29185 2024-05-11 14:21:21.000000 accurate_timed_loop-0.0.17/tools/xplat_utils/do_check.py
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)     2630 2024-03-07 23:15:50.000000 accurate_timed_loop-0.0.17/tools/xplat_utils/do_clean.py
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)     3880 2024-02-26 17:02:10.000000 accurate_timed_loop-0.0.17/tools/xplat_utils/do_coverage.py
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)     5580 2024-02-20 05:18:25.000000 accurate_timed_loop-0.0.17/tools/xplat_utils/do_doc.py
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)     3611 2024-03-09 16:54:31.000000 accurate_timed_loop-0.0.17/tools/xplat_utils/do_lint.py
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)     3388 2024-05-11 14:21:21.000000 accurate_timed_loop-0.0.17/tools/xplat_utils/do_post_ver.py
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)     2460 2024-02-17 03:26:37.000000 accurate_timed_loop-0.0.17/tools/xplat_utils/do_publish.py
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)     1713 2024-03-11 22:17:02.000000 accurate_timed_loop-0.0.17/tools/xplat_utils/do_upload.py
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)     2074 2024-02-26 17:02:10.000000 accurate_timed_loop-0.0.17/tools/xplat_utils/do_ver_info.py
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)     6076 2024-02-26 17:02:10.000000 accurate_timed_loop-0.0.17/tools/xplat_utils/gen_build_info.py
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)     4064 2024-02-26 17:02:10.000000 accurate_timed_loop-0.0.17/tools/xplat_utils/gen_files.py
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)      174 2024-02-17 01:38:03.000000 accurate_timed_loop-0.0.17/tools/xplat_utils/main.py
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)    12926 2024-02-26 17:02:10.000000 accurate_timed_loop-0.0.17/tools/xplat_utils/os_specific.py
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)     1330 2024-03-07 17:23:42.000000 accurate_timed_loop-0.0.17/tools/xplat_utils/svc.py
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)     8201 2024-03-29 17:26:56.000000 accurate_timed_loop-0.0.17/tools/xplat_utils/utils.py
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)     4670 2024-03-07 17:23:42.000000 accurate_timed_loop-0.0.17/tools/xplat_utils/utils_fs.py
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)     5091 2024-04-16 20:36:28.000000 accurate_timed_loop-0.0.17/tools/xplat_utils/utils_logger.py
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)     2938 2024-02-21 00:38:29.000000 accurate_timed_loop-0.0.17/tools/xplat_utils/utils_ps.py
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)     1142 2024-02-13 13:56:34.000000 accurate_timed_loop-0.0.17/tools/xplat_utils/utils_val.py
+drwxrwxr-x   0 arrizza   (1000) arrizza   (1000)        0 2024-05-12 00:18:49.038115 accurate_timed_loop-0.0.17/ver/
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)        0 2023-12-06 06:30:03.000000 accurate_timed_loop-0.0.17/ver/__init__.py
+drwxrwxr-x   0 arrizza   (1000) arrizza   (1000)        0 2024-05-12 00:18:49.038115 accurate_timed_loop-0.0.17/ver/helpers/
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)        0 2023-12-06 06:30:03.000000 accurate_timed_loop-0.0.17/ver/helpers/__init__.py
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)       99 2023-12-06 08:31:28.000000 accurate_timed_loop-0.0.17/ver/helpers/gen_report.py
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)     3282 2024-03-29 20:40:54.000000 accurate_timed_loop-0.0.17/ver/test_tp001_basic.py
```

### Comparing `accurate-timed-loop-0.0.16/LICENSE.txt` & `accurate_timed_loop-0.0.17/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `accurate-timed-loop-0.0.16/PKG-INFO` & `accurate_timed_loop-0.0.17/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: accurate-timed-loop
-Version: 0.0.16
+Version: 0.0.17
 Summary: Accurate timed loop
 Home-page: https://bitbucket.org/arrizza-public/accurate-timed-loop/src/master
 Download-URL: https://bitbucket.org/arrizza-public/accurate-timed-loop/get/master.zip
 Author: JA
 Author-email: cppgent0@gmail.com
 License: MIT
 Keywords: accurate loop,utility
@@ -12,39 +12,46 @@
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Utilities
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: pytest-ver
+Requires-Dist: medver-pytest
 Requires-Dist: pytest
 Requires-Dist: on_the_fly_stats
 
-# Accurate Timed Loop #
+website: <https://arrizza.com/python-accurate-timed-loop>
 
-This is a python module that provide a way to have an acccurate timed loop.
+## Summary
+
+This is a python module that provides a way to have an acccurate timed loop.
 
 For example if you need to do an activity every 250ms +/-10ms, this loop will do that.
 
-### Sample code ###
+## Sample code
 
 see sample.py for a full example
 
 ```python
 import accurate_timed_loop
 
 loop_delay = 0.250  # seconds
 total_wait = 25.0  # seconds
 for elapsed, start_time in accurate_timed_loop.accurate_wait(total_wait, loop_delay):
     # ... do task every 250 mS
     pass
 ```
 
-### Accuracy and Limitations ###
+## Scripts
+
+* See [Quick Start](https://arrizza.com/user-guide-quick-start) for information on using scripts.
+* See [xplat-utils submodule](https://arrizza.com/xplat-utils) for information on the submodule.
+
+## Accuracy and Limitations
 
 The sample.py does testing and shows that on Windows MSYS2 the std deviation error is roughly
 4mS in a 250mS loop. This means that 95% of loops will be +/-8 mS of the requested loop_delay.
 
 ```text
       expected    elapsed  diff1(ms)  actual(s)  diff2(ms)
   1   0.000000   0.000000      0.000   0.000000      0.000
@@ -71,25 +78,25 @@
 The Stdev and Average error values at that point should be miminal.
 
 ```python
 import accurate_timed_loop
 
 loop_delay = 0.250  # seconds
 total_wait = 25.0  # seconds
-adj = 0.009228  # macos
+adj = 0.009228  # macOS
 for elapsed, start_time in accurate_timed_loop.accurate_wait(total_wait, loop_delay, fixed_adjustment=adj):
     # ... do task every 250 mS
     pass
 ```
 
 Notes:
 
 * Re-run this several times, and tweak the fixed adjustment.
 * The sample.py reports a "Recommended adj" that usually results in better accuracy.
-* Macos and Ubuntu tend to be less variant than Windows
+* macOS and Ubuntu tend to be less variant than Windows
 
 This report shows that std deviation is much better.
 
 ```text
       expected    elapsed  diff1(ms)  actual(s)  diff2(ms)
   1   0.000000   0.000000      0.000   0.000000      0.000
   2   0.250000   0.251537      1.537   0.251537      1.537
@@ -107,15 +114,15 @@
      sample rc=0
      doit overall rc=0
 ```
 
 Limitations:
 
 * there is NO guarantee that the average error will always be that low or that consistent
-* the following runs were on a Macos
+* the following runs were on a macOS
 
 ```text
 # === first run:
 Stats:
 loop count     : 102 loops
 Error Range    : -9.486 to 4.613 mS
 Error Stddev   :      1.962 mS
```

### Comparing `accurate-timed-loop-0.0.16/README.md` & `accurate_timed_loop-0.0.17/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,35 @@
-# Accurate Timed Loop #
+website: <https://arrizza.com/python-accurate-timed-loop>
 
-This is a python module that provide a way to have an acccurate timed loop.
+## Summary
+
+This is a python module that provides a way to have an acccurate timed loop.
 
 For example if you need to do an activity every 250ms +/-10ms, this loop will do that.
 
-### Sample code ###
+## Sample code
 
 see sample.py for a full example
 
 ```python
 import accurate_timed_loop
 
 loop_delay = 0.250  # seconds
 total_wait = 25.0  # seconds
 for elapsed, start_time in accurate_timed_loop.accurate_wait(total_wait, loop_delay):
     # ... do task every 250 mS
     pass
 ```
 
-### Accuracy and Limitations ###
+## Scripts
+
+* See [Quick Start](https://arrizza.com/user-guide-quick-start) for information on using scripts.
+* See [xplat-utils submodule](https://arrizza.com/xplat-utils) for information on the submodule.
+
+## Accuracy and Limitations
 
 The sample.py does testing and shows that on Windows MSYS2 the std deviation error is roughly
 4mS in a 250mS loop. This means that 95% of loops will be +/-8 mS of the requested loop_delay.
 
 ```text
       expected    elapsed  diff1(ms)  actual(s)  diff2(ms)
   1   0.000000   0.000000      0.000   0.000000      0.000
@@ -49,25 +56,25 @@
 The Stdev and Average error values at that point should be miminal.
 
 ```python
 import accurate_timed_loop
 
 loop_delay = 0.250  # seconds
 total_wait = 25.0  # seconds
-adj = 0.009228  # macos
+adj = 0.009228  # macOS
 for elapsed, start_time in accurate_timed_loop.accurate_wait(total_wait, loop_delay, fixed_adjustment=adj):
     # ... do task every 250 mS
     pass
 ```
 
 Notes:
 
 * Re-run this several times, and tweak the fixed adjustment.
 * The sample.py reports a "Recommended adj" that usually results in better accuracy.
-* Macos and Ubuntu tend to be less variant than Windows
+* macOS and Ubuntu tend to be less variant than Windows
 
 This report shows that std deviation is much better.
 
 ```text
       expected    elapsed  diff1(ms)  actual(s)  diff2(ms)
   1   0.000000   0.000000      0.000   0.000000      0.000
   2   0.250000   0.251537      1.537   0.251537      1.537
@@ -85,15 +92,15 @@
      sample rc=0
      doit overall rc=0
 ```
 
 Limitations:
 
 * there is NO guarantee that the average error will always be that low or that consistent
-* the following runs were on a Macos
+* the following runs were on a macOS
 
 ```text
 # === first run:
 Stats:
 loop count     : 102 loops
 Error Range    : -9.486 to 4.613 mS
 Error Stddev   :      1.962 mS
```

### Comparing `accurate-timed-loop-0.0.16/accurate_timed_loop/lib/main.py` & `accurate_timed_loop-0.0.17/accurate_timed_loop/lib/main.py`

 * *Files identical despite different names*

### Comparing `accurate-timed-loop-0.0.16/accurate_timed_loop.egg-info/PKG-INFO` & `accurate_timed_loop-0.0.17/accurate_timed_loop.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: accurate-timed-loop
-Version: 0.0.16
+Version: 0.0.17
 Summary: Accurate timed loop
 Home-page: https://bitbucket.org/arrizza-public/accurate-timed-loop/src/master
 Download-URL: https://bitbucket.org/arrizza-public/accurate-timed-loop/get/master.zip
 Author: JA
 Author-email: cppgent0@gmail.com
 License: MIT
 Keywords: accurate loop,utility
@@ -12,39 +12,46 @@
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Utilities
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: pytest-ver
+Requires-Dist: medver-pytest
 Requires-Dist: pytest
 Requires-Dist: on_the_fly_stats
 
-# Accurate Timed Loop #
+website: <https://arrizza.com/python-accurate-timed-loop>
 
-This is a python module that provide a way to have an acccurate timed loop.
+## Summary
+
+This is a python module that provides a way to have an acccurate timed loop.
 
 For example if you need to do an activity every 250ms +/-10ms, this loop will do that.
 
-### Sample code ###
+## Sample code
 
 see sample.py for a full example
 
 ```python
 import accurate_timed_loop
 
 loop_delay = 0.250  # seconds
 total_wait = 25.0  # seconds
 for elapsed, start_time in accurate_timed_loop.accurate_wait(total_wait, loop_delay):
     # ... do task every 250 mS
     pass
 ```
 
-### Accuracy and Limitations ###
+## Scripts
+
+* See [Quick Start](https://arrizza.com/user-guide-quick-start) for information on using scripts.
+* See [xplat-utils submodule](https://arrizza.com/xplat-utils) for information on the submodule.
+
+## Accuracy and Limitations
 
 The sample.py does testing and shows that on Windows MSYS2 the std deviation error is roughly
 4mS in a 250mS loop. This means that 95% of loops will be +/-8 mS of the requested loop_delay.
 
 ```text
       expected    elapsed  diff1(ms)  actual(s)  diff2(ms)
   1   0.000000   0.000000      0.000   0.000000      0.000
@@ -71,25 +78,25 @@
 The Stdev and Average error values at that point should be miminal.
 
 ```python
 import accurate_timed_loop
 
 loop_delay = 0.250  # seconds
 total_wait = 25.0  # seconds
-adj = 0.009228  # macos
+adj = 0.009228  # macOS
 for elapsed, start_time in accurate_timed_loop.accurate_wait(total_wait, loop_delay, fixed_adjustment=adj):
     # ... do task every 250 mS
     pass
 ```
 
 Notes:
 
 * Re-run this several times, and tweak the fixed adjustment.
 * The sample.py reports a "Recommended adj" that usually results in better accuracy.
-* Macos and Ubuntu tend to be less variant than Windows
+* macOS and Ubuntu tend to be less variant than Windows
 
 This report shows that std deviation is much better.
 
 ```text
       expected    elapsed  diff1(ms)  actual(s)  diff2(ms)
   1   0.000000   0.000000      0.000   0.000000      0.000
   2   0.250000   0.251537      1.537   0.251537      1.537
@@ -107,15 +114,15 @@
      sample rc=0
      doit overall rc=0
 ```
 
 Limitations:
 
 * there is NO guarantee that the average error will always be that low or that consistent
-* the following runs were on a Macos
+* the following runs were on a macOS
 
 ```text
 # === first run:
 Stats:
 loop count     : 102 loops
 Error Range    : -9.486 to 4.613 mS
 Error Stddev   :      1.962 mS
```

### Comparing `accurate-timed-loop-0.0.16/sample/main.py` & `accurate_timed_loop-0.0.17/sample/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import datetime
+import math
 import random
 import sys
 import time
-
-import math
 from on_the_fly_stats import OTFStats
 
 import accurate_timed_loop
 
 
 # --------------------
 ## sample run of the loop calculating average timing error
```

### Comparing `accurate-timed-loop-0.0.16/setup.cfg` & `accurate_timed_loop-0.0.17/setup.cfg`

 * *Files identical despite different names*

### Comparing `accurate-timed-loop-0.0.16/setup.py` & `accurate_timed_loop-0.0.17/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from pathlib import Path
 
 from setuptools import find_packages
 from setuptools import setup
 
-print('     setup: version:  v0.0.16')
+print('     setup: version:  v0.0.17')
 print('     setup: module :  accurate_timed_loop')
 
 # @formatter:off
 setup(
     description='Accurate timed loop',
     keywords=['accurate loop', 'utility'],
     install_requires=[
-        'pytest-ver',
+        'medver-pytest',
         'pytest',
         'on_the_fly_stats',
     ],
     classifiers=[
         # Choose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable"
         'Development Status :: 5 - Production/Stable',
         'Environment :: Console',
@@ -26,15 +26,15 @@
     ],
 
     # common attributes from here on
     name='accurate-timed-loop',
     packages=find_packages(include='./accurate_timed_loop*', ),
     include_package_data=True,
     exclude_package_data={'./accurate_timed_loop/lib': ['.gitignore']},
-    version='0.0.16',
+    version='0.0.17',
     license='MIT',
     long_description=(Path(__file__).parent / 'README.md').read_text(),
     long_description_content_type='text/markdown',
     author='JA',
     author_email='cppgent0@gmail.com',
     url='https://bitbucket.org/arrizza-public/accurate-timed-loop/src/master',
     download_url='https://bitbucket.org/arrizza-public/accurate-timed-loop/get/master.zip',
```

### Comparing `accurate-timed-loop-0.0.16/tools/debug_logger.py` & `accurate_timed_loop-0.0.17/tools/xplat_utils/utils_logger.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,134 +1,171 @@
 import sys
 
 
 # -------------------
 ## Holds all info for logging debug lines
-class DebugLogger:
+class UtilsLogger:
     ## flag to log to stdout or not
     verbose = True
+    ## for UT only
+    ut_mode = False
+    ## for UT only
+    ut_lines = []
 
     # --------------------
     ## log a message. Use ok() or err() as appropriate.
     #
     # @param ok      the check state
     # @param msg     the message to print
     # @param prefix  (optional) prefix for each line printed
     # @return None
     @staticmethod
     def check(ok, msg, prefix=None):
         if ok:
-            DebugLogger.ok(msg, prefix)
+            UtilsLogger.ok(msg, prefix)
         else:
-            DebugLogger.err(msg, prefix)
+            UtilsLogger.err(msg, prefix)
 
     # --------------------
     ## log a series of messages. Use ok() or err() as appropriate.
     #
     # @param ok      the check state
     # @param title   the line indicating what the check is about
     # @param msgs    individual list of lines to print
     # @param prefix  (optional) prefix for each line printed
     # @return None
     @staticmethod
     def check_all(ok, title, msgs, prefix=None):
-        DebugLogger.check(ok, f'{title}: {ok}', prefix)
+        UtilsLogger.check(ok, f'{title}: {ok}', prefix)
         for msg in msgs:
-            DebugLogger.check(ok, f'   - {msg}', prefix)
+            UtilsLogger.check(ok, f'   - {msg}', prefix)
 
     # -------------------
     ## write a "====" line with the given message
     #
     # @param msg     the message to write
     # @param prefix  (optional) prefix for each line printed
     # @return None
     @staticmethod
     def start(msg, prefix=None):
-        DebugLogger._write_line('====', msg, prefix)
+        UtilsLogger._write_line('====', msg, prefix)
 
     # -------------------
     ## write a "line" line with the given message
     #
     # @param msg     the message to write
     # @param prefix  (optional) prefix for each line printed
     # @return None
     @staticmethod
     def line(msg, prefix=None):
-        DebugLogger._write_line(' ', msg, prefix)
+        UtilsLogger._write_line(' ', msg, prefix)
+
+    # -------------------
+    ## write a "highlight" line with the given message
+    #
+    # @param msg     the message to write
+    # @param prefix  (optional) prefix for each line printed
+    # @return None
+    @staticmethod
+    def highlight(msg, prefix=None):
+        UtilsLogger._write_line('  ->', msg, prefix)
 
     # -------------------
     ## write a "ok" line with the given message
     #
     # @param msg     the message to write
     # @param prefix  (optional) prefix for each line printed
     # @return None
     @staticmethod
     def ok(msg, prefix=None):
-        DebugLogger._write_line('OK', msg, prefix)
+        UtilsLogger._write_line('OK', msg, prefix)
 
     # -------------------
     ## write a "err" line with the given message
     #
     # @param msg     the message to write
     # @param prefix  (optional) prefix for each line printed
     # @return None
     @staticmethod
     def err(msg, prefix=None):
-        DebugLogger._write_line('ERR', msg, prefix)
+        UtilsLogger._write_line('ERR', msg, prefix)
 
     # -------------------
     ## write a "bug" line with the given message
     #
     # @param msg     the message to write
     # @param prefix  (optional) prefix for each line printed
     # @return None
     @staticmethod
     def bug(msg, prefix=None):
-        DebugLogger._write_line('BUG', msg, prefix)
+        UtilsLogger._write_line('BUG', msg, prefix)
 
     # -------------------
     ## write an output line with the given message
     #
     # @param msg     the message to write
     # @param prefix  (optional) prefix for each line printed
+    # @param lineno  (optional) the current line number for each line printed
     # @return None
     @staticmethod
-    def output(msg, prefix=None):
-        DebugLogger._write_line(' -- ', msg, prefix)
+    def output(msg, prefix=None, lineno=None):
+        if lineno is None:
+            tag = ' --    '
+        else:
+            tag = f' --{lineno: >3}] '
+        UtilsLogger._write_line(tag, msg, prefix)
 
     # -------------------
     ## write a "warn" line with the given message
     #
     # @param msg     the message to write
     # @param prefix  (optional) prefix for each line printed
     # @return None
     @staticmethod
     def warn(msg, prefix=None):
-        DebugLogger._write_line('WARN', msg, prefix)
+        UtilsLogger._write_line('WARN', msg, prefix)
 
     # -------------------
     ## write a "err" line with the given message
     #
     # @param msg     the message to write
     # @param prefix  (optional) prefix for each line printed
     # @return None
     @staticmethod
     def dbg(msg, prefix=None):
-        DebugLogger._write_line('DBG', msg, prefix)
+        UtilsLogger._write_line('DBG', msg, prefix)
+
+    # -------------------
+    ## write a raw line (no tag) with the given message
+    #
+    # @param msg     the message to write
+    # @return None
+    @staticmethod
+    def raw(msg):
+        UtilsLogger._write_line(None, msg)
 
     # -------------------
     ## write the given line to stdout
     #
     # @param tag     the prefix tag
     # @param msg     the message to write
     # @param prefix  (optional) prefix for line
     # @return None
     @staticmethod
     def _write_line(tag, msg, prefix=None):
-        if not DebugLogger.verbose:
+        if not UtilsLogger.verbose:
             return
 
-        if prefix:
-            print(f'{prefix} {tag: <4} {msg}')  # print okay
+        # TODO add ability to optionally save to file
+
+        if tag is None:
+            line = msg
+        elif prefix:
+            line = f'{prefix} {tag: <4} {msg}'
+        else:
+            line = f'{tag: <4} {msg}'
+
+        if UtilsLogger.ut_mode:
+            UtilsLogger.ut_lines.append(line)
         else:
-            print(f'{tag: <4} {msg}')  # print okay
+            print(line)  # print okay
         sys.stdout.flush()
```

### Comparing `accurate-timed-loop-0.0.16/tools/loader.py` & `accurate_timed_loop-0.0.17/tools/loader.py`

 * *Files identical despite different names*

### Comparing `accurate-timed-loop-0.0.16/tools/setup_template.py` & `accurate_timed_loop-0.0.17/tools/setup_template.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 print('     setup: module :  $$mod_dir_name$$')
 
 # @formatter:off
 setup(
     description='Accurate timed loop',
     keywords=['accurate loop', 'utility'],
     install_requires=[
-        'pytest-ver',
+        'medver-pytest',
         'pytest',
         'on_the_fly_stats',
     ],
     classifiers=[
         # Choose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable"
         'Development Status :: 5 - Production/Stable',
         'Environment :: Console',
```

### Comparing `accurate-timed-loop-0.0.16/ver/test_tp001_basic.py` & `accurate_timed_loop-0.0.17/ver/test_tp001_basic.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import datetime
+import math
 import random
 import sys
 import time
 import unittest
-
-import math
 from pytest_ver import pth
 
 from tools import loader
 
 loader.loader_init()
 
 # pylint: disable=wrong-import-order
```

