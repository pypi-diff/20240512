# Comparing `tmp/playlist2podcast-0.6.8.tar.gz` & `tmp/playlist2podcast-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "playlist2podcast-0.6.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "playlist2podcast-1.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `playlist2podcast-0.6.8.tar` & `playlist2podcast-1.0.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     4968 2023-12-10 04:28:55.015415 playlist2podcast-0.6.8/README.rst
--rw-r--r--   0        0        0     3375 2023-12-10 04:28:55.015415 playlist2podcast-0.6.8/pyproject.toml
--rw-r--r--   0        0        0      218 2023-12-10 04:28:55.015415 playlist2podcast-0.6.8/src/playlist2podcast/__init__.py
--rw-r--r--   0        0        0    20870 2023-12-10 04:28:55.015415 playlist2podcast-0.6.8/src/playlist2podcast/playlist_2_podcast.py
--rw-r--r--   0        0        0     6114 1970-01-01 00:00:00.000000 playlist2podcast-0.6.8/PKG-INFO
+-rw-r--r--   0        0        0     4968 2024-05-12 09:28:41.903430 playlist2podcast-1.0.0/README.rst
+-rw-r--r--   0        0        0     2489 2024-05-12 09:28:41.903430 playlist2podcast-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      411 2024-05-12 09:28:41.903430 playlist2podcast-1.0.0/src/playlist2podcast/__init__.py
+-rw-r--r--   0        0        0    20319 2024-05-12 09:28:41.903430 playlist2podcast-1.0.0/src/playlist2podcast/playlist_2_podcast.py
+-rw-r--r--   0        0        0     6176 1970-01-01 00:00:00.000000 playlist2podcast-1.0.0/PKG-INFO
```

### Comparing `playlist2podcast-0.6.8/README.rst` & `playlist2podcast-1.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `playlist2podcast-0.6.8/pyproject.toml` & `playlist2podcast-1.0.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -5,47 +5,50 @@
 [project]
 name = "playlist2podcast"
 description = "Creates podcast feed from playlist URL"
 readme = "README.rst"
 authors = [
   { name = "marvin8", email = "marvin8@tuta.io" },
 ]
-requires-python = ">=3.8"
+requires-python = ">=3.8,<3.13"
 license = {text = "AGPL-3.0-or-later"}
-dynamic = ["version"]
+version = "1.0.0"
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
+  "Programming Language :: Python :: 3.12",
 ]
 
 dependencies = [
-    "Pillow>=10.1.0",
-    "arrow>=1.3.0",
-    "feedgen>=0.9.0",
-    "outdated>=0.2.2",
+    "Pillow>=10.3.0",
+    "feedgen>=1.0.0",
+    "pycryptodomex>=3.20.0",
     "requests>=2.31.0",
-    "rich>=13.7.0",
-    "typer>=0.9.0",
-    "typing-extensions>=4.9.0",
-    "yt-dlp>=2023.11.16",
+    "rich>=13.7.1",
+    "typer>=0.12.3",
+    "yt-dlp>=2024.4.9",
 ]
 
 [project.scripts]
 playlist2podcast = "playlist2podcast.playlist_2_podcast:start_main"
 
 [project.urls]
 Documentation = "https://codeberg.org/PyYtTools/Playlist2Podcasts/src/branch/main/README.rst"
 Issues ="https://codeberg.org/PyYtTools/Playlist2Podcasts/issues"
 Source ="https://codeberg.org/PyYtTools/Playlist2Podcasts"
 Changelog = "https://codeberg.org/PyYtTools/Playlist2Podcasts/src/branch/main/CHANGELOG.rst"
 
+[project.optional-dependencies]
+dev = [
+    "icecream>=2.1.3",
+]
 [tool.interrogate]
 ignore-init-method = true
 ignore-init-module = false
 ignore-magic = false
 ignore-semiprivate = false
 ignore-private = false
 ignore-property-decorators = false
@@ -81,58 +84,13 @@
 no_implicit_reexport = true
 
 [tool.pytest.ini_options]
 testpaths = [
 "tests",
 ]
 
-[tool.ruff]
-select = ["ARG", "B", "C4", "C90", "D", "E", "ERA", "F", "I", "PL", "RUF", "S", "UP", "W"]
-ignore = ["D203", "D205", "D213"]
-
-# Allow autofix for all enabled rules (when `--fix`) is provided.
-fixable = ["A", "B", "C", "D", "E", "F", "I", "UP"]
-unfixable = []
-
-# Exclude a variety of commonly ignored directories.
-exclude = [
-    ".bzr",
-    ".direnv",
-    ".eggs",
-    ".git",
-    ".hg",
-    ".mypy_cache",
-    ".nox",
-    ".pants.d",
-    ".ruff_cache",
-    ".svn",
-    ".tox",
-    ".venv",
-    "__pypackages__",
-    "_build",
-    "buck-out",
-    "build",
-    "dist",
-    "node_modules",
-    "venv",
-]
-
-# Same as Black.
-line-length = 120
-
-# Allow unused variables when underscore-prefixed.
-dummy-variable-rgx = "^(_+|(_+[a-zA-Z0-9_]*[a-zA-Z0-9]+?))$"
-
-# Assume Python 3.8.
-target-version = "py38"
-
-[tool.ruff.mccabe]
-# Unlike Flake8, default to a complexity level of 10.
-max-complexity = 10
-
-[tool.ruff.isort]
-force-single-line = true
-
 [tool.scriv]
 categories = "Breaking, Added, Changed, Deprecated, Removed, Fixed, Security"
 format = "rst"
-version = "literal: src/playlist2podcast/__init__.py: __version__"
+version = "literal: pyproject.toml: project.version"
+
+[tool.pdm]
```

