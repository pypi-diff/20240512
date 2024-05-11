# Comparing `tmp/clear_skies_stripe-0.9.3.tar.gz` & `tmp/clear_skies_stripe-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clear_skies_stripe-0.9.3.tar", max compression
+gzip compressed data, was "clear_skies_stripe-0.9.4.tar", max compression
```

## Comparing `clear_skies_stripe-0.9.3.tar` & `clear_skies_stripe-0.9.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1065 2024-04-12 11:44:22.990759 clear_skies_stripe-0.9.3/LICENSE
--rw-r--r--   0        0        0     8999 2024-04-19 18:20:25.160175 clear_skies_stripe-0.9.3/README.md
--rw-r--r--   0        0        0      728 2024-04-21 18:00:36.833130 clear_skies_stripe-0.9.3/pyproject.toml
--rw-r--r--   0        0        0       45 2024-04-19 18:15:31.887302 clear_skies_stripe-0.9.3/src/clearskies_stripe/__init__.py
--rw-r--r--   0        0        0       88 2024-04-19 11:45:03.248687 clear_skies_stripe-0.9.3/src/clearskies_stripe/backends/__init__.py
--rw-r--r--   0        0        0     2848 2024-04-19 18:17:49.367726 clear_skies_stripe-0.9.3/src/clearskies_stripe/backends/stripe_sdk_backend.py
--rw-r--r--   0        0        0      267 2024-04-19 06:51:54.068916 clear_skies_stripe-0.9.3/src/clearskies_stripe/di/__init__.py
--rw-r--r--   0        0        0     3410 2024-04-21 18:00:23.248867 clear_skies_stripe-0.9.3/src/clearskies_stripe/di/stripe.py
--rw-r--r--   0        0        0       91 2024-04-14 19:53:52.183390 clear_skies_stripe-0.9.3/src/clearskies_stripe/handlers/__init__.py
--rw-r--r--   0        0        0     3950 2024-04-19 06:57:54.561778 clear_skies_stripe-0.9.3/src/clearskies_stripe/handlers/create_setup_intent.py
--rw-r--r--   0        0        0     3545 2024-04-19 06:45:32.468903 clear_skies_stripe-0.9.3/src/clearskies_stripe/handlers/create_setup_intent_test.py
--rw-r--r--   0        0        0       81 2024-04-19 12:12:27.528744 clear_skies_stripe-0.9.3/src/clearskies_stripe/models/__init__.py
--rw-r--r--   0        0        0     1268 2024-04-19 18:18:47.575898 clear_skies_stripe-0.9.3/src/clearskies_stripe/models/stripe_customer.py
--rw-r--r--   0        0        0        0 2024-04-19 12:03:26.288725 clear_skies_stripe-0.9.3/src/clearskies_stripe/models/stripe_payment.py
--rw-r--r--   0        0        0        0 2024-04-19 12:03:29.652725 clear_skies_stripe-0.9.3/src/clearskies_stripe/models/stripe_payment_method.py
--rw-r--r--   0        0        0     9668 1970-01-01 00:00:00.000000 clear_skies_stripe-0.9.3/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-12 11:44:22.990759 clear_skies_stripe-0.9.4/LICENSE
+-rw-r--r--   0        0        0     8999 2024-04-19 18:20:25.160175 clear_skies_stripe-0.9.4/README.md
+-rw-r--r--   0        0        0      728 2024-04-22 20:43:24.177547 clear_skies_stripe-0.9.4/pyproject.toml
+-rw-r--r--   0        0        0       45 2024-04-19 18:15:31.887302 clear_skies_stripe-0.9.4/src/clearskies_stripe/__init__.py
+-rw-r--r--   0        0        0       88 2024-04-19 11:45:03.248687 clear_skies_stripe-0.9.4/src/clearskies_stripe/backends/__init__.py
+-rw-r--r--   0        0        0     2848 2024-04-19 18:17:49.367726 clear_skies_stripe-0.9.4/src/clearskies_stripe/backends/stripe_sdk_backend.py
+-rw-r--r--   0        0        0      267 2024-04-19 06:51:54.068916 clear_skies_stripe-0.9.4/src/clearskies_stripe/di/__init__.py
+-rw-r--r--   0        0        0     3410 2024-04-21 18:00:23.248867 clear_skies_stripe-0.9.4/src/clearskies_stripe/di/stripe.py
+-rw-r--r--   0        0        0       91 2024-04-14 19:53:52.183390 clear_skies_stripe-0.9.4/src/clearskies_stripe/handlers/__init__.py
+-rw-r--r--   0        0        0     3948 2024-04-22 20:41:16.037215 clear_skies_stripe-0.9.4/src/clearskies_stripe/handlers/create_setup_intent.py
+-rw-r--r--   0        0        0     3569 2024-04-22 20:43:04.981495 clear_skies_stripe-0.9.4/src/clearskies_stripe/handlers/create_setup_intent_test.py
+-rw-r--r--   0        0        0       81 2024-04-19 12:12:27.528744 clear_skies_stripe-0.9.4/src/clearskies_stripe/models/__init__.py
+-rw-r--r--   0        0        0     1268 2024-04-19 18:18:47.575898 clear_skies_stripe-0.9.4/src/clearskies_stripe/models/stripe_customer.py
+-rw-r--r--   0        0        0        0 2024-04-19 12:03:26.288725 clear_skies_stripe-0.9.4/src/clearskies_stripe/models/stripe_payment.py
+-rw-r--r--   0        0        0        0 2024-04-19 12:03:29.652725 clear_skies_stripe-0.9.4/src/clearskies_stripe/models/stripe_payment_method.py
+-rw-r--r--   0        0        0     9668 1970-01-01 00:00:00.000000 clear_skies_stripe-0.9.4/PKG-INFO
```

### Comparing `clear_skies_stripe-0.9.3/LICENSE` & `clear_skies_stripe-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `clear_skies_stripe-0.9.3/README.md` & `clear_skies_stripe-0.9.4/README.md`

 * *Files identical despite different names*

