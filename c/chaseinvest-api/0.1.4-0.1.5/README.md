# Comparing `tmp/chaseinvest_api-0.1.4.tar.gz` & `tmp/chaseinvest_api-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chaseinvest_api-0.1.4.tar", last modified: Thu May  9 14:23:16 2024, max compression
+gzip compressed data, was "chaseinvest_api-0.1.5.tar", last modified: Sat May 11 22:59:50 2024, max compression
```

## Comparing `chaseinvest_api-0.1.4.tar` & `chaseinvest_api-0.1.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:23:16.126992 chaseinvest_api-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-09 14:23:11.000000 chaseinvest_api-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6916 2024-05-09 14:23:16.126992 chaseinvest_api-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6032 2024-05-09 14:23:11.000000 chaseinvest_api-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:23:16.122992 chaseinvest_api-0.1.4/chase/
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-09 14:23:11.000000 chaseinvest_api-0.1.4/chase/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8446 2024-05-09 14:23:11.000000 chaseinvest_api-0.1.4/chase/account.py
--rw-r--r--   0 runner    (1001) docker     (127)    12962 2024-05-09 14:23:11.000000 chaseinvest_api-0.1.4/chase/order.py
--rw-r--r--   0 runner    (1001) docker     (127)     9489 2024-05-09 14:23:11.000000 chaseinvest_api-0.1.4/chase/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     9284 2024-05-09 14:23:11.000000 chaseinvest_api-0.1.4/chase/symbols.py
--rw-r--r--   0 runner    (1001) docker     (127)     4830 2024-05-09 14:23:11.000000 chaseinvest_api-0.1.4/chase/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:23:16.126992 chaseinvest_api-0.1.4/chaseinvest_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6916 2024-05-09 14:23:16.000000 chaseinvest_api-0.1.4/chaseinvest_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-09 14:23:16.000000 chaseinvest_api-0.1.4/chaseinvest_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 14:23:16.000000 chaseinvest_api-0.1.4/chaseinvest_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-09 14:23:16.000000 chaseinvest_api-0.1.4/chaseinvest_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-09 14:23:16.000000 chaseinvest_api-0.1.4/chaseinvest_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 14:23:16.126992 chaseinvest_api-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-05-09 14:23:11.000000 chaseinvest_api-0.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:23:16.126992 chaseinvest_api-0.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4462 2024-05-09 14:23:11.000000 chaseinvest_api-0.1.4/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 22:59:50.299345 chaseinvest_api-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-11 22:59:46.000000 chaseinvest_api-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6916 2024-05-11 22:59:50.299345 chaseinvest_api-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6032 2024-05-11 22:59:46.000000 chaseinvest_api-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 22:59:50.299345 chaseinvest_api-0.1.5/chase/
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-11 22:59:46.000000 chaseinvest_api-0.1.5/chase/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8446 2024-05-11 22:59:46.000000 chaseinvest_api-0.1.5/chase/account.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12932 2024-05-11 22:59:46.000000 chaseinvest_api-0.1.5/chase/order.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10067 2024-05-11 22:59:46.000000 chaseinvest_api-0.1.5/chase/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9284 2024-05-11 22:59:46.000000 chaseinvest_api-0.1.5/chase/symbols.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4830 2024-05-11 22:59:46.000000 chaseinvest_api-0.1.5/chase/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 22:59:50.299345 chaseinvest_api-0.1.5/chaseinvest_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6916 2024-05-11 22:59:50.000000 chaseinvest_api-0.1.5/chaseinvest_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-11 22:59:50.000000 chaseinvest_api-0.1.5/chaseinvest_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 22:59:50.000000 chaseinvest_api-0.1.5/chaseinvest_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-11 22:59:50.000000 chaseinvest_api-0.1.5/chaseinvest_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-11 22:59:50.000000 chaseinvest_api-0.1.5/chaseinvest_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 22:59:50.299345 chaseinvest_api-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-05-11 22:59:46.000000 chaseinvest_api-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 22:59:50.299345 chaseinvest_api-0.1.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4462 2024-05-11 22:59:46.000000 chaseinvest_api-0.1.5/tests/test.py
```

### Comparing `chaseinvest_api-0.1.4/LICENSE` & `chaseinvest_api-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `chaseinvest_api-0.1.4/PKG-INFO` & `chaseinvest_api-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: chaseinvest-api
-Version: 0.1.4
+Version: 0.1.5
 Summary: An unofficial API for Chase Invest
 Home-page: https://github.com/MaxxRK/chaseinvest-api
-Download-URL: https://github.com/MaxxRK/chaseinvest-api/archive/refs/tags/v0.1.4.tar.gz
+Download-URL: https://github.com/MaxxRK/chaseinvest-api/archive/refs/tags/v0.1.5.tar.gz
 Author: MaxxRK
 Author-email: maxxrk@pm.me
 License: MIT
 Keywords: CHASE,API
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Internet :: WWW/HTTP :: Session
```

