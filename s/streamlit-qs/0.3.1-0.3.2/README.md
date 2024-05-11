# Comparing `tmp/streamlit-qs-0.3.1.tar.gz` & `tmp/streamlit_qs-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit-qs-0.3.1.tar", last modified: Thu Mar  7 09:45:41 2024, max compression
+gzip compressed data, was "streamlit_qs-0.3.2.tar", last modified: Sat May 11 23:15:47 2024, max compression
```

## Comparing `streamlit-qs-0.3.1.tar` & `streamlit_qs-0.3.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-03-07 09:45:41.165022 streamlit-qs-0.3.1/
--rw-rw-rw-   0        0        0    11357 2023-06-05 05:42:27.000000 streamlit-qs-0.3.1/LICENSE
--rw-rw-rw-   0        0        0     1797 2024-03-07 09:45:41.165022 streamlit-qs-0.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     1219 2024-01-28 06:11:15.000000 streamlit-qs-0.3.1/README.md
--rw-rw-rw-   0        0        0       42 2024-03-07 09:45:41.165022 streamlit-qs-0.3.1/setup.cfg
--rw-rw-rw-   0        0        0      884 2024-03-07 09:43:27.000000 streamlit-qs-0.3.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-07 09:45:41.139277 streamlit-qs-0.3.1/streamlit_qs/
--rw-rw-rw-   0        0        0    29243 2024-03-07 09:43:38.000000 streamlit-qs-0.3.1/streamlit_qs/__init__.py
--rw-rw-rw-   0        0        0        0 2023-06-07 06:37:36.000000 streamlit-qs-0.3.1/streamlit_qs/py.typed
-drwxrwxrwx   0        0        0        0 2024-03-07 09:45:41.162043 streamlit-qs-0.3.1/streamlit_qs.egg-info/
--rw-rw-rw-   0        0        0     1797 2024-03-07 09:45:41.000000 streamlit-qs-0.3.1/streamlit_qs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      279 2024-03-07 09:45:41.000000 streamlit-qs-0.3.1/streamlit_qs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-07 09:45:41.000000 streamlit-qs-0.3.1/streamlit_qs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2024-03-07 09:45:41.000000 streamlit-qs-0.3.1/streamlit_qs.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-03-07 09:45:41.000000 streamlit-qs-0.3.1/streamlit_qs.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-03-07 09:45:41.163027 streamlit-qs-0.3.1/tests/
--rw-rw-rw-   0        0        0    22782 2024-01-28 05:55:00.000000 streamlit-qs-0.3.1/tests/test_streamlit_qs.py
+drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2024-05-11 23:15:47.000780 streamlit_qs-0.3.2/
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)    11357 2024-04-26 12:15:25.000000 streamlit_qs-0.3.2/LICENSE
+-rw-r--r--   0 alexander  (1000) alexander  (1000)     1777 2024-05-11 23:15:47.000780 streamlit_qs-0.3.2/PKG-INFO
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     1219 2024-04-26 12:15:25.000000 streamlit_qs-0.3.2/README.md
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)       38 2024-05-11 23:15:47.000780 streamlit_qs-0.3.2/setup.cfg
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)      884 2024-05-11 23:14:38.000000 streamlit_qs-0.3.2/setup.py
+drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2024-05-11 23:15:46.996780 streamlit_qs-0.3.2/streamlit_qs/
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)    29665 2024-05-06 07:35:09.000000 streamlit_qs-0.3.2/streamlit_qs/__init__.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)        0 2024-04-26 12:15:25.000000 streamlit_qs-0.3.2/streamlit_qs/py.typed
+drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2024-05-11 23:15:47.000780 streamlit_qs-0.3.2/streamlit_qs.egg-info/
+-rw-r--r--   0 alexander  (1000) alexander  (1000)     1777 2024-05-11 23:15:46.000000 streamlit_qs-0.3.2/streamlit_qs.egg-info/PKG-INFO
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)      279 2024-05-11 23:15:46.000000 streamlit_qs-0.3.2/streamlit_qs.egg-info/SOURCES.txt
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)        1 2024-05-11 23:15:46.000000 streamlit_qs-0.3.2/streamlit_qs.egg-info/dependency_links.txt
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)       18 2024-05-11 23:15:46.000000 streamlit_qs-0.3.2/streamlit_qs.egg-info/requires.txt
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)       13 2024-05-11 23:15:46.000000 streamlit_qs-0.3.2/streamlit_qs.egg-info/top_level.txt
+drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2024-05-11 23:15:46.996780 streamlit_qs-0.3.2/tests/
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)    22487 2024-05-06 07:35:21.000000 streamlit_qs-0.3.2/tests/test_streamlit_qs.py
```

### Comparing `streamlit-qs-0.3.1/LICENSE` & `streamlit_qs-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit-qs-0.3.1/PKG-INFO` & `streamlit_qs-0.3.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,53 +1,54 @@
-Metadata-Version: 2.1
-Name: streamlit-qs
-Version: 0.3.1
-Summary: A small library to add extra functionality on top of streamlit's st.query_params API
-Home-page: https://github.com/Asaurus1/streamlit-qs
-Author: Alexander Martin
-Author-email: fauxjunk-1@yahoo.com
-License: Apache 2
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Query String functions for Streamlit
-This app shows off the [Query String Utility Functions](https://github.com/Asaurus1/streamlit-qs) for Streamlit.
-
-The functions in this library allow you to easily create "permalink-like" functionality in your application,
-This can let users to share links with others that will populate streamlit with the same set of input values
-that they were using. Or you can use the query string to pass data into your streamlit application from
-another website or program.
-
-
-## Installation
-
-First install Streamlit (of course!) then install this library:
-
-```bash
-pip install streamlit-qs
-```
-or
-```bash
-pip install git+https://github.com/Asaurus1/streamlit-qs.git@main
-```
-
-## Example
-
-```python
-import streamlit as st
-import streamlit_qs as stqs
-
-st.markdown("[Click this URL](?input_some_text=Hello+World)") 
-stqs.text_input_qs("Enter Some Text", key="input_some_text")
-```
-
-For more examples, including :sparkles:**customization options**:sparkles:, see
-[the demo app](https://query-string.streamlit.app/).
-
-
-## Version Compatibility
-For Streamlit v1.29.0 or below use release v0.2.0 of this app
-For Streamlit v1.30.0 or above, use the latest released version of this app above v0.2.0
+Metadata-Version: 2.1
+Name: streamlit-qs
+Version: 0.3.2
+Summary: A small library to add extra functionality on top of streamlit's st.query_params API
+Home-page: https://github.com/Asaurus1/streamlit-qs
+Author: Alexander Martin
+Author-email: fauxjunk-1@yahoo.com
+License: Apache 2
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: streamlit>=1.30.0
+
+# Query String functions for Streamlit
+This app shows off the [Query String Utility Functions](https://github.com/Asaurus1/streamlit-qs) for Streamlit.
+
+The functions in this library allow you to easily create "permalink-like" functionality in your application,
+This can let users to share links with others that will populate streamlit with the same set of input values
+that they were using. Or you can use the query string to pass data into your streamlit application from
+another website or program.
+
+
+## Installation
+
+First install Streamlit (of course!) then install this library:
+
+```bash
+pip install streamlit-qs
+```
+or
+```bash
+pip install git+https://github.com/Asaurus1/streamlit-qs.git@main
+```
+
+## Example
+
+```python
+import streamlit as st
+import streamlit_qs as stqs
+
+st.markdown("[Click this URL](?input_some_text=Hello+World)") 
+stqs.text_input_qs("Enter Some Text", key="input_some_text")
+```
+
+For more examples, including :sparkles:**customization options**:sparkles:, see
+[the demo app](https://query-string.streamlit.app/).
+
+
+## Version Compatibility
+For Streamlit v1.29.0 or below use release v0.2.0 of this app
+For Streamlit v1.30.0 or above, use the latest released version of this app above v0.2.0
```

### Comparing `streamlit-qs-0.3.1/README.md` & `streamlit_qs-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `streamlit-qs-0.3.1/setup.py` & `streamlit_qs-0.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding='utf8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="streamlit-qs",
-    version="0.3.1",
+    version="0.3.2",
     author="Alexander Martin",
     author_email="fauxjunk-1@yahoo.com",
     description="A small library to add extra functionality on top of streamlit's st.query_params API",
     license="Apache 2",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Asaurus1/streamlit-qs",
```

### Comparing `streamlit-qs-0.3.1/streamlit_qs/__init__.py` & `streamlit_qs-0.3.2/streamlit_qs/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,642 +1,664 @@
-"""Query string extensions for Streamlit."""
-from __future__ import annotations
-from enum import Enum
-
-import functools
-import re
-import urllib.parse
-from typing import (
-    TYPE_CHECKING,
-    Any,
-    Callable,
-    Collection,
-    KeysView,
-    List,
-    Mapping,
-    MutableMapping,
-    Sequence,
-    Set,
-    Type,
-    TypeVar,
-    cast,
-    overload,
-)
-
-import streamlit as st
-
-if TYPE_CHECKING:
-    Number = int | float
-
-from streamlit.type_util import OptionSequence, ensure_indexable
-from streamlit.errors import StreamlitAPIException, StreamlitAPIWarning
-from typing_extensions import Literal
-
-
-# TypeVars
-T = TypeVar("T")
-Tenum = TypeVar("Tenum", bound=Enum)
-Tbs = TypeVar("Tbs", bytes, str)
-
-
-# Settings/Constants
-DISABLE_WARNINGS = False
-"""This flag controls the display of warning message for common problems.
-Set to false if you know what you're doing."""
-
-
-QS_BLACKLIST_KEYS: Set[str] = set()
-"""A list of query string keys are are not allowed because they are used elsewhere in application
-backend code. Expected to be set by the user at application initalization."""
-
-
-def blacklist_key(key: str):
-    """Add a key to the list of blacklisted keys that won't show up in the query string."""
-    QS_BLACKLIST_KEYS.add(key)
-
-
-def unblacklist_key(key: str):
-    """Remove a key from the list of blacklisted keys that won't show up in the query string.
-
-    Key is ignored if it isn't already blacklisted.
-    """
-    QS_BLACKLIST_KEYS.discard(key)
-
-
-# Start of the "_qs" functions
-def selectbox_qs(
-    label: str,
-    options: OptionSequence[T],
-    index: int | None = 0,
-    *,
-    key: str,
-    autoupdate: bool = False,
-    unformat_func: Any = str,
-    **kwargs
-) -> T | None:
-    """Create a streamlit selectbox which automatically populates itself from the URL query string.
-
-    Takes all arguments that st.selectbox takes, but the "key" keyword argument _must_ be provided. Returns the value
-    selected by the user.
-    """
-    indexible_options = ensure_indexable(options)
-    _raise_if_option_is_none(indexible_options, widgettype="selectbox_qs")
-
-    query_index = from_query_args_index(key, options, default=index, unformat_func=unformat_func)
-    if query_index is not None and key not in st.session_state:
-        st.session_state.setdefault(key, indexible_options[query_index])
-    if autoupdate:
-        _wrap_on_change_with_qs_update(key, kwargs, remove_none_values=(index is None))
-
-    return st.selectbox(label, options, index=index, key=key, **kwargs)
-
-
-def radio_qs(
-    label: str,
-    options: OptionSequence[T],
-    index: int | None = 0,
-    *,
-    key: str,
-    autoupdate: bool = False,
-    unformat_func: Any = str,
-    **kwargs
-) -> T | None:
-    """Create a streamlit radio widget which automatically populates itself from the URL query string.
-
-    Takes all arguments that st.radio takes, but the "key" keyword argument _must_ be provided. Returns the value
-    selected by the user. "autoupdate" causes that value to also be populated into the URL query string on change.
-    """
-    indexible_options = ensure_indexable(options)
-    _raise_if_option_is_none(indexible_options, widgettype="radio_qs")
-
-    query_index=from_query_args_index(key, options, default=index, unformat_func=unformat_func)
-    if query_index is not None and key not in st.session_state:
-        st.session_state.setdefault(key, indexible_options[query_index])
-    if autoupdate:
-        _wrap_on_change_with_qs_update(key, kwargs, remove_none_values=(index is None))
-
-    return st.radio(label, options, index=query_index, key=key, **kwargs)
-
-
-def multiselect_qs(
-    label: str,
-    options: OptionSequence[T],
-    default: Sequence[T] | T | None = None,
-    *,
-    key: str,
-    discard_missing: bool = True,
-    unformat_func: Any = str,
-    autoupdate: bool = False,
-    **kwargs,
-) -> List[T]:
-    """Create a streamlit multi_select widget which automatically populates itself from the URL query string.
-
-    Takes all arguments that st.multiselect takes, but the "key" keyword argument _must_ be provided. Returns the value
-    selected by the user. If the additional argument discard_missing is set to True, a ValueError will be raised
-    if the query string contains selection options which are not in the set of available options.
-    "autoupdate" causes that value to also be populated into the URL query string on change.
-    "unformat_func" can be used to specify a callable that turns a string value from the query string back into a python
-    object. For example, pass `unformat_func=int` to convert query string values to integers.
-    """
-    indexible_options = ensure_indexable(options)
-    _raise_if_option_is_none(indexible_options, widgettype="multiselect_qs")
-
-    default_list: List[T] = [] if default is None else _ensure_list(default)
-    maybe_from_query = from_query_args(key, default=default_list, as_list=True, unformat_func=unformat_func)
-    
-    ms_default_subset = [item for item in maybe_from_query if item in indexible_options]
-        
-    # discard missing items or throw an exception if we got a value from the query string that is not in the options
-    if not discard_missing and ms_default_subset != maybe_from_query:
-        raise ValueError(
-            "Some query string options were not contained in the available options for multiselect "
-            f'key = "{key}". Missing values: {[item for item in maybe_from_query if item not in indexible_options]}'
-        )
-    if maybe_from_query != default_list:
-        # Set session state IF we're not using the default value.
-        st.session_state.setdefault(key, ms_default_subset)
-    if autoupdate:
-        _wrap_on_change_with_qs_update(key, kwargs, remove_none_values=(default is None))
-    return st.multiselect(label, options, default=default, key=key, **kwargs)
-
-
-def checkbox_qs(label: str, default: bool = False, *, key: str, autoupdate: bool = False, **kwargs) -> bool:
-    """Create a streamlit checkbox widget which automatically populates itself from the URL query string.
-
-    Takes all arguments that st.radio takes, but the "key" keyword argument _must_ be provided.
-    The following values will be treated as True: "true", "1" (case insensitive)
-    The following values will be treated as False: "false", "0" (case insensitive)
-    Any other value will result in the checkbox using the "default" value.
-
-    "autoupdate" causes that value to also be populated into the URL query string on change.
-    """
-    query_bool = from_query_args(key, default=default, unformat_func=lambda val: _convert_bool_checkbox(val, default=default))
-    st.session_state.setdefault(key, query_bool)
-    if autoupdate:
-        _wrap_on_change_with_qs_update(key, kwargs, remove_none_values=(default is None))
-    return st.checkbox(label, value=default, key=key, **kwargs)
-
-
-@overload
-def text_input_qs(label: str, default: None, *, key: str, autoupdate: bool = False, **kwargs) -> str | None: ...
-
-@overload
-def text_input_qs(label: str, default: str = "", *, key: str, autoupdate: bool = False, **kwargs) -> str: ...
-
-def text_input_qs(label: str, default: str | None = "", *, key: str, autoupdate: bool = False, **kwargs) -> str | None:
-    """Create a streamlit text_input which automatically populates itself from the URL query string.
-
-    Takes all arguments that st.text_input takes, but the "key" keyword argument _must_ be provided. Returns the value
-    selected by the user. "autoupdate" causes that value to also be populated into the URL query string on change.
-    """
-    st.session_state.setdefault(key, from_query_args(key, default=default))
-    if autoupdate:
-        _wrap_on_change_with_qs_update(key, kwargs, remove_none_values=(default is None))
-    return st.text_input(label, value=default, key=key, **kwargs)
-
-
-@overload
-def text_area_qs(label: str, default: None, *, key: str, autoupdate: bool = False, **kwargs) -> str | None: ...
-
-@overload
-def text_area_qs(label: str, default: str = "", *, key: str, autoupdate: bool = False, **kwargs) -> str: ...
-
-def text_area_qs(label: str, default: str | None = "", *, key: str, autoupdate: bool = False, **kwargs) -> str | None:
-    """Create a streamlit text_area which automatically populates itself from the URL query string.
-
-    Takes all arguments that st.text_area takes, but the "key" keyword argument _must_ be provided. Returns the value
-    selected by the user. "autoupdate" causes that value to also be populated into the URL query string on change.
-    """
-    st.session_state.setdefault(key, from_query_args(key, default=default))
-    if autoupdate:
-        _wrap_on_change_with_qs_update(key, kwargs, remove_none_values=(default is None))
-    return st.text_area(label, value=default, key=key, **kwargs)
-
-
-@overload
-def number_input_qs(label: str, default: Number | Literal["min"] = "min", *, key: str, autoupdate: bool = False, **kwargs) -> Number:
-    ...
-
-@overload
-def number_input_qs(label: str, default: Number | None  = None, *, key: str, autoupdate: bool = False, **kwargs) -> Number | None:
-    ...
-
-def number_input_qs(label: str, default = "min", *, key: str, autoupdate: bool = False, **kwargs) -> Number | None:
-    """Create a streamlit number_input which automatically populates itself from the URL query string.
-
-    Takes all arguments that st.number_input takes, but the "key" keyword argument _must_ be provided. Returns the value
-    selected by the user. "autoupdate" causes that value to also be populated into the URL query string on change.
-    """
-    query_value: Number | None | Literal["min"]
-
-    # Get the query string value and attempt to coerce it to an int or float depending on
-    # the arguments to this function, in a similar way that number_input changes from an int
-    # widget to a float widget depending on the types here.
-    # If this works, we set up session_state with the value we got from the url, otherwise
-    # we just do nothing and call the regular number_input function (with a possible wrapped
-    # autoupdate callback).
-    query_arg = from_query_args(key, default="NOT_A_NUMBER")
-    if isinstance(default, (int, float)):
-        expected_type = type(default)
-    elif "min_value" in kwargs:
-        expected_type = type(kwargs["min_value"])
-    elif "max_value" in kwargs:
-        expected_type = type(kwargs["max_value"])
-    elif "step" in kwargs:
-        expected_type = type(kwargs["step"])
-    else:
-        expected_type = float
-    if not issubclass(expected_type, (int, float)):
-        raise TypeError(f"Expected type was not a float. Got {expected_type}")
-
-    try:
-        query_value = expected_type(query_arg)
-        st.session_state.setdefault(key, query_value)
-    except (ValueError, TypeError):
-        pass
-
-    if autoupdate:
-        _wrap_on_change_with_qs_update(key, kwargs, remove_none_values=(default is None))
-    return st.number_input(label, value=default, key=key, **kwargs)
-
-
-@overload
-def from_query_args(key: str, default: str = "", *, as_list: Literal[False] = False, unformat_func: Any = str) -> str:
-    ...
-
-
-@overload
-def from_query_args(key: str, default: T, *, unformat_func: Any, as_list: Literal[False] = False) -> T:
-    ...
-
-@overload
-def from_query_args(key: str, default: None, *, as_list: Literal[False] = False, unformat_func: Any = str) -> Any:
-    # actually returns an Optional[str] but mypy won't let us do that until https://github.com/python/mypy/pull/15846
-    # is released in 1.5.2.
-    ...
-
-@overload
-def from_query_args(key: str, default: List[str], *, as_list: Literal[True], unformat_func: Any = str) -> List[str]:
-    ...
-
-@overload
-def from_query_args(key: str, default: List[None], *, as_list: Literal[True], unformat_func: Any = str) -> Any:
-    # actually returns a List[Optional[str]] but mypy won't let us do that until
-    # https://github.com/python/mypy/pull/15846 is released in 1.5.2
-    ...
-    
-@overload
-def from_query_args(key: str, default: List[T], *, as_list: Literal[True], unformat_func: Any) -> List[T]:
-    ...
-
-def from_query_args(key, default = "", *, as_list=False, unformat_func: Any = str):
-    """Return the value passed to the webpage URL via the query string for the given key.
-
-    If the key does not exist in the query string, default is returned.
-    Values are returned as a single python object, unless as_list is True. If as_list is True, the values
-    returned are lists of objects. By default all objects are strings. The `unformat_func` argument takes
-    a callable that converts a single `str` to type `T` and can be used to parse serialized data into
-    python objects.
-
-    If multiple values are defined for a given key, this code will throw an exception when as_list is False
-    and will return all defined values when as_list is true.
-    """
-    values = st.query_params.get_all(key)
-
-    if not values:
-        # if there's nothing in the query string, give the default
-        out_value = default if as_list else [default]
-    elif unformat_func is str:
-        # Otherwise the list of values from the query string as strings
-        out_value = values  # values is always str and user expects str
-    else:
-        # Or possibly convert them first
-        out_value = [unformat_func(val) for val in values]  # convert str -> T using unformat_func
-
-    if as_list:
-        return out_value
-    elif len(out_value) > 1:
-        raise ValueError(f"Got multiple values for query string key {key}. Query contents: \n\n {st.query_params.to_dict()}")
-
-    return out_value[0]
-
-
-@overload
-def from_query_args_index(key: str, options: OptionSequence[T], default: int = 0, unformat_func: Any = str) -> int:
-    ...
-
-@overload
-def from_query_args_index(key: str, options: OptionSequence[T], default: None, unformat_func: Any = str) -> int | None:
-    ...
-
-def from_query_args_index(key: str, options: OptionSequence[T], default: int | None = 0, unformat_func: Any = str) -> int | None:
-    """Return the index in the sequence "options" of the value given for the key in the URL query string.
-
-    If the value is not present in the sequence "options", or if multiple values are provided, returns the default
-    value. This can be used to create a selectbox with a default choice.
-
-    >>> st.selectbox("my box", [1, 2, 3], stu.from_query_args_index("myoption", [1, 2, 3]))
-    """
-    indexible_options = ensure_indexable(options)
-    unformat_func = _infer_common_unformat_funcs(indexible_options, unformat_func)
-    try:
-        return indexible_options.index(from_query_args(key, as_list=False, unformat_func=unformat_func))
-    except ValueError:
-        return default
-
-
-def make_query_string(keys: Collection[str] | None = None, regex: Collection[str | re.Pattern] = ()) -> str:
-    """Get a (relative) URL for a query string of of user-keyed fields on the page and their current values.
-
-    Usage:
-        >>> permalink = stu.make_query_string({"a", "b", "c"})
-        >>> st.markdown(f"[permalink]({permalink})")
-
-    Args:
-        keys (optional, set[str]): The set of keys to be included in the query string.
-        regex (optional, sequence[Pattern]): an optional set of patterns to match with keys as an alternate method of
-            specifying which keys to include.
-
-    Returns:
-        url (str): the relative URL string (everything after the "?")
-
-    Note: This method does NOT guarantee that the URL will return you to this exact session state, as
-    only fields which are watching for a default value from the query string will autopopulate when someone navigates
-    to the URL. When called without arguments, the query string will include values for fields which MAY NOT be watching
-    the query string for values. These will be silently ignored.
-
-    Note: Calling this method will only capture values for fields which have already been rendered, in other words, for
-    >>> stu.make_query_string()
-    >>> stu.number_input_gs("Hello", key="mykey")
-    the make_query_string() call will not always capture the value of "mykey" because the streamlit application has not
-    yet processed that line. At other times it may capture the value of mykey, but the value captured may be "stale"
-    or out-of-date.
-    """
-    return "?" + urllib.parse.urlencode(_qs_intersect(keys, regex), doseq=True)
-
-
-def set_qs_callback(keys: Collection[str] | None = None, regex: Collection[str | re.Pattern] = ()) -> Callable[[], None]:
-    """Return a callable that replaces the browser URL query string with keys-value pairs for the user-defined keys specified.
-
-    Usage:
-        >>> st.button("Update URL!", on_click=stu.set_qs_callback(["field1", "field2"]))
-
-    Args:
-        keys (optional, set[str]): The set of keys to be included in the query string.
-        regex (optional, sequence[Pattern]): an optional set of patterns to match with keys as an alternate method of
-            specifying which keys to include.
-
-
-    Note: This method does NOT guarantee that the URL will return you to this exact session state, as only fields
-    which are watching for a default value from the query string will autopopulate when someone navigates to the URL.
-    When called without arguments, the query string will include values for fields which MAY NOT be watching the query
-    string for values. These will be silently ignored.
-    """
-
-    def _set_qs_callback():
-        st.query_params.clear()
-        st.query_params.update(_qs_intersect(keys, regex))
-
-    return _set_qs_callback
-
-
-def clear_qs_callback(keys: Collection[str] | None = None, regex: Collection[str | re.Pattern] = ()) -> Callable[[], None]:
-    """Return a callable that clears the query string from the URL. If a specific set of keys or patterns are provided,
-    only those keys will be cleared. This callback is designed to be used with the "on_click" or "on_change" argument
-    of a button or widget.
-
-    This will NOT reset the values of any fields that depend on the query string, you must do that yourself by
-    removing the fields' keys from `st.session_state`.
-
-    Args:
-        keys (set[str]): The set of keys to be removed to the query string.
-        regex (optional, sequence[Pattern]): an optional set of patterns to match with keys as an alternate method of
-            specifying which keys to add.
-    """
-
-    def _clear_qs_callback():
-        if not keys and not regex:
-            st.query_params.clear()
-        else:
-            for key in _qs_intersect(keys, regex).keys():
-                st.query_params.pop(key, None)
-
-    return _clear_qs_callback
-
-
-def add_qs_callback(keys: Collection[str] | None = None, regex: Collection[str | re.Pattern] = ()) -> Callable[[], None]:
-    """Return a callable that adds to the browser URL the keys-value pairs for the user-defined keys specified.
-    Keys with a None value are ignored. Existing key-value pairs in the URL will not be changed or removed
-    (they may be reordered). This callback is designed to be used with the "on_click" or "on_change" argument
-    of a button or widget.
-
-    Args:
-        keys (optional, set[str]): The set of keys to be added to the query string.
-        regex (optional, sequence[Pattern]): an optional set of patterns to match with keys as an alternate method of
-            specifying which keys to add.
-
-    Note: This method does NOT guarantee that the URL will return you to this exact session state, as only fields
-    which are watching for a default value from the query string will autopopulate when someone navigates to the URL.
-    When called without arguments, the query string will include values for fields which MAY NOT be watching the query
-    string for values. These will be silently ignored.
-    """
-
-    def _add_qs_callback():
-        st.query_params.update(_qs_intersect(keys, regex))
-
-    return _add_qs_callback
-
-
-def update_qs_callback(keys: Collection[str] | None = None, regex: Collection[str | re.Pattern] = ()) -> Callable[[], None]:
-    """Return a callable that updates the browser URL with keys-value pairs for the user-defined keys specified.
-    Keys which are paired with a None value are *removed* from the query string. Other existing key-value pairs
-    in the URL will not be changed or removed (they may be reordered). This callback is designed to be used with
-    the "on_click" or "on_change" argument of a button or widget.
-
-    Args:
-        keys (optional, set[str]): The set of keys to be added to the query string.
-        regex (optional, sequence[Pattern]): an optional set of patterns to match with keys as an alternate method of
-            specifying which keys to add.
-
-    Note: This method does NOT guarantee that the URL will return you to this exact session state, as only fields
-    which are watching for a default value from the query string will autopopulate when someone navigates to the URL.
-    When called without arguments, the query string will include values for fields which MAY NOT be watching the query
-    string for values. These will be silently ignored.
-    """
-
-    def _update_qs_callback():
-        new_dict = _qs_intersect(keys, regex, allownone=True)
-        update_dict = {}
-        none_keys = []
-        for key, value in new_dict.items():
-            if value is None:
-                none_keys.append(key)
-            else:
-                update_dict[key] = value
-        for key in none_keys:
-            st.query_params.pop(key, None)
-        st.query_params.update(update_dict)
-
-    return _update_qs_callback
-
-def unenumifier(cls: Type[Tenum]) -> Callable[[str], Tenum] :
-    """Get a factory function for turning strings into enum members.
-
-    Python's default Enums render as strings as "<cls>.<member>". This function
-    returns a callable that looks up the member based on this string.
-    """
-    def _unenum(value: str) -> Tenum:
-        """Convert a string into a member of {cls}"""
-        value_name = value.replace(cls.__name__ + ".", "")
-        try:
-            return cls[value_name]
-        except KeyError:
-            raise ValueError(f"'{value_name} is not a valid member of '{cls.__qualname__}'")
-
-    _unenum.__name__ += "_" + cls.__name__
-    _unenum.__doc__ = _unenum.__doc__.format(cls=cls)  # type: ignore
-
-    return _unenum
-
-
-# Helper Functions -----------------------------------------------------------------------------
-
-def _qs_intersect(keys: Collection[str] | None, regex: Collection[str | re.Pattern], allownone: bool = False) -> Mapping[str, Any]:
-    """Get a dictionary containing pairs from st.session_state whose keys match the arguments/patterns."""
-    if isinstance(keys, str) or isinstance(regex, str):
-        raise ValueError("Arguments to query string functions must be non-str collections, e.g. list, tuple, set ...")
-    # Keys are guaranteed to always be strs by SessionStateProxy
-    session_keys = cast(KeysView[str], st.session_state.keys())
-    if keys is None and not regex:
-        use_keys = set(session_keys)
-    else:
-        # Find keys in session_keys that match the regex
-        reg_keys = {key for key in session_keys if any(re.match(pattern, key) for pattern in regex)}
-        # Put the intersection of the string keys and the reg keys together
-        use_keys = (set(keys).intersection(session_keys) if keys else set()) | reg_keys
-
-    # Return the new query string dictionary, but filter out blacklisted keys and None values
-    return {
-        key: st.session_state[key] for key in use_keys if key not in QS_BLACKLIST_KEYS and (allownone or st.session_state[key] is not None)
-    }
-
-
-def _wrap_on_change_with_qs_update(key: str, kwargs: MutableMapping, remove_none_values: bool):
-    """Mutates kwargs to add a query string update for the specified key to the on_change argument."""
-    existing_callback: Callable | None = kwargs.get("on_change", None)
-
-    # Select the right kind of callback
-    if remove_none_values:
-        pre_update_func = update_qs_callback(keys=(key,))
-    else:
-        pre_update_func = add_qs_callback(keys=(key,))
-
-    # Use the existing function if there's not one already defined for on_change.
-    if existing_callback is None:
-        kwargs["on_change"] = pre_update_func
-        return
-    elif not callable(existing_callback):
-        raise TypeError(f"'on_change' keyword argument is not callable: {existing_callback}")
-
-    # Otherwise decorate the existing function with an update to the query params beforehand
-    @functools.wraps(existing_callback)
-    def wrapper(*args, **kwargs):
-        pre_update_func()
-        existing_callback(*args, **kwargs)
-
-    # At the end, mutate kwargs
-    kwargs["on_change"] = wrapper
-
-
-def _convert_bool_checkbox(string_bool: str, default: bool) -> bool:
-    """Convert from string values to boolean values, with a default value if conversion fails."""
-    if string_bool.lower() in ("1", "true"):
-        return True
-    elif string_bool.lower() in ("0", "false"):
-        return False
-    return default
-
-
-@overload
-def _ensure_list(maybe_list: Tbs) -> List[Tbs]:
-    ...
-
-@overload
-def _ensure_list(maybe_list: Sequence[T]) -> List[T]:
-    ...
-
-@overload
-def _ensure_list(maybe_list: T) -> List[T]:
-    ...
-
-def _ensure_list(maybe_list):
-    """Convert single values and sequences (except bytes and str) to lists."""
-    if isinstance(maybe_list, list):
-        return maybe_list
-    elif isinstance(maybe_list, (bytes, str)) or not isinstance(maybe_list, Sequence):
-        return [maybe_list]
-    else:
-        return list(maybe_list)
-
-
-def _infer_common_unformat_funcs(indexible_options: Sequence[Any], unformat_func):
-    """Infers some common unformat_funcs based on the items in the indexible_options and returns the new function."""
-    if unformat_func is str and len(indexible_options)!=0 and not all(isinstance(opt, str) for opt in indexible_options):
-        # If they're ints or floats or bytes (uniformly), coerce back to those.
-        for typ in (int, float, bytes):
-            if all(isinstance(opt, typ) for opt in indexible_options):
-                return typ
-
-        # If they all come from the same enum, coerce back to that
-        if isinstance(indexible_options[0], Enum):
-            enum_cls = indexible_options[0].__class__
-            if all(isinstance(opt, enum_cls) for opt in indexible_options):
-                return unenumifier(enum_cls)
-
-    _warn_on_common_unmatching_unformat_functions(indexible_options, unformat_func)
-    return unformat_func
-
-
-def _warn_on_common_unmatching_unformat_functions(options, unformat_func):
-    """Produces a warning if the user registers non-string options but provides or leaves the
-    default "str" as an unformat_func."""
-    if DISABLE_WARNINGS:
-        return
-    if not all(isinstance(opt, str) for opt in options) and unformat_func is str:
-        detected_types = {type(opt) for opt in options}
-        msg = f"""In the widget below, you've used a select or multi-select streamlit_qs element
-with non-string-type options (we found {detected_types}), but did not provide an `unformat_func`
-to deserialize the values from the URL back into those objects, and we could not deduce one for you.
-For example, you may have tried something like
-
-    st.selectbox_qs("Pick a number", options=[1, 1.5, 2], key="picknumber")
-
-To do this correctly, you need to explicitly specify how to convert the values in the URL back to options.
-In this case you might define a function like
-
-    def int_or_float(string):
-        try: return int(string)
-        except ValueError: pass
-        return float(string)
-
-And then call
-
-    st.selectbox_qs("Pick a number", options=[1, 1.5, 2], key="pickanumber", unformat_func=int_or_float)
-
-    """
-        st.exception(StreamlitAPIWarning(msg))
-        st._logger.get_logger(__name__).warning(msg, stack_info=True, stacklevel=5)
-
-
-def _raise_if_option_is_none(indexible_options, widgettype="widget that supports section from a list of options"):
-    """Raises an exception if the user tries to pass None as an option. While this is technically allowed
-    with the base streamlit widgets, we can't serialize "None" to the URL string in a way that is differentiable
-    from the string "None" as well as the None value that some widgets can now return in Streamlit 1.27.0+. So we
-    must disallow it."""
-    if any(opt is None for opt in indexible_options):
-        msg = f"""You may not pass the value None as an item to a streamlit_qs {widgettype}, as there is no reliable
-way to serialize this value to the URL query string. If you are trying to create a widget with an empty default value,
-please pass None as the 'default' argument instead of adding to the 'options' list.
-
-Got the following options: {indexible_options}
-        """
-        raise StreamlitAPIException(msg)
+"""Query string extensions for Streamlit."""
+from __future__ import annotations
+from enum import Enum
+
+import functools
+import re
+import urllib.parse
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Callable,
+    Collection,
+    KeysView,
+    List,
+    Mapping,
+    MutableMapping,
+    Sequence,
+    Set,
+    Type,
+    TypeVar,
+    cast,
+    overload,
+)
+
+import streamlit as st
+
+if TYPE_CHECKING:
+    Number = int | float
+
+from streamlit.type_util import OptionSequence, ensure_indexable
+from streamlit.errors import StreamlitAPIException, StreamlitAPIWarning
+from typing_extensions import Literal
+
+
+# TypeVars
+T = TypeVar("T")
+Tenum = TypeVar("Tenum", bound=Enum)
+Tbs = TypeVar("Tbs", bytes, str)
+
+
+# Settings/Constants
+DISABLE_WARNINGS = False
+"""This flag controls the display of warning message for common problems.
+Set to false if you know what you're doing."""
+
+
+QS_BLACKLIST_KEYS: Set[str] = set()
+"""A list of query string keys are are not allowed because they are used elsewhere in application
+backend code. Expected to be set by the user at application initalization."""
+
+
+def blacklist_key(key: str):
+    """Add a key to the list of blacklisted keys that won't show up in the query string."""
+    QS_BLACKLIST_KEYS.add(key)
+
+
+def unblacklist_key(key: str):
+    """Remove a key from the list of blacklisted keys that won't show up in the query string.
+
+    Key is ignored if it isn't already blacklisted.
+    """
+    QS_BLACKLIST_KEYS.discard(key)
+
+
+# Start of the "_qs" functions
+def selectbox_qs(
+    label: str,
+    options: OptionSequence[T],
+    index: int | None = 0,
+    *,
+    key: str,
+    autoupdate: bool = False,
+    unformat_func: Any = str,
+    **kwargs
+) -> T | None:
+    """Create a streamlit selectbox which automatically populates itself from the URL query string.
+
+    Takes all arguments that st.selectbox takes, but the "key" keyword argument _must_ be provided. Returns the value
+    selected by the user.
+    """
+    indexible_options = ensure_indexable(options)
+    _raise_if_option_is_none(indexible_options, widgettype="selectbox_qs")
+
+    query_index = from_query_args_index(key, options, default=index, unformat_func=unformat_func)
+    if query_index is not None and key not in st.session_state:
+        st.session_state.setdefault(key, indexible_options[query_index])
+    if autoupdate:
+        _wrap_on_change_with_qs_update(key, kwargs, remove_none_values=(index is None))
+
+    return st.selectbox(label, options, index=index, key=key, **kwargs)
+
+
+def radio_qs(
+    label: str,
+    options: OptionSequence[T],
+    index: int | None = 0,
+    *,
+    key: str,
+    autoupdate: bool = False,
+    unformat_func: Any = str,
+    **kwargs
+) -> T | None:
+    """Create a streamlit radio widget which automatically populates itself from the URL query string.
+
+    Takes all arguments that st.radio takes, but the "key" keyword argument _must_ be provided. Returns the value
+    selected by the user. "autoupdate" causes that value to also be populated into the URL query string on change.
+    """
+    indexible_options = ensure_indexable(options)
+    _raise_if_option_is_none(indexible_options, widgettype="radio_qs")
+
+    query_index=from_query_args_index(key, options, default=index, unformat_func=unformat_func)
+    if query_index is not None and key not in st.session_state:
+        st.session_state.setdefault(key, indexible_options[query_index])
+    if autoupdate:
+        _wrap_on_change_with_qs_update(key, kwargs, remove_none_values=(index is None))
+
+    return st.radio(label, options, index=query_index, key=key, **kwargs)
+
+
+def multiselect_qs(
+    label: str,
+    options: OptionSequence[T],
+    default: Sequence[T] | T | None = None,
+    *,
+    key: str,
+    discard_missing: bool = True,
+    unformat_func: Any = str,
+    autoupdate: bool = False,
+    **kwargs,
+) -> List[T]:
+    """Create a streamlit multi_select widget which automatically populates itself from the URL query string.
+
+    Takes all arguments that st.multiselect takes, but the "key" keyword argument _must_ be provided. Returns the value
+    selected by the user. If the additional argument discard_missing is set to True, a ValueError will be raised
+    if the query string contains selection options which are not in the set of available options.
+    "autoupdate" causes that value to also be populated into the URL query string on change.
+    "unformat_func" can be used to specify a callable that turns a string value from the query string back into a python
+    object. For example, pass `unformat_func=int` to convert query string values to integers.
+    """
+    indexible_options = ensure_indexable(options)
+    _raise_if_option_is_none(indexible_options, widgettype="multiselect_qs")
+
+    default_list: List[T] = [] if default is None else _ensure_list(default)
+    maybe_from_query = from_query_args(key, default=default_list, as_list=True, unformat_func=unformat_func)
+
+    ms_default_subset = [item for item in maybe_from_query if item in indexible_options]
+
+    # discard missing items or throw an exception if we got a value from the query string that is not in the options
+    if not discard_missing and ms_default_subset != maybe_from_query:
+        raise ValueError(
+            "Some query string options were not contained in the available options for multiselect "
+            f'key = "{key}". Missing values: {[item for item in maybe_from_query if item not in indexible_options]}'
+        )
+    if maybe_from_query != default_list:
+        # Set session state IF we're not using the default value.
+        st.session_state.setdefault(key, ms_default_subset)
+    if autoupdate:
+        _wrap_on_change_with_qs_update(key, kwargs, remove_none_values=(default is None))
+    return st.multiselect(label, options, default=default, key=key, **kwargs)
+
+
+def checkbox_qs(label: str, default: bool = False, *, key: str, autoupdate: bool = False, **kwargs) -> bool:
+    """Create a streamlit checkbox widget which automatically populates itself from the URL query string.
+
+    Takes all arguments that st.radio takes, but the "key" keyword argument _must_ be provided.
+    The following values will be treated as True: "true", "1" (case insensitive)
+    The following values will be treated as False: "false", "0" (case insensitive)
+    Any other value will result in the checkbox using the "default" value.
+
+    "autoupdate" causes that value to also be populated into the URL query string on change.
+    """
+    query_bool = from_query_args(key, default=default, unformat_func=lambda val: _convert_bool_checkbox(val, default=default))
+    st.session_state.setdefault(key, query_bool)
+    if autoupdate:
+        _wrap_on_change_with_qs_update(key, kwargs, remove_none_values=(default is None))
+    return st.checkbox(label, value=default, key=key, **kwargs)
+
+
+@overload
+def text_input_qs(label: str, default: None, *, key: str, autoupdate: bool = False, **kwargs) -> str | None: ...
+
+@overload
+def text_input_qs(label: str, default: str = "", *, key: str, autoupdate: bool = False, **kwargs) -> str: ...
+
+def text_input_qs(label: str, default: str | None = "", *, key: str, autoupdate: bool = False, **kwargs) -> str | None:
+    """Create a streamlit text_input which automatically populates itself from the URL query string.
+
+    Takes all arguments that st.text_input takes, but the "key" keyword argument _must_ be provided. Returns the value
+    selected by the user. "autoupdate" causes that value to also be populated into the URL query string on change.
+    """
+    st.session_state.setdefault(key, from_query_args(key, default=default))
+    if autoupdate:
+        _wrap_on_change_with_qs_update(key, kwargs, remove_none_values=(default is None))
+    return st.text_input(label, value=default, key=key, **kwargs)
+
+
+@overload
+def text_area_qs(label: str, default: None, *, key: str, autoupdate: bool = False, **kwargs) -> str | None: ...
+
+@overload
+def text_area_qs(label: str, default: str = "", *, key: str, autoupdate: bool = False, **kwargs) -> str: ...
+
+def text_area_qs(label: str, default: str | None = "", *, key: str, autoupdate: bool = False, **kwargs) -> str | None:
+    """Create a streamlit text_area which automatically populates itself from the URL query string.
+
+    Takes all arguments that st.text_area takes, but the "key" keyword argument _must_ be provided. Returns the value
+    selected by the user. "autoupdate" causes that value to also be populated into the URL query string on change.
+    """
+    st.session_state.setdefault(key, from_query_args(key, default=default))
+    if autoupdate:
+        _wrap_on_change_with_qs_update(key, kwargs, remove_none_values=(default is None))
+    return st.text_area(label, value=default, key=key, **kwargs)
+
+
+@overload
+def number_input_qs(label: str, default: Number | Literal["min"] = "min", *, key: str, autoupdate: bool = False, **kwargs) -> Number:
+    ...
+
+@overload
+def number_input_qs(label: str, default: Number | None  = None, *, key: str, autoupdate: bool = False, **kwargs) -> Number | None:
+    ...
+
+def number_input_qs(label: str, default = "min", *, key: str, autoupdate: bool = False, **kwargs) -> Number | None:
+    """Create a streamlit number_input which automatically populates itself from the URL query string.
+
+    Takes all arguments that st.number_input takes, but the "key" keyword argument _must_ be provided. Returns the value
+    selected by the user. "autoupdate" causes that value to also be populated into the URL query string on change.
+    """
+    query_value: Number | None | Literal["min"]
+
+    # Get the query string value and attempt to coerce it to an int or float depending on
+    # the arguments to this function, in a similar way that number_input changes from an int
+    # widget to a float widget depending on the types here.
+    # If this works, we set up session_state with the value we got from the url, otherwise
+    # we just do nothing and call the regular number_input function (with a possible wrapped
+    # autoupdate callback).
+    query_arg = from_query_args(key, default="NOT_A_NUMBER")
+    if isinstance(default, (int, float)):
+        expected_type = type(default)
+    elif "min_value" in kwargs:
+        expected_type = type(kwargs["min_value"])
+    elif "max_value" in kwargs:
+        expected_type = type(kwargs["max_value"])
+    elif "step" in kwargs:
+        expected_type = type(kwargs["step"])
+    else:
+        expected_type = float
+    if not issubclass(expected_type, (int, float)):
+        raise TypeError(f"Expected type was not a float. Got {expected_type}")
+
+    try:
+        query_value = expected_type(query_arg)
+        st.session_state.setdefault(key, query_value)
+    except (ValueError, TypeError):
+        pass
+
+    if autoupdate:
+        _wrap_on_change_with_qs_update(key, kwargs, remove_none_values=(default is None))
+    return st.number_input(label, value=default, key=key, **kwargs)
+
+
+@overload
+def from_query_args(key: str, default: str = "", *, as_list: Literal[False] = False, unformat_func: Any = str) -> str:
+    ...
+
+
+@overload
+def from_query_args(key: str, default: T, *, unformat_func: Any, as_list: Literal[False] = False) -> T:
+    ...
+
+@overload
+def from_query_args(key: str, default: None, *, as_list: Literal[False] = False, unformat_func: Any = str) -> Any:
+    # actually returns an Optional[str] but mypy won't let us do that until https://github.com/python/mypy/pull/15846
+    # is released in 1.5.2.
+    ...
+
+@overload
+def from_query_args(key: str, default: List[str], *, as_list: Literal[True], unformat_func: Any = str) -> List[str]:
+    ...
+
+@overload
+def from_query_args(key: str, default: List[None], *, as_list: Literal[True], unformat_func: Any = str) -> Any:
+    # actually returns a List[Optional[str]] but mypy won't let us do that until
+    # https://github.com/python/mypy/pull/15846 is released in 1.5.2
+    ...
+
+@overload
+def from_query_args(key: str, default: List[T], *, as_list: Literal[True], unformat_func: Any) -> List[T]:
+    ...
+
+def from_query_args(key, default = "", *, as_list=False, unformat_func: Any = str):
+    """Return the value passed to the webpage URL via the query string for the given key.
+
+    If the key does not exist in the query string, default is returned.
+    Values are returned as a single python object, unless as_list is True. If as_list is True, the values
+    returned are lists of objects. By default all objects are strings. The `unformat_func` argument takes
+    a callable that converts a single `str` to type `T` and can be used to parse serialized data into
+    python objects.
+
+    If multiple values are defined for a given key, this code will throw an exception when as_list is False
+    and will return all defined values when as_list is true.
+    """
+    values = st.query_params.get_all(key)
+
+    if not values:
+        # if there's nothing in the query string, give the default
+        out_value = default if as_list else [default]
+    elif unformat_func is str:
+        # Otherwise the list of values from the query string as strings
+        out_value = values  # values is always str and user expects str
+    else:
+        # Or possibly convert them first
+        out_value = [unformat_func(val) for val in values]  # convert str -> T using unformat_func
+
+    if as_list:
+        return out_value
+    elif len(out_value) > 1:
+        raise ValueError(f"Got multiple values for query string key {key}. Query contents: \n\n {st.query_params.to_dict()}")
+
+    return out_value[0]
+
+
+@overload
+def from_query_args_index(key: str, options: OptionSequence[T], default: int = 0, unformat_func: Any = str) -> int:
+    ...
+
+@overload
+def from_query_args_index(key: str, options: OptionSequence[T], default: None, unformat_func: Any = str) -> int | None:
+    ...
+
+def from_query_args_index(key: str, options: OptionSequence[T], default: int | None = 0, unformat_func: Any = str) -> int | None:
+    """Return the index in the sequence "options" of the value given for the key in the URL query string.
+
+    If the value is not present in the sequence "options", or if multiple values are provided, returns the default
+    value. This can be used to create a selectbox with a default choice.
+
+    >>> st.selectbox("my box", [1, 2, 3], stu.from_query_args_index("myoption", [1, 2, 3]))
+    """
+    indexible_options = ensure_indexable(options)
+    unformat_func = _infer_common_unformat_funcs(indexible_options, unformat_func)
+    try:
+        return indexible_options.index(from_query_args(key, as_list=False, unformat_func=unformat_func))
+    except ValueError:
+        return default
+
+
+def make_query_string(keys: Collection[str] | None = None, regex: Collection[str | re.Pattern] = ()) -> str:
+    """Get a (relative) URL for a query string of of user-keyed fields on the page and their current values.
+
+    Usage:
+        >>> permalink = stu.make_query_string({"a", "b", "c"})
+        >>> st.markdown(f"[permalink]({permalink})")
+
+    Args:
+        keys (optional, set[str]): The set of keys to be included in the query string.
+        regex (optional, sequence[Pattern]): an optional set of patterns to match with keys as an alternate method of
+            specifying which keys to include.
+
+    Returns:
+        url (str): the relative URL string (everything after the "?")
+
+    Note: This method does NOT guarantee that the URL will return you to this exact session state, as
+    only fields which are watching for a default value from the query string will autopopulate when someone navigates
+    to the URL. When called without arguments, the query string will include values for fields which MAY NOT be watching
+    the query string for values. These will be silently ignored.
+
+    Note: Calling this method will only capture values for fields which have already been rendered, in other words, for
+    >>> stu.make_query_string()
+    >>> stu.number_input_gs("Hello", key="mykey")
+    the make_query_string() call will not always capture the value of "mykey" because the streamlit application has not
+    yet processed that line. At other times it may capture the value of mykey, but the value captured may be "stale"
+    or out-of-date.
+    """
+    return "?" + urllib.parse.urlencode(_qs_intersect(keys, regex), doseq=True)
+
+
+def set_qs_callback(keys: Collection[str] | None = None, regex: Collection[str | re.Pattern] = ()) -> Callable[[], None]:
+    """Return a callable that replaces the browser URL query string with keys-value pairs for the user-defined keys specified.
+
+    Usage:
+        >>> st.button("Update URL!", on_click=stu.set_qs_callback(["field1", "field2"]))
+
+    Args:
+        keys (optional, set[str]): The set of keys to be included in the query string.
+        regex (optional, sequence[Pattern]): an optional set of patterns to match with keys as an alternate method of
+            specifying which keys to include.
+
+
+    Note: This method does NOT guarantee that the URL will return you to this exact session state, as only fields
+    which are watching for a default value from the query string will autopopulate when someone navigates to the URL.
+    When called without arguments, the query string will include values for fields which MAY NOT be watching the query
+    string for values. These will be silently ignored.
+    """
+
+    def _set_qs_callback():
+        st.query_params.clear()
+        st.query_params.update(_qs_intersect(keys, regex))
+
+    return _set_qs_callback
+
+
+def clear_qs_callback(keys: Collection[str] | None = None, regex: Collection[str | re.Pattern] = ()) -> Callable[[], None]:
+    """Return a callable that clears the query string from the URL. If a specific set of keys or patterns are provided,
+    only those keys will be cleared. This callback is designed to be used with the "on_click" or "on_change" argument
+    of a button or widget.
+
+    This will NOT reset the values of any fields that depend on the query string, you must do that yourself by
+    removing the fields' keys from `st.session_state`.
+
+    Args:
+        keys (set[str]): The set of keys to be removed to the query string.
+        regex (optional, sequence[Pattern]): an optional set of patterns to match with keys as an alternate method of
+            specifying which keys to add.
+    """
+
+    if hasattr(st.query_params, "from_dict"):
+        # Streamlit 1.34.0
+        def _clear_qs_callback():
+            if not keys and not regex:
+                st.query_params.clear()
+            else:
+                clear_dict = {k: st.query_params.get_all(k) for k in st.query_params if k not in _qs_intersect(keys, regex)}
+                st.query_params.from_dict(clear_dict)
+    else:
+        # Streamlit 1.33 and earlier (less efficient)
+        def _clear_qs_callback():
+            if not keys and not regex:
+                st.query_params.clear()
+            else:
+                for key in _qs_intersect(keys, regex).keys():
+                    st.query_params.pop(key, None)
+
+    return _clear_qs_callback
+
+
+def add_qs_callback(keys: Collection[str] | None = None, regex: Collection[str | re.Pattern] = ()) -> Callable[[], None]:
+    """Return a callable that adds to the browser URL the keys-value pairs for the user-defined keys specified.
+    Keys with a None value are ignored. Existing key-value pairs in the URL will not be changed or removed
+    (they may be reordered). This callback is designed to be used with the "on_click" or "on_change" argument
+    of a button or widget.
+
+    Args:
+        keys (optional, set[str]): The set of keys to be added to the query string.
+        regex (optional, sequence[Pattern]): an optional set of patterns to match with keys as an alternate method of
+            specifying which keys to add.
+
+    Note: This method does NOT guarantee that the URL will return you to this exact session state, as only fields
+    which are watching for a default value from the query string will autopopulate when someone navigates to the URL.
+    When called without arguments, the query string will include values for fields which MAY NOT be watching the query
+    string for values. These will be silently ignored.
+    """
+
+    def _add_qs_callback():
+        st.query_params.update(_qs_intersect(keys, regex))
+
+    return _add_qs_callback
+
+
+def update_qs_callback(keys: Collection[str] | None = None, regex: Collection[str | re.Pattern] = ()) -> Callable[[], None]:
+    """Return a callable that updates the browser URL with keys-value pairs for the user-defined keys specified.
+    Keys which are paired with a None value are *removed* from the query string. Other existing key-value pairs
+    in the URL will not be changed or removed (they may be reordered). This callback is designed to be used with
+    the "on_click" or "on_change" argument of a button or widget.
+
+    Args:
+        keys (optional, set[str]): The set of keys to be added to the query string.
+        regex (optional, sequence[Pattern]): an optional set of patterns to match with keys as an alternate method of
+            specifying which keys to add.
+
+    Note: This method does NOT guarantee that the URL will return you to this exact session state, as only fields
+    which are watching for a default value from the query string will autopopulate when someone navigates to the URL.
+    When called without arguments, the query string will include values for fields which MAY NOT be watching the query
+    string for values. These will be silently ignored.
+    """
+
+    if hasattr(st.query_params, "from_dict"):
+        # Streamlit 1.34.0
+        def _update_qs_callback():
+            new_dict = _qs_intersect(keys, regex, allownone=True)
+            update_dict = {k: st.query_params.get_all(k) for k in st.query_params}
+            for key, value in new_dict.items():
+                if value is not None:
+                    update_dict[key] = value
+                elif key in update_dict:
+                    del update_dict[key]
+            st.query_params.from_dict(update_dict)  # type: ignore  # doesn't accept a list[str] right now
+    else:
+        # Streamlit 1.33 and earlier (less efficient)
+        def _update_qs_callback():
+            new_dict = _qs_intersect(keys, regex, allownone=True)
+            update_dict = {}
+            for key, value in new_dict.items():
+                if value is not None:
+                    update_dict[key] = value
+                elif key in update_dict:
+                    st.query_params.pop(key)
+            st.query_params.update(update_dict)
+
+    return _update_qs_callback
+
+
+
+def unenumifier(cls: Type[Tenum]) -> Callable[[str], Tenum] :
+    """Get a factory function for turning strings into enum members.
+
+    Python's default Enums render as strings as "<cls>.<member>". This function
+    returns a callable that looks up the member based on this string.
+    """
+    def _unenum(value: str) -> Tenum:
+        """Convert a string into a member of {cls}"""
+        value_name = value.replace(cls.__name__ + ".", "")
+        try:
+            return cls[value_name]
+        except KeyError:
+            raise ValueError(f"'{value_name} is not a valid member of '{cls.__qualname__}'")
+
+    _unenum.__name__ += "_" + cls.__name__
+    _unenum.__doc__ = _unenum.__doc__.format(cls=cls)  # type: ignore
+
+    return _unenum
+
+
+# Helper Functions -----------------------------------------------------------------------------
+
+def _qs_intersect(keys: Collection[str] | None, regex: Collection[str | re.Pattern], allownone: bool = False) -> Mapping[str, Any]:
+    """Get a dictionary containing pairs from st.session_state whose keys match the arguments/patterns."""
+    if isinstance(keys, str) or isinstance(regex, str):
+        raise ValueError("Arguments to query string functions must be non-str collections, e.g. list, tuple, set ...")
+    # Keys are guaranteed to always be strs by SessionStateProxy
+    session_keys = cast(KeysView[str], st.session_state.keys())
+    if keys is None and not regex:
+        use_keys = set(session_keys)
+    else:
+        # Find keys in session_keys that match the regex
+        reg_keys = {key for key in session_keys if any(re.match(pattern, key) for pattern in regex)}
+        # Put the intersection of the string keys and the reg keys together
+        use_keys = (set(keys).intersection(session_keys) if keys else set()) | reg_keys
+
+    # Return the new query string dictionary, but filter out blacklisted keys and None values
+    return {
+        key: st.session_state[key] for key in use_keys if key not in QS_BLACKLIST_KEYS and (allownone or st.session_state[key] is not None)
+    }
+
+
+def _wrap_on_change_with_qs_update(key: str, kwargs: MutableMapping, remove_none_values: bool):
+    """Mutates kwargs to add a query string update for the specified key to the on_change argument."""
+    existing_callback: Callable | None = kwargs.get("on_change", None)
+
+    # Select the right kind of callback
+    if remove_none_values:
+        pre_update_func = update_qs_callback(keys=(key,))
+    else:
+        pre_update_func = add_qs_callback(keys=(key,))
+
+    # Use the existing function if there's not one already defined for on_change.
+    if existing_callback is None:
+        kwargs["on_change"] = pre_update_func
+        return
+    elif not callable(existing_callback):
+        raise TypeError(f"'on_change' keyword argument is not callable: {existing_callback}")
+
+    # Otherwise decorate the existing function with an update to the query params beforehand
+    @functools.wraps(existing_callback)
+    def wrapper(*args, **kwargs):
+        pre_update_func()
+        existing_callback(*args, **kwargs)
+
+    # At the end, mutate kwargs
+    kwargs["on_change"] = wrapper
+
+
+def _convert_bool_checkbox(string_bool: str, default: bool) -> bool:
+    """Convert from string values to boolean values, with a default value if conversion fails."""
+    if string_bool.lower() in ("1", "true"):
+        return True
+    elif string_bool.lower() in ("0", "false"):
+        return False
+    return default
+
+
+@overload
+def _ensure_list(maybe_list: Tbs) -> List[Tbs]:
+    ...
+
+@overload
+def _ensure_list(maybe_list: Sequence[T]) -> List[T]:
+    ...
+
+@overload
+def _ensure_list(maybe_list: T) -> List[T]:
+    ...
+
+def _ensure_list(maybe_list):
+    """Convert single values and sequences (except bytes and str) to lists."""
+    if isinstance(maybe_list, list):
+        return maybe_list
+    elif isinstance(maybe_list, (bytes, str)) or not isinstance(maybe_list, Sequence):
+        return [maybe_list]
+    else:
+        return list(maybe_list)
+
+
+def _infer_common_unformat_funcs(indexible_options: Sequence[Any], unformat_func):
+    """Infers some common unformat_funcs based on the items in the indexible_options and returns the new function."""
+    if unformat_func is str and len(indexible_options)!=0 and not all(isinstance(opt, str) for opt in indexible_options):
+        # If they're ints or floats or bytes (uniformly), coerce back to those.
+        for typ in (int, float, bytes):
+            if all(isinstance(opt, typ) for opt in indexible_options):
+                return typ
+
+        # If they all come from the same enum, coerce back to that
+        if isinstance(indexible_options[0], Enum):
+            enum_cls = indexible_options[0].__class__
+            if all(isinstance(opt, enum_cls) for opt in indexible_options):
+                return unenumifier(enum_cls)
+
+    _warn_on_common_unmatching_unformat_functions(indexible_options, unformat_func)
+    return unformat_func
+
+
+def _warn_on_common_unmatching_unformat_functions(options, unformat_func):
+    """Produces a warning if the user registers non-string options but provides or leaves the
+    default "str" as an unformat_func."""
+    if DISABLE_WARNINGS:
+        return
+    if not all(isinstance(opt, str) for opt in options) and unformat_func is str:
+        detected_types = {type(opt) for opt in options}
+        msg = f"""In the widget below, you've used a select or multi-select streamlit_qs element
+with non-string-type options (we found {detected_types}), but did not provide an `unformat_func`
+to deserialize the values from the URL back into those objects, and we could not deduce one for you.
+For example, you may have tried something like
+
+    st.selectbox_qs("Pick a number", options=[1, 1.5, 2], key="picknumber")
+
+To do this correctly, you need to explicitly specify how to convert the values in the URL back to options.
+In this case you might define a function like
+
+    def int_or_float(string):
+        try: return int(string)
+        except ValueError: pass
+        return float(string)
+
+And then call
+
+    st.selectbox_qs("Pick a number", options=[1, 1.5, 2], key="pickanumber", unformat_func=int_or_float)
+
+    """
+        st.exception(StreamlitAPIWarning(msg))
+        st._logger.get_logger(__name__).warning(msg, stack_info=True, stacklevel=5)
+
+
+def _raise_if_option_is_none(indexible_options, widgettype="widget that supports section from a list of options"):
+    """Raises an exception if the user tries to pass None as an option. While this is technically allowed
+    with the base streamlit widgets, we can't serialize "None" to the URL string in a way that is differentiable
+    from the string "None" as well as the None value that some widgets can now return in Streamlit 1.27.0+. So we
+    must disallow it."""
+    if any(opt is None for opt in indexible_options):
+        msg = f"""You may not pass the value None as an item to a streamlit_qs {widgettype}, as there is no reliable
+way to serialize this value to the URL query string. If you are trying to create a widget with an empty default value,
+please pass None as the 'default' argument instead of adding to the 'options' list.
+
+Got the following options: {indexible_options}
+        """
+        raise StreamlitAPIException(msg)
```

### Comparing `streamlit-qs-0.3.1/streamlit_qs.egg-info/PKG-INFO` & `streamlit_qs-0.3.2/streamlit_qs.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,53 +1,54 @@
-Metadata-Version: 2.1
-Name: streamlit-qs
-Version: 0.3.1
-Summary: A small library to add extra functionality on top of streamlit's st.query_params API
-Home-page: https://github.com/Asaurus1/streamlit-qs
-Author: Alexander Martin
-Author-email: fauxjunk-1@yahoo.com
-License: Apache 2
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Query String functions for Streamlit
-This app shows off the [Query String Utility Functions](https://github.com/Asaurus1/streamlit-qs) for Streamlit.
-
-The functions in this library allow you to easily create "permalink-like" functionality in your application,
-This can let users to share links with others that will populate streamlit with the same set of input values
-that they were using. Or you can use the query string to pass data into your streamlit application from
-another website or program.
-
-
-## Installation
-
-First install Streamlit (of course!) then install this library:
-
-```bash
-pip install streamlit-qs
-```
-or
-```bash
-pip install git+https://github.com/Asaurus1/streamlit-qs.git@main
-```
-
-## Example
-
-```python
-import streamlit as st
-import streamlit_qs as stqs
-
-st.markdown("[Click this URL](?input_some_text=Hello+World)") 
-stqs.text_input_qs("Enter Some Text", key="input_some_text")
-```
-
-For more examples, including :sparkles:**customization options**:sparkles:, see
-[the demo app](https://query-string.streamlit.app/).
-
-
-## Version Compatibility
-For Streamlit v1.29.0 or below use release v0.2.0 of this app
-For Streamlit v1.30.0 or above, use the latest released version of this app above v0.2.0
+Metadata-Version: 2.1
+Name: streamlit-qs
+Version: 0.3.2
+Summary: A small library to add extra functionality on top of streamlit's st.query_params API
+Home-page: https://github.com/Asaurus1/streamlit-qs
+Author: Alexander Martin
+Author-email: fauxjunk-1@yahoo.com
+License: Apache 2
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: streamlit>=1.30.0
+
+# Query String functions for Streamlit
+This app shows off the [Query String Utility Functions](https://github.com/Asaurus1/streamlit-qs) for Streamlit.
+
+The functions in this library allow you to easily create "permalink-like" functionality in your application,
+This can let users to share links with others that will populate streamlit with the same set of input values
+that they were using. Or you can use the query string to pass data into your streamlit application from
+another website or program.
+
+
+## Installation
+
+First install Streamlit (of course!) then install this library:
+
+```bash
+pip install streamlit-qs
+```
+or
+```bash
+pip install git+https://github.com/Asaurus1/streamlit-qs.git@main
+```
+
+## Example
+
+```python
+import streamlit as st
+import streamlit_qs as stqs
+
+st.markdown("[Click this URL](?input_some_text=Hello+World)") 
+stqs.text_input_qs("Enter Some Text", key="input_some_text")
+```
+
+For more examples, including :sparkles:**customization options**:sparkles:, see
+[the demo app](https://query-string.streamlit.app/).
+
+
+## Version Compatibility
+For Streamlit v1.29.0 or below use release v0.2.0 of this app
+For Streamlit v1.30.0 or above, use the latest released version of this app above v0.2.0
```

### Comparing `streamlit-qs-0.3.1/tests/test_streamlit_qs.py` & `streamlit_qs-0.3.2/tests/test_streamlit_qs.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,539 +1,528 @@
-from enum import Enum
-from typing import Any, Dict
-import unittest.mock as mock
-
-import pytest
-import streamlit as st
-from streamlit.errors import StreamlitAPIException, StreamlitAPIWarning
-
-import streamlit_qs as stqs
-
-
-@pytest.fixture
-def session_state():
-    with mock.patch("streamlit.session_state", new={}) as ss:  # type: ignore
-        yield ss
-
-@pytest.fixture
-def mock_qp():
-    with mock.patch("streamlit.query_params", spec=st.query_params) as mock_qp:
-        mock_qp.__mock_dict = {}
-        mock_qp.get_all = lambda key: mock_qp.__mock_dict.get(key, [])
-        yield mock_qp
-
-@pytest.fixture
-def mock_pop(mock_qp):
-    return mock_qp.pop
-
-
-@pytest.fixture
-def mock_update(mock_qp):
-    return mock_qp.update
-
-
-@pytest.fixture
-def mock_setitem(mock_qp):
-    return mock_qp.__setitem__
-
-
-@pytest.fixture
-def mock_from_query_args():
-    with mock.patch("streamlit_qs.from_query_args") as mock_from_query_args:
-        yield mock_from_query_args
-
-
-@pytest.fixture
-def mock_query_args_index():
-    with mock.patch("streamlit_qs.from_query_args_index") as mock_from_query_args_index:
-        yield mock_from_query_args_index
-
-
-def test_from_query_args_str(mock_qp: mock.MagicMock):
-    mock_qp.__mock_dict = {"a": ["1"], "b": ["2"], "c": ["3", "4"]}
-    deflist = ["default"]
-    stqs.from_query_args("a") == "1"
-    stqs.from_query_args("b", "default") == "2"
-    stqs.from_query_args("b", None) == "2"
-    stqs.from_query_args("c", deflist, as_list=True) == ["3", "4"]
-    stqs.from_query_args("d", "default") == "default"
-    stqs.from_query_args("d", None) is None
-    stqs.from_query_args("e", deflist, as_list=True) is deflist
-    with pytest.raises(ValueError):
-        stqs.from_query_args("c", "5") != ["3", "4"]  # type: ignore
-
-
-def test_from_query_args_nonstr(mock_qp: mock.MagicMock):
-    mock_qp.__mock_dict = {"a": ["1"], "b": ["2"], "c": ["3", "4"]}
-    stqs.from_query_args("a", unformat_func=int) == 1
-    stqs.from_query_args("b", "default", unformat_func=int) == 2
-    stqs.from_query_args("c", [5], as_list=True, unformat_func=int) == [3, 4]
-    stqs.from_query_args("d", 5, unformat_func=int) == 5
-
-
-def test_from_query_args_index_str(mock_from_query_args: mock.MagicMock):
-    mock_from_query_args.return_value = "1"
-    options = ["3", "1", "5"]
-    stqs.from_query_args_index("a", options) == 1
-    mock_from_query_args.return_value = "10"
-    stqs.from_query_args_index("b", options, default=99) == 99
-    stqs.from_query_args_index("b", options, default=None) == None
-
-
-def test_from_query_args_index_nonstr(mock_from_query_args: mock.MagicMock):
-    mock_from_query_args.return_value = 1
-    options = [3, 1, 5]
-    stqs.from_query_args_index("a", options, unformat_func=int) == 1
-    mock_from_query_args.return_value = 10
-    stqs.from_query_args_index("b", options, default=99, unformat_func=int) == 99
-
-
-def test_selectbox_qs(mock_query_args_index: mock.MagicMock, session_state):
-    mock_query_args_index.return_value = 1
-    stqs.selectbox_qs("Test", ["a", "b", "c"], key="test")
-    assert session_state["test"] == "b"
-    mock_query_args_index.assert_called_with("test", ["a", "b", "c"], default=0, unformat_func=str)
-    stqs.selectbox_qs("Test", [1, 2, 3], key="test2", unformat_func=int)
-    assert session_state["test2"] == 2
-    mock_query_args_index.assert_called_with("test2", [1, 2, 3], default=0, unformat_func=int)
-
-    assert _test_helper_autoupdate(stqs.selectbox_qs, "Test", ["a", "b", "c"], key="test3", autoupdate=True)
-    assert session_state["test3"] == "b"
-
-    with pytest.raises(TypeError):
-        # can't call without key
-        stqs.selectbox_qs("Test", [1, 2, 3])  # type: ignore
-
-    with pytest.raises(StreamlitAPIException):
-        stqs.selectbox_qs("Test", options=[1, 2, None], key="badtest")
-
-
-def test_radio_qs(mock_query_args_index: mock.MagicMock, session_state):
-    mock_query_args_index.return_value = 1
-    stqs.radio_qs("Test", ["a", "b", "c"], key="test")
-    assert session_state["test"] == "b"
-    mock_query_args_index.assert_called_with("test", ["a", "b", "c"], default=0, unformat_func=str)
-    stqs.radio_qs("Test", [1, 2, 3], key="test2", unformat_func=int) == 2
-    mock_query_args_index.assert_called_with("test2", [1, 2, 3], default=0, unformat_func=int)
-
-    assert _test_helper_autoupdate(stqs.radio_qs, "Test", ["a", "b", "c"], key="test3", autoupdate=True)
-    assert session_state["test3"] == "b"
-
-    with pytest.raises(TypeError):
-        # can't call without key
-        stqs.radio_qs("Test", [1, 2, 3])  # type: ignore
-
-    with pytest.raises(StreamlitAPIException):
-        stqs.radio_qs("Test", options=[1, 2, None], key="badtest")
-
-
-@mock.patch("streamlit.multiselect", wraps=st.multiselect)
-def test_multiselect_qs_strings(mock_ms: mock.MagicMock, mock_from_query_args: mock.MagicMock, session_state):
-    options = ["3", "1", "5"]
-
-    mock_from_query_args.return_value = ["1"]
-    stqs.multiselect_qs("Test", options, key="test")
-    assert session_state["test"] == ["1"]
-    mock_ms.assert_called_with("Test", options, default=None, key="test")
-
-    mock_from_query_args.return_value = ["1", "5", "7"]
-    stqs.multiselect_qs("Test", options, key="test2")
-    assert session_state["test2"] == ["1", "5"]
-    mock_ms.assert_called_with("Test", options, default=None, key="test2")
-
-    mock_from_query_args.return_value = ["1", "3"]
-    stqs.multiselect_qs("Test", options, default=["1", "3"], key="test3")
-    "test3" not in session_state
-    mock_ms.assert_called_with("Test", options, default=["1", "3"], key="test3")
-
-    mock_from_query_args.return_value = ["3"]
-    stqs.multiselect_qs("Test", options, default="3", key="test4")
-    mock_ms.assert_called_with("Test", options, default="3", key="test4")
-
-    mock_from_query_args.return_value = []
-    stqs.multiselect_qs("Test", options, key="test5")
-    mock_ms.assert_called_with("Test", options, default=None, key="test5")
-
-    mock_from_query_args.return_value = []
-    _test_helper_autoupdate(stqs.multiselect_qs, "Test", options, key="test6", autoupdate=True)
-
-    mock_from_query_args.return_value = ["1", "5", "7"]
-    with pytest.raises(ValueError):
-        stqs.multiselect_qs("Test", options, key="test7", discard_missing=False) != ["1", "5"]
-
-    with pytest.raises(TypeError):
-        # can't call without key
-        stqs.multiselect_qs("Test", ["1", "2", "3"])  # type: ignore
-
-
-@mock.patch("streamlit.multiselect", wraps=st.multiselect)
-def test_multiselect_qs_nonstring(mock_ms: mock.MagicMock, mock_from_query_args: mock.MagicMock, session_state):
-    options = [1, 3, 5]
-
-    mock_from_query_args.return_value = [1]
-    stqs.multiselect_qs("Test", options, key="test", unformat_func=int)
-    assert session_state["test"] == [1]
-    mock_ms.assert_called_with("Test", options, default=None, key="test")
-
-    mock_from_query_args.return_value = [1, 2, 3]
-    stqs.multiselect_qs("Test", options, key="test2", unformat_func=lambda x: len(x))
-    assert session_state["test2"] == [1, 3]
-    mock_ms.assert_called_with("Test", options, default=None, key="test2")
-
-    mock_from_query_args.return_value = [1, 5]
-    stqs.multiselect_qs("Test", options, default=[1, 5], key="test3")
-    "test3" not in session_state
-    mock_ms.assert_called_with("Test", options, default=[1, 5], key="test3")
-
-    mock_from_query_args.return_value = []
-    stqs.multiselect_qs("Test", options, key="test4")
-    mock_ms.assert_called_with("Test", options, default=None, key="test4")
-
-    with pytest.raises(StreamlitAPIException):
-        stqs.multiselect_qs("Test", options=[1, 2, None], key="badtest")
-
-
-def test_checkbox_qs(mock_from_query_args: mock.MagicMock, session_state):
-    for val in ("1", "True", "tRue", "TRUE"):
-        mock_from_query_args.return_value = stqs._convert_bool_checkbox(val, False)
-        stqs.checkbox_qs("Test", key="test")
-        assert session_state["test"] is True
-    for val in ("0", "FALSE", "False", "false"):
-        mock_from_query_args.return_value = stqs._convert_bool_checkbox(val, False)
-        stqs.checkbox_qs("Test", key="test2")
-        assert session_state["test2"] is False
-
-    mock_from_query_args.return_value = stqs._convert_bool_checkbox("TROO", True)
-    stqs.checkbox_qs("Test", key="test3", default=True)
-    assert session_state["test3"] is True
-    mock_from_query_args.return_value = stqs._convert_bool_checkbox("TROO", False)
-    stqs.checkbox_qs("Test", key="test4", default=False)
-    assert session_state["test4"] is False
-    
-    mock_from_query_args.return_value = False
-    _test_helper_autoupdate(stqs.checkbox_qs, "Test", key="test5", autoupdate=True)
-    assert session_state["test5"] is False
-
-    with pytest.raises(TypeError):
-        # can't call without key
-        stqs.selectbox_qs("Test", [1, 2])  # type: ignore
-
-
-def test_text_input_qs(mock_from_query_args: mock.MagicMock, session_state):
-    mock_from_query_args.return_value = "hello"
-    stqs.text_input_qs("Test", default="world", key="test")
-    assert session_state["test"] == "hello"
-    mock_from_query_args.assert_called_with("test", default="world")
-
-    _test_helper_autoupdate(stqs.text_input_qs, "Test", key="test2", autoupdate=True)
-    assert session_state["test2"] == "hello"
-
-    mock_from_query_args.side_effect = ValueError("multiple values")
-    with pytest.raises(ValueError):
-        stqs.text_input_qs("Test", key="a")
-    with pytest.raises(TypeError):
-        # can't call without key
-        stqs.text_input_qs("Test", [1, 2])  # type: ignore
-
-
-def test_text_area_qs(mock_from_query_args, session_state):
-    mock_from_query_args.return_value = "hello"
-    stqs.text_area_qs("Test", default="world", key="test")
-    assert session_state["test"] == "hello"
-    mock_from_query_args.assert_called_with("test", default="world")
-
-    _test_helper_autoupdate(stqs.text_area_qs, "Test", key="test2", autoupdate=True)
-    assert session_state["test2"] == "hello"
-
-    mock_from_query_args.side_effect = ValueError("multiple values")
-    with pytest.raises(ValueError):
-        stqs.text_area_qs("Test", key="a")
-    with pytest.raises(TypeError):
-        # can't call without key
-        stqs.text_area_qs("Test")  # type: ignore
-
-
-def test_number_input_qs(mock_from_query_args, session_state):
-    mock_from_query_args.return_value = "hello"
-    val = stqs.number_input_qs("Test", default=4, key="test0")
-    # When query string invalid and default=="min" we dont expect session_state to get set
-    assert "test0" not in session_state
-    assert val == 4 and isinstance(val, int)
-
-    mock_from_query_args.return_value = "hello"
-    val = stqs.number_input_qs("Test", key="test1")
-    # When query string invalid and default=="min" we dont expect session_state to get set
-    assert "test1" not in session_state
-    assert val == 0.0 and isinstance(val, float)
-
-    mock_from_query_args.return_value = "6"
-    stqs.number_input_qs("Test", default=5.0, key="test2")
-    val = session_state["test2"]
-    assert val == 6.0 and isinstance(val, float)
-    stqs.number_input_qs("Test", default=4, key="test3")
-    val = session_state["test3"]
-    assert val == 6 and isinstance(val, int)
-    stqs.number_input_qs("Test", min_value=5, key="test4")
-    val = session_state["test4"]
-    assert val == 6 and isinstance(val, int)
-    stqs.number_input_qs("Test", max_value=7, key="test5")
-    val = session_state["test5"]
-    assert val == 6 and isinstance(val, int)
-    stqs.number_input_qs("Test", max_value=4, key="test5.1")  # it even lets you go outside normal bounds?
-    val = session_state["test5.1"]
-    assert val == 6 and isinstance(val, int)
-    stqs.number_input_qs("Test", step=4.5, key="test6")
-    val = session_state["test6"]
-    assert val == 6.0 and isinstance(val, float)
-    stqs.number_input_qs("Test", key="test7")
-    val = session_state["test7"]
-    assert val == 6.0 and isinstance(val, float)
-
-    stqs.number_input_qs("Test", default=None, key="test8")
-    val = session_state["test8"]
-    assert val == 6.0 and isinstance(val, float)
-
-    mock_from_query_args.return_value = "NOT_A_NUMBER"
-    assert _test_helper_autoupdate(stqs.number_input_qs, "Test", key="test9", autoupdate=True) == 0
-    assert "test9" not in session_state
-    assert stqs.number_input_qs("Test", default=None, key="test10") is None
-    assert "test10" not in session_state
-
-    mock_from_query_args.return_value = None
-    assert stqs.number_input_qs("Test", key="test11") == 0
-    assert "test11" not in session_state
-    assert stqs.number_input_qs("Test", default=5.0, key="test12") == 5.0
-    assert "test12" not in session_state
-    assert stqs.number_input_qs("Test", max_value=5, key="test13") == 0
-    assert "test13" not in session_state
-
-    mock_from_query_args.side_effect = ValueError("multiple values")
-    with pytest.raises(ValueError):
-        stqs.number_input_qs("Test", key="a")
-
-    mock_from_query_args.side_effect = None
-    mock_from_query_args.return_value = "6"
-    with pytest.raises(TypeError, match="Expected type was not a float"):
-        stqs.number_input_qs("Test", min_value="string", key="test")  # bad type with no default
-    with pytest.raises(TypeError, match="Expected type was not a float"):
-        stqs.number_input_qs("Test", max_value="string", key="test")  # bad type with no default
-    with pytest.raises(TypeError, match="Expected type was not a float"):
-        stqs.number_input_qs("Test", step="string", key="test")  # bad type with no default
-    with pytest.raises(TypeError, match="keyword-only"):
-        # can't call without key
-        stqs.number_input_qs("Test")  # type: ignore
-
-
-def test_qs_intersect():
-    new_session_state1 = {"a3": 1, "b3": 2, "b2": 3}
-    with mock.patch("streamlit.session_state", new=new_session_state1):
-        stqs._qs_intersect(None, tuple()) == new_session_state1
-        stqs._qs_intersect(tuple(), tuple()) == {}  # i.e. if the user passes in keys=[]
-        stqs._qs_intersect(["a3", "b3"], tuple()) == {"a3": 1, "b3": 2}
-        stqs._qs_intersect(["a3", "badval"], tuple()) == {"a3": 1}
-        stqs._qs_intersect(None, ["b.$"]) == {"b2": 3, "b3": 2}
-        stqs._qs_intersect(["a3"], ["b.$"]) == {"a3": 1, "b2": 3, "b3": 2}
-
-    new_session_state2 = {"a3": 1, "blacklisted_key": "blacklisted"}
-    with mock.patch("streamlit.session_state", new=new_session_state2):
-        stqs.blacklist_key("blacklisted_key")
-        stqs._qs_intersect(None, tuple()) == {"a3": 1}
-        stqs.unblacklist_key("blacklisted_key")
-        assert "blacklisted_key" not in stqs.QS_BLACKLIST_KEYS
-
-    with pytest.raises(ValueError, match="Arguments to query string functions must be non-str collections"):
-        stqs._qs_intersect("foo", tuple())
-    with pytest.raises(ValueError, match="Arguments to query string functions must be non-str collections"):
-        stqs._qs_intersect(None, "foo")
-
-
-def test_make_query_string(session_state):
-    session_state.update({"a3": 1, "b3": "hello world", "b2": 3})
-    assert all(kv in stqs.make_query_string() for kv in ["?", "a3=1", "b3=hello+world", "b2=3"])
-    assert all(kv in stqs.make_query_string(regex=["b.$"]) for kv in ["?", "b3=hello+world", "b2=3"])
-    stqs.make_query_string(["b3"]) == "?b3=hello+world"
-
-
-def test_set_qs_callback(mock_update, session_state):
-    session_state.update({"a3": 1, "b3": "hello world", "b2": 3})
-
-    func = stqs.set_qs_callback(["a3", "b3"], regex=[])
-    mock_update.assert_not_called()
-    func()
-    mock_update.assert_called_with(dict(a3=1, b3="hello world"))
-    mock_update.reset_mock()
-
-    assert stqs.set_qs_callback()() is None
-    mock_update.assert_called_with(dict(a3=1, b3="hello world", b2=3))
-    mock_update.reset_mock()
-
-
-def test_add_qs_callback(mock_qp, mock_update, session_state):
-    session_state.update({"a3": 1, "b3": "hello world", "b2": 3, "nonekey": None})
-
-    mock_qp.__mock_dict = {"a1": "hi", "nonekey": "5"}
-    func = stqs.add_qs_callback(["b2"], regex=[])
-    mock_update.assert_not_called()
-    func()
-    mock_update.assert_called_with(dict(b2=3))
-
-    assert stqs.add_qs_callback(["nonekey"])() is None
-    mock_update.assert_called_with(dict())
-    mock_update.reset_mock()
-
-
-def test_update_qs_callback(mock_qp, mock_setitem, session_state):
-    session_state.update({"a3": 1, "b3": "hello world", "b2": 3, "nonekey": None})
-
-    mock_qp.__mock_dict = {"a1": "hi", "nonekey": "5"}
-    func = stqs.update_qs_callback(["b2"], regex=[])
-    mock_setitem.assert_not_called()
-    func()
-    mock_setitem.has_calls(
-        mock.call("a1", "hi"),
-        mock.call("b2", 3),
-        mock.call("nonekey", 5)
-    )
-    mock_setitem.reset_mock()
-
-    assert stqs.update_qs_callback(["nonekey"])() is None
-    mock_setitem.has_calls(
-        mock.call("a1", "hi"),
-        mock.call("b2", 3),
-    )
-    mock_setitem.reset_mock()
-
-    assert stqs.update_qs_callback()() is None
-    mock_setitem.has_calls(
-        mock.call("a1", "hi"),
-        mock.call("b2", 3),
-        mock.call("b3", "hello world"),
-        mock.call("a3", 1),
-    )
-    mock_setitem.reset_mock()
-
-
-def test_clear_qs_callback(mock_qp, session_state):
-    session_state.update({"a3": 1, "b3": "hello world", "b2": 3, "nonekey": None})
-
-    func = stqs.clear_qs_callback()
-    mock_qp.clear.assert_not_called()
-    func()
-    mock_qp.clear.assert_called_once()
-
-    mock_qp.__mock_dict = {"a1": "hi", "b3": "world"}
-    assert stqs.clear_qs_callback(["b3"])() is None
-    mock_qp.pop.assert_called_with("b3", None)
-
-
-def test_wrap_on_chage_with_qs_update(mock_qp, mock_setitem, mock_pop, mock_update, session_state):
-    kwargs: Any = {"foo": "a", "bar": "b", "none": None}
-    stqs._wrap_on_change_with_qs_update("key", kwargs, remove_none_values=False)
-    assert callable(kwargs["on_change"])
-    assert kwargs["on_change"].__name__ == "_add_qs_callback"
-    mock_update.assert_not_called()
-    mock_qp.__mock_dict = {"key": "hi"}
-    kwargs["on_change"]()
-    mock_update.assert_called_with(dict())
-
-    callback = mock.MagicMock(__name__="mockfunction")
-    kwargs = {"foo": "a", "bar": "b", "on_change": callback}
-    stqs._wrap_on_change_with_qs_update("key", kwargs, remove_none_values=True)
-    assert callable(kwargs["on_change"])
-    assert kwargs["on_change"].__name__ == "mockfunction"
-    assert kwargs["on_change"] is not callback
-    callback.assert_not_called()
-    mock_pop.assert_not_called()
-    mock_qp.__mock_dict = {"key": "a", "foobar": "b"}
-    session_state["key"] = None
-    kwargs["on_change"]()
-    callback.assert_called()
-    mock_pop.assert_called_with("key", None)
-    mock_pop.reset_mock()
-
-    kwargs = {"foo": "a", "bar": "b", "on_change": 1}
-    with pytest.raises(TypeError, match="keyword argument is not callable"):
-        stqs._wrap_on_change_with_qs_update("key", kwargs, remove_none_values=True)
-
-
-def _test_helper_autoupdate(func, *args, **kwargs):
-    """Helper function to test an "autoupdate" call"""
-
-    # patch the wrap on change function
-    with mock.patch("streamlit_qs._wrap_on_change_with_qs_update") as mock_wrap:
-        # Add autoupdate=True as a kwarg if it hasn't been by the caller
-        kwargs.update(autoupdate=True)
-        # Call the function under test
-        retval = func(*args, **kwargs)
-        # assert that wrap_on_change was called
-        mock_wrap.assert_called()
-    # Return whatever was returned by the function under test
-    return retval
-
-
-def test_unenumifier():
-    class AnEnum(Enum):
-        FOO = 0
-        BAR = 1
-
-    class NotAnEnum:
-        ...
-
-    unenumifier = stqs.unenumifier(AnEnum)
-    assert callable(unenumifier)
-    assert unenumifier("FOO") == AnEnum.FOO
-    assert unenumifier("AnEnum.BAR") == AnEnum.BAR
-    with pytest.raises(ValueError):
-        unenumifier("invalid")
-    with pytest.raises(AttributeError):
-        stqs.unenumifier("foo")  # type: ignore
-    with pytest.raises(TypeError):
-        stqs.unenumifier(NotAnEnum)("FOO")  # type: ignore
-
-
-def test_ensure_list():
-    assert stqs._ensure_list("abc") == ["abc"]
-    assert stqs._ensure_list(b"abc") == [b"abc"]
-    assert stqs._ensure_list((5, 6, 7)) == [5, 6, 7]
-    assert stqs._ensure_list([1, 2, 3]) == [1, 2, 3]
-    assert stqs._ensure_list(5) == [5]
-
-
-def test_infer_unformat_func():
-    class AnEnum(Enum):
-        FOO = 0
-        BAR = 1
-
-    assert stqs._infer_common_unformat_funcs([1, 2, 3], str) is int
-    assert stqs._infer_common_unformat_funcs([1.0, 2.0, 3.0], str) is float
-    assert stqs._infer_common_unformat_funcs([AnEnum.FOO, AnEnum.BAR], str).__name__ == "_unenum_AnEnum"
-
-    assert stqs._infer_common_unformat_funcs([1, 2, 3.0], str) is str
-    assert stqs._infer_common_unformat_funcs([1.0, 2.0, AnEnum.FOO], str) is str
-    assert stqs._infer_common_unformat_funcs([AnEnum.FOO, AnEnum.BAR, "AnEnum.BAZ"], str) is str
-
-    assert stqs._infer_common_unformat_funcs([1, 2, 3], float) is float
-    assert stqs._infer_common_unformat_funcs([1.0, 2.0, 3.0], int) is int
-    def enum_unformat(e): return e.name
-    assert stqs._infer_common_unformat_funcs([AnEnum.FOO, AnEnum.BAR], enum_unformat) is enum_unformat
-
-
-@mock.patch("streamlit.exception")
-def test_warn_on_common_unmatching_unformat_funcs(mock_warning):
-    stqs._warn_on_common_unmatching_unformat_functions([1, 2, 3], str)
-    assert isinstance(mock_warning.call_args[0][0], StreamlitAPIWarning)
-    assert repr({int}) in str(mock_warning.call_args[0][0])
-
-    stqs._warn_on_common_unmatching_unformat_functions([1, 2.0, "str"], str)
-    assert isinstance(mock_warning.call_args[0][0], StreamlitAPIWarning)
-    assert repr({int, float, str}) in str(mock_warning.call_args[0][0])
-
-    stqs._warn_on_common_unmatching_unformat_functions([StreamlitAPIException(), StreamlitAPIWarning()], str)
-    assert isinstance(mock_warning.call_args[0][0], StreamlitAPIWarning)
-    assert repr({StreamlitAPIException, StreamlitAPIWarning}) in str(mock_warning.call_args[0][0])
-
-    mock_warning.reset_mock()  # remaining tests should NOT call this
-    stqs._warn_on_common_unmatching_unformat_functions([StreamlitAPIException(), StreamlitAPIWarning()], int)
-    stqs._warn_on_common_unmatching_unformat_functions([1, 2.0, "str"], float)
-    stqs._warn_on_common_unmatching_unformat_functions([1, 2, 3], float)
-    stqs._warn_on_common_unmatching_unformat_functions([1, 2, 3], int)
-    mock_warning.assert_not_called()
+from enum import Enum
+from typing import Any, Dict
+import unittest.mock as mock
+
+import pytest
+import streamlit as st
+from streamlit.runtime.state.query_params import QueryParams
+from streamlit.errors import StreamlitAPIException, StreamlitAPIWarning
+
+import streamlit_qs as stqs
+
+
+@pytest.fixture
+def session_state():
+    with mock.patch("streamlit.session_state", new={}) as ss:  # type: ignore
+        yield ss
+
+@pytest.fixture
+def qp():
+    # Replace the Proxy "query_params" with the underlying object
+    with mock.patch("streamlit.query_params", new=QueryParams({})) as qp:
+        yield qp
+
+@pytest.fixture
+def streamlit_1_33(qp):
+    QueryParams._from_dict = QueryParams.from_dict  # type: ignore[attr-defined]
+    del QueryParams.from_dict
+    try:
+        yield
+    finally:
+        QueryParams.from_dict = QueryParams._from_dict  # type: ignore[method-assign, attr-defined]
+
+
+@pytest.fixture
+def mock_from_query_args():
+    with mock.patch("streamlit_qs.from_query_args") as mock_from_query_args:
+        yield mock_from_query_args
+
+
+@pytest.fixture
+def mock_query_args_index():
+    with mock.patch("streamlit_qs.from_query_args_index") as mock_from_query_args_index:
+        yield mock_from_query_args_index
+
+
+def test_from_query_args_str(qp: QueryParams):
+    qp._query_params = {"a": ["1"], "b": ["2"], "c": ["3", "4"]}
+    deflist = ["default"]
+    stqs.from_query_args("a") == "1"
+    stqs.from_query_args("b", "default") == "2"
+    stqs.from_query_args("b", None) == "2"
+    stqs.from_query_args("c", deflist, as_list=True) == ["3", "4"]
+    stqs.from_query_args("d", "default") == "default"
+    stqs.from_query_args("d", None) is None
+    stqs.from_query_args("e", deflist, as_list=True) is deflist
+    with pytest.raises(ValueError):
+        stqs.from_query_args("c", "5") != ["3", "4"]  # type: ignore
+
+
+def test_from_query_args_nonstr(qp: QueryParams):
+    qp._query_params = {"a": ["1"], "b": ["2"], "c": ["3", "4"]}
+    stqs.from_query_args("a", unformat_func=int) == 1
+    stqs.from_query_args("b", "default", unformat_func=int) == 2
+    stqs.from_query_args("c", [5], as_list=True, unformat_func=int) == [3, 4]
+    stqs.from_query_args("d", 5, unformat_func=int) == 5
+
+
+def test_from_query_args_index_str(mock_from_query_args: mock.MagicMock):
+    mock_from_query_args.return_value = "1"
+    options = ["3", "1", "5"]
+    stqs.from_query_args_index("a", options) == 1
+    mock_from_query_args.return_value = "10"
+    stqs.from_query_args_index("b", options, default=99) == 99
+    stqs.from_query_args_index("b", options, default=None) == None
+
+
+def test_from_query_args_index_nonstr(mock_from_query_args: mock.MagicMock):
+    mock_from_query_args.return_value = 1
+    options = [3, 1, 5]
+    stqs.from_query_args_index("a", options, unformat_func=int) == 1
+    mock_from_query_args.return_value = 10
+    stqs.from_query_args_index("b", options, default=99, unformat_func=int) == 99
+
+
+def test_selectbox_qs(mock_query_args_index: mock.MagicMock, session_state):
+    mock_query_args_index.return_value = 1
+    stqs.selectbox_qs("Test", ["a", "b", "c"], key="test")
+    assert session_state["test"] == "b"
+    mock_query_args_index.assert_called_with("test", ["a", "b", "c"], default=0, unformat_func=str)
+    stqs.selectbox_qs("Test", [1, 2, 3], key="test2", unformat_func=int)
+    assert session_state["test2"] == 2
+    mock_query_args_index.assert_called_with("test2", [1, 2, 3], default=0, unformat_func=int)
+
+    assert _test_helper_autoupdate(stqs.selectbox_qs, "Test", ["a", "b", "c"], key="test3", autoupdate=True)
+    assert session_state["test3"] == "b"
+
+    with pytest.raises(TypeError):
+        # can't call without key
+        stqs.selectbox_qs("Test", [1, 2, 3])  # type: ignore
+
+    with pytest.raises(StreamlitAPIException):
+        stqs.selectbox_qs("Test", options=[1, 2, None], key="badtest")
+
+
+def test_radio_qs(mock_query_args_index: mock.MagicMock, session_state):
+    mock_query_args_index.return_value = 1
+    stqs.radio_qs("Test", ["a", "b", "c"], key="test")
+    assert session_state["test"] == "b"
+    mock_query_args_index.assert_called_with("test", ["a", "b", "c"], default=0, unformat_func=str)
+    stqs.radio_qs("Test", [1, 2, 3], key="test2", unformat_func=int) == 2
+    mock_query_args_index.assert_called_with("test2", [1, 2, 3], default=0, unformat_func=int)
+
+    assert _test_helper_autoupdate(stqs.radio_qs, "Test", ["a", "b", "c"], key="test3", autoupdate=True)
+    assert session_state["test3"] == "b"
+
+    with pytest.raises(TypeError):
+        # can't call without key
+        stqs.radio_qs("Test", [1, 2, 3])  # type: ignore
+
+    with pytest.raises(StreamlitAPIException):
+        stqs.radio_qs("Test", options=[1, 2, None], key="badtest")
+
+
+@mock.patch("streamlit.multiselect", wraps=st.multiselect)
+def test_multiselect_qs_strings(mock_ms: mock.MagicMock, mock_from_query_args: mock.MagicMock, session_state):
+    options = ["3", "1", "5"]
+
+    mock_from_query_args.return_value = ["1"]
+    stqs.multiselect_qs("Test", options, key="test")
+    assert session_state["test"] == ["1"]
+    mock_ms.assert_called_with("Test", options, default=None, key="test")
+
+    mock_from_query_args.return_value = ["1", "5", "7"]
+    stqs.multiselect_qs("Test", options, key="test2")
+    assert session_state["test2"] == ["1", "5"]
+    mock_ms.assert_called_with("Test", options, default=None, key="test2")
+
+    mock_from_query_args.return_value = ["1", "3"]
+    stqs.multiselect_qs("Test", options, default=["1", "3"], key="test3")
+    "test3" not in session_state
+    mock_ms.assert_called_with("Test", options, default=["1", "3"], key="test3")
+
+    mock_from_query_args.return_value = ["3"]
+    stqs.multiselect_qs("Test", options, default="3", key="test4")
+    mock_ms.assert_called_with("Test", options, default="3", key="test4")
+
+    mock_from_query_args.return_value = []
+    stqs.multiselect_qs("Test", options, key="test5")
+    mock_ms.assert_called_with("Test", options, default=None, key="test5")
+
+    mock_from_query_args.return_value = []
+    _test_helper_autoupdate(stqs.multiselect_qs, "Test", options, key="test6", autoupdate=True)
+
+    mock_from_query_args.return_value = ["1", "5", "7"]
+    with pytest.raises(ValueError):
+        stqs.multiselect_qs("Test", options, key="test7", discard_missing=False) != ["1", "5"]
+
+    with pytest.raises(TypeError):
+        # can't call without key
+        stqs.multiselect_qs("Test", ["1", "2", "3"])  # type: ignore
+
+
+@mock.patch("streamlit.multiselect", wraps=st.multiselect)
+def test_multiselect_qs_nonstring(mock_ms: mock.MagicMock, mock_from_query_args: mock.MagicMock, session_state):
+    options = [1, 3, 5]
+
+    mock_from_query_args.return_value = [1]
+    stqs.multiselect_qs("Test", options, key="test", unformat_func=int)
+    assert session_state["test"] == [1]
+    mock_ms.assert_called_with("Test", options, default=None, key="test")
+
+    mock_from_query_args.return_value = [1, 2, 3]
+    stqs.multiselect_qs("Test", options, key="test2", unformat_func=lambda x: len(x))
+    assert session_state["test2"] == [1, 3]
+    mock_ms.assert_called_with("Test", options, default=None, key="test2")
+
+    mock_from_query_args.return_value = [1, 5]
+    stqs.multiselect_qs("Test", options, default=[1, 5], key="test3")
+    "test3" not in session_state
+    mock_ms.assert_called_with("Test", options, default=[1, 5], key="test3")
+
+    mock_from_query_args.return_value = []
+    stqs.multiselect_qs("Test", options, key="test4")
+    mock_ms.assert_called_with("Test", options, default=None, key="test4")
+
+    with pytest.raises(StreamlitAPIException):
+        stqs.multiselect_qs("Test", options=[1, 2, None], key="badtest")
+
+
+def test_checkbox_qs(mock_from_query_args: mock.MagicMock, session_state):
+    for val in ("1", "True", "tRue", "TRUE"):
+        mock_from_query_args.return_value = stqs._convert_bool_checkbox(val, False)
+        stqs.checkbox_qs("Test", key="test")
+        assert session_state["test"] is True
+    for val in ("0", "FALSE", "False", "false"):
+        mock_from_query_args.return_value = stqs._convert_bool_checkbox(val, False)
+        stqs.checkbox_qs("Test", key="test2")
+        assert session_state["test2"] is False
+
+    mock_from_query_args.return_value = stqs._convert_bool_checkbox("TROO", True)
+    stqs.checkbox_qs("Test", key="test3", default=True)
+    assert session_state["test3"] is True
+    mock_from_query_args.return_value = stqs._convert_bool_checkbox("TROO", False)
+    stqs.checkbox_qs("Test", key="test4", default=False)
+    assert session_state["test4"] is False
+    
+    mock_from_query_args.return_value = False
+    _test_helper_autoupdate(stqs.checkbox_qs, "Test", key="test5", autoupdate=True)
+    assert session_state["test5"] is False
+
+    with pytest.raises(TypeError):
+        # can't call without key
+        stqs.selectbox_qs("Test", [1, 2])  # type: ignore
+
+
+def test_text_input_qs(mock_from_query_args: mock.MagicMock, session_state):
+    mock_from_query_args.return_value = "hello"
+    stqs.text_input_qs("Test", default="world", key="test")
+    assert session_state["test"] == "hello"
+    mock_from_query_args.assert_called_with("test", default="world")
+
+    _test_helper_autoupdate(stqs.text_input_qs, "Test", key="test2", autoupdate=True)
+    assert session_state["test2"] == "hello"
+
+    mock_from_query_args.side_effect = ValueError("multiple values")
+    with pytest.raises(ValueError):
+        stqs.text_input_qs("Test", key="a")
+    with pytest.raises(TypeError):
+        # can't call without key
+        stqs.text_input_qs("Test", [1, 2])  # type: ignore
+
+
+def test_text_area_qs(mock_from_query_args, session_state):
+    mock_from_query_args.return_value = "hello"
+    stqs.text_area_qs("Test", default="world", key="test")
+    assert session_state["test"] == "hello"
+    mock_from_query_args.assert_called_with("test", default="world")
+
+    _test_helper_autoupdate(stqs.text_area_qs, "Test", key="test2", autoupdate=True)
+    assert session_state["test2"] == "hello"
+
+    mock_from_query_args.side_effect = ValueError("multiple values")
+    with pytest.raises(ValueError):
+        stqs.text_area_qs("Test", key="a")
+    with pytest.raises(TypeError):
+        # can't call without key
+        stqs.text_area_qs("Test")  # type: ignore
+
+
+def test_number_input_qs(mock_from_query_args, session_state):
+    mock_from_query_args.return_value = "hello"
+    val = stqs.number_input_qs("Test", default=4, key="test0")
+    # When query string invalid and default=="min" we dont expect session_state to get set
+    assert "test0" not in session_state
+    assert val == 4 and isinstance(val, int)
+
+    mock_from_query_args.return_value = "hello"
+    val = stqs.number_input_qs("Test", key="test1")
+    # When query string invalid and default=="min" we dont expect session_state to get set
+    assert "test1" not in session_state
+    assert val == 0.0 and isinstance(val, float)
+
+    mock_from_query_args.return_value = "6"
+    stqs.number_input_qs("Test", default=5.0, key="test2")
+    val = session_state["test2"]
+    assert val == 6.0 and isinstance(val, float)
+    stqs.number_input_qs("Test", default=4, key="test3")
+    val = session_state["test3"]
+    assert val == 6 and isinstance(val, int)
+    stqs.number_input_qs("Test", min_value=5, key="test4")
+    val = session_state["test4"]
+    assert val == 6 and isinstance(val, int)
+    stqs.number_input_qs("Test", max_value=7, key="test5")
+    val = session_state["test5"]
+    assert val == 6 and isinstance(val, int)
+    stqs.number_input_qs("Test", max_value=4, key="test5.1")  # it even lets you go outside normal bounds?
+    val = session_state["test5.1"]
+    assert val == 6 and isinstance(val, int)
+    stqs.number_input_qs("Test", step=4.5, key="test6")
+    val = session_state["test6"]
+    assert val == 6.0 and isinstance(val, float)
+    stqs.number_input_qs("Test", key="test7")
+    val = session_state["test7"]
+    assert val == 6.0 and isinstance(val, float)
+
+    stqs.number_input_qs("Test", default=None, key="test8")
+    val = session_state["test8"]
+    assert val == 6.0 and isinstance(val, float)
+
+    mock_from_query_args.return_value = "NOT_A_NUMBER"
+    assert _test_helper_autoupdate(stqs.number_input_qs, "Test", key="test9", autoupdate=True) == 0
+    assert "test9" not in session_state
+    assert stqs.number_input_qs("Test", default=None, key="test10") is None
+    assert "test10" not in session_state
+
+    mock_from_query_args.return_value = None
+    assert stqs.number_input_qs("Test", key="test11") == 0
+    assert "test11" not in session_state
+    assert stqs.number_input_qs("Test", default=5.0, key="test12") == 5.0
+    assert "test12" not in session_state
+    assert stqs.number_input_qs("Test", max_value=5, key="test13") == 0
+    assert "test13" not in session_state
+
+    mock_from_query_args.side_effect = ValueError("multiple values")
+    with pytest.raises(ValueError):
+        stqs.number_input_qs("Test", key="a")
+
+    mock_from_query_args.side_effect = None
+    mock_from_query_args.return_value = "6"
+    with pytest.raises(TypeError, match="Expected type was not a float"):
+        stqs.number_input_qs("Test", min_value="string", key="test")  # bad type with no default
+    with pytest.raises(TypeError, match="Expected type was not a float"):
+        stqs.number_input_qs("Test", max_value="string", key="test")  # bad type with no default
+    with pytest.raises(TypeError, match="Expected type was not a float"):
+        stqs.number_input_qs("Test", step="string", key="test")  # bad type with no default
+    with pytest.raises(TypeError, match="keyword-only"):
+        # can't call without key
+        stqs.number_input_qs("Test")  # type: ignore
+
+
+def test_qs_intersect():
+    new_session_state1 = {"a3": 1, "b3": 2, "b2": 3}
+    with mock.patch("streamlit.session_state", new=new_session_state1):
+        stqs._qs_intersect(None, tuple()) == new_session_state1
+        stqs._qs_intersect(tuple(), tuple()) == {}  # i.e. if the user passes in keys=[]
+        stqs._qs_intersect(["a3", "b3"], tuple()) == {"a3": 1, "b3": 2}
+        stqs._qs_intersect(["a3", "badval"], tuple()) == {"a3": 1}
+        stqs._qs_intersect(None, ["b.$"]) == {"b2": 3, "b3": 2}
+        stqs._qs_intersect(["a3"], ["b.$"]) == {"a3": 1, "b2": 3, "b3": 2}
+
+    new_session_state2 = {"a3": 1, "blacklisted_key": "blacklisted"}
+    with mock.patch("streamlit.session_state", new=new_session_state2):
+        stqs.blacklist_key("blacklisted_key")
+        stqs._qs_intersect(None, tuple()) == {"a3": 1}
+        stqs.unblacklist_key("blacklisted_key")
+        assert "blacklisted_key" not in stqs.QS_BLACKLIST_KEYS
+
+    with pytest.raises(ValueError, match="Arguments to query string functions must be non-str collections"):
+        stqs._qs_intersect("foo", tuple())
+    with pytest.raises(ValueError, match="Arguments to query string functions must be non-str collections"):
+        stqs._qs_intersect(None, "foo")
+
+
+def test_make_query_string(session_state):
+    session_state.update({"a3": 1, "b3": "hello world", "b2": 3})
+    assert all(kv in stqs.make_query_string() for kv in ["?", "a3=1", "b3=hello+world", "b2=3"])
+    assert all(kv in stqs.make_query_string(regex=["b.$"]) for kv in ["?", "b3=hello+world", "b2=3"])
+    stqs.make_query_string(["b3"]) == "?b3=hello+world"
+
+
+def test_set_qs_callback(qp: QueryParams, session_state):
+    session_state.update({"a3": 1, "b3": "hello world", "b2": 3})
+
+    func = stqs.set_qs_callback(["a3", "b3"], regex=[])
+    assert qp._query_params == {}
+    func()
+    assert qp._query_params == dict(a3="1", b3="hello world")
+
+    assert stqs.set_qs_callback()() is None
+    assert qp._query_params == dict(a3="1", b3="hello world", b2="3")
+
+
+def test_add_qs_callback(qp: QueryParams, session_state):
+    session_state.update({"a3": 1, "b3": "hello world", "b2": 3, "nonekey": None})
+
+    qp._query_params = {"a1": "hi", "nonekey": "5"}
+    func = stqs.add_qs_callback(["b2"], regex=[])
+    assert qp._query_params == {"a1": "hi", "nonekey": "5"}
+    func()
+    assert qp._query_params == {"a1": "hi", "nonekey": "5", "b2": "3"}
+
+    assert stqs.add_qs_callback(["nonekey"])() is None
+    assert qp._query_params == {"a1": "hi", "nonekey": "5", "b2": "3"}
+
+
+def test_update_qs_callback(qp: QueryParams, session_state):
+    session_state.update({"a3": 1, "b3": "hello world", "b2": 3, "nonekey": None})
+
+    qp._query_params = {"a1": "hi", "nonekey": "5"}
+    func = stqs.update_qs_callback(["b2"], regex=[])
+    assert qp._query_params == {"a1": "hi", "nonekey": "5"}
+    func()
+    assert qp._query_params == {"a1": ["hi"], "b2": "3", "nonekey": ["5"]}
+
+    assert stqs.update_qs_callback(["nonekey"])() is None
+    assert qp._query_params == {"a1": ["hi"], "b2": ["3"]}
+
+    assert stqs.update_qs_callback()() is None
+    assert qp._query_params == {"a1": ["hi"], "b3": "hello world", "b2": "3", "a3": "1"}
+
+
+def test_clear_qs_callback_legacy(qp: QueryParams, streamlit_1_33, session_state):
+    session_state.update({"a3": 1, "b3": "hello world", "b2": 3, "nonekey": None})
+
+    qp._query_params = {"oldkey": "value"}
+    func = stqs.clear_qs_callback()
+    assert qp._query_params == {"oldkey": "value"}
+    func()
+    assert qp._query_params == {}
+
+    qp._query_params = {"a1": "hi", "b3": "world"}
+    assert stqs.clear_qs_callback(["b3"])() is None
+    assert qp._query_params == {"a1": "hi"}
+
+
+def test_clear_qs_callback_optimized(qp: QueryParams, session_state):
+    session_state.update({"a3": 1, "b3": "hello world", "b2": 3, "nonekey": None})
+
+    qp._query_params = {"oldkey": "value"}
+    func = stqs.clear_qs_callback()
+    assert qp._query_params == {"oldkey": "value"}
+    func()
+    assert qp._query_params == {}
+
+    qp._query_params = {"a1": "hi", "b3": "world"}
+    assert stqs.clear_qs_callback(["b3"])() is None
+    assert qp._query_params == {"a1": ["hi"]}
+
+
+def test_wrap_on_chage_with_qs_update(qp: QueryParams, session_state):
+    kwargs: Any = {"foo": "a", "bar": "b", "none": None}
+    stqs._wrap_on_change_with_qs_update("key", kwargs, remove_none_values=False)
+    assert callable(kwargs["on_change"])
+    assert kwargs["on_change"].__name__ == "_add_qs_callback"
+    qp._query_params = {"key": "hi"}
+    kwargs["on_change"]()
+    assert qp._query_params == {"key": "hi"}
+
+    callback = mock.MagicMock(__name__="mockfunction")
+    kwargs = {"foo": "a", "bar": "b", "on_change": callback}
+    stqs._wrap_on_change_with_qs_update("key", kwargs, remove_none_values=True)
+    assert callable(kwargs["on_change"])
+    assert kwargs["on_change"].__name__ == "mockfunction"
+    assert kwargs["on_change"] is not callback
+    callback.assert_not_called()
+    qp._query_params = {"key": "a", "foobar": "b"}
+    session_state["key"] = None
+    kwargs["on_change"]()
+    callback.assert_called()
+    assert qp._query_params == {"foobar": ["b"]}
+
+    kwargs = {"foo": "a", "bar": "b", "on_change": 1}
+    with pytest.raises(TypeError, match="keyword argument is not callable"):
+        stqs._wrap_on_change_with_qs_update("key", kwargs, remove_none_values=True)
+
+
+def _test_helper_autoupdate(func, *args, **kwargs):
+    """Helper function to test an "autoupdate" call"""
+
+    # patch the wrap on change function
+    with mock.patch("streamlit_qs._wrap_on_change_with_qs_update") as mock_wrap:
+        # Add autoupdate=True as a kwarg if it hasn't been by the caller
+        kwargs.update(autoupdate=True)
+        # Call the function under test
+        retval = func(*args, **kwargs)
+        # assert that wrap_on_change was called
+        mock_wrap.assert_called()
+    # Return whatever was returned by the function under test
+    return retval
+
+
+def test_unenumifier():
+    class AnEnum(Enum):
+        FOO = 0
+        BAR = 1
+
+    class NotAnEnum:
+        ...
+
+    unenumifier = stqs.unenumifier(AnEnum)
+    assert callable(unenumifier)
+    assert unenumifier("FOO") == AnEnum.FOO
+    assert unenumifier("AnEnum.BAR") == AnEnum.BAR
+    with pytest.raises(ValueError):
+        unenumifier("invalid")
+    with pytest.raises(AttributeError):
+        stqs.unenumifier("foo")  # type: ignore
+    with pytest.raises(TypeError):
+        stqs.unenumifier(NotAnEnum)("FOO")  # type: ignore
+
+
+def test_ensure_list():
+    assert stqs._ensure_list("abc") == ["abc"]
+    assert stqs._ensure_list(b"abc") == [b"abc"]
+    assert stqs._ensure_list((5, 6, 7)) == [5, 6, 7]
+    assert stqs._ensure_list([1, 2, 3]) == [1, 2, 3]
+    assert stqs._ensure_list(5) == [5]
+
+
+def test_infer_unformat_func():
+    class AnEnum(Enum):
+        FOO = 0
+        BAR = 1
+
+    assert stqs._infer_common_unformat_funcs([1, 2, 3], str) is int
+    assert stqs._infer_common_unformat_funcs([1.0, 2.0, 3.0], str) is float
+    assert stqs._infer_common_unformat_funcs([AnEnum.FOO, AnEnum.BAR], str).__name__ == "_unenum_AnEnum"
+
+    assert stqs._infer_common_unformat_funcs([1, 2, 3.0], str) is str
+    assert stqs._infer_common_unformat_funcs([1.0, 2.0, AnEnum.FOO], str) is str
+    assert stqs._infer_common_unformat_funcs([AnEnum.FOO, AnEnum.BAR, "AnEnum.BAZ"], str) is str
+
+    assert stqs._infer_common_unformat_funcs([1, 2, 3], float) is float
+    assert stqs._infer_common_unformat_funcs([1.0, 2.0, 3.0], int) is int
+    def enum_unformat(e): return e.name
+    assert stqs._infer_common_unformat_funcs([AnEnum.FOO, AnEnum.BAR], enum_unformat) is enum_unformat
+
+
+@mock.patch("streamlit.exception")
+def test_warn_on_common_unmatching_unformat_funcs(mock_warning):
+    stqs._warn_on_common_unmatching_unformat_functions([1, 2, 3], str)
+    assert isinstance(mock_warning.call_args[0][0], StreamlitAPIWarning)
+    assert repr({int}) in str(mock_warning.call_args[0][0])
+
+    stqs._warn_on_common_unmatching_unformat_functions([1, 2.0, "str"], str)
+    assert isinstance(mock_warning.call_args[0][0], StreamlitAPIWarning)
+    assert repr({int, float, str}) in str(mock_warning.call_args[0][0])
+
+    stqs._warn_on_common_unmatching_unformat_functions([StreamlitAPIException(), StreamlitAPIWarning()], str)
+    assert isinstance(mock_warning.call_args[0][0], StreamlitAPIWarning)
+    assert repr({StreamlitAPIException, StreamlitAPIWarning}) in str(mock_warning.call_args[0][0])
+
+    mock_warning.reset_mock()  # remaining tests should NOT call this
+    stqs._warn_on_common_unmatching_unformat_functions([StreamlitAPIException(), StreamlitAPIWarning()], int)
+    stqs._warn_on_common_unmatching_unformat_functions([1, 2.0, "str"], float)
+    stqs._warn_on_common_unmatching_unformat_functions([1, 2, 3], float)
+    stqs._warn_on_common_unmatching_unformat_functions([1, 2, 3], int)
+    mock_warning.assert_not_called()
```

