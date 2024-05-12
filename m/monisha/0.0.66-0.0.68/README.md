# Comparing `tmp/monisha-0.0.66.tar.gz` & `tmp/monisha-0.0.68.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monisha-0.0.66.tar", last modified: Sun May  5 06:11:07 2024, max compression
+gzip compressed data, was "monisha-0.0.68.tar", last modified: Sun May 12 11:28:35 2024, max compression
```

## Comparing `monisha-0.0.66.tar` & `monisha-0.0.68.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 06:11:07.303020 monisha-0.0.66/
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-05 06:11:02.000000 monisha-0.0.66/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 06:11:07.299020 monisha-0.0.66/Monisha/
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-05 06:11:02.000000 monisha-0.0.66/Monisha/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 06:11:07.303020 monisha-0.0.66/Monisha/functions/
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-05 06:11:02.000000 monisha-0.0.66/Monisha/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-05-05 06:11:02.000000 monisha-0.0.66/Monisha/functions/function01.py
--rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-05-05 06:11:02.000000 monisha-0.0.66/Monisha/functions/function02.py
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-05-05 06:11:02.000000 monisha-0.0.66/Monisha/functions/function03.py
--rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-05-05 06:11:02.000000 monisha-0.0.66/Monisha/functions/function04.py
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-05 06:11:02.000000 monisha-0.0.66/Monisha/functions/function05.py
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-05-05 06:11:02.000000 monisha-0.0.66/Monisha/functions/function06.py
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-05 06:11:02.000000 monisha-0.0.66/Monisha/functions/function07.py
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-05 06:11:02.000000 monisha-0.0.66/Monisha/functions/function08.py
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-05 06:11:02.000000 monisha-0.0.66/Monisha/functions/function09.py
--rw-r--r--   0 runner    (1001) docker     (127)    60666 2024-05-05 06:11:02.000000 monisha-0.0.66/Monisha/functions/function10.py
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-05 06:11:02.000000 monisha-0.0.66/Monisha/functions/function11.py
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-05-05 06:11:02.000000 monisha-0.0.66/Monisha/functions/function12.py
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-05 06:11:02.000000 monisha-0.0.66/Monisha/functions/function13.py
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-05-05 06:11:02.000000 monisha-0.0.66/Monisha/functions/function14.py
--rw-r--r--   0 runner    (1001) docker     (127)     4654 2024-05-05 06:11:02.000000 monisha-0.0.66/Monisha/functions/function15.py
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-05 06:11:02.000000 monisha-0.0.66/Monisha/functions/function16.py
--rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-05-05 06:11:02.000000 monisha-0.0.66/Monisha/functions/function17.py
--rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-05-05 06:11:02.000000 monisha-0.0.66/Monisha/functions/function18.py
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-05-05 06:11:02.000000 monisha-0.0.66/Monisha/functions/function19.py
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-05 06:11:02.000000 monisha-0.0.66/Monisha/functions/function20.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 06:11:07.303020 monisha-0.0.66/Monisha/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-05 06:11:02.000000 monisha-0.0.66/Monisha/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-05 06:11:02.000000 monisha-0.0.66/Monisha/scripts/en.py
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-05 06:11:02.000000 monisha-0.0.66/Monisha/scripts/eo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-05-05 06:11:02.000000 monisha-0.0.66/Monisha/scripts/es.py
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-05 06:11:02.000000 monisha-0.0.66/Monisha/scripts/eu.py
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-05 06:11:07.303020 monisha-0.0.66/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-05 06:11:02.000000 monisha-0.0.66/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 06:11:07.303020 monisha-0.0.66/monisha.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-05 06:11:07.000000 monisha-0.0.66/monisha.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-05 06:11:07.000000 monisha-0.0.66/monisha.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 06:11:07.000000 monisha-0.0.66/monisha.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-05 06:11:07.000000 monisha-0.0.66/monisha.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-05 06:11:07.000000 monisha-0.0.66/monisha.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 06:11:07.303020 monisha-0.0.66/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-05-05 06:11:02.000000 monisha-0.0.66/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:28:35.221935 monisha-0.0.68/
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-12 11:28:31.000000 monisha-0.0.68/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:28:35.213935 monisha-0.0.68/Monisha/
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-05-12 11:28:31.000000 monisha-0.0.68/Monisha/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:28:35.217935 monisha-0.0.68/Monisha/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-12 11:28:31.000000 monisha-0.0.68/Monisha/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-05-12 11:28:31.000000 monisha-0.0.68/Monisha/functions/function01.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-05-12 11:28:31.000000 monisha-0.0.68/Monisha/functions/function02.py
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-05-12 11:28:31.000000 monisha-0.0.68/Monisha/functions/function03.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-05-12 11:28:31.000000 monisha-0.0.68/Monisha/functions/function04.py
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-12 11:28:31.000000 monisha-0.0.68/Monisha/functions/function05.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-05-12 11:28:31.000000 monisha-0.0.68/Monisha/functions/function06.py
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-12 11:28:31.000000 monisha-0.0.68/Monisha/functions/function07.py
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-12 11:28:31.000000 monisha-0.0.68/Monisha/functions/function08.py
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-12 11:28:31.000000 monisha-0.0.68/Monisha/functions/function09.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60666 2024-05-12 11:28:31.000000 monisha-0.0.68/Monisha/functions/function10.py
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-12 11:28:31.000000 monisha-0.0.68/Monisha/functions/function11.py
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-05-12 11:28:31.000000 monisha-0.0.68/Monisha/functions/function12.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-12 11:28:31.000000 monisha-0.0.68/Monisha/functions/function13.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-05-12 11:28:31.000000 monisha-0.0.68/Monisha/functions/function14.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4654 2024-05-12 11:28:31.000000 monisha-0.0.68/Monisha/functions/function15.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-12 11:28:31.000000 monisha-0.0.68/Monisha/functions/function16.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-05-12 11:28:31.000000 monisha-0.0.68/Monisha/functions/function17.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-05-12 11:28:31.000000 monisha-0.0.68/Monisha/functions/function18.py
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-05-12 11:28:31.000000 monisha-0.0.68/Monisha/functions/function19.py
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-05-12 11:28:31.000000 monisha-0.0.68/Monisha/functions/function20.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:28:35.221935 monisha-0.0.68/Monisha/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-12 11:28:31.000000 monisha-0.0.68/Monisha/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-12 11:28:31.000000 monisha-0.0.68/Monisha/scripts/en.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-12 11:28:31.000000 monisha-0.0.68/Monisha/scripts/eo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-05-12 11:28:31.000000 monisha-0.0.68/Monisha/scripts/es.py
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-12 11:28:31.000000 monisha-0.0.68/Monisha/scripts/eu.py
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-12 11:28:35.221935 monisha-0.0.68/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-12 11:28:31.000000 monisha-0.0.68/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:28:35.221935 monisha-0.0.68/monisha.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-12 11:28:35.000000 monisha-0.0.68/monisha.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-12 11:28:35.000000 monisha-0.0.68/monisha.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 11:28:35.000000 monisha-0.0.68/monisha.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-12 11:28:35.000000 monisha-0.0.68/monisha.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-12 11:28:35.000000 monisha-0.0.68/monisha.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 11:28:35.221935 monisha-0.0.68/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-05-12 11:28:31.000000 monisha-0.0.68/setup.py
```

### Comparing `monisha-0.0.66/LICENSE` & `monisha-0.0.68/LICENSE`

 * *Files identical despite different names*

### Comparing `monisha-0.0.66/Monisha/__init__.py` & `monisha-0.0.68/Monisha/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 appname = "monisha"
-version = "0.0.66"
+version = "0.0.68"
 
