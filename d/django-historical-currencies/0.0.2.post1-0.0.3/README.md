# Comparing `tmp/django-historical-currencies-0.0.2.post1.tar.gz` & `tmp/django_historical_currencies-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-historical-currencies-0.0.2.post1.tar", last modified: Wed Mar 13 17:32:24 2024, max compression
+gzip compressed data, was "django_historical_currencies-0.0.3.tar", last modified: Sun May 12 20:46:17 2024, max compression
```

## Comparing `django-historical-currencies-0.0.2.post1.tar` & `django_historical_currencies-0.0.3.tar`

### file list

```diff
@@ -1,48 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 17:32:24.981594 django-historical-currencies-0.0.2.post1/
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-03-13 17:32:18.000000 django-historical-currencies-0.0.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-03-13 17:32:18.000000 django-historical-currencies-0.0.2.post1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3486 2024-03-13 17:32:24.981594 django-historical-currencies-0.0.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-03-13 17:32:18.000000 django-historical-currencies-0.0.2.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 17:32:24.981594 django-historical-currencies-0.0.2.post1/django_historical_currencies.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3486 2024-03-13 17:32:24.000000 django-historical-currencies-0.0.2.post1/django_historical_currencies.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-03-13 17:32:24.000000 django-historical-currencies-0.0.2.post1/django_historical_currencies.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-13 17:32:24.000000 django-historical-currencies-0.0.2.post1/django_historical_currencies.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-13 17:32:24.000000 django-historical-currencies-0.0.2.post1/django_historical_currencies.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-13 17:32:24.000000 django-historical-currencies-0.0.2.post1/django_historical_currencies.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 17:32:24.977594 django-historical-currencies-0.0.2.post1/historical_currencies/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-03-13 17:32:18.000000 django-historical-currencies-0.0.2.post1/historical_currencies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-03-13 17:32:18.000000 django-historical-currencies-0.0.2.post1/historical_currencies/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-03-13 17:32:18.000000 django-historical-currencies-0.0.2.post1/historical_currencies/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-03-13 17:32:18.000000 django-historical-currencies-0.0.2.post1/historical_currencies/choices.py
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-03-13 17:32:18.000000 django-historical-currencies-0.0.2.post1/historical_currencies/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4050 2024-03-13 17:32:18.000000 django-historical-currencies-0.0.2.post1/historical_currencies/exchange.py
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-03-13 17:32:18.000000 django-historical-currencies-0.0.2.post1/historical_currencies/formatting.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 17:32:24.977594 django-historical-currencies-0.0.2.post1/historical_currencies/management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 17:32:18.000000 django-historical-currencies-0.0.2.post1/historical_currencies/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 17:32:24.977594 django-historical-currencies-0.0.2.post1/historical_currencies/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 17:32:18.000000 django-historical-currencies-0.0.2.post1/historical_currencies/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-03-13 17:32:18.000000 django-historical-currencies-0.0.2.post1/historical_currencies/management/commands/import_ecb_exchangerates.py
--rw-r--r--   0 runner    (1001) docker     (127)     5446 2024-03-13 17:32:18.000000 django-historical-currencies-0.0.2.post1/historical_currencies/management/commands/import_openexchangerates.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 17:32:24.977594 django-historical-currencies-0.0.2.post1/historical_currencies/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-03-13 17:32:18.000000 django-historical-currencies-0.0.2.post1/historical_currencies/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 17:32:18.000000 django-historical-currencies-0.0.2.post1/historical_currencies/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-03-13 17:32:18.000000 django-historical-currencies-0.0.2.post1/historical_currencies/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 17:32:24.973594 django-historical-currencies-0.0.2.post1/historical_currencies/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 17:32:24.977594 django-historical-currencies-0.0.2.post1/historical_currencies/templates/historical_currencies/
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-03-13 17:32:18.000000 django-historical-currencies-0.0.2.post1/historical_currencies/templates/historical_currencies/currency_choices_options.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 17:32:24.977594 django-historical-currencies-0.0.2.post1/historical_currencies/templatetags/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 17:32:18.000000 django-historical-currencies-0.0.2.post1/historical_currencies/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-03-13 17:32:18.000000 django-historical-currencies-0.0.2.post1/historical_currencies/templatetags/currency_choices.py
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-03-13 17:32:18.000000 django-historical-currencies-0.0.2.post1/historical_currencies/templatetags/currency_format.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 17:32:24.981594 django-historical-currencies-0.0.2.post1/historical_currencies/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 17:32:18.000000 django-historical-currencies-0.0.2.post1/historical_currencies/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-03-13 17:32:18.000000 django-historical-currencies-0.0.2.post1/historical_currencies/tests/test_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     5854 2024-03-13 17:32:18.000000 django-historical-currencies-0.0.2.post1/historical_currencies/tests/test_exchange.py
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-03-13 17:32:18.000000 django-historical-currencies-0.0.2.post1/historical_currencies/tests/test_formatting.py
--rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-03-13 17:32:18.000000 django-historical-currencies-0.0.2.post1/historical_currencies/tests/test_importers.py
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-03-13 17:32:18.000000 django-historical-currencies-0.0.2.post1/historical_currencies/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     3273 2024-03-13 17:32:18.000000 django-historical-currencies-0.0.2.post1/historical_currencies/tests/test_templatetags.py
--rw-r--r--   0 runner    (1001) docker     (127)      898 2024-03-13 17:32:18.000000 django-historical-currencies-0.0.2.post1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-13 17:32:24.981594 django-historical-currencies-0.0.2.post1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 17:32:24.981594 django-historical-currencies-0.0.2.post1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-03-13 17:32:18.000000 django-historical-currencies-0.0.2.post1/tests/test_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 20:46:17.891305 django_historical_currencies-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-12 20:46:13.000000 django_historical_currencies-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-12 20:46:13.000000 django_historical_currencies-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3508 2024-05-12 20:46:17.891305 django_historical_currencies-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-05-12 20:46:13.000000 django_historical_currencies-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 20:46:17.891305 django_historical_currencies-0.0.3/django_historical_currencies.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3508 2024-05-12 20:46:17.000000 django_historical_currencies-0.0.3/django_historical_currencies.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-05-12 20:46:17.000000 django_historical_currencies-0.0.3/django_historical_currencies.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 20:46:17.000000 django_historical_currencies-0.0.3/django_historical_currencies.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-12 20:46:17.000000 django_historical_currencies-0.0.3/django_historical_currencies.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-12 20:46:17.000000 django_historical_currencies-0.0.3/django_historical_currencies.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 20:46:17.887305 django_historical_currencies-0.0.3/historical_currencies/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-12 20:46:13.000000 django_historical_currencies-0.0.3/historical_currencies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-12 20:46:13.000000 django_historical_currencies-0.0.3/historical_currencies/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-12 20:46:13.000000 django_historical_currencies-0.0.3/historical_currencies/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-12 20:46:13.000000 django_historical_currencies-0.0.3/historical_currencies/choices.py
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-12 20:46:13.000000 django_historical_currencies-0.0.3/historical_currencies/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4293 2024-05-12 20:46:13.000000 django_historical_currencies-0.0.3/historical_currencies/exchange.py
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-12 20:46:13.000000 django_historical_currencies-0.0.3/historical_currencies/formatting.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 20:46:17.887305 django_historical_currencies-0.0.3/historical_currencies/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 20:46:13.000000 django_historical_currencies-0.0.3/historical_currencies/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 20:46:17.887305 django_historical_currencies-0.0.3/historical_currencies/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 20:46:13.000000 django_historical_currencies-0.0.3/historical_currencies/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-05-12 20:46:13.000000 django_historical_currencies-0.0.3/historical_currencies/management/commands/import_ecb_exchangerates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5446 2024-05-12 20:46:13.000000 django_historical_currencies-0.0.3/historical_currencies/management/commands/import_openexchangerates.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 20:46:17.891305 django_historical_currencies-0.0.3/historical_currencies/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-12 20:46:13.000000 django_historical_currencies-0.0.3/historical_currencies/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 20:46:13.000000 django_historical_currencies-0.0.3/historical_currencies/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-12 20:46:13.000000 django_historical_currencies-0.0.3/historical_currencies/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 20:46:13.000000 django_historical_currencies-0.0.3/historical_currencies/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 20:46:17.883305 django_historical_currencies-0.0.3/historical_currencies/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 20:46:17.891305 django_historical_currencies-0.0.3/historical_currencies/templates/historical_currencies/
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-12 20:46:13.000000 django_historical_currencies-0.0.3/historical_currencies/templates/historical_currencies/currency_choices_options.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 20:46:17.891305 django_historical_currencies-0.0.3/historical_currencies/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 20:46:13.000000 django_historical_currencies-0.0.3/historical_currencies/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-12 20:46:13.000000 django_historical_currencies-0.0.3/historical_currencies/templatetags/currency_choices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-12 20:46:13.000000 django_historical_currencies-0.0.3/historical_currencies/templatetags/currency_format.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 20:46:17.891305 django_historical_currencies-0.0.3/historical_currencies/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 20:46:13.000000 django_historical_currencies-0.0.3/historical_currencies/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-12 20:46:13.000000 django_historical_currencies-0.0.3/historical_currencies/tests/test_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6535 2024-05-12 20:46:13.000000 django_historical_currencies-0.0.3/historical_currencies/tests/test_exchange.py
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-12 20:46:13.000000 django_historical_currencies-0.0.3/historical_currencies/tests/test_formatting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-05-12 20:46:13.000000 django_historical_currencies-0.0.3/historical_currencies/tests/test_importers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-12 20:46:13.000000 django_historical_currencies-0.0.3/historical_currencies/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3273 2024-05-12 20:46:13.000000 django_historical_currencies-0.0.3/historical_currencies/tests/test_templatetags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-12 20:46:13.000000 django_historical_currencies-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 20:46:17.891305 django_historical_currencies-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 20:46:17.891305 django_historical_currencies-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-12 20:46:13.000000 django_historical_currencies-0.0.3/tests/test_settings.py
```

### Comparing `django-historical-currencies-0.0.2.post1/LICENSE` & `django_historical_currencies-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django-historical-currencies-0.0.2.post1/PKG-INFO` & `django_historical_currencies-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: django-historical-currencies
-Version: 0.0.2.post1
+Version: 0.0.3
 Summary: Django currencies with historical exchange rates
 Author-email: Stefano Rivera <stefano@rivera.za.net>
 License: ISC
 Project-URL: Repository, https://github.com/stefanor/django-historical-currencies/
 Project-URL: Changelog, https://github.com/stefanor/django-historical-currencies/blob/master/CHANGELOG.md
 Keywords: django,currencies,exchange,xe
 Classifier: Framework :: Django
 Classifier: Programming Language :: Python :: 3
+Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: django
 Requires-Dist: iso4217
 
 # Django currencies with historical exchange rates
```

### Comparing `django-historical-currencies-0.0.2.post1/README.md` & `django_historical_currencies-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `django-historical-currencies-0.0.2.post1/django_historical_currencies.egg-info/PKG-INFO` & `django_historical_currencies-0.0.3/django_historical_currencies.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: django-historical-currencies
-Version: 0.0.2.post1
+Version: 0.0.3
 Summary: Django currencies with historical exchange rates
 Author-email: Stefano Rivera <stefano@rivera.za.net>
 License: ISC
 Project-URL: Repository, https://github.com/stefanor/django-historical-currencies/
 Project-URL: Changelog, https://github.com/stefanor/django-historical-currencies/blob/master/CHANGELOG.md
 Keywords: django,currencies,exchange,xe
 Classifier: Framework :: Django
 Classifier: Programming Language :: Python :: 3
+Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: django
 Requires-Dist: iso4217
 
 # Django currencies with historical exchange rates
```

### Comparing `django-historical-currencies-0.0.2.post1/django_historical_currencies.egg-info/SOURCES.txt` & `django_historical_currencies-0.0.3/django_historical_currencies.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 historical_currencies/admin.py
 historical_currencies/apps.py
 historical_currencies/choices.py
 historical_currencies/exceptions.py
 historical_currencies/exchange.py
 historical_currencies/formatting.py
 historical_currencies/models.py
