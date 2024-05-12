# Comparing `tmp/qtharmony-0.2.1.tar.gz` & `tmp/qtharmony-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qtharmony-0.2.1.tar", max compression
+gzip compressed data, was "qtharmony-0.2.2.tar", max compression
```

## Comparing `qtharmony-0.2.1.tar` & `qtharmony-0.2.2.tar`

### file list

```diff
@@ -1,53 +1,55 @@
--rw-r--r--   0        0        0     1067 2024-05-02 17:11:53.147941 qtharmony-0.2.1/LICENSE
--rw-r--r--   0        0        0     2050 2024-05-12 11:50:16.448380 qtharmony-0.2.1/README.md
--rw-r--r--   0        0        0      609 2024-05-12 11:59:05.305004 qtharmony-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      327 2024-05-11 05:40:26.229552 qtharmony-0.2.1/qtharmony/__init__.py
--rw-r--r--   0        0        0       38 2024-05-11 05:40:26.229552 qtharmony-0.2.1/qtharmony/constructor/__init__.py
--rw-r--r--   0        0        0      636 2024-05-12 06:38:54.294789 qtharmony-0.2.1/qtharmony/constructor/initialize.py
--rw-r--r--   0        0        0        2 2024-05-11 08:08:22.630008 qtharmony-0.2.1/qtharmony/resources/__init__.py
--rw-r--r--   0        0        0     4295 2024-05-12 11:50:16.451713 qtharmony-0.2.1/qtharmony/resources/themes/dark-default.json
--rw-r--r--   0        0        0     4563 2024-05-12 11:50:16.451713 qtharmony-0.2.1/qtharmony/resources/themes/light-default.json
--rw-r--r--   0        0        0    31042 2024-05-11 05:40:26.229552 qtharmony-0.2.1/qtharmony/resources/ui/Icon.png
--rw-r--r--   0        0        0    17484 2024-05-11 05:40:26.229552 qtharmony-0.2.1/qtharmony/resources/ui/Logo.png
--rw-r--r--   0        0        0     5387 2024-05-11 05:40:26.229552 qtharmony-0.2.1/qtharmony/resources/ui/angle-down.png
--rw-r--r--   0        0        0       22 2024-05-11 08:08:22.630008 qtharmony-0.2.1/qtharmony/src/config/__init__.py
--rw-r--r--   0        0        0      233 2024-05-11 14:21:59.267556 qtharmony-0.2.1/qtharmony/src/config/config.py
--rw-r--r--   0        0        0      120 2024-05-11 05:40:26.229552 qtharmony-0.2.1/qtharmony/src/core/__init__.py
--rw-r--r--   0        0        0      985 2024-05-11 05:40:26.232885 qtharmony-0.2.1/qtharmony/src/core/dialog.py
--rw-r--r--   0        0        0      151 2024-05-11 05:40:26.232885 qtharmony-0.2.1/qtharmony/src/core/exceptions.py
--rw-r--r--   0        0        0     2506 2024-05-11 05:40:26.232885 qtharmony-0.2.1/qtharmony/src/core/font.py
--rw-r--r--   0        0        0      876 2024-05-11 17:33:26.077741 qtharmony-0.2.1/qtharmony/src/core/load.py
--rw-r--r--   0        0        0      576 2024-05-12 11:50:16.451713 qtharmony-0.2.1/qtharmony/src/core/sizes.py
--rw-r--r--   0        0        0     1235 2024-05-12 07:41:31.423989 qtharmony-0.2.1/qtharmony/src/core/stylesheet.py
--rw-r--r--   0        0        0       80 2024-05-11 14:21:59.267556 qtharmony-0.2.1/qtharmony/src/core/theme/__init__.py
--rw-r--r--   0        0        0     1299 2024-05-11 14:29:14.506368 qtharmony-0.2.1/qtharmony/src/core/theme/theme_builder.py
--rw-r--r--   0        0        0     2096 2024-05-12 11:58:05.970970 qtharmony-0.2.1/qtharmony/src/core/theme/theme_manager.py
--rw-r--r--   0        0        0      464 2024-05-12 11:50:16.451713 qtharmony-0.2.1/qtharmony/widgets/__init__.py
--rw-r--r--   0        0        0     2316 2024-05-12 10:49:33.152065 qtharmony-0.2.1/qtharmony/widgets/basic/button.py
--rw-r--r--   0        0        0     2642 2024-05-12 07:41:31.423989 qtharmony-0.2.1/qtharmony/widgets/basic/check_box.py
--rw-r--r--   0        0        0     2492 2024-05-12 07:41:31.423989 qtharmony-0.2.1/qtharmony/widgets/basic/digital_entry.py
--rw-r--r--   0        0        0     3472 2024-05-12 11:50:16.451713 qtharmony-0.2.1/qtharmony/widgets/basic/drop_down_menu.py
--rw-r--r--   0        0        0     2489 2024-05-12 10:24:10.276814 qtharmony-0.2.1/qtharmony/widgets/basic/entry.py
--rw-r--r--   0        0        0      815 2024-05-12 11:50:16.451713 qtharmony-0.2.1/qtharmony/widgets/basic/frame.py
--rw-r--r--   0        0        0     2704 2024-05-12 11:50:16.451713 qtharmony-0.2.1/qtharmony/widgets/basic/groups.py
--rw-r--r--   0        0        0     3190 2024-05-12 11:50:16.451713 qtharmony-0.2.1/qtharmony/widgets/basic/label.py
--rw-r--r--   0        0        0     3784 2024-05-12 07:41:31.423989 qtharmony-0.2.1/qtharmony/widgets/basic/path_entry.py
--rw-r--r--   0        0        0     1922 2024-05-12 07:41:31.423989 qtharmony-0.2.1/qtharmony/widgets/basic/radio_button.py
--rw-r--r--   0        0        0     1994 2024-05-12 07:41:31.423989 qtharmony-0.2.1/qtharmony/widgets/basic/splitter.py
--rw-r--r--   0        0        0       61 2024-05-12 07:41:31.423989 qtharmony-0.2.1/qtharmony/widgets/basic/styles/button.css
--rw-r--r--   0        0        0      115 2024-05-12 06:38:54.304789 qtharmony-0.2.1/qtharmony/widgets/basic/styles/check_box.css
--rw-r--r--   0        0        0       63 2024-05-12 06:38:54.304789 qtharmony-0.2.1/qtharmony/widgets/basic/styles/digital_entry.css
--rw-r--r--   0        0        0      147 2024-05-12 11:50:16.451713 qtharmony-0.2.1/qtharmony/widgets/basic/styles/drop_down_menu.css
--rw-r--r--   0        0        0      108 2024-05-12 11:50:16.451713 qtharmony-0.2.1/qtharmony/widgets/basic/styles/entry.css
--rw-r--r--   0        0        0        0 2024-05-12 11:50:16.451713 qtharmony-0.2.1/qtharmony/widgets/basic/styles/frame.css
--rw-r--r--   0        0        0       60 2024-05-12 06:38:54.308122 qtharmony-0.2.1/qtharmony/widgets/basic/styles/group_box.css
--rw-r--r--   0        0        0       35 2024-05-11 06:45:00.352043 qtharmony-0.2.1/qtharmony/widgets/basic/styles/label.css
--rw-r--r--   0        0        0        0 2024-05-12 06:38:54.308122 qtharmony-0.2.1/qtharmony/widgets/basic/styles/path_entry.css
--rw-r--r--   0        0        0       67 2024-05-12 06:38:54.318122 qtharmony-0.2.1/qtharmony/widgets/basic/styles/radio_button.css
--rw-r--r--   0        0        0        0 2024-05-12 07:41:31.423989 qtharmony-0.2.1/qtharmony/widgets/basic/styles/splitter.css
--rw-r--r--   0        0        0      313 2024-05-11 05:40:26.236219 qtharmony-0.2.1/qtharmony/widgets/basic/styles/widgets_list.css
--rw-r--r--   0        0        0     1578 2024-05-11 05:40:26.236219 qtharmony-0.2.1/qtharmony/widgets/basic/widgets_list.py
--rw-r--r--   0        0        0       36 2024-05-11 05:40:26.236219 qtharmony-0.2.1/qtharmony/windows/__init__.py
--rw-r--r--   0        0        0     2692 2024-05-12 07:41:31.423989 qtharmony-0.2.1/qtharmony/windows/main_window.py
--rw-r--r--   0        0        0        0 2024-05-11 14:29:14.509702 qtharmony-0.2.1/qtharmony/windows/styles/main_window.css
--rw-r--r--   0        0        0     2792 1970-01-01 00:00:00.000000 qtharmony-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-05-02 17:11:53.147941 qtharmony-0.2.2/LICENSE
+-rw-r--r--   0        0        0     2050 2024-05-12 11:50:16.448380 qtharmony-0.2.2/README.md
+-rw-r--r--   0        0        0      609 2024-05-12 12:20:36.796776 qtharmony-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      327 2024-05-11 05:40:26.229552 qtharmony-0.2.2/qtharmony/__init__.py
+-rw-r--r--   0        0        0       38 2024-05-11 05:40:26.229552 qtharmony-0.2.2/qtharmony/constructor/__init__.py
+-rw-r--r--   0        0        0      636 2024-05-12 06:38:54.294789 qtharmony-0.2.2/qtharmony/constructor/initialize.py
+-rw-r--r--   0        0        0        2 2024-05-11 08:08:22.630008 qtharmony-0.2.2/qtharmony/resources/__init__.py
+-rw-r--r--   0        0        0     4295 2024-05-12 11:50:16.451713 qtharmony-0.2.2/qtharmony/resources/themes/dark-default.json
+-rw-r--r--   0        0        0     4580 2024-05-12 12:20:22.144106 qtharmony-0.2.2/qtharmony/resources/themes/dark-green.json
+-rw-r--r--   0        0        0     4563 2024-05-12 11:50:16.451713 qtharmony-0.2.2/qtharmony/resources/themes/light-default.json
+-rw-r--r--   0        0        0     4560 2024-05-12 12:20:22.144106 qtharmony-0.2.2/qtharmony/resources/themes/light-green.json
+-rw-r--r--   0        0        0    31042 2024-05-11 05:40:26.229552 qtharmony-0.2.2/qtharmony/resources/ui/Icon.png
+-rw-r--r--   0        0        0    17484 2024-05-11 05:40:26.229552 qtharmony-0.2.2/qtharmony/resources/ui/Logo.png
+-rw-r--r--   0        0        0     5387 2024-05-11 05:40:26.229552 qtharmony-0.2.2/qtharmony/resources/ui/angle-down.png
+-rw-r--r--   0        0        0       22 2024-05-11 08:08:22.630008 qtharmony-0.2.2/qtharmony/src/config/__init__.py
+-rw-r--r--   0        0        0      233 2024-05-11 14:21:59.267556 qtharmony-0.2.2/qtharmony/src/config/config.py
+-rw-r--r--   0        0        0      120 2024-05-11 05:40:26.229552 qtharmony-0.2.2/qtharmony/src/core/__init__.py
+-rw-r--r--   0        0        0      985 2024-05-11 05:40:26.232885 qtharmony-0.2.2/qtharmony/src/core/dialog.py
+-rw-r--r--   0        0        0      151 2024-05-11 05:40:26.232885 qtharmony-0.2.2/qtharmony/src/core/exceptions.py
+-rw-r--r--   0        0        0     2506 2024-05-11 05:40:26.232885 qtharmony-0.2.2/qtharmony/src/core/font.py
+-rw-r--r--   0        0        0      876 2024-05-11 17:33:26.077741 qtharmony-0.2.2/qtharmony/src/core/load.py
+-rw-r--r--   0        0        0      576 2024-05-12 11:50:16.451713 qtharmony-0.2.2/qtharmony/src/core/sizes.py
+-rw-r--r--   0        0        0     1235 2024-05-12 07:41:31.423989 qtharmony-0.2.2/qtharmony/src/core/stylesheet.py
+-rw-r--r--   0        0        0       80 2024-05-11 14:21:59.267556 qtharmony-0.2.2/qtharmony/src/core/theme/__init__.py
+-rw-r--r--   0        0        0     1299 2024-05-11 14:29:14.506368 qtharmony-0.2.2/qtharmony/src/core/theme/theme_builder.py
+-rw-r--r--   0        0        0     2096 2024-05-12 11:59:50.366337 qtharmony-0.2.2/qtharmony/src/core/theme/theme_manager.py
+-rw-r--r--   0        0        0      464 2024-05-12 11:50:16.451713 qtharmony-0.2.2/qtharmony/widgets/__init__.py
+-rw-r--r--   0        0        0     2316 2024-05-12 10:49:33.152065 qtharmony-0.2.2/qtharmony/widgets/basic/button.py
+-rw-r--r--   0        0        0     2642 2024-05-12 07:41:31.423989 qtharmony-0.2.2/qtharmony/widgets/basic/check_box.py
+-rw-r--r--   0        0        0     2492 2024-05-12 07:41:31.423989 qtharmony-0.2.2/qtharmony/widgets/basic/digital_entry.py
+-rw-r--r--   0        0        0     3472 2024-05-12 11:50:16.451713 qtharmony-0.2.2/qtharmony/widgets/basic/drop_down_menu.py
+-rw-r--r--   0        0        0     2489 2024-05-12 10:24:10.276814 qtharmony-0.2.2/qtharmony/widgets/basic/entry.py
+-rw-r--r--   0        0        0      815 2024-05-12 11:50:16.451713 qtharmony-0.2.2/qtharmony/widgets/basic/frame.py
+-rw-r--r--   0        0        0     2704 2024-05-12 11:50:16.451713 qtharmony-0.2.2/qtharmony/widgets/basic/groups.py
+-rw-r--r--   0        0        0     3190 2024-05-12 11:50:16.451713 qtharmony-0.2.2/qtharmony/widgets/basic/label.py
+-rw-r--r--   0        0        0     3784 2024-05-12 07:41:31.423989 qtharmony-0.2.2/qtharmony/widgets/basic/path_entry.py
+-rw-r--r--   0        0        0     1922 2024-05-12 07:41:31.423989 qtharmony-0.2.2/qtharmony/widgets/basic/radio_button.py
+-rw-r--r--   0        0        0     1994 2024-05-12 07:41:31.423989 qtharmony-0.2.2/qtharmony/widgets/basic/splitter.py
+-rw-r--r--   0        0        0       61 2024-05-12 07:41:31.423989 qtharmony-0.2.2/qtharmony/widgets/basic/styles/button.css
+-rw-r--r--   0        0        0      115 2024-05-12 06:38:54.304789 qtharmony-0.2.2/qtharmony/widgets/basic/styles/check_box.css
+-rw-r--r--   0        0        0       63 2024-05-12 06:38:54.304789 qtharmony-0.2.2/qtharmony/widgets/basic/styles/digital_entry.css
+-rw-r--r--   0        0        0      147 2024-05-12 11:50:16.451713 qtharmony-0.2.2/qtharmony/widgets/basic/styles/drop_down_menu.css
+-rw-r--r--   0        0        0      108 2024-05-12 11:50:16.451713 qtharmony-0.2.2/qtharmony/widgets/basic/styles/entry.css
+-rw-r--r--   0        0        0        0 2024-05-12 11:50:16.451713 qtharmony-0.2.2/qtharmony/widgets/basic/styles/frame.css
+-rw-r--r--   0        0        0       60 2024-05-12 06:38:54.308122 qtharmony-0.2.2/qtharmony/widgets/basic/styles/group_box.css
+-rw-r--r--   0        0        0       35 2024-05-11 06:45:00.352043 qtharmony-0.2.2/qtharmony/widgets/basic/styles/label.css
+-rw-r--r--   0        0        0        0 2024-05-12 06:38:54.308122 qtharmony-0.2.2/qtharmony/widgets/basic/styles/path_entry.css
+-rw-r--r--   0        0        0       67 2024-05-12 06:38:54.318122 qtharmony-0.2.2/qtharmony/widgets/basic/styles/radio_button.css
+-rw-r--r--   0        0        0        0 2024-05-12 07:41:31.423989 qtharmony-0.2.2/qtharmony/widgets/basic/styles/splitter.css
+-rw-r--r--   0        0        0      313 2024-05-11 05:40:26.236219 qtharmony-0.2.2/qtharmony/widgets/basic/styles/widgets_list.css
+-rw-r--r--   0        0        0     1578 2024-05-11 05:40:26.236219 qtharmony-0.2.2/qtharmony/widgets/basic/widgets_list.py
+-rw-r--r--   0        0        0       36 2024-05-11 05:40:26.236219 qtharmony-0.2.2/qtharmony/windows/__init__.py
+-rw-r--r--   0        0        0     2692 2024-05-12 07:41:31.423989 qtharmony-0.2.2/qtharmony/windows/main_window.py
+-rw-r--r--   0        0        0        0 2024-05-11 14:29:14.509702 qtharmony-0.2.2/qtharmony/windows/styles/main_window.css
+-rw-r--r--   0        0        0     2792 1970-01-01 00:00:00.000000 qtharmony-0.2.2/PKG-INFO
```

### Comparing `qtharmony-0.2.1/LICENSE` & `qtharmony-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `qtharmony-0.2.1/README.md` & `qtharmony-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `qtharmony-0.2.1/pyproject.toml` & `qtharmony-0.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "QtHarmony"
-version = "0.2.1"
+version = "0.2.2"
 description = "QtHarmony - is a Cutting-Edge GUI Library Built on PyQt6 QtHarmony is a intuitive graphical user interface (GUI) library designed to simplify the development of modern, visually stunning, and highly functional applications. Built on the robust foundation of PyQt6. Now QtHarmony is in development."
 authors = ["chebupelka8 <stpzamyatin@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.11,<3.13"
```

### Comparing `qtharmony-0.2.1/qtharmony/constructor/initialize.py` & `qtharmony-0.2.2/qtharmony/constructor/initialize.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.2.1/qtharmony/resources/themes/dark-default.json` & `qtharmony-0.2.2/qtharmony/resources/themes/dark-default.json`

 * *Files identical despite different names*

### Comparing `qtharmony-0.2.1/qtharmony/resources/themes/light-default.json` & `qtharmony-0.2.2/qtharmony/resources/themes/light-default.json`

 * *Files identical despite different names*

### Comparing `qtharmony-0.2.1/qtharmony/resources/ui/Icon.png` & `qtharmony-0.2.2/qtharmony/resources/ui/Icon.png`

 * *Files identical despite different names*

### Comparing `qtharmony-0.2.1/qtharmony/resources/ui/Logo.png` & `qtharmony-0.2.2/qtharmony/resources/ui/Logo.png`

 * *Files identical despite different names*

### Comparing `qtharmony-0.2.1/qtharmony/resources/ui/angle-down.png` & `qtharmony-0.2.2/qtharmony/resources/ui/angle-down.png`

 * *Files identical despite different names*

### Comparing `qtharmony-0.2.1/qtharmony/src/core/dialog.py` & `qtharmony-0.2.2/qtharmony/src/core/dialog.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.2.1/qtharmony/src/core/font.py` & `qtharmony-0.2.2/qtharmony/src/core/font.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.2.1/qtharmony/src/core/load.py` & `qtharmony-0.2.2/qtharmony/src/core/load.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.2.1/qtharmony/src/core/sizes.py` & `qtharmony-0.2.2/qtharmony/src/core/sizes.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.2.1/qtharmony/src/core/stylesheet.py` & `qtharmony-0.2.2/qtharmony/src/core/stylesheet.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.2.1/qtharmony/src/core/theme/theme_builder.py` & `qtharmony-0.2.2/qtharmony/src/core/theme/theme_builder.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.2.1/qtharmony/src/core/theme/theme_manager.py` & `qtharmony-0.2.2/qtharmony/src/core/theme/theme_manager.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.2.1/qtharmony/widgets/basic/button.py` & `qtharmony-0.2.2/qtharmony/widgets/basic/button.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.2.1/qtharmony/widgets/basic/check_box.py` & `qtharmony-0.2.2/qtharmony/widgets/basic/check_box.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.2.1/qtharmony/widgets/basic/digital_entry.py` & `qtharmony-0.2.2/qtharmony/widgets/basic/digital_entry.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.2.1/qtharmony/widgets/basic/drop_down_menu.py` & `qtharmony-0.2.2/qtharmony/widgets/basic/drop_down_menu.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.2.1/qtharmony/widgets/basic/entry.py` & `qtharmony-0.2.2/qtharmony/widgets/basic/entry.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.2.1/qtharmony/widgets/basic/frame.py` & `qtharmony-0.2.2/qtharmony/widgets/basic/frame.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.2.1/qtharmony/widgets/basic/groups.py` & `qtharmony-0.2.2/qtharmony/widgets/basic/groups.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.2.1/qtharmony/widgets/basic/label.py` & `qtharmony-0.2.2/qtharmony/widgets/basic/label.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.2.1/qtharmony/widgets/basic/path_entry.py` & `qtharmony-0.2.2/qtharmony/widgets/basic/path_entry.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.2.1/qtharmony/widgets/basic/radio_button.py` & `qtharmony-0.2.2/qtharmony/widgets/basic/radio_button.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.2.1/qtharmony/widgets/basic/splitter.py` & `qtharmony-0.2.2/qtharmony/widgets/basic/splitter.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.2.1/qtharmony/widgets/basic/widgets_list.py` & `qtharmony-0.2.2/qtharmony/widgets/basic/widgets_list.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.2.1/qtharmony/windows/main_window.py` & `qtharmony-0.2.2/qtharmony/windows/main_window.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.2.1/PKG-INFO` & `qtharmony-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QtHarmony
-Version: 0.2.1
+Version: 0.2.2
 Summary: QtHarmony - is a Cutting-Edge GUI Library Built on PyQt6 QtHarmony is a intuitive graphical user interface (GUI) library designed to simplify the development of modern, visually stunning, and highly functional applications. Built on the robust foundation of PyQt6. Now QtHarmony is in development.
 License: MIT
 Author: chebupelka8
 Author-email: stpzamyatin@gmail.com
 Requires-Python: >=3.11,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```
