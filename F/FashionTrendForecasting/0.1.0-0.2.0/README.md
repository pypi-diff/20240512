# Comparing `tmp/FashionTrendForecasting-0.1.0.tar.gz` & `tmp/fashiontrendforecasting-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FashionTrendForecasting-0.1.0.tar", last modified: Sat May 11 20:21:20 2024, max compression
+gzip compressed data, was "fashiontrendforecasting-0.2.0.tar", last modified: Sun May 12 00:31:30 2024, max compression
```

## Comparing `FashionTrendForecasting-0.1.0.tar` & `fashiontrendforecasting-0.2.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 inesa      (501) staff       (20)        0 2024-05-11 20:21:20.502327 FashionTrendForecasting-0.1.0/
-drwxr-xr-x   0 inesa      (501) staff       (20)        0 2024-05-11 20:21:20.500064 FashionTrendForecasting-0.1.0/FashionTrendForecasting/
--rw-rw-r--   0 inesa      (501) staff       (20)      104 2024-05-11 17:32:43.000000 FashionTrendForecasting-0.1.0/FashionTrendForecasting/__init__.py
-drwxr-xr-x   0 inesa      (501) staff       (20)        0 2024-05-11 20:21:20.500771 FashionTrendForecasting-0.1.0/FashionTrendForecasting/api/
--rw-rw-r--   0 inesa      (501) staff       (20)        0 2024-05-11 17:32:43.000000 FashionTrendForecasting-0.1.0/FashionTrendForecasting/api/__init__.py
--rw-rw-r--   0 inesa      (501) staff       (20)      443 2024-05-11 17:32:43.000000 FashionTrendForecasting-0.1.0/FashionTrendForecasting/api/main.py
-drwxr-xr-x   0 inesa      (501) staff       (20)        0 2024-05-11 20:21:20.501071 FashionTrendForecasting-0.1.0/FashionTrendForecasting/data_processing/
--rw-rw-r--   0 inesa      (501) staff       (20)       55 2024-05-11 17:32:43.000000 FashionTrendForecasting-0.1.0/FashionTrendForecasting/data_processing/__init__.py
--rw-rw-r--   0 inesa      (501) staff       (20)      783 2024-05-11 17:32:43.000000 FashionTrendForecasting-0.1.0/FashionTrendForecasting/data_processing/insert_data.py
--rw-rw-r--   0 inesa      (501) staff       (20)    11265 2024-05-11 17:32:43.000000 FashionTrendForecasting-0.1.0/FashionTrendForecasting/data_processing/sql_interactions.py
-drwxr-xr-x   0 inesa      (501) staff       (20)        0 2024-05-11 20:21:20.501449 FashionTrendForecasting-0.1.0/FashionTrendForecasting/trend_analysis/
--rw-rw-r--   0 inesa      (501) staff       (20)     3463 2024-05-11 17:32:43.000000 FashionTrendForecasting-0.1.0/FashionTrendForecasting/trend_analysis/Simple_Model.py
--rw-rw-r--   0 inesa      (501) staff       (20)      105 2024-05-11 17:32:43.000000 FashionTrendForecasting-0.1.0/FashionTrendForecasting/trend_analysis/__init__.py
--rw-rw-r--   0 inesa      (501) staff       (20)     2889 2024-05-11 17:32:43.000000 FashionTrendForecasting-0.1.0/FashionTrendForecasting/trend_analysis/model.py
-drwxr-xr-x   0 inesa      (501) staff       (20)        0 2024-05-11 20:21:20.500611 FashionTrendForecasting-0.1.0/FashionTrendForecasting.egg-info/
--rw-r--r--   0 inesa      (501) staff       (20)     4502 2024-05-11 20:21:20.000000 FashionTrendForecasting-0.1.0/FashionTrendForecasting.egg-info/PKG-INFO
--rw-r--r--   0 inesa      (501) staff       (20)      747 2024-05-11 20:21:20.000000 FashionTrendForecasting-0.1.0/FashionTrendForecasting.egg-info/SOURCES.txt
--rw-r--r--   0 inesa      (501) staff       (20)        1 2024-05-11 20:21:20.000000 FashionTrendForecasting-0.1.0/FashionTrendForecasting.egg-info/dependency_links.txt
--rw-r--r--   0 inesa      (501) staff       (20)     2344 2024-05-11 20:21:20.000000 FashionTrendForecasting-0.1.0/FashionTrendForecasting.egg-info/requires.txt
--rw-r--r--   0 inesa      (501) staff       (20)       24 2024-05-11 20:21:20.000000 FashionTrendForecasting-0.1.0/FashionTrendForecasting.egg-info/top_level.txt
--rw-rw-r--   0 inesa      (501) staff       (20)     1063 2024-05-11 17:32:43.000000 FashionTrendForecasting-0.1.0/LICENSE
--rw-r--r--   0 inesa      (501) staff       (20)     4502 2024-05-11 20:21:20.502135 FashionTrendForecasting-0.1.0/PKG-INFO
--rw-rw-r--   0 inesa      (501) staff       (20)     1906 2024-05-11 17:32:43.000000 FashionTrendForecasting-0.1.0/README.md
--rw-r--r--   0 inesa      (501) staff       (20)       38 2024-05-11 20:21:20.502361 FashionTrendForecasting-0.1.0/setup.cfg
--rw-rw-r--   0 inesa      (501) staff       (20)     4253 2024-05-11 17:32:43.000000 FashionTrendForecasting-0.1.0/setup.py
-drwxr-xr-x   0 inesa      (501) staff       (20)        0 2024-05-11 20:21:20.501654 FashionTrendForecasting-0.1.0/tests/
--rw-rw-r--   0 inesa      (501) staff       (20)     1503 2024-05-11 17:32:43.000000 FashionTrendForecasting-0.1.0/tests/test_prediction.py
--rw-rw-r--   0 inesa      (501) staff       (20)      535 2024-05-11 17:32:43.000000 FashionTrendForecasting-0.1.0/tests/test_trend_analysis.py
+drwxr-xr-x   0 sateantaranyan   (501) staff       (20)        0 2024-05-12 00:31:30.903890 fashiontrendforecasting-0.2.0/
+drwxr-xr-x   0 sateantaranyan   (501) staff       (20)        0 2024-05-12 00:31:30.896594 fashiontrendforecasting-0.2.0/FashionTrendForecasting/
+-rw-r--r--   0 sateantaranyan   (501) staff       (20)      104 2024-05-11 13:27:18.000000 fashiontrendforecasting-0.2.0/FashionTrendForecasting/__init__.py
+drwxr-xr-x   0 sateantaranyan   (501) staff       (20)        0 2024-05-12 00:31:30.897603 fashiontrendforecasting-0.2.0/FashionTrendForecasting/api/
+-rw-r--r--   0 sateantaranyan   (501) staff       (20)        0 2024-05-11 13:27:18.000000 fashiontrendforecasting-0.2.0/FashionTrendForecasting/api/__init__.py
+-rw-r--r--   0 sateantaranyan   (501) staff       (20)      443 2024-05-11 13:27:18.000000 fashiontrendforecasting-0.2.0/FashionTrendForecasting/api/main.py
+drwxr-xr-x   0 sateantaranyan   (501) staff       (20)        0 2024-05-12 00:31:30.898441 fashiontrendforecasting-0.2.0/FashionTrendForecasting/data_processing/
+-rw-r--r--   0 sateantaranyan   (501) staff       (20)       55 2024-05-11 13:27:18.000000 fashiontrendforecasting-0.2.0/FashionTrendForecasting/data_processing/__init__.py
+-rw-r--r--   0 sateantaranyan   (501) staff       (20)      783 2024-05-11 13:27:18.000000 fashiontrendforecasting-0.2.0/FashionTrendForecasting/data_processing/insert_data.py
+-rw-r--r--   0 sateantaranyan   (501) staff       (20)    11265 2024-05-11 13:27:18.000000 fashiontrendforecasting-0.2.0/FashionTrendForecasting/data_processing/sql_interactions.py
+drwxr-xr-x   0 sateantaranyan   (501) staff       (20)        0 2024-05-12 00:31:30.899150 fashiontrendforecasting-0.2.0/FashionTrendForecasting/trend_analysis/
+-rw-r--r--   0 sateantaranyan   (501) staff       (20)     3463 2024-05-11 13:27:18.000000 fashiontrendforecasting-0.2.0/FashionTrendForecasting/trend_analysis/Simple_Model.py
+-rw-r--r--   0 sateantaranyan   (501) staff       (20)      105 2024-05-11 13:27:18.000000 fashiontrendforecasting-0.2.0/FashionTrendForecasting/trend_analysis/__init__.py
+-rw-r--r--   0 sateantaranyan   (501) staff       (20)     2889 2024-05-11 13:27:18.000000 fashiontrendforecasting-0.2.0/FashionTrendForecasting/trend_analysis/model.py
+drwxr-xr-x   0 sateantaranyan   (501) staff       (20)        0 2024-05-12 00:31:30.899908 fashiontrendforecasting-0.2.0/FashionTrendForecasting.egg-info/
+-rw-r--r--   0 sateantaranyan   (501) staff       (20)     4686 2024-05-12 00:31:30.000000 fashiontrendforecasting-0.2.0/FashionTrendForecasting.egg-info/PKG-INFO
+-rw-r--r--   0 sateantaranyan   (501) staff       (20)      747 2024-05-12 00:31:30.000000 fashiontrendforecasting-0.2.0/FashionTrendForecasting.egg-info/SOURCES.txt
+-rw-r--r--   0 sateantaranyan   (501) staff       (20)        1 2024-05-12 00:31:30.000000 fashiontrendforecasting-0.2.0/FashionTrendForecasting.egg-info/dependency_links.txt
+-rw-r--r--   0 sateantaranyan   (501) staff       (20)     2398 2024-05-12 00:31:30.000000 fashiontrendforecasting-0.2.0/FashionTrendForecasting.egg-info/requires.txt
+-rw-r--r--   0 sateantaranyan   (501) staff       (20)       24 2024-05-12 00:31:30.000000 fashiontrendforecasting-0.2.0/FashionTrendForecasting.egg-info/top_level.txt
+-rw-r--r--   0 sateantaranyan   (501) staff       (20)     1063 2024-05-11 13:27:18.000000 fashiontrendforecasting-0.2.0/LICENSE
+-rw-r--r--   0 sateantaranyan   (501) staff       (20)     4686 2024-05-12 00:31:30.903580 fashiontrendforecasting-0.2.0/PKG-INFO
+-rw-r--r--   0 sateantaranyan   (501) staff       (20)     1952 2024-05-11 13:27:18.000000 fashiontrendforecasting-0.2.0/README.md
+-rw-r--r--   0 sateantaranyan   (501) staff       (20)       38 2024-05-12 00:31:30.903953 fashiontrendforecasting-0.2.0/setup.cfg
+-rw-r--r--   0 sateantaranyan   (501) staff       (20)     4408 2024-05-11 13:27:18.000000 fashiontrendforecasting-0.2.0/setup.py
+drwxr-xr-x   0 sateantaranyan   (501) staff       (20)        0 2024-05-12 00:31:30.899622 fashiontrendforecasting-0.2.0/tests/
+-rw-r--r--   0 sateantaranyan   (501) staff       (20)     1503 2024-05-11 13:27:18.000000 fashiontrendforecasting-0.2.0/tests/test_prediction.py
+-rw-r--r--   0 sateantaranyan   (501) staff       (20)      535 2024-05-11 13:27:18.000000 fashiontrendforecasting-0.2.0/tests/test_trend_analysis.py
```

### Comparing `FashionTrendForecasting-0.1.0/FashionTrendForecasting/data_processing/insert_data.py` & `fashiontrendforecasting-0.2.0/FashionTrendForecasting/data_processing/insert_data.py`

 * *Files identical despite different names*

### Comparing `FashionTrendForecasting-0.1.0/FashionTrendForecasting/data_processing/sql_interactions.py` & `fashiontrendforecasting-0.2.0/FashionTrendForecasting/data_processing/sql_interactions.py`

 * *Files identical despite different names*

### Comparing `FashionTrendForecasting-0.1.0/FashionTrendForecasting/trend_analysis/Simple_Model.py` & `fashiontrendforecasting-0.2.0/FashionTrendForecasting/trend_analysis/Simple_Model.py`

 * *Files identical despite different names*

### Comparing `FashionTrendForecasting-0.1.0/FashionTrendForecasting/trend_analysis/model.py` & `fashiontrendforecasting-0.2.0/FashionTrendForecasting/trend_analysis/model.py`

 * *Files identical despite different names*

### Comparing `FashionTrendForecasting-0.1.0/FashionTrendForecasting.egg-info/PKG-INFO` & `fashiontrendforecasting-0.2.0/FashionTrendForecasting.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,38 @@
 Metadata-Version: 2.1
 Name: FashionTrendForecasting
