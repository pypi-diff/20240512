# Comparing `tmp/mrsegmentator-1.0.2.tar.gz` & `tmp/mrsegmentator-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mrsegmentator-1.0.2.tar", last modified: Sun May 12 14:50:24 2024, max compression
+gzip compressed data, was "mrsegmentator-1.0.3.tar", last modified: Sun May 12 15:10:21 2024, max compression
```

## Comparing `mrsegmentator-1.0.2.tar` & `mrsegmentator-1.0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 haha16   (167466) posix-nogroup (100100)        0 2024-05-12 14:50:24.827567 mrsegmentator-1.0.2/
--rw-r--r--   0 haha16   (167466) posix-nogroup (100100)     5561 2024-05-12 14:50:24.823523 mrsegmentator-1.0.2/PKG-INFO
--rw-r--r--   0 haha16   (167466) posix-nogroup (100100)     4531 2024-05-12 14:10:02.000000 mrsegmentator-1.0.2/README.md
--rw-r--r--   0 haha16   (167466) posix-nogroup (100100)       86 2024-02-27 08:52:29.000000 mrsegmentator-1.0.2/pyproject.toml
--rw-r--r--   0 haha16   (167466) posix-nogroup (100100)     1660 2024-05-12 14:50:24.833344 mrsegmentator-1.0.2/setup.cfg
-drwxr-xr-x   0 haha16   (167466) posix-nogroup (100100)        0 2024-05-12 14:50:24.682407 mrsegmentator-1.0.2/src/
-drwxr-xr-x   0 haha16   (167466) posix-nogroup (100100)        0 2024-05-12 14:50:24.755658 mrsegmentator-1.0.2/src/mrsegmentator/
--rw-r--r--   0 haha16   (167466) posix-nogroup (100100)        0 2024-02-27 08:52:29.000000 mrsegmentator-1.0.2/src/mrsegmentator/__init__.py
--rw-r--r--   0 haha16   (167466) posix-nogroup (100100)     4111 2024-05-12 14:10:02.000000 mrsegmentator-1.0.2/src/mrsegmentator/config.py
--rw-r--r--   0 haha16   (167466) posix-nogroup (100100)     4749 2024-05-12 14:10:02.000000 mrsegmentator-1.0.2/src/mrsegmentator/inference.py
--rw-r--r--   0 haha16   (167466) posix-nogroup (100100)     1427 2024-05-12 14:10:02.000000 mrsegmentator-1.0.2/src/mrsegmentator/main.py
--rw-r--r--   0 haha16   (167466) posix-nogroup (100100)     3378 2024-05-12 14:10:02.000000 mrsegmentator-1.0.2/src/mrsegmentator/parser.py
--rw-r--r--   0 haha16   (167466) posix-nogroup (100100)     3236 2024-05-12 14:10:02.000000 mrsegmentator-1.0.2/src/mrsegmentator/simpleitk_reader_writer.py
--rw-r--r--   0 haha16   (167466) posix-nogroup (100100)     2516 2024-05-12 14:10:02.000000 mrsegmentator-1.0.2/src/mrsegmentator/utils.py
-drwxr-xr-x   0 haha16   (167466) posix-nogroup (100100)        0 2024-05-12 14:50:24.814283 mrsegmentator-1.0.2/src/mrsegmentator.egg-info/
--rw-r--r--   0 haha16   (167466) posix-nogroup (100100)     5561 2024-05-12 14:50:24.000000 mrsegmentator-1.0.2/src/mrsegmentator.egg-info/PKG-INFO
--rw-r--r--   0 haha16   (167466) posix-nogroup (100100)      497 2024-05-12 14:50:24.000000 mrsegmentator-1.0.2/src/mrsegmentator.egg-info/SOURCES.txt
--rw-r--r--   0 haha16   (167466) posix-nogroup (100100)        1 2024-05-12 14:50:24.000000 mrsegmentator-1.0.2/src/mrsegmentator.egg-info/dependency_links.txt
--rw-r--r--   0 haha16   (167466) posix-nogroup (100100)       58 2024-05-12 14:50:24.000000 mrsegmentator-1.0.2/src/mrsegmentator.egg-info/entry_points.txt
--rw-r--r--   0 haha16   (167466) posix-nogroup (100100)       25 2024-05-12 14:50:24.000000 mrsegmentator-1.0.2/src/mrsegmentator.egg-info/requires.txt
--rw-r--r--   0 haha16   (167466) posix-nogroup (100100)       14 2024-05-12 14:50:24.000000 mrsegmentator-1.0.2/src/mrsegmentator.egg-info/top_level.txt
+drwxr-xr-x   0 haha16   (167466) posix-nogroup (100100)        0 2024-05-12 15:10:21.020377 mrsegmentator-1.0.3/
+-rw-r--r--   0 haha16   (167466) posix-nogroup (100100)     5561 2024-05-12 15:10:21.016679 mrsegmentator-1.0.3/PKG-INFO
+-rw-r--r--   0 haha16   (167466) posix-nogroup (100100)     4531 2024-05-12 14:10:02.000000 mrsegmentator-1.0.3/README.md
+-rw-r--r--   0 haha16   (167466) posix-nogroup (100100)       86 2024-02-27 08:52:29.000000 mrsegmentator-1.0.3/pyproject.toml
+-rw-r--r--   0 haha16   (167466) posix-nogroup (100100)     1660 2024-05-12 15:10:21.026015 mrsegmentator-1.0.3/setup.cfg
+drwxr-xr-x   0 haha16   (167466) posix-nogroup (100100)        0 2024-05-12 15:10:20.875536 mrsegmentator-1.0.3/src/
+drwxr-xr-x   0 haha16   (167466) posix-nogroup (100100)        0 2024-05-12 15:10:20.950079 mrsegmentator-1.0.3/src/mrsegmentator/
+-rw-r--r--   0 haha16   (167466) posix-nogroup (100100)        0 2024-02-27 08:52:29.000000 mrsegmentator-1.0.3/src/mrsegmentator/__init__.py
+-rw-r--r--   0 haha16   (167466) posix-nogroup (100100)     4088 2024-05-12 15:08:12.000000 mrsegmentator-1.0.3/src/mrsegmentator/config.py
+-rw-r--r--   0 haha16   (167466) posix-nogroup (100100)     4749 2024-05-12 14:10:02.000000 mrsegmentator-1.0.3/src/mrsegmentator/inference.py
+-rw-r--r--   0 haha16   (167466) posix-nogroup (100100)     1427 2024-05-12 14:10:02.000000 mrsegmentator-1.0.3/src/mrsegmentator/main.py
+-rw-r--r--   0 haha16   (167466) posix-nogroup (100100)     3378 2024-05-12 14:10:02.000000 mrsegmentator-1.0.3/src/mrsegmentator/parser.py
+-rw-r--r--   0 haha16   (167466) posix-nogroup (100100)     3236 2024-05-12 14:10:02.000000 mrsegmentator-1.0.3/src/mrsegmentator/simpleitk_reader_writer.py
+-rw-r--r--   0 haha16   (167466) posix-nogroup (100100)     2516 2024-05-12 14:10:02.000000 mrsegmentator-1.0.3/src/mrsegmentator/utils.py
+drwxr-xr-x   0 haha16   (167466) posix-nogroup (100100)        0 2024-05-12 15:10:21.007866 mrsegmentator-1.0.3/src/mrsegmentator.egg-info/
+-rw-r--r--   0 haha16   (167466) posix-nogroup (100100)     5561 2024-05-12 15:10:20.000000 mrsegmentator-1.0.3/src/mrsegmentator.egg-info/PKG-INFO
+-rw-r--r--   0 haha16   (167466) posix-nogroup (100100)      497 2024-05-12 15:10:20.000000 mrsegmentator-1.0.3/src/mrsegmentator.egg-info/SOURCES.txt
+-rw-r--r--   0 haha16   (167466) posix-nogroup (100100)        1 2024-05-12 15:10:20.000000 mrsegmentator-1.0.3/src/mrsegmentator.egg-info/dependency_links.txt
+-rw-r--r--   0 haha16   (167466) posix-nogroup (100100)       58 2024-05-12 15:10:20.000000 mrsegmentator-1.0.3/src/mrsegmentator.egg-info/entry_points.txt
+-rw-r--r--   0 haha16   (167466) posix-nogroup (100100)       25 2024-05-12 15:10:20.000000 mrsegmentator-1.0.3/src/mrsegmentator.egg-info/requires.txt
+-rw-r--r--   0 haha16   (167466) posix-nogroup (100100)       14 2024-05-12 15:10:20.000000 mrsegmentator-1.0.3/src/mrsegmentator.egg-info/top_level.txt
```

### Comparing `mrsegmentator-1.0.2/PKG-INFO` & `mrsegmentator-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mrsegmentator
-Version: 1.0.2
+Version: 1.0.3
 Summary: Robust Multi-Modality Segmentation of 40 Classes in MRI and CT Sequences
 Home-page: https://github.com/hhaentze/mrsegmentator
 Author: Hartmut Häntze
 Author-email: hartmut.haentze@charite.de
 Project-URL: Bug Tracker, https://github.com/hhaentze/mrsegmentator/issues
 Project-URL: repository, https://github.com/hhaentze/mrsegmentator
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mrsegmentator Version: 1.0.2 Summary: Robust Multi-
+Metadata-Version: 2.1 Name: mrsegmentator Version: 1.0.3 Summary: Robust Multi-
 Modality Segmentation of 40 Classes in MRI and CT Sequences Home-page: https://
 github.com/hhaentze/mrsegmentator Author: Hartmut HÃ¤ntze Author-email:
 hartmut.haentze@charite.de Project-URL: Bug Tracker, https://github.com/
 hhaentze/mrsegmentator/issues Project-URL: repository, https://github.com/
 hhaentze/mrsegmentator Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Operating System :: POSIX :: Linux Classifier: Intended Audience :: Developers
