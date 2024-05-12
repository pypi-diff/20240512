# Comparing `tmp/deepdog-1.2.0.tar.gz` & `tmp/deepdog-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepdog-1.2.0.tar", max compression
+gzip compressed data, was "deepdog-1.2.1.tar", max compression
```

## Comparing `deepdog-1.2.0.tar` & `deepdog-1.2.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0      366 2024-05-09 03:25:18.347863 deepdog-1.2.0/deepdog/__init__.py
--rw-r--r--   0        0        0        0 2024-05-09 03:25:18.347863 deepdog-1.2.0/deepdog/cli/__init__.py
--rw-r--r--   0        0        0       80 2024-05-09 03:25:18.347863 deepdog-1.2.0/deepdog/cli/probs/__init__.py
--rw-r--r--   0        0        0     1389 2024-05-09 03:25:18.347863 deepdog-1.2.0/deepdog/cli/probs/args.py
--rw-r--r--   0        0        0     6243 2024-05-09 03:25:18.347863 deepdog-1.2.0/deepdog/cli/probs/dicts.py
--rw-r--r--   0        0        0     2945 2024-05-09 03:25:18.347863 deepdog-1.2.0/deepdog/cli/probs/main.py
--rw-r--r--   0        0        0      161 2024-05-09 03:25:18.347863 deepdog-1.2.0/deepdog/direct_monte_carlo/__init__.py
--rw-r--r--   0        0        0      329 2024-05-09 03:25:59.053941 deepdog-1.2.0/deepdog/direct_monte_carlo/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     7897 2024-05-09 03:25:59.057942 deepdog-1.2.0/deepdog/direct_monte_carlo/__pycache__/direct_mc.cpython-39.pyc
--rw-r--r--   0        0        0     3902 2024-05-09 03:25:59.061942 deepdog-1.2.0/deepdog/direct_monte_carlo/__pycache__/dmc_filters.cpython-39.pyc
--rw-r--r--   0        0        0      461 2024-05-09 03:25:18.347863 deepdog-1.2.0/deepdog/direct_monte_carlo/compose_filter.py
--rw-r--r--   0        0        0     9338 2024-05-09 03:25:18.347863 deepdog-1.2.0/deepdog/direct_monte_carlo/direct_mc.py
--rw-r--r--   0        0        0     3393 2024-05-09 03:25:18.347863 deepdog-1.2.0/deepdog/direct_monte_carlo/dmc_filters.py
--rw-r--r--   0        0        0     1700 2024-05-09 03:25:18.347863 deepdog-1.2.0/deepdog/indexify/__init__.py
--rw-r--r--   0        0        0     2432 2024-05-09 03:25:59.109944 deepdog-1.2.0/deepdog/indexify/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0       73 2024-05-09 03:25:18.347863 deepdog-1.2.0/deepdog/meta.py
--rw-r--r--   0        0        0    12392 2024-05-09 03:25:18.351863 deepdog-1.2.0/deepdog/real_spectrum_run.py
--rw-r--r--   0        0        0     5732 2024-05-09 03:25:18.351863 deepdog-1.2.0/deepdog/results/__init__.py
--rw-r--r--   0        0        0     6896 2024-05-09 03:25:59.133946 deepdog-1.2.0/deepdog/results/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0      110 2024-05-09 03:25:18.351863 deepdog-1.2.0/deepdog/subset_simulation/__init__.py
--rw-r--r--   0        0        0    11428 2024-05-09 03:25:18.351863 deepdog-1.2.0/deepdog/subset_simulation/subset_simulation_impl.py
--rw-r--r--   0        0        0     6794 2024-05-09 03:25:18.351863 deepdog-1.2.0/deepdog/temp_aware_real_spectrum_run.py
--rw-r--r--   0        0        0     1084 2024-05-09 03:25:18.351863 deepdog-1.2.0/pyproject.toml
--rw-r--r--   0        0        0      398 1970-01-01 00:00:00.000000 deepdog-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0      366 2024-05-12 01:51:49.254232 deepdog-1.2.1/deepdog/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-12 01:51:49.254232 deepdog-1.2.1/deepdog/cli/__init__.py
+-rw-r--r--   0        0        0       80 2024-05-12 01:51:49.254232 deepdog-1.2.1/deepdog/cli/probs/__init__.py
+-rw-r--r--   0        0        0     1389 2024-05-12 01:51:49.254232 deepdog-1.2.1/deepdog/cli/probs/args.py
+-rw-r--r--   0        0        0     6243 2024-05-12 01:51:49.254232 deepdog-1.2.1/deepdog/cli/probs/dicts.py
+-rw-r--r--   0        0        0     2945 2024-05-12 01:51:49.254232 deepdog-1.2.1/deepdog/cli/probs/main.py
+-rw-r--r--   0        0        0      161 2024-05-12 01:51:49.258232 deepdog-1.2.1/deepdog/direct_monte_carlo/__init__.py
+-rw-r--r--   0        0        0      329 2024-05-12 01:52:16.423528 deepdog-1.2.1/deepdog/direct_monte_carlo/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     7897 2024-05-12 01:52:16.427528 deepdog-1.2.1/deepdog/direct_monte_carlo/__pycache__/direct_mc.cpython-39.pyc
+-rw-r--r--   0        0        0     3902 2024-05-12 01:52:16.435528 deepdog-1.2.1/deepdog/direct_monte_carlo/__pycache__/dmc_filters.cpython-39.pyc
+-rw-r--r--   0        0        0      461 2024-05-12 01:51:49.258232 deepdog-1.2.1/deepdog/direct_monte_carlo/compose_filter.py
+-rw-r--r--   0        0        0     9338 2024-05-12 01:51:49.258232 deepdog-1.2.1/deepdog/direct_monte_carlo/direct_mc.py
+-rw-r--r--   0        0        0     3393 2024-05-12 01:51:49.258232 deepdog-1.2.1/deepdog/direct_monte_carlo/dmc_filters.py
+-rw-r--r--   0        0        0     1710 2024-05-12 01:51:49.258232 deepdog-1.2.1/deepdog/indexify/__init__.py
+-rw-r--r--   0        0        0     2436 2024-05-12 01:52:16.511532 deepdog-1.2.1/deepdog/indexify/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0       73 2024-05-12 01:51:49.258232 deepdog-1.2.1/deepdog/meta.py
+-rw-r--r--   0        0        0    12392 2024-05-12 01:51:49.258232 deepdog-1.2.1/deepdog/real_spectrum_run.py
+-rw-r--r--   0        0        0     5869 2024-05-12 01:51:49.258232 deepdog-1.2.1/deepdog/results/__init__.py
+-rw-r--r--   0        0        0     7172 2024-05-12 01:52:16.539533 deepdog-1.2.1/deepdog/results/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0      110 2024-05-12 01:51:49.258232 deepdog-1.2.1/deepdog/subset_simulation/__init__.py
+-rw-r--r--   0        0        0    11428 2024-05-12 01:51:49.258232 deepdog-1.2.1/deepdog/subset_simulation/subset_simulation_impl.py
+-rw-r--r--   0        0        0     6794 2024-05-12 01:51:49.258232 deepdog-1.2.1/deepdog/temp_aware_real_spectrum_run.py
+-rw-r--r--   0        0        0     1084 2024-05-12 01:51:49.258232 deepdog-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0      398 1970-01-01 00:00:00.000000 deepdog-1.2.1/PKG-INFO
```

### Comparing `deepdog-1.2.0/deepdog/cli/probs/args.py` & `deepdog-1.2.1/deepdog/cli/probs/args.py`

 * *Files identical despite different names*

### Comparing `deepdog-1.2.0/deepdog/cli/probs/dicts.py` & `deepdog-1.2.1/deepdog/cli/probs/dicts.py`

 * *Files identical despite different names*

### Comparing `deepdog-1.2.0/deepdog/cli/probs/main.py` & `deepdog-1.2.1/deepdog/cli/probs/main.py`

 * *Files identical despite different names*

### Comparing `deepdog-1.2.0/deepdog/direct_monte_carlo/__pycache__/direct_mc.cpython-39.pyc` & `deepdog-1.2.1/deepdog/direct_monte_carlo/__pycache__/direct_mc.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu May  9 03:25:18 2024 UTC, .py size: 9338 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 1e42 3c66 7a24 0000  a........B<fz$..
+00000000: 610d 0d0a 0000 0000 b520 4066 7a24 0000  a........ @fz$..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 e400 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a02 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c03 5a02 6400 6401 6c04 5a02 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6401 6c05 5a02 6400 6401 6c06 5a06 6400  d.l.Z.d.d.l.Z.d.
 00000060: 6402 6c07 6d08 5a08 6d09 5a09 6d0a 5a0a  d.l.m.Z.m.Z.m.Z.
 00000070: 6d0b 5a0b 6d0c 5a0c 0100 6400 6403 6c0d  m.Z.m.Z...d.d.l.
