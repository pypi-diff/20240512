# Comparing `tmp/zibuyu_LLM-0.0.7-py3-none-any.whl.zip` & `tmp/zibuyu_LLM-0.0.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 60475 bytes, number of entries: 18
+Zip file size: 60606 bytes, number of entries: 18
 -rw-rw-rw-  2.0 fat      305 b- defN 24-May-11 08:41 zibuyu_llm_api/__init__.py
 -rw-rw-rw-  2.0 fat    31879 b- defN 24-May-11 08:41 zibuyu_llm_api/minmax_api.py
 -rw-rw-rw-  2.0 fat      735 b- defN 24-May-11 08:46 zibuyu_llm_web/__init__.py
--rw-rw-rw-  2.0 fat     7346 b- defN 24-May-11 13:34 zibuyu_llm_web/baichuan.py
+-rw-rw-rw-  2.0 fat     7376 b- defN 24-May-11 14:22 zibuyu_llm_web/baichuan.py
 -rw-rw-rw-  2.0 fat     7099 b- defN 24-May-11 01:45 zibuyu_llm_web/base.py
--rw-rw-rw-  2.0 fat    14836 b- defN 24-May-11 13:34 zibuyu_llm_web/deepseek.py
+-rw-rw-rw-  2.0 fat    14789 b- defN 24-May-11 14:25 zibuyu_llm_web/deepseek.py
 -rw-rw-rw-  2.0 fat      732 b- defN 24-May-11 08:49 zibuyu_llm_web/errors.py
--rw-rw-rw-  2.0 fat     9932 b- defN 24-May-11 13:34 zibuyu_llm_web/kimi.py
--rw-rw-rw-  2.0 fat    37682 b- defN 24-May-11 13:34 zibuyu_llm_web/minmax.py
+-rw-rw-rw-  2.0 fat     9962 b- defN 24-May-11 14:22 zibuyu_llm_web/kimi.py
+-rw-rw-rw-  2.0 fat    37747 b- defN 24-May-12 02:39 zibuyu_llm_web/minmax.py
 -rw-rw-rw-  2.0 fat    37730 b- defN 24-May-11 13:49 zibuyu_llm_web/qwen.py
--rw-rw-rw-  2.0 fat     5239 b- defN 24-May-11 13:49 zibuyu_llm_web/types.py
+-rw-rw-rw-  2.0 fat     5302 b- defN 24-May-12 03:06 zibuyu_llm_web/types.py
 -rw-rw-rw-  2.0 fat     8118 b- defN 24-May-11 08:37 zibuyu_llm_web/wanxiang.py
--rw-rw-rw-  2.0 fat    14675 b- defN 24-May-11 13:34 zibuyu_llm_web/xinchen.py
--rw-rw-rw-  2.0 fat    26122 b- defN 24-May-11 13:34 zibuyu_llm_web/xunfei.py
--rw-rw-rw-  2.0 fat     1435 b- defN 24-May-11 14:10 zibuyu_LLM-0.0.7.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-11 14:10 zibuyu_LLM-0.0.7.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       30 b- defN 24-May-11 14:10 zibuyu_LLM-0.0.7.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1455 b- defN 24-May-11 14:10 zibuyu_LLM-0.0.7.dist-info/RECORD
-18 files, 205442 bytes uncompressed, 58117 bytes compressed:  71.7%
+-rw-rw-rw-  2.0 fat    14705 b- defN 24-May-11 14:25 zibuyu_llm_web/xinchen.py
+-rw-rw-rw-  2.0 fat    26160 b- defN 24-May-12 01:33 zibuyu_llm_web/xunfei.py
+-rw-rw-rw-  2.0 fat     1503 b- defN 24-May-12 03:06 zibuyu_LLM-0.0.8.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-12 03:06 zibuyu_LLM-0.0.8.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       30 b- defN 24-May-12 03:06 zibuyu_LLM-0.0.8.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1455 b- defN 24-May-12 03:06 zibuyu_LLM-0.0.8.dist-info/RECORD
+18 files, 205719 bytes uncompressed, 58248 bytes compressed:  71.7%
```

## zipnote {}

```diff
@@ -36,20 +36,20 @@
 
 Filename: zibuyu_llm_web/xinchen.py
 Comment: 
 
 Filename: zibuyu_llm_web/xunfei.py
 Comment: 
 
-Filename: zibuyu_LLM-0.0.7.dist-info/METADATA
+Filename: zibuyu_LLM-0.0.8.dist-info/METADATA
 Comment: 
 
-Filename: zibuyu_LLM-0.0.7.dist-info/WHEEL
+Filename: zibuyu_LLM-0.0.8.dist-info/WHEEL
 Comment: 
 
