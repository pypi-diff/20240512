# Comparing `tmp/TDSR-UWB-1.535.tar.gz` & `tmp/TDSR-UWB-1.536.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TDSR-UWB-1.535.tar", last modified: Fri May 10 02:30:25 2024, max compression
+gzip compressed data, was "TDSR-UWB-1.536.tar", last modified: Sun May 12 20:15:36 2024, max compression
```

## Comparing `TDSR-UWB-1.535.tar` & `TDSR-UWB-1.536.tar`

### file list

```diff
@@ -1,100 +1,100 @@
-drwxrwxr-x   0 senter    (1000) senter    (1000)        0 2024-05-10 02:30:25.338326 TDSR-UWB-1.535/
--rw-rw-r--   0 senter    (1000) senter    (1000)       74 2024-05-09 23:00:07.000000 TDSR-UWB-1.535/LICENSE.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       37 2024-05-09 21:21:05.000000 TDSR-UWB-1.535/MANIFEST.in
--rw-rw-r--   0 senter    (1000) senter    (1000)      748 2024-05-10 02:30:25.338326 TDSR-UWB-1.535/PKG-INFO
--rw-rw-r--   0 senter    (1000) senter    (1000)       93 2024-05-09 23:01:32.000000 TDSR-UWB-1.535/README.md
-drwxrwxr-x   0 senter    (1000) senter    (1000)        0 2024-05-10 02:30:25.334326 TDSR-UWB-1.535/TDSR-UWB/
-drwxrwxr-x   0 senter    (1000) senter    (1000)        0 2024-05-10 02:30:25.334326 TDSR-UWB-1.535/TDSR-UWB/TDSR_Support/
-drwxrwxr-x   0 senter    (1000) senter    (1000)        0 2024-05-10 02:30:25.338326 TDSR-UWB-1.535/TDSR-UWB/TDSR_Support/JsonDoc/
--rw-rw-r--   0 senter    (1000) senter    (1000)     6148 2023-03-30 19:11:25.000000 TDSR-UWB-1.535/TDSR-UWB/TDSR_Support/JsonDoc/.DS_Store
--rw-rw-r--   0 senter    (1000) senter    (1000)      161 2023-03-30 02:12:00.000000 TDSR-UWB-1.535/TDSR-UWB/TDSR_Support/JsonDoc/.txt
-drwxrwxr-x   0 senter    (1000) senter    (1000)        0 2024-05-10 02:30:25.338326 TDSR-UWB-1.535/TDSR-UWB/TDSR_Support/JsonDoc/.vscode/
--rw-rw-r--   0 senter    (1000) senter    (1000)      536 2023-03-02 20:09:11.000000 TDSR-UWB-1.535/TDSR-UWB/TDSR_Support/JsonDoc/.vscode/launch.json
--rw-rw-r--   0 senter    (1000) senter    (1000)     9479 2023-02-26 18:51:27.000000 TDSR-UWB-1.535/TDSR-UWB/TDSR_Support/JsonDoc/API.md
--rw-rw-r--   0 senter    (1000) senter    (1000)     5515 2022-12-23 02:15:12.000000 TDSR-UWB-1.535/TDSR-UWB/TDSR_Support/JsonDoc/API.template.md
--rw-rw-r--   0 senter    (1000) senter    (1000)     5563 2022-12-23 02:08:30.000000 TDSR-UWB-1.535/TDSR-UWB/TDSR_Support/JsonDoc/APIwith_cat_template.md
--rw-rw-r--   0 senter    (1000) senter    (1000)       45 2023-03-30 02:12:00.000000 TDSR-UWB-1.535/TDSR-UWB/TDSR_Support/JsonDoc/DATA_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)      124 2023-03-30 02:12:00.000000 TDSR-UWB-1.535/TDSR-UWB/TDSR_Support/JsonDoc/DATA_INFO.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)      144 2023-08-10 03:26:43.000000 TDSR-UWB-1.535/TDSR-UWB/TDSR_Support/JsonDoc/DATA_REQUEST.txt
-drwxrwxr-x   0 senter    (1000) senter    (1000)        0 2024-05-10 02:30:25.338326 TDSR-UWB-1.535/TDSR-UWB/TDSR_Support/JsonDoc/Doc/
--rw-rw-r--   0 senter    (1000) senter    (1000)    12524 2022-10-06 21:41:33.000000 TDSR-UWB-1.535/TDSR-UWB/TDSR_Support/JsonDoc/Doc/TDSR_logo_250x134.png
--rw-rw-r--   0 senter    (1000) senter    (1000)      405 2023-03-30 02:12:00.000000 TDSR-UWB-1.535/TDSR-UWB/TDSR_Support/JsonDoc/NETWORKING_GET_SLOT_MAP_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       50 2023-03-30 02:12:00.000000 TDSR-UWB-1.535/TDSR-UWB/TDSR_Support/JsonDoc/NETWORKING_GET_SLOT_MAP_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)      411 2023-03-30 02:12:35.000000 TDSR-UWB-1.535/TDSR-UWB/TDSR_Support/JsonDoc/NETWORKING_GET_STATS_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       47 2023-03-30 02:12:00.000000 TDSR-UWB-1.535/TDSR-UWB/TDSR_Support/JsonDoc/NETWORKING_GET_STATS_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       64 2023-03-30 02:12:00.000000 TDSR-UWB-1.535/TDSR-UWB/TDSR_Support/JsonDoc/NETWORKING_SET_SLOT_MAP_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)      405 2023-03-30 02:12:00.000000 TDSR-UWB-1.535/TDSR-UWB/TDSR_Support/JsonDoc/NETWORKING_SET_SLOT_MAP_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)      111 2023-05-16 19:39:21.000000 TDSR-UWB-1.535/TDSR-UWB/TDSR_Support/JsonDoc/NET_DATA_QUEUE_STATUS_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       93 2023-05-16 19:38:24.000000 TDSR-UWB-1.535/TDSR-UWB/TDSR_Support/JsonDoc/NET_DATA_QUEUE_STATUS_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       61 2024-03-13 14:34:07.000000 TDSR-UWB-1.535/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_APPLY_PRESET_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       91 2024-03-13 02:20:50.000000 TDSR-UWB-1.535/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_APPLY_PRESET_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       62 2024-03-13 14:31:51.000000 TDSR-UWB-1.535/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_DELETE_PRESET_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       75 2024-03-13 02:21:52.000000 TDSR-UWB-1.535/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_DELETE_PRESET_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       75 2024-03-16 16:10:28.000000 TDSR-UWB-1.535/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_ACTIVE_PRESET_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       51 2024-03-16 16:10:10.000000 TDSR-UWB-1.535/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_ACTIVE_PRESET_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)      228 2023-03-30 02:12:00.000000 TDSR-UWB-1.535/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_CONFIG_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       57 2023-03-30 02:12:00.000000 TDSR-UWB-1.535/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_CONFIG_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       44 2023-03-30 02:12:00.000000 TDSR-UWB-1.535/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_CONNECT_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       41 2023-03-30 02:12:00.000000 TDSR-UWB-1.535/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_INFO_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       41 2023-03-30 02:12:00.000000 TDSR-UWB-1.535/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_INFO_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)      143 2024-03-13 14:30:56.000000 TDSR-UWB-1.535/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_IP_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       40 2024-03-13 01:42:44.000000 TDSR-UWB-1.535/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_IP_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       77 2023-03-30 02:12:00.000000 TDSR-UWB-1.535/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_NODE_CONFIG_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       48 2023-03-30 02:12:00.000000 TDSR-UWB-1.535/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_NODE_CONFIG_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)      379 2024-03-14 17:35:25.000000 TDSR-UWB-1.535/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_PRESET_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       72 2024-03-14 17:30:36.000000 TDSR-UWB-1.535/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_PRESET_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)      120 2023-05-15 23:46:31.000000 TDSR-UWB-1.535/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_STATE_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       42 2023-03-30 02:12:00.000000 TDSR-UWB-1.535/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_STATE_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)      550 2023-03-30 02:12:00.000000 TDSR-UWB-1.535/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_STATS_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       40 2022-12-20 14:51:26.000000 TDSR-UWB-1.535/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_STATS_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)      136 2023-09-28 14:06:18.000000 TDSR-UWB-1.535/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_TUNING_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       43 2023-09-28 14:06:22.000000 TDSR-UWB-1.535/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_TUNING_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)      173 2024-03-13 14:33:30.000000 TDSR-UWB-1.535/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_LIST_PRESETS_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       46 2024-03-13 02:21:17.000000 TDSR-UWB-1.535/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_LIST_PRESETS_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       61 2023-03-30 02:12:00.000000 TDSR-UWB-1.535/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_MESSAGE_ERROR.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       53 2023-03-30 02:12:00.000000 TDSR-UWB-1.535/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_REBOOT_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       39 2023-03-30 02:12:00.000000 TDSR-UWB-1.535/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_REBOOT_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       60 2023-03-30 02:12:00.000000 TDSR-UWB-1.535/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_RESET_FACTORY_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       46 2023-03-30 02:12:00.000000 TDSR-UWB-1.535/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_RESET_FACTORY_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       60 2024-03-13 14:32:21.000000 TDSR-UWB-1.535/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SAVE_PRESET_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       87 2024-03-13 02:21:36.000000 TDSR-UWB-1.535/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SAVE_PRESET_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       57 2023-03-30 02:12:00.000000 TDSR-UWB-1.535/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_CONFIG_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)      228 2023-03-30 02:12:00.000000 TDSR-UWB-1.535/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_CONFIG_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)      138 2023-03-30 02:12:00.000000 TDSR-UWB-1.535/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_CONNECT_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       55 2024-03-13 14:35:17.000000 TDSR-UWB-1.535/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_IP_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)      116 2024-03-13 02:22:22.000000 TDSR-UWB-1.535/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_IP_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       62 2023-03-30 02:12:00.000000 TDSR-UWB-1.535/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_NODE_CONFIG_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       77 2023-03-30 02:12:00.000000 TDSR-UWB-1.535/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_NODE_CONFIG_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       56 2023-03-30 02:12:00.000000 TDSR-UWB-1.535/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_STATE_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)      184 2023-03-30 02:12:00.000000 TDSR-UWB-1.535/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_STATE_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       48 2023-03-30 02:12:00.000000 TDSR-UWB-1.535/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_STATS_CLEAR_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       48 2023-03-30 02:12:00.000000 TDSR-UWB-1.535/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_STATS_CLEAR_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       57 2023-09-28 14:06:26.000000 TDSR-UWB-1.535/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_TUNING_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)      136 2023-09-28 14:06:29.000000 TDSR-UWB-1.535/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_TUNING_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)      348 2023-03-30 02:12:00.000000 TDSR-UWB-1.535/TDSR-UWB/TDSR_Support/JsonDoc/RANGE_INFO.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       57 2023-03-30 02:12:00.000000 TDSR-UWB-1.535/TDSR-UWB/TDSR_Support/JsonDoc/RANGE_SEND_RANGE_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       81 2023-05-16 19:37:46.000000 TDSR-UWB-1.535/TDSR-UWB/TDSR_Support/JsonDoc/RANGE_SEND_RANGE_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)    12521 2023-03-30 01:57:06.000000 TDSR-UWB-1.535/TDSR-UWB/TDSR_Support/JsonDoc/networking.md
--rw-rw-r--   0 senter    (1000) senter    (1000)   107545 2023-03-30 01:57:24.000000 TDSR-UWB-1.535/TDSR-UWB/TDSR_Support/JsonDoc/networking.pdf
--rw-rw-r--   0 senter    (1000) senter    (1000)     9971 2023-03-30 01:57:02.000000 TDSR-UWB-1.535/TDSR-UWB/TDSR_Support/JsonDoc/networking.template.md
--rw-rw-r--   0 senter    (1000) senter    (1000)     6747 2023-03-04 15:21:05.000000 TDSR-UWB-1.535/TDSR-UWB/TDSR_Support/JsonDoc/networking_.md
--rw-rw-r--   0 senter    (1000) senter    (1000)      157 2022-12-08 14:50:04.000000 TDSR-UWB-1.535/TDSR-UWB/TDSR_Support/JsonDoc/processJSONFiles.sh
--rw-rw-r--   0 senter    (1000) senter    (1000)     1097 2023-03-02 20:30:55.000000 TDSR-UWB-1.535/TDSR-UWB/TDSR_Support/JsonDoc/updateReadme.py
--rw-rw-r--   0 senter    (1000) senter    (1000)   243991 2024-05-10 02:19:06.000000 TDSR-UWB-1.535/TDSR-UWB/TDSR_Support/TDSR_PW_GUI.py
--rw-rw-r--   0 senter    (1000) senter    (1000)     6230 2024-05-10 02:19:20.000000 TDSR-UWB-1.535/TDSR-UWB/TDSR_Support/TDSR_logging.py
--rw-rw-r--   0 senter    (1000) senter    (1000)    14174 2024-05-10 02:24:28.000000 TDSR-UWB-1.535/TDSR-UWB/TDSR_Support/TDSR_radioAPI.py
--rw-rw-r--   0 senter    (1000) senter    (1000)    25037 2024-05-10 02:28:58.000000 TDSR-UWB-1.535/TDSR-UWB/TDSR_Support/TDSR_radioConnection.py
--rw-rw-r--   0 senter    (1000) senter    (1000)    80999 2024-05-10 02:25:23.000000 TDSR-UWB-1.535/TDSR-UWB/TDSR_Support/TDSR_radioControl.py
--rw-rw-r--   0 senter    (1000) senter    (1000)     3825 2024-05-10 02:19:01.000000 TDSR-UWB-1.535/TDSR-UWB/TDSR_Support/TDSR_settings.py
--rw-rw-r--   0 senter    (1000) senter    (1000)        0 2024-05-08 17:38:57.000000 TDSR-UWB-1.535/TDSR-UWB/TDSR_Support/__init__.py
--rw-rw-r--   0 senter    (1000) senter    (1000)     2912 2022-12-27 01:25:43.000000 TDSR-UWB-1.535/TDSR-UWB/TDSR_Support/crc16.py
--rw-rw-r--   0 senter    (1000) senter    (1000)     2121 2024-04-15 16:20:28.000000 TDSR-UWB-1.535/TDSR-UWB/TDSR_Support/logReader.py
--rw-rw-r--   0 senter    (1000) senter    (1000)      376 2024-04-15 16:19:41.000000 TDSR-UWB-1.535/TDSR-UWB/TDSR_Support/logReader_Minimal.py
-drwxrwxr-x   0 senter    (1000) senter    (1000)        0 2024-05-10 02:30:25.338326 TDSR-UWB-1.535/TDSR-UWB/TDSR_UWB.egg-info/
--rw-rw-r--   0 senter    (1000) senter    (1000)      748 2024-05-10 02:30:25.000000 TDSR-UWB-1.535/TDSR-UWB/TDSR_UWB.egg-info/PKG-INFO
--rw-rw-r--   0 senter    (1000) senter    (1000)     4735 2024-05-10 02:30:25.000000 TDSR-UWB-1.535/TDSR-UWB/TDSR_UWB.egg-info/SOURCES.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)        1 2024-05-10 02:30:25.000000 TDSR-UWB-1.535/TDSR-UWB/TDSR_UWB.egg-info/dependency_links.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       29 2024-05-10 02:30:25.000000 TDSR-UWB-1.535/TDSR-UWB/TDSR_UWB.egg-info/requires.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       13 2024-05-10 02:30:25.000000 TDSR-UWB-1.535/TDSR-UWB/TDSR_UWB.egg-info/top_level.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       38 2024-05-10 02:30:25.338326 TDSR-UWB-1.535/setup.cfg
--rw-rw-r--   0 senter    (1000) senter    (1000)     7654 2024-05-10 02:14:11.000000 TDSR-UWB-1.535/setup.py
+drwxrwxr-x   0 senter    (1000) senter    (1000)        0 2024-05-12 20:15:36.647590 TDSR-UWB-1.536/
+-rw-rw-r--   0 senter    (1000) senter    (1000)       74 2024-05-09 23:00:07.000000 TDSR-UWB-1.536/LICENSE.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       37 2024-05-09 21:21:05.000000 TDSR-UWB-1.536/MANIFEST.in
+-rw-rw-r--   0 senter    (1000) senter    (1000)      748 2024-05-12 20:15:36.647590 TDSR-UWB-1.536/PKG-INFO
+-rw-rw-r--   0 senter    (1000) senter    (1000)       93 2024-05-09 23:01:32.000000 TDSR-UWB-1.536/README.md
+drwxrwxr-x   0 senter    (1000) senter    (1000)        0 2024-05-12 20:15:36.643590 TDSR-UWB-1.536/TDSR-UWB/
+drwxrwxr-x   0 senter    (1000) senter    (1000)        0 2024-05-12 20:15:36.643590 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/
+drwxrwxr-x   0 senter    (1000) senter    (1000)        0 2024-05-12 20:15:36.647590 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/
+-rw-rw-r--   0 senter    (1000) senter    (1000)     6148 2023-03-30 19:11:25.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/.DS_Store
+-rw-rw-r--   0 senter    (1000) senter    (1000)      161 2023-03-30 02:12:00.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/.txt
+drwxrwxr-x   0 senter    (1000) senter    (1000)        0 2024-05-12 20:15:36.647590 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/.vscode/
+-rw-rw-r--   0 senter    (1000) senter    (1000)      536 2023-03-02 20:09:11.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/.vscode/launch.json
+-rw-rw-r--   0 senter    (1000) senter    (1000)     9479 2023-02-26 18:51:27.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/API.md
+-rw-rw-r--   0 senter    (1000) senter    (1000)     5515 2022-12-23 02:15:12.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/API.template.md
+-rw-rw-r--   0 senter    (1000) senter    (1000)     5563 2022-12-23 02:08:30.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/APIwith_cat_template.md
+-rw-rw-r--   0 senter    (1000) senter    (1000)       45 2023-03-30 02:12:00.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/DATA_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)      124 2023-03-30 02:12:00.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/DATA_INFO.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)      144 2023-08-10 03:26:43.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/DATA_REQUEST.txt
+drwxrwxr-x   0 senter    (1000) senter    (1000)        0 2024-05-12 20:15:36.647590 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/Doc/
+-rw-rw-r--   0 senter    (1000) senter    (1000)    12524 2022-10-06 21:41:33.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/Doc/TDSR_logo_250x134.png
+-rw-rw-r--   0 senter    (1000) senter    (1000)      405 2023-03-30 02:12:00.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/NETWORKING_GET_SLOT_MAP_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       50 2023-03-30 02:12:00.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/NETWORKING_GET_SLOT_MAP_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)      411 2023-03-30 02:12:35.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/NETWORKING_GET_STATS_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       47 2023-03-30 02:12:00.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/NETWORKING_GET_STATS_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       64 2023-03-30 02:12:00.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/NETWORKING_SET_SLOT_MAP_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)      405 2023-03-30 02:12:00.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/NETWORKING_SET_SLOT_MAP_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)      111 2023-05-16 19:39:21.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/NET_DATA_QUEUE_STATUS_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       93 2023-05-16 19:38:24.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/NET_DATA_QUEUE_STATUS_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       61 2024-03-13 14:34:07.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_APPLY_PRESET_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       91 2024-03-13 02:20:50.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_APPLY_PRESET_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       62 2024-03-13 14:31:51.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_DELETE_PRESET_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       75 2024-03-13 02:21:52.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_DELETE_PRESET_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       75 2024-03-16 16:10:28.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_ACTIVE_PRESET_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       51 2024-03-16 16:10:10.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_ACTIVE_PRESET_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)      228 2023-03-30 02:12:00.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_CONFIG_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       57 2023-03-30 02:12:00.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_CONFIG_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       44 2023-03-30 02:12:00.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_CONNECT_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       41 2023-03-30 02:12:00.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_INFO_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       41 2023-03-30 02:12:00.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_INFO_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)      143 2024-03-13 14:30:56.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_IP_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       40 2024-03-13 01:42:44.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_IP_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       77 2023-03-30 02:12:00.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_NODE_CONFIG_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       48 2023-03-30 02:12:00.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_NODE_CONFIG_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)      379 2024-03-14 17:35:25.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_PRESET_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       72 2024-03-14 17:30:36.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_PRESET_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)      120 2023-05-15 23:46:31.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_STATE_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       42 2023-03-30 02:12:00.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_STATE_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)      550 2023-03-30 02:12:00.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_STATS_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       40 2022-12-20 14:51:26.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_STATS_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)      136 2023-09-28 14:06:18.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_TUNING_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       43 2023-09-28 14:06:22.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_TUNING_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)      173 2024-03-13 14:33:30.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_LIST_PRESETS_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       46 2024-03-13 02:21:17.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_LIST_PRESETS_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       61 2023-03-30 02:12:00.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_MESSAGE_ERROR.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       53 2023-03-30 02:12:00.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_REBOOT_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       39 2023-03-30 02:12:00.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_REBOOT_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       60 2023-03-30 02:12:00.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_RESET_FACTORY_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       46 2023-03-30 02:12:00.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_RESET_FACTORY_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       60 2024-03-13 14:32:21.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SAVE_PRESET_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       87 2024-03-13 02:21:36.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SAVE_PRESET_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       57 2023-03-30 02:12:00.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_CONFIG_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)      228 2023-03-30 02:12:00.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_CONFIG_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)      138 2023-03-30 02:12:00.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_CONNECT_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       55 2024-03-13 14:35:17.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_IP_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)      116 2024-03-13 02:22:22.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_IP_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       62 2023-03-30 02:12:00.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_NODE_CONFIG_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       77 2023-03-30 02:12:00.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_NODE_CONFIG_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       56 2023-03-30 02:12:00.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_STATE_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)      184 2023-03-30 02:12:00.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_STATE_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       48 2023-03-30 02:12:00.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_STATS_CLEAR_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       48 2023-03-30 02:12:00.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_STATS_CLEAR_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       57 2023-09-28 14:06:26.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_TUNING_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)      136 2023-09-28 14:06:29.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_TUNING_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)      348 2023-03-30 02:12:00.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/RANGE_INFO.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       57 2023-03-30 02:12:00.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/RANGE_SEND_RANGE_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       81 2023-05-16 19:37:46.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/RANGE_SEND_RANGE_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)    12521 2023-03-30 01:57:06.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/networking.md
+-rw-rw-r--   0 senter    (1000) senter    (1000)   107545 2023-03-30 01:57:24.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/networking.pdf
+-rw-rw-r--   0 senter    (1000) senter    (1000)     9971 2023-03-30 01:57:02.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/networking.template.md
+-rw-rw-r--   0 senter    (1000) senter    (1000)     6747 2023-03-04 15:21:05.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/networking_.md
+-rw-rw-r--   0 senter    (1000) senter    (1000)      157 2022-12-08 14:50:04.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/processJSONFiles.sh
+-rw-rw-r--   0 senter    (1000) senter    (1000)     1097 2023-03-02 20:30:55.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/updateReadme.py
+-rw-rw-r--   0 senter    (1000) senter    (1000)   250067 2024-05-12 20:07:11.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/TDSR_PW_GUI.py
+-rw-rw-r--   0 senter    (1000) senter    (1000)     6230 2024-05-10 15:18:23.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/TDSR_logging.py
+-rw-rw-r--   0 senter    (1000) senter    (1000)    14320 2024-05-12 17:20:28.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/TDSR_radioAPI.py
+-rw-rw-r--   0 senter    (1000) senter    (1000)    15138 2024-05-12 20:04:54.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/TDSR_radioConnection.py
+-rw-rw-r--   0 senter    (1000) senter    (1000)    82001 2024-05-12 20:06:04.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/TDSR_radioControl.py
+-rw-rw-r--   0 senter    (1000) senter    (1000)     3843 2024-05-11 19:59:04.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/TDSR_settings.py
+-rw-rw-r--   0 senter    (1000) senter    (1000)        0 2024-05-08 17:38:57.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/__init__.py
+-rw-rw-r--   0 senter    (1000) senter    (1000)     2912 2022-12-27 01:25:43.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/crc16.py
+-rw-rw-r--   0 senter    (1000) senter    (1000)     2121 2024-04-15 16:20:28.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/logReader.py
+-rw-rw-r--   0 senter    (1000) senter    (1000)      376 2024-04-15 16:19:41.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/logReader_Minimal.py
+drwxrwxr-x   0 senter    (1000) senter    (1000)        0 2024-05-12 20:15:36.647590 TDSR-UWB-1.536/TDSR-UWB/TDSR_UWB.egg-info/
+-rw-rw-r--   0 senter    (1000) senter    (1000)      748 2024-05-12 20:15:36.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_UWB.egg-info/PKG-INFO
+-rw-rw-r--   0 senter    (1000) senter    (1000)     4735 2024-05-12 20:15:36.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_UWB.egg-info/SOURCES.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)        1 2024-05-12 20:15:36.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_UWB.egg-info/dependency_links.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       29 2024-05-12 20:15:36.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_UWB.egg-info/requires.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       13 2024-05-12 20:15:36.000000 TDSR-UWB-1.536/TDSR-UWB/TDSR_UWB.egg-info/top_level.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       38 2024-05-12 20:15:36.647590 TDSR-UWB-1.536/setup.cfg
+-rw-rw-r--   0 senter    (1000) senter    (1000)     7654 2024-05-12 20:12:53.000000 TDSR-UWB-1.536/setup.py
```

### Comparing `TDSR-UWB-1.535/PKG-INFO` & `TDSR-UWB-1.536/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TDSR-UWB
-Version: 1.535
+Version: 1.536
 Summary: Support libraries for TDSR LLC UWB Radios
 Home-page: UNKNOWN
 Author: TDSR-LLC
 Author-email: contact@tdsr-uwb.com
 License: UNKNOWN
 Project-URL: Company:, https://www.tdsr-uwb.com
 Platform: UNKNOWN
