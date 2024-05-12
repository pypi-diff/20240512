# Comparing `tmp/regipy-4.2.0.tar.gz` & `tmp/regipy-4.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "regipy-4.2.0.tar", last modified: Mon Apr 15 18:45:25 2024, max compression
+gzip compressed data, was "regipy-4.2.1.tar", last modified: Sun May 12 14:34:18 2024, max compression
```

## Comparing `regipy-4.2.0.tar` & `regipy-4.2.1.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:45:25.427455 regipy-4.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-15 18:45:17.000000 regipy-4.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-15 18:45:17.000000 regipy-4.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3315 2024-04-15 18:45:25.427455 regipy-4.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10010 2024-04-15 18:45:17.000000 regipy-4.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:45:25.415455 regipy-4.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-15 18:45:17.000000 regipy-4.2.0/docs/PLUGINS.md
--rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-04-15 18:45:17.000000 regipy-4.2.0/docs/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:45:25.419455 regipy-4.2.0/regipy/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10522 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2431 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/cli_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    27229 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/hive_types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:45:25.419455 regipy-4.2.0/regipy/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:45:25.419455 regipy-4.2.0/regipy/plugins/amcache/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/plugins/amcache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3867 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/plugins/amcache/amcache.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:45:25.419455 regipy-4.2.0/regipy/plugins/bcd/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/plugins/bcd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3399 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/plugins/bcd/boot_entry_list.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:45:25.423455 regipy-4.2.0/regipy/plugins/ntuser/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/plugins/ntuser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/plugins/ntuser/classes_installer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/plugins/ntuser/installed_programs_ntuser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/plugins/ntuser/network_drives.py
--rw-r--r--   0 runner    (1001) docker     (127)     1765 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/plugins/ntuser/persistence.py
--rw-r--r--   0 runner    (1001) docker     (127)    13417 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/plugins/ntuser/shellbags_ntuser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/plugins/ntuser/tsclient.py
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/plugins/ntuser/typed_paths.py
--rw-r--r--   0 runner    (1001) docker     (127)      984 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/plugins/ntuser/typed_urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     4945 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/plugins/ntuser/user_assist.py
--rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/plugins/ntuser/winrar.py
--rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/plugins/ntuser/winscp_saved_sessions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/plugins/ntuser/word_wheel_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/plugins/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/plugins/plugin_template.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:45:25.423455 regipy-4.2.0/regipy/plugins/sam/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/plugins/sam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/plugins/sam/local_sid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:45:25.423455 regipy-4.2.0/regipy/plugins/security/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/plugins/security/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/plugins/security/domain_sid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:45:25.423455 regipy-4.2.0/regipy/plugins/software/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/plugins/software/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/plugins/software/classes_installer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/plugins/software/image_file_execution_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/plugins/software/installed_programs.py
--rw-r--r--   0 runner    (1001) docker     (127)      981 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/plugins/software/last_logon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/plugins/software/persistence.py
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/plugins/software/printdemon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/plugins/software/profilelist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/plugins/software/tracing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/plugins/software/uac.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:45:25.427455 regipy-4.2.0/regipy/plugins/system/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/plugins/system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/plugins/system/active_controlset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/plugins/system/bam.py
--rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/plugins/system/bootkey.py
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/plugins/system/computer_name.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:45:25.427455 regipy-4.2.0/regipy/plugins/system/external/
--rwxr-xr-x   0 runner    (1001) docker     (127)    17390 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/plugins/system/external/ShimCacheParser.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/plugins/system/external/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/plugins/system/host_domain_name.py
--rw-r--r--   0 runner    (1001) docker     (127)     3581 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/plugins/system/network_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/plugins/system/routes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/plugins/system/safeboot_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/plugins/system/services.py
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/plugins/system/shimcache.py
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/plugins/system/timezone_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     5471 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/plugins/system/usbstor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/plugins/system/wdigest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:45:25.427455 regipy-4.2.0/regipy/plugins/usrclass/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/plugins/usrclass/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13677 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/plugins/usrclass/shellbags_usrclass.py
--rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/plugins/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8406 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/recovery.py
--rw-r--r--   0 runner    (1001) docker     (127)     6744 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/regdiff.py
--rw-r--r--   0 runner    (1001) docker     (127)    26690 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)      969 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/security_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8721 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/structs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5521 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:45:25.427455 regipy-4.2.0/regipy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3315 2024-04-15 18:45:25.000000 regipy-4.2.0/regipy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-04-15 18:45:25.000000 regipy-4.2.0/regipy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 18:45:25.000000 regipy-4.2.0/regipy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-15 18:45:25.000000 regipy-4.2.0/regipy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-15 18:45:25.000000 regipy-4.2.0/regipy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-15 18:45:25.000000 regipy-4.2.0/regipy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 18:45:25.427455 regipy-4.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3004 2024-04-15 18:45:17.000000 regipy-4.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 14:34:18.066654 regipy-4.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-12 14:34:11.000000 regipy-4.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-12 14:34:11.000000 regipy-4.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3315 2024-05-12 14:34:18.066654 regipy-4.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10010 2024-05-12 14:34:11.000000 regipy-4.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 14:34:18.050654 regipy-4.2.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-12 14:34:11.000000 regipy-4.2.1/docs/PLUGINS.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-05-12 14:34:11.000000 regipy-4.2.1/docs/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 14:34:18.054654 regipy-4.2.1/regipy/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-12 14:34:11.000000 regipy-4.2.1/regipy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10522 2024-05-12 14:34:11.000000 regipy-4.2.1/regipy/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2431 2024-05-12 14:34:11.000000 regipy-4.2.1/regipy/cli_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27229 2024-05-12 14:34:11.000000 regipy-4.2.1/regipy/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-12 14:34:11.000000 regipy-4.2.1/regipy/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-12 14:34:11.000000 regipy-4.2.1/regipy/hive_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 14:34:18.054654 regipy-4.2.1/regipy/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-05-12 14:34:11.000000 regipy-4.2.1/regipy/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 14:34:18.054654 regipy-4.2.1/regipy/plugins/amcache/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 14:34:11.000000 regipy-4.2.1/regipy/plugins/amcache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3867 2024-05-12 14:34:11.000000 regipy-4.2.1/regipy/plugins/amcache/amcache.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 14:34:18.054654 regipy-4.2.1/regipy/plugins/bcd/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 14:34:11.000000 regipy-4.2.1/regipy/plugins/bcd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3399 2024-05-12 14:34:11.000000 regipy-4.2.1/regipy/plugins/bcd/boot_entry_list.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 14:34:18.058654 regipy-4.2.1/regipy/plugins/ntuser/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 14:34:11.000000 regipy-4.2.1/regipy/plugins/ntuser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-05-12 14:34:11.000000 regipy-4.2.1/regipy/plugins/ntuser/classes_installer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-05-12 14:34:11.000000 regipy-4.2.1/regipy/plugins/ntuser/installed_programs_ntuser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-05-12 14:34:11.000000 regipy-4.2.1/regipy/plugins/ntuser/network_drives.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1765 2024-05-12 14:34:11.000000 regipy-4.2.1/regipy/plugins/ntuser/persistence.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13417 2024-05-12 14:34:11.000000 regipy-4.2.1/regipy/plugins/ntuser/shellbags_ntuser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-12 14:34:11.000000 regipy-4.2.1/regipy/plugins/ntuser/tsclient.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-05-12 14:34:11.000000 regipy-4.2.1/regipy/plugins/ntuser/typed_paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-05-12 14:34:11.000000 regipy-4.2.1/regipy/plugins/ntuser/typed_urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4945 2024-05-12 14:34:11.000000 regipy-4.2.1/regipy/plugins/ntuser/user_assist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-05-12 14:34:11.000000 regipy-4.2.1/regipy/plugins/ntuser/winrar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-05-12 14:34:11.000000 regipy-4.2.1/regipy/plugins/ntuser/winscp_saved_sessions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-05-12 14:34:11.000000 regipy-4.2.1/regipy/plugins/ntuser/word_wheel_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-05-12 14:34:11.000000 regipy-4.2.1/regipy/plugins/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-12 14:34:11.000000 regipy-4.2.1/regipy/plugins/plugin_template.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 14:34:18.058654 regipy-4.2.1/regipy/plugins/sam/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 14:34:11.000000 regipy-4.2.1/regipy/plugins/sam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-05-12 14:34:11.000000 regipy-4.2.1/regipy/plugins/sam/local_sid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 14:34:18.058654 regipy-4.2.1/regipy/plugins/security/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 14:34:11.000000 regipy-4.2.1/regipy/plugins/security/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-05-12 14:34:11.000000 regipy-4.2.1/regipy/plugins/security/domain_sid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 14:34:18.062654 regipy-4.2.1/regipy/plugins/software/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 14:34:11.000000 regipy-4.2.1/regipy/plugins/software/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-05-12 14:34:11.000000 regipy-4.2.1/regipy/plugins/software/classes_installer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-05-12 14:34:11.000000 regipy-4.2.1/regipy/plugins/software/image_file_execution_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-05-12 14:34:11.000000 regipy-4.2.1/regipy/plugins/software/installed_programs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-05-12 14:34:11.000000 regipy-4.2.1/regipy/plugins/software/last_logon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-05-12 14:34:11.000000 regipy-4.2.1/regipy/plugins/software/persistence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-12 14:34:11.000000 regipy-4.2.1/regipy/plugins/software/printdemon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-05-12 14:34:11.000000 regipy-4.2.1/regipy/plugins/software/profilelist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-05-12 14:34:11.000000 regipy-4.2.1/regipy/plugins/software/tracing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-05-12 14:34:11.000000 regipy-4.2.1/regipy/plugins/software/uac.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 14:34:18.062654 regipy-4.2.1/regipy/plugins/system/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 14:34:11.000000 regipy-4.2.1/regipy/plugins/system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-05-12 14:34:11.000000 regipy-4.2.1/regipy/plugins/system/active_controlset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-05-12 14:34:11.000000 regipy-4.2.1/regipy/plugins/system/bam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-05-12 14:34:11.000000 regipy-4.2.1/regipy/plugins/system/bootkey.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-12 14:34:11.000000 regipy-4.2.1/regipy/plugins/system/computer_name.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 14:34:18.062654 regipy-4.2.1/regipy/plugins/system/external/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    17390 2024-05-12 14:34:11.000000 regipy-4.2.1/regipy/plugins/system/external/ShimCacheParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 14:34:11.000000 regipy-4.2.1/regipy/plugins/system/external/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-05-12 14:34:11.000000 regipy-4.2.1/regipy/plugins/system/host_domain_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3581 2024-05-12 14:34:11.000000 regipy-4.2.1/regipy/plugins/system/network_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-05-12 14:34:11.000000 regipy-4.2.1/regipy/plugins/system/routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-05-12 14:34:11.000000 regipy-4.2.1/regipy/plugins/system/safeboot_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-05-12 14:34:11.000000 regipy-4.2.1/regipy/plugins/system/services.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-05-12 14:34:11.000000 regipy-4.2.1/regipy/plugins/system/shimcache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-12 14:34:11.000000 regipy-4.2.1/regipy/plugins/system/timezone_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5471 2024-05-12 14:34:11.000000 regipy-4.2.1/regipy/plugins/system/usbstor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-12 14:34:11.000000 regipy-4.2.1/regipy/plugins/system/wdigest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 14:34:18.062654 regipy-4.2.1/regipy/plugins/usrclass/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 14:34:11.000000 regipy-4.2.1/regipy/plugins/usrclass/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13677 2024-05-12 14:34:11.000000 regipy-4.2.1/regipy/plugins/usrclass/shellbags_usrclass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-05-12 14:34:11.000000 regipy-4.2.1/regipy/plugins/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8406 2024-05-12 14:34:11.000000 regipy-4.2.1/regipy/recovery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6744 2024-05-12 14:34:11.000000 regipy-4.2.1/regipy/regdiff.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26690 2024-05-12 14:34:11.000000 regipy-4.2.1/regipy/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-05-12 14:34:11.000000 regipy-4.2.1/regipy/security_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8721 2024-05-12 14:34:11.000000 regipy-4.2.1/regipy/structs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5521 2024-05-12 14:34:11.000000 regipy-4.2.1/regipy/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 14:34:18.062654 regipy-4.2.1/regipy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3315 2024-05-12 14:34:18.000000 regipy-4.2.1/regipy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-05-12 14:34:18.000000 regipy-4.2.1/regipy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 14:34:18.000000 regipy-4.2.1/regipy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-12 14:34:18.000000 regipy-4.2.1/regipy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-12 14:34:18.000000 regipy-4.2.1/regipy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-12 14:34:18.000000 regipy-4.2.1/regipy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 14:34:18.066654 regipy-4.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3004 2024-05-12 14:34:11.000000 regipy-4.2.1/setup.py
```

### Comparing `regipy-4.2.0/LICENSE` & `regipy-4.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `regipy-4.2.0/PKG-INFO` & `regipy-4.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: regipy
-Version: 4.2.0
+Version: 4.2.1
 Summary: Python Registry Parser
 Home-page: https://github.com/mkorman90/regipy/
 Author: Martin G. Korman
 Author-email: martin@centauri.co.il
 License: MIT
 Keywords: Python,Python3,registry,windows registry,registry parser
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `regipy-4.2.0/README.md` & `regipy-4.2.1/README.md`

 * *Files identical despite different names*

### Comparing `regipy-4.2.0/docs/PLUGINS.md` & `regipy-4.2.1/docs/PLUGINS.md`

 * *Files identical despite different names*

### Comparing `regipy-4.2.0/docs/README.rst` & `regipy-4.2.1/docs/README.rst`

 * *Files identical despite different names*

### Comparing `regipy-4.2.0/regipy/cli.py` & `regipy-4.2.1/regipy/cli.py`

 * *Files identical despite different names*

### Comparing `regipy-4.2.0/regipy/cli_utils.py` & `regipy-4.2.1/regipy/cli_utils.py`

 * *Files identical despite different names*

### Comparing `regipy-4.2.0/regipy/constants.py` & `regipy-4.2.1/regipy/constants.py`

 * *Files identical despite different names*

### Comparing `regipy-4.2.0/regipy/exceptions.py` & `regipy-4.2.1/regipy/exceptions.py`

 * *Files identical despite different names*

### Comparing `regipy-4.2.0/regipy/hive_types.py` & `regipy-4.2.1/regipy/hive_types.py`

 * *Files identical despite different names*

### Comparing `regipy-4.2.0/regipy/plugins/__init__.py` & `regipy-4.2.1/regipy/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `regipy-4.2.0/regipy/plugins/amcache/amcache.py` & `regipy-4.2.1/regipy/plugins/amcache/amcache.py`

 * *Files identical despite different names*

