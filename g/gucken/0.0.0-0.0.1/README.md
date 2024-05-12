# Comparing `tmp/gucken-0.0.0.tar.gz` & `tmp/gucken-0.0.1.tar.gz`

## Comparing `gucken-0.0.0.tar` & `gucken-0.0.1.tar`

### file list

```diff
@@ -1,36 +1,38 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gucken-0.0.0/src/gucken/__init__.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 gucken-0.0.0/src/gucken/__main__.py
--rw-r--r--   0        0        0     3878 2020-02-02 00:00:00.000000 gucken-0.0.0/src/gucken/aniskip.py
--rw-r--r--   0        0        0    19475 2020-02-02 00:00:00.000000 gucken-0.0.0/src/gucken/gucken.py
--rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 gucken-0.0.0/src/gucken/gucken.tcss
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gucken-0.0.0/src/gucken/hoster/__init__.py
--rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 gucken-0.0.0/src/gucken/hoster/common.py
--rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 gucken-0.0.0/src/gucken/hoster/doodstream.py
--rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 gucken-0.0.0/src/gucken/hoster/streamtape.py
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 gucken-0.0.0/src/gucken/hoster/veo.py
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 gucken-0.0.0/src/gucken/hoster/vidoza.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gucken-0.0.0/src/gucken/player/__init__.py
--rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 gucken-0.0.0/src/gucken/player/android.py
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 gucken-0.0.0/src/gucken/player/common.py
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 gucken-0.0.0/src/gucken/player/ffplay.py
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 gucken-0.0.0/src/gucken/player/mpv.py
--rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 gucken-0.0.0/src/gucken/player/vlc.py
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 gucken-0.0.0/src/gucken/player/wmplayer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gucken-0.0.0/src/gucken/provider/__init__.py
--rw-r--r--   0        0        0     9790 2020-02-02 00:00:00.000000 gucken-0.0.0/src/gucken/provider/aniworld.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 gucken-0.0.0/src/gucken/provider/burningseries.py
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 gucken-0.0.0/src/gucken/provider/common.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 gucken-0.0.0/src/gucken/provider/crunchyroll.py
--rw-r--r--   0        0        0     9848 2020-02-02 00:00:00.000000 gucken-0.0.0/src/gucken/provider/serienstream.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 gucken-0.0.0/src/gucken/provider/streamcloud.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gucken-0.0.0/src/gucken/tracker/__init__.py
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 gucken-0.0.0/src/gucken/tracker/anilist.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 gucken-0.0.0/src/gucken/tracker/aniworld.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 gucken-0.0.0/src/gucken/tracker/common.py
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 gucken-0.0.0/src/gucken/tracker/myanimelist.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 gucken-0.0.0/src/gucken/tracker/serienstream.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 gucken-0.0.0/.gitignore
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 gucken-0.0.0/LICENSE.txt
--rw-r--r--   0        0        0     4186 2020-02-02 00:00:00.000000 gucken-0.0.0/README.md
--rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 gucken-0.0.0/pyproject.toml
--rw-r--r--   0        0        0     6361 2020-02-02 00:00:00.000000 gucken-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 gucken-0.0.1/src/gucken/__init__.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 gucken-0.0.1/src/gucken/__main__.py
+-rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 gucken-0.0.1/src/gucken/aniskip.py
+-rw-r--r--   0        0        0    22746 2020-02-02 00:00:00.000000 gucken-0.0.1/src/gucken/gucken.py
+-rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 gucken-0.0.1/src/gucken/gucken.tcss
+-rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 gucken-0.0.1/src/gucken/update.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gucken-0.0.1/src/gucken/hoster/__init__.py
+-rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 gucken-0.0.1/src/gucken/hoster/common.py
+-rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 gucken-0.0.1/src/gucken/hoster/doodstream.py
+-rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 gucken-0.0.1/src/gucken/hoster/streamtape.py
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 gucken-0.0.1/src/gucken/hoster/veo.py
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 gucken-0.0.1/src/gucken/hoster/vidoza.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gucken-0.0.1/src/gucken/player/__init__.py
+-rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 gucken-0.0.1/src/gucken/player/android.py
+-rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 gucken-0.0.1/src/gucken/player/common.py
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 gucken-0.0.1/src/gucken/player/ffplay.py
+-rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 gucken-0.0.1/src/gucken/player/flatpak.py
+-rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 gucken-0.0.1/src/gucken/player/mpv.py
+-rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 gucken-0.0.1/src/gucken/player/vlc.py
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 gucken-0.0.1/src/gucken/player/wmplayer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gucken-0.0.1/src/gucken/provider/__init__.py
+-rw-r--r--   0        0        0     9780 2020-02-02 00:00:00.000000 gucken-0.0.1/src/gucken/provider/aniworld.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 gucken-0.0.1/src/gucken/provider/burningseries.py
+-rw-r--r--   0        0        0     1757 2020-02-02 00:00:00.000000 gucken-0.0.1/src/gucken/provider/common.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 gucken-0.0.1/src/gucken/provider/crunchyroll.py
+-rw-r--r--   0        0        0     9819 2020-02-02 00:00:00.000000 gucken-0.0.1/src/gucken/provider/serienstream.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 gucken-0.0.1/src/gucken/provider/streamcloud.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gucken-0.0.1/src/gucken/tracker/__init__.py
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 gucken-0.0.1/src/gucken/tracker/anilist.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 gucken-0.0.1/src/gucken/tracker/aniworld.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 gucken-0.0.1/src/gucken/tracker/common.py
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 gucken-0.0.1/src/gucken/tracker/myanimelist.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 gucken-0.0.1/src/gucken/tracker/serienstream.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 gucken-0.0.1/.gitignore
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 gucken-0.0.1/LICENSE.txt
+-rw-r--r--   0        0        0     4497 2020-02-02 00:00:00.000000 gucken-0.0.1/README.md
+-rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 gucken-0.0.1/pyproject.toml
+-rw-r--r--   0        0        0     6771 2020-02-02 00:00:00.000000 gucken-0.0.1/PKG-INFO
```

### Comparing `gucken-0.0.0/src/gucken/aniskip.py` & `gucken-0.0.1/src/gucken/aniskip.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,14 @@
-from httpx import AsyncClient
-from .tracker.myanimelist import search
 from difflib import SequenceMatcher
+from tempfile import NamedTemporaryFile
 from typing import Union
-from tempfile import TemporaryFile
+
+from httpx import AsyncClient
+
+from .tracker.myanimelist import search
 
 
 # TODO: improve fuzzy
 
 def fuzzy_search(pattern, possibilities, threshold=0.6):
     matches = []
     for word in possibilities:
@@ -85,19 +87,16 @@
             ";FFMETADATA1" +
             chapter(op_start_time, op_end_time, "Opening") +
             chapter(ed_start_time, ed_end_time, "Ending") +
             chapter(op_end_time, ed_start_time, "Episode")
     )
 
 
-def generate_chapters_file(timings=dict[str, float]) -> TemporaryFile:
-    temp_file = TemporaryFile(mode='w', prefix="gucken-", delete=False)
+def generate_chapters_file(timings=dict[str, float]) -> NamedTemporaryFile:
+    temp_file = NamedTemporaryFile(mode='w', prefix="gucken-", delete=False)
     temp_file.write(get_chapters_file_content(timings))
