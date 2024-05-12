# Comparing `tmp/nonebot_plugin_ranfurrypic-1.1.4.tar.gz` & `tmp/nonebot_plugin_ranfurrypic-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_ranfurrypic-1.1.4.tar", last modified: Sat May 11 15:56:36 2024, max compression
+gzip compressed data, was "nonebot_plugin_ranfurrypic-1.1.5.tar", last modified: Sun May 12 02:09:52 2024, max compression
```

## Comparing `nonebot_plugin_ranfurrypic-1.1.4.tar` & `nonebot_plugin_ranfurrypic-1.1.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-11 15:56:36.854638 nonebot_plugin_ranfurrypic-1.1.4/
--rw-rw-rw-   0        0        0     1082 2024-05-10 14:34:54.000000 nonebot_plugin_ranfurrypic-1.1.4/LICENSE
--rw-rw-rw-   0        0        0     2953 2024-05-11 15:56:36.852639 nonebot_plugin_ranfurrypic-1.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     2586 2024-05-11 15:55:57.000000 nonebot_plugin_ranfurrypic-1.1.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-11 15:56:36.836649 nonebot_plugin_ranfurrypic-1.1.4/nonebot_plugin_RanFurryPic/
--rw-rw-rw-   0        0        0     3145 2024-05-11 15:52:58.000000 nonebot_plugin_ranfurrypic-1.1.4/nonebot_plugin_RanFurryPic/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-11 15:56:36.851640 nonebot_plugin_ranfurrypic-1.1.4/nonebot_plugin_RanFurryPic.egg-info/
--rw-rw-rw-   0        0        0     2953 2024-05-11 15:56:36.000000 nonebot_plugin_ranfurrypic-1.1.4/nonebot_plugin_RanFurryPic.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      320 2024-05-11 15:56:36.000000 nonebot_plugin_ranfurrypic-1.1.4/nonebot_plugin_RanFurryPic.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-11 15:56:36.000000 nonebot_plugin_ranfurrypic-1.1.4/nonebot_plugin_RanFurryPic.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2024-05-11 15:56:36.000000 nonebot_plugin_ranfurrypic-1.1.4/nonebot_plugin_RanFurryPic.egg-info/requires.txt
--rw-rw-rw-   0        0        0       27 2024-05-11 15:56:36.000000 nonebot_plugin_ranfurrypic-1.1.4/nonebot_plugin_RanFurryPic.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      380 2024-05-11 15:55:21.000000 nonebot_plugin_ranfurrypic-1.1.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-11 15:56:36.854638 nonebot_plugin_ranfurrypic-1.1.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-12 02:09:52.557617 nonebot_plugin_ranfurrypic-1.1.5/
+-rw-rw-rw-   0        0        0     1082 2024-05-10 14:34:54.000000 nonebot_plugin_ranfurrypic-1.1.5/LICENSE
+-rw-rw-rw-   0        0        0     2828 2024-05-12 02:09:52.556648 nonebot_plugin_ranfurrypic-1.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2461 2024-05-12 02:08:44.000000 nonebot_plugin_ranfurrypic-1.1.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-12 02:09:52.524638 nonebot_plugin_ranfurrypic-1.1.5/nonebot_plugin_RanFurryPic/
+-rw-rw-rw-   0        0        0     3145 2024-05-11 15:52:58.000000 nonebot_plugin_ranfurrypic-1.1.5/nonebot_plugin_RanFurryPic/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-12 02:09:52.554622 nonebot_plugin_ranfurrypic-1.1.5/nonebot_plugin_RanFurryPic.egg-info/
+-rw-rw-rw-   0        0        0     2828 2024-05-12 02:09:52.000000 nonebot_plugin_ranfurrypic-1.1.5/nonebot_plugin_RanFurryPic.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      320 2024-05-12 02:09:52.000000 nonebot_plugin_ranfurrypic-1.1.5/nonebot_plugin_RanFurryPic.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-12 02:09:52.000000 nonebot_plugin_ranfurrypic-1.1.5/nonebot_plugin_RanFurryPic.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2024-05-12 02:09:52.000000 nonebot_plugin_ranfurrypic-1.1.5/nonebot_plugin_RanFurryPic.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2024-05-12 02:09:52.000000 nonebot_plugin_ranfurrypic-1.1.5/nonebot_plugin_RanFurryPic.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      380 2024-05-12 02:09:00.000000 nonebot_plugin_ranfurrypic-1.1.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-12 02:09:52.557617 nonebot_plugin_ranfurrypic-1.1.5/setup.cfg
```

### Comparing `nonebot_plugin_ranfurrypic-1.1.4/LICENSE` & `nonebot_plugin_ranfurrypic-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_ranfurrypic-1.1.4/PKG-INFO` & `nonebot_plugin_ranfurrypic-1.1.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_RanFurryPic
-Version: 1.1.4
+Version: 1.1.5
 Summary: 基于NoneBot2进行适配的兽云随机毛图插件
 Author-email: Ekac <2396382559@qq.com>
 License: MIT
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: nonebot2
@@ -20,21 +20,18 @@
 <div align="center">
 
 # nonebot-plugin-RanFurryPic
 
 _✨ 随机毛图 ✨_
 
 
