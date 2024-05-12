# Comparing `tmp/nonebot_plugin_furryfusion-0.1.0.tar.gz` & `tmp/nonebot_plugin_furryfusion-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_furryfusion-0.1.0.tar", last modified: Sun May 12 01:54:07 2024, max compression
+gzip compressed data, was "nonebot_plugin_furryfusion-0.1.1.tar", last modified: Sun May 12 02:04:51 2024, max compression
```

## Comparing `nonebot_plugin_furryfusion-0.1.0.tar` & `nonebot_plugin_furryfusion-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-12 01:54:07.748835 nonebot_plugin_furryfusion-0.1.0/
--rw-rw-rw-   0        0        0     1082 2024-05-10 14:34:54.000000 nonebot_plugin_furryfusion-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     2725 2024-05-12 01:54:07.747835 nonebot_plugin_furryfusion-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2358 2024-05-12 01:52:33.000000 nonebot_plugin_furryfusion-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-12 01:54:07.724851 nonebot_plugin_furryfusion-0.1.0/nonebot_plugin_furryfusion/
--rw-rw-rw-   0        0        0     2559 2024-05-12 01:46:50.000000 nonebot_plugin_furryfusion-0.1.0/nonebot_plugin_furryfusion/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-12 01:54:07.745836 nonebot_plugin_furryfusion-0.1.0/nonebot_plugin_furryfusion.egg-info/
--rw-rw-rw-   0        0        0     2725 2024-05-12 01:54:07.000000 nonebot_plugin_furryfusion-0.1.0/nonebot_plugin_furryfusion.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      320 2024-05-12 01:54:07.000000 nonebot_plugin_furryfusion-0.1.0/nonebot_plugin_furryfusion.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-12 01:54:07.000000 nonebot_plugin_furryfusion-0.1.0/nonebot_plugin_furryfusion.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2024-05-12 01:54:07.000000 nonebot_plugin_furryfusion-0.1.0/nonebot_plugin_furryfusion.egg-info/requires.txt
--rw-rw-rw-   0        0        0       27 2024-05-12 01:54:07.000000 nonebot_plugin_furryfusion-0.1.0/nonebot_plugin_furryfusion.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      380 2024-05-12 01:38:12.000000 nonebot_plugin_furryfusion-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-12 01:54:07.748835 nonebot_plugin_furryfusion-0.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-12 02:04:51.156317 nonebot_plugin_furryfusion-0.1.1/
+-rw-rw-rw-   0        0        0     1082 2024-05-10 14:34:54.000000 nonebot_plugin_furryfusion-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     2606 2024-05-12 02:04:51.155321 nonebot_plugin_furryfusion-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2239 2024-05-12 02:04:17.000000 nonebot_plugin_furryfusion-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-12 02:04:51.132345 nonebot_plugin_furryfusion-0.1.1/nonebot_plugin_furryfusion/
+-rw-rw-rw-   0        0        0     2559 2024-05-12 01:46:50.000000 nonebot_plugin_furryfusion-0.1.1/nonebot_plugin_furryfusion/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-12 02:04:51.154319 nonebot_plugin_furryfusion-0.1.1/nonebot_plugin_furryfusion.egg-info/
+-rw-rw-rw-   0        0        0     2606 2024-05-12 02:04:51.000000 nonebot_plugin_furryfusion-0.1.1/nonebot_plugin_furryfusion.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      320 2024-05-12 02:04:51.000000 nonebot_plugin_furryfusion-0.1.1/nonebot_plugin_furryfusion.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-12 02:04:51.000000 nonebot_plugin_furryfusion-0.1.1/nonebot_plugin_furryfusion.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2024-05-12 02:04:51.000000 nonebot_plugin_furryfusion-0.1.1/nonebot_plugin_furryfusion.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2024-05-12 02:04:51.000000 nonebot_plugin_furryfusion-0.1.1/nonebot_plugin_furryfusion.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      380 2024-05-12 02:00:03.000000 nonebot_plugin_furryfusion-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-12 02:04:51.156317 nonebot_plugin_furryfusion-0.1.1/setup.cfg
```

### Comparing `nonebot_plugin_furryfusion-0.1.0/LICENSE` & `nonebot_plugin_furryfusion-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_furryfusion-0.1.0/PKG-INFO` & `nonebot_plugin_furryfusion-0.1.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_furryfusion
-Version: 0.1.0
+Version: 0.1.1
 Summary: 基于NoneBot2进行适配的兽聚动态查询插件
 Author-email: Ekac <2396382559@qq.com>
 License: MIT
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: nonebot2
@@ -20,21 +20,19 @@
 <div align="center">
 
 # nonebot-plugin-furryfusion
 
 _✨ 兽聚动态 ✨_
 
 
