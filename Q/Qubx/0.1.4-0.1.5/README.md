# Comparing `tmp/qubx-0.1.4.tar.gz` & `tmp/qubx-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qubx-0.1.4.tar", max compression
+gzip compressed data, was "qubx-0.1.5.tar", max compression
```

## Comparing `qubx-0.1.4.tar` & `qubx-0.1.5.tar`

### file list

```diff
@@ -1,35 +1,37 @@
--rw-r--r--   0        0        0      940 2024-04-25 07:51:17.473695 qubx-0.1.4/README.md
--rw-r--r--   0        0        0     9305 2024-04-21 10:35:06.164526 qubx-0.1.4/build.py
--rw-r--r--   0        0        0     1378 2024-05-08 18:11:34.565668 qubx-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     5428 2024-04-21 10:35:06.176526 qubx-0.1.4/src/qubx/__init__.py
--rw-r--r--   0        0        0     1730 2024-04-25 07:51:17.477695 qubx-0.1.4/src/qubx/_nb_magic.py
--rw-r--r--   0        0        0        0 2024-02-29 14:43:31.739720 qubx-0.1.4/src/qubx/core/__init__.py
--rw-r--r--   0        0        0     6707 2024-04-25 07:51:17.477695 qubx-0.1.4/src/qubx/core/account.py
--rw-r--r--   0        0        0    14777 2024-05-07 13:17:10.565607 qubx-0.1.4/src/qubx/core/basics.py
--rw-r--r--   0        0        0    11559 2024-05-07 13:17:10.565607 qubx-0.1.4/src/qubx/core/helpers.py
--rw-r--r--   0        0        0    11910 2024-05-07 13:17:10.565607 qubx-0.1.4/src/qubx/core/loggers.py
--rw-r--r--   0        0        0    13688 2024-04-21 10:35:06.176526 qubx-0.1.4/src/qubx/core/lookups.py
--rw-r--r--   0        0        0     2847 2024-04-21 10:35:06.176526 qubx-0.1.4/src/qubx/core/series.pxd
--rw-r--r--   0        0        0    28108 2024-04-21 10:35:06.176526 qubx-0.1.4/src/qubx/core/series.pyx
--rw-r--r--   0        0        0    30330 2024-05-07 13:17:10.565607 qubx-0.1.4/src/qubx/core/strategy.py
--rw-r--r--   0        0        0     1368 2024-02-29 14:43:31.739720 qubx-0.1.4/src/qubx/core/utils.pyx
--rw-r--r--   0        0        0    19648 2024-05-08 18:11:34.565668 qubx-0.1.4/src/qubx/data/readers.py
--rw-r--r--   0        0        0     9150 2024-05-07 13:17:10.565607 qubx-0.1.4/src/qubx/impl/ccxt_connector.py
--rw-r--r--   0        0        0     3488 2024-05-07 13:17:10.565607 qubx-0.1.4/src/qubx/impl/ccxt_customizations.py
--rw-r--r--   0        0        0     9097 2024-05-07 13:17:10.565607 qubx-0.1.4/src/qubx/impl/ccxt_trading.py
--rw-r--r--   0        0        0     3565 2024-05-07 13:17:10.565607 qubx-0.1.4/src/qubx/impl/ccxt_utils.py
--rw-r--r--   0        0        0       33 2024-02-29 14:43:31.739720 qubx-0.1.4/src/qubx/math/__init__.py
--rw-r--r--   0        0        0     1176 2024-02-29 14:43:31.739720 qubx-0.1.4/src/qubx/math/stats.py
--rw-r--r--   0        0        0        0 2024-02-29 14:43:31.739720 qubx-0.1.4/src/qubx/ta/__init__.py
--rw-r--r--   0        0        0     7708 2024-02-29 14:43:31.739720 qubx-0.1.4/src/qubx/ta/indicators.pyx
--rw-r--r--   0        0        0       60 2024-04-21 10:35:06.176526 qubx-0.1.4/src/qubx/trackers/__init__.py
--rw-r--r--   0        0        0     5522 2024-04-21 10:35:06.176526 qubx-0.1.4/src/qubx/trackers/rebalancers.py
--rw-r--r--   0        0        0      273 2024-05-07 13:17:10.569607 qubx-0.1.4/src/qubx/utils/__init__.py
--rw-r--r--   0        0        0    12076 2024-04-21 10:35:06.176526 qubx-0.1.4/src/qubx/utils/_pyxreloader.py
--rw-r--r--   0        0        0    35158 2024-05-07 13:17:10.569607 qubx-0.1.4/src/qubx/utils/charting/mpl_helpers.py
--rw-r--r--   0        0        0    10999 2024-04-21 10:35:06.176526 qubx-0.1.4/src/qubx/utils/marketdata/binance.py
--rw-r--r--   0        0        0     9837 2024-05-07 13:17:10.569607 qubx-0.1.4/src/qubx/utils/misc.py
--rw-r--r--   0        0        0    18605 2024-05-07 13:17:10.569607 qubx-0.1.4/src/qubx/utils/pandas.py
--rw-r--r--   0        0        0     9277 2024-05-07 13:17:10.569607 qubx-0.1.4/src/qubx/utils/runner.py
--rw-r--r--   0        0        0     4884 2024-05-07 13:17:10.569607 qubx-0.1.4/src/qubx/utils/time.py
--rw-r--r--   0        0        0     2144 1970-01-01 00:00:00.000000 qubx-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      940 2024-04-25 07:51:17.473695 qubx-0.1.5/README.md
+-rw-r--r--   0        0        0     9305 2024-04-21 10:35:06.164526 qubx-0.1.5/build.py
+-rw-r--r--   0        0        0     1378 2024-05-12 17:27:41.499398 qubx-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     5428 2024-04-21 10:35:06.176526 qubx-0.1.5/src/qubx/__init__.py
+-rw-r--r--   0        0        0     1875 2024-05-12 17:27:41.499398 qubx-0.1.5/src/qubx/_nb_magic.py
+-rw-r--r--   0        0        0        0 2024-02-29 14:43:31.739720 qubx-0.1.5/src/qubx/core/__init__.py
+-rw-r--r--   0        0        0     6707 2024-04-25 07:51:17.477695 qubx-0.1.5/src/qubx/core/account.py
+-rw-r--r--   0        0        0    14777 2024-05-07 13:17:10.565607 qubx-0.1.5/src/qubx/core/basics.py
+-rw-r--r--   0        0        0    11559 2024-05-07 13:17:10.565607 qubx-0.1.5/src/qubx/core/helpers.py
+-rw-r--r--   0        0        0    11910 2024-05-07 13:17:10.565607 qubx-0.1.5/src/qubx/core/loggers.py
+-rw-r--r--   0        0        0    13688 2024-04-21 10:35:06.176526 qubx-0.1.5/src/qubx/core/lookups.py
+-rw-r--r--   0        0        0     2847 2024-04-21 10:35:06.176526 qubx-0.1.5/src/qubx/core/series.pxd
+-rw-r--r--   0        0        0    28108 2024-04-21 10:35:06.176526 qubx-0.1.5/src/qubx/core/series.pyx
+-rw-r--r--   0        0        0    30330 2024-05-07 13:17:10.565607 qubx-0.1.5/src/qubx/core/strategy.py
+-rw-r--r--   0        0        0     1368 2024-02-29 14:43:31.739720 qubx-0.1.5/src/qubx/core/utils.pyx
+-rw-r--r--   0        0        0    19648 2024-05-08 18:11:34.565668 qubx-0.1.5/src/qubx/data/readers.py
+-rw-r--r--   0        0        0     9150 2024-05-07 13:17:10.565607 qubx-0.1.5/src/qubx/impl/ccxt_connector.py
+-rw-r--r--   0        0        0     3488 2024-05-07 13:17:10.565607 qubx-0.1.5/src/qubx/impl/ccxt_customizations.py
+-rw-r--r--   0        0        0     9097 2024-05-07 13:17:10.565607 qubx-0.1.5/src/qubx/impl/ccxt_trading.py
+-rw-r--r--   0        0        0     3565 2024-05-07 13:17:10.565607 qubx-0.1.5/src/qubx/impl/ccxt_utils.py
+-rw-r--r--   0        0        0       33 2024-02-29 14:43:31.739720 qubx-0.1.5/src/qubx/math/__init__.py
+-rw-r--r--   0        0        0     1176 2024-02-29 14:43:31.739720 qubx-0.1.5/src/qubx/math/stats.py
+-rw-r--r--   0        0        0      175 2024-05-12 17:27:41.499398 qubx-0.1.5/src/qubx/pandaz/__init__.py
+-rw-r--r--   0        0        0    85271 2024-05-12 17:27:41.503398 qubx-0.1.5/src/qubx/pandaz/ta.py
+-rw-r--r--   0        0        0    19109 2024-05-12 17:27:41.503398 qubx-0.1.5/src/qubx/pandaz/utils.py
+-rw-r--r--   0        0        0        0 2024-02-29 14:43:31.739720 qubx-0.1.5/src/qubx/ta/__init__.py
+-rw-r--r--   0        0        0     7708 2024-02-29 14:43:31.739720 qubx-0.1.5/src/qubx/ta/indicators.pyx
+-rw-r--r--   0        0        0       60 2024-04-21 10:35:06.176526 qubx-0.1.5/src/qubx/trackers/__init__.py
+-rw-r--r--   0        0        0     5522 2024-04-21 10:35:06.176526 qubx-0.1.5/src/qubx/trackers/rebalancers.py
+-rw-r--r--   0        0        0      273 2024-05-07 13:17:10.569607 qubx-0.1.5/src/qubx/utils/__init__.py
+-rw-r--r--   0        0        0    12076 2024-04-21 10:35:06.176526 qubx-0.1.5/src/qubx/utils/_pyxreloader.py
+-rw-r--r--   0        0        0    35158 2024-05-07 13:17:10.569607 qubx-0.1.5/src/qubx/utils/charting/mpl_helpers.py
+-rw-r--r--   0        0        0    10993 2024-05-12 17:27:41.503398 qubx-0.1.5/src/qubx/utils/marketdata/binance.py
+-rw-r--r--   0        0        0     9831 2024-05-12 17:27:41.503398 qubx-0.1.5/src/qubx/utils/misc.py
+-rw-r--r--   0        0        0     9306 2024-05-12 17:27:41.503398 qubx-0.1.5/src/qubx/utils/runner.py
+-rw-r--r--   0        0        0     4884 2024-05-07 13:17:10.569607 qubx-0.1.5/src/qubx/utils/time.py
+-rw-r--r--   0        0        0     2144 1970-01-01 00:00:00.000000 qubx-0.1.5/PKG-INFO
```

### Comparing `qubx-0.1.4/README.md` & `qubx-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `qubx-0.1.4/build.py` & `qubx-0.1.5/build.py`

 * *Files identical despite different names*

