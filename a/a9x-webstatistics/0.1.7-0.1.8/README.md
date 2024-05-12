# Comparing `tmp/a9x_webstatistics-0.1.7.tar.gz` & `tmp/a9x_webstatistics-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "a9x_webstatistics-0.1.7.tar", last modified: Sat May 11 18:11:16 2024, max compression
+gzip compressed data, was "a9x_webstatistics-0.1.8.tar", last modified: Sat May 11 19:02:02 2024, max compression
```

## Comparing `a9x_webstatistics-0.1.7.tar` & `a9x_webstatistics-0.1.8.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 18:11:16.025854 a9x_webstatistics-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-05-11 18:11:02.000000 a9x_webstatistics-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-11 18:11:02.000000 a9x_webstatistics-0.1.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    16544 2024-05-11 18:11:16.025854 a9x_webstatistics-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15480 2024-05-11 18:11:02.000000 a9x_webstatistics-0.1.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 18:11:02.000000 a9x_webstatistics-0.1.7/dist_del
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-11 18:11:02.000000 a9x_webstatistics-0.1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-11 18:11:16.025854 a9x_webstatistics-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-05-11 18:11:02.000000 a9x_webstatistics-0.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 18:11:16.021854 a9x_webstatistics-0.1.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 18:11:16.021854 a9x_webstatistics-0.1.7/src/a9x_webstatistics/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-11 18:11:02.000000 a9x_webstatistics-0.1.7/src/a9x_webstatistics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6517 2024-05-11 18:11:02.000000 a9x_webstatistics-0.1.7/src/a9x_webstatistics/main.py
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-11 18:11:02.000000 a9x_webstatistics-0.1.7/src/a9x_webstatistics/module1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-05-11 18:11:02.000000 a9x_webstatistics-0.1.7/src/a9x_webstatistics/updatestatistics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 18:11:16.025854 a9x_webstatistics-0.1.7/src/a9x_webstatistics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16544 2024-05-11 18:11:16.000000 a9x_webstatistics-0.1.7/src/a9x_webstatistics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-11 18:11:16.000000 a9x_webstatistics-0.1.7/src/a9x_webstatistics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 18:11:16.000000 a9x_webstatistics-0.1.7/src/a9x_webstatistics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-11 18:11:16.000000 a9x_webstatistics-0.1.7/src/a9x_webstatistics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-11 18:11:16.000000 a9x_webstatistics-0.1.7/src/a9x_webstatistics.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 18:11:16.025854 a9x_webstatistics-0.1.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-11 18:11:02.000000 a9x_webstatistics-0.1.7/tests/test_main001.py
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-11 18:11:02.000000 a9x_webstatistics-0.1.7/tests/test_main010.py
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-11 18:11:02.000000 a9x_webstatistics-0.1.7/tests/test_module1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 19:02:02.485813 a9x_webstatistics-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-05-11 19:01:52.000000 a9x_webstatistics-0.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-11 19:01:52.000000 a9x_webstatistics-0.1.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    16544 2024-05-11 19:02:02.485813 a9x_webstatistics-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15480 2024-05-11 19:01:52.000000 a9x_webstatistics-0.1.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 19:01:52.000000 a9x_webstatistics-0.1.8/dist_del
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-11 19:01:52.000000 a9x_webstatistics-0.1.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-11 19:02:02.485813 a9x_webstatistics-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-05-11 19:01:52.000000 a9x_webstatistics-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 19:02:02.481813 a9x_webstatistics-0.1.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 19:02:02.481813 a9x_webstatistics-0.1.8/src/a9x_webstatistics/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-11 19:01:52.000000 a9x_webstatistics-0.1.8/src/a9x_webstatistics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6091 2024-05-11 19:01:52.000000 a9x_webstatistics-0.1.8/src/a9x_webstatistics/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-11 19:01:52.000000 a9x_webstatistics-0.1.8/src/a9x_webstatistics/module1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-05-11 19:01:52.000000 a9x_webstatistics-0.1.8/src/a9x_webstatistics/updatestatistics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 19:02:02.485813 a9x_webstatistics-0.1.8/src/a9x_webstatistics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16544 2024-05-11 19:02:02.000000 a9x_webstatistics-0.1.8/src/a9x_webstatistics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-11 19:02:02.000000 a9x_webstatistics-0.1.8/src/a9x_webstatistics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 19:02:02.000000 a9x_webstatistics-0.1.8/src/a9x_webstatistics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-11 19:02:02.000000 a9x_webstatistics-0.1.8/src/a9x_webstatistics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-11 19:02:02.000000 a9x_webstatistics-0.1.8/src/a9x_webstatistics.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 19:02:02.485813 a9x_webstatistics-0.1.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-11 19:01:52.000000 a9x_webstatistics-0.1.8/tests/test_main001.py
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-11 19:01:52.000000 a9x_webstatistics-0.1.8/tests/test_main010.py
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-11 19:01:52.000000 a9x_webstatistics-0.1.8/tests/test_module1.py
```

### Comparing `a9x_webstatistics-0.1.7/LICENSE` & `a9x_webstatistics-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `a9x_webstatistics-0.1.7/PKG-INFO` & `a9x_webstatistics-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: a9x_webstatistics
-Version: 0.1.7
+Version: 0.1.8
 Summary: Web Statistics and Analytics Package
 Home-page: https://github.com/ava007/a9x-webstatistics
 Author: André von Arx
 Author-email: andrevonarx@bluewin.ch
 Project-URL: Documentation, https://github.com/ava007/a9x-webstatistics
 Project-URL: Bug Reports, https://github.com/ava007/a9x-webstatistics/issues
 Project-URL: Source Code, https://github.com/ava007/a9x-webstatistics
```

