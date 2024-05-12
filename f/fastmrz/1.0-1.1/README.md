# Comparing `tmp/fastmrz-1.0.tar.gz` & `tmp/fastmrz-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastmrz-1.0.tar", last modified: Mon Apr  8 17:12:45 2024, max compression
+gzip compressed data, was "fastmrz-1.1.tar", last modified: Sun May 12 14:00:51 2024, max compression
```

## Comparing `fastmrz-1.0.tar` & `fastmrz-1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-04-08 17:12:45.551335 fastmrz-1.0/
--rw-rw-rw-   0        0        0    35184 2024-03-31 11:40:54.000000 fastmrz-1.0/LICENSE
--rw-rw-rw-   0        0        0       34 2024-04-08 11:27:20.000000 fastmrz-1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     7326 2024-04-08 17:12:45.550326 fastmrz-1.0/PKG-INFO
--rw-rw-rw-   0        0        0     4722 2024-04-08 16:36:51.000000 fastmrz-1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-08 17:12:45.535451 fastmrz-1.0/fastmrz/
--rw-rw-rw-   0        0        0       62 2024-04-07 16:27:29.000000 fastmrz-1.0/fastmrz/__init__.py
--rw-rw-rw-   0        0        0     8647 2024-04-08 16:17:12.000000 fastmrz-1.0/fastmrz/fastmrz.py
--rw-rw-rw-   0        0        0      664 2024-04-08 16:17:47.000000 fastmrz-1.0/fastmrz/main.py
-drwxrwxrwx   0        0        0        0 2024-04-08 17:12:45.542417 fastmrz-1.0/fastmrz/model/
--rw-rw-rw-   0        0        0  5254428 2024-03-31 11:40:54.000000 fastmrz-1.0/fastmrz/model/mrz_seg.tflite
-drwxrwxrwx   0        0        0        0 2024-04-08 17:12:45.541276 fastmrz-1.0/fastmrz.egg-info/
--rw-rw-rw-   0        0        0     7326 2024-04-08 17:12:45.000000 fastmrz-1.0/fastmrz.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      290 2024-04-08 17:12:45.000000 fastmrz-1.0/fastmrz.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-08 17:12:45.000000 fastmrz-1.0/fastmrz.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      688 2024-04-08 17:12:45.000000 fastmrz-1.0/fastmrz.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-08 17:12:45.000000 fastmrz-1.0/fastmrz.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-08 17:12:45.552333 fastmrz-1.0/setup.cfg
--rw-rw-rw-   0        0        0     2729 2024-04-08 17:12:06.000000 fastmrz-1.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-08 17:12:45.549292 fastmrz-1.0/tests/
--rw-rw-rw-   0        0        0     2172 2024-04-07 16:29:57.000000 fastmrz-1.0/tests/test.py
+drwxrwxrwx   0        0        0        0 2024-05-12 14:00:51.058173 fastmrz-1.1/
+-rw-rw-rw-   0        0        0    35184 2024-03-31 11:40:54.000000 fastmrz-1.1/LICENSE
+-rw-rw-rw-   0        0        0       34 2024-04-08 11:27:20.000000 fastmrz-1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     7491 2024-05-12 14:00:51.057021 fastmrz-1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4887 2024-05-12 08:09:25.000000 fastmrz-1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-12 14:00:51.044569 fastmrz-1.1/fastmrz/
+-rw-rw-rw-   0        0        0       62 2024-04-07 16:27:29.000000 fastmrz-1.1/fastmrz/__init__.py
+-rw-rw-rw-   0        0        0     9375 2024-05-12 08:11:25.000000 fastmrz-1.1/fastmrz/fastmrz.py
+-rw-rw-rw-   0        0        0      498 2024-05-12 08:19:01.000000 fastmrz-1.1/fastmrz/main.py
+drwxrwxrwx   0        0        0        0 2024-05-12 14:00:51.050085 fastmrz-1.1/fastmrz/model/
+-rw-rw-rw-   0        0        0  5254428 2024-03-31 11:40:54.000000 fastmrz-1.1/fastmrz/model/mrz_seg.tflite
+drwxrwxrwx   0        0        0        0 2024-05-12 14:00:51.049075 fastmrz-1.1/fastmrz.egg-info/
+-rw-rw-rw-   0        0        0     7491 2024-05-12 14:00:50.000000 fastmrz-1.1/fastmrz.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      290 2024-05-12 14:00:50.000000 fastmrz-1.1/fastmrz.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-12 14:00:50.000000 fastmrz-1.1/fastmrz.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      688 2024-05-12 14:00:50.000000 fastmrz-1.1/fastmrz.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-12 14:00:50.000000 fastmrz-1.1/fastmrz.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-12 14:00:51.058173 fastmrz-1.1/setup.cfg
+-rw-rw-rw-   0        0        0     2729 2024-05-12 14:00:27.000000 fastmrz-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-12 14:00:51.055623 fastmrz-1.1/tests/
+-rw-rw-rw-   0        0        0     2172 2024-04-07 16:29:57.000000 fastmrz-1.1/tests/test.py
```

### Comparing `fastmrz-1.0/LICENSE` & `fastmrz-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fastmrz-1.0/PKG-INFO` & `fastmrz-1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastmrz
-Version: 1.0
+Version: 1.1
 Summary: Extracts the Machine Readable Zone (MRZ) data from document images
 Home-page: https://github.com/sivakumar-mahalingam/fastmrz
 Author: Sivakumar Mahalingam
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3.8
@@ -64,14 +64,15 @@
 Requires-Dist: wrapt>=1.16.0
 
 # Fast MRZ
 
 ![License](https://img.shields.io/badge/license-AGPL%203.0-green)
 ![Python](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue?logo=python)
 [![CodeQL](https://github.com/sivakumar-mahalingam/fastmrz/actions/workflows/codeql.yml/badge.svg)](https://github.com/sivakumar-mahalingam/fastmrz/actions/workflows/codeql.yml)
+[![PyPI](https://img.shields.io/pypi/v/fastmrz.svg)](https://pypi.org/project/fastmrz/)
 
 <a href="https://github.com/sivakumar-mahalingam/fastmrz/" target="_blank">
     <img src="https://raw.githubusercontent.com/sivakumar-mahalingam/fastmrz/main/docs/FastMRZ.png" target="_blank" />
 </a>
 
 This repository extracts the Machine Readable Zone (MRZ) from document images. The MRZ typically contains important information such as the document holder's name, nationality, document number, date of birth, etc.
 
@@ -98,15 +99,15 @@
     $ pip install fastmrz
     
     ---> 100%
     ```
 
 2. You also need to install [Tesseract OCR](https://tesseract-ocr.github.io/tessdoc/Installation.html) engine. And set `PATH` variable with the executable. 
 
-3. Replace `eng.traineddata` in `tessdata` folder with the downloaded `tessdata/mrz_v2.traineddata` file from the repo
+3. Copy `mrz.traineddata` in `tessdata` folder of [repo](https://github.com/sivakumar-mahalingam/fastmrz/raw/main/tessdata/mrz.traineddata) to the tessdata folder in installed tesseract location
 
 ## Example
 
 ```Python
 from fastmrz import FastMRZ
 import os
 import json
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fastmrz Version: 1.0 Summary: Extracts the Machine
+Metadata-Version: 2.1 Name: fastmrz Version: 1.1 Summary: Extracts the Machine
 Readable Zone (MRZ) data from document images Home-page: https://github.com/
 sivakumar-mahalingam/fastmrz Author: Sivakumar Mahalingam Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: GNU Affero
 General Public License v3 Classifier: License :: OSI Approved :: GNU Affero
 General Public License v3 or later (AGPLv3+) Classifier: Programming Language
 :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
@@ -32,16 +32,17 @@
 gcs-filesystem>=0.31.0 Requires-Dist: termcolor>=2.4.0 Requires-Dist:
 typing_extensions>=4.10.0 Requires-Dist: urllib3>=2.2.1 Requires-Dist:
 Werkzeug>=3.0.1 Requires-Dist: wrapt>=1.16.0 # Fast MRZ ![License](https://
 img.shields.io/badge/license-AGPL%203.0-green) ![Python](https://
 img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-
 blue?logo=python) [![CodeQL](https://github.com/sivakumar-mahalingam/fastmrz/
 actions/workflows/codeql.yml/badge.svg)](https://github.com/sivakumar-
-mahalingam/fastmrz/actions/workflows/codeql.yml) _[_h_t_t_p_s_:_/_/
-_r_a_w_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_s_i_v_a_k_u_m_a_r_-_m_a_h_a_l_i_n_g_a_m_/_f_a_s_t_m_r_z_/_m_a_i_n_/_d_o_c_s_/
+mahalingam/fastmrz/actions/workflows/codeql.yml) [![PyPI](https://
+img.shields.io/pypi/v/fastmrz.svg)](https://pypi.org/project/fastmrz/) _[_h_t_t_p_s_:_/
+_/_r_a_w_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_s_i_v_a_k_u_m_a_r_-_m_a_h_a_l_i_n_g_a_m_/_f_a_s_t_m_r_z_/_m_a_i_n_/_d_o_c_s_/
 _F_a_s_t_M_R_Z_._p_n_g_]This repository extracts the Machine Readable Zone (MRZ) from
 document images. The MRZ typically contains important information such as the
 document holder's name, nationality, document number, date of birth, etc.
 **ï¸Features:** - Detects and extracts the MRZ region from document images -
 Contour detection to accurately identify the MRZ area - Custom trained models
 for Tensor and Tesseract - Contains checksum logics for data validation -
 Outputs the extracted MRZ region as text/json for further processing or
@@ -50,30 +51,31 @@
 img.shields.io/badge/OpenCV-27338e?style=for-the-
 badge&logo=OpenCV&logoColor=white) ![Tesseract OCR](https://img.shields.io/
 badge/Tesseract%20OCR-0F9D58?style=for-the-badge&logo=google&logoColor=white) !
 [NumPy](https://img.shields.io/badge/numpy-316192?style=for-the-
 badge&logo=numpy&logoColor=white) ## Installation 1. Install `fastmrz` from pip
 ```Console $ pip install fastmrz ---> 100% ``` 2. You also need to install
 [Tesseract OCR](https://tesseract-ocr.github.io/tessdoc/Installation.html)
-engine. And set `PATH` variable with the executable. 3. Replace
-`eng.traineddata` in `tessdata` folder with the downloaded `tessdata/
-mrz_v2.traineddata` file from the repo ## Example ```Python from fastmrz import
-FastMRZ import os import json fast_mrz = FastMRZ() # Pass file path of
-installed Tesseract OCR, incase if not added to PATH variable # fast_mrz =
-FastMRZ(tesseract_path=r'/opt/homebrew/Cellar/tesseract/5.3.4_1/bin/tesseract')
-# Default path in Mac # fast_mrz = FastMRZ(tesseract_path=r'C:\\Program
-Files\\Tesseract-OCR\\tesseract.exe') # Default path in Windows passport_mrz =
-fast_mrz.get_mrz(os.path.abspath('../data/passport_uk.jpg')) print("JSON:")
-print(json.dumps(passport_mrz, indent=4)) print("\n") passport_mrz =
-fast_mrz.get_raw_mrz(os.path.abspath('../data/passport_uk.jpg')) print("TEXT:")
-print(passport_mrz) ``` **OUTPUT:** ```Console JSON: { "mrz_type": "TD3",
-"document_type": "P", "country_code": "GBR", "surname": "PUDARSAN",
-"given_name": "HENERT", "document_number": "707797979", "nationality": "GBR",
-"date_of_birth": "1995-05-20", "sex": "M", "date_of_expiry": "2017-04-22",
-"status": "SUCCESS" } TEXT: P
+engine. And set `PATH` variable with the executable. 3. Copy `mrz.traineddata`
+in `tessdata` folder of [repo](https://github.com/sivakumar-mahalingam/fastmrz/
+raw/main/tessdata/mrz.traineddata) to the tessdata folder in installed
+tesseract location ## Example ```Python from fastmrz import FastMRZ import os
+import json fast_mrz = FastMRZ() # Pass file path of installed Tesseract OCR,
+incase if not added to PATH variable # fast_mrz = FastMRZ(tesseract_path=r'/
+opt/homebrew/Cellar/tesseract/5.3.4_1/bin/tesseract') # Default path in Mac #
+fast_mrz = FastMRZ(tesseract_path=r'C:\\Program Files\\Tesseract-
+OCR\\tesseract.exe') # Default path in Windows passport_mrz = fast_mrz.get_mrz
+(os.path.abspath('../data/passport_uk.jpg')) print("JSON:") print(json.dumps
+(passport_mrz, indent=4)) print("\n") passport_mrz = fast_mrz.get_raw_mrz
+(os.path.abspath('../data/passport_uk.jpg')) print("TEXT:") print(passport_mrz)
+``` **OUTPUT:** ```Console JSON: { "mrz_type": "TD3", "document_type": "P",
+"country_code": "GBR", "surname": "PUDARSAN", "given_name": "HENERT",
+"document_number": "707797979", "nationality": "GBR", "date_of_birth": "1995-
+05-20", "sex": "M", "date_of_expiry": "2017-04-22", "status": "SUCCESS" } TEXT:
+P
 <<<<<<<<<<<<<<<<<<<<<< 7077979792GBR9505209M1704224<<<<<<<<<<<<<<00 ``` ## MRZ
 Wiki MMRRZZ TTyyppeess && FFoorrmmaatt The standard for MRZ code is strictly regulated and has
 to comply with [Doc 9303](https://www.icao.int/publications/pages/
 publication.aspx?docnum=9303). Machine Readable Travel Documents published by
 the International Civil Aviation Organization. There are currently several
 types of ICAO standard machine-readable zones, which vary in the number of
 lines and characters in each line: - TD-1 (e.g. citizenâs identification
```

### Comparing `fastmrz-1.0/README.md` & `fastmrz-1.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Fast MRZ
 
 ![License](https://img.shields.io/badge/license-AGPL%203.0-green)
 ![Python](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue?logo=python)
 [![CodeQL](https://github.com/sivakumar-mahalingam/fastmrz/actions/workflows/codeql.yml/badge.svg)](https://github.com/sivakumar-mahalingam/fastmrz/actions/workflows/codeql.yml)
+[![PyPI](https://img.shields.io/pypi/v/fastmrz.svg)](https://pypi.org/project/fastmrz/)
 
 <a href="https://github.com/sivakumar-mahalingam/fastmrz/" target="_blank">
     <img src="https://raw.githubusercontent.com/sivakumar-mahalingam/fastmrz/main/docs/FastMRZ.png" target="_blank" />
 </a>
 
 This repository extracts the Machine Readable Zone (MRZ) from document images. The MRZ typically contains important information such as the document holder's name, nationality, document number, date of birth, etc.
 
@@ -33,15 +34,15 @@
     $ pip install fastmrz
     
     ---> 100%
     ```
 
 2. You also need to install [Tesseract OCR](https://tesseract-ocr.github.io/tessdoc/Installation.html) engine. And set `PATH` variable with the executable. 
 
-3. Replace `eng.traineddata` in `tessdata` folder with the downloaded `tessdata/mrz_v2.traineddata` file from the repo
+3. Copy `mrz.traineddata` in `tessdata` folder of [repo](https://github.com/sivakumar-mahalingam/fastmrz/raw/main/tessdata/mrz.traineddata) to the tessdata folder in installed tesseract location
 
 ## Example
 
 ```Python
 from fastmrz import FastMRZ
 import os
 import json
```

#### html2text {}

```diff
@@ -1,45 +1,47 @@
 # Fast MRZ ![License](https://img.shields.io/badge/license-AGPL%203.0-green) !
 [Python](https://img.shields.io/badge/python-
 3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue?logo=python) [![CodeQL](https://
 github.com/sivakumar-mahalingam/fastmrz/actions/workflows/codeql.yml/
 badge.svg)](https://github.com/sivakumar-mahalingam/fastmrz/actions/workflows/
-codeql.yml) _[_h_t_t_p_s_:_/_/_r_a_w_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_s_i_v_a_k_u_m_a_r_-_m_a_h_a_l_i_n_g_a_m_/_f_a_s_t_m_r_z_/
-_m_a_i_n_/_d_o_c_s_/_F_a_s_t_M_R_Z_._p_n_g_]This repository extracts the Machine Readable Zone (MRZ)
-from document images. The MRZ typically contains important information such as
-the document holder's name, nationality, document number, date of birth, etc.
-**ï¸Features:** - Detects and extracts the MRZ region from document images -
-Contour detection to accurately identify the MRZ area - Custom trained models
-for Tensor and Tesseract - Contains checksum logics for data validation -
-Outputs the extracted MRZ region as text/json for further processing or
-analysis ## Built With ![Tensorflow](https://img.shields.io/badge/TensorFlow-
-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white) ![OpenCV](https://
-img.shields.io/badge/OpenCV-27338e?style=for-the-
+codeql.yml) [![PyPI](https://img.shields.io/pypi/v/fastmrz.svg)](https://
+pypi.org/project/fastmrz/) _[_h_t_t_p_s_:_/_/_r_a_w_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_s_i_v_a_k_u_m_a_r_-
+_m_a_h_a_l_i_n_g_a_m_/_f_a_s_t_m_r_z_/_m_a_i_n_/_d_o_c_s_/_F_a_s_t_M_R_Z_._p_n_g_]This repository extracts the Machine
+Readable Zone (MRZ) from document images. The MRZ typically contains important
+information such as the document holder's name, nationality, document number,
+date of birth, etc. **ï¸Features:** - Detects and extracts the MRZ region from
+document images - Contour detection to accurately identify the MRZ area -
+Custom trained models for Tensor and Tesseract - Contains checksum logics for
+data validation - Outputs the extracted MRZ region as text/json for further
+processing or analysis ## Built With ![Tensorflow](https://img.shields.io/
+badge/TensorFlow-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white) !
+[OpenCV](https://img.shields.io/badge/OpenCV-27338e?style=for-the-
 badge&logo=OpenCV&logoColor=white) ![Tesseract OCR](https://img.shields.io/
 badge/Tesseract%20OCR-0F9D58?style=for-the-badge&logo=google&logoColor=white) !
 [NumPy](https://img.shields.io/badge/numpy-316192?style=for-the-
 badge&logo=numpy&logoColor=white) ## Installation 1. Install `fastmrz` from pip
 ```Console $ pip install fastmrz ---> 100% ``` 2. You also need to install
 [Tesseract OCR](https://tesseract-ocr.github.io/tessdoc/Installation.html)
-engine. And set `PATH` variable with the executable. 3. Replace
-`eng.traineddata` in `tessdata` folder with the downloaded `tessdata/
-mrz_v2.traineddata` file from the repo ## Example ```Python from fastmrz import
-FastMRZ import os import json fast_mrz = FastMRZ() # Pass file path of
-installed Tesseract OCR, incase if not added to PATH variable # fast_mrz =
-FastMRZ(tesseract_path=r'/opt/homebrew/Cellar/tesseract/5.3.4_1/bin/tesseract')
-# Default path in Mac # fast_mrz = FastMRZ(tesseract_path=r'C:\\Program
-Files\\Tesseract-OCR\\tesseract.exe') # Default path in Windows passport_mrz =
-fast_mrz.get_mrz(os.path.abspath('../data/passport_uk.jpg')) print("JSON:")
-print(json.dumps(passport_mrz, indent=4)) print("\n") passport_mrz =
-fast_mrz.get_raw_mrz(os.path.abspath('../data/passport_uk.jpg')) print("TEXT:")
-print(passport_mrz) ``` **OUTPUT:** ```Console JSON: { "mrz_type": "TD3",
-"document_type": "P", "country_code": "GBR", "surname": "PUDARSAN",
-"given_name": "HENERT", "document_number": "707797979", "nationality": "GBR",
-"date_of_birth": "1995-05-20", "sex": "M", "date_of_expiry": "2017-04-22",
-"status": "SUCCESS" } TEXT: P
+engine. And set `PATH` variable with the executable. 3. Copy `mrz.traineddata`
+in `tessdata` folder of [repo](https://github.com/sivakumar-mahalingam/fastmrz/
+raw/main/tessdata/mrz.traineddata) to the tessdata folder in installed
+tesseract location ## Example ```Python from fastmrz import FastMRZ import os
+import json fast_mrz = FastMRZ() # Pass file path of installed Tesseract OCR,
+incase if not added to PATH variable # fast_mrz = FastMRZ(tesseract_path=r'/
+opt/homebrew/Cellar/tesseract/5.3.4_1/bin/tesseract') # Default path in Mac #
+fast_mrz = FastMRZ(tesseract_path=r'C:\\Program Files\\Tesseract-
+OCR\\tesseract.exe') # Default path in Windows passport_mrz = fast_mrz.get_mrz
+(os.path.abspath('../data/passport_uk.jpg')) print("JSON:") print(json.dumps
+(passport_mrz, indent=4)) print("\n") passport_mrz = fast_mrz.get_raw_mrz
+(os.path.abspath('../data/passport_uk.jpg')) print("TEXT:") print(passport_mrz)
+``` **OUTPUT:** ```Console JSON: { "mrz_type": "TD3", "document_type": "P",
+"country_code": "GBR", "surname": "PUDARSAN", "given_name": "HENERT",
+"document_number": "707797979", "nationality": "GBR", "date_of_birth": "1995-
+05-20", "sex": "M", "date_of_expiry": "2017-04-22", "status": "SUCCESS" } TEXT:
+P
 <<<<<<<<<<<<<<<<<<<<<< 7077979792GBR9505209M1704224<<<<<<<<<<<<<<00 ``` ## MRZ
 Wiki MMRRZZ TTyyppeess && FFoorrmmaatt The standard for MRZ code is strictly regulated and has
 to comply with [Doc 9303](https://www.icao.int/publications/pages/
 publication.aspx?docnum=9303). Machine Readable Travel Documents published by
 the International Civil Aviation Organization. There are currently several
 types of ICAO standard machine-readable zones, which vary in the number of
 lines and characters in each line: - TD-1 (e.g. citizenâs identification
```

### Comparing `fastmrz-1.0/fastmrz/fastmrz.py` & `fastmrz-1.1/fastmrz/fastmrz.py`

 * *Files 9% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 
         c_area = np.zeros([len(contours)])
         for j in range(len(contours)):
             c_area[j] = cv2.contourArea(contours[j])
 
         x, y, w, h = cv2.boundingRect(contours[np.argmax(c_area)])
         roi_arr = image[y:y + h, x:x + w].copy()
-        roi = pytesseract.image_to_string(roi_arr)
+        roi = pytesseract.image_to_string(roi_arr, lang='mrz')
 
         return roi
 
     def _cleanse_roi(self, raw_text):
         input_list = raw_text.replace(' ', '').split('\n')
 
         selection_length = None
@@ -93,27 +93,44 @@
 
         return str(check_digit)
 
     def _format_date(self, input_date):
         formatted_date = str(datetime.strptime(input_date, '%y%m%d').date())
         return formatted_date
 
+    def _is_valid_file(self, image_path):
+        if isinstance(image_path, str):
+            if not os.path.isfile(image_path):
+                return f"Input file {image_path} is not valid or accessed"
+            else:
+                return image_path
+        elif not isinstance(image_path, np.ndarray):
+            return "Input is not vectorized"
+
     def get_raw_mrz(self, image_path):
-        image_array = self._process_image(image_path)
-        self.interpreter.set_tensor(self.input_details[0]['index'], image_array)
-        self.interpreter.invoke()
-        output_data = self.interpreter.get_tensor(self.output_details[0]['index'])
-        raw_roi = self._get_roi(output_data, image_path)
-        cleansed_roi = self._cleanse_roi(raw_roi)
+        file_status = self._is_valid_file(image_path)
+        if image_path == file_status:
+            image_array = self._process_image(image_path)
+            self.interpreter.set_tensor(self.input_details[0]['index'], image_array)
+            self.interpreter.invoke()
+            output_data = self.interpreter.get_tensor(self.output_details[0]['index'])
+            raw_roi = self._get_roi(output_data, image_path)
+            cleansed_roi = self._cleanse_roi(raw_roi)
 
-        return cleansed_roi
+            return cleansed_roi
+        else:
+            return file_status
 
     def get_mrz(self, image_path):
-        mrz_text = self.get_raw_mrz(image_path)
-        return self._parse_mrz(mrz_text)
+        file_status = self._is_valid_file(image_path)
+        if image_path == file_status:
+            mrz_text = self.get_raw_mrz(image_path)
+            return self._parse_mrz(mrz_text)
+        else:
+            return {'status': 'FAILURE', 'message': file_status}
 
     def _parse_mrz(self, mrz_text):
         mrz_lines = mrz_text.strip().split('\n')
         if len(mrz_lines) not in [2, 3]:
             return {'status': 'FAILURE', 'message': 'Invalid MRZ format'}
 
         mrz_code_dict = {}
```

### Comparing `fastmrz-1.0/fastmrz/model/mrz_seg.tflite` & `fastmrz-1.1/fastmrz/model/mrz_seg.tflite`

 * *Files identical despite different names*

### Comparing `fastmrz-1.0/fastmrz.egg-info/PKG-INFO` & `fastmrz-1.1/fastmrz.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastmrz
-Version: 1.0
+Version: 1.1
 Summary: Extracts the Machine Readable Zone (MRZ) data from document images
 Home-page: https://github.com/sivakumar-mahalingam/fastmrz
 Author: Sivakumar Mahalingam
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3.8
@@ -64,14 +64,15 @@
 Requires-Dist: wrapt>=1.16.0
 
 # Fast MRZ
 
 ![License](https://img.shields.io/badge/license-AGPL%203.0-green)
 ![Python](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue?logo=python)
 [![CodeQL](https://github.com/sivakumar-mahalingam/fastmrz/actions/workflows/codeql.yml/badge.svg)](https://github.com/sivakumar-mahalingam/fastmrz/actions/workflows/codeql.yml)
+[![PyPI](https://img.shields.io/pypi/v/fastmrz.svg)](https://pypi.org/project/fastmrz/)
 
 <a href="https://github.com/sivakumar-mahalingam/fastmrz/" target="_blank">
     <img src="https://raw.githubusercontent.com/sivakumar-mahalingam/fastmrz/main/docs/FastMRZ.png" target="_blank" />
 </a>
 
 This repository extracts the Machine Readable Zone (MRZ) from document images. The MRZ typically contains important information such as the document holder's name, nationality, document number, date of birth, etc.
 
@@ -98,15 +99,15 @@
     $ pip install fastmrz
     
     ---> 100%
     ```
 
 2. You also need to install [Tesseract OCR](https://tesseract-ocr.github.io/tessdoc/Installation.html) engine. And set `PATH` variable with the executable. 
 
-3. Replace `eng.traineddata` in `tessdata` folder with the downloaded `tessdata/mrz_v2.traineddata` file from the repo
+3. Copy `mrz.traineddata` in `tessdata` folder of [repo](https://github.com/sivakumar-mahalingam/fastmrz/raw/main/tessdata/mrz.traineddata) to the tessdata folder in installed tesseract location
 
 ## Example
 
 ```Python
 from fastmrz import FastMRZ
 import os
 import json
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fastmrz Version: 1.0 Summary: Extracts the Machine
+Metadata-Version: 2.1 Name: fastmrz Version: 1.1 Summary: Extracts the Machine
 Readable Zone (MRZ) data from document images Home-page: https://github.com/
 sivakumar-mahalingam/fastmrz Author: Sivakumar Mahalingam Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: GNU Affero
 General Public License v3 Classifier: License :: OSI Approved :: GNU Affero
 General Public License v3 or later (AGPLv3+) Classifier: Programming Language
 :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
@@ -32,16 +32,17 @@
 gcs-filesystem>=0.31.0 Requires-Dist: termcolor>=2.4.0 Requires-Dist:
 typing_extensions>=4.10.0 Requires-Dist: urllib3>=2.2.1 Requires-Dist:
 Werkzeug>=3.0.1 Requires-Dist: wrapt>=1.16.0 # Fast MRZ ![License](https://
 img.shields.io/badge/license-AGPL%203.0-green) ![Python](https://
 img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-
 blue?logo=python) [![CodeQL](https://github.com/sivakumar-mahalingam/fastmrz/
 actions/workflows/codeql.yml/badge.svg)](https://github.com/sivakumar-
-mahalingam/fastmrz/actions/workflows/codeql.yml) _[_h_t_t_p_s_:_/_/
-_r_a_w_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_s_i_v_a_k_u_m_a_r_-_m_a_h_a_l_i_n_g_a_m_/_f_a_s_t_m_r_z_/_m_a_i_n_/_d_o_c_s_/
+mahalingam/fastmrz/actions/workflows/codeql.yml) [![PyPI](https://
+img.shields.io/pypi/v/fastmrz.svg)](https://pypi.org/project/fastmrz/) _[_h_t_t_p_s_:_/
+_/_r_a_w_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_s_i_v_a_k_u_m_a_r_-_m_a_h_a_l_i_n_g_a_m_/_f_a_s_t_m_r_z_/_m_a_i_n_/_d_o_c_s_/
 _F_a_s_t_M_R_Z_._p_n_g_]This repository extracts the Machine Readable Zone (MRZ) from
 document images. The MRZ typically contains important information such as the
 document holder's name, nationality, document number, date of birth, etc.
 **ï¸Features:** - Detects and extracts the MRZ region from document images -
 Contour detection to accurately identify the MRZ area - Custom trained models
 for Tensor and Tesseract - Contains checksum logics for data validation -
 Outputs the extracted MRZ region as text/json for further processing or
@@ -50,30 +51,31 @@
 img.shields.io/badge/OpenCV-27338e?style=for-the-
 badge&logo=OpenCV&logoColor=white) ![Tesseract OCR](https://img.shields.io/
 badge/Tesseract%20OCR-0F9D58?style=for-the-badge&logo=google&logoColor=white) !
 [NumPy](https://img.shields.io/badge/numpy-316192?style=for-the-
 badge&logo=numpy&logoColor=white) ## Installation 1. Install `fastmrz` from pip
 ```Console $ pip install fastmrz ---> 100% ``` 2. You also need to install
 [Tesseract OCR](https://tesseract-ocr.github.io/tessdoc/Installation.html)
-engine. And set `PATH` variable with the executable. 3. Replace
-`eng.traineddata` in `tessdata` folder with the downloaded `tessdata/
-mrz_v2.traineddata` file from the repo ## Example ```Python from fastmrz import
-FastMRZ import os import json fast_mrz = FastMRZ() # Pass file path of
-installed Tesseract OCR, incase if not added to PATH variable # fast_mrz =
-FastMRZ(tesseract_path=r'/opt/homebrew/Cellar/tesseract/5.3.4_1/bin/tesseract')
-# Default path in Mac # fast_mrz = FastMRZ(tesseract_path=r'C:\\Program
-Files\\Tesseract-OCR\\tesseract.exe') # Default path in Windows passport_mrz =
-fast_mrz.get_mrz(os.path.abspath('../data/passport_uk.jpg')) print("JSON:")
-print(json.dumps(passport_mrz, indent=4)) print("\n") passport_mrz =
-fast_mrz.get_raw_mrz(os.path.abspath('../data/passport_uk.jpg')) print("TEXT:")
-print(passport_mrz) ``` **OUTPUT:** ```Console JSON: { "mrz_type": "TD3",
-"document_type": "P", "country_code": "GBR", "surname": "PUDARSAN",
-"given_name": "HENERT", "document_number": "707797979", "nationality": "GBR",
-"date_of_birth": "1995-05-20", "sex": "M", "date_of_expiry": "2017-04-22",
-"status": "SUCCESS" } TEXT: P
+engine. And set `PATH` variable with the executable. 3. Copy `mrz.traineddata`
+in `tessdata` folder of [repo](https://github.com/sivakumar-mahalingam/fastmrz/
+raw/main/tessdata/mrz.traineddata) to the tessdata folder in installed
+tesseract location ## Example ```Python from fastmrz import FastMRZ import os
+import json fast_mrz = FastMRZ() # Pass file path of installed Tesseract OCR,
+incase if not added to PATH variable # fast_mrz = FastMRZ(tesseract_path=r'/
+opt/homebrew/Cellar/tesseract/5.3.4_1/bin/tesseract') # Default path in Mac #
+fast_mrz = FastMRZ(tesseract_path=r'C:\\Program Files\\Tesseract-
+OCR\\tesseract.exe') # Default path in Windows passport_mrz = fast_mrz.get_mrz
+(os.path.abspath('../data/passport_uk.jpg')) print("JSON:") print(json.dumps
+(passport_mrz, indent=4)) print("\n") passport_mrz = fast_mrz.get_raw_mrz
+(os.path.abspath('../data/passport_uk.jpg')) print("TEXT:") print(passport_mrz)
+``` **OUTPUT:** ```Console JSON: { "mrz_type": "TD3", "document_type": "P",
+"country_code": "GBR", "surname": "PUDARSAN", "given_name": "HENERT",
+"document_number": "707797979", "nationality": "GBR", "date_of_birth": "1995-
+05-20", "sex": "M", "date_of_expiry": "2017-04-22", "status": "SUCCESS" } TEXT:
+P
 <<<<<<<<<<<<<<<<<<<<<< 7077979792GBR9505209M1704224<<<<<<<<<<<<<<00 ``` ## MRZ
 Wiki MMRRZZ TTyyppeess && FFoorrmmaatt The standard for MRZ code is strictly regulated and has
 to comply with [Doc 9303](https://www.icao.int/publications/pages/
 publication.aspx?docnum=9303). Machine Readable Travel Documents published by
 the International Civil Aviation Organization. There are currently several
 types of ICAO standard machine-readable zones, which vary in the number of
 lines and characters in each line: - TD-1 (e.g. citizenâs identification
```

### Comparing `fastmrz-1.0/fastmrz.egg-info/requires.txt` & `fastmrz-1.1/fastmrz.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `fastmrz-1.0/setup.py` & `fastmrz-1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open('README.md', 'r', encoding='utf8') as f:
     long_description = f.read()
 
 
 setup(
     name='fastmrz',
-    version='1.0',
+    version='1.1',
     author='Sivakumar Mahalingam',
     description='Extracts the Machine Readable Zone (MRZ) data from document images',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/sivakumar-mahalingam/fastmrz',
     packages=find_packages(),
     include_package_data=True,
```

### Comparing `fastmrz-1.0/tests/test.py` & `fastmrz-1.1/tests/test.py`

 * *Files identical despite different names*

