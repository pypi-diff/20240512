# Comparing `tmp/menuchoice-0.2.tar.gz` & `tmp/menuchoice-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "menuchoice-0.2.tar", last modified: Fri May 10 10:50:53 2024, max compression
+gzip compressed data, was "menuchoice-0.3.tar", last modified: Sun May 12 03:46:58 2024, max compression
```

## Comparing `menuchoice-0.2.tar` & `menuchoice-0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 xyz       (1000) xyz       (1000)        0 2024-05-10 10:50:53.891928 menuchoice-0.2/
--rw-r--r--   0 xyz       (1000) xyz       (1000)     1465 2024-05-10 10:50:53.891928 menuchoice-0.2/PKG-INFO
--rw-r--r--   0 xyz       (1000) xyz       (1000)      726 2024-05-10 10:19:19.000000 menuchoice-0.2/README.md
-drwxr-xr-x   0 xyz       (1000) xyz       (1000)        0 2024-05-10 10:50:53.890928 menuchoice-0.2/menuchoice/
--rw-r--r--   0 xyz       (1000) xyz       (1000)     4035 2024-05-10 10:49:57.000000 menuchoice-0.2/menuchoice/__init__.py
--rw-r--r--   0 xyz       (1000) xyz       (1000)      643 2024-05-10 05:16:56.000000 menuchoice-0.2/menuchoice/_validator.py
-drwxr-xr-x   0 xyz       (1000) xyz       (1000)        0 2024-05-10 10:50:53.891928 menuchoice-0.2/menuchoice/curser_control/
--rw-r--r--   0 xyz       (1000) xyz       (1000)     3938 2024-05-10 06:53:29.000000 menuchoice-0.2/menuchoice/curser_control/_cursorInput.py
--rw-r--r--   0 xyz       (1000) xyz       (1000)      142 2024-05-10 03:13:36.000000 menuchoice-0.2/menuchoice/exceptions.py
-drwxr-xr-x   0 xyz       (1000) xyz       (1000)        0 2024-05-10 10:50:53.891928 menuchoice-0.2/menuchoice.egg-info/
--rw-r--r--   0 xyz       (1000) xyz       (1000)     1465 2024-05-10 10:50:53.000000 menuchoice-0.2/menuchoice.egg-info/PKG-INFO
--rw-r--r--   0 xyz       (1000) xyz       (1000)      269 2024-05-10 10:50:53.000000 menuchoice-0.2/menuchoice.egg-info/SOURCES.txt
--rw-r--r--   0 xyz       (1000) xyz       (1000)        1 2024-05-10 10:50:53.000000 menuchoice-0.2/menuchoice.egg-info/dependency_links.txt
--rw-r--r--   0 xyz       (1000) xyz       (1000)       11 2024-05-10 10:50:53.000000 menuchoice-0.2/menuchoice.egg-info/top_level.txt
--rw-r--r--   0 xyz       (1000) xyz       (1000)       38 2024-05-10 10:50:53.891928 menuchoice-0.2/setup.cfg
--rw-r--r--   0 xyz       (1000) xyz       (1000)     1028 2024-05-10 10:49:41.000000 menuchoice-0.2/setup.py
+drwxr-xr-x   0 xyz       (1000) xyz       (1000)        0 2024-05-12 03:46:58.709096 menuchoice-0.3/
+-rw-r--r--   0 xyz       (1000) xyz       (1000)     1793 2024-05-12 03:46:58.709096 menuchoice-0.3/PKG-INFO
+-rw-r--r--   0 xyz       (1000) xyz       (1000)     1055 2024-05-12 03:45:48.000000 menuchoice-0.3/README.md
+drwxr-xr-x   0 xyz       (1000) xyz       (1000)        0 2024-05-12 03:46:58.709096 menuchoice-0.3/menuchoice/
+-rw-r--r--   0 xyz       (1000) xyz       (1000)     4916 2024-05-12 02:28:07.000000 menuchoice-0.3/menuchoice/__init__.py
+-rw-r--r--   0 xyz       (1000) xyz       (1000)      643 2024-05-10 05:16:56.000000 menuchoice-0.3/menuchoice/_validator.py
+drwxr-xr-x   0 xyz       (1000) xyz       (1000)        0 2024-05-12 03:46:58.709096 menuchoice-0.3/menuchoice/cursor_control/
+-rw-r--r--   0 xyz       (1000) xyz       (1000)     6201 2024-05-12 03:37:00.000000 menuchoice-0.3/menuchoice/cursor_control/_cursorInput.py
+-rw-r--r--   0 xyz       (1000) xyz       (1000)      142 2024-05-10 03:13:36.000000 menuchoice-0.3/menuchoice/exceptions.py
+drwxr-xr-x   0 xyz       (1000) xyz       (1000)        0 2024-05-12 03:46:58.709096 menuchoice-0.3/menuchoice.egg-info/
+-rw-r--r--   0 xyz       (1000) xyz       (1000)     1793 2024-05-12 03:46:58.000000 menuchoice-0.3/menuchoice.egg-info/PKG-INFO
+-rw-r--r--   0 xyz       (1000) xyz       (1000)      269 2024-05-12 03:46:58.000000 menuchoice-0.3/menuchoice.egg-info/SOURCES.txt
+-rw-r--r--   0 xyz       (1000) xyz       (1000)        1 2024-05-12 03:46:58.000000 menuchoice-0.3/menuchoice.egg-info/dependency_links.txt
+-rw-r--r--   0 xyz       (1000) xyz       (1000)       11 2024-05-12 03:46:58.000000 menuchoice-0.3/menuchoice.egg-info/top_level.txt
+-rw-r--r--   0 xyz       (1000) xyz       (1000)       38 2024-05-12 03:46:58.709096 menuchoice-0.3/setup.cfg
+-rw-r--r--   0 xyz       (1000) xyz       (1000)     1028 2024-05-10 10:49:41.000000 menuchoice-0.3/setup.py
```

### Comparing `menuchoice-0.2/PKG-INFO` & `menuchoice-0.3/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: menuchoice
-Version: 0.2
+Version: 0.3
 Summary: Command line menu selector.
 Home-page: https://github.com/xyzpw/menuchoice/
 Author: xyzpw
 Maintainer: xyzpw
 License: MIT
 Keywords: menu selector,item selector,ansi
 Classifier: Programming Language :: Python :: 3
