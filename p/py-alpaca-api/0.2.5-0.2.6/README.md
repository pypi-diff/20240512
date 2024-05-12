# Comparing `tmp/py_alpaca_api-0.2.5.tar.gz` & `tmp/py_alpaca_api-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_alpaca_api-0.2.5.tar", max compression
+gzip compressed data, was "py_alpaca_api-0.2.6.tar", max compression
```

## Comparing `py_alpaca_api-0.2.5.tar` & `py_alpaca_api-0.2.6.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1066 2024-05-11 23:37:32.674625 py_alpaca_api-0.2.5/LICENSE
--rw-r--r--   0        0        0    12576 2024-05-12 02:52:40.341369 py_alpaca_api-0.2.5/README.md
--rw-r--r--   0        0        0        0 2024-05-11 00:31:44.448417 py_alpaca_api-0.2.5/py_alpaca_api/__init__.py
--rw-r--r--   0        0        0    43735 2024-05-12 16:00:21.371412 py_alpaca_api-0.2.5/py_alpaca_api/alpaca.py
--rw-r--r--   0        0        0    17342 2024-05-12 16:00:21.371412 py_alpaca_api-0.2.5/py_alpaca_api/src/data_classes.py
--rw-r--r--   0        0        0     1225 2024-05-12 16:00:21.371412 py_alpaca_api-0.2.5/pyproject.toml
--rw-r--r--   0        0        0    13337 1970-01-01 00:00:00.000000 py_alpaca_api-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-05-11 23:37:32.674625 py_alpaca_api-0.2.6/LICENSE
+-rw-r--r--   0        0        0    12576 2024-05-12 02:52:40.341369 py_alpaca_api-0.2.6/README.md
+-rw-r--r--   0        0        0        0 2024-05-11 00:31:44.448417 py_alpaca_api-0.2.6/py_alpaca_api/__init__.py
+-rw-r--r--   0        0        0    44564 2024-05-12 20:57:16.476460 py_alpaca_api-0.2.6/py_alpaca_api/alpaca.py
+-rw-r--r--   0        0        0    18290 2024-05-12 20:57:16.456460 py_alpaca_api-0.2.6/py_alpaca_api/src/data_classes.py
+-rw-r--r--   0        0        0     1225 2024-05-12 20:57:54.646449 py_alpaca_api-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0    13337 1970-01-01 00:00:00.000000 py_alpaca_api-0.2.6/PKG-INFO
```

### Comparing `py_alpaca_api-0.2.5/LICENSE` & `py_alpaca_api-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `py_alpaca_api-0.2.5/README.md` & `py_alpaca_api-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `py_alpaca_api-0.2.5/py_alpaca_api/alpaca.py` & `py_alpaca_api-0.2.6/py_alpaca_api/alpaca.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import pandas as pd
 import requests
 
 from .src.data_classes import (
     account_class_from_dict,
     asset_class_from_dict,
+    clock_class_from_dict,
     order_class_from_dict,
     position_class_from_dict,
 )
 
 
 # PyAlpacaApi class
 class PyAlpacaApi:
@@ -54,14 +55,31 @@
         if api_paper:
             self.trade_url = "https://paper-api.alpaca.markets/v2"
         else:
             self.trade_url = "https://api.alpaca.markets/v2"
 
         self.data_url = "https://data.alpaca.markets/v2"
 
