# Comparing `tmp/PySingBoxConverter-0.4.4.dev0.tar.gz` & `tmp/pysingboxconverter-0.5.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PySingBoxConverter-0.4.4.dev0.tar", last modified: Thu Jan  4 19:02:32 2024, max compression
+gzip compressed data, was "pysingboxconverter-0.5.0.dev0.tar", last modified: Sun May 12 09:33:34 2024, max compression
```

## Comparing `PySingBoxConverter-0.4.4.dev0.tar` & `pysingboxconverter-0.5.0.dev0.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 19:02:32.286881 PySingBoxConverter-0.4.4.dev0/
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-01-04 19:02:23.000000 PySingBoxConverter-0.4.4.dev0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-01-04 19:02:32.286881 PySingBoxConverter-0.4.4.dev0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-01-04 19:02:23.000000 PySingBoxConverter-0.4.4.dev0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-01-04 19:02:32.286881 PySingBoxConverter-0.4.4.dev0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-01-04 19:02:23.000000 PySingBoxConverter-0.4.4.dev0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 19:02:32.278881 PySingBoxConverter-0.4.4.dev0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 19:02:32.286881 PySingBoxConverter-0.4.4.dev0/src/PySingBoxConverter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-01-04 19:02:32.000000 PySingBoxConverter-0.4.4.dev0/src/PySingBoxConverter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-01-04 19:02:32.000000 PySingBoxConverter-0.4.4.dev0/src/PySingBoxConverter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-04 19:02:32.000000 PySingBoxConverter-0.4.4.dev0/src/PySingBoxConverter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-01-04 19:02:32.000000 PySingBoxConverter-0.4.4.dev0/src/PySingBoxConverter.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-01-04 19:02:32.000000 PySingBoxConverter-0.4.4.dev0/src/PySingBoxConverter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-01-04 19:02:32.000000 PySingBoxConverter-0.4.4.dev0/src/PySingBoxConverter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-04 19:02:32.000000 PySingBoxConverter-0.4.4.dev0/src/PySingBoxConverter.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 19:02:32.282881 PySingBoxConverter-0.4.4.dev0/src/singbox_converter/
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-01-04 19:02:23.000000 PySingBoxConverter-0.4.4.dev0/src/singbox_converter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 19:02:32.282881 PySingBoxConverter-0.4.4.dev0/src/singbox_converter/config_template/
--rw-r--r--   0 runner    (1001) docker     (127)    17339 2024-01-04 19:02:23.000000 PySingBoxConverter-0.4.4.dev0/src/singbox_converter/config_template/config_template_groups_rule_set_tun.json
--rw-r--r--   0 runner    (1001) docker     (127)    10635 2024-01-04 19:02:23.000000 PySingBoxConverter-0.4.4.dev0/src/singbox_converter/config_template/config_template_groups_tun.json
--rw-r--r--   0 runner    (1001) docker     (127)    17754 2024-01-04 19:02:23.000000 PySingBoxConverter-0.4.4.dev0/src/singbox_converter/config_template/config_template_groups_v6_rule_set_tun.json
--rw-r--r--   0 runner    (1001) docker     (127)    17867 2024-01-04 19:02:23.000000 PySingBoxConverter-0.4.4.dev0/src/singbox_converter/config_template/config_template_groups_wechat_rule_set_tun.json
--rw-r--r--   0 runner    (1001) docker     (127)     3927 2024-01-04 19:02:23.000000 PySingBoxConverter-0.4.4.dev0/src/singbox_converter/config_template/config_template_no_groups_tun.json
--rw-r--r--   0 runner    (1001) docker     (127)     3141 2024-01-04 19:02:23.000000 PySingBoxConverter-0.4.4.dev0/src/singbox_converter/config_template/config_template_no_groups_tun_VN.json
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-01-04 19:02:23.000000 PySingBoxConverter-0.4.4.dev0/src/singbox_converter/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    35340 2024-01-04 19:02:23.000000 PySingBoxConverter-0.4.4.dev0/src/singbox_converter/core.py
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-01-04 19:02:23.000000 PySingBoxConverter-0.4.4.dev0/src/singbox_converter/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2950 2024-01-04 19:02:23.000000 PySingBoxConverter-0.4.4.dev0/src/singbox_converter/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 19:02:32.286881 PySingBoxConverter-0.4.4.dev0/src/singbox_converter/parsers/
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-01-04 19:02:23.000000 PySingBoxConverter-0.4.4.dev0/src/singbox_converter/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-01-04 19:02:23.000000 PySingBoxConverter-0.4.4.dev0/src/singbox_converter/parsers/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    20553 2024-01-04 19:02:23.000000 PySingBoxConverter-0.4.4.dev0/src/singbox_converter/parsers/clash2base64.py
--rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-01-04 19:02:23.000000 PySingBoxConverter-0.4.4.dev0/src/singbox_converter/parsers/http.py
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-01-04 19:02:23.000000 PySingBoxConverter-0.4.4.dev0/src/singbox_converter/parsers/https.py
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-01-04 19:02:23.000000 PySingBoxConverter-0.4.4.dev0/src/singbox_converter/parsers/hysteria.py
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-01-04 19:02:23.000000 PySingBoxConverter-0.4.4.dev0/src/singbox_converter/parsers/hysteria2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-01-04 19:02:23.000000 PySingBoxConverter-0.4.4.dev0/src/singbox_converter/parsers/socks.py
--rw-r--r--   0 runner    (1001) docker     (127)     7272 2024-01-04 19:02:23.000000 PySingBoxConverter-0.4.4.dev0/src/singbox_converter/parsers/ss.py
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-01-04 19:02:23.000000 PySingBoxConverter-0.4.4.dev0/src/singbox_converter/parsers/ssr.py
--rw-r--r--   0 runner    (1001) docker     (127)     3030 2024-01-04 19:02:23.000000 PySingBoxConverter-0.4.4.dev0/src/singbox_converter/parsers/trojan.py
--rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-01-04 19:02:23.000000 PySingBoxConverter-0.4.4.dev0/src/singbox_converter/parsers/tuic.py
--rw-r--r--   0 runner    (1001) docker     (127)     3992 2024-01-04 19:02:23.000000 PySingBoxConverter-0.4.4.dev0/src/singbox_converter/parsers/vless.py
--rw-r--r--   0 runner    (1001) docker     (127)     5779 2024-01-04 19:02:23.000000 PySingBoxConverter-0.4.4.dev0/src/singbox_converter/parsers/vmess.py
--rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-01-04 19:02:23.000000 PySingBoxConverter-0.4.4.dev0/src/singbox_converter/parsers/wg.py
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-01-04 19:02:23.000000 PySingBoxConverter-0.4.4.dev0/src/singbox_converter/providers-example.json
--rw-r--r--   0 runner    (1001) docker     (127)    12637 2024-01-04 19:02:23.000000 PySingBoxConverter-0.4.4.dev0/src/singbox_converter/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 09:33:34.346853 pysingboxconverter-0.5.0.dev0/
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-12 09:33:20.000000 pysingboxconverter-0.5.0.dev0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-05-12 09:33:34.346853 pysingboxconverter-0.5.0.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-05-12 09:33:20.000000 pysingboxconverter-0.5.0.dev0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-12 09:33:34.346853 pysingboxconverter-0.5.0.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-05-12 09:33:20.000000 pysingboxconverter-0.5.0.dev0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 09:33:34.338853 pysingboxconverter-0.5.0.dev0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 09:33:34.346853 pysingboxconverter-0.5.0.dev0/src/PySingBoxConverter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-05-12 09:33:34.000000 pysingboxconverter-0.5.0.dev0/src/PySingBoxConverter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-05-12 09:33:34.000000 pysingboxconverter-0.5.0.dev0/src/PySingBoxConverter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 09:33:34.000000 pysingboxconverter-0.5.0.dev0/src/PySingBoxConverter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-12 09:33:34.000000 pysingboxconverter-0.5.0.dev0/src/PySingBoxConverter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-12 09:33:34.000000 pysingboxconverter-0.5.0.dev0/src/PySingBoxConverter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-12 09:33:34.000000 pysingboxconverter-0.5.0.dev0/src/PySingBoxConverter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 09:33:34.000000 pysingboxconverter-0.5.0.dev0/src/PySingBoxConverter.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 09:33:34.342853 pysingboxconverter-0.5.0.dev0/src/singbox_converter/
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-12 09:33:20.000000 pysingboxconverter-0.5.0.dev0/src/singbox_converter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 09:33:34.342853 pysingboxconverter-0.5.0.dev0/src/singbox_converter/config_template/
+-rw-r--r--   0 runner    (1001) docker     (127)    17339 2024-05-12 09:33:20.000000 pysingboxconverter-0.5.0.dev0/src/singbox_converter/config_template/config_template_groups_rule_set_tun.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10635 2024-05-12 09:33:20.000000 pysingboxconverter-0.5.0.dev0/src/singbox_converter/config_template/config_template_groups_tun.json
+-rw-r--r--   0 runner    (1001) docker     (127)    17754 2024-05-12 09:33:20.000000 pysingboxconverter-0.5.0.dev0/src/singbox_converter/config_template/config_template_groups_v6_rule_set_tun.json
+-rw-r--r--   0 runner    (1001) docker     (127)    17867 2024-05-12 09:33:20.000000 pysingboxconverter-0.5.0.dev0/src/singbox_converter/config_template/config_template_groups_wechat_rule_set_tun.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3927 2024-05-12 09:33:20.000000 pysingboxconverter-0.5.0.dev0/src/singbox_converter/config_template/config_template_no_groups_tun.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3141 2024-05-12 09:33:20.000000 pysingboxconverter-0.5.0.dev0/src/singbox_converter/config_template/config_template_no_groups_tun_VN.json
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-12 09:33:20.000000 pysingboxconverter-0.5.0.dev0/src/singbox_converter/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36422 2024-05-12 09:33:20.000000 pysingboxconverter-0.5.0.dev0/src/singbox_converter/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-12 09:33:20.000000 pysingboxconverter-0.5.0.dev0/src/singbox_converter/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2950 2024-05-12 09:33:20.000000 pysingboxconverter-0.5.0.dev0/src/singbox_converter/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 09:33:34.346853 pysingboxconverter-0.5.0.dev0/src/singbox_converter/parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-05-12 09:33:20.000000 pysingboxconverter-0.5.0.dev0/src/singbox_converter/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-12 09:33:20.000000 pysingboxconverter-0.5.0.dev0/src/singbox_converter/parsers/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20553 2024-05-12 09:33:20.000000 pysingboxconverter-0.5.0.dev0/src/singbox_converter/parsers/clash2base64.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-05-12 09:33:20.000000 pysingboxconverter-0.5.0.dev0/src/singbox_converter/parsers/http.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-12 09:33:20.000000 pysingboxconverter-0.5.0.dev0/src/singbox_converter/parsers/https.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-05-12 09:33:20.000000 pysingboxconverter-0.5.0.dev0/src/singbox_converter/parsers/hysteria.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-05-12 09:33:20.000000 pysingboxconverter-0.5.0.dev0/src/singbox_converter/parsers/hysteria2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-12 09:33:20.000000 pysingboxconverter-0.5.0.dev0/src/singbox_converter/parsers/socks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7272 2024-05-12 09:33:20.000000 pysingboxconverter-0.5.0.dev0/src/singbox_converter/parsers/ss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-12 09:33:20.000000 pysingboxconverter-0.5.0.dev0/src/singbox_converter/parsers/ssr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3030 2024-05-12 09:33:20.000000 pysingboxconverter-0.5.0.dev0/src/singbox_converter/parsers/trojan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-05-12 09:33:20.000000 pysingboxconverter-0.5.0.dev0/src/singbox_converter/parsers/tuic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3992 2024-05-12 09:33:20.000000 pysingboxconverter-0.5.0.dev0/src/singbox_converter/parsers/vless.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5779 2024-05-12 09:33:20.000000 pysingboxconverter-0.5.0.dev0/src/singbox_converter/parsers/vmess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-05-12 09:33:20.000000 pysingboxconverter-0.5.0.dev0/src/singbox_converter/parsers/wg.py
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-12 09:33:20.000000 pysingboxconverter-0.5.0.dev0/src/singbox_converter/providers-example.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12637 2024-05-12 09:33:20.000000 pysingboxconverter-0.5.0.dev0/src/singbox_converter/tool.py
```

### Comparing `PySingBoxConverter-0.4.4.dev0/PKG-INFO` & `pysingboxconverter-0.5.0.dev0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PySingBoxConverter
-Version: 0.4.4.dev0
+Version: 0.5.0.dev0
 Summary: SingBox converter, Python
 Home-page: 
 Author: 
 Author-email: 
 License: MIT
 Keywords: singbox converter clash subconverter
 Classifier: Development Status :: 3 - Alpha
