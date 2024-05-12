# Comparing `tmp/openalex-analysis-0.8.2.tar.gz` & `tmp/openalex-analysis-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openalex-analysis-0.8.2.tar", last modified: Tue Oct 10 14:51:17 2023, max compression
+gzip compressed data, was "openalex-analysis-0.9.0.tar", last modified: Mon Feb 12 16:49:59 2024, max compression
```

## Comparing `openalex-analysis-0.8.2.tar` & `openalex-analysis-0.9.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 romain    (1000) romain    (1000)        0 2023-10-10 14:51:17.257611 openalex-analysis-0.8.2/
--rw-rw-r--   0 romain    (1000) romain    (1000)    35149 2023-06-19 14:21:45.000000 openalex-analysis-0.8.2/LICENCE.txt
--rw-rw-r--   0 romain    (1000) romain    (1000)      119 2023-09-07 12:12:26.000000 openalex-analysis-0.8.2/MANIFEST.in
--rw-r--r--   0 romain    (1000) romain    (1000)    51006 2023-10-10 14:51:17.257611 openalex-analysis-0.8.2/PKG-INFO
--rw-rw-r--   0 romain    (1000) romain    (1000)     9429 2023-10-10 14:48:56.000000 openalex-analysis-0.8.2/README.md
-drwxrwxr-x   0 romain    (1000) romain    (1000)        0 2023-10-10 14:51:17.253611 openalex-analysis-0.8.2/openalex_analysis/
--rw-rw-r--   0 romain    (1000) romain    (1000)       95 2023-07-18 10:11:47.000000 openalex-analysis-0.8.2/openalex_analysis/__init__.py
-drwxrwxr-x   0 romain    (1000) romain    (1000)        0 2023-10-10 14:51:17.253611 openalex-analysis-0.8.2/openalex_analysis/analysis/
--rw-rw-r--   0 romain    (1000) romain    (1000)     1276 2023-10-04 12:24:13.000000 openalex-analysis-0.8.2/openalex_analysis/analysis/__init__.py
--rw-rw-r--   0 romain    (1000) romain    (1000)    54183 2023-10-05 12:43:08.000000 openalex-analysis-0.8.2/openalex_analysis/analysis/entities_analysis.py
-drwxrwxr-x   0 romain    (1000) romain    (1000)        0 2023-10-10 14:51:17.257611 openalex-analysis-0.8.2/openalex_analysis/names/
--rw-rw-r--   0 romain    (1000) romain    (1000)       98 2023-07-18 10:11:40.000000 openalex-analysis-0.8.2/openalex_analysis/names/__init__.py
--rw-rw-r--   0 romain    (1000) romain    (1000)     1564 2023-09-07 12:13:00.000000 openalex-analysis-0.8.2/openalex_analysis/names/entitie_names.py
--rw-rw-r--   0 romain    (1000) romain    (1000)  1533228 2023-07-18 09:50:11.000000 openalex-analysis-0.8.2/openalex_analysis/names/list_all_concepts.parquet
--rw-rw-r--   0 romain    (1000) romain    (1000)  1576130 2023-07-18 09:50:11.000000 openalex-analysis-0.8.2/openalex_analysis/names/list_all_institutions.parquet
-drwxrwxr-x   0 romain    (1000) romain    (1000)        0 2023-10-10 14:51:17.257611 openalex-analysis-0.8.2/openalex_analysis/plot/
--rw-rw-r--   0 romain    (1000) romain    (1000)     1123 2023-10-04 12:23:53.000000 openalex-analysis-0.8.2/openalex_analysis/plot/__init__.py
--rw-rw-r--   0 romain    (1000) romain    (1000)    20034 2023-10-05 13:45:37.000000 openalex-analysis-0.8.2/openalex_analysis/plot/entities_plot.py
-drwxrwxr-x   0 romain    (1000) romain    (1000)        0 2023-10-10 14:51:17.253611 openalex-analysis-0.8.2/openalex_analysis.egg-info/
--rw-r--r--   0 romain    (1000) romain    (1000)    51006 2023-10-10 14:51:17.000000 openalex-analysis-0.8.2/openalex_analysis.egg-info/PKG-INFO
--rw-rw-r--   0 romain    (1000) romain    (1000)      625 2023-10-10 14:51:17.000000 openalex-analysis-0.8.2/openalex_analysis.egg-info/SOURCES.txt
--rw-rw-r--   0 romain    (1000) romain    (1000)        1 2023-10-10 14:51:17.000000 openalex-analysis-0.8.2/openalex_analysis.egg-info/dependency_links.txt
--rw-rw-r--   0 romain    (1000) romain    (1000)      164 2023-10-10 14:51:17.000000 openalex-analysis-0.8.2/openalex_analysis.egg-info/requires.txt
--rw-rw-r--   0 romain    (1000) romain    (1000)       18 2023-10-10 14:51:17.000000 openalex-analysis-0.8.2/openalex_analysis.egg-info/top_level.txt
--rw-rw-r--   0 romain    (1000) romain    (1000)     1262 2023-10-10 14:50:10.000000 openalex-analysis-0.8.2/pyproject.toml
--rw-rw-r--   0 romain    (1000) romain    (1000)       38 2023-10-10 14:51:17.261611 openalex-analysis-0.8.2/setup.cfg
+drwxrwxr-x   0 romain    (1000) romain    (1000)        0 2024-02-12 16:49:59.370841 openalex-analysis-0.9.0/
+-rw-rw-r--   0 romain    (1000) romain    (1000)    35149 2023-06-19 14:21:45.000000 openalex-analysis-0.9.0/LICENCE.txt
+-rw-rw-r--   0 romain    (1000) romain    (1000)      119 2023-09-07 12:12:26.000000 openalex-analysis-0.9.0/MANIFEST.in
+-rw-r--r--   0 romain    (1000) romain    (1000)    51006 2024-02-12 16:49:59.366841 openalex-analysis-0.9.0/PKG-INFO
+-rw-rw-r--   0 romain    (1000) romain    (1000)     9429 2024-02-12 16:46:46.000000 openalex-analysis-0.9.0/README.md
+drwxrwxr-x   0 romain    (1000) romain    (1000)        0 2024-02-12 16:49:59.362841 openalex-analysis-0.9.0/openalex_analysis/
+-rw-rw-r--   0 romain    (1000) romain    (1000)       95 2023-07-18 10:11:47.000000 openalex-analysis-0.9.0/openalex_analysis/__init__.py
+drwxrwxr-x   0 romain    (1000) romain    (1000)        0 2024-02-12 16:49:59.366841 openalex-analysis-0.9.0/openalex_analysis/analysis/
+-rw-rw-r--   0 romain    (1000) romain    (1000)     1276 2023-10-04 12:24:13.000000 openalex-analysis-0.9.0/openalex_analysis/analysis/__init__.py
+-rw-rw-r--   0 romain    (1000) romain    (1000)    58903 2024-02-12 14:24:20.000000 openalex-analysis-0.9.0/openalex_analysis/analysis/entities_analysis.py
+drwxrwxr-x   0 romain    (1000) romain    (1000)        0 2024-02-12 16:49:59.366841 openalex-analysis-0.9.0/openalex_analysis/names/
+-rw-rw-r--   0 romain    (1000) romain    (1000)       98 2023-07-18 10:11:40.000000 openalex-analysis-0.9.0/openalex_analysis/names/__init__.py
+-rw-rw-r--   0 romain    (1000) romain    (1000)     1564 2023-09-07 12:13:00.000000 openalex-analysis-0.9.0/openalex_analysis/names/entitie_names.py
+-rw-rw-r--   0 romain    (1000) romain    (1000)  1533228 2023-07-18 09:50:11.000000 openalex-analysis-0.9.0/openalex_analysis/names/list_all_concepts.parquet
+-rw-rw-r--   0 romain    (1000) romain    (1000)  1576130 2023-07-18 09:50:11.000000 openalex-analysis-0.9.0/openalex_analysis/names/list_all_institutions.parquet
+drwxrwxr-x   0 romain    (1000) romain    (1000)        0 2024-02-12 16:49:59.366841 openalex-analysis-0.9.0/openalex_analysis/plot/
+-rw-rw-r--   0 romain    (1000) romain    (1000)     1123 2023-10-04 12:23:53.000000 openalex-analysis-0.9.0/openalex_analysis/plot/__init__.py
+-rw-rw-r--   0 romain    (1000) romain    (1000)    23199 2023-11-01 17:02:48.000000 openalex-analysis-0.9.0/openalex_analysis/plot/entities_plot.py
+drwxrwxr-x   0 romain    (1000) romain    (1000)        0 2024-02-12 16:49:59.366841 openalex-analysis-0.9.0/openalex_analysis.egg-info/
+-rw-r--r--   0 romain    (1000) romain    (1000)    51006 2024-02-12 16:49:59.000000 openalex-analysis-0.9.0/openalex_analysis.egg-info/PKG-INFO
+-rw-rw-r--   0 romain    (1000) romain    (1000)      625 2024-02-12 16:49:59.000000 openalex-analysis-0.9.0/openalex_analysis.egg-info/SOURCES.txt
+-rw-rw-r--   0 romain    (1000) romain    (1000)        1 2024-02-12 16:49:59.000000 openalex-analysis-0.9.0/openalex_analysis.egg-info/dependency_links.txt
+-rw-rw-r--   0 romain    (1000) romain    (1000)      164 2024-02-12 16:49:59.000000 openalex-analysis-0.9.0/openalex_analysis.egg-info/requires.txt
+-rw-rw-r--   0 romain    (1000) romain    (1000)       18 2024-02-12 16:49:59.000000 openalex-analysis-0.9.0/openalex_analysis.egg-info/top_level.txt
+-rw-rw-r--   0 romain    (1000) romain    (1000)     1262 2024-02-12 16:46:31.000000 openalex-analysis-0.9.0/pyproject.toml
+-rw-rw-r--   0 romain    (1000) romain    (1000)       38 2024-02-12 16:49:59.370841 openalex-analysis-0.9.0/setup.cfg
```

### Comparing `openalex-analysis-0.8.2/LICENCE.txt` & `openalex-analysis-0.9.0/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `openalex-analysis-0.8.2/PKG-INFO` & `openalex-analysis-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openalex-analysis
-Version: 0.8.2
+Version: 0.9.0
 Summary: A python library to analyse articles, institutions, and others entities from the OpenAlex API
 Author-email: Romain Thomas <romain.thomas@su.se>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -914,8 +914,8 @@
 
 - `redis_client` The Redis client configuration. Don't forget to add `from redis import StrictRedis` where the configuration is defined.
 
 - `redis_cache` The Redis cache configuration. Don't forget to add `from redis_cache import RedisCache` where the configuration is defined.
 
 
 
-Romain Thomas 2023
+Romain Thomas 2024
```

