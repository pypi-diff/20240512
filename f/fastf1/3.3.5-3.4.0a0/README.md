# Comparing `tmp/fastf1-3.3.5.tar.gz` & `tmp/fastf1-3.4.0a0.tar.gz`

## Comparing `fastf1-3.3.5.tar` & `fastf1-3.4.0a0.tar`

### file list

```diff
@@ -1,62 +1,76 @@
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 fastf1-3.3.5/examples/README.rst
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 fastf1-3.3.5/examples/example_fastf1_signalrclient.py
--rw-r--r--   0        0        0     4020 2020-02-02 00:00:00.000000 fastf1-3.3.5/examples/plot_annotate_corners.py
--rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 fastf1-3.3.5/examples/plot_annotate_speed_trace.py
--rwxr-xr-x   0        0        0     2014 2020-02-02 00:00:00.000000 fastf1-3.3.5/examples/plot_driver_laptimes.py
--rw-r--r--   0        0        0     2132 2020-02-02 00:00:00.000000 fastf1-3.3.5/examples/plot_gear_shifts_on_track.py
--rwxr-xr-x   0        0        0     3163 2020-02-02 00:00:00.000000 fastf1-3.3.5/examples/plot_laptimes_distribution.py
--rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 fastf1-3.3.5/examples/plot_position_changes.py
--rw-r--r--   0        0        0     3157 2020-02-02 00:00:00.000000 fastf1-3.3.5/examples/plot_qualifying_results.py
--rw-r--r--   0        0        0     3716 2020-02-02 00:00:00.000000 fastf1-3.3.5/examples/plot_results_tracker.py
--rw-r--r--   0        0        0     2793 2020-02-02 00:00:00.000000 fastf1-3.3.5/examples/plot_speed_on_track.py
--rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 fastf1-3.3.5/examples/plot_speed_traces.py
--rw-r--r--   0        0        0     2878 2020-02-02 00:00:00.000000 fastf1-3.3.5/examples/plot_strategy.py
--rwxr-xr-x   0        0        0     2053 2020-02-02 00:00:00.000000 fastf1-3.3.5/examples/plot_team_pace_ranking.py
--rw-r--r--   0        0        0     3524 2020-02-02 00:00:00.000000 fastf1-3.3.5/examples/plot_who_can_still_win_wdc.py
--rw-r--r--   0        0        0     5356 2020-02-02 00:00:00.000000 fastf1-3.3.5/fastf1/__init__.py
--rw-r--r--   0        0        0    74642 2020-02-02 00:00:00.000000 fastf1-3.3.5/fastf1/_api.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 fastf1-3.3.5/fastf1/_version.py
--rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 fastf1-3.3.5/fastf1/api.py
--rw-r--r--   0        0        0   154780 2020-02-02 00:00:00.000000 fastf1-3.3.5/fastf1/core.py
--rw-r--r--   0        0        0    41549 2020-02-02 00:00:00.000000 fastf1-3.3.5/fastf1/events.py
--rw-r--r--   0        0        0    10591 2020-02-02 00:00:00.000000 fastf1-3.3.5/fastf1/legacy.py
--rw-r--r--   0        0        0     5508 2020-02-02 00:00:00.000000 fastf1-3.3.5/fastf1/logger.py
--rw-r--r--   0        0        0    16355 2020-02-02 00:00:00.000000 fastf1-3.3.5/fastf1/plotting.py
--rw-r--r--   0        0        0    26173 2020-02-02 00:00:00.000000 fastf1-3.3.5/fastf1/req.py
--rw-r--r--   0        0        0     7583 2020-02-02 00:00:00.000000 fastf1-3.3.5/fastf1/utils.py
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 fastf1-3.3.5/fastf1/ergast/__init__.py
--rw-r--r--   0        0        0    61561 2020-02-02 00:00:00.000000 fastf1-3.3.5/fastf1/ergast/interface.py
--rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 fastf1-3.3.5/fastf1/ergast/legacy.py
--rw-r--r--   0        0        0     7548 2020-02-02 00:00:00.000000 fastf1-3.3.5/fastf1/ergast/sphinx.py
--rw-r--r--   0        0        0    18692 2020-02-02 00:00:00.000000 fastf1-3.3.5/fastf1/ergast/structure.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 fastf1-3.3.5/fastf1/internals/__init__.py
--rw-r--r--   0        0        0     5717 2020-02-02 00:00:00.000000 fastf1-3.3.5/fastf1/internals/pandas_base.py
--rw-r--r--   0        0        0     3788 2020-02-02 00:00:00.000000 fastf1-3.3.5/fastf1/internals/pandas_extensions.py
--rw-r--r--   0        0        0     5294 2020-02-02 00:00:00.000000 fastf1-3.3.5/fastf1/livetiming/__init__.py
--rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 fastf1-3.3.5/fastf1/livetiming/__main__.py
--rw-r--r--   0        0        0     7159 2020-02-02 00:00:00.000000 fastf1-3.3.5/fastf1/livetiming/client.py
--rw-r--r--   0        0        0    10489 2020-02-02 00:00:00.000000 fastf1-3.3.5/fastf1/livetiming/data.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 fastf1-3.3.5/fastf1/mvapi/__init__.py
--rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 fastf1-3.3.5/fastf1/mvapi/api.py
--rw-r--r--   0        0        0     5891 2020-02-02 00:00:00.000000 fastf1-3.3.5/fastf1/mvapi/data.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 fastf1-3.3.5/fastf1/mvapi/internals.py
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 fastf1-3.3.5/fastf1/signalr_aio/LICENSE
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 fastf1-3.3.5/fastf1/signalr_aio/README.md
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 fastf1-3.3.5/fastf1/signalr_aio/__init__.py
--rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 fastf1-3.3.5/fastf1/signalr_aio/_connection.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 fastf1-3.3.5/fastf1/signalr_aio/events/__init__.py
--rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 fastf1-3.3.5/fastf1/signalr_aio/events/_events.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 fastf1-3.3.5/fastf1/signalr_aio/hubs/__init__.py
--rw-r--r--   0        0        0     1458 2020-02-02 00:00:00.000000 fastf1-3.3.5/fastf1/signalr_aio/hubs/_hub.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 fastf1-3.3.5/fastf1/signalr_aio/transports/__init__.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 fastf1-3.3.5/fastf1/signalr_aio/transports/_exceptions.py
--rw-r--r--   0        0        0     2298 2020-02-02 00:00:00.000000 fastf1-3.3.5/fastf1/signalr_aio/transports/_parameters.py
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 fastf1-3.3.5/fastf1/signalr_aio/transports/_queue_events.py
--rw-r--r--   0        0        0     3588 2020-02-02 00:00:00.000000 fastf1-3.3.5/fastf1/signalr_aio/transports/_transport.py
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 fastf1-3.3.5/requirements/dev.txt
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 fastf1-3.3.5/requirements/minver.txt
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 fastf1-3.3.5/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 fastf1-3.3.5/LICENSE
--rw-r--r--   0        0        0     1995 2020-02-02 00:00:00.000000 fastf1-3.3.5/README.md
--rw-r--r--   0        0        0     2047 2020-02-02 00:00:00.000000 fastf1-3.3.5/pyproject.toml
--rw-r--r--   0        0        0     3986 2020-02-02 00:00:00.000000 fastf1-3.3.5/PKG-INFO
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/examples/README.rst
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/examples/example_fastf1_signalrclient.py
+-rw-r--r--   0        0        0     4020 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/examples/plot_annotate_corners.py
+-rw-r--r--   0        0        0     2475 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/examples/plot_annotate_speed_trace.py
+-rwxr-xr-x   0        0        0     2135 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/examples/plot_driver_laptimes.py
+-rw-r--r--   0        0        0     3890 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/examples/plot_driver_styling.py
+-rw-r--r--   0        0        0     2132 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/examples/plot_gear_shifts_on_track.py
+-rwxr-xr-x   0        0        0     2837 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/examples/plot_laptimes_distribution.py
+-rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/examples/plot_position_changes.py
+-rw-r--r--   0        0        0     3177 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/examples/plot_qualifying_results.py
+-rw-r--r--   0        0        0     3716 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/examples/plot_results_tracker.py
+-rw-r--r--   0        0        0     2793 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/examples/plot_speed_on_track.py
+-rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/examples/plot_speed_traces.py
+-rw-r--r--   0        0        0     2998 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/examples/plot_strategy.py
+-rwxr-xr-x   0        0        0     2091 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/examples/plot_team_pace_ranking.py
+-rw-r--r--   0        0        0     3486 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/examples/plot_who_can_still_win_wdc.py
+-rw-r--r--   0        0        0     5356 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/fastf1/__init__.py
+-rw-r--r--   0        0        0    74642 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/fastf1/_api.py
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/fastf1/_version.py
+-rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/fastf1/api.py
+-rw-r--r--   0        0        0   154357 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/fastf1/core.py
+-rw-r--r--   0        0        0    43127 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/fastf1/events.py
+-rw-r--r--   0        0        0    10633 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/fastf1/legacy.py
+-rw-r--r--   0        0        0     5508 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/fastf1/logger.py
+-rw-r--r--   0        0        0    26173 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/fastf1/req.py
+-rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/fastf1/utils.py
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/fastf1/ergast/__init__.py
+-rw-r--r--   0        0        0    61561 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/fastf1/ergast/interface.py
+-rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/fastf1/ergast/legacy.py
+-rw-r--r--   0        0        0     7548 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/fastf1/ergast/sphinx.py
+-rw-r--r--   0        0        0    18692 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/fastf1/ergast/structure.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/fastf1/internals/__init__.py
+-rw-r--r--   0        0        0     5717 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/fastf1/internals/pandas_base.py
+-rw-r--r--   0        0        0     3788 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/fastf1/internals/pandas_extensions.py
+-rw-r--r--   0        0        0     5294 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/fastf1/livetiming/__init__.py
+-rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/fastf1/livetiming/__main__.py
+-rw-r--r--   0        0        0     7159 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/fastf1/livetiming/client.py
+-rw-r--r--   0        0        0    10468 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/fastf1/livetiming/data.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/fastf1/mvapi/__init__.py
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/fastf1/mvapi/api.py
+-rw-r--r--   0        0        0     5891 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/fastf1/mvapi/data.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/fastf1/mvapi/internals.py
+-rw-r--r--   0        0        0     4907 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/fastf1/plotting/__init__.py
+-rw-r--r--   0        0        0     2154 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/fastf1/plotting/_backend.py
+-rw-r--r--   0        0        0     2312 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/fastf1/plotting/_base.py
+-rw-r--r--   0        0        0    22757 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/fastf1/plotting/_interface.py
+-rw-r--r--   0        0        0    14085 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/fastf1/plotting/_plotting.py
+-rw-r--r--   0        0        0     3156 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/fastf1/plotting/_constants/__init__.py
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/fastf1/plotting/_constants/base.py
+-rw-r--r--   0        0        0     2337 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/fastf1/plotting/_constants/season2018.py
+-rw-r--r--   0        0        0     2034 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/fastf1/plotting/_constants/season2019.py
+-rw-r--r--   0        0        0     2034 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/fastf1/plotting/_constants/season2020.py
+-rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/fastf1/plotting/_constants/season2021.py
+-rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/fastf1/plotting/_constants/season2022.py
+-rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/fastf1/plotting/_constants/season2023.py
+-rw-r--r--   0        0        0     2033 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/fastf1/plotting/_constants/season2024.py
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/fastf1/signalr_aio/LICENSE
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/fastf1/signalr_aio/README.md
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/fastf1/signalr_aio/__init__.py
+-rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/fastf1/signalr_aio/_connection.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/fastf1/signalr_aio/events/__init__.py
+-rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/fastf1/signalr_aio/events/_events.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/fastf1/signalr_aio/hubs/__init__.py
+-rw-r--r--   0        0        0     1458 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/fastf1/signalr_aio/hubs/_hub.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/fastf1/signalr_aio/transports/__init__.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/fastf1/signalr_aio/transports/_exceptions.py
+-rw-r--r--   0        0        0     2298 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/fastf1/signalr_aio/transports/_parameters.py
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/fastf1/signalr_aio/transports/_queue_events.py
+-rw-r--r--   0        0        0     3588 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/fastf1/signalr_aio/transports/_transport.py
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/requirements/dev.txt
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/requirements/minver.txt
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/LICENSE
+-rw-r--r--   0        0        0     1995 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/README.md
+-rw-r--r--   0        0        0     2049 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/pyproject.toml
+-rw-r--r--   0        0        0     3990 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/PKG-INFO
```

