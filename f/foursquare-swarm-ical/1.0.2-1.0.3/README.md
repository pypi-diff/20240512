# Comparing `tmp/foursquare_swarm_ical-1.0.2.tar.gz` & `tmp/foursquare_swarm_ical-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foursquare_swarm_ical-1.0.2.tar", last modified: Wed May  1 08:05:54 2024, max compression
+gzip compressed data, was "foursquare_swarm_ical-1.0.3.tar", last modified: Sun May 12 13:33:42 2024, max compression
```

## Comparing `foursquare_swarm_ical-1.0.2.tar` & `foursquare_swarm_ical-1.0.3.tar`

### file list

```diff
@@ -1,43 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 08:05:54.512749 foursquare_swarm_ical-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-01 08:05:27.000000 foursquare_swarm_ical-1.0.2/.cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 08:05:54.504749 foursquare_swarm_ical-1.0.2/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-01 08:05:27.000000 foursquare_swarm_ical-1.0.2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 08:05:54.504749 foursquare_swarm_ical-1.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     5396 2024-05-01 08:05:27.000000 foursquare_swarm_ical-1.0.2/.github/workflows/check.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-05-01 08:05:27.000000 foursquare_swarm_ical-1.0.2/.github/workflows/pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-01 08:05:27.000000 foursquare_swarm_ical-1.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-01 08:05:27.000000 foursquare_swarm_ical-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3668 2024-05-01 08:05:27.000000 foursquare_swarm_ical-1.0.2/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     6993 2024-05-01 08:05:54.512749 foursquare_swarm_ical-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5032 2024-05-01 08:05:27.000000 foursquare_swarm_ical-1.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-05-01 08:05:27.000000 foursquare_swarm_ical-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-01 08:05:54.512749 foursquare_swarm_ical-1.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 08:05:54.504749 foursquare_swarm_ical-1.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 08:05:54.508749 foursquare_swarm_ical-1.0.2/src/foursquare_swarm_ical/
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-01 08:05:27.000000 foursquare_swarm_ical-1.0.2/src/foursquare_swarm_ical/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-01 08:05:27.000000 foursquare_swarm_ical-1.0.2/src/foursquare_swarm_ical/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-05-01 08:05:27.000000 foursquare_swarm_ical-1.0.2/src/foursquare_swarm_ical/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2621 2024-05-01 08:05:27.000000 foursquare_swarm_ical-1.0.2/src/foursquare_swarm_ical/config_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     2722 2024-05-01 08:05:27.000000 foursquare_swarm_ical-1.0.2/src/foursquare_swarm_ical/db.py
--rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-05-01 08:05:27.000000 foursquare_swarm_ical-1.0.2/src/foursquare_swarm_ical/emoji.py
--rw-r--r--   0 runner    (1001) docker     (127)    63578 2024-05-01 08:05:27.000000 foursquare_swarm_ical-1.0.2/src/foursquare_swarm_ical/emoji.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-05-01 08:05:27.000000 foursquare_swarm_ical-1.0.2/src/foursquare_swarm_ical/ical.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 08:05:27.000000 foursquare_swarm_ical-1.0.2/src/foursquare_swarm_ical/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 08:05:54.508749 foursquare_swarm_ical-1.0.2/src/foursquare_swarm_ical.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6993 2024-05-01 08:05:54.000000 foursquare_swarm_ical-1.0.2/src/foursquare_swarm_ical.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-05-01 08:05:54.000000 foursquare_swarm_ical-1.0.2/src/foursquare_swarm_ical.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 08:05:54.000000 foursquare_swarm_ical-1.0.2/src/foursquare_swarm_ical.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-01 08:05:54.000000 foursquare_swarm_ical-1.0.2/src/foursquare_swarm_ical.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-01 08:05:54.000000 foursquare_swarm_ical-1.0.2/src/foursquare_swarm_ical.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-01 08:05:54.000000 foursquare_swarm_ical-1.0.2/src/foursquare_swarm_ical.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 08:05:54.508749 foursquare_swarm_ical-1.0.2/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 08:05:54.504749 foursquare_swarm_ical-1.0.2/tests/cassettes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 08:05:54.508749 foursquare_swarm_ical-1.0.2/tests/cassettes/test_sync/
--rw-r--r--   0 runner    (1001) docker     (127)    13846 2024-05-01 08:05:27.000000 foursquare_swarm_ical-1.0.2/tests/cassettes/test_sync/test_sync.yaml
--rwxr-xr-x   0 runner    (1001) docker     (127)      452 2024-05-01 08:05:27.000000 foursquare_swarm_ical-1.0.2/tests/include.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      157 2024-05-01 08:05:27.000000 foursquare_swarm_ical-1.0.2/tests/prysk-noescape.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 08:05:54.508749 foursquare_swarm_ical-1.0.2/tests/readme/
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-01 08:05:27.000000 foursquare_swarm_ical-1.0.2/tests/readme/config-sample.md
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-05-01 08:05:27.000000 foursquare_swarm_ical-1.0.2/tests/readme/help.md
--rw-r--r--   0 runner    (1001) docker     (127)     7817 2024-05-01 08:05:27.000000 foursquare_swarm_ical-1.0.2/tests/test_ical.py
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-01 08:05:27.000000 foursquare_swarm_ical-1.0.2/tests/test_sync.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 13:33:42.071488 foursquare_swarm_ical-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-12 13:33:18.000000 foursquare_swarm_ical-1.0.3/.cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 13:33:42.067487 foursquare_swarm_ical-1.0.3/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-12 13:33:18.000000 foursquare_swarm_ical-1.0.3/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 13:33:42.067487 foursquare_swarm_ical-1.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     5396 2024-05-12 13:33:18.000000 foursquare_swarm_ical-1.0.3/.github/workflows/check.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-05-12 13:33:18.000000 foursquare_swarm_ical-1.0.3/.github/workflows/pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-12 13:33:18.000000 foursquare_swarm_ical-1.0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-12 13:33:18.000000 foursquare_swarm_ical-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3653 2024-05-12 13:33:18.000000 foursquare_swarm_ical-1.0.3/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     6993 2024-05-12 13:33:42.071488 foursquare_swarm_ical-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5032 2024-05-12 13:33:18.000000 foursquare_swarm_ical-1.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-05-12 13:33:18.000000 foursquare_swarm_ical-1.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-12 13:33:42.071488 foursquare_swarm_ical-1.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 13:33:42.067487 foursquare_swarm_ical-1.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 13:33:42.067487 foursquare_swarm_ical-1.0.3/src/foursquare_swarm_ical/
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-12 13:33:18.000000 foursquare_swarm_ical-1.0.3/src/foursquare_swarm_ical/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-12 13:33:18.000000 foursquare_swarm_ical-1.0.3/src/foursquare_swarm_ical/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-05-12 13:33:18.000000 foursquare_swarm_ical-1.0.3/src/foursquare_swarm_ical/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2621 2024-05-12 13:33:18.000000 foursquare_swarm_ical-1.0.3/src/foursquare_swarm_ical/config_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2726 2024-05-12 13:33:18.000000 foursquare_swarm_ical-1.0.3/src/foursquare_swarm_ical/db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-05-12 13:33:18.000000 foursquare_swarm_ical-1.0.3/src/foursquare_swarm_ical/emoji.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63578 2024-05-12 13:33:18.000000 foursquare_swarm_ical-1.0.3/src/foursquare_swarm_ical/emoji.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-05-12 13:33:18.000000 foursquare_swarm_ical-1.0.3/src/foursquare_swarm_ical/ical.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 13:33:18.000000 foursquare_swarm_ical-1.0.3/src/foursquare_swarm_ical/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 13:33:42.071488 foursquare_swarm_ical-1.0.3/src/foursquare_swarm_ical.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6993 2024-05-12 13:33:42.000000 foursquare_swarm_ical-1.0.3/src/foursquare_swarm_ical.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-12 13:33:42.000000 foursquare_swarm_ical-1.0.3/src/foursquare_swarm_ical.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 13:33:42.000000 foursquare_swarm_ical-1.0.3/src/foursquare_swarm_ical.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-12 13:33:42.000000 foursquare_swarm_ical-1.0.3/src/foursquare_swarm_ical.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-12 13:33:42.000000 foursquare_swarm_ical-1.0.3/src/foursquare_swarm_ical.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-12 13:33:42.000000 foursquare_swarm_ical-1.0.3/src/foursquare_swarm_ical.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 13:33:42.071488 foursquare_swarm_ical-1.0.3/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 13:33:42.067487 foursquare_swarm_ical-1.0.3/tests/cassettes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 13:33:42.071488 foursquare_swarm_ical-1.0.3/tests/cassettes/test_sync/
+-rw-r--r--   0 runner    (1001) docker     (127)    13846 2024-05-12 13:33:18.000000 foursquare_swarm_ical-1.0.3/tests/cassettes/test_sync/test_sync.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      452 2024-05-12 13:33:18.000000 foursquare_swarm_ical-1.0.3/tests/include.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 13:33:42.071488 foursquare_swarm_ical-1.0.3/tests/readme/
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-12 13:33:18.000000 foursquare_swarm_ical-1.0.3/tests/readme/config-sample.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-05-12 13:33:18.000000 foursquare_swarm_ical-1.0.3/tests/readme/help.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7817 2024-05-12 13:33:18.000000 foursquare_swarm_ical-1.0.3/tests/test_ical.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-12 13:33:18.000000 foursquare_swarm_ical-1.0.3/tests/test_sync.py
```

### Comparing `foursquare_swarm_ical-1.0.2/.github/workflows/check.yaml` & `foursquare_swarm_ical-1.0.3/.github/workflows/check.yaml`

 * *Files identical despite different names*

### Comparing `foursquare_swarm_ical-1.0.2/.github/workflows/pypi.yaml` & `foursquare_swarm_ical-1.0.3/.github/workflows/pypi.yaml`

 * *Files identical despite different names*

### Comparing `foursquare_swarm_ical-1.0.2/LICENSE` & `foursquare_swarm_ical-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `foursquare_swarm_ical-1.0.2/Makefile` & `foursquare_swarm_ical-1.0.3/Makefile`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 
 .PHONY: test-prysk
 test-prysk: PRYSK_INTERACTIVE=$(shell [ -t 0 ] && echo --interactive)
 test-prysk: $(VENV_DONE)
 	PATH="$(CURDIR)/$(VENV)/bin:$$PATH" \
 	XDG_DATA_HOME=/home/user/.local/share \
 	XDG_CONFIG_HOME=/home/user/.config \
