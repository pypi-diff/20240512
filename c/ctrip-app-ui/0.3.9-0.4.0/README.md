# Comparing `tmp/ctrip-app-ui-0.3.9.tar.gz` & `tmp/ctrip-app-ui-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctrip-app-ui-0.3.9.tar", last modified: Sat Apr 27 10:28:36 2024, max compression
+gzip compressed data, was "ctrip-app-ui-0.4.0.tar", last modified: Sat May 11 17:24:22 2024, max compression
```

## Comparing `ctrip-app-ui-0.3.9.tar` & `ctrip-app-ui-0.4.0.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-04-27 10:28:36.254396 ctrip-app-ui-0.3.9/
--rw-rw-rw-   0        0        0    11558 2024-04-27 01:24:22.000000 ctrip-app-ui-0.3.9/LICENSE
--rw-rw-rw-   0        0        0      474 2024-04-27 10:28:36.253900 ctrip-app-ui-0.3.9/PKG-INFO
--rw-rw-rw-   0        0        0       47 2024-04-27 01:24:22.000000 ctrip-app-ui-0.3.9/README.md
-drwxrwxrwx   0        0        0        0 2024-04-27 10:28:36.250423 ctrip-app-ui-0.3.9/capp_ui/
--rw-rw-rw-   0        0        0      470 2024-04-27 01:24:22.000000 ctrip-app-ui-0.3.9/capp_ui/__init__.py
--rw-rw-rw-   0        0        0     3628 2024-04-27 02:13:31.000000 ctrip-app-ui-0.3.9/capp_ui/date_extend.py
--rw-rw-rw-   0        0        0     1191 2024-04-27 01:24:22.000000 ctrip-app-ui-0.3.9/capp_ui/device.py
--rw-rw-rw-   0        0        0     1391 2024-04-27 01:24:22.000000 ctrip-app-ui-0.3.9/capp_ui/dir.py
--rw-rw-rw-   0        0        0    59908 2024-04-27 10:27:48.000000 ctrip-app-ui-0.3.9/capp_ui/domain_service.py
--rw-rw-rw-   0        0        0      613 2024-04-27 01:24:22.000000 ctrip-app-ui-0.3.9/capp_ui/fee.py
--rw-rw-rw-   0        0        0     2270 2024-04-27 01:24:22.000000 ctrip-app-ui-0.3.9/capp_ui/libs.py
--rw-rw-rw-   0        0        0    23814 2024-04-27 01:24:22.000000 ctrip-app-ui-0.3.9/capp_ui/mobile_terminals.py
--rw-rw-rw-   0        0        0     1799 2024-04-27 01:24:22.000000 ctrip-app-ui-0.3.9/capp_ui/platforms.py
--rw-rw-rw-   0        0        0      689 2024-04-27 01:24:22.000000 ctrip-app-ui-0.3.9/capp_ui/test.py
--rw-rw-rw-   0        0        0     5563 2024-04-27 01:24:22.000000 ctrip-app-ui-0.3.9/capp_ui/utils.py
--rw-rw-rw-   0        0        0     3016 2024-04-27 01:24:22.000000 ctrip-app-ui-0.3.9/capp_ui/validators.py
-drwxrwxrwx   0        0        0        0 2024-04-27 10:28:36.253403 ctrip-app-ui-0.3.9/ctrip_app_ui.egg-info/
--rw-rw-rw-   0        0        0      474 2024-04-27 10:28:36.000000 ctrip-app-ui-0.3.9/ctrip_app_ui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      442 2024-04-27 10:28:36.000000 ctrip-app-ui-0.3.9/ctrip_app_ui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-27 10:28:36.000000 ctrip-app-ui-0.3.9/ctrip_app_ui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2024-04-27 10:28:36.000000 ctrip-app-ui-0.3.9/ctrip_app_ui.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-27 10:28:36.000000 ctrip-app-ui-0.3.9/ctrip_app_ui.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-27 10:28:36.254893 ctrip-app-ui-0.3.9/setup.cfg
--rw-rw-rw-   0        0        0     1087 2024-04-27 10:28:27.000000 ctrip-app-ui-0.3.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-11 17:24:22.013197 ctrip-app-ui-0.4.0/
+-rw-rw-rw-   0        0        0    11558 2024-04-24 09:02:35.000000 ctrip-app-ui-0.4.0/LICENSE
+-rw-rw-rw-   0        0        0      474 2024-05-11 17:24:22.012227 ctrip-app-ui-0.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0       47 2024-04-24 09:02:35.000000 ctrip-app-ui-0.4.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-11 17:24:22.001230 ctrip-app-ui-0.4.0/capp_ui/
+-rw-rw-rw-   0        0        0      470 2024-04-24 09:06:21.000000 ctrip-app-ui-0.4.0/capp_ui/__init__.py
+-rw-rw-rw-   0        0        0      736 2024-05-06 07:02:29.000000 ctrip-app-ui-0.4.0/capp_ui/config.py
+-rw-rw-rw-   0        0        0     4060 2024-05-07 16:57:27.000000 ctrip-app-ui-0.4.0/capp_ui/date_extend.py
+-rw-rw-rw-   0        0        0     1664 2024-05-09 13:31:21.000000 ctrip-app-ui-0.4.0/capp_ui/device.py
+-rw-rw-rw-   0        0        0     1391 2024-04-25 08:27:58.000000 ctrip-app-ui-0.4.0/capp_ui/dir.py
+-rw-rw-rw-   0        0        0    63525 2024-05-11 17:23:53.000000 ctrip-app-ui-0.4.0/capp_ui/domain_service.py
+-rw-rw-rw-   0        0        0      613 2024-04-24 15:31:00.000000 ctrip-app-ui-0.4.0/capp_ui/fee.py
+-rw-rw-rw-   0        0        0     3859 2024-05-11 16:34:35.000000 ctrip-app-ui-0.4.0/capp_ui/libs.py
+-rw-rw-rw-   0        0        0    24704 2024-05-11 03:15:13.000000 ctrip-app-ui-0.4.0/capp_ui/mobile_terminals.py
+-rw-rw-rw-   0        0        0     1719 2024-04-28 16:15:39.000000 ctrip-app-ui-0.4.0/capp_ui/platforms.py
+-rw-rw-rw-   0        0        0      765 2024-04-28 16:02:26.000000 ctrip-app-ui-0.4.0/capp_ui/test.py
+-rw-rw-rw-   0        0        0     5486 2024-05-11 03:13:30.000000 ctrip-app-ui-0.4.0/capp_ui/utils.py
+-rw-rw-rw-   0        0        0     3023 2024-05-11 03:13:43.000000 ctrip-app-ui-0.4.0/capp_ui/validators.py
+drwxrwxrwx   0        0        0        0 2024-05-11 17:24:22.011203 ctrip-app-ui-0.4.0/ctrip_app_ui.egg-info/
+-rw-rw-rw-   0        0        0      474 2024-05-11 17:24:21.000000 ctrip-app-ui-0.4.0/ctrip_app_ui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      460 2024-05-11 17:24:21.000000 ctrip-app-ui-0.4.0/ctrip_app_ui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-11 17:24:21.000000 ctrip-app-ui-0.4.0/ctrip_app_ui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2024-05-11 17:24:21.000000 ctrip-app-ui-0.4.0/ctrip_app_ui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-11 17:24:21.000000 ctrip-app-ui-0.4.0/ctrip_app_ui.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-11 17:24:22.013197 ctrip-app-ui-0.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     1103 2024-05-11 17:24:16.000000 ctrip-app-ui-0.4.0/setup.py
```

### Comparing `ctrip-app-ui-0.3.9/LICENSE` & `ctrip-app-ui-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.3.9/capp_ui/date_extend.py` & `ctrip-app-ui-0.4.0/capp_ui/date_extend.py`

 * *Files 9% similar despite different names*

```diff
@@ -87,18 +87,27 @@
     return dt_step.strftime(standard_date_format)
 
 
 def current_datetime_str() -> str:
     return datetime.now().strftime(standard_date_format)
 
 
