# Comparing `tmp/kitab-0.0.25.tar.gz` & `tmp/kitab-0.0.26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kitab-0.0.25.tar", last modified: Sat May  4 08:51:35 2024, max compression
+gzip compressed data, was "kitab-0.0.26.tar", last modified: Sun May 12 10:25:09 2024, max compression
```

## Comparing `kitab-0.0.25.tar` & `kitab-0.0.26.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2024-05-04 08:51:35.378851 kitab-0.0.25/
--rw-rw-rw-   0        0        0     1100 2024-04-07 17:53:03.000000 kitab-0.0.25/LICENSE
--rw-rw-rw-   0        0        0     5908 2024-05-04 08:51:35.370647 kitab-0.0.25/PKG-INFO
--rw-rw-rw-   0        0        0     5298 2024-05-04 08:45:45.000000 kitab-0.0.25/README.md
-drwxrwxrwx   0        0        0        0 2024-05-04 08:51:35.297118 kitab-0.0.25/kitab/
--rw-rw-rw-   0        0        0      131 2024-04-08 06:51:45.000000 kitab-0.0.25/kitab/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-04 08:51:35.330411 kitab-0.0.25/kitab/api/
--rw-rw-rw-   0        0        0        0 2024-04-07 17:53:03.000000 kitab-0.0.25/kitab/api/__init__.py
--rw-rw-rw-   0        0        0     7848 2024-04-26 08:09:51.000000 kitab-0.0.25/kitab/api/app.py
-drwxrwxrwx   0        0        0        0 2024-05-04 08:51:35.346168 kitab-0.0.25/kitab/db/
--rw-rw-rw-   0        0        0      416 2024-04-26 08:05:03.000000 kitab-0.0.25/kitab/db/__init__.py
--rw-rw-rw-   0        0        0      232 2024-05-04 08:17:25.000000 kitab-0.0.25/kitab/db/db_credentials.py
--rw-rw-rw-   0        0        0     1836 2024-04-25 20:34:46.000000 kitab-0.0.25/kitab/db/db_info.py
--rw-rw-rw-   0        0        0    20768 2024-05-04 08:20:57.000000 kitab-0.0.25/kitab/db/functions.py
--rw-rw-rw-   0        0        0     6825 2024-04-26 09:12:48.000000 kitab-0.0.25/kitab/db/get_data.py
--rw-rw-rw-   0        0        0    16160 2024-05-03 14:12:28.000000 kitab-0.0.25/kitab/db/sql_interactions.py
-drwxrwxrwx   0        0        0        0 2024-05-04 08:51:35.354192 kitab-0.0.25/kitab/logger/
--rw-rw-rw-   0        0        0       37 2024-04-07 17:53:03.000000 kitab-0.0.25/kitab/logger/__init__.py
--rw-rw-rw-   0        0        0     1812 2024-04-25 18:53:05.000000 kitab-0.0.25/kitab/logger/logger.py
-drwxrwxrwx   0        0        0        0 2024-05-04 08:51:35.362489 kitab-0.0.25/kitab/recommendation_model/
--rw-rw-rw-   0        0        0       88 2024-04-08 13:12:13.000000 kitab-0.0.25/kitab/recommendation_model/__init__.py
--rw-rw-rw-   0        0        0     5162 2024-05-03 14:37:05.000000 kitab-0.0.25/kitab/recommendation_model/models.py
--rw-rw-rw-   0        0        0     6366 2024-04-26 09:08:13.000000 kitab-0.0.25/kitab/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-04 08:51:35.370647 kitab-0.0.25/kitab.egg-info/
--rw-rw-rw-   0        0        0     5908 2024-05-04 08:51:35.000000 kitab-0.0.25/kitab.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      550 2024-05-04 08:51:35.000000 kitab-0.0.25/kitab.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-04 08:51:35.000000 kitab-0.0.25/kitab.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       78 2024-05-04 08:51:35.000000 kitab-0.0.25/kitab.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-05-04 08:51:35.000000 kitab-0.0.25/kitab.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-04 08:51:35.378851 kitab-0.0.25/setup.cfg
--rw-rw-rw-   0        0        0     1053 2024-05-04 08:50:31.000000 kitab-0.0.25/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-04 08:51:35.362489 kitab-0.0.25/tests/
--rw-rw-rw-   0        0        0        0 2024-04-07 17:53:03.000000 kitab-0.0.25/tests/test_module1.py
--rw-rw-rw-   0        0        0        0 2024-04-07 17:53:03.000000 kitab-0.0.25/tests/test_module2.py
+drwxrwxrwx   0        0        0        0 2024-05-12 10:25:09.444533 kitab-0.0.26/
+-rw-rw-rw-   0        0        0     1100 2024-04-07 17:53:03.000000 kitab-0.0.26/LICENSE
+-rw-rw-rw-   0        0        0     6212 2024-05-12 10:25:09.434761 kitab-0.0.26/PKG-INFO
+-rw-rw-rw-   0        0        0     5602 2024-05-12 10:23:37.000000 kitab-0.0.26/README.md
+drwxrwxrwx   0        0        0        0 2024-05-12 10:25:09.318653 kitab-0.0.26/kitab/
+-rw-rw-rw-   0        0        0      131 2024-04-08 06:51:45.000000 kitab-0.0.26/kitab/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-12 10:25:09.383859 kitab-0.0.26/kitab/api/
+-rw-rw-rw-   0        0        0        0 2024-04-07 17:53:03.000000 kitab-0.0.26/kitab/api/__init__.py
+-rw-rw-rw-   0        0        0     8126 2024-05-12 10:22:02.000000 kitab-0.0.26/kitab/api/app.py
+drwxrwxrwx   0        0        0        0 2024-05-12 10:25:09.404101 kitab-0.0.26/kitab/db/
+-rw-rw-rw-   0        0        0      416 2024-04-26 08:05:03.000000 kitab-0.0.26/kitab/db/__init__.py
+-rw-rw-rw-   0        0        0      232 2024-05-07 05:22:41.000000 kitab-0.0.26/kitab/db/db_credentials.py
+-rw-rw-rw-   0        0        0     1836 2024-04-25 20:34:46.000000 kitab-0.0.26/kitab/db/db_info.py
+-rw-rw-rw-   0        0        0    20768 2024-05-10 10:10:49.000000 kitab-0.0.26/kitab/db/functions.py
+-rw-rw-rw-   0        0        0     6825 2024-04-26 09:12:48.000000 kitab-0.0.26/kitab/db/get_data.py
+-rw-rw-rw-   0        0        0    16160 2024-05-03 14:12:28.000000 kitab-0.0.26/kitab/db/sql_interactions.py
+drwxrwxrwx   0        0        0        0 2024-05-12 10:25:09.413947 kitab-0.0.26/kitab/logger/
+-rw-rw-rw-   0        0        0       37 2024-04-07 17:53:03.000000 kitab-0.0.26/kitab/logger/__init__.py
+-rw-rw-rw-   0        0        0     1812 2024-04-25 18:53:05.000000 kitab-0.0.26/kitab/logger/logger.py
+drwxrwxrwx   0        0        0        0 2024-05-12 10:25:09.417577 kitab-0.0.26/kitab/recommendation_model/
+-rw-rw-rw-   0        0        0       88 2024-04-08 13:12:13.000000 kitab-0.0.26/kitab/recommendation_model/__init__.py
+-rw-rw-rw-   0        0        0     5162 2024-05-03 14:37:05.000000 kitab-0.0.26/kitab/recommendation_model/models.py
+-rw-rw-rw-   0        0        0     6366 2024-05-12 10:18:08.000000 kitab-0.0.26/kitab/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-12 10:25:09.434761 kitab-0.0.26/kitab.egg-info/
+-rw-rw-rw-   0        0        0     6212 2024-05-12 10:25:09.000000 kitab-0.0.26/kitab.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      550 2024-05-12 10:25:09.000000 kitab-0.0.26/kitab.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-12 10:25:09.000000 kitab-0.0.26/kitab.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       78 2024-05-12 10:25:09.000000 kitab-0.0.26/kitab.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-12 10:25:09.000000 kitab-0.0.26/kitab.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-12 10:25:09.445200 kitab-0.0.26/setup.cfg
+-rw-rw-rw-   0        0        0     1053 2024-05-12 10:24:36.000000 kitab-0.0.26/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-12 10:25:09.429329 kitab-0.0.26/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-07 17:53:03.000000 kitab-0.0.26/tests/test_module1.py
+-rw-rw-rw-   0        0        0        0 2024-04-07 17:53:03.000000 kitab-0.0.26/tests/test_module2.py
```

### Comparing `kitab-0.0.25/LICENSE` & `kitab-0.0.26/LICENSE`

 * *Files identical despite different names*

### Comparing `kitab-0.0.25/PKG-INFO` & `kitab-0.0.26/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kitab
-Version: 0.0.25
+Version: 0.0.26
 Summary: A package for book recommendation.
 Author: Alexander Shahramanyan, Anna Charchyan, Yeva Manukyan, Lilith Asminian, Maria Petrosyan
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -140,10 +140,18 @@
 
 ```{python}
 from kitab.recommendation_model.models import recommend_books_by_title
 
 recommend_books_by_title(title="The Ghostly Rental", n=5)
 ```
 
