# Comparing `tmp/mtbase-4.8.202309011515-py3-none-any.whl.zip` & `tmp/mtbase-4.9.202309220816-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,80 +1,66 @@
-Zip file size: 121713 bytes, number of entries: 78
--rw-r--r--  2.0 unx     2172 b- defN 23-May-09 19:51 mt/aio/__init__.py
--rw-r--r--  2.0 unx     4130 b- defN 23-May-09 19:51 mt/aio/base.py
--rw-rw-r--  2.0 unx    12618 b- defN 23-Apr-02 05:53 mt/aio/files.py
--rw-rw-r--  2.0 unx     8978 b- defN 23-Apr-02 05:53 mt/aio/multiprocessing.py
--rw-rw-r--  2.0 unx     9873 b- defN 23-Apr-02 05:53 mt/aio/path.py
--rw-rw-r--  2.0 unx     3323 b- defN 23-Apr-02 05:53 mt/aio/procedure.py
--rw-r--r--  2.0 unx     1659 b- defN 23-May-09 19:51 mt/base/__init__.py
--rw-r--r--  2.0 unx      221 b- defN 23-Aug-16 10:05 mt/base/aio.py
--rw-rw-r--  2.0 unx    16034 b- defN 23-Apr-02 05:53 mt/base/bg_invoke.py
--rw-rw-r--  2.0 unx     2471 b- defN 23-Apr-02 05:53 mt/base/casting.py
--rw-r--r--  2.0 unx      259 b- defN 23-Aug-16 10:05 mt/base/concurrency.py
--rw-rw-r--  2.0 unx      165 b- defN 23-Apr-02 05:53 mt/base/const.py
--rw-rw-r--  2.0 unx      245 b- defN 23-Apr-02 05:53 mt/base/contextlib.py
--rw-rw-r--  2.0 unx    30365 b- defN 23-Apr-02 05:53 mt/base/dataframe_processing.py
--rw-rw-r--  2.0 unx      885 b- defN 23-Apr-02 05:53 mt/base/datatype.py
--rw-rw-r--  2.0 unx     5676 b- defN 23-Apr-02 05:53 mt/base/debug_process.py
--rw-rw-r--  2.0 unx     6863 b- defN 23-Apr-02 05:53 mt/base/deprecated.py
--rw-r--r--  2.0 unx     1786 b- defN 23-May-09 19:51 mt/base/exec.py
--rw-rw-r--  2.0 unx     2655 b- defN 23-Apr-02 05:53 mt/base/filetype.py
--rw-rw-r--  2.0 unx     1810 b- defN 23-Apr-02 05:53 mt/base/functional.py
--rw-rw-r--  2.0 unx      444 b- defN 23-Apr-02 05:53 mt/base/hashing.py
--rw-rw-r--  2.0 unx     6323 b- defN 23-Apr-02 05:53 mt/base/http.py
--rw-rw-r--  2.0 unx     5322 b- defN 23-Apr-02 05:53 mt/base/locket.py
--rw-rw-r--  2.0 unx      187 b- defN 23-Apr-02 05:53 mt/base/logging.py
--rw-rw-r--  2.0 unx       80 b- defN 23-Apr-02 05:53 mt/base/net.py
--rw-rw-r--  2.0 unx     7783 b- defN 23-Apr-02 05:53 mt/base/object_store.py
--rw-rw-r--  2.0 unx      147 b- defN 23-Apr-02 05:53 mt/base/path.py
--rw-r--r--  2.0 unx      613 b- defN 23-Aug-22 15:11 mt/base/pyximportcpp.py
--rw-r--r--  2.0 unx    19519 b- defN 23-Aug-16 10:05 mt/base/s3.py
--rw-rw-r--  2.0 unx    11810 b- defN 23-Apr-02 05:53 mt/base/s3transfer.py
--rw-rw-r--  2.0 unx     3363 b- defN 23-Apr-02 05:53 mt/base/str.py
--rw-rw-r--  2.0 unx      104 b- defN 23-Apr-02 05:53 mt/base/terminal.py
--rw-rw-r--  2.0 unx      110 b- defN 23-Apr-02 05:53 mt/base/threading.py
--rw-rw-r--  2.0 unx       86 b- defN 23-Apr-02 05:53 mt/base/traceback.py
--rw-r--r--  2.0 unx      396 b- defN 23-Sep-01 15:15 mt/base/version.py
--rw-rw-r--  2.0 unx      547 b- defN 23-Apr-02 05:53 mt/base/with_utils.py
--rw-rw-r--  2.0 unx     1765 b- defN 23-Apr-02 05:53 mt/base/zipfile.py
--rw-rw-r--  2.0 unx      124 b- defN 23-Apr-02 05:53 mt/base/concurrency/__init__.py
--rw-rw-r--  2.0 unx    15628 b- defN 23-Apr-02 05:53 mt/base/concurrency/aio.py
--rw-rw-r--  2.0 unx     2408 b- defN 23-Apr-02 05:53 mt/base/concurrency/base.py
--rw-rw-r--  2.0 unx    41884 b- defN 23-Apr-02 05:53 mt/base/concurrency/beehive.py
--rw-rw-r--  2.0 unx    18240 b- defN 23-Apr-02 05:53 mt/base/concurrency/multiprocessing.py
--rw-r--r--  2.0 unx      411 b- defN 23-Aug-16 10:05 mt/concurrency/__init__.py
--rw-r--r--  2.0 unx    15560 b- defN 23-Aug-16 10:05 mt/concurrency/aio.py
--rw-r--r--  2.0 unx     2442 b- defN 23-Aug-16 10:05 mt/concurrency/base.py
--rw-r--r--  2.0 unx    41913 b- defN 23-Aug-16 10:05 mt/concurrency/beehive.py
--rw-r--r--  2.0 unx    19267 b- defN 23-Aug-16 10:05 mt/concurrency/multiprocessing.py
--rw-rw-r--  2.0 unx      804 b- defN 23-Apr-02 05:53 mt/ctx/__init__.py
--rw-rw-r--  2.0 unx      901 b- defN 23-Apr-02 05:53 mt/jax/__init__.py
--rw-rw-r--  2.0 unx      847 b- defN 23-Apr-02 05:53 mt/jnp/__init__.py
--rw-rw-r--  2.0 unx      847 b- defN 23-Apr-02 05:53 mt/jsp/__init__.py
--rw-r--r--  2.0 unx    20596 b- defN 23-May-09 19:51 mt/logg/__init__.py
--rw-rw-r--  2.0 unx     3847 b- defN 23-Apr-02 05:53 mt/logging/__init__.py
--rw-rw-r--  2.0 unx      679 b- defN 23-Apr-02 05:53 mt/mpl/__init__.py
--rw-rw-r--  2.0 unx      539 b- defN 23-Apr-02 05:53 mt/net/__init__.py
--rw-rw-r--  2.0 unx     2986 b- defN 23-Apr-02 05:53 mt/net/base.py
--rw-rw-r--  2.0 unx     5102 b- defN 23-Apr-02 05:53 mt/net/host_port.py
--rw-rw-r--  2.0 unx    10611 b- defN 23-Apr-02 05:53 mt/net/port_forwarding.py
--rw-rw-r--  2.0 unx     9630 b- defN 23-Apr-02 06:17 mt/net/port_forwarding_async.py
--rw-rw-r--  2.0 unx     5483 b- defN 23-Apr-02 05:53 mt/net/ssh_forwarding.py
--rw-r--r--  2.0 unx     1000 b- defN 23-Aug-16 10:05 mt/np/__init__.py
--rw-rw-r--  2.0 unx     1953 b- defN 23-Apr-02 05:53 mt/np/image.py
--rw-rw-r--  2.0 unx     1660 b- defN 23-Apr-02 05:53 mt/np/matrix.py
--rw-r--r--  2.0 unx     2287 b- defN 23-Sep-01 15:15 mt/np/ndarray.py
--rw-rw-r--  2.0 unx     1402 b- defN 23-Apr-02 05:53 mt/np/sparse.py
--rw-rw-r--  2.0 unx     1513 b- defN 23-Apr-02 05:53 mt/path/__init__.py
--rw-rw-r--  2.0 unx      694 b- defN 23-Apr-02 05:53 mt/plt/__init__.py
--rw-rw-r--  2.0 unx      990 b- defN 23-Apr-02 05:53 mt/shutil/__init__.py
--rw-rw-r--  2.0 unx     4994 b- defN 23-Apr-02 05:53 mt/threading/__init__.py
--rw-rw-r--  2.0 unx     2158 b- defN 23-Apr-02 05:53 mt/time/__init__.py
--rw-rw-r--  2.0 unx      521 b- defN 23-Apr-02 05:53 mt/tp/__init__.py
--rw-rw-r--  2.0 unx     1043 b- defN 23-Apr-02 05:53 mt/traceback/__init__.py
--rwxrwxr-x  2.0 unx      690 b- defN 23-Sep-01 15:16 mtbase-4.8.202309011515.data/scripts/path_exists
--rw-rw-r--  2.0 unx     1070 b- defN 23-Sep-01 15:16 mtbase-4.8.202309011515.dist-info/LICENSE
--rw-r--r--  2.0 unx      697 b- defN 23-Sep-01 15:16 mtbase-4.8.202309011515.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Sep-01 15:16 mtbase-4.8.202309011515.dist-info/WHEEL
--rw-rw-r--  2.0 unx        3 b- defN 23-Sep-01 15:16 mtbase-4.8.202309011515.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     6079 b- defN 23-Sep-01 15:16 mtbase-4.8.202309011515.dist-info/RECORD
-78 files, 420382 bytes uncompressed, 112345 bytes compressed:  73.3%
+Zip file size: 85180 bytes, number of entries: 64
+-rw-r--r--  2.0 unx     2172 b- defN 23-Apr-15 06:17 mt/aio/__init__.py
+-rw-r--r--  2.0 unx     4130 b- defN 23-Apr-15 06:17 mt/aio/base.py
+-rw-r--r--  2.0 unx    12618 b- defN 23-Jan-22 22:24 mt/aio/files.py
+-rw-r--r--  2.0 unx     8978 b- defN 23-Jan-22 22:24 mt/aio/multiprocessing.py
+-rw-r--r--  2.0 unx     9873 b- defN 23-Jan-24 17:12 mt/aio/path.py
+-rw-r--r--  2.0 unx     3323 b- defN 23-Jan-22 22:24 mt/aio/procedure.py
+-rw-r--r--  2.0 unx     1659 b- defN 23-Apr-15 06:08 mt/base/__init__.py
+-rw-r--r--  2.0 unx      221 b- defN 23-May-24 06:11 mt/base/aio.py
+-rw-r--r--  2.0 unx    16034 b- defN 23-Jan-22 22:24 mt/base/bg_invoke.py
+-rw-r--r--  2.0 unx     2471 b- defN 23-Jan-22 22:24 mt/base/casting.py
+-rw-r--r--  2.0 unx      259 b- defN 23-May-24 09:39 mt/base/concurrency.py
+-rw-r--r--  2.0 unx      165 b- defN 23-Jan-22 22:24 mt/base/const.py
+-rw-r--r--  2.0 unx      245 b- defN 23-Jan-22 22:24 mt/base/contextlib.py
+-rw-r--r--  2.0 unx      885 b- defN 23-Feb-26 09:07 mt/base/datatype.py
+-rw-r--r--  2.0 unx     5676 b- defN 23-Jan-22 22:24 mt/base/debug_process.py
+-rw-r--r--  2.0 unx     6863 b- defN 23-Jan-22 22:24 mt/base/deprecated.py
+-rw-r--r--  2.0 unx     1786 b- defN 23-Apr-15 06:08 mt/base/exec.py
+-rw-r--r--  2.0 unx     2633 b- defN 23-Sep-21 18:06 mt/base/filetype.py
+-rw-r--r--  2.0 unx     1810 b- defN 23-Jan-22 22:24 mt/base/functional.py
+-rw-r--r--  2.0 unx      444 b- defN 23-Jan-22 22:24 mt/base/hashing.py
+-rw-r--r--  2.0 unx     6323 b- defN 23-Mar-19 21:04 mt/base/http.py
+-rw-r--r--  2.0 unx     5322 b- defN 23-Jan-22 22:24 mt/base/locket.py
+-rw-r--r--  2.0 unx      187 b- defN 23-Jan-22 22:24 mt/base/logging.py
+-rw-r--r--  2.0 unx     7783 b- defN 23-Jan-22 22:24 mt/base/object_store.py
+-rw-r--r--  2.0 unx      147 b- defN 23-Jan-22 22:24 mt/base/path.py
+-rw-r--r--  2.0 unx      613 b- defN 23-Sep-13 05:15 mt/base/pyximportcpp.py
+-rw-r--r--  2.0 unx    19519 b- defN 23-Aug-03 05:38 mt/base/s3.py
+-rw-r--r--  2.0 unx    11810 b- defN 23-Feb-15 12:15 mt/base/s3transfer.py
+-rw-r--r--  2.0 unx     3363 b- defN 23-Jan-22 22:24 mt/base/str.py
+-rw-r--r--  2.0 unx      104 b- defN 23-Jan-22 22:24 mt/base/terminal.py
+-rw-r--r--  2.0 unx      110 b- defN 23-Jan-22 22:24 mt/base/threading.py
+-rw-r--r--  2.0 unx       86 b- defN 23-Jan-22 22:24 mt/base/traceback.py
+-rw-r--r--  2.0 unx      396 b- defN 23-Sep-22 08:16 mt/base/version.py
+-rw-r--r--  2.0 unx      547 b- defN 23-Jan-22 22:24 mt/base/with_utils.py
+-rw-r--r--  2.0 unx     1765 b- defN 23-Jan-22 22:24 mt/base/zipfile.py
+-rw-r--r--  2.0 unx      428 b- defN 23-Sep-22 07:18 mt/concurrency/__init__.py
+-rw-r--r--  2.0 unx    21386 b- defN 23-Sep-22 08:15 mt/concurrency/aio.py
+-rw-r--r--  2.0 unx     2442 b- defN 23-May-24 09:33 mt/concurrency/base.py
+-rw-r--r--  2.0 unx    41913 b- defN 23-Jun-08 19:34 mt/concurrency/beehive.py
+-rw-r--r--  2.0 unx    19267 b- defN 23-May-24 09:40 mt/concurrency/multiprocessing.py
+-rw-r--r--  2.0 unx      804 b- defN 23-Jan-22 22:24 mt/ctx/__init__.py
+-rw-r--r--  2.0 unx      901 b- defN 23-Mar-01 10:58 mt/jax/__init__.py
+-rw-r--r--  2.0 unx      847 b- defN 23-Mar-01 10:58 mt/jnp/__init__.py
+-rw-r--r--  2.0 unx      847 b- defN 23-Mar-01 10:58 mt/jsp/__init__.py
+-rw-r--r--  2.0 unx    20596 b- defN 23-Apr-15 05:57 mt/logg/__init__.py
+-rw-r--r--  2.0 unx      679 b- defN 23-Jan-24 17:12 mt/mpl/__init__.py
+-rw-r--r--  2.0 unx     1000 b- defN 23-Aug-03 05:57 mt/np/__init__.py
+-rw-r--r--  2.0 unx     1953 b- defN 23-Jan-28 08:03 mt/np/image.py
+-rw-r--r--  2.0 unx     1660 b- defN 23-Jan-28 08:04 mt/np/matrix.py
+-rw-r--r--  2.0 unx     2287 b- defN 23-Sep-13 05:15 mt/np/ndarray.py
+-rw-r--r--  2.0 unx     1402 b- defN 23-Jan-28 08:03 mt/np/sparse.py
+-rw-r--r--  2.0 unx     1513 b- defN 23-Jan-22 22:24 mt/path/__init__.py
+-rw-r--r--  2.0 unx      694 b- defN 23-Jan-24 17:12 mt/plt/__init__.py
+-rw-r--r--  2.0 unx      990 b- defN 23-Jan-22 22:24 mt/shutil/__init__.py
+-rw-r--r--  2.0 unx     4994 b- defN 23-Jan-22 22:24 mt/threading/__init__.py
+-rw-r--r--  2.0 unx     2158 b- defN 23-Jan-22 22:24 mt/time/__init__.py
+-rw-r--r--  2.0 unx      521 b- defN 23-Jan-24 17:12 mt/tp/__init__.py
+-rw-r--r--  2.0 unx     1043 b- defN 23-Jan-22 22:24 mt/traceback/__init__.py
+-rwxr-xr-x  2.0 unx      690 b- defN 23-Sep-22 08:19 mtbase-4.9.202309220816.data/scripts/path_exists
+-rw-r--r--  2.0 unx     1070 b- defN 23-Sep-22 08:19 mtbase-4.9.202309220816.dist-info/LICENSE
+-rw-r--r--  2.0 unx      697 b- defN 23-Sep-22 08:19 mtbase-4.9.202309220816.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Sep-22 08:19 mtbase-4.9.202309220816.dist-info/WHEEL
+-rw-r--r--  2.0 unx        3 b- defN 23-Sep-22 08:19 mtbase-4.9.202309220816.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     4930 b- defN 23-Sep-22 08:19 mtbase-4.9.202309220816.dist-info/RECORD
+64 files, 278127 bytes uncompressed, 77576 bytes compressed:  72.1%
```

## zipnote {}

```diff
@@ -33,17 +33,14 @@
 
 Filename: mt/base/const.py
 Comment: 
 
 Filename: mt/base/contextlib.py
 Comment: 
 
