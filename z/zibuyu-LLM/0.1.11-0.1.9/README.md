# Comparing `tmp/zibuyu_LLM-0.1.11-py3-none-any.whl.zip` & `tmp/zibuyu_LLM-0.1.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 67515 bytes, number of entries: 18
+Zip file size: 67284 bytes, number of entries: 18
 -rw-rw-rw-  2.0 fat      305 b- defN 24-May-11 08:41 zibuyu_llm_api/__init__.py
 -rw-rw-rw-  2.0 fat    31879 b- defN 24-May-11 08:41 zibuyu_llm_api/minmax_api.py
 -rw-rw-rw-  2.0 fat      735 b- defN 24-May-11 08:46 zibuyu_llm_web/__init__.py
 -rw-rw-rw-  2.0 fat     7376 b- defN 24-May-11 14:22 zibuyu_llm_web/baichuan.py
 -rw-rw-rw-  2.0 fat     7104 b- defN 24-May-12 05:31 zibuyu_llm_web/base.py
 -rw-rw-rw-  2.0 fat    14789 b- defN 24-May-11 14:25 zibuyu_llm_web/deepseek.py
 -rw-rw-rw-  2.0 fat      732 b- defN 24-May-11 08:49 zibuyu_llm_web/errors.py
 -rw-rw-rw-  2.0 fat     9962 b- defN 24-May-11 14:22 zibuyu_llm_web/kimi.py
 -rw-rw-rw-  2.0 fat    37747 b- defN 24-May-12 02:39 zibuyu_llm_web/minmax.py
 -rw-rw-rw-  2.0 fat    37730 b- defN 24-May-11 13:49 zibuyu_llm_web/qwen.py
 -rw-rw-rw-  2.0 fat     5308 b- defN 24-May-12 03:43 zibuyu_llm_web/types.py
 -rw-rw-rw-  2.0 fat     8118 b- defN 24-May-11 08:37 zibuyu_llm_web/wanxiang.py
 -rw-rw-rw-  2.0 fat    14705 b- defN 24-May-11 14:25 zibuyu_llm_web/xinchen.py
--rw-rw-rw-  2.0 fat    57022 b- defN 24-May-12 08:07 zibuyu_llm_web/xunfei.py
--rw-rw-rw-  2.0 fat     1697 b- defN 24-May-12 08:07 zibuyu_LLM-0.1.11.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-12 08:07 zibuyu_LLM-0.1.11.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       30 b- defN 24-May-12 08:07 zibuyu_LLM-0.1.11.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1459 b- defN 24-May-12 08:07 zibuyu_LLM-0.1.11.dist-info/RECORD
-18 files, 236790 bytes uncompressed, 65149 bytes compressed:  72.5%
+-rw-rw-rw-  2.0 fat    55663 b- defN 24-May-12 05:50 zibuyu_llm_web/xunfei.py
+-rw-rw-rw-  2.0 fat     1621 b- defN 24-May-12 05:51 zibuyu_LLM-0.1.9.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-12 05:51 zibuyu_LLM-0.1.9.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       30 b- defN 24-May-12 05:51 zibuyu_LLM-0.1.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1455 b- defN 24-May-12 05:51 zibuyu_LLM-0.1.9.dist-info/RECORD
+18 files, 235351 bytes uncompressed, 64926 bytes compressed:  72.4%
```

## zipnote {}

```diff
@@ -36,20 +36,20 @@
 
 Filename: zibuyu_llm_web/xinchen.py
 Comment: 
 
 Filename: zibuyu_llm_web/xunfei.py
 Comment: 
 
-Filename: zibuyu_LLM-0.1.11.dist-info/METADATA
+Filename: zibuyu_LLM-0.1.9.dist-info/METADATA
 Comment: 
 
-Filename: zibuyu_LLM-0.1.11.dist-info/WHEEL
+Filename: zibuyu_LLM-0.1.9.dist-info/WHEEL
 Comment: 
 
-Filename: zibuyu_LLM-0.1.11.dist-info/top_level.txt
+Filename: zibuyu_LLM-0.1.9.dist-info/top_level.txt
 Comment: 
 
-Filename: zibuyu_LLM-0.1.11.dist-info/RECORD
+Filename: zibuyu_LLM-0.1.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## zibuyu_llm_web/xunfei.py