```

### Comparing `TDSR-UWB-1.535/TDSR-UWB/TDSR_Support/JsonDoc/.DS_Store` & `TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/.DS_Store`

 * *Files identical despite different names*

### Comparing `TDSR-UWB-1.535/TDSR-UWB/TDSR_Support/JsonDoc/.vscode/launch.json` & `TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `TDSR-UWB-1.535/TDSR-UWB/TDSR_Support/JsonDoc/API.md` & `TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/API.md`

 * *Files identical despite different names*

### Comparing `TDSR-UWB-1.535/TDSR-UWB/TDSR_Support/JsonDoc/API.template.md` & `TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/API.template.md`

 * *Files identical despite different names*

### Comparing `TDSR-UWB-1.535/TDSR-UWB/TDSR_Support/JsonDoc/APIwith_cat_template.md` & `TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/APIwith_cat_template.md`

 * *Files identical despite different names*

### Comparing `TDSR-UWB-1.535/TDSR-UWB/TDSR_Support/JsonDoc/Doc/TDSR_logo_250x134.png` & `TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/Doc/TDSR_logo_250x134.png`

 * *Files identical despite different names*

### Comparing `TDSR-UWB-1.535/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_STATS_CONFIRM.txt` & `TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_STATS_CONFIRM.txt`

 * *Files identical despite different names*

### Comparing `TDSR-UWB-1.535/TDSR-UWB/TDSR_Support/JsonDoc/networking.md` & `TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/networking.md`

 * *Files identical despite different names*

### Comparing `TDSR-UWB-1.535/TDSR-UWB/TDSR_Support/JsonDoc/networking.pdf` & `TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/networking.pdf`

 * *Files identical despite different names*

### Comparing `TDSR-UWB-1.535/TDSR-UWB/TDSR_Support/JsonDoc/networking.template.md` & `TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/networking.template.md`

 * *Files identical despite different names*

### Comparing `TDSR-UWB-1.535/TDSR-UWB/TDSR_Support/JsonDoc/networking_.md` & `TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/networking_.md`

 * *Files identical despite different names*

### Comparing `TDSR-UWB-1.535/TDSR-UWB/TDSR_Support/JsonDoc/updateReadme.py` & `TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/JsonDoc/updateReadme.py`

 * *Files identical despite different names*

### Comparing `TDSR-UWB-1.535/TDSR-UWB/TDSR_Support/TDSR_PW_GUI.py` & `TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/TDSR_PW_GUI.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 from TDSR_Support import TDSR_logging
 from TDSR_Support import TDSR_settings
 from TDSR_Support import TDSR_radioControl
 from TDSR_Support import TDSR_radioConnection
 
 # Primary window GUI class. All sub windows are launched from here as well.
-__version__ = "1.535"
+__version__ = "1.536"
 # Primary application window and GUI
 class MainWindow(QMainWindow):
     def __init__(self, app, *args, **kwargs):
         super(MainWindow, self).__init__(*args, **kwargs)
         title = "PennyWhistle Ranging GUI V" + __version__
         self.setWindowTitle(title)
         self.myScreen = app.primaryScreen()                      # self is mainwindow Widget and myScreen is the display it lives on
@@ -39,18 +39,17 @@
         self.initWindows()
         self.screenSetup()
         self.chipTempTimer = QTimer()
         self.initGUI()
         self.show()
         self.appSetup()
 
-
     def screenSetup(self):
         allScreens = self.myScreen.virtualSiblings() # list of each available monitor as a QScreen
