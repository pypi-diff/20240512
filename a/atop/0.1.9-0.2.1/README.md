# Comparing `tmp/atop-0.1.9.tar.gz` & `tmp/atop-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atop-0.1.9.tar", last modified: Mon Jan  1 23:35:10 2024, max compression
+gzip compressed data, was "atop-0.2.1.tar", last modified: Sat May 11 23:36:04 2024, max compression
```

## Comparing `atop-0.1.9.tar` & `atop-0.2.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 giacomogiallombardo   (501) staff       (20)        0 2024-01-01 23:35:10.101467 atop-0.1.9/
--rw-r--r--   0 giacomogiallombardo   (501) staff       (20)     1076 2023-09-29 22:18:25.000000 atop-0.1.9/LICENSE
--rw-r--r--   0 giacomogiallombardo   (501) staff       (20)     8633 2024-01-01 23:35:10.101142 atop-0.1.9/PKG-INFO
--rw-r--r--   0 giacomogiallombardo   (501) staff       (20)     7879 2024-01-01 18:49:00.000000 atop-0.1.9/README.md
--rw-r--r--   0 giacomogiallombardo   (501) staff       (20)       38 2024-01-01 23:35:10.101522 atop-0.1.9/setup.cfg
--rw-r--r--   0 giacomogiallombardo   (501) staff       (20)     1047 2024-01-01 23:29:28.000000 atop-0.1.9/setup.py
-drwxr-xr-x   0 giacomogiallombardo   (501) staff       (20)        0 2024-01-01 23:35:10.097359 atop-0.1.9/src/
-drwxr-xr-x   0 giacomogiallombardo   (501) staff       (20)        0 2024-01-01 23:35:10.098231 atop-0.1.9/src/atop/
--rw-r--r--   0 giacomogiallombardo   (501) staff       (20)        0 2023-09-04 09:32:52.000000 atop-0.1.9/src/atop/__init__.py
--rw-r--r--   0 giacomogiallombardo   (501) staff       (20)    26523 2024-01-01 19:09:13.000000 atop-0.1.9/src/atop/atop.py
-drwxr-xr-x   0 giacomogiallombardo   (501) staff       (20)        0 2024-01-01 23:35:10.100315 atop-0.1.9/src/atop/modules/
--rw-r--r--   0 giacomogiallombardo   (501) staff       (20)        0 2023-09-24 21:56:33.000000 atop-0.1.9/src/atop/modules/__init__.py
--rw-r--r--   0 giacomogiallombardo   (501) staff       (20)     5704 2023-09-28 16:29:24.000000 atop-0.1.9/src/atop/modules/const.py
--rw-r--r--   0 giacomogiallombardo   (501) staff       (20)    13810 2024-01-01 23:26:52.000000 atop-0.1.9/src/atop/modules/telegramhelper.py
--rw-r--r--   0 giacomogiallombardo   (501) staff       (20)     1894 2024-01-01 16:58:36.000000 atop-0.1.9/src/atop/modules/util.py
-drwxr-xr-x   0 giacomogiallombardo   (501) staff       (20)        0 2024-01-01 23:35:10.100901 atop-0.1.9/src/atop.egg-info/
--rw-r--r--   0 giacomogiallombardo   (501) staff       (20)     8633 2024-01-01 23:35:10.000000 atop-0.1.9/src/atop.egg-info/PKG-INFO
--rw-r--r--   0 giacomogiallombardo   (501) staff       (20)      422 2024-01-01 23:35:10.000000 atop-0.1.9/src/atop.egg-info/SOURCES.txt
--rw-r--r--   0 giacomogiallombardo   (501) staff       (20)        1 2024-01-01 23:35:10.000000 atop-0.1.9/src/atop.egg-info/dependency_links.txt
--rw-r--r--   0 giacomogiallombardo   (501) staff       (20)       51 2024-01-01 23:35:10.000000 atop-0.1.9/src/atop.egg-info/entry_points.txt
--rw-r--r--   0 giacomogiallombardo   (501) staff       (20)        1 2023-09-22 17:54:44.000000 atop-0.1.9/src/atop.egg-info/not-zip-safe
--rw-r--r--   0 giacomogiallombardo   (501) staff       (20)      215 2024-01-01 23:35:10.000000 atop-0.1.9/src/atop.egg-info/requires.txt
--rw-r--r--   0 giacomogiallombardo   (501) staff       (20)        5 2024-01-01 23:35:10.000000 atop-0.1.9/src/atop.egg-info/top_level.txt
-drwxr-xr-x   0 giacomogiallombardo   (501) staff       (20)        0 2024-01-01 23:35:10.100617 atop-0.1.9/tests/
--rw-r--r--   0 giacomogiallombardo   (501) staff       (20)     1284 2023-09-29 22:17:06.000000 atop-0.1.9/tests/test_ens.py
+drwxr-xr-x   0 giacomogiallombardo   (501) staff       (20)        0 2024-05-11 23:36:04.422823 atop-0.2.1/
+-rw-r--r--   0 giacomogiallombardo   (501) staff       (20)     1076 2023-09-29 22:18:25.000000 atop-0.2.1/LICENSE
+-rw-r--r--   0 giacomogiallombardo   (501) staff       (20)     8830 2024-05-11 23:36:04.422539 atop-0.2.1/PKG-INFO
+-rw-r--r--   0 giacomogiallombardo   (501) staff       (20)     8168 2024-05-11 23:25:28.000000 atop-0.2.1/README.md
+-rw-r--r--   0 giacomogiallombardo   (501) staff       (20)       38 2024-05-11 23:36:04.422885 atop-0.2.1/setup.cfg
+-rw-r--r--   0 giacomogiallombardo   (501) staff       (20)      956 2024-05-11 23:25:28.000000 atop-0.2.1/setup.py
+drwxr-xr-x   0 giacomogiallombardo   (501) staff       (20)        0 2024-05-11 23:36:04.418124 atop-0.2.1/src/
+drwxr-xr-x   0 giacomogiallombardo   (501) staff       (20)        0 2024-05-11 23:36:04.419150 atop-0.2.1/src/atop/
+-rw-r--r--   0 giacomogiallombardo   (501) staff       (20)        0 2023-09-04 09:32:52.000000 atop-0.2.1/src/atop/__init__.py
+-rw-r--r--   0 giacomogiallombardo   (501) staff       (20)    24145 2024-05-11 23:25:41.000000 atop-0.2.1/src/atop/atop.py
+drwxr-xr-x   0 giacomogiallombardo   (501) staff       (20)        0 2024-05-11 23:36:04.421605 atop-0.2.1/src/atop/modules/
+-rw-r--r--   0 giacomogiallombardo   (501) staff       (20)        0 2023-09-24 21:56:33.000000 atop-0.2.1/src/atop/modules/__init__.py
+-rw-r--r--   0 giacomogiallombardo   (501) staff       (20)     5704 2023-09-28 16:29:24.000000 atop-0.2.1/src/atop/modules/const.py
+-rw-r--r--   0 giacomogiallombardo   (501) staff       (20)    14040 2024-01-07 21:26:24.000000 atop-0.2.1/src/atop/modules/telegramhelper.py
+-rw-r--r--   0 giacomogiallombardo   (501) staff       (20)     6157 2024-05-11 23:25:49.000000 atop-0.2.1/src/atop/modules/util.py
+drwxr-xr-x   0 giacomogiallombardo   (501) staff       (20)        0 2024-05-11 23:36:04.422254 atop-0.2.1/src/atop.egg-info/
+-rw-r--r--   0 giacomogiallombardo   (501) staff       (20)     8830 2024-05-11 23:36:04.000000 atop-0.2.1/src/atop.egg-info/PKG-INFO
+-rw-r--r--   0 giacomogiallombardo   (501) staff       (20)      422 2024-05-11 23:36:04.000000 atop-0.2.1/src/atop.egg-info/SOURCES.txt
+-rw-r--r--   0 giacomogiallombardo   (501) staff       (20)        1 2024-05-11 23:36:04.000000 atop-0.2.1/src/atop.egg-info/dependency_links.txt
+-rw-r--r--   0 giacomogiallombardo   (501) staff       (20)       51 2024-05-11 23:36:04.000000 atop-0.2.1/src/atop.egg-info/entry_points.txt
+-rw-r--r--   0 giacomogiallombardo   (501) staff       (20)        1 2023-09-22 17:54:44.000000 atop-0.2.1/src/atop.egg-info/not-zip-safe
+-rw-r--r--   0 giacomogiallombardo   (501) staff       (20)      123 2024-05-11 23:36:04.000000 atop-0.2.1/src/atop.egg-info/requires.txt
+-rw-r--r--   0 giacomogiallombardo   (501) staff       (20)        5 2024-05-11 23:36:04.000000 atop-0.2.1/src/atop.egg-info/top_level.txt
+drwxr-xr-x   0 giacomogiallombardo   (501) staff       (20)        0 2024-05-11 23:36:04.421988 atop-0.2.1/tests/
+-rw-r--r--   0 giacomogiallombardo   (501) staff       (20)     1284 2023-09-29 22:17:06.000000 atop-0.2.1/tests/test_ens.py
```

### Comparing `atop-0.1.9/LICENSE` & `atop-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `atop-0.1.9/PKG-INFO` & `atop-0.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.1
 Name: atop
-Version: 0.1.9
+Version: 0.2.1
 Summary: "A TON of Privacy" formally called ATOP ... is a tool for conducting OSINT investigations on TON NFTs.
 Home-page: https://github.com/aaarghhh/a_TON_of_privacy
 Author: Aaarghhh
 Author-email: giacomo@udontneed.it
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: beautifulsoup4==4.12.2
-Requires-Dist: certifi==2023.7.22
-Requires-Dist: charset-normalizer==3.2.0
-Requires-Dist: colorama==0.4.6
-Requires-Dist: idna==3.4
-Requires-Dist: pyaes>=1.6.1
-Requires-Dist: pyasn1>=0.5.0
-Requires-Dist: python-dotenv>=1.0.0
-Requires-Dist: requests==2.31.0
-Requires-Dist: rsa>=4.9
-Requires-Dist: soupsieve>=2.5
-Requires-Dist: Telethon==1.30.3
-Requires-Dist: urllib3>=2.0.5
+Requires-Dist: beautifulsoup4
+Requires-Dist: certifi
+Requires-Dist: charset-normalizer
+Requires-Dist: colorama
+Requires-Dist: idna
+Requires-Dist: pyaes
+Requires-Dist: pyasn1
+Requires-Dist: python-dotenv
+Requires-Dist: requests
+Requires-Dist: rsa
+Requires-Dist: soupsieve
+Requires-Dist: Telethon
+Requires-Dist: urllib3
 
-# A TON of privacy v0.1.9
+# A TON of privacy v0.1.11
 ## ATOP - A tool for investigating TON network and its NFT.
 
 "A TON of Privacy" formally called ATOP ... is a tool for conducting OSINT investigations on TON (Telegram 🙃) NFTs.  
   
 The TON network is increasingly integrated with the Telegram ecosystem, via NFT. Telegram allows people to purchase numbers, domains and nicknames through cryptocurrency.  
   
 ATOP aims to give visibility into the addresses and details of the holders of these assets. Using this tool you will be able to retrieve:
@@ -37,29 +37,40 @@
   
 ATOP supports:
 - TON DNS
 - TON NICKNAME
 - TON PHONE NUMBERS (+888)
 
 ## INSTALLATION
+### 1. Git clone the repository.
+```
+$ git clone https://github.com/aaarghhh/a_TON_of_privacy.git
+$ cd a_TON_of_privacy
+```
 Install dependencies using pip and the file requirements.
 ```
 $ pip install -r requirements.txt
 ```
-Install via pip
+### 2. Via pipx
 ```
