# Comparing `tmp/snapquery-0.0.8.tar.gz` & `tmp/snapquery-0.0.9.tar.gz`

## Comparing `snapquery-0.0.8.tar` & `snapquery-0.0.9.tar`

### file list

```diff
@@ -1,42 +1,46 @@
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 snapquery-0.0.8/.project
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 snapquery-0.0.8/.pydevproject
--rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 snapquery-0.0.8/snapquery.puml
--rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 snapquery-0.0.8/.github/workflows/build.yml
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 snapquery-0.0.8/.github/workflows/upload-to-pypi.yml
--rwxr-xr-x   0        0        0      120 2020-02-02 00:00:00.000000 snapquery-0.0.8/scripts/blackisort
--rwxr-xr-x   0        0        0       42 2020-02-02 00:00:00.000000 snapquery-0.0.8/scripts/install
--rwxr-xr-x   0        0        0      586 2020-02-02 00:00:00.000000 snapquery-0.0.8/scripts/restore_db
--rwxr-xr-x   0        0        0      147 2020-02-02 00:00:00.000000 snapquery-0.0.8/scripts/test
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 snapquery-0.0.8/snapquery/__init__.py
--rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 snapquery-0.0.8/snapquery/error_filter.py
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 snapquery-0.0.8/snapquery/mwlogin.py
--rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 snapquery-0.0.8/snapquery/params_view.py
--rw-r--r--   0        0        0     2933 2020-02-02 00:00:00.000000 snapquery-0.0.8/snapquery/qimport.py
--rw-r--r--   0        0        0     2870 2020-02-02 00:00:00.000000 snapquery-0.0.8/snapquery/qimport_view.py
--rw-r--r--   0        0        0     3350 2020-02-02 00:00:00.000000 snapquery-0.0.8/snapquery/scholia.py
--rw-r--r--   0        0        0     4686 2020-02-02 00:00:00.000000 snapquery-0.0.8/snapquery/snapquery_cmd.py
--rw-r--r--   0        0        0    23153 2020-02-02 00:00:00.000000 snapquery-0.0.8/snapquery/snapquery_core.py
--rw-r--r--   0        0        0     7775 2020-02-02 00:00:00.000000 snapquery-0.0.8/snapquery/snapquery_view.py
--rw-r--r--   0        0        0    11121 2020-02-02 00:00:00.000000 snapquery-0.0.8/snapquery/snapquery_webserver.py
--rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 snapquery-0.0.8/snapquery/version.py
--rw-r--r--   0        0        0     3882 2020-02-02 00:00:00.000000 snapquery-0.0.8/snapquery/wd_examples.py
--rw-r--r--   0        0        0    34098 2020-02-02 00:00:00.000000 snapquery-0.0.8/snapquery/samples/ceur-ws.json
--rw-r--r--   0        0        0     7914 2020-02-02 00:00:00.000000 snapquery-0.0.8/snapquery/samples/endpoints.yaml
--rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 snapquery-0.0.8/snapquery/samples/meta_query.yaml
--rw-r--r--   0        0        0   487163 2020-02-02 00:00:00.000000 snapquery-0.0.8/snapquery/samples/scholia.json
--rw-r--r--   0        0        0   280446 2020-02-02 00:00:00.000000 snapquery-0.0.8/snapquery/samples/wikidata-examples.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snapquery-0.0.8/tests/__init__.py
--rw-r--r--   0        0        0     2057 2020-02-02 00:00:00.000000 snapquery-0.0.8/tests/test_cmdline.py
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 snapquery-0.0.8/tests/test_endpoints.py
--rw-r--r--   0        0        0     9431 2020-02-02 00:00:00.000000 snapquery-0.0.8/tests/test_error_filter.py
--rw-r--r--   0        0        0     3036 2020-02-02 00:00:00.000000 snapquery-0.0.8/tests/test_import.py
--rw-r--r--   0        0        0     3275 2020-02-02 00:00:00.000000 snapquery-0.0.8/tests/test_namedqueries.py
--rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 snapquery-0.0.8/tests/test_oauth.py
--rw-r--r--   0        0        0     2134 2020-02-02 00:00:00.000000 snapquery-0.0.8/tests/test_restful_api.py
--rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 snapquery-0.0.8/tests/test_scholia.py
--rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 snapquery-0.0.8/tests/test_wd_query_parsing.py
--rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 snapquery-0.0.8/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 snapquery-0.0.8/LICENSE
--rw-r--r--   0        0        0     9293 2020-02-02 00:00:00.000000 snapquery-0.0.8/README.md
--rw-r--r--   0        0        0     2187 2020-02-02 00:00:00.000000 snapquery-0.0.8/pyproject.toml
--rw-r--r--   0        0        0    10798 2020-02-02 00:00:00.000000 snapquery-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 snapquery-0.0.9/.project
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 snapquery-0.0.9/.pydevproject
+-rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 snapquery-0.0.9/snapquery.puml
+-rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 snapquery-0.0.9/.github/workflows/build.yml
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 snapquery-0.0.9/.github/workflows/upload-to-pypi.yml
+-rwxr-xr-x   0        0        0      120 2020-02-02 00:00:00.000000 snapquery-0.0.9/scripts/blackisort
+-rwxr-xr-x   0        0        0       42 2020-02-02 00:00:00.000000 snapquery-0.0.9/scripts/install
+-rwxr-xr-x   0        0        0      586 2020-02-02 00:00:00.000000 snapquery-0.0.9/scripts/restore_db
+-rwxr-xr-x   0        0        0      147 2020-02-02 00:00:00.000000 snapquery-0.0.9/scripts/test
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 snapquery-0.0.9/snapquery/__init__.py
+-rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 snapquery-0.0.9/snapquery/error_filter.py
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 snapquery-0.0.9/snapquery/mwlogin.py
+-rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 snapquery-0.0.9/snapquery/params_view.py
+-rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 snapquery-0.0.9/snapquery/qimport.py
+-rw-r--r--   0        0        0     2830 2020-02-02 00:00:00.000000 snapquery-0.0.9/snapquery/qimport_view.py
+-rw-r--r--   0        0        0     3351 2020-02-02 00:00:00.000000 snapquery-0.0.9/snapquery/scholia.py
+-rw-r--r--   0        0        0     6677 2020-02-02 00:00:00.000000 snapquery-0.0.9/snapquery/snapquery_cmd.py
+-rw-r--r--   0        0        0    30526 2020-02-02 00:00:00.000000 snapquery-0.0.9/snapquery/snapquery_core.py
+-rw-r--r--   0        0        0    11191 2020-02-02 00:00:00.000000 snapquery-0.0.9/snapquery/snapquery_view.py
+-rw-r--r--   0        0        0    11094 2020-02-02 00:00:00.000000 snapquery-0.0.9/snapquery/snapquery_webserver.py
+-rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 snapquery-0.0.9/snapquery/version.py
+-rw-r--r--   0        0        0     3882 2020-02-02 00:00:00.000000 snapquery-0.0.9/snapquery/wd_examples.py
+-rw-r--r--   0        0        0     6663 2020-02-02 00:00:00.000000 snapquery-0.0.9/snapquery/wd_short_url.py
+-rw-r--r--   0        0        0    34098 2020-02-02 00:00:00.000000 snapquery-0.0.9/snapquery/samples/ceur-ws.json
+-rw-r--r--   0        0        0     7914 2020-02-02 00:00:00.000000 snapquery-0.0.9/snapquery/samples/endpoints.yaml
+-rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 snapquery-0.0.9/snapquery/samples/meta_query.yaml
+-rw-r--r--   0        0        0   487163 2020-02-02 00:00:00.000000 snapquery-0.0.9/snapquery/samples/scholia.json
+-rw-r--r--   0        0        0   280446 2020-02-02 00:00:00.000000 snapquery-0.0.9/snapquery/samples/wikidata-examples.json
+-rw-r--r--   0        0        0    96356 2020-02-02 00:00:00.000000 snapquery-0.0.9/snapquery/samples/wikidata-short-urls.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snapquery-0.0.9/tests/__init__.py
+-rw-r--r--   0        0        0     2246 2020-02-02 00:00:00.000000 snapquery-0.0.9/tests/test_cmdline.py
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 snapquery-0.0.9/tests/test_endpoints.py
+-rw-r--r--   0        0        0    17162 2020-02-02 00:00:00.000000 snapquery-0.0.9/tests/test_error_filter.py
+-rw-r--r--   0        0        0     3056 2020-02-02 00:00:00.000000 snapquery-0.0.9/tests/test_import.py
+-rw-r--r--   0        0        0     3352 2020-02-02 00:00:00.000000 snapquery-0.0.9/tests/test_namedqueries.py
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 snapquery-0.0.9/tests/test_oauth.py
+-rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 snapquery-0.0.9/tests/test_query_execution.py
+-rw-r--r--   0        0        0     2134 2020-02-02 00:00:00.000000 snapquery-0.0.9/tests/test_restful_api.py
+-rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 snapquery-0.0.9/tests/test_scholia.py
+-rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 snapquery-0.0.9/tests/test_wd_query_parsing.py
+-rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 snapquery-0.0.9/tests/test_wd_short_url.py
+-rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 snapquery-0.0.9/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 snapquery-0.0.9/LICENSE
+-rw-r--r--   0        0        0     9293 2020-02-02 00:00:00.000000 snapquery-0.0.9/README.md
+-rw-r--r--   0        0        0     2210 2020-02-02 00:00:00.000000 snapquery-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0    10829 2020-02-02 00:00:00.000000 snapquery-0.0.9/PKG-INFO
```