-        print(allScreens)
+        # print(allScreens)
         if int(self.monitor.height()) < 1100:
             self.reduceSize = (1000 - int(self.monitor.height()) + 80)
         else:
             self.reduceSize = 0
         self.mainWindowHeight = 1000 - self.reduceSize
         self.mainWindowWidth = 1000
         savedPosition = self.appSettings['savePosition'].split(",")
@@ -89,15 +88,19 @@
         #     y = 0
         # self.move(currentScreen.availableGeometry().left()+x, currentScreen.availableGeometry().top()+y)
         self.positionWindows()
 
 
     def appSetup(self):
         self.multiCastIP = "239.255.92.43"
+        self.radioIP_Port = 8888
+        self.radioMultiCast_Port = 8890
         self.radioMode = 'idle'
+        self.ipRadios = []
+        self.usbRadios = []
         self.radioReq = None
         self.radioResp = None
         self.configID = 0
         self.radioConfigReq = None
         self.radioConfigResp = None
         self.radioStateReq = None
         self.radioStateResp = None
@@ -113,24 +116,33 @@
         self.stdNoiseMax = -10
         self.stdNoiseMin = 20000
         self.maxNoiseMax = -10
         self.maxNoiseMin = 20000
         self.destSlotDataMax = 100
         self.consoleBuf = ""
         self.logFile = TDSR_logging.logData(self)
+        self.radioScanComplete = False
+        self.usbRadios = self.getUSBPorts()
         self.radioConnectMultiCast()
-        self.getMultiCastRadioIPs()
+        self.ipRadios = self.getMultiCastRadioIPs()
+        self.radioScanComplete = False
+        self.compileRadioList()
+        self.radioScanComplete = True
         self.radioConnectReq()
         self.radioConnectResp()
         self.statsTimer = QTimer()
         self.statsTimer.setInterval(4000)
         self.statsTimer.timeout.connect(self.updateStats)
         self.chipTempTimer = QTimer()
         self.chipTempTimer.setInterval(4000)
         self.chipTempTimer.timeout.connect(self.updateChipTemp)
+        self.radioCheckTimer = QTimer()
+        self.radioCheckTimer.setInterval(2000)
+        self.radioCheckTimer.timeout.connect(self.radioCheck)
+        self.radioCheckTimer.start()
         self.guiUpdateTimer = QTimer()
         updateTime = int(1000*(1/(int(self.appSettings['guiUpdateRate']))))
         self.guiUpdateTimer.setInterval(updateTime)
         self.guiUpdateTimer.timeout.connect(self.updateGUI)
         self.rangingActive = False
         self.rangeInProgress = False
         if self.connectedRequester == 1:
@@ -139,69 +151,98 @@
         self.updateConsole(text)
         # for thread in threading.enumerate():
         #     print(thread.name)
 
 # Connects to requester radio. Needed for ranging to run.
     def radioConnectReq(self):
         if self.connectedRequester != 1:
-            self.radioReq = TDSR_radioConnection.Radio(self, self.messageTypes, 'ip', self.appSettings['reqIP'])
+            radioName = self.appSettings['reqRadio']
+            self.radioReq = None
+            for radio in self.radioList:
+                if radioName == radio['name'] and radioName != 'Disconnect':
+                    self.radioReq = TDSR_radioConnection.Radio(self, self.messageTypes, radio['type'], radio['addr'], radio['port'])
+            if self.radioReq == None:
+                self.radioReq = TDSR_radioConnection.Radio(self, self.messageTypes, 'None', 'None', 'None')
             if self.radioReq.status == False:
-                print(f"Could not connect to IP Address: {self.appSettings['reqIP']}")
+                if self.appSettings['reqRadio'] == "Disconnect":
+                    print("Not connected to a primary radio")
+                else:
+                    print(f"Could not connect to Radio: {self.appSettings['reqRadio']}")
                 self.connectedRequester = 0
                 self.windowDataTransfer.radioData.reqMsgTimer.stop()
                 self.chipTempTimer.stop()
                 self.dispChipTemp.setText("-")
             else:
                 self.windowDataTransfer.radioData.reqMsgTimer.start()
-                self.radioConfigReq, addr = self.radioReq.API.radio_GetConfig_Request(self.appSettings['reqIP'], self.configID)
-                self.radioStateReq, addr = self.radioReq.API.radio_GetState_Request(self.appSettings['reqIP'])
-                self.radioReqNodeID, addr = self.radioReq.API.radio_GetNodeID_Request(self.appSettings['reqIP'])
+                self.radioConfigReq, addr = self.radioReq.API.radio_GetConfig_Request(self.appSettings['reqRadio'], self.configID)
+                self.radioStateReq, addr = self.radioReq.API.radio_GetState_Request(self.appSettings['reqRadio'])
+                self.radioReqNodeID, addr = self.radioReq.API.radio_GetNodeID_Request(self.appSettings['reqRadio'])
                 self.radioReqNodeID = self.radioReqNodeID['RADIO_GET_NODE_CONFIG_CONFIRM']['nodeId']
                 self.chipTempTimer.start()
                 self.connectedRequester = 1
             self.updateConnectReq(self.radioReq.status)
 
 # Connects to responding radio. Needed to get stats and set configuration but not needed to range.
     def radioConnectResp(self):
         if self.check_connectResp.isChecked():
             self.appSettings['connectResp'] = 1
         else:
             self.appSettings['connectResp'] = 0
         if self.appSettings['connectResp'] == 1:
             if self.connectedResponder != 1:
-                self.radioResp = TDSR_radioConnection.Radio(self, self.messageTypes, 'ip', self.appSettings['respIP'])
+                self.radioResp = None
+                radioName = self.appSettings['respRadio']
+                for radio in self.radioList:
+                    if radioName == radio['name'] and radioName != 'Disconnect':
+                        self.radioResp = TDSR_radioConnection.Radio(self, self.messageTypes, radio['type'], radio['addr'], radio['port'])
+                if self.radioResp == None:
+                    self.radioResp = TDSR_radioConnection.Radio(self, self.messageTypes, 'None', 'None', 'None')
                 if self.radioResp.status == False:
-                    print(f"Could not connect to IP Address: {self.appSettings['respIP']}")
+                    print(f"Could not connect to IP Address: {self.appSettings['respRadio']}")
                     self.connectedResponder = 0
                     self.windowDataTransfer.radioData.respMsgTimer.stop()
                 else:
                     self.connectedResponder = 1
                     self.windowDataTransfer.radioData.respMsgTimer.start()
-                    self.radioConfigResp, addr = self.radioResp.API.radio_GetConfig_Request(self.appSettings['respIP'], self.configID)
-                    self.radioStateResp, addr = self.radioResp.API.radio_GetState_Request(self.appSettings['respIP'])
-                    self.radioRespNodeID, addr = self.radioResp.API.radio_GetNodeID_Request(self.appSettings['respIP'])
+                    self.radioConfigResp, addr = self.radioResp.API.radio_GetConfig_Request(self.appSettings['respRadio'], self.configID)
+                    self.radioStateResp, addr = self.radioResp.API.radio_GetState_Request(self.appSettings['respRadio'])
+                    self.radioRespNodeID, addr = self.radioResp.API.radio_GetNodeID_Request(self.appSettings['respRadio'])
                     self.radioRespNodeID = self.radioRespNodeID['RADIO_GET_NODE_CONFIG_CONFIRM']['nodeId']
                     self.updateRespID(self.radioRespNodeID)
                     # self.respMsgTimer.start()
                 self.updateConnectResp(self.radioResp.status)
         else:
             if self.connectedResponder == 1:
                 self.windowDataTransfer.radioData.respMsgTimer.stop()
                 self.connectedResponder = 0
                 self.radioResp.disconnect()
             self.updateConnectResp(False)
 
     def radioConnectMultiCast(self):
         if self.connectedMultiCast != 1:
-            self.radioMultiCast = TDSR_radioConnection.Radio(self, self.messageTypes, 'ip', self.multiCastIP)
+            self.radioMultiCast = TDSR_radioConnection.Radio(self, self.messageTypes, 'ip', self.multiCastIP, self.radioMultiCast_Port)
             if self.radioMultiCast.status == False:
                 self.connectedMultiCast = 0
             else:
                 self.connectedMultiCast = 1
 
+    def USBTest(self):
+        print("Trying:", self.usbRadios[0]['addr'])
+        usbRadio = TDSR_radioConnection.Radio(self, self.messageTypes, 'usb', 'connect', self.usbRadios[0]['addr'])
+        stats,packet,addr = usbRadio.API.radio_GetIP_Request("USB")
+        # packet = '{"RADIO_GET_IP_REQUEST":{"msgId": 101}}'
+        # usbRadio.radioIf.sendPacket(packet)
+        # print("trying again")
+        # sleep(3)
+        # packet = usbRadio.radioIf.readPacketInternal()
+        # print("USBTest:", packet)
+        # packet = usbRadio.radioIf.readPacketInternal()
+        print("USBTest:", packet)
+        usbRadio.radioIf.disconnect()
+
     def radioMessageTypes(self,top_dir):
         messageTypes = {}
         basePath = path.dirname(path.abspath(__file__))
         top_dir = basePath + "/" + top_dir + "/"
         if (path.isdir(top_dir)):
             filesTxt = glob(path.join(top_dir,"*.txt"))
             for filePair in filesTxt:
@@ -214,74 +255,170 @@
         return messageTypes
 
 # Get various running statistics from requester radio
     def getReqStats(self):
         if self.connectedRequester != 1:
             self.radioConnectReq()
         if self.connectedRequester == 1:
-            stats, packet, addr = self.radioReq.API.radio_GetStats_Request(self.appSettings['reqIP'])
+            stats, packet, addr = self.radioReq.API.radio_GetStats_Request(self.appSettings['reqRadio'])
             self.updateReqStats(packet)
 
 # Get various running statistics from responder radio if connected
     def getRespStats(self):
         if self.connectedResponder != 1:
             self.radioConnectResp()
         if self.connectedResponder == 1:
-            stats,packet,addr = self.radioResp.API.radio_GetStats_Request(self.appSettings['respIP'])
+            stats,packet,addr = self.radioResp.API.radio_GetStats_Request(self.appSettings['respRadio'])
             self.updateRespStats(packet)
 
 # gets config information from requester radio
     def getReqConfig(self):
-        self.radioConfigReq,addr = self.radioReq.API.radio_GetConfig_Request(self.appSettings['reqIP'], self.configID)
-        self.radioReqNodeID,addr = self.radioReq.API.radio_GetNodeID_Request(self.appSettings['reqIP'])
+        self.radioConfigReq,addr = self.radioReq.API.radio_GetConfig_Request(self.appSettings['reqRadio'], self.configID)
+        self.radioReqNodeID,addr = self.radioReq.API.radio_GetNodeID_Request(self.appSettings['reqRadio'])
         self.radioReqNodeID = self.radioReqNodeID['RADIO_GET_NODE_CONFIG_CONFIRM']['nodeId']
 
 # gets config information from responder radio
     def getRespConfig(self):
-        self.radioConfigResp,addr = self.radioResp.API.radio_GetConfig_Request(self.appSettings['respIP'], self.configID)
-        self.radioRespNodeID, addr = self.radioResp.API.radio_GetNodeID_Request(self.appSettings['respIP'])
+        self.radioConfigResp,addr = self.radioResp.API.radio_GetConfig_Request(self.appSettings['respRadio'], self.configID)
+        self.radioRespNodeID, addr = self.radioResp.API.radio_GetNodeID_Request(self.appSettings['respRadio'])
         self.radioRespNodeID = self.radioRespNodeID['RADIO_GET_NODE_CONFIG_CONFIRM']['nodeId']
 
 # gets general radio information from requester radio
     def getReqRadioInfo(self):
         self.radioConnectReq()
         if self.connectedRequester == 1:
-            stats,packet,addr = self.radioReq.API.radio_GetInfo_Request(self.appSettings['reqIP'])
+            stats,packet,addr = self.radioReq.API.radio_GetInfo_Request(self.appSettings['reqRadio'])
             self.showReqRadioInfo(packet)
 
     def getMultiCastRadioIPs(self):
         self.radioConnectMultiCast()
-        print()
-        text = "Detected Following Radio IP Addresses:"
-        print(text)
-        self.updateConsole(text)
-        self.updateConsole("\n")
+        ipRadios = []
         if self.connectedMultiCast == 1:
             stats,packet,addr = self.radioMultiCast.API.radio_GetIP_Request(self.multiCastIP)
             sleep(.1)
             if 'RADIO_GET_IP_CONFIRM' in packet.keys():
-                text = packet['RADIO_GET_IP_CONFIRM']['ipv4']
-                print(text)
-                self.updateConsole(text)
+                radioObj = {}
+                addr = packet['RADIO_GET_IP_CONFIRM']['ipv4']
+                radioObj['type'] = "ip"
+                radioObj['name'] = addr
+                radioObj['addr'] = addr
+                radioObj['port'] = self.radioIP_Port
+                ipRadios.append(radioObj)
             for i in self.radioMultiCast.messageQueues:
                 while not self.radioMultiCast.messageQueues[i].empty():
                     packet = self.radioMultiCast.messageQueues[i].get()
                     if 'RADIO_GET_IP_CONFIRM' in packet.keys():
