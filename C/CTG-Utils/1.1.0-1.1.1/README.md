# Comparing `tmp/CTG_Utils-1.1.0.tar.gz` & `tmp/CTG_Utils-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CTG_Utils-1.1.0.tar", last modified: Sat May 11 06:52:48 2024, max compression
+gzip compressed data, was "CTG_Utils-1.1.1.tar", last modified: Sun May 12 12:47:52 2024, max compression
```

## Comparing `CTG_Utils-1.1.0.tar` & `CTG_Utils-1.1.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxrwx   0        0        0        0 2024-05-11 06:52:48.081676 CTG_Utils-1.1.0/
-drwxrwxrwx   0        0        0        0 2024-05-11 06:52:48.026275 CTG_Utils-1.1.0/CTG_Utils/
-drwxrwxrwx   0        0        0        0 2024-05-11 06:52:48.045225 CTG_Utils-1.1.0/CTG_Utils/CTG_Func/
--rw-rw-rw-   0        0        0     6571 2024-05-10 17:41:23.000000 CTG_Utils-1.1.0/CTG_Utils/CTG_Func/CTGClasses.py
-drwxrwxrwx   0        0        0        0 2024-05-11 06:52:48.055200 CTG_Utils-1.1.0/CTG_Utils/CTG_Func/CTG_RefFiles/
--rw-rw-rw-   0        0        0       41 2024-04-03 06:31:10.000000 CTG_Utils-1.1.0/CTG_Utils/CTG_Func/CTG_RefFiles/CTG.yaml
--rw-rw-rw-   0        0        0      605 2023-09-01 12:09:43.000000 CTG_Utils-1.1.0/CTG_Utils/CTG_Func/CTG_RefFiles/CTG_correction.yaml
--rw-rw-rw-   0        0        0   228969 2024-05-05 16:57:27.000000 CTG_Utils-1.1.0/CTG_Utils/CTG_Func/CTG_RefFiles/logo_ffvelo.ico
--rw-rw-rw-   0        0        0    34827 2024-05-05 14:03:57.000000 CTG_Utils-1.1.0/CTG_Utils/CTG_Func/CTG_RefFiles/logo_ffvelo.png
--rw-rw-rw-   0        0        0    26973 2024-05-06 17:53:49.000000 CTG_Utils-1.1.0/CTG_Utils/CTG_Func/CTG_RefFiles/logoctg4.PNG
--rw-rw-rw-   0        0        0   100526 2024-05-06 17:57:15.000000 CTG_Utils-1.1.0/CTG_Utils/CTG_Func/CTG_RefFiles/logoctg4.ico
--rw-rw-rw-   0        0        0     1576 2024-05-10 18:06:52.000000 CTG_Utils-1.1.0/CTG_Utils/CTG_Func/CTG_RefFiles/memory_sorties.yml
--rw-rw-rw-   0        0        0      574 2024-04-15 12:33:24.000000 CTG_Utils-1.1.0/CTG_Utils/CTG_Func/CTG_RefFiles/memory_sorties_old.yml
--rw-rw-rw-   0        0        0  9545867 2024-04-03 11:27:38.000000 CTG_Utils-1.1.0/CTG_Utils/CTG_Func/CTG_RefFiles/villes_france_premium.csv
--rw-rw-rw-   0        0        0      488 2024-05-09 07:18:30.000000 CTG_Utils-1.1.0/CTG_Utils/CTG_Func/CTG_config.py
--rw-rw-rw-   0        0        0    19835 2024-05-09 11:52:03.000000 CTG_Utils-1.1.0/CTG_Utils/CTG_Func/CTG_effectif.py
--rw-rw-rw-   0        0        0    11586 2024-05-10 13:31:57.000000 CTG_Utils-1.1.0/CTG_Utils/CTG_Func/CTG_plot.py
--rw-rw-rw-   0        0        0    15509 2024-05-10 17:36:41.000000 CTG_Utils-1.1.0/CTG_Utils/CTG_Func/CTG_synthese.py
--rw-rw-rw-   0        0        0     4645 2024-05-10 17:35:42.000000 CTG_Utils-1.1.0/CTG_Utils/CTG_Func/CTG_utility.py
--rw-rw-rw-   0        0        0      218 2024-05-10 17:42:50.000000 CTG_Utils-1.1.0/CTG_Utils/CTG_Func/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-11 06:52:48.079650 CTG_Utils-1.1.0/CTG_Utils/CTG_GUI/
--rw-rw-rw-   0        0        0    15700 2024-05-10 12:50:50.000000 CTG_Utils-1.1.0/CTG_Utils/CTG_GUI/GUI_Globals.py
--rw-rw-rw-   0        0        0    10886 2024-05-10 12:46:38.000000 CTG_Utils-1.1.0/CTG_Utils/CTG_GUI/PageDivers.py
--rw-rw-rw-   0        0        0    11530 2024-05-07 13:39:45.000000 CTG_Utils-1.1.0/CTG_Utils/CTG_GUI/PageEffectif.py
--rw-rw-rw-   0        0        0    11613 2024-05-07 11:49:29.000000 CTG_Utils-1.1.0/CTG_Utils/CTG_GUI/PageSorties.py
--rw-rw-rw-   0        0        0    10763 2024-05-09 13:49:41.000000 CTG_Utils-1.1.0/CTG_Utils/CTG_GUI/PageSynthese.py
--rw-rw-rw-   0        0        0     9011 2024-05-08 07:41:08.000000 CTG_Utils-1.1.0/CTG_Utils/CTG_GUI/PageTendance.py
--rw-rw-rw-   0        0        0    30344 2024-05-10 07:03:45.000000 CTG_Utils-1.1.0/CTG_Utils/CTG_GUI/Page_Classes.py
--rw-rw-rw-   0        0        0    13687 2024-04-26 08:07:42.000000 CTG_Utils-1.1.0/CTG_Utils/CTG_GUI/Useful_Classes.py
--rw-rw-rw-   0        0        0    11470 2024-05-10 06:56:47.000000 CTG_Utils-1.1.0/CTG_Utils/CTG_GUI/Useful_Functions.py
--rw-rw-rw-   0        0        0      198 2024-05-10 17:28:54.000000 CTG_Utils-1.1.0/CTG_Utils/CTG_GUI/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-11 06:52:48.038245 CTG_Utils-1.1.0/CTG_Utils.egg-info/
--rw-rw-rw-   0        0        0      681 2024-05-11 06:52:47.000000 CTG_Utils-1.1.0/CTG_Utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1215 2024-05-11 06:52:47.000000 CTG_Utils-1.1.0/CTG_Utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-11 06:52:47.000000 CTG_Utils-1.1.0/CTG_Utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       80 2024-05-11 06:52:47.000000 CTG_Utils-1.1.0/CTG_Utils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       37 2024-05-11 06:52:47.000000 CTG_Utils-1.1.0/CTG_Utils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1088 2022-03-26 14:35:29.000000 CTG_Utils-1.1.0/LICENSE
--rw-rw-rw-   0        0        0       43 2024-05-08 19:17:34.000000 CTG_Utils-1.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0      681 2024-05-11 06:52:48.080648 CTG_Utils-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0       22 2022-03-19 12:02:13.000000 CTG_Utils-1.1.0/README.md
--rw-rw-rw-   0        0        0       42 2024-05-11 06:52:48.081676 CTG_Utils-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1398 2024-05-09 18:13:06.000000 CTG_Utils-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-12 12:47:52.896909 CTG_Utils-1.1.1/
+drwxrwxrwx   0        0        0        0 2024-05-12 12:47:52.846569 CTG_Utils-1.1.1/CTG_Utils/
+drwxrwxrwx   0        0        0        0 2024-05-12 12:47:52.863524 CTG_Utils-1.1.1/CTG_Utils/CTG_Func/
+-rw-rw-rw-   0        0        0     6530 2024-05-12 12:12:01.000000 CTG_Utils-1.1.1/CTG_Utils/CTG_Func/CTGClasses.py
+drwxrwxrwx   0        0        0        0 2024-05-12 12:47:52.872500 CTG_Utils-1.1.1/CTG_Utils/CTG_Func/CTG_RefFiles/
+-rw-rw-rw-   0        0        0       41 2024-04-03 06:31:10.000000 CTG_Utils-1.1.1/CTG_Utils/CTG_Func/CTG_RefFiles/CTG.yaml
+-rw-rw-rw-   0        0        0      605 2023-09-01 12:09:43.000000 CTG_Utils-1.1.1/CTG_Utils/CTG_Func/CTG_RefFiles/CTG_correction.yaml
+-rw-rw-rw-   0        0        0   228969 2024-05-05 16:57:27.000000 CTG_Utils-1.1.1/CTG_Utils/CTG_Func/CTG_RefFiles/logo_ffvelo.ico
+-rw-rw-rw-   0        0        0    34827 2024-05-05 14:03:57.000000 CTG_Utils-1.1.1/CTG_Utils/CTG_Func/CTG_RefFiles/logo_ffvelo.png
+-rw-rw-rw-   0        0        0    26973 2024-05-06 17:53:49.000000 CTG_Utils-1.1.1/CTG_Utils/CTG_Func/CTG_RefFiles/logoctg4.PNG
+-rw-rw-rw-   0        0        0   100526 2024-05-06 17:57:15.000000 CTG_Utils-1.1.1/CTG_Utils/CTG_Func/CTG_RefFiles/logoctg4.ico
+-rw-rw-rw-   0        0        0     1576 2024-05-10 18:06:52.000000 CTG_Utils-1.1.1/CTG_Utils/CTG_Func/CTG_RefFiles/memory_sorties.yml
+-rw-rw-rw-   0        0        0      574 2024-04-15 12:33:24.000000 CTG_Utils-1.1.1/CTG_Utils/CTG_Func/CTG_RefFiles/memory_sorties_old.yml
+-rw-rw-rw-   0        0        0  9545867 2024-04-03 11:27:38.000000 CTG_Utils-1.1.1/CTG_Utils/CTG_Func/CTG_RefFiles/villes_france_premium.csv
+-rw-rw-rw-   0        0        0      488 2024-05-09 07:18:30.000000 CTG_Utils-1.1.1/CTG_Utils/CTG_Func/CTG_config.py
+-rw-rw-rw-   0        0        0    19037 2024-05-12 12:31:46.000000 CTG_Utils-1.1.1/CTG_Utils/CTG_Func/CTG_effectif.py
+-rw-rw-rw-   0        0        0    11461 2024-05-12 12:33:31.000000 CTG_Utils-1.1.1/CTG_Utils/CTG_Func/CTG_plot.py
+-rw-rw-rw-   0        0        0    15563 2024-05-12 12:39:25.000000 CTG_Utils-1.1.1/CTG_Utils/CTG_Func/CTG_synthese.py
+-rw-rw-rw-   0        0        0     4645 2024-05-10 17:35:42.000000 CTG_Utils-1.1.1/CTG_Utils/CTG_Func/CTG_utility.py
+-rw-rw-rw-   0        0        0      191 2024-05-12 12:09:52.000000 CTG_Utils-1.1.1/CTG_Utils/CTG_Func/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-12 12:47:52.894970 CTG_Utils-1.1.1/CTG_Utils/CTG_GUI/
+-rw-rw-rw-   0        0        0    15700 2024-05-10 12:50:50.000000 CTG_Utils-1.1.1/CTG_Utils/CTG_GUI/GUI_Globals.py
+-rw-rw-rw-   0        0        0    10886 2024-05-10 12:46:38.000000 CTG_Utils-1.1.1/CTG_Utils/CTG_GUI/PageDivers.py
+-rw-rw-rw-   0        0        0    11530 2024-05-07 13:39:45.000000 CTG_Utils-1.1.1/CTG_Utils/CTG_GUI/PageEffectif.py
+-rw-rw-rw-   0        0        0    11622 2024-05-12 11:11:49.000000 CTG_Utils-1.1.1/CTG_Utils/CTG_GUI/PageSorties.py
+-rw-rw-rw-   0        0        0    10763 2024-05-09 13:49:41.000000 CTG_Utils-1.1.1/CTG_Utils/CTG_GUI/PageSynthese.py
+-rw-rw-rw-   0        0        0     9011 2024-05-08 07:41:08.000000 CTG_Utils-1.1.1/CTG_Utils/CTG_GUI/PageTendance.py
+-rw-rw-rw-   0        0        0    30344 2024-05-10 07:03:45.000000 CTG_Utils-1.1.1/CTG_Utils/CTG_GUI/Page_Classes.py
+-rw-rw-rw-   0        0        0    13687 2024-04-26 08:07:42.000000 CTG_Utils-1.1.1/CTG_Utils/CTG_GUI/Useful_Classes.py
+-rw-rw-rw-   0        0        0    11454 2024-05-12 12:03:55.000000 CTG_Utils-1.1.1/CTG_Utils/CTG_GUI/Useful_Functions.py
+-rw-rw-rw-   0        0        0      198 2024-05-10 17:28:54.000000 CTG_Utils-1.1.1/CTG_Utils/CTG_GUI/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-12 12:47:52.855545 CTG_Utils-1.1.1/CTG_Utils.egg-info/
+-rw-rw-rw-   0        0        0      681 2024-05-12 12:47:51.000000 CTG_Utils-1.1.1/CTG_Utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1215 2024-05-12 12:47:51.000000 CTG_Utils-1.1.1/CTG_Utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-12 12:47:51.000000 CTG_Utils-1.1.1/CTG_Utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       80 2024-05-12 12:47:51.000000 CTG_Utils-1.1.1/CTG_Utils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       37 2024-05-12 12:47:51.000000 CTG_Utils-1.1.1/CTG_Utils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1088 2022-03-26 14:35:29.000000 CTG_Utils-1.1.1/LICENSE
+-rw-rw-rw-   0        0        0       43 2024-05-08 19:17:34.000000 CTG_Utils-1.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      681 2024-05-12 12:47:52.895949 CTG_Utils-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0       22 2022-03-19 12:02:13.000000 CTG_Utils-1.1.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-12 12:47:52.896909 CTG_Utils-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1398 2024-05-12 12:45:27.000000 CTG_Utils-1.1.1/setup.py
```

### Comparing `CTG_Utils-1.1.0/CTG_Utils/CTG_Func/CTGClasses.py` & `CTG_Utils-1.1.1/CTG_Utils/CTG_Func/CTGClasses.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,14 @@
         # Standard library imports
         from pathlib import Path
 
         # Third party imports
         import pandas as pd
 
         # Internal imports
-        from CTG_Utils.CTG_Func.CTG_config import _config_ctg
         from CTG_Utils.CTG_Func.CTG_plot import built_lat_long
 
         self.year = year
         self.ctg_path = ctg_path
         df = pd.read_excel(self.ctg_path / Path(str(year))/ Path('DATA')/Path(str(year)+'.xlsx'))
         
         year_1 = int(year)-1
@@ -126,10 +125,11 @@
         fig, ax = plt.subplots(figsize=(10,10))
         self.effectif['age group'] = pd.cut(self.effectif.Age, bins=range(0, 95, 5), right=False)
         result_hist = self.effectif.groupby('Sexe')['age group'].value_counts().unstack().T.plot.bar(width=1, stacked=False,ax=ax)
         
         plt.tick_params(axis='x', labelsize=20)
         plt.tick_params(axis='y', labelsize=20)
         plt.title(self.year,fontsize=20)
+        plt.legend()
         plt.tight_layout()
         plt.show()
```

### Comparing `CTG_Utils-1.1.0/CTG_Utils/CTG_Func/CTG_RefFiles/CTG_correction.yaml` & `CTG_Utils-1.1.1/CTG_Utils/CTG_Func/CTG_RefFiles/CTG_correction.yaml`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.1.0/CTG_Utils/CTG_Func/CTG_RefFiles/logo_ffvelo.ico` & `CTG_Utils-1.1.1/CTG_Utils/CTG_Func/CTG_RefFiles/logo_ffvelo.ico`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.1.0/CTG_Utils/CTG_Func/CTG_RefFiles/logo_ffvelo.png` & `CTG_Utils-1.1.1/CTG_Utils/CTG_Func/CTG_RefFiles/logo_ffvelo.png`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.1.0/CTG_Utils/CTG_Func/CTG_RefFiles/logoctg4.PNG` & `CTG_Utils-1.1.1/CTG_Utils/CTG_Func/CTG_RefFiles/logoctg4.PNG`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.1.0/CTG_Utils/CTG_Func/CTG_RefFiles/logoctg4.ico` & `CTG_Utils-1.1.1/CTG_Utils/CTG_Func/CTG_RefFiles/logoctg4.ico`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.1.0/CTG_Utils/CTG_Func/CTG_RefFiles/memory_sorties.yml` & `CTG_Utils-1.1.1/CTG_Utils/CTG_Func/CTG_RefFiles/memory_sorties.yml`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.1.0/CTG_Utils/CTG_Func/CTG_RefFiles/memory_sorties_old.yml` & `CTG_Utils-1.1.1/CTG_Utils/CTG_Func/CTG_RefFiles/memory_sorties_old.yml`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.1.0/CTG_Utils/CTG_Func/CTG_RefFiles/villes_france_premium.csv` & `CTG_Utils-1.1.1/CTG_Utils/CTG_Func/CTG_RefFiles/villes_france_premium.csv`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.1.0/CTG_Utils/CTG_Func/CTG_effectif.py` & `CTG_Utils-1.1.1/CTG_Utils/CTG_Func/CTG_effectif.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,42 +4,36 @@
            'parse_date',
            'read_effectif',
            'read_effectif_corrected',
            'evolution_effectif',
            'builds_excel_presence_au_club',
            'statistique_vae',
            'anciennete_au_club',]
-           
-from CTG_Utils.CTG_Func.CTG_config import GLOBAL           
+                      
 
-def read_effectif_corrected(dic_correction_licence, list_non_licencie, part_club, year=None):
+def read_effectif_corrected(dic_correction_licence, list_non_licencie, part_club, ctg_path, year=None):
     
     '''Lecture du fichier effectif et correction
     '''
     # Standard library imports
     from pathlib import Path
     import datetime
    
     # 3rd party imports
     import numpy as np
     import pandas as pd
     
-    
-    
-    #file_effectif = GLOBAL['EFFECTIF'])
-    
     if year is not None:
         file_effectif = str(year) + '.xlsx'
     else:
         currentDateTime = datetime.datetime.now()
         date = currentDateTime.date()
         year = date.strftime("%Y")
         file_effectif = year + '.xlsx'
-        
-    df_effectif = pd.read_excel(GLOBAL['ROOT']/ Path(str(year))/Path('DATA')/ Path(file_effectif))
+    df_effectif = pd.read_excel(ctg_path / Path(str(year))/Path('DATA')/ Path(file_effectif))
     df_effectif = df_effectif[['N° Licencié', 'Nom','Prénom','Sexe','Pratique VAE']]
     
         
     for num_licence in dic_correction_licence.keys():
         idx = df_effectif[df_effectif["N° Licencié"]==num_licence].index
         df_effectif.loc[idx,'Prénom'] = dic_correction_licence[num_licence]['Prénom']
         df_effectif.loc[idx,'Nom'] = dic_correction_licence[num_licence]['Nom']
@@ -131,24 +125,24 @@
         else:
             dg = pd.DataFrame([[None,None,None,None,sejour,]], columns=['N° Licencié','Nom','Prénom','Sexe','sejour',])
     else:
         dg = pd.DataFrame([[None,None,None,None,sejour,]], columns=['N° Licencié','Nom','Prénom','Sexe','sejour',])
     
     return dg
 
-def correction_effectif(year):
+def correction_effectif(year,ctg_path):
     
     # Standard library import
     from pathlib import Path
     
     #3rd party import
     import yaml
     
     #path_cor_yaml = Path(__file__).parent / Path('CTG_RefFiles/CTG_correction.yaml')
-    path_cor_yaml = GLOBAL['ROOT'] / Path(str(year)) / Path('DATA') / Path('CTG_correction.yaml')
+    path_cor_yaml = ctg_path / Path(str(year)) / Path('DATA') / Path('CTG_correction.yaml')
     
     with open(path_cor_yaml, "r",encoding='utf8') as stream:
         data_list_dict = yaml.safe_load(stream)
     
     list_non_licencie  = []   
     if data_list_dict['list_non_licencie']:
         list_non_licencie = [(x.split(',')[0].strip(),x.split(',')[1].strip(),x.split(',')[2].strip())
@@ -157,31 +151,31 @@
                          for x in data_list_dict['dic_part_club']]
     dic_correction_licence = data_list_dict['dic_correction_licence']
     dic_correction_licence = {list(x.keys())[0] : list(x.values())[0] for x in dic_correction_licence}
     
     return list_non_licencie, dic_correction_licence, dic_part_club
 
     
-def count_participation(path,year,info_rando):
+def count_participation(path,ctg_path,year,info_rando):
     
     import os
     import re
     from pathlib import Path
 
     import pandas as pd
     
     flag_sejour = False
     if os.path.split(path)[-1] == 'SEJOUR' : 
         flag_sejour = True
 
     type_sortie_default = os.path.basename(path)
     type_sortie_default = type_sortie_default.split('.', 1)[0]
-    list_non_licencie, dic_correction_licence, dic_part_club = correction_effectif(year)
+    list_non_licencie, dic_correction_licence, dic_part_club = correction_effectif(year,ctg_path)
 
-    df_effectif = read_effectif_corrected(dic_correction_licence, list_non_licencie, dic_part_club,year)
+    df_effectif = read_effectif_corrected(dic_correction_licence, list_non_licencie, dic_part_club,ctg_path,year)
 
     no_match = []
     df_list = [] 
     sejours = [x for x in os.listdir( path / Path('CSV')) if x.endswith('.csv')]
     
     
     nbr_moyen_participants = 0
@@ -252,15 +246,15 @@
         pattern = re.compile(r"(?P<month>\d{1,2}_)(?P<day>\d{1,2})")
         match = pattern.search(s)
         date = convert_to_date(str(year)+'_'+match.group("month")+match.group("day"))
     
     return date
 
     
-def read_effectif(year = None):
+def read_effectif(ctg_path,year):
     
     from pathlib import Path
     
     import numpy as np
     import pandas as pd
     
     from CTG_Utils.CTG_Func.CTG_plot import built_lat_long
@@ -274,35 +268,21 @@
         rad = 6371
         dist = 2 * rad * asin(
                                 sqrt(
                                     sin((phi2 - phi1) / 2) ** 2
                                     + cos(phi1) * cos(phi2) * sin((lon2 - lon1) / 2) ** 2
                                 ))
         return np.round(dist,1)
-    
-    def certificat_medical(row):
-        if row['Certificat médical'] != 'Non':
-            return '01/01/2000'
-        else:
-            return row['Date du certificat']
 
-    if year is None:
-        df = pd.read_excel(GLOBAL['ROOT'] / Path(GLOBAL['EFFECTIF']))
-    else:
-        df = pd.read_excel(GLOBAL['ROOT'] / Path(str(year))/ Path('DATA')/Path(str(year)+'.xlsx'))
+    
+    df = pd.read_excel(ctg_path / Path(str(year))/ Path('DATA')/Path(str(year)+'.xlsx'))
         
     df['Date de naissance'] = pd.to_datetime(df['Date de naissance'], format="%d/%m/%Y")
     
-    #df['Age']  = df['Date de naissance'].apply(lambda x : (pd.Timestamp.today()-x).days/365)
-    
     df['Age']  = df['Date de naissance'].apply(lambda x : (pd.Timestamp(year, 9, 30)-x).days/365)
-    #df['Date du certificat'] = df.apply(certificat_medical,axis=1)
-    #return df
-    #df['Date du certificat'] = pd.to_datetime(df['Date du certificat'], format="%d/%m/%Y")
-    #df['Limite certificat médical']  = df['Date du certificat'].apply(lambda x : (pd.Timestamp.today()-x).days/365)
 
     df,dh = built_lat_long(df)
 
     df['distance'] = df.apply(distance_,axis=1)
     
     return df
     
@@ -331,33 +311,37 @@
         for year in years:
             if year == 2006:
                 nbr_femmes.append(41)
                 nbr_hommes.append(100)
                 nbr_total.append(141)
                 ratio_femmes.append(str(29)+'%')
             else:  
-                df_effectif = read_effectif(year)
+                df_effectif = read_effectif(ctg_path,year)
                 nh = len(df_effectif.query('Sexe =="M"'))
                 nbr_hommes.append(nh)
                 nf = len(df_effectif.query('Sexe =="F"'))
                 nbr_femmes.append(nf)
                 nbr_total.append(nh + nf)
                 ratio_femmes.append(str(int(100*nf/(nh+nf)))+'%')
         return nbr_hommes, nbr_femmes,nbr_total,ratio_femmes
     
     years = [2006] + [int(x) for x in os.listdir(ctg_path) if re.findall('^\d{4}$',x)]
     nbr_hommes, nbr_femmes,nbr_total,ratio_femmes = _evolution_effectif(years)
     
     title='Evolution du nombre de licenciés CTG'
-    title = ''
-    
     
+    ax = plt.axes() 
     plt.bar(years, nbr_femmes,label= 'Femme')
+    addlabels(years, nbr_femmes)
     plt.bar(years, nbr_hommes,bottom=nbr_femmes,label= 'Hommes')
+    plt.legend()
     addlabels(years, nbr_total)
+    ax.set_xticks(years)
+    plt.xticks(rotation=90)    
+    plt.tight_layout()
     plt.show()
     
 def evolution_age_median(ctg_path):
     from pathlib import Path
     from collections import Counter
     import os
     import re
@@ -377,22 +361,18 @@
     xt = range(55,90)
     years = [int(x) for x in os.listdir(ctg_path) if re.findall('^\d{4}$',x)]
     nbr_femmes = []
     ratio_femmes = []
     nbr_total = []
     age_mean = [] 
     for year in years:
-        try:
-            df_effectif = pd.read_excel(GLOBAL['ROOT'] / Path(str(year))/ Path('DATA') /Path(str(year)+'.xlsx'))
-        except:
-            df_effectif = pd.read_excel(GLOBAL['ROOT'] / Path('DATA\FICHIERS REFERENCES') / Path(str(year)+'.xlsx'))
-        
+        df_effectif = pd.read_excel(ctg_path / Path(str(year)) / Path('DATA') / Path(str(year)+'.xlsx'))
         df_effectif['Date de naissance'] = pd.to_datetime(df_effectif['Date de naissance'], format="%d/%m/%Y")
         df_effectif['Age']  = df_effectif['Date de naissance'].apply(lambda x : (pd.Timestamp(year, 9, 30)-x).days/365)#.astype(int)
-        print(year,df_effectif['Age'].median())
+        #print(year,df_effectif['Age'].median())
         age_mean.append(df_effectif['Age'].median())
         
     plt.bar(years,age_mean)
     plt.ylabel('Age moyen')
     plt.ylim(50,71)
     linear_model=np.polyfit(years,age_mean,1)
     linear_model_fn=np.poly1d(linear_model)
@@ -446,15 +426,15 @@
     
     df = pd.concat([df, split_df], axis=1)
     df = df.drop('date',axis=1)
     out_path = ctg_path / Path(str(list_date[-1])) / Path('DATA') / Path('effectif_history.xlsx')
     df.to_excel(out_path)
     return out_path
     
-def statistique_vae():
+def statistique_vae(ctg_path):
 
     from datetime import datetime
     from pathlib import Path
     
     import matplotlib.pyplot as plt
     import pandas as pd
     
@@ -469,15 +449,15 @@
     
     last_year = 2018
     years =[]
     nb_vae_m = []
     nb_vae_f = []
     nb_vae_tot = []
     for year in range(last_year,current_year+1):
-        df_N1 = pd.read_excel(Path(GLOBAL['ROOT']) / Path(str(year)) / Path('DATA') /Path(str(year)+'.xlsx'))
+        df_N1 = pd.read_excel(ctg_path / Path(str(year)) / Path('DATA') /Path(str(year)+'.xlsx'))
         years.append(year)
         nb_vae_m.append(sum((df_N1['Pratique VAE'] == 'Oui') & (df_N1['Sexe'] == 'M')))
         nb_vae_f.append(sum((df_N1['Pratique VAE'] == 'Oui') & (df_N1['Sexe'] == 'F')))
         nb_vae_tot.append(sum((df_N1['Pratique VAE'] == 'Oui') & (df_N1['Sexe'] == 'F')) +
                           sum((df_N1['Pratique VAE'] == 'Oui') & (df_N1['Sexe'] == 'M')))
     plt.bar(years, nb_vae_m,label= 'Homme')
     plt.bar(years, nb_vae_f,bottom=nb_vae_m,label= 'Femme')
