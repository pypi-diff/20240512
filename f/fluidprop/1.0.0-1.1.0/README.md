# Comparing `tmp/fluidprop-1.0.0.tar.gz` & `tmp/fluidprop-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fluidprop-1.0.0.tar", last modified: Sat May 11 11:09:44 2024, max compression
+gzip compressed data, was "fluidprop-1.1.0.tar", last modified: Sun May 12 12:14:57 2024, max compression
```

## Comparing `fluidprop-1.0.0.tar` & `fluidprop-1.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-11 11:09:44.875564 fluidprop-1.0.0/
--rw-rw-rw-   0        0        0       76 2024-05-11 11:03:33.000000 fluidprop-1.0.0/AUTHORS.rst
--rw-rw-rw-   0        0        0       83 2024-05-11 11:03:34.000000 fluidprop-1.0.0/CHANGELOG.rst
--rw-rw-rw-   0        0        0     1098 2024-05-11 11:03:33.000000 fluidprop-1.0.0/LICENSE.txt
--rw-rw-rw-   0        0        0      289 2020-07-01 17:41:38.000000 fluidprop-1.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     9295 2024-05-11 11:09:44.859939 fluidprop-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     8033 2024-05-11 11:03:33.000000 fluidprop-1.0.0/README.rst
--rw-rw-rw-   0        0        0       42 2024-05-11 11:09:44.875564 fluidprop-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     2349 2024-05-11 11:09:03.000000 fluidprop-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-11 11:09:44.859939 fluidprop-1.0.0/src/
-drwxrwxrwx   0        0        0        0 2024-05-11 11:09:44.859939 fluidprop-1.0.0/src/fluidprop.egg-info/
--rw-rw-rw-   0        0        0     9295 2024-05-11 11:09:44.000000 fluidprop-1.0.0/src/fluidprop.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      306 2024-05-11 11:09:44.000000 fluidprop-1.0.0/src/fluidprop.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-11 11:09:44.000000 fluidprop-1.0.0/src/fluidprop.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-05-10 21:28:56.000000 fluidprop-1.0.0/src/fluidprop.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       26 2024-05-11 11:09:44.000000 fluidprop-1.0.0/src/fluidprop.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-11 11:09:44.000000 fluidprop-1.0.0/src/fluidprop.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    16372 2024-05-11 11:03:33.000000 fluidprop-1.0.0/src/fluidprop.py
+drwxrwxrwx   0        0        0        0 2024-05-12 12:14:57.521348 fluidprop-1.1.0/
+-rw-rw-rw-   0        0        0       76 2024-05-11 11:03:33.000000 fluidprop-1.1.0/AUTHORS.rst
+-rw-rw-rw-   0        0        0      220 2024-05-12 12:04:18.000000 fluidprop-1.1.0/CHANGELOG.rst
+-rw-rw-rw-   0        0        0     1098 2024-05-11 11:03:33.000000 fluidprop-1.1.0/LICENSE.txt
+-rw-rw-rw-   0        0        0      289 2020-07-01 17:41:38.000000 fluidprop-1.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     9690 2024-05-12 12:14:57.520350 fluidprop-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     8291 2024-05-12 12:06:40.000000 fluidprop-1.1.0/README.rst
+-rw-rw-rw-   0        0        0       42 2024-05-12 12:14:57.521348 fluidprop-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     2349 2024-05-12 11:55:11.000000 fluidprop-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-12 12:14:57.514347 fluidprop-1.1.0/src/
+drwxrwxrwx   0        0        0        0 2024-05-12 12:14:57.519348 fluidprop-1.1.0/src/fluidprop.egg-info/
+-rw-rw-rw-   0        0        0     9690 2024-05-12 12:14:57.000000 fluidprop-1.1.0/src/fluidprop.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      306 2024-05-12 12:14:57.000000 fluidprop-1.1.0/src/fluidprop.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-12 12:14:57.000000 fluidprop-1.1.0/src/fluidprop.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-05-10 21:28:56.000000 fluidprop-1.1.0/src/fluidprop.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       26 2024-05-12 12:14:57.000000 fluidprop-1.1.0/src/fluidprop.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-12 12:14:57.000000 fluidprop-1.1.0/src/fluidprop.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    17154 2024-05-12 12:06:46.000000 fluidprop-1.1.0/src/fluidprop.py
```

### Comparing `fluidprop-1.0.0/LICENSE.txt` & `fluidprop-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fluidprop-1.0.0/PKG-INFO` & `fluidprop-1.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fluidprop
-Version: 1.0.0
+Version: 1.1.0
 Summary: Easy access to thermodynamic fluid properties as a function of temperature and pressure. With a minimal command-line interface.
 Home-page: https://github.com/Dennis-van-Gils/python-fluidprop/
 Author: Dennis van Gils
 Author-email: vangils.dennis@gmail.com
 License: MIT
 Project-URL: Issue Tracker, https://github.com/Dennis-van-Gils/python-fluidprop/issues
 Keywords: CoolProp,fluids,thermodynamic
