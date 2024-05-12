# Comparing `tmp/tcrutils-12.0.154.tar.gz` & `tmp/tcrutils-12.0.156.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tcrutils-12.0.154.tar", max compression
+gzip compressed data, was "tcrutils-12.0.156.tar", max compression
```

## Comparing `tcrutils-12.0.154.tar` & `tcrutils-12.0.156.tar`

### file list

```diff
@@ -1,60 +1,68 @@
--rw-r--r--   0        0        0    35823 2023-11-04 23:11:02.596565 tcrutils-12.0.154/LICENSE
--rw-r--r--   0        0        0      586 2024-04-30 10:29:01.501066 tcrutils-12.0.154/pyproject.toml
--rw-r--r--   0        0        0      527 2024-04-30 10:28:43.628294 tcrutils-12.0.154/README.md
--rw-r--r--   0        0        0     4499 2024-04-30 10:23:15.604483 tcrutils-12.0.154/tcrutils/__init__.py
--rw-r--r--   0        0        0      209 2024-04-30 10:29:02.299896 tcrutils-12.0.154/tcrutils/_version.py
--rw-r--r--   0        0        0      778 2024-04-07 14:45:13.688614 tcrutils-12.0.154/tcrutils/discord/__init__.py
--rw-r--r--   0        0        0       81 2024-04-07 12:08:11.885327 tcrutils-12.0.154/tcrutils/discord/tcrd_alias.py
--rw-r--r--   0        0        0       98 2024-01-19 16:02:12.088184 tcrutils-12.0.154/tcrutils/discord/tcrd_constants.py
--rw-r--r--   0        0        0     2244 2024-03-19 14:26:22.018806 tcrutils-12.0.154/tcrutils/discord/tcrd_embeds.py
--rw-r--r--   0        0        0      378 2024-02-19 21:50:08.127201 tcrutils-12.0.154/tcrutils/discord/tcrd_limits.py
--rw-r--r--   0        0        0     4302 2024-02-23 20:13:37.429288 tcrutils-12.0.154/tcrutils/discord/tcrd_permissions.py
--rw-r--r--   0        0        0      518 2024-02-23 20:13:37.429288 tcrutils-12.0.154/tcrutils/discord/tcrd_snowflake.py
--rw-r--r--   0        0        0     5788 2024-02-23 20:51:35.076170 tcrutils-12.0.154/tcrutils/discord/tcrd_string.py
--rw-r--r--   0        0        0     2156 2024-02-23 20:13:37.428288 tcrutils-12.0.154/tcrutils/discord/tcrd_types.py
--rw-r--r--   0        0        0      140 2024-04-28 17:11:30.234263 tcrutils-12.0.154/tcrutils/imgui/__init__.py
--rw-r--r--   0        0        0      768 2024-04-26 20:35:07.575035 tcrutils-12.0.154/tcrutils/imgui/tcri_dependencies.py
--rw-r--r--   0        0        0     3402 2024-04-27 23:44:35.840582 tcrutils-12.0.154/tcrutils/imgui/tcri_handler.py
--rw-r--r--   0        0        0   141566 2024-04-27 23:44:35.849274 tcrutils-12.0.154/tcrutils/imgui/types/tcri_types_imgui.py
--rw-r--r--   0        0        0      125 2023-11-06 18:52:45.144847 tcrutils-12.0.154/tcrutils/src/pyproject.toml
--rw-r--r--   0        0        0      456 2024-04-30 10:22:34.407852 tcrutils-12.0.154/tcrutils/src/tcr_b64.py
--rw-r--r--   0        0        0     1519 2024-03-19 14:20:08.937583 tcrutils-12.0.154/tcrutils/src/tcr_class.py
--rw-r--r--   0        0        0      550 2024-03-19 14:19:35.424053 tcrutils-12.0.154/tcrutils/src/tcr_classfuncs.py
--rw-r--r--   0        0        0     2270 2024-04-26 17:59:16.788049 tcrutils-12.0.154/tcrutils/src/tcr_compare.py
--rw-r--r--   0        0        0     4962 2024-04-14 13:12:08.350757 tcrutils-12.0.154/tcrutils/src/tcr_console.py
--rw-r--r--   0        0        0      347 2023-12-23 23:11:59.731531 tcrutils-12.0.154/tcrutils/src/tcr_constants.py
--rw-r--r--   0        0        0     5514 2024-04-26 17:59:16.787050 tcrutils-12.0.154/tcrutils/src/tcr_decorator.py
--rw-r--r--   0        0        0     4881 2024-04-26 20:24:04.669671 tcrutils-12.0.154/tcrutils/src/tcr_dev.py
--rw-r--r--   0        0        0     5710 2024-03-19 17:47:20.530561 tcrutils-12.0.154/tcrutils/src/tcr_dict.py
--rw-r--r--   0        0        0      245 2024-04-07 14:45:13.688614 tcrutils-12.0.154/tcrutils/src/tcr_dir.py
--rw-r--r--   0        0        0      987 2024-02-17 18:48:50.338606 tcrutils-12.0.154/tcrutils/src/tcr_error.py
--rw-r--r--   0        0        0     3290 2024-04-11 21:25:26.870189 tcrutils-12.0.154/tcrutils/src/tcr_execute.py
--rw-r--r--   0        0        0      451 2024-04-28 17:18:28.266885 tcrutils-12.0.154/tcrutils/src/tcr_execute_parsed.py
--rw-r--r--   0        0        0     1006 2024-03-08 15:03:30.998287 tcrutils-12.0.154/tcrutils/src/tcr_extract_error.py
--rw-r--r--   0        0        0       81 2023-12-23 23:01:58.550444 tcrutils-12.0.154/tcrutils/src/tcr_F.py
--rw-r--r--   0        0        0     1093 2023-11-06 18:49:03.607042 tcrutils-12.0.154/tcrutils/src/tcr_getch.py
--rw-r--r--   0        0        0     4301 2024-03-19 17:47:20.530561 tcrutils-12.0.154/tcrutils/src/tcr_inject.py
--rw-r--r--   0        0        0      950 2024-01-29 17:47:31.333032 tcrutils-12.0.154/tcrutils/src/tcr_input.py
--rw-r--r--   0        0        0     2241 2024-04-11 22:00:21.527336 tcrutils-12.0.154/tcrutils/src/tcr_inspect.py
--rw-r--r--   0        0        0     1080 2024-04-11 22:06:10.025542 tcrutils-12.0.154/tcrutils/src/tcr_int.py
--rw-r--r--   0        0        0     7697 2024-02-23 20:13:37.423287 tcrutils-12.0.154/tcrutils/src/tcr_iterable.py
--rw-r--r--   0        0        0     2253 2024-04-26 19:06:23.600151 tcrutils-12.0.154/tcrutils/src/tcr_joke.py
--rw-r--r--   0        0        0     2748 2024-02-15 12:39:41.609862 tcrutils-12.0.154/tcrutils/src/tcr_language.py
--rw-r--r--   0        0        0     1155 2024-03-09 23:40:24.608413 tcrutils-12.0.154/tcrutils/src/tcr_markdown.py
--rw-r--r--   0        0        0     1299 2024-02-23 20:13:37.423287 tcrutils-12.0.154/tcrutils/src/tcr_misspellings.py
--rw-r--r--   0        0        0     1409 2024-03-19 17:47:20.529553 tcrutils-12.0.154/tcrutils/src/tcr_null.py
--rw-r--r--   0        0        0      298 2024-02-23 23:16:27.228751 tcrutils-12.0.154/tcrutils/src/tcr_other.py
--rw-r--r--   0        0        0     7588 2024-02-23 20:13:37.420287 tcrutils-12.0.154/tcrutils/src/tcr_overload.py
--rw-r--r--   0        0        0     3127 2024-02-23 20:13:37.419287 tcrutils-12.0.154/tcrutils/src/tcr_path.py
--rw-r--r--   0        0        0    29286 2024-04-19 22:20:25.582375 tcrutils-12.0.154/tcrutils/src/tcr_print.py
--rw-r--r--   0        0        0     1361 2024-02-10 21:19:35.084757 tcrutils-12.0.154/tcrutils/src/tcr_regex.py
--rw-r--r--   0        0        0      743 2023-11-07 15:44:27.527859 tcrutils-12.0.154/tcrutils/src/tcr_run.py
--rw-r--r--   0        0        0     3867 2024-03-19 17:47:20.540561 tcrutils-12.0.154/tcrutils/src/tcr_sdb.py
--rw-r--r--   0        0        0     4083 2024-04-12 20:31:09.874612 tcrutils-12.0.154/tcrutils/src/tcr_string.py
--rw-r--r--   0        0        0     1152 2024-03-19 17:47:20.531561 tcrutils-12.0.154/tcrutils/src/tcr_terminal.py
--rw-r--r--   0        0        0     5038 2024-03-20 15:11:07.733764 tcrutils-12.0.154/tcrutils/src/tcr_test.py
--rw-r--r--   0        0        0    16373 2024-02-23 20:13:37.427288 tcrutils-12.0.154/tcrutils/src/tcr_timestr.py
--rw-r--r--   0        0        0      311 2024-04-07 14:45:13.688614 tcrutils-12.0.154/tcrutils/src/tcr_types.py
--rw-r--r--   0        0        0     1819 2024-02-17 18:23:07.659452 tcrutils-12.0.154/tcrutils/src/tcr_uptime.py
--rw-r--r--   0        0        0     1089 2024-01-13 22:57:18.979846 tcrutils-12.0.154/tcrutils/src/tcr_void.py
--rw-r--r--   0        0        0     1204 1970-01-01 00:00:00.000000 tcrutils-12.0.154/PKG-INFO
+-rw-r--r--   0        0        0    35823 2023-11-04 23:11:02.596565 tcrutils-12.0.156/LICENSE
+-rw-r--r--   0        0        0      586 2024-05-12 19:39:08.751635 tcrutils-12.0.156/pyproject.toml
+-rw-r--r--   0        0        0     1942 2024-05-12 19:30:06.391823 tcrutils-12.0.156/README.md
+-rw-r--r--   0        0        0     4819 2024-05-11 21:17:23.617418 tcrutils-12.0.156/tcrutils/__init__.py
+-rw-r--r--   0        0        0      209 2024-05-12 19:39:11.491581 tcrutils-12.0.156/tcrutils/_version.py
+-rw-r--r--   0        0        0      778 2024-04-07 14:45:13.688614 tcrutils-12.0.156/tcrutils/discord/__init__.py
+-rw-r--r--   0        0        0       81 2024-04-07 12:08:11.885327 tcrutils-12.0.156/tcrutils/discord/tcrd_alias.py
+-rw-r--r--   0        0        0       98 2024-01-19 16:02:12.088184 tcrutils-12.0.156/tcrutils/discord/tcrd_constants.py
+-rw-r--r--   0        0        0     2244 2024-03-19 14:26:22.018806 tcrutils-12.0.156/tcrutils/discord/tcrd_embeds.py
+-rw-r--r--   0        0        0      378 2024-02-19 21:50:08.127201 tcrutils-12.0.156/tcrutils/discord/tcrd_limits.py
+-rw-r--r--   0        0        0     4302 2024-02-23 20:13:37.429288 tcrutils-12.0.156/tcrutils/discord/tcrd_permissions.py
+-rw-r--r--   0        0        0      518 2024-02-23 20:13:37.429288 tcrutils-12.0.156/tcrutils/discord/tcrd_snowflake.py
+-rw-r--r--   0        0        0     5788 2024-02-23 20:51:35.076170 tcrutils-12.0.156/tcrutils/discord/tcrd_string.py
+-rw-r--r--   0        0        0     2156 2024-02-23 20:13:37.428288 tcrutils-12.0.156/tcrutils/discord/tcrd_types.py
+-rw-r--r--   0        0        0      414 2024-05-07 17:26:58.759172 tcrutils-12.0.156/tcrutils/dr/__init__.py
+-rw-r--r--   0        0        0     8244 2024-05-11 19:05:09.032438 tcrutils-12.0.156/tcrutils/dr/core.py
+-rw-r--r--   0        0        0     2493 2024-05-07 17:26:58.759172 tcrutils-12.0.156/tcrutils/dr/error.py
+-rw-r--r--   0        0        0     2542 2024-05-12 19:29:17.797028 tcrutils-12.0.156/tcrutils/dr/placeholder_sets.py
+-rw-r--r--   0        0        0       72 2024-05-11 19:56:28.575713 tcrutils-12.0.156/tcrutils/dr/placeholders/__init__.py
+-rw-r--r--   0        0        0     1574 2024-05-11 21:47:23.390141 tcrutils-12.0.156/tcrutils/dr/placeholders/p_discord.py
+-rw-r--r--   0        0        0     4389 2024-05-12 19:28:10.182266 tcrutils-12.0.156/tcrutils/dr/placeholders/p_math.py
+-rw-r--r--   0        0        0     1566 2024-05-12 18:44:29.418679 tcrutils-12.0.156/tcrutils/dr/placeholders/p_text.py
+-rw-r--r--   0        0        0     4537 2024-05-12 18:55:58.211193 tcrutils-12.0.156/tcrutils/dr/util.py
+-rw-r--r--   0        0        0      140 2024-05-02 14:13:55.166736 tcrutils-12.0.156/tcrutils/imgui/__init__.py
+-rw-r--r--   0        0        0      768 2024-04-26 20:35:07.575035 tcrutils-12.0.156/tcrutils/imgui/tcri_dependencies.py
+-rw-r--r--   0        0        0     3386 2024-05-12 19:36:59.859676 tcrutils-12.0.156/tcrutils/imgui/tcri_handler.py
+-rw-r--r--   0        0        0   141566 2024-04-27 23:44:35.849274 tcrutils-12.0.156/tcrutils/imgui/types/tcri_types_imgui.py
+-rw-r--r--   0        0        0      456 2024-04-30 10:22:34.407852 tcrutils-12.0.156/tcrutils/src/tcr_b64.py
+-rw-r--r--   0        0        0     1655 2024-05-02 14:13:55.166736 tcrutils-12.0.156/tcrutils/src/tcr_class.py
+-rw-r--r--   0        0        0      550 2024-03-19 14:19:35.424053 tcrutils-12.0.156/tcrutils/src/tcr_classfuncs.py
+-rw-r--r--   0        0        0     4092 2024-05-11 21:11:34.733039 tcrutils-12.0.156/tcrutils/src/tcr_cloud_imports.py
+-rw-r--r--   0        0        0     2270 2024-04-26 17:59:16.788049 tcrutils-12.0.156/tcrutils/src/tcr_compare.py
+-rw-r--r--   0        0        0     7105 2024-05-11 21:52:09.173816 tcrutils-12.0.156/tcrutils/src/tcr_console.py
+-rw-r--r--   0        0        0      347 2023-12-23 23:11:59.731531 tcrutils-12.0.156/tcrutils/src/tcr_constants.py
+-rw-r--r--   0        0        0     5892 2024-05-02 12:11:41.388680 tcrutils-12.0.156/tcrutils/src/tcr_decorator.py
+-rw-r--r--   0        0        0     4881 2024-05-03 17:37:29.849453 tcrutils-12.0.156/tcrutils/src/tcr_dev.py
+-rw-r--r--   0        0        0     5802 2024-05-02 10:34:38.791291 tcrutils-12.0.156/tcrutils/src/tcr_dict.py
+-rw-r--r--   0        0        0      245 2024-04-07 14:45:13.688614 tcrutils-12.0.156/tcrutils/src/tcr_dir.py
+-rw-r--r--   0        0        0      987 2024-02-17 18:48:50.338606 tcrutils-12.0.156/tcrutils/src/tcr_error.py
+-rw-r--r--   0        0        0     1006 2024-03-08 15:03:30.998287 tcrutils-12.0.156/tcrutils/src/tcr_extract_error.py
+-rw-r--r--   0        0        0       81 2023-12-23 23:01:58.550444 tcrutils-12.0.156/tcrutils/src/tcr_F.py
+-rw-r--r--   0        0        0     1093 2023-11-06 18:49:03.607042 tcrutils-12.0.156/tcrutils/src/tcr_getch.py
+-rw-r--r--   0        0        0     4301 2024-03-19 17:47:20.530561 tcrutils-12.0.156/tcrutils/src/tcr_inject.py
+-rw-r--r--   0        0        0      950 2024-01-29 17:47:31.333032 tcrutils-12.0.156/tcrutils/src/tcr_input.py
+-rw-r--r--   0        0        0     2241 2024-04-11 22:00:21.527336 tcrutils-12.0.156/tcrutils/src/tcr_inspect.py
+-rw-r--r--   0        0        0     1080 2024-04-11 22:06:10.025542 tcrutils-12.0.156/tcrutils/src/tcr_int.py
+-rw-r--r--   0        0        0     7697 2024-02-23 20:13:37.423287 tcrutils-12.0.156/tcrutils/src/tcr_iterable.py
+-rw-r--r--   0        0        0     3264 2024-05-11 21:18:41.050978 tcrutils-12.0.156/tcrutils/src/tcr_joke.py
+-rw-r--r--   0        0        0     2748 2024-02-15 12:39:41.609862 tcrutils-12.0.156/tcrutils/src/tcr_language.py
+-rw-r--r--   0        0        0     1155 2024-03-09 23:40:24.608413 tcrutils-12.0.156/tcrutils/src/tcr_markdown.py
+-rw-r--r--   0        0        0     1299 2024-02-23 20:13:37.423287 tcrutils-12.0.156/tcrutils/src/tcr_misspellings.py
+-rw-r--r--   0        0        0     1409 2024-03-19 17:47:20.529553 tcrutils-12.0.156/tcrutils/src/tcr_null.py
+-rw-r--r--   0        0        0      298 2024-02-23 23:16:27.228751 tcrutils-12.0.156/tcrutils/src/tcr_other.py
+-rw-r--r--   0        0        0     7591 2024-05-11 21:11:55.531404 tcrutils-12.0.156/tcrutils/src/tcr_overload.py
+-rw-r--r--   0        0        0     3127 2024-02-23 20:13:37.419287 tcrutils-12.0.156/tcrutils/src/tcr_path.py
+-rw-r--r--   0        0        0    29286 2024-04-19 22:20:25.582375 tcrutils-12.0.156/tcrutils/src/tcr_print.py
+-rw-r--r--   0        0        0     1361 2024-02-10 21:19:35.084757 tcrutils-12.0.156/tcrutils/src/tcr_regex.py
+-rw-r--r--   0        0        0      743 2023-11-07 15:44:27.527859 tcrutils-12.0.156/tcrutils/src/tcr_run.py
+-rw-r--r--   0        0        0     3888 2024-05-07 16:07:40.280190 tcrutils-12.0.156/tcrutils/src/tcr_sdb.py
+-rw-r--r--   0        0        0     4083 2024-04-12 20:31:09.874612 tcrutils-12.0.156/tcrutils/src/tcr_string.py
+-rw-r--r--   0        0        0     1152 2024-03-19 17:47:20.531561 tcrutils-12.0.156/tcrutils/src/tcr_terminal.py
+-rw-r--r--   0        0        0     6883 2024-05-11 21:36:56.860614 tcrutils-12.0.156/tcrutils/src/tcr_test.py
+-rw-r--r--   0        0        0    16373 2024-02-23 20:13:37.427288 tcrutils-12.0.156/tcrutils/src/tcr_timestr.py
+-rw-r--r--   0        0        0      404 2024-05-11 19:19:25.965833 tcrutils-12.0.156/tcrutils/src/tcr_types.py
+-rw-r--r--   0        0        0     1819 2024-02-17 18:23:07.659452 tcrutils-12.0.156/tcrutils/src/tcr_uptime.py
+-rw-r--r--   0        0        0     1089 2024-01-13 22:57:18.979846 tcrutils-12.0.156/tcrutils/src/tcr_void.py
+-rw-r--r--   0        0        0        0 2024-05-10 19:09:13.830177 tcrutils-12.0.156/tcrutils/str
+-rw-r--r--   0        0        0     2557 1970-01-01 00:00:00.000000 tcrutils-12.0.156/PKG-INFO
```

### Comparing `tcrutils-12.0.154/LICENSE` & `tcrutils-12.0.156/LICENSE`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.154/pyproject.toml` & `tcrutils-12.0.156/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 extend = "C:/CUSTOM_ASSETS/pyproject.toml"
 [tool.ruff.format]
 quote-style = "single"
 indent-style = "space"
 
 [tool.poetry]
 name = "tcrutils"
-version = "12.0.154"
+version = "12.0.156"
 description = "Useful stuff for TCR projects!"
 authors = ["TheCreatorrrr"]
 license = "GPL-3.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.11.0,<3.13"
```

