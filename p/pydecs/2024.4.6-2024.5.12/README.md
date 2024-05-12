# Comparing `tmp/pydecs-2024.4.6.tar.gz` & `tmp/pydecs-2024.5.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydecs-2024.4.6.tar", last modified: Sat Apr  6 08:01:57 2024, max compression
+gzip compressed data, was "pydecs-2024.5.12.tar", last modified: Sun May 12 11:26:58 2024, max compression
```

## Comparing `pydecs-2024.4.6.tar` & `pydecs-2024.5.12.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0 ogawa     (1000) ogawa     (1000)        0 2024-04-06 08:01:57.842695 pydecs-2024.4.6/
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)    11357 2024-04-06 07:44:30.000000 pydecs-2024.4.6/LICENSE.txt
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)      646 2024-04-06 08:01:57.834600 pydecs-2024.4.6/PKG-INFO
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)      484 2024-04-06 07:44:30.000000 pydecs-2024.4.6/README.md
-drwxrwxrwx   0 ogawa     (1000) ogawa     (1000)        0 2024-04-06 08:01:57.596332 pydecs-2024.4.6/pydecs/
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)      257 2024-04-06 07:44:30.000000 pydecs-2024.4.6/pydecs/__init__.py
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)    36214 2024-04-06 07:44:30.000000 pydecs-2024.4.6/pydecs/aux_EdefCorrection_VASP.py
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)     2700 2024-04-06 07:59:58.000000 pydecs-2024.4.6/pydecs/aux_check_equilibrium_phases.py
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)     6569 2024-04-06 07:44:30.000000 pydecs-2024.4.6/pydecs/aux_convDOS.py
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)     1343 2024-04-06 07:44:30.000000 pydecs-2024.4.6/pydecs/aux_convGasEne.py
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)     1855 2024-04-06 07:44:30.000000 pydecs-2024.4.6/pydecs/aux_plot_defectdata.py
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)      671 2024-04-06 07:44:30.000000 pydecs-2024.4.6/pydecs/common.py
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)    13630 2024-04-06 07:44:30.000000 pydecs-2024.4.6/pydecs/defects.py
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)    22348 2024-04-06 07:44:30.000000 pydecs-2024.4.6/pydecs/eqcond.py
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)     7104 2024-04-06 07:44:30.000000 pydecs-2024.4.6/pydecs/host.py
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)    67472 2024-04-06 07:44:30.000000 pydecs-2024.4.6/pydecs/inout.py
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)     4681 2024-04-06 07:44:30.000000 pydecs-2024.4.6/pydecs/pydecs.py
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)     9491 2024-04-06 07:44:30.000000 pydecs-2024.4.6/pydecs/reference_phases.py
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)    32689 2024-04-06 07:44:30.000000 pydecs-2024.4.6/pydecs/solver.py
-drwxrwxrwx   0 ogawa     (1000) ogawa     (1000)        0 2024-04-06 08:01:57.816057 pydecs-2024.4.6/pydecs.egg-info/
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)      646 2024-04-06 08:01:56.000000 pydecs-2024.4.6/pydecs.egg-info/PKG-INFO
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)      570 2024-04-06 08:01:57.000000 pydecs-2024.4.6/pydecs.egg-info/SOURCES.txt
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)        1 2024-04-06 08:01:56.000000 pydecs-2024.4.6/pydecs.egg-info/dependency_links.txt
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)      420 2024-04-06 08:01:56.000000 pydecs-2024.4.6/pydecs.egg-info/entry_points.txt
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)        1 2024-04-06 08:01:56.000000 pydecs-2024.4.6/pydecs.egg-info/not-zip-safe
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)       35 2024-04-06 08:01:56.000000 pydecs-2024.4.6/pydecs.egg-info/requires.txt
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)        7 2024-04-06 08:01:56.000000 pydecs-2024.4.6/pydecs.egg-info/top_level.txt
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)       91 2024-04-06 07:44:30.000000 pydecs-2024.4.6/pyproject.toml
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)     1098 2024-04-06 08:01:57.853235 pydecs-2024.4.6/setup.cfg
+drwxrwxrwx   0 ogawa     (1000) ogawa     (1000)        0 2024-05-12 11:26:58.846746 pydecs-2024.5.12/
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)    11357 2024-05-11 20:28:14.000000 pydecs-2024.5.12/LICENSE.txt
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)      647 2024-05-12 11:26:58.846746 pydecs-2024.5.12/PKG-INFO
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)      484 2024-05-11 20:28:14.000000 pydecs-2024.5.12/README.md
+drwxrwxrwx   0 ogawa     (1000) ogawa     (1000)        0 2024-05-12 11:26:58.690245 pydecs-2024.5.12/pydecs/
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)      257 2024-05-11 20:28:14.000000 pydecs-2024.5.12/pydecs/__init__.py
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)    36214 2024-05-11 20:28:14.000000 pydecs-2024.5.12/pydecs/aux_EdefCorrection_VASP.py
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)     2700 2024-05-11 20:28:14.000000 pydecs-2024.5.12/pydecs/aux_check_equilibrium_phases.py
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)     6716 2024-05-12 11:10:05.000000 pydecs-2024.5.12/pydecs/aux_convDOS.py
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)     1343 2024-05-11 20:28:14.000000 pydecs-2024.5.12/pydecs/aux_convGasEne.py
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)     1855 2024-05-11 20:28:14.000000 pydecs-2024.5.12/pydecs/aux_plot_defectdata.py
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)      671 2024-05-11 20:28:14.000000 pydecs-2024.5.12/pydecs/common.py
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)    13639 2024-05-11 20:28:14.000000 pydecs-2024.5.12/pydecs/defects.py
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)    22355 2024-05-11 20:28:14.000000 pydecs-2024.5.12/pydecs/eqcond.py
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)     7626 2024-05-12 10:53:59.000000 pydecs-2024.5.12/pydecs/host.py
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)    68598 2024-05-11 20:28:14.000000 pydecs-2024.5.12/pydecs/inout.py
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)     4688 2024-05-11 20:28:14.000000 pydecs-2024.5.12/pydecs/pydecs.py
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)     9571 2024-05-11 20:28:14.000000 pydecs-2024.5.12/pydecs/reference_phases.py
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)    32686 2024-05-11 20:28:14.000000 pydecs-2024.5.12/pydecs/solver.py
+drwxrwxrwx   0 ogawa     (1000) ogawa     (1000)        0 2024-05-12 11:26:58.831127 pydecs-2024.5.12/pydecs.egg-info/
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)      647 2024-05-12 11:26:58.000000 pydecs-2024.5.12/pydecs.egg-info/PKG-INFO
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)      570 2024-05-12 11:26:58.000000 pydecs-2024.5.12/pydecs.egg-info/SOURCES.txt
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)        1 2024-05-12 11:26:58.000000 pydecs-2024.5.12/pydecs.egg-info/dependency_links.txt
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)      420 2024-05-12 11:26:58.000000 pydecs-2024.5.12/pydecs.egg-info/entry_points.txt
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)        1 2024-05-12 11:26:57.000000 pydecs-2024.5.12/pydecs.egg-info/not-zip-safe
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)       35 2024-05-12 11:26:58.000000 pydecs-2024.5.12/pydecs.egg-info/requires.txt
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)        7 2024-05-12 11:26:58.000000 pydecs-2024.5.12/pydecs.egg-info/top_level.txt
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)       91 2024-05-11 20:28:14.000000 pydecs-2024.5.12/pyproject.toml
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)     1098 2024-05-12 11:26:58.846746 pydecs-2024.5.12/setup.cfg
```

### Comparing `pydecs-2024.4.6/LICENSE.txt` & `pydecs-2024.5.12/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pydecs-2024.4.6/PKG-INFO` & `pydecs-2024.5.12/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydecs
-Version: 2024.4.6
+Version: 2024.5.12
 Summary: This tool enables us to analyze equilibrium concentrations of point and complex defects in crystalline solids
 Home-page: https://gitlab.com/tkog/pydecs
 Author: Takafumi Ogawa
 Author-email: takafumi.ogawa.1+pydecs@gmail.com
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Topic :: Scientific/Engineering :: Physics
```

### Comparing `pydecs-2024.4.6/pydecs/aux_EdefCorrection_VASP.py` & `pydecs-2024.5.12/pydecs/aux_EdefCorrection_VASP.py`

 * *Files identical despite different names*

### Comparing `pydecs-2024.4.6/pydecs/aux_check_equilibrium_phases.py` & `pydecs-2024.5.12/pydecs/aux_check_equilibrium_phases.py`

 * *Files identical despite different names*

### Comparing `pydecs-2024.4.6/pydecs/aux_convDOS.py` & `pydecs-2024.5.12/pydecs/aux_convDOS.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 # Licensed under the Apache License, Version2.0.
 #---------------------------------------------------------------------------
 # Auxiliary tool of pydecs library for producing inpydecs_dos.csv file
 #---------------------------------------------------------------------------
 import os,sys
 import datetime
 import matplotlib.pyplot as plt