+    ########################################################
+    # \\\\\\\\\\\\\\\\\ Market Clock //////////////////////#
+    ########################################################
+    def market_clock(self):
+        # Alpaca API URL for market clock
+        url = f"{self.trade_url}/clock"
+        # Get request to Alpaca API for market clock
+        response = requests.get(url, headers=self.headers)
+        # Check if response is successful
+        if response.status_code == 200:
+            # Return market clock status
+            return clock_class_from_dict(json.loads(response.text))
+        # If response is not successful, raise an exception
+        else:
+            res = json.loads(response.text)
+            raise Exception(f'Failed to get market clock. Response: {res["message"]}')
+
     ############################
     # Get Stock Historical Data
     ############################
     def get_stock_historical_data(
         self,
         symbol,
         start,
```

### Comparing `py_alpaca_api-0.2.5/py_alpaca_api/src/data_classes.py` & `py_alpaca_api-0.2.6/py_alpaca_api/src/data_classes.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,35 @@
 from dataclasses import dataclass
 from datetime import datetime
 
 
 @dataclass
 ############################################
+# Data Class for Clock
+############################################
+class ClockClass:
+    """Clock class data structure.
+
+    Attributes:
+    ----------
+
+    timestamp: datetime
+    is_open: bool
+    next_open: datetime
+    next_close: datetime
+    """  # noqa
+
+    market_time: datetime
+    is_open: bool
+    next_open: datetime
+    next_close: datetime
+
+
+@dataclass
+############################################
 # Data Class for Position
 ############################################
 class PositionClass:
     """Position class data structure.
 
     Attributes:
     ------------
@@ -225,16 +247,14 @@
     balance_asof: str
     crypto_tier: int
     intraday_adjustments: int
     pending_reg_taf_fees: float
     """  # noqa
 
     id: str
-    admin_configurations: object
-    user_configurations: object
     account_number: str
     status: str
     crypto_status: str
     options_approved_level: int
     options_trading_level: int
     currency: str
     buying_power: float
@@ -269,14 +289,38 @@
     balance_asof: str
     crypto_tier: int
     intraday_adjustments: int
     pending_reg_taf_fees: float
 
 
 ############################################
+# Data Class Clock Conversion Functions
+############################################
+def clock_class_from_dict(data_dict):
+    """Converts a dictionary to a ClockClass object.
+
+    Parameters:
+    -----------
+    data_dict: dict
+        A dictionary containing the clock data.
+
+    Returns:
+    --------
+    ClockClass
+        A ClockClass object.
+    """  # noqa
+    return ClockClass(
+        market_time=(data_dict["timestamp"].split(".")[0].replace("T", " ") if data_dict["timestamp"] else ""),
+        is_open=bool(data_dict["is_open"]),
+        next_open=(data_dict["next_open"].replace("T", " ").replace("-04:00", "") if data_dict["next_open"] else ""),
+        next_close=(data_dict["next_close"].replace("-04:00", "").replace("T", " ") if data_dict["next_close"] else ""),
+    )
+
+
+############################################
 # Data Class Position Conversion Functions
 ############################################
 def position_class_from_dict(data_dict):
     """Converts a dictionary to a PositionClass object.
 
     Parameters:
     -----------
@@ -325,16 +369,14 @@
     Returns:
     --------
     AccountClass
         An AccountClass object.
     """  # noqa
     return AccountClass(
         id=str(data_dict["id"]) if data_dict["id"] else "",
-        admin_configurations=(object(data_dict["admin_configurations"]) if data_dict["admin_configurations"] else {}),
-        user_configurations=(object(data_dict["user_configurations"]) if data_dict["user_configurations"] else {}),
         account_number=str(data_dict["account_number"]),
         status=str(data_dict["status"]) if data_dict["status"] else "",
         crypto_status=(str(data_dict["crypto_status"]) if data_dict["crypto_status"] else ""),
         options_approved_level=(int(data_dict["options_approved_level"]) if data_dict["options_approved_level"] else None),
         options_trading_level=(int(data_dict["options_trading_level"]) if data_dict["options_trading_level"] else None),
         currency=str(data_dict["currency"]) if data_dict["currency"] else "",
         buying_power=(float(data_dict["buying_power"]) if data_dict["buying_power"] else None),
```

### Comparing `py_alpaca_api-0.2.5/pyproject.toml` & `py_alpaca_api-0.2.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "py-alpaca-api"
-version = "0.2.5"
+version = "0.2.6"
 description = "Python package, for communicating with Alpaca Markets REST API."
 authors = ["TexasCoding <jeff10278@me.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/TexasCoding/py-alpaca-api"
 repository = "https://github.com/TexasCoding/py-alpaca-api"
 documentation = "https://py-alpaca-api.readthedocs.io/en/latest/"
```

### Comparing `py_alpaca_api-0.2.5/PKG-INFO` & `py_alpaca_api-0.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-alpaca-api
-Version: 0.2.5
+Version: 0.2.6
 Summary: Python package, for communicating with Alpaca Markets REST API.
 Home-page: https://github.com/TexasCoding/py-alpaca-api
 License: MIT
 Keywords: alpaca,python
 Author: TexasCoding
 Author-email: jeff10278@me.com
 Requires-Python: >=3.12,<4.0
```

