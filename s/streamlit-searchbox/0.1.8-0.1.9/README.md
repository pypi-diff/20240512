# Comparing `tmp/streamlit-searchbox-0.1.8.tar.gz` & `tmp/streamlit-searchbox-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit-searchbox-0.1.8.tar", last modified: Sun Mar 17 16:08:22 2024, max compression
+gzip compressed data, was "streamlit-searchbox-0.1.9.tar", last modified: Mon Apr 15 05:11:55 2024, max compression
```

## Comparing `streamlit-searchbox-0.1.8.tar` & `streamlit-searchbox-0.1.9.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 wrzr       (501) staff       (20)        0 2024-03-17 16:08:22.593387 streamlit-searchbox-0.1.8/
--rw-rw-r--   0 wrzr       (501) staff       (20)     1063 2022-04-12 22:00:53.000000 streamlit-searchbox-0.1.8/LICENSE
--rw-rw-r--   0 wrzr       (501) staff       (20)       55 2022-05-29 16:47:35.000000 streamlit-searchbox-0.1.8/MANIFEST.in
--rw-r--r--   0 wrzr       (501) staff       (20)      410 2024-03-17 16:08:22.593206 streamlit-searchbox-0.1.8/PKG-INFO
--rw-r--r--   0 wrzr       (501) staff       (20)     2535 2024-03-17 15:27:24.000000 streamlit-searchbox-0.1.8/README.md
--rw-r--r--   0 wrzr       (501) staff       (20)      868 2024-02-02 18:10:07.000000 streamlit-searchbox-0.1.8/pyproject.toml
--rw-r--r--   0 wrzr       (501) staff       (20)       38 2024-03-17 16:08:22.593429 streamlit-searchbox-0.1.8/setup.cfg
--rw-r--r--   0 wrzr       (501) staff       (20)      867 2024-03-17 15:40:33.000000 streamlit-searchbox-0.1.8/setup.py
-drwxr-xr-x   0 wrzr       (501) staff       (20)        0 2024-03-17 16:08:22.588119 streamlit-searchbox-0.1.8/streamlit_searchbox/
--rw-r--r--   0 wrzr       (501) staff       (20)     6240 2024-03-17 16:02:07.000000 streamlit-searchbox-0.1.8/streamlit_searchbox/__init__.py
-drwxr-xr-x   0 wrzr       (501) staff       (20)        0 2024-03-17 16:08:22.586818 streamlit-searchbox-0.1.8/streamlit_searchbox/frontend/
-drwxr-xr-x   0 wrzr       (501) staff       (20)        0 2024-03-17 16:08:22.589382 streamlit-searchbox-0.1.8/streamlit_searchbox/frontend/build/
--rw-r--r--   0 wrzr       (501) staff       (20)      415 2024-03-17 16:07:51.000000 streamlit-searchbox-0.1.8/streamlit_searchbox/frontend/build/asset-manifest.json
--rw-r--r--   0 wrzr       (501) staff       (20)   197406 2024-03-17 16:07:46.000000 streamlit-searchbox-0.1.8/streamlit_searchbox/frontend/build/bootstrap.min.css
--rw-r--r--   0 wrzr       (501) staff       (20)      492 2024-03-17 16:07:51.000000 streamlit-searchbox-0.1.8/streamlit_searchbox/frontend/build/index.html
-drwxr-xr-x   0 wrzr       (501) staff       (20)        0 2024-03-17 16:08:22.587014 streamlit-searchbox-0.1.8/streamlit_searchbox/frontend/build/static/
-drwxr-xr-x   0 wrzr       (501) staff       (20)        0 2024-03-17 16:08:22.589972 streamlit-searchbox-0.1.8/streamlit_searchbox/frontend/build/static/js/
--rw-r--r--   0 wrzr       (501) staff       (20)   406849 2024-03-17 16:07:51.000000 streamlit-searchbox-0.1.8/streamlit_searchbox/frontend/build/static/js/main.48ab4925.js
--rw-r--r--   0 wrzr       (501) staff       (20)     1293 2024-03-17 16:07:51.000000 streamlit-searchbox-0.1.8/streamlit_searchbox/frontend/build/static/js/main.48ab4925.js.LICENSE.txt
--rw-r--r--   0 wrzr       (501) staff       (20)  1419424 2024-03-17 16:07:51.000000 streamlit-searchbox-0.1.8/streamlit_searchbox/frontend/build/static/js/main.48ab4925.js.map
-drwxr-xr-x   0 wrzr       (501) staff       (20)        0 2024-03-17 16:08:22.591112 streamlit-searchbox-0.1.8/streamlit_searchbox/frontend/build/static/media/
--rw-r--r--   0 wrzr       (501) staff       (20)      276 2024-03-17 16:07:51.000000 streamlit-searchbox-0.1.8/streamlit_searchbox/frontend/build/static/media/st-arrow.cec31a87db5bef89b72042f6dfae9845.svg
--rw-r--r--   0 wrzr       (501) staff       (20)      750 2024-03-17 16:07:51.000000 streamlit-searchbox-0.1.8/streamlit_searchbox/frontend/build/static/media/st-clear.6e2f7cc05ea4a1c4fe780ea30d5d82a2.svg
-drwxr-xr-x   0 wrzr       (501) staff       (20)        0 2024-03-17 16:08:22.588875 streamlit-searchbox-0.1.8/streamlit_searchbox.egg-info/
--rw-r--r--   0 wrzr       (501) staff       (20)      410 2024-03-17 16:08:22.000000 streamlit-searchbox-0.1.8/streamlit_searchbox.egg-info/PKG-INFO
--rw-r--r--   0 wrzr       (501) staff       (20)      921 2024-03-17 16:08:22.000000 streamlit-searchbox-0.1.8/streamlit_searchbox.egg-info/SOURCES.txt
--rw-r--r--   0 wrzr       (501) staff       (20)        1 2024-03-17 16:08:22.000000 streamlit-searchbox-0.1.8/streamlit_searchbox.egg-info/dependency_links.txt
--rw-r--r--   0 wrzr       (501) staff       (20)      102 2024-03-17 16:08:22.000000 streamlit-searchbox-0.1.8/streamlit_searchbox.egg-info/requires.txt
--rw-r--r--   0 wrzr       (501) staff       (20)       26 2024-03-17 16:08:22.000000 streamlit-searchbox-0.1.8/streamlit_searchbox.egg-info/top_level.txt
-drwxr-xr-x   0 wrzr       (501) staff       (20)        0 2024-03-17 16:08:22.592708 streamlit-searchbox-0.1.8/tests/
--rw-r--r--   0 wrzr       (501) staff       (20)        0 2024-02-02 18:10:07.000000 streamlit-searchbox-0.1.8/tests/__init__.py
--rw-r--r--   0 wrzr       (501) staff       (20)     4363 2024-02-02 18:10:17.000000 streamlit-searchbox-0.1.8/tests/playwright.py
--rw-r--r--   0 wrzr       (501) staff       (20)     1615 2024-02-02 18:10:07.000000 streamlit-searchbox-0.1.8/tests/test_conversion.py
--rw-r--r--   0 wrzr       (501) staff       (20)     3499 2024-02-02 18:10:07.000000 streamlit-searchbox-0.1.8/tests/utils.py
+drwxr-xr-x   0 wrzr       (501) staff       (20)        0 2024-04-15 05:11:55.459833 streamlit-searchbox-0.1.9/
+-rw-rw-r--   0 wrzr       (501) staff       (20)     1063 2022-04-12 22:00:53.000000 streamlit-searchbox-0.1.9/LICENSE
+-rw-rw-r--   0 wrzr       (501) staff       (20)       55 2022-05-29 16:47:35.000000 streamlit-searchbox-0.1.9/MANIFEST.in
+-rw-r--r--   0 wrzr       (501) staff       (20)      410 2024-04-15 05:11:55.459668 streamlit-searchbox-0.1.9/PKG-INFO
+-rw-r--r--   0 wrzr       (501) staff       (20)     2535 2024-03-17 16:18:03.000000 streamlit-searchbox-0.1.9/README.md
+-rw-r--r--   0 wrzr       (501) staff       (20)      868 2024-02-02 18:10:07.000000 streamlit-searchbox-0.1.9/pyproject.toml
+-rw-r--r--   0 wrzr       (501) staff       (20)       38 2024-04-15 05:11:55.459875 streamlit-searchbox-0.1.9/setup.cfg
+-rw-r--r--   0 wrzr       (501) staff       (20)      867 2024-04-15 05:08:50.000000 streamlit-searchbox-0.1.9/setup.py
+drwxr-xr-x   0 wrzr       (501) staff       (20)        0 2024-04-15 05:11:55.452701 streamlit-searchbox-0.1.9/streamlit_searchbox/
+-rw-r--r--   0 wrzr       (501) staff       (20)     6268 2024-04-15 05:08:11.000000 streamlit-searchbox-0.1.9/streamlit_searchbox/__init__.py
+drwxr-xr-x   0 wrzr       (501) staff       (20)        0 2024-04-15 05:11:55.451361 streamlit-searchbox-0.1.9/streamlit_searchbox/frontend/
+drwxr-xr-x   0 wrzr       (501) staff       (20)        0 2024-04-15 05:11:55.454481 streamlit-searchbox-0.1.9/streamlit_searchbox/frontend/build/
+-rw-r--r--   0 wrzr       (501) staff       (20)      415 2024-04-15 05:09:41.000000 streamlit-searchbox-0.1.9/streamlit_searchbox/frontend/build/asset-manifest.json
+-rw-r--r--   0 wrzr       (501) staff       (20)   197406 2024-04-15 05:09:37.000000 streamlit-searchbox-0.1.9/streamlit_searchbox/frontend/build/bootstrap.min.css
+-rw-r--r--   0 wrzr       (501) staff       (20)      492 2024-04-15 05:09:41.000000 streamlit-searchbox-0.1.9/streamlit_searchbox/frontend/build/index.html
+drwxr-xr-x   0 wrzr       (501) staff       (20)        0 2024-04-15 05:11:55.451557 streamlit-searchbox-0.1.9/streamlit_searchbox/frontend/build/static/
+drwxr-xr-x   0 wrzr       (501) staff       (20)        0 2024-04-15 05:11:55.456061 streamlit-searchbox-0.1.9/streamlit_searchbox/frontend/build/static/js/
+-rw-r--r--   0 wrzr       (501) staff       (20)   406849 2024-04-15 05:09:41.000000 streamlit-searchbox-0.1.9/streamlit_searchbox/frontend/build/static/js/main.48ab4925.js
+-rw-r--r--   0 wrzr       (501) staff       (20)     1293 2024-04-15 05:09:41.000000 streamlit-searchbox-0.1.9/streamlit_searchbox/frontend/build/static/js/main.48ab4925.js.LICENSE.txt
+-rw-r--r--   0 wrzr       (501) staff       (20)  1419424 2024-04-15 05:09:41.000000 streamlit-searchbox-0.1.9/streamlit_searchbox/frontend/build/static/js/main.48ab4925.js.map
+drwxr-xr-x   0 wrzr       (501) staff       (20)        0 2024-04-15 05:11:55.458058 streamlit-searchbox-0.1.9/streamlit_searchbox/frontend/build/static/media/
+-rw-r--r--   0 wrzr       (501) staff       (20)      276 2024-04-15 05:09:41.000000 streamlit-searchbox-0.1.9/streamlit_searchbox/frontend/build/static/media/st-arrow.cec31a87db5bef89b72042f6dfae9845.svg
+-rw-r--r--   0 wrzr       (501) staff       (20)      750 2024-04-15 05:09:41.000000 streamlit-searchbox-0.1.9/streamlit_searchbox/frontend/build/static/media/st-clear.6e2f7cc05ea4a1c4fe780ea30d5d82a2.svg
+drwxr-xr-x   0 wrzr       (501) staff       (20)        0 2024-04-15 05:11:55.453376 streamlit-searchbox-0.1.9/streamlit_searchbox.egg-info/
+-rw-r--r--   0 wrzr       (501) staff       (20)      410 2024-04-15 05:11:55.000000 streamlit-searchbox-0.1.9/streamlit_searchbox.egg-info/PKG-INFO
+-rw-r--r--   0 wrzr       (501) staff       (20)      921 2024-04-15 05:11:55.000000 streamlit-searchbox-0.1.9/streamlit_searchbox.egg-info/SOURCES.txt
+-rw-r--r--   0 wrzr       (501) staff       (20)        1 2024-04-15 05:11:55.000000 streamlit-searchbox-0.1.9/streamlit_searchbox.egg-info/dependency_links.txt
+-rw-r--r--   0 wrzr       (501) staff       (20)      102 2024-04-15 05:11:55.000000 streamlit-searchbox-0.1.9/streamlit_searchbox.egg-info/requires.txt
+-rw-r--r--   0 wrzr       (501) staff       (20)       26 2024-04-15 05:11:55.000000 streamlit-searchbox-0.1.9/streamlit_searchbox.egg-info/top_level.txt
+drwxr-xr-x   0 wrzr       (501) staff       (20)        0 2024-04-15 05:11:55.459349 streamlit-searchbox-0.1.9/tests/
+-rw-r--r--   0 wrzr       (501) staff       (20)        0 2024-02-02 18:10:07.000000 streamlit-searchbox-0.1.9/tests/__init__.py
+-rw-r--r--   0 wrzr       (501) staff       (20)     4363 2024-02-02 18:10:17.000000 streamlit-searchbox-0.1.9/tests/playwright.py
+-rw-r--r--   0 wrzr       (501) staff       (20)     1615 2024-02-02 18:10:07.000000 streamlit-searchbox-0.1.9/tests/test_conversion.py
+-rw-r--r--   0 wrzr       (501) staff       (20)     3499 2024-02-02 18:10:07.000000 streamlit-searchbox-0.1.9/tests/utils.py
```

### Comparing `streamlit-searchbox-0.1.8/LICENSE` & `streamlit-searchbox-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit-searchbox-0.1.8/README.md` & `streamlit-searchbox-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `streamlit-searchbox-0.1.8/pyproject.toml` & `streamlit-searchbox-0.1.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `streamlit-searchbox-0.1.8/setup.py` & `streamlit-searchbox-0.1.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="streamlit-searchbox",
-    version="0.1.8",
+    version="0.1.9",
     author="m-wrzr",
     description="Autocomplete Searchbox",
     long_description="Streamlit searchbox that dynamically updates "
     + "and provides a list of suggestions based on a provided function",
     long_description_content_type="text/plain",
     url="https://github.com/m-wrzr/streamlit-searchbox",
     packages=setuptools.find_packages(),
