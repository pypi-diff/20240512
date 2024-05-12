# Comparing `tmp/revtongyi-0.1.2.0.tar.gz` & `tmp/revtongyi-0.1.2.1.tar.gz`

## Comparing `revtongyi-0.1.2.0.tar` & `revtongyi-0.1.2.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 revtongyi-0.1.2.0/.github/workflows/publish-pypi.yaml
--rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 revtongyi-0.1.2.0/revTongYi/__init__.py
--rw-r--r--   0        0        0     2876 2020-02-02 00:00:00.000000 revtongyi-0.1.2.0/revTongYi/entity.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 revtongyi-0.1.2.0/revTongYi/errors.py
--rw-r--r--   0        0        0    11810 2020-02-02 00:00:00.000000 revtongyi-0.1.2.0/revTongYi/qianwen.py
--rw-r--r--   0        0        0     4103 2020-02-02 00:00:00.000000 revtongyi-0.1.2.0/revTongYi/wanxiang.py
--rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 revtongyi-0.1.2.0/tests/qianwen.py
--rw-r--r--   0        0        0     3098 2020-02-02 00:00:00.000000 revtongyi-0.1.2.0/.gitignore
--rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 revtongyi-0.1.2.0/LICENSE
--rw-r--r--   0        0        0     3044 2020-02-02 00:00:00.000000 revtongyi-0.1.2.0/README.md
--rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 revtongyi-0.1.2.0/pyproject.toml
--rw-r--r--   0        0        0     3684 2020-02-02 00:00:00.000000 revtongyi-0.1.2.0/PKG-INFO
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 revtongyi-0.1.2.1/.github/workflows/publish-pypi.yaml
+-rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 revtongyi-0.1.2.1/revTongYi/__init__.py
+-rw-r--r--   0        0        0     3180 2020-02-02 00:00:00.000000 revtongyi-0.1.2.1/revTongYi/entity.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 revtongyi-0.1.2.1/revTongYi/errors.py
+-rw-r--r--   0        0        0    11810 2020-02-02 00:00:00.000000 revtongyi-0.1.2.1/revTongYi/qianwen.py
+-rw-r--r--   0        0        0     4103 2020-02-02 00:00:00.000000 revtongyi-0.1.2.1/revTongYi/wanxiang.py
+-rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 revtongyi-0.1.2.1/tests/qianwen.py
+-rw-r--r--   0        0        0     3098 2020-02-02 00:00:00.000000 revtongyi-0.1.2.1/.gitignore
+-rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 revtongyi-0.1.2.1/LICENSE
+-rw-r--r--   0        0        0     3044 2020-02-02 00:00:00.000000 revtongyi-0.1.2.1/README.md
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 revtongyi-0.1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     3684 2020-02-02 00:00:00.000000 revtongyi-0.1.2.1/PKG-INFO
```

### Comparing `revtongyi-0.1.2.0/.github/workflows/publish-pypi.yaml` & `revtongyi-0.1.2.1/.github/workflows/publish-pypi.yaml`

 * *Files identical despite different names*

### Comparing `revtongyi-0.1.2.0/revTongYi/__init__.py` & `revtongyi-0.1.2.1/revTongYi/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import time
 import requests
 import typing
 import json
 import uuid
 
 from fake_useragent import UserAgent
 
@@ -36,17 +37,18 @@
 
         last_out = ""
 
         print("AI  > ", end="")
 
         for resp in reply_iter:
             lastId = resp.msgId
-            if 'contents' in resp:
+            if resp.contents:
                 resp_text = resp.contents[-1].content
-                print(resp_text.replace(last_out, ""), end="")
+                print(resp_text.replace(last_out, ""), end="", flush=True)
+                time.sleep(0.1)
                 last_out = resp_text
                 sessionId = resp.sessionId
         
         question = input("\nYou > ")
 
 
 if __name__ == "__main__":
