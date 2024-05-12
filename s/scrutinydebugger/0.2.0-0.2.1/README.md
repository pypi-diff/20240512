# Comparing `tmp/scrutinydebugger-0.2.0.tar.gz` & `tmp/scrutinydebugger-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrutinydebugger-0.2.0.tar", last modified: Sat May  4 13:41:43 2024, max compression
+gzip compressed data, was "scrutinydebugger-0.2.1.tar", last modified: Sun May 12 14:48:17 2024, max compression
```

## Comparing `scrutinydebugger-0.2.0.tar` & `scrutinydebugger-0.2.1.tar`

### file list

```diff
@@ -1,145 +1,146 @@
-drwxrwxr-x   0 py        (1000) py        (1000)        0 2024-05-04 13:41:43.279700 scrutinydebugger-0.2.0/
--rw-rw-r--   0 py        (1000) py        (1000)     1073 2024-03-25 03:09:50.000000 scrutinydebugger-0.2.0/LICENSE
--rw-r--r--   0 py        (1000) py        (1000)      887 2024-05-04 13:41:43.279700 scrutinydebugger-0.2.0/PKG-INFO
--rw-rw-r--   0 py        (1000) py        (1000)      596 2024-04-11 01:05:46.000000 scrutinydebugger-0.2.0/README.md
-drwxrwxr-x   0 py        (1000) py        (1000)        0 2024-05-04 13:41:43.259700 scrutinydebugger-0.2.0/scrutiny/
--rw-rw-r--   0 py        (1000) py        (1000)      188 2024-05-04 13:40:52.000000 scrutinydebugger-0.2.0/scrutiny/__init__.py
--rw-rw-r--   0 py        (1000) py        (1000)      453 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.0/scrutiny/__main__.py
-drwxrwxr-x   0 py        (1000) py        (1000)        0 2024-05-04 13:41:43.259700 scrutinydebugger-0.2.0/scrutiny/cli/
--rw-rw-r--   0 py        (1000) py        (1000)       39 2024-03-25 02:32:28.000000 scrutinydebugger-0.2.0/scrutiny/cli/__init__.py
--rw-rw-r--   0 py        (1000) py        (1000)     5089 2024-04-15 01:53:14.000000 scrutinydebugger-0.2.0/scrutiny/cli/cli.py
-drwxrwxr-x   0 py        (1000) py        (1000)        0 2024-05-04 13:41:43.263700 scrutinydebugger-0.2.0/scrutiny/cli/commands/
--rw-rw-r--   0 py        (1000) py        (1000)     1577 2024-03-25 02:32:28.000000 scrutinydebugger-0.2.0/scrutiny/cli/commands/__init__.py
--rw-rw-r--   0 py        (1000) py        (1000)     5166 2024-04-15 02:52:23.000000 scrutinydebugger-0.2.0/scrutiny/cli/commands/add_alias.py
--rw-rw-r--   0 py        (1000) py        (1000)     1431 2024-04-15 01:53:14.000000 scrutinydebugger-0.2.0/scrutiny/cli/commands/base_command.py
--rw-rw-r--   0 py        (1000) py        (1000)     2774 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.0/scrutiny/cli/commands/datalog_info.py
--rw-rw-r--   0 py        (1000) py        (1000)     1481 2024-04-15 01:53:14.000000 scrutinydebugger-0.2.0/scrutiny/cli/commands/delete_datalog.py
--rw-rw-r--   0 py        (1000) py        (1000)     2148 2024-04-15 01:53:14.000000 scrutinydebugger-0.2.0/scrutiny/cli/commands/elf2varmap.py
--rw-rw-r--   0 py        (1000) py        (1000)     1699 2024-04-15 01:53:14.000000 scrutinydebugger-0.2.0/scrutiny/cli/commands/export_datalog.py
--rw-rw-r--   0 py        (1000) py        (1000)     2082 2024-04-15 01:53:14.000000 scrutinydebugger-0.2.0/scrutiny/cli/commands/get_firmware_id.py
--rw-rw-r--   0 py        (1000) py        (1000)     1314 2024-04-15 01:53:14.000000 scrutinydebugger-0.2.0/scrutiny/cli/commands/install_sfd.py
--rw-rw-r--   0 py        (1000) py        (1000)     2024 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.0/scrutiny/cli/commands/launch_server.py
--rw-rw-r--   0 py        (1000) py        (1000)     5569 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.0/scrutiny/cli/commands/list_datalog.py
--rw-rw-r--   0 py        (1000) py        (1000)     3746 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.0/scrutiny/cli/commands/list_sfd.py
--rw-rw-r--   0 py        (1000) py        (1000)     2880 2024-04-15 01:53:14.000000 scrutinydebugger-0.2.0/scrutiny/cli/commands/make_metadata.py
--rw-rw-r--   0 py        (1000) py        (1000)     1641 2024-04-15 01:53:14.000000 scrutinydebugger-0.2.0/scrutiny/cli/commands/make_sfd.py
--rw-rw-r--   0 py        (1000) py        (1000)     3618 2024-04-15 01:53:14.000000 scrutinydebugger-0.2.0/scrutiny/cli/commands/runtest.py
--rw-rw-r--   0 py        (1000) py        (1000)     1970 2024-04-15 01:53:14.000000 scrutinydebugger-0.2.0/scrutiny/cli/commands/tag_firmware_id.py
--rw-rw-r--   0 py        (1000) py        (1000)     1498 2024-04-22 02:42:58.000000 scrutinydebugger-0.2.0/scrutiny/cli/commands/uninstall_sfd.py
-drwxrwxr-x   0 py        (1000) py        (1000)        0 2024-05-04 13:41:43.263700 scrutinydebugger-0.2.0/scrutiny/core/
--rw-rw-r--   0 py        (1000) py        (1000)        0 2024-03-25 02:32:28.000000 scrutinydebugger-0.2.0/scrutiny/core/__init__.py
--rw-rw-r--   0 py        (1000) py        (1000)     7134 2024-04-22 02:42:58.000000 scrutinydebugger-0.2.0/scrutiny/core/alias.py
--rw-rw-r--   0 py        (1000) py        (1000)     5938 2024-04-11 01:05:46.000000 scrutinydebugger-0.2.0/scrutiny/core/basic_types.py
-drwxrwxr-x   0 py        (1000) py        (1000)        0 2024-05-04 13:41:43.263700 scrutinydebugger-0.2.0/scrutiny/core/bintools/
--rw-rw-r--   0 py        (1000) py        (1000)        0 2024-03-25 02:32:28.000000 scrutinydebugger-0.2.0/scrutiny/core/bintools/__init__.py
--rw-rw-r--   0 py        (1000) py        (1000)     1924 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.0/scrutiny/core/bintools/demangler.py
--rw-rw-r--   0 py        (1000) py        (1000)    31787 2024-05-03 19:11:00.000000 scrutinydebugger-0.2.0/scrutiny/core/bintools/elf_dwarf_var_extractor.py
--rw-rw-r--   0 py        (1000) py        (1000)      223 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.0/scrutiny/core/bintools/elftools_stubs.py
--rw-rw-r--   0 py        (1000) py        (1000)      547 2024-04-15 01:53:14.000000 scrutinydebugger-0.2.0/scrutiny/core/bintools/elftools_stubs.pyi
--rw-rw-r--   0 py        (1000) py        (1000)      755 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.0/scrutiny/core/bintools/get_var_memrange.py
--rw-rw-r--   0 py        (1000) py        (1000)     5385 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.0/scrutiny/core/codecs.py
--rw-rw-r--   0 py        (1000) py        (1000)     7670 2024-04-21 14:05:12.000000 scrutinydebugger-0.2.0/scrutiny/core/datalogging.py
--rw-rw-r--   0 py        (1000) py        (1000)    10600 2024-04-21 03:45:36.000000 scrutinydebugger-0.2.0/scrutiny/core/firmware_description.py
--rw-rw-r--   0 py        (1000) py        (1000)      402 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.0/scrutiny/core/firmware_id.py
--rw-rw-r--   0 py        (1000) py        (1000)     3653 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.0/scrutiny/core/firmware_parser.py
--rw-rw-r--   0 py        (1000) py        (1000)    14117 2024-04-22 02:42:58.000000 scrutinydebugger-0.2.0/scrutiny/core/memory_content.py
--rw-rw-r--   0 py        (1000) py        (1000)     6939 2024-04-15 02:52:23.000000 scrutinydebugger-0.2.0/scrutiny/core/sfd_storage.py
--rw-rw-r--   0 py        (1000) py        (1000)      787 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.0/scrutiny/core/typehints.py
--rw-rw-r--   0 py        (1000) py        (1000)     3000 2024-04-11 01:05:46.000000 scrutinydebugger-0.2.0/scrutiny/core/validation.py
--rw-rw-r--   0 py        (1000) py        (1000)    13755 2024-05-03 19:11:00.000000 scrutinydebugger-0.2.0/scrutiny/core/variable.py
--rw-rw-r--   0 py        (1000) py        (1000)    10690 2024-04-15 01:53:14.000000 scrutinydebugger-0.2.0/scrutiny/core/varmap.py
--rw-rw-r--   0 py        (1000) py        (1000)      290 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.0/scrutiny/exceptions.py
--rw-rw-r--   0 py        (1000) py        (1000)        0 2024-03-27 04:12:19.000000 scrutinydebugger-0.2.0/scrutiny/py.typed
-drwxrwxr-x   0 py        (1000) py        (1000)        0 2024-05-04 13:41:43.267700 scrutinydebugger-0.2.0/scrutiny/sdk/
--rw-rw-r--   0 py        (1000) py        (1000)      350 2024-03-25 02:32:28.000000 scrutinydebugger-0.2.0/scrutiny/sdk/__init__.py
--rw-rw-r--   0 py        (1000) py        (1000)    35478 2024-04-22 02:42:58.000000 scrutinydebugger-0.2.0/scrutiny/sdk/_api_parser.py
--rw-rw-r--   0 py        (1000) py        (1000)    73474 2024-04-11 01:05:46.000000 scrutinydebugger-0.2.0/scrutiny/sdk/client.py
--rw-rw-r--   0 py        (1000) py        (1000)    23098 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.0/scrutiny/sdk/datalogging.py
--rw-rw-r--   0 py        (1000) py        (1000)    13027 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.0/scrutiny/sdk/definitions.py
--rw-rw-r--   0 py        (1000) py        (1000)     1539 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.0/scrutiny/sdk/exceptions.py
-drwxrwxr-x   0 py        (1000) py        (1000)        0 2024-05-04 13:41:43.267700 scrutinydebugger-0.2.0/scrutiny/sdk/listeners/
--rw-rw-r--   0 py        (1000) py        (1000)    11930 2024-04-11 01:05:46.000000 scrutinydebugger-0.2.0/scrutiny/sdk/listeners/__init__.py
--rw-rw-r--   0 py        (1000) py        (1000)     1365 2024-04-11 01:05:46.000000 scrutinydebugger-0.2.0/scrutiny/sdk/listeners/buffered_reader_listener.py
--rw-rw-r--   0 py        (1000) py        (1000)    10506 2024-04-11 01:05:46.000000 scrutinydebugger-0.2.0/scrutiny/sdk/listeners/csv_file_listener.py
--rw-rw-r--   0 py        (1000) py        (1000)     2127 2024-04-11 01:05:46.000000 scrutinydebugger-0.2.0/scrutiny/sdk/listeners/text_stream_listener.py
--rw-rw-r--   0 py        (1000) py        (1000)     9981 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.0/scrutiny/sdk/watchable_handle.py
--rw-rw-r--   0 py        (1000) py        (1000)     3707 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.0/scrutiny/sdk/write_request.py
-drwxrwxr-x   0 py        (1000) py        (1000)        0 2024-05-04 13:41:43.267700 scrutinydebugger-0.2.0/scrutiny/server/
--rw-rw-r--   0 py        (1000) py        (1000)        0 2024-03-25 02:32:28.000000 scrutinydebugger-0.2.0/scrutiny/server/__init__.py
--rw-rw-r--   0 py        (1000) py        (1000)     8039 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.0/scrutiny/server/active_sfd_handler.py
-drwxrwxr-x   0 py        (1000) py        (1000)        0 2024-05-04 13:41:43.267700 scrutinydebugger-0.2.0/scrutiny/server/api/
--rw-rw-r--   0 py        (1000) py        (1000)    79420 2024-04-22 02:42:58.000000 scrutinydebugger-0.2.0/scrutiny/server/api/API.py
--rw-rw-r--   0 py        (1000) py        (1000)       64 2024-03-25 02:32:28.000000 scrutinydebugger-0.2.0/scrutiny/server/api/__init__.py
--rw-rw-r--   0 py        (1000) py        (1000)     1203 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.0/scrutiny/server/api/abstract_client_handler.py
--rw-rw-r--   0 py        (1000) py        (1000)     5976 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.0/scrutiny/server/api/dummy_client_handler.py
--rw-rw-r--   0 py        (1000) py        (1000)    11185 2024-04-22 02:42:58.000000 scrutinydebugger-0.2.0/scrutiny/server/api/typing.py
--rw-rw-r--   0 py        (1000) py        (1000)     2868 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.0/scrutiny/server/api/value_streamer.py
--rw-rw-r--   0 py        (1000) py        (1000)     4652 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.0/scrutiny/server/api/websocket_client_handler.py
-drwxrwxr-x   0 py        (1000) py        (1000)        0 2024-05-04 13:41:43.267700 scrutinydebugger-0.2.0/scrutiny/server/datalogging/
--rw-rw-r--   0 py        (1000) py        (1000)        0 2024-03-25 02:32:28.000000 scrutinydebugger-0.2.0/scrutiny/server/datalogging/__init__.py
--rw-rw-r--   0 py        (1000) py        (1000)    29373 2024-04-22 02:42:58.000000 scrutinydebugger-0.2.0/scrutiny/server/datalogging/datalogging_manager.py
--rw-rw-r--   0 py        (1000) py        (1000)    22438 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.0/scrutiny/server/datalogging/datalogging_storage.py
--rw-rw-r--   0 py        (1000) py        (1000)     2294 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.0/scrutiny/server/datalogging/datalogging_utilities.py
-drwxrwxr-x   0 py        (1000) py        (1000)        0 2024-05-04 13:41:43.271700 scrutinydebugger-0.2.0/scrutiny/server/datalogging/definitions/
--rw-rw-r--   0 py        (1000) py        (1000)        0 2024-03-25 02:32:28.000000 scrutinydebugger-0.2.0/scrutiny/server/datalogging/definitions/__init__.py
--rw-rw-r--   0 py        (1000) py        (1000)     2771 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.0/scrutiny/server/datalogging/definitions/api.py
--rw-rw-r--   0 py        (1000) py        (1000)    11122 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.0/scrutiny/server/datalogging/definitions/device.py
-drwxrwxr-x   0 py        (1000) py        (1000)        0 2024-05-04 13:41:43.271700 scrutinydebugger-0.2.0/scrutiny/server/datastore/
--rw-rw-r--   0 py        (1000) py        (1000)        0 2024-03-25 02:32:28.000000 scrutinydebugger-0.2.0/scrutiny/server/datastore/__init__.py
--rw-rw-r--   0 py        (1000) py        (1000)    14837 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.0/scrutiny/server/datastore/datastore.py
--rw-rw-r--   0 py        (1000) py        (1000)    17593 2024-04-22 02:42:58.000000 scrutinydebugger-0.2.0/scrutiny/server/datastore/datastore_entry.py
--rw-rw-r--   0 py        (1000) py        (1000)      716 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.0/scrutiny/server/datastore/entry_type.py
-drwxrwxr-x   0 py        (1000) py        (1000)        0 2024-05-04 13:41:43.271700 scrutinydebugger-0.2.0/scrutiny/server/device/
--rw-rw-r--   0 py        (1000) py        (1000)        0 2024-03-25 02:32:28.000000 scrutinydebugger-0.2.0/scrutiny/server/device/__init__.py
--rw-rw-r--   0 py        (1000) py        (1000)    48107 2024-04-22 02:42:58.000000 scrutinydebugger-0.2.0/scrutiny/server/device/device_handler.py
--rw-rw-r--   0 py        (1000) py        (1000)     5021 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.0/scrutiny/server/device/device_info.py
--rw-rw-r--   0 py        (1000) py        (1000)    50160 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.0/scrutiny/server/device/emulated_device.py
-drwxrwxr-x   0 py        (1000) py        (1000)        0 2024-05-04 13:41:43.271700 scrutinydebugger-0.2.0/scrutiny/server/device/links/
--rw-rw-r--   0 py        (1000) py        (1000)       94 2024-03-25 02:32:28.000000 scrutinydebugger-0.2.0/scrutiny/server/device/links/__init__.py
--rw-rw-r--   0 py        (1000) py        (1000)     1946 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.0/scrutiny/server/device/links/abstract_link.py
--rw-rw-r--   0 py        (1000) py        (1000)     5921 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.0/scrutiny/server/device/links/dummy_link.py
--rw-rw-r--   0 py        (1000) py        (1000)     7384 2024-04-22 02:42:58.000000 scrutinydebugger-0.2.0/scrutiny/server/device/links/serial_link.py
--rw-rw-r--   0 py        (1000) py        (1000)     5386 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.0/scrutiny/server/device/links/udp_link.py
--rw-rw-r--   0 py        (1000) py        (1000)     9056 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.0/scrutiny/server/device/request_dispatcher.py
-drwxrwxr-x   0 py        (1000) py        (1000)        0 2024-05-04 13:41:43.271700 scrutinydebugger-0.2.0/scrutiny/server/device/submodules/
--rw-rw-r--   0 py        (1000) py        (1000)        0 2024-03-25 02:32:28.000000 scrutinydebugger-0.2.0/scrutiny/server/device/submodules/__init__.py
--rw-rw-r--   0 py        (1000) py        (1000)    37665 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.0/scrutiny/server/device/submodules/datalogging_poller.py
--rw-rw-r--   0 py        (1000) py        (1000)     6350 2024-04-22 02:42:58.000000 scrutinydebugger-0.2.0/scrutiny/server/device/submodules/device_searcher.py
--rw-rw-r--   0 py        (1000) py        (1000)     6341 2024-04-22 02:42:58.000000 scrutinydebugger-0.2.0/scrutiny/server/device/submodules/heartbeat_generator.py
--rw-rw-r--   0 py        (1000) py        (1000)    28019 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.0/scrutiny/server/device/submodules/info_poller.py
--rw-rw-r--   0 py        (1000) py        (1000)    30897 2024-04-22 02:42:58.000000 scrutinydebugger-0.2.0/scrutiny/server/device/submodules/memory_reader.py
--rw-rw-r--   0 py        (1000) py        (1000)    25434 2024-04-19 01:49:41.000000 scrutinydebugger-0.2.0/scrutiny/server/device/submodules/memory_writer.py
--rw-rw-r--   0 py        (1000) py        (1000)     6047 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.0/scrutiny/server/device/submodules/session_initializer.py
-drwxrwxr-x   0 py        (1000) py        (1000)        0 2024-05-04 13:41:43.275700 scrutinydebugger-0.2.0/scrutiny/server/protocol/
--rw-rw-r--   0 py        (1000) py        (1000)      191 2024-03-25 02:32:28.000000 scrutinydebugger-0.2.0/scrutiny/server/protocol/__init__.py
--rw-rw-r--   0 py        (1000) py        (1000)    15748 2024-04-22 02:42:58.000000 scrutinydebugger-0.2.0/scrutiny/server/protocol/comm_handler.py
-drwxrwxr-x   0 py        (1000) py        (1000)        0 2024-05-04 13:41:43.275700 scrutinydebugger-0.2.0/scrutiny/server/protocol/commands/
--rw-rw-r--   0 py        (1000) py        (1000)      360 2024-03-25 02:32:28.000000 scrutinydebugger-0.2.0/scrutiny/server/protocol/commands/__init__.py
--rw-rw-r--   0 py        (1000) py        (1000)     1639 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.0/scrutiny/server/protocol/commands/base_command.py
--rw-rw-r--   0 py        (1000) py        (1000)     1084 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.0/scrutiny/server/protocol/commands/comm_control.py
--rw-rw-r--   0 py        (1000) py        (1000)     1439 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.0/scrutiny/server/protocol/commands/datalog_control.py
--rw-rw-r--   0 py        (1000) py        (1000)      517 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.0/scrutiny/server/protocol/commands/dummy_command.py
--rw-rw-r--   0 py        (1000) py        (1000)     1738 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.0/scrutiny/server/protocol/commands/get_info.py
--rw-rw-r--   0 py        (1000) py        (1000)     1448 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.0/scrutiny/server/protocol/commands/memory_control.py
--rw-rw-r--   0 py        (1000) py        (1000)      481 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.0/scrutiny/server/protocol/commands/user_command.py
--rw-rw-r--   0 py        (1000) py        (1000)      622 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.0/scrutiny/server/protocol/crc32.py
--rw-rw-r--   0 py        (1000) py        (1000)      790 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.0/scrutiny/server/protocol/exceptions.py
--rw-rw-r--   0 py        (1000) py        (1000)    61707 2024-04-22 02:42:58.000000 scrutinydebugger-0.2.0/scrutiny/server/protocol/protocol.py
--rw-rw-r--   0 py        (1000) py        (1000)     4218 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.0/scrutiny/server/protocol/request.py
--rw-rw-r--   0 py        (1000) py        (1000)     4315 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.0/scrutiny/server/protocol/response.py
--rw-rw-r--   0 py        (1000) py        (1000)     6527 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.0/scrutiny/server/protocol/typing.py
--rw-rw-r--   0 py        (1000) py        (1000)     5269 2024-04-22 02:42:58.000000 scrutinydebugger-0.2.0/scrutiny/server/server.py
-drwxrwxr-x   0 py        (1000) py        (1000)        0 2024-05-04 13:41:43.275700 scrutinydebugger-0.2.0/scrutiny/tools/
--rw-rw-r--   0 py        (1000) py        (1000)      101 2024-03-25 02:32:28.000000 scrutinydebugger-0.2.0/scrutiny/tools/__init__.py
--rw-rw-r--   0 py        (1000) py        (1000)     4733 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.0/scrutiny/tools/synchronous_websocket_server.py
--rw-rw-r--   0 py        (1000) py        (1000)     5442 2024-04-22 02:42:58.000000 scrutinydebugger-0.2.0/scrutiny/tools/throttler.py
--rw-rw-r--   0 py        (1000) py        (1000)     1287 2024-04-22 02:42:58.000000 scrutinydebugger-0.2.0/scrutiny/tools/timer.py
-drwxrwxr-x   0 py        (1000) py        (1000)        0 2024-05-04 13:41:43.275700 scrutinydebugger-0.2.0/scrutinydebugger.egg-info/
--rw-r--r--   0 py        (1000) py        (1000)      887 2024-05-04 13:41:43.000000 scrutinydebugger-0.2.0/scrutinydebugger.egg-info/PKG-INFO
--rw-rw-r--   0 py        (1000) py        (1000)     4595 2024-05-04 13:41:43.000000 scrutinydebugger-0.2.0/scrutinydebugger.egg-info/SOURCES.txt
--rw-rw-r--   0 py        (1000) py        (1000)        1 2024-05-04 13:41:43.000000 scrutinydebugger-0.2.0/scrutinydebugger.egg-info/dependency_links.txt
--rw-rw-r--   0 py        (1000) py        (1000)       52 2024-05-04 13:41:43.000000 scrutinydebugger-0.2.0/scrutinydebugger.egg-info/entry_points.txt
--rw-rw-r--   0 py        (1000) py        (1000)      222 2024-05-04 13:41:43.000000 scrutinydebugger-0.2.0/scrutinydebugger.egg-info/requires.txt
--rw-rw-r--   0 py        (1000) py        (1000)        9 2024-05-04 13:41:43.000000 scrutinydebugger-0.2.0/scrutinydebugger.egg-info/top_level.txt
--rw-rw-r--   0 py        (1000) py        (1000)       38 2024-05-04 13:41:43.279700 scrutinydebugger-0.2.0/setup.cfg
--rw-rw-r--   0 py        (1000) py        (1000)     1403 2024-03-27 04:12:19.000000 scrutinydebugger-0.2.0/setup.py
+drwxrwxr-x   0 py        (1000) py        (1000)        0 2024-05-12 14:48:17.801810 scrutinydebugger-0.2.1/
+-rw-rw-r--   0 py        (1000) py        (1000)     1073 2024-03-25 03:09:50.000000 scrutinydebugger-0.2.1/LICENSE
+-rw-r--r--   0 py        (1000) py        (1000)      887 2024-05-12 14:48:17.801810 scrutinydebugger-0.2.1/PKG-INFO
+-rw-rw-r--   0 py        (1000) py        (1000)      596 2024-04-11 01:05:46.000000 scrutinydebugger-0.2.1/README.md
+drwxrwxr-x   0 py        (1000) py        (1000)        0 2024-05-12 14:48:17.785810 scrutinydebugger-0.2.1/scrutiny/
+-rw-rw-r--   0 py        (1000) py        (1000)      188 2024-05-12 14:42:30.000000 scrutinydebugger-0.2.1/scrutiny/__init__.py
+-rw-rw-r--   0 py        (1000) py        (1000)      453 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.1/scrutiny/__main__.py
+drwxrwxr-x   0 py        (1000) py        (1000)        0 2024-05-12 14:48:17.789810 scrutinydebugger-0.2.1/scrutiny/cli/
+-rw-rw-r--   0 py        (1000) py        (1000)       39 2024-03-25 02:32:28.000000 scrutinydebugger-0.2.1/scrutiny/cli/__init__.py
+-rw-rw-r--   0 py        (1000) py        (1000)     5089 2024-04-15 01:53:14.000000 scrutinydebugger-0.2.1/scrutiny/cli/cli.py
+drwxrwxr-x   0 py        (1000) py        (1000)        0 2024-05-12 14:48:17.789810 scrutinydebugger-0.2.1/scrutiny/cli/commands/
+-rw-rw-r--   0 py        (1000) py        (1000)     1577 2024-03-25 02:32:28.000000 scrutinydebugger-0.2.1/scrutiny/cli/commands/__init__.py
+-rw-rw-r--   0 py        (1000) py        (1000)     5166 2024-04-15 02:52:23.000000 scrutinydebugger-0.2.1/scrutiny/cli/commands/add_alias.py
+-rw-rw-r--   0 py        (1000) py        (1000)     1431 2024-04-15 01:53:14.000000 scrutinydebugger-0.2.1/scrutiny/cli/commands/base_command.py
+-rw-rw-r--   0 py        (1000) py        (1000)     2774 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.1/scrutiny/cli/commands/datalog_info.py
+-rw-rw-r--   0 py        (1000) py        (1000)     1481 2024-04-15 01:53:14.000000 scrutinydebugger-0.2.1/scrutiny/cli/commands/delete_datalog.py
+-rw-rw-r--   0 py        (1000) py        (1000)     2148 2024-04-15 01:53:14.000000 scrutinydebugger-0.2.1/scrutiny/cli/commands/elf2varmap.py
+-rw-rw-r--   0 py        (1000) py        (1000)     1699 2024-04-15 01:53:14.000000 scrutinydebugger-0.2.1/scrutiny/cli/commands/export_datalog.py
+-rw-rw-r--   0 py        (1000) py        (1000)     2082 2024-04-15 01:53:14.000000 scrutinydebugger-0.2.1/scrutiny/cli/commands/get_firmware_id.py
+-rw-rw-r--   0 py        (1000) py        (1000)     1314 2024-04-15 01:53:14.000000 scrutinydebugger-0.2.1/scrutiny/cli/commands/install_sfd.py
+-rw-rw-r--   0 py        (1000) py        (1000)     2024 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.1/scrutiny/cli/commands/launch_server.py
+-rw-rw-r--   0 py        (1000) py        (1000)     5569 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.1/scrutiny/cli/commands/list_datalog.py
+-rw-rw-r--   0 py        (1000) py        (1000)     3746 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.1/scrutiny/cli/commands/list_sfd.py
+-rw-rw-r--   0 py        (1000) py        (1000)     2880 2024-04-15 01:53:14.000000 scrutinydebugger-0.2.1/scrutiny/cli/commands/make_metadata.py
+-rw-rw-r--   0 py        (1000) py        (1000)     1641 2024-04-15 01:53:14.000000 scrutinydebugger-0.2.1/scrutiny/cli/commands/make_sfd.py
+-rw-rw-r--   0 py        (1000) py        (1000)     3618 2024-04-15 01:53:14.000000 scrutinydebugger-0.2.1/scrutiny/cli/commands/runtest.py
+-rw-rw-r--   0 py        (1000) py        (1000)     1970 2024-04-15 01:53:14.000000 scrutinydebugger-0.2.1/scrutiny/cli/commands/tag_firmware_id.py
+-rw-rw-r--   0 py        (1000) py        (1000)     1498 2024-04-22 02:42:58.000000 scrutinydebugger-0.2.1/scrutiny/cli/commands/uninstall_sfd.py
+drwxrwxr-x   0 py        (1000) py        (1000)        0 2024-05-12 14:48:17.789810 scrutinydebugger-0.2.1/scrutiny/core/
+-rw-rw-r--   0 py        (1000) py        (1000)        0 2024-03-25 02:32:28.000000 scrutinydebugger-0.2.1/scrutiny/core/__init__.py
+-rw-rw-r--   0 py        (1000) py        (1000)     7134 2024-04-22 02:42:58.000000 scrutinydebugger-0.2.1/scrutiny/core/alias.py
+-rw-rw-r--   0 py        (1000) py        (1000)     6707 2024-05-08 23:43:40.000000 scrutinydebugger-0.2.1/scrutiny/core/basic_types.py
+drwxrwxr-x   0 py        (1000) py        (1000)        0 2024-05-12 14:48:17.793810 scrutinydebugger-0.2.1/scrutiny/core/bintools/
+-rw-rw-r--   0 py        (1000) py        (1000)        0 2024-03-25 02:32:28.000000 scrutinydebugger-0.2.1/scrutiny/core/bintools/__init__.py
+-rw-rw-r--   0 py        (1000) py        (1000)     1924 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.1/scrutiny/core/bintools/demangler.py
+-rw-rw-r--   0 py        (1000) py        (1000)    37593 2024-05-08 23:43:40.000000 scrutinydebugger-0.2.1/scrutiny/core/bintools/elf_dwarf_var_extractor.py
+-rw-rw-r--   0 py        (1000) py        (1000)      223 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.1/scrutiny/core/bintools/elftools_stubs.py
+-rw-rw-r--   0 py        (1000) py        (1000)      547 2024-04-15 01:53:14.000000 scrutinydebugger-0.2.1/scrutiny/core/bintools/elftools_stubs.pyi
+-rw-rw-r--   0 py        (1000) py        (1000)      755 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.1/scrutiny/core/bintools/get_var_memrange.py
+-rw-rw-r--   0 py        (1000) py        (1000)     5385 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.1/scrutiny/core/codecs.py
+-rw-rw-r--   0 py        (1000) py        (1000)     7670 2024-04-21 14:05:12.000000 scrutinydebugger-0.2.1/scrutiny/core/datalogging.py
+-rw-rw-r--   0 py        (1000) py        (1000)    10600 2024-04-21 03:45:36.000000 scrutinydebugger-0.2.1/scrutiny/core/firmware_description.py
+-rw-rw-r--   0 py        (1000) py        (1000)      402 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.1/scrutiny/core/firmware_id.py
+-rw-rw-r--   0 py        (1000) py        (1000)     3653 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.1/scrutiny/core/firmware_parser.py
+-rw-rw-r--   0 py        (1000) py        (1000)    14117 2024-04-22 02:42:58.000000 scrutinydebugger-0.2.1/scrutiny/core/memory_content.py
+-rw-rw-r--   0 py        (1000) py        (1000)     6939 2024-04-15 02:52:23.000000 scrutinydebugger-0.2.1/scrutiny/core/sfd_storage.py
+-rw-rw-r--   0 py        (1000) py        (1000)      787 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.1/scrutiny/core/typehints.py
+-rw-rw-r--   0 py        (1000) py        (1000)     3000 2024-04-11 01:05:46.000000 scrutinydebugger-0.2.1/scrutiny/core/validation.py
+-rw-rw-r--   0 py        (1000) py        (1000)    14999 2024-05-08 23:43:40.000000 scrutinydebugger-0.2.1/scrutiny/core/variable.py
+-rw-rw-r--   0 py        (1000) py        (1000)    10690 2024-04-15 01:53:14.000000 scrutinydebugger-0.2.1/scrutiny/core/varmap.py
+-rw-rw-r--   0 py        (1000) py        (1000)      290 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.1/scrutiny/exceptions.py
+-rw-rw-r--   0 py        (1000) py        (1000)        0 2024-03-27 04:12:19.000000 scrutinydebugger-0.2.1/scrutiny/py.typed
+drwxrwxr-x   0 py        (1000) py        (1000)        0 2024-05-12 14:48:17.793810 scrutinydebugger-0.2.1/scrutiny/sdk/
+-rw-rw-r--   0 py        (1000) py        (1000)      350 2024-03-25 02:32:28.000000 scrutinydebugger-0.2.1/scrutiny/sdk/__init__.py
+-rw-rw-r--   0 py        (1000) py        (1000)    35478 2024-04-22 02:42:58.000000 scrutinydebugger-0.2.1/scrutiny/sdk/_api_parser.py
+-rw-rw-r--   0 py        (1000) py        (1000)    73474 2024-04-11 01:05:46.000000 scrutinydebugger-0.2.1/scrutiny/sdk/client.py
+-rw-rw-r--   0 py        (1000) py        (1000)    23098 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.1/scrutiny/sdk/datalogging.py
+-rw-rw-r--   0 py        (1000) py        (1000)    13027 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.1/scrutiny/sdk/definitions.py
+-rw-rw-r--   0 py        (1000) py        (1000)     1539 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.1/scrutiny/sdk/exceptions.py
+drwxrwxr-x   0 py        (1000) py        (1000)        0 2024-05-12 14:48:17.793810 scrutinydebugger-0.2.1/scrutiny/sdk/listeners/
+-rw-rw-r--   0 py        (1000) py        (1000)    11930 2024-04-11 01:05:46.000000 scrutinydebugger-0.2.1/scrutiny/sdk/listeners/__init__.py
+-rw-rw-r--   0 py        (1000) py        (1000)     1365 2024-04-11 01:05:46.000000 scrutinydebugger-0.2.1/scrutiny/sdk/listeners/buffered_reader_listener.py
+-rw-rw-r--   0 py        (1000) py        (1000)    10506 2024-04-11 01:05:46.000000 scrutinydebugger-0.2.1/scrutiny/sdk/listeners/csv_file_listener.py
+-rw-rw-r--   0 py        (1000) py        (1000)     2127 2024-04-11 01:05:46.000000 scrutinydebugger-0.2.1/scrutiny/sdk/listeners/text_stream_listener.py
+-rw-rw-r--   0 py        (1000) py        (1000)     9981 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.1/scrutiny/sdk/watchable_handle.py
+-rw-rw-r--   0 py        (1000) py        (1000)     3707 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.1/scrutiny/sdk/write_request.py
+drwxrwxr-x   0 py        (1000) py        (1000)        0 2024-05-12 14:48:17.793810 scrutinydebugger-0.2.1/scrutiny/server/
+-rw-rw-r--   0 py        (1000) py        (1000)        0 2024-03-25 02:32:28.000000 scrutinydebugger-0.2.1/scrutiny/server/__init__.py
+-rw-rw-r--   0 py        (1000) py        (1000)     8039 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.1/scrutiny/server/active_sfd_handler.py
+drwxrwxr-x   0 py        (1000) py        (1000)        0 2024-05-12 14:48:17.793810 scrutinydebugger-0.2.1/scrutiny/server/api/
+-rw-rw-r--   0 py        (1000) py        (1000)    79420 2024-04-22 02:42:58.000000 scrutinydebugger-0.2.1/scrutiny/server/api/API.py
+-rw-rw-r--   0 py        (1000) py        (1000)       64 2024-03-25 02:32:28.000000 scrutinydebugger-0.2.1/scrutiny/server/api/__init__.py
+-rw-rw-r--   0 py        (1000) py        (1000)     1203 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.1/scrutiny/server/api/abstract_client_handler.py
+-rw-rw-r--   0 py        (1000) py        (1000)     5976 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.1/scrutiny/server/api/dummy_client_handler.py
+-rw-rw-r--   0 py        (1000) py        (1000)    11185 2024-04-22 02:42:58.000000 scrutinydebugger-0.2.1/scrutiny/server/api/typing.py
+-rw-rw-r--   0 py        (1000) py        (1000)     2868 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.1/scrutiny/server/api/value_streamer.py
+-rw-rw-r--   0 py        (1000) py        (1000)     4652 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.1/scrutiny/server/api/websocket_client_handler.py
+drwxrwxr-x   0 py        (1000) py        (1000)        0 2024-05-12 14:48:17.793810 scrutinydebugger-0.2.1/scrutiny/server/datalogging/
+-rw-rw-r--   0 py        (1000) py        (1000)        0 2024-03-25 02:32:28.000000 scrutinydebugger-0.2.1/scrutiny/server/datalogging/__init__.py
+-rw-rw-r--   0 py        (1000) py        (1000)    29373 2024-04-22 02:42:58.000000 scrutinydebugger-0.2.1/scrutiny/server/datalogging/datalogging_manager.py
+-rw-rw-r--   0 py        (1000) py        (1000)    22438 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.1/scrutiny/server/datalogging/datalogging_storage.py
+-rw-rw-r--   0 py        (1000) py        (1000)     2294 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.1/scrutiny/server/datalogging/datalogging_utilities.py
+drwxrwxr-x   0 py        (1000) py        (1000)        0 2024-05-12 14:48:17.797810 scrutinydebugger-0.2.1/scrutiny/server/datalogging/definitions/
+-rw-rw-r--   0 py        (1000) py        (1000)        0 2024-03-25 02:32:28.000000 scrutinydebugger-0.2.1/scrutiny/server/datalogging/definitions/__init__.py
+-rw-rw-r--   0 py        (1000) py        (1000)     2771 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.1/scrutiny/server/datalogging/definitions/api.py
+-rw-rw-r--   0 py        (1000) py        (1000)    11122 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.1/scrutiny/server/datalogging/definitions/device.py
+drwxrwxr-x   0 py        (1000) py        (1000)        0 2024-05-12 14:48:17.797810 scrutinydebugger-0.2.1/scrutiny/server/datastore/
+-rw-rw-r--   0 py        (1000) py        (1000)        0 2024-03-25 02:32:28.000000 scrutinydebugger-0.2.1/scrutiny/server/datastore/__init__.py
+-rw-rw-r--   0 py        (1000) py        (1000)    14837 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.1/scrutiny/server/datastore/datastore.py
+-rw-rw-r--   0 py        (1000) py        (1000)    17593 2024-04-22 02:42:58.000000 scrutinydebugger-0.2.1/scrutiny/server/datastore/datastore_entry.py
+-rw-rw-r--   0 py        (1000) py        (1000)      716 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.1/scrutiny/server/datastore/entry_type.py
+drwxrwxr-x   0 py        (1000) py        (1000)        0 2024-05-12 14:48:17.797810 scrutinydebugger-0.2.1/scrutiny/server/device/
+-rw-rw-r--   0 py        (1000) py        (1000)        0 2024-03-25 02:32:28.000000 scrutinydebugger-0.2.1/scrutiny/server/device/__init__.py
+-rw-rw-r--   0 py        (1000) py        (1000)    48107 2024-04-22 02:42:58.000000 scrutinydebugger-0.2.1/scrutiny/server/device/device_handler.py
+-rw-rw-r--   0 py        (1000) py        (1000)     5021 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.1/scrutiny/server/device/device_info.py
+-rw-rw-r--   0 py        (1000) py        (1000)    50160 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.1/scrutiny/server/device/emulated_device.py
+drwxrwxr-x   0 py        (1000) py        (1000)        0 2024-05-12 14:48:17.797810 scrutinydebugger-0.2.1/scrutiny/server/device/links/
+-rw-rw-r--   0 py        (1000) py        (1000)       94 2024-03-25 02:32:28.000000 scrutinydebugger-0.2.1/scrutiny/server/device/links/__init__.py
+-rw-rw-r--   0 py        (1000) py        (1000)     1946 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.1/scrutiny/server/device/links/abstract_link.py
+-rw-rw-r--   0 py        (1000) py        (1000)     5921 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.1/scrutiny/server/device/links/dummy_link.py
+-rw-rw-r--   0 py        (1000) py        (1000)     7384 2024-04-22 02:42:58.000000 scrutinydebugger-0.2.1/scrutiny/server/device/links/serial_link.py
+-rw-rw-r--   0 py        (1000) py        (1000)     5386 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.1/scrutiny/server/device/links/udp_link.py
+-rw-rw-r--   0 py        (1000) py        (1000)     9056 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.1/scrutiny/server/device/request_dispatcher.py
+drwxrwxr-x   0 py        (1000) py        (1000)        0 2024-05-12 14:48:17.797810 scrutinydebugger-0.2.1/scrutiny/server/device/submodules/
+-rw-rw-r--   0 py        (1000) py        (1000)        0 2024-03-25 02:32:28.000000 scrutinydebugger-0.2.1/scrutiny/server/device/submodules/__init__.py
+-rw-rw-r--   0 py        (1000) py        (1000)    37665 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.1/scrutiny/server/device/submodules/datalogging_poller.py
+-rw-rw-r--   0 py        (1000) py        (1000)     6350 2024-04-22 02:42:58.000000 scrutinydebugger-0.2.1/scrutiny/server/device/submodules/device_searcher.py
+-rw-rw-r--   0 py        (1000) py        (1000)     6341 2024-04-22 02:42:58.000000 scrutinydebugger-0.2.1/scrutiny/server/device/submodules/heartbeat_generator.py
+-rw-rw-r--   0 py        (1000) py        (1000)    28019 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.1/scrutiny/server/device/submodules/info_poller.py
+-rw-rw-r--   0 py        (1000) py        (1000)    30897 2024-04-22 02:42:58.000000 scrutinydebugger-0.2.1/scrutiny/server/device/submodules/memory_reader.py
+-rw-rw-r--   0 py        (1000) py        (1000)    25434 2024-04-19 01:49:41.000000 scrutinydebugger-0.2.1/scrutiny/server/device/submodules/memory_writer.py
+-rw-rw-r--   0 py        (1000) py        (1000)     6047 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.1/scrutiny/server/device/submodules/session_initializer.py
+drwxrwxr-x   0 py        (1000) py        (1000)        0 2024-05-12 14:48:17.801810 scrutinydebugger-0.2.1/scrutiny/server/protocol/
+-rw-rw-r--   0 py        (1000) py        (1000)      191 2024-03-25 02:32:28.000000 scrutinydebugger-0.2.1/scrutiny/server/protocol/__init__.py
+-rw-rw-r--   0 py        (1000) py        (1000)    16181 2024-05-05 03:12:23.000000 scrutinydebugger-0.2.1/scrutiny/server/protocol/comm_handler.py
+drwxrwxr-x   0 py        (1000) py        (1000)        0 2024-05-12 14:48:17.801810 scrutinydebugger-0.2.1/scrutiny/server/protocol/commands/
+-rw-rw-r--   0 py        (1000) py        (1000)      360 2024-03-25 02:32:28.000000 scrutinydebugger-0.2.1/scrutiny/server/protocol/commands/__init__.py
+-rw-rw-r--   0 py        (1000) py        (1000)     1639 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.1/scrutiny/server/protocol/commands/base_command.py
+-rw-rw-r--   0 py        (1000) py        (1000)     1084 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.1/scrutiny/server/protocol/commands/comm_control.py
+-rw-rw-r--   0 py        (1000) py        (1000)     1439 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.1/scrutiny/server/protocol/commands/datalog_control.py
+-rw-rw-r--   0 py        (1000) py        (1000)      517 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.1/scrutiny/server/protocol/commands/dummy_command.py
+-rw-rw-r--   0 py        (1000) py        (1000)     1738 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.1/scrutiny/server/protocol/commands/get_info.py
+-rw-rw-r--   0 py        (1000) py        (1000)     1448 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.1/scrutiny/server/protocol/commands/memory_control.py
+-rw-rw-r--   0 py        (1000) py        (1000)      481 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.1/scrutiny/server/protocol/commands/user_command.py
+-rw-rw-r--   0 py        (1000) py        (1000)      622 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.1/scrutiny/server/protocol/crc32.py
+-rw-rw-r--   0 py        (1000) py        (1000)      790 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.1/scrutiny/server/protocol/exceptions.py
+-rw-rw-r--   0 py        (1000) py        (1000)    61707 2024-04-22 02:42:58.000000 scrutinydebugger-0.2.1/scrutiny/server/protocol/protocol.py
+-rw-rw-r--   0 py        (1000) py        (1000)     4218 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.1/scrutiny/server/protocol/request.py
+-rw-rw-r--   0 py        (1000) py        (1000)     4315 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.1/scrutiny/server/protocol/response.py
+-rw-rw-r--   0 py        (1000) py        (1000)     6527 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.1/scrutiny/server/protocol/typing.py
+-rw-rw-r--   0 py        (1000) py        (1000)     5269 2024-04-22 02:42:58.000000 scrutinydebugger-0.2.1/scrutiny/server/server.py
+drwxrwxr-x   0 py        (1000) py        (1000)        0 2024-05-12 14:48:17.801810 scrutinydebugger-0.2.1/scrutiny/tools/
+-rw-rw-r--   0 py        (1000) py        (1000)      101 2024-05-12 14:19:24.000000 scrutinydebugger-0.2.1/scrutiny/tools/__init__.py
+-rw-rw-r--   0 py        (1000) py        (1000)     2573 2024-05-08 20:47:25.000000 scrutinydebugger-0.2.1/scrutiny/tools/selectable_queue.py
+-rw-rw-r--   0 py        (1000) py        (1000)     4733 2024-04-08 03:00:50.000000 scrutinydebugger-0.2.1/scrutiny/tools/synchronous_websocket_server.py
+-rw-rw-r--   0 py        (1000) py        (1000)     5442 2024-04-22 02:42:58.000000 scrutinydebugger-0.2.1/scrutiny/tools/throttler.py
+-rw-rw-r--   0 py        (1000) py        (1000)     1287 2024-04-22 02:42:58.000000 scrutinydebugger-0.2.1/scrutiny/tools/timer.py
+drwxrwxr-x   0 py        (1000) py        (1000)        0 2024-05-12 14:48:17.801810 scrutinydebugger-0.2.1/scrutinydebugger.egg-info/
+-rw-r--r--   0 py        (1000) py        (1000)      887 2024-05-12 14:48:17.000000 scrutinydebugger-0.2.1/scrutinydebugger.egg-info/PKG-INFO
+-rw-rw-r--   0 py        (1000) py        (1000)     4630 2024-05-12 14:48:17.000000 scrutinydebugger-0.2.1/scrutinydebugger.egg-info/SOURCES.txt
+-rw-rw-r--   0 py        (1000) py        (1000)        1 2024-05-12 14:48:17.000000 scrutinydebugger-0.2.1/scrutinydebugger.egg-info/dependency_links.txt
+-rw-rw-r--   0 py        (1000) py        (1000)       52 2024-05-12 14:48:17.000000 scrutinydebugger-0.2.1/scrutinydebugger.egg-info/entry_points.txt
+-rw-rw-r--   0 py        (1000) py        (1000)      222 2024-05-12 14:48:17.000000 scrutinydebugger-0.2.1/scrutinydebugger.egg-info/requires.txt
+-rw-rw-r--   0 py        (1000) py        (1000)        9 2024-05-12 14:48:17.000000 scrutinydebugger-0.2.1/scrutinydebugger.egg-info/top_level.txt
+-rw-rw-r--   0 py        (1000) py        (1000)       38 2024-05-12 14:48:17.801810 scrutinydebugger-0.2.1/setup.cfg
+-rw-rw-r--   0 py        (1000) py        (1000)     1403 2024-05-12 14:19:24.000000 scrutinydebugger-0.2.1/setup.py
```

### Comparing `scrutinydebugger-0.2.0/LICENSE` & `scrutinydebugger-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.0/PKG-INFO` & `scrutinydebugger-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrutinydebugger
-Version: 0.2.0
+Version: 0.2.1
 Summary: Scrutiny debugger Python framework
 Home-page: https://github.com/scrutinydebugger/scrutiny-python
 Author: Pier-Yves Lessard
 License: MIT
 Requires-Python: >3.8
 License-File: LICENSE
 Requires-Dist: appdirs>=1.4.4
