# Comparing `tmp/spotibar-0.3.9.tar.gz` & `tmp/spotibar-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotibar-0.3.9.tar", last modified: Mon Mar 20 21:30:37 2023, max compression
+gzip compressed data, was "spotibar-0.4.0.tar", last modified: Sun May 12 13:09:31 2024, max compression
```

## Comparing `spotibar-0.3.9.tar` & `spotibar-0.4.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 21:30:37.101115 spotibar-0.3.9/
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-03-20 21:30:37.101115 spotibar-0.3.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3944 2023-03-20 21:30:14.000000 spotibar-0.3.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-20 21:30:37.101115 spotibar-0.3.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-03-20 21:30:14.000000 spotibar-0.3.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 21:30:37.097115 spotibar-0.3.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 21:30:37.097115 spotibar-0.3.9/src/spotibar/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-20 21:30:14.000000 spotibar-0.3.9/src/spotibar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15910 2023-03-20 21:30:14.000000 spotibar-0.3.9/src/spotibar/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-03-20 21:30:14.000000 spotibar-0.3.9/src/spotibar/config_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-03-20 21:30:14.000000 spotibar-0.3.9/src/spotibar/popups.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 21:30:37.101115 spotibar-0.3.9/src/spotibar.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-03-20 21:30:37.000000 spotibar-0.3.9/src/spotibar.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-03-20 21:30:37.000000 spotibar-0.3.9/src/spotibar.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-20 21:30:37.000000 spotibar-0.3.9/src/spotibar.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-03-20 21:30:37.000000 spotibar-0.3.9/src/spotibar.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-20 21:30:37.000000 spotibar-0.3.9/src/spotibar.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-20 21:30:37.000000 spotibar-0.3.9/src/spotibar.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 13:09:31.463627 spotibar-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-12 13:09:31.463627 spotibar-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5184 2024-05-12 13:09:18.000000 spotibar-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 13:09:31.463627 spotibar-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-12 13:09:18.000000 spotibar-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 13:09:31.459627 spotibar-0.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 13:09:31.459627 spotibar-0.4.0/src/spotibar/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 13:09:18.000000 spotibar-0.4.0/src/spotibar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14962 2024-05-12 13:09:18.000000 spotibar-0.4.0/src/spotibar/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-05-12 13:09:18.000000 spotibar-0.4.0/src/spotibar/config_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-05-12 13:09:18.000000 spotibar-0.4.0/src/spotibar/popups.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 13:09:31.459627 spotibar-0.4.0/src/spotibar.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-12 13:09:31.000000 spotibar-0.4.0/src/spotibar.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-12 13:09:31.000000 spotibar-0.4.0/src/spotibar.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 13:09:31.000000 spotibar-0.4.0/src/spotibar.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-12 13:09:31.000000 spotibar-0.4.0/src/spotibar.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-12 13:09:31.000000 spotibar-0.4.0/src/spotibar.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-12 13:09:31.000000 spotibar-0.4.0/src/spotibar.egg-info/top_level.txt
```

### Comparing `spotibar-0.3.9/src/spotibar/client.py` & `spotibar-0.4.0/src/spotibar/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,51 +1,42 @@
 import argparse
 import json
 import os
 import pylast
 import spotipy
 import subprocess
+import sys
 
 from .config_helper import SpotibarConfig
 from datetime import datetime
 from getpass import getpass
 from .popups import ConfigPopup
 
 
 class SpotibarClient:
     def __init__(self, *args, **kwargs):
-        """
-        :kwarg config_file: String path relative to ~/ of a config file to load.
-        """
+        """ """
         self.scope = "playlist-read-private playlist-modify-private user-read-playback-state user-modify-playback-state playlist-modify-public"
 
-        self.config_file = kwargs.get("config_file")
-
-        if not self.config_file:
-            raise Exception("A config_file must be passed.")
+        os.makedirs("~/.config/spotibar/", exist_ok=True)
 
+        self.config_file = "~/.config/spotibar/default.json"
         self.config = SpotibarConfig(config_file=self.config_file)
 
         self.client_id = self.config.get("client_id", kwargs.get("client_id", None))
         self.client_secret = self.config.get(
             "client_secret", kwargs.get("client_secret", None)
         )
         self.currently_playing_trunclen = int(
             self.config.get("currently_playing_trunclen", 45)
         )
 
         self.redirect_uri = "http://127.0.0.1"
 
