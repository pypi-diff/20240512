# Comparing `tmp/nonebot-plugin-hx-yinying-1.2.0.tar.gz` & `tmp/nonebot-plugin-hx-yinying-1.2.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-hx-yinying-1.2.0.tar", last modified: Fri May 10 17:56:18 2024, max compression
+gzip compressed data, was "nonebot-plugin-hx-yinying-1.2.11.tar", last modified: Sun May 12 06:58:45 2024, max compression
```

## Comparing `nonebot-plugin-hx-yinying-1.2.0.tar` & `nonebot-plugin-hx-yinying-1.2.11.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-05-10 17:56:18.662410 nonebot-plugin-hx-yinying-1.2.0/
--rw-rw-rw-   0        0        0     1098 2024-04-16 15:27:11.000000 nonebot-plugin-hx-yinying-1.2.0/LICENSE
--rw-rw-rw-   0        0        0     6502 2024-05-10 17:56:18.666539 nonebot-plugin-hx-yinying-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     6062 2024-04-28 16:24:12.000000 nonebot-plugin-hx-yinying-1.2.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-10 17:56:18.518412 nonebot-plugin-hx-yinying-1.2.0/nonebot_plugin_hx_yinying/
--rw-rw-rw-   0        0        0    57847 2024-05-07 15:39:33.000000 nonebot-plugin-hx-yinying-1.2.0/nonebot_plugin_hx_yinying/__init__.py
--rw-rw-rw-   0        0        0    91238 2024-05-10 16:16:29.000000 nonebot-plugin-hx-yinying-1.2.0/nonebot_plugin_hx_yinying/chat.py
--rw-rw-rw-   0        0        0     1532 2024-05-10 14:38:31.000000 nonebot-plugin-hx-yinying-1.2.0/nonebot_plugin_hx_yinying/config.py
--rw-rw-rw-   0        0        0     2553 2024-05-10 15:19:05.000000 nonebot-plugin-hx-yinying-1.2.0/nonebot_plugin_hx_yinying/image_check.py
--rw-rw-rw-   0        0        0     5501 2024-05-09 13:48:28.000000 nonebot-plugin-hx-yinying-1.2.0/nonebot_plugin_hx_yinying/report.py
--rw-rw-rw-   0        0        0     5038 2024-05-10 14:31:14.000000 nonebot-plugin-hx-yinying-1.2.0/nonebot_plugin_hx_yinying/smms.py
-drwxrwxrwx   0        0        0        0 2024-05-10 17:56:18.657411 nonebot-plugin-hx-yinying-1.2.0/nonebot_plugin_hx_yinying.egg-info/
--rw-rw-rw-   0        0        0     6502 2024-05-10 17:56:17.000000 nonebot-plugin-hx-yinying-1.2.0/nonebot_plugin_hx_yinying.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      499 2024-05-10 17:56:18.000000 nonebot-plugin-hx-yinying-1.2.0/nonebot_plugin_hx_yinying.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 17:56:17.000000 nonebot-plugin-hx-yinying-1.2.0/nonebot_plugin_hx_yinying.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      274 2024-05-10 17:56:17.000000 nonebot-plugin-hx-yinying-1.2.0/nonebot_plugin_hx_yinying.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2024-05-10 17:56:17.000000 nonebot-plugin-hx-yinying-1.2.0/nonebot_plugin_hx_yinying.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       85 2024-05-10 17:56:18.677973 nonebot-plugin-hx-yinying-1.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1002 2024-05-10 17:56:00.000000 nonebot-plugin-hx-yinying-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-12 06:58:45.912371 nonebot-plugin-hx-yinying-1.2.11/
+-rw-rw-rw-   0        0        0     1098 2024-04-16 15:27:11.000000 nonebot-plugin-hx-yinying-1.2.11/LICENSE
+-rw-rw-rw-   0        0        0     6503 2024-05-12 06:58:45.926562 nonebot-plugin-hx-yinying-1.2.11/PKG-INFO
+-rw-rw-rw-   0        0        0     6062 2024-04-28 16:24:12.000000 nonebot-plugin-hx-yinying-1.2.11/README.md
+drwxrwxrwx   0        0        0        0 2024-05-12 06:58:45.831545 nonebot-plugin-hx-yinying-1.2.11/nonebot_plugin_hx_yinying/
+-rw-rw-rw-   0        0        0    55316 2024-05-11 17:47:15.000000 nonebot-plugin-hx-yinying-1.2.11/nonebot_plugin_hx_yinying/__init__.py
+-rw-rw-rw-   0        0        0    89401 2024-05-12 06:53:55.000000 nonebot-plugin-hx-yinying-1.2.11/nonebot_plugin_hx_yinying/chat.py
+-rw-rw-rw-   0        0        0     1533 2024-05-12 06:58:41.000000 nonebot-plugin-hx-yinying-1.2.11/nonebot_plugin_hx_yinying/config.py
+-rw-rw-rw-   0        0        0     2549 2024-05-11 16:56:48.000000 nonebot-plugin-hx-yinying-1.2.11/nonebot_plugin_hx_yinying/image_check.py
+-rw-rw-rw-   0        0        0     5492 2024-05-11 17:03:36.000000 nonebot-plugin-hx-yinying-1.2.11/nonebot_plugin_hx_yinying/report.py
+-rw-rw-rw-   0        0        0     5038 2024-05-10 14:31:14.000000 nonebot-plugin-hx-yinying-1.2.11/nonebot_plugin_hx_yinying/smms.py
+drwxrwxrwx   0        0        0        0 2024-05-12 06:58:45.912371 nonebot-plugin-hx-yinying-1.2.11/nonebot_plugin_hx_yinying.egg-info/
+-rw-rw-rw-   0        0        0     6503 2024-05-12 06:58:45.000000 nonebot-plugin-hx-yinying-1.2.11/nonebot_plugin_hx_yinying.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      499 2024-05-12 06:58:45.000000 nonebot-plugin-hx-yinying-1.2.11/nonebot_plugin_hx_yinying.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-12 06:58:45.000000 nonebot-plugin-hx-yinying-1.2.11/nonebot_plugin_hx_yinying.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      274 2024-05-12 06:58:45.000000 nonebot-plugin-hx-yinying-1.2.11/nonebot_plugin_hx_yinying.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2024-05-12 06:58:45.000000 nonebot-plugin-hx-yinying-1.2.11/nonebot_plugin_hx_yinying.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2024-05-12 06:58:45.932306 nonebot-plugin-hx-yinying-1.2.11/setup.cfg
+-rw-rw-rw-   0        0        0     1003 2024-05-12 06:58:32.000000 nonebot-plugin-hx-yinying-1.2.11/setup.py
```

### Comparing `nonebot-plugin-hx-yinying-1.2.0/LICENSE` & `nonebot-plugin-hx-yinying-1.2.11/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-hx-yinying-1.2.0/PKG-INFO` & `nonebot-plugin-hx-yinying-1.2.11/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-hx-yinying
-Version: 1.2.0
+Version: 1.2.11
 Summary: chat with yinying
 Home-page: https://github.com/huanxin996/nonebot_plugin_hx-yinying
 Author: Huan Xin
 Author-email: mc.xiaolang@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-hx-yinying Version: 1.2.0 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-hx-yinying Version: 1.2.11 Summary:
 chat with yinying Home-page: https://github.com/huanxin996/nonebot_plugin_hx-
 yinying Author: Huan Xin Author-email: mc.xiaolang@foxmail.com Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Description-Content-
 Type: text/markdown License-File: LICENSE [![All Contributors](https://
 img.shields.io/badge/all_contributors-2-orange.svg?style=flat-square)]
 (#contributors-) * @Author : huanxin996 * @Date : 2024-4-17 * @LastEditors :
```

### Comparing `nonebot-plugin-hx-yinying-1.2.0/README.md` & `nonebot-plugin-hx-yinying-1.2.11/README.md`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-hx-yinying-1.2.0/nonebot_plugin_hx_yinying/__init__.py` & `nonebot-plugin-hx-yinying-1.2.11/nonebot_plugin_hx_yinying/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,69 +36,55 @@
 )
 
 hx_config = get_plugin_config(Config)
 global_config = config_in_global()
 dy_list = json_get(config_in_global(),"dy_list")
 log_dir = path_in()
    
-#检查更新
-new_verision, time = update_hx()
-
-if not new_verision and not time:
-    logger.error(f"[Hx_YinYing]:无法获取最新的版本，当前版本为{hx_config.hx_version}，可能已经过时！")
-else:
-    if new_verision <= hx_config.hx_version:
-        logger.success(f"[Hx_YinYing]:你的Hx_YinYing已经是最新版本了！当前版本为{hx_config.hx_version},仓库版本为{new_verision}")
-    else:
-        if os.path.exists(f"{log_dir}/config/config_glob21.json"):
-            logger.success("121")
-        else:
-            logger.success("[Hx_YinYing]:检查到Hx_YinYing有新版本！")
-            logger.warning("【Hx】正在自动更新中--未找到虚拟环境【安装在本地环境！】")
-            os.system(f'pip install nonebot-plugin-hx-yinying=={new_verision} -i https://pypi.Python.org/simple/')
-            logger.success(f"[Hx_YinYing]:更新完成！最新版本为{new_verision}|当前使用版本为{hx_config.hx_version}")
-            logger.warning(f"[Hx_YinYing]:你可能需要重新启动nonebot来完成插件的重载")
-
 #检查关键配置
-if hx_config.yinying_appid == None or hx_config.yinying_token == None:
-    logger.opt(colors=True).error("未设置核心配置？！,请检查你配置里的yinying_appid和yinying_token")
+if not hx_config.yinying_appid or not hx_config.yinying_token:
+    raise RuntimeError("未设置核心配置？！,请检查你配置里的yinying_appid和yinying_token")
 else:
     logger.opt(colors=True).success("【Hx】加载核心配置成功")
 
+
+#检测更新
+try:
+    check_update()
+except Exception as e:
+    logger.opt(colors=True).error("【Hx】检测更新失败！！，联系开发者！错误捕获{e}")
+
+#尝试自动更新-1day
+try:
+    extent = int(len(dy_list))
+    for key in dy_list:
+        config_1 = config_in_user(key,False)
+        user_config = json_get(config_1,key)
+        config_time = json_get_time(user_config,"dy_time")
+        config_minute = json_get_time(user_config,"dy_minute")
+        scheduler.add_job(func=check_update,trigger='interval',hours=24,id="huanxin996")
+    logger.opt(colors=True).success(f"【Hx】定时检测更新启动。")
+except Exception as e:
+    logger.opt(colors=True).error("【Hx】定时检测更新启动失败！！，联系开发者！错误捕获{e}")
+
 #根据订阅信息注册定时任务
 try:
     extent = int(len(dy_list))
     for key in dy_list:
         config_1 = config_in_user(key,False)
         user_config = json_get(config_1,key)
         config_time = json_get_time(user_config,"dy_time")
         config_minute = json_get_time(user_config,"dy_minute")
         scheduler.add_job(func=get_chat,trigger='interval',args=[key] ,hours=config_time, minutes=config_minute, id=key)
     logger.opt(colors=True).success(f"【Hx】定时任务加载成功,当前共加载{extent}个订阅用户")
-    logger.opt(colors=True).success( f"""
-    <fg #60F5F5>                   ------------------<Y>幻歆v{hx_config.hx_version}</Y>----------------</fg #60F5F5>
-<fg #60F5F5>,--,                                                                                                 </fg #60F5F5>                 
-<r>      ,--.'|                                       ,--,     ,--,                                 ,---,.               ___   </r> 
-<y>   ,--,  | :                                       |'. \   / .`|  ,--,                         ,'  .'  \            ,--.'|_   </y>
-<g>,---.'|  : '         ,--,                    ,---, ; \ `\ /' / ;,--.'|         ,---,         ,---.' .' |   ,---.    |  | :,' </g> 
-<c>|   | : _' |       ,'_ /|                ,-+-. /  |`. \  /  / .'|  |,      ,-+-. /  |        |   |  |: |  '   ,'\   :  : ' :  </c>
-<e>:   : |.'  |  .--. |  | :    ,--.--.    ,--.'|'   | \  \/  / ./ `--'_     ,--.'|'   |        :   :  :  / /   /   |.;__,'  /   </e>
-<m>|   ' '  ; :,'_ /| :  . |   /       \  |   |  ,"' |  \  \.'  /  ,' ,'|   |   |  ,"' |        :   |    ; .   ; ,. :|  |   |    </m>
-<e>'   |  .'. ||  ' | |  . .  .--.  .-. | |   | /  | |   \  ;  ;   '  | |   |   | /  | |        |   :     \'   | |: ::__,'| :    </e>
-<c>|   | :  | '|  | ' |  | |   \__\/: . . |   | |  | |  / \  \  \  |  | :   |   | |  | |        |   |   . |'   | .; :  '  : |__  </c>
-<g>'   : |  : ;:  | : ;  ; |   ," .--.; | |   | |  |/  ;  /\  \  \ '  : |__ |   | |  |/         '   :  '; ||   :    |  |  | '.'| </g>
-<y>|   | '  ,/ '  :  `--'   \ /  /  ,.  | |   | |--' ./__;  \  ;  \|  | '.'||   | |--'          |   |  | ;  \   \  /   ;  :    ; </y>
-<r>;   : ;--'  :  ,      .-./;  :   .'   \|   |/     |   : / \  \  ;  :    ;|   |/              |   :   /    `----'    |  ,   /  </r>
-<m>|   ,/       `--`----'    |  ,     .-./'---'      ;   |/   \  ' |  ,   / '---'               |   | ,'                ---`-'   </m>
-<r>'---'                      `--`---'               `---'     `--` ---`-'                      `----'</r>
-    <fg #60F5F5>                   ------------------<Y>幻歆v{hx_config.hx_version}</Y>----------------</fg #60F5F5>
-""")
 except Exception as e:
-    logger.opt(colors=True).error(f"【Hx】:错误捕获{e}，联系开发者！")
-    logger.opt(colors=True).error("【Hx】定时任务加载失败！！，联系开发者！")
+    logger.opt(colors=True).error("【Hx】定时任务加载失败！！，联系开发者！错误捕获{e}")
+
+
+
 
 #主要命令列表
 msg_at = on_message(rule=Rule(chek_rule_base)&to_me(), priority=10,  block=True)
 msg_ml = on_command("hx", aliases={"chat","yinying","yy"},rule=Rule(chek_rule_base),  priority=10, block=True)
 clear =  on_command("刷新对话", aliases={"clear"},rule=Rule(chek_rule_base),  priority=0, block=True)
 history_get = on_command("导出对话", aliases={"getchat"},rule=Rule(chek_rule_base),  priority=0, block=True)
 set_global_config = on_command("设置全局配置", aliases={"设置配置全局","globalset"},rule=Rule(chek_rule_admin),  priority=0, block=True)
@@ -491,15 +477,15 @@
                 s["last"] = True
                 msg = "easycyber预设“Hx”不能删除或修改，如要改动请改源码"
                 await send_msg(matcher,event,msg)
             elif text == "退出":
                 s["last"] = True
                 msg = "已退出"
                 await send_msg(matcher,event,msg)
-            elif text in easycyber_in_tg(text,False) or text in easycyber_in(text,False):
+            elif text in easycyber_in_tg(text,False) or text in easycyber_in(text,False) or not text:
                 s["last"] = "增加"
                 msg = "该预设角色名称已经存在，请不要重复使用该昵称，请重新输入，如需退出请发送退出"
                 await send_msg_reject(matcher,event,msg)
             else:
                 s["cfnickname"] = text
                 s["last"] = "cfSpecies"
                 msg = "请输入角色物种"
@@ -753,15 +739,15 @@
                     easycyber_package["public"] = key[f"{text}"]
                     easycyber_package["creator"] = int(id)
                     s["last"] = True
                     g = json_get(config_in_global(),"admin_group")
                     u = json_get(config_in_global(),"admin_pro")
                     g_k = json_get(config_in_global(),"admin_group_switch")
                     u_k = json_get(config_in_global(),"admin_user_switch")
-                    msg_tg = f"新投稿！\n来源于QQ[{id}]\n以下为设定内容\n===========\n昵称:{name}\nsystem:{systempromote}==========="
+                    msg_tg = f"新投稿！\n来源于QQ[{id}]\n以下为设定内容\n===========\n昵称:{name}\nsystem:{systempromote}\n\n==========="
                     msg = "投稿成功！，等待审核(问就是权限还没写好)]"
                     if not g and not u:
                         logger.opt(colors=True).success(f"{g},{u}")
                         msg ="bot管理者未配置，超级管理员和bot控制台,审核失败！"
                     elif not u and g:
                         cyber_in_tg(name,easycyber_package)
                         await bot.call_api("send_group_msg",group_id=g, message=msg_tg)
```

### Comparing `nonebot-plugin-hx-yinying-1.2.0/nonebot_plugin_hx_yinying/chat.py` & `nonebot-plugin-hx-yinying-1.2.11/nonebot_plugin_hx_yinying/chat.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -- coding: utf-8 --**
 from nonebot.adapters.onebot.v11 import Bot, GroupMessageEvent ,MessageSegment ,Message,MessageEvent,Event
 from html import unescape
 from typing import List
 import os,httpx, json, time, requests,platform
 from loguru import logger as lg
 from .config import Config
-import operator,nonebot
+import operator,nonebot,random,string
 from nonebot import get_plugin_config, logger, require,get_driver
 from pathlib import Path
 require("nonebot_plugin_localstore")
 import nonebot_plugin_localstore as store
 from .image_check import image_check
 from .report import error_oops
 
@@ -60,14 +60,20 @@
     <fg #60F5F5>                   ------------------<Y>幻歆v{hx_config.hx_version}</Y>----------------</fg #60F5F5>
 """)
     logger.success("找到配置里的路径，载入成功")
     history_dir = store.get_data_dir(f"{hx_config.hx_path}")
     log_dir = Path(f"{history_dir}/yinying_chat").absolute()
     log_dir.mkdir(parents=True, exist_ok=True)
 