+import math 
 
 def convDOSfromVASP():
     print(" Preparing \"inpydecs_dos.csv\" from VASP-output files in the current directory.")
     print(" Parsed files: DOSCAR, OUTCAR, EIGENVAL")
     if not os.path.exists("OUTCAR"):
         print("ERROR::file_not_found: OUTCAR")
         sys.exit()
@@ -114,53 +115,58 @@
             for i3,occ3 in enumerate(occlist):
                 if occ3 >0.5:
                     if E_VBM<elist[i3]:
                         E_VBM=elist[i3]
                 elif occ3<0.1:
                     if E_CBM>elist[i3]:
                         E_CBM=elist[i3]
-    E_gap=E_CBM-E_VBM
     fin=open("DOSCAR")
     for i1 in range(6):
         l1=fin.readline()
     enelist=[]
     doslist=[]
     l1=fin.readline()
     for i1 in range(NEDOS-1):
         l2=fin.readline().split()
         enelist.append(float(l2[0]))
         dsum=0.0
         for d1 in l2[1:1+NSPIN]:
             dsum+=float(d1)
         doslist.append(dsum)
+    E_gap=E_CBM-E_VBM
 
-    fout=open("inpydecs_dos.csv","w")
+    fnout_dos = "inpydecs_dos.csv"
+    fout=open(fnout_dos,"w")
     fout.write("##############################\n")
     fout.write("# Produced by pydecs-aux-tool\n")
     dt1=str(datetime.datetime.today())
     fout.write("# Time = "+dt1[:dt1.rfind(":")]+"\n")
     fout.write("# ELEMENTS = ")
     for e1 in elems:
         fout.write(e1+" ")
     fout.write("\n")
     fout.write("# NATOMS = ")
+    natoms_tot=0
     for n1 in natoms:
         fout.write(str(n1)+" ")
+        natoms_tot+=n1
     fout.write("\n")
-    fout.write("# NATOMStot = "+str(NIONS)+"\n")
+    # fout.write("# NATOMStot = "+str(natoms_tot)+"\n")
     fout.write("# Volume = "+str(volume)+" [A^3]\n")
-    fout.write("# Egap = "+str(E_gap)+" [eV]\n")
     fout.write("# EVBM = "+str(E_VBM)+" [eV]\n")
-    fout.write("# NEDOS = "+str(NEDOS-1)+"\n")
+    fout.write("# ECBM = "+str(E_CBM)+" [eV]\n")
+    fout.write("# Egap = "+str(E_gap)+" [eV]\n")
+    fout.write("# NEDOS = "+str(len(enelist))+"\n")
+    # fout.write("# NEDOS = "+str(NEDOS-1)+"\n")
     fout.write("##############################\n")
     fout.write("# energy,dos\n")
     for i2,e2 in enumerate(enelist):
         fout.write(str(e2)+","+str(doslist[i2])+"\n")
     fout.close()
-    print(" Finished: Output filename = inpydecs_dos.csv") 
+    print(" Finished: Output filename = "+fnout_dos) 
     print("-"*100)
 
     plt.figure(figsize=(7,6))
     plt.tick_params(axis="x",direction="in",top=True)
     plt.tick_params(axis="y",direction="in",right=True)
     plt.plot(enelist,doslist,"k-",linewidth=2.0)
     plt.xlim([enelist[0],enelist[-1]])
@@ -168,16 +174,10 @@
     plt.axvline(E_VBM,color="tab:red",ls="--",lw=1.5)
     plt.axvline(E_CBM,color="tab:red",ls="--",lw=1.5)
     plt.xlabel(r"$\mathrm{Energy\ [eV]}$",size=14)
     plt.ylabel(r"$\mathrm{Dinsity\ of\ states\ [/cell]}$",size=14)
     plt.savefig("inpydecs_dos.png",dpi=200,bbox_inches="tight")
     plt.close()
 
-
-    plt.figure()
-    plt.plot()
-
 if __name__=="__main__":
     convDOSfromVASP()
 
-
-
```

### Comparing `pydecs-2024.4.6/pydecs/aux_convGasEne.py` & `pydecs-2024.5.12/pydecs/aux_convGasEne.py`

 * *Files identical despite different names*

### Comparing `pydecs-2024.4.6/pydecs/aux_plot_defectdata.py` & `pydecs-2024.5.12/pydecs/aux_plot_defectdata.py`

 * *Files identical despite different names*

### Comparing `pydecs-2024.4.6/pydecs/common.py` & `pydecs-2024.5.12/pydecs/common.py`

 * *Files identical despite different names*

### Comparing `pydecs-2024.4.6/pydecs/defects.py` & `pydecs-2024.5.12/pydecs/defects.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 #!/usr/bin/env python
 #---------------------------------------------------------------------------
 # Copyright 2021 Takafumi Ogawa
 # Licensed under the Apache License, Version2.0.
 #---------------------------------------------------------------------------
 # pydecs-defects module
 #---------------------------------------------------------------------------
-import os,sys
+import os
+import sys
 import copy
 import random
 import numpy as np
 from scipy.special import expit
 from scipy.special import expm1
 
 from pydecs.host import Host
@@ -80,16 +81,16 @@
                 at2=self.host.get_atom_at_site(s3)
                 if at2 in deltaNum_atoms.keys():
                     deltaNum_atoms[at2]-=occ3
         return (deltaNum_atoms,occ_sites,primary_occ_site)
 
     def __init__(self,host_in,elemsList_in,input_paths=["./"],densform_in="v2",root_outfiles=None):
         fout_lm=open(root_outfiles+"_loading_messages.txt","a")
-        print(" Reading defects-information")
-        fout_lm.write(" Reading defects-information\n")
+        print(" Reading defect information")
+        fout_lm.write(" Reading defect information\n")
         self.densform=densform_in
         if self.densform=="v1" or self.densform=="v2":
             print(f"   Selected density formulation: {self.densform}")
             fout_lm.write(f"   Selected density formulation: {self.densform}\n")
         else:
             print(f"   ERROR:: not-supported density formulation is given: {self.densform}")
             sys.exit()
@@ -110,15 +111,15 @@
         
         fnin="NONE"
         for path1 in input_paths:
             if os.path.exists(path1+"inpydecs_defects.csv"):
                 fnin=path1+"inpydecs_defects.csv"
                 break
         if fnin=="NONE":
-            print(" ERROR::file not-found: inpydecs_defects.csv")
+            print(" ERROR::file not found: inpydecs_defects.csv")
             sys.exit()
         print("   Reading file: "+fnin)
         fout_lm.write("   Reading file: "+fnin+"\n")
         fin=open(fnin).readlines()
         columns=[ t1.strip() for t1 in fin[0].split(",")]
         column_names=set(["commentout","defect_type","charge","energy_defect","energy_perfect"
             ,"energy_correction","multiplicity","line_color","line_style","line_width"])
@@ -341,7 +342,8 @@
 
     def get_line_width(self,defType_in):
         return self.data_defects[defType_in]["line_width"]
 
     def set_espot(self,espot_in):
         self.espot=espot_in
         return
