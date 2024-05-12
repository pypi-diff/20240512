# Comparing `tmp/bruhanimate-0.2.8.tar.gz` & `tmp/bruhanimate-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bruhanimate-0.2.8.tar", last modified: Sun Mar 17 06:00:54 2024, max compression
+gzip compressed data, was "bruhanimate-0.2.9.tar", last modified: Sun Mar 17 06:09:47 2024, max compression
```

## Comparing `bruhanimate-0.2.8.tar` & `bruhanimate-0.2.9.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2024-03-17 06:00:54.923338 bruhanimate-0.2.8/
--rw-rw-rw-   0        0        0     2821 2023-11-29 01:09:15.000000 bruhanimate-0.2.8/.gitignore
--rw-rw-rw-   0        0        0    11641 2023-09-16 23:07:43.000000 bruhanimate-0.2.8/COPYING
--rw-rw-rw-   0        0        0    11541 2023-09-16 23:07:43.000000 bruhanimate-0.2.8/LICENSE
--rw-rw-rw-   0        0        0     4720 2024-03-17 06:00:54.922334 bruhanimate-0.2.8/PKG-INFO
--rw-rw-rw-   0        0        0     3809 2024-01-03 23:58:13.000000 bruhanimate-0.2.8/README.md
-drwxrwxrwx   0        0        0        0 2024-03-17 06:00:54.896876 bruhanimate-0.2.8/bruhanimate/
--rw-rw-rw-   0        0        0     1611 2024-03-17 05:59:43.000000 bruhanimate-0.2.8/bruhanimate/__init__.py
--rw-rw-rw-   0        0        0    54656 2024-03-17 05:00:37.000000 bruhanimate-0.2.8/bruhanimate/bruheffects.py
--rw-rw-rw-   0        0        0     6762 2024-03-16 21:15:42.000000 bruhanimate-0.2.8/bruhanimate/bruhffer.py
--rw-rw-rw-   0        0        0    31392 2024-03-17 05:54:09.000000 bruhanimate-0.2.8/bruhanimate/bruhrenderer.py
--rw-rw-rw-   0        0        0    10712 2024-03-17 05:54:10.000000 bruhanimate-0.2.8/bruhanimate/bruhscreen.py
-drwxrwxrwx   0        0        0        0 2024-03-17 06:00:54.920825 bruhanimate-0.2.8/bruhanimate/demos/
--rw-rw-rw-   0        0        0        0 2023-11-21 03:37:40.000000 bruhanimate-0.2.8/bruhanimate/demos/__init__.py
--rw-rw-rw-   0        0        0      601 2024-03-17 05:54:32.000000 bruhanimate-0.2.8/bruhanimate/demos/gol_demo.py
--rw-rw-rw-   0        0        0      613 2024-03-17 05:54:46.000000 bruhanimate-0.2.8/bruhanimate/demos/holiday.py
--rw-rw-rw-   0        0        0     1222 2024-03-17 05:55:00.000000 bruhanimate-0.2.8/bruhanimate/demos/line_demo.py
--rw-rw-rw-   0        0        0      467 2024-03-17 05:55:14.000000 bruhanimate-0.2.8/bruhanimate/demos/matrix_demo.py
--rw-rw-rw-   0        0        0      594 2024-03-17 05:55:26.000000 bruhanimate-0.2.8/bruhanimate/demos/noise_demo.py
--rw-rw-rw-   0        0        0      572 2024-03-17 05:55:35.000000 bruhanimate-0.2.8/bruhanimate/demos/offset_demo.py
--rw-rw-rw-   0        0        0     1003 2024-03-17 05:55:49.000000 bruhanimate-0.2.8/bruhanimate/demos/plasma_demo.py
--rw-rw-rw-   0        0        0      761 2024-03-17 05:55:59.000000 bruhanimate-0.2.8/bruhanimate/demos/rain_demo.py
--rw-rw-rw-   0        0        0      628 2024-03-17 05:56:06.000000 bruhanimate-0.2.8/bruhanimate/demos/snow_demo.py
--rw-rw-rw-   0        0        0      518 2024-03-17 05:56:20.000000 bruhanimate-0.2.8/bruhanimate/demos/stars_demo.py
--rw-rw-rw-   0        0        0      577 2024-03-17 05:56:30.000000 bruhanimate-0.2.8/bruhanimate/demos/static_demo.py
--rw-rw-rw-   0        0        0      554 2024-03-17 05:56:38.000000 bruhanimate-0.2.8/bruhanimate/demos/twinkle_demo.py
--rw-rw-rw-   0        0        0     9997 2024-03-17 04:50:03.000000 bruhanimate-0.2.8/bruhanimate/images.py
-drwxrwxrwx   0        0        0        0 2024-03-17 06:00:54.912454 bruhanimate-0.2.8/bruhanimate.egg-info/
--rw-rw-rw-   0        0        0     4720 2024-03-17 06:00:54.000000 bruhanimate-0.2.8/bruhanimate.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      793 2024-03-17 06:00:54.000000 bruhanimate-0.2.8/bruhanimate.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-17 06:00:54.000000 bruhanimate-0.2.8/bruhanimate.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2024-03-17 06:00:54.000000 bruhanimate-0.2.8/bruhanimate.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-03-17 06:00:54.000000 bruhanimate-0.2.8/bruhanimate.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      571 2023-09-16 23:07:43.000000 bruhanimate-0.2.8/plasma.txt
--rw-rw-rw-   0        0        0       42 2024-03-17 06:00:54.923338 bruhanimate-0.2.8/setup.cfg
--rw-rw-rw-   0        0        0     1367 2024-03-17 05:59:26.000000 bruhanimate-0.2.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-03-17 06:09:47.898412 bruhanimate-0.2.9/
+-rw-rw-rw-   0        0        0     2821 2023-11-29 01:09:15.000000 bruhanimate-0.2.9/.gitignore
+-rw-rw-rw-   0        0        0    11641 2023-09-16 23:07:43.000000 bruhanimate-0.2.9/COPYING
+-rw-rw-rw-   0        0        0    11541 2023-09-16 23:07:43.000000 bruhanimate-0.2.9/LICENSE
+-rw-rw-rw-   0        0        0     4720 2024-03-17 06:09:47.898412 bruhanimate-0.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3809 2024-01-03 23:58:13.000000 bruhanimate-0.2.9/README.md
+drwxrwxrwx   0        0        0        0 2024-03-17 06:09:47.882834 bruhanimate-0.2.9/bruhanimate/
+-rw-rw-rw-   0        0        0     1609 2024-03-17 06:08:29.000000 bruhanimate-0.2.9/bruhanimate/__init__.py
+-rw-rw-rw-   0        0        0    54656 2024-03-17 05:00:37.000000 bruhanimate-0.2.9/bruhanimate/bruheffects.py
+-rw-rw-rw-   0        0        0     6762 2024-03-16 21:15:42.000000 bruhanimate-0.2.9/bruhanimate/bruhffer.py
+-rw-rw-rw-   0        0        0    31392 2024-03-17 05:54:09.000000 bruhanimate-0.2.9/bruhanimate/bruhrenderer.py
+-rw-rw-rw-   0        0        0    10712 2024-03-17 05:54:10.000000 bruhanimate-0.2.9/bruhanimate/bruhscreen.py
+drwxrwxrwx   0        0        0        0 2024-03-17 06:09:47.897405 bruhanimate-0.2.9/bruhanimate/demos/
+-rw-rw-rw-   0        0        0        0 2023-11-21 03:37:40.000000 bruhanimate-0.2.9/bruhanimate/demos/__init__.py
+-rw-rw-rw-   0        0        0      601 2024-03-17 05:54:32.000000 bruhanimate-0.2.9/bruhanimate/demos/gol_demo.py
+-rw-rw-rw-   0        0        0      613 2024-03-17 05:54:46.000000 bruhanimate-0.2.9/bruhanimate/demos/holiday.py
+-rw-rw-rw-   0        0        0     1222 2024-03-17 05:55:00.000000 bruhanimate-0.2.9/bruhanimate/demos/line_demo.py
+-rw-rw-rw-   0        0        0      467 2024-03-17 05:55:14.000000 bruhanimate-0.2.9/bruhanimate/demos/matrix_demo.py
+-rw-rw-rw-   0        0        0      594 2024-03-17 05:55:26.000000 bruhanimate-0.2.9/bruhanimate/demos/noise_demo.py
+-rw-rw-rw-   0        0        0      572 2024-03-17 05:55:35.000000 bruhanimate-0.2.9/bruhanimate/demos/offset_demo.py
+-rw-rw-rw-   0        0        0     1003 2024-03-17 05:55:49.000000 bruhanimate-0.2.9/bruhanimate/demos/plasma_demo.py
+-rw-rw-rw-   0        0        0      761 2024-03-17 05:55:59.000000 bruhanimate-0.2.9/bruhanimate/demos/rain_demo.py
+-rw-rw-rw-   0        0        0      628 2024-03-17 05:56:06.000000 bruhanimate-0.2.9/bruhanimate/demos/snow_demo.py
+-rw-rw-rw-   0        0        0      518 2024-03-17 05:56:20.000000 bruhanimate-0.2.9/bruhanimate/demos/stars_demo.py
+-rw-rw-rw-   0        0        0      577 2024-03-17 05:56:30.000000 bruhanimate-0.2.9/bruhanimate/demos/static_demo.py
+-rw-rw-rw-   0        0        0      554 2024-03-17 05:56:38.000000 bruhanimate-0.2.9/bruhanimate/demos/twinkle_demo.py
+-rw-rw-rw-   0        0        0     9997 2024-03-17 04:50:03.000000 bruhanimate-0.2.9/bruhanimate/images.py
+drwxrwxrwx   0        0        0        0 2024-03-17 06:09:47.888361 bruhanimate-0.2.9/bruhanimate.egg-info/
+-rw-rw-rw-   0        0        0     4720 2024-03-17 06:09:47.000000 bruhanimate-0.2.9/bruhanimate.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      793 2024-03-17 06:09:47.000000 bruhanimate-0.2.9/bruhanimate.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-03-17 06:09:47.000000 bruhanimate-0.2.9/bruhanimate.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2024-03-17 06:09:47.000000 bruhanimate-0.2.9/bruhanimate.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-03-17 06:09:47.000000 bruhanimate-0.2.9/bruhanimate.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      571 2023-09-16 23:07:43.000000 bruhanimate-0.2.9/plasma.txt
+-rw-rw-rw-   0        0        0       42 2024-03-17 06:09:47.899525 bruhanimate-0.2.9/setup.cfg
+-rw-rw-rw-   0        0        0     1367 2024-03-17 06:08:34.000000 bruhanimate-0.2.9/setup.py
```

### Comparing `bruhanimate-0.2.8/.gitignore` & `bruhanimate-0.2.9/.gitignore`

 * *Files identical despite different names*

### Comparing `bruhanimate-0.2.8/COPYING` & `bruhanimate-0.2.9/COPYING`

 * *Files identical despite different names*

### Comparing `bruhanimate-0.2.8/LICENSE` & `bruhanimate-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `bruhanimate-0.2.8/PKG-INFO` & `bruhanimate-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bruhanimate
-Version: 0.2.8
+Version: 0.2.9
 Summary: ASCII Terminal Animation Package
 Home-page: https://github.com/ethanlchristensen/bruhanimate
 Author: Ethan Christensen
 Author-email: ethanlchristensen@outlook.com
 Keywords: python,terminal,terminal-animation,bruhanimate
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `bruhanimate-0.2.8/README.md` & `bruhanimate-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `bruhanimate-0.2.8/bruhanimate/__init__.py` & `bruhanimate-0.2.9/bruhanimate/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,16 +24,16 @@
     PanRenderer,
     FocusRenderer,
     BackgroundColorRenderer,
 )
 from bruhanimate import images
 from bruhanimate.demos import line_demo, plasma_demo, snow_demo, holiday, stars_demo, twinkle_demo, noise_demo, matrix_demo, gol_demo, rain_demo, offset_demo, static_demo
 
-__version__ = "0.2.8"
-__valid_demos__ = [demo.split(".")[0] for demo in os.listdir("./demos") if "init" not in demo and "pycache" not in demo]
+__version__ = "0.2.9"
+__valid_demos__ = [demo.split(".")[0] for demo in os.listdir("demos") if "init" not in demo and "pycache" not in demo]
 
 __all__ = [
     "Screen",
     "plasma_demo",
     "line_demo",
     "holiday",
     "snow_demo",
```

