# Comparing `tmp/gitappwebhook-0.3.tar.gz` & `tmp/gitappwebhook-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitappwebhook-0.3.tar", last modified: Thu Apr 18 16:36:32 2024, max compression
+gzip compressed data, was "gitappwebhook-0.4.tar", last modified: Sun May 12 14:18:51 2024, max compression
```

## Comparing `gitappwebhook-0.3.tar` & `gitappwebhook-0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:36:32.797811 gitappwebhook-0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     6659 2024-04-18 16:36:32.797811 gitappwebhook-0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6207 2024-04-18 16:36:26.000000 gitappwebhook-0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:36:32.797811 gitappwebhook-0.3/gitAppWebhook.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6659 2024-04-18 16:36:32.000000 gitappwebhook-0.3/gitAppWebhook.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-18 16:36:32.000000 gitappwebhook-0.3/gitAppWebhook.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 16:36:32.000000 gitappwebhook-0.3/gitAppWebhook.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-18 16:36:32.000000 gitappwebhook-0.3/gitAppWebhook.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-18 16:36:32.000000 gitappwebhook-0.3/gitAppWebhook.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:36:32.797811 gitappwebhook-0.3/gitWebhook/
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-18 16:36:26.000000 gitappwebhook-0.3/gitWebhook/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-04-18 16:36:26.000000 gitappwebhook-0.3/gitWebhook/abstractWebhook.py
--rw-r--r--   0 runner    (1001) docker     (127)     4317 2024-04-18 16:36:26.000000 gitappwebhook-0.3/gitWebhook/functionWebhook.py
--rw-r--r--   0 runner    (1001) docker     (127)     4190 2024-04-18 16:36:26.000000 gitappwebhook-0.3/gitWebhook/pullerWebhook.py
--rw-r--r--   0 runner    (1001) docker     (127)     7071 2024-04-18 16:36:26.000000 gitappwebhook-0.3/gitWebhook/webhook.py
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-18 16:36:26.000000 gitappwebhook-0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 16:36:32.797811 gitappwebhook-0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 14:18:51.138449 gitappwebhook-0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     6411 2024-05-12 14:18:51.138449 gitappwebhook-0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6009 2024-05-12 14:18:42.000000 gitappwebhook-0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 14:18:51.138449 gitappwebhook-0.4/gitAppWebhook.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6411 2024-05-12 14:18:51.000000 gitappwebhook-0.4/gitAppWebhook.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-12 14:18:51.000000 gitappwebhook-0.4/gitAppWebhook.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 14:18:51.000000 gitappwebhook-0.4/gitAppWebhook.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-12 14:18:51.000000 gitappwebhook-0.4/gitAppWebhook.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-12 14:18:51.000000 gitappwebhook-0.4/gitAppWebhook.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 14:18:51.138449 gitappwebhook-0.4/gitWebhook/
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-12 14:18:42.000000 gitappwebhook-0.4/gitWebhook/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-05-12 14:18:42.000000 gitappwebhook-0.4/gitWebhook/abstractWebhook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4317 2024-05-12 14:18:42.000000 gitappwebhook-0.4/gitWebhook/functionWebhook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4190 2024-05-12 14:18:42.000000 gitappwebhook-0.4/gitWebhook/pullerWebhook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7071 2024-05-12 14:18:42.000000 gitappwebhook-0.4/gitWebhook/webhook.py
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-12 14:18:42.000000 gitappwebhook-0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 14:18:51.138449 gitappwebhook-0.4/setup.cfg
```

### Comparing `gitappwebhook-0.3/PKG-INFO` & `gitappwebhook-0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: gitAppWebhook
-Version: 0.3
+Version: 0.4
 Summary: Flask blueprints for handling GitHub and GitLab webhooks
 Author-email: TCA <tca.youtub@gmail.com>
 Project-URL: Homepage, https://github.com/TCA166/gitWebhook
 Classifier: Programming Language :: Python :: 3
-Classifier: License :: Free To Use But Restricted
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: flask
 
 # gitWebhook
 
@@ -131,9 +130,8 @@
     This isn't that daunting.
     There are two methods in the class: ```receiveWebhook``` and ```processWebhook```.
     Override the former to change how the raw request is handled and verified.
     Override the latter to change what is done once the webhook is verified.
 
 ## License
 
-[![CCimg](https://i.creativecommons.org/l/by/4.0/88x31.png)](http://creativecommons.org/licenses/by/4.0/)  
-This work is licensed under a [Creative Commons Attribution 4.0 International License](http://creativecommons.org/licenses/by/4.0/).  
+This work is licensed under the MIT license.
```

### Comparing `gitappwebhook-0.3/README.md` & `gitappwebhook-0.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -118,9 +118,8 @@
     This isn't that daunting.
     There are two methods in the class: ```receiveWebhook``` and ```processWebhook```.
     Override the former to change how the raw request is handled and verified.
     Override the latter to change what is done once the webhook is verified.
 
 ## License
 
-[![CCimg](https://i.creativecommons.org/l/by/4.0/88x31.png)](http://creativecommons.org/licenses/by/4.0/)  
-This work is licensed under a [Creative Commons Attribution 4.0 International License](http://creativecommons.org/licenses/by/4.0/).  
+This work is licensed under the MIT license.
```

### Comparing `gitappwebhook-0.3/gitAppWebhook.egg-info/PKG-INFO` & `gitappwebhook-0.4/gitAppWebhook.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: gitAppWebhook
-Version: 0.3
+Version: 0.4
 Summary: Flask blueprints for handling GitHub and GitLab webhooks
 Author-email: TCA <tca.youtub@gmail.com>
 Project-URL: Homepage, https://github.com/TCA166/gitWebhook
 Classifier: Programming Language :: Python :: 3
-Classifier: License :: Free To Use But Restricted
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: flask
 
 # gitWebhook
 
@@ -131,9 +130,8 @@
     This isn't that daunting.
     There are two methods in the class: ```receiveWebhook``` and ```processWebhook```.
     Override the former to change how the raw request is handled and verified.
     Override the latter to change what is done once the webhook is verified.
 
 ## License
 
-[![CCimg](https://i.creativecommons.org/l/by/4.0/88x31.png)](http://creativecommons.org/licenses/by/4.0/)  
-This work is licensed under a [Creative Commons Attribution 4.0 International License](http://creativecommons.org/licenses/by/4.0/).  
+This work is licensed under the MIT license.
```

### Comparing `gitappwebhook-0.3/gitWebhook/__init__.py` & `gitappwebhook-0.4/gitWebhook/__init__.py`

 * *Files identical despite different names*

### Comparing `gitappwebhook-0.3/gitWebhook/abstractWebhook.py` & `gitappwebhook-0.4/gitWebhook/abstractWebhook.py`

 * *Files identical despite different names*

### Comparing `gitappwebhook-0.3/gitWebhook/functionWebhook.py` & `gitappwebhook-0.4/gitWebhook/functionWebhook.py`

 * *Files identical despite different names*

### Comparing `gitappwebhook-0.3/gitWebhook/pullerWebhook.py` & `gitappwebhook-0.4/gitWebhook/pullerWebhook.py`

 * *Files identical despite different names*

### Comparing `gitappwebhook-0.3/gitWebhook/webhook.py` & `gitappwebhook-0.4/gitWebhook/webhook.py`

 * *Files identical despite different names*

