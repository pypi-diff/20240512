# Comparing `tmp/volstreet-8.2.0.tar.gz` & `tmp/volstreet-8.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "volstreet-8.2.0.tar", last modified: Mon May  6 03:10:02 2024, max compression
+gzip compressed data, was "volstreet-8.2.1.tar", last modified: Sun May 12 11:54:46 2024, max compression
```

## Comparing `volstreet-8.2.0.tar` & `volstreet-8.2.1.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 03:10:02.170958 volstreet-8.2.0/
--rw-rw-rw-   0        0        0     1293 2024-05-06 03:10:02.169957 volstreet-8.2.0/PKG-INFO
--rw-rw-rw-   0        0        0      124 2024-03-14 04:36:05.000000 volstreet-8.2.0/README.md
--rw-rw-rw-   0        0        0       91 2024-03-14 04:36:05.000000 volstreet-8.2.0/pyproject.toml
--rw-rw-rw-   0        0        0     1155 2024-05-06 03:10:02.171957 volstreet-8.2.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-06 03:10:02.079141 volstreet-8.2.0/volstreet/
--rw-rw-rw-   0        0        0      442 2024-03-14 09:55:16.000000 volstreet-8.2.0/volstreet/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-06 03:10:02.098231 volstreet-8.2.0/volstreet/angel_interface/
--rw-rw-rw-   0        0        0      247 2024-04-26 02:47:59.000000 volstreet-8.2.0/volstreet/angel_interface/__init__.py
--rw-rw-rw-   0        0        0     3726 2024-04-26 02:48:50.000000 volstreet-8.2.0/volstreet/angel_interface/access_rate_handler.py
--rw-rw-rw-   0        0        0      274 2024-04-23 04:22:25.000000 volstreet-8.2.0/volstreet/angel_interface/active_session.py
--rw-rw-rw-   0        0        0     2843 2024-04-28 03:29:15.000000 volstreet-8.2.0/volstreet/angel_interface/async_interface.py
--rw-rw-rw-   0        0        0     7280 2024-03-14 04:36:05.000000 volstreet-8.2.0/volstreet/angel_interface/base_websocket.py
--rw-rw-rw-   0        0        0    18658 2024-04-26 03:17:20.000000 volstreet-8.2.0/volstreet/angel_interface/interface.py
--rw-rw-rw-   0        0        0     2501 2024-04-06 10:22:09.000000 volstreet-8.2.0/volstreet/angel_interface/login.py
--rw-rw-rw-   0        0        0     1988 2024-03-14 04:36:05.000000 volstreet-8.2.0/volstreet/angel_interface/order_websocket.py
--rw-rw-rw-   0        0        0    30773 2024-04-29 09:17:58.000000 volstreet-8.2.0/volstreet/angel_interface/price_websocket.py
--rw-rw-rw-   0        0        0     6687 2024-04-26 02:56:08.000000 volstreet-8.2.0/volstreet/angel_interface/smart_connect.py
-drwxrwxrwx   0        0        0        0 2024-05-06 03:10:02.116512 volstreet-8.2.0/volstreet/backtests/
--rw-rw-rw-   0        0        0      290 2024-04-28 14:01:14.000000 volstreet-8.2.0/volstreet/backtests/__init__.py
--rw-rw-rw-   0        0        0     4064 2024-04-23 04:22:25.000000 volstreet-8.2.0/volstreet/backtests/analysis.py
--rw-rw-rw-   0        0        0     4181 2024-05-04 08:33:34.000000 volstreet-8.2.0/volstreet/backtests/data_updation.py
--rw-rw-rw-   0        0        0    11857 2024-04-25 10:13:39.000000 volstreet-8.2.0/volstreet/backtests/database.py
--rw-rw-rw-   0        0        0    38400 2024-04-03 08:06:51.000000 volstreet-8.2.0/volstreet/backtests/delta_hedging.py
--rw-rw-rw-   0        0        0     5695 2024-03-14 04:36:05.000000 volstreet-8.2.0/volstreet/backtests/delta_optimizer.py
--rw-rw-rw-   0        0        0    48672 2024-05-02 12:46:20.000000 volstreet-8.2.0/volstreet/backtests/framework.py
--rw-rw-rw-   0        0        0     5410 2024-04-13 06:57:57.000000 volstreet-8.2.0/volstreet/backtests/intraday_backtest_abc.py
--rw-rw-rw-   0        0        0     7201 2024-05-05 08:31:29.000000 volstreet-8.2.0/volstreet/backtests/proxy_functions.py
--rw-rw-rw-   0        0        0     2707 2024-04-24 14:17:18.000000 volstreet-8.2.0/volstreet/backtests/result_processing.py
--rw-rw-rw-   0        0        0     6149 2024-05-04 09:19:15.000000 volstreet-8.2.0/volstreet/backtests/runner.py
--rw-rw-rw-   0        0        0     6446 2024-03-26 10:23:44.000000 volstreet-8.2.0/volstreet/backtests/tools.py
--rw-rw-rw-   0        0        0    15734 2024-04-13 06:57:57.000000 volstreet-8.2.0/volstreet/backtests/trend.py
--rw-rw-rw-   0        0        0     1923 2024-05-05 08:57:06.000000 volstreet-8.2.0/volstreet/backtests/underlying_info.py
--rw-rw-rw-   0        0        0    20882 2024-05-02 08:25:42.000000 volstreet-8.2.0/volstreet/blackscholes.py
--rw-rw-rw-   0        0        0     5574 2024-04-24 06:53:53.000000 volstreet-8.2.0/volstreet/config.py
--rw-rw-rw-   0        0        0     2162 2024-03-14 04:36:05.000000 volstreet-8.2.0/volstreet/database_connection.py
-drwxrwxrwx   0        0        0        0 2024-05-06 03:10:02.128637 volstreet-8.2.0/volstreet/datamodule/
--rw-rw-rw-   0        0        0      163 2024-04-13 05:46:57.000000 volstreet-8.2.0/volstreet/datamodule/__init__.py
--rw-rw-rw-   0        0        0     7358 2024-03-14 04:36:05.000000 volstreet-8.2.0/volstreet/datamodule/analysis.py
--rw-rw-rw-   0        0        0    21130 2024-03-14 04:36:05.000000 volstreet-8.2.0/volstreet/datamodule/archive.py
--rw-rw-rw-   0        0        0     9685 2024-05-04 09:32:35.000000 volstreet-8.2.0/volstreet/datamodule/data_handling.py
--rw-rw-rw-   0        0        0     4534 2024-03-14 04:36:05.000000 volstreet-8.2.0/volstreet/datamodule/eod_client.py
--rw-rw-rw-   0        0        0     5639 2024-03-14 04:36:05.000000 volstreet-8.2.0/volstreet/datamodule/gambling.py
--rw-rw-rw-   0        0        0     8098 2024-03-14 04:36:05.000000 volstreet-8.2.0/volstreet/datamodule/intraday_data.py
--rw-rw-rw-   0        0        0    15754 2024-03-26 10:23:44.000000 volstreet-8.2.0/volstreet/datamodule/stockmock.py
--rw-rw-rw-   0        0        0     1219 2024-03-14 04:36:05.000000 volstreet-8.2.0/volstreet/datamodule/trading_assistance.py
--rw-rw-rw-   0        0        0    25622 2024-05-06 02:53:39.000000 volstreet-8.2.0/volstreet/dealingroom.py
--rw-rw-rw-   0        0        0     2573 2024-04-03 08:06:51.000000 volstreet-8.2.0/volstreet/decorators.py
--rw-rw-rw-   0        0        0     1683 2024-03-14 04:36:05.000000 volstreet-8.2.0/volstreet/discord_bot.py
--rw-rw-rw-   0        0        0     1698 2024-03-14 04:36:05.000000 volstreet-8.2.0/volstreet/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-05-06 03:10:02.133434 volstreet-8.2.0/volstreet/historical_info/
--rw-rw-rw-   0        0        0      975 2024-04-24 06:53:53.000000 volstreet-8.2.0/volstreet/historical_info/__init__.py
--rw-rw-rw-   0        0        0    21031 2024-05-04 08:38:02.000000 volstreet-8.2.0/volstreet/historical_info/index_expiries.pkl
--rw-rw-rw-   0        0        0    16910 2024-05-04 09:35:37.000000 volstreet-8.2.0/volstreet/historical_info/market_days.pkl
-drwxrwxrwx   0        0        0        0 2024-05-06 03:10:02.134439 volstreet-8.2.0/volstreet/models/
--rw-rw-rw-   0        0        0      568 2024-04-29 10:45:14.000000 volstreet-8.2.0/volstreet/models/__init__.py
--rw-rw-rw-   0        0        0      772 2024-03-14 04:36:05.000000 volstreet-8.2.0/volstreet/parallelization.py
--rw-rw-rw-   0        0        0     1659 2024-04-06 06:31:33.000000 volstreet-8.2.0/volstreet/performance_tracking.py
-drwxrwxrwx   0        0        0        0 2024-05-06 03:10:02.137550 volstreet-8.2.0/volstreet/position_dashboard/
--rw-rw-rw-   0        0        0        0 2024-04-17 11:41:53.000000 volstreet-8.2.0/volstreet/position_dashboard/__init__.py
--rw-rw-rw-   0        0        0     1972 2024-04-17 11:41:53.000000 volstreet-8.2.0/volstreet/position_dashboard/app.py
--rw-rw-rw-   0        0        0      572 2024-04-17 11:41:53.000000 volstreet-8.2.0/volstreet/position_dashboard/formatting.py
-drwxrwxrwx   0        0        0        0 2024-05-06 03:10:02.148640 volstreet-8.2.0/volstreet/strategies/
--rw-rw-rw-   0        0        0      183 2024-05-03 07:00:07.000000 volstreet-8.2.0/volstreet/strategies/__init__.py
--rw-rw-rw-   0        0        0    32426 2024-05-06 02:53:39.000000 volstreet-8.2.0/volstreet/strategies/deployment.py
--rw-rw-rw-   0        0        0     1925 2024-05-03 06:56:48.000000 volstreet-8.2.0/volstreet/strategies/error_handling.py
--rw-rw-rw-   0        0        0    54994 2024-05-03 11:29:24.000000 volstreet-8.2.0/volstreet/strategies/helpers.py
--rw-rw-rw-   0        0        0     6352 2024-05-03 06:56:48.000000 volstreet-8.2.0/volstreet/strategies/monitoring.py
--rw-rw-rw-   0        0        0    18535 2024-05-02 10:20:37.000000 volstreet-8.2.0/volstreet/strategies/optimization.py
--rw-rw-rw-   0        0        0   106431 2024-05-06 02:59:53.000000 volstreet-8.2.0/volstreet/strategies/strats.py
--rw-rw-rw-   0        0        0      349 2024-04-12 11:13:05.000000 volstreet-8.2.0/volstreet/strategies/tools.py
-drwxrwxrwx   0        0        0        0 2024-05-06 03:10:02.153640 volstreet-8.2.0/volstreet/trade_interface/
--rw-rw-rw-   0        0        0      224 2024-04-17 11:41:53.000000 volstreet-8.2.0/volstreet/trade_interface/__init__.py
--rw-rw-rw-   0        0        0    26799 2024-04-23 04:22:25.000000 volstreet-8.2.0/volstreet/trade_interface/instruments.py
--rw-rw-rw-   0        0        0    19389 2024-04-29 10:19:25.000000 volstreet-8.2.0/volstreet/trade_interface/order_execution.py
--rw-rw-rw-   0        0        0    20204 2024-05-05 08:31:29.000000 volstreet-8.2.0/volstreet/trade_interface/underlyings.py
-drwxrwxrwx   0        0        0        0 2024-05-06 03:10:02.161809 volstreet-8.2.0/volstreet/utils/
--rw-rw-rw-   0        0        0      138 2024-03-14 04:36:05.000000 volstreet-8.2.0/volstreet/utils/__init__.py
--rw-rw-rw-   0        0        0      757 2024-03-14 04:36:05.000000 volstreet-8.2.0/volstreet/utils/change_config.py
--rw-rw-rw-   0        0        0     3052 2024-04-09 12:38:37.000000 volstreet-8.2.0/volstreet/utils/communication.py
--rw-rw-rw-   0        0        0    14475 2024-05-03 08:15:05.000000 volstreet-8.2.0/volstreet/utils/core.py
--rw-rw-rw-   0        0        0     4419 2024-03-14 04:36:05.000000 volstreet-8.2.0/volstreet/utils/data_io.py
--rw-rw-rw-   0        0        0     9915 2024-04-26 13:19:30.000000 volstreet-8.2.0/volstreet/utils/scrip_processing.py
--rw-rw-rw-   0        0        0     6488 2024-04-23 04:22:25.000000 volstreet-8.2.0/volstreet/vectorized_blackscholes.py
--rw-rw-rw-   0        0        0       20 2024-05-04 09:32:55.000000 volstreet-8.2.0/volstreet/volstreet_mode.json
-drwxrwxrwx   0        0        0        0 2024-05-06 03:10:02.167957 volstreet-8.2.0/volstreet/vslogging/
--rw-rw-rw-   0        0        0       81 2024-03-15 09:40:04.000000 volstreet-8.2.0/volstreet/vslogging/__init__.py
--rw-rw-rw-   0        0        0     2023 2024-03-26 10:23:44.000000 volstreet-8.2.0/volstreet/vslogging/formatters.py
--rw-rw-rw-   0        0        0     1492 2024-03-27 04:16:21.000000 volstreet-8.2.0/volstreet/vslogging/logging_config.json
--rw-rw-rw-   0        0        0      842 2024-03-26 10:23:44.000000 volstreet-8.2.0/volstreet/vslogging/logging_setup.py
--rw-rw-rw-   0        0        0     1390 2024-04-17 11:41:53.000000 volstreet-8.2.0/volstreet/vslogging/parsing.py
-drwxrwxrwx   0        0        0        0 2024-05-06 03:10:02.168970 volstreet-8.2.0/volstreet.egg-info/
--rw-rw-rw-   0        0        0     1293 2024-05-06 03:10:02.000000 volstreet-8.2.0/volstreet.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2833 2024-05-06 03:10:02.000000 volstreet-8.2.0/volstreet.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 03:10:02.000000 volstreet-8.2.0/volstreet.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      460 2024-05-06 03:10:02.000000 volstreet-8.2.0/volstreet.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-06 03:10:02.000000 volstreet-8.2.0/volstreet.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-12 11:54:46.062015 volstreet-8.2.1/
+-rw-rw-rw-   0        0        0     1293 2024-05-12 11:54:46.062015 volstreet-8.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0      124 2024-03-14 04:36:05.000000 volstreet-8.2.1/README.md
+-rw-rw-rw-   0        0        0       91 2024-03-14 04:36:05.000000 volstreet-8.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0     1155 2024-05-12 11:54:46.062015 volstreet-8.2.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-12 11:54:45.934477 volstreet-8.2.1/volstreet/
+-rw-rw-rw-   0        0        0      442 2024-03-14 09:55:16.000000 volstreet-8.2.1/volstreet/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-12 11:54:45.959890 volstreet-8.2.1/volstreet/angel_interface/
+-rw-rw-rw-   0        0        0      247 2024-04-26 02:47:59.000000 volstreet-8.2.1/volstreet/angel_interface/__init__.py
+-rw-rw-rw-   0        0        0     3726 2024-04-26 02:48:50.000000 volstreet-8.2.1/volstreet/angel_interface/access_rate_handler.py
+-rw-rw-rw-   0        0        0      274 2024-04-23 04:22:25.000000 volstreet-8.2.1/volstreet/angel_interface/active_session.py
+-rw-rw-rw-   0        0        0     3315 2024-05-06 03:22:49.000000 volstreet-8.2.1/volstreet/angel_interface/async_interface.py
+-rw-rw-rw-   0        0        0     7280 2024-03-14 04:36:05.000000 volstreet-8.2.1/volstreet/angel_interface/base_websocket.py
+-rw-rw-rw-   0        0        0    18658 2024-04-26 03:17:20.000000 volstreet-8.2.1/volstreet/angel_interface/interface.py
+-rw-rw-rw-   0        0        0     2501 2024-04-06 10:22:09.000000 volstreet-8.2.1/volstreet/angel_interface/login.py
+-rw-rw-rw-   0        0        0     1988 2024-03-14 04:36:05.000000 volstreet-8.2.1/volstreet/angel_interface/order_websocket.py
+-rw-rw-rw-   0        0        0    30773 2024-04-29 09:17:58.000000 volstreet-8.2.1/volstreet/angel_interface/price_websocket.py
+-rw-rw-rw-   0        0        0     6687 2024-04-26 02:56:08.000000 volstreet-8.2.1/volstreet/angel_interface/smart_connect.py
+drwxrwxrwx   0        0        0        0 2024-05-12 11:54:45.991426 volstreet-8.2.1/volstreet/backtests/
+-rw-rw-rw-   0        0        0      290 2024-04-28 14:01:14.000000 volstreet-8.2.1/volstreet/backtests/__init__.py
+-rw-rw-rw-   0        0        0     4064 2024-04-23 04:22:25.000000 volstreet-8.2.1/volstreet/backtests/analysis.py
+-rw-rw-rw-   0        0        0     4181 2024-05-04 08:33:34.000000 volstreet-8.2.1/volstreet/backtests/data_updation.py
+-rw-rw-rw-   0        0        0    11857 2024-04-25 10:13:39.000000 volstreet-8.2.1/volstreet/backtests/database.py
+-rw-rw-rw-   0        0        0    38400 2024-04-03 08:06:51.000000 volstreet-8.2.1/volstreet/backtests/delta_hedging.py
+-rw-rw-rw-   0        0        0     5695 2024-03-14 04:36:05.000000 volstreet-8.2.1/volstreet/backtests/delta_optimizer.py
+-rw-rw-rw-   0        0        0    48672 2024-05-02 12:46:20.000000 volstreet-8.2.1/volstreet/backtests/framework.py
+-rw-rw-rw-   0        0        0     5410 2024-04-13 06:57:57.000000 volstreet-8.2.1/volstreet/backtests/intraday_backtest_abc.py
+-rw-rw-rw-   0        0        0     7201 2024-05-05 08:31:29.000000 volstreet-8.2.1/volstreet/backtests/proxy_functions.py
+-rw-rw-rw-   0        0        0     2707 2024-04-24 14:17:18.000000 volstreet-8.2.1/volstreet/backtests/result_processing.py
+-rw-rw-rw-   0        0        0     6184 2024-05-09 04:00:00.000000 volstreet-8.2.1/volstreet/backtests/runner.py
+-rw-rw-rw-   0        0        0     6446 2024-03-26 10:23:44.000000 volstreet-8.2.1/volstreet/backtests/tools.py
+-rw-rw-rw-   0        0        0    15734 2024-04-13 06:57:57.000000 volstreet-8.2.1/volstreet/backtests/trend.py
+-rw-rw-rw-   0        0        0     1941 2024-05-09 03:54:28.000000 volstreet-8.2.1/volstreet/backtests/underlying_info.py
+-rw-rw-rw-   0        0        0    20882 2024-05-02 08:25:42.000000 volstreet-8.2.1/volstreet/blackscholes.py
+-rw-rw-rw-   0        0        0     5574 2024-04-24 06:53:53.000000 volstreet-8.2.1/volstreet/config.py
+-rw-rw-rw-   0        0        0     2162 2024-03-14 04:36:05.000000 volstreet-8.2.1/volstreet/database_connection.py
+drwxrwxrwx   0        0        0        0 2024-05-12 11:54:46.007459 volstreet-8.2.1/volstreet/datamodule/
+-rw-rw-rw-   0        0        0      163 2024-04-13 05:46:57.000000 volstreet-8.2.1/volstreet/datamodule/__init__.py
+-rw-rw-rw-   0        0        0     7358 2024-03-14 04:36:05.000000 volstreet-8.2.1/volstreet/datamodule/analysis.py
+-rw-rw-rw-   0        0        0    21130 2024-03-14 04:36:05.000000 volstreet-8.2.1/volstreet/datamodule/archive.py
+-rw-rw-rw-   0        0        0     9786 2024-05-09 13:39:03.000000 volstreet-8.2.1/volstreet/datamodule/data_handling.py
+-rw-rw-rw-   0        0        0     4534 2024-03-14 04:36:05.000000 volstreet-8.2.1/volstreet/datamodule/eod_client.py
+-rw-rw-rw-   0        0        0     5639 2024-03-14 04:36:05.000000 volstreet-8.2.1/volstreet/datamodule/gambling.py
+-rw-rw-rw-   0        0        0     8098 2024-03-14 04:36:05.000000 volstreet-8.2.1/volstreet/datamodule/intraday_data.py
+-rw-rw-rw-   0        0        0    15754 2024-03-26 10:23:44.000000 volstreet-8.2.1/volstreet/datamodule/stockmock.py
+-rw-rw-rw-   0        0        0     1219 2024-03-14 04:36:05.000000 volstreet-8.2.1/volstreet/datamodule/trading_assistance.py
+-rw-rw-rw-   0        0        0    25622 2024-05-06 02:53:39.000000 volstreet-8.2.1/volstreet/dealingroom.py
+-rw-rw-rw-   0        0        0     2573 2024-04-03 08:06:51.000000 volstreet-8.2.1/volstreet/decorators.py
+-rw-rw-rw-   0        0        0     1683 2024-03-14 04:36:05.000000 volstreet-8.2.1/volstreet/discord_bot.py
+-rw-rw-rw-   0        0        0     1698 2024-03-14 04:36:05.000000 volstreet-8.2.1/volstreet/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-05-12 11:54:46.007459 volstreet-8.2.1/volstreet/historical_info/
+-rw-rw-rw-   0        0        0      975 2024-04-24 06:53:53.000000 volstreet-8.2.1/volstreet/historical_info/__init__.py
+-rw-rw-rw-   0        0        0    21031 2024-05-04 08:38:02.000000 volstreet-8.2.1/volstreet/historical_info/index_expiries.pkl
+-rw-rw-rw-   0        0        0    16975 2024-05-11 04:49:24.000000 volstreet-8.2.1/volstreet/historical_info/market_days.pkl
+drwxrwxrwx   0        0        0        0 2024-05-12 11:54:46.007459 volstreet-8.2.1/volstreet/models/
+-rw-rw-rw-   0        0        0      568 2024-04-29 10:45:14.000000 volstreet-8.2.1/volstreet/models/__init__.py
+-rw-rw-rw-   0        0        0      772 2024-03-14 04:36:05.000000 volstreet-8.2.1/volstreet/parallelization.py
+-rw-rw-rw-   0        0        0     1659 2024-04-06 06:31:33.000000 volstreet-8.2.1/volstreet/performance_tracking.py
+drwxrwxrwx   0        0        0        0 2024-05-12 11:54:46.007459 volstreet-8.2.1/volstreet/position_dashboard/
+-rw-rw-rw-   0        0        0        0 2024-04-17 11:41:53.000000 volstreet-8.2.1/volstreet/position_dashboard/__init__.py
+-rw-rw-rw-   0        0        0     1972 2024-04-17 11:41:53.000000 volstreet-8.2.1/volstreet/position_dashboard/app.py
+-rw-rw-rw-   0        0        0      572 2024-04-17 11:41:53.000000 volstreet-8.2.1/volstreet/position_dashboard/formatting.py
+drwxrwxrwx   0        0        0        0 2024-05-12 11:54:46.023094 volstreet-8.2.1/volstreet/strategies/
+-rw-rw-rw-   0        0        0      183 2024-05-03 07:00:07.000000 volstreet-8.2.1/volstreet/strategies/__init__.py
+-rw-rw-rw-   0        0        0    32426 2024-05-06 02:53:39.000000 volstreet-8.2.1/volstreet/strategies/deployment.py
+-rw-rw-rw-   0        0        0     1925 2024-05-03 06:56:48.000000 volstreet-8.2.1/volstreet/strategies/error_handling.py
+-rw-rw-rw-   0        0        0    56751 2024-05-10 10:17:25.000000 volstreet-8.2.1/volstreet/strategies/helpers.py
+-rw-rw-rw-   0        0        0     6352 2024-05-03 06:56:48.000000 volstreet-8.2.1/volstreet/strategies/monitoring.py
+-rw-rw-rw-   0        0        0    18535 2024-05-02 10:20:37.000000 volstreet-8.2.1/volstreet/strategies/optimization.py
+-rw-rw-rw-   0        0        0   106164 2024-05-10 03:43:38.000000 volstreet-8.2.1/volstreet/strategies/strats.py
+-rw-rw-rw-   0        0        0      349 2024-04-12 11:13:05.000000 volstreet-8.2.1/volstreet/strategies/tools.py
+drwxrwxrwx   0        0        0        0 2024-05-12 11:54:46.023094 volstreet-8.2.1/volstreet/trade_interface/
+-rw-rw-rw-   0        0        0      224 2024-04-17 11:41:53.000000 volstreet-8.2.1/volstreet/trade_interface/__init__.py
+-rw-rw-rw-   0        0        0    26799 2024-04-23 04:22:25.000000 volstreet-8.2.1/volstreet/trade_interface/instruments.py
+-rw-rw-rw-   0        0        0    19389 2024-04-29 10:19:25.000000 volstreet-8.2.1/volstreet/trade_interface/order_execution.py
+-rw-rw-rw-   0        0        0    20204 2024-05-05 08:31:29.000000 volstreet-8.2.1/volstreet/trade_interface/underlyings.py
+drwxrwxrwx   0        0        0        0 2024-05-12 11:54:46.040254 volstreet-8.2.1/volstreet/utils/
+-rw-rw-rw-   0        0        0      138 2024-03-14 04:36:05.000000 volstreet-8.2.1/volstreet/utils/__init__.py
+-rw-rw-rw-   0        0        0      757 2024-03-14 04:36:05.000000 volstreet-8.2.1/volstreet/utils/change_config.py
+-rw-rw-rw-   0        0        0     3052 2024-04-09 12:38:37.000000 volstreet-8.2.1/volstreet/utils/communication.py
+-rw-rw-rw-   0        0        0    14475 2024-05-03 08:15:05.000000 volstreet-8.2.1/volstreet/utils/core.py
+-rw-rw-rw-   0        0        0     4419 2024-03-14 04:36:05.000000 volstreet-8.2.1/volstreet/utils/data_io.py
+-rw-rw-rw-   0        0        0     9915 2024-04-26 13:19:30.000000 volstreet-8.2.1/volstreet/utils/scrip_processing.py
+-rw-rw-rw-   0        0        0     6488 2024-04-23 04:22:25.000000 volstreet-8.2.1/volstreet/vectorized_blackscholes.py
+-rw-rw-rw-   0        0        0       20 2024-05-11 04:46:04.000000 volstreet-8.2.1/volstreet/volstreet_mode.json
+drwxrwxrwx   0        0        0        0 2024-05-12 11:54:46.054761 volstreet-8.2.1/volstreet/vslogging/
+-rw-rw-rw-   0        0        0       81 2024-03-15 09:40:04.000000 volstreet-8.2.1/volstreet/vslogging/__init__.py
+-rw-rw-rw-   0        0        0     2023 2024-03-26 10:23:44.000000 volstreet-8.2.1/volstreet/vslogging/formatters.py
+-rw-rw-rw-   0        0        0     1492 2024-03-27 04:16:21.000000 volstreet-8.2.1/volstreet/vslogging/logging_config.json
+-rw-rw-rw-   0        0        0      842 2024-03-26 10:23:44.000000 volstreet-8.2.1/volstreet/vslogging/logging_setup.py
+-rw-rw-rw-   0        0        0     1390 2024-04-17 11:41:53.000000 volstreet-8.2.1/volstreet/vslogging/parsing.py
+drwxrwxrwx   0        0        0        0 2024-05-12 11:54:46.054761 volstreet-8.2.1/volstreet.egg-info/
+-rw-rw-rw-   0        0        0     1293 2024-05-12 11:54:45.000000 volstreet-8.2.1/volstreet.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2833 2024-05-12 11:54:45.000000 volstreet-8.2.1/volstreet.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-12 11:54:45.000000 volstreet-8.2.1/volstreet.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      460 2024-05-12 11:54:45.000000 volstreet-8.2.1/volstreet.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-12 11:54:45.000000 volstreet-8.2.1/volstreet.egg-info/top_level.txt
```

### Comparing `volstreet-8.2.0/PKG-INFO` & `volstreet-8.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: volstreet
-Version: 8.2.0
+Version: 8.2.1
 Summary: VolStreet is a Python library for automated trading
 Home-page: https://github.com/rahulthakkr/volstreet
 Author: Rahul Thakkar
 Author-email: r.thakkar15@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `volstreet-8.2.0/setup.cfg` & `volstreet-8.2.1/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2076 6f6c 7374 7265 6574 0d0a 7665   = volstreet..ve
-00000020: 7273 696f 6e20 3d20 382e 322e 300d 0a61  rsion = 8.2.0..a
+00000020: 7273 696f 6e20 3d20 382e 322e 310d 0a61  rsion = 8.2.1..a
 00000030: 7574 686f 7220 3d20 5261 6875 6c20 5468  uthor = Rahul Th
 00000040: 616b 6b61 720d 0a61 7574 686f 725f 656d  akkar..author_em
 00000050: 6169 6c20 3d20 722e 7468 616b 6b61 7231  ail = r.thakkar1
 00000060: 3540 676d 6169 6c2e 636f 6d0d 0a64 6573  5@gmail.com..des
 00000070: 6372 6970 7469 6f6e 203d 2056 6f6c 5374  cription = VolSt
 00000080: 7265 6574 2069 7320 6120 5079 7468 6f6e  reet is a Python
 00000090: 206c 6962 7261 7279 2066 6f72 2061 7574   library for aut
```

