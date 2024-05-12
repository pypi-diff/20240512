# Comparing `tmp/gologin-2024.4.4122950.tar.gz` & `tmp/gologin-2024.5.12063328.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gologin-2024.4.4122950.tar", last modified: Thu Apr  4 12:29:51 2024, max compression
+gzip compressed data, was "gologin-2024.5.12063328.tar", last modified: Sun May 12 06:33:28 2024, max compression
```

## Comparing `gologin-2024.4.4122950.tar` & `gologin-2024.5.12063328.tar`

### file list

```diff
@@ -1,24 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:29:51.163204 gologin-2024.4.4122950/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 12:29:42.000000 gologin-2024.4.4122950/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5153 2024-04-04 12:29:51.163204 gologin-2024.4.4122950/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4822 2024-04-04 12:29:42.000000 gologin-2024.4.4122950/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:29:51.159204 gologin-2024.4.4122950/gologin/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-04 12:29:42.000000 gologin-2024.4.4122950/gologin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:29:51.163204 gologin-2024.4.4122950/gologin/extensionsManager/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-04 12:29:42.000000 gologin-2024.4.4122950/gologin/extensionsManager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3105 2024-04-04 12:29:42.000000 gologin-2024.4.4122950/gologin/extensionsManager/extensionsManager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-04-04 12:29:42.000000 gologin-2024.4.4122950/gologin/gologin-create-profile.py
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-04 12:29:42.000000 gologin-2024.4.4122950/gologin/gologin-local.py
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-04 12:29:42.000000 gologin-2024.4.4122950/gologin/gologin-pyppeteer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-04-04 12:29:42.000000 gologin-2024.4.4122950/gologin/gologin-selenium-multiprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-04 12:29:42.000000 gologin-2024.4.4122950/gologin/gologin-selenium.py
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-04-04 12:29:42.000000 gologin-2024.4.4122950/gologin/gologin-selenium_4.11.py
--rw-r--r--   0 runner    (1001) docker     (127)    29704 2024-04-04 12:29:42.000000 gologin-2024.4.4122950/gologin/gologin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:29:51.163204 gologin-2024.4.4122950/gologin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5153 2024-04-04 12:29:51.000000 gologin-2024.4.4122950/gologin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-04 12:29:51.000000 gologin-2024.4.4122950/gologin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 12:29:51.000000 gologin-2024.4.4122950/gologin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-04 12:29:51.000000 gologin-2024.4.4122950/gologin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-04 12:29:51.000000 gologin-2024.4.4122950/gologin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 12:29:51.163204 gologin-2024.4.4122950/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-04 12:29:50.000000 gologin-2024.4.4122950/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 06:33:28.691938 gologin-2024.5.12063328/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 06:33:19.000000 gologin-2024.5.12063328/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5154 2024-05-12 06:33:28.691938 gologin-2024.5.12063328/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4822 2024-05-12 06:33:19.000000 gologin-2024.5.12063328/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 06:33:28.687938 gologin-2024.5.12063328/gologin/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-12 06:33:19.000000 gologin-2024.5.12063328/gologin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-05-12 06:33:19.000000 gologin-2024.5.12063328/gologin/gologin-create-profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-12 06:33:19.000000 gologin-2024.5.12063328/gologin/gologin-local.py
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-12 06:33:19.000000 gologin-2024.5.12063328/gologin/gologin-pyppeteer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-05-12 06:33:19.000000 gologin-2024.5.12063328/gologin/gologin-selenium-multiprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-12 06:33:19.000000 gologin-2024.5.12063328/gologin/gologin-selenium.py
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-05-12 06:33:19.000000 gologin-2024.5.12063328/gologin/gologin-selenium_4.11.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31976 2024-05-12 06:33:19.000000 gologin-2024.5.12063328/gologin/gologin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 06:33:28.691938 gologin-2024.5.12063328/gologin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5154 2024-05-12 06:33:28.000000 gologin-2024.5.12063328/gologin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-12 06:33:28.000000 gologin-2024.5.12063328/gologin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 06:33:28.000000 gologin-2024.5.12063328/gologin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-12 06:33:28.000000 gologin-2024.5.12063328/gologin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-12 06:33:28.000000 gologin-2024.5.12063328/gologin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 06:33:28.691938 gologin-2024.5.12063328/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-12 06:33:28.000000 gologin-2024.5.12063328/setup.py
```

### Comparing `gologin-2024.4.4122950/PKG-INFO` & `gologin-2024.5.12063328/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gologin
-Version: 2024.4.4122950
+Version: 2024.5.12063328
 Summary: Official GoLogin python package
 Home-page: https://github.com/gologinapp/pygologin
 Author: GoLogin
 Author-email: yuri@gologin.com
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: gologin Version: 2024.4.4122950 Summary: Official
+Metadata-Version: 2.1 Name: gologin Version: 2024.5.12063328 Summary: Official
 GoLogin python package Home-page: https://github.com/gologinapp/pygologin
 Author: GoLogin Author-email: yuri@gologin.com Requires-Python: >=3.5
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 requests Requires-Dist: psutil # pygologin REST API provides programmatic
 access to GoLogin App. Create a new browser profile, get a list of all browser
 profiles, add a browser profile and running # class GoLogin - class for working
 with _g_o_l_o_g_i_n_._c_o_m API # Official Package ## Getting Started GoLogin supports