+historical_currencies/py.typed
 historical_currencies/management/__init__.py
 historical_currencies/management/commands/__init__.py
 historical_currencies/management/commands/import_ecb_exchangerates.py
 historical_currencies/management/commands/import_openexchangerates.py
 historical_currencies/migrations/0001_initial.py
 historical_currencies/migrations/__init__.py
 historical_currencies/templates/historical_currencies/currency_choices_options.html
```

### Comparing `django-historical-currencies-0.0.2.post1/historical_currencies/choices.py` & `django_historical_currencies-0.0.3/historical_currencies/choices.py`

 * *Files identical despite different names*

### Comparing `django-historical-currencies-0.0.2.post1/historical_currencies/exchange.py` & `django_historical_currencies-0.0.3/historical_currencies/exchange.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,19 +18,21 @@
 
 
 @lru_cache()
 def latest_rate(
     currency_from: str,
     currency_to: str,
     date: datetime.date,
-) -> (datetime.date, Decimal):
+) -> Tuple[datetime.date, Decimal]:
     """The latest exchange rate from currency_from to currency_to as of date.
 
     currency_from and currency_to must have a direct conversion available
     """
+    if currency_from == currency_to:
+        return (date, Decimal(1))
     rates = list(_iter_available_rates(currency_from, currency_to, date))
     rates.sort(reverse=True)
     if not rates:
         raise ExchangeRateUnavailable(
             f"No exchange rate available between {currency_from} and {currency_to} for {date}"
         )
     return rates[0]