```

### Comparing `streamlit-searchbox-0.1.8/streamlit_searchbox/__init__.py` & `streamlit-searchbox-0.1.9/streamlit_searchbox/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,21 +74,22 @@
 
 
 def _process_search(
     search_function: Callable[[str], List[Any]],
     key: str,
     searchterm: str,
     rerun_on_update: bool,
+    kwargs: dict[str, Any],
 ) -> None:
     # nothing changed, avoid new search
     if searchterm == st.session_state[key]["search"]:
         return st.session_state[key]["result"]
 
     st.session_state[key]["search"] = searchterm
-    search_results = search_function(searchterm)
+    search_results = search_function(searchterm, **kwargs)
 
     if search_results is None:
         search_results = []
 
     st.session_state[key]["options_js"] = _list_to_options_js(search_results)
     st.session_state[key]["options_py"] = _list_to_options_py(search_results)
 
@@ -166,25 +167,24 @@
         options=st.session_state[key]["options_js"],
         clear_on_submit=clear_on_submit,
         placeholder=placeholder,
         label=label,
         edit_after_submit=edit_after_submit,
         # react return state within streamlit session_state
         key=st.session_state[key]["key_react"],
-        **kwargs,
     )
 
     if react_state is None:
         return st.session_state[key]["result"]
 
     interaction, value = react_state["interaction"], react_state["value"]
 
     if interaction == "search":
         # triggers rerun, no ops afterwards executed
