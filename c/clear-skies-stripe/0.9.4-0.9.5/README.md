# Comparing `tmp/clear_skies_stripe-0.9.4.tar.gz` & `tmp/clear_skies_stripe-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clear_skies_stripe-0.9.4.tar", max compression
+gzip compressed data, was "clear_skies_stripe-0.9.5.tar", max compression
```

## Comparing `clear_skies_stripe-0.9.4.tar` & `clear_skies_stripe-0.9.5.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0     1065 2024-04-12 11:44:22.990759 clear_skies_stripe-0.9.4/LICENSE
--rw-r--r--   0        0        0     8999 2024-04-19 18:20:25.160175 clear_skies_stripe-0.9.4/README.md
--rw-r--r--   0        0        0      728 2024-04-22 20:43:24.177547 clear_skies_stripe-0.9.4/pyproject.toml
--rw-r--r--   0        0        0       45 2024-04-19 18:15:31.887302 clear_skies_stripe-0.9.4/src/clearskies_stripe/__init__.py
--rw-r--r--   0        0        0       88 2024-04-19 11:45:03.248687 clear_skies_stripe-0.9.4/src/clearskies_stripe/backends/__init__.py
--rw-r--r--   0        0        0     2848 2024-04-19 18:17:49.367726 clear_skies_stripe-0.9.4/src/clearskies_stripe/backends/stripe_sdk_backend.py
--rw-r--r--   0        0        0      267 2024-04-19 06:51:54.068916 clear_skies_stripe-0.9.4/src/clearskies_stripe/di/__init__.py
--rw-r--r--   0        0        0     3410 2024-04-21 18:00:23.248867 clear_skies_stripe-0.9.4/src/clearskies_stripe/di/stripe.py
--rw-r--r--   0        0        0       91 2024-04-14 19:53:52.183390 clear_skies_stripe-0.9.4/src/clearskies_stripe/handlers/__init__.py
--rw-r--r--   0        0        0     3948 2024-04-22 20:41:16.037215 clear_skies_stripe-0.9.4/src/clearskies_stripe/handlers/create_setup_intent.py
--rw-r--r--   0        0        0     3569 2024-04-22 20:43:04.981495 clear_skies_stripe-0.9.4/src/clearskies_stripe/handlers/create_setup_intent_test.py
--rw-r--r--   0        0        0       81 2024-04-19 12:12:27.528744 clear_skies_stripe-0.9.4/src/clearskies_stripe/models/__init__.py
--rw-r--r--   0        0        0     1268 2024-04-19 18:18:47.575898 clear_skies_stripe-0.9.4/src/clearskies_stripe/models/stripe_customer.py
--rw-r--r--   0        0        0        0 2024-04-19 12:03:26.288725 clear_skies_stripe-0.9.4/src/clearskies_stripe/models/stripe_payment.py
--rw-r--r--   0        0        0        0 2024-04-19 12:03:29.652725 clear_skies_stripe-0.9.4/src/clearskies_stripe/models/stripe_payment_method.py
--rw-r--r--   0        0        0     9668 1970-01-01 00:00:00.000000 clear_skies_stripe-0.9.4/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-12 11:44:22.990759 clear_skies_stripe-0.9.5/LICENSE
+-rw-r--r--   0        0        0     8999 2024-04-19 18:20:25.160175 clear_skies_stripe-0.9.5/README.md
+-rw-r--r--   0        0        0      728 2024-05-11 23:45:08.264729 clear_skies_stripe-0.9.5/pyproject.toml
+-rw-r--r--   0        0        0       45 2024-04-19 18:15:31.887302 clear_skies_stripe-0.9.5/src/clearskies_stripe/__init__.py
+-rw-r--r--   0        0        0       88 2024-04-19 11:45:03.248687 clear_skies_stripe-0.9.5/src/clearskies_stripe/backends/__init__.py
+-rw-r--r--   0        0        0     2848 2024-04-19 18:17:49.367726 clear_skies_stripe-0.9.5/src/clearskies_stripe/backends/stripe_sdk_backend.py
+-rw-r--r--   0        0        0      267 2024-04-19 06:51:54.068916 clear_skies_stripe-0.9.5/src/clearskies_stripe/di/__init__.py
+-rw-r--r--   0        0        0     3410 2024-04-21 18:00:23.248867 clear_skies_stripe-0.9.5/src/clearskies_stripe/di/stripe.py
+-rw-r--r--   0        0        0       91 2024-04-14 19:53:52.183390 clear_skies_stripe-0.9.5/src/clearskies_stripe/handlers/__init__.py
+-rw-r--r--   0        0        0     3948 2024-04-22 20:41:16.037215 clear_skies_stripe-0.9.5/src/clearskies_stripe/handlers/create_setup_intent.py
+-rw-r--r--   0        0        0     3569 2024-04-22 20:43:04.981495 clear_skies_stripe-0.9.5/src/clearskies_stripe/handlers/create_setup_intent_test.py
+-rw-r--r--   0        0        0      223 2024-05-11 23:44:40.209139 clear_skies_stripe-0.9.5/src/clearskies_stripe/models/__init__.py
+-rw-r--r--   0        0        0     2187 2024-05-11 23:44:40.209139 clear_skies_stripe-0.9.5/src/clearskies_stripe/models/stripe_charge.py
+-rw-r--r--   0        0        0     1279 2024-05-11 23:44:40.209139 clear_skies_stripe-0.9.5/src/clearskies_stripe/models/stripe_customer.py
+-rw-r--r--   0        0        0        0 2024-05-11 23:44:40.209139 clear_skies_stripe-0.9.5/src/clearskies_stripe/models/stripe_payment.py
+-rw-r--r--   0        0        0      615 2024-05-11 23:44:40.209139 clear_skies_stripe-0.9.5/src/clearskies_stripe/models/stripe_payment_method.py
+-rw-r--r--   0        0        0     9668 1970-01-01 00:00:00.000000 clear_skies_stripe-0.9.5/PKG-INFO
```

### Comparing `clear_skies_stripe-0.9.4/LICENSE` & `clear_skies_stripe-0.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `clear_skies_stripe-0.9.4/README.md` & `clear_skies_stripe-0.9.5/README.md`

 * *Files identical despite different names*