-Filename: zibuyu_LLM-0.0.7.dist-info/top_level.txt
+Filename: zibuyu_LLM-0.0.8.dist-info/top_level.txt
 Comment: 
 
-Filename: zibuyu_LLM-0.0.7.dist-info/RECORD
+Filename: zibuyu_LLM-0.0.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## zibuyu_llm_web/baichuan.py

```diff
@@ -177,14 +177,15 @@
                 self.input_tokens += resp_json.get("usage", {}).get("prompt_tokens", 0)
                 self.output_tokens += resp_json.get("usage", {}).get("answer_tokens", 0)
 
         self.history.append({"from": 0, "data": question})
         self.history.append({"from": 1, "data": self.single_answer})
 
         self.single_answer_obj = AiAnswer(
+            is_success=True,
             content=self.single_answer
         )
 
         return self.single_answer_obj
 
     def get_session_list(self, page: int = 1, limit: int = 50) -> list[BaiChuanSession]:
```

## zibuyu_llm_web/deepseek.py

```diff
@@ -156,14 +156,21 @@
                         callback_func(self.end_signal)
                     except:
                         self.logger.error(f'回调函数【{callback_func.__name__}】执行失败', exc_info=True)
 
             if self.__single_padding:
                 self.__single_answer += self.__single_padding
 
+        self.single_answer_obj = AiAnswer(
+            content=self.__single_answer,
+            is_success=True,
+        )
+
+        return self.single_answer_obj
+
     def __get_history(self, model: str, referer: str) -> dict:
         uri = '/api/v0/chat/history'
 
         params = {
             'model_class': model,
             'filter_server_error': True,
             'forward_query': False,
@@ -269,34 +276,26 @@
         代码助手
         :param question:
         :param callback_func:
         :return:
         """
 
         model = "deepseek_code"
-        self.__ask(question, model, callback_func=callback_func)
-
-        self.single_answer_obj = AiAnswer(content=self.__single_answer)
-
-        return self.single_answer_obj
+        return self.__ask(question, model, callback_func=callback_func)
 
     def ask(self, question: str, callback_func=None) -> AiAnswer:
         """
         通用助手
         :param question:
         :param callback_func:
         :return:
         """
 
         model = "deepseek_chat"
-        self.__ask(question, model, callback_func=callback_func)
-
-        self.single_answer_obj = AiAnswer(content=self.__single_answer)
-
-        return self.single_answer_obj
+        return self.__ask(question, model, callback_func=callback_func)
 
     def get_chat_history(self):
         """
         获取通用助手聊天记录
         :return:
         """
```

## zibuyu_llm_web/kimi.py

```diff
@@ -252,14 +252,15 @@
 
             elif event == 'all_done':
                 if callable(callback_func):
                     callback_func(self.end_signal)
 
         # 封装回答
         self.single_answer_obj = AiAnswer(
+            is_success=True,
             content=self.single_answer,
             conversation_id=self.chat_id,
             reference_link_list=self.single_answer_url_list
         )
 
         return self.single_answer_obj
```

## zibuyu_llm_web/minmax.py

```diff
@@ -658,14 +658,15 @@
         """服务端返回最后总结信息"""
 
         self.single_answer = data.get('data', {}).get('messageResult', {}).get('content')
 
         reference_link_list = data.get('data', {}).get('extra', {}).get('netSearchStatus', {}).get('linkDetail', [])
 
         answer_obj = AiAnswer(
+            is_success=True,
             content=self.single_answer,
             conversation_id=self.chat_id,
             reference_link_list=[ReferenceLink(
                 title=item['detail'],
                 url=item['url'],
             ) for item in reference_link_list]
         )
@@ -925,25 +926,25 @@
         except:
             self.logger.error(f"发送验证码失败")
 
     def login(
             self,
             phone: str,
             sms_code: str,
-    ) -> str:
+    ) -> bool:
         """
         登录
         :param phone: 手机号
         :param sms_code: 手机验证码
         :return: 登录成功时返回获取到的Token
         """
 
         if len(sms_code) != 6:
             self.logger.error(f"验证码长度错误")
-            return ''
+            return False
 
         uri = '/v1/api/user/login/phone'
 
         data = {
             "phone": phone,
             "code": sms_code,
             "loginType": ""
@@ -970,28 +971,29 @@
             )
 
             response_data = response.json()
 
             status_code = response_data.get('statusInfo', {}).get('code')
             if status_code != 0:
                 self.logger.error(f"登录失败")
-                return ''
+                return False
 
             self.logger.info(f"登录成功，已获取到Token")
             token = response_data.get('data', {}).get('token')
 
             if not token:
                 self.logger.error(f"登录失败")
-                return ''
+                return False
 
             self.token_str = token
-            return token
+            return True
 
         except:
             self.logger.error(f"登录失败")
+            return False
 
     def test(self):
         unix = '1715264091000'
 
         user_data = {
             'msgID': 244977956405796869,
             'timbre': "male-botong",
```