-Filename: mt/base/dataframe_processing.py
-Comment: 
-
 Filename: mt/base/datatype.py
 Comment: 
 
 Filename: mt/base/debug_process.py
 Comment: 
 
 Filename: mt/base/deprecated.py
@@ -66,17 +63,14 @@
 
 Filename: mt/base/locket.py
 Comment: 
 
 Filename: mt/base/logging.py
 Comment: 
 
-Filename: mt/base/net.py
-Comment: 
-
 Filename: mt/base/object_store.py
 Comment: 
 
 Filename: mt/base/path.py
 Comment: 
 
 Filename: mt/base/pyximportcpp.py
@@ -105,29 +99,14 @@
 
 Filename: mt/base/with_utils.py
 Comment: 
 
 Filename: mt/base/zipfile.py
 Comment: 
 
-Filename: mt/base/concurrency/__init__.py
-Comment: 
-
-Filename: mt/base/concurrency/aio.py
-Comment: 
-
-Filename: mt/base/concurrency/base.py
-Comment: 
-
-Filename: mt/base/concurrency/beehive.py
-Comment: 
-
-Filename: mt/base/concurrency/multiprocessing.py
-Comment: 
-
 Filename: mt/concurrency/__init__.py
 Comment: 
 
 Filename: mt/concurrency/aio.py
 Comment: 
 
 Filename: mt/concurrency/base.py
