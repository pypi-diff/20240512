# Comparing `tmp/wxhelper-0.0.1.tar.gz` & `tmp/wxhelper-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wxhelper-0.0.1.tar", last modified: Sat May 11 10:07:10 2024, max compression
+gzip compressed data, was "wxhelper-0.0.2.tar", last modified: Sun May 12 05:53:57 2024, max compression
```

## Comparing `wxhelper-0.0.1.tar` & `wxhelper-0.0.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-05-11 10:07:10.199904 wxhelper-0.0.1/
--rw-rw-rw-   0        0        0     1077 2024-05-06 06:49:40.000000 wxhelper-0.0.1/LICENSE
--rw-rw-rw-   0        0        0       53 2024-05-11 10:04:00.000000 wxhelper-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     3510 2024-05-11 10:07:10.199904 wxhelper-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2878 2024-05-11 10:03:16.000000 wxhelper-0.0.1/README.md
--rw-rw-rw-   0        0        0       42 2024-05-11 10:07:10.199904 wxhelper-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     3932 2024-05-11 10:06:57.000000 wxhelper-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-11 10:07:10.188897 wxhelper-0.0.1/wxhelper/
--rw-rw-rw-   0        0        0       44 2024-05-11 09:54:16.000000 wxhelper-0.0.1/wxhelper/__init__.py
--rw-rw-rw-   0        0        0    20285 2024-05-11 09:54:16.000000 wxhelper-0.0.1/wxhelper/core.py
--rw-rw-rw-   0        0        0      630 2024-05-06 06:49:40.000000 wxhelper-0.0.1/wxhelper/events.py
--rw-rw-rw-   0        0        0      314 2024-05-11 09:43:59.000000 wxhelper-0.0.1/wxhelper/logger.py
--rw-rw-rw-   0        0        0     2918 2024-05-11 09:48:05.000000 wxhelper-0.0.1/wxhelper/model.py
-drwxrwxrwx   0        0        0        0 2024-05-11 10:07:10.197902 wxhelper-0.0.1/wxhelper/tools/
--rwxrwxrwx   0        0        0   270336 2024-05-06 06:49:40.000000 wxhelper-0.0.1/wxhelper/tools/faker.exe
--rwxrwxrwx   0        0        0   884736 2024-05-11 03:43:40.000000 wxhelper-0.0.1/wxhelper/tools/start-wechat.exe
--rw-rw-rw-   0        0        0   489984 2024-04-13 13:17:52.000000 wxhelper-0.0.1/wxhelper/tools/wxhelper.dll
--rw-rw-rw-   0        0        0     3789 2024-05-11 03:58:06.000000 wxhelper-0.0.1/wxhelper/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-11 10:07:10.192900 wxhelper-0.0.1/wxhelper.egg-info/
--rw-rw-rw-   0        0        0     3510 2024-05-11 10:07:10.000000 wxhelper-0.0.1/wxhelper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      394 2024-05-11 10:07:10.000000 wxhelper-0.0.1/wxhelper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-11 10:07:10.000000 wxhelper-0.0.1/wxhelper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2024-05-11 10:07:10.000000 wxhelper-0.0.1/wxhelper.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-11 10:07:10.000000 wxhelper-0.0.1/wxhelper.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-12 05:53:57.254561 wxhelper-0.0.2/
+-rw-rw-rw-   0        0        0     1077 2024-05-12 03:43:34.000000 wxhelper-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0       53 2024-05-12 03:43:34.000000 wxhelper-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     3628 2024-05-12 05:53:57.253090 wxhelper-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2880 2024-05-12 03:43:35.000000 wxhelper-0.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-12 05:53:57.254561 wxhelper-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     3932 2024-05-12 05:49:21.000000 wxhelper-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-12 05:53:57.236424 wxhelper-0.0.2/wxhelper/
+-rw-rw-rw-   0        0        0       44 2024-05-12 05:49:21.000000 wxhelper-0.0.2/wxhelper/__init__.py
+-rw-rw-rw-   0        0        0    20724 2024-05-12 05:49:21.000000 wxhelper-0.0.2/wxhelper/core.py
+-rw-rw-rw-   0        0        0      630 2024-05-12 03:43:35.000000 wxhelper-0.0.2/wxhelper/events.py
+-rw-rw-rw-   0        0        0      314 2024-05-12 03:43:35.000000 wxhelper-0.0.2/wxhelper/logger.py
+-rw-rw-rw-   0        0        0     2693 2024-05-12 04:58:55.000000 wxhelper-0.0.2/wxhelper/model.py
+drwxrwxrwx   0        0        0        0 2024-05-12 05:53:57.250271 wxhelper-0.0.2/wxhelper/tools/
+-rwxrwxrwx   0        0        0   270336 2024-05-12 03:43:35.000000 wxhelper-0.0.2/wxhelper/tools/faker.exe
+-rwxrwxrwx   0        0        0   884736 2024-05-12 05:45:22.000000 wxhelper-0.0.2/wxhelper/tools/start-wechat.exe
+-rw-rw-rw-   0        0        0   489984 2024-05-12 03:43:35.000000 wxhelper-0.0.2/wxhelper/tools/wxhelper.dll
+-rw-rw-rw-   0        0        0     3789 2024-05-12 03:43:35.000000 wxhelper-0.0.2/wxhelper/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-12 05:53:57.244961 wxhelper-0.0.2/wxhelper.egg-info/
+-rw-rw-rw-   0        0        0     3628 2024-05-12 05:53:57.000000 wxhelper-0.0.2/wxhelper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      394 2024-05-12 05:53:57.000000 wxhelper-0.0.2/wxhelper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-12 05:53:57.000000 wxhelper-0.0.2/wxhelper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2024-05-12 05:53:57.000000 wxhelper-0.0.2/wxhelper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-12 05:53:57.000000 wxhelper-0.0.2/wxhelper.egg-info/top_level.txt
```

### Comparing `wxhelper-0.0.1/LICENSE` & `wxhelper-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wxhelper-0.0.1/PKG-INFO` & `wxhelper-0.0.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 Metadata-Version: 2.1
 Name: wxhelper
