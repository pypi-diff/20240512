# Comparing `tmp/qtharmony-0.1.9.tar.gz` & `tmp/qtharmony-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qtharmony-0.1.9.tar", max compression
+gzip compressed data, was "qtharmony-0.2.0.tar", max compression
```

## Comparing `qtharmony-0.1.9.tar` & `qtharmony-0.2.0.tar`

### file list

```diff
@@ -1,50 +1,53 @@
--rw-r--r--   0        0        0     1067 2024-05-02 17:11:53.147941 qtharmony-0.1.9/LICENSE
--rw-r--r--   0        0        0     1981 2024-05-11 08:16:36.349414 qtharmony-0.1.9/README.md
--rw-r--r--   0        0        0      609 2024-05-12 07:15:40.663236 qtharmony-0.1.9/pyproject.toml
--rw-r--r--   0        0        0      327 2024-05-11 05:40:26.229552 qtharmony-0.1.9/qtharmony/__init__.py
--rw-r--r--   0        0        0       38 2024-05-11 05:40:26.229552 qtharmony-0.1.9/qtharmony/constructor/__init__.py
--rw-r--r--   0        0        0      636 2024-05-12 06:38:54.294789 qtharmony-0.1.9/qtharmony/constructor/initialize.py
--rw-r--r--   0        0        0        2 2024-05-11 08:08:22.630008 qtharmony-0.1.9/qtharmony/resources/__init__.py
--rw-r--r--   0        0        0     3435 2024-05-12 07:15:27.110567 qtharmony-0.1.9/qtharmony/resources/themes/dark-default.json
--rw-r--r--   0        0        0      684 2024-05-12 07:15:27.110567 qtharmony-0.1.9/qtharmony/resources/themes/light-default.json
--rw-r--r--   0        0        0    31042 2024-05-11 05:40:26.229552 qtharmony-0.1.9/qtharmony/resources/ui/Icon.png
--rw-r--r--   0        0        0    17484 2024-05-11 05:40:26.229552 qtharmony-0.1.9/qtharmony/resources/ui/Logo.png
--rw-r--r--   0        0        0     5387 2024-05-11 05:40:26.229552 qtharmony-0.1.9/qtharmony/resources/ui/angle-down.png
--rw-r--r--   0        0        0       22 2024-05-11 08:08:22.630008 qtharmony-0.1.9/qtharmony/src/config/__init__.py
--rw-r--r--   0        0        0      233 2024-05-11 14:21:59.267556 qtharmony-0.1.9/qtharmony/src/config/config.py
--rw-r--r--   0        0        0      120 2024-05-11 05:40:26.229552 qtharmony-0.1.9/qtharmony/src/core/__init__.py
--rw-r--r--   0        0        0      985 2024-05-11 05:40:26.232885 qtharmony-0.1.9/qtharmony/src/core/dialog.py
--rw-r--r--   0        0        0      151 2024-05-11 05:40:26.232885 qtharmony-0.1.9/qtharmony/src/core/exceptions.py
--rw-r--r--   0        0        0     2506 2024-05-11 05:40:26.232885 qtharmony-0.1.9/qtharmony/src/core/font.py
--rw-r--r--   0        0        0      876 2024-05-11 17:33:26.077741 qtharmony-0.1.9/qtharmony/src/core/load.py
--rw-r--r--   0        0        0     1235 2024-05-12 07:15:27.110567 qtharmony-0.1.9/qtharmony/src/core/stylesheet.py
--rw-r--r--   0        0        0       80 2024-05-11 14:21:59.267556 qtharmony-0.1.9/qtharmony/src/core/theme/__init__.py
--rw-r--r--   0        0        0     1299 2024-05-11 14:29:14.506368 qtharmony-0.1.9/qtharmony/src/core/theme/theme_builder.py
--rw-r--r--   0        0        0     1903 2024-05-12 07:15:27.110567 qtharmony-0.1.9/qtharmony/src/core/theme/theme_manager.py
--rw-r--r--   0        0        0      433 2024-05-11 08:23:35.711704 qtharmony-0.1.9/qtharmony/widgets/__init__.py
--rw-r--r--   0        0        0     2316 2024-05-12 07:15:27.110567 qtharmony-0.1.9/qtharmony/widgets/basic/button.py
--rw-r--r--   0        0        0     2642 2024-05-12 07:15:27.110567 qtharmony-0.1.9/qtharmony/widgets/basic/check_box.py
--rw-r--r--   0        0        0     2492 2024-05-12 07:15:27.110567 qtharmony-0.1.9/qtharmony/widgets/basic/digital_entry.py
--rw-r--r--   0        0        0     3476 2024-05-12 07:15:27.110567 qtharmony-0.1.9/qtharmony/widgets/basic/drop_down_menu.py
--rw-r--r--   0        0        0     2489 2024-05-12 07:15:27.113900 qtharmony-0.1.9/qtharmony/widgets/basic/entry.py
--rw-r--r--   0        0        0     1663 2024-05-12 07:15:27.113900 qtharmony-0.1.9/qtharmony/widgets/basic/groups.py
--rw-r--r--   0        0        0     3195 2024-05-12 07:15:27.113900 qtharmony-0.1.9/qtharmony/widgets/basic/label.py
--rw-r--r--   0        0        0     3784 2024-05-12 07:15:27.113900 qtharmony-0.1.9/qtharmony/widgets/basic/path_entry.py
--rw-r--r--   0        0        0     1922 2024-05-12 07:15:27.113900 qtharmony-0.1.9/qtharmony/widgets/basic/radio_button.py
--rw-r--r--   0        0        0     1994 2024-05-12 07:15:27.113900 qtharmony-0.1.9/qtharmony/widgets/basic/splitter.py
--rw-r--r--   0        0        0       61 2024-05-12 07:15:27.113900 qtharmony-0.1.9/qtharmony/widgets/basic/styles/button.css
--rw-r--r--   0        0        0      115 2024-05-12 06:38:54.304789 qtharmony-0.1.9/qtharmony/widgets/basic/styles/check_box.css
--rw-r--r--   0        0        0       63 2024-05-12 06:38:54.304789 qtharmony-0.1.9/qtharmony/widgets/basic/styles/digital_entry.css
--rw-r--r--   0        0        0      139 2024-05-11 14:29:14.509702 qtharmony-0.1.9/qtharmony/widgets/basic/styles/drop_down_menu.css
--rw-r--r--   0        0        0       56 2024-05-11 14:29:14.509702 qtharmony-0.1.9/qtharmony/widgets/basic/styles/entry.css
--rw-r--r--   0        0        0       60 2024-05-12 06:38:54.308122 qtharmony-0.1.9/qtharmony/widgets/basic/styles/group_box.css
--rw-r--r--   0        0        0       35 2024-05-11 06:45:00.352043 qtharmony-0.1.9/qtharmony/widgets/basic/styles/label.css
--rw-r--r--   0        0        0        0 2024-05-12 06:38:54.308122 qtharmony-0.1.9/qtharmony/widgets/basic/styles/path_entry.css
--rw-r--r--   0        0        0       67 2024-05-12 06:38:54.318122 qtharmony-0.1.9/qtharmony/widgets/basic/styles/radio_button.css
--rw-r--r--   0        0        0        0 2024-05-12 07:15:27.113900 qtharmony-0.1.9/qtharmony/widgets/basic/styles/splitter.css
--rw-r--r--   0        0        0      313 2024-05-11 05:40:26.236219 qtharmony-0.1.9/qtharmony/widgets/basic/styles/widgets_list.css
--rw-r--r--   0        0        0     1578 2024-05-11 05:40:26.236219 qtharmony-0.1.9/qtharmony/widgets/basic/widgets_list.py
--rw-r--r--   0        0        0       36 2024-05-11 05:40:26.236219 qtharmony-0.1.9/qtharmony/windows/__init__.py
--rw-r--r--   0        0        0     2692 2024-05-12 07:15:27.113900 qtharmony-0.1.9/qtharmony/windows/main_window.py
--rw-r--r--   0        0        0        0 2024-05-11 14:29:14.509702 qtharmony-0.1.9/qtharmony/windows/styles/main_window.css
--rw-r--r--   0        0        0     2723 1970-01-01 00:00:00.000000 qtharmony-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-05-02 17:11:53.147941 qtharmony-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2050 2024-05-12 11:50:16.448380 qtharmony-0.2.0/README.md
+-rw-r--r--   0        0        0      609 2024-05-12 11:50:34.160935 qtharmony-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      327 2024-05-11 05:40:26.229552 qtharmony-0.2.0/qtharmony/__init__.py
+-rw-r--r--   0        0        0       38 2024-05-11 05:40:26.229552 qtharmony-0.2.0/qtharmony/constructor/__init__.py
+-rw-r--r--   0        0        0      636 2024-05-12 06:38:54.294789 qtharmony-0.2.0/qtharmony/constructor/initialize.py
+-rw-r--r--   0        0        0        2 2024-05-11 08:08:22.630008 qtharmony-0.2.0/qtharmony/resources/__init__.py
+-rw-r--r--   0        0        0     4295 2024-05-12 11:50:16.451713 qtharmony-0.2.0/qtharmony/resources/themes/dark-default.json
+-rw-r--r--   0        0        0     4563 2024-05-12 11:50:16.451713 qtharmony-0.2.0/qtharmony/resources/themes/light-default.json
+-rw-r--r--   0        0        0    31042 2024-05-11 05:40:26.229552 qtharmony-0.2.0/qtharmony/resources/ui/Icon.png
+-rw-r--r--   0        0        0    17484 2024-05-11 05:40:26.229552 qtharmony-0.2.0/qtharmony/resources/ui/Logo.png
+-rw-r--r--   0        0        0     5387 2024-05-11 05:40:26.229552 qtharmony-0.2.0/qtharmony/resources/ui/angle-down.png
+-rw-r--r--   0        0        0       22 2024-05-11 08:08:22.630008 qtharmony-0.2.0/qtharmony/src/config/__init__.py
+-rw-r--r--   0        0        0      233 2024-05-11 14:21:59.267556 qtharmony-0.2.0/qtharmony/src/config/config.py
+-rw-r--r--   0        0        0      120 2024-05-11 05:40:26.229552 qtharmony-0.2.0/qtharmony/src/core/__init__.py
+-rw-r--r--   0        0        0      985 2024-05-11 05:40:26.232885 qtharmony-0.2.0/qtharmony/src/core/dialog.py
+-rw-r--r--   0        0        0      151 2024-05-11 05:40:26.232885 qtharmony-0.2.0/qtharmony/src/core/exceptions.py
+-rw-r--r--   0        0        0     2506 2024-05-11 05:40:26.232885 qtharmony-0.2.0/qtharmony/src/core/font.py
+-rw-r--r--   0        0        0      876 2024-05-11 17:33:26.077741 qtharmony-0.2.0/qtharmony/src/core/load.py
+-rw-r--r--   0        0        0      576 2024-05-12 11:50:16.451713 qtharmony-0.2.0/qtharmony/src/core/sizes.py
+-rw-r--r--   0        0        0     1235 2024-05-12 07:41:31.423989 qtharmony-0.2.0/qtharmony/src/core/stylesheet.py
+-rw-r--r--   0        0        0       80 2024-05-11 14:21:59.267556 qtharmony-0.2.0/qtharmony/src/core/theme/__init__.py
+-rw-r--r--   0        0        0     1299 2024-05-11 14:29:14.506368 qtharmony-0.2.0/qtharmony/src/core/theme/theme_builder.py
+-rw-r--r--   0        0        0     1903 2024-05-12 10:25:21.480254 qtharmony-0.2.0/qtharmony/src/core/theme/theme_manager.py
+-rw-r--r--   0        0        0      464 2024-05-12 11:50:16.451713 qtharmony-0.2.0/qtharmony/widgets/__init__.py
+-rw-r--r--   0        0        0     2316 2024-05-12 10:49:33.152065 qtharmony-0.2.0/qtharmony/widgets/basic/button.py
+-rw-r--r--   0        0        0     2642 2024-05-12 07:41:31.423989 qtharmony-0.2.0/qtharmony/widgets/basic/check_box.py
+-rw-r--r--   0        0        0     2492 2024-05-12 07:41:31.423989 qtharmony-0.2.0/qtharmony/widgets/basic/digital_entry.py
+-rw-r--r--   0        0        0     3472 2024-05-12 11:50:16.451713 qtharmony-0.2.0/qtharmony/widgets/basic/drop_down_menu.py
+-rw-r--r--   0        0        0     2489 2024-05-12 10:24:10.276814 qtharmony-0.2.0/qtharmony/widgets/basic/entry.py
+-rw-r--r--   0        0        0      815 2024-05-12 11:50:16.451713 qtharmony-0.2.0/qtharmony/widgets/basic/frame.py
+-rw-r--r--   0        0        0     2704 2024-05-12 11:50:16.451713 qtharmony-0.2.0/qtharmony/widgets/basic/groups.py
+-rw-r--r--   0        0        0     3190 2024-05-12 11:50:16.451713 qtharmony-0.2.0/qtharmony/widgets/basic/label.py
+-rw-r--r--   0        0        0     3784 2024-05-12 07:41:31.423989 qtharmony-0.2.0/qtharmony/widgets/basic/path_entry.py
+-rw-r--r--   0        0        0     1922 2024-05-12 07:41:31.423989 qtharmony-0.2.0/qtharmony/widgets/basic/radio_button.py
+-rw-r--r--   0        0        0     1994 2024-05-12 07:41:31.423989 qtharmony-0.2.0/qtharmony/widgets/basic/splitter.py
+-rw-r--r--   0        0        0       61 2024-05-12 07:41:31.423989 qtharmony-0.2.0/qtharmony/widgets/basic/styles/button.css
+-rw-r--r--   0        0        0      115 2024-05-12 06:38:54.304789 qtharmony-0.2.0/qtharmony/widgets/basic/styles/check_box.css
+-rw-r--r--   0        0        0       63 2024-05-12 06:38:54.304789 qtharmony-0.2.0/qtharmony/widgets/basic/styles/digital_entry.css
+-rw-r--r--   0        0        0      147 2024-05-12 11:50:16.451713 qtharmony-0.2.0/qtharmony/widgets/basic/styles/drop_down_menu.css
+-rw-r--r--   0        0        0      108 2024-05-12 11:50:16.451713 qtharmony-0.2.0/qtharmony/widgets/basic/styles/entry.css
+-rw-r--r--   0        0        0        0 2024-05-12 11:50:16.451713 qtharmony-0.2.0/qtharmony/widgets/basic/styles/frame.css
+-rw-r--r--   0        0        0       60 2024-05-12 06:38:54.308122 qtharmony-0.2.0/qtharmony/widgets/basic/styles/group_box.css
+-rw-r--r--   0        0        0       35 2024-05-11 06:45:00.352043 qtharmony-0.2.0/qtharmony/widgets/basic/styles/label.css
+-rw-r--r--   0        0        0        0 2024-05-12 06:38:54.308122 qtharmony-0.2.0/qtharmony/widgets/basic/styles/path_entry.css
+-rw-r--r--   0        0        0       67 2024-05-12 06:38:54.318122 qtharmony-0.2.0/qtharmony/widgets/basic/styles/radio_button.css
+-rw-r--r--   0        0        0        0 2024-05-12 07:41:31.423989 qtharmony-0.2.0/qtharmony/widgets/basic/styles/splitter.css
+-rw-r--r--   0        0        0      313 2024-05-11 05:40:26.236219 qtharmony-0.2.0/qtharmony/widgets/basic/styles/widgets_list.css
+-rw-r--r--   0        0        0     1578 2024-05-11 05:40:26.236219 qtharmony-0.2.0/qtharmony/widgets/basic/widgets_list.py
+-rw-r--r--   0        0        0       36 2024-05-11 05:40:26.236219 qtharmony-0.2.0/qtharmony/windows/__init__.py
+-rw-r--r--   0        0        0     2692 2024-05-12 07:41:31.423989 qtharmony-0.2.0/qtharmony/windows/main_window.py
+-rw-r--r--   0        0        0        0 2024-05-11 14:29:14.509702 qtharmony-0.2.0/qtharmony/windows/styles/main_window.css
+-rw-r--r--   0        0        0     2792 1970-01-01 00:00:00.000000 qtharmony-0.2.0/PKG-INFO
```

### Comparing `qtharmony-0.1.9/LICENSE` & `qtharmony-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qtharmony-0.1.9/README.md` & `qtharmony-0.2.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -81,7 +81,10 @@
     window = MainWindow(widget=Widget(), title="Hello", size=(600, 400))
     window.run()
 
     Initialization.exec()
 ```
 
 <img src="examples/buttons/default_button.png">
+
+<h3>Other Examples</h3>
+<img src="examples/groupbox/group_box.png">
```