### Comparing `openalex-analysis-0.8.2/README.md` & `openalex-analysis-0.9.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -212,8 +212,8 @@
 
 - `redis_client` The Redis client configuration. Don't forget to add `from redis import StrictRedis` where the configuration is defined.
 
 - `redis_cache` The Redis cache configuration. Don't forget to add `from redis_cache import RedisCache` where the configuration is defined.
 
 
 
-Romain Thomas 2023
+Romain Thomas 2024
```

### Comparing `openalex-analysis-0.8.2/openalex_analysis/analysis/__init__.py` & `openalex-analysis-0.9.0/openalex_analysis/analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `openalex-analysis-0.8.2/openalex_analysis/analysis/entities_analysis.py` & `openalex-analysis-0.9.0/openalex_analysis/analysis/entities_analysis.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,20 @@
-# Romain THOMAS 2023
+# Romain THOMAS 2024
 # Stockholm Resilience Centre, Stockholm University
 
-import os, sys
+import os
 from os.path import exists, join # To check if a file exist
 import psutil
-import json
+import hashlib # to generate file names
 
 from tqdm import tqdm
 import pandas as pd
-import numpy as np
 import country_converter as coco
-from redis import StrictRedis
-from redis_cache import RedisCache
 import requests
 
-# sys.path.append(os.path.abspath('pyalex'))
 from pyalex import Works, Authors, Sources, Institutions, Concepts, Publishers, config
 
 from openalex_analysis.names import EntitieNames
 
 
 class AnalysisConfig(dict):
     """!
@@ -38,22 +34,14 @@
         @param      max_storage_percent       TODO
         @param      redis_parameters          TODO TO UPDATE DOC
     """
     def __getattr__(self, key):
         return super().__getitem__(key)
 
     def __setattr__(self, key, value):
-        # if key == 'redis_parameters':
-        #     print("coucou1")
-        #     if value != None:
-        #         print("coucou2")
-        #         super().__setitem__('redis_client', StrictRedis(value))
-        #         super().__setitem__('cache', RedisCache(redis_client=self.redis_client))
-        #         # redis_client = StrictRedis(**config.redis_parameters)
-        #         # cache = RedisCache(redis_client=redis_client)
         return super().__setitem__(key, value)
 
 
 config = AnalysisConfig(email=None,
                         api_key=None,
                         openalex_url="https://api.openalex.org",
                         allow_automatic_download = True,
@@ -69,39 +57,37 @@
 
 
 class EntitiesAnalysis(EntitieNames):
     """!
     OpenAlexAnalysis class which contains generic methods to do analysis over OpenAlex entities
     """
 
-    
-
     # to convert country code to country name
     cc = coco.CountryConverter()
 
-
     def __init__(self,
                  entitie_from_id = None,
                  extra_filters = None,
                  database_file_path = None,
                  create_dataframe = True,
                  entitie_name = None,
                  load_only_columns = None,
+                 # custom_query = None,
                 ):
         """!
         @param      entitie_from_id           The entitie identifier (eg an
                                               institution id) from which to take
                                               the entities (eg the works) to
                                               analyse (str)
-        @param      filters                   Optional additionnal filters,
+        @param      extra_filters             Optional additional filters,
                                               refer to the documentation of
                                               openalex and pyalex for the format
                                               (dict)
         @param      database_file_path        The database file path to force
-                                              the analyse over datas in a
+                                              the analysis over datas in a
                                               specific file (str)
         @param      create_dataframe          Create the dataframe at the
                                               initialisation (and download the
                                               data if needed and allowed)
         @param      entitie_name              To specify the name of the entitie
                                               to avoid downloading it via the
                                               API if needed
@@ -110,14 +96,15 @@
 
         self.entitie_from_id = entitie_from_id
         self.entitie_from_type = None
         self.extra_filters = extra_filters
         self.database_file_path = database_file_path
         self.entitie_name = entitie_name
         self.load_only_columns = load_only_columns
+        # self.custom_query = custom_query
 
         # dictionary containning for each concept a list of the entities linked to the concept
         # self.entities_concepts = {} # DEPRECATED
         # same than self.entities_concepts formated as a dataframe with extra informations
         # self.entities_concepts_df = {} # DEPRECATED
         # a dataframe containing entities related to the instance
         self.entities_df = None
@@ -140,21 +127,21 @@
         self.count_element_years = None
         self.count_entities_cols = []
 
         # maximum values for the storage usage (used to remove the databases)
         # self.max_storage_percent = max_storage_percent # it will delete databases if storage usage > max_storage_percent
 
         # initialize the values only if entitie_from_type is known
-        if self.entitie_from_id != None:
-            self.entitie_from_type = self.get_entitie_type_from_id(self.entitie_from_id)
+        if self.entitie_from_id != None or self.extra_filters != None:
+            if self.entitie_from_id != None:
+                self.entitie_from_type = self.get_entitie_type_from_id(self.entitie_from_id)
             if self.database_file_path == None:
                 self.database_file_path = join(config.project_datas_folder_path, self.get_database_file_name())
-
-        if entitie_from_id != None and create_dataframe == True:
-            self.load_entities_dataframe()
+            if create_dataframe == True:
+                self.load_entities_dataframe()
 
     def get_count_entities_matched(self, query_filters):
         """!
         @brief      Gets and return the number of entities which match the query
                     fitlers.
         
         @param      query_filters  The query filters (dict)
@@ -168,34 +155,41 @@
 
     def get_api_query(self):
         """!
         @brief      Gets the api query from the parameters of the instance
 
         @return     The api query (dict)
         """
-        query_filters = {self.get_entitie_string_name(self.entitie_from_type): {"id": self.entitie_from_id}}
-        # special cases:
-        # concept of institution as the query key word is x_concepts instead of concepts
-        if self.get_entitie_type_from_id() == Institutions and self.get_entitie_type_from_id(self.entitie_from_id) == Concepts:
-            query_filters = {'x_concepts': {"id": self.entitie_from_id}}
-        if self.get_entitie_type_from_id(self.entitie_from_id) == Authors:
-            query_filters = {'author': {"id": self.entitie_from_id}}
+        if self.entitie_from_id != None:
+            query_filters = {self.get_entitie_string_name(self.entitie_from_type): {"id": self.entitie_from_id}}
+            # special cases:
+            # concept of institution as the query key word is x_concepts instead of concepts
+            if self.get_entitie_type_from_id() == Institutions and self.get_entitie_type_from_id(self.entitie_from_id) == Concepts:
+                query_filters = {'x_concepts': {"id": self.entitie_from_id}}
+            if self.get_entitie_type_from_id(self.entitie_from_id) == Authors:
+                query_filters = {'author': {"id": self.entitie_from_id}}
+        else:
+            query_filters = {}
         if self.extra_filters != None:
             query_filters = query_filters | self.extra_filters
-            print("query:", query_filters)
+        print("query:", query_filters)
         return query_filters
 
 
     def download_list_entities(self):
         """!
         @brief      Downloads the entities which match the parameters of the
                     instance, and store the dataset as a parquet file
                 """
 
-        print("Downloading list of "+self.get_entitie_string_name()+" of the "+self.get_entitie_string_name(self.entitie_from_type)[0:-1]+" "+str(self.entitie_from_id))
+        print("Downloading list of "+self.get_entitie_string_name())
+        if self.entitie_from_id != None:
+             print("of the "+self.get_entitie_string_name(self.entitie_from_type)[0:-1]+" "+str(self.entitie_from_id))
+        if self.extra_filters != None:
+            print("with extra filters: "+str(self.extra_filters))
 
         query = self.get_api_query()
         print("Query to download from the API:", query)
 
         count_entities_matched = self.get_count_entities_matched(query)
 
         if config.n_max_entities == None or config.n_max_entities > count_entities_matched:
@@ -230,38 +224,41 @@
                     i += 1
                 # update the progress bar
                 pbar.update(self.per_page)
                 # update the progress percentage variable
                 self.entitie_downloading_progress_percentage = i/n_entities_to_download*100
         self.entitie_downloading_progress_percentage = 100
 
-        # sort the list by concept score
-        # Not working + useless?: entities_list = sorted(entities_list, key=lambda d: self.get_concept_score(d, concept), reverse=True)
-        
         # normalize the json format (one column for each field)
         print("Normalizing the json data downloaded...")
         entities_list_df = pd.json_normalize(entities_list)
         # We don't use multi index dataframe as plotly and dask doesn't support it and the use case is minor
         # # convert to multi index dataframe (we create an index for each 'subcolumn' (=when there is a '.'))
         # tuple_cols = entities_list_df.columns.str.split('.')
         # entities_list_df.columns = pd.MultiIndex.from_tuples(tuple(i) for i in tuple_cols)
+        if not os.path.isdir(config.project_datas_folder_path):
+            print("Creating the directory to store the datas from OpenAlex")
+            os.makedirs(config.project_datas_folder_path)
         print("Checking space left on disk...")
         self.auto_remove_databases_saved()
         # save as compressed parquet file
         print("Saving the list of entities as a parquet file...")
         entities_list_df.to_parquet(self.database_file_path, compression=config.parquet_compression)
 
 
     def load_entities_dataframe(self):
         """!
         @brief      Loads an entities dataset from file (or download it if needed and
                     allowed by the instance) to the dataframe of the instance
         """
-        print("Loading dataframe of "+self.get_entitie_string_name()+" of the "+self.get_entitie_string_name(self.entitie_from_type)[0:-1]+" "+self.entitie_from_id)
-        #print("Creating dataframe for entities (concept: "+self.concepts_normalized_names[concept]+")")
+        print("Loading dataframe of "+self.get_entitie_string_name())
+        if self.entitie_from_id != None:
+             print("of the "+self.get_entitie_string_name(self.entitie_from_type)[0:-1]+" "+str(self.entitie_from_id))
+        if self.extra_filters != None:
+            print("with extra filters: "+str(self.extra_filters))
 
         # # check if the database file exists
         if exists(self.database_file_path):
             # the database exists, we can load it
             pass
         elif config.allow_automatic_download == True:
             # the database doesn't exist and we can download the datas
@@ -299,30 +296,25 @@
 
 
     def get_df_filtered_entities_selection_threshold(self, df_filters):
         """!
         @brief      Gets df_filtered which contains the entities of self.entities_df
                     fitting the filters in df_filters
         
-        @param      df_filters  The filters in a dictionnary with for the key
+        @param      df_filters  The filters in a dictionary with for the key
                                 for the data to filter and for the value the
                                 minimum threshold (dict)
         
         @return     df_filtered, corresponding the the entities fitting the
                     thresholds (pandas DataFrame)
         """
         entities_df_filtered = self.entities_df
         for key_filter, value_filter in df_filters.items():
             entities_df_filtered = entities_df_filtered.loc[(entities_df_filtered[key_filter] >= value_filter)]
-        # # fitler for cited_by_threshold
-        # if cited_by_threshold != 0:
-        #     entities_df_filtered = entities_df_filtered.loc[(entities_df_filtered['works_cited_by_count_average'] >= cited_by_threshold)]
-        
-        #     if len(display_only_selected_entities):
-        #         entities_df_filtered = entities_df_filtered.loc[(entities_df_filtered[x_datas] >= x_threshold) & (entities_df_filtered[y_datas] >= y_threshold)]
+
         return entities_df_filtered
 
 
     def get_number_of_entities_selected(self, x_threshold, y_threshold, cited_by_threshold, x_datas, y_datas):
         """!
         @brief      Gets the number of entities selected on the plot
         
@@ -404,50 +396,52 @@
         
         @param      concepts_from  The concepts to use to calculate the combined
                                    concept score (list of str)
         """
         concept_links = ["https://openalex.org/"+item for item in concepts_from]
         self.entities_multi_filtered_df['average_combined_concepts_score'] = [self.get_sum_concept_scores(entitie, concept_links)/len(concepts_from) for index, entitie in self.entities_multi_filtered_df.iterrows()]
     
-    def get_database_file_name(self, entitie_from_id = None, entities_type = None, db_format = "parquet", extra_text = None):
+    def get_database_file_name(self, entitie_from_id = None, entities_type = None, db_format = "parquet"):
         """!
         @brief      Gets the database file name according to the parameters of the
                     ojbect or the arguments given.
-        
+
         @param      entitie_from_id  The identifier of the entitie (eg a concept
                                      id) which was used to filter the entities
                                      (eg works) in the database (str)
         @param      entities_type    The entities type in the database (eg
                                      works) (EntitieOpenAlex)
         @param      db_format        The database file format (str)
-        @param      extra_text       Extra text to add to the file name (str)
-        
+
         @return     The database file name (str)
         """
         if entitie_from_id == None:
             entitie_from_id = self.entitie_from_id
         if entities_type == None:
             entities_type = self.EntitieOpenAlex
-        file_name = self.get_entitie_string_name(entities_type)+"_"+self.get_entitie_string_name(self.get_entitie_type_from_id(entitie_from_id))[0:-1]+"_"+entitie_from_id
-        # if it's a concept, we add it's name to the file name (we can't do that for the other entitie type as
-        # the names can change. For the concept, all the names are known and saved locally in a csv file)
-        if self.get_entitie_type_from_id(entitie_from_id) == Concepts:
-            file_name += "_"+self.concepts_normalized_names[entitie_from_id].replace(' ', '_')
-        # temporary solution (can be problematic as database number can grow fast)
-        # add the hash value of filters if used
+        file_name = self.get_entitie_string_name(entities_type)
+        if entitie_from_id != None:
+            file_name += "_"+self.get_entitie_string_name(self.get_entitie_type_from_id(entitie_from_id))[0:-1]+"_"+entitie_from_id
+            # if it's a concept, we add it's name to the file name (we can't do that for the other entities type as
+            # the names can change. For the concept, all the names are known and saved locally in a parquet file)
+            # we don't add the concept name if there is more than one concept in the request (OR query with |)
+            if self.get_entitie_type_from_id(entitie_from_id) == Concepts and entitie_from_id.find('|') == -1:
+                file_name += "_"+self.concepts_normalized_names[entitie_from_id].replace(' ', '_')
         if self.extra_filters != None:
-            # hash not working accross class instances
-            #file_name += "_"+str(abs(hash(json.dumps(self.extra_filters, sort_keys=True))))
-            # Can be a problem in case of many filters as file names are limited to 255 char
             file_name += "_" + str(self.extra_filters).replace("'", '').replace(":", '').replace(' ', '_')
+        # keep the file name below 120 characters and reserve 22 for the max size + parquet extension (csv extension
+        # is shorter)
+        if len(file_name) > 98:
+            # sha224 length: 56
+            file_name = file_name[:41] + "-" + hashlib.sha224(file_name.encode()).hexdigest()
         file_name += "_max_"+str(config.n_max_entities)
-        if extra_text != None:
-            file_name += "_" + extra_text
+        # add warning for nb max entities to large (>9 999 999 999) because of file name
         return file_name+"."+db_format
 
+    # TODO: rename function to get_entitie_type_string_name
     def get_entitie_string_name(self, entitie = None):
         """!
         @brief      Gets the entitie type string name.
         
         @param      entitie  The entitie, if not provided, the instance entitie
                              id will be used (BaseOpenAlex)
         
@@ -478,26 +472,31 @@
         @param      allow_download_from_API  Allow to download the entitie name
                                              from the OpenAlex API (bool)
         
         @return     The name of entitie (str)
         """
         if entitie == None:
             entitie = self.entitie_from_id
+            # if entitie is None then we return None
+            if entitie == None:
+                return None
         # if the entitie name asked is the one of the current instance and it was provided in the initialisation
         if entitie == self.entitie_from_id and self.entitie_name != None:
             return self.entitie_name
         elif allow_download_from_API:
             return get_name_of_entitie_from_api(entitie)
         else:
             raise ValueError("Can't get the entitie name because not allowed to download from API and not provided at the initialisation")
 
 
     def get_info_about_entitie(self, entitie, infos = ["display_name"], return_as_pd_serie = True, allow_download_from_API = True):
         if entitie == None:
             entitie = self.entitie_from_id
+            if entitie == None:
+                raise ValueError("Can't get the entitie info of None")
         if allow_download_from_API:
             return get_info_about_entitie_from_api(entitie, infos = infos, return_as_pd_serie = return_as_pd_serie)
         else:
             raise ValueError("Can't get the entitie info because not allowed to download from API")
 
 
 
@@ -535,36 +534,29 @@
 
     @return     The name of entitie (str)
     """
     # call the API
     e = get_entitie_type_from_id(entitie)()[entitie]
     return e['display_name']
 
-# @config.cache.cache()
-# def get_name_of_entitie_from_api_cache(entitie):
-#     print("Getting name of "+entitie+" from the OpenAlex API (not found in cache)...")
-#     return get_info_about_entitie_from_api_core(entitie)
-
-# def get_name_of_entitie_from_api_no_cache(entitie):
-    # print("Getting name of "+entitie+" from the OpenAlex API (cache disabled)...")
-    # return get_info_about_entitie_from_api_core(entitie)
 
 def get_name_of_entitie_from_api(entitie):
     # if config.redis_parameters != None:
     #     return get_name_of_entitie_from_api_cache(entitie)
     # else:
     #     return get_name_of_entitie_from_api_no_cache(entitie)
     if config.redis_enabled == True:
         print("Getting name of "+entitie+" from the OpenAlex API (cache enabled)...")
         get_name_of_entitie_from_api_core_cached = config.redis_cache.cache()(get_name_of_entitie_from_api_core)
         return get_name_of_entitie_from_api_core_cached(entitie)
     else:
         print("Getting name of "+entitie+" from the OpenAlex API (cache disabled)...")
         return get_name_of_entitie_from_api_core(entitie)
 
+
 def extract_authorships_citation_style(authorships):
     if len(authorships) == 0:
         res = "Unknown author"
     if len(authorships) >= 1:
         res = authorships[0]['author']['display_name']
     if len(authorships) >= 2:
         res += ", "+authorships[1]['author']['display_name']
@@ -586,23 +578,14 @@
     e = get_entitie_type_from_id(entitie)()[entitie]
     if "author_citation_style" in infos:
         e["author_citation_style"] = extract_authorships_citation_style(e["authorships"])
     e = {key: val for key, val in e.items() if key in infos}
     return e
 
 
-# @config.cache.cache()
-# def get_info_about_entitie_from_api_cache(entitie, infos = ["display_name"]):
-#     print("Getting information about "+entitie+" from the OpenAlex API (not found in cache)...")
-#     return get_info_about_entitie_from_api_core(entitie, infos = infos)
-
-# def get_info_about_entitie_from_api_no_cache(entitie, infos = ["display_name"]):
-#     print("Getting information about "+entitie+" from the OpenAlex API (cahe disabled)...")
-#     return get_info_about_entitie_from_api_core(entitie, infos = infos)
-
 def get_info_about_entitie_from_api(entitie, infos = ["display_name"], return_as_pd_serie = True):
     # if config.redis_parameters != None:
     #     res = get_info_about_entitie_from_api_cache(entitie, infos = infos)
     # else:
     #     res = get_info_about_entitie_from_api_no_cache(entitie, infos = infos)
     if config.redis_enabled == True:
         print("Getting information about "+entitie+" from the OpenAlex API (cache enabled)...")
@@ -640,15 +623,16 @@
     if config.redis_enabled == True:
         print("Checking if "+entitie+" exists (cache enabled)...")
         check_if_entity_exists_core_cached = config.redis_cache.cache()(check_if_entity_exists_core)
         return check_if_entity_exists_core_cached(entitie)
     else:
         print("Checking if "+entitie+" exists (cache disabled)...")
         return check_if_entity_exists_core(entitie)
-        
+
+
 class WorksAnalysis(EntitiesAnalysis, Works):
     """!
     @brief      This class contains specific methods for Works concepts analysis.
     """
     EntitieOpenAlex = Works
     def filter_and_format_entitie_data_from_api_response(self, entitie):
         """!
@@ -656,16 +640,15 @@
         
         @param      entitie  The works data from the API (dict)
         
         @return     The works datas (dict)
         """
         # # transform datas
         # # abstract
-        # disabled for now
-        # entitie['extracted_abstract'] = entitie['abstract']
+        entitie['extracted_abstract'] = entitie['abstract']
 
         # delete useless datas
         # for now storing the abstract_inverted_index isn't possible because if expand in the dataframe
         # and makes it too big --> storing full abstract
         del entitie['abstract_inverted_index']
         
         # add computed datas:
@@ -714,15 +697,15 @@
     
     def get_works_references_count(self, count_years = []):
         """!
         @brief      Gets the works references count of the works list of the instance
         
         @return     The works references count (pandas Serie)
         """
-        print("Creating the works references count of "+self.get_entitie_string_name()+" "+self.entitie_from_id+"...")
+        print("Creating the works references count of "+self.get_entitie_string_name()+"...")
         if count_years == []:
             return self.entities_df['referenced_works'].explode().value_counts().convert_dtypes()
         else:
             counts_df_list = [None] * len(count_years)
             for i, year in enumerate(count_years):
                 counts_df_list[i] = self.entities_df[self.entities_df.publication_year == year]['referenced_works'].explode().value_counts().convert_dtypes()
             entities_count = pd.concat(counts_df_list, axis=1, keys=count_years).reset_index().fillna(0)
@@ -737,33 +720,28 @@
         
         @param      count_only_year  If different than None, count only the
                                      concepts of the works of the given year
                                      (int)
         
         @return     The concept count (pandas Serie)
         """
-        print("Creating the concept count of "+self.get_entitie_string_name()+" "+self.entitie_from_id+"...")
+        print("Creating the concept count of "+self.get_entitie_string_name()+"...")
         if count_years == []:
             return self.entities_df['concepts'].explode().apply(lambda c: c['id'] if type(c) == dict else None).value_counts().convert_dtypes()
         else:
             counts_df_list = [None] * len(count_years)
             for i, year in enumerate(count_years):
                 counts_df_list[i] = self.entities_df[self.entities_df.publication_year == year]['concepts'].explode().apply(lambda c: c['id'] if type(c) == dict else None).value_counts().convert_dtypes()
             entities_count = pd.concat(counts_df_list, axis=1, keys=count_years).reset_index().fillna(0)
             entities_count = entities_count.set_index('concepts').stack()
             entities_count.name = 'count'
             return entities_count
 
 
     def get_element_count(self, element_type, count_years = []):
-        # entities_to_count_df = None
-        # if count_only_year == None:
-        #     entities_to_count_df = self.entities_df
-        # else:
-        #     entities_to_count_df = self.entities_df[self.entities_df.publication_year == count_only_year]
         match element_type:
             case 'reference':
                 return self.get_works_references_count(count_years = count_years)
             case 'concept':
                 return self.get_works_concepts_count(count_years = count_years)
             case _:
                 raise ValueError("Can only count for 'references' or 'concept'")
@@ -974,16 +952,152 @@
 
         df_authors = df_authors.drop_duplicates('author.id')
         df_authors = df_authors.set_index('author.id')
 
         authors_count = pd.merge(authors_count, df_authors, how='left', left_index=True, right_index=True).reset_index()
 
         return authors_count[cols]
+
+
+    def count_yearly_entity_usage(self, entity: str, count_years: list) -> list:
+        """!
+        @brief      Counts the yearly number of time the entity is used.
+
+        @param      entity       The entity to count
+        @param      count_years  The years for which we need to count the entity
+
+        @return     Number of time the entity is used on a yearly basis.
+        """
+        entity_link = "https://openalex.org/"+entity
+        count_res = [None] * len(count_years)
+        for i, year in enumerate(count_years):
+            # get the list of works from the year
+            df = self.entities_df.loc[self.entities_df['publication_year'] == year]
+            if self.get_entitie_type_from_id(entity) == Concepts:
+                # get a dataframe with all the concepts used during the year in the column id
+                df = pd.json_normalize(df['concepts'].explode().to_list())
+            elif self.get_entitie_type_from_id(entity) == Works:
+                # get a dataframe with all the works used during the year in the column id
+                df = pd.DataFrame({'id':df['referenced_works'].explode().dropna()})
+            else:
+                raise ValueError("Entity type not supported")
+            if df.empty:
+                count_res[i] = 0
+            else:
+                # count the concept usage
+                count = pd.DataFrame(df.value_counts('id'))
+                count_res[i] = count['count'].get(entity_link, 0)
+                #count_res[i] = count.loc[concept]['count']
+        return count_res
+
+
+    def count_yearly_works(self, count_years: list) -> list:
+        """!
+        @brief      Return the number of works present per year in entities_df
+        
+        @param      count_years  The years for which we need to count the works
         
+        @return     Number of yearly works.
+        """
+        count_res = [None] * len(count_years)
+        for i, year in enumerate(count_years):
+            # get the list of works from the year
+            df = self.entities_df.loc[self.entities_df['publication_year'] == year]
+            if df.empty:
+                count_res[i] = 0
+            else:
+                # get the number of rows
+                count_res[i] = len(df.index)
+        return count_res
+
+
+    def get_df_yearly_usage_of_entities(self,
+                                        count_years: list,
+                                        entity_used_ids,
+                                        entity_from_legend = "Custom dataset"
+                                       ) -> pd.DataFrame:
+        """!
+        @brief      Gets the dataframe with the yearly usage by works of
+                    entity_used_ids.
+        
+        @param      count_years      The years for which we need to count the
+                                     entity
+        @param      entity_used_ids  The entity ids to count (str or str[])
+
+        @param      entity_from_legend    The legend on the plot for the entity_from dataset
+        
+        @return     The df yearly usage by works.
+        """    
+        if not isinstance(entity_used_ids, list):
+            entity_used_ids = [entity_used_ids]
+        if entity_from_legend == "Custom dataset" and self.entitie_from_id is not None:
+            entity_from_legend = self.entitie_from_id
+        df = pd.DataFrame()
+        for entity_used_id in entity_used_ids:
+            # count
+            usage_count = self.count_yearly_entity_usage(entity_used_id, count_years)
+            works_count = self.count_yearly_works(count_years)
+            entity_used_id_list = [entity_used_id] * len(count_years)
+            entity_from_list = [entity_from_legend] * len(count_years)
+
+            # create the dataframe
+            zipped_data = list(zip(count_years,
+                                   usage_count,
+                                   works_count,
+                                   entity_used_id_list,
+                                   entity_from_list))
+            
+            df_i = pd.DataFrame(zipped_data, columns=['years',
+                                               'usage_count',
+                                               'works_count',
+                                               'entity_used',
+                                               'entity_from',
+                                              ])
+
+            df = pd.concat([df, df_i])
+
+        return df
+
+
+    def get_df_yearly_usage_of_entities_by_multiples_entities(self,
+                                                              count_years: list,
+                                                              entity_used_ids,
+                                                              entity_from_ids = None,
+                                                             ) -> pd.DataFrame:
+        """!
+        @brief      Gets the dataframe with the yearly usage by works of
+                    entity_used_ids, works for multiple entities from.
+        
+        @param      count_years      The years for which we need to count the
+                                     entity
+        @param      entity_used_ids  The entity ids to count (str or str[])
+        @param      entity_from_ids  The entity from identifiers
+         
+        @return     The df yearly usage by works.
+        """
+        if entity_from_ids is None:
+            entity_from_ids = self.entitie_from_id
+            if entity_from_ids is None:
+                raise ValueError("entity_from_ids not provided and entities_from_id is None. You must provide either entitie_from_id to the class or entity_from_ids to the function")
+
+        if not isinstance(entity_from_ids, list):
+            entity_from_ids = [entity_from_ids]
+
+        df = pd.DataFrame()
+
+        for entity_from_id in entity_from_ids:
+            work_analysis = WorksAnalysis(entity_from_id)
+            df = pd.concat([
+                df,
+                work_analysis.get_df_yearly_usage_of_entities(count_years = count_years,
+                                                              entity_used_ids = entity_used_ids,
+                                                             )
+            ])
 
+        return df
 
 
 class AuthorsAnalysis(EntitiesAnalysis, Authors):
     EntitieOpenAlex = Authors
     
 
 class SourcesAnalysis(EntitiesAnalysis, Sources):
```