+
```

### Comparing `pydecs-2024.4.6/pydecs/eqcond.py` & `pydecs-2024.5.12/pydecs/eqcond.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 #!/usr/bin/env python
 #---------------------------------------------------------------------------
 # Copyright 2021 Takafumi Ogawa
 # Licensed under the Apache License, Version2.0.
 #---------------------------------------------------------------------------
 # pydecs-eqcond module
 #---------------------------------------------------------------------------
-import os,sys
+import os
+import sys
 import copy
 import numpy as np
 from pydecs.reference_phases import ReferencePhases
 from pydecs.common import product_local
 
 class EquilibriumConditions:
 
@@ -27,22 +28,22 @@
         print(" Reading equilibrium conditions (eq)")
         fout1.write(" Reading equilibrium conditions (eq)\n")
         ### constructing conditions
         temperatures_list=[]
         if "temperature" in input_params:
             temp_params=input_params["temperature"]
             if "tempK_min" in temp_params:
-                print(" Error:: temK_min(max) were changed to tempK_start(end)")
-                print("         Other parameters to set a parameter range were also.")
-                print(" Very sorry for this forced chage!")
+                print(" Error:: temK_min(max) was changed to tempK_start(end)")
+                print("         Other parameter ranges were also altered.")
+                print(" Very sorry for this forced change!")
                 sys.exit()
             if "tempK_start" in temp_params:
                 temp_min=temp_params["tempK_start"]
             else:
-                print(" ERROR(temperatures):: missed tempK_start")
+                print(" ERROR(temperatures):: missing tempK_start")
                 sys.exit()
             if "tempK_end" in temp_params:
                 temp_max=temp_params["tempK_end"]
             else:
                 temp_max=temp_min
             if "tempK_num" in temp_params:
                 temp_num=temp_params["tempK_num"]
@@ -57,15 +58,15 @@
                     print(str1)
                     fout1.write(str1+"\n")
                     str1=len1*" "
                 str1+=f"{t1:7.2f}, "
             print(str1[:-2])
             fout1.write(str1[:-2]+"\n")
         else:
-            print(" ERROR(eq.temperature):: missed temperature")
+            print(" ERROR(eq.temperature):: missing temperature")
             sys.exit()
         ###############################################
         ### Reading fix_Natoms
         self.elements_fix_Natoms=[]
         self.Natoms_list=[]
         self.Natoms_chempot_init=[]
         if "fix_Natoms" in input_params:
@@ -76,54 +77,54 @@
                 nat2_min="NONE"
                 nat2_max="NONE"
                 nat2_num=0
                 nat2_log=False
                 if "numCell_array" in params2:
                     nat2_array=params2["numCell_array"]
                 if "numCell_min" in params2:
-                    print(" Error:: numCell_min(max) were changed to numCell_start(end)")
-                    print("         Other parameters to set a parameter range were also.")
-                    print(" Very sorry for this forced chage!")
+                    print(" Error:: numCell_min(max) was changed to numCell_start(end)")
+                    print("         Other parameter ranges were also altered.")
+                    print(" Very sorry for this forced change!")
                     sys.exit()
                 if "numCell_start" in params2:
                     nat2_min=params2["numCell_start"]
                 if "numCell_end" in params2:
                     nat2_max=params2["numCell_end"]
                 if "numCell_num" in params2:
                     nat2_num=params2["numCell_num"]
                 if "numCell_log" in params2:
                     nat2_log=params2["numCell_log"]
                 if "chempot_init" in params2:
                     cpinit2=params2["chempot_init"]
                 else:
-                    print(" ERROR(eq.fix_Natoms):: missed chempot_init for "+e2)
-                    print("   If this block isn't used, please comment out.")
+                    print(" ERROR(eq.fix_Natoms):: missing chempot_init for "+e2)
+                    print("   If this block isn't used, please comment it out.")
                     sys.exit()
                 if len(nat2_array)>0:
                     self.Natoms_list.append(np.array(nat2_array))
                 else:
                     if nat2_num==0:
-                        print(" ERROR(eq.fix_Natoms):: missed numCell_num for "+e2)
-                        print("   If this block isn't used, please comment out.")
+                        print(" ERROR(eq.fix_Natoms):: missing numCell_num for "+e2)
+                        print("   If this block isn't used, please comment it out.")
                         sys.exit()
                     if nat2_min=="NONE":
-                        print(" ERROR(eq.fix_Natoms):: missed numCell_start for "+e2)
-                        print("   If this block isn't used, please comment out.")
+                        print(" ERROR(eq.fix_Natoms):: missing numCell_start for "+e2)
+                        print("   If this block isn't used, please comment it out.")
                         sys.exit()
                     if nat2_max=="NONE":
                         nat2_max=nat2_min
                     if nat2_log:
                         self.Natoms_list.append(np.logspace(np.log10(nat2_min),np.log10(nat2_max),nat2_num))
                     else:
                         self.Natoms_list.append(np.linspace(nat2_min,nat2_max,nat2_num))
                 self.elements_fix_Natoms.append(e2)
                 self.Natoms_chempot_init.append(cpinit2)
         if len(self.elements_fix_Natoms)!=0:
             for ie1,e1 in enumerate(self.elements_fix_Natoms):
-                str1=f"   fix_Natoms({e1}): "
+                str1=f"   fix_Natoms ({e1}): "
                 len1=len(str1)
                 for n1 in self.Natoms_list[ie1]:
                     if len(str1)>90:
                         print(str1)
                         fout1.write(str1+"\n")
                         str1=len1*" "
                     str1+=f"{n1:8.3e}, "
@@ -149,28 +150,28 @@
             if "potV_end" in params1:
                 pot2_end=float(params1["potV_end"])
             if "potV_num" in params1:
                 pot2_num=params1["potV_num"]
             #if "charges" in params1:
             #    self.espots_charges=params1["charges"]
             if pot2_start=="NONE":
-                print("   ERROR(eq.eqpots):: missed potV_start")
-                print("     If this function isn't used, please comment out.")
+                print("   ERROR(eq.eqpots):: missing potV_start")
+                print("     If this function isn't used, please comment it out.")
                 sys.exit()
             if pot2_end=="NONE":
                 pot2_end=pot2_start
-                print("   WARNING(eq.espots):: potV_num is forced to 1.")
-                fout1.write("   WARNING(eq.espots):: potV_num is forced to 1.\n")
+                print("   WARNING(eq.espots):: potV_num forced to 1.")
+                fout1.write("   WARNING(eq.espots):: potV_num forced to 1.\n")
                 pot2_num=1
             if pot2_num==0:
-                print("   ERROR(eq.espots):: missed potV_num")
-                print("     If this function isn't used, please comment out.")
+                print("   ERROR(eq.espots):: missing potV_num")
+                print("     If this function isn't used, please comment it out.")
                 sys.exit()
             #if len(self.espots_charges)==0:
-            #    print("   ERROR(eq.espots):: missed espots.charges")
+            #    print("   ERROR(eq.espots):: missing espots.charges")
             #    print("     Please give (effective) charge values of ions and electrons.")
             #    print("     If this function isn't used, please comment out.")
             #    sys.exit()
             self.espots_list=np.linspace(pot2_start,pot2_end,pot2_num)
         if len(self.espots_list)!=0:
             str1=f"   espots: "
             len1=len(str1)
@@ -212,55 +213,55 @@
                 str1+=f"{e1}, "
             print(str1[:-2])
             print("-"*50)
             fout1.write(str1[:-2]+"\n")
             fout1.write("-"*50+"\n")
             refPhase=ReferencePhases(self.elements_fix_chempots,input_paths,fout1)
             if not "eq_phases" in params1:
-                print(" ERROR(eq.fix_chempots.eq_phases):: missed")
+                print(" ERROR(eq.fix_chempots.eq_phases):: missing")
                 sys.exit()
             ### reading eq_phases
             phases_whole_range=[]
             phases_limits={}
             for params2 in params1["eq_phases"]:
                 if not "label" in params2:
-                    print(" ERROR(eq.fix_chempots.eq_phases):: missed label")
+                    print(" ERROR(eq.fix_chempots.eq_phases):: missing label")
                     sys.exit()
                 l1=params2["label"]
                 if not "phases" in params2:
-                    print(" ERROR(eq.fix_chempots.eq_phases):: missed phases")
+                    print(" ERROR(eq.fix_chempots.eq_phases):: missing phases")
                     sys.exit()
                 if l1=="whole-range":
                     phases_whole_range=params2["phases"]
                 else:
                     phases_limits[l1]=params2["phases"]
             if len(phases_limits)==0:
                 phases_limits["whole"]=phases_whole_range
             else:
                 for l1,ph_list in phases_limits.items():
                     ph_list.extend(phases_whole_range)
             if len(phases_limits)==1:
                 for l1,ph_list in phases_limits.items():
                     phases_limits={"whole":ph_list}
             for l1,ph_list in phases_limits.items():
-                str1=f"   Eq-phases ({l1}): "
+                str1=f"   Equil. phases ({l1}): "
                 len1=len(str1)
                 for ph1 in ph_list:
                     if len(str1)>90:
                         print(str1)
                         fout1.write(str1+"\n")
                         str1=" "*len1
                     str1+=f"{ph1}, "
                     if not refPhase.exists(ph1):
-                        print(f" ERROR(eq.fix_chempots):: phase not found: {ph1}")
+                        print(f" ERROR(eq.fix_chempots):: Phase not found: {ph1}")
                         sys.exit()
                 print(str1[:-2])
                 fout1.write(str1[:-2]+"\n")
                 if len(ph_list)!=len(self.elements_fix_chempots):
-                    print(f" ERROR(eq.fix_chempots):: #eq_phases({l1}) is not equal to #elements(fix_chempots)")
+                    print(f" ERROR(eq.fix_chempots):: # of eq_phases ({l1}) is not equal to # of elements (fix_chempots)")
                     sys.exit()
             #### Constructing lambda-list
             lambda_list=[]
             if len(phases_limits)==1:
                 lambda_list=[{"whole":1.0}]
             elif len(phases_limits)>1:
                 lambda_prodlist=[[t1] for t1 in np.arange(0.0,1.0+1.0e-10,lambda_del)]
@@ -313,23 +314,23 @@
                 return phlist_out
 
             ### reading gas_pressures
             gas_pressures={}
             if "gas_pressures" in params1:
                 for params2 in params1["gas_pressures"]:
                     if not "label" in params2:
-                        print(" ERROR(eq.fix_chempots.gas_pressures):: missed label")
+                        print(" ERROR(eq.fix_chempots.gas_pressures):: missing label")
                         sys.exit()
                     if "pressPa_min" in params2:
-                        print(" Error:: pressPa_min(max) were changed to pressPa_start(end)")
-                        print("         Other parameters to set a parameter range were also.")
-                        print(" Very sorry for this forced chage!")
+                        print(" Error:: pressPa_min(max) was changed to pressPa_start(end)")
+                        print("         Other parameter ranges were also altered.")
+                        print(" Very sorry for this forced change!")
                         sys.exit()
                     if not "pressPa_start" in params2:
-                        print(" ERROR(eq.fix_chempots.gas_pressures):: missed pressPa_start")
+                        print(" ERROR(eq.fix_chempots.gas_pressures):: missing pressPa_start")
                         sys.exit()
                     if "scale_log" in params2:
                         scale_log=params2["scale_log"]
                     else:
                         scale_log=True
                     l1=params2["label"]
                     pmin=params2["pressPa_start"]
@@ -351,15 +352,15 @@
                                 bool_label=True
                     if bool_label:
                         if scale_log:
                             gas_pressures[l1]=np.logspace(np.log10(pmin),np.log10(pmax),pnum)
                         else:
                             gas_pressures[l1]=np.linspace(pmin,pmax,pnum)
             for l1,p1_list in gas_pressures.items():
-                str1=f"   Pressures({l1}): "
+                str1=f"   Pressures ({l1}): "
                 len_head1=len(str1)
                 for p1 in p1_list:
                     if len(str1)>90:
                         print(str1)
                         fout1.write(str1+"\n")
                         str1=len_head1*" "
                     str1+=f"{p1:8.2e}, "
@@ -416,15 +417,15 @@
                 Natoms_target_prod_list=[[t1] for t1 in self.Natoms_list[0]]
             else:
                 if self.Natoms_linking:
                     len1=len(self.Natoms_list[0])
                     for i1 in range(1,len(self.Natoms_list)):
                         len2=len(self.Natoms_list[i1])
                         if len1!=len2:
-                            print(" ERROR(eq.fix_Natoms_params):: linking_multiple-param is set in the input toml-file, but the length of input Natoms values in [[fix_Natoms]] are not coincident!")
+                            print(" ERROR(eq.fix_Natoms_params):: linking_multiple-param is set in the input toml file, but the lengths of input Natoms values in [[fix_Natoms]] are different!")
                             sys.exit()
                     for i1 in range(len1):
                         tmp_target=[]
                         for ie1 in range(len(self.Natoms_list)):
                             tmp_target.append(self.Natoms_list[ie1][i1])
                         Natoms_target_prod_list.append(tmp_target)
                 else:
@@ -492,8 +493,7 @@
         return cond_out
 
     def get_eq_conditions(self):
         return self.eq_conditions
 
     def get_elements(self):
         return self.elements_fix_chempots+self.elements_fix_Natoms
-
```

### Comparing `pydecs-2024.4.6/pydecs/host.py` & `pydecs-2024.5.12/pydecs/host.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 #!/usr/bin/env python
 #---------------------------------------------------------------------------
 # Copyright 2021 Takafumi Ogawa
 # Licensed under the Apache License, Version2.0.
 #---------------------------------------------------------------------------
 # pydecs-host module
 #---------------------------------------------------------------------------
-import os,sys
+import os
+import sys
 import copy
 import numpy as np
 from scipy.special import expit
 
 class Host:
     
     def __init__(self,input_host,input_paths=["./"],root_outfiles=None):
         fout_lm=open(root_outfiles+"_loading_messages.txt","a")
-        print(" Reading host-information")
-        fout_lm.write(" Reading host-information\n")
-        print(" Lattice-sites")
-        fout_lm.write(" Lattice-sites\n")
+        print(" Reading host information")
+        fout_lm.write(" Reading host information\n")
+        print(" Lattice sites")
+        fout_lm.write(" Lattice sites\n")
         self.lattice_sites={}
         for t1 in input_host["site"]:
             k1=t1.pop("label")
             #for t2 in k1:
             #    if t2.isdigit():
             #        print(f"  ERROR::Site-labels cannot include numeric: {k1}")
             #        print(f"     Please change to only-alphabet label like intA")
@@ -35,30 +36,33 @@
             self.lattice_sites[k1]["num_in_defective_cell"]=self.lattice_sites[k1]["num_in_cell"]
         fndos="NONE"
         for path1 in input_paths:
             fn1=path1+"inpydecs_dos.csv"
             if os.path.exists(fn1):
                 fndos=fn1
         if fndos=="NONE":
-            print(" ERROR:: not-found inpydecs_dos.csv")
+            print(" ERROR:: not found inpydecs_dos.csv")
             sys.exit()
         allowEVBM0=False
         if "allowEVBM0" in input_host:
             allowEVBM0=input_host["allowEVBM0"]
-
+        Escissor=0.0
+        if "Escissor" in input_host:
+            Escissor=input_host["Escissor"]
+        
         self.elements_host=[]
         for k1,s1 in self.lattice_sites.items():
             e1=s1["occ_atom"]
             if e1.upper()=="NONE":
                 continue
             if not e1 in self.elements_host:
                 self.elements_host.append(e1)
 
-        print(" DOS-filename: "+fndos)
-        fout_lm.write(" DOS-filename: "+fndos+"\n")
+        print(" DOS filename: "+fndos)
+        fout_lm.write(" DOS filename: "+fndos+"\n")
         fin = open(fndos)
         l1=fin.readline()
         self.dosList=[]
         self.eneList=[]
         while l1:
             l2=l1.strip()
             if len(l2)==0:
@@ -73,34 +77,44 @@
                     self.Volume=float(l2.split("=")[1].split()[0])
             else:
                 l2=l2.split(",")
                 self.eneList.append(float(l2[0])-self.EVBM)
                 self.dosList.append(float(l2[1]))
             l1=fin.readline()
         self.ene_delta=self.eneList[1]-self.eneList[0]
+        for i1 in range(len(self.eneList)):
+            e1=self.eneList[i1]
+            if e1>self.ene_delta:
+                self.eneList[i1]+=Escissor
+        self.Egap+=Escissor
+        #for i1 in range(len(self.eneList)):
+        #    print(str(self.eneList[i1]),str(self.dosList[i1]))
+
         print(f"   Volume = {self.Volume:<11.6f}")
         fout_lm.write(f"   Volume = {self.Volume:<11.6f}\n")
-        print(f"   Egap   = {self.Egap:<11.6f}")
-        fout_lm.write(f"   Egap   = {self.Egap:<11.6f}\n")
         print(f"   EVBM   = {self.EVBM:<11.6f}")
         fout_lm.write(f"   EVBM   = {self.EVBM:<11.6f}\n")
+        print(f"   Egap   = {self.Egap:<11.6f}")
+        fout_lm.write(f"   Egap   = {self.Egap:<11.6f}\n")
+        print(f"   Escissor   = {Escissor:<11.6f}")
+        fout_lm.write(f"   Escissor   = {Escissor:<11.6f}\n")
         print(f"   NEDOS  = {len(self.dosList)}")
         fout_lm.write(f"   NEDOS  = {len(self.dosList)}\n")
         if np.fabs(self.EVBM)<1e-15:
             if allowEVBM0:
                 print("   WARNING(dos):: EVBM is zero, where energies may be shifted by the original EVBM value.")
                 print("      DOS data for pydecs should be raw values.")
-                print("      This setting is allowed by '   allowEVBM0 = true' in the input toml-file (inpydecs.toml).")
+                print("      This setting is allowed by '   allowEVBM0 = true' in the input toml file (inpydecs.toml).")
                 fout_lm.write("   WARNING(dos):: EVBM is zero, where energies may be shifted by the original EVBM value.\n")
                 fout_lm.write("      DOS data for pydecs should be raw values.\n")
-                fout_lm.write("      This setting is allowed by '   allowEVBM0 = true' in the input toml-file (inpydecs.toml).\n")
+                fout_lm.write("      This setting is allowed by '   allowEVBM0 = true' in the input toml file (inpydecs.toml).\n")
             else:
                 print("   ERROR(dos):: EVBM is zero, where energies may be shifted by the original EVBM value.")
                 print("      DOS data for pydecs should be raw values.")
-                print("      If this setting should be allowed, set '   allowEVBM0 = true' in the input toml-file (inpydecs.toml).")
+                print("      If this setting should be allowed, set '   allowEVBM0 = true' in the input toml file (inpydecs.toml).")
                 sys.exit()
         print(f"-"*100)
         fout_lm.write(f"-"*100+"\n")
         fout_lm.close()
         self.espot=0.0
 
     def calc_electronic_carrier_densities(self,temperature_in,eFermi_in):
```

### Comparing `pydecs-2024.4.6/pydecs/inout.py` & `pydecs-2024.5.12/pydecs/inout.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 #!/usr/bin/env python
 #---------------------------------------------------------------------------
 # Copyright 2021 Takafumi Ogawa
 # Licensed under the Apache License, Version2.0.
 #---------------------------------------------------------------------------
 # pydecs-io module
 #---------------------------------------------------------------------------
-import os,sys
+import os
+import sys
 import shutil
 import copy
 import math
 import numpy as np
 import matplotlib.pyplot as plt
 from matplotlib import ticker
 import toml
@@ -127,48 +128,48 @@
         label_charge_int=int(label_charge)
         ##### Space-filling commands: \! = -3/18em, \; = +5/18em,  \: = +4/18em, \, =+3/18 em
         if legend_KV_in:
             label_charge="?"
             if label_charge_int==0:
                 label_charge=r"\times"
             elif label_charge_int<0:
-                label_charge="\;\!"
+                label_charge=r"\;\!"
                 for i1 in range(abs(label_charge_int)):
                     label_charge+=r"\prime"
             else:
                 label_charge=r"\!\!\;\bullet"
                 for i1 in range(abs(label_charge_int)-1):
                     label_charge+=r"\!\!\!\!\bullet"
         else:
             if label_charge_int==-1:
                 label_charge="-"
             elif label_charge_int==1:
                 label_charge="+"
             elif label_charge_int>1:
                 label_charge=label_charge+"\!\!+"
             elif label_charge_int<-1:
-                label_charge=label_charge[1:]+"\!\!-"
+                label_charge=label_charge[1:]+r"\!\!-"
         label_id=label_def1[label_def1.find("(")+1:label_def1.find(")")]
-        label_legend="\mathrm{"+label_def4+"^{"+label_charge+"}}"
+        label_legend=r"\mathrm{"+label_def4+"^{"+label_charge+"}}"
         label_legend_noQ=label_legend[:label_legend.find("^")]+"}"
         if duplication_in:
             label_legend=label_legend+"("+label_id+")"
             label_legend_noQ=label_legend_noQ+"("+label_id+")"
         label_legend="$"+label_legend+"$"
         label_legend_noQ="$"+label_legend_noQ+"$"
     return label_legend,label_legend_noQ
 
 
 class InputParamsToml:
 
     def __init__(self,filename_in="inpydecs.toml"):
         if not os.path.exists(filename_in):
-            print(" ERROR: file not-found: "+filename_in)
+            print(" ERROR: File not found: "+filename_in)
             sys.exit()
-        print(" Reading input-file: "+filename_in)
+        print(" Reading input file: "+filename_in)
         try:
             self.input_parameters=toml.load(filename_in)
         except Exception as e:
             print(" ERROR: Check TOML-format in the input file")
             print("  => "+str(e))
             sys.exit()
         self.input_paths=["./"]
@@ -243,15 +244,15 @@
     if not "Edef_ylabel" in plot_params_in.keys():
         plot_params_in["Edef_ylabel"]=r"$\mathrm{Defect\ formation\ energy\ [eV]}$"
     if not "Edef_zero_line" in plot_params_in.keys():
         plot_params_in["Edef_zero_line"]=True
     if not "Edef_bands_fill" in plot_params_in.keys():
         plot_params_in["Edef_bands_fill"]=True
     if not os.path.exists(filename_in):
-        print(" ERROR: file not-found: "+filename_in)
+        print(" ERROR: file not found: "+filename_in)
         sys.exit()
     fin=open(filename_in).readlines()
     for l1 in fin:
         if "Fermi_level" in l1:
             labels=l1.split(",")
             num_data=len(labels)
         if l1.strip()[0]!="#":
@@ -524,24 +525,32 @@
             str1+=f"{k2}, "
         elif k1=="T":
             str1+=f"temperature, "
         elif k1=="fix_Natoms":
             for v2 in v1:
                 k2=f"fix_Natoms_{v2['element']}"
                 str1+=f"{k2}, "
+        elif k1=="fix_Natoms_linked":
+            for v2 in v1:
+                k2=f"fix_Natoms_linked_{v2['element']}"
+                str1+=f"{k2}, "
         else:
             str1+=f"{k1}, "
     fout1.write(str1[:-2]+"\n")
     for ieq1,eqc1 in enumerate(eqcond_list_in):
         str1=f"{ieq1+1:04}, "
         for k1,v1 in eqc1.items():
             if k1=="fix_Natoms":
                 for v2 in v1:
                     v3=f"{v2['target_Natoms']}"
                     str1+=f"{v3}, "
+            elif k1=="fix_Natoms_linked":
+                for v2 in v1:
+                    v3=f"{v2['target_Natoms']}"
+                    str1+=f"{v3}, "
             else:
                 str1+=f"{v1}, "
         fout1.write(str1[:-2]+"\n")
     fout1.close()
 
 def output_density_with_eqcond(dens_in,eqcond_in,out_filename):
     add_list=[]