```diff
@@ -32,14 +32,16 @@
 from .errors import LoginFailError, APIConnectionError, NeedLoginError
 
 BASE_DIR = Path(__file__).parent
 STATIC_DIR = BASE_DIR / 'static_data'
 if not STATIC_DIR.exists():
     STATIC_DIR.mkdir(parents=True)
 
+JS_FILE_PATH = STATIC_DIR / 'generate_w.js'
+
 
 class GTrace(object):
     def __init__(self):
         self.__pos_x = []
         self.__pos_y = []
         self.__pos_z = []
 
@@ -170,30 +172,30 @@
         for idx in range(len(x)):
             result.append([int(x[idx]), int(y[idx]), int(z[idx])])
 
         return int(_distance), result
 
 
 class WebLogin(object):
-    """该类用于讯飞网页版登录，获取登录token"""
+    """
+    该类用于讯飞网页版登录，获取登录token
+    """
 
     def __init__(
             self,
             account_name: str,
             password: str,
             logger: logging.Logger = None,
-            generate_w_js_file_path: str = None,
     ):
         """
 
         :param account_name: 账号
         :param password: 密码
         """
 
-        self.generate_w_js_file_path = generate_w_js_file_path
         self.account_name = account_name
         self.password = password
         self.logger = logger or logging.getLogger(__name__)
 
         self.gt = ''
         self.challenge = ''
         self.c = ''
@@ -610,15 +612,15 @@
 
     def generate_w(self, target_bytes, background_bytes):
 
         res = self.get_slice_res(target_bytes, background_bytes)
         self.logger.info(f'【generate_w】识别结果：{res}')
 
         # 读取slide.js执行get_w()方法
-        with open(self.generate_w_js_file_path, 'r', encoding='utf-8') as f:
+        with open(JS_FILE_PATH, 'r', encoding='utf-8') as f:
             js = f.read()
 
         ctx = execjs.compile(js)
 
         gtrace = GTrace()
 
         # -10，图片不是从头部开始的
@@ -772,18 +774,14 @@
         self.logger.info(f'【get_cookie】请求响应数据：{response.text}')
 
         for k, v in self.session.cookies.items():
             print(f'{k}: {v}')
 
     def run(self):
 
-        if not self.generate_w_js_file_path:
-            print('缺少js解密文件')
-            return
-
         self.if_captcha()
         print(f"第一次请求，if_captcha")
 
         print('-'.center(50, '-'))
 
         self.get_gt_and_challenge()
         print(f"第二次请求，获取gt和challenge")
@@ -836,20 +834,15 @@
         self.login()
         print('-'.center(50, '-'))
 
         if self.sso_session_id:
             print(f"第十一次请求，获取cookie")
             self.get_cookie()
 
-    def get_session_id(self, generate_w_js_file_path: str = None):
-
-        self.generate_w_js_file_path = generate_w_js_file_path
-
-        if not self.generate_w_js_file_path:
-            raise Exception('缺少js解密文件')
+    def get_session_id(self):
 
         for i in range(3):
 
             self.if_captcha()
 
             self.get_gt_and_challenge()
 
@@ -883,43 +876,31 @@
 
 class XunFeiWeb(LLMBase):
     model_name = 'XunFeiWeb'
     base_url = 'https://xinghuo.xfyun.cn'
 
     def __init__(
             self,
-            cookie: str = None,
             account: str = None,
             password: str = None,
-            error_dir: str = None,
+            cookie: str = None,
             sso_session_id: str = None,
             logger_obj: logging.Logger = None,
-            generate_w_js_file_path: str = None,
+            error_dir: str = None,
             *args,
             **kwargs
     ):
-        """
-        :param generate_w_js_file_path: js解密文件
-        :param account: 账号
-        :param password: 密码
-        :param cookie: cookie
-        :param sso_session_id: ssoSessionId
-        :param logger_obj: 日志对象
-        :param error_dir: 错误保存目录
-        """
-
         self.logger = logger_obj
         self.account = account
         self.password = password
         self.cookie = cookie
         self._sso_session_id = sso_session_id
         self._account_id: str = ''
         self.__gt_token = ''
         self.error_dir = error_dir
-        self.generate_w_js_file_path = generate_w_js_file_path
 
         super().__init__()
         self.request_session.cookies.update(self.cookies_dict)
 
         if self._sso_session_id:
             self.request_session.cookies.set('ssoSessionId', self._sso_session_id)
 
@@ -1010,15 +991,15 @@
         raise APIConnectionError(f'【{self.model_name}】 get request failed. URL: 【{url}】')
 
     def post(
             self,
             url: str,
             headers: dict = None,
             params: Optional[dict] = None,
-            _json: Optional[dict] = None,
+            json: Optional[dict] = None,
             data: [dict, str] = None,
             stream=False
     ) -> Optional[requests.Response]:
 
         # 防止网络错误，设置重试次数
         for i in range(3):
 
@@ -1026,15 +1007,15 @@
                 if not headers:
                     headers = self.__headers
 
                 response = self.request_session.post(
                     url,
                     headers=headers,
                     params=params,
-                    json=_json,
+                    json=json,
                     data=data,
                     stream=stream,
                     verify=False
                 )
 
                 if response.status_code == 200:
                     return response
@@ -1048,23 +1029,25 @@
                     self.logger.error('重新登录失败，即将退出程序...')
                     break
                 else:
                     self.logger.error(f'【{self.model_name}】 post failed, status_code: 【{response.status_code}】')
             except:
                 self.logger.error(f'【{self.model_name}】 post request got an unexpected error.', exc_info=True)
 
+        raise APIConnectionError(f'【{self.model_name}】 post request failed. URL: 【{url}】')
+
     def login(self) -> bool:
         """登录新方法，添加极验滑块的逆向"""
 
         try:
             handler = WebLogin(
                 account_name=self.account,
                 password=self.password,
             )
-            session_id = handler.get_session_id(self.generate_w_js_file_path)
+            session_id = handler.get_session_id()
 
             if session_id:
                 self.request_session.headers.update({'Cookie': f'ssoSessionId={session_id}'})
                 self._sso_session_id = session_id
                 return True
         except:
             self.logger.error(f'【{self.model_name}】 login failed', exc_info=True)
@@ -1109,71 +1092,56 @@
 
     def get_chat_list(self) -> List[dict]:
         """获取会话列表"""
 
         url = self.base_url + '/iflygpt/u/chat-list/v1/chat-list'
 
         response = self.get(url=url)
-
-        if not response:
-            return []
-
         return self.parse_data(response.json(), 'get_chat_list')
 
     def get_prompt_list(self) -> dict:
         """
         获取提示列表
         :return：提示列表
         """
 
         url = self.base_url + '/iflygpt/u/prompt/getPromptList'
 
         response = self.get(url)
-
-        if not response:
-            return {}
-
         return self.parse_data(response.json(), 'get_prompt_list')
 
     def get_chat_history(self, chat_id: [int, str]) -> dict:
         """
         获取会话记录
         :param chat_id：会话 ID
         :return：会话记录
         """
 
         url = self.base_url + f'/iflygpt/u/chat_history/all/{chat_id}'
 
         response = self.get(url)
 
-        if not response:
-            return {}
-
         return self.parse_data(response.json(), 'get_chat_history')
 
     def create_new_chat(self, bot_id: str = None) -> str:
         """
         创建新的会话，注意，在新的会话窗口未被使用前，重复创建返回的chat_id是一样的
-        :return：成功时返回新建的chat_id；失败时返回空字符串
+        :return：chat_id
         """
 
         url = self.base_url + '/iflygpt/u/chat-list/v1/create-chat-list'
         headers = self.__headers.copy()
         headers['Content-Type'] = 'application/json;charset=UTF-8'
 
         if bot_id:
             data = json.dumps({"botId": bot_id})
         else:
             data = "{}"
 
         response = self.post(url=url, headers=headers, data=data)
-
-        if not response:
-            return ''
-
         data = self.parse_data(response.json(), 'create_new_chat')
         chat_id = data.get('id')
 
         if chat_id:
             self.chat_id = chat_id
             return chat_id
 
@@ -1187,38 +1155,30 @@
 
         url = self.base_url + '/iflygpt/u/chat-list/v1/rename-chat-list'
         headers = self.__headers.copy()
         headers['Content-Type'] = 'application/json;charset=UTF-8'
 
         _json = {'chatListId': chat_id, 'chatListName': name}
 
-        response = self.post(url=url, headers=headers, _json=_json)
-
-        if not response:
-            return False
-
+        response = self.post(url=url, headers=headers, json=_json)
         return self.parse_data(response.json(), 'rename_chat') or False
 
     def delete_chat(self, chat_id: int) -> bool:
         """
         删除会话
         :param chat_id：会话 ID
         :return：bool
         """
 
         url = self.base_url + '/iflygpt/u/chat-list/v1/del-chat-list'
         headers = self.__headers.copy()
         headers['Content-Type'] = 'application/json;charset=UTF-8'
         _json = {'chatListId': chat_id}
 
-        response = self.post(url=url, headers=headers, _json=_json)
-
-        if not response:
-            return False
-
+        response = self.post(url=url, headers=headers, json=_json)
         return self.parse_data(response.json(), 'delete_chat') or False
 
     def get_chat_sid(self, chat_id: str) -> str:
         """
         通过会话id获取最新的机器人消息的sid；
         该值与chat_id一起确保了会话的上下文记忆
         新会话没有消息时，返回空字符串；
@@ -1291,15 +1251,15 @@
             'sid': self.get_chat_sid(chat_id),
             'GtToken': gt_token or self.gt_token,
             'clientType': client_type
         }
 
         response = self.post(url=url, headers=headers, data=data, stream=True)
 
-        if not response:
+        if response.status_code != 200:
             self.logger.error(f'【{self.model_name}】 ask failed, status_code: 【{response.status_code}】')
             return AiAnswer()
 
         self.single_answer = ''
         for line in response.iter_lines():
 
             if not line:
@@ -1355,20 +1315,15 @@
         data = {
             "searchValue": bot_name,
             "pageIndex": 1,
             "pageSize": 45,
             "botType": ""
         }
 
-        response = self.post(url=url, _json=data)
-
-        if not response:
-            self.logger.error(f'【{self.model_name}】 search_bot failed.')
-            return
-
+        response = self.post(url=url, json=data)
         return self.parse_data(response.json(), 'search_bot')
 
     def reset_bot(self, bot_id: str, chat_id: str):
         """
         【待完成】
         助手2.0重置话题
         """
@@ -1376,19 +1331,14 @@
 
         params = {
             'botId': bot_id,
             'chatId': chat_id
         }
 
         response = self.get(url=url, params=params)
-
-        if not response:
-            self.logger.error(f'【{self.model_name}】 reset_bot failed.')
-            return
-
         return response.text
 
     def get_gt_token(self):
         """
         【待完成】
         对于gt_token，经分析是极验的风控，定时将旧的gt_token更换
         但讯飞似乎并没有进行验证
```

