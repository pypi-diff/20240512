# Comparing `tmp/samples-filter-0.4.1.tar.gz` & `tmp/samples-filter-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "samples-filter-0.4.1.tar", last modified: Wed May  8 13:01:47 2024, max compression
+gzip compressed data, was "samples-filter-0.5.1.tar", last modified: Sun May 12 10:34:12 2024, max compression
```

## Comparing `samples-filter-0.4.1.tar` & `samples-filter-0.5.1.tar`

### file list

```diff
@@ -1,28 +1,27 @@
-drwxrwxr-x   0 r         (1000) r         (1001)        0 2024-05-08 13:01:47.452942 samples-filter-0.4.1/
--rw-r--r--   0 r         (1000) r         (1001)     1087 2024-05-08 12:56:33.000000 samples-filter-0.4.1/LICENSE.txt
--rw-rw-r--   0 r         (1000) r         (1001)     4145 2024-05-08 13:01:47.452942 samples-filter-0.4.1/PKG-INFO
--rw-r--r--   0 r         (1000) r         (1001)     3442 2024-05-08 12:56:33.000000 samples-filter-0.4.1/README.md
-drwxrwxr-x   0 r         (1000) r         (1001)        0 2024-05-08 13:01:47.436943 samples-filter-0.4.1/samples_filter.egg-info/
--rw-rw-r--   0 r         (1000) r         (1001)     4145 2024-05-08 13:01:47.000000 samples-filter-0.4.1/samples_filter.egg-info/PKG-INFO
--rw-rw-r--   0 r         (1000) r         (1001)      495 2024-05-08 13:01:47.000000 samples-filter-0.4.1/samples_filter.egg-info/SOURCES.txt
--rw-rw-r--   0 r         (1000) r         (1001)        1 2024-05-08 13:01:47.000000 samples-filter-0.4.1/samples_filter.egg-info/dependency_links.txt
--rw-rw-r--   0 r         (1000) r         (1001)       54 2024-05-08 13:01:47.000000 samples-filter-0.4.1/samples_filter.egg-info/entry_points.txt
--rw-rw-r--   0 r         (1000) r         (1001)       49 2024-05-08 13:01:47.000000 samples-filter-0.4.1/samples_filter.egg-info/requires.txt
--rw-rw-r--   0 r         (1000) r         (1001)        4 2024-05-08 13:01:47.000000 samples-filter-0.4.1/samples_filter.egg-info/top_level.txt
--rw-rw-r--   0 r         (1000) r         (1001)       38 2024-05-08 13:01:47.452942 samples-filter-0.4.1/setup.cfg
--rw-r--r--   0 r         (1000) r         (1001)     2592 2024-05-08 12:56:33.000000 samples-filter-0.4.1/setup.py
-drwxrwxr-x   0 r         (1000) r         (1001)        0 2024-05-08 13:01:47.448942 samples-filter-0.4.1/src/
--rw-r--r--   0 r         (1000) r         (1001)     1261 2024-05-08 12:56:33.000000 samples-filter-0.4.1/src/__init__.py
--rw-r--r--   0 r         (1000) r         (1001)     1430 2024-05-08 12:56:33.000000 samples-filter-0.4.1/src/__main__.py
--rw-r--r--   0 r         (1000) r         (1001)     2781 2024-05-08 12:56:33.000000 samples-filter-0.4.1/src/cli.py
--rw-r--r--   0 r         (1000) r         (1001)     2757 2024-05-08 12:56:33.000000 samples-filter-0.4.1/src/dataset.py
--rw-r--r--   0 r         (1000) r         (1001)     2134 2024-05-08 12:56:33.000000 samples-filter-0.4.1/src/feed.py
--rw-r--r--   0 r         (1000) r         (1001)     3452 2024-05-08 12:56:33.000000 samples-filter-0.4.1/src/filter_pipe.py
--rw-r--r--   0 r         (1000) r         (1001)     2980 2024-05-08 12:56:33.000000 samples-filter-0.4.1/src/input.py
--rw-r--r--   0 r         (1000) r         (1001)     1405 2024-05-08 12:56:33.000000 samples-filter-0.4.1/src/model_map.py
--rw-r--r--   0 r         (1000) r         (1001)     1433 2024-05-08 12:56:33.000000 samples-filter-0.4.1/src/pre_filter.py
--rw-r--r--   0 r         (1000) r         (1001)     1586 2024-05-08 12:56:33.000000 samples-filter-0.4.1/src/readme.py
--rw-r--r--   0 r         (1000) r         (1001)     1792 2024-05-08 12:56:33.000000 samples-filter-0.4.1/src/remote_asset.py
--rw-r--r--   0 r         (1000) r         (1001)     1561 2024-05-08 12:56:33.000000 samples-filter-0.4.1/src/rf_model.py
--rw-r--r--   0 r         (1000) r         (1001)     1596 2024-05-08 12:56:33.000000 samples-filter-0.4.1/src/text_prediction.py
--rw-r--r--   0 r         (1000) r         (1001)     1493 2024-05-08 12:56:33.000000 samples-filter-0.4.1/src/transformer_model.py
+drwxrwxr-x   0 r         (1000) r         (1001)        0 2024-05-12 10:34:12.225903 samples-filter-0.5.1/
+-rw-r--r--   0 r         (1000) r         (1001)     1087 2024-05-12 10:28:56.000000 samples-filter-0.5.1/LICENSE.txt
+-rw-rw-r--   0 r         (1000) r         (1001)     4145 2024-05-12 10:34:12.225903 samples-filter-0.5.1/PKG-INFO
+-rw-r--r--   0 r         (1000) r         (1001)     3442 2024-05-12 10:28:56.000000 samples-filter-0.5.1/README.md
+drwxrwxr-x   0 r         (1000) r         (1001)        0 2024-05-12 10:34:12.209903 samples-filter-0.5.1/samples_filter.egg-info/
+-rw-rw-r--   0 r         (1000) r         (1001)     4145 2024-05-12 10:34:12.000000 samples-filter-0.5.1/samples_filter.egg-info/PKG-INFO
+-rw-rw-r--   0 r         (1000) r         (1001)      480 2024-05-12 10:34:12.000000 samples-filter-0.5.1/samples_filter.egg-info/SOURCES.txt
+-rw-rw-r--   0 r         (1000) r         (1001)        1 2024-05-12 10:34:12.000000 samples-filter-0.5.1/samples_filter.egg-info/dependency_links.txt
+-rw-rw-r--   0 r         (1000) r         (1001)       54 2024-05-12 10:34:12.000000 samples-filter-0.5.1/samples_filter.egg-info/entry_points.txt
+-rw-rw-r--   0 r         (1000) r         (1001)       49 2024-05-12 10:34:12.000000 samples-filter-0.5.1/samples_filter.egg-info/requires.txt
+-rw-rw-r--   0 r         (1000) r         (1001)        4 2024-05-12 10:34:12.000000 samples-filter-0.5.1/samples_filter.egg-info/top_level.txt
+-rw-rw-r--   0 r         (1000) r         (1001)       38 2024-05-12 10:34:12.225903 samples-filter-0.5.1/setup.cfg
+-rw-r--r--   0 r         (1000) r         (1001)     2592 2024-05-12 10:28:56.000000 samples-filter-0.5.1/setup.py
+drwxrwxr-x   0 r         (1000) r         (1001)        0 2024-05-12 10:34:12.221903 samples-filter-0.5.1/src/
+-rw-r--r--   0 r         (1000) r         (1001)     1261 2024-05-12 10:28:56.000000 samples-filter-0.5.1/src/__init__.py
+-rw-r--r--   0 r         (1000) r         (1001)     1430 2024-05-12 10:28:56.000000 samples-filter-0.5.1/src/__main__.py
+-rw-r--r--   0 r         (1000) r         (1001)     2378 2024-05-12 10:28:56.000000 samples-filter-0.5.1/src/cli.py
+-rw-r--r--   0 r         (1000) r         (1001)     2041 2024-05-12 10:28:56.000000 samples-filter-0.5.1/src/feed.py
+-rw-r--r--   0 r         (1000) r         (1001)     3491 2024-05-12 10:28:56.000000 samples-filter-0.5.1/src/filter_pipe.py
+-rw-r--r--   0 r         (1000) r         (1001)     2348 2024-05-12 10:28:56.000000 samples-filter-0.5.1/src/input.py
+-rw-r--r--   0 r         (1000) r         (1001)     1405 2024-05-12 10:28:56.000000 samples-filter-0.5.1/src/model_map.py
+-rw-r--r--   0 r         (1000) r         (1001)     1433 2024-05-12 10:28:56.000000 samples-filter-0.5.1/src/pre_filter.py
+-rw-r--r--   0 r         (1000) r         (1001)     1586 2024-05-12 10:28:56.000000 samples-filter-0.5.1/src/readme.py
+-rw-r--r--   0 r         (1000) r         (1001)     1792 2024-05-12 10:28:56.000000 samples-filter-0.5.1/src/remote_asset.py
+-rw-r--r--   0 r         (1000) r         (1001)     1561 2024-05-12 10:28:56.000000 samples-filter-0.5.1/src/rf_model.py
+-rw-r--r--   0 r         (1000) r         (1001)     1596 2024-05-12 10:28:56.000000 samples-filter-0.5.1/src/text_prediction.py
+-rw-r--r--   0 r         (1000) r         (1001)     1493 2024-05-12 10:28:56.000000 samples-filter-0.5.1/src/transformer_model.py
```

### Comparing `samples-filter-0.4.1/LICENSE.txt` & `samples-filter-0.5.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `samples-filter-0.4.1/PKG-INFO` & `samples-filter-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: samples-filter
-Version: 0.4.1
+Version: 0.5.1
 Summary: Command-line filter for GitHub repositories that contain "samples", instead of real project or framework or library
 Home-page: https://github.com/h1alexbel/samples-filter
 Author: Aliaksei Bialiauski
 Author-email: aliaksei.bialiauski@hey.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -61,16 +61,16 @@
 
 For `--repositories` you should provide a name of **existing** [CSV] dataset
 with GitHub repositories, and name for the output file in `--out`
 (it will be created automatically). If you feel missed, try `--help` and tool
 will explain to you what you should do.
 
 Optionally, you can decide which [model](/model/README.md) to use for
-filtering via `--model`. You can pass either `rf` (the default one), or
-`transformer`.
+filtering via `--model`. You can pass either `transformer` (the default one), or
+`rf`.
 
 ## How to contribute
 
 Fork repository, make changes, send us a [pull request](https://www.yegor256.com/2014/04/15/github-guidelines.html).
 We will review your changes and apply them to the `master` branch shortly,
 provided they don't violate our quality standards. To avoid frustration,
 before sending us your pull request please run full build:
```