@@ -150,38 +129,17 @@
 
 Filename: mt/jsp/__init__.py
 Comment: 
 
 Filename: mt/logg/__init__.py
 Comment: 
 
-Filename: mt/logging/__init__.py
-Comment: 
-
 Filename: mt/mpl/__init__.py
 Comment: 
 
-Filename: mt/net/__init__.py
-Comment: 
-
-Filename: mt/net/base.py
-Comment: 
-
-Filename: mt/net/host_port.py
-Comment: 
-
-Filename: mt/net/port_forwarding.py
-Comment: 
-
-Filename: mt/net/port_forwarding_async.py
-Comment: 
-
-Filename: mt/net/ssh_forwarding.py
-Comment: 
-
 Filename: mt/np/__init__.py
 Comment: 
 
 Filename: mt/np/image.py
 Comment: 
 
 Filename: mt/np/matrix.py
@@ -210,26 +168,26 @@
 
 Filename: mt/tp/__init__.py
 Comment: 
 
 Filename: mt/traceback/__init__.py
 Comment: 
 
-Filename: mtbase-4.8.202309011515.data/scripts/path_exists
+Filename: mtbase-4.9.202309220816.data/scripts/path_exists
 Comment: 
 
-Filename: mtbase-4.8.202309011515.dist-info/LICENSE
+Filename: mtbase-4.9.202309220816.dist-info/LICENSE
 Comment: 
 