### Comparing `qubx-0.1.4/pyproject.toml` & `qubx-0.1.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "Qubx"
-version = "0.1.4"
+version = "0.1.5"
 description = "Qubx - quantitative trading framework"
 authors = ["Dmitry Marienko <dmitry@gmail.com>"]
 readme = "README.md"
 packages = [
     { include = "qubx", from = "src" },
 ]
 repository = "https://github.com/dmarienko/Qubx"
```

### Comparing `qubx-0.1.4/src/qubx/__init__.py` & `qubx-0.1.5/src/qubx/__init__.py`

 * *Files identical despite different names*

### Comparing `qubx-0.1.4/src/qubx/_nb_magic.py` & `qubx-0.1.5/src/qubx/_nb_magic.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,21 +28,25 @@
     # - - - - Common stuff - - - -
     import numpy as np
     import pandas as pd
     from datetime import time, timedelta
     from tqdm.auto import tqdm
 
     # - - - - TA stuff and indicators - - - -
+    import qubx.pandaz.ta as pta
+
     # - - - - Portfolio analysis - - - -
     # - - - - Simulator stuff - - - -
     # - - - - Learn stuff - - - -
     # - - - - Charting stuff - - - -
     from matplotlib import pyplot as plt
     from qubx.utils.charting.mpl_helpers import fig, subplot, sbp
