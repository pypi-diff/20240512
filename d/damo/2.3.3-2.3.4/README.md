# Comparing `tmp/damo-2.3.3.tar.gz` & `tmp/damo-2.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "damo-2.3.3.tar", last modified: Mon Apr 29 19:56:34 2024, max compression
+gzip compressed data, was "damo-2.3.4.tar", last modified: Sun May 12 16:23:41 2024, max compression
```

## Comparing `damo-2.3.3.tar` & `damo-2.3.4.tar`

### file list

```diff
@@ -1,57 +1,56 @@
-drwxr-xr-x   0 sjpark    (1000) sjpark    (1000)        0 2024-04-29 19:56:34.077430 damo-2.3.3/
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     9538 2024-04-29 19:56:34.077430 damo-2.3.3/PKG-INFO
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     9017 2024-04-29 19:56:30.000000 damo-2.3.3/README.md
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)      104 2023-09-30 00:42:34.000000 damo-2.3.3/pyproject.toml
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)       38 2024-04-29 19:56:34.077430 damo-2.3.3/setup.cfg
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1104 2023-09-30 00:42:34.000000 damo-2.3.3/setup.py
-drwxr-xr-x   0 sjpark    (1000) sjpark    (1000)        0 2024-04-29 19:56:34.065430 damo-2.3.3/src/
-drwxr-xr-x   0 sjpark    (1000) sjpark    (1000)        0 2024-04-29 19:56:34.077430 damo-2.3.3/src/damo/
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)        0 2024-04-29 19:56:30.000000 damo-2.3.3/src/damo/__init__.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1442 2023-12-31 19:18:55.000000 damo-2.3.3/src/damo/_damo_ascii_color.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     7357 2023-09-30 00:42:34.000000 damo-2.3.3/src/damo/_damo_deprecated.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)      963 2023-09-30 00:42:34.000000 damo-2.3.3/src/damo/_damo_deprecation_notice.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)      620 2023-09-30 00:42:34.000000 damo-2.3.3/src/damo/_damo_dist.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)    10121 2024-03-03 19:19:45.000000 damo-2.3.3/src/damo/_damo_fmt_str.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     2356 2024-04-18 21:22:30.000000 damo-2.3.3/src/damo/_damo_fs.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     5535 2023-12-31 19:18:55.000000 damo-2.3.3/src/damo/_damo_paddr_layout.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)      522 2023-12-31 18:33:59.000000 damo-2.3.3/src/damo/_damo_print.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)    44940 2024-04-27 18:41:30.000000 damo-2.3.3/src/damo/_damo_records.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)      780 2023-12-31 19:18:55.000000 damo-2.3.3/src/damo/_damo_subcmds.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)    47260 2024-04-27 18:53:46.000000 damo-2.3.3/src/damo/_damon.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)    22388 2024-04-27 19:00:02.000000 damo-2.3.3/src/damo/_damon_args.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)    17432 2024-03-17 18:52:09.000000 damo-2.3.3/src/damo/_damon_dbgfs.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)    28814 2024-03-17 17:58:17.000000 damo-2.3.3/src/damo/_damon_sysfs.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)      256 2024-04-27 18:18:15.000000 damo-2.3.3/src/damo/abc.py
--rwxr-xr-x   0 sjpark    (1000) sjpark    (1000)     4258 2024-04-20 20:06:09.000000 damo-2.3.3/src/damo/damo.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1858 2024-04-06 16:27:42.000000 damo-2.3.3/src/damo/damo_adjust.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1094 2024-04-06 16:27:57.000000 damo-2.3.3/src/damo/damo_convert_record_format.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1309 2024-03-09 21:22:25.000000 damo-2.3.3/src/damo/damo_features.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1144 2024-02-17 20:37:12.000000 damo-2.3.3/src/damo/damo_fmt_json.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)    12165 2024-04-06 16:21:28.000000 damo-2.3.3/src/damo/damo_heats.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     4498 2024-02-17 20:36:55.000000 damo-2.3.3/src/damo/damo_lru_sort.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     2860 2024-02-17 20:37:38.000000 damo-2.3.3/src/damo/damo_monitor.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     2578 2024-04-06 16:21:33.000000 damo-2.3.3/src/damo/damo_nr_regions.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     4472 2024-02-17 20:36:38.000000 damo-2.3.3/src/damo/damo_reclaim.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     5330 2024-04-28 19:08:50.000000 damo-2.3.3/src/damo/damo_record.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     3866 2024-04-06 16:21:42.000000 damo-2.3.3/src/damo/damo_record_info.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     4278 2024-04-06 16:21:46.000000 damo-2.3.3/src/damo/damo_replay.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1587 2024-04-14 17:07:12.000000 damo-2.3.3/src/damo/damo_report.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     4566 2024-04-21 16:55:34.000000 damo-2.3.3/src/damo/damo_report_footprint.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1672 2024-04-06 16:21:52.000000 damo-2.3.3/src/damo/damo_report_profile.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     3886 2024-04-06 16:21:55.000000 damo-2.3.3/src/damo/damo_report_raw.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1493 2024-04-06 16:21:59.000000 damo-2.3.3/src/damo/damo_report_times.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1502 2024-02-17 20:37:22.000000 damo-2.3.3/src/damo/damo_schemes.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)    26317 2024-04-06 16:22:07.000000 damo-2.3.3/src/damo/damo_show.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)      520 2024-02-17 20:35:10.000000 damo-2.3.3/src/damo/damo_start.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     4201 2024-02-17 20:35:59.000000 damo-2.3.3/src/damo/damo_status.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)      567 2024-02-17 20:35:34.000000 damo-2.3.3/src/damo/damo_stop.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)      685 2024-04-14 15:16:45.000000 damo-2.3.3/src/damo/damo_tune.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     3763 2024-04-06 16:22:11.000000 damo-2.3.3/src/damo/damo_validate.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)       22 2024-04-29 19:56:20.000000 damo-2.3.3/src/damo/damo_version.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     6186 2024-04-28 19:04:36.000000 damo-2.3.3/src/damo/damo_wss.py
-drwxr-xr-x   0 sjpark    (1000) sjpark    (1000)        0 2024-04-29 19:56:34.077430 damo-2.3.3/src/damo.egg-info/
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     9538 2024-04-29 19:56:34.000000 damo-2.3.3/src/damo.egg-info/PKG-INFO
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1293 2024-04-29 19:56:34.000000 damo-2.3.3/src/damo.egg-info/SOURCES.txt
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)        1 2024-04-29 19:56:34.000000 damo-2.3.3/src/damo.egg-info/dependency_links.txt
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)       40 2024-04-29 19:56:34.000000 damo-2.3.3/src/damo.egg-info/entry_points.txt
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)        5 2024-04-29 19:56:34.000000 damo-2.3.3/src/damo.egg-info/top_level.txt
+drwxr-xr-x   0 sjpark    (1000) sjpark    (1000)        0 2024-05-12 16:23:41.666266 damo-2.3.4/
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     7492 2024-05-12 16:23:41.666266 damo-2.3.4/PKG-INFO
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     6971 2024-05-12 16:23:38.000000 damo-2.3.4/README.md
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)      104 2023-09-30 00:42:34.000000 damo-2.3.4/pyproject.toml
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)       38 2024-05-12 16:23:41.666266 damo-2.3.4/setup.cfg
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1104 2024-05-11 18:53:35.000000 damo-2.3.4/setup.py
+drwxr-xr-x   0 sjpark    (1000) sjpark    (1000)        0 2024-05-12 16:23:41.654266 damo-2.3.4/src/
+drwxr-xr-x   0 sjpark    (1000) sjpark    (1000)        0 2024-05-12 16:23:41.666266 damo-2.3.4/src/damo/
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)        0 2024-05-12 16:23:38.000000 damo-2.3.4/src/damo/__init__.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1442 2024-05-12 16:21:31.000000 damo-2.3.4/src/damo/_damo_ascii_color.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     7357 2024-05-12 16:21:31.000000 damo-2.3.4/src/damo/_damo_deprecated.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)      963 2024-05-12 16:21:31.000000 damo-2.3.4/src/damo/_damo_deprecation_notice.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)      620 2024-05-12 16:21:31.000000 damo-2.3.4/src/damo/_damo_dist.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)    10121 2024-05-12 16:21:31.000000 damo-2.3.4/src/damo/_damo_fmt_str.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     2356 2024-05-12 16:21:31.000000 damo-2.3.4/src/damo/_damo_fs.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     5535 2024-05-12 16:21:31.000000 damo-2.3.4/src/damo/_damo_paddr_layout.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)      522 2024-05-12 16:21:31.000000 damo-2.3.4/src/damo/_damo_print.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)    44940 2024-05-12 16:21:31.000000 damo-2.3.4/src/damo/_damo_records.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)      780 2024-05-12 16:21:31.000000 damo-2.3.4/src/damo/_damo_subcmds.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)    47260 2024-05-12 16:21:31.000000 damo-2.3.4/src/damo/_damon.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)    22388 2024-05-12 16:21:31.000000 damo-2.3.4/src/damo/_damon_args.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)    17432 2024-05-12 16:21:31.000000 damo-2.3.4/src/damo/_damon_dbgfs.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)    28814 2024-05-12 16:21:31.000000 damo-2.3.4/src/damo/_damon_sysfs.py
+-rwxr-xr-x   0 sjpark    (1000) sjpark    (1000)     4258 2024-05-12 16:21:31.000000 damo-2.3.4/src/damo/damo.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1858 2024-05-12 16:21:31.000000 damo-2.3.4/src/damo/damo_adjust.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1094 2024-05-12 16:21:31.000000 damo-2.3.4/src/damo/damo_convert_record_format.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1309 2024-05-12 16:21:31.000000 damo-2.3.4/src/damo/damo_features.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1144 2024-05-12 16:21:31.000000 damo-2.3.4/src/damo/damo_fmt_json.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)    12165 2024-05-12 16:21:31.000000 damo-2.3.4/src/damo/damo_heats.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     4498 2024-05-12 16:21:31.000000 damo-2.3.4/src/damo/damo_lru_sort.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     2860 2024-05-12 16:21:31.000000 damo-2.3.4/src/damo/damo_monitor.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     2578 2024-05-12 16:21:31.000000 damo-2.3.4/src/damo/damo_nr_regions.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     4472 2024-05-12 16:21:31.000000 damo-2.3.4/src/damo/damo_reclaim.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     5645 2024-05-12 16:21:31.000000 damo-2.3.4/src/damo/damo_record.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     3866 2024-05-12 16:21:31.000000 damo-2.3.4/src/damo/damo_record_info.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     4278 2024-05-12 16:21:31.000000 damo-2.3.4/src/damo/damo_replay.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1587 2024-05-12 16:21:31.000000 damo-2.3.4/src/damo/damo_report.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     4566 2024-05-12 16:21:31.000000 damo-2.3.4/src/damo/damo_report_footprint.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1672 2024-05-12 16:21:31.000000 damo-2.3.4/src/damo/damo_report_profile.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     3886 2024-05-12 16:21:31.000000 damo-2.3.4/src/damo/damo_report_raw.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1493 2024-05-12 16:21:31.000000 damo-2.3.4/src/damo/damo_report_times.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1502 2024-05-12 16:21:31.000000 damo-2.3.4/src/damo/damo_schemes.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)    26317 2024-05-12 16:21:31.000000 damo-2.3.4/src/damo/damo_show.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)      520 2024-05-12 16:21:31.000000 damo-2.3.4/src/damo/damo_start.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     4201 2024-05-12 16:21:31.000000 damo-2.3.4/src/damo/damo_status.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)      567 2024-05-12 16:21:31.000000 damo-2.3.4/src/damo/damo_stop.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)      685 2024-05-12 16:21:31.000000 damo-2.3.4/src/damo/damo_tune.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     3763 2024-05-12 16:21:31.000000 damo-2.3.4/src/damo/damo_validate.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)       22 2024-05-12 16:23:29.000000 damo-2.3.4/src/damo/damo_version.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     6186 2024-05-12 16:21:31.000000 damo-2.3.4/src/damo/damo_wss.py
+drwxr-xr-x   0 sjpark    (1000) sjpark    (1000)        0 2024-05-12 16:23:41.666266 damo-2.3.4/src/damo.egg-info/
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     7492 2024-05-12 16:23:41.000000 damo-2.3.4/src/damo.egg-info/PKG-INFO
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1277 2024-05-12 16:23:41.000000 damo-2.3.4/src/damo.egg-info/SOURCES.txt
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)        1 2024-05-12 16:23:41.000000 damo-2.3.4/src/damo.egg-info/dependency_links.txt
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)       40 2024-05-12 16:23:41.000000 damo-2.3.4/src/damo.egg-info/entry_points.txt
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)        5 2024-05-12 16:23:41.000000 damo-2.3.4/src/damo.egg-info/top_level.txt
```

### Comparing `damo-2.3.3/PKG-INFO` & `damo-2.3.4/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: damo
-Version: 2.3.3
+Version: 2.3.4
 Summary: DAMON user-space tool
 Home-page: https://github.com/awslabs/damo
 Author: SeongJae Park
 Author-email: sj@kernel.org
 Project-URL: Bug Tracker, https://github.com/awslabs/damo/issues
 Project-URL: DAMON, https://damonitor.github.io
 Classifier: Programming Language :: Python :: 3