-        self.auth_cache = self.config.get(
-            "auth_cache_path", kwargs.get(
-                "auth_cache_path", "~/.spotibar_cache/auth_cache"
-            )
-        )
-
-        os.makedirs(os.path.dirname(self.auth_cache), exist_ok=True)
+        self.auth_cache = "~/.cache/spotibar/auth_cache"
 
         self.client = None
         self.lastfm_client = None
 
         if kwargs.get("require_clients", True):
             self.client = self.get_client()
             self.lastfm_client = self.get_lastfm_client()
@@ -59,15 +50,15 @@
         """
         return spotipy.Spotify(
             auth_manager=spotipy.oauth2.SpotifyOAuth(
                 scope=self.scope,
                 client_id=self.client_id,
                 client_secret=self.client_secret,
                 redirect_uri=self.redirect_uri,
-                cache_path=self.auth_cache,
+                cache_path=os.path.expanduser(self.auth_cache),
                 open_browser=False,
             )
         )
 
     def get_lastfm_client(self):
         if self.config.get("should_heart_on_lastfm", False):
             try:
@@ -273,47 +264,44 @@
 
     def get_simple_timestamp(self):
         """
         Return a simple int timestamp.
         """
         return int(datetime.now().timestamp())
 
-    def is_playing_locally(self):
+    def is_playing(self):
         """
         Returns True if dbus thinks we are currently playing Spotify locally, False otherwise.
         """
         cmd = "dbus-send --print-reply --dest=org.mpris.MediaPlayer2.spotify /org/mpris/MediaPlayer2 org.freedesktop.DBus.Properties.Get string:'org.mpris.MediaPlayer2.Player' string:'PlaybackStatus'|egrep -A 1 \"string\"|cut -b 26-|cut -d '\"' -f 1|egrep -v ^$"
         try:
             if subprocess.check_output(cmd, shell=True, text=True).strip() == "Playing":
                 self.config.set("last_playing_timestamp", self.get_simple_timestamp())
                 return True
 
             return False
         except Exception as e:
-            # This is an expected case if X11 isn't running. Just return False.
-            return False
+            # This is an expected case if X11 isn't running. Do the expensive
+            # check of polling the API:
+            return self.is_currently_playing()
 
     def was_playing_recently(self, seconds=20):
         """
         Returns True if Spotibar found that Spotify was playing within the last seconds.
         """
         last_timestamp = self.config.get("last_playing_timestamp", 0)
         current_timestamp = self.get_simple_timestamp()
 
         return (current_timestamp - last_timestamp) < seconds
 
     def is_live(self):
         """
         Returns True if Spotify is currently playing, False otherwise.
         """
-        return (
-            self.is_playing_locally()
-            or self.was_playing_recently()
-            or self.is_currently_playing()
-        )
+        return self.is_playing() or self.was_playing_recently()
 
     def get_current_album_image_url(self):
         """
         Return a string of the URL of the album cover.
         """
         if self.is_live():
             currently_playing = self.client.currently_playing()
@@ -330,21 +318,21 @@
     print("\tWelcome to Spotibar!")
     print(
         "This script will set up the initial config file and enable/disable/configure features based on your preferences."
     )
 
     config = {}
 
-    response = input("Do you want to add tracks to a monthly playlist? [Y/n]")
+    response = input("Do you want to add tracks to a monthly playlist? [Y/n] ")
     if response == "" or response.lower() == "y":
         config["should_put_to_monthly_playlist"] = True
     else:
         config["should_put_to_monthly_playlist"] = False
 
-    response = input("Do you want to set up LastFM track hearting? [Y/n]")
+    response = input("Do you want to set up LastFM track hearting? [Y/n] ")
     if response == "" or response.lower() == "y":
         print("Setting up LastFM track hearting...")
         print(
             "\tPlease go to https://www.last.fm/api/account/create to get your credentials:"
         )
 
         config["should_heart_on_lastfm"] = True
@@ -374,34 +362,24 @@
         "Please go to https://developer.spotify.com/dashboard/applications to set up an application to get the following API keys. See the README for more details."
     )
     response = input("\tSpotify client ID: ")
     config["client_id"] = response
     response = input("\tSpotify client secret: ")
     config["client_secret"] = response
 
-    print("Where should we write this config?")
-    response = input("\tFilepath: [~/.spotibar_config.json]")
-
-    config_filepath = "~/.spotibar_config.json" if response == "" else response
-
-    print("Where should we cache your authentication tokens?")
-    response = input("\tFilepath: [~/.spotibar_auth_cache]")
-
-    auth_filepath = "~/.spotibar_auth_cache" if response == "" else response
-
     spotibar_client = SpotibarClient(
         client_id=config["client_id"],
         client_secret=config["client_secret"],
-        config_file=config_filepath,
-        auth_cache_path=auth_filepath,
     )
     spotibar_client.auth()
 
     try:
-        with open(config_filepath, "w") as fh:
+        os.makedirs(os.path.expanduser("~/.config/spotibar/"), exist_ok=True)
+        os.makedirs(os.path.expanduser("~/.cache/spotibar/"), exist_ok=True)
+        with open(os.path.expanduser("~/.config/spotibar/default.json"), "x") as fh:
             json.dump(config, fh)
 
     except Exception as e:
         print(f"Problem writing config file:")
         print(e)
 
         print("Here's your config to manually add:")
@@ -411,20 +389,14 @@
 
 
 def main():
     parser = argparse.ArgumentParser(
         description="Entrypoint for Spotify/Polybar integration."
     )
 
-    parser.add_argument("--config-filepath", default="~/.spotibar_config.json")
-    parser.add_argument(
-        "--auth-filepath",
-        default="~/.spotibar_cache/auth_cache"
-    )
-
     group = parser.add_mutually_exclusive_group()
     group.add_argument("--get-currently-playing", action="store_true")
     group.add_argument("--previous-track", action="store_true")
     group.add_argument("--next-track", action="store_true")
     group.add_argument("--toggle-playback", action="store_true")
     group.add_argument("--add-track-to-monthly-playlist", action="store_true")
     group.add_argument("--auth", action="store_true")
@@ -433,24 +405,20 @@
     group.add_argument("--init", action="store_true")
 
     args = parser.parse_args()
 
     if args.init:
         first_run()
 
-    spotibar_client = (
-        SpotibarClient(
-            config_file=args.config_filepath,
-            require_clients=False,
-            auth_cache_path=args.auth_filepath,
-        ) if args.is_live else SpotibarClient(
-            config_file=args.config_filepath,
-            auth_cache_path=args.auth_filepath,
-        )
-    )
+        sys.exit(0)
+
+    if args.is_live:
+        spotibar_client = SpotibarClient(require_clients=False)
+    else:
+        spotibar_client = SpotibarClient()
 
     if args.get_currently_playing:
         print(spotibar_client.get_currently_playing_string())
     elif args.previous_track:
         spotibar_client.previous()
     elif args.next_track:
         spotibar_client.next()
```

### Comparing `spotibar-0.3.9/src/spotibar/config_helper.py` & `spotibar-0.4.0/src/spotibar/config_helper.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,52 +1,47 @@
 import json
 import os
 
 
 class SpotibarConfig:
     def __init__(self, *args, **kwargs):
-        self.config_file = kwargs.get("config_file", ".spotibar_config.json")
-
-        self.path = os.path.expanduser("~") + "/" + self.config_file
-
-        # If we supply an absolute path, use that instead of expanding the home
-        # dir.
-        if self.config_file[0] == "/":
-            self.path = self.config_file
+        self.config_file = os.path.expanduser(
+            kwargs.get("config_file", "~/.config/spotibar/default.json")
+        )
 
     def get(self, key, default):
-        if not os.path.exists(self.path):
+        if not os.path.exists(self.config_file):
             return default
         try:
-            with open(self.path, "r") as fh:
+            with open(self.config_file, "r") as fh:
                 config = json.load(fh)
 
                 if key in config.keys():
                     return config[key]
                 else:
                     return default
         except Exception as e:
-            print(f"Problem reading from ~/{self.config_file}!")
+            print(f"Problem reading from {self.config_file}!")
             print(e)
 
     def set(self, key, value):
         config = None
 
         try:
-            with open(self.path, "r") as fh:
+            with open(self.config_file, "r") as fh:
                 config = json.load(fh)
         except Exception as e:
-            print(f"Problem reading from ~/{self.config_file}!")
+            print(f"Problem reading from {self.config_file}!")
             print(e)
 
             return
 
         config[key] = value
 
         try:
-            with open(self.path, "w") as fh:
+            with open(self.config_file, "w") as fh:
                 json.dump(config, fh)
         except Exception as e:
-            print(f"Problem writing to ~/{self.config_file}!")
+            print(f"Problem writing to {self.config_file}!")
             print(e)
 
             return
```

### Comparing `spotibar-0.3.9/src/spotibar/popups.py` & `spotibar-0.4.0/src/spotibar/popups.py`

 * *Files identical despite different names*

