# Comparing `tmp/databricks_labs_blueprint-0.5.0.tar.gz` & `tmp/databricks_labs_blueprint-0.6.0.tar.gz`

## Comparing `databricks_labs_blueprint-0.5.0.tar` & `databricks_labs_blueprint-0.6.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.5.0/databricks/__init__.py
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.5.0/databricks/labs/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.5.0/databricks/labs/blueprint/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.5.0/databricks/labs/blueprint/__init__.py
--rw-r--r--   0        0        0     4078 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.5.0/databricks/labs/blueprint/__main__.py
--rw-r--r--   0        0        0     3723 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.5.0/databricks/labs/blueprint/cli.py
--rw-r--r--   0        0        0     8420 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.5.0/databricks/labs/blueprint/commands.py
--rw-r--r--   0        0        0     2723 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.5.0/databricks/labs/blueprint/entrypoint.py
--rw-r--r--   0        0        0    42934 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.5.0/databricks/labs/blueprint/installation.py
--rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.5.0/databricks/labs/blueprint/installer.py
--rw-r--r--   0        0        0     2764 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.5.0/databricks/labs/blueprint/limiter.py
--rw-r--r--   0        0        0     3292 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.5.0/databricks/labs/blueprint/logger.py
--rw-r--r--   0        0        0     6424 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.5.0/databricks/labs/blueprint/parallel.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.5.0/databricks/labs/blueprint/py.typed
--rw-r--r--   0        0        0     5590 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.5.0/databricks/labs/blueprint/tui.py
--rw-r--r--   0        0        0     6176 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.5.0/databricks/labs/blueprint/upgrades.py
--rw-r--r--   0        0        0    12749 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.5.0/databricks/labs/blueprint/wheels.py
--rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.5.0/.gitignore
--rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.5.0/LICENSE
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.5.0/NOTICE
--rw-r--r--   0        0        0    43925 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.5.0/README.md
--rw-r--r--   0        0        0    26290 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.5.0/pyproject.toml
--rw-r--r--   0        0        0    44728 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.0/databricks/__init__.py
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.0/databricks/labs/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.0/databricks/labs/blueprint/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.0/databricks/labs/blueprint/__init__.py
+-rw-r--r--   0        0        0     4078 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.0/databricks/labs/blueprint/__main__.py
+-rw-r--r--   0        0        0     3723 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.0/databricks/labs/blueprint/cli.py
+-rw-r--r--   0        0        0     8420 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.0/databricks/labs/blueprint/commands.py
+-rw-r--r--   0        0        0     2723 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.0/databricks/labs/blueprint/entrypoint.py
+-rw-r--r--   0        0        0    42934 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.0/databricks/labs/blueprint/installation.py
+-rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.0/databricks/labs/blueprint/installer.py
+-rw-r--r--   0        0        0     2764 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.0/databricks/labs/blueprint/limiter.py
+-rw-r--r--   0        0        0     3292 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.0/databricks/labs/blueprint/logger.py
+-rw-r--r--   0        0        0     6424 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.0/databricks/labs/blueprint/parallel.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.0/databricks/labs/blueprint/py.typed
+-rw-r--r--   0        0        0     5590 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.0/databricks/labs/blueprint/tui.py
+-rw-r--r--   0        0        0     6176 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.0/databricks/labs/blueprint/upgrades.py
+-rw-r--r--   0        0        0    14208 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.0/databricks/labs/blueprint/wheels.py
+-rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.0/.gitignore
+-rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.0/LICENSE
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.0/NOTICE
+-rw-r--r--   0        0        0    45992 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.0/README.md
+-rw-r--r--   0        0        0    26290 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0    46795 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.0/PKG-INFO
```

### Comparing `databricks_labs_blueprint-0.5.0/databricks/labs/blueprint/__main__.py` & `databricks_labs_blueprint-0.6.0/databricks/labs/blueprint/__main__.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_blueprint-0.5.0/databricks/labs/blueprint/cli.py` & `databricks_labs_blueprint-0.6.0/databricks/labs/blueprint/cli.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_blueprint-0.5.0/databricks/labs/blueprint/commands.py` & `databricks_labs_blueprint-0.6.0/databricks/labs/blueprint/commands.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_blueprint-0.5.0/databricks/labs/blueprint/entrypoint.py` & `databricks_labs_blueprint-0.6.0/databricks/labs/blueprint/entrypoint.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_blueprint-0.5.0/databricks/labs/blueprint/installation.py` & `databricks_labs_blueprint-0.6.0/databricks/labs/blueprint/installation.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_blueprint-0.5.0/databricks/labs/blueprint/installer.py` & `databricks_labs_blueprint-0.6.0/databricks/labs/blueprint/installer.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_blueprint-0.5.0/databricks/labs/blueprint/limiter.py` & `databricks_labs_blueprint-0.6.0/databricks/labs/blueprint/limiter.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_blueprint-0.5.0/databricks/labs/blueprint/logger.py` & `databricks_labs_blueprint-0.6.0/databricks/labs/blueprint/logger.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_blueprint-0.5.0/databricks/labs/blueprint/parallel.py` & `databricks_labs_blueprint-0.6.0/databricks/labs/blueprint/parallel.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_blueprint-0.5.0/databricks/labs/blueprint/tui.py` & `databricks_labs_blueprint-0.6.0/databricks/labs/blueprint/tui.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_blueprint-0.5.0/databricks/labs/blueprint/upgrades.py` & `databricks_labs_blueprint-0.6.0/databricks/labs/blueprint/upgrades.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_blueprint-0.5.0/databricks/labs/blueprint/wheels.py` & `databricks_labs_blueprint-0.6.0/databricks/labs/blueprint/wheels.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import sys
 import tempfile
 import warnings
 from collections.abc import Iterable
 from contextlib import AbstractContextManager
 from dataclasses import dataclass
 from datetime import datetime, timezone
