# Comparing `tmp/nonebot_plugin_kurogames-0.1.3.tar.gz` & `tmp/nonebot_plugin_kurogames-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_kurogames-0.1.3.tar", max compression
+gzip compressed data, was "nonebot_plugin_kurogames-0.1.4.tar", max compression
```

## Comparing `nonebot_plugin_kurogames-0.1.3.tar` & `nonebot_plugin_kurogames-0.1.4.tar`

### file list

```diff
@@ -1,21 +1,22 @@
--rw-r--r--   0        0        0     1062 2024-05-11 12:56:28.167262 nonebot_plugin_kurogames-0.1.3/LICENSE
--rw-r--r--   0        0        0     2823 2024-05-11 12:56:28.171262 nonebot_plugin_kurogames-0.1.3/README.md
--rw-r--r--   0        0        0     8272 2024-05-11 12:56:28.171262 nonebot_plugin_kurogames-0.1.3/nonebot_plugin_kurogames/Static/PNSResult.html
--rw-r--r--   0        0        0    36234 2024-05-11 12:56:28.171262 nonebot_plugin_kurogames-0.1.3/nonebot_plugin_kurogames/Static/Pics/ACTIONICON.png
--rw-r--r--   0        0        0    25514 2024-05-11 12:56:28.171262 nonebot_plugin_kurogames-0.1.3/nonebot_plugin_kurogames/Static/Pics/ARENAICON.png
--rw-r--r--   0        0        0    41565 2024-05-11 12:56:28.171262 nonebot_plugin_kurogames-0.1.3/nonebot_plugin_kurogames/Static/Pics/BLACKCARD.png
--rw-r--r--   0        0        0    36944 2024-05-11 12:56:28.171262 nonebot_plugin_kurogames-0.1.3/nonebot_plugin_kurogames/Static/Pics/BOSSICON.png
--rw-r--r--   0        0        0  5682114 2024-05-11 12:56:28.187262 nonebot_plugin_kurogames-0.1.3/nonebot_plugin_kurogames/Static/Pics/LAMIA.png
--rw-r--r--   0        0        0    10716 2024-05-11 12:56:28.187262 nonebot_plugin_kurogames-0.1.3/nonebot_plugin_kurogames/Static/Pics/PNS.png
--rw-r--r--   0        0        0    40106 2024-05-11 12:56:28.187262 nonebot_plugin_kurogames-0.1.3/nonebot_plugin_kurogames/Static/Pics/STRONGHOLDICON.png
--rw-r--r--   0        0        0    39390 2024-05-11 12:56:28.187262 nonebot_plugin_kurogames-0.1.3/nonebot_plugin_kurogames/Static/Pics/TRANSFINITEICON.png
--rw-r--r--   0        0        0     1391 2024-05-11 12:56:28.187262 nonebot_plugin_kurogames-0.1.3/nonebot_plugin_kurogames/__init__.py
--rw-r--r--   0        0        0      498 2024-05-11 12:56:28.187262 nonebot_plugin_kurogames-0.1.3/nonebot_plugin_kurogames/handler/calculate_time_stamp.py
--rw-r--r--   0        0        0     3279 2024-05-11 12:56:28.187262 nonebot_plugin_kurogames-0.1.3/nonebot_plugin_kurogames/handler/pns_dao.py
--rw-r--r--   0        0        0     2982 2024-05-11 12:56:28.187262 nonebot_plugin_kurogames-0.1.3/nonebot_plugin_kurogames/handler/pns_handlers/pns_data_handler.py
--rw-r--r--   0        0        0     3059 2024-05-11 12:56:28.187262 nonebot_plugin_kurogames-0.1.3/nonebot_plugin_kurogames/handler/pns_handlers/pns_detail_handler.py
--rw-r--r--   0        0        0     1725 2024-05-11 12:56:28.187262 nonebot_plugin_kurogames-0.1.3/nonebot_plugin_kurogames/handler/pns_handlers/pns_login_handler.py
--rw-r--r--   0        0        0     2498 2024-05-11 12:56:28.187262 nonebot_plugin_kurogames-0.1.3/nonebot_plugin_kurogames/handler/pns_handlers/pns_pic_render.py
--rw-r--r--   0        0        0      483 2024-05-11 12:56:28.187262 nonebot_plugin_kurogames-0.1.3/nonebot_plugin_kurogames/handler/token_judgement.py
--rw-r--r--   0        0        0      558 2024-05-11 12:56:28.187262 nonebot_plugin_kurogames-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     3705 1970-01-01 00:00:00.000000 nonebot_plugin_kurogames-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1062 2024-05-11 13:22:18.454563 nonebot_plugin_kurogames-0.1.4/LICENSE
+-rw-r--r--   0        0        0     2823 2024-05-11 13:22:18.454563 nonebot_plugin_kurogames-0.1.4/README.md
+-rw-r--r--   0        0        0        0 2024-05-11 13:22:18.454563 nonebot_plugin_kurogames-0.1.4/nonebot_plugin_kurogames/Static/Outputs/rendered_template.html
+-rw-r--r--   0        0        0     8272 2024-05-11 13:22:18.454563 nonebot_plugin_kurogames-0.1.4/nonebot_plugin_kurogames/Static/PNSResult.html
+-rw-r--r--   0        0        0    36234 2024-05-11 13:22:18.454563 nonebot_plugin_kurogames-0.1.4/nonebot_plugin_kurogames/Static/Pics/ACTIONICON.png
+-rw-r--r--   0        0        0    25514 2024-05-11 13:22:18.454563 nonebot_plugin_kurogames-0.1.4/nonebot_plugin_kurogames/Static/Pics/ARENAICON.png
+-rw-r--r--   0        0        0    41565 2024-05-11 13:22:18.454563 nonebot_plugin_kurogames-0.1.4/nonebot_plugin_kurogames/Static/Pics/BLACKCARD.png
+-rw-r--r--   0        0        0    36944 2024-05-11 13:22:18.454563 nonebot_plugin_kurogames-0.1.4/nonebot_plugin_kurogames/Static/Pics/BOSSICON.png
+-rw-r--r--   0        0        0  5682114 2024-05-11 13:22:18.470563 nonebot_plugin_kurogames-0.1.4/nonebot_plugin_kurogames/Static/Pics/LAMIA.png
+-rw-r--r--   0        0        0    10716 2024-05-11 13:22:18.470563 nonebot_plugin_kurogames-0.1.4/nonebot_plugin_kurogames/Static/Pics/PNS.png
+-rw-r--r--   0        0        0    40106 2024-05-11 13:22:18.470563 nonebot_plugin_kurogames-0.1.4/nonebot_plugin_kurogames/Static/Pics/STRONGHOLDICON.png
+-rw-r--r--   0        0        0    39390 2024-05-11 13:22:18.470563 nonebot_plugin_kurogames-0.1.4/nonebot_plugin_kurogames/Static/Pics/TRANSFINITEICON.png
+-rw-r--r--   0        0        0     1391 2024-05-11 13:22:18.470563 nonebot_plugin_kurogames-0.1.4/nonebot_plugin_kurogames/__init__.py
+-rw-r--r--   0        0        0      498 2024-05-11 13:22:18.470563 nonebot_plugin_kurogames-0.1.4/nonebot_plugin_kurogames/handler/calculate_time_stamp.py
+-rw-r--r--   0        0        0     3279 2024-05-11 13:22:18.470563 nonebot_plugin_kurogames-0.1.4/nonebot_plugin_kurogames/handler/pns_dao.py
+-rw-r--r--   0        0        0     2982 2024-05-11 13:22:18.470563 nonebot_plugin_kurogames-0.1.4/nonebot_plugin_kurogames/handler/pns_handlers/pns_data_handler.py
+-rw-r--r--   0        0        0     3059 2024-05-11 13:22:18.470563 nonebot_plugin_kurogames-0.1.4/nonebot_plugin_kurogames/handler/pns_handlers/pns_detail_handler.py
+-rw-r--r--   0        0        0     1725 2024-05-11 13:22:18.470563 nonebot_plugin_kurogames-0.1.4/nonebot_plugin_kurogames/handler/pns_handlers/pns_login_handler.py
+-rw-r--r--   0        0        0     2498 2024-05-11 13:22:18.470563 nonebot_plugin_kurogames-0.1.4/nonebot_plugin_kurogames/handler/pns_handlers/pns_pic_render.py
+-rw-r--r--   0        0        0      483 2024-05-11 13:22:18.470563 nonebot_plugin_kurogames-0.1.4/nonebot_plugin_kurogames/handler/token_judgement.py
+-rw-r--r--   0        0        0      558 2024-05-11 13:22:18.470563 nonebot_plugin_kurogames-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     3705 1970-01-01 00:00:00.000000 nonebot_plugin_kurogames-0.1.4/PKG-INFO
```

### Comparing `nonebot_plugin_kurogames-0.1.3/LICENSE` & `nonebot_plugin_kurogames-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_kurogames-0.1.3/README.md` & `nonebot_plugin_kurogames-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_kurogames-0.1.3/nonebot_plugin_kurogames/Static/PNSResult.html` & `nonebot_plugin_kurogames-0.1.4/nonebot_plugin_kurogames/Static/PNSResult.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_kurogames-0.1.3/nonebot_plugin_kurogames/Static/Pics/ACTIONICON.png` & `nonebot_plugin_kurogames-0.1.4/nonebot_plugin_kurogames/Static/Pics/ACTIONICON.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_kurogames-0.1.3/nonebot_plugin_kurogames/Static/Pics/ARENAICON.png` & `nonebot_plugin_kurogames-0.1.4/nonebot_plugin_kurogames/Static/Pics/ARENAICON.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_kurogames-0.1.3/nonebot_plugin_kurogames/Static/Pics/BLACKCARD.png` & `nonebot_plugin_kurogames-0.1.4/nonebot_plugin_kurogames/Static/Pics/BLACKCARD.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_kurogames-0.1.3/nonebot_plugin_kurogames/Static/Pics/BOSSICON.png` & `nonebot_plugin_kurogames-0.1.4/nonebot_plugin_kurogames/Static/Pics/BOSSICON.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_kurogames-0.1.3/nonebot_plugin_kurogames/Static/Pics/LAMIA.png` & `nonebot_plugin_kurogames-0.1.4/nonebot_plugin_kurogames/Static/Pics/LAMIA.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_kurogames-0.1.3/nonebot_plugin_kurogames/Static/Pics/PNS.png` & `nonebot_plugin_kurogames-0.1.4/nonebot_plugin_kurogames/Static/Pics/PNS.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_kurogames-0.1.3/nonebot_plugin_kurogames/Static/Pics/STRONGHOLDICON.png` & `nonebot_plugin_kurogames-0.1.4/nonebot_plugin_kurogames/Static/Pics/STRONGHOLDICON.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_kurogames-0.1.3/nonebot_plugin_kurogames/Static/Pics/TRANSFINITEICON.png` & `nonebot_plugin_kurogames-0.1.4/nonebot_plugin_kurogames/Static/Pics/TRANSFINITEICON.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_kurogames-0.1.3/nonebot_plugin_kurogames/__init__.py` & `nonebot_plugin_kurogames-0.1.4/nonebot_plugin_kurogames/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_kurogames-0.1.3/nonebot_plugin_kurogames/handler/pns_dao.py` & `nonebot_plugin_kurogames-0.1.4/nonebot_plugin_kurogames/handler/pns_dao.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_kurogames-0.1.3/nonebot_plugin_kurogames/handler/pns_handlers/pns_data_handler.py` & `nonebot_plugin_kurogames-0.1.4/nonebot_plugin_kurogames/handler/pns_handlers/pns_data_handler.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_kurogames-0.1.3/nonebot_plugin_kurogames/handler/pns_handlers/pns_detail_handler.py` & `nonebot_plugin_kurogames-0.1.4/nonebot_plugin_kurogames/handler/pns_handlers/pns_detail_handler.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_kurogames-0.1.3/nonebot_plugin_kurogames/handler/pns_handlers/pns_login_handler.py` & `nonebot_plugin_kurogames-0.1.4/nonebot_plugin_kurogames/handler/pns_handlers/pns_login_handler.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_kurogames-0.1.3/nonebot_plugin_kurogames/handler/pns_handlers/pns_pic_render.py` & `nonebot_plugin_kurogames-0.1.4/nonebot_plugin_kurogames/handler/pns_handlers/pns_pic_render.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_kurogames-0.1.3/pyproject.toml` & `nonebot_plugin_kurogames-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-kurogames"
-version = "0.1.3"
+version = "0.1.4"
 description = "库洛游戏数据详情 谢比螺六~"
 authors = ["ConcyWee <concywee@163.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/ConcyWee/nonebot-plugin-kurogames"
 repository = "https://github.com/ConcyWee/nonebot-plugin-kurogames"
```

### Comparing `nonebot_plugin_kurogames-0.1.3/PKG-INFO` & `nonebot_plugin_kurogames-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-kurogames
-Version: 0.1.3
+Version: 0.1.4
 Summary: 库洛游戏数据详情 谢比螺六~
 Home-page: https://github.com/ConcyWee/nonebot-plugin-kurogames
 License: MIT
 Author: ConcyWee
 Author-email: concywee@163.com
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-kurogames Version: 0.1.3 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-kurogames Version: 0.1.4 Summary:
 åºæ´æ¸¸ææ°æ®è¯¦æ è°¢æ¯èºå­~ Home-page: https://github.com/ConcyWee/
 nonebot-plugin-kurogames License: MIT Author: ConcyWee Author-email:
 concywee@163.com Requires-Python: >=3.8 Classifier: License :: OSI Approved ::
 MIT License Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
```