@@ -33,15 +33,15 @@
 
 ```bash
 pip install PySingBoxConverter
 ```
 
 ## Use in commandline
 
-#### Create a `providers.json` from [`providers-example.json`](https://raw.githubusercontent.com/dzhuang/sing-box-subscribe/main/providers-example.json):
+#### Create a `providers.json` from [`providers-example.json`](https://raw.githubusercontent.com/dzhuang/sing-box-converter/main/src/singbox_converter/providers-example.json):
 
 ```bash
 cp providers-example.json providers.json
 
 vi providers.json
 ```
```

### Comparing `PySingBoxConverter-0.4.4.dev0/README.md` & `pysingboxconverter-0.5.0.dev0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 ```bash
 pip install PySingBoxConverter
 ```
 
 ## Use in commandline
 
-#### Create a `providers.json` from [`providers-example.json`](https://raw.githubusercontent.com/dzhuang/sing-box-subscribe/main/providers-example.json):
+#### Create a `providers.json` from [`providers-example.json`](https://raw.githubusercontent.com/dzhuang/sing-box-converter/main/src/singbox_converter/providers-example.json):
 
 ```bash
 cp providers-example.json providers.json
 
 vi providers.json
 ```
```

### Comparing `PySingBoxConverter-0.4.4.dev0/setup.py` & `pysingboxconverter-0.5.0.dev0/setup.py`

 * *Files identical despite different names*

### Comparing `PySingBoxConverter-0.4.4.dev0/src/PySingBoxConverter.egg-info/PKG-INFO` & `pysingboxconverter-0.5.0.dev0/src/PySingBoxConverter.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PySingBoxConverter
-Version: 0.4.4.dev0
+Version: 0.5.0.dev0
 Summary: SingBox converter, Python
 Home-page: 
 Author: 
 Author-email: 
 License: MIT
 Keywords: singbox converter clash subconverter
 Classifier: Development Status :: 3 - Alpha