-	$(VENV_PYTHON) tests/prysk-noescape.py --indent=4 --shell=/bin/bash $(PRYSK_INTERACTIVE) \
+	$(VENV_PYTHON) -m prysk --indent=4 --shell=/bin/bash $(PRYSK_INTERACTIVE) \
 		$(wildcard tests/*.md tests/*/*.md tests/*/*/*.md)
 
 .PHONY: README.md
 README.md: test-prysk
 	tests/include.py < $@ > $@.tmp
 	mv -f $@.tmp $@
```

### Comparing `foursquare_swarm_ical-1.0.2/PKG-INFO` & `foursquare_swarm_ical-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foursquare-swarm-ical
-Version: 1.0.2
+Version: 1.0.3
 Summary: Sync Foursquare Swarm check-ins to local sqlite DB and generate iCalendar
 Author-email: Tomáš Janoušek <tomi@nomi.cz>
 License: MIT
 Project-URL: Homepage, https://github.com/liskin/foursquare-swarm-ical
 Project-URL: Release Notes, https://github.com/liskin/foursquare-swarm-ical/releases
 Project-URL: Issues, https://github.com/liskin/foursquare-swarm-ical/issues
 Project-URL: CI, https://github.com/liskin/foursquare-swarm-ical/actions
@@ -32,15 +32,15 @@
 Requires-Dist: importlib-resources; python_version < "3.9"
 Requires-Dist: platformdirs>=2.1
 Provides-Extra: dev
 Requires-Dist: build>=0.7; extra == "dev"
 Requires-Dist: flake8; extra == "dev"
 Requires-Dist: isort>=5.0; extra == "dev"
 Requires-Dist: mypy>=0.900; extra == "dev"
