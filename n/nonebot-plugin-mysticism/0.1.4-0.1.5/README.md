# Comparing `tmp/nonebot_plugin_mysticism-0.1.4.tar.gz` & `tmp/nonebot_plugin_mysticism-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_mysticism-0.1.4.tar", max compression
+gzip compressed data, was "nonebot_plugin_mysticism-0.1.5.tar", max compression
```

## Comparing `nonebot_plugin_mysticism-0.1.4.tar` & `nonebot_plugin_mysticism-0.1.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    11332 2024-05-09 15:03:26.870225 nonebot_plugin_mysticism-0.1.4/LICENSE
--rw-r--r--   0        0        0     2483 2024-05-09 15:03:26.870225 nonebot_plugin_mysticism-0.1.4/README.md
--rw-r--r--   0        0        0      466 2024-05-09 15:03:26.870225 nonebot_plugin_mysticism-0.1.4/nonebot_plugin_mysticism/__init__.py
--rw-r--r--   0        0        0      158 2024-05-09 15:03:26.870225 nonebot_plugin_mysticism-0.1.4/nonebot_plugin_mysticism/config.py
--rw-r--r--   0        0        0      702 2024-05-09 15:03:26.870225 nonebot_plugin_mysticism-0.1.4/nonebot_plugin_mysticism/rule.py
--rw-r--r--   0        0        0     6350 2024-05-09 15:03:26.870225 nonebot_plugin_mysticism-0.1.4/nonebot_plugin_mysticism/tarot.py
--rw-r--r--   0        0        0     3611 2024-05-09 15:03:26.870225 nonebot_plugin_mysticism-0.1.4/nonebot_plugin_mysticism/tarot_formations.yaml
--rw-r--r--   0        0        0    11099 2024-05-09 15:03:26.870225 nonebot_plugin_mysticism-0.1.4/nonebot_plugin_mysticism/tarot_keywords.yml
--rw-r--r--   0        0        0        0 2024-05-09 15:03:26.870225 nonebot_plugin_mysticism-0.1.4/nonebot_plugin_mysticism/tarot_theme/__init__.py
--rw-r--r--   0        0        0     3327 2024-05-09 15:03:26.870225 nonebot_plugin_mysticism-0.1.4/nonebot_plugin_mysticism/tarot_theme/bilibili.yaml
--rw-r--r--   0        0        0      774 2024-05-09 15:03:26.870225 nonebot_plugin_mysticism-0.1.4/nonebot_plugin_mysticism/tarot_theme/blue_archive.yaml
--rw-r--r--   0        0        0     2120 2024-05-09 15:03:26.870225 nonebot_plugin_mysticism-0.1.4/nonebot_plugin_mysticism/tarot_theme/waite.yaml
--rw-r--r--   0        0        0    11221 2024-05-09 15:03:26.870225 nonebot_plugin_mysticism-0.1.4/nonebot_plugin_mysticism/tarot_uitls.py
--rw-r--r--   0        0        0     1043 2024-05-09 15:03:26.870225 nonebot_plugin_mysticism-0.1.4/nonebot_plugin_mysticism/utils.py
--rw-r--r--   0        0        0      555 2024-05-09 15:03:26.870225 nonebot_plugin_mysticism-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     3247 1970-01-01 00:00:00.000000 nonebot_plugin_mysticism-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0    11332 2024-05-12 07:33:51.714149 nonebot_plugin_mysticism-0.1.5/LICENSE
+-rw-r--r--   0        0        0     2483 2024-05-12 07:33:51.714149 nonebot_plugin_mysticism-0.1.5/README.md
+-rw-r--r--   0        0        0      465 2024-05-12 07:33:51.718149 nonebot_plugin_mysticism-0.1.5/nonebot_plugin_mysticism/__init__.py
+-rw-r--r--   0        0        0      109 2024-05-12 07:33:51.718149 nonebot_plugin_mysticism-0.1.5/nonebot_plugin_mysticism/config.py
+-rw-r--r--   0        0        0      702 2024-05-12 07:33:51.718149 nonebot_plugin_mysticism-0.1.5/nonebot_plugin_mysticism/rule.py
+-rw-r--r--   0        0        0     6572 2024-05-12 07:33:51.718149 nonebot_plugin_mysticism-0.1.5/nonebot_plugin_mysticism/tarot.py
+-rw-r--r--   0        0        0     3611 2024-05-12 07:33:51.718149 nonebot_plugin_mysticism-0.1.5/nonebot_plugin_mysticism/tarot_formations.yaml
+-rw-r--r--   0        0        0    11099 2024-05-12 07:33:51.718149 nonebot_plugin_mysticism-0.1.5/nonebot_plugin_mysticism/tarot_keywords.yml
+-rw-r--r--   0        0        0        0 2024-05-12 07:33:51.718149 nonebot_plugin_mysticism-0.1.5/nonebot_plugin_mysticism/tarot_theme/__init__.py
+-rw-r--r--   0        0        0     3327 2024-05-12 07:33:51.718149 nonebot_plugin_mysticism-0.1.5/nonebot_plugin_mysticism/tarot_theme/bilibili.yaml
+-rw-r--r--   0        0        0      774 2024-05-12 07:33:51.718149 nonebot_plugin_mysticism-0.1.5/nonebot_plugin_mysticism/tarot_theme/blue_archive.yaml
+-rw-r--r--   0        0        0     2120 2024-05-12 07:33:51.718149 nonebot_plugin_mysticism-0.1.5/nonebot_plugin_mysticism/tarot_theme/waite.yaml
+-rw-r--r--   0        0        0    11242 2024-05-12 07:33:51.718149 nonebot_plugin_mysticism-0.1.5/nonebot_plugin_mysticism/tarot_uitls.py
+-rw-r--r--   0        0        0     1043 2024-05-12 07:33:51.718149 nonebot_plugin_mysticism-0.1.5/nonebot_plugin_mysticism/utils.py
+-rw-r--r--   0        0        0      555 2024-05-12 07:33:51.718149 nonebot_plugin_mysticism-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     3247 1970-01-01 00:00:00.000000 nonebot_plugin_mysticism-0.1.5/PKG-INFO
```

### Comparing `nonebot_plugin_mysticism-0.1.4/LICENSE` & `nonebot_plugin_mysticism-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mysticism-0.1.4/README.md` & `nonebot_plugin_mysticism-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mysticism-0.1.4/nonebot_plugin_mysticism/rule.py` & `nonebot_plugin_mysticism-0.1.5/nonebot_plugin_mysticism/rule.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mysticism-0.1.4/nonebot_plugin_mysticism/tarot.py` & `nonebot_plugin_mysticism-0.1.5/nonebot_plugin_mysticism/tarot.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 import yaml
 import pathlib
 import random