### Comparing `snapquery-0.0.8/snapquery.puml` & `snapquery-0.0.9/snapquery.puml`

 * *Files identical despite different names*

### Comparing `snapquery-0.0.8/.github/workflows/build.yml` & `snapquery-0.0.9/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `snapquery-0.0.8/.github/workflows/upload-to-pypi.yml` & `snapquery-0.0.9/.github/workflows/upload-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `snapquery-0.0.8/scripts/restore_db` & `snapquery-0.0.9/scripts/restore_db`

 * *Files identical despite different names*

### Comparing `snapquery-0.0.8/snapquery/error_filter.py` & `snapquery-0.0.9/snapquery/error_filter.py`

 * *Files 21% similar despite different names*

```diff
@@ -12,38 +12,59 @@
     """
 
     def __init__(self, raw_error_message: str):
         self.raw_error_message = raw_error_message
         self.filtered_message = self._extract_relevant_info()
 
     def _extract_relevant_info(self) -> str:
-        # Extract SPARQL query if present
+        """
+        Extract relevant information from the given raw error message.
+        Identifies and processes different error message formats.
+        """
+        if not self.raw_error_message:
+            return None
+
+        if "SPARQL-QUERY:" in self.raw_error_message:
+            return self._extract_sparql_error()
+        elif "Not supported:" in self.raw_error_message:
+            return self._extract_qlever_error()
+        else:
+            return "Error: Unrecognized error format."
+
+    def _extract_sparql_error(self) -> str:
+        """
+        Specifically extract and format SPARQL error messages.
+        """
         sparql_start_token = "SPARQL-QUERY:"
         sparql_end_token = "java.util.concurrent.ExecutionException"
-
-        # Extract the malformed query
         sparql_start_idx = self.raw_error_message.find(sparql_start_token)
         sparql_end_idx = self.raw_error_message.find(sparql_end_token)
 
         if sparql_start_idx != -1 and sparql_end_idx != -1:
             sparql_query = self.raw_error_message[sparql_start_idx:sparql_end_idx]
             sparql_query = sparql_query.replace("SPARQL-QUERY:", "").strip()
+            return f"Query error in SPARQL:\n{sparql_query}"
         else:
-            sparql_query = "SPARQL query not found."
-
-        # Find and include error message
-        error_summary = "Query error: A bad request was sent to the endpoint, possibly due to a malformed SPARQL query."
-
-        # Combine error message and SPARQL query
-        filtered_message = f"{error_summary}\n\nMalformed Query:\n{sparql_query}"
+            return "Error: SPARQL query information is incomplete."
 
-        return filtered_message
+    def _extract_qlever_error(self) -> str:
+        """
+        Specifically extract and format QLever error messages.
+        """
+        start_idx = self.raw_error_message.find("Not supported:")
+        if start_idx != -1:
+            end_idx = self.raw_error_message.find('}', start_idx)
+            error_message = self.raw_error_message[start_idx:end_idx+1].strip()
+            return f"QLever error:\n{error_message}"
+        else:
+            return "Error: QLever error information is incomplete."
 
     def get_message(self, for_html: bool = True) -> str:
         """
         get the filtered message
         """
         filtered_msg = self.filtered_message
-        if for_html:
-            filtered_msg = filtered_msg.replace("\n", "<br>\n")
-            filtered_msg = filtered_msg.replace("\\n", "<br>\n")
+        if filtered_msg:
+            filtered_msg = filtered_msg.replace("\\n", "\n")
+            if for_html:
+                filtered_msg = filtered_msg.replace("\n", "<br>\n")
         return filtered_msg
```

