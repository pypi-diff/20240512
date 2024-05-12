# Comparing `tmp/wlkata_mirobot_Virtual-1.0.1.tar.gz` & `tmp/wlkata_mirobot_Virtual-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wlkata_mirobot_Virtual-1.0.1.tar", last modified: Sun May 12 02:47:19 2024, max compression
+gzip compressed data, was "wlkata_mirobot_Virtual-1.1.0.tar", last modified: Sun May 12 07:16:54 2024, max compression
```

## Comparing `wlkata_mirobot_Virtual-1.0.1.tar` & `wlkata_mirobot_Virtual-1.1.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-12 02:47:19.496020 wlkata_mirobot_Virtual-1.0.1/
--rw-rw-rw-   0        0        0      110 2024-05-12 02:47:19.495023 wlkata_mirobot_Virtual-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      592 2024-05-11 10:00:37.000000 wlkata_mirobot_Virtual-1.0.1/license.txt
--rw-rw-rw-   0        0        0       42 2024-05-12 02:47:19.496020 wlkata_mirobot_Virtual-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      236 2024-05-12 02:46:51.000000 wlkata_mirobot_Virtual-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-12 02:47:19.490037 wlkata_mirobot_Virtual-1.0.1/wlkata_mirobot_Virtual/
--rw-rw-rw-   0        0        0       83 2024-05-12 02:38:37.000000 wlkata_mirobot_Virtual-1.0.1/wlkata_mirobot_Virtual/__init__.py
--rw-rw-rw-   0        0        0    15551 2024-05-11 09:50:49.000000 wlkata_mirobot_Virtual-1.0.1/wlkata_mirobot_Virtual/wlkata_mirobot_Virtual.py
-drwxrwxrwx   0        0        0        0 2024-05-12 02:47:19.494025 wlkata_mirobot_Virtual-1.0.1/wlkata_mirobot_Virtual.egg-info/
--rw-rw-rw-   0        0        0      110 2024-05-12 02:47:19.000000 wlkata_mirobot_Virtual-1.0.1/wlkata_mirobot_Virtual.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      288 2024-05-12 02:47:19.000000 wlkata_mirobot_Virtual-1.0.1/wlkata_mirobot_Virtual.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-12 02:47:19.000000 wlkata_mirobot_Virtual-1.0.1/wlkata_mirobot_Virtual.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2024-05-12 02:47:19.000000 wlkata_mirobot_Virtual-1.0.1/wlkata_mirobot_Virtual.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-12 07:16:54.628884 wlkata_mirobot_Virtual-1.1.0/
+-rw-rw-rw-   0        0        0      110 2024-05-12 07:16:54.627886 wlkata_mirobot_Virtual-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      592 2024-05-11 10:00:37.000000 wlkata_mirobot_Virtual-1.1.0/license.txt
+-rw-rw-rw-   0        0        0       42 2024-05-12 07:16:54.628884 wlkata_mirobot_Virtual-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      236 2024-05-12 07:16:24.000000 wlkata_mirobot_Virtual-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-12 07:16:54.622900 wlkata_mirobot_Virtual-1.1.0/wlkata_mirobot_Virtual/
+-rw-rw-rw-   0        0        0       83 2024-05-12 02:38:37.000000 wlkata_mirobot_Virtual-1.1.0/wlkata_mirobot_Virtual/__init__.py
+-rw-rw-rw-   0        0        0    15587 2024-05-12 05:43:43.000000 wlkata_mirobot_Virtual-1.1.0/wlkata_mirobot_Virtual/wlkata_mirobot_Virtual.py
+drwxrwxrwx   0        0        0        0 2024-05-12 07:16:54.626889 wlkata_mirobot_Virtual-1.1.0/wlkata_mirobot_Virtual.egg-info/
+-rw-rw-rw-   0        0        0      110 2024-05-12 07:16:54.000000 wlkata_mirobot_Virtual-1.1.0/wlkata_mirobot_Virtual.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      288 2024-05-12 07:16:54.000000 wlkata_mirobot_Virtual-1.1.0/wlkata_mirobot_Virtual.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-12 07:16:54.000000 wlkata_mirobot_Virtual-1.1.0/wlkata_mirobot_Virtual.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2024-05-12 07:16:54.000000 wlkata_mirobot_Virtual-1.1.0/wlkata_mirobot_Virtual.egg-info/top_level.txt
```

### Comparing `wlkata_mirobot_Virtual-1.0.1/license.txt` & `wlkata_mirobot_Virtual-1.1.0/license.txt`

 * *Files identical despite different names*

### Comparing `wlkata_mirobot_Virtual-1.0.1/wlkata_mirobot_Virtual/wlkata_mirobot_Virtual.py` & `wlkata_mirobot_Virtual-1.1.0/wlkata_mirobot_Virtual/wlkata_mirobot_Virtual.py`

 * *Files 1% similar despite different names*

```diff
@@ -411,17 +411,17 @@
         msg = self.generate_args_string(instruction, pairings)
         if is_com2:
             self.send_msg(com2_data=msg, wait_idle=True)
         else:
             self.send_msg(com1_data=msg, wait_idle=True)
         return True
     
-    def linear_interpolation(self,P1,speed=None, is_relative=False, wait_ok=None):
+    def linear_interpolation(self,P1,speed=None, is_relative=False, is_com2 = False, wait_ok=None):
         self.linear_interpolation_o( x=P1[6], y=P1[7], z=P1[8], a=P1[9], b=P1[10], c=P1[11],
-                            speed=speed,is_relative=is_relative,wait_ok=wait_ok)
+                            speed=speed,is_relative=is_relative,is_com2 = is_com2, wait_ok=wait_ok)
     
     def linear_interpolation_o(self, x=None, y=None, z=None, a=None, b=None, c=None, speed=None, is_relative=False, is_com2 = False, wait_ok=None):
         '''直线插补'''
         instruction = 'M20 G90 G1'  # X{x} Y{y} Z{z} A{a} B{b} C{c} F{speed}
         if is_relative:
             instruction = 'M20 G91 G1'
         if not speed:
```

