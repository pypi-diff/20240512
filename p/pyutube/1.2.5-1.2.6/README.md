# Comparing `tmp/pyutube-1.2.5.tar.gz` & `tmp/pyutube-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyutube-1.2.5.tar", last modified: Thu Apr 25 18:13:35 2024, max compression
+gzip compressed data, was "pyutube-1.2.6.tar", last modified: Sun May 12 13:30:06 2024, max compression
```

## Comparing `pyutube-1.2.5.tar` & `pyutube-1.2.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0 brhoom    (1000) brhoom    (1000)        0 2024-04-25 18:13:35.335940 pyutube-1.2.5/
--rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)     1078 2024-03-05 00:46:11.000000 pyutube-1.2.5/LICENSE.md
--rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)     8616 2024-04-25 18:13:35.334613 pyutube-1.2.5/PKG-INFO
--rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)     7795 2024-04-25 18:13:26.000000 pyutube-1.2.5/README.md
-drwxrwxrwx   0 brhoom    (1000) brhoom    (1000)        0 2024-04-25 18:13:35.320942 pyutube-1.2.5/pyutube/
--rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)      399 2024-04-07 04:16:19.000000 pyutube-1.2.5/pyutube/__init__.py
--rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)      184 2024-03-31 03:14:16.000000 pyutube-1.2.5/pyutube/__main__.py
--rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)     6728 2024-04-25 18:09:31.000000 pyutube-1.2.5/pyutube/cli.py
--rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)    14053 2024-04-25 18:09:31.000000 pyutube-1.2.5/pyutube/downloader.py
-drwxrwxrwx   0 brhoom    (1000) brhoom    (1000)        0 2024-04-25 18:13:35.331625 pyutube-1.2.5/pyutube/tests/
--rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)       30 2024-02-14 23:03:00.000000 pyutube-1.2.5/pyutube/tests/__init__.py
--rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)     4676 2024-04-12 09:09:48.000000 pyutube-1.2.5/pyutube/tests/test_utils.py
--rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)    11218 2024-04-25 18:12:02.000000 pyutube-1.2.5/pyutube/utils.py
-drwxrwxrwx   0 brhoom    (1000) brhoom    (1000)        0 2024-04-25 18:13:35.332997 pyutube-1.2.5/pyutube.egg-info/
--rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)     8616 2024-04-25 18:13:35.000000 pyutube-1.2.5/pyutube.egg-info/PKG-INFO
--rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)      365 2024-04-25 18:13:35.000000 pyutube-1.2.5/pyutube.egg-info/SOURCES.txt
--rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)        1 2024-04-25 18:13:35.000000 pyutube-1.2.5/pyutube.egg-info/dependency_links.txt
--rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)       44 2024-04-25 18:13:35.000000 pyutube-1.2.5/pyutube.egg-info/entry_points.txt
--rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)       70 2024-04-25 18:13:35.000000 pyutube-1.2.5/pyutube.egg-info/requires.txt
--rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)        8 2024-04-25 18:13:35.000000 pyutube-1.2.5/pyutube.egg-info/top_level.txt
--rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)       38 2024-04-25 18:13:35.336148 pyutube-1.2.5/setup.cfg
--rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)     1436 2024-04-07 04:18:59.000000 pyutube-1.2.5/setup.py
+drwxrwxrwx   0 brhoom    (1000) brhoom    (1000)        0 2024-05-12 13:30:06.923330 pyutube-1.2.6/
+-rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)     1078 2024-04-27 12:45:59.000000 pyutube-1.2.6/LICENSE.md
+-rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)     8619 2024-05-12 13:30:06.920975 pyutube-1.2.6/PKG-INFO
+-rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)     7795 2024-05-12 13:29:54.000000 pyutube-1.2.6/README.md
+drwxrwxrwx   0 brhoom    (1000) brhoom    (1000)        0 2024-05-12 13:30:06.907234 pyutube-1.2.6/pyutube/
+-rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)      399 2024-04-07 04:16:19.000000 pyutube-1.2.6/pyutube/__init__.py
+-rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)      184 2024-03-31 03:14:16.000000 pyutube-1.2.6/pyutube/__main__.py
+-rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)     6728 2024-04-30 18:17:01.000000 pyutube-1.2.6/pyutube/cli.py
+-rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)    14111 2024-05-12 13:19:01.000000 pyutube-1.2.6/pyutube/downloader.py
+drwxrwxrwx   0 brhoom    (1000) brhoom    (1000)        0 2024-05-12 13:30:06.917039 pyutube-1.2.6/pyutube/tests/
+-rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)       30 2024-02-14 23:03:00.000000 pyutube-1.2.6/pyutube/tests/__init__.py
+-rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)     4676 2024-04-12 09:09:48.000000 pyutube-1.2.6/pyutube/tests/test_utils.py
+-rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)    11218 2024-05-12 13:20:14.000000 pyutube-1.2.6/pyutube/utils.py
+drwxrwxrwx   0 brhoom    (1000) brhoom    (1000)        0 2024-05-12 13:30:06.918258 pyutube-1.2.6/pyutube.egg-info/
+-rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)     8619 2024-05-12 13:30:06.000000 pyutube-1.2.6/pyutube.egg-info/PKG-INFO
+-rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)      365 2024-05-12 13:30:06.000000 pyutube-1.2.6/pyutube.egg-info/SOURCES.txt
+-rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)        1 2024-05-12 13:30:06.000000 pyutube-1.2.6/pyutube.egg-info/dependency_links.txt
+-rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)       44 2024-05-12 13:30:06.000000 pyutube-1.2.6/pyutube.egg-info/entry_points.txt
+-rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)       70 2024-05-12 13:30:06.000000 pyutube-1.2.6/pyutube.egg-info/requires.txt
+-rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)        8 2024-05-12 13:30:06.000000 pyutube-1.2.6/pyutube.egg-info/top_level.txt
+-rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)       38 2024-05-12 13:30:06.923832 pyutube-1.2.6/setup.cfg
+-rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)     1439 2024-05-12 13:08:51.000000 pyutube-1.2.6/setup.py
```

### Comparing `pyutube-1.2.5/LICENSE.md` & `pyutube-1.2.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyutube-1.2.5/PKG-INFO` & `pyutube-1.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: pyutube
-Version: 1.2.5
+Version: 1.2.6
 Summary: Awesome CLI to download YouTube videos (as video or audio)/shorts/playlists from the terminal
 Author: Ebraheem Alhetari
 Author-email: hetari4all@gmail.com
 License: MIT
 Project-URL: Homepage, https://github.com/Hetari/pyutube
