# Comparing `tmp/nonebot_plugin_ranfurrypic-1.1.5.tar.gz` & `tmp/nonebot_plugin_ranfurrypic-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_ranfurrypic-1.1.5.tar", last modified: Sun May 12 02:09:52 2024, max compression
+gzip compressed data, was "nonebot_plugin_ranfurrypic-1.1.6.tar", last modified: Sun May 12 02:51:56 2024, max compression
```

## Comparing `nonebot_plugin_ranfurrypic-1.1.5.tar` & `nonebot_plugin_ranfurrypic-1.1.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-12 02:09:52.557617 nonebot_plugin_ranfurrypic-1.1.5/
--rw-rw-rw-   0        0        0     1082 2024-05-10 14:34:54.000000 nonebot_plugin_ranfurrypic-1.1.5/LICENSE
--rw-rw-rw-   0        0        0     2828 2024-05-12 02:09:52.556648 nonebot_plugin_ranfurrypic-1.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     2461 2024-05-12 02:08:44.000000 nonebot_plugin_ranfurrypic-1.1.5/README.md
-drwxrwxrwx   0        0        0        0 2024-05-12 02:09:52.524638 nonebot_plugin_ranfurrypic-1.1.5/nonebot_plugin_RanFurryPic/
--rw-rw-rw-   0        0        0     3145 2024-05-11 15:52:58.000000 nonebot_plugin_ranfurrypic-1.1.5/nonebot_plugin_RanFurryPic/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-12 02:09:52.554622 nonebot_plugin_ranfurrypic-1.1.5/nonebot_plugin_RanFurryPic.egg-info/
--rw-rw-rw-   0        0        0     2828 2024-05-12 02:09:52.000000 nonebot_plugin_ranfurrypic-1.1.5/nonebot_plugin_RanFurryPic.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      320 2024-05-12 02:09:52.000000 nonebot_plugin_ranfurrypic-1.1.5/nonebot_plugin_RanFurryPic.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-12 02:09:52.000000 nonebot_plugin_ranfurrypic-1.1.5/nonebot_plugin_RanFurryPic.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2024-05-12 02:09:52.000000 nonebot_plugin_ranfurrypic-1.1.5/nonebot_plugin_RanFurryPic.egg-info/requires.txt
--rw-rw-rw-   0        0        0       27 2024-05-12 02:09:52.000000 nonebot_plugin_ranfurrypic-1.1.5/nonebot_plugin_RanFurryPic.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      380 2024-05-12 02:09:00.000000 nonebot_plugin_ranfurrypic-1.1.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-12 02:09:52.557617 nonebot_plugin_ranfurrypic-1.1.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-12 02:51:56.378185 nonebot_plugin_ranfurrypic-1.1.6/
+-rw-rw-rw-   0        0        0     1082 2024-05-10 14:34:54.000000 nonebot_plugin_ranfurrypic-1.1.6/LICENSE
+-rw-rw-rw-   0        0        0     2828 2024-05-12 02:51:56.377186 nonebot_plugin_ranfurrypic-1.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2461 2024-05-12 02:08:44.000000 nonebot_plugin_ranfurrypic-1.1.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-12 02:51:56.362195 nonebot_plugin_ranfurrypic-1.1.6/nonebot_plugin_RanFurryPic/
+-rw-rw-rw-   0        0        0     3131 2024-05-12 02:50:52.000000 nonebot_plugin_ranfurrypic-1.1.6/nonebot_plugin_RanFurryPic/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-12 02:51:56.375191 nonebot_plugin_ranfurrypic-1.1.6/nonebot_plugin_RanFurryPic.egg-info/
+-rw-rw-rw-   0        0        0     2828 2024-05-12 02:51:56.000000 nonebot_plugin_ranfurrypic-1.1.6/nonebot_plugin_RanFurryPic.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      320 2024-05-12 02:51:56.000000 nonebot_plugin_ranfurrypic-1.1.6/nonebot_plugin_RanFurryPic.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-12 02:51:56.000000 nonebot_plugin_ranfurrypic-1.1.6/nonebot_plugin_RanFurryPic.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2024-05-12 02:51:56.000000 nonebot_plugin_ranfurrypic-1.1.6/nonebot_plugin_RanFurryPic.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2024-05-12 02:51:56.000000 nonebot_plugin_ranfurrypic-1.1.6/nonebot_plugin_RanFurryPic.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      380 2024-05-12 02:51:33.000000 nonebot_plugin_ranfurrypic-1.1.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-12 02:51:56.378185 nonebot_plugin_ranfurrypic-1.1.6/setup.cfg
```

### Comparing `nonebot_plugin_ranfurrypic-1.1.5/LICENSE` & `nonebot_plugin_ranfurrypic-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_ranfurrypic-1.1.5/PKG-INFO` & `nonebot_plugin_ranfurrypic-1.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_RanFurryPic
-Version: 1.1.5
+Version: 1.1.6
 Summary: 基于NoneBot2进行适配的兽云随机毛图插件
 Author-email: Ekac <2396382559@qq.com>
 License: MIT
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: nonebot2
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot_plugin_RanFurryPic Version: 1.1.5 Summary:
+Metadata-Version: 2.1 Name: nonebot_plugin_RanFurryPic Version: 1.1.6 Summary:
 åºäºNoneBot2è¿è¡ééçå½äºéæºæ¯å¾æä»¶ Author-email: Ekac
 <2396382559@qq.com> License: MIT Requires-Python: >=3.9 Description-Content-
 Type: text/markdown License-File: LICENSE Requires-Dist: nonebot2 Requires-
 Dist: httpx Requires-Dist: nonebot-adapter-onebot
                               _[_N_o_n_e_B_o_t_P_l_u_g_i_n_L_o_g_o_]
                               [NoneBotPluginText]
        # nonebot-plugin-RanFurryPic _â¨ éæºæ¯å¾ â¨__[_p_y_p_i_][python]
