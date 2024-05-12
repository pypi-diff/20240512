# Comparing `tmp/drawlib-0.1.3.tar.gz` & `tmp/drawlib-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drawlib-0.1.3.tar", max compression
+gzip compressed data, was "drawlib-0.1.4.tar", max compression
```

## Comparing `drawlib-0.1.3.tar` & `drawlib-0.1.4.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0    11344 2024-04-05 18:42:05.538150 drawlib-0.1.3/LICENSE.txt
--rw-r--r--   0        0        0     2421 2024-05-04 15:36:12.546708 drawlib-0.1.3/README.md
--rw-r--r--   0        0        0       27 2024-03-29 11:45:48.926601 drawlib-0.1.3/drawlib/.pylintrc
--rw-r--r--   0        0        0     1039 2024-05-04 02:00:36.942996 drawlib-0.1.3/drawlib/__init__.py
--rw-r--r--   0        0        0      688 2024-04-06 11:43:47.512263 drawlib-0.1.3/drawlib/__main__.py
--rw-r--r--   0        0        0      777 2024-04-07 14:54:59.159171 drawlib-0.1.3/drawlib/apis.py
--rw-r--r--   0        0        0      407 2024-04-12 07:27:54.821931 drawlib-0.1.3/drawlib/assets/__init__.py
--rw-r--r--   0        0        0      407 2024-05-01 10:34:11.053352 drawlib-0.1.3/drawlib/assets/v0_1/__init__.py
--rw-r--r--   0        0        0      407 2024-04-12 07:28:01.917218 drawlib-0.1.3/drawlib/assets/v0_1/fonticons/__init__.py
--rw-r--r--   0        0        0      407 2024-04-13 15:48:11.439423 drawlib-0.1.3/drawlib/assets/v0_1/fonts/__init__.py
--rw-r--r--   0        0        0     1084 2024-04-07 03:53:05.340986 drawlib-0.1.3/drawlib/v0_1/__init__.py
--rw-r--r--   0        0        0      663 2024-04-06 12:40:11.972278 drawlib-0.1.3/drawlib/v0_1/__main__.py
--rw-r--r--   0        0        0     2437 2024-05-04 13:37:40.227151 drawlib-0.1.3/drawlib/v0_1/apis.py
--rw-r--r--   0        0        0      763 2024-04-06 11:52:52.776827 drawlib-0.1.3/drawlib/v0_1/private/__init__.py
--rw-r--r--   0        0        0     5949 2024-04-27 06:45:13.999149 drawlib-0.1.3/drawlib/v0_1/private/arg_validator.py
--rw-r--r--   0        0        0     6207 2024-04-27 06:44:59.377242 drawlib-0.1.3/drawlib/v0_1/private/command.py
--rw-r--r--   0        0        0      548 2024-04-07 14:22:07.928062 drawlib-0.1.3/drawlib/v0_1/private/core/__init__.py
--rw-r--r--   0        0        0    12776 2024-04-23 00:24:17.718876 drawlib-0.1.3/drawlib/v0_1/private/core/colors.py
--rw-r--r--   0        0        0    13577 2024-04-28 11:41:37.164049 drawlib-0.1.3/drawlib/v0_1/private/core/dimage.py
--rw-r--r--   0        0        0    14228 2024-05-01 15:22:54.625259 drawlib-0.1.3/drawlib/v0_1/private/core/fonts.py
--rw-r--r--   0        0        0    31889 2024-04-30 02:48:39.419245 drawlib-0.1.3/drawlib/v0_1/private/core/model.py
--rw-r--r--   0        0        0     7060 2024-04-27 01:01:21.281062 drawlib-0.1.3/drawlib/v0_1/private/core/model_validator.py
--rw-r--r--   0        0        0    47248 2024-05-04 15:05:41.334797 drawlib-0.1.3/drawlib/v0_1/private/core/theme.py
--rw-r--r--   0        0        0    26316 2024-05-01 14:16:45.894958 drawlib-0.1.3/drawlib/v0_1/private/core/util.py
--rw-r--r--   0        0        0      548 2024-04-27 02:06:25.820510 drawlib-0.1.3/drawlib/v0_1/private/core_canvas/__init__.py
--rw-r--r--   0        0        0    20588 2024-04-29 14:29:33.370357 drawlib-0.1.3/drawlib/v0_1/private/core_canvas/base.py
--rw-r--r--   0        0        0     2328 2024-04-29 17:11:04.449382 drawlib-0.1.3/drawlib/v0_1/private/core_canvas/canvas.py
--rw-r--r--   0        0        0     5197 2024-04-30 01:18:42.581902 drawlib-0.1.3/drawlib/v0_1/private/core_canvas/image.py
--rw-r--r--   0        0        0     7634 2024-04-27 05:11:32.344915 drawlib-0.1.3/drawlib/v0_1/private/core_canvas/line.py
--rw-r--r--   0        0        0     4938 2024-05-04 15:02:18.931580 drawlib-0.1.3/drawlib/v0_1/private/core_canvas/original_arrow.py
--rw-r--r--   0        0        0    19394 2024-05-04 15:03:47.555194 drawlib-0.1.3/drawlib/v0_1/private/core_canvas/original_polygon.py
--rw-r--r--   0        0        0    18918 2024-05-04 15:01:29.902781 drawlib-0.1.3/drawlib/v0_1/private/core_canvas/patches.py
--rw-r--r--   0        0        0     3862 2024-04-29 17:10:15.748016 drawlib-0.1.3/drawlib/v0_1/private/core_canvas/text.py
--rw-r--r--   0        0        0     2067 2024-05-03 16:29:49.262484 drawlib-0.1.3/drawlib/v0_1/private/download.py
--rw-r--r--   0        0        0      881 2024-05-02 13:00:20.440339 drawlib-0.1.3/drawlib/v0_1/private/dutil.py
--rw-r--r--   0        0        0      589 2024-04-13 03:31:11.518478 drawlib-0.1.3/drawlib/v0_1/private/icons/__init__.py
--rw-r--r--   0        0        0   888357 2024-05-04 13:36:37.049300 drawlib-0.1.3/drawlib/v0_1/private/icons/phosphor.py
--rw-r--r--   0        0        0     2609 2024-05-04 13:36:12.625942 drawlib-0.1.3/drawlib/v0_1/private/icons/util.py
--rw-r--r--   0        0        0     1206 2024-04-27 06:44:36.108567 drawlib-0.1.3/drawlib/v0_1/private/logging.py
--rw-r--r--   0        0        0     6687 2024-05-02 12:04:01.063777 drawlib-0.1.3/drawlib/v0_1/private/settings.py
--rw-r--r--   0        0        0      589 2024-04-25 02:41:30.472250 drawlib-0.1.3/drawlib/v0_1/private/smartarts/__init__.py
--rw-r--r--   0        0        0      426 2024-04-14 23:53:18.451455 drawlib-0.1.3/drawlib/v0_1/private/smartarts/cycle.py
--rw-r--r--   0        0        0      617 2024-04-14 10:51:41.389757 drawlib-0.1.3/drawlib/v0_1/private/smartarts/dsart.py
--rw-r--r--   0        0        0      660 2024-04-14 23:53:28.113177 drawlib-0.1.3/drawlib/v0_1/private/smartarts/groups.py
--rw-r--r--   0        0        0      619 2024-04-14 23:53:33.993167 drawlib-0.1.3/drawlib/v0_1/private/smartarts/pyramid.py
--rw-r--r--   0        0        0     6787 2024-05-01 15:20:41.772611 drawlib-0.1.3/drawlib/v0_1/private/smartarts/sourcecode.py
--rw-r--r--   0        0        0      426 2024-04-14 23:53:43.397670 drawlib-0.1.3/drawlib/v0_1/private/smartarts/table.py
--rw-r--r--   0        0        0      651 2024-04-14 23:53:50.199157 drawlib-0.1.3/drawlib/v0_1/private/smartarts/tree.py
--rw-r--r--   0        0        0     5807 2024-04-27 01:15:26.015254 drawlib-0.1.3/drawlib/v0_1/private/tools.py
--rw-r--r--   0        0        0    10163 2024-05-02 13:00:08.257932 drawlib-0.1.3/drawlib/v0_1/private/util.py
--rw-r--r--   0        0        0      758 2024-05-04 15:41:54.091618 drawlib-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     3081 1970-01-01 00:00:00.000000 drawlib-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    11344 2024-04-05 18:42:05.538150 drawlib-0.1.4/LICENSE.txt
+-rw-r--r--   0        0        0     2421 2024-05-04 15:36:12.546708 drawlib-0.1.4/README.md
+-rw-r--r--   0        0        0       27 2024-03-29 11:45:48.926601 drawlib-0.1.4/drawlib/.pylintrc
+-rw-r--r--   0        0        0     1039 2024-05-12 02:04:42.720811 drawlib-0.1.4/drawlib/__init__.py
+-rw-r--r--   0        0        0      688 2024-04-06 11:43:47.512263 drawlib-0.1.4/drawlib/__main__.py
+-rw-r--r--   0        0        0      777 2024-04-07 14:54:59.159171 drawlib-0.1.4/drawlib/apis.py
+-rw-r--r--   0        0        0      407 2024-04-12 07:27:54.821931 drawlib-0.1.4/drawlib/assets/__init__.py
+-rw-r--r--   0        0        0      407 2024-05-01 10:34:11.053352 drawlib-0.1.4/drawlib/assets/v0_1/__init__.py
+-rw-r--r--   0        0        0      407 2024-04-12 07:28:01.917218 drawlib-0.1.4/drawlib/assets/v0_1/fonticons/__init__.py
+-rw-r--r--   0        0        0      407 2024-04-13 15:48:11.439423 drawlib-0.1.4/drawlib/assets/v0_1/fonts/__init__.py
+-rw-r--r--   0        0        0     1084 2024-04-07 03:53:05.340986 drawlib-0.1.4/drawlib/v0_1/__init__.py
+-rw-r--r--   0        0        0      663 2024-04-06 12:40:11.972278 drawlib-0.1.4/drawlib/v0_1/__main__.py
+-rw-r--r--   0        0        0     2437 2024-05-04 13:37:40.227151 drawlib-0.1.4/drawlib/v0_1/apis.py
+-rw-r--r--   0        0        0      763 2024-04-06 11:52:52.776827 drawlib-0.1.4/drawlib/v0_1/private/__init__.py
+-rw-r--r--   0        0        0     5949 2024-04-27 06:45:13.999149 drawlib-0.1.4/drawlib/v0_1/private/arg_validator.py
+-rw-r--r--   0        0        0     6207 2024-04-27 06:44:59.377242 drawlib-0.1.4/drawlib/v0_1/private/command.py
+-rw-r--r--   0        0        0      548 2024-04-07 14:22:07.928062 drawlib-0.1.4/drawlib/v0_1/private/core/__init__.py
+-rw-r--r--   0        0        0    12776 2024-04-23 00:24:17.718876 drawlib-0.1.4/drawlib/v0_1/private/core/colors.py
+-rw-r--r--   0        0        0    13577 2024-04-28 11:41:37.164049 drawlib-0.1.4/drawlib/v0_1/private/core/dimage.py
+-rw-r--r--   0        0        0    14228 2024-05-01 15:22:54.625259 drawlib-0.1.4/drawlib/v0_1/private/core/fonts.py
+-rw-r--r--   0        0        0    32410 2024-05-11 15:17:05.404584 drawlib-0.1.4/drawlib/v0_1/private/core/model.py
+-rw-r--r--   0        0        0     7060 2024-04-27 01:01:21.281062 drawlib-0.1.4/drawlib/v0_1/private/core/model_validator.py
+-rw-r--r--   0        0        0    49184 2024-05-12 01:39:42.759450 drawlib-0.1.4/drawlib/v0_1/private/core/theme.py
+-rw-r--r--   0        0        0    26316 2024-05-01 14:16:45.894958 drawlib-0.1.4/drawlib/v0_1/private/core/util.py
+-rw-r--r--   0        0        0      548 2024-04-27 02:06:25.820510 drawlib-0.1.4/drawlib/v0_1/private/core_canvas/__init__.py
+-rw-r--r--   0        0        0    20400 2024-05-11 17:25:26.212255 drawlib-0.1.4/drawlib/v0_1/private/core_canvas/base.py
+-rw-r--r--   0        0        0     2328 2024-04-29 17:11:04.449382 drawlib-0.1.4/drawlib/v0_1/private/core_canvas/canvas.py
+-rw-r--r--   0        0        0     5297 2024-05-12 01:03:24.423089 drawlib-0.1.4/drawlib/v0_1/private/core_canvas/image.py
+-rw-r--r--   0        0        0     8444 2024-05-12 00:55:21.009215 drawlib-0.1.4/drawlib/v0_1/private/core_canvas/line.py
+-rw-r--r--   0        0        0     5051 2024-05-12 00:48:19.055312 drawlib-0.1.4/drawlib/v0_1/private/core_canvas/original_arrow.py
+-rw-r--r--   0        0        0    20315 2024-05-12 00:50:38.663131 drawlib-0.1.4/drawlib/v0_1/private/core_canvas/original_polygon.py
+-rw-r--r--   0        0        0    20051 2024-05-12 00:41:36.243898 drawlib-0.1.4/drawlib/v0_1/private/core_canvas/patches.py
+-rw-r--r--   0        0        0     3862 2024-04-29 17:10:15.748016 drawlib-0.1.4/drawlib/v0_1/private/core_canvas/text.py
+-rw-r--r--   0        0        0     2067 2024-05-03 16:29:49.262484 drawlib-0.1.4/drawlib/v0_1/private/download.py
+-rw-r--r--   0        0        0      881 2024-05-02 13:00:20.440339 drawlib-0.1.4/drawlib/v0_1/private/dutil.py
+-rw-r--r--   0        0        0      589 2024-04-13 03:31:11.518478 drawlib-0.1.4/drawlib/v0_1/private/icons/__init__.py
+-rw-r--r--   0        0        0   901217 2024-05-12 01:55:52.732933 drawlib-0.1.4/drawlib/v0_1/private/icons/phosphor.py
+-rw-r--r--   0        0        0     2705 2024-05-12 01:58:41.948187 drawlib-0.1.4/drawlib/v0_1/private/icons/util.py
+-rw-r--r--   0        0        0     1206 2024-04-27 06:44:36.108567 drawlib-0.1.4/drawlib/v0_1/private/logging.py
+-rw-r--r--   0        0        0     6687 2024-05-02 12:04:01.063777 drawlib-0.1.4/drawlib/v0_1/private/settings.py
+-rw-r--r--   0        0        0      589 2024-04-25 02:41:30.472250 drawlib-0.1.4/drawlib/v0_1/private/smartarts/__init__.py
+-rw-r--r--   0        0        0      426 2024-04-14 23:53:18.451455 drawlib-0.1.4/drawlib/v0_1/private/smartarts/cycle.py
+-rw-r--r--   0        0        0      617 2024-04-14 10:51:41.389757 drawlib-0.1.4/drawlib/v0_1/private/smartarts/dsart.py
+-rw-r--r--   0        0        0      660 2024-04-14 23:53:28.113177 drawlib-0.1.4/drawlib/v0_1/private/smartarts/groups.py
+-rw-r--r--   0        0        0      619 2024-04-14 23:53:33.993167 drawlib-0.1.4/drawlib/v0_1/private/smartarts/pyramid.py
+-rw-r--r--   0        0        0     6787 2024-05-01 15:20:41.772611 drawlib-0.1.4/drawlib/v0_1/private/smartarts/sourcecode.py
+-rw-r--r--   0        0        0      426 2024-04-14 23:53:43.397670 drawlib-0.1.4/drawlib/v0_1/private/smartarts/table.py
+-rw-r--r--   0        0        0      651 2024-04-14 23:53:50.199157 drawlib-0.1.4/drawlib/v0_1/private/smartarts/tree.py
+-rw-r--r--   0        0        0     5807 2024-04-27 01:15:26.015254 drawlib-0.1.4/drawlib/v0_1/private/tools.py
+-rw-r--r--   0        0        0    10163 2024-05-02 13:00:08.257932 drawlib-0.1.4/drawlib/v0_1/private/util.py
+-rw-r--r--   0        0        0      758 2024-05-12 02:05:22.899811 drawlib-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     3081 1970-01-01 00:00:00.000000 drawlib-0.1.4/PKG-INFO
```

### Comparing `drawlib-0.1.3/LICENSE.txt` & `drawlib-0.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.3/README.md` & `drawlib-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.3/drawlib/__init__.py` & `drawlib-0.1.4/drawlib/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,14 @@
 - drawlib.v0_1: API v0.1 interface (latest)
 
 """
 
 from typing import Final
 
 # please update here when you release new version
-VERSION = "0.1.3"
+VERSION = "0.1.4"
 
 # might not be changed
 LIB_NAME: Final[str] = "drawlib"
 AUTHOR: Final[str] = "Yuichi Ito"
 CONTACT: Final[str] = "yuichi@yuichi.com"
 __version__: Final[str] = VERSION
```

### Comparing `drawlib-0.1.3/drawlib/__main__.py` & `drawlib-0.1.4/drawlib/__main__.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.3/drawlib/apis.py` & `drawlib-0.1.4/drawlib/apis.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.3/drawlib/v0_1/__init__.py` & `drawlib-0.1.4/drawlib/v0_1/__init__.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.3/drawlib/v0_1/__main__.py` & `drawlib-0.1.4/drawlib/v0_1/__main__.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.3/drawlib/v0_1/apis.py` & `drawlib-0.1.4/drawlib/v0_1/apis.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.3/drawlib/v0_1/private/__init__.py` & `drawlib-0.1.4/drawlib/v0_1/private/__init__.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.3/drawlib/v0_1/private/arg_validator.py` & `drawlib-0.1.4/drawlib/v0_1/private/arg_validator.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.3/drawlib/v0_1/private/command.py` & `drawlib-0.1.4/drawlib/v0_1/private/command.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.3/drawlib/v0_1/private/core/__init__.py` & `drawlib-0.1.4/drawlib/v0_1/private/core/__init__.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.3/drawlib/v0_1/private/core/colors.py` & `drawlib-0.1.4/drawlib/v0_1/private/core/colors.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.3/drawlib/v0_1/private/core/dimage.py` & `drawlib-0.1.4/drawlib/v0_1/private/core/dimage.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.3/drawlib/v0_1/private/core/fonts.py` & `drawlib-0.1.4/drawlib/v0_1/private/core/fonts.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.3/drawlib/v0_1/private/core/model.py` & `drawlib-0.1.4/drawlib/v0_1/private/core/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,16 @@
 
 
 #
 # Please don't use external data classes such as pydantic.
 # Use property for validation
 #
 
+from __future__ import annotations
+from copy import deepcopy
 import dataclasses
 from typing import (
     Union,
     Optional,
     Tuple,
     Literal,
     Final,
@@ -70,14 +72,17 @@
 
     style: Optional[Literal["thin", "light", "regular", "bold", "fill"]] = None
     color: Union[Tuple[int, int, int], Tuple[int, int, int, float], None] = None
     alpha: Optional[float] = None
     halign: Optional[Literal["left", "center", "right"]] = None
     valign: Optional[Literal["bottom", "center", "top"]] = None
 
+    def copy(self) -> IconStyle:
+        return deepcopy(self)
+
     @property  # type: ignore[no-redef]
     def style(self) -> Optional[str]:
         """getter of style"""
         return getattr(self, "_style", None)
 
     @style.setter
     def style(self, value: Optional[str]) -> None:
@@ -165,14 +170,17 @@
 
     halign: Optional[Literal["left", "center", "right"]] = None
     valign: Optional[Literal["bottom", "center", "top"]] = None
     lwidth: Optional[float] = None
     lstyle: Optional[Literal["solid", "dashed", "dotted", "dashdot"]] = None
     lcolor: Union[Tuple[int, int, int], Tuple[int, int, int, float], None] = None
 
+    def copy(self) -> ImageStyle:
+        return deepcopy(self)
+
     @property  # type: ignore[no-redef]
     def halign(self) -> Optional[str]:
         """getter of halign"""
         return self._halign
 
     @halign.setter
     def halign(self, value: Optional[Literal["left", "center", "right"]]) -> None:
@@ -272,14 +280,17 @@
     """
 
     width: Optional[float] = None
     style: Optional[Literal["solid", "dashed", "dotted", "dashdot"]] = None
     color: Union[Tuple[int, int, int], Tuple[int, int, int, float], None] = None
     alpha: Optional[None] = None
 
+    def copy(self) -> LineStyle:
+        return deepcopy(self)
+
     @property  # type: ignore[no-redef]
     def width(self) -> Optional[float]:
         """getter of width"""
         return self._width
 
     @width.setter
     def width(self, value: Optional[float]) -> None:
@@ -368,14 +379,17 @@
     lstyle: Optional[Literal["solid", "dashed", "dotted", "dashdot"]] = None
     lwidth: Optional[float] = None
     hstyle: Optional[Literal["->", "<-", "<->", "-|>", "<|-", "<|-|>"]] = None
     hscale: Optional[int] = None
     color: Union[Tuple[int, int, int], Tuple[int, int, int, float], None] = None
     alpha: Optional[float] = None
 
+    def copy(self) -> LineArrowStyle:
+        return deepcopy(self)
+
     @property  # type: ignore[no-redef]
     def lwidth(self) -> Optional[float]:
         """getter of lwidth"""
         return self._lwidth
 
     @lwidth.setter
     def lwidth(self, value: Optional[float]) -> None:
@@ -497,14 +511,17 @@
     valign: Optional[Literal["bottom", "center", "top"]] = None
     alpha: Optional[float] = None
     lwidth: Optional[float] = None
     lcolor: Union[Tuple[int, int, int], Tuple[int, int, int, float], None] = None
     lstyle: Optional[Literal["solid", "dashed", "dotted", "dashdot"]] = None
     fcolor: Union[Tuple[int, int, int], Tuple[int, int, int, float], None] = None
 
+    def copy(self) -> ShapeStyle:
+        return deepcopy(self)
+
     @property  # type: ignore[no-redef]
     def halign(self) -> Optional[str]:
         """getter of halign"""
         return self._halign
 
     @halign.setter
     def halign(self, value: Optional[Literal["left", "center", "right"]]) -> None:
@@ -655,14 +672,17 @@
         FontFile,
         None,
     ] = None
     angle: Optional[float] = None
     flip: Optional[bool] = None
     xy_shift: Optional[Tuple[float, float]] = None
 
+    def copy(self) -> ShapeTextStyle:
+        return deepcopy(self)
+
     @property  # type: ignore[no-redef]
     def halign(self) -> Optional[str]:
         """getter of halign"""
         return self._halign
 
     @halign.setter
     def halign(self, value: Optional[Literal["left", "center", "right"]]) -> None:
@@ -881,14 +901,17 @@
     # background
     bgalpha: Optional[float] = None
     bglcolor: Union[Tuple[int, int, int], Tuple[int, int, int, float], None] = None
     bglstyle: Optional[Literal["solid", "dashed", "dotted", "dashdot"]] = None
     bglwidth: Optional[float] = None
     bgfcolor: Union[Tuple[int, int, int], Tuple[int, int, int, float], None] = None
 
+    def copy(self) -> TextStyle:
+        return deepcopy(self)
+
     @property  # type: ignore[no-redef]
     def halign(self) -> Optional[str]:
         """getter of halign"""
         return self._halign
 
     @halign.setter
     def halign(self, value: Optional[Literal["left", "center", "right"]]) -> None:
```

### Comparing `drawlib-0.1.3/drawlib/v0_1/private/core/model_validator.py` & `drawlib-0.1.4/drawlib/v0_1/private/core/model_validator.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.3/drawlib/v0_1/private/core/theme.py` & `drawlib-0.1.4/drawlib/v0_1/private/core/theme.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
 Define style theme at class ``Theme``.
 Default or choosed theme is applied if style is not provided.
 Instance ``dtheme``  is provided to user to control theme.
 
 """
 
+from __future__ import annotations
 import dataclasses
 from typing import Optional, Dict, Tuple, Union, Literal, List
 from copy import deepcopy
 
 from drawlib.v0_1.private.util import error_handler
 from drawlib.v0_1.private.core.model import (
     IconStyle,
@@ -34,17 +35,20 @@
     Font,
     FontSourceCode,
 )
 from drawlib.v0_1.private.arg_validator import ArgValidator
 
 
 @dataclasses.dataclass
-class _ThemeStyle:
+class ThemeTemplate:
     """Helper dataclass for defining theme styles"""
 
+    def copy(self) -> ThemeTemplate:
+        return deepcopy(self)
+
     # icon
     icon_style: Literal["thin", "light", "regular", "bold", "fill"]
     icon_color: Union[
         Tuple[float, float, float],
         Tuple[float, float, float, float],
     ]
 
@@ -107,15 +111,15 @@
     * define theme here
     * provide theme access methods
 
     """
 
     @error_handler
     def __init__(self):
-        self.theme_default()
+        self.theme_apply_by_name("default")
 
     #############
     ### Thema ###
     #############
 
     @error_handler
     def theme_initialize(self) -> None:
@@ -162,15 +166,146 @@
         self._shapestyles_star: Dict[str, ShapeStyle] = {}
         self._shapetextstyles: Dict[str, ShapeTextStyle] = {}
 
         # text
         self._textstyles: Dict[str, TextStyle] = {}
 
     @error_handler