@@ -16,29 +16,34 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Environment :: Console
 Classifier: Environment :: Console :: Curses
 Classifier: Intended Audience :: Developers
 Description-Content-Type: text/markdown
 
 # menuchoice
+![Pepy Total Downlods](https://img.shields.io/pepy/dt/menuchoice)
+![GitHub repo size](https://img.shields.io/github/repo-size/xyzpw/menuchoice)
+
 Command line menu selector
 
+![menuchoice-demo2](https://github.com/xyzpw/menuchoice/assets/76017734/c3ca060d-0c39-47be-9173-fa0d415a20b9)
+
 ## Usage
 Creating a selection menu:
 ```python
 import menuchoice
 myMenu = menuchoice.MenuSelector(items=[
     "Hip-hop",
     "Rock",
     "Pop",
     "Country",
     "EDM",
 ], title="Most Streamed Music USA", description="Select a genre of music.")
 ```
-> [!HINT]
+> [!TIP]
 > items can be given brief descriptions if they are type dictionary.
 > `{"option": "brief description"}`
 
 Selecting an option:
 ```python
 myMenu.prompt_select() # basic user-input method
 myMenu.arrow_select()
@@ -47,12 +52,14 @@
 ```python
 [(4, "EDM")]
 ```
 Additionally, multiple options can be selected
 ```python
 # no less than 2, no more than 3
 myMenu.arrow_select(max_items=(2, 3))
+# Adds an option to select all items
+myMenu.arrow_select(allow_all=True)
 ```
 Output:
 ```python
 [(4, "EDM"), (1, "Rock")]
 ```
```

### Comparing `menuchoice-0.2/README.md` & `menuchoice-0.3/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 # menuchoice
+![Pepy Total Downlods](https://img.shields.io/pepy/dt/menuchoice)
+![GitHub repo size](https://img.shields.io/github/repo-size/xyzpw/menuchoice)
+
 Command line menu selector
 
+![menuchoice-demo2](https://github.com/xyzpw/menuchoice/assets/76017734/c3ca060d-0c39-47be-9173-fa0d415a20b9)
+
 ## Usage
 Creating a selection menu:
 ```python
 import menuchoice
 myMenu = menuchoice.MenuSelector(items=[
     "Hip-hop",
     "Rock",
     "Pop",
     "Country",
     "EDM",
 ], title="Most Streamed Music USA", description="Select a genre of music.")
 ```
-> [!HINT]
+> [!TIP]
 > items can be given brief descriptions if they are type dictionary.
 > `{"option": "brief description"}`
 
 Selecting an option:
 ```python
 myMenu.prompt_select() # basic user-input method
 myMenu.arrow_select()
@@ -26,12 +31,14 @@
 ```python
 [(4, "EDM")]
 ```
 Additionally, multiple options can be selected
 ```python
 # no less than 2, no more than 3
 myMenu.arrow_select(max_items=(2, 3))
+# Adds an option to select all items
+myMenu.arrow_select(allow_all=True)
 ```
 Output:
 ```python
 [(4, "EDM"), (1, "Rock")]
-```
+```
```

### Comparing `menuchoice-0.2/menuchoice/__init__.py` & `menuchoice-0.3/menuchoice/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Command line menu selector."""
 
 import curses
 import re
-from .curser_control import _cursorInput
+from .cursor_control import _cursorInput
 from .exceptions import *
 from . import _validator
 
-__version__ = "0.2"
+__version__ = "0.3"
 __author__ = "xyzpw"
 __description__ = "Command line menu selector."
 __license__ = "MIT"
 
 class MenuSelector:
     """Contains items which can be prompted via a menu selector."""
     def __init__(self, items: list | dict, title: str = None, description: str = None):
@@ -29,43 +29,57 @@
                     lengthiestItem = int(_length)
         makePadding = lambda itemStr: f"{' '*(lengthiestItem - len(itemStr))}" if lengthiestItem > 1 else ""
         for item in self.items:
             _index = list(self.items).index(item)
             menu += "%s%s %s" % (_index, num_sep, item)
             menu += f" - {makePadding(item)}{self.items.get(item)}\n" if isinstance(self.items, dict) else "\n"
         return menu
-    def prompt_select(self, num_sep: str = ")", align: bool = False, max_items: tuple = (1, 1), clear: bool = False) -> list[tuple]:
+    def prompt_select(self, num_sep: str = ")", align: bool = False,
+            max_items: tuple = (1, 1), clear: bool = False,
+            allow_all: bool = False, center: bool = False) -> list[tuple]:
         """Prompts for an integer while displaying the values associated with that index.
 
         :param num_sep: separator between number and item, e.g. ) for N)
         :param align: aligns items by adding additional spaces between items and their descriptions
         :param max_items: a range of numbers which represent the number of items required to be selected
-        :param clear: clears the screen prior to displaying the menu"""
+        :param clear: clears the screen prior to displaying the menu
+        :param allow_all: adds a select all option to the item list
+        :param center: positions the menu selector to the center of the terminal"""
+        if allow_all:
+            max_items = (max_items[0], len(self.items))
         if not _validator.validateMaxItemsRange(max_items):
             raise MenuItemError("allowed items range is invalid")
         menu = self.createMenuString(num_sep, align)
+        if allow_all: menu += "%d%s Select All\n" % (len(self.items), num_sep)
         if clear:
             print("\x1b[H\x1b[2J\x1b[3J", end='') # using ansi codes to clear buffer and entirety of terminal screen
+        if center: menu = cursor_control._cursorInput.makeStrCentered(menu, True)
         choiceIndexes = re.findall(r"(?P<index>\d+)(?:,\s?|\s|\Z)", input(menu + "> "))
+        if allow_all and str(len(self.items)) in choiceIndexes: choiceIndexes = list(range(len(self.items)))
         if not _validator.validateItemSelectionCount(max_items, choiceIndexes):
             raise MenuItemError("number of items selected is out of range")
         return [(i, list(self.items)[int(i)]) for i in choiceIndexes]
     def arrow_select(self, num_sep: str = ")", align: bool = False,
-            arrow: str = "=>", max_items: tuple = (1, 1)):
+            arrow: str = "=>", max_items: tuple = (1, 1),
+            allow_all: bool = False, center: bool = False):
         """Allows the user to select options with the arrow keys.
 
         :param num_sep: separator between number and item, e.g. ) for N)
         :param align: aligns items by adding additional spaces between items and their descriptions
         :param arrow: the string which represents the arrow that points to the text which will be selected
-        :param max_items: a range of numbers which represent the number of items required to be selected"""
+        :param max_items: a range of numbers which represent the number of items required to be selected
+        :param allow_all: adds a select all option to the item list
+        :param center: positions the menu selector to the center of the terminal"""
+        if allow_all:
+            max_items = (max_items[0], len(self.items))
         if not _validator.validateMaxItemsRange(max_items):
             raise MenuItemError("allowed items range is invalid")
         menu = self.createMenuString(num_sep, align)
         if max_items[1] > 1 if max_items[1] != None else True:
-            selectedIndexes = curses.wrapper(_cursorInput.cursorArrowMultiselectMenu, menu, max_items[1])
+            selectedIndexes = curses.wrapper(_cursorInput.cursorArrowMultiselectMenu, menu, max_items[1], allow_all, center)
             usrChoices = [(i, list(self.items)[i]) for i in selectedIndexes] if selectedIndexes != None else []
         else:
-            selectedIndexes = curses.wrapper(_cursorInput.cursorArrowMenu, menu, arrow)
+            selectedIndexes = curses.wrapper(_cursorInput.cursorArrowMenu, menu, arrow, center)
             usrChoices = [(selectedIndexes, list(self.items)[selectedIndexes])] if selectedIndexes != None else []
         if not _validator.validateItemSelectionCount(max_items, usrChoices):
             raise MenuItemError("number of items selected is out of range")
         return usrChoices
```

### Comparing `menuchoice-0.2/menuchoice/_validator.py` & `menuchoice-0.3/menuchoice/_validator.py`

 * *Files identical despite different names*

### Comparing `menuchoice-0.2/menuchoice.egg-info/PKG-INFO` & `menuchoice-0.3/menuchoice.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: menuchoice
-Version: 0.2
+Version: 0.3
 Summary: Command line menu selector.
 Home-page: https://github.com/xyzpw/menuchoice/
 Author: xyzpw
 Maintainer: xyzpw
 License: MIT
 Keywords: menu selector,item selector,ansi
 Classifier: Programming Language :: Python :: 3
@@ -16,29 +16,34 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Environment :: Console
 Classifier: Environment :: Console :: Curses
 Classifier: Intended Audience :: Developers
 Description-Content-Type: text/markdown
 
 # menuchoice
+![Pepy Total Downlods](https://img.shields.io/pepy/dt/menuchoice)
+![GitHub repo size](https://img.shields.io/github/repo-size/xyzpw/menuchoice)
+
 Command line menu selector
 
+![menuchoice-demo2](https://github.com/xyzpw/menuchoice/assets/76017734/c3ca060d-0c39-47be-9173-fa0d415a20b9)
+
 ## Usage
 Creating a selection menu:
 ```python
 import menuchoice
 myMenu = menuchoice.MenuSelector(items=[
     "Hip-hop",
     "Rock",
     "Pop",
     "Country",
     "EDM",
 ], title="Most Streamed Music USA", description="Select a genre of music.")
 ```
-> [!HINT]
+> [!TIP]
 > items can be given brief descriptions if they are type dictionary.
 > `{"option": "brief description"}`
 
 Selecting an option:
 ```python
 myMenu.prompt_select() # basic user-input method
 myMenu.arrow_select()
@@ -47,12 +52,14 @@
 ```python
 [(4, "EDM")]
 ```
 Additionally, multiple options can be selected
 ```python
 # no less than 2, no more than 3
 myMenu.arrow_select(max_items=(2, 3))
+# Adds an option to select all items
+myMenu.arrow_select(allow_all=True)
 ```
 Output:
 ```python
 [(4, "EDM"), (1, "Rock")]
 ```
```

### Comparing `menuchoice-0.2/setup.py` & `menuchoice-0.3/setup.py`

 * *Files identical despite different names*