@@ -34,15 +34,15 @@
 00000210: 7175 616c 6e61 6d65 5f5f da03 696e 74da  qualname__..int.
 00000220: 0f5f 5f61 6e6e 6f74 6174 696f 6e73 5f5f  .__annotations__
 00000230: da05 666c 6f61 74da 0373 7472 a900 7214  ..float..str..r.
 00000240: 0000 0072 1400 0000 fa61 2f68 6f6d 652f  ...r.....a/home/
 00000250: 6a65 6e6b 696e 732f 6167 656e 742f 776f  jenkins/agent/wo
 00000260: 726b 7370 6163 652f 6769 7465 612d 7068  rkspace/gitea-ph
 00000270: 7973 6963 735f 6465 6570 646f 675f 312e  ysics_deepdog_1.
-00000280: 322e 302f 6465 6570 646f 672f 6469 7265  2.0/deepdog/dire
+00000280: 322e 312f 6465 6570 646f 672f 6469 7265  2.1/deepdog/dire
 00000290: 6374 5f6d 6f6e 7465 5f63 6172 6c6f 2f64  ct_monte_carlo/d
 000002a0: 6972 6563 745f 6d63 2e70 7972 0800 0000  irect_mc.pyr....
 000002b0: 1400 0000 7308 0000 000a 0208 0108 0108  ....s...........
 000002c0: 0172 0800 0000 6300 0000 0000 0000 0000  .r....c.........
 000002d0: 0000 0000 0000 0003 0000 0040 0000 0073  ...........@...s
 000002e0: 8200 0000 6500 5a01 6400 5a02 5500 6401  ....e.Z.d.Z.U.d.
 000002f0: 5a03 6504 6505 6402 3c00 6403 5a06 6504  Z.e.e.d.<.d.Z.e.