### Comparing `fastf1-3.3.5/examples/plot_annotate_corners.py` & `fastf1-3.4.0a0/examples/plot_annotate_corners.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.5/examples/plot_annotate_speed_trace.py` & `fastf1-3.4.0a0/examples/plot_annotate_speed_trace.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,17 +6,18 @@
 
 
 import matplotlib.pyplot as plt
 
 import fastf1.plotting
 
 
-# enable some matplotlib patches for plotting timedelta values and load
-# FastF1's default color scheme
-fastf1.plotting.setup_mpl(misc_mpl_mods=False)
+# Enable Matplotlib patches for plotting timedelta values and load
+# FastF1's dark color scheme
+fastf1.plotting.setup_mpl(mpl_timedelta_support=True, misc_mpl_mods=False,
+                          color_scheme='fastf1')
 
 # load a session and its telemetry data
 session = fastf1.get_session(2021, 'Spanish Grand Prix', 'Q')
 session.load()
 
 ##############################################################################
 # First, we select the fastest lap and get the car telemetry data for this
@@ -31,15 +32,16 @@
 
 circuit_info = session.get_circuit_info()
 
 ##############################################################################
 # Finally, we create a plot and plot the speed trace as well as the corner
 # markers.
 
-team_color = fastf1.plotting.team_color(fastest_lap['Team'])
+team_color = fastf1.plotting.get_team_color(fastest_lap['Team'],
+                                            session=session)
 
 fig, ax = plt.subplots()
 ax.plot(car_data['Distance'], car_data['Speed'],
         color=team_color, label=fastest_lap['Driver'])
 
 # Draw vertical dotted lines at each corner that range from slightly below the
 # minimum speed to slightly above the maximum speed.
```

### Comparing `fastf1-3.3.5/examples/plot_driver_laptimes.py` & `fastf1-3.4.0a0/examples/plot_driver_laptimes.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,16 +7,19 @@
 import seaborn as sns
 from matplotlib import pyplot as plt
 
 import fastf1
 import fastf1.plotting
 
 
-# The misc_mpl_mods option enables minor grid lines which clutter the plot
-fastf1.plotting.setup_mpl(misc_mpl_mods=False)
+# Enable Matplotlib patches for plotting timedelta values and load
+# FastF1's dark color scheme
+fastf1.plotting.setup_mpl(mpl_timedelta_support=True, misc_mpl_mods=False,
+                          color_scheme='fastf1')
+
 
 ###############################################################################
 # Load the race session.
 
 race = fastf1.get_session(2023, "Azerbaijan", 'R')
 race.load()
 
@@ -35,15 +38,15 @@
 fig, ax = plt.subplots(figsize=(8, 8))
 
 sns.scatterplot(data=driver_laps,
                 x="LapNumber",
                 y="LapTime",
                 ax=ax,
                 hue="Compound",
-                palette=fastf1.plotting.COMPOUND_COLORS,
+                palette=fastf1.plotting.get_compound_mapping(session=race),
                 s=80,
                 linewidth=0,
                 legend='auto')
 # sphinx_gallery_defer_figures
 
 ###############################################################################
 # Make the plot more aesthetic.
```

### Comparing `fastf1-3.3.5/examples/plot_gear_shifts_on_track.py` & `fastf1-3.4.0a0/examples/plot_gear_shifts_on_track.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.5/examples/plot_laptimes_distribution.py` & `fastf1-3.4.0a0/examples/plot_laptimes_distribution.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,16 +6,19 @@
 import seaborn as sns
 from matplotlib import pyplot as plt
 
 import fastf1
 import fastf1.plotting
 
 
-# enabling misc_mpl_mods will turn on minor grid lines that clutters the plot
-fastf1.plotting.setup_mpl(mpl_timedelta_support=False, misc_mpl_mods=False)
+# Enable Matplotlib patches for plotting timedelta values and load
+# FastF1's dark color scheme
+fastf1.plotting.setup_mpl(mpl_timedelta_support=True, misc_mpl_mods=False,
+                          color_scheme='fastf1')
+
 
 ###############################################################################
 # Load the race session
 
 race = fastf1.get_session(2023, "Azerbaijan", 'R')
 race.load()
 
@@ -31,49 +34,40 @@
 ###############################################################################
 # To plot the drivers by finishing order,
 # we need to get their three-letter abbreviations in the finishing order.
 finishing_order = [race.get_driver(i)["Abbreviation"] for i in point_finishers]
 print(finishing_order)
 
 ###############################################################################
-# We need to modify the DRIVER_COLORS palette.
-# Its keys are the driver's full names but we need the keys to be the drivers'
-# three-letter abbreviations.
-# We can do this with the DRIVER_TRANSLATE mapping.
-driver_colors = {abv: fastf1.plotting.DRIVER_COLORS[driver] for abv,
-                 driver in fastf1.plotting.DRIVER_TRANSLATE.items()}
-print(driver_colors)
-
-###############################################################################
 # First create the violin plots to show the distributions.
 # Then use the swarm plot to show the actual laptimes.
 
 # create the figure
 fig, ax = plt.subplots(figsize=(10, 5))
 
-# Seaborn doesn't have proper timedelta support
+# Seaborn doesn't have proper timedelta support,
 # so we have to convert timedelta to float (in seconds)
 driver_laps["LapTime(s)"] = driver_laps["LapTime"].dt.total_seconds()
 
 sns.violinplot(data=driver_laps,
                x="Driver",
                y="LapTime(s)",
                hue="Driver",
                inner=None,
                density_norm="area",
                order=finishing_order,
-               palette=driver_colors
+               palette=fastf1.plotting.get_driver_color_mapping(session=race)
                )
 
 sns.swarmplot(data=driver_laps,
               x="Driver",
               y="LapTime(s)",
               order=finishing_order,
               hue="Compound",
-              palette=fastf1.plotting.COMPOUND_COLORS,
+              palette=fastf1.plotting.get_compound_mapping(session=race),
               hue_order=["SOFT", "MEDIUM", "HARD"],
               linewidth=0,
               size=4,
               )
 # sphinx_gallery_defer_figures
 
 ###############################################################################