### Comparing `volstreet-8.2.0/volstreet/angel_interface/access_rate_handler.py` & `volstreet-8.2.1/volstreet/angel_interface/access_rate_handler.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.2.0/volstreet/angel_interface/async_interface.py` & `volstreet-8.2.1/volstreet/angel_interface/async_interface.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,52 +1,61 @@
 import asyncio
 from collections import defaultdict
 import functools
+from volstreet.utils.communication import notifier
+from volstreet import config
 from volstreet.config import token_exchange_dict, logger
 from volstreet.angel_interface.active_session import ActiveSession
 from volstreet.angel_interface.interface import format_quote_response
 
 
-def retry_on_error(func):
-    """Only for async functions. Retries the function 5 times with exponential backoff if an error occurs."""
+def retry_on_error(notify=False):
+    def decorator(func):
+        """Only for async functions. Retries the function 5 times with exponential backoff if an error occurs."""
+
+        @functools.wraps(func)
+        async def async_wrapped(*args, **kwargs):
+            sleep_time = 1
+            for attempt in range(5):
+                try:
+                    return await func(*args, **kwargs)
+                except Exception as e:
+                    message = (
+                        f"Attempt {attempt + 1} function {func.__name__} failed with error {e}. "
+                        f"Retrying in {sleep_time} seconds."
+                    )
+                    if notify:
+                        notifier(
+                            message, config.ERROR_NOTIFICATION_SETTINGS["url"], "ERROR"
+                        )
+                    if attempt < 4:
+                        logger.warning(message, exc_info=True)
+                        await asyncio.sleep(sleep_time)
+                        sleep_time *= 1.2  # Exponential backoff
+                    else:
+                        logger.error(f"Max attempts reached. {message}")
+                        raise e
 