-Filename: mtbase-4.8.202309011515.dist-info/METADATA
+Filename: mtbase-4.9.202309220816.dist-info/METADATA
 Comment: 
 
-Filename: mtbase-4.8.202309011515.dist-info/WHEEL
+Filename: mtbase-4.9.202309220816.dist-info/WHEEL
 Comment: 
 
-Filename: mtbase-4.8.202309011515.dist-info/top_level.txt
+Filename: mtbase-4.9.202309220816.dist-info/top_level.txt
 Comment: 
 
-Filename: mtbase-4.8.202309011515.dist-info/RECORD
+Filename: mtbase-4.9.202309220816.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mt/base/filetype.py

```diff
@@ -1,15 +1,14 @@
 """Extra subroutines using package 'filetype' asynchronously."""
 
 
-import aiofiles
 from filetype import *
 import filetype
 
-from mt.aio import srun, read_binary
+from mt.aio import read_binary
 
 
 __all__ = ["read_file_header", "is_image_asyn", "image_match_asyn"]
 
 
 async def read_file_header(filepath, context_vars: dict = {}):
     """An asyn function that reads the file header so :module:`filetype` can work on.
```

## mt/base/version.py

```diff
@@ -1,11 +1,11 @@
 VERSION_YEAR = 2023
 VERSION_MONTH = int('09')
-VERSION_DAY = int('01')
-VERSION_HOUR = int('15')
-VERSION_MINUTE = int('15')
+VERSION_DAY = int('22')
+VERSION_HOUR = int('08')
+VERSION_MINUTE = int('16')
 MAJOR_VERSION = 4
-MINOR_VERSION = 8
-PATCH_VERSION = 202309011515
-version_date = '2023/09/01 15:15'
+MINOR_VERSION = 9
+PATCH_VERSION = 202309220816
+version_date = '2023/09/22 08:16'
 version = '{}.{}.{}'.format(MAJOR_VERSION, MINOR_VERSION, PATCH_VERSION)
 __all__  = ['MAJOR_VERSION', 'MINOR_VERSION', 'PATCH_VERSION', 'version_date', 'version']
```