### Comparing `regipy-4.2.0/regipy/plugins/bcd/boot_entry_list.py` & `regipy-4.2.1/regipy/plugins/bcd/boot_entry_list.py`

 * *Files identical despite different names*

### Comparing `regipy-4.2.0/regipy/plugins/ntuser/classes_installer.py` & `regipy-4.2.1/regipy/plugins/ntuser/classes_installer.py`

 * *Files identical despite different names*

### Comparing `regipy-4.2.0/regipy/plugins/ntuser/installed_programs_ntuser.py` & `regipy-4.2.1/regipy/plugins/ntuser/installed_programs_ntuser.py`

 * *Files identical despite different names*

### Comparing `regipy-4.2.0/regipy/plugins/ntuser/network_drives.py` & `regipy-4.2.1/regipy/plugins/ntuser/network_drives.py`

 * *Files identical despite different names*

### Comparing `regipy-4.2.0/regipy/plugins/ntuser/persistence.py` & `regipy-4.2.1/regipy/plugins/ntuser/persistence.py`

 * *Files identical despite different names*

### Comparing `regipy-4.2.0/regipy/plugins/ntuser/shellbags_ntuser.py` & `regipy-4.2.1/regipy/plugins/ntuser/shellbags_ntuser.py`

 * *Files identical despite different names*