-Keywords: youtube,download,cli,pyutube,pytube
+Keywords: youtube,download,cli,pyutube,pytubefix
 Platform: Windows
 Platform: MacOS
 Platform: Linux
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
```

#### html2text {}

```diff
@@ -1,20 +1,20 @@
-Metadata-Version: 2.1 Name: pyutube Version: 1.2.5 Summary: Awesome CLI to
+Metadata-Version: 2.1 Name: pyutube Version: 1.2.6 Summary: Awesome CLI to
 download YouTube videos (as video or audio)/shorts/playlists from the terminal
 Author: Ebraheem Alhetari Author-email: hetari4all@gmail.com License: MIT
 Project-URL: Homepage, https://github.com/Hetari/pyutube Keywords:
-youtube,download,cli,pyutube,pytube Platform: Windows Platform: MacOS Platform:
-Linux Classifier: License :: OSI Approved :: MIT License Classifier: Operating
-System :: OS Independent Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
-LICENSE.md Requires-Dist: pytube Requires-Dist: inquirer Requires-Dist: yaspin
-Requires-Dist: typer Requires-Dist: requests Requires-Dist: rich Requires-Dist:
-inquirer Requires-Dist: termcolor Requires-Dist: moviepy # ð¹ YouTube
-Downloader CLI ### Enjoying my project? Please show your appreciation by
-starring it on GitHub! â­ [![Version](https://img.shields.io/pypi/v/
+youtube,download,cli,pyutube,pytubefix Platform: Windows Platform: MacOS
+Platform: Linux Classifier: License :: OSI Approved :: MIT License Classifier:
+Operating System :: OS Independent Classifier: Programming Language :: Python
+:: 3 Requires-Python: >=3.6 Description-Content-Type: text/markdown License-
+File: LICENSE.md Requires-Dist: pytube Requires-Dist: inquirer Requires-Dist:
+yaspin Requires-Dist: typer Requires-Dist: requests Requires-Dist: rich
+Requires-Dist: inquirer Requires-Dist: termcolor Requires-Dist: moviepy # ð¹
+YouTube Downloader CLI ### Enjoying my project? Please show your appreciation
+by starring it on GitHub! â­ [![Version](https://img.shields.io/pypi/v/
 pyutube.svg?style=flat)](https://pypi.org/project/pyutube/) [![Downloads]
 (https://static.pepy.tech/badge/pyutube)](https://pepy.tech/project/pyutube) >
 [!NOTE] > Have a new feature? Please don't hesitate to [tell me](https://
 github.com/Hetari/pyutube/issues/new)! _[_P_y_u_t_u_b_e_]## ð Description This
 command-line tool downloads YouTube videos from the `Terminal`, written under
 [Pytube](https://pytube.io/), and offers a user-friendly interface. it is
 cross-platform (Windows, Mac, Linux) and can be used in any terminal. ## ð¤
```

### Comparing `pyutube-1.2.5/README.md` & `pyutube-1.2.6/README.md`

 * *Files identical despite different names*

### Comparing `pyutube-1.2.5/pyutube/cli.py` & `pyutube-1.2.6/pyutube/cli.py`

 * *Files identical despite different names*

### Comparing `pyutube-1.2.5/pyutube/downloader.py` & `pyutube-1.2.6/pyutube/downloader.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 
 import os
 import sys
 
 
 from yaspin import yaspin
 from yaspin.spinners import Spinners
-from pytube import YouTube, Playlist
-from pytube.cli import on_progress
+from pytubefix import YouTube, Playlist
+from pytubefix.cli import on_progress
 from termcolor import colored
 from moviepy.video.io.ffmpeg_tools import ffmpeg_merge_video_audio
 
 
 class Downloader:
     """
     This class provides functionality for downloading videos from YouTube.
@@ -65,15 +65,14 @@
 
         Args:
             url: The URL of the video to search for.
 
         Returns:
             YouTube: An instance of the YouTube class representing the searched video.
         """
-
         return YouTube(
             url,
             use_oauth=False,
             allow_oauth_cache=True,
             on_progress_callback=on_progress,
         )
 
@@ -389,15 +388,17 @@
 
         # If file with the same name already exists in the path
         if is_file_exists(self.path, video_filename):
             video_filename = self.handle_existing_file(video_filename)
             if not video_filename:
                 sys.exit()
         try:
-            console.print("⏳ Downloading video...", style="info")
+            console.print(
+                f"⏳ Downloading {'audio' if self.is_audio else 'video'}...", style="info")
+
             self.save_file(footage, self.path, video_filename)
 
             if not self.is_audio:
                 self.save_file(video_audio, self.path, audio_filename)
                 self.merging(video_filename, audio_filename)
 
         except Exception as error:
```

### Comparing `pyutube-1.2.5/pyutube/tests/test_utils.py` & `pyutube-1.2.6/pyutube/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `pyutube-1.2.5/pyutube/utils.py` & `pyutube-1.2.6/pyutube/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from yaspin import yaspin
 from yaspin.spinners import Spinners
 from rich.console import Console
 from rich.theme import Theme
 from termcolor import colored
 
 
-__version__ = "1.2.5"
+__version__ = "1.2.6"
 __app__ = "pyutube"
 ABORTED_PREFIX = "aborted"
 CANCEL_PREFIX = "cancel"
 
 
 # Set up the console
 custom_theme = Theme({
```

### Comparing `pyutube-1.2.5/pyutube.egg-info/PKG-INFO` & `pyutube-1.2.6/pyutube.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: pyutube
-Version: 1.2.5
+Version: 1.2.6
 Summary: Awesome CLI to download YouTube videos (as video or audio)/shorts/playlists from the terminal
 Author: Ebraheem Alhetari
 Author-email: hetari4all@gmail.com
 License: MIT
 Project-URL: Homepage, https://github.com/Hetari/pyutube
-Keywords: youtube,download,cli,pyutube,pytube
+Keywords: youtube,download,cli,pyutube,pytubefix
 Platform: Windows
 Platform: MacOS
 Platform: Linux
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
```

#### html2text {}

```diff
@@ -1,20 +1,20 @@
-Metadata-Version: 2.1 Name: pyutube Version: 1.2.5 Summary: Awesome CLI to
+Metadata-Version: 2.1 Name: pyutube Version: 1.2.6 Summary: Awesome CLI to
 download YouTube videos (as video or audio)/shorts/playlists from the terminal
 Author: Ebraheem Alhetari Author-email: hetari4all@gmail.com License: MIT
 Project-URL: Homepage, https://github.com/Hetari/pyutube Keywords:
-youtube,download,cli,pyutube,pytube Platform: Windows Platform: MacOS Platform:
-Linux Classifier: License :: OSI Approved :: MIT License Classifier: Operating
-System :: OS Independent Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
-LICENSE.md Requires-Dist: pytube Requires-Dist: inquirer Requires-Dist: yaspin
-Requires-Dist: typer Requires-Dist: requests Requires-Dist: rich Requires-Dist:
-inquirer Requires-Dist: termcolor Requires-Dist: moviepy # ð¹ YouTube
-Downloader CLI ### Enjoying my project? Please show your appreciation by
-starring it on GitHub! â­ [![Version](https://img.shields.io/pypi/v/
+youtube,download,cli,pyutube,pytubefix Platform: Windows Platform: MacOS
+Platform: Linux Classifier: License :: OSI Approved :: MIT License Classifier:
+Operating System :: OS Independent Classifier: Programming Language :: Python
+:: 3 Requires-Python: >=3.6 Description-Content-Type: text/markdown License-
+File: LICENSE.md Requires-Dist: pytube Requires-Dist: inquirer Requires-Dist:
+yaspin Requires-Dist: typer Requires-Dist: requests Requires-Dist: rich
+Requires-Dist: inquirer Requires-Dist: termcolor Requires-Dist: moviepy # ð¹
+YouTube Downloader CLI ### Enjoying my project? Please show your appreciation
+by starring it on GitHub! â­ [![Version](https://img.shields.io/pypi/v/
 pyutube.svg?style=flat)](https://pypi.org/project/pyutube/) [![Downloads]
 (https://static.pepy.tech/badge/pyutube)](https://pepy.tech/project/pyutube) >
 [!NOTE] > Have a new feature? Please don't hesitate to [tell me](https://
 github.com/Hetari/pyutube/issues/new)! _[_P_y_u_t_u_b_e_]## ð Description This
 command-line tool downloads YouTube videos from the `Terminal`, written under
 [Pytube](https://pytube.io/), and offers a user-friendly interface. it is
 cross-platform (Windows, Mac, Linux) and can be used in any terminal. ## ð¤
```

### Comparing `pyutube-1.2.5/setup.py` & `pyutube-1.2.6/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
     description="Awesome CLI to download YouTube videos (as video or audio)/shorts/playlists from the terminal",
 
     long_description=description,
 
     long_description_content_type="text/markdown",
 
-    keywords=["youtube", "download", "cli", "pyutube", "pytube"],
+    keywords=["youtube", "download", "cli", "pyutube", "pytubefix"],
 
     license="MIT",
 
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
```