-        _process_search(search_function, key, value, rerun_on_update)
+        _process_search(search_function, key, value, rerun_on_update, kwargs)
 
     if interaction == "submit":
         st.session_state[key]["result"] = (
             st.session_state[key]["options_py"][value]
             if "options_py" in st.session_state[key]
             else value
         )
```

### Comparing `streamlit-searchbox-0.1.8/streamlit_searchbox/frontend/build/bootstrap.min.css` & `streamlit-searchbox-0.1.9/streamlit_searchbox/frontend/build/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `streamlit-searchbox-0.1.8/streamlit_searchbox/frontend/build/static/js/main.48ab4925.js` & `streamlit-searchbox-0.1.9/streamlit_searchbox/frontend/build/static/js/main.48ab4925.js`

 * *Files identical despite different names*

### Comparing `streamlit-searchbox-0.1.8/streamlit_searchbox/frontend/build/static/js/main.48ab4925.js.LICENSE.txt` & `streamlit-searchbox-0.1.9/streamlit_searchbox/frontend/build/static/js/main.48ab4925.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit-searchbox-0.1.8/streamlit_searchbox/frontend/build/static/js/main.48ab4925.js.map` & `streamlit-searchbox-0.1.9/streamlit_searchbox/frontend/build/static/js/main.48ab4925.js.map`

 * *Files identical despite different names*

### Comparing `streamlit-searchbox-0.1.8/streamlit_searchbox/frontend/build/static/media/st-clear.6e2f7cc05ea4a1c4fe780ea30d5d82a2.svg` & `streamlit-searchbox-0.1.9/streamlit_searchbox/frontend/build/static/media/st-clear.6e2f7cc05ea4a1c4fe780ea30d5d82a2.svg`

 * *Files identical despite different names*

### Comparing `streamlit-searchbox-0.1.8/streamlit_searchbox.egg-info/SOURCES.txt` & `streamlit-searchbox-0.1.9/streamlit_searchbox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `streamlit-searchbox-0.1.8/tests/playwright.py` & `streamlit-searchbox-0.1.9/tests/playwright.py`

 * *Files identical despite different names*

### Comparing `streamlit-searchbox-0.1.8/tests/test_conversion.py` & `streamlit-searchbox-0.1.9/tests/test_conversion.py`

 * *Files identical despite different names*

### Comparing `streamlit-searchbox-0.1.8/tests/utils.py` & `streamlit-searchbox-0.1.9/tests/utils.py`

 * *Files identical despite different names*