### Comparing `regipy-4.2.0/regipy/plugins/ntuser/tsclient.py` & `regipy-4.2.1/regipy/plugins/ntuser/tsclient.py`

 * *Files identical despite different names*

### Comparing `regipy-4.2.0/regipy/plugins/ntuser/typed_paths.py` & `regipy-4.2.1/regipy/plugins/ntuser/typed_paths.py`

 * *Files identical despite different names*

### Comparing `regipy-4.2.0/regipy/plugins/ntuser/typed_urls.py` & `regipy-4.2.1/regipy/plugins/ntuser/typed_urls.py`

 * *Files identical despite different names*

### Comparing `regipy-4.2.0/regipy/plugins/ntuser/user_assist.py` & `regipy-4.2.1/regipy/plugins/ntuser/user_assist.py`

 * *Files identical despite different names*

### Comparing `regipy-4.2.0/regipy/plugins/ntuser/winrar.py` & `regipy-4.2.1/regipy/plugins/ntuser/winrar.py`

 * *Files identical despite different names*

### Comparing `regipy-4.2.0/regipy/plugins/ntuser/winscp_saved_sessions.py` & `regipy-4.2.1/regipy/plugins/ntuser/winscp_saved_sessions.py`

 * *Files identical despite different names*

### Comparing `regipy-4.2.0/regipy/plugins/ntuser/word_wheel_query.py` & `regipy-4.2.1/regipy/plugins/ntuser/word_wheel_query.py`

 * *Files identical despite different names*

