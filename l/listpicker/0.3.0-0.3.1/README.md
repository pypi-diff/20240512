# Comparing `tmp/listpicker-0.3.0.tar.gz` & `tmp/listpicker-0.3.1.tar.gz`

## Comparing `listpicker-0.3.0.tar` & `listpicker-0.3.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     3185 2020-02-02 00:00:00.000000 listpicker-0.3.0/src/listpicker/__init__.py
--rw-r--r--   0        0        0     3609 2020-02-02 00:00:00.000000 listpicker-0.3.0/src/listpicker/keyboard.py
--rw-r--r--   0        0        0    21202 2020-02-02 00:00:00.000000 listpicker-0.3.0/src/listpicker/listpicker.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 listpicker-0.3.0/src/listpicker/py.typed
--rw-r--r--   0        0        0     2764 2020-02-02 00:00:00.000000 listpicker-0.3.0/src/listpicker/util.py
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 listpicker-0.3.0/.gitignore
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 listpicker-0.3.0/LICENSE
--rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 listpicker-0.3.0/README.md
--rw-r--r--   0        0        0     3187 2020-02-02 00:00:00.000000 listpicker-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     5000 2020-02-02 00:00:00.000000 listpicker-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     3185 2020-02-02 00:00:00.000000 listpicker-0.3.1/src/listpicker/__init__.py
+-rw-r--r--   0        0        0     3559 2020-02-02 00:00:00.000000 listpicker-0.3.1/src/listpicker/keyboard.py
+-rw-r--r--   0        0        0    20987 2020-02-02 00:00:00.000000 listpicker-0.3.1/src/listpicker/listpicker.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 listpicker-0.3.1/src/listpicker/py.typed
+-rw-r--r--   0        0        0     2764 2020-02-02 00:00:00.000000 listpicker-0.3.1/src/listpicker/util.py
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 listpicker-0.3.1/.gitignore
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 listpicker-0.3.1/LICENSE
+-rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 listpicker-0.3.1/README.md
+-rw-r--r--   0        0        0     3187 2020-02-02 00:00:00.000000 listpicker-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     5000 2020-02-02 00:00:00.000000 listpicker-0.3.1/PKG-INFO
```

### Comparing `listpicker-0.3.0/src/listpicker/__init__.py` & `listpicker-0.3.1/src/listpicker/__init__.py`

 * *Files identical despite different names*

### Comparing `listpicker-0.3.0/src/listpicker/keyboard.py` & `listpicker-0.3.1/src/listpicker/keyboard.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 # FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS
 # IN THE SOFTWARE.
 
 import termios
 import tty
-from typing import Any, Optional, TextIO
+from typing import Optional, TextIO
 
 import regex
 
 from .util import bytes_to_int
 
 # https://en.wikipedia.org/wiki/ANSI_escape_code#Terminal_input_sequences
 NAMED_KEY_BY_CODE = {
@@ -47,17 +47,14 @@
     bytes_to_int(0x1B, ord("["), ord("8"), ord("~")): "End",  # vt
     bytes_to_int(0x1B, ord("["), ord("1"), ord("1"), ord("~")): "F1",
     bytes_to_int(0x1B, ord("O"), ord("P")): "F1",
 }
 
 
 class NonCanonicalModeTerminalInput:
-    _file: TextIO
-    _old_attrs: list[Any]
-
     def __init__(self, file: TextIO):
         if not file.isatty():
             raise ValueError(f"file is not a tty: ${file!r}")
 
         self._file = file
 
     def __enter__(self) -> TextIO:
```

### Comparing `listpicker-0.3.0/src/listpicker/listpicker.py` & `listpicker-0.3.1/src/listpicker/listpicker.py`

 * *Files 2% similar despite different names*

```diff
@@ -138,32 +138,14 @@
             case None:
                 checkbox = ""
 
         return f"%-{number_width}s %s%s" % (str(self.number) + ".", checkbox, self.value)
 
 
 class ListPicker:
-    _prompt: list[str]
-    _all_options: list[Option]
-    _options: list[Option]
-    _option_index_width: int
-    _multiselect: bool
-    _multiselect_minimum: int
-    _selected_options: set[Option]
-    _filter = ""
-    _columns: int = 80
-    _lines: int = 24
-    _state = ListPickerState.INACTIVE
-    _infile: TextIO
-    _outfile: TextIO
-    _index: int = 0  # Array index of _options, not Option.number
-    _option_window: range
-    _draw_height: int = 0
-    _max_draw_height: int = 0
-
     def __init__(
         self,
         prompt: str,
         options: Sequence[str],
         *,
         multiselect: bool = False,
         minimum: int = 0,
@@ -175,17 +157,24 @@
         self._all_options = [Option(i + 1, o) for i, o in enumerate(options)]
         self._options = self._all_options
         self._option_index_width = len("%d." % (self._all_options[-1].number))
         self._multiselect = multiselect
         self._multiselect_minimum = minimum
         self._infile = infile
         self._outfile = outfile
-        self._selected_options = set()
+        self._selected_options: set[Option] = set()
         self._preselected_options = set(preselected) if preselected else set()
         self._option_window = range(len(self._all_options))
+        self._filter = ""
+        self._columns = 80
+        self._lines = 24
+        self._state = ListPickerState.INACTIVE
+        self._index = 0  # Array index of _options, not Option.number
+        self._draw_height = 0
+        self._max_draw_height = 0
 
         if self._multiselect_minimum > 0:
             if not self._multiselect:
                 raise ValueError("minimum > 0 has no effect unless multiselect=True")
             if len(self._all_options) < self._multiselect_minimum:
                 raise ValueError("not enough options to satisfy minimum constraint")
```

### Comparing `listpicker-0.3.0/src/listpicker/util.py` & `listpicker-0.3.1/src/listpicker/util.py`

 * *Files identical despite different names*

### Comparing `listpicker-0.3.0/LICENSE` & `listpicker-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `listpicker-0.3.0/README.md` & `listpicker-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `listpicker-0.3.0/pyproject.toml` & `listpicker-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "listpicker"
 description = "Interactive list selection and multiselect for POSIX terminals (non-curses)"
-version = "0.3.0"
+version = "0.3.1"
 authors = [
     {name = "Sung Pae", email = "self@sungpae.com"},
 ]
 readme = "README.md"
 license = {file = "LICENSE"}
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `listpicker-0.3.0/PKG-INFO` & `listpicker-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: listpicker
-Version: 0.3.0
+Version: 0.3.1
 Summary: Interactive list selection and multiselect for POSIX terminals (non-curses)
 Project-URL: Homepage, https://github.com/guns/python-listpicker
 Project-URL: Repository, https://github.com/guns/python-listpicker.git
 Author-email: Sung Pae <self@sungpae.com>
 License: The MIT License (MIT)
         
         Copyright © 2024 Sung Pae <self@sungpae.com>
```

