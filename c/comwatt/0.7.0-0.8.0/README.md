# Comparing `tmp/comwatt-0.7.0.tar.gz` & `tmp/comwatt-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "comwatt-0.7.0.tar", last modified: Fri May 10 15:05:33 2024, max compression
+gzip compressed data, was "comwatt-0.8.0.tar", last modified: Sat May 11 14:30:07 2024, max compression
```

## Comparing `comwatt-0.7.0.tar` & `comwatt-0.8.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:05:33.755677 comwatt-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-10 15:05:25.000000 comwatt-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      908 2024-05-10 15:05:33.751677 comwatt-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-10 15:05:25.000000 comwatt-0.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:05:33.751677 comwatt-0.7.0/comwatt/
--rwxr-xr-x   0 runner    (1001) docker     (127)     5922 2024-05-10 15:05:25.000000 comwatt-0.7.0/comwatt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:05:33.751677 comwatt-0.7.0/comwatt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      908 2024-05-10 15:05:33.000000 comwatt-0.7.0/comwatt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-10 15:05:33.000000 comwatt-0.7.0/comwatt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 15:05:33.000000 comwatt-0.7.0/comwatt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-10 15:05:33.000000 comwatt-0.7.0/comwatt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-10 15:05:33.000000 comwatt-0.7.0/comwatt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-10 15:05:25.000000 comwatt-0.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 15:05:33.755677 comwatt-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-10 15:05:25.000000 comwatt-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:30:07.413853 comwatt-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-11 14:30:03.000000 comwatt-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-05-11 14:30:07.413853 comwatt-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-11 14:30:03.000000 comwatt-0.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:30:07.413853 comwatt-0.8.0/comwatt/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6122 2024-05-11 14:30:03.000000 comwatt-0.8.0/comwatt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:30:07.413853 comwatt-0.8.0/comwatt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-05-11 14:30:07.000000 comwatt-0.8.0/comwatt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-11 14:30:07.000000 comwatt-0.8.0/comwatt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 14:30:07.000000 comwatt-0.8.0/comwatt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-11 14:30:07.000000 comwatt-0.8.0/comwatt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-11 14:30:07.000000 comwatt-0.8.0/comwatt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-11 14:30:03.000000 comwatt-0.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 14:30:07.413853 comwatt-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-11 14:30:03.000000 comwatt-0.8.0/setup.py
```

### Comparing `comwatt-0.7.0/LICENSE` & `comwatt-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `comwatt-0.7.0/PKG-INFO` & `comwatt-0.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: comwatt
-Version: 0.7.0
+Version: 0.8.0
 Summary: Python client for Comwatt
 Home-page: https://github.com/51CGO/comwatt
 Author: Christophe Godart
 Author-email: 51CGO@lilo.org
 License: MIT
 Keywords: Comwatt,client
 Description-Content-Type: text/markdown
```

### Comparing `comwatt-0.7.0/README.md` & `comwatt-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `comwatt-0.7.0/comwatt/__init__.py` & `comwatt-0.8.0/comwatt/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -150,17 +150,23 @@
 
         self.logger.debug("Begin refresh %s" % site)
 
         if not site:
             site = self.default_site
 
         self.zones = []
-
-        self.get('https://energy.comwatt.com/#/sites/%s/devices/' % site)
-        WebDriverWait(self, timeout=20).until(lambda d: d.find_element(By.CLASS_NAME, 'ZoneDevices-item'))
+        
+        if self.current_url != 'https://energy.comwatt.com/#/sites/%s/devices/' % site:
+            self.get('https://energy.comwatt.com/#/sites/%s/devices/' % site)
+
+        try:
+            WebDriverWait(self, timeout=20).until(lambda d: d.find_element(By.CLASS_NAME, 'ZoneDevices-item'))
+        except:
+            raise RuntimeError
+            # Todo : Add refresh ?
 
         for elt_zone in self.find_elements(By.CLASS_NAME, 'ZoneDevices-item'): 
 
             elem_title = elt_zone.find_element(By.CLASS_NAME, 'css-2bb7pl')
             zone = Zone(elem_title.text)
             
             self.zones.append(zone)
```

### Comparing `comwatt-0.7.0/comwatt.egg-info/PKG-INFO` & `comwatt-0.8.0/comwatt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: comwatt
-Version: 0.7.0
+Version: 0.8.0
 Summary: Python client for Comwatt
 Home-page: https://github.com/51CGO/comwatt
 Author: Christophe Godart
 Author-email: 51CGO@lilo.org
 License: MIT
 Keywords: Comwatt,client
 Description-Content-Type: text/markdown
```