### Comparing `snapquery-0.0.8/snapquery/mwlogin.py` & `snapquery-0.0.9/snapquery/mwlogin.py`

 * *Files identical despite different names*

### Comparing `snapquery-0.0.8/snapquery/params_view.py` & `snapquery-0.0.9/snapquery/params_view.py`

 * *Files identical despite different names*

### Comparing `snapquery-0.0.8/snapquery/qimport.py` & `snapquery-0.0.9/snapquery/scholia.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,97 +1,104 @@
 """
-Created on 2024-05-05
+Created on 2024-05-04
 
 @author: wf
 """
-import urllib.parse
 
 import requests
-from tqdm import tqdm
-from lodstorage.params import Params
 
-from snapquery.snapquery_core import QueryDetails,NamedQueryList, NamedQueryManager
+from snapquery.snapquery_core import NamedQuery, NamedQueryList, NamedQueryManager
 
 
-class QueryImport:
+class ScholiaQueries:
     """
-    Import named queries from a given URL or file.
+    A class to handle the extraction and management of Scholia queries.
     """
 
-    def __init__(self, nqm: NamedQueryManager = None):
+    repository_url = (
+        "https://api.github.com/repos/WDscholia/scholia/contents/scholia/app/templates"
+    )
+
+    def __init__(self, nqm: NamedQueryManager, debug: bool = False):
         """
         Constructor
 
         Args:
-            nqm (NamedQueryManager, optional): The NamedQueryManager to use for storing queries.
+            nqm (NamedQueryManager): The NamedQueryManager to use for storing queries.
+            debug (bool): Enable debug output. Defaults to False.
         """
         self.nqm = nqm
-        pass
+        self.named_query_list = NamedQueryList(name="scholia")
+        self.debug = debug
+
+    def get_scholia_file_list(self):
+        """
+        Retrieve the list of SPARQL files from the Scholia repository.
 
-    def import_from_json_file(
-        self, json_file: str, with_store: bool = False, show_progress: bool = False
-    ) -> NamedQueryList:
+        Returns:
+            list: List of dictionaries representing file information.
         """
-        Import named queries from a JSON file.
+        headers = {"Accept": "application/vnd.github.v3+json"}
+        response = requests.get(self.repository_url, headers=headers)
+        response.raise_for_status()  # Ensure we notice bad responses
+        return response.json()
+
+    def extract_query(self, file_info) -> NamedQuery:
+        """
+        Extract a single query from file information.
 
         Args:
-            json_file (str): Path to the JSON file.
-            with_store (bool): If True, store the results in the NamedQueryManager.
-            show_progress (bool): If True, show a progress bar during the import.
+            file_info (dict): Dictionary containing information about the file.
 
         Returns:
-            NamedQueryList: A NamedQueryList object containing the imported NamedQuery objects.
+            NamedQuery: The extracted NamedQuery object.
         """
-        nq_list = NamedQueryList.load_from_json_file(json_file)
-        qd_list = []
-        iterable = (
-            tqdm(nq_list.queries, desc="Importing Named Queries")
-            if show_progress
-            else nq_list.queries
-        )
-
-        for nq in iterable:
-            if not nq.sparql and nq.url.startswith("https://w.wiki/"):
-                nq.sparql = self.read_from_short_url(nq.url)
-            params=Params(query=nq.sparql)
-            signature=",".join(params.params) if params.params else None
-            qd=QueryDetails(query_id=nq.query_id,params=signature)
-            qd_list.append(qd)
-            
-
-        if with_store and self.nqm:
-            self.nqm.store_named_query_list(nq_list)
-            self.nqm.store_query_details_list(qd_list)
-
-        return nq_list
+        file_name = file_info["name"]
+        if file_name.endswith(".sparql") and file_name[:-7]:
+            file_response = requests.get(file_info["download_url"])
+            file_response.raise_for_status()
+            query_str = file_response.text
+            name = file_name[:-7]
+            return NamedQuery(
+                namespace="scholia",
+                name=name,
+                url=file_info["download_url"],
+                title=name,
+                sparql=query_str,
+            )
 
-    def read_from_short_url(self, short_url: str) -> str:
+    def extract_queries(self, limit: int = None):
         """
-        Read a query from a short URL.
+        Extract all queries from the Scholia repository.
 
         Args:
-            short_url (str): The short URL from which to read the query.
+            limit (int, optional): Limit the number of queries fetched. Defaults to None.
+        """
+        file_list_json = self.get_scholia_file_list()
+        for i, file_info in enumerate(file_list_json, start=1):
+            named_query = self.extract_query(file_info)
+            if named_query:
+                self.named_query_list.queries.append(named_query)
+                if self.debug:
+                    if i % 80 == 0:
+                        print(f"{i}")
+                    print(".", end="", flush=True)
+                if limit and len(self.named_query_list.queries) >= limit:
+                    break
 
-        Returns:
-            str: The SPARQL query extracted from the short URL.
+        if self.debug:
+            print(f"found {len(self.named_query_list.queries)} scholia queries")
 
-        Raises:
-            Exception: If there's an error fetching or processing the URL.
+    def save_to_json(self, file_path: str = "/tmp/scholia-queries.json"):
         """
-        sparql_query = None
-        try:
-            # Follow the redirection
-            response = requests.head(short_url, allow_redirects=True)
-            redirected_url = response.url
-
-            # Check if the URL has the correct format
-            parsed_url = urllib.parse.urlparse(redirected_url)
-            if (
-                parsed_url.scheme == "https"
-                and parsed_url.netloc == "query.wikidata.org"
-            ):
-                sparql_query = urllib.parse.unquote(parsed_url.fragment)
+        Save the NamedQueryList to a JSON file.
 
-        except Exception as ex:
-            print(f"Error fetching URL: {ex}")
+        Args:
+            file_path (str): Path to the JSON file.
+        """
+        self.named_query_list.save_to_json_file(file_path, indent=2)
 
-        return sparql_query
+    def store_queries(self):
+        """
+        Store the named queries into the database.
+        """
+        self.nqm.store_named_query_list(self.named_query_list)
```

### Comparing `snapquery-0.0.8/snapquery/qimport_view.py` & `snapquery-0.0.9/snapquery/qimport_view.py`

 * *Files 8% similar despite different names*

```diff
@@ -58,17 +58,15 @@
             "name": self.name,
             "title": self.title,
             "url": self.url,
             "description": self.description,
             "sparql": self.query.query,
         }
         nq = NamedQuery.from_record(nq_record)