-<a href="./LICENSE">
-    <img src="https://img.shields.io/github/license/owner/nonebot-plugin-template.svg" alt="license">
 </a>
-<a href="https://pypi.python.org/pypi/nonebot-plugin-template">
-    <img src="https://img.shields.io/pypi/v/nonebot-plugin-template.svg" alt="pypi">
+<a href="https://pypi.python.org/pypi/nonebot-plugin-furryfusion">
+    <img src="https://img.shields.io/pypi/v/nonebot-plugin-furryfusion.svg" alt="pypi">
 </a>
-<img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">
+<img src="https://img.shields.io/badge/python-3.9+-blue.svg" alt="python">
 
 </div>
 
 基于NoneBot2进行适配的兽聚动态查询插件
 
 ## 📖 介绍
```

#### html2text {}

```diff
@@ -1,15 +1,16 @@
-Metadata-Version: 2.1 Name: nonebot_plugin_furryfusion Version: 0.1.0 Summary:
+Metadata-Version: 2.1 Name: nonebot_plugin_furryfusion Version: 0.1.1 Summary:
 åºäºNoneBot2è¿è¡ééçå½èå¨ææ¥è¯¢æä»¶ Author-email: Ekac
 <2396382559@qq.com> License: MIT Requires-Python: >=3.9 Description-Content-
 Type: text/markdown License-File: LICENSE Requires-Dist: nonebot2 Requires-
 Dist: httpx Requires-Dist: nonebot-adapter-onebot
                               _[_N_o_n_e_B_o_t_P_l_u_g_i_n_L_o_g_o_]
                               [NoneBotPluginText]
