# Comparing `tmp/comwatt-0.10.0.tar.gz` & `tmp/comwatt-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "comwatt-0.10.0.tar", last modified: Sun May 12 16:33:08 2024, max compression
+gzip compressed data, was "comwatt-0.9.0.tar", last modified: Sun May 12 08:40:20 2024, max compression
```

## Comparing `comwatt-0.10.0.tar` & `comwatt-0.9.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:33:08.377941 comwatt-0.10.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-12 16:33:00.000000 comwatt-0.10.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      909 2024-05-12 16:33:08.377941 comwatt-0.10.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-12 16:33:00.000000 comwatt-0.10.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:33:08.373942 comwatt-0.10.0/comwatt/
--rwxr-xr-x   0 runner    (1001) docker     (127)     6822 2024-05-12 16:33:00.000000 comwatt-0.10.0/comwatt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:33:08.377941 comwatt-0.10.0/comwatt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      909 2024-05-12 16:33:08.000000 comwatt-0.10.0/comwatt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-12 16:33:08.000000 comwatt-0.10.0/comwatt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 16:33:08.000000 comwatt-0.10.0/comwatt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-12 16:33:08.000000 comwatt-0.10.0/comwatt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-12 16:33:08.000000 comwatt-0.10.0/comwatt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-12 16:33:00.000000 comwatt-0.10.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 16:33:08.377941 comwatt-0.10.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-12 16:33:00.000000 comwatt-0.10.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 08:40:20.807753 comwatt-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-12 08:40:17.000000 comwatt-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-05-12 08:40:20.807753 comwatt-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-12 08:40:17.000000 comwatt-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 08:40:20.803753 comwatt-0.9.0/comwatt/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6781 2024-05-12 08:40:17.000000 comwatt-0.9.0/comwatt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 08:40:20.803753 comwatt-0.9.0/comwatt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-05-12 08:40:20.000000 comwatt-0.9.0/comwatt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-12 08:40:20.000000 comwatt-0.9.0/comwatt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 08:40:20.000000 comwatt-0.9.0/comwatt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-12 08:40:20.000000 comwatt-0.9.0/comwatt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-12 08:40:20.000000 comwatt-0.9.0/comwatt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-12 08:40:17.000000 comwatt-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 08:40:20.807753 comwatt-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-12 08:40:17.000000 comwatt-0.9.0/setup.py
```

### Comparing `comwatt-0.10.0/LICENSE` & `comwatt-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `comwatt-0.10.0/PKG-INFO` & `comwatt-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: comwatt
-Version: 0.10.0
+Version: 0.9.0
 Summary: Python client for Comwatt
 Home-page: https://github.com/51CGO/comwatt
 Author: Christophe Godart
 Author-email: 51CGO@lilo.org
 License: MIT
 Keywords: Comwatt,client
 Description-Content-Type: text/markdown
```

### Comparing `comwatt-0.10.0/README.md` & `comwatt-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `comwatt-0.10.0/comwatt/__init__.py` & `comwatt-0.9.0/comwatt/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -155,16 +155,14 @@
     def display_devices_page(self, site=None):
 
         if not site:
             site = self.default_site
 
         if self.current_url != 'https://energy.comwatt.com/#/sites/%s/devices/' % site:
             self.get('https://energy.comwatt.com/#/sites/%s/devices/' % site)
-        else:
-            self.refresh()
 
         try:
             WebDriverWait(self, timeout=20).until(lambda d: d.find_element(By.CLASS_NAME, 'ZoneDevices-item'))
         except:
             raise RuntimeError
             # Todo : Add update ?
```

### Comparing `comwatt-0.10.0/comwatt.egg-info/PKG-INFO` & `comwatt-0.9.0/comwatt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: comwatt
-Version: 0.10.0
+Version: 0.9.0
 Summary: Python client for Comwatt
 Home-page: https://github.com/51CGO/comwatt
 Author: Christophe Godart
 Author-email: 51CGO@lilo.org
 License: MIT
 Keywords: Comwatt,client
 Description-Content-Type: text/markdown
```

