# Comparing `tmp/nonebot_plugin_furryfusion-0.1.1.tar.gz` & `tmp/nonebot_plugin_furryfusion-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_furryfusion-0.1.1.tar", last modified: Sun May 12 02:04:51 2024, max compression
+gzip compressed data, was "nonebot_plugin_furryfusion-0.1.2.tar", last modified: Sun May 12 02:21:50 2024, max compression
```

## Comparing `nonebot_plugin_furryfusion-0.1.1.tar` & `nonebot_plugin_furryfusion-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-12 02:04:51.156317 nonebot_plugin_furryfusion-0.1.1/
--rw-rw-rw-   0        0        0     1082 2024-05-10 14:34:54.000000 nonebot_plugin_furryfusion-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     2606 2024-05-12 02:04:51.155321 nonebot_plugin_furryfusion-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     2239 2024-05-12 02:04:17.000000 nonebot_plugin_furryfusion-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-12 02:04:51.132345 nonebot_plugin_furryfusion-0.1.1/nonebot_plugin_furryfusion/
--rw-rw-rw-   0        0        0     2559 2024-05-12 01:46:50.000000 nonebot_plugin_furryfusion-0.1.1/nonebot_plugin_furryfusion/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-12 02:04:51.154319 nonebot_plugin_furryfusion-0.1.1/nonebot_plugin_furryfusion.egg-info/
--rw-rw-rw-   0        0        0     2606 2024-05-12 02:04:51.000000 nonebot_plugin_furryfusion-0.1.1/nonebot_plugin_furryfusion.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      320 2024-05-12 02:04:51.000000 nonebot_plugin_furryfusion-0.1.1/nonebot_plugin_furryfusion.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-12 02:04:51.000000 nonebot_plugin_furryfusion-0.1.1/nonebot_plugin_furryfusion.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2024-05-12 02:04:51.000000 nonebot_plugin_furryfusion-0.1.1/nonebot_plugin_furryfusion.egg-info/requires.txt
--rw-rw-rw-   0        0        0       27 2024-05-12 02:04:51.000000 nonebot_plugin_furryfusion-0.1.1/nonebot_plugin_furryfusion.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      380 2024-05-12 02:00:03.000000 nonebot_plugin_furryfusion-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-12 02:04:51.156317 nonebot_plugin_furryfusion-0.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-12 02:21:50.031122 nonebot_plugin_furryfusion-0.1.2/
+-rw-rw-rw-   0        0        0     1082 2024-05-10 14:34:54.000000 nonebot_plugin_furryfusion-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0     2743 2024-05-12 02:21:50.030122 nonebot_plugin_furryfusion-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2376 2024-05-12 02:18:19.000000 nonebot_plugin_furryfusion-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-12 02:21:50.018130 nonebot_plugin_furryfusion-0.1.2/nonebot_plugin_furryfusion/
+-rw-rw-rw-   0        0        0     2559 2024-05-12 01:46:50.000000 nonebot_plugin_furryfusion-0.1.2/nonebot_plugin_furryfusion/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-12 02:21:50.029123 nonebot_plugin_furryfusion-0.1.2/nonebot_plugin_furryfusion.egg-info/
+-rw-rw-rw-   0        0        0     2743 2024-05-12 02:21:49.000000 nonebot_plugin_furryfusion-0.1.2/nonebot_plugin_furryfusion.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      320 2024-05-12 02:21:49.000000 nonebot_plugin_furryfusion-0.1.2/nonebot_plugin_furryfusion.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-12 02:21:49.000000 nonebot_plugin_furryfusion-0.1.2/nonebot_plugin_furryfusion.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2024-05-12 02:21:49.000000 nonebot_plugin_furryfusion-0.1.2/nonebot_plugin_furryfusion.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2024-05-12 02:21:49.000000 nonebot_plugin_furryfusion-0.1.2/nonebot_plugin_furryfusion.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      380 2024-05-12 02:19:01.000000 nonebot_plugin_furryfusion-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-12 02:21:50.032121 nonebot_plugin_furryfusion-0.1.2/setup.cfg
```

### Comparing `nonebot_plugin_furryfusion-0.1.1/LICENSE` & `nonebot_plugin_furryfusion-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_furryfusion-0.1.1/PKG-INFO` & `nonebot_plugin_furryfusion-0.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_furryfusion
-Version: 0.1.1
+Version: 0.1.2
 Summary: 基于NoneBot2进行适配的兽聚动态查询插件
 Author-email: Ekac <2396382559@qq.com>
 License: MIT
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: nonebot2
@@ -32,15 +32,15 @@
 
 </div>
 
 基于NoneBot2进行适配的兽聚动态查询插件
 
 ## 📖 介绍
 