-  # nonebot-plugin-furryfusion _â¨ å½èå¨æ â¨__[_l_i_c_e_n_s_e_]_[_p_y_p_i_][python]
+              # nonebot-plugin-furryfusion _â¨ å½èå¨æ â¨_
+_[_p_y_p_i_][python]
 åºäºNoneBot2è¿è¡ééçå½èå¨ææ¥è¯¢æä»¶ ## ð ä»ç»
 æ¬æä»¶ä½¿ç¨_f_u_r_r_y_f_u_s_i_o_n_._n_e_t_ _A_P_Iæ¥å£è¿è¡ç¼å
 
 å¨å¼å§åè¯·åç¹ä¸ä¸ªåè´¹çstarå§è°¢è°¢å¦~ ###
 ç±äºå¨ç¿»é¡µåå¥½åæ¶æ¯ä»ä¸ºæ´æ®µååºï¼å¯è½ä¼è¢«è¯¯è¯å«ä¸ºå·å±
 ### ç±äºé¿æ¶æ¯ï¼go-cqhttpåè®®ç¨æ·æç¨ï¼é²é£æ§ï¼ ä¹°å®¶ç§
 [https://img2.imgtp.com/2024/05/12/dQ97OBnd.png]## ð¿ å®è£ ä½¿ç¨ nb-cli
```

### Comparing `nonebot_plugin_furryfusion-0.1.0/README.md` & `nonebot_plugin_furryfusion-0.1.1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -7,21 +7,19 @@
 <div align="center">
 
 # nonebot-plugin-furryfusion
 
 _✨ 兽聚动态 ✨_
 
 
-<a href="./LICENSE">
-    <img src="https://img.shields.io/github/license/owner/nonebot-plugin-template.svg" alt="license">
 </a>
-<a href="https://pypi.python.org/pypi/nonebot-plugin-template">
-    <img src="https://img.shields.io/pypi/v/nonebot-plugin-template.svg" alt="pypi">
+<a href="https://pypi.python.org/pypi/nonebot-plugin-furryfusion">
+    <img src="https://img.shields.io/pypi/v/nonebot-plugin-furryfusion.svg" alt="pypi">
 </a>
-<img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">
+<img src="https://img.shields.io/badge/python-3.9+-blue.svg" alt="python">
 
 </div>
 
 基于NoneBot2进行适配的兽聚动态查询插件
 
 ## 📖 介绍
```

#### html2text {}

```diff
@@ -1,10 +1,11 @@
                               _[_N_o_n_e_B_o_t_P_l_u_g_i_n_L_o_g_o_]
                               [NoneBotPluginText]
-  # nonebot-plugin-furryfusion _â¨ å½èå¨æ â¨__[_l_i_c_e_n_s_e_]_[_p_y_p_i_][python]
+              # nonebot-plugin-furryfusion _â¨ å½èå¨æ â¨_
+_[_p_y_p_i_][python]
 åºäºNoneBot2è¿è¡ééçå½èå¨ææ¥è¯¢æä»¶ ## ð ä»ç»
 æ¬æä»¶ä½¿ç¨_f_u_r_r_y_f_u_s_i_o_n_._n_e_t_ _A_P_Iæ¥å£è¿è¡ç¼å
 
 å¨å¼å§åè¯·åç¹ä¸ä¸ªåè´¹çstarå§è°¢è°¢å¦~ ###
 ç±äºå¨ç¿»é¡µåå¥½åæ¶æ¯ä»ä¸ºæ´æ®µååºï¼å¯è½ä¼è¢«è¯¯è¯å«ä¸ºå·å±
 ### ç±äºé¿æ¶æ¯ï¼go-cqhttpåè®®ç¨æ·æç¨ï¼é²é£æ§ï¼ ä¹°å®¶ç§
 [https://img2.imgtp.com/2024/05/12/dQ97OBnd.png]## ð¿ å®è£ ä½¿ç¨ nb-cli
```

### Comparing `nonebot_plugin_furryfusion-0.1.0/nonebot_plugin_furryfusion/__init__.py` & `nonebot_plugin_furryfusion-0.1.1/nonebot_plugin_furryfusion/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_furryfusion-0.1.0/nonebot_plugin_furryfusion.egg-info/PKG-INFO` & `nonebot_plugin_furryfusion-0.1.1/nonebot_plugin_furryfusion.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_furryfusion
-Version: 0.1.0
+Version: 0.1.1
 Summary: 基于NoneBot2进行适配的兽聚动态查询插件
 Author-email: Ekac <2396382559@qq.com>
 License: MIT
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: nonebot2
@@ -20,21 +20,19 @@
 <div align="center">
 
 # nonebot-plugin-furryfusion
 
 _✨ 兽聚动态 ✨_
 
 
-<a href="./LICENSE">
-    <img src="https://img.shields.io/github/license/owner/nonebot-plugin-template.svg" alt="license">
 </a>
-<a href="https://pypi.python.org/pypi/nonebot-plugin-template">
-    <img src="https://img.shields.io/pypi/v/nonebot-plugin-template.svg" alt="pypi">
+<a href="https://pypi.python.org/pypi/nonebot-plugin-furryfusion">
+    <img src="https://img.shields.io/pypi/v/nonebot-plugin-furryfusion.svg" alt="pypi">
 </a>
-<img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">
+<img src="https://img.shields.io/badge/python-3.9+-blue.svg" alt="python">
 
 </div>
 
 基于NoneBot2进行适配的兽聚动态查询插件
 
 ## 📖 介绍
```

#### html2text {}

```diff
@@ -1,15 +1,16 @@
-Metadata-Version: 2.1 Name: nonebot_plugin_furryfusion Version: 0.1.0 Summary:
+Metadata-Version: 2.1 Name: nonebot_plugin_furryfusion Version: 0.1.1 Summary:
 åºäºNoneBot2è¿è¡ééçå½èå¨ææ¥è¯¢æä»¶ Author-email: Ekac
 <2396382559@qq.com> License: MIT Requires-Python: >=3.9 Description-Content-
 Type: text/markdown License-File: LICENSE Requires-Dist: nonebot2 Requires-
 Dist: httpx Requires-Dist: nonebot-adapter-onebot
                               _[_N_o_n_e_B_o_t_P_l_u_g_i_n_L_o_g_o_]
                               [NoneBotPluginText]
-  # nonebot-plugin-furryfusion _â¨ å½èå¨æ â¨__[_l_i_c_e_n_s_e_]_[_p_y_p_i_][python]
+              # nonebot-plugin-furryfusion _â¨ å½èå¨æ â¨_
+_[_p_y_p_i_][python]
 åºäºNoneBot2è¿è¡ééçå½èå¨ææ¥è¯¢æä»¶ ## ð ä»ç»
 æ¬æä»¶ä½¿ç¨_f_u_r_r_y_f_u_s_i_o_n_._n_e_t_ _A_P_Iæ¥å£è¿è¡ç¼å
 
 å¨å¼å§åè¯·åç¹ä¸ä¸ªåè´¹çstarå§è°¢è°¢å¦~ ###
 ç±äºå¨ç¿»é¡µåå¥½åæ¶æ¯ä»ä¸ºæ´æ®µååºï¼å¯è½ä¼è¢«è¯¯è¯å«ä¸ºå·å±
 ### ç±äºé¿æ¶æ¯ï¼go-cqhttpåè®®ç¨æ·æç¨ï¼é²é£æ§ï¼ ä¹°å®¶ç§
 [https://img2.imgtp.com/2024/05/12/dQ97OBnd.png]## ð¿ å®è£ ä½¿ç¨ nb-cli
```