@@ -40,21 +40,23 @@
 
 Follow below instructions and commands to monitor and visualize the access
 pattern of your workload.
 
     $ # ensure DAMON is enabled on your kernel
     $ # install damo from PyPI, or use your distribution's package manager
     $ sudo pip3 install damo
+    $ sudo damo show $(pidof <your workload>)
     $ sudo damo record $(pidof <your workload>)
     $ sudo damo report heats --heatmap stdout --stdout_heatmap_color emotion
 
-The last command will show the access pattern of your workload, like below:
+The second and last commands will show the access pattern of your workload,
+like below:
 
-![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v2.3.3/images/masim_zigzag_heatmap_ascii.png)
-![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v2.3.3/images/masim_stairs_heatmap_ascii.png)
+![masim_stairs_snapshot](images/masim_stairs_snapshot.png)
+![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v2.3.4/images/masim_stairs_heatmap_ascii.png)
 
 
 FAQs
 ====
 
 How can I ensure DAMON is enabled on my kernel?
 -----------------------------------------------
@@ -62,15 +64,15 @@
 Please refer to 'Install'
 [section](https://sjp38.github.io/post/damon/#install) of the project webpage.
 
 Where can I get more detailed usage?
 ------------------------------------
 
 The below sections provide quick introductions for `damo`'s major features.
-For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v2.3.3/USAGE.md) file.
+For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v2.3.4/USAGE.md) file.
 
 
 What does the version numbers mean?
 -----------------------------------
 
 Nothing at all but indicate which version is more fresh.  A higher version
 number means it is more recently released.