### Comparing `regipy-4.2.0/regipy/plugins/plugin.py` & `regipy-4.2.1/regipy/plugins/plugin.py`

 * *Files identical despite different names*

### Comparing `regipy-4.2.0/regipy/plugins/plugin_template.py` & `regipy-4.2.1/regipy/plugins/plugin_template.py`

 * *Files identical despite different names*

### Comparing `regipy-4.2.0/regipy/plugins/sam/local_sid.py` & `regipy-4.2.1/regipy/plugins/sam/local_sid.py`

 * *Files identical despite different names*

### Comparing `regipy-4.2.0/regipy/plugins/security/domain_sid.py` & `regipy-4.2.1/regipy/plugins/security/domain_sid.py`

 * *Files identical despite different names*

### Comparing `regipy-4.2.0/regipy/plugins/software/classes_installer.py` & `regipy-4.2.1/regipy/plugins/software/classes_installer.py`

 * *Files identical despite different names*

### Comparing `regipy-4.2.0/regipy/plugins/software/image_file_execution_options.py` & `regipy-4.2.1/regipy/plugins/software/image_file_execution_options.py`

 * *Files identical despite different names*

### Comparing `regipy-4.2.0/regipy/plugins/software/installed_programs.py` & `regipy-4.2.1/regipy/plugins/software/installed_programs.py`

 * *Files identical despite different names*