## mt/concurrency/__init__.py

```diff
@@ -13,8 +13,9 @@
     "serial_work_generator",
     "aio_work_generator",
     "run_asyn_works_in_context",
     "asyn_work_generator",
     "worker_process",
     "ProcessParalleliser",
     "WorkIterator",
+    "asyn_pmap",
 ]
```

## mt/concurrency/aio.py

```diff
@@ -1,12 +1,14 @@
 """Concurrency using asyncio and multiprocessing."""
 
+import typing as tp
 import asyncio
-import multiprocessing as _mp
+import multiprocessing as mp
 import queue as _q
+import itertools
 
 from .base import split_works
 
 
 async def aio_work_generator(
     func,
     num_work_ids,
@@ -75,15 +77,15 @@
                     raise e
                 result = done_task.result()
                 if not skip_null or result is not None:
                     yield result
 
 
 async def run_asyn_works_in_context(
-    progress_queue: _mp.Queue,
+    progress_queue: mp.Queue,
     func,
     func_args: tuple = (),
     func_kwargs: dict = {},
     context_id=None,
     work_id_list: list = [],
     max_concurrency: int = 1024,
     context_vars: dict = {},
@@ -189,15 +191,15 @@
                         )
                     else:
                         task = asyncio.ensure_future(
                             func(
                                 work_id,
                                 *func_args,
                                 context_vars=context_vars,
-                                **func_kwargs
+                                **func_kwargs,
                             )
                         )
                         progress_queue.put_nowait(
                             (context_id, "task_scheduled", work_id)
                         )
                         cur_task_map[task] = work_id
                 cur_pos += spare
@@ -272,21 +274,21 @@
     https://bugs.python.org/issue42683
     """
 
     if num_works <= 0:
         return
 
     # for communicating between processes
-    queue = _mp.Queue() if progress_queue is None else progress_queue
+    queue = mp.Queue() if progress_queue is None else progress_queue
 
-    num_buckets = _mp.cpu_count() if num_processes is None else num_processes
+    num_buckets = mp.cpu_count() if num_processes is None else num_processes
     work_id_list_list = split_works(num_works, num_buckets)
 
     def worker_process(
-        progress_queue: _mp.Queue,
+        progress_queue: mp.Queue,
         func,
         func_args: tuple = (),
         func_kwargs: dict = {},
         context_id=None,
         work_id_list: list = [],
         max_concurrency: int = 1024,
         profile=None,
@@ -331,15 +333,15 @@
                 (context_id, "context_raised", e, extract_stack_compact())
             )
         progress_queue.put_nowait((context_id, "context_destroyed"))
 
     # launch the concurrency suite
     process_list = []
     for context_id in range(num_buckets):
-        p = _mp.Process(
+        p = mp.Process(
             target=worker_process,
             args=(queue, func),
             kwargs={
                 "func_args": func_args,
                 "func_kwargs": func_kwargs,
                 "context_id": context_id,
                 "work_id_list": work_id_list_list[context_id],
@@ -393,7 +395,171 @@
         for p in process_list:
             p.terminate()  # ouch!
 
     if keyboard_interrupted:
         raise KeyboardInterrupt(
             "Keyboard interrupted while asyn_work_generator() is running."
         )
+
+
+def batched(iterable, n):
+    "Batch data into tuples of length n. The last batch may be shorter."
+    # batched('ABCDEFG', 3) --> ABC DEF G
+    if n < 1:
+        raise ValueError("n must be at least one")
+    it = iter(iterable)
+    while batch := tuple(itertools.islice(it, n)):
+        yield batch
+
+
+def unbatched(iterable):
+    "Unbatch tuples of data into just data."
+    for x in iterable:
+        for y in x:
+            yield y
+
+
+def pool_initializer(
+    pool_func: tp.Callable,
+    asyn_func: tp.Callable,
+    asyn_func_args: tuple = (),
+    asyn_func_kwargs: dict = {},
+    init_func: tp.Optional[tp.Callable] = None,
+    init_func_args: tuple = (),
+    init_func_kwargs: dict = {},
+    cvc_func: tp.Optional[tp.Callable] = None,
+    cvc_func_args: tuple = (),
+    cvc_func_kwargs: dict = {},
+):
+    pool_func.asyn_func = asyn_func
+    pool_func.asyn_func_args = asyn_func_args
+    pool_func.asyn_func_kwargs = asyn_func_kwargs
+
+    if init_func is not None:
+        init_func(*init_func_args, **init_func_kwargs)
+
+    import asyncio
+
+    pool_func.asyncio = asyncio
+    if cvc_func is not None:
+        pool_func.context_vars = cvc_func(*cvc_func_args, **cvc_func_kwargs)
+    else:
+        pool_func.context_vars = {"async": True}
+
+
+def pool_func(
+    t_items: tuple,
+):
+    async def func(t_items: tuple):
+        l_outputs = []
+        for item in t_items:
+            output = await pool_func.asyn_func(
+                item,
+                *pool_func.asyn_func_args,
+                context_vars=pool_func.context_vars,
+                **pool_func.asyn_func_kwargs,
+            )
+            l_outputs.append(output)
+
+        return l_outputs
+
+    return asyncio.run(func(t_items))
+
+
+def asyn_pmap(
+    asyn_func: tp.Callable,
+    input_iterable: tp.Iterable,
+    batch_size: int = 1024,
+    asyn_func_args: tuple = (),
+    asyn_func_kwargs: dict = {},
+    pool_processes: tp.Optional[int] = None,
+    pool_maxtasksperchild: tp.Optional[int] = None,
+    pool_ordered: bool = True,
+    init_func: tp.Optional[tp.Callable] = None,
+    init_func_args: tuple = (),
+    init_func_kwargs: dict = {},
+    cvc_func: tp.Optional[tp.Callable] = None,
+    cvc_func_args: tuple = (),
+    cvc_func_kwargs: dict = {},
+) -> tp.Iterable:
+    """pmap over an iterator with an asyn function.
+
+    Internally, the iterator is batched into a batch iterator. Each batch is sent to one worker for
+    processing. The worker goes through every item of a batch and invokes asyn function `asyn_func`
+    providing the `context_vars` dictionary. Each batch of results is then unbatched. The output
+    iterator yield resultant items, which may or may not in order depending on the `pool_ordered`
+    argument.
+
+    Parameters
+    ----------
+    asyn_func : function
+        an asyn function that returns something. The first positional argument of function is the
+        item to be processed. The keyword argument 'context_vars' is provided to the function.
+    input_iterable : iterable
+        any iterable object to act as the input iterator
+    batch_size : int
+        number of batch items in each batch. It should be chosen by the user to balance between the
+        benefit of iterating over the items of a batch in async mode and the cost of allocated
+        memory to store pending transformed items of the batch
+    asyn_func_args : tuple, optional
+        additional positional arguments to be passed to the asyn function as-is
+    asyn_func_kwargs : dict, optional
+        additional keyword arguments to be passed to the asyn function as-is
+    pool_processes : int, optional
+        the number of processes to be created. If not specified, it is equal to the number of CPUs.
+        Passed as-is to :class:`multiprocessing.Pool`.
+    pool_maxtasksperchild : int, optional
+        the number of tasks a worker process can complete before it will exit and be replaced with
+        a fresh worker process, to enable unused resources to be freed. The default
+        `maxtasksperchild` is None, which means worker processes will live as long as the pool.
+        Passed as-is to :class:`multiprocessing.Pool`.
+    pool_ordered : bool
+        whether the output iterator provides the same order as the input iterator or not
+    init_func : function, optional
+        a function returning None that is invoked after a worker process is created
+    init_func_args : tuple, optional
+        additional positional arguments to be passed to the init function as-is
+    init_func_kwargs : dict, optional
+        additional keyword arguments to be passed to the init function as-is
+    cvc_func : function, optional
+        a function returning the `context_vars` dictionary to be provided to the asyn function as a
+        keyword argument. If not provided, `context_vars={"async": True}`.
+    cvc_func_args : tuple, optional
+        additional positional arguments to be passed to the cvc function as-is
+    cvc_func_kwargs : dict, optional
+        additional keyword arguments to be passed to the cvc function as-is
+
+    Returns
+    -------
+    output_iterable : iterable
+        the output iterator
+    """
+
+    iterable = batched(input_iterable, batch_size)
+
+    initargs = (
+        pool_func,
+        asyn_func,
+        asyn_func_args,
+        asyn_func_kwargs,
+        init_func,
+        init_func_args,
+        init_func_kwargs,
+        cvc_func,
+        cvc_func_args,
+        cvc_func_kwargs,
+    )
+    pool = mp.Pool(
+        processes=pool_processes,
+        initializer=pool_initializer,
+        initargs=initargs,
+        maxtasksperchild=pool_maxtasksperchild,
+    )
+
+    if pool_ordered:
+        iterable = pool.imap(pool_func, iterable)
+    else:
+        iterable = pool.imap_unordered(pool_func, iterable)
+
+    output_iterable = unbatched(iterable)
+
+    return output_iterable
```