-def is_later_than_current_time(time_str: str, minutes: int = 5):
-    # 将给定时间字符串转换为 datetime 对象
-    given_time = datetime.strptime(time_str, '%H:%M')
-    # 获取当前时间
-    current_datatime = datetime.now()
-    current_time_str = current_datatime.strftime("%H:%M")
-    current_time = datetime.strptime(current_time_str, '%H:%M')
-    # 计算当前时间之后5分钟的时间
-    five_minutes_later = current_time + timedelta(minutes=minutes)
-    # 比较给定时间是否晚于当前时间5分钟后的时间
-    return given_time > five_minutes_later
+def is_later_than_current_time(time_str: str, minutes: int = 5, current_dt: str = None):
+    # 将给定的时间字符串转换为 datetime 对象
+    given_time = datetime.strptime(time_str, '%H:%M').time()
+    if current_dt is None:
+        # 获取当前日期和时间
+        current_datetime = datetime.now()
+    else:
+        current_datetime = datetime.strptime(current_dt, standard_date_format)
+    current_time = current_datetime.time()
+    # 如果给定时间跨越了当前日期，则调整为明天的时间
+    if given_time < current_time:
+        given_date = (current_datetime + timedelta(days=1)).date()
+    else:
+        given_date = current_datetime.date()
+    # 合并给定时间的日期和当前日期的时间
+    given_datetime = datetime.combine(given_date, given_time)
+    # 计算给定时间与当前时间的差值
+    time_difference = given_datetime - current_datetime
+    # 判断差值是否大于 多少 分钟
+    return time_difference.total_seconds() > minutes * 60
```

### Comparing `ctrip-app-ui-0.3.9/capp_ui/dir.py` & `ctrip-app-ui-0.4.0/capp_ui/dir.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.3.9/capp_ui/domain_service.py` & `ctrip-app-ui-0.4.0/capp_ui/domain_service.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,167 +6,158 @@
 # Description:  TODO
 # Author:       mfkifhss2023
 # CreateDate:   2024/04/24
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
 import re
+import time
 import typing as t
 from decimal import Decimal
 from poco.proxy import UIObjectProxy
 from poco.exceptions import PocoNoSuchNodeException, PocoTargetTimeout
 
 from capp_ui.platforms import PlatformService
 from capp_ui.mobile_terminals import stop_app
-from capp_ui.libs import SleepWait, LoopFindElement
-from capp_ui.utils import logger, get_ui_object_proxy_attr
+from capp_ui.utils import get_ui_object_proxy_attr
+from capp_ui.config import ctrip_soft_keyboard_position
 from capp_ui.date_extend import is_later_than_current_time
 from capp_ui.dir import get_images_dir, is_exists, join_path
 from capp_ui.date_extend import get_trip_year_month_day, get_datetime_area, is_public_holiday
+from capp_ui.libs import SleepWait, LoopFindElement, LoopFindElementSubmit, logger, LoopClickElement
 
 
-class CtripAppService(PlatformService):
+class CtripAppService(object):
     """
     携程APP
     """
     IMAGE_DIR = get_images_dir()
 
-    def __init__(self, device=None, app_name: str = None, *args, **kwargs) -> None:
+    def __init__(self, device_id: str, port: int = 0, enable_debug: bool = False, platform: str = "Android",
+                 app_name: str = None, *args, **kwargs) -> None:
         super().__init__(*args, **kwargs)
         self.app_name = app_name or "ctrip.android.view"
-        self.device = device or PlatformService().device
+        self.device = PlatformService(device_id=device_id, enable_debug=enable_debug, platform=platform,
+                                      port=port).device
 
     def start(self) -> None:
         self.device.start_app(self.app_name)
 
     def stop(self) -> None:
-        stop_app(self.app_name)
+        stop_app(self.app_name, device_id=self.device.device_id)
 
-    def restart(self) -> None:
-        stop_app(self.app_name)
+    @LoopFindElementSubmit(loop=1, action="重启应用")
+    def restart(self):
+        stop_app(self.app_name, device_id=self.device.device_id)
         self.device.start_app(self.app_name)
 
-    def hide_navigation_bar(self) -> None:
+    def hide_navigation_bar(self):
         """如果导航栏已打开，需要隐藏，导航栏很影响元素定位"""
         try:
             navigation_bar = self.device.get_po(
                 type="android.widget.ImageView", name="com.android.systemui:id/hide", desc="隐藏"
             )
-            if navigation_bar.exists():
-                navigation_bar.click()
-        except (PocoNoSuchNodeException, Exception):
-            logger.warning("导航栏没有打开，无需处理.")
+            navigation_bar.click()
+            logger.warning("手机导航栏已被隐藏")
+        except (PocoNoSuchNodeException, PocoTargetTimeout):
+            logger.warning("手机没有开启导航栏")
+        except Exception as e:
+            logger.error("导航栏元素定位失败，error: {}".format(e))
 
-    @SleepWait(wait_time=1)
-    def touch_home(self) -> None:
+    @LoopFindElementSubmit(loop=3, action="首页")
+    def touch_home(self):
         """进入app后，点击【首页】"""
         file_name = join_path([get_images_dir(), "首页.png"])
         if is_exists(file_name):
             temp = self.device.get_cv_template(file_name=file_name)
         else:
             temp = (154, 2878)  # LG g7手机上对应的坐标位置，其他型号手机可能不是这个值
         self.device.touch(v=temp)
 