+def number_suiji():
+    digits = "0123456789"
+    str_list =[random.choice(digits) for i in range(3)]
+    random_str =''.join(str_list)
+    return random_str
+
 #判断模型
 def model_got(msg) -> str:
     back = "yinyingllm-v2"
     try:
         if msg == "1" or msg == "yinyingllm-v1" or msg == "yinyingllmv1":
             back = "yinyingllm-v1"
         elif msg == "2" or msg == "yinyingllm-v2" or msg == "yinyingllmv2":
@@ -181,23 +187,14 @@
             seg.data["url"]
             for seg in event.message
             if (seg.type == "image") and ("url" in seg.data)
         ]
     )
     return urls
 
-#结果消息函数，发送消息直接await就行
-async def send_msg_reject(matcher, event, content):
-    config_global = config_in_global()
-    reply_config = json_get(config_global,"reply")
-    if reply_config == True:
-        await matcher.reject(MessageSegment.reply(event.message_id) + content)
-    else:
-        reply_at = json_get(config_global,"reply_at")
-        await matcher.reject(content, at_sender=reply_at)
 
 #创建用户文件夹
 def create_dir_usr(path):
     if not os.path.exists(path):
         os.mkdir(path)
 
 #获取json函数
@@ -261,72 +258,31 @@
                     package['msg'] = '初始化log记录'
                     history_package.append(package)
                     json_data['114514'] = history_package
                     json.dump(json_data,file)
                     back = json_data
     return back
 
