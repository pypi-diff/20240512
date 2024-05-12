# Comparing `tmp/nonebot_adapter_kritor-0.1.1.tar.gz` & `tmp/nonebot_adapter_kritor-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_adapter_kritor-0.1.1.tar", last modified: Mon Apr 22 09:08:15 2024, max compression
+gzip compressed data, was "nonebot_adapter_kritor-0.2.0.tar", last modified: Sun May 12 06:19:34 2024, max compression
```

## Comparing `nonebot_adapter_kritor-0.1.1.tar` & `nonebot_adapter_kritor-0.2.0.tar`

### file list

```diff
@@ -1,31 +1,32 @@
--rw-r--r--   0        0        0     1064 2024-04-22 09:07:47.013935 nonebot_adapter_kritor-0.1.1/LICENSE
--rw-r--r--   0        0        0     1042 2024-04-22 09:07:47.013935 nonebot_adapter_kritor-0.1.1/README.md
--rw-r--r--   0        0        0     2262 2024-04-22 09:08:15.218109 nonebot_adapter_kritor-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      244 2024-04-22 09:07:47.017935 nonebot_adapter_kritor-0.1.1/src/nonebot/adapters/kritor/__init__.py
--rw-r--r--   0        0        0     7191 2024-04-22 09:07:47.017935 nonebot_adapter_kritor-0.1.1/src/nonebot/adapters/kritor/adapter.py
--rw-r--r--   0        0        0    55211 2024-04-22 09:07:47.017935 nonebot_adapter_kritor-0.1.1/src/nonebot/adapters/kritor/bot.py
--rw-r--r--   0        0        0      618 2024-04-22 09:07:47.017935 nonebot_adapter_kritor-0.1.1/src/nonebot/adapters/kritor/compat.py
--rw-r--r--   0        0        0      451 2024-04-22 09:07:47.017935 nonebot_adapter_kritor-0.1.1/src/nonebot/adapters/kritor/config.py
--rw-r--r--   0        0        0    21042 2024-04-22 09:07:47.017935 nonebot_adapter_kritor-0.1.1/src/nonebot/adapters/kritor/event.py
--rw-r--r--   0        0        0     2482 2024-04-22 09:07:47.017935 nonebot_adapter_kritor-0.1.1/src/nonebot/adapters/kritor/exception.py
--rw-r--r--   0        0        0    15038 2024-04-22 09:07:47.017935 nonebot_adapter_kritor-0.1.1/src/nonebot/adapters/kritor/message.py
--rw-r--r--   0        0        0     1665 2024-04-22 09:07:47.017935 nonebot_adapter_kritor-0.1.1/src/nonebot/adapters/kritor/model.py
--rw-r--r--   0        0        0        0 2024-04-22 09:07:47.017935 nonebot_adapter_kritor-0.1.1/src/nonebot/adapters/kritor/protos/__init__.py
--rw-r--r--   0        0        0        0 2024-04-22 09:07:47.017935 nonebot_adapter_kritor-0.1.1/src/nonebot/adapters/kritor/protos/kritor/__init__.py
--rw-r--r--   0        0        0     9573 2024-04-22 09:07:47.017935 nonebot_adapter_kritor-0.1.1/src/nonebot/adapters/kritor/protos/kritor/authentication/__init__.py
--rw-r--r--   0        0        0    13153 2024-04-22 09:07:47.017935 nonebot_adapter_kritor-0.1.1/src/nonebot/adapters/kritor/protos/kritor/common/__init__.py
--rw-r--r--   0        0        0     7604 2024-04-22 09:07:47.017935 nonebot_adapter_kritor-0.1.1/src/nonebot/adapters/kritor/protos/kritor/core/__init__.py
--rw-r--r--   0        0        0     1965 2024-04-22 09:07:47.017935 nonebot_adapter_kritor-0.1.1/src/nonebot/adapters/kritor/protos/kritor/customization/__init__.py
--rw-r--r--   0        0        0    15256 2024-04-22 09:07:47.017935 nonebot_adapter_kritor-0.1.1/src/nonebot/adapters/kritor/protos/kritor/developer/__init__.py
--rw-r--r--   0        0        0    14777 2024-04-22 09:07:47.017935 nonebot_adapter_kritor-0.1.1/src/nonebot/adapters/kritor/protos/kritor/event/__init__.py
--rw-r--r--   0        0        0    13287 2024-04-22 09:07:47.017935 nonebot_adapter_kritor-0.1.1/src/nonebot/adapters/kritor/protos/kritor/file/__init__.py
--rw-r--r--   0        0        0    16773 2024-04-22 09:07:47.017935 nonebot_adapter_kritor-0.1.1/src/nonebot/adapters/kritor/protos/kritor/friend/__init__.py
--rw-r--r--   0        0        0    34177 2024-04-22 09:07:47.017935 nonebot_adapter_kritor-0.1.1/src/nonebot/adapters/kritor/protos/kritor/group/__init__.py
--rw-r--r--   0        0        0    28678 2024-04-22 09:07:47.017935 nonebot_adapter_kritor-0.1.1/src/nonebot/adapters/kritor/protos/kritor/guild/__init__.py
--rw-r--r--   0        0        0    26122 2024-04-22 09:07:47.017935 nonebot_adapter_kritor-0.1.1/src/nonebot/adapters/kritor/protos/kritor/message/__init__.py
--rw-r--r--   0        0        0     6218 2024-04-22 09:07:47.017935 nonebot_adapter_kritor-0.1.1/src/nonebot/adapters/kritor/protos/kritor/process/__init__.py
--rw-r--r--   0        0        0     2267 2024-04-22 09:07:47.017935 nonebot_adapter_kritor-0.1.1/src/nonebot/adapters/kritor/protos/kritor/reverse/__init__.py
--rw-r--r--   0        0        0     7047 2024-04-22 09:07:47.017935 nonebot_adapter_kritor-0.1.1/src/nonebot/adapters/kritor/protos/kritor/web/__init__.py
--rw-r--r--   0        0        0     1188 2024-04-22 09:07:47.017935 nonebot_adapter_kritor-0.1.1/src/nonebot/adapters/kritor/utils.py
--rw-r--r--   0        0        0        0 2024-04-22 09:07:47.017935 nonebot_adapter_kritor-0.1.1/tests/__init__.py
--rw-r--r--   0        0        0     1346 1970-01-01 00:00:00.000000 nonebot_adapter_kritor-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-05-12 06:19:03.125750 nonebot_adapter_kritor-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1042 2024-05-12 06:19:03.125750 nonebot_adapter_kritor-0.2.0/README.md
+-rw-r--r--   0        0        0     2262 2024-05-12 06:19:34.517679 nonebot_adapter_kritor-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      244 2024-05-12 06:19:03.125750 nonebot_adapter_kritor-0.2.0/src/nonebot/adapters/kritor/__init__.py
+-rw-r--r--   0        0        0     7191 2024-05-12 06:19:03.125750 nonebot_adapter_kritor-0.2.0/src/nonebot/adapters/kritor/adapter.py
+-rw-r--r--   0        0        0    55219 2024-05-12 06:19:03.125750 nonebot_adapter_kritor-0.2.0/src/nonebot/adapters/kritor/bot.py
+-rw-r--r--   0        0        0      618 2024-05-12 06:19:03.125750 nonebot_adapter_kritor-0.2.0/src/nonebot/adapters/kritor/compat.py
+-rw-r--r--   0        0        0      451 2024-05-12 06:19:03.125750 nonebot_adapter_kritor-0.2.0/src/nonebot/adapters/kritor/config.py
+-rw-r--r--   0        0        0    21042 2024-05-12 06:19:03.125750 nonebot_adapter_kritor-0.2.0/src/nonebot/adapters/kritor/event.py
+-rw-r--r--   0        0        0     2482 2024-05-12 06:19:03.125750 nonebot_adapter_kritor-0.2.0/src/nonebot/adapters/kritor/exception.py
+-rw-r--r--   0        0        0    15038 2024-05-12 06:19:03.125750 nonebot_adapter_kritor-0.2.0/src/nonebot/adapters/kritor/message.py
+-rw-r--r--   0        0        0     1899 2024-05-12 06:19:03.125750 nonebot_adapter_kritor-0.2.0/src/nonebot/adapters/kritor/model.py
+-rw-r--r--   0        0        0     2054 2024-05-12 06:19:03.125750 nonebot_adapter_kritor-0.2.0/src/nonebot/adapters/kritor/permission.py
+-rw-r--r--   0        0        0        0 2024-05-12 06:19:03.125750 nonebot_adapter_kritor-0.2.0/src/nonebot/adapters/kritor/protos/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-12 06:19:03.129750 nonebot_adapter_kritor-0.2.0/src/nonebot/adapters/kritor/protos/kritor/__init__.py
+-rw-r--r--   0        0        0     9573 2024-05-12 06:19:03.129750 nonebot_adapter_kritor-0.2.0/src/nonebot/adapters/kritor/protos/kritor/authentication/__init__.py
+-rw-r--r--   0        0        0    13329 2024-05-12 06:19:03.129750 nonebot_adapter_kritor-0.2.0/src/nonebot/adapters/kritor/protos/kritor/common/__init__.py
+-rw-r--r--   0        0        0     7604 2024-05-12 06:19:03.129750 nonebot_adapter_kritor-0.2.0/src/nonebot/adapters/kritor/protos/kritor/core/__init__.py
+-rw-r--r--   0        0        0     1965 2024-05-12 06:19:03.129750 nonebot_adapter_kritor-0.2.0/src/nonebot/adapters/kritor/protos/kritor/customization/__init__.py
+-rw-r--r--   0        0        0    15256 2024-05-12 06:19:03.129750 nonebot_adapter_kritor-0.2.0/src/nonebot/adapters/kritor/protos/kritor/developer/__init__.py
+-rw-r--r--   0        0        0    14777 2024-05-12 06:19:03.129750 nonebot_adapter_kritor-0.2.0/src/nonebot/adapters/kritor/protos/kritor/event/__init__.py
+-rw-r--r--   0        0        0    13287 2024-05-12 06:19:03.129750 nonebot_adapter_kritor-0.2.0/src/nonebot/adapters/kritor/protos/kritor/file/__init__.py
+-rw-r--r--   0        0        0    16773 2024-05-12 06:19:03.129750 nonebot_adapter_kritor-0.2.0/src/nonebot/adapters/kritor/protos/kritor/friend/__init__.py
+-rw-r--r--   0        0        0    34172 2024-05-12 06:19:03.129750 nonebot_adapter_kritor-0.2.0/src/nonebot/adapters/kritor/protos/kritor/group/__init__.py
+-rw-r--r--   0        0        0    28687 2024-05-12 06:19:03.129750 nonebot_adapter_kritor-0.2.0/src/nonebot/adapters/kritor/protos/kritor/guild/__init__.py
+-rw-r--r--   0        0        0    26122 2024-05-12 06:19:03.129750 nonebot_adapter_kritor-0.2.0/src/nonebot/adapters/kritor/protos/kritor/message/__init__.py
+-rw-r--r--   0        0        0     6218 2024-05-12 06:19:03.129750 nonebot_adapter_kritor-0.2.0/src/nonebot/adapters/kritor/protos/kritor/process/__init__.py
+-rw-r--r--   0        0        0     2267 2024-05-12 06:19:03.129750 nonebot_adapter_kritor-0.2.0/src/nonebot/adapters/kritor/protos/kritor/reverse/__init__.py
+-rw-r--r--   0        0        0     7047 2024-05-12 06:19:03.129750 nonebot_adapter_kritor-0.2.0/src/nonebot/adapters/kritor/protos/kritor/web/__init__.py
+-rw-r--r--   0        0        0     1188 2024-05-12 06:19:03.129750 nonebot_adapter_kritor-0.2.0/src/nonebot/adapters/kritor/utils.py
+-rw-r--r--   0        0        0        0 2024-05-12 06:19:03.129750 nonebot_adapter_kritor-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0     1346 1970-01-01 00:00:00.000000 nonebot_adapter_kritor-0.2.0/PKG-INFO
```

### Comparing `nonebot_adapter_kritor-0.1.1/LICENSE` & `nonebot_adapter_kritor-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_kritor-0.1.1/README.md` & `nonebot_adapter_kritor-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_kritor-0.1.1/pyproject.toml` & `nonebot_adapter_kritor-0.2.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-adapter-kritor"
-version = "0.1.1"
+version = "0.2.0"
 description = "Nonebot Adapter for Kritor Protocol"
 authors = [
     { name = "rf_tar_railt", email = "rf_tar_railt@qq.com" },
 ]
 dependencies = [
     "betterproto>=2.0.0b6",
     "nonebot2>=2.2.1",
```

### Comparing `nonebot_adapter_kritor-0.1.1/src/nonebot/adapters/kritor/adapter.py` & `nonebot_adapter_kritor-0.2.0/src/nonebot/adapters/kritor/adapter.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_kritor-0.1.1/src/nonebot/adapters/kritor/bot.py` & `nonebot_adapter_kritor-0.2.0/src/nonebot/adapters/kritor/bot.py`

 * *Files 0% similar despite different names*

```diff
@@ -383,15 +383,15 @@
         if event.contact.type == SceneType.GUILD:
             resp = await self.send_channel_message(
                 guild_id=int(event.contact.id),
                 channel_id=int(event.contact.sub_id or "0"),
                 message=str(message),
                 **kwargs,
             )
-            return SendMessageResponse(message_id=resp.message_id, message_time=resp.time)
+            return SendMessageResponse(message_id=resp.message_id, message_time=resp.message_time)
         if isinstance(message, str):
             message = Message(message)
         elif isinstance(message, MessageSegment):
             message = Message([message])
         elements = message.to_elements()
         return await self.send_message(contact=event.contact, elements=elements, message_id=event.message_id)
```

### Comparing `nonebot_adapter_kritor-0.1.1/src/nonebot/adapters/kritor/compat.py` & `nonebot_adapter_kritor-0.2.0/src/nonebot/adapters/kritor/compat.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_kritor-0.1.1/src/nonebot/adapters/kritor/event.py` & `nonebot_adapter_kritor-0.2.0/src/nonebot/adapters/kritor/event.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_kritor-0.1.1/src/nonebot/adapters/kritor/exception.py` & `nonebot_adapter_kritor-0.2.0/src/nonebot/adapters/kritor/exception.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_kritor-0.1.1/src/nonebot/adapters/kritor/message.py` & `nonebot_adapter_kritor-0.2.0/src/nonebot/adapters/kritor/message.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_kritor-0.1.1/src/nonebot/adapters/kritor/model.py` & `nonebot_adapter_kritor-0.2.0/src/nonebot/adapters/kritor/model.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from enum import IntEnum
 from typing import Union, Literal, Optional
 
 from pydantic import Field, BaseModel
 
 from .protos.kritor.common import Scene
+from .protos.kritor.common import Role as ProtoRole
 from .protos.kritor.common import Sender as ProtoSender
 from .protos.kritor.common import Contact as ProtoContact
 
 
 class SceneType(IntEnum):
     GROUP = 0
     FRIEND = 1
@@ -58,18 +59,27 @@
 
 ContactType = Union[
     Union[Group, Friend, Guild, Stranger, StrangerFromGroup, Nearby],
     Contact,
 ]
 
 
+class Role(IntEnum):
+    UNKNOWN = 0
+    MEMBER = 1
+    ADMIN = 2
+    OWNER = 3
+
+
 class Sender(BaseModel):
     uid: str
     uin: Optional[int] = None
     nick: Optional[str] = None
+    role: Optional[Role] = None
 
     def dump(self) -> ProtoSender:
         return ProtoSender(
             uid=self.uid,
             uin=self.uin,
             nick=self.nick,
+            role=ProtoRole(self.role.value) if self.role else None,
         )
```

### Comparing `nonebot_adapter_kritor-0.1.1/src/nonebot/adapters/kritor/protos/kritor/authentication/__init__.py` & `nonebot_adapter_kritor-0.2.0/src/nonebot/adapters/kritor/protos/kritor/authentication/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_kritor-0.1.1/src/nonebot/adapters/kritor/protos/kritor/common/__init__.py` & `nonebot_adapter_kritor-0.2.0/src/nonebot/adapters/kritor/protos/kritor/common/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,21 @@
     STRANGER_FROM_GROUP = 10
     NEARBY = 5
     """以下类型为可选实现"""
 
     STRANGER = 9
 
 
+class Role(betterproto.Enum):
+    UNKNOWN = 0
+    MEMBER = 1
+    ADMIN = 2
+    OWNER = 3
+
+
 class ElementElementType(betterproto.Enum):
     TEXT = 0
     AT = 1
     FACE = 2
     BUBBLE_FACE = 3
     REPLY = 4
     IMAGE = 5
@@ -76,14 +83,15 @@
 
 
 @dataclass(eq=False, repr=False)
 class Sender(betterproto.Message):
     uid: str = betterproto.string_field(1)
     uin: Optional[int] = betterproto.uint64_field(2, optional=True, group="_uin")
     nick: Optional[str] = betterproto.string_field(3, optional=True, group="_nick")
+    role: Optional["Role"] = betterproto.enum_field(4, optional=True, group="_role")
 
 
 @dataclass(eq=False, repr=False)
 class Element(betterproto.Message):
     type: "ElementElementType" = betterproto.enum_field(1)
     """be friendly to some languages that don't support oneof"""
 
@@ -324,15 +332,15 @@
 class KeyboardElement(betterproto.Message):
     rows: List["KeyboardRow"] = betterproto.message_field(1)
     bot_appid: int = betterproto.uint64_field(2)
 
 
 @dataclass(eq=False, repr=False)
 class PushMessageBody(betterproto.Message):
-    time: int = betterproto.uint32_field(1)
+    time: int = betterproto.uint64_field(1)
     message_id: str = betterproto.string_field(2)
     message_seq: int = betterproto.uint64_field(3)
     contact: "Contact" = betterproto.message_field(4)
     sender: "Sender" = betterproto.message_field(5)
     elements: List["Element"] = betterproto.message_field(6)
 
 
@@ -347,16 +355,16 @@
     group_id: int = betterproto.uint32_field(1)
     sender_uid: str = betterproto.string_field(2)
     sender_uin: int = betterproto.uint64_field(3)
     sender_nick: str = betterproto.string_field(4)
     operator_uid: int = betterproto.uint64_field(5)
     operator_uin: int = betterproto.uint64_field(6)
     operator_nick: str = betterproto.string_field(7)
-    operation_time: int = betterproto.uint32_field(8)
-    message_time: int = betterproto.uint32_field(9)
+    operation_time: int = betterproto.uint64_field(8)
+    message_time: int = betterproto.uint64_field(9)
     message_id: str = betterproto.string_field(10)
     message_seq: int = betterproto.uint64_field(11)
     json_elements: str = betterproto.string_field(12)
 
 
 @dataclass(eq=False, repr=False)
 class Request(betterproto.Message):
```

### Comparing `nonebot_adapter_kritor-0.1.1/src/nonebot/adapters/kritor/protos/kritor/core/__init__.py` & `nonebot_adapter_kritor-0.2.0/src/nonebot/adapters/kritor/protos/kritor/core/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_kritor-0.1.1/src/nonebot/adapters/kritor/protos/kritor/customization/__init__.py` & `nonebot_adapter_kritor-0.2.0/src/nonebot/adapters/kritor/protos/kritor/customization/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_kritor-0.1.1/src/nonebot/adapters/kritor/protos/kritor/developer/__init__.py` & `nonebot_adapter_kritor-0.2.0/src/nonebot/adapters/kritor/protos/kritor/developer/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_kritor-0.1.1/src/nonebot/adapters/kritor/protos/kritor/event/__init__.py` & `nonebot_adapter_kritor-0.2.0/src/nonebot/adapters/kritor/protos/kritor/event/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,15 +89,15 @@
 class PrivateFileUploadedNotice(betterproto.Message):
     operator_uid: str = betterproto.string_field(1)
     operator_uin: int = betterproto.uint64_field(2)
     file_id: str = betterproto.string_field(3)
     file_sub_id: str = betterproto.string_field(4)
     file_name: str = betterproto.string_field(5)
     file_size: int = betterproto.uint64_field(6)
-    expire_time: int = betterproto.uint32_field(7)
+    expire_time: int = betterproto.uint64_field(7)
     url: str = betterproto.string_field(8)
 
 
 @dataclass(eq=False, repr=False)
 class GroupPokeNotice(betterproto.Message):
     group_id: int = betterproto.uint64_field(1)
     operator_uid: str = betterproto.string_field(2)
@@ -125,15 +125,15 @@
     group_id: int = betterproto.uint64_field(1)
     operator_uid: str = betterproto.string_field(2)
     operator_uin: int = betterproto.uint64_field(3)
     file_id: str = betterproto.string_field(4)
     file_name: str = betterproto.string_field(5)
     file_size: int = betterproto.uint64_field(6)
     bus_id: int = betterproto.int32_field(7)
-    expire_time: int = betterproto.uint32_field(8)
+    expire_time: int = betterproto.uint64_field(8)
     file_url: str = betterproto.string_field(9)
 
 
 @dataclass(eq=False, repr=False)
 class GroupCardChangedNotice(betterproto.Message):
     group_id: int = betterproto.uint64_field(1)
     operator_uid: str = betterproto.string_field(2)
@@ -225,15 +225,15 @@
     face_id: int = betterproto.uint32_field(3)
     is_set: bool = betterproto.bool_field(4)
 
 
 @dataclass(eq=False, repr=False)
 class NoticeEvent(betterproto.Message):
     type: "NoticeEventNoticeType" = betterproto.enum_field(1)
-    time: int = betterproto.uint32_field(2)
+    time: int = betterproto.uint64_field(2)
     notice_id: str = betterproto.string_field(3)
     private_poke: "PrivatePokeNotice" = betterproto.message_field(10, group="notice")
     private_recall: "PrivateRecallNotice" = betterproto.message_field(11, group="notice")
     private_file_uploaded: "PrivateFileUploadedNotice" = betterproto.message_field(12, group="notice")
     group_poke: "GroupPokeNotice" = betterproto.message_field(20, group="notice")
     group_recall: "GroupRecallNotice" = betterproto.message_field(21, group="notice")
     group_file_uploaded: "GroupFileUploadedNotice" = betterproto.message_field(22, group="notice")
@@ -272,15 +272,15 @@
     inviter_uid: str = betterproto.string_field(2)
     inviter_uin: int = betterproto.uint64_field(3)
 
 
 @dataclass(eq=False, repr=False)
 class RequestEvent(betterproto.Message):
     type: "RequestEventRequestType" = betterproto.enum_field(1)
-    time: int = betterproto.uint32_field(2)
+    time: int = betterproto.uint64_field(2)
     request_id: str = betterproto.string_field(3)
     friend_apply: "FriendApplyRequest" = betterproto.message_field(10, group="request")
     group_apply: "GroupApplyRequest" = betterproto.message_field(11, group="request")
     invited_group: "InvitedJoinGroupRequest" = betterproto.message_field(12, group="request")
 
 
 @dataclass(eq=False, repr=False)
```

### Comparing `nonebot_adapter_kritor-0.1.1/src/nonebot/adapters/kritor/protos/kritor/file/__init__.py` & `nonebot_adapter_kritor-0.2.0/src/nonebot/adapters/kritor/protos/kritor/file/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,31 +18,31 @@
 
 @dataclass(eq=False, repr=False)
 class File(betterproto.Message):
     file_id: str = betterproto.string_field(1)
     file_name: str = betterproto.string_field(2)
     file_size: int = betterproto.uint64_field(3)
     bus_id: int = betterproto.int32_field(4)
-    upload_time: int = betterproto.uint32_field(5)
-    expire_time: int = betterproto.uint32_field(6)
-    modify_time: int = betterproto.uint32_field(7)
+    upload_time: int = betterproto.uint64_field(5)
+    expire_time: int = betterproto.uint64_field(6)
+    modify_time: int = betterproto.uint64_field(7)
     download_times: int = betterproto.uint32_field(8)
     uploader: int = betterproto.uint64_field(9)
     uploader_name: str = betterproto.string_field(10)
     sha: str = betterproto.string_field(11)
     sha3: str = betterproto.string_field(12)
     md5: str = betterproto.string_field(13)
 
 
 @dataclass(eq=False, repr=False)
 class Folder(betterproto.Message):
     folder_id: str = betterproto.string_field(1)
     folder_name: str = betterproto.string_field(2)
     total_file_count: int = betterproto.uint32_field(3)
-    create_time: int = betterproto.uint32_field(4)
+    create_time: int = betterproto.uint64_field(4)
     creator: int = betterproto.uint64_field(5)
     creator_name: str = betterproto.string_field(6)
 
 
 @dataclass(eq=False, repr=False)
 class CreateFolderRequest(betterproto.Message):
     group_id: int = betterproto.uint64_field(1)
```

### Comparing `nonebot_adapter_kritor-0.1.1/src/nonebot/adapters/kritor/protos/kritor/friend/__init__.py` & `nonebot_adapter_kritor-0.2.0/src/nonebot/adapters/kritor/protos/kritor/friend/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_kritor-0.1.1/src/nonebot/adapters/kritor/protos/kritor/group/__init__.py` & `nonebot_adapter_kritor-0.2.0/src/nonebot/adapters/kritor/protos/kritor/group/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,24 +39,24 @@
 class NotJoinedGroupInfo(betterproto.Message):
     group_id: int = betterproto.uint64_field(1)
     max_member_count: int = betterproto.uint32_field(2)
     member_count: int = betterproto.uint32_field(3)
     group_name: str = betterproto.string_field(4)
     group_desc: str = betterproto.string_field(5)
     owner: int = betterproto.uint64_field(6)
-    create_time: int = betterproto.uint32_field(7)
+    create_time: int = betterproto.uint64_field(7)
     group_flag: int = betterproto.uint32_field(8)
     group_flag_ext: int = betterproto.uint32_field(9)
 
 
 @dataclass(eq=False, repr=False)
 class ProhibitedUserInfo(betterproto.Message):
     uid: str = betterproto.string_field(1)
     uin: int = betterproto.uint64_field(2)
-    prohibited_time: int = betterproto.uint32_field(3)
+    prohibited_time: int = betterproto.uint64_field(3)
 
 
 @dataclass(eq=False, repr=False)
 class GroupHonorInfo(betterproto.Message):
     uid: str = betterproto.string_field(1)
     uin: int = betterproto.uint64_field(2)
     nick: str = betterproto.string_field(3)
@@ -69,20 +69,20 @@
 @dataclass(eq=False, repr=False)
 class GroupMemberInfo(betterproto.Message):
     uid: str = betterproto.string_field(1)
     uin: int = betterproto.uint64_field(2)
     nick: str = betterproto.string_field(3)
     age: int = betterproto.uint32_field(4)
     unique_title: str = betterproto.string_field(5)
-    unique_title_expire_time: int = betterproto.uint32_field(6)
+    unique_title_expire_time: int = betterproto.uint64_field(6)
     card: str = betterproto.string_field(7)
     join_time: int = betterproto.uint64_field(8)
     last_active_time: int = betterproto.uint64_field(9)
     level: int = betterproto.uint32_field(10)
-    shut_up_timestamp: int = betterproto.uint64_field(11)
+    shut_up_time: int = betterproto.uint64_field(11)
     distance: Optional[int] = betterproto.uint32_field(100, optional=True, group="_distance")
     honors: List[int] = betterproto.uint32_field(101)
     unfriendly: Optional[bool] = betterproto.bool_field(102, optional=True, group="_unfriendly")
     card_changeable: Optional[bool] = betterproto.bool_field(103, optional=True, group="_card_changeable")
 
 
 @dataclass(eq=False, repr=False)
```

### Comparing `nonebot_adapter_kritor-0.1.1/src/nonebot/adapters/kritor/protos/kritor/guild/__init__.py` & `nonebot_adapter_kritor-0.2.0/src/nonebot/adapters/kritor/protos/kritor/guild/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -241,15 +241,15 @@
 
 
 @dataclass(eq=False, repr=False)
 class SendChannelMessageResponse(betterproto.Message):
     """发送信息到子频道响应"""
 
     message_id: str = betterproto.string_field(1)
-    time: int = betterproto.int64_field(2)
+    message_time: int = betterproto.uint64_field(2)
 
 
 @dataclass(eq=False, repr=False)
 class GetGuildFeedListRequest(betterproto.Message):
     """获取频道帖子广场帖子请求"""
 
     guild_id: int = betterproto.uint64_field(1)
```

### Comparing `nonebot_adapter_kritor-0.1.1/src/nonebot/adapters/kritor/protos/kritor/message/__init__.py` & `nonebot_adapter_kritor-0.2.0/src/nonebot/adapters/kritor/protos/kritor/message/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,28 +29,28 @@
     notice_id: Optional[str] = betterproto.string_field(5, optional=True, group="_notice_id")
     request_id: Optional[str] = betterproto.string_field(6, optional=True, group="_request_id")
 
 
 @dataclass(eq=False, repr=False)
 class SendMessageResponse(betterproto.Message):
     message_id: str = betterproto.string_field(1)
-    message_time: int = betterproto.uint32_field(2)
+    message_time: int = betterproto.uint64_field(2)
 
 
 @dataclass(eq=False, repr=False)
 class SendMessageByResIdRequest(betterproto.Message):
     contact: "_common__.Contact" = betterproto.message_field(1)
     res_id: str = betterproto.string_field(2)
     retry_count: Optional[int] = betterproto.uint32_field(3, optional=True, group="_retry_count")
 
 
 @dataclass(eq=False, repr=False)
 class SendMessageByResIdResponse(betterproto.Message):
     message_id: str = betterproto.string_field(1)
-    message_time: int = betterproto.uint32_field(2)
+    message_time: int = betterproto.uint64_field(2)
 
 
 @dataclass(eq=False, repr=False)
 class SetMessageReadRequest(betterproto.Message):
     contact: "_common__.Contact" = betterproto.message_field(1)
```

### Comparing `nonebot_adapter_kritor-0.1.1/src/nonebot/adapters/kritor/protos/kritor/process/__init__.py` & `nonebot_adapter_kritor-0.2.0/src/nonebot/adapters/kritor/protos/kritor/process/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_kritor-0.1.1/src/nonebot/adapters/kritor/protos/kritor/reverse/__init__.py` & `nonebot_adapter_kritor-0.2.0/src/nonebot/adapters/kritor/protos/kritor/reverse/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_kritor-0.1.1/src/nonebot/adapters/kritor/protos/kritor/web/__init__.py` & `nonebot_adapter_kritor-0.2.0/src/nonebot/adapters/kritor/protos/kritor/web/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_kritor-0.1.1/src/nonebot/adapters/kritor/utils.py` & `nonebot_adapter_kritor-0.2.0/src/nonebot/adapters/kritor/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_kritor-0.1.1/PKG-INFO` & `nonebot_adapter_kritor-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-adapter-kritor
-Version: 0.1.1
+Version: 0.2.0
 Summary: Nonebot Adapter for Kritor Protocol
 Author-Email: rf_tar_railt <rf_tar_railt@qq.com>
 License: MIT
 Requires-Python: >=3.9
 Requires-Dist: betterproto>=2.0.0b6
 Requires-Dist: nonebot2>=2.2.1
 Description-Content-Type: text/markdown
```