-    @SleepWait(wait_time=1)
-    def touch_my(self) -> None:
+    @LoopFindElementSubmit(loop=2, action="我的")
+    def touch_my(self):
         """进入app后，点击【我的】"""
         my_button = self.device.poco(type="android.view.ViewGroup", name="ctrip.android.view:id/a", desc="我的")
         my_button.click()
 
-    @SleepWait(wait_time=1)
+    @LoopFindElementSubmit(loop=1, action="设置")
     def touch_settings(self):
         """我的主页，点击【设置】"""
         setting_button = self.device.poco(type="android.widget.ImageView", name="ctrip.android.view:id/a", desc="设置")
         setting_button.click()
 
-    @SleepWait(wait_time=1)
+    @LoopFindElementSubmit(loop=1, action="退出")
     def touch_logout_user(self):
         """在设置界面，点击【退出登录】"""
         self.device.quick_slide_screen(duration=1)
-        try:
-            logout_user = self.device.poco(
-                type="android.widget.Button", name="ctrip.android.view:id/a", text="退出登录"
-            )
-            if logout_user.exists() is True:
-                logout_user.click()
-        except (PocoNoSuchNodeException,):
-            pass
+        logout_user = self.device.poco(
+            type="android.widget.Button", name="ctrip.android.view:id/a", text="退出登录"
+        )
+        logout_user.click()
 
-    @SleepWait(wait_time=1)
+    @LoopFindElementSubmit(loop=1, action="确认退出")
     def touch_submit_logout(self):
         """退出登录弹框，点击【确定】"""
-        try:
-            logout_user = self.device.poco(
-                type="android.widget.TextView", name="ctrip.android.view:id/a", text="确定"
-            )
-            if logout_user.exists() is True:
-                logout_user.click()
-        except (PocoNoSuchNodeException,):
-            pass
+        logout_user = self.device.poco(
+            type="android.widget.TextView", name="ctrip.android.view:id/a", text="确定"
+        )
+        logout_user.click()
 
-    @SleepWait(wait_time=1)
-    def touch_unpaid(self) -> None:
+    def touch_unpaid(self) -> bool:
         """进入my主页后，点击【待付款】"""
+        flag = False
         try:
-            # 登录后的待付款元素定位
-            login_unpaid_button = self.device.poco(
+            # 待付款元素定位1
+            unpaid_button_1 = self.device.poco(
                 type="android.widget.TextView", name="ctrip.android.view:id/a", text="待付款"
             )
-            # 未登录的待付款元素定位
-            logout_unpaid_button = self.device.poco(
-                type="android.widget.TextView", name="android.widget.TextView", text="待付款"
-            )
-            if login_unpaid_button.exists() is True:
-                login_unpaid_button.click()
-            elif logout_unpaid_button.exists() is True:
-                logout_unpaid_button.click()
-            else:
-                logger.warning("没有找到待付款按钮")
-        except (PocoNoSuchNodeException, PocoTargetTimeout):
+            unpaid_button_1.click()
+            flag = True
+            time.sleep(1)
+        except (Exception,):
             pass
-        except Exception as e:
-            logger.error(e)
+        if flag is False:
+            try:
+                # 待付款元素定位2
+                unpaid_button_2 = self.device.poco(
+                    type="android.widget.TextView", name="android.widget.TextView", text="待付款"
+                )
+                unpaid_button_2.click()
+                flag = True
+                time.sleep(1)
+            except (Exception,):
+                pass
+        return flag
 
-    @SleepWait(wait_time=1)
-    def touch_list_page_search_box(self) -> None:
+    @LoopFindElementSubmit(loop=3, action="列表页搜索框")
+    def touch_list_page_search_box(self):
         """进入待付款列表页，点击【搜索框】"""
-        try:
-            search_box = self.device.poco(
-                type="android.widget.TextView", name="android.widget.TextView", text="搜索订单"
-            )
-            search_box.click()
-        except (PocoNoSuchNodeException, PocoTargetTimeout):
-            pass
-        except Exception as e:
-            logger.error(e)
+        search_box = self.device.poco(
+            type="android.widget.TextView", name="android.widget.TextView", text="搜索订单"
+        )
+        search_box.click()
 
-    @SleepWait(wait_time=1)
-    def touch_search_page_search_box(self, ctrip_order_id: str) -> None:
+    @LoopFindElementSubmit(loop=3, action="搜索页搜索框")
+    def touch_search_page_search_box(self, ctrip_order_id: str):
         """进入搜索页，点击【搜索框】"""
-        try:
-            search_box = self.device.poco(
-                type="android.widget.EditText", name="android.widget.EditText", text="输入城市名/订单号 搜索订单"
-            )
-            search_box.click()
-            search_box.set_text(ctrip_order_id)
-            # 模拟键盘按下回车键（keyCode为66表示回车键）
-            # self.device.poco.device.input(keyevent="66")
-            self.device.keyevent(keyname="66")
-        except (PocoNoSuchNodeException, PocoTargetTimeout):
-            pass
-        except Exception as e:
-            logger.error(e)
+        search_box = self.device.poco(
+            type="android.widget.EditText", name="android.widget.EditText", text="输入城市名/订单号 搜索订单"
+        )
+        search_box.click()
+        search_box.set_text(ctrip_order_id)
+        # 模拟键盘按下回车键（keyCode为66表示回车键）
+        self.device.keyevent(keyname="66")
 
     @SleepWait(wait_time=1)
     def is_exist_to_payment_at_list_page(self) -> bool:
         """检查搜索列表界面，是否存在【去支付】按钮"""
         flag = False
         try:
-            search_box = self.device.poco(type="android.widget.TextView", name="android.widget.TextView", text="去支付")
-            if search_box.exists() is True:
+            is_exist = self.device.poco(type="android.widget.TextView", name="android.widget.TextView", text="去支付")
+            if is_exist.exists() is True:
                 flag = True
         except (PocoNoSuchNodeException, PocoTargetTimeout):
             pass
         except Exception as e:
             logger.error(e)
         return flag
 
@@ -174,51 +165,72 @@
     def get_order_status(self) -> str:
         """检查搜索列表界面，获取订单的状态"""
         status = None
         try:
             unpaid_status = self.device.poco(
                 type="android.widget.TextView", name="android.widget.TextView", text="去支付"
             )
+            if unpaid_status.exists() is True:
+                status = "待支付"
+        except (PocoNoSuchNodeException, PocoTargetTimeout, Exception):
+            pass
+        try:
             cancel_status = self.device.poco(
                 type="android.widget.TextView", name="android.widget.TextView", text="已取消"
             )
-            if unpaid_status.exists() is True:
-                status = "待支付"
-            elif cancel_status.exists() is True:
+            if cancel_status.exists() is True:
                 status = "已取消"
-        except (PocoNoSuchNodeException, PocoTargetTimeout):
+        except (PocoNoSuchNodeException, PocoTargetTimeout, Exception):
+            pass
+        try:
+            out_ticketed_status = self.device.poco(
+                type="android.widget.TextView", name="android.widget.TextView", text="已出票"
+            )
+            if out_ticketed_status.exists() is True:
+                status = "已出票"
+        except (PocoNoSuchNodeException, PocoTargetTimeout, Exception):
             pass
-        except Exception as e:
-            logger.error(e)
         return status
 
     def is_order_detail_page(self) -> bool:
         """是否在订单详情界面"""
         flag = False
         try:
             order_detail_page_1 = self.device.poco(
                 type="android.widget.TextView", name="浮层标题", text="出行前必读"
             )
+            if order_detail_page_1.exists() is True:
+                flag = True
+        except (PocoNoSuchNodeException, PocoTargetTimeout, Exception):
+            pass
+        try:
             order_detail_page_2 = self.device.poco(
                 type="android.widget.TextView", name="header_Text_订单详情", text="订单详情"
             )
+            if order_detail_page_2.exists() is True:
+                flag = True
+        except (PocoNoSuchNodeException, PocoTargetTimeout, Exception):
+            pass
+        try:
             order_detail_page_3 = self.device.poco(
                 type="android.widget.TextView", name="operateBtnList_Text_我要退订", text="我要退订"
             )
+            if order_detail_page_3.exists() is True:
+                flag = True
+        except (PocoNoSuchNodeException, PocoTargetTimeout, Exception):
+            pass
+        try:
             order_detail_page_4 = self.device.poco(
                 type="android.view.ViewGroup", name="CusHeaderView_TouchableOpacity_leftIconWrap",
                 desc="CusHeaderView_TouchableOpacity_leftIconWrap"
             )
-            if (order_detail_page_1.exists() is True or order_detail_page_2.exists() is True or
-                    order_detail_page_3.exists() is True or order_detail_page_4.exists() is True):
+            if order_detail_page_4.exists() is True:
                 flag = True
-        except (PocoNoSuchNodeException, PocoTargetTimeout):
+        except (PocoNoSuchNodeException, PocoTargetTimeout, Exception):
             pass
-        except Exception as e:
-            logger.error(e)
         return flag
 
     @SleepWait(wait_time=1)
     def touch_go_back_to_unpaid_list_page_by_search_page(self) -> None:
         """从搜索界面退回到【待支付】列表页"""
         try:
             go_back = self.device.poco(type="android.widget.TextView", name="icon_back")
@@ -241,99 +253,108 @@
             if go_back.exists() is True:
                 go_back.click()
         except (PocoNoSuchNodeException, PocoTargetTimeout):
             pass
         except Exception as e:
             logger.error(e)
 
-    @SleepWait(wait_time=1)
-    def touch_to_payment_at_list_page(self) -> None:
+    @LoopFindElementSubmit(loop=1, action="去支付")
+    def touch_to_payment_at_list_page(self):
         """进入待付款列表页，点击【去支付】"""
         search_box = self.device.poco(type="android.widget.TextView", name="android.widget.TextView", text="去支付")
         search_box.click()
 
     @SleepWait(wait_time=1)
-    def is_cancel_order(self, out_total_price: str) -> tuple:
+    def is_cancel_order(self, out_total_price: str, amount_loss_limit: str, profit_cap: str, passenger_number: int,
+                        discount_amount: str = None) -> tuple:
         """在订单详情页，判断是否需要取消订单"""
         flag = False
         remark = None
         try:
             is_cancel = self.device.poco(
                 type="android.widget.TextView", name="android.widget.TextView", textMatches=r"^请在\d+:\d+前支付.*"
             )
             if is_cancel.exists() is True:
                 text = is_cancel.get_text()
                 time_match = re.search(r'(\d{2}:\d{2})', text)
                 amount_match = re.search(r'¥(\d+)', text)
                 if time_match and amount_match:
                     time_str = time_match.group(1)
                     string = "从订单获取到的过期时间为：{}".format(time_str)
-                    is_later = is_later_than_current_time(time_str=time_str, minutes=5)
+                    minutes = 1
+                    is_later = is_later_than_current_time(time_str=time_str, minutes=minutes)
                     if is_later is False:
                         flag = True
-                        remark = "支付时间少于5分钟"
+                        remark = "支付时间少于{}分钟".format(minutes)
                         string = string + "，" + remark
                     else:
                         amount_str = amount_match.group(1)
-                        string = "从订单获取到的支付金额为：{}，实际出票总订单价：{}".format(amount_str, out_total_price)
-                        if Decimal(amount_str) > Decimal(out_total_price):
-                            flag = True
-                            remark = "航班已变价"
-                            string = string + "，" + remark
+                        string = "从携程订单获取的支付金额：{}，劲旅订单总价：{}".format(amount_str, out_total_price)
+                        # 预期订单利润
+                        ex_order_profit = Decimal(out_total_price) - Decimal(amount_str)
+                        if discount_amount:
+                            # 实际订单利润
+                            ac_order_profit = ex_order_profit + Decimal(discount_amount)
+                        else:
+                            ac_order_profit = ex_order_profit
+                        # 订单利润 < 0, 存在亏钱，与亏钱的下限进行比较
+                        if ac_order_profit < 0:
+                            total = Decimal(amount_loss_limit) * passenger_number
+                            if ac_order_profit + total < 0:
+                                flag = True
+                                remark = "订单亏钱{:.2f}太多，超过订单总下限值{}(单人下限{} * {}人)".format(
+                                    abs(ac_order_profit), total, amount_loss_limit, passenger_number
+                                )
+                                logger.warning(remark)
+                        # 订单利润 >= 0, 存在毛利，与利润的上限进行比较
+                        else:
+                            total = Decimal(profit_cap) * passenger_number
+                            if ac_order_profit - total > 0:
+                                flag = True
+                                remark = "订单利润{:.2f}太高，超过订单总下限值{}(单人下限{} * {}人)".format(
+                                    ac_order_profit, total, profit_cap, passenger_number
+                                )
+                                logger.warning(remark)
+
                 else:
                     string = "从元素的文案<{}>提取时间与金额信息有异常".format(text)
             else:
                 string = "元素定位存在异常，订单详情页没有找到订单支付金额和过期时间"
-            print(string)
+            logger.warning(string)
         except (PocoNoSuchNodeException, PocoTargetTimeout):
             pass
         except Exception as e:
             logger.error(e)
         return flag, remark
 
-    @SleepWait(wait_time=1)
-    def touch_cancel_order(self) -> None:
-        try:
-            cancel_order = self.device.poco(
-                type="android.widget.TextView", name="operateBtnList_Text_取消订单", text="取消订单"
-            )
-            cancel_order.click()
-        except (PocoNoSuchNodeException, PocoTargetTimeout):
-            pass
-        except Exception as e:
-            logger.error(e)
+    @LoopFindElementSubmit(loop=1, action="取消订单")
+    def touch_cancel_order(self):
+        cancel_order = self.device.poco(
+            type="android.widget.TextView", name="operateBtnList_Text_取消订单", text="取消订单"
+        )
+        cancel_order.click()
 
-    @SleepWait(wait_time=1)
-    def touch_submit_cancel_order(self) -> None:
+    @LoopFindElementSubmit(loop=1, action="确认取消订单")
+    def touch_submit_cancel_order(self):
         """再次确认是否要取消订单"""
-        try:
-            submit_cancel_order = self.device.poco(
-                type="android.widget.TextView", name="Button_Text_取消订单", text="取消订单"
-            )
-            submit_cancel_order.click()
-        except (PocoNoSuchNodeException, PocoTargetTimeout):
-            pass
-        except Exception as e:
-            logger.error(e)
+        submit_cancel_order = self.device.poco(
+            type="android.widget.TextView", name="Button_Text_取消订单", text="取消订单"
+        )
+        submit_cancel_order.click()
 
-    @SleepWait(wait_time=1)
-    def touch_know_the_cancel_order(self) -> None:
+    @LoopFindElementSubmit(loop=1, action="知道了")
+    def touch_know_the_cancel_order(self):
         """确认取消后，会有一个【知道了】的小弹框"""
-        try:
-            submit_cancel_order = self.device.poco(
-                type="android.widget.TextView", name="Button_Text_知道了", text="知道了"
-            )
-            submit_cancel_order.click()
-        except (PocoNoSuchNodeException, PocoTargetTimeout):
-            pass
-        except Exception as e:
-            logger.error(e)
+        submit_cancel_order = self.device.poco(
+            type="android.widget.TextView", name="Button_Text_知道了", text="知道了"
+        )
+        submit_cancel_order.click()
 
-    @SleepWait(wait_time=2)
-    def touch_to_payment_at_order_detail(self) -> None:
+    @LoopFindElementSubmit(loop=1, action="详情-去支付")
+    def touch_to_payment_at_order_detail(self):
         """在订单详情页，点击【去支付】"""
         search_box = self.device.poco(type="android.widget.TextView", name="pcardLimit_Text_去支付", text="去支付")
         search_box.click()
 
     @SleepWait(wait_time=1)
     def touch_flight_ticket(self) -> None:
         """进入app后，点击【首页】，点击【机票】"""
@@ -726,71 +747,81 @@
             text="订",
             global_num=0,
             local_num=1,
             touchable=False,
         )[0]
         ordinary_booking_button.click()
 
