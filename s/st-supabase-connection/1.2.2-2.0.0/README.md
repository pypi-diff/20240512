# Comparing `tmp/st-supabase-connection-1.2.2.tar.gz` & `tmp/st_supabase_connection-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "st-supabase-connection-1.2.2.tar", last modified: Sat Dec  9 15:45:46 2023, max compression
+gzip compressed data, was "st_supabase_connection-2.0.0.tar", last modified: Sun May 12 11:47:01 2024, max compression
```

## Comparing `st-supabase-connection-1.2.2.tar` & `st_supabase_connection-2.0.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 15:45:45.999281 st-supabase-connection-1.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2023-12-09 15:45:38.000000 st-supabase-connection-1.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       34 2023-12-09 15:45:38.000000 st-supabase-connection-1.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    17574 2023-12-09 15:45:45.999281 st-supabase-connection-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    16326 2023-12-09 15:45:38.000000 st-supabase-connection-1.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-09 15:45:45.999281 st-supabase-connection-1.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1980 2023-12-09 15:45:38.000000 st-supabase-connection-1.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 15:45:45.995281 st-supabase-connection-1.2.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 15:45:45.995281 st-supabase-connection-1.2.2/src/st_supabase_connection/
--rw-r--r--   0 runner    (1001) docker     (127)    17821 2023-12-09 15:45:38.000000 st-supabase-connection-1.2.2/src/st_supabase_connection/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 15:45:45.999281 st-supabase-connection-1.2.2/src/st_supabase_connection.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    17574 2023-12-09 15:45:45.000000 st-supabase-connection-1.2.2/src/st_supabase_connection.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      326 2023-12-09 15:45:45.000000 st-supabase-connection-1.2.2/src/st_supabase_connection.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-09 15:45:45.000000 st-supabase-connection-1.2.2/src/st_supabase_connection.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2023-12-09 15:45:45.000000 st-supabase-connection-1.2.2/src/st_supabase_connection.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2023-12-09 15:45:45.000000 st-supabase-connection-1.2.2/src/st_supabase_connection.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:47:01.684188 st_supabase_connection-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-12 11:46:54.000000 st_supabase_connection-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-12 11:46:54.000000 st_supabase_connection-2.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    17742 2024-05-12 11:47:01.684188 st_supabase_connection-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    16494 2024-05-12 11:46:54.000000 st_supabase_connection-2.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 11:47:01.684188 st_supabase_connection-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-05-12 11:46:54.000000 st_supabase_connection-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:47:01.680188 st_supabase_connection-2.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:47:01.680188 st_supabase_connection-2.0.0/src/st_supabase_connection/
+-rw-r--r--   0 runner    (1001) docker     (127)    18244 2024-05-12 11:46:54.000000 st_supabase_connection-2.0.0/src/st_supabase_connection/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:47:01.684188 st_supabase_connection-2.0.0/src/st_supabase_connection.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    17742 2024-05-12 11:47:01.000000 st_supabase_connection-2.0.0/src/st_supabase_connection.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-12 11:47:01.000000 st_supabase_connection-2.0.0/src/st_supabase_connection.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 11:47:01.000000 st_supabase_connection-2.0.0/src/st_supabase_connection.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-12 11:47:01.000000 st_supabase_connection-2.0.0/src/st_supabase_connection.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-12 11:47:01.000000 st_supabase_connection-2.0.0/src/st_supabase_connection.egg-info/top_level.txt
```

### Comparing `st-supabase-connection-1.2.2/LICENSE` & `st_supabase_connection-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `st-supabase-connection-1.2.2/PKG-INFO` & `st_supabase_connection-2.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: st-supabase-connection
-Version: 1.2.2
+Version: 2.0.0
 Summary: A Streamlit connection component for Supabase.
 Home-page: https://github.com/SiddhantSadangi/st_supabase_connection
 Author: Siddhant Sadangi
 Author-email: siddhant.sadangi@gmail.com
 Project-URL: Homepage, https://github.com/SiddhantSadangi/st_supabase_connection
 Project-URL: Documentation, https://github.com/SiddhantSadangi/st_supabase_connection/blob/main/README.md
 Project-URL: Funding, https://www.buymeacoffee.com/siddhantsadangi
@@ -182,27 +182,27 @@
 > [!NOTE]  
 > For local development outside Streamlit, you can also set these as your environment variables (recommended), or pass these to the `url` and `key` args of `st.connection()`.
 
 ## :magic_wand: Usage
 
 1. Import
   ```python
