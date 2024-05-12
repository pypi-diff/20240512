# Comparing `tmp/zibuyu_LLM-0.0.8-py3-none-any.whl.zip` & `tmp/zibuyu_LLM-0.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -5,16 +5,16 @@
 -rw-rw-rw-  2.0 fat     7376 b- defN 24-May-11 14:22 zibuyu_llm_web/baichuan.py
 -rw-rw-rw-  2.0 fat     7099 b- defN 24-May-11 01:45 zibuyu_llm_web/base.py
 -rw-rw-rw-  2.0 fat    14789 b- defN 24-May-11 14:25 zibuyu_llm_web/deepseek.py
 -rw-rw-rw-  2.0 fat      732 b- defN 24-May-11 08:49 zibuyu_llm_web/errors.py
 -rw-rw-rw-  2.0 fat     9962 b- defN 24-May-11 14:22 zibuyu_llm_web/kimi.py
 -rw-rw-rw-  2.0 fat    37747 b- defN 24-May-12 02:39 zibuyu_llm_web/minmax.py
 -rw-rw-rw-  2.0 fat    37730 b- defN 24-May-11 13:49 zibuyu_llm_web/qwen.py
--rw-rw-rw-  2.0 fat     5302 b- defN 24-May-12 03:06 zibuyu_llm_web/types.py
+-rw-rw-rw-  2.0 fat     5308 b- defN 24-May-12 03:43 zibuyu_llm_web/types.py
 -rw-rw-rw-  2.0 fat     8118 b- defN 24-May-11 08:37 zibuyu_llm_web/wanxiang.py
 -rw-rw-rw-  2.0 fat    14705 b- defN 24-May-11 14:25 zibuyu_llm_web/xinchen.py
 -rw-rw-rw-  2.0 fat    26160 b- defN 24-May-12 01:33 zibuyu_llm_web/xunfei.py
--rw-rw-rw-  2.0 fat     1503 b- defN 24-May-12 03:06 zibuyu_LLM-0.0.8.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-12 03:06 zibuyu_LLM-0.0.8.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       30 b- defN 24-May-12 03:06 zibuyu_LLM-0.0.8.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1455 b- defN 24-May-12 03:06 zibuyu_LLM-0.0.8.dist-info/RECORD
-18 files, 205719 bytes uncompressed, 58248 bytes compressed:  71.7%
+-rw-rw-rw-  2.0 fat     1571 b- defN 24-May-12 03:43 zibuyu_LLM-0.0.9.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-12 03:43 zibuyu_LLM-0.0.9.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       30 b- defN 24-May-12 03:43 zibuyu_LLM-0.0.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1455 b- defN 24-May-12 03:43 zibuyu_LLM-0.0.9.dist-info/RECORD
+18 files, 205793 bytes uncompressed, 58248 bytes compressed:  71.7%
```

## zipnote {}

```diff
@@ -36,20 +36,20 @@
 
 Filename: zibuyu_llm_web/xinchen.py
 Comment: 
 
 Filename: zibuyu_llm_web/xunfei.py
 Comment: 
 
-Filename: zibuyu_LLM-0.0.8.dist-info/METADATA
+Filename: zibuyu_LLM-0.0.9.dist-info/METADATA
 Comment: 
 
-Filename: zibuyu_LLM-0.0.8.dist-info/WHEEL
+Filename: zibuyu_LLM-0.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: zibuyu_LLM-0.0.8.dist-info/top_level.txt
+Filename: zibuyu_LLM-0.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: zibuyu_LLM-0.0.8.dist-info/RECORD
+Filename: zibuyu_LLM-0.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## zibuyu_llm_web/types.py

```diff
@@ -112,15 +112,15 @@
 
     session_id: str
     msg_id: str
     parent_msg_id: str
 
     msg_status: str  # 会话状态：是否完整生成
 
-    content_list: list[QwenChatContent] | None
+    content_list: Union[list[QwenChatContent], None]
 
     interrupted: bool = False  # AI生成内容时是否被打断
     ai_disclaimer: bool = False
     can_regenerate: bool = True
     can_share: bool = True
     can_show: bool = True
```