@@ -90,29 +92,38 @@
 How can I participate in the development of `damo`?
 ---------------------------------------------------
 
 Please refer to
 [CONTRIBUTING](https://github.com/awslabs/damo/blob/next/CONTRIBUTING) file.
 
 
-Why some subcommands are not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v2.3.3/USAGE.md) file?
----------------------------------------------------------------------
+Why some features are not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v2.3.4/USAGE.md) file?
+------------------------------------------------------------------
 
-Only sufficiently stabilized features are documented there.  In other words,
-any feature that not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v2.3.3/USAGE.md) are in experimental
-stage.  Such experimental features could be deprecated and removed without any
-notice and grace periods.  The documented features could also be deprecated,
-but those will provide some notification and grace periods.
+Because those are not yet stabilized.  In other words, such features are in
+their experimental stages, and therefore could be deprecated and removed
+without notice and grace periods.  The documented features could also be
+deprecated, but those will provide some notifications and grace periods.  If
+there are some features you're relying on but not documented, please
+[report](REPORTING.md) your usecase to the community.
+
+
+How can I know deprecation schedule and alternatives of specific features?
+--------------------------------------------------------------------------
+
+The list of features that will be, or already deprecated, the deprecation
+schedule, and their alternatives are summarized in
+[FEATURES_DEPRECATION_SCHEDULE.md](FEATURES_DEPRECATION_SCHEDULE.md) file.
 
 
 Quick Intro for Major Features
 ==============================
 
 Below are quick introductions for `damo`'s major features.