## Comparing `mtbase-4.8.202309011515.data/scripts/path_exists` & `mtbase-4.9.202309220816.data/scripts/path_exists`

 * *Files identical despite different names*

## Comparing `mtbase-4.8.202309011515.dist-info/LICENSE` & `mtbase-4.9.202309220816.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mtbase-4.8.202309011515.dist-info/METADATA` & `mtbase-4.9.202309220816.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mtbase
-Version: 4.8.202309011515
+Version: 4.9.202309220816
 Summary: The most fundamental Python modules for Minh-Tri Pham
 Home-page: https://github.com/inteplus/mtbase
 Author: ['Minh-Tri Pham']
 Project-URL: Documentation, https://mtdoc.readthedocs.io/en/latest/mt.base/mt.base.html
 Project-URL: Source Code, https://github.com/inteplus/mtbase
 Requires-Python: >=3.6
 License-File: LICENSE
```

## Comparing `mtbase-4.8.202309011515.dist-info/RECORD` & `mtbase-4.9.202309220816.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -7,72 +7,58 @@
 mt/base/__init__.py,sha256=1LzDyZSIZrxAsfgYNRHSHLUlntv47uVQ4qNOzmGTV-o,1659
 mt/base/aio.py,sha256=d-nijaZ-saqowUK1bn7HBriw5CCl9yjn_6lfuF-O2l4,221
 mt/base/bg_invoke.py,sha256=NzFNMl8fbS26dod-gi0m1f-BlQworFzWtrOTCwFT_WQ,16034
 mt/base/casting.py,sha256=yHmHDzISEsarasHQXg6MmqNYuxt1Ab4MYj8Okh2-oN8,2471
 mt/base/concurrency.py,sha256=6jjrHDdO4KxAWYYTc_8gsJ3m0yn82LZnL78yIUYVDRU,259
 mt/base/const.py,sha256=ifyavLDbeEeeAHmfsu7VDhcVpi1UcMFUg6fYL6bMPPk,165
 mt/base/contextlib.py,sha256=F-7j3hDxeyZIutD7Q7xgRER8AQSpX7KtZFcU9JPKlk8,245