+from nonebot import get_plugin_config
 from nonebot.adapters import Bot
 from PIL import Image
 from nonebot import on_command
 from nonebot.params import CommandArg
 from nonebot.params import ArgPlainText
-from nonebot.adapters.onebot.v11.message import Message as V11Msg
 from nonebot.adapters.onebot.v11.event import GroupMessageEvent as V11G
 from nonebot.adapters.onebot.v11.message import MessageSegment as V11Seg
 from nonebot.internal.adapter import Bot
 from nonebot.matcher import Matcher
 from nonebot.typing import T_State
 from io import BytesIO
+
 from .utils import send_image_as_bytes
+from .config import Config
 from . import tarot_uitls
 
+p_config = get_plugin_config(Config)
+
 FORMATIONS = None
 FORMATIONS_ALIAS = None
 with open(
     pathlib.Path(__file__).parent / "tarot_formations.yaml", encoding="utf-8"
 ) as f:
     data = yaml.load(f, yaml.FullLoader)
     FORMATIONS = data["formations"]
@@ -39,15 +43,17 @@
     if formations not in FORMATIONS:
         formations = random.choice(list(FORMATIONS.keys()))
         result = "牌阵没有找到喵。\n"
 
     state["formations"] = FORMATIONS[formations]
     state["cards_num"] = state["formations"]["cards_num"]
     state["cnumber"] = []
-    state["tarot_theme"] = random.choice(tarot_uitls.THEME)
+    state["tarot_theme"] = tarot_uitls.THEME.get(
+        p_config.tarot_theme, random.choice(tarot_uitls.THEME)
+    )
     state["stack_card"] = tarot_uitls.TAROT_STACK.copy()
     random.shuffle(state["stack_card"])
     # 先洗牌更有仪式感（x）
 
     result += f"目前抽取到了：{formations}\n"
     result += f'所以接下来请发送 {state["cards_num"]} 个 1-78 的数字。\n'
     result += f"(注：其实不是1-78也行，我取模了（？）)\n"
@@ -67,15 +73,15 @@
             sep = "."
         for i in map(lambda x: x % 78, map(int, nums.split(sep=sep))):
             if i in state["cnumber"]:
                 continue
             state["cnumber"].append(i)
     except:
         await tarot.reject(
-            f"似乎，这些不只是数字……\n你还得再输入 {state['cards_num']} 个数字"
+            f"似乎，这些不只是数字……\n你还得再输入 {state['cards_num']-len(state['cnumber'])} 个数字"
         )
 
     if state["cards_num"] > len(state["cnumber"]):
         await tarot.reject(
             f"你还得再输入 {state['cards_num']-len(state['cnumber'])} 个数字"
         )
 