### Comparing `openalex-analysis-0.8.2/openalex_analysis/names/entitie_names.py` & `openalex-analysis-0.9.0/openalex_analysis/names/entitie_names.py`

 * *Files identical despite different names*

### Comparing `openalex-analysis-0.8.2/openalex_analysis/names/list_all_concepts.parquet` & `openalex-analysis-0.9.0/openalex_analysis/names/list_all_concepts.parquet`

 * *Files identical despite different names*

### Comparing `openalex-analysis-0.8.2/openalex_analysis/names/list_all_institutions.parquet` & `openalex-analysis-0.9.0/openalex_analysis/names/list_all_institutions.parquet`

 * *Files identical despite different names*

### Comparing `openalex-analysis-0.8.2/openalex_analysis/plot/__init__.py` & `openalex-analysis-0.9.0/openalex_analysis/plot/__init__.py`

 * *Files identical despite different names*

### Comparing `openalex-analysis-0.8.2/openalex_analysis/plot/entities_plot.py` & `openalex-analysis-0.9.0/openalex_analysis/plot/entities_plot.py`

 * *Files 8% similar despite different names*

```diff
@@ -323,14 +323,85 @@
                       log_x=True,
                       labels={'x':'Element rank', 'y':'Number of time used'},
                       title="Number of time the same element is used by the works in "+self.get_name_of_entitie(),
                       line_shape='hv')
         return fig
 
 
+    def get_figure_entities_yearly_usage(self,
+                                         count_years: list,
+                                         entity_used_ids,
+                                         entity_from_ids = None,
+                                        ):
+        """!
+        @brief      Gets the plot bar figure with the yearly usage of an entity
+                    (concept, work) in the works from another entitiy (institution,
+                    author)
+        
+        @param      count_years     The years to count (list of int)
+        @param      entity_used_ids The entities used (str or str[])
+        @param      entity_from_ids The entities which used the entities to count (str or str[])
+        
+        @return     The figure (fig)
+        """
+
+        df = self.get_df_yearly_usage_of_entities_by_multiples_entities(
+                                                                        count_years = count_years,
+                                                                        entity_used_ids = entity_used_ids,
+                                                                        entity_from_ids = entity_from_ids,
+                                                                       )
+
+        fig = px.bar(df,
+                      x='years',
+                      y='usage_count',
+                      color='entity_from',
+                      pattern_shape='entity_used',
+                      barmode='group',
+                      height=600,
+                     )
+        
+        return fig
+
+
+    def get_figure_entities_yearly_position(self,
+                                            count_years: list,
+                                            entity_used_ids: str,
+                                            entity_from_ids = None,
+                                           ):
+        """!
+        @brief      Gets the plot figure with the yearly usage of an entity (concept,
+                    work) in the works from another entitiy (institution, author)
+        
+        @param      count_years     The years to count (list of int)
+        @param      entity_used_id  The entity used (str)
+        @param      entity_from_ids The entities which used the entities to count (str or str[])
+        
+        @return     The figure (fig)
+        """
+
+        df = self.get_df_yearly_usage_of_entities_by_multiples_entities(
+                                                                        count_years = count_years,
+                                                                        entity_used_ids = entity_used_ids,
+                                                                        entity_from_ids = entity_from_ids,
+                                                                       )
+        
+        fig = px.line(df,
+                      x='works_count',
+                      y='usage_count',
+                      text='years',
+                      color='entity_from',
+                      line_dash='entity_used',
+                      height=600,
+                     )
+        
+        fig.update_traces(textposition="bottom right")
+
+        return fig
+
+
 class AuthorsPlot(EntitiesPlot, AuthorsAnalysis):
     pass
 
 
 class SourcesPlot(EntitiesPlot, SourcesAnalysis):
     pass
```