+    temp_file.close()
     return temp_file
 
 
 def get_chapters_file_mpv_option(path: str) -> str:
     return f"--chapters-file={path}"
-
-
-def generate_chapters_file_and_get_mpv_option(timings=dict[str, float]) -> str:
-    return get_chapters_file_mpv_option(generate_chapters_file(timings).name)
```

### Comparing `gucken-0.0.0/src/gucken/gucken.py` & `gucken-0.0.1/src/gucken/gucken.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,86 +1,142 @@
-# !/usr/bin/env python3
-# -*- coding: utf-8 -*-
-
-"""
-MIT License
-
-Copyright (c) 2024 Commandcracker
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
-"""
-
-from textual.reactive import reactive
-from textual.screen import ModalScreen
-
-# built-in modules
+import asyncio
+import logging
+import sys
+from atexit import register as register_atexit
 from asyncio import gather
+from os import name as os_name, getenv, remove
+from os.path import join
+from pathlib import Path
+from random import choice
 from shutil import which
+from subprocess import PIPE, Popen, DEVNULL
 from time import sleep, time
 from typing import Union
-from subprocess import Popen, PIPE
-from os import name as os_name
-import sys
 
-# pip modules
-# import mpv
-# import ytdl
+from pypresence import AioPresence, DiscordNotFound
 from textual import events, on, work
-from random import choice
 from textual.app import App, ComposeResult
-from textual.containers import Center, Container, Horizontal, ScrollableContainer
+from textual.containers import (Center, Container, Horizontal,
+                                ScrollableContainer)
+from textual.reactive import reactive
+from textual.screen import ModalScreen
 from textual.widgets import (Button, Checkbox, DataTable, Footer, Header,
                              Input, Label, ListItem, ListView, Markdown,
-                             TabbedContent, TabPane, Static, Switch, RadioButton)
-from textual.widgets._toggle_button import ToggleButton
+                             RadioButton, TabbedContent, TabPane)
 
-from .provider.common import SearchResult, Series, Episode, Language
-from .provider.aniworld import AniWorldProvider
-from .provider.serienstream import SerienStreamProvider
+from .update import check
+from .aniskip import (get_timings_from_search, timings_to_mpv_options, generate_chapters_file,
+                      get_chapters_file_mpv_option)
+from .hoster.common import DirectLink, Hoster
+from .hoster.doodstream import DoodstreamHoster
+from .hoster.streamtape import StreamtapeHoster
+from .hoster.veo import VOEHoster
+from .hoster.vidoza import VidozaHoster
+from .player.android import (AndroidChoosePlayer, AndroidMPVPlayer,
+                             AndroidVLCPlayer)
 from .player.common import Player
-from .player.mpv import MPVPlayer
+from .player.ffplay import FFPlayPlayer
+from .player.mpv import MPVPlayer, MPV_NETPlayer, CelluloidPlayer
 from .player.vlc import VLCPlayer
 from .player.wmplayer import WMPlayer
-from .player.ffplay import FFPlayPlayer
-from .player.android import AndroidVLCPlayer, AndroidMPVPlayer, AndroidChoosePlayer
-from .hoster.common import Hoster, DirectLink
-from .hoster.veo import VOEHoster
-from .hoster.vidoza import VidozaHoster
-from .hoster.streamtape import StreamtapeHoster
-from .hoster.doodstream import DoodstreamHoster
-from .aniskip import (
-    get_timings_from_search,
-    timings_to_mpv_options,
-    generate_chapters_file_and_get_mpv_option
-)
-
-import logging
-from pathlib import Path
+from .player.flatpak import FlatpakMPVPlayer, FlatpakVLCPlayer, FlatpakCelluloidPlayer
+from .provider.aniworld import AniWorldProvider
+from .provider.common import Episode, Language, SearchResult, Series
+from .provider.serienstream import SerienStreamProvider
 
+# TODO: fix this mess
 logs_path = Path(__file__).parent.parent.parent.joinpath("logs")
 logs_path.mkdir(exist_ok=True, parents=True)
 logging.basicConfig(filename=logs_path.joinpath("gucken.log"), encoding='utf-8', level=logging.INFO)
 
 
+def detect_player() -> Union[Player, None]:
+    if hasattr(sys, 'getandroidapilevel'):
+        # TODO: detect right
+        return AndroidMPVPlayer()
+        # return AndroidVLCPlayer()
+        # return AndroidChoosePlayer()
+        # return None
+
+    if os_name == "nt":
+        if which("mpv.exe"):
+            return MPVPlayer("mpv.exe")
+    elif which("mpv"):
+        return MPVPlayer()
+
+    if os_name == "nt":
+        if which("mpvnet.exe"):
+            return MPV_NETPlayer()
+        if getenv("LOCALAPPDATA"):
+            mpvnet = join(getenv("LOCALAPPDATA"), "Programs", "mpv.net", "mpvnet.exe")
+            if which(mpvnet):
+                return MPV_NETPlayer(mpvnet)
+
+    if os_name == "posix":
+        if which("celluloid"):
+            return CelluloidPlayer()
+
+    if which("vlc"):
+        return VLCPlayer()
+
+    if os_name == "posix":
+        # TODO: fix this will slow down
+        if which("flatpak"):
+            p = Popen(["flatpak", "info", "io.mpv.Mpv"], stdout=DEVNULL, stderr=DEVNULL, stdin=DEVNULL)
+            if p.wait() == 0:
+                return FlatpakMPVPlayer()
+            p = Popen(["flatpak", "info", "io.github.celluloid_player.Celluloid"], stdout=DEVNULL, stderr=DEVNULL,
+                      stdin=DEVNULL)
+            if p.wait() == 0:
+                return FlatpakCelluloidPlayer()
+            p = Popen(["flatpak", "info", "org.videolan.VLC"], stdout=DEVNULL, stderr=DEVNULL, stdin=DEVNULL)
+            if p.wait() == 0:
+                return FlatpakVLCPlayer()
+
+    if os_name == "nt":
+        vlc = r"C:\Program Files\VideoLAN\VLC\vlc.exe"
+        if which(vlc):
+            return VLCPlayer(vlc)
+
+    if which("ffplay"):
+        return FFPlayPlayer()
+
+    if os_name == "nt":
+        return WMPlayer()
+
+    return None
+
+
+def sort_favorite_lang(language_list: list[Language]) -> list[Language]:
+    return sorted(language_list, key=lambda x: (
+        x != Language.DE,
+        x != Language.JP_DESUB,
+        x != Language.JP_ENSUB,
+    ))
+
+
+def sort_favorite_hoster(hoster_list: list[Hoster]) -> list[Hoster]:
+    return sorted(hoster_list, key=lambda x: (
+        not isinstance(x, StreamtapeHoster),
+        not isinstance(x, VOEHoster),
+        not isinstance(x, VidozaHoster),
+        not isinstance(x, DoodstreamHoster),
+    ))
+
+
+async def get_working_direct_link(hosters: list[Hoster]) -> Union[DirectLink, None]:
+    for hoster in hosters:
+        direct_link = await hoster.get_direct_link()
+        is_working = await direct_link.check_is_working()
+        logging.info('Check: "%s" Working: "%s" URL: "%s"', type(hoster).__name__, is_working, direct_link)
+        if is_working:
+            return direct_link
+    return None
+
+
 class Next(ModalScreen):
     time = reactive(3)
 
     def __init__(self, question: str, no_time: bool = False):
         super().__init__()
         self.question = question
         self.no_time = no_time