## zibuyu_llm_web/types.py

```diff
@@ -5,15 +5,16 @@
 project: zibuyu_LLM
 author: 子不语
 date: 2024/4/26
 contact: 【公众号】思维兵工厂
 description: 
 --------------------------------------------
 """
-from typing import Literal, Optional
+
+from typing import Literal, Optional, Union
 from dataclasses import dataclass
 
 
 # #################### 公用模型类 ####################
 
 @dataclass
 class ReferenceLink:
@@ -24,14 +25,15 @@
 
 
 @dataclass
 class AiAnswer:
     """AI回复"""
 
     content: str = ''
+    is_success: bool = False
     latest_msg_id: str = ''  # 上一次消息id，有些AI需要用到
     conversation_id: str = ''  # 会话id，不同AI的称呼可能不同，这里统一为conversation_id
     audio_path_list: list[str] = None
     reference_link_list: Optional[list[ReferenceLink]] = None
 
 
 # #################### ####################
@@ -69,22 +71,22 @@
 class QwenWebResponse:
     """通义千问 - 对话响应模版 """
 
     content_type: Literal["text", "text2image",]
     content_from: Literal["text", "text2image",]
 
     # 回应内容列表，可能包含插件搜索结果、相关网页链接等
-    content_list: list[QwenChatContent] | None
+    content_list: Union[list[QwenChatContent], None]
 
     # 插件类型特有字段
-    web_search_list: list[QwenPluginWebSearchResult] | None
-    reference_link_list: list[ReferenceLink] | None
+    web_search_list: Union[list[QwenPluginWebSearchResult], None]
+    reference_link_list: Union[list[ReferenceLink], None]
 
     # 文生图特有字段，存储图片地址
-    image_url_list: list[str] | None
+    image_url_list: Union[list[str], None]
 
     msg_id: str
     parent_msg_id: str
     session_id: str
     msg_status: str
     params: dict
     stop_reason: dict
```

## zibuyu_llm_web/xinchen.py

```diff
@@ -180,14 +180,15 @@
 
                 all_data = f"{host}\n\n{json.dumps(data)}\n\n{request_response}\n\n{traceback_info}"
                 file_path = self.save_bad_request_data('AI交互出现未知错误', all_data)
 
                 self.logger.error(f"AI交互出现未知错误，请求相关数据已保存于：{file_path}")
 
         self.single_answer_obj = AiAnswer(
+            is_success=True,
             content=self.single_answer
         )
         return self.single_answer_obj
 
     def get_history(self, chat_room_id: str) -> XincChatHistory:
         """
         根据room_id获取会话历史
```

## zibuyu_llm_web/xunfei.py

```diff
@@ -379,15 +379,15 @@
             'clientType': client_type
         }
 
         response = self.post(url=url, headers=headers, data=data, stream=True)
 
         if response.status_code != 200:
             self.logger.error(f'【{self.model_name}】 ask failed, status_code: 【{response.status_code}】')
-            return ''
+            return AiAnswer()
 
         self.single_answer = ''
         for line in response.iter_lines():
 
             if not line:
                 continue
 
@@ -423,14 +423,15 @@
                     try:
                         callback_func('<<<end>>>')
                     except Exception as e:
                         self.logger.error(f"回调函数执行出错: {e}", exc_info=True)
 
         self.single_answer_obj = AiAnswer(
             content=self.single_answer,
+            is_success=True,
             conversation_id=chat_id,
         )
 
         return self.single_answer_obj
 
     def search_bot(self, bot_name: str):
         """根据名称搜索助手"""
```

## Comparing `zibuyu_LLM-0.0.7.dist-info/METADATA` & `zibuyu_LLM-0.0.8.dist-info/METADATA`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zibuyu-LLM
-Version: 0.0.7
+Version: 0.0.8
 Summary: 子不语个人工具包-LLM
 Author: 子不语
 License: MIT
 Keywords: LLM,zibuyu
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
@@ -37,14 +37,16 @@
 - 通义千问（Qwen）
 - 通义星辰（XinChen)
 - 通义万相（XinXiang）
 - 讯飞星火（Spark）
 
 # 版本记录
 
+`0.0.8`：修复由于类型注解引起的版本不兼容问题
+
 `0.0.7`：统一各模型交互输出类型
 
 `0.0.6`：修改讯飞星火调用的传值
 
 `0.0.5`：增加error与types模块
 
 `0.0.4`：修复导包路径问题