### Comparing `bruhanimate-0.2.8/bruhanimate/bruheffects.py` & `bruhanimate-0.2.9/bruhanimate/bruheffects.py`

 * *Files identical despite different names*

### Comparing `bruhanimate-0.2.8/bruhanimate/bruhffer.py` & `bruhanimate-0.2.9/bruhanimate/bruhffer.py`

 * *Files identical despite different names*

### Comparing `bruhanimate-0.2.8/bruhanimate/bruhrenderer.py` & `bruhanimate-0.2.9/bruhanimate/bruhrenderer.py`

 * *Files identical despite different names*

### Comparing `bruhanimate-0.2.8/bruhanimate/bruhscreen.py` & `bruhanimate-0.2.9/bruhanimate/bruhscreen.py`

 * *Files identical despite different names*

### Comparing `bruhanimate-0.2.8/bruhanimate/demos/gol_demo.py` & `bruhanimate-0.2.9/bruhanimate/demos/gol_demo.py`

 * *Files identical despite different names*

### Comparing `bruhanimate-0.2.8/bruhanimate/demos/holiday.py` & `bruhanimate-0.2.9/bruhanimate/demos/holiday.py`

 * *Files identical despite different names*

### Comparing `bruhanimate-0.2.8/bruhanimate/demos/line_demo.py` & `bruhanimate-0.2.9/bruhanimate/demos/line_demo.py`

 * *Files identical despite different names*