-mt/base/dataframe_processing.py,sha256=pTFIIALi9UpjpNNbMeudgmEJTQ3lPjC6os4UfHFttdc,30365
 mt/base/datatype.py,sha256=psLw2Aus9kk8gCv2orY6qzM2_QFmKJe1Kzf9zC2DURo,885
 mt/base/debug_process.py,sha256=0m0TkTsg8dMvHafdK4dcXliRZ8PeZeDcOtzWQEMA7HE,5676
 mt/base/deprecated.py,sha256=RGNXdAlxjrLQj4kCCI3qhxE8bUBjn1ZtZUfsbnGjQ5M,6863
 mt/base/exec.py,sha256=npgBV9memCutw9xBOQthwCS3Tj44TN_UqVqfldVWSNU,1786
-mt/base/filetype.py,sha256=LaBEhDARcISamnNjOv90X0_Z7M-ofmpXS5YHc3NNqO4,2655
+mt/base/filetype.py,sha256=rf-SpmkjtAgEZFIFFfGcwjPu12iuh0RzfvDCU7O28qM,2633
 mt/base/functional.py,sha256=je1agyP_iLcUg4p88OQDJP6byQbbKxppQgYav-hMhi4,1810
 mt/base/hashing.py,sha256=QhX1vlpxCtGZu1oQSZYXfvGE-uDf33Odpqqk9hvojZg,444
 mt/base/http.py,sha256=Wk3OAp7BzXiRxOTtiJY0tIr6VNi8_0yRClS0s0iYGuw,6323
 mt/base/locket.py,sha256=CL2syNTpWjEIGRE5aAb_iZBRHMJ2PNvEj9e88e3Ogeo,5322
 mt/base/logging.py,sha256=NA7LNsSj8A9v5VKlwAwOVUkM4xtPCxHwdyG2QM7pvJw,187
-mt/base/net.py,sha256=tnlqpDk5MDPjc_5Lf7NMxPw6AbZFgK4HkhssHmOzupY,80
 mt/base/object_store.py,sha256=oD6m2ZX7EVvlUq5JCK3TkSgCFVPYtNRvg9vf3DqB3JM,7783
 mt/base/path.py,sha256=f4Ej4-5KrxyyGlaMhTGDYltlv9Csvfqi3ANSBZhkjXI,147
 mt/base/pyximportcpp.py,sha256=XpdiNluVxsqbY1jL685lLsWcnf2ix3mDLeFL8NMz8B8,613
 mt/base/s3.py,sha256=hf1rxN8frXb1DhEAN0q3FdDEDX0_CZpglUIYGPEYAe4,19519
 mt/base/s3transfer.py,sha256=RVdh2qL_t-EsztILt87K8D1TcA8ZydJzZ-l3Sl0hV4U,11810
 mt/base/str.py,sha256=GdEv5lBns95hMovlWohtQGVI4bt-SmoONfKRJ5qtRvk,3363
 mt/base/terminal.py,sha256=_23Kk7oihgCbe2yjJw2SQrTCqymSi-drejn1SWIS6IY,104
 mt/base/threading.py,sha256=MTVjpaTg_sbZWCksoP_5iMVYFjjUxrgpYBMOWxFY4Ms,110
 mt/base/traceback.py,sha256=Zn4oNs_f4mleJakpSaCbpMNfMt4O0gQEQrA6oChixdk,86
-mt/base/version.py,sha256=s5vpjxyNRa1IHEtl8dgLA62klzpdTIMWB_GCtgCdBBY,396
+mt/base/version.py,sha256=VAphOZ1T3FRzhDJRg3cbts8QryBbk2B1BDRL6LNKHjg,396
 mt/base/with_utils.py,sha256=-7OAVtGjL1dy2bhJ0II8McJKaAG8yUWr_GhccxT15Z8,547
 mt/base/zipfile.py,sha256=SnsBCaPlPw300_mi7WYB6wSqjvW-U_g96vS2S9JwrnE,1765
-mt/base/concurrency/__init__.py,sha256=Ev2nE_flaHbtEaFXyNtHrKZip37jHqIJWUOziyEfqTU,124
-mt/base/concurrency/aio.py,sha256=m1NiDC7tHf4wntkbdTMq6syfzKoF_a9voISvJKRWY68,15628
-mt/base/concurrency/base.py,sha256=bHe8BuPm7elqBA3YDCDZHzswXLX3ILq6b6STd1S6zBo,2408
-mt/base/concurrency/beehive.py,sha256=IG7mw8eKjrGW7Im7JJWSWHrZEh1JUyffERqxgka5ErA,41884
-mt/base/concurrency/multiprocessing.py,sha256=uVGDvk2iwIKPjxAE5Pm-_BS14d79qxIaxwDIBwfHq2I,18240
-mt/concurrency/__init__.py,sha256=XxsRYuCXlM3fGNERLIHY0m9IrhQH06TqMVqPkOiIevU,411
-mt/concurrency/aio.py,sha256=BHTvp12wDpDUF4SariY_-d4SDazdSEeXy-1q8AP0_Yc,15560
+mt/concurrency/__init__.py,sha256=jF7NoWRKap-QhuJaJZ3EUpfrn2HaZa_8MAS0bT325AY,428
+mt/concurrency/aio.py,sha256=uHrEkb_vRc5SBrM84AU9GIx-1xfacZ5ai8XTNt2E3hY,21386
 mt/concurrency/base.py,sha256=psGzEzyoARWl97N5y0Hbhkjq8RnE-jkPoBK6u44PNEg,2442
 mt/concurrency/beehive.py,sha256=S6lqJMLKjgu45Tr-3zIO09AJ25l4JETvFwmfujo1YJk,41913
 mt/concurrency/multiprocessing.py,sha256=Ejnt_4y2V2_Nf34ZOpt1tE_rP2mJ8JbNWJXkESL7hQU,19267
 mt/ctx/__init__.py,sha256=7V7zNr6VGNVNOxLQGZhZVmAP_jCw7JeHr77oAIwK68A,804
 mt/jax/__init__.py,sha256=H8yaQTicZJirPJAIJ59dqyUlW9HKjtSFMVhm77-n_04,901
 mt/jnp/__init__.py,sha256=ffCUR9x3KOcoHWZRFNHxL56EvcR3D-Vq3ODLIDG6Orc,847
 mt/jsp/__init__.py,sha256=JWOoWzwT_4mGyklotUbtSg4Sx5Sr_C16Nd7AvxRnQ2o,847
 mt/logg/__init__.py,sha256=w43fyKjZzeXDY9XXLml1ixdg1KFXuh4-bWYX5LNGD24,20596
