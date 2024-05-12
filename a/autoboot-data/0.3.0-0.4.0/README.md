# Comparing `tmp/autoboot_data-0.3.0.tar.gz` & `tmp/autoboot_data-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoboot_data-0.3.0.tar", last modified: Fri May 10 20:13:03 2024, max compression
+gzip compressed data, was "autoboot_data-0.4.0.tar", last modified: Sun May 12 08:08:57 2024, max compression
```

## Comparing `autoboot_data-0.3.0.tar` & `autoboot_data-0.4.0.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 yizzuide   (501) staff       (20)        0 2024-05-10 20:13:03.936733 autoboot_data-0.3.0/
--rw-r--r--   0 yizzuide   (501) staff       (20)     1065 2023-11-15 08:28:44.000000 autoboot_data-0.3.0/LICENSE.txt
--rw-r--r--   0 yizzuide   (501) staff       (20)       62 2023-12-13 10:01:40.000000 autoboot_data-0.3.0/MANIFEST.in
--rw-r--r--   0 yizzuide   (501) staff       (20)     2633 2024-05-10 20:13:03.936587 autoboot_data-0.3.0/PKG-INFO
--rw-r--r--   0 yizzuide   (501) staff       (20)     1946 2024-01-01 18:26:21.000000 autoboot_data-0.3.0/README.md
-drwxr-xr-x   0 yizzuide   (501) staff       (20)        0 2024-05-10 20:13:03.930297 autoboot_data-0.3.0/autoboot_data/
--rw-r--r--   0 yizzuide   (501) staff       (20)       18 2024-05-10 20:12:52.000000 autoboot_data-0.3.0/autoboot_data/__init__.py
-drwxr-xr-x   0 yizzuide   (501) staff       (20)        0 2024-05-10 20:13:03.935298 autoboot_data-0.3.0/autoboot_data/redis/
--rw-r--r--   0 yizzuide   (501) staff       (20)      127 2023-11-24 07:07:32.000000 autoboot_data-0.3.0/autoboot_data/redis/__init__.py
--rw-r--r--   0 yizzuide   (501) staff       (20)      790 2023-12-13 18:47:25.000000 autoboot_data-0.3.0/autoboot_data/redis/queue.py
--rw-r--r--   0 yizzuide   (501) staff       (20)     1725 2024-05-08 13:14:40.000000 autoboot_data-0.3.0/autoboot_data/redis/redis_config.py
--rw-r--r--   0 yizzuide   (501) staff       (20)     1368 2024-05-10 20:11:53.000000 autoboot_data-0.3.0/autoboot_data/redis/redis_properties.py
-drwxr-xr-x   0 yizzuide   (501) staff       (20)        0 2024-05-10 20:13:03.935922 autoboot_data-0.3.0/autoboot_data.egg-info/
--rw-r--r--   0 yizzuide   (501) staff       (20)     2633 2024-05-10 20:13:03.000000 autoboot_data-0.3.0/autoboot_data.egg-info/PKG-INFO
--rw-r--r--   0 yizzuide   (501) staff       (20)      458 2024-05-10 20:13:03.000000 autoboot_data-0.3.0/autoboot_data.egg-info/SOURCES.txt
--rw-r--r--   0 yizzuide   (501) staff       (20)        1 2024-05-10 20:13:03.000000 autoboot_data-0.3.0/autoboot_data.egg-info/dependency_links.txt
--rw-r--r--   0 yizzuide   (501) staff       (20)        1 2023-12-13 10:07:55.000000 autoboot_data-0.3.0/autoboot_data.egg-info/not-zip-safe
--rw-r--r--   0 yizzuide   (501) staff       (20)       43 2024-05-10 20:13:03.000000 autoboot_data-0.3.0/autoboot_data.egg-info/requires.txt
--rw-r--r--   0 yizzuide   (501) staff       (20)       14 2024-05-10 20:13:03.000000 autoboot_data-0.3.0/autoboot_data.egg-info/top_level.txt
--rw-r--r--   0 yizzuide   (501) staff       (20)     1419 2023-12-13 10:09:56.000000 autoboot_data-0.3.0/pyproject.toml
--rw-r--r--   0 yizzuide   (501) staff       (20)       21 2024-05-10 20:12:07.000000 autoboot_data-0.3.0/requirements.txt
--rw-r--r--   0 yizzuide   (501) staff       (20)     1032 2024-05-10 20:13:03.937313 autoboot_data-0.3.0/setup.cfg
+drwxr-xr-x   0 yizzuide   (501) staff       (20)        0 2024-05-12 08:08:57.621748 autoboot_data-0.4.0/
+-rw-r--r--   0 yizzuide   (501) staff       (20)     1065 2023-11-15 08:28:44.000000 autoboot_data-0.4.0/LICENSE.txt
+-rw-r--r--   0 yizzuide   (501) staff       (20)      101 2024-05-12 07:49:30.000000 autoboot_data-0.4.0/MANIFEST.in
+-rw-r--r--   0 yizzuide   (501) staff       (20)     2633 2024-05-12 08:08:57.621583 autoboot_data-0.4.0/PKG-INFO
+-rw-r--r--   0 yizzuide   (501) staff       (20)     1946 2024-01-01 18:26:21.000000 autoboot_data-0.4.0/README.md
+drwxr-xr-x   0 yizzuide   (501) staff       (20)        0 2024-05-12 08:08:57.615348 autoboot_data-0.4.0/autoboot_data/
+-rw-r--r--   0 yizzuide   (501) staff       (20)       18 2024-05-12 07:48:47.000000 autoboot_data-0.4.0/autoboot_data/__init__.py
+-rw-r--r--   0 yizzuide   (501) staff       (20)     3114 2024-05-12 08:06:01.000000 autoboot_data-0.4.0/autoboot_data/autoboot-data-redis.schema.json
+drwxr-xr-x   0 yizzuide   (501) staff       (20)        0 2024-05-12 08:08:57.620294 autoboot_data-0.4.0/autoboot_data/redis/
+-rw-r--r--   0 yizzuide   (501) staff       (20)      127 2023-11-24 07:07:32.000000 autoboot_data-0.4.0/autoboot_data/redis/__init__.py
+-rw-r--r--   0 yizzuide   (501) staff       (20)      790 2023-12-13 18:47:25.000000 autoboot_data-0.4.0/autoboot_data/redis/queue.py
+-rw-r--r--   0 yizzuide   (501) staff       (20)     1725 2024-05-08 13:14:40.000000 autoboot_data-0.4.0/autoboot_data/redis/redis_config.py
+-rw-r--r--   0 yizzuide   (501) staff       (20)     1368 2024-05-10 20:11:53.000000 autoboot_data-0.4.0/autoboot_data/redis/redis_properties.py
+drwxr-xr-x   0 yizzuide   (501) staff       (20)        0 2024-05-12 08:08:57.620828 autoboot_data-0.4.0/autoboot_data.egg-info/
+-rw-r--r--   0 yizzuide   (501) staff       (20)     2633 2024-05-12 08:08:57.000000 autoboot_data-0.4.0/autoboot_data.egg-info/PKG-INFO
+-rw-r--r--   0 yizzuide   (501) staff       (20)      504 2024-05-12 08:08:57.000000 autoboot_data-0.4.0/autoboot_data.egg-info/SOURCES.txt
+-rw-r--r--   0 yizzuide   (501) staff       (20)        1 2024-05-12 08:08:57.000000 autoboot_data-0.4.0/autoboot_data.egg-info/dependency_links.txt
+-rw-r--r--   0 yizzuide   (501) staff       (20)        1 2023-12-13 10:07:55.000000 autoboot_data-0.4.0/autoboot_data.egg-info/not-zip-safe
+-rw-r--r--   0 yizzuide   (501) staff       (20)       43 2024-05-12 08:08:57.000000 autoboot_data-0.4.0/autoboot_data.egg-info/requires.txt
+-rw-r--r--   0 yizzuide   (501) staff       (20)       14 2024-05-12 08:08:57.000000 autoboot_data-0.4.0/autoboot_data.egg-info/top_level.txt
+-rw-r--r--   0 yizzuide   (501) staff       (20)     1419 2023-12-13 10:09:56.000000 autoboot_data-0.4.0/pyproject.toml
+-rw-r--r--   0 yizzuide   (501) staff       (20)       21 2024-05-12 07:52:56.000000 autoboot_data-0.4.0/requirements.txt
+-rw-r--r--   0 yizzuide   (501) staff       (20)     1081 2024-05-12 08:08:57.622361 autoboot_data-0.4.0/setup.cfg
```

### Comparing `autoboot_data-0.3.0/LICENSE.txt` & `autoboot_data-0.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `autoboot_data-0.3.0/PKG-INFO` & `autoboot_data-0.4.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: autoboot-data
-Version: 0.3.0
+Version: 0.4.0
 Summary: Data access build with autoboot
 Home-page: https://github.com/yizzuide/autoboot_data
 Author: yizzuide
 Author-email: fu837014586@163.com
 License: MIT
 Keywords: autoboot,data,redis
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: autoboot<1.0,>=0.7.0
+Requires-Dist: autoboot<1.0,>=0.9.0
 Provides-Extra: redis
 Requires-Dist: redis>=4.0.0; extra == "redis"
 
 # autoboot data starter
 基于 [autoboot](https://github.com/yizzuide/autoboot) 框架的扩展，用于支持数据层接入。
 <p>
   <a href="https://pypi.org/project/autoboot-data">
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1 Name: autoboot-data Version: 0.3.0 Summary: Data access
+Metadata-Version: 2.1 Name: autoboot-data Version: 0.4.0 Summary: Data access
 build with autoboot Home-page: https://github.com/yizzuide/autoboot_data
 Author: yizzuide Author-email: fu837014586@163.com License: MIT Keywords:
 autoboot,data,redis Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent Classifier: Intended Audience ::
 Developers Classifier: Programming Language :: Python :: 3.8 Classifier:
 License :: OSI Approved :: MIT License Requires-Python: >=3.8 Description-
 Content-Type: text/markdown License-File: LICENSE.txt Requires-Dist:
-autoboot<1.0,>=0.7.0 Provides-Extra: redis Requires-Dist: redis>=4.0.0; extra
+autoboot<1.0,>=0.9.0 Provides-Extra: redis Requires-Dist: redis>=4.0.0; extra
 == "redis" # autoboot data starter åºäº [autoboot](https://github.com/
 yizzuide/autoboot) æ¡æ¶çæ©å±ï¼ç¨äºæ¯ææ°æ®å±æ¥å¥ã
 _[_V_e_r_s_i_o_n_]_[_P_y_t_h_o_n_]_[_D_o_w_n_l_o_a_d_s_]_[_L_i_c_e_n_s_e_]
 ## Quick Start ### Install ```sh pip install autoboot-web ``` ### Usage ####
 éç½® * å¯å¨éç½®æä»¶`.env` ```ini #
 ç¯å¢åç§°ï¼é»è®¤å¼ï¼devï¼æ¡æ¶æ ¹æ®è¿ä¸ªéç½®é¡¹æ¥å è½½å½åçç¯å¢éç½®ï¼
 ENV_NAME=dev APPLICATION_NAME=data-runner ``` * ç¯å¢éç½®æä»¶`.env.dev`
```

