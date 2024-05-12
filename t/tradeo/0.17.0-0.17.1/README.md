# Comparing `tmp/tradeo-0.17.0.tar.gz` & `tmp/tradeo-0.17.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tradeo-0.17.0.tar", max compression
+gzip compressed data, was "tradeo-0.17.1.tar", max compression
```

## Comparing `tradeo-0.17.0.tar` & `tradeo-0.17.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1524 2024-05-08 15:51:10.507547 tradeo-0.17.0/LICENSE
--rw-r--r--   0        0        0     4282 2024-05-08 15:51:10.507547 tradeo-0.17.0/README.md
--rw-r--r--   0        0        0     1095 2024-05-08 15:51:10.511546 tradeo-0.17.0/pyproject.toml
--rw-r--r--   0        0        0     1208 2024-05-08 15:51:10.511546 tradeo-0.17.0/tradeo/__init__.py
--rw-r--r--   0        0        0      353 2024-05-08 15:51:10.511546 tradeo-0.17.0/tradeo/bash/launch-mt5.sh
--rw-r--r--   0        0        0      172 2024-05-08 15:51:10.511546 tradeo-0.17.0/tradeo/bash/stop-mt.sh
--rw-r--r--   0        0        0     2569 2024-05-08 15:51:10.511546 tradeo-0.17.0/tradeo/config.py
--rw-r--r--   0        0        0        0 2024-05-08 15:51:10.511546 tradeo-0.17.0/tradeo/context_managers/__init__.py
--rw-r--r--   0        0        0      677 2024-05-08 15:51:10.511546 tradeo-0.17.0/tradeo/context_managers/blocker.py
--rw-r--r--   0        0        0        1 2024-05-08 15:51:10.511546 tradeo-0.17.0/tradeo/data/consecutive_times_down.txt
--rw-r--r--   0        0        0        1 2024-05-08 15:51:10.511546 tradeo-0.17.0/tradeo/data/last_balance.txt
--rw-r--r--   0        0        0        0 2024-05-08 15:51:10.511546 tradeo-0.17.0/tradeo/event_handlers/__init__.py
--rw-r--r--   0        0        0     1106 2024-05-08 15:51:10.511546 tradeo-0.17.0/tradeo/event_handlers/basic_event_handler.py
--rw-r--r--   0        0        0     1699 2024-05-08 15:51:10.511546 tradeo-0.17.0/tradeo/event_handlers/event_handler.py
--rw-r--r--   0        0        0     5899 2024-05-08 15:51:10.515546 tradeo-0.17.0/tradeo/executable/basic_forex.py
--rw-r--r--   0        0        0     1087 2024-05-08 15:51:10.515546 tradeo-0.17.0/tradeo/executable/executable.py
--rw-r--r--   0        0        0     2129 2024-05-08 15:51:10.515546 tradeo-0.17.0/tradeo/files.py
--rw-r--r--   0        0        0     2389 2024-05-08 15:51:10.515546 tradeo-0.17.0/tradeo/log.py
--rw-r--r--   0        0        0    24080 2024-05-08 15:51:10.515546 tradeo-0.17.0/tradeo/mt_client.py
--rw-r--r--   0        0        0     1984 2024-05-08 15:51:10.515546 tradeo-0.17.0/tradeo/mt_message.py
--rw-r--r--   0        0        0    45319 2024-05-08 15:51:10.515546 tradeo-0.17.0/tradeo/mt_tb_expert.mq5
--rw-r--r--   0        0        0      427 2024-05-08 15:51:10.515546 tradeo-0.17.0/tradeo/ohlc.py
--rw-r--r--   0        0        0     4286 2024-05-08 15:51:10.515546 tradeo-0.17.0/tradeo/order.py
--rw-r--r--   0        0        0      268 2024-05-08 15:51:10.515546 tradeo-0.17.0/tradeo/order_operations.py
--rw-r--r--   0        0        0     2471 2024-05-08 15:51:10.515546 tradeo-0.17.0/tradeo/order_type.py
--rw-r--r--   0        0        0      750 2024-05-08 15:51:10.515546 tradeo-0.17.0/tradeo/paths.py
--rw-r--r--   0        0        0      319 2024-05-08 15:51:10.515546 tradeo-0.17.0/tradeo/singleton.py
--rw-r--r--   0        0        0        0 2024-05-08 15:51:10.515546 tradeo-0.17.0/tradeo/strategies/__init__.py
--rw-r--r--   0        0        0     2417 2024-05-08 15:51:10.515546 tradeo-0.17.0/tradeo/strategies/basic_strategy.py
--rw-r--r--   0        0        0     4551 2024-05-08 15:51:10.515546 tradeo-0.17.0/tradeo/strategies/strategy.py
--rw-r--r--   0        0        0     5847 2024-05-08 15:51:10.515546 tradeo-0.17.0/tradeo/trading_methods.py
--rw-r--r--   0        0        0     2000 2024-05-08 15:51:10.515546 tradeo-0.17.0/tradeo/utils.py
--rw-r--r--   0        0        0     4677 1970-01-01 00:00:00.000000 tradeo-0.17.0/PKG-INFO
+-rw-r--r--   0        0        0     1524 2024-05-12 15:34:23.259460 tradeo-0.17.1/LICENSE
+-rw-r--r--   0        0        0     4463 2024-05-12 15:34:23.259460 tradeo-0.17.1/README.md
+-rw-r--r--   0        0        0     1097 2024-05-12 15:34:23.259460 tradeo-0.17.1/pyproject.toml
+-rw-r--r--   0        0        0     1208 2024-05-12 15:34:23.263460 tradeo-0.17.1/tradeo/__init__.py
+-rw-r--r--   0        0        0      353 2024-05-12 15:34:23.263460 tradeo-0.17.1/tradeo/bash/launch-mt5.sh
+-rw-r--r--   0        0        0      172 2024-05-12 15:34:23.263460 tradeo-0.17.1/tradeo/bash/stop-mt.sh
+-rw-r--r--   0        0        0     2569 2024-05-12 15:34:23.263460 tradeo-0.17.1/tradeo/config.py
+-rw-r--r--   0        0        0        0 2024-05-12 15:34:23.263460 tradeo-0.17.1/tradeo/context_managers/__init__.py
+-rw-r--r--   0        0        0      677 2024-05-12 15:34:23.263460 tradeo-0.17.1/tradeo/context_managers/blocker.py
+-rw-r--r--   0        0        0        1 2024-05-12 15:34:23.263460 tradeo-0.17.1/tradeo/data/consecutive_times_down.txt
+-rw-r--r--   0        0        0        1 2024-05-12 15:34:23.263460 tradeo-0.17.1/tradeo/data/last_balance.txt
+-rw-r--r--   0        0        0        0 2024-05-12 15:34:23.263460 tradeo-0.17.1/tradeo/event_handlers/__init__.py
+-rw-r--r--   0        0        0     1106 2024-05-12 15:34:23.263460 tradeo-0.17.1/tradeo/event_handlers/basic_event_handler.py
+-rw-r--r--   0        0        0     1699 2024-05-12 15:34:23.263460 tradeo-0.17.1/tradeo/event_handlers/event_handler.py
+-rw-r--r--   0        0        0     5926 2024-05-12 15:34:23.263460 tradeo-0.17.1/tradeo/executable/basic_forex.py
+-rw-r--r--   0        0        0     1087 2024-05-12 15:34:23.263460 tradeo-0.17.1/tradeo/executable/executable.py
+-rw-r--r--   0        0        0     2129 2024-05-12 15:34:23.263460 tradeo-0.17.1/tradeo/files.py
+-rw-r--r--   0        0        0     2389 2024-05-12 15:34:23.263460 tradeo-0.17.1/tradeo/log.py
+-rw-r--r--   0        0        0    24388 2024-05-12 15:34:23.263460 tradeo-0.17.1/tradeo/mt_client.py
+-rw-r--r--   0        0        0     1984 2024-05-12 15:34:23.263460 tradeo-0.17.1/tradeo/mt_message.py
+-rw-r--r--   0        0        0    45319 2024-05-12 15:34:23.263460 tradeo-0.17.1/tradeo/mt_tb_expert.mq5
+-rw-r--r--   0        0        0      427 2024-05-12 15:34:23.263460 tradeo-0.17.1/tradeo/ohlc.py
+-rw-r--r--   0        0        0     4286 2024-05-12 15:34:23.263460 tradeo-0.17.1/tradeo/order.py
+-rw-r--r--   0        0        0      268 2024-05-12 15:34:23.263460 tradeo-0.17.1/tradeo/order_operations.py
+-rw-r--r--   0        0        0     2471 2024-05-12 15:34:23.263460 tradeo-0.17.1/tradeo/order_type.py
+-rw-r--r--   0        0        0      750 2024-05-12 15:34:23.263460 tradeo-0.17.1/tradeo/paths.py
+-rw-r--r--   0        0        0      319 2024-05-12 15:34:23.263460 tradeo-0.17.1/tradeo/singleton.py
+-rw-r--r--   0        0        0        0 2024-05-12 15:34:23.263460 tradeo-0.17.1/tradeo/strategies/__init__.py
+-rw-r--r--   0        0        0     2417 2024-05-12 15:34:23.263460 tradeo-0.17.1/tradeo/strategies/basic_strategy.py
+-rw-r--r--   0        0        0     4551 2024-05-12 15:34:23.263460 tradeo-0.17.1/tradeo/strategies/strategy.py
+-rw-r--r--   0        0        0     5847 2024-05-12 15:34:23.263460 tradeo-0.17.1/tradeo/trading_methods.py
+-rw-r--r--   0        0        0     2000 2024-05-12 15:34:23.263460 tradeo-0.17.1/tradeo/utils.py
+-rw-r--r--   0        0        0     4872 1970-01-01 00:00:00.000000 tradeo-0.17.1/PKG-INFO
```

### Comparing `tradeo-0.17.0/LICENSE` & `tradeo-0.17.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tradeo-0.17.0/README.md` & `tradeo-0.17.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # TRADEO - A forex trading framework using MetaTrader
-
-![alt text](docs/images/logo.PNG "Title")
+![Logo](docs/images/logo.PNG "Title")
 
 This library contains a series of tools to create a trading bot for Forex trading. It uses the [DWX Connect](https://github.com/darwinex/dwxconnect/) (modified) to send commands and receive information of MetaTrader.
 This library is created **based on a linux installation of MetaTrader**.
 
+![Test](https://github.com/sorul/tradeo/actions/workflows/testing_coverage.yml/badge.svg?branch=master)
+![codecov.io](https://codecov.io/github/sorul/tradeo/coverage.svg?branch=master)
+
 ## Installation
 
 ### Install the library
 
 #### PIP
 ```shell
 pip install tradeo
```

### Comparing `tradeo-0.17.0/pyproject.toml` & `tradeo-0.17.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "tradeo"
-version = "0.17.0"
+version = "0.17.1"
 description = ""
 authors = ["sorul <cromerovargas2d@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = "3.8.1"
+python = "~3.8.1"
 python-dotenv = "^1.0.0"
 pytz = "^2023.3.post1"
-pandas = "1.5.3"
+pandas = "^1.5.3"
 requests = "^2.31.0"
 
 [tool.poetry.dev-dependencies]
 freezegun = "^1.4.0"
 flake8-bugbear = "^24.1.17"
 flake8-print = "^5.0.0"
 flake8-builtins = "^2.2.0"
```

### Comparing `tradeo-0.17.0/tradeo/__init__.py` & `tradeo-0.17.1/tradeo/__init__.py`

 * *Files identical despite different names*

### Comparing `tradeo-0.17.0/tradeo/config.py` & `tradeo-0.17.1/tradeo/config.py`

 * *Files identical despite different names*

### Comparing `tradeo-0.17.0/tradeo/context_managers/blocker.py` & `tradeo-0.17.1/tradeo/context_managers/blocker.py`

 * *Files identical despite different names*

### Comparing `tradeo-0.17.0/tradeo/event_handlers/basic_event_handler.py` & `tradeo-0.17.1/tradeo/event_handlers/basic_event_handler.py`

 * *Files identical despite different names*

### Comparing `tradeo-0.17.0/tradeo/event_handlers/event_handler.py` & `tradeo-0.17.1/tradeo/event_handlers/event_handler.py`

 * *Files identical despite different names*

### Comparing `tradeo-0.17.0/tradeo/executable/basic_forex.py` & `tradeo-0.17.1/tradeo/executable/basic_forex.py`

 * *Files 1% similar despite different names*

```diff
@@ -171,7 +171,8 @@
     # we need to consider testing the removal of this condition.
     is_not_on_the_hour = now_date.minute != 0
     return is_weekday and is_not_on_the_hour
 
   def finish(self, mt_client: MT_Client) -> None:
     """Finish the forex bot."""
     mt_client.stop()
+    mt_client.deactivate()
```

### Comparing `tradeo-0.17.0/tradeo/executable/executable.py` & `tradeo-0.17.1/tradeo/executable/executable.py`

 * *Files identical despite different names*

### Comparing `tradeo-0.17.0/tradeo/files.py` & `tradeo-0.17.1/tradeo/files.py`

 * *Files identical despite different names*

### Comparing `tradeo-0.17.0/tradeo/log.py` & `tradeo-0.17.1/tradeo/log.py`

 * *Files identical despite different names*

### Comparing `tradeo-0.17.0/tradeo/mt_client.py` & `tradeo-0.17.1/tradeo/mt_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,23 +41,25 @@
 
   This includes all of the functions needed for communication with MT4/MT5.
   """
 
   def __init__(self,
                event_handler: Union[EventHandler, None] = None,
                sleep_delay: float = 0.005,
-               max_retry_command_seconds: int = 5 * 60
+               max_retry_command_seconds: int = 10,
+               files_subfolder: str = 'AgentFiles'
                ):
     """Initialize the attributes."""
     # Parameter attributes
     self.sleep_delay = sleep_delay
     self.max_retry_command_seconds = max_retry_command_seconds
     self.num_command_files = 50
 
     # Paths to output MT files
+    self.prefix_files_path = files_subfolder
     self.set_agent_paths()
 
     # Control attributes
     self.event_handler = event_handler
     self.lock = Lock()
     self._last_messages_millis = 0
     self.command_id = 0
@@ -66,24 +68,25 @@
     self.messages: messages_type = {'INFO': [], 'ERROR': []}
     self.open_orders: List[Order] = []
     self.account_info: account_info_type = {}
     self.market_data: attributes_data_type = {}
     self.bar_data: attributes_data_type = {}
     self.historical_data: historical_data_type = {}
     self.historical_trades: attributes_data_type = {}
-    self.successful_symbols: Set[str] = set()
+    self._successful_symbols: Set[str] = set()
 
     # State attributes
     self.activate()
 
   def set_agent_paths(self) -> None:
     """Set the paths to the files generated by MQL."""
     mt_files_path = Config.mt_files_path
-    self.prefix_files_path = 'AgentFiles'
-    if exists(mt_files_path):
+    if Path(mt_files_path).exists():
+      prefix_folder = Path(mt_files_path / self.prefix_files_path)
+      prefix_folder.mkdir(exist_ok=True)
       self.path_orders = Path(
           join(mt_files_path, self.prefix_files_path, 'Orders.json'))
       self.path_messages = Path(
           join(mt_files_path, self.prefix_files_path, 'Messages.json'))
       self.path_market_data = Path(
           join(mt_files_path, self.prefix_files_path, 'Market_Data.json'))
       self.path_bar_data = Path(
@@ -100,14 +103,19 @@
           join(mt_files_path, self.prefix_files_path,
                'Messages_Stored.json'))
       self.path_commands_prefix = Path(
           join(mt_files_path, self.prefix_files_path, 'Commands_'))
     else:
       log.error(f'mt_files_path: {mt_files_path} does not exist!')
 
+  @property
+  def successful_symbols(self) -> Set[str]:
+    """Return the set of successful symbols."""
+    return self._successful_symbols
+
   @staticmethod
   def start_thread(target: Callable) -> Thread:
     """To start the thread with a method as target."""
     thread = Thread(target=target, args=(), daemon=True)
     thread.start()
     return thread
```

### Comparing `tradeo-0.17.0/tradeo/mt_message.py` & `tradeo-0.17.1/tradeo/mt_message.py`

 * *Files identical despite different names*

### Comparing `tradeo-0.17.0/tradeo/mt_tb_expert.mq5` & `tradeo-0.17.1/tradeo/mt_tb_expert.mq5`

 * *Files identical despite different names*

### Comparing `tradeo-0.17.0/tradeo/order.py` & `tradeo-0.17.1/tradeo/order.py`

 * *Files identical despite different names*

### Comparing `tradeo-0.17.0/tradeo/order_type.py` & `tradeo-0.17.1/tradeo/order_type.py`

 * *Files identical despite different names*

### Comparing `tradeo-0.17.0/tradeo/paths.py` & `tradeo-0.17.1/tradeo/paths.py`

 * *Files identical despite different names*

### Comparing `tradeo-0.17.0/tradeo/strategies/basic_strategy.py` & `tradeo-0.17.1/tradeo/strategies/basic_strategy.py`

 * *Files identical despite different names*

### Comparing `tradeo-0.17.0/tradeo/strategies/strategy.py` & `tradeo-0.17.1/tradeo/strategies/strategy.py`

 * *Files identical despite different names*

### Comparing `tradeo-0.17.0/tradeo/trading_methods.py` & `tradeo-0.17.1/tradeo/trading_methods.py`

 * *Files identical despite different names*

### Comparing `tradeo-0.17.0/tradeo/utils.py` & `tradeo-0.17.1/tradeo/utils.py`

 * *Files identical despite different names*

### Comparing `tradeo-0.17.0/PKG-INFO` & `tradeo-0.17.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 Metadata-Version: 2.1
 Name: tradeo
-Version: 0.17.0
+Version: 0.17.1
 Summary: 
 Author: sorul
 Author-email: cromerovargas2d@gmail.com
-Requires-Python: ==3.8.1
+Requires-Python: >=3.8.1,<3.9.0
 Classifier: Programming Language :: Python :: 3
-Requires-Dist: pandas (==1.5.3)
+Requires-Dist: pandas (>=1.5.3,<2.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: pytz (>=2023.3.post1,<2024.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 # TRADEO - A forex trading framework using MetaTrader
-
-![alt text](docs/images/logo.PNG "Title")
+![Logo](docs/images/logo.PNG "Title")
 
 This library contains a series of tools to create a trading bot for Forex trading. It uses the [DWX Connect](https://github.com/darwinex/dwxconnect/) (modified) to send commands and receive information of MetaTrader.
 This library is created **based on a linux installation of MetaTrader**.
 
+![Test](https://github.com/sorul/tradeo/actions/workflows/testing_coverage.yml/badge.svg?branch=master)
+![codecov.io](https://codecov.io/github/sorul/tradeo/coverage.svg?branch=master)
+
 ## Installation
 
 ### Install the library
 
 #### PIP
 ```shell
 pip install tradeo
```