### Comparing `bruhanimate-0.2.8/bruhanimate/demos/noise_demo.py` & `bruhanimate-0.2.9/bruhanimate/demos/noise_demo.py`

 * *Files identical despite different names*

### Comparing `bruhanimate-0.2.8/bruhanimate/demos/offset_demo.py` & `bruhanimate-0.2.9/bruhanimate/demos/offset_demo.py`

 * *Files identical despite different names*

### Comparing `bruhanimate-0.2.8/bruhanimate/demos/plasma_demo.py` & `bruhanimate-0.2.9/bruhanimate/demos/plasma_demo.py`

 * *Files identical despite different names*

### Comparing `bruhanimate-0.2.8/bruhanimate/demos/rain_demo.py` & `bruhanimate-0.2.9/bruhanimate/demos/rain_demo.py`

 * *Files identical despite different names*

### Comparing `bruhanimate-0.2.8/bruhanimate/demos/snow_demo.py` & `bruhanimate-0.2.9/bruhanimate/demos/snow_demo.py`

 * *Files identical despite different names*

### Comparing `bruhanimate-0.2.8/bruhanimate/demos/stars_demo.py` & `bruhanimate-0.2.9/bruhanimate/demos/stars_demo.py`

 * *Files identical despite different names*

### Comparing `bruhanimate-0.2.8/bruhanimate/demos/static_demo.py` & `bruhanimate-0.2.9/bruhanimate/demos/static_demo.py`

 * *Files identical despite different names*