-install = ["hachoir"]
+install = ["hachoir",
+           "requests",
+           "beautifulsoup4"]
 
 DATA01 = "clintonabrahamc@gmail.com"
 DATA02 = ['Natural Language :: English',
         'Intended Audience :: Developers',
         'Operating System :: OS Independent',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
```

### Comparing `monisha-0.0.66/Monisha/functions/__init__.py` & `monisha-0.0.68/Monisha/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.66/Monisha/functions/function01.py` & `monisha-0.0.68/Monisha/functions/function01.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,11 +39,11 @@
     hours, minute = divmod(minute, 60)
     days, hours = divmod(hours, 24)
     year, days = divmod(days, 365)
     mos  = ((str(year) + "year, ") if year else Scripted.DATA01)
     mos += ((str(days) + "days, ") if days else Scripted.DATA01)
     mos += ((str(hours) + "hrs, ") if hours else Scripted.DATA01)
     mos += ((str(minute) + "min, ") if minute else Scripted.DATA01)
-    mos += ((str(seconds) + "sec, ") if seconds else Scripted.DATA07)
+    mos += ((str(seconds) + "sec") if seconds else Scripted.DATA07)
     return mos
 
 #=========================================================================
```

### Comparing `monisha-0.0.66/Monisha/functions/function02.py` & `monisha-0.0.68/Monisha/functions/function02.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 from ..scripts import Humon, Scripted
 #=============================================================================
 
 def Dbytes(sizes, second=Scripted.DATA01):
     if not sizes or sizes == Scripted.DATA02 or sizes < 0:
-        return Scripted.DATA09
+        return Scripted.DATA09 + second
     nomos = 0
     POWEO = 1024
     POWER = Humon.DATA01
     while sizes > POWEO:
         sizes /= POWEO
         nomos += 1
-    ouing = str(round(sizes, 2)) + Scripted.DATA02 + POWER[nomos] + second
-    return ouing
+    moonus = str(round(sizes, 2)) + Scripted.DATA02 + POWER[nomos] + second
+    return moonus
 
 #=============================================================================
 
 def Hbytes(sizes, second=Scripted.DATA01):
     if not sizes or sizes == Scripted.DATA02 or sizes < 0:
-        return Scripted.DATA08
+        return Scripted.DATA08 + second
     nomos = 0
     POWEO = 1024
     POWER = Humon.DATA02
     while sizes > POWEO:
         sizes /= POWEO
         nomos += 1
-    ouing = str(round(sizes, 2)) + Scripted.DATA02 + POWER[nomos] + second
-    return ouing
+    moonus = str(round(sizes, 2)) + Scripted.DATA02 + POWER[nomos] + second
+    return moonus
 
 #=============================================================================
 
 def Gbytes(sizes, second=Scripted.DATA01):
     if not sizes or sizes == Scripted.DATA02 or sizes < 0:
-        return Scripted.DATA01
+        return Scripted.DATA01 + second
     nomos = 0
     POWEO = 1024
     POWER = Humon.DATA01
     while sizes > POWEO:
         sizes /= POWEO
         nomos += 1
-    ouing = str(round(sizes, 2)) + Scripted.DATA02 + POWER[nomos] + second
-    return ouing
+    moonus = str(round(sizes, 2)) + Scripted.DATA02 + POWER[nomos] + second
+    return moonus
 
 #=============================================================================
```

### Comparing `monisha-0.0.66/Monisha/functions/function03.py` & `monisha-0.0.68/Monisha/functions/function03.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.66/Monisha/functions/function04.py` & `monisha-0.0.68/Monisha/functions/function04.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.66/Monisha/functions/function06.py` & `monisha-0.0.68/Monisha/functions/function06.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.66/Monisha/functions/function07.py` & `monisha-0.0.68/Monisha/functions/function07.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.66/Monisha/functions/function10.py` & `monisha-0.0.68/Monisha/functions/function10.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.66/Monisha/functions/function14.py` & `monisha-0.0.68/Monisha/functions/function14.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.66/Monisha/functions/function15.py` & `monisha-0.0.68/Monisha/functions/function15.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.66/Monisha/functions/function16.py` & `monisha-0.0.68/Monisha/functions/function16.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.66/Monisha/functions/function17.py` & `monisha-0.0.68/Monisha/functions/function17.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.66/Monisha/functions/function18.py` & `monisha-0.0.68/Monisha/functions/function18.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.66/Monisha/functions/function19.py` & `monisha-0.0.68/Monisha/functions/function19.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.66/Monisha/functions/function20.py` & `monisha-0.0.68/Monisha/functions/function20.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import requests
 from bs4 import BeautifulSoup
-from ..scripts import Links, Scripted
+from ..scripts import Apis, Scripted
 #=======================================================================
 
 class Money:
 
     def convert(money, FROM="USD", TO="INR"):
         moni = float(money)
-        page = requests.get(Links.DATA01.format(FROM, TO))
+        page = requests.get(Apis.DATA01.format(FROM, TO))
         soup = BeautifulSoup(page.text, 'html.parser')
         dat1 = soup.find(class_="ccOutputTrail").previous_sibling
         dat2 = soup.find(class_="ccOutputTrail").get_text(strip=True)
         rate = float(Scripted.DATA12.format(dat1, dat2))
         oumo = round(moni * rate, 2)
         return oumo
```

### Comparing `monisha-0.0.66/Monisha/scripts/es.py` & `monisha-0.0.68/Monisha/scripts/es.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.66/PKG-INFO` & `monisha-0.0.68/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monisha
-Version: 0.0.66
+Version: 0.0.68
 Summary: ㅤ
 Home-page: https://github.com/Clinton-Abraham
 Author: Clinton-Abraham
 Author-email: clintonabrahamc@gmail.com
 License: MIT
 Keywords: python,clinton,abraham
 Classifier: Natural Language :: English
@@ -16,11 +16,13 @@
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Requires-Python: ~=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: hachoir
+Requires-Dist: requests
+Requires-Dist: beautifulsoup4
 
 <p align="center">
  📦 <a href="https://pypi.org/project/monisha" style="text-decoration:none;">MONISHA</a>
 </p>
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
-Metadata-Version: 2.1 Name: monisha Version: 0.0.66 Summary: ã¤ Home-page:
+Metadata-Version: 2.1 Name: monisha Version: 0.0.68 Summary: ã¤ Home-page:
 https://github.com/Clinton-Abraham Author: Clinton-Abraham Author-email:
 clintonabrahamc@gmail.com License: MIT Keywords: python,clinton,abraham
 Classifier: Natural Language :: English Classifier: Intended Audience ::
 Developers Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
 Topic :: Software Development :: Libraries Classifier: Topic :: Software
 Development :: Libraries :: Python Modules Classifier: License :: OSI Approved
 :: GNU Lesser General Public License v3 (LGPLv3) Requires-Python: ~=3.10
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
-hachoir
+hachoir Requires-Dist: requests Requires-Dist: beautifulsoup4
                                  ð¦ _M_O_N_I_S_H_A
```

### Comparing `monisha-0.0.66/monisha.egg-info/PKG-INFO` & `monisha-0.0.68/monisha.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monisha
-Version: 0.0.66
+Version: 0.0.68
 Summary: ㅤ
 Home-page: https://github.com/Clinton-Abraham
 Author: Clinton-Abraham
 Author-email: clintonabrahamc@gmail.com
 License: MIT
 Keywords: python,clinton,abraham
 Classifier: Natural Language :: English
@@ -16,11 +16,13 @@
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Requires-Python: ~=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: hachoir
+Requires-Dist: requests
+Requires-Dist: beautifulsoup4
 
 <p align="center">
  📦 <a href="https://pypi.org/project/monisha" style="text-decoration:none;">MONISHA</a>
 </p>
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
-Metadata-Version: 2.1 Name: monisha Version: 0.0.66 Summary: ã¤ Home-page:
+Metadata-Version: 2.1 Name: monisha Version: 0.0.68 Summary: ã¤ Home-page:
 https://github.com/Clinton-Abraham Author: Clinton-Abraham Author-email:
 clintonabrahamc@gmail.com License: MIT Keywords: python,clinton,abraham
 Classifier: Natural Language :: English Classifier: Intended Audience ::
 Developers Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
 Topic :: Software Development :: Libraries Classifier: Topic :: Software
 Development :: Libraries :: Python Modules Classifier: License :: OSI Approved
 :: GNU Lesser General Public License v3 (LGPLv3) Requires-Python: ~=3.10
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
-hachoir
+hachoir Requires-Dist: requests Requires-Dist: beautifulsoup4
                                  ð¦ _M_O_N_I_S_H_A
```

### Comparing `monisha-0.0.66/monisha.egg-info/SOURCES.txt` & `monisha-0.0.68/monisha.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `monisha-0.0.66/setup.py` & `monisha-0.0.68/setup.py`

 * *Files identical despite different names*