## Comparing `zibuyu_LLM-0.0.8.dist-info/METADATA` & `zibuyu_LLM-0.0.9.dist-info/METADATA`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zibuyu-LLM
-Version: 0.0.8
+Version: 0.0.9
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
 
+`0.0.9`：修复由于类型注解引起的版本不兼容问题
+
 `0.0.8`：修复由于类型注解引起的版本不兼容问题
 
 `0.0.7`：统一各模型交互输出类型
 
 `0.0.6`：修改讯飞星火调用的传值
 
 `0.0.5`：增加error与types模块
```

## Comparing `zibuyu_LLM-0.0.8.dist-info/RECORD` & `zibuyu_LLM-0.0.9.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 zibuyu_llm_web/baichuan.py,sha256=lFq8jX7VwTBqB9EP31-H1Zj-WIiDWD4JScVMiq9yxUA,7376
 zibuyu_llm_web/base.py,sha256=s7GYbP70kKt7nhMLK0Jp22gVu2EfmS30eA5b6k_aYa8,7099
 zibuyu_llm_web/deepseek.py,sha256=b7buJU59WMri4qqulb_T2HuBEqsTtkoulI9M4aPRzpc,14789
 zibuyu_llm_web/errors.py,sha256=Vib55tBOR1goqM7ddmx51TbJ8vKEXOCJEqcbvjTNaWw,732
 zibuyu_llm_web/kimi.py,sha256=kWj7tUqTOyFsbe60bFhg6dcNdzNKtDQ0kAIxEvSFvdU,9962
 zibuyu_llm_web/minmax.py,sha256=TUbX4Dzn3JP9vNYdYdeYzcZIJgBK-tySdypHQF12URc,37747
 zibuyu_llm_web/qwen.py,sha256=ja3fyFtY6bQmjCWNtcOtgMIRt6RSgtuYmNxDCQBk5oU,37730
-zibuyu_llm_web/types.py,sha256=9wqxlqi3llDAcUKRfpTJfliE49hyc1dTHBq-Yp5r1Ps,5302
+zibuyu_llm_web/types.py,sha256=a_kIEwO3gK8tHgHqfYOi7ug2qNK9s54PDjEdm1Z5ZKg,5308
 zibuyu_llm_web/wanxiang.py,sha256=YU9R42VaxWlY7gpcT_qAkguSqhCfDuK19-lpWaWgRDA,8118
 zibuyu_llm_web/xinchen.py,sha256=PTkPhh-S8gsWr6ULAvJV2E2kwBtO95lKohyxQiGA_hE,14705
 zibuyu_llm_web/xunfei.py,sha256=gHBQvLI998W-flOqi6aB1vs_AQqurc2PWTB5u2tfGnI,26160
-zibuyu_LLM-0.0.8.dist-info/METADATA,sha256=2Keb1F8YF-Z1Ae7aupGlvCGNJ7QYnAaVFp0PKU4e6V0,1503
-zibuyu_LLM-0.0.8.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
-zibuyu_LLM-0.0.8.dist-info/top_level.txt,sha256=QF6FI2Tcc78mYBpfy15YWDU-j16KK_2WqGF-3kj8Jew,30
-zibuyu_LLM-0.0.8.dist-info/RECORD,,
+zibuyu_LLM-0.0.9.dist-info/METADATA,sha256=hb8icx4zePAX4eC2niIzgid1jLa-nr-9AXsDCuuLjfU,1571
+zibuyu_LLM-0.0.9.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
+zibuyu_LLM-0.0.9.dist-info/top_level.txt,sha256=QF6FI2Tcc78mYBpfy15YWDU-j16KK_2WqGF-3kj8Jew,30
+zibuyu_LLM-0.0.9.dist-info/RECORD,,
```