-<a href="./LICENSE">
-    <img src="https://img.shields.io/github/license/owner/nonebot-plugin-template.svg" alt="license">
+<a href="https://pypi.python.org/pypi/nonebot-plugin-RanFurryPic">
+    <img src="https://img.shields.io/pypi/v/nonebot-plugin-RanFurryPic.svg" alt="pypi">
 </a>
-<a href="https://pypi.python.org/pypi/nonebot-plugin-template">
-    <img src="https://img.shields.io/pypi/v/nonebot-plugin-template.svg" alt="pypi">
-</a>
-<img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">
+<img src="https://img.shields.io/badge/python-3.9+-blue.svg" alt="python">
 
 </div>
 
 基于NoneBot2进行适配的兽云随机毛图插件
 
 ## 📖 介绍
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
-Metadata-Version: 2.1 Name: nonebot_plugin_RanFurryPic Version: 1.1.4 Summary:
+Metadata-Version: 2.1 Name: nonebot_plugin_RanFurryPic Version: 1.1.5 Summary:
 åºäºNoneBot2è¿è¡ééçå½äºéæºæ¯å¾æä»¶ Author-email: Ekac
 <2396382559@qq.com> License: MIT Requires-Python: >=3.9 Description-Content-
 Type: text/markdown License-File: LICENSE Requires-Dist: nonebot2 Requires-
 Dist: httpx Requires-Dist: nonebot-adapter-onebot
                               _[_N_o_n_e_B_o_t_P_l_u_g_i_n_L_o_g_o_]
                               [NoneBotPluginText]
-  # nonebot-plugin-RanFurryPic _â¨ éæºæ¯å¾ â¨__[_l_i_c_e_n_s_e_]_[_p_y_p_i_][python]
+       # nonebot-plugin-RanFurryPic _â¨ éæºæ¯å¾ â¨__[_p_y_p_i_][python]
 åºäºNoneBot2è¿è¡ééçå½äºéæºæ¯å¾æä»¶ ## ð ä»ç»
 å½äºå®æ¹æä»¶å¤ªå¤æï¼åè½å¤ªæï¼çä¸æï¼ä¸å¼å®¹ï¼æåæä»¶ç»æï¼
 æ¬æä»¶ä½¿ç¨å®æ¹_A_P_Iè¿è¡ç¼åï¼æ éä»¤çï¼æ éTokenï¼å³å¯ä½¿ç¨éæºæ¯å¾åè½
 
 å¨å¼å§åè¯·åç¹ä¸ä¸ªåè´¹çstarå§è°¢è°¢å¦~ ä¹°å®¶ç§ [https://
 img2.imgtp.com/2024/05/10/U4xrcU7e.png]## ð¿ å®è£ ä½¿ç¨ nb-cli
 å®è£ï¼æ¨èï¼ å¨ nonebot2 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡,
```

### Comparing `nonebot_plugin_ranfurrypic-1.1.4/README.md` & `nonebot_plugin_ranfurrypic-1.1.5/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -7,21 +7,18 @@
 <div align="center">
 
 # nonebot-plugin-RanFurryPic
 
 _✨ 随机毛图 ✨_
 
 
-<a href="./LICENSE">
-    <img src="https://img.shields.io/github/license/owner/nonebot-plugin-template.svg" alt="license">
+<a href="https://pypi.python.org/pypi/nonebot-plugin-RanFurryPic">
+    <img src="https://img.shields.io/pypi/v/nonebot-plugin-RanFurryPic.svg" alt="pypi">
 </a>
-<a href="https://pypi.python.org/pypi/nonebot-plugin-template">
-    <img src="https://img.shields.io/pypi/v/nonebot-plugin-template.svg" alt="pypi">
-</a>
-<img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">
+<img src="https://img.shields.io/badge/python-3.9+-blue.svg" alt="python">
 
 </div>
 
 基于NoneBot2进行适配的兽云随机毛图插件
 
 ## 📖 介绍
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
                               _[_N_o_n_e_B_o_t_P_l_u_g_i_n_L_o_g_o_]
                               [NoneBotPluginText]
