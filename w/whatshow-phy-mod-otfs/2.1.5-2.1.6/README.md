# Comparing `tmp/whatshow_phy_mod_otfs-2.1.5.tar.gz` & `tmp/whatshow_phy_mod_otfs-2.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whatshow_phy_mod_otfs-2.1.5.tar", last modified: Sun May 12 05:55:33 2024, max compression
+gzip compressed data, was "whatshow_phy_mod_otfs-2.1.6.tar", last modified: Sun May 12 07:23:37 2024, max compression
```

## Comparing `whatshow_phy_mod_otfs-2.1.5.tar` & `whatshow_phy_mod_otfs-2.1.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-12 05:55:33.262412 whatshow_phy_mod_otfs-2.1.5/
--rw-rw-rw-   0        0        0    13032 2024-05-12 05:55:33.259376 whatshow_phy_mod_otfs-2.1.5/PKG-INFO
--rw-rw-rw-   0        0        0    12916 2024-05-12 05:55:32.000000 whatshow_phy_mod_otfs-2.1.5/README.md
--rw-rw-rw-   0        0        0       42 2024-05-12 05:55:33.262412 whatshow_phy_mod_otfs-2.1.5/setup.cfg
--rw-rw-rw-   0        0        0      365 2024-05-12 05:55:32.000000 whatshow_phy_mod_otfs-2.1.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-12 05:55:33.208595 whatshow_phy_mod_otfs-2.1.5/whatshow_phy_mod_otfs/
--rw-rw-rw-   0        0        0    26699 2024-05-12 05:55:32.000000 whatshow_phy_mod_otfs-2.1.5/whatshow_phy_mod_otfs/OTFS.py
--rw-rw-rw-   0        0        0    16003 2024-05-12 05:55:32.000000 whatshow_phy_mod_otfs-2.1.5/whatshow_phy_mod_otfs/OTFSDetector.py
--rw-rw-rw-   0        0        0    28494 2024-05-12 05:55:32.000000 whatshow_phy_mod_otfs-2.1.5/whatshow_phy_mod_otfs/OTFSResGrid.py
--rw-rw-rw-   0        0        0      100 2024-05-12 05:55:32.000000 whatshow_phy_mod_otfs-2.1.5/whatshow_phy_mod_otfs/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-12 05:55:33.257369 whatshow_phy_mod_otfs-2.1.5/whatshow_phy_mod_otfs.egg-info/
--rw-rw-rw-   0        0        0    13032 2024-05-12 05:55:33.000000 whatshow_phy_mod_otfs-2.1.5/whatshow_phy_mod_otfs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      337 2024-05-12 05:55:33.000000 whatshow_phy_mod_otfs-2.1.5/whatshow_phy_mod_otfs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-12 05:55:33.000000 whatshow_phy_mod_otfs-2.1.5/whatshow_phy_mod_otfs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2024-05-12 05:55:33.000000 whatshow_phy_mod_otfs-2.1.5/whatshow_phy_mod_otfs.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-12 07:23:37.386853 whatshow_phy_mod_otfs-2.1.6/
+-rw-rw-rw-   0        0        0    13032 2024-05-12 07:23:37.385002 whatshow_phy_mod_otfs-2.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0    12916 2024-05-12 07:23:36.000000 whatshow_phy_mod_otfs-2.1.6/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-12 07:23:37.386853 whatshow_phy_mod_otfs-2.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      365 2024-05-12 07:23:36.000000 whatshow_phy_mod_otfs-2.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-12 07:23:37.368255 whatshow_phy_mod_otfs-2.1.6/whatshow_phy_mod_otfs/
+-rw-rw-rw-   0        0        0    26551 2024-05-12 07:23:36.000000 whatshow_phy_mod_otfs-2.1.6/whatshow_phy_mod_otfs/OTFS.py
+-rw-rw-rw-   0        0        0    16003 2024-05-12 07:23:36.000000 whatshow_phy_mod_otfs-2.1.6/whatshow_phy_mod_otfs/OTFSDetector.py
+-rw-rw-rw-   0        0        0    28494 2024-05-12 07:23:36.000000 whatshow_phy_mod_otfs-2.1.6/whatshow_phy_mod_otfs/OTFSResGrid.py
+-rw-rw-rw-   0        0        0      100 2024-05-12 07:23:36.000000 whatshow_phy_mod_otfs-2.1.6/whatshow_phy_mod_otfs/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-12 07:23:37.382262 whatshow_phy_mod_otfs-2.1.6/whatshow_phy_mod_otfs.egg-info/
+-rw-rw-rw-   0        0        0    13032 2024-05-12 07:23:37.000000 whatshow_phy_mod_otfs-2.1.6/whatshow_phy_mod_otfs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      337 2024-05-12 07:23:37.000000 whatshow_phy_mod_otfs-2.1.6/whatshow_phy_mod_otfs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-12 07:23:37.000000 whatshow_phy_mod_otfs-2.1.6/whatshow_phy_mod_otfs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2024-05-12 07:23:37.000000 whatshow_phy_mod_otfs-2.1.6/whatshow_phy_mod_otfs.egg-info/top_level.txt
```

### Comparing `whatshow_phy_mod_otfs-2.1.5/PKG-INFO` & `whatshow_phy_mod_otfs-2.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whatshow_phy_mod_otfs
-Version: 2.1.5
+Version: 2.1.6
 Description-Content-Type: text/markdown
 
 # OTFS Modulation
 [![PyPi](https://img.shields.io/badge/PyPi-2.1.5-blue)](https://pypi.org/project/whatshow-phy-mod-otfs/) [![MathWorks](https://img.shields.io/badge/MathWorks-2.1.5-red)](https://mathworks.com/matlabcentral/fileexchange/161136-whatshow_phy_mod_otfs)
 
 This repository is a fundamental toolbox of OTFS modulation crossing `matlab` and `python`. This repositiory is based on papers below:
 > Raviteja, P., Phan, K. T., Hong, Y., & Viterbo, E. (2018). Interference cancellation and iterative detection for orthogonal time frequency space modulation. *IEEE transactions on wireless communications, 17(10)*, 6501-6515.
```

### Comparing `whatshow_phy_mod_otfs-2.1.5/README.md` & `whatshow_phy_mod_otfs-2.1.6/README.md`

 * *Files identical despite different names*

### Comparing `whatshow_phy_mod_otfs-2.1.5/whatshow_phy_mod_otfs/OTFS.py` & `whatshow_phy_mod_otfs-2.1.6/whatshow_phy_mod_otfs/OTFS.py`

 * *Files 2% similar despite different names*

```diff
@@ -447,34 +447,34 @@
             raise Exception("The resource grid is not given.");
         
         #TODO: remove zero padding area
         nans = self.nan(self.sig_len);
         pg_num, pg_delay_beg, pg_delay_end, pg_doppl_beg, pg_doppl_end = self.rg.getAreaPG();
         ce_num, ce_delay_beg, ce_delay_end, ce_doppl_beg, ce_doppl_end = self.rg.getAreaCE();
         # mark redundant values - columns (PG area)
+        col_ids = [];
         if pg_num > 0:
             for doppl_id in range(pg_doppl_beg, pg_doppl_end+1):
                 for delay_id in range(pg_delay_beg, pg_delay_end+1):
                     col_id = doppl_id*self.nSubcarNum + delay_id;
+                    col_ids.append(col_id);
                     H_DD[..., :, col_id] = nans;
         # mark redundant values - rows (CE area)
+        row_ids = [];
         if ce_num > 0:
             for doppl_id in range(ce_doppl_beg,ce_doppl_end+1):
                 for delay_id in range(ce_delay_beg,ce_delay_end+1):
                     row_id = doppl_id*self.nSubcarNum + delay_id;
+                    row_ids.append(row_id);
                     H_DD[..., row_id, :] = nans;
         # remove
         # remove - columns
-        if pg_num > 0:
-            col_idx = self.sum(self.isnan(H_DD)) == self.sig_len;
-            H_DD = np.delete(H_DD, col_idx, axis=-1);
+        H_DD = np.delete(H_DD, col_ids, axis=-1);
         # remove - rows
-        if ce_num > 0:
-            row_idx = self.sum(self.isnan(H_DD), axis=-1) == (self.sig_len - pg_num);
-            H_DD = np.delete(H_DD, row_idx, axis=-2);
+        H_DD = np.delete(H_DD, row_ids, axis=-2);
         return H_DD;
     
     '''
     build the ideal pulse DD channel (callable after modulate)
     @taps_num:  the number of paths
     @his:       the channel gains
     @lis:       the channel delays
@@ -486,21 +486,21 @@
             raise Exception("Cannot build the ideal pulse DD channel while not using ideal pulse.");
         hw = self.zeros(self.nTimeslotNum, self.nSubcarNum).astype(complex);
         H_DD = self.zeros(self.sig_len, self.sig_len).astype(complex);
         for l in range(self.nSubcarNum):
             for k in range(self.nTimeslotNum):
                     for tap_id in range(p):
                         if self.batch_size == self.BATCH_SIZE_NO:
-                            hi = self.chan_coef[tap_id];
-                            li = self.delay_taps[tap_id];
-                            ki = self.doppler_taps[tap_id];
+                            hi = his[tap_id];
+                            li = lis[tap_id];
+                            ki = kis[tap_id];
                         else:
-                            hi = np.expand_dims(self.chan_coef[..., tap_id], axis=-1);
-                            li = np.expand_dims(self.delay_taps[..., tap_id], axis=-1);
-                            ki = np.expand_dims(self.doppler_taps[..., tap_id], axis=-1);
+                            hi = np.expand_dims(his[..., tap_id], axis=-1);
+                            li = np.expand_dims(lis[..., tap_id], axis=-1);
+                            ki = np.expand_dims(kis[..., tap_id], axis=-1);
                         hw_add = 1/self.sig_len*hi*np.exp(-2j*np.pi*li*ki/self.sig_len)* \
                                 np.expand_dims(np.sum(np.exp(2j*np.pi*(l-li)*self.seq(self.nSubcarNum)/self.nSubcarNum), axis=-1), axis=-1)* \
                                 np.expand_dims(np.sum(np.exp(-2j*np.pi*(k-ki)*self.seq(self.nTimeslotNum)/self.nTimeslotNum), axis=-1), axis=-1);
                         if self.batch_size == self.BATCH_SIZE_NO:
                             hw[k, l]= hw[k, l] + hw_add;
                         else:
                             hw[..., k, l]= hw[...,k, l] + self.squeeze(hw_add);
```

### Comparing `whatshow_phy_mod_otfs-2.1.5/whatshow_phy_mod_otfs/OTFSDetector.py` & `whatshow_phy_mod_otfs-2.1.6/whatshow_phy_mod_otfs/OTFSDetector.py`

 * *Files identical despite different names*

### Comparing `whatshow_phy_mod_otfs-2.1.5/whatshow_phy_mod_otfs/OTFSResGrid.py` & `whatshow_phy_mod_otfs-2.1.6/whatshow_phy_mod_otfs/OTFSResGrid.py`

 * *Files identical despite different names*

### Comparing `whatshow_phy_mod_otfs-2.1.5/whatshow_phy_mod_otfs.egg-info/PKG-INFO` & `whatshow_phy_mod_otfs-2.1.6/whatshow_phy_mod_otfs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whatshow-phy-mod-otfs
-Version: 2.1.5
+Version: 2.1.6
 Description-Content-Type: text/markdown
 
 # OTFS Modulation
 [![PyPi](https://img.shields.io/badge/PyPi-2.1.5-blue)](https://pypi.org/project/whatshow-phy-mod-otfs/) [![MathWorks](https://img.shields.io/badge/MathWorks-2.1.5-red)](https://mathworks.com/matlabcentral/fileexchange/161136-whatshow_phy_mod_otfs)
 
 This repository is a fundamental toolbox of OTFS modulation crossing `matlab` and `python`. This repositiory is based on papers below:
 > Raviteja, P., Phan, K. T., Hong, Y., & Viterbo, E. (2018). Interference cancellation and iterative detection for orthogonal time frequency space modulation. *IEEE transactions on wireless communications, 17(10)*, 6501-6515.
```

