# Comparing `tmp/qtharmony-0.1.7.tar.gz` & `tmp/qtharmony-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qtharmony-0.1.7.tar", max compression
+gzip compressed data, was "qtharmony-0.1.8.tar", max compression
```

## Comparing `qtharmony-0.1.7.tar` & `qtharmony-0.1.8.tar`

### file list

```diff
@@ -1,48 +1,49 @@
--rw-r--r--   0        0        0     1067 2024-05-02 17:11:53.147941 qtharmony-0.1.7/LICENSE
--rw-r--r--   0        0        0     1981 2024-05-11 08:16:36.349414 qtharmony-0.1.7/README.md
--rw-r--r--   0        0        0      609 2024-05-11 14:57:35.851311 qtharmony-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      327 2024-05-11 05:40:26.229552 qtharmony-0.1.7/qtharmony/__init__.py
--rw-r--r--   0        0        0       38 2024-05-11 05:40:26.229552 qtharmony-0.1.7/qtharmony/constructor/__init__.py
--rw-r--r--   0        0        0      636 2024-05-11 14:57:15.152216 qtharmony-0.1.7/qtharmony/constructor/initialize.py
--rw-r--r--   0        0        0        2 2024-05-11 08:08:22.630008 qtharmony-0.1.7/qtharmony/resources/__init__.py
--rw-r--r--   0        0        0     2883 2024-05-11 14:57:15.152216 qtharmony-0.1.7/qtharmony/resources/themes/dark-default.json
--rw-r--r--   0        0        0        0 2024-05-11 14:21:59.267556 qtharmony-0.1.7/qtharmony/resources/themes/light-default.json
--rw-r--r--   0        0        0    31042 2024-05-11 05:40:26.229552 qtharmony-0.1.7/qtharmony/resources/ui/Icon.png
--rw-r--r--   0        0        0    17484 2024-05-11 05:40:26.229552 qtharmony-0.1.7/qtharmony/resources/ui/Logo.png
--rw-r--r--   0        0        0     5387 2024-05-11 05:40:26.229552 qtharmony-0.1.7/qtharmony/resources/ui/angle-down.png
--rw-r--r--   0        0        0       22 2024-05-11 08:08:22.630008 qtharmony-0.1.7/qtharmony/src/config/__init__.py
--rw-r--r--   0        0        0      233 2024-05-11 14:21:59.267556 qtharmony-0.1.7/qtharmony/src/config/config.py
--rw-r--r--   0        0        0      120 2024-05-11 05:40:26.229552 qtharmony-0.1.7/qtharmony/src/core/__init__.py
--rw-r--r--   0        0        0      985 2024-05-11 05:40:26.232885 qtharmony-0.1.7/qtharmony/src/core/dialog.py
--rw-r--r--   0        0        0      151 2024-05-11 05:40:26.232885 qtharmony-0.1.7/qtharmony/src/core/exceptions.py
--rw-r--r--   0        0        0     2506 2024-05-11 05:40:26.232885 qtharmony-0.1.7/qtharmony/src/core/font.py
--rw-r--r--   0        0        0      876 2024-05-11 14:21:59.267556 qtharmony-0.1.7/qtharmony/src/core/load.py
--rw-r--r--   0        0        0      965 2024-05-11 13:53:23.349703 qtharmony-0.1.7/qtharmony/src/core/stylesheet.py
--rw-r--r--   0        0        0       80 2024-05-11 14:21:59.267556 qtharmony-0.1.7/qtharmony/src/core/theme/__init__.py
--rw-r--r--   0        0        0     1299 2024-05-11 14:29:14.506368 qtharmony-0.1.7/qtharmony/src/core/theme/theme_builder.py
--rw-r--r--   0        0        0     1914 2024-05-11 14:57:15.152216 qtharmony-0.1.7/qtharmony/src/core/theme/theme_manager.py
--rw-r--r--   0        0        0      433 2024-05-11 08:23:35.711704 qtharmony-0.1.7/qtharmony/widgets/__init__.py
--rw-r--r--   0        0        0     2318 2024-05-11 14:21:59.267556 qtharmony-0.1.7/qtharmony/widgets/basic/button.py
--rw-r--r--   0        0        0     2645 2024-05-11 14:57:15.152216 qtharmony-0.1.7/qtharmony/widgets/basic/check_box.py
--rw-r--r--   0        0        0     2495 2024-05-11 14:57:15.152216 qtharmony-0.1.7/qtharmony/widgets/basic/digital_entry.py
--rw-r--r--   0        0        0     3478 2024-05-11 14:29:14.506368 qtharmony-0.1.7/qtharmony/widgets/basic/drop_down_menu.py
--rw-r--r--   0        0        0     2492 2024-05-11 14:29:14.506368 qtharmony-0.1.7/qtharmony/widgets/basic/entry.py
--rw-r--r--   0        0        0     1518 2024-05-11 07:50:41.511507 qtharmony-0.1.7/qtharmony/widgets/basic/groups.py
--rw-r--r--   0        0        0     3329 2024-05-11 07:50:41.511507 qtharmony-0.1.7/qtharmony/widgets/basic/label.py
--rw-r--r--   0        0        0     3737 2024-05-11 07:50:41.511507 qtharmony-0.1.7/qtharmony/widgets/basic/path_entry.py
--rw-r--r--   0        0        0     1924 2024-05-11 14:57:15.152216 qtharmony-0.1.7/qtharmony/widgets/basic/radio_button.py
--rw-r--r--   0        0        0     1906 2024-05-11 07:50:41.511507 qtharmony-0.1.7/qtharmony/widgets/basic/splitter.py
--rw-r--r--   0        0        0       68 2024-05-11 14:29:14.506368 qtharmony-0.1.7/qtharmony/widgets/basic/styles/button.css
--rw-r--r--   0        0        0      115 2024-05-11 14:57:15.152216 qtharmony-0.1.7/qtharmony/widgets/basic/styles/check_box.css
--rw-r--r--   0        0        0       63 2024-05-11 14:57:15.152216 qtharmony-0.1.7/qtharmony/widgets/basic/styles/digital_entry.css
--rw-r--r--   0        0        0      139 2024-05-11 14:29:14.509702 qtharmony-0.1.7/qtharmony/widgets/basic/styles/drop_down_menu.css
--rw-r--r--   0        0        0       56 2024-05-11 14:29:14.509702 qtharmony-0.1.7/qtharmony/widgets/basic/styles/entry.css
--rw-r--r--   0        0        0      153 2024-05-11 06:45:00.352043 qtharmony-0.1.7/qtharmony/widgets/basic/styles/group_box.css
--rw-r--r--   0        0        0       35 2024-05-11 06:45:00.352043 qtharmony-0.1.7/qtharmony/widgets/basic/styles/label.css
--rw-r--r--   0        0        0       67 2024-05-11 14:57:15.152216 qtharmony-0.1.7/qtharmony/widgets/basic/styles/radio_button.css
--rw-r--r--   0        0        0      313 2024-05-11 05:40:26.236219 qtharmony-0.1.7/qtharmony/widgets/basic/styles/widgets_list.css
--rw-r--r--   0        0        0     1578 2024-05-11 05:40:26.236219 qtharmony-0.1.7/qtharmony/widgets/basic/widgets_list.py
--rw-r--r--   0        0        0       36 2024-05-11 05:40:26.236219 qtharmony-0.1.7/qtharmony/windows/__init__.py
--rw-r--r--   0        0        0     2694 2024-05-11 14:29:14.509702 qtharmony-0.1.7/qtharmony/windows/main_window.py
--rw-r--r--   0        0        0        0 2024-05-11 14:29:14.509702 qtharmony-0.1.7/qtharmony/windows/styles/main_window.css
--rw-r--r--   0        0        0     2723 1970-01-01 00:00:00.000000 qtharmony-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-05-02 17:11:53.147941 qtharmony-0.1.8/LICENSE
+-rw-r--r--   0        0        0     1981 2024-05-11 08:16:36.349414 qtharmony-0.1.8/README.md
+-rw-r--r--   0        0        0      609 2024-05-11 16:55:26.771146 qtharmony-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0      327 2024-05-11 05:40:26.229552 qtharmony-0.1.8/qtharmony/__init__.py
+-rw-r--r--   0        0        0       38 2024-05-11 05:40:26.229552 qtharmony-0.1.8/qtharmony/constructor/__init__.py
+-rw-r--r--   0        0        0      636 2024-05-11 14:57:15.152216 qtharmony-0.1.8/qtharmony/constructor/initialize.py
+-rw-r--r--   0        0        0        2 2024-05-11 08:08:22.630008 qtharmony-0.1.8/qtharmony/resources/__init__.py
+-rw-r--r--   0        0        0     3463 2024-05-11 16:54:57.602357 qtharmony-0.1.8/qtharmony/resources/themes/dark-default.json
+-rw-r--r--   0        0        0        0 2024-05-11 14:21:59.267556 qtharmony-0.1.8/qtharmony/resources/themes/light-default.json
+-rw-r--r--   0        0        0    31042 2024-05-11 05:40:26.229552 qtharmony-0.1.8/qtharmony/resources/ui/Icon.png
+-rw-r--r--   0        0        0    17484 2024-05-11 05:40:26.229552 qtharmony-0.1.8/qtharmony/resources/ui/Logo.png
+-rw-r--r--   0        0        0     5387 2024-05-11 05:40:26.229552 qtharmony-0.1.8/qtharmony/resources/ui/angle-down.png
+-rw-r--r--   0        0        0       22 2024-05-11 08:08:22.630008 qtharmony-0.1.8/qtharmony/src/config/__init__.py
+-rw-r--r--   0        0        0      233 2024-05-11 14:21:59.267556 qtharmony-0.1.8/qtharmony/src/config/config.py
+-rw-r--r--   0        0        0      120 2024-05-11 05:40:26.229552 qtharmony-0.1.8/qtharmony/src/core/__init__.py
+-rw-r--r--   0        0        0      985 2024-05-11 05:40:26.232885 qtharmony-0.1.8/qtharmony/src/core/dialog.py
+-rw-r--r--   0        0        0      151 2024-05-11 05:40:26.232885 qtharmony-0.1.8/qtharmony/src/core/exceptions.py
+-rw-r--r--   0        0        0     2506 2024-05-11 05:40:26.232885 qtharmony-0.1.8/qtharmony/src/core/font.py
+-rw-r--r--   0        0        0      876 2024-05-11 14:21:59.267556 qtharmony-0.1.8/qtharmony/src/core/load.py
+-rw-r--r--   0        0        0      965 2024-05-11 13:53:23.349703 qtharmony-0.1.8/qtharmony/src/core/stylesheet.py
+-rw-r--r--   0        0        0       80 2024-05-11 14:21:59.267556 qtharmony-0.1.8/qtharmony/src/core/theme/__init__.py
+-rw-r--r--   0        0        0     1299 2024-05-11 14:29:14.506368 qtharmony-0.1.8/qtharmony/src/core/theme/theme_builder.py
+-rw-r--r--   0        0        0     1914 2024-05-11 14:57:15.152216 qtharmony-0.1.8/qtharmony/src/core/theme/theme_manager.py
+-rw-r--r--   0        0        0      433 2024-05-11 08:23:35.711704 qtharmony-0.1.8/qtharmony/widgets/__init__.py
+-rw-r--r--   0        0        0     2318 2024-05-11 14:21:59.267556 qtharmony-0.1.8/qtharmony/widgets/basic/button.py
+-rw-r--r--   0        0        0     2645 2024-05-11 14:57:15.152216 qtharmony-0.1.8/qtharmony/widgets/basic/check_box.py
+-rw-r--r--   0        0        0     2495 2024-05-11 14:57:15.152216 qtharmony-0.1.8/qtharmony/widgets/basic/digital_entry.py
+-rw-r--r--   0        0        0     3478 2024-05-11 14:29:14.506368 qtharmony-0.1.8/qtharmony/widgets/basic/drop_down_menu.py
+-rw-r--r--   0        0        0     2492 2024-05-11 14:29:14.506368 qtharmony-0.1.8/qtharmony/widgets/basic/entry.py
+-rw-r--r--   0        0        0     1665 2024-05-11 16:43:43.496785 qtharmony-0.1.8/qtharmony/widgets/basic/groups.py
+-rw-r--r--   0        0        0     3329 2024-05-11 07:50:41.511507 qtharmony-0.1.8/qtharmony/widgets/basic/label.py
+-rw-r--r--   0        0        0     3873 2024-05-11 15:31:31.325171 qtharmony-0.1.8/qtharmony/widgets/basic/path_entry.py
+-rw-r--r--   0        0        0     1924 2024-05-11 14:57:15.152216 qtharmony-0.1.8/qtharmony/widgets/basic/radio_button.py
+-rw-r--r--   0        0        0     1906 2024-05-11 07:50:41.511507 qtharmony-0.1.8/qtharmony/widgets/basic/splitter.py
+-rw-r--r--   0        0        0       68 2024-05-11 14:29:14.506368 qtharmony-0.1.8/qtharmony/widgets/basic/styles/button.css
+-rw-r--r--   0        0        0      115 2024-05-11 14:57:15.152216 qtharmony-0.1.8/qtharmony/widgets/basic/styles/check_box.css
+-rw-r--r--   0        0        0       63 2024-05-11 14:57:15.152216 qtharmony-0.1.8/qtharmony/widgets/basic/styles/digital_entry.css
+-rw-r--r--   0        0        0      139 2024-05-11 14:29:14.509702 qtharmony-0.1.8/qtharmony/widgets/basic/styles/drop_down_menu.css
+-rw-r--r--   0        0        0       56 2024-05-11 14:29:14.509702 qtharmony-0.1.8/qtharmony/widgets/basic/styles/entry.css
+-rw-r--r--   0        0        0       60 2024-05-11 16:31:40.096075 qtharmony-0.1.8/qtharmony/widgets/basic/styles/group_box.css
+-rw-r--r--   0        0        0       35 2024-05-11 06:45:00.352043 qtharmony-0.1.8/qtharmony/widgets/basic/styles/label.css
+-rw-r--r--   0        0        0        0 2024-05-11 15:28:16.799734 qtharmony-0.1.8/qtharmony/widgets/basic/styles/path_entry.css
+-rw-r--r--   0        0        0       67 2024-05-11 14:57:15.152216 qtharmony-0.1.8/qtharmony/widgets/basic/styles/radio_button.css
+-rw-r--r--   0        0        0      313 2024-05-11 05:40:26.236219 qtharmony-0.1.8/qtharmony/widgets/basic/styles/widgets_list.css
+-rw-r--r--   0        0        0     1578 2024-05-11 05:40:26.236219 qtharmony-0.1.8/qtharmony/widgets/basic/widgets_list.py
+-rw-r--r--   0        0        0       36 2024-05-11 05:40:26.236219 qtharmony-0.1.8/qtharmony/windows/__init__.py
+-rw-r--r--   0        0        0     2694 2024-05-11 14:29:14.509702 qtharmony-0.1.8/qtharmony/windows/main_window.py
+-rw-r--r--   0        0        0        0 2024-05-11 14:29:14.509702 qtharmony-0.1.8/qtharmony/windows/styles/main_window.css
+-rw-r--r--   0        0        0     2723 1970-01-01 00:00:00.000000 qtharmony-0.1.8/PKG-INFO
```

### Comparing `qtharmony-0.1.7/LICENSE` & `qtharmony-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `qtharmony-0.1.7/README.md` & `qtharmony-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `qtharmony-0.1.7/pyproject.toml` & `qtharmony-0.1.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "QtHarmony"
-version = "0.1.7"
+version = "0.1.8"
 description = "QtHarmony - is a Cutting-Edge GUI Library Built on PyQt6 QtHarmony is a intuitive graphical user interface (GUI) library designed to simplify the development of modern, visually stunning, and highly functional applications. Built on the robust foundation of PyQt6. Now QtHarmony is in development."
 authors = ["chebupelka8 <stpzamyatin@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.11,<3.13"
```

### Comparing `qtharmony-0.1.7/qtharmony/constructor/initialize.py` & `qtharmony-0.1.8/qtharmony/constructor/initialize.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.1.7/qtharmony/resources/themes/dark-default.json` & `qtharmony-0.1.8/qtharmony/resources/themes/dark-default.json`

 * *Files 13% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6575%*

 * *Differences: {"'CheckBox'": "{'': OrderedDict([('color', '#ffffff')]), delete: [':active']}",*

 * * "'DigitalEntry'": "{'': OrderedDict([('color', '#1A3B5D'), ('background-color', '#ffffff'), "*

 * *                   "('border', '1px solid #adb5bd'), ('border-radius', '6px')]), delete: "*

 * *                   "[':active']}",*

 * * "'DropDownMenu'": "{'': OrderedDict([('background-color', '#ffffff'), ('color', '#1A3B5D'), "*

 * *                   "('border', '1px solid #adb5bd'), ('border-radius', '6px')]), delete: "*

 * *                   "[':a […]*

```diff
@@ -1,111 +1,133 @@
 {
     "CheckBox": {
+        "": {
+            "color": "#ffffff"
+        },
         "::indicator": {
             "border": "1px solid #0166fc",
             "border-radius": "3px"
         },
         "::indicator:checked:disabled": {
             "background-color": "lightgray"
         },
         "::indicator:checked:enabled": {
             "background-color": "#0166fc"
         },
         "::indicator:disabled": {
             "border-color": "gray"
         },
-        ":active": {
-            "color": "#ffffff"
-        },
         ":disabled": {
             "color": "gray"
         },
         "object-name": "QCheckBox#check-box"
     },
     "DigitalEntry": {
-        ":active": {
+        "": {
             "background-color": "#ffffff",
             "border": "1px solid #adb5bd",
             "border-radius": "6px",
             "color": "#1A3B5D"
         },
         ":focus": {
             "border-color": "#405cf5"
         },
         ":hover": {
             "border-color": "#6185DF"
         },
         "object-name": "QSpinBox#digital-entry"
     },
     "DropDownMenu": {
+        "": {
+            "background-color": "#ffffff",
+            "border": "1px solid #adb5bd",
+            "border-radius": "6px",
+            "color": "#1A3B5D"
+        },
         " QAbstractItemView": {
             "background-color": "#ffffff"
         },
         "::drop-down": {
             "border": "none"
         },
-        ":active": {
-            "background-color": "#ffffff",
-            "border": "1px solid #adb5bd",
-            "border-radius": "6px",
-            "color": "#1A3B5D"
-        },
         ":hover": {
             "border-color": "#6185DF"
         },
         "object-name": "QComboBox#drop-down-menu"
     },
     "Entry": {
-        ":active": {
+        "": {
             "background-color": "#ffffff",
             "border": "1px solid #adb5bd",
             "border-radius": "6px",
             "color": "#1A3B5D"
         },
         ":focus": {
             "border-color": "#405cf5"
         },
         ":hover": {
             "border-color": "#6185DF"
         },
         "object-name": "QLineEdit#entry"
     },
+    "GroupBox": {
+        "": {
+            "background-color": "#323232",
+            "border": "none",
+            "border-radius": "6px"
+        },
+        "::title": {
+            "background-color": "#404040",
+            "border-radius": "6px",
+            "color": "#ffffff",
+            "margin-top": "5px",
+            "min-height": "30px",
+            "padding-left": "20px",
+            "padding-right": "20px",
+            "subcontrol-position": "top"
+        },
+        "object-name": "QGroupBox#group-box"
+    },
     "Info": {
         "author": null,
         "name": "Dark-Default"
     },
     "MainWindow": {
-        ":active": {
+        "": {
             "background-color": "#252525",
             "border": "none",
             "border-radius": "0px"
         },
         "object-name": "QMainWindow#main-window"
     },
+    "PathEntry": {
+        "": {},
+        "object-name": "QWidget#path-entry"
+    },
     "PushButton": {
-        ":active": {
+        "": {
             "background-color": "#405cf5",
             "border": "none",
             "border-radius": "6px"
         },
         ":hover": {
             "background-color": "#3045B8"
         },
         ":pressed": {
             "background-color": "#283A9A"
         },
         "object-name": "QPushButton#button"
     },
     "RadioButton": {
+        "": {
+            "color": "#ffffff"
+        },
         "::indicator": {
             "border": "1px solid #0166fc",
             "border-radius": "7px"
         },
         "::indicator:checked": {
             "background-color": "#0166fc"
         },
-        ":active": {
-            "color": "#ffffff"
-        },
         "object-name": "QRadioButton#radio-button"
     }
 }
```

### Comparing `qtharmony-0.1.7/qtharmony/resources/ui/Icon.png` & `qtharmony-0.1.8/qtharmony/resources/ui/Icon.png`

 * *Files identical despite different names*

### Comparing `qtharmony-0.1.7/qtharmony/resources/ui/Logo.png` & `qtharmony-0.1.8/qtharmony/resources/ui/Logo.png`

 * *Files identical despite different names*

### Comparing `qtharmony-0.1.7/qtharmony/resources/ui/angle-down.png` & `qtharmony-0.1.8/qtharmony/resources/ui/angle-down.png`

 * *Files identical despite different names*

### Comparing `qtharmony-0.1.7/qtharmony/src/core/dialog.py` & `qtharmony-0.1.8/qtharmony/src/core/dialog.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.1.7/qtharmony/src/core/font.py` & `qtharmony-0.1.8/qtharmony/src/core/font.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.1.7/qtharmony/src/core/load.py` & `qtharmony-0.1.8/qtharmony/src/core/load.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.1.7/qtharmony/src/core/stylesheet.py` & `qtharmony-0.1.8/qtharmony/src/core/stylesheet.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.1.7/qtharmony/src/core/theme/theme_builder.py` & `qtharmony-0.1.8/qtharmony/src/core/theme/theme_builder.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.1.7/qtharmony/src/core/theme/theme_manager.py` & `qtharmony-0.1.8/qtharmony/src/core/theme/theme_manager.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.1.7/qtharmony/widgets/basic/button.py` & `qtharmony-0.1.8/qtharmony/widgets/basic/button.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.1.7/qtharmony/widgets/basic/check_box.py` & `qtharmony-0.1.8/qtharmony/widgets/basic/check_box.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.1.7/qtharmony/widgets/basic/digital_entry.py` & `qtharmony-0.1.8/qtharmony/widgets/basic/digital_entry.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.1.7/qtharmony/widgets/basic/drop_down_menu.py` & `qtharmony-0.1.8/qtharmony/widgets/basic/drop_down_menu.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.1.7/qtharmony/widgets/basic/entry.py` & `qtharmony-0.1.8/qtharmony/widgets/basic/entry.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.1.7/qtharmony/widgets/basic/groups.py` & `qtharmony-0.1.8/qtharmony/widgets/basic/radio_button.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,49 +1,51 @@
-from typing import Optional, TYPE_CHECKING
-
-from PySide6.QtWidgets import (
-    QGroupBox, QButtonGroup
-)
+from PySide6.QtWidgets import QRadioButton
+from PySide6.QtCore import QSize
 
-from qtharmony.src.core import Loader, StyleSheetLoader
-
-import os.path
+from qtharmony.src.core import StyleSheetLoader
+from qtharmony.src.core.theme import ThemeManager
 
+from typing import Optional, TYPE_CHECKING
 if TYPE_CHECKING:
     from PySide6.QtWidgets import QWidget
 
 
-class GroupBox(QGroupBox):
+class RadioButton(QRadioButton):
     """
-    Custom QGroupBox widget for grouping widgets.
+    Custom QRadioButton widget for radio button functionality.
 
     Methods:
-    - __init__(title: Optional[str] = None, *, stylesheet: Optional[str] = None, parent: Optional["QWidget"] = None): None
-              - Initializes the GroupBox widget with optional title and stylesheet.
+    - __init__(text: Optional[str] = None, size: tuple[int, int] = (200, 30),
+              *, stylesheet: Optional[str] = None, parent: Optional["QWidget"] = None): None
+              - Initializes the RadioButton widget with optional text, size, and stylesheet.
     """
 
     def __init__(
             self,
-            title: Optional[str] = None,
+            text: Optional[str] = None,
+            size: tuple[int, int] = (200, 30),
             *,
             stylesheet: Optional[str] = None,
             parent: Optional["QWidget"] = None
     ) -> None:
         """
-        Initializes the GroupBox widget with optional title and stylesheet.
+        Initializes the RadioButton widget with optional text, size, and stylesheet.
 
         Args:
-            title (Optional[str], optional): The title of the group box. Defaults to None.
-            stylesheet (Optional[str], optional): Custom stylesheet for the group box widget. Defaults to None.
-            parent (Optional["QWidget"], optional): Parent widget of the group box. Defaults to None.
-        """
+            text (Optional[str], optional): The text displayed next to the radio button. Defaults to None.
+            size (tuple[int, int], optional): The size of the radio button widget (width, height). Defaults to (200, 30).
+            stylesheet (Optional[str], optional): Custom stylesheet for the radio button widget. Defaults to None.
+            parent (Optional["QWidget"], optional): Parent widget of the radio button. Defaults to None.
+        """ 
 
         super().__init__(parent)
+        ThemeManager.add_widgets(self)
+
+        if text is not None: self.setText(text)
+        self.setFixedSize(QSize(*size))
 
-        self.setObjectName("group-box")
+        self.setObjectName("radio-button")
         self.setStyleSheet(StyleSheetLoader.load_stylesheet(
-            __file__, "styles/group_box.css", 
-            name="GroupBox", obj_name="QGroupBox#group-box",
+            __file__, "styles/radio_button.css", 
+            name="RadioButton", obj_name="QRadioButton#radio-button",
             stylesheet=stylesheet
         ))
-
-        if title is not None: self.setTitle(title)
```

### Comparing `qtharmony-0.1.7/qtharmony/widgets/basic/label.py` & `qtharmony-0.1.8/qtharmony/widgets/basic/label.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.1.7/qtharmony/widgets/basic/path_entry.py` & `qtharmony-0.1.8/qtharmony/widgets/basic/path_entry.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from PySide6.QtWidgets import ( 
     QWidget, QHBoxLayout, 
     QSpacerItem, QSizePolicy
 )
 
 from qtharmony.src.core import FileDialog, StyleSheetLoader
+from qtharmony.src.core.theme import ThemeManager
 
 from .button import PushButton
 from .entry import Entry
 
 from typing import Optional, TYPE_CHECKING
 if TYPE_CHECKING:
     from PySide6.QtGui import QFont
@@ -48,29 +49,32 @@
             size (tuple[int, int], optional): The size of the path entry widget (width, height). Defaults to (200, 30).
             font (Optional["QFont"], optional): The font to be used for text input. Defaults to None.
             stylesheet (Optional[str], optional): Custom stylesheet for the path entry widget. Defaults to None.
             parent (Optional["QWidget"], optional): Parent widget of the path entry. Defaults to None.
         """        
 
         super().__init__(parent)
+        ThemeManager.add_widgets(self)
 
         self.setObjectName("path-entry")
         if font is not None: self.setFont(font)
 
         self.setStyleSheet(StyleSheetLoader.load_stylesheet(
             __file__, "styles/path_entry.css", 
-            name="PathEntry", obj_name="QLineEdit#path-entry",
+            name="PathEntry", obj_name="QWidget#path-entry",
             stylesheet=stylesheet
         ))
 
+        print(self.styleSheet())
+
         self.mainLayout = QHBoxLayout()
 
         self.pathEntry = Entry(placed, placeholder, size)
 
-        self.specifyPathBtn = PushButton("...")
+        self.specifyPathBtn = PushButton("...", size=(28, 28))
         self.specifyPathBtn.clicked.connect(lambda: self.set_path(FileDialog.get_open_file_name()))
 
         self.mainLayout.addWidget(self.pathEntry)
         self.mainLayout.addWidget(self.specifyPathBtn)
         self.mainLayout.addItem(QSpacerItem(20, 20, QSizePolicy.Policy.Expanding, QSizePolicy.Policy.Minimum))
         self.setLayout(self.mainLayout)
```

### Comparing `qtharmony-0.1.7/qtharmony/widgets/basic/radio_button.py` & `qtharmony-0.1.8/qtharmony/widgets/basic/groups.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,51 +1,51 @@
-from PySide6.QtWidgets import QRadioButton
-from PySide6.QtCore import QSize
+from typing import Optional, TYPE_CHECKING
+
+from PySide6.QtWidgets import (
+    QGroupBox, QButtonGroup
+)
 
 from qtharmony.src.core import StyleSheetLoader
-from qtharmony.src.core.theme import ThemeManager
+from qtharmony.src.core.theme import ThemeManager 
 
-from typing import Optional, TYPE_CHECKING
 if TYPE_CHECKING:
     from PySide6.QtWidgets import QWidget
 
 
-class RadioButton(QRadioButton):
+class GroupBox(QGroupBox):
     """
-    Custom QRadioButton widget for radio button functionality.
+    Custom QGroupBox widget for grouping widgets.
 
     Methods:
-    - __init__(text: Optional[str] = None, size: tuple[int, int] = (200, 30),
-              *, stylesheet: Optional[str] = None, parent: Optional["QWidget"] = None): None
-              - Initializes the RadioButton widget with optional text, size, and stylesheet.
+    - __init__(title: Optional[str] = None, *, stylesheet: Optional[str] = None, parent: Optional["QWidget"] = None): None
+              - Initializes the GroupBox widget with optional title and stylesheet.
     """
 
     def __init__(
             self,
-            text: Optional[str] = None,
-            size: tuple[int, int] = (200, 30),
+            title: Optional[str] = None,
+            size: tuple[int, int] = (400, 200),
             *,
             stylesheet: Optional[str] = None,
             parent: Optional["QWidget"] = None
     ) -> None:
         """
-        Initializes the RadioButton widget with optional text, size, and stylesheet.
+        Initializes the GroupBox widget with optional title and stylesheet.
 
         Args:
-            text (Optional[str], optional): The text displayed next to the radio button. Defaults to None.
-            size (tuple[int, int], optional): The size of the radio button widget (width, height). Defaults to (200, 30).
-            stylesheet (Optional[str], optional): Custom stylesheet for the radio button widget. Defaults to None.
-            parent (Optional["QWidget"], optional): Parent widget of the radio button. Defaults to None.
-        """ 
+            title (Optional[str], optional): The title of the group box. Defaults to None.
+            stylesheet (Optional[str], optional): Custom stylesheet for the group box widget. Defaults to None.
+            parent (Optional["QWidget"], optional): Parent widget of the group box. Defaults to None.
+        """
 
         super().__init__(parent)
         ThemeManager.add_widgets(self)
 
-        if text is not None: self.setText(text)
-        self.setFixedSize(QSize(*size))
-
-        self.setObjectName("radio-button")
+        self.setObjectName("group-box")
         self.setStyleSheet(StyleSheetLoader.load_stylesheet(
-            __file__, "styles/radio_button.css", 
-            name="RadioButton", obj_name="QRadioButton#radio-button",
+            __file__, "styles/group_box.css", 
+            name="GroupBox", obj_name="QGroupBox#group-box",
             stylesheet=stylesheet
         ))
+
+        if title is not None: self.setTitle(title)
+        self.setFixedSize(*size)
```

### Comparing `qtharmony-0.1.7/qtharmony/widgets/basic/splitter.py` & `qtharmony-0.1.8/qtharmony/widgets/basic/splitter.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.1.7/qtharmony/widgets/basic/widgets_list.py` & `qtharmony-0.1.8/qtharmony/widgets/basic/widgets_list.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.1.7/qtharmony/windows/main_window.py` & `qtharmony-0.1.8/qtharmony/windows/main_window.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.1.7/PKG-INFO` & `qtharmony-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QtHarmony
-Version: 0.1.7
+Version: 0.1.8
 Summary: QtHarmony - is a Cutting-Edge GUI Library Built on PyQt6 QtHarmony is a intuitive graphical user interface (GUI) library designed to simplify the development of modern, visually stunning, and highly functional applications. Built on the robust foundation of PyQt6. Now QtHarmony is in development.
 License: MIT
 Author: chebupelka8
 Author-email: stpzamyatin@gmail.com
 Requires-Python: >=3.11,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