-                        text = packet['RADIO_GET_IP_CONFIRM']['ipv4']
-                        print(text)
-                        self.updateConsole(text)
-                        self.updateConsole("\n")
-        self.updateConsole("\n")
-        print()
+                        radioObj = {}
+                        addr = packet['RADIO_GET_IP_CONFIRM']['ipv4']
+                        radioObj['type'] = "ip"
+                        radioObj['name'] = addr
+                        radioObj['addr'] = addr
+                        radioObj['port'] = self.radioIP_Port
+                        ipRadios.append(radioObj)
+        return ipRadios
+
+    def getUSBPorts(self):
+        usbRadiosCheck = TDSR_radioConnection.Radio(self, self.messageTypes, 'usb', '', 'find')
+        radios = usbRadiosCheck.findUsbRadios()
+        usbRadios = []
+        for radio in radios:
+            radioObj = {}
+            radioName = str(radio)
+            if "tty" in radioName:
+                radioName = radioName.split(" ")
+                radioAddr = radioName[0]
+                radioName = radioName[0].split("/")
+                radioName = radioName[2]
+                radioName = "USB-Port " + radioName[len(radioName)-1:]
+            if "COM" in radioName:
+                radioName = radioName.split(" ")
+                radioAddr = radioName[0]
+                radioName = radioName[0]
+                radioName = radioName + " USB"
+            if "modem" in radioName:
+                radioName = radioName.split(" ")
+                radioAddr = radioName[0]
+                radioName = radioName[0].split("modem")
+                radioName = "USB " + radioName[1]
+            radioObj['type'] = "usb"
+            radioObj['name'] = radioName
+            radioObj['addr'] = radioAddr
+            radioObj['port'] = "connect"
+            usbRadios.append(radioObj)
+        return usbRadios
+
+    def radioCheck(self):
+        ipRadios = self.getMultiCastRadioIPs()
+        usbRadios = self.getUSBPorts()
+        radioChange = 0
+        if len(ipRadios) == len(self.ipRadios) and len(usbRadios) == len(self.usbRadios):
+            for radio in ipRadios:
+                if radio not in self.ipRadios:
+                    radioChange = 1
+            for radio in usbRadios:
+                if radio not in self.usbRadios:
+                    radioChange = 1
+        else:
+            radioChange = 1
+        if radioChange == 1:
+            self.ipRadios = ipRadios
+            self.usbRadios = usbRadios
+            self.compileRadioList()
+            print("Change Detected")
+
+    def compileRadioList(self):
+        self.radioList = []
+        radioObj = {}
+        radioObj['type'] = "Disconnect"
+        radioObj['name'] = "Disconnect"
+        radioObj['addr'] = "Disconnect"
+        self.radioList.append(radioObj)
+        for radio in self.ipRadios:
+            self.radioList.append(radio)
+        for radio in self.usbRadios:
+            self.radioList.append(radio)
+        self.radioScanComplete = False
+        self.dropMenuReqRadio.clear()
+        self.dropMenuRespRadio.clear()
+        radios = []
+        for radio in self.radioList:
+            radios.append(radio['name'])
+        self.dropMenuReqRadio.addItems(radios)
+        self.dropMenuRespRadio.addItems(radios)
+        self.radioScanComplete = True
+        radioIndex = self.dropMenuReqRadio.findText(self.appSettings['reqRadio'])
+        if radioIndex != -1:
+            self.radioScanComplete = False
+            self.dropMenuReqRadio.setCurrentIndex(radioIndex)
+            self.radioScanComplete = True
+        else:
+            if self.connectedRequester == 1:
+                self.radioReq.disconnect()
+                self.connectedRequester = 0
+            self.dropMenuReqRadio.setCurrentIndex(0)
+            self.appSettings['reqRadio'] = self.dropMenuReqRadio.currentText()
+            self.updateConnectReq(False)
+        radioIndex = self.dropMenuRespRadio.findText(self.appSettings['respRadio'])
+        if radioIndex != -1:
+            self.radioScanComplete = False
+            self.dropMenuRespRadio.setCurrentIndex(radioIndex)
+            self.radioScanComplete = True
+        else:
+            if self.connectedResponder == 1:
+                self.radioResp.disconnect()
+                self.connectedResponder = 0
+            self.dropMenuRespRadio.setCurrentIndex(0)
+            self.appSettings['respRadio'] = self.dropMenuRespRadio.currentText()
+            self.updateConnectResp(False)
 
 # gets general radio information from requester radio
     def getReqRadioChipTemp(self):
         self.radioConnectReq()
         if self.connectedRequester == 1:
-            status,packet,addr = self.radioReq.API.radio_GetInfo_Request(self.appSettings['reqIP'])
+            status,packet,addr = self.radioReq.API.radio_GetInfo_Request(self.appSettings['reqRadio'])
             if status:
                 tmp = packet['RADIO_GET_INFO_CONFIRM']['chipTemp']
                 # if tmp > 100:
                 #     print(packet)
                 # else:
                 #     print(packet)
                 tmp = "%0.1f" % tmp
@@ -293,15 +430,15 @@
         self.plotData()
         self.guiPacketUpdates(self.radioRanging.packetDisplay)
 
 # gets general radio information from responder radio if connected
     def getRespRadioInfo(self):
         self.radioConnectResp()
         if self.connectedResponder == 1:
-            stats,packet,addr = self.radioResp.API.radio_GetInfo_Request(self.appSettings['respIP'])
+            stats,packet,addr = self.radioResp.API.radio_GetInfo_Request(self.appSettings['respRadio'])
             self.showRespRadioInfo(packet)
 # Updates small range display and large one if open. Color codes each based on signal strength.
 # Updates stat and data windows if them are open.
     def guiPacketUpdates(self, packet):
         if packet != None:
             if self.radioMode == 'networking':
                 slot = int(packet['RANGE_INFO']['slotIdx'])
@@ -754,45 +891,48 @@
         yBias = 0
         xBump = 210
         yBump = 75
         xWidth = 200
         yWidth = 40
         x = 0
         y = 0
-        self.labelReqIP = QLabel(self)
-        self.labelReqIP.resize(xWidth,yWidth)
-        self.labelReqIP.move(x*xBump + xStart + xBias, yStart + y*yBump + yBias)
-        self.labelReqIP.setAlignment(Qt.AlignmentFlag.AlignCenter)
-        self.labelReqIP.setFont(self.guiFont.guiFont20)
-        self.labelReqIP.setText("Primary Radio IP")
-        self.dispReqIP = QLineEdit(self)
-        self.dispReqIP.setToolTip("Enter IP address of range requesting radio")
-        self.dispReqIP.setFont(self.guiFont.guiFont20)
-        self.dispReqIP.move(x*xBump + xStart + xBias, yStart + y*yBump + yBias + 35)
-        self.dispReqIP.resize(xWidth,yWidth)
-        self.dispReqIP.setAlignment(Qt.AlignmentFlag.AlignCenter)
-        self.dispReqIP.setText(self.appSettings['reqIP'])
-        self.dispReqIP.editingFinished.connect(self.updateReqIP)
+        self.labelreqRadio = QLabel(self)
+        self.labelreqRadio.resize(xWidth,yWidth)
+        self.labelreqRadio.move(x*xBump + xStart + xBias, yStart + y*yBump + yBias)
+        self.labelreqRadio.setAlignment(Qt.AlignmentFlag.AlignCenter)
+        self.labelreqRadio.setFont(self.guiFont.guiFont20)
+        self.labelreqRadio.setText("Primary Radio")
+        self.dropMenuReqRadio = QComboBox(self)
+        self.dropMenuReqRadio.resize(xWidth,yWidth)
+        self.dropMenuReqRadio.setToolTip("Select range requesting radio")
+        self.dropMenuReqRadio.setFont(self.guiFont.guiFont20)
+        self.dropMenuReqRadio.move(x*xBump + xStart + xBias, yStart + y*yBump + yBias + 35)
+        self.dropMenuReqRadio.addItems([])
+        self.dropMenuReqRadio.setEditable(False)
+        self.dropMenuReqRadio.setStyleSheet("QComboBox {color: GhostWhite; background-color: SteelBlue;} QAbstractItemView {color: GhostWhite; background-color: DarkBlue;}")
+        self.dropMenuReqRadio.currentTextChanged.connect(self.updateReqRadio)
 
         x = 0
         y = 1
-        self.labelRespIP = QLabel(self)
-        self.labelRespIP.resize(xWidth,yWidth)
-        self.labelRespIP.move(x*xBump + xStart + xBias, yStart + y*yBump + yBias)
-        self.labelRespIP.setAlignment(Qt.AlignmentFlag.AlignCenter)
-        self.labelRespIP.setFont(self.guiFont.guiFont20)
-        self.labelRespIP.setText("Secondary IP")
-        self.dispRespIP = QLineEdit(self)
-        self.dispRespIP.setToolTip("If connected, enter IP address of responding radio")
-        self.dispRespIP.setFont(self.guiFont.guiFont20)
-        self.dispRespIP.move(x*xBump + xStart + xBias, yStart + y*yBump + yBias + 35)
-        self.dispRespIP.resize(xWidth,yWidth)
-        self.dispRespIP.setAlignment(Qt.AlignmentFlag.AlignCenter)
-        self.dispRespIP.setText(self.appSettings['respIP'])
-        self.dispRespIP.editingFinished.connect(self.updateRespIP)
+        self.labelrespRadio = QLabel(self)
+        self.labelrespRadio.resize(xWidth,yWidth)
+        self.labelrespRadio.move(x*xBump + xStart + xBias + 10, yStart + y*yBump + yBias)
+        self.labelrespRadio.setAlignment(Qt.AlignmentFlag.AlignCenter)
+        self.labelrespRadio.setFont(self.guiFont.guiFont20)
+        self.labelrespRadio.setText("Secondary Radio")
+
+        self.dropMenuRespRadio = QComboBox(self)
+        self.dropMenuRespRadio.resize(xWidth,yWidth)
+        self.dropMenuRespRadio.setToolTip("Select range responding radio")
+        self.dropMenuRespRadio.setFont(self.guiFont.guiFont20)
+        self.dropMenuRespRadio.move(x*xBump + xStart + xBias, yStart + y*yBump + yBias + 35)
+        self.dropMenuRespRadio.addItems([])
+        self.dropMenuRespRadio.setEditable(False)
+        self.dropMenuRespRadio.setStyleSheet("QComboBox {color: GhostWhite; background-color: SteelBlue;} QAbstractItemView {color: GhostWhite; background-color: DarkBlue;}")
+        self.dropMenuRespRadio.currentTextChanged.connect(self.updateRespRadio)
 
         self.check_connectResp = QCheckBox('', self)
         self.check_connectResp.setToolTip('Connect GUI to Responding Radio')
         self.check_connectResp.setFont(self.guiFont.guiFont14)
         self.check_connectResp.move(x*xBump + xStart + xBias, yStart + y*yBump + yBias)
         self.check_connectResp.resize(200,40)
         if self.appSettings['connectResp'] == 0:
@@ -1155,70 +1295,43 @@
             self.dispGuiUpdateRate.setText("10")
         self.appSettings['guiUpdateRate'] = self.dispGuiUpdateRate.text()
         updateTime = int(1000*(1/(int(self.dispGuiUpdateRate.text()))))
         self.guiUpdateTimer.setInterval(updateTime)
         self.guiUpdateTimer.stop()
         self.guiUpdateTimer.start()
 # tests to see if new requester IP number is valid and updates variables and GUI
-    def updateReqIP(self):
-        tmp = self.dispReqIP.text()
-        testPass = 1
-        try:
-            tmp = tmp.split(".")
-        except:
-            testPass = 0
-        if testPass == 1:
-            for k in range(len(tmp)):
-                try:
-                    test = int(tmp[k])
-                except:
-                    testPass = 0
-        if testPass == 1:
-            for k in range(len(tmp)):
-                if int(tmp[k]) > 255 or int(tmp[k]) < 0:
-                    testPass = 0
-        if testPass != 1:
-            text = "\n  == Bad IP Address Entry: ''" + str(self.dispReqIP.text()) + "'' . Using Default ==\n\n"
-            self.updateConsole(text)
-            self.dispReqIP.setText("192.168.1.100")
-        if self.connectedRequester == 1:
-            self.radioReq.disconnect()
-        self.connectedRequester = 0
-        self.radioReq = None
-        self.appSettings['reqIP'] = (self.dispReqIP.text())
-        self.radioConnectReq()
+    def updateReqRadio(self):
+        if self.radioScanComplete == True:
+            radioSelection = self.dropMenuReqRadio.currentText()
+            testPass = 1
+            if radioSelection == self.dropMenuRespRadio.currentText():
+                self.dropMenuRespRadio.setCurrentIndex(0)
+            if self.connectedRequester == 1:
+                self.radioReq.disconnect()
+                self.windowDataTransfer.radioData.reqMsgTimer.stop()
+            self.connectedRequester = 0
+            self.radioReq = None
+            self.appSettings['reqRadio'] = radioSelection
+            if testPass == 1:
+                self.radioConnectReq()
 # tests to see if new responder IP number is valid and updates variables and GUI
-    def updateRespIP(self):
-        tmp = self.dispRespIP.text()
-        testPass = 1
-        try:
-            tmp = tmp.split(".")
-        except:
-            testPass = 0
-        if testPass == 1:
-            for k in range(len(tmp)):
-                try:
-                    test = int(tmp[k])
-                except:
-                    testPass = 0
-        if testPass == 1:
-            for k in range(len(tmp)):
-                if int(tmp[k]) > 255 or int(tmp[k]) < 0:
-                    testPass = 0
-        if testPass != 1:
-            text = "\n  == Bad IP Address Entry: ''" + str(self.dispReqIP.text()) + "'' . Using Default ==\n\n"
-            self.updateConsole(text)
-            self.dispRespIP.setText("192.168.1.100")
-        if self.connectedResponder == 1:
-            self.radioResp.disconnect()
-        self.connectedResponder = 0
-        self.radioResp = None
-        self.appSettings['respIP'] = (self.dispRespIP.text())
-        self.connectedResponder = 0
-        self.radioConnectResp()
+    def updateRespRadio(self):
+        if self.radioScanComplete:
+            radioSelection = self.dropMenuRespRadio.currentText()
+            testPass = 1
+            if radioSelection == self.dropMenuReqRadio.currentText():
+                self.dropMenuReqRadio.setCurrentIndex(0)
+            if self.connectedResponder == 1:
+                self.radioResp.disconnect()
+            self.connectedResponder = 0
+            self.radioResp = None
+            self.appSettings['respRadio'] = radioSelection
+            self.connectedResponder = 0
+            if testPass == 1:
+                self.radioConnectResp()
 # tests to see if new responder ID number is valid and updates variables and GUI, comes from responder connection.
     def updateRespID(self, nodeId):
         self.dispRespID.setText(str(nodeId))
         self.appSettings['respID'] = (self.dispRespID.text())
         if self.dispReqID.text() != "-":
             if self.dispReqID.text() == self.dispRespID.text():
                 text = "  == ERROR, reqester and responder must have different nodeIDs ==\n"
@@ -1404,60 +1517,61 @@
         if self.windowRespStats.isVisible():
             self.getRespStats()
         if (not self.windowRespStats.isVisible()) and (not self.windowReqStats.isVisible()):
             self.statsTimer.stop()
 # Updates GUI connection status of requester
     def updateConnectReq(self, status):
         if status == False:
-            self.dispReqIP.setStyleSheet("QLineEdit {background-color: red;}")
+            self.dropMenuReqRadio.setStyleSheet("QComboBox {background-color: red;}")
             self.but_RadioConfigReq.setStyleSheet("QPushButton {background-color: red;}")
-            text = "== Could not connect to Requester IP Address " + self.appSettings['reqIP'] + " ==\n"
+            text = "== Could not connect to primary radio address " + self.appSettings['reqRadio'] + " ==\n"
             self.updateConsole(text)
         else:
-            self.dispReqIP.setStyleSheet("QLineEdit {background-color: lightgreen;}")
+            self.dropMenuReqRadio.setStyleSheet("QComboBox {background-color: lightgreen;}")
             self.but_RadioConfigReq.setStyleSheet("QPushButton {background-color: SteelBlue; color: GhostWhite;}")
             self.dispReqID.setText(str(self.radioReqNodeID))