### Comparing `playlist2podcast-0.6.8/src/playlist2podcast/playlist_2_podcast.py` & `playlist2podcast-1.0.0/src/playlist2podcast/playlist_2_podcast.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,55 +13,81 @@
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU Affero General Public License for more details.
 
 You should have received a copy of the GNU Affero General Public License
 along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """
-import datetime
+
 import json
 import logging.handlers
 import os
 import re
 from dataclasses import asdict
 from dataclasses import dataclass
+from datetime import datetime
+from datetime import timedelta
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Optional
 from typing import TypeVar
 from typing import Union
 from typing import cast
 
-import arrow
 import requests
 import typer
 from feedgen.feed import FeedEntry
 from feedgen.feed import FeedGenerator
-from outdated import check_outdated
 from PIL import Image
 from rich import print as rprint
 from rich import traceback
 from rich.logging import RichHandler
 from typing_extensions import Annotated
 from yt_dlp import YoutubeDL
 
-from . import __display_name__
-from . import __package_name__
-from . import __version__
+from playlist2podcast import UTC
+from playlist2podcast import __display_name__
+from playlist2podcast import __version__
 
 traceback.install(show_locals=True)
 log = logging.getLogger("VideoPlaylist2Podcast")
 
 CFG = TypeVar("CFG", bound="Configuration")
 
+
+class IgnoringLogger:
+    """Logger class that ignores all logging silently."""
+
+    def debug(self, msg):
+        """Process debug log messages."""
+        # For compatibility with youtube-dl, both debug and info are passed into debug
+        # You can distinguish them by the prefix '[debug] '
+        if msg.startswith("[debug] "):
+            pass
+        else:
+            self.info(msg)
+
+    def info(self, msg):
+        """Process info log messages."""
+        pass
+
+    def warning(self, msg):
+        """Process warning log messages."""
+        pass
+
+    def error(self, msg):
+        """Process error log messages."""
+        pass
+
+
 YDL_DL_OPTS = {
     "quiet": "true",
     "ignoreerrors": "true",
-    "logger": logging.getLogger("Youtube_dl"),
+    "logger": IgnoringLogger(),
     "format": "bestaudio/best",
     "outtmpl": "publish/media/%(id)s.%(ext)s",
     "postprocessors": [
         {
             "key": "FFmpegExtractAudio",
             "preferredcodec": "opus",
         }
@@ -240,40 +266,31 @@
 
     setup_logging(config, debug_log_file)
 
     if publish_dir:
         config.publish_dir = publish_dir
 
     print_welcome()
-    check_updates()
 
     feed = create_feed(config)
 
     downloader = setup_downloader(config)
 
     for current_play_list in config.play_lists:
         rprint(f"Downloading info for videos on playlist: {current_play_list['url']}")
         log.debug("Downloading info for videos on playlist: %s", current_play_list["url"])
-        download_info = downloader.extract_info(
-            url=current_play_list["url"],
-            download=False,
-        )
+        download_info = downloader.extract_info(url=current_play_list["url"], download=False)
         log.debug("main() - download_info = %s", json.dumps(download_info, indent=4))
         videos_list = download_info["entries"]
 
         videos_to_download = determine_videos_to_download(current_play_list, videos_list)
 
         add_episodes(config, downloader, feed, videos_to_download)
 
-    feed.rss_file(
-        f"{config.publish_dir}/feed.rss",
-        extensions=True,
-        pretty=True,
-        xml_declaration=True,
-    )
+    feed.rss_file(filename=f"{config.publish_dir}/feed.rss", extensions=True, pretty=True, xml_declaration=True)
 
 
 def determine_videos_to_download(current_play_list, videos_list) -> List[Any]:
     """Determine list of videos to download."""
     videos_to_download = []
     for video in videos_list:
         if video and is_video_included(
@@ -355,19 +372,15 @@
         If one include filter matches, video will be considered for adding.
     :param exclude_filters: List of regex patterns acting as exclude filters.
         If one exclude filter matches, video will be skipped, even if there is a
         matching include filter. I.e. exclude > include
     :return: True if video should be considered for adding and False if video should
         be skipped based on filters.
     """