-#用户输入
-def user_in(id, text):
-    data = log_in()
-    if f'{id}' in data: 
-        id_log = data[f'{id}']['log']
-        package = {}
-        package['rule'] = 'user'
-        text_r = json_replace(text)
-        package['msg'] = f'{text_r}'
-        id_log.append(package)
-        data[f'{id}']['log'] = id_log
-        with open(f'{log_dir}/chat/all_log.json','w',encoding='utf-8') as file:
-            json.dump(data,file)
-    else : 
-        package = {}
-        log = {}
-        history_package = []
-        package['rule'] = 'user'
-        text_r = json_replace(text)
-        package['msg'] = f'{text_r}'
-        history_package.append(package)
-        log['log'] = history_package
-        dt = time.time()
-        t = int(dt)
-        log['time'] = t
-        data[f'{id}'] = log
-        with open(f'{log_dir}/chat/all_log.json','w',encoding='utf-8') as file:
-            json.dump(data,file)
-
-#AI输出
-def ai_out(id, text):
-    data = log_in()
-    if f'{id}' in data: 
-        id_log = data[f'{id}']['log']
-        package = {}
-        package['rule'] = 'ai'
-        text_r = json_replace(text)
-        package['msg'] = f'{text_r}'
-        id_log.append(package)
-        data[f'{id}']['log'] = id_log
-        with open(f'{log_dir}/chat/all_log.json','w',encoding='utf-8') as file:
-            json.dump(data,file)
-    else : 
-        package = {}
-        log = {}
-        history_package = []
-        package['rule'] = 'ai'
-        text_r = json_replace(text)
-        package['msg'] = f'{text_r}'
-        history_package.append(package)
-        log['log'] = history_package
-        dt = time.time()
-        t = int(dt)
-        log['time'] = t
-        data[f'{id}'] = log
-        with open(f'{log_dir}/chat/all_log.json','w',encoding='utf-8') as file:
-            json.dump(data,file)
-
+#检查更新
+def check_update():
+    new_verision, time = update_hx()
+    if not new_verision and not time:
+        logger.error(f"[Hx_YinYing]:无法获取最新的版本，当前版本为{hx_config.hx_version}，可能已经过时！")
+    else:
+        if new_verision <= hx_config.hx_version:
+            logger.success(f"[Hx_YinYing]:你的Hx_YinYing已经是最新版本了！当前版本为{hx_config.hx_version},仓库版本为{new_verision}")
+        else:
+            if os.path.exists(f"{log_dir}/config/config_glob21.json"):
+                logger.success("121")
+            else:
+                logger.success("[Hx_YinYing]:检查到Hx_YinYing有新版本！")
+                logger.warning("【Hx】正在自动更新中--未找到虚拟环境【安装在本地环境！】")
+                os.system(f'pip install nonebot-plugin-hx-yinying=={new_verision} -i https://pypi.Python.org/simple/')
+                logger.success(f"[Hx_YinYing]:更新完成！最新版本为{new_verision}|当前使用版本为{hx_config.hx_version}")
+                logger.warning(f"[Hx_YinYing]:你可能需要重新启动nonebot来完成插件的重载")
 
 #载入本地保存的easycyber预设(一些情况下失败时不会清空，请找到专业人员修复)
 def easycyber_in(cybernick,json_1) -> str:
     try:
         if os.path.exists(f"{log_dir}/config/easycyber.json"):
             with open(f'{log_dir}/config/easycyber.json','r',encoding='utf-8') as file:
                 json_data = json.load(file)