-Version: 0.1.0
+Version: 0.2.0
 Summary: A package for predicting fashion trends
 Author: Anahit Manukyan, Milena Bazoyan, Lusine Torosyan, Sate Antaranyan
-Requires-Python: >=3.12.0
+Requires-Python: >=3.11.7
+Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: aiobotocore
+Requires-Dist: aiohttp
+Requires-Dist: aioitertools
+Requires-Dist: aiosignal
+Requires-Dist: alabaster
+Requires-Dist: altair
+Requires-Dist: anaconda-client
+Requires-Dist: anaconda-navigator
+Requires-Dist: anaconda-project
 Requires-Dist: annotated-types==0.6.0
 Requires-Dist: anyio==4.3.0
 Requires-Dist: appnope==0.1.4
 Requires-Dist: argon2-cffi==23.1.0
-Requires-Dist: argon2-cffi-bindings==21.2.0
 Requires-Dist: arrow==1.3.0
 Requires-Dist: asttokens==2.4.1
-Requires-Dist: async-lru==2.0.4
 Requires-Dist: attrs==23.2.0
 Requires-Dist: Babel==2.15.0
 Requires-Dist: beautifulsoup4==4.12.3
 Requires-Dist: bleach==6.1.0
 Requires-Dist: certifi==2024.2.2
 Requires-Dist: cffi==1.16.0
 Requires-Dist: charset-normalizer==3.3.2
 Requires-Dist: click==8.1.7