-    log.debug(
-        "Filtering: Checking video: '%s' at '%s'",
-        video_title,
-        video_original_url,
-    )
+    log.debug("Filtering: Checking video: '%s' at '%s'", video_title, video_original_url)
 
     should_include_video = False
 
     title_len = len(video_title)
     url_len = len(video_original_url)
 
     if title_len == 0 and url_len == 0:
@@ -423,40 +436,36 @@
     ids_in_feed = {entry.id() for entry in feed.entry()}
     number_episodes_added = 0
     for video in play_list_info:
         video_id = video["id"]
         if number_episodes_added < config.number_of_episodes:
             local_audio_file = f"{config.publish_dir}/{config.media_dir}/{video_id}.opus"
             host_audio_file = f"{config.podcast_host}/{config.media_dir}/{video_id}.opus"
-            thumbnail = get_thumbnail(
-                config=config,
-                video_id=video_id,
-                video=video,
-            )
+            thumbnail = get_thumbnail(config=config, video_id=video_id, video=video)
 
             feed_entry = create_feed_entry(
                 video=video,
                 thumbnail=thumbnail,
                 host_audio_file=host_audio_file,
                 config=config,
             )
             feed.add_entry(feedEntry=feed_entry)
 
             # Download video if needed
             if not os.path.isfile(local_audio_file):
                 rprint(
                     f"Downloading episode with id {feed_entry.id()} "
-                    f"and length {datetime.timedelta(seconds=int(video['duration']))} "
+                    f"and length {timedelta(seconds=int(video['duration']))} "
                     f"uploaded on {feed_entry.published().strftime('%Y-%m-%d')} with "
                     f"title [green]{feed_entry.title()}"
                 )
                 log.debug(
                     "Downloading episode with id %s and length %s uploaded on %s with title %s",
                     feed_entry.id(),
-                    datetime.timedelta(seconds=int(video["duration"])),
+                    timedelta(seconds=int(video["duration"])),
                     feed_entry.published().strftime("%Y-%m-%d"),
                     feed_entry.title(),
                 )
                 downloader.download(url_list=[video["webpage_url"]])
 
             number_episodes_added += 1
             ids_in_feed.add(feed_entry.id())
@@ -479,23 +488,23 @@
 def create_feed_entry(
     video: Dict[str, str],
     thumbnail: str,
     host_audio_file: str,
     config: Configuration,
 ) -> FeedEntry:
     """Create feed entry to add to rss feed."""
