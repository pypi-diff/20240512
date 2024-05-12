# Comparing `tmp/specpolFlow-0.3.4.tar.gz` & `tmp/specpolflow-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "specpolFlow-0.3.4.tar", last modified: Sat Apr 13 04:12:18 2024, max compression
+gzip compressed data, was "specpolflow-0.4.0.tar", last modified: Sun May 12 00:33:33 2024, max compression
```

## Comparing `specpolFlow-0.3.4.tar` & `specpolflow-0.4.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2024-04-13 04:12:18.632286 specpolFlow-0.3.4/
--rw-rw-r--   0 colin     (1000) colin     (1000)    18092 2022-06-10 18:49:06.000000 specpolFlow-0.3.4/LICENSE
--rw-r--r--   0 colin     (1000) colin     (1000)     3336 2024-04-13 04:12:18.632286 specpolFlow-0.3.4/PKG-INFO
--rw-rw-r--   0 colin     (1000) colin     (1000)     2491 2024-04-13 03:59:50.000000 specpolFlow-0.3.4/README.md
--rw-rw-r--   0 colin     (1000) colin     (1000)     1607 2024-04-13 02:17:02.000000 specpolFlow-0.3.4/pyproject.toml
--rw-rw-r--   0 colin     (1000) colin     (1000)       38 2024-04-13 04:12:18.632286 specpolFlow-0.3.4/setup.cfg
-drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2024-04-13 04:12:18.628286 specpolFlow-0.3.4/specpolFlow/
-drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2024-04-13 04:12:18.632286 specpolFlow-0.3.4/specpolFlow/CommandLine/
--rw-rw-r--   0 colin     (1000) colin     (1000)        0 2024-03-13 20:56:33.000000 specpolFlow-0.3.4/specpolFlow/CommandLine/__init__.py
--rwxrwxr-x   0 colin     (1000) colin     (1000)     4650 2024-03-15 22:20:13.000000 specpolFlow-0.3.4/specpolFlow/CommandLine/bz.py
--rwxrwxr-x   0 colin     (1000) colin     (1000)     2158 2024-03-15 22:24:26.000000 specpolFlow-0.3.4/specpolFlow/CommandLine/cleanMaskUI.py
--rwxrwxr-x   0 colin     (1000) colin     (1000)     3199 2024-03-15 22:25:02.000000 specpolFlow-0.3.4/specpolFlow/CommandLine/makeMask.py
--rwxrwxr-x   0 colin     (1000) colin     (1000)     1819 2024-03-15 22:20:41.000000 specpolFlow-0.3.4/specpolFlow/CommandLine/plotLSD.py
--rwxrwxr-x   0 colin     (1000) colin     (1000)     2093 2024-03-15 22:20:52.000000 specpolFlow-0.3.4/specpolFlow/CommandLine/rvFit.py
--rw-rw-r--   0 colin     (1000) colin     (1000)      179 2024-03-27 20:03:58.000000 specpolFlow-0.3.4/specpolFlow/__init__.py
--rw-rw-r--   0 colin     (1000) colin     (1000)     5218 2023-11-12 06:43:08.000000 specpolFlow-0.3.4/specpolFlow/cleanMaskUI.py
--rw-rw-r--   0 colin     (1000) colin     (1000)    58511 2023-10-24 00:52:17.000000 specpolFlow-0.3.4/specpolFlow/cleanMaskUISubroutines.py
-drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2024-04-13 04:12:18.632286 specpolFlow-0.3.4/specpolFlow/converters/
--rw-rw-r--   0 colin     (1000) colin     (1000)       23 2023-10-24 00:52:17.000000 specpolFlow-0.3.4/specpolFlow/converters/__init__.py
--rw-rw-r--   0 colin     (1000) colin     (1000)     7530 2023-05-25 16:03:53.000000 specpolFlow-0.3.4/specpolFlow/converters/convert-spirou-fits-s0.2.py
--rw-rw-r--   0 colin     (1000) colin     (1000)     5539 2024-03-27 20:03:58.000000 specpolFlow-0.3.4/specpolFlow/converters/espadons.py
--rw-rw-r--   0 colin     (1000) colin     (1000)    26745 2023-11-12 05:42:08.000000 specpolFlow-0.3.4/specpolFlow/lineList.py
--rw-rw-r--   0 colin     (1000) colin     (1000)    24183 2024-03-16 02:04:01.000000 specpolFlow-0.3.4/specpolFlow/mask.py
--rw-rw-r--   0 colin     (1000) colin     (1000)     8544 2023-11-12 05:42:21.000000 specpolFlow-0.3.4/specpolFlow/obsSpec.py
--rw-rw-r--   0 colin     (1000) colin     (1000)    39882 2024-03-13 20:59:04.000000 specpolFlow-0.3.4/specpolFlow/profileLSD.py
-drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2024-04-13 04:12:18.632286 specpolFlow-0.3.4/specpolFlow.egg-info/
--rw-r--r--   0 colin     (1000) colin     (1000)     3336 2024-04-13 04:12:18.000000 specpolFlow-0.3.4/specpolFlow.egg-info/PKG-INFO
--rw-rw-r--   0 colin     (1000) colin     (1000)      756 2024-04-13 04:12:18.000000 specpolFlow-0.3.4/specpolFlow.egg-info/SOURCES.txt
--rw-rw-r--   0 colin     (1000) colin     (1000)        1 2024-04-13 04:12:18.000000 specpolFlow-0.3.4/specpolFlow.egg-info/dependency_links.txt
--rw-rw-r--   0 colin     (1000) colin     (1000)      361 2024-04-13 04:12:18.000000 specpolFlow-0.3.4/specpolFlow.egg-info/entry_points.txt
--rw-rw-r--   0 colin     (1000) colin     (1000)       54 2024-04-13 04:12:18.000000 specpolFlow-0.3.4/specpolFlow.egg-info/requires.txt
--rw-rw-r--   0 colin     (1000) colin     (1000)       12 2024-04-13 04:12:18.000000 specpolFlow-0.3.4/specpolFlow.egg-info/top_level.txt
+drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2024-05-12 00:33:33.866972 specpolflow-0.4.0/
+-rw-rw-r--   0 colin     (1000) colin     (1000)    18092 2022-06-10 18:49:06.000000 specpolflow-0.4.0/LICENSE
+-rw-r--r--   0 colin     (1000) colin     (1000)     3336 2024-05-12 00:33:33.866972 specpolflow-0.4.0/PKG-INFO
+-rw-rw-r--   0 colin     (1000) colin     (1000)     2491 2024-04-13 03:59:50.000000 specpolflow-0.4.0/README.md
+-rw-rw-r--   0 colin     (1000) colin     (1000)     1607 2024-05-11 17:51:30.000000 specpolflow-0.4.0/pyproject.toml
+-rw-rw-r--   0 colin     (1000) colin     (1000)       38 2024-05-12 00:33:33.866972 specpolflow-0.4.0/setup.cfg
+drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2024-05-12 00:33:33.866972 specpolflow-0.4.0/specpolFlow/
+drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2024-05-12 00:33:33.866972 specpolflow-0.4.0/specpolFlow/CommandLine/
+-rw-rw-r--   0 colin     (1000) colin     (1000)        0 2024-03-13 20:56:33.000000 specpolflow-0.4.0/specpolFlow/CommandLine/__init__.py
+-rwxrwxr-x   0 colin     (1000) colin     (1000)     4650 2024-03-15 22:20:13.000000 specpolflow-0.4.0/specpolFlow/CommandLine/bz.py
+-rwxrwxr-x   0 colin     (1000) colin     (1000)     2343 2024-05-11 04:23:30.000000 specpolflow-0.4.0/specpolFlow/CommandLine/cleanMaskUI.py
+-rwxrwxr-x   0 colin     (1000) colin     (1000)     3170 2024-05-11 18:22:22.000000 specpolflow-0.4.0/specpolFlow/CommandLine/makeMask.py
+-rwxrwxr-x   0 colin     (1000) colin     (1000)     1820 2024-05-10 20:30:57.000000 specpolflow-0.4.0/specpolFlow/CommandLine/plotLSD.py
+-rwxrwxr-x   0 colin     (1000) colin     (1000)     2093 2024-03-15 22:20:52.000000 specpolflow-0.4.0/specpolFlow/CommandLine/rvFit.py
+-rw-rw-r--   0 colin     (1000) colin     (1000)      179 2024-05-11 17:51:42.000000 specpolflow-0.4.0/specpolFlow/__init__.py
+-rw-rw-r--   0 colin     (1000) colin     (1000)     6048 2024-05-11 05:01:55.000000 specpolflow-0.4.0/specpolFlow/cleanMaskUI.py
+-rw-rw-r--   0 colin     (1000) colin     (1000)    58136 2024-05-11 04:58:30.000000 specpolflow-0.4.0/specpolFlow/cleanMaskUISubroutines.py
+drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2024-05-12 00:33:33.866972 specpolflow-0.4.0/specpolFlow/converters/
+-rw-rw-r--   0 colin     (1000) colin     (1000)       23 2023-10-24 00:52:17.000000 specpolflow-0.4.0/specpolFlow/converters/__init__.py
+-rw-rw-r--   0 colin     (1000) colin     (1000)     7530 2023-05-25 16:03:53.000000 specpolflow-0.4.0/specpolFlow/converters/convert-spirou-fits-s0.2.py
+-rw-rw-r--   0 colin     (1000) colin     (1000)     6293 2024-05-10 20:30:57.000000 specpolflow-0.4.0/specpolFlow/converters/espadons.py
+-rw-rw-r--   0 colin     (1000) colin     (1000)    26719 2024-05-10 20:30:57.000000 specpolflow-0.4.0/specpolFlow/lineList.py
+-rw-rw-r--   0 colin     (1000) colin     (1000)    24221 2024-05-11 18:18:52.000000 specpolflow-0.4.0/specpolFlow/mask.py
+-rw-rw-r--   0 colin     (1000) colin     (1000)    22255 2024-05-10 20:30:57.000000 specpolflow-0.4.0/specpolFlow/obsSpec.py
+-rw-rw-r--   0 colin     (1000) colin     (1000)    46978 2024-05-11 23:55:29.000000 specpolflow-0.4.0/specpolFlow/profileLSD.py
+drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2024-05-12 00:33:33.866972 specpolflow-0.4.0/specpolFlow.egg-info/
+-rw-r--r--   0 colin     (1000) colin     (1000)     3336 2024-05-12 00:33:33.000000 specpolflow-0.4.0/specpolFlow.egg-info/PKG-INFO
+-rw-rw-r--   0 colin     (1000) colin     (1000)      756 2024-05-12 00:33:33.000000 specpolflow-0.4.0/specpolFlow.egg-info/SOURCES.txt
+-rw-rw-r--   0 colin     (1000) colin     (1000)        1 2024-05-12 00:33:33.000000 specpolflow-0.4.0/specpolFlow.egg-info/dependency_links.txt
+-rw-rw-r--   0 colin     (1000) colin     (1000)      361 2024-05-12 00:33:33.000000 specpolflow-0.4.0/specpolFlow.egg-info/entry_points.txt
+-rw-rw-r--   0 colin     (1000) colin     (1000)       54 2024-05-12 00:33:33.000000 specpolflow-0.4.0/specpolFlow.egg-info/requires.txt
+-rw-rw-r--   0 colin     (1000) colin     (1000)       12 2024-05-12 00:33:33.000000 specpolflow-0.4.0/specpolFlow.egg-info/top_level.txt
```

### Comparing `specpolFlow-0.3.4/LICENSE` & `specpolflow-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `specpolFlow-0.3.4/PKG-INFO` & `specpolflow-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: specpolFlow
-Version: 0.3.4
+Version: 0.4.0
 Summary: Tools for the analysis of stellar spectropolarimetric data
 Author-email: SpecpolFlow Team <specpolflow@gmail.com>
 Project-URL: Homepage, https://github.com/folsomcp/specpolFlow
 Project-URL: Documentation, https://folsomcp.github.io/specpolFlow/
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Astronomy
```