-        lod = []
-        lod.append(nq_record)
-        self.nqm.store(lod)
+        self.nqm.add_and_store(nq)
         with self.query_row:
             ui.notify(f"added named query {self.name}")
             self.named_query_link.content = nq.as_link()
 
     def on_input_button(self, _args):
         """
         imput a query
```

### Comparing `snapquery-0.0.8/snapquery/snapquery_core.py` & `snapquery-0.0.9/snapquery/snapquery_core.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,40 +4,45 @@
 @author: wf
 """
 import datetime
 import json
 import os
 import re
 import uuid
-from dataclasses import dataclass,field,asdict, is_dataclass
+from dataclasses import asdict, field, fields, is_dataclass
 from pathlib import Path
 from typing import Any, Dict, List, Optional, Type
 
 import requests
 from lodstorage.lod_csv import CSV
+from lodstorage.params import Params
 from lodstorage.query import Endpoint, EndpointManager, Format, Query, QueryManager
 from lodstorage.sparql import SPARQL
 from lodstorage.sql import SQLDB, EntityInfo
 from lodstorage.yamlable import lod_storable
 from ngwidgets.widgets import Link
 
+from snapquery.error_filter import ErrorFilter
+
 
 @lod_storable
 class QueryStats:
     """
     statistics about a query
     """
 
     stats_id: str = field(init=False)
     query_id: str  # foreign key
     endpoint_name: str  # foreign key
+    context:Optional[str] = None # a context for the query stats
     records: Optional[int] = None
     time_stamp: datetime.datetime = field(init=False)
-    duration: float = field(init=False, default=None)  # duration in seconds
+    duration: Optional[float] = field(init=False, default=None)  # duration in seconds
     error_msg: Optional[str] = None
+    filtered_msg: Optional[str] = None
 
     def __post_init__(self):
         """
         Post-initialization processing to construct a unique identifier for the query
         and record the timestamp when the query stats object is created.
         """
         self.stats_id = str(uuid.uuid4())
@@ -45,42 +50,84 @@
 
     def done(self):
         """
         Set the duration by calculating the elapsed time since the `time_stamp`.
         """
         self.duration = (datetime.datetime.now() - self.time_stamp).total_seconds()
 
+    def apply_error_filter(self, for_html: bool = False):
+        error_filter = ErrorFilter(self.error_msg)
+        self.filtered_msg = error_filter.get_message(for_html=for_html)
+
     def error(self, ex: Exception):
         """
         Handle exception of query
         """
         self.duration = None
         self.error_msg = str(ex)
+        self.apply_error_filter()
+
+    @classmethod
+    def from_record(cls, record: Dict) -> "QueryStats":
+        """
+        Class method to instantiate NamedQuery
+        from a dictionary record.
+        """
+        stat = cls(
+                query_id=record.get("query_id", None),
+                endpoint_name=record.get("endpoint_name", None),
+                records=record.get("records", None),
+                error_msg=record.get("error_msg", None),
+        )
+        stat.stats_id = record.get("stats_id", stat.stats_id)
+        stat.time_stamp = record.get("time_stamp", stat.time_stamp)
+        stat.duration = record.get("duration", None)
+        return stat
+
+    def as_record(self) -> Dict:
+        """
+        convert my declared attributes to a dict
+        @TODO may be use asdict from dataclasses instead?
+        """
+        record = {}
+        for field in fields(self):
+            # Include field in the record dictionary if it has already been initialized (i.e., not None or has default)
+            if hasattr(self, field.name):
+                record[field.name] = getattr(self, field.name)
+        return record
 
     @classmethod
     def get_samples(cls) -> dict[str, "QueryStats"]:
         """
         get samples
         """
         samples = {
             "snapquery-examples": [
                 QueryStats(
                     query_id="snapquery-examples.cats",
                     endpoint_name="wikidata",
+                    context="samples",
                     records=223,
                     error_msg="",
+                    filtered_msg="",
                 )
             ]
         }
         # Set the duration for each sample instance
         for sample_list in samples.values():
             for sample in sample_list:
                 sample.duration = 0.5
         return samples
 
+    def is_successful(self) -> bool:
+        """
+        Returns True if the query was successful
+        """
+        return self.duration and self.error_msg is None
+
 
 @lod_storable
 class NamedQuery:
     """
     A named query that encapsulates the details and SPARQL query for a specific purpose.
 
     Attributes:
@@ -95,15 +142,15 @@
     query_id: str = field(init=False)
 
     # namespace
     namespace: str
     # name/id
     name: str
     # sparql query (to be hidden later)
-    sparql: Optional[str]=None
+    sparql: Optional[str] = None
     # the url of the source code of the query
     url: Optional[str] = None
     # one line title
     title: Optional[str] = None
     # multiline description
     description: Optional[str] = None
 
@@ -185,14 +232,26 @@
             name=record["name"],
             title=record.get("title"),
             url=record.get("url"),
             description=record.get("description"),
             sparql=record.get("sparql"),
         )
 
+    def as_record(self) -> Dict:
+        record = {
+            "query_id": self.query_id,
+            "namespace": self.namespace,
+            "name": self.name,
+            "url": self.url,
+            "title": self.title,
+            "description": self.description,
+            "sparql": self.sparql,
+        }
+        return record
+
     def as_viewrecord(self) -> Dict:
         """
         Return a dictionary representing the NamedQuery with keys ordered as Name, Namespace, Title, Description.
         """
         url_link = Link.create(self.url, self.url)
         return {
             "name": self.as_link(),
@@ -206,37 +265,90 @@
 class QueryDetails:
     """
     Details for a named query
     """
 
     query_id: str
     params: str
-    
+    param_count: int
+    lines: int
+    size: int
+
+    @classmethod
+    def from_sparql(cls, query_id: str, sparql: str) -> "QueryDetails":
+        """
+        Creates an instance of QueryDetails from a SPARQL query string.
+
+        This method parses the SPARQL query to determine the number of lines and the size of the query.
+        It also identifies and lists the parameters used within the SPARQL query.
+
+        Args:
+            query_id (str): The identifier of the query.
+            sparql (str): The SPARQL query string from which to generate the query details.
+
+        Returns:
+            QueryDetails: An instance containing details about the SPARQL query.
+        """
+        # Calculate the number of lines and the size of the sparql string
+        lines = sparql.count("\n") + 1
+        size = len(sparql.encode("utf-8"))
+
+        # Example to extract parameters - this may need to be replaced with actual parameter extraction logic
+        sparql_params = Params(
+            query=sparql
+        )  # Assuming Params is a class that can parse SPARQL queries to extract parameters
+        params = ",".join(sparql_params.params) if sparql_params.params else None
+        param_count = len(sparql_params.params)
+
+        # Create and return the QueryDetails instance
+        return cls(
+            query_id=query_id,
+            params=params,
+            param_count=param_count,
+            lines=lines,
+            size=size,
+        )
+
     @classmethod
     def get_samples(cls) -> dict[str, "QueryDetails"]:
         """
         get samples
         """
         samples = {
             "snapquery-examples": [
-                QueryDetails(query_id="scholia.test",params="q")
+                QueryDetails(
+                    query_id="scholia.test", params="q", param_count=1, lines=1, size=50
+                )
             ]
         }
         return samples
 
 
 @lod_storable
+class QueryStatsList:
+    """
+    a list of query statistics
+    """
+
+    name: str  # the name of the list
+    stats: List[QueryStats] = field(default_factory=list)
+
+
+@lod_storable
 class NamedQueryList:
     """
     a list of named queries with details
     """
 
     name: str  # the name of the list
     queries: List[NamedQuery] = field(default_factory=list)
 
+    def __len__(self):
+        return len(self.queries)
+
 
 class QueryBundle:
     """
     Bundles a named query, a query, and an endpoint into a single manageable object, facilitating the execution of SPARQL queries.
 
     Attributes:
         named_query (NamedQuery): The named query object, which includes metadata about the query.