```

### Comparing `CTG_Utils-1.1.0/CTG_Utils/CTG_Func/CTG_plot.py` & `CTG_Utils-1.1.1/CTG_Utils/CTG_Func/CTG_plot.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 __all_ = ["built_lat_long",
           "plot_club_38",
           "plot_ctg",
           "stat_sorties_club",]
-          
-from CTG_Utils.CTG_Func.CTG_config import GLOBAL   
+             
 
-def plot_club_38():
+def plot_club_38(ctg_path):
 
     # Standard library import
     from pathlib import Path
 
     # 3rd party imports
     import folium
     import numpy as np
     import pandas as pd
 
 
-    df = pd.read_excel(GLOBAL['ROOT'] / Path('club_38.xlsx'))
+    df = pd.read_excel(ctg_path / Path('club_38.xlsx'))
     path_villes_de_france = Path(__file__).parent.parent / Path('CTG_Func') / Path('CTG_RefFiles/villes_france_premium.csv')
     df_villes = pd.read_csv(path_villes_de_france,header=None,usecols=[2,19,20])
     dic_long = dict(zip(df_villes[2] , df_villes[19]))
     dic_lat = dict(zip(df_villes[2] , df_villes[20]))
 
     #df =pd.read_excel(root / Path(effectif))
 
@@ -157,15 +156,15 @@
                 radius=size*100,
                 popup=f'{ville} ({size}): {dict_cyclo[ville]}',
                 color=color,
                 fill=True,
             ).add_to(kol)
     return kol
     
-def stat_sorties_club(path_sorties_club, ylim=None, file_label=None, year = None):
+def stat_sorties_club(path_sorties_club, ctg_path, ylim=None, file_label=None,year = None):
 
     import datetime
     import os
     from pathlib import Path
     from collections import Counter
     from tkinter import messagebox
     
@@ -174,15 +173,14 @@
     from yaml.loader import SafeLoader
     
     from CTG_Utils.CTG_Func.CTG_effectif import read_effectif
     from CTG_Utils.CTG_Func.CTG_effectif import correction_effectif
     from CTG_Utils.CTG_Func.CTG_effectif import read_effectif_corrected
     from CTG_Utils.CTG_Func.CTG_effectif import count_participation
     from CTG_Utils.CTG_Func.CTG_effectif import parse_date
-    from CTG_Utils.CTG_Func.CTG_config import GLOBAL 
     
     def addlabels(x,y):
         for i in range(len(x)):
             if info_rando is not None:
                 if x[i] in info_rando.keys():
                     plt.text(i-0.2,y[i]+1,
                              info_rando[x[i]][0],
@@ -194,15 +192,15 @@
         flag_labels = True
         with open(file_label,'r') as f:
             info_rando_dict = yaml.safe_load(f)
             info_rando = info_rando_dict['INFO_RANDO']
     else:
         flag_labels = False
     
-    no_match,df_total,_ = count_participation(path_sorties_club,year,info_rando)
+    no_match,df_total,_ = count_participation(path_sorties_club,ctg_path,year,info_rando)
     if no_match is None:
         messagebox.showinfo('WARNING',"Aucun participant n'a participé à ce type de sortie" )
     else:
         text_message = ''
         for tup in no_match:
               text_message += f'Le nom {tup[1]}, {tup[2]} est inconnu dans le fichier : "{os.path.split(tup[0])[-1]}"'
               text_message += '\n'
@@ -210,18 +208,19 @@
         if len(text_message) : messagebox.showinfo('WARNING',text_message )
     
     if year is None:
         currentDateTime = datetime.datetime.now()
         date = currentDateTime.date()
         year = date.strftime("%Y")
         
-    list_non_licencie, dic_correction_licence, dic_part_club = correction_effectif(year)
+    list_non_licencie, dic_correction_licence, dic_part_club = correction_effectif(year,ctg_path)
     df_effectif = read_effectif_corrected(dic_correction_licence,
                                           list_non_licencie,
                                           dic_part_club,
+                                          ctg_path,
                                           year)
     
     dic_sexe = dict(zip(df_effectif['N° Licencié'], df_effectif['Sexe']))
     dic_sexe[None] = 'irrelevant'
     dic_vae =dict(zip(df_effectif['N° Licencié'],df_effectif['Pratique VAE']))
 
     df_total['sexe'] = df_total['N° Licencié'].map(dic_sexe)
@@ -254,34 +253,34 @@
                                 ('Femme', 'VAE'): '#ff7f0e',
                                 ('Homme', 'Musculaire'): '#2ca02c',
                                 ('Homme', 'VAE'): '#d62728',} )
     
     if flag_labels : addlabels(dg.index,dg.sum(axis=1).astype(int).tolist())
     
     plt.xlabel('')
-    plt.tick_params(axis='x', rotation=90,labelsize=GLOBAL['LABEL_SIZE'])
-    plt.ylabel('Nombre de licenciers',size=GLOBAL['LABEL_SIZE'])
+    plt.tick_params(axis='x', rotation=90,labelsize=15)
+    plt.ylabel('Nombre de licenciers',size=15)
     plt.xlabel('')
-    plt.tick_params(axis='x', rotation=90,labelsize=GLOBAL['LABEL_SIZE'])
-    plt.tick_params(axis='y',labelsize=GLOBAL['LABEL_SIZE'])
+    plt.tick_params(axis='x', rotation=90,labelsize=15)
+    plt.tick_params(axis='y',labelsize=15)
     type_sortie = os.path.split(path_sorties_club)[-1] + ' ' + str(year)
-    plt.title(type_sortie,fontsize=GLOBAL['LABEL_SIZE'],pad=50)
+    plt.title(type_sortie,fontsize=15,pad=50)
     
     if ylim is not None:
         plt.ylim(ylim)
     else:
         ylim = (0,1.5*max(Counter(df_total['sejour']).values()))
         plt.ylim(ylim)
 
     
     plt.legend(bbox_to_anchor =(0.75, 1.15), ncol = 2)
     plt.tight_layout()
     plt.show()
     fig_file = os.path.split(path_sorties_club)[-1].replace(' ','_')+'.png'
-    plt.savefig(Path(GLOBAL['ROOT']) / Path(str(year)) / Path('STATISTIQUES') / Path(fig_file),bbox_inches='tight')
+    plt.savefig(ctg_path / Path(str(year)) / Path('STATISTIQUES') / Path(fig_file),bbox_inches='tight')
     
     return df_total
 
 def _distance(ϕ1, λ1,ϕ2, λ2):
     from math import asin, cos, radians, sin, sqrt
     ϕ1, λ1 = radians(ϕ1), radians(λ1)
     ϕ2, λ2 = radians(ϕ2), radians(λ2)