+
     # - - - - Utils - - - -
+    from qubx.pandaz.utils import scols, srows, ohlc_resample, continuous_periods, generate_equal_date_ranges
 
     # - setup short numpy output format
     np_fmt_short()
     
     # - add project home to system path
     add_project_to_system_path()
```

### Comparing `qubx-0.1.4/src/qubx/core/account.py` & `qubx-0.1.5/src/qubx/core/account.py`

 * *Files identical despite different names*

### Comparing `qubx-0.1.4/src/qubx/core/basics.py` & `qubx-0.1.5/src/qubx/core/basics.py`

 * *Files identical despite different names*

### Comparing `qubx-0.1.4/src/qubx/core/helpers.py` & `qubx-0.1.5/src/qubx/core/helpers.py`

 * *Files identical despite different names*

### Comparing `qubx-0.1.4/src/qubx/core/loggers.py` & `qubx-0.1.5/src/qubx/core/loggers.py`

 * *Files identical despite different names*

### Comparing `qubx-0.1.4/src/qubx/core/lookups.py` & `qubx-0.1.5/src/qubx/core/lookups.py`

 * *Files identical despite different names*

### Comparing `qubx-0.1.4/src/qubx/core/series.pxd` & `qubx-0.1.5/src/qubx/core/series.pxd`

 * *Files identical despite different names*

### Comparing `qubx-0.1.4/src/qubx/core/series.pyx` & `qubx-0.1.5/src/qubx/core/series.pyx`

 * *Files identical despite different names*

### Comparing `qubx-0.1.4/src/qubx/core/strategy.py` & `qubx-0.1.5/src/qubx/core/strategy.py`

 * *Files identical despite different names*

### Comparing `qubx-0.1.4/src/qubx/core/utils.pyx` & `qubx-0.1.5/src/qubx/core/utils.pyx`

 * *Files identical despite different names*

### Comparing `qubx-0.1.4/src/qubx/data/readers.py` & `qubx-0.1.5/src/qubx/data/readers.py`

 * *Files identical despite different names*

### Comparing `qubx-0.1.4/src/qubx/impl/ccxt_connector.py` & `qubx-0.1.5/src/qubx/impl/ccxt_connector.py`

 * *Files identical despite different names*

### Comparing `qubx-0.1.4/src/qubx/impl/ccxt_customizations.py` & `qubx-0.1.5/src/qubx/impl/ccxt_customizations.py`

 * *Files identical despite different names*

### Comparing `qubx-0.1.4/src/qubx/impl/ccxt_trading.py` & `qubx-0.1.5/src/qubx/impl/ccxt_trading.py`

 * *Files identical despite different names*

### Comparing `qubx-0.1.4/src/qubx/impl/ccxt_utils.py` & `qubx-0.1.5/src/qubx/impl/ccxt_utils.py`

 * *Files identical despite different names*

### Comparing `qubx-0.1.4/src/qubx/math/stats.py` & `qubx-0.1.5/src/qubx/math/stats.py`

 * *Files identical despite different names*

### Comparing `qubx-0.1.4/src/qubx/ta/indicators.pyx` & `qubx-0.1.5/src/qubx/ta/indicators.pyx`

 * *Files identical despite different names*

### Comparing `qubx-0.1.4/src/qubx/trackers/rebalancers.py` & `qubx-0.1.5/src/qubx/trackers/rebalancers.py`

 * *Files identical despite different names*

### Comparing `qubx-0.1.4/src/qubx/utils/_pyxreloader.py` & `qubx-0.1.5/src/qubx/utils/_pyxreloader.py`

 * *Files identical despite different names*

### Comparing `qubx-0.1.4/src/qubx/utils/charting/mpl_helpers.py` & `qubx-0.1.5/src/qubx/utils/charting/mpl_helpers.py`

 * *Files identical despite different names*

### Comparing `qubx-0.1.4/src/qubx/utils/marketdata/binance.py` & `qubx-0.1.5/src/qubx/utils/marketdata/binance.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from os.path import exists, join, split, basename
 from tqdm.notebook import tqdm
 import requests
 from collections import defaultdict
 
 from qubx import logger
 from qubx.utils.misc import makedirs, get_local_qubx_folder