@@ -404,14 +516,22 @@
         self.endpoints = EndpointManager.getEndpoints(
             endpointPath=endpoints_path, lang="sparql", with_default=False
         )
         yaml_path = os.path.join(self.samples_path, "meta_query.yaml")
         self.meta_qm = QueryManager(
             queriesPath=yaml_path, with_default=False, lang="sql"
         )
+        # SQL meta data handling
+        # primary keys
+        self.primary_keys = {
+            QueryStats: "stats_id",
+            NamedQuery: "query_id",
+            QueryDetails: "query_id",
+        }
+        self.entity_infos = {}
         pass
 
     @classmethod
     def get_cache_path(cls) -> str:
         home = str(Path.home())
         cache_dir = f"{home}/.solutions/snapquery/storage"
         os.makedirs(cache_dir, exist_ok=True)
@@ -431,21 +551,21 @@
 
         Returns:
             NamedQueryManager: An instance of the manager initialized with the database at `db_path`.
         """
         if db_path is None:
             db_path = cls.get_cache_path()
 
-        nqm = NamedQueryManager(debug=debug)
+        nqm = NamedQueryManager(db_path=db_path, debug=debug)
         path_obj = Path(db_path)
         if not path_obj.exists() or path_obj.stat().st_size == 0:
             for (source_class, pk) in [
                 (NamedQuery, "query_id"),
                 (QueryStats, "stats_id"),
-                (QueryDetails,"quer_id")
+                (QueryDetails, "quer_id"),
             ]:
                 # Fetch sample records from the specified class
                 sample_records = cls.get_sample_records(source_class=source_class)
 
                 # Define entity information dynamically based on the class and primary key
                 entityInfo = EntityInfo(
                     sample_records, name=source_class.__name__, primaryKey=pk
@@ -465,58 +585,109 @@
         Args:
             nq_list: NamedQueryList
         """
         lod = []
         for nq in nq_list.queries:
             lod.append(asdict(nq))
         self.store(lod=lod)
-        
-    def store_query_details_list(self,qd_list:List[QueryDetails]):
-        qd_lod=[]
+
+    def store_query_details_list(self, qd_list: List[QueryDetails]):
+        qd_lod = []
         for qd in qd_list:
             qd_lod.append(asdict(qd))
-        self.store(lod=qd_lod,source_class=QueryDetails,primary_key="query_id")
-        
-    def store_stats(self,stats_list:List[QueryStats]):
+        self.store(lod=qd_lod, source_class=QueryDetails)
+
+    def store_stats(self, stats_list: List[QueryStats]):
         """
         store the given list of query statistics
         """
-        stats_lod=[]
+        stats_lod = []
         for stats in stats_list:
             stats_lod.append(asdict(stats))
-        self.store(lod=stats_lod, source_class=QueryStats, primary_key="stats_id")
+        self.store(lod=stats_lod, source_class=QueryStats)
+
+    def execute_query(
+        self,
+        named_query: NamedQuery,
+        params_dict: Dict,
+        endpoint_name: str = "wikidata",
+        limit: int = None,
+    ):
+        """
+        execute the given named_query
+
+        Args:
+            named_query(NamedQuery): the query to execute
+            params_dict(Dict): the query parameters to apply (if any)
+            endpoint_name(str): the endpoint where to the excute the query
+            limit(int): the record limit for the results (if any)
+        """
+        # Assemble the query bundle using the named query, endpoint, and limit
+        query_bundle = self.as_query_bundle(named_query, endpoint_name, limit)
+        params=Params(query_bundle.query.query)
+        if params.has_params:
+            params.set(params_dict)
+            query=params.apply_parameters()
+            query_bundle.query.query=query
+        # Execute the query
+        results, stats = query_bundle.get_lod_with_stats()
+        self.store_stats([stats])
+        return results, stats
+
+    def add_and_store(self, nq: NamedQuery):
+        """
+        Adds a new NamedQuery instance and stores it in the database.
+
+        Args:
+            nq (NamedQuery): The NamedQuery instance to add and store.
+
+        """
+        qd = QueryDetails.from_sparql(query_id=nq.query_id, sparql=nq.sparql)
+        lod = []
+        nq_record = asdict(nq)
+        lod.append(nq_record)
+        self.store(lod)
+        qd_list = []
+        qd_list.append(qd)
+        self.store_query_details_list(qd_list)
+
+    def get_entity_info(self, source_class: Type) -> EntityInfo:
+        """
+        Gets or creates EntityInfo for the given source class.
+        """
+        if source_class not in self.entity_infos:
+            primary_key = self.primary_keys.get(source_class, None)
+            sample_records = self.get_sample_records(source_class)
+            self.entity_infos[source_class] = EntityInfo(
+                sample_records,
+                name=source_class.__name__,
+                primaryKey=primary_key,
+                debug=self.debug,
+            )
+        return self.entity_infos[source_class]
 
     def store(
         self,
         lod: List[Dict[str, Any]],
         source_class: Type = NamedQuery,
-        primary_key: str = "query_id",
     ) -> None:
         """
         Stores the given list of dictionaries in the database using entity information
         derived from a specified source class.
 
         Args:
             lod (List[Dict[str, Any]]): List of dictionaries that represent the records to be stored.
             source_class (Type): The class from which the entity information is derived. This class
                 should have an attribute or method that defines its primary key and must have a `__name__` attribute.
-            primary_key(str): the primary key to use
         Raises:
             AttributeError: If the source class does not have the necessary method or attribute to define the primary key.
         """