-$ pip install atop
+$ pipx install atop
 ```
 ## USAGE 
-If atop was installed as a **global package**: 
+
+
+If atop was installed as a **global package** (pipx): 
 ```
 $ a-ton-of-privacy --target "+888 12345678"
 ```
-Retrieve information about a:  
-  
+If atop was installed cloning the repository, from the root directory of the repository:
+```
+cd src/
+# python -m atop.atop --target @whatiamlookingfor
+```
+It retrieves information about a:
 - Telephone numbers
 ```
 $ python3 /src/atop/atop.py --target "+888 12345678"
 ```
 - Nickname 
 ```
 $ python3 /src/atop/atop.py --target @telegram_nickname
```

### Comparing `atop-0.1.9/README.md` & `atop-0.2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# A TON of privacy v0.1.9
+# A TON of privacy v0.1.11
 ## ATOP - A tool for investigating TON network and its NFT.
 
 "A TON of Privacy" formally called ATOP ... is a tool for conducting OSINT investigations on TON (Telegram 🙃) NFTs.  
   
 The TON network is increasingly integrated with the Telegram ecosystem, via NFT. Telegram allows people to purchase numbers, domains and nicknames through cryptocurrency.  
   
 ATOP aims to give visibility into the addresses and details of the holders of these assets. Using this tool you will be able to retrieve:
