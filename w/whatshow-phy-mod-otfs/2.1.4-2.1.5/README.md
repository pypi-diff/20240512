# Comparing `tmp/whatshow_phy_mod_otfs-2.1.4.tar.gz` & `tmp/whatshow_phy_mod_otfs-2.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whatshow_phy_mod_otfs-2.1.4.tar", last modified: Thu May  9 07:22:46 2024, max compression
+gzip compressed data, was "whatshow_phy_mod_otfs-2.1.5.tar", last modified: Sun May 12 05:55:33 2024, max compression
```

## Comparing `whatshow_phy_mod_otfs-2.1.4.tar` & `whatshow_phy_mod_otfs-2.1.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-09 07:22:46.864421 whatshow_phy_mod_otfs-2.1.4/
--rw-rw-rw-   0        0        0    13032 2024-05-09 07:22:46.861335 whatshow_phy_mod_otfs-2.1.4/PKG-INFO
--rw-rw-rw-   0        0        0    12916 2024-05-09 07:22:46.000000 whatshow_phy_mod_otfs-2.1.4/README.md
--rw-rw-rw-   0        0        0       42 2024-05-09 07:22:46.864421 whatshow_phy_mod_otfs-2.1.4/setup.cfg
--rw-rw-rw-   0        0        0      365 2024-05-09 07:22:46.000000 whatshow_phy_mod_otfs-2.1.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-09 07:22:46.788766 whatshow_phy_mod_otfs-2.1.4/whatshow_phy_mod_otfs/
--rw-rw-rw-   0        0        0    26695 2024-05-09 07:22:45.000000 whatshow_phy_mod_otfs-2.1.4/whatshow_phy_mod_otfs/OTFS.py
--rw-rw-rw-   0        0        0    15922 2024-05-09 07:22:46.000000 whatshow_phy_mod_otfs-2.1.4/whatshow_phy_mod_otfs/OTFSDetector.py
--rw-rw-rw-   0        0        0    28494 2024-05-09 07:22:45.000000 whatshow_phy_mod_otfs-2.1.4/whatshow_phy_mod_otfs/OTFSResGrid.py
--rw-rw-rw-   0        0        0      100 2024-05-09 07:22:46.000000 whatshow_phy_mod_otfs-2.1.4/whatshow_phy_mod_otfs/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-09 07:22:46.856574 whatshow_phy_mod_otfs-2.1.4/whatshow_phy_mod_otfs.egg-info/
--rw-rw-rw-   0        0        0    13032 2024-05-09 07:22:46.000000 whatshow_phy_mod_otfs-2.1.4/whatshow_phy_mod_otfs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      337 2024-05-09 07:22:46.000000 whatshow_phy_mod_otfs-2.1.4/whatshow_phy_mod_otfs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-09 07:22:46.000000 whatshow_phy_mod_otfs-2.1.4/whatshow_phy_mod_otfs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2024-05-09 07:22:46.000000 whatshow_phy_mod_otfs-2.1.4/whatshow_phy_mod_otfs.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-12 05:55:33.262412 whatshow_phy_mod_otfs-2.1.5/
+-rw-rw-rw-   0        0        0    13032 2024-05-12 05:55:33.259376 whatshow_phy_mod_otfs-2.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0    12916 2024-05-12 05:55:32.000000 whatshow_phy_mod_otfs-2.1.5/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-12 05:55:33.262412 whatshow_phy_mod_otfs-2.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      365 2024-05-12 05:55:32.000000 whatshow_phy_mod_otfs-2.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-12 05:55:33.208595 whatshow_phy_mod_otfs-2.1.5/whatshow_phy_mod_otfs/
+-rw-rw-rw-   0        0        0    26699 2024-05-12 05:55:32.000000 whatshow_phy_mod_otfs-2.1.5/whatshow_phy_mod_otfs/OTFS.py
+-rw-rw-rw-   0        0        0    16003 2024-05-12 05:55:32.000000 whatshow_phy_mod_otfs-2.1.5/whatshow_phy_mod_otfs/OTFSDetector.py
+-rw-rw-rw-   0        0        0    28494 2024-05-12 05:55:32.000000 whatshow_phy_mod_otfs-2.1.5/whatshow_phy_mod_otfs/OTFSResGrid.py
+-rw-rw-rw-   0        0        0      100 2024-05-12 05:55:32.000000 whatshow_phy_mod_otfs-2.1.5/whatshow_phy_mod_otfs/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-12 05:55:33.257369 whatshow_phy_mod_otfs-2.1.5/whatshow_phy_mod_otfs.egg-info/
+-rw-rw-rw-   0        0        0    13032 2024-05-12 05:55:33.000000 whatshow_phy_mod_otfs-2.1.5/whatshow_phy_mod_otfs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      337 2024-05-12 05:55:33.000000 whatshow_phy_mod_otfs-2.1.5/whatshow_phy_mod_otfs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-12 05:55:33.000000 whatshow_phy_mod_otfs-2.1.5/whatshow_phy_mod_otfs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2024-05-12 05:55:33.000000 whatshow_phy_mod_otfs-2.1.5/whatshow_phy_mod_otfs.egg-info/top_level.txt
```

### Comparing `whatshow_phy_mod_otfs-2.1.4/PKG-INFO` & `whatshow_phy_mod_otfs-2.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: whatshow_phy_mod_otfs
-Version: 2.1.4
+Version: 2.1.5
 Description-Content-Type: text/markdown
 
 # OTFS Modulation