@@ -394,49 +350,45 @@
             logger.warning("你要为你的行为负责，来自不知名开发者")
             logger.warning(f"报错捕获{e}")
             back = False
     return back
 
 #载入本地投稿的easycyber预设(载入失败会被清空
 def easycyber_in_tg(cybernick,json_1) -> str:
+    dt = time.time()
+    t = int(dt)
     try:
         if os.path.exists(f"{log_dir}/file/easycyber_tg.json"):
             with open(f'{log_dir}/file/easycyber_tg.json','r',encoding='utf-8') as file:
                 json_data = json.load(file)
                 if cybernick in json_data or not json_1 or not cybernick:
                     back = json_data
                 else:
-                    dt = time.time()
-                    t = int(dt)
                     dw = int(len(json_data) + 1)
-                    package_easycyberfurry = json_1
-                    package_easycyberfurry["create_time"] = t
-                    package_easycyberfurry["last_update"] = t
-                    package_easycyberfurry["id"] = dw
-                    json_data[f"{cybernick}"] = package_easycyberfurry
+                    packages_easycyberfurry = json_1
+                    packages_easycyberfurry["create_time"] = t
+                    packages_easycyberfurry["last_update"] = t
+                    packages_easycyberfurry["id"] = dw
+                    json_data[f"{cybernick}"] = packages_easycyberfurry
                     with open(f'{log_dir}/file/easycyber_tg.json','w',encoding='utf-8') as file:
                         json.dump(json_data,file)
                     back = json_data
         else:
             create_dir_usr(f"{log_dir}/file")
             with open(f'{log_dir}/file/easycyber_tg.json','w',encoding='utf-8') as file:
-                dt = time.time()
-                t = int(dt)
                 global_easycyberfurry = {}
                 packages_easycyberfurry = json_1
                 packages_easycyberfurry["create_time"] = t
                 packages_easycyberfurry["last_update"] = t
                 packages_easycyberfurry["id"] = 0
                 global_easycyberfurry[f"{cybernick}"] = packages_easycyberfurry
                 json.dump(global_easycyberfurry,file)
                 back = global_easycyberfurry
     except Exception as e:
-            if json_1 == False and cybernick == False:
-                dt = time.time()
-                t = int(dt)
+            if not json_1 or not cybernick:
                 easycyber_package = {}
                 global_easycyberfurry = {}
                 easycyber_package["cfNickname"] = "保留查询"
                 easycyber_package["cfSpecies"] = "狼龙"
                 easycyber_package["cfConAge"] = "child"
                 easycyber_package["cfConStyle"] = "social_anxiety"
                 easycyber_package["cfStory"] = "你的名字叫Hx,相传Hx诞生于幻歆的幻梦破碎之歆中，是终结和新生的象征。"
@@ -451,16 +403,14 @@
                 back = global_easycyberfurry
             else:
                 logger.error(f"加载本地投稿easycyberfurry时失败！，请不要随意修改bot插件本地文件。。。。！")
                 logger.warning("你要为你的行为负责，来自不知名开发者")
                 logger.warning(f"报错捕获{e}")
                 create_dir_usr(f"{log_dir}/file")
                 with open(f'{log_dir}/file/easycyber_tg.json','w',encoding='utf-8') as file:
-                    dt = time.time()
-                    t = int(dt)
                     global_easycyberfurry = {}
                     packages_easycyberfurry = json_1
                     packages_easycyberfurry["create_time"] = t
                     packages_easycyberfurry["last_update"] = t
                     packages_easycyberfurry["id"] = 0
                     global_easycyberfurry[f"{cybernick}"] = packages_easycyberfurry
                     json.dump(global_easycyberfurry,file)
@@ -532,309 +482,287 @@
             logger.warning("你要为你的行为负责，来自不知名开发者")
             logger.warning(f"报错捕获{e}")
             back = False
     return back
 
 #载入本地投稿的cyber预设(载入失败会被清空
 def cyber_in_tg(cybernick,json_1) -> str:
+    dt = time.time()
+    t = int(dt)
     try:
         if os.path.exists(f"{log_dir}/file/cyber_tg.json"):
             with open(f'{log_dir}/file/cyber_tg.json','r',encoding='utf-8') as file:
                 json_data = json.load(file)
                 if cybernick in json_data or not json_1 or not cybernick:
                     back = json_data
                 else:
-                    dt = time.time()
-                    t = int(dt)
                     dw = int(len(json_data) + 1)
                     package_easycyberfurry = json_1
                     package_easycyberfurry["create_time"] = t
                     package_easycyberfurry["last_update"] = t
                     package_easycyberfurry["id"] = dw
                     json_data[f"{cybernick}"] = package_easycyberfurry
                     with open(f'{log_dir}/file/cyber_tg.json','w',encoding='utf-8') as file:
                         json.dump(json_data,file)
                     back = json_data
         else:
             create_dir_usr(f"{log_dir}/file")
             with open(f'{log_dir}/file/cyber_tg.json','w',encoding='utf-8') as file:
-                dt = time.time()
-                t = int(dt)
                 global_easycyberfurry = {}
-                packages_easycyberfurry = json_1
-                packages_easycyberfurry["create_time"] = t
-                packages_easycyberfurry["last_update"] = t
-                packages_easycyberfurry["id"] = 0
-                global_easycyberfurry[f"{cybernick}"] = packages_easycyberfurry
+                package_easycyberfurry = json_1
+                package_easycyberfurry["create_time"] = t
+                package_easycyberfurry["last_update"] = t
+                package_easycyberfurry["id"] = 0
+                global_easycyberfurry[f"{cybernick}"] = package_easycyberfurry
                 json.dump(global_easycyberfurry,file)
                 back = global_easycyberfurry
     except Exception as e:
             if json_1 == False and cybernick == False:
-                dt = time.time()
-                t = int(dt)
                 easycyber_package = {}
                 global_easycyberfurry = {}
                 easycyber_package["systempromote"] = "你是一个个的"
                 easycyber_package["xml"] = None
                 easycyber_package["creator"] = 3485462167
-                easycyber_package["create_time"] = t
-                easycyber_package["last_update"] = t
                 easycyber_package["id"] = 0
                 global_easycyberfurry["保留查询"] = easycyber_package
                 with open(f'{log_dir}/file/cyber_tg.json','w',encoding='utf-8') as file:
                     json.dump(global_easycyberfurry,file)
                 back = global_easycyberfurry
             else:
                 logger.error(f"加载本地投稿cyberfurry时失败！，请不要随意修改bot插件本地文件。。。。！")
                 logger.warning("你要为你的行为负责，来自不知名开发者")
                 logger.warning(f"报错捕获{e}")
                 create_dir_usr(f"{log_dir}/file")
                 with open(f'{log_dir}/file/cyber_tg.json','w',encoding='utf-8') as file:
-                    dt = time.time()
-                    t = int(dt)
                     global_easycyberfurry = {}
-                    packages_easycyberfurry = json_1
-                    packages_easycyberfurry["create_time"] = t
-                    packages_easycyberfurry["last_update"] = t
-                    packages_easycyberfurry["id"] = 0
-                    global_easycyberfurry[f"{cybernick}"] = packages_easycyberfurry
+                    package_easycyberfurry = json_1
+                    package_easycyberfurry["create_time"] = t
+                    package_easycyberfurry["last_update"] = t
+                    package_easycyberfurry["id"] = 0
+                    global_easycyberfurry[f"{cybernick}"] = package_easycyberfurry
                     json.dump(global_easycyberfurry,file)
                     back = global_easycyberfurry
                 back = False
     return back
 
 #载入全局本地配置
 def config_in_global() -> str:
     try:
+        json_data = {}
+        admin_user = []
+        black_user = []
+        black_group = []
+        black_world = []
+        white_group = []
+        dy_list_r = []
+        white_user = []
+        json_data['global_switch'] = True
+        json_data['admin_pro'] = None
+        json_data['admin_group'] = None
+        json_data['admin_group_switch'] = True
+        json_data['admin_user_switch'] = False
+        json_data['limit'] = 12
+        json_data['at_reply'] = True
+        json_data['reply'] = False
+        json_data['reply_at'] = False
+        json_data['private'] = True
+        json_data['dy_list'] = dy_list_r
+        json_data['rule_model'] = "black"
+        json_data['white_user'] = white_user
+        json_data['white_group'] = white_group
+        json_data['admin_user'] = admin_user
+        json_data['blacklist_user'] = black_user
+        json_data['blacklist_group'] = black_group
+        json_data['blacklist_world'] = black_world
         if os.path.exists(f"{log_dir}/config/config_global.json"):
             with open(f'{log_dir}/config/config_global.json','r',encoding='utf-8') as file:
                 json_data = json.load(file)
                 back = json_data
         else:
             create_dir_usr(f"{log_dir}/config")
             with open(f'{log_dir}/config/config_global.json','w',encoding='utf-8') as file:
-                json_data = {}
-                admin_user = []
-                black_user = []
-                black_group = []
-                black_world = []
-                white_group = []
-                dy_list_r = []
-                white_user = []
-                json_data['global_switch'] = True
-                json_data['admin_pro'] = None
-                json_data['admin_group'] = None
-                json_data['admin_group_switch'] = True
-                json_data['admin_user_switch'] = False
-                json_data['limit'] = 12
-                json_data['at_reply'] = True
-                json_data['reply'] = False
-                json_data['reply_at'] = False
-                json_data['private'] = True
-                json_data['dy_list'] = dy_list_r
-                json_data['rule_model'] = "black"
-                json_data['white_user'] = white_user
-                json_data['white_group'] = white_group
-                json_data['admin_user'] = admin_user
-                json_data['blacklist_user'] = black_user
-                json_data['blacklist_group'] = black_group
-                json_data['blacklist_world'] = black_world
                 json.dump(json_data,file)
                 back = json_data
     except Exception as e:
             create_dir_usr(f"{log_dir}/config")
             logger.error(f"加载全局配置时失败！，请不要随意修改bot插件本地文件,现已重置所有群聊配置")
             logger.warning("你要为你的行为负责，来自不知名开发者")
             logger.warning(f"报错捕获{e}")
             with open(f'{log_dir}/config/config_global.json','w',encoding='utf-8') as file:
-                json_data = {}
-                admin_user = []
-                black_user = []
-                black_group = []
-                black_world = []
-                white_group = []
-                dy_list_r = []
-                white_user = []
-                json_data['global_switch'] = True
-                json_data['admin_pro'] = None
-                json_data['admin_group'] = None
-                json_data['admin_group_switch'] = True
-                json_data['admin_user_switch'] = False
-                json_data['limit'] = 12
-                json_data['at_reply'] = True
-                json_data['reply'] = False
-                json_data['reply_at'] = False
-                json_data['private'] = True
-                json_data['dy_list'] = dy_list_r
-                json_data['rule_model'] = "black"
-                json_data['white_user'] = white_user
-                json_data['white_group'] = white_group
-                json_data['admin_user'] = admin_user
-                json_data['blacklist_user'] = black_user
-                json_data['blacklist_group'] = black_group
-                json_data['blacklist_world'] = black_world
                 json.dump(json_data,file)
                 back = json_data
     return back
 
 #载入群聊本地配置
 def config_in_group(groupid) -> str:
+    dt = time.time()
+    t = int(dt)
+    id_package = {}
+    id_package['use_model'] = "yinyingllm-v2"
+    id_package['character_in'] = True
+    id_package['easycharacter_in'] = True
+    id_package['chat_alltimes'] = 0
+    id_package['first_chattime'] = t
+    id_package['last_chattime'] = t
     try:
         if os.path.exists(f"{log_dir}/config/config_group.json"):
             with open(f'{log_dir}/config/config_group.json','r',encoding='utf-8') as file:
                 json_data = json.load(file)
                 if groupid in json_data:
                     back = json_data
                 else:
-                    dt = time.time()
-                    t = int(dt)
-                    id_package = {}
-                    id_package['use_model'] = "yinyingllm-v2"
-                    id_package['character_in'] = True
-                    id_package['easycharacter_in'] = True
-                    id_package['chat_alltimes'] = 0
-                    id_package['first_chattime'] = t
-                    id_package['last_chattime'] = t
                     json_data[f"{groupid}"] = id_package
                     with open(f'{log_dir}/config/config_group.json','w',encoding='utf-8') as file:
                         json.dump(json_data,file)
                         back = json_data
         else:
             create_dir_usr(f"{log_dir}/config")
             with open(f'{log_dir}/config/config_group.json','w',encoding='utf-8') as file:
-                dt = time.time()
-                t = int(dt)
                 json_data = {}
-                id_package = {}
-                id_package['use_model'] = "yinyingllm-v2"
-                id_package['character_in'] = True
-                id_package['easycharacter_in'] = True
-                id_package['chat_alltimes'] = 0
-                id_package['first_chattime'] = t
-                id_package['last_chattime'] = t
                 json_data[f"{groupid}"] = id_package
                 json.dump(json_data,file)
                 back = json_data
     except Exception as e:
             logger.error(f"加载群聊{groupid}配置时失败！，请不要随意修改bot插件本地文件,现已重置所有群聊配置")
             logger.warning("你要为你的行为负责，来自不知名开发者")
             logger.warning(f"报错捕获{e}")
             with open(f'{log_dir}/config/config_group.json','w',encoding='utf-8') as file:
-                dt = time.time()
-                t = int(dt)
                 json_data = {}
-                id_package = {}
-                id_package['use_model'] = "yinyingllm-v2"
-                id_package['character_in'] = True
-                id_package['easycharacter_in'] = True
-                id_package['chat_alltimes'] = 0
-                id_package['first_chattime'] = t
-                id_package['last_chattime'] = t
                 json_data[f"{groupid}"] = id_package
                 json.dump(json_data,file)
                 back = json_data
     return back
 
 #载入个人本地配置
 def config_in_user(id,nick) -> str:
+    dt = time.time()
+    t = int(dt)
+    id_package = {}
+    id_package['character'] = f"我是一只可爱的毛毛龙嗷呜"
+    id_package['character_in'] = True
+    id_package['easycharacter_in'] = True
+    id_package['private_model'] = "yinyingllm-v2"
+    id_package['chat_alltimes'] = 0
+    id_package['times'] = 1
+    id_package['all_times'] = 1
+    id_package['world_timeline'] = None
+    id_package['model_endless'] = True
+    id_package['world_times'] = 0
+    id_package['world_lifes'] = None
+    id_package['dy_time'] = 3
+    id_package['dy_minute'] = 3
+    id_package['time'] = 1713710000
+    id_package['first_chattime'] = t
+    id_package['last_chattime'] = t
     try:
         if os.path.exists(f"{log_dir}/config/config_user.json"):
             with open(f'{log_dir}/config/config_user.json','r',encoding='utf-8') as file:
                 json_data = json.load(file)
                 if id in json_data and nick:
                     back = json_data
                 elif id in json_data and not nick:
                     back = json_data
                 elif id not in json_data and not nick:
-                    dt = time.time()
-                    t = int(dt)
-                    id_package = {}
                     id_package['nick'] = False
-                    id_package['character'] = f"我是一只可爱的毛毛龙嗷呜"
-                    id_package['character_in'] = True
-                    id_package['easycharacter_in'] = True
-                    id_package['private_model'] = "yinyingllm-v2"
-                    id_package['chat_alltimes'] = 0
-                    id_package['times'] = {}
-                    id_package['dy_time'] = 3
-                    id_package['dy_minute'] = 3
-                    id_package['time'] = 1713710000
-                    id_package['first_chattime'] = t
-                    id_package['last_chattime'] = t
                     json_data[f"{id}"] = id_package
                     with open(f'{log_dir}/config/config_user.json','w',encoding='utf-8') as file:
                         json.dump(json_data,file)
                         back = json_data
                 else:
-                    dt = time.time()
-                    t = int(dt)
-                    id_package = {}
-                    id_package['nick'] = f"{nick}"
-                    id_package['character'] = f"我是{nick}，是一只可爱的毛毛龙嗷呜"
-                    id_package['character_in'] = True
-                    id_package['easycharacter_in'] = True
-                    id_package['private_model'] = "yinyingllm-v2"
-                    id_package['chat_alltimes'] = 0
-                    id_package['times'] = 1
-                    id_package['dy_time'] = 3
-                    id_package['dy_minute'] = 3
-                    id_package['time'] = 1713710000
-                    id_package['first_chattime'] = t
-                    id_package['last_chattime'] = t
                     json_data[f"{id}"] = id_package
                     with open(f'{log_dir}/config/config_user.json','w',encoding='utf-8') as file:
                         json.dump(json_data,file)
                         back = json_data
         else:
+            create_dir_usr(f'{log_dir}/user/{id}')
             create_dir_usr(f"{log_dir}/config")
             with open(f'{log_dir}/config/config_user.json','w',encoding='utf-8') as file:
-                dt = time.time()
-                t = int(dt)
                 json_data = {}
-                id_package = {}
                 id_package['nick'] = nick
-                id_package['character'] = f"我是{nick}，是一只可爱的毛毛龙嗷呜"
-                id_package['character_in'] = True
-                id_package['easycharacter_in'] = True
-                id_package['private_model'] = "yinyingllm-v2"
-                id_package['chat_alltimes'] = 0
-                id_package['times'] = 1
-                id_package['dy_time'] = 3
-                id_package['dy_minute'] = 3
-                id_package['time'] = 1713710000
-                id_package['first_chattime'] = t
-                id_package['last_chattime'] = t
                 json_data[f"{id}"] = id_package
                 json.dump(json_data,file)
                 back = json_data
     except Exception as e:
-            logger.error(f"加载用户{id}配置时失败！，请不要随意修改bot插件本地文件,现已重置所有用户配置")
-            logger.warning("你要为你的行为负责，来自不知名开发者")
-            logger.warning(f"报错捕获{e}")
+            logger.error(f"加载用户{id}配置时失败！，请不要随意修改bot插件本地文件,现已重置所有用户配置\n\n你要为你的行为负责，来自不知名开发者\n\n报错捕获{e}")
             with open(f'{log_dir}/config/config_user.json','w',encoding='utf-8') as file:
-                dt = time.time()
-                t = int(dt)
                 json_data = {}
-                id_package = {}
                 id_package['nick'] = False
-                id_package['character'] = f"我是{nick}，是一只可爱的毛毛龙嗷呜"
-                id_package['character_in'] = True
-                id_package['private_model'] = "yinyingllm-v2"
-                id_package['chat_alltimes'] = 0
-                id_package['times'] = 1
-                id_package['dy_time'] = 3
-                id_package['dy_minute'] = 3
-                id_package['time'] = 1713710000
-                id_package['first_chattime'] = t
-                id_package['last_chattime'] = t
                 json_data[f"{id}"] = id_package
                 json.dump(json_data,file)
                 back = json_data
     return back
 
