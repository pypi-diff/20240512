# Comparing `tmp/vanguard_api-0.0.4.tar.gz` & `tmp/vanguard_api-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vanguard_api-0.0.4.tar", last modified: Sat May 11 02:13:24 2024, max compression
+gzip compressed data, was "vanguard_api-0.0.5.tar", last modified: Sat May 11 02:22:56 2024, max compression
```

## Comparing `vanguard_api-0.0.4.tar` & `vanguard_api-0.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 02:13:24.736575 vanguard_api-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-11 02:13:20.000000 vanguard_api-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-05-11 02:13:24.736575 vanguard_api-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-05-11 02:13:20.000000 vanguard_api-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 02:13:24.736575 vanguard_api-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-05-11 02:13:20.000000 vanguard_api-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 02:13:24.736575 vanguard_api-0.0.4/vanguard/
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-11 02:13:20.000000 vanguard_api-0.0.4/vanguard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7325 2024-05-11 02:13:20.000000 vanguard_api-0.0.4/vanguard/account.py
--rw-r--r--   0 runner    (1001) docker     (127)    13047 2024-05-11 02:13:20.000000 vanguard_api-0.0.4/vanguard/order.py
--rw-r--r--   0 runner    (1001) docker     (127)     9404 2024-05-11 02:13:20.000000 vanguard_api-0.0.4/vanguard/session.py
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-11 02:13:20.000000 vanguard_api-0.0.4/vanguard/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 02:13:24.736575 vanguard_api-0.0.4/vanguard_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-05-11 02:13:24.000000 vanguard_api-0.0.4/vanguard_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-11 02:13:24.000000 vanguard_api-0.0.4/vanguard_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 02:13:24.000000 vanguard_api-0.0.4/vanguard_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-11 02:13:24.000000 vanguard_api-0.0.4/vanguard_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-11 02:13:24.000000 vanguard_api-0.0.4/vanguard_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 02:22:56.146478 vanguard_api-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-11 02:22:49.000000 vanguard_api-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-05-11 02:22:56.146478 vanguard_api-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-05-11 02:22:49.000000 vanguard_api-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 02:22:56.146478 vanguard_api-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-05-11 02:22:49.000000 vanguard_api-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 02:22:56.146478 vanguard_api-0.0.5/vanguard/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-11 02:22:49.000000 vanguard_api-0.0.5/vanguard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7325 2024-05-11 02:22:49.000000 vanguard_api-0.0.5/vanguard/account.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13047 2024-05-11 02:22:49.000000 vanguard_api-0.0.5/vanguard/order.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9339 2024-05-11 02:22:49.000000 vanguard_api-0.0.5/vanguard/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-11 02:22:49.000000 vanguard_api-0.0.5/vanguard/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 02:22:56.146478 vanguard_api-0.0.5/vanguard_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-05-11 02:22:56.000000 vanguard_api-0.0.5/vanguard_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-11 02:22:56.000000 vanguard_api-0.0.5/vanguard_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 02:22:56.000000 vanguard_api-0.0.5/vanguard_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-11 02:22:56.000000 vanguard_api-0.0.5/vanguard_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-11 02:22:56.000000 vanguard_api-0.0.5/vanguard_api.egg-info/top_level.txt
```

### Comparing `vanguard_api-0.0.4/LICENSE` & `vanguard_api-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `vanguard_api-0.0.4/PKG-INFO` & `vanguard_api-0.0.5/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: vanguard-api
-Version: 0.0.4
+Version: 0.0.5
 Summary: An unofficial API for Vanguard Invest
 Home-page: https://github.com/MaxxRK/vanguard-api
-Download-URL: https://github.com/MaxxRK/vanguard-api/archive/refs/tags/v0.0.4.tar.gz
+Download-URL: https://github.com/MaxxRK/vanguard-api/archive/refs/tags/v0.0.5.tar.gz
 Author: MaxxRK
 Author-email: maxxrk@pm.me
 License: MIT
 Keywords: VANGUARD,API
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Internet :: WWW/HTTP :: Session
```

### Comparing `vanguard_api-0.0.4/README.md` & `vanguard_api-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `vanguard_api-0.0.4/setup.py` & `vanguard_api-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import setuptools
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="vanguard-api",
-    version="0.0.4",
+    version="0.0.5",
     author="MaxxRK",
     author_email="maxxrk@pm.me",
     description="An unofficial API for Vanguard Invest",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
     url="https://github.com/MaxxRK/vanguard-api",
-    download_url="https://github.com/MaxxRK/vanguard-api/archive/refs/tags/v0.0.4.tar.gz",
+    download_url="https://github.com/MaxxRK/vanguard-api/archive/refs/tags/v0.0.5.tar.gz",
     keywords=["VANGUARD", "API"],
     install_requires=["playwright", "playwright-stealth"],
     packages=["vanguard"],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "Topic :: Internet :: WWW/HTTP :: Session",
```

### Comparing `vanguard_api-0.0.4/vanguard/account.py` & `vanguard_api-0.0.5/vanguard/account.py`

 * *Files identical despite different names*

### Comparing `vanguard_api-0.0.4/vanguard/order.py` & `vanguard_api-0.0.5/vanguard/order.py`

 * *Files identical despite different names*

### Comparing `vanguard_api-0.0.4/vanguard/session.py` & `vanguard_api-0.0.5/vanguard/session.py`

 * *Files 4% similar despite different names*

```diff
@@ -139,23 +139,21 @@
 
         Raises:
             Exception: If there is an error during the login process in step one.
         """
         try:
             self.password = password
             self.go_url(landing_page())
-            for _ in range(30):
+            try:
+                self.page.wait_for_selector("#username-password-submit-btn-1", timeout=30000)
+            except PlaywrightTimeoutError:
                 if self.page.url == landing_page():
-                    try:
-                        self.page.wait_for_selector("slot", timeout=1000)
-                    except PlaywrightTimeoutError:
-                        return False
+                    return False
                 else:
-                    break
-            self.page.wait_for_selector("#username-password-submit-btn-1", timeout=30000)
+                    raise Exception("Could not find submit button on login page.")
             username_box = self.page.query_selector("#USER")
             username_box.type(username, delay=random.randint(50, 500))
             username_box.press("Tab")
             password_box = self.page.query_selector("#PASSWORD-blocked")
             password_box.type(password, delay=random.randint(50, 500))
             sleep(random.uniform(1, 3))
             self.page.query_selector("#username-password-submit-btn-1").click()
```

### Comparing `vanguard_api-0.0.4/vanguard_api.egg-info/PKG-INFO` & `vanguard_api-0.0.5/vanguard_api.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: vanguard-api
-Version: 0.0.4
+Version: 0.0.5
 Summary: An unofficial API for Vanguard Invest
 Home-page: https://github.com/MaxxRK/vanguard-api
-Download-URL: https://github.com/MaxxRK/vanguard-api/archive/refs/tags/v0.0.4.tar.gz
+Download-URL: https://github.com/MaxxRK/vanguard-api/archive/refs/tags/v0.0.5.tar.gz
 Author: MaxxRK
 Author-email: maxxrk@pm.me
 License: MIT
 Keywords: VANGUARD,API
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Internet :: WWW/HTTP :: Session
```