@@ -586,16 +595,16 @@
     fout1.write(" Starting plot_defect_densities\n")
     ####################
     if "input_filename" in plot_params_in.keys():
         filename_in=plot_params_in["input_filename"]
     else:
         filename_in="out_densities.csv"
     if not os.path.exists(filename_in):
-        print(f" ERROR(plot_defect_densities):: density-file not found: {filename_in}")
-        fout1.write(f" ERROR(plot_defect_densities):: density-file not found: {filename_in}\n")
+        print(f" ERROR(plot_defect_densities):: density file not found: {filename_in}")
+        fout1.write(f" ERROR(plot_defect_densities):: density file not found: {filename_in}\n")
         sys.exit()
     if not "format" in plot_params_in.keys():
         plot_params_in["format"]=["png"]
     if not "dpi" in plot_params_in.keys():
         plot_params_in["dpi"]=100
     if not "figsize_x_cm" in plot_params_in.keys():
         plot_params_in["figsize_x_cm"]=9.0
@@ -715,16 +724,16 @@
                 datalist0[key_list0[i2]]["values"].append(float(v2.strip()))
     if plot_params_in["dens_xaxis_parameter"]!="NONE":
         if not plot_params_in["dens_xaxis_parameter"] in key_list0:
             print(f" ERROR(plot)::"+plot_params_in["dens_xaxis_parameter"]+" is not found." )
             fout1.write(f" ERROR(plot)::"+plot_params_in["dens_xaxis_parameter"]+" is not found.\n" )
             sys.exit()
     ####################
-    print("  Reading eq-conditions")
-    fout1.write("  Reading eq-conditions\n")
+    print("  Reading equilibrium conditions")
+    fout1.write("  Reading equilibrium conditions\n")
     parameters_list1={}
     parameters_list2={}
     datalist1={}
     for k1,d1 in datalist0.items():
         if "fix_Natoms_" in k1:
             d2=np.array(d1["values"])/plot_params_in["dens_scale"]
         else:
@@ -803,38 +812,56 @@
         if plot_params_in["dens_xaxis_parameter"].find("pressure_")==0:
             plot_params_in["dens_xaxis_log"]=True
         else:
             plot_params_in["dens_xaxis_log"]=False
 
     parameters_list_main=[]
     parameters_list_exclmain={}
-    bool_rmlambda=False
-    bool_rmchempot=False
-    bool_rmpressure=True
-    if plot_params_in["dens_xaxis_parameter"].find("lambda_")==0:
-        bool_rmlambda=True
-        bool_rmchempot=True
-    if plot_params_in["dens_xaxis_parameter"].find("chempot_")==0:
-        bool_rmlambda=True
-        bool_rmchempot=True
-        bool_rmpressure=True
+    lambda_including=[]
+    fix_Natoms_linked_including=[]
+    for k1,v1 in parameters_list2.items():
+        if k1.find("lambda_")==0:
+            lambda_including.append(k1)
+        if k1.find("fix_Natoms_linked_")==0:
+            fix_Natoms_linked_including.append(k1)
+    cnt_lambda = len(lambda_including)-1
+    bool_fix_Natoms_linked = False
+    if len(fix_Natoms_linked_including) > 1:
+        bool_fix_Natoms_linked = True
     for k1,v1 in parameters_list2.items():
         if k1==plot_params_in["dens_xaxis_parameter"]:
             parameters_list_main=v1
         else:
-            if bool_rmlambda and k1.find("lambda_")==0:
-                if plot_params_in["dens_xaxis_parameter"].find("lambda_")==0:
-                    bool_rmlambda=False
-            elif bool_rmchempot and k1.find("chempot_")==0:
-                if plot_params_in["dens_xaxis_parameter"].find("chempot_")==0:
-                    bool_rmchempot=False
-            elif bool_rmpressure and k1.find("pressure_")==0:
-                a1=1
+            if plot_params_in["dens_xaxis_parameter"].find("chempot_")==0:
+                if k1.find("pressure_")==0 or k1.find("fix_Natoms_")==0 \
+                        or k1.find("lambda_")==0:
+                    continue
+                if k1.find("chempot_")==0 and len(lambda_including)==1:
+                    continue
+                if k1.find("chempot_")==0 and cnt_lambda>0:
+                    cnt_lambda-=1
+                    continue
             else:
-                parameters_list_exclmain[k1]=v1
+                if k1.find("chempot_")==0:
+                    continue
+                if k1.find("lambda_")==0 and cnt_lambda>0:
+                    cnt_lambda-=1
+                    continue
+                if k1.find("fix_Natoms_linked_")==0:
+                    if plot_params_in["dens_xaxis_parameter"].find("fix_Natoms_linked_")==0:
+                        continue
+                    if bool_fix_Natoms_linked:
+                        bool_fix_Natoms_linked = False
+                        parameters_list_exclmain[k1]=v1
+                        continue
+                    else:
+                        continue
+            parameters_list_exclmain[k1]=v1
+    # print(parameters_list_exclmain)
+    # print(parameters_list_main)
 
     if len(parameters_list_main)<=3:
         print(f" WARNING(plot)::Num. of dens_xaxis_parameter values is very small!")
         fout1.write(f" WARNING(plot)::Num. of dens_xaxis_parameter values is very small!\n")
     if plot_params_in["dens_x_lower_limit"]=="NONE":
         plot_params_in["dens_x_lower_limit"]=min(parameters_list_main)
     if plot_params_in["dens_x_upper_limit"]=="NONE":
@@ -1396,8 +1423,7 @@
             fig2legend.savefig(root_outfiles+"_defectDensities_separated_legend."+f1,dpi=plot_params_in["dpi"],bbox_inches="tight")
         plt.close(fig1)
         plt.close(fig2legend)
         os.chdir("../")
     print("-"*100)
     fout1.write("-"*100+"\n")
     return
-
```

### Comparing `pydecs-2024.4.6/pydecs/pydecs.py` & `pydecs-2024.5.12/pydecs/pydecs.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,16 @@
 #   limitations under the License.
 #---------------------------------------------------------------------------
 # pydecs-main module
 # pydecs = PYthon code for Defect Equilibria in Crystalline Solids
 # Library-homepage = /https://gitlab.com/tkog/pydecs
 # Citation: ***
 #---------------------------------------------------------------------------
-import os,sys
+import os
+import sys
 import numpy as np
 import shutil
 import time
 # from multiprocessing  import Pool
 # import threading 
 # from concurrent import futures
 from pathos.multiprocessing import ProcessingPool
@@ -37,18 +38,18 @@
 
 def pydecs_main():
     print(f"-"*100)
     print(f" Starting pydecs (PYthon code for Defect Equilibria in Crystalline Solids)")
     fnin_toml="inpydecs.toml"
     if len(sys.argv)>1:
         fnin_toml=sys.argv[1]
-    print(f" Input toml-file = {fnin_toml}")
+    print(f" Input toml file = {fnin_toml}")
     print(f"-"*100)
     if not os.path.exists(fnin_toml):
-        print(f" ERROR:: file not-found: {fnin_toml}")
+        print(f" ERROR:: file not found: {fnin_toml}")
         print(f"-"*100)
         sys.exit()
     intoml=InputParamsToml(fnin_toml)
     inparams=intoml.get_input_parameters()
     root_outfiles=intoml.get_root_outfiles()
     dirname=f"{root_outfiles}_outdata"
     if os.path.exists(dirname):
```

### Comparing `pydecs-2024.4.6/pydecs/reference_phases.py` & `pydecs-2024.5.12/pydecs/reference_phases.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 #!/usr/bin/env python
 #-----------------------------------------------------------------------------
 # Copyright 2021 Takafumi Ogawa
 # Licensed under the Apache License, Version2.0.
 #-----------------------------------------------------------------------------
 # Auxiliary tool of pydecs library for checking equilibrium phases
 #-----------------------------------------------------------------------------
-import os,sys
+import os
+import sys
 import numpy as np
 from scipy import interpolate
 
 class ReferencePhases:
 
     def parse_composition(self,comp_in):
         comp1=[]
@@ -28,24 +29,22 @@
                     num1+=c2
                 else:
                     elem1+=c2
             if len(num1)==0:
                 num1="1"
             atomList[elem1]=int(num1)
         return atomList