-  from st_supabase_connection import SupabaseConnection
+  from st_supabase_connection import SupabaseConnection, execute_query
   ```
 2. Initialize
   ```python
   st_supabase_client = st.connection(
       name="YOUR_CONNECTION_NAME",
       type=SupabaseConnection,
       ttl=None,
       url="YOUR_SUPABASE_URL", # not needed if provided as a streamlit secret
       key="YOUR_SUPABASE_KEY", # not needed if provided as a streamlit secret
   )
   ```
-3. Use in your app to query tables and files. Happy Streamlit-ing! :balloon:
+3. Use in your app to query tables and files, and add authentication. Happy Streamlit-ing! :balloon:
 
 ## :ok_hand: Supported methods
 <details close>
 <summary> Storage </summary>
 <ul>
     <li> <code>delete_bucket()</code> </li>
     <li> <code>empty_bucket()</code> </li>
@@ -221,15 +221,15 @@
 </ul> 
 
 </details>
 
 <details close>
 <summary> Database </summary>
 <ul>
-    <li> <code>query()</code> - Runs a cached SELECT query </li>
+    <li> <code>execute_query()</code> - Executes the passed query with caching enabled. </li>
     <li> All methods supported by <a href="https://postgrest-py.readthedocs.io/en/latest/api/request_builders.html">postgrest-py</a>.
 </details>
 
 <details>
 <summary> Auth </summary>
 <ul>
     All methods supported by <a href="https://supabase.com/docs/reference/python/auth-signup">Supabase's Python API </a>.
@@ -324,40 +324,45 @@
 ```python
 >>> st_supabase_client.delete_bucket("new_bucket")
 {'message': 'Successfully deleted'}
 ```
 ### :file_cabinet: Database operations
 #### Simple query 
 ```python
->>> st_supabase_client.query("*", table="countries", ttl=0).execute()
+>>> execute_query(st_supabase_client.table("countries").select("*"), ttl=0)
 APIResponse(
     data=[
         {"id": 1, "name": "Afghanistan"},
         {"id": 2, "name": "Albania"},
         {"id": 3, "name": "Algeria"},
     ],
     count=None,
 )
 ```
 #### Query with join
 ```python
->>> st_supabase_client.query("name, teams(name)", table="users",  count="exact", ttl="1h").execute()
+>>> execute_query(
+        st_supabase_client.table("users").select("name, teams(name)", count="exact"), 
+        ttl="1h",
+    )
+    
 APIResponse(
     data=[
         {"name": "Kiran", "teams": [{"name": "Green"}, {"name": "Blue"}]},
         {"name": "Evan", "teams": [{"name": "Blue"}]},
     ],
-    count=None,
+    count=2,
 )
 ```
 #### Filter through foreign tables
 ```python