-For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v2.3.3/USAGE.md) file.
+For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v2.3.4/USAGE.md) file.
 
 
 Snapshot Data Access Pattern
 ----------------------------
 
 Below commands repeatedly get a snapshot of the access pattern of a program for
 every second.
@@ -181,71 +192,7 @@
 Below command makes every memory region of size >=4K that hasn't accessed for
 >=60 seconds in your workload to be swapped out.  By doing this, you can make
 your workload more memory efficient with only modest performance overhead.
 
     $ sudo damo start --damos_access_rate 0 0 --damos_sz_region 4K max \
                         --damos_age 60s max --damos_action pageout \
                         <pid of your workload>
-
-
-Deprecated, or Will be Deprecated Features
-==========================================
-
-Below are features that recently deprecated, or will be deprecated.  If you
-depend on any of those, please report your usecase to the community via github
-issue, sj@kernel.org, damon@lists.linux.dev, and/or linux-mm@kvack.org.
-
-
-`damo translate_damos`
-----------------------
-
-Deprecated.  Use the command of v2.0.2 or lower version of DAMO instead.
-
-
-DAMON record binary format
---------------------------
-
-Deprecated.  Use `json_compressed` format instead.
-
-At the beginning, DAMO used its special binary format, namely `record`.  It is
-designed for lightweight saving of the monitoring results.  It is difficult to
-read, and not that efficient compared to fancy compression techniques.  `json`
-based monitoring results can be easier to read, and more efficient when
-compression technique is used.  Hence, the format is deprecated.  You may
-use `damo convert_record_format` of v2.0.2 or lower version of DAMO to convert
-your old record binary format monitoring results files to the new format.
-
-
-Python2 support
----------------
-
-Deprecated.  Use Python3.
-
-For some old distros, DAMO initially supported Python2.  Because Python2 is
-really old now, the support has deprecated.  Please use Python3 or newer.
-
-
-DAMOS single line format
-------------------------
-
-Deprecated.  Use `--damos_*` command line options or json format input.
-
-A simple DAMOS scheme specification format called one-line scheme specification
-was initially supported.  Because it is not flexible for extension of features,
-it has deprecated now.  You may use `--damos_*` command line options or json
-format instead.  You could use `damo translate_damos` ov v2.0.2 or lower
-version of DAMO to convert your old single line DAMOS schemes specification to
-the new json format.
-
-
---rbuf option of `damo record`
-------------------------------
-
-Deprecated.
-
-Early versions of DAMON supported in-kernel direct monitoring results record
-file generation.  To control the overhead of it, DAMO allowed user to specify
-the size of buffer for the work.  The feature has not merged into the mainline,
-and discarded.  Hence the option was available for only few kernels that ported
-the feature.  For most of kernels, tracepoint based record file generation is
-being used, and the overhead of the approach is subtle.  Hence, the option has
-deprecated.
```

### Comparing `damo-2.3.3/README.md` & `damo-2.3.4/src/damo.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: damo
+Version: 2.3.4
+Summary: DAMON user-space tool
+Home-page: https://github.com/awslabs/damo
+Author: SeongJae Park
+Author-email: sj@kernel.org
+Project-URL: Bug Tracker, https://github.com/awslabs/damo/issues
+Project-URL: DAMON, https://damonitor.github.io
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
+Classifier: Operating System :: POSIX :: Linux
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+
 DAMO: Data Access Monitoring Operator
 =====================================
 
 `damo` is a user space tool for [DAMON](https://damonitor.github.io).  Using
 this, you can monitor the data access patterns of your system or workloads and
 make data access-aware memory management optimizations.
 
@@ -25,21 +40,23 @@
 
 Follow below instructions and commands to monitor and visualize the access
 pattern of your workload.
 
     $ # ensure DAMON is enabled on your kernel
     $ # install damo from PyPI, or use your distribution's package manager
     $ sudo pip3 install damo
+    $ sudo damo show $(pidof <your workload>)
     $ sudo damo record $(pidof <your workload>)
     $ sudo damo report heats --heatmap stdout --stdout_heatmap_color emotion
 
-The last command will show the access pattern of your workload, like below:
+The second and last commands will show the access pattern of your workload,
+like below:
 
-![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v2.3.3/images/masim_zigzag_heatmap_ascii.png)
-![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v2.3.3/images/masim_stairs_heatmap_ascii.png)
+![masim_stairs_snapshot](images/masim_stairs_snapshot.png)
+![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v2.3.4/images/masim_stairs_heatmap_ascii.png)
 
 
 FAQs
 ====
 
 How can I ensure DAMON is enabled on my kernel?
 -----------------------------------------------
@@ -47,15 +64,15 @@
 Please refer to 'Install'
 [section](https://sjp38.github.io/post/damon/#install) of the project webpage.
 
 Where can I get more detailed usage?
 ------------------------------------
 
 The below sections provide quick introductions for `damo`'s major features.
-For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v2.3.3/USAGE.md) file.
+For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v2.3.4/USAGE.md) file.
 
 
 What does the version numbers mean?
 -----------------------------------
 
 Nothing at all but indicate which version is more fresh.  A higher version
 number means it is more recently released.