### Comparing `specpolFlow-0.3.4/README.md` & `specpolflow-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `specpolFlow-0.3.4/pyproject.toml` & `specpolflow-0.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 [tool.setuptools.packages.find]
 # All the following settings are optional:
 #where = ["src"]  # ["."] by default
 include = ["specpolFlow*"]  # ["*"] by default
 
 [project]
 name = "specpolFlow"
-version = "0.3.4"
+version = "0.4.0"
 authors = [ {name="SpecpolFlow Team", email="specpolflow@gmail.com"},
 ]
 description = "Tools for the analysis of stellar spectropolarimetric data"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Development Status :: 3 - Alpha",
```

### Comparing `specpolFlow-0.3.4/specpolFlow/CommandLine/bz.py` & `specpolflow-0.4.0/specpolFlow/CommandLine/bz.py`

 * *Files identical despite different names*

### Comparing `specpolFlow-0.3.4/specpolFlow/CommandLine/cleanMaskUI.py` & `specpolflow-0.4.0/specpolFlow/CommandLine/cleanMaskUI.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 #!/usr/bin/python3
-## @module cleanMaskUI.py
 #
-#Interactive tool for cleaning poor lines from an LSD line mask
+# Interactive tool for cleaning poor lines from an LSD line mask
+# also can fit line depths in the mask.
 
 import argparse
 
 try:
     import specpolFlow as pol
 except ModuleNotFoundError:
     #If specpolFlow is not installed or in the python path
     #try guessing the location and adding it temporarily
     import sys, os
     loc0 = os.path.dirname(__file__)
     sys.path.insert(0, os.path.join(loc0, '..', '..'))
     import specpolFlow as pol
 
 def clean_mask_cli():
-    """Main function for running cleanMaskUI as a terminal program
+    """Main function for running cleanMaskUI as a terminal program.
     """
     parser = argparse.ArgumentParser(description='Interactively remove poor lines from an LSD line mask, and optionally modify line depths. This plots the mask, a comparison observation, and the model LSD spectrum (the convolution of the mask and LSD profile). For the model LSD spectrum calculation, some more useful parameters can be set within the graphical UI, and there is an option for displaying the resulting profile.')
     parser.add_argument('mask', help='The line mask to clean')
     parser.add_argument('observation', help='An observed spectrum for comparison')
     parser.add_argument('outName', nargs='?', default=None, help='Optional name for the output cleaned line mask, defaults to [input_file_name].clean')
     parser.add_argument('-e', '--exclude', default='excludeRanges.dat', help='Optional, a file of wavelength ranges to exclude from the line mask.  If the file does not exist default initial values will be used.')
     parser.add_argument('-b', '--batch', action='store_true', help='Run in batch mode, just apply the exclude regions from file, skip the interactive UI and LSD calculations.')
@@ -28,15 +28,17 @@
 
     maskName = args.mask
     obsName = args.observation
     outMaskName = args.outName
     excludeFileName = args.exclude
     batchMode = args.batch
     
-    cleanMask = pol.cleanMaskUI(maskName, obsName, outMaskName=outMaskName,
-                                excludeFileName=excludeFileName,
-                                batchMode=batchMode)
+    cleanMask, excludeRanges = pol.cleanMaskUI(maskName, obsName,
+                                               outMaskName=outMaskName,
+                                               inExcludeName=excludeFileName,
+                                               outExcludeName=excludeFileName,
+                                               batchMode=batchMode)
     return
 
 #For running this Python script as a terminal program
 if __name__ == "__main__":
     clean_mask_cli()
```

### Comparing `specpolFlow-0.3.4/specpolFlow/CommandLine/makeMask.py` & `specpolflow-0.4.0/specpolFlow/CommandLine/makeMask.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     import sys, os
     loc0 = os.path.dirname(__file__) 
     sys.path.insert(0, os.path.join(loc0, '..', '..'))
     import specpolFlow as pol
 
 def make_mask_cli():
     """
-    Main function for running make_mask as a terminal program
+    Main function for running make_mask as a terminal program.
 
     Takes no arguments, but uses command line parameters instead.
     """
     #Take input and output file names as command line arguments,
     #with some additional optional control parameters.
     parser = argparse.ArgumentParser(description='Generate an LSD line mask from a VALD line list. When Lande factors are not in the line list they will be estimated if possible.')
     parser.add_argument("lineList", help="Line list from VALD. This file should be an 'extract stellar' line list in the 'long' format.")
@@ -41,19 +41,19 @@
     lande1 = float(args.g1)
     lande2 = float(args.g2)
     elementsUsed = args.elements.split()
     elementsExclude = args.excludeEl.split()
     
     #Run the line mask generating code
     print('reading line list from', llistName)
-    mask = pol.make_mask(llistName, maskName, depthCutoff = depthCutoff,
-                                  wlStart = wl1, wlEnd = wl2,
-                                  landeStart = lande1, landeEnd = lande2,
-                                  elementsUsed = elementsUsed,
-                                  elementsExclude = elementsExclude,
-                                  includeNoLande = False)
+    mask = pol.make_mask(llistName, outMaskName = maskName, 
+                         depthCutoff = depthCutoff, wlStart = wl1, wlEnd = wl2,
+                         landeStart = lande1, landeEnd = lande2,
+                         elementsUsed = elementsUsed,
+                         elementsExclude = elementsExclude,
+                         includeNoLande = False)
     print('mask saved to', maskName)
     return
 
 #For running this script as a terminal program
 if __name__ == "__main__":
     make_mask_cli()
```

### Comparing `specpolFlow-0.3.4/specpolFlow/CommandLine/plotLSD.py` & `specpolflow-0.4.0/specpolFlow/CommandLine/plotLSD.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     import sys, os
     loc0 = os.path.dirname(__file__) 
     sys.path.insert(0, os.path.join(loc0, '..', '..'))
     import specpolFlow as pol
 
 def plot_lsd_cli():
     """
-    Function for quickly reading and plotting LSD profiles from a terminal
+    Function for quickly reading and plotting LSD profiles from a terminal.
     """
     #Take input file names as command line arguments,
     #with some additional optional control parameters.
     parser = argparse.ArgumentParser(description='Plot a set of LSD profiles.')
     parser.add_argument("fileList", nargs='*',
                         help="LSD profile files to plot, can be more than one file.")
     parser.add_argument("-l", "--legend", action='store_true',
```

### Comparing `specpolFlow-0.3.4/specpolFlow/CommandLine/rvFit.py` & `specpolflow-0.4.0/specpolFlow/CommandLine/rvFit.py`

 * *Files identical despite different names*

### Comparing `specpolFlow-0.3.4/specpolFlow/cleanMaskUI.py` & `specpolflow-0.4.0/specpolFlow/cleanMaskUI.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-## @module cleanMaskUI.py
 """
 An interactive program for cleaning problem lines from a LSD line mask
 and tweaking (fitting) depths of some lines.  This opens its main
 program in another window.  The LSDpy package must be installed
 (in your Python path) to use this program.  
 """
 
@@ -13,33 +12,42 @@
 from . import profileLSD
 from . import mask as maskTools
 from . import obsSpec
 
 ###################################
 ###################################
 
-def cleanMaskUI(maskName, obsName, outMaskName=None,
-                excludeFileName='excludeRanges.dat', batchMode=False):
+def cleanMaskUI(maskName, obsName, outMaskName=None, inExcludeName=None,
+                outExcludeName='excludeRanges.dat', batchMode=False):
     """
     Run an interactive tool for LSD line mask cleaning.
 
     This opens a window with a plot of the line mask, a reference observation,
     and a model LSD spectrum (convolution of a line mask and LSD profile).
     The parameters for the LSD calculation are taken from the defaults in
     the cleanMaskUISubroutines lsdParams() function.
 
+    This saves a copy of the cleaned mask to a file, and also returns
+    a copy as a Mask object and the regions excluded from the mask
+    as an ExcludeMaskRegions object.
+
     :param maskName: File name, or a Mask object, for the input line mask
                      to clean.
     :param obsName: File name for the reference observation to compare with.
     :param outMaskName: File name for the output cleaned mask,
                         defaults to [maskName].clean
-    :param excludeFileName: File name for a set of regions to be excluded from
-                            the line mask (read from and write to). If the file
-                            doesn't exist a set of default values will be used.
-    :rtype: Mask
+    :param inExcludeName: File name for reading a set of regions to be excluded
+                          from the line mask.
+    :param outExcludeName: File name for saving the set of regions excluded 
+                           from the mask. (may be the same as inExcludeName)
+    :param batchMode: Flag for skipping the GUI. False = open the GUI (the default).
+                      True = skip the GUI, just read inExcludeName and apply 
+                      those exclude regions.
+    :return: a Mask object with the cleaned mask,
+             and an ExcludeMaskRegions with the selected exclude regions.
     """
     
     if outMaskName is None:
         if isinstance(maskName, maskTools.Mask):
             outMaskName = 'mask.clean'
         else:
             outMaskName = maskName+'.clean'
@@ -49,15 +57,16 @@
         mask = maskName
     else:
         mask = maskTools.read_mask(maskName)
     
     #Read a list of wavelength regions to exclude from the mask 
     #(if the file exists), or generate one from default values.
     try:
-        regions = maskTools.read_exclude_mask_regions(excludeFileName)
+        if inExcludeName is None: raise OSError #fall back to except block
+        regions = maskTools.read_exclude_mask_regions(inExcludeName)
     except OSError:
         regionsBalmer = maskTools.get_Balmer_regions_default(1000.)
         regionsTelluric = maskTools.get_telluric_regions_default()
         regions = regionsBalmer + regionsTelluric
     #Update the mask with these initial exclude regions
     mask = mask.clean(regions)
     #Make a list of lists from the exclude regions, used internally.
@@ -77,22 +86,21 @@
         #Make an initial LSD model spectrum
         print('Generating test LSD profile...')
         lsdp = cleanSub.lsdParams(obsName, outMaskName)
         #first save the current updated mask, so we can run LSDpy on it
         mask.save(outMaskName)
         #then run LSDpy, with specific 'default' parameters
         lsdProf, modelSpec = profileLSD.run_lsdpy(obs=lsdp.obs, mask=lsdp.mask,
-            outName=lsdp.outName, velStart=lsdp.velStart, velEnd=lsdp.velEnd,
+            outLSDName=lsdp.outName, velStart=lsdp.velStart, velEnd=lsdp.velEnd,
             velPixel=lsdp.velPixel, normDepth=lsdp.normDepth,
             normLande=lsdp.normLande, normWave=lsdp.normWave,
             removeContPol=lsdp.removeContPol, trimMask=lsdp.trimMask,
             sigmaClipIter=lsdp.sigmaClipIter, sigmaClip=lsdp.sigmaClip,
-            interpMode=lsdp.interpMode, outModelName=lsdp.outModelName,
-            fLSDPlotImg=lsdp.fLSDPlotImg, fSavePlotImg=lsdp.fSavePlotImg,
-            outPlotImgName=lsdp.outPlotImgName)
+            outModelName=lsdp.outModelName,
+            plotLSD=lsdp.plotLSD, outPlotLSDName=lsdp.outPlotLSDName)
         
         #Make a plot of the reference observation, mask, and LSD model spectrum
         fig =  Figure()
         ax1 = fig.add_subplot(111)
         pltObsI = ax1.plot(obs.wl, obs.specI, 'k')
         maskUsed = mask[mask.iuse == 1]
         maskNot = mask[mask.iuse == 0]
@@ -108,12 +116,18 @@
 
         #initialize an array of flags for fitting LSD line depths
         fitDepthFlags = np.zeros_like(mask.wl, dtype=int)
         
         #Run the main interactive program
         cleanSub.makeWin(fig, ax1, mask, obs, lsdp, pltMaskU, 
                          pltMaskN, pltMaskF, pltModelI, excludeRanges, 
-                         excludeFileName, fitDepthFlags)
-    
+                         outExcludeName, fitDepthFlags)
+
+    #make an ExcludeMaskRegions object to return
+    wlStarts = np.array([ran[0] for ran in excludeRanges])
+    wlEnds = np.array([ran[1] for ran in excludeRanges])
+    labels = np.array(['cleanMaskUI']*len(excludeRanges),dtype=object)
+    regions = maskTools.ExcludeMaskRegions(wlStarts, wlEnds, labels)
+
     #Save the final result
     mask.save(outMaskName)
-    return mask
+    return mask, regions
```

### Comparing `specpolFlow-0.3.4/specpolFlow/cleanMaskUISubroutines.py` & `specpolflow-0.4.0/specpolFlow/cleanMaskUISubroutines.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         _mplToolbar=0
 
 from . import profileLSD
 from . import mask as maskTools
 from . import obsSpec
 
 def makeWin(fig, ax, mask, obs, lsdp, pltMaskU, pltMaskN,
-            pltMaskF, pltModelI, excludeRanges, excludeFileName, fitDepthFlags):
+            pltMaskF, pltModelI, excludeRanges, outExcludeName, fitDepthFlags):
     #Build GUI with tkinter
     root = tk.Tk(className='Clean Masks')
     #the className seems to set an icon title (at least in Ubuntu)
     root.title("Clean Masks")
 
     ##For an icon image (used by window managers)
     #try:
@@ -178,18 +178,18 @@
                              command=excRangeM.runSpanSelect)
     ToolTip(butExcRange, 'Exclude selected lines from the mask')
     butExcRange.grid(row=0, column=8, sticky=tk.E, padx=2, pady=2)
     #Link the include and exclude buttons so they can turn each other off
     incRangeM.linkButton(butIncRange, excRangeM)
     excRangeM.linkButton(butExcRange, incRangeM)
     #Save the exclude ranges to a text file
-    saveRangesM = saveRanges(excludeFileName, excludeRanges)
+    saveRangesM = saveRanges(outExcludeName, excludeRanges)
     butSaveRanges = ttk.Button(master=tools, text='save\nranges',
                                command=saveRangesM.saveToFile)
-    ToolTip(butSaveRanges, 'Save the excluded wavelength ranges to the {:} file'.format(excludeFileName))
+    ToolTip(butSaveRanges, 'Save the excluded wavelength ranges to the {:} file'.format(outExcludeName))
     butSaveRanges.grid(row=0, column=9, sticky=tk.E, padx=2, pady=2)
 
     #Modify LSD control parameters
     modifyLSDparM = modifyLSDpar(root, lsdp)
     butModLSD = ttk.Button(master=tools, text='LSD param.',
                               command=modifyLSDparM.openWindow)
     ToolTip(butModLSD, 'Modify the parameters related to the LSD calculation')
@@ -274,15 +274,15 @@
             rangesO += [r1]
     return rangesO
 
 
 #A fairly simple, fairly general tooltip
 class ToolTip(object):
     """