### Comparing `openalex-analysis-0.8.2/openalex_analysis.egg-info/PKG-INFO` & `openalex-analysis-0.9.0/openalex_analysis.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openalex-analysis
-Version: 0.8.2
+Version: 0.9.0
 Summary: A python library to analyse articles, institutions, and others entities from the OpenAlex API
 Author-email: Romain Thomas <romain.thomas@su.se>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -914,8 +914,8 @@
 
 - `redis_client` The Redis client configuration. Don't forget to add `from redis import StrictRedis` where the configuration is defined.
 
 - `redis_cache` The Redis cache configuration. Don't forget to add `from redis_cache import RedisCache` where the configuration is defined.
 
 
 
-Romain Thomas 2023
+Romain Thomas 2024
```

### Comparing `openalex-analysis-0.8.2/openalex_analysis.egg-info/SOURCES.txt` & `openalex-analysis-0.9.0/openalex_analysis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openalex-analysis-0.8.2/pyproject.toml` & `openalex-analysis-0.9.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=65", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "openalex-analysis"
-version = "0.8.2"
+version = "0.9.0"
 description = "A python library to analyse articles, institutions, and others entities from the OpenAlex API"
 readme = "README.md"
 authors = [{ name = "Romain Thomas", email = "romain.thomas@su.se" }]
 license = { file = "LICENCE.txt" }
 classifiers = [
     "Development Status :: 3 - Alpha",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
```