```

### Comparing `revtongyi-0.1.2.0/revTongYi/entity.py` & `revtongyi-0.1.2.1/revTongYi/entity.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 响应模版
 """
+from typing import List, Union
 
 
 class ChatContent:
     """
     对话内容模版
     """
     content: str
@@ -25,30 +26,39 @@
     def __str__(self):
         return str(self.__dict__)
 
     def __repr__(self):
         return str(self)
 
 
+def handle_contents(contents: List[dict]) -> List[ChatContent]:
+    """处理对话内容"""
+    content_list = []
+    for content in contents:
+        if content["contentType"] in ["text", "text2image"]:
+            content["content"] = content["content"]
+            content_list.append(ChatContent(content))
+    return content_list
+
+
 class QianWenChatResponse:
     """
     对话响应模版
     """
     contentType: str
-    contents: list[ChatContent] | None
+    contents: Union[List[ChatContent], None]
     msgStatus: str
     msgId: str
     parentMsgId: str
     sessionId: str
 
     def __init__(self, response: dict):
         packaged_response = {
             "contentType": response["contentType"],
-            "contents": [ChatContent(content) for content in response["contents"]] if response.get(
-                "contents") else None,
+            "contents": handle_contents(response["contents"]) if response.get("contents") else None,
             "msgStatus": response["msgStatus"],
             "msgId": response["msgId"],
             "parentMsgId": response["parentMsgId"],
             "sessionId": response["sessionId"]
         }
         self.__dict__ = packaged_response
 
@@ -70,27 +80,26 @@
     历史记录响应模版
     """
     sessionId: str
     msgId: str
     msgStatus: str
     parentMsgId: str
     contentType: str
-    contents: list[ChatContent] | None
+    contents: Union[List[ChatContent], None]
     senderType: str
     createTime: int
 
     def __init__(self, response: dict):
         packaged_response = {
             "sessionId": response["sessionId"],
             "msgId": response["msgId"],
             "msgStatus": response["msgStatus"],
             "parentMsgId": response["parentMsgId"],
             "contentType": response["contentType"],
-            "contents": [ChatContent(content) for content in response["contents"]] if response.get(
-                "contents") else None,
+            "contents": handle_contents(response["contents"]) if response.get("contents") else None,
             "senderType": response["senderType"],
             "createTime": response["createTime"]
         }
         self.__dict__ = packaged_response
 
     def __getitem__(self, key):
         return getattr(self, key)
```

### Comparing `revtongyi-0.1.2.0/revTongYi/qianwen.py` & `revtongyi-0.1.2.1/revTongYi/qianwen.py`

 * *Files identical despite different names*

### Comparing `revtongyi-0.1.2.0/revTongYi/wanxiang.py` & `revtongyi-0.1.2.1/revTongYi/wanxiang.py`

 * *Files identical despite different names*

### Comparing `revtongyi-0.1.2.0/tests/qianwen.py` & `revtongyi-0.1.2.1/tests/qianwen.py`

 * *Files identical despite different names*

### Comparing `revtongyi-0.1.2.0/.gitignore` & `revtongyi-0.1.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `revtongyi-0.1.2.0/LICENSE` & `revtongyi-0.1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `revtongyi-0.1.2.0/README.md` & `revtongyi-0.1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `revtongyi-0.1.2.0/pyproject.toml` & `revtongyi-0.1.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "revTongYi"
-version = "0.1.2.0"
+version = "0.1.2.1"
 authors = [
   { name="xw5xr6", email="xw5xr6@hotmail.com" },
   { name="leeeduke", email="dukelee652@gmail.com" }
 ]
 description = "阿里通义千问逆向工程API"
 readme = "README.md"
 requires-python = ">=3.7"
@@ -21,8 +21,8 @@
     "fake-useragent",
     "requests",
     "filetype"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/leeeduke/revTongYi"
-"Bug Tracker" = "https://github.com/leeeduke/revTongYi/issues"
+"Bug Tracker" = "https://github.com/leeeduke/revTongYi/issues"
```

### Comparing `revtongyi-0.1.2.0/PKG-INFO` & `revtongyi-0.1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: revTongYi
-Version: 0.1.2.0
+Version: 0.1.2.1
 Summary: 阿里通义千问逆向工程API
 Project-URL: Homepage, https://github.com/leeeduke/revTongYi
 Project-URL: Bug Tracker, https://github.com/leeeduke/revTongYi/issues
 Author-email: xw5xr6 <xw5xr6@hotmail.com>, leeeduke <dukelee652@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

