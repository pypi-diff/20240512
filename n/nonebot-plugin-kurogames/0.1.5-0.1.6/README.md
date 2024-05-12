# Comparing `tmp/nonebot_plugin_kurogames-0.1.5.tar.gz` & `tmp/nonebot_plugin_kurogames-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_kurogames-0.1.5.tar", max compression
+gzip compressed data, was "nonebot_plugin_kurogames-0.1.6.tar", max compression
```

## Comparing `nonebot_plugin_kurogames-0.1.5.tar` & `nonebot_plugin_kurogames-0.1.6.tar`

### file list

```diff
@@ -1,22 +1,23 @@
--rw-r--r--   0        0        0     1062 2024-05-12 02:44:09.324770 nonebot_plugin_kurogames-0.1.5/LICENSE
--rw-r--r--   0        0        0     3019 2024-05-12 02:44:09.324770 nonebot_plugin_kurogames-0.1.5/README.md
--rw-r--r--   0        0        0        0 2024-05-12 02:44:09.324770 nonebot_plugin_kurogames-0.1.5/nonebot_plugin_kurogames/Static/Outputs/rendered_template.html
--rw-r--r--   0        0        0     8272 2024-05-12 02:44:09.324770 nonebot_plugin_kurogames-0.1.5/nonebot_plugin_kurogames/Static/PNSResult.html
--rw-r--r--   0        0        0    36234 2024-05-12 02:44:09.324770 nonebot_plugin_kurogames-0.1.5/nonebot_plugin_kurogames/Static/Pics/ACTIONICON.png
--rw-r--r--   0        0        0    25514 2024-05-12 02:44:09.324770 nonebot_plugin_kurogames-0.1.5/nonebot_plugin_kurogames/Static/Pics/ARENAICON.png
--rw-r--r--   0        0        0    41565 2024-05-12 02:44:09.324770 nonebot_plugin_kurogames-0.1.5/nonebot_plugin_kurogames/Static/Pics/BLACKCARD.png
--rw-r--r--   0        0        0    36944 2024-05-12 02:44:09.324770 nonebot_plugin_kurogames-0.1.5/nonebot_plugin_kurogames/Static/Pics/BOSSICON.png
--rw-r--r--   0        0        0  5682114 2024-05-12 02:44:09.340770 nonebot_plugin_kurogames-0.1.5/nonebot_plugin_kurogames/Static/Pics/LAMIA.png
--rw-r--r--   0        0        0    10716 2024-05-12 02:44:09.340770 nonebot_plugin_kurogames-0.1.5/nonebot_plugin_kurogames/Static/Pics/PNS.png
--rw-r--r--   0        0        0    40106 2024-05-12 02:44:09.340770 nonebot_plugin_kurogames-0.1.5/nonebot_plugin_kurogames/Static/Pics/STRONGHOLDICON.png
--rw-r--r--   0        0        0    39390 2024-05-12 02:44:09.340770 nonebot_plugin_kurogames-0.1.5/nonebot_plugin_kurogames/Static/Pics/TRANSFINITEICON.png
--rw-r--r--   0        0        0     1391 2024-05-12 02:44:09.340770 nonebot_plugin_kurogames-0.1.5/nonebot_plugin_kurogames/__init__.py
--rw-r--r--   0        0        0      498 2024-05-12 02:44:09.340770 nonebot_plugin_kurogames-0.1.5/nonebot_plugin_kurogames/handler/calculate_time_stamp.py
--rw-r--r--   0        0        0     3279 2024-05-12 02:44:09.340770 nonebot_plugin_kurogames-0.1.5/nonebot_plugin_kurogames/handler/pns_dao.py
--rw-r--r--   0        0        0     2982 2024-05-12 02:44:09.340770 nonebot_plugin_kurogames-0.1.5/nonebot_plugin_kurogames/handler/pns_handlers/pns_data_handler.py
--rw-r--r--   0        0        0     3059 2024-05-12 02:44:09.340770 nonebot_plugin_kurogames-0.1.5/nonebot_plugin_kurogames/handler/pns_handlers/pns_detail_handler.py
--rw-r--r--   0        0        0     1725 2024-05-12 02:44:09.340770 nonebot_plugin_kurogames-0.1.5/nonebot_plugin_kurogames/handler/pns_handlers/pns_login_handler.py
--rw-r--r--   0        0        0     2498 2024-05-12 02:44:09.340770 nonebot_plugin_kurogames-0.1.5/nonebot_plugin_kurogames/handler/pns_handlers/pns_pic_render.py
--rw-r--r--   0        0        0      483 2024-05-12 02:44:09.340770 nonebot_plugin_kurogames-0.1.5/nonebot_plugin_kurogames/handler/token_judgement.py
--rw-r--r--   0        0        0      582 2024-05-12 02:44:09.340770 nonebot_plugin_kurogames-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     3938 1970-01-01 00:00:00.000000 nonebot_plugin_kurogames-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1062 2024-05-12 03:59:34.264203 nonebot_plugin_kurogames-0.1.6/LICENSE
+-rw-r--r--   0        0        0     3019 2024-05-12 03:59:34.264203 nonebot_plugin_kurogames-0.1.6/README.md
+-rw-r--r--   0        0        0        0 2024-05-12 03:59:34.264203 nonebot_plugin_kurogames-0.1.6/nonebot_plugin_kurogames/Static/Outputs/rendered_template.html
+-rw-r--r--   0        0        0     8272 2024-05-12 03:59:34.264203 nonebot_plugin_kurogames-0.1.6/nonebot_plugin_kurogames/Static/PNSResult.html
+-rw-r--r--   0        0        0    36234 2024-05-12 03:59:34.264203 nonebot_plugin_kurogames-0.1.6/nonebot_plugin_kurogames/Static/Pics/ACTIONICON.png
+-rw-r--r--   0        0        0    25514 2024-05-12 03:59:34.264203 nonebot_plugin_kurogames-0.1.6/nonebot_plugin_kurogames/Static/Pics/ARENAICON.png
+-rw-r--r--   0        0        0    41565 2024-05-12 03:59:34.264203 nonebot_plugin_kurogames-0.1.6/nonebot_plugin_kurogames/Static/Pics/BLACKCARD.png
+-rw-r--r--   0        0        0    36944 2024-05-12 03:59:34.264203 nonebot_plugin_kurogames-0.1.6/nonebot_plugin_kurogames/Static/Pics/BOSSICON.png
+-rw-r--r--   0        0        0  5682114 2024-05-12 03:59:34.280203 nonebot_plugin_kurogames-0.1.6/nonebot_plugin_kurogames/Static/Pics/LAMIA.png
+-rw-r--r--   0        0        0    10716 2024-05-12 03:59:34.280203 nonebot_plugin_kurogames-0.1.6/nonebot_plugin_kurogames/Static/Pics/PNS.png
+-rw-r--r--   0        0        0    40106 2024-05-12 03:59:34.280203 nonebot_plugin_kurogames-0.1.6/nonebot_plugin_kurogames/Static/Pics/STRONGHOLDICON.png
+-rw-r--r--   0        0        0    39390 2024-05-12 03:59:34.280203 nonebot_plugin_kurogames-0.1.6/nonebot_plugin_kurogames/Static/Pics/TRANSFINITEICON.png
+-rw-r--r--   0        0        0      198 2024-05-12 03:59:34.280203 nonebot_plugin_kurogames-0.1.6/nonebot_plugin_kurogames/Static/kuro_help.py
+-rw-r--r--   0        0        0     1758 2024-05-12 03:59:34.280203 nonebot_plugin_kurogames-0.1.6/nonebot_plugin_kurogames/__init__.py
+-rw-r--r--   0        0        0      498 2024-05-12 03:59:34.280203 nonebot_plugin_kurogames-0.1.6/nonebot_plugin_kurogames/handler/calculate_time_stamp.py
+-rw-r--r--   0        0        0     3279 2024-05-12 03:59:34.280203 nonebot_plugin_kurogames-0.1.6/nonebot_plugin_kurogames/handler/pns_dao.py
+-rw-r--r--   0        0        0     2982 2024-05-12 03:59:34.280203 nonebot_plugin_kurogames-0.1.6/nonebot_plugin_kurogames/handler/pns_handlers/pns_data_handler.py
+-rw-r--r--   0        0        0     3059 2024-05-12 03:59:34.280203 nonebot_plugin_kurogames-0.1.6/nonebot_plugin_kurogames/handler/pns_handlers/pns_detail_handler.py
+-rw-r--r--   0        0        0     1725 2024-05-12 03:59:34.280203 nonebot_plugin_kurogames-0.1.6/nonebot_plugin_kurogames/handler/pns_handlers/pns_login_handler.py
+-rw-r--r--   0        0        0     2498 2024-05-12 03:59:34.280203 nonebot_plugin_kurogames-0.1.6/nonebot_plugin_kurogames/handler/pns_handlers/pns_pic_render.py
+-rw-r--r--   0        0        0      483 2024-05-12 03:59:34.280203 nonebot_plugin_kurogames-0.1.6/nonebot_plugin_kurogames/handler/token_judgement.py
+-rw-r--r--   0        0        0      582 2024-05-12 03:59:34.284203 nonebot_plugin_kurogames-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     3938 1970-01-01 00:00:00.000000 nonebot_plugin_kurogames-0.1.6/PKG-INFO
```

### Comparing `nonebot_plugin_kurogames-0.1.5/LICENSE` & `nonebot_plugin_kurogames-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_kurogames-0.1.5/README.md` & `nonebot_plugin_kurogames-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_kurogames-0.1.5/nonebot_plugin_kurogames/Static/PNSResult.html` & `nonebot_plugin_kurogames-0.1.6/nonebot_plugin_kurogames/Static/PNSResult.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_kurogames-0.1.5/nonebot_plugin_kurogames/Static/Pics/ACTIONICON.png` & `nonebot_plugin_kurogames-0.1.6/nonebot_plugin_kurogames/Static/Pics/ACTIONICON.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_kurogames-0.1.5/nonebot_plugin_kurogames/Static/Pics/ARENAICON.png` & `nonebot_plugin_kurogames-0.1.6/nonebot_plugin_kurogames/Static/Pics/ARENAICON.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_kurogames-0.1.5/nonebot_plugin_kurogames/Static/Pics/BLACKCARD.png` & `nonebot_plugin_kurogames-0.1.6/nonebot_plugin_kurogames/Static/Pics/BLACKCARD.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_kurogames-0.1.5/nonebot_plugin_kurogames/Static/Pics/BOSSICON.png` & `nonebot_plugin_kurogames-0.1.6/nonebot_plugin_kurogames/Static/Pics/BOSSICON.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_kurogames-0.1.5/nonebot_plugin_kurogames/Static/Pics/LAMIA.png` & `nonebot_plugin_kurogames-0.1.6/nonebot_plugin_kurogames/Static/Pics/LAMIA.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_kurogames-0.1.5/nonebot_plugin_kurogames/Static/Pics/PNS.png` & `nonebot_plugin_kurogames-0.1.6/nonebot_plugin_kurogames/Static/Pics/PNS.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_kurogames-0.1.5/nonebot_plugin_kurogames/Static/Pics/STRONGHOLDICON.png` & `nonebot_plugin_kurogames-0.1.6/nonebot_plugin_kurogames/Static/Pics/STRONGHOLDICON.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_kurogames-0.1.5/nonebot_plugin_kurogames/Static/Pics/TRANSFINITEICON.png` & `nonebot_plugin_kurogames-0.1.6/nonebot_plugin_kurogames/Static/Pics/TRANSFINITEICON.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_kurogames-0.1.5/nonebot_plugin_kurogames/__init__.py` & `nonebot_plugin_kurogames-0.1.6/nonebot_plugin_kurogames/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 from nonebot import on_command
 from nonebot.plugin import PluginMetadata
 from nonebot.adapters import Event, Message
 from nonebot.params import CommandArg
 from .handler.pns_handlers.pns_data_handler import pns_data_handler
 from .handler.pns_handlers.pns_login_handler import pns_login_handler, get_kuro_token
 from nonebot.adapters.onebot.v11 import MessageSegment
