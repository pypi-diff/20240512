# Comparing `tmp/nonebot_plugin_furryfusion-0.1.2.tar.gz` & `tmp/nonebot_plugin_furryfusion-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_furryfusion-0.1.2.tar", last modified: Sun May 12 02:21:50 2024, max compression
+gzip compressed data, was "nonebot_plugin_furryfusion-0.1.3.tar", last modified: Sun May 12 02:46:58 2024, max compression
```

## Comparing `nonebot_plugin_furryfusion-0.1.2.tar` & `nonebot_plugin_furryfusion-0.1.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-12 02:21:50.031122 nonebot_plugin_furryfusion-0.1.2/
--rw-rw-rw-   0        0        0     1082 2024-05-10 14:34:54.000000 nonebot_plugin_furryfusion-0.1.2/LICENSE
--rw-rw-rw-   0        0        0     2743 2024-05-12 02:21:50.030122 nonebot_plugin_furryfusion-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     2376 2024-05-12 02:18:19.000000 nonebot_plugin_furryfusion-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-12 02:21:50.018130 nonebot_plugin_furryfusion-0.1.2/nonebot_plugin_furryfusion/
--rw-rw-rw-   0        0        0     2559 2024-05-12 01:46:50.000000 nonebot_plugin_furryfusion-0.1.2/nonebot_plugin_furryfusion/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-12 02:21:50.029123 nonebot_plugin_furryfusion-0.1.2/nonebot_plugin_furryfusion.egg-info/
--rw-rw-rw-   0        0        0     2743 2024-05-12 02:21:49.000000 nonebot_plugin_furryfusion-0.1.2/nonebot_plugin_furryfusion.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      320 2024-05-12 02:21:49.000000 nonebot_plugin_furryfusion-0.1.2/nonebot_plugin_furryfusion.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-12 02:21:49.000000 nonebot_plugin_furryfusion-0.1.2/nonebot_plugin_furryfusion.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2024-05-12 02:21:49.000000 nonebot_plugin_furryfusion-0.1.2/nonebot_plugin_furryfusion.egg-info/requires.txt
--rw-rw-rw-   0        0        0       27 2024-05-12 02:21:49.000000 nonebot_plugin_furryfusion-0.1.2/nonebot_plugin_furryfusion.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      380 2024-05-12 02:19:01.000000 nonebot_plugin_furryfusion-0.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-12 02:21:50.032121 nonebot_plugin_furryfusion-0.1.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-12 02:46:58.556288 nonebot_plugin_furryfusion-0.1.3/
+-rw-rw-rw-   0        0        0     1082 2024-05-10 14:34:54.000000 nonebot_plugin_furryfusion-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0     2743 2024-05-12 02:46:58.555289 nonebot_plugin_furryfusion-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2376 2024-05-12 02:18:19.000000 nonebot_plugin_furryfusion-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-12 02:46:58.541298 nonebot_plugin_furryfusion-0.1.3/nonebot_plugin_furryfusion/
+-rw-rw-rw-   0        0        0     2545 2024-05-12 02:45:40.000000 nonebot_plugin_furryfusion-0.1.3/nonebot_plugin_furryfusion/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-12 02:46:58.553290 nonebot_plugin_furryfusion-0.1.3/nonebot_plugin_furryfusion.egg-info/
+-rw-rw-rw-   0        0        0     2743 2024-05-12 02:46:58.000000 nonebot_plugin_furryfusion-0.1.3/nonebot_plugin_furryfusion.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      320 2024-05-12 02:46:58.000000 nonebot_plugin_furryfusion-0.1.3/nonebot_plugin_furryfusion.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-12 02:46:58.000000 nonebot_plugin_furryfusion-0.1.3/nonebot_plugin_furryfusion.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2024-05-12 02:46:58.000000 nonebot_plugin_furryfusion-0.1.3/nonebot_plugin_furryfusion.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2024-05-12 02:46:58.000000 nonebot_plugin_furryfusion-0.1.3/nonebot_plugin_furryfusion.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      380 2024-05-12 02:46:00.000000 nonebot_plugin_furryfusion-0.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-12 02:46:58.556288 nonebot_plugin_furryfusion-0.1.3/setup.cfg
```

### Comparing `nonebot_plugin_furryfusion-0.1.2/LICENSE` & `nonebot_plugin_furryfusion-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_furryfusion-0.1.2/PKG-INFO` & `nonebot_plugin_furryfusion-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_furryfusion
-Version: 0.1.2
+Version: 0.1.3
 Summary: 基于NoneBot2进行适配的兽聚动态查询插件
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
-Metadata-Version: 2.1 Name: nonebot_plugin_furryfusion Version: 0.1.2 Summary:
+Metadata-Version: 2.1 Name: nonebot_plugin_furryfusion Version: 0.1.3 Summary:
 åºäºNoneBot2è¿è¡ééçå½èå¨ææ¥è¯¢æä»¶ Author-email: Ekac
 <2396382559@qq.com> License: MIT Requires-Python: >=3.9 Description-Content-
 Type: text/markdown License-File: LICENSE Requires-Dist: nonebot2 Requires-
 Dist: httpx Requires-Dist: nonebot-adapter-onebot
                               _[_N_o_n_e_B_o_t_P_l_u_g_i_n_L_o_g_o_]
                               [NoneBotPluginText]
               # nonebot-plugin-furryfusion _â¨ å½èå¨æ â¨_
```

### Comparing `nonebot_plugin_furryfusion-0.1.2/README.md` & `nonebot_plugin_furryfusion-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_furryfusion-0.1.2/nonebot_plugin_furryfusion/__init__.py` & `nonebot_plugin_furryfusion-0.1.3/nonebot_plugin_furryfusion/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import httpx
 from nonebot.plugin import on_command
 from nonebot.plugin import PluginMetadata
 
 __plugin_meta__ = PluginMetadata(
-    name="nonebot-plugin-furryfusion",
+    name="兽聚动态",
     description="基于NoneBot2进行适配的兽聚动态查询插件",
     usage="使用“兽聚动态”查询最新兽聚",
 
     type="application",
     # 发布必填，当前有效类型有：`library`（为其他插件编写提供功能），`application`（向机器人用户提供功能）。
 
     homepage="https://github.com/Ekac00/nonebot-plugin-furryfusion",
```

### Comparing `nonebot_plugin_furryfusion-0.1.2/nonebot_plugin_furryfusion.egg-info/PKG-INFO` & `nonebot_plugin_furryfusion-0.1.3/nonebot_plugin_furryfusion.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_furryfusion
-Version: 0.1.2
+Version: 0.1.3
 Summary: 基于NoneBot2进行适配的兽聚动态查询插件
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
-Metadata-Version: 2.1 Name: nonebot_plugin_furryfusion Version: 0.1.2 Summary:
+Metadata-Version: 2.1 Name: nonebot_plugin_furryfusion Version: 0.1.3 Summary:
 åºäºNoneBot2è¿è¡ééçå½èå¨ææ¥è¯¢æä»¶ Author-email: Ekac
 <2396382559@qq.com> License: MIT Requires-Python: >=3.9 Description-Content-
 Type: text/markdown License-File: LICENSE Requires-Dist: nonebot2 Requires-
 Dist: httpx Requires-Dist: nonebot-adapter-onebot
                               _[_N_o_n_e_B_o_t_P_l_u_g_i_n_L_o_g_o_]
                               [NoneBotPluginText]
               # nonebot-plugin-furryfusion _â¨ å½èå¨æ â¨_
```