@@ -75,29 +92,38 @@
 How can I participate in the development of `damo`?
 ---------------------------------------------------
 
 Please refer to
 [CONTRIBUTING](https://github.com/awslabs/damo/blob/next/CONTRIBUTING) file.
 
 
-Why some subcommands are not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v2.3.3/USAGE.md) file?
----------------------------------------------------------------------
+Why some features are not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v2.3.4/USAGE.md) file?
+------------------------------------------------------------------
 
-Only sufficiently stabilized features are documented there.  In other words,
-any feature that not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v2.3.3/USAGE.md) are in experimental
-stage.  Such experimental features could be deprecated and removed without any
-notice and grace periods.  The documented features could also be deprecated,
-but those will provide some notification and grace periods.
+Because those are not yet stabilized.  In other words, such features are in
+their experimental stages, and therefore could be deprecated and removed
+without notice and grace periods.  The documented features could also be
+deprecated, but those will provide some notifications and grace periods.  If
+there are some features you're relying on but not documented, please
+[report](REPORTING.md) your usecase to the community.
+
+
+How can I know deprecation schedule and alternatives of specific features?
+--------------------------------------------------------------------------
+
+The list of features that will be, or already deprecated, the deprecation
+schedule, and their alternatives are summarized in
+[FEATURES_DEPRECATION_SCHEDULE.md](FEATURES_DEPRECATION_SCHEDULE.md) file.
 
 
 Quick Intro for Major Features
 ==============================
 
 Below are quick introductions for `damo`'s major features.