-    def theme_default(self) -> None:
+    def theme_list(self) -> List[str]:
+        return ["default", "gray"]
+
+    @error_handler
+    def theme_apply_by_name(self, name: Literal["default", "gray"]) -> None:
+        if name == "default":
+            self._theme_default()
+        elif name == "gray":
+            self._theme_gray()
+        else:
+            raise ValueError(f'Theme "{name}" is not supported.')
+
+    @error_handler
+    def theme_apply_by_styles(
+        self,
+        background: Union[Tuple[int, int, int], Tuple[int, int, int, float]],
+        sourcecode_font: FontSourceCode,
+        default_styles: Tuple[
+            IconStyle,
+            ImageStyle,
+            LineStyle,
+            LineArrowStyle,
+            ShapeStyle,
+            ShapeTextStyle,
+            TextStyle,
+        ],
+        named_styles_list: List[
+            Tuple[
+                str,
+                IconStyle,
+                ImageStyle,
+                LineStyle,
+                LineArrowStyle,
+                ShapeStyle,
+                ShapeTextStyle,
+                TextStyle,
+            ]
+        ],
+    ) -> None:
+
+        # initialize
+        self.theme_initialize()
+
+        # set background and sourcecode font
+        self._background = background
+        self._sourcecode_font = sourcecode_font
+
+        # insert default styles to head of named_styles
+        default = ("",) + default_styles
+        named_styles_list.insert(0, default)
+
+        # set styles to theme
+        for name, icon, image, line, linearrow, shape, shapetext, text in named_styles_list:
+            # icon register with 3 names
+            icon_lcolor = icon.copy()
+            icon_lcolor.color = shape.lcolor
+            icon_fcolor = icon.copy()
+            icon_fcolor.color = shape.fcolor
+            self.iconstyle_set(style=icon, name=name)
+            self.iconstyle_set(style=icon_lcolor, name=f"lcolor-{name}")
+            self.iconstyle_set(style=icon_fcolor, name=f"fcolor-{name}")
+
+            self.imagestyle_set(style=image, name=name)
+            self.linestyle_set(style=line, name=name)
+
+            # line arrow register with 2 names
+            # providing just name makes style LineStyle.
+            # But using linearrow-{name} makes style LineArrowStyle
+            self.linearrowstyle_set(style=linearrow, name=name)
+            self.linearrowstyle_set(style=linearrow, name=f"linearrow-{name}")
+
+            self.shapestyle_set(style=shape, name=name)
+            self.shapetextstyle_set(style=shapetext, name=name)
+            self.textstyle_set(style=text, name=name)
+
+    @error_handler
+    def theme_generate_styles(
+        self, template: ThemeTemplate
+    ) -> Tuple[IconStyle, ImageStyle, LineStyle, LineArrowStyle, ShapeStyle, ShapeTextStyle, TextStyle]:
+
+        icon = IconStyle(
+            style=template.icon_style,
+            color=template.icon_color,
+            halign="center",
+            valign="center",
+        )
+        image = ImageStyle(
+            lwidth=0,
+            lstyle=template.shape_line_style,
+            lcolor=template.shape_line_color,
+            halign="center",
+            valign="center",
+        )
+        line = LineStyle(
+            style=template.line_style,
+            width=template.line_width,
+            color=template.line_color,
+        )
+        linearrow = LineArrowStyle(
+            lstyle=template.line_style,
+            lwidth=template.line_width,
+            hstyle=template.arrowhead_style,
+            hscale=template.arrowhead_scale,
+            color=template.line_color,
+        )
+        shape = ShapeStyle(
+            lwidth=template.shape_line_width,
+            lstyle=template.shape_line_style,
+            lcolor=template.shape_line_color,
+            fcolor=template.shape_fill_color,
+            halign="center",
+            valign="center",
+        )
+        shapetext = ShapeTextStyle(
+            font=template.text_font,
+            size=template.text_size,
+            color=template.text_color,
+            halign="center",
+            valign="center",
+        )
+        text = TextStyle(
+            font=template.text_font,
+            size=template.text_size,
+            color=template.text_color,
+            halign="center",
+            valign="center",
+        )
+
+        return (icon, image, line, linearrow, shape, shapetext, text)
+
+    @error_handler
+    def _theme_default(self) -> None:
         """Change theme to default.
 
         Returns:
             None
 
         """
 
@@ -184,15 +319,15 @@
         green_light = _get_rgba_from_hex("#70C2BF")
         green_dark = _get_rgba_from_hex("#0C1D1C")
 
         # third color
         pink_light = _get_rgba_from_hex("#C1666B")
         pink_dark = _get_rgba_from_hex("#1D0C0D")
 