@@ -33,15 +33,15 @@
 
 ```bash
 pip install PySingBoxConverter
 ```
 
 ## Use in commandline
 
-#### Create a `providers.json` from [`providers-example.json`](https://raw.githubusercontent.com/dzhuang/sing-box-subscribe/main/providers-example.json):
+#### Create a `providers.json` from [`providers-example.json`](https://raw.githubusercontent.com/dzhuang/sing-box-converter/main/src/singbox_converter/providers-example.json):
 
 ```bash
 cp providers-example.json providers.json
 
 vi providers.json
 ```
```

### Comparing `PySingBoxConverter-0.4.4.dev0/src/PySingBoxConverter.egg-info/SOURCES.txt` & `pysingboxconverter-0.5.0.dev0/src/PySingBoxConverter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PySingBoxConverter-0.4.4.dev0/src/singbox_converter/config_template/config_template_groups_rule_set_tun.json` & `pysingboxconverter-0.5.0.dev0/src/singbox_converter/config_template/config_template_groups_rule_set_tun.json`

 * *Files identical despite different names*

### Comparing `PySingBoxConverter-0.4.4.dev0/src/singbox_converter/config_template/config_template_groups_tun.json` & `pysingboxconverter-0.5.0.dev0/src/singbox_converter/config_template/config_template_groups_tun.json`

 * *Files identical despite different names*

### Comparing `PySingBoxConverter-0.4.4.dev0/src/singbox_converter/config_template/config_template_groups_v6_rule_set_tun.json` & `pysingboxconverter-0.5.0.dev0/src/singbox_converter/config_template/config_template_groups_v6_rule_set_tun.json`

 * *Files identical despite different names*

### Comparing `PySingBoxConverter-0.4.4.dev0/src/singbox_converter/config_template/config_template_groups_wechat_rule_set_tun.json` & `pysingboxconverter-0.5.0.dev0/src/singbox_converter/config_template/config_template_groups_wechat_rule_set_tun.json`

 * *Files identical despite different names*

### Comparing `PySingBoxConverter-0.4.4.dev0/src/singbox_converter/config_template/config_template_no_groups_tun.json` & `pysingboxconverter-0.5.0.dev0/src/singbox_converter/config_template/config_template_no_groups_tun.json`

 * *Files identical despite different names*

### Comparing `PySingBoxConverter-0.4.4.dev0/src/singbox_converter/config_template/config_template_no_groups_tun_VN.json` & `pysingboxconverter-0.5.0.dev0/src/singbox_converter/config_template/config_template_no_groups_tun_VN.json`

 * *Files identical despite different names*

### Comparing `PySingBoxConverter-0.4.4.dev0/src/singbox_converter/core.py` & `pysingboxconverter-0.5.0.dev0/src/singbox_converter/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,19 +64,19 @@
             fetch_sub_fallback_ua=DEFAULT_FALLBACK_UA,
             auto_fix_empty_outbound=True,
             log_level=logging.INFO,
             disable_log=False,
     ):
         """
         :param dict | None providers_config: Configuration for providers. 
-            See example at `providers example <https://raw.githubusercontent.com/dzhuang/sing-box-subscribe/main/providers-example.json>`_.
+            See example at `providers example <https://raw.githubusercontent.com/dzhuang/sing-box-converter/main/providers-example.json>`_.
         :param template: A 0-based integer representing the index of built-in templates 
           (in alphabetical order), a URL of the template, or a file path to the 
           template, or a dict as the template config itself.
-          See available templates at `built-in templates <https://github.com/dzhuang/sing-box-subscribe/tree/package/src/singbox_converter/config_template>`_.
+          See available templates at `built-in templates <https://github.com/dzhuang/sing-box-converter/tree/main/src/singbox_converter/config_template>`_.
         :type template: int, str, dict, or None
         :param bool is_console_mode: Specifies if the instance is running in console mode.
         :param str fetch_sub_ua: The User-Agent string used when fetching 
           subscriptions. Can be overridden by `User-Agent` value in `providers_config`.
         :param str fetch_sub_fallback_ua: The fallback User-Agent used when 
           requests fail with a 403 error.
         :param bool auto_fix_empty_outbound: Whether to automatically remove 
@@ -401,26 +401,52 @@
                                 f"Fetching subscription failed with 503, "
                                 f"with user-agent {self.fetch_sub_ua} and "
                                 f"{self.fetch_sub_fallback_ua}. Please set a valid "
                                 f"fetch_sub_ua or fetch_sub_fallback_ua."
                             )
                 n_retries += 1
 
+    def get_content_from_url(self, subscribe):
+        url = subscribe["url"]
+        user_agent = subscribe.get('User-Agent', self.fetch_sub_ua)
+        response = self.session.get(
+            url, headers={"User-Agent": user_agent}
+        )
+        if response.status_code != 200:
+            raise FailedToFetchSubscription()
+
+        from ruamel.yaml import YAML
+
+        yaml = YAML(typ="safe", pure=True)
+        yaml_data = dict(yaml.load(response.text))
+        return yaml_data
+
     def get_nodes_from_sub(self, subscribe):
         url_or_path = subscribe["url"]
 
         _content = None
 
         if url_or_path.startswith('sub://'):
             url_or_path = b64_decode(url_or_path[6:]).decode('utf-8')
 
-        try:
-            _content = self.get_content_from_file(url_or_path)
-        except Exception:
-            pass
+        if os.path.exists(url_or_path):
+            try:
+                _content = self.get_content_from_file(url_or_path)
+            except Exception as e:
+                self.logger.warning(
+                    f"Failed to load '{url_or_path}' as a subscription file: "
+                    f"{type(e).__name__}: {str(e)}")
+        else:
+            if url_or_path.startswith(('http://', 'https://')):
+                try:
+                    _content = self.get_content_from_url(subscribe)
+                except Exception as e:
+                    self.logger.warning(
+                        f"Failed to load '{url_or_path}' as a subscription url: "
+                        f"{type(e).__name__}: {str(e)}")
 
         if _content is None:
             url_str = urlparse(url_or_path)
             if not url_str.scheme:
                 try:
                     _content = b64_decode(url_or_path).decode('utf-8')
                     data = self.parse_content(_content)
```

### Comparing `PySingBoxConverter-0.4.4.dev0/src/singbox_converter/main.py` & `pysingboxconverter-0.5.0.dev0/src/singbox_converter/main.py`

 * *Files identical despite different names*

### Comparing `PySingBoxConverter-0.4.4.dev0/src/singbox_converter/parsers/__init__.py` & `pysingboxconverter-0.5.0.dev0/src/singbox_converter/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `PySingBoxConverter-0.4.4.dev0/src/singbox_converter/parsers/clash2base64.py` & `pysingboxconverter-0.5.0.dev0/src/singbox_converter/parsers/clash2base64.py`

 * *Files identical despite different names*

### Comparing `PySingBoxConverter-0.4.4.dev0/src/singbox_converter/parsers/http.py` & `pysingboxconverter-0.5.0.dev0/src/singbox_converter/parsers/http.py`

 * *Files identical despite different names*

### Comparing `PySingBoxConverter-0.4.4.dev0/src/singbox_converter/parsers/https.py` & `pysingboxconverter-0.5.0.dev0/src/singbox_converter/parsers/https.py`

 * *Files identical despite different names*

### Comparing `PySingBoxConverter-0.4.4.dev0/src/singbox_converter/parsers/hysteria.py` & `pysingboxconverter-0.5.0.dev0/src/singbox_converter/parsers/hysteria.py`

 * *Files identical despite different names*

### Comparing `PySingBoxConverter-0.4.4.dev0/src/singbox_converter/parsers/hysteria2.py` & `pysingboxconverter-0.5.0.dev0/src/singbox_converter/parsers/hysteria2.py`

 * *Files identical despite different names*

### Comparing `PySingBoxConverter-0.4.4.dev0/src/singbox_converter/parsers/socks.py` & `pysingboxconverter-0.5.0.dev0/src/singbox_converter/parsers/socks.py`

 * *Files identical despite different names*

### Comparing `PySingBoxConverter-0.4.4.dev0/src/singbox_converter/parsers/ss.py` & `pysingboxconverter-0.5.0.dev0/src/singbox_converter/parsers/ss.py`

 * *Files identical despite different names*

### Comparing `PySingBoxConverter-0.4.4.dev0/src/singbox_converter/parsers/ssr.py` & `pysingboxconverter-0.5.0.dev0/src/singbox_converter/parsers/ssr.py`

 * *Files identical despite different names*

### Comparing `PySingBoxConverter-0.4.4.dev0/src/singbox_converter/parsers/trojan.py` & `pysingboxconverter-0.5.0.dev0/src/singbox_converter/parsers/trojan.py`

 * *Files identical despite different names*

### Comparing `PySingBoxConverter-0.4.4.dev0/src/singbox_converter/parsers/tuic.py` & `pysingboxconverter-0.5.0.dev0/src/singbox_converter/parsers/tuic.py`

 * *Files identical despite different names*

### Comparing `PySingBoxConverter-0.4.4.dev0/src/singbox_converter/parsers/vless.py` & `pysingboxconverter-0.5.0.dev0/src/singbox_converter/parsers/vless.py`

 * *Files identical despite different names*

### Comparing `PySingBoxConverter-0.4.4.dev0/src/singbox_converter/parsers/vmess.py` & `pysingboxconverter-0.5.0.dev0/src/singbox_converter/parsers/vmess.py`

 * *Files identical despite different names*

### Comparing `PySingBoxConverter-0.4.4.dev0/src/singbox_converter/parsers/wg.py` & `pysingboxconverter-0.5.0.dev0/src/singbox_converter/parsers/wg.py`

 * *Files identical despite different names*

### Comparing `PySingBoxConverter-0.4.4.dev0/src/singbox_converter/tool.py` & `pysingboxconverter-0.5.0.dev0/src/singbox_converter/tool.py`

 * *Files identical despite different names*