```

### Comparing `fastf1-3.3.5/examples/plot_position_changes.py` & `fastf1-3.4.0a0/examples/plot_position_changes.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,18 @@
 """
 
 import matplotlib.pyplot as plt
 
 import fastf1.plotting
 
 
-fastf1.plotting.setup_mpl(misc_mpl_mods=False)
+# Load FastF1's dark color scheme
+fastf1.plotting.setup_mpl(mpl_timedelta_support=False, misc_mpl_mods=False,
+                          color_scheme='fastf1')
+
 
 ##############################################################################
 # Load the session and create the plot
 session = fastf1.get_session(2023, 1, 'R')
 session.load(telemetry=False, weather=False)
 
 fig, ax = plt.subplots(figsize=(8.0, 4.9))
@@ -24,18 +27,20 @@
 # For each driver, get their three letter abbreviation (e.g. 'HAM') by simply
 # using the value of the first lap, get their color and then plot their
 # position over the number of laps.
 for drv in session.drivers:
     drv_laps = session.laps.pick_driver(drv)
 
     abb = drv_laps['Driver'].iloc[0]
-    color = fastf1.plotting.driver_color(abb)
+    style = fastf1.plotting.get_driver_style(identifier=abb,
+                                             style=['color', 'linestyle'],
+                                             session=session)
 
     ax.plot(drv_laps['LapNumber'], drv_laps['Position'],
-            label=abb, color=color)
+            label=abb, **style)
 # sphinx_gallery_defer_figures
 
 ##############################################################################
 # Finalize the plot by setting y-limits that invert the y-axis so that position
 # one is at the top, set custom tick positions and axis labels.
 ax.set_ylim([20.5, 0.5])
 ax.set_yticks([1, 5, 10, 15, 20])
```

### Comparing `fastf1-3.3.5/examples/plot_qualifying_results.py` & `fastf1-3.4.0a0/examples/plot_qualifying_results.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,46 +10,47 @@
 from timple.timedelta import strftimedelta
 
 import fastf1
 import fastf1.plotting
 from fastf1.core import Laps
 
 
-# we only want support for timedelta plotting in this example
-fastf1.plotting.setup_mpl(mpl_timedelta_support=True, color_scheme=None,
-                          misc_mpl_mods=False)
+# Enable Matplotlib patches for plotting timedelta values
+fastf1.plotting.setup_mpl(mpl_timedelta_support=True, misc_mpl_mods=False,
+                          color_scheme=None)
+
 
 session = fastf1.get_session(2021, 'Spanish Grand Prix', 'Q')
 session.load()
 
 
 ##############################################################################
 # First, we need to get an array of all drivers.
 
 drivers = pd.unique(session.laps['Driver'])
 print(drivers)
 
 
 ##############################################################################
-# After that we'll get each drivers fastest lap, create a new laps object
+# After that we'll get each driver's fastest lap, create a new laps object
 # from these laps, sort them by lap time and have pandas reindex them to
 # number them nicely by starting position.
 
 list_fastest_laps = list()
 for drv in drivers:
     drvs_fastest_lap = session.laps.pick_driver(drv).pick_fastest()
     list_fastest_laps.append(drvs_fastest_lap)
 fastest_laps = Laps(list_fastest_laps) \
     .sort_values(by='LapTime') \
     .reset_index(drop=True)
 
 
 ##############################################################################
 # The plot is nicer to look at and more easily understandable if we just plot
-# the time differences. Therefore we subtract the fastest lap time from all
+# the time differences. Therefore, we subtract the fastest lap time from all
 # other lap times.
 
 pole_lap = fastest_laps.pick_fastest()
 fastest_laps['LapTimeDelta'] = fastest_laps['LapTime'] - pole_lap['LapTime']
 
 
 ##############################################################################
@@ -60,15 +61,15 @@
 print(fastest_laps[['Driver', 'LapTime', 'LapTimeDelta']])
 
 
 ##############################################################################
 # Finally, we'll create a list of team colors per lap to color our plot.
 team_colors = list()
 for index, lap in fastest_laps.iterlaps():
-    color = fastf1.plotting.team_color(lap['Team'])
+    color = fastf1.plotting.get_team_color(lap['Team'], session=session)
     team_colors.append(color)
 
 
 ##############################################################################
 # Now, we can plot all the data
 fig, ax = plt.subplots()
 ax.barh(fastest_laps.index, fastest_laps['LapTimeDelta'],
```

### Comparing `fastf1-3.3.5/examples/plot_results_tracker.py` & `fastf1-3.4.0a0/examples/plot_results_tracker.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.5/examples/plot_speed_on_track.py` & `fastf1-3.4.0a0/examples/plot_speed_on_track.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.5/examples/plot_speed_traces.py` & `fastf1-3.4.0a0/examples/plot_speed_traces.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,17 +6,18 @@
 
 
 import matplotlib.pyplot as plt
 
 import fastf1.plotting
 
 
-# enable some matplotlib patches for plotting timedelta values and load
-# FastF1's default color scheme
-fastf1.plotting.setup_mpl(misc_mpl_mods=False)
+# Enable Matplotlib patches for plotting timedelta values and load
+# FastF1's dark color scheme
+fastf1.plotting.setup_mpl(mpl_timedelta_support=True, misc_mpl_mods=False,
+                          color_scheme='fastf1')
 
 # load a session and its telemetry data
 session = fastf1.get_session(2021, 'Spanish Grand Prix', 'Q')
 session.load()
 
 ##############################################################################
 # First, we select the two laps that we want to compare
@@ -31,16 +32,16 @@
 ver_tel = ver_lap.get_car_data().add_distance()
 ham_tel = ham_lap.get_car_data().add_distance()
 
 ##############################################################################
 # Finally, we create a plot and plot both speed traces.
 # We color the individual lines with the driver's team colors.
 
-rbr_color = fastf1.plotting.team_color('RBR')
-mer_color = fastf1.plotting.team_color('MER')
+rbr_color = fastf1.plotting.get_team_color(ver_lap['Team'], session=session)
+mer_color = fastf1.plotting.get_team_color(ham_lap['Team'], session=session)
 
 fig, ax = plt.subplots()
 ax.plot(ver_tel['Distance'], ver_tel['Speed'], color=rbr_color, label='VER')
 ax.plot(ham_tel['Distance'], ham_tel['Speed'], color=mer_color, label='HAM')
 
 ax.set_xlabel('Distance in m')
 ax.set_ylabel('Speed in km/h')
```

### Comparing `fastf1-3.3.5/examples/plot_strategy.py` & `fastf1-3.4.0a0/examples/plot_strategy.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,19 +51,21 @@
 for driver in drivers:
     driver_stints = stints.loc[stints["Driver"] == driver]
 
     previous_stint_end = 0
     for idx, row in driver_stints.iterrows():
         # each row contains the compound name and stint length
         # we can use these information to draw horizontal bars
+        compound_color = fastf1.plotting.get_compound_color(row["Compound"],
+                                                            session=session)
         plt.barh(
             y=driver,
             width=row["StintLength"],
             left=previous_stint_end,
-            color=fastf1.plotting.COMPOUND_COLORS[row["Compound"]],
+            color=compound_color,
             edgecolor="black",
             fill=True
         )
 
         previous_stint_end += row["StintLength"]
 
 # sphinx_gallery_defer_figures
```

### Comparing `fastf1-3.3.5/examples/plot_team_pace_ranking.py` & `fastf1-3.4.0a0/examples/plot_team_pace_ranking.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,22 +6,24 @@
 import seaborn as sns
 from matplotlib import pyplot as plt
 
 import fastf1
 import fastf1.plotting
 
 
-# activate the fastf1 color scheme (and no other modifications)
-fastf1.plotting.setup_mpl(mpl_timedelta_support=False, misc_mpl_mods=False)
+# Load FastF1's dark color scheme
+fastf1.plotting.setup_mpl(mpl_timedelta_support=False, misc_mpl_mods=False,
+                          color_scheme='fastf1')
+
 
 ###############################################################################
 # Load the race session.
 # Pick all quick laps (within 107% of fastest lap).
 # For races with mixed conditions, pick_wo_box() is better.
-race = fastf1.get_session(2023, "British Grand Prix", 'R')
+race = fastf1.get_session(2024, 1, 'R')
 race.load()
 laps = race.laps.pick_quicklaps()
 
 ###############################################################################
 # Convert the lap time column from timedelta to integer.
 # This is a seaborn-specific modification.
 # If plotting with matplotlib, set mpl_timedelta_support to true
@@ -36,15 +38,16 @@
     .median()["LapTime (s)"]
     .sort_values()
     .index
 )
 print(team_order)
 
 # make a color palette associating team names to hex codes
-team_palette = {team: fastf1.plotting.team_color(team) for team in team_order}
+team_palette = {team: fastf1.plotting.get_team_color(team, session=race)
+                for team in team_order}
 
 ###############################################################################
 fig, ax = plt.subplots(figsize=(15, 10))
 sns.boxplot(
     data=transformed_laps,
     x="Team",
     y="LapTime (s)",
```

### Comparing `fastf1-3.3.5/examples/plot_who_can_still_win_wdc.py` & `fastf1-3.4.0a0/examples/plot_who_can_still_win_wdc.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 SEASON = 2023
 ROUND = 15
 
 
 ##############################################################################
 # Get the current driver standings from Ergast.
-# Reference https://theoehrly.github.io/Fast-F1-Pre-Release-Documentation/ergast.html#fastf1.ergast.Ergast.get_driver_standings
+# Reference https://docs.fastf1.dev/ergast.html#fastf1.ergast.Ergast.get_driver_standings
 def get_drivers_standings():
     ergast = Ergast()
     standings = ergast.get_driver_standings(season=SEASON, round=ROUND)
     return standings.content[0]
 
 
 ##############################################################################
```

### Comparing `fastf1-3.3.5/fastf1/__init__.py` & `fastf1-3.4.0a0/fastf1/__init__.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.5/fastf1/_api.py` & `fastf1-3.4.0a0/fastf1/_api.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.5/fastf1/api.py` & `fastf1-3.4.0a0/fastf1/api.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.5/fastf1/core.py` & `fastf1-3.4.0a0/fastf1/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,26 +75,14 @@
     get_circuit_info
 )
 from fastf1.utils import to_timedelta
 
 
 _logger = get_logger(__name__)
 
-D_LOOKUP: List[List] = \
-    [[44, 'HAM', 'Mercedes'], [77, 'BOT', 'Mercedes'],
-     [55, 'SAI', 'Ferrari'], [16, 'LEC', 'Ferrari'],
-     [33, 'VER', 'Red Bull'], [11, 'PER', 'Red Bull'],
-     [3, 'RIC', 'McLaren'], [4, 'NOR', 'McLaren'],
-     [5, 'VET', 'Aston Martin'], [18, 'STR', 'Aston Martin'],
-     [14, 'ALO', 'Alpine'], [31, 'OCO', 'Alpine'],
-     [22, 'TSU', 'AlphaTauri'], [10, 'GAS', 'AlphaTauri'],
-     [47, 'MSC', 'Haas F1 Team'], [9, 'MAZ', 'Haas F1 Team'],
-     [7, 'RAI', 'Alfa Romeo'], [99, 'GIO', 'Alfa Romeo'],
-     [6, 'LAT', 'Williams'], [63, 'RUS', 'Williams']]
-
 
 class Telemetry(pd.DataFrame):
     """Multi-channel time series telemetry data
 
     The object can contain multiple telemetry channels. Multiple telemetry
     objects with different channels can be merged on time. Each telemetry
     channel is one dataframe column. Partial telemetry (e.g. for one lap only)