-Find full documentation [here](https://alexshah1.github.io/ds223-book-recommendation/).
+### API
+We have also implemented an API that can be used to interact with the model and the database. You can find information on API endpoints and how to use them in the documentation. To run the API, run the following:
+
+```{python}
+from kitab.api.app import run_api
+run_api(port=5552)
+```
+
+Find the full documentation [here](https://alexshah1.github.io/ds223-book-recommendation/).
 
 © 2024 Team 8, DS 223 Marketing Analytics, AUA
```

### Comparing `kitab-0.0.25/README.md` & `kitab-0.0.26/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -122,10 +122,18 @@
 
 ```{python}
 from kitab.recommendation_model.models import recommend_books_by_title
 
 recommend_books_by_title(title="The Ghostly Rental", n=5)
 ```
 
-Find full documentation [here](https://alexshah1.github.io/ds223-book-recommendation/).
+### API
+We have also implemented an API that can be used to interact with the model and the database. You can find information on API endpoints and how to use them in the documentation. To run the API, run the following:
+
+```{python}
+from kitab.api.app import run_api
+run_api(port=5552)
+```
+
+Find the full documentation [here](https://alexshah1.github.io/ds223-book-recommendation/).
 
 © 2024 Team 8, DS 223 Marketing Analytics, AUA
```

### Comparing `kitab-0.0.25/kitab/api/app.py` & `kitab-0.0.26/kitab/api/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from ..db.functions import get_book_by_ISBN, get_book_by_title, add_book_db, update_book_db, add_recommendation_log, get_history_by_recommendation_isbn
 from ..recommendation_model.models import recommend_books, recommend_books_by_ISBN, recommend_books_by_title
 from fastapi import FastAPI
 from pydantic import BaseModel
 import uvicorn
 import logging
 from ..logger.logger import CustomFormatter
+import uvicorn
 
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.DEBUG)
 ch = logging.StreamHandler()
 ch.setLevel(logging.DEBUG)
 ch.setFormatter(CustomFormatter())
 logger.addHandler(ch)
@@ -250,9 +251,22 @@
     # If book isn't in the database, add it
     if add_recommendation_log(description, recommendation_isbn, successful):
         return {"message": "Log successfully added."}
     
     return {"message": "Something went wrong. Log not added."}
 
 
-if __name__ == "__main__":
-    uvicorn.run(app, host="localhost")
+def run_api(port=5552) -> None:
+    """
+    Run the API server.
+    
+    Examples:
+        >>> from kitab.utils import run_api
+        >>> run_api(port=5552)
+    
+    Parameters:
+    port (int): The port number on which the API server will run.
+    
+    Returns:
+    None
+    """
+    uvicorn.run(app, port=port)
```

### Comparing `kitab-0.0.25/kitab/db/db_info.py` & `kitab-0.0.26/kitab/db/db_info.py`

 * *Files identical despite different names*

### Comparing `kitab-0.0.25/kitab/db/functions.py` & `kitab-0.0.26/kitab/db/functions.py`

 * *Files identical despite different names*

### Comparing `kitab-0.0.25/kitab/db/get_data.py` & `kitab-0.0.26/kitab/db/get_data.py`

 * *Files identical despite different names*

### Comparing `kitab-0.0.25/kitab/db/sql_interactions.py` & `kitab-0.0.26/kitab/db/sql_interactions.py`

 * *Files identical despite different names*

### Comparing `kitab-0.0.25/kitab/logger/logger.py` & `kitab-0.0.26/kitab/logger/logger.py`

 * *Files identical despite different names*

### Comparing `kitab-0.0.25/kitab/recommendation_model/models.py` & `kitab-0.0.26/kitab/recommendation_model/models.py`

 * *Files identical despite different names*

### Comparing `kitab-0.0.25/kitab/utils.py` & `kitab-0.0.26/kitab/utils.py`

 * *Files identical despite different names*

### Comparing `kitab-0.0.25/kitab.egg-info/PKG-INFO` & `kitab-0.0.26/kitab.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kitab
-Version: 0.0.25
+Version: 0.0.26
 Summary: A package for book recommendation.
 Author: Alexander Shahramanyan, Anna Charchyan, Yeva Manukyan, Lilith Asminian, Maria Petrosyan
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -140,10 +140,18 @@
 
 ```{python}
 from kitab.recommendation_model.models import recommend_books_by_title
 
 recommend_books_by_title(title="The Ghostly Rental", n=5)
 ```
 
-Find full documentation [here](https://alexshah1.github.io/ds223-book-recommendation/).
+### API
+We have also implemented an API that can be used to interact with the model and the database. You can find information on API endpoints and how to use them in the documentation. To run the API, run the following:
+
+```{python}
+from kitab.api.app import run_api
+run_api(port=5552)
+```
+
+Find the full documentation [here](https://alexshah1.github.io/ds223-book-recommendation/).
 
 © 2024 Team 8, DS 223 Marketing Analytics, AUA
```

### Comparing `kitab-0.0.25/kitab.egg-info/SOURCES.txt` & `kitab-0.0.26/kitab.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kitab-0.0.25/setup.py` & `kitab-0.0.26/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 # Add install requirements
 setup(
     author="Alexander Shahramanyan, Anna Charchyan, Yeva Manukyan, Lilith Asminian, Maria Petrosyan",
     description="A package for book recommendation.",
     name="kitab",
     packages=find_packages(include=["kitab", "kitab.*"]),
-    version="0.0.25",
+    version="0.0.26",
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
     install_requires=['pandas', 'sentence-transformers>=2.6', 'psycopg2-binary', 'pgvector', 'python-dotenv', 'tqdm'],
     python_requires=">=3.9",
```