### Comparing `tcrutils-12.0.154/tcrutils/__init__.py` & `tcrutils-12.0.156/tcrutils/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,32 +6,39 @@
 ```
 
 It's also recommended to import stuff directly instead of the entire module
 ```py
 >>> from tcrutils import timestr
 ```
 
-Star-importing is fine, ctrl-click whatever you're hovering on right now to see __all__ if you wish.
+~~Star-importing is fine, ctrl-click whatever you're hovering on right now to see __all__ if you wish.~~
+Update: neeevermind there's just so much stuff you better import directly. __all__ is still maintained tho...
 ```py
 >>> from tcrutils import *
 ```
-Joke functions and other barely useful crap is not included in star imports.
+Joke functions and other barely useful crap are not included in star imports.
 """
 
 from . import discord, src
+from . import dr as dynamic_responses
+from . import dr as execute
 from ._version import __version__
 from .discord.tcrd_embeds import embed, modal
 from .discord.tcrd_limits import DiscordLimits
 from .discord.tcrd_string import get_token
+from .dr import placeholder_set as dr_placeholder_sets
+from .dr import placeholders as dr_placeholders
+from .src import tcr_joke as joke
 from .src import tcr_types as types
 from .src.tcr_b64 import b64
 from .src.tcr_class import Singleton
 from .src.tcr_classfuncs import get_classname, get_name_classname, get_qualname_classname
 from .src.tcr_compare import able, isdunder
-from .src.tcr_console import breakpoint, console
+from .src.tcr_console import breakpoint, console, start_eval_session
+from .src.tcr_console import console as c
 from .src.tcr_constants import *
 from .src.tcr_decorator import autorun, convert, copy_kwargs, instance, test, timeit
 from .src.tcr_dev import generate_function_argument_typehints, generate_type_hinter
 from .src.tcr_dict import DotDict, JSDict, JSDotDict, clean_dunder_dict, dict_zip, merge_dicts
 from .src.tcr_dir import dir2, dir3
 from .src.tcr_error import error  # 'tcrerror' in star imports, either in 'tcr.error'/'tcr.tcrerror'
 from .src.tcr_error import error as tcrerror
@@ -40,15 +47,14 @@
 from .src.tcr_F import F
 from .src.tcr_getch import getch
 from .src.tcr_inject import ErrorCatcher, WarningCatcher
 from .src.tcr_input import insist
 from .src.tcr_inspect import get_file_colon_lineno, get_lineno
 from .src.tcr_int import float2int, hex, recursive_sum
 from .src.tcr_iterable import Or, batched, bogo_sort, cut_at, getattr_queue, getmanyattrs, hasmanyattrs, limited_iterable, shuffled, stalin_sort
-from .src.tcr_joke import CInt, christmas_tree, fizzbuzz, oddeven
 from .src.tcr_language import apostrophe_s, make_plural, nth
 from .src.tcr_markdown import codeblock, uncodeblock
 from .src.tcr_misspellings import asert, trei
 from .src.tcr_null import Null, Undefined, UniqueDefault
 from .src.tcr_other import intbool
 from .src.tcr_overload import Overload, OverloadMeta, overload
 from .src.tcr_path import path
```