```

### Comparing `mrsegmentator-1.0.2/README.md` & `mrsegmentator-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `mrsegmentator-1.0.2/setup.cfg` & `mrsegmentator-1.0.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = mrsegmentator
-version = 1.0.2
+version = 1.0.3
 author = Hartmut Häntze
 author_email = hartmut.haentze@charite.de
 description = Robust Multi-Modality Segmentation of 40 Classes in MRI and CT Sequences
 long_description = file: README.md, LICENSE.txt
 long_description_content_type = text/markdown
 url = https://github.com/hhaentze/mrsegmentator
 project_urls =
```

### Comparing `mrsegmentator-1.0.2/src/mrsegmentator/config.py` & `mrsegmentator-1.0.3/src/mrsegmentator/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,14 @@
     if "MRSEG_WEIGHTS_PATH" in os.environ:
         weights_dir = Path(os.environ["MRSEG_WEIGHTS_PATH"])
     else:
         module_dir = Path(os.path.dirname(__file__))
         weights_dir = module_dir / "weights"
 
     weights_dir.mkdir(exist_ok=True)
-    print(weights_dir)
 
     return weights_dir
 
 
 def read_config():
 
     weights_dir = get_weights_dir()
```

### Comparing `mrsegmentator-1.0.2/src/mrsegmentator/inference.py` & `mrsegmentator-1.0.3/src/mrsegmentator/inference.py`

 * *Files identical despite different names*

### Comparing `mrsegmentator-1.0.2/src/mrsegmentator/main.py` & `mrsegmentator-1.0.3/src/mrsegmentator/main.py`

 * *Files identical despite different names*

### Comparing `mrsegmentator-1.0.2/src/mrsegmentator/parser.py` & `mrsegmentator-1.0.3/src/mrsegmentator/parser.py`

 * *Files identical despite different names*

### Comparing `mrsegmentator-1.0.2/src/mrsegmentator/simpleitk_reader_writer.py` & `mrsegmentator-1.0.3/src/mrsegmentator/simpleitk_reader_writer.py`

 * *Files identical despite different names*

### Comparing `mrsegmentator-1.0.2/src/mrsegmentator/utils.py` & `mrsegmentator-1.0.3/src/mrsegmentator/utils.py`

 * *Files identical despite different names*

### Comparing `mrsegmentator-1.0.2/src/mrsegmentator.egg-info/PKG-INFO` & `mrsegmentator-1.0.3/src/mrsegmentator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mrsegmentator
-Version: 1.0.2
+Version: 1.0.3
 Summary: Robust Multi-Modality Segmentation of 40 Classes in MRI and CT Sequences
 Home-page: https://github.com/hhaentze/mrsegmentator
 Author: Hartmut Häntze
 Author-email: hartmut.haentze@charite.de
 Project-URL: Bug Tracker, https://github.com/hhaentze/mrsegmentator/issues
 Project-URL: repository, https://github.com/hhaentze/mrsegmentator
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mrsegmentator Version: 1.0.2 Summary: Robust Multi-
+Metadata-Version: 2.1 Name: mrsegmentator Version: 1.0.3 Summary: Robust Multi-
 Modality Segmentation of 40 Classes in MRI and CT Sequences Home-page: https://
 github.com/hhaentze/mrsegmentator Author: Hartmut HÃ¤ntze Author-email:
 hartmut.haentze@charite.de Project-URL: Bug Tracker, https://github.com/
 hhaentze/mrsegmentator/issues Project-URL: repository, https://github.com/
 hhaentze/mrsegmentator Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Operating System :: POSIX :: Linux Classifier: Intended Audience :: Developers
```