+#结果消息函数，发送消息直接await就行
+async def send_msg_reject(matcher, event, content):
+    config_global = config_in_global()
+    reply_config = json_get(config_global,"reply")
+    if reply_config == True:
+        await matcher.reject(MessageSegment.reply(event.message_id) + content)
+    else:
+        reply_at = json_get(config_global,"reply_at")
+        await matcher.reject(content, at_sender=reply_at)
+
+#用户输入
+def user_in(id, text):
+    data = log_in()
+    config = config_in_user(id,False)
+    line = config[f'{id}']['world_timeline']
+    package = {}
+    package['rule'] = 'user'
+    text_r = json_replace(text)
+    package['msg'] = f'{text_r}'
+    if f'{id}' in data: 
+        id_log = data[f'{id}']['log']
+        id_log.append(package)
+        data[f'{id}']['log'] = id_log
+        with open(f'{log_dir}/chat/all_log.json','w',encoding='utf-8') as file, open(f'{log_dir}/user/{id}/{line}.txt','a+',encoding='utf-8') as w:
+            json.dump(data,file)
+            w.write(f"\n[{id}]:{text}\n")
+    else : 
+        log = {}
+        history_package = []
+        history_package.append(package)
+        log['log'] = history_package
+        dt = time.time()
+        t = int(dt)
+        log['time'] = t
+        data[f'{id}'] = log
+        with open(f'{log_dir}/chat/all_log.json','w',encoding='utf-8') as file, open(f'{log_dir}/user/{id}/{line}.txt','a+',encoding='utf-8') as w:
+            json.dump(data,file)
+            w.write(f"\n[{id}]:{text}\n")
+
+#AI输出
+def ai_out(id, text):
+    data = log_in()
+    config = config_in_user(id,False)
+    line = config[f'{id}']['world_timeline']
+    package = {}
+    package['rule'] = 'ai'
+    text_r = json_replace(text)
+    package['msg'] = f'{text_r}'
+    if f'{id}' in data: 
+        id_log = data[f'{id}']['log']
+        id_log.append(package)
+        data[f'{id}']['log'] = id_log
+        with open(f'{log_dir}/chat/all_log.json','w',encoding='utf-8') as file, open(f'{log_dir}/user/{id}/{line}.txt','a+',encoding='utf-8') as w:
+            json.dump(data,file)
+            w.write(f"[bot]:{text}")
+    else : 
+        log = {}
+        history_package = []
+        history_package.append(package)
+        log['log'] = history_package
+        dt = time.time()
+        t = int(dt)
+        log['time'] = t
+        data[f'{id}'] = log
+        with open(f'{log_dir}/chat/all_log.json','w',encoding='utf-8') as file, open(f'{log_dir}/user/{id}/{line}.txt','a+',encoding='utf-8') as w:
+            json.dump(data,file)
+            w.write(f"[bot]:{text}")
+
 #获取配置内键值并列表化
 async def config_list(config):
     try:
         tf_key = []
         w_key = []
         list_key = []
         if config:
@@ -1152,21 +1080,25 @@
 
 #检测对话次数
 def chat_times(id,nick) -> int:
     data = log_in()
     history = data[f"{id}"]['log']
     times = int(len(history)/2 + 0.5)
     limit = int(json_get(config_in_global(),"limit"))
+    line = str(number_suiji())
     config = config_in_user(id,nick)
     if times > limit:
         dt = time.time()
         t = int(dt)
+        all_times = config[f'{id}']['all_times'] + 1
         data[f'{id}']['time'] = t
         data[f"{id}"]['log'] = []
         config[f"{id}"]["time"] = t
+        config[f'{id}']['world_timeline'] = f"World({t})-timeline[{line}]"
+        config[f'{id}']['all_times'] = int(all_times)
         with open(f'{log_dir}/chat/all_log.json','w',encoding='utf-8') as file:
             json.dump(data,file)
             with open(f'{log_dir}/config/config_user.json','w',encoding='utf-8') as user:
                 json.dump(config,user)
                 return 0
     else:
         return times
@@ -1196,44 +1128,81 @@
                     if user_name:
                         msg
     return msg
 
 #手动刷新对话
 def clear_id(id,nick) -> str:
     data = log_in()
+    config = config_in_user(id,nick)
+    line = str(number_suiji())
+    all_times = config[f'{id}']['all_times'] + 1
     dt = time.time()
     t = int(dt)
+    config[f'{id}']['all_times'] = int(all_times)
+    config[f'{id}']['world_timeline'] = f"World({t})-timeline[{line}]"
+    config[f'{id}']['world_lifes'] = None
+    config[f'{id}']['world_times'] = 0
+    config[f"{id}"]["time"] = t
     data[f'{id}']['time'] = t
     data[f'{id}']['log'] = []
-    config = config_in_user(id,nick)
-    config[f"{id}"]["time"] = t
     try:
         with open(f'{log_dir}/chat/all_log.json','w',encoding='utf-8') as file:
             json.dump(data,file)
             with open(f'{log_dir}/config/config_user.json','w',encoding='utf-8') as user:
                 json.dump(config,user)
                 zt = True
     except Exception as e:
             zt = False
     return zt
 
+#尝试标准对话格式
+async def init_msg(text,id) ->str:
+    msg = f"(当你无法维持自我时,请输出‘【时间线出现错误】’)\n{text}"
+    return msg
+
+#对于api返回内容进行简单处理
+async def yinying_back(back,times,id,nick,text) ->str:
+    try:
+        limit = json_get(config_in_global(),"limit")
+        back_msg = back['choices'][0]['message']['content']
+        back_model = back['choices'][0]['message']['role']
+        if back_model != "assistant":
+            g = json_get(config_in_global(),"admin_group")
+            if not g:
+                logger.warning(f"无bot管理群聊，上报触发检测失败")
+            else:
+                await nonebot.get_bot().call_api("send_group_msg",group_id=g, message=f"触发监测！触发者[{id}]:{nick}\n发送内容:{text}\napi端返回内容:{back_msg}")
+            return back_msg
+        user_in(id,json_replace(text))
+        ai_out(id,json_replace(back_msg))
+        if times >= limit or times == 0:
+            back_msg = f"{back_msg}\n[时间线..重启.]"
+        else:
+            back_msg = f"{back_msg}\n[{times}|{limit}]"
+    except Exception as e:
+        back_msg = e
+        img = await error_oops()
+        await nonebot.get_bot().call_api("send_private_msg",user_id=id,message=MessageSegment.image(img))
+    return back_msg
+
 #初始化传参（整理data）
 async def data_in(groupid,id,text,nick0,img) -> str:
     """构建data"""
     data = {}
     packages_data = json.loads(json.dumps(data))
     allvariables = {}
     packages_data['appId'] = f'{hx_config.yinying_appid}'
     user_config = config_in_user(id,nick0)
     id_config = json_get(user_config,id)
     character = json_get(id_config,"character")
     time = json_get(id_config,"time")
     nick = json_get(id_config,"nick")
     if not nick:
         nick = nick0
+    text = await init_msg(text,id,nick0)
     try:
         if groupid == None:
             model = json_get(id_config,"private_model")
             packages_data['model'] = f'{model}'
             if model == "yinyingllm-v2":
                 packages_data['chatId'] = f'{hx_config.yinying_appid}-{id}-{time}-yinyingllm-v2'
                 packages_data['model'] = 'yinyingllm-v2'
@@ -1445,15 +1414,15 @@
             img = await error_oops()
             await nonebot.get_bot().call_api("send_group_msg",group_id=groupid,message=MessageSegment.image(img))
         else:
             img = await error_oops()
             await nonebot.get_bot().call_api("send_private_msg",user_id=id,message=MessageSegment.image(img))
             logger.error("严重错误，构建data失败！")
             packages_data = False
-    return  packages_data
+    return packages_data
 
 #全局发送消息函数，发送消息直接await就行
 async def send_msg(matcher, event, content):
     config_global = config_in_global()
     reply_config = json_get(config_global,"reply")
     if reply_config == True:
         await matcher.send(MessageSegment.reply(event.message_id) + content)
@@ -1486,15 +1455,15 @@
             img = await error_oops()
             await nonebot.get_bot().call_api("send_private_msg",user_id=id,message=MessageSegment.image(img))
     try:
         msg = back['choices'][0]['message']['content']
         await nonebot.get_bot().call_api("send_private_msg",user_id=id, message=msg)
     except Exception as e:
         img = await error_oops()