### Comparing `tcrutils-12.0.154/tcrutils/discord/__init__.py` & `tcrutils-12.0.156/tcrutils/discord/__init__.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.154/tcrutils/discord/tcrd_embeds.py` & `tcrutils-12.0.156/tcrutils/discord/tcrd_embeds.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.154/tcrutils/discord/tcrd_permissions.py` & `tcrutils-12.0.156/tcrutils/discord/tcrd_permissions.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.154/tcrutils/discord/tcrd_snowflake.py` & `tcrutils-12.0.156/tcrutils/discord/tcrd_snowflake.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.154/tcrutils/discord/tcrd_string.py` & `tcrutils-12.0.156/tcrutils/discord/tcrd_string.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.154/tcrutils/discord/tcrd_types.py` & `tcrutils-12.0.156/tcrutils/discord/tcrd_types.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.154/tcrutils/imgui/tcri_dependencies.py` & `tcrutils-12.0.156/tcrutils/imgui/tcri_dependencies.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.154/tcrutils/imgui/tcri_handler.py` & `tcrutils-12.0.156/tcrutils/imgui/tcri_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import OpenGL.GL as gl
 from imgui.integrations.glfw import GlfwRenderer
 
 from ..src.tcr_console import console as c
 
 
 def ctrlc_grace_exit() -> bool:
-  c.info('Exitting due to Ctrl+C...')
+  print('^C', end='')
   return True  # Exit
 
 
 class ImGuiHandler:
   frame: Callable[[], None]
   """The frame callback."""
   title: str
```

### Comparing `tcrutils-12.0.154/tcrutils/imgui/types/tcri_types_imgui.py` & `tcrutils-12.0.156/tcrutils/imgui/types/tcri_types_imgui.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.154/tcrutils/src/tcr_class.py` & `tcrutils-12.0.156/tcrutils/src/tcr_class.py`

 * *Files 13% similar despite different names*

```diff
@@ -49,7 +49,12 @@
 
   __singleton_instance__ = None
 
   def __new__(cls, *args, **kwargs) -> Self:
     if cls.__singleton_instance__ is None:
       cls.__singleton_instance__ = super().__new__(cls, *args, **kwargs)
     return cls.__singleton_instance__
+
+
+class NoInit:
+  def __init__(self, *args, **kwargs) -> None:
+    raise NotImplementedError('You cannot instiantiate this class')
```

### Comparing `tcrutils-12.0.154/tcrutils/src/tcr_classfuncs.py` & `tcrutils-12.0.156/tcrutils/src/tcr_classfuncs.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.154/tcrutils/src/tcr_compare.py` & `tcrutils-12.0.156/tcrutils/src/tcr_compare.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.154/tcrutils/src/tcr_decorator.py` & `tcrutils-12.0.156/tcrutils/src/tcr_decorator.py`

 * *Files 22% similar despite different names*

```diff
@@ -180,14 +180,28 @@
 
         return wrapper
 
       return decorator
 
   convert = Convert()
 
