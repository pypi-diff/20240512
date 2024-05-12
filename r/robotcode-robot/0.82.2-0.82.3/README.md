# Comparing `tmp/robotcode_robot-0.82.2.tar.gz` & `tmp/robotcode_robot-0.82.3.tar.gz`

## Comparing `robotcode_robot-0.82.2.tar` & `robotcode_robot-0.82.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_robot-0.82.2/src/robotcode/robot/__init__.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_robot-0.82.2/src/robotcode/robot/__version__.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_robot-0.82.2/src/robotcode/robot/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_robot-0.82.2/src/robotcode/robot/config/__init__.py
--rw-r--r--   0        0        0     6077 2020-02-02 00:00:00.000000 robotcode_robot-0.82.2/src/robotcode/robot/config/loader.py
--rw-r--r--   0        0        0    88642 2020-02-02 00:00:00.000000 robotcode_robot-0.82.2/src/robotcode/robot/config/model.py
--rw-r--r--   0        0        0     2827 2020-02-02 00:00:00.000000 robotcode_robot-0.82.2/src/robotcode/robot/config/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_robot-0.82.2/src/robotcode/robot/diagnostics/__init__.py
--rw-r--r--   0        0        0    22292 2020-02-02 00:00:00.000000 robotcode_robot-0.82.2/src/robotcode/robot/diagnostics/document_cache_helper.py
--rw-r--r--   0        0        0    11110 2020-02-02 00:00:00.000000 robotcode_robot-0.82.2/src/robotcode/robot/diagnostics/entities.py
--rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 robotcode_robot-0.82.2/src/robotcode/robot/diagnostics/errors.py
--rw-r--r--   0        0        0    56251 2020-02-02 00:00:00.000000 robotcode_robot-0.82.2/src/robotcode/robot/diagnostics/imports_manager.py
--rw-r--r--   0        0        0    97124 2020-02-02 00:00:00.000000 robotcode_robot-0.82.2/src/robotcode/robot/diagnostics/library_doc.py
--rw-r--r--   0        0        0    30232 2020-02-02 00:00:00.000000 robotcode_robot-0.82.2/src/robotcode/robot/diagnostics/model_helper.py
--rw-r--r--   0        0        0    91315 2020-02-02 00:00:00.000000 robotcode_robot-0.82.2/src/robotcode/robot/diagnostics/namespace.py
--rw-r--r--   0        0        0    50937 2020-02-02 00:00:00.000000 robotcode_robot-0.82.2/src/robotcode/robot/diagnostics/namespace_analyzer.py
--rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 robotcode_robot-0.82.2/src/robotcode/robot/diagnostics/workspace_config.py
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 robotcode_robot-0.82.2/src/robotcode/robot/utils/__init__.py
--rw-r--r--   0        0        0    10193 2020-02-02 00:00:00.000000 robotcode_robot-0.82.2/src/robotcode/robot/utils/ast.py
--rw-r--r--   0        0        0    11621 2020-02-02 00:00:00.000000 robotcode_robot-0.82.2/src/robotcode/robot/utils/markdownformatter.py
--rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 robotcode_robot-0.82.2/src/robotcode/robot/utils/match.py
--rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 robotcode_robot-0.82.2/src/robotcode/robot/utils/robot_path.py
--rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 robotcode_robot-0.82.2/src/robotcode/robot/utils/stubs.py
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 robotcode_robot-0.82.2/src/robotcode/robot/utils/variables.py
--rw-r--r--   0        0        0     3241 2020-02-02 00:00:00.000000 robotcode_robot-0.82.2/src/robotcode/robot/utils/visitor.py
--rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_robot-0.82.2/.gitignore
--rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_robot-0.82.2/LICENSE.txt
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 robotcode_robot-0.82.2/README.md
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 robotcode_robot-0.82.2/pyproject.toml
--rw-r--r--   0        0        0     2240 2020-02-02 00:00:00.000000 robotcode_robot-0.82.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_robot-0.82.3/src/robotcode/robot/__init__.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_robot-0.82.3/src/robotcode/robot/__version__.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_robot-0.82.3/src/robotcode/robot/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_robot-0.82.3/src/robotcode/robot/config/__init__.py
+-rw-r--r--   0        0        0     6077 2020-02-02 00:00:00.000000 robotcode_robot-0.82.3/src/robotcode/robot/config/loader.py
+-rw-r--r--   0        0        0    88642 2020-02-02 00:00:00.000000 robotcode_robot-0.82.3/src/robotcode/robot/config/model.py
+-rw-r--r--   0        0        0     2827 2020-02-02 00:00:00.000000 robotcode_robot-0.82.3/src/robotcode/robot/config/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_robot-0.82.3/src/robotcode/robot/diagnostics/__init__.py
+-rw-r--r--   0        0        0    22292 2020-02-02 00:00:00.000000 robotcode_robot-0.82.3/src/robotcode/robot/diagnostics/document_cache_helper.py
+-rw-r--r--   0        0        0    11110 2020-02-02 00:00:00.000000 robotcode_robot-0.82.3/src/robotcode/robot/diagnostics/entities.py
+-rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 robotcode_robot-0.82.3/src/robotcode/robot/diagnostics/errors.py
+-rw-r--r--   0        0        0    56251 2020-02-02 00:00:00.000000 robotcode_robot-0.82.3/src/robotcode/robot/diagnostics/imports_manager.py
+-rw-r--r--   0        0        0    97124 2020-02-02 00:00:00.000000 robotcode_robot-0.82.3/src/robotcode/robot/diagnostics/library_doc.py
+-rw-r--r--   0        0        0    30232 2020-02-02 00:00:00.000000 robotcode_robot-0.82.3/src/robotcode/robot/diagnostics/model_helper.py
+-rw-r--r--   0        0        0    91311 2020-02-02 00:00:00.000000 robotcode_robot-0.82.3/src/robotcode/robot/diagnostics/namespace.py
+-rw-r--r--   0        0        0    50937 2020-02-02 00:00:00.000000 robotcode_robot-0.82.3/src/robotcode/robot/diagnostics/namespace_analyzer.py
+-rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 robotcode_robot-0.82.3/src/robotcode/robot/diagnostics/workspace_config.py
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 robotcode_robot-0.82.3/src/robotcode/robot/utils/__init__.py
+-rw-r--r--   0        0        0    10193 2020-02-02 00:00:00.000000 robotcode_robot-0.82.3/src/robotcode/robot/utils/ast.py
+-rw-r--r--   0        0        0    11621 2020-02-02 00:00:00.000000 robotcode_robot-0.82.3/src/robotcode/robot/utils/markdownformatter.py
+-rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 robotcode_robot-0.82.3/src/robotcode/robot/utils/match.py
+-rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 robotcode_robot-0.82.3/src/robotcode/robot/utils/robot_path.py
+-rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 robotcode_robot-0.82.3/src/robotcode/robot/utils/stubs.py
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 robotcode_robot-0.82.3/src/robotcode/robot/utils/variables.py
+-rw-r--r--   0        0        0     3241 2020-02-02 00:00:00.000000 robotcode_robot-0.82.3/src/robotcode/robot/utils/visitor.py
+-rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_robot-0.82.3/.gitignore
+-rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_robot-0.82.3/LICENSE.txt
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 robotcode_robot-0.82.3/README.md
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 robotcode_robot-0.82.3/pyproject.toml
+-rw-r--r--   0        0        0     2240 2020-02-02 00:00:00.000000 robotcode_robot-0.82.3/PKG-INFO
```

### Comparing `robotcode_robot-0.82.2/src/robotcode/robot/config/loader.py` & `robotcode_robot-0.82.3/src/robotcode/robot/config/loader.py`

 * *Files identical despite different names*

### Comparing `robotcode_robot-0.82.2/src/robotcode/robot/config/model.py` & `robotcode_robot-0.82.3/src/robotcode/robot/config/model.py`

 * *Files identical despite different names*

### Comparing `robotcode_robot-0.82.2/src/robotcode/robot/config/utils.py` & `robotcode_robot-0.82.3/src/robotcode/robot/config/utils.py`

 * *Files identical despite different names*

### Comparing `robotcode_robot-0.82.2/src/robotcode/robot/diagnostics/document_cache_helper.py` & `robotcode_robot-0.82.3/src/robotcode/robot/diagnostics/document_cache_helper.py`

 * *Files identical despite different names*

### Comparing `robotcode_robot-0.82.2/src/robotcode/robot/diagnostics/entities.py` & `robotcode_robot-0.82.3/src/robotcode/robot/diagnostics/entities.py`

 * *Files identical despite different names*

### Comparing `robotcode_robot-0.82.2/src/robotcode/robot/diagnostics/errors.py` & `robotcode_robot-0.82.3/src/robotcode/robot/diagnostics/errors.py`

 * *Files identical despite different names*

### Comparing `robotcode_robot-0.82.2/src/robotcode/robot/diagnostics/imports_manager.py` & `robotcode_robot-0.82.3/src/robotcode/robot/diagnostics/imports_manager.py`

 * *Files identical despite different names*

### Comparing `robotcode_robot-0.82.2/src/robotcode/robot/diagnostics/library_doc.py` & `robotcode_robot-0.82.3/src/robotcode/robot/diagnostics/library_doc.py`

 * *Files identical despite different names*

### Comparing `robotcode_robot-0.82.2/src/robotcode/robot/diagnostics/model_helper.py` & `robotcode_robot-0.82.3/src/robotcode/robot/diagnostics/model_helper.py`

 * *Files identical despite different names*

### Comparing `robotcode_robot-0.82.2/src/robotcode/robot/diagnostics/namespace.py` & `robotcode_robot-0.82.3/src/robotcode/robot/diagnostics/namespace.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     cast,
 )
 
 from robot.errors import VariableError
 from robot.libraries import STDLIBS
 from robot.parsing.lexer.tokens import Token
 from robot.parsing.model.blocks import Keyword, SettingSection, TestCase, VariableSection