-本插件使用<a href="https://api.furryfusion.net/service/activity">furryfusion.net API</a>接口进行编写<br><br>
+本插件使用<a href="https://console-docs.apipost.cn/preview/fcba96ab381efa80/fdb51b00b68a9bbf?target_id=3a8b741e-9648-4469-8f47-98484378fdcf">兽云API</a>进行编写<del>别问我为什么不集成到随机毛图里，问就是报错（</del><br><br>
 在开始前请先点一个免费的star吧谢谢啦~
 
 ### 由于在翻页做好前消息仍为整段发出，可能会被误识别为刷屏
 ### 由于长消息，go-cqhttp协议用户慎用，防风控！
 
 <details>
 <summary>买家秀</summary>
```

#### html2text {}

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1 Name: nonebot_plugin_furryfusion Version: 0.1.1 Summary:
+Metadata-Version: 2.1 Name: nonebot_plugin_furryfusion Version: 0.1.2 Summary:
 åºäºNoneBot2è¿è¡ééçå½èå¨ææ¥è¯¢æä»¶ Author-email: Ekac
 <2396382559@qq.com> License: MIT Requires-Python: >=3.9 Description-Content-
 Type: text/markdown License-File: LICENSE Requires-Dist: nonebot2 Requires-
 Dist: httpx Requires-Dist: nonebot-adapter-onebot
                               _[_N_o_n_e_B_o_t_P_l_u_g_i_n_L_o_g_o_]
                               [NoneBotPluginText]
               # nonebot-plugin-furryfusion _â¨ å½èå¨æ â¨_
 _[_p_y_p_i_][python]
 åºäºNoneBot2è¿è¡ééçå½èå¨ææ¥è¯¢æä»¶ ## ð ä»ç»
-æ¬æä»¶ä½¿ç¨_f_u_r_r_y_f_u_s_i_o_n_._n_e_t_ _A_P_Iæ¥å£è¿è¡ç¼å
+æ¬æä»¶ä½¿ç¨_å__½_ä_º__A_P_Iè¿è¡ç¼åå«é®æä¸ºä»ä¹ä¸éæå°éæºæ¯å¾éï¼é®å°±æ¯æ¥éï¼
 
 å¨å¼å§åè¯·åç¹ä¸ä¸ªåè´¹çstarå§è°¢è°¢å¦~ ###
 ç±äºå¨ç¿»é¡µåå¥½åæ¶æ¯ä»ä¸ºæ´æ®µååºï¼å¯è½ä¼è¢«è¯¯è¯å«ä¸ºå·å±
 ### ç±äºé¿æ¶æ¯ï¼go-cqhttpåè®®ç¨æ·æç¨ï¼é²é£æ§ï¼ ä¹°å®¶ç§
 [https://img2.imgtp.com/2024/05/12/dQ97OBnd.png]## ð¿ å®è£ ä½¿ç¨ nb-cli
 å®è£ï¼æ¨èï¼ å¨ nonebot2 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡,
 è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ nb plugin install nonebot-plugin-furryfusion
```

### Comparing `nonebot_plugin_furryfusion-0.1.1/README.md` & `nonebot_plugin_furryfusion-0.1.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 </div>
 
 基于NoneBot2进行适配的兽聚动态查询插件
 
 ## 📖 介绍
 
-本插件使用<a href="https://api.furryfusion.net/service/activity">furryfusion.net API</a>接口进行编写<br><br>
+本插件使用<a href="https://console-docs.apipost.cn/preview/fcba96ab381efa80/fdb51b00b68a9bbf?target_id=3a8b741e-9648-4469-8f47-98484378fdcf">兽云API</a>进行编写<del>别问我为什么不集成到随机毛图里，问就是报错（</del><br><br>
 在开始前请先点一个免费的star吧谢谢啦~
 
 ### 由于在翻页做好前消息仍为整段发出，可能会被误识别为刷屏
 ### 由于长消息，go-cqhttp协议用户慎用，防风控！
 
 <details>
 <summary>买家秀</summary>
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
                               _[_N_o_n_e_B_o_t_P_l_u_g_i_n_L_o_g_o_]
                               [NoneBotPluginText]
               # nonebot-plugin-furryfusion _â¨ å½èå¨æ â¨_
 _[_p_y_p_i_][python]
 åºäºNoneBot2è¿è¡ééçå½èå¨ææ¥è¯¢æä»¶ ## ð ä»ç»