### Comparing `clear_skies_stripe-0.9.4/pyproject.toml` & `clear_skies_stripe-0.9.5/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 
 [tool.poetry]
 name = "clear-skies-stripe"
-version = "0.9.4"
+version = "0.9.5"
 description = "clearskies bindings for working with Stripe"
 authors = [
     "Conor Mancone <cmancone@gmail.com>",
 ]
 repository = "https://github.com/cmancone/clearskies-stripe"
 license = "MIT"
 readme = "./README.md"
```

### Comparing `clear_skies_stripe-0.9.4/src/clearskies_stripe/backends/stripe_sdk_backend.py` & `clear_skies_stripe-0.9.5/src/clearskies_stripe/backends/stripe_sdk_backend.py`

 * *Files identical despite different names*

### Comparing `clear_skies_stripe-0.9.4/src/clearskies_stripe/di/stripe.py` & `clear_skies_stripe-0.9.5/src/clearskies_stripe/di/stripe.py`

 * *Files identical despite different names*

### Comparing `clear_skies_stripe-0.9.4/src/clearskies_stripe/handlers/create_setup_intent.py` & `clear_skies_stripe-0.9.5/src/clearskies_stripe/handlers/create_setup_intent.py`

 * *Files identical despite different names*

### Comparing `clear_skies_stripe-0.9.4/src/clearskies_stripe/handlers/create_setup_intent_test.py` & `clear_skies_stripe-0.9.5/src/clearskies_stripe/handlers/create_setup_intent_test.py`

 * *Files identical despite different names*

### Comparing `clear_skies_stripe-0.9.4/src/clearskies_stripe/models/stripe_customer.py` & `clear_skies_stripe-0.9.5/src/clearskies_stripe/models/stripe_customer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import clearskies
-from clearskies.column_types import boolean, integer, json, string
+from clearskies.column_types import boolean, integer, json, string, timestamp
 from collections import OrderedDict
 
 
 class StripeCustomer(clearskies.Model):
     id_column_alt_name = "customer"
 
     def __init__(self, stripe_sdk_backend, columns):
```

### Comparing `clear_skies_stripe-0.9.4/PKG-INFO` & `clear_skies_stripe-0.9.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clear-skies-stripe
-Version: 0.9.4
+Version: 0.9.5
 Summary: clearskies bindings for working with Stripe
 Home-page: https://github.com/cmancone/clearskies-stripe
 License: MIT
 Author: Conor Mancone
 Author-email: cmancone@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

