# Comparing `tmp/drf_api_action-1.2.0.tar.gz` & `tmp/drf_api_action-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drf_api_action-1.2.0.tar", max compression
+gzip compressed data, was "drf_api_action-1.2.1.tar", max compression
```

## Comparing `drf_api_action-1.2.0.tar` & `drf_api_action-1.2.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     4913 2024-04-29 15:06:56.791408 drf_api_action-1.2.0/README.md
--rw-r--r--   0        0        0        0 2023-12-31 11:07:58.025649 drf_api_action-1.2.0/drf_api_action/__init__.py
--rw-r--r--   0        0        0      320 2023-11-27 08:33:36.127871 drf_api_action-1.2.0/drf_api_action/exceptions.py
--rw-r--r--   0        0        0      856 2023-12-30 17:05:16.841747 drf_api_action-1.2.0/drf_api_action/mixins.py
--rw-r--r--   0        0        0     1169 2024-04-29 15:06:56.792375 drf_api_action-1.2.0/drf_api_action/plugin.py
--rw-r--r--   0        0        0     2587 2024-04-29 15:06:56.793606 drf_api_action-1.2.0/drf_api_action/utils.py
--rw-r--r--   0        0        0     5403 2024-04-29 15:06:56.794512 drf_api_action-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     6308 1970-01-01 00:00:00.000000 drf_api_action-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     5663 2024-05-12 10:53:11.221007 drf_api_action-1.2.1/README.md
+-rw-r--r--   0        0        0        0 2023-12-31 11:07:58.025649 drf_api_action-1.2.1/drf_api_action/__init__.py
+-rw-r--r--   0        0        0      320 2023-11-27 08:33:36.127871 drf_api_action-1.2.1/drf_api_action/exceptions.py
+-rw-r--r--   0        0        0      856 2023-12-30 17:05:16.841747 drf_api_action-1.2.1/drf_api_action/mixins.py
+-rw-r--r--   0        0        0     1323 2024-05-12 10:53:11.221807 drf_api_action-1.2.1/drf_api_action/plugin.py
+-rw-r--r--   0        0        0     2910 2024-05-12 10:53:11.222528 drf_api_action-1.2.1/drf_api_action/utils.py
+-rw-r--r--   0        0        0     5403 2024-05-12 10:53:11.223250 drf_api_action-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     7058 1970-01-01 00:00:00.000000 drf_api_action-1.2.1/PKG-INFO
```

### Comparing `drf_api_action-1.2.0/README.md` & `drf_api_action-1.2.1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -2,61 +2,61 @@
 
 [![codecov](https://codecov.io/gh/Ori-Roza/drf-api-action/graph/badge.svg?token=2PB7NG8A4W)](https://codecov.io/gh/Ori-Roza/drf-api-action)
 [![python - 3.8 | 3.9 | 3.10 | 3.11](https://img.shields.io/badge/python-3.8_|_3.9_|_3.10_|_3.11-blue)](https://)[![CI](https://github.com/Ori-Roza/drf-api-action/actions/workflows/tests.yaml/badge.svg?branch=master)](https://github.com/Ori-Roza/drf-api-action/actions/workflows/tests.yaml)
 [![license - MIT](https://img.shields.io/badge/license-MIT-yellow)](https://)
 
 
 The drf-api-action Python package is designed to elevate your testing experience for Django Rest Framework (DRF) REST endpoints.
-With the api-action fixture, this package empowers you to effortlessly test your REST endpoints as if they were conventional functions.
+With the api_action fixture, this package empowers you to effortlessly test your REST endpoints as if they were conventional functions.
 
 Features:
 
-* **Simplified Testing:** Testing DRF REST endpoints using the api-action decorator, treating them like regular functions.
+* **Simplified Testing:** Testing DRF REST endpoints using the api_action plugin, treating them like regular functions.
 
-* **Seamless Integration:** Replacing DRF's action decorator with api-action in your WebViewSet seamlessly.
+* **Seamless Integration:** you don't need to do anything in existing server code.
 
-* **Clear Traceback:** Instead of getting a response with error code, get the real traceback that led to the error.
+* **Easy Debugging:** Instead of getting a response with error code by using default drf testing `client` object , get the real traceback that led to the error.
 
-* **Pagination Support**: Paginating easily through pages by a single kwarg.
+* **Pagination Support**: Paginating easily through pages by using `page` argument.
 
 
 ## Installation
 
 You can install `drf-api-action` using pip:
 
 ```shell
 pip install drf-api-action
 ```
 
 ## Usage
 
 ### To use `drf-api-action` as a Pytest fixture, you need to follow these steps:
 
-#### Step 1: Import the Required Classes and our fixture
+#### Step 1: Import your Viewsets explicitly:
 
 ```python
 import pytest
 from tests.test_server.test_app.models import DummyModel
 from tests.test_server.test_app.views import DummyViewSetFixture
 ```
 
 #### Step 2: use the following action_api mark decorator:
 
-`@pytest.mark.action_api(view_set_class={YOUR VIEW_SET})`
+`@pytest.mark.api_action(view_set_class={YOUR VIEW_SET})`
 
 e.g:
 our ViewSet is called `DummyViewSetFixture`
 
 ```python
 import pytest
 from tests.test_server.test_app.views import DummyViewSetFixture
 
 
-@pytest.mark.action_api(view_set_class=DummyViewSetFixture)
-def test_call_as_api_fixture(db, action_api):
+@pytest.mark.api_action(view_set_class=DummyViewSetFixture)
+def test_call_as_api_fixture(db, api_action):
   pass
 ```
 Now you can use all `DummyViewSetFixture` functionality!
 
 #### Step 3: write your tests
 
 e.g:
@@ -64,32 +64,33 @@
 
 ```python
 import pytest
 from tests.test_server.test_app.models import DummyModel
 from tests.test_server.test_app.views import DummyViewSetFixture
 
 
-@pytest.mark.action_api(view_set_class=DummyViewSetFixture)
-def test_call_as_api_fixture(db, action_api):
+@pytest.mark.api_action(view_set_class=DummyViewSetFixture)
+def test_call_as_api_fixture(db, api_action):
   dummy_model = DummyModel()
   dummy_model.dummy_int = 1
   dummy_model.save()
-  res = action_api.api_dummy(pk=1)
+  res = api_action.api_dummy(pk=1)
   assert res["dummy_int"] == 1
 
 ```
+Here as an example, the real exception and trace will be thrown, make it easy to understand what the issue is:
 
 ```python
 import pytest
 from tests.test_server.test_app.views import DummyViewSetFixture
 
 
-@pytest.mark.action_api(view_set_class=DummyViewSetFixture)
-def test_dummy(db, action_api):
-  result = action_api.dummy(pk='bbb')
+@pytest.mark.api_action(view_set_class=DummyViewSetFixture)
+def test_dummy(db, api_action):
+  result = api_action.dummy(pk='bbb')
   assert result['dummy_int'] == 1
 ```
 
 ```shell
 tests/functionality_tests/test_as_api.py:11 (test_call_as_api)
 self = <django.db.models.fields.BigAutoField: id>, value = 'bb'
 
@@ -113,16 +114,39 @@
         Same as Django's standard shortcut, but make sure to also raise 404
         if the filter_kwargs don't match the required types.
         """
         try:
 >           return _get_object_or_404(queryset, *filter_args, **filter_kwargs)
 
 ../venv/lib/python3.9/site-packages/rest_framework/generics.py:19: 
+....
+....
+...
+```
+
+Call endpoints with pagination:
+```python
+@pytest.mark.api_action(view_set_class=DummyAPIViewSet)
+def test_pagination_data(db, api_action):
+    for i in range(1, 3):
+        dummy_model = DummyModel()
+        dummy_model.dummy_int = 1
+        dummy_model.save()
+
+    response = api_action.by_dummy_int(dummy_int=1, page=1)
+
+    obj = response['results'][0]
+    assert obj['dummy_int'] == 1
+
+    assert extract_page_number(response['next']) == 2
+
+    response = api_action.by_dummy_int(dummy_int=1, page=2)
+    assert extract_page_number(response['previous']) == 1
+    assert extract_page_number(response['next']) is None
 
-and so on....
 ```
 
 
 ## Package Testing
 
 The `drf-api-action` library includes tests to ensure the functionality works as expected. To run the tests run `pytest`:
```

### Comparing `drf_api_action-1.2.0/drf_api_action/mixins.py` & `drf_api_action-1.2.1/drf_api_action/mixins.py`

 * *Files identical despite different names*

### Comparing `drf_api_action-1.2.0/drf_api_action/plugin.py` & `drf_api_action-1.2.1/drf_api_action/plugin.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,36 +2,38 @@
 
 from drf_api_action.utils import run_as_api
 from drf_api_action.exceptions import ActionsAPIException
 
 
 def run_function(self, func):
     def api_item(*args, **kwargs):
+        # here we retrieve serializer_class from @action decorator in order to inject it to the ViewSet
         serializer_class = func.kwargs['serializer_class']
         return run_as_api(self, func, serializer_class, *args, **kwargs)
 
     return api_item
 
 
 @pytest.fixture
-def action_api(request):
+def api_action(request):
     """
     Make Dango WebView endpoints accessible
     """
     from drf_api_action.mixins import APIRestMixin  # pylint: disable=import-outside-toplevel
 
-    if request.keywords['action_api'].kwargs.get("view_set_class") is None:
-        raise ActionsAPIException('using action_api fixture must require a view_set_class kwarg')
+    if request.keywords['api_action'].kwargs.get("view_set_class") is None:
+        raise ActionsAPIException('using api_action fixture must require a view_set_class kwarg')
 
-    view_set_class = request.keywords['action_api'].kwargs["view_set_class"]
+    view_set_class = request.keywords['api_action'].kwargs["view_set_class"]
 
     class WrapperApiClass(APIRestMixin, view_set_class):
         def __getattribute__(self, item):
             class_attribute = super().__getattribute__(item)
 
+            # running our logic on endpoints only
             if callable(class_attribute) and hasattr(class_attribute, 'detail'):
                 return run_function(self, class_attribute)
 
             return class_attribute
 
     api = WrapperApiClass()
     return api
```

### Comparing `drf_api_action-1.2.0/drf_api_action/utils.py` & `drf_api_action-1.2.1/drf_api_action/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,36 +8,38 @@
     """
 
     def __init__(self, data, query_params):
         self.data = data
         self.query_params = query_params
 
     def build_absolute_uri(self, _=None):
+        """
+        mocking django/http/request.py::HTTPRequest::build_absolute_uri
+        It's irrelevant since we do not provide any web resource
+        """
         return ''
 
 
 def run_as_api(self, func, serializer_class, *args, **kw):
-    kw.update({"serializer_class": serializer_class})
+    # adding to the view the request & kwargs including the serializer class
+    kw.update({"serializer_class": serializer_class})  # adding serializer class from @action
+    # decorator into our instance
     request = CustomRequest(kw, kw)
-    self.kwargs = kw
-    self.request = request
+    self.kwargs = kw  # adding our enhanced kwargs into instance kwargs
+    self.request = request  # mocking request with our arguments as data in the instance
 
     try:
-        if hasattr(func, 'detail'):
-            # called from pytest fixture
-            ret = func(request, **kw)
-        else:
-            # called straight from viewer
-            ret = func(self, request, **kw)
+        ret = func(request, **kw)
         if isinstance(ret.data, list):  # multiple results
             results = [dict(res) for res in ret.data]
-        else:
+        else:  # only one json
             results = {k.lower(): v for k, v in ret.data.items()}
     except Exception as error:  # pylint: disable=broad-except
         error_type = type(error)
+        # re-constructing the error with the actual traceback
         raised_exception = ActionsAPIExceptionMiddleware(*error.args,
                                                          error_type=error_type,
                                                          traceback=error.__traceback__)  # fixing stack frames
         raise raised_exception  # pylint: disable=raising-non-exception
 
     return results
```

### Comparing `drf_api_action-1.2.0/pyproject.toml` & `drf_api_action-1.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "drf_api_action"
-version = "1.2.0"
+version = "1.2.1"
 description = "drf-api-action elevates DRF testing by simplifying REST endpoint testing to a seamless, function-like experience."
 readme = "README.md"
 authors = ["Ori Roza <ori75660@gmail.com>"]
 license = "MIT"
 repository = "https://github.com/Ori-Roza/drf-api-action"
 homepage = "https://github.com/Ori-Roza/drf-api-action"
 
@@ -37,15 +37,15 @@
   "Operating System :: OS Independent",
 ]
 
 [tool.pytest.ini_options]
 DJANGO_SETTINGS_MODULE = "tests.test_server.settings"
 python_files = "tests.py test_*.py *_tests.py"
 markers = [
-    "action_api: Viewset"
+    "api_action: Viewset"
 ]
 testpaths = ["tests"]
 
 [tool.poetry.plugins.pytest11]
 api_action = "drf_api_action.plugin"
```

### Comparing `drf_api_action-1.2.0/PKG-INFO` & `drf_api_action-1.2.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drf_api_action
-Version: 1.2.0
+Version: 1.2.1
 Summary: drf-api-action elevates DRF testing by simplifying REST endpoint testing to a seamless, function-like experience.
 Home-page: https://github.com/Ori-Roza/drf-api-action
 License: MIT
 Keywords: pytest,mocks,testing,fixtures,tests,django
 Author: Ori Roza
 Author-email: ori75660@gmail.com
 Requires-Python: >=3.7,<4.0
@@ -34,61 +34,61 @@
 
 [![codecov](https://codecov.io/gh/Ori-Roza/drf-api-action/graph/badge.svg?token=2PB7NG8A4W)](https://codecov.io/gh/Ori-Roza/drf-api-action)
 [![python - 3.8 | 3.9 | 3.10 | 3.11](https://img.shields.io/badge/python-3.8_|_3.9_|_3.10_|_3.11-blue)](https://)[![CI](https://github.com/Ori-Roza/drf-api-action/actions/workflows/tests.yaml/badge.svg?branch=master)](https://github.com/Ori-Roza/drf-api-action/actions/workflows/tests.yaml)
 [![license - MIT](https://img.shields.io/badge/license-MIT-yellow)](https://)
 
 
 The drf-api-action Python package is designed to elevate your testing experience for Django Rest Framework (DRF) REST endpoints.
-With the api-action fixture, this package empowers you to effortlessly test your REST endpoints as if they were conventional functions.
+With the api_action fixture, this package empowers you to effortlessly test your REST endpoints as if they were conventional functions.
 
 Features:
 
-* **Simplified Testing:** Testing DRF REST endpoints using the api-action decorator, treating them like regular functions.
+* **Simplified Testing:** Testing DRF REST endpoints using the api_action plugin, treating them like regular functions.
 
-* **Seamless Integration:** Replacing DRF's action decorator with api-action in your WebViewSet seamlessly.
+* **Seamless Integration:** you don't need to do anything in existing server code.
 
-* **Clear Traceback:** Instead of getting a response with error code, get the real traceback that led to the error.
+* **Easy Debugging:** Instead of getting a response with error code by using default drf testing `client` object , get the real traceback that led to the error.
 
-* **Pagination Support**: Paginating easily through pages by a single kwarg.
+* **Pagination Support**: Paginating easily through pages by using `page` argument.
 
 
 ## Installation
 
 You can install `drf-api-action` using pip:
 
 ```shell
 pip install drf-api-action
 ```
 
 ## Usage
 
 ### To use `drf-api-action` as a Pytest fixture, you need to follow these steps:
 
-#### Step 1: Import the Required Classes and our fixture
+#### Step 1: Import your Viewsets explicitly:
 
 ```python
 import pytest
 from tests.test_server.test_app.models import DummyModel
 from tests.test_server.test_app.views import DummyViewSetFixture
 ```
 
 #### Step 2: use the following action_api mark decorator:
 
-`@pytest.mark.action_api(view_set_class={YOUR VIEW_SET})`
+`@pytest.mark.api_action(view_set_class={YOUR VIEW_SET})`
 
 e.g:
 our ViewSet is called `DummyViewSetFixture`
 
 ```python
 import pytest
 from tests.test_server.test_app.views import DummyViewSetFixture
 
 
-@pytest.mark.action_api(view_set_class=DummyViewSetFixture)
-def test_call_as_api_fixture(db, action_api):
+@pytest.mark.api_action(view_set_class=DummyViewSetFixture)
+def test_call_as_api_fixture(db, api_action):
   pass
 ```
 Now you can use all `DummyViewSetFixture` functionality!
 
 #### Step 3: write your tests
 
 e.g:
@@ -96,32 +96,33 @@
 
 ```python
 import pytest
 from tests.test_server.test_app.models import DummyModel
 from tests.test_server.test_app.views import DummyViewSetFixture
 
 
-@pytest.mark.action_api(view_set_class=DummyViewSetFixture)
-def test_call_as_api_fixture(db, action_api):
+@pytest.mark.api_action(view_set_class=DummyViewSetFixture)
+def test_call_as_api_fixture(db, api_action):
   dummy_model = DummyModel()
   dummy_model.dummy_int = 1
   dummy_model.save()
-  res = action_api.api_dummy(pk=1)
+  res = api_action.api_dummy(pk=1)
   assert res["dummy_int"] == 1
 
 ```
+Here as an example, the real exception and trace will be thrown, make it easy to understand what the issue is:
 
 ```python
 import pytest
 from tests.test_server.test_app.views import DummyViewSetFixture
 
 
-@pytest.mark.action_api(view_set_class=DummyViewSetFixture)
-def test_dummy(db, action_api):
-  result = action_api.dummy(pk='bbb')
+@pytest.mark.api_action(view_set_class=DummyViewSetFixture)
+def test_dummy(db, api_action):
+  result = api_action.dummy(pk='bbb')
   assert result['dummy_int'] == 1
 ```
 
 ```shell
 tests/functionality_tests/test_as_api.py:11 (test_call_as_api)
 self = <django.db.models.fields.BigAutoField: id>, value = 'bb'
 
@@ -145,16 +146,39 @@
         Same as Django's standard shortcut, but make sure to also raise 404
         if the filter_kwargs don't match the required types.
         """
         try:
 >           return _get_object_or_404(queryset, *filter_args, **filter_kwargs)
 
 ../venv/lib/python3.9/site-packages/rest_framework/generics.py:19: 
+....
+....
+...
+```
+
+Call endpoints with pagination:
+```python
+@pytest.mark.api_action(view_set_class=DummyAPIViewSet)
+def test_pagination_data(db, api_action):
+    for i in range(1, 3):
+        dummy_model = DummyModel()
+        dummy_model.dummy_int = 1
+        dummy_model.save()
+
+    response = api_action.by_dummy_int(dummy_int=1, page=1)
+
+    obj = response['results'][0]
+    assert obj['dummy_int'] == 1
+
+    assert extract_page_number(response['next']) == 2
+
+    response = api_action.by_dummy_int(dummy_int=1, page=2)
+    assert extract_page_number(response['previous']) == 1
+    assert extract_page_number(response['next']) is None
 
-and so on....
 ```
 
 
 ## Package Testing
 
 The `drf-api-action` library includes tests to ensure the functionality works as expected. To run the tests run `pytest`:
```