-æ¬æä»¶ä½¿ç¨_f_u_r_r_y_f_u_s_i_o_n_._n_e_t_ _A_P_Iæ¥å£è¿è¡ç¼å
+æ¬æä»¶ä½¿ç¨_å__½_ä_º__A_P_Iè¿è¡ç¼åå«é®æä¸ºä»ä¹ä¸éæå°éæºæ¯å¾éï¼é®å°±æ¯æ¥éï¼
 
 å¨å¼å§åè¯·åç¹ä¸ä¸ªåè´¹çstarå§è°¢è°¢å¦~ ###
 ç±äºå¨ç¿»é¡µåå¥½åæ¶æ¯ä»ä¸ºæ´æ®µååºï¼å¯è½ä¼è¢«è¯¯è¯å«ä¸ºå·å±
 ### ç±äºé¿æ¶æ¯ï¼go-cqhttpåè®®ç¨æ·æç¨ï¼é²é£æ§ï¼ ä¹°å®¶ç§
 [https://img2.imgtp.com/2024/05/12/dQ97OBnd.png]## ð¿ å®è£ ä½¿ç¨ nb-cli
 å®è£ï¼æ¨èï¼ å¨ nonebot2 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡,
 è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ nb plugin install nonebot-plugin-furryfusion
```

### Comparing `nonebot_plugin_furryfusion-0.1.1/nonebot_plugin_furryfusion/__init__.py` & `nonebot_plugin_furryfusion-0.1.2/nonebot_plugin_furryfusion/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_furryfusion-0.1.1/nonebot_plugin_furryfusion.egg-info/PKG-INFO` & `nonebot_plugin_furryfusion-0.1.2/nonebot_plugin_furryfusion.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_furryfusion
-Version: 0.1.1
+Version: 0.1.2
 Summary: 基于NoneBot2进行适配的兽聚动态查询插件
 Author-email: Ekac <2396382559@qq.com>
 License: MIT
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: nonebot2
@@ -32,15 +32,15 @@
 
 </div>
 
 基于NoneBot2进行适配的兽聚动态查询插件
 
 ## 📖 介绍
 
-本插件使用<a href="https://api.furryfusion.net/service/activity">furryfusion.net API</a>接口进行编写<br><br>
+本插件使用<a href="https://console-docs.apipost.cn/preview/fcba96ab381efa80/fdb51b00b68a9bbf?target_id=3a8b741e-9648-4469-8f47-98484378fdcf">兽云API</a>进行编写<del>别问我为什么不集成到随机毛图里，问就是报错（</del><br><br>
 在开始前请先点一个免费的star吧谢谢啦~
 
 ### 由于在翻页做好前消息仍为整段发出，可能会被误识别为刷屏
 ### 由于长消息，go-cqhttp协议用户慎用，防风控！
 
 <details>
 <summary>买家秀</summary>
```

#### html2text {}

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1 Name: nonebot_plugin_furryfusion Version: 0.1.1 Summary:
+Metadata-Version: 2.1 Name: nonebot_plugin_furryfusion Version: 0.1.2 Summary:
 åºäºNoneBot2è¿è¡ééçå½èå¨ææ¥è¯¢æä»¶ Author-email: Ekac
 <2396382559@qq.com> License: MIT Requires-Python: >=3.9 Description-Content-
 Type: text/markdown License-File: LICENSE Requires-Dist: nonebot2 Requires-
 Dist: httpx Requires-Dist: nonebot-adapter-onebot
                               _[_N_o_n_e_B_o_t_P_l_u_g_i_n_L_o_g_o_]
                               [NoneBotPluginText]
               # nonebot-plugin-furryfusion _â¨ å½èå¨æ â¨_
 _[_p_y_p_i_][python]
 åºäºNoneBot2è¿è¡ééçå½èå¨ææ¥è¯¢æä»¶ ## ð ä»ç»
-æ¬æä»¶ä½¿ç¨_f_u_r_r_y_f_u_s_i_o_n_._n_e_t_ _A_P_Iæ¥å£è¿è¡ç¼å
+æ¬æä»¶ä½¿ç¨_å__½_ä_º__A_P_Iè¿è¡ç¼åå«é®æä¸ºä»ä¹ä¸éæå°éæºæ¯å¾éï¼é®å°±æ¯æ¥éï¼
 
 å¨å¼å§åè¯·åç¹ä¸ä¸ªåè´¹çstarå§è°¢è°¢å¦~ ###
 ç±äºå¨ç¿»é¡µåå¥½åæ¶æ¯ä»ä¸ºæ´æ®µååºï¼å¯è½ä¼è¢«è¯¯è¯å«ä¸ºå·å±
 ### ç±äºé¿æ¶æ¯ï¼go-cqhttpåè®®ç¨æ·æç¨ï¼é²é£æ§ï¼ ä¹°å®¶ç§
 [https://img2.imgtp.com/2024/05/12/dQ97OBnd.png]## ð¿ å®è£ ä½¿ç¨ nb-cli
 å®è£ï¼æ¨èï¼ å¨ nonebot2 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡,
 è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ nb plugin install nonebot-plugin-furryfusion
```