+from functools import cached_property
 from pathlib import Path
 
 from databricks.sdk import WorkspaceClient
 from databricks.sdk.mixins.compute import SemVer
 
 from databricks.labs.blueprint.entrypoint import find_project_root
 from databricks.labs.blueprint.installation import Installation
@@ -225,85 +226,111 @@
         with self._local_wheel.open("rb") as f:
             return self._installation.upload_dbfs(f"wheels/{self._local_wheel.name}", f)
 
     def upload_to_wsfs(self) -> str:
         """Uploads the wheel to WSFS location of installation and returns the remote path."""
         with self._local_wheel.open("rb") as f:
             remote_wheel = self._installation.upload(f"wheels/{self._local_wheel.name}", f.read())
-            self._installation.save(Version(self._product_info.version(), remote_wheel, self._now_iso()))
+            self._installation.save(Version(self._current_version, remote_wheel, self._now_iso()))
             return remote_wheel
 
+    def upload_wheel_dependencies(self, prefixes: list[str]) -> list[str]:
+        """Uploads the wheel dependencies to WSFS location of installation and returns the remote paths.
+        :param prefixes : A list of prefixes to match against the wheel names. If a prefix matches, the wheel is uploaded.
+        """
+        remote_paths = []
+        for wheel in self._build_wheel(self._tmp_dir.name, verbose=self._verbose, no_deps=False, dirs_exist_ok=True):
+            if not wheel.name.endswith("-none-any.whl"):
+                continue
+            # main wheel is uploaded with upload_to_wsfs() method.
+            if wheel.name == self._local_wheel.name:
+                continue
+            for prefix in prefixes:
+                if not wheel.name.startswith(prefix):
+                    continue
+                remote_wheel = self._installation.upload(f"wheels/{wheel.name}", wheel.read_bytes())
+                remote_paths.append(remote_wheel)
+        return remote_paths
+
+    @cached_property
+    def _current_version(self):
+        # addresses double-uploaded bug for unreleased versions uploaded to airgapped workspaces
+        return self._product_info.version()
+
     @staticmethod
     def _now_iso():
         """Returns the current time in ISO format."""
         return datetime.now(timezone.utc).isoformat()
 
     def __enter__(self) -> "WheelsV2":
         """Builds the wheel and returns the instance. Use it as a context manager."""
         self._tmp_dir = tempfile.TemporaryDirectory()
-        self._local_wheel = self._build_wheel(self._tmp_dir.name, verbose=self._verbose)
+        self._local_wheel = next(self._build_wheel(self._tmp_dir.name, verbose=self._verbose, no_deps=True))
         return self
 
     def __exit__(self, __exc_type, __exc_value, __traceback):
         """Cleans up the temporary directory. Use it as a context manager."""
         self._tmp_dir.cleanup()
 
