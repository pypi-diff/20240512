# Comparing `tmp/gui-api-tkinter-0.0.23.tar.gz` & `tmp/gui_api_tkinter-0.0.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gui-api-tkinter-0.0.23.tar", last modified: Wed Dec 20 04:32:32 2023, max compression
+gzip compressed data, was "gui_api_tkinter-0.0.24.tar", last modified: Sun May 12 00:15:29 2024, max compression
```

## Comparing `gui-api-tkinter-0.0.23.tar` & `gui_api_tkinter-0.0.24.tar`

### file list

```diff
@@ -1,90 +1,109 @@
-drwxrwxr-x   0 arrizza   (1000) arrizza   (1000)        0 2023-12-20 04:32:32.474185 gui-api-tkinter-0.0.23/
--rw-rw-r--   0 arrizza   (1000) arrizza   (1000)     1088 2023-03-13 00:13:36.000000 gui-api-tkinter-0.0.23/LICENSE.txt
--rw-rw-r--   0 arrizza   (1000) arrizza   (1000)       47 2023-12-20 04:32:32.000000 gui-api-tkinter-0.0.23/MANIFEST.in
--rw-r--r--   0 arrizza   (1000) arrizza   (1000)     2373 2023-12-20 04:32:32.474185 gui-api-tkinter-0.0.23/PKG-INFO
--rw-rw-r--   0 arrizza   (1000) arrizza   (1000)     1591 2023-12-07 04:48:04.000000 gui-api-tkinter-0.0.23/README.md
-drwxrwxr-x   0 arrizza   (1000) arrizza   (1000)        0 2023-12-20 04:32:32.466185 gui-api-tkinter-0.0.23/gui_api_tkinter/
--rw-rw-r--   0 arrizza   (1000) arrizza   (1000)      138 2023-03-13 00:13:36.000000 gui-api-tkinter-0.0.23/gui_api_tkinter/__init__.py
-drwxrwxr-x   0 arrizza   (1000) arrizza   (1000)        0 2023-12-20 04:32:32.470185 gui-api-tkinter-0.0.23/gui_api_tkinter/lib/
--rw-rw-r--   0 arrizza   (1000) arrizza   (1000)       29 2023-12-12 22:58:34.000000 gui-api-tkinter-0.0.23/gui_api_tkinter/lib/.gitignore
--rw-rw-r--   0 arrizza   (1000) arrizza   (1000)        0 2023-03-13 00:13:36.000000 gui-api-tkinter-0.0.23/gui_api_tkinter/lib/__init__.py
--rw-rw-r--   0 arrizza   (1000) arrizza   (1000)      282 2023-12-20 04:32:32.000000 gui-api-tkinter-0.0.23/gui_api_tkinter/lib/build_info.py
--rw-rw-r--   0 arrizza   (1000) arrizza   (1000)      542 2023-03-13 00:13:36.000000 gui-api-tkinter-0.0.23/gui_api_tkinter/lib/cfg.py
--rw-rw-r--   0 arrizza   (1000) arrizza   (1000)      531 2023-03-13 00:13:36.000000 gui-api-tkinter-0.0.23/gui_api_tkinter/lib/constants.py
-drwxrwxr-x   0 arrizza   (1000) arrizza   (1000)        0 2023-12-20 04:32:32.470185 gui-api-tkinter-0.0.23/gui_api_tkinter/lib/guiapi/
--rw-rw-r--   0 arrizza   (1000) arrizza   (1000)        0 2023-03-13 00:13:36.000000 gui-api-tkinter-0.0.23/gui_api_tkinter/lib/guiapi/__init__.py
--rw-rw-r--   0 arrizza   (1000) arrizza   (1000)     3567 2023-12-07 20:16:52.000000 gui-api-tkinter-0.0.23/gui_api_tkinter/lib/guiapi/gui_api_server.py
--rw-rw-r--   0 arrizza   (1000) arrizza   (1000)    10815 2023-12-07 20:17:33.000000 gui-api-tkinter-0.0.23/gui_api_tkinter/lib/guiapi/gui_api_tkinter.py
-drwxrwxr-x   0 arrizza   (1000) arrizza   (1000)        0 2023-12-20 04:32:32.470185 gui-api-tkinter-0.0.23/gui_api_tkinter/lib/harness/
--rw-rw-r--   0 arrizza   (1000) arrizza   (1000)        0 2023-03-13 00:13:36.000000 gui-api-tkinter-0.0.23/gui_api_tkinter/lib/harness/__init__.py
--rw-rw-r--   0 arrizza   (1000) arrizza   (1000)     5815 2023-12-07 20:17:49.000000 gui-api-tkinter-0.0.23/gui_api_tkinter/lib/harness/client.py
--rw-rw-r--   0 arrizza   (1000) arrizza   (1000)    10470 2023-12-07 20:18:06.000000 gui-api-tkinter-0.0.23/gui_api_tkinter/lib/harness/gui_api_harness.py
--rw-rw-r--   0 arrizza   (1000) arrizza   (1000)     5301 2023-03-13 00:13:36.000000 gui-api-tkinter-0.0.23/gui_api_tkinter/lib/harness/response.py
--rw-rw-r--   0 arrizza   (1000) arrizza   (1000)      900 2023-03-13 00:13:36.000000 gui-api-tkinter-0.0.23/gui_api_tkinter/lib/harness/widget_base.py
--rw-rw-r--   0 arrizza   (1000) arrizza   (1000)     2587 2023-03-13 00:13:36.000000 gui-api-tkinter-0.0.23/gui_api_tkinter/lib/harness/widget_click.py
--rw-rw-r--   0 arrizza   (1000) arrizza   (1000)     3082 2023-03-13 00:13:36.000000 gui-api-tkinter-0.0.23/gui_api_tkinter/lib/harness/widget_combobox.py
--rw-rw-r--   0 arrizza   (1000) arrizza   (1000)     3287 2023-03-13 00:13:36.000000 gui-api-tkinter-0.0.23/gui_api_tkinter/lib/harness/widget_listbox.py
--rw-rw-r--   0 arrizza   (1000) arrizza   (1000)     2943 2023-03-13 00:13:36.000000 gui-api-tkinter-0.0.23/gui_api_tkinter/lib/harness/widget_text.py
--rw-rw-r--   0 arrizza   (1000) arrizza   (1000)      209 2023-03-13 00:13:36.000000 gui-api-tkinter-0.0.23/gui_api_tkinter/lib/logger_null.py
--rw-rw-r--   0 arrizza   (1000) arrizza   (1000)      174 2023-03-13 00:13:36.000000 gui-api-tkinter-0.0.23/gui_api_tkinter/lib/svc.py
--rw-rw-r--   0 arrizza   (1000) arrizza   (1000)       27 2023-12-20 04:32:32.000000 gui-api-tkinter-0.0.23/gui_api_tkinter/lib/version.json
-drwxrwxr-x   0 arrizza   (1000) arrizza   (1000)        0 2023-12-20 04:32:32.474185 gui-api-tkinter-0.0.23/gui_api_tkinter.egg-info/
--rw-r--r--   0 arrizza   (1000) arrizza   (1000)     2373 2023-12-20 04:32:32.000000 gui-api-tkinter-0.0.23/gui_api_tkinter.egg-info/PKG-INFO
--rw-rw-r--   0 arrizza   (1000) arrizza   (1000)     2033 2023-12-20 04:32:32.000000 gui-api-tkinter-0.0.23/gui_api_tkinter.egg-info/SOURCES.txt
--rw-rw-r--   0 arrizza   (1000) arrizza   (1000)        1 2023-12-20 04:32:32.000000 gui-api-tkinter-0.0.23/gui_api_tkinter.egg-info/dependency_links.txt
--rw-rw-r--   0 arrizza   (1000) arrizza   (1000)       33 2023-12-20 04:32:32.000000 gui-api-tkinter-0.0.23/gui_api_tkinter.egg-info/requires.txt
--rw-rw-r--   0 arrizza   (1000) arrizza   (1000)       33 2023-12-20 04:32:32.000000 gui-api-tkinter-0.0.23/gui_api_tkinter.egg-info/top_level.txt
-drwxrwxr-x   0 arrizza   (1000) arrizza   (1000)        0 2023-12-20 04:32:32.470185 gui-api-tkinter-0.0.23/sample/
--rw-rw-r--   0 arrizza   (1000) arrizza   (1000)        0 2023-03-13 00:13:36.000000 gui-api-tkinter-0.0.23/sample/__init__.py
-drwxrwxr-x   0 arrizza   (1000) arrizza   (1000)        0 2023-12-20 04:32:32.470185 gui-api-tkinter-0.0.23/sample/common/
--rw-rw-r--   0 arrizza   (1000) arrizza   (1000)        0 2023-12-08 02:22:31.000000 gui-api-tkinter-0.0.23/sample/common/__init__.py
--rw-rw-r--   0 arrizza   (1000) arrizza   (1000)     4107 2023-12-07 20:18:16.000000 gui-api-tkinter-0.0.23/sample/common/cmd_runner.py
--rw-rw-r--   0 arrizza   (1000) arrizza   (1000)     1509 2023-03-13 00:13:36.000000 gui-api-tkinter-0.0.23/sample/common/logger.py
--rw-rw-r--   0 arrizza   (1000) arrizza   (1000)     2839 2023-03-13 00:13:36.000000 gui-api-tkinter-0.0.23/sample/main.py
--rw-rw-r--   0 arrizza   (1000) arrizza   (1000)      621 2023-12-20 04:32:32.474185 gui-api-tkinter-0.0.23/setup.cfg
--rw-rw-r--   0 arrizza   (1000) arrizza   (1000)     1469 2023-12-20 04:32:32.000000 gui-api-tkinter-0.0.23/setup.py
-drwxrwxr-x   0 arrizza   (1000) arrizza   (1000)        0 2023-12-20 04:32:32.470185 gui-api-tkinter-0.0.23/tools/
--rw-rw-r--   0 arrizza   (1000) arrizza   (1000)        0 2023-03-13 00:13:36.000000 gui-api-tkinter-0.0.23/tools/__init__.py
--rw-rw-r--   0 arrizza   (1000) arrizza   (1000)     4065 2023-12-19 00:36:34.000000 gui-api-tkinter-0.0.23/tools/debug_logger.py
-drwxrwxr-x   0 arrizza   (1000) arrizza   (1000)        0 2023-12-20 04:32:32.470185 gui-api-tkinter-0.0.23/tools/install/
--rw-rw-r--   0 arrizza   (1000) arrizza   (1000)        0 2023-12-07 04:48:04.000000 gui-api-tkinter-0.0.23/tools/install/__init__.py
--rw-rw-r--   0 arrizza   (1000) arrizza   (1000)      637 2023-03-13 00:01:54.000000 gui-api-tkinter-0.0.23/tools/loader.py
--rw-rw-r--   0 arrizza   (1000) arrizza   (1000)     1437 2023-12-20 04:25:40.000000 gui-api-tkinter-0.0.23/tools/main.py
--rw-rw-r--   0 arrizza   (1000) arrizza   (1000)     1399 2023-12-20 04:20:34.000000 gui-api-tkinter-0.0.23/tools/setup_template.py
-drwxrwxr-x   0 arrizza   (1000) arrizza   (1000)        0 2023-12-20 04:32:32.470185 gui-api-tkinter-0.0.23/tools/xplat_utils/
--rw-rw-r--   0 arrizza   (1000) arrizza   (1000)       29 2023-12-20 04:21:50.000000 gui-api-tkinter-0.0.23/tools/xplat_utils/__init__.py
-drwxrwxr-x   0 arrizza   (1000) arrizza   (1000)        0 2023-12-20 04:32:32.474185 gui-api-tkinter-0.0.23/ver/
--rw-rw-r--   0 arrizza   (1000) arrizza   (1000)        0 2023-03-13 00:13:36.000000 gui-api-tkinter-0.0.23/ver/__init__.py
-drwxrwxr-x   0 arrizza   (1000) arrizza   (1000)        0 2023-12-20 04:32:32.474185 gui-api-tkinter-0.0.23/ver/gui/
--rw-rw-r--   0 arrizza   (1000) arrizza   (1000)        0 2023-03-13 00:13:36.000000 gui-api-tkinter-0.0.23/ver/gui/__init__.py
--rw-rw-r--   0 arrizza   (1000) arrizza   (1000)     1667 2023-03-13 00:13:36.000000 gui-api-tkinter-0.0.23/ver/gui/app.py
--rw-rw-r--   0 arrizza   (1000) arrizza   (1000)      713 2023-03-13 00:13:36.000000 gui-api-tkinter-0.0.23/ver/gui/cfg.py
--rw-rw-r--   0 arrizza   (1000) arrizza   (1000)      793 2023-03-13 00:13:36.000000 gui-api-tkinter-0.0.23/ver/gui/cli.py
--rw-rw-r--   0 arrizza   (1000) arrizza   (1000)      163 2023-12-07 05:10:33.000000 gui-api-tkinter-0.0.23/ver/gui/constants.py
--rw-rw-r--   0 arrizza   (1000) arrizza   (1000)      186 2023-12-07 05:10:37.000000 gui-api-tkinter-0.0.23/ver/gui/frame_base.py
--rw-rw-r--   0 arrizza   (1000) arrizza   (1000)      172 2023-03-13 00:13:36.000000 gui-api-tkinter-0.0.23/ver/gui/main.py
--rw-rw-r--   0 arrizza   (1000) arrizza   (1000)      872 2023-03-13 00:13:36.000000 gui-api-tkinter-0.0.23/ver/gui/model.py
--rw-rw-r--   0 arrizza   (1000) arrizza   (1000)      280 2023-03-13 00:13:36.000000 gui-api-tkinter-0.0.23/ver/gui/mvc.py
--rw-rw-r--   0 arrizza   (1000) arrizza   (1000)     8440 2023-12-07 05:28:01.000000 gui-api-tkinter-0.0.23/ver/gui/page1_frame.py
--rw-rw-r--   0 arrizza   (1000) arrizza   (1000)     5409 2023-12-07 05:05:38.000000 gui-api-tkinter-0.0.23/ver/gui/view.py
-drwxrwxr-x   0 arrizza   (1000) arrizza   (1000)        0 2023-12-20 04:32:32.474185 gui-api-tkinter-0.0.23/ver/helpers/
--rw-rw-r--   0 arrizza   (1000) arrizza   (1000)        0 2023-03-13 00:13:36.000000 gui-api-tkinter-0.0.23/ver/helpers/__init__.py
--rw-rw-r--   0 arrizza   (1000) arrizza   (1000)     4061 2023-12-07 05:33:01.000000 gui-api-tkinter-0.0.23/ver/helpers/cmd_runner.py
--rw-rw-r--   0 arrizza   (1000) arrizza   (1000)       99 2023-12-06 06:30:03.000000 gui-api-tkinter-0.0.23/ver/helpers/gen_report.py
--rw-rw-r--   0 arrizza   (1000) arrizza   (1000)     2372 2023-12-07 05:33:01.000000 gui-api-tkinter-0.0.23/ver/helpers/helper.py
--rw-rw-r--   0 arrizza   (1000) arrizza   (1000)     1734 2023-12-07 05:24:53.000000 gui-api-tkinter-0.0.23/ver/helpers/logger_file.py
--rw-rw-r--   0 arrizza   (1000) arrizza   (1000)      669 2023-12-07 04:56:10.000000 gui-api-tkinter-0.0.23/ver/helpers/logger_mock.py
--rw-rw-r--   0 arrizza   (1000) arrizza   (1000)     1517 2023-12-07 05:23:11.000000 gui-api-tkinter-0.0.23/ver/helpers/logger_stdout.py
--rw-rw-r--   0 arrizza   (1000) arrizza   (1000)       73 2023-12-07 04:48:04.000000 gui-api-tkinter-0.0.23/ver/helpers/svc.py
--rw-rw-r--   0 arrizza   (1000) arrizza   (1000)     2959 2023-12-07 05:34:25.000000 gui-api-tkinter-0.0.23/ver/test_tp001_basic.py
--rw-rw-r--   0 arrizza   (1000) arrizza   (1000)     2079 2023-12-07 05:33:01.000000 gui-api-tkinter-0.0.23/ver/test_tp002_no_callback.py
--rw-rw-r--   0 arrizza   (1000) arrizza   (1000)     6521 2023-12-07 05:41:52.000000 gui-api-tkinter-0.0.23/ver/test_tp003_click_button.py
--rw-rw-r--   0 arrizza   (1000) arrizza   (1000)     4375 2023-12-07 05:34:25.000000 gui-api-tkinter-0.0.23/ver/test_tp004_search.py
--rw-rw-r--   0 arrizza   (1000) arrizza   (1000)     1840 2023-12-07 05:37:13.000000 gui-api-tkinter-0.0.23/ver/test_tp005_1client.py
--rw-rw-r--   0 arrizza   (1000) arrizza   (1000)     5933 2023-12-07 05:37:13.000000 gui-api-tkinter-0.0.23/ver/test_tp006_info.py
--rw-rw-r--   0 arrizza   (1000) arrizza   (1000)     4174 2023-12-07 05:37:13.000000 gui-api-tkinter-0.0.23/ver/test_tp007_menuitem.py
--rw-rw-r--   0 arrizza   (1000) arrizza   (1000)     8840 2023-12-07 05:37:13.000000 gui-api-tkinter-0.0.23/ver/test_tp008_entry.py
--rw-rw-r--   0 arrizza   (1000) arrizza   (1000)     5008 2023-12-07 05:34:25.000000 gui-api-tkinter-0.0.23/ver/test_tp009_radiobutton.py
--rw-rw-r--   0 arrizza   (1000) arrizza   (1000)     8817 2023-12-07 05:37:13.000000 gui-api-tkinter-0.0.23/ver/test_tp010_text.py
--rw-rw-r--   0 arrizza   (1000) arrizza   (1000)     9573 2023-12-07 05:41:52.000000 gui-api-tkinter-0.0.23/ver/test_tp011_listbox.py
--rw-rw-r--   0 arrizza   (1000) arrizza   (1000)     9027 2023-12-07 05:41:52.000000 gui-api-tkinter-0.0.23/ver/test_tp012_combobox.py
+drwxrwxr-x   0 arrizza   (1000) arrizza   (1000)        0 2024-05-12 00:15:29.912327 gui_api_tkinter-0.0.24/
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)     1088 2023-03-13 00:13:36.000000 gui_api_tkinter-0.0.24/LICENSE.txt
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)       47 2024-05-12 00:15:29.000000 gui_api_tkinter-0.0.24/MANIFEST.in
+-rw-r--r--   0 arrizza   (1000) arrizza   (1000)     2630 2024-05-12 00:15:29.912327 gui_api_tkinter-0.0.24/PKG-INFO
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)     1845 2024-02-29 02:16:51.000000 gui_api_tkinter-0.0.24/README.md
+drwxrwxr-x   0 arrizza   (1000) arrizza   (1000)        0 2024-05-12 00:15:29.904327 gui_api_tkinter-0.0.24/gui_api_tkinter/
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)      138 2024-02-13 17:33:18.000000 gui_api_tkinter-0.0.24/gui_api_tkinter/__init__.py
+drwxrwxr-x   0 arrizza   (1000) arrizza   (1000)        0 2024-05-12 00:15:29.904327 gui_api_tkinter-0.0.24/gui_api_tkinter/lib/
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)       29 2023-12-12 22:58:34.000000 gui_api_tkinter-0.0.24/gui_api_tkinter/lib/.gitignore
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)        0 2023-03-13 00:13:36.000000 gui_api_tkinter-0.0.24/gui_api_tkinter/lib/__init__.py
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)      282 2024-05-12 00:15:29.000000 gui_api_tkinter-0.0.24/gui_api_tkinter/lib/build_info.py
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)      542 2023-03-13 00:13:36.000000 gui_api_tkinter-0.0.24/gui_api_tkinter/lib/cfg.py
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)      531 2023-03-13 00:13:36.000000 gui_api_tkinter-0.0.24/gui_api_tkinter/lib/constants.py
+drwxrwxr-x   0 arrizza   (1000) arrizza   (1000)        0 2024-05-12 00:15:29.904327 gui_api_tkinter-0.0.24/gui_api_tkinter/lib/guiapi/
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)        0 2023-03-13 00:13:36.000000 gui_api_tkinter-0.0.24/gui_api_tkinter/lib/guiapi/__init__.py
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)     3566 2024-03-29 20:52:06.000000 gui_api_tkinter-0.0.24/gui_api_tkinter/lib/guiapi/gui_api_server.py
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)    10815 2023-12-07 20:17:33.000000 gui_api_tkinter-0.0.24/gui_api_tkinter/lib/guiapi/gui_api_tkinter.py
+drwxrwxr-x   0 arrizza   (1000) arrizza   (1000)        0 2024-05-12 00:15:29.908326 gui_api_tkinter-0.0.24/gui_api_tkinter/lib/harness/
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)        0 2023-03-13 00:13:36.000000 gui_api_tkinter-0.0.24/gui_api_tkinter/lib/harness/__init__.py
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)     5814 2024-03-29 20:52:06.000000 gui_api_tkinter-0.0.24/gui_api_tkinter/lib/harness/client.py
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)    10470 2023-12-07 20:18:06.000000 gui_api_tkinter-0.0.24/gui_api_tkinter/lib/harness/gui_api_harness.py
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)     5301 2023-03-13 00:13:36.000000 gui_api_tkinter-0.0.24/gui_api_tkinter/lib/harness/response.py
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)      900 2023-03-13 00:13:36.000000 gui_api_tkinter-0.0.24/gui_api_tkinter/lib/harness/widget_base.py
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)     2587 2023-03-13 00:13:36.000000 gui_api_tkinter-0.0.24/gui_api_tkinter/lib/harness/widget_click.py
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)     3082 2023-03-13 00:13:36.000000 gui_api_tkinter-0.0.24/gui_api_tkinter/lib/harness/widget_combobox.py
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)     3287 2023-03-13 00:13:36.000000 gui_api_tkinter-0.0.24/gui_api_tkinter/lib/harness/widget_listbox.py
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)     2943 2023-03-13 00:13:36.000000 gui_api_tkinter-0.0.24/gui_api_tkinter/lib/harness/widget_text.py
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)      209 2023-03-13 00:13:36.000000 gui_api_tkinter-0.0.24/gui_api_tkinter/lib/logger_null.py
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)      174 2023-03-13 00:13:36.000000 gui_api_tkinter-0.0.24/gui_api_tkinter/lib/svc.py
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)       27 2024-05-12 00:15:29.000000 gui_api_tkinter-0.0.24/gui_api_tkinter/lib/version.json
+drwxrwxr-x   0 arrizza   (1000) arrizza   (1000)        0 2024-05-12 00:15:29.912327 gui_api_tkinter-0.0.24/gui_api_tkinter.egg-info/
+-rw-r--r--   0 arrizza   (1000) arrizza   (1000)     2630 2024-05-12 00:15:29.000000 gui_api_tkinter-0.0.24/gui_api_tkinter.egg-info/PKG-INFO
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)     2634 2024-05-12 00:15:29.000000 gui_api_tkinter-0.0.24/gui_api_tkinter.egg-info/SOURCES.txt
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)        1 2024-05-12 00:15:29.000000 gui_api_tkinter-0.0.24/gui_api_tkinter.egg-info/dependency_links.txt
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)       36 2024-05-12 00:15:29.000000 gui_api_tkinter-0.0.24/gui_api_tkinter.egg-info/requires.txt
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)       33 2024-05-12 00:15:29.000000 gui_api_tkinter-0.0.24/gui_api_tkinter.egg-info/top_level.txt
+drwxrwxr-x   0 arrizza   (1000) arrizza   (1000)        0 2024-05-12 00:15:29.908326 gui_api_tkinter-0.0.24/sample/
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)        0 2023-03-13 00:13:36.000000 gui_api_tkinter-0.0.24/sample/__init__.py
+drwxrwxr-x   0 arrizza   (1000) arrizza   (1000)        0 2024-05-12 00:15:29.908326 gui_api_tkinter-0.0.24/sample/common/
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)        0 2023-12-08 02:22:31.000000 gui_api_tkinter-0.0.24/sample/common/__init__.py
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)     4106 2024-03-29 20:52:06.000000 gui_api_tkinter-0.0.24/sample/common/cmd_runner.py
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)     1509 2023-03-13 00:13:36.000000 gui_api_tkinter-0.0.24/sample/common/logger.py
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)     2839 2023-03-13 00:13:36.000000 gui_api_tkinter-0.0.24/sample/main.py
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)      621 2024-05-12 00:15:29.916327 gui_api_tkinter-0.0.24/setup.cfg
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)     1472 2024-05-12 00:15:29.000000 gui_api_tkinter-0.0.24/setup.py
+drwxrwxr-x   0 arrizza   (1000) arrizza   (1000)        0 2024-05-12 00:15:29.908326 gui_api_tkinter-0.0.24/tools/
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)        0 2023-03-13 00:13:36.000000 gui_api_tkinter-0.0.24/tools/__init__.py
+drwxrwxr-x   0 arrizza   (1000) arrizza   (1000)        0 2024-05-12 00:15:29.908326 gui_api_tkinter-0.0.24/tools/install/
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)        0 2023-12-07 04:48:04.000000 gui_api_tkinter-0.0.24/tools/install/__init__.py
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)      637 2023-03-13 00:01:54.000000 gui_api_tkinter-0.0.24/tools/loader.py
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)     1402 2024-05-11 21:41:40.000000 gui_api_tkinter-0.0.24/tools/setup_template.py
+drwxrwxr-x   0 arrizza   (1000) arrizza   (1000)        0 2024-05-12 00:15:29.908326 gui_api_tkinter-0.0.24/tools/xplat_utils/
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)       25 2024-02-13 13:56:38.000000 gui_api_tkinter-0.0.24/tools/xplat_utils/__init__.py
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)    11846 2024-03-07 17:23:53.000000 gui_api_tkinter-0.0.24/tools/xplat_utils/cfg.py
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)     2942 2024-03-26 21:36:01.000000 gui_api_tkinter-0.0.24/tools/xplat_utils/do_build.py
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)    29185 2024-05-11 14:21:26.000000 gui_api_tkinter-0.0.24/tools/xplat_utils/do_check.py
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)     2630 2024-03-07 23:16:05.000000 gui_api_tkinter-0.0.24/tools/xplat_utils/do_clean.py
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)     3880 2024-02-26 17:02:19.000000 gui_api_tkinter-0.0.24/tools/xplat_utils/do_coverage.py
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)     5580 2024-02-20 05:18:30.000000 gui_api_tkinter-0.0.24/tools/xplat_utils/do_doc.py
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)     3611 2024-03-09 16:54:42.000000 gui_api_tkinter-0.0.24/tools/xplat_utils/do_lint.py
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)     3388 2024-05-11 14:21:26.000000 gui_api_tkinter-0.0.24/tools/xplat_utils/do_post_ver.py
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)     2460 2024-02-17 03:26:40.000000 gui_api_tkinter-0.0.24/tools/xplat_utils/do_publish.py
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)     1713 2024-03-11 22:17:17.000000 gui_api_tkinter-0.0.24/tools/xplat_utils/do_upload.py
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)     2074 2024-02-26 17:02:19.000000 gui_api_tkinter-0.0.24/tools/xplat_utils/do_ver_info.py
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)     6076 2024-02-26 17:02:19.000000 gui_api_tkinter-0.0.24/tools/xplat_utils/gen_build_info.py
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)     4064 2024-02-26 17:02:19.000000 gui_api_tkinter-0.0.24/tools/xplat_utils/gen_files.py
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)      174 2024-02-17 01:38:07.000000 gui_api_tkinter-0.0.24/tools/xplat_utils/main.py
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)    12926 2024-02-26 17:02:19.000000 gui_api_tkinter-0.0.24/tools/xplat_utils/os_specific.py
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)     1330 2024-03-07 17:23:53.000000 gui_api_tkinter-0.0.24/tools/xplat_utils/svc.py
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)     8201 2024-03-29 17:27:03.000000 gui_api_tkinter-0.0.24/tools/xplat_utils/utils.py
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)     4670 2024-03-07 17:23:53.000000 gui_api_tkinter-0.0.24/tools/xplat_utils/utils_fs.py
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)     5091 2024-04-16 20:36:33.000000 gui_api_tkinter-0.0.24/tools/xplat_utils/utils_logger.py
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)     2938 2024-02-21 00:38:34.000000 gui_api_tkinter-0.0.24/tools/xplat_utils/utils_ps.py
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)     1142 2024-02-13 13:56:38.000000 gui_api_tkinter-0.0.24/tools/xplat_utils/utils_val.py
+drwxrwxr-x   0 arrizza   (1000) arrizza   (1000)        0 2024-05-12 00:15:29.912327 gui_api_tkinter-0.0.24/ver/
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)        0 2023-03-13 00:13:36.000000 gui_api_tkinter-0.0.24/ver/__init__.py
+drwxrwxr-x   0 arrizza   (1000) arrizza   (1000)        0 2024-05-12 00:15:29.912327 gui_api_tkinter-0.0.24/ver/gui/
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)        0 2023-03-13 00:13:36.000000 gui_api_tkinter-0.0.24/ver/gui/__init__.py
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)     1667 2024-02-13 17:34:20.000000 gui_api_tkinter-0.0.24/ver/gui/app.py
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)      713 2023-03-13 00:13:36.000000 gui_api_tkinter-0.0.24/ver/gui/cfg.py
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)      793 2023-03-13 00:13:36.000000 gui_api_tkinter-0.0.24/ver/gui/cli.py
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)      163 2023-12-07 05:10:33.000000 gui_api_tkinter-0.0.24/ver/gui/constants.py
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)      186 2023-12-07 05:10:37.000000 gui_api_tkinter-0.0.24/ver/gui/frame_base.py
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)      172 2023-03-13 00:13:36.000000 gui_api_tkinter-0.0.24/ver/gui/main.py
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)      872 2023-03-13 00:13:36.000000 gui_api_tkinter-0.0.24/ver/gui/model.py
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)      280 2023-03-13 00:13:36.000000 gui_api_tkinter-0.0.24/ver/gui/mvc.py
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)     8440 2023-12-07 05:28:01.000000 gui_api_tkinter-0.0.24/ver/gui/page1_frame.py
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)     5409 2023-12-07 05:05:38.000000 gui_api_tkinter-0.0.24/ver/gui/view.py
+drwxrwxr-x   0 arrizza   (1000) arrizza   (1000)        0 2024-05-12 00:15:29.912327 gui_api_tkinter-0.0.24/ver/helpers/
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)        0 2023-03-13 00:13:36.000000 gui_api_tkinter-0.0.24/ver/helpers/__init__.py
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)     4060 2024-03-29 20:52:06.000000 gui_api_tkinter-0.0.24/ver/helpers/cmd_runner.py
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)      102 2024-05-11 21:41:40.000000 gui_api_tkinter-0.0.24/ver/helpers/gen_report.py
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)     2384 2024-02-13 17:32:34.000000 gui_api_tkinter-0.0.24/ver/helpers/helper.py
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)     1734 2023-12-07 05:24:53.000000 gui_api_tkinter-0.0.24/ver/helpers/logger_file.py
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)      669 2023-12-07 04:56:10.000000 gui_api_tkinter-0.0.24/ver/helpers/logger_mock.py
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)     1517 2023-12-07 05:23:11.000000 gui_api_tkinter-0.0.24/ver/helpers/logger_stdout.py
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)       73 2023-12-07 04:48:04.000000 gui_api_tkinter-0.0.24/ver/helpers/svc.py
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)     2961 2024-05-11 21:41:40.000000 gui_api_tkinter-0.0.24/ver/test_tp001_basic.py
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)     2081 2024-05-11 21:41:40.000000 gui_api_tkinter-0.0.24/ver/test_tp002_no_callback.py
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)     6523 2024-05-11 21:41:40.000000 gui_api_tkinter-0.0.24/ver/test_tp003_click_button.py
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)     4377 2024-05-11 21:41:40.000000 gui_api_tkinter-0.0.24/ver/test_tp004_search.py
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)     1842 2024-05-11 21:41:40.000000 gui_api_tkinter-0.0.24/ver/test_tp005_1client.py
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)     5935 2024-05-11 21:41:40.000000 gui_api_tkinter-0.0.24/ver/test_tp006_info.py
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)     4176 2024-05-11 21:41:40.000000 gui_api_tkinter-0.0.24/ver/test_tp007_menuitem.py
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)     8842 2024-05-11 21:41:40.000000 gui_api_tkinter-0.0.24/ver/test_tp008_entry.py
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)     5010 2024-05-11 21:41:40.000000 gui_api_tkinter-0.0.24/ver/test_tp009_radiobutton.py
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)     8819 2024-05-11 21:41:40.000000 gui_api_tkinter-0.0.24/ver/test_tp010_text.py
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)     9575 2024-05-11 21:41:40.000000 gui_api_tkinter-0.0.24/ver/test_tp011_listbox.py
+-rw-rw-r--   0 arrizza   (1000) arrizza   (1000)     9029 2024-05-11 21:41:40.000000 gui_api_tkinter-0.0.24/ver/test_tp012_combobox.py
```

### Comparing `gui-api-tkinter-0.0.23/LICENSE.txt` & `gui_api_tkinter-0.0.24/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gui-api-tkinter-0.0.23/PKG-INFO` & `gui_api_tkinter-0.0.24/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gui-api-tkinter
-Version: 0.0.23
+Version: 0.0.24
 Summary: Base Class for interacting with a GUI based in tkinter
 Home-page: https://bitbucket.org/arrizza-public/gui-api-tkinter/src/master
 Download-URL: https://bitbucket.org/arrizza-public/gui-api-tkinter/get/master.zip
 Author: JA
 Author-email: cppgent0@gmail.com
 License: MIT
 Keywords: gui,tkinter,test,verification