-[![PyPi](https://img.shields.io/badge/PyPi-2.1.4-blue)](https://pypi.org/project/whatshow-phy-mod-otfs/) [![MathWorks](https://img.shields.io/badge/MathWorks-2.1.4-red)](https://mathworks.com/matlabcentral/fileexchange/161136-whatshow_phy_mod_otfs)
+[![PyPi](https://img.shields.io/badge/PyPi-2.1.5-blue)](https://pypi.org/project/whatshow-phy-mod-otfs/) [![MathWorks](https://img.shields.io/badge/MathWorks-2.1.5-red)](https://mathworks.com/matlabcentral/fileexchange/161136-whatshow_phy_mod_otfs)
 
 This repository is a fundamental toolbox of OTFS modulation crossing `matlab` and `python`. This repositiory is based on papers below:
 > Raviteja, P., Phan, K. T., Hong, Y., & Viterbo, E. (2018). Interference cancellation and iterative detection for orthogonal time frequency space modulation. *IEEE transactions on wireless communications, 17(10)*, 6501-6515.
 
 > Raviteja, P., Phan, K. T., & Hong, Y. (2019). Embedded pilot-aided channel estimation for OTFS in delayâ€“Doppler channels. *IEEE transactions on vehicular technology, 68(5)*, 4906-4917.
 
 ## How to use
```

### Comparing `whatshow_phy_mod_otfs-2.1.4/README.md` & `whatshow_phy_mod_otfs-2.1.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # OTFS Modulation
-[![PyPi](https://img.shields.io/badge/PyPi-2.1.4-blue)](https://pypi.org/project/whatshow-phy-mod-otfs/) [![MathWorks](https://img.shields.io/badge/MathWorks-2.1.4-red)](https://mathworks.com/matlabcentral/fileexchange/161136-whatshow_phy_mod_otfs)
+[![PyPi](https://img.shields.io/badge/PyPi-2.1.5-blue)](https://pypi.org/project/whatshow-phy-mod-otfs/) [![MathWorks](https://img.shields.io/badge/MathWorks-2.1.5-red)](https://mathworks.com/matlabcentral/fileexchange/161136-whatshow_phy_mod_otfs)
 
 This repository is a fundamental toolbox of OTFS modulation crossing `matlab` and `python`. This repositiory is based on papers below:
 > Raviteja, P., Phan, K. T., Hong, Y., & Viterbo, E. (2018). Interference cancellation and iterative detection for orthogonal time frequency space modulation. *IEEE transactions on wireless communications, 17(10)*, 6501-6515.
 
 > Raviteja, P., Phan, K. T., & Hong, Y. (2019). Embedded pilot-aided channel estimation for OTFS in delay–Doppler channels. *IEEE transactions on vehicular technology, 68(5)*, 4906-4917.
 
 ## How to use
```

### Comparing `whatshow_phy_mod_otfs-2.1.4/whatshow_phy_mod_otfs/OTFS.py` & `whatshow_phy_mod_otfs-2.1.5/whatshow_phy_mod_otfs/OTFS.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 import numpy as np
 from numpy import floor, sqrt, kron
 from numpy.fft import fft, ifft
 from whatshow_toolbox import MatlabFuncHelper
-from OTFSResGrid import OTFSResGrid
+if '.' not in __name__ :
+    from OTFSResGrid import OTFSResGrid
+else:
+    from .OTFSResGrid import OTFSResGrid
+
 eps = np.finfo(float).eps;
 
 class OTFS(MatlabFuncHelper):
     ###########################################################################
     # Constants
     # Pulse Types
     PULSE_IDEAL = 10;   # ideal pulses (if we use ideal pulses, `ISI_CANCEL_CP` is forced to chosen)
@@ -70,15 +74,15 @@
     
     '''
     modulate (use fast method by default)
     @in1:       an OTFS resource grid or a 2D matrix [Doppler, delay]
     @isFast:    DD domain -> TD domain (no X_TF) 
     '''
     def modulate(self, in1, *, isFast=True):
-        if isinstance(in1, OTFSResGrid) or str(type(in1))=="<class 'whatshow_phy_mod_otfs.OTFSResGrid.OTFSResGrid'>":
+        if isinstance(in1, OTFSResGrid):
             # load RG
             self.nSubcarNum, self.nTimeslotNum = in1.getContentSize();
             self.calcRes();
             self.sig_len = self.nSubcarNum*self.nTimeslotNum;
             if in1.isPulseIdeal():
                 self.pulse_type = self.PULSE_IDEAL;
             elif in1.isPulseRecta():
```

### Comparing `whatshow_phy_mod_otfs-2.1.4/whatshow_phy_mod_otfs/OTFSDetector.py` & `whatshow_phy_mod_otfs-2.1.5/whatshow_phy_mod_otfs/OTFSDetector.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 import numpy as np
 from whatshow_toolbox import MatlabFuncHelper
-from OTFSResGrid import OTFSResGrid
+if '.' not in __name__ :
+    from OTFSResGrid import OTFSResGrid
+else:
+    from .OTFSResGrid import OTFSResGrid
+
 # constants
 pi = np.pi;
 
 class OTFSDetector(MatlabFuncHelper):
     # constants
     # Detect
     DETECT_MP_BASE = 10;                            # base OTFS MP detector proposed by P. Raviteja in 2018
```

### Comparing `whatshow_phy_mod_otfs-2.1.4/whatshow_phy_mod_otfs/OTFSResGrid.py` & `whatshow_phy_mod_otfs-2.1.5/whatshow_phy_mod_otfs/OTFSResGrid.py`

 * *Files identical despite different names*

### Comparing `whatshow_phy_mod_otfs-2.1.4/whatshow_phy_mod_otfs.egg-info/PKG-INFO` & `whatshow_phy_mod_otfs-2.1.5/whatshow_phy_mod_otfs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: whatshow-phy-mod-otfs
-Version: 2.1.4
+Version: 2.1.5
 Description-Content-Type: text/markdown
 
 # OTFS Modulation
-[![PyPi](https://img.shields.io/badge/PyPi-2.1.4-blue)](https://pypi.org/project/whatshow-phy-mod-otfs/) [![MathWorks](https://img.shields.io/badge/MathWorks-2.1.4-red)](https://mathworks.com/matlabcentral/fileexchange/161136-whatshow_phy_mod_otfs)
+[![PyPi](https://img.shields.io/badge/PyPi-2.1.5-blue)](https://pypi.org/project/whatshow-phy-mod-otfs/) [![MathWorks](https://img.shields.io/badge/MathWorks-2.1.5-red)](https://mathworks.com/matlabcentral/fileexchange/161136-whatshow_phy_mod_otfs)
 
 This repository is a fundamental toolbox of OTFS modulation crossing `matlab` and `python`. This repositiory is based on papers below:
 > Raviteja, P., Phan, K. T., Hong, Y., & Viterbo, E. (2018). Interference cancellation and iterative detection for orthogonal time frequency space modulation. *IEEE transactions on wireless communications, 17(10)*, 6501-6515.
 
 > Raviteja, P., Phan, K. T., & Hong, Y. (2019). Embedded pilot-aided channel estimation for OTFS in delayâ€“Doppler channels. *IEEE transactions on vehicular technology, 68(5)*, 4906-4917.
 
 ## How to use
```

