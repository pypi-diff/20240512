# Comparing `tmp/QuantileClient-0.3.tar.gz` & `tmp/QuantileClient-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "QuantileClient-0.3.tar", last modified: Thu May  2 14:20:06 2024, max compression
+gzip compressed data, was "QuantileClient-0.4.tar", last modified: Sun May 12 18:38:26 2024, max compression
```

## Comparing `QuantileClient-0.3.tar` & `QuantileClient-0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 aryanrajpurohit   (501) staff       (20)        0 2024-05-02 14:20:06.742400 QuantileClient-0.3/
--rw-r--r--   0 aryanrajpurohit   (501) staff       (20)     4447 2024-05-02 14:20:06.740938 QuantileClient-0.3/PKG-INFO
-drwxr-xr-x   0 aryanrajpurohit   (501) staff       (20)        0 2024-05-02 14:20:06.730940 QuantileClient-0.3/QuantileClient/
--rw-r--r--   0 aryanrajpurohit   (501) staff       (20)       32 2024-03-24 20:48:45.000000 QuantileClient-0.3/QuantileClient/__init__.py
--rw-r--r--   0 aryanrajpurohit   (501) staff       (20)     6912 2024-05-02 13:30:35.000000 QuantileClient-0.3/QuantileClient/main.py
-drwxr-xr-x   0 aryanrajpurohit   (501) staff       (20)        0 2024-05-02 14:20:06.739765 QuantileClient-0.3/QuantileClient.egg-info/
--rw-r--r--   0 aryanrajpurohit   (501) staff       (20)     4447 2024-05-02 14:20:06.000000 QuantileClient-0.3/QuantileClient.egg-info/PKG-INFO
--rw-r--r--   0 aryanrajpurohit   (501) staff       (20)      257 2024-05-02 14:20:06.000000 QuantileClient-0.3/QuantileClient.egg-info/SOURCES.txt
--rw-r--r--   0 aryanrajpurohit   (501) staff       (20)        1 2024-05-02 14:20:06.000000 QuantileClient-0.3/QuantileClient.egg-info/dependency_links.txt
--rw-r--r--   0 aryanrajpurohit   (501) staff       (20)       23 2024-05-02 14:20:06.000000 QuantileClient-0.3/QuantileClient.egg-info/requires.txt
--rw-r--r--   0 aryanrajpurohit   (501) staff       (20)       15 2024-05-02 14:20:06.000000 QuantileClient-0.3/QuantileClient.egg-info/top_level.txt
--rw-r--r--   0 aryanrajpurohit   (501) staff       (20)     4108 2024-05-02 14:17:20.000000 QuantileClient-0.3/README.md
--rw-r--r--   0 aryanrajpurohit   (501) staff       (20)       38 2024-05-02 14:20:06.742680 QuantileClient-0.3/setup.cfg
--rw-r--r--   0 aryanrajpurohit   (501) staff       (20)      519 2024-05-02 14:19:00.000000 QuantileClient-0.3/setup.py
+drwxr-xr-x   0 aryanrajpurohit   (501) staff       (20)        0 2024-05-12 18:38:26.783042 QuantileClient-0.4/
+-rw-r--r--   0 aryanrajpurohit   (501) staff       (20)     4447 2024-05-12 18:38:26.782368 QuantileClient-0.4/PKG-INFO
+drwxr-xr-x   0 aryanrajpurohit   (501) staff       (20)        0 2024-05-12 18:38:26.778169 QuantileClient-0.4/QuantileClient/
+-rw-r--r--   0 aryanrajpurohit   (501) staff       (20)       32 2024-03-24 20:48:45.000000 QuantileClient-0.4/QuantileClient/__init__.py
+-rw-r--r--   0 aryanrajpurohit   (501) staff       (20)     6992 2024-05-12 18:22:05.000000 QuantileClient-0.4/QuantileClient/main.py
+drwxr-xr-x   0 aryanrajpurohit   (501) staff       (20)        0 2024-05-12 18:38:26.781819 QuantileClient-0.4/QuantileClient.egg-info/
+-rw-r--r--   0 aryanrajpurohit   (501) staff       (20)     4447 2024-05-12 18:38:26.000000 QuantileClient-0.4/QuantileClient.egg-info/PKG-INFO
+-rw-r--r--   0 aryanrajpurohit   (501) staff       (20)      257 2024-05-12 18:38:26.000000 QuantileClient-0.4/QuantileClient.egg-info/SOURCES.txt
+-rw-r--r--   0 aryanrajpurohit   (501) staff       (20)        1 2024-05-12 18:38:26.000000 QuantileClient-0.4/QuantileClient.egg-info/dependency_links.txt
+-rw-r--r--   0 aryanrajpurohit   (501) staff       (20)       23 2024-05-12 18:38:26.000000 QuantileClient-0.4/QuantileClient.egg-info/requires.txt
+-rw-r--r--   0 aryanrajpurohit   (501) staff       (20)       15 2024-05-12 18:38:26.000000 QuantileClient-0.4/QuantileClient.egg-info/top_level.txt
+-rw-r--r--   0 aryanrajpurohit   (501) staff       (20)     4108 2024-05-02 14:17:20.000000 QuantileClient-0.4/README.md
+-rw-r--r--   0 aryanrajpurohit   (501) staff       (20)       38 2024-05-12 18:38:26.783156 QuantileClient-0.4/setup.cfg
+-rw-r--r--   0 aryanrajpurohit   (501) staff       (20)      519 2024-05-12 18:36:08.000000 QuantileClient-0.4/setup.py
```

### Comparing `QuantileClient-0.3/PKG-INFO` & `QuantileClient-0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QuantileClient
-Version: 0.3
+Version: 0.4
 Summary: Its a wrapper lib from quantile ai api service
 Home-page: https://github.com/Quantileaidev/QuantileClientLib
 Author: QuantileaiDev
 Author-email: quantileai@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 Requires-Dist: python-dotenv