-            text = "Connected to Requester IP Address " + self.appSettings['reqIP'] + "\n"
+            text = "Connected to Primary Radio Address " + self.appSettings['reqRadio'] + "\n"
             self.updateConsole(text)
 # Updates GUI connection status of responder
     def updateConnectResp(self, status):
         if status == False:
             # self.connectedResponder = 0
-            self.dispRespIP.setStyleSheet("QLineEdit {background-color: red;}")
+            self.dropMenuRespRadio.setStyleSheet("QComboBox {background-color: red;}")
             self.but_RadioConfigResp.setStyleSheet("QPushButton {background-color: red;}")
             self.but_respRadioInfo.setStyleSheet("QPushButton {background-color: red;}")
             self.but_respStats.setStyleSheet("QPushButton {background-color: red;}")
             if self.appSettings['connectResp'] == 1:
-                text = "== Could not connect to Responder IP Address " + self.appSettings['respIP'] + " ==\n"
+                text = "== Could not connect to secondary radio address " + self.appSettings['respRadio'] + " ==\n"
                 self.updateConsole(text)
             else:
                 # self.connectedResponder = 0
                 text = "Connected responder not selected\n"
                 self.updateConsole(text)
         else:
             # self.connectedResponder = 1
-            self.dispRespIP.setStyleSheet("QLineEdit {background-color: lightgreen;}")
+            self.dropMenuRespRadio.setStyleSheet("QComboBox {background-color: lightgreen;}")
             self.but_RadioConfigResp.setStyleSheet("QPushButton {background-color: SteelBlue; color: GhostWhite;}")
             self.but_respRadioInfo.setStyleSheet("QPushButton {background-color: SteelBlue; color: GhostWhite;}")
             self.but_respStats.setStyleSheet("QPushButton {background-color: SteelBlue; color: GhostWhite;}")
-            text = "Connected to Responder IP Address " + self.appSettings['respIP'] + "\n"
+            text = "Connected to Secondary Radio Address " + self.appSettings['respRadio'] + "\n"
             self.updateConsole(text)
         self.windowDataTransfer.updateRespAvailable()
 # Updates text in GUI console output.
     def updateConsole(self, text):
         self.consoleBuf = self.consoleBuf + text
         self.consoleOutput.setText(self.consoleBuf)
         self.consoleOutputScrollBar.setValue(self.consoleOutputScrollBar.maximum())
     def updateChipTemp(self):
         if self.connectedRequester == 1:
             tmp = self.getReqRadioChipTemp()
             self.dispChipTemp.setText(str(tmp))
 
 # App close signal triggers closing of any open gui windows.
     def closeEvent(self, event):
+        self.radioCheckTimer.stop()
         self.radioRanging.networkTimer.stop()
         self.appSettings['savePosition'] = str(self.x()) + "," + str(self.y())
         self.radioRanging.closeApp()
         print("\nRanging Halted, Ranging App Closed.\n")
         self.chipTempTimer.stop()
         if self.windowReqStats.isVisible():
             self.windowReqStats.close()
@@ -1861,15 +1975,15 @@
         pgTarget = int(self.dispPGTarget.text(), 16)
         pgDelay = int(self.dispPGDelay.text(), 16)
         rxDelay = int(self.dispRXDelay.text(), 16)
         txDelay = int(self.dispTXDelay.text(), 16)
         txPower = (byte3 << 24) + (byte2 << 16) + (byte1 << 8) + byte0
         newPacket = {"RADIO_SET_TUNING_REQUEST":{"msgId":0,"TxPwrContrl":txPower,"PGCount_Target":pgTarget,"TC_PGDelay":pgDelay,"RXAntDelay":rxDelay,"TXAntDelay":txDelay,"persistFlag":1}}
         if self.gui.connectedRequester == 1:
-            self.gui.radioReq.API.radio_SetTuning_Request(self.gui.appSettings['reqIP'], newPacket)
+            self.gui.radioReq.API.radio_SetTuning_Request(self.gui.appSettings['reqRadio'], newPacket)
             self.but_storeTuning.setStyleSheet("QPushButton {background-color: FireBrick;}")
             self.but_storeTuning.setText("Writing...")
             self.flashTimer = QTimer()
             self.flashTimer.setInterval(500)
             self.flashTimer.timeout.connect(self.updateFlashButton)
             self.flashTimer.start()
 
@@ -1887,19 +2001,19 @@
         pgTarget = int(self.dispPGTarget.text(), 16)
         pgDelay = int(self.dispPGDelay.text(), 16)
         rxDelay = int(self.dispRXDelay.text(), 16)
         txDelay = int(self.dispTXDelay.text(), 16)
         txPower = (byte3 << 24) + (byte2 << 16) + (byte1 << 8) + byte0
         newPacket = {"RADIO_SET_TUNING_REQUEST":{"msgId":0,"TxPwrContrl":txPower,"PGCount_Target":pgTarget,"TC_PGDelay":pgDelay,"RXAntDelay":rxDelay,"TXAntDelay":txDelay,"persistFlag":0}}
         if self.gui.connectedRequester == 1:
-            self.gui.radioReq.API.radio_SetTuning_Request(self.gui.appSettings['reqIP'], newPacket)
+            self.gui.radioReq.API.radio_SetTuning_Request(self.gui.appSettings['reqRadio'], newPacket)
 
     def radioGetTuning(self):
         if self.gui.connectedRequester == 1:
-            status,packet,addr = self.gui.radioReq.API.radio_GetTuning_Request(self.gui.appSettings['reqIP'])
+            status,packet,addr = self.gui.radioReq.API.radio_GetTuning_Request(self.gui.appSettings['reqRadio'])
             data = packet['RADIO_GET_TUNING_CONFIRM']
             try:
                 pgTarget = data['PGCount_Target']
             except:
                 pgTarget = 0
             pgDelay = data['TC_PGDelay']
             rxDelay = data['RXAntDelay']
@@ -2150,20 +2264,20 @@
             self.radioUpdateActivePreset()
             self.radioUpdatePresets()
             self.radioGetIP()
 
     def updateNodeID(self):
         if self.configFormUpdate == 1:  # config get = 1. 0 is either set or set and store
             if self.req:
-                self.gui.radioReqNodeID, addr = self.gui.radioReq.API.radio_GetNodeID_Request(self.gui.appSettings['reqIP'])
+                self.gui.radioReqNodeID, addr = self.gui.radioReq.API.radio_GetNodeID_Request(self.gui.appSettings['reqRadio'])
                 self.gui.radioReqNodeID = self.gui.radioReqNodeID['RADIO_GET_NODE_CONFIG_CONFIRM']['nodeId']
                 self.dispNodeID.setText(str(self.gui.radioReqNodeID))
                 self.gui.dispReqID.setText(str(self.gui.radioReqNodeID))
             else:
-                self.gui.radioRespNodeID, addr = self.gui.radioResp.API.radio_GetNodeID_Request(self.gui.appSettings['respIP'])
+                self.gui.radioRespNodeID, addr = self.gui.radioResp.API.radio_GetNodeID_Request(self.gui.appSettings['respRadio'])
                 self.gui.radioRespNodeID = self.gui.radioRespNodeID['RADIO_GET_NODE_CONFIG_CONFIRM']['nodeId']
                 self.dispNodeID.setText(str(self.gui.radioRespNodeID))
                 self.gui.dispRespID.setText(str(self.gui.radioRespNodeID))
         else:                           # set or set and store branch
             if self.req:
                 self.gui.radioReqNodeID = int(self.dispNodeID.text())
                 self.gui.dispReqID.setText(str(self.gui.radioReqNodeID))
@@ -2338,19 +2452,19 @@
         self.updateAntDelay()
         self.but_storeRadioConfig.setStyleSheet("QPushButton {background-color: FireBrick;}")
         self.but_storeRadioConfig.setText("Writing...")
         self.flashTimer = QTimer()
         self.flashTimer.setInterval(500)
         self.flashTimer.timeout.connect(self.updateFlashButton)
         if self.req:
-            self.gui.radioReq.API.radio_SetConfig_Request(self.gui.appSettings['reqIP'], self.radioConfig, 1)
-            self.gui.radioReq.API.radio_SetNodeID_Request(self.gui.appSettings['reqIP'], self.gui.radioReqNodeID, 1)
+            self.gui.radioReq.API.radio_SetConfig_Request(self.gui.appSettings['reqRadio'], self.radioConfig, 1)
+            self.gui.radioReq.API.radio_SetNodeID_Request(self.gui.appSettings['reqRadio'], self.gui.radioReqNodeID, 1)
         else:
-            self.gui.radioResp.API.radio_SetConfig_Request(self.gui.appSettings['respIP'], self.radioConfig, 1)
-            self.gui.radioResp.API.radio_SetNodeID_Request(self.gui.appSettings['respIP'], self.gui.radioRespNodeID, 1)
+            self.gui.radioResp.API.radio_SetConfig_Request(self.gui.appSettings['respRadio'], self.radioConfig, 1)
+            self.gui.radioResp.API.radio_SetNodeID_Request(self.gui.appSettings['respRadio'], self.gui.radioRespNodeID, 1)
         self.flashTimer.start()
         text = "Configuration Updated In Flash\n"
         self.gui.updateConsole(text)
         self.radioGetConfig()
 
 # Simply gives visual display delay to let flash save and indicate that it happened.
     def updateFlashButton(self):
@@ -2368,32 +2482,32 @@
         # self.updateMenuPAC()
         self.updateMenuChannel()
         self.updateMenuPreamCode()
         self.updateNodeID()
         self.updateTxPower()
         self.updateAntDelay()
         if self.req:
-            self.gui.radioReq.API.radio_SetConfig_Request(self.gui.appSettings['reqIP'], self.radioConfig, 0)
-            self.gui.radioReq.API.radio_SetNodeID_Request(self.gui.appSettings['reqIP'], self.gui.radioReqNodeID, 0)
+            self.gui.radioReq.API.radio_SetConfig_Request(self.gui.appSettings['reqRadio'], self.radioConfig, 0)
+            self.gui.radioReq.API.radio_SetNodeID_Request(self.gui.appSettings['reqRadio'], self.gui.radioReqNodeID, 0)
         else:
-            self.gui.radioResp.API.radio_SetConfig_Request(self.gui.appSettings['respIP'], self.radioConfig, 0)
-            self.gui.radioResp.API.radio_SetNodeID_Request(self.gui.appSettings['respIP'], self.gui.radioRespNodeID, 0)
+            self.gui.radioResp.API.radio_SetConfig_Request(self.gui.appSettings['respRadio'], self.radioConfig, 0)
+            self.gui.radioResp.API.radio_SetNodeID_Request(self.gui.appSettings['respRadio'], self.gui.radioRespNodeID, 0)
         text =  "Configuration Set\n"
         self.gui.updateConsole(text)
         self.radioGetConfig()
         self.but_setRadioConfig.setStyleSheet("QPushButton {background-color: SteelBlue; color: GhostWhite;}")
 
 ## IP Config
     def radioGetIP(self):
         ip = ""
         if self.req:
-            ip = self.gui.appSettings['reqIP']
+            ip = self.gui.appSettings['reqRadio']
             status, msg, addr = self.gui.radioReq.API.radio_GetIP_Request(ip)
         else:
-            ip = self.gui.appSettings['respIP']
+            ip = self.gui.appSettings['respRadio']
             status, msg, addr = self.gui.radioResp.API.radio_GetIP_Request(ip)
         msg = msg['RADIO_GET_IP_CONFIRM']
         ip = msg['ipv4']
         netmask = msg ['netmask']
         gateway = msg['gateway']
         self.dispIP.setText(ip)
         self.dispNetMask.setText(netmask)
@@ -2401,87 +2515,87 @@
 
     def radioSetIP(self):
         newIP = self.dispIP.text()
         netmask = self.dispNetMask.text()
         gateway = self.dispGateWay.text()
         ip = ""
         if self.req:
-            ip = self.gui.appSettings['reqIP']
+            ip = self.gui.appSettings['reqRadio']
             self.gui.radioReq.API.radio_SetIP_Request(ip, newIP, netmask, gateway)
         else:
-            ip = self.gui.appSettings['respIP']
+            ip = self.gui.appSettings['respRadio']
             self.gui.radioResp.API.radio_SetIP_Request(ip, newIP, netmask, gateway)
         self.gui.updateConsole("\nRadio IP information updated\n")
 
     def radioReboot(self):
         newIP = self.dispIP.text()
         ip = ""
         if self.req:
-            ip = self.gui.appSettings['reqIP']
+            ip = self.gui.appSettings['reqRadio']
             self.gui.radioReq.API.radio_Reboot_Request(ip)
-            self.gui.appSettings['reqIP'] = newIP
+            self.gui.appSettings['reqRadio'] = newIP
             self.connectedRequester = 0
-            self.gui.dispReqIP.setStyleSheet("QLineEdit {background-color: red;}")
+            self.gui.dispreqRadio.setStyleSheet("QLineEdit {background-color: red;}")
             self.gui.radioReq.disconnect()
         else:
-            ip = self.gui.appSettings['respIP']
+            ip = self.gui.appSettings['respRadio']
             self.gui.radioResp.API.radio_Reboot_Request(ip)
-            self.gui.appSettings['respIP'] = newIP
-            self.gui.dispRespIP.setStyleSheet("QLineEdit {background-color: red;}")
+            self.gui.appSettings['respRadio'] = newIP
+            self.gui.disprespRadio.setStyleSheet("QLineEdit {background-color: red;}")
             self.gui.radioResp.disconnect()
             self.connectedResponder = 0
         self.but_reboot.setStyleSheet("QPushButton {background-color: red;}")
         self.gui.updateConsole("\nRebooting Radio. Changing to new IP\n == Waiting for reboot ==\n")
         self.rebootTimer = QTimer()
         self.rebootTimer.setInterval(20000)
         self.rebootTimer.timeout.connect(self.radioReconnect)
         self.rebootTimer.start()
         self.gui.statsTimer.stop()
         self.gui.chipTempTimer.stop()
 
     def radioReconnect(self):
         self.rebootTimer.stop()
         if self.req:
-            self.gui.dispReqIP.setText(self.gui.appSettings['reqIP'])
-            self.gui.updateReqIP()
+            self.gui.dispreqRadio.setText(self.gui.appSettings['reqRadio'])
+            self.gui.updateReqRadio()
         else:
-            self.gui.dispRespIP.setText(self.gui.appSettings['respIP'])
-            self.gui.updateRespIP()
+            self.gui.disprespRadio.setText(self.gui.appSettings['respRadio'])
+            self.gui.updateRespRadio()
         self.gui.updateConsole("\nAttempting reconnect after reboot\n")
         self.but_reboot.setStyleSheet("QPushButton {background-color: DarkOrange;}")
         self.gui.statsTimer.start()
         self.gui.chipTempTimer.start()
 
 ## Presets
 
     # Gets a list of all presets on the radio and adds to dropdown menu.
     def radioGetPresets(self):
         ip = ""
         if self.req:
-            ip = self.gui.appSettings['reqIP']
+            ip = self.gui.appSettings['reqRadio']
             msg, addr = self.gui.radioReq.API.radio_ListPresets_Request(ip)
         else:
-            ip = self.gui.appSettings['respIP']
+            ip = self.gui.appSettings['respRadio']
             msg, addr = self.gui.radioResp.API.radio_ListPresets_Request(ip)
         msg = msg['RADIO_LIST_PRESETS_CONFIRM']
         presets = msg['presetNames']
         self.dropMenuPresets.clear()
         if len(presets) < 1:
             print("No presets stored on radio")
             self.dropMenuPresets.addItems(["Current Active Settings"])
         else:
             self.dropMenuPresets.addItems(["Current Active Settings"])
             self.dropMenuPresets.addItems(presets)
 
     def radioUpdateActivePreset(self):
         if self.req:
-            ip = self.gui.appSettings['reqIP']
+            ip = self.gui.appSettings['reqRadio']
             nameMsgActive, addr = self.gui.radioReq.API.radio_Get_Active_Preset_Request(ip)
         else:
-            ip = self.gui.appSettings['respIP']
+            ip = self.gui.appSettings['respRadio']
             nameMsgActive, addr = self.gui.radioReq.API.radio_Get_Active_Preset_Request(ip)
         # print(nameMsgActive)
         nameMsgActive = nameMsgActive['RADIO_GET_ACTIVE_PRESET_CONFIRM']
         nameActive = nameMsgActive['activePreset']
         self.dropMenuPresets.setCurrentText(nameActive)
 
     def radioUpdatePresets(self):
@@ -2489,19 +2603,19 @@
         nameSelected = self.dropMenuPresets.currentText()
         ip = ""
         configMsgSelected = ""
         nameMsgActive = ""
         # Get the config of name currently selected in drop down
         # Get the name of the active preset if one exists.
         if self.req:
-            ip = self.gui.appSettings['reqIP']
+            ip = self.gui.appSettings['reqRadio']
             configMsgSelected, addr = self.gui.radioReq.API.radio_GetPreset_Request(ip, nameSelected)
             # nameMsgActive, addr = self.gui.radioReq.API.radio_Get_Active_Preset_Request(ip)
         else:
-            ip = self.gui.appSettings['respIP']
+            ip = self.gui.appSettings['respRadio']
             configMsgSelected, addr = self.gui.radioResp.API.radio_GetPreset_Request(ip, nameSelected)
             # nameMsgActive, addr = self.gui.radioReq.API.radio_Get_Active_Preset_Request(ip)
         # nameMsgActive = nameMsgActive['RADIO_GET_ACTIVE_PRESET_CONFIRM']
         # nameActive = nameMsgActive['activePreset']
         # if a preset is active on radio and GUI does not match, make GUI match active preset. Else show current config
         if nameSelected == "Current Active Settings" or nameSelected == "":
             self.radioGetConfig()
@@ -2576,18 +2690,18 @@
             print("Please enter a preset name")
             self.gui.updateConsole("\n== Please enter a preset name == \n")
         else:
             lock = "false"
             ip = ""
             self.radioSetConfig()
             if self.req:
-                ip = self.gui.appSettings['reqIP']
+                ip = self.gui.appSettings['reqRadio']
                 self.gui.radioReq.API.radio_SavePreset_Request(ip, name, lock)
             else:
-                ip = self.gui.appSettings['respIP']
+                ip = self.gui.appSettings['respRadio']
                 self.gui.radioResp.API.radio_SavePreset_Request(ip, name, lock)
             self.radioGetPresets()
             self.gui.updateConsole("\nPreset saved\n")
             self.dropMenuPresets.setCurrentText(name)
             # print(len(self.dropMenuPresets))
             # for i in range(len(self.dropMenuPresets)):
             #     print(self.dropMenuPresets.itemText(i))
@@ -2598,36 +2712,36 @@
         if name == "":
             print("Please enter a preset name")
             self.gui.updateConsole("\n== Please enter a preset name == \n")
         else:
             lock = "true"
             ip = ""
             if self.req:
-                ip = self.gui.appSettings['reqIP']
+                ip = self.gui.appSettings['reqRadio']
                 self.gui.radioReq.API.radio_SavePreset_Request(ip, name, lock)
             else:
-                ip = self.gui.appSettings['respIP']
+                ip = self.gui.appSettings['respRadio']
                 self.gui.radioResp.API.radio_SavePreset_Request(ip, name, lock)
             self.gui.updateConsole("\nLocked preset saved\n")
             self.radioGetPresets()
 
     # Causes a preset to be applied to the radio.
     def radioApplyPreset(self):
         name = self.dropMenuPresets.currentText()
         if name == "" or name == "No Stored Presets":
             print("Need to first save a preset before it can be applied")
             self.gui.updateConsole("\n== Need to first save a preset before it can be applied ==\n")
         else:
             persist = 0
             ip = ""
             if self.req:
-                ip = self.gui.appSettings['reqIP']
+                ip = self.gui.appSettings['reqRadio']
                 self.gui.radioReq.API.radio_ApplyPreset_Request(ip, name, persist)
             else:
-                ip = self.gui.appSettings['respIP']
+                ip = self.gui.appSettings['respRadio']
                 self.gui.radioResp.API.radio_ApplyPreset_Request(ip, name, persist)
             self.gui.updateConsole("\nPreset Applied\n")
             self.radioGetConfig()
             self.gui.windowChipTuning.radioGetTuning()
 
     # Applies with persistence after reboot.
     def radioPersistPreset(self):
@@ -2635,36 +2749,36 @@
         if name == "" or name == "No Stored Presets":
             print("Need to first save a preset before it can be applied")
             self.gui.updateConsole("\n== Need to first save a preset before it can be applied ==\n")
         else:
             persist = 1
             ip = ""
             if self.req:
-                ip = self.gui.appSettings['reqIP']
+                ip = self.gui.appSettings['reqRadio']
                 self.gui.radioReq.API.radio_ApplyPreset_Request(ip, name, persist)
             else:
-                ip = self.gui.appSettings['respIP']
+                ip = self.gui.appSettings['respRadio']
                 self.gui.radioResp.API.radio_ApplyPreset_Request(ip, name, persist)
             self.gui.updateConsole("\nPersistent Preset Applied\n")
             self.radioGetConfig()
             self.gui.windowChipTuning.radioGetTuning()
 
     # Deletes a preset from the radio.
     def radioDeletePreset(self):
         name = self.dropMenuPresets.currentText()
         if name == "" or name == "No Stored Presets" or name == "Current Active Settings":
             print("No presets to delete")
             self.gui.updateConsole("\n== No presets to delete == \n")
         else:
             ip = ""
             if self.req:
-                ip = self.gui.appSettings['reqIP']
+                ip = self.gui.appSettings['reqRadio']
                 self.gui.radioReq.API.radio_DeletePreset_Request(ip, name)
             else:
-                ip = self.gui.appSettings['respIP']
+                ip = self.gui.appSettings['respRadio']
                 self.gui.radioResp.API.radio_DeletePreset_Request(ip, name)
             self.gui.updateConsole("\nSelected Preset Deleted\n")
             self.radioGetPresets()
             self.dropMenuPresets.setCurrentText("Current Active Settings")
 
     # Indicates that config has changed and needs to be updated on the radio.
     def updateConfigButton(self):
@@ -3441,15 +3555,15 @@
             self.but_enableLogging.setText("Logging Disabled")
             self.but_enableLogging.setStyleSheet("QPushButton {background-color: lightyellow;}")
             self.gui.logFile.closeLogFile()
         else:
             self.gui.appSettings['enableLogging'] = 1
             self.but_enableLogging.setText("Logging Enabled")
             self.but_enableLogging.setStyleSheet("QPushButton {background-color: coral;}")
-            # self.gui.logFile.logToFile(None, self.gui.appSettings['reqIP'])
+            # self.gui.logFile.logToFile(None, self.gui.appSettings['reqRadio'])
 # Sets whether logs are one large file or broken up by a determined length of time.
     def updateLogSegmented(self):
         self.gui.appSettings['segmentTime'] = self.dispSegmentTime.text()
         if self.check_logSegmented.isChecked():
             self.gui.appSettings['logSegmented'] = 1
         else:
             self.gui.appSettings['logSegmented'] = 0
@@ -4150,30 +4264,30 @@
             self.gui.updateConsole(tmp)
         else:
             # self.updateTabs()
             # print("set\n",self.slotMap)
             # print("totalTime", self.slotMapTime)
             if self.gui.connectedRequester == 1:
                 self.makeMap()
-                status = self.gui.radioReq.API.network_SetSlotMap_Request(self.gui.appSettings['reqIP'], self.slotMap,1)
+                status = self.gui.radioReq.API.network_SetSlotMap_Request(self.gui.appSettings['reqRadio'], self.slotMap,1)
                 # print("status:", status)
                 text = "Slotmap sent to radio\n"
                 self.gui.updateConsole(text)
                 self.buttonHandlerGetMap()
             else:
                 text = "Need to connect to a primary radio@!\n"
                 self.gui.updateConsole(text)
                 self.slotMap = [{"slotIdx":0,"slotType":"SLOT_RANGE","configId":0,"ownerId":100,"targetId":101,"period":20,"maxUserData":10}]
                 self.populateMap()
             self.but_slotMapSetMap.setStyleSheet("QPushButton {background-color: SteelBlue; color: GhostWhite;}")
 
 
     def buttonHandlerGetMap(self):
         if self.gui.connectedRequester == 1:
-            status, self.slotMap, addr = self.gui.radioReq.API.network_GetSlotMap_Request(self.gui.appSettings['reqIP'])
+            status, self.slotMap, addr = self.gui.radioReq.API.network_GetSlotMap_Request(self.gui.appSettings['reqRadio'])
             self.slotMap = self.slotMap['NETWORKING_GET_SLOT_MAP_CONFIRM']['slotMap']
         else:
             self.slotMap = []
             text = "Need to connect to a primary radio@!\n"
             self.gui.updateConsole(text)
         # print("getMapStatus", status)
         # print(self.slotMap)
@@ -4250,15 +4364,15 @@
                 self.netMaxNoiseArray.append(maxNoiseArray)
                 self.netStdNoiseArray.append(stdNoiseArray)
         if len(self.localSlots) > 0:
             self.localSlotFirst = self.localSlots[0][0]
             self.localSlotLast = self.localSlots[len(self.localSlots)-1][0]
 
     def buttonHandlerShowStats(self):
-        status, stats, addr = self.gui.radioReq.API.network_Stats_Request(self.gui.appSettings['reqIP'])
+        status, stats, addr = self.gui.radioReq.API.network_Stats_Request(self.gui.appSettings['reqRadio'])
         print(stats)
 
     def buttonHandlerLoadMap(self):
         self.clearMap()
         filename = QFileDialog.getOpenFileName(self, 'Open SlotMap File', "./slotMaps/slotMap.map", "map (*.map)")
         filename = filename[0]
         f = open(filename, "r")
@@ -4292,27 +4406,27 @@
         except:
             print("== Invalid filename, save aborted")
             text = "== Invalid filename, save aborted\n"
             self.gui.updateConsole(text)
 
     def buttonHandlerNetworkToggle(self):
         if self.gui.connectedRequester == 1:
-            self.gui.radioStateReq,addr = self.gui.radioReq.API.radio_GetState_Request(self.gui.appSettings['reqIP'])
+            self.gui.radioStateReq,addr = self.gui.radioReq.API.radio_GetState_Request(self.gui.appSettings['reqRadio'])
             if self.gui.radioMode == 'idle':
                 self.savedNodeId = self.gui.dispRespID.text() # network changes this while running, so save value before network start
                 status = self.gui.radioRanging.rangingSetup('networking')
                 if status == True:
                     # setup the networking state
                     self.gui.radioStateReq[list([self.gui.radioStateReq.keys()][0])[0]]['state'] = "RADIO_STATE_NETWORKING"
                     self.layoutTop.itemAt(len(self.layoutTop)-1).widget().setText("Stop Network")
                     self.layoutTop.itemAt(len(self.layoutTop)-1).widget().setStyleSheet("QPushButton {background-color: coral; color: black;}")
                     self.gui.radioMode = 'networking'
                     self.gui.radioStateReq[list([self.gui.radioStateReq.keys()][0])[0]]['flags']  = ""
                     self.gui.radioStateReq[list([self.gui.radioStateReq.keys()][0])[0]]['persistFlag'] = 1
-                    self.gui.radioReq.API.radio_SetState_Request(self.gui.appSettings['reqIP'],self.gui.radioStateReq)
+                    self.gui.radioReq.API.radio_SetState_Request(self.gui.appSettings['reqRadio'],self.gui.radioStateReq)
                     self.gui.windowDataTransfer.radioData.reqMsgTimer.stop()
                     self.gui.windowDataTransfer.radioData.respMsgTimer.stop()
                     self.updateDestMenu()
                     self.resetDataArrays()
                     self.gui.checkChartRange(None)
                     # clear the stale messages
                     for i in self.gui.radioReq.messageQueues:
@@ -4337,15 +4451,15 @@
                     self.layoutTop.itemAt(len(self.layoutTop)-1).widget().setStyleSheet("QPushButton {background-color: SteelBlue; color: GhostWhite;}")
                     self.gui.radioMode = 'idle'
                     self.gui.radioRanging.networkTimer.stop()
                     # self.gui.guiUpdateTimer.stop()
                     self.netGuiTimer.stop()
                     self.gui.radioStateReq[list([self.gui.radioStateReq.keys()][0])[0]]['flags']  = ""
                     self.gui.radioStateReq[list([self.gui.radioStateReq.keys()][0])[0]]['persistFlag'] = 1
-                    self.gui.radioReq.API.radio_SetState_Request(self.gui.appSettings['reqIP'],self.gui.radioStateReq)
+                    self.gui.radioReq.API.radio_SetState_Request(self.gui.appSettings['reqRadio'],self.gui.radioStateReq)
                     if self.gui.connectedResponder == 1:
                         self.gui.windowDataTransfer.radioData.respMsgTimer.start()
                     if self.gui.connectedRequester == 1:
                         self.gui.windowDataTransfer.radioData.reqMsgTimer.start()
                     text = "\n==============\n Network Stopping\n"
                     self.gui.updateConsole(text)
                 else:
```

### Comparing `TDSR-UWB-1.535/TDSR-UWB/TDSR_Support/TDSR_logging.py` & `TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/TDSR_logging.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from datetime import datetime, date
 from time import time
 from pathlib import Path
 from os import path, mkdir, makedirs
 from json import dumps
 
