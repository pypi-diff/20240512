# Comparing `tmp/qtharmony-0.1.8.tar.gz` & `tmp/qtharmony-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qtharmony-0.1.8.tar", max compression
+gzip compressed data, was "qtharmony-0.1.9.tar", max compression
```

## Comparing `qtharmony-0.1.8.tar` & `qtharmony-0.1.9.tar`

### file list

```diff
@@ -1,49 +1,50 @@
--rw-r--r--   0        0        0     1067 2024-05-02 17:11:53.147941 qtharmony-0.1.8/LICENSE
--rw-r--r--   0        0        0     1981 2024-05-11 08:16:36.349414 qtharmony-0.1.8/README.md
--rw-r--r--   0        0        0      609 2024-05-11 16:55:26.771146 qtharmony-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      327 2024-05-11 05:40:26.229552 qtharmony-0.1.8/qtharmony/__init__.py
--rw-r--r--   0        0        0       38 2024-05-11 05:40:26.229552 qtharmony-0.1.8/qtharmony/constructor/__init__.py
--rw-r--r--   0        0        0      636 2024-05-11 14:57:15.152216 qtharmony-0.1.8/qtharmony/constructor/initialize.py
--rw-r--r--   0        0        0        2 2024-05-11 08:08:22.630008 qtharmony-0.1.8/qtharmony/resources/__init__.py
--rw-r--r--   0        0        0     3463 2024-05-11 16:54:57.602357 qtharmony-0.1.8/qtharmony/resources/themes/dark-default.json
--rw-r--r--   0        0        0        0 2024-05-11 14:21:59.267556 qtharmony-0.1.8/qtharmony/resources/themes/light-default.json
--rw-r--r--   0        0        0    31042 2024-05-11 05:40:26.229552 qtharmony-0.1.8/qtharmony/resources/ui/Icon.png
--rw-r--r--   0        0        0    17484 2024-05-11 05:40:26.229552 qtharmony-0.1.8/qtharmony/resources/ui/Logo.png
--rw-r--r--   0        0        0     5387 2024-05-11 05:40:26.229552 qtharmony-0.1.8/qtharmony/resources/ui/angle-down.png
--rw-r--r--   0        0        0       22 2024-05-11 08:08:22.630008 qtharmony-0.1.8/qtharmony/src/config/__init__.py
--rw-r--r--   0        0        0      233 2024-05-11 14:21:59.267556 qtharmony-0.1.8/qtharmony/src/config/config.py
--rw-r--r--   0        0        0      120 2024-05-11 05:40:26.229552 qtharmony-0.1.8/qtharmony/src/core/__init__.py
--rw-r--r--   0        0        0      985 2024-05-11 05:40:26.232885 qtharmony-0.1.8/qtharmony/src/core/dialog.py
--rw-r--r--   0        0        0      151 2024-05-11 05:40:26.232885 qtharmony-0.1.8/qtharmony/src/core/exceptions.py
--rw-r--r--   0        0        0     2506 2024-05-11 05:40:26.232885 qtharmony-0.1.8/qtharmony/src/core/font.py
--rw-r--r--   0        0        0      876 2024-05-11 14:21:59.267556 qtharmony-0.1.8/qtharmony/src/core/load.py
--rw-r--r--   0        0        0      965 2024-05-11 13:53:23.349703 qtharmony-0.1.8/qtharmony/src/core/stylesheet.py
--rw-r--r--   0        0        0       80 2024-05-11 14:21:59.267556 qtharmony-0.1.8/qtharmony/src/core/theme/__init__.py
--rw-r--r--   0        0        0     1299 2024-05-11 14:29:14.506368 qtharmony-0.1.8/qtharmony/src/core/theme/theme_builder.py
--rw-r--r--   0        0        0     1914 2024-05-11 14:57:15.152216 qtharmony-0.1.8/qtharmony/src/core/theme/theme_manager.py
--rw-r--r--   0        0        0      433 2024-05-11 08:23:35.711704 qtharmony-0.1.8/qtharmony/widgets/__init__.py
--rw-r--r--   0        0        0     2318 2024-05-11 14:21:59.267556 qtharmony-0.1.8/qtharmony/widgets/basic/button.py
--rw-r--r--   0        0        0     2645 2024-05-11 14:57:15.152216 qtharmony-0.1.8/qtharmony/widgets/basic/check_box.py
--rw-r--r--   0        0        0     2495 2024-05-11 14:57:15.152216 qtharmony-0.1.8/qtharmony/widgets/basic/digital_entry.py
--rw-r--r--   0        0        0     3478 2024-05-11 14:29:14.506368 qtharmony-0.1.8/qtharmony/widgets/basic/drop_down_menu.py
--rw-r--r--   0        0        0     2492 2024-05-11 14:29:14.506368 qtharmony-0.1.8/qtharmony/widgets/basic/entry.py
--rw-r--r--   0        0        0     1665 2024-05-11 16:43:43.496785 qtharmony-0.1.8/qtharmony/widgets/basic/groups.py
--rw-r--r--   0        0        0     3329 2024-05-11 07:50:41.511507 qtharmony-0.1.8/qtharmony/widgets/basic/label.py
--rw-r--r--   0        0        0     3873 2024-05-11 15:31:31.325171 qtharmony-0.1.8/qtharmony/widgets/basic/path_entry.py
--rw-r--r--   0        0        0     1924 2024-05-11 14:57:15.152216 qtharmony-0.1.8/qtharmony/widgets/basic/radio_button.py
--rw-r--r--   0        0        0     1906 2024-05-11 07:50:41.511507 qtharmony-0.1.8/qtharmony/widgets/basic/splitter.py
--rw-r--r--   0        0        0       68 2024-05-11 14:29:14.506368 qtharmony-0.1.8/qtharmony/widgets/basic/styles/button.css
--rw-r--r--   0        0        0      115 2024-05-11 14:57:15.152216 qtharmony-0.1.8/qtharmony/widgets/basic/styles/check_box.css
--rw-r--r--   0        0        0       63 2024-05-11 14:57:15.152216 qtharmony-0.1.8/qtharmony/widgets/basic/styles/digital_entry.css
--rw-r--r--   0        0        0      139 2024-05-11 14:29:14.509702 qtharmony-0.1.8/qtharmony/widgets/basic/styles/drop_down_menu.css
--rw-r--r--   0        0        0       56 2024-05-11 14:29:14.509702 qtharmony-0.1.8/qtharmony/widgets/basic/styles/entry.css
--rw-r--r--   0        0        0       60 2024-05-11 16:31:40.096075 qtharmony-0.1.8/qtharmony/widgets/basic/styles/group_box.css
--rw-r--r--   0        0        0       35 2024-05-11 06:45:00.352043 qtharmony-0.1.8/qtharmony/widgets/basic/styles/label.css
--rw-r--r--   0        0        0        0 2024-05-11 15:28:16.799734 qtharmony-0.1.8/qtharmony/widgets/basic/styles/path_entry.css
--rw-r--r--   0        0        0       67 2024-05-11 14:57:15.152216 qtharmony-0.1.8/qtharmony/widgets/basic/styles/radio_button.css
--rw-r--r--   0        0        0      313 2024-05-11 05:40:26.236219 qtharmony-0.1.8/qtharmony/widgets/basic/styles/widgets_list.css
--rw-r--r--   0        0        0     1578 2024-05-11 05:40:26.236219 qtharmony-0.1.8/qtharmony/widgets/basic/widgets_list.py
--rw-r--r--   0        0        0       36 2024-05-11 05:40:26.236219 qtharmony-0.1.8/qtharmony/windows/__init__.py
--rw-r--r--   0        0        0     2694 2024-05-11 14:29:14.509702 qtharmony-0.1.8/qtharmony/windows/main_window.py
--rw-r--r--   0        0        0        0 2024-05-11 14:29:14.509702 qtharmony-0.1.8/qtharmony/windows/styles/main_window.css
--rw-r--r--   0        0        0     2723 1970-01-01 00:00:00.000000 qtharmony-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-05-02 17:11:53.147941 qtharmony-0.1.9/LICENSE
+-rw-r--r--   0        0        0     1981 2024-05-11 08:16:36.349414 qtharmony-0.1.9/README.md
+-rw-r--r--   0        0        0      609 2024-05-12 07:15:40.663236 qtharmony-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      327 2024-05-11 05:40:26.229552 qtharmony-0.1.9/qtharmony/__init__.py
+-rw-r--r--   0        0        0       38 2024-05-11 05:40:26.229552 qtharmony-0.1.9/qtharmony/constructor/__init__.py
+-rw-r--r--   0        0        0      636 2024-05-12 06:38:54.294789 qtharmony-0.1.9/qtharmony/constructor/initialize.py
+-rw-r--r--   0        0        0        2 2024-05-11 08:08:22.630008 qtharmony-0.1.9/qtharmony/resources/__init__.py
+-rw-r--r--   0        0        0     3435 2024-05-12 07:15:27.110567 qtharmony-0.1.9/qtharmony/resources/themes/dark-default.json
+-rw-r--r--   0        0        0      684 2024-05-12 07:15:27.110567 qtharmony-0.1.9/qtharmony/resources/themes/light-default.json
+-rw-r--r--   0        0        0    31042 2024-05-11 05:40:26.229552 qtharmony-0.1.9/qtharmony/resources/ui/Icon.png
+-rw-r--r--   0        0        0    17484 2024-05-11 05:40:26.229552 qtharmony-0.1.9/qtharmony/resources/ui/Logo.png
+-rw-r--r--   0        0        0     5387 2024-05-11 05:40:26.229552 qtharmony-0.1.9/qtharmony/resources/ui/angle-down.png
+-rw-r--r--   0        0        0       22 2024-05-11 08:08:22.630008 qtharmony-0.1.9/qtharmony/src/config/__init__.py
+-rw-r--r--   0        0        0      233 2024-05-11 14:21:59.267556 qtharmony-0.1.9/qtharmony/src/config/config.py
+-rw-r--r--   0        0        0      120 2024-05-11 05:40:26.229552 qtharmony-0.1.9/qtharmony/src/core/__init__.py
+-rw-r--r--   0        0        0      985 2024-05-11 05:40:26.232885 qtharmony-0.1.9/qtharmony/src/core/dialog.py
+-rw-r--r--   0        0        0      151 2024-05-11 05:40:26.232885 qtharmony-0.1.9/qtharmony/src/core/exceptions.py
+-rw-r--r--   0        0        0     2506 2024-05-11 05:40:26.232885 qtharmony-0.1.9/qtharmony/src/core/font.py
+-rw-r--r--   0        0        0      876 2024-05-11 17:33:26.077741 qtharmony-0.1.9/qtharmony/src/core/load.py
+-rw-r--r--   0        0        0     1235 2024-05-12 07:15:27.110567 qtharmony-0.1.9/qtharmony/src/core/stylesheet.py
+-rw-r--r--   0        0        0       80 2024-05-11 14:21:59.267556 qtharmony-0.1.9/qtharmony/src/core/theme/__init__.py
+-rw-r--r--   0        0        0     1299 2024-05-11 14:29:14.506368 qtharmony-0.1.9/qtharmony/src/core/theme/theme_builder.py
+-rw-r--r--   0        0        0     1903 2024-05-12 07:15:27.110567 qtharmony-0.1.9/qtharmony/src/core/theme/theme_manager.py
+-rw-r--r--   0        0        0      433 2024-05-11 08:23:35.711704 qtharmony-0.1.9/qtharmony/widgets/__init__.py
+-rw-r--r--   0        0        0     2316 2024-05-12 07:15:27.110567 qtharmony-0.1.9/qtharmony/widgets/basic/button.py
+-rw-r--r--   0        0        0     2642 2024-05-12 07:15:27.110567 qtharmony-0.1.9/qtharmony/widgets/basic/check_box.py
+-rw-r--r--   0        0        0     2492 2024-05-12 07:15:27.110567 qtharmony-0.1.9/qtharmony/widgets/basic/digital_entry.py
+-rw-r--r--   0        0        0     3476 2024-05-12 07:15:27.110567 qtharmony-0.1.9/qtharmony/widgets/basic/drop_down_menu.py
+-rw-r--r--   0        0        0     2489 2024-05-12 07:15:27.113900 qtharmony-0.1.9/qtharmony/widgets/basic/entry.py
+-rw-r--r--   0        0        0     1663 2024-05-12 07:15:27.113900 qtharmony-0.1.9/qtharmony/widgets/basic/groups.py
+-rw-r--r--   0        0        0     3195 2024-05-12 07:15:27.113900 qtharmony-0.1.9/qtharmony/widgets/basic/label.py
+-rw-r--r--   0        0        0     3784 2024-05-12 07:15:27.113900 qtharmony-0.1.9/qtharmony/widgets/basic/path_entry.py
+-rw-r--r--   0        0        0     1922 2024-05-12 07:15:27.113900 qtharmony-0.1.9/qtharmony/widgets/basic/radio_button.py
+-rw-r--r--   0        0        0     1994 2024-05-12 07:15:27.113900 qtharmony-0.1.9/qtharmony/widgets/basic/splitter.py
+-rw-r--r--   0        0        0       61 2024-05-12 07:15:27.113900 qtharmony-0.1.9/qtharmony/widgets/basic/styles/button.css
+-rw-r--r--   0        0        0      115 2024-05-12 06:38:54.304789 qtharmony-0.1.9/qtharmony/widgets/basic/styles/check_box.css
+-rw-r--r--   0        0        0       63 2024-05-12 06:38:54.304789 qtharmony-0.1.9/qtharmony/widgets/basic/styles/digital_entry.css
+-rw-r--r--   0        0        0      139 2024-05-11 14:29:14.509702 qtharmony-0.1.9/qtharmony/widgets/basic/styles/drop_down_menu.css
+-rw-r--r--   0        0        0       56 2024-05-11 14:29:14.509702 qtharmony-0.1.9/qtharmony/widgets/basic/styles/entry.css
+-rw-r--r--   0        0        0       60 2024-05-12 06:38:54.308122 qtharmony-0.1.9/qtharmony/widgets/basic/styles/group_box.css
+-rw-r--r--   0        0        0       35 2024-05-11 06:45:00.352043 qtharmony-0.1.9/qtharmony/widgets/basic/styles/label.css
+-rw-r--r--   0        0        0        0 2024-05-12 06:38:54.308122 qtharmony-0.1.9/qtharmony/widgets/basic/styles/path_entry.css
+-rw-r--r--   0        0        0       67 2024-05-12 06:38:54.318122 qtharmony-0.1.9/qtharmony/widgets/basic/styles/radio_button.css
+-rw-r--r--   0        0        0        0 2024-05-12 07:15:27.113900 qtharmony-0.1.9/qtharmony/widgets/basic/styles/splitter.css
+-rw-r--r--   0        0        0      313 2024-05-11 05:40:26.236219 qtharmony-0.1.9/qtharmony/widgets/basic/styles/widgets_list.css
+-rw-r--r--   0        0        0     1578 2024-05-11 05:40:26.236219 qtharmony-0.1.9/qtharmony/widgets/basic/widgets_list.py
+-rw-r--r--   0        0        0       36 2024-05-11 05:40:26.236219 qtharmony-0.1.9/qtharmony/windows/__init__.py
+-rw-r--r--   0        0        0     2692 2024-05-12 07:15:27.113900 qtharmony-0.1.9/qtharmony/windows/main_window.py
+-rw-r--r--   0        0        0        0 2024-05-11 14:29:14.509702 qtharmony-0.1.9/qtharmony/windows/styles/main_window.css
+-rw-r--r--   0        0        0     2723 1970-01-01 00:00:00.000000 qtharmony-0.1.9/PKG-INFO
```

### Comparing `qtharmony-0.1.8/LICENSE` & `qtharmony-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `qtharmony-0.1.8/README.md` & `qtharmony-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `qtharmony-0.1.8/pyproject.toml` & `qtharmony-0.1.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "QtHarmony"
-version = "0.1.8"
+version = "0.1.9"
 description = "QtHarmony - is a Cutting-Edge GUI Library Built on PyQt6 QtHarmony is a intuitive graphical user interface (GUI) library designed to simplify the development of modern, visually stunning, and highly functional applications. Built on the robust foundation of PyQt6. Now QtHarmony is in development."
 authors = ["chebupelka8 <stpzamyatin@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.11,<3.13"
```

### Comparing `qtharmony-0.1.8/qtharmony/constructor/initialize.py` & `qtharmony-0.1.9/qtharmony/constructor/initialize.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.1.8/qtharmony/resources/themes/dark-default.json` & `qtharmony-0.1.9/qtharmony/resources/themes/dark-default.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8181818181818182%*

 * *Differences: {"'Splitter'": "OrderedDict([('object-name', 'QSplitter#splitter')])", 'delete': "['PathEntry']"}*

```diff
@@ -95,18 +95,14 @@
         "": {
             "background-color": "#252525",
             "border": "none",
             "border-radius": "0px"
         },
         "object-name": "QMainWindow#main-window"
     },
-    "PathEntry": {
-        "": {},
-        "object-name": "QWidget#path-entry"
-    },
     "PushButton": {
         "": {
             "background-color": "#405cf5",
             "border": "none",
             "border-radius": "6px"
         },
         ":hover": {
@@ -125,9 +121,12 @@
             "border": "1px solid #0166fc",
             "border-radius": "7px"
         },
         "::indicator:checked": {
             "background-color": "#0166fc"
         },
         "object-name": "QRadioButton#radio-button"
+    },
+    "Splitter": {
+        "object-name": "QSplitter#splitter"
     }
 }
```

### Comparing `qtharmony-0.1.8/qtharmony/resources/ui/Icon.png` & `qtharmony-0.1.9/qtharmony/resources/ui/Icon.png`

 * *Files identical despite different names*

### Comparing `qtharmony-0.1.8/qtharmony/resources/ui/Logo.png` & `qtharmony-0.1.9/qtharmony/resources/ui/Logo.png`

 * *Files identical despite different names*

### Comparing `qtharmony-0.1.8/qtharmony/resources/ui/angle-down.png` & `qtharmony-0.1.9/qtharmony/resources/ui/angle-down.png`

 * *Files identical despite different names*

### Comparing `qtharmony-0.1.8/qtharmony/src/core/dialog.py` & `qtharmony-0.1.9/qtharmony/src/core/dialog.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.1.8/qtharmony/src/core/font.py` & `qtharmony-0.1.9/qtharmony/src/core/font.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.1.8/qtharmony/src/core/load.py` & `qtharmony-0.1.9/qtharmony/src/core/load.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.1.8/qtharmony/src/core/theme/theme_builder.py` & `qtharmony-0.1.9/qtharmony/src/core/theme/theme_builder.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.1.8/qtharmony/src/core/theme/theme_manager.py` & `qtharmony-0.1.9/qtharmony/src/core/theme/theme_manager.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,14 +12,19 @@
     from PySide6.QtWidgets import QWidget
 
 
 class ThemeManager:
     __widgets: list["QWidget"] = []
     __current_theme: str = "Dark-Default" 
 
+    @classmethod
+    def change_theme(cls, __name: str) -> None:
+        cls.__current_theme = __name
+        cls.update()
+
     @staticmethod
     def get_all_themes() -> list[str]:
         res: list[str] = []
 
         for theme in os.listdir(THEME_RESOURCES):
             res.append(os.path.join(THEME_RESOURCES, theme))
         
@@ -39,24 +44,18 @@
     
     @classmethod
     def update(cls) -> None:
         data = ThemeBuilder.build_theme(cls.get_theme_by_name(cls.__current_theme))
 
         for widget in cls.__widgets:
             try:
-                widget.setStyleSheet(data[widget.__class__.__name__] + widget.styleSheet())
+                widget.setStyleSheet(data[widget.__class__.__name__] + widget.stylesheet)  # type: ignore
             
             except KeyError:
-                ...
-            
-            # print(widget.styleSheet())
-            # print("\n\n\n----------------\n\n\n")
-            # print(widget.styleSheet())
-
-            # print(data[widget.__class__.__name__])
+                widget.setStyleSheet(widget.stylesheet)  # type: ignore
 
     @classmethod
     def add_widgets(cls, *__widgets: "QWidget") -> None:
         for widget in __widgets:
             cls.__widgets.append(widget)
     
     @classmethod
```

### Comparing `qtharmony-0.1.8/qtharmony/widgets/basic/button.py` & `qtharmony-0.1.9/qtharmony/widgets/basic/button.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,19 +45,19 @@
 
 
         super().__init__(parent)
         ThemeManager.add_widgets(self)
 
         if font is not None: self.setFont(font)
 
-        self.setStyleSheet(StyleSheetLoader.load_stylesheet(
+        self.stylesheet = StyleSheetLoader.load_stylesheet(
             __file__, "styles/button.css", 
             name="PushButton", obj_name="QPushButton#button",
             stylesheet=stylesheet
-        ))
+        )
         
         self.setObjectName("button")
         self.setFixedSize(QSize(*size))
 
         if text is not None:
             self.setText(text)
```

### Comparing `qtharmony-0.1.8/qtharmony/widgets/basic/check_box.py` & `qtharmony-0.1.9/qtharmony/widgets/basic/check_box.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,13 +52,12 @@
         self.setCheckable(is_checkable)
         self.setDisabled(is_disabled)
 
         self.setObjectName("check-box")
         if text is not None:
             self.setText(text)
         
-        self.setStyleSheet(StyleSheetLoader.load_stylesheet(
+        self.stylesheet = StyleSheetLoader.load_stylesheet(
             __file__, "styles/check_box.css", 
             name="CheckBox", obj_name="CheckBox#check-box",
             stylesheet=stylesheet
-        ))
-
+        )
```

### Comparing `qtharmony-0.1.8/qtharmony/widgets/basic/digital_entry.py` & `qtharmony-0.1.9/qtharmony/widgets/basic/digital_entry.py`

 * *Files 5% similar despite different names*

```diff
@@ -49,13 +49,12 @@
         self.setFixedSize(QSize(*size))
         if not include_buttons: self.setButtonSymbols(QSpinBox.ButtonSymbols.NoButtons)
         if font is not None: self.setFont(font)
 
         self.setObjectName("digital-entry")
         self.setRange(*range)
 
-        self.setStyleSheet(StyleSheetLoader.load_stylesheet(
+        self.stylesheet = StyleSheetLoader.load_stylesheet(
             __file__, "styles/digital_entry.css", 
             name="DigitalEntry", obj_name="QSpinBox#digital-entry",
             stylesheet=stylesheet
-        ))
-
+        )
```

### Comparing `qtharmony-0.1.8/qtharmony/widgets/basic/drop_down_menu.py` & `qtharmony-0.1.9/qtharmony/widgets/basic/drop_down_menu.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,19 +55,19 @@
         self.__values = []
 
         if values is not None: self.__values = [*values]
         self.addItems(self.__values)
         self.setObjectName("drop-down-menu")
         if font is not None: self.setFont(font)
 
-        self.setStyleSheet(StyleSheetLoader.load_stylesheet(
+        self.stylesheet = StyleSheetLoader.load_stylesheet(
             __file__, "styles/drop_down_menu.css", 
             name="DropDownMenu", obj_name="QComboBox#drop-down-menu",
             stylesheet=stylesheet
-        ))
+        )
 
         self.__load_down_arrow_style()
     
     def __load_down_arrow_style(self) -> None:
         """
         Loads the custom style for the drop-down arrow in the DropDownMenu widget.
         """
```

### Comparing `qtharmony-0.1.8/qtharmony/widgets/basic/entry.py` & `qtharmony-0.1.9/qtharmony/widgets/basic/entry.py`

 * *Files 6% similar despite different names*

```diff
@@ -49,13 +49,12 @@
         if placeholder is not None: self.setPlaceholderText(placeholder)
         if font is not None: self.setFont(font)
 
         self.setFixedSize(QSize(*size))
         self.setObjectName("entry")
         self.setFocusPolicy(Qt.FocusPolicy.WheelFocus)
 
-        self.setStyleSheet(StyleSheetLoader.load_stylesheet(
+        self.stylesheet = StyleSheetLoader.load_stylesheet(
             __file__, "styles/entry.css", 
             name="Entry", obj_name="QLineEdit#entry",
             stylesheet=stylesheet
-        ))
-
+        )
```

### Comparing `qtharmony-0.1.8/qtharmony/widgets/basic/groups.py` & `qtharmony-0.1.9/qtharmony/widgets/basic/groups.py`

 * *Files 9% similar despite different names*

```diff
@@ -37,15 +37,15 @@
             parent (Optional["QWidget"], optional): Parent widget of the group box. Defaults to None.
         """
 
         super().__init__(parent)
         ThemeManager.add_widgets(self)
 
         self.setObjectName("group-box")
-        self.setStyleSheet(StyleSheetLoader.load_stylesheet(
+        self.stylesheet = StyleSheetLoader.load_stylesheet(
             __file__, "styles/group_box.css", 
             name="GroupBox", obj_name="QGroupBox#group-box",
             stylesheet=stylesheet
-        ))
+        )
 
         if title is not None: self.setTitle(title)
         self.setFixedSize(*size)
```

### Comparing `qtharmony-0.1.8/qtharmony/widgets/basic/label.py` & `qtharmony-0.1.9/qtharmony/widgets/basic/label.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from PySide6.QtWidgets import QLabel
 
 from qtharmony.src.core import Font, StyleSheetLoader
+from qtharmony.src.core.theme import ThemeManager
 
 from typing import Optional, TYPE_CHECKING
 
 if TYPE_CHECKING:
     from PySide6.QtWidgets import QWidget
 
 
@@ -47,42 +48,37 @@
             color (str, optional): The color of the label text. Defaults to "#000000".
             word_wrap (bool, optional): Flag to enable word wrap for the label text. Defaults to False.
             stylesheet (Optional[str], optional): Custom stylesheet for the label widget. Defaults to None.
             parent (Optional["QWidget"], optional): Parent widget of the label. Defaults to None.
         """
 
         super().__init__(parent)
+        ThemeManager.add_widgets(self)
 
         self.setObjectName("label")
-        self.setStyleSheet(StyleSheetLoader.load_stylesheet(
+        self.stylesheet = StyleSheetLoader.load_stylesheet(
             __file__, "styles/label.css", 
             name="Label", obj_name="QLabel#label",
             stylesheet=stylesheet
-        ))
+        )
 
         self.setText(text)
         self.set_color(color)
         
         self.setWordWrap(word_wrap)
         self.setFont(Font.get_system_font(font_family, font_size, bold, italic))
+
+        print(self.stylesheet)
     
     def set_color(self, color: str) -> None:
         """
         Sets the color of the label text.
 
         Args:
             color (str): The color of the label text.
         """
 
-        self.__append_stylesheet("Label {" + f"color: {color}" + "}")
-    
-    def __append_stylesheet(self, stylesheet: str) -> None:
-        """
-        Appends a custom stylesheet to the label widget.
-
-        Args:
-            stylesheet (str): The custom stylesheet to be appended.
-        """
-
-        self.setStyleSheet(StyleSheetLoader.append_stylesheet(
-            self.styleSheet(), stylesheet, name="Label", obj_name="QLabel#label"
-        ))
+        self.stylesheet = StyleSheetLoader.append_stylesheet(
+            self.stylesheet, 
+            "Label {" + f"color: {color}" + "}",
+            "Label", "QLabel#label", reversed=True
+        )
```

### Comparing `qtharmony-0.1.8/qtharmony/widgets/basic/path_entry.py` & `qtharmony-0.1.9/qtharmony/widgets/basic/path_entry.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 from PySide6.QtWidgets import ( 
     QWidget, QHBoxLayout, 
     QSpacerItem, QSizePolicy
 )
 
 from qtharmony.src.core import FileDialog, StyleSheetLoader
-from qtharmony.src.core.theme import ThemeManager
 
 from .button import PushButton
 from .entry import Entry
 
 from typing import Optional, TYPE_CHECKING
 if TYPE_CHECKING:
     from PySide6.QtGui import QFont
@@ -49,15 +48,14 @@
             size (tuple[int, int], optional): The size of the path entry widget (width, height). Defaults to (200, 30).
             font (Optional["QFont"], optional): The font to be used for text input. Defaults to None.
             stylesheet (Optional[str], optional): Custom stylesheet for the path entry widget. Defaults to None.
             parent (Optional["QWidget"], optional): Parent widget of the path entry. Defaults to None.
         """        
 
         super().__init__(parent)
-        ThemeManager.add_widgets(self)
 
         self.setObjectName("path-entry")
         if font is not None: self.setFont(font)
 
         self.setStyleSheet(StyleSheetLoader.load_stylesheet(
             __file__, "styles/path_entry.css", 
             name="PathEntry", obj_name="QWidget#path-entry",
```

### Comparing `qtharmony-0.1.8/qtharmony/widgets/basic/radio_button.py` & `qtharmony-0.1.9/qtharmony/widgets/basic/radio_button.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,12 +40,12 @@
         super().__init__(parent)
         ThemeManager.add_widgets(self)
 
         if text is not None: self.setText(text)
         self.setFixedSize(QSize(*size))
 
         self.setObjectName("radio-button")
-        self.setStyleSheet(StyleSheetLoader.load_stylesheet(
+        self.stylesheet = StyleSheetLoader.load_stylesheet(
             __file__, "styles/radio_button.css", 
             name="RadioButton", obj_name="QRadioButton#radio-button",
             stylesheet=stylesheet
-        ))
+        )
```

### Comparing `qtharmony-0.1.8/qtharmony/widgets/basic/splitter.py` & `qtharmony-0.1.9/qtharmony/widgets/basic/splitter.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from PySide6.QtWidgets import QSplitter
 from PySide6.QtCore import Qt
 
 from qtharmony.src.core import StyleSheetLoader
+from qtharmony.src.core.theme import ThemeManager
 
 from typing import Optional, TYPE_CHECKING
 if TYPE_CHECKING:
     from PySide6.QtWidgets import QWidget
 
 
 class Splitter(QSplitter):
@@ -32,20 +33,22 @@
             stylesheet (Optional[str], optional): Custom stylesheet for the splitter. Defaults to None.
             parent (Optional["QWidget"], optional): Parent widget of the splitter. Defaults to None.
         """
 
         if __orientation == "horizontal": super().__init__(Qt.Orientation.Horizontal, parent)
         elif __orientation == "vertical": super().__init__(Qt.Orientation.Vertical, parent)
 
+        ThemeManager.add_widgets(self)
+
         self.setObjectName("splitter")
-        self.setStyleSheet(StyleSheetLoader.load_stylesheet(
+        self.stylesheet = StyleSheetLoader.load_stylesheet(
             __file__, "styles/splitter.css", 
             name="Splitter", obj_name="QSplitter#splitter",
             stylesheet=stylesheet
-        ))
+        )
 
     def addWidget(self, widget):
         """
         Adds a widget to the splitter and sets it as non-collapsible.
 
         Args:
             widget (QWidget): The widget to be added to the splitter.
```

### Comparing `qtharmony-0.1.8/qtharmony/widgets/basic/widgets_list.py` & `qtharmony-0.1.9/qtharmony/widgets/basic/widgets_list.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.1.8/qtharmony/windows/main_window.py` & `qtharmony-0.1.9/qtharmony/windows/main_window.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,19 +50,19 @@
         super().__init__(parent)
         ThemeManager.add_widgets(self)
 
         if widget is not None: self.setCentralWidget(widget)
         self.setWindowIcon(QIcon(f"{os.path.join(UI_RESOURCES, 'Icon.png')}"))
         
         self.setObjectName("main-window")
-        self.setStyleSheet(StyleSheetLoader.load_stylesheet(
+        self.stylesheet = StyleSheetLoader.load_stylesheet(
             __file__, "styles/main_window.css", 
             name="MainWindow", obj_name="QMainWindow#main-window",
             stylesheet=stylesheet
-        ))
+        )
 
         self.resize(*size)
         if title is not None: self.setWindowTitle(title)
         else: self.setWindowTitle("QtHarmony")
 
         if not is_resizable: self.setFixedSize(*size)
```

### Comparing `qtharmony-0.1.8/PKG-INFO` & `qtharmony-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QtHarmony
-Version: 0.1.8
+Version: 0.1.9
 Summary: QtHarmony - is a Cutting-Edge GUI Library Built on PyQt6 QtHarmony is a intuitive graphical user interface (GUI) library designed to simplify the development of modern, visually stunning, and highly functional applications. Built on the robust foundation of PyQt6. Now QtHarmony is in development.
 License: MIT
 Author: chebupelka8
 Author-email: stpzamyatin@gmail.com
 Requires-Python: >=3.11,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

