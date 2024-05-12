# Comparing `tmp/minebannerlib-0.0.3.tar.gz` & `tmp/minebannerlib-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minebannerlib-0.0.3.tar", last modified: Mon Apr 22 18:54:28 2024, max compression
+gzip compressed data, was "minebannerlib-0.0.5.tar", last modified: Sun May 12 00:05:14 2024, max compression
```

## Comparing `minebannerlib-0.0.3.tar` & `minebannerlib-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,13 @@
-drwxr-xr-x   0 saddy      (501) staff       (20)        0 2024-04-22 18:54:28.940091 minebannerlib-0.0.3/
-drwxr-xr-x   0 saddy      (501) staff       (20)        0 2024-04-22 18:54:28.938975 minebannerlib-0.0.3/MineBannerLib/
--rw-r--r--   0 saddy      (501) staff       (20)     4013 2024-04-22 18:54:04.000000 minebannerlib-0.0.3/MineBannerLib/CreateBanner.py
--rw-r--r--   0 saddy      (501) staff       (20)       27 2024-04-21 16:52:22.000000 minebannerlib-0.0.3/MineBannerLib/__init__.py
--rw-r--r--   0 saddy      (501) staff       (20)     1350 2024-04-22 18:54:28.940025 minebannerlib-0.0.3/PKG-INFO
--rw-r--r--   0 saddy      (501) staff       (20)      744 2024-04-22 18:51:35.000000 minebannerlib-0.0.3/README.md
-drwxr-xr-x   0 saddy      (501) staff       (20)        0 2024-04-22 18:54:28.939781 minebannerlib-0.0.3/minebannerlib.egg-info/
--rw-r--r--   0 saddy      (501) staff       (20)     1350 2024-04-22 18:54:28.000000 minebannerlib-0.0.3/minebannerlib.egg-info/PKG-INFO
--rw-r--r--   0 saddy      (501) staff       (20)      268 2024-04-22 18:54:28.000000 minebannerlib-0.0.3/minebannerlib.egg-info/SOURCES.txt
--rw-r--r--   0 saddy      (501) staff       (20)        1 2024-04-22 18:54:28.000000 minebannerlib-0.0.3/minebannerlib.egg-info/dependency_links.txt
--rw-r--r--   0 saddy      (501) staff       (20)       31 2024-04-22 18:54:28.000000 minebannerlib-0.0.3/minebannerlib.egg-info/requires.txt
--rw-r--r--   0 saddy      (501) staff       (20)       14 2024-04-22 18:54:28.000000 minebannerlib-0.0.3/minebannerlib.egg-info/top_level.txt
--rw-r--r--   0 saddy      (501) staff       (20)       38 2024-04-22 18:54:28.940323 minebannerlib-0.0.3/setup.cfg
--rw-r--r--   0 saddy      (501) staff       (20)      811 2024-04-22 18:54:01.000000 minebannerlib-0.0.3/setup.py
+drwxr-xr-x   0 saddy      (501) staff       (20)        0 2024-05-12 00:05:14.742671 minebannerlib-0.0.5/
+drwxr-xr-x   0 saddy      (501) staff       (20)        0 2024-05-12 00:05:14.741123 minebannerlib-0.0.5/MineBannerLib/
+-rw-r--r--   0 saddy      (501) staff       (20)     4159 2024-05-11 23:44:11.000000 minebannerlib-0.0.5/MineBannerLib/CreateBanner.py
+-rw-r--r--   0 saddy      (501) staff       (20)     1376 2024-05-12 00:05:14.742605 minebannerlib-0.0.5/PKG-INFO
+-rw-r--r--   0 saddy      (501) staff       (20)      738 2024-05-11 23:37:45.000000 minebannerlib-0.0.5/README.md
+drwxr-xr-x   0 saddy      (501) staff       (20)        0 2024-05-12 00:05:14.742316 minebannerlib-0.0.5/minebannerlib.egg-info/
+-rw-r--r--   0 saddy      (501) staff       (20)     1376 2024-05-12 00:05:14.000000 minebannerlib-0.0.5/minebannerlib.egg-info/PKG-INFO
+-rw-r--r--   0 saddy      (501) staff       (20)      242 2024-05-12 00:05:14.000000 minebannerlib-0.0.5/minebannerlib.egg-info/SOURCES.txt
+-rw-r--r--   0 saddy      (501) staff       (20)        1 2024-05-12 00:05:14.000000 minebannerlib-0.0.5/minebannerlib.egg-info/dependency_links.txt
+-rw-r--r--   0 saddy      (501) staff       (20)       48 2024-05-12 00:05:14.000000 minebannerlib-0.0.5/minebannerlib.egg-info/requires.txt
+-rw-r--r--   0 saddy      (501) staff       (20)        1 2024-05-12 00:05:14.000000 minebannerlib-0.0.5/minebannerlib.egg-info/top_level.txt
+-rw-r--r--   0 saddy      (501) staff       (20)       38 2024-05-12 00:05:14.742878 minebannerlib-0.0.5/setup.cfg
+-rw-r--r--   0 saddy      (501) staff       (20)      831 2024-05-11 23:54:47.000000 minebannerlib-0.0.5/setup.py
```

### Comparing `minebannerlib-0.0.3/MineBannerLib/CreateBanner.py` & `minebannerlib-0.0.5/MineBannerLib/CreateBanner.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from nbtlib import parse_nbt
+from multipledispatch import dispatch
 from dataclasses import dataclass
 import enum
 import os
 from PIL import Image, ImageOps
 
 
 pattern = {"b": "base",
@@ -117,20 +118,24 @@
     blue_zero = zero(a[2] / 255.0, b[2] / 255.0, a[3] / 255.0, b[3] / 255.0, alpha_zero)
     return int(red_zero * 255), int(green_zero * 255), int(blue_zero * 255), int(alpha_zero * 255)
 
 def zero(a, b, alpha_a, alpha_b, alpha):
     return (a * alpha_a + b * alpha_b * (1 - alpha_a)) / alpha
 
 
-def getPartsFlag(nbts, clr: int):
+def get_parts_flag_from_nbts(nbts, clr: int):
     comp = parse_nbt(nbts)
     tags = [Layer(pattern='b', color=clr)]
     for i in comp['BlockEntityTag']['Patterns']:
         layer = Layer(pattern=i['Pattern'], color=i['Color'])
         tags.append(layer)
     return tags
 
 
-def create_banner(name: str, json: str, base_color: int):
-    createImg(getPartsFlag(json, base_color), name)
-
-#create_banner('test', '{BlockEntityTag:{Patterns:[{Color:14,Pattern:"cre"},{Color:4,Pattern:"sku"}]}}', 12)
+@dispatch(str, str, int)
+def create_banner(name: str, nbts: str, base_color: int):
+    createImg(get_parts_flag_from_nbts(nbts, base_color), name)
+
+@dispatch(str, list, int)
+def create_banner(name: str, nbts: list, base_color: int):
+    nbts.insert(0, Layer(pattern='b', color=base_color))
+    createImg(nbts, name)
```

### Comparing `minebannerlib-0.0.3/PKG-INFO` & `minebannerlib-0.0.5/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: minebannerlib
-Version: 0.0.3
+Version: 0.0.5
 Summary: Lib for create minecraft banner image
 Home-page: https://github.com/saddydead1/minebannerlib
 Author: saddydead1
 Author-email: saddydead1@gmail.com
 Project-URL: GitHub, https://github.com/saddydead1/minebannerlib
 Keywords: minecraft banner python pil
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 Requires-Dist: requests>=2.25.1
 Requires-Dist: nbtlib
 Requires-Dist: pillow
+Requires-Dist: multipledispatch
 
 # MineBannerLib
 
 Python library for drawing banners.
 
 ## How it works?
 
@@ -41,19 +42,19 @@
 To do this, call the `create_banner()` function, to which you need to pass the _**NBTS**_, _**name of the flag**_ and the _**base color**_
 
 ## Example
 
 ```python
 from MineBannerLib import CreateBanner
 
-banner = CreateBanner
+mbl = CreateBanner
 
 nbts = '{BlockEntityTag:{Patterns:[{Color:14,Pattern:"cre"},{Color:4,Pattern:"sku"}]}}'
 color_base = 15
 name = 'test'
 
 def main():
-  banner.create_banner(name, nbts, color_base)
+  mbl.create_banner(name, nbts, color_base)
 
 if __name__ == '__main__':
   main()
 ```
```

### Comparing `minebannerlib-0.0.3/README.md` & `minebannerlib-0.0.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -23,19 +23,19 @@
 To do this, call the `create_banner()` function, to which you need to pass the _**NBTS**_, _**name of the flag**_ and the _**base color**_
 
 ## Example
 
 ```python
 from MineBannerLib import CreateBanner
 
-banner = CreateBanner
+mbl = CreateBanner
 
 nbts = '{BlockEntityTag:{Patterns:[{Color:14,Pattern:"cre"},{Color:4,Pattern:"sku"}]}}'
 color_base = 15
 name = 'test'
 
 def main():
-  banner.create_banner(name, nbts, color_base)
+  mbl.create_banner(name, nbts, color_base)
 
 if __name__ == '__main__':
   main()
 ```
```

### Comparing `minebannerlib-0.0.3/minebannerlib.egg-info/PKG-INFO` & `minebannerlib-0.0.5/minebannerlib.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: minebannerlib
-Version: 0.0.3
+Version: 0.0.5
 Summary: Lib for create minecraft banner image
 Home-page: https://github.com/saddydead1/minebannerlib
 Author: saddydead1
 Author-email: saddydead1@gmail.com
 Project-URL: GitHub, https://github.com/saddydead1/minebannerlib
 Keywords: minecraft banner python pil
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 Requires-Dist: requests>=2.25.1
 Requires-Dist: nbtlib
 Requires-Dist: pillow
+Requires-Dist: multipledispatch
 
 # MineBannerLib
 
 Python library for drawing banners.
 
 ## How it works?
 
@@ -41,19 +42,19 @@
 To do this, call the `create_banner()` function, to which you need to pass the _**NBTS**_, _**name of the flag**_ and the _**base color**_
 
 ## Example
 
 ```python
 from MineBannerLib import CreateBanner
 
-banner = CreateBanner
+mbl = CreateBanner
 
 nbts = '{BlockEntityTag:{Patterns:[{Color:14,Pattern:"cre"},{Color:4,Pattern:"sku"}]}}'
 color_base = 15
 name = 'test'
 
 def main():
-  banner.create_banner(name, nbts, color_base)
+  mbl.create_banner(name, nbts, color_base)
 
 if __name__ == '__main__':
   main()
 ```
```

### Comparing `minebannerlib-0.0.3/setup.py` & `minebannerlib-0.0.5/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,23 +4,23 @@
 def readme():
   with open('README.md', 'r') as f:
     return f.read()
 
 
 setup(
   name='minebannerlib',
-  version='0.0.3',
+  version='0.0.5',
   author='saddydead1',
   author_email='saddydead1@gmail.com',
   description='Lib for create minecraft banner image',
   long_description=readme(),
   long_description_content_type='text/markdown',
   url='https://github.com/saddydead1/minebannerlib',
   packages=find_packages(),
-  install_requires=['requests>=2.25.1','nbtlib', 'pillow'],
+  install_requires=['requests>=2.25.1','nbtlib', 'pillow', 'multipledispatch'],
   classifiers=[
     'Programming Language :: Python :: 3.11',
     'License :: OSI Approved :: MIT License',
     'Operating System :: OS Independent'
   ],
   keywords='minecraft banner python pil',
   project_urls={
```