-    Create a tooltip for a given widget, using Tkinter
+    Create a tooltip for a given widget, using Tkinter.
     This is a fairly simple class, but it wraps text at a specified length,
     puts the tooltip below the widget, and moves the tooltip to keep it 
     within the screen limits.  
     Based on the recipe from:
     http://www.voidspace.org.uk/python/weblog/arch_d7_2006_07_01.shtml#e387
     and some discussion from: 
     https://stackoverflow.com/questions/3221956/how-do-i-display-tooltips-in-tkinter
@@ -739,19 +739,14 @@
         #make an ExcludeMaskRegions object
         wlStarts = np.array([ran[0] for ran in self.ranges])
         wlEnds = np.array([ran[1] for ran in self.ranges])
         labels = np.array(['cleanMaskUI']*len(self.ranges),dtype=object)
         regions = maskTools.ExcludeMaskRegions(wlStarts, wlEnds, labels)
         #Save the set of exclude ranges to a file
         regions.save(self.fname)
-        #fout = open(self.fname,'w')
-        #fout.write('#exclude wavelength ranges\n')
-        #for ran in self.ranges:
-        #    fout.write('{:9.3f} {:9.3f}\n'.format(ran[0], ran[1]))
-        #fout.close()
         return
 
 
 class fitDepths:
     #mini manager to run the fitting of line depths
     def __init__(self, mask, obs, lsdp, fitDepthFlags, root, canvas,
                  pltMaskU, pltMaskN, pltMaskF):
@@ -832,15 +827,15 @@
     def __init__(self, parent, lsdp):
         self.parent = parent
         self.lsdp = lsdp
         self.active = False
         self.win = None
 
         self.varSaveMod = tk.IntVar()
-        if self.lsdp.outModelName == '':
+        if self.lsdp.outModelName is None:
             self.varSaveMod.set(0)
         else:
             self.varSaveMod.set(1)
     
     def closeWindow(self, *event):
         #Update any input information
         self.setVelStart()
@@ -932,15 +927,15 @@
                               width=8, validate='focusout',
                             validatecommand=self.setNLande)
         entNLande.bind('<Key-Return>', self.setNLande)
         ToolTip(entNLande, 'Set the normalizing Landé factor for the LSD mask/profile')
 
         #remove closely spaced lines in the LSD calculation?
         self.varRemoveClose = tk.IntVar()
-        self.varRemoveClose.set(self.lsdp.trimMask)
+        self.varRemoveClose.set(int(self.lsdp.trimMask))
         checkRemoveClose = ttk.Checkbutton(wframe,
                                            text='remove closely\nspaced lines',
                                            variable=self.varRemoveClose,
                                            command=self.setRemoveClose)
         ToolTip(checkRemoveClose, "Remove very closely spaced lines in the mask when calculating the LSD profile")
 
         #Optionally save the model LSD spectrum
@@ -948,15 +943,18 @@
                                        text='save model\nspectrum',
                                        variable=self.varSaveMod,
                                        command=self.setSaveMod)
         ToolTip(checkSaveMod, "Save a copy of the model LSD spectrum to a file?")
         labModName = ttk.Label(wframe, text='model\nfile name',
                                justify='right')
         self.txtModName = tk.StringVar()
-        self.txtModName.set('{:}'.format(self.lsdp.outModelName))
+        if self.lsdp.outModelName is None:
+            self.txtModName.set('')
+        else:
+            self.txtModName.set('{:}'.format(self.lsdp.outModelName))
         entModName = ttk.Entry(master=wframe,
                                textvariable=self.txtModName, width=25,
                                validate='focusout',
                                validatecommand=self.setModName)
         entModName.bind('<Key-Return>', self.setModName)
         ToolTip(entModName, 'File name for the output model LSD spectrum')
         
@@ -969,15 +967,15 @@
                                 textvariable=self.txtProfName, width=25, 
                                 validate='focusout',
                                 validatecommand=self.setProfName)
         entProfName.bind('<Key-Return>', self.setProfName)
         ToolTip(entProfName, 'File name for the output LSD profile')
 
         self.varPltProf = tk.IntVar()
-        self.varPltProf.set(self.lsdp.fLSDPlotImg)
+        self.varPltProf.set(int(self.lsdp.plotLSD))
         checkPltProf = ttk.Checkbutton(wframe, text='plot\nprofile',
                                        variable=self.varPltProf,
                                        command=self.setPlotProf)
         ToolTip(checkPltProf, "Plot the LSD profile in a new window when updated?")
 
         #Lay out the widgits in the window
         labVelStart.grid(row=0, column=0, sticky=tk.E, pady=4, padx=4)
@@ -1107,42 +1105,42 @@
             val = 10.0
             self.txtNLande.set('{:.2f}'.format(val))
         self.lsdp.normLande = val
         return True
 
     def setRemoveClose(self, *event):
         val = self.varRemoveClose.get()
-        self.lsdp.trimMask = int(val)
+        self.lsdp.trimMask = bool(val)
         return
     
     def setSaveMod(self, *event):
         val = self.varSaveMod.get()
         if val == 0:
-            self.lsdp.outModelName = ''
+            self.lsdp.outModelName = None
         else:
             self.lsdp.outModelName = self.txtModName.get()
         return
     def setModName(self, *event):
         flag = self.varSaveMod.get()
         if flag != 0:
             self.lsdp.outModelName = self.txtModName.get()
         else:
-            self.lsdp.outModelName = ''
+            self.lsdp.outModelName = None
         return
     def setProfName(self, *event):
         val = self.txtProfName.get()
         if val != '':
             self.lsdp.outName = val
         return
     def setPlotProf(self, *event):
         val = self.varPltProf.get()
         if val == 0:
-            self.lsdp.fLSDPlotImg = 0
+            self.lsdp.plotLSD = False
         else:
-            self.lsdp.fLSDPlotImg = 1
+            self.lsdp.plotLSD = True
         return
 
 
 class updateLSD:
     def __init__(self, canvas, root, mask, lsdp, pltModelI):
         self.canvas = canvas
         self.root = root
@@ -1155,22 +1153,21 @@
         oldCursor = self.root.cget('cursor')
         self.root.config(cursor='watch')
         self.root.update()
         #Run LSD
         lsdp = self.lsdp
         self.mask.save(lsdp.mask)
         lsdProf, modelSpec = profileLSD.run_lsdpy(obs=lsdp.obs, mask=lsdp.mask,
-            outName=lsdp.outName, velStart=lsdp.velStart, velEnd=lsdp.velEnd,
+            outLSDName=lsdp.outName, velStart=lsdp.velStart, velEnd=lsdp.velEnd,
             velPixel=lsdp.velPixel, normDepth=lsdp.normDepth,
             normLande=lsdp.normLande, normWave=lsdp.normWave,
             removeContPol=lsdp.removeContPol, trimMask=lsdp.trimMask,
             sigmaClipIter=lsdp.sigmaClipIter, sigmaClip=lsdp.sigmaClip,
-            interpMode=lsdp.interpMode, outModelName=lsdp.outModelName,
-            fLSDPlotImg=lsdp.fLSDPlotImg, fSavePlotImg=lsdp.fSavePlotImg,
-            outPlotImgName=lsdp.outPlotImgName)
+            outModelName=lsdp.outModelName,
+            plotLSD=lsdp.plotLSD, outPlotLSDName=lsdp.outPlotLSDName)
         #Return the cursor to normal
         self.root.config(cursor=oldCursor)
         
         #re-draw points used in the fit
         for dline in self.pltModelI:
             dline.set_data(modelSpec.wl, modelSpec.specI)
         self.canvas.draw()
@@ -1284,21 +1281,21 @@
 
     ##If one wanted a shorter mask
     #mask = mask.prune()
     return
 
 
 class lsdParams:
-    def __init__(self, obs, mask, outName='prof.dat',
+    def __init__(self, obs, mask, outName='',
                  velStart=-200., velEnd=200., velPixel=None,
                  normDepth=0.2, normLande=1.2, normWave=500.,
-                 removeContPol=1, trimMask=0, 
-                 sigmaClipIter=0, sigmaClip=500., interpMode=1, 
-                 outModelName='',
-                 fLSDPlotImg=0, fSavePlotImg=0, outPlotImgName=''):
+                 removeContPol=True, trimMask=False, 
+                 sigmaClipIter=0, sigmaClip=500.,
+                 outModelName=None,
+                 plotLSD=False, outPlotLSDName=None):
         """
         A simple data structure to hold input parameters for LSD calculations,
         and to set some sensible defaults.
         """
         self.obs = obs
         self.mask = mask
         self.outName = outName