```

### Comparing `nonebot_plugin_ranfurrypic-1.1.5/README.md` & `nonebot_plugin_ranfurrypic-1.1.6/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_ranfurrypic-1.1.5/nonebot_plugin_RanFurryPic/__init__.py` & `nonebot_plugin_ranfurrypic-1.1.6/nonebot_plugin_RanFurryPic/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from nonebot.adapters.onebot.v11 import MessageSegment
 import httpx
 from nonebot.plugin import PluginMetadata
 from nonebot.adapters import Message
 from nonebot.params import CommandArg
 
 __plugin_meta__ = PluginMetadata(
-    name="nonebot-plugin-RanFurryPic",
+    name="随机毛图",
     description="基于NoneBot2进行适配的兽云随机毛图插件",
     usage="预设指令有furry、来只毛、毛毛三种指令，发送后将会调用兽云的随即图片API并返回图片及基本介绍",
 
     type="application",
     # 发布必填，当前有效类型有：`library`（为其他插件编写提供功能），`application`（向机器人用户提供功能）。
 
     homepage="https://github.com/Ekac00/nonebot-plugin-RanFurryPic/",
```

### Comparing `nonebot_plugin_ranfurrypic-1.1.5/nonebot_plugin_RanFurryPic.egg-info/PKG-INFO` & `nonebot_plugin_ranfurrypic-1.1.6/nonebot_plugin_RanFurryPic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_RanFurryPic
-Version: 1.1.5
+Version: 1.1.6
 Summary: 基于NoneBot2进行适配的兽云随机毛图插件
 Author-email: Ekac <2396382559@qq.com>
 License: MIT
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: nonebot2
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot_plugin_RanFurryPic Version: 1.1.5 Summary:
+Metadata-Version: 2.1 Name: nonebot_plugin_RanFurryPic Version: 1.1.6 Summary:
 åºäºNoneBot2è¿è¡ééçå½äºéæºæ¯å¾æä»¶ Author-email: Ekac
 <2396382559@qq.com> License: MIT Requires-Python: >=3.9 Description-Content-
 Type: text/markdown License-File: LICENSE Requires-Dist: nonebot2 Requires-
 Dist: httpx Requires-Dist: nonebot-adapter-onebot
                               _[_N_o_n_e_B_o_t_P_l_u_g_i_n_L_o_g_o_]
                               [NoneBotPluginText]
        # nonebot-plugin-RanFurryPic _â¨ éæºæ¯å¾ â¨__[_p_y_p_i_][python]
```