@@ -133,23 +189,28 @@
         if row_index <= -1:
             return
         if self.last_click.get(row_index) and time() - self.last_click[row_index] < 0.5:
             self.app.play_selected()
         self.last_click[row_index] = time()
 
 
+client_id = "1238219157464416266"
+
+
 class GuckenApp(App):
     TITLE = "Gucken TUI"
     # TODO: color theme https://textual.textualize.io/guide/design/#designing-with-colors
     CSS_PATH = "gucken.tcss"
 
     def __init__(self):
         super().__init__()
         self.current: Union[list[SearchResult], None] = None
         self.current_info: Union[Series, None] = None
+        self.player = detect_player()
+        self.RPC: Union[AioPresence, None] = None
 
     def compose(self) -> ComposeResult:
         yield Header()
         with TabbedContent():
             with TabPane("Search", id="search"):  # Search "🔎"
                 with Horizontal(id="hosters"):
                     yield Checkbox("AniWorld.to", True, id="aniworld_to")
@@ -157,81 +218,115 @@
                 yield Input(id="input", placeholder="Search for a Anime")
                 yield ListView(id="results")
             with TabPane("Info", id="info", disabled=True):  # Info "ℹ"
                 with ScrollableContainer(id="res_con"):
                     yield Markdown(id="markdown")
                     yield ClickableDataTable(id="season_list")
             with TabPane("Settings", id="setting"):  # Settings "⚙"
+                # TODO: dont show unneeded on android
                 yield RadioButton("Fullscreen", id="fullscreen", value=True)
                 yield RadioButton("Syncplay", id="syncplay", value=False)
                 yield RadioButton("ani-skip", id="ani_skip", value=True)
+                yield RadioButton("Discord Presence", id="discord_presence", value=False)
             # with RadioSet():
             #    yield RadioButton("VOE", id="voe", value=True)
             #    yield RadioButton("Doodstream", id="doodstream")
             #    yield RadioButton("Vidoza", id="vidoza")
             #    yield RadioButton("Streamtape", id="streamtape")
         with Footer():
             with Center():
                 yield Label("Made by Commandcracker with ❤")
 
-    def on_mount(self) -> None:
+    # TODO: dont lock - no async
+    async def on_mount(self) -> None:
         self.query_one(Input).focus()
-        self.query_one("#info", TabPane).set_loading(True)
+        # TODO: FIx sometimes not disabling loading
+        # TODO: dont lock
+        await self.query_one("#info", TabPane).set_loading(True)
         table = self.query_one(DataTable)
         table.cursor_type = "row"
         # TODO: make them scale
         table.add_columns("FT", "S", "F", "Name", "Title", "Hoster", "Sprache")
-        if not which("mpv"):
+        if self.player is None:
             self.notify(
-                "You wont be able to play videos directly.\n"
-                "Please install MPV!",
-                title="MPV not found",
+                "You wont be able to play videos.\n"
+                "Without an supported video player!",
+                title="No player found",
                 severity="warning",
             )
+        self.update_check()
+        # TODO: dont lock
+        if self.query_one("#discord_presence", RadioButton).value is True:
+            await self.enable_RPC()
+        else:
+            await self.disable_RPC()
+
+    async def enable_RPC(self):
+        if self.RPC is None:
+            self.RPC = AioPresence(client_id)
+        try:
+            await self.RPC.connect()
+        except DiscordNotFound:
+            pass
+
+    async def disable_RPC(self):
+        if self.RPC is not None:
+            await self.RPC.clear()
+            # close without closing event loop
+            self.RPC.send_data(2, {'v': 1, 'client_id': self.RPC.client_id})
+            self.RPC.sock_writer.close()
+            self.RPC = None
 
     async def on_checkbox_changed(self):
         self.lookup_anime(self.query_one("#input", Input).value)
 
+    async def on_radio_button_changed(self, event: RadioButton.Changed):
+        if event.radio_button.id == "discord_presence":
+            if event.value is True:
+                await self.enable_RPC()
+            else:
+                await self.disable_RPC()
+
     async def on_input_changed(self, message: Input.Changed) -> None:
         if message.value:
             self.lookup_anime(message.value)
         else:
             await self.query_one("#results", ListView).clear()
 
     # TODO: https://textual.textualize.io/guide/workers/#thread-workers
     @work(exclusive=True)
     async def lookup_anime(self, keyword: str) -> None:
-
-        owos = []
+        search_providers = []
         if self.query_one("#aniworld_to", Checkbox).value:
-            owos.append(AniWorldProvider.search(keyword))
+            search_providers.append(AniWorldProvider.search(keyword))
 
         if self.query_one("#serienstream_to", Checkbox).value:
-            owos.append(SerienStreamProvider.search(keyword))
+            search_providers.append(SerienStreamProvider.search(keyword))
 
-        lv = self.query_one("#results", ListView)
-        await lv.clear()
-        await lv.set_loading(True)
-        results = await gather(*owos)
-        f_results = []
+        results_list_view = self.query_one("#results", ListView)
+        await results_list_view.clear()
+        await results_list_view.set_loading(True)
+        results = await gather(*search_providers)
+        final_results = []
         for l in results:
             if l is not None:
                 for e in l:
-                    f_results.append(e)
+                    final_results.append(e)
 