@@ -317,29 +305,29 @@
             pad_side: Where to pad the data; possible options:
                 'both', 'before', 'after
             interpolate_edges: Add an interpolated sample at the beginning
                 and end to exactly match the provided time window.
         """
         if isinstance(ref_laps, Laps) and len(ref_laps) > 1:
             if 'DriverNumber' not in ref_laps.columns:
-                ValueError("Laps is missing 'DriverNumber'. Cannot return "
-                           "telemetry for unknown driver.")
+                raise ValueError("Laps is missing 'DriverNumber'. "
+                           "Cannot return telemetry for unknown driver.")
             if not len(ref_laps['DriverNumber'].unique()) <= 1:
                 raise ValueError("Cannot create telemetry for multiple "
                                  "drivers at once!")
 
             end_time = ref_laps['Time'].max()
             start_time = ref_laps['LapStartTime'].min()
 
         elif isinstance(ref_laps, (Lap, Laps)):
             if isinstance(ref_laps, Laps):  # one lap in Laps
                 ref_laps = ref_laps.iloc[0]  # handle as a single lap
             if 'DriverNumber' not in ref_laps.index:
-                ValueError("Lap is missing 'DriverNumber'. Cannot return "
-                           "telemetry for unknown driver.")
+                raise ValueError("Lap is missing 'DriverNumber'. "
+                           "Cannot return telemetry for unknown driver.")
             end_time = ref_laps['Time']
             start_time = ref_laps['LapStartTime']
 
         else:
             raise TypeError("Attribute 'ref_laps' needs to be an instance of "
                             "`Lap` or `Laps`")
 
@@ -455,15 +443,15 @@
         # save dtypes before merging, so they can be restored after merging
         # necessary for example because merging produces NaN values which
         # would cause an int column to become float, but it can be converted
         # back to int after interpolating missing values
         dtype_map = dict()
         for df in data, other:
             for col in df.columns:
-                if col not in dtype_map.keys():
+                if col not in dtype_map:
                     dtype_map[col] = df[col].dtype
 
         # Exclude columns existing on both dataframes from one dataframe
         # before merging (cannot merge with duplicates)
         on_both_columns = set(other.columns).intersection(set(data.columns))
         merged = other.merge(
             data[data.columns.difference(on_both_columns, sort=False)],
@@ -497,15 +485,15 @@
             merged = merged.reset_index().rename(columns={'index': 'Date'})
 
         else:
             frq = pd.Timedelta(seconds=1/frequency)
 
             resampled_columns = dict()
 
-            for ch in self._CHANNELS.keys():
+            for ch in self._CHANNELS:
                 if ch not in merged.columns:
                     continue
                 sig_type = self._CHANNELS[ch]['type']
 
                 if sig_type == 'continuous':
                     method = self._CHANNELS[ch]['method']
                     if method in ('nearest', 'zero', 'slinear', 'quadratic',
@@ -562,15 +550,15 @@
             # recalculate the time columns
             merged['SessionTime'] \
                 = merged['Date'] - self.session.t0_date
             merged['Time'] \
                 = merged['SessionTime'] - merged['SessionTime'].iloc[0]
 
         # restore data types from before merging
-        for col in dtype_map.keys():
+        for col in dtype_map:
             try:
                 merged[col] = merged.loc[:, col].astype(dtype_map[col])
             except ValueError:
                 _logger.warning(f"Failed to preserve data type for column "
                                 f"'{col}' while merging telemetry.")
 
         return merged
@@ -641,15 +629,15 @@
         | Linear interpolation will be used for continuous values (Speed, RPM)
         | Forward-fill will be used for discrete values (Gear, DRS, ...)
 
         See :meth:`register_new_channel` for adding custom channels.
         """
         ret = self.copy()
 
-        for ch in self._CHANNELS.keys():
+        for ch in self._CHANNELS:
             if ch not in self.columns:
                 continue
             sig_type = self._CHANNELS[ch]['type']
             if sig_type == 'continuous':
                 if ret[ch].dtype == 'object':
                     warnings.warn("Interpolation not possible for telemetry "
                                   "channel because dtype is 'object'")
@@ -1492,15 +1480,15 @@
             self._results = SessionResults(_nums_df.join(_info_df),
                                            force_default_cols=True)
 
             _logger.warning("Generating minimal driver "
                             "list from timing data.")
 
         df = None
-        for i, driver in enumerate(drivers):
+        for _, driver in enumerate(drivers):
             d1 = data[data['Driver'] == driver]
             d2 = useful[useful['Driver'] == driver]
             if d2.shape[0] != len(d2['Stint'].unique()):
                 # tyre info includes correction messages that need to be
                 # applied before continuing
                 d2 = self.__fix_tyre_info(d2)
 
@@ -1844,14 +1832,21 @@
             return
 
         if not self.results['Position'].isna().all() and not force:
             # Don't do anything if results are already available
             # unless force is True
             return
 
+        if self.laps['Deleted'].dtype.name != 'bool':
+            _logger.warning(
+                "Cannot calculate qualifying results: missing information "
+                "about deleted laps. Make sure that race control messages are "
+                "being loaded."
+            )
+
         quali_results = (self._laps.loc[:, ['DriverNumber']].copy()
                          .drop_duplicates()
                          .reset_index(drop=True))
         sessions = self._laps.pick_accurate().split_qualifying_sessions()
 
         for i, session in enumerate(sessions):
             session_name = f'Q{i + 1}'
@@ -2107,15 +2102,15 @@
                         lap_integrity_ok = False
                 else:
                     check_2 = False  # data not available means fail
 
                 if prev_lap is not None:
                     # first lap after safety car often has timing issues
                     # (as do all laps under safety car)
-                    check_3 = (prev_lap['TrackStatus'] != '4')
+                    check_3 = prev_lap['TrackStatus'] != '4'
                 else:
                     check_3 = True  # no previous lap, no SC error
 
                 pre_check_4 = (((not pd.isnull(lap['Time']))
                                & (not pd.isnull(lap['LapTime'])))
                                and (prev_lap is not None)
                                and (not pd.isnull(prev_lap['Time'])))
@@ -3025,17 +3020,14 @@
         .. deprecated:: 3.1.0
             pick_team is deprecated and will be removed in a future release.
             Use :func:`pick_teams` instead.
 
             mercedes = session_laps.pick_team('Mercedes')
             alfa_romeo = session_laps.pick_team('Alfa Romeo')
 
-        Have a look to :attr:`fastf1.plotting.TEAM_COLORS` for a quick
-        reference on team names.
-
         Args:
             name (str): Team name
 
         Returns:
             instance of :class:`Laps`
         """
         warnings.warn(("pick_team is deprecated and will be removed"
```

### Comparing `fastf1-3.3.5/fastf1/events.py` & `fastf1-3.4.0a0/fastf1/events.py`

 * *Files 2% similar despite different names*

```diff
@@ -203,15 +203,15 @@
 
 with warnings.catch_warnings():
     warnings.filterwarnings(
         'ignore', message="Using slow pure-python SequenceMatcher"
     )
     # suppress that warning, it's confusing at best here, we don't need fast
     # sequence matching and the installation (on windows) requires some effort
-    from thefuzz import fuzz
+    from rapidfuzz import fuzz
 
 import pandas as pd
 
 import fastf1._api
 import fastf1.ergast
 from fastf1.core import Session
 from fastf1.internals.pandas_base import (
@@ -357,15 +357,16 @@
 
 def get_event(
         year: int,
         gp: Union[int, str],
         *,
         backend: Optional[Literal['fastf1', 'f1timing', 'ergast']] = None,
         force_ergast: bool = False,
-        strict_search: bool = False
+        strict_search: bool = False,
+        exact_match: bool = False
 ) -> "Event":
     """Create an :class:`~fastf1.events.Event` object for a specific
     season and gp.
 
     To get a testing event, use :func:`get_testing_event`.
 
     Args:
@@ -396,26 +397,30 @@
             is not available.
 
             For seasons older than 2018 ``'ergast'`` is always used.
 
         force_ergast: [Deprecated, use ``backend='ergast'``] Always use data
             from the ergast database to create the event schedule
 
-        strict_search: Match precisely the query, or default to
+        strict_search: This argument is deprecated and planned for removal,
+            use the equivalent ``exact_match`` instead
+
+        exact_match: Match precisely the query, or default to
             fuzzy search. If no event is found with
-            ``strict_search=True``, the function will return None
+            ``exact_match=True``, the function will return None
 
     .. versionadded:: 2.2
     """
     schedule = get_event_schedule(year=year, include_testing=False,
                                   force_ergast=force_ergast,
                                   backend=backend)
 
     if isinstance(gp, str):
-        event = schedule.get_event_by_name(gp, strict_search=strict_search)
+        event = schedule.get_event_by_name(
+            gp, strict_search=strict_search, exact_match=exact_match)
     else:
         event = schedule.get_event_by_round(gp)
 
     return event
 
 
 def get_testing_event(
@@ -923,46 +928,76 @@
                 if event['EventName'].lower() == query:
                     return self.loc[i]
         else:
             return None
 
     def _fuzzy_event_search(self, name: str) -> "Event":
 
+        def _remove_common_words(event_name):
+            common_words = ["formula 1", str(self.year), "grand prix", "gp"]
+            event_name = event_name.casefold()
+
+            for word in common_words:
+                event_name = event_name.replace(word, "")
+
+            return event_name.replace(" ", "")
+
         def _matcher_strings(ev):
             strings = list()
             if 'Location' in ev:
-                strings.append(ev['Location'])
+                strings.append(ev['Location'].casefold())
             if 'Country' in ev:
-                strings.append(ev['Country'])
+                strings.append(ev['Country'].casefold())
             if 'EventName' in ev:
-                strings.append(ev['EventName'].replace("Grand Prix", ""))
+                strings.append(_remove_common_words(ev["EventName"]))
             if 'OfficialEventName' in ev:
-                strings.append(ev['OfficialEventName']
-                               .replace("FORMULA 1", "")
-                               .replace(str(self.year), "")
-                               .replace("GRAND PRIX", ""))
+                strings.append(_remove_common_words(ev["OfficialEventName"]))
             return strings
 
-        max_ratio = 0
-        index = 0
+        user_input = name
+        name = _remove_common_words(name)
+        full_partial_match_indices = []
+
+        # check partial matches first
+        # if there is either zero or multiple 100% matches
+        # fall back to the full ratio
         for i, event in self.iterrows():
+            if any([name in val for val in _matcher_strings(event)]):
+                full_partial_match_indices.append(i)
+
+        if len(full_partial_match_indices) == 1:
+            return self.loc[full_partial_match_indices[0]]
+
+        max_ratio = 0
+        max_index = 0
+
+        for i, event in self.loc[full_partial_match_indices
+                                  or self.index].iterrows():
             ratio = max(
-                [fuzz.ratio(val.casefold(), name.casefold())
+                [fuzz.ratio(val, name)
                  for val in _matcher_strings(event)]
             )
             if ratio > max_ratio:
                 max_ratio = ratio
-                index = i
-        return self.loc[index]
+                max_index = i
+
+        if max_ratio != 100:
+            _logger.warning((
+                "Correcting user input "
+                f"'{user_input}' to'{self.loc[max_index].EventName}'"
+            )
+            )
+        return self.loc[max_index]
 
     def get_event_by_name(
             self,
             name: str,
             *,
-            strict_search: bool = False
+            strict_search: bool = False,
+            exact_match: bool = False
     ) -> "Event":
         """Get an :class:`Event` by its name.
 
         A fuzzy match is performed to find the event that best matches the
         given name. Fuzzy matching is performed using the country, location,
         name and officialName of each event. This is not guaranteed to return
         the correct result. You should therefore always check if the function
@@ -977,24 +1012,29 @@
             Grand Prix" as ``name``.
 
         Args:
             name: The name of the event. For example,
                 ``.get_event_by_name("british")`` and
                 ``.get_event_by_name("silverstone")`` will both return the
                 event for the British Grand Prix.
-            strict_search: Search only for exact query matches
+            strict_search: This argument is deprecated and planned for removal.
+                Use the equivalent ``exact_match`` instead
+            exact_match: Search only for exact query matches
                 instead of using fuzzy search. For example,
                 ``.get_event_by_name("British Grand Prix",
-                strict_search=True)``
+                exact_match=True)``
                 will return the event for the British Grand Prix, whereas
-                ``.get_event_by_name("British", strict_search=True)``
+                ``.get_event_by_name("British", exact_match=True)``
                 will return ``None``
         """
-
         if strict_search:
+            warnings.warn(("strict_search is deprecated and planned for "
+                           "removal, use the equivalent exact_match instead"),
+                          FutureWarning)
+        if strict_search or exact_match:
             return self._strict_event_search(name)
         else:
             return self._fuzzy_event_search(name)
 
 
 class Event(BaseSeries):
     """This class represents a single event (race weekend or testing event).
```

### Comparing `fastf1-3.3.5/fastf1/legacy.py` & `fastf1-3.4.0a0/fastf1/legacy.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
     import fastf1
     import fastf1.plotting
     import fastf1.legacy
     import numpy as np
     import matplotlib.pyplot as plt
 
-    fastf1.plotting.setup_mpl()
+    fastf1.plotting.setup_mpl(misc_mpl_mods=False, color_scheme='fastf1')
 
     session = fastf1.get_session(2020, 'Italy', 'R')
     session.load()
 
     DRIVER = 'VER'  # which driver; need to specify number and abbreviation
     DRIVER_NUMBER = '33'
     LAP_N = 10  # which lap number to plot
```

### Comparing `fastf1-3.3.5/fastf1/logger.py` & `fastf1-3.4.0a0/fastf1/logger.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.5/fastf1/plotting.py` & `fastf1-3.4.0a0/fastf1/plotting/_plotting.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,206 +1,77 @@
-"""
-Helper functions for creating data plots.
-
-:mod:`fastf1.plotting` provides optional functionality with the intention of
-making it easy to create nice plots.
-
-This module offers mainly two things:
-    - team names and colors
-    - matplotlib mods and helper functions
-
-Fast-F1 focuses on plotting data with matplotlib. Of course, you are not
-required to use matplotlib and you can use any other tool you like.
-
-If you wish to use matplotlib, it is highly recommended to enable some
-helper functions by calling :func:`setup_mpl`.
-
-If you don't want to use matplotlib, you can still use the team names
-and colors which are provided below.
-
-
-.. note:: Plotting related functionality is likely to change in a future
-    release.
-"""
 import warnings
 from typing import (
-    Dict,
-    List
+    List,
+    Optional
 )
 
 import numpy as np
 import pandas as pd
 
 
 try:
     import matplotlib
     from matplotlib import cycler
     from matplotlib import pyplot as plt
 except ImportError:
     warnings.warn("Failed to import optional dependency 'matplotlib'!"
-                  "Plotting functionality will be unavailable!", UserWarning)
+                  "Plotting functionality will be unavailable!",
+                  RuntimeWarning)
 try:
     import timple
 except ImportError:
     warnings.warn("Failed to import optional dependency 'timple'!"
                   "Plotting of timedelta values will be restricted!",
-                  UserWarning)
+                  RuntimeWarning)
 
-import warnings
+from rapidfuzz import fuzz
+
+from fastf1.logger import get_logger
+from fastf1.plotting._constants import (
+    LEGACY_DRIVER_COLORS,
+    LEGACY_DRIVER_TRANSLATE,
+    LEGACY_TEAM_COLORS,
+    LEGACY_TEAM_TRANSLATE
+)
 
 
-with warnings.catch_warnings():
-    warnings.filterwarnings('ignore',
-                            message="Using slow pure-python SequenceMatcher")
-    # suppress that warning, it's confusing at best here, we don't need fast
-    # sequence matching and the installation (on windows) some effort
-    from thefuzz import fuzz
-
-
-class __TeamColorsWarnDict(dict):
-    """Implements userwarning on KeyError in :any:`TEAM_COLORS` after
-    changing team names."""
-
-    def get(self, key, default=None):
-        value = super().get(key, default)
-        if value is None:
-            self.warn_change()
-        return value
-
-    def __getitem__(self, item):
-        try:
-            return super().__getitem__(item)
-        except KeyError as err:
-            self.warn_change()
-            raise err
-        except Exception as err:
-            raise err
+_logger = get_logger(__package__)
+
+
+_COLOR_PALETTE: List[str] = ['#FF79C6', '#50FA7B', '#8BE9FD', '#BD93F9',
+                             '#FFB86C', '#FF5555', '#F1FA8C']
+# The default color palette for matplotlib plot lines in fastf1's color scheme
 
-    def warn_change(self):
-        warnings.warn(
-            "Team names in `TEAM_COLORS` are now lower-case and only contain "
-            "the most identifying part of the name. "
-            "Use function `.team_color` alternatively.", UserWarning
-        )
 
+class __DefaultStringArgType(str):
+    pass
 