```

### Comparing `scrutinydebugger-0.2.0/README.md` & `scrutinydebugger-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.0/scrutiny/cli/cli.py` & `scrutinydebugger-0.2.1/scrutiny/cli/cli.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.0/scrutiny/cli/commands/__init__.py` & `scrutinydebugger-0.2.1/scrutiny/cli/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.0/scrutiny/cli/commands/add_alias.py` & `scrutinydebugger-0.2.1/scrutiny/cli/commands/add_alias.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.0/scrutiny/cli/commands/base_command.py` & `scrutinydebugger-0.2.1/scrutiny/cli/commands/base_command.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.0/scrutiny/cli/commands/datalog_info.py` & `scrutinydebugger-0.2.1/scrutiny/cli/commands/datalog_info.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.0/scrutiny/cli/commands/delete_datalog.py` & `scrutinydebugger-0.2.1/scrutiny/cli/commands/delete_datalog.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.0/scrutiny/cli/commands/elf2varmap.py` & `scrutinydebugger-0.2.1/scrutiny/cli/commands/elf2varmap.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.0/scrutiny/cli/commands/export_datalog.py` & `scrutinydebugger-0.2.1/scrutiny/cli/commands/export_datalog.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.0/scrutiny/cli/commands/get_firmware_id.py` & `scrutinydebugger-0.2.1/scrutiny/cli/commands/get_firmware_id.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.0/scrutiny/cli/commands/install_sfd.py` & `scrutinydebugger-0.2.1/scrutiny/cli/commands/install_sfd.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.0/scrutiny/cli/commands/launch_server.py` & `scrutinydebugger-0.2.1/scrutiny/cli/commands/launch_server.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.0/scrutiny/cli/commands/list_datalog.py` & `scrutinydebugger-0.2.1/scrutiny/cli/commands/list_datalog.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.0/scrutiny/cli/commands/list_sfd.py` & `scrutinydebugger-0.2.1/scrutiny/cli/commands/list_sfd.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.0/scrutiny/cli/commands/make_metadata.py` & `scrutinydebugger-0.2.1/scrutiny/cli/commands/make_metadata.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.0/scrutiny/cli/commands/make_sfd.py` & `scrutinydebugger-0.2.1/scrutiny/cli/commands/make_sfd.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.0/scrutiny/cli/commands/runtest.py` & `scrutinydebugger-0.2.1/scrutiny/cli/commands/runtest.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.0/scrutiny/cli/commands/tag_firmware_id.py` & `scrutinydebugger-0.2.1/scrutiny/cli/commands/tag_firmware_id.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.0/scrutiny/cli/commands/uninstall_sfd.py` & `scrutinydebugger-0.2.1/scrutiny/cli/commands/uninstall_sfd.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.0/scrutiny/core/alias.py` & `scrutinydebugger-0.2.1/scrutiny/core/alias.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.0/scrutiny/core/basic_types.py` & `scrutinydebugger-0.2.1/scrutiny/core/basic_types.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     'RuntimePublishedValue',
     'MemoryRegion'
 ]
 
 from enum import Enum
 from dataclasses import dataclass
 from scrutiny.core import validation