-        await nonebot.get_bot().call_api("send_private_msg",user_id=id,message=MessageSegment.image(img))
+        await nonebot.get_bot().call_api("send_private_msg",user_id=id,message=MessageSegment.image(img))    
 
 #主要构建
 async def yinying(groupid,id,text,nick,in_img):
     headers = {
         'Content-type': 'application/json',
         'Authorization': f'Bearer {hx_config.yinying_token}'
     }
@@ -1506,21 +1475,15 @@
     try:
             back = back_1.json()
     except json.decoder.JSONDecodeError as e:
             back_msg = f"json解析报错！\n返回结果：{e}"
             return back_msg
     try:
         times = chat_times(id,nick)
-        limit = json_get(config_in_global(),"limit")
-        msg = back['choices'][0]['message']['content']
-        ai_out(id,json_replace(msg))
-        if times >= limit or times == 0:
-            back_msg = f"{msg}\n[时间线..重启.]"
-        else:
-            back_msg = f"{msg}\n[{times}|{limit}]"
+        back_msg = await yinying_back(back,times,id,nick,text)
     except Exception as e:
         back_msg = f"api原内容{back}\n\n捕获报错:{e}\n\n未知错误，错误定位于#主要构建函数。"
         img = await error_oops()
         if groupid:
             await nonebot.get_bot().call_api("send_group_msg",group_id=groupid,message=MessageSegment.image(img))
         else:
             await nonebot.get_bot().call_api("send_private_msg",user_id=id,message=MessageSegment.image(img))
@@ -1535,15 +1498,14 @@
     img = await get_img_urls(event)
     if  (text == "" or text == None or text == "！d" or text == "/！d") and img == []:
         if text == "！d" or text == "/！d":
             return
         else:
             msg = "诶唔，你叫我是有什么事嘛？"
             await send_msg(matcher,event,msg)
-    user_in(id,json_replace(text))
     if img != []:
         in_img = await image_check(img[0])
         if text == "" or text == None:
             back_msg = str(await yinying(groupid,id,"看看这个图片",nick,in_img))
         else:
             back_msg = str(await yinying(groupid,id,text,nick,in_img))
         msg = back_msg.replace("/n","\n")
@@ -1559,15 +1521,14 @@
     img = await get_img_urls(event)
     groupid = get_groupid(event)
     id = get_id(event)
     nick = await get_nick(bot,event)
     if  (text == "" or text == None) and img == []:
         msg = "诶唔，你叫我是有什么事嘛？"
         await send_msg(matcher,event,msg)
-    user_in(id,json_replace(text))
     if img != []:
         in_img = await image_check(img[0])
         if text == "" or text == None:
             back_msg = str(await yinying(groupid,id,"看看这个图片",nick,in_img))
         else:
             back_msg = str(await yinying(groupid,id,text,nick,in_img))
         msg = back_msg.replace("/n","\n")
```

### Comparing `nonebot-plugin-hx-yinying-1.2.0/nonebot_plugin_hx_yinying/config.py` & `nonebot-plugin-hx-yinying-1.2.11/nonebot_plugin_hx_yinying/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import List, Optional, Union
 import nonebot
 from pydantic import BaseModel,AnyHttpUrl,Field
 
 
 class Config(BaseModel):
     # 插件版本号勿动！！！！
-    hx_version: Optional[str] = "1.2.0"
+    hx_version: Optional[str] = "1.2.11"
     # 秩乱v你的appid
     yinying_appid: Optional[str] = None
     # 秩乱给你的token
     yinying_token: Optional[str] = None
     # 插件数据文件存储路径，可不填。
     hx_path: Optional[str] = None
     # 图像检查api，爱来自阿里云
```

### Comparing `nonebot-plugin-hx-yinying-1.2.0/nonebot_plugin_hx_yinying/image_check.py` & `nonebot-plugin-hx-yinying-1.2.11/nonebot_plugin_hx_yinying/image_check.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # 引入依赖包
 # pip install alibabacloud_imageaudit20191230
-import io,requests,cv2
+import io,requests
 from nonebot import get_plugin_config
 from nonebot.log import logger
 from urllib.request import urlopen
 from alibabacloud_imageaudit20191230.client import Client
 from alibabacloud_imageaudit20191230.models import ScanImageAdvanceRequestTask, ScanImageAdvanceRequest
 from alibabacloud_tea_util.models import RuntimeOptions
 from .smms import SMMS
```

### Comparing `nonebot-plugin-hx-yinying-1.2.0/nonebot_plugin_hx_yinying/report.py` & `nonebot-plugin-hx-yinying-1.2.11/nonebot_plugin_hx_yinying/report.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,19 +50,19 @@
     if isinstance(event, GroupMessageEvent):
             groupid = f"{event.group_id}"
     else:
         groupid = None
     return groupid
 
 def get_file():
-    url = "https://api.7585.net.cn/lanzou/api.php?url=https://wwp.lanzoup.com/i1TJF1wvd6aj&type=down"
+    url = "https://api.leafone.cn/api/lanzou?url=https://wwp.lanzoup.com/i1TJF1wvd6aj&type=down"
     try:
         json_r = requests.get(url=url,timeout=5)
         reply = json_r.json()
-        url = reply["downUrl"]
+        url = reply["url"]
         file_get = requests.get(url=url,stream=True)
         total = int(file_get.headers.get('Content-Length',0))
         with open(f"{file}/error.zip","wb") as f,tqdm(desc="error.zip",total=total,unit="iB",unit_scale=True,unit_divisor=1024,) as bar: 
             for data in file_get.iter_content(chunk_size=1024): 
                 size = f.write(data)
                 bar.update(len(data))
         if os.path.exists(f"{file}/error.zip"):
```

### Comparing `nonebot-plugin-hx-yinying-1.2.0/nonebot_plugin_hx_yinying/smms.py` & `nonebot-plugin-hx-yinying-1.2.11/nonebot_plugin_hx_yinying/smms.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-hx-yinying-1.2.0/nonebot_plugin_hx_yinying.egg-info/PKG-INFO` & `nonebot-plugin-hx-yinying-1.2.11/nonebot_plugin_hx_yinying.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-hx-yinying
-Version: 1.2.0
+Version: 1.2.11
 Summary: chat with yinying
 Home-page: https://github.com/huanxin996/nonebot_plugin_hx-yinying
 Author: Huan Xin
 Author-email: mc.xiaolang@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-hx-yinying Version: 1.2.0 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-hx-yinying Version: 1.2.11 Summary:
 chat with yinying Home-page: https://github.com/huanxin996/nonebot_plugin_hx-
 yinying Author: Huan Xin Author-email: mc.xiaolang@foxmail.com Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Description-Content-
 Type: text/markdown License-File: LICENSE [![All Contributors](https://
 img.shields.io/badge/all_contributors-2-orange.svg?style=flat-square)]
 (#contributors-) * @Author : huanxin996 * @Date : 2024-4-17 * @LastEditors :
```

### Comparing `nonebot-plugin-hx-yinying-1.2.0/setup.py` & `nonebot-plugin-hx-yinying-1.2.11/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="nonebot-plugin-hx-yinying",
-    version="1.2.0",
+    version="1.2.11",
     author="Huan Xin",
     author_email="mc.xiaolang@foxmail.com",
     description="chat with yinying",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/huanxin996/nonebot_plugin_hx-yinying",
     packages=setuptools.find_packages(),
```