@@ -74,49 +76,51 @@
             rate = 1 / rate
         yield direct_rate.date, rate
 
     for base_currency in _possible_base_currencies():
         rate_date = None
         rate_from = None
         rate_to = None
-        for rate in (
+        for ex_rate in (
             ExchangeRate.objects.filter(
                 date__lte=date, date__gte=oldest_acceptable_rate
             )
             .filter(
                 Q(currency=currency_from, base_currency=base_currency)
                 | Q(currency=currency_to, base_currency=base_currency)
             )
             .order_by("-date")
         ):
-            if rate_date != rate.date:
-                rate_date = rate.date
-                rate_from = rate.rate if rate.currency == currency_from else None
-                rate_to = rate.rate if rate.currency == currency_to else None
-            elif rate.currency == currency_from and rate_to is not None:
-                rate_from = rate.rate
+            if rate_date != ex_rate.date:
+                rate_date = ex_rate.date
+                rate_from = ex_rate.rate if ex_rate.currency == currency_from else None
+                rate_to = ex_rate.rate if ex_rate.currency == currency_to else None
+            elif ex_rate.currency == currency_from and rate_to is not None:
+                rate_from = ex_rate.rate
+                assert rate_date is not None
                 yield rate_date, rate_to / rate_from
                 continue
-            elif rate.currency == currency_to and rate_from is not None:
-                rate_to = rate.rate
+            elif ex_rate.currency == currency_to and rate_from is not None:
+                rate_to = ex_rate.rate
+                assert rate_date is not None
                 yield rate_date, rate_to / rate_from
                 continue
 
 
 def exchange(
     amount: Decimal,
     currency_from: str,
     currency_to: str,
     date: Optional[datetime.date] = None,
 ) -> Decimal:
     """Exchange amount of currency_from to currency_to as of date"""
     if date is None:
         date = datetime.date.today()
 
-    if currency_from == currency_to:
+    if currency_from == currency_to:  # No need to pollute the latest_rate cache
         rate_date = date
         rate = Decimal(1)
     else:
         rate_date, rate = latest_rate(currency_from, currency_to, date)
 
     amount *= rate
     if date - rate_date > datetime.timedelta(days=settings.MAX_EXCHANGE_RATE_AGE):
```

### Comparing `django-historical-currencies-0.0.2.post1/historical_currencies/management/commands/import_ecb_exchangerates.py` & `django_historical_currencies-0.0.3/historical_currencies/management/commands/import_ecb_exchangerates.py`

 * *Files identical despite different names*

### Comparing `django-historical-currencies-0.0.2.post1/historical_currencies/management/commands/import_openexchangerates.py` & `django_historical_currencies-0.0.3/historical_currencies/management/commands/import_openexchangerates.py`

 * *Files identical despite different names*

### Comparing `django-historical-currencies-0.0.2.post1/historical_currencies/migrations/0001_initial.py` & `django_historical_currencies-0.0.3/historical_currencies/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-historical-currencies-0.0.2.post1/historical_currencies/models.py` & `django_historical_currencies-0.0.3/historical_currencies/models.py`

 * *Files identical despite different names*

### Comparing `django-historical-currencies-0.0.2.post1/historical_currencies/templatetags/currency_choices.py` & `django_historical_currencies-0.0.3/historical_currencies/templatetags/currency_choices.py`

 * *Files identical despite different names*

### Comparing `django-historical-currencies-0.0.2.post1/historical_currencies/templatetags/currency_format.py` & `django_historical_currencies-0.0.3/historical_currencies/templatetags/currency_format.py`

 * *Files identical despite different names*

### Comparing `django-historical-currencies-0.0.2.post1/historical_currencies/tests/test_checks.py` & `django_historical_currencies-0.0.3/historical_currencies/tests/test_checks.py`

 * *Files identical despite different names*

### Comparing `django-historical-currencies-0.0.2.post1/historical_currencies/tests/test_exchange.py` & `django_historical_currencies-0.0.3/historical_currencies/tests/test_exchange.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,14 +11,27 @@
     exchange,
     latest_rate,
     _possible_base_currencies,
 )
 from historical_currencies.models import ExchangeRate
 
 