### Comparing `regipy-4.2.0/regipy/plugins/software/last_logon.py` & `regipy-4.2.1/regipy/plugins/software/last_logon.py`

 * *Files identical despite different names*

### Comparing `regipy-4.2.0/regipy/plugins/software/persistence.py` & `regipy-4.2.1/regipy/plugins/software/persistence.py`

 * *Files identical despite different names*

### Comparing `regipy-4.2.0/regipy/plugins/software/printdemon.py` & `regipy-4.2.1/regipy/plugins/software/printdemon.py`

 * *Files identical despite different names*

### Comparing `regipy-4.2.0/regipy/plugins/software/profilelist.py` & `regipy-4.2.1/regipy/plugins/software/profilelist.py`

 * *Files identical despite different names*

### Comparing `regipy-4.2.0/regipy/plugins/software/tracing.py` & `regipy-4.2.1/regipy/plugins/software/tracing.py`

 * *Files identical despite different names*

### Comparing `regipy-4.2.0/regipy/plugins/software/uac.py` & `regipy-4.2.1/regipy/plugins/software/uac.py`

 * *Files identical despite different names*

### Comparing `regipy-4.2.0/regipy/plugins/system/active_controlset.py` & `regipy-4.2.1/regipy/plugins/system/active_controlset.py`

 * *Files identical despite different names*