```

### Comparing `deepdog-1.2.0/deepdog/direct_monte_carlo/__pycache__/dmc_filters.cpython-39.pyc` & `deepdog-1.2.1/deepdog/direct_monte_carlo/__pycache__/dmc_filters.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu May  9 03:25:18 2024 UTC, .py size: 3393 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 1e42 3c66 410d 0000  a........B<fA...
+00000000: 610d 0d0a 0000 0000 b520 4066 410d 0000  a........ @fA...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 8000 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c06 5a07 6400 6404 6c08  ..d.d.l.Z.d.d.l.
 00000060: 5a07 6400 6404 6c09 5a07 6400 6404 6c0a  Z.d.d.l.Z.d.d.l.
 00000070: 5a07 6400 6404 6c00 5a00 4700 6405 6406  Z.d.d.l.Z.G.d.d.
@@ -31,15 +31,15 @@
 000001e0: 0000 0073 1800 0000 6700 7c00 5d10 7d01  ...s....g.|.].}.
 000001f0: 7c01 6a00 7c01 6a01 6602 9102 7104 5300  |.j.|.j.f...q.S.
 00000200: a900 a902 da01 72da 0166 a902 da02 2e30  ......r..f.....0
 00000210: da07 6d65 6173 7572 6572 0800 0000 7208  ..measurer....r.
 00000220: 0000 00fa 632f 686f 6d65 2f6a 656e 6b69  ....c/home/jenki
 00000230: 6e73 2f61 6765 6e74 2f77 6f72 6b73 7061  ns/agent/workspa
 00000240: 6365 2f67 6974 6561 2d70 6879 7369 6373  ce/gitea-physics
-00000250: 5f64 6565 7064 6f67 5f31 2e32 2e30 2f64  _deepdog_1.2.0/d
+00000250: 5f64 6565 7064 6f67 5f31 2e32 2e31 2f64  _deepdog_1.2.1/d
 00000260: 6565 7064 6f67 2f64 6972 6563 745f 6d6f  eepdog/direct_mo
 00000270: 6e74 655f 6361 726c 6f2f 646d 635f 6669  nte_carlo/dmc_fi
 00000280: 6c74 6572 732e 7079 da0a 3c6c 6973 7463  lters.py..<listc
 00000290: 6f6d 703e 0e00 0000 f300 0000 007a 3553  omp>.........z5S
 000002a0: 696e 676c 6544 6f74 506f 7465 6e74 6961  ingleDotPotentia
 000002b0: 6c46 696c 7465 722e 5f5f 696e 6974 5f5f  lFilter.__init__
 000002c0: 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973 7463  .<locals>.<listc
```

### Comparing `deepdog-1.2.0/deepdog/direct_monte_carlo/direct_mc.py` & `deepdog-1.2.1/deepdog/direct_monte_carlo/direct_mc.py`

 * *Files identical despite different names*

### Comparing `deepdog-1.2.0/deepdog/direct_monte_carlo/dmc_filters.py` & `deepdog-1.2.1/deepdog/direct_monte_carlo/dmc_filters.py`

 * *Files identical despite different names*

### Comparing `deepdog-1.2.0/deepdog/indexify/__init__.py` & `deepdog-1.2.1/deepdog/indexify/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -27,18 +27,18 @@
 	"""
 	The order of keys is very important, but collections.OrderedDict is no longer needed in python 3.7.
 	I think it's okay to rely on that.
 	"""
 
 	def __init__(self, list_dict: typing.Dict[str, typing.Sequence]):
 		self.dict = list_dict
+		self.product_dict = _dict_product(self.dict)
 
 	def indexify(self, n: int) -> typing.Dict[str, typing.Any]:
-		product_dict = _dict_product(self.dict)
-		return product_dict[n]
+		return self.product_dict[n]
 
 	def _indexify_indices(self, n: int) -> typing.Sequence[int]:
 		"""
 		legacy indexify from old scripts, copypast.
 		could be used like
 		>>> ret = {}
 		>>> for k, i in zip(self.dict.keys(), self._indexify_indices):
```

### Comparing `deepdog-1.2.0/deepdog/indexify/__pycache__/__init__.cpython-39.pyc` & `deepdog-1.2.1/deepdog/indexify/__pycache__/__init__.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu May  9 03:25:18 2024 UTC, .py size: 1700 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 1e42 3c66 a406 0000  a........B<f....
+00000000: 610d 0d0a 0000 0000 b520 4066 ae06 0000  a........ @f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 4800 0000 6400  .....@...sH...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6402 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 5a04 6503 a005 6506 a101 5a07 6403 6404  Z.e...e...Z.d.d.
 00000060: 8400 5a08 4700 6405 6406 8400 6406 8302  ..Z.G.d.d...d...
 00000070: 5a09 6402 5300 2907 7ac7 0a50 726f 6261  Z.d.S.).z..Proba
@@ -41,15 +41,15 @@
 00000280: 8302 8301 5600 0100 7102 6400 5300 a901  ....V...q.d.S...
 00000290: 4e29 03da 0464 6963 74da 037a 6970 da04  N)...dict..zip..
 000002a0: 6b65 7973 2902 da02 2e30 da01 78a9 01da  keys)....0..x...
 000002b0: 0564 6963 7473 a900 fa56 2f68 6f6d 652f  .dicts...V/home/
 000002c0: 6a65 6e6b 696e 732f 6167 656e 742f 776f  jenkins/agent/wo
 000002d0: 726b 7370 6163 652f 6769 7465 612d 7068  rkspace/gitea-ph
 000002e0: 7973 6963 735f 6465 6570 646f 675f 312e  ysics_deepdog_1.
-000002f0: 322e 302f 6465 6570 646f 672f 696e 6465  2.0/deepdog/inde
+000002f0: 322e 312f 6465 6570 646f 672f 696e 6465  2.1/deepdog/inde
 00000300: 7869 6679 2f5f 5f69 6e69 745f 5f2e 7079  xify/__init__.py
 00000310: da09 3c67 656e 6578 7072 3e17 0000 00f3  ..<genexpr>.....
 00000320: 0000 0000 7a20 5f64 6963 745f 7072 6f64  ....z _dict_prod
 00000330: 7563 742e 3c6c 6f63 616c 733e 2e3c 6765  uct.<locals>.<ge
 00000340: 6e65 7870 723e 2904 da04 6c69 7374 da09  nexpr>)...list..
 00000350: 6974 6572 746f 6f6c 73da 0770 726f 6475  itertools..produ
 00000360: 6374 da06 7661 6c75 6573 7208 0000 0072  ct..valuesr....r
@@ -71,82 +71,83 @@
 00000460: 6465 7265 6444 6963 7420 6973 206e 6f20  deredDict is no 
 00000470: 6c6f 6e67 6572 206e 6565 6465 6420 696e  longer needed in
 00000480: 2070 7974 686f 6e20 332e 372e 0a09 4920   python 3.7...I 
 00000490: 7468 696e 6b20 6974 2773 206f 6b61 7920  think it's okay 
 000004a0: 746f 2072 656c 7920 6f6e 2074 6861 742e  to rely on that.
 000004b0: 0a09 2901 da09 6c69 7374 5f64 6963 7463  ..)...list_dictc
 000004c0: 0200 0000 0000 0000 0000 0000 0200 0000  ................
-000004d0: 0200 0000 4300 0000 730a 0000 007c 017c  ....C...s....|.|
-000004e0: 005f 0064 0053 0072 0200 0000 2901 7203  ._.d.S.r....).r.
-000004f0: 0000 0029 02da 0473 656c 6672 1400 0000  ...)...selfr....
-00000500: 720a 0000 0072 0a00 0000 720b 0000 00da  r....r....r.....
-00000510: 085f 5f69 6e69 745f 5f20 0000 0073 0200  .__init__ ...s..
-00000520: 0000 0001 7a13 496e 6465 7869 6669 6572  ....z.Indexifier
-00000530: 2e5f 5f69 6e69 745f 5f29 02da 016e da06  .__init__)...n..
-00000540: 7265 7475 726e 6302 0000 0000 0000 0000  returnc.........
-00000550: 0000 0003 0000 0002 0000 0043 0000 0073  ...........C...s
-00000560: 1200 0000 7400 7c00 6a01 8301 7d02 7c02  ....t.|.j...}.|.
-00000570: 7c01 1900 5300 7202 0000 0029 0272 1200  |...S.r....).r..
-00000580: 0000 7203 0000 0029 0372 1500 0000 7217  ..r....).r....r.
-00000590: 0000 005a 0c70 726f 6475 6374 5f64 6963  ...Z.product_dic
-000005a0: 7472 0a00 0000 720a 0000 0072 0b00 0000  tr....r....r....
-000005b0: da08 696e 6465 7869 6679 2300 0000 7304  ..indexify#...s.
-000005c0: 0000 0000 010a 017a 1349 6e64 6578 6966  .......z.Indexif
-000005d0: 6965 722e 696e 6465 7869 6679 6302 0000  ier.indexifyc...
-000005e0: 0000 0000 0000 0000 0008 0000 0005 0000  ................
-000005f0: 0043 0000 0073 5e00 0000 6401 6402 8400  .C...s^...d.d...
-00000600: 7c00 6a00 a001 a100 4400 8301 7d02 7402  |.j.....D...}.t.
-00000610: a003 7c02 a101 7d03 7c01 7d04 7c03 7d05  ..|...}.|.}.|.}.
-00000620: 6700 7d06 7c02 6403 6404 8502 1900 4400  g.}.|.d.d.....D.
-00000630: 5d22 7d07 7c05 7c07 1a00 7d05 7c06 a004  ]"}.|.|...}.|...
-00000640: 7c04 7c05 1a00 a101 0100 7c04 7c05 1600  |.|.......|.|...
-00000650: 7d04 7136 7c06 5300 2905 7ac7 0a09 096c  }.q6|.S.).z....l
-00000660: 6567 6163 7920 696e 6465 7869 6679 2066  egacy indexify f
-00000670: 726f 6d20 6f6c 6420 7363 7269 7074 732c  rom old scripts,
-00000680: 2063 6f70 7970 6173 742e 0a09 0963 6f75   copypast....cou
-00000690: 6c64 2062 6520 7573 6564 206c 696b 650a  ld be used like.
-000006a0: 0909 3e3e 3e20 7265 7420 3d20 7b7d 0a09  ..>>> ret = {}..
-000006b0: 093e 3e3e 2066 6f72 206b 2c20 6920 696e  .>>> for k, i in
-000006c0: 207a 6970 2873 656c 662e 6469 6374 2e6b   zip(self.dict.k
-000006d0: 6579 7328 292c 2073 656c 662e 5f69 6e64  eys(), self._ind
-000006e0: 6578 6966 795f 696e 6469 6365 7329 3a0a  exify_indices):.
-000006f0: 0909 3e3e 3e09 0972 6574 5b6b 5d20 3d20  ..>>>..ret[k] = 
-00000700: 7365 6c66 2e64 6963 745b 6b5d 5b69 5d0a  self.dict[k][i].
-00000710: 0909 3e3e 3e20 7265 7475 726e 2072 6574  ..>>> return ret
-00000720: 0a09 0963 0100 0000 0000 0000 0000 0000  ...c............
-00000730: 0200 0000 0400 0000 5300 0000 7314 0000  ........S...s...
-00000740: 0067 007c 005d 0c7d 0174 007c 0183 0191  .g.|.].}.t.|....
-00000750: 0271 0453 0072 0a00 0000 2901 da03 6c65  .q.S.r....)...le
-00000760: 6e29 0272 0600 0000 da01 7672 0a00 0000  n).r......vr....
-00000770: 720a 0000 0072 0b00 0000 da0a 3c6c 6973  r....r......<lis
-00000780: 7463 6f6d 703e 3000 0000 720d 0000 007a  tcomp>0...r....z
-00000790: 3049 6e64 6578 6966 6965 722e 5f69 6e64  0Indexifier._ind
-000007a0: 6578 6966 795f 696e 6469 6365 732e 3c6c  exify_indices.<l
-000007b0: 6f63 616c 733e 2e3c 6c69 7374 636f 6d70  ocals>.<listcomp
-000007c0: 3e4e e9ff ffff ff29 0572 0300 0000 7211  >N.....).r....r.
-000007d0: 0000 00da 046d 6174 68da 0470 726f 64da  .....math..prod.
-000007e0: 0661 7070 656e 6429 0872 1500 0000 7217  .append).r....r.
-000007f0: 0000 00da 0777 6569 6768 7473 da01 4e5a  .....weights..NZ
-00000800: 0663 7572 725f 6e5a 0663 7572 725f 4eda  .curr_nZ.curr_N.
-00000810: 036f 7574 da01 7772 0a00 0000 720a 0000  .out..wr....r...
-00000820: 0072 0b00 0000 da11 5f69 6e64 6578 6966  .r......_indexif
-00000830: 795f 696e 6469 6365 7327 0000 0073 1400  y_indices'...s..
-00000840: 0000 0009 1401 0a01 0401 0401 0401 1002  ................
-00000850: 0801 0e01 0a01 7a1c 496e 6465 7869 6669  ......z.Indexifi
-00000860: 6572 2e5f 696e 6465 7869 6679 5f69 6e64  er._indexify_ind
-00000870: 6963 6573 4e29 0dda 085f 5f6e 616d 655f  icesN)...__name_
-00000880: 5fda 0a5f 5f6d 6f64 756c 655f 5fda 0c5f  _..__module__.._
-00000890: 5f71 7561 6c6e 616d 655f 5fda 075f 5f64  _qualname__..__d
-000008a0: 6f63 5f5f da06 7479 7069 6e67 da04 4469  oc__..typing..Di
-000008b0: 6374 da03 7374 72da 0853 6571 7565 6e63  ct..str..Sequenc
-000008c0: 6572 1600 0000 da03 696e 74da 0341 6e79  er......int..Any
-000008d0: 7219 0000 0072 2500 0000 720a 0000 0072  r....r%...r....r
-000008e0: 0a00 0000 720a 0000 0072 0b00 0000 7213  ....r....r....r.
-000008f0: 0000 001a 0000 0073 0800 0000 0801 0405  .......s........
-00000900: 1a03 1c04 7213 0000 0029 0a72 2900 0000  ....r....).r)...
-00000910: 720f 0000 0072 2a00 0000 da07 6c6f 6767  r....r*.....logg
-00000920: 696e 6772 1e00 0000 da09 6765 744c 6f67  ingr......getLog
-00000930: 6765 7272 2600 0000 da07 5f6c 6f67 6765  gerr&....._logge
-00000940: 7272 1200 0000 7213 0000 0072 0a00 0000  rr....r....r....
-00000950: 720a 0000 0072 0a00 0000 720b 0000 00da  r....r....r.....
-00000960: 083c 6d6f 6475 6c65 3e01 0000 0073 0e00  .<module>....s..
-00000970: 0000 0405 0801 0801 0801 0802 0a04 080b  ................
+000004d0: 0200 0000 4300 0000 7316 0000 007c 017c  ....C...s....|.|
+000004e0: 005f 0074 017c 006a 0083 017c 005f 0264  ._.t.|.j...|._.d
+000004f0: 0053 0072 0200 0000 2903 7203 0000 0072  .S.r....).r....r
+00000500: 1200 0000 da0c 7072 6f64 7563 745f 6469  ......product_di
+00000510: 6374 2902 da04 7365 6c66 7214 0000 0072  ct)...selfr....r
+00000520: 0a00 0000 720a 0000 0072 0b00 0000 da08  ....r....r......
+00000530: 5f5f 696e 6974 5f5f 2000 0000 7304 0000  __init__ ...s...
+00000540: 0000 0106 017a 1349 6e64 6578 6966 6965  .....z.Indexifie
+00000550: 722e 5f5f 696e 6974 5f5f 2902 da01 6eda  r.__init__)...n.
+00000560: 0672 6574 7572 6e63 0200 0000 0000 0000  .returnc........
+00000570: 0000 0000 0200 0000 0200 0000 4300 0000  ............C...
+00000580: 730a 0000 007c 006a 007c 0119 0053 0072  s....|.j.|...S.r
+00000590: 0200 0000 2901 7215 0000 0029 0272 1600  ....).r....).r..
+000005a0: 0000 7218 0000 0072 0a00 0000 720a 0000  ..r....r....r...
+000005b0: 0072 0b00 0000 da08 696e 6465 7869 6679  .r......indexify
+000005c0: 2400 0000 7302 0000 0000 017a 1349 6e64  $...s......z.Ind
+000005d0: 6578 6966 6965 722e 696e 6465 7869 6679  exifier.indexify
+000005e0: 6302 0000 0000 0000 0000 0000 0008 0000  c...............
+000005f0: 0005 0000 0043 0000 0073 5e00 0000 6401  .....C...s^...d.
+00000600: 6402 8400 7c00 6a00 a001 a100 4400 8301  d...|.j.....D...
+00000610: 7d02 7402 a003 7c02 a101 7d03 7c01 7d04  }.t...|...}.|.}.
+00000620: 7c03 7d05 6700 7d06 7c02 6403 6404 8502  |.}.g.}.|.d.d...
+00000630: 1900 4400 5d22 7d07 7c05 7c07 1a00 7d05  ..D.]"}.|.|...}.
+00000640: 7c06 a004 7c04 7c05 1a00 a101 0100 7c04  |...|.|.......|.
+00000650: 7c05 1600 7d04 7136 7c06 5300 2905 7ac7  |...}.q6|.S.).z.
+00000660: 0a09 096c 6567 6163 7920 696e 6465 7869  ...legacy indexi
+00000670: 6679 2066 726f 6d20 6f6c 6420 7363 7269  fy from old scri
+00000680: 7074 732c 2063 6f70 7970 6173 742e 0a09  pts, copypast...
+00000690: 0963 6f75 6c64 2062 6520 7573 6564 206c  .could be used l
+000006a0: 696b 650a 0909 3e3e 3e20 7265 7420 3d20  ike...>>> ret = 
+000006b0: 7b7d 0a09 093e 3e3e 2066 6f72 206b 2c20  {}...>>> for k, 
+000006c0: 6920 696e 207a 6970 2873 656c 662e 6469  i in zip(self.di
+000006d0: 6374 2e6b 6579 7328 292c 2073 656c 662e  ct.keys(), self.
+000006e0: 5f69 6e64 6578 6966 795f 696e 6469 6365  _indexify_indice
+000006f0: 7329 3a0a 0909 3e3e 3e09 0972 6574 5b6b  s):...>>>..ret[k
+00000700: 5d20 3d20 7365 6c66 2e64 6963 745b 6b5d  ] = self.dict[k]
+00000710: 5b69 5d0a 0909 3e3e 3e20 7265 7475 726e  [i]...>>> return
+00000720: 2072 6574 0a09 0963 0100 0000 0000 0000   ret...c........
+00000730: 0000 0000 0200 0000 0400 0000 5300 0000  ............S...
+00000740: 7314 0000 0067 007c 005d 0c7d 0174 007c  s....g.|.].}.t.|
+00000750: 0183 0191 0271 0453 0072 0a00 0000 2901  .....q.S.r....).
+00000760: da03 6c65 6e29 0272 0600 0000 da01 7672  ..len).r......vr
+00000770: 0a00 0000 720a 0000 0072 0b00 0000 da0a  ....r....r......
+00000780: 3c6c 6973 7463 6f6d 703e 3000 0000 720d  <listcomp>0...r.
+00000790: 0000 007a 3049 6e64 6578 6966 6965 722e  ...z0Indexifier.
+000007a0: 5f69 6e64 6578 6966 795f 696e 6469 6365  _indexify_indice
+000007b0: 732e 3c6c 6f63 616c 733e 2e3c 6c69 7374  s.<locals>.<list
+000007c0: 636f 6d70 3e4e e9ff ffff ff29 0572 0300  comp>N.....).r..
+000007d0: 0000 7211 0000 00da 046d 6174 68da 0470  ..r......math..p
+000007e0: 726f 64da 0661 7070 656e 6429 0872 1600  rod..append).r..
+000007f0: 0000 7218 0000 00da 0777 6569 6768 7473  ..r......weights
+00000800: da01 4e5a 0663 7572 725f 6e5a 0663 7572  ..NZ.curr_nZ.cur
+00000810: 725f 4eda 036f 7574 da01 7772 0a00 0000  r_N..out..wr....
+00000820: 720a 0000 0072 0b00 0000 da11 5f69 6e64  r....r......_ind
+00000830: 6578 6966 795f 696e 6469 6365 7327 0000  exify_indices'..
+00000840: 0073 1400 0000 0009 1401 0a01 0401 0401  .s..............
+00000850: 0401 1002 0801 0e01 0a01 7a1c 496e 6465  ..........z.Inde
+00000860: 7869 6669 6572 2e5f 696e 6465 7869 6679  xifier._indexify
+00000870: 5f69 6e64 6963 6573 4e29 0dda 085f 5f6e  _indicesN)...__n
+00000880: 616d 655f 5fda 0a5f 5f6d 6f64 756c 655f  ame__..__module_
+00000890: 5fda 0c5f 5f71 7561 6c6e 616d 655f 5fda  _..__qualname__.
+000008a0: 075f 5f64 6f63 5f5f da06 7479 7069 6e67  .__doc__..typing
+000008b0: da04 4469 6374 da03 7374 72da 0853 6571  ..Dict..str..Seq
+000008c0: 7565 6e63 6572 1700 0000 da03 696e 74da  uencer......int.
+000008d0: 0341 6e79 721a 0000 0072 2600 0000 720a  .Anyr....r&...r.
+000008e0: 0000 0072 0a00 0000 720a 0000 0072 0b00  ...r....r....r..
+000008f0: 0000 7213 0000 001a 0000 0073 0800 0000  ..r........s....
+00000900: 0801 0405 1a04 1c03 7213 0000 0029 0a72  ........r....).r
+00000910: 2a00 0000 720f 0000 0072 2b00 0000 da07  *...r....r+.....
+00000920: 6c6f 6767 696e 6772 1f00 0000 da09 6765  loggingr......ge
+00000930: 744c 6f67 6765 7272 2700 0000 da07 5f6c  tLoggerr'....._l
+00000940: 6f67 6765 7272 1200 0000 7213 0000 0072  oggerr....r....r
+00000950: 0a00 0000 720a 0000 0072 0a00 0000 720b  ....r....r....r.
+00000960: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
+00000970: 0073 0e00 0000 0405 0801 0801 0801 0802  .s..............
+00000980: 0a04 080b                                ....
```

### Comparing `deepdog-1.2.0/deepdog/real_spectrum_run.py` & `deepdog-1.2.1/deepdog/real_spectrum_run.py`

 * *Files identical despite different names*

### Comparing `deepdog-1.2.0/deepdog/results/__init__.py` & `deepdog-1.2.1/deepdog/results/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,28 +4,38 @@
 import logging
 import deepdog.indexify
 import pathlib
 import csv
 
 _logger = logging.getLogger(__name__)
 
-FILENAME_REGEX = r"(?P<timestamp>\d{8}-\d{6})-(?P<filename_slug>.*)\.realdata\.fast_filter\.bayesrun\.csv"
+FILENAME_REGEX = re.compile(
+	r"(?P<timestamp>\d{8}-\d{6})-(?P<filename_slug>.*)\.realdata\.fast_filter\.bayesrun\.csv"
+)
 
 MODEL_REGEXES = [
-	r"geom_(?P<xmin>-?\d+)_(?P<xmax>-?\d+)_(?P<ymin>-?\d+)_(?P<ymax>-?\d+)_(?P<zmin>-?\d+)_(?P<zmax>-?\d+)-orientation_(?P<orientation>free|fixedxy|fixedz)-dipole_count_(?P<avg_filled>\d+)_(?P<field_name>\w*)",
-	r"geom_(?P<xmin>-?\d+)_(?P<xmax>-?\d+)_(?P<ymin>-?\d+)_(?P<ymax>-?\d+)_(?P<zmin>-?\d+)_(?P<zmax>-?\d+)-magnitude_(?P<log_magnitude>\d*\.?\d+)-orientation_(?P<orientation>free|fixedxy|fixedz)-dipole_count_(?P<avg_filled>\d+)_(?P<field_name>\w*)",
-	r"geom_(?P<xmin>-?\d*\.?\d+)_(?P<xmax>-?\d*\.?\d+)_(?P<ymin>-?\d*\.?\d+)_(?P<ymax>-?\d*\.?\d+)_(?P<zmin>-?\d*\.?\d+)_(?P<zmax>-?\d*\.?\d+)-magnitude_(?P<log_magnitude>\d*\.?\d+)-orientation_(?P<orientation>free|fixedxy|fixedz)-dipole_count_(?P<avg_filled>\d+)_(?P<field_name>\w*)"
+	re.compile(pattern)
+	for pattern in [
+		r"geom_(?P<xmin>-?\d+)_(?P<xmax>-?\d+)_(?P<ymin>-?\d+)_(?P<ymax>-?\d+)_(?P<zmin>-?\d+)_(?P<zmax>-?\d+)-orientation_(?P<orientation>free|fixedxy|fixedz)-dipole_count_(?P<avg_filled>\d+)_(?P<field_name>\w*)",
+		r"geom_(?P<xmin>-?\d+)_(?P<xmax>-?\d+)_(?P<ymin>-?\d+)_(?P<ymax>-?\d+)_(?P<zmin>-?\d+)_(?P<zmax>-?\d+)-magnitude_(?P<log_magnitude>\d*\.?\d+)-orientation_(?P<orientation>free|fixedxy|fixedz)-dipole_count_(?P<avg_filled>\d+)_(?P<field_name>\w*)",
+		r"geom_(?P<xmin>-?\d*\.?\d+)_(?P<xmax>-?\d*\.?\d+)_(?P<ymin>-?\d*\.?\d+)_(?P<ymax>-?\d*\.?\d+)_(?P<zmin>-?\d*\.?\d+)_(?P<zmax>-?\d*\.?\d+)-magnitude_(?P<log_magnitude>\d*\.?\d+)-orientation_(?P<orientation>free|fixedxy|fixedz)-dipole_count_(?P<avg_filled>\d+)_(?P<field_name>\w*)",
+	]
 ]
 
 FILE_SLUG_REGEXES = [
-	r"mock_tarucha-(?P<job_index>\d+)",
-	r"(?:(?P<mock>mock)_)?tarucha(?:_(?P<tarucha_run_id>\d+))?-(?P<job_index>\d+)",
-	r"(?P<tag>\w+)-(?P<job_index>\d+)",
+	re.compile(pattern)
+	for pattern in [
+		r"(?P<tag>\w+)-(?P<job_index>\d+)",
+		r"mock_tarucha-(?P<job_index>\d+)",
+		r"(?:(?P<mock>mock)_)?tarucha(?:_(?P<tarucha_run_id>\d+))?-(?P<job_index>\d+)",
+	]
 ]
 
+SIMPLE_TAG_REGEX = re.compile(r"\w+-\d+")
+
 
 @dataclasses.dataclass
 class BayesrunOutputFilename:
 	timestamp: str
 	filename_slug: str
 	path: pathlib.Path
 
@@ -82,15 +92,15 @@
 	column: str,
 ) -> typing.Optional[BayesrunColumnParsed]:
 	"""
 	Tries one by one all of a predefined list of regexes that I might have used in the past.
 	Returns the groupdict for the first match, or None if no match found.
 	"""
 	for pattern in MODEL_REGEXES:
-		match = re.match(pattern, column)
+		match = pattern.match(column)
 		if match:
 			return BayesrunColumnParsed(match.groupdict())
 	else:
 		return None
 
 
 def _parse_bayesrun_row(
@@ -121,26 +131,26 @@
 			)
 		)
 	return results
 
 
 def _parse_output_filename(file: pathlib.Path) -> BayesrunOutputFilename:
 	filename = file.name
-	match = re.match(FILENAME_REGEX, filename)
+	match = FILENAME_REGEX.match(filename)
 	if not match:
 		raise ValueError(f"{filename} was not a valid bayesrun output")
 	groups = match.groupdict()
 	return BayesrunOutputFilename(
 		timestamp=groups["timestamp"], filename_slug=groups["filename_slug"], path=file
 	)
 
 
 def _parse_file_slug(slug: str) -> typing.Optional[typing.Dict[str, str]]:
 	for pattern in FILE_SLUG_REGEXES:
-		match = re.match(pattern, slug)
+		match = pattern.match(slug)
 		if match:
 			return match.groupdict()
 	else:
 		return None
 
 
 def read_output_file(
```

### Comparing `deepdog-1.2.0/deepdog/subset_simulation/subset_simulation_impl.py` & `deepdog-1.2.1/deepdog/subset_simulation/subset_simulation_impl.py`

 * *Files identical despite different names*

### Comparing `deepdog-1.2.0/deepdog/temp_aware_real_spectrum_run.py` & `deepdog-1.2.1/deepdog/temp_aware_real_spectrum_run.py`

 * *Files identical despite different names*

### Comparing `deepdog-1.2.0/pyproject.toml` & `deepdog-1.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "deepdog"
-version = "1.2.0"
+version = "1.2.1"
 description = ""
 authors = ["Deepak Mallubhotla <dmallubhotla+github@gmail.com>"]
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.10"
 pdme = "^1.2.0"
 numpy = "1.22.3"
```