-        # Fetch sample records to define the structure of data and to extract entity information.
-        sample_records = NamedQueryManager.get_sample_records(source_class=source_class)
-
-        # Define entity information based on the source class
-        entityInfo = EntityInfo(
-            sample_records, name=source_class.__name__, primaryKey=primary_key
-        )
-
+        entity_info = self.get_entity_info(source_class)
         # Store the list of dictionaries in the database using the defined entity information
-        self.sql_db.store(lod, entityInfo, fixNone=True, replace=True)
+        self.sql_db.store(lod, entity_info, fixNone=True, replace=True)
 
     @classmethod
     def get_sample_records(cls, source_class: Type) -> List[Dict[str, Any]]:
         """
         Generates a list of dictionary records based on the sample instances
         provided by a source class. This method utilizes the `get_samples` method
         of the source class, which should return a dictionary of sample instances.
@@ -595,40 +766,89 @@
         self,
         name: str,
         namespace: str = "wikidata-examples",
         endpoint_name: str = "wikidata",
         limit: int = None,
     ) -> QueryBundle:
         """
-        get the query for the given parameters
+        Get the query for the given parameters.
 
         Args:
             name (str): The name of the named query to execute.
             namespace (str): The namespace of the named query, default is 'wikidata-examples'.
             endpoint_name (str): The name of the endpoint to send the SPARQL query to, default is 'wikidata'.
-            limit(int): the query limit (if any)
+            limit (int): The query limit (if any).
 
         Returns:
-            QueryBundle: named_query, query and endpoint
+            QueryBundle: named_query, query, and endpoint.
         """
         named_query = self.lookup(name, namespace)
+        return self.as_query_bundle(named_query, endpoint_name, limit)
+
+    def as_query_bundle(
+        self, named_query: NamedQuery, endpoint_name: str, limit: int = None
+    ) -> QueryBundle:
+        """
+        Assembles a QueryBundle from a NamedQuery, endpoint name, and optional limit.
+
+        Args:
+            named_query (NamedQuery): Named query object.
+            endpoint_name (str): Name of the endpoint where the query should be executed.
+            limit (int): Optional limit for the query.
+
+        Returns:
+            QueryBundle: A bundle containing the named query, the query object, and the endpoint.
+        """
         if endpoint_name not in self.endpoints:
-            msg = f"Invalid endpoint {endpoint_name}"
-            ValueError(msg)
-        endpoint = self.endpoints.get(endpoint_name)
-        sparql_query = named_query.sparql
+            raise ValueError(f"Invalid endpoint {endpoint_name}")
+
+        endpoint = self.endpoints[endpoint_name]
         query = Query(
-            name=name,
-            query=sparql_query,
+            name=named_query.name,
+            query=named_query.sparql,
             lang="sparql",
             endpoint=endpoint.endpoint,
             limit=limit,
         )
-        self.endpointConf = self.endpoints.get(endpoint_name, Endpoint.getDefault())
-        query.tryItUrl = query.getTryItUrl(endpoint.website, endpoint.database)
-        query.database = self.endpointConf.database
-        query.query = f"{self.endpointConf.prefixes}\n{query.query}"
-        query_bundle = QueryBundle(
-            named_query=named_query, query=query, endpoint=endpoint
-        )
-        query_bundle.set_limit(limit)
-        return query_bundle
+        query.query = f"{endpoint.prefixes}\n{query.query}"
+        if limit:
+            query.query += f"\nLIMIT {limit}"
+        return QueryBundle(named_query=named_query, query=query, endpoint=endpoint)
+
+    def get_all_queries(self,namespace:str="snapquery-examples") -> List[NamedQuery]:
+        """
+        Retrieves all named queries stored in the database.
+
+        Returns:
+            List[NamedQuery]: A list of all NamedQuery instances in the database.
+        """
+        sql_query = "SELECT * FROM NamedQuery WHERE namespace = ?"
+        query_records = self.sql_db.query(sql_query,(namespace,))
+        named_queries = []
+        for record in query_records:
+            named_query = NamedQuery.from_record(record)
+            named_queries.append(named_query)
+        return named_queries
+
+    def get_query_stats(self, query_id: str) -> list[QueryStats]:
+        """
+        Get query stats for the given query name
+        Args:
+            query_id: id of the query
+
+        Returns:
+            list of query stats
+        """
+        sql_query = f"""
+        SELECT *
+        FROM QueryStats
+        WHERE query_id = ?
+        """
+        query_records = self.sql_db.query(sql_query, (query_id,))
+        stats = []
+        if query_records:
+            for record in query_records:
+                query_stat = QueryStats.from_record(record)
+                stats.append(query_stat)
+        return stats
+
+
```

### Comparing `snapquery-0.0.8/snapquery/snapquery_webserver.py` & `snapquery-0.0.9/snapquery/snapquery_webserver.py`

 * *Files 0% similar despite different names*

```diff
@@ -107,16 +107,16 @@
                 )
             query = self.nqm.meta_qm.queriesByName[name]
             qb = QueryBundle(named_query=None, query=query)
             qlod = self.nqm.sql_db.query(query.query)
             if limit:
                 qlod = qlod[:limit]
             content = qb.format_result(qlod, r_format)
-            #content=content.replace("\n", "<br>\n")
-            if r_format==Format.html:
+            # content=content.replace("\n", "<br>\n")
+            if r_format == Format.html:
                 return HTMLResponse(content)
             return PlainTextResponse(content)
 
         @app.get("/api/sparql/{namespace}/{name}")
         def sparql(
             namespace: str,
             name: str,
@@ -213,17 +213,15 @@
                 str: the content retrieved
         """
         try:
             # content negotiation
             name, r_format = self.get_r_format(name)
             qb = self.nqm.get_query(name, namespace, endpoint_name, limit)
             (qlod, stats) = qb.get_lod_with_stats()
-            self.nqm.store_stats(
-                [stats]
-            )
+            self.nqm.store_stats([stats])
             content = qb.format_result(qlod, r_format)
             return content
         except Exception as e:
             # Handling specific exceptions can be more detailed based on what nqm.get_sparql and nqm.query can raise
             raise HTTPException(status_code=404, detail=str(e))