-from qubx.utils.pandas import generate_equal_date_ranges, srows
+from qubx.pandaz import generate_equal_date_ranges, srows
 
 
 DEFALT_LOCAL_FILE_STORAGE = makedirs(get_local_qubx_folder(), 'data/import/binance_history/')
 DEFALT_LOCAL_CSV_STORAGE = makedirs(get_local_qubx_folder(), 'data/binance/')
 
 # _DEFAULT_MARKET_DATA_DB = 'md'
 BINANCE_DATA_STORAGE = "https://s3-ap-northeast-1.amazonaws.com"
```

### Comparing `qubx-0.1.4/src/qubx/utils/misc.py` & `qubx-0.1.5/src/qubx/utils/misc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from typing import Dict, Optional, Union, List
-import glob, os
+import os
 from collections import OrderedDict, defaultdict, namedtuple
 from os.path import basename, exists, dirname, join, expanduser
 import time
 from pathlib import Path
 
 
 def version() -> str:
```

### Comparing `qubx-0.1.4/src/qubx/utils/pandas.py` & `qubx-0.1.5/src/qubx/pandaz/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,30 @@
-from typing import Callable, Dict, Iterable, Optional, Union, List
+from typing import Callable, Dict, Iterable, Literal, Optional, Union, List
 from datetime import timedelta
 import pandas as pd
 import numpy as np
 
 from numpy.lib.stride_tricks import as_strided as stride
 
 from qubx.utils.misc import Struct
 
 