@@ -172,15 +178,17 @@
         args = NUM2ID.get(args, "")
     except:
         args = ""
 
     _id = random.choice(
         list(filter(lambda x: x.startswith(args), tarot_uitls.TAROT_STACK))
     )
-
+    theme = tarot_uitls.THEME.get(
+        p_config.tarot_theme, random.choice(tarot_uitls.THEME)
+    )
     theme = random.choice(tarot_uitls.THEME)
     img = Image.open(await send_image_as_bytes(theme[_id].face_url))
     postfix = f"「{tarot_uitls.CN_Name[_id]} 正位」"
     if random.randint(0, 1) == 1:
         img = img.transpose(Image.ROTATE_180)
         postfix = f"「{tarot_uitls.CN_Name[_id]} 逆位」"
     image = BytesIO()
```

### Comparing `nonebot_plugin_mysticism-0.1.4/nonebot_plugin_mysticism/tarot_formations.yaml` & `nonebot_plugin_mysticism-0.1.5/nonebot_plugin_mysticism/tarot_formations.yaml`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mysticism-0.1.4/nonebot_plugin_mysticism/tarot_keywords.yml` & `nonebot_plugin_mysticism-0.1.5/nonebot_plugin_mysticism/tarot_keywords.yml`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mysticism-0.1.4/nonebot_plugin_mysticism/tarot_theme/bilibili.yaml` & `nonebot_plugin_mysticism-0.1.5/nonebot_plugin_mysticism/tarot_theme/bilibili.yaml`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mysticism-0.1.4/nonebot_plugin_mysticism/tarot_theme/blue_archive.yaml` & `nonebot_plugin_mysticism-0.1.5/nonebot_plugin_mysticism/tarot_theme/blue_archive.yaml`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mysticism-0.1.4/nonebot_plugin_mysticism/tarot_theme/waite.yaml` & `nonebot_plugin_mysticism-0.1.5/nonebot_plugin_mysticism/tarot_theme/waite.yaml`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mysticism-0.1.4/nonebot_plugin_mysticism/tarot_uitls.py` & `nonebot_plugin_mysticism-0.1.5/nonebot_plugin_mysticism/tarot_uitls.py`

 * *Files 0% similar despite different names*

```diff
@@ -233,15 +233,15 @@
 
 WAITE = get_tarot(pathlib.Path(__file__).parent / "tarot_theme" / "waite.yaml")
 BULE_ARCHIVE = get_tarot(
     pathlib.Path(__file__).parent / "tarot_theme" / "blue_archive.yaml"
 )
 
 
-THEME = [BILIBILI, BULE_ARCHIVE, WAITE]
+THEME = {v.name: v for v in [BILIBILI, BULE_ARCHIVE, WAITE]}
 
 TAROT_STACK = [
     "cups.ace",
     "cups.two",
     "cups.three",
     "cups.four",
     "cups.five",
```

### Comparing `nonebot_plugin_mysticism-0.1.4/nonebot_plugin_mysticism/utils.py` & `nonebot_plugin_mysticism-0.1.5/nonebot_plugin_mysticism/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mysticism-0.1.4/pyproject.toml` & `nonebot_plugin_mysticism-0.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-mysticism"
-version = "0.1.4"
+version = "0.1.5"
 description = "占卜辅助工具"
 authors = ["Yan <1964649083@qq.com>"]
 license = "Apache License 2.0"
 readme = "README.md"
 
 keywords = ["tarot", "nonebot", "nonebot2", "bot", "qq"]
 homepage = "https://github.com/Yan-Zero/nonebot_plugin_mysticism"
```

### Comparing `nonebot_plugin_mysticism-0.1.4/PKG-INFO` & `nonebot_plugin_mysticism-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-mysticism
-Version: 0.1.4
+Version: 0.1.5
 Summary: 占卜辅助工具
 Home-page: https://github.com/Yan-Zero/nonebot_plugin_mysticism
 License: Apache-2.0
 Keywords: tarot,nonebot,nonebot2,bot,qq
 Author: Yan
 Author-email: 1964649083@qq.com
 Requires-Python: >=3.11,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-mysticism Version: 0.1.4 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-mysticism Version: 0.1.5 Summary:
 å åè¾å©å·¥å· Home-page: https://github.com/Yan-Zero/
 nonebot_plugin_mysticism License: Apache-2.0 Keywords:
 tarot,nonebot,nonebot2,bot,qq Author: Yan Author-email: 1964649083@qq.com
 Requires-Python: >=3.11,<4.0 Classifier: License :: OSI Approved :: Apache
 Software License Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
 Python :: 3.12 Requires-Dist: aiohttp (>=3.9.5,<4.0.0) Requires-Dist: nonebot-
```