### Comparing `regipy-4.2.0/regipy/plugins/system/bam.py` & `regipy-4.2.1/regipy/plugins/system/bam.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,50 +5,53 @@
 from regipy.exceptions import RegistryKeyNotFoundException
 from regipy.hive_types import SYSTEM_HIVE_TYPE
 from regipy.plugins.plugin import Plugin
 from regipy.utils import convert_wintime
 
 logger = logging.getLogger(__name__)
 
-BAM_PATH = r'Services\bam\UserSettings'
+BAM_PATH = [r'Services\bam\UserSettings',
+            r'Services\bam\state\UserSettings']
 
 
 class BAMPlugin(Plugin):
     NAME = 'background_activity_moderator'
     DESCRIPTION = 'Get the computer name'
     COMPATIBLE_HIVE = SYSTEM_HIVE_TYPE
 
     def run(self):
         logger.debug('Started Computer Name Plugin...')
 
-        try:
-            for subkey_path in self.registry_hive.get_control_sets(BAM_PATH):
-                subkey = self.registry_hive.get_key(subkey_path)
-                for sid_subkey in subkey.iter_subkeys():
-
-                    sid = sid_subkey.name
-                    logger.debug(f'Parsing BAM for {sid}')
-                    sequence_number = None
-                    version = None
-                    entries = []
-
-                    for value in sid_subkey.get_values(trim_values=self.trim_values):
-                        if value.name == 'SequenceNumber':
-                            sequence_number = value.value
-                        elif value.name == 'Version':
-                            version = value.value
-                        else:
-                            entries.append({
-                                'executable': value.name,
-                                'timestamp': convert_wintime(Int64ul.parse(value.value), as_json=self.as_json)
-                            })
-
-                    self.entries.extend([
-                        {
-                            'sequence_number': sequence_number,
-                            'version': version,
-                            'sid': sid,
-                            **x
-                        } for x in entries]
-                    )
-        except RegistryKeyNotFoundException as ex:
-            logger.error(ex)
+        for path in BAM_PATH:
+            try:
+                for subkey_path in self.registry_hive.get_control_sets(path):
+                    subkey = self.registry_hive.get_key(subkey_path)
+                    for sid_subkey in subkey.iter_subkeys():
+
+                        sid = sid_subkey.name
+                        logger.debug(f'Parsing BAM for {sid}')
+                        sequence_number = None
+                        version = None
+                        entries = []
+
+                        for value in sid_subkey.get_values(trim_values=self.trim_values):
+                            if value.name == 'SequenceNumber':
+                                sequence_number = value.value
+                            elif value.name == 'Version':
+                                version = value.value
+                            else:
+                                entries.append({
+                                    'executable': value.name,
+                                    'timestamp': convert_wintime(Int64ul.parse(value.value), as_json=self.as_json)
+                                })
+
+                        self.entries.extend([
+                            {
+                                'sequence_number': sequence_number,
+                                'version': version,
+                                'sid': sid,
+                                'key_path': f'{subkey_path}\\{sid}',
+                                **x
+                            } for x in entries]
+                        )
+            except RegistryKeyNotFoundException as ex:
+                logger.error(ex)
```

### Comparing `regipy-4.2.0/regipy/plugins/system/bootkey.py` & `regipy-4.2.1/regipy/plugins/system/bootkey.py`

 * *Files identical despite different names*

### Comparing `regipy-4.2.0/regipy/plugins/system/computer_name.py` & `regipy-4.2.1/regipy/plugins/system/computer_name.py`

 * *Files identical despite different names*

### Comparing `regipy-4.2.0/regipy/plugins/system/external/ShimCacheParser.py` & `regipy-4.2.1/regipy/plugins/system/external/ShimCacheParser.py`

 * *Files identical despite different names*

### Comparing `regipy-4.2.0/regipy/plugins/system/host_domain_name.py` & `regipy-4.2.1/regipy/plugins/system/host_domain_name.py`

 * *Files identical despite different names*

### Comparing `regipy-4.2.0/regipy/plugins/system/network_data.py` & `regipy-4.2.1/regipy/plugins/system/network_data.py`

 * *Files identical despite different names*

### Comparing `regipy-4.2.0/regipy/plugins/system/routes.py` & `regipy-4.2.1/regipy/plugins/system/routes.py`

 * *Files identical despite different names*

### Comparing `regipy-4.2.0/regipy/plugins/system/safeboot_configuration.py` & `regipy-4.2.1/regipy/plugins/system/safeboot_configuration.py`

 * *Files identical despite different names*

### Comparing `regipy-4.2.0/regipy/plugins/system/services.py` & `regipy-4.2.1/regipy/plugins/system/services.py`

 * *Files identical despite different names*

### Comparing `regipy-4.2.0/regipy/plugins/system/shimcache.py` & `regipy-4.2.1/regipy/plugins/system/shimcache.py`

 * *Files identical despite different names*

### Comparing `regipy-4.2.0/regipy/plugins/system/timezone_data.py` & `regipy-4.2.1/regipy/plugins/system/timezone_data.py`

 * *Files identical despite different names*

### Comparing `regipy-4.2.0/regipy/plugins/system/usbstor.py` & `regipy-4.2.1/regipy/plugins/system/usbstor.py`

 * *Files identical despite different names*

### Comparing `regipy-4.2.0/regipy/plugins/system/wdigest.py` & `regipy-4.2.1/regipy/plugins/system/wdigest.py`

 * *Files identical despite different names*

### Comparing `regipy-4.2.0/regipy/plugins/usrclass/shellbags_usrclass.py` & `regipy-4.2.1/regipy/plugins/usrclass/shellbags_usrclass.py`

 * *Files identical despite different names*

### Comparing `regipy-4.2.0/regipy/plugins/utils.py` & `regipy-4.2.1/regipy/plugins/utils.py`

 * *Files identical despite different names*

### Comparing `regipy-4.2.0/regipy/recovery.py` & `regipy-4.2.1/regipy/recovery.py`

 * *Files identical despite different names*

### Comparing `regipy-4.2.0/regipy/regdiff.py` & `regipy-4.2.1/regipy/regdiff.py`

 * *Files identical despite different names*

### Comparing `regipy-4.2.0/regipy/registry.py` & `regipy-4.2.1/regipy/registry.py`

 * *Files identical despite different names*

### Comparing `regipy-4.2.0/regipy/security_utils.py` & `regipy-4.2.1/regipy/security_utils.py`

 * *Files identical despite different names*

### Comparing `regipy-4.2.0/regipy/structs.py` & `regipy-4.2.1/regipy/structs.py`

 * *Files identical despite different names*

### Comparing `regipy-4.2.0/regipy/utils.py` & `regipy-4.2.1/regipy/utils.py`

 * *Files identical despite different names*

### Comparing `regipy-4.2.0/regipy.egg-info/PKG-INFO` & `regipy-4.2.1/regipy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: regipy
-Version: 4.2.0
+Version: 4.2.1
 Summary: Python Registry Parser
 Home-page: https://github.com/mkorman90/regipy/
 Author: Martin G. Korman
 Author-email: martin@centauri.co.il
 License: MIT
 Keywords: Python,Python3,registry,windows registry,registry parser
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `regipy-4.2.0/regipy.egg-info/SOURCES.txt` & `regipy-4.2.1/regipy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `regipy-4.2.0/setup.py` & `regipy-4.2.1/setup.py`

 * *Files identical despite different names*