```

## Comparing `zibuyu_LLM-0.0.7.dist-info/RECORD` & `zibuyu_LLM-0.0.8.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 zibuyu_llm_api/__init__.py,sha256=Ox3V8_X8l52LqJ_ATAWv0xpxBZxq5o1xn16TcEvSUl4,305
 zibuyu_llm_api/minmax_api.py,sha256=6gZMHkmSfwsmbFtjkJF2W9uUX35zmdk1vLwIlcUuOJo,31879
 zibuyu_llm_web/__init__.py,sha256=1YEBJuq9b5XG8jUOtgdrMNDiSiHZ9_OCT6PxH_xDoiY,735
-zibuyu_llm_web/baichuan.py,sha256=vqR3gupplB6y0c8BE6T2IxhSR5mwgeqSqCEmGsazO-c,7346
+zibuyu_llm_web/baichuan.py,sha256=lFq8jX7VwTBqB9EP31-H1Zj-WIiDWD4JScVMiq9yxUA,7376
 zibuyu_llm_web/base.py,sha256=s7GYbP70kKt7nhMLK0Jp22gVu2EfmS30eA5b6k_aYa8,7099
-zibuyu_llm_web/deepseek.py,sha256=PZH6kUYeHG75YRTqqm1SctBuMwZ-SQth2q5x2W9ltrA,14836
+zibuyu_llm_web/deepseek.py,sha256=b7buJU59WMri4qqulb_T2HuBEqsTtkoulI9M4aPRzpc,14789
 zibuyu_llm_web/errors.py,sha256=Vib55tBOR1goqM7ddmx51TbJ8vKEXOCJEqcbvjTNaWw,732
-zibuyu_llm_web/kimi.py,sha256=6DaC8HXY0a8XV64HVX1Cqs9xeUcccGzpExSQttzs2BU,9932
-zibuyu_llm_web/minmax.py,sha256=X9VFPbKkth37-9noccCfEHL1gvLj5DjsGobZJ04gNmo,37682
+zibuyu_llm_web/kimi.py,sha256=kWj7tUqTOyFsbe60bFhg6dcNdzNKtDQ0kAIxEvSFvdU,9962
+zibuyu_llm_web/minmax.py,sha256=TUbX4Dzn3JP9vNYdYdeYzcZIJgBK-tySdypHQF12URc,37747
 zibuyu_llm_web/qwen.py,sha256=ja3fyFtY6bQmjCWNtcOtgMIRt6RSgtuYmNxDCQBk5oU,37730
-zibuyu_llm_web/types.py,sha256=FfDmEsUiL9HpbwWKuFqBSTbkcuCVXQTEQCl5vYQ5p0E,5239
+zibuyu_llm_web/types.py,sha256=9wqxlqi3llDAcUKRfpTJfliE49hyc1dTHBq-Yp5r1Ps,5302
 zibuyu_llm_web/wanxiang.py,sha256=YU9R42VaxWlY7gpcT_qAkguSqhCfDuK19-lpWaWgRDA,8118
-zibuyu_llm_web/xinchen.py,sha256=abCJmbjcFgFc6UjJng8c9D33qMn4hwWrUg4cT2N9-no,14675
-zibuyu_llm_web/xunfei.py,sha256=mtiEh5Uj0jz46t8QcWIvnEoXACEHT7hbX8hCU-uIOPA,26122
-zibuyu_LLM-0.0.7.dist-info/METADATA,sha256=UFRbHtSnzYCfzQbe4_WAWOqNwVBFMX2Gj8kvzWOpkyw,1435
-zibuyu_LLM-0.0.7.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
-zibuyu_LLM-0.0.7.dist-info/top_level.txt,sha256=QF6FI2Tcc78mYBpfy15YWDU-j16KK_2WqGF-3kj8Jew,30
-zibuyu_LLM-0.0.7.dist-info/RECORD,,
+zibuyu_llm_web/xinchen.py,sha256=PTkPhh-S8gsWr6ULAvJV2E2kwBtO95lKohyxQiGA_hE,14705
+zibuyu_llm_web/xunfei.py,sha256=gHBQvLI998W-flOqi6aB1vs_AQqurc2PWTB5u2tfGnI,26160
+zibuyu_LLM-0.0.8.dist-info/METADATA,sha256=2Keb1F8YF-Z1Ae7aupGlvCGNJ7QYnAaVFp0PKU4e6V0,1503
+zibuyu_LLM-0.0.8.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
+zibuyu_LLM-0.0.8.dist-info/top_level.txt,sha256=QF6FI2Tcc78mYBpfy15YWDU-j16KK_2WqGF-3kj8Jew,30
+zibuyu_LLM-0.0.8.dist-info/RECORD,,
```