```

### Comparing `snapquery-0.0.8/snapquery/version.py` & `snapquery-0.0.9/snapquery/version.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     """
     Version handling for nicepdf
     """
 
     name = "snapquery"
     version = snapquery.__version__
     date = "2024-05-03"
-    updated = "2024-05-10"
+    updated = "2024-05-11"
     description = "Introduce Named Queries and Named Query Middleware to wikidata"
 
     authors = "Wolfgang Fahl"
 
     doc_url = "https://wiki.bitplan.com/index.php/snapquery"
     chat_url = "https://github.com/WolfgangFahl/snapquery/discussions"
     cm_url = "https://github.com/WolfgangFahl/snapquery"
```

### Comparing `snapquery-0.0.8/snapquery/wd_examples.py` & `snapquery-0.0.9/snapquery/wd_examples.py`

 * *Files identical despite different names*

### Comparing `snapquery-0.0.8/snapquery/samples/ceur-ws.json` & `snapquery-0.0.9/snapquery/samples/ceur-ws.json`

 * *Files identical despite different names*

### Comparing `snapquery-0.0.8/snapquery/samples/endpoints.yaml` & `snapquery-0.0.9/snapquery/samples/endpoints.yaml`

 * *Files identical despite different names*

### Comparing `snapquery-0.0.8/snapquery/samples/meta_query.yaml` & `snapquery-0.0.9/snapquery/samples/meta_query.yaml`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,35 @@
 # Meta Queries
 # WF 2025-05-06
 'query_count':
     sql: |
       SELECT COUNT(*)
       FROM NamedQuery
+'query_success':
+    sql: |
+        SELECT 
+           COUNT(*) AS count,
+           endpoint_name
+        
+        FROM "QueryStats"
+        WHERE records>0
+        GROUP BY endpoint_name
+        ORDER BY 1 DESC
+'query_success_by_namespace':
+    sql: |
+        SELECT 
+           COUNT(*) AS count,
+           nq.namespace,
+           qs.endpoint_name
+           
+        FROM QueryStats qs
+        JOIN NamedQuery nq on qs.query_id=nq.query_id
+        WHERE records>0
+        GROUP BY endpoint_name,namespace
+        ORDER BY 2 ASC,1 DESC
 'all_queries':
     sql: |
       SELECT * FROM NamedQuery
 'error_histogram':
     sql: |
       SELECT COUNT(*), query_id
       FROM QueryStats
@@ -30,7 +52,21 @@
 'params_stats':
     sql: |
         SELECT count(*),
             params 
         FROM "QueryDetails" 
         GROUP BY params 
         ORDER BY 1 desc
+'query_details_stats':
+    sql: |
+      SELECT 
+        MIN(param_count) AS min_param_count,
+        MAX(param_count) AS max_param_count,
+        AVG(param_count) AS avg_param_count,
+        MIN(lines) AS min_lines,
+        MAX(lines) AS max_lines,
+        AVG(lines) AS avg_lines,
+        MIN(size) AS min_size,
+        MAX(size) AS max_size,
+        AVG(size) AS avg_size
+      FROM 
+        QueryDetails;
```

### Comparing `snapquery-0.0.8/snapquery/samples/scholia.json` & `snapquery-0.0.9/snapquery/samples/scholia.json`

 * *Files identical despite different names*

### Comparing `snapquery-0.0.8/snapquery/samples/wikidata-examples.json` & `snapquery-0.0.9/snapquery/samples/wikidata-examples.json`

 * *Files identical despite different names*

### Comparing `snapquery-0.0.8/tests/test_cmdline.py` & `snapquery-0.0.9/tests/test_cmdline.py`

 * *Files 8% similar despite different names*

```diff
@@ -49,15 +49,25 @@
     def test_namedquery(self):
         """
         test a named query via command line
         """
         limit = 10
 
         def run_cmd():
-            snapquery_cmd.main(["-d", "--namespace", "snapquery-examples", "-qn", "cats", "--limit", f"{limit}"])
+            snapquery_cmd.main(
+                [
+                    "-d",
+                    "--namespace",
+                    "snapquery-examples",
+                    "-qn",
+                    "cats",
+                    "--limit",
+                    f"{limit}",
+                ]
+            )
 
         # Capture the output of running the command
         output = self.capture_stdout(run_cmd)
         if self.debug:
             print(output)
         # Parse the JSON output
         result = json.loads(output)
```

### Comparing `snapquery-0.0.8/tests/test_import.py` & `snapquery-0.0.9/tests/test_import.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,22 +8,23 @@
 import os
 import tempfile
 
 from ngwidgets.basetest import Basetest
 
 from snapquery.qimport import QueryImport
 from snapquery.snapquery_core import NamedQueryManager
+from snapquery.wd_short_url import ShortUrl
 
 
 class TestImport(Basetest):
     """
     test importing  named queries
     """
 
-    def setUp(self, debug=True, profile=True):
+    def setUp(self, debug=False, profile=True):
         Basetest.setUp(self, debug=debug, profile=profile)
 
     def testSamplesImports(self):
         """
         test importing the samples
         """
         with tempfile.NamedTemporaryFile() as tmpfile:
@@ -64,29 +65,28 @@
                     "description": "Map of all CEUR-WS event locations",
                     "url": "https://w.wiki/8gRw",
                 },
             ],
         }
         json_file = "/tmp/sample_ceur-ws_queries.json"
         with open(json_file, "w") as f:
-            json.dump(sample_data, f,indent=2)
+            json.dump(sample_data, f, indent=2)
 
         nq_list = qimport.import_from_json_file(json_file)
-        queries=nq_list.queries
+        queries = nq_list.queries
         for query in queries:
             if self.debug:
                 print(query)
 
         self.assertEqual(len(queries), 2)
         self.assertTrue(any(q.name == "AllVolumes" for q in queries))
         self.assertTrue(any(q.name == "LocationOfEvents" for q in queries))
 
     def testReadFromShortUrl(self):
         """
         test reading from a short url
         """
-        url = "https://w.wiki/6UCU"
-        qimport = QueryImport()
-        query = qimport.read_from_short_url(url)
+        short_url=ShortUrl("https://w.wiki/6UCU")
+        query = short_url.read_query()
         if self.debug:
             print(query)
         self.assertTrue("Q0.1" in query)