### Comparing `autoboot_data-0.3.0/README.md` & `autoboot_data-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `autoboot_data-0.3.0/autoboot_data/redis/queue.py` & `autoboot_data-0.4.0/autoboot_data/redis/queue.py`

 * *Files identical despite different names*

### Comparing `autoboot_data-0.3.0/autoboot_data/redis/redis_config.py` & `autoboot_data-0.4.0/autoboot_data/redis/redis_config.py`

 * *Files identical despite different names*

### Comparing `autoboot_data-0.3.0/autoboot_data/redis/redis_properties.py` & `autoboot_data-0.4.0/autoboot_data/redis/redis_properties.py`

 * *Files identical despite different names*

### Comparing `autoboot_data-0.3.0/autoboot_data.egg-info/PKG-INFO` & `autoboot_data-0.4.0/autoboot_data.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: autoboot-data
-Version: 0.3.0
+Version: 0.4.0
 Summary: Data access build with autoboot
 Home-page: https://github.com/yizzuide/autoboot_data
 Author: yizzuide
 Author-email: fu837014586@163.com
 License: MIT
 Keywords: autoboot,data,redis
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: autoboot<1.0,>=0.7.0
+Requires-Dist: autoboot<1.0,>=0.9.0
 Provides-Extra: redis
 Requires-Dist: redis>=4.0.0; extra == "redis"
 
 # autoboot data starter
 基于 [autoboot](https://github.com/yizzuide/autoboot) 框架的扩展，用于支持数据层接入。
 <p>
   <a href="https://pypi.org/project/autoboot-data">
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1 Name: autoboot-data Version: 0.3.0 Summary: Data access
+Metadata-Version: 2.1 Name: autoboot-data Version: 0.4.0 Summary: Data access
 build with autoboot Home-page: https://github.com/yizzuide/autoboot_data
 Author: yizzuide Author-email: fu837014586@163.com License: MIT Keywords:
 autoboot,data,redis Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent Classifier: Intended Audience ::
 Developers Classifier: Programming Language :: Python :: 3.8 Classifier:
 License :: OSI Approved :: MIT License Requires-Python: >=3.8 Description-
 Content-Type: text/markdown License-File: LICENSE.txt Requires-Dist:
-autoboot<1.0,>=0.7.0 Provides-Extra: redis Requires-Dist: redis>=4.0.0; extra
+autoboot<1.0,>=0.9.0 Provides-Extra: redis Requires-Dist: redis>=4.0.0; extra
 == "redis" # autoboot data starter åºäº [autoboot](https://github.com/
 yizzuide/autoboot) æ¡æ¶çæ©å±ï¼ç¨äºæ¯ææ°æ®å±æ¥å¥ã
 _[_V_e_r_s_i_o_n_]_[_P_y_t_h_o_n_]_[_D_o_w_n_l_o_a_d_s_]_[_L_i_c_e_n_s_e_]
 ## Quick Start ### Install ```sh pip install autoboot-web ``` ### Usage ####
 éç½® * å¯å¨éç½®æä»¶`.env` ```ini #
 ç¯å¢åç§°ï¼é»è®¤å¼ï¼devï¼æ¡æ¶æ ¹æ®è¿ä¸ªéç½®é¡¹æ¥å è½½å½åçç¯å¢éç½®ï¼
 ENV_NAME=dev APPLICATION_NAME=data-runner ``` * ç¯å¢éç½®æä»¶`.env.dev`
```

### Comparing `autoboot_data-0.3.0/pyproject.toml` & `autoboot_data-0.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `autoboot_data-0.3.0/setup.cfg` & `autoboot_data-0.4.0/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -22,14 +22,18 @@
 packages = find:
 python_requires = >=3.8
 install_requires = file: requirements.txt
 tests_require = 
 	pytest>=6.2.0
 	pytest-cov>=2.10.0
 
+[options.package_data]
+autoboot_data = 
+	*.json
+
 [options.entry_points]
 console_scripts = 
 executable_name = 
 
 [options.extras_require]
 redis = 
 	redis>=4.0.0
```