-For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v2.3.3/USAGE.md) file.
+For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v2.3.4/USAGE.md) file.
 
 
 Snapshot Data Access Pattern
 ----------------------------
 
 Below commands repeatedly get a snapshot of the access pattern of a program for
 every second.
@@ -166,71 +192,7 @@
 Below command makes every memory region of size >=4K that hasn't accessed for
 >=60 seconds in your workload to be swapped out.  By doing this, you can make
 your workload more memory efficient with only modest performance overhead.
 
     $ sudo damo start --damos_access_rate 0 0 --damos_sz_region 4K max \
                         --damos_age 60s max --damos_action pageout \
                         <pid of your workload>
-
-
-Deprecated, or Will be Deprecated Features
-==========================================
-
-Below are features that recently deprecated, or will be deprecated.  If you
-depend on any of those, please report your usecase to the community via github
-issue, sj@kernel.org, damon@lists.linux.dev, and/or linux-mm@kvack.org.
-
-
-`damo translate_damos`
-----------------------
-
-Deprecated.  Use the command of v2.0.2 or lower version of DAMO instead.
-
-
-DAMON record binary format
---------------------------
-
-Deprecated.  Use `json_compressed` format instead.
-
-At the beginning, DAMO used its special binary format, namely `record`.  It is
-designed for lightweight saving of the monitoring results.  It is difficult to
-read, and not that efficient compared to fancy compression techniques.  `json`
-based monitoring results can be easier to read, and more efficient when
-compression technique is used.  Hence, the format is deprecated.  You may
-use `damo convert_record_format` of v2.0.2 or lower version of DAMO to convert
-your old record binary format monitoring results files to the new format.
-
-
-Python2 support
----------------
-
-Deprecated.  Use Python3.
-
-For some old distros, DAMO initially supported Python2.  Because Python2 is
-really old now, the support has deprecated.  Please use Python3 or newer.
-
-
-DAMOS single line format
-------------------------
-
-Deprecated.  Use `--damos_*` command line options or json format input.
-
-A simple DAMOS scheme specification format called one-line scheme specification
-was initially supported.  Because it is not flexible for extension of features,
-it has deprecated now.  You may use `--damos_*` command line options or json
-format instead.  You could use `damo translate_damos` ov v2.0.2 or lower
-version of DAMO to convert your old single line DAMOS schemes specification to
-the new json format.
-
-
---rbuf option of `damo record`
-------------------------------
-
-Deprecated.
-
-Early versions of DAMON supported in-kernel direct monitoring results record
-file generation.  To control the overhead of it, DAMO allowed user to specify
-the size of buffer for the work.  The feature has not merged into the mainline,
-and discarded.  Hence the option was available for only few kernels that ported
-the feature.  For most of kernels, tracepoint based record file generation is
-being used, and the overhead of the approach is subtle.  Hence, the option has
-deprecated.
```

### Comparing `damo-2.3.3/setup.py` & `damo-2.3.4/setup.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.3/src/damo/_damo_ascii_color.py` & `damo-2.3.4/src/damo/_damo_ascii_color.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.3/src/damo/_damo_deprecated.py` & `damo-2.3.4/src/damo/_damo_deprecated.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.3/src/damo/_damo_deprecation_notice.py` & `damo-2.3.4/src/damo/_damo_deprecation_notice.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.3/src/damo/_damo_dist.py` & `damo-2.3.4/src/damo/_damo_dist.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.3/src/damo/_damo_fmt_str.py` & `damo-2.3.4/src/damo/_damo_fmt_str.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.3/src/damo/_damo_fs.py` & `damo-2.3.4/src/damo/_damo_fs.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.3/src/damo/_damo_paddr_layout.py` & `damo-2.3.4/src/damo/_damo_paddr_layout.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.3/src/damo/_damo_print.py` & `damo-2.3.4/src/damo/_damo_print.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.3/src/damo/_damo_records.py` & `damo-2.3.4/src/damo/_damo_records.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.3/src/damo/_damo_subcmds.py` & `damo-2.3.4/src/damo/_damo_subcmds.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.3/src/damo/_damon.py` & `damo-2.3.4/src/damo/_damon.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.3/src/damo/_damon_args.py` & `damo-2.3.4/src/damo/_damon_args.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.3/src/damo/_damon_dbgfs.py` & `damo-2.3.4/src/damo/_damon_dbgfs.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.3/src/damo/_damon_sysfs.py` & `damo-2.3.4/src/damo/_damon_sysfs.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.3/src/damo/damo.py` & `damo-2.3.4/src/damo/damo.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.3/src/damo/damo_adjust.py` & `damo-2.3.4/src/damo/damo_adjust.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.3/src/damo/damo_convert_record_format.py` & `damo-2.3.4/src/damo/damo_convert_record_format.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.3/src/damo/damo_features.py` & `damo-2.3.4/src/damo/damo_features.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.3/src/damo/damo_fmt_json.py` & `damo-2.3.4/src/damo/damo_fmt_json.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.3/src/damo/damo_heats.py` & `damo-2.3.4/src/damo/damo_heats.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.3/src/damo/damo_lru_sort.py` & `damo-2.3.4/src/damo/damo_lru_sort.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.3/src/damo/damo_monitor.py` & `damo-2.3.4/src/damo/damo_monitor.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.3/src/damo/damo_nr_regions.py` & `damo-2.3.4/src/damo/damo_nr_regions.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.3/src/damo/damo_reclaim.py` & `damo-2.3.4/src/damo/damo_reclaim.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.3/src/damo/damo_record.py` & `damo-2.3.4/src/damo/damo_record.py`

 * *Files 3% similar despite different names*

```diff
@@ -139,13 +139,18 @@
     parser.add_argument('--exclude_child_tasks', action='store_false',
                         dest='include_child_tasks',
                         help='do not record access of child processes')
     parser.add_argument('--include_child_tasks', action='store_true',
                         help='record accesses of child processes')
     parser.add_argument('--schemes_target_regions', action='store_true',
                         help='record schemes tried to be applied regions')