-Version: 0.0.1
+Version: 0.0.2
 Summary: wechat robot framework.
 Home-page: https://github.com/miloira/wxhelper
 Author: Msky
 Author-email: 690126048@qq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: loguru
+Requires-Dist: psutil
+Requires-Dist: pyee
+Requires-Dist: requests
+Requires-Dist: xmltodict
 
 
 # WxHelper
 
 ## 简介
 
 WxHelper是一个基于dll注入实现的python微信机器人框架，支持多种接口、高扩展性、多线程消息处理，让你轻松应对海量消息，为你的需求实现提供便捷灵活的支持。
@@ -28,15 +33,15 @@
 2. 取消消息回调
 3. hook日志
 4. 取消hook日志
 5. 检查登录状态
 6. 登录用户信息
 7. 发送文本消息
 8. 发送图片消息
-9. 发送图片消息
+9. 发送文件消息
 10. 发送群at消息
 11. 发送app消息
 12. 发送拍一拍消息
 13. 转发消息
 14. 转发公众号消息
 15. 转发公众号消息通过svrid
 16. 撤回消息
```

### Comparing `wxhelper-0.0.1/README.md` & `wxhelper-0.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 2. 取消消息回调
 3. hook日志
 4. 取消hook日志
 5. 检查登录状态
 6. 登录用户信息
 7. 发送文本消息
 8. 发送图片消息
-9. 发送图片消息
+9. 发送文件消息
 10. 发送群at消息
 11. 发送app消息
 12. 发送拍一拍消息
 13. 转发消息
 14. 转发公众号消息
 15. 转发公众号消息通过svrid
 16. 撤回消息
@@ -110,8 +110,8 @@
 
 bot.run()
 ```
 QQ交流群:625920216
 
 ## 感谢项目
 
-https://github.com/ttttupup/wxhelper
+https://github.com/ttttupup/wxhelper
```

### Comparing `wxhelper-0.0.1/setup.py` & `wxhelper-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'wxhelper'
 DESCRIPTION = 'wechat robot framework.'
 URL = 'https://github.com/miloira/wxhelper'
 EMAIL = '690126048@qq.com'
 AUTHOR = 'Msky'
 REQUIRES_PYTHON = '>=3.8.0'
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     'loguru',
     'psutil',
     'pyee',
     'requests',