-    @functools.wraps(func)
-    async def async_wrapped(*args, **kwargs):
-        sleep_time = 1
-        for attempt in range(5):
-            try:
-                return await func(*args, **kwargs)
-            except Exception as e:
-                message = (
-                    f"Attempt {attempt + 1} function {func.__name__} failed with error {e}. "
-                    f"Retrying in {sleep_time} seconds."
-                )
-                if attempt < 4:
-                    logger.warning(message, exc_info=True)
-                    await asyncio.sleep(sleep_time)
-                    sleep_time *= 1.2  # Exponential backoff
-                else:
-                    logger.error(f"Max attempts reached. {message}")
-                    raise e
+        return async_wrapped
 
-    return async_wrapped
+    return decorator
 
 
-@retry_on_error
+@retry_on_error(notify=False)
 async def get_ltp_async(token, session=None):
     params = {
         "exchange": token_exchange_dict.get(token),
         "symboltoken": token,
         "tradingsymbol": "",
     }
     response = await ActiveSession.obj.async_get_ltp(params, session)
     return response["data"]["ltp"]
 
 
-@retry_on_error
+@retry_on_error(notify=False)
 async def get_quotes_async(
     tokens: list, mode: str = "FULL", return_type="dict", session=None
 ):
     payload = defaultdict(list)
     for token in tokens:
         exchange = token_exchange_dict.get(token)
         if exchange:
@@ -60,24 +69,24 @@
     response = format_quote_response(response)
     if return_type.lower() == "dict":
         return {entry["token"]: entry for entry in response}
     elif return_type.lower() == "list":
         return response
 
 
-@retry_on_error
+@retry_on_error(notify=True)
 async def place_order_async(params: dict, session=None):
     response = await ActiveSession.obj.async_place_order(params, session)
     return response["data"]
 
 
-@retry_on_error
+@retry_on_error(notify=False)
 async def unique_order_status_async(unique_order_id: str, session=None):
     response = await ActiveSession.obj.async_unique_order_status(
         unique_order_id, session
     )
     return response["data"]
 
 
-@retry_on_error
+@retry_on_error(notify=False)
 async def modify_order_async(params: dict, session=None):
     return await ActiveSession.obj.async_modify_order(params, session)
```

### Comparing `volstreet-8.2.0/volstreet/angel_interface/base_websocket.py` & `volstreet-8.2.1/volstreet/angel_interface/base_websocket.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.2.0/volstreet/angel_interface/interface.py` & `volstreet-8.2.1/volstreet/angel_interface/interface.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.2.0/volstreet/angel_interface/login.py` & `volstreet-8.2.1/volstreet/angel_interface/login.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.2.0/volstreet/angel_interface/order_websocket.py` & `volstreet-8.2.1/volstreet/angel_interface/order_websocket.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.2.0/volstreet/angel_interface/price_websocket.py` & `volstreet-8.2.1/volstreet/angel_interface/price_websocket.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.2.0/volstreet/angel_interface/smart_connect.py` & `volstreet-8.2.1/volstreet/angel_interface/smart_connect.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.2.0/volstreet/backtests/analysis.py` & `volstreet-8.2.1/volstreet/backtests/analysis.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.2.0/volstreet/backtests/data_updation.py` & `volstreet-8.2.1/volstreet/backtests/data_updation.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.2.0/volstreet/backtests/database.py` & `volstreet-8.2.1/volstreet/backtests/database.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.2.0/volstreet/backtests/delta_hedging.py` & `volstreet-8.2.1/volstreet/backtests/delta_hedging.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.2.0/volstreet/backtests/delta_optimizer.py` & `volstreet-8.2.1/volstreet/backtests/delta_optimizer.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.2.0/volstreet/backtests/framework.py` & `volstreet-8.2.1/volstreet/backtests/framework.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.2.0/volstreet/backtests/intraday_backtest_abc.py` & `volstreet-8.2.1/volstreet/backtests/intraday_backtest_abc.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.2.0/volstreet/backtests/proxy_functions.py` & `volstreet-8.2.1/volstreet/backtests/proxy_functions.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.2.0/volstreet/backtests/result_processing.py` & `volstreet-8.2.1/volstreet/backtests/result_processing.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.2.0/volstreet/backtests/runner.py` & `volstreet-8.2.1/volstreet/backtests/runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
         self,
         only_expiry: bool = False,
         num_strikes: int = 50,
         num_exp: int = 2,
         start_time: tuple[int, int] = (9, 16),
         end_time: tuple[int, int] = (15, 30),
         include_vix_data: bool = False,