```

### Comparing `gologin-2024.4.4122950/README.md` & `gologin-2024.5.12063328/README.md`

 * *Files identical despite different names*

### Comparing `gologin-2024.4.4122950/gologin/gologin-create-profile.py` & `gologin-2024.5.12063328/gologin/gologin-create-profile.py`

 * *Files identical despite different names*

### Comparing `gologin-2024.4.4122950/gologin/gologin-local.py` & `gologin-2024.5.12063328/gologin/gologin-local.py`

 * *Files identical despite different names*

### Comparing `gologin-2024.4.4122950/gologin/gologin-pyppeteer.py` & `gologin-2024.5.12063328/gologin/gologin-pyppeteer.py`

 * *Files identical despite different names*

### Comparing `gologin-2024.4.4122950/gologin/gologin-selenium-multiprocess.py` & `gologin-2024.5.12063328/gologin/gologin-selenium-multiprocess.py`

 * *Files identical despite different names*

### Comparing `gologin-2024.4.4122950/gologin/gologin-selenium.py` & `gologin-2024.5.12063328/gologin/gologin-selenium.py`

 * *Files identical despite different names*

### Comparing `gologin-2024.4.4122950/gologin/gologin-selenium_4.11.py` & `gologin-2024.5.12063328/gologin/gologin-selenium_4.11.py`

 * *Files identical despite different names*

### Comparing `gologin-2024.4.4122950/gologin/gologin.py` & `gologin-2024.5.12063328/gologin/gologin.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,19 +11,20 @@
 import tempfile
 import math
 import socket
 import random
 import psutil
 
 from .extensionsManager import ExtensionsManager
+from .cookiesManager import CookiesManager
 
 API_URL = 'https://api.gologin.com'
 PROFILES_URL = 'https://gprofiles-new.gologin.com/'
 GET_TIMEZONE_URL = 'https://geo.myip.link'
-FILES_GATEWAY = ' https://files-gateway.gologin.com'
+FILES_GATEWAY = 'https://files-gateway.gologin.com'
 
 class ProtocolException(Exception):
     def __init__(self, data:dict):
         self._json =data
         super().__init__(data.__repr__())
     @property
     def json(self) -> dict:
@@ -38,14 +39,16 @@
         self.extra_params = options.get('extra_params', [])
         self.port = options.get('port', 3500)
         self.local = options.get('local', False)
         self.spawn_browser = options.get('spawn_browser', True)
         self.credentials_enable_service = options.get(
             'credentials_enable_service')
         self.cleaningLocalCookies = options.get('cleaningLocalCookies', False)
+        self.uploadCookiesToServer = options.get('uploadCookiesToServer', False)
+        self.writeCookiesFromServer = options.get('writeCookiesFromServer', False)
         self.executablePath = ''
         self.is_cloud_headless = options.get('is_cloud_headless', True)
         self.is_new_cloud_browser = options.get('is_new_cloud_browser', True)
 
         home = str(pathlib.Path.home())
         browser_gologin = os.path.join(home, '.gologin', 'browser')
         try:
@@ -80,15 +83,15 @@
     def setProfileId(self, profile_id):
         self.profile_id = profile_id
         if self.profile_id == None:
             return
         self.profile_path = os.path.join(
             self.tmpdir, 'gologin_' + self.profile_id)
         self.profile_zip_path = os.path.join(
-            self.tmpdir, 'gologin_' + self.profile_id+'.zip')
+            self.tmpdir, 'gologin_' + self.profile_id + '.zip')
         self.profile_zip_path_upload = os.path.join(
             self.tmpdir, 'gologin_' + self.profile_id+'_upload.zip')
 
     def loadExtensions(self):
         profile = self.profile
         chromeExtensions = profile.get('chromeExtensions')
         extensionsManagerInst = ExtensionsManager()
@@ -164,14 +167,15 @@
                 break
             except:
                 try_count += 1
                 time.sleep(1)
         return url
 
     def start(self):
+        print('start')
         profile_path = self.createStartup()
         if self.spawn_browser == True:
             return self.spawnBrowser()
         return profile_path
 
     def zipdir(self, path, ziph):
         for root, dirs, files in os.walk(path):
@@ -204,28 +208,32 @@
                 proc.kill()
         self.waitUntilProfileUsing()
         self.sanitizeProfile()
         if self.local == False:
             self.commitProfile()
             os.remove(self.profile_zip_path_upload)
             shutil.rmtree(self.profile_path)
+        print('profile stopped')
 
     def commitProfile(self):
+        print('commitProfile')
         zipf = zipfile.ZipFile(
             self.profile_zip_path_upload, 'w', zipfile.ZIP_DEFLATED)
         self.zipdir(self.profile_path, zipf)
         zipf.close()
 
         headers = {
             'Authorization': 'Bearer ' + self.access_token,
             'User-Agent': 'Selenium-API',
+            'Content-Type': 'application/zip',
             'browserId': self.profile_id
         }
 
-        requests.put(FILES_GATEWAY + '/upload', data=open(self.profile_zip_path_upload, 'rb'))
+        data = requests.put(FILES_GATEWAY + '/upload', data=open(self.profile_zip_path_upload, 'rb'), headers=headers)
+        print('commitProfile completed', data)
 
 
     def commitProfileOld(self):
         zipf = zipfile.ZipFile(
             self.profile_zip_path_upload, 'w', zipfile.ZIP_DEFLATED)
         self.zipdir(self.profile_path, zipf)
         zipf.close()
@@ -316,36 +324,36 @@
         if data.get("statusCode") == 404:
             raise Exception(data.get("error") + ": " + data.get("message"))
         return data
 
     def downloadProfileZip(self):
         print("downloadProfileZip")
         s3path = self.profile.get('s3Path', '')
+        print('s3path', s3path)
         data = ''
         headers = {
             'Authorization': 'Bearer ' + self.access_token,
             'User-Agent': 'Selenium-API',
             'browserId': self.profile_id
         }
-        data = requests.get(FILES_GATEWAY + '/download', headers=headers).content
 
+        data = requests.get(FILES_GATEWAY + '/download', headers=headers).content
 
         if len(data) == 0:
-            print('data is 0 - creating fresh profile content')
+            print('data is 0 - creating empty profile')
             self.createEmptyProfile()
         else:
-            print(data)
             with open(self.profile_zip_path, 'wb') as f:
                 f.write(data)
 
         try:
             print('extracting profile')
             self.extractProfileZip()
         except Exception as e:
-            print('exception', e)
+            print('ERROR!', e)
             self.uploadEmptyProfile()
             self.createEmptyProfile()
             self.extractProfileZip()
 
         # if not os.path.exists(os.path.join(self.profile_path, 'Default', 'Preferences')):
         #     print('preferences not found - creating fresh profile content')
         #     self.uploadEmptyProfile()
@@ -398,21 +406,33 @@
         source = requests.get(PROFILES_URL + 'zero_profile.zip')
         upload_profile.write(source.content)
         upload_profile.close
 
     def createEmptyProfile(self):
         print('createEmptyProfile')
         empty_profile = '../gologin_zeroprofile.zip'
+
         if not os.path.exists(empty_profile):
             empty_profile = 'gologin_zeroprofile.zip'
-        shutil.copy(empty_profile, self.profile_zip_path)
+
+        if os.path.exists(empty_profile):
+            shutil.copy(empty_profile, self.profile_zip_path)
+
+        if not os.path.exists(empty_profile):
+            print('downloading zero profile')
+            source = requests.get(PROFILES_URL + 'zero_profile.zip')
+            with open(self.profile_zip_path, 'wb') as profile_zip:
+                profile_zip.write(source.content)
+
 
     def extractProfileZip(self):