-Requires-Dist: comm==0.2.2
 Requires-Dist: contourpy==1.2.1
 Requires-Dist: cycler==0.12.1
 Requires-Dist: debugpy==1.8.1
 Requires-Dist: decorator==5.1.1
 Requires-Dist: defusedxml==0.7.1
 Requires-Dist: executing==2.0.1
 Requires-Dist: Faker==24.14.0
```

### Comparing `FashionTrendForecasting-0.1.0/FashionTrendForecasting.egg-info/SOURCES.txt` & `fashiontrendforecasting-0.2.0/FashionTrendForecasting.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `FashionTrendForecasting-0.1.0/FashionTrendForecasting.egg-info/requires.txt` & `fashiontrendforecasting-0.2.0/FashionTrendForecasting.egg-info/requires.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,30 @@
+aiobotocore
+aiohttp
+aioitertools
+aiosignal
+alabaster
+altair
+anaconda-client
+anaconda-navigator
+anaconda-project
 annotated-types==0.6.0
 anyio==4.3.0
 appnope==0.1.4
 argon2-cffi==23.1.0
-argon2-cffi-bindings==21.2.0
 arrow==1.3.0
 asttokens==2.4.1
-async-lru==2.0.4
 attrs==23.2.0
 Babel==2.15.0
 beautifulsoup4==4.12.3
 bleach==6.1.0
 certifi==2024.2.2
 cffi==1.16.0
 charset-normalizer==3.3.2
 click==8.1.7
-comm==0.2.2
 contourpy==1.2.1
 cycler==0.12.1
 debugpy==1.8.1
 decorator==5.1.1
 defusedxml==0.7.1
 executing==2.0.1
 Faker==24.14.0
```