+  def aconvert(converter: Callable, await_converter: bool = False):
+    def decorator(afunc):
+      @wraps(afunc)
+      async def wrapper(*args, **kwargs):
+        if await_converter:
+          return await converter(await afunc(*args, **kwargs))
+        else:
+          return converter(await afunc(*args, **kwargs))
+
+      return wrapper
+
+    return decorator
+
+
 if True:  # \/ # @printer
 
   def printer(*, printhook: Callable[[str], None] = print, passthrough: bool = True):
     def decorator(func: Callable):
       @wraps(func)
       def wrapper(*args, **kwargs):
         result = func(*args, **kwargs)
```

### Comparing `tcrutils-12.0.154/tcrutils/src/tcr_dev.py` & `tcrutils-12.0.156/tcrutils/src/tcr_dev.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,15 +92,15 @@
     processed_hints_dict[attr_name] = attr_value
 
   if not obj_dir:
     hints.append('...')
 
   # hint types (imports)
 
-  result = f'class {get_name_classname(obj).split('.')[-1]}:\n' + '\n'.join(f'  {x}' for x in hints)
+  result = f'class {get_name_classname(obj).split(".")[-1]}:\n' + '\n'.join(f'  {x}' for x in hints)
 
   if print:
     if callable(print):
       print(result)
     else:
       print_(result)