-    def _build_wheel(self, tmp_dir: str, *, verbose: bool = False):
+    def _build_wheel(self, tmp_dir: str, *, verbose: bool = False, no_deps: bool = True, dirs_exist_ok: bool = False):
         """Helper to build the wheel package
 
         :param tmp_dir: str:
         :param *:
         :param verbose: bool:  (Default value = False)
-
+        :param no_deps: bool:  (Default value = True)
+        :param dirs_exist_ok: bool:  (Default value = False)
         """
         stdout = subprocess.STDOUT
         stderr = subprocess.STDOUT
         if not verbose:
             stdout = subprocess.DEVNULL
             stderr = subprocess.DEVNULL
         checkout_root = self._product_info.checkout_root()
         if self._product_info.is_git_checkout() and self._product_info.is_unreleased_version():
             # working copy becomes project root for building a wheel
-            checkout_root = self._copy_root_to(tmp_dir)
+            checkout_root = self._copy_root_to(tmp_dir, dirs_exist_ok)
             # and override the version file
             self._override_version_to_unreleased(checkout_root)
+        args = [sys.executable, "-m", "pip", "wheel", "--wheel-dir", tmp_dir, checkout_root.as_posix()]
         logger.debug(f"Building wheel for {checkout_root} in {tmp_dir}")
+        if no_deps:
+            args.append("--no-deps")
         subprocess.run(
-            [sys.executable, "-m", "pip", "wheel", "--no-deps", "--wheel-dir", tmp_dir, checkout_root.as_posix()],
+            args,
             check=True,
             stdout=stdout,
             stderr=stderr,
         )
-        # get wheel name as first file in the temp directory
-        return next(Path(tmp_dir).glob("*.whl"))
+        return Path(tmp_dir).glob("*.whl")
 
     def _override_version_to_unreleased(self, tmp_dir_path: Path):
         """Overrides the version file to unreleased version."""
         checkout_root = self._product_info.checkout_root()
         relative_version_file = self._product_info.version_file().relative_to(checkout_root)
         version_file = tmp_dir_path / relative_version_file
         with version_file.open("w") as f:
-            f.write(f'__version__ = "{self._product_info.version()}"')
+            f.write(f'__version__ = "{self._current_version}"')
 
-    def _copy_root_to(self, tmp_dir: str | Path):
+    def _copy_root_to(self, tmp_dir: str | Path, dirs_exist_ok: bool = False):
         """Copies the root to a temporary directory."""
         checkout_root = self._product_info.checkout_root()
         tmp_dir_path = Path(tmp_dir) / "working-copy"
 
         # copy everything to a temporary directory
         def copy_ignore(_, names: list[str]):
             # callable(src, names) -> ignored_names
             ignored_names = []
             for name in names:
                 if name not in IGNORE_DIR_NAMES:
                     continue
                 ignored_names.append(name)
             return ignored_names
 