### Comparing `FashionTrendForecasting-0.1.0/LICENSE` & `fashiontrendforecasting-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `FashionTrendForecasting-0.1.0/PKG-INFO` & `fashiontrendforecasting-0.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,38 @@
 Metadata-Version: 2.1
 Name: FashionTrendForecasting
-Version: 0.1.0
+Version: 0.2.0
 Summary: A package for predicting fashion trends
 Author: Anahit Manukyan, Milena Bazoyan, Lusine Torosyan, Sate Antaranyan
-Requires-Python: >=3.12.0
+Requires-Python: >=3.11.7
+Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: aiobotocore
+Requires-Dist: aiohttp
+Requires-Dist: aioitertools
+Requires-Dist: aiosignal
+Requires-Dist: alabaster
+Requires-Dist: altair
+Requires-Dist: anaconda-client
+Requires-Dist: anaconda-navigator
+Requires-Dist: anaconda-project
 Requires-Dist: annotated-types==0.6.0
 Requires-Dist: anyio==4.3.0
 Requires-Dist: appnope==0.1.4
 Requires-Dist: argon2-cffi==23.1.0
-Requires-Dist: argon2-cffi-bindings==21.2.0
 Requires-Dist: arrow==1.3.0
 Requires-Dist: asttokens==2.4.1