### Comparing `chaseinvest_api-0.1.4/README.md` & `chaseinvest_api-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `chaseinvest_api-0.1.4/chase/account.py` & `chaseinvest_api-0.1.5/chase/account.py`

 * *Files identical despite different names*

### Comparing `chaseinvest_api-0.1.4/chase/order.py` & `chaseinvest_api-0.1.5/chase/order.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,17 +89,15 @@
                                       Defaults to True.
 
         Returns:
             Order:order_confirmation: Dictionary containing the order confirmation data.
         """
 
         self.session.page.goto(order_page(account_id))
-        experience = self.session.page.wait_for_selector(
-                "span > a > span.link__text"
-            )
+        experience = self.session.page.wait_for_selector("span > a > span.link__text")
         if experience.text_content() == "Switch back to classic trading experience":
             experience.click()
             self.session.page.reload()
 
         order_messages = {
             "ORDER INVALID": "",
             "WARNING": "",
```

### Comparing `chaseinvest_api-0.1.4/chase/session.py` & `chaseinvest_api-0.1.5/chase/session.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import random
 import traceback
 from time import sleep
 
 from playwright.sync_api import TimeoutError as PlaywrightTimeoutError
 from playwright.sync_api import sync_playwright
 
-from .urls import login_page
+from .urls import login_page, landing_page
 
 
 class ChaseSession:
     """
     A class to manage a session with Chase.
 
     This class provides methods to initialize a WebDriver with the necessary options, log into Chase, and perform other actions on the Chase website.
@@ -183,17 +183,28 @@
                     if str(last_four) in item_text:
                         item.click()
                         break
                 self.page.click('button[type="submit"]')
                 self.page.wait_for_load_state("load", timeout=30000)
                 return True
             except PlaywrightTimeoutError:
-                if self.title is not None:
-                    self.save_storage_state()
-                return False
+                try:
+                    self.page.wait_for_selector(
+                        "input#input-sec-auth-options-0", timeout=1000
+                    )
+                    sleep(random.uniform(0.1, 1.0))
+                    self.page.click("input#input-sec-auth-options-0")
+                    sleep(random.uniform(0.1, 1.0))
+                    self.page.click('button[type="submit"]')
+                    self.page.wait_for_url(landing_page(), timeout=60000)
+                    return False
+                except PlaywrightTimeoutError:
+                    if self.title is not None:
+                        self.save_storage_state()
+                    return False
         except Exception as e:
             self.close_browser()
             traceback.print_exc()
             raise Exception(f"Error in first step of login into Chase: {e}")
 
     def login_two(self, code):
         """
```

### Comparing `chaseinvest_api-0.1.4/chase/symbols.py` & `chaseinvest_api-0.1.5/chase/symbols.py`

 * *Files identical despite different names*

### Comparing `chaseinvest_api-0.1.4/chase/urls.py` & `chaseinvest_api-0.1.5/chase/urls.py`

 * *Files identical despite different names*

### Comparing `chaseinvest_api-0.1.4/chaseinvest_api.egg-info/PKG-INFO` & `chaseinvest_api-0.1.5/chaseinvest_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: chaseinvest-api
-Version: 0.1.4
+Version: 0.1.5
 Summary: An unofficial API for Chase Invest
 Home-page: https://github.com/MaxxRK/chaseinvest-api
-Download-URL: https://github.com/MaxxRK/chaseinvest-api/archive/refs/tags/v0.1.4.tar.gz
+Download-URL: https://github.com/MaxxRK/chaseinvest-api/archive/refs/tags/v0.1.5.tar.gz
 Author: MaxxRK
 Author-email: maxxrk@pm.me
 License: MIT
 Keywords: CHASE,API
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Internet :: WWW/HTTP :: Session
```

### Comparing `chaseinvest_api-0.1.4/setup.py` & `chaseinvest_api-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import setuptools
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="chaseinvest-api",
-    version="0.1.4",
+    version="0.1.5",
     author="MaxxRK",
     author_email="maxxrk@pm.me",
     description="An unofficial API for Chase Invest",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
     url="https://github.com/MaxxRK/chaseinvest-api",
-    download_url="https://github.com/MaxxRK/chaseinvest-api/archive/refs/tags/v0.1.4.tar.gz",
+    download_url="https://github.com/MaxxRK/chaseinvest-api/archive/refs/tags/v0.1.5.tar.gz",
     keywords=["CHASE", "API"],
     install_requires=["playwright", "playwright-stealth"],
     packages=["chase"],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "Topic :: Internet :: WWW/HTTP :: Session",
```

### Comparing `chaseinvest_api-0.1.4/tests/test.py` & `chaseinvest_api-0.1.5/tests/test.py`

 * *Files identical despite different names*

