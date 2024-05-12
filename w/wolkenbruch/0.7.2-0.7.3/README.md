# Comparing `tmp/wolkenbruch-0.7.2.tar.gz` & `tmp/wolkenbruch-0.7.3.tar.gz`

## Comparing `wolkenbruch-0.7.2.tar` & `wolkenbruch-0.7.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 wolkenbruch-0.7.2/.flake8
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 wolkenbruch-0.7.2/.pylintrc
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 wolkenbruch-0.7.2/CHANGELOG.md
--rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 wolkenbruch-0.7.2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 wolkenbruch-0.7.2/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 wolkenbruch-0.7.2/.github/workflows/build.yml
--rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 wolkenbruch-0.7.2/.github/workflows/lint.yml
--rw-r--r--   0        0        0     2181 2020-02-02 00:00:00.000000 wolkenbruch-0.7.2/.github/workflows/release.yml
--rw-r--r--   0        0        0     2817 2020-02-02 00:00:00.000000 wolkenbruch-0.7.2/extra/img/wolkenbruch.svg
--rw-r--r--   0        0        0     2397 2020-02-02 00:00:00.000000 wolkenbruch-0.7.2/extra/img/wolkenbruch_256x160.svg
--rw-r--r--   0        0        0     2621 2020-02-02 00:00:00.000000 wolkenbruch-0.7.2/extra/img/wolkenbruch_bw_256x256.svg
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 wolkenbruch-0.7.2/extra/systemd/wolkenbruch.service
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 wolkenbruch-0.7.2/extra/systemd/wolkenbruch.timer
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 wolkenbruch-0.7.2/src/wolkenbruch/__init__.py
--rw-r--r--   0        0        0     1151 2020-02-02 00:00:00.000000 wolkenbruch-0.7.2/src/wolkenbruch/__main__.py
--rw-r--r--   0        0        0     4035 2020-02-02 00:00:00.000000 wolkenbruch-0.7.2/src/wolkenbruch/config.py
--rw-r--r--   0        0        0     3039 2020-02-02 00:00:00.000000 wolkenbruch-0.7.2/src/wolkenbruch/emailsender.py
--rw-r--r--   0        0        0     2869 2020-02-02 00:00:00.000000 wolkenbruch-0.7.2/src/wolkenbruch/precipitationchecker.py
--rw-r--r--   0        0        0     3074 2020-02-02 00:00:00.000000 wolkenbruch-0.7.2/src/wolkenbruch/wolkenbruch.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 wolkenbruch-0.7.2/src/wolkenbruch/wolkenbruch.yml.template
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 wolkenbruch-0.7.2/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 wolkenbruch-0.7.2/LICENSE
--rw-r--r--   0        0        0     4379 2020-02-02 00:00:00.000000 wolkenbruch-0.7.2/README.md
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 wolkenbruch-0.7.2/pyproject.toml
--rw-r--r--   0        0        0     5264 2020-02-02 00:00:00.000000 wolkenbruch-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 wolkenbruch-0.7.3/.flake8
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 wolkenbruch-0.7.3/.pylintrc
+-rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 wolkenbruch-0.7.3/CHANGELOG.md
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 wolkenbruch-0.7.3/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 wolkenbruch-0.7.3/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 wolkenbruch-0.7.3/.github/workflows/build.yml
+-rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 wolkenbruch-0.7.3/.github/workflows/lint.yml
+-rw-r--r--   0        0        0     2181 2020-02-02 00:00:00.000000 wolkenbruch-0.7.3/.github/workflows/release.yml
+-rw-r--r--   0        0        0     2817 2020-02-02 00:00:00.000000 wolkenbruch-0.7.3/extra/img/wolkenbruch.svg
+-rw-r--r--   0        0        0     2397 2020-02-02 00:00:00.000000 wolkenbruch-0.7.3/extra/img/wolkenbruch_256x160.svg
+-rw-r--r--   0        0        0     2621 2020-02-02 00:00:00.000000 wolkenbruch-0.7.3/extra/img/wolkenbruch_bw_256x256.svg
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 wolkenbruch-0.7.3/extra/systemd/wolkenbruch.service
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 wolkenbruch-0.7.3/extra/systemd/wolkenbruch.timer
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 wolkenbruch-0.7.3/src/wolkenbruch/__init__.py
+-rw-r--r--   0        0        0     1151 2020-02-02 00:00:00.000000 wolkenbruch-0.7.3/src/wolkenbruch/__main__.py
+-rw-r--r--   0        0        0     4035 2020-02-02 00:00:00.000000 wolkenbruch-0.7.3/src/wolkenbruch/config.py
+-rw-r--r--   0        0        0     3039 2020-02-02 00:00:00.000000 wolkenbruch-0.7.3/src/wolkenbruch/emailsender.py
+-rw-r--r--   0        0        0     2869 2020-02-02 00:00:00.000000 wolkenbruch-0.7.3/src/wolkenbruch/precipitationchecker.py
+-rw-r--r--   0        0        0     4538 2020-02-02 00:00:00.000000 wolkenbruch-0.7.3/src/wolkenbruch/wolkenbruch.py
+-rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 wolkenbruch-0.7.3/src/wolkenbruch/wolkenbruch.yml.template
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 wolkenbruch-0.7.3/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 wolkenbruch-0.7.3/LICENSE
+-rw-r--r--   0        0        0     4366 2020-02-02 00:00:00.000000 wolkenbruch-0.7.3/README.md
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 wolkenbruch-0.7.3/pyproject.toml
+-rw-r--r--   0        0        0     5281 2020-02-02 00:00:00.000000 wolkenbruch-0.7.3/PKG-INFO
```

### Comparing `wolkenbruch-0.7.2/CHANGELOG.md` & `wolkenbruch-0.7.3/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+- **0.7.3** (2024-05-12):
+    - fix configuration file handling
+
 - **0.7.2** (2024-05-06):
     - fix broken local imports
 
 - **0.7.1** (2024-05-06):
     - migrate source repository and build toolchain to GitHub
 
 - **0.7.0** (2024-05-06):