-__version__ = "1.535"
+__version__ = "1.536"
 
 # All application data logging functions
 class logData():
     def __init__(self, gui):
         self.gui = gui
         self.settings = gui.appSettings
         self.logFile = ""
```

### Comparing `TDSR-UWB-1.535/TDSR-UWB/TDSR_Support/TDSR_radioAPI.py` & `TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/TDSR_radioAPI.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from json import dumps
+from time import sleep
 
-__version__ = "1.535"
+__version__ = "1.536"
 
 class RadioAPI:
     _msgId = 0
 
     def __init__(self, messageQueues, messageList, TxQueue):
         self.TxQueue = TxQueue
         self.messageList = messageList
@@ -209,15 +210,15 @@
 # Ranging Command section
     def range_Send_Request(self,ip, responderId, encoding, data):
         message = self.getMessageFromList('RANGE_SEND_RANGE_REQUEST')
         message[list(message.keys())[0]]['responderId'] = responderId
         message[list(message.keys())[0]]['encoding'] = "ENCODING_BASE64"
         message[list(message.keys())[0]]['data'] = data
         status, packet, addr = self.readPacketRequestConfirm(message,'RANGE_SEND_RANGE_CONFIRM',ip,retryCount  = 1 )
-        return packet,addr
+        return status,packet,addr
 
     def getMessageFromList(self,messageName):
         messages = [value for key, value in self.messageList.items() if messageName.upper() in key.upper()]
         #for key, value in self.messageList.items():
             #print(key.upper())
         # print(messages)
         if (messages):
@@ -247,27 +248,30 @@
         if rxMessageName in self.messageQueues.keys():
             # print(f"Found: {rxMessageName}")
             try:
                 packet = self.messageQueues[rxMessageName].get(timeout = 0.1)
                 # print("Got: ", rxMessageName)
                 # print(f'{packet}\n')
             except:
+                print("failed queue")
                 print(f"Missed a {rxMessageName} packet")
                 status = False
                 pass
         else:
             # otherwise, if it's a comfirm message, draw from the general confirm.
             if "CONFIRM" in rxMessageName:
                 # print(f"General Confirm: {rxMessageName}")
                 try:
                     # print(time.time())
                     packet = self.messageQueues['General_Confirm'].get(timeout = 0.4)
                     # print(f'{packet}\n')
                 except:
                     print(f"Missed a {rxMessageName} message")
+                    # print("I'm here")
+                    print(packet)
                     # print(time.time())
                     status = False
                     pass
             else:
                 # should never really land here since message wasn't a confirm request.
                 print(f"Looking For: {rxMessageName}")
                 while not self.messageQueues['General_Msg'].empty():
```

### Comparing `TDSR-UWB-1.535/TDSR-UWB/TDSR_Support/TDSR_radioControl.py` & `TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/TDSR_radioControl.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from time import time, sleep
 from math import sqrt, log10
 from numpy import power
 from pathlib import Path
 from base64 import b64encode, b64decode
 from threading import Thread
 
-__version__ = "1.535"
+__version__ = "1.536"
 
 # Primary ranging functions
 class rangeCmds():
     def __init__(self, gui):
         self.gui = gui
         self.appSetup()
 
@@ -35,27 +35,28 @@
         self.networkTimer.setInterval(10)
         self.networkTimer.timeout.connect(self.networkCheck)
         self.rangeArray = []
         self.rangeFilteredArray = []
         self.rangeFPPArray = []
         self.chartPointsX = []
         self.packetDisplay = None
+        self.missedComms = 0
 
 # Runs on startup and before each ranging run. Resets everything to known state.
     def rangingSetup(self, mode):
         # confirm radio is connected at each ranging start
         status = False
         self.gui.radioConnectReq()
         self.rangeCountValid = 0
         if self.gui.connectedRequester == 1:
-            status, msg, addr = self.gui.radioReq.API.network_GetSlotMap_Request(self.gui.appSettings['reqIP'])
+            status, msg, addr = self.gui.radioReq.API.network_GetSlotMap_Request(self.gui.appSettings['reqRadio'])
             if msg:
                 self.gui.windowNetwork.slotMap = msg['NETWORKING_GET_SLOT_MAP_CONFIRM']['slotMap']
-            self.gui.appSettings['reqIP'] = self.gui.dispReqIP.text()
-            self.gui.appSettings['respIP'] = self.gui.dispRespIP.text()
+            self.gui.appSettings['reqRadio'] = self.gui.dropMenuReqRadio.currentText()
+            self.gui.appSettings['respRadio'] = self.gui.dropMenuRespRadio.currentText()
             self.gui.updateMemoryDepth()
             if (self.gui.dispReqID.text() == self.gui.dispRespID.text()) or self.gui.dispReqID.text() == "-":
                 if self.gui.dispReqID.text() == "-":
                     text = "  == ERROR, invalid requester nodeID ==\n"
                 else:
                     text = "  == ERROR, requester and responder must have different nodeIDs ==\n"
                 self.gui.updateConsole(text)
@@ -101,39 +102,42 @@
             self.rangeFPPowerSum = 0
             self.packetDisplay = None
             self.rangeCount = 0
             self.rangeCountValid = 0
             self.rangeTimeArray = []
             if self.gui.radioMode == 'idle':
                 self.gui.updateRunTotal()
-                self.nodeIPs.append(self.gui.appSettings['reqIP'])
+                self.nodeIPs.append(self.gui.appSettings['reqRadio'])
                 self.targetNodes = int(self.gui.dispRespID.text())
                 if self.gui.connectedResponder == 1:
-                    self.gui.radioStateResp, addr = self.gui.radioResp.API.radio_GetState_Request(self.gui.appSettings['respIP'])
+                    self.gui.radioStateResp, addr = self.gui.radioResp.API.radio_GetState_Request(self.gui.appSettings['respRadio'])
                     self.gui.radioStateResp[list([self.gui.radioStateResp.keys()][0])[0]]['flags']  = ""
                     self.gui.radioStateResp[list([self.gui.radioStateResp.keys()][0])[0]]['state'] ="RADIO_STATE_RANGING"
                     self.gui.radioStateResp[list([self.gui.radioStateResp.keys()][0])[0]]['persistFlag'] = 1
-                    self.gui.radioResp.API.radio_SetState_Request(self.gui.appSettings['respIP'],self.gui.radioStateResp)
+                    self.gui.radioResp.API.radio_SetState_Request(self.gui.appSettings['respRadio'],self.gui.radioStateResp)
                 else:
                     if mode != 'networking':
                         print("Unabled to connect to responder. Make sure it is in active mode.")
                         text =  "Unabled to connect to responder. Make sure it is in active mode.\n"
                         self.gui.updateConsole(text)
         if self.gui.connectedRequester == 1:
-            status, packet, addr = self.gui.radioReq.API.radio_GetInfo_Request(self.gui.appSettings['reqIP'])
-            self.gui.radioStateReq, addr = self.gui.radioReq.API.radio_GetState_Request(self.gui.appSettings['reqIP'])
+            status, packet, addr = self.gui.radioReq.API.radio_GetInfo_Request(self.gui.appSettings['reqRadio'])
+            self.gui.radioStateReq, addr = self.gui.radioReq.API.radio_GetState_Request(self.gui.appSettings['reqRadio'])
             self.needComma = False
             status = True
         else:   # If couldn't connect, then shutdown run and reset
             status = False
             if mode != 'networking':
                 self.running = 1
                 print("Ranging setup error, can't reach requester, aborting run.")
                 self.rangeTimer.stop()
                 self.toggleRun()
+        if (self.gui.appSettings['reqRadio'] == self.gui.appSettings['respRadio']) and self.gui.appSettings['connectResp'] == 1:
+            print("Ranging setup error. Primary and Secondary radios are the sane.")
+            status = False
         return status
 
 # Procedure for starting a new run or ending a current run depending on the state of self.running when togglerun is called.
     def toggleRun(self):
         if self.running == 0 and self.gui.radioMode == 'idle':
             for i in self.gui.radioReq.messageQueues:
                 while not self.gui.radioReq.messageQueues[i].empty():
@@ -151,19 +155,19 @@
                     self.gui.windowNetwork.netPlot1[i].setData(self.gui.windowNetwork.netXArray, self.gui.windowNetwork.netRangeArray[i])
                     self.gui.windowNetwork.netPlot2[i].setData(self.gui.windowNetwork.netXArray, self.gui.windowNetwork.netRangeArray[i])
                     self.gui.windowNetwork.netPlotT[i].setData(self.gui.windowNetwork.netXArray, self.gui.windowNetwork.netRangeArray[i])
                     self.gui.windowNetwork.netPlotB[i].setData(self.gui.windowNetwork.netXArray, self.gui.windowNetwork.netRangeArray[i])
                 self.gui.plotYT = []
                 self.gui.plotX = []
                 self.gui.chartData1.setData(self.gui.plotX, self.gui.plotYT)
-                self.gui.radioStateReq,addr = self.gui.radioReq.API.radio_GetState_Request(self.gui.appSettings['reqIP'])
+                self.gui.radioStateReq,addr = self.gui.radioReq.API.radio_GetState_Request(self.gui.appSettings['reqRadio'])
                 self.gui.radioStateReq[list([self.gui.radioStateReq.keys()][0])[0]]['state'] = "RADIO_STATE_RANGING"
                 self.gui.radioStateReq[list([self.gui.radioStateReq.keys()][0])[0]]['flags']  = ""
                 self.gui.radioStateReq[list([self.gui.radioStateReq.keys()][0])[0]]['persistFlag'] = 1
-                self.gui.radioReq.API.radio_SetState_Request(self.gui.appSettings['reqIP'],self.gui.radioStateReq)
+                self.gui.radioReq.API.radio_SetState_Request(self.gui.appSettings['reqRadio'],self.gui.radioStateReq)
                 self.gui.windowDataTransfer.dropMenuDestination.clear()
                 self.gui.windowDataTransfer.dropMenuDestination.addItems([str(self.gui.appSettings['respID'])])
                 self.gui.checkChartRange(None)
                 self.runStartTime = time()
                 self.running = 1
                 self.gui.but_run.setText("Stop")
                 self.gui.but_run.setStyleSheet("QPushButton {background-color: coral;}")
@@ -173,24 +177,27 @@
                     # self.rangeTimer.setInterval(int(self.gui.dispRangeDelay.text()))
                     self.rangeTimer.start()
                     self.gui.rangingActive = True
                     self.gui.guiUpdateTimer.start()
                     text = "Executing " + str(self.gui.appSettings['rangeRequests']) + " Ranging Attempts\n"
                     self.gui.updateConsole(text)
                     self.gui.radioMode = 'ranging'
+                    self.gui.radioCheckTimer.stop()
                 else:
                     text = "Could not connect to requester radio, check cables and IP addresses.\n"
                     self.gui.updateConsole(text)
                     self.gui.radioMode = 'idle'
                     self.running = 0
+                    self.gui.radioCheckTimer.start()
             else:
                 text = "Could not connect to requester radio, check cables and IP addresses.\n"
                 self.gui.updateConsole(text)
                 self.gui.radioMode = 'idle'
                 self.running = 0
+                self.gui.radioCheckTimer.start()
         else:
             if self.gui.radioMode == 'networking':
                 text = "=====\nRadio is in Network Mode.\n  Stop network before ranging\n=====\n"
                 self.gui.updateConsole(text)
             else:
                 self.rangeTimer.stop()
                 self.runStopTime = time()
@@ -206,14 +213,15 @@
                 self.gui.but_run.setText("Start\nRanging")
                 self.gui.but_run.setStyleSheet("QPushButton {background-color: SteelBlue; color: GhostWhite;}")
                 self.gui.logFile.closeLogFile()
                 self.computeRunStats()
                 self.gui.guiUpdateTimer.stop()
                 self.gui.updateGUI()
                 self.gui.radioMode = 'idle'
+                self.gui.radioCheckTimer.start()
 
     def networkCheck(self):
         if self.gui.connectedRequester == 1:
             self.networkTimer.stop()
             while not self.gui.radioReq.messageQueues['RANGE_INFO'].empty():
                 packet =  self.gui.radioReq.messageQueues['RANGE_INFO'].get()
                 slot = int(packet['RANGE_INFO']['slotIdx'])
@@ -222,46 +230,55 @@
                 packet =  self.gui.radioReq.messageQueues['DATA_INFO'].get()
                 self.gui.windowDataTransfer.radioData.processNetworkDataInfo(packet)
             self.networkTimer.start()
 
 # Requests range from designated responder nodeID.
     def rangeRequest(self):
         self.rangeTimer.stop()
+        if self.missedComms > 4:
+            print("rangeRequest abort")
+            self.gui.radioReq.disconnect()
+            self.gui.dropMenuReqRadio.setCurrentIndex(0)
+            self.missedComms = 0
         if self.gui.connectedRequester == 1:
             self.gui.rangeInProgress = 1
             # if there is data to send, append it to the ranging packet
             if self.gui.windowDataTransfer.radioData.dataReadyStatus > 0:
                 data = self.gui.windowDataTransfer.radioData.getDataPacket()
             else:
                 data = ""
             # if 0 then hold ranges to allow confirmation data packet to come in.
             if self.gui.windowDataTransfer.radioData.dataReadyStatus != 0:
-                self.gui.radioReq.API.range_Send_Request(self.gui.appSettings['reqIP'],self.targetNodes, "ENCODING_BASE64", data)
+                status, pkt, addr = self.gui.radioReq.API.range_Send_Request(self.gui.appSettings['reqRadio'],self.targetNodes, "ENCODING_BASE64", data)
+                if status == False:
+                    self.missedComms = self.missedComms + 1
             if self.gui.windowDataTransfer.radioData.dataReadyStatus == 1:  # indicated last in transmission
                 self.gui.windowDataTransfer.radioData.dataReadyStatus = 0   # enter hold until confirmation cycle
             self.startRange = time()
             # Once range request is set, wait for answer and process the data
             self.rangeProcessData(None)
         else:
-            text = "== Not connected to Requester IP Address" + self.gui.appSettings['reqIP'] + " ==\n"
+            text = "== Not connected to Requester Radio" + self.gui.appSettings['reqRadio'] + " ==\n"
             self.gui.updateConsole(text)
             print("Ranging requested while not connected to requester, aborting run.")
             self.toggleRun()
 
 # Processes ranging data when it comes in from the API
     def rangeProcessData(self, packet):
         if packet == None: # case for ranging mode
             try:
                 packet = self.gui.radioReq.messageQueues['RANGE_INFO'].get(timeout = 0.2)
             except:
-                print("Miss")
+                # print("Miss")
                 packet = {"RANGE_INFO":{"rangeStatus":4,"precisionRangeM":0.0,"rxPower":0.0}}
                 packet['RANGE_INFO']['rangeStatus'] = 4
                 packet['RANGE_INFO']['precisionRangeM'] = 0.0
                 packet['RANGE_INFO']['filteredRangeM'] = 0.0