@@ -1307,23 +1304,20 @@
         self.normDepth = normDepth
         self.normLande = normLande
         self.normWave = normWave
         self.removeContPol = removeContPol
         self.trimMask = trimMask
         self.sigmaClipIter = sigmaClipIter
         self.sigmaClip = sigmaClip
-        self.interpMode = interpMode
         self.outModelName = outModelName
-        self.fLSDPlotImg = fLSDPlotImg
-        self.fSavePlotImg = fSavePlotImg
-        self.outPlotImgName = outPlotImgName
+        self.plotLSD = plotLSD
+        self.outPlotLSDName = outPlotLSDName
         
         cvel = 2.99792458e5 #c in km/s
         if velPixel == None:
             #Get average observed wavelength spacing
             obsSp = obsSpec.read_spectrum(self.obs)
             wlStep = obsSp.wl[1:] - obsSp.wl[:-1]
-            indWlSteps = ((wlStep > 0.) & (wlStep < 0.1))
-            meanVelPix = np.average(wlStep[indWlSteps]/obsSp.wl[:-1][indWlSteps]*cvel)
-            self.velPixel = round(meanVelPix, ndigits=2)
+            medianVelPix = np.median(wlStep/obsSp.wl[:-1]*cvel)
+            self.velPixel = round(medianVelPix, ndigits=2)
         else:
             self.velPixel = velPixel
```

### Comparing `specpolFlow-0.3.4/specpolFlow/converters/convert-spirou-fits-s0.2.py` & `specpolflow-0.4.0/specpolFlow/converters/convert-spirou-fits-s0.2.py`

 * *Files identical despite different names*

### Comparing `specpolFlow-0.3.4/specpolFlow/converters/espadons.py` & `specpolflow-0.4.0/specpolFlow/converters/espadons.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,32 +7,46 @@
 import astropy.io.fits as fits
 
 def espadons(flist, flistout=None):
     """
     Convert a list of .fits files in the CADC ESPaDOnS format into
     text .s files. 
 
-    The code provides two files in .s format:
-    * The UPENA normalized spectrum, with automated radial velocity corrections from the telluric lines.
-    * The UPENA unnormalized spectrum, using the automated radial velocity correction from the normalized spectrum.
-    For we use the unnormalized spectrum without the automated radial velocity correction, 
-    and we apply the radial velocity correction determined from the normalized spectrum.  
+    The code provides two files in .s format:  
+     
+    * The UPENA normalized spectrum (n.s), with automated radial velocity corrections from the telluric lines.
+    * The UPENA unnormalized spectrum (u.s), using the automated radial velocity correction from the normalized spectrum.
+    This is done starting from the unnormalized spectrum without the automated radial velocity correction, to which 
+    we apply the radial velocity correction determined from the normalized spectrum.  
     The reason behind this is that the UPENA automated radial velocity determination performed on 
     unnormalized spectra does not produce consistently reliable results. 
     The content of the fits header is also saved in a .out ascii file.
-    If flistout=None (default) The files are written at the same path as the fits-format data, with the '.fits' stripped, 
+    If flistout=None (default), the files are written at the same path as the fits-format data, with the '.fits' stripped, 
     and 'n.s' and 'u.s' appended to the filename root. 
     If flistout is a list of paths ending with a rootname, the files will be saved at that path with that rootname, 
-    and 'n.s' and 'u.s' appended to the filename root
+    and 'n.s' and 'u.s' appended to the filename root.
 
     :param flist: (list of strings) a list of ESPaDOnS filenames
     :param flistout: (list of strings) optional, list of output file rootnames
     """
 
     if isinstance(flist, str): flist = [flist,]
+    #Some basic error checking
+    if not isinstance(flist, list):
+        raise ValueError('in espadons(), the flist argument must be a Python '
+                         'list of input file names (or a single file name)')
+    if not (flistout is None):
+        if isinstance(flistout, str): flistout = [flistout,]
+        if not isinstance(flistout, list):
+            raise ValueError('in espadons(), the flistout argument must be a '
+                             'Python list of output file names')
+        if len(flist) != len(flistout):
+            raise ValueError('in espadons(), the list of input file names and '
+                             'list of output file names must have the same length')
+    
     for i, fname in enumerate(flist):
         print('converting ', fname.strip())
         if flistout is None:
             # striping of white spaces
             fnameOut = fname.strip()
             # removing the '.fits' from the end of the string, 
             # to create the root name for the output files.
```

### Comparing `specpolFlow-0.3.4/specpolFlow/lineList.py` & `specpolflow-0.4.0/specpolFlow/lineList.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,23 @@
-## @module lineList.py
 """
 Tools for manipulating lists of spectral line data.
 Includes tools for reading and parsing VALD version 3 line lists 
-(typically 'long format' 'extract stellar' requests).
+(typically 'long format', 'extract stellar' requests).
 """
 
 import numpy as np
 
 ###################################
 
 class LineList:
     """
     Container for a set of spectral line data, usually from VALD.
 
-    This usually contains:
-    
+    This usually contains: 
+     
     * nLines - number of lines in the line list
     * ion - list of species identifiers (element or molecule and ionization)
     * wl - array of wavelengths
     * loggf - array of oscillator strengths (log gf)
     * Elo - array of excitation potentials for the lower level in
       the transition (in eV)
     * Jlo - array of J quantum numbers for the lower level
@@ -166,15 +165,15 @@
         return
     
 def line_list_zeros(nLines):
     """
     Generate a line list of zeros and blank text.
     
     Used by read_VALD
-    (It can be a bit faster to allocate all the array space at once)
+    (It can be a bit faster to allocate all the array space at once.)
     
     :param nLines: the number of lines in the LineList of zeros
     :rtype: LineList
     """
     ion      = np.tile(np.array([''], dtype='U6'), nLines)
     wl       = np.zeros(nLines)
     loggf    = np.zeros(nLines)
@@ -195,15 +194,15 @@
     lList = LineList(ion, wl, loggf, Elo, Jlo, Eup, Jup, landeLo,
                      landeUp, landeEff, rad, stark, waals, depth,
                      configLo, configUp, refs)
     return lList
 
 def read_VALD(fname):
     """
-    Read a list of spectral line data from VALD and return a LineList
+    Read a list of spectral line data from VALD and return a LineList.
 
     This expects VALD version 3 line list, in an 'extract stellar'
     'long' format.
 
     :param fname: the file name for the VALD line list.
     :rtype: LineList
     """
@@ -274,15 +273,15 @@
     landeEff = 0.5*(landeUp + landeLo) + 0.25*(landeUp - landeLo)*(Jup*(Jup + 1) - Jlo*(Jlo + 1))
     
     return landeEff
 
 
 def estimateLande(J, config, verbose=False):
     """
