# Comparing `tmp/flameengine-0.0.4.36.tar.gz` & `tmp/flameengine-0.0.4.37.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flameengine-0.0.4.36.tar", last modified: Thu May  9 12:50:53 2024, max compression
+gzip compressed data, was "flameengine-0.0.4.37.tar", last modified: Sun May 12 13:06:42 2024, max compression
```

## Comparing `flameengine-0.0.4.36.tar` & `flameengine-0.0.4.37.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-09 12:50:53.697198 flameengine-0.0.4.36/
--rw-rw-rw-   0        0        0      621 2024-05-09 12:50:53.694199 flameengine-0.0.4.36/PKG-INFO
--rw-rw-rw-   0        0        0       38 2024-05-05 17:14:33.000000 flameengine-0.0.4.36/README.md
-drwxrwxrwx   0        0        0        0 2024-05-09 12:50:53.677498 flameengine-0.0.4.36/flameEngine/
--rw-rw-rw-   0        0        0       39 2024-05-05 17:55:36.000000 flameengine-0.0.4.36/flameEngine/__init__.py
--rw-rw-rw-   0        0        0     1078 2024-05-09 12:49:38.000000 flameengine-0.0.4.36/flameEngine/example.py
--rw-rw-rw-   0        0        0    47546 2024-05-09 12:49:39.000000 flameengine-0.0.4.36/flameEngine/flame.py
-drwxrwxrwx   0        0        0        0 2024-05-09 12:50:53.691986 flameengine-0.0.4.36/flameEngine.egg-info/
--rw-rw-rw-   0        0        0      621 2024-05-09 12:50:53.000000 flameengine-0.0.4.36/flameEngine.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      253 2024-05-09 12:50:53.000000 flameengine-0.0.4.36/flameEngine.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-09 12:50:53.000000 flameengine-0.0.4.36/flameEngine.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-05-09 12:50:53.000000 flameengine-0.0.4.36/flameEngine.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2489 2024-05-05 16:37:14.000000 flameengine-0.0.4.36/license.txt
--rw-rw-rw-   0        0        0       88 2024-05-05 17:13:41.000000 flameengine-0.0.4.36/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-09 12:50:53.697198 flameengine-0.0.4.36/setup.cfg
--rw-rw-rw-   0        0        0      946 2024-05-09 12:50:43.000000 flameengine-0.0.4.36/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-12 13:06:42.149400 flameengine-0.0.4.37/
+-rw-rw-rw-   0        0        0      621 2024-05-12 13:06:42.148242 flameengine-0.0.4.37/PKG-INFO
+-rw-rw-rw-   0        0        0       38 2024-05-05 17:14:33.000000 flameengine-0.0.4.37/README.md
+drwxrwxrwx   0        0        0        0 2024-05-12 13:06:42.139009 flameengine-0.0.4.37/flameEngine/
+-rw-rw-rw-   0        0        0       39 2024-05-05 17:55:36.000000 flameengine-0.0.4.37/flameEngine/__init__.py
+-rw-rw-rw-   0        0        0     1078 2024-05-09 12:49:38.000000 flameengine-0.0.4.37/flameEngine/example.py
+-rw-rw-rw-   0        0        0    47556 2024-05-12 13:06:17.000000 flameengine-0.0.4.37/flameEngine/flame.py
+drwxrwxrwx   0        0        0        0 2024-05-12 13:06:42.146720 flameengine-0.0.4.37/flameEngine.egg-info/
+-rw-rw-rw-   0        0        0      621 2024-05-12 13:06:42.000000 flameengine-0.0.4.37/flameEngine.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      253 2024-05-12 13:06:42.000000 flameengine-0.0.4.37/flameEngine.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-12 13:06:42.000000 flameengine-0.0.4.37/flameEngine.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-05-12 13:06:42.000000 flameengine-0.0.4.37/flameEngine.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2489 2024-05-05 16:37:14.000000 flameengine-0.0.4.37/license.txt
+-rw-rw-rw-   0        0        0       88 2024-05-05 17:13:41.000000 flameengine-0.0.4.37/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-12 13:06:42.149400 flameengine-0.0.4.37/setup.cfg
+-rw-rw-rw-   0        0        0      946 2024-05-12 13:06:36.000000 flameengine-0.0.4.37/setup.py
```

### Comparing `flameengine-0.0.4.36/PKG-INFO` & `flameengine-0.0.4.37/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flameEngine
-Version: 0.0.4.36
+Version: 0.0.4.37
 Summary: Flame simulation package
 Author: Piotr Mikolajczyk
 Author-email: <pio.mikolajczyk@email.com>
 Keywords: python,flameEngine package,flameEngine,flameEngine
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 3
```

### Comparing `flameengine-0.0.4.36/flameEngine/example.py` & `flameengine-0.0.4.37/flameEngine/example.py`

 * *Files identical despite different names*

### Comparing `flameengine-0.0.4.36/flameEngine/flame.py` & `flameengine-0.0.4.37/flameEngine/flame.py`

 * *Files 0% similar despite different names*

```diff
@@ -851,12 +851,12 @@
                                  self.oxidizer_density, self.oxidizer_density_prev,
                                  self.product_density, self.product_density_prev, self.u,
                                  self.u_prev, self.v,
                                  self.v_prev, self.pressure, self.temperature, self.temperature_prev,
                                  self.mass_fuel, self.mass_oxidizer, self.mass_product,
                                  self.poisson_v_term, self.dt,
                                  self.viscosity, self.diff, 0)
-        torch.cuda.empty_cache()
-        import sys
-        sys.modules[__name__].__dict__.clear()
-        import gc
-        gc.collect()
+        # torch.cuda.empty_cache()
+        # import sys
+        # sys.modules[__name__].__dict__.clear()
+        # import gc
+        # gc.collect()
```

### Comparing `flameengine-0.0.4.36/flameEngine.egg-info/PKG-INFO` & `flameengine-0.0.4.37/flameEngine.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flameEngine
-Version: 0.0.4.36
+Version: 0.0.4.37
 Summary: Flame simulation package
 Author: Piotr Mikolajczyk
 Author-email: <pio.mikolajczyk@email.com>
 Keywords: python,flameEngine package,flameEngine,flameEngine
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 3
```

### Comparing `flameengine-0.0.4.36/license.txt` & `flameengine-0.0.4.37/license.txt`

 * *Files identical despite different names*

### Comparing `flameengine-0.0.4.36/setup.py` & `flameengine-0.0.4.37/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.4.36'
+VERSION = '0.0.4.37'
 DESCRIPTION = 'Flame simulation package'
 LONG_DESCRIPTION = 'Simulation engine implementation of stable fluids with extra steps for dataset generation in neural network env and test'
 
 setup(
     name="flameEngine",
     version=VERSION,
     author="Piotr Mikolajczyk",
```