+    parser.add_argument('--no_profile', action='store_false', dest='profile',
+                        help='do not record profiling information')
     parser.add_argument('--profile', action='store_true',
                         help='record profiling information together')
+    parser.add_argument('--no_footprint', action='store_false',
+                        dest='footprint',
+                        help='do not record memory footprint')
     parser.add_argument('--footprint', action='store_true',
                         help='record memory footprint')
     parser.description = 'Record monitoring results'
     return parser
```

### Comparing `damo-2.3.3/src/damo/damo_record_info.py` & `damo-2.3.4/src/damo/damo_record_info.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.3/src/damo/damo_replay.py` & `damo-2.3.4/src/damo/damo_replay.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.3/src/damo/damo_report.py` & `damo-2.3.4/src/damo/damo_report.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.3/src/damo/damo_report_footprint.py` & `damo-2.3.4/src/damo/damo_report_footprint.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.3/src/damo/damo_report_profile.py` & `damo-2.3.4/src/damo/damo_report_profile.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.3/src/damo/damo_report_raw.py` & `damo-2.3.4/src/damo/damo_report_raw.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.3/src/damo/damo_report_times.py` & `damo-2.3.4/src/damo/damo_report_times.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.3/src/damo/damo_schemes.py` & `damo-2.3.4/src/damo/damo_schemes.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.3/src/damo/damo_show.py` & `damo-2.3.4/src/damo/damo_show.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.3/src/damo/damo_start.py` & `damo-2.3.4/src/damo/damo_start.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.3/src/damo/damo_status.py` & `damo-2.3.4/src/damo/damo_status.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.3/src/damo/damo_stop.py` & `damo-2.3.4/src/damo/damo_stop.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.3/src/damo/damo_tune.py` & `damo-2.3.4/src/damo/damo_tune.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.3/src/damo/damo_validate.py` & `damo-2.3.4/src/damo/damo_validate.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.3/src/damo/damo_wss.py` & `damo-2.3.4/src/damo/damo_wss.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.3/src/damo.egg-info/SOURCES.txt` & `damo-2.3.4/src/damo.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 src/damo/_damo_print.py
 src/damo/_damo_records.py
 src/damo/_damo_subcmds.py
 src/damo/_damon.py
 src/damo/_damon_args.py
 src/damo/_damon_dbgfs.py
 src/damo/_damon_sysfs.py
-src/damo/abc.py
 src/damo/damo.py
 src/damo/damo_adjust.py
 src/damo/damo_convert_record_format.py
 src/damo/damo_features.py
 src/damo/damo_fmt_json.py
 src/damo/damo_heats.py
 src/damo/damo_lru_sort.py
```