@@ -13,29 +13,40 @@
   
 ATOP supports:
 - TON DNS
 - TON NICKNAME
 - TON PHONE NUMBERS (+888)
 
 ## INSTALLATION
+### 1. Git clone the repository.
+```
+$ git clone https://github.com/aaarghhh/a_TON_of_privacy.git
+$ cd a_TON_of_privacy
+```
 Install dependencies using pip and the file requirements.
 ```
 $ pip install -r requirements.txt
 ```
-Install via pip
+### 2. Via pipx
 ```
-$ pip install atop
+$ pipx install atop
 ```
 ## USAGE 
-If atop was installed as a **global package**: 
+
+
+If atop was installed as a **global package** (pipx): 
 ```
 $ a-ton-of-privacy --target "+888 12345678"
 ```
-Retrieve information about a:  
-  
+If atop was installed cloning the repository, from the root directory of the repository:
+```
+cd src/
+# python -m atop.atop --target @whatiamlookingfor
+```
+It retrieves information about a:
 - Telephone numbers
 ```
 $ python3 /src/atop/atop.py --target "+888 12345678"
 ```
 - Nickname 
 ```
 $ python3 /src/atop/atop.py --target @telegram_nickname
```

### Comparing `atop-0.1.9/setup.py` & `atop-0.2.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 from setuptools import (
     setup,
     find_packages,
 )
 
 setup(
     name="atop",
-    version="0.1.9",
+    version="0.2.01",
     author="Aaarghhh",
     author_email="giacomo@udontneed.it",
     packages=["atop", "atop.modules"],
     package_dir={"": "src"},
     include_package_data=True,
     entry_points={"console_scripts": ["a-ton-of-privacy = atop.atop:run"]},
     url="https://github.com/aaarghhh/a_TON_of_privacy",
     license="MIT",
     description='"A TON of Privacy" formally called ATOP ... is a tool for conducting OSINT investigations on TON NFTs.',
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     install_requires=[
-        "beautifulsoup4==4.12.2",
-        "certifi==2023.7.22",
-        "charset-normalizer==3.2.0",
-        "colorama==0.4.6",
-        "idna==3.4",
-        "pyaes>=1.6.1",
-        "pyasn1>=0.5.0",
-        "python-dotenv>=1.0.0",
-        "requests==2.31.0",
-        "rsa>=4.9",
-        "soupsieve>=2.5",
-        "Telethon==1.30.3",
-        "urllib3>=2.0.5",
+        "beautifulsoup4",
+        "certifi",
+        "charset-normalizer",
+        "colorama",
+        "idna",
+        "pyaes",
+        "pyasn1",
+        "python-dotenv",
+        "requests",
+        "rsa",
+        "soupsieve",
+        "Telethon",
+        "urllib3",
     ],
     zip_safe=False,
 )