-    Estimate a Lande factor for a level (if VALD doesn't have one)
+    Estimate a Lande factor for a level (if VALD doesn't have one).
 
     This supports levels in LS coupling, JJ coupling, and JK coupling.
     Levels in LK coupling are not supported.  This relies on VALD3's text 
     format for electron term symbols and configurations.
     
     :param J: The J quantum number for this level
     :param config: The text string from VALD with the electron configuration
@@ -438,15 +437,15 @@
     """
     Extract the L1, S1, J1, L2, S2, and J2 quantum numbers for a level in JJ 
     coupling from VALD's electron configuration and term symbol text string.
 
     This should cover the J1-J2 case (where two subgroups combine to produce
     J1 and J2, which combine to produce the total J), the J1-j case (where
     one subgroup makes J1, which combines with an additional electron with j
-    combines to produce J), and it should work for the j-j case (for two
+    to produce J), and it should work for the j-j case (for two
     equivalent electrons with their own j, which combine to make J).
     
     :param config: the electron configuration and term symbol text string
     :return: The L1, S1, J1, L2, S2, and J2 quantum numbers
              (if a parsing error occurs, negative values are returned)
     """
     #Letters for L quantum numbers (note J is omitted in this notation)
```

### Comparing `specpolFlow-0.3.4/specpolFlow/mask.py` & `specpolflow-0.4.0/specpolFlow/mask.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-## @module mask.py
 """
 Tools for generating and manipulating line masks for LSD.
 Includes creating a line mask from a VALD line list, cleaning problem 
 lines from the mask, managing regions to exclude from the mask,
 and interacively cleaning and tweaking.
 """
 
 import numpy as np
+import warnings
 #from . import lineList as lineListLib #(moved inside some functions)
 
 ###################################
 ###################################
 
 class Mask:
     """
     The data for the LSD line Mask.
 
-    This usually contains arrays:
-    
+    This usually contains the arrays: 
+
     * wl - wavelengths of lines
     * element - the element+ion code for the line
     * depth - the depth of the line
     * lande - the effective Lande factor of the line
     * iuse - integer flag for whether the line is used
     """
     def __init__(self, wl, element, depth, excite, lande, iuse):
@@ -66,15 +66,15 @@
             self.depth[key] = newval.depth
             self.excite[key] = newval.excite
             self.lande[key] = newval.lande
             self.iuse[key] = newval.iuse
 
     def __len__(self):
         """
-        Returns the number of lines in the mask
+        Returns the number of lines in the mask.
         """
         return len(self.wl)
     
     def prune(self):
         """
         Return a Mask object with unused lines removed from the Mask.
         
@@ -84,19 +84,19 @@
         :rtype: Mask
         """
         trimmedMask = self[self.iuse != 0]
         return trimmedMask
         
     def get_weights(self, normDepth, normWave, normLande):
         """
-        Returns the calculated the LSD weights of all the lines in the mask
+        Returns the calculated LSD weights of all the lines in the mask
         (includes lines with both the iuse flag 0 and 1).
         
         This assumes the Stokes I lines are weighted as depth,
-        and Stokes V is weighted as depth*wavelength*Lande factor
+        and Stokes V is weighted as depth*wavelength*Lande factor.
         
         :param normDepth: the normalizing line depth for the mask/LSD profile
         :param normWave: the normalizing wavelength (nm) for
                          the mask/LSD profile
         :param normLande: the normalizing effective Lande factor for
                           the mask/LSD profile
         :return: weightI, weightV (as arrays)
@@ -105,15 +105,15 @@
         weightV = self.depth*self.wl*self.lande / (normDepth*normWave*normLande)
         return weightI, weightV
     
     def save(self, fname):
         """
         Save the line Mask to a text file, in Donati's and LSDpy format.
         
-        :param fname: the file name to output the Mask to.
+        :param fname: the file name to output the Mask to
         """
         
         nlines = self.wl.shape[0]
         with open(fname, 'w') as oFile:
             oFile.write('{:d}\n'.format(nlines))
             for i in range(nlines):
                 oFile.write('{:9.4f} {:6.2f} {:6.3f} {:6.3f} {:6.3f} {:2d}\n'.format(
@@ -143,18 +143,18 @@
                                     (self.wl<=regions[i].stop) )
             mask_clean.iuse[is_in] = 0
 
         return mask_clean
 
 def read_mask(fname):
     """
-    Read in an LSD line mask file and returns a Mask object.
+    Read in an LSD line mask file and return a Mask object.
+
+    The mask file will have one line of header and columns of:  
 
-    The mask file should one line of header and columns of:
-    
     * Wavelength (nm)
     * Atomic number + (ionization state)*0.01
     * Line depth
     * Excitation potential of the lower level (eV)
     * Effective Lande factor
     * Flag for whether the line is used (1=use, 0=skip).
 
@@ -178,16 +178,16 @@
 ###################################
 ###################################
 
 class ExcludeMaskRegions:
     """
     Class for a region object that records spectral regions to exclude from a Mask.
 
-    Usualy contrains arrays of:
-
+    Usually contrains arrays of:  
+    
     * start - starting wavelengths for the regions
     * stop - ending wavelengths for the regions
     * type - optionally, text comments for the type of region \
              (inside a numpy array with dtype=object)
     """
 
     def __init__(self, start, stop, type):
@@ -224,15 +224,15 @@
         """
         Returns the number of lines in the mask
         """
         return len(self.start)
 
     def __add__(self, other):
         """
-        Concatenate two ExcludeMaskRegions objects
+        Concatenate two ExcludeMaskRegions objects.
         
         :param other: an ExcludeMaskRegions object to combine with this one
         :rtype: ExcludeMaskRegions
         """
         start = np.concatenate([self.start, other.start])
         stop = np.concatenate([self.stop, other.stop])
         type = np.concatenate([self.type, other.type])
@@ -259,15 +259,15 @@
         This is useful to transform ExcludeMaskRegions objects
         to Panda dataframes.
         """
         return {'start':self.start, 'stop':self.stop,'type':self.type}
 
 def read_exclude_mask_regions(fname):
     """
-    Read in a ExcludeMaskRegions file into an ExcludeMaskRegions object. 
+    Read in an ExcludeMaskRegions file into an ExcludeMaskRegions object. 
 
     The file should be a text file with one line for each region,
     containing the start wavelength, end wavelength, and the type comment.
     
     :param fname: the path/name of the file
     :rtype: ExcludeMaskRegions
     """
@@ -288,15 +288,15 @@
     
     return ExcludeMaskRegions(start, stop, np.array(type, dtype=object))
 
 def get_Balmer_regions_default(velrange=500):
     '''
     Generate an ExcludeMaskRegions object with regions around Balmer H-lines
     (alpha to epsilon) up to a given radial velocity,
-    and a region that excludes the Balmer jump (from 360-392 nm)
+    and a region that excludes the Balmer jump (from 360-392 nm).
     
     :param velrange: velocity range around the H-line to be excluded
                      (default 500 km/s)
     :rtype: ExcludeMaskRegions
     '''
 
     c = 299792.458 # Speed of light in km/s
@@ -328,45 +328,45 @@
 
     return ExcludeMaskRegions(np.array(start), np.array(stop),
                               np.array(types,dtype=object))
 
 def get_telluric_regions_default():
     '''
     Generate an ExcludeMaskRegions object with regions containing
-    heavy telluric line contamination in the optical
+    heavy telluric line contamination in the optical.
     
     :rtype: ExcludeMaskRegions
     '''
     start = np.array([587.5,627.5,684.0,717.0,757.0,790.0,809.0])  # nm
     stop   = np.array([592.0,632.5,705.3,735.0,771.0,795.0,990.0])  # nm
 
     return ExcludeMaskRegions(start, stop,
                               np.array(['telluric']*len(start),dtype=object))
 
 
 ###################################
 ###################################
 
-def make_mask(lineListFile, maskFile, depthCutoff=0.0, 
+def make_mask(lineListFile, outMaskName=None, depthCutoff=0.0, 
               wlStart=None, wlEnd=None, landeStart=None, landeEnd=None,
               elementsUsed=[], elementsExclude=[],
               atomsOnly=True, includeNoLande=False, defaultLande=1.0):
     """
     Generate an LSD line mask from a VALD line list and save it.
-    The main interface for generating new line masks with Python scrips.
+    This is the main interface for generating new line masks with Python scrips.
     
     This generates an LSD line mask from atomic lines in the list,
-    and estimates Lande factors for lines where possible.  Lines that 
-    no Lande factor can be estimated for are omitted by default.
+    and estimates Lande factors for lines where possible.  Lines for which 
+    no Lande factor can be estimated are omitted by default.
     This assumes input line list wavelengths in A, and returns a mask in nm.
     
     :param lineListFile: The name of the file containing the line list
                          (in the VALD3 'extract stellar' 'long' format)
-    :param maskFile: The name of the to write the mask to
-                     (set this to None to avoid saving a files)
+    :param outMaskName: The name of the to write the mask to
+                        (set this to None to avoid saving a file, default)
     :param depthCutoff: Only include lines in the mask deeper than this value
                         (defaults to 0, all lines included)
     :param wlStart: Optionally, only use lines with wavelengths above this
                     (note: value in nm!)
     :param wlEnd: Optionally, only use lines with wavelengths below this
                   (note: value in nm!)
     :param landeStart: Optionally, only use lines with effective Lande factors
@@ -386,40 +386,41 @@
     :param includeNoLande: Include lines in the mask even if no Lande factor
                            can be estimated for them (defaults to False)
     :param defaultLande: The value of the effective Lande factor to use if
                          no value can be estimated (only used if
                          includeNoLande = True)
     :rtype: Mask
     """
+
     from . import lineList as lineListLib
     lineList = lineListLib.read_VALD(lineListFile)
     
     mask = convert_list_to_mask(lineList, depthCutoff=depthCutoff,
                                 atomsOnly=atomsOnly,
                                 includeNoLande=includeNoLande,
                                 defaultLande=defaultLande)
     
     mask = filter_mask(mask, depthCutoff=depthCutoff,
                        wlStart=wlStart, wlEnd=wlEnd,
                        landeStart=landeStart, landeEnd=landeEnd,
                        elementsUsed=elementsUsed,
                        elementsExclude=elementsExclude)
 
-    if maskFile is not None:
-        mask.save(maskFile)
+    if outMaskName is not None:
+        mask.save(outMaskName)
     return mask
 
     
 def convert_list_to_mask(lineList, depthCutoff=0.0, atomsOnly = True,
                          includeNoLande = False, defaultLande=1.0):
     """
-    Convert a VALD line list to an LSD line mask.
+    Convert a lineList to an LSD line mask.
     
-    This estimates Lande factors when VALD doesn't have a known value
-    This also can automatically reject any H lines and any molecular lines.
+    This estimates Lande factors when VALD doesn't have a known value.
+    This can also automatically reject any H lines and any molecular lines.
     Note, this assumes an input line list in A, and returns a mask in nm.
     See also the make_mask() function.
     
     :param lineList: The line list object to be converted to a mask
     :param depthCutoff: Only include lines deeper than this depth cutoff
                         (defaults to 0, all lines included)
     :param atomsOnly: Flag to use only atomic lines (no molecular lines)
@@ -529,15 +530,15 @@
 
     Usually, only one of elementsUsed and elementsExclude should be used.
     Both can be used, in that case only elements in elementsUsed are included,
     and then any elements in elementsExclude are removed from that.
     (Filtering by element currently only works for atomic lines,
     not molecular lines)
 
-    :param mask: The line mask object to filter lines out of.
+    :param mask: The line mask object to filter lines out of
     :param depthCutoff: Only include lines in the mask deeper than this value
                         (defaults to 0, all lines included)
     :param wlStart: Optionally, only use lines with wavelengths above this
                     (note: value in nm!)
     :param wlEnd: Optionally, only use lines with wavelengths below this
                   (note: value in nm!)
     :param landeStart: Optionally, only use lines with effective Lande factors
```

### Comparing `specpolFlow-0.3.4/specpolFlow/profileLSD.py` & `specpolflow-0.4.0/specpolFlow/profileLSD.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,44 +1,44 @@
-## @module profileLSD.py
 """
 Tools for generating and manipulating LSD profiles.  Includes calculating
 longitudinal magnetic fields and radial velocities.  Also includes a wrapper
 around LSDpy.
 """
 
 import copy
+import warnings
 import numpy as np
 import matplotlib.pyplot as plt
 import scipy.special as specialf
 from scipy.optimize import curve_fit
 
-from .obsSpec import Spectrum
+from .obsSpec import Spectrum, read_spectrum
 
 ###################################
 ###################################
 class LSD:
     """
     Holds the LSD profile data.
 
     This usually includes numpy arrays:
-    
+
     * vel - velocity grid for the LSD profile
     * specI - the Stokes I profile
     * specSigI - the uncertainties on Stokes I
     * specV - the polarization profile, most often Stokes V
     * specSigI - the uncertainties on the polarization profile
     * specN1 - the Null1 profile
     * specSigN1 - the uncertainties on specN1
     * specN2 - the Null2 profile, if it exists, otherwise zeros
     * specSigN2 - the uncertainties on Null2 if they exist
     * header - an optional text header for the LSD profile file
 
     And integers:
-    
-    * numParam - The number of Stokes I V & Null profiles used (usually 1, 3, or 4)
+      
+    * numParam - The number of Stokes I, V, & Null profiles used (usually 1, 3, or 4)
     * npix - the number of pixels (points in velocity) in the LSD profile
     """
     def __init__(self, vel, specI, specSigI, specV=None, specSigV=None,
                  specN1=None, specSigN1=None, specN2=None, specSigN2=None,
                  header=None):
         """
         Initialize an LSD profile, using data from an existing profile. 
@@ -47,15 +47,16 @@
         :param specI: the Stokes I profile
         :param specSigI: the uncertainties on Stokes I
         :param specV: the polarization profile, usually Stokes V
         :param specSigV: the uncertainties on the polarization profile 
         :param specN1: the Null1 profile
         :param specSigN1: the uncertainties on Null1
         :param specN2: the Null2 profile, if it exists, otherwise it is all 0s (optional)
-        :param specSigN2: the uncertainties on Null2 if there are any, otherwise all 0s (optional)
+        :param specSigN2: the uncertainties on Null2 if there are any,
+                          otherwise all 0s (optional)
         :param header: the header of the LSD profile file, if it exists (optional) 
         """
         self.vel = vel
         self.specI = specI
         self.specSigI = specSigI
         self.npix = vel.size
         self.numParam = 1
@@ -119,15 +120,15 @@
         slice_prof = LSD(vel_s, specI_s, specSigI_s, specV_s, specSigV_s,
                          specN1_s, specSigN1_s, specN2_s, specSigN2_s, self.header)
         slice_prof.numParam = self.numParam
         return slice_prof
 
     def __setitem__(self, key, newval):
         """
-        Sets all values of the LSD at the specified location equal to the
+        Sets all values of the LSD object at the specified location equal to the
         input profile's values.
 
         :param key: the index or slice being overwritten
         :param newval: LSD object used to replace the overwritten values
         """
         if not(isinstance(newval, LSD)):
             raise TypeError()
@@ -141,18 +142,17 @@
             self.specSigN1[key] = newval.specSigN1
             self.specN2[key] = newval.specN2
             self.specSigN2[key] = newval.specSigN2
 
     def save(self, fname):
         """
         Save the LSD profile to a file.
-        
         This saves to a text file in Donati's format.
         
-        :param fname: the name of the file the LSD profile to save to.
+        :param fname: the name of the file the LSD profile to saves to.
         """
         
         oFile = open(fname, 'w')
         if self.header != None:
             if self.header == "":
                 #For blank headers include some placeholder text
                 oFile.write('#LSD profile\n')
@@ -177,72 +177,97 @@
                     self.specSigV[i], self.specN1[i], self.specSigN1[i],
                     self.specN2[i], self.specSigN2[i]))
         oFile.close()
         return
 
     def norm(self, normValue):
         """
-        Return a renormalize an LSD profile, divide the I, V, and null 
-        profiles by a value.
+        Return a renormalized LSD profile. Divides the I, V, and Null 
+        profiles, and their uncertainties, by a value.
         
         :param normValue: the value to renormalize (divide) the LSD profile by
         :rtype: LSD
         """
- 
         new = LSD(self.vel, 
                   self.specI/normValue, self.specSigI/normValue, 
                   self.specV/normValue, self.specSigV/normValue,
                   self.specN1/normValue, self.specSigN1/normValue, 
                   self.specN2/normValue, self.specSigN2/normValue, 
                   self.header)
         new.numParam = self.numParam