```

### Comparing `wxhelper-0.0.1/wxhelper/core.py` & `wxhelper-0.0.2/wxhelper/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,14 +100,15 @@
     def init_bot(self, bot: "Bot", event: Event) -> None:
         self.DATA_SAVE_PATH = bot.info.dataSavePath
         self.WXHELPER_PATH = os.path.join(self.DATA_SAVE_PATH, "wxhelper")
         self.FILE_SAVE_PATH = os.path.join(self.WXHELPER_PATH, "file")
         self.IMAGE_SAVE_PATH = os.path.join(self.WXHELPER_PATH, "image")
         self.VIDEO_SAVE_PATH = os.path.join(self.WXHELPER_PATH, "video")
         self.call_hook_func(self.on_login, bot, event)
+        logger.info(f"login success, {bot.info}")
 
     def set_webhook_url(self, webhook_url: str) -> None:
         self.webhook_url = webhook_url
 
     def webhook(self, event: dict) -> None:
         if self.webhook_url is not None:
             try:
@@ -197,32 +198,32 @@
         data = {
             "wxid": wxid,
             "imagePath": os.path.abspath(image_path)
         }
         return Response(**self.call_api(params=params, json=data))
 
     def send_file(self, wxid: str, file_path: str) -> Response:
-        """发送图片消息"""
+        """发送文件消息"""
         params = {
             "type": "6"
         }
         data = {
             "wxid": wxid,
             "filePath": os.path.abspath(file_path)
         }
         return Response(**self.call_api(params=params, json=data))
 
-    def send_room_at(self, room_id: str, wxids: str, msg: str) -> Response:
+    def send_room_at(self, room_id: str, wxids: list[str], msg: str) -> Response:
         """发送群at消息"""
         params = {
             "type": "3"
         }
         data = {
             "chatRoomId": room_id,
-            "wxids": wxids,
+            "wxids": ",".join(wxids),
             "msg": msg
         }
         return Response(**self.call_api(params=params, json=data))
 
     def send_app(self, wxid: str, applet_id: str) -> Response:
         """发送app消息"""
         params = {
@@ -299,15 +300,14 @@
             "type": "61"
         }
         data = {
             "msgId": msg_id
         }
         return Response(**self.call_api(params=params, json=data))
 
-
     def get_contacts(self) -> typing.List[Contact]:
         """获取好友列表"""
         params = {
             "type": "46"
         }
         return [Contact(**item) for item in self.call_api(params=params)["data"]]
 
@@ -471,14 +471,26 @@
         }
         data = {
             "wxid": wxid,
             "msg": msg
         }
         return Response(**self.call_api(params=params, json=data))
 