### Comparing `clear_skies_stripe-0.9.3/pyproject.toml` & `clear_skies_stripe-0.9.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 
 [tool.poetry]
 name = "clear-skies-stripe"
-version = "0.9.3"
+version = "0.9.4"
 description = "clearskies bindings for working with Stripe"
 authors = [
     "Conor Mancone <cmancone@gmail.com>",
 ]
 repository = "https://github.com/cmancone/clearskies-stripe"
 license = "MIT"
 readme = "./README.md"
```

### Comparing `clear_skies_stripe-0.9.3/src/clearskies_stripe/backends/stripe_sdk_backend.py` & `clear_skies_stripe-0.9.4/src/clearskies_stripe/backends/stripe_sdk_backend.py`

 * *Files identical despite different names*

### Comparing `clear_skies_stripe-0.9.3/src/clearskies_stripe/di/stripe.py` & `clear_skies_stripe-0.9.4/src/clearskies_stripe/di/stripe.py`

 * *Files identical despite different names*

### Comparing `clear_skies_stripe-0.9.3/src/clearskies_stripe/handlers/create_setup_intent.py` & `clear_skies_stripe-0.9.4/src/clearskies_stripe/handlers/create_setup_intent.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,15 +82,15 @@
                     **callable_kwargs,
                 )
             }
             if not isinstance(stripe_kwargs, dict):
                 raise ValueError("parameters_callable for handler " + (self.__class__.__name__) + " must return a dictionary, but returned something else.")
 
         response = {
-            **self.stripe.setup_intents.create(**stripe_kwargs),
+            **self.stripe.setup_intents.create(stripe_kwargs),
             "publishable_key": self.stripe.get_publishable_key(),
         }
         output_callable = self._configuration.get("output_callable")
         if output_callable is not None:
             response = self._di.call_function(
                 output_callable,
                 response=response,
```

### Comparing `clear_skies_stripe-0.9.3/src/clearskies_stripe/handlers/create_setup_intent_test.py` & `clear_skies_stripe-0.9.4/src/clearskies_stripe/handlers/create_setup_intent_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,15 +25,15 @@
                 "stripe": self.stripe
             },
         )
         response = create_setup_intent()
         response_data = response[0]["data"]
         self.assertEqual(200, response[1])
         self.assertEqual({"client_secret":"super secret", "id": "seti_asdf", "publishable_key": "pk_asdfer"}, response_data)
-        self.stripe.setup_intents.create.assert_called_with(confirm=True, payment_method_options={"hey": "sup"})
+        self.stripe.setup_intents.create.assert_called_with({"confirm": True, "payment_method_options":{"hey": "sup"}})
 
     def paramaters_callable(self, input_output):
         return {
             "customer":  "cust_asdfer",
             "route": input_output.get_full_path(),
             "confirm": False,
         }
@@ -52,15 +52,15 @@
                 "stripe": self.stripe
             },
         )
         response = create_setup_intent(url="/path/to/my/route")
         response_data = response[0]["data"]
         self.assertEqual(200, response[1])
         self.assertEqual({"client_secret":"super secret", "id": "seti_asdf", "publishable_key": "pk_asdfer"}, response_data)
-        self.stripe.setup_intents.create.assert_called_with(confirm=False, payment_method_options={"hey": "sup"}, customer="cust_asdfer", route="/path/to/my/route")
+        self.stripe.setup_intents.create.assert_called_with({"confirm":False, "payment_method_options":{"hey": "sup"}, "customer":"cust_asdfer", "route": "/path/to/my/route"})
 
     def output_map(self, response, input_output):
         return {
             **response,
             "route": input_output.get_full_path(),
             "hello": "world",
         }
@@ -79,8 +79,8 @@
                 "stripe": self.stripe
             },
         )
         response = create_setup_intent(url="/path/to/my/route")
         response_data = response[0]["data"]
         self.assertEqual(200, response[1])
         self.assertEqual({"client_secret":"super secret", "id": "seti_asdf", "publishable_key": "pk_asdfer", "route": "/path/to/my/route", "hello": "world"}, response_data)
-        self.stripe.setup_intents.create.assert_called_with(confirm=True, payment_method_options={"hey": "sup"})
+        self.stripe.setup_intents.create.assert_called_with({"confirm":True, "payment_method_options":{"hey": "sup"}})
```

### Comparing `clear_skies_stripe-0.9.3/src/clearskies_stripe/models/stripe_customer.py` & `clear_skies_stripe-0.9.4/src/clearskies_stripe/models/stripe_customer.py`

 * *Files identical despite different names*

### Comparing `clear_skies_stripe-0.9.3/PKG-INFO` & `clear_skies_stripe-0.9.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clear-skies-stripe
-Version: 0.9.3
+Version: 0.9.4
 Summary: clearskies bindings for working with Stripe
 Home-page: https://github.com/cmancone/clearskies-stripe
 License: MIT
 Author: Conor Mancone
 Author-email: cmancone@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