-
         return new
 
     def vshift(self, velShift):
         """
-        Return a LSD profile with a shift to the velocities of the LSD profile
+        Return an LSD profile, with a shift to the velocities of the LSD profile.
         
         :param velShift: the change in velocity to be added
         :rtype: LSD
         """
         new = LSD(self.vel-velShift, 
                   self.specI, self.specSigI, 
                   self.specV, self.specSigV,
                   self.specN1, self.specSigN1, 
                   self.specN2, self.specSigN2, 
                   self.header)
         new.numParam = self.numParam
-
         return new
 
     def scale(self, scale_int, scale_pol):
         """
-        Return a LSD profile with rescaled amplitudes of the LSD profile
-        (see also set_weights())
+        Return an LSD profile with rescaled amplitudes of the LSD profile
+        (see also set_weights()).
         
         :param scale_int: scale the intensity profile by this
         :param scale_pol: scale the polarization and null profiles by this
         :rtype: LSD
         """
 
         new = LSD(self.vel, 
                   1.0 - ((1.0-self.specI)*scale_int), self.specSigI*scale_int, 
                   self.specV*scale_pol, self.specSigV*scale_pol,
                   self.specN1*scale_pol, self.specSigN1*scale_pol, 
                   self.specN2*scale_pol, self.specSigN2*scale_pol, 
                   self.header)
         new.numParam = self.numParam
+        
+        # If we have scaled the profile we may need to adjust 
+        # the weights in the header. Parse the old header,
+        # and if necessary re-write the portion with the weights.
+        if 'normalizing: d=' in self.header:
+            ihead = self.header.index('normalizing: d=') - 1
+            depth = 0; lande = 0; wl0 = 0
+            #Get the old depth
+            indDepth = self.header.find('d=')
+            if indDepth >= 0:
+                depth = float(self.header[indDepth+2:].split()[0])
+            #Get the old Lande factor
+            indLande = self.header.find('lande=')
+            if indLande >= 0:
+                lande = float(self.header[indLande+6:].split()[0])
+            #Get the old wavelength
+            indWl0 = self.header.find('wl=')
+            if indWl0 >= 0:
+                wl0 = float(self.header[indWl0+3:].split()[0])
+
+            depth *= scale_int
+            wl0 *= scale_pol/scale_int
+            sFormat = (' normalizing: d={:5.3f} lande={:5.3f} wl={:6.1f} '
+                       '(I norm weight {:5.3f}, V norm weight {:7.3f})\n')
+            headerAdd = sFormat.format(depth, lande, wl0, depth,
+                                       depth*lande*wl0)
+            headder = self.header[:ihead] + headerAdd
+            new.header = headder
 
         return new
 
     def set_weights(self, wint_old, wpol_old, wint_new, wpol_new):
         """
-        Return a LSD profile with different mask normalization/scaling weights
-        (see also scale())
+        Return an LSD profile with different mask normalization/scaling weights
+        (see also scale()).
         
         :param wint_old: The current intensity weight (d)
         :param wpol_old: The current polarization weight (g*d*lambda)
         :param wint_new: The new intensity weight (d)
         :param wpol_new: The new polarization weight (g*d*lambda)
         :rtype: LSD
         """
@@ -251,15 +276,15 @@
     def plot(self, figsize=(10,10), sameYRange=True, plotZeroLevel=True,
              fig=None, **kwargs):
         """
         Plot the LSD profile
 
         This generates a matplotlib figure. To display the figure, after
         running this function, use 'import matplotlib.pyplot as plt' and
-        'plt.show()'. To save the figure you can use 
+        'plt.show()'. To save the figure, you can use 
         'fig.savefig("fileName.pdf")' on the new figure object.
         
         :param figsize: the size of the figure being created
         :param sameYRange: optionally set the Stokes V and Null plots to have
                            the same y scale
         :param plotZeroLevel: optionally include a dashed line at 0 for
                               the V and Null plots
@@ -333,24 +358,24 @@
 
     def fit_gaussian_rv(self, velrange=None, plotFit=False, fullOutput=False,
                         scaleErrs=False):
         """
         Fit a Gaussian function to this LSD profile, to determine a
         radial velocity.
         
-        :param velrange: Range of velocity to fit include in the fit
-                         (a tuple or list with 2 elements)
-                         If not given, the whole range will be used
-        :param plotFit: If True, Plot the fit to the LSD profile with matplotlib
-        :param fullOutput: If True, Return all the Gaussian best fit parameters,
+        :param velrange: Range of velocities included in the fit
+                         (a tuple or list with 2 elements).
+                         If not given, the whole range will be used.
+        :param plotFit: If True, plot the fit to the LSD profile with matplotlib
+        :param fullOutput: If True, return all the Gaussian best fit parameters,
                            rather than just the RV and RV error
-        :param scaleErrs: If True scale the errors on the fitting parameters by
+        :param scaleErrs: If True, scale the errors on the fitting parameters by
                           the square root of the reduced chi^2
-        :return: Tuple of best fit RV and RV error.
-                 If fullOutput is True then also includes continuum & error,
+        :return: Tuple of best fit RV and RV error;
+                 If fullOutput is True, then also includes continuum & error,
                  amplitude & error, and width & error
         """
 
         if velrange == None:
             velrange = (self.vel[1], self.vel[-2])
         elif not(isinstance(velrange, list) or isinstance(velrange, tuple)):
             raise TypeError('velrange in fitGaussianRV should be a list or '
@@ -397,69 +422,84 @@
 
         #Optionally return all fit parameters
         if fullOutput == True:
             return (fitVel, fitVelErr, fitCont, fitContErr, fitAmpl, 
                     fitAmplErr, fitWidth, fitWidthErr)
         return fitVel, fitVelErr
 
-    def cog_I(self, Ic=1.0):
+    def cog_I(self, Ic=1.0, fullOutput=False):
         '''
         Helper function to return the center of gravity of Stokes I for
-        this LSD profile, for a given continuum level
+        the LSD profile, for a given continuum level.
 
-        :param Ic: the continnum level to use the the COG calculation
+        :param Ic: the continuum level to use the the COG calculation
                    (float, default=1.0)
+        :param fullOutput: If True, return the error of the velocity
+                            of the center of gravity
         :return: the velocity of the center of gravity
         '''
+        # Computes the velocity of the center of gravity
         nominator = np.trapz(self.vel * (Ic-self.specI), x=self.vel)
         denominator = np.trapz( Ic-self.specI, x=self.vel )
-        return nominator/denominator
+        rv = nominator/denominator
+
+        # Estimate the associated error
+        deltav = self.vel[1] - self.vel[0]
+        nominatorSig = np.sqrt(np.sum(self.vel**2 * self.specSigI**2) * deltav**2)
+        denominatorSig = np.sqrt(np.sum(self.specSigI**2) * deltav**2)
+        rvSig = np.abs(rv * np.sqrt((nominatorSig/nominator)**2
+                                    + (denominatorSig/denominator)**2))
+
+        #Optionally return the rv and its error 
+        if fullOutput == True:
+            return rv, rvSig
+        return rv
 
     def cog_IV(self, Ic=1.0):
         '''
         Helper function to return the center of gravity of (Stokes I)*(Stoke V)
-        for this LSD profile, for a given continuum level
+        for the LSD profile, for a given continuum level.
 
         :param Ic: the continnum level to use the the COG calculation
                    (float, default=1.0)
         :return: the velocity of the center of gravity
         '''
         nominator = np.trapz(self.vel * np.abs( self.specV * (Ic-self.specI) ),
                              x=self.vel )
         denominator = np.trapz(np.abs( self.specV * (Ic-self.specI) ),
                                x=self.vel )
         return nominator/denominator
 
     def cog_V(self):
         '''
-        Helper function to return the center of gravity of this Stokes V
-        LSD profile
+        Helper function to return the center of gravity of the Stokes V
+        LSD profile.
         
         :return: the velocity of the center of gravity
         '''
         nominator = np.trapz(self.vel * np.abs(self.specV), x=self.vel )
         denominator = np.trapz( np.abs(self.specV), x=self.vel )
         return(nominator/denominator)        
 
     def cog_min(self):
         '''
-        Helper function to return the velocity of the minimum of this
-        Stokes I LSD profile
+        Helper function to return the velocity of the minimum of the
+        Stokes I LSD profile.
         
-        :return: the velocity of the Stokes I minumum
+        :return: the velocity of the Stokes I minimum
         '''
         
         cog_min = self.vel[self.specI.argmin()]
         if cog_min.size > 1:
             cog_min = cog_min[0]
-        return cog_min 
+        return cog_min
 
     def calc_fap(self):
         '''Helper function that calculates the FAP for Stokes V, null1,
-        and null2, for this LSD profile.
+        and null2, for the LSD profile.
 
         The False Alarm Probability (FAP) is the probability that the observed
         data are consistent with the null hypothesis of no magnetic field.
         In this case, the null hypothesis is a flat line in Stokes V
         (an offset from 0 is allowed to account for continuum polarization).
         The probability is evaluated from chi^2.
         
@@ -489,50 +529,55 @@
             contN2 = np.sum(self.specN2/self.specSigN2**2) / np.sum(1./self.specSigN2**2)
             chi2N2 = np.sum(((self.specN2 - contN2)/self.specSigN2)**2)
             probN2 = 1.0-specialf.gammainc(approxDOF/2., chi2N2/2.)
         
         return(probV, probN1, probN2)
 
     def calc_bz(self, cog='I', norm='auto', lambda0=500., geff=1.2,
-                velrange=None, bzwidth=None, plot=True):
+                velrange=None, bzwidth=None, plot=True, **kwargs):
         '''Calculate the Bz of an LSD profile
         
-        :param cog: The value, or calculation method for the center of gravity.
+        :param cog: The value or calculation method for the center of gravity.
                     The choices are:
-                    'I': center of gravity of I,
-                    'V': center of gravity of V,
+                    'I': center of gravity of Stokes I,
+                    'V': center of gravity of Stokes V,
                     'IV': center of gravity of I*V,
+                    'min': velocity of the minimum of Stokes I,
                     or a float: a user defined value in km/s.
         :param norm: calculation method for the continuum. The choices are:
-                    'auto': the median of I outside of velrange (if defined)
+                    'auto': the median of I outside of velrange (if defined),
                     or the full range (if velrange is not defined),
                     or float: a user defined value to use for Ic.
         :param lambda0: wavelength of the transition in nanometers (default=500).
                     For an LSD profile, this is the lambda value the LSD
                     profile shape was scaled with.
         :param geff: effective Lande factor of the transition.
                     For an LSD profile, this is the geff value the LSD profile
                     shape was scaled with.
         :param velrange: range of velocity to use for the determination of the
-                    line center and the continuum. If not defined, the whole
-                    range will be used. If bzwidth is not defined, this range
-                    will also be used for the line Bz calculation.
-        :param bzwidth: distance from the line center for the Bz calculation.
+                    line center and the continuum. If bzwidth is not given,
+                    this range will also be used for the integration range
+                    in the Bz calculation. 
+                    If not given, the whole LSD profile will be used. 
+        :param bzwidth: distance from the line center (from the cog) used 
+                    for the integration range in the Bz calculation. 
                     One element = same on each side of line center.
-                    Two elements, left and right of line center.
-                    Not defined: using velrange.
-        :param plot: whether or not a graph is generated, and returned.
+                    Two elements = left and right of line center.
+                    Not given (default): instead use velrange for this.
+        :param plot: whether or not a graph is generated and returned.
+        :param kwargs: additional keyword arguments are passed to the
+                   matplotlib plotting routines, if a plot is generated.
         :return: a dictionary with Bz (in G) and FAP calculations,
                  optionally also a matplotlib figure.
         '''
         
-        # Velrange is used to identify the position of the line,
+        # velrange is used to identify the position of the line,
         # for calculating the cog, and for calculating the position
         # of the continuum.
-        # If Velrange is not defined, it will use the whole range.
+        # If velrange is not defined, it will use the whole range.
         # The range for calculating Bz itself is controlled by bzwidth below
         if velrange != None:
             inside = np.logical_and(self.vel>=velrange[0], self.vel<=velrange[1])
             lsd_in = self[inside]
             lsd_out = self[np.logical_not(inside)]
         else:
             lsd_in=copy.deepcopy(self)
@@ -540,15 +585,16 @@
         # Check if norm is a string.
         if isinstance(norm, str):
             print('using AUTO method for the normalization')
             if velrange != None:
                 print('  using the median of the continuum outside of the line')
                 norm_val = np.median(lsd_out.specI)
             else:
-                print('  no range in velocity given, using the median of the whole specI to determine continuum')
+                print('  no range in velocity given, using the median '
+                      +'of the whole specI to determine continuum')
                 norm_val = np.median(lsd_in.specI)
         else:
             norm_val = copy.copy(norm)
             print('using given norm value')
 
         # Check if cog is a string.
         if isinstance(cog, str):
@@ -558,51 +604,79 @@
             elif cog == 'min':
                 cog_val = lsd_in.cog_min()
             elif cog == 'IV':
                 cog_val = lsd_in.cog_IV(norm_val)
             elif cog == 'V':
                 cog_val = lsd_in.cog_V()
             else:
-                raise ValueError('calcBz got unrecognized value for cog: {:}'.format(cog))
+                raise ValueError('calcBz got unrecognized value for cog: '
+                                 +'{:}'.format(cog))
         else:
             cog_val=copy.copy(cog)
         
         # Now we define the position of the line for the Bz calculation itself.
         # If the keyword bzwidth is defined, we use that range from the chosen cog.
         if bzwidth == None:
             # No bzwidth. using vrange if defined
             if velrange != None:
                 print('no bzwidth defined, using velrange to calculate Bz')
                 lsd_bz = copy.copy(lsd_in)
                 # saving the range for plotting later.
                 p_bzwidth = np.copy(velrange)
             else:
-                print('no bzwidth nor velrange defined, using full velocity range to calculate Bz')
+                print('no bzwidth nor velrange defined, using full range to calculate Bz')
                 p_bzwidth = [self.vel.min(), self.vel.max()]
                 lsd_bz = copy.copy(self)
         else:
             # Check whether it is a numpy array
             if isinstance(bzwidth, list) or isinstance(bzwidth, tuple):
                 if len(bzwidth) == 1:
                     #print('list with one element')
                     # keeping the actual bz calculation range for plotting later.
                     p_bzwidth = [cog_val-bzwidth, cog_val+bzwidth]
-                    lsd_bz = self[ np.logical_and(self.vel >= p_bzwidth[0], self.vel <= p_bzwidth[1]) ]
+                    lsd_bz = self[ np.logical_and(self.vel >= p_bzwidth[0],
+                                                  self.vel <= p_bzwidth[1]) ]
                 elif len(bzwidth) == 2:
                     #print('list with two elements')
                     p_bzwidth = [cog_val-bzwidth[0], cog_val+bzwidth[1]]
-                    lsd_bz = self[ np.logical_and(self.vel >= p_bzwidth[0], self.vel <= p_bzwidth[1]) ]
+                    lsd_bz = self[ np.logical_and(self.vel >= p_bzwidth[0],
+                                                  self.vel <= p_bzwidth[1]) ]
                 else:
                     print('bzwidth has too many elements (need one or two)')
-                    raise ValueError('bzwidth has too many elements {:} (need 1 or 2)'.format(len(bzwidth)))
+                    raise ValueError('bzwidth has too many elements '
+                                     +'{:} (need 1 or 2)'.format(len(bzwidth)))
             else:
                 p_bzwidth = [cog_val-bzwidth, cog_val+bzwidth]
-                lsd_bz = self[ np.logical_and(self.vel >= p_bzwidth[0], self.vel <= p_bzwidth[1]) ]
+                lsd_bz = self[ np.logical_and(self.vel >= p_bzwidth[0],
+                                              self.vel <= p_bzwidth[1]) ]
+
+    
+        # Dealing with potential order overlaps 
+        # or uneven velocity grid
+        deltav_array = lsd_bz.vel[1:]-lsd_bz.vel[:-1]
+        if np.any(deltav_array < 0.0):
+            warnings.warn("\n The velocity array is not monotonically increasing. "
+                          "\n There might be an order overlap in the region of the "
+                          "observation used. \n calc_bz will sort the LSD "
+                          "profile in velocity order. \n Make sure this is what "
+                          "you want -- merge orders before running calc_bz()!",
+                          stacklevel=2)
+            lsd_bz = lsd_bz._sortvel()
+            deltav_array = lsd_bz.vel[1:]-lsd_bz.vel[:-1]
+
+        # check if the spacing is uneven by a lot
+        deltav_min = deltav_array.min()
+        deltav_max = deltav_array.max()
+        if (deltav_max - deltav_min) > 0.1 : # in km/s
+            warnings.warn("The velocity spacing is uneven: "
+                          "min spacing {}km/s, max spacing {}km/s".format(
+                              deltav_min, deltav_max), stacklevel=2)
 
         # Actual calculation of the Bz:
+
         # Call the integration function for each V, Null1, Null2 parameter
         blv, blvSig = _integrate_bz(lsd_bz.vel, lsd_bz.specV, lsd_bz.specSigV, 
                     geff, lambda0, cog_val, lsd_bz.specI, lsd_bz.specSigI, norm_val)
         if self.numParam > 2:
             bln1, bln1Sig = _integrate_bz(lsd_bz.vel, lsd_bz.specN1, lsd_bz.specSigN1,
                     geff, lambda0, cog_val, lsd_bz.specI, lsd_bz.specSigI, norm_val)
         else: bln1, bln1Sig = (0.0, 0.0)
@@ -625,21 +699,28 @@
                 'N1 bz (G)': bln1,
                 'N1 bz sig (G)': bln1Sig,
                 'N1 FAP': FAP_N1,
                 'N2 bz (G)': bln2,
                 'N2 bz sig (G)': bln2Sig,
                 'N2 FAP': FAP_N2
                 }
+                #maybe rename:
+                #'int. range start': p_bzwidth[0],
+                #'int. range end': p_bzwidth[1]
 
         if plot:
             fig  = _plot_bz_calc(self, lsd_in, lsd_bz, velrange,
-                            p_bzwidth, norm_val, cog_val, cog)
+                            p_bzwidth, norm_val, cog_val, cog, **kwargs)
             return result,fig
         else:
             return result
+        
+    def _sortvel(self):
+        n = np.argsort(self.vel)
+        return self[n]
 
 ##################
 ##################
 
 def _gaussProf(x, cont, ampl, center, width):
     """
     Define a simple Gaussian line profile (for fitting with)