+class LatestRateTestCase(TestCase):
+    date = datetime.date(2021, 12, 31)
+
+    def setUp(self):
+        latest_rate.cache_clear()
+
+    def test_latest_rate_noop(self):
+        self.assertEqual(
+            latest_rate("EUR", "EUR", self.date),
+            (self.date, Decimal(1)),
+        )
+
+
 class SimpleExchangeTestCase(TestCase):
     date = datetime.date(2021, 12, 31)
 
     def setUp(self):
         latest_rate.cache_clear()
         _possible_base_currencies.cache_clear()
         ExchangeRate.objects.create(
@@ -51,14 +64,21 @@
 
     def test_raises_exception_with_old_data(self):
         with self.settings(MAX_EXCHANGE_RATE_AGE=30):
             with self.assertRaises(ExchangeRateUnavailable):
                 exchange(1, "EUR", "USD", date=datetime.date(2022, 2, 1))
 
     @mock.patch("historical_currencies.exchange.latest_rate")
+    def test_raises_exception_with_cached_old_data(self, latest_rate):
+        latest_rate.return_value = (self.date, Decimal(1.1326))
+        with self.settings(MAX_EXCHANGE_RATE_AGE=30):
+            with self.assertRaises(ExchangeRateUnavailable):
+                exchange(1, "EUR", "USD", date=datetime.date(2022, 2, 1))
+
+    @mock.patch("historical_currencies.exchange.latest_rate")
     def test_without_date(self, latest_rate):
         today = datetime.date.today()
         yesterday = today - datetime.timedelta(days=1)
         latest_rate.return_value = (yesterday, Decimal(1))
         self.assertEqual(exchange(1, "EUR", "USD"), 1)
         latest_rate.assert_called_once_with("EUR", "USD", today)
```

### Comparing `django-historical-currencies-0.0.2.post1/historical_currencies/tests/test_importers.py` & `django_historical_currencies-0.0.3/historical_currencies/tests/test_importers.py`

 * *Files identical despite different names*

### Comparing `django-historical-currencies-0.0.2.post1/historical_currencies/tests/test_templatetags.py` & `django_historical_currencies-0.0.3/historical_currencies/tests/test_templatetags.py`

 * *Files identical despite different names*

### Comparing `django-historical-currencies-0.0.2.post1/pyproject.toml` & `django_historical_currencies-0.0.3/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 readme = "README.md"
 requires-python = ">=3.7"
 keywords = ["django", "currencies", "exchange", "xe"]
 license = {text = "ISC"}
 classifiers = [
     "Framework :: Django",
     "Programming Language :: Python :: 3",
+    "Typing :: Typed",
 ]
 dependencies = [
     'django',
     'iso4217',
 ]
 dynamic = ["version"]
 
@@ -27,7 +28,16 @@
 Changelog = "https://github.com/stefanor/django-historical-currencies/blob/master/CHANGELOG.md"
 
 [tool.setuptools.packages.find]
 include = ["historical_currencies*"]
 
 [tool.setuptools.dynamic]
 version = {attr = "historical_currencies.__version__"}
+
+[tool.mypy]
+plugins = [
+    "mypy_django_plugin.main",
+]
+
+[tool.django-stubs]
+django_settings_module = "tests.test_settings"
+strict_settings = false
```

### Comparing `django-historical-currencies-0.0.2.post1/tests/test_settings.py` & `django_historical_currencies-0.0.3/tests/test_settings.py`

 * *Files identical despite different names*