-    def is_need_login(self) -> bool:
+    def is_need_login_with_my_page(self) -> bool:
         flag = False
         try:
-            login_page = self.device.get_po(
-                type="android.widget.TextView", name="ctrip.android.view:id/a", text="手机验证码登录"
-            )
             my_login = self.device.get_po(
                 type="android.widget.Button", name="ctrip.android.view:id/a", text="登录/注册"
             )
-            if login_page.exists() is True:
+            if my_login.exists() is True:
+                my_login.click()
                 logger.warning("手机app已经跳转至登录界面，需要做登录操作.")
                 flag = True
-            elif my_login.exists() is True:
-                my_login.click()
+        except (PocoNoSuchNodeException, PocoTargetTimeout):
+            pass
+        except Exception as e:
+            logger.error(e)
+        return flag
+
+    def is_need_login_with_login_page(self) -> bool:
+        flag = False
+        try:
+            login_page = self.device.get_po(
+                type="android.widget.TextView", name="ctrip.android.view:id/a", text="手机验证码登录"
+            )
+            if login_page.exists() is True:
                 logger.warning("手机app已经跳转至登录界面，需要做登录操作.")
                 flag = True
         except (PocoNoSuchNodeException, PocoTargetTimeout):
             pass
         except Exception as e:
             logger.error(e)
         return flag
 
-    def select_agree_service_agreement(self) -> None:
+    @LoopFindElementSubmit(loop=1, action="同意服务协议")
+    def select_agree_service_agreement(self):
         """选择【同意服务协议】"""
         service_agreement = self.device.get_po(
             type="android.widget.ImageView", name="ctrip.android.view:id/a", desc="勾选服务协议和个人信息保护指引"
         )
         service_agreement.click()
 
-    def touch_account_password_login(self) -> None:
+    @LoopFindElementSubmit(loop=1, action="账号密码登录")
+    def touch_account_password_login(self):
         """选择【账号密码登录】"""
         account_password_login = self.device.get_po(
             type="android.widget.TextView", name="ctrip.android.view:id/a", text="账号密码登录"
         )
         account_password_login.click()
 
-    def enter_account(self, username: str) -> None:
+    @LoopFindElementSubmit(loop=1, action="输入用户名")
+    def enter_account(self, username: str):
         """输入登录用户"""
         username_poco = self.device.get_po_extend(
             type="android.widget.EditText", name="android.widget.EditText", textMatches_inner=r"^\d+.*",
             global_num=0, local_num=2, touchable=True
         )[0]
-        # username_poco.click()
         username_poco.set_text(username)
 
-    def enter_password(self, password: str) -> None:
+    @LoopFindElementSubmit(loop=1, action="输入密码")
+    def enter_password(self, password: str):
         """输入登录密码"""
         password_poco = self.device.get_po(
             type="android.widget.EditText", name="android.widget.EditText", text="登录密码"
         )
-        # password_poco.click()
         password_poco.set_text(password)
-        # file_name = join_path([get_images_dir(), "键盘隐藏.png"])
-        # self.device.hide_keyword(file_name=file_name)
         self.device.quick_slide_screen(duration=0.5)
 
-    def touch_login(self) -> None:
+    @LoopFindElementSubmit(loop=1, action="登录")
+    def touch_login(self):
         """点击【登录】"""
         login_poco = self.device.get_po(type="android.widget.TextView", name="ctrip.android.view:id/a",
                                         text="登录")
         login_poco.click()
 
     @LoopFindElement(loop=5)
     # @SleepWait(wait_time=3)
@@ -1121,26 +1152,31 @@
             type="android.widget.TextView",
             name="android.widget.TextView",
             text=payment_method
         )
         method.click()
         logger.info("点击选择【{}】".format(payment_method))
 