-        shutil.copytree(checkout_root, tmp_dir_path, ignore=copy_ignore)
+        shutil.copytree(checkout_root, tmp_dir_path, ignore=copy_ignore, dirs_exist_ok=dirs_exist_ok)
         return tmp_dir_path
 
 
 class Wheels(WheelsV2):
     """Wheel builder"""
 
     def __init__(
```

### Comparing `databricks_labs_blueprint-0.5.0/.gitignore` & `databricks_labs_blueprint-0.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `databricks_labs_blueprint-0.5.0/LICENSE` & `databricks_labs_blueprint-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `databricks_labs_blueprint-0.5.0/README.md` & `databricks_labs_blueprint-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,28 @@
+Metadata-Version: 2.3
+Name: databricks-labs-blueprint
+Version: 0.6.0
+Summary: Common libraries for Databricks Labs
+Project-URL: Issues, https://github.com/databrickslabs/blueprint/issues
+Project-URL: Source, https://github.com/databrickslabs/blueprint
+License-File: LICENSE
+License-File: NOTICE
+Keywords: Databricks
+Classifier: Development Status :: 3 - Alpha
+Classifier: License :: Other/Proprietary License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Requires-Python: >=3.10
+Requires-Dist: databricks-sdk>=0.16.0
+Provides-Extra: yaml
+Requires-Dist: pyyaml<7.0.0,>=6.0.0; extra == 'yaml'
+Description-Content-Type: text/markdown
+
 <!-- FOR CONTRIBUTORS: Edit this file in Visual Studio Code with the recommended extensions, so that we update the table of contents automatically -->
 Databricks Labs Blueprint
 ===
 
 [![python](https://img.shields.io/badge/python-3.10,%203.11,%203.12-green)](https://github.com/databrickslabs/blueprint/actions/workflows/push.yml)
 [![codecov](https://codecov.io/github/databrickslabs/blueprint/graph/badge.svg?token=x1JSVddfZa)](https://codecov.io/github/databrickslabs/blueprint) [![lines of code](https://tokei.rs/b1/github/databrickslabs/blueprint)]([https://codecov.io/github/databrickslabs/blueprint](https://github.com/databrickslabs/blueprint))
 
@@ -19,39 +40,40 @@
     * [Single Choice from Dictionary](#single-choice-from-dictionary)
     * [Multiple Choices from Dictionary](#multiple-choices-from-dictionary)
     * [Unit Testing Prompts](#unit-testing-prompts)
   * [Nicer Logging Formatter](#nicer-logging-formatter)
     * [Rendering on Dark Background](#rendering-on-dark-background)
     * [Rendering in Databricks Notebooks](#rendering-in-databricks-notebooks)
     * [Integration With Your App](#integration-with-your-app)
-    * [Integration with `console_script` Entrypoints](#integration-with-consolescript-entrypoints)
+    * [Integration with `console_script` Entrypoints](#integration-with-console_script-entrypoints)
   * [Parallel Task Execution](#parallel-task-execution)
     * [Collecting Results](#collecting-results)
     * [Collecting Errors from Background Tasks](#collecting-errors-from-background-tasks)
     * [Strict Failures from Background Tasks](#strict-failures-from-background-tasks)
   * [Application and Installation State](#application-and-installation-state)
     * [Install Folder](#install-folder)
     * [Detecting Current Installation](#detecting-current-installation)
     * [Detecting Installations From All Users](#detecting-installations-from-all-users)
     * [Saving `@dataclass` configuration](#saving-dataclass-configuration)
     * [Saving CSV files](#saving-csv-files)
     * [Loading `@dataclass` configuration](#loading-dataclass-configuration)
-    * [Brute-forcing `SerdeError` with `as_dict()` and `from_dict()`](#brute-forcing-serdeerror-with-asdict-and-fromdict)
+    * [Brute-forcing `SerdeError` with `as_dict()` and `from_dict()`](#brute-forcing-serdeerror-with-as_dict-and-from_dict)
     * [Configuration Format Evolution](#configuration-format-evolution)
     * [Uploading Untyped Files](#uploading-untyped-files)
     * [Listing All Files in the Install Folder](#listing-all-files-in-the-install-folder)
     * [Unit Testing Installation State](#unit-testing-installation-state)
     * [Assert Rewriting with PyTest](#assert-rewriting-with-pytest)
   * [Application State Migrations](#application-state-migrations)
   * [Building Wheels](#building-wheels)
     * [Released Version Detection](#released-version-detection)
     * [Unreleased Version Detection](#unreleased-version-detection)
     * [Application Name Detection](#application-name-detection)
     * [Using `ProductInfo` with integration tests](#using-productinfo-with-integration-tests)
     * [Publishing Wheels to Databricks Workspace](#publishing-wheels-to-databricks-workspace)
+    * [Publishing upstream dependencies to workspaces without Public Internet access](#publishing-upstream-dependencies-to-workspaces-without-public-internet-access)
   * [Databricks CLI's `databricks labs ...` Router](#databricks-clis-databricks-labs--router)
     * [Account-level Commands](#account-level-commands)
     * [Commands with interactive prompts](#commands-with-interactive-prompts)
     * [Integration with Databricks Connect](#integration-with-databricks-connect)
     * [Starting New Projects](#starting-new-projects)
 * [Notable Downstream Projects](#notable-downstream-projects)
 * [Project Support](#project-support)
@@ -929,14 +951,41 @@
 
 ```
 15:08:44  INFO [dist.logger] Uploaded to /Users/serge.smertin@databricks.com/.blueprint/wheels/databricks_labs_blueprint-0.0.2+120240105150840-py3-none-any.whl
 ```
 
 You can also do `wheels.upload_to_dbfs()`, though you're not able to set any access control over it.
 
+### Publishing upstream dependencies to workspaces without Public Internet access
+
+Python wheel may have dependencies that are not included in the wheel itself. These dependencies are usually other Python packages that your wheel relies on. During installation on regular Databricks Workspaces, these dependencies get automatically fetched from [Python Package Index](https://pypi.org/). 
+
+Some Databricks Workspaces are configured with extra layers of network security, that block all access to Public Internet, including [Python Package Index](https://pypi.org/). To ensure installations working on these kinds of workspaces, developers need to explicitly upload all upstream dependencies for their applications to work correctly.
+
+The `upload_wheel_dependencies(prefixes)` method can be used to upload these dependencies to Databricks Workspace. This method takes a list of prefixes as an argument. It will upload all the dependencies of the wheel that have names starting with any of the provided prefixes.
+
+Here is an example of how you can use this method:
+
+```python
+from databricks.sdk import WorkspaceClient
+from databricks.labs.blueprint.wheels import ProductInfo
+
+ws = WorkspaceClient()
+product_info = ProductInfo(__file__)
+installation = product_info.current_installation(ws)
+
+with product_info.wheels(ws) as wheels:
+    wheel_paths = wheels.upload_wheel_dependencies(['databricks_sdk', 'pandas'])
+    for path in wheel_paths:
+        print(f'Uploaded dependency to {path}')
+```
+
+In this example, the `upload_wheel_dependencies(['databricks_sdk', 'pandas'])` call will upload all the dependencies of the wheel that have names starting with 'databricks_sdk' or 'pandas'. This method excludes any platform specific dependencies (i.e. ending with `-none-any.whl`). Also the main wheel file is not uploaded. The method returns a list of paths to the uploaded dependencies on WorkspaceFS.
+
+
 [[back to top](#databricks-labs-blueprint)]
 
 ## Databricks CLI's `databricks labs ...` Router
 
 This library contains common utilities for Databricks CLI entrypoints defined in [`labs.yml`](labs.yml) file. Here's the example metadata for a tool named `blueprint` with a single `me` command and flag named `--greeting`, that has `Hello` as default value:
 
 ```yaml
```

### Comparing `databricks_labs_blueprint-0.5.0/pyproject.toml` & `databricks_labs_blueprint-0.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `databricks_labs_blueprint-0.5.0/PKG-INFO` & `databricks_labs_blueprint-0.6.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,7 @@
-Metadata-Version: 2.3
-Name: databricks-labs-blueprint
-Version: 0.5.0
-Summary: Common libraries for Databricks Labs
-Project-URL: Issues, https://github.com/databrickslabs/blueprint/issues
-Project-URL: Source, https://github.com/databrickslabs/blueprint
-License-File: LICENSE
-License-File: NOTICE
-Keywords: Databricks
-Classifier: Development Status :: 3 - Alpha
-Classifier: License :: Other/Proprietary License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Requires-Python: >=3.10
-Requires-Dist: databricks-sdk>=0.16.0
-Provides-Extra: yaml
-Requires-Dist: pyyaml<7.0.0,>=6.0.0; extra == 'yaml'
-Description-Content-Type: text/markdown
-
 <!-- FOR CONTRIBUTORS: Edit this file in Visual Studio Code with the recommended extensions, so that we update the table of contents automatically -->
 Databricks Labs Blueprint
 ===
 
 [![python](https://img.shields.io/badge/python-3.10,%203.11,%203.12-green)](https://github.com/databrickslabs/blueprint/actions/workflows/push.yml)
 [![codecov](https://codecov.io/github/databrickslabs/blueprint/graph/badge.svg?token=x1JSVddfZa)](https://codecov.io/github/databrickslabs/blueprint) [![lines of code](https://tokei.rs/b1/github/databrickslabs/blueprint)]([https://codecov.io/github/databrickslabs/blueprint](https://github.com/databrickslabs/blueprint))
 
@@ -40,39 +19,40 @@
     * [Single Choice from Dictionary](#single-choice-from-dictionary)
     * [Multiple Choices from Dictionary](#multiple-choices-from-dictionary)
     * [Unit Testing Prompts](#unit-testing-prompts)
   * [Nicer Logging Formatter](#nicer-logging-formatter)
     * [Rendering on Dark Background](#rendering-on-dark-background)
     * [Rendering in Databricks Notebooks](#rendering-in-databricks-notebooks)
     * [Integration With Your App](#integration-with-your-app)
-    * [Integration with `console_script` Entrypoints](#integration-with-consolescript-entrypoints)
+    * [Integration with `console_script` Entrypoints](#integration-with-console_script-entrypoints)
   * [Parallel Task Execution](#parallel-task-execution)
     * [Collecting Results](#collecting-results)
     * [Collecting Errors from Background Tasks](#collecting-errors-from-background-tasks)
     * [Strict Failures from Background Tasks](#strict-failures-from-background-tasks)
   * [Application and Installation State](#application-and-installation-state)
     * [Install Folder](#install-folder)
     * [Detecting Current Installation](#detecting-current-installation)
     * [Detecting Installations From All Users](#detecting-installations-from-all-users)
     * [Saving `@dataclass` configuration](#saving-dataclass-configuration)
     * [Saving CSV files](#saving-csv-files)
     * [Loading `@dataclass` configuration](#loading-dataclass-configuration)
-    * [Brute-forcing `SerdeError` with `as_dict()` and `from_dict()`](#brute-forcing-serdeerror-with-asdict-and-fromdict)
+    * [Brute-forcing `SerdeError` with `as_dict()` and `from_dict()`](#brute-forcing-serdeerror-with-as_dict-and-from_dict)
     * [Configuration Format Evolution](#configuration-format-evolution)
     * [Uploading Untyped Files](#uploading-untyped-files)
     * [Listing All Files in the Install Folder](#listing-all-files-in-the-install-folder)
     * [Unit Testing Installation State](#unit-testing-installation-state)
     * [Assert Rewriting with PyTest](#assert-rewriting-with-pytest)
   * [Application State Migrations](#application-state-migrations)
   * [Building Wheels](#building-wheels)
     * [Released Version Detection](#released-version-detection)
     * [Unreleased Version Detection](#unreleased-version-detection)
     * [Application Name Detection](#application-name-detection)
     * [Using `ProductInfo` with integration tests](#using-productinfo-with-integration-tests)
     * [Publishing Wheels to Databricks Workspace](#publishing-wheels-to-databricks-workspace)
+    * [Publishing upstream dependencies to workspaces without Public Internet access](#publishing-upstream-dependencies-to-workspaces-without-public-internet-access)
   * [Databricks CLI's `databricks labs ...` Router](#databricks-clis-databricks-labs--router)
     * [Account-level Commands](#account-level-commands)
     * [Commands with interactive prompts](#commands-with-interactive-prompts)
     * [Integration with Databricks Connect](#integration-with-databricks-connect)
     * [Starting New Projects](#starting-new-projects)
 * [Notable Downstream Projects](#notable-downstream-projects)
 * [Project Support](#project-support)
@@ -950,14 +930,41 @@
 
 ```
 15:08:44  INFO [dist.logger] Uploaded to /Users/serge.smertin@databricks.com/.blueprint/wheels/databricks_labs_blueprint-0.0.2+120240105150840-py3-none-any.whl
 ```
 
 You can also do `wheels.upload_to_dbfs()`, though you're not able to set any access control over it.
 
+### Publishing upstream dependencies to workspaces without Public Internet access
+
+Python wheel may have dependencies that are not included in the wheel itself. These dependencies are usually other Python packages that your wheel relies on. During installation on regular Databricks Workspaces, these dependencies get automatically fetched from [Python Package Index](https://pypi.org/). 
+
+Some Databricks Workspaces are configured with extra layers of network security, that block all access to Public Internet, including [Python Package Index](https://pypi.org/). To ensure installations working on these kinds of workspaces, developers need to explicitly upload all upstream dependencies for their applications to work correctly.
+
+The `upload_wheel_dependencies(prefixes)` method can be used to upload these dependencies to Databricks Workspace. This method takes a list of prefixes as an argument. It will upload all the dependencies of the wheel that have names starting with any of the provided prefixes.
+
+Here is an example of how you can use this method:
+
+```python
+from databricks.sdk import WorkspaceClient
+from databricks.labs.blueprint.wheels import ProductInfo
+
+ws = WorkspaceClient()
+product_info = ProductInfo(__file__)
+installation = product_info.current_installation(ws)
+
+with product_info.wheels(ws) as wheels:
+    wheel_paths = wheels.upload_wheel_dependencies(['databricks_sdk', 'pandas'])
+    for path in wheel_paths:
+        print(f'Uploaded dependency to {path}')
+```
+
+In this example, the `upload_wheel_dependencies(['databricks_sdk', 'pandas'])` call will upload all the dependencies of the wheel that have names starting with 'databricks_sdk' or 'pandas'. This method excludes any platform specific dependencies (i.e. ending with `-none-any.whl`). Also the main wheel file is not uploaded. The method returns a list of paths to the uploaded dependencies on WorkspaceFS.
+
+
 [[back to top](#databricks-labs-blueprint)]
 
 ## Databricks CLI's `databricks labs ...` Router
 
 This library contains common utilities for Databricks CLI entrypoints defined in [`labs.yml`](labs.yml) file. Here's the example metadata for a tool named `blueprint` with a single `me` command and flag named `--greeting`, that has `Hello` as default value:
 
 ```yaml
```