### Comparing `a9x_webstatistics-0.1.7/README.md` & `a9x_webstatistics-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `a9x_webstatistics-0.1.7/setup.py` & `a9x_webstatistics-0.1.8/setup.py`

 * *Files identical despite different names*

### Comparing `a9x_webstatistics-0.1.7/src/a9x_webstatistics/main.py` & `a9x_webstatistics-0.1.8/src/a9x_webstatistics/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -45,35 +45,19 @@
             'timestamp': dto.strftime("%Y%m%d%H%M%S") ,
             'request': request,
             'status': status,
             'bytes_sent': bytes_sent,
             'referer': referer,
             'user_agent': user_agent
         }
-
+        if country:
+            r['country'] = country
+    
     return r,j
 
-def detectDeviceClass(ua):
-  if ua is None:
-     return 'desktop'
-  if (ua.lower().find('bot') > 0):
-     return 'bots'
-  if (ua.lower().find('python') > 0):
-     return 'bots'
-  if (ua.lower().find('mediapartner') > 0):
-     return 'others'
-  if (ua.lower().find('curl') > 0):
-     return 'others'
-  if (ua.lower().find('ipad') > 0):
-     return 'tablet'
-  if (ua.lower().find('mobile') > 0):
-     return 'mobile'
-  if (ua.lower().find('android') > 0):
-     return 'tablet'
-  return 'desktop'
 
 def runws(statfile, infile, geoip):
 
     try: 
         georeader = geoip2.database.Reader(geoip)
     except FileNotFoundError:
         print("geoip2 file not found, continue processing")
@@ -144,15 +128,15 @@
             recparsed, j = parseRec(rec, log_pattern, j, georeader)
             # skip unrecognized records:
             if not recparsed or recparsed['timestamp'] is None or recparsed['ip'] is None:
                 continue
             # skip already processed data:
             if recparsed['timestamp']  <=  d['timelastrec']:
                 continue
-            d = upd(d, recparsed, visitIP)
+            d, visitIP = upd(d, recparsed, visitIP)
             
     # write updated statistic file:
     with open(statfile, "w") as sf:
        json.dump(d,sf)  
     return 0
 
 if __name__ == "__main__":
```

### Comparing `a9x_webstatistics-0.1.7/src/a9x_webstatistics.egg-info/PKG-INFO` & `a9x_webstatistics-0.1.8/src/a9x_webstatistics.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: a9x_webstatistics
-Version: 0.1.7
+Version: 0.1.8
 Summary: Web Statistics and Analytics Package
 Home-page: https://github.com/ava007/a9x-webstatistics
 Author: André von Arx
 Author-email: andrevonarx@bluewin.ch
 Project-URL: Documentation, https://github.com/ava007/a9x-webstatistics
 Project-URL: Bug Reports, https://github.com/ava007/a9x-webstatistics/issues
 Project-URL: Source Code, https://github.com/ava007/a9x-webstatistics
```

### Comparing `a9x_webstatistics-0.1.7/tests/test_main001.py` & `a9x_webstatistics-0.1.8/tests/test_main001.py`

 * *Files identical despite different names*

### Comparing `a9x_webstatistics-0.1.7/tests/test_main010.py` & `a9x_webstatistics-0.1.8/tests/test_main010.py`

 * *Files identical despite different names*