-TEAM_COLORS = __TeamColorsWarnDict({
-    'mercedes': '#00d2be', 'ferrari': '#dc0000',
-    'red bull': '#fcd700', 'mclaren': '#ff8700',
-    'alpine': '#fe86bc', 'aston martin': '#006f62',
-    'sauber': '#00e701', 'visa rb': '#1634cb',
-    'haas': '#ffffff', 'williams': '#00a0dd'
-})
-"""Mapping of team names to team colors (hex color codes).
-(current season only)"""
-
-TEAM_TRANSLATE: Dict[str, str] = {
-    'MER': 'mercedes', 'FER': 'ferrari',
-    'RBR': 'red bull', 'MCL': 'mclaren',
-    'APN': 'alpine', 'AMR': 'aston martin',
-    'SAU': 'sauber', 'VRB': 'visa rb',
-    'HAA': 'haas', 'WIL': 'williams'}
-"""Mapping of team names to theirs respective abbreviations."""
-
-DRIVER_COLORS: Dict[str, str] = {
-    "valtteri bottas": "#00e701",
-    "zhou guanyu": "#008d01",
-    "theo pourchaire": "#004601",
-
-    "nyck de vries": "#1e3d61",
-    "yuki tsunoda": "#356cac",
-    "daniel ricciardo": "#2b4562",
-    "liam lawson": "#2b4562",
-    "isack hadjar": "#1e6176",
-    "ayumu iwasa": "#1e6176",
-
-    "pierre gasly": "#fe86bc",
-    "esteban ocon": "#ff117c",
-    "jack doohan": "#894667",
-
-    "fernando alonso": "#006f62",
-    "lance stroll": "#00413b",
-    "felipe drugovich": "#2f9b90",
-
-    "charles leclerc": "#dc0000",
-    "carlos sainz": "#ff8181",
-    "robert shwartzman": "#9c0000",
-    "oliver bearman": "#c40000",
-
-    "kevin magnussen": "#ffffff",
-    "nico hulkenberg": "#cacaca",
-
-    "oscar piastri": "#ff8700",
-    "lando norris": "#eeb370",
-    "pato oward": "#ee6d3a",
-
-    "lewis hamilton": "#00d2be",
-    "george russell": "#24ffff",
-    "frederik vesti": "#00a6ff",
-
-    "max verstappen": "#fcd700",
-    "sergio perez": "#ffec7b",
-    "jake dennis": "#907400",
-
-    "alexander albon": "#005aff",
-    "logan sargeant": "#012564",
-    "zak osullivan": "#1b3d97",
-}
-"""Mapping of driver names to driver colors (hex color codes).
-(current season only)"""
-
-DRIVER_TRANSLATE: Dict[str, str] = {
-    'LEC': 'charles leclerc', 'SAI': 'carlos sainz',
-    'SHW': 'robert shwartzman',
-    'VER': 'max verstappen', 'PER': 'sergio perez',
-    'DEN': 'jake dennis',
-    'PIA': 'oscar piastri', 'NOR': 'lando norris',
-    'OWA': 'pato oward',
-    'GAS': 'pierre gasly', 'OCO': 'esteban ocon',
-    'DOO': 'jack doohan',
-    'BOT': 'valtteri bottas', 'ZHO': 'zhou guanyu',
-    'POU': 'theo pourchaire',
-    'DEV': 'nyck de vries', 'TSU': 'yuki tsunoda',
-    'RIC': 'daniel ricciardo', 'LAW': 'liam lawson',
-    'HAD': 'isack hadjar', 'IWA': 'ayumu iwasa',
-    'MAG': 'kevin magnussen', 'HUL': 'nico hulkenberg',
-    'BEA': 'oliver bearman',
-    'ALO': 'fernando alonso', 'STR': 'lance stroll',
-    'DRU': 'felipe drugovich',
-    'HAM': 'lewis hamilton', 'RUS': 'george russell',
-    'VES': 'frederik vesti',
-    'ALB': 'alexander albon', 'SAR': 'logan sargeant',
-    'OSU': 'zak osullivan'}
-"""Mapping of driver names to theirs respective abbreviations."""
-
-COMPOUND_COLORS: Dict[str, str] = {
-    "SOFT": "#da291c",
-    "MEDIUM": "#ffd12e",
-    "HARD": "#f0f0ec",
-    "INTERMEDIATE": "#43b02a",
-    "WET": "#0067ad",
-    "UNKNOWN": "#00ffff",
-    "TEST-UNKNOWN": "#434649"
-}
-"""Mapping of tyre compound names to compound colors (hex color codes).
-(current season only)"""
-
-COLOR_PALETTE: List[str] = ['#FF79C6', '#50FA7B', '#8BE9FD', '#BD93F9',
-                            '#FFB86C', '#FF5555', '#F1FA8C']
-"""The default color palette for matplotlib plot lines in fastf1's color
-scheme."""
+
+__color_scheme_default_arg = __DefaultStringArgType('fastf1')
 
 
 def setup_mpl(
-        mpl_timedelta_support: bool = True, color_scheme: str = 'fastf1',
+        mpl_timedelta_support: bool = True,
+        color_scheme: Optional[str] = __color_scheme_default_arg,
         misc_mpl_mods: bool = True):
     """Setup matplotlib for use with fastf1.
 
     This is optional but, at least partly, highly recommended.
 
+    .. deprecated:: 3.4.0
+
+        The optional argument ``misc_mpls_mods`` is deprecated.
+
+    .. deprecated:: 3.4.0
+
+        The default value for ``color_scheme`` will change from ``'fastf1'``
+        to ``None``. You should explicitly set the desired value when calling
+        this function.
+
+
     Parameters:
         mpl_timedelta_support (bool):
             Matplotlib itself offers very limited functionality for plotting
             timedelta values. (Lap times, sector times and other kinds of time
             spans are represented as timedelta.)
 
             Enabling this option will patch some internal matplotlib functions
@@ -211,188 +82,208 @@
 
         color_scheme (str, None):
             This enables the Fast-F1 color scheme that you can see in all
             example images.
             Valid color scheme names are: ['fastf1', None]
 
         misc_mpl_mods (bool):
-            This enables a collection of patches for the following mpl
-            features:
-
-                - ``.savefig`` (saving of figures)
-                - ``.bar``/``.barh`` (plotting of bar graphs)
-                - ``plt.subplots`` (for creating a nice background grid)
+            This argument is deprecated since v3.4.0 and should no longer be
+            used.
     """
+    if color_scheme is __color_scheme_default_arg:
+        warnings.warn(
+            "FastF1 will no longer silently modify the default Matplotlib "
+            "colors in the future.\nTo remove this warning, explicitly set "
+            "`color_scheme=None` or `color_scheme='fastf1'` when calling "
+            "`.setup_mpl()`.", FutureWarning
+        )
+
+    if misc_mpl_mods:
+        warnings.warn(
+            "FastF1 will stop modifying the default Matplotlib settings in "
+            "the future.\nTo opt-in to the new behaviour and remove this "
+            "warning, explicitly set `misc_mpl_mods=False` when calling "
+            "`.setup_mpl()`.", FutureWarning
+        )
+
     if mpl_timedelta_support:
         _enable_timple()
     if color_scheme == 'fastf1':
         _enable_fastf1_color_scheme()
     if misc_mpl_mods:
         _enable_misc_mpl_mods()
 
 
 def driver_color(identifier: str) -> str:
-    """Get a driver's color from a driver name or abbreviation.
+    """
+    Get a driver's color from a driver name or abbreviation.
+
+    .. deprecated:: 3.4.0
+        This function is deprecated and will be removed in a future version.
+        Use :func:`~fastf1.plotting.get_driver_color` instead.
 
     This function will try to find a matching driver for any identifier string
-    that is passed to it. This involves case insensitive matching and partial
+    that is passed to it. This involves case-insensitive matching and partial
     string matching.
 
-    If you want exact string matching, you should use the
-    :any:`DRIVER_COLORS` dictionary directly, using :any:`DRIVER_TRANSLATE` to
-    convert abbreviations to team names if necessary.
-
     Example::
 
-        >>> driver_color('charles leclerc')
+        >>> driver_color('charles leclerc')  # doctest: +SKIP
         '#dc0000'
-        >>> driver_color('max verstappen')
+        >>> driver_color('max verstappen')  # doctest: +SKIP
         '#fcd700'
-        >>> driver_color('ver')
+        >>> driver_color('ver')  # doctest: +SKIP
         '#fcd700'
-        >>> driver_color('lec')
+        >>> driver_color('lec')  # doctest: +SKIP
         '#dc0000'
 
         shortened driver names and typos can be dealt with
         too (within reason)
 
-        >>> driver_color('Max Verst')
+        >>> driver_color('Max Verst')  # doctest: +SKIP
         '#fcd700'