+def has_columns(x, *args):
+    return isinstance(x, pd.DataFrame) and sum(x.columns.isin(args)) == len(args)
+
+
+def check_frame_columns(x, *args):
+    if not isinstance(x, pd.DataFrame):
+        raise ValueError(f"Input data must be DataFrame but {type(x)} received !")
+
+    if sum(x.columns.isin(args)) != len(args):
+        required = [y for y in args if y not in x.columns]
+        raise ValueError(f"> Required {required} columns not found in dataframe !")
+
+
 def rolling_forward_test_split(x: pd.Series | pd.DataFrame, training_period: int, test_period: int, units: str | None = None ):
     """
     Split data into training and testing **rolling** periods.
      
     Example:
 
     >>> for train_idx, test_idx in rolling_forward_test_split(np.array(range(15)), 5, 3):
@@ -94,15 +107,15 @@
     for a, b in rolling_forward_test_split(
         pd.Series(0, pd.date_range(start, end)), freq, freq, units=units):
         yield _as_f(a[0]), _as_f(a[-1])
         
     yield _as_f(b[0]), _as_f(b[-1])
 
 
-def drop_duplicated_indexes(df: pd.DataFrame, keep='first'):
+def drop_duplicated_indexes(df: pd.DataFrame, keep: Literal['first', 'last', False]='first'):
     """
     Drops duplicated indexes in dataframe/series
     Keeps either first or last occurence (parameter keep)
     """
     return df[~df.index.duplicated(keep=keep)]
```

### Comparing `qubx-0.1.4/src/qubx/utils/runner.py` & `qubx-0.1.5/src/qubx/utils/runner.py`

 * *Files 4% similar despite different names*

```diff
@@ -180,15 +180,16 @@
 # - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
 import qubx
 %qubxd
 import pandas as pd
 import nest_asyncio; nest_asyncio.apply()
 from qubx.utils.misc import dequotify, quotify
 from qubx.utils.runner import create_strategy_context
-from qubx.utils.pandas import *
+from qubx.pandaz.utils import *
+import qubx.pandaz.ta as pta
 
 # - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
 ctx = create_strategy_context('{filename}', '{accounts}', {paths})
 ctx.start()
 
 # - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
 def orders(symbol=None):
```

### Comparing `qubx-0.1.4/src/qubx/utils/time.py` & `qubx-0.1.5/src/qubx/utils/time.py`

 * *Files identical despite different names*

### Comparing `qubx-0.1.4/PKG-INFO` & `qubx-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Qubx
-Version: 0.1.4
+Version: 0.1.5
 Summary: Qubx - quantitative trading framework
 Home-page: https://github.com/dmarienko/Qubx
 Author: Dmitry Marienko
 Author-email: dmitry@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