```

### Comparing `atop-0.1.9/src/atop/modules/const.py` & `atop-0.2.1/src/atop/modules/const.py`

 * *Files identical despite different names*

### Comparing `atop-0.1.9/src/atop/modules/telegramhelper.py` & `atop-0.2.1/src/atop/modules/telegramhelper.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,22 +32,31 @@
         api_id = input(" [!] Please enter your API ID:\n")
         api_hash = input(" [!] Please enter your API Hash:\n")
         phone_number = input(" [!] Please enter your phone number:\n")
         # validate with regex phone number
         _api_id = 0
         if not phone_number.startswith("+"):
             phone_number = "+" + phone_number.replace(" ", "")
-            if not re.compile(r"^(\+)[0-9]{11,12}$").match(phone_number):
-                print(" [-] Phone number is valid.")
-                return -1
+        phone_number = phone_number.strip()
+
+        if not re.compile(r"^(\+)[0-9]{11,12}$").match(phone_number):
+            print(" [-] Phone number is not valid!!!")
+            return -1
+
         if not re.compile(r"^\d+$").match(api_id):
-            print(" [-] App id is valid.")
+            print(" [-] App id is not valid!!!")
             return -1
         else:
-            _api_id = int(api_id)
+            _api_id = int(api_id.strip())
+
+        api_hash = api_hash.strip()
+        if not re.compile(r"^[a-fA-F0-9]{32}$").match(api_hash):
+            print(" [-] App hash is not valid!!!")
+            return -1
+
         with TelegramClient(StringSession(), _api_id, api_hash) as client:
             saved = False
             if path and path != "":
                 if Util.is_pathname_valid(path):
                     sessionstring = client.session.save()
                     with open(path, "w+") as f:
                         f.write("API_ID=" + api_id + "\n")