-    @SleepWait(wait_time=1)
-    def select_more_payment(self) -> None:
+    @LoopClickElement(loop=5)
+    # @SleepWait(wait_time=1)
+    def select_more_payment(self) -> bool:
         """
         当【同意并支付】后，特殊情况下，会出现支付小弹框，这个时候需要先判断是否存在小框，如果存在，则切换到通用支付选择界面
         """
+        flag = False
         try:
             more_payment = self.device.get_po(type="android.widget.TextView", name="android.widget.TextView",
                                               text="更多付款方式")
-            more_payment.click()
-            logger.info("小弹框选择【更多付款方式】.")
+            if more_payment.exists() is True:
+                more_payment.click()
+                logger.warning("小弹框选择【更多付款方式】.")
+                flag = True
         except (PocoNoSuchNodeException, Exception):
             logger.info("没有出现支付小弹框，请在通用支付选择界面操作.")
+        return flag
 
     def __get_wallet_element(self) -> UIObjectProxy:
         return self.device.get_po(
             type="android.widget.TextView", name="android.widget.TextView", textMatches=r'^钱包.*'
         )
 
     @SleepWait(wait_time=1)
@@ -1159,15 +1195,15 @@
                 pattern = r'\d+\.\d+'
                 # 使用 re.findall() 函数查找字符串中匹配的浮点数
                 matches = re.findall(pattern, text)
                 # 如果找到了匹配的浮点数，则返回第一个匹配结果（应该只有一个）
                 if matches:
                     flag, amount = True, Decimal(matches[0])
                 else:
-                    logger.warning("钱包的可用文案<{}>有异常.".format(text))
+                    logger.warning("提取钱包余额<{}>有异常，钱包为不可用状态，将选择银行卡支付".format(text))
             else:
                 logger.info("账户钱包被隐藏了，不能操作钱包.")
         except (PocoNoSuchNodeException, Exception):
             logger.warning("安全收银台界面，没有出现钱包的选择入口.")
         return flag, amount
 
     @SleepWait(wait_time=1)
@@ -1180,14 +1216,34 @@
         """选择对应的礼品卡"""
         gift_card = self.device.get_po(
             type="android.widget.TextView", name="android.widget.TextView", text=payment_method
         )
         gift_card.click()
 
     @SleepWait(wait_time=1)
+    def get_gift_card_deduction_amount(self) -> str:
+        """获取礼品卡抵扣金额"""
+        value = ""
+        try:
+            gift_card = self.device.get_po(
+                type="android.widget.TextView", name="android.widget.TextView", textMatches=r"^使用.*"
+            )
+            text_value = gift_card.get_text()
+            pattern = r'¥(\d+(\.\d+)?)'
+            matches = re.findall(pattern, text_value)
+            if len(matches) > 0:
+                value = matches[0][0]
+                # logger.warning("当前礼品卡抵扣金额为：{}".format(value))
+            else:
+                logger.warning("获取到的礼品卡抵扣金额文案未：{}".format(text_value))
+        except (Exception,):
+            logger.error("获取礼品卡抵扣金额出现异常")
+        return value
+
+    @SleepWait(wait_time=1)
     def touch_wallet_immediate_payment(self) -> None:
         """选择对应的礼品卡，点击【使用钱包全额抵扣，立即支付】"""
         wallet_immediate_payment = self.device.get_po(
             type="android.widget.TextView", name="android.widget.TextView", text="使用钱包全额抵扣，立即支付"
         )
         wallet_immediate_payment.click()
 
@@ -1239,23 +1295,23 @@
         )[0]
         point_deduction.click()
 
     def get_ticket_actual_amount(self) -> Decimal:
         """
         确定使用积分抵扣后，票据的实际支付金额
         """