```

### Comparing `tcrutils-12.0.154/tcrutils/src/tcr_dict.py` & `tcrutils-12.0.156/tcrutils/src/tcr_dict.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,23 +26,28 @@
     msg = 'Mismatched keys'
     raise ValueError(msg)
 
   for k, v in dicks[0].items():
     yield (k, (v, *(dick[k] for dick in dicks[1:])))
 
 
-def merge_dicts(master: Mapping, slave: Mapping, *dicts: Mapping, recursive=True, strict=False) -> Mapping:
+def merge_dicts(master: Mapping = None, slave: Mapping = None, *dicts: Mapping, recursive=True, strict=False) -> Mapping:
   """Merge dictionaries, made to prioritize the `master` dictionary and if key is not found there, then it takes from the `slave` dictionary.
 
   Optionally if `recursive=True`, then if the same key is a dict in both master and slave, merge dicts operation is performed on both of them.\\
   Optionally if `strict=True` it raises `ValueError` if there exists a key that is in master dictionary but not in slave dictionary.\\
   If there are more than 2 arguments passed in the list is reduced from back to front until two elements are left by the process of merge_dicts(master=list[-2], slave=list[-1])
   """
   merged = {}
 
+  if master is None:
+    master = {}
+  if slave is None:
+    slave = {}
+
   dicts = [master, slave, *dicts]
 
   while len(dicts) > 2:
     slave_ = dicts.pop()
     master_ = dicts[-1]
     dicts[-1] = merge_dicts(master_, slave_, recursive=recursive, strict=strict)