-
-
     
     def check_host(self,phaseList_in):
         self.phase_host=""
         for ph1 in phaseList_in:
             if ph1["type"]=="solid*":
                 self.phase_host=ph1
         if self.phase_host=="":
-            print(" WARNING::host-tag not-found (inpydecs_phases.csv): solid*")
+            print(" WARNING:: Host tag not found (inpydecs_phases.csv): solid*")
             return False
         return True
 
 #    def get_host_composition(self):
 #        return self.phase_host["composition"]
     def get_host(self,phaseList_in):
         if self.check_host(phaseList_in):
@@ -70,24 +69,24 @@
                     ylist.append(float(l2[1]))
                 l1 = fin.readline()
             finterp=interpolate.interp1d(xlist,ylist,kind="cubic")
             ph1["delG_finterp"]=finterp
 
     def parse_phases(self,filename_phases_in="inpydecs_phases.csv",elemsList_in="host",fout_lm=None):
         if not os.path.exists(filename_phases_in):
-            print(" ERROR::file_not_found: "+filename_phases_in)
+            print(" ERROR:: File not found: "+filename_phases_in)
             sys.exit()
         print(" Reading file: "+filename_phases_in)
         fout_lm.write(" Reading file: "+filename_phases_in+"\n")
         fin=open(filename_phases_in).readlines()
         columns=[ t1.strip() for t1 in fin[0].split(",")]
         column_names=set(["commentout","type","composition","energy_0K","filename_delG"])
         for c1 in column_names:
             if not c1 in columns:
-                print(" ERROR::column_not_found: "+c1)
+                print(" ERROR:: Column not found: "+c1)
                 sys.exit()
         phaseList0=[]
         for l1 in fin[1:]:
             l2=[ t1.strip() for t1 in l1.split(",")]
             ph0={}
             for i3,l3 in enumerate(l2):
                 c3=columns[i3]
@@ -105,30 +104,30 @@
             if not "composition" in ph0.keys()\
                 or not "composition_dict" in ph0.keys()\
                 or not "energy_0K" in ph0.keys()\
                 or not "type" in ph0.keys():
                 continue
             if len(ph0["commentout"])==0 and len(ph0["composition"])>0:
                 if not ph0["type"] in ["gas","solid","solid*"]:
-                   print(" WARNING::invalid type: "+(l3))
-                   fout_lm.write(" WARNING::invalid type: "+(l3)+"\n")
-                ph0["energy_0K"]=float(ph0["energy_0K"])
+                   print(" WARNING:: Invalid type: "+(l3))
+                   fout_lm.write(" WARNING:: Invalid type: "+(l3)+"\n")
+                ph0["energy_0K"]=float_unicode(ph0["energy_0K"])
                 phaseList0.append(ph0)
         self.check_host(phaseList0)
         comp_host=self.phase_host["composition"]
         comp_host_elems=set(self.phase_host["composition_dict"].keys())
         if elemsList_in=="host":
             slected_elems=comp_host_elems
         else:
             slected_elems=set(elemsList_in)
-        print("   Host-composition: "+self.phase_host["composition"])
-        fout_lm.write("   Host-composition: "+self.phase_host["composition"]+"\n")
+        print("   Host composition: "+self.phase_host["composition"])
+        fout_lm.write("   Host composition: "+self.phase_host["composition"]+"\n")
         phaseList1=[]
-        str1_solid="   Solid-list: "
-        str1_gas="   Gas-list: "
+        str1_solid="   Solids: "
+        str1_gas="   Gases: "
         for ph1 in phaseList0:
             comp1_elems=set(ph1["composition_dict"].keys())
             elems_sum=slected_elems.union(comp1_elems)
             if len(elems_sum)<=len(slected_elems):
                 phaseList1.append(ph1)
             if ph1["type"]=="solid":
                 str1_solid+=f"{ph1['composition']}, "
@@ -156,30 +155,30 @@
     def __init__(self,elemsList_in="host",input_paths=["./"],fout_lm=None):
         fnin="NONE"
         for path1 in input_paths:
             if os.path.exists(path1+"inpydecs_phases.csv"):
                 fnin=path1+"inpydecs_phases.csv"
                 break
         if fnin=="NONE":
-            print(" ERROR::file not-found: inpydecs_phases.csv")
+            print(" ERROR:: File not found: inpydecs_phases.csv")
             sys.exit()
         if "/" in fnin:
             self.filename_root=fnin[:fnin.rfind("/")+1]
         else:
             self.filename_root=""
         self.parse_phases(fnin,elemsList_in,fout_lm)
 
     def get_phasedata(self,comp_in):
         ph_target="NONE"
         for ph1 in self.phaseList:
             if ph1["composition"]==comp_in:
                 ph_target=ph1
                 return ph_target
         if ph_target=="NONE":
-            print(" WARNING::phasedata not-found for compound: "+comp_in)
+            print(" WARNING:: No data found for phase "+comp_in)
         return ph_target
 
     def get_singleFreeEnergy(self,comp_in,temp_in,press_in):
         ph1=self.get_phasedata(comp_in)
         energy1=ph1["energy_0K"]
         if "delG_finterp" not in ph1.keys():
             self.prepare_finterp()
@@ -190,15 +189,15 @@
         return energy1
     
     def calc_atomChempots(self,temp_in,comp_press_list_in,bool_silent=False):
         if not bool_silent:
             print(" Calculating chemical potentials")
             print("   Temperature = "+str(temp_in))
             for (c1,p1) in comp_press_list_in:
-                print("   Compound = "+str(c1)+" ; Presssure = "+str(p1))
+                print("   Phase = "+str(c1)+" ; Pressure = "+str(p1))
         elems=[]
         atomnumsList=[]
         eneList=[]
         for (c1,p1) in comp_press_list_in:
             ph1=self.get_phasedata(c1)
             ene1=self.get_singleFreeEnergy(c1,temp_in,p1)
             c2=ph1["composition_dict"]
@@ -228,15 +227,15 @@
         if len(comp_press_list_in)<len(elems):
             print(" ERROR:: The above equations cannot be solved.")
             sys.exit()
         coeffsList=np.matrix(coeffsList)
         coeffsList_inv=np.linalg.inv(coeffsList)
         muList1=coeffsList_inv*np.matrix(eneList)
         if not bool_silent:
-            print(" Solved results")
+            print(" Equations solved")
         muList2={}
         for ie1,e1 in enumerate(elems):
             muList2[e1]=float(muList1[ie1][0])
         for ie1,e1 in enumerate(elems):
             str1="   mu_"+e1+" = "+str(muList2[e1])
             if not bool_silent:
                 print(str1)
@@ -251,7 +250,10 @@
         return True
 
     def issolid(self,phase_in):
         t1=self.get_phasedata(phase_in)
         if "solid" in t1["type"]:
             return True
         return False
+
+def float_unicode(arg_str):
+    return float(arg_str.replace(u"\u2212", "-"))
```

### Comparing `pydecs-2024.4.6/pydecs/solver.py` & `pydecs-2024.5.12/pydecs/solver.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 #!/usr/bin/env python
 #-----------------------------------------------------------------------------
 # Copyright 2021 Takafumi Ogawa
 # Licensed under the Apache License, Version2.0.
 #-----------------------------------------------------------------------------
 # pydecs-solver module
 #-----------------------------------------------------------------------------
-import os,sys
+import os
+import sys
 import copy
 import numpy as np
 from scipy import optimize
 from scipy import interpolate
 
 from pydecs.defects import Defects
 from pydecs.host import Host
@@ -44,15 +45,15 @@
 
     def output_defEne_wrt_eFermi(self,temperature_in,chempots_in,root_outfiles,plot_params_in):
         if not "Edef_x_lower_limit" in plot_params_in.keys():
             plot_params_in["Edef_x_lower_limit"]=0.0
         if not "Edef_x_upper_limit" in plot_params_in.keys():
             plot_params_in["Edef_x_upper_limit"]=self.host.get_Egap()
         if plot_params_in["Edef_x_upper_limit"]<plot_params_in["Edef_x_lower_limit"]:
-            print(" ERROR:: emax is less than emin, in eFermi serach.")
+            print(" ERROR:: emax is less than emin in eFermi search.")
             print("   Please check the input file")
             print("   plot.Edef_x_lower_limit and plot.Edef_x_upper_limit")
             sys.exit()
         if not "Edef_x_delta" in plot_params_in.keys():
             plot_params_in["Edef_x_delta"]=(plot_params_in["Edef_x_upper_limit"]-plot_params_in["Edef_x_lower_limit"])/100.0
         (energy_list,qtot_list,defect_energy_list)=self.calc_defEne_wrt_eFermi(temperature_in,chempots_in,
             plot_params_in["Edef_x_lower_limit"],plot_params_in["Edef_x_upper_limit"],plot_params_in["Edef_x_delta"])
@@ -269,27 +270,27 @@
         else:
             residualRMS_Nsites=opt_params_in["opt_Nsites_tol"]*2.0
             Nsites_previous=self.host.get_Nsites_perfect()
             i_loop=1
             while residualRMS_Nsites>opt_params_in["opt_Nsites_tol"] and i_loop<opt_params_in["opt_Nsites_maxloop"]:
                 (res_eF,res_qtot)=self.opt_eFermi_for_chempots(temperature_in,chempots_in,opt_params_in,root_outfiles)
                 if self.defects.check_minus_defect_energy():
-                    print(" ERROR(opt_Nsites):: Densities cannot be obtained for minus defect formation energies.")
-                    print("    You can check the case by using 'just_plot_Edef = True' in the input file (inpydecs.toml).")
+                    print(" ERROR(opt_Nsites):: Densities cannot be obtained for negative defect formation energies.")
+                    print("    You can check these by setting 'just_plot_Edef = True' in the input file (inpydecs.toml).")
                     # print("   Check output-files: *_Edef_eFermi.*  ")
                     return None
                 self.update_Nsites_defective()
                 Nsites_new=self.host.get_Nsites_defective()
                 residuals_Nsites=self.calc_residual_Nsites(Nsites_previous,Nsites_new)
                 residualRMS_Nsites=residuals_Nsites["RMS"]
                 outdata_local(self.outstr_Nsites(res_eF,res_qtot,residuals_Nsites))
                 Nsites_previous=copy.deepcopy(Nsites_new)
                 i_loop+=1
             if i_loop==opt_params_in["opt_Nsites_maxloop"]:
-                print(" WARNING(opt_Nsites):: Nsites_loop reaches maxloop:"+str(i_loop))
+                print(" WARNING(opt_Nsites):: Nsites_loop reached maxloop:"+str(i_loop))
         data_defect_densities=self.produce_outheader_density(temperature_in,chempots_in,res_eF,res_qtot,self.host.get_Egap(),self.host.get_Volume())
         # fnout_csv=root_outfiles+"_defect_densities.csv"
         # self.output_density_data(data_defect_densities,fnout_csv)
         if opt_params_in["opt_Nsites_output_Edef_atlast"]:
             self.output_defEne_wrt_eFermi(temperature_in,chempots_in,root_outfiles,plot_params_in)
             self.calc_defEne_single(temperature_in,chempots_in,res_eF)
         self.id_loop_Nsites+=1
@@ -361,15 +362,15 @@
             outdata.append("energy_"+self.defects.get_label(dt1))
             outdata.append(self.defects.get_defect_energy(dt1))
             outdata_all.append(outdata)
         return outdata_all
 
 
     def opt_steady_line_minimization(self,func_resid,vect_grad,cp0,step_size,fout=None,tol_in=1e-7,maxiter=1000):
-        fout.write(f" ------ Starting step-wize minimization with step size of {step_size} -----\n")
+        fout.write(f" ------ Starting stepwise minimization with step size of {step_size} -----\n")
         residArray0=func_resid(cp0)
         if residArray0 is None:
             return (None,None)
         # resid0=np.max(np.fabs(residArray0))
         # resid0=np.sqrt(np.square(residArray0).mean(axis=0))
         resid0=np.linalg.norm(residArray0)
         cp1=[]
@@ -390,15 +391,15 @@
                 for i1,v1 in enumerate(vect_grad):
                     cp2.append(cp1[i1]+step_size*v1)
                 cp0=cp1
                 residArray0=residArray1
                 resid0=resid1
                 cp1=cp2
             i_loop+=1
-        print("finished: step-wize minimization")
+        print("finished: stepwise minimization")
         fout.write(" ------ Starting golden minimization -----\n")
         print(" [opt_Natoms] Starting minimization")
         def func_resid_local(x_in):
             cp2=[]
             for i1 in range(len(cp0)):
                 cp2.append(x_in*cp0[i1]+(1.0-x_in)*cp1[i1])
             residArray2=func_resid(cp2)
@@ -568,15 +569,15 @@
             str1+=f" {resid_new:18.11e} |"
             if bool_output_std:
                 print(" [Natoms] "+str_outlabel)
                 print(" [Natoms] "+str1)
                 print("-"*100)
             if bool_output_file:
                 fout1.write(str1+"\n")
-        print(" [opt_Natoms] Starating")
+        print(" [opt_Natoms] Starting")
         def func_resid_fixNatoms(cp_in):
             cp1=copy.deepcopy(chempots_in)
             for icp1,cp_in1 in enumerate(cp_in):
                 cp1[Natoms_elem_list[icp1]]=cp_in1
             out_defect_densities=self.opt_Nsites_for_chempots(temperature_in,cp1,opt_params_in,root_outfiles)
             if out_defect_densities is None:
                 return None
@@ -641,16 +642,16 @@
             self.host.set_espot(eq_cond_in["espot"])
             self.defects.set_espot(eq_cond_in["espot"])
         if not "just_plot_Edef" in solver_params_in:
             solver_params_in["just_plot_Edef"]=False
         if solver_params_in["just_plot_Edef"]:
             print(" [solver] Just plotting Edef")
             if "fix_Natoms" in eq_cond_in.keys():
-                print("   WARNING: fix_Natoms is detected.")
-                print("   chemical potentials are set to [eq.fix_Natoms.chempot_init] values.")
+                print("   WARNING: fix_Natoms detected.")
+                print("   chemical potentials set to [eq.fix_Natoms.chempot_init] values.")
                 for fix1 in eq_cond_in["fix_Natoms"]:
                     chempots[fix1["element"]]=fix1["chempot_init"]
             self.output_defEne_wrt_eFermi(temp,chempots,root_outfiles,plot_params_in)
             return None
 
         bool_fixNatoms=False
         self.eqlabel_fixNatoms="NONE"
@@ -676,8 +677,7 @@
                     for d1 in defect_densities:
                         if d1[-2]=="chempot_"+e1:
                             self.chempots_fixNatoms[e1]=float(d1[-1])
         else:
             defect_densities=self.opt_Nsites_for_chempots(temp,chempots,solver_params_in,root_outfiles,plot_params_in)
         
         return defect_densities
-
```

### Comparing `pydecs-2024.4.6/pydecs.egg-info/PKG-INFO` & `pydecs-2024.5.12/pydecs.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydecs
-Version: 2024.4.6
+Version: 2024.5.12
 Summary: This tool enables us to analyze equilibrium concentrations of point and complex defects in crystalline solids
 Home-page: https://gitlab.com/tkog/pydecs
 Author: Takafumi Ogawa
 Author-email: takafumi.ogawa.1+pydecs@gmail.com
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Topic :: Scientific/Engineering :: Physics
```

### Comparing `pydecs-2024.4.6/pydecs.egg-info/SOURCES.txt` & `pydecs-2024.5.12/pydecs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pydecs-2024.4.6/setup.cfg` & `pydecs-2024.5.12/setup.cfg`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pydecs
-version = 2024.04.06
+version = 2024.05.12
 description = This tool enables us to analyze equilibrium concentrations of point and complex defects in crystalline solids
 author = Takafumi Ogawa
 author_email = takafumi.ogawa.1+pydecs@gmail.com
 url = https://gitlab.com/tkog/pydecs
 lisense_file = LICENSE.txt
 classifiers = 
 	Intended Audience :: Science/Research
```