-
+from typing import Union
 
 @dataclass(frozen=True)
 class MemoryRegion:
     """(Immutable struct) 
     Represent a memory region spanning from ``start`` to ``start+size-1``"""
 
     start: int
@@ -150,14 +150,31 @@
 
     def is_signed(self) -> bool:
         """Tells if the datatype support a sign (sint, float, cfloat)"""
         type_type = self.value & 0xF0
         if type_type in (DataTypeType._sint.value, DataTypeType._float.value, DataTypeType._cfloat.value):
             return True
         return False
+    
+    @classmethod
+    def make(cls, datatype_type:DataTypeType, size:Union[int, DataTypeSize]) -> "EmbeddedDataType":
+        if isinstance(size, int):
+            if size == 1:
+                return cls.make(datatype_type, DataTypeSize._8)
+            if size == 2:
+                return cls.make(datatype_type, DataTypeSize._16)
+            if size == 4:
+                return cls.make(datatype_type, DataTypeSize._32)
+            if size == 8:
+                return cls.make(datatype_type, DataTypeSize._64)
+            if size == 16:
+                return cls.make(datatype_type, DataTypeSize._128)
+            raise ValueError(f"Impossible size given {size}")
+        else:
+            return cls(datatype_type.value | size.value)
 
 
 @dataclass(frozen=True)
 class RuntimePublishedValue:
     """ 
     (Immutable struct) A Runtime Published Value (RPV) is on of the basic element that can be read from a target device.
     RPVs are defined in the embedded code and known by the server by polling the device.
```

### Comparing `scrutinydebugger-0.2.0/scrutiny/core/bintools/demangler.py` & `scrutinydebugger-0.2.1/scrutiny/core/bintools/demangler.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.0/scrutiny/core/bintools/elf_dwarf_var_extractor.py` & `scrutinydebugger-0.2.1/scrutiny/core/bintools/elf_dwarf_var_extractor.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,15 @@
 class TypeOfVar(Enum):
     BaseType=auto()
     Struct=auto()
     Class=auto()
     Union=auto()
     Pointer=auto()
     Array=auto()
+    EnumOnly=auto() # Clang dwarf v2
 
 @dataclass
 class TypeDescriptor:
     type: TypeOfVar
     enum_die:Optional[ "elftools_stubs.Die"]
     type_die: "elftools_stubs.Die"
 
@@ -112,14 +113,15 @@
         'DW_TAG_union_type': '<union>'
     }
 
     STATIC = 'static'
     GLOBAL = 'global'
     MAX_CU_DISPLAY_NAME_LENGTH = 40
     DW_OP_ADDR = 3
+    DW_OP_plus_uconst = 0x23
 
     class DwarfEncoding(Enum):
         DW_ATE_address = 0x1
         DW_ATE_boolean = 0x2
         DW_ATE_complex_float = 0x3
         DW_ATE_float = 0x4
         DW_ATE_signed = 0x5
@@ -160,15 +162,17 @@
         
         self.logger.handlers
         self.initial_stack_depth= len(inspect.stack())
 
         if filename is not None:
             self.load_from_elf_file(filename)
 
-    def make_name_for_log(self, die: "elftools_stubs.Die") -> str:
+    def make_name_for_log(self, die: Optional["elftools_stubs.Die"]) -> str:
+        if die is None:
+            return "<None>"
         name=''
         try:
             name = self.get_name(die, nolog=True)
         except:
             pass
         return f'{die.tag} <{die.offset:x}> "{name}"'
 
@@ -260,35 +264,53 @@
     def get_cu_name(self, die: "elftools_stubs.Die") -> str:
         return self.cu_name_map[die.cu]
 
     def get_die_at_spec(self, die: "elftools_stubs.Die") -> "elftools_stubs.Die":
         self.log_debug_process_die(die)
         refaddr = cast(int, die.attributes['DW_AT_specification'].value) + die.cu.cu_offset
         return die.dwarfinfo.get_DIE_from_refaddr(refaddr)
+    
+    def get_die_at_abstract_origin(self, die: "elftools_stubs.Die") -> "elftools_stubs.Die":
+        self.log_debug_process_die(die)
+        refaddr = cast(int, die.attributes['DW_AT_abstract_origin'].value) + die.cu.cu_offset
+        return die.dwarfinfo.get_DIE_from_refaddr(refaddr)
 
     def get_name(self, die: "elftools_stubs.Die", default: Optional[str] = None, nolog:bool=False) -> str:
         if not nolog:
             self.log_debug_process_die(die)
         if 'DW_AT_name' in die.attributes:
             return cast(str, die.attributes['DW_AT_name'].value.decode('ascii'))
         else:
             if default is not None:
                 return default
             elif die.tag in self.defaults_names:
                 return self.defaults_names[die.tag]
             else:
                 raise ElfParsingError('Cannot get a name for this die. %s' % die)
 
+    def has_linkage_name(self, die: "elftools_stubs.Die") -> bool:
+        if 'DW_AT_linkage_name' in die.attributes:
+            return True
+        if 'DW_AT_MIPS_linkage_name' in die.attributes:
+            return True
+        return False
+    
     def get_linkage_name(self, die: "elftools_stubs.Die") -> str:
         self.log_debug_process_die(die)
-        return self.demangler.demangle(die.attributes['DW_AT_linkage_name'].value.decode('ascii'))
-
-    # Tells if the die is accessible from outside the compile unit. If it is, it's global, otherwise it's static.
+        if 'DW_AT_linkage_name' in die.attributes:
+            mangled_encoded = die.attributes['DW_AT_linkage_name'].value
+        elif 'DW_AT_MIPS_linkage_name' in die.attributes:
+            mangled_encoded = die.attributes['DW_AT_MIPS_linkage_name'].value
+        else:
+            raise ElfParsingError("No linkage name available")
+        
+        return self.demangler.demangle(mangled_encoded.decode('ascii'))
 
     def is_external(self, die: "elftools_stubs.Die") -> bool:
+        """Tells if the die is accessible from outside the compile unit. If it is, it's global, otherwise it's static."""
         try:
             return cast(bool, die.attributes['DW_AT_external'].value)
         except Exception:
             return False
 
     def get_core_base_type(self, encoding: DwarfEncoding, bytesize: int) -> EmbeddedDataType:
 
@@ -378,15 +400,20 @@
             self.demangler = GccDemangler(*args)  # todo : adapt according to compile unit producer
 
             if not self.demangler.can_run():
                 raise EnvionmentNotSetUpException("Demangler cannot be used. %s" % self.demangler.get_error())
 
             self.initial_stack_depth = len(inspect.stack())
             
+            bad_support_warning_written = False
             for cu in self.dwarfinfo.iter_CUs():
+                if cu.header['version'] not in (2,3,4):
+                    if not bad_support_warning_written:
+                        bad_support_warning_written = True
+                        self.logger.warning(f"DWARF format version {cu.header['version']} is not well supported, output may be incomplete")
                 die = cu.get_top_DIE()
                 self.extract_var_recursive(die) # Recursion start point
 
     def extract_var_recursive(self, die: "elftools_stubs.Die") -> None:
         # Finds all "variable" tags and create an entry in the varmap.
         # Types / structures / enums are discovered as we go. We only take
         # definitions that are used by a variables, the rest will be ignored.
@@ -478,84 +505,149 @@
             elif nextdie.tag == 'DW_TAG_base_type':
                 return TypeDescriptor(TypeOfVar.BaseType, enum, nextdie)
             elif nextdie.tag == 'DW_TAG_pointer_type':
                 return TypeDescriptor(TypeOfVar.Pointer, enum, nextdie)
             elif nextdie.tag == 'DW_TAG_union_type':
                 return TypeDescriptor(TypeOfVar.Union, enum, nextdie)
             elif nextdie.tag == 'DW_TAG_enumeration_type':
-                enum = nextdie  # Should resolve to a basetype on next iteration.
+                enum = nextdie  # Will resolve on next iteration (if a type is available)
+                if 'DW_AT_type' not in nextdie.attributes: # Clang dwarfv2 may not have type, but has a byte size   
+                    if 'DW_AT_byte_size' in nextdie.attributes:
+                        return TypeDescriptor(TypeOfVar.EnumOnly, enum, type_die=enum)
+                    else:
+                        raise ElfParsingError(f"Cannot find the enum underlying type {enum}")
 
             prevdie = nextdie
 
     # When we encounter a struct die, we make a definition that we keep global,
     # this definition includes all submember with their respective offset.
     # each time we will encounter a instance of this struct, we will generate a variable for each sub member
 
-    def die_process_struct_or_class(self, die: "elftools_stubs.Die") -> None:
+    def die_process_struct_class_union(self, die: "elftools_stubs.Die") -> None:
         self.log_debug_process_die(die)
 
         if die not in self.struct_die_map:
-            self.struct_die_map[die] = self.get_struct_or_class_def(die)
+            self.struct_die_map[die] = self.get_composite_type_def(die)
 
 
     # Go down the hierarchy to get the whole struct def in a recursive way
-    def get_struct_or_class_def(self, die: "elftools_stubs.Die") -> Struct:
+    def get_composite_type_def(self, die: "elftools_stubs.Die") -> Struct:
+        """Get the definition of a struct/class/union type"""
+
         self.log_debug_process_die(die)
-        if die.tag not in ['DW_TAG_structure_type', 'DW_TAG_class_type']:
-            raise ValueError('DIE must be a structure or a class type')
+        if die.tag not in ('DW_TAG_structure_type', 'DW_TAG_class_type', 'DW_TAG_union_type'):
+            raise ValueError('DIE must be a structure, class or union type')
 
         struct = Struct(self.get_name(die))
-
+        is_in_union = die.tag == 'DW_TAG_union_type'
         for child in die.iter_children():
             if child.tag == 'DW_TAG_member':
-                member = self.get_member_from_die(child)
+                member = self.get_member_from_die(child, is_in_union)
                 if member is not None:
                     struct.add_member(member)
             elif child.tag == 'DW_TAG_inheritance':
                 offset = 0
-                if 'DW_AT_data_member_location' in child.attributes:
-                    offset = child.attributes['DW_AT_data_member_location'].value
+                if self.has_member_byte_offset(child):
+                    offset = self.get_member_byte_offset(child)
                 refaddr = child.attributes['DW_AT_type'].value + child.cu.cu_offset
                 typedie = child.dwarfinfo.get_DIE_from_refaddr(refaddr)
-                if typedie.tag not in ['DW_TAG_structure_type', 'DW_TAG_class_type']:
+                if typedie.tag not in ['DW_TAG_structure_type', 'DW_TAG_class_type']:   # Add union here?
                     self.logger.warning(f"Line {get_linenumber()}: Inheritance to a type die {self.make_name_for_log(typedie)}. Not supported yet")
                     continue
-                self.die_process_struct_or_class(typedie)
+                self.die_process_struct_class_union(typedie)
                 parent_struct = self.struct_die_map[typedie]
                 struct.inherit(parent_struct, offset=offset)
 
         return struct
+    
+    def has_member_byte_offset(self, die: "elftools_stubs.Die") -> bool:
+        """Tells if an offset relative to the structure base is available on this member die"""
+        return 'DW_AT_data_member_location' in die.attributes
+
+    def get_member_byte_offset(self, die: "elftools_stubs.Die") -> int:
+        """Tell the offset at which this member is located relative to the structure base"""
+
+        if 'DW_AT_data_member_location' not in die.attributes:
+            raise ElfParsingError(f"No member location on die {die}")
+        
+        val = die.attributes['DW_AT_data_member_location'].value
+        if isinstance(val, int):
+            return val
+        
+        if isinstance(val, list):
+            if len(val) < 2:
+                raise ElfParsingError(f"Invalid member offset data length for die {die}")
+            
+            if val[0] != self.DW_OP_plus_uconst:
+                raise ElfParsingError(f"Does not know how to read member location for die {die}. Operator is unsupported")
+
+            return int.from_bytes(val[1:], byteorder= 'little' if self.endianness == Endianness.Little else 'big') 
+
+        raise ElfParsingError(f"Does not know how to read member location for die {die}")
 
+    def process_enum_only_type(self, enum_die:"elftools_stubs.Die") -> str:
+        """With clang Dwarf V2, some enums may have no base type, so we try to deduce it from the propertie son the enum"""
+        enum = self.enum_die_map[enum_die]
+        if 'DW_AT_byte_size' not in enum_die.attributes:
+            raise ElfParsingError(f"Cannot determine enum size {enum_die}")
+        bytesize = enum_die.attributes['DW_AT_byte_size'].value
+        try:
+            encoding = self.DwarfEncoding(cast(int, enum_die.attributes['DW_AT_encoding'].value))
+        except:
+            encoding = self.DwarfEncoding.DW_ATE_signed if enum.has_signed_value() else self.DwarfEncoding.DW_ATE_unsigned
+        basetype = self.get_core_base_type(encoding, bytesize)
+        fakename = 'enum_default_'
+        fakename += 's' if basetype.is_signed() else 'u'
+        fakename += str(basetype.get_size_bit())
+        self.varmap.register_base_type(fakename, basetype)
+        return fakename
+    
     # Read a member die and generate a Struct.Member that we will later on use to register a variable.
     # The struct.Member object contains everything we need to map a
-    def get_member_from_die(self, die: "elftools_stubs.Die") -> Optional[Struct.Member]:
+    def get_member_from_die(self, die: "elftools_stubs.Die", is_in_union:bool=False) -> Optional[Struct.Member]:
         self.log_debug_process_die(die)
-        name = self.get_name(die)
+        try:
+            name = self.get_name(die) 
+        except Exception:
+            name = ""
         type_desc = self.get_type_of_var(die)
         enum:Optional[VariableEnum] = None
-        if type_desc.type in (TypeOfVar.Struct, TypeOfVar.Class):
-            substruct = self.get_struct_or_class_def(type_desc.type_die)  # recursion
+        if type_desc.type in (TypeOfVar.Struct, TypeOfVar.Class, TypeOfVar.Union):
+            substruct = self.get_composite_type_def(type_desc.type_die)  # recursion
             typename = None
-        elif type_desc.type == TypeOfVar.BaseType:
-            self.die_process_base_type(type_desc.type_die)    # Just in case it is unknown yet
+        elif type_desc.type in (TypeOfVar.BaseType, TypeOfVar.EnumOnly):
             if type_desc.enum_die is not None:
                 self.die_process_enum(type_desc.enum_die)
                 enum = self.enum_die_map[type_desc.enum_die]
-            typename = self.get_typename_from_die(type_desc.type_die)
+        
+            if type_desc.type == TypeOfVar.BaseType :
+                self.die_process_base_type(type_desc.type_die)    # Just in case it is unknown yet
+                typename = self.get_typename_from_die(type_desc.type_die)
+            elif type_desc.type == TypeOfVar.EnumOnly:    # clang dwarf v2 may do that for enums
+                assert type_desc.enum_die is type_desc.type_die
+                typename = self.process_enum_only_type(type_desc.enum_die)
+            else:
+                raise ElfParsingError("Impossible to process base type")
+            
             substruct = None
         else:
             self.logger.warning(f"Line {get_linenumber()}: Found a member with a type die {self.make_name_for_log(type_desc.type_die)} (type={type_desc.type.name}). Not supported yet")
             return None
 
 
         # We are looking at a forward declared member.
         if 'DW_AT_declaration' in die.attributes and die.attributes['DW_AT_declaration'].value == True:
             return None
-
-        byte_offset = die.attributes['DW_AT_data_member_location'].value
+        
+        if is_in_union:
+            if self.has_member_byte_offset(die) and self.get_member_byte_offset(die) != 0:
+                raise ElfParsingError("Encountered an union with a non-zero member location.")
+            byte_offset = 0
+        else:
+            byte_offset = self.get_member_byte_offset(die)
 
         if 'DW_AT_bit_offset' in die.attributes:
             if 'DW_AT_byte_size' not in die.attributes:
                 raise ElfParsingError('Missing DW_AT_byte_size for bitfield %s' % (self.get_name(die, '')))
             if 'DW_AT_bit_size' not in die.attributes:
                 raise ElfParsingError('Missing DW_AT_bit_size for bitfield %s' % (self.get_name(die, '')))
 
@@ -576,27 +668,28 @@
             name=name,
             is_substruct=True if substruct is not None else False,
             original_type_name=typename,
             byte_offset=byte_offset,
             bitoffset=bitoffset,
             bitsize=bitsize,
             substruct=substruct,
-            enum=enum
-            
+            enum=enum,
+            is_unnamed = True if (len(name) == 0) else False
         )
 
     # We have an instance of a struct. Use the location and go down the structure recursively
     # using the members offsets to find the final address that we will apply to the output var
     def register_struct_var(self, die: "elftools_stubs.Die", type_die:"elftools_stubs.Die", location: VariableLocation) -> None:
+        """Register an instance of a struct at a given location"""
         path_segments = self.make_varpath(die)
         path_segments.append(self.get_name(die))
         struct = self.struct_die_map[type_die]
         startpoint = Struct.Member(struct.name, is_substruct=True, bitoffset=None, bitsize=None, substruct=struct)
 
-        # Start the recursion
+        # Start the recursion that will create all the sub elements
         self.register_member_as_var_recursive(path_segments, startpoint, location, offset=0)
 
     # Recursive function to dig into a structure and register all possible variables.
     def register_member_as_var_recursive(self, path_segments: List[str], member: Struct.Member, base_location: VariableLocation, offset: int) -> None:
         if member.is_substruct:
             assert member.substruct is not None
             struct = member.substruct
@@ -682,51 +775,67 @@
         """Process a variable die and insert a variable in the varmap object if it has an absolute address"""
         if location is None:
             location = self.get_location(die)
 
         if 'DW_AT_specification' in die.attributes:
             vardie = self.get_die_at_spec(die)
             self.die_process_variable(vardie, location) # Recursion
+       
+        elif 'DW_AT_abstract_origin' in die.attributes:
+            vardie = self.get_die_at_abstract_origin(die)
+            self.die_process_variable(vardie, location) # Recursion
 
         else:
             if location is not None:
                 type_desc = self.get_type_of_var(die)
 
-                if type_desc.type in (TypeOfVar.Struct, TypeOfVar.Class):   # TODO: Union
-                    self.die_process_struct_or_class(type_desc.type_die)
+                # Composite type
+                if type_desc.type in (TypeOfVar.Struct, TypeOfVar.Class, TypeOfVar.Union): 
+                    self.die_process_struct_class_union(type_desc.type_die)
                     self.register_struct_var(die, type_desc.type_die, location)
-                elif type_desc.type == TypeOfVar.BaseType:
+                # Base type
+                elif type_desc.type in (TypeOfVar.BaseType, TypeOfVar.EnumOnly):
                     path_segments = self.make_varpath(die)
                     name = self.get_name(die)
-                    self.die_process_base_type(type_desc.type_die)
+                    
                     enum:Optional[VariableEnum] = None
                     if type_desc.enum_die is not None:
                         self.die_process_enum(type_desc.enum_die)
                         enum = self.enum_die_map[type_desc.enum_die]
-                   
+
+                    if type_desc.type == TypeOfVar.BaseType :   # Most common case
+                        self.die_process_base_type(type_desc.type_die)    # Just in case it is unknown yet
+                        typename = self.get_typename_from_die(type_desc.type_die)
+                    elif type_desc.type == TypeOfVar.EnumOnly:    # clang dwarf v2 may do that for enums
+                        assert type_desc.enum_die is type_desc.type_die
+                        assert type_desc.enum_die is not None
+                        typename = self.process_enum_only_type(type_desc.enum_die)
+                    else:
+                        raise ElfParsingError("Impossible to process base type")
+
                     self.register_variable(
                         name=name,
                         path_segments=path_segments,
                         location=location,
-                        original_type_name=self.get_typename_from_die(type_desc.type_die),
+                        original_type_name=typename,
                         enum=enum
                     )
                 else:
                     self.logger.warning(f"Line {get_linenumber()}: Found a variable with a type die {self.make_name_for_log(type_desc.type_die)} (type={type_desc.type.name}). Not supported yet")
 
     def get_varpath_from_hierarchy(self, die: "elftools_stubs.Die") -> List[str]:
         """Go up in the DWARF hierarchy and make a path segment for each level"""
         segments: List[str] = []
         parent = die.get_parent()
         while parent is not None:
             if parent.tag == 'DW_TAG_compile_unit':
                 break
 
             try:
-                if 'DW_AT_linkage_name' in parent.attributes:
+                if self.has_linkage_name(parent):
                     name = self.get_linkage_name(parent)
                 else:
                     name = self.get_name(parent)
             except Exception:
                 if 'DW_AT_specification' in parent.attributes:
                     parent2 = self.get_die_at_spec(parent)
                     name = self.get_name(parent2)
@@ -734,28 +843,27 @@
             if name is not None:
                 segments.insert(0, name)
             parent = parent.get_parent()
         return segments
 
     def get_varpath_from_linkage_name(self, die: "elftools_stubs.Die") -> List[str]:
         """Generate path segments by parsing the linkage name. Relies on the ability to demangle"""
-        mangled = die.attributes['DW_AT_linkage_name'].value.decode('ascii')
-        demangled = self.demangler.demangle(mangled)
+        demangled = self.get_linkage_name(die)
         segments = demangled.split('::')
         try:
             name = self.get_name(die)
             if segments[-1] == name:
                 segments.pop()
         except Exception:
             pass
         return segments
 
     def make_varpath(self, die: "elftools_stubs.Die") -> List[str]:
         """Generate the display path for a die, either from the hierarchy or the linkage name"""
-        if 'DW_AT_linkage_name' in die.attributes:
+        if self.has_linkage_name(die):
             segments = self.get_varpath_from_linkage_name(die)
         else:
             segments = self.get_varpath_from_hierarchy(die)
 
         if self.is_external(die):
             segments.insert(0, self.GLOBAL)
         else:
```

### Comparing `scrutinydebugger-0.2.0/scrutiny/core/bintools/elftools_stubs.pyi` & `scrutinydebugger-0.2.1/scrutiny/core/bintools/elftools_stubs.pyi`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.0/scrutiny/core/bintools/get_var_memrange.py` & `scrutinydebugger-0.2.1/scrutiny/core/bintools/get_var_memrange.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.0/scrutiny/core/codecs.py` & `scrutinydebugger-0.2.1/scrutiny/core/codecs.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.0/scrutiny/core/datalogging.py` & `scrutinydebugger-0.2.1/scrutiny/core/datalogging.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.0/scrutiny/core/firmware_description.py` & `scrutinydebugger-0.2.1/scrutiny/core/firmware_description.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.0/scrutiny/core/firmware_parser.py` & `scrutinydebugger-0.2.1/scrutiny/core/firmware_parser.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.0/scrutiny/core/memory_content.py` & `scrutinydebugger-0.2.1/scrutiny/core/memory_content.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.0/scrutiny/core/sfd_storage.py` & `scrutinydebugger-0.2.1/scrutiny/core/sfd_storage.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.0/scrutiny/core/typehints.py` & `scrutinydebugger-0.2.1/scrutiny/core/typehints.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.0/scrutiny/core/validation.py` & `scrutinydebugger-0.2.1/scrutiny/core/validation.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.0/scrutiny/core/variable.py` & `scrutinydebugger-0.2.1/scrutiny/core/variable.py`

 * *Files 6% similar despite different names*

```diff
@@ -132,14 +132,21 @@
         """Export to dict for json serialization mainly"""
         obj: VariableEnumDef = {
             'name': self.name,
             'values': self.vals
         }
         return obj
 
+    def has_signed_value(self) -> bool:
+        for v in self.vals.values():
+            if v < 0:
+                return True
+        return False
+
+
     @classmethod
     def from_def(cls, enum_def: VariableEnumDef) -> "VariableEnum":
         """Recreate from a .json dict"""
         obj = VariableEnum(enum_def['name'])
         obj.vals = enum_def['values']
         return obj
 
@@ -150,23 +157,25 @@
         is_substruct: bool
         original_type_name: Optional[str]
         bitoffset: Optional[int]
         byte_offset: Optional[int]
         bitsize: Optional[int]
         substruct: Optional['Struct']
         enum:Optional['VariableEnum']
+        is_unnamed:bool
 
         def __init__(self, name: str,
                      is_substruct: bool = False,
                      original_type_name: Optional[str] = None,
                      byte_offset: Optional[int] = None,
                      bitoffset: Optional[int] = None,
                      bitsize: Optional[int] = None,
                      substruct: Optional['Struct'] = None,
-                     enum:Optional['VariableEnum'] = None
+                     enum:Optional['VariableEnum'] = None,
+                     is_unnamed:bool=False
                      ):
 
             if not is_substruct:
                 if original_type_name is None:
                     raise ValueError('A typename must be given for non-struct member')
 
             if bitoffset is not None:
@@ -186,40 +195,59 @@
                     raise ValueError('byte_offset must be an integer value')
                 if byte_offset < 0:
                     raise ValueError('byte_offset must be a positive integer')
 
             if substruct is not None:
                 if not isinstance(substruct, Struct):
                     raise ValueError('substruct must be Struct instance')
+            
+            if is_unnamed:
+                if not is_substruct:
+                    raise ValueError("Only substruct members can be unnamed")
 
             self.name = name
             self.is_substruct = is_substruct
             self.original_type_name = original_type_name
             self.bitoffset = bitoffset
             self.byte_offset = byte_offset
             self.bitsize = bitsize
             self.substruct = substruct
             self.enum = enum
+            self.is_unnamed = is_unnamed
 
     name: str
     members: Dict[str, "Struct.Member"]
 
     def __init__(self, name: str) -> None:
         self.name = name
         self.members = {}
 
     def add_member(self, member: "Struct.Member") -> None:
         """Add a member to the struct"""
-        if member.name in self.members:
-            raise KeyError('Duplicate member %s' % member.name)
-
         if not isinstance(member, Struct.Member):
             raise ValueError('Node must be a Struct.Member')
-
-        self.members[member.name] = member
+        
+        if member.is_unnamed:
+            # Unnamed struct,class,union are defined like this : struct { struct {int a; int b;}} x
+            # They are considered as being declared at the same level as the members of the parent
+            assert member.is_substruct==True
+            assert member.substruct is not None
+            assert member.byte_offset is not None
+
+            for subtruct_member in member.substruct.members.values():
+                substruct_member2 = deepcopy(subtruct_member)
+                if substruct_member2.byte_offset is None:
+                    raise RuntimeError("Expect byte_offset to be set to handle unnamed composite type")
+                substruct_member2.byte_offset+=member.byte_offset
+                self.add_member(substruct_member2)
+        else:    
+            if member.name in self.members:
+                raise KeyError('Duplicate member %s' % member.name)
+        
+            self.members[member.name] = member
     
     def inherit(self, other:"Struct", offset:int=0) -> None:
         for member in other.members.values():
             member2 = deepcopy(member)
             if member2.byte_offset is None:
                 raise RuntimeError("Expect byte_offset to be set to handle inheritance")
             member2.byte_offset += offset
```

### Comparing `scrutinydebugger-0.2.0/scrutiny/core/varmap.py` & `scrutinydebugger-0.2.1/scrutiny/core/varmap.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.0/scrutiny/sdk/_api_parser.py` & `scrutinydebugger-0.2.1/scrutiny/sdk/_api_parser.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.0/scrutiny/sdk/client.py` & `scrutinydebugger-0.2.1/scrutiny/sdk/client.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.0/scrutiny/sdk/datalogging.py` & `scrutinydebugger-0.2.1/scrutiny/sdk/datalogging.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.0/scrutiny/sdk/definitions.py` & `scrutinydebugger-0.2.1/scrutiny/sdk/definitions.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.0/scrutiny/sdk/exceptions.py` & `scrutinydebugger-0.2.1/scrutiny/sdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.0/scrutiny/sdk/listeners/__init__.py` & `scrutinydebugger-0.2.1/scrutiny/sdk/listeners/__init__.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.0/scrutiny/sdk/listeners/buffered_reader_listener.py` & `scrutinydebugger-0.2.1/scrutiny/sdk/listeners/buffered_reader_listener.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.0/scrutiny/sdk/listeners/csv_file_listener.py` & `scrutinydebugger-0.2.1/scrutiny/sdk/listeners/csv_file_listener.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.0/scrutiny/sdk/listeners/text_stream_listener.py` & `scrutinydebugger-0.2.1/scrutiny/sdk/listeners/text_stream_listener.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.0/scrutiny/sdk/watchable_handle.py` & `scrutinydebugger-0.2.1/scrutiny/sdk/watchable_handle.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.0/scrutiny/sdk/write_request.py` & `scrutinydebugger-0.2.1/scrutiny/sdk/write_request.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.0/scrutiny/server/active_sfd_handler.py` & `scrutinydebugger-0.2.1/scrutiny/server/active_sfd_handler.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.0/scrutiny/server/api/API.py` & `scrutinydebugger-0.2.1/scrutiny/server/api/API.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.0/scrutiny/server/api/abstract_client_handler.py` & `scrutinydebugger-0.2.1/scrutiny/server/api/abstract_client_handler.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.0/scrutiny/server/api/dummy_client_handler.py` & `scrutinydebugger-0.2.1/scrutiny/server/api/dummy_client_handler.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.0/scrutiny/server/api/typing.py` & `scrutinydebugger-0.2.1/scrutiny/server/api/typing.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.0/scrutiny/server/api/value_streamer.py` & `scrutinydebugger-0.2.1/scrutiny/server/api/value_streamer.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.0/scrutiny/server/api/websocket_client_handler.py` & `scrutinydebugger-0.2.1/scrutiny/server/api/websocket_client_handler.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.0/scrutiny/server/datalogging/datalogging_manager.py` & `scrutinydebugger-0.2.1/scrutiny/server/datalogging/datalogging_manager.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.0/scrutiny/server/datalogging/datalogging_storage.py` & `scrutinydebugger-0.2.1/scrutiny/server/datalogging/datalogging_storage.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.0/scrutiny/server/datalogging/datalogging_utilities.py` & `scrutinydebugger-0.2.1/scrutiny/server/datalogging/datalogging_utilities.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.0/scrutiny/server/datalogging/definitions/api.py` & `scrutinydebugger-0.2.1/scrutiny/server/datalogging/definitions/api.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.0/scrutiny/server/datalogging/definitions/device.py` & `scrutinydebugger-0.2.1/scrutiny/server/datalogging/definitions/device.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.0/scrutiny/server/datastore/datastore.py` & `scrutinydebugger-0.2.1/scrutiny/server/datastore/datastore.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.0/scrutiny/server/datastore/datastore_entry.py` & `scrutinydebugger-0.2.1/scrutiny/server/datastore/datastore_entry.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.0/scrutiny/server/datastore/entry_type.py` & `scrutinydebugger-0.2.1/scrutiny/server/datastore/entry_type.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.0/scrutiny/server/device/device_handler.py` & `scrutinydebugger-0.2.1/scrutiny/server/device/device_handler.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.0/scrutiny/server/device/device_info.py` & `scrutinydebugger-0.2.1/scrutiny/server/device/device_info.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.0/scrutiny/server/device/emulated_device.py` & `scrutinydebugger-0.2.1/scrutiny/server/device/emulated_device.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.0/scrutiny/server/device/links/abstract_link.py` & `scrutinydebugger-0.2.1/scrutiny/server/device/links/abstract_link.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.0/scrutiny/server/device/links/dummy_link.py` & `scrutinydebugger-0.2.1/scrutiny/server/device/links/dummy_link.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.0/scrutiny/server/device/links/serial_link.py` & `scrutinydebugger-0.2.1/scrutiny/server/device/links/serial_link.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.0/scrutiny/server/device/links/udp_link.py` & `scrutinydebugger-0.2.1/scrutiny/server/device/links/udp_link.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.0/scrutiny/server/device/request_dispatcher.py` & `scrutinydebugger-0.2.1/scrutiny/server/device/request_dispatcher.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.0/scrutiny/server/device/submodules/datalogging_poller.py` & `scrutinydebugger-0.2.1/scrutiny/server/device/submodules/datalogging_poller.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.0/scrutiny/server/device/submodules/device_searcher.py` & `scrutinydebugger-0.2.1/scrutiny/server/device/submodules/device_searcher.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.0/scrutiny/server/device/submodules/heartbeat_generator.py` & `scrutinydebugger-0.2.1/scrutiny/server/device/submodules/heartbeat_generator.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.0/scrutiny/server/device/submodules/info_poller.py` & `scrutinydebugger-0.2.1/scrutiny/server/device/submodules/info_poller.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.0/scrutiny/server/device/submodules/memory_reader.py` & `scrutinydebugger-0.2.1/scrutiny/server/device/submodules/memory_reader.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.0/scrutiny/server/device/submodules/memory_writer.py` & `scrutinydebugger-0.2.1/scrutiny/server/device/submodules/memory_writer.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.0/scrutiny/server/device/submodules/session_initializer.py` & `scrutinydebugger-0.2.1/scrutiny/server/device/submodules/session_initializer.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.0/scrutiny/server/protocol/comm_handler.py` & `scrutinydebugger-0.2.1/scrutiny/server/protocol/comm_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,14 +66,15 @@
     throttler: Throttler
     rx_bitcount: int
     tx_bitcount: int
     bitcount_time: float
     timed_out: bool
     pending_request: Optional[Request]
     link_type: str
+    last_open_error: Optional[str]
 
     def __init__(self, params: Dict[str, Any] = {}) -> None:
         self.active_request = None      # Contains the request object that has been sent to the device. When None, no request sent and we are standby
         self.received_response = None   # Indicates that a response has been received.
         self.link = None                # Abstracted communication channel that implements  initialize, destroy, write, read
         self.params = copy(self.DEFAULT_PARAMS)
         self.params.update(cast(CommHandler.Params, params))
@@ -81,14 +82,15 @@
         self.response_timer = Timer(self.params['response_timeout'])    # Timer for response timeout management
         self.rx_data = self.RxData()    # Contains the response data while we read it.
         self.logger = logging.getLogger(self.__class__.__name__)
         self.opened = False     # True when communication channel is active and working.
         self.reset_bitrate_monitor()
         self.throttler = Throttler()
         self.link_type = "none"
+        self.last_open_error = None
 
     def enable_throttling(self, bitrate: float) -> None:
         """Enable throttling on communication.
         Overall bitrate (incoming and outgoing data included) will try to be respected.
         This does not take in account the protocol overhead. Just the payload sum.
         """
         self.throttler.set_bitrate(bitrate)
@@ -131,14 +133,15 @@
             self.link_type = "none"
             return
 
         self.link_type = link_type
 
         link_class = self.get_link_class(link_type)
         self.link = link_class.make(link_config)
+        self.last_open_error = None
 
     def validate_link_config(self, link_type: str, link_config: LinkConfig) -> None:
         """Raises an exception if the given configuration is wrong for the given link type"""
         link_class = self.get_link_class(link_type)
         return link_class.validate_config(link_config)
 
     def get_link_class(self, link_type: str) -> Type[AbstractLink]:
@@ -166,29 +169,37 @@
         """Try to open the communication channel with the device."""
         if self.link is None:
             raise Exception('Link must be set before opening')
 
         try:
             self.link.initialize()
             self.opened = True
+            self.last_open_error = None
         except Exception as e:
-            self.logger.error("Cannot connect to device. " + str(e))
-            self.opened = False
+            err = str(e)
+            full_error = f"Cannot initialize device. {err}"
+            if self.last_open_error != err:
+                self.logger.error(full_error)
+            elif self.logger.isEnabledFor(logging.DEBUG):
+                self.logger.debug(full_error)
+            self.last_open_error = err
+            self.opened = False 
 
     def is_open(self) -> bool:
         """Return True if the communication channel is open with the device"""
         return self.opened
 
     def close(self) -> None:
         """Close the communication channel with the device"""
         if self.link is not None:
             self.link.destroy()
 
         self.reset()
         self.opened = False
+        self.last_open_error = None
 
     def is_operational(self) -> bool:
         """Return True if the communication channel is presently in a healthy state."""
         if self.link is None:
             return False
 
         return self.opened and self.link.operational()
```

### Comparing `scrutinydebugger-0.2.0/scrutiny/server/protocol/commands/base_command.py` & `scrutinydebugger-0.2.1/scrutiny/server/protocol/commands/base_command.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.0/scrutiny/server/protocol/commands/comm_control.py` & `scrutinydebugger-0.2.1/scrutiny/server/protocol/commands/comm_control.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.0/scrutiny/server/protocol/commands/datalog_control.py` & `scrutinydebugger-0.2.1/scrutiny/server/protocol/commands/datalog_control.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.0/scrutiny/server/protocol/commands/dummy_command.py` & `scrutinydebugger-0.2.1/scrutiny/server/protocol/commands/dummy_command.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.0/scrutiny/server/protocol/commands/get_info.py` & `scrutinydebugger-0.2.1/scrutiny/server/protocol/commands/get_info.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.0/scrutiny/server/protocol/commands/memory_control.py` & `scrutinydebugger-0.2.1/scrutiny/server/protocol/commands/memory_control.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.0/scrutiny/server/protocol/crc32.py` & `scrutinydebugger-0.2.1/scrutiny/server/protocol/crc32.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.0/scrutiny/server/protocol/exceptions.py` & `scrutinydebugger-0.2.1/scrutiny/server/protocol/exceptions.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.0/scrutiny/server/protocol/protocol.py` & `scrutinydebugger-0.2.1/scrutiny/server/protocol/protocol.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.0/scrutiny/server/protocol/request.py` & `scrutinydebugger-0.2.1/scrutiny/server/protocol/request.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.0/scrutiny/server/protocol/response.py` & `scrutinydebugger-0.2.1/scrutiny/server/protocol/response.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.0/scrutiny/server/protocol/typing.py` & `scrutinydebugger-0.2.1/scrutiny/server/protocol/typing.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.0/scrutiny/server/server.py` & `scrutinydebugger-0.2.1/scrutiny/server/server.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.0/scrutiny/tools/synchronous_websocket_server.py` & `scrutinydebugger-0.2.1/scrutiny/tools/synchronous_websocket_server.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.0/scrutiny/tools/throttler.py` & `scrutinydebugger-0.2.1/scrutiny/tools/throttler.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.0/scrutiny/tools/timer.py` & `scrutinydebugger-0.2.1/scrutiny/tools/timer.py`

 * *Files identical despite different names*

### Comparing `scrutinydebugger-0.2.0/scrutinydebugger.egg-info/PKG-INFO` & `scrutinydebugger-0.2.1/scrutinydebugger.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrutinydebugger
-Version: 0.2.0
+Version: 0.2.1
 Summary: Scrutiny debugger Python framework
 Home-page: https://github.com/scrutinydebugger/scrutiny-python
 Author: Pier-Yves Lessard
 License: MIT
 Requires-Python: >3.8
 License-File: LICENSE
 Requires-Dist: appdirs>=1.4.4
```

### Comparing `scrutinydebugger-0.2.0/scrutinydebugger.egg-info/SOURCES.txt` & `scrutinydebugger-0.2.1/scrutinydebugger.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -108,14 +108,15 @@
 scrutiny/server/protocol/commands/comm_control.py
 scrutiny/server/protocol/commands/datalog_control.py
 scrutiny/server/protocol/commands/dummy_command.py
 scrutiny/server/protocol/commands/get_info.py
 scrutiny/server/protocol/commands/memory_control.py
 scrutiny/server/protocol/commands/user_command.py
 scrutiny/tools/__init__.py
+scrutiny/tools/selectable_queue.py
 scrutiny/tools/synchronous_websocket_server.py
 scrutiny/tools/throttler.py
 scrutiny/tools/timer.py
 scrutinydebugger.egg-info/PKG-INFO
 scrutinydebugger.egg-info/SOURCES.txt
 scrutinydebugger.egg-info/dependency_links.txt
 scrutinydebugger.egg-info/entry_points.txt
```

### Comparing `scrutinydebugger-0.2.0/setup.py` & `scrutinydebugger-0.2.1/setup.py`

 * *Files identical despite different names*

