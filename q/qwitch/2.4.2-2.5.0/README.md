# Comparing `tmp/qwitch-2.4.2.tar.gz` & `tmp/qwitch-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qwitch-2.4.2.tar", last modified: Sat Dec  9 13:11:13 2023, max compression
+gzip compressed data, was "qwitch-2.5.0.tar", last modified: Sun May 12 09:54:03 2024, max compression
```

## Comparing `qwitch-2.4.2.tar` & `qwitch-2.5.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 13:11:13.323182 qwitch-2.4.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2023-12-09 13:11:02.000000 qwitch-2.4.2/LICENCE
--rw-r--r--   0 runner    (1001) docker     (127)     8599 2023-12-09 13:11:13.323182 qwitch-2.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7492 2023-12-09 13:11:02.000000 qwitch-2.4.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2023-12-09 13:11:02.000000 qwitch-2.4.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 13:11:13.323182 qwitch-2.4.2/qwitch/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-09 13:11:02.000000 qwitch-2.4.2/qwitch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8060 2023-12-09 13:11:02.000000 qwitch-2.4.2/qwitch/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     8682 2023-12-09 13:11:02.000000 qwitch-2.4.2/qwitch/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5180 2023-12-09 13:11:02.000000 qwitch-2.4.2/qwitch/qwitch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 13:11:13.323182 qwitch-2.4.2/qwitch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8599 2023-12-09 13:11:13.000000 qwitch-2.4.2/qwitch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      281 2023-12-09 13:11:13.000000 qwitch-2.4.2/qwitch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-09 13:11:13.000000 qwitch-2.4.2/qwitch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2023-12-09 13:11:13.000000 qwitch-2.4.2/qwitch.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2023-12-09 13:11:13.000000 qwitch-2.4.2/qwitch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-12-09 13:11:13.000000 qwitch-2.4.2/qwitch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-09 13:11:13.323182 qwitch-2.4.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 09:54:03.721416 qwitch-2.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-12 09:53:59.000000 qwitch-2.5.0/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (127)     8599 2024-05-12 09:54:03.721416 qwitch-2.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7492 2024-05-12 09:53:59.000000 qwitch-2.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-05-12 09:53:59.000000 qwitch-2.5.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 09:54:03.717416 qwitch-2.5.0/qwitch/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 09:53:59.000000 qwitch-2.5.0/qwitch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10354 2024-05-12 09:53:59.000000 qwitch-2.5.0/qwitch/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8682 2024-05-12 09:53:59.000000 qwitch-2.5.0/qwitch/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5128 2024-05-12 09:53:59.000000 qwitch-2.5.0/qwitch/qwitch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 09:54:03.717416 qwitch-2.5.0/qwitch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8599 2024-05-12 09:54:03.000000 qwitch-2.5.0/qwitch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-12 09:54:03.000000 qwitch-2.5.0/qwitch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 09:54:03.000000 qwitch-2.5.0/qwitch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-12 09:54:03.000000 qwitch-2.5.0/qwitch.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-12 09:54:03.000000 qwitch-2.5.0/qwitch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-12 09:54:03.000000 qwitch-2.5.0/qwitch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 09:54:03.721416 qwitch-2.5.0/setup.cfg
```

### Comparing `qwitch-2.4.2/LICENCE` & `qwitch-2.5.0/LICENCE`

 * *Files identical despite different names*

### Comparing `qwitch-2.4.2/PKG-INFO` & `qwitch-2.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qwitch
-Version: 2.4.2
+Version: 2.5.0
 Summary: Stream twitch in Quicktime.
 Author-email: Jean-Francois Vaduret <jean.francois.vaduret@gmail.com>
 Project-URL: Source, https://github.com/gencys/qwitch
 Project-URL: Tracker, https://github.com/gencys/qwitch/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Environment :: Console
```

### Comparing `qwitch-2.4.2/README.md` & `qwitch-2.5.0/README.md`

 * *Files identical despite different names*

### Comparing `qwitch-2.4.2/pyproject.toml` & `qwitch-2.5.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools>=64.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "qwitch"
-version = "2.4.2"
+dynamic = ["version"]
 description = "Stream twitch in Quicktime."
 readme = "README.md"
 authors = [{ name = "Jean-Francois Vaduret", email = "jean.francois.vaduret@gmail.com" }]
 license = {file = "LICENSE"}
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "License :: OSI Approved :: MIT License",
@@ -34,9 +34,12 @@
 ]
 requires-python = ">=3.8"
 
 [project.urls]
 Source = "https://github.com/gencys/qwitch"
 Tracker = "https://github.com/gencys/qwitch/issues"
 
+[tool.setuptools.dynamic]
+version = {attr = "qwitch.config.VER"}
+
 [project.scripts]
 qwitch = "qwitch.qwitch:main"
```

### Comparing `qwitch-2.4.2/qwitch/config.py` & `qwitch-2.5.0/qwitch/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import time
 import json
 import webbrowser
 import time
 import requests
 
 DEBUG = False
-VER = '2.4.2'
+VER = '2.5.0'
 
 home_dir = os.path.expanduser('~')
 home_dir += '/Library/Application Support'
 if not os.path.exists(home_dir + '/qwitch/config.json'):
     os.makedirs(os.path.dirname(home_dir + '/qwitch/config.json'), exist_ok=True)
 
 ##
```

### Comparing `qwitch-2.4.2/qwitch/qwitch.py` & `qwitch-2.5.0/qwitch/qwitch.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import argparse
 import re
 from . import config
-from . import api
+from .api import TwitchAPI, exec_streamlink
 
 def main():
     try:
         cli = argparse.ArgumentParser(
             prog = 'qwitch',
             description = 'Stream twitch in Quicktime'
         )