## Comparing `zibuyu_LLM-0.1.11.dist-info/METADATA` & `zibuyu_LLM-0.1.9.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zibuyu-LLM
-Version: 0.1.11
+Version: 0.1.9
 Summary: 子不语个人工具包-LLM
 Author: 子不语
 License: MIT
 Keywords: LLM,zibuyu
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
@@ -37,18 +37,14 @@
 - 通义千问（Qwen）
 - 通义星辰（XinChen)
 - 通义万相（XinXiang）
 - 讯飞星火（Spark）
 
 # 版本记录
 
-`0.1.11`：修改讯飞星火请求出错判断
-
-`0.1.10`：修改bug
-
 `0.1.9`：讯飞星火部分添加自动鉴权
 
 `0.0.9`：修复由于类型注解引起的版本不兼容问题
 
 `0.0.8`：修复由于类型注解引起的版本不兼容问题
 
 `0.0.7`：统一各模型交互输出类型
```

## Comparing `zibuyu_LLM-0.1.11.dist-info/RECORD` & `zibuyu_LLM-0.1.9.dist-info/RECORD`

 * *Files 9% similar despite different names*

```diff
@@ -7,12 +7,12 @@
 zibuyu_llm_web/errors.py,sha256=Vib55tBOR1goqM7ddmx51TbJ8vKEXOCJEqcbvjTNaWw,732
 zibuyu_llm_web/kimi.py,sha256=kWj7tUqTOyFsbe60bFhg6dcNdzNKtDQ0kAIxEvSFvdU,9962
 zibuyu_llm_web/minmax.py,sha256=TUbX4Dzn3JP9vNYdYdeYzcZIJgBK-tySdypHQF12URc,37747
 zibuyu_llm_web/qwen.py,sha256=ja3fyFtY6bQmjCWNtcOtgMIRt6RSgtuYmNxDCQBk5oU,37730
 zibuyu_llm_web/types.py,sha256=a_kIEwO3gK8tHgHqfYOi7ug2qNK9s54PDjEdm1Z5ZKg,5308
 zibuyu_llm_web/wanxiang.py,sha256=YU9R42VaxWlY7gpcT_qAkguSqhCfDuK19-lpWaWgRDA,8118
 zibuyu_llm_web/xinchen.py,sha256=PTkPhh-S8gsWr6ULAvJV2E2kwBtO95lKohyxQiGA_hE,14705