-  # nonebot-plugin-RanFurryPic _â¨ éæºæ¯å¾ â¨__[_l_i_c_e_n_s_e_]_[_p_y_p_i_][python]
+       # nonebot-plugin-RanFurryPic _â¨ éæºæ¯å¾ â¨__[_p_y_p_i_][python]
 åºäºNoneBot2è¿è¡ééçå½äºéæºæ¯å¾æä»¶ ## ð ä»ç»
 å½äºå®æ¹æä»¶å¤ªå¤æï¼åè½å¤ªæï¼çä¸æï¼ä¸å¼å®¹ï¼æåæä»¶ç»æï¼
 æ¬æä»¶ä½¿ç¨å®æ¹_A_P_Iè¿è¡ç¼åï¼æ éä»¤çï¼æ éTokenï¼å³å¯ä½¿ç¨éæºæ¯å¾åè½
 
 å¨å¼å§åè¯·åç¹ä¸ä¸ªåè´¹çstarå§è°¢è°¢å¦~ ä¹°å®¶ç§ [https://
 img2.imgtp.com/2024/05/10/U4xrcU7e.png]## ð¿ å®è£ ä½¿ç¨ nb-cli
 å®è£ï¼æ¨èï¼ å¨ nonebot2 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡,
```

### Comparing `nonebot_plugin_ranfurrypic-1.1.4/nonebot_plugin_RanFurryPic/__init__.py` & `nonebot_plugin_ranfurrypic-1.1.5/nonebot_plugin_RanFurryPic/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_ranfurrypic-1.1.4/nonebot_plugin_RanFurryPic.egg-info/PKG-INFO` & `nonebot_plugin_ranfurrypic-1.1.5/nonebot_plugin_RanFurryPic.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_RanFurryPic
-Version: 1.1.4
+Version: 1.1.5
 Summary: 基于NoneBot2进行适配的兽云随机毛图插件
 Author-email: Ekac <2396382559@qq.com>
 License: MIT
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: nonebot2
@@ -20,21 +20,18 @@
 <div align="center">
 
 # nonebot-plugin-RanFurryPic
 
 _✨ 随机毛图 ✨_
 
 
-<a href="./LICENSE">
-    <img src="https://img.shields.io/github/license/owner/nonebot-plugin-template.svg" alt="license">
+<a href="https://pypi.python.org/pypi/nonebot-plugin-RanFurryPic">
+    <img src="https://img.shields.io/pypi/v/nonebot-plugin-RanFurryPic.svg" alt="pypi">
 </a>
-<a href="https://pypi.python.org/pypi/nonebot-plugin-template">
-    <img src="https://img.shields.io/pypi/v/nonebot-plugin-template.svg" alt="pypi">
-</a>
-<img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">
+<img src="https://img.shields.io/badge/python-3.9+-blue.svg" alt="python">
 
 </div>
 
 基于NoneBot2进行适配的兽云随机毛图插件
 
 ## 📖 介绍
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
-Metadata-Version: 2.1 Name: nonebot_plugin_RanFurryPic Version: 1.1.4 Summary:
+Metadata-Version: 2.1 Name: nonebot_plugin_RanFurryPic Version: 1.1.5 Summary:
 åºäºNoneBot2è¿è¡ééçå½äºéæºæ¯å¾æä»¶ Author-email: Ekac
 <2396382559@qq.com> License: MIT Requires-Python: >=3.9 Description-Content-
 Type: text/markdown License-File: LICENSE Requires-Dist: nonebot2 Requires-
 Dist: httpx Requires-Dist: nonebot-adapter-onebot
                               _[_N_o_n_e_B_o_t_P_l_u_g_i_n_L_o_g_o_]
                               [NoneBotPluginText]
-  # nonebot-plugin-RanFurryPic _â¨ éæºæ¯å¾ â¨__[_l_i_c_e_n_s_e_]_[_p_y_p_i_][python]
+       # nonebot-plugin-RanFurryPic _â¨ éæºæ¯å¾ â¨__[_p_y_p_i_][python]
 åºäºNoneBot2è¿è¡ééçå½äºéæºæ¯å¾æä»¶ ## ð ä»ç»
 å½äºå®æ¹æä»¶å¤ªå¤æï¼åè½å¤ªæï¼çä¸æï¼ä¸å¼å®¹ï¼æåæä»¶ç»æï¼
 æ¬æä»¶ä½¿ç¨å®æ¹_A_P_Iè¿è¡ç¼åï¼æ éä»¤çï¼æ éTokenï¼å³å¯ä½¿ç¨éæºæ¯å¾åè½
 
 å¨å¼å§åè¯·åç¹ä¸ä¸ªåè´¹çstarå§è°¢è°¢å¦~ ä¹°å®¶ç§ [https://
 img2.imgtp.com/2024/05/10/U4xrcU7e.png]## ð¿ å®è£ ä½¿ç¨ nb-cli
 å®è£ï¼æ¨èï¼ å¨ nonebot2 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡,
```