```

### Comparing `wolkenbruch-0.7.2/.github/ISSUE_TEMPLATE/bug_report.md` & `wolkenbruch-0.7.3/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `wolkenbruch-0.7.2/.github/ISSUE_TEMPLATE/feature_request.md` & `wolkenbruch-0.7.3/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `wolkenbruch-0.7.2/.github/workflows/build.yml` & `wolkenbruch-0.7.3/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `wolkenbruch-0.7.2/.github/workflows/release.yml` & `wolkenbruch-0.7.3/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `wolkenbruch-0.7.2/extra/img/wolkenbruch.svg` & `wolkenbruch-0.7.3/extra/img/wolkenbruch.svg`

 * *Files identical despite different names*

### Comparing `wolkenbruch-0.7.2/extra/img/wolkenbruch_256x160.svg` & `wolkenbruch-0.7.3/extra/img/wolkenbruch_256x160.svg`

 * *Files identical despite different names*

### Comparing `wolkenbruch-0.7.2/extra/img/wolkenbruch_bw_256x256.svg` & `wolkenbruch-0.7.3/extra/img/wolkenbruch_bw_256x256.svg`

 * *Files identical despite different names*

### Comparing `wolkenbruch-0.7.2/src/wolkenbruch/__init__.py` & `wolkenbruch-0.7.3/src/wolkenbruch/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,8 +28,8 @@
     "remind_me_if_it_rains",
 ]
 
 
 from .wolkenbruch import remind_me_if_it_rains
 
 
-__version__ = "0.7.2"
+__version__ = "0.7.3"
```

### Comparing `wolkenbruch-0.7.2/src/wolkenbruch/__main__.py` & `wolkenbruch-0.7.3/src/wolkenbruch/__main__.py`

 * *Files identical despite different names*

### Comparing `wolkenbruch-0.7.2/src/wolkenbruch/config.py` & `wolkenbruch-0.7.3/src/wolkenbruch/config.py`

 * *Files identical despite different names*

### Comparing `wolkenbruch-0.7.2/src/wolkenbruch/emailsender.py` & `wolkenbruch-0.7.3/src/wolkenbruch/emailsender.py`

 * *Files identical despite different names*

### Comparing `wolkenbruch-0.7.2/src/wolkenbruch/precipitationchecker.py` & `wolkenbruch-0.7.3/src/wolkenbruch/precipitationchecker.py`

 * *Files identical despite different names*

### Comparing `wolkenbruch-0.7.2/LICENSE` & `wolkenbruch-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `wolkenbruch-0.7.2/README.md` & `wolkenbruch-0.7.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -66,26 +66,27 @@
 - The verbose flag toggles whether `wolkenbruch` prints a status or operated
   silently.
 
 ```yaml
 # example configuration file
 # (/etc/wolkenbruch.yml, ~/.config/wolkenbruch.yml,
 #    %APPDATA%/wolkenbruch.yml, ${XDG_CONFIG_HOME}/wolkenbruch.yml)