```

### Comparing `atop-0.1.9/src/atop.egg-info/PKG-INFO` & `atop-0.2.1/src/atop.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.1
 Name: atop
-Version: 0.1.9
+Version: 0.2.1
 Summary: "A TON of Privacy" formally called ATOP ... is a tool for conducting OSINT investigations on TON NFTs.
 Home-page: https://github.com/aaarghhh/a_TON_of_privacy
 Author: Aaarghhh
 Author-email: giacomo@udontneed.it
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: beautifulsoup4==4.12.2
-Requires-Dist: certifi==2023.7.22
-Requires-Dist: charset-normalizer==3.2.0
-Requires-Dist: colorama==0.4.6
-Requires-Dist: idna==3.4
-Requires-Dist: pyaes>=1.6.1
-Requires-Dist: pyasn1>=0.5.0
-Requires-Dist: python-dotenv>=1.0.0
-Requires-Dist: requests==2.31.0
-Requires-Dist: rsa>=4.9
-Requires-Dist: soupsieve>=2.5
-Requires-Dist: Telethon==1.30.3
-Requires-Dist: urllib3>=2.0.5
+Requires-Dist: beautifulsoup4
+Requires-Dist: certifi
+Requires-Dist: charset-normalizer
+Requires-Dist: colorama
+Requires-Dist: idna
+Requires-Dist: pyaes
+Requires-Dist: pyasn1
+Requires-Dist: python-dotenv
+Requires-Dist: requests
+Requires-Dist: rsa
+Requires-Dist: soupsieve
+Requires-Dist: Telethon
+Requires-Dist: urllib3
 
-# A TON of privacy v0.1.9
+# A TON of privacy v0.1.11
 ## ATOP - A tool for investigating TON network and its NFT.
 
 "A TON of Privacy" formally called ATOP ... is a tool for conducting OSINT investigations on TON (Telegram 🙃) NFTs.  
   
 The TON network is increasingly integrated with the Telegram ecosystem, via NFT. Telegram allows people to purchase numbers, domains and nicknames through cryptocurrency.  
   
 ATOP aims to give visibility into the addresses and details of the holders of these assets. Using this tool you will be able to retrieve:
@@ -37,29 +37,40 @@
   
 ATOP supports:
 - TON DNS
 - TON NICKNAME
 - TON PHONE NUMBERS (+888)
 
 ## INSTALLATION
+### 1. Git clone the repository.
+```
+$ git clone https://github.com/aaarghhh/a_TON_of_privacy.git
+$ cd a_TON_of_privacy
+```
 Install dependencies using pip and the file requirements.
 ```
 $ pip install -r requirements.txt
 ```
-Install via pip
+### 2. Via pipx
 ```
-$ pip install atop
+$ pipx install atop
 ```
 ## USAGE 
-If atop was installed as a **global package**: 
+
+
+If atop was installed as a **global package** (pipx): 
 ```
 $ a-ton-of-privacy --target "+888 12345678"
 ```
-Retrieve information about a:  
-  
+If atop was installed cloning the repository, from the root directory of the repository:
+```
+cd src/
+# python -m atop.atop --target @whatiamlookingfor
+```
+It retrieves information about a:
 - Telephone numbers
 ```
 $ python3 /src/atop/atop.py --target "+888 12345678"
 ```
 - Nickname 
 ```
 $ python3 /src/atop/atop.py --target @telegram_nickname
```

### Comparing `atop-0.1.9/tests/test_ens.py` & `atop-0.2.1/tests/test_ens.py`

 * *Files identical despite different names*