-zibuyu_llm_web/xunfei.py,sha256=rhpCcb4bitoyhLMUeELxfLe-rP6yKbcsO4JmF_A4kk4,57022
-zibuyu_LLM-0.1.11.dist-info/METADATA,sha256=0Iu0jXzEc-9mhmdKEkn16cMG5G91-49oK8P0PA9BHYY,1697
-zibuyu_LLM-0.1.11.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
-zibuyu_LLM-0.1.11.dist-info/top_level.txt,sha256=QF6FI2Tcc78mYBpfy15YWDU-j16KK_2WqGF-3kj8Jew,30
-zibuyu_LLM-0.1.11.dist-info/RECORD,,
+zibuyu_llm_web/xunfei.py,sha256=3PtnE7Tv9Hs1r4AAUfPkGXnVmJIlEWB28h1JQ1_1sPo,55663
+zibuyu_LLM-0.1.9.dist-info/METADATA,sha256=4RikLUzMc_jtRXXy8MfEQ7W0a5aPZkASb55eRVJqOYU,1621
+zibuyu_LLM-0.1.9.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
+zibuyu_LLM-0.1.9.dist-info/top_level.txt,sha256=QF6FI2Tcc78mYBpfy15YWDU-j16KK_2WqGF-3kj8Jew,30
+zibuyu_LLM-0.1.9.dist-info/RECORD,,
```