@@ -12,19 +12,21 @@
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
 Requires-Dist: socket-oneline
 
-# GUI API - tkinter
+website: <https://arrizza.com/python-gui-api-tkinter>
+
+## Summary
 
 This module contains a set of simple base classes that can be
 used for test or verification purposes on GUIs based on Tkinter.
 
 A test harness can connect to this class using a TCPIP socket and
 get the current screen content, press an x,y coordinate, and
 invoke a menu item.
@@ -33,14 +35,19 @@
 gui-api-tkinter server into it. Then a test harness is built
 using gui_api_harness and that is used by pytest (or whatever
 other test driver you wish) to run tests against the GUI.
 
 For a more detailed description of the available commands and
 responses see gui_api.md
 
+## Scripts
+
+* See [Quick Start](https://arrizza.com/user-guide-quick-start) for information on using scripts.
+* See [xplat-utils submodule](https://arrizza.com/xplat-utils) for information on the submodule.
+
 ## Sample code
 
 See the sample directory for a sample client and server. Use
 doit script to run the sample server.
 
     ./doit
```

### Comparing `gui-api-tkinter-0.0.23/README.md` & `gui_api_tkinter-0.0.24/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-# GUI API - tkinter
+website: <https://arrizza.com/python-gui-api-tkinter>
+
+## Summary
 
 This module contains a set of simple base classes that can be
 used for test or verification purposes on GUIs based on Tkinter.
 
 A test harness can connect to this class using a TCPIP socket and
 get the current screen content, press an x,y coordinate, and
 invoke a menu item.
@@ -11,14 +13,19 @@
 gui-api-tkinter server into it. Then a test harness is built
 using gui_api_harness and that is used by pytest (or whatever
 other test driver you wish) to run tests against the GUI.
 
 For a more detailed description of the available commands and
 responses see gui_api.md
 
+## Scripts
+
+* See [Quick Start](https://arrizza.com/user-guide-quick-start) for information on using scripts.
+* See [xplat-utils submodule](https://arrizza.com/xplat-utils) for information on the submodule.
+
 ## Sample code
 
 See the sample directory for a sample client and server. Use
 doit script to run the sample server.
 
     ./doit
```

### Comparing `gui-api-tkinter-0.0.23/gui_api_tkinter/lib/cfg.py` & `gui_api_tkinter-0.0.24/gui_api_tkinter/lib/cfg.py`

 * *Files identical despite different names*

### Comparing `gui-api-tkinter-0.0.23/gui_api_tkinter/lib/constants.py` & `gui_api_tkinter-0.0.24/gui_api_tkinter/lib/constants.py`

 * *Files identical despite different names*

### Comparing `gui-api-tkinter-0.0.23/gui_api_tkinter/lib/guiapi/gui_api_server.py` & `gui_api_tkinter-0.0.24/gui_api_tkinter/lib/guiapi/gui_api_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import json
 import time
-
 from socket_oneline import OnelineServer
 
 from .. import svc
 
 
 # --------------------
 ## Server mainline to communication with the socket server
```

### Comparing `gui-api-tkinter-0.0.23/gui_api_tkinter/lib/guiapi/gui_api_tkinter.py` & `gui_api_tkinter-0.0.24/gui_api_tkinter/lib/guiapi/gui_api_tkinter.py`

 * *Files identical despite different names*

### Comparing `gui-api-tkinter-0.0.23/gui_api_tkinter/lib/harness/client.py` & `gui_api_tkinter-0.0.24/gui_api_tkinter/lib/harness/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import json
 import time
-
 from socket_oneline import OnelineClient
 
 from .. import svc
 
 
 # --------------------
 ## sample Client that wraps the OnelineClient
```

### Comparing `gui-api-tkinter-0.0.23/gui_api_tkinter/lib/harness/gui_api_harness.py` & `gui_api_tkinter-0.0.24/gui_api_tkinter/lib/harness/gui_api_harness.py`

 * *Files identical despite different names*

### Comparing `gui-api-tkinter-0.0.23/gui_api_tkinter/lib/harness/response.py` & `gui_api_tkinter-0.0.24/gui_api_tkinter/lib/harness/response.py`

 * *Files identical despite different names*

### Comparing `gui-api-tkinter-0.0.23/gui_api_tkinter/lib/harness/widget_base.py` & `gui_api_tkinter-0.0.24/gui_api_tkinter/lib/harness/widget_base.py`

 * *Files identical despite different names*

### Comparing `gui-api-tkinter-0.0.23/gui_api_tkinter/lib/harness/widget_click.py` & `gui_api_tkinter-0.0.24/gui_api_tkinter/lib/harness/widget_click.py`

 * *Files identical despite different names*

### Comparing `gui-api-tkinter-0.0.23/gui_api_tkinter/lib/harness/widget_combobox.py` & `gui_api_tkinter-0.0.24/gui_api_tkinter/lib/harness/widget_combobox.py`

 * *Files identical despite different names*

### Comparing `gui-api-tkinter-0.0.23/gui_api_tkinter/lib/harness/widget_listbox.py` & `gui_api_tkinter-0.0.24/gui_api_tkinter/lib/harness/widget_listbox.py`

 * *Files identical despite different names*

### Comparing `gui-api-tkinter-0.0.23/gui_api_tkinter/lib/harness/widget_text.py` & `gui_api_tkinter-0.0.24/gui_api_tkinter/lib/harness/widget_text.py`

 * *Files identical despite different names*

### Comparing `gui-api-tkinter-0.0.23/gui_api_tkinter.egg-info/PKG-INFO` & `gui_api_tkinter-0.0.24/gui_api_tkinter.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gui-api-tkinter
-Version: 0.0.23
+Version: 0.0.24
 Summary: Base Class for interacting with a GUI based in tkinter
 Home-page: https://bitbucket.org/arrizza-public/gui-api-tkinter/src/master
 Download-URL: https://bitbucket.org/arrizza-public/gui-api-tkinter/get/master.zip
 Author: JA
 Author-email: cppgent0@gmail.com
 License: MIT
 Keywords: gui,tkinter,test,verification
@@ -12,19 +12,21 @@
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
 Requires-Dist: socket-oneline
 
-# GUI API - tkinter
+website: <https://arrizza.com/python-gui-api-tkinter>
+
+## Summary
 
 This module contains a set of simple base classes that can be
 used for test or verification purposes on GUIs based on Tkinter.
 
 A test harness can connect to this class using a TCPIP socket and
 get the current screen content, press an x,y coordinate, and
 invoke a menu item.
@@ -33,14 +35,19 @@
 gui-api-tkinter server into it. Then a test harness is built
 using gui_api_harness and that is used by pytest (or whatever
 other test driver you wish) to run tests against the GUI.
 
 For a more detailed description of the available commands and
 responses see gui_api.md
 
+## Scripts
+
+* See [Quick Start](https://arrizza.com/user-guide-quick-start) for information on using scripts.
+* See [xplat-utils submodule](https://arrizza.com/xplat-utils) for information on the submodule.
+
 ## Sample code
 
 See the sample directory for a sample client and server. Use
 doit script to run the sample server.
 
     ./doit
```

### Comparing `gui-api-tkinter-0.0.23/sample/common/cmd_runner.py` & `gui_api_tkinter-0.0.24/sample/common/cmd_runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
+import psutil
 import subprocess
 import threading
 import time
 
-import psutil
-
 
 # --------------------
 ## holds various functions to run OS processes
 class CmdRunner:
     # --------------------
     ## constructor
     #
```

### Comparing `gui-api-tkinter-0.0.23/sample/common/logger.py` & `gui_api_tkinter-0.0.24/sample/common/logger.py`

 * *Files identical despite different names*

### Comparing `gui-api-tkinter-0.0.23/sample/main.py` & `gui_api_tkinter-0.0.24/sample/main.py`

 * *Files identical despite different names*

### Comparing `gui-api-tkinter-0.0.23/setup.cfg` & `gui_api_tkinter-0.0.24/setup.cfg`

 * *Files identical despite different names*

### Comparing `gui-api-tkinter-0.0.23/setup.py` & `gui_api_tkinter-0.0.24/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from pathlib import Path
 
 from setuptools import find_packages
 from setuptools import setup
 
-print('     setup: version:  v0.0.23')
+print('     setup: version:  v0.0.24')
 print('     setup: module :  gui_api_tkinter')
 
 # @formatter:off
 setup(
     description='Base Class for interacting with a GUI based in tkinter',
     keywords=['gui', 'tkinter', 'test', 'verification'],
     install_requires=[
-        'pytest-ver',
+        'medver-pytest',
         'pytest',
         'socket-oneline',
     ],
     classifiers=[
         # TODO update as needed
         # Choose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable"
         'Development Status :: 2 - Pre-Alpha',
@@ -27,15 +27,15 @@
     ],
 
     # common attributes from here on
     name='gui-api-tkinter',
     packages=find_packages(include='./gui_api_tkinter*', ),
     include_package_data=True,
     exclude_package_data={'./gui_api_tkinter/lib': ['.gitignore']},
-    version='0.0.23',
+    version='0.0.24',
     license='MIT',
     long_description=(Path(__file__).parent / 'README.md').read_text(),
     long_description_content_type='text/markdown',
     author='JA',
     author_email='cppgent0@gmail.com',
     url='https://bitbucket.org/arrizza-public/gui-api-tkinter/src/master',
     download_url='https://bitbucket.org/arrizza-public/gui-api-tkinter/get/master.zip',
```

### Comparing `gui-api-tkinter-0.0.23/tools/debug_logger.py` & `gui_api_tkinter-0.0.24/tools/xplat_utils/utils_logger.py`

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

### Comparing `gui-api-tkinter-0.0.23/tools/loader.py` & `gui_api_tkinter-0.0.24/tools/loader.py`

 * *Files identical despite different names*

### Comparing `gui-api-tkinter-0.0.23/tools/setup_template.py` & `gui_api_tkinter-0.0.24/tools/setup_template.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 print('     setup: module :  $$mod_dir_name$$')
 
 # @formatter:off
 setup(
     description='Base Class for interacting with a GUI based in tkinter',
     keywords=['gui', 'tkinter', 'test', 'verification'],
     install_requires=[
-        'pytest-ver',
+        'medver-pytest',
         'pytest',
         'socket-oneline',
     ],
     classifiers=[
         # TODO update as needed
         # Choose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable"
         'Development Status :: 2 - Pre-Alpha',
```

### Comparing `gui-api-tkinter-0.0.23/ver/gui/app.py` & `gui_api_tkinter-0.0.24/ver/gui/app.py`

 * *Files identical despite different names*

### Comparing `gui-api-tkinter-0.0.23/ver/gui/cfg.py` & `gui_api_tkinter-0.0.24/ver/gui/cfg.py`

 * *Files identical despite different names*

### Comparing `gui-api-tkinter-0.0.23/ver/gui/cli.py` & `gui_api_tkinter-0.0.24/ver/gui/cli.py`

 * *Files identical despite different names*

### Comparing `gui-api-tkinter-0.0.23/ver/gui/model.py` & `gui_api_tkinter-0.0.24/ver/gui/model.py`

 * *Files identical despite different names*

### Comparing `gui-api-tkinter-0.0.23/ver/gui/page1_frame.py` & `gui_api_tkinter-0.0.24/ver/gui/page1_frame.py`

 * *Files identical despite different names*

### Comparing `gui-api-tkinter-0.0.23/ver/gui/view.py` & `gui_api_tkinter-0.0.24/ver/gui/view.py`

 * *Files identical despite different names*

### Comparing `gui-api-tkinter-0.0.23/ver/helpers/cmd_runner.py` & `gui_api_tkinter-0.0.24/ver/helpers/cmd_runner.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
+import psutil
 import subprocess
 import threading
 import time
 
-import psutil
-
 from ver.helpers import svc
 
 
 # --------------------
 ## holds various functions to run OS processes
 class CmdRunner:
     # --------------------
```

### Comparing `gui-api-tkinter-0.0.23/ver/helpers/helper.py` & `gui_api_tkinter-0.0.24/ver/helpers/helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import sys
 import time
 
 from gui_api_tkinter.lib.harness.gui_api_harness import GuiApiHarness
-from tools.debug_logger import DebugLogger as logger
+from tools.xplat_utils.utils_logger import UtilsLogger as logger
 from ver.helpers import svc
 from ver.helpers.cmd_runner import CmdRunner
 from ver.helpers.logger_mock import Logger
 
 
 # --------------------
 class Helper:
```

### Comparing `gui-api-tkinter-0.0.23/ver/helpers/logger_file.py` & `gui_api_tkinter-0.0.24/ver/helpers/logger_file.py`

 * *Files identical despite different names*

### Comparing `gui-api-tkinter-0.0.23/ver/helpers/logger_mock.py` & `gui_api_tkinter-0.0.24/ver/helpers/logger_mock.py`

 * *Files identical despite different names*

### Comparing `gui-api-tkinter-0.0.23/ver/helpers/logger_stdout.py` & `gui_api_tkinter-0.0.24/ver/helpers/logger_stdout.py`

 * *Files identical despite different names*

### Comparing `gui-api-tkinter-0.0.23/ver/test_tp001_basic.py` & `gui_api_tkinter-0.0.24/ver/test_tp001_basic.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import unittest
-
-from pytest_ver import pth
+from medver_pytest import pth
 
 from ver.helpers import svc
 from ver.helpers.helper import Helper
 
 
 # -------------------
 class TestTp001(unittest.TestCase):
```

### Comparing `gui-api-tkinter-0.0.23/ver/test_tp002_no_callback.py` & `gui_api_tkinter-0.0.24/ver/test_tp002_no_callback.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import unittest
-
-from pytest_ver import pth
+from medver_pytest import pth
 
 from gui_api_tkinter.lib.constants import Constants
 from ver.helpers import svc
 from ver.helpers.helper import Helper
 
 
 # -------------------
```

### Comparing `gui-api-tkinter-0.0.23/ver/test_tp003_click_button.py` & `gui_api_tkinter-0.0.24/ver/test_tp003_click_button.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import unittest
-
-from pytest_ver import pth
+from medver_pytest import pth
 
 from ver.helpers import svc
 from ver.helpers.helper import Helper
 
 
 # -------------------
 class TestTp003(unittest.TestCase):
```

### Comparing `gui-api-tkinter-0.0.23/ver/test_tp004_search.py` & `gui_api_tkinter-0.0.24/ver/test_tp004_search.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import unittest
-
-from pytest_ver import pth
+from medver_pytest import pth
 
 from ver.helpers import svc
 from ver.helpers.helper import Helper
 
 
 # -------------------
 class TestTp004(unittest.TestCase):
```

### Comparing `gui-api-tkinter-0.0.23/ver/test_tp005_1client.py` & `gui_api_tkinter-0.0.24/ver/test_tp005_1client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import unittest
-
-from pytest_ver import pth
+from medver_pytest import pth
 
 from ver.helpers import svc
 from ver.helpers.helper import Helper
 
 
 # -------------------
 class TestTp005(unittest.TestCase):
```

### Comparing `gui-api-tkinter-0.0.23/ver/test_tp006_info.py` & `gui_api_tkinter-0.0.24/ver/test_tp006_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import unittest
-
-from pytest_ver import pth
+from medver_pytest import pth
 
 from ver.helpers import svc
 from ver.helpers.helper import Helper
 
 
 # -------------------
 class TestTp006(unittest.TestCase):
```

### Comparing `gui-api-tkinter-0.0.23/ver/test_tp007_menuitem.py` & `gui_api_tkinter-0.0.24/ver/test_tp007_menuitem.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import unittest
-
-from pytest_ver import pth
+from medver_pytest import pth
 
 from ver.helpers import svc
 from ver.helpers.helper import Helper
 
 
 # -------------------
 class TestTp007(unittest.TestCase):
```

### Comparing `gui-api-tkinter-0.0.23/ver/test_tp008_entry.py` & `gui_api_tkinter-0.0.24/ver/test_tp008_entry.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import unittest
-
-from pytest_ver import pth
+from medver_pytest import pth
 
 from ver.helpers import svc
 from ver.helpers.helper import Helper
 
 
 # -------------------
 class TestTp008(unittest.TestCase):
```

### Comparing `gui-api-tkinter-0.0.23/ver/test_tp009_radiobutton.py` & `gui_api_tkinter-0.0.24/ver/test_tp009_radiobutton.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import unittest
-
-from pytest_ver import pth
+from medver_pytest import pth
 
 from ver.helpers import svc
 from ver.helpers.helper import Helper
 
 
 # -------------------
 class TestTp009(unittest.TestCase):
```

### Comparing `gui-api-tkinter-0.0.23/ver/test_tp010_text.py` & `gui_api_tkinter-0.0.24/ver/test_tp010_text.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import unittest
-
-from pytest_ver import pth
+from medver_pytest import pth
 
 from ver.helpers import svc
 from ver.helpers.helper import Helper
 
 
 # -------------------
 class TestTp010(unittest.TestCase):
```

### Comparing `gui-api-tkinter-0.0.23/ver/test_tp011_listbox.py` & `gui_api_tkinter-0.0.24/ver/test_tp011_listbox.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import unittest
-
-from pytest_ver import pth
+from medver_pytest import pth
 
 from ver.helpers import svc
 from ver.helpers.helper import Helper
 
 
 # -------------------
 class TestTp011(unittest.TestCase):
```

### Comparing `gui-api-tkinter-0.0.23/ver/test_tp012_combobox.py` & `gui_api_tkinter-0.0.24/ver/test_tp012_combobox.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import unittest
-
-from pytest_ver import pth
+from medver_pytest import pth
 
 from ver.helpers import svc
 from ver.helpers.helper import Helper
 
 
 # -------------------
 class TestTp012(unittest.TestCase):
```