->>> st_supabase_client.query("name, countries(*)", count="exact", table="cities", ttl=None).eq(
-        "countries.name", "Curaçao"
-    ).execute()
+>>> execute_query(
+        st_supabase_client.table("cities").select("name, countries(*)", count="exact").eq("countries.name", "Curaçao"),
+        ttl=None,
+    )
 
 APIResponse(
     data=[
         {
             "name": "Kralendijk",
             "countries": {
                 "id": 2,
@@ -372,17 +377,21 @@
     ],
     count=2,
 )
 ```
 
 #### Insert rows
 ```python
->>> st_supabase_client.table("countries").insert(
-        [{"name": "Wakanda", "iso2": "WK"}, {"name": "Wadiya", "iso2": "WD"}], count="None"
-    ).execute()
+>>> execute_query(
+        st_supabase_client.table("countries").insert(
+            [{"name": "Wakanda", "iso2": "WK"}, {"name": "Wadiya", "iso2": "WD"}], count="None"
+        ),
+        ttl=0,
+    )
+    
 APIResponse(
     data=[
         {
             "id": 250,
             "name": "Wakanda",
             "iso2": "WK",
             "iso3": None,
```

### Comparing `st-supabase-connection-1.2.2/README.md` & `st_supabase_connection-2.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -154,27 +154,27 @@
 > [!NOTE]  
 > For local development outside Streamlit, you can also set these as your environment variables (recommended), or pass these to the `url` and `key` args of `st.connection()`.
 
 ## :magic_wand: Usage
 
 1. Import
   ```python
-  from st_supabase_connection import SupabaseConnection
+  from st_supabase_connection import SupabaseConnection, execute_query
   ```
 2. Initialize
   ```python
   st_supabase_client = st.connection(
       name="YOUR_CONNECTION_NAME",
       type=SupabaseConnection,
       ttl=None,
       url="YOUR_SUPABASE_URL", # not needed if provided as a streamlit secret
       key="YOUR_SUPABASE_KEY", # not needed if provided as a streamlit secret
   )
   ```
-3. Use in your app to query tables and files. Happy Streamlit-ing! :balloon:
+3. Use in your app to query tables and files, and add authentication. Happy Streamlit-ing! :balloon:
 
 ## :ok_hand: Supported methods
 <details close>
 <summary> Storage </summary>
 <ul>
     <li> <code>delete_bucket()</code> </li>
     <li> <code>empty_bucket()</code> </li>
@@ -193,15 +193,15 @@
 </ul> 
 
 </details>
 
 <details close>
 <summary> Database </summary>
 <ul>
-    <li> <code>query()</code> - Runs a cached SELECT query </li>
+    <li> <code>execute_query()</code> - Executes the passed query with caching enabled. </li>
     <li> All methods supported by <a href="https://postgrest-py.readthedocs.io/en/latest/api/request_builders.html">postgrest-py</a>.
 </details>
 
 <details>
 <summary> Auth </summary>
 <ul>
     All methods supported by <a href="https://supabase.com/docs/reference/python/auth-signup">Supabase's Python API </a>.
@@ -296,40 +296,45 @@
 ```python
 >>> st_supabase_client.delete_bucket("new_bucket")
 {'message': 'Successfully deleted'}
 ```
 ### :file_cabinet: Database operations
 #### Simple query 
 ```python
->>> st_supabase_client.query("*", table="countries", ttl=0).execute()
+>>> execute_query(st_supabase_client.table("countries").select("*"), ttl=0)
 APIResponse(
     data=[
         {"id": 1, "name": "Afghanistan"},
         {"id": 2, "name": "Albania"},
         {"id": 3, "name": "Algeria"},
     ],
     count=None,
 )
 ```
 #### Query with join
 ```python
->>> st_supabase_client.query("name, teams(name)", table="users",  count="exact", ttl="1h").execute()
+>>> execute_query(
+        st_supabase_client.table("users").select("name, teams(name)", count="exact"), 
+        ttl="1h",
+    )
+    
 APIResponse(
     data=[
         {"name": "Kiran", "teams": [{"name": "Green"}, {"name": "Blue"}]},
         {"name": "Evan", "teams": [{"name": "Blue"}]},
     ],
-    count=None,
+    count=2,
 )
 ```
 #### Filter through foreign tables
 ```python
->>> st_supabase_client.query("name, countries(*)", count="exact", table="cities", ttl=None).eq(
-        "countries.name", "Curaçao"
-    ).execute()
+>>> execute_query(
+        st_supabase_client.table("cities").select("name, countries(*)", count="exact").eq("countries.name", "Curaçao"),
+        ttl=None,
+    )
 
 APIResponse(
     data=[
         {
             "name": "Kralendijk",
             "countries": {
                 "id": 2,
@@ -344,17 +349,21 @@
     ],
     count=2,
 )
 ```
 
 #### Insert rows
 ```python
->>> st_supabase_client.table("countries").insert(
-        [{"name": "Wakanda", "iso2": "WK"}, {"name": "Wadiya", "iso2": "WD"}], count="None"
-    ).execute()
+>>> execute_query(
+        st_supabase_client.table("countries").insert(
+            [{"name": "Wakanda", "iso2": "WK"}, {"name": "Wadiya", "iso2": "WD"}], count="None"
+        ),
+        ttl=0,
+    )
+    
 APIResponse(
     data=[
         {
             "id": 250,
             "name": "Wakanda",
             "iso2": "WK",
             "iso3": None,
```

### Comparing `st-supabase-connection-1.2.2/setup.py` & `st_supabase_connection-2.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `st-supabase-connection-1.2.2/src/st_supabase_connection/__init__.py` & `st_supabase_connection-2.0.0/src/st_supabase_connection/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 import mimetypes
 import os
 import urllib
 from datetime import timedelta
 from io import BytesIO
 from pathlib import Path
-from typing import Literal, Optional, Tuple, Union, types
+from typing import Literal, Optional, Tuple, Union
 
-from postgrest import SyncSelectRequestBuilder, types
+from postgrest import (
+    APIResponse,
+    SyncFilterRequestBuilder,
+    SyncQueryRequestBuilder,
+    SyncSelectRequestBuilder,
+)
 from streamlit import cache_data, cache_resource
 from streamlit.connections import BaseConnection
 from supabase import Client, create_client
 
-__version__ = "1.2.2"
+__version__ = "2.0.0"
 
 
 class SupabaseConnection(BaseConnection[Client]):
     """
     Connects a streamlit app to Supabase Storage and Database
 
     Attributes
@@ -62,41 +67,14 @@
 
         self.client = create_client(url, key)
         self.table = self.client.table
         self.auth = self.client.auth
         self.delete_bucket = self.client.storage.delete_bucket
         self.empty_bucket = self.client.storage.empty_bucket
 
-    def query(
-        self,
-        *columns: str,
-        table: str,
-        count: Optional[types.CountMethod] = None,
-        ttl: Optional[Union[float, timedelta, str]] = None,
-    ) -> SyncSelectRequestBuilder:
-        """Run a SELECT query.
-
-        Parameters
-        ----------
-        *columns : str
-            The names of the columns to fetch.
-        table : str
-            The table to run the query on.
-        count : str
-            The method to use to get the count of rows returned. Defaults to `None`.
-        ttl : float, timedelta, str, or None
-            The maximum time to keep an entry in the cache. Defaults to `None` (cache never expires).
-        """
-
-        @cache_resource(ttl=ttl)
-        def _query(_self, *columns, table, count):
-            return _self.client.table(table).select(*columns, count=count)
-
-        return _query(self, *columns, table=table, count=count)
-
     def get_bucket(
         self,
         bucket_id: str,
         ttl: Optional[Union[float, timedelta, str]] = None,
     ):
         """Retrieves the details of an existing storage bucket.
 
@@ -497,7 +475,42 @@
                 response = self.client.storage.from_(bucket_id)._request(
                     "PUT",
                     final_url,
                     files=_file,
                 )
 
         return response.json()
+
+
+def execute_query(
+    query: Union[SyncSelectRequestBuilder, SyncQueryRequestBuilder, SyncFilterRequestBuilder],
+    ttl: Optional[Union[float, timedelta, str]] = None,
+) -> APIResponse:
+    """Execute the query.
+    This function is a wrapper around the `query.execute()` method, with caching enabled.
+    This works with all types of queries, but caching may lead to unexpected results when running DML queries.
+
+    It is recommended to set `ttl` to 0 for DML queries (insert, update, upsert, delete) to avoid caching issues.
+
+    Parameters
+    ----------
+    query : SyncSelectRequestBuilder, SyncQueryRequestBuilder, SyncFilterRequestBuilder
+        The query to execute. Can contain any number of chained filters and operators.
+    ttl : float, timedelta, str, or None
+        The maximum time to keep an entry in the cache. Defaults to `None` (cache never expires).
+    """
+
+    def _hash_func(x):
+        return hash(x.path + str(x.params))
+
+    @cache_resource(
+        ttl=ttl,
+        hash_funcs={
+            SyncSelectRequestBuilder: _hash_func,
+            SyncQueryRequestBuilder: _hash_func,
+            SyncFilterRequestBuilder: _hash_func,
+        },
+    )
+    def _execute(query):
+        return query.execute()
+
+    return _execute(query)
```

### Comparing `st-supabase-connection-1.2.2/src/st_supabase_connection.egg-info/PKG-INFO` & `st_supabase_connection-2.0.0/src/st_supabase_connection.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: st-supabase-connection
-Version: 1.2.2
+Version: 2.0.0
 Summary: A Streamlit connection component for Supabase.
 Home-page: https://github.com/SiddhantSadangi/st_supabase_connection
 Author: Siddhant Sadangi
 Author-email: siddhant.sadangi@gmail.com
 Project-URL: Homepage, https://github.com/SiddhantSadangi/st_supabase_connection
 Project-URL: Documentation, https://github.com/SiddhantSadangi/st_supabase_connection/blob/main/README.md
 Project-URL: Funding, https://www.buymeacoffee.com/siddhantsadangi
@@ -182,27 +182,27 @@
 > [!NOTE]  
 > For local development outside Streamlit, you can also set these as your environment variables (recommended), or pass these to the `url` and `key` args of `st.connection()`.
 
 ## :magic_wand: Usage
 
 1. Import
   ```python
-  from st_supabase_connection import SupabaseConnection
+  from st_supabase_connection import SupabaseConnection, execute_query
   ```
 2. Initialize
   ```python
   st_supabase_client = st.connection(
       name="YOUR_CONNECTION_NAME",
       type=SupabaseConnection,
       ttl=None,
       url="YOUR_SUPABASE_URL", # not needed if provided as a streamlit secret
       key="YOUR_SUPABASE_KEY", # not needed if provided as a streamlit secret
   )
   ```
-3. Use in your app to query tables and files. Happy Streamlit-ing! :balloon:
+3. Use in your app to query tables and files, and add authentication. Happy Streamlit-ing! :balloon:
 
 ## :ok_hand: Supported methods
 <details close>
 <summary> Storage </summary>
 <ul>
     <li> <code>delete_bucket()</code> </li>
     <li> <code>empty_bucket()</code> </li>
@@ -221,15 +221,15 @@
 </ul> 
 
 </details>
 
 <details close>
 <summary> Database </summary>
 <ul>
-    <li> <code>query()</code> - Runs a cached SELECT query </li>
+    <li> <code>execute_query()</code> - Executes the passed query with caching enabled. </li>
     <li> All methods supported by <a href="https://postgrest-py.readthedocs.io/en/latest/api/request_builders.html">postgrest-py</a>.
 </details>
 
 <details>
 <summary> Auth </summary>
 <ul>
     All methods supported by <a href="https://supabase.com/docs/reference/python/auth-signup">Supabase's Python API </a>.
@@ -324,40 +324,45 @@
 ```python
 >>> st_supabase_client.delete_bucket("new_bucket")
 {'message': 'Successfully deleted'}
 ```
 ### :file_cabinet: Database operations
 #### Simple query 
 ```python
->>> st_supabase_client.query("*", table="countries", ttl=0).execute()
+>>> execute_query(st_supabase_client.table("countries").select("*"), ttl=0)
 APIResponse(
     data=[
         {"id": 1, "name": "Afghanistan"},
         {"id": 2, "name": "Albania"},
         {"id": 3, "name": "Algeria"},
     ],
     count=None,
 )
 ```
 #### Query with join
 ```python
->>> st_supabase_client.query("name, teams(name)", table="users",  count="exact", ttl="1h").execute()
+>>> execute_query(
+        st_supabase_client.table("users").select("name, teams(name)", count="exact"), 
+        ttl="1h",
+    )
+    
 APIResponse(
     data=[
         {"name": "Kiran", "teams": [{"name": "Green"}, {"name": "Blue"}]},
         {"name": "Evan", "teams": [{"name": "Blue"}]},
     ],
-    count=None,
+    count=2,
 )
 ```
 #### Filter through foreign tables
 ```python
->>> st_supabase_client.query("name, countries(*)", count="exact", table="cities", ttl=None).eq(
-        "countries.name", "Curaçao"
-    ).execute()
+>>> execute_query(
+        st_supabase_client.table("cities").select("name, countries(*)", count="exact").eq("countries.name", "Curaçao"),
+        ttl=None,
+    )
 
 APIResponse(
     data=[
         {
             "name": "Kralendijk",
             "countries": {
                 "id": 2,
@@ -372,17 +377,21 @@
     ],
     count=2,
 )
 ```
 
 #### Insert rows
 ```python
->>> st_supabase_client.table("countries").insert(
-        [{"name": "Wakanda", "iso2": "WK"}, {"name": "Wadiya", "iso2": "WD"}], count="None"
-    ).execute()
+>>> execute_query(
+        st_supabase_client.table("countries").insert(
+            [{"name": "Wakanda", "iso2": "WK"}, {"name": "Wadiya", "iso2": "WD"}], count="None"
+        ),
+        ttl=0,
+    )
+    
 APIResponse(
     data=[
         {
             "id": 250,
             "name": "Wakanda",
             "iso2": "WK",
             "iso3": None,
```