-mt/logging/__init__.py,sha256=a79fElTaZnELuwD8GFCH57zH2xtAui2lDnghBqyAUxY,3847
 mt/mpl/__init__.py,sha256=T0xg7jVS4Ix3LXnbi1hE_tod5LUMjkKpLRwEozdRRcE,679
-mt/net/__init__.py,sha256=0Oym71x8dvtGYo9Ol6UmJElW2RC0hAMPpR-jIrtoets,539
-mt/net/base.py,sha256=rakNfgstwB3RMtCuQerHYcYUe2n7zkd7dmsI9CKZa6Y,2986
-mt/net/host_port.py,sha256=pFhPYDdI7oHYQnIZ2cZdr46zKT4qtxfGMAQk36m7cXc,5102
-mt/net/port_forwarding.py,sha256=f5_4SZ8Io__N9RgcGsF-G-hn57zX2U3_xSxc0_u_89E,10611
-mt/net/port_forwarding_async.py,sha256=lPrUSz2-NIMNmMTO0_FeOsZ8ZNteXOhXJ1Ylnes0P2E,9630
-mt/net/ssh_forwarding.py,sha256=8_bQFayadHStqK0x1_qOFYF5M1hnBswz1oLVuuIxKSw,5483
 mt/np/__init__.py,sha256=IfnNfzCrjN7WTa0C1OoZEyStb4ok6TJ-uUdr-kMIX74,1000
 mt/np/image.py,sha256=ZB_pmJXpagOZmeKIlUePGIFy2pCaEwgU9rI53CUSubY,1953
 mt/np/matrix.py,sha256=RIzZ-9cYNzyHiKHqaMuzl_tQ4ZmgR8-C9ekE8bdJPmg,1660
 mt/np/ndarray.py,sha256=lScwY3b7vVWdP608_OpnT_-zcg7y_KQSbgNdFjQkrmQ,2287
 mt/np/sparse.py,sha256=xEdFVG1hDIqY2uvfy9ov5BqzRTPumNsMNP09bV4qkvo,1402
 mt/path/__init__.py,sha256=7sFKV5T0nDk9lWIHhDPiDqZtE3sazKfkBBMedJrb4RA,1513
 mt/plt/__init__.py,sha256=y1RQmfTCjOYOzeAvnbnwTzw89LKiquUj28_PpwKslFg,694
 mt/shutil/__init__.py,sha256=PW9_pxVH3EVdxETupRoFc5StyyS8A8LX1lRFGVr8I4A,990
 mt/threading/__init__.py,sha256=dE7YEfeBMyxJ1DzFox28r0e2CzsSMWtm2XCvyk_ewXg,4994
 mt/time/__init__.py,sha256=lAjC0En0X0spHTu2YC120AchNlv1SzHgQlX0RmXWLEc,2158
 mt/tp/__init__.py,sha256=9yEoip3w8V2X1a49APJDC8EqVlGoa3WpR3DNXBX-cKk,521
 mt/traceback/__init__.py,sha256=7_aNd4u_CXRgWlzgfz3x7BnWta4DoAqrFFrIAiEqjJI,1043
-mtbase-4.8.202309011515.data/scripts/path_exists,sha256=9rYAZNiVEeTTi-hKM8NkQVIZOaEQkWE_WVw72avfUDo,690
-mtbase-4.8.202309011515.dist-info/LICENSE,sha256=PojkRlQzTT5Eg6Nj03XoIVEefN3u8iiIFf1p4rqe_t4,1070
-mtbase-4.8.202309011515.dist-info/METADATA,sha256=3WPHUuEtHHGhd6-jSad9S5SFfOZqklNobXdQQfbmivk,697
-mtbase-4.8.202309011515.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-mtbase-4.8.202309011515.dist-info/top_level.txt,sha256=WcqGFu9cV7iMZg09iam8eNxUvGpLSKKF2Iubf6SJVOo,3
-mtbase-4.8.202309011515.dist-info/RECORD,,
+mtbase-4.9.202309220816.data/scripts/path_exists,sha256=9rYAZNiVEeTTi-hKM8NkQVIZOaEQkWE_WVw72avfUDo,690
+mtbase-4.9.202309220816.dist-info/LICENSE,sha256=PojkRlQzTT5Eg6Nj03XoIVEefN3u8iiIFf1p4rqe_t4,1070
+mtbase-4.9.202309220816.dist-info/METADATA,sha256=pGkRbMHBZrk-DsoCYzxvB5AZgH260b-lSH_4V5UOlxg,697
+mtbase-4.9.202309220816.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+mtbase-4.9.202309220816.dist-info/top_level.txt,sha256=WcqGFu9cV7iMZg09iam8eNxUvGpLSKKF2Iubf6SJVOo,3
+mtbase-4.9.202309220816.dist-info/RECORD,,
```