+    def verify_apply(self, v3: str, v4: str, permission: int) -> Response:
+        """验证好友请求"""
+        params = {
+            "type": "23"
+        }
+        data = {
+            "v3": v3,
+            "v4": v4,
+            "permission": permission
+        }
+        return Response(**self.call_api(params=params, json=data))
+
     def get_db_info(self) -> typing.List[DB]:
         """获取数据库句柄"""
         params = {
             "type": "32"
         }
         return [
             DB(databaseName=item["databaseName"], handle=item["handle"], tables=[
@@ -610,16 +622,19 @@
             self.event_emitter.emit(str(event.type), self, event)
             self.call_hook_func(self.on_after_message, self, event)
             self.webhook(data)
         except Exception:
             logger.error(traceback.format_exc())
             logger.error(raw_data)
 
-    def handle(self, events: typing.Union[typing.List[str], str, None] = None, once: bool = False) -> typing.Callable[
-        [typing.Callable], None]:
+    def handle(
+        self,
+        events: typing.Union[typing.List[str], str, None] = None,
+        once: bool = False
+    ) -> typing.Callable[[typing.Callable], None]:
         def wrapper(func):
             listen = self.event_emitter.on if not once else self.event_emitter.once
             if not events:
                 listen(str(ALL_MESSAGE), func)
             else:
                 for event in events if isinstance(events, list) else [events]:
                     listen(str(event), func)
```

### Comparing `wxhelper-0.0.1/wxhelper/events.py` & `wxhelper-0.0.2/wxhelper/events.py`

 * *Files identical despite different names*

### Comparing `wxhelper-0.0.1/wxhelper/model.py` & `wxhelper-0.0.2/wxhelper/model.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,32 @@
 import typing
 from dataclasses import dataclass
 from typing import List
 
 
 @dataclass
+class Event:
+    """消息事件"""
+    content: typing.Optional[typing.Any] = None
+    fromGroup: typing.Optional[str] = None
+    fromUser: typing.Optional[str] = None
+    isSendByPhone: typing.Optional[int] = None
+    isSendMsg: typing.Optional[int] = None
+    msgId: typing.Optional[int] = None
+    path: typing.Optional[str] = None
+    thumbPath: typing.Optional[str] = None
+    pid: typing.Optional[int] = None
+    sign: typing.Optional[str] = None
+    signature: typing.Optional[str] = None
+    time: typing.Optional[str] = None
+    timestamp: typing.Optional[int] = None
+    type: typing.Optional[int] = None
+
+
+@dataclass
 class Account:
     """用户"""
     account: str
     city: str
     country: str
     currentDataPath: str
     dataSavePath: str
@@ -61,38 +80,14 @@
     """群成员"""
     admin: str
     chatRoomId: str
     members: str
 
 
 @dataclass
-class Event:
-    """消息事件"""
-    content: typing.Optional[typing.Any] = None
-    base64Img: typing.Optional[str] = None
-    data: typing.Optional[list] = None
-    createTime: typing.Optional[int] = None
-    displayFullContent: typing.Optional[str] = None
-    fromGroup: typing.Optional[str] = None
-    fromUser: typing.Optional[str] = None
-    isSendByPhone: typing.Optional[int] = None
-    isSendMsg: typing.Optional[int] = None
-    msgId: typing.Optional[int] = None
-    path: typing.Optional[str] = None
-    msgSequence: typing.Optional[int] = None
-    pid: typing.Optional[int] = None
-    sign: typing.Optional[str] = None
-    signature: typing.Optional[str] = None
-    toUser: typing.Optional[str] = None
-    time: typing.Optional[str] = None
-    timestamp: typing.Optional[int] = None
-    type: typing.Optional[int] = None
-
-
-@dataclass
 class Table:
     """表结构"""
     name: str
     rootpage: str
     sql: str
     tableName: str
```

### Comparing `wxhelper-0.0.1/wxhelper/tools/faker.exe` & `wxhelper-0.0.2/wxhelper/tools/faker.exe`

 * *Files identical despite different names*

### Comparing `wxhelper-0.0.1/wxhelper/tools/start-wechat.exe` & `wxhelper-0.0.2/wxhelper/tools/start-wechat.exe`

 * *Files identical despite different names*

### Comparing `wxhelper-0.0.1/wxhelper/tools/wxhelper.dll` & `wxhelper-0.0.2/wxhelper/tools/wxhelper.dll`

 * *Files identical despite different names*

### Comparing `wxhelper-0.0.1/wxhelper/utils.py` & `wxhelper-0.0.2/wxhelper/utils.py`

 * *Files identical despite different names*

### Comparing `wxhelper-0.0.1/wxhelper.egg-info/PKG-INFO` & `wxhelper-0.0.2/wxhelper.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 Metadata-Version: 2.1
 Name: wxhelper
-Version: 0.0.1
+Version: 0.0.2
 Summary: wechat robot framework.
 Home-page: https://github.com/miloira/wxhelper
 Author: Msky
 Author-email: 690126048@qq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: loguru
+Requires-Dist: psutil
+Requires-Dist: pyee
+Requires-Dist: requests
+Requires-Dist: xmltodict
 
 
 # WxHelper
 
 ## 简介
 
 WxHelper是一个基于dll注入实现的python微信机器人框架，支持多种接口、高扩展性、多线程消息处理，让你轻松应对海量消息，为你的需求实现提供便捷灵活的支持。
@@ -28,15 +33,15 @@
 2. 取消消息回调
 3. hook日志
 4. 取消hook日志
 5. 检查登录状态
 6. 登录用户信息
 7. 发送文本消息
 8. 发送图片消息
-9. 发送图片消息
+9. 发送文件消息
 10. 发送群at消息
 11. 发送app消息
 12. 发送拍一拍消息
 13. 转发消息
 14. 转发公众号消息
 15. 转发公众号消息通过svrid
 16. 撤回消息
```