-smtp:
-    host:     localhost:587
-    user:     foobar
-    password: BARFOO
-email:
-    from:     me@whereever.com
-    to:       myself@whereever.com
-    subject:  Pack your rain gear!
-    message:  The forecast precipitation rate for today is {a:.2f} mm/h, maximum {m:2f} mm/h.
 place: Helsinki
 average_precipitation_rate_threshold: 0.1
 max_precipitation_rate_threshold: 0.5
+
+email-to: myself@whereever.com
+email-from: me@whereever.com
+email-subject: Pack your rain gear!
+email-message: The average forecast precipitation rate for today is {a:0.2f}, maximum {m:0.2f} mm/h.
+
+smtp-host: localhost:587
+smtp-user: foobar
+smtp-password: BARFOO
+
 verbose: False
 ```
 
 ### Usage
 
 Run `wolkenbruch` to check the precipitation for the next 14 hours and send you
 an e-mail reminder. Ideally, set up a cron job or a systemd timer to run
```

### Comparing `wolkenbruch-0.7.2/pyproject.toml` & `wolkenbruch-0.7.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 readme = "README.md"
 
 authors = [
     { name = "Christoph Fink", email = "christoph.fink@gmail.com" }
 ]
 
 dependencies = [
+    "ConfigArgParse",
     "geocoder",
     "importlib_resources",
     "PyYAML",
     "requests"
 ]
 requires-python = ">=3.9"
```

### Comparing `wolkenbruch-0.7.2/PKG-INFO` & `wolkenbruch-0.7.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.3
 Name: wolkenbruch
-Version: 0.7.2
+Version: 0.7.3
 Summary: Send an e-mail reminder if precipitation is forecast
 Project-URL: Documentation, https://github.com/christophfink/wolkenbruch/
 Project-URL: Repository, https://github.com/christophfink/wolkenbruch/
 Project-URL: Change log, https://github.com/christophfink/wolkenbruch/blob/main/CHANGELOG.md
 Project-URL: Bug tracker, https://github.com/christophfink/wolkenbruch/issues
 Author-email: Christoph Fink <christoph.fink@gmail.com>
 License: GPL-3.0-or-later or MIT
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
+Requires-Dist: configargparse
 Requires-Dist: geocoder
 Requires-Dist: importlib-resources
 Requires-Dist: pyyaml
 Requires-Dist: requests
 Description-Content-Type: text/markdown
 
 ![rain cloud](extra/img/wolkenbruch_256x160.svg)
@@ -87,26 +88,27 @@
 - The verbose flag toggles whether `wolkenbruch` prints a status or operated
   silently.
 
 ```yaml
 # example configuration file
 # (/etc/wolkenbruch.yml, ~/.config/wolkenbruch.yml,
 #    %APPDATA%/wolkenbruch.yml, ${XDG_CONFIG_HOME}/wolkenbruch.yml)
-smtp:
-    host:     localhost:587
-    user:     foobar
-    password: BARFOO
-email:
-    from:     me@whereever.com
-    to:       myself@whereever.com
-    subject:  Pack your rain gear!
-    message:  The forecast precipitation rate for today is {a:.2f} mm/h, maximum {m:2f} mm/h.
 place: Helsinki
 average_precipitation_rate_threshold: 0.1
 max_precipitation_rate_threshold: 0.5
+
+email-to: myself@whereever.com
+email-from: me@whereever.com
+email-subject: Pack your rain gear!
+email-message: The average forecast precipitation rate for today is {a:0.2f}, maximum {m:0.2f} mm/h.
+
+smtp-host: localhost:587
+smtp-user: foobar
+smtp-password: BARFOO
+
 verbose: False
 ```
 
 ### Usage
 
 Run `wolkenbruch` to check the precipitation for the next 14 hours and send you
 an e-mail reminder. Ideally, set up a cron job or a systemd timer to run
```