-        # TODO: stor f_results by fuzzy sort keyword
-        if len(f_results) > 0:
-            self.current = f_results
-            for series in f_results:
-                await lv.append(ClickableListItem(Markdown(
+        # TODO: Sort final_results with fuzzy-sort
+        if len(final_results) > 0:
+            self.current = final_results
+            for series in final_results:
+                await results_list_view.append(ClickableListItem(Markdown(
                     f"##### **{series.name}** {series.production_year}\n{series.description}"
                 )))
-        await lv.set_loading(False)
-        if len(f_results) > 0:
-            lv.index = 0
+        await results_list_view.set_loading(False)
+        if len(final_results) > 0:
+            # TODO: FIX this sometimes makes the program crash
+            results_list_view.index = 0
 
     async def on_key(self, event: events.Key) -> None:
         key = event.key
         if self.screen.id == "_default":
             if self.query_one(TabbedContent).active == "search":
                 lv = self.query_one("#results", ListView)
                 inp = self.query_one("#input", Input)
@@ -254,61 +349,27 @@
                         if key == "backspace":
                             inp.action_delete_left()
                         else:
                             await inp.on_event(event)
             if key == "enter" and self.query_one(DataTable).has_focus:
                 self.play_selected()
 
-    def sort_favorite_lang(self, language_list: list[Language]) -> list[Language]:
-        return sorted(language_list, key=lambda x: (
-            x != Language.DE,
-            x != Language.JP_DESUB,
-            x != Language.JP_ENSUB,
-        ))
-
-    def sort_favorite_hoster(self, hoster_list: list[Hoster]) -> list[Hoster]:
-        return sorted(hoster_list, key=lambda x: (
-            not isinstance(x, StreamtapeHoster),
-            not isinstance(x, VOEHoster),
-            not isinstance(x, VidozaHoster),
-            not isinstance(x, DoodstreamHoster),
-        ))
-
-    async def get_working_direct_link(self, hosters: list[Hoster]) -> Union[DirectLink, None]:
-        for hoster in hosters:
-            direct_link = await hoster.get_direct_link()
-            is_working = await direct_link.check_is_working()
-            logging.info('Check: "%s" Working: "%s" URL: "%s"', type(hoster).__name__, is_working, direct_link)
-            if is_working:
-                return direct_link
-        return None
-
     @work(exclusive=True)
     async def play_selected(self):
-        # TODO: cache more
-        # TODO: dont only check for mpv
-        #if which("mpv"):
         dt = self.query_one(DataTable)
         # TODO: show loading
         await dt.set_loading(True)
         index = self.app.query_one("#results", ListView).index
         series_search_result = self.current[index]
         self.play(
-                series_search_result=series_search_result,
-                episodes=self.current_info.episodes,
-                index=dt.cursor_row
-            )
+            series_search_result=series_search_result,
+            episodes=self.current_info.episodes,
+            index=dt.cursor_row
+        )
         await dt.set_loading(False)
-        #else:
-        #    self.notify(
-        #        "You wont be able to play videos directly.\n"
-        #        "Please install MPV!",
-        #        title="MPV not found",
-        #        severity="error",
-        #    )
 
     @work(exclusive=True)
     async def open_info(self) -> None:
         series_search_result: SearchResult = self.current[self.app.query_one("#results", ListView).index]
         info_tab = self.query_one("#info", TabPane)
         info_tab.disabled = False
         self.query_one(TabbedContent).active = "info"
@@ -351,106 +412,115 @@
                 "",
                 ", ".join(hl),
                 ", ".join(ll)
             )
         table.focus(scroll_visible=False)
         await info_tab.set_loading(False)
 
-    def detect_player(self) -> Union[Player, None]:
-        # Android
-        if hasattr(sys, 'getandroidapilevel'):
-            # TODO: detect right
-            return AndroidMPVPlayer()
-            #return AndroidVLCPlayer()
-            #return AndroidChoosePlayer()
-            #return None
-
-        # All
-        if which("mpv"):
-            return MPVPlayer()
-        if which("vlc"):
-            return VLCPlayer()
-
-        # Windows
-        if os_name == "nt":
-            if which(r"C:\Program Files\VideoLAN\VLC\vlc.exe"):
-                # r"C:\Program Files\VideoLAN\VLC\vlc.exe"
-                return VLCPlayer()
-
-        if which("ffplay"):
-            return FFPlayPlayer()
-
-        # Windows
-        if os_name == "nt":
-            return WMPlayer()
-
-        return None
+    @work(exclusive=True, thread=True)
+    async def update_check(self):
+        res = await check()
+        if res:
+            self.notify(
+                f"{res.current} -> {res.latest}\npip install -U gucken",
+                title="Update available",
+                severity="information",
+            )
 
     @work(thread=True)
     async def play(
             self,
             series_search_result: SearchResult,
             episodes: list[Episode],
             index: int
     ) -> None:
         episode: Episode = episodes[index]
         processed_hoster = await episode.process_hoster()
 
-        lang = self.sort_favorite_lang(episode.available_language)[0]
-        sorted_hoster = self.sort_favorite_hoster(processed_hoster.get(lang))
-        direct_link = await self.get_working_direct_link(sorted_hoster)
+        lang = sort_favorite_lang(episode.available_language)[0]
+        sorted_hoster = sort_favorite_hoster(processed_hoster.get(lang))
+        direct_link = await get_working_direct_link(sorted_hoster)
 
-        player = self.detect_player()
+        # TODO: check for header support
 
-        if player is None:
-            raise RuntimeError()
+        if self.player is None:
+            self.notify(
+                "You wont be able to play videos.\n"
+                "Without an supported video player!",
+                title="No player found",
+                severity="error",
+            )
+            return
 
-        # TODO: ani_skip, syncplay, fullscreen as arg
+        # TODO: ani_skip, syncplay, fullscreen as cli arg
         # TODO: pass ani_skip as script
         ani_skip = self.query_one("#ani_skip", RadioButton).value
         syncplay = self.query_one("#syncplay", RadioButton).value
         fullscreen = self.query_one("#fullscreen", RadioButton).value
 
         title = f"{series_search_result.name} - {episode.title}"
+        args = self.player.play(direct_link.url, title, fullscreen, direct_link.headers)
+
+        if self.RPC and self.RPC.sock_writer:
+            async def update():
+                await self.RPC.update(
+                    #state="00:20:00 / 00:25:00 57% complete",
+                    details=title[:128],
+                    large_text=title,
+                    large_image=series_search_result.cover,
+                    # small_image as playing or stopped ?
+                    #small_image="https://jooinn.com/images/lonely-tree-reflection-3.jpg",
+                    #small_text="ff 15",
+                    # start=time.time(), # for paused
+                    # end=time.time() + timedelta(minutes=20).seconds   # for time left
+                )
 
-        path = None
-        if isinstance(player, VLCPlayer):
-            if not which("vlc"):
-                if which(r"C:\Program Files\VideoLAN\VLC\vlc.exe"):
-                    path = r"C:\Program Files\VideoLAN\VLC\vlc.exe"
+            self.app.call_later(update)
 
-        args = player.play(direct_link.url, title, fullscreen, direct_link.headers, path)
+        chapters_file = None
 
-        if isinstance(player, MPVPlayer):
+        # TODO: cache more
+        if isinstance(self.player, MPVPlayer):
             if ani_skip:
                 timings = await get_timings_from_search(series_search_result.name, index + 1)
                 if timings:
+                    chapters_file = generate_chapters_file(timings)
+
+                    def delete_chapters_file():
+                        try:
+                            remove(chapters_file.name)
+                        except FileNotFoundError:
+                            pass
+
+                    register_atexit(delete_chapters_file)
                     # --start=00:56
                     args += [
                         timings_to_mpv_options(timings),
-                        generate_chapters_file_and_get_mpv_option(timings)
+                        get_chapters_file_mpv_option(chapters_file.name)
                     ]
 
         if syncplay:
+            # TODO: make work with flatpak
+            # TODO: make work with android
             syncplay_path = None
             if which("syncplay"):
                 syncplay_path = "syncplay"
             if not syncplay_path:
                 if os_name == "nt":
                     if which(r"C:\Program Files (x86)\Syncplay\Syncplay.exe"):
                         syncplay_path = r"C:\Program Files (x86)\Syncplay\Syncplay.exe"
             if not syncplay_path:
                 self.notify(
                     "Syncplay not found",
                     title="Syncplay not found",
                     severity="error",
                 )
             else:
-                if isinstance(player, MPVPlayer) or isinstance(player, VLCPlayer):
-                    # TODO: dont detect mpv.com
+                # TODO: add mpv.net, IINA, MPC-BE, MPC-HE, celluloid ?
+                if isinstance(self.player, MPVPlayer) or isinstance(self.player, VLCPlayer):
                     player_path = which(args[0])
                     url = args[1]
                     args.pop(0)
                     args.pop(0)
                     args = [syncplay_path, "--player-path", player_path, url, "--"] + args
                 else:
                     self.notify(
@@ -458,15 +528,17 @@
                         title="Player not supported",
                         severity="warning",
                     )
 
         logging.info("Running: %s", args)
         process = Popen(
             args,
-            stderr=PIPE
+            stderr=PIPE,
+            stdout=DEVNULL,
+            stdin=DEVNULL
         )
         while not self.app._exit:
             sleep(0.1)
 
             resume_time = None
 
             # only if mpv
@@ -483,25 +555,33 @@
 
             if resume_time:
                 logging.info("Resume: %s", resume_time)
 
             exit_code = process.poll()
 
             if exit_code is not None:
+                if chapters_file:
+                    try:
+                        remove(chapters_file.name)
+                    except FileNotFoundError:
+                        pass
+                if self.RPC and self.RPC.sock_writer:
+                    self.app.call_later(self.RPC.clear)
 
                 async def push_next_screen():
                     async def play_next(should_next):
                         if should_next:
                             self.play(
                                 series_search_result,
                                 episodes,
                                 index + 1,
                             )
 
-                    await self.app.push_screen(Next("Playing next episode in", no_time=hasattr(sys, 'getandroidapilevel')), callback=play_next)
+                    await self.app.push_screen(
+                        Next("Playing next episode in", no_time=hasattr(sys, 'getandroidapilevel')), callback=play_next)
 
                 self.app.call_later(push_next_screen)
                 return
 
 
 exit_quotes = [
     "Closing one anime is just an invitation to open another.",
```

### Comparing `gucken-0.0.0/src/gucken/gucken.tcss` & `gucken-0.0.1/src/gucken/gucken.tcss`

 * *Files identical despite different names*

### Comparing `gucken-0.0.0/src/gucken/hoster/common.py` & `gucken-0.0.1/src/gucken/hoster/common.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from abc import abstractmethod
-from dataclasses import dataclass, field
-from httpx import HTTPError, AsyncClient
+from dataclasses import dataclass
+
+from httpx import AsyncClient, HTTPError
 
 
 @dataclass
 class DirectLink:
     url: str
     headers: dict[str, str] = None
 
@@ -24,12 +25,12 @@
             return True
         return False
 
 
 @dataclass
 class Hoster:
     url: str
-    requires_headers: bool = field(default=False, init=False)
+    requires_headers: bool = False
 
     @abstractmethod
     async def get_direct_link(self) -> DirectLink:
         raise NotImplementedError
```

### Comparing `gucken-0.0.0/src/gucken/hoster/doodstream.py` & `gucken-0.0.1/src/gucken/hoster/doodstream.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from dataclasses import dataclass
-
-from httpx import AsyncClient
-from time import time
 from random import choices
-from string import ascii_letters, digits
 from re import compile as re_compile
+from string import ascii_letters, digits
+from time import time
 from urllib.parse import urlparse
-from .common import Hoster, DirectLink
+
+from httpx import AsyncClient
+
+from .common import DirectLink, Hoster
 
 EXTRACT_DOODSTREAM_HLS_PATTERN = re_compile(r"/pass_md5/[\w-]+/[\w-]+")
 
 
 def random_str(length: int = 10) -> str:
     return ''.join(choices(ascii_letters + digits, k=length))
 
@@ -18,14 +19,15 @@
 def js_date_now() -> int:
     return int(time() * 1000)
 
 
 headers = {'Referer': 'https://d0000d.com/'}
 
 
+@dataclass
 class DoodstreamHoster(Hoster):
     requires_headers = True
 
     async def get_direct_link(self) -> DirectLink:
         async with (AsyncClient(verify=False) as client):
             response = await client.head(self.url)
             if response.has_redirect_location:
```

### Comparing `gucken-0.0.0/src/gucken/hoster/streamtape.py` & `gucken-0.0.1/src/gucken/hoster/streamtape.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from re import compile as re_compile
+
 from httpx import AsyncClient
-from .common import Hoster, DirectLink
+
+from .common import DirectLink, Hoster
 
 STREAMTAPE_PATTERN = re_compile(r'botlink(.*?)innerHTML(.*?)\);')
 STREAMTAPE_PATTERN_SUBSTRING = re_compile(r'substring\(\d+')
 STREAMTAPE_PATTERN_DIGETS = re_compile(r'\d+')
 
 
 class StreamtapeHoster(Hoster):
```

### Comparing `gucken-0.0.0/src/gucken/hoster/veo.py` & `gucken-0.0.1/src/gucken/hoster/veo.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from base64 import b64decode
 from re import compile as re_compile
+
 from httpx import AsyncClient
-from .common import Hoster, DirectLink
+
+from .common import DirectLink, Hoster
 
 EXTRACT_VEO_HLS_PATTERN = re_compile(r"'hls': '(.*?)'")
 
 
 class VOEHoster(Hoster):
     async def get_direct_link(self) -> DirectLink:
         async with AsyncClient(verify=False) as client:
```

### Comparing `gucken-0.0.0/src/gucken/hoster/vidoza.py` & `gucken-0.0.1/src/gucken/hoster/vidoza.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from re import compile as re_compile
+
 from httpx import AsyncClient
-from .common import Hoster, DirectLink
+
+from .common import DirectLink, Hoster
 
 # TODO: improve all patterns
 EXTRACT_VIDOZA_HLS_PATTERN = re_compile(r"sourcesCode:.*?\[.*?\{.*?src:.*?[\'|\"](?P<hls>.*?)[\'|\"],")
 
 
 class VidozaHoster(Hoster):
     async def get_direct_link(self) -> DirectLink:
```

### Comparing `gucken-0.0.0/src/gucken/player/android.py` & `gucken-0.0.1/src/gucken/player/android.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,13 @@
+from dataclasses import dataclass
+
 from .common import Player
 
 
+@dataclass
 class AndroidChoosePlayer(Player):
     supports_headers = False
 
     def play(
             self,
             url: str,
             title: str,
@@ -23,14 +26,15 @@
             url,
             "-c",
             "android.intent.category.BROWSABLE"
         ]
 
 
 # http://mpv-android.github.io/mpv-android/intent.html
+@dataclass
 class AndroidMPVPlayer(Player):
     supports_headers = False
 
     def play(
             self,
             url: str,
             title: str,
@@ -49,14 +53,15 @@
             url,
             "-n",
             "is.xyz.mpv/.MPVActivity"
         ]
 
 
 # https://wiki.videolan.org/Android_Player_Intents/
+@dataclass
 class AndroidVLCPlayer(Player):
     supports_headers = False
 
     def play(
             self,
             url: str,
             title: str,
```

### Comparing `gucken-0.0.0/src/gucken/player/common.py` & `gucken-0.0.1/src/gucken/player/common.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 def dict_to_string(dictionary):
     return ','.join([f"{key}: {value}" for key, value in dictionary.items()])
 
 
 @dataclass
 class Player:
+    executable: str = None
     supports_headers: bool = False
 
     @abstractmethod
     def play(
             self,
             url: str,
             title: str,
```

### Comparing `gucken-0.0.0/src/gucken/player/mpv.py` & `gucken-0.0.1/src/gucken/player/ffplay.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,28 @@
+from dataclasses import dataclass
+
 from .common import Player, dict_to_string
 
 
-class MPVPlayer(Player):
+@dataclass
+class FFPlayPlayer(Player):
+    executable = "ffplay"
     supports_headers = True
 
     def play(
             self,
             url: str,
             title: str,
             full_screen: bool,
             headers: dict[str, str] = None,
             override_executable: str = None
     ) -> list[str]:
         args = [
-            override_executable or "mpv",
+            override_executable or self.executable,
             url
         ]
-        if full_screen:
-            args.append("--fullscreen")
         if title:
-            args.append(f"--force-media-title={title}")
+            args.append("-window_title")
+            args.append(title)
         if headers:
-            args.append(f"--http-header-fields={dict_to_string(headers)}")
+            args.append(f"-headers={dict_to_string(headers)}")
         return args
```

### Comparing `gucken-0.0.0/src/gucken/player/vlc.py` & `gucken-0.0.1/src/gucken/player/vlc.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,26 @@
+from dataclasses import dataclass
+
 from .common import Player
 
 
+@dataclass
 class VLCPlayer(Player):
+    executable = "vlc"
+
     def play(
             self,
             url: str,
             title: str,
             full_screen: bool,
             headers: dict[str, str] = None,
             override_executable: str = None
     ) -> list[str]:
         args = [
-            override_executable or "vlc",
+            override_executable or self.executable,
             url,
             "--no-video-title-show",
             "--play-and-exit",
         ]
         if full_screen:
             args.append("--fullscreen")
         if title:
```

### Comparing `gucken-0.0.0/src/gucken/provider/aniworld.py` & `gucken-0.0.1/src/gucken/provider/aniworld.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,20 @@
 from asyncio import gather
 from dataclasses import dataclass
-from typing import Union
 from html import unescape
+from typing import Union
 
-from httpx import AsyncClient
 from bs4 import BeautifulSoup
+from httpx import AsyncClient
 
-from .common import (
-    Provider,
-    SearchResult,
-    Series,
-    Episode,
-    Hoster,
-    Language
-)
 from ..hoster.doodstream import DoodstreamHoster
 from ..hoster.streamtape import StreamtapeHoster
 from ..hoster.veo import VOEHoster
 from ..hoster.vidoza import VidozaHoster
+from .common import Episode, Hoster, Language, Provider, SearchResult, Series
 
 
 def data_lang_key_to_lang(data_lang_key: str) -> Language:
     if data_lang_key == "1":
         return Language.DE
     if data_lang_key == "2":
         return Language.JP_ENSUB
@@ -99,26 +92,26 @@
             f"**Tags**: {', '.join(self.tags)}"
         )
 
 
 @dataclass
 class AniWorldSearchResult(SearchResult):
     link: str = None
-    cover: str = None
     production_year: str = None
     host: str = None
 
     async def get_series(self) -> AniWorldSeries:
         return await AniWorldProvider.get_series(self)
 
     @property
     def url(self) -> str:
         return f"https://{self.host}/anime/stream/{self.link}"
 
 
+@dataclass
 class AniWorldProvider(Provider):
     host = "aniworld.to"
 
     @staticmethod
     async def search(keyword: str) -> Union[list[AniWorldSearchResult], None]:
         if keyword.strip() == "":
             return None
@@ -127,15 +120,15 @@
             results = response.json()
             search_results = []
             for series in results:
                 search_results.append(AniWorldSearchResult(
                     name=unescape(series.get("name")),
                     link=series.get("link"),
                     description=unescape(series.get("description")),
-                    cover=series.get("cover"),
+                    cover=f"https://{AniWorldProvider.host}{series.get('cover')}",
                     production_year=series.get("productionYear"),
                     host=AniWorldProvider.host
                 ))
             return search_results
 
     @staticmethod
     async def get_series(search_result: AniWorldSearchResult) -> AniWorldSeries:
```

### Comparing `gucken-0.0.0/src/gucken/provider/common.py` & `gucken-0.0.1/src/gucken/provider/common.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-from abc import abstractmethod, ABC
+from abc import ABC, abstractmethod
 from dataclasses import dataclass
 from enum import Enum
 from typing import Union
+
 from ..hoster.common import Hoster
 
 
 class Language(Enum):
     DE = "Deutsch"
     JP_DESUB = "Japanisch mit deutschen untertitel"
     JP_ENSUB = "Japanisch mit englischen untertitel"
@@ -45,14 +46,15 @@
         raise NotImplementedError
 
 
 @dataclass
 class SearchResult:
     name: str
     description: str = None
+    cover: str = None
 
     @abstractmethod
     async def get_series(self) -> Series:
         raise NotImplementedError
 
     @property
     @abstractmethod
```

### Comparing `gucken-0.0.0/src/gucken/provider/serienstream.py` & `gucken-0.0.1/src/gucken/provider/serienstream.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,20 @@
 from asyncio import gather
 from dataclasses import dataclass
-from typing import Union
 from html import unescape
+from typing import Union
 
-from httpx import AsyncClient
 from bs4 import BeautifulSoup
+from httpx import AsyncClient
 
-from .common import (
-    Provider,
-    SearchResult,
-    Series,
-    Episode,
-    Hoster,
-    Language
-)
 from ..hoster.doodstream import DoodstreamHoster
 from ..hoster.streamtape import StreamtapeHoster
 from ..hoster.veo import VOEHoster
 from ..hoster.vidoza import VidozaHoster
+from .common import Episode, Hoster, Language, Provider, SearchResult, Series
 
 
 def data_lang_key_to_lang(data_lang_key: str) -> Language:
     if data_lang_key == "1":
         return Language.DE
     if data_lang_key == "2":
         return Language.JP_ENSUB
@@ -99,26 +92,26 @@
             f"**Tags**: {', '.join(self.tags)}"
         )
 
 
 @dataclass
 class SerienStreamSearchResult(SearchResult):
     link: str = None
-    cover: str = None
     production_year: str = None
     host: str = None
 
     async def get_series(self) -> SerienStreamSeries:
         return await SerienStreamProvider.get_series(self)
 
     @property
     def url(self) -> str:
         return f"https://{self.host}/serie/stream/{self.link}"
 
 
+@dataclass
 class SerienStreamProvider(Provider):
     host = "186.2.175.5"
 
     @staticmethod
     async def search(keyword: str) -> Union[list[SerienStreamSearchResult], None]:
         if keyword.strip() == "":
             return None
@@ -127,15 +120,15 @@
             results = response.json()
             search_results = []
             for series in results:
                 search_results.append(SerienStreamSearchResult(
                     name=unescape(series.get("name")),
                     link=series.get("link"),
                     description=unescape(series.get("description")),
-                    cover=series.get("cover"),
+                    cover=f"https://s.to{series.get('cover')}",
                     production_year=series.get("productionYear"),
                     host=SerienStreamProvider.host
                 ))
             return search_results
 
     @staticmethod
     async def get_series(search_result: SerienStreamSearchResult) -> SerienStreamSeries:
```

### Comparing `gucken-0.0.0/src/gucken/tracker/anilist.py` & `gucken-0.0.1/src/gucken/tracker/anilist.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from httpx import AsyncClient
 
-
 SEARCH_QUERY = """
 query ($id: Int, $page: Int, $perPage: Int, $search: String) {
   Page (page: $page, perPage: $perPage) {
     pageInfo {
       total
       currentPage
       lastPage
```

### Comparing `gucken-0.0.0/LICENSE.txt` & `gucken-0.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gucken-0.0.0/README.md` & `gucken-0.0.1/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,63 +1,72 @@
 # Gucken
 
-Anime Terminal User Interface
-
----
-
 ## Description
 
-AniTUI is a Terminal User Interface which allows you to browse and watch your favorite anime's with style. 
+Gucken is a Terminal User Interface which allows you to browse and watch your favorite anime's with style. 
 
 ## Usage
 
 Search
 ![Search](.README/Search.png)
 and watch
 ![Watch](.README/Watch.png)
 
 ## Installation
 
-soon tm, you can do it
+### Windows
+
+Install [Python] and if you are **on Windows 10** [Windows Terminal] for a better experience.
+
+```
+pip install gucken
+gucken
+```
 
 ### Linux
 
-You can do it :D
+Install [Python] and then
+
+```
+pip install gucken
+gucken
+```
 
 ### Android
 
 Install [Termux](https://termux.dev/en/) and run:
 
-yt-dlp: https://github.com/termux/termux-packages/issues/20039
-
 ```
 pkg update -y
 pkg upgrade -y
-pkg install python ffmpeg git -y
-git clone https://github.com/Commandcracker/AniTUI
-cd AniTUI/src
-python -m anitui
+pkg install python ffmpeg -y
+pip install gucken
+gucken
 ```
 
-Optional setup storage for downloads
+#### Optional
+
+Setup storage for downloads.
+
 ```
 termux-setup-storage
 ```
 
 ## Features
 
+- [x] Update checker
 - [x] Browsing
   - [x] Descriptions
 - [x] Watching
   - [x] Automatically start next episode
-  - [ ] Discord Presence
+  - [x] Discord Presence **WIP**
   - [MPV] only
-    - [X] [ani-skip](https://github.com/synacktraa/ani-skip) support (very WIP)
+    - [X] [ani-skip](https://github.com/synacktraa/ani-skip) support **Very WIP**
     - [x] [Syncplay](https://github.com/Syncplay/syncplay) support
-    - [ ] Remember watch time (WIP)
+    - [ ] Remember watch time **WIP**
     - [ ] Remember completed Episodes (and series)
   - [ ] Tracker support
     - [ ] [MyAnimeList](https://myanimelist.net/)
     - [ ] [AniList](https://anilist.co/)
     - [ ] [AniWorld.to] & [SerienStream.to]
 - [ ] Downloading
   - [ ] Watch from download
@@ -82,27 +91,28 @@
 ## Player
 
 List of supported video players
 
 - [x] [MPV] (most features, recommended)
 - [x] [VLC]
 - [x] [ffplay](https://www.ffmpeg.org/ffplay.html)
+- [ ] Custom
 - Windows
-  - [ ] [mpv.net](https://github.com/mpvnet-player/mpv.net)
+  - [x] [mpv.net](https://github.com/mpvnet-player/mpv.net)
   - [x] wmplayer.exe (fallback on Windows)
 - Android
   - [x] [mpv-android](https://github.com/mpv-android/mpv-android)
   - [x] [VLC]
   - [x] Choose
 - Linux (Flatpack)
-  - [ ] [MPV](https://flathub.org/apps/io.mpv.Mpv)
-  - [ ] [VLC](https://flathub.org/apps/org.videolan.VLC)
-  - [ ] [Celluloid](https://flathub.org/apps/io.github.celluloid_player.Celluloid)
+  - [x] [MPV](https://flathub.org/apps/io.mpv.Mpv)
+  - [x] [VLC](https://flathub.org/apps/org.videolan.VLC)
+  - [x] [Celluloid](https://flathub.org/apps/io.github.celluloid_player.Celluloid)
 - Linux
-  - [ ] [Celluloid](https://celluloid-player.github.io/)
+  - [x] [Celluloid](https://celluloid-player.github.io/)
 - MacOS
   - [ ] [IINA](https://iina.io/)
 
 ## Todo
 
 - [ ] Up-scaling (after download)
   - [ ] [video2x](https://github.com/k4yt3x/video2x)
@@ -128,35 +138,42 @@
   Note:
   AniWorld.to need Cloudflare captcha and JS challange
   SerienStream.to can be bypassed by using diract ip
   
   Cloudflare captcha and JS challange can be solved by using something like
   selenium or playwright
   ```
-- [ ] [MPV] screen selection
-- [ ] Settings (Save)
-- [ ] [MPV] custom args
-- [ ] Option for full screen
-- [ ] Theme (Dark/Light and Colors)
+- [ ] [MPV] Screen selection
+- [ ] Save settings
+- [ ] Custom player args
+- [ ] Custom player
+- [ ] Colors themes
 - [ ] Installation helper
   - [ ] [MPV]
     - [ ] [Anime4k]
-  - [ ] python
-    - [ ] requirements (venv)
   - [ ] [VLC]
-  - [ ] git (for automatic updating)
-- [ ] CLI flags
-- [ ] Testing (Windows, Linux)
-- [ ] Windows, Linux Support
+- [ ] Create shortcut Windows & Linux
+- [ ] CLI args
+- [ ] CI Testing (Windows, Linux)
+- [ ] CD pip
 - [ ] [Anime4k] options
-- [ ] Modular (Custom extractors, API)
+- [ ] Modular (Custom extractors/players, API)
 - [ ] Proper error handling
 - [ ] Logging and Crash reports
 - [ ] Pre-fetching
 - [ ] improve [ani-skip](https://github.com/synacktraa/ani-skip) support
 - [ ] Use something like opencv to time match a sub from aniworld with a high quality video form another site.
+- [ ] Image preview
+- [ ] Blacklist detection & bypass
+- [ ] Syncplay on Android
+- [ ] Mac support
+- [ ] IOS support
+- [ ] Option to disable update checker
+- [ ] Update checker option to perform update
 
 [Anime4k]: https://github.com/bloc97/Anime4K
 [MPV]: https://mpv.io/
 [VLC]: https://www.videolan.org/vlc/
 [AniWorld.to]: https://aniworld.to
 [SerienStream.to]: https://186.2.175.5
+[Python]: https://www.python.org/downloads/
+[Windows Terminal]: https://apps.microsoft.com/detail/9n0dx20hk701
```

### Comparing `gucken-0.0.0/pyproject.toml` & `gucken-0.0.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,61 +1,60 @@
 [project]
 name = "gucken"
-version = "0.0.0"
+dynamic = ["version"]
+description = "Gucken is a Terminal User Interface which allows you to browse and watch your favorite anime's with style."
 authors = [{name="Commandcracker"}]
 maintainers = [{name="Commandcracker"}]
 license = {file = "LICENSE.txt"}
 readme = "README.md"
 dependencies = [
   "textual>=0.58.1",
   "beautifulsoup4>=4.12.3",
   "httpx>=0.27.0",
   "pypresence>=4.3.0",
-  #"yt-dlp>=2024.4.9"
-  #"httpx[socks]"
+  #"yt-dlp>=2024.4.9",
+  #"mpv>=1.0.6",
+  #"httpx[socks]",
 ]
 keywords = [
   "gucken",
   "anime",
   "serien",
   "series",
   "tui"
 ]
 classifiers = [
   "Development Status :: 2 - Pre-Alpha",
   "Environment :: Console",
-
   "Intended Audience :: End Users/Desktop",
   "Intended Audience :: Developers",
-
   "License :: OSI Approved :: MIT License",
-
   "Natural Language :: English",
   "Natural Language :: German",
-
   "Programming Language :: Lua",
   "Programming Language :: Python",
-
   "Topic :: Games/Entertainment",
   "Topic :: Multimedia",
   "Topic :: Multimedia :: Sound/Audio",
   "Topic :: Multimedia :: Video",
-
   "Operating System :: Microsoft :: Windows",
   "Operating System :: POSIX :: Linux",
   "Operating System :: Android",
-  #"Operating System :: MacOS"
-  #"Operating System :: iOS"
+  #"Operating System :: MacOS",
+  #"Operating System :: iOS",
 ]
 
 [project.urls]
 Repository = "https://github.com/Commandcracker/gucken"
 
 [project.scripts]
 gucken = "gucken.gucken:main"
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [tool.hatch.build.targets.sdist]
 include = ["src/gucken/**", ]
+
+[tool.hatch.version]
+path = "src/gucken/__init__.py"
```

### Comparing `gucken-0.0.0/PKG-INFO` & `gucken-0.0.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 Metadata-Version: 2.3
 Name: gucken
-Version: 0.0.0
+Version: 0.0.1
+Summary: Gucken is a Terminal User Interface which allows you to browse and watch your favorite anime's with style.
 Project-URL: Repository, https://github.com/Commandcracker/gucken
 Author: Commandcracker
 Maintainer: Commandcracker
 License: MIT License
         
         Copyright (c) 2024 Commandcracker
         
@@ -47,68 +48,77 @@
 Requires-Dist: httpx>=0.27.0
 Requires-Dist: pypresence>=4.3.0
 Requires-Dist: textual>=0.58.1
 Description-Content-Type: text/markdown
 
 # Gucken
 
-Anime Terminal User Interface
-
----
-
 ## Description
 
-AniTUI is a Terminal User Interface which allows you to browse and watch your favorite anime's with style. 
+Gucken is a Terminal User Interface which allows you to browse and watch your favorite anime's with style. 
 
 ## Usage
 
 Search
 ![Search](.README/Search.png)
 and watch
 ![Watch](.README/Watch.png)
 
 ## Installation
 
-soon tm, you can do it
+### Windows
+
+Install [Python] and if you are **on Windows 10** [Windows Terminal] for a better experience.
+
+```
+pip install gucken
+gucken
+```
 
 ### Linux
 
-You can do it :D
+Install [Python] and then
+
+```
+pip install gucken
+gucken
+```
 
 ### Android
 
 Install [Termux](https://termux.dev/en/) and run:
 
-yt-dlp: https://github.com/termux/termux-packages/issues/20039
-
 ```
 pkg update -y
 pkg upgrade -y
-pkg install python ffmpeg git -y
-git clone https://github.com/Commandcracker/AniTUI
-cd AniTUI/src
-python -m anitui
+pkg install python ffmpeg -y
+pip install gucken
+gucken
 ```
 
-Optional setup storage for downloads
+#### Optional
+
+Setup storage for downloads.
+
 ```
 termux-setup-storage
 ```
 
 ## Features
 
+- [x] Update checker
 - [x] Browsing
   - [x] Descriptions
 - [x] Watching
   - [x] Automatically start next episode
-  - [ ] Discord Presence
+  - [x] Discord Presence **WIP**
   - [MPV] only
-    - [X] [ani-skip](https://github.com/synacktraa/ani-skip) support (very WIP)
+    - [X] [ani-skip](https://github.com/synacktraa/ani-skip) support **Very WIP**
     - [x] [Syncplay](https://github.com/Syncplay/syncplay) support
-    - [ ] Remember watch time (WIP)
+    - [ ] Remember watch time **WIP**
     - [ ] Remember completed Episodes (and series)
   - [ ] Tracker support
     - [ ] [MyAnimeList](https://myanimelist.net/)
     - [ ] [AniList](https://anilist.co/)
     - [ ] [AniWorld.to] & [SerienStream.to]
 - [ ] Downloading
   - [ ] Watch from download
@@ -133,27 +143,28 @@
 ## Player
 
 List of supported video players
 
 - [x] [MPV] (most features, recommended)
 - [x] [VLC]
 - [x] [ffplay](https://www.ffmpeg.org/ffplay.html)
+- [ ] Custom
 - Windows
-  - [ ] [mpv.net](https://github.com/mpvnet-player/mpv.net)
+  - [x] [mpv.net](https://github.com/mpvnet-player/mpv.net)
   - [x] wmplayer.exe (fallback on Windows)
 - Android
   - [x] [mpv-android](https://github.com/mpv-android/mpv-android)
   - [x] [VLC]
   - [x] Choose
 - Linux (Flatpack)
-  - [ ] [MPV](https://flathub.org/apps/io.mpv.Mpv)
-  - [ ] [VLC](https://flathub.org/apps/org.videolan.VLC)
-  - [ ] [Celluloid](https://flathub.org/apps/io.github.celluloid_player.Celluloid)
+  - [x] [MPV](https://flathub.org/apps/io.mpv.Mpv)
+  - [x] [VLC](https://flathub.org/apps/org.videolan.VLC)
+  - [x] [Celluloid](https://flathub.org/apps/io.github.celluloid_player.Celluloid)
 - Linux
-  - [ ] [Celluloid](https://celluloid-player.github.io/)
+  - [x] [Celluloid](https://celluloid-player.github.io/)
 - MacOS
   - [ ] [IINA](https://iina.io/)
 
 ## Todo
 
 - [ ] Up-scaling (after download)
   - [ ] [video2x](https://github.com/k4yt3x/video2x)
@@ -179,35 +190,42 @@
   Note:
   AniWorld.to need Cloudflare captcha and JS challange
   SerienStream.to can be bypassed by using diract ip
   
   Cloudflare captcha and JS challange can be solved by using something like
   selenium or playwright
   ```
-- [ ] [MPV] screen selection
-- [ ] Settings (Save)
-- [ ] [MPV] custom args
-- [ ] Option for full screen
-- [ ] Theme (Dark/Light and Colors)
+- [ ] [MPV] Screen selection
+- [ ] Save settings
+- [ ] Custom player args
+- [ ] Custom player
+- [ ] Colors themes
 - [ ] Installation helper
   - [ ] [MPV]
     - [ ] [Anime4k]
-  - [ ] python
-    - [ ] requirements (venv)
   - [ ] [VLC]
-  - [ ] git (for automatic updating)
-- [ ] CLI flags
-- [ ] Testing (Windows, Linux)
-- [ ] Windows, Linux Support
+- [ ] Create shortcut Windows & Linux
+- [ ] CLI args
+- [ ] CI Testing (Windows, Linux)
+- [ ] CD pip
 - [ ] [Anime4k] options
-- [ ] Modular (Custom extractors, API)
+- [ ] Modular (Custom extractors/players, API)
 - [ ] Proper error handling
 - [ ] Logging and Crash reports
 - [ ] Pre-fetching
 - [ ] improve [ani-skip](https://github.com/synacktraa/ani-skip) support
 - [ ] Use something like opencv to time match a sub from aniworld with a high quality video form another site.
+- [ ] Image preview
+- [ ] Blacklist detection & bypass
+- [ ] Syncplay on Android
+- [ ] Mac support
+- [ ] IOS support
+- [ ] Option to disable update checker
+- [ ] Update checker option to perform update
 
 [Anime4k]: https://github.com/bloc97/Anime4K
 [MPV]: https://mpv.io/
 [VLC]: https://www.videolan.org/vlc/
 [AniWorld.to]: https://aniworld.to
 [SerienStream.to]: https://186.2.175.5
+[Python]: https://www.python.org/downloads/
+[Windows Terminal]: https://apps.microsoft.com/detail/9n0dx20hk701
```