-Requires-Dist: prysk==0.17.0; extra == "dev"
+Requires-Dist: prysk>=0.20.0; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 Requires-Dist: types-PyYAML; extra == "dev"
 Requires-Dist: types-pytz; extra == "dev"
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-recording; extra == "test"
```

### Comparing `foursquare_swarm_ical-1.0.2/README.md` & `foursquare_swarm_ical-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `foursquare_swarm_ical-1.0.2/pyproject.toml` & `foursquare_swarm_ical-1.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
 [project.optional-dependencies]
 dev = [
     "build >= 0.7",
     "flake8",
     "isort >= 5.0",
     "mypy >= 0.900",
-    "prysk == 0.17.0",
+    "prysk >= 0.20.0",
     "twine",
     "types-PyYAML",
     "types-pytz",
 ]
 test = [
     "pytest",
     "pytest-recording",
```

### Comparing `foursquare_swarm_ical-1.0.2/src/foursquare_swarm_ical/cli.py` & `foursquare_swarm_ical-1.0.3/src/foursquare_swarm_ical/cli.py`

 * *Files identical despite different names*

### Comparing `foursquare_swarm_ical-1.0.2/src/foursquare_swarm_ical/config_file.py` & `foursquare_swarm_ical-1.0.3/src/foursquare_swarm_ical/config_file.py`

 * *Files identical despite different names*

### Comparing `foursquare_swarm_ical-1.0.2/src/foursquare_swarm_ical/db.py` & `foursquare_swarm_ical-1.0.3/src/foursquare_swarm_ical/db.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,9 +82,9 @@
 
 def fetch_checkins(access_token: str) -> Iterator[Any]:
     client = Foursquare(access_token=access_token)
     return client.users.all_checkins()
 
 
 def checkins(db: sqlite3.Connection) -> Iterator[Any]:
-    for checkin in db.execute("SELECT data FROM checkins ORDER BY createdAt DESC"):
+    for checkin in db.execute("SELECT data FROM checkins ORDER BY createdAt DESC, id"):
         yield json.loads(checkin['data'])
```

### Comparing `foursquare_swarm_ical-1.0.2/src/foursquare_swarm_ical/emoji.py` & `foursquare_swarm_ical-1.0.3/src/foursquare_swarm_ical/emoji.py`

 * *Files identical despite different names*

### Comparing `foursquare_swarm_ical-1.0.2/src/foursquare_swarm_ical/emoji.yaml` & `foursquare_swarm_ical-1.0.3/src/foursquare_swarm_ical/emoji.yaml`

 * *Files identical despite different names*

### Comparing `foursquare_swarm_ical-1.0.2/src/foursquare_swarm_ical/ical.py` & `foursquare_swarm_ical-1.0.3/src/foursquare_swarm_ical/ical.py`

 * *Files identical despite different names*

### Comparing `foursquare_swarm_ical-1.0.2/src/foursquare_swarm_ical.egg-info/PKG-INFO` & `foursquare_swarm_ical-1.0.3/src/foursquare_swarm_ical.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foursquare-swarm-ical
-Version: 1.0.2
+Version: 1.0.3
 Summary: Sync Foursquare Swarm check-ins to local sqlite DB and generate iCalendar
 Author-email: Tomáš Janoušek <tomi@nomi.cz>
 License: MIT
 Project-URL: Homepage, https://github.com/liskin/foursquare-swarm-ical
 Project-URL: Release Notes, https://github.com/liskin/foursquare-swarm-ical/releases
 Project-URL: Issues, https://github.com/liskin/foursquare-swarm-ical/issues
 Project-URL: CI, https://github.com/liskin/foursquare-swarm-ical/actions
@@ -32,15 +32,15 @@
 Requires-Dist: importlib-resources; python_version < "3.9"
 Requires-Dist: platformdirs>=2.1
 Provides-Extra: dev
 Requires-Dist: build>=0.7; extra == "dev"
 Requires-Dist: flake8; extra == "dev"
 Requires-Dist: isort>=5.0; extra == "dev"
 Requires-Dist: mypy>=0.900; extra == "dev"
-Requires-Dist: prysk==0.17.0; extra == "dev"
+Requires-Dist: prysk>=0.20.0; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 Requires-Dist: types-PyYAML; extra == "dev"
 Requires-Dist: types-pytz; extra == "dev"
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-recording; extra == "test"
```

### Comparing `foursquare_swarm_ical-1.0.2/src/foursquare_swarm_ical.egg-info/SOURCES.txt` & `foursquare_swarm_ical-1.0.3/src/foursquare_swarm_ical.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -20,13 +20,12 @@
 src/foursquare_swarm_ical.egg-info/PKG-INFO
 src/foursquare_swarm_ical.egg-info/SOURCES.txt
 src/foursquare_swarm_ical.egg-info/dependency_links.txt
 src/foursquare_swarm_ical.egg-info/entry_points.txt
 src/foursquare_swarm_ical.egg-info/requires.txt
 src/foursquare_swarm_ical.egg-info/top_level.txt
 tests/include.py
-tests/prysk-noescape.py
 tests/test_ical.py
 tests/test_sync.py
 tests/cassettes/test_sync/test_sync.yaml
 tests/readme/config-sample.md
 tests/readme/help.md
```

### Comparing `foursquare_swarm_ical-1.0.2/tests/cassettes/test_sync/test_sync.yaml` & `foursquare_swarm_ical-1.0.3/tests/cassettes/test_sync/test_sync.yaml`

 * *Files identical despite different names*

### Comparing `foursquare_swarm_ical-1.0.2/tests/readme/config-sample.md` & `foursquare_swarm_ical-1.0.3/tests/readme/config-sample.md`

 * *Files identical despite different names*

### Comparing `foursquare_swarm_ical-1.0.2/tests/readme/help.md` & `foursquare_swarm_ical-1.0.3/tests/readme/help.md`

 * *Files identical despite different names*

### Comparing `foursquare_swarm_ical-1.0.2/tests/test_ical.py` & `foursquare_swarm_ical-1.0.3/tests/test_ical.py`

 * *Files identical despite different names*

### Comparing `foursquare_swarm_ical-1.0.2/tests/test_sync.py` & `foursquare_swarm_ical-1.0.3/tests/test_sync.py`

 * *Files identical despite different names*