-from robot.parsing.model.statements import Arguments, Fixture, Statement, Timeout
+from robot.parsing.model.statements import Arguments, Setup, Statement, Timeout
 from robot.parsing.model.statements import LibraryImport as RobotLibraryImport
 from robot.parsing.model.statements import ResourceImport as RobotResourceImport
 from robot.parsing.model.statements import (
     VariablesImport as RobotVariablesImport,
 )
 from robot.variables.search import (
     is_scalar_assign,
@@ -1035,15 +1035,15 @@
                     nodes if nodes else [],
                 )
             )
             test_or_keyword = test_or_keyword_nodes[0] if test_or_keyword_nodes else None
 
         in_args = isinstance(test_or_keyword_nodes[-1], Arguments) if test_or_keyword_nodes else False
         only_args = (
-            isinstance(test_or_keyword_nodes[-1], (Arguments, Fixture, Timeout)) if test_or_keyword_nodes else False
+            isinstance(test_or_keyword_nodes[-1], (Arguments, Setup, Timeout)) if test_or_keyword_nodes else False
         )
 
         for var in chain(
             *[
                 (
                     (
                         (OnlyArgumentsVisitor if only_args else BlockVariableVisitor)(
```

### Comparing `robotcode_robot-0.82.2/src/robotcode/robot/diagnostics/namespace_analyzer.py` & `robotcode_robot-0.82.3/src/robotcode/robot/diagnostics/namespace_analyzer.py`

 * *Files identical despite different names*

### Comparing `robotcode_robot-0.82.2/src/robotcode/robot/diagnostics/workspace_config.py` & `robotcode_robot-0.82.3/src/robotcode/robot/diagnostics/workspace_config.py`

 * *Files identical despite different names*

### Comparing `robotcode_robot-0.82.2/src/robotcode/robot/utils/ast.py` & `robotcode_robot-0.82.3/src/robotcode/robot/utils/ast.py`

 * *Files identical despite different names*

### Comparing `robotcode_robot-0.82.2/src/robotcode/robot/utils/markdownformatter.py` & `robotcode_robot-0.82.3/src/robotcode/robot/utils/markdownformatter.py`

 * *Files identical despite different names*

### Comparing `robotcode_robot-0.82.2/src/robotcode/robot/utils/match.py` & `robotcode_robot-0.82.3/src/robotcode/robot/utils/match.py`

 * *Files identical despite different names*

### Comparing `robotcode_robot-0.82.2/src/robotcode/robot/utils/robot_path.py` & `robotcode_robot-0.82.3/src/robotcode/robot/utils/robot_path.py`

 * *Files identical despite different names*

### Comparing `robotcode_robot-0.82.2/src/robotcode/robot/utils/stubs.py` & `robotcode_robot-0.82.3/src/robotcode/robot/utils/stubs.py`

 * *Files identical despite different names*

### Comparing `robotcode_robot-0.82.2/src/robotcode/robot/utils/variables.py` & `robotcode_robot-0.82.3/src/robotcode/robot/utils/variables.py`

 * *Files identical despite different names*

### Comparing `robotcode_robot-0.82.2/src/robotcode/robot/utils/visitor.py` & `robotcode_robot-0.82.3/src/robotcode/robot/utils/visitor.py`

 * *Files identical despite different names*

### Comparing `robotcode_robot-0.82.2/.gitignore` & `robotcode_robot-0.82.3/.gitignore`

 * *Files identical despite different names*

### Comparing `robotcode_robot-0.82.2/LICENSE.txt` & `robotcode_robot-0.82.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `robotcode_robot-0.82.2/README.md` & `robotcode_robot-0.82.3/README.md`

 * *Files identical despite different names*

### Comparing `robotcode_robot-0.82.2/pyproject.toml` & `robotcode_robot-0.82.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
   "Framework :: Robot Framework",
   "Framework :: Robot Framework :: Tool",
 ]
 dependencies = [
   "robotframework>=4.1.0",
   "tomli>=1.1.0; python_version < '3.11'",
   "platformdirs>=3.2.0,<4.2.0",
-  "robotcode-core==0.82.2",
+  "robotcode-core==0.82.3",
 ]
 dynamic = ["version"]
 
 [project.urls]
 Homepage = "https://robotcode.io"
 Donate = "https://opencollective.com/robotcode"
 Documentation = "https://github.com/robotcodedev/robotcode#readme"
```

### Comparing `robotcode_robot-0.82.2/PKG-INFO` & `robotcode_robot-0.82.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: robotcode-robot
-Version: 0.82.2
+Version: 0.82.3
 Summary: Support classes for RobotCode for handling Robot Framework projects.
 Project-URL: Homepage, https://robotcode.io
 Project-URL: Donate, https://opencollective.com/robotcode
 Project-URL: Documentation, https://github.com/robotcodedev/robotcode#readme
 Project-URL: Changelog, https://github.com/robotcodedev/robotcode/blob/main/CHANGELOG.md
 Project-URL: Issues, https://github.com/robotcodedev/robotcode/issues
 Project-URL: Source, https://github.com/robotcodedev/robotcode
@@ -22,15 +22,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Requires-Dist: platformdirs<4.2.0,>=3.2.0
-Requires-Dist: robotcode-core==0.82.2
+Requires-Dist: robotcode-core==0.82.3
 Requires-Dist: robotframework>=4.1.0
 Requires-Dist: tomli>=1.1.0; python_version < '3.11'
 Description-Content-Type: text/markdown
 
 # robotcode-robot
 
 [![PyPI - Version](https://img.shields.io/pypi/v/robotcode-robot.svg)](https://pypi.org/project/robotcode-robot)
```

