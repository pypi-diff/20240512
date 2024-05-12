# Comparing `tmp/congress_transaction_scraper-0.0.7.tar.gz` & `tmp/congress_transaction_scraper-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "congress_transaction_scraper-0.0.7.tar", last modified: Sun May  5 20:57:17 2024, max compression
+gzip compressed data, was "congress_transaction_scraper-0.0.8.tar", last modified: Sun May 12 21:01:50 2024, max compression
```

## Comparing `congress_transaction_scraper-0.0.7.tar` & `congress_transaction_scraper-0.0.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 mkm        (501) staff       (20)        0 2024-05-05 20:57:17.542149 congress_transaction_scraper-0.0.7/
--rw-r--r--   0 mkm        (501) staff       (20)    35149 2023-12-29 17:09:27.000000 congress_transaction_scraper-0.0.7/LICENSE
--rw-r--r--   0 mkm        (501) staff       (20)      817 2024-05-05 20:57:17.541871 congress_transaction_scraper-0.0.7/PKG-INFO
--rw-r--r--   0 mkm        (501) staff       (20)       94 2023-05-07 21:02:14.000000 congress_transaction_scraper-0.0.7/README.md
--rw-r--r--   0 mkm        (501) staff       (20)      680 2024-05-05 20:56:59.000000 congress_transaction_scraper-0.0.7/pyproject.toml
--rw-r--r--   0 mkm        (501) staff       (20)       38 2024-05-05 20:57:17.542199 congress_transaction_scraper-0.0.7/setup.cfg
-drwxr-xr-x   0 mkm        (501) staff       (20)        0 2024-05-05 20:57:17.539423 congress_transaction_scraper-0.0.7/src/
--rw-r--r--   0 mkm        (501) staff       (20)        0 2023-12-29 17:09:27.000000 congress_transaction_scraper-0.0.7/src/__init__.py
-drwxr-xr-x   0 mkm        (501) staff       (20)        0 2024-05-05 20:57:17.541605 congress_transaction_scraper-0.0.7/src/congress_transaction_scraper.egg-info/
--rw-r--r--   0 mkm        (501) staff       (20)      817 2024-05-05 20:57:17.000000 congress_transaction_scraper-0.0.7/src/congress_transaction_scraper.egg-info/PKG-INFO
--rw-r--r--   0 mkm        (501) staff       (20)      457 2024-05-05 20:57:17.000000 congress_transaction_scraper-0.0.7/src/congress_transaction_scraper.egg-info/SOURCES.txt
--rw-r--r--   0 mkm        (501) staff       (20)        1 2024-05-05 20:57:17.000000 congress_transaction_scraper-0.0.7/src/congress_transaction_scraper.egg-info/dependency_links.txt
--rw-r--r--   0 mkm        (501) staff       (20)       44 2024-05-05 20:57:17.000000 congress_transaction_scraper-0.0.7/src/congress_transaction_scraper.egg-info/requires.txt
--rw-r--r--   0 mkm        (501) staff       (20)       24 2024-05-05 20:57:17.000000 congress_transaction_scraper-0.0.7/src/congress_transaction_scraper.egg-info/top_level.txt
-drwxr-xr-x   0 mkm        (501) staff       (20)        0 2024-05-05 20:57:17.540498 congress_transaction_scraper-0.0.7/src/scrapers/
--rw-r--r--   0 mkm        (501) staff       (20)        0 2023-12-29 17:24:19.000000 congress_transaction_scraper-0.0.7/src/scrapers/__init__.py
--rw-r--r--   0 mkm        (501) staff       (20)      187 2024-05-05 20:56:13.000000 congress_transaction_scraper-0.0.7/src/scrapers/base.py
--rw-r--r--   0 mkm        (501) staff       (20)     4722 2024-05-05 20:56:47.000000 congress_transaction_scraper-0.0.7/src/scrapers/senate.py
-drwxr-xr-x   0 mkm        (501) staff       (20)        0 2024-05-05 20:57:17.541263 congress_transaction_scraper-0.0.7/src/utils/
--rw-r--r--   0 mkm        (501) staff       (20)      105 2024-01-07 20:12:24.000000 congress_transaction_scraper-0.0.7/src/utils/__init__.py
--rw-r--r--   0 mkm        (501) staff       (20)     1656 2024-05-05 20:56:47.000000 congress_transaction_scraper-0.0.7/src/utils/data.py
--rw-r--r--   0 mkm        (501) staff       (20)     1127 2023-12-29 17:33:08.000000 congress_transaction_scraper-0.0.7/src/utils/session.py
+drwxr-xr-x   0 mkm        (501) staff       (20)        0 2024-05-12 21:01:50.318853 congress_transaction_scraper-0.0.8/
+-rw-r--r--   0 mkm        (501) staff       (20)    35149 2023-12-29 17:09:27.000000 congress_transaction_scraper-0.0.8/LICENSE
+-rw-r--r--   0 mkm        (501) staff       (20)      817 2024-05-12 21:01:50.318620 congress_transaction_scraper-0.0.8/PKG-INFO
+-rw-r--r--   0 mkm        (501) staff       (20)       94 2023-05-07 21:02:14.000000 congress_transaction_scraper-0.0.8/README.md
+-rw-r--r--   0 mkm        (501) staff       (20)      680 2024-05-12 21:01:39.000000 congress_transaction_scraper-0.0.8/pyproject.toml
+-rw-r--r--   0 mkm        (501) staff       (20)       38 2024-05-12 21:01:50.318898 congress_transaction_scraper-0.0.8/setup.cfg
+drwxr-xr-x   0 mkm        (501) staff       (20)        0 2024-05-12 21:01:50.315518 congress_transaction_scraper-0.0.8/src/
+-rw-r--r--   0 mkm        (501) staff       (20)        0 2023-12-29 17:09:27.000000 congress_transaction_scraper-0.0.8/src/__init__.py
+drwxr-xr-x   0 mkm        (501) staff       (20)        0 2024-05-12 21:01:50.318276 congress_transaction_scraper-0.0.8/src/congress_transaction_scraper.egg-info/
+-rw-r--r--   0 mkm        (501) staff       (20)      817 2024-05-12 21:01:50.000000 congress_transaction_scraper-0.0.8/src/congress_transaction_scraper.egg-info/PKG-INFO
+-rw-r--r--   0 mkm        (501) staff       (20)      457 2024-05-12 21:01:50.000000 congress_transaction_scraper-0.0.8/src/congress_transaction_scraper.egg-info/SOURCES.txt
+-rw-r--r--   0 mkm        (501) staff       (20)        1 2024-05-12 21:01:50.000000 congress_transaction_scraper-0.0.8/src/congress_transaction_scraper.egg-info/dependency_links.txt
+-rw-r--r--   0 mkm        (501) staff       (20)       44 2024-05-12 21:01:50.000000 congress_transaction_scraper-0.0.8/src/congress_transaction_scraper.egg-info/requires.txt
+-rw-r--r--   0 mkm        (501) staff       (20)       24 2024-05-12 21:01:50.000000 congress_transaction_scraper-0.0.8/src/congress_transaction_scraper.egg-info/top_level.txt
+drwxr-xr-x   0 mkm        (501) staff       (20)        0 2024-05-12 21:01:50.316636 congress_transaction_scraper-0.0.8/src/scrapers/
+-rw-r--r--   0 mkm        (501) staff       (20)        0 2023-12-29 17:24:19.000000 congress_transaction_scraper-0.0.8/src/scrapers/__init__.py
+-rw-r--r--   0 mkm        (501) staff       (20)      187 2024-05-05 20:56:13.000000 congress_transaction_scraper-0.0.8/src/scrapers/base.py
+-rw-r--r--   0 mkm        (501) staff       (20)     4716 2024-05-12 21:00:52.000000 congress_transaction_scraper-0.0.8/src/scrapers/senate.py
+drwxr-xr-x   0 mkm        (501) staff       (20)        0 2024-05-12 21:01:50.317958 congress_transaction_scraper-0.0.8/src/utils/
+-rw-r--r--   0 mkm        (501) staff       (20)      105 2024-01-07 20:12:24.000000 congress_transaction_scraper-0.0.8/src/utils/__init__.py
+-rw-r--r--   0 mkm        (501) staff       (20)     1656 2024-05-05 20:56:47.000000 congress_transaction_scraper-0.0.8/src/utils/data.py
+-rw-r--r--   0 mkm        (501) staff       (20)     1127 2023-12-29 17:33:08.000000 congress_transaction_scraper-0.0.8/src/utils/session.py
```

### Comparing `congress_transaction_scraper-0.0.7/LICENSE` & `congress_transaction_scraper-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `congress_transaction_scraper-0.0.7/PKG-INFO` & `congress_transaction_scraper-0.0.8/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: congress-transaction-scraper
-Version: 0.0.7
+Version: 0.0.8
 Summary: Congressional transaction scraper
 Author-email: Example Author <author@example.com>
 Project-URL: Homepage, https://github.com/antidipyramid/congressional-transaction-scraper
 Project-URL: Issues, https://github.com/antidipyramid/congressional-transaction-scraper/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `congress_transaction_scraper-0.0.7/pyproject.toml` & `congress_transaction_scraper-0.0.8/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "congress-transaction-scraper"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="Example Author", email="author@example.com" },
 ]
 description = "Congressional transaction scraper"
 readme = "README.md"
 requires-python = ">=3.11"
 dependencies = [
```

### Comparing `congress_transaction_scraper-0.0.7/src/congress_transaction_scraper.egg-info/PKG-INFO` & `congress_transaction_scraper-0.0.8/src/congress_transaction_scraper.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: congress-transaction-scraper
-Version: 0.0.7
+Version: 0.0.8
 Summary: Congressional transaction scraper
 Author-email: Example Author <author@example.com>
 Project-URL: Homepage, https://github.com/antidipyramid/congressional-transaction-scraper
 Project-URL: Issues, https://github.com/antidipyramid/congressional-transaction-scraper/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `congress_transaction_scraper-0.0.7/src/scrapers/senate.py` & `congress_transaction_scraper-0.0.8/src/scrapers/senate.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
         results = self.post(
             SenateTransactionScraper.SEARCH_PATH,
             data={
                 "start": str(start),
                 "length": str(SenateTransactionScraper.RESULTS_PER_PAGE),
                 "report_types": "[11]",
                 "filer_types": "[1]",
-                "submitted_start_date": "06/01/2023 00:00:00",
+                "submitted_start_date": self.start_date,
                 "submitted_end_date": "",
                 "candidate_state": "",
                 "senator_state": state,
                 "office_id": "",
                 "first_name": "",
                 "last_name": "",
             },
```

### Comparing `congress_transaction_scraper-0.0.7/src/utils/data.py` & `congress_transaction_scraper-0.0.8/src/utils/data.py`

 * *Files identical despite different names*

### Comparing `congress_transaction_scraper-0.0.7/src/utils/session.py` & `congress_transaction_scraper-0.0.8/src/utils/session.py`

 * *Files identical despite different names*