+
         with zipfile.ZipFile(self.profile_zip_path, 'r') as zip_ref:
             zip_ref.extractall(self.profile_path)
+        print('profile extracted', self.profile_path)
         os.remove(self.profile_zip_path)
 
     def getGeolocationParams(self, profileGeolocationParams, tzGeolocationParams):
         if profileGeolocationParams.get('fillBasedOnIp'):
             return {
                 'mode': profileGeolocationParams['mode'],
                 'latitude': float(tzGeolocationParams['latitude']),
@@ -570,26 +590,69 @@
         if self.credentials_enable_service != None:
             preferences['credentials_enable_service'] = self.credentials_enable_service
         preferences['gologin'] = gologin
         pfile = open(pref_file, 'w')
         json.dump(preferences, pfile)
 
     def createStartup(self):
+        print('createStartup', self.profile_path)
         if self.local == False and os.path.exists(self.profile_path):
             try:
                 shutil.rmtree(self.profile_path)
             except:
                 print("error removing profile", self.profile_path)
         self.profile = self.getProfile()
         if self.local == False:
             self.downloadProfileZip()
         self.updatePreferences()
 
+        print('writeCookiesFromServer', self.writeCookiesFromServer)
+        if self.writeCookiesFromServer:
+            self.downloadCookies()
+            print('cookies downloaded')
         return self.profile_path
 
+
+    def downloadCookies(self):
+        api_base_url = API_URL
+        access_token = self.access_token
+
+        cookiesManagerInst = CookiesManager(
+            profile_id = self.profile_id,
+            tmpdir = self.tmpdir
+        );
+
+        try:
+            response = requests.get(f"{api_base_url}/browser/{self.profile_id}/cookies", headers={
+                'Authorization': f'Bearer {self.access_token}',
+                'user-agent': 'Selenium-API'
+            })
+
+            cookies = response.json()
+            print('COOKIES LENGTH', len(cookies))
+            cookiesManagerInst.write_cookies_to_file(cookies)
+        except Exception as e:
+            print('downloadCookies exc', e, e.__traceback__.tb_lineno)
+            raise e
+
+
+    def uploadCookies(self, cookies):
+        api_base_url = API_URL
+        access_token = self.access_token
+
+        try:
+            response = requests.post(f"{api_base_url}/browser/{self.profile_id}/cookies/?encrypted=true", headers={
+                'Authorization': f'Bearer {self.access_token}',
+                'User-Agent': 'Selenium-API'
+            }, json=cookies)
+            return response
+        except Exception as e:
+            print('uploadCookies', e)
+            return e
+
     def headers(self):
         return {
             'Authorization': 'Bearer ' + self.access_token,
             'User-Agent': 'Selenium-API'
         }
 
     def getRandomFingerprint(self, options):
```

### Comparing `gologin-2024.4.4122950/gologin.egg-info/PKG-INFO` & `gologin-2024.5.12063328/gologin.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gologin
-Version: 2024.4.4122950
+Version: 2024.5.12063328
 Summary: Official GoLogin python package
 Home-page: https://github.com/gologinapp/pygologin
 Author: GoLogin
 Author-email: yuri@gologin.com
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: gologin Version: 2024.4.4122950 Summary: Official
+Metadata-Version: 2.1 Name: gologin Version: 2024.5.12063328 Summary: Official
 GoLogin python package Home-page: https://github.com/gologinapp/pygologin
 Author: GoLogin Author-email: yuri@gologin.com Requires-Python: >=3.5
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 requests Requires-Dist: psutil # pygologin REST API provides programmatic
 access to GoLogin App. Create a new browser profile, get a list of all browser
 profiles, add a browser profile and running # class GoLogin - class for working
 with _g_o_l_o_g_i_n_._c_o_m API # Official Package ## Getting Started GoLogin supports
```

### Comparing `gologin-2024.4.4122950/setup.py` & `gologin-2024.5.12063328/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("requirements.txt", "r") as f:
     install_requires = [line.strip() for line in f.readlines()]
 
 setup(
     name='gologin',
-    version='2024.04.04122950',
+    version='2024.05.12063328',
     packages=find_packages(),
     install_requires=install_requires,
     author='GoLogin',
     author_email='yuri@gologin.com',
     description='Official GoLogin python package',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
```