@@ -142,15 +142,17 @@
         Molecular weight       | MW      = 18.01527    g/mol
         Density                | rho     = 9.982e+02   kg/m^3
         Kinematic viscosity    | nu      = 1.003e-06   m^2/s
         Dynamic   viscosity    | eta     = 1.002e-03   kg/(m s)
         Thermal exp. coeff.    | alpha   = 2.068e-04   1/K
         Thermal diffusivity    | kappa   = 1.432e-07   m^2/s
         Thermal conductivity   | lambda_ = 5.980e-01   W/(m K)
-        Isobaric heat capacity | Cp      = 4.184e+03   J/(kg K)
+        Isobaric  heat capac.  | Cp      = 4.184e+03   J/(kg K)
+        Isochoric heat capac.  | Cv      = 4.157e+03   J/(kg K)
+        Isothermal compress.   | comp    = 4.589e-10   1/Pa
         Prandtl                | Pr      = 7.008
     ------------------------------------------------------------
 
 When asked to enter the temperature in ``['C]``, you can *once* enter a single
 character instead to change the input unit to::
 
     k | [K]     Kelvin                  K + 273.15 'C
@@ -206,17 +208,26 @@
 
     kappa   (ndarray): Thermal diffusivity            [m^2/s]
 
     lambda_ (ndarray): Thermal conductivity           [W/(m K)]
 
     Cp      (ndarray): Isobaric heat capacity         [J/(kg K)]
 
+    Cv      (ndarray): Isochoric heat capacity        [J/(kg K)]
+
+    comp    (ndarray): Isothermal compressibility     [1/Pa]
+
     Pr      (ndarray): Prandtl number                 [-]
 
-Dennis van Gils, 11-05-2024
+Dennis van Gils, 12-05-2024
 
 Changelog
 =========
 
+1.1.0 (2024-05-12)
+------------------
+* Added field `Cv`: Isochoric heat capacity
+* Added field `comp`: Isothermal compressibility
+
 1.0.0 (2024-05-11)
 ------------------
 * Initial release
```

### Comparing `fluidprop-1.0.0/README.rst` & `fluidprop-1.1.0/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -114,15 +114,17 @@
         Molecular weight       | MW      = 18.01527    g/mol
         Density                | rho     = 9.982e+02   kg/m^3
         Kinematic viscosity    | nu      = 1.003e-06   m^2/s
         Dynamic   viscosity    | eta     = 1.002e-03   kg/(m s)
         Thermal exp. coeff.    | alpha   = 2.068e-04   1/K
         Thermal diffusivity    | kappa   = 1.432e-07   m^2/s
         Thermal conductivity   | lambda_ = 5.980e-01   W/(m K)
-        Isobaric heat capacity | Cp      = 4.184e+03   J/(kg K)
+        Isobaric  heat capac.  | Cp      = 4.184e+03   J/(kg K)
+        Isochoric heat capac.  | Cv      = 4.157e+03   J/(kg K)
+        Isothermal compress.   | comp    = 4.589e-10   1/Pa
         Prandtl                | Pr      = 7.008
     ------------------------------------------------------------
 
 When asked to enter the temperature in ``['C]``, you can *once* enter a single
 character instead to change the input unit to::
 
     k | [K]     Kelvin                  K + 273.15 'C
@@ -178,10 +180,14 @@
 
     kappa   (ndarray): Thermal diffusivity            [m^2/s]
 
     lambda_ (ndarray): Thermal conductivity           [W/(m K)]
 
     Cp      (ndarray): Isobaric heat capacity         [J/(kg K)]
 
+    Cv      (ndarray): Isochoric heat capacity        [J/(kg K)]
+
+    comp    (ndarray): Isothermal compressibility     [1/Pa]
+
     Pr      (ndarray): Prandtl number                 [-]
 
-Dennis van Gils, 11-05-2024
+Dennis van Gils, 12-05-2024
```

### Comparing `fluidprop-1.0.0/setup.py` & `fluidprop-1.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     ) as fh:
         return fh.read()
 
 
 setup(
     name="fluidprop",
     license="MIT",
-    version="1.0.0",
+    version="1.1.0",
     description="Easy access to thermodynamic fluid properties as a function of temperature and pressure. With a minimal command-line interface.",
     long_description="%s\n%s"
     % (
         re.compile("^.. start-badges.*^.. end-badges", re.M | re.S).sub(
             "", read("README.rst")
         ),
         re.sub(":[a-z]+:`~?(.*?)`", r"``\1``", read("CHANGELOG.rst")),
```

### Comparing `fluidprop-1.0.0/src/fluidprop.egg-info/PKG-INFO` & `fluidprop-1.1.0/src/fluidprop.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fluidprop
-Version: 1.0.0
+Version: 1.1.0
 Summary: Easy access to thermodynamic fluid properties as a function of temperature and pressure. With a minimal command-line interface.
 Home-page: https://github.com/Dennis-van-Gils/python-fluidprop/
 Author: Dennis van Gils
 Author-email: vangils.dennis@gmail.com
 License: MIT
 Project-URL: Issue Tracker, https://github.com/Dennis-van-Gils/python-fluidprop/issues
 Keywords: CoolProp,fluids,thermodynamic
@@ -142,15 +142,17 @@
         Molecular weight       | MW      = 18.01527    g/mol
         Density                | rho     = 9.982e+02   kg/m^3
         Kinematic viscosity    | nu      = 1.003e-06   m^2/s
         Dynamic   viscosity    | eta     = 1.002e-03   kg/(m s)
         Thermal exp. coeff.    | alpha   = 2.068e-04   1/K
         Thermal diffusivity    | kappa   = 1.432e-07   m^2/s
         Thermal conductivity   | lambda_ = 5.980e-01   W/(m K)
-        Isobaric heat capacity | Cp      = 4.184e+03   J/(kg K)
+        Isobaric  heat capac.  | Cp      = 4.184e+03   J/(kg K)
+        Isochoric heat capac.  | Cv      = 4.157e+03   J/(kg K)
+        Isothermal compress.   | comp    = 4.589e-10   1/Pa
         Prandtl                | Pr      = 7.008
     ------------------------------------------------------------
 
 When asked to enter the temperature in ``['C]``, you can *once* enter a single
 character instead to change the input unit to::
 
     k | [K]     Kelvin                  K + 273.15 'C
@@ -206,17 +208,26 @@
 
     kappa   (ndarray): Thermal diffusivity            [m^2/s]
 
     lambda_ (ndarray): Thermal conductivity           [W/(m K)]
 
     Cp      (ndarray): Isobaric heat capacity         [J/(kg K)]
 
+    Cv      (ndarray): Isochoric heat capacity        [J/(kg K)]
+
+    comp    (ndarray): Isothermal compressibility     [1/Pa]
+
     Pr      (ndarray): Prandtl number                 [-]
 
-Dennis van Gils, 11-05-2024
+Dennis van Gils, 12-05-2024
 
 Changelog
 =========
 
+1.1.0 (2024-05-12)
+------------------
+* Added field `Cv`: Isochoric heat capacity
+* Added field `comp`: Isothermal compressibility
+
 1.0.0 (2024-05-11)
 ------------------
 * Initial release
```

### Comparing `fluidprop-1.0.0/src/fluidprop.py` & `fluidprop-1.1.0/src/fluidprop.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 Thermodynamic properties are provided by CoolProp:
 * http://www.coolprop.org/
 * http://pubs.acs.org/doi/abs/10.1021/ie4033999
 """
 __author__ = "Dennis van Gils"
 __authoremail__ = "vangils.dennis@gmail.com"
 __url__ = "https://github.com/Dennis-van-Gils/python-fluidprop"
-__date__ = "11-05-2024"
-__version__ = "1.0.0"
+__date__ = "12-05-2024"
+__version__ = "1.1.0"
 
 import re
 from typing import Union
 
 import numpy.typing as npt
 import numpy as np
 import CoolProp
@@ -118,14 +118,20 @@
 
         lambda_ (`numpy.ndarray[]`):
             Thermal conductivity [W/(m K)].
 
         Cp (`numpy.ndarray[]`):
             Isobaric heat capacity [J/(kg K)].
 
+        Cv (`numpy.ndarray[]`):
+            Isochoric heat capacity [J/(kg K)].
+
+        comp (`numpy.ndarray[]`):
+            Isothermal compressibility [1/Pa].
+
         Pr (`numpy.ndarray[]`):
             Prandtl number.
     """
 
     def __init__(
         self,
         coolprop_name: str,
@@ -203,14 +209,20 @@
 
         self.lambda_: npt.NDArray[np.float64] = np.copy(nan_array)
         """Thermal conductivity [W/(m K)]"""
 
         self.Cp: npt.NDArray[np.float64] = np.copy(nan_array)
         """Isobaric heat capacity [J/(kg K)]"""
 
+        self.Cv: npt.NDArray[np.float64] = np.copy(nan_array)
+        """Isochoric heat capacity [J/(kg K)]"""
+
+        self.comp: npt.NDArray[np.float64] = np.copy(nan_array)
+        """Isothermal compressibility [1/Pa]"""
+
         self.Pr: npt.NDArray[np.float64] = np.copy(nan_array)
         """Prandtl number"""
 
         # ------------------------------
         #   Calculate fluid properties
         # ------------------------------
 
@@ -231,14 +243,16 @@
         # http://coolprop.org/coolprop/HighLevelAPI.html#table-of-string-inputs-to-propssi-function
         requested_quantities = [
             "DMASS",
             "VISCOSITY",
             "ISOBARIC_EXPANSION_COEFFICIENT",
             "CONDUCTIVITY",
             "CPMASS",
+            "CVMASS",
+            "ISOTHERMAL_COMPRESSIBILITY",
             "PRANDTL",
         ]
 
         for idx_, (T, P) in enumerate(zip(self.T, self.P)):
             values = np.zeros(len(requested_quantities))
             values[:] = np.nan
 
@@ -254,14 +268,16 @@
             # fmt: off
             (
                 self.rho[idx_],     # Density                       [kg/m^3]
                 self.eta[idx_],     # Dynamic viscosity             [kg/(m s)]
                 self.alpha[idx_],   # Thermal expansion coefficient [1/K]
                 self.lambda_[idx_], # Thermal conductivity          [W/(m K)]
                 self.Cp[idx_],      # Isobaric heat capacity        [J/(kg K)]
+                self.Cv[idx_],      # Isochoric heat capacity       [J/(kg K)]
+                self.comp[idx_],    # Isothermal compressibility    [1/Pa]
                 self.Pr[idx_],      # Prandtl number                [-]
             ) = values
             # fmt: on
 
         # Derived: Kinematic viscosity [m^2/s]
         self.nu = self.eta / self.rho
         # Derived: Thermal diffusivity [m^2/s]
@@ -288,15 +304,17 @@
                format_spec="f", N_decimals=5)
         pprint("Density"               , "rho"    , self.rho[0]    , "kg/m^3")
         pprint("Kinematic viscosity"   , "nu"     , self.nu[0]     , "m^2/s")
         pprint("Dynamic   viscosity"   , "eta"    , self.eta[0]    , "kg/(m s)")
         pprint("Thermal exp. coeff."   , "alpha"  , self.alpha[0]  , "1/K")
         pprint("Thermal diffusivity"   , "kappa"  , self.kappa[0]  , "m^2/s")
         pprint("Thermal conductivity"  , "lambda_", self.lambda_[0], "W/(m K)")
-        pprint("Isobaric heat capacity", "Cp"     , self.Cp[0]     , "J/(kg K)")
+        pprint("Isobaric  heat capac." , "Cp"     , self.Cp[0]     , "J/(kg K)")
+        pprint("Isochoric heat capac." , "Cv"     , self.Cv[0]     , "J/(kg K)")
+        pprint("Isothermal compress. " , "comp"   , self.comp[0]   , "1/Pa")
         pprint("Prandtl"               , "Pr"     , self.Pr[0]     ,
                format_spec="f")
         # fmt: on
         print(HRULE)
 
 
 # ------------------------------------------------------------------------------
```