### Comparing `qtharmony-0.1.9/pyproject.toml` & `qtharmony-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "QtHarmony"
-version = "0.1.9"
+version = "0.2.0"
 description = "QtHarmony - is a Cutting-Edge GUI Library Built on PyQt6 QtHarmony is a intuitive graphical user interface (GUI) library designed to simplify the development of modern, visually stunning, and highly functional applications. Built on the robust foundation of PyQt6. Now QtHarmony is in development."
 authors = ["chebupelka8 <stpzamyatin@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.11,<3.13"
```

### Comparing `qtharmony-0.1.9/qtharmony/constructor/initialize.py` & `qtharmony-0.2.0/qtharmony/constructor/initialize.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.1.9/qtharmony/resources/ui/Icon.png` & `qtharmony-0.2.0/qtharmony/resources/ui/Icon.png`

 * *Files identical despite different names*

### Comparing `qtharmony-0.1.9/qtharmony/resources/ui/Logo.png` & `qtharmony-0.2.0/qtharmony/resources/ui/Logo.png`

 * *Files identical despite different names*

### Comparing `qtharmony-0.1.9/qtharmony/resources/ui/angle-down.png` & `qtharmony-0.2.0/qtharmony/resources/ui/angle-down.png`

 * *Files identical despite different names*

### Comparing `qtharmony-0.1.9/qtharmony/src/core/dialog.py` & `qtharmony-0.2.0/qtharmony/src/core/dialog.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.1.9/qtharmony/src/core/font.py` & `qtharmony-0.2.0/qtharmony/src/core/font.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.1.9/qtharmony/src/core/load.py` & `qtharmony-0.2.0/qtharmony/src/core/load.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.1.9/qtharmony/src/core/stylesheet.py` & `qtharmony-0.2.0/qtharmony/src/core/stylesheet.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.1.9/qtharmony/src/core/theme/theme_builder.py` & `qtharmony-0.2.0/qtharmony/src/core/theme/theme_builder.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.1.9/qtharmony/src/core/theme/theme_manager.py` & `qtharmony-0.2.0/qtharmony/src/core/theme/theme_manager.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.1.9/qtharmony/widgets/basic/button.py` & `qtharmony-0.2.0/qtharmony/widgets/basic/button.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.1.9/qtharmony/widgets/basic/check_box.py` & `qtharmony-0.2.0/qtharmony/widgets/basic/check_box.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.1.9/qtharmony/widgets/basic/digital_entry.py` & `qtharmony-0.2.0/qtharmony/widgets/basic/digital_entry.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.1.9/qtharmony/widgets/basic/drop_down_menu.py` & `qtharmony-0.2.0/qtharmony/widgets/basic/drop_down_menu.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,18 +74,18 @@
 
         down_arrow = (
             "\nDropDownMenu::down-arrow {" 
             + f"image: url({os.path.join(UI_RESOURCES, 'angle-down.png')})" 
             + "}"
         )
 
-        self.setStyleSheet(StyleSheetLoader.append_stylesheet(
-            self.styleSheet(), down_arrow, 
+        self.stylesheet = StyleSheetLoader.append_stylesheet(
+            self.stylesheet, down_arrow, 
             name="DropDownMenu", obj_name="QComboBox#drop-down-menu"
-        ))
+        )
 
     def set_items(self, *__values: str) -> None:
         """
         Sets the items in the drop-down menu with the provided values.
 
         Args:
             *__values (str): Variable number of values to populate the drop-down menu.
```

### Comparing `qtharmony-0.1.9/qtharmony/widgets/basic/entry.py` & `qtharmony-0.2.0/qtharmony/widgets/basic/entry.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.1.9/qtharmony/widgets/basic/groups.py` & `qtharmony-0.2.0/qtharmony/widgets/basic/radio_button.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,51 +1,51 @@
-from typing import Optional, TYPE_CHECKING
-
-from PySide6.QtWidgets import (
-    QGroupBox, QButtonGroup
-)
+from PySide6.QtWidgets import QRadioButton
+from PySide6.QtCore import QSize
 
 from qtharmony.src.core import StyleSheetLoader
-from qtharmony.src.core.theme import ThemeManager 
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
-            size: tuple[int, int] = (400, 200),
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
         ThemeManager.add_widgets(self)
 
-        self.setObjectName("group-box")
+        if text is not None: self.setText(text)
+        self.setFixedSize(QSize(*size))
+
+        self.setObjectName("radio-button")
         self.stylesheet = StyleSheetLoader.load_stylesheet(
-            __file__, "styles/group_box.css", 
-            name="GroupBox", obj_name="QGroupBox#group-box",
+            __file__, "styles/radio_button.css", 
+            name="RadioButton", obj_name="QRadioButton#radio-button",
             stylesheet=stylesheet
         )
-
-        if title is not None: self.setTitle(title)
-        self.setFixedSize(*size)
```

### Comparing `qtharmony-0.1.9/qtharmony/widgets/basic/label.py` & `qtharmony-0.2.0/qtharmony/widgets/basic/label.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     def __init__(
             self, 
             text: str,
             font_family: str, 
             font_size: int,
             bold: bool = False,
             italic: bool = False,
-            color: str = "#000000",
+            color: Optional[str] = None,
             word_wrap: bool = False,
             *,
             stylesheet: Optional[str] = None,
             parent: Optional["QWidget"] = None
     ) -> None:
         """
         Initializes the Label widget with optional text, font family, font size, bold, italic, color, word wrap, and stylesheet.
@@ -58,20 +58,18 @@
         self.stylesheet = StyleSheetLoader.load_stylesheet(
             __file__, "styles/label.css", 
             name="Label", obj_name="QLabel#label",
             stylesheet=stylesheet
         )
 
         self.setText(text)
-        self.set_color(color)
+        if color is not None: self.set_color(color)
         
         self.setWordWrap(word_wrap)
         self.setFont(Font.get_system_font(font_family, font_size, bold, italic))
-
-        print(self.stylesheet)
     
     def set_color(self, color: str) -> None:
         """
         Sets the color of the label text.
 
         Args:
             color (str): The color of the label text.
```

### Comparing `qtharmony-0.1.9/qtharmony/widgets/basic/path_entry.py` & `qtharmony-0.2.0/qtharmony/widgets/basic/path_entry.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.1.9/qtharmony/widgets/basic/radio_button.py` & `qtharmony-0.2.0/qtharmony/windows/main_window.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,51 +1,70 @@
-from PySide6.QtWidgets import QRadioButton
-from PySide6.QtCore import QSize
+from PySide6.QtWidgets import QMainWindow, QWidget
+from PySide6.QtGui import QIcon
 
 from qtharmony.src.core import StyleSheetLoader
+from qtharmony.src.config import UI_RESOURCES
+
 from qtharmony.src.core.theme import ThemeManager
 
-from typing import Optional, TYPE_CHECKING
-if TYPE_CHECKING:
-    from PySide6.QtWidgets import QWidget
+from typing import Optional
+import os.path
 
 
-class RadioButton(QRadioButton):
+class MainWindow(QMainWindow):
     """
-    Custom QRadioButton widget for radio button functionality.
+    Custom QMainWindow widget for main window functionality.
 
     Methods:
-    - __init__(text: Optional[str] = None, size: tuple[int, int] = (200, 30),
-              *, stylesheet: Optional[str] = None, parent: Optional["QWidget"] = None): None
-              - Initializes the RadioButton widget with optional text, size, and stylesheet.
+    - __init__(widget: Optional[QWidget] = None, size: tuple[int, int] = (1000, 600),
+              title: Optional[str] = None, is_resizable: bool = True,
+              *, stylesheet: Optional[str] = None, parent: Optional[QWidget] = None): None
+              - Initializes the MainWindow widget with optional central widget, size, title, resizable option, and stylesheet.
+    
+    - run(): None
+              - Displays the main window.
+
     """
 
     def __init__(
-            self,
-            text: Optional[str] = None,
-            size: tuple[int, int] = (200, 30),
+            self, 
+            widget: Optional[QWidget] = None,
+            size: tuple[int, int] = (1000, 600),
+            title: Optional[str] = None,
+            is_resizable: bool = True,
             *,
             stylesheet: Optional[str] = None,
-            parent: Optional["QWidget"] = None
+            parent: Optional[QWidget] = None
     ) -> None:
         """
-        Initializes the RadioButton widget with optional text, size, and stylesheet.
+        Initializes the MainWindow widget with optional central widget, size, title, resizable option, and stylesheet.
 
         Args:
-            text (Optional[str], optional): The text displayed next to the radio button. Defaults to None.
-            size (tuple[int, int], optional): The size of the radio button widget (width, height). Defaults to (200, 30).
-            stylesheet (Optional[str], optional): Custom stylesheet for the radio button widget. Defaults to None.
-            parent (Optional["QWidget"], optional): Parent widget of the radio button. Defaults to None.
+            widget (Optional[QWidget], optional): The central widget to set in the main window. Defaults to None.
+            size (tuple[int, int], optional): The size of the main window (width, height). Defaults to (1000, 600).
+            title (Optional[str], optional): The title of the main window. Defaults to None.
+            is_resizable (bool, optional): Flag to set if the main window is resizable. Defaults to True.
+            stylesheet (Optional[str], optional): Custom stylesheet for the main window. Defaults to None.
+            parent (Optional[QWidget], optional): Parent widget of the main window. Defaults to None.
         """ 
 
         super().__init__(parent)
         ThemeManager.add_widgets(self)
 
-        if text is not None: self.setText(text)
-        self.setFixedSize(QSize(*size))
-
-        self.setObjectName("radio-button")
+        if widget is not None: self.setCentralWidget(widget)
+        self.setWindowIcon(QIcon(f"{os.path.join(UI_RESOURCES, 'Icon.png')}"))
+        
+        self.setObjectName("main-window")
         self.stylesheet = StyleSheetLoader.load_stylesheet(
-            __file__, "styles/radio_button.css", 
-            name="RadioButton", obj_name="QRadioButton#radio-button",
+            __file__, "styles/main_window.css", 
+            name="MainWindow", obj_name="QMainWindow#main-window",
             stylesheet=stylesheet
         )
+
+        self.resize(*size)
+        if title is not None: self.setWindowTitle(title)
+        else: self.setWindowTitle("QtHarmony")
+
+        if not is_resizable: self.setFixedSize(*size)
+    
+    def run(self) -> None:
+        self.show()
```

### Comparing `qtharmony-0.1.9/qtharmony/widgets/basic/splitter.py` & `qtharmony-0.2.0/qtharmony/widgets/basic/splitter.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.1.9/qtharmony/widgets/basic/widgets_list.py` & `qtharmony-0.2.0/qtharmony/widgets/basic/widgets_list.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.1.9/PKG-INFO` & `qtharmony-0.2.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QtHarmony
-Version: 0.1.9
+Version: 0.2.0
 Summary: QtHarmony - is a Cutting-Edge GUI Library Built on PyQt6 QtHarmony is a intuitive graphical user interface (GUI) library designed to simplify the development of modern, visually stunning, and highly functional applications. Built on the robust foundation of PyQt6. Now QtHarmony is in development.
 License: MIT
 Author: chebupelka8
 Author-email: stpzamyatin@gmail.com
 Requires-Python: >=3.11,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -97,7 +97,10 @@
     window.run()
 
     Initialization.exec()
 ```
 
 <img src="examples/buttons/default_button.png">
 
+<h3>Other Examples</h3>
+<img src="examples/groupbox/group_box.png">
+
```