```

### Comparing `CTG_Utils-1.1.0/CTG_Utils/CTG_Func/CTG_synthese.py` & `CTG_Utils-1.1.1/CTG_Utils/CTG_Func/CTG_synthese.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,970 +1,973 @@
-00000000: 0d0a 6672 6f6d 2043 5447 5f55 7469 6c73  ..from CTG_Utils
-00000010: 2e43 5447 5f46 756e 632e 4354 475f 636f  .CTG_Func.CTG_co
-00000020: 6e66 6967 2069 6d70 6f72 7420 474c 4f42  nfig import GLOB
-00000030: 414c 2020 0d0a 0d0a 6465 6620 7379 6e74  AL  ....def synt
-00000040: 6865 7365 2879 6561 722c 6374 675f 7061  hese(year,ctg_pa
-00000050: 7468 293a 0d0a 0d0a 2020 2020 696d 706f  th):....    impo
-00000060: 7274 206f 730d 0a20 2020 2066 726f 6d20  rt os..    from 
-00000070: 7061 7468 6c69 6220 696d 706f 7274 2050  pathlib import P
-00000080: 6174 680d 0a20 2020 200d 0a20 2020 2066  ath..    ..    f
-00000090: 726f 6d20 4354 475f 5574 696c 732e 4354  rom CTG_Utils.CT
-000000a0: 475f 4675 6e63 2e43 5447 5f65 6666 6563  G_Func.CTG_effec
-000000b0: 7469 6620 696d 706f 7274 2063 6f72 7265  tif import corre
-000000c0: 6374 696f 6e5f 6566 6665 6374 6966 0d0a  ction_effectif..
-000000d0: 2020 2020 6672 6f6d 2043 5447 5f55 7469      from CTG_Uti
-000000e0: 6c73 2e43 5447 5f46 756e 632e 4354 475f  ls.CTG_Func.CTG_
-000000f0: 6566 6665 6374 6966 2069 6d70 6f72 7420  effectif import 
-00000100: 7265 6164 5f65 6666 6563 7469 665f 636f  read_effectif_co
-00000110: 7272 6563 7465 640d 0a20 2020 200d 0a20  rrected..    .. 
-00000120: 2020 2069 6d70 6f72 7420 7061 6e64 6173     import pandas
-00000130: 2061 7320 7064 0d0a 2020 2020 0d0a 2020   as pd..    ..  
-00000140: 2020 0d0a 2020 2020 7061 7468 5f64 6972    ..    path_dir
-00000150: 5f6c 6973 7420 3d20 5b63 7467 5f70 6174  _list = [ctg_pat
-00000160: 6820 2f20 5061 7468 2873 7472 2879 6561  h / Path(str(yea
-00000170: 7229 2920 2f20 5061 7468 2827 534f 5254  r)) / Path('SORT
-00000180: 4945 5320 4455 2053 414d 4544 4927 2920  IES DU SAMEDI') 
-00000190: 2f20 5061 7468 2827 4558 4345 4c27 292c  / Path('EXCEL'),
-000001a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000001b0: 2020 2020 2020 2063 7467 5f70 6174 6820         ctg_path 
-000001c0: 2f20 5061 7468 2873 7472 2879 6561 7229  / Path(str(year)
-000001d0: 2920 2f20 5061 7468 2827 534f 5254 4945  ) / Path('SORTIE
-000001e0: 5320 4455 2044 494d 414e 4348 4527 2920  S DU DIMANCHE') 
-000001f0: 2f20 5061 7468 2827 4558 4345 4c27 292c  / Path('EXCEL'),
-00000200: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00000210: 2020 2020 2020 2063 7467 5f70 6174 6820         ctg_path 
-00000220: 2f20 5061 7468 2873 7472 2879 6561 7229  / Path(str(year)
-00000230: 2920 2f20 5061 7468 2827 534f 5254 4945  ) / Path('SORTIE
-00000240: 5320 4455 204a 4555 4449 2729 202f 2050  S DU JEUDI') / P
-00000250: 6174 6828 2745 5843 454c 2729 2c0d 0a20  ath('EXCEL'),.. 
-00000260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000270: 2020 2020 6374 675f 7061 7468 202f 2050      ctg_path / P
-00000280: 6174 6828 7374 7228 7965 6172 2929 202f  ath(str(year)) /
-00000290: 2050 6174 6828 2753 4f52 5449 4553 2048   Path('SORTIES H
-000002a0: 4956 4552 2729 202f 2050 6174 6828 2745  IVER') / Path('E
-000002b0: 5843 454c 2729 2c0d 0a20 2020 2020 2020  XCEL'),..       
-000002c0: 2020 2020 2020 2020 2020 2020 2020 6374                ct
-000002d0: 675f 7061 7468 202f 2050 6174 6828 7374  g_path / Path(st
-000002e0: 7228 7965 6172 2929 202f 2050 6174 6828  r(year)) / Path(
-000002f0: 2753 4f52 5449 4553 2044 5520 4c55 4e44  'SORTIES DU LUND
-00000300: 4927 292f 2050 6174 6828 2745 5843 454c  I')/ Path('EXCEL
-00000310: 2729 2c0d 0a20 2020 2020 2020 2020 2020  '),..           
-00000320: 2020 2020 2020 2020 2020 6374 675f 7061            ctg_pa
-00000330: 7468 202f 2050 6174 6828 7374 7228 7965  th / Path(str(ye
-00000340: 6172 2929 202f 2050 6174 6828 2753 454a  ar)) / Path('SEJ
-00000350: 4f55 5227 2920 2f20 5061 7468 2827 4558  OUR') / Path('EX
-00000360: 4345 4c27 295d 0d0a 0d0a 2020 2020 6c69  CEL')]....    li
-00000370: 7374 5f64 6620 3d20 5b5d 0d0a 2020 2020  st_df = []..    
-00000380: 666f 7220 7061 7468 5f64 6972 2069 6e20  for path_dir in 
-00000390: 7061 7468 5f64 6972 5f6c 6973 743a 0d0a  path_dir_list:..
-000003a0: 2020 2020 2020 2020 6966 206f 732e 7061          if os.pa
-000003b0: 7468 2e69 7364 6972 2870 6174 685f 6469  th.isdir(path_di
-000003c0: 7229 3a0d 0a20 2020 2020 2020 2020 2020  r):..           
-000003d0: 2066 696c 6573 203d 205b 7820 666f 7220   files = [x for 
-000003e0: 7820 696e 206f 732e 6c69 7374 6469 7228  x in os.listdir(
-000003f0: 7061 7468 5f64 6972 2920 6966 2078 2e65  path_dir) if x.e
-00000400: 6e64 7377 6974 6828 272e 786c 7378 2729  ndswith('.xlsx')
-00000410: 2061 6e64 2022 7e24 2220 6e6f 7420 696e   and "~$" not in
-00000420: 2078 5d20 0d0a 2020 2020 2020 2020 2020   x] ..          
-00000430: 2020 6c69 7374 5f64 662e 6578 7465 6e64    list_df.extend
-00000440: 285b 7064 2e72 6561 645f 6578 6365 6c28  ([pd.read_excel(
-00000450: 7061 7468 5f64 6972 202f 2050 6174 6828  path_dir / Path(
-00000460: 6669 6c65 292c 2065 6e67 696e 653d 276f  file), engine='o
-00000470: 7065 6e70 7978 6c27 2920 666f 7220 6669  penpyxl') for fi
-00000480: 6c65 2069 6e20 6669 6c65 735d 290d 0a20  le in files]).. 
-00000490: 2020 200d 0a20 2020 2064 665f 746f 7461     ..    df_tota
-000004a0: 6c20 3d20 7064 2e63 6f6e 6361 7428 6c69  l = pd.concat(li
-000004b0: 7374 5f64 662c 2069 676e 6f72 655f 696e  st_df, ignore_in
-000004c0: 6465 783d 5472 7565 290d 0a20 2020 200d  dex=True)..    .
-000004d0: 0a20 2020 206c 6973 745f 6e6f 6e5f 6c69  .    list_non_li
-000004e0: 6365 6e63 6965 2c20 6469 635f 636f 7272  cencie, dic_corr
-000004f0: 6563 7469 6f6e 5f6c 6963 656e 6365 2c20  ection_licence, 
-00000500: 6469 635f 7061 7274 5f63 6c75 6220 3d20  dic_part_club = 
-00000510: 636f 7272 6563 7469 6f6e 5f65 6666 6563  correction_effec
-00000520: 7469 6628 7965 6172 290d 0a20 2020 2064  tif(year)..    d
-00000530: 665f 6566 6665 6374 6966 203d 2072 6561  f_effectif = rea
-00000540: 645f 6566 6665 6374 6966 5f63 6f72 7265  d_effectif_corre
-00000550: 6374 6564 2864 6963 5f63 6f72 7265 6374  cted(dic_correct
-00000560: 696f 6e5f 6c69 6365 6e63 652c 206c 6973  ion_licence, lis
-00000570: 745f 6e6f 6e5f 6c69 6365 6e63 6965 2c20  t_non_licencie, 
-00000580: 6469 635f 7061 7274 5f63 6c75 6229 0d0a  dic_part_club)..
-00000590: 2020 2020 0d0a 2020 2020 6466 5f74 6f74      ..    df_tot
-000005a0: 616c 5b27 5072 6174 6971 7565 2056 4145  al['Pratique VAE
-000005b0: 275d 2e66 696c 6c6e 6128 274e 6f6e 272c  '].fillna('Non',
-000005c0: 696e 706c 6163 653d 5472 7565 290d 0a20  inplace=True).. 
-000005d0: 2020 200d 0a20 2020 2023 206e 6f6d 6272     ..    # nombr
-000005e0: 6520 6d6f 7965 6e20 6465 2070 6172 7469  e moyen de parti
-000005f0: 6369 7061 6e74 2070 6172 2061 6374 6976  cipant par activ
-00000600: 6974 c3a9 0d0a 2020 2020 666f 7220 7820  it....    for x 
-00000610: 696e 2064 665f 746f 7461 6c2e 6772 6f75  in df_total.grou
-00000620: 7062 7928 5b27 5479 7065 275d 293a 0d0a  pby(['Type']):..
-00000630: 2020 2020 2020 2020 7072 696e 7428 785b          print(x[
-00000640: 305d 2c6c 656e 2878 5b31 5d29 2c6c 656e  0],len(x[1]),len
-00000650: 2873 6574 2878 5b31 5d5b 2773 656a 6f75  (set(x[1]['sejou
-00000660: 7227 5d29 292c 6c65 6e28 785b 315d 292f  r'])),len(x[1])/
-00000670: 6c65 6e28 7365 7428 785b 315d 5b27 7365  len(set(x[1]['se
-00000680: 6a6f 7572 275d 2929 290d 0a20 2020 200d  jour'])))..    .
-00000690: 0a20 2020 2066 696c 6520 3d20 6374 675f  .    file = ctg_
-000006a0: 7061 7468 202f 2050 6174 6828 7374 7228  path / Path(str(
-000006b0: 7965 6172 2929 202f 2050 6174 6828 2753  year)) / Path('S
-000006c0: 5441 5449 5354 4951 5545 5327 2920 2f20  TATISTIQUES') / 
-000006d0: 5061 7468 2827 7379 6e74 6865 7365 2e78  Path('synthese.x
-000006e0: 6c73 7827 290d 0a20 2020 2064 665f 746f  lsx')..    df_to
-000006f0: 7461 6c2e 746f 5f65 7863 656c 2866 696c  tal.to_excel(fil
-00000700: 6529 0d0a 0d0a 6465 6620 706c 6f74 5f70  e)....def plot_p
-00000710: 6965 5f73 796e 7468 6573 6528 7965 6172  ie_synthese(year
-00000720: 2c63 7467 5f70 6174 6829 3a0d 0a20 2020  ,ctg_path):..   
-00000730: 200d 0a20 2020 2066 726f 6d20 7061 7468   ..    from path
-00000740: 6c69 6220 696d 706f 7274 2050 6174 680d  lib import Path.
-00000750: 0a20 2020 200d 0a20 2020 2069 6d70 6f72  .    ..    impor
-00000760: 7420 6e75 6d70 7920 6173 206e 700d 0a20  t numpy as np.. 
-00000770: 2020 2069 6d70 6f72 7420 6d61 7470 6c6f     import matplo
-00000780: 746c 6962 2e70 7970 6c6f 7420 6173 2070  tlib.pyplot as p
-00000790: 6c74 0d0a 2020 2020 696d 706f 7274 2070  lt..    import p
-000007a0: 616e 6461 7320 6173 2070 640d 0a20 2020  andas as pd..   
-000007b0: 200d 0a20 2020 2064 6566 2066 756e 6328   ..    def func(
-000007c0: 7063 742c 2061 6c6c 7661 6c75 6573 293a  pct, allvalues):
-000007d0: 0d0a 2020 2020 2020 2020 6162 736f 6c75  ..        absolu
-000007e0: 7465 203d 2072 6f75 6e64 2870 6374 202f  te = round(pct /
-000007f0: 2031 3030 2e2a 6e70 2e73 756d 2861 6c6c   100.*np.sum(all
-00000800: 7661 6c75 6573 292c 3029 0d0a 2020 2020  values),0)..    
-00000810: 2020 2020 2372 6574 7572 6e20 227b 3a2e      #return "{:.
-00000820: 3166 7d25 5c6e 287b 3a64 7d29 222e 666f  1f}%\n({:d})".fo
-00000830: 726d 6174 2870 6374 2c20 6162 736f 6c75  rmat(pct, absolu
-00000840: 7465 290d 0a20 2020 2020 2020 2072 6574  te)..        ret
-00000850: 7572 6e20 2066 227b 696e 7428 726f 756e  urn  f"{int(roun
-00000860: 6428 6162 736f 6c75 7465 2c31 2929 7d5c  d(absolute,1))}\
-00000870: 6e7b 726f 756e 6428 7063 742c 3129 7d20  n{round(pct,1)} 
-00000880: 2522 0d0a 2020 2020 2020 2020 0d0a 2020  %"..        ..  
-00000890: 2020 6669 6c65 5f69 6e20 3d20 6374 675f    file_in = ctg_
-000008a0: 7061 7468 202f 2050 6174 6828 7374 7228  path / Path(str(
-000008b0: 7965 6172 2929 202f 2050 6174 6828 2753  year)) / Path('S
-000008c0: 5441 5449 5354 4951 5545 5327 2920 2f20  TATISTIQUES') / 
-000008d0: 5061 7468 2827 7379 6e74 6865 7365 2e78  Path('synthese.x
-000008e0: 6c73 7827 290d 0a20 2020 2064 665f 746f  lsx')..    df_to
-000008f0: 7461 6c20 3d20 7064 2e72 6561 645f 6578  tal = pd.read_ex
-00000900: 6365 6c28 6669 6c65 5f69 6e29 0d0a 2020  cel(file_in)..  
-00000910: 2020 6466 5f74 6f74 616c 203d 2064 665f    df_total = df_
-00000920: 746f 7461 6c2e 6472 6f70 6e61 2873 7562  total.dropna(sub
-00000930: 7365 743d 5b27 5479 7065 275d 2920 0d0a  set=['Type']) ..
-00000940: 2020 2020 6466 5f74 6f74 616c 203d 2064      df_total = d
-00000950: 665f 746f 7461 6c2e 6472 6f70 6e61 2873  f_total.dropna(s
-00000960: 7562 7365 743d 5b27 4e6f 6d27 5d29 0d0a  ubset=['Nom'])..
-00000970: 0d0a 2020 2020 6461 6767 203d 2064 665f  ..    dagg = df_
-00000980: 746f 7461 6c2e 6772 6f75 7062 7928 2754  total.groupby('T
-00000990: 7970 6527 295b 276e 6272 5f6a 6f75 7273  ype')['nbr_jours
-000009a0: 275d 2e61 6767 2873 756d 290d 0a0d 0a20  '].agg(sum).... 
-000009b0: 2020 200d 0a20 2020 200d 0a20 2020 2065     ..    ..    e
-000009c0: 7870 6c6f 6465 5f64 6963 203d 207b 2752  xplode_dic = {'R
-000009d0: 414e 444f 4e4e 4545 273a 302e 312c 0d0a  ANDONNEE':0.1,..
-000009e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000009f0: 2020 2027 5345 4a4f 5552 273a 302e 302c     'SEJOUR':0.0,
-00000a00: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-00000a10: 2020 2020 2020 2753 4f52 5449 4553 2044        'SORTIES D
-00000a20: 5520 4449 4d41 4e43 4845 273a 302e 322c  U DIMANCHE':0.2,
-00000a30: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00000a40: 2020 2020 2027 534f 5254 4945 5320 4455       'SORTIES DU
-00000a50: 204a 4555 4449 273a 302e 322c 0d0a 2020   JEUDI':0.2,..  
-00000a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000a70: 2027 534f 5254 4945 5320 4455 204c 554e   'SORTIES DU LUN
-00000a80: 4449 273a 302e 322c 200d 0a20 2020 2020  DI':0.2, ..     
-00000a90: 2020 2020 2020 2020 2020 2020 2020 2753                'S
-00000aa0: 4f52 5449 4553 2044 5520 5341 4d45 4449  ORTIES DU SAMEDI
-00000ab0: 273a 302e 322c 0d0a 2020 2020 2020 2020  ':0.2,..        
-00000ac0: 2020 2020 2020 2020 2020 2027 534f 5254             'SORT
-00000ad0: 4945 5320 4849 5645 5227 3a30 2e32 7d0d  IES HIVER':0.2}.
-00000ae0: 0a0d 0a20 2020 2064 6174 6120 3d20 5b5d  ...    data = []
-00000af0: 0d0a 2020 2020 736f 7274 6965 7320 3d20  ..    sorties = 
-00000b00: 5b5d 0d0a 2020 2020 666f 7220 7479 7065  []..    for type
-00000b10: 5f73 656a 6f75 722c 206e 6272 2069 6e20  _sejour, nbr in 
-00000b20: 7a69 7028 6461 6767 2e69 6e64 6578 2c64  zip(dagg.index,d
-00000b30: 6167 672e 746f 6c69 7374 2829 293a 0d0a  agg.tolist()):..
-00000b40: 2020 2020 2020 2020 6966 206e 6272 213d          if nbr!=
-00000b50: 303a 0d0a 2020 2020 2020 2020 2020 2020  0:..            
-00000b60: 6461 7461 2e61 7070 656e 6428 6e62 7229  data.append(nbr)
-00000b70: 0d0a 2020 2020 2020 2020 2020 2020 736f  ..            so
-00000b80: 7274 6965 732e 6170 7065 6e64 2874 7970  rties.append(typ
-00000b90: 655f 7365 6a6f 7572 290d 0a0d 0a20 2020  e_sejour)....   
-00000ba0: 2065 7870 6c6f 6465 203d 205b 6578 706c   explode = [expl
-00000bb0: 6f64 655f 6469 635b 7479 705d 2066 6f72  ode_dic[typ] for
-00000bc0: 2074 7970 2069 6e20 736f 7274 6965 735d   typ in sorties]
-00000bd0: 0d0a 2020 2020 0d0a 2020 2020 0d0a 2020  ..    ..    ..  
-00000be0: 2020 2320 4372 6561 7469 6e67 2070 6c6f    # Creating plo
-00000bf0: 740d 0a20 2020 2066 6967 203d 2070 6c74  t..    fig = plt
-00000c00: 2e66 6967 7572 6528 6669 6773 697a 6520  .figure(figsize 
-00000c10: 3d28 3130 2c20 3729 290d 0a20 2020 205f  =(10, 7))..    _
-00000c20: 2c20 5f2c 2061 7574 6f74 6578 7473 203d  , _, autotexts =
-00000c30: 2070 6c74 2e70 6965 2864 6174 612c 0d0a   plt.pie(data,..
-00000c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000c50: 2020 2020 2020 2020 2020 2020 2020 6c61                la
-00000c60: 6265 6c73 203d 2073 6f72 7469 6573 2c0d  bels = sorties,.
-00000c70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000c80: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-00000c90: 7574 6f70 6374 203d 206c 616d 6264 6120  utopct = lambda 
-00000ca0: 7063 743a 2066 756e 6328 7063 742c 2064  pct: func(pct, d
-00000cb0: 6174 6129 2c0d 0a20 2020 2020 2020 2020  ata),..         
-00000cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000cd0: 2020 2020 2065 7870 6c6f 6465 203d 2065       explode = e
-00000ce0: 7870 6c6f 6465 2c0d 0a20 2020 2020 2020  xplode,..       
-00000cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000d00: 2020 2020 2020 2074 6578 7470 726f 7073         textprops
-00000d10: 3d7b 2766 6f6e 7473 697a 6527 3a20 3138  ={'fontsize': 18
-00000d20: 7d29 0d0a 2020 2020 706c 742e 7469 746c  })..    plt.titl
-00000d30: 6528 7374 7228 7965 6172 292c 2070 6164  e(str(year), pad
-00000d40: 3d35 302c 2066 6f6e 7473 697a 653d 3230  =50, fontsize=20
-00000d50: 290d 0a20 2020 200d 0a20 2020 205f 203d  )..    ..    _ =
-00000d60: 2070 6c74 2e73 6574 7028 6175 746f 7465   plt.setp(autote
-00000d70: 7874 732c 202a 2a7b 2763 6f6c 6f72 273a  xts, **{'color':
-00000d80: 276b 272c 2027 7765 6967 6874 273a 2762  'k', 'weight':'b
-00000d90: 6f6c 6427 2c20 2766 6f6e 7473 697a 6527  old', 'fontsize'
-00000da0: 3a31 347d 290d 0a20 2020 200d 0a20 2020  :14})..    ..   
-00000db0: 2070 6c74 2e74 6967 6874 5f6c 6179 6f75   plt.tight_layou
-00000dc0: 7428 290d 0a20 2020 2070 6c74 2e73 686f  t()..    plt.sho
-00000dd0: 7728 290d 0a20 2020 200d 0a20 2020 2066  w()..    ..    f
-00000de0: 6967 5f66 696c 6520 3d20 2753 4f52 5449  ig_file = 'SORTI
-00000df0: 4553 5f50 4945 2e70 6e67 270d 0a20 2020  ES_PIE.png'..   
-00000e00: 2070 6c74 2e73 6176 6566 6967 2850 6174   plt.savefig(Pat
-00000e10: 6828 474c 4f42 414c 5b27 524f 4f54 275d  h(GLOBAL['ROOT']
-00000e20: 2920 2f20 5061 7468 2873 7472 2879 6561  ) / Path(str(yea
-00000e30: 7229 2920 2f20 5061 7468 2827 5354 4154  r)) / Path('STAT
-00000e40: 4953 5449 5155 4553 2729 202f 2050 6174  ISTIQUES') / Pat
-00000e50: 6828 6669 675f 6669 6c65 292c 6262 6f78  h(fig_file),bbox
-00000e60: 5f69 6e63 6865 733d 2774 6967 6874 2729  _inches='tight')
-00000e70: 090d 0a0d 0a20 2020 2072 6574 7572 6e20  .....    return 
-00000e80: 090d 0a09 0d0a 0d0a 6465 6620 7379 6e74  ........def synt
-00000e90: 6865 7365 5f61 6468 6572 656e 7428 7965  hese_adherent(ye
-00000ea0: 6172 2c63 7467 5f70 6174 6829 3a0d 0a0d  ar,ctg_path):...
-00000eb0: 0a20 2020 2066 726f 6d20 7061 7468 6c69  .    from pathli
-00000ec0: 6220 696d 706f 7274 2050 6174 680d 0a20  b import Path.. 
-00000ed0: 2020 200d 0a20 2020 2069 6d70 6f72 7420     ..    import 
-00000ee0: 7061 6e64 6173 2061 7320 7064 0d0a 2020  pandas as pd..  
-00000ef0: 2020 0d0a 2020 2020 6672 6f6d 2043 5447    ..    from CTG
-00000f00: 5f55 7469 6c73 2e43 5447 5f46 756e 632e  _Utils.CTG_Func.
-00000f10: 4354 4743 6c61 7373 6573 2069 6d70 6f72  CTGClasses impor
-00000f20: 7420 4566 6665 6374 6966 4374 670d 0a20  t EffectifCtg.. 
-00000f30: 2020 200d 0a20 2020 2066 696c 655f 696e     ..    file_in
-00000f40: 203d 2063 7467 5f70 6174 6820 2f20 5061   = ctg_path / Pa
-00000f50: 7468 2873 7472 2879 6561 7229 2920 2f20  th(str(year)) / 
-00000f60: 5061 7468 2827 5354 4154 4953 5449 5155  Path('STATISTIQU
-00000f70: 4553 2729 202f 2050 6174 6828 2773 796e  ES') / Path('syn
-00000f80: 7468 6573 652e 786c 7378 2729 0d0a 2020  these.xlsx')..  
-00000f90: 2020 6466 5f74 6f74 616c 203d 2070 642e    df_total = pd.
-00000fa0: 7265 6164 5f65 7863 656c 2866 696c 655f  read_excel(file_
-00000fb0: 696e 290d 0a20 2020 2064 665f 746f 7461  in)..    df_tota
-00000fc0: 6c20 3d20 6466 5f74 6f74 616c 2e64 726f  l = df_total.dro
-00000fd0: 706e 6128 7375 6273 6574 3d5b 2754 7970  pna(subset=['Typ
-00000fe0: 6527 5d29 0d0a 2020 2020 6e62 7265 203d  e'])..    nbre =
-00000ff0: 207b 7d0d 0a20 2020 200d 0a20 2020 2066   {}..    ..    f
-00001000: 6f72 2069 645f 6c69 6365 6e63 652c 2064  or id_licence, d
-00001010: 6720 696e 2064 665f 746f 7461 6c2e 6772  g in df_total.gr
-00001020: 6f75 7062 7928 274e c2b0 204c 6963 656e  oupby('N.. Licen
-00001030: 6369 c3a9 2729 3a0d 0a20 2020 2020 2020  ci..'):..       
-00001040: 200d 0a20 2020 2020 2020 206e 6272 655b   ..        nbre[
-00001050: 6964 5f6c 6963 656e 6365 5d3d 5b64 675b  id_licence]=[dg[
-00001060: 274e 6f6d 275d 2e75 6e69 7175 6528 295b  'Nom'].unique()[
-00001070: 305d 2c64 675b 2750 72c3 a96e 6f6d 275d  0],dg['Pr..nom']
-00001080: 2e75 6e69 7175 6528 295b 305d 5d0d 0a20  .unique()[0]].. 
-00001090: 2020 200d 0a20 2020 2020 2020 206e 625f     ..        nb_
-000010a0: 736f 7274 6965 5f64 696d 616e 6368 6520  sortie_dimanche 
-000010b0: 3d20 6c65 6e28 6467 2e71 7565 7279 2822  = len(dg.query("
-000010c0: 5479 7065 2e73 7472 2e63 6f6e 7461 696e  Type.str.contain
-000010d0: 7328 2753 4f52 5449 4553 2044 5520 4449  s('SORTIES DU DI
-000010e0: 4d41 4e43 4845 2729 2229 290d 0a20 2020  MANCHE')"))..   
-000010f0: 2020 2020 206e 6272 655b 6964 5f6c 6963       nbre[id_lic
-00001100: 656e 6365 5d20 3d20 6e62 7265 5b69 645f  ence] = nbre[id_
-00001110: 6c69 6365 6e63 655d 202b 205b 6e62 5f73  licence] + [nb_s
-00001120: 6f72 7469 655f 6469 6d61 6e63 6865 5d0d  ortie_dimanche].
-00001130: 0a20 2020 200d 0a20 2020 2020 2020 206e  .    ..        n
-00001140: 625f 736f 7274 6965 5f73 616d 6564 6920  b_sortie_samedi 
-00001150: 3d20 6c65 6e28 6467 2e71 7565 7279 2822  = len(dg.query("
-00001160: 5479 7065 2e73 7472 2e63 6f6e 7461 696e  Type.str.contain
-00001170: 7328 2753 4f52 5449 4553 2044 5520 5341  s('SORTIES DU SA
-00001180: 4d45 4449 2729 2229 290d 0a20 2020 2020  MEDI')"))..     
-00001190: 2020 206e 6272 655b 6964 5f6c 6963 656e     nbre[id_licen
-000011a0: 6365 5d20 3d20 6e62 7265 5b69 645f 6c69  ce] = nbre[id_li
-000011b0: 6365 6e63 655d 202b 205b 6e62 5f73 6f72  cence] + [nb_sor
-000011c0: 7469 655f 7361 6d65 6469 5d0d 0a20 2020  tie_samedi]..   
-000011d0: 200d 0a20 2020 2020 2020 206e 625f 736f   ..        nb_so
-000011e0: 7274 6965 5f6a 6575 6469 203d 206c 656e  rtie_jeudi = len
-000011f0: 2864 672e 7175 6572 7928 2254 7970 652e  (dg.query("Type.
-00001200: 7374 722e 636f 6e74 6169 6e73 2827 534f  str.contains('SO
-00001210: 5254 4945 5320 4455 204a 4555 4449 2729  RTIES DU JEUDI')
-00001220: 2229 290d 0a20 2020 2020 2020 206e 6272  "))..        nbr
-00001230: 655b 6964 5f6c 6963 656e 6365 5d20 3d20  e[id_licence] = 
-00001240: 6e62 7265 5b69 645f 6c69 6365 6e63 655d  nbre[id_licence]
-00001250: 202b 205b 6e62 5f73 6f72 7469 655f 6a65   + [nb_sortie_je
-00001260: 7564 695d 0d0a 2020 2020 0d0a 2020 2020  udi]..    ..    
-00001270: 2020 2020 6e62 5f72 616e 646f 203d 206c      nb_rando = l
-00001280: 656e 2864 672e 7175 6572 7928 2254 7970  en(dg.query("Typ
-00001290: 652e 7374 722e 636f 6e74 6169 6e73 2827  e.str.contains('
-000012a0: 5241 4e44 4f4e 4e45 4527 2922 2929 0d0a  RANDONNEE')"))..
-000012b0: 2020 2020 2020 2020 6e62 7265 5b69 645f          nbre[id_
-000012c0: 6c69 6365 6e63 655d 203d 206e 6272 655b  licence] = nbre[
-000012d0: 6964 5f6c 6963 656e 6365 5d20 2b20 5b6e  id_licence] + [n
-000012e0: 625f 7261 6e64 6f5d 0d0a 2020 2020 0d0a  b_rando]..    ..
-000012f0: 2020 2020 2020 2020 6e62 5f73 656a 6f75          nb_sejou
-00001300: 725f 6a6f 7572 7320 3d20 7375 6d28 6467  r_jours = sum(dg
-00001310: 2e71 7565 7279 2822 5479 7065 2e73 7472  .query("Type.str
-00001320: 2e63 6f6e 7461 696e 7328 2753 454a 4f55  .contains('SEJOU
-00001330: 5227 2922 295b 276e 6272 5f6a 6f75 7273  R')")['nbr_jours
-00001340: 275d 2e74 6f6c 6973 7428 2929 0d0a 2020  '].tolist())..  
-00001350: 2020 2020 2020 6e62 7265 5b69 645f 6c69        nbre[id_li
-00001360: 6365 6e63 655d 203d 206e 6272 655b 6964  cence] = nbre[id
-00001370: 5f6c 6963 656e 6365 5d20 2b20 5b6e 625f  _licence] + [nb_
-00001380: 7365 6a6f 7572 5f6a 6f75 7273 5d0d 0a0d  sejour_jours]...
-00001390: 0a20 2020 2020 2020 206e 625f 7365 6a6f  .        nb_sejo
-000013a0: 7572 203d 206c 656e 2864 672e 7175 6572  ur = len(dg.quer
-000013b0: 7928 2254 7970 652e 7374 722e 636f 6e74  y("Type.str.cont
-000013c0: 6169 6e73 2827 5345 4a4f 5552 2729 2229  ains('SEJOUR')")
-000013d0: 5b27 7365 6a6f 7572 275d 2e75 6e69 7175  ['sejour'].uniqu
-000013e0: 6528 2929 0d0a 2020 2020 2020 2020 6e62  e())..        nb
-000013f0: 7265 5b69 645f 6c69 6365 6e63 655d 203d  re[id_licence] =
-00001400: 206e 6272 655b 6964 5f6c 6963 656e 6365   nbre[id_licence
-00001410: 5d20 2b20 5b6e 625f 7365 6a6f 7572 5d0d  ] + [nb_sejour].
-00001420: 0a20 2020 200d 0a20 2020 2020 2020 206e  .    ..        n
-00001430: 625f 6869 7665 7220 3d20 6c65 6e28 6467  b_hiver = len(dg
-00001440: 2e71 7565 7279 2822 5479 7065 2e73 7472  .query("Type.str
-00001450: 2e63 6f6e 7461 696e 7328 2753 4f52 5449  .contains('SORTI
-00001460: 4553 2048 4956 4552 2729 2229 290d 0a20  ES HIVER')")).. 
-00001470: 2020 2020 2020 206e 6272 655b 6964 5f6c         nbre[id_l
-00001480: 6963 656e 6365 5d20 3d20 6e62 7265 5b69  icence] = nbre[i
-00001490: 645f 6c69 6365 6e63 655d 202b 205b 6e62  d_licence] + [nb
-000014a0: 5f68 6976 6572 5d0d 0a20 2020 200d 0a20  _hiver]..    .. 
-000014b0: 2020 2020 2020 206e 6272 5f65 7665 6e65         nbr_evene
-000014c0: 6d65 6e74 7320 3d20 5b6e 625f 736f 7274  ments = [nb_sort
-000014d0: 6965 5f64 696d 616e 6368 6520 2b0d 0a20  ie_dimanche +.. 
-000014e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000014f0: 2020 2020 2020 2020 206e 625f 736f 7274           nb_sort
-00001500: 6965 5f73 616d 6564 6920 2b20 0d0a 2020  ie_samedi + ..  
-00001510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001520: 2020 2020 2020 2020 6e62 5f73 6f72 7469          nb_sorti
-00001530: 655f 6a65 7564 6920 2b0d 0a20 2020 2020  e_jeudi +..     
-00001540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001550: 2020 2020 206e 625f 7261 6e64 6f20 2b0d       nb_rando +.
-00001560: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001570: 2020 2020 2020 2020 2020 206e 625f 7365             nb_se
-00001580: 6a6f 7572 5f6a 6f75 7273 202b 0d0a 2020  jour_jours +..  
+00000000: 0d0a 6465 6620 7379 6e74 6865 7365 2879  ..def synthese(y
+00000010: 6561 722c 6374 675f 7061 7468 293a 0d0a  ear,ctg_path):..
+00000020: 0d0a 2020 2020 696d 706f 7274 206f 730d  ..    import os.
+00000030: 0a20 2020 2066 726f 6d20 7061 7468 6c69  .    from pathli
+00000040: 6220 696d 706f 7274 2050 6174 680d 0a20  b import Path.. 
+00000050: 2020 200d 0a20 2020 2066 726f 6d20 4354     ..    from CT
+00000060: 475f 5574 696c 732e 4354 475f 4675 6e63  G_Utils.CTG_Func
+00000070: 2e43 5447 5f65 6666 6563 7469 6620 696d  .CTG_effectif im
+00000080: 706f 7274 2063 6f72 7265 6374 696f 6e5f  port correction_
+00000090: 6566 6665 6374 6966 0d0a 2020 2020 6672  effectif..    fr
+000000a0: 6f6d 2043 5447 5f55 7469 6c73 2e43 5447  om CTG_Utils.CTG
+000000b0: 5f46 756e 632e 4354 475f 6566 6665 6374  _Func.CTG_effect
+000000c0: 6966 2069 6d70 6f72 7420 7265 6164 5f65  if import read_e
+000000d0: 6666 6563 7469 665f 636f 7272 6563 7465  ffectif_correcte
+000000e0: 640d 0a20 2020 200d 0a20 2020 2069 6d70  d..    ..    imp
+000000f0: 6f72 7420 7061 6e64 6173 2061 7320 7064  ort pandas as pd
+00000100: 0d0a 2020 2020 0d0a 2020 2020 0d0a 2020  ..    ..    ..  
+00000110: 2020 7061 7468 5f64 6972 5f6c 6973 7420    path_dir_list 
+00000120: 3d20 5b63 7467 5f70 6174 6820 2f20 5061  = [ctg_path / Pa
+00000130: 7468 2873 7472 2879 6561 7229 2920 2f20  th(str(year)) / 
+00000140: 5061 7468 2827 534f 5254 4945 5320 4455  Path('SORTIES DU
+00000150: 2053 414d 4544 4927 2920 2f20 5061 7468   SAMEDI') / Path
+00000160: 2827 4558 4345 4c27 292c 0d0a 2020 2020  ('EXCEL'),..    
+00000170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000180: 2063 7467 5f70 6174 6820 2f20 5061 7468   ctg_path / Path
+00000190: 2873 7472 2879 6561 7229 2920 2f20 5061  (str(year)) / Pa
+000001a0: 7468 2827 534f 5254 4945 5320 4455 2044  th('SORTIES DU D
+000001b0: 494d 414e 4348 4527 2920 2f20 5061 7468  IMANCHE') / Path
+000001c0: 2827 4558 4345 4c27 292c 0d0a 2020 2020  ('EXCEL'),..    
+000001d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000001e0: 2063 7467 5f70 6174 6820 2f20 5061 7468   ctg_path / Path
+000001f0: 2873 7472 2879 6561 7229 2920 2f20 5061  (str(year)) / Pa
+00000200: 7468 2827 534f 5254 4945 5320 4455 204a  th('SORTIES DU J
+00000210: 4555 4449 2729 202f 2050 6174 6828 2745  EUDI') / Path('E
+00000220: 5843 454c 2729 2c0d 0a20 2020 2020 2020  XCEL'),..       
+00000230: 2020 2020 2020 2020 2020 2020 2020 6374                ct
+00000240: 675f 7061 7468 202f 2050 6174 6828 7374  g_path / Path(st
+00000250: 7228 7965 6172 2929 202f 2050 6174 6828  r(year)) / Path(
+00000260: 2753 4f52 5449 4553 2048 4956 4552 2729  'SORTIES HIVER')
+00000270: 202f 2050 6174 6828 2745 5843 454c 2729   / Path('EXCEL')
+00000280: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00000290: 2020 2020 2020 2020 6374 675f 7061 7468          ctg_path
+000002a0: 202f 2050 6174 6828 7374 7228 7965 6172   / Path(str(year
+000002b0: 2929 202f 2050 6174 6828 2753 4f52 5449  )) / Path('SORTI
+000002c0: 4553 2044 5520 4c55 4e44 4927 292f 2050  ES DU LUNDI')/ P
+000002d0: 6174 6828 2745 5843 454c 2729 2c0d 0a20  ath('EXCEL'),.. 
+000002e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000002f0: 2020 2020 6374 675f 7061 7468 202f 2050      ctg_path / P
+00000300: 6174 6828 7374 7228 7965 6172 2929 202f  ath(str(year)) /
+00000310: 2050 6174 6828 2753 454a 4f55 5227 2920   Path('SEJOUR') 
+00000320: 2f20 5061 7468 2827 4558 4345 4c27 295d  / Path('EXCEL')]
+00000330: 0d0a 0d0a 2020 2020 6c69 7374 5f64 6620  ....    list_df 
+00000340: 3d20 5b5d 0d0a 2020 2020 666f 7220 7061  = []..    for pa
+00000350: 7468 5f64 6972 2069 6e20 7061 7468 5f64  th_dir in path_d
+00000360: 6972 5f6c 6973 743a 0d0a 2020 2020 2020  ir_list:..      
+00000370: 2020 6966 206f 732e 7061 7468 2e69 7364    if os.path.isd
+00000380: 6972 2870 6174 685f 6469 7229 3a0d 0a20  ir(path_dir):.. 
+00000390: 2020 2020 2020 2020 2020 2066 696c 6573             files
+000003a0: 203d 205b 7820 666f 7220 7820 696e 206f   = [x for x in o
+000003b0: 732e 6c69 7374 6469 7228 7061 7468 5f64  s.listdir(path_d
+000003c0: 6972 2920 6966 2078 2e65 6e64 7377 6974  ir) if x.endswit
+000003d0: 6828 272e 786c 7378 2729 2061 6e64 2022  h('.xlsx') and "
+000003e0: 7e24 2220 6e6f 7420 696e 2078 5d20 0d0a  ~$" not in x] ..
+000003f0: 2020 2020 2020 2020 2020 2020 6c69 7374              list
+00000400: 5f64 662e 6578 7465 6e64 285b 7064 2e72  _df.extend([pd.r
+00000410: 6561 645f 6578 6365 6c28 7061 7468 5f64  ead_excel(path_d
+00000420: 6972 202f 2050 6174 6828 6669 6c65 292c  ir / Path(file),
+00000430: 2065 6e67 696e 653d 276f 7065 6e70 7978   engine='openpyx
+00000440: 6c27 2920 666f 7220 6669 6c65 2069 6e20  l') for file in 
+00000450: 6669 6c65 735d 290d 0a20 2020 200d 0a20  files])..    .. 
+00000460: 2020 2064 665f 746f 7461 6c20 3d20 7064     df_total = pd
+00000470: 2e63 6f6e 6361 7428 6c69 7374 5f64 662c  .concat(list_df,
+00000480: 2069 676e 6f72 655f 696e 6465 783d 5472   ignore_index=Tr
+00000490: 7565 290d 0a20 2020 200d 0a20 2020 206c  ue)..    ..    l
+000004a0: 6973 745f 6e6f 6e5f 6c69 6365 6e63 6965  ist_non_licencie
+000004b0: 2c20 6469 635f 636f 7272 6563 7469 6f6e  , dic_correction
+000004c0: 5f6c 6963 656e 6365 2c20 6469 635f 7061  _licence, dic_pa
+000004d0: 7274 5f63 6c75 6220 3d20 636f 7272 6563  rt_club = correc
+000004e0: 7469 6f6e 5f65 6666 6563 7469 6628 7965  tion_effectif(ye
+000004f0: 6172 2c63 7467 5f70 6174 6829 0d0a 2020  ar,ctg_path)..  
+00000500: 2020 6466 5f65 6666 6563 7469 6620 3d20    df_effectif = 
+00000510: 7265 6164 5f65 6666 6563 7469 665f 636f  read_effectif_co
+00000520: 7272 6563 7465 6428 6469 635f 636f 7272  rrected(dic_corr
+00000530: 6563 7469 6f6e 5f6c 6963 656e 6365 2c0d  ection_licence,.
+00000540: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000550: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000560: 2020 2020 2020 2020 2020 206c 6973 745f             list_
+00000570: 6e6f 6e5f 6c69 6365 6e63 6965 2c0d 0a20  non_licencie,.. 
+00000580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000005a0: 2020 2020 2020 2020 2064 6963 5f70 6172           dic_par
+000005b0: 745f 636c 7562 2c0d 0a20 2020 2020 2020  t_club,..       
+000005c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000005d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000005e0: 2020 2063 7467 5f70 6174 6829 0d0a 2020     ctg_path)..  
+000005f0: 2020 0d0a 2020 2020 6466 5f74 6f74 616c    ..    df_total
+00000600: 5b27 5072 6174 6971 7565 2056 4145 275d  ['Pratique VAE']
+00000610: 2e66 696c 6c6e 6128 274e 6f6e 272c 696e  .fillna('Non',in
+00000620: 706c 6163 653d 5472 7565 290d 0a20 2020  place=True)..   
+00000630: 200d 0a20 2020 2023 206e 6f6d 6272 6520   ..    # nombre 
+00000640: 6d6f 7965 6e20 6465 2070 6172 7469 6369  moyen de partici
+00000650: 7061 6e74 2070 6172 2061 6374 6976 6974  pant par activit
+00000660: c3a9 0d0a 2020 2020 666f 7220 7820 696e  ....    for x in
+00000670: 2064 665f 746f 7461 6c2e 6772 6f75 7062   df_total.groupb
+00000680: 7928 5b27 5479 7065 275d 293a 0d0a 2020  y(['Type']):..  
+00000690: 2020 2020 2020 7072 696e 7428 785b 305d        print(x[0]
+000006a0: 2c6c 656e 2878 5b31 5d29 2c6c 656e 2873  ,len(x[1]),len(s
+000006b0: 6574 2878 5b31 5d5b 2773 656a 6f75 7227  et(x[1]['sejour'
+000006c0: 5d29 292c 6c65 6e28 785b 315d 292f 6c65  ])),len(x[1])/le
+000006d0: 6e28 7365 7428 785b 315d 5b27 7365 6a6f  n(set(x[1]['sejo
+000006e0: 7572 275d 2929 290d 0a20 2020 200d 0a20  ur'])))..    .. 
+000006f0: 2020 2066 696c 6520 3d20 6374 675f 7061     file = ctg_pa
+00000700: 7468 202f 2050 6174 6828 7374 7228 7965  th / Path(str(ye
+00000710: 6172 2929 202f 2050 6174 6828 2753 5441  ar)) / Path('STA
+00000720: 5449 5354 4951 5545 5327 2920 2f20 5061  TISTIQUES') / Pa
+00000730: 7468 2827 7379 6e74 6865 7365 2e78 6c73  th('synthese.xls
+00000740: 7827 290d 0a20 2020 2064 665f 746f 7461  x')..    df_tota
+00000750: 6c2e 746f 5f65 7863 656c 2866 696c 6529  l.to_excel(file)
+00000760: 0d0a 0d0a 6465 6620 706c 6f74 5f70 6965  ....def plot_pie
+00000770: 5f73 796e 7468 6573 6528 7965 6172 2c63  _synthese(year,c
+00000780: 7467 5f70 6174 6829 3a0d 0a20 2020 200d  tg_path):..    .
+00000790: 0a20 2020 2066 726f 6d20 7061 7468 6c69  .    from pathli
+000007a0: 6220 696d 706f 7274 2050 6174 680d 0a20  b import Path.. 
+000007b0: 2020 200d 0a20 2020 2069 6d70 6f72 7420     ..    import 
+000007c0: 6e75 6d70 7920 6173 206e 700d 0a20 2020  numpy as np..   
+000007d0: 2069 6d70 6f72 7420 6d61 7470 6c6f 746c   import matplotl
+000007e0: 6962 2e70 7970 6c6f 7420 6173 2070 6c74  ib.pyplot as plt
+000007f0: 0d0a 2020 2020 696d 706f 7274 2070 616e  ..    import pan
+00000800: 6461 7320 6173 2070 640d 0a20 2020 200d  das as pd..    .
+00000810: 0a20 2020 2064 6566 2066 756e 6328 7063  .    def func(pc
+00000820: 742c 2061 6c6c 7661 6c75 6573 293a 0d0a  t, allvalues):..
+00000830: 2020 2020 2020 2020 6162 736f 6c75 7465          absolute
+00000840: 203d 2072 6f75 6e64 2870 6374 202f 2031   = round(pct / 1
+00000850: 3030 2e2a 6e70 2e73 756d 2861 6c6c 7661  00.*np.sum(allva
+00000860: 6c75 6573 292c 3029 0d0a 2020 2020 2020  lues),0)..      
+00000870: 2020 2372 6574 7572 6e20 227b 3a2e 3166    #return "{:.1f
+00000880: 7d25 5c6e 287b 3a64 7d29 222e 666f 726d  }%\n({:d})".form
+00000890: 6174 2870 6374 2c20 6162 736f 6c75 7465  at(pct, absolute
+000008a0: 290d 0a20 2020 2020 2020 2072 6574 7572  )..        retur
+000008b0: 6e20 2066 227b 696e 7428 726f 756e 6428  n  f"{int(round(
+000008c0: 6162 736f 6c75 7465 2c31 2929 7d5c 6e7b  absolute,1))}\n{
+000008d0: 726f 756e 6428 7063 742c 3129 7d20 2522  round(pct,1)} %"
+000008e0: 0d0a 2020 2020 2020 2020 0d0a 2020 2020  ..        ..    
+000008f0: 6669 6c65 5f69 6e20 3d20 6374 675f 7061  file_in = ctg_pa
+00000900: 7468 202f 2050 6174 6828 7374 7228 7965  th / Path(str(ye
+00000910: 6172 2929 202f 2050 6174 6828 2753 5441  ar)) / Path('STA
+00000920: 5449 5354 4951 5545 5327 2920 2f20 5061  TISTIQUES') / Pa
+00000930: 7468 2827 7379 6e74 6865 7365 2e78 6c73  th('synthese.xls
+00000940: 7827 290d 0a20 2020 2064 665f 746f 7461  x')..    df_tota
+00000950: 6c20 3d20 7064 2e72 6561 645f 6578 6365  l = pd.read_exce
+00000960: 6c28 6669 6c65 5f69 6e29 0d0a 2020 2020  l(file_in)..    
+00000970: 6466 5f74 6f74 616c 203d 2064 665f 746f  df_total = df_to
+00000980: 7461 6c2e 6472 6f70 6e61 2873 7562 7365  tal.dropna(subse
+00000990: 743d 5b27 5479 7065 275d 2920 0d0a 2020  t=['Type']) ..  
+000009a0: 2020 6466 5f74 6f74 616c 203d 2064 665f    df_total = df_
+000009b0: 746f 7461 6c2e 6472 6f70 6e61 2873 7562  total.dropna(sub
+000009c0: 7365 743d 5b27 4e6f 6d27 5d29 0d0a 0d0a  set=['Nom'])....
+000009d0: 2020 2020 6461 6767 203d 2064 665f 746f      dagg = df_to
+000009e0: 7461 6c2e 6772 6f75 7062 7928 2754 7970  tal.groupby('Typ
+000009f0: 6527 295b 276e 6272 5f6a 6f75 7273 275d  e')['nbr_jours']
+00000a00: 2e61 6767 2873 756d 290d 0a0d 0a20 2020  .agg(sum)....   
+00000a10: 200d 0a20 2020 200d 0a20 2020 2065 7870   ..    ..    exp
+00000a20: 6c6f 6465 5f64 6963 203d 207b 2752 414e  lode_dic = {'RAN
+00000a30: 444f 4e4e 4545 273a 302e 312c 0d0a 2020  DONNEE':0.1,..  
+00000a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000a50: 2027 5345 4a4f 5552 273a 302e 302c 200d   'SEJOUR':0.0, .
+00000a60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000a70: 2020 2020 2753 4f52 5449 4553 2044 5520      'SORTIES DU 
+00000a80: 4449 4d41 4e43 4845 273a 302e 322c 0d0a  DIMANCHE':0.2,..
+00000a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000aa0: 2020 2027 534f 5254 4945 5320 4455 204a     'SORTIES DU J
+00000ab0: 4555 4449 273a 302e 322c 0d0a 2020 2020  EUDI':0.2,..    
+00000ac0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+00000ad0: 534f 5254 4945 5320 4455 204c 554e 4449  SORTIES DU LUNDI
+00000ae0: 273a 302e 322c 200d 0a20 2020 2020 2020  ':0.2, ..       
+00000af0: 2020 2020 2020 2020 2020 2020 2753 4f52              'SOR
+00000b00: 5449 4553 2044 5520 5341 4d45 4449 273a  TIES DU SAMEDI':
+00000b10: 302e 322c 0d0a 2020 2020 2020 2020 2020  0.2,..          
+00000b20: 2020 2020 2020 2020 2027 534f 5254 4945           'SORTIE
+00000b30: 5320 4849 5645 5227 3a30 2e32 7d0d 0a0d  S HIVER':0.2}...
+00000b40: 0a20 2020 2064 6174 6120 3d20 5b5d 0d0a  .    data = []..
+00000b50: 2020 2020 736f 7274 6965 7320 3d20 5b5d      sorties = []
+00000b60: 0d0a 2020 2020 666f 7220 7479 7065 5f73  ..    for type_s
+00000b70: 656a 6f75 722c 206e 6272 2069 6e20 7a69  ejour, nbr in zi
+00000b80: 7028 6461 6767 2e69 6e64 6578 2c64 6167  p(dagg.index,dag
+00000b90: 672e 746f 6c69 7374 2829 293a 0d0a 2020  g.tolist()):..  
+00000ba0: 2020 2020 2020 6966 206e 6272 213d 303a        if nbr!=0:
+00000bb0: 0d0a 2020 2020 2020 2020 2020 2020 6461  ..            da
+00000bc0: 7461 2e61 7070 656e 6428 6e62 7229 0d0a  ta.append(nbr)..
+00000bd0: 2020 2020 2020 2020 2020 2020 736f 7274              sort
+00000be0: 6965 732e 6170 7065 6e64 2874 7970 655f  ies.append(type_
+00000bf0: 7365 6a6f 7572 290d 0a0d 0a20 2020 2065  sejour)....    e
+00000c00: 7870 6c6f 6465 203d 205b 6578 706c 6f64  xplode = [explod
+00000c10: 655f 6469 635b 7479 705d 2066 6f72 2074  e_dic[typ] for t
+00000c20: 7970 2069 6e20 736f 7274 6965 735d 0d0a  yp in sorties]..
+00000c30: 2020 2020 0d0a 2020 2020 0d0a 2020 2020      ..    ..    
+00000c40: 2320 4372 6561 7469 6e67 2070 6c6f 740d  # Creating plot.
+00000c50: 0a20 2020 2066 6967 203d 2070 6c74 2e66  .    fig = plt.f
+00000c60: 6967 7572 6528 6669 6773 697a 6520 3d28  igure(figsize =(
+00000c70: 3130 2c20 3729 290d 0a20 2020 205f 2c20  10, 7))..    _, 
+00000c80: 5f2c 2061 7574 6f74 6578 7473 203d 2070  _, autotexts = p
+00000c90: 6c74 2e70 6965 2864 6174 612c 0d0a 2020  lt.pie(data,..  
+00000ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000cb0: 2020 2020 2020 2020 2020 2020 6c61 6265              labe
+00000cc0: 6c73 203d 2073 6f72 7469 6573 2c0d 0a20  ls = sorties,.. 
+00000cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000ce0: 2020 2020 2020 2020 2020 2020 2061 7574               aut
+00000cf0: 6f70 6374 203d 206c 616d 6264 6120 7063  opct = lambda pc
+00000d00: 743a 2066 756e 6328 7063 742c 2064 6174  t: func(pct, dat
+00000d10: 6129 2c0d 0a20 2020 2020 2020 2020 2020  a),..           
+00000d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000d30: 2020 2065 7870 6c6f 6465 203d 2065 7870     explode = exp
+00000d40: 6c6f 6465 2c0d 0a20 2020 2020 2020 2020  lode,..         
+00000d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000d60: 2020 2020 2074 6578 7470 726f 7073 3d7b       textprops={
+00000d70: 2766 6f6e 7473 697a 6527 3a20 3138 7d29  'fontsize': 18})
+00000d80: 0d0a 2020 2020 706c 742e 7469 746c 6528  ..    plt.title(
+00000d90: 7374 7228 7965 6172 292c 2070 6164 3d35  str(year), pad=5
+00000da0: 302c 2066 6f6e 7473 697a 653d 3230 290d  0, fontsize=20).
+00000db0: 0a20 2020 200d 0a20 2020 205f 203d 2070  .    ..    _ = p
+00000dc0: 6c74 2e73 6574 7028 6175 746f 7465 7874  lt.setp(autotext
+00000dd0: 732c 202a 2a7b 2763 6f6c 6f72 273a 276b  s, **{'color':'k
+00000de0: 272c 2027 7765 6967 6874 273a 2762 6f6c  ', 'weight':'bol
+00000df0: 6427 2c20 2766 6f6e 7473 697a 6527 3a31  d', 'fontsize':1
+00000e00: 347d 290d 0a20 2020 200d 0a20 2020 2070  4})..    ..    p
+00000e10: 6c74 2e74 6967 6874 5f6c 6179 6f75 7428  lt.tight_layout(
+00000e20: 290d 0a20 2020 2070 6c74 2e73 686f 7728  )..    plt.show(
+00000e30: 290d 0a20 2020 200d 0a20 2020 2066 6967  )..    ..    fig
+00000e40: 5f66 696c 6520 3d20 2753 4f52 5449 4553  _file = 'SORTIES
+00000e50: 5f50 4945 2e70 6e67 270d 0a20 2020 2070  _PIE.png'..    p
+00000e60: 6c74 2e73 6176 6566 6967 2863 7467 5f70  lt.savefig(ctg_p
+00000e70: 6174 6820 2f20 5061 7468 2873 7472 2879  ath / Path(str(y
+00000e80: 6561 7229 2920 2f20 5061 7468 2827 5354  ear)) / Path('ST
+00000e90: 4154 4953 5449 5155 4553 2729 202f 2050  ATISTIQUES') / P
+00000ea0: 6174 6828 6669 675f 6669 6c65 292c 6262  ath(fig_file),bb
+00000eb0: 6f78 5f69 6e63 6865 733d 2774 6967 6874  ox_inches='tight
+00000ec0: 2729 090d 0a0d 0a20 2020 2072 6574 7572  ').....    retur
+00000ed0: 6e20 090d 0a09 0d0a 0d0a 6465 6620 7379  n ........def sy
+00000ee0: 6e74 6865 7365 5f61 6468 6572 656e 7428  nthese_adherent(
+00000ef0: 7965 6172 2c63 7467 5f70 6174 6829 3a0d  year,ctg_path):.
+00000f00: 0a0d 0a20 2020 2066 726f 6d20 7061 7468  ...    from path
+00000f10: 6c69 6220 696d 706f 7274 2050 6174 680d  lib import Path.
+00000f20: 0a20 2020 200d 0a20 2020 2069 6d70 6f72  .    ..    impor
+00000f30: 7420 7061 6e64 6173 2061 7320 7064 0d0a  t pandas as pd..
+00000f40: 2020 2020 0d0a 2020 2020 6672 6f6d 2043      ..    from C
+00000f50: 5447 5f55 7469 6c73 2e43 5447 5f46 756e  TG_Utils.CTG_Fun
+00000f60: 632e 4354 4743 6c61 7373 6573 2069 6d70  c.CTGClasses imp
+00000f70: 6f72 7420 4566 6665 6374 6966 4374 670d  ort EffectifCtg.
+00000f80: 0a20 2020 200d 0a20 2020 2066 696c 655f  .    ..    file_
+00000f90: 696e 203d 2063 7467 5f70 6174 6820 2f20  in = ctg_path / 
+00000fa0: 5061 7468 2873 7472 2879 6561 7229 2920  Path(str(year)) 
+00000fb0: 2f20 5061 7468 2827 5354 4154 4953 5449  / Path('STATISTI
+00000fc0: 5155 4553 2729 202f 2050 6174 6828 2773  QUES') / Path('s
+00000fd0: 796e 7468 6573 652e 786c 7378 2729 0d0a  ynthese.xlsx')..
+00000fe0: 2020 2020 6466 5f74 6f74 616c 203d 2070      df_total = p
+00000ff0: 642e 7265 6164 5f65 7863 656c 2866 696c  d.read_excel(fil
+00001000: 655f 696e 290d 0a20 2020 2064 665f 746f  e_in)..    df_to
+00001010: 7461 6c20 3d20 6466 5f74 6f74 616c 2e64  tal = df_total.d
+00001020: 726f 706e 6128 7375 6273 6574 3d5b 2754  ropna(subset=['T
+00001030: 7970 6527 5d29 0d0a 2020 2020 6e62 7265  ype'])..    nbre
+00001040: 203d 207b 7d0d 0a20 2020 200d 0a20 2020   = {}..    ..   
+00001050: 2066 6f72 2069 645f 6c69 6365 6e63 652c   for id_licence,
+00001060: 2064 6720 696e 2064 665f 746f 7461 6c2e   dg in df_total.
+00001070: 6772 6f75 7062 7928 274e c2b0 204c 6963  groupby('N.. Lic
+00001080: 656e 6369 c3a9 2729 3a0d 0a20 2020 2020  enci..'):..     
+00001090: 2020 200d 0a20 2020 2020 2020 206e 6272     ..        nbr
+000010a0: 655b 6964 5f6c 6963 656e 6365 5d3d 5b64  e[id_licence]=[d
+000010b0: 675b 274e 6f6d 275d 2e75 6e69 7175 6528  g['Nom'].unique(
+000010c0: 295b 305d 2c64 675b 2750 72c3 a96e 6f6d  )[0],dg['Pr..nom
+000010d0: 275d 2e75 6e69 7175 6528 295b 305d 5d0d  '].unique()[0]].
+000010e0: 0a20 2020 200d 0a20 2020 2020 2020 206e  .    ..        n
+000010f0: 625f 736f 7274 6965 5f64 696d 616e 6368  b_sortie_dimanch
+00001100: 6520 3d20 6c65 6e28 6467 2e71 7565 7279  e = len(dg.query
+00001110: 2822 5479 7065 2e73 7472 2e63 6f6e 7461  ("Type.str.conta
+00001120: 696e 7328 2753 4f52 5449 4553 2044 5520  ins('SORTIES DU 
+00001130: 4449 4d41 4e43 4845 2729 2229 290d 0a20  DIMANCHE')")).. 
+00001140: 2020 2020 2020 206e 6272 655b 6964 5f6c         nbre[id_l
+00001150: 6963 656e 6365 5d20 3d20 6e62 7265 5b69  icence] = nbre[i
+00001160: 645f 6c69 6365 6e63 655d 202b 205b 6e62  d_licence] + [nb
+00001170: 5f73 6f72 7469 655f 6469 6d61 6e63 6865  _sortie_dimanche
+00001180: 5d0d 0a20 2020 200d 0a20 2020 2020 2020  ]..    ..       
+00001190: 206e 625f 736f 7274 6965 5f73 616d 6564   nb_sortie_samed
+000011a0: 6920 3d20 6c65 6e28 6467 2e71 7565 7279  i = len(dg.query
+000011b0: 2822 5479 7065 2e73 7472 2e63 6f6e 7461  ("Type.str.conta
+000011c0: 696e 7328 2753 4f52 5449 4553 2044 5520  ins('SORTIES DU 
+000011d0: 5341 4d45 4449 2729 2229 290d 0a20 2020  SAMEDI')"))..   
+000011e0: 2020 2020 206e 6272 655b 6964 5f6c 6963       nbre[id_lic
+000011f0: 656e 6365 5d20 3d20 6e62 7265 5b69 645f  ence] = nbre[id_
+00001200: 6c69 6365 6e63 655d 202b 205b 6e62 5f73  licence] + [nb_s
+00001210: 6f72 7469 655f 7361 6d65 6469 5d0d 0a20  ortie_samedi].. 
+00001220: 2020 200d 0a20 2020 2020 2020 206e 625f     ..        nb_
+00001230: 736f 7274 6965 5f6a 6575 6469 203d 206c  sortie_jeudi = l
+00001240: 656e 2864 672e 7175 6572 7928 2254 7970  en(dg.query("Typ
+00001250: 652e 7374 722e 636f 6e74 6169 6e73 2827  e.str.contains('
+00001260: 534f 5254 4945 5320 4455 204a 4555 4449  SORTIES DU JEUDI
+00001270: 2729 2229 290d 0a20 2020 2020 2020 206e  ')"))..        n
+00001280: 6272 655b 6964 5f6c 6963 656e 6365 5d20  bre[id_licence] 
+00001290: 3d20 6e62 7265 5b69 645f 6c69 6365 6e63  = nbre[id_licenc
+000012a0: 655d 202b 205b 6e62 5f73 6f72 7469 655f  e] + [nb_sortie_
+000012b0: 6a65 7564 695d 0d0a 2020 2020 0d0a 2020  jeudi]..    ..  
+000012c0: 2020 2020 2020 6e62 5f72 616e 646f 203d        nb_rando =
+000012d0: 206c 656e 2864 672e 7175 6572 7928 2254   len(dg.query("T
+000012e0: 7970 652e 7374 722e 636f 6e74 6169 6e73  ype.str.contains
+000012f0: 2827 5241 4e44 4f4e 4e45 4527 2922 2929  ('RANDONNEE')"))
+00001300: 0d0a 2020 2020 2020 2020 6e62 7265 5b69  ..        nbre[i
+00001310: 645f 6c69 6365 6e63 655d 203d 206e 6272  d_licence] = nbr
+00001320: 655b 6964 5f6c 6963 656e 6365 5d20 2b20  e[id_licence] + 
+00001330: 5b6e 625f 7261 6e64 6f5d 0d0a 2020 2020  [nb_rando]..    
+00001340: 0d0a 2020 2020 2020 2020 6e62 5f73 656a  ..        nb_sej
+00001350: 6f75 725f 6a6f 7572 7320 3d20 7375 6d28  our_jours = sum(
+00001360: 6467 2e71 7565 7279 2822 5479 7065 2e73  dg.query("Type.s
+00001370: 7472 2e63 6f6e 7461 696e 7328 2753 454a  tr.contains('SEJ
+00001380: 4f55 5227 2922 295b 276e 6272 5f6a 6f75  OUR')")['nbr_jou
+00001390: 7273 275d 2e74 6f6c 6973 7428 2929 0d0a  rs'].tolist())..
+000013a0: 2020 2020 2020 2020 6e62 7265 5b69 645f          nbre[id_
+000013b0: 6c69 6365 6e63 655d 203d 206e 6272 655b  licence] = nbre[
+000013c0: 6964 5f6c 6963 656e 6365 5d20 2b20 5b6e  id_licence] + [n
+000013d0: 625f 7365 6a6f 7572 5f6a 6f75 7273 5d0d  b_sejour_jours].
+000013e0: 0a0d 0a20 2020 2020 2020 206e 625f 7365  ...        nb_se
+000013f0: 6a6f 7572 203d 206c 656e 2864 672e 7175  jour = len(dg.qu
+00001400: 6572 7928 2254 7970 652e 7374 722e 636f  ery("Type.str.co
+00001410: 6e74 6169 6e73 2827 5345 4a4f 5552 2729  ntains('SEJOUR')
+00001420: 2229 5b27 7365 6a6f 7572 275d 2e75 6e69  ")['sejour'].uni
+00001430: 7175 6528 2929 0d0a 2020 2020 2020 2020  que())..        
+00001440: 6e62 7265 5b69 645f 6c69 6365 6e63 655d  nbre[id_licence]
+00001450: 203d 206e 6272 655b 6964 5f6c 6963 656e   = nbre[id_licen
+00001460: 6365 5d20 2b20 5b6e 625f 7365 6a6f 7572  ce] + [nb_sejour
+00001470: 5d0d 0a20 2020 200d 0a20 2020 2020 2020  ]..    ..       
+00001480: 206e 625f 6869 7665 7220 3d20 6c65 6e28   nb_hiver = len(
+00001490: 6467 2e71 7565 7279 2822 5479 7065 2e73  dg.query("Type.s
+000014a0: 7472 2e63 6f6e 7461 696e 7328 2753 4f52  tr.contains('SOR
+000014b0: 5449 4553 2048 4956 4552 2729 2229 290d  TIES HIVER')")).
+000014c0: 0a20 2020 2020 2020 206e 6272 655b 6964  .        nbre[id
+000014d0: 5f6c 6963 656e 6365 5d20 3d20 6e62 7265  _licence] = nbre
+000014e0: 5b69 645f 6c69 6365 6e63 655d 202b 205b  [id_licence] + [
+000014f0: 6e62 5f68 6976 6572 5d0d 0a20 2020 200d  nb_hiver]..    .
+00001500: 0a20 2020 2020 2020 206e 6272 5f65 7665  .        nbr_eve
+00001510: 6e65 6d65 6e74 7320 3d20 5b6e 625f 736f  nements = [nb_so
+00001520: 7274 6965 5f64 696d 616e 6368 6520 2b0d  rtie_dimanche +.
+00001530: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001540: 2020 2020 2020 2020 2020 206e 625f 736f             nb_so
+00001550: 7274 6965 5f73 616d 6564 6920 2b20 0d0a  rtie_samedi + ..
+00001560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001570: 2020 2020 2020 2020 2020 6e62 5f73 6f72            nb_sor
+00001580: 7469 655f 6a65 7564 6920 2b0d 0a20 2020  tie_jeudi +..   
 00001590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000015a0: 2020 2020 2020 2020 6e62 5f68 6976 6572          nb_hiver
-000015b0: 5d0d 0a20 2020 2020 2020 206e 6272 655b  ]..        nbre[
-000015c0: 6964 5f6c 6963 656e 6365 5d20 3d20 6e62  id_licence] = nb
-000015d0: 7265 5b69 645f 6c69 6365 6e63 655d 202b  re[id_licence] +
-000015e0: 206e 6272 5f65 7665 6e65 6d65 6e74 730d   nbr_evenements.
-000015f0: 0a20 2020 200d 0a20 2020 2064 6720 3d20  .    ..    dg = 
-00001600: 7064 2e44 6174 6146 7261 6d65 2e66 726f  pd.DataFrame.fro
-00001610: 6d5f 6469 6374 286e 6272 6529 2e54 0d0a  m_dict(nbre).T..
-00001620: 2020 2020 6467 2e63 6f6c 756d 6e73 203d      dg.columns =
-00001630: 205b 0d0a 2020 2020 2020 2020 2020 2020   [..            
-00001640: 2020 2020 2027 4e6f 6d27 2c0d 0a20 2020       'Nom',..   
-00001650: 2020 2020 2020 2020 2020 2020 2020 2750                'P
-00001660: 72c3 a96e 6f6d 272c 0d0a 2020 2020 2020  r..nom',..      
-00001670: 2020 2020 2020 2020 2020 2027 534f 5254             'SORT
-00001680: 4945 2044 5520 4449 4d41 4e43 4845 2043  IE DU DIMANCHE C
-00001690: 4c55 4227 2c0d 0a20 2020 2020 2020 2020  LUB',..         
-000016a0: 2020 2020 2020 2020 2753 4f52 5449 4520          'SORTIE 
-000016b0: 4455 2053 414d 4544 4920 434c 5542 272c  DU SAMEDI CLUB',
-000016c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000016d0: 2020 2027 534f 5254 4945 2044 5520 4a45     'SORTIE DU JE
-000016e0: 5544 4920 434c 5542 272c 0d0a 2020 2020  UDI CLUB',..    
-000016f0: 2020 2020 2020 2020 2020 2020 2027 5241               'RA
-00001700: 4e44 4f4e 4e45 4527 2c0d 0a20 2020 2020  NDONNEE',..     
-00001710: 2020 2020 2020 2020 2020 2020 2753 454a              'SEJ
-00001720: 4f55 522d 4a4f 5552 272c 0d0a 2020 2020  OUR-JOUR',..    
-00001730: 2020 2020 2020 2020 2020 2020 2027 4e62               'Nb
-00001740: 725f 5345 4a4f 5552 5327 2c0d 0a20 2020  r_SEJOURS',..   
-00001750: 2020 2020 2020 2020 2020 2020 2020 2753                'S
-00001760: 4f52 5449 4520 4849 5645 5227 2c0d 0a20  ORTIE HIVER',.. 
-00001770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001780: 2754 4f54 414c 272c 0d0a 2020 2020 2020  'TOTAL',..      
-00001790: 2020 2020 2020 2020 2020 205d 0d0a 2020             ]..  
-000017a0: 2020 0d0a 2020 2020 6566 6665 6374 6966    ..    effectif
-000017b0: 203d 2045 6666 6563 7469 6643 7467 2879   = EffectifCtg(y
-000017c0: 6561 722c 6374 675f 7061 7468 290d 0a20  ear,ctg_path).. 
-000017d0: 2020 2064 665f 6566 6665 6374 6966 203d     df_effectif =
-000017e0: 2065 6666 6563 7469 662e 6566 6665 6374   effectif.effect
-000017f0: 6966 0d0a 2020 2020 6466 5f65 6666 6563  if..    df_effec
-00001800: 7469 662e 696e 6465 7820 3d20 6466 5f65  tif.index = df_e
-00001810: 6666 6563 7469 665b 274e c2b0 204c 6963  ffectif['N.. Lic
-00001820: 656e 6369 c3a9 275d 0d0a 2020 2020 6f72  enci..']..    or
-00001830: 7068 616e 203d 2073 6574 2864 665f 6566  phan = set(df_ef
-00001840: 6665 6374 6966 2e69 6e64 6578 2920 2d20  fectif.index) - 
-00001850: 7365 7428 6467 2e69 6e64 6578 290d 0a20  set(dg.index).. 
-00001860: 2020 2064 665f 6f72 7068 616e 203d 2064     df_orphan = d
-00001870: 665f 6566 6665 6374 6966 2e6c 6f63 5b6c  f_effectif.loc[l
-00001880: 6973 7428 6f72 7068 616e 295d 5b5b 274e  ist(orphan)][['N
-00001890: 6f6d 272c 2750 72c3 a96e 6f6d 275d 5d0d  om','Pr..nom']].
-000018a0: 0a20 2020 2064 665f 6f72 7068 616e 5b5b  .    df_orphan[[
-000018b0: 2753 4f52 5449 4520 4455 2044 494d 414e  'SORTIE DU DIMAN
-000018c0: 4348 4520 434c 5542 272c 0d0a 2020 2020  CHE CLUB',..    
-000018d0: 2020 2020 2020 2020 2020 2027 534f 5254             'SORT
-000018e0: 4945 2044 5520 5341 4d45 4449 2043 4c55  IE DU SAMEDI CLU
-000018f0: 4227 2c0d 0a20 2020 2020 2020 2020 2020  B',..           
-00001900: 2020 2020 2753 4f52 5449 4520 4455 204a      'SORTIE DU J
-00001910: 4555 4449 2043 4c55 4227 2c0d 0a20 2020  EUDI CLUB',..   
-00001920: 2020 2020 2020 2020 2020 2020 2752 414e              'RAN
-00001930: 444f 4e4e 4545 272c 0d0a 2020 2020 2020  DONNEE',..      
-00001940: 2020 2020 2020 2020 2027 5345 4a4f 5552           'SEJOUR
-00001950: 2d4a 4f55 5227 2c0d 0a20 2020 2020 2020  -JOUR',..       
-00001960: 2020 2020 2020 2020 274e 6272 5f53 454a          'Nbr_SEJ
-00001970: 4f55 5253 272c 0d0a 2020 2020 2020 2020  OURS',..        
-00001980: 2020 2020 2020 2027 534f 5254 4945 2048         'SORTIE H
-00001990: 4956 4552 272c 0d0a 2020 2020 2020 2020  IVER',..        
-000019a0: 2020 2020 2020 2027 544f 5441 4c27 5d5d         'TOTAL']]
-000019b0: 203d 205b 302c 302c 302c 302c 302c 302c   = [0,0,0,0,0,0,
-000019c0: 302c 305d 0d0a 2020 2020 0d0a 2020 2020  0,0]..    ..    
-000019d0: 6467 203d 2070 642e 636f 6e63 6174 285b  dg = pd.concat([
-000019e0: 6467 2c20 6466 5f6f 7270 6861 6e5d 2c20  dg, df_orphan], 
-000019f0: 6178 6973 3d30 290d 0a20 2020 200d 0a20  axis=0)..    .. 
-00001a00: 2020 2066 696c 655f 6f75 7420 3d20 5061     file_out = Pa
-00001a10: 7468 2847 4c4f 4241 4c5b 2752 4f4f 5427  th(GLOBAL['ROOT'
-00001a20: 5d29 202f 2050 6174 6828 7374 7228 7965  ]) / Path(str(ye
-00001a30: 6172 2929 202f 2050 6174 6828 2753 5441  ar)) / Path('STA
-00001a40: 5449 5354 4951 5545 5327 2920 2f20 5061  TISTIQUES') / Pa
-00001a50: 7468 2827 7379 6e74 6865 7365 5f61 6468  th('synthese_adh
-00001a60: 6572 656e 742e 786c 7378 2729 0d0a 2020  erent.xlsx')..  
-00001a70: 2020 6467 2e74 6f5f 6578 6365 6c28 6669    dg.to_excel(fi
-00001a80: 6c65 5f6f 7574 290d 0a20 2020 200d 0a64  le_out)..    ..d
-00001a90: 6566 2073 796e 7468 6573 655f 7261 6e64  ef synthese_rand
-00001aa0: 6f6e 6e65 6528 7965 6172 2c63 7467 5f70  onnee(year,ctg_p
-00001ab0: 6174 6829 3a0d 0a0d 0a20 2020 200d 0a20  ath):....    .. 
-00001ac0: 2020 2066 726f 6d20 7061 7468 6c69 6220     from pathlib 
-00001ad0: 696d 706f 7274 2050 6174 680d 0a0d 0a20  import Path.... 
-00001ae0: 2020 2069 6d70 6f72 7420 6d61 7470 6c6f     import matplo
-00001af0: 746c 6962 2e70 7970 6c6f 7420 6173 2070  tlib.pyplot as p
-00001b00: 6c74 0d0a 2020 2020 696d 706f 7274 2070  lt..    import p
-00001b10: 616e 6461 7320 6173 2070 640d 0a20 2020  andas as pd..   
-00001b20: 200d 0a20 2020 2069 6d70 6f72 7420 4354   ..    import CT
-00001b30: 475f 5574 696c 7320 6173 2063 7467 0d0a  G_Utils as ctg..
-00001b40: 2020 2020 0d0a 2020 2020 6465 6620 6164      ..    def ad
-00001b50: 646c 6162 656c 7328 782c 792c 6f66 6673  dlabels(x,y,offs
-00001b60: 6574 293a 0d0a 2020 2020 2020 2020 666f  et):..        fo
-00001b70: 7220 6920 696e 2072 616e 6765 286c 656e  r i in range(len
-00001b80: 2878 2929 3a0d 0a20 2020 2020 2020 2020  (x)):..         
-00001b90: 2020 2069 6620 795b 695d 2021 3d20 303a     if y[i] != 0:
-00001ba0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00001bb0: 2020 706c 742e 7465 7874 2878 5b69 5d2c    plt.text(x[i],
-00001bc0: 795b 695d 2b6f 6666 7365 742c 726f 756e  y[i]+offset,roun
-00001bd0: 6428 795b 695d 2c31 292c 7369 7a65 3d31  d(y[i],1),size=1
-00001be0: 3029 0d0a 2020 2020 2020 2020 0d0a 2020  0)..        ..  
-00001bf0: 2020 0d0a 2020 2020 6669 6c65 5f69 6e20    ..    file_in 
-00001c00: 3d20 5061 7468 2863 7467 5f70 6174 6829  = Path(ctg_path)
-00001c10: 202f 2050 6174 6828 7374 7228 7965 6172   / Path(str(year
-00001c20: 2929 202f 2050 6174 6828 2753 5441 5449  )) / Path('STATI
-00001c30: 5354 4951 5545 5327 2920 2f20 5061 7468  STIQUES') / Path
-00001c40: 2827 7379 6e74 6865 7365 2e78 6c73 7827  ('synthese.xlsx'
-00001c50: 290d 0a20 2020 2064 665f 746f 7461 6c20  )..    df_total 
-00001c60: 3d20 7064 2e72 6561 645f 6578 6365 6c28  = pd.read_excel(
-00001c70: 6669 6c65 5f69 6e29 0d0a 2020 2020 6466  file_in)..    df
-00001c80: 5f74 6f74 616c 203d 2064 665f 746f 7461  _total = df_tota
-00001c90: 6c2e 6472 6f70 6e61 2873 7562 7365 743d  l.dropna(subset=
-00001ca0: 5b27 4e6f 6d27 5d29 200d 0a20 2020 2064  ['Nom']) ..    d
-00001cb0: 6720 3d20 6466 5f74 6f74 616c 2e71 7565  g = df_total.que
-00001cc0: 7279 2827 5479 7065 3d3d 2252 414e 444f  ry('Type=="RANDO
-00001cd0: 4e4e 4545 2227 292e 6772 6f75 7062 7928  NNEE"').groupby(
-00001ce0: 2773 656a 6f75 7227 292e 6167 6728 2763  'sejour').agg('c
-00001cf0: 6f75 6e74 2729 5b27 4ec2 b020 4c69 6365  ount')['N.. Lice
-00001d00: 6e63 69c3 a927 5d0d 0a20 2020 200d 0a20  nci..']..    .. 
-00001d10: 2020 2066 6967 203d 2070 6c74 2e66 6967     fig = plt.fig
-00001d20: 7572 6528 6669 6773 697a 653d 2831 302c  ure(figsize=(10,
-00001d30: 3529 290d 0a20 2020 2070 6c74 2e62 6172  5))..    plt.bar
-00001d40: 2872 616e 6765 286c 656e 2864 6729 292c  (range(len(dg)),
-00001d50: 6467 2e74 6f6c 6973 7428 2929 0d0a 2020  dg.tolist())..  
-00001d60: 2020 6164 646c 6162 656c 7328 6c69 7374    addlabels(list
-00001d70: 2872 616e 6765 286c 656e 2864 6729 2929  (range(len(dg)))
-00001d80: 2c64 672e 746f 6c69 7374 2829 2c30 2e32  ,dg.tolist(),0.2
-00001d90: 290d 0a20 2020 2070 6c74 2e78 7469 636b  )..    plt.xtick
-00001da0: 7328 7261 6e67 6528 6c65 6e28 6467 2929  s(range(len(dg))
-00001db0: 2c20 6467 2e69 6e64 6578 2c20 726f 7461  , dg.index, rota
-00001dc0: 7469 6f6e 3d27 7665 7274 6963 616c 2729  tion='vertical')
-00001dd0: 0d0a 2020 2020 706c 742e 7469 636b 5f70  ..    plt.tick_p
-00001de0: 6172 616d 7328 6178 6973 3d27 7827 2c20  arams(axis='x', 
-00001df0: 726f 7461 7469 6f6e 3d39 302c 206c 6162  rotation=90, lab
-00001e00: 656c 7369 7a65 3d31 3029 0d0a 2020 2020  elsize=10)..    
-00001e10: 706c 742e 7469 636b 5f70 6172 616d 7328  plt.tick_params(
-00001e20: 6178 6973 3d27 7927 2c6c 6162 656c 7369  axis='y',labelsi
-00001e30: 7a65 3d31 3029 0d0a 2020 2020 0d0a 2020  ze=10)..    ..  
-00001e40: 2020 5f20 3d20 706c 742e 7469 746c 6528    _ = plt.title(
-00001e50: 6627 2320 7261 6e64 6f73 203a 207b 6c65  f'# randos : {le
-00001e60: 6e28 6467 297d 202c 2023 2070 6172 7469  n(dg)} , # parti
-00001e70: 6369 7061 6e74 7320 3a20 7b73 756d 2864  cipants : {sum(d
-00001e80: 6729 7d27 290d 0a20 2020 2070 6c74 2e74  g)}')..    plt.t
-00001e90: 6967 6874 5f6c 6179 6f75 7428 290d 0a20  ight_layout().. 
-00001ea0: 2020 2070 6c74 2e73 686f 7728 290d 0a20     plt.show().. 
-00001eb0: 2020 200d 0a20 2020 2066 6967 5f66 696c     ..    fig_fil
-00001ec0: 6520 3d20 2753 594e 5448 4553 455f 5241  e = 'SYNTHESE_RA
-00001ed0: 4e44 4f4e 4e45 4553 2e70 6e67 270d 0a20  NDONNEES.png'.. 
-00001ee0: 2020 2070 6c74 2e73 6176 6566 6967 2850     plt.savefig(P
-00001ef0: 6174 6828 474c 4f42 414c 5b27 524f 4f54  ath(GLOBAL['ROOT
-00001f00: 275d 2920 2f20 5061 7468 2873 7472 2879  ']) / Path(str(y
-00001f10: 6561 7229 2920 2f20 5061 7468 2827 5354  ear)) / Path('ST
-00001f20: 4154 4953 5449 5155 4553 2729 202f 2050  ATISTIQUES') / P
-00001f30: 6174 6828 6669 675f 6669 6c65 292c 6262  ath(fig_file),bb
-00001f40: 6f78 5f69 6e63 6865 733d 2774 6967 6874  ox_inches='tight
-00001f50: 2729 0d0a 2020 2020 0d0a 6465 6620 6e62  ')..    ..def nb
-00001f60: 725f 7365 6a6f 7572 735f 6164 6865 7265  r_sejours_adhere
-00001f70: 6e74 2879 6561 722c 2063 7467 5f70 6174  nt(year, ctg_pat
-00001f80: 6829 3a0d 0a0d 0a20 2020 2066 726f 6d20  h):....    from 
-00001f90: 636f 6c6c 6563 7469 6f6e 7320 696d 706f  collections impo
-00001fa0: 7274 2043 6f75 6e74 6572 0d0a 2020 2020  rt Counter..    
-00001fb0: 6672 6f6d 2070 6174 686c 6962 2069 6d70  from pathlib imp
-00001fc0: 6f72 7420 5061 7468 0d0a 2020 2020 0d0a  ort Path..    ..
-00001fd0: 2020 2020 696d 706f 7274 206d 6174 706c      import matpl
-00001fe0: 6f74 6c69 622e 7079 706c 6f74 2061 7320  otlib.pyplot as 
-00001ff0: 706c 740d 0a20 2020 2069 6d70 6f72 7420  plt..    import 
-00002000: 7061 6e64 6173 2061 7320 7064 0d0a 2020  pandas as pd..  
-00002010: 2020 0d0a 2020 2020 706c 742e 7374 796c    ..    plt.styl
-00002020: 652e 7573 6528 2767 6770 6c6f 7427 290d  e.use('ggplot').
-00002030: 0a20 2020 200d 0a20 2020 2023 2066 756e  .    ..    # fun
-00002040: 6374 696f 6e20 746f 2061 6464 2076 616c  ction to add val
-00002050: 7565 206c 6162 656c 730d 0a20 2020 2064  ue labels..    d
-00002060: 6566 2061 6464 6c61 6265 6c73 2878 2c79  ef addlabels(x,y
-00002070: 293a 0d0a 2020 2020 2020 2020 666f 7220  ):..        for 
-00002080: 6920 696e 2072 616e 6765 286c 656e 2878  i in range(len(x
-00002090: 2929 3a0d 0a20 2020 2020 2020 2020 2020  )):..           
-000020a0: 2070 6c74 2e74 6578 7428 785b 695d 2d30   plt.text(x[i]-0
-000020b0: 2e32 2c79 5b69 5d2b 312c 795b 695d 2c73  .2,y[i]+1,y[i],s
-000020c0: 697a 653d 6c61 6265 6c5f 7369 7a65 290d  ize=label_size).
-000020d0: 0a20 2020 206c 6162 656c 5f73 697a 6520  .    label_size 
-000020e0: 3d20 3135 0d0a 2020 2020 6669 6c65 5f69  = 15..    file_i
-000020f0: 6e20 3d20 6374 675f 7061 7468 202f 2050  n = ctg_path / P
-00002100: 6174 6828 7374 7228 7965 6172 2929 202f  ath(str(year)) /
-00002110: 2050 6174 6828 2753 5441 5449 5354 4951   Path('STATISTIQ
-00002120: 5545 5327 2920 2f20 5061 7468 2827 7379  UES') / Path('sy
-00002130: 6e74 6865 7365 5f61 6468 6572 656e 742e  nthese_adherent.
-00002140: 786c 7378 2729 0d0a 2020 2020 6466 5f74  xlsx')..    df_t
-00002150: 6f74 616c 203d 2070 642e 7265 6164 5f65  otal = pd.read_e
-00002160: 7863 656c 2866 696c 655f 696e 290d 0a20  xcel(file_in).. 
-00002170: 2020 200d 0a20 2020 2063 203d 2043 6f75     ..    c = Cou
-00002180: 6e74 6572 2829 0d0a 2020 2020 6320 3d20  nter()..    c = 
-00002190: 436f 756e 7465 7228 6466 5f74 6f74 616c  Counter(df_total
-000021a0: 5b27 4e62 725f 5345 4a4f 5552 5327 5d2e  ['Nbr_SEJOURS'].
-000021b0: 746f 6c69 7374 2829 290d 0a20 2020 2063  tolist())..    c
-000021c0: 203d 2063 2e6d 6f73 745f 636f 6d6d 6f6e   = c.most_common
-000021d0: 2829 0d0a 0d0a 2020 2020 782c 2079 203d  ()....    x, y =
-000021e0: 207a 6970 282a 6329 0d0a 2020 2020 7820   zip(*c)..    x 
-000021f0: 3d20 6c69 7374 2878 290d 0a20 2020 2079  = list(x)..    y
-00002200: 203d 206c 6973 7428 7929 0d0a 2020 2020   = list(y)..    
-00002210: 0d0a 2020 2020 6669 672c 2061 7820 3d20  ..    fig, ax = 
-00002220: 706c 742e 7375 6270 6c6f 7473 2866 6967  plt.subplots(fig
-00002230: 7369 7a65 3d28 352c 3529 290d 0a20 2020  size=(5,5))..   
-00002240: 2070 6c74 2e62 6172 285b 7374 7228 785f   plt.bar([str(x_
-00002250: 7329 2066 6f72 2078 5f73 2069 6e20 785d  s) for x_s in x]
-00002260: 2c79 290d 0a20 2020 2070 6c74 2e78 6c61  ,y)..    plt.xla
-00002270: 6265 6c28 274e 6f6d 6272 6520 6465 2070  bel('Nombre de p
-00002280: 6172 7469 6369 7061 7469 6f6e 20c3 a020  articipation .. 
-00002290: 6465 7320 73c3 a96a 6f75 7273 2729 0d0a  des s..jours')..
-000022a0: 2020 2020 706c 742e 796c 6162 656c 2827      plt.ylabel('
-000022b0: 4e6f 6d62 7265 2064 6520 6c69 6365 6e63  Nombre de licenc
-000022c0: 6965 7273 2729 0d0a 2020 2020 706c 742e  iers')..    plt.
-000022d0: 7469 636b 5f70 6172 616d 7328 6178 6973  tick_params(axis
-000022e0: 3d27 7827 2c20 6c61 6265 6c73 697a 653d  ='x', labelsize=
-000022f0: 6c61 6265 6c5f 7369 7a65 290d 0a20 2020  label_size)..   
-00002300: 2070 6c74 2e74 6963 6b5f 7061 7261 6d73   plt.tick_params
-00002310: 2861 7869 733d 2779 272c 206c 6162 656c  (axis='y', label
-00002320: 7369 7a65 3d6c 6162 656c 5f73 697a 6529  size=label_size)
-00002330: 0d0a 2020 2020 706c 742e 7469 746c 6528  ..    plt.title(
-00002340: 7374 7228 7965 6172 292c 7061 643d 3230  str(year),pad=20
-00002350: 2c20 666f 6e74 7369 7a65 3d32 3029 0d0a  , fontsize=20)..
-00002360: 2020 2020 0d0a 2020 2020 6178 2e73 6574      ..    ax.set
-00002370: 5f78 6c61 6265 6c28 274e 2073 c3a9 6a6f  _xlabel('N s..jo
-00002380: 7572 7327 2c20 666f 6e74 7369 7a65 203d  urs', fontsize =
-00002390: 206c 6162 656c 5f73 697a 6529 0d0a 2020   label_size)..  
-000023a0: 2020 6178 2e73 6574 5f79 6c61 6265 6c28    ax.set_ylabel(
-000023b0: 274e 6f6d 6272 6520 6465 2043 5447 2061  'Nombre de CTG a
-000023c0: 7961 6e74 205c 6e20 7061 7274 6963 6970  yant \n particip
-000023d0: c3a9 20c3 a020 4e20 73c3 a96a 6f75 7273  .. .. N s..jours
-000023e0: 272c 2066 6f6e 7473 697a 6520 3d20 6c61  ', fontsize = la
-000023f0: 6265 6c5f 7369 7a65 290d 0a20 2020 200d  bel_size)..    .
-00002400: 0a20 2020 2078 2e73 6f72 7428 290d 0a20  .    x.sort().. 
-00002410: 2020 2061 6464 6c61 6265 6c73 2878 2c79     addlabels(x,y
-00002420: 290d 0a20 2020 2070 6c74 2e74 6967 6874  )..    plt.tight
-00002430: 5f6c 6179 6f75 7428 290d 0a20 2020 2070  _layout()..    p
-00002440: 6c74 2e73 686f 7728 290d 0a0d 0a20 2020  lt.show()....   
-00002450: 2066 6967 5f66 696c 6520 3d20 2753 454a   fig_file = 'SEJ
-00002460: 4f55 5253 5f53 5441 545f 5041 5254 4943  OURS_STAT_PARTIC
-00002470: 4950 4154 494f 4e2e 706e 6727 0d0a 2020  IPATION.png'..  
-00002480: 2020 706c 742e 7361 7665 6669 6728 5061    plt.savefig(Pa
-00002490: 7468 2847 4c4f 4241 4c5b 2752 4f4f 5427  th(GLOBAL['ROOT'
-000024a0: 5d29 202f 2050 6174 6828 7374 7228 7965  ]) / Path(str(ye
-000024b0: 6172 2929 202f 2050 6174 6828 2753 5441  ar)) / Path('STA
-000024c0: 5449 5354 4951 5545 5327 2920 2f20 5061  TISTIQUES') / Pa
-000024d0: 7468 2866 6967 5f66 696c 6529 2c62 626f  th(fig_file),bbo
-000024e0: 785f 696e 6368 6573 3d27 7469 6768 7427  x_inches='tight'
-000024f0: 290d 0a20 2020 200d 0a64 6566 2072 6561  )..    ..def rea
-00002500: 645f 6d65 6d6f 7279 5f73 6f72 7469 6573  d_memory_sorties
-00002510: 2829 3a0d 0a0d 0a20 2020 2023 2053 7461  ():....    # Sta
-00002520: 6e64 6172 6420 6c69 6272 6172 7920 696d  ndard library im
-00002530: 706f 7274 730d 0a20 2020 2069 6d70 6f72  ports..    impor
-00002540: 7420 6f73 2e70 6174 680d 0a20 2020 2066  t os.path..    f
-00002550: 726f 6d20 7061 7468 6c69 6220 696d 706f  rom pathlib impo
-00002560: 7274 2050 6174 680d 0a0d 0a20 2020 2023  rt Path....    #
-00002570: 2033 7264 2070 6172 7479 2069 6d70 6f72   3rd party impor
-00002580: 7473 0d0a 2020 2020 696d 706f 7274 2079  ts..    import y
-00002590: 616d 6c0d 0a20 2020 200d 0a20 2020 2023  aml..    ..    #
-000025a0: 2052 6561 6473 2074 6865 2064 6566 6175   Reads the defau
-000025b0: 6c74 2050 5663 6861 7261 6374 6572 697a  lt PVcharacteriz
-000025c0: 6174 696f 6e2e 7961 6d6c 2063 6f6e 6669  ation.yaml confi
-000025d0: 6720 6669 6c65 0d0a 2020 2020 7061 7468  g file..    path
-000025e0: 5f63 6f6e 6669 675f 6669 6c65 203d 2050  _config_file = P
-000025f0: 6174 6828 5f5f 6669 6c65 5f5f 292e 7061  ath(__file__).pa
-00002600: 7265 6e74 2e70 6172 656e 7420 2f20 5061  rent.parent / Pa
-00002610: 7468 2827 4354 475f 4675 6e63 2729 202f  th('CTG_Func') /
-00002620: 2050 6174 6828 2743 5447 5f52 6566 4669   Path('CTG_RefFi
-00002630: 6c65 7327 2920 2f20 5061 7468 2827 6d65  les') / Path('me
-00002640: 6d6f 7279 5f73 6f72 7469 6573 2e79 6d6c  mory_sorties.yml
-00002650: 2729 0d0a 2020 2020 7769 7468 206f 7065  ')..    with ope
-00002660: 6e28 7061 7468 5f63 6f6e 6669 675f 6669  n(path_config_fi
-00002670: 6c65 2920 6173 2066 696c 653a 0d0a 2020  le) as file:..  
-00002680: 2020 2020 2020 6d65 6d6f 7279 203d 2079        memory = y
-00002690: 616d 6c2e 7361 6665 5f6c 6f61 6428 6669  aml.safe_load(fi
-000026a0: 6c65 290d 0a20 2020 2020 2020 200d 0a20  le)..        .. 
-000026b0: 2020 2020 2020 0d0a 2020 2020 7265 7475        ..    retu
-000026c0: 726e 206d 656d 6f72 790d 0a20 2020 200d  rn memory..    .
-000026d0: 0a64 6566 2065 766f 6c75 7469 6f6e 5f73  .def evolution_s
-000026e0: 6f72 7469 6573 2874 7970 652c 6374 675f  orties(type,ctg_
-000026f0: 7061 7468 293a 0d0a 0d0a 2020 2020 2320  path):....    # 
-00002700: 5374 616e 6461 7264 206c 6962 7261 7279  Standard library
-00002710: 2069 6d70 6f72 7420 2020 200d 0a20 2020   import    ..   
-00002720: 2069 6d70 6f72 7420 6461 7465 7469 6d65   import datetime
-00002730: 0d0a 2020 2020 6672 6f6d 2070 6174 686c  ..    from pathl
-00002740: 6962 2069 6d70 6f72 7420 5061 7468 0d0a  ib import Path..
-00002750: 2020 2020 6672 6f6d 2063 6f6c 6c65 6374      from collect
-00002760: 696f 6e73 2069 6d70 6f72 7420 6e61 6d65  ions import name
-00002770: 6474 7570 6c65 0d0a 0d0a 2020 2020 2320  dtuple....    # 
-00002780: 5468 6972 6420 7061 7274 7920 6c69 6272  Third party libr
-00002790: 6172 7920 696d 706f 7274 2020 2020 200d  ary import     .
-000027a0: 0a20 2020 2069 6d70 6f72 7420 6d61 7470  .    import matp
-000027b0: 6c6f 746c 6962 2e70 7970 6c6f 7420 6173  lotlib.pyplot as
-000027c0: 2070 6c74 0d0a 2020 2020 696d 706f 7274   plt..    import
-000027d0: 2070 616e 6461 7320 6173 2070 640d 0a20   pandas as pd.. 
-000027e0: 2020 2020 200d 0a20 2020 2023 2049 6e74       ..    # Int
-000027f0: 6572 6e61 6c20 696d 706f 7274 0d0a 2020  ernal import..  
-00002800: 2020 696d 706f 7274 2043 5447 5f55 7469    import CTG_Uti
-00002810: 6c73 2061 7320 6374 670d 0a20 2020 2066  ls as ctg..    f
-00002820: 726f 6d20 4354 475f 5574 696c 732e 4354  rom CTG_Utils.CT
-00002830: 475f 4755 492e 4755 495f 476c 6f62 616c  G_GUI.GUI_Global
-00002840: 7320 696d 706f 7274 2041 4354 4956 4954  s import ACTIVIT
-00002850: 455f 4c49 5354 200d 0a20 2020 200d 0a20  E_LIST ..    .. 
-00002860: 2020 2064 6566 2061 6464 5f6d 656d 6f72     def add_memor
-00002870: 7928 7374 6174 5f64 6963 2c79 6561 7273  y(stat_dic,years
-00002880: 293a 0d0a 2020 2020 2020 2020 6d65 6d6f  ):..        memo
-00002890: 7279 203d 2072 6561 645f 6d65 6d6f 7279  ry = read_memory
-000028a0: 5f73 6f72 7469 6573 2829 0d0a 2020 2020  _sorties()..    
-000028b0: 0d0a 2020 2020 0d0a 2020 2020 2020 2020  ..    ..        
-000028c0: 666f 7220 7965 6172 2c76 2069 6e20 6d65  for year,v in me
-000028d0: 6d6f 7279 5b27 6d65 6d6f 7279 275d 2e69  mory['memory'].i
-000028e0: 7465 6d73 2829 3a0d 0a20 2020 2020 2020  tems():..       
-000028f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002910: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-00002920: 2020 7374 6174 5f64 6963 5b73 7472 2879    stat_dic[str(y
-00002930: 6561 7229 5d20 3d20 7374 6174 7965 6172  ear)] = statyear
-00002940: 2876 5b27 5041 5254 4943 4950 4154 494f  (v['PARTICIPATIO
-00002950: 4e5f 5345 4a4f 5552 5327 5d2c 2020 2020  N_SEJOURS'],    
-00002960: 2020 2020 2020 2020 2020 2020 2320 6e62              # nb
-00002970: 725f 7365 6a6f 7572 730d 0a20 2020 2020  r_sejours..     
-00002980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000029a0: 2020 2020 2020 302c 2020 2020 2020 2020        0,        
+000015a0: 2020 2020 2020 206e 625f 7261 6e64 6f20         nb_rando 
+000015b0: 2b0d 0a20 2020 2020 2020 2020 2020 2020  +..             
+000015c0: 2020 2020 2020 2020 2020 2020 206e 625f               nb_
+000015d0: 7365 6a6f 7572 5f6a 6f75 7273 202b 0d0a  sejour_jours +..
+000015e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000015f0: 2020 2020 2020 2020 2020 6e62 5f68 6976            nb_hiv
+00001600: 6572 5d0d 0a20 2020 2020 2020 206e 6272  er]..        nbr
+00001610: 655b 6964 5f6c 6963 656e 6365 5d20 3d20  e[id_licence] = 
+00001620: 6e62 7265 5b69 645f 6c69 6365 6e63 655d  nbre[id_licence]
+00001630: 202b 206e 6272 5f65 7665 6e65 6d65 6e74   + nbr_evenement
+00001640: 730d 0a20 2020 200d 0a20 2020 2064 6720  s..    ..    dg 
+00001650: 3d20 7064 2e44 6174 6146 7261 6d65 2e66  = pd.DataFrame.f
+00001660: 726f 6d5f 6469 6374 286e 6272 6529 2e54  rom_dict(nbre).T
+00001670: 0d0a 2020 2020 6467 2e63 6f6c 756d 6e73  ..    dg.columns
+00001680: 203d 205b 0d0a 2020 2020 2020 2020 2020   = [..          
+00001690: 2020 2020 2020 2027 4e6f 6d27 2c0d 0a20         'Nom',.. 
+000016a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000016b0: 2750 72c3 a96e 6f6d 272c 0d0a 2020 2020  'Pr..nom',..    
+000016c0: 2020 2020 2020 2020 2020 2020 2027 534f               'SO
+000016d0: 5254 4945 2044 5520 4449 4d41 4e43 4845  RTIE DU DIMANCHE
+000016e0: 2043 4c55 4227 2c0d 0a20 2020 2020 2020   CLUB',..       
+000016f0: 2020 2020 2020 2020 2020 2753 4f52 5449            'SORTI
+00001700: 4520 4455 2053 414d 4544 4920 434c 5542  E DU SAMEDI CLUB
+00001710: 272c 0d0a 2020 2020 2020 2020 2020 2020  ',..            
+00001720: 2020 2020 2027 534f 5254 4945 2044 5520       'SORTIE DU 
+00001730: 4a45 5544 4920 434c 5542 272c 0d0a 2020  JEUDI CLUB',..  
+00001740: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+00001750: 5241 4e44 4f4e 4e45 4527 2c0d 0a20 2020  RANDONNEE',..   
+00001760: 2020 2020 2020 2020 2020 2020 2020 2753                'S
+00001770: 454a 4f55 522d 4a4f 5552 272c 0d0a 2020  EJOUR-JOUR',..  
+00001780: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+00001790: 4e62 725f 5345 4a4f 5552 5327 2c0d 0a20  Nbr_SEJOURS',.. 
+000017a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000017b0: 2753 4f52 5449 4520 4849 5645 5227 2c0d  'SORTIE HIVER',.
+000017c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000017d0: 2020 2754 4f54 414c 272c 0d0a 2020 2020    'TOTAL',..    
+000017e0: 2020 2020 2020 2020 2020 2020 205d 0d0a               ]..
+000017f0: 2020 2020 0d0a 2020 2020 6566 6665 6374      ..    effect
+00001800: 6966 203d 2045 6666 6563 7469 6643 7467  if = EffectifCtg
+00001810: 2879 6561 722c 6374 675f 7061 7468 290d  (year,ctg_path).
+00001820: 0a20 2020 2064 665f 6566 6665 6374 6966  .    df_effectif
+00001830: 203d 2065 6666 6563 7469 662e 6566 6665   = effectif.effe
+00001840: 6374 6966 0d0a 2020 2020 6466 5f65 6666  ctif..    df_eff
+00001850: 6563 7469 662e 696e 6465 7820 3d20 6466  ectif.index = df
+00001860: 5f65 6666 6563 7469 665b 274e c2b0 204c  _effectif['N.. L
+00001870: 6963 656e 6369 c3a9 275d 0d0a 2020 2020  icenci..']..    
+00001880: 6f72 7068 616e 203d 2073 6574 2864 665f  orphan = set(df_
+00001890: 6566 6665 6374 6966 2e69 6e64 6578 2920  effectif.index) 
+000018a0: 2d20 7365 7428 6467 2e69 6e64 6578 290d  - set(dg.index).
+000018b0: 0a20 2020 2064 665f 6f72 7068 616e 203d  .    df_orphan =
+000018c0: 2064 665f 6566 6665 6374 6966 2e6c 6f63   df_effectif.loc
+000018d0: 5b6c 6973 7428 6f72 7068 616e 295d 5b5b  [list(orphan)][[
+000018e0: 274e 6f6d 272c 2750 72c3 a96e 6f6d 275d  'Nom','Pr..nom']
+000018f0: 5d0d 0a20 2020 2064 665f 6f72 7068 616e  ]..    df_orphan
+00001900: 5b5b 2753 4f52 5449 4520 4455 2044 494d  [['SORTIE DU DIM
+00001910: 414e 4348 4520 434c 5542 272c 0d0a 2020  ANCHE CLUB',..  
+00001920: 2020 2020 2020 2020 2020 2020 2027 534f               'SO
+00001930: 5254 4945 2044 5520 5341 4d45 4449 2043  RTIE DU SAMEDI C
+00001940: 4c55 4227 2c0d 0a20 2020 2020 2020 2020  LUB',..         
+00001950: 2020 2020 2020 2753 4f52 5449 4520 4455        'SORTIE DU
+00001960: 204a 4555 4449 2043 4c55 4227 2c0d 0a20   JEUDI CLUB',.. 
+00001970: 2020 2020 2020 2020 2020 2020 2020 2752                'R
+00001980: 414e 444f 4e4e 4545 272c 0d0a 2020 2020  ANDONNEE',..    
+00001990: 2020 2020 2020 2020 2020 2027 5345 4a4f             'SEJO
+000019a0: 5552 2d4a 4f55 5227 2c0d 0a20 2020 2020  UR-JOUR',..     
+000019b0: 2020 2020 2020 2020 2020 274e 6272 5f53            'Nbr_S
+000019c0: 454a 4f55 5253 272c 0d0a 2020 2020 2020  EJOURS',..      
+000019d0: 2020 2020 2020 2020 2027 534f 5254 4945           'SORTIE
+000019e0: 2048 4956 4552 272c 0d0a 2020 2020 2020   HIVER',..      
+000019f0: 2020 2020 2020 2020 2027 544f 5441 4c27           'TOTAL'
+00001a00: 5d5d 203d 205b 302c 302c 302c 302c 302c  ]] = [0,0,0,0,0,
+00001a10: 302c 302c 305d 0d0a 2020 2020 0d0a 2020  0,0,0]..    ..  
+00001a20: 2020 6467 203d 2070 642e 636f 6e63 6174    dg = pd.concat
+00001a30: 285b 6467 2c20 6466 5f6f 7270 6861 6e5d  ([dg, df_orphan]
+00001a40: 2c20 6178 6973 3d30 290d 0a20 2020 200d  , axis=0)..    .
+00001a50: 0a20 2020 2066 696c 655f 6f75 7420 3d20  .    file_out = 
+00001a60: 6374 675f 7061 7468 202f 2050 6174 6828  ctg_path / Path(
+00001a70: 7374 7228 7965 6172 2929 202f 2050 6174  str(year)) / Pat
+00001a80: 6828 2753 5441 5449 5354 4951 5545 5327  h('STATISTIQUES'
+00001a90: 2920 2f20 5061 7468 2827 7379 6e74 6865  ) / Path('synthe
+00001aa0: 7365 5f61 6468 6572 656e 742e 786c 7378  se_adherent.xlsx
+00001ab0: 2729 0d0a 2020 2020 6467 2e74 6f5f 6578  ')..    dg.to_ex
+00001ac0: 6365 6c28 6669 6c65 5f6f 7574 290d 0a20  cel(file_out).. 
+00001ad0: 2020 200d 0a64 6566 2073 796e 7468 6573     ..def synthes
+00001ae0: 655f 7261 6e64 6f6e 6e65 6528 7965 6172  e_randonnee(year
+00001af0: 2c63 7467 5f70 6174 6829 3a0d 0a0d 0a20  ,ctg_path):.... 
+00001b00: 2020 200d 0a20 2020 2066 726f 6d20 7061     ..    from pa
+00001b10: 7468 6c69 6220 696d 706f 7274 2050 6174  thlib import Pat
+00001b20: 680d 0a0d 0a20 2020 2069 6d70 6f72 7420  h....    import 
+00001b30: 6d61 7470 6c6f 746c 6962 2e70 7970 6c6f  matplotlib.pyplo
+00001b40: 7420 6173 2070 6c74 0d0a 2020 2020 696d  t as plt..    im
+00001b50: 706f 7274 2070 616e 6461 7320 6173 2070  port pandas as p
+00001b60: 640d 0a20 2020 200d 0a20 2020 2069 6d70  d..    ..    imp
+00001b70: 6f72 7420 4354 475f 5574 696c 7320 6173  ort CTG_Utils as
+00001b80: 2063 7467 0d0a 2020 2020 0d0a 2020 2020   ctg..    ..    
+00001b90: 6465 6620 6164 646c 6162 656c 7328 782c  def addlabels(x,
+00001ba0: 792c 6f66 6673 6574 293a 0d0a 2020 2020  y,offset):..    
+00001bb0: 2020 2020 666f 7220 6920 696e 2072 616e      for i in ran
+00001bc0: 6765 286c 656e 2878 2929 3a0d 0a20 2020  ge(len(x)):..   
+00001bd0: 2020 2020 2020 2020 2069 6620 795b 695d           if y[i]
+00001be0: 2021 3d20 303a 0d0a 2020 2020 2020 2020   != 0:..        
+00001bf0: 2020 2020 2020 2020 706c 742e 7465 7874          plt.text
+00001c00: 2878 5b69 5d2c 795b 695d 2b6f 6666 7365  (x[i],y[i]+offse
+00001c10: 742c 726f 756e 6428 795b 695d 2c31 292c  t,round(y[i],1),
+00001c20: 7369 7a65 3d31 3029 0d0a 2020 2020 2020  size=10)..      
+00001c30: 2020 0d0a 2020 2020 0d0a 2020 2020 6669    ..    ..    fi
+00001c40: 6c65 5f69 6e20 3d20 5061 7468 2863 7467  le_in = Path(ctg
+00001c50: 5f70 6174 6829 202f 2050 6174 6828 7374  _path) / Path(st
+00001c60: 7228 7965 6172 2929 202f 2050 6174 6828  r(year)) / Path(
+00001c70: 2753 5441 5449 5354 4951 5545 5327 2920  'STATISTIQUES') 
+00001c80: 2f20 5061 7468 2827 7379 6e74 6865 7365  / Path('synthese
+00001c90: 2e78 6c73 7827 290d 0a20 2020 2064 665f  .xlsx')..    df_
+00001ca0: 746f 7461 6c20 3d20 7064 2e72 6561 645f  total = pd.read_
+00001cb0: 6578 6365 6c28 6669 6c65 5f69 6e29 0d0a  excel(file_in)..
+00001cc0: 2020 2020 6466 5f74 6f74 616c 203d 2064      df_total = d
+00001cd0: 665f 746f 7461 6c2e 6472 6f70 6e61 2873  f_total.dropna(s
+00001ce0: 7562 7365 743d 5b27 4e6f 6d27 5d29 200d  ubset=['Nom']) .
+00001cf0: 0a20 2020 2064 6720 3d20 6466 5f74 6f74  .    dg = df_tot
+00001d00: 616c 2e71 7565 7279 2827 5479 7065 3d3d  al.query('Type==
+00001d10: 2252 414e 444f 4e4e 4545 2227 292e 6772  "RANDONNEE"').gr
+00001d20: 6f75 7062 7928 2773 656a 6f75 7227 292e  oupby('sejour').
+00001d30: 6167 6728 2763 6f75 6e74 2729 5b27 4ec2  agg('count')['N.
+00001d40: b020 4c69 6365 6e63 69c3 a927 5d0d 0a20  . Licenci..'].. 
+00001d50: 2020 200d 0a20 2020 2066 6967 203d 2070     ..    fig = p
+00001d60: 6c74 2e66 6967 7572 6528 6669 6773 697a  lt.figure(figsiz
+00001d70: 653d 2831 302c 3529 290d 0a20 2020 2070  e=(10,5))..    p
+00001d80: 6c74 2e62 6172 2872 616e 6765 286c 656e  lt.bar(range(len
+00001d90: 2864 6729 292c 6467 2e74 6f6c 6973 7428  (dg)),dg.tolist(
+00001da0: 2929 0d0a 2020 2020 6164 646c 6162 656c  ))..    addlabel
+00001db0: 7328 6c69 7374 2872 616e 6765 286c 656e  s(list(range(len
+00001dc0: 2864 6729 2929 2c64 672e 746f 6c69 7374  (dg))),dg.tolist
+00001dd0: 2829 2c30 2e32 290d 0a20 2020 2070 6c74  (),0.2)..    plt
+00001de0: 2e78 7469 636b 7328 7261 6e67 6528 6c65  .xticks(range(le
+00001df0: 6e28 6467 2929 2c20 6467 2e69 6e64 6578  n(dg)), dg.index
+00001e00: 2c20 726f 7461 7469 6f6e 3d27 7665 7274  , rotation='vert
+00001e10: 6963 616c 2729 0d0a 2020 2020 706c 742e  ical')..    plt.
+00001e20: 7469 636b 5f70 6172 616d 7328 6178 6973  tick_params(axis
+00001e30: 3d27 7827 2c20 726f 7461 7469 6f6e 3d39  ='x', rotation=9
+00001e40: 302c 206c 6162 656c 7369 7a65 3d31 3029  0, labelsize=10)
+00001e50: 0d0a 2020 2020 706c 742e 7469 636b 5f70  ..    plt.tick_p
+00001e60: 6172 616d 7328 6178 6973 3d27 7927 2c6c  arams(axis='y',l
+00001e70: 6162 656c 7369 7a65 3d31 3029 0d0a 2020  abelsize=10)..  
+00001e80: 2020 0d0a 2020 2020 5f20 3d20 706c 742e    ..    _ = plt.
+00001e90: 7469 746c 6528 6627 2320 7261 6e64 6f73  title(f'# randos
+00001ea0: 203a 207b 6c65 6e28 6467 297d 202c 2023   : {len(dg)} , #
+00001eb0: 2070 6172 7469 6369 7061 6e74 7320 3a20   participants : 
+00001ec0: 7b73 756d 2864 6729 7d27 290d 0a20 2020  {sum(dg)}')..   
+00001ed0: 2070 6c74 2e74 6967 6874 5f6c 6179 6f75   plt.tight_layou
+00001ee0: 7428 290d 0a20 2020 2070 6c74 2e73 686f  t()..    plt.sho
+00001ef0: 7728 290d 0a20 2020 200d 0a20 2020 2066  w()..    ..    f
+00001f00: 6967 5f66 696c 6520 3d20 2753 594e 5448  ig_file = 'SYNTH
+00001f10: 4553 455f 5241 4e44 4f4e 4e45 4553 2e70  ESE_RANDONNEES.p
+00001f20: 6e67 270d 0a20 2020 2070 6c74 2e73 6176  ng'..    plt.sav
+00001f30: 6566 6967 2863 7467 5f70 6174 6820 2f20  efig(ctg_path / 
+00001f40: 5061 7468 2873 7472 2879 6561 7229 2920  Path(str(year)) 
+00001f50: 2f20 5061 7468 2827 5354 4154 4953 5449  / Path('STATISTI
+00001f60: 5155 4553 2729 202f 2050 6174 6828 6669  QUES') / Path(fi
+00001f70: 675f 6669 6c65 292c 6262 6f78 5f69 6e63  g_file),bbox_inc
+00001f80: 6865 733d 2774 6967 6874 2729 0d0a 2020  hes='tight')..  
+00001f90: 2020 0d0a 6465 6620 6e62 725f 7365 6a6f    ..def nbr_sejo
+00001fa0: 7572 735f 6164 6865 7265 6e74 2879 6561  urs_adherent(yea
+00001fb0: 722c 2063 7467 5f70 6174 6829 3a0d 0a0d  r, ctg_path):...
+00001fc0: 0a20 2020 2066 726f 6d20 636f 6c6c 6563  .    from collec
+00001fd0: 7469 6f6e 7320 696d 706f 7274 2043 6f75  tions import Cou
+00001fe0: 6e74 6572 0d0a 2020 2020 6672 6f6d 2070  nter..    from p
+00001ff0: 6174 686c 6962 2069 6d70 6f72 7420 5061  athlib import Pa
+00002000: 7468 0d0a 2020 2020 0d0a 2020 2020 696d  th..    ..    im
+00002010: 706f 7274 206d 6174 706c 6f74 6c69 622e  port matplotlib.
+00002020: 7079 706c 6f74 2061 7320 706c 740d 0a20  pyplot as plt.. 
+00002030: 2020 2069 6d70 6f72 7420 7061 6e64 6173     import pandas
+00002040: 2061 7320 7064 0d0a 2020 2020 0d0a 2020   as pd..    ..  
+00002050: 2020 706c 742e 7374 796c 652e 7573 6528    plt.style.use(
+00002060: 2767 6770 6c6f 7427 290d 0a20 2020 200d  'ggplot')..    .
+00002070: 0a20 2020 2023 2066 756e 6374 696f 6e20  .    # function 
+00002080: 746f 2061 6464 2076 616c 7565 206c 6162  to add value lab
+00002090: 656c 730d 0a20 2020 2064 6566 2061 6464  els..    def add
+000020a0: 6c61 6265 6c73 2878 2c79 293a 0d0a 2020  labels(x,y):..  
+000020b0: 2020 2020 2020 666f 7220 6920 696e 2072        for i in r
+000020c0: 616e 6765 286c 656e 2878 2929 3a0d 0a20  ange(len(x)):.. 
+000020d0: 2020 2020 2020 2020 2020 2070 6c74 2e74             plt.t
+000020e0: 6578 7428 785b 695d 2d30 2e32 2c79 5b69  ext(x[i]-0.2,y[i
+000020f0: 5d2b 312c 795b 695d 2c73 697a 653d 6c61  ]+1,y[i],size=la
+00002100: 6265 6c5f 7369 7a65 290d 0a20 2020 206c  bel_size)..    l
+00002110: 6162 656c 5f73 697a 6520 3d20 3135 0d0a  abel_size = 15..
+00002120: 2020 2020 6669 6c65 5f69 6e20 3d20 6374      file_in = ct
+00002130: 675f 7061 7468 202f 2050 6174 6828 7374  g_path / Path(st
+00002140: 7228 7965 6172 2929 202f 2050 6174 6828  r(year)) / Path(
+00002150: 2753 5441 5449 5354 4951 5545 5327 2920  'STATISTIQUES') 
+00002160: 2f20 5061 7468 2827 7379 6e74 6865 7365  / Path('synthese
+00002170: 5f61 6468 6572 656e 742e 786c 7378 2729  _adherent.xlsx')
+00002180: 0d0a 2020 2020 6466 5f74 6f74 616c 203d  ..    df_total =
+00002190: 2070 642e 7265 6164 5f65 7863 656c 2866   pd.read_excel(f
+000021a0: 696c 655f 696e 290d 0a20 2020 200d 0a20  ile_in)..    .. 
+000021b0: 2020 2063 203d 2043 6f75 6e74 6572 2829     c = Counter()
+000021c0: 0d0a 2020 2020 6320 3d20 436f 756e 7465  ..    c = Counte
+000021d0: 7228 6466 5f74 6f74 616c 5b27 4e62 725f  r(df_total['Nbr_
+000021e0: 5345 4a4f 5552 5327 5d2e 746f 6c69 7374  SEJOURS'].tolist
+000021f0: 2829 290d 0a20 2020 2063 203d 2063 2e6d  ())..    c = c.m
+00002200: 6f73 745f 636f 6d6d 6f6e 2829 0d0a 0d0a  ost_common()....
+00002210: 2020 2020 782c 2079 203d 207a 6970 282a      x, y = zip(*
+00002220: 6329 0d0a 2020 2020 7820 3d20 6c69 7374  c)..    x = list
+00002230: 2878 290d 0a20 2020 2079 203d 206c 6973  (x)..    y = lis
+00002240: 7428 7929 0d0a 2020 2020 0d0a 2020 2020  t(y)..    ..    
+00002250: 6669 672c 2061 7820 3d20 706c 742e 7375  fig, ax = plt.su
+00002260: 6270 6c6f 7473 2866 6967 7369 7a65 3d28  bplots(figsize=(
+00002270: 352c 3529 290d 0a20 2020 2070 6c74 2e62  5,5))..    plt.b
+00002280: 6172 285b 7374 7228 785f 7329 2066 6f72  ar([str(x_s) for
+00002290: 2078 5f73 2069 6e20 785d 2c79 290d 0a20   x_s in x],y).. 
+000022a0: 2020 2070 6c74 2e78 6c61 6265 6c28 274e     plt.xlabel('N
+000022b0: 6f6d 6272 6520 6465 2070 6172 7469 6369  ombre de partici
+000022c0: 7061 7469 6f6e 20c3 a020 6465 7320 73c3  pation .. des s.
+000022d0: a96a 6f75 7273 2729 0d0a 2020 2020 706c  .jours')..    pl
+000022e0: 742e 796c 6162 656c 2827 4e6f 6d62 7265  t.ylabel('Nombre
+000022f0: 2064 6520 6c69 6365 6e63 6965 7273 2729   de licenciers')
+00002300: 0d0a 2020 2020 706c 742e 7469 636b 5f70  ..    plt.tick_p
+00002310: 6172 616d 7328 6178 6973 3d27 7827 2c20  arams(axis='x', 
+00002320: 6c61 6265 6c73 697a 653d 6c61 6265 6c5f  labelsize=label_
+00002330: 7369 7a65 290d 0a20 2020 2070 6c74 2e74  size)..    plt.t
+00002340: 6963 6b5f 7061 7261 6d73 2861 7869 733d  ick_params(axis=
+00002350: 2779 272c 206c 6162 656c 7369 7a65 3d6c  'y', labelsize=l
+00002360: 6162 656c 5f73 697a 6529 0d0a 2020 2020  abel_size)..    
+00002370: 706c 742e 7469 746c 6528 7374 7228 7965  plt.title(str(ye
+00002380: 6172 292c 7061 643d 3230 2c20 666f 6e74  ar),pad=20, font
+00002390: 7369 7a65 3d32 3029 0d0a 2020 2020 0d0a  size=20)..    ..
+000023a0: 2020 2020 6178 2e73 6574 5f78 6c61 6265      ax.set_xlabe
+000023b0: 6c28 274e 2073 c3a9 6a6f 7572 7327 2c20  l('N s..jours', 
+000023c0: 666f 6e74 7369 7a65 203d 206c 6162 656c  fontsize = label
+000023d0: 5f73 697a 6529 0d0a 2020 2020 6178 2e73  _size)..    ax.s
+000023e0: 6574 5f79 6c61 6265 6c28 274e 6f6d 6272  et_ylabel('Nombr
+000023f0: 6520 6465 2043 5447 2061 7961 6e74 205c  e de CTG ayant \
+00002400: 6e20 7061 7274 6963 6970 c3a9 20c3 a020  n particip.. .. 
+00002410: 4e20 73c3 a96a 6f75 7273 272c 2066 6f6e  N s..jours', fon
+00002420: 7473 697a 6520 3d20 6c61 6265 6c5f 7369  tsize = label_si
+00002430: 7a65 290d 0a20 2020 200d 0a20 2020 2078  ze)..    ..    x
+00002440: 2e73 6f72 7428 290d 0a20 2020 2061 6464  .sort()..    add
+00002450: 6c61 6265 6c73 2878 2c79 290d 0a20 2020  labels(x,y)..   
+00002460: 2070 6c74 2e74 6967 6874 5f6c 6179 6f75   plt.tight_layou
+00002470: 7428 290d 0a20 2020 2070 6c74 2e73 686f  t()..    plt.sho
+00002480: 7728 290d 0a0d 0a20 2020 2066 6967 5f66  w()....    fig_f
+00002490: 696c 6520 3d20 2753 454a 4f55 5253 5f53  ile = 'SEJOURS_S
+000024a0: 5441 545f 5041 5254 4943 4950 4154 494f  TAT_PARTICIPATIO
+000024b0: 4e2e 706e 6727 0d0a 2020 2020 706c 742e  N.png'..    plt.
+000024c0: 7361 7665 6669 6728 6374 675f 7061 7468  savefig(ctg_path
+000024d0: 202f 2050 6174 6828 7374 7228 7965 6172   / Path(str(year
+000024e0: 2929 202f 2050 6174 6828 2753 5441 5449  )) / Path('STATI
+000024f0: 5354 4951 5545 5327 2920 2f20 5061 7468  STIQUES') / Path
+00002500: 2866 6967 5f66 696c 6529 2c62 626f 785f  (fig_file),bbox_
+00002510: 696e 6368 6573 3d27 7469 6768 7427 290d  inches='tight').
+00002520: 0a20 2020 200d 0a64 6566 2072 6561 645f  .    ..def read_
+00002530: 6d65 6d6f 7279 5f73 6f72 7469 6573 2829  memory_sorties()
+00002540: 3a0d 0a0d 0a20 2020 2023 2053 7461 6e64  :....    # Stand
+00002550: 6172 6420 6c69 6272 6172 7920 696d 706f  ard library impo
+00002560: 7274 730d 0a20 2020 2069 6d70 6f72 7420  rts..    import 
+00002570: 6f73 2e70 6174 680d 0a20 2020 2066 726f  os.path..    fro
+00002580: 6d20 7061 7468 6c69 6220 696d 706f 7274  m pathlib import
+00002590: 2050 6174 680d 0a0d 0a20 2020 2023 2033   Path....    # 3
+000025a0: 7264 2070 6172 7479 2069 6d70 6f72 7473  rd party imports
+000025b0: 0d0a 2020 2020 696d 706f 7274 2079 616d  ..    import yam
+000025c0: 6c0d 0a20 2020 200d 0a20 2020 2023 2052  l..    ..    # R
+000025d0: 6561 6473 2074 6865 2064 6566 6175 6c74  eads the default
+000025e0: 2050 5663 6861 7261 6374 6572 697a 6174   PVcharacterizat
+000025f0: 696f 6e2e 7961 6d6c 2063 6f6e 6669 6720  ion.yaml config 
+00002600: 6669 6c65 0d0a 2020 2020 7061 7468 5f63  file..    path_c
+00002610: 6f6e 6669 675f 6669 6c65 203d 2050 6174  onfig_file = Pat
+00002620: 6828 5f5f 6669 6c65 5f5f 292e 7061 7265  h(__file__).pare
+00002630: 6e74 2e70 6172 656e 7420 2f20 5061 7468  nt.parent / Path
+00002640: 2827 4354 475f 4675 6e63 2729 202f 2050  ('CTG_Func') / P
+00002650: 6174 6828 2743 5447 5f52 6566 4669 6c65  ath('CTG_RefFile
+00002660: 7327 2920 2f20 5061 7468 2827 6d65 6d6f  s') / Path('memo
+00002670: 7279 5f73 6f72 7469 6573 2e79 6d6c 2729  ry_sorties.yml')
+00002680: 0d0a 2020 2020 7769 7468 206f 7065 6e28  ..    with open(
+00002690: 7061 7468 5f63 6f6e 6669 675f 6669 6c65  path_config_file
+000026a0: 2920 6173 2066 696c 653a 0d0a 2020 2020  ) as file:..    
+000026b0: 2020 2020 6d65 6d6f 7279 203d 2079 616d      memory = yam
+000026c0: 6c2e 7361 6665 5f6c 6f61 6428 6669 6c65  l.safe_load(file
+000026d0: 290d 0a20 2020 2020 2020 200d 0a20 2020  )..        ..   
+000026e0: 2020 2020 0d0a 2020 2020 7265 7475 726e      ..    return
+000026f0: 206d 656d 6f72 790d 0a20 2020 200d 0a64   memory..    ..d
+00002700: 6566 2065 766f 6c75 7469 6f6e 5f73 6f72  ef evolution_sor
+00002710: 7469 6573 2874 7970 652c 6374 675f 7061  ties(type,ctg_pa
+00002720: 7468 293a 0d0a 0d0a 2020 2020 2320 5374  th):....    # St
+00002730: 616e 6461 7264 206c 6962 7261 7279 2069  andard library i
+00002740: 6d70 6f72 7420 2020 200d 0a20 2020 2069  mport    ..    i
+00002750: 6d70 6f72 7420 6461 7465 7469 6d65 0d0a  mport datetime..
+00002760: 2020 2020 6672 6f6d 2070 6174 686c 6962      from pathlib
+00002770: 2069 6d70 6f72 7420 5061 7468 0d0a 2020   import Path..  
+00002780: 2020 6672 6f6d 2063 6f6c 6c65 6374 696f    from collectio
+00002790: 6e73 2069 6d70 6f72 7420 6e61 6d65 6474  ns import namedt
+000027a0: 7570 6c65 0d0a 0d0a 2020 2020 2320 5468  uple....    # Th
+000027b0: 6972 6420 7061 7274 7920 6c69 6272 6172  ird party librar
+000027c0: 7920 696d 706f 7274 2020 2020 200d 0a20  y import     .. 
+000027d0: 2020 2069 6d70 6f72 7420 6d61 7470 6c6f     import matplo
+000027e0: 746c 6962 2e70 7970 6c6f 7420 6173 2070  tlib.pyplot as p
+000027f0: 6c74 0d0a 2020 2020 696d 706f 7274 2070  lt..    import p
+00002800: 616e 6461 7320 6173 2070 640d 0a20 2020  andas as pd..   
+00002810: 2020 200d 0a20 2020 2023 2049 6e74 6572     ..    # Inter
+00002820: 6e61 6c20 696d 706f 7274 0d0a 2020 2020  nal import..    
+00002830: 696d 706f 7274 2043 5447 5f55 7469 6c73  import CTG_Utils
+00002840: 2061 7320 6374 670d 0a20 2020 2066 726f   as ctg..    fro
+00002850: 6d20 4354 475f 5574 696c 732e 4354 475f  m CTG_Utils.CTG_
+00002860: 4755 492e 4755 495f 476c 6f62 616c 7320  GUI.GUI_Globals 
+00002870: 696d 706f 7274 2041 4354 4956 4954 455f  import ACTIVITE_
+00002880: 4c49 5354 200d 0a20 2020 200d 0a20 2020  LIST ..    ..   
+00002890: 2064 6566 2061 6464 5f6d 656d 6f72 7928   def add_memory(
+000028a0: 7374 6174 5f64 6963 2c79 6561 7273 293a  stat_dic,years):
+000028b0: 0d0a 2020 2020 2020 2020 6d65 6d6f 7279  ..        memory
+000028c0: 203d 2072 6561 645f 6d65 6d6f 7279 5f73   = read_memory_s
+000028d0: 6f72 7469 6573 2829 0d0a 2020 2020 0d0a  orties()..    ..
+000028e0: 2020 2020 0d0a 2020 2020 2020 2020 666f      ..        fo
+000028f0: 7220 7965 6172 2c76 2069 6e20 6d65 6d6f  r year,v in memo
+00002900: 7279 5b27 6d65 6d6f 7279 275d 2e69 7465  ry['memory'].ite
+00002910: 6d73 2829 3a0d 0a20 2020 2020 2020 2020  ms():..         
+00002920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002940: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+00002950: 7374 6174 5f64 6963 5b73 7472 2879 6561  stat_dic[str(yea
+00002960: 7229 5d20 3d20 7374 6174 7965 6172 2876  r)] = statyear(v
+00002970: 5b27 5041 5254 4943 4950 4154 494f 4e5f  ['PARTICIPATION_
+00002980: 5345 4a4f 5552 5327 5d2c 2020 2020 2020  SEJOURS'],      
+00002990: 2020 2020 2020 2020 2020 2320 6e62 725f            # nbr_
+000029a0: 7365 6a6f 7572 730d 0a20 2020 2020 2020  sejours..       
 000029b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000029c0: 2020 2320 6a6f 7572 735f 7365 6a6f 7572    # jours_sejour
-000029d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000029c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000029d0: 2020 2020 302c 2020 2020 2020 2020 2020      0,          
 000029e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000029f0: 2020 2020 2020 2020 2020 2020 2076 5b27               v['
-00002a00: 534f 5254 4945 535f 434c 5542 5f44 494d  SORTIES_CLUB_DIM
-00002a10: 414e 4348 4527 5d2c 2023 2073 6f72 7469  ANCHE'], # sorti
-00002a20: 655f 6469 6d61 6e63 6865 5f63 6c75 620d  e_dimanche_club.
-00002a30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002a50: 2020 2020 2020 2020 2020 2020 765b 2753              v['S
-00002a60: 4f52 5449 4553 5f43 4c55 425f 5341 4d45  ORTIES_CLUB_SAME
-00002a70: 4449 275d 2c20 2020 2320 736f 7274 6965  DI'],   # sortie
-00002a80: 5f73 616d 6564 695f 636c 7562 0d0a 2020  _samedi_club..  
-00002a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002ab0: 2020 2020 2020 2020 2076 5b27 534f 5254           v['SORT
-00002ac0: 4945 535f 4849 5645 5227 5d2c 2020 2020  IES_HIVER'],    
-00002ad0: 2020 2020 2023 2073 6f72 7469 655f 6869       # sortie_hi
-00002ae0: 7665 725f 636c 7562 0d0a 2020 2020 2020  ver_club..      
-00002af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002b10: 2020 2020 2076 5b27 534f 5254 4945 535f       v['SORTIES_
-00002b20: 434c 5542 5f4a 4555 4449 275d 2c20 2020  CLUB_JEUDI'],   
-00002b30: 2023 2073 6f72 7469 655f 6a65 7564 695f   # sortie_jeudi_
-00002b40: 636c 7562 0d0a 2020 2020 2020 2020 2020  club..          
-00002b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002b70: 2076 5b27 5241 4e44 4f4e 4e45 4553 275d   v['RANDONNEES']
-00002b80: 2c20 2020 2020 2020 2020 2020 2023 2072  ,            # r
-00002b90: 616e 646f 6e6e 6565 0d0a 2020 2020 2020  andonnee..      
-00002ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002bc0: 2020 2020 2076 5b27 4e6f 6d62 7265 5f73       v['Nombre_s
-00002bd0: 656a 6f75 7273 275d 2c20 2020 2020 2020  ejours'],       
-00002be0: 2023 206e 6272 5f73 656a 6f75 7273 0d0a   # nbr_sejours..
-00002bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002c10: 2020 2020 2020 2020 2020 2030 2c29 2020             0,)  
+000029f0: 2320 6a6f 7572 735f 7365 6a6f 7572 0d0a  # jours_sejour..
+00002a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002a20: 2020 2020 2020 2020 2020 2076 5b27 534f             v['SO
+00002a30: 5254 4945 535f 434c 5542 5f44 494d 414e  RTIES_CLUB_DIMAN
+00002a40: 4348 4527 5d2c 2023 2073 6f72 7469 655f  CHE'], # sortie_
+00002a50: 6469 6d61 6e63 6865 5f63 6c75 620d 0a20  dimanche_club.. 
+00002a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002a80: 2020 2020 2020 2020 2020 765b 2753 4f52            v['SOR
+00002a90: 5449 4553 5f43 4c55 425f 5341 4d45 4449  TIES_CLUB_SAMEDI
+00002aa0: 275d 2c20 2020 2320 736f 7274 6965 5f73  '],   # sortie_s
+00002ab0: 616d 6564 695f 636c 7562 0d0a 2020 2020  amedi_club..    
+00002ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002ae0: 2020 2020 2020 2076 5b27 534f 5254 4945         v['SORTIE
+00002af0: 535f 4849 5645 5227 5d2c 2020 2020 2020  S_HIVER'],      
+00002b00: 2020 2023 2073 6f72 7469 655f 6869 7665     # sortie_hive
+00002b10: 725f 636c 7562 0d0a 2020 2020 2020 2020  r_club..        
+00002b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002b40: 2020 2076 5b27 534f 5254 4945 535f 434c     v['SORTIES_CL
+00002b50: 5542 5f4a 4555 4449 275d 2c20 2020 2023  UB_JEUDI'],    #
+00002b60: 2073 6f72 7469 655f 6a65 7564 695f 636c   sortie_jeudi_cl
+00002b70: 7562 0d0a 2020 2020 2020 2020 2020 2020  ub..            
+00002b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002b90: 2020 2020 2020 2020 2020 2020 2020 2076                 v
+00002ba0: 5b27 5241 4e44 4f4e 4e45 4553 275d 2c20  ['RANDONNEES'], 
+00002bb0: 2020 2020 2020 2020 2020 2023 2072 616e             # ran
+00002bc0: 646f 6e6e 6565 0d0a 2020 2020 2020 2020  donnee..        
+00002bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002bf0: 2020 2076 5b27 4e6f 6d62 7265 5f73 656a     v['Nombre_sej
+00002c00: 6f75 7273 275d 2c20 2020 2020 2020 2023  ours'],        #
+00002c10: 206e 6272 5f73 656a 6f75 7273 0d0a 2020   nbr_sejours..  
 00002c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002c30: 2020 2020 2020 2023 206e 6272 5f6a 6f75         # nbr_jou
-00002c40: 7273 5f73 656a 6f75 7273 0d0a 2020 2020  rs_sejours..    
+00002c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002c40: 2020 2020 2020 2020 2030 2c29 2020 2020           0,)    
 00002c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002c80: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-00002c90: 2020 2020 2020 7965 6172 732e 6170 7065        years.appe
-00002ca0: 6e64 2873 7472 2879 6561 7229 290d 0a20  nd(str(year)).. 
-00002cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002cc0: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-00002cd0: 0a20 2020 2064 6566 2066 696c 6c5f 7374  .    def fill_st
-00002ce0: 6174 5f79 6561 7228 7965 6172 293a 0d0a  at_year(year):..
-00002cf0: 2020 2020 0d0a 2020 2020 2020 2020 2320      ..        # 
-00002d00: 496e 7465 726e 616c 206c 6962 7261 7279  Internal library
-00002d10: 2069 6d70 6f72 7473 0d0a 2020 2020 2020   imports..      
-00002d20: 2020 6672 6f6d 2043 5447 5f55 7469 6c73    from CTG_Utils
-00002d30: 2e43 5447 5f46 756e 632e 4354 475f 7574  .CTG_Func.CTG_ut
-00002d40: 696c 6974 7920 696d 706f 7274 2067 6574  ility import get
-00002d50: 5f73 656a 6f75 725f 696e 666f 0d0a 2020  _sejour_info..  
-00002d60: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-00002d70: 7365 6a6f 7572 5f69 6e66 6f20 3d20 6765  sejour_info = ge
-00002d80: 745f 7365 6a6f 7572 5f69 6e66 6f28 6374  t_sejour_info(ct
-00002d90: 675f 7061 7468 2c79 6561 7229 0d0a 2020  g_path,year)..  
-00002da0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-00002db0: 0d0a 2020 2020 2020 2020 6669 6c65 5f69  ..        file_i
-00002dc0: 6e20 3d20 6374 675f 7061 7468 202f 2050  n = ctg_path / P
-00002dd0: 6174 6828 7374 7228 7965 6172 2929 202f  ath(str(year)) /
-00002de0: 2050 6174 6828 2753 5441 5449 5354 4951   Path('STATISTIQ
-00002df0: 5545 5327 2920 2f20 5061 7468 2827 7379  UES') / Path('sy
-00002e00: 6e74 6865 7365 5f61 6468 6572 656e 742e  nthese_adherent.
-00002e10: 786c 7378 2729 0d0a 2020 2020 2020 2020  xlsx')..        
-00002e20: 0d0a 2020 2020 2020 2020 6466 203d 2070  ..        df = p
-00002e30: 642e 7265 6164 5f65 7863 656c 2866 696c  d.read_excel(fil
-00002e40: 655f 696e 290d 0a20 2020 2020 2020 200d  e_in)..        .
-00002e50: 0a20 2020 2020 2020 2073 7461 745f 7965  .        stat_ye
-00002e60: 6172 203d 2073 7461 7479 6561 7228 6466  ar = statyear(df
-00002e70: 5b27 4e62 725f 5345 4a4f 5552 5327 5d2e  ['Nbr_SEJOURS'].
-00002e80: 7375 6d28 292c 2020 2020 2020 2020 2020  sum(),          
-00002e90: 2020 2023 206e 6272 5f6a 6f75 7273 5f70     # nbr_jours_p
-00002ea0: 6172 7469 6369 7061 7469 6f6e 5f73 656a  articipation_sej
-00002eb0: 6f75 7273 0d0a 2020 2020 2020 2020 2020  ours..          
-00002ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002ed0: 2020 2064 665b 2753 454a 4f55 522d 4a4f     df['SEJOUR-JO
-00002ee0: 5552 275d 2e73 756d 2829 2c20 2020 2020  UR'].sum(),     
-00002ef0: 2020 2020 2020 2020 2320 6e62 725f 7061          # nbr_pa
-00002f00: 7274 6963 6970 6174 696f 6e73 5f73 656a  rticipations_sej
-00002f10: 6f75 720d 0a20 2020 2020 2020 2020 2020  our..           
-00002f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002f30: 2020 6466 5b27 534f 5254 4945 2044 5520    df['SORTIE DU 
-00002f40: 4449 4d41 4e43 4845 2043 4c55 4227 5d2e  DIMANCHE CLUB'].
-00002f50: 7375 6d28 292c 2023 2073 6f72 7469 655f  sum(), # sortie_
-00002f60: 6469 6d61 6e63 6865 5f63 6c75 620d 0a20  dimanche_club.. 
-00002f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002f80: 2020 2020 2020 2020 2020 2020 6466 5b27              df['
-00002f90: 534f 5254 4945 2044 5520 5341 4d45 4449  SORTIE DU SAMEDI
-00002fa0: 2043 4c55 4227 5d2e 7375 6d28 292c 2020   CLUB'].sum(),  
-00002fb0: 2023 2073 6f72 7469 655f 7361 6d65 6469   # sortie_samedi
-00002fc0: 5f63 6c75 620d 0a20 2020 2020 2020 2020  _club..         
-00002fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002fe0: 2020 2020 6466 5b27 534f 5254 4945 2048      df['SORTIE H
-00002ff0: 4956 4552 275d 2e73 756d 2829 2c20 2020  IVER'].sum(),   
-00003000: 2020 2020 2020 2020 2023 2073 6f72 7469           # sorti
-00003010: 655f 6869 7665 725f 636c 7562 0d0a 2020  e_hiver_club..  
-00003020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003030: 2020 2020 2020 2020 2020 2064 665b 2753             df['S
-00003040: 4f52 5449 4520 4455 204a 4555 4449 2043  ORTIE DU JEUDI C
-00003050: 4c55 4227 5d2e 7375 6d28 292c 2020 2020  LUB'].sum(),    
-00003060: 2320 736f 7274 6965 5f6a 6575 6469 5f63  # sortie_jeudi_c
-00003070: 6c75 620d 0a20 2020 2020 2020 2020 2020  lub..           
-00003080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003090: 2020 6466 5b27 5241 4e44 4f4e 4e45 4527    df['RANDONNEE'
-000030a0: 5d2e 7375 6d28 292c 2020 2020 2020 2020  ].sum(),        
-000030b0: 2020 2020 2020 2023 2072 616e 646f 6e6e         # randonn
-000030c0: 6565 0d0a 2020 2020 2020 2020 2020 2020  ee..            
-000030d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000030e0: 2073 656a 6f75 725f 696e 666f 2e6e 6272   sejour_info.nbr
-000030f0: 5f73 656a 6f75 7273 2c20 2020 2020 2020  _sejours,       
-00003100: 2020 2020 2020 2320 6e62 725f 7365 6a6f        # nbr_sejo
-00003110: 7572 7320 0d0a 2020 2020 2020 2020 2020  urs ..          
-00003120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003130: 2020 2073 656a 6f75 725f 696e 666f 2e6e     sejour_info.n
-00003140: 6272 5f6a 6f75 7273 2920 2020 2020 2020  br_jours)       
-00003150: 2020 2020 2020 2020 2320 6e62 725f 6a6f          # nbr_jo
-00003160: 7572 735f 7365 6a6f 7572 7320 2020 2020  urs_sejours     
-00003170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003180: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-00003190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000031a0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-000031b0: 2020 7265 7475 726e 2073 7461 745f 7965    return stat_ye
-000031c0: 6172 0d0a 2020 2020 0d0a 2020 2020 6465  ar..    ..    de
-000031d0: 6620 6164 646c 6162 656c 7328 782c 792c  f addlabels(x,y,
-000031e0: 6f66 6673 6574 293a 0d0a 2020 2020 2020  offset):..      
-000031f0: 2020 666f 7220 6920 696e 2072 616e 6765    for i in range
-00003200: 286c 656e 2878 2929 3a0d 0a20 2020 2020  (len(x)):..     
-00003210: 2020 2020 2020 2070 6c74 2e74 6578 7428         plt.text(
-00003220: 785b 695d 2c79 5b69 5d2b 6f66 6673 6574  x[i],y[i]+offset
-00003230: 2c72 6f75 6e64 2879 5b69 5d2c 3129 2c73  ,round(y[i],1),s
-00003240: 697a 653d 3130 290d 0a20 2020 2020 2020  ize=10)..       
-00003250: 2020 2020 200d 0a20 2020 2064 6566 2070       ..    def p
-00003260: 6c6f 745f 7374 6174 2879 6561 7273 2c6e  lot_stat(years,n
-00003270: 625f 7061 7274 6963 6970 616e 7473 2c74  b_participants,t
-00003280: 6974 6c65 2c6c 6162 656c 5f79 293a 0d0a  itle,label_y):..
-00003290: 2020 2020 2020 2020 706c 742e 7375 6270          plt.subp
-000032a0: 6c6f 7428 312c 312c 3129 0d0a 2020 2020  lot(1,1,1)..    
-000032b0: 2020 2020 636f 6c6f 7273 203d 205b 2723      colors = ['#
-000032c0: 6664 6161 3438 275d 200d 0a20 2020 2020  fdaa48'] ..     
-000032d0: 2020 2073 697a 655f 6c61 6265 6c20 3d20     size_label = 
-000032e0: 3230 0d0a 2020 2020 2020 2020 706c 742e  20..        plt.
-000032f0: 6261 7228 7965 6172 732c 6e62 5f70 6172  bar(years,nb_par
-00003300: 7469 6369 7061 6e74 732c 636f 6c6f 723d  ticipants,color=
-00003310: 636f 6c6f 7273 290d 0a20 2020 2020 2020  colors)..       
-00003320: 2070 6c74 2e79 6c61 6265 6c28 6c61 6265   plt.ylabel(labe
-00003330: 6c5f 792c 7369 7a65 3d73 697a 655f 6c61  l_y,size=size_la
-00003340: 6265 6c29 0d0a 2020 2020 2020 2020 6164  bel)..        ad
-00003350: 646c 6162 656c 7328 7965 6172 732c 6e62  dlabels(years,nb
-00003360: 5f70 6172 7469 6369 7061 6e74 732c 3129  _participants,1)
-00003370: 0d0a 2020 2020 2020 2020 706c 742e 7874  ..        plt.xt
-00003380: 6963 6b73 2872 6f74 6174 696f 6e3d 3930  icks(rotation=90
-00003390: 290d 0a20 2020 2020 2020 2070 6c74 2e74  )..        plt.t
-000033a0: 6963 6b5f 7061 7261 6d73 2861 7869 733d  ick_params(axis=
-000033b0: 2778 272c 206c 6162 656c 7369 7a65 3d73  'x', labelsize=s
-000033c0: 697a 655f 6c61 6265 6c29 0d0a 2020 2020  ize_label)..    
-000033d0: 2020 2020 706c 742e 7469 636b 5f70 6172      plt.tick_par
-000033e0: 616d 7328 6178 6973 3d27 7927 2c20 6c61  ams(axis='y', la
-000033f0: 6265 6c73 697a 653d 7369 7a65 5f6c 6162  belsize=size_lab
-00003400: 656c 290d 0a20 2020 2020 2020 2070 6c74  el)..        plt
-00003410: 2e74 6974 6c65 2874 6974 6c65 2c66 6f6e  .title(title,fon
-00003420: 7473 697a 653d 3138 290d 0a20 2020 2020  tsize=18)..     
-00003430: 2020 2070 6c74 2e74 6967 6874 5f6c 6179     plt.tight_lay
-00003440: 6f75 7428 290d 0a20 2020 2020 2020 2070  out()..        p
-00003450: 6c74 2e73 686f 7728 290d 0a20 2020 200d  lt.show()..    .
-00003460: 0a20 2020 2073 7461 7479 6561 7220 3d20  .    statyear = 
-00003470: 6e61 6d65 6474 7570 6c65 2827 6163 7469  namedtuple('acti
-00003480: 7669 7465 272c 2041 4354 4956 4954 455f  vite', ACTIVITE_
-00003490: 4c49 5354 290d 0a20 0d0a 2020 2020 706c  LIST).. ..    pl
-000034a0: 742e 7374 796c 652e 7573 6528 2767 6770  t.style.use('ggp
-000034b0: 6c6f 7427 290d 0a20 2020 2079 6561 7273  lot')..    years
-000034c0: 203d 205b 5d0d 0a20 2020 2073 7461 745f   = []..    stat_
-000034d0: 6469 6320 3d20 7b7d 0d0a 2020 2020 6164  dic = {}..    ad
-000034e0: 645f 6d65 6d6f 7279 2873 7461 745f 6469  d_memory(stat_di
-000034f0: 632c 7965 6172 7329 0d0a 0d0a 2020 2020  c,years)....    
-00003500: 746f 6461 7920 3d20 6461 7465 7469 6d65  today = datetime
-00003510: 2e64 6174 6574 696d 652e 6e6f 7728 290d  .datetime.now().
-00003520: 0a20 2020 2079 6561 7273 5f6e 6577 203d  .    years_new =
-00003530: 205b 7374 7228 7965 6172 2920 666f 7220   [str(year) for 
-00003540: 7965 6172 2069 6e20 7261 6e67 6528 3230  year in range(20
-00003550: 3232 2c74 6f64 6179 2e79 6561 722b 3129  22,today.year+1)
-00003560: 5d0d 0a20 2020 2066 6f72 2079 6561 7220  ]..    for year 
-00003570: 696e 2079 6561 7273 5f6e 6577 3a0d 0a20  in years_new:.. 
-00003580: 2020 2020 2020 2073 7461 745f 6469 635b         stat_dic[
-00003590: 7965 6172 5d20 3d20 6669 6c6c 5f73 7461  year] = fill_sta
-000035a0: 745f 7965 6172 2879 6561 7229 0d0a 2020  t_year(year)..  
-000035b0: 2020 2020 2020 0d0a 2020 2020 7965 6172        ..    year
-000035c0: 7320 3d20 7965 6172 7320 2b20 7965 6172  s = years + year
-000035d0: 735f 6e65 7720 2020 0d0a 2020 2020 0d0a  s_new   ..    ..
-000035e0: 2020 2020 0d0a 2020 2020 6966 2074 7970      ..    if typ
-000035f0: 6520 3d3d 2027 6e62 725f 6a6f 7572 735f  e == 'nbr_jours_
-00003600: 7061 7274 6963 6970 6174 696f 6e5f 7365  participation_se
-00003610: 6a6f 7572 7327 3a0d 0a20 2020 2020 2020  jours':..       
-00003620: 2070 6c6f 745f 7374 6174 2879 6561 7273   plot_stat(years
-00003630: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00003640: 2020 2020 205b 7374 6174 5f64 6963 5b79       [stat_dic[y
-00003650: 6561 725d 2e6e 6272 5f6a 6f75 7273 5f70  ear].nbr_jours_p
-00003660: 6172 7469 6369 7061 7469 6f6e 5f73 656a  articipation_sej
-00003670: 6f75 7273 2066 6f72 2079 6561 7220 696e  ours for year in
-00003680: 2079 6561 7273 5d2c 0d0a 2020 2020 2020   years],..      
-00003690: 2020 2020 2020 2020 2020 2020 7479 7065              type
-000036a0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-000036b0: 2020 2020 2074 7970 6529 0d0a 2020 2020       type)..    
-000036c0: 656c 6966 2020 7479 7065 203d 3d20 2773  elif  type == 's
-000036d0: 6f72 7469 655f 6469 6d61 6e63 6865 5f63  ortie_dimanche_c
-000036e0: 6c75 6227 3a0d 0a20 2020 2020 2020 2070  lub':..        p
-000036f0: 6c6f 745f 7374 6174 2879 6561 7273 2c0d  lot_stat(years,.
-00003700: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003710: 2020 205b 7374 6174 5f64 6963 5b79 6561     [stat_dic[yea
-00003720: 725d 2e73 6f72 7469 655f 6469 6d61 6e63  r].sortie_dimanc
-00003730: 6865 5f63 6c75 6220 666f 7220 7965 6172  he_club for year
-00003740: 2069 6e20 7965 6172 735d 2c0d 0a20 2020   in years],..   
-00003750: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-00003760: 7970 652c 0d0a 2020 2020 2020 2020 2020  ype,..          
-00003770: 2020 2020 2020 2020 2723 7061 7274 6963          '#partic
-00003780: 6970 616e 7473 2729 0d0a 2020 2020 656c  ipants')..    el
-00003790: 6966 2020 7479 7065 203d 3d20 2773 6f72  if  type == 'sor
-000037a0: 7469 655f 7361 6d65 6469 5f63 6c75 6227  tie_samedi_club'
-000037b0: 3a0d 0a20 2020 2020 2020 2070 6c6f 745f  :..        plot_
-000037c0: 7374 6174 2879 6561 7273 2c0d 0a20 2020  stat(years,..   
-000037d0: 2020 2020 2020 2020 2020 2020 2020 205b                 [
-000037e0: 7374 6174 5f64 6963 5b79 6561 725d 2e73  stat_dic[year].s
-000037f0: 6f72 7469 655f 7361 6d65 6469 5f63 6c75  ortie_samedi_clu
-00003800: 6220 666f 7220 7965 6172 2069 6e20 7965  b for year in ye
-00003810: 6172 735d 2c0d 0a20 2020 2020 2020 2020  ars],..         
-00003820: 2020 2020 2020 2020 2074 7970 652c 0d0a           type,..
-00003830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003840: 2020 2723 7061 7274 6963 6970 616e 7473    '#participants
-00003850: 2729 0d0a 2020 2020 656c 6966 2020 7479  ')..    elif  ty
-00003860: 7065 203d 3d20 2773 6f72 7469 655f 6a65  pe == 'sortie_je
-00003870: 7564 695f 636c 7562 273a 0d0a 2020 2020  udi_club':..    
-00003880: 2020 2020 706c 6f74 5f73 7461 7428 7965      plot_stat(ye
-00003890: 6172 732c 0d0a 2020 2020 2020 2020 2020  ars,..          
-000038a0: 2020 2020 2020 2020 5b73 7461 745f 6469          [stat_di
-000038b0: 635b 7965 6172 5d2e 736f 7274 6965 5f6a  c[year].sortie_j
-000038c0: 6575 6469 5f63 6c75 6220 666f 7220 7965  eudi_club for ye
-000038d0: 6172 2069 6e20 7965 6172 735d 2c0d 0a20  ar in years],.. 
-000038e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000038f0: 2074 7970 652c 0d0a 2020 2020 2020 2020   type,..        
-00003900: 2020 2020 2020 2020 2020 2723 7061 7274            '#part
-00003910: 6963 6970 616e 7473 2729 2020 0d0a 2020  icipants')  ..  
-00003920: 2020 656c 6966 2020 7479 7065 203d 3d20    elif  type == 
-00003930: 2772 616e 646f 6e6e 6565 273a 0d0a 2020  'randonnee':..  
-00003940: 2020 2020 2020 706c 6f74 5f73 7461 7428        plot_stat(
-00003950: 7965 6172 732c 0d0a 2020 2020 2020 2020  years,..        
-00003960: 2020 2020 2020 2020 2020 5b73 7461 745f            [stat_
-00003970: 6469 635b 7965 6172 5d2e 7261 6e64 6f6e  dic[year].randon
-00003980: 6e65 6520 666f 7220 7965 6172 2069 6e20  nee for year in 
-00003990: 7965 6172 735d 2c0d 0a20 2020 2020 2020  years],..       
-000039a0: 2020 2020 2020 2020 2020 2074 7970 652c             type,
-000039b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000039c0: 2020 2020 2723 7061 7274 6963 6970 616e      '#participan
-000039d0: 7473 2729 2020 0d0a 2020 2020 656c 6966  ts')  ..    elif
-000039e0: 2020 7479 7065 203d 3d20 276e 6272 5f70    type == 'nbr_p
-000039f0: 6172 7469 6369 7061 7469 6f6e 735f 7365  articipations_se
-00003a00: 6a6f 7572 7327 3a0d 0a20 2020 2020 2020  jours':..       
-00003a10: 2070 6c6f 745f 7374 6174 2879 6561 7273   plot_stat(years
-00003a20: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00003a30: 2020 2020 205b 7374 6174 5f64 6963 5b79       [stat_dic[y
-00003a40: 6561 725d 2e6e 6272 5f70 6172 7469 6369  ear].nbr_partici
-00003a50: 7061 7469 6f6e 735f 7365 6a6f 7572 7320  pations_sejours 
-00003a60: 666f 7220 7965 6172 2069 6e20 7965 6172  for year in year
-00003a70: 735d 2c0d 0a20 2020 2020 2020 2020 2020  s],..           
-00003a80: 2020 2020 2020 2027 4e6f 6d62 7265 2064         'Nombre d
-00003a90: 6520 7061 7274 6963 6970 6174 696f 6e73  e participations
-00003aa0: 2061 7578 2073 c3a9 6a6f 7572 7327 2c0d   aux s..jours',.
-00003ab0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003ac0: 2020 2027 2320 7061 7274 6963 6970 6174     '# participat
-00003ad0: 696f 6e73 2061 7578 2073 c3a9 6a6f 7572  ions aux s..jour
-00003ae0: 7327 2920 0d0a 2020 2020 656c 6966 2020  s') ..    elif  
-00003af0: 7479 7065 203d 3d20 276e 6272 5f73 656a  type == 'nbr_sej
-00003b00: 6f75 7273 273a 0d0a 2020 2020 2020 2020  ours':..        
-00003b10: 706c 6f74 5f73 7461 7428 7965 6172 732c  plot_stat(years,
-00003b20: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00003b30: 2020 2020 5b73 7461 745f 6469 635b 7965      [stat_dic[ye
-00003b40: 6172 5d2e 6e62 725f 7365 6a6f 7572 7320  ar].nbr_sejours 
-00003b50: 666f 7220 7965 6172 2069 6e20 7965 6172  for year in year
-00003b60: 735d 2c0d 0a20 2020 2020 2020 2020 2020  s],..           
-00003b70: 2020 2020 2020 2027 4e6f 6d62 7265 2064         'Nombre d
-00003b80: 6520 73c3 a96a 6f75 7273 272c 0d0a 2020  e s..jours',..  
-00003b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003ba0: 2723 2073 c3a9 6a6f 7572 7327 290d 0a20  '# s..jours').. 
-00003bb0: 2020 2065 6c69 6620 2074 7970 6520 3d3d     elif  type ==
-00003bc0: 2027 6e62 725f 6a6f 7572 735f 7365 6a6f   'nbr_jours_sejo
-00003bd0: 7572 7327 3a0d 0a20 2020 2020 2020 2070  urs':..        p
-00003be0: 6c6f 745f 7374 6174 2879 6561 7273 2c0d  lot_stat(years,.
-00003bf0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003c00: 2020 205b 7374 6174 5f64 6963 5b79 6561     [stat_dic[yea
-00003c10: 725d 2e6e 6272 5f6a 6f75 7273 5f73 656a  r].nbr_jours_sej
-00003c20: 6f75 7273 2066 6f72 2079 6561 7220 696e  ours for year in
-00003c30: 2079 6561 7273 5d2c 0d0a 2020 2020 2020   years],..      
-00003c40: 2020 2020 2020 2020 2020 2020 274e 6f6d              'Nom
-00003c50: 6272 6520 6465 206a 6f75 7273 2073 c3a9  bre de jours s..
-00003c60: 6a6f 7572 7327 2c0d 0a20 2020 2020 2020  jours',..       
-00003c70: 2020 2020 2020 2020 2020 2027 2320 6a6f             '# jo
-00003c80: 7572 7320 73c3 a96a 6f75 7227 2920 2020  urs s..jour')   
-00003c90: 2020 2020 20                                  
+00002c60: 2020 2020 2023 206e 6272 5f6a 6f75 7273       # nbr_jours
+00002c70: 5f73 656a 6f75 7273 0d0a 2020 2020 2020  _sejours..      
+00002c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002cb0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+00002cc0: 2020 2020 7965 6172 732e 6170 7065 6e64      years.append
+00002cd0: 2873 7472 2879 6561 7229 290d 0a20 2020  (str(year))..   
+00002ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002cf0: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
+00002d00: 2020 2064 6566 2066 696c 6c5f 7374 6174     def fill_stat
+00002d10: 5f79 6561 7228 7965 6172 293a 0d0a 2020  _year(year):..  
+00002d20: 2020 0d0a 2020 2020 2020 2020 2320 496e    ..        # In
+00002d30: 7465 726e 616c 206c 6962 7261 7279 2069  ternal library i
+00002d40: 6d70 6f72 7473 0d0a 2020 2020 2020 2020  mports..        
+00002d50: 6672 6f6d 2043 5447 5f55 7469 6c73 2e43  from CTG_Utils.C
+00002d60: 5447 5f46 756e 632e 4354 475f 7574 696c  TG_Func.CTG_util
+00002d70: 6974 7920 696d 706f 7274 2067 6574 5f73  ity import get_s
+00002d80: 656a 6f75 725f 696e 666f 0d0a 2020 2020  ejour_info..    
+00002d90: 2020 2020 0d0a 2020 2020 2020 2020 7365      ..        se
+00002da0: 6a6f 7572 5f69 6e66 6f20 3d20 6765 745f  jour_info = get_
+00002db0: 7365 6a6f 7572 5f69 6e66 6f28 6374 675f  sejour_info(ctg_
+00002dc0: 7061 7468 2c79 6561 7229 0d0a 2020 2020  path,year)..    
+00002dd0: 2020 2020 0d0a 2020 2020 2020 2020 0d0a      ..        ..
+00002de0: 2020 2020 2020 2020 6669 6c65 5f69 6e20          file_in 
+00002df0: 3d20 6374 675f 7061 7468 202f 2050 6174  = ctg_path / Pat
+00002e00: 6828 7374 7228 7965 6172 2929 202f 2050  h(str(year)) / P
+00002e10: 6174 6828 2753 5441 5449 5354 4951 5545  ath('STATISTIQUE
+00002e20: 5327 2920 2f20 5061 7468 2827 7379 6e74  S') / Path('synt
+00002e30: 6865 7365 5f61 6468 6572 656e 742e 786c  hese_adherent.xl
+00002e40: 7378 2729 0d0a 2020 2020 2020 2020 0d0a  sx')..        ..
+00002e50: 2020 2020 2020 2020 6466 203d 2070 642e          df = pd.
+00002e60: 7265 6164 5f65 7863 656c 2866 696c 655f  read_excel(file_
+00002e70: 696e 290d 0a20 2020 2020 2020 200d 0a20  in)..        .. 
+00002e80: 2020 2020 2020 2073 7461 745f 7965 6172         stat_year
+00002e90: 203d 2073 7461 7479 6561 7228 6466 5b27   = statyear(df['
+00002ea0: 4e62 725f 5345 4a4f 5552 5327 5d2e 7375  Nbr_SEJOURS'].su
+00002eb0: 6d28 292c 2020 2020 2020 2020 2020 2020  m(),            
+00002ec0: 2023 206e 6272 5f6a 6f75 7273 5f70 6172   # nbr_jours_par
+00002ed0: 7469 6369 7061 7469 6f6e 5f73 656a 6f75  ticipation_sejou
+00002ee0: 7273 0d0a 2020 2020 2020 2020 2020 2020  rs..            
+00002ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002f00: 2064 665b 2753 454a 4f55 522d 4a4f 5552   df['SEJOUR-JOUR
+00002f10: 275d 2e73 756d 2829 2c20 2020 2020 2020  '].sum(),       
+00002f20: 2020 2020 2020 2320 6e62 725f 7061 7274        # nbr_part
+00002f30: 6963 6970 6174 696f 6e73 5f73 656a 6f75  icipations_sejou
+00002f40: 720d 0a20 2020 2020 2020 2020 2020 2020  r..             
+00002f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002f60: 6466 5b27 534f 5254 4945 2044 5520 4449  df['SORTIE DU DI
+00002f70: 4d41 4e43 4845 2043 4c55 4227 5d2e 7375  MANCHE CLUB'].su
+00002f80: 6d28 292c 2023 2073 6f72 7469 655f 6469  m(), # sortie_di
+00002f90: 6d61 6e63 6865 5f63 6c75 620d 0a20 2020  manche_club..   
+00002fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002fb0: 2020 2020 2020 2020 2020 6466 5b27 534f            df['SO
+00002fc0: 5254 4945 2044 5520 5341 4d45 4449 2043  RTIE DU SAMEDI C
+00002fd0: 4c55 4227 5d2e 7375 6d28 292c 2020 2023  LUB'].sum(),   #
+00002fe0: 2073 6f72 7469 655f 7361 6d65 6469 5f63   sortie_samedi_c
+00002ff0: 6c75 620d 0a20 2020 2020 2020 2020 2020  lub..           
+00003000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003010: 2020 6466 5b27 534f 5254 4945 2048 4956    df['SORTIE HIV
+00003020: 4552 275d 2e73 756d 2829 2c20 2020 2020  ER'].sum(),     
+00003030: 2020 2020 2020 2023 2073 6f72 7469 655f         # sortie_
+00003040: 6869 7665 725f 636c 7562 0d0a 2020 2020  hiver_club..    
+00003050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003060: 2020 2020 2020 2020 2064 665b 2753 4f52           df['SOR
+00003070: 5449 4520 4455 204a 4555 4449 2043 4c55  TIE DU JEUDI CLU
+00003080: 4227 5d2e 7375 6d28 292c 2020 2020 2320  B'].sum(),    # 
+00003090: 736f 7274 6965 5f6a 6575 6469 5f63 6c75  sortie_jeudi_clu
+000030a0: 620d 0a20 2020 2020 2020 2020 2020 2020  b..             
+000030b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000030c0: 6466 5b27 5241 4e44 4f4e 4e45 4527 5d2e  df['RANDONNEE'].
+000030d0: 7375 6d28 292c 2020 2020 2020 2020 2020  sum(),          
+000030e0: 2020 2020 2023 2072 616e 646f 6e6e 6565       # randonnee
+000030f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00003100: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00003110: 656a 6f75 725f 696e 666f 2e6e 6272 5f73  ejour_info.nbr_s
+00003120: 656a 6f75 7273 2c20 2020 2020 2020 2020  ejours,         
+00003130: 2020 2020 2320 6e62 725f 7365 6a6f 7572      # nbr_sejour
+00003140: 7320 0d0a 2020 2020 2020 2020 2020 2020  s ..            
+00003150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003160: 2073 656a 6f75 725f 696e 666f 2e6e 6272   sejour_info.nbr
+00003170: 5f6a 6f75 7273 2920 2020 2020 2020 2020  _jours)         
+00003180: 2020 2020 2020 2320 6e62 725f 6a6f 7572        # nbr_jour
+00003190: 735f 7365 6a6f 7572 7320 2020 2020 2020  s_sejours       
+000031a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000031b0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+000031c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000031d0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+000031e0: 7265 7475 726e 2073 7461 745f 7965 6172  return stat_year
+000031f0: 0d0a 2020 2020 0d0a 2020 2020 6465 6620  ..    ..    def 
+00003200: 6164 646c 6162 656c 7328 782c 792c 6f66  addlabels(x,y,of
+00003210: 6673 6574 293a 0d0a 2020 2020 2020 2020  fset):..        
+00003220: 666f 7220 6920 696e 2072 616e 6765 286c  for i in range(l
+00003230: 656e 2878 2929 3a0d 0a20 2020 2020 2020  en(x)):..       
+00003240: 2020 2020 2070 6c74 2e74 6578 7428 785b       plt.text(x[
+00003250: 695d 2c79 5b69 5d2b 6f66 6673 6574 2c72  i],y[i]+offset,r
+00003260: 6f75 6e64 2879 5b69 5d2c 3129 2c73 697a  ound(y[i],1),siz
+00003270: 653d 3130 290d 0a20 2020 2020 2020 2020  e=10)..         
+00003280: 2020 200d 0a20 2020 2064 6566 2070 6c6f     ..    def plo
+00003290: 745f 7374 6174 2879 6561 7273 2c6e 625f  t_stat(years,nb_
+000032a0: 7061 7274 6963 6970 616e 7473 2c74 6974  participants,tit
+000032b0: 6c65 2c6c 6162 656c 5f79 293a 0d0a 2020  le,label_y):..  
+000032c0: 2020 2020 2020 706c 742e 6669 6775 7265        plt.figure
+000032d0: 2866 6967 7369 7a65 3d28 382c 2036 2929  (figsize=(8, 6))
+000032e0: 0d0a 2020 2020 2020 2020 636f 6c6f 7273  ..        colors
+000032f0: 203d 205b 2723 6664 6161 3438 275d 200d   = ['#fdaa48'] .
+00003300: 0a20 2020 2020 2020 2073 697a 655f 6c61  .        size_la
+00003310: 6265 6c20 3d20 3230 0d0a 2020 2020 2020  bel = 20..      
+00003320: 2020 706c 742e 6261 7228 7965 6172 732c    plt.bar(years,
+00003330: 6e62 5f70 6172 7469 6369 7061 6e74 732c  nb_participants,
+00003340: 636f 6c6f 723d 636f 6c6f 7273 290d 0a20  color=colors).. 
+00003350: 2020 2020 2020 2070 6c74 2e79 6c61 6265         plt.ylabe
+00003360: 6c28 6c61 6265 6c5f 792c 7369 7a65 3d73  l(label_y,size=s
+00003370: 697a 655f 6c61 6265 6c29 0d0a 2020 2020  ize_label)..    
+00003380: 2020 2020 6164 646c 6162 656c 7328 7965      addlabels(ye
+00003390: 6172 732c 6e62 5f70 6172 7469 6369 7061  ars,nb_participa
+000033a0: 6e74 732c 3129 0d0a 2020 2020 2020 2020  nts,1)..        
+000033b0: 706c 742e 7874 6963 6b73 2872 6f74 6174  plt.xticks(rotat
+000033c0: 696f 6e3d 3930 290d 0a20 2020 2020 2020  ion=90)..       
+000033d0: 2070 6c74 2e74 6963 6b5f 7061 7261 6d73   plt.tick_params
+000033e0: 2861 7869 733d 2778 272c 206c 6162 656c  (axis='x', label
+000033f0: 7369 7a65 3d73 697a 655f 6c61 6265 6c29  size=size_label)
+00003400: 0d0a 2020 2020 2020 2020 706c 742e 7469  ..        plt.ti
+00003410: 636b 5f70 6172 616d 7328 6178 6973 3d27  ck_params(axis='
+00003420: 7927 2c20 6c61 6265 6c73 697a 653d 7369  y', labelsize=si
+00003430: 7a65 5f6c 6162 656c 290d 0a20 2020 2020  ze_label)..     
+00003440: 2020 2070 6c74 2e74 6974 6c65 2874 6974     plt.title(tit
+00003450: 6c65 2c66 6f6e 7473 697a 653d 3138 290d  le,fontsize=18).
+00003460: 0a20 2020 2020 2020 2070 6c74 2e74 6967  .        plt.tig
+00003470: 6874 5f6c 6179 6f75 7428 290d 0a20 2020  ht_layout()..   
+00003480: 2020 2020 2070 6c74 2e73 686f 7728 290d       plt.show().
+00003490: 0a20 2020 200d 0a20 2020 2073 7461 7479  .    ..    staty
+000034a0: 6561 7220 3d20 6e61 6d65 6474 7570 6c65  ear = namedtuple
+000034b0: 2827 6163 7469 7669 7465 272c 2041 4354  ('activite', ACT
+000034c0: 4956 4954 455f 4c49 5354 290d 0a20 0d0a  IVITE_LIST).. ..
+000034d0: 2020 2020 706c 742e 7374 796c 652e 7573      plt.style.us
+000034e0: 6528 2767 6770 6c6f 7427 290d 0a20 2020  e('ggplot')..   
+000034f0: 2079 6561 7273 203d 205b 5d0d 0a20 2020   years = []..   
+00003500: 2073 7461 745f 6469 6320 3d20 7b7d 0d0a   stat_dic = {}..
+00003510: 2020 2020 6164 645f 6d65 6d6f 7279 2873      add_memory(s
+00003520: 7461 745f 6469 632c 7965 6172 7329 0d0a  tat_dic,years)..
+00003530: 0d0a 2020 2020 746f 6461 7920 3d20 6461  ..    today = da
+00003540: 7465 7469 6d65 2e64 6174 6574 696d 652e  tetime.datetime.
+00003550: 6e6f 7728 290d 0a20 2020 2079 6561 7273  now()..    years
+00003560: 5f6e 6577 203d 205b 7374 7228 7965 6172  _new = [str(year
+00003570: 2920 666f 7220 7965 6172 2069 6e20 7261  ) for year in ra
+00003580: 6e67 6528 3230 3232 2c74 6f64 6179 2e79  nge(2022,today.y
+00003590: 6561 722b 3129 5d0d 0a20 2020 2066 6f72  ear+1)]..    for
+000035a0: 2079 6561 7220 696e 2079 6561 7273 5f6e   year in years_n
+000035b0: 6577 3a0d 0a20 2020 2020 2020 2073 7461  ew:..        sta
+000035c0: 745f 6469 635b 7965 6172 5d20 3d20 6669  t_dic[year] = fi
+000035d0: 6c6c 5f73 7461 745f 7965 6172 2879 6561  ll_stat_year(yea
+000035e0: 7229 0d0a 2020 2020 2020 2020 0d0a 2020  r)..        ..  
+000035f0: 2020 7965 6172 7320 3d20 7965 6172 7320    years = years 
+00003600: 2b20 7965 6172 735f 6e65 7720 2020 0d0a  + years_new   ..
+00003610: 2020 2020 0d0a 2020 2020 0d0a 2020 2020      ..    ..    
+00003620: 6966 2074 7970 6520 3d3d 2027 6e62 725f  if type == 'nbr_
+00003630: 6a6f 7572 735f 7061 7274 6963 6970 6174  jours_participat
+00003640: 696f 6e5f 7365 6a6f 7572 7327 3a0d 0a20  ion_sejours':.. 
+00003650: 2020 2020 2020 2070 6c6f 745f 7374 6174         plot_stat
+00003660: 2879 6561 7273 2c0d 0a20 2020 2020 2020  (years,..       
+00003670: 2020 2020 2020 2020 2020 205b 7374 6174             [stat
+00003680: 5f64 6963 5b79 6561 725d 2e6e 6272 5f6a  _dic[year].nbr_j
+00003690: 6f75 7273 5f70 6172 7469 6369 7061 7469  ours_participati
+000036a0: 6f6e 5f73 656a 6f75 7273 2066 6f72 2079  on_sejours for y
+000036b0: 6561 7220 696e 2079 6561 7273 5d2c 0d0a  ear in years],..
+000036c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000036d0: 2020 7479 7065 2c0d 0a20 2020 2020 2020    type,..       
+000036e0: 2020 2020 2020 2020 2020 2074 7970 6529             type)
+000036f0: 0d0a 2020 2020 656c 6966 2020 7479 7065  ..    elif  type
+00003700: 203d 3d20 2773 6f72 7469 655f 6469 6d61   == 'sortie_dima
+00003710: 6e63 6865 5f63 6c75 6227 3a0d 0a20 2020  nche_club':..   
+00003720: 2020 2020 2070 6c6f 745f 7374 6174 2879       plot_stat(y
+00003730: 6561 7273 2c0d 0a20 2020 2020 2020 2020  ears,..         
+00003740: 2020 2020 2020 2020 205b 7374 6174 5f64           [stat_d
+00003750: 6963 5b79 6561 725d 2e73 6f72 7469 655f  ic[year].sortie_
+00003760: 6469 6d61 6e63 6865 5f63 6c75 6220 666f  dimanche_club fo
+00003770: 7220 7965 6172 2069 6e20 7965 6172 735d  r year in years]
+00003780: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00003790: 2020 2020 2074 7970 652c 0d0a 2020 2020       type,..    
+000037a0: 2020 2020 2020 2020 2020 2020 2020 2723                '#
+000037b0: 7061 7274 6963 6970 616e 7473 2729 0d0a  participants')..
+000037c0: 2020 2020 656c 6966 2020 7479 7065 203d      elif  type =
+000037d0: 3d20 2773 6f72 7469 655f 7361 6d65 6469  = 'sortie_samedi
+000037e0: 5f63 6c75 6227 3a0d 0a20 2020 2020 2020  _club':..       
+000037f0: 2070 6c6f 745f 7374 6174 2879 6561 7273   plot_stat(years
+00003800: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00003810: 2020 2020 205b 7374 6174 5f64 6963 5b79       [stat_dic[y
+00003820: 6561 725d 2e73 6f72 7469 655f 7361 6d65  ear].sortie_same
+00003830: 6469 5f63 6c75 6220 666f 7220 7965 6172  di_club for year
+00003840: 2069 6e20 7965 6172 735d 2c0d 0a20 2020   in years],..   
+00003850: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+00003860: 7970 652c 0d0a 2020 2020 2020 2020 2020  ype,..          
+00003870: 2020 2020 2020 2020 2723 7061 7274 6963          '#partic
+00003880: 6970 616e 7473 2729 0d0a 2020 2020 656c  ipants')..    el
+00003890: 6966 2020 7479 7065 203d 3d20 2773 6f72  if  type == 'sor
+000038a0: 7469 655f 6a65 7564 695f 636c 7562 273a  tie_jeudi_club':
+000038b0: 0d0a 2020 2020 2020 2020 706c 6f74 5f73  ..        plot_s
+000038c0: 7461 7428 7965 6172 732c 0d0a 2020 2020  tat(years,..    
+000038d0: 2020 2020 2020 2020 2020 2020 2020 5b73                [s
+000038e0: 7461 745f 6469 635b 7965 6172 5d2e 736f  tat_dic[year].so
+000038f0: 7274 6965 5f6a 6575 6469 5f63 6c75 6220  rtie_jeudi_club 
+00003900: 666f 7220 7965 6172 2069 6e20 7965 6172  for year in year
+00003910: 735d 2c0d 0a20 2020 2020 2020 2020 2020  s],..           
+00003920: 2020 2020 2020 2074 7970 652c 0d0a 2020         type,..  
+00003930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003940: 2723 7061 7274 6963 6970 616e 7473 2729  '#participants')
+00003950: 2020 0d0a 2020 2020 656c 6966 2020 7479    ..    elif  ty
+00003960: 7065 203d 3d20 2772 616e 646f 6e6e 6565  pe == 'randonnee
+00003970: 273a 0d0a 2020 2020 2020 2020 706c 6f74  ':..        plot
+00003980: 5f73 7461 7428 7965 6172 732c 0d0a 2020  _stat(years,..  
+00003990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000039a0: 5b73 7461 745f 6469 635b 7965 6172 5d2e  [stat_dic[year].
+000039b0: 7261 6e64 6f6e 6e65 6520 666f 7220 7965  randonnee for ye
+000039c0: 6172 2069 6e20 7965 6172 735d 2c0d 0a20  ar in years],.. 
+000039d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000039e0: 2074 7970 652c 0d0a 2020 2020 2020 2020   type,..        
+000039f0: 2020 2020 2020 2020 2020 2723 7061 7274            '#part
+00003a00: 6963 6970 616e 7473 2729 2020 0d0a 2020  icipants')  ..  
+00003a10: 2020 656c 6966 2020 7479 7065 203d 3d20    elif  type == 
+00003a20: 276e 6272 5f70 6172 7469 6369 7061 7469  'nbr_participati
+00003a30: 6f6e 735f 7365 6a6f 7572 7327 3a0d 0a20  ons_sejours':.. 
+00003a40: 2020 2020 2020 2070 6c6f 745f 7374 6174         plot_stat
+00003a50: 2879 6561 7273 2c0d 0a20 2020 2020 2020  (years,..       
+00003a60: 2020 2020 2020 2020 2020 205b 7374 6174             [stat
+00003a70: 5f64 6963 5b79 6561 725d 2e6e 6272 5f70  _dic[year].nbr_p
+00003a80: 6172 7469 6369 7061 7469 6f6e 735f 7365  articipations_se
+00003a90: 6a6f 7572 7320 666f 7220 7965 6172 2069  jours for year i
+00003aa0: 6e20 7965 6172 735d 2c0d 0a20 2020 2020  n years],..     
+00003ab0: 2020 2020 2020 2020 2020 2020 2027 4e6f               'No
+00003ac0: 6d62 7265 2064 6520 7061 7274 6963 6970  mbre de particip
+00003ad0: 6174 696f 6e73 2061 7578 2073 c3a9 6a6f  ations aux s..jo
+00003ae0: 7572 7327 2c0d 0a20 2020 2020 2020 2020  urs',..         
+00003af0: 2020 2020 2020 2020 2027 2320 7061 7274           '# part
+00003b00: 6963 6970 6174 696f 6e73 2061 7578 2073  icipations aux s
+00003b10: c3a9 6a6f 7572 7327 2920 0d0a 2020 2020  ..jours') ..    
+00003b20: 656c 6966 2020 7479 7065 203d 3d20 276e  elif  type == 'n
+00003b30: 6272 5f73 656a 6f75 7273 273a 0d0a 2020  br_sejours':..  
+00003b40: 2020 2020 2020 706c 6f74 5f73 7461 7428        plot_stat(
+00003b50: 7965 6172 732c 0d0a 2020 2020 2020 2020  years,..        
+00003b60: 2020 2020 2020 2020 2020 5b73 7461 745f            [stat_
+00003b70: 6469 635b 7965 6172 5d2e 6e62 725f 7365  dic[year].nbr_se
+00003b80: 6a6f 7572 7320 666f 7220 7965 6172 2069  jours for year i
+00003b90: 6e20 7965 6172 735d 2c0d 0a20 2020 2020  n years],..     
+00003ba0: 2020 2020 2020 2020 2020 2020 2027 4e6f               'No
+00003bb0: 6d62 7265 2064 6520 73c3 a96a 6f75 7273  mbre de s..jours
+00003bc0: 272c 0d0a 2020 2020 2020 2020 2020 2020  ',..            
+00003bd0: 2020 2020 2020 2723 2073 c3a9 6a6f 7572        '# s..jour
+00003be0: 7327 290d 0a20 2020 2065 6c69 6620 2074  s')..    elif  t
+00003bf0: 7970 6520 3d3d 2027 6e62 725f 6a6f 7572  ype == 'nbr_jour
+00003c00: 735f 7365 6a6f 7572 7327 3a0d 0a20 2020  s_sejours':..   
+00003c10: 2020 2020 2070 6c6f 745f 7374 6174 2879       plot_stat(y
+00003c20: 6561 7273 2c0d 0a20 2020 2020 2020 2020  ears,..         
+00003c30: 2020 2020 2020 2020 205b 7374 6174 5f64           [stat_d
+00003c40: 6963 5b79 6561 725d 2e6e 6272 5f6a 6f75  ic[year].nbr_jou
+00003c50: 7273 5f73 656a 6f75 7273 2066 6f72 2079  rs_sejours for y
+00003c60: 6561 7220 696e 2079 6561 7273 5d2c 0d0a  ear in years],..
+00003c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003c80: 2020 274e 6f6d 6272 6520 6465 206a 6f75    'Nombre de jou
+00003c90: 7273 2073 c3a9 6a6f 7572 7327 2c0d 0a20  rs s..jours',.. 
+00003ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003cb0: 2027 2320 6a6f 7572 7320 73c3 a96a 6f75   '# jours s..jou
+00003cc0: 7227 2920 2020 2020 2020 20              r')
```

### Comparing `CTG_Utils-1.1.0/CTG_Utils/CTG_Func/CTG_utility.py` & `CTG_Utils-1.1.1/CTG_Utils/CTG_Func/CTG_utility.py`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.1.0/CTG_Utils/CTG_GUI/GUI_Globals.py` & `CTG_Utils-1.1.1/CTG_Utils/CTG_GUI/GUI_Globals.py`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.1.0/CTG_Utils/CTG_GUI/PageDivers.py` & `CTG_Utils-1.1.1/CTG_Utils/CTG_GUI/PageDivers.py`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.1.0/CTG_Utils/CTG_GUI/PageEffectif.py` & `CTG_Utils-1.1.1/CTG_Utils/CTG_GUI/PageEffectif.py`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.1.0/CTG_Utils/CTG_GUI/PageSorties.py` & `CTG_Utils-1.1.1/CTG_Utils/CTG_GUI/PageSorties.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     from tkinter import messagebox
     
     # Local imports
     from CTG_Utils.CTG_Func.CTG_plot import stat_sorties_club
     
     path_sorties =  ctg_path / Path(str(year)) / Path(type_sortie)
     file_label =  ctg_path / Path(str(year)) / Path(r'DATA/info_randos.yaml')    
-    df_total = stat_sorties_club(path_sorties,None,file_label,year)
+    df_total = stat_sorties_club(path_sorties,ctg_path,None,file_label,year)
     
     
     #info_title = "- Information -"
     #info_text  = f"L'analyse des IFs a été effectuée pour l'année {year_select} "
     #info_text += f"avec les valeurs {analysis_if}. "
     #info_text += f"\n\nLes fichiers obtenus ont été créés dans le dossier :"
     #info_text += f"\n\n''."
```

### Comparing `CTG_Utils-1.1.0/CTG_Utils/CTG_GUI/PageSynthese.py` & `CTG_Utils-1.1.1/CTG_Utils/CTG_GUI/PageSynthese.py`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.1.0/CTG_Utils/CTG_GUI/PageTendance.py` & `CTG_Utils-1.1.1/CTG_Utils/CTG_GUI/PageTendance.py`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.1.0/CTG_Utils/CTG_GUI/Page_Classes.py` & `CTG_Utils-1.1.1/CTG_Utils/CTG_GUI/Page_Classes.py`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.1.0/CTG_Utils/CTG_GUI/Useful_Classes.py` & `CTG_Utils-1.1.1/CTG_Utils/CTG_GUI/Useful_Classes.py`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.1.0/CTG_Utils/CTG_GUI/Useful_Functions.py` & `CTG_Utils-1.1.1/CTG_Utils/CTG_GUI/Useful_Functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -265,15 +265,15 @@
                  6: 'samedi'}
     inv_days_dict = dict(zip(days_dict.values(),days_dict.keys()))
     month_dict = dict(zip(itertools.islice(itertools.cycle(l:=range(1,13)),2,2+len(l)),l))
 
     root = Path(ctg_path) / Path(str(year))
 
     for day in ['dimanche','samedi','jeudi']:
-        path = Path(ctg.GLOBAL['ROOT']) / Path(str(year)) / Path('SORTIES DU '+day.upper()) / Path('CSV')
+        path = ctg_path / Path(str(year)) / Path('SORTIES DU '+day.upper()) / Path('CSV')
             
         r = []
         rw = []
         for m in range(1,13):
             m_save=m
             y = int(year)%100
             c = int(int(year)/100)
```

### Comparing `CTG_Utils-1.1.0/CTG_Utils.egg-info/PKG-INFO` & `CTG_Utils-1.1.1/CTG_Utils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CTG-Utils
-Version: 1.1.0
+Version: 1.1.1
 Summary: A toolbox for ctg statistics analysis
 Home-page: https://github.com/Bertin-fap/CTG_Utils 
 Author: f. bertin
 Author-email: francois.bertin7@wanadoo.fr
 License: MIT
 Keywords: ffvelo,ctg
 Platform: UNKNOWN
```

### Comparing `CTG_Utils-1.1.0/CTG_Utils.egg-info/SOURCES.txt` & `CTG_Utils-1.1.1/CTG_Utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.1.0/LICENSE` & `CTG_Utils-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.1.0/PKG-INFO` & `CTG_Utils-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CTG_Utils
-Version: 1.1.0
+Version: 1.1.1
 Summary: A toolbox for ctg statistics analysis
 Home-page: https://github.com/Bertin-fap/CTG_Utils 
 Author: f. bertin
 Author-email: francois.bertin7@wanadoo.fr
 License: MIT
 Keywords: ffvelo,ctg
 Platform: UNKNOWN
```

### Comparing `CTG_Utils-1.1.0/setup.py` & `CTG_Utils-1.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     long_description = f.read()
 
 install_requires = open(path.join(this_directory, 'requirements.txt'), encoding='utf-8').read().strip().split('\n') 
 
 # This setup is suitable for "python setup.py develop".
 
 setup(name='CTG_Utils',
-      version='1.1.0',
+      version='1.1.1',
       description='A toolbox for ctg statistics analysis',
       long_description=long_description,
       long_description_content_type='text/markdown',
       include_package_data = True,
       license = 'MIT',
       classifiers = [
         'Development Status :: 4 - Beta',
```

