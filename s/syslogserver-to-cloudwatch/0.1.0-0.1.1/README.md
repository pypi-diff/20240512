# Comparing `tmp/syslogserver_to_cloudwatch-0.1.0.tar.gz` & `tmp/syslogserver_to_cloudwatch-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syslogserver_to_cloudwatch-0.1.0.tar", max compression
+gzip compressed data, was "syslogserver_to_cloudwatch-0.1.1.tar", max compression
```

## Comparing `syslogserver_to_cloudwatch-0.1.0.tar` & `syslogserver_to_cloudwatch-0.1.1.tar`

### file list

```diff
@@ -1,4 +1,6 @@
--rw-r--r--   0        0        0      431 2024-05-10 04:02:33.826603 syslogserver_to_cloudwatch-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       30 2024-05-10 03:59:48.283566 syslogserver_to_cloudwatch-0.1.0/README.md
--rw-r--r--   0        0        0     2489 2024-05-10 05:02:21.058362 syslogserver_to_cloudwatch-0.1.0/syslogserver_to_cloudwatch/__main__.py
--rw-r--r--   0        0        0      462 1970-01-01 00:00:00.000000 syslogserver_to_cloudwatch-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      542 2024-05-12 15:30:02.437438 syslogserver_to_cloudwatch-0.1.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1070 2024-05-12 15:30:02.437438 syslogserver_to_cloudwatch-0.1.1/LICENSE
+-rw-r--r--   0        0        0       30 2024-05-12 15:30:02.441438 syslogserver_to_cloudwatch-0.1.1/README.md
+-rw-r--r--   0        0        0      586 2024-05-12 15:30:02.441438 syslogserver_to_cloudwatch-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2490 2024-05-12 15:30:02.441438 syslogserver_to_cloudwatch-0.1.1/syslogserver_to_cloudwatch/__main__.py
+-rw-r--r--   0        0        0      698 1970-01-01 00:00:00.000000 syslogserver_to_cloudwatch-0.1.1/PKG-INFO
```

### Comparing `syslogserver_to_cloudwatch-0.1.0/syslogserver_to_cloudwatch/__main__.py` & `syslogserver_to_cloudwatch-0.1.1/syslogserver_to_cloudwatch/__main__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 import asyncio
-from datetime import datetime, timezone
-from functools import cache, partial
 import os
 import sys
 import time
+from datetime import datetime, timezone
+from functools import partial
 from operator import itemgetter
 
 import boto3
 
 cloudwatch_logs = boto3.client("logs")
 BULK_MESSAGES = 1000
 PORT = int(os.getenv("PORT", "5140"))
 CLOUDWATCH_LOG_GROUP = os.getenv("CLOUDWATCH_LOG_GROUP")
-CLOUDWATCH_LOG_STREAM = f"syslogserver-to-cloudwatch/{datetime.now(timezone.utc):%Y-%m-%d-%H-%M-%S}"
+CLOUDWATCH_LOG_STREAM = (
+    f"syslogserver-to-cloudwatch/{datetime.now(timezone.utc):%Y-%m-%d-%H-%M-%S}"
+)
 
 if CLOUDWATCH_LOG_GROUP is None:
     print(
         "CLOUDWATCH_LOG_GROUP environment variable not set, could not start server",
         file=sys.stderr,
     )
     sys.exit(1)
```