@@ -13,15 +13,15 @@
 
         cli.add_argument('channel', nargs='?', default = False, help= 'channel name given in red with -s/--streams. Needed to launch livestream or videos.')
         cli.add_argument('quality', nargs='?', default = False, help= 'video quality name, e.g. 720p, 1080p, best, worst, etc... (defaults to best). You can defined a default quality in the config file (see the README)')
         cli.add_argument('-d', '--debug', action = 'store_true', help= 'enable debugging.')
         cli.add_argument('--version', action='version', version = f'%(prog)s {config.VER}')
 
         group.add_argument('-l', '--last', action = 'store_true', help= 'play the most recent video of the channel.')
-        group.add_argument('-V', '--Videos', action = 'store_true', help= 'list the last 20 videos of the channel.')
+        group.add_argument('-V', '--Videos', action = 'store_true', help= 'list the last 100 videos of the channel.')
         group.add_argument('-s', '--streams', action = 'store_true', help= 'list the streamers you follow which are currently currently live.')
         group.add_argument('-f', '--follows', action = 'store_true', help= 'list the streamers you follow.')
         group.add_argument('-v', '--vod', action = 'store', type = str, help= 'search for a video by keyword(s) or ID. The keyword needs to be in quotation marks and an exact match (this is not a search engine)')
         group.add_argument('-t', '--token', action = 'store_true', help= 'change the auth-token of you twitch account in the qwitch config file.')
         args = cli.parse_args()
 
         try:
@@ -34,68 +34,70 @@
             if (config.get_package_ver_and_compare()):
                 exit()
             cli.error('Could not authenticate in the Twitch API.')
         
         if (config.get_package_ver_and_compare()):
             exit()
 
+        api = TwitchAPI(token = auth_token)
+
         if args.debug:
             config.DEBUG = True
 
         if args.token:
             config.write_streamlink_config()
         elif args.follows:
             try:
-                api.get_follows(token = auth_token)
+                api.get_follows()
             except:
                 cli.error('Could not get the list of followed streamers.')
         elif args.channel:
-            try:
-                channel_id = api.get_channel_id(channel = args.channel, token = auth_token)
-            except RuntimeError:
-                cli.error('Could not get user id for the channel name provided.\nCheck that the channel name you provided is correct.')
-            except:
-                cli.error('Something unknown went wrong.')
+            # try:
+            channel_id = api.get_channel_id(channel = args.channel)
+            # except RuntimeError:
+            #     cli.error('Could not get user id for the channel name provided.\nCheck that the channel name you provided is correct.')
+            # except:
+            #     cli.error('Something unknown went wrong.')
 
             if args.last:
-                url = api.get_vod(channel_id=channel_id, token=auth_token)
+                url = api.get_vod(channel_id=channel_id)
                 url = url.replace('https://www.', '')
                 config.debug_log('Playing the video now...')
-                api.exec_streamlink(url = url, streamlink_config = streamlink_config, quality = args.quality)
+                exec_streamlink(url = url, streamlink_config = streamlink_config, quality = args.quality)
             elif args.Videos:
                 try:
-                    url = api.print_vod_list(channel_id=channel_id, token=auth_token)
+                    url = api.print_vod_list(channel_id=channel_id)
                     if url:
-                        api.exec_streamlink(url = url, streamlink_config = streamlink_config, quality = args.quality)
+                        exec_streamlink(url = url, streamlink_config = streamlink_config, quality = args.quality)
                 except KeyboardInterrupt:
                     exit()
                 # except:
                 #     cli.error('Could not retrieve the video list')
             elif args.vod:
                 try:
-                    url = api.get_vod(channel_id=channel_id, token=auth_token, keyword=args.vod)
+                    url = api.get_vod(channel_id=channel_id, keyword=args.vod)
                     url = url.replace('https://www.', '')
                     config.debug_log('Playing the video now...')
-                    api.exec_streamlink(url = url, streamlink_config = streamlink_config, quality = args.quality)
+                    exec_streamlink(url = url, streamlink_config = streamlink_config, quality = args.quality)
                 except:
                     cli.error('Could not find a video that matched the keyword.')
             else:
                 try:
                     url = 'twitch.tv/' + args.channel
                     config.debug_log('Playing the livestream now...')
-                    api.exec_streamlink(url = url, streamlink_config = streamlink_config, quality = args.quality)
+                    exec_streamlink(url = url, streamlink_config = streamlink_config, quality = args.quality)
                 except:
                     cli.error('Could not get the livestream feed.')
         elif args.vod:
             if re.match('^[0-9]{9,10}$', args.vod):
                 url = 'twitch.tv/videos/' + args.vod
-                api.exec_streamlink(url = url, streamlink_config = streamlink_config, quality = args.quality)
+                exec_streamlink(url = url, streamlink_config = streamlink_config, quality = args.quality)
         elif args.streams:
             try:
-                api.get_livestreams(token = auth_token)
+                api.get_livestreams()
             except:
                 cli.error('Could not get the livestream list.')
     except KeyboardInterrupt:
         exit()
 
 if __name__ == "__main__":
     main()
```

### Comparing `qwitch-2.4.2/qwitch.egg-info/PKG-INFO` & `qwitch-2.5.0/qwitch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qwitch
-Version: 2.4.2
+Version: 2.5.0
 Summary: Stream twitch in Quicktime.
 Author-email: Jean-Francois Vaduret <jean.francois.vaduret@gmail.com>
 Project-URL: Source, https://github.com/gencys/qwitch
 Project-URL: Tracker, https://github.com/gencys/qwitch/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Environment :: Console
```