```

### Comparing `snapquery-0.0.8/tests/test_namedqueries.py` & `snapquery-0.0.9/tests/test_namedqueries.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,45 +4,43 @@
 @author: wf
 """
 
 import json
 import tempfile
 
 from ngwidgets.basetest import Basetest
-
-from snapquery.snapquery_core import NamedQuery, NamedQueryManager, QueryStats
-
+from snapquery.snapquery_core import NamedQuery, NamedQueryManager
 
 class TestNamedQueryManager(Basetest):
     """
     test the named query Manager
     """
 
     def setUp(self, debug=False, profile=True):
         Basetest.setUp(self, debug=debug, profile=profile)
 
-    def testNamedQueries(self):
+    def test_named_queries(self):
         """
         test getting a named query manager
         """
-        db_path = "/tmp/named_queries.db"
-        nqm = NamedQueryManager.from_samples(db_path=db_path)
-        for name, ex_count in [("x-invalid", -1), ("cats", 205)]:
-            try:
-                query_bundle = nqm.get_query(namespace="snapquery-examples", name=name)
-                lod = query_bundle.get_lod()
-                if self.debug:
-                    print(f"{name}:")
-                    print(json.dumps(lod, default=str, indent=2))
-                self.assertEqual(ex_count, len(lod))
-            except Exception as ex:
-                if self.debug:
-                    print(f"{name}:Exception {str(ex)}")
-                self.assertEqual(-1, ex_count)
-
+        with tempfile.NamedTemporaryFile() as tmpfile:
+            nqm = NamedQueryManager.from_samples(db_path=tmpfile.name)
+            for name, ex_count in [("x-invalid", -1), ("cats", 207)]:
+                try:
+                    query_bundle = nqm.get_query(namespace="snapquery-examples", name=name)
+                    lod = query_bundle.get_lod()
+                    if self.debug:
+                        print(f"{name}:")
+                        print(json.dumps(lod, default=str, indent=2))
+                    self.assertTrue(len(lod)>=ex_count)
+                except Exception as ex:
+                    if self.debug:
+                        print(f"{name}:Exception {str(ex)}")
+                        self.assertEqual(-1, ex_count)
+                
     def test_query_with_stats(self):
         """
         tests executing a query with stats
         """
         with tempfile.NamedTemporaryFile() as tmpfile:
             nqm = NamedQueryManager.from_samples(db_path=tmpfile.name)
             query_bundle = nqm.get_query(namespace="snapquery-examples", name="cats")
```

### Comparing `snapquery-0.0.8/tests/test_oauth.py` & `snapquery-0.0.9/tests/test_oauth.py`

 * *Files identical despite different names*

### Comparing `snapquery-0.0.8/tests/test_restful_api.py` & `snapquery-0.0.9/tests/test_restful_api.py`

 * *Files identical despite different names*

### Comparing `snapquery-0.0.8/tests/test_scholia.py` & `snapquery-0.0.9/tests/test_scholia.py`

 * *Files identical despite different names*

### Comparing `snapquery-0.0.8/tests/test_wd_query_parsing.py` & `snapquery-0.0.9/tests/test_wd_query_parsing.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """
 Created on 2024-05-04
 
 @author: tholzheim
 """
-import json
 import pprint
 import tempfile
 
 from ngwidgets.basetest import Basetest
 
 from snapquery.snapquery_core import NamedQueryManager
 from snapquery.wd_examples import WikidataExamples
@@ -23,15 +22,15 @@
 
     def test_wikidata_examples_query_extraction(self):
         """
         Test extraction and parsing of Wikidata example queries to NamedQueries.
 
         Queries can be found at https://www.wikidata.org/wiki/Wikidata:SPARQL_query_service/queries/examples
         """
-        with tempfile.NamedTemporaryFile() as tmpfile:
+        with tempfile.NamedTemporaryFile(delete=False) as tmpfile:
             nqm = NamedQueryManager.from_samples(db_path=tmpfile.name)
             self.wikidata_examples = WikidataExamples(nqm)
             self.wikidata_examples.extract_queries()
             if self.debug:
                 for query in self.wikidata_examples.named_query_list.queries:
                     pprint.pprint(query)
```

### Comparing `snapquery-0.0.8/.gitignore` & `snapquery-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `snapquery-0.0.8/LICENSE` & `snapquery-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `snapquery-0.0.8/README.md` & `snapquery-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `snapquery-0.0.8/pyproject.toml` & `snapquery-0.0.9/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -18,22 +18,23 @@
 license = {text = "Apache-2.0"}
 
 
 dependencies = [
 	# https://github.com/WolfgangFahl/nicegui_widgets
 	"ngwidgets>=0.15.0",
     # https://pypi.org/project/pyLodStorage/
-    "pyLodStorage>=0.11.3",
+    "pyLodStorage>=0.11.5",
     "wikitextparser",
     "requests",
     # https://pypi.org/project/mwoauth/
     "mwoauth>=0.4.0",
     #"mwoauth@git+https://github.com/mediawiki-utilities/python-mwoauth"
     #https://pypi.org/project/tqdm/
-    "tqdm>=4.66.4"
+    "tqdm>=4.66.4",
+    "nicegui[plotly]"
 ]
 
 requires-python = ">=3.9"
 classifiers=[
     "Development Status :: 4 - Beta",
     "Environment :: Web Environment",
     "Programming Language :: Python :: 3 :: Only",
```

### Comparing `snapquery-0.0.8/PKG-INFO` & `snapquery-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: snapquery
-Version: 0.0.8
+Version: 0.0.9
 Summary: snapquery: Introduce Named Queries and Named Query Middleware to wikidata
 Project-URL: Home, https://github.com/WolfgangFahl/snapquery
 Project-URL: Documentation, https://wiki.bitplan.com/index.php/snapquery
 Project-URL: Source, https://github.com/WolfgangFahl/snapquery
 Author-email: Wolfgang Fahl <wf@WolfgangFahl.com>
 Maintainer-email: Wolfgang Fahl <wf@WolfgangFahl.com>
 License: Apache-2.0
@@ -22,15 +22,16 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: User Interfaces
 Requires-Python: >=3.9
 Requires-Dist: mwoauth>=0.4.0
 Requires-Dist: ngwidgets>=0.15.0
-Requires-Dist: pylodstorage>=0.11.3
+Requires-Dist: nicegui[plotly]
+Requires-Dist: pylodstorage>=0.11.5
 Requires-Dist: requests
 Requires-Dist: tqdm>=4.66.4
 Requires-Dist: wikitextparser
 Provides-Extra: test
 Requires-Dist: green; extra == 'test'
 Description-Content-Type: text/markdown
```