```

### Comparing `QuantileClient-0.3/QuantileClient/main.py` & `QuantileClient-0.4/QuantileClient/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -169,28 +169,30 @@
             return {"error": "File not found"}
         
         with open(pdf_file, 'rb') as file:
             files = {'pdf_file': (os.path.basename(pdf_file), file)}
             response = requests.post(url, headers=headers, params=params, files=files)
         
         return response.json()
-    def rag_chat(self,db_name,description,question,embedding_model="text-embedding-3-small",inference_model="gpt-3.5-turbo-0125",temperature=0):
+    def rag_chat(self,db_name,description,question,embedding_model="text-embedding-3-small",inference_model="gpt-3.5-turbo-0125",temperature=0,max_token:int=500,k:int=1):
         url = f"{self.base_url}/rag_assistant"
         
         headers = {
             "accept": "application/json",
             "quant-api-key": self.api_key
         }
         params = {
             "db_name": db_name,
             "description": description,
             "question": question,
             "embedding_model": embedding_model,
             "inference_model": inference_model,
-            "temperature": temperature
+            "temperature": temperature,
+            "max_token":max_token,
+            "k":k
         }
         
         response = requests.get(url, headers=headers, params=params)
         return response.json()
```

### Comparing `QuantileClient-0.3/QuantileClient.egg-info/PKG-INFO` & `QuantileClient-0.4/QuantileClient.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QuantileClient
-Version: 0.3
+Version: 0.4
 Summary: Its a wrapper lib from quantile ai api service
 Home-page: https://github.com/Quantileaidev/QuantileClientLib
 Author: QuantileaiDev
 Author-email: quantileai@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 Requires-Dist: python-dotenv
```

### Comparing `QuantileClient-0.3/README.md` & `QuantileClient-0.4/README.md`

 * *Files identical despite different names*

### Comparing `QuantileClient-0.3/setup.py` & `QuantileClient-0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='QuantileClient',
-    version='0.3',
+    version='0.4',
     packages=find_packages(),
     install_requires=[
         'python-dotenv',
         'requests',
     ],
     author='QuantileaiDev',
     author_email='quantileai@gmail.com',
```