```

### Comparing `tcrutils-12.0.154/tcrutils/src/tcr_error.py` & `tcrutils-12.0.156/tcrutils/src/tcr_error.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.154/tcrutils/src/tcr_extract_error.py` & `tcrutils-12.0.156/tcrutils/src/tcr_extract_error.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.154/tcrutils/src/tcr_getch.py` & `tcrutils-12.0.156/tcrutils/src/tcr_getch.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.154/tcrutils/src/tcr_inject.py` & `tcrutils-12.0.156/tcrutils/src/tcr_inject.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.154/tcrutils/src/tcr_input.py` & `tcrutils-12.0.156/tcrutils/src/tcr_input.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.154/tcrutils/src/tcr_inspect.py` & `tcrutils-12.0.156/tcrutils/src/tcr_inspect.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.154/tcrutils/src/tcr_int.py` & `tcrutils-12.0.156/tcrutils/src/tcr_int.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.154/tcrutils/src/tcr_iterable.py` & `tcrutils-12.0.156/tcrutils/src/tcr_iterable.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.154/tcrutils/src/tcr_language.py` & `tcrutils-12.0.156/tcrutils/src/tcr_language.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.154/tcrutils/src/tcr_markdown.py` & `tcrutils-12.0.156/tcrutils/src/tcr_markdown.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.154/tcrutils/src/tcr_misspellings.py` & `tcrutils-12.0.156/tcrutils/src/tcr_misspellings.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.154/tcrutils/src/tcr_null.py` & `tcrutils-12.0.156/tcrutils/src/tcr_null.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.154/tcrutils/src/tcr_overload.py` & `tcrutils-12.0.156/tcrutils/src/tcr_overload.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """### This code was not written by me, however it's licensed with the MIT License which allows for free copy and sublicensing of the licensed material.
 
-This code was written by [James Murphy](https://github.com/jamesmurphy-mc) from [MCoding](https://github.com/mCodingLLC/) ((YouTube)[https://www.youtube.com/@mCoding])
+This code was written by [James Murphy](https://github.com/jamesmurphy-mc) from [MCoding](https://github.com/mCodingLLC/) ([YouTube](https://www.youtube.com/@mCoding))
 
 [Original Source Code](https://github.com/mCodingLLC/VideosSampleCode/blob/master/videos/077_metaclasses_in_python/overloading.py)
 
 Copy of the original license (applies only to this file):
 
-```
+```txt
 MIT License
 
 Copyright (c) 2022 MCODING, LLC
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
```

### Comparing `tcrutils-12.0.154/tcrutils/src/tcr_path.py` & `tcrutils-12.0.156/tcrutils/src/tcr_path.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.154/tcrutils/src/tcr_print.py` & `tcrutils-12.0.156/tcrutils/src/tcr_print.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.154/tcrutils/src/tcr_regex.py` & `tcrutils-12.0.156/tcrutils/src/tcr_regex.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.154/tcrutils/src/tcr_run.py` & `tcrutils-12.0.156/tcrutils/src/tcr_run.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.154/tcrutils/src/tcr_sdb.py` & `tcrutils-12.0.156/tcrutils/src/tcr_sdb.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,25 +44,26 @@
 
 
 class ShelveDB(dict):
   """### Wrapper for shelve module databases.
 
   ```py
   class DB(tcr.ShelveDB):
-  directory = "/VALID/path/to/db/dir/" # Or pathlib.Path object
+    directory = "/VALID/path/to/db/dir/" # Or pathlib.Path object
   ```
 
   Raises:
     - ValueError: provided alnum_id is invalid.
     - RuntimeError: You did not or incorrectly set up the class declaration (shown above).
     - NotADirectoryError: The directory path you provided points to a file, not a directory or nothing.
   """
 
   directory: str | p.Path | None = None
   __directory: p.Path
+  s: shelve.Shelf
 
   def __init__(self, alnum_id: str | int) -> None:
     if isinstance(self.directory, str | p.Path):
       if isinstance(self.directory, str):
         self.directory = p.Path(self.directory)
       self.__directory = self.directory
     else:
```

### Comparing `tcrutils-12.0.154/tcrutils/src/tcr_string.py` & `tcrutils-12.0.156/tcrutils/src/tcr_string.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.154/tcrutils/src/tcr_terminal.py` & `tcrutils-12.0.156/tcrutils/src/tcr_terminal.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.154/tcrutils/src/tcr_timestr.py` & `tcrutils-12.0.156/tcrutils/src/tcr_timestr.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.154/tcrutils/src/tcr_uptime.py` & `tcrutils-12.0.156/tcrutils/src/tcr_uptime.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.154/tcrutils/src/tcr_void.py` & `tcrutils-12.0.156/tcrutils/src/tcr_void.py`

 * *Files identical despite different names*