@@ -647,16 +728,16 @@
     y = cont - ampl*np.exp(-(x-center)**2/(2.*width**2))
     return y
 
 
 def _integrate_bz(vel, spec, specSig, geff, lambda0, cog_val,
                   specI, specSigI, norm_val):
     '''
-    Helper function that is used in the Bz calculations. Internal.
-    to integrate one Stokes parameter. 
+    Helper function that is used in the Bz calculations to integrate one Stokes parameter. 
+    Internal.
 
     :param vel: (numpy array) the velocity array
     :param spec: (numpy array) the associated Stokes parameter array
     :param specSig: (numpy array) the error bar on the Stokes parameter
     :param geff: the effective lande factor of the profile
     :param lambda0: the nominal wavelength of the profile
     :cog_val: the chose center of gravity value (km/s)
@@ -669,55 +750,86 @@
     # This is the constant for the Zeeman splitting
     # Lambda_B = constant * lambda0**2 B
     # lambda_B_constant = e/(4*pi*m_e*c) = 4.668644778304102e-05 in cgs units
     lambda_B_constant = 4.668644778304102e-12 #to match/cancel lambda0 in nm
     cvel = 2.99792458e5 #c in km/s to match/cancel the LSD profile velocities
     
     # set the velocity step for error propagation
-    deltav = (vel[1] - vel[0]) # This is in km/s
-    
+    # (There might be some issues with order overlap if the function is used
+    # with an LSD object that was calculated with individual_line function. )
+    ###
+    # For trapezoidal integration
+    # A = sum of  0.5 [ x_(i+1) - x_(i) ]*[ Y_(i) + Y_(i+1) ] (from i=1 to i=N-1)
+    # If we define dx_i = x_(i+1) - x_(i) we can rewrite this as:
+    # A = sum of 0.5*dx_(i)*[ Y_(i) + Y_(i+1) ]  (from i=1 to i=N-1)
+    # if we expand the sum, and gather all of the Y_i together, we get:
+    # dx_1 Y_1 + [dx_1+dx_2]Y_2 + [dx_2+dx_3]Y_3 +
+    #      ... + [dx_{N-2}+dx_{N-1}]Y_{N-1} + dx_{N-1} Y_N
+    # Now, assuming uncertainties only on the Y_i, of s_i, the propagated error is
+    # error^2 = 0.5 * ( (dx_1 s_1)**2 + ([dx_1+dx_2]s_2)**2 + ([dx_2+dx_3]s_3)**2 +
+    #           ... +  ([dx_{N-2}+dx_{N-1}]*s_{N-1})**2 + (dx_{N-1} s_N)**2 )
+    # numerically, if we have: vel = [x_1, x_2, x_3, ..., x_n],
+    #              then: vel[1:]-vel[:-1] = [dx_1, dx_2, dx_3, ..., dx_{n-1}]
+    # adding a zero at each end: [0, dx1, dx2, dx3, ..., dx_(n-1), 0], and doing [1:]+[:-1] 
+    # will give us the array that we need to multiply with the s_i array. Et voila!
+    ###
+    #deltav_arr = vel[1:] - vel[:-1]
+    #dx = np.hstack([0., deltav_arr, 0.])
+    #err_scale = 0.5*(dx[:-1] + dx[1:])
+    # or more intuitively to Colin (and marginally faster):
+    deltav_arr = vel[1:] - vel[:-1]
+    err_scale = deltav_arr[:-1] + deltav_arr[1:]
+    err_scale = 0.5*np.concatenate((deltav_arr[:1], err_scale, deltav_arr[-1:]))
+
     # Calculation of the integral in the numerator of the Bz function
     # with a trapezoidal numerical integral
-    # For the error calculation, we propagate like we would for
-    # summation in a numerical integral.
-    fnum = np.trapz( (vel - cog_val) * spec, x=vel-cog_val ) #in (km/s)^2
-    sfnum = np.sqrt(np.sum( (vel - cog_val )**2 * specSig**2 ) * deltav**2)
+    fnum = np.trapz((vel - cog_val) * spec, x=vel-cog_val) #in (km/s)^2
+    sfnum = np.sqrt(np.sum(((vel - cog_val) * specSig * err_scale)**2))
+    # for a constant pixel spacing deltav (with the end points treated exactly)
+    #sfnumConst = np.sqrt((0.5*(vel[0] - cog_val)*specSig[0]*deltav)**2
+    #               + np.sum(((vel[1:-1] - cog_val)*specSig[1:-1])**2)*deltav**2
+    #               + (0.5*(vel[-1] - cog_val)*specSig[-1]*deltav)**2)
     
     # Calculation of the integral in the denominator of the Bz function
     # with a trapezoidal numerical integral
     # For the square error calculation, we propagate like we would for
     # summation in a numerical integral.
-    ri0v = np.trapz(norm_val-specI, x=vel ) # in km/s
-    si0v = np.sqrt(np.sum(specSigI**2 )* deltav**2) # in km/s
+    ri0v = np.trapz(norm_val - specI, x=vel) # in km/s
+    si0v = np.sqrt(np.sum((specSigI * err_scale)**2)) # in km/s
+    # for a constant pixel spacing deltav (with the end points treated exactly)
+    #si0vConst = np.sqrt((0.5*specSigI[0]*deltav)**2
+    #                    + np.sum(specSigI[1:-1]**2)*deltav**2
+    #                    + (0.5*specSigI[-1]*deltav)**2)
     
     # Make the actual Bz calculation.
     # for the units to work out, lambda0 should be in nm
-    bl = -1*fnum / ( ri0v*geff*lambda0*cvel*lambda_B_constant)
-    blSig = np.abs(bl * np.sqrt( (sfnum/fnum)**2 + (si0v/ri0v)**2 ))
+    bl = -1*fnum / (ri0v*geff*lambda0*cvel*lambda_B_constant)
+    blSig = np.abs(bl * np.sqrt((sfnum/fnum)**2 + (si0v/ri0v)**2))
     return bl, blSig
 
 
-def _plot_bz_calc(lsd, lsd_in, lsd_bz, velrange, p_bzwidth, norm_val, cog_val, cog):
+def _plot_bz_calc(lsd, lsd_in, lsd_bz, velrange, p_bzwidth, norm_val, cog_val, cog,
+                  **kwargs):
     """
     Generate a plot showing the center of gravity and integration ranges used
-    in the calculation of Bz from and LSD profile.  Called by the calc_bz
+    in the calculation of Bz from an LSD profile.  Called by the calc_bz
     function. Mostly just for internal use.
 
     :param lsd: the full LSD profile to plot
     :param lsd_in: slice of an LSD profile with the range used for COG calculation
     :param lsd_bz: slice of an LSD profile with the range used for integration of Bz
     :param velrange: the velocity range used for COG calculation
     :param p_bzwidth: the velocity range used for integration of Bz
     :param norm_val: the continuum level used for normalization
     :param cog_val: the final COG used for Bz calculation
     :param cog: the input COG flag/value given by the user
     :return: a matplotlib figure object
     """
     #This function relies on the plot method of the LSD profile class
-    fig, ax = lsd.plot(sameYRange=False)
+    fig, ax = lsd.plot(sameYRange=False, **kwargs)
     
     for item in ax:
         if velrange != None:
             item.axvline(x=velrange[0], ls='--', label='velrange')
             item.axvline(x=velrange[1], ls='--')
         item.axvline(x=p_bzwidth[0], ls='dotted', label='bzwidth')
         item.axvline(x=p_bzwidth[1], ls='dotted')
@@ -747,18 +859,18 @@
         ax[2].fill_between(lsd_bz.vel[blue], lsd_bz.specN2[blue], step='mid', color='blue')
     
     return fig
 
 
 def read_lsd(fname):
     """
-    Read in an LSD profile and return an instance of the LSD class
+    Read in an LSD profile and return an instance of the LSD class.
     
-    The LSD profiles are in Donati's text format.
-    However, the two lines of header in Donati's format are optional.
+    The LSD profiles are in Donati's text format;
+    however, the two lines of header in Donati's format are optional.
     
     :param fname: the name of the file containing the LSD profile
     :rtype: LSD
     """
     #check if this file has a header
     fcheck = open(fname, 'r')
     head1txt = fcheck.readline()
@@ -829,86 +941,127 @@
     if ncols != 3 and ncols != 7 and ncols != 9:
         raise ValueError("Read an unexpected number of columns from "
                          +"{:}, can't read as an LSD profile.".format(fname))
     return prof
 
 ###################################
 
-def run_lsdpy(obs=None, mask=None, outName='prof.dat',
-              velStart=None, velEnd=None, velPixel=None, 
+def run_lsdpy(obs, mask, outLSDName=None,
+              velStart=-200.0, velEnd=+200.0, velPixel=None, 
               normDepth=0.2, normLande=1.2, normWave=500.0,
-              removeContPol=1, trimMask=1, sigmaClipIter=0,
-              sigmaClip=500, interpMode=1, outModelName='',
-              fLSDPlotImg=1, fSavePlotImg=0, outPlotImgName='figProf.pdf'):
+              removeContPol=True, trimMask=True, sigmaClipIter=0,
+              sigmaClip=500, outModelName=None,
+              plotLSD=True,  outPlotLSDName=None):
     """
     Run the LSDpy code and return an LSD object  
-    (a convenience wrapper around the lsdpy.main() function)
+    (a convenience wrapper around the lsdpy.main() function).
 
-    This requires LSDpy to be installed and in your Python path.
-    (see https://github.com/folsomcp/LSDpy )
+    This requires LSDpy to be installed and in your Python path,
+    which should be installed if you installed specpolFlow with pip
+    (see https://github.com/folsomcp/LSDpy ).
     
-    Any arguments not specified will be read from the file inlsd.dat.
-    The file inlsd.dat is optional, but if the file does not exist and 
-    any arguments are 'None', the program will error and halt.
-    Some arguments have default values, which will be used if they are not
-    explicitly specified and if the inlsd.dat file is missing.
+    While some reasonable default values are included, pay attention to
+    the parameters: velPixel, normDepth, normLande, normWave, and outName.
     
     Arguments are: 
     
     :param obs:           name of the input observed spectrum file
     :param mask:          name of the input LSD mask file
-    :param outName:       name of the output LSD profile (Default = 'prof.dat')
+    :param outLSDName:    if provided, save the output LSD profile to this
+                          file (Default = None, not saved)
     :param velStart:      float, starting velocity for the LSD profile (km/s)
     :param velEnd:        float, ending  velocity (km/s)
-    :param velPixel:      float, velocity pixel size (km/s)
+    :param velPixel:      float, velocity pixel size (km/s). If not provided,
+                          this will be the median pixel size in the observation,
+                          however it is recommended to set this explicitly.
     :param normDepth:     float, normalizing line depth
     :param normLande:     float, normalizing effective Lande factor
     :param normWave:      float, normalizing wavelength
-    :param removeContPol: int, flag for whether continuum polarization is 
-                          subtracted from the LSD profile (0=no, 1=yes)
-                          (Default = 1)
-    :param trimMask:      int, flag for whether very closely spaced lines 
-                          should be removed from the line mask (0=no, 1=yes)
-                          (Default = 1)
+    :param removeContPol: flag for whether continuum polarization is 
+                          subtracted from the LSD profile
+                          (Default = True)
+    :param trimMask:      flag for whether very closely spaced lines 
+                          should be removed from the line mask
+                          (Default = True)
     :param sigmaClipIter: int, number of iterations for sigma clipping, 
                           rejecting possible bad pixels based on the fit to
                           Stokes I. Set to 0 for no sigma clipping.
                           (Default = 0, no sigma clipping)
     :param sigmaClip:     float, if sigma clipping, reject pixels where the
                           observation differs from the model by more than this
                           number of sigma.  Should be a large value so only very
                           bad pixels are rejected.
                           (Default = 500.)
-    :param interpMode:    int, mode for interpolating the model on to the
-                          observation during LSD 0 = nearest neighbour,
-                          1 = linear interpolation.
-                          (Default = 1)
-    :param outModelName:  name of the file for the output model spectrum 
-                          (if saved). If this is '' a model 
-                          will be generated but not saved to file.
-                          (Default = '')
-    :param fLSDPlotImg:   int, flag for whether to plot the LSD profile
-                          (using matplotlib) (0=no, 1=yes)
-                          (Default = 1)
-    :param fSavePlotImg:  int, flag for whether to save the plot of the 
-                          LSD profile (0=no, 1=yes)
-                          (Default = 0)
-    :param outPlotImgName: name of the plotted figure of the LSD profile 
-                          (if saved) (Default = 'figProf.pdf')
+    :param outModelName:  if provided, save the output model spectrum to this
+                          file  (Default = None, not saved)
+    :param plotLSD:       flag for whether to plot the LSD profile
+                          (using matplotlib) (Default = True)
+    :param outPlotLSDName: if provided, save the the plotted figure of the LSD 
+                           profile  to this file (e.g. 'figProf.pdf'). Supports
+                           the output file formats using the matplotlib savefig
+                           function.
     :return: an LSD profile object, and a 'Spectrum' object containing the model
                           spectrum (the fit to the observation,
                           i.e. the convolution of the line mask and LSD profile)
     """
     import LSDpy
 
+    # Passing LSD calculation controls to the LSDpy.lsd call
+    interpMode = 1
+    if removeContPol is False:
+        _removeContPol = 0
+    else:
+        _removeContPol = 1
+    if trimMask is False:
+        _trimMask = 0
+    else:
+        _trimMask = 1
+
+    # Passing figure generation and saving controls to the LSDpy.lsd call
+    if plotLSD is False:
+        _fLSDPlotImg = 0
+    else:
+        _fLSDPlotImg = 1
+    if outPlotLSDName is None:
+        _fSavePlotImg = 0
+        _outPlotImgName = ''
+    else:
+        _fSavePlotImg = 1
+        _outPlotImgName = outPlotLSDName
+
+    # Make a default calculation for the pixel spacing if not user-defined
+    if velPixel is None:
+        #Get average observed wavelength spacing
+        cvel = 2.99792458e5 #c in km/s
+        obsSp = read_spectrum(obs)
+        wlStep = obsSp.wl[1:] - obsSp.wl[:-1]
+        medianVelPix = np.median(wlStep/obsSp.wl[:-1]*cvel)
+        #indWlSteps = ((wlStep > 0.) & (wlStep < 0.5))
+        #meanVelPix = np.average(wlStep[indWlSteps]/obsSp.wl[:-1][indWlSteps]*cvel)        
+        velPixel = round(medianVelPix, ndigits=2)
+
+    # Set the controls to the call to LSDpy for saving the files if needed.
+    if outModelName is None:
+        _outModelName = ''
+    else:
+        _outModelName = outModelName
+    _fSaveModelS = 1     # and set the model spectrum calculation flag
+
+    if outLSDName is None:
+        _outLSDName = ''
+    else:
+        _outLSDName = outLSDName
+        
+    # Make the call to LSDpy.py
     vel, sI, sIerr, sV, sVerr, sN1, sN1err, headerTxt, specList = LSDpy.lsd(
-        obs, mask, outName, velStart, velEnd, velPixel, 
-        normDepth, normLande, normWave, removeContPol, trimMask, 
-        sigmaClipIter, sigmaClip, interpMode, 1, outModelName, 
-        fLSDPlotImg, fSavePlotImg, outPlotImgName)
+        obs, mask, _outLSDName, velStart, velEnd, velPixel, 
+        normDepth, normLande, normWave, _removeContPol, _trimMask, 
+        sigmaClipIter, sigmaClip, interpMode, _fSaveModelS, _outModelName, 
+        _fLSDPlotImg, _fSavePlotImg, _outPlotImgName)
 
     prof = LSD(vel, sI, sIerr, sV, sVerr, sN1, sN1err, header=headerTxt)
     modelSpec = Spectrum(specList[0], specList[1], specList[2], specList[3],
                             np.zeros_like(specList[0]), np.zeros_like(specList[0]))
+    
     return prof, modelSpec
 
 ###################################
```

### Comparing `specpolFlow-0.3.4/specpolFlow.egg-info/PKG-INFO` & `specpolflow-0.4.0/specpolFlow.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: specpolFlow
-Version: 0.3.4
+Version: 0.4.0
 Summary: Tools for the analysis of stellar spectropolarimetric data
 Author-email: SpecpolFlow Team <specpolflow@gmail.com>
 Project-URL: Homepage, https://github.com/folsomcp/specpolFlow
 Project-URL: Documentation, https://folsomcp.github.io/specpolFlow/
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Astronomy
```

### Comparing `specpolFlow-0.3.4/specpolFlow.egg-info/SOURCES.txt` & `specpolflow-0.4.0/specpolFlow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