-        tstyle1 = _ThemeStyle(
+        default_template = ThemeTemplate(
             icon_style="thin",
             icon_color=blue_dark,
             line_style="solid",
             line_width=2,
             line_color=blue_dark,
             arrowhead_style="->",
             arrowhead_scale=20,
@@ -205,38 +340,46 @@
             shapetext_size=16,
             shapetext_color=blue_dark,
             text_font=Font.SANSSERIF_REGULAR,
             text_size=16,
             text_color=blue_dark,
         )
 
-        tstyle2 = deepcopy(tstyle1)
-        tstyle2.line_color = green_dark
-        tstyle2.shape_line_color = green_dark
-        tstyle2.shape_fill_color = green_light
-        tstyle2.shapetext_color = green_dark
-        tstyle2.text_color = green_dark
-
-        tstyle3 = deepcopy(tstyle1)
-        tstyle3.line_color = pink_dark
-        tstyle3.shape_line_color = pink_dark
-        tstyle3.shape_fill_color = pink_light
-        tstyle3.shapetext_color = pink_dark
-        tstyle3.text_color = pink_dark
+        blue_template = default_template.copy()
 
-        self._apply_thema_styles(
+        green_template = default_template.copy()
+        green_template.line_color = green_dark
+        green_template.shape_line_color = green_dark
+        green_template.shape_fill_color = green_light
+        green_template.shapetext_color = green_dark
+        green_template.text_color = green_dark
+
+        pink_template = default_template.copy()
+        pink_template.line_color = pink_dark
+        pink_template.shape_line_color = pink_dark
+        pink_template.shape_fill_color = pink_light
+        pink_template.shapetext_color = pink_dark
+        pink_template.text_color = pink_dark
+
+        default_styles = self.theme_generate_styles(default_template)
+        named_styles_list = [
+            ("blue",) + self.theme_generate_styles(blue_template),
+            ("green",) + self.theme_generate_styles(green_template),
+            ("pink",) + self.theme_generate_styles(pink_template),
+        ]
+
+        self.theme_apply_by_styles(
             background=(255, 255, 255, 1),  # white
             sourcecode_font=FontSourceCode.SOURCECODEPRO,
-            tstyle1=tstyle1,
-            tstyle2=tstyle2,
-            tstyle3=tstyle3,
+            default_styles=default_styles,
+            named_styles_list=named_styles_list,
         )
 
     @error_handler
-    def theme_gray(self) -> None:
+    def _theme_gray(self) -> None:
         """Change theme to gray.
 
         Returns:
             None
 
         """
 
@@ -248,15 +391,15 @@
 
         # secondary color
         gray2 = _get_rgba_from_hex("#CED4DA")
 
         # third color
         gray3 = _get_rgba_from_hex("#DEE2E6")
 
-        tstyle1 = _ThemeStyle(
+        default_template = ThemeTemplate(
             icon_style="thin",
             icon_color=gray_dark,
             line_style="solid",
             line_width=2,
             line_color=gray_dark,
             arrowhead_style="->",
             arrowhead_scale=20,
@@ -269,26 +412,32 @@
             shapetext_size=16,
             shapetext_color=gray_dark,
             text_font=Font.SANSSERIF_REGULAR,
             text_size=16,
             text_color=gray_dark,
         )
 
-        tstyle2 = deepcopy(tstyle1)
-        tstyle2.shape_fill_color = gray2
-
-        tstyle3 = deepcopy(tstyle1)
-        tstyle3.shape_fill_color = gray3
+        gray1_template = default_template.copy()
+        gray2_template = default_template.copy()
+        gray2_template.shape_fill_color = gray2
+        gray3_template = default_template.copy()
+        gray3_template.shape_fill_color = gray3
+
+        default_styles = self.theme_generate_styles(default_template)
+        named_styles_list = [
+            ("gray1",) + self.theme_generate_styles(gray1_template),
+            ("gray2",) + self.theme_generate_styles(gray2_template),
+            ("gray3",) + self.theme_generate_styles(gray3_template),
+        ]
 
-        self._apply_thema_styles(
+        self.theme_apply_by_styles(
             background=(255, 255, 255, 1),  # white
             sourcecode_font=FontSourceCode.SOURCECODEPRO,
-            tstyle1=tstyle1,
-            tstyle2=tstyle2,
-            tstyle3=tstyle3,
+            default_styles=default_styles,
+            named_styles_list=named_styles_list,
         )
 
     ##################
     ### Background ###
     ##################
 
     @error_handler
@@ -367,29 +516,29 @@
         self._background = self._background[:-1] + (alpha,)
 
     ############
     ### Icon ###
     ############
 
     @error_handler
-    def iconstyle_get(self, name: str = "1") -> IconStyle:
+    def iconstyle_get(self, name: str = "") -> IconStyle:
         """Get theme IconStyle.
 
         Args:
             name(option): key
 
         Returns:
             IconStyle
 
         """
 
         return deepcopy(self._iconstyles[name])
 
     @error_handler
-    def iconstyle_set(self, style: IconStyle, name: str = "1") -> None:
+    def iconstyle_set(self, style: IconStyle, name: str = "") -> None:
         """Set theme IconStyle.
 
         Args:
             style: theme IconStyle
             name(optional): key
 
         Returns:
@@ -397,15 +546,15 @@
 
         """
 
         ArgValidator.validate_iconstyle("style", style)
         ArgValidator.validate_str("name", name)
         self._iconstyles[name] = deepcopy(style)
 
-    def iconstyle_has(self, name: str = "1") -> bool:
+    def iconstyle_has(self, name: str = "") -> bool:
         """Check having theme IconStyle.
 
         Args:
             name(option): key
 
         Returns:
             bool
@@ -425,29 +574,29 @@
         return list(self._iconstyles.keys())
 
     ############
     ### Image ###
     ############
 
     @error_handler
-    def imagestyle_get(self, name: str = "1") -> ImageStyle:
+    def imagestyle_get(self, name: str = "") -> ImageStyle:
         """Get theme ImageStyle.
 
         Args:
             name(option): key
 
         Returns:
             ImageStyle
 
         """
 
         return deepcopy(self._imagestyles[name])
 
     @error_handler
-    def imagestyle_set(self, style: ImageStyle, name: str = "1") -> None:
+    def imagestyle_set(self, style: ImageStyle, name: str = "") -> None:
         """Set theme ImageStyle.
 
         Args:
             style: theme ImageStyle
             name(optional): key
 
         Returns:
@@ -455,15 +604,15 @@
 
         """
 
         ArgValidator.validate_imagestyle("style", style)
         ArgValidator.validate_str("name", name)
         self._imagestyles[name] = deepcopy(style)
 
-    def imagestyle_has(self, name: str = "1") -> bool:
+    def imagestyle_has(self, name: str = "") -> bool:
         """Check having theme ImageStyle.
 
         Args:
             name(option): key
 
         Returns:
             bool
@@ -483,29 +632,29 @@
         return list(self._imagestyles.keys())
 
     ############
     ### Line ###
     ############
 
     @error_handler
-    def linestyle_get(self, name: str = "1") -> LineStyle:
+    def linestyle_get(self, name: str = "") -> LineStyle:
         """Get theme LineStyle.
 
         Args:
             name(option): key
 
         Returns:
             LineStyle
 
         """
 
         return deepcopy(self._linestyles[name])
 
     @error_handler
-    def linestyle_set(self, style: LineStyle, name: str = "1") -> None:
+    def linestyle_set(self, style: LineStyle, name: str = "") -> None:
         """Set theme LineStyle.
 
         Args:
             style: theme LineStyle
             name(optional): key
 
         Returns:
@@ -513,15 +662,15 @@
 
         """
 
         ArgValidator.validate_linestyle("style", style)
         ArgValidator.validate_str("name", name)
         self._linestyles[name] = deepcopy(style)
 
-    def linestyle_has(self, name: str = "1") -> bool:
+    def linestyle_has(self, name: str = "") -> bool:
         """Check having theme LineStyle.
 
         Args:
             name(option): key
 
         Returns:
             bool
@@ -537,29 +686,29 @@
             List[str]: names
 
         """
 
         return list(self._linestyles.keys())
 
     @error_handler
-    def linearrowstyle_get(self, name: str = "1") -> LineArrowStyle:
+    def linearrowstyle_get(self, name: str = "") -> LineArrowStyle:
         """Get theme LineArrowStyle.
 
         Args:
             name(optional): key
 
         Returns:
             LineArrowStyle
 
         """
 
         return deepcopy(self._linearrowstyles[name])
 
     @error_handler
-    def linearrowstyle_set(self, style: LineArrowStyle, name: str = "1") -> None:
+    def linearrowstyle_set(self, style: LineArrowStyle, name: str = "") -> None:
         """Set theme LineArrowStyle.
 
         Args:
             style: theme LineArrowStyle
             name(optional): key
 
         Returns:
@@ -567,15 +716,15 @@
 
         """
 
         ArgValidator.validate_linearrowstyle("style", style)
         ArgValidator.validate_str("name", name)
         self._linearrowstyles[name] = deepcopy(style)
 
-    def linearrowstyle_has(self, name: str = "1") -> bool:
+    def linearrowstyle_has(self, name: str = "") -> bool:
         """Check having theme LineArrowStyle.
 
         Args:
             name(option): key
 
         Returns:
             bool
@@ -595,29 +744,29 @@
         return list(self._linearrowstyles.keys())
 
     ############
     ### Text ###
     ############
 
     @error_handler
-    def textstyle_get(self, name: str = "1") -> TextStyle:
+    def textstyle_get(self, name: str = "") -> TextStyle:
         """Get theme TextStyle.
 
         Args:
             name(optional): key
 
         Returns:
             TextStyle
 
         """
 
         return deepcopy(self._textstyles[name])
 
     @error_handler
-    def textstyle_set(self, style: TextStyle, name: str = "1") -> None:
+    def textstyle_set(self, style: TextStyle, name: str = "") -> None:
         """Set theme TextStyle.
 
         Args:
             style: theme TextStyle
             name(optional): key
 
         Returns:
@@ -625,15 +774,15 @@
 
         """
 
         ArgValidator.validate_textstyle("style", style)
         ArgValidator.validate_str("name", name)
         self._textstyles[name] = deepcopy(style)
 
-    def textstyle_has(self, name: str = "1") -> bool:
+    def textstyle_has(self, name: str = "") -> bool:
         """Check having theme TextStyle.
 
         Args:
             name(option): key
 
         Returns:
             bool
@@ -677,29 +826,29 @@
         self._sourcecode_font = font
 
     #############
     ### Shape ###
     #############
 
     @error_handler
-    def shapestyle_get(self, name: str = "1") -> ShapeStyle:
+    def shapestyle_get(self, name: str = "") -> ShapeStyle:
         """Get theme ShapeStyle.
 
         Args:
             name(optional): key
 
         Returns:
             ShapeStyle
 
         """
 
         return deepcopy(self._shapestyles[name])
 
     @error_handler
-    def shapestyle_set(self, style: ShapeStyle, name: str = "1") -> None:
+    def shapestyle_set(self, style: ShapeStyle, name: str = "") -> None:
         """Set theme ShapeStyle.
 
         Args:
             style: theme ShapeStyle
             name(optional): key
 
         Returns:
@@ -707,15 +856,15 @@
 
         """
 
         ArgValidator.validate_shapestyle("style", style)
         ArgValidator.validate_str("name", name)
         self._shapestyles[name] = deepcopy(style)
 
-    def shapestyle_has(self, name: str = "1") -> bool:
+    def shapestyle_has(self, name: str = "") -> bool:
         """Check having theme ShapeStyle.
 
         Args:
             name(option): key
 
         Returns:
             bool
@@ -731,29 +880,29 @@
             List[str]: names
 
         """
 
         return list(self._shapestyles.keys())
 
     @error_handler
-    def shapetextstyle_get(self, name: str = "1") -> ShapeTextStyle:
+    def shapetextstyle_get(self, name: str = "") -> ShapeTextStyle:
         """Get theme ShapeTextStyle.
 
         Args:
             name(optional): key
 
         Returns:
             ShapeTextStyle
 
         """
 
         return deepcopy(self._shapetextstyles[name])
 
     @error_handler
-    def shapetextstyle_set(self, style: ShapeTextStyle, name: str = "1") -> None:
+    def shapetextstyle_set(self, style: ShapeTextStyle, name: str = "") -> None:
         """Set theme ShapeTextStyle.
 
         Args:
             style: theme ShapeTextStyle
             name(optional): key
 
         Returns:
@@ -761,15 +910,15 @@
 
         """
 
         ArgValidator.validate_shapetextstyle("style", style)
         ArgValidator.validate_str("name", name)
         self._shapetextstyles[name] = deepcopy(style)
 
-    def shapetextstyle_has(self, name: str = "1") -> bool:
+    def shapetextstyle_has(self, name: str = "") -> bool:
         """Check having theme ShapeTextStyle.
 
         Args:
             name(option): key
 
         Returns:
             bool
@@ -785,15 +934,15 @@
             List[str]: names
 
         """
 
         return list(self._shapetextstyles.keys())
 
     @error_handler
-    def shapestyle_arc_get(self, name: str = "1") -> ShapeStyle:
+    def shapestyle_arc_get(self, name: str = "") -> ShapeStyle:
         """Get theme ShapeStyle for arc.
 
         If ShapeStyle is not set for arc, get general ShapeStyle.
 
         Args:
             name(optional): key
 
@@ -805,15 +954,15 @@
         if name in self._shapestyles_arc:
             return deepcopy(self._shapestyles_arc[name])
         style = deepcopy(self._shapestyles[name])
         style.fcolor = None  # arc default style doesn't have fill color
         return style
 
     @error_handler
-    def shapestyle_arc_set(self, style: ShapeStyle, name: str = "1") -> None:
+    def shapestyle_arc_set(self, style: ShapeStyle, name: str = "") -> None:
         """Set theme ShapeStyle for arc.
 
         Args:
             style: theme ShapeStyle for arc
             name(optional): key
 
         Returns:
@@ -821,15 +970,15 @@
 
         """
 
         ArgValidator.validate_shapestyle("style", style)
         ArgValidator.validate_str("name", name)
         self._shapestyles_arc[name] = deepcopy(style)
 
-    def shapestyle_arc_has(self, name: str = "1") -> bool:
+    def shapestyle_arc_has(self, name: str = "") -> bool:
         """Check having theme ShapeStyle for arc.
 
         Args:
             name(option): key
 
         Returns:
             bool
@@ -845,15 +994,15 @@
             List[str]: names
 
         """
 
         return list(self._shapestyles_arc.keys())
 
     @error_handler
-    def shapestyle_arrow_get(self, name: str = "1") -> ShapeStyle:
+    def shapestyle_arrow_get(self, name: str = "") -> ShapeStyle:
         """Get theme ShapeStyle for arrow.
 
         If ShapeStyle is not set for arrow, get general ShapeStyle.
 
         Args:
             name(optional): key
 
@@ -863,15 +1012,15 @@
         """
 
         if name in self._shapestyles_arrow:
             return deepcopy(self._shapestyles_arrow[name])
         return deepcopy(self._shapestyles[name])
 
     @error_handler
-    def shapestyle_arrow_set(self, style: ShapeStyle, name: str = "1") -> None:
+    def shapestyle_arrow_set(self, style: ShapeStyle, name: str = "") -> None:
         """Set theme ShapeStyle for arrow.
 
         Args:
             style: theme ShapeStyle for arrow
             name(optional): key
 
         Returns:
@@ -879,15 +1028,15 @@
 
         """
 
         ArgValidator.validate_shapestyle("style", style)
         ArgValidator.validate_str("name", name)
         self._shapestyles_arrow[name] = deepcopy(style)
 
-    def shapestyle_arrow_has(self, name: str = "1") -> bool:
+    def shapestyle_arrow_has(self, name: str = "") -> bool:
         """Check having theme ShapeStyle for arrow.
 
         Args:
             name(option): key
 
         Returns:
             bool
@@ -903,15 +1052,15 @@
             List[str]: names
 
         """
 
         return list(self._shapestyles_arrow.keys())
 
     @error_handler
-    def shapestyle_circle_get(self, name: str = "1") -> ShapeStyle:
+    def shapestyle_circle_get(self, name: str = "") -> ShapeStyle:
         """Get theme ShapeStyle for circle.
 
         If ShapeStyle is not set for circle, get general ShapeStyle.
 
         Args:
             name(optional): key
 
@@ -921,30 +1070,30 @@
         """
 
         if name in self._shapestyles_circle:
             return deepcopy(self._shapestyles_circle[name])
         return deepcopy(self._shapestyles[name])
 
     @error_handler
-    def shapestyle_circle_set(self, style: ShapeStyle, name: str = "1") -> None:
+    def shapestyle_circle_set(self, style: ShapeStyle, name: str = "") -> None:
         """Set theme ShapeStyle for circle.
 
         Args:
             style: theme ShapeStyle for circle
             name(optional): key
 
         Returns:
             None
 
         """
         ArgValidator.validate_shapestyle("style", style)
         ArgValidator.validate_str("name", name)
         self._shapestyles_circle[name] = deepcopy(style)
 
-    def shapestyle_circle_has(self, name: str = "1") -> bool:
+    def shapestyle_circle_has(self, name: str = "") -> bool:
         """Check having theme ShapeStyle for circle.
 
         Args:
             name(option): key
 
         Returns:
             bool
@@ -960,15 +1109,15 @@
             List[str]: names
 
         """
 
         return list(self._shapestyles_circle.keys())
 
     @error_handler
-    def shapestyle_ellipse_get(self, name: str = "1") -> ShapeStyle:
+    def shapestyle_ellipse_get(self, name: str = "") -> ShapeStyle:
         """Get theme ShapeStyle for ellipse.
 
         If ShapeStyle is not set for ellipse, get general ShapeStyle.
 
         Args:
             name(optional): key
 
@@ -978,15 +1127,15 @@
         """
 
         if name in self._shapestyles_ellipse:
             return deepcopy(self._shapestyles_ellipse[name])
         return deepcopy(self._shapestyles[name])
 
     @error_handler
-    def shapestyle_ellipse_set(self, style: ShapeStyle, name: str = "1") -> None:
+    def shapestyle_ellipse_set(self, style: ShapeStyle, name: str = "") -> None:
         """Set theme ShapeStyle for ellipse.
 
         Args:
             style: theme ShapeStyle for ellipse
             name(optional): key
 
         Returns:
@@ -994,15 +1143,15 @@
 
         """
 
         ArgValidator.validate_shapestyle("style", style)
         ArgValidator.validate_str("name", name)
         self._shapestyles_ellipse[name] = deepcopy(style)
 
-    def shapestyle_ellipse_has(self, name: str = "1") -> bool:
+    def shapestyle_ellipse_has(self, name: str = "") -> bool:
         """Check having theme ShapeStyle for ellipse.
 
         Args:
             name(option): key
 
         Returns:
             bool
@@ -1018,15 +1167,15 @@
             List[str]: names
 
         """
 
         return list(self._shapestyles_ellipse.keys())
 
     @error_handler
-    def shapestyle_polygon_get(self, name: str = "1") -> ShapeStyle:
+    def shapestyle_polygon_get(self, name: str = "") -> ShapeStyle:
         """Get theme ShapeStyle for polygon.
 
         If ShapeStyle is not set for polygon, get general ShapeStyle.
 
         Args:
             name(optional): key
 
@@ -1036,15 +1185,15 @@
         """
 
         if name in self._shapestyles_polygon:
             return deepcopy(self._shapestyles_polygon[name])
         return deepcopy(self._shapestyles[name])
 
     @error_handler
-    def shapestyle_polygon_set(self, style: ShapeStyle, name: str = "1") -> None:
+    def shapestyle_polygon_set(self, style: ShapeStyle, name: str = "") -> None:
         """Set theme ShapeStyle for polygon.
 
         Args:
             style: theme ShapeStyle for polygon
             name(optional): key
 
         Returns:
@@ -1052,15 +1201,15 @@
 
         """
 
         ArgValidator.validate_shapestyle("style", style)
         ArgValidator.validate_str("name", name)
         self._shapestyles_polygon[name] = deepcopy(style)
 
-    def shapestyle_polygon_has(self, name: str = "1") -> bool:
+    def shapestyle_polygon_has(self, name: str = "") -> bool:
         """Check having theme ShapeStyle for polygon.
 
         Args:
             name(option): key
 
         Returns:
             bool
@@ -1076,15 +1225,15 @@
             List[str]: names
 
         """
 
         return list(self._shapestyles_polygon.keys())
 
     @error_handler
-    def shapestyle_rectangle_get(self, name: str = "1") -> ShapeStyle:
+    def shapestyle_rectangle_get(self, name: str = "") -> ShapeStyle:
         """Get theme ShapeStyle for rectangle.
 
         If ShapeStyle is not set for rectangle, get general ShapeStyle.
 
         Args:
             name(optional): key
 
@@ -1094,15 +1243,15 @@
         """
 
         if name in self._shapestyles_rectangle:
             return deepcopy(self._shapestyles_rectangle[name])
         return deepcopy(self._shapestyles[name])
 
     @error_handler
-    def shapestyle_rectangle_set(self, style: ShapeStyle, name: str = "1") -> None:
+    def shapestyle_rectangle_set(self, style: ShapeStyle, name: str = "") -> None:
         """Set theme ShapeStyle for rectangle.
 
         Args:
             style: theme ShapeStyle for rectangle
             name(optional): key
 
         Returns:
@@ -1110,15 +1259,15 @@
 
         """
 
         ArgValidator.validate_shapestyle("style", style)
         ArgValidator.validate_str("name", name)
         self._shapestyles_rectangle[name] = deepcopy(style)
 
-    def shapestyle_rectangle_has(self, name: str = "1") -> bool:
+    def shapestyle_rectangle_has(self, name: str = "") -> bool:
         """Check having theme ShapeStyle for rectangle.
 
         Args:
             name(option): key
 
         Returns:
             bool
@@ -1134,15 +1283,15 @@
             List[str]: names
 
         """
 
         return list(self._shapestyles_rectangle.keys())
 
     @error_handler
-    def shapestyle_regularpolygon_get(self, name: str = "1") -> ShapeStyle:
+    def shapestyle_regularpolygon_get(self, name: str = "") -> ShapeStyle:
         """Get theme ShapeStyle for regularpolygon.
 
         If ShapeStyle is not set for regularpolygon, get general ShapeStyle.
 
         Args:
             name(optional): key
 
@@ -1152,15 +1301,15 @@
         """
 
         if name in self._shapestyles_regularpolygon:
             return deepcopy(self._shapestyles_regularpolygon[name])
         return deepcopy(self._shapestyles[name])
 
     @error_handler
-    def shapestyle_regularpolygon_set(self, style: ShapeStyle, name: str = "1") -> None:
+    def shapestyle_regularpolygon_set(self, style: ShapeStyle, name: str = "") -> None:
         """Set theme ShapeStyle for regularpolygon.
 
         Args:
             style: theme ShapeStyle for regularpolygon
             name(optional): key
 
         Returns:
@@ -1168,15 +1317,15 @@
 
         """
 
         ArgValidator.validate_shapestyle("style", style)
         ArgValidator.validate_str("name", name)
         self._shapestyles_regularpolygon[name] = deepcopy(style)
 
-    def shapestyle_regularpolygon_has(self, name: str = "1") -> bool:
+    def shapestyle_regularpolygon_has(self, name: str = "") -> bool:
         """Check having theme ShapeStyle for regularpolygon.
 
         Args:
             name(option): key
 
         Returns:
             bool
@@ -1192,15 +1341,15 @@
             List[str]: names
 
         """
 
         return list(self._shapestyles_regularpolygon.keys())
 
     @error_handler
-    def shapestyle_wedge_get(self, name: str = "1") -> ShapeStyle:
+    def shapestyle_wedge_get(self, name: str = "") -> ShapeStyle:
         """Get theme ShapeStyle for wedge.
 
         If ShapeStyle is not set for wedge, get general ShapeStyle.
 
         Args:
             name(optional): key
 
@@ -1210,15 +1359,15 @@
         """
 
         if name in self._shapestyles_wedge:
             return deepcopy(self._shapestyles_wedge[name])
         return deepcopy(self._shapestyles[name])
 
     @error_handler
-    def shapestyle_wedge_set(self, style: ShapeStyle, name: str = "1") -> None:
+    def shapestyle_wedge_set(self, style: ShapeStyle, name: str = "") -> None:
         """Set theme ShapeStyle for wedge.
 
         Args:
             style: theme ShapeStyle for wedge
             name(optional): key
 
         Returns:
@@ -1226,15 +1375,15 @@
 
         """
 
         ArgValidator.validate_shapestyle("style", style)
         ArgValidator.validate_str("name", name)
         self._shapestyles_wedge[name] = deepcopy(style)
 
-    def shapestyle_wedge_has(self, name: str = "1") -> bool:
+    def shapestyle_wedge_has(self, name: str = "") -> bool:
         """Check having theme ShapeStyle for wedge.
 
         Args:
             name(option): key
 
         Returns:
             bool
@@ -1252,15 +1401,15 @@
         """
 
         return list(self._shapestyles_wedge.keys())
 
     # donuts
 
     @error_handler
-    def shapestyle_donuts_get(self, name: str = "1") -> ShapeStyle:
+    def shapestyle_donuts_get(self, name: str = "") -> ShapeStyle:
         """Get theme ShapeStyle for donuts.
 
         If ShapeStyle is not set for arc, get general ShapeStyle.
 
         Args:
             name(optional): key
 
@@ -1271,15 +1420,15 @@
 
         if name in self._shapestyles_donuts:
             return deepcopy(self._shapestyles_donuts[name])
         style = deepcopy(self._shapestyles[name])
         return style
 
     @error_handler
-    def shapestyle_donuts_set(self, style: ShapeStyle, name: str = "1") -> None:
+    def shapestyle_donuts_set(self, style: ShapeStyle, name: str = "") -> None:
         """Set theme ShapeStyle for donuts.
 
         Args:
             style: theme ShapeStyle for donuts
             name(optional): key
 
         Returns:
@@ -1287,15 +1436,15 @@
 
         """
 
         ArgValidator.validate_shapestyle("style", style)
         ArgValidator.validate_str("name", name)
         self._shapestyles_donuts[name] = deepcopy(style)
 
-    def shapestyle_donuts_has(self, name: str = "1") -> bool:
+    def shapestyle_donuts_has(self, name: str = "") -> bool:
         """Check having theme ShapeStyle for donuts.
 
         Args:
             name(option): key
 
         Returns:
             bool
@@ -1313,15 +1462,15 @@
         """
 
         return list(self._shapestyles_donuts.keys())
 
     # fan
 
     @error_handler
-    def shapestyle_fan_get(self, name: str = "1") -> ShapeStyle:
+    def shapestyle_fan_get(self, name: str = "") -> ShapeStyle:
         """Get theme ShapeStyle for fan.
 
         If ShapeStyle is not set for arc, get general ShapeStyle.
 
         Args:
             name(optional): key
 
@@ -1332,15 +1481,15 @@
 
         if name in self._shapestyles_fan:
             return deepcopy(self._shapestyles_fan[name])
         style = deepcopy(self._shapestyles[name])
         return style
 
     @error_handler
-    def shapestyle_fan_set(self, style: ShapeStyle, name: str = "1") -> None:
+    def shapestyle_fan_set(self, style: ShapeStyle, name: str = "") -> None:
         """Set theme ShapeStyle for fan.
 
         Args:
             style: theme ShapeStyle for fan
             name(optional): key
 
         Returns:
@@ -1348,15 +1497,15 @@
 
         """
 
         ArgValidator.validate_shapestyle("style", style)
         ArgValidator.validate_str("name", name)
         self._shapestyles_fan[name] = deepcopy(style)
 
-    def shapestyle_fan_has(self, name: str = "1") -> bool:
+    def shapestyle_fan_has(self, name: str = "") -> bool:
         """Check having theme ShapeStyle for fan.
 
         Args:
             name(option): key
 
         Returns:
             bool
@@ -1374,15 +1523,15 @@
         """
 
         return list(self._shapestyles_fan.keys())
 
     # bubblespeech
 
     @error_handler
-    def shapestyle_bubblespeech_get(self, name: str = "1") -> ShapeStyle:
+    def shapestyle_bubblespeech_get(self, name: str = "") -> ShapeStyle:
         """Get theme ShapeStyle for bubblespeech.
 
         If ShapeStyle is not set for arc, get general ShapeStyle.
 
         Args:
             name(optional): key
 
@@ -1393,15 +1542,15 @@
 
         if name in self._shapestyles_bubblespeech:
             return deepcopy(self._shapestyles_bubblespeech[name])
         style = deepcopy(self._shapestyles[name])
         return style
 
     @error_handler
-    def shapestyle_bubblespeech_set(self, style: ShapeStyle, name: str = "1") -> None:
+    def shapestyle_bubblespeech_set(self, style: ShapeStyle, name: str = "") -> None:
         """Set theme ShapeStyle for bubblespeech.
 
         Args:
             style: theme ShapeStyle for bubblespeech
             name(optional): key
 
         Returns:
@@ -1409,15 +1558,15 @@
 
         """
 
         ArgValidator.validate_shapestyle("style", style)
         ArgValidator.validate_str("name", name)
         self._shapestyles_bubblespeech[name] = deepcopy(style)
 
-    def shapestyle_bubblespeech_has(self, name: str = "1") -> bool:
+    def shapestyle_bubblespeech_has(self, name: str = "") -> bool:
         """Check having theme ShapeStyle for bubblespeech.
 
         Args:
             name(option): key
 
         Returns:
             bool
@@ -1435,15 +1584,15 @@
         """
 
         return list(self._shapestyles_bubblespeech.keys())
 
     # triangle
 
     @error_handler
-    def shapestyle_triangle_get(self, name: str = "1") -> ShapeStyle:
+    def shapestyle_triangle_get(self, name: str = "") -> ShapeStyle:
         """Get theme ShapeStyle for triangle.
 
         If ShapeStyle is not set for arc, get general ShapeStyle.
 
         Args:
             name(optional): key
 
@@ -1454,15 +1603,15 @@
 
         if name in self._shapestyles_triangle:
             return deepcopy(self._shapestyles_triangle[name])
         style = deepcopy(self._shapestyles[name])
         return style
 
     @error_handler
-    def shapestyle_triangle_set(self, style: ShapeStyle, name: str = "1") -> None:
+    def shapestyle_triangle_set(self, style: ShapeStyle, name: str = "") -> None:
         """Set theme ShapeStyle for triangle.
 
         Args:
             style: theme ShapeStyle for triangle
             name(optional): key
 
         Returns:
@@ -1470,15 +1619,15 @@
 
         """
 
         ArgValidator.validate_shapestyle("style", style)
         ArgValidator.validate_str("name", name)
         self._shapestyles_triangle[name] = deepcopy(style)
 
-    def shapestyle_triangle_has(self, name: str = "1") -> bool:
+    def shapestyle_triangle_has(self, name: str = "") -> bool:
         """Check having theme ShapeStyle for triangle.
 
         Args:
             name(option): key
 
         Returns:
             bool
@@ -1496,15 +1645,15 @@
         """
 
         return list(self._shapestyles_triangle.keys())
 
     # parallelogram
 
     @error_handler
-    def shapestyle_parallelogram_get(self, name: str = "1") -> ShapeStyle:
+    def shapestyle_parallelogram_get(self, name: str = "") -> ShapeStyle:
         """Get theme ShapeStyle for parallelogram.
 
         If ShapeStyle is not set for arc, get general ShapeStyle.
 
         Args:
             name(optional): key
 
@@ -1515,15 +1664,15 @@
 
         if name in self._shapestyles_parallelogram:
             return deepcopy(self._shapestyles_parallelogram[name])
         style = deepcopy(self._shapestyles[name])
         return style
 
     @error_handler
-    def shapestyle_parallelogram_set(self, style: ShapeStyle, name: str = "1") -> None:
+    def shapestyle_parallelogram_set(self, style: ShapeStyle, name: str = "") -> None:
         """Set theme ShapeStyle for parallelogram.
 
         Args:
             style: theme ShapeStyle for parallelogram
             name(optional): key
 
         Returns:
@@ -1531,15 +1680,15 @@
 
         """
 
         ArgValidator.validate_shapestyle("style", style)
         ArgValidator.validate_str("name", name)
         self._shapestyles_parallelogram[name] = deepcopy(style)
 
-    def shapestyle_parallelogram_has(self, name: str = "1") -> bool:
+    def shapestyle_parallelogram_has(self, name: str = "") -> bool:
         """Check having theme ShapeStyle for parallelogram.
 
         Args:
             name(option): key
 
         Returns:
             bool
@@ -1557,15 +1706,15 @@
         """
 
         return list(self._shapestyles_parallelogram.keys())
 
     # trapezoid
 
     @error_handler
-    def shapestyle_trapezoid_get(self, name: str = "1") -> ShapeStyle:
+    def shapestyle_trapezoid_get(self, name: str = "") -> ShapeStyle:
         """Get theme ShapeStyle for trapezoid.
 
         If ShapeStyle is not set for arc, get general ShapeStyle.
 
         Args:
             name(optional): key
 
@@ -1576,15 +1725,15 @@
 
         if name in self._shapestyles_trapezoid:
             return deepcopy(self._shapestyles_trapezoid[name])
         style = deepcopy(self._shapestyles[name])
         return style
 
     @error_handler
-    def shapestyle_trapezoid_set(self, style: ShapeStyle, name: str = "1") -> None:
+    def shapestyle_trapezoid_set(self, style: ShapeStyle, name: str = "") -> None:
         """Set theme ShapeStyle for trapezoid.
 
         Args:
             style: theme ShapeStyle for trapezoid
             name(optional): key
 
         Returns:
@@ -1592,15 +1741,15 @@
 
         """
 
         ArgValidator.validate_shapestyle("style", style)
         ArgValidator.validate_str("name", name)
         self._shapestyles_trapezoid[name] = deepcopy(style)
 
-    def shapestyle_trapezoid_has(self, name: str = "1") -> bool:
+    def shapestyle_trapezoid_has(self, name: str = "") -> bool:
         """Check having theme ShapeStyle for trapezoid.
 
         Args:
             name(option): key
 
         Returns:
             bool
@@ -1618,15 +1767,15 @@
         """
 
         return list(self._shapestyles_trapezoid.keys())
 
     # rhombus
 
     @error_handler
-    def shapestyle_rhombus_get(self, name: str = "1") -> ShapeStyle:
+    def shapestyle_rhombus_get(self, name: str = "") -> ShapeStyle:
         """Get theme ShapeStyle for rhombus.
 
         If ShapeStyle is not set for arc, get general ShapeStyle.
 
         Args:
             name(optional): key
 
@@ -1637,15 +1786,15 @@
 
         if name in self._shapestyles_rhombus:
             return deepcopy(self._shapestyles_rhombus[name])
         style = deepcopy(self._shapestyles[name])
         return style
 
     @error_handler
-    def shapestyle_rhombus_set(self, style: ShapeStyle, name: str = "1") -> None:
+    def shapestyle_rhombus_set(self, style: ShapeStyle, name: str = "") -> None:
         """Set theme ShapeStyle for rhombus.
 
         Args:
             style: theme ShapeStyle for rhombus
             name(optional): key
 
         Returns:
@@ -1653,15 +1802,15 @@
 
         """
 
         ArgValidator.validate_shapestyle("style", style)
         ArgValidator.validate_str("name", name)
         self._shapestyles_rhombus[name] = deepcopy(style)
 
-    def shapestyle_rhombus_has(self, name: str = "1") -> bool:
+    def shapestyle_rhombus_has(self, name: str = "") -> bool:
         """Check having theme ShapeStyle for rhombus.
 
         Args:
             name(option): key
 
         Returns:
             bool
@@ -1679,15 +1828,15 @@
         """
 
         return list(self._shapestyles_rhombus.keys())
 
     # chevron
 
     @error_handler
-    def shapestyle_chevron_get(self, name: str = "1") -> ShapeStyle:
+    def shapestyle_chevron_get(self, name: str = "") -> ShapeStyle:
         """Get theme ShapeStyle for chevron.
 
         If ShapeStyle is not set for arc, get general ShapeStyle.
 
         Args:
             name(optional): key
 
@@ -1698,15 +1847,15 @@
 
         if name in self._shapestyles_chevron:
             return deepcopy(self._shapestyles_chevron[name])
         style = deepcopy(self._shapestyles[name])
         return style
 
     @error_handler
-    def shapestyle_chevron_set(self, style: ShapeStyle, name: str = "1") -> None:
+    def shapestyle_chevron_set(self, style: ShapeStyle, name: str = "") -> None:
         """Set theme ShapeStyle for chevron.
 
         Args:
             style: theme ShapeStyle for chevron
             name(optional): key
 
         Returns:
@@ -1714,15 +1863,15 @@
 
         """
 
         ArgValidator.validate_shapestyle("style", style)
         ArgValidator.validate_str("name", name)
         self._shapestyles_chevron[name] = deepcopy(style)
 
-    def shapestyle_chevron_has(self, name: str = "1") -> bool:
+    def shapestyle_chevron_has(self, name: str = "") -> bool:
         """Check having theme ShapeStyle for chevron.
 
         Args:
             name(option): key
 
         Returns:
             bool
@@ -1740,15 +1889,15 @@
         """
 
         return list(self._shapestyles_chevron.keys())
 
     # star
 
     @error_handler
-    def shapestyle_star_get(self, name: str = "1") -> ShapeStyle:
+    def shapestyle_star_get(self, name: str = "") -> ShapeStyle:
         """Get theme ShapeStyle for star.
 
         If ShapeStyle is not set for arc, get general ShapeStyle.
 
         Args:
             name(optional): key
 
@@ -1759,15 +1908,15 @@
 
         if name in self._shapestyles_star:
             return deepcopy(self._shapestyles_star[name])
         style = deepcopy(self._shapestyles[name])
         return style
 
     @error_handler
-    def shapestyle_star_set(self, style: ShapeStyle, name: str = "1") -> None:
+    def shapestyle_star_set(self, style: ShapeStyle, name: str = "") -> None:
         """Set theme ShapeStyle for star.
 
         Args:
             style: theme ShapeStyle for star
             name(optional): key
 
         Returns:
@@ -1775,15 +1924,15 @@
 
         """
 
         ArgValidator.validate_shapestyle("style", style)
         ArgValidator.validate_str("name", name)
         self._shapestyles_star[name] = deepcopy(style)
 
-    def shapestyle_star_has(self, name: str = "1") -> bool:
+    def shapestyle_star_has(self, name: str = "") -> bool:
         """Check having theme ShapeStyle for star.
 
         Args:
             name(option): key
 
         Returns:
             bool
@@ -1798,115 +1947,14 @@
         Returns:
             List[str]: names
 
         """
 
         return list(self._shapestyles_star.keys())
 
-    ###############
-    ### Private ###
-    ###############
-
-    def _apply_thema_styles(
-        self,
-        background: Union[Tuple[int, int, int], Tuple[int, int, int, float]],
-        sourcecode_font: FontSourceCode,
-        tstyle1: _ThemeStyle,
-        tstyle2: Optional[_ThemeStyle] = None,
-        tstyle3: Optional[_ThemeStyle] = None,
-        tstyle4: Optional[_ThemeStyle] = None,
-        tstyle5: Optional[_ThemeStyle] = None,
-    ) -> None:
-
-        self.theme_initialize()
-        self._background = background
-        self._sourcecode_font = sourcecode_font
-
-        tstyles: List[_ThemeStyle] = [
-            tstyle1,
-            tstyle2,
-            tstyle3,
-            tstyle4,
-            tstyle5,
-        ]
-        for i, tstyle in enumerate(tstyles, start=1):
-            name = str(i)
-            if tstyle is None:
-                if name == "1":
-                    raise ValueError('default thema style "1" must be configured.')
-                continue
-
-            self.iconstyle_set(
-                style=IconStyle(
-                    style=tstyle.icon_style,
-                    color=tstyle.icon_color,
-                ),
-                name=name,
-            )
-            self.imagestyle_set(
-                style=ImageStyle(
-                    lstyle=tstyle.shape_line_style,
-                    lcolor=tstyle.shape_line_color,
-                ),
-                name=name,
-            )
-            self.linestyle_set(
-                style=LineStyle(
-                    style=tstyle.line_style,
-                    width=tstyle.line_width,
-                    color=tstyle.line_color,
-                ),
-                name=name,
-            )
-
-            self.linearrowstyle_set(
-                style=LineArrowStyle(
-                    lstyle=tstyle.line_style,
-                    lwidth=tstyle.line_width,
-                    hstyle=tstyle.arrowhead_style,
-                    hscale=tstyle.arrowhead_scale,
-                    color=tstyle.line_color,
-                ),
-                name=name,
-            )
-
-            self.textstyle_set(
-                style=TextStyle(
-                    font=tstyle.text_font,
-                    size=tstyle.text_size,
-                    color=tstyle.text_color,
-                    halign=None,  # depends on situation. keep None.
-                    valign=None,  # depends on situation. keep None.
-                ),
-                name=name,
-            )
-
-            self.shapestyle_set(
-                style=ShapeStyle(
-                    lwidth=tstyle.shape_line_width,
-                    lstyle=tstyle.shape_line_style,
-                    lcolor=tstyle.shape_line_color,
-                    fcolor=tstyle.shape_fill_color,
-                    halign=None,  # depends on situation. keep None.
-                    valign=None,  # depends on situation. keep None.
-                ),
-                name=name,
-            )
-
-            self.shapetextstyle_set(
-                style=ShapeTextStyle(
-                    font=tstyle.text_font,
-                    size=tstyle.text_size,
-                    color=tstyle.text_color,
-                    halign=None,  # depends on situation. keep None.
-                    valign=None,  # depends on situation. keep None.
-                ),
-                name=name,
-            )
-
 
 def _get_rgba_from_hex(hex_color: str) -> Tuple[int, int, int, float]:
     """
     Convert a hexadecimal color code to RGBA values.
 
     Args:
         hex_color (str): The hexadecimal color code (e.g., "#FF5733" or "#FFF").
```

### Comparing `drawlib-0.1.3/drawlib/v0_1/private/core/util.py` & `drawlib-0.1.4/drawlib/v0_1/private/core/util.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.3/drawlib/v0_1/private/core_canvas/__init__.py` & `drawlib-0.1.4/drawlib/v0_1/private/core_canvas/__init__.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.3/drawlib/v0_1/private/core_canvas/base.py` & `drawlib-0.1.4/drawlib/v0_1/private/core_canvas/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -239,21 +239,15 @@
             self._ax.set_aspect("equal")
             self._ax.axis("off")
             self._ax.margins(0, 0)
 
         def config_theme():
             if theme is None:
                 return
-
-            if theme == "default":
-                dtheme.theme_default()
-            elif theme == "gray":
-                dtheme.theme_gray()
-            else:
-                raise ValueError(f'Theme "{theme}" is not supported.')
+            dtheme.theme_apply_by_name(theme)
 
         def config_background():
             if background_color is not None:
                 self._background_color = background_color
             if background_alpha is not None:
                 self._background_alpha = background_alpha
```

### Comparing `drawlib-0.1.3/drawlib/v0_1/private/core_canvas/canvas.py` & `drawlib-0.1.4/drawlib/v0_1/private/core_canvas/canvas.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.3/drawlib/v0_1/private/core_canvas/image.py` & `drawlib-0.1.4/drawlib/v0_1/private/core_canvas/image.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     @error_handler
     def image(
         self,
         xy: Tuple[float, float],
         width: float,
         image: Union[str, Image, Dimage],
         angle: Optional[float] = None,
-        style: Optional[ImageStyle] = None,
+        style: Union[ImageStyle, str, None] = None,
     ) -> None:
         """Draw image
 
         Args:
             xy: Left bottom of image
             width: Width of image. Height is calculated automatically.
             image: Image path or image itself.
@@ -60,14 +60,16 @@
 
         ArgValidator.validate_xy("xy", xy)
         ArgValidator.validate_int("width", width)
         ArgValidator.validate_image_objects("image", image)
         if angle is not None:
             ArgValidator.validate_angle("angle", angle)
         if style is not None:
+            if isinstance(style, str):
+                style = dtheme.imagestyle_get(style)
             ArgValidator.validate_imagestyle("style", style)
 
         # standadize
 
         x, y = xy
         pimg = Dimage(image, copy=True)
         image_width, image_height = pimg.get_image_size()
```

### Comparing `drawlib-0.1.3/drawlib/v0_1/private/core_canvas/line.py` & `drawlib-0.1.4/drawlib/v0_1/private/core_canvas/line.py`

 * *Files 22% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         super().__init__()
 
     @error_handler
     def line(
         self,
         xy1: Tuple[float, float],
         xy2: Tuple[float, float],
-        style: Union[LineStyle, LineArrowStyle, None] = None,
+        style: Union[LineStyle, LineArrowStyle, str, None] = None,
     ) -> None:
         """Draw line from xy1 to xy2.
 
         Args:
             xy1: start point.
             xy2: end point.
             style(optional): LineStyle or LineArrowStyle.
@@ -64,15 +64,15 @@
 
     @error_handler
     def line_curved(
         self,
         xy1: Tuple[float, float],
         xy2: Tuple[float, float],
         bend: float,
-        style: Union[LineStyle, LineArrowStyle, None] = None,
+        style: Union[LineStyle, LineArrowStyle, str, None] = None,
     ) -> None:
         """Draw curved line from xy1 to xy2.
 
         Args:
             xy1: start point.
             xy2: end point.
             bend: additional line length between xy1 and xy2. 0 is straight.
@@ -87,14 +87,21 @@
 
         ArgValidator.validate_xy("xy1", xy1)
         ArgValidator.validate_xy("xy2", xy2)
         ArgValidator.validate_float("bend", bend)
         if not -2.0 <= bend <= 2.0:
             raise ValueError(f'Arg "bend" supports float between -2.0 ~ 2.0. But {bend} is given.')
         if style is not None:
+            if isinstance(style, str):
+                if dtheme.linestyle_has(style):
+                    style = dtheme.linestyle_get(style)
+                elif dtheme.linearrowstyle_has(style):
+                    style = dtheme.linearrowstyle_get(style)
+                else:
+                    raise Exception(f'Both LineStyle and LineArrowStyle does not have theme name "{style}"')
             ArgValidator.validate_linestyle_or_linearrowstyle("style", style)
 
         # create FancyArrowPatch
 
         style = LineUtil.get_merged_style(style, dtheme.linestyle_get(), dtheme.linearrowstyle_get())
         options = LineUtil.get_fancyarrowpatch_options(style)
         self._artists.append(
@@ -108,15 +115,15 @@
 
     @error_handler
     def line_bezier1(
         self,
         xy1: Tuple[float, float],
         cp: Tuple[float, float],
         xy2: Tuple[float, float],
-        style: Union[LineStyle, LineArrowStyle, None] = None,
+        style: Union[LineStyle, LineArrowStyle, str, None] = None,
     ) -> None:
         """Draw bezier line from xy1 to xy2. Control line via 1 control point.
 
         Args:
             xy1: start point.
             cp: control point.
             xy2: end point.
@@ -143,15 +150,15 @@
     @error_handler
     def line_bezier2(
         self,
         xy1: Tuple[float, float],
         cp1: Tuple[float, float],
         cp2: Tuple[float, float],
         xy2: Tuple[float, float],
-        style: Union[LineStyle, LineArrowStyle, None] = None,
+        style: Union[LineStyle, LineArrowStyle, str, None] = None,
     ) -> None:
         """Draw bezier line from xy1 to xy2. Control line via 2 control point.
 
         Args:
             xy1: start point.
             cp1: control point 1.
             cp2: control point 2.
@@ -177,15 +184,15 @@
             style=style,
         )
 
     @error_handler
     def lines(
         self,
         xys: List[Tuple[float, float]],
-        style: Union[LineStyle, LineArrowStyle, None] = None,
+        style: Union[LineStyle, LineArrowStyle, str, None] = None,
     ) -> None:
         """Draw line which paths provided xys.
 
         Args:
             xys: list of xy.
             style(optional): LineStyle or LineArrowStyle.
 
@@ -212,15 +219,15 @@
         path_points: List[
             Union[
                 Tuple[float, float],
                 Tuple[float, float, float, float],
                 Tuple[float, float, float, float, float, float],
             ]
         ],
-        style: Union[LineStyle, LineArrowStyle, None] = None,
+        style: Union[LineStyle, LineArrowStyle, str, None] = None,
     ) -> None:
         """Draw bezier line which paths provided path points.
 
         Args:
             xy: start point.
             path_points: path point and control points.
             style(optional): LineStyle or LineArrowStyle.
@@ -231,14 +238,21 @@
         """
 
         # validate args
 
         ArgValidator.validate_xy("xy", xy)
         ArgValidator.validate_path_points("path_points", path_points)
         if style is not None:
+            if isinstance(style, str):
+                if dtheme.linestyle_has(style):
+                    style = dtheme.linestyle_get(style)
+                elif dtheme.linearrowstyle_has(style):
+                    style = dtheme.linearrowstyle_get(style)
+                else:
+                    raise Exception(f'Both LineStyle and LineArrowStyle does not have theme name "{style}"')
             ArgValidator.validate_linestyle_or_linearrowstyle("style", style)
 
         # create Path
 
         vertices = [xy]
         codes = [Path.MOVETO]
         for p in path_points:
```

### Comparing `drawlib-0.1.3/drawlib/v0_1/private/core_canvas/original_arrow.py` & `drawlib-0.1.4/drawlib/v0_1/private/core_canvas/original_arrow.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 """Wrapper of matplotlib image draw
 
 Matplotlib is difficult for just drawing image.
 This module wraps it and provides easy to use interfaces.
 
 """
 
-from typing import Optional, List, Tuple, Literal
+from typing import Optional, List, Tuple, Literal, Union
 from drawlib.v0_1.private.util import (
     error_handler,
     get_angle,
     get_distance,
 )
 from drawlib.v0_1.private.core.model import ShapeStyle, ShapeTextStyle
 from drawlib.v0_1.private.core.util import ShapeUtil
@@ -40,15 +40,15 @@
         head_width: float,
         head_length: float,
         head_style: Literal[
             "-|>",
             "<|-",
             "<|-|>",
         ] = "-|>",
-        style: Optional[ShapeStyle] = None,
+        style: Union[ShapeStyle, str, None] = None,
         text: Optional[str] = None,
         textstyle: Optional[ShapeTextStyle] = None,
     ) -> None:
         """Draw sing and double heads arrow.
 
         Args:
             xy1: Arrow start point
@@ -76,14 +76,16 @@
         ArgValidator.validate_xy("xy2", xy2)
         ArgValidator.validate_float("tail_width", tail_width)
         ArgValidator.validate_float("head_width", head_width)
         ArgValidator.validate_float("head_length", head_length)
         if head_style not in ["-|>", "<|-", "<|-|>"]:
             raise ValueError('Arg "tail_edge" must be one of ["-|>", "<|-", "<|-|>"].')
         if style is not None:
+            if isinstance(style, str):
+                style = dtheme.shapestyle_arrow_get(style)
             ArgValidator.validate_shapestyle("style", style)
         if text is not None:
             ArgValidator.validate_str("text", text)
         if textstyle is not None:
             ArgValidator.validate_shapetextstyle("textstyle", textstyle)
 
         style = ShapeUtil.get_merged_shapestyle(style, dtheme.shapestyle_arrow_get())
```

### Comparing `drawlib-0.1.3/drawlib/v0_1/private/core_canvas/original_polygon.py` & `drawlib-0.1.4/drawlib/v0_1/private/core_canvas/original_polygon.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 Matplotlib is difficult for just drawing image.
 This module wraps it and provides easy to use interfaces.
 
 """
 
 import math
-from typing import Optional, List, Tuple, Literal
+from typing import Optional, List, Tuple, Literal, Union
 from matplotlib.text import Text
 from matplotlib.patches import Polygon
 from matplotlib.path import Path
 from matplotlib.patches import PathPatch
 
 from drawlib.v0_1.private.util import error_handler, minus_2points
 from drawlib.v0_1.private.core.model import ShapeStyle, ShapeTextStyle
@@ -36,18 +36,18 @@
     @error_handler
     def bubblespeech(
         self,
         xy: Tuple[float, float],
         width: float,
         height: float,
         tail_edge: Literal["left", "top", "right", "bottom"],
-        tail_start: float,
-        tail_vertex: Tuple[float, float],
-        tail_width: float,
-        style: Optional[ShapeStyle] = None,
+        tail_from_ratio: float,
+        tail_vertex_xy: Tuple[float, float],
+        tail_to_ratio: float,
+        style: Union[ShapeStyle, str, None] = None,
         text: Optional[str] = None,
         textstyle: Optional[ShapeTextStyle] = None,
     ) -> None:
         """Draw bubble speech.
 
         Almost same to rectangle. But having tail.
 
@@ -71,52 +71,56 @@
         # validate args
 
         ArgValidator.validate_xy("xy", xy)
         ArgValidator.validate_float("width", width)
         ArgValidator.validate_float("height", height)
         if tail_edge not in ["left", "top", "right", "bottom"]:
             raise ValueError('Arg "tail_edge" must be one of ["left", "top", "right", "bottom"].')
-        ArgValidator.validate_float("tail_start", tail_start)
-        ArgValidator.validate_xy("tail_vertex", tail_vertex)
-        ArgValidator.validate_float("tail_width", tail_width)
+        ArgValidator.validate_float("tail_from_ratio", tail_from_ratio)
+        ArgValidator.validate_xy("tail_vertex_xy", tail_vertex_xy)
+        ArgValidator.validate_float("tail_to_ratio", tail_to_ratio)
         if style is not None:
+            if isinstance(style, str):
+                style = dtheme.shapestyle_bubblespeech_get(style)
             ArgValidator.validate_shapestyle("style", style)
         if text is not None:
             ArgValidator.validate_str("text", text)
         if textstyle is not None:
             ArgValidator.validate_shapetextstyle("textstyle", textstyle)
 
-        if tail_start + tail_width > 1.0:
-            raise ValueError(f"Sum of tail_start={tail_start} and tail_width={tail_width} must be less than 1.0")
+        if tail_from_ratio > tail_to_ratio:
+            raise ValueError("tail_from_ratio must be smaller than tail_to_ratio.")
+        if tail_to_ratio > 1.0:
+            raise ValueError(f"tail_from_ratio and tail_to_ratio must be smaller than 1.0")
 
         x, y = xy
         style = ShapeUtil.get_merged_shapestyle(style, dtheme.shapestyle_bubblespeech_get())
         textstyle = ShapeUtil.get_merged_shapetextstyle(textstyle, dtheme.shapetextstyle_get())
 
         xys = []
         xys.append((x, y))  # left bottom
         if tail_edge == "left":
-            xys.append((x, y + height * tail_start))
-            xys.append(tail_vertex)
-            xys.append((x, y + height * (tail_start + tail_width)))
+            xys.append((x, y + height * tail_from_ratio))
+            xys.append(tail_vertex_xy)
+            xys.append((x, y + height * tail_to_ratio))
         xys.append((x, y + height))  # left top
         if tail_edge == "top":
-            xys.append((x + width * tail_start, y + height))
-            xys.append(tail_vertex)
-            xys.append((x + width * (tail_start + tail_width), y + height))
+            xys.append((x + width * tail_from_ratio, y + height))
+            xys.append(tail_vertex_xy)
+            xys.append((x + width * tail_to_ratio, y + height))
         xys.append((x + width, y + height))  # right top
         if tail_edge == "right":
-            xys.append((x + width, y + height * (tail_start + tail_width)))
-            xys.append(tail_vertex)
-            xys.append((x + width, y + height * tail_start))
+            xys.append((x + width, y + height * tail_to_ratio))
+            xys.append(tail_vertex_xy)
+            xys.append((x + width, y + height * tail_from_ratio))
         xys.append((x + width, y))  # right bottom
         if tail_edge == "bottom":
-            xys.append((x + width * (tail_start + tail_width), y))
-            xys.append(tail_vertex)
-            xys.append((x + width * tail_start, y))
+            xys.append((x + width * tail_to_ratio, y))
+            xys.append(tail_vertex_xy)
+            xys.append((x + width * tail_from_ratio, y))
 
         options = ShapeUtil.get_shape_options(style)
         self._artists.append(Polygon(xy=xys, closed=True, **options))
 
         if text:
             center_x = x + width / 2
             center_y = y + height / 2
@@ -130,27 +134,27 @@
             )
 
     def triangle(
         self,
         xy: Tuple[float, float],
         width: float,
         height: float,
-        topvertex_start: Optional[float] = None,
+        topvertex_x: Optional[float] = None,
         angle: Optional[float] = None,
-        style: Optional[ShapeStyle] = None,
+        style: Union[ShapeStyle, str, None] = None,
         text: Optional[str] = None,
         textstyle: Optional[ShapeTextStyle] = None,
     ) -> None:
         """Draw triangle.
 
         Args:
             xy: default left bottom.
             width: width of triangle bottom
             height: height of traiangle
-            topvertex_start(option): topvertex location from left side. default is center.
+            topvertex_x(option): topvertex x coordinate from left side. default make it center.
             angle(optional): rotate degree
             style(optional): style of shape.
             text(optional): center text.
             textstyle(optional): style of text.
 
         Returns:
             None
@@ -158,34 +162,36 @@
         """
 
         # validate args
 
         ArgValidator.validate_xy("xy", xy)
         ArgValidator.validate_float("width", width)
         ArgValidator.validate_float("height", height)
-        if topvertex_start is not None:
-            ArgValidator.validate_float("topvertex_width", topvertex_start)
+        if topvertex_x is not None:
+            ArgValidator.validate_float("topvertex_x", topvertex_x)
         if angle is not None:
             ArgValidator.validate_angle("angle", angle)
         if style is not None:
+            if isinstance(style, str):
+                style = dtheme.shapestyle_triangle_get(style)
             ArgValidator.validate_shapestyle("style", style)
         if text is not None:
             ArgValidator.validate_str("text", text)
         if textstyle is not None:
             ArgValidator.validate_shapetextstyle("textstyle", textstyle)
 
         # apply default if styles are not specified
 
         style = ShapeUtil.get_merged_shapestyle(style, dtheme.shapestyle_triangle_get())
         textstyle = ShapeUtil.get_merged_shapetextstyle(textstyle, dtheme.shapetextstyle_get())
 
-        if topvertex_start is None:
-            topvertex_start = width / 2
+        if topvertex_x is None:
+            topvertex_x = width / 2
         p1 = (0, 0)
-        p2 = (topvertex_start, height)
+        p2 = (topvertex_x, height)
         p3 = (width, 0)
         self.shape(
             xy=xy,
             path_points=[p1, p2, p3],
             angle=angle,
             style=style,
             text=text,
@@ -195,15 +201,15 @@
     def parallelogram(
         self,
         xy: Tuple[float, float],
         width: float,
         height: float,
         corner_angle: float,
         angle: Optional[float] = None,
-        style: Optional[ShapeStyle] = None,
+        style: Union[ShapeStyle, str, None] = None,
         text: Optional[str] = None,
         textstyle: Optional[ShapeTextStyle] = None,
     ):
         """Draw parallelogram.
 
         Args:
             xy: default left bottom.
@@ -225,14 +231,16 @@
         ArgValidator.validate_xy("xy", xy)
         ArgValidator.validate_float("width", width)
         ArgValidator.validate_float("height", height)
         ArgValidator.validate_float("corner_angle", corner_angle)
         if angle is not None:
             ArgValidator.validate_angle("angle", angle)
         if style is not None:
+            if isinstance(style, str):
+                style = dtheme.shapestyle_parallelogram_get(style)
             ArgValidator.validate_shapestyle("style", style)
         if text is not None:
             ArgValidator.validate_str("text", text)
         if textstyle is not None:
             ArgValidator.validate_shapetextstyle("textstyle", textstyle)
 
         # apply default if styles are not specified
@@ -259,68 +267,70 @@
             textstyle=textstyle,
         )
 
     def trapezoid(
         self,
         xy: Tuple[float, float],
         height: float,
-        bottom_width: float,
-        top_width: float,
-        top_start: Optional[float] = None,
+        bottomedge_width: float,
+        topedge_width: float,
+        topedge_x: Optional[float] = None,
         angle: Optional[float] = None,
-        style: Optional[ShapeStyle] = None,
+        style: Union[ShapeStyle, str, None] = None,
         text: Optional[str] = None,
         textstyle: Optional[ShapeTextStyle] = None,
     ):
         """Draw triangle.
 
         Args:
             xy: default left bottom.
             height: height of traiangle
-            bottom_width: width of bottom
-            top_width: width of top
-            top_start(optional): start point of top. Default makes top center.
+            bottomedge_width: width of bottom
+            topedge_width: width of top
+            topedge_x(optional): start point of top edge. Default makes top edge center.
             angle(optional): rotate degree
             style(optional): style of shape.
             text(optional): center text.
             textstyle(optional): style of text.
 
         Returns:
             None
 
         """
 
         # validate args
 
         ArgValidator.validate_xy("xy", xy)
         ArgValidator.validate_float("height", height)
-        ArgValidator.validate_float("bottom_width", bottom_width)
-        ArgValidator.validate_float("top_width", top_width)
-        if top_start is not None:
-            ArgValidator.validate_float("topvertex_width", top_start)
+        ArgValidator.validate_float("bottomedge_width", bottomedge_width)
+        ArgValidator.validate_float("topedge_width", topedge_width)
+        if topedge_x is not None:
+            ArgValidator.validate_float("topedge_xstart", topedge_x)
         if angle is not None:
             ArgValidator.validate_angle("angle", angle)
         if style is not None:
+            if isinstance(style, str):
+                style = dtheme.shapestyle_trapezoid_get(style)
             ArgValidator.validate_shapestyle("style", style)
         if text is not None:
             ArgValidator.validate_str("text", text)
         if textstyle is not None:
             ArgValidator.validate_shapetextstyle("textstyle", textstyle)
 
         # apply default if styles are not specified
 
         style = ShapeUtil.get_merged_shapestyle(style, dtheme.shapestyle_trapezoid_get())
         textstyle = ShapeUtil.get_merged_shapetextstyle(textstyle, dtheme.shapetextstyle_get())
 
-        if top_start is None:
-            top_start = (bottom_width - top_width) / 2
+        if topedge_x is None:
+            topedge_x = (bottomedge_width - topedge_width) / 2
         p1 = (0, 0)
-        p2 = (top_start, height)
-        p3 = (top_start + top_width, height)
-        p4 = (bottom_width, 0)
+        p2 = (topedge_x, height)
+        p3 = (topedge_x + topedge_width, height)
+        p4 = (bottomedge_width, 0)
 
         self.shape(
             xy=xy,
             path_points=[p1, p2, p3, p4],
             angle=angle,
             style=style,
             text=text,
@@ -329,15 +339,15 @@
 
     def rhombus(
         self,
         xy: Tuple[float, float],
         width: float,
         height: float,
         angle: Optional[float] = None,
-        style: Optional[ShapeStyle] = None,
+        style: Union[ShapeStyle, str, None] = None,
         text: Optional[str] = None,
         textstyle: Optional[ShapeTextStyle] = None,
     ):
         """Draw rhombus.
 
         Args:
             xy: default left bottom.
@@ -357,14 +367,16 @@
 
         ArgValidator.validate_xy("xy", xy)
         ArgValidator.validate_float("width", width)
         ArgValidator.validate_float("height", height)
         if angle is not None:
             ArgValidator.validate_angle("angle", angle)
         if style is not None:
+            if isinstance(style, str):
+                style = dtheme.shapestyle_rhombus_get(style)
             ArgValidator.validate_shapestyle("style", style)
         if text is not None:
             ArgValidator.validate_str("text", text)
         if textstyle is not None:
             ArgValidator.validate_shapetextstyle("textstyle", textstyle)
 
         style = ShapeUtil.get_merged_shapestyle(style, dtheme.shapestyle_rhombus_get())
@@ -388,15 +400,15 @@
         self,
         xy: Tuple[float, float],
         width: float,
         height: float,
         corner_angle: float,
         mirror: bool = False,
         angle: Optional[float] = None,
-        style: Optional[ShapeStyle] = None,
+        style: Union[ShapeStyle, str, None] = None,
         text: Optional[str] = None,
         textstyle: Optional[ShapeTextStyle] = None,
     ) -> None:
         """Draw chevron.
 
         Vertex is right on default. Provide True for mirror makes left side vertex.
 
@@ -424,14 +436,16 @@
         ArgValidator.validate_float("corner_angle", corner_angle)
         if not 0.0 <= corner_angle <= 90.0:
             raise ValueError(f"corner_angles supports 0.0 ~ 90.0. But {corner_angle} is given.")
         ArgValidator.validate_bool("mirror", mirror)
         if angle is not None:
             ArgValidator.validate_angle("angle", angle)
         if style is not None:
+            if isinstance(style, str):
+                style = dtheme.shapestyle_chevron_get(style)
             ArgValidator.validate_shapestyle("style", style)
         if text is not None:
             ArgValidator.validate_str("text", text)
         if textstyle is not None:
             ArgValidator.validate_shapetextstyle("textstyle", textstyle)
 
         style = ShapeUtil.get_merged_shapestyle(style, dtheme.shapestyle_chevron_get())
@@ -460,15 +474,15 @@
     def star(
         self,
         xy: Tuple[float, float],
         num_vertex: int,
         radius_ext: float,
         radius_int: float,
         angle: Optional[float] = None,
-        style: Optional[ShapeStyle] = None,
+        style: Union[ShapeStyle, str, None] = None,
         text: Optional[str] = None,
         textstyle: Optional[ShapeTextStyle] = None,
     ) -> None:
         """Draw star.
 
         Args:
             xy: default center, center.
@@ -490,14 +504,16 @@
         ArgValidator.validate_xy("xy", xy)
         ArgValidator.validate_int("num_vertex", num_vertex)
         ArgValidator.validate_float("radius_ext", radius_ext)
         ArgValidator.validate_float("radius_int", radius_int)
         if angle is not None:
             ArgValidator.validate_angle("angle", angle)
         if style is not None:
+            if isinstance(style, str):
+                style = dtheme.shapestyle_star_get(style)
             ArgValidator.validate_shapestyle("style", style)
         if text is not None:
             ArgValidator.validate_str("text", text)
         if textstyle is not None:
             ArgValidator.validate_shapetextstyle("textstyle", textstyle)
 
         if num_vertex < 3:
```

### Comparing `drawlib-0.1.3/drawlib/v0_1/private/core_canvas/patches.py` & `drawlib-0.1.4/drawlib/v0_1/private/core_canvas/patches.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 This module wraps it and provides easy to use interfaces.
 
 """
 
 # pylint: disable=too-many-arguments
 # pylint: disable=too-many-locals
 
-from typing import Optional, List, Tuple
+from typing import Optional, List, Tuple, Union
 import math
 from matplotlib.patches import (
     Arc,
     Circle,
     Ellipse,
     Polygon,
     RegularPolygon,
@@ -45,29 +45,29 @@
 
     @error_handler
     def arc(
         self,
         xy: Tuple[float, float],
         width: float,
         height: float,
-        theta_begin: int = 0,
-        theta_end: int = 360,
+        from_angle: int = 0,
+        to_angle: int = 360,
         angle: Optional[float] = None,
-        style: Optional[ShapeStyle] = None,
+        style: Union[ShapeStyle, str, None] = None,
         text: Optional[str] = None,
         textstyle: Optional[ShapeTextStyle] = None,
     ) -> None:
         """Draw arc.
 
         Args:
             xy: center of arc.
             width: width of arc.
             height: height of arc.
-            theta_begin(optional): where drawing arc start. default is angle 0.0
-            theta_end(optional): where drawing arc end. default is angle 360.0
+            from_angle(optional): where drawing arc start. default is angle 0.0
+            to_angle(optional): where drawing arc end. default is angle 360.0
             angle(optional): rotate arc with specified angle
             style(optional): style of arc.
             text(optional): text which is shown at center of arc.
             textstyle(optional): style of text.
 
         Returns:
             None.
@@ -75,19 +75,21 @@
         """
 
         # validate args
 
         ArgValidator.validate_xy("xy", xy)
         ArgValidator.validate_float("width", width)
         ArgValidator.validate_float("height", height)
-        ArgValidator.validate_angle("theta_begin", theta_begin)
-        ArgValidator.validate_angle("theta_end", theta_end)
+        ArgValidator.validate_angle("from_angle", from_angle)
+        ArgValidator.validate_angle("to_angle", to_angle)
         if angle is not None:
             ArgValidator.validate_angle("angle", angle)
         if style is not None:
+            if isinstance(style, str):
+                style = dtheme.shapestyle_arc_get(style)
             ArgValidator.validate_shapestyle("style", style)
         if text is not None:
             ArgValidator.validate_str("text", text)
         if textstyle is not None:
             ArgValidator.validate_shapetextstyle("textstyle", textstyle)
 
         # apply default if style not specified
@@ -101,29 +103,29 @@
         options = ShapeUtil.get_shape_options(style, default_no_line=False)
         self._artists.append(
             Arc(
                 xy,
                 width=width,
                 height=height,
                 angle=angle,
-                theta1=theta_begin,
-                theta2=theta_end,
+                theta1=from_angle,
+                theta2=to_angle,
                 **options,
             )
         )
         if text:
             self._artists.append(ShapeUtil.get_shape_text(xy=xy, text=text, angle=angle, style=textstyle))
 
     @error_handler
     def circle(
         self,
         xy: Tuple[float, float],
         radius: float,
         angle: Optional[float] = None,
-        style: Optional[ShapeStyle] = None,
+        style: Union[ShapeStyle, str, None] = None,
         text: Optional[str] = None,
         textstyle: Optional[ShapeTextStyle] = None,
     ) -> None:
         """Draw cicle.
 
         Args:
             xy: center of circle.
@@ -141,14 +143,16 @@
         # validate args
 
         ArgValidator.validate_xy("xy", xy)
         ArgValidator.validate_float("radius", radius)
         if angle is not None:
             ArgValidator.validate_angle("angle", angle)
         if style is not None:
+            if isinstance(style, str):
+                style = dtheme.shapestyle_circle_get(style)
             ArgValidator.validate_shapestyle("style", style)
         if text is not None:
             ArgValidator.validate_str("text", text)
         if textstyle is not None:
             ArgValidator.validate_shapetextstyle("textstyle", textstyle)
 
         style = ShapeUtil.get_merged_shapestyle(style, dtheme.shapestyle_circle_get())
@@ -164,15 +168,15 @@
     @error_handler
     def ellipse(
         self,
         xy: Tuple[float, float],
         width: float,
         height: float,
         angle: Optional[float] = None,
-        style: Optional[ShapeStyle] = None,
+        style: Union[ShapeStyle, str, None] = None,
         text: Optional[str] = None,
         textstyle: Optional[ShapeTextStyle] = None,
     ) -> None:
         """Draw ellipse
 
         Args:
             xy: center of ellipse
@@ -192,14 +196,16 @@
 
         ArgValidator.validate_xy("xy", xy)
         ArgValidator.validate_float("width", width)
         ArgValidator.validate_float("height", height)
         if angle is not None:
             ArgValidator.validate_angle("angle", angle)
         if style is not None:
+            if isinstance(style, str):
+                style = dtheme.shapestyle_ellipse_get(style)
             ArgValidator.validate_shapestyle("style", style)
         if text is not None:
             ArgValidator.validate_str("text", text)
         if textstyle is not None:
             ArgValidator.validate_shapetextstyle("textstyle", textstyle)
 
         # apply default if styles are not specified
@@ -214,15 +220,15 @@
         if text:
             self._artists.append(ShapeUtil.get_shape_text(xy=xy, text=text, angle=angle, style=textstyle))
 
     @error_handler
     def polygon(
         self,
         xys: List[Tuple[float, float]],
-        style: Optional[ShapeStyle] = None,
+        style: Union[ShapeStyle, str, None] = None,
         text: Optional[str] = None,
         textstyle: Optional[ShapeTextStyle] = None,
     ) -> None:
         """Draw polygon.
 
         Args:
             xys: List of points. [(x1, y1), ...(x_n, y_n)].
@@ -235,14 +241,16 @@
 
         """
 
         # validate args
 
         ArgValidator.validate_xys("xys", xys)
         if style is not None:
+            if isinstance(style, str):
+                style = dtheme.shapestyle_polygon_get(style)
             ArgValidator.validate_shapestyle("style", style)
         if text is not None:
             ArgValidator.validate_str("text", text)
         if textstyle is not None:
             ArgValidator.validate_shapetextstyle("textstyle", textstyle)
 
         style = ShapeUtil.get_merged_shapestyle(style, dtheme.shapestyle_polygon_get())
@@ -259,15 +267,15 @@
     @error_handler
     def regularpolygon(
         self,
         xy: Tuple[float, float],
         radius: float,
         num_vertex: int,
         angle: Optional[float] = None,
-        style: Optional[ShapeStyle] = None,
+        style: Union[ShapeStyle, str, None] = None,
         text: Optional[str] = None,
         textstyle: Optional[ShapeTextStyle] = None,
     ) -> None:
         """Draw regular polygon.
 
         Args:
             xy: center of regular polygon
@@ -285,14 +293,16 @@
 
         ArgValidator.validate_xy("xy", xy)
         ArgValidator.validate_float("radius", radius)
         ArgValidator.validate_int("num_vertex", num_vertex)
         if angle is not None:
             ArgValidator.validate_angle("angle", angle)
         if style is not None:
+            if isinstance(style, str):
+                style = dtheme.shapestyle_regularpolygon_get(style)
             ArgValidator.validate_shapestyle("style", style)
         if text is not None:
             ArgValidator.validate_str("text", text)
         if textstyle is not None:
             ArgValidator.validate_shapetextstyle("textstyle", textstyle)
 
         style = ShapeUtil.get_merged_shapestyle(style, dtheme.shapestyle_regularpolygon_get())
@@ -320,15 +330,15 @@
     def rectangle(
         self,
         xy: Tuple[float, float],
         width: float,
         height: float,
         r: float = 0.0,
         angle: Optional[float] = None,
-        style: Optional[ShapeStyle] = None,
+        style: Union[ShapeStyle, str, None] = None,
         text: Optional[str] = None,
         textstyle: Optional[ShapeTextStyle] = None,
     ) -> None:
         """Draw rectangle
 
         Args:
             xy: left bottom of rectangle.
@@ -350,14 +360,16 @@
         ArgValidator.validate_xy("xy", xy)
         ArgValidator.validate_float("width", width)
         ArgValidator.validate_float("height", height)
         ArgValidator.validate_float("r", r)
         if angle is not None:
             ArgValidator.validate_angle("angle", angle)
         if style is not None:
+            if isinstance(style, str):
+                style = dtheme.shapestyle_rectangle_get(style)
             ArgValidator.validate_shapestyle("style", style)
         if text is not None:
             ArgValidator.validate_str("text", text)
         if textstyle is not None:
             ArgValidator.validate_shapetextstyle("textstyle", textstyle)
 
         # apply default if styles are not specified
@@ -394,29 +406,29 @@
 
     @error_handler
     def wedge(
         self,
         xy: Tuple[float, float],
         radius: float,
         width: Optional[float] = None,
-        theta_begin: float = 0,
-        theta_end: float = 360,
+        from_angle: float = 0,
+        to_angle: float = 360,
         angle: Optional[float] = None,
-        style: Optional[ShapeStyle] = None,
+        style: Union[ShapeStyle, str, None] = None,
         text: Optional[str] = None,
         textstyle: Optional[ShapeTextStyle] = None,
     ) -> None:
         """Draw wedge
 
         Args:
             xy: center of wedge
             radius: radius of wedge.
             width(optional): length from outer to inner circumference. default is same to radius value.
-            theta_begin(optional): where drawing arc start. default is angle 0.0
-            theta_end(optional): where drawing arc end. default is angle 360.0
+            from_angle(optional): where drawing arc start. default is angle 0.0
+            to_angle(optional): where drawing arc end. default is angle 360.0
             angle(optional): rotate wedge with specified angle
             style(optional): style of wedge.
             text(optional): text which is shown at center of wedge.
             textstyle(optional): style of text.
 
         Returns:
             None.
@@ -425,19 +437,21 @@
 
         # validate args
 
         ArgValidator.validate_xy("xy", xy)
         ArgValidator.validate_float("radius", radius)
         if width is not None:
             ArgValidator.validate_float("width", width)
-        ArgValidator.validate_angle("theta_begin", theta_begin)
-        ArgValidator.validate_angle("theta_end", theta_end)
+        ArgValidator.validate_angle("from_angle", from_angle)
+        ArgValidator.validate_angle("to_angle", to_angle)
         if angle is not None:
             ArgValidator.validate_angle("angle", angle)
         if style is not None:
+            if isinstance(style, str):
+                style = dtheme.shapestyle_wedge_get(style)
             ArgValidator.validate_shapestyle("style", style)
         if text is not None:
             ArgValidator.validate_str("text", text)
         if textstyle is not None:
             ArgValidator.validate_shapetextstyle("textstyle", textstyle)
 
         # apply default if style not specified
@@ -452,31 +466,31 @@
 
         options = ShapeUtil.get_shape_options(style)
         self._artists.append(
             Wedge(
                 center=xy,
                 r=radius,
                 width=width,  # None makes no hole
-                theta1=theta_begin + angle,
-                theta2=theta_end + angle,
+                theta1=from_angle + angle,
+                theta2=to_angle + angle,
                 **options,
             )
         )
 
         if text:
             self._artists.append(ShapeUtil.get_shape_text(xy=xy, text=text, angle=angle, style=textstyle))
 
     @error_handler
     def donuts(
         self,
         xy: Tuple[float, float],
         radius: float,
         width: Optional[float] = None,
         angle: Optional[float] = None,
-        style: Optional[ShapeStyle] = None,
+        style: Union[ShapeStyle, str, None] = None,
         text: Optional[str] = None,
         textstyle: Optional[ShapeTextStyle] = None,
     ) -> None:
         """Draw donuts
 
         Args:
             xy: center of donuts
@@ -487,14 +501,20 @@
             text(optional): text which is shown at center of wedge.
             textstyle(optional): style of text.
 
         Returns:
             None.
 
         """
+
+        if style is not None:
+            if isinstance(style, str):
+                style = dtheme.shapestyle_donuts_get(style)
+            ArgValidator.validate_shapestyle("style", style)
+
         style = ShapeUtil.get_merged_shapestyle(style, dtheme.shapestyle_donuts_get())
         textstyle = ShapeUtil.get_merged_shapetextstyle(textstyle, dtheme.shapetextstyle_get())
         self.wedge(
             xy=xy,
             radius=radius,
             width=width,
             angle=angle,
@@ -504,44 +524,49 @@
         )
 
     @error_handler
     def fan(
         self,
         xy: Tuple[float, float],
         radius: float,
-        theta_begin: float = 0,
-        theta_end: float = 180,
+        from_angle: float = 0,
+        to_angle: float = 180,
         angle: Optional[float] = None,
-        style: Optional[ShapeStyle] = None,
+        style: Union[ShapeStyle, str, None] = None,
         text: Optional[str] = None,
         textstyle: Optional[ShapeTextStyle] = None,
     ) -> None:
         """Draw fan
 
         Args:
             xy: center of fan
             radius: radius of fan.
-            theta_begin(optional): where drawing arc start. default is angle 0.0
-            theta_end(optional): where drawing arc end. default is angle 360.0
+            from_angle(optional): where drawing arc start. default is angle 0.0
+            to_angle(optional): where drawing arc end. default is angle 360.0
             angle(optional): rotate wedge with specified angle
             style(optional): style of wedge.
             text(optional): text which is shown at center of wedge.
             textstyle(optional): style of text.
 
         Returns:
             None.
 
         """
 
+        if style is not None:
+            if isinstance(style, str):
+                style = dtheme.shapestyle_fan_get(style)
+            ArgValidator.validate_shapestyle("style", style)
+
         style = ShapeUtil.get_merged_shapestyle(style, dtheme.shapestyle_fan_get())
         textstyle = ShapeUtil.get_merged_shapetextstyle(textstyle, dtheme.shapetextstyle_get())
         self.wedge(
             xy=xy,
             radius=radius,
             width=None,
-            theta_begin=theta_begin,
-            theta_end=theta_end,
+            from_angle=from_angle,
+            to_angle=to_angle,
             angle=angle,
             style=style,
             text=text,
             textstyle=textstyle,
         )
```

### Comparing `drawlib-0.1.3/drawlib/v0_1/private/core_canvas/text.py` & `drawlib-0.1.4/drawlib/v0_1/private/core_canvas/text.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.3/drawlib/v0_1/private/download.py` & `drawlib-0.1.4/drawlib/v0_1/private/download.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.3/drawlib/v0_1/private/dutil.py` & `drawlib-0.1.4/drawlib/v0_1/private/dutil.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.3/drawlib/v0_1/private/icons/__init__.py` & `drawlib-0.1.4/drawlib/v0_1/private/icons/__init__.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.3/drawlib/v0_1/private/icons/phosphor.py` & `drawlib-0.1.4/drawlib/v0_1/private/icons/phosphor.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 import typing
 import urllib.parse
 import drawlib.assets.v0_1.fonticons
 import drawlib.v0_1.private.core.model
 import drawlib.v0_1.private.icons.util
 import drawlib.v0_1.private.util
 import drawlib.v0_1.private.download
+import drawlib.v0_1.private.core.theme
 
 
 def _get_fontfile_tuple(path: str, md5_hash: str) -> typing.Tuple[str, str, str]:
     paths = [p for p in path.split("/") if p]
 
     # font path
     dir_path = os.path.dirname(drawlib.assets.v0_1.fonticons.__file__)
@@ -61,40 +62,64 @@
 
 
 def _write(
     xy: typing.Tuple[float, float],
     width: float,
     code: str,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
+
     DEFAULT_STYLE = "thin"
+
+    # None, str -> IconStyle
     if style is None:
-        file = _get_font_path(DEFAULT_STYLE)
-    elif style.style is None:
-        file = _get_font_path(DEFAULT_STYLE)
+        style = drawlib.v0_1.private.core.theme.dtheme.iconstyle_get()
+    elif isinstance(style, str):
+        style = drawlib.v0_1.private.core.theme.dtheme.iconstyle_get(style)
+    elif isinstance(style, drawlib.v0_1.private.core.model.IconStyle):
+        ...
     else:
-        if style.style not in ["thin", "light", "regular", "bold", "fill"]:
-            raise ValueError(f'dicon_phosphor does not support style "{style.style}".')
-        file = _get_font_path(style.style)
-
-    drawlib.v0_1.private.icons.util.icon(xy=xy, width=width, code=code, file=file, angle=angle, style=style)
+        raise ValueError(
+            f'Unsupported type "{type(style)}" is passed to arg style. ' "Supports only IconStyle, str, None."
+        )
+
+    # set IconStyle.Style if it is None
+    if style.style is None:
+        style.style = DEFAULT_STYLE
+
+    # validate IconStyle.Style
+    if style.style not in ["thin", "light", "regular", "bold", "fill"]:
+        raise ValueError(f'icon_phosphor does not support style "{style.style}".')
+
+    # set icon file path
+    file = _get_font_path(style.style)
+
+    # draw phosphor icon with generic function
+    drawlib.v0_1.private.icons.util.icon(
+        xy=xy,
+        width=width,
+        code=code,
+        file=file,
+        angle=angle,
+        style=style,
+    )
 
 
 #####################################
 ### Auto generated code from here ###
 #####################################
 
 
 @drawlib.v0_1.private.util.error_handler
 def acorn(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon acorn. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -109,15 +134,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def address_book(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon address-book. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -132,15 +157,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def address_book_tabs(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon address-book-tabs. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -155,15 +180,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def air_traffic_control(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon air-traffic-control. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -178,15 +203,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def airplane(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon airplane. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -201,15 +226,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def airplane_in_flight(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon airplane-in-flight. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -224,15 +249,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def airplane_landing(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon airplane-landing. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -247,15 +272,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def airplane_takeoff(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon airplane-takeoff. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -270,15 +295,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def airplane_taxiing(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon airplane-taxiing. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -293,15 +318,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def airplane_tilt(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon airplane-tilt. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -316,15 +341,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def airplay(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon airplay. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -339,15 +364,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def alarm(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon alarm. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -362,15 +387,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def alien(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon alien. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -385,15 +410,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def align_bottom(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon align-bottom. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -408,15 +433,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def align_bottom_simple(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon align-bottom-simple. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -431,15 +456,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def align_center_horizontal(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon align-center-horizontal. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -454,15 +479,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def align_center_horizontal_simple(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon align-center-horizontal-simple. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -477,15 +502,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def align_center_vertical(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon align-center-vertical. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -500,15 +525,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def align_center_vertical_simple(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon align-center-vertical-simple. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -523,15 +548,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def align_left(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon align-left. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -546,15 +571,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def align_left_simple(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon align-left-simple. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -569,15 +594,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def align_right(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon align-right. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -592,15 +617,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def align_right_simple(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon align-right-simple. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -615,15 +640,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def align_top(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon align-top. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -638,15 +663,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def align_top_simple(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon align-top-simple. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -661,15 +686,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def amazon_logo(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon amazon-logo. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -684,15 +709,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def ambulance(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon ambulance. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -707,15 +732,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def anchor(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon anchor. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -730,15 +755,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def anchor_simple(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon anchor-simple. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -753,15 +778,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def android_logo(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon android-logo. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -776,15 +801,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def angle(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon angle. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -799,15 +824,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def angular_logo(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon angular-logo. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -822,15 +847,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def aperture(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon aperture. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -845,15 +870,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def app_store_logo(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon app-store-logo. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -868,15 +893,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def app_window(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon app-window. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -891,15 +916,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def apple_logo(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon apple-logo. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -914,15 +939,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def apple_podcasts_logo(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon apple-podcasts-logo. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -937,15 +962,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def approximate_equals(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon approximate-equals. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -960,15 +985,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def archive(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon archive. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -983,15 +1008,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def armchair(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon armchair. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -1006,15 +1031,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def arrow_arc_left(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon arrow-arc-left. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -1029,15 +1054,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def arrow_arc_right(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon arrow-arc-right. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -1052,15 +1077,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def arrow_bend_double_up_left(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon arrow-bend-double-up-left. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -1075,15 +1100,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def arrow_bend_double_up_right(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon arrow-bend-double-up-right. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -1098,15 +1123,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def arrow_bend_down_left(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon arrow-bend-down-left. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -1121,15 +1146,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def arrow_bend_down_right(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon arrow-bend-down-right. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -1144,15 +1169,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def arrow_bend_left_down(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon arrow-bend-left-down. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -1167,15 +1192,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def arrow_bend_left_up(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon arrow-bend-left-up. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -1190,15 +1215,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def arrow_bend_right_down(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon arrow-bend-right-down. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -1213,15 +1238,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def arrow_bend_right_up(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon arrow-bend-right-up. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -1236,15 +1261,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def arrow_bend_up_left(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon arrow-bend-up-left. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -1259,15 +1284,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def arrow_bend_up_right(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon arrow-bend-up-right. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -1282,15 +1307,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def arrow_circle_down(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon arrow-circle-down. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -1305,15 +1330,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def arrow_circle_down_left(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon arrow-circle-down-left. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -1328,15 +1353,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def arrow_circle_down_right(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon arrow-circle-down-right. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -1351,15 +1376,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def arrow_circle_left(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon arrow-circle-left. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -1374,15 +1399,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def arrow_circle_right(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon arrow-circle-right. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -1397,15 +1422,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def arrow_circle_up(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon arrow-circle-up. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -1420,15 +1445,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def arrow_circle_up_left(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon arrow-circle-up-left. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -1443,15 +1468,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def arrow_circle_up_right(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon arrow-circle-up-right. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -1466,15 +1491,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def arrow_clockwise(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon arrow-clockwise. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -1489,15 +1514,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def arrow_counter_clockwise(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon arrow-counter-clockwise. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -1512,15 +1537,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def arrow_down(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon arrow-down. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -1535,15 +1560,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def arrow_down_left(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon arrow-down-left. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -1558,15 +1583,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def arrow_down_right(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon arrow-down-right. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -1581,15 +1606,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def arrow_elbow_down_left(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon arrow-elbow-down-left. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -1604,15 +1629,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def arrow_elbow_down_right(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon arrow-elbow-down-right. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -1627,15 +1652,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def arrow_elbow_left(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon arrow-elbow-left. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -1650,15 +1675,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def arrow_elbow_left_down(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon arrow-elbow-left-down. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -1673,15 +1698,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def arrow_elbow_left_up(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon arrow-elbow-left-up. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -1696,15 +1721,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def arrow_elbow_right(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon arrow-elbow-right. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -1719,15 +1744,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def arrow_elbow_right_down(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon arrow-elbow-right-down. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -1742,15 +1767,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def arrow_elbow_right_up(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon arrow-elbow-right-up. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -1765,15 +1790,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def arrow_elbow_up_left(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon arrow-elbow-up-left. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -1788,15 +1813,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def arrow_elbow_up_right(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon arrow-elbow-up-right. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -1811,15 +1836,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def arrow_fat_down(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon arrow-fat-down. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -1834,15 +1859,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def arrow_fat_left(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon arrow-fat-left. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -1857,15 +1882,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def arrow_fat_line_down(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon arrow-fat-line-down. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -1880,15 +1905,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def arrow_fat_line_left(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon arrow-fat-line-left. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -1903,15 +1928,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def arrow_fat_line_right(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon arrow-fat-line-right. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -1926,15 +1951,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def arrow_fat_line_up(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon arrow-fat-line-up. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -1949,15 +1974,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def arrow_fat_lines_down(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon arrow-fat-lines-down. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -1972,15 +1997,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def arrow_fat_lines_left(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon arrow-fat-lines-left. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -1995,15 +2020,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def arrow_fat_lines_right(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon arrow-fat-lines-right. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -2018,15 +2043,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def arrow_fat_lines_up(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon arrow-fat-lines-up. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -2041,15 +2066,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def arrow_fat_right(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon arrow-fat-right. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -2064,15 +2089,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def arrow_fat_up(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon arrow-fat-up. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -2087,15 +2112,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def arrow_left(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon arrow-left. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -2110,15 +2135,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def arrow_line_down(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon arrow-line-down. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -2133,15 +2158,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def arrow_line_down_left(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon arrow-line-down-left. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -2156,15 +2181,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def arrow_line_down_right(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon arrow-line-down-right. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -2179,15 +2204,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def arrow_line_left(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon arrow-line-left. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -2202,15 +2227,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def arrow_line_right(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon arrow-line-right. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -2225,15 +2250,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def arrow_line_up(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon arrow-line-up. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -2248,15 +2273,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def arrow_line_up_left(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon arrow-line-up-left. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -2271,15 +2296,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def arrow_line_up_right(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon arrow-line-up-right. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -2294,15 +2319,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def arrow_right(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon arrow-right. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -2317,15 +2342,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def arrow_square_down(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon arrow-square-down. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -2340,15 +2365,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def arrow_square_down_left(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon arrow-square-down-left. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -2363,15 +2388,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def arrow_square_down_right(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon arrow-square-down-right. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -2386,15 +2411,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def arrow_square_in(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon arrow-square-in. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -2409,15 +2434,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def arrow_square_left(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon arrow-square-left. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -2432,15 +2457,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def arrow_square_out(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon arrow-square-out. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -2455,15 +2480,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def arrow_square_right(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon arrow-square-right. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -2478,15 +2503,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def arrow_square_up(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon arrow-square-up. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -2501,15 +2526,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def arrow_square_up_left(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon arrow-square-up-left. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -2524,15 +2549,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def arrow_square_up_right(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon arrow-square-up-right. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -2547,15 +2572,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def arrow_u_down_left(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon arrow-u-down-left. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -2570,15 +2595,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def arrow_u_down_right(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon arrow-u-down-right. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -2593,15 +2618,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def arrow_u_left_down(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon arrow-u-left-down. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -2616,15 +2641,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def arrow_u_left_up(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon arrow-u-left-up. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -2639,15 +2664,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def arrow_u_right_down(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon arrow-u-right-down. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -2662,15 +2687,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def arrow_u_right_up(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon arrow-u-right-up. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -2685,15 +2710,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def arrow_u_up_left(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon arrow-u-up-left. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -2708,15 +2733,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def arrow_u_up_right(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon arrow-u-up-right. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -2731,15 +2756,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def arrow_up(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon arrow-up. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -2754,15 +2779,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def arrow_up_left(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon arrow-up-left. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -2777,15 +2802,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def arrow_up_right(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon arrow-up-right. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -2800,15 +2825,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def arrows_clockwise(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon arrows-clockwise. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -2823,15 +2848,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def arrows_counter_clockwise(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon arrows-counter-clockwise. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -2846,15 +2871,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def arrows_down_up(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon arrows-down-up. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -2869,15 +2894,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def arrows_horizontal(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon arrows-horizontal. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -2892,15 +2917,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def arrows_in(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon arrows-in. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -2915,15 +2940,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def arrows_in_cardinal(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon arrows-in-cardinal. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -2938,15 +2963,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def arrows_in_line_horizontal(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon arrows-in-line-horizontal. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -2961,15 +2986,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def arrows_in_line_vertical(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon arrows-in-line-vertical. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -2984,15 +3009,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def arrows_in_simple(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon arrows-in-simple. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -3007,15 +3032,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def arrows_left_right(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon arrows-left-right. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -3030,15 +3055,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def arrows_merge(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon arrows-merge. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -3053,15 +3078,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def arrows_out(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon arrows-out. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -3076,15 +3101,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def arrows_out_cardinal(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon arrows-out-cardinal. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -3099,15 +3124,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def arrows_out_line_horizontal(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon arrows-out-line-horizontal. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -3122,15 +3147,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def arrows_out_line_vertical(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon arrows-out-line-vertical. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -3145,15 +3170,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def arrows_out_simple(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon arrows-out-simple. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -3168,15 +3193,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def arrows_split(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon arrows-split. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -3191,15 +3216,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def arrows_vertical(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon arrows-vertical. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -3214,15 +3239,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def article(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon article. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -3237,15 +3262,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def article_medium(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon article-medium. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -3260,15 +3285,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def article_ny_times(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon article-ny-times. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -3283,15 +3308,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def asclepius(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon asclepius. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -3306,15 +3331,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def caduceus(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon caduceus. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -3329,15 +3354,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def asterisk(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon asterisk. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -3352,15 +3377,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def asterisk_simple(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon asterisk-simple. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -3375,15 +3400,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def at(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon at. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -3398,15 +3423,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def atom(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon atom. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -3421,15 +3446,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def avocado(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon avocado. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -3444,15 +3469,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def axe(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon axe. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -3467,15 +3492,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def baby(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon baby. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -3490,15 +3515,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def baby_carriage(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon baby-carriage. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -3513,15 +3538,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def backpack(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon backpack. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -3536,15 +3561,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def backspace(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon backspace. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -3559,15 +3584,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def bag(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon bag. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -3582,15 +3607,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def bag_simple(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon bag-simple. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -3605,15 +3630,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def balloon(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon balloon. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -3628,15 +3653,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def bandaids(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon bandaids. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -3651,15 +3676,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def bank(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon bank. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -3674,15 +3699,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def barbell(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon barbell. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -3697,15 +3722,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def barcode(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon barcode. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -3720,15 +3745,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def barn(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon barn. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -3743,15 +3768,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def barricade(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon barricade. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -3766,15 +3791,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def baseball(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon baseball. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -3789,15 +3814,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def baseball_cap(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon baseball-cap. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -3812,15 +3837,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def baseball_helmet(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon baseball-helmet. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -3835,15 +3860,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def basket(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon basket. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -3858,15 +3883,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def basketball(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon basketball. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -3881,15 +3906,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def bathtub(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon bathtub. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -3904,15 +3929,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def battery_charging(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon battery-charging. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -3927,15 +3952,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def battery_charging_vertical(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon battery-charging-vertical. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -3950,15 +3975,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def battery_empty(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon battery-empty. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -3973,15 +3998,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def battery_full(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon battery-full. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -3996,15 +4021,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def battery_high(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon battery-high. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -4019,15 +4044,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def battery_low(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon battery-low. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -4042,15 +4067,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def battery_medium(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon battery-medium. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -4065,15 +4090,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def battery_plus(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon battery-plus. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -4088,15 +4113,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def battery_plus_vertical(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon battery-plus-vertical. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -4111,15 +4136,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def battery_vertical_empty(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon battery-vertical-empty. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -4134,15 +4159,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def battery_vertical_full(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon battery-vertical-full. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -4157,15 +4182,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def battery_vertical_high(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon battery-vertical-high. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -4180,15 +4205,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def battery_vertical_low(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon battery-vertical-low. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -4203,15 +4228,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def battery_vertical_medium(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon battery-vertical-medium. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -4226,15 +4251,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def battery_warning(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon battery-warning. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -4249,15 +4274,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def battery_warning_vertical(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon battery-warning-vertical. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -4272,15 +4297,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def beach_ball(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon beach-ball. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -4295,15 +4320,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def beanie(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon beanie. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -4318,15 +4343,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def bed(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon bed. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -4341,15 +4366,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def beer_bottle(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon beer-bottle. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -4364,15 +4389,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def beer_stein(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon beer-stein. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -4387,15 +4412,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def behance_logo(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon behance-logo. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -4410,15 +4435,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def bell(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon bell. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -4433,15 +4458,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def bell_ringing(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon bell-ringing. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -4456,15 +4481,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def bell_simple(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon bell-simple. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -4479,15 +4504,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def bell_simple_ringing(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon bell-simple-ringing. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -4502,15 +4527,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def bell_simple_slash(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon bell-simple-slash. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -4525,15 +4550,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def bell_simple_z(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon bell-simple-z. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -4548,15 +4573,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def bell_slash(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon bell-slash. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -4571,15 +4596,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def bell_z(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon bell-z. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -4594,15 +4619,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def belt(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon belt. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -4617,15 +4642,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def bezier_curve(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon bezier-curve. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -4640,15 +4665,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def bicycle(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon bicycle. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -4663,15 +4688,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def binary(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon binary. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -4686,15 +4711,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def binoculars(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon binoculars. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -4709,15 +4734,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def biohazard(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon biohazard. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -4732,15 +4757,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def bird(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon bird. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -4755,15 +4780,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def blueprint(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon blueprint. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -4778,15 +4803,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def bluetooth(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon bluetooth. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -4801,15 +4826,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def bluetooth_connected(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon bluetooth-connected. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -4824,15 +4849,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def bluetooth_slash(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon bluetooth-slash. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -4847,15 +4872,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def bluetooth_x(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon bluetooth-x. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -4870,15 +4895,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def boat(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon boat. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -4893,15 +4918,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def bomb(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon bomb. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -4916,15 +4941,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def bone(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon bone. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -4939,15 +4964,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def book(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon book. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -4962,15 +4987,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def book_bookmark(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon book-bookmark. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -4985,15 +5010,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def book_open(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon book-open. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -5008,15 +5033,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def book_open_text(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon book-open-text. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -5031,15 +5056,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def book_open_user(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon book-open-user. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -5054,15 +5079,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def bookmark(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon bookmark. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -5077,15 +5102,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def bookmark_simple(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon bookmark-simple. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -5100,15 +5125,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def bookmarks(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon bookmarks. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -5123,15 +5148,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def bookmarks_simple(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon bookmarks-simple. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -5146,15 +5171,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def books(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon books. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -5169,15 +5194,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def boot(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon boot. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -5192,15 +5217,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def boules(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon boules. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -5215,15 +5240,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def bounding_box(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon bounding-box. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -5238,15 +5263,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def bowl_food(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon bowl-food. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -5261,15 +5286,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def bowl_steam(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon bowl-steam. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -5284,15 +5309,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def bowling_ball(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon bowling-ball. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -5307,15 +5332,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def box_arrow_down(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon box-arrow-down. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -5330,15 +5355,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def archive_box(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon archive-box. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -5353,15 +5378,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def box_arrow_up(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon box-arrow-up. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -5376,15 +5401,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def boxing_glove(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon boxing-glove. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -5399,15 +5424,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def brackets_angle(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon brackets-angle. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -5422,15 +5447,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def brackets_curly(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon brackets-curly. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -5445,15 +5470,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def brackets_round(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon brackets-round. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -5468,15 +5493,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def brackets_square(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon brackets-square. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -5491,15 +5516,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def brain(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon brain. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -5514,15 +5539,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def brandy(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon brandy. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -5537,15 +5562,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def bread(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon bread. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -5560,15 +5585,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def bridge(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon bridge. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -5583,15 +5608,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def briefcase(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon briefcase. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -5606,15 +5631,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def briefcase_metal(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon briefcase-metal. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -5629,15 +5654,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def broadcast(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon broadcast. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -5652,15 +5677,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def broom(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon broom. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -5675,15 +5700,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def browser(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon browser. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -5698,15 +5723,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def browsers(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon browsers. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -5721,15 +5746,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def bug(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon bug. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -5744,15 +5769,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def bug_beetle(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon bug-beetle. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -5767,15 +5792,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def bug_droid(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon bug-droid. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -5790,15 +5815,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def building(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon building. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -5813,15 +5838,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def building_apartment(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon building-apartment. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -5836,15 +5861,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def building_office(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon building-office. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -5859,15 +5884,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def buildings(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon buildings. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -5882,15 +5907,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def bulldozer(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon bulldozer. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -5905,15 +5930,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def bus(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon bus. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -5928,15 +5953,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def butterfly(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon butterfly. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -5951,15 +5976,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def cable_car(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon cable-car. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -5974,15 +5999,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def cactus(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon cactus. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -5997,15 +6022,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def cake(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon cake. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -6020,15 +6045,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def calculator(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon calculator. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -6043,15 +6068,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def calendar(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon calendar. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -6066,15 +6091,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def calendar_blank(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon calendar-blank. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -6089,15 +6114,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def calendar_check(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon calendar-check. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -6112,15 +6137,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def calendar_dot(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon calendar-dot. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -6135,15 +6160,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def calendar_dots(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon calendar-dots. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -6158,15 +6183,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def calendar_heart(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon calendar-heart. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -6181,15 +6206,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def calendar_minus(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon calendar-minus. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -6204,15 +6229,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def calendar_plus(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon calendar-plus. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -6227,15 +6252,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def calendar_slash(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon calendar-slash. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -6250,15 +6275,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def calendar_star(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon calendar-star. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -6273,15 +6298,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def calendar_x(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon calendar-x. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -6296,15 +6321,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def call_bell(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon call-bell. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -6319,15 +6344,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def camera(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon camera. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -6342,15 +6367,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def camera_plus(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon camera-plus. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -6365,15 +6390,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def camera_rotate(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon camera-rotate. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -6388,15 +6413,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def camera_slash(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon camera-slash. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -6411,15 +6436,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def campfire(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon campfire. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -6434,15 +6459,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def car(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon car. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -6457,15 +6482,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def car_battery(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon car-battery. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -6480,15 +6505,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def car_profile(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon car-profile. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -6503,15 +6528,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def car_simple(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon car-simple. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -6526,15 +6551,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def cardholder(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon cardholder. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -6549,15 +6574,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def cards(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon cards. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -6572,15 +6597,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def cards_three(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon cards-three. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -6595,15 +6620,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def caret_circle_double_down(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon caret-circle-double-down. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -6618,15 +6643,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def caret_circle_double_left(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon caret-circle-double-left. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -6641,15 +6666,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def caret_circle_double_right(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon caret-circle-double-right. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -6664,15 +6689,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def caret_circle_double_up(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon caret-circle-double-up. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -6687,15 +6712,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def caret_circle_down(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon caret-circle-down. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -6710,15 +6735,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def caret_circle_left(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon caret-circle-left. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -6733,15 +6758,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def caret_circle_right(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon caret-circle-right. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -6756,15 +6781,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def caret_circle_up(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon caret-circle-up. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -6779,15 +6804,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def caret_circle_up_down(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon caret-circle-up-down. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -6802,15 +6827,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def caret_double_down(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon caret-double-down. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -6825,15 +6850,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def caret_double_left(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon caret-double-left. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -6848,15 +6873,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def caret_double_right(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon caret-double-right. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -6871,15 +6896,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def caret_double_up(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon caret-double-up. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -6894,15 +6919,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def caret_down(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon caret-down. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -6917,15 +6942,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def caret_left(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon caret-left. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -6940,15 +6965,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def caret_line_down(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon caret-line-down. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -6963,15 +6988,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def caret_line_left(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon caret-line-left. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -6986,15 +7011,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def caret_line_right(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon caret-line-right. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -7009,15 +7034,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def caret_line_up(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon caret-line-up. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -7032,15 +7057,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def caret_right(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon caret-right. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -7055,15 +7080,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def caret_up(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon caret-up. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -7078,15 +7103,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def caret_up_down(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon caret-up-down. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -7101,15 +7126,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def carrot(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon carrot. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -7124,15 +7149,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def cash_register(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon cash-register. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -7147,15 +7172,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def cassette_tape(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon cassette-tape. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -7170,15 +7195,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def castle_turret(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon castle-turret. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -7193,15 +7218,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def cat(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon cat. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -7216,15 +7241,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def cell_signal_full(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon cell-signal-full. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -7239,15 +7264,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def cell_signal_high(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon cell-signal-high. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -7262,15 +7287,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def cell_signal_low(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon cell-signal-low. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -7285,15 +7310,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def cell_signal_medium(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon cell-signal-medium. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -7308,15 +7333,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def cell_signal_none(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon cell-signal-none. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -7331,15 +7356,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def cell_signal_slash(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon cell-signal-slash. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -7354,15 +7379,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def cell_signal_x(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon cell-signal-x. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -7377,15 +7402,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def cell_tower(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon cell-tower. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -7400,15 +7425,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def certificate(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon certificate. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -7423,15 +7448,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def chair(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon chair. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -7446,15 +7471,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def chalkboard(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon chalkboard. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -7469,15 +7494,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def chalkboard_simple(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon chalkboard-simple. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -7492,15 +7517,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def chalkboard_teacher(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon chalkboard-teacher. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -7515,15 +7540,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def champagne(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon champagne. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -7538,15 +7563,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def charging_station(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon charging-station. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -7561,15 +7586,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def chart_bar(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon chart-bar. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -7584,15 +7609,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def chart_bar_horizontal(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon chart-bar-horizontal. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -7607,15 +7632,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def chart_donut(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon chart-donut. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -7630,15 +7655,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def chart_line(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon chart-line. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -7653,15 +7678,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def chart_line_down(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon chart-line-down. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -7676,15 +7701,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def chart_line_up(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon chart-line-up. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -7699,15 +7724,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def chart_pie(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon chart-pie. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -7722,15 +7747,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def chart_pie_slice(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon chart-pie-slice. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -7745,15 +7770,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def chart_polar(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon chart-polar. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -7768,15 +7793,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def chart_scatter(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon chart-scatter. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -7791,15 +7816,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def chat(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon chat. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -7814,15 +7839,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def chat_centered(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon chat-centered. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -7837,15 +7862,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def chat_centered_dots(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon chat-centered-dots. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -7860,15 +7885,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def chat_centered_slash(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon chat-centered-slash. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -7883,15 +7908,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def chat_centered_text(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon chat-centered-text. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -7906,15 +7931,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def chat_circle(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon chat-circle. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -7929,15 +7954,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def chat_circle_dots(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon chat-circle-dots. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -7952,15 +7977,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def chat_circle_slash(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon chat-circle-slash. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -7975,15 +8000,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def chat_circle_text(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon chat-circle-text. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -7998,15 +8023,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def chat_dots(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon chat-dots. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -8021,15 +8046,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def chat_slash(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon chat-slash. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -8044,15 +8069,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def chat_teardrop(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon chat-teardrop. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -8067,15 +8092,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def chat_teardrop_dots(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon chat-teardrop-dots. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -8090,15 +8115,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def chat_teardrop_slash(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon chat-teardrop-slash. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -8113,15 +8138,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def chat_teardrop_text(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon chat-teardrop-text. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -8136,15 +8161,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def chat_text(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon chat-text. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -8159,15 +8184,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def chats(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon chats. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -8182,15 +8207,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def chats_circle(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon chats-circle. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -8205,15 +8230,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def chats_teardrop(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon chats-teardrop. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -8228,15 +8253,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def check(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon check. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -8251,15 +8276,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def check_circle(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon check-circle. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -8274,15 +8299,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def check_fat(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon check-fat. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -8297,15 +8322,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def check_square(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon check-square. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -8320,15 +8345,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def check_square_offset(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon check-square-offset. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -8343,15 +8368,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def checkerboard(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon checkerboard. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -8366,15 +8391,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def checks(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon checks. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -8389,15 +8414,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def cheers(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon cheers. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -8412,15 +8437,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def cheese(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon cheese. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -8435,15 +8460,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def chef_hat(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon chef-hat. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -8458,15 +8483,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def cherries(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon cherries. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -8481,15 +8506,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def church(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon church. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -8504,15 +8529,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def cigarette(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon cigarette. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -8527,15 +8552,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def cigarette_slash(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon cigarette-slash. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -8550,15 +8575,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def circle(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon circle. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -8573,15 +8598,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def circle_dashed(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon circle-dashed. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -8596,15 +8621,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def circle_half(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon circle-half. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -8619,15 +8644,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def circle_half_tilt(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon circle-half-tilt. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -8642,15 +8667,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def circle_notch(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon circle-notch. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -8665,15 +8690,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def circles_four(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon circles-four. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -8688,15 +8713,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def circles_three(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon circles-three. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -8711,15 +8736,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def circles_three_plus(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon circles-three-plus. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -8734,15 +8759,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def circuitry(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon circuitry. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -8757,15 +8782,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def city(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon city. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -8780,15 +8805,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def clipboard(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon clipboard. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -8803,15 +8828,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def clipboard_text(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon clipboard-text. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -8826,15 +8851,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def clock(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon clock. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -8849,15 +8874,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def clock_afternoon(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon clock-afternoon. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -8872,15 +8897,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def clock_clockwise(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon clock-clockwise. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -8895,15 +8920,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def clock_countdown(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon clock-countdown. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -8918,15 +8943,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def clock_counter_clockwise(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon clock-counter-clockwise. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -8941,15 +8966,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def clock_user(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon clock-user. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -8964,15 +8989,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def closed_captioning(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon closed-captioning. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -8987,15 +9012,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def cloud(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon cloud. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -9010,15 +9035,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def cloud_arrow_down(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon cloud-arrow-down. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -9033,15 +9058,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def cloud_arrow_up(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon cloud-arrow-up. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -9056,15 +9081,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def cloud_check(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon cloud-check. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -9079,15 +9104,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def cloud_fog(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon cloud-fog. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -9102,15 +9127,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def cloud_lightning(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon cloud-lightning. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -9125,15 +9150,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def cloud_moon(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon cloud-moon. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -9148,15 +9173,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def cloud_rain(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon cloud-rain. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -9171,15 +9196,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def cloud_slash(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon cloud-slash. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -9194,15 +9219,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def cloud_snow(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon cloud-snow. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -9217,15 +9242,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def cloud_sun(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon cloud-sun. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -9240,15 +9265,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def cloud_warning(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon cloud-warning. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -9263,15 +9288,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def cloud_x(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon cloud-x. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -9286,15 +9311,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def clover(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon clover. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -9309,15 +9334,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def club(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon club. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -9332,15 +9357,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def coat_hanger(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon coat-hanger. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -9355,15 +9380,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def coda_logo(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon coda-logo. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -9378,15 +9403,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def code(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon code. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -9401,15 +9426,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def code_block(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon code-block. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -9424,15 +9449,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def code_simple(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon code-simple. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -9447,15 +9472,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def codepen_logo(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon codepen-logo. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -9470,15 +9495,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def codesandbox_logo(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon codesandbox-logo. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -9493,15 +9518,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def coffee(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon coffee. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -9516,15 +9541,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def coffee_bean(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon coffee-bean. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -9539,15 +9564,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def coin(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon coin. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -9562,15 +9587,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def coin_vertical(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon coin-vertical. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -9585,15 +9610,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def coins(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon coins. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -9608,15 +9633,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def columns(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon columns. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -9631,15 +9656,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def columns_plus_left(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon columns-plus-left. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -9654,15 +9679,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def columns_plus_right(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon columns-plus-right. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -9677,15 +9702,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def command(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon command. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -9700,15 +9725,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def compass(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon compass. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -9723,15 +9748,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def compass_rose(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon compass-rose. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -9746,15 +9771,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def compass_tool(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon compass-tool. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -9769,15 +9794,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def computer_tower(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon computer-tower. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -9792,15 +9817,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def confetti(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon confetti. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -9815,15 +9840,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def contactless_payment(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon contactless-payment. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -9838,15 +9863,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def control(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon control. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -9861,15 +9886,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def cookie(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon cookie. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -9884,15 +9909,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def cooking_pot(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon cooking-pot. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -9907,15 +9932,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def copy(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon copy. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -9930,15 +9955,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def copy_simple(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon copy-simple. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -9953,15 +9978,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def copyleft(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon copyleft. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -9976,15 +10001,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def copyright(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon copyright. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -9999,15 +10024,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def corners_in(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon corners-in. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -10022,15 +10047,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def corners_out(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon corners-out. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -10045,15 +10070,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def couch(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon couch. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -10068,15 +10093,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def court_basketball(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon court-basketball. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -10091,15 +10116,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def cow(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon cow. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -10114,15 +10139,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def cowboy_hat(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon cowboy-hat. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -10137,15 +10162,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def cpu(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon cpu. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -10160,15 +10185,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def crane(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon crane. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -10183,15 +10208,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def crane_tower(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon crane-tower. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -10206,15 +10231,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def credit_card(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon credit-card. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -10229,15 +10254,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def cricket(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon cricket. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -10252,15 +10277,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def crop(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon crop. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -10275,15 +10300,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def cross(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon cross. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -10298,15 +10323,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def crosshair(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon crosshair. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -10321,15 +10346,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def crosshair_simple(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon crosshair-simple. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -10344,15 +10369,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def crown(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon crown. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -10367,15 +10392,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def crown_cross(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon crown-cross. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -10390,15 +10415,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def crown_simple(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon crown-simple. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -10413,15 +10438,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def cube(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon cube. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -10436,15 +10461,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def cube_focus(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon cube-focus. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -10459,15 +10484,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def cube_transparent(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon cube-transparent. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -10482,15 +10507,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def currency_btc(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon currency-btc. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -10505,15 +10530,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def currency_circle_dollar(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon currency-circle-dollar. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -10528,15 +10553,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def currency_cny(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon currency-cny. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -10551,15 +10576,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def currency_dollar(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon currency-dollar. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -10574,15 +10599,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def currency_dollar_simple(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon currency-dollar-simple. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -10597,15 +10622,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def currency_eth(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon currency-eth. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -10620,15 +10645,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def currency_eur(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon currency-eur. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -10643,15 +10668,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def currency_gbp(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon currency-gbp. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -10666,15 +10691,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def currency_inr(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon currency-inr. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -10689,15 +10714,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def currency_jpy(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon currency-jpy. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -10712,15 +10737,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def currency_krw(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon currency-krw. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -10735,15 +10760,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def currency_kzt(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon currency-kzt. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -10758,15 +10783,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def currency_ngn(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon currency-ngn. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -10781,15 +10806,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def currency_rub(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon currency-rub. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -10804,15 +10829,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def cursor(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon cursor. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -10827,15 +10852,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def cursor_click(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon cursor-click. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -10850,15 +10875,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def cursor_text(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon cursor-text. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -10873,15 +10898,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def cylinder(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon cylinder. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -10896,15 +10921,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def database(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon database. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -10919,15 +10944,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def desk(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon desk. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -10942,15 +10967,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def desktop(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon desktop. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -10965,15 +10990,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def desktop_tower(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon desktop-tower. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -10988,15 +11013,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def detective(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon detective. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -11011,15 +11036,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def dev_to_logo(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon dev-to-logo. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -11034,15 +11059,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def device_mobile(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon device-mobile. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -11057,15 +11082,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def device_mobile_camera(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon device-mobile-camera. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -11080,15 +11105,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def device_mobile_slash(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon device-mobile-slash. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -11103,15 +11128,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def device_mobile_speaker(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon device-mobile-speaker. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -11126,15 +11151,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def device_rotate(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon device-rotate. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -11149,15 +11174,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def device_tablet(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon device-tablet. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -11172,15 +11197,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def device_tablet_camera(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon device-tablet-camera. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -11195,15 +11220,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def device_tablet_speaker(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon device-tablet-speaker. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -11218,15 +11243,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def devices(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon devices. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -11241,15 +11266,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def diamond(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon diamond. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -11264,15 +11289,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def diamonds_four(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon diamonds-four. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -11287,15 +11312,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def dice_five(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon dice-five. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -11310,15 +11335,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def dice_four(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon dice-four. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -11333,15 +11358,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def dice_one(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon dice-one. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -11356,15 +11381,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def dice_six(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon dice-six. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -11379,15 +11404,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def dice_three(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon dice-three. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -11402,15 +11427,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def dice_two(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon dice-two. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -11425,15 +11450,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def disc(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon disc. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -11448,15 +11473,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def disco_ball(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon disco-ball. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -11471,15 +11496,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def discord_logo(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon discord-logo. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -11494,15 +11519,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def divide(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon divide. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -11517,15 +11542,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def dna(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon dna. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -11540,15 +11565,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def dog(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon dog. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -11563,15 +11588,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def door(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon door. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -11586,15 +11611,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def door_open(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon door-open. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -11609,15 +11634,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def dot(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon dot. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -11632,15 +11657,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def dot_outline(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon dot-outline. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -11655,15 +11680,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def dots_nine(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon dots-nine. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -11678,15 +11703,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def dots_six(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon dots-six. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -11701,15 +11726,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def dots_six_vertical(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon dots-six-vertical. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -11724,15 +11749,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def dots_three(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon dots-three. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -11747,15 +11772,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def dots_three_circle(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon dots-three-circle. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -11770,15 +11795,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def dots_three_circle_vertical(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon dots-three-circle-vertical. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -11793,15 +11818,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def dots_three_outline(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon dots-three-outline. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -11816,15 +11841,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def dots_three_outline_vertical(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon dots-three-outline-vertical. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -11839,15 +11864,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def dots_three_vertical(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon dots-three-vertical. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -11862,15 +11887,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def download(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon download. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -11885,15 +11910,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def download_simple(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon download-simple. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -11908,15 +11933,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def dress(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon dress. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -11931,15 +11956,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def dresser(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon dresser. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -11954,15 +11979,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def dribbble_logo(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon dribbble-logo. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -11977,15 +12002,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def drone(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon drone. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -12000,15 +12025,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def drop(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon drop. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -12023,15 +12048,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def drop_half(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon drop-half. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -12046,15 +12071,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def drop_half_bottom(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon drop-half-bottom. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -12069,15 +12094,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def drop_simple(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon drop-simple. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -12092,15 +12117,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def drop_slash(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon drop-slash. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -12115,15 +12140,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def dropbox_logo(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon dropbox-logo. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -12138,15 +12163,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def ear(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon ear. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -12161,15 +12186,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def ear_slash(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon ear-slash. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -12184,15 +12209,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def egg(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon egg. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -12207,15 +12232,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def egg_crack(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon egg-crack. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -12230,15 +12255,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def eject(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon eject. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -12253,15 +12278,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def eject_simple(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon eject-simple. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -12276,15 +12301,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def elevator(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon elevator. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -12299,15 +12324,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def empty(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon empty. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -12322,15 +12347,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def engine(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon engine. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -12345,15 +12370,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def envelope(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon envelope. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -12368,15 +12393,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def envelope_open(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon envelope-open. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -12391,15 +12416,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def envelope_simple(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon envelope-simple. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -12414,15 +12439,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def envelope_simple_open(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon envelope-simple-open. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -12437,15 +12462,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def equalizer(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon equalizer. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -12460,15 +12485,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def equals(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon equals. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -12483,15 +12508,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def eraser(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon eraser. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -12506,15 +12531,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def escalator_down(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon escalator-down. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -12529,15 +12554,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def escalator_up(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon escalator-up. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -12552,15 +12577,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def exam(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon exam. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -12575,15 +12600,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def exclamation_mark(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon exclamation-mark. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -12598,15 +12623,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def exclude(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon exclude. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -12621,15 +12646,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def exclude_square(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon exclude-square. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -12644,15 +12669,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def export(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon export. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -12667,15 +12692,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def eye(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon eye. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -12690,15 +12715,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def eye_closed(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon eye-closed. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -12713,15 +12738,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def eye_slash(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon eye-slash. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -12736,15 +12761,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def eyedropper(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon eyedropper. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -12759,15 +12784,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def eyedropper_sample(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon eyedropper-sample. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -12782,15 +12807,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def eyeglasses(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon eyeglasses. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -12805,15 +12830,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def eyes(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon eyes. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -12828,15 +12853,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def face_mask(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon face-mask. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -12851,15 +12876,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def facebook_logo(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon facebook-logo. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -12874,15 +12899,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def factory(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon factory. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -12897,15 +12922,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def faders(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon faders. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -12920,15 +12945,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def faders_horizontal(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon faders-horizontal. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -12943,15 +12968,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def fallout_shelter(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon fallout-shelter. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -12966,15 +12991,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def fan(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon fan. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -12989,15 +13014,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def farm(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon farm. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -13012,15 +13037,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def fast_forward(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon fast-forward. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -13035,15 +13060,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def fast_forward_circle(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon fast-forward-circle. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -13058,15 +13083,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def feather(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon feather. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -13081,15 +13106,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def fediverse_logo(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon fediverse-logo. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -13104,15 +13129,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def figma_logo(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon figma-logo. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -13127,15 +13152,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def file(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon file. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -13150,15 +13175,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def file_archive(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon file-archive. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -13173,15 +13198,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def file_arrow_down(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon file-arrow-down. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -13196,15 +13221,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def file_arrow_up(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon file-arrow-up. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -13219,15 +13244,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def file_audio(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon file-audio. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -13242,15 +13267,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def file_c(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon file-c. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -13265,15 +13290,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def file_c_sharp(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon file-c-sharp. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -13288,15 +13313,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def file_cloud(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon file-cloud. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -13311,15 +13336,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def file_code(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon file-code. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -13334,15 +13359,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def file_cpp(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon file-cpp. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -13357,15 +13382,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def file_css(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon file-css. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -13380,15 +13405,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def file_csv(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon file-csv. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -13403,15 +13428,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def file_dashed(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon file-dashed. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -13426,15 +13451,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def file_dotted(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon file-dotted. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -13449,15 +13474,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def file_doc(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon file-doc. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -13472,15 +13497,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def file_html(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon file-html. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -13495,15 +13520,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def file_image(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon file-image. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -13518,15 +13543,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def file_ini(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon file-ini. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -13541,15 +13566,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def file_jpg(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon file-jpg. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -13564,15 +13589,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def file_js(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon file-js. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -13587,15 +13612,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def file_jsx(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon file-jsx. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -13610,15 +13635,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def file_lock(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon file-lock. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -13633,15 +13658,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def file_magnifying_glass(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon file-magnifying-glass. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -13656,15 +13681,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def file_search(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon file-search. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -13679,15 +13704,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def file_md(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon file-md. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -13702,15 +13727,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def file_minus(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon file-minus. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -13725,15 +13750,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def file_pdf(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon file-pdf. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -13748,15 +13773,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def file_plus(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon file-plus. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -13771,15 +13796,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def file_png(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon file-png. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -13794,15 +13819,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def file_ppt(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon file-ppt. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -13817,15 +13842,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def file_py(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon file-py. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -13840,15 +13865,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def file_rs(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon file-rs. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -13863,15 +13888,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def file_sql(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon file-sql. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -13886,15 +13911,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def file_svg(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon file-svg. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -13909,15 +13934,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def file_text(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon file-text. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -13932,15 +13957,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def file_ts(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon file-ts. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -13955,15 +13980,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def file_tsx(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon file-tsx. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -13978,15 +14003,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def file_txt(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon file-txt. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -14001,15 +14026,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def file_video(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon file-video. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -14024,15 +14049,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def file_vue(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon file-vue. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -14047,15 +14072,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def file_x(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon file-x. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -14070,15 +14095,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def file_xls(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon file-xls. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -14093,15 +14118,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def file_zip(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon file-zip. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -14116,15 +14141,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def files(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon files. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -14139,15 +14164,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def film_reel(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon film-reel. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -14162,15 +14187,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def film_script(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon film-script. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -14185,15 +14210,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def film_slate(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon film-slate. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -14208,15 +14233,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def film_strip(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon film-strip. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -14231,15 +14256,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def fingerprint(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon fingerprint. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -14254,15 +14279,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def fingerprint_simple(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon fingerprint-simple. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -14277,15 +14302,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def finn_the_human(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon finn-the-human. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -14300,15 +14325,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def fire(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon fire. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -14323,15 +14348,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def fire_extinguisher(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon fire-extinguisher. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -14346,15 +14371,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def fire_simple(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon fire-simple. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -14369,15 +14394,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def fire_truck(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon fire-truck. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -14392,15 +14417,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def first_aid(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon first-aid. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -14415,15 +14440,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def first_aid_kit(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon first-aid-kit. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -14438,15 +14463,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def fish(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon fish. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -14461,15 +14486,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def fish_simple(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon fish-simple. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -14484,15 +14509,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def flag(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon flag. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -14507,15 +14532,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def flag_banner(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon flag-banner. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -14530,15 +14555,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def flag_banner_fold(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon flag-banner-fold. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -14553,15 +14578,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def flag_checkered(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon flag-checkered. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -14576,15 +14601,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def flag_pennant(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon flag-pennant. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -14599,15 +14624,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def flame(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon flame. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -14622,15 +14647,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def flashlight(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon flashlight. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -14645,15 +14670,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def flask(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon flask. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -14668,15 +14693,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def flip_horizontal(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon flip-horizontal. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -14691,15 +14716,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def flip_vertical(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon flip-vertical. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -14714,15 +14739,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def floppy_disk(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon floppy-disk. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -14737,15 +14762,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def floppy_disk_back(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon floppy-disk-back. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -14760,15 +14785,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def flow_arrow(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon flow-arrow. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -14783,15 +14808,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def flower(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon flower. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -14806,15 +14831,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def flower_lotus(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon flower-lotus. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -14829,15 +14854,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def flower_tulip(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon flower-tulip. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -14852,15 +14877,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def flying_saucer(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon flying-saucer. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -14875,15 +14900,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def folder(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon folder. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -14898,15 +14923,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def folder_notch(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon folder-notch. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -14921,15 +14946,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def folder_dashed(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon folder-dashed. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -14944,15 +14969,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def folder_dotted(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon folder-dotted. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -14967,15 +14992,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def folder_lock(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon folder-lock. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -14990,15 +15015,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def folder_minus(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon folder-minus. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -15013,15 +15038,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def folder_notch_minus(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon folder-notch-minus. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -15036,15 +15061,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def folder_open(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon folder-open. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -15059,15 +15084,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def folder_notch_open(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon folder-notch-open. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -15082,15 +15107,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def folder_plus(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon folder-plus. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -15105,15 +15130,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def folder_notch_plus(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon folder-notch-plus. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -15128,15 +15153,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def folder_simple(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon folder-simple. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -15151,15 +15176,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def folder_simple_dashed(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon folder-simple-dashed. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -15174,15 +15199,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def folder_simple_dotted(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon folder-simple-dotted. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -15197,15 +15222,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def folder_simple_lock(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon folder-simple-lock. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -15220,15 +15245,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def folder_simple_minus(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon folder-simple-minus. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -15243,15 +15268,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def folder_simple_plus(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon folder-simple-plus. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -15266,15 +15291,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def folder_simple_star(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon folder-simple-star. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -15289,15 +15314,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def folder_simple_user(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon folder-simple-user. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -15312,15 +15337,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def folder_star(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon folder-star. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -15335,15 +15360,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def folder_user(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon folder-user. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -15358,15 +15383,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def folders(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon folders. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -15381,15 +15406,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def football(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon football. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -15404,15 +15429,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def football_helmet(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon football-helmet. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -15427,15 +15452,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def footprints(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon footprints. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -15450,15 +15475,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def fork_knife(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon fork-knife. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -15473,15 +15498,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def four_k(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon four-k. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -15496,15 +15521,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def frame_corners(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon frame-corners. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -15519,15 +15544,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def framer_logo(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon framer-logo. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -15542,15 +15567,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def function(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon function. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -15565,15 +15590,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def funnel(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon funnel. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -15588,15 +15613,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def funnel_simple(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon funnel-simple. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -15611,15 +15636,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def funnel_simple_x(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon funnel-simple-x. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -15634,15 +15659,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def funnel_x(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon funnel-x. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -15657,15 +15682,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def game_controller(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon game-controller. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -15680,15 +15705,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def garage(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon garage. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -15703,15 +15728,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def gas_can(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon gas-can. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -15726,15 +15751,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def gas_pump(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon gas-pump. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -15749,15 +15774,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def gauge(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon gauge. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -15772,15 +15797,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def gavel(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon gavel. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -15795,15 +15820,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def gear(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon gear. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -15818,15 +15843,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def gear_fine(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon gear-fine. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -15841,15 +15866,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def gear_six(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon gear-six. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -15864,15 +15889,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def gender_female(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon gender-female. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -15887,15 +15912,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def gender_intersex(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon gender-intersex. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -15910,15 +15935,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def gender_male(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon gender-male. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -15933,15 +15958,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def gender_neuter(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon gender-neuter. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -15956,15 +15981,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def gender_nonbinary(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon gender-nonbinary. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -15979,15 +16004,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def gender_transgender(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon gender-transgender. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -16002,15 +16027,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def ghost(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon ghost. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -16025,15 +16050,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def gif(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon gif. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -16048,15 +16073,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def gift(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon gift. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -16071,15 +16096,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def git_branch(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon git-branch. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -16094,15 +16119,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def git_commit(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon git-commit. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -16117,15 +16142,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def git_diff(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon git-diff. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -16140,15 +16165,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def git_fork(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon git-fork. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -16163,15 +16188,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def git_merge(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon git-merge. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -16186,15 +16211,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def git_pull_request(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon git-pull-request. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -16209,15 +16234,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def github_logo(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon github-logo. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -16232,15 +16257,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def gitlab_logo(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon gitlab-logo. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -16255,15 +16280,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def gitlab_logo_simple(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon gitlab-logo-simple. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -16278,15 +16303,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def globe(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon globe. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -16301,15 +16326,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def globe_hemisphere_east(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon globe-hemisphere-east. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -16324,15 +16349,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def globe_hemisphere_west(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon globe-hemisphere-west. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -16347,15 +16372,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def globe_simple(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon globe-simple. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -16370,15 +16395,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def globe_simple_x(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon globe-simple-x. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -16393,15 +16418,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def globe_stand(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon globe-stand. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -16416,15 +16441,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def globe_x(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon globe-x. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -16439,15 +16464,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def goggles(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon goggles. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -16462,15 +16487,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def golf(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon golf. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -16485,15 +16510,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def goodreads_logo(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon goodreads-logo. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -16508,15 +16533,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def google_cardboard_logo(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon google-cardboard-logo. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -16531,15 +16556,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def google_chrome_logo(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon google-chrome-logo. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -16554,15 +16579,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def google_drive_logo(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon google-drive-logo. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -16577,15 +16602,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def google_logo(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon google-logo. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -16600,15 +16625,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def google_photos_logo(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon google-photos-logo. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -16623,15 +16648,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def google_play_logo(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon google-play-logo. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -16646,15 +16671,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def google_podcasts_logo(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon google-podcasts-logo. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -16669,15 +16694,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def gps(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon gps. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -16692,15 +16717,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def gps_fix(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon gps-fix. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -16715,15 +16740,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def gps_slash(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon gps-slash. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -16738,15 +16763,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def gradient(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon gradient. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -16761,15 +16786,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def graduation_cap(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon graduation-cap. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -16784,15 +16809,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def grains(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon grains. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -16807,15 +16832,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def grains_slash(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon grains-slash. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -16830,15 +16855,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def graph(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon graph. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -16853,15 +16878,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def graphics_card(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon graphics-card. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -16876,15 +16901,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def greater_than(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon greater-than. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -16899,15 +16924,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def greater_than_or_equal(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon greater-than-or-equal. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -16922,15 +16947,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def grid_four(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon grid-four. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -16945,15 +16970,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def grid_nine(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon grid-nine. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -16968,15 +16993,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def guitar(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon guitar. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -16991,15 +17016,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def hair_dryer(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon hair-dryer. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -17014,15 +17039,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def hamburger(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon hamburger. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -17037,15 +17062,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def hammer(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon hammer. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -17060,15 +17085,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def hand(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon hand. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -17083,15 +17108,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def hand_arrow_down(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon hand-arrow-down. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -17106,15 +17131,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def hand_arrow_up(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon hand-arrow-up. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -17129,15 +17154,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def hand_coins(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon hand-coins. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -17152,15 +17177,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def hand_deposit(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon hand-deposit. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -17175,15 +17200,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def hand_eye(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon hand-eye. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -17198,15 +17223,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def hand_fist(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon hand-fist. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -17221,15 +17246,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def hand_grabbing(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon hand-grabbing. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -17244,15 +17269,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def hand_heart(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon hand-heart. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -17267,15 +17292,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def hand_palm(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon hand-palm. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -17290,15 +17315,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def hand_peace(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon hand-peace. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -17313,15 +17338,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def hand_pointing(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon hand-pointing. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -17336,15 +17361,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def hand_soap(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon hand-soap. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -17359,15 +17384,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def hand_swipe_left(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon hand-swipe-left. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -17382,15 +17407,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def hand_swipe_right(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon hand-swipe-right. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -17405,15 +17430,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def hand_tap(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon hand-tap. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -17428,15 +17453,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def hand_waving(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon hand-waving. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -17451,15 +17476,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def hand_withdraw(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon hand-withdraw. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -17474,15 +17499,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def handbag(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon handbag. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -17497,15 +17522,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def handbag_simple(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon handbag-simple. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -17520,15 +17545,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def hands_clapping(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon hands-clapping. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -17543,15 +17568,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def hands_praying(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon hands-praying. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -17566,15 +17591,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def handshake(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon handshake. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -17589,15 +17614,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def hard_drive(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon hard-drive. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -17612,15 +17637,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def hard_drives(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon hard-drives. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -17635,15 +17660,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def hard_hat(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon hard-hat. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -17658,15 +17683,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def hash(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon hash. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -17681,15 +17706,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def hash_straight(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon hash-straight. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -17704,15 +17729,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def head_circuit(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon head-circuit. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -17727,15 +17752,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def headlights(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon headlights. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -17750,15 +17775,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def headphones(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon headphones. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -17773,15 +17798,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def headset(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon headset. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -17796,15 +17821,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def heart(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon heart. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -17819,15 +17844,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def heart_break(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon heart-break. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -17842,15 +17867,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def heart_half(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon heart-half. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -17865,15 +17890,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def heart_straight(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon heart-straight. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -17888,15 +17913,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def heart_straight_break(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon heart-straight-break. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -17911,15 +17936,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def heartbeat(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon heartbeat. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -17934,15 +17959,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def hexagon(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon hexagon. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -17957,15 +17982,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def high_definition(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon high-definition. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -17980,15 +18005,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def high_heel(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon high-heel. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -18003,15 +18028,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def highlighter(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon highlighter. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -18026,15 +18051,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def highlighter_circle(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon highlighter-circle. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -18049,15 +18074,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def hockey(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon hockey. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -18072,15 +18097,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def hoodie(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon hoodie. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -18095,15 +18120,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def horse(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon horse. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -18118,15 +18143,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def hospital(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon hospital. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -18141,15 +18166,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def hourglass(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon hourglass. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -18164,15 +18189,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def hourglass_high(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon hourglass-high. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -18187,15 +18212,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def hourglass_low(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon hourglass-low. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -18210,15 +18235,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def hourglass_medium(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon hourglass-medium. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -18233,15 +18258,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def hourglass_simple(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon hourglass-simple. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -18256,15 +18281,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def hourglass_simple_high(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon hourglass-simple-high. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -18279,15 +18304,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def hourglass_simple_low(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon hourglass-simple-low. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -18302,15 +18327,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def hourglass_simple_medium(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon hourglass-simple-medium. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -18325,15 +18350,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def house(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon house. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -18348,15 +18373,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def house_line(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon house-line. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -18371,15 +18396,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def house_simple(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon house-simple. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -18394,15 +18419,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def hurricane(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon hurricane. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -18417,15 +18442,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def ice_cream(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon ice-cream. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -18440,15 +18465,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def identification_badge(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon identification-badge. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -18463,15 +18488,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def identification_card(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon identification-card. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -18486,15 +18511,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def image(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon image. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -18509,15 +18534,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def image_broken(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon image-broken. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -18532,15 +18557,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def image_square(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon image-square. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -18555,15 +18580,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def images(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon images. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -18578,15 +18603,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def images_square(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon images-square. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -18601,15 +18626,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def infinity(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon infinity. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -18624,15 +18649,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def lemniscate(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon lemniscate. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -18647,15 +18672,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def info(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon info. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -18670,15 +18695,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def instagram_logo(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon instagram-logo. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -18693,15 +18718,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def intersect(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon intersect. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -18716,15 +18741,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def intersect_square(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon intersect-square. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -18739,15 +18764,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def intersect_three(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon intersect-three. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -18762,15 +18787,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def intersection(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon intersection. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -18785,15 +18810,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def invoice(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon invoice. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -18808,15 +18833,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def island(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon island. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -18831,15 +18856,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def jar(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon jar. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -18854,15 +18879,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def jar_label(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon jar-label. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -18877,15 +18902,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def jeep(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon jeep. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -18900,15 +18925,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def joystick(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon joystick. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -18923,15 +18948,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def kanban(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon kanban. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -18946,15 +18971,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def key(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon key. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -18969,15 +18994,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def key_return(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon key-return. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -18992,15 +19017,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def keyboard(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon keyboard. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -19015,15 +19040,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def keyhole(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon keyhole. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -19038,15 +19063,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def knife(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon knife. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -19061,15 +19086,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def ladder(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon ladder. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -19084,15 +19109,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def ladder_simple(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon ladder-simple. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -19107,15 +19132,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def lamp(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon lamp. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -19130,15 +19155,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def lamp_pendant(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon lamp-pendant. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -19153,15 +19178,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def laptop(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon laptop. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -19176,15 +19201,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def lasso(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon lasso. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -19199,15 +19224,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def lastfm_logo(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon lastfm-logo. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -19222,15 +19247,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def layout(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon layout. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -19245,15 +19270,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def leaf(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon leaf. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -19268,15 +19293,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def lectern(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon lectern. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -19291,15 +19316,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def lego(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon lego. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -19314,15 +19339,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def lego_smiley(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon lego-smiley. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -19337,15 +19362,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def less_than(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon less-than. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -19360,15 +19385,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def less_than_or_equal(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon less-than-or-equal. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -19383,15 +19408,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def letter_circle_h(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon letter-circle-h. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -19406,15 +19431,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def letter_circle_p(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon letter-circle-p. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -19429,15 +19454,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def letter_circle_v(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon letter-circle-v. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -19452,15 +19477,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def lifebuoy(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon lifebuoy. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -19475,15 +19500,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def lightbulb(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon lightbulb. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -19498,15 +19523,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def lightbulb_filament(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon lightbulb-filament. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -19521,15 +19546,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def lighthouse(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon lighthouse. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -19544,15 +19569,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def lightning(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon lightning. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -19567,15 +19592,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def lightning_a(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon lightning-a. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -19590,15 +19615,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def lightning_slash(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon lightning-slash. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -19613,15 +19638,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def line_segment(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon line-segment. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -19636,15 +19661,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def line_segments(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon line-segments. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -19659,15 +19684,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def line_vertical(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon line-vertical. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -19682,15 +19707,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def link(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon link. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -19705,15 +19730,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def link_break(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon link-break. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -19728,15 +19753,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def link_simple(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon link-simple. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -19751,15 +19776,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def link_simple_break(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon link-simple-break. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -19774,15 +19799,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def link_simple_horizontal(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon link-simple-horizontal. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -19797,15 +19822,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def link_simple_horizontal_break(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon link-simple-horizontal-break. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -19820,15 +19845,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def linkedin_logo(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon linkedin-logo. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -19843,15 +19868,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def linktree_logo(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon linktree-logo. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -19866,15 +19891,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def linux_logo(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon linux-logo. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -19889,15 +19914,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def list(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon list. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -19912,15 +19937,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def list_bullets(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon list-bullets. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -19935,15 +19960,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def list_checks(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon list-checks. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -19958,15 +19983,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def list_dashes(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon list-dashes. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -19981,15 +20006,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def list_heart(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon list-heart. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -20004,15 +20029,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def list_magnifying_glass(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon list-magnifying-glass. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -20027,15 +20052,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def list_numbers(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon list-numbers. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -20050,15 +20075,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def list_plus(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon list-plus. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -20073,15 +20098,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def list_star(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon list-star. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -20096,15 +20121,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def lock(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon lock. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -20119,15 +20144,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def lock_key(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon lock-key. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -20142,15 +20167,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def lock_key_open(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon lock-key-open. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -20165,15 +20190,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def lock_laminated(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon lock-laminated. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -20188,15 +20213,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def lock_laminated_open(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon lock-laminated-open. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -20211,15 +20236,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def lock_open(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon lock-open. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -20234,15 +20259,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def lock_simple(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon lock-simple. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -20257,15 +20282,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def lock_simple_open(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon lock-simple-open. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -20280,15 +20305,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def lockers(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon lockers. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -20303,15 +20328,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def log(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon log. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -20326,15 +20351,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def magic_wand(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon magic-wand. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -20349,15 +20374,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def magnet(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon magnet. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -20372,15 +20397,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def magnet_straight(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon magnet-straight. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -20395,15 +20420,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def magnifying_glass(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon magnifying-glass. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -20418,15 +20443,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def magnifying_glass_minus(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon magnifying-glass-minus. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -20441,15 +20466,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def magnifying_glass_plus(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon magnifying-glass-plus. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -20464,15 +20489,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def mailbox(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon mailbox. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -20487,15 +20512,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def map_pin(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon map-pin. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -20510,15 +20535,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def map_pin_area(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon map-pin-area. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -20533,15 +20558,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def map_pin_line(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon map-pin-line. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -20556,15 +20581,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def map_pin_plus(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon map-pin-plus. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -20579,15 +20604,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def map_pin_simple(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon map-pin-simple. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -20602,15 +20627,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def map_pin_simple_area(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon map-pin-simple-area. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -20625,15 +20650,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def map_pin_simple_line(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon map-pin-simple-line. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -20648,15 +20673,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def map_trifold(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon map-trifold. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -20671,15 +20696,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def markdown_logo(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon markdown-logo. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -20694,15 +20719,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def marker_circle(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon marker-circle. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -20717,15 +20742,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def martini(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon martini. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -20740,15 +20765,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def mask_happy(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon mask-happy. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -20763,15 +20788,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def mask_sad(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon mask-sad. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -20786,15 +20811,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def mastodon_logo(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon mastodon-logo. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -20809,15 +20834,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def math_operations(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon math-operations. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -20832,15 +20857,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def matrix_logo(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon matrix-logo. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -20855,15 +20880,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def medal(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon medal. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -20878,15 +20903,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def medal_military(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon medal-military. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -20901,15 +20926,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def medium_logo(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon medium-logo. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -20924,15 +20949,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def megaphone(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon megaphone. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -20947,15 +20972,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def megaphone_simple(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon megaphone-simple. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -20970,15 +20995,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def member_of(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon member-of. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -20993,15 +21018,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def memory(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon memory. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -21016,15 +21041,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def messenger_logo(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon messenger-logo. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -21039,15 +21064,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def meta_logo(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon meta-logo. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -21062,15 +21087,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def meteor(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon meteor. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -21085,15 +21110,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def metronome(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon metronome. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -21108,15 +21133,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def microphone(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon microphone. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -21131,15 +21156,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def microphone_slash(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon microphone-slash. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -21154,15 +21179,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def microphone_stage(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon microphone-stage. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -21177,15 +21202,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def microscope(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon microscope. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -21200,15 +21225,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def microsoft_excel_logo(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon microsoft-excel-logo. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -21223,15 +21248,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def microsoft_outlook_logo(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon microsoft-outlook-logo. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -21246,15 +21271,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def microsoft_powerpoint_logo(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon microsoft-powerpoint-logo. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -21269,15 +21294,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def microsoft_teams_logo(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon microsoft-teams-logo. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -21292,15 +21317,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def microsoft_word_logo(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon microsoft-word-logo. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -21315,15 +21340,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def minus(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon minus. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -21338,15 +21363,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def minus_circle(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon minus-circle. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -21361,15 +21386,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def minus_square(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon minus-square. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -21384,15 +21409,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def money(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon money. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -21407,15 +21432,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def money_wavy(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon money-wavy. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -21430,15 +21455,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def monitor(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon monitor. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -21453,15 +21478,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def monitor_arrow_up(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon monitor-arrow-up. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -21476,15 +21501,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def monitor_play(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon monitor-play. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -21499,15 +21524,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def moon(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon moon. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -21522,15 +21547,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def moon_stars(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon moon-stars. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -21545,15 +21570,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def moped(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon moped. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -21568,15 +21593,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def moped_front(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon moped-front. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -21591,15 +21616,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def mosque(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon mosque. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -21614,15 +21639,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def motorcycle(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon motorcycle. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -21637,15 +21662,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def mountains(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon mountains. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -21660,15 +21685,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def mouse(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon mouse. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -21683,15 +21708,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def mouse_left_click(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon mouse-left-click. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -21706,15 +21731,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def mouse_middle_click(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon mouse-middle-click. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -21729,15 +21754,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def mouse_right_click(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon mouse-right-click. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -21752,15 +21777,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def mouse_scroll(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon mouse-scroll. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -21775,15 +21800,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def mouse_simple(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon mouse-simple. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -21798,15 +21823,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def music_note(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon music-note. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -21821,15 +21846,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def music_note_simple(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon music-note-simple. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -21844,15 +21869,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def music_notes(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon music-notes. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -21867,15 +21892,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def music_notes_minus(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon music-notes-minus. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -21890,15 +21915,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def music_notes_plus(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon music-notes-plus. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -21913,15 +21938,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def music_notes_simple(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon music-notes-simple. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -21936,15 +21961,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def navigation_arrow(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon navigation-arrow. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -21959,15 +21984,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def needle(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon needle. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -21982,15 +22007,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def network(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon network. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -22005,15 +22030,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def network_slash(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon network-slash. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -22028,15 +22053,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def network_x(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon network-x. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -22051,15 +22076,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def newspaper(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon newspaper. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -22074,15 +22099,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def newspaper_clipping(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon newspaper-clipping. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -22097,15 +22122,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def not_equals(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon not-equals. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -22120,15 +22145,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def not_member_of(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon not-member-of. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -22143,15 +22168,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def not_subset_of(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon not-subset-of. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -22166,15 +22191,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def not_superset_of(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon not-superset-of. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -22189,15 +22214,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def notches(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon notches. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -22212,15 +22237,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def note(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon note. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -22235,15 +22260,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def note_blank(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon note-blank. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -22258,15 +22283,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def note_pencil(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon note-pencil. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -22281,15 +22306,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def notebook(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon notebook. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -22304,15 +22329,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def notepad(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon notepad. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -22327,15 +22352,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def notification(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon notification. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -22350,15 +22375,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def notion_logo(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon notion-logo. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -22373,15 +22398,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def nuclear_plant(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon nuclear-plant. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -22396,15 +22421,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def number_circle_eight(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon number-circle-eight. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -22419,15 +22444,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def number_circle_five(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon number-circle-five. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -22442,15 +22467,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def number_circle_four(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon number-circle-four. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -22465,15 +22490,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def number_circle_nine(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon number-circle-nine. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -22488,15 +22513,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def number_circle_one(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon number-circle-one. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -22511,15 +22536,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def number_circle_seven(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon number-circle-seven. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -22534,15 +22559,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def number_circle_six(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon number-circle-six. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -22557,15 +22582,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def number_circle_three(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon number-circle-three. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -22580,15 +22605,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def number_circle_two(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon number-circle-two. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -22603,15 +22628,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def number_circle_zero(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon number-circle-zero. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -22626,15 +22651,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def number_eight(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon number-eight. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -22649,15 +22674,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def number_five(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon number-five. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -22672,15 +22697,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def number_four(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon number-four. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -22695,15 +22720,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def number_nine(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon number-nine. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -22718,15 +22743,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def number_one(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon number-one. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -22741,15 +22766,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def number_seven(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon number-seven. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -22764,15 +22789,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def number_six(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon number-six. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -22787,15 +22812,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def number_square_eight(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon number-square-eight. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -22810,15 +22835,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def number_square_five(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon number-square-five. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -22833,15 +22858,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def number_square_four(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon number-square-four. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -22856,15 +22881,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def number_square_nine(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon number-square-nine. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -22879,15 +22904,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def number_square_one(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon number-square-one. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -22902,15 +22927,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def number_square_seven(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon number-square-seven. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -22925,15 +22950,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def number_square_six(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon number-square-six. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -22948,15 +22973,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def number_square_three(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon number-square-three. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -22971,15 +22996,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def number_square_two(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon number-square-two. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -22994,15 +23019,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def number_square_zero(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon number-square-zero. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -23017,15 +23042,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def number_three(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon number-three. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -23040,15 +23065,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def number_two(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon number-two. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -23063,15 +23088,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def number_zero(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon number-zero. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -23086,15 +23111,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def numpad(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon numpad. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -23109,15 +23134,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def nut(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon nut. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -23132,15 +23157,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def ny_times_logo(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon ny-times-logo. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -23155,15 +23180,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def octagon(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon octagon. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -23178,15 +23203,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def office_chair(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon office-chair. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -23201,15 +23226,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def onigiri(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon onigiri. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -23224,15 +23249,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def open_ai_logo(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon open-ai-logo. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -23247,15 +23272,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def option(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon option. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -23270,15 +23295,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def orange(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon orange. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -23293,15 +23318,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def orange_slice(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon orange-slice. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -23316,15 +23341,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def oven(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon oven. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -23339,15 +23364,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def package(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon package. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -23362,15 +23387,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def paint_brush(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon paint-brush. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -23385,15 +23410,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def paint_brush_broad(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon paint-brush-broad. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -23408,15 +23433,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def paint_brush_household(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon paint-brush-household. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -23431,15 +23456,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def paint_bucket(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon paint-bucket. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -23454,15 +23479,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def paint_roller(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon paint-roller. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -23477,15 +23502,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def palette(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon palette. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -23500,15 +23525,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def panorama(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon panorama. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -23523,15 +23548,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def pants(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon pants. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -23546,15 +23571,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def paper_plane(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon paper-plane. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -23569,15 +23594,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def paper_plane_right(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon paper-plane-right. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -23592,15 +23617,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def paper_plane_tilt(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon paper-plane-tilt. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -23615,15 +23640,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def paperclip(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon paperclip. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -23638,15 +23663,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def paperclip_horizontal(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon paperclip-horizontal. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -23661,15 +23686,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def parachute(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon parachute. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -23684,15 +23709,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def paragraph(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon paragraph. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -23707,15 +23732,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def parallelogram(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon parallelogram. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -23730,15 +23755,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def park(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon park. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -23753,15 +23778,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def password(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon password. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -23776,15 +23801,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def path(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon path. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -23799,15 +23824,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def patreon_logo(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon patreon-logo. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -23822,15 +23847,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def pause(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon pause. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -23845,15 +23870,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def pause_circle(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon pause-circle. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -23868,15 +23893,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def paw_print(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon paw-print. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -23891,15 +23916,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def paypal_logo(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon paypal-logo. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -23914,15 +23939,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def peace(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon peace. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -23937,15 +23962,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def pen(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon pen. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -23960,15 +23985,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def pen_nib(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon pen-nib. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -23983,15 +24008,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def pen_nib_straight(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon pen-nib-straight. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -24006,15 +24031,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def pencil(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon pencil. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -24029,15 +24054,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def pencil_circle(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon pencil-circle. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -24052,15 +24077,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def pencil_line(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon pencil-line. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -24075,15 +24100,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def pencil_ruler(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon pencil-ruler. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -24098,15 +24123,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def pencil_simple(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon pencil-simple. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -24121,15 +24146,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def pencil_simple_line(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon pencil-simple-line. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -24144,15 +24169,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def pencil_simple_slash(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon pencil-simple-slash. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -24167,15 +24192,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def pencil_slash(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon pencil-slash. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -24190,15 +24215,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def pentagon(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon pentagon. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -24213,15 +24238,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def pentagram(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon pentagram. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -24236,15 +24261,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def pepper(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon pepper. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -24259,15 +24284,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def percent(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon percent. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -24282,15 +24307,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def person(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon person. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -24305,15 +24330,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def person_arms_spread(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon person-arms-spread. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -24328,15 +24353,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def person_simple(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon person-simple. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -24351,15 +24376,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def person_simple_bike(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon person-simple-bike. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -24374,15 +24399,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def person_simple_circle(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon person-simple-circle. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -24397,15 +24422,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def person_simple_hike(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon person-simple-hike. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -24420,15 +24445,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def person_simple_run(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon person-simple-run. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -24443,15 +24468,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def person_simple_ski(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon person-simple-ski. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -24466,15 +24491,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def person_simple_snowboard(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon person-simple-snowboard. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -24489,15 +24514,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def person_simple_swim(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon person-simple-swim. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -24512,15 +24537,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def person_simple_tai_chi(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon person-simple-tai-chi. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -24535,15 +24560,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def person_simple_throw(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon person-simple-throw. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -24558,15 +24583,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def person_simple_walk(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon person-simple-walk. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -24581,15 +24606,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def perspective(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon perspective. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -24604,15 +24629,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def phone(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon phone. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -24627,15 +24652,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def phone_call(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon phone-call. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -24650,15 +24675,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def phone_disconnect(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon phone-disconnect. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -24673,15 +24698,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def phone_incoming(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon phone-incoming. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -24696,15 +24721,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def phone_list(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon phone-list. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -24719,15 +24744,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def phone_outgoing(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon phone-outgoing. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -24742,15 +24767,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def phone_pause(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon phone-pause. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -24765,15 +24790,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def phone_plus(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon phone-plus. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -24788,15 +24813,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def phone_slash(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon phone-slash. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -24811,15 +24836,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def phone_transfer(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon phone-transfer. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -24834,15 +24859,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def phone_x(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon phone-x. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -24857,15 +24882,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def phosphor_logo(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon phosphor-logo. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -24880,15 +24905,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def pi(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon pi. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -24903,15 +24928,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def piano_keys(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon piano-keys. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -24926,15 +24951,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def picnic_table(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon picnic-table. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -24949,15 +24974,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def picture_in_picture(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon picture-in-picture. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -24972,15 +24997,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def piggy_bank(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon piggy-bank. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -24995,15 +25020,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def pill(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon pill. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -25018,15 +25043,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def ping_pong(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon ping-pong. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -25041,15 +25066,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def pint_glass(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon pint-glass. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -25064,15 +25089,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def pinterest_logo(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon pinterest-logo. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -25087,15 +25112,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def pinwheel(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon pinwheel. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -25110,15 +25135,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def pipe(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon pipe. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -25133,15 +25158,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def pipe_wrench(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon pipe-wrench. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -25156,15 +25181,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def pix_logo(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon pix-logo. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -25179,15 +25204,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def pizza(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon pizza. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -25202,15 +25227,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def placeholder(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon placeholder. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -25225,15 +25250,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def planet(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon planet. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -25248,15 +25273,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def plant(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon plant. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -25271,15 +25296,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def play(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon play. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -25294,15 +25319,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def play_circle(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon play-circle. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -25317,15 +25342,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def play_pause(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon play-pause. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -25340,15 +25365,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def playlist(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon playlist. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -25363,15 +25388,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def plug(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon plug. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -25386,15 +25411,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def plug_charging(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon plug-charging. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -25409,15 +25434,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def plugs(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon plugs. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -25432,15 +25457,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def plugs_connected(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon plugs-connected. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -25455,15 +25480,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def plus(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon plus. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -25478,15 +25503,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def plus_circle(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon plus-circle. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -25501,15 +25526,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def plus_minus(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon plus-minus. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -25524,15 +25549,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def plus_square(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon plus-square. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -25547,15 +25572,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def poker_chip(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon poker-chip. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -25570,15 +25595,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def police_car(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon police-car. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -25593,15 +25618,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def polygon(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon polygon. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -25616,15 +25641,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def popcorn(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon popcorn. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -25639,15 +25664,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def popsicle(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon popsicle. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -25662,15 +25687,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def potted_plant(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon potted-plant. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -25685,15 +25710,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def power(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon power. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -25708,15 +25733,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def prescription(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon prescription. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -25731,15 +25756,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def presentation(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon presentation. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -25754,15 +25779,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def presentation_chart(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon presentation-chart. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -25777,15 +25802,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def printer(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon printer. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -25800,15 +25825,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def prohibit(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon prohibit. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -25823,15 +25848,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def prohibit_inset(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon prohibit-inset. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -25846,15 +25871,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def projector_screen(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon projector-screen. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -25869,15 +25894,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def projector_screen_chart(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon projector-screen-chart. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -25892,15 +25917,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def pulse(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon pulse. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -25915,15 +25940,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def activity(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon activity. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -25938,15 +25963,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def push_pin(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon push-pin. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -25961,15 +25986,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def push_pin_simple(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon push-pin-simple. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -25984,15 +26009,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def push_pin_simple_slash(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon push-pin-simple-slash. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -26007,15 +26032,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def push_pin_slash(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon push-pin-slash. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -26030,15 +26055,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def puzzle_piece(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon puzzle-piece. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -26053,15 +26078,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def qr_code(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon qr-code. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -26076,15 +26101,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def question(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon question. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -26099,15 +26124,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def question_mark(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon question-mark. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -26122,15 +26147,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def queue(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon queue. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -26145,15 +26170,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def quotes(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon quotes. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -26168,15 +26193,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def rabbit(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon rabbit. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -26191,15 +26216,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def racquet(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon racquet. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -26214,15 +26239,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def radical(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon radical. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -26237,15 +26262,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def radio(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon radio. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -26260,15 +26285,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def radio_button(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon radio-button. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -26283,15 +26308,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def radioactive(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon radioactive. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -26306,15 +26331,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def rainbow(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon rainbow. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -26329,15 +26354,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def rainbow_cloud(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon rainbow-cloud. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -26352,15 +26377,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def ranking(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon ranking. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -26375,15 +26400,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def read_cv_logo(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon read-cv-logo. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -26398,15 +26423,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def receipt(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon receipt. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -26421,15 +26446,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def receipt_x(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon receipt-x. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -26444,15 +26469,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def record(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon record. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -26467,15 +26492,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def rectangle(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon rectangle. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -26490,15 +26515,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def rectangle_dashed(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon rectangle-dashed. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -26513,15 +26538,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def recycle(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon recycle. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -26536,15 +26561,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def reddit_logo(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon reddit-logo. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -26559,15 +26584,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def repeat(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon repeat. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -26582,15 +26607,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def repeat_once(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon repeat-once. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -26605,15 +26630,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def replit_logo(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon replit-logo. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -26628,15 +26653,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def resize(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon resize. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -26651,15 +26676,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def rewind(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon rewind. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -26674,15 +26699,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def rewind_circle(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon rewind-circle. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -26697,15 +26722,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def road_horizon(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon road-horizon. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -26720,15 +26745,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def robot(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon robot. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -26743,15 +26768,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def rocket(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon rocket. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -26766,15 +26791,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def rocket_launch(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon rocket-launch. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -26789,15 +26814,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def rows(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon rows. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -26812,15 +26837,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def rows_plus_bottom(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon rows-plus-bottom. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -26835,15 +26860,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def rows_plus_top(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon rows-plus-top. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -26858,15 +26883,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def rss(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon rss. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -26881,15 +26906,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def rss_simple(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon rss-simple. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -26904,15 +26929,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def rug(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon rug. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -26927,15 +26952,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def ruler(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon ruler. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -26950,15 +26975,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def sailboat(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon sailboat. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -26973,15 +26998,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def scales(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon scales. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -26996,15 +27021,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def scan(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon scan. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -27019,15 +27044,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def scan_smiley(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon scan-smiley. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -27042,15 +27067,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def scissors(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon scissors. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -27065,15 +27090,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def scooter(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon scooter. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -27088,15 +27113,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def screencast(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon screencast. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -27111,15 +27136,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def screwdriver(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon screwdriver. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -27134,15 +27159,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def scribble(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon scribble. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -27157,15 +27182,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def scribble_loop(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon scribble-loop. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -27180,15 +27205,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def scroll(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon scroll. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -27203,15 +27228,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def seal(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon seal. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -27226,15 +27251,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def circle_wavy(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon circle-wavy. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -27249,15 +27274,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def seal_check(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon seal-check. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -27272,15 +27297,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def circle_wavy_check(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon circle-wavy-check. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -27295,15 +27320,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def seal_percent(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon seal-percent. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -27318,15 +27343,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def seal_question(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon seal-question. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -27341,15 +27366,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def circle_wavy_question(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon circle-wavy-question. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -27364,15 +27389,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def seal_warning(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon seal-warning. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -27387,15 +27412,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def circle_wavy_warning(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon circle-wavy-warning. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -27410,15 +27435,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def seat(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon seat. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -27433,15 +27458,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def seatbelt(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon seatbelt. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -27456,15 +27481,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def security_camera(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon security-camera. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -27479,15 +27504,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def selection(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon selection. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -27502,15 +27527,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def selection_all(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon selection-all. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -27525,15 +27550,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def selection_background(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon selection-background. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -27548,15 +27573,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def selection_foreground(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon selection-foreground. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -27571,15 +27596,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def selection_inverse(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon selection-inverse. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -27594,15 +27619,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def selection_plus(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon selection-plus. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -27617,15 +27642,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def selection_slash(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon selection-slash. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -27640,15 +27665,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def shapes(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon shapes. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -27663,15 +27688,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def share(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon share. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -27686,15 +27711,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def share_fat(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon share-fat. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -27709,15 +27734,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def share_network(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon share-network. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -27732,15 +27757,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def shield(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon shield. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -27755,15 +27780,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def shield_check(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon shield-check. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -27778,15 +27803,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def shield_checkered(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon shield-checkered. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -27801,15 +27826,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def shield_chevron(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon shield-chevron. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -27824,15 +27849,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def shield_plus(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon shield-plus. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -27847,15 +27872,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def shield_slash(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon shield-slash. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -27870,15 +27895,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def shield_star(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon shield-star. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -27893,15 +27918,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def shield_warning(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon shield-warning. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -27916,15 +27941,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def shipping_container(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon shipping-container. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -27939,15 +27964,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def shirt_folded(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon shirt-folded. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -27962,15 +27987,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def shooting_star(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon shooting-star. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -27985,15 +28010,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def shopping_bag(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon shopping-bag. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -28008,15 +28033,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def shopping_bag_open(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon shopping-bag-open. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -28031,15 +28056,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def shopping_cart(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon shopping-cart. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -28054,15 +28079,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def shopping_cart_simple(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon shopping-cart-simple. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -28077,15 +28102,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def shovel(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon shovel. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -28100,15 +28125,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def shower(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon shower. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -28123,15 +28148,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def shrimp(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon shrimp. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -28146,15 +28171,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def shuffle(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon shuffle. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -28169,15 +28194,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def shuffle_angular(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon shuffle-angular. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -28192,15 +28217,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def shuffle_simple(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon shuffle-simple. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -28215,15 +28240,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def sidebar(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon sidebar. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -28238,15 +28263,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def sidebar_simple(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon sidebar-simple. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -28261,15 +28286,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def sigma(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon sigma. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -28284,15 +28309,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def sign_in(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon sign-in. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -28307,15 +28332,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def sign_out(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon sign-out. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -28330,15 +28355,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def signature(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon signature. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -28353,15 +28378,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def signpost(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon signpost. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -28376,15 +28401,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def sim_card(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon sim-card. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -28399,15 +28424,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def siren(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon siren. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -28422,15 +28447,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def sketch_logo(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon sketch-logo. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -28445,15 +28470,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def skip_back(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon skip-back. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -28468,15 +28493,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def skip_back_circle(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon skip-back-circle. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -28491,15 +28516,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def skip_forward(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon skip-forward. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -28514,15 +28539,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def skip_forward_circle(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon skip-forward-circle. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -28537,15 +28562,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def skull(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon skull. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -28560,15 +28585,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def skype_logo(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon skype-logo. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -28583,15 +28608,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def slack_logo(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon slack-logo. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -28606,15 +28631,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def sliders(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon sliders. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -28629,15 +28654,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def sliders_horizontal(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon sliders-horizontal. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -28652,15 +28677,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def slideshow(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon slideshow. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -28675,15 +28700,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def smiley(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon smiley. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -28698,15 +28723,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def smiley_angry(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon smiley-angry. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -28721,15 +28746,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def smiley_blank(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon smiley-blank. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -28744,15 +28769,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def smiley_meh(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon smiley-meh. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -28767,15 +28792,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def smiley_melting(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon smiley-melting. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -28790,15 +28815,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def smiley_nervous(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon smiley-nervous. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -28813,15 +28838,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def smiley_sad(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon smiley-sad. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -28836,15 +28861,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def smiley_sticker(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon smiley-sticker. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -28859,15 +28884,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def smiley_wink(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon smiley-wink. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -28882,15 +28907,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def smiley_x_eyes(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon smiley-x-eyes. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -28905,15 +28930,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def snapchat_logo(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon snapchat-logo. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -28928,15 +28953,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def sneaker(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon sneaker. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -28951,15 +28976,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def sneaker_move(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon sneaker-move. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -28974,15 +28999,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def snowflake(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon snowflake. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -28997,15 +29022,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def soccer_ball(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon soccer-ball. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -29020,15 +29045,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def sock(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon sock. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -29043,15 +29068,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def solar_panel(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon solar-panel. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -29066,15 +29091,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def solar_roof(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon solar-roof. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -29089,15 +29114,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def sort_ascending(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon sort-ascending. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -29112,15 +29137,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def sort_descending(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon sort-descending. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -29135,15 +29160,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def soundcloud_logo(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon soundcloud-logo. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -29158,15 +29183,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def spade(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon spade. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -29181,15 +29206,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def sparkle(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon sparkle. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -29204,15 +29229,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def speaker_hifi(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon speaker-hifi. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -29227,15 +29252,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def speaker_high(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon speaker-high. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -29250,15 +29275,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def speaker_low(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon speaker-low. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -29273,15 +29298,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def speaker_none(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon speaker-none. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -29296,15 +29321,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def speaker_simple_high(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon speaker-simple-high. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -29319,15 +29344,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def speaker_simple_low(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon speaker-simple-low. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -29342,15 +29367,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def speaker_simple_none(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon speaker-simple-none. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -29365,15 +29390,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def speaker_simple_slash(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon speaker-simple-slash. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -29388,15 +29413,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def speaker_simple_x(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon speaker-simple-x. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -29411,15 +29436,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def speaker_slash(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon speaker-slash. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -29434,15 +29459,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def speaker_x(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon speaker-x. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -29457,15 +29482,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def speedometer(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon speedometer. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -29480,15 +29505,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def sphere(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon sphere. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -29503,15 +29528,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def spinner(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon spinner. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -29526,15 +29551,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def spinner_ball(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon spinner-ball. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -29549,15 +29574,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def spinner_gap(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon spinner-gap. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -29572,15 +29597,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def spiral(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon spiral. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -29595,15 +29620,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def split_horizontal(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon split-horizontal. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -29618,15 +29643,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def split_vertical(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon split-vertical. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -29641,15 +29666,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def spotify_logo(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon spotify-logo. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -29664,15 +29689,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def spray_bottle(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon spray-bottle. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -29687,15 +29712,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def square(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon square. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -29710,15 +29735,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def square_half(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon square-half. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -29733,15 +29758,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def square_half_bottom(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon square-half-bottom. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -29756,15 +29781,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def square_logo(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon square-logo. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -29779,15 +29804,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def square_split_horizontal(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon square-split-horizontal. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -29802,15 +29827,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def square_split_vertical(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon square-split-vertical. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -29825,15 +29850,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def squares_four(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon squares-four. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -29848,15 +29873,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def stack(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon stack. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -29871,15 +29896,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def stack_minus(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon stack-minus. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -29894,15 +29919,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def stack_overflow_logo(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon stack-overflow-logo. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -29917,15 +29942,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def stack_plus(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon stack-plus. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -29940,15 +29965,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def stack_simple(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon stack-simple. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -29963,15 +29988,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def stairs(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon stairs. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -29986,15 +30011,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def stamp(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon stamp. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -30009,15 +30034,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def standard_definition(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon standard-definition. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -30032,15 +30057,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def star(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon star. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -30055,15 +30080,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def star_and_crescent(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon star-and-crescent. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -30078,15 +30103,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def star_four(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon star-four. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -30101,15 +30126,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def star_half(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon star-half. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -30124,15 +30149,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def star_of_david(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon star-of-david. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -30147,15 +30172,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def steam_logo(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon steam-logo. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -30170,15 +30195,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def steering_wheel(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon steering-wheel. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -30193,15 +30218,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def steps(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon steps. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -30216,15 +30241,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def stethoscope(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon stethoscope. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -30239,15 +30264,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def sticker(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon sticker. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -30262,15 +30287,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def stool(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon stool. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -30285,15 +30310,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def stop(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon stop. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -30308,15 +30333,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def stop_circle(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon stop-circle. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -30331,15 +30356,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def storefront(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon storefront. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -30354,15 +30379,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def strategy(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon strategy. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -30377,15 +30402,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def stripe_logo(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon stripe-logo. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -30400,15 +30425,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def student(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon student. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -30423,15 +30448,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def subset_of(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon subset-of. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -30446,15 +30471,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def subset_proper_of(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon subset-proper-of. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -30469,15 +30494,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def subtitles(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon subtitles. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -30492,15 +30517,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def subtitles_slash(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon subtitles-slash. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -30515,15 +30540,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def subtract(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon subtract. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -30538,15 +30563,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def subtract_square(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon subtract-square. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -30561,15 +30586,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def subway(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon subway. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -30584,15 +30609,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def suitcase(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon suitcase. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -30607,15 +30632,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def suitcase_rolling(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon suitcase-rolling. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -30630,15 +30655,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def suitcase_simple(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon suitcase-simple. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -30653,15 +30678,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def sun(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon sun. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -30676,15 +30701,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def sun_dim(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon sun-dim. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -30699,15 +30724,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def sun_horizon(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon sun-horizon. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -30722,15 +30747,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def sunglasses(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon sunglasses. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -30745,15 +30770,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def superset_of(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon superset-of. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -30768,15 +30793,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def superset_proper_of(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon superset-proper-of. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -30791,15 +30816,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def swap(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon swap. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -30814,15 +30839,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def swatches(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon swatches. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -30837,15 +30862,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def swimming_pool(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon swimming-pool. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -30860,15 +30885,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def sword(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon sword. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -30883,15 +30908,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def synagogue(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon synagogue. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -30906,15 +30931,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def syringe(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon syringe. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -30929,15 +30954,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def t_shirt(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon t-shirt. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -30952,15 +30977,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def table(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon table. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -30975,15 +31000,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def tabs(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon tabs. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -30998,15 +31023,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def tag(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon tag. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -31021,15 +31046,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def tag_chevron(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon tag-chevron. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -31044,15 +31069,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def tag_simple(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon tag-simple. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -31067,15 +31092,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def target(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon target. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -31090,15 +31115,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def taxi(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon taxi. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -31113,15 +31138,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def tea_bag(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon tea-bag. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -31136,15 +31161,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def telegram_logo(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon telegram-logo. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -31159,15 +31184,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def television(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon television. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -31182,15 +31207,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def television_simple(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon television-simple. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -31205,15 +31230,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def tennis_ball(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon tennis-ball. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -31228,15 +31253,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def tent(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon tent. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -31251,15 +31276,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def terminal(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon terminal. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -31274,15 +31299,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def terminal_window(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon terminal-window. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -31297,15 +31322,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def test_tube(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon test-tube. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -31320,15 +31345,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def text_a_underline(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon text-a-underline. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -31343,15 +31368,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def text_aa(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon text-aa. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -31366,15 +31391,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def text_align_center(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon text-align-center. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -31389,15 +31414,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def text_align_justify(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon text-align-justify. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -31412,15 +31437,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def text_align_left(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon text-align-left. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -31435,15 +31460,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def text_align_right(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon text-align-right. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -31458,15 +31483,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def text_b(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon text-b. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -31481,15 +31506,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def text_bolder(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon text-bolder. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -31504,15 +31529,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def text_columns(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon text-columns. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -31527,15 +31552,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def text_h(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon text-h. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -31550,15 +31575,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def text_h_five(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon text-h-five. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -31573,15 +31598,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def text_h_four(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon text-h-four. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -31596,15 +31621,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def text_h_one(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon text-h-one. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -31619,15 +31644,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def text_h_six(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon text-h-six. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -31642,15 +31667,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def text_h_three(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon text-h-three. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -31665,15 +31690,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def text_h_two(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon text-h-two. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -31688,15 +31713,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def text_indent(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon text-indent. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -31711,15 +31736,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def text_italic(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon text-italic. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -31734,15 +31759,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def text_outdent(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon text-outdent. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -31757,15 +31782,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def text_strikethrough(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon text-strikethrough. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -31780,15 +31805,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def text_subscript(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon text-subscript. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -31803,15 +31828,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def text_superscript(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon text-superscript. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -31826,15 +31851,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def text_t(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon text-t. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -31849,15 +31874,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def text_t_slash(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon text-t-slash. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -31872,15 +31897,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def text_underline(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon text-underline. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -31895,15 +31920,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def textbox(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon textbox. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -31918,15 +31943,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def thermometer(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon thermometer. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -31941,15 +31966,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def thermometer_cold(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon thermometer-cold. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -31964,15 +31989,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def thermometer_hot(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon thermometer-hot. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -31987,15 +32012,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def thermometer_simple(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon thermometer-simple. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -32010,15 +32035,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def threads_logo(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon threads-logo. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -32033,15 +32058,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def three_d(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon three-d. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -32056,15 +32081,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def thumbs_down(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon thumbs-down. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -32079,15 +32104,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def thumbs_up(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon thumbs-up. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -32102,15 +32127,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def ticket(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon ticket. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -32125,15 +32150,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def tidal_logo(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon tidal-logo. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -32148,15 +32173,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def tiktok_logo(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon tiktok-logo. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -32171,15 +32196,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def tilde(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon tilde. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -32194,15 +32219,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def timer(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon timer. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -32217,15 +32242,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def tip_jar(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon tip-jar. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -32240,15 +32265,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def tipi(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon tipi. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -32263,15 +32288,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def tire(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon tire. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -32286,15 +32311,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def toggle_left(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon toggle-left. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -32309,15 +32334,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def toggle_right(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon toggle-right. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -32332,15 +32357,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def toilet(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon toilet. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -32355,15 +32380,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def toilet_paper(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon toilet-paper. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -32378,15 +32403,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def toolbox(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon toolbox. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -32401,15 +32426,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def tooth(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon tooth. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -32424,15 +32449,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def tornado(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon tornado. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -32447,15 +32472,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def tote(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon tote. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -32470,15 +32495,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def tote_simple(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon tote-simple. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -32493,15 +32518,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def towel(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon towel. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -32516,15 +32541,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def tractor(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon tractor. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -32539,15 +32564,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def trademark(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon trademark. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -32562,15 +32587,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def trademark_registered(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon trademark-registered. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -32585,15 +32610,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def traffic_cone(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon traffic-cone. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -32608,15 +32633,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def traffic_sign(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon traffic-sign. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -32631,15 +32656,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def traffic_signal(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon traffic-signal. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -32654,15 +32679,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def train(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon train. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -32677,15 +32702,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def train_regional(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon train-regional. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -32700,15 +32725,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def train_simple(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon train-simple. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -32723,15 +32748,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def tram(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon tram. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -32746,15 +32771,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def translate(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon translate. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -32769,15 +32794,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def trash(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon trash. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -32792,15 +32817,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def trash_simple(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon trash-simple. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -32815,15 +32840,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def tray(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon tray. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -32838,15 +32863,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def tray_arrow_down(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon tray-arrow-down. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -32861,15 +32886,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def archive_tray(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon archive-tray. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -32884,15 +32909,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def tray_arrow_up(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon tray-arrow-up. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -32907,15 +32932,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def treasure_chest(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon treasure-chest. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -32930,15 +32955,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def tree(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon tree. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -32953,15 +32978,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def tree_evergreen(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon tree-evergreen. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -32976,15 +33001,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def tree_palm(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon tree-palm. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -32999,15 +33024,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def tree_structure(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon tree-structure. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -33022,15 +33047,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def tree_view(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon tree-view. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -33045,15 +33070,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def trend_down(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon trend-down. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -33068,15 +33093,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def trend_up(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon trend-up. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -33091,15 +33116,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def triangle(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon triangle. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -33114,15 +33139,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def triangle_dashed(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon triangle-dashed. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -33137,15 +33162,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def trolley(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon trolley. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -33160,15 +33185,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def trolley_suitcase(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon trolley-suitcase. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -33183,15 +33208,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def trophy(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon trophy. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -33206,15 +33231,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def truck(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon truck. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -33229,15 +33254,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def truck_trailer(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon truck-trailer. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -33252,15 +33277,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def tumblr_logo(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon tumblr-logo. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -33275,15 +33300,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def twitch_logo(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon twitch-logo. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -33298,15 +33323,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def twitter_logo(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon twitter-logo. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -33321,15 +33346,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def umbrella(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon umbrella. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -33344,15 +33369,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def umbrella_simple(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon umbrella-simple. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -33367,15 +33392,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def union(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon union. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -33390,15 +33415,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def unite(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon unite. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -33413,15 +33438,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def unite_square(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon unite-square. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -33436,15 +33461,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def upload(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon upload. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -33459,15 +33484,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def upload_simple(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon upload-simple. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -33482,15 +33507,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def usb(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon usb. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -33505,15 +33530,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def user(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon user. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -33528,15 +33553,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def user_check(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon user-check. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -33551,15 +33576,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def user_circle(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon user-circle. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -33574,15 +33599,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def user_circle_check(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon user-circle-check. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -33597,15 +33622,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def user_circle_dashed(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon user-circle-dashed. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -33620,15 +33645,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def user_circle_gear(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon user-circle-gear. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -33643,15 +33668,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def user_circle_minus(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon user-circle-minus. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -33666,15 +33691,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def user_circle_plus(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon user-circle-plus. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -33689,15 +33714,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def user_focus(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon user-focus. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -33712,15 +33737,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def user_gear(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon user-gear. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -33735,15 +33760,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def user_list(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon user-list. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -33758,15 +33783,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def user_minus(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon user-minus. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -33781,15 +33806,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def user_plus(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon user-plus. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -33804,15 +33829,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def user_rectangle(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon user-rectangle. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -33827,15 +33852,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def user_sound(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon user-sound. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -33850,15 +33875,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def user_square(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon user-square. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -33873,15 +33898,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def user_switch(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon user-switch. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -33896,15 +33921,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def users(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon users. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -33919,15 +33944,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def users_four(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon users-four. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -33942,15 +33967,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def users_three(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon users-three. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -33965,15 +33990,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def van(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon van. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -33988,15 +34013,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def vault(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon vault. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -34011,15 +34036,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def vector_three(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon vector-three. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -34034,15 +34059,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def vector_two(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon vector-two. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -34057,15 +34082,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def vibrate(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon vibrate. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -34080,15 +34105,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def video(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon video. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -34103,15 +34128,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def video_camera(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon video-camera. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -34126,15 +34151,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def video_camera_slash(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon video-camera-slash. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -34149,15 +34174,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def video_conference(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon video-conference. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -34172,15 +34197,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def vignette(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon vignette. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -34195,15 +34220,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def vinyl_record(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon vinyl-record. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -34218,15 +34243,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def virtual_reality(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon virtual-reality. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -34241,15 +34266,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def virus(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon virus. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -34264,15 +34289,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def visor(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon visor. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -34287,15 +34312,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def voicemail(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon voicemail. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -34310,15 +34335,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def volleyball(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon volleyball. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -34333,15 +34358,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def wall(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon wall. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -34356,15 +34381,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def wallet(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon wallet. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -34379,15 +34404,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def warehouse(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon warehouse. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -34402,15 +34427,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def warning(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon warning. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -34425,15 +34450,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def warning_circle(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon warning-circle. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -34448,15 +34473,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def warning_diamond(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon warning-diamond. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -34471,15 +34496,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def warning_octagon(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon warning-octagon. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -34494,15 +34519,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def washing_machine(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon washing-machine. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -34517,15 +34542,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def watch(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon watch. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -34540,15 +34565,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def wave_sawtooth(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon wave-sawtooth. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -34563,15 +34588,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def wave_sine(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon wave-sine. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -34586,15 +34611,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def wave_square(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon wave-square. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -34609,15 +34634,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def wave_triangle(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon wave-triangle. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -34632,15 +34657,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def waveform(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon waveform. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -34655,15 +34680,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def waveform_slash(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon waveform-slash. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -34678,15 +34703,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def waves(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon waves. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -34701,15 +34726,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def webcam(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon webcam. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -34724,15 +34749,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def webcam_slash(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon webcam-slash. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -34747,15 +34772,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def webhooks_logo(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon webhooks-logo. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -34770,15 +34795,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def wechat_logo(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon wechat-logo. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -34793,15 +34818,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def whatsapp_logo(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon whatsapp-logo. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -34816,15 +34841,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def wheelchair(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon wheelchair. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -34839,15 +34864,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def wheelchair_motion(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon wheelchair-motion. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -34862,15 +34887,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def wifi_high(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon wifi-high. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -34885,15 +34910,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def wifi_low(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon wifi-low. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -34908,15 +34933,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def wifi_medium(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon wifi-medium. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -34931,15 +34956,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def wifi_none(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon wifi-none. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -34954,15 +34979,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def wifi_slash(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon wifi-slash. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -34977,15 +35002,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def wifi_x(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon wifi-x. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -35000,15 +35025,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def wind(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon wind. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -35023,15 +35048,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def windmill(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon windmill. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -35046,15 +35071,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def windows_logo(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon windows-logo. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -35069,15 +35094,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def wine(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon wine. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -35092,15 +35117,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def wrench(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon wrench. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -35115,15 +35140,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def x(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon x. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -35138,15 +35163,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def x_circle(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon x-circle. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -35161,15 +35186,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def x_logo(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon x-logo. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -35184,15 +35209,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def x_square(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon x-square. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -35207,15 +35232,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def yarn(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon yarn. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -35230,15 +35255,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def yin_yang(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon yin-yang. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
@@ -35253,15 +35278,15 @@
 
 
 @drawlib.v0_1.private.util.error_handler
 def youtube_logo(
     xy: typing.Tuple[float, float],
     width: float,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[drawlib.v0_1.private.core.model.IconStyle] = None,
+    style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
     """Draw phosphor icon youtube-logo. This is auto generated code.
 
     Args:
         xy: default align is center, center.
         width: horizontal icon size.
         angle: rotation. 0.0 ~ 360.0
```

### Comparing `drawlib-0.1.3/drawlib/v0_1/private/icons/util.py` & `drawlib-0.1.4/drawlib/v0_1/private/icons/util.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 def icon(
     xy: typing.Tuple[float, float],
     width: float,
     code: str,
     file: str,
     angle: typing.Optional[float] = None,
-    style: typing.Optional[IconStyle] = None,
+    style: typing.Union[IconStyle, str, None] = None,
 ) -> None:
     """Draw provided iconfont's icon.
 
     Args:
         code: code point
         font_file: font file path
         x: default align left if angle is not specified. center if specified.
@@ -51,14 +51,16 @@
     ArgValidator.validate_xy("xy", xy)
     ArgValidator.validate_float("width", width)
     ArgValidator.validate_str("code", code)
     ArgValidator.validate_str("file", file)
     if angle is not None:
         ArgValidator.validate_angle("angle", angle)
     if style is not None:
+        if isinstance(style, str):
+            style = dtheme.iconstyle_get(name=style)
         ArgValidator.validate_iconstyle("style", style)
 
     # set default parameters if not provided
 
     style = IconUtil.get_merged_style(style, dtheme.iconstyle_get())
     if style.halign is None:
         style.halign = "left" if angle is None else "center"
```

### Comparing `drawlib-0.1.3/drawlib/v0_1/private/logging.py` & `drawlib-0.1.4/drawlib/v0_1/private/logging.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.3/drawlib/v0_1/private/settings.py` & `drawlib-0.1.4/drawlib/v0_1/private/settings.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.3/drawlib/v0_1/private/smartarts/__init__.py` & `drawlib-0.1.4/drawlib/v0_1/private/smartarts/__init__.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.3/drawlib/v0_1/private/smartarts/dsart.py` & `drawlib-0.1.4/drawlib/v0_1/private/smartarts/dsart.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.3/drawlib/v0_1/private/smartarts/groups.py` & `drawlib-0.1.4/drawlib/v0_1/private/smartarts/groups.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.3/drawlib/v0_1/private/smartarts/pyramid.py` & `drawlib-0.1.4/drawlib/v0_1/private/smartarts/pyramid.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.3/drawlib/v0_1/private/smartarts/sourcecode.py` & `drawlib-0.1.4/drawlib/v0_1/private/smartarts/sourcecode.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.3/drawlib/v0_1/private/smartarts/tree.py` & `drawlib-0.1.4/drawlib/v0_1/private/smartarts/tree.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.3/drawlib/v0_1/private/tools.py` & `drawlib-0.1.4/drawlib/v0_1/private/tools.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.3/drawlib/v0_1/private/util.py` & `drawlib-0.1.4/drawlib/v0_1/private/util.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.3/pyproject.toml` & `drawlib-0.1.4/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "poetry-core",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "drawlib"
-version = "0.1.3"
+version = "0.1.4"
 description = "Python drawing library. Illustration as Code."
 homepage = "https://www.drawlib.com"
 repository = "https://github.com/yuichi110/drawlib"
 authors = [ "Yuichi Ito <yuichi@yuichi.com>",]
 readme = "README.md"
 
 [tool.black]
```

### Comparing `drawlib-0.1.3/PKG-INFO` & `drawlib-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drawlib
-Version: 0.1.3
+Version: 0.1.4
 Summary: Python drawing library. Illustration as Code.
 Home-page: https://www.drawlib.com
 Author: Yuichi Ito
 Author-email: yuichi@yuichi.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