### Comparing `bruhanimate-0.2.8/bruhanimate/demos/twinkle_demo.py` & `bruhanimate-0.2.9/bruhanimate/demos/twinkle_demo.py`

 * *Files identical despite different names*

### Comparing `bruhanimate-0.2.8/bruhanimate/images.py` & `bruhanimate-0.2.9/bruhanimate/images.py`

 * *Files identical despite different names*

### Comparing `bruhanimate-0.2.8/bruhanimate.egg-info/PKG-INFO` & `bruhanimate-0.2.9/bruhanimate.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bruhanimate
-Version: 0.2.8
+Version: 0.2.9
 Summary: ASCII Terminal Animation Package
 Home-page: https://github.com/ethanlchristensen/bruhanimate
 Author: Ethan Christensen
 Author-email: ethanlchristensen@outlook.com
 Keywords: python,terminal,terminal-animation,bruhanimate
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `bruhanimate-0.2.8/bruhanimate.egg-info/SOURCES.txt` & `bruhanimate-0.2.9/bruhanimate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bruhanimate-0.2.8/plasma.txt` & `bruhanimate-0.2.9/plasma.txt`

 * *Files identical despite different names*

### Comparing `bruhanimate-0.2.8/setup.py` & `bruhanimate-0.2.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import sys
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.2.8'
+VERSION = '0.2.9'
 DESCRIPTION = 'ASCII Terminal Animation Package'
 LONG_DESCRIPTION = 'A package that allows for various animations in the terminal'
 
 # Setting up
 setup(
     name="bruhanimate",
     version=VERSION,
```