-    ) -> None:
+    ) -> pd.DataFrame:
         valid_range = pd.date_range(self.start_date, self.end_date)
         valid_range = [day.date() for day in valid_range if day.date() in market_days]
 
         if only_expiry:
             target_days = map(lambda x: x.date(), self.underlying.expiry_dates)
             target_days = [day for day in target_days if day in valid_range]
         else:
@@ -117,14 +117,15 @@
                     )
                     error_list.append(date)
 
             config.logger.info(
                 f"Finished running the strategy {self.strategy.__name__} from {self.start_date} to {self.end_date}. "
                 f"Total errors: {len(error_list)}. Error days: {error_list}"
             )
+            return result
 
 
 def get_parallel_runners(
     underlying: UnderlyingInfo,
     start_date: datetime,
     end_date: datetime,
     strategy,
```

### Comparing `volstreet-8.2.0/volstreet/backtests/tools.py` & `volstreet-8.2.1/volstreet/backtests/tools.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.2.0/volstreet/backtests/trend.py` & `volstreet-8.2.1/volstreet/backtests/trend.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.2.0/volstreet/backtests/underlying_info.py` & `volstreet-8.2.1/volstreet/backtests/underlying_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,8 +45,8 @@
     nearest_exp_dates = sorted(filtered_dates)
     if n_exp == 1:
         return nearest_exp_dates[0] if len(nearest_exp_dates) != 0 else None
     if len(nearest_exp_dates) < n_exp:
         logger.warning(f"Insufficient expiry dates for {underlying} on {date_time}")
         while len(nearest_exp_dates) < n_exp:
             nearest_exp_dates = nearest_exp_dates.append(np.nan)
-    return nearest_exp_dates[:n_exp]
+    return pd.DatetimeIndex(nearest_exp_dates[:n_exp])
```

### Comparing `volstreet-8.2.0/volstreet/blackscholes.py` & `volstreet-8.2.1/volstreet/blackscholes.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.2.0/volstreet/config.py` & `volstreet-8.2.1/volstreet/config.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.2.0/volstreet/database_connection.py` & `volstreet-8.2.1/volstreet/database_connection.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.2.0/volstreet/datamodule/analysis.py` & `volstreet-8.2.1/volstreet/datamodule/analysis.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.2.0/volstreet/datamodule/archive.py` & `volstreet-8.2.1/volstreet/datamodule/archive.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.2.0/volstreet/datamodule/data_handling.py` & `volstreet-8.2.1/volstreet/datamodule/data_handling.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import io
 import pandas as pd
 import os
 import ftplib
 import warnings
 from datetime import datetime, timedelta
 import re
 from sqlalchemy import create_engine
@@ -204,27 +205,25 @@
     df["expiry"] = pd.to_datetime(df["expiry"])
 
     df.to_sql("index_options", con=engine, if_exists="append", index=False)
 
     logger.info(f"Inserted {csv_file} into the database")
 
 
-def get_new_daily_data(
-    database_connection, remote_base_directory, local_base_directory
-):
+def get_new_daily_data(database_connection, remote_base_directory):
     host = os.getenv("GDFL_FTP_HOST")
     username = os.getenv("GDFL_FTP_USER")
     password = os.getenv("GDFL_FTP_PASS")
 
     dates_present = database_connection.execute_query(
         "SELECT DISTINCT DATE(timestamp) FROM index_options WHERE underlying = 'NIFTY'"
     )  # Nifty as a proxy to get the max date of NSE data (DB contains NSE and BSE data)
     dates_present = [date[0] for date in dates_present]
 
-    new_files = []  # List to keep track of new files
+    dataframes = []  # List to keep track of new dataframes
     for attempt in range(3):
         try:
             with FTPConnection(host, username, password) as ftp:
                 zip_files = find_zip_files(ftp, remote_base_directory)
                 zip_files = [
                     file for file in zip_files if "CONTRACT" not in file
                 ]  # Filter out CONTRACT files
@@ -234,19 +233,25 @@
                 dates_of_files = [
                     datetime.strptime(date, "%d%m%Y").date() for date in dates_of_files
                 ]
                 for file, date in zip(zip_files, dates_of_files):
                     zip_name = file.split("/")[-1]
                     if date not in dates_present:
                         logger.info(f"Downloading {zip_name}")
-                        local_path = os.path.join(local_base_directory, zip_name)
-                        with open(local_path, "wb") as local_file:
-                            ftp.retrbinary("RETR " + file, local_file.write)
-                        new_files.append(zip_name)  # Add the new file to the list
-            return new_files
+                        zip_data = io.BytesIO()
+                        ftp.retrbinary("RETR " + file, zip_data.write)
+                        zip_data.seek(0)  # Go to the start of the BytesIO object
+                        csv_name = zip_name.split(".")[0] + ".csv"
+                        with zipfile.ZipFile(zip_data, "r") as zip_ref:
+                            with zip_ref.open(csv_name) as csv_file:
+                                df = pd.read_csv(csv_file)
+                                dataframes.append(
+                                    df
+                                )  # Add the new dataframe to the list
+            return dataframes
         except ftplib.error_temp as e:
             logger.warning(f"Error in downloading data from GDFL: {e}")
     logger.error("Failed to download data from GDFL")
 
 
 def upload_option_data(processed_data, database_connection):
     with create_engine(database_connection._alchemy_engine_url).connect() as conn:
@@ -256,15 +261,10 @@
 def unzip_file(zip_path, csv_filename):
     with zipfile.ZipFile(zip_path, "r") as zip_file:
         with zip_file.open(csv_filename) as csv_file:
             df = pd.read_csv(csv_file)
     return df
 
 
-def process_and_upload_zip_file(
-    local_directory: str, zip_file_name: str, database_connection
-):
-    local_file_path = os.path.join(local_directory, zip_file_name)
-    csv_name = zip_file_name.split(".")[0] + ".csv"
-    csv_data = unzip_file(local_file_path, csv_name)
-    processed_data = process_daily_prices(csv_data)
+def process_and_upload_data(data: pd.DataFrame, database_connection):
+    processed_data = process_daily_prices(data)
     upload_option_data(processed_data, database_connection)
```

### Comparing `volstreet-8.2.0/volstreet/datamodule/eod_client.py` & `volstreet-8.2.1/volstreet/datamodule/eod_client.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.2.0/volstreet/datamodule/gambling.py` & `volstreet-8.2.1/volstreet/datamodule/gambling.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.2.0/volstreet/datamodule/intraday_data.py` & `volstreet-8.2.1/volstreet/datamodule/intraday_data.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.2.0/volstreet/datamodule/stockmock.py` & `volstreet-8.2.1/volstreet/datamodule/stockmock.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.2.0/volstreet/datamodule/trading_assistance.py` & `volstreet-8.2.1/volstreet/datamodule/trading_assistance.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.2.0/volstreet/dealingroom.py` & `volstreet-8.2.1/volstreet/dealingroom.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.2.0/volstreet/decorators.py` & `volstreet-8.2.1/volstreet/decorators.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.2.0/volstreet/discord_bot.py` & `volstreet-8.2.1/volstreet/discord_bot.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.2.0/volstreet/exceptions.py` & `volstreet-8.2.1/volstreet/exceptions.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.2.0/volstreet/historical_info/__init__.py` & `volstreet-8.2.1/volstreet/historical_info/__init__.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.2.0/volstreet/historical_info/index_expiries.pkl` & `volstreet-8.2.1/volstreet/historical_info/index_expiries.pkl`

 * *Files identical despite different names*

### Comparing `volstreet-8.2.0/volstreet/historical_info/market_days.pkl` & `volstreet-8.2.1/volstreet/historical_info/market_days.pkl`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 8004 9503 4200 0000 0000 005d 9428 8c08  ....B......].(..
+00000000: 8004 9544 4200 0000 0000 005d 9428 8c08  ...DB......].(..
 00000010: 6461 7465 7469 6d65 948c 0464 6174 6594  datetime...date.
 00000020: 9394 4304 07e3 0201 9485 9452 9468 0343  ..C........R.h.C
 00000030: 0407 e302 0494 8594 5294 6803 4304 07e3  ........R.h.C...
 00000040: 0205 9485 9452 9468 0343 0407 e302 0694  .....R.h.C......
 00000050: 8594 5294 6803 4304 07e3 0207 9485 9452  ..R.h.C........R
 00000060: 9468 0343 0407 e302 0894 8594 5294 6803  .h.C........R.h.
 00000070: 4304 07e3 020b 9485 9452 9468 0343 0407  C........R.h.C..
@@ -1050,8 +1050,12 @@
 00004190: 0413 9485 9452 9468 0343 0407 e804 1694  .....R.h.C......
 000041a0: 8594 5294 6803 4304 07e8 0417 9485 9452  ..R.h.C........R
 000041b0: 9468 0343 0407 e804 1894 8594 5294 6803  .h.C........R.h.
 000041c0: 4304 07e8 0419 9485 9452 9468 0343 0407  C........R.h.C..
 000041d0: e804 1a94 8594 5294 6803 4304 07e8 041d  ......R.h.C.....
 000041e0: 9485 9452 9468 0343 0407 e804 1e94 8594  ...R.h.C........
 000041f0: 5294 6803 4304 07e8 0502 9485 9452 9468  R.h.C........R.h
-00004200: 0343 0407 e805 0394 8594 5294 652e       .C........R.e.
+00004200: 0343 0407 e805 0394 8594 5294 6803 4304  .C........R.h.C.
+00004210: 07e8 0506 9485 9452 9468 0343 0407 e805  .......R.h.C....
+00004220: 0794 8594 5294 6803 4304 07e8 0508 9485  ....R.h.C.......
+00004230: 9452 9468 0343 0407 e805 0994 8594 5294  .R.h.C........R.
+00004240: 6803 4304 07e8 050a 9485 9452 9465 2e    h.C........R.e.
```

### Comparing `volstreet-8.2.0/volstreet/models/__init__.py` & `volstreet-8.2.1/volstreet/models/__init__.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.2.0/volstreet/parallelization.py` & `volstreet-8.2.1/volstreet/parallelization.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.2.0/volstreet/performance_tracking.py` & `volstreet-8.2.1/volstreet/performance_tracking.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.2.0/volstreet/position_dashboard/app.py` & `volstreet-8.2.1/volstreet/position_dashboard/app.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.2.0/volstreet/position_dashboard/formatting.py` & `volstreet-8.2.1/volstreet/position_dashboard/formatting.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.2.0/volstreet/strategies/deployment.py` & `volstreet-8.2.1/volstreet/strategies/deployment.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.2.0/volstreet/strategies/error_handling.py` & `volstreet-8.2.1/volstreet/strategies/error_handling.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.2.0/volstreet/strategies/helpers.py` & `volstreet-8.2.1/volstreet/strategies/helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -995,14 +995,49 @@
 
     if np.isnan(target_gamma):
         setattr(target_greeks, "gamma", counter_gamma)
 
     return target_greeks
 
 
+def get_above_below_strangles_with_prices(
+    underlying: Index,
+    spot_price: float,
+    expiry: str,
+    for_type: bool = None,
+) -> tuple[tuple[Strangle, tuple[float, float]], tuple[Strangle, tuple[float, float]]]:
+    above_strangle, above_prices = get_strangle_with_prices(
+        underlying, spot_price, 1, expiry, for_type
+    )
+    below_strangle, below_prices = get_strangle_with_prices(
+        underlying, spot_price, -1, expiry, for_type
+    )
+    return (above_strangle, above_prices), (below_strangle, below_prices)
+
+
+def get_strangle_with_prices(
+    underlying: Index,
+    spot_price: float,
+    n_steps: int,
+    expiry: str,
+    for_type: bool = None,
+) -> tuple[Strangle, tuple[float, float]]:
+    offset = underlying.base * n_steps
+    # Dividing offset by 2 because sometimes the above strike is very close to the spot
+    strike = find_strike(spot_price + (offset / 2), underlying.base)
+    strangle: Strangle = Strangle(strike, strike, underlying.name, expiry)
+    prices = strangle.fetch_ltp(for_type=for_type)
+    return strangle, prices
+
+
+def disparity_calculator(call_ltp, put_ltp):
+    disparity = abs(call_ltp - put_ltp) / min(call_ltp, put_ltp)
+    return disparity
+
+
 def efficient_ltp_for_options(
     options: list[Option] | set[Option],
 ) -> dict[Option, float]:
     """
     Fetches the latest trading prices (LTPs) for a set of options.
 
     :param options: A list of Option objects.
@@ -1350,41 +1385,50 @@
 
 def sleep_until_next_action(
     interval_minutes: int,
     exit_time: tuple[int, int],
     special_condition: Callable = lambda: False,
     tasks_to_perform: list[Callable] = None,
 ) -> None:
+    # Lets handle cases when tuple is either (hour, minute) or (hour, minute, second)
+    exit_hour, exit_minute, exit_second = exit_time + (0,) * (3 - len(exit_time))
     time_now = current_time()
     if tasks_to_perform is None:
         tasks_to_perform = []
 
     # Determining the next timestamp
     if isinstance(interval_minutes, int):
-        next_timestamp = (time_now + timedelta(minutes=interval_minutes)).replace(
+        # Rounding the time_now to the nearest minute
+        rounded_time_now = (time_now + timedelta(seconds=30)).replace(
             second=0, microsecond=0
         )
+        next_timestamp = (
+            rounded_time_now + timedelta(minutes=(interval_minutes - 1))
+        ).replace(second=58, microsecond=0)
+        if next_timestamp <= time_now:
+            next_timestamp += timedelta(minutes=1)
     elif isinstance(interval_minutes, float):
         next_timestamp = time_now + timedelta(minutes=interval_minutes)
     else:
         raise ValueError("Invalid interval_minutes value")
     next_timestamp = min(
         next_timestamp,
         current_time().replace(
-            hour=exit_time[0], minute=exit_time[1], second=0, microsecond=0
+            hour=exit_hour, minute=exit_minute, second=exit_second, microsecond=0
         ),
     )
 
     for task in tasks_to_perform:
         task()
 
     while current_time() < next_timestamp:
         if special_condition():
             return
         sleep(1)
+    sleep(0.05)  # Just in case to prevent a very tight loop
 
 
 def filter_out_illiquid_options(
     options: list[ActiveOption], timedelta_minutes: float | int = 3
 ) -> list[ActiveOption]:
     try:
         if LiveFeeds.price_feed_connected() and all(
```

### Comparing `volstreet-8.2.0/volstreet/strategies/monitoring.py` & `volstreet-8.2.1/volstreet/strategies/monitoring.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.2.0/volstreet/strategies/optimization.py` & `volstreet-8.2.1/volstreet/strategies/optimization.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.2.0/volstreet/strategies/strats.py` & `volstreet-8.2.1/volstreet/strategies/strats.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,14 +38,16 @@
     place_option_order_and_notify,
     execute_instructions,
     cancel_pending_orders,
 )
 from volstreet.strategies.helpers import (
     sleep_until_next_action,
     round_shares_to_lot_size,
+    get_above_below_strangles_with_prices,
+    disparity_calculator,
     most_equal_strangle,
     DeltaPosition,
     TrendPosition,
     PositionMonitor,
     load_current_strangle,
     approve_execution,
     notify_pnl,
@@ -1875,15 +1877,15 @@
     notification_url: Optional[str] = None,
     strategy_tag: Optional[str] = "Quick Strangle",
 ):
 
     if not exposure and not investment:
         raise ValueError("Exposure or investment must be provided")
 
-    DISPARITY_THRESHOLD = 1000
+    DISPARITY_THRESHOLD = 0.2
 
     # Entering the main function
     if time(*scan_exit_time) < current_time().time():
         notifier(
             f"{underlying.name} {strategy_tag} not being deployed after exit time",
             notification_url,
             "INFO",
@@ -1893,29 +1895,20 @@
     def fetch_spot_and_basis(underlying: Index, expiry: str) -> tuple[float, float]:
         spot_price = underlying.fetch_ltp()
         current_basis = underlying.get_basis_for_expiry(
             expiry=expiry, underlying_price=spot_price
         )
         return spot_price, current_basis
 
-    def get_strangle_with_prices(
-        underlying: Index, offset: float, expiry: str
-    ) -> tuple[Strangle, tuple[float, float]]:
-        # Dividing offset by 2 to get the two strikes between which the spot lies
-        strike = find_strike(spot + (offset / 2), underlying.base)
-        strangle: Strangle = Strangle(strike, strike, underlying.name, expiry)
-        prices = strangle.fetch_ltp(for_type=action.value)
-        return strangle, prices
-
     def calculate_ivs(strangle, spot_price, r, prices):
         ivs = strangle.fetch_ivs(spot=spot_price, r=r, prices=prices)
         return np.mean(ivs)
 
     def disparity_check(call_ltp, put_ltp):
-        disparity = abs(call_ltp - put_ltp) / min(call_ltp, put_ltp)
+        disparity = disparity_calculator(call_ltp, put_ltp)
         return disparity < DISPARITY_THRESHOLD
 
     last_log_time = current_time()
 
     def log_iv_status():
         nonlocal ivs, last_log_time
         if current_time() - last_log_time > timedelta(seconds=0.1):
@@ -1963,20 +1956,19 @@
     if stop_loss is None:
         stop_loss = np.nan
 
     position = PositionMonitor(underlying)
 
     while current_time().time() < time(*scan_exit_time):
         spot, basis = fetch_spot_and_basis(underlying, expiry)
-        above_strangle, above_prices = get_strangle_with_prices(
-            underlying, underlying.base, expiry
-        )
-        below_strangle, below_prices = get_strangle_with_prices(
-            underlying, -underlying.base, expiry
+        above_info, below_info = get_above_below_strangles_with_prices(
+            underlying, spot, expiry, action.value
         )
+        above_strangle, above_prices = above_info
+        below_strangle, below_prices = below_info
         ivs = {}
         if disparity_check(*above_prices):
             ivs[above_strangle] = calculate_ivs(
                 above_strangle, spot, basis, above_prices
             )
         if disparity_check(*below_prices):
             ivs[below_strangle] = calculate_ivs(
@@ -2630,24 +2622,30 @@
             f"{underlying.name} {strategy_tag} not being deployed after exit time",
             notification_url,
             "INFO",
         )
         return
 
     spot_price = underlying.fetch_ltp()
-    atm_strike = find_strike(spot_price, underlying.base)
     expiry = underlying.current_expiry
+    above_info, below_info = get_above_below_strangles_with_prices(
+        underlying,
+        spot_price,
+        expiry,
+    )
+    straddle, prices = min(
+        above_info, below_info, key=lambda info: disparity_calculator(*info[1])
+    )
+
     quantity_in_lots = convert_exposure_to_lots(
         exposure, spot_price, underlying.lot_size
     )
 
-    straddle = Straddle(atm_strike, underlying.name, expiry)
-
     notifier(
-        f"{underlying.name} {strategy_tag} starting with straddle {straddle}",
+        f"{underlying.name} {strategy_tag} starting with straddle {straddle} and prices {prices}",
         notification_url,
         "INFO",
     )
 
     # Placing the main order
     execution_details = execute_instructions(
         {
```

### Comparing `volstreet-8.2.0/volstreet/trade_interface/instruments.py` & `volstreet-8.2.1/volstreet/trade_interface/instruments.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.2.0/volstreet/trade_interface/order_execution.py` & `volstreet-8.2.1/volstreet/trade_interface/order_execution.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.2.0/volstreet/trade_interface/underlyings.py` & `volstreet-8.2.1/volstreet/trade_interface/underlyings.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.2.0/volstreet/utils/change_config.py` & `volstreet-8.2.1/volstreet/utils/change_config.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.2.0/volstreet/utils/communication.py` & `volstreet-8.2.1/volstreet/utils/communication.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.2.0/volstreet/utils/core.py` & `volstreet-8.2.1/volstreet/utils/core.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.2.0/volstreet/utils/data_io.py` & `volstreet-8.2.1/volstreet/utils/data_io.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.2.0/volstreet/utils/scrip_processing.py` & `volstreet-8.2.1/volstreet/utils/scrip_processing.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.2.0/volstreet/vectorized_blackscholes.py` & `volstreet-8.2.1/volstreet/vectorized_blackscholes.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.2.0/volstreet/vslogging/formatters.py` & `volstreet-8.2.1/volstreet/vslogging/formatters.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.2.0/volstreet/vslogging/logging_config.json` & `volstreet-8.2.1/volstreet/vslogging/logging_config.json`

 * *Files identical despite different names*

### Comparing `volstreet-8.2.0/volstreet/vslogging/logging_setup.py` & `volstreet-8.2.1/volstreet/vslogging/logging_setup.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.2.0/volstreet/vslogging/parsing.py` & `volstreet-8.2.1/volstreet/vslogging/parsing.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.2.0/volstreet.egg-info/PKG-INFO` & `volstreet-8.2.1/volstreet.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: volstreet
-Version: 8.2.0
+Version: 8.2.1
 Summary: VolStreet is a Python library for automated trading
 Home-page: https://github.com/rahulthakkr/volstreet
 Author: Rahul Thakkar
 Author-email: r.thakkar15@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `volstreet-8.2.0/volstreet.egg-info/SOURCES.txt` & `volstreet-8.2.1/volstreet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