+                packet['RANGE_INFO']['maxNoise'] = 0.0
+                packet['RANGE_INFO']['stdNoise'] = 0.0
                 pass
         # If count = desired requests then stop run, otherwise, range transaction is complete, start the next one.
             self.gui.rangeInProgress = False
             if self.rangeCount == self.gui.appSettings['rangeRequests']:
                 print("Run Complete.")
                 self.toggleRun()
             else:
@@ -549,27 +566,27 @@
             command = {"retries":0, "msgType":"d","destination":dest, "slot":slot, "order":order, "msgNum":self.sendCount, "payload":dataPacket}
             # print("Sending:",command)
             if self.sendCount == 1:
                 tmp = f"Sending: {len(self.packetList) + 1} packets\n"
                 self.gui.updateConsole(tmp)
             # print(f"Sending: {self.sendCount}")
             self.networkConfirmQueue.append(command)
-            self.gui.radioReq.API.dataSend_B64_Request(self.gui.appSettings['reqIP'],dest, slot, order, dataPacket)
+            self.gui.radioReq.API.dataSend_B64_Request(self.gui.appSettings['reqRadio'],dest, slot, order, dataPacket)
             self.networkDataTXAbortTimer.start()
 
     def reqSendTextData(self):
         text = self.gui.windowDataTransfer.dataTextInput.toPlainText()
         msgNum = 1
         text = f"t1,{msgNum},{text}"
         text = self.toBase64(text)
         self.gui.windowDataTransfer.updateDropMenuDest()
         dest = self.gui.windowDataTransfer.dataDestination
         slot = self.gui.windowDataTransfer.dataDestinationSlot
         order = "front"
-        localIP = self.gui.appSettings['reqIP']
+        localIP = self.gui.appSettings['reqRadio']
         if self.gui.radioMode == 'networking':
             if self.gui.windowDataTransfer.dataBackSlot >= 0:
                 command = {"retries":0, "msgType":"t", "destination":dest, "slot":slot, "order":order, "msgNum":msgNum, "payload":text}
                 self.networkConfirmQueue.insert(0,command)
                 self.networkDataTXAbortTimer.start()
             else:
                 tmp = "Sending text but no confirm slot available\n"
@@ -806,15 +823,15 @@
             order = "front"
         slotFound = False
         for k in range(len(self.gui.windowNetwork.localSlots)):
             if self.gui.windowNetwork.localSlots[k][1] == fromID:
                 slot = self.gui.windowNetwork.localSlots[k][0]
                 slotFound = True
         if slotFound == True:
-            self.gui.radioReq.API.dataSend_B64_Request(self.gui.appSettings['reqIP'], dest, slot, order, msg)
+            self.gui.radioReq.API.dataSend_B64_Request(self.gui.appSettings['reqRadio'], dest, slot, order, msg)
             if str(msgType) == "t" or str(msgType) == "a":
                 if str(msgType) == "t":
                     print("Confirming Text Message")
                 else:
                     print("Confirming Tranfer Abort")
             else:
                 # print(f"Confirming: {msgNum} out of {self.lastMsgExpected}")
@@ -829,15 +846,15 @@
         self.networkDataTXAbortTimer.stop()
         if len(self.networkConfirmQueue) > 0:
             command = self.networkConfirmQueue[0]
             self.networkConfirmQueue = self.networkConfirmQueue[1:]
             # resends oldest data in resend queue to the front of the transmit line
             print(f"### Resending {command['msgNum']} ###")
             self.txResendCount = self.txResendCount + 1
-            localIP = self.gui.appSettings['reqIP']
+            localIP = self.gui.appSettings['reqRadio']
             self.gui.radioReq.API.dataSend_B64_Request(localIP, command["destination"], command["slot"], "front", command["payload"])
             command["retries"] = command["retries"] + 1
             self.networkConfirmQueue.append(command)
             self.networkDataTXAbortTimer.start()
 
     def networkDataAbort(self):
         # print(force)
@@ -878,15 +895,15 @@
         msgID = 1
         msg = f"a1,{str(msgID)},{str(msgType)},{str(msgNum)}"
         msg = self.toBase64(msg)
         self.gui.windowDataTransfer.updateDropMenuDest()
         dest = self.gui.windowDataTransfer.dataDestination
         slot = self.gui.windowDataTransfer.dataDestinationSlot
         order = "front"
-        localIP = self.gui.appSettings['reqIP']
+        localIP = self.gui.appSettings['reqRadio']
         command = {"retries":0, "msgType":"a", "destination":dest, "slot":slot, "order":order, "msgNum":msgNum, "payload":msg}
         self.networkConfirmQueue.insert(0,command)
         self.networkDataTXAbortTimer.start()
         self.gui.radioReq.API.dataSend_B64_Request(localIP, dest, slot, order, msg)
 
     ####################
     # Ranging and Data Mode Specific Commands
@@ -1004,28 +1021,28 @@
                                     print("New Last should be:", self.lastMsgExpected)
                                 else:
                                     self.lastMsgExpected = 0
                             self.rxResendCount = self.rxResendCount + len(self.rxMissingList)
                             # if we found misses, then ask for a resend of all of them
                             slot = self.gui.windowDataTransfer.dataDestinationSlot
                             dest = self.gui.windowDataTransfer.dataDestination
-                            src = self.gui.appSettings['reqIP']
+                            src = self.gui.appSettings['reqRadio']
                             order = "queue"
                             if self.lastMsgExpected != 0:
                                 print("Requesting following missed packets:", self.rxMissingList)
                                 tmp = "c1," + str(self.rxMissingList)
                                 # print(tmp)
                                 tmp = tmp.encode()
                                 tmp = b64encode(tmp)
                                 tmp = tmp.decode('utf-8')
                                 slot = self.gui.windowDataTransfer.dataDestinationSlot
                                 # print(src, dest, slot, order, tmp)
                                 self.rxAbortTimer.start()
                                 self.gui.radioReq.API.dataSend_B64_Request(src, dest, slot, order, tmp)
-                                # self.gui.radioReq.API.dataSend_B64_Request(self.gui.appSettings['reqIP'],int(self.gui.windowDataTransfer.dropMenuDestination.currentText()), tmp)
+                                # self.gui.radioReq.API.dataSend_B64_Request(self.gui.appSettings['reqRadio'],int(self.gui.windowDataTransfer.dropMenuDestination.currentText()), tmp)
                             # if we didn't find any misses, then save the file.
                             else:
                                 tmp = "c1," + str(self.rxMissingList)
                                 tmp = tmp.encode()
                                 tmp = b64encode(tmp)
                                 tmp = tmp.decode('utf-8')
                                 self.gui.radioReq.API.dataSend_B64_Request(src, dest, slot, order, tmp)
@@ -1148,34 +1165,34 @@
                                     print("New Last should be:", self.lastMsgExpected)
                                 else:
                                     self.lastMsgExpected = 0
                             self.rxResendCount = self.rxResendCount + len(self.rxMissingList)
                             # if we found misses, then ask for a resend of all of them
                             slot = self.gui.windowDataTransfer.dataDestinationSlot
                             dest = self.gui.windowDataTransfer.dataDestination
-                            src = self.gui.appSettings['reqIP']
+                            src = self.gui.appSettings['reqRadio']
                             order = "queue"
                             if self.lastMsgExpected != 0:
                                 print("Requesting following missed packets:", self.rxMissingList)
                                 tmp = "c1," + str(self.rxMissingList)
                                 tmp = tmp.encode()
                                 tmp = b64encode(tmp)
                                 tmp = tmp.decode('utf-8')
                                 slot = self.gui.windowDataTransfer.dataDestinationSlot
                                 self.rxAbortTimer.start()
                                 self.gui.radioReq.API.dataSend_B64_Request(src, dest, slot, order, tmp)
-                                # self.gui.radioResp.API.dataSend_B64_Request(self.gui.appSettings['respIP'], int(srcNode), slot, order, tmp)
+                                # self.gui.radioResp.API.dataSend_B64_Request(self.gui.appSettings['respRadio'], int(srcNode), slot, order, tmp)
                             # if we didn't find any misses, then save the file.
                             else:
                                 tmp = "c1," + str(self.rxMissingList)
                                 tmp = tmp.encode()
                                 tmp = b64encode(tmp)
                                 tmp = tmp.decode('utf-8')
                                 self.gui.radioReq.API.dataSend_B64_Request(src, dest, slot, order, tmp)
-                                # self.gui.radioResp.API.dataSend_B64_Request(self.gui.appSettings['respIP'], int(srcNode), slot, order, tmp)
+                                # self.gui.radioResp.API.dataSend_B64_Request(self.gui.appSettings['respRadio'], int(srcNode), slot, order, tmp)
                                 self.startBuild = time()
                                 if len(self.rxMissingList) == 0:
                                     self.packetBuffer = ""
                                     tmp = "Building file from packet array\n"
                                     self.gui.updateConsole(tmp)
                                     self.threadRunningRx = 1
                                     rxPacketBuild = Thread(target=self.threadRxPacketBuild, daemon=True)
@@ -1197,15 +1214,15 @@
         if not self.gui.rangingActive:
             # while self.sendCount != (len(self.packetList)):
             dataPacket = self.getDataPacket()
             order = "queue"
             dest = self.gui.windowDataTransfer.dataDestination
             msgNum = self.sendCount
             slot = 0
-            self.gui.radioReq.API.dataSend_B64_Request(self.gui.appSettings['reqIP'],dest, slot, order, dataPacket)
+            self.gui.radioReq.API.dataSend_B64_Request(self.gui.appSettings['reqRadio'],dest, slot, order, dataPacket)
 
     def getDataPacket(self):
         dataPacket = self.packetList[self.sendCount]
         if self.sendCount != (len(self.packetList)-1):
             if (self.sendCount % 250) == 0 and self.sendCount > 1:
                 text = "Sent " + str(self.sendCount) + " of " + str(len(self.packetList)) + " packets.\n"
                 self.gui.updateConsole(text)
@@ -1286,15 +1303,15 @@
         msgID = 1
         msg = f"a1,{str(msgID)},{str(msgType)},{str(msgNum)}"
         msg = self.toBase64(msg)
         self.gui.windowDataTransfer.updateDropMenuDest()
         dest = self.gui.windowDataTransfer.dataDestination
         slot = 0
         order = "front"
-        localIP = self.gui.appSettings['reqIP']
+        localIP = self.gui.appSettings['reqRadio']
         self.gui.radioReq.API.dataSend_B64_Request(localIP, dest, slot, order, msg)
 
     def processDataAbort(self):
         self.rxAbortTimer.stop()
         text = "\n== Transfer aborted by sender ==\n"
         print(text)
         self.gui.updateConsole(text)
```

### Comparing `TDSR-UWB-1.535/TDSR-UWB/TDSR_Support/TDSR_settings.py` & `TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/TDSR_settings.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from pathlib import Path
 from json import dumps, loads
 
-__version__ = "1.535"
+__version__ = "1.536"
 
 # loads and saves GUI settings. Also sets default values if settings file does not include all keys.
 class appSettings():
     def __init__(self):
         self.settings = {}
 
     def settingsSetup(self):
@@ -21,18 +21,18 @@
                 self.settings['connectResp'] = 0
             if 'chartDepth' not in self.settings:
                 self.settings['chartDepth'] = 5000
             if 'memoryDepth' not in self.settings:
                 self.settings['memoryDepth'] = 250000
             if 'rangeRequests' not in self.settings:
                 self.settings['rangeRequests'] = 250
-            if 'reqIP' not in self.settings:
-                self.settings['reqIP'] = "192.168.1.100"
-            if 'respIP' not in self.settings:
-                self.settings['respIP'] = "192.168.1.101"
+            if 'reqRadio' not in self.settings:
+                self.settings['reqRadio'] = "192.168.1.100"
+            if 'respRadio' not in self.settings:
+                self.settings['respRadio'] = "192.168.1.101"
             if 'respID' not in self.settings:
                 self.settings['respID'] = "101"
             if 'logDirectory' not in self.settings:
                 self.settings['logDirectory'] = "./data_directory/"
             if 'logFile' not in self.settings:
                 self.settings['logFile'] = "logfile.log"
             if 'logJson' not in self.settings:
@@ -56,16 +56,16 @@
         else:
             print("Creating Default Settings File")
             self.settings['showDrops'] = 0
             self.settings['connectResp'] = 0
             self.settings['chartDepth'] = 5000
             self.settings['memoryDepth'] = 250000
             self.settings['rangeRequests'] = 250
-            self.settings['reqIP'] = "192.168.1.51"
-            self.settings['respIP'] = "192.168.1.52"
+            self.settings['reqRadio'] = "192.168.1.51"
+            self.settings['respRadio'] = "192.168.1.52"
             self.settings['respID'] = "52"
             self.settings['logDirectory'] = "./data_directory/"
             self.settings['logFile'] = "logfile.log"
             self.settings['logJson'] = 1
             self.settings['enableLogging'] = 0
             self.settings['logRangeInfoOnly'] = 1
             self.settings['logDateBased'] = 0
```

### Comparing `TDSR-UWB-1.535/TDSR-UWB/TDSR_Support/crc16.py` & `TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/crc16.py`

 * *Files identical despite different names*

### Comparing `TDSR-UWB-1.535/TDSR-UWB/TDSR_Support/logReader.py` & `TDSR-UWB-1.536/TDSR-UWB/TDSR_Support/logReader.py`

 * *Files identical despite different names*

### Comparing `TDSR-UWB-1.535/TDSR-UWB/TDSR_UWB.egg-info/PKG-INFO` & `TDSR-UWB-1.536/TDSR-UWB/TDSR_UWB.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TDSR-UWB
-Version: 1.535
+Version: 1.536
 Summary: Support libraries for TDSR LLC UWB Radios
 Home-page: UNKNOWN
 Author: TDSR-LLC
 Author-email: contact@tdsr-uwb.com
 License: UNKNOWN
 Project-URL: Company:, https://www.tdsr-uwb.com
 Platform: UNKNOWN
```

### Comparing `TDSR-UWB-1.535/TDSR-UWB/TDSR_UWB.egg-info/SOURCES.txt` & `TDSR-UWB-1.536/TDSR-UWB/TDSR_UWB.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `TDSR-UWB-1.535/setup.py` & `TDSR-UWB-1.536/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     name="TDSR-UWB",  # Required
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/guides/single-sourcing-package-version/
-    version="1.535",  # Required
+    version="1.536",  # Required
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description="Support libraries for TDSR LLC UWB Radios",  # Optional
     # This is an optional longer description of your project that represents
     # the body of text which users will see when they visit PyPI.
     #
```