-        >>> driver_color('Charles')
+        >>> driver_color('Charles')  # doctest: +SKIP
         '#dc0000'
 
     Args:
         identifier (str): Abbreviation or uniquely identifying name of the
             driver.
 
     Returns:
         str: hex color code
     """
+    warnings.warn("The function `driver_color` is deprecated and will be "
+                  "removed in a future version. Use "
+                  "`fastf1.plotting.get_driver_color` instead.",
+                  FutureWarning)
 
-    if identifier.upper() in DRIVER_TRANSLATE:
+    if identifier.upper() in LEGACY_DRIVER_TRANSLATE:
         # try short team abbreviations first
-        return DRIVER_COLORS[DRIVER_TRANSLATE[identifier.upper()]]
+        return LEGACY_DRIVER_COLORS[
+            LEGACY_DRIVER_TRANSLATE[identifier.upper()]
+        ]
     else:
         identifier = identifier.lower()
 
         # check for an exact team name match
-        if identifier in DRIVER_COLORS:
-            return DRIVER_COLORS[identifier]
+        if identifier in LEGACY_DRIVER_COLORS:
+            return LEGACY_DRIVER_COLORS[identifier]
 
         # check for exact partial string match
-        for team_name, color in DRIVER_COLORS.items():
+        for team_name, color in LEGACY_DRIVER_COLORS.items():
             if identifier in team_name:
                 return color
 
         # do fuzzy string matching
         key_ratios = list()
-        for existing_key in DRIVER_COLORS.keys():
+        for existing_key in LEGACY_DRIVER_COLORS:
             ratio = fuzz.ratio(identifier, existing_key)
             key_ratios.append((ratio, existing_key))
         key_ratios.sort(reverse=True)
+        if key_ratios[0][0] != 100:
+            _logger.warning(
+                ("Correcting invalid user input "
+                 f"'{identifier}' to '{key_ratios[0][1]}'."
+                 )
+            )
         if ((key_ratios[0][0] < 35)
                 or (key_ratios[0][0] / key_ratios[1][0] < 1.2)):
             # ensure that the best match has a minimum accuracy (35 out of
             # 100) and that it has a minimum confidence (at least 20% better
             # than second best)
             raise KeyError
         best_matched_key = key_ratios[0][1]
-        return DRIVER_COLORS[best_matched_key]
+        return LEGACY_DRIVER_COLORS[best_matched_key]
 
 
 def team_color(identifier: str) -> str:
-    """Get a team's color from a team name or abbreviation.
+    """
+    Get a team's color from a team name or abbreviation.
+
+    .. deprecated:: 3.4.0
+        This function is deprecated and will be removed in a future version.
+        Use :func:`~fastf1.plotting.get_team_color` instead.
 
     This function will try to find a matching team for any identifier string
-    that is passed to it. This involves case insensitive matching and partial
+    that is passed to it. This involves case-insensitive matching and partial
     string matching.
 
-    If you want exact string matching, you should use the
-    :any:`TEAM_COLORS` dictionary directly, using :any:`TEAM_TRANSLATE` to
-    convert abbreviations to team names if necessary.
-
     Example::
 
-        >>> team_color('Red Bull')
+        >>> team_color('Red Bull')  # doctest: +SKIP
         '#fcd700'
-        >>> team_color('redbull')
+        >>> team_color('redbull')  # doctest: +SKIP
         '#fcd700'
-        >>> team_color('Red')
+        >>> team_color('Red')  # doctest: +SKIP
         '#fcd700'
-        >>> team_color('RBR')
+        >>> team_color('RBR')  # doctest: +SKIP
         '#fcd700'
 
-        shortened team names, included sponsors and typos can be dealt with
-        too (within reason)
+        # shortened team names, included sponsors and typos can be dealt with
+        # too (within reason)
 
-        >>> team_color('Mercedes')
+        >>> team_color('Mercedes')  # doctest: +SKIP
         '#00d2be'
-        >>> team_color('Merc')
+        >>> team_color('Merc')  # doctest: +SKIP
         '#00d2be'
-        >>> team_color('Merecds')
+        >>> team_color('Merecds')  # doctest: +SKIP
         '#00d2be'
-        >>> team_color('Mercedes-AMG Petronas F1 Team')
+        >>> team_color('Mercedes-AMG Petronas F1 Team')  # doctest: +SKIP
         '#00d2be'
 
     Args:
         identifier (str): Abbreviation or uniquely identifying name of the
             team.
 
     Returns:
         str: hex color code
     """
-    if identifier.upper() in TEAM_TRANSLATE:
+    warnings.warn("The function `team_color` is deprecated and will be "
+                  "removed in a future version. Use "
+                  "`fastf1.plotting.get_team_color` instead.",
+                  FutureWarning)
+
+    if identifier.upper() in LEGACY_TEAM_TRANSLATE:
         # try short team abbreviations first
-        return TEAM_COLORS[TEAM_TRANSLATE[identifier.upper()]]
+        return LEGACY_TEAM_COLORS[LEGACY_TEAM_TRANSLATE[identifier.upper()]]
     else:
         identifier = identifier.lower()
         # remove common non-unique words
         for word in ('racing', 'team', 'f1', 'scuderia'):
             identifier = identifier.replace(word, "")
 
         # check for an exact team name match
-        if identifier in TEAM_COLORS:
-            return TEAM_COLORS[identifier]
+        if identifier in LEGACY_TEAM_COLORS:
+            return LEGACY_TEAM_COLORS[identifier]
 
         # check for exact partial string match
-        for team_name, color in TEAM_COLORS.items():
+        for team_name, color in LEGACY_TEAM_COLORS.items():
             if identifier in team_name:
                 return color
 
         # do fuzzy string matching
         key_ratios = list()
-        for existing_key in TEAM_COLORS.keys():
+        for existing_key in LEGACY_TEAM_COLORS.keys():
             ratio = fuzz.ratio(identifier, existing_key)
             key_ratios.append((ratio, existing_key))
         key_ratios.sort(reverse=True)
+        if key_ratios[0][0] != 100:
+            _logger.warning(
+                ("Correcting invalid user input "
+                 f"'{identifier}' to '{key_ratios[0][1]}'."
+                 )
+            )
         if ((key_ratios[0][0] < 35)
                 or (key_ratios[0][0] / key_ratios[1][0] < 1.2)):
             # ensure that the best match has a minimum accuracy (35 out of
             # 100) and that it has a minimum confidence (at least 20% better
             # than second best)
             raise KeyError
         best_matched_key = key_ratios[0][1]
-        return TEAM_COLORS[best_matched_key]
-
-
-def lapnumber_axis(ax, axis='xaxis'):
-    """Set axis to integer ticks only."
-
-    Args:
-        ax: matplotlib axis
-        axis: can be 'xaxis' or 'yaxis'
-
-    Returns:
-        the modified axis instance
-
-    """
-    getattr(ax, axis).get_major_locator().set_params(integer=True,
-                                                     min_n_ticks=0)
-
-    return ax
+        return LEGACY_TEAM_COLORS[best_matched_key]
 
 
 def _enable_timple():
     # use external package timple to patch matplotlib
     # this adds converters, locators and formatters for
     # plotting timedelta values
     tick_formats = [
@@ -483,13 +374,37 @@
     plt.rcParams['axes.titlesize'] = 'x-large'
     # plt.rcParams['font.family'] = 'Gravity'
     plt.rcParams['font.weight'] = 'medium'
     plt.rcParams['text.color'] = '#F1F1F3'
     plt.rcParams['axes.titlesize'] = '19'
     plt.rcParams['axes.titlepad'] = '12'
     plt.rcParams['axes.titleweight'] = 'light'
-    plt.rcParams['axes.prop_cycle'] = cycler('color', COLOR_PALETTE)
+    plt.rcParams['axes.prop_cycle'] = cycler('color', _COLOR_PALETTE)
     plt.rcParams['legend.fancybox'] = False
     plt.rcParams['legend.facecolor'] = (0.1, 0.1, 0.1, 0.7)
     plt.rcParams['legend.edgecolor'] = (0.1, 0.1, 0.1, 0.9)
     plt.rcParams['savefig.transparent'] = False
     plt.rcParams['axes.axisbelow'] = True
+
+
+def lapnumber_axis(ax, axis='xaxis'):
+    """
+    Set axis to integer ticks only.
+
+    .. deprecated:: 3.4.0
+        The function ``lapnumber_axis`` is deprecated and will ber removed in a
+        future version without replacement.
+
+    Args:
+        ax: matplotlib axis
+        axis: can be 'xaxis' or 'yaxis'
+
+    Returns:
+        the modified axis instance
+    """
+    warnings.warn("The function `lapnumber_axis` is deprecated and will be "
+                  "removed without replacement in a future version.",
+                  FutureWarning)
+    getattr(ax, axis).get_major_locator().set_params(integer=True,
+                                                     min_n_ticks=0)
+
+    return ax
```

### Comparing `fastf1-3.3.5/fastf1/req.py` & `fastf1-3.4.0a0/fastf1/req.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.5/fastf1/utils.py` & `fastf1-3.4.0a0/fastf1/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,31 +46,31 @@
         :include-source:
 
         import fastf1 as ff1
         from fastf1 import plotting
         from fastf1 import utils
         from matplotlib import pyplot as plt
 
-        plotting.setup_mpl()
+        plotting.setup_mpl(misc_mpl_mods=False, color_scheme='fastf1')
 
         session = ff1.get_session(2021, 'Emilia Romagna', 'Q')
         session.load()
         lec = session.laps.pick_driver('LEC').pick_fastest()
         ham = session.laps.pick_driver('HAM').pick_fastest()
 
         delta_time, ref_tel, compare_tel = utils.delta_time(ham, lec)
         # ham is reference, lec is compared
 
         fig, ax = plt.subplots()
         # use telemetry returned by .delta_time for best accuracy,
-        # this ensure the same applied interpolation and resampling
+        # this ensures the same applied interpolation and resampling
         ax.plot(ref_tel['Distance'], ref_tel['Speed'],
-                color=plotting.team_color(ham['Team']))
+                color=plotting.get_team_color(ham['Team'], session))
         ax.plot(compare_tel['Distance'], compare_tel['Speed'],
-                color=plotting.team_color(lec['Team']))
+                color=plotting.get_team_color(lec['Team'], session))
 
         twin = ax.twinx()
         twin.plot(ref_tel['Distance'], delta_time, '--', color='white')
         twin.set_ylabel("<-- Lec ahead | Ham ahead -->")
         plt.show()
 
     Args:
```

### Comparing `fastf1-3.3.5/fastf1/ergast/interface.py` & `fastf1-3.4.0a0/fastf1/ergast/interface.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.5/fastf1/ergast/legacy.py` & `fastf1-3.4.0a0/fastf1/ergast/legacy.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.5/fastf1/ergast/sphinx.py` & `fastf1-3.4.0a0/fastf1/ergast/sphinx.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.5/fastf1/ergast/structure.py` & `fastf1-3.4.0a0/fastf1/ergast/structure.py`

 * *Files 0% similar despite different names*

```diff
@@ -244,15 +244,15 @@
     Transform to ::
 
         {'value' : [1, 2, 3, 4, 5, 6, ...], ...},
     """
     if len(data) <= 1:
         return data[0]
 
-    for i in range(len(data) - 1):
+    for _ in range(len(data) - 1):
         _tmp = data.pop(1)
         for key in data[0].keys():
             data[0][key].extend(_tmp.pop(key))
 
     return data[0]
```

### Comparing `fastf1-3.3.5/fastf1/internals/pandas_base.py` & `fastf1-3.4.0a0/fastf1/internals/pandas_base.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.5/fastf1/internals/pandas_extensions.py` & `fastf1-3.4.0a0/fastf1/internals/pandas_extensions.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.5/fastf1/livetiming/__init__.py` & `fastf1-3.4.0a0/fastf1/livetiming/__init__.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.5/fastf1/livetiming/__main__.py` & `fastf1-3.4.0a0/fastf1/livetiming/__main__.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.5/fastf1/livetiming/client.py` & `fastf1-3.4.0a0/fastf1/livetiming/client.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.5/fastf1/livetiming/data.py` & `fastf1-3.4.0a0/fastf1/livetiming/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -159,18 +159,18 @@
         if cat not in self.data:
             self.data[cat] = [entry, ]
         else:
             self.data[cat].append(entry)
 
     def _parse_session_data(self, msg):
         # make sure the categories exist as we want to append to them
-        if 'TrackStatus' not in self.data.keys():
+        if 'TrackStatus' not in self.data:
             self.data['TrackStatus'] = {'Time': [], 'Status': [],
                                         'Message': []}
-        if 'SessionStatus' not in self.data.keys():
+        if 'SessionStatus' not in self.data:
             self.data['SessionStatus'] = {'Time': [], 'Status': []}
 
         if ('StatusSeries' in msg) and isinstance(msg['StatusSeries'], dict):
             for entry in msg['StatusSeries'].values():
                 # convert timestamp to timedelta
                 try:
                     status_dt = to_datetime(entry['Utc'])
@@ -190,15 +190,15 @@
                     self.data['TrackStatus']['Message'].append("")
 
                 elif 'SessionStatus' in entry.keys():
                     self.data['SessionStatus']['Time'].append(status_timedelta)
                     self.data['SessionStatus']['Status'].append(entry['SessionStatus'])
 
     def _parse_race_control_message(self, msg):
-        if 'RaceControlMessages' not in self.data.keys():
+        if 'RaceControlMessages' not in self.data:
             self.data['RaceControlMessages'] = {
                 'Utc': [], 'Category': [], 'Message': [], 'Status': [],
                 'Flag': [], 'Scope': [], 'Sector': [], 'RacingNumber': []
             }
 
         if ('Messages' in msg) and isinstance(msg['Messages'], dict):
             for data in msg['Messages'].values():
```

### Comparing `fastf1-3.3.5/fastf1/mvapi/api.py` & `fastf1-3.4.0a0/fastf1/mvapi/api.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.5/fastf1/mvapi/data.py` & `fastf1-3.4.0a0/fastf1/mvapi/data.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.5/fastf1/signalr_aio/LICENSE` & `fastf1-3.4.0a0/fastf1/signalr_aio/LICENSE`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.5/fastf1/signalr_aio/_connection.py` & `fastf1-3.4.0a0/fastf1/signalr_aio/_connection.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.5/fastf1/signalr_aio/hubs/_hub.py` & `fastf1-3.4.0a0/fastf1/signalr_aio/hubs/_hub.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.5/fastf1/signalr_aio/transports/_parameters.py` & `fastf1-3.4.0a0/fastf1/signalr_aio/transports/_parameters.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.5/fastf1/signalr_aio/transports/_transport.py` & `fastf1-3.4.0a0/fastf1/signalr_aio/transports/_transport.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.5/.gitignore` & `fastf1-3.4.0a0/.gitignore`

 * *Files 6% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 # temporary testrun directories
 fastf1/tests/testenv/
 fastf1/tests/mpl-results/
 fastf1/tests/mpl-baseline-new/
 
 # documentation build directories
 docs/_build/
-docs/examples_gallery/
+docs/gen_modules/
 **/sg_execution_times.rst
 
 # all variations of cache directories
 *_cache/
 .DS_Store
 
 # other data directories
```

### Comparing `fastf1-3.3.5/LICENSE` & `fastf1-3.4.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.5/README.md` & `fastf1-3.4.0a0/README.md`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.5/pyproject.toml` & `fastf1-3.4.0a0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
   "matplotlib>=3.5.1,<4.0.0",
   "numpy>=1.21.5,<2.0.0",
   "pandas>=1.4.1,<3.0.0",
   "python-dateutil",
   "requests>=2.28.1",
   "requests-cache>=1.0.0",
   "scipy>=1.7.3,<2.0.0",
-  "thefuzz",
+  "rapidfuzz",
   "timple>=0.1.6",
   "websockets>=10.3",
 ]
 
 [project.urls]
 "Source Code" = "https://github.com/theOehrly/Fast-F1"
 "Documentation" = "https://docs.fastf1.dev"
```

### Comparing `fastf1-3.3.5/PKG-INFO` & `fastf1-3.4.0a0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: fastf1
-Version: 3.3.5
+Version: 3.4.0a0
 Summary: Python package for accessing and analyzing Formula 1 results, schedules, timing data and telemetry.
 Project-URL: Source Code, https://github.com/theOehrly/Fast-F1
 Project-URL: Documentation, https://docs.fastf1.dev
 Author: Philipp Schaefer
 Author-email: oehrly@mailbox.org
 License: MIT License
         
@@ -29,18 +29,18 @@
         SOFTWARE.
 License-File: LICENSE
 Requires-Python: >=3.8
 Requires-Dist: matplotlib<4.0.0,>=3.5.1
 Requires-Dist: numpy<2.0.0,>=1.21.5
 Requires-Dist: pandas<3.0.0,>=1.4.1
 Requires-Dist: python-dateutil
+Requires-Dist: rapidfuzz
 Requires-Dist: requests-cache>=1.0.0
 Requires-Dist: requests>=2.28.1
 Requires-Dist: scipy<2.0.0,>=1.7.3
-Requires-Dist: thefuzz
 Requires-Dist: timple>=0.1.6
 Requires-Dist: websockets>=10.3
 Description-Content-Type: text/markdown
 
 # FastF1
 
 FastF1 is a python package for accessing and analyzing Formula 1 results,
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.3 Name: fastf1 Version: 3.3.5 Summary: Python package for
+Metadata-Version: 2.3 Name: fastf1 Version: 3.4.0a0 Summary: Python package for
 accessing and analyzing Formula 1 results, schedules, timing data and
 telemetry. Project-URL: Source Code, https://github.com/theOehrly/Fast-F1
 Project-URL: Documentation, https://docs.fastf1.dev Author: Philipp Schaefer
 Author-email: oehrly@mailbox.org License: MIT License Copyright (c) 2024
 Philipp SchÃ¤fer Permission is hereby granted, free of charge, to any person
 obtaining a copy of this software and associated documentation files (the
 "Software"), to deal in the Software without restriction, including without
@@ -15,18 +15,18 @@
 LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE
 AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE
 LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF
 CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE
 SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE. License-File: LICENSE
 Requires-Python: >=3.8 Requires-Dist: matplotlib<4.0.0,>=3.5.1 Requires-Dist:
 numpy<2.0.0,>=1.21.5 Requires-Dist: pandas<3.0.0,>=1.4.1 Requires-Dist: python-
-dateutil Requires-Dist: requests-cache>=1.0.0 Requires-Dist: requests>=2.28.1
-Requires-Dist: scipy<2.0.0,>=1.7.3 Requires-Dist: thefuzz Requires-Dist:
-timple>=0.1.6 Requires-Dist: websockets>=10.3 Description-Content-Type: text/
-markdown # FastF1 FastF1 is a python package for accessing and analyzing
+dateutil Requires-Dist: rapidfuzz Requires-Dist: requests-cache>=1.0.0
+Requires-Dist: requests>=2.28.1 Requires-Dist: scipy<2.0.0,>=1.7.3 Requires-
+Dist: timple>=0.1.6 Requires-Dist: websockets>=10.3 Description-Content-Type:
+text/markdown # FastF1 FastF1 is a python package for accessing and analyzing
 Formula 1 results, schedules, timing data and telemetry. ![](docs/_static/
 readme.png "banner") ## Main Features - Access to F1 timing data, telemetry,
 sessions results and more - Full support for [Ergast](http://ergast.com/mrd/
 ) to access current and historical F1 data - All data is provided in the form
 of extended Pandas DataFrames to make working with the data easy while having
 powerful tools available - Adds custom functions to the Pandas objects
 specifically to make working with F1 data quick and simple - Integration with
```