+from .Static.kuro_help import kuro_help
 
 
-plugin_meta = PluginMetadata(
+__plugin_meta__ = PluginMetadata(
     name="库洛游戏信息",
     description="一款库洛游戏角色信息插件",
-    usage="发送“战双登录”",
+    usage="发送“战双登录”注册，发送“战双”查询战双详情",
     type="application",
     homepage="https://github.com/ConcyWee/nonebot-plugin-kurogames",
     config=None,
     supported_adapters=None
 )
 
 
 punishing = on_command("pns", aliases={"战双","战双详情"}, priority=5)
-pns_login = on_command("pnslogin", aliases={"战双登陆","战双登录"}, priority=5)
+pns_login = on_command("pnslogin", aliases={"战双登陆","战双登录", "库洛登录", "库洛登陆", "鸣潮登录", "鸣潮登陆"}, priority=5)
+pns_help  = on_command("pnshelp", aliases={"战双帮助", "库洛帮助", "鸣潮帮助"}, priority=5)
 
 
 @pns_login.handle()
 async def _(event: Event, arg: Message = CommandArg()):
     user_id = event.get_user_id()
     data_content = arg.extract_plain_text()
     result = pns_login_handler(user_id, data_content)
@@ -33,8 +35,13 @@
 async def _(event: Event):
     user_id = event.get_user_id()
     data_row = get_kuro_token(user_id)
     if data_row:
         pic_result = await pns_data_handler(data_row)
         await punishing.finish(MessageSegment.image(pic_result))
     else:
-        await punishing.finish("请先输入token")
+        await punishing.finish("请先输入token")
+
+@pns_help.handle()
+async def _():
+    help_datail = await kuro_help()
+    await pns_help.finish(help_datail)
```

### Comparing `nonebot_plugin_kurogames-0.1.5/nonebot_plugin_kurogames/handler/pns_dao.py` & `nonebot_plugin_kurogames-0.1.6/nonebot_plugin_kurogames/handler/pns_dao.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_kurogames-0.1.5/nonebot_plugin_kurogames/handler/pns_handlers/pns_data_handler.py` & `nonebot_plugin_kurogames-0.1.6/nonebot_plugin_kurogames/handler/pns_handlers/pns_data_handler.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_kurogames-0.1.5/nonebot_plugin_kurogames/handler/pns_handlers/pns_detail_handler.py` & `nonebot_plugin_kurogames-0.1.6/nonebot_plugin_kurogames/handler/pns_handlers/pns_detail_handler.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_kurogames-0.1.5/nonebot_plugin_kurogames/handler/pns_handlers/pns_login_handler.py` & `nonebot_plugin_kurogames-0.1.6/nonebot_plugin_kurogames/handler/pns_handlers/pns_login_handler.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_kurogames-0.1.5/nonebot_plugin_kurogames/handler/pns_handlers/pns_pic_render.py` & `nonebot_plugin_kurogames-0.1.6/nonebot_plugin_kurogames/handler/pns_handlers/pns_pic_render.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_kurogames-0.1.5/pyproject.toml` & `nonebot_plugin_kurogames-0.1.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-kurogames"
-version = "0.1.5"
+version = "0.1.6"
 description = "库洛游戏数据详情 谢比螺六~"
 authors = ["ConcyWee <concywee@163.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/ConcyWee/nonebot-plugin-kurogames"
 repository = "https://github.com/ConcyWee/nonebot-plugin-kurogames"
```

### Comparing `nonebot_plugin_kurogames-0.1.5/PKG-INFO` & `nonebot_plugin_kurogames-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-kurogames
-Version: 0.1.5
+Version: 0.1.6
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
-Metadata-Version: 2.1 Name: nonebot-plugin-kurogames Version: 0.1.5 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-kurogames Version: 0.1.6 Summary:
 åºæ´æ¸¸ææ°æ®è¯¦æ è°¢æ¯èºå­~ Home-page: https://github.com/ConcyWee/
 nonebot-plugin-kurogames License: MIT Author: ConcyWee Author-email:
 concywee@163.com Requires-Python: >=3.8 Classifier: License :: OSI Approved ::
 MIT License Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
```