-    published_on = arrow.get(video["upload_date"], "YYYYMMDD")
+    published_on = datetime.fromtimestamp(float(video["epoch"]), tz=UTC)
     feed_entry = FeedEntry()
     feed_entry.load_extension("podcast")
     feed_entry.author(name=video["uploader"])
     feed_entry.id(id=video["id"])
     feed_entry.link(href=video["webpage_url"])
     feed_entry.title(title=video["title"])
     feed_entry.description(description=video["description"])
-    feed_entry.published(published=published_on.datetime)
+    feed_entry.published(published=published_on)
     feed_entry.podcast.itunes_image(f"{config.podcast_host}/{config.media_dir}/{thumbnail}")
     feed_entry.podcast.itunes_duration(int(video["duration"]))
     feed_entry.enclosure(url=host_audio_file, type="audio/ogg")
 
     return feed_entry
 
 
@@ -515,42 +524,14 @@
             "Skipping episode with id %s from %s with title %s",
             video["id"],
             video["upload_date"],
             video["title"],
         )
 
 
-def check_updates() -> None:
-    """Check if there is a newer version of MastodonAmnesia available on
-    PyPI.
-    """
-    is_outdated = False
-    try:
-        is_outdated, pypi_version = check_outdated(
-            package=__package_name__,
-            version=__version__,
-        )
-
-        log.debug("Checked for updates for %s version %s", __package_name__, __version__)
-        log.debug("Is outdated: %s (PyPi version: %s)", is_outdated, pypi_version)
-
-        if is_outdated:
-            rprint(
-                f"[bold][red]!!! New version of {__display_name__} ({pypi_version}) " f"is available on PyPI.org !!!\n"
-            )
-            log.debug(
-                "!!! New version of %s (%s) is available on PyPI.org",
-                __display_name__,
-                pypi_version,
-            )
-    except ValueError:
-        rprint("[yellow]Notice - Your version is higher than last published version on PyPI")
-        log.debug("Notice - Your version is higher than the last publish version")
-
-
 def get_thumbnail(config: Configuration, video_id: str, video: Dict[str, Any]) -> str:
     """Get the highest quality thumbnail out of the video dict, converts it to
     JPG and returns the filename of the converted file.
 
     :param config: Configuration class instance
     :param video_id: YouTube video id
     :param video: youtube-dl information dict about one particular video
```

### Comparing `playlist2podcast-0.6.8/PKG-INFO` & `playlist2podcast-1.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 Metadata-Version: 2.1
 Name: playlist2podcast
-Version: 0.6.8
+Version: 1.0.0
 Summary: Creates podcast feed from playlist URL
 Author-email: marvin8 <marvin8@tuta.io>
-Requires-Python: >=3.8
+Requires-Python: >=3.8,<3.13
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: Pillow>=10.1.0
-Requires-Dist: arrow>=1.3.0
-Requires-Dist: feedgen>=0.9.0
-Requires-Dist: outdated>=0.2.2
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: Pillow>=10.3.0
+Requires-Dist: feedgen>=1.0.0
+Requires-Dist: pycryptodomex>=3.20.0
 Requires-Dist: requests>=2.31.0
-Requires-Dist: rich>=13.7.0
-Requires-Dist: typer>=0.9.0
-Requires-Dist: typing-extensions>=4.9.0
-Requires-Dist: yt-dlp>=2023.11.16
+Requires-Dist: rich>=13.7.1
+Requires-Dist: typer>=0.12.3
+Requires-Dist: yt-dlp>=2024.4.9
+Requires-Dist: icecream>=2.1.3 ; extra == "dev"
 Project-URL: Changelog, https://codeberg.org/PyYtTools/Playlist2Podcasts/src/branch/main/CHANGELOG.rst
 Project-URL: Documentation, https://codeberg.org/PyYtTools/Playlist2Podcasts/src/branch/main/README.rst
 Project-URL: Issues, https://codeberg.org/PyYtTools/Playlist2Podcasts/issues
 Project-URL: Source, https://codeberg.org/PyYtTools/Playlist2Podcasts
+Provides-Extra: dev
 
 Playlist2Podcast
 ================
 
 |Repo| |Downloads| |Code style| |Checked against| |Checked with| |PyPI - Python Version| |PyPI - Wheel|
 |CI - Woodpecker| |AGPL|
```