### Comparing `samples-filter-0.4.1/README.md` & `samples-filter-0.5.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -43,16 +43,16 @@
 
 For `--repositories` you should provide a name of **existing** [CSV] dataset
 with GitHub repositories, and name for the output file in `--out`
 (it will be created automatically). If you feel missed, try `--help` and tool
 will explain to you what you should do.
 
 Optionally, you can decide which [model](/model/README.md) to use for
-filtering via `--model`. You can pass either `rf` (the default one), or
-`transformer`.
+filtering via `--model`. You can pass either `transformer` (the default one), or
+`rf`.
 
 ## How to contribute
 
 Fork repository, make changes, send us a [pull request](https://www.yegor256.com/2014/04/15/github-guidelines.html).
 We will review your changes and apply them to the `master` branch shortly,
 provided they don't violate our quality standards. To avoid frustration,
 before sending us your pull request please run full build:
```

### Comparing `samples-filter-0.4.1/samples_filter.egg-info/PKG-INFO` & `samples-filter-0.5.1/samples_filter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: samples-filter
-Version: 0.4.1
+Version: 0.5.1
 Summary: Command-line filter for GitHub repositories that contain "samples", instead of real project or framework or library
 Home-page: https://github.com/h1alexbel/samples-filter
 Author: Aliaksei Bialiauski
 Author-email: aliaksei.bialiauski@hey.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -61,16 +61,16 @@
 
 For `--repositories` you should provide a name of **existing** [CSV] dataset
 with GitHub repositories, and name for the output file in `--out`
 (it will be created automatically). If you feel missed, try `--help` and tool
 will explain to you what you should do.
 
 Optionally, you can decide which [model](/model/README.md) to use for
-filtering via `--model`. You can pass either `rf` (the default one), or
-`transformer`.
+filtering via `--model`. You can pass either `transformer` (the default one), or
+`rf`.
 
 ## How to contribute
 
 Fork repository, make changes, send us a [pull request](https://www.yegor256.com/2014/04/15/github-guidelines.html).
 We will review your changes and apply them to the `master` branch shortly,
 provided they don't violate our quality standards. To avoid frustration,
 before sending us your pull request please run full build:
```

### Comparing `samples-filter-0.4.1/setup.py` & `samples-filter-0.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `samples-filter-0.4.1/src/__init__.py` & `samples-filter-0.5.1/src/__init__.py`

 * *Files identical despite different names*

### Comparing `samples-filter-0.4.1/src/__main__.py` & `samples-filter-0.5.1/src/__main__.py`

 * *Files identical despite different names*

### Comparing `samples-filter-0.4.1/src/cli.py` & `samples-filter-0.5.1/src/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -68,107 +68,82 @@
 00000430: 5741 5245 204f 5220 5448 4520 5553 4520  WARE OR THE USE 
 00000440: 4f52 204f 5448 4552 2044 4541 4c49 4e47  OR OTHER DEALING
 00000450: 5320 494e 2054 4845 0a23 2053 4f46 5457  S IN THE.# SOFTW
 00000460: 4152 452e 0a0a 2222 220a 436c 6920 7275  ARE...""".Cli ru
 00000470: 6e6e 6572 2e0a 2222 220a 6672 6f6d 2074  nner..""".from t
 00000480: 7970 696e 6720 696d 706f 7274 204f 7074  yping import Opt
 00000490: 696f 6e61 6c0a 0a69 6d70 6f72 7420 7479  ional..import ty
-000004a0: 7065 720a 0a66 726f 6d20 2e6d 6f64 656c  per..from .model
-000004b0: 5f6d 6170 2069 6d70 6f72 7420 4d6f 6465  _map import Mode
-000004c0: 6c4d 6170 0a66 726f 6d20 2e66 696c 7465  lMap.from .filte
-000004d0: 725f 7069 7065 2069 6d70 6f72 7420 4669  r_pipe import Fi
-000004e0: 6c74 6572 5069 7065 0a66 726f 6d20 7372  lterPipe.from sr
-000004f0: 6320 696d 706f 7274 204e 414d 452c 2056  c import NAME, V
-00000500: 4552 5349 4f4e 0a0a 6170 7020 3d20 7479  ERSION..app = ty
-00000510: 7065 722e 5479 7065 7228 290a 0a0a 6465  per.Typer()...de
-00000520: 6620 5f76 6572 7369 6f6e 5f63 616c 6c62  f _version_callb
-00000530: 6163 6b28 7661 6c75 653a 2062 6f6f 6c29  ack(value: bool)
-00000540: 202d 3e20 4e6f 6e65 3a0a 2020 2020 6966   -> None:.    if
-00000550: 2076 616c 7565 3a0a 2020 2020 2020 2020   value:.        
-00000560: 7479 7065 722e 6563 686f 2866 227b 5645  typer.echo(f"{VE
-00000570: 5253 494f 4e7d 2229 0a20 2020 2020 2020  RSION}").       
-00000580: 2072 6169 7365 2074 7970 6572 2e45 7869   raise typer.Exi
-00000590: 7428 290a 0a0a 4061 7070 2e63 6f6d 6d61  t()...@app.comma
-000005a0: 6e64 2829 0a64 6566 2066 696c 7465 7228  nd().def filter(
-000005b0: 0a20 2020 2020 2020 2072 6570 6f73 6974  .        reposit
-000005c0: 6f72 6965 733a 2073 7472 203d 2074 7970  ories: str = typ
-000005d0: 6572 2e4f 7074 696f 6e28 0a20 2020 2020  er.Option(.     
-000005e0: 2020 2020 2020 202e 2e2e 2c20 222d 2d72         ..., "--r
-000005f0: 6570 6f73 6974 6f72 6965 7322 2c20 6865  epositories", he
-00000600: 6c70 3d22 5061 7468 2074 6f20 7468 6520  lp="Path to the 
-00000610: 696e 7075 7420 7265 706f 7369 746f 7269  input repositori
-00000620: 6573 2043 5356 2066 696c 652e 220a 2020  es CSV file.".  
-00000630: 2020 2020 2020 292c 0a20 2020 2020 2020        ),.       
-00000640: 206f 7574 3a20 7374 7220 3d20 7479 7065   out: str = type
-00000650: 722e 4f70 7469 6f6e 280a 2020 2020 2020  r.Option(.      
-00000660: 2020 2020 2020 2e2e 2e2c 2022 2d2d 6f75        ..., "--ou
-00000670: 7422 2c20 6865 6c70 3d22 5061 7468 2074  t", help="Path t
-00000680: 6f20 7468 6520 6f75 7470 7574 2043 5356  o the output CSV
-00000690: 2066 696c 652e 220a 2020 2020 2020 2020   file.".        
-000006a0: 292c 0a20 2020 2020 2020 206d 6f64 656c  ),.        model
-000006b0: 3a20 7374 7220 3d20 7479 7065 722e 4f70  : str = typer.Op
-000006c0: 7469 6f6e 280a 2020 2020 2020 2020 2020  tion(.          
-000006d0: 2020 2272 6622 2c20 222d 2d6d 6f64 656c    "rf", "--model
-000006e0: 222c 2068 656c 703d 2257 6869 6368 204d  ", help="Which M
-000006f0: 4c20 6d6f 6465 6c20 746f 2075 7365 2e22  L model to use."
-00000700: 0a20 2020 2020 2020 2029 0a29 3a0a 2020  .        ).):.  
-00000710: 2020 2222 220a 2020 2020 4669 6c74 6572    """.    Filter
-00000720: 2072 6570 6f73 6974 6f72 6965 732e 0a20   repositories.. 
-00000730: 2020 2022 2222 0a20 2020 206d 6f64 656c     """.    model
-00000740: 7320 3d20 4d6f 6465 6c4d 6170 2829 2e62  s = ModelMap().b
-00000750: 7569 6c64 2829 0a20 2020 2023 2040 746f  uild().    # @to
-00000760: 646f 2023 3138 3a33 306d 696e 2046 696e  do #18:30min Fin
-00000770: 6420 6566 6665 6374 6976 6520 7761 7920  d effective way 
-00000780: 666f 7220 7072 6f63 6573 7369 6e67 2072  for processing r
-00000790: 6561 646d 652e 0a20 2020 2023 2020 466f  eadme..    #  Fo
-000007a0: 7220 6e6f 7720 7765 2061 7265 206e 6f74  r now we are not
-000007b0: 2070 726f 6365 7373 696e 6720 7265 6164   processing read
-000007c0: 6d65 2062 6563 6175 7365 206f 660a 2020  me because of.  
-000007d0: 2020 2320 203c 6120 6872 6566 3d22 6874    #  <a href="ht
-000007e0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-000007f0: 2f68 3161 6c65 7862 656c 2f73 616d 706c  /h1alexbel/sampl
-00000800: 6573 2d66 696c 7465 722f 6973 7375 6573  es-filter/issues
-00000810: 2f33 3922 3e74 6869 733c 2f61 3e2e 0a20  /39">this</a>.. 
-00000820: 2020 2023 2020 5765 206e 6565 6420 746f     #  We need to
-00000830: 2066 696e 6420 6163 7475 616c 2077 6179   find actual way
-00000840: 2074 6f20 7072 6f63 6573 7320 7265 6164   to process read
-00000850: 6d65 2074 6f6f 2073 696e 6365 2069 7420  me too since it 
-00000860: 6361 6e20 6265 2063 7275 6369 616c 0a20  can be crucial. 
-00000870: 2020 2023 2020 6461 7461 2061 7320 6d6f     #  data as mo
-00000880: 6465 6c20 696e 7075 742e 204c 6574 2773  del input. Let's
-00000890: 2073 7475 6479 2070 6170 6572 732c 206f   study papers, o
-000008a0: 7574 6c69 6e65 640a 2020 2020 2320 203c  utlined.    #  <
-000008b0: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
-000008c0: 6769 7468 7562 2e63 6f6d 2f79 6567 6f72  github.com/yegor
-000008d0: 3235 362f 6361 6d2f 6973 7375 6573 2f32  256/cam/issues/2
-000008e0: 3237 2369 7373 7565 2d32 3230 3030 3830  27#issue-2200080
-000008f0: 3535 3922 3e68 6572 653c 2f61 3e0a 2020  559">here</a>.  
-00000900: 2020 2320 2066 6972 7374 2c20 7265 7468    #  first, reth
-00000910: 696e 6b20 6974 2061 6e64 2074 7279 2074  ink it and try t
-00000920: 6f20 696d 706c 656d 656e 7420 6865 7265  o implement here
-00000930: 2e0a 2020 2020 4669 6c74 6572 5069 7065  ..    FilterPipe
-00000940: 2872 6570 6f73 6974 6f72 6965 732c 206f  (repositories, o
-00000950: 7574 2c20 6d6f 6465 6c73 2e67 6574 286d  ut, models.get(m
-00000960: 6f64 656c 292c 2074 7970 6572 292e 6170  odel), typer).ap
-00000970: 706c 7928 290a 0a0a 2320 5275 6e20 6974  ply()...# Run it
-00000980: 2e0a 4061 7070 2e63 616c 6c62 6163 6b28  ..@app.callback(
-00000990: 290a 6465 6620 6d61 696e 280a 2020 2020  ).def main(.    
-000009a0: 2020 2020 2320 7079 6c69 6e74 3a20 6469      # pylint: di
-000009b0: 7361 626c 653d 756e 7573 6564 2d61 7267  sable=unused-arg
-000009c0: 756d 656e 740a 2020 2020 2020 2020 7665  ument.        ve
-000009d0: 7273 696f 6e3a 204f 7074 696f 6e61 6c5b  rsion: Optional[
-000009e0: 626f 6f6c 5d20 3d20 7479 7065 722e 4f70  bool] = typer.Op
-000009f0: 7469 6f6e 280a 2020 2020 2020 2020 2020  tion(.          
-00000a00: 2020 4e6f 6e65 2c0a 2020 2020 2020 2020    None,.        
-00000a10: 2020 2020 222d 2d76 6572 7369 6f6e 222c      "--version",
-00000a20: 0a20 2020 2020 2020 2020 2020 2068 656c  .            hel
-00000a30: 703d 2253 686f 7720 7468 6520 6170 706c  p="Show the appl
-00000a40: 6963 6174 696f 6e27 7320 7665 7273 696f  ication's versio
-00000a50: 6e20 616e 6420 6578 6974 2e22 2c0a 2020  n and exit.",.  
-00000a60: 2020 2020 2020 2020 2020 6361 6c6c 6261            callba
-00000a70: 636b 3d5f 7665 7273 696f 6e5f 6361 6c6c  ck=_version_call
-00000a80: 6261 636b 2c0a 2020 2020 2020 2020 2020  back,.          
-00000a90: 2020 6973 5f65 6167 6572 3d54 7275 652c    is_eager=True,
-00000aa0: 0a20 2020 2020 2020 2029 0a29 202d 3e20  .        ).) -> 
-00000ab0: 4e6f 6e65 3a0a 2020 2020 6622 2222 0a20  None:.    f""". 
-00000ac0: 2020 207b 4e41 4d45 7d0a 2020 2020 2222     {NAME}.    ""
-00000ad0: 220a 2020 2020 7265 7475 726e 0a         ".    return.
+000004a0: 7065 720a 0a66 726f 6d20 2e70 7265 5f66  per..from .pre_f
+000004b0: 696c 7465 7220 696d 706f 7274 2050 7265  ilter import Pre
+000004c0: 4669 6c74 6572 0a66 726f 6d20 2e6d 6f64  Filter.from .mod
+000004d0: 656c 5f6d 6170 2069 6d70 6f72 7420 4d6f  el_map import Mo
+000004e0: 6465 6c4d 6170 0a66 726f 6d20 2e66 696c  delMap.from .fil
+000004f0: 7465 725f 7069 7065 2069 6d70 6f72 7420  ter_pipe import 
+00000500: 4669 6c74 6572 5069 7065 0a66 726f 6d20  FilterPipe.from 
+00000510: 7372 6320 696d 706f 7274 204e 414d 452c  src import NAME,
+00000520: 2056 4552 5349 4f4e 0a0a 6170 7020 3d20   VERSION..app = 
+00000530: 7479 7065 722e 5479 7065 7228 290a 0a0a  typer.Typer()...
+00000540: 6465 6620 5f76 6572 7369 6f6e 5f63 616c  def _version_cal
+00000550: 6c62 6163 6b28 7661 6c75 653a 2062 6f6f  lback(value: boo
+00000560: 6c29 202d 3e20 4e6f 6e65 3a0a 2020 2020  l) -> None:.    
+00000570: 6966 2076 616c 7565 3a0a 2020 2020 2020  if value:.      
+00000580: 2020 7479 7065 722e 6563 686f 2866 227b    typer.echo(f"{
+00000590: 5645 5253 494f 4e7d 2229 0a20 2020 2020  VERSION}").     
+000005a0: 2020 2072 6169 7365 2074 7970 6572 2e45     raise typer.E
+000005b0: 7869 7428 290a 0a0a 4061 7070 2e63 6f6d  xit()...@app.com
+000005c0: 6d61 6e64 2829 0a64 6566 2066 696c 7465  mand().def filte
+000005d0: 7228 0a20 2020 2020 2020 2072 6570 6f73  r(.        repos
+000005e0: 6974 6f72 6965 733a 2073 7472 203d 2074  itories: str = t
+000005f0: 7970 6572 2e4f 7074 696f 6e28 0a20 2020  yper.Option(.   
+00000600: 2020 2020 2020 2020 202e 2e2e 2c20 222d           ..., "-
+00000610: 2d72 6570 6f73 6974 6f72 6965 7322 2c20  -repositories", 
+00000620: 6865 6c70 3d22 5061 7468 2074 6f20 7468  help="Path to th
+00000630: 6520 696e 7075 7420 7265 706f 7369 746f  e input reposito
+00000640: 7269 6573 2043 5356 2066 696c 652e 220a  ries CSV file.".
+00000650: 2020 2020 2020 2020 292c 0a20 2020 2020          ),.     
+00000660: 2020 206f 7574 3a20 7374 7220 3d20 7479     out: str = ty
+00000670: 7065 722e 4f70 7469 6f6e 280a 2020 2020  per.Option(.    
+00000680: 2020 2020 2020 2020 2e2e 2e2c 2022 2d2d          ..., "--
+00000690: 6f75 7422 2c20 6865 6c70 3d22 5061 7468  out", help="Path
+000006a0: 2074 6f20 7468 6520 6f75 7470 7574 2043   to the output C
+000006b0: 5356 2066 696c 652e 220a 2020 2020 2020  SV file.".      
+000006c0: 2020 292c 0a20 2020 2020 2020 206d 6f64    ),.        mod
+000006d0: 656c 3a20 7374 7220 3d20 7479 7065 722e  el: str = typer.
+000006e0: 4f70 7469 6f6e 280a 2020 2020 2020 2020  Option(.        
+000006f0: 2020 2020 2274 7261 6e73 666f 726d 6572      "transformer
+00000700: 222c 2022 2d2d 6d6f 6465 6c22 2c20 6865  ", "--model", he
+00000710: 6c70 3d22 5768 6963 6820 4d4c 206d 6f64  lp="Which ML mod
+00000720: 656c 2074 6f20 7573 652e 220a 2020 2020  el to use.".    
+00000730: 2020 2020 290a 293a 0a20 2020 2022 2222      ).):.    """
+00000740: 0a20 2020 2046 696c 7465 7220 7265 706f  .    Filter repo
+00000750: 7369 746f 7269 6573 2e0a 2020 2020 2222  sitories..    ""
+00000760: 220a 2020 2020 5072 6546 696c 7465 7228  ".    PreFilter(
+00000770: 6f75 7429 2e70 7265 7061 7265 2829 0a20  out).prepare(). 
+00000780: 2020 206d 6f64 656c 7320 3d20 4d6f 6465     models = Mode
+00000790: 6c4d 6170 2829 2e62 7569 6c64 2829 0a20  lMap().build(). 
+000007a0: 2020 2046 696c 7465 7250 6970 6528 7265     FilterPipe(re
+000007b0: 706f 7369 746f 7269 6573 2c20 6f75 742c  positories, out,
+000007c0: 206d 6f64 656c 732e 6765 7428 6d6f 6465   models.get(mode
+000007d0: 6c29 2c20 7479 7065 7229 2e61 7070 6c79  l), typer).apply
+000007e0: 2829 0a0a 0a23 2052 756e 2069 742e 0a40  ()...# Run it..@
+000007f0: 6170 702e 6361 6c6c 6261 636b 2829 0a64  app.callback().d
+00000800: 6566 206d 6169 6e28 0a20 2020 2020 2020  ef main(.       
+00000810: 2023 2070 796c 696e 743a 2064 6973 6162   # pylint: disab
+00000820: 6c65 3d75 6e75 7365 642d 6172 6775 6d65  le=unused-argume
+00000830: 6e74 0a20 2020 2020 2020 2076 6572 7369  nt.        versi
+00000840: 6f6e 3a20 4f70 7469 6f6e 616c 5b62 6f6f  on: Optional[boo
+00000850: 6c5d 203d 2074 7970 6572 2e4f 7074 696f  l] = typer.Optio
+00000860: 6e28 0a20 2020 2020 2020 2020 2020 204e  n(.            N
+00000870: 6f6e 652c 0a20 2020 2020 2020 2020 2020  one,.           
+00000880: 2022 2d2d 7665 7273 696f 6e22 2c0a 2020   "--version",.  
+00000890: 2020 2020 2020 2020 2020 6865 6c70 3d22            help="
+000008a0: 5368 6f77 2074 6865 2061 7070 6c69 6361  Show the applica
+000008b0: 7469 6f6e 2773 2076 6572 7369 6f6e 2061  tion's version a
+000008c0: 6e64 2065 7869 742e 222c 0a20 2020 2020  nd exit.",.     
+000008d0: 2020 2020 2020 2063 616c 6c62 6163 6b3d         callback=
+000008e0: 5f76 6572 7369 6f6e 5f63 616c 6c62 6163  _version_callbac
+000008f0: 6b2c 0a20 2020 2020 2020 2020 2020 2069  k,.            i
+00000900: 735f 6561 6765 723d 5472 7565 2c0a 2020  s_eager=True,.  
+00000910: 2020 2020 2020 290a 2920 2d3e 204e 6f6e        ).) -> Non
+00000920: 653a 0a20 2020 2066 2222 220a 2020 2020  e:.    f""".    
+00000930: 7b4e 414d 457d 0a20 2020 2022 2222 0a20  {NAME}.    """. 
+00000940: 2020 2072 6574 7572 6e0a                    return.
```

### Comparing `samples-filter-0.4.1/src/dataset.py` & `samples-filter-0.5.1/src/input.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,54 +17,46 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NON-INFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 """
-Dataset.
+Pipeline input.
 """
 import csv
+from .readme import Readme
 
+class Input:
+    DESTINATION = "pipeline/input.csv"
 
-class Dataset:
-    DESTINATION = "pipeline/dataset.csv"
+    def __init__(self, name):
+        self.name = name
 
-    def __init__(self, where):
-        self.where = where
-
-    """
-    Formulate dataset.
-    """
-    def formulate(self):
-        with open(self.where, "r") as input, open(self.DESTINATION, "w", newline="") as pipe:
+    def copy(self):
+        with open(self.name, "r") as input, open(self.DESTINATION, "w", newline="") as pipe:
             reader = csv.DictReader(input)
             writer = csv.DictWriter(
                 pipe,
                 fieldnames=[
                     "full_name",
+                    "created_at",
                     "description",
-                    "topics",
                     "readme"
                 ]
             )
             writer.writeheader()
-            # @todo #34:60min CSV column 'readme' is too big to read with reader.
-            #  Column that contains readme in some cases is over the limit,
-            #  which is `131072`. It this problem causes exception and
-            #  terminates next row processing. Let's try to compress +
-            #  decompress readme when writing/reading it. Another option can
-            #  be to present the whole dataset in other format, for instance
-            #  JSON. Don't forget to remove this puzzle.
             for row in reader:
                 repo = row["full_name"]
+                branch = row["default_branch"]
+                created = row["created_at"]
                 description = row["description"]
-                topics = row["topics"]
-                readme = row["readme"]
+                readme = Readme(repo, branch).asText()
                 out = {
                     "full_name": repo,
+                    "created_at": created,
                     "description": description,
-                    "topics": topics,
                     "readme": readme
                 }
                 writer.writerow(out)
-                print(f"Prepared dataset for {repo}")
+                print(f"Copied {repo} to {self.DESTINATION}")
+            return self.DESTINATION
```

### Comparing `samples-filter-0.4.1/src/feed.py` & `samples-filter-0.5.1/src/feed.py`

 * *Files 18% similar despite different names*

```diff
@@ -26,19 +26,18 @@
 """
 
 
 class Feed:
     def __init__(self, file):
         self.file = file
 
-    # @todo #105:60min Process all fields required as inputs.
-    #  We should process all fields required as inputs: full_name, readme,
-    #  created_at, last_commit. In case of transformer we should do it in a
-    #  prompt way, like repository advanced description. Check
-    #  <a href="https://github.com/h1alexbel/samples-filter/issues/75#issuecomment-2094153280">this</a>.
+    # @todo #109:90min Feed `readme`, `last_commit`, `created_at`, and `commits`.
+    #  We should feed other important fields too. For now we can feed readme,
+    #  but transformer model can't process it since input tensor is too big.
+    #  Let's resolve that problem and feed readme.
     def read(self):
         with open(self.file, "r") as input:
             csv.field_size_limit(2 * 1024 * 1024 * 1024)
             reader = csv.DictReader(input)
             feed = []
             for row in reader:
                 name = row["full_name"]
```

### Comparing `samples-filter-0.4.1/src/filter_pipe.py` & `samples-filter-0.5.1/src/filter_pipe.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NON-INFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 import csv
 
+from .input import Input
 from .feed import Feed
 from .text_prediction import TextPrediction
 
 """
 Filter pipe.
 """
 
@@ -39,15 +40,15 @@
     # @todo #18:60min Create integration test case for filter_pipe.py.
     #  We should create some sort of integration test that checks filtering
     #  together with model prediction, files creation and other things happening
     #  in #apply(). Don't forget to remove this puzzle.
     def apply(self):
         instance = self.model()
         self.typer.echo(f"Filtering {self.repos} with {instance.name()}...")
-        feed = Feed(self.repos).read()
+        feed = Feed(Input(self.repos).copy()).read()
         with open("predictions.csv", "w") as predictions:
             writer = csv.DictWriter(
                 predictions,
                 fieldnames=["candidate", "input", "prediction", "model"]
             )
             writer.writeheader()
             samples = []
```

### Comparing `samples-filter-0.4.1/src/model_map.py` & `samples-filter-0.5.1/src/model_map.py`

 * *Files identical despite different names*

### Comparing `samples-filter-0.4.1/src/pre_filter.py` & `samples-filter-0.5.1/src/pre_filter.py`

 * *Files identical despite different names*

### Comparing `samples-filter-0.4.1/src/readme.py` & `samples-filter-0.5.1/src/readme.py`

 * *Files identical despite different names*

### Comparing `samples-filter-0.4.1/src/remote_asset.py` & `samples-filter-0.5.1/src/remote_asset.py`

 * *Files identical despite different names*

### Comparing `samples-filter-0.4.1/src/rf_model.py` & `samples-filter-0.5.1/src/rf_model.py`

 * *Files identical despite different names*

### Comparing `samples-filter-0.4.1/src/text_prediction.py` & `samples-filter-0.5.1/src/text_prediction.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 class TextPrediction:
     def __init__(self, pred, name):
         self.pred = pred
         self.model = name
 
     def as_text(self):
         if self.model == "rf":
-            if self.pred == [0]:
+            if self.pred == [1]:
                 label = "sample"
             else:
                 label = "real"
         elif self.pred[0]["label"] == "POSITIVE":
             label = "sample"
         else:
             label = "real"
```

### Comparing `samples-filter-0.4.1/src/transformer_model.py` & `samples-filter-0.5.1/src/transformer_model.py`

 * *Files identical despite different names*