-        tickect_actual_amount = self.device.get_po_extend(
+        ticket_actual_amount = self.device.get_po_extend(
             type="android.widget.TextView",
             name="android.widget.TextView",
             textMatches_inner=r"^¥\d+.\d*",
             global_num=0,
             local_num=2,
             touchable=False,
         )[0]
-        actual_amount = tickect_actual_amount.get_text()
+        actual_amount = ticket_actual_amount.get_text()
         actual_amount = Decimal(actual_amount[1:]) if isinstance(
             actual_amount, str) else 9999999999.9999999999
         return actual_amount
 
     def get_ticket_deduction_amount(self) -> Decimal:
         """
         使用积分抵扣的金额
@@ -1269,29 +1325,42 @@
             touchable=False,
         )[0]
         deduction_amount = tickect_deduction_amount.get_text()
         deduction_amount = Decimal(deduction_amount[2:]) if isinstance(deduction_amount,
                                                                        str) else -9999999999.9999999999
         return deduction_amount
 
-    @SleepWait(wait_time=5)
-    def enter_payment_pass(self, payment_pass: str) -> None:
+    @SleepWait(wait_time=8)
+    def enter_payment_pass(self, payment_pass: str, device_id: str, enable_debug: bool = False, port: int = 0,
+                           platform: str = "Android") -> None:
         """
         请输入支付密码
         """
-        device = PlatformService.minicap_device()
+        device = PlatformService.minicap_device(
+            device_id=device_id, enable_debug=enable_debug, platform=platform, port=port
+        )
         payment_pass = payment_pass if isinstance(payment_pass, str) else str(payment_pass)
         for char in payment_pass:
             file_name = join_path([get_images_dir(), "支付_{}.png".format(char)])
             if is_exists(file_name):
                 temp = device.get_cv_template(file_name=file_name)
                 device.touch(v=temp)
             else:
                 raise ValueError("文件<{}>缺失...", format(file_name))
 
+    @SleepWait(wait_time=8)
+    def enter_payment_pass_by_position(self, payment_pass: str) -> None:
+        """
+        请输入支付密码
+        """
+        payment_pass = payment_pass if isinstance(payment_pass, str) else str(payment_pass)
+        for char in payment_pass:
+            char_position = ctrip_soft_keyboard_position.get(char)
+            self.device.touch(v=char_position)
+
     @SleepWait(wait_time=1)
     def is_balance(self, payment_card: str) -> bool:
         """
         判断是否出现余额不足的小弹框
         """
         flag = False
         try:
@@ -1311,27 +1380,24 @@
     @SleepWait(wait_time=1)
     def is_payment_complete(self) -> bool:
         """
         判断是否限额，余额不足或其他异常，没有异常的话，输入密码后，会出现【完成】小弹框界面
         """
         flag = False
         try:
-            limit_quotas = self.device.get_po_extend(
+            limit_quotas = self.device.poco(
                 type="android.widget.TextView",
                 name="android.widget.TextView",
-                text="完成",
-                global_num=0,
-                local_num=1,
-                touchable=False,
-            )[0]
+                text="完成"
+            )
             if limit_quotas.exists():
-                logger.warning("已经支付成功，等待出票.")
+                # logger.warning("银行卡支付成功，等待出票.")
                 flag = True
         except (PocoNoSuchNodeException, Exception):
-            logger.warning("支付有异常，需要更新支付类型，重新支付.")
+            logger.warning("银行卡支付有异常，需要更新支付类型，重新支付.")
         return flag
 
     @SleepWait(wait_time=1)
     def get_order_with_payment_amount(self) -> Decimal:
         """获取支付成功后的订单金额"""
         payment_amount = -9999999999.9999999999
         try:
@@ -1346,30 +1412,24 @@
             payment_amount = payment_amount.get_text()
             logger.info("从支付成功界面获取到的实际支付金额是: {}".format(payment_amount))
             payment_amount = Decimal(payment_amount) if isinstance(payment_amount, str) else payment_amount
         except Exception as e:
             logger.error(str(e))
         return payment_amount
 
-    @SleepWait(wait_time=3)
-    def touch_payment_complete(self) -> None:
+    @LoopFindElementSubmit(loop=3, action="支付完成")
+    def touch_payment_complete(self):
         """在支付成功界面，点击【完成】"""
-        try:
-            payment_complete_button = self.device.get_po_extend(
-                type="android.widget.TextView",
-                name="android.widget.TextView",
-                text="完成",
-                global_num=0,
-                local_num=1,
-                touchable=False,
-            )[0]
-            payment_complete_button.click()
-            logger.info("点击支付成功界面的【完成】按钮.")
-        except Exception as e:
-            logger.error("查询界面的完成按钮失败，原因：{}".format(str(e)))
+        payment_complete_button = self.device.poco(
+            type="android.widget.TextView",
+            name="android.widget.TextView",
+            text="完成"
+        )
+        payment_complete_button.click()
+        logger.warning("点击支付成功界面的【完成】按钮.")
 
     @SleepWait(wait_time=1)
     def close_coupon_dialog(self) -> None:
         """支付完成后，会有一个优惠卷弹框，需要关闭"""
         try:
             coupon_dialog = self.device.get_po(
                 type="android.view.ViewGroup", name="领券弹窗关闭按钮")
```

### Comparing `ctrip-app-ui-0.3.9/capp_ui/fee.py` & `ctrip-app-ui-0.4.0/capp_ui/fee.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.3.9/capp_ui/mobile_terminals.py` & `ctrip-app-ui-0.4.0/capp_ui/mobile_terminals.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,89 +12,109 @@
 import re
 import shlex
 import airtest
 import warnings
 import subprocess
 import typing as t
 from poco.proxy import UIObjectProxy
-from airtest.cli.parser import cli_setup
+# from airtest.cli.parser import cli_setup
 from airtest.utils.transform import TargetPos
 
 from poco.drivers.android.uiautomation import AndroidUiautomationPoco
 from airtest.core.api import auto_setup, device, Template, touch, find_all, connect_device
 
-from capp_ui.utils import logger
+from capp_ui.device import cli_setup
 from capp_ui.dir import get_project_path
-from capp_ui.libs import airtest_exception_format
+from capp_ui.libs import airtest_exception_format, logger
 
 iOS_PLATFORM = "iOS"
 DEFAULT_PLATFORM = "Android"  # Android、Windows、iOS
 WINDOWS_PLATFORM = "Windows"
 
 warnings.filterwarnings("ignore", category=UserWarning,
                         message="Currently using ADB touch, the efficiency may be very low.")
 
 
-def stop_app(app_name, timeout=5):
+def stop_app(app_name, device_id: str, timeout=5):
     # 构造ADB命令
-    adb_cmd = "adb.exe shell am force-stop {}".format(app_name)
+    adb_cmd = "adb.exe -s {} shell am force-stop {}".format(device_id, app_name)
     # 将命令字符串分割成列表
     cmd_list = shlex.split(adb_cmd)
     try:
         # 执行ADB命令并设置超时时间
         subprocess.run(cmd_list, timeout=timeout, check=True)
         logger.info("execute cmd: {}".format(adb_cmd))
     except subprocess.TimeoutExpired:
         logger.error("Timeout occurred. Failed to stop the app.")
     except subprocess.CalledProcessError:
         logger.error("Failed to stop the app.")
     except Exception as e:
         logger.error("An error occurred: {}".format(e))
 
 
-def get_screen_size_via_adb():
+def get_screen_size_via_adb(device_id: str):
     # 使用ADB命令获取设备屏幕大小
     try:
-        output = subprocess.check_output(['adb', 'shell', 'wm', 'size']).decode('utf-8')
+        output = subprocess.check_output(['adb', '-s', device_id, 'shell', 'wm', 'size']).decode('utf-8')
         match = re.search(r'Physical size: (\d+)x(\d+)', output)
         if match:
             width = int(match.group(1))
             height = int(match.group(2))
             return width, height
     except subprocess.CalledProcessError as e:
         logger.error("Error: ADB command failed: {}".format(e))
     return None
 
 
+def get_connected_devices():
+    devices = list()
+    try:
+        # 执行 adb 命令获取设备列表信息
+        result = subprocess.run(['adb', 'devices'], capture_output=True, text=True)
+        # 检查是否成功执行 adb 命令
+        if result.returncode == 0:
+            # 解析 adb 输出，获取设备列表信息
+            output_lines = result.stdout.strip().split('\n')
+            # 第一行是标题，需要跳过
+            devices = [line.split('\t')[0] for line in output_lines[1:] if line.strip()]
+        else:
+            logger.error("Failed to execute adb command.")
+    except Exception as e:
+        logger.error(f"An error occurred: {e}")
+    return devices
+
+
 class Phone(object):
 
     def __init__(
             self,
             device_id: str,
-            device_conn: str,
+            port: int = 0,
+            device_conn: str = None,
             platform: str = "Android",
-            enable_debug: bool = False,
+            enable_debug: bool = False
     ) -> None:
         self.platform = platform
         self.device_id = device_id
+        self.port = port
         self.device_conn = device_conn
         self.enable_debug = enable_debug
         self.__init_device()
         self.dev = device()
         self.poco = AndroidUiautomationPoco(
-            use_airtest_input=True, screenshot_each_action=False
+            use_airtest_input=True, screenshot_each_action=False, force_restart=True
         )
 
     def __init_device(self) -> None:
         if not cli_setup():
             project_root = get_project_path()
             airtest.utils.compat.DEFAULT_LOG_DIR = "logs"
             airtest.core.settings.Settings.DEBUG = self.enable_debug
             airtest.core.settings.Settings.LOG_FILE = "{}.log".format(self.device_id)
-            if self.device_conn.find(":5555") != -1:
+            if self.port > 0:
                 if self.platform == DEFAULT_PLATFORM:
                     connect_device(self.device_conn)
                 else:
                     raise ValueError("暂时还不支持非android平台的手机初始化...")
             else:
                 auto_setup(
                     project_root,
@@ -522,26 +542,25 @@
                 if lg_keyword.exists():
                     logger.info("目前检测到LG键盘已经打开，需要隐藏键盘，再做后续操作...")
                     lg_keyword.click()
                 else:
                     logger.info("键盘已经隐藏，无需处理键盘...")
 
     # 获取元素在屏幕上的绝对坐标
-    @staticmethod
-    def get_abs_position(element: AndroidUiautomationPoco) -> t.Tuple:
-        screen_width, screen_height = get_screen_size_via_adb()
+    def get_abs_position(self, element: AndroidUiautomationPoco) -> t.Tuple:
+        screen_width, screen_height = get_screen_size_via_adb(device_id=self.device_id)
         relative_position = element.get_position()
         absolute_x = int(relative_position[0] * screen_width)
         absolute_y = int(relative_position[1] * screen_height)
         return absolute_x, absolute_y
 
     # 快捷滑屏
     def quick_slide_screen(self, duration: float = 0.5):
         # 获取屏幕尺寸
-        screen_width, screen_height = get_screen_size_via_adb()
+        screen_width, screen_height = get_screen_size_via_adb(device_id=self.device_id)
         # 定义起始点和终止点坐标
         start_x = screen_width // 2  # 屏幕中心点的横坐标
         start_y = screen_height // 2  # 屏幕中心点的纵坐标
         end_x = start_x  # 横坐标保持不变
         end_y = screen_height // 4  # 终止点纵坐标为屏幕顶部 1/4 处
         # 执行滑动操作
         self.swipe((start_x, start_y), (end_x, end_y), duration=duration)
```

### Comparing `ctrip-app-ui-0.3.9/capp_ui/platforms.py` & `ctrip-app-ui-0.4.0/capp_ui/platforms.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,37 +5,39 @@
 # FileName:     platforms.py
 # Description:  TODO
 # Author:       mfkifhss2023
 # CreateDate:   2024/04/24
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
-from capp_ui.device import default_andriod_device, default_minicap_device
+from capp_ui.device import get_minicap_url, get_default_url
 from capp_ui.mobile_terminals import Phone, DEFAULT_PLATFORM, WINDOWS_PLATFORM
 
 
 class PlatformService(object):
 
-    def __init__(self, device_config: dict = None) -> None:
+    def __init__(self, device_id: str, port: int, enable_debug: bool = False, platform: str = "Android") -> None:
         # 暂时支持Android和Windows平台
-        self.device_config = device_config or default_andriod_device
-        if self.device_config.get("platform") == DEFAULT_PLATFORM:
+        self.default_device = get_default_url(device_id=device_id)
+        if platform == DEFAULT_PLATFORM:
             self.device = Phone(
-                device_id=self.device_config.get("device_id"),
-                device_conn=self.device_config.get("device_conn"),
-                platform=self.device_config.get("platform"),
-                enable_debug=self.device_config.get("enable_debug")
+                device_id=device_id,
+                port=port,
+                device_conn=self.default_device,
+                platform=platform,
+                enable_debug=enable_debug
             )
-        elif self.device_config.get("platform") == WINDOWS_PLATFORM:
+        elif platform == WINDOWS_PLATFORM:
             pass
         else:
             raise ValueError("The platform configuration only supports Andriod and Windows.")
 
     @classmethod
-    def minicap_device(cls, device_config: dict = None) -> Phone:
-        config = device_config or default_minicap_device
+    def minicap_device(cls, device_id: str, enable_debug: bool, platform: str, port: int) -> Phone:
+        min_device = get_minicap_url(device_id=device_id)
         return Phone(
-            device_id=config.get("device_id"),
-            device_conn=config.get("device_conn"),
-            platform=config.get("platform"),
-            enable_debug=config.get("enable_debug"),
+            port=port,
+            device_id=device_id,
+            device_conn=min_device,
+            platform=platform,
+            enable_debug=enable_debug,
         )
```

### Comparing `ctrip-app-ui-0.3.9/capp_ui/test.py` & `ctrip-app-ui-0.4.0/capp_ui/test.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
 from domain_service import CtripAppService
 
 
 def test_service():
-    app = CtripAppService()
+    app = CtripAppService(device_id="66J5T19627007749", enable_debug=False, platform="Android", port=0)
     app.device.wake()
     app.restart()
     app.hide_navigation_bar()
 
 
 if __name__ == '__main__':
     test_service()
```

### Comparing `ctrip-app-ui-0.3.9/capp_ui/utils.py` & `ctrip-app-ui-0.4.0/capp_ui/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,22 +5,17 @@
 # FileName:     utils.py
 # Description:  TODO
 # Author:       mfkifhss2023
 # CreateDate:   2024/04/24
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
-import os
-import sys
-import logging
 from collections import OrderedDict
 from poco.drivers.android.uiautomation import AndroidUiautomationPoco
 
-logger = logging.getLogger("root")
-
 
 def get_ui_object_proxy_attr(ui_object_proxy: AndroidUiautomationPoco) -> OrderedDict:
     ordered_dict = OrderedDict()
     ordered_dict["type"] = (
         ui_object_proxy.attr("type").strip()
         if isinstance(ui_object_proxy.attr("type"), str)
         else ui_object_proxy.attr("type")
```

### Comparing `ctrip-app-ui-0.3.9/capp_ui/validators.py` & `ctrip-app-ui-0.4.0/capp_ui/validators.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 # FileName:     validators.py
 # Description:  TODO
 # Author:       mfkifhss2023
 # CreateDate:   2024/04/24
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
-from utils import logger
 from decimal import Decimal
+from capp_ui.libs import logger
 from capp_ui.fee import flight_fee
 
 __all__ = ["FlightTicketValidator"]
 
 
 class FlightTicketValidator(object):
     """机票校验器"""
```

### Comparing `ctrip-app-ui-0.3.9/setup.py` & `ctrip-app-ui-0.4.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
 from setuptools import setup, find_packages
 
 setup(
     name='ctrip-app-ui',
-    version='0.3.9',
+    version='0.4.0'
+            '',
     description='This is my ctrip app ui package',
     long_description='This is my ctrip app ui package',
     author='ckf10000',
     author_email='ckf10000@sina.com',
     url='https://github.com/ckf10000/ctrip-app-ui',
     packages=find_packages(),
     install_requires=[
```