-Requires-Dist: async-lru==2.0.4
 Requires-Dist: attrs==23.2.0
 Requires-Dist: Babel==2.15.0
 Requires-Dist: beautifulsoup4==4.12.3
 Requires-Dist: bleach==6.1.0
 Requires-Dist: certifi==2024.2.2
 Requires-Dist: cffi==1.16.0
 Requires-Dist: charset-normalizer==3.3.2
 Requires-Dist: click==8.1.7
-Requires-Dist: comm==0.2.2
 Requires-Dist: contourpy==1.2.1
 Requires-Dist: cycler==0.12.1
 Requires-Dist: debugpy==1.8.1
 Requires-Dist: decorator==5.1.1
 Requires-Dist: defusedxml==0.7.1
 Requires-Dist: executing==2.0.1
 Requires-Dist: Faker==24.14.0
```

### Comparing `FashionTrendForecasting-0.1.0/README.md` & `fashiontrendforecasting-0.2.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 ## Project Objective
 FashionTrendForecasting aims to address the rapidly changing trends in the fashion industry, focusing particularly on sustainability and personalization. By leveraging advanced data analytics and machine learning algorithms, this Python package helps fashion brands dynamically adapt their product development cycles to meet consumer demands efficiently. Our model predicts emerging trends by analyzing real-time data from social media, sales channels, and consumer feedback, enabling brands to respond with agility. The methodology includes comprehensive data collection, AI-driven trend analysis, and implementation strategies that emphasize sustainable and ethical production practices. EcoTrendz is designed to enhance the capability of fashion brands to maintain profitability while prioritizing environmental consciousness and personalized consumer experiences.
 
 ## Installation
 To install FashionTrendForecasting, use the following pip command:
 
 ```bash
-pip install ecotrendz
+pip install FashionTrendForecasting==0.1.0
 ```
 
 For more details, updates, and versions, please visit our project on PyPI:
-[FashionTrendForecasting on PyPI]( "should be the link of the package")
+[FashionTrendForecasting on PyPI]( "(https://pypi.org/project/FashionTrendForecasting/0.1.0/)")
 
 
 ## License
 This project is licensed under the MIT License. For more details, see the LICENSE file in the repository.
 
 
 ## Getting Started
@@ -32,7 +32,8 @@
    ```bash
    python run.py
    ```
 3. **Access the Application**:
    - **Open the Application**: Navigate to [http://127.0.0.1:8000](http://127.0.0.1:8000) in your browser.
    - **API Documentation**: To access the API documentation, visit [http://127.0.0.1:8000/docs](http://127.0.0.1:8000/docs). 
 
+
```

### Comparing `FashionTrendForecasting-0.1.0/setup.py` & `fashiontrendforecasting-0.2.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,36 +1,42 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
-
 setup(
-    author = 'Anahit Manukyan, Milena Bazoyan, Lusine Torosyan, Sate Antaranyan',
-    description= 'A package for predicting fashion trends',
-    name = 'FashionTrendForecasting',
-    version = '0.1.0',
-    packages = find_packages(include = ['FashionTrendForecasting', 'FashionTrendForecasting.*']),
+    author='Anahit Manukyan, Milena Bazoyan, Lusine Torosyan, Sate Antaranyan',
+    description='A package for predicting fashion trends',
+    long_description_content_type="text/markdown",
+    name='FashionTrendForecasting',
+    version='0.2.0',
+    packages=find_packages(include=['FashionTrendForecasting', 'FashionTrendForecasting.*']),
     install_requires=[
+        'aiobotocore',
+        'aiohttp',
+        'aioitertools',
+        'aiosignal',
+        'alabaster',
+        'altair',
+        'anaconda-client',
+        'anaconda-navigator',
+        'anaconda-project',
         'annotated-types==0.6.0',
         'anyio==4.3.0',
         'appnope==0.1.4',
         'argon2-cffi==23.1.0',
-        'argon2-cffi-bindings==21.2.0',
         'arrow==1.3.0',
         'asttokens==2.4.1',
-        'async-lru==2.0.4',
         'attrs==23.2.0',
         'Babel==2.15.0',
         'beautifulsoup4==4.12.3',
         'bleach==6.1.0',
         'certifi==2024.2.2',
         'cffi==1.16.0',
         'charset-normalizer==3.3.2',
         'click==8.1.7',
-        'comm==0.2.2',
         'contourpy==1.2.1',
         'cycler==0.12.1',
         'debugpy==1.8.1',
         'decorator==5.1.1',
         'defusedxml==0.7.1',
         'executing==2.0.1',
         'Faker==24.14.0',
@@ -129,16 +135,16 @@
         'tzdata==2024.1',
         'uri-template==1.3.0',
         'urllib3==2.2.1',
         'uvicorn==0.29.0',
         'uvloop==0.19.0',
         'watchfiles==0.21.0',
         'wcwidth==0.2.13',
-        'webcolors==1.13',
+
+'webcolors==1.13',
         'webencodings==0.5.1',
         'websocket-client==1.8.0',
         'websockets==12.0',
         'widgetsnbextension==4.0.10'
     ],
-
-python_requires='>=3.12.0'
+    python_requires='>=3.11.7'
 )
```

### Comparing `FashionTrendForecasting-0.1.0/tests/test_prediction.py` & `fashiontrendforecasting-0.2.0/tests/test_prediction.py`

 * *Files identical despite different names*

### Comparing `FashionTrendForecasting-0.1.0/tests/test_trend_analysis.py` & `fashiontrendforecasting-0.2.0/tests/test_trend_analysis.py`

 * *Files identical despite different names*

