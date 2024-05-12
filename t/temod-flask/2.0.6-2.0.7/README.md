# Comparing `tmp/temod-flask-2.0.6.tar.gz` & `tmp/temod_flask-2.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "temod-flask-2.0.6.tar", last modified: Thu Feb 29 20:12:50 2024, max compression
+gzip compressed data, was "temod_flask-2.0.7.tar", last modified: Sun May 12 12:25:53 2024, max compression
```

## Comparing `temod-flask-2.0.6.tar` & `temod_flask-2.0.7.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 oem      (29999) oem      (29999)        0 2024-02-29 20:12:50.271729 temod-flask-2.0.6/
--rw-rw-r--   0 oem      (29999) oem      (29999)     1069 2023-07-16 09:53:59.000000 temod-flask-2.0.6/LICENSE.txt
--rw-r--r--   0 oem      (29999) oem      (29999)      761 2024-02-29 20:12:50.271729 temod-flask-2.0.6/PKG-INFO
--rw-rw-r--   0 oem      (29999) oem      (29999)       68 2023-07-16 10:44:24.000000 temod-flask-2.0.6/README.md
--rw-rw-r--   0 oem      (29999) oem      (29999)      755 2024-02-29 20:12:45.000000 temod-flask-2.0.6/pyproject.toml
--rw-rw-r--   0 oem      (29999) oem      (29999)       38 2024-02-29 20:12:50.271729 temod-flask-2.0.6/setup.cfg
-drwxrwxr-x   0 oem      (29999) oem      (29999)        0 2024-02-29 20:12:50.271729 temod-flask-2.0.6/src/
-drwxrwxr-x   0 oem      (29999) oem      (29999)        0 2024-02-29 20:12:50.271729 temod-flask-2.0.6/src/temod_flask/
--rw-rw-r--   0 oem      (29999) oem      (29999)        0 2023-07-15 13:46:19.000000 temod-flask-2.0.6/src/temod_flask/__init__.py
-drwxrwxr-x   0 oem      (29999) oem      (29999)        0 2024-02-29 20:12:50.271729 temod-flask-2.0.6/src/temod_flask/ext/
--rw-rw-r--   0 oem      (29999) oem      (29999)       34 2023-07-15 13:46:19.000000 temod-flask-2.0.6/src/temod_flask/ext/__init__.py
--rw-rw-r--   0 oem      (29999) oem      (29999)     1279 2023-07-15 13:46:20.000000 temod-flask-2.0.6/src/temod_flask/ext/forms.py
-drwxrwxr-x   0 oem      (29999) oem      (29999)        0 2024-02-29 20:12:50.271729 temod-flask-2.0.6/src/temod_flask/security/
-drwxrwxr-x   0 oem      (29999) oem      (29999)        0 2024-02-29 20:12:50.271729 temod-flask-2.0.6/src/temod_flask/security/authentification/
--rw-rw-r--   0 oem      (29999) oem      (29999)       51 2023-07-15 13:46:25.000000 temod-flask-2.0.6/src/temod_flask/security/authentification/__init__.py
--rw-rw-r--   0 oem      (29999) oem      (29999)     5629 2024-02-29 19:59:17.000000 temod-flask-2.0.6/src/temod_flask/security/authentification/authenticators.py
--rw-rw-r--   0 oem      (29999) oem      (29999)      103 2024-02-19 14:46:44.000000 temod-flask-2.0.6/src/temod_flask/security/authentification/exceptions.py
--rw-rw-r--   0 oem      (29999) oem      (29999)     4322 2024-02-29 19:57:28.000000 temod-flask-2.0.6/src/temod_flask/security/authentification/users.py
-drwxrwxr-x   0 oem      (29999) oem      (29999)        0 2024-02-29 20:12:50.271729 temod-flask-2.0.6/src/temod_flask/security/authority/
--rw-rw-r--   0 oem      (29999) oem      (29999)       66 2023-07-15 13:46:23.000000 temod-flask-2.0.6/src/temod_flask/security/authority/__init__.py
--rw-rw-r--   0 oem      (29999) oem      (29999)     1683 2023-07-15 13:46:20.000000 temod-flask-2.0.6/src/temod_flask/security/authority/alarm.py
--rw-rw-r--   0 oem      (29999) oem      (29999)      920 2023-07-15 13:46:23.000000 temod-flask-2.0.6/src/temod_flask/security/authority/exceptions.py
--rw-rw-r--   0 oem      (29999) oem      (29999)     4762 2023-07-15 13:46:23.000000 temod-flask-2.0.6/src/temod_flask/security/authority/gardian.py
--rw-rw-r--   0 oem      (29999) oem      (29999)     2310 2023-07-15 13:46:20.000000 temod-flask-2.0.6/src/temod_flask/security/authority/right.py
--rw-rw-r--   0 oem      (29999) oem      (29999)      167 2023-07-15 13:46:23.000000 temod-flask-2.0.6/src/temod_flask/security/authority/utils.py
-drwxrwxr-x   0 oem      (29999) oem      (29999)        0 2024-02-29 20:12:50.271729 temod-flask-2.0.6/src/temod_flask/utils/
--rw-rw-r--   0 oem      (29999) oem      (29999)       30 2023-07-15 13:46:18.000000 temod-flask-2.0.6/src/temod_flask/utils/__init__.py
--rw-rw-r--   0 oem      (29999) oem      (29999)      787 2023-07-15 13:46:18.000000 temod-flask-2.0.6/src/temod_flask/utils/content_readers.py
-drwxrwxr-x   0 oem      (29999) oem      (29999)        0 2024-02-29 20:12:50.271729 temod-flask-2.0.6/src/temod_flask.egg-info/
--rw-r--r--   0 oem      (29999) oem      (29999)      761 2024-02-29 20:12:50.000000 temod-flask-2.0.6/src/temod_flask.egg-info/PKG-INFO
--rw-rw-r--   0 oem      (29999) oem      (29999)      889 2024-02-29 20:12:50.000000 temod-flask-2.0.6/src/temod_flask.egg-info/SOURCES.txt
--rw-rw-r--   0 oem      (29999) oem      (29999)        1 2024-02-29 20:12:50.000000 temod-flask-2.0.6/src/temod_flask.egg-info/dependency_links.txt
--rw-rw-r--   0 oem      (29999) oem      (29999)       78 2024-02-29 20:12:50.000000 temod-flask-2.0.6/src/temod_flask.egg-info/requires.txt
--rw-rw-r--   0 oem      (29999) oem      (29999)       12 2024-02-29 20:12:50.000000 temod-flask-2.0.6/src/temod_flask.egg-info/top_level.txt
+drwxrwxr-x   0 oem      (29999) oem      (29999)        0 2024-05-12 12:25:53.082412 temod_flask-2.0.7/
+-rw-rw-r--   0 oem      (29999) oem      (29999)     1069 2023-07-16 09:53:59.000000 temod_flask-2.0.7/LICENSE.txt
+-rw-r--r--   0 oem      (29999) oem      (29999)      761 2024-05-12 12:25:53.082412 temod_flask-2.0.7/PKG-INFO
+-rw-rw-r--   0 oem      (29999) oem      (29999)       68 2023-07-16 10:44:24.000000 temod_flask-2.0.7/README.md
+-rw-rw-r--   0 oem      (29999) oem      (29999)      755 2024-05-12 12:25:45.000000 temod_flask-2.0.7/pyproject.toml
+-rw-rw-r--   0 oem      (29999) oem      (29999)       38 2024-05-12 12:25:53.082412 temod_flask-2.0.7/setup.cfg
+drwxrwxr-x   0 oem      (29999) oem      (29999)        0 2024-05-12 12:25:53.078412 temod_flask-2.0.7/src/
+drwxrwxr-x   0 oem      (29999) oem      (29999)        0 2024-05-12 12:25:53.078412 temod_flask-2.0.7/src/temod_flask/
+-rw-rw-r--   0 oem      (29999) oem      (29999)        0 2023-07-15 13:46:19.000000 temod_flask-2.0.7/src/temod_flask/__init__.py
+drwxrwxr-x   0 oem      (29999) oem      (29999)        0 2024-05-12 12:25:53.078412 temod_flask-2.0.7/src/temod_flask/ext/
+-rw-rw-r--   0 oem      (29999) oem      (29999)       34 2023-07-15 13:46:19.000000 temod_flask-2.0.7/src/temod_flask/ext/__init__.py
+-rw-rw-r--   0 oem      (29999) oem      (29999)     1279 2023-07-15 13:46:20.000000 temod_flask-2.0.7/src/temod_flask/ext/forms.py
+drwxrwxr-x   0 oem      (29999) oem      (29999)        0 2024-05-12 12:25:53.078412 temod_flask-2.0.7/src/temod_flask/security/
+drwxrwxr-x   0 oem      (29999) oem      (29999)        0 2024-05-12 12:25:53.082412 temod_flask-2.0.7/src/temod_flask/security/authentification/
+-rw-rw-r--   0 oem      (29999) oem      (29999)       51 2023-07-15 13:46:25.000000 temod_flask-2.0.7/src/temod_flask/security/authentification/__init__.py
+-rw-rw-r--   0 oem      (29999) oem      (29999)     5709 2024-05-12 12:20:51.000000 temod_flask-2.0.7/src/temod_flask/security/authentification/authenticators.py
+-rw-rw-r--   0 oem      (29999) oem      (29999)      103 2024-02-19 14:46:44.000000 temod_flask-2.0.7/src/temod_flask/security/authentification/exceptions.py
+-rw-rw-r--   0 oem      (29999) oem      (29999)     4390 2024-05-12 12:25:13.000000 temod_flask-2.0.7/src/temod_flask/security/authentification/users.py
+drwxrwxr-x   0 oem      (29999) oem      (29999)        0 2024-05-12 12:25:53.082412 temod_flask-2.0.7/src/temod_flask/security/authority/
+-rw-rw-r--   0 oem      (29999) oem      (29999)       66 2023-07-15 13:46:23.000000 temod_flask-2.0.7/src/temod_flask/security/authority/__init__.py
+-rw-rw-r--   0 oem      (29999) oem      (29999)     1683 2023-07-15 13:46:20.000000 temod_flask-2.0.7/src/temod_flask/security/authority/alarm.py
+-rw-rw-r--   0 oem      (29999) oem      (29999)      920 2023-07-15 13:46:23.000000 temod_flask-2.0.7/src/temod_flask/security/authority/exceptions.py
+-rw-rw-r--   0 oem      (29999) oem      (29999)     4762 2023-07-15 13:46:23.000000 temod_flask-2.0.7/src/temod_flask/security/authority/gardian.py
+-rw-rw-r--   0 oem      (29999) oem      (29999)     2310 2023-07-15 13:46:20.000000 temod_flask-2.0.7/src/temod_flask/security/authority/right.py
+-rw-rw-r--   0 oem      (29999) oem      (29999)      167 2023-07-15 13:46:23.000000 temod_flask-2.0.7/src/temod_flask/security/authority/utils.py
+drwxrwxr-x   0 oem      (29999) oem      (29999)        0 2024-05-12 12:25:53.082412 temod_flask-2.0.7/src/temod_flask/utils/
+-rw-rw-r--   0 oem      (29999) oem      (29999)       30 2023-07-15 13:46:18.000000 temod_flask-2.0.7/src/temod_flask/utils/__init__.py
+-rw-rw-r--   0 oem      (29999) oem      (29999)      787 2023-07-15 13:46:18.000000 temod_flask-2.0.7/src/temod_flask/utils/content_readers.py
+drwxrwxr-x   0 oem      (29999) oem      (29999)        0 2024-05-12 12:25:53.082412 temod_flask-2.0.7/src/temod_flask.egg-info/
+-rw-r--r--   0 oem      (29999) oem      (29999)      761 2024-05-12 12:25:53.000000 temod_flask-2.0.7/src/temod_flask.egg-info/PKG-INFO
+-rw-rw-r--   0 oem      (29999) oem      (29999)      889 2024-05-12 12:25:53.000000 temod_flask-2.0.7/src/temod_flask.egg-info/SOURCES.txt
+-rw-rw-r--   0 oem      (29999) oem      (29999)        1 2024-05-12 12:25:53.000000 temod_flask-2.0.7/src/temod_flask.egg-info/dependency_links.txt
+-rw-rw-r--   0 oem      (29999) oem      (29999)       78 2024-05-12 12:25:53.000000 temod_flask-2.0.7/src/temod_flask.egg-info/requires.txt
+-rw-rw-r--   0 oem      (29999) oem      (29999)       12 2024-05-12 12:25:53.000000 temod_flask-2.0.7/src/temod_flask.egg-info/top_level.txt
```

### Comparing `temod-flask-2.0.6/LICENSE.txt` & `temod_flask-2.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `temod-flask-2.0.6/PKG-INFO` & `temod_flask-2.0.7/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: temod-flask
-Version: 2.0.6
+Version: 2.0.7
 Summary: Connects python-flask features with Temod data models
 Author-email: PyAxolotl <abdellatifzied.saada@gmail.com>
 Project-URL: Homepage, https://github.com/TuburboMajus/temod-flask
 Project-URL: Bug Tracker, https://github.com/TuburboMajus/temod-flask/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `temod-flask-2.0.6/pyproject.toml` & `temod_flask-2.0.7/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['setuptools>=42']
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = "temod-flask"
-version = "2.0.6"
+version = "2.0.7"
 authors = [
   { name="PyAxolotl", email="abdellatifzied.saada@gmail.com" },
 ]
 description = "Connects python-flask features with Temod data models"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `temod-flask-2.0.6/src/temod_flask/ext/forms.py` & `temod_flask-2.0.7/src/temod_flask/ext/forms.py`

 * *Files identical despite different names*

### Comparing `temod-flask-2.0.6/src/temod_flask/security/authentification/authenticators.py` & `temod_flask-2.0.7/src/temod_flask/security/authentification/authenticators.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,17 @@
 		self.login_view = login_view
 		if loader is not None:
 			self.setLoader(loader)
 		self.postload = None;
 		if postload is not None:
 			self.setPostLoader(postload)
 
+	def load_user(self,identifier):
+		return self.loader.load_user(identifier)
+
 	def search_user(self,*logins):
 		return self.loader.search_user(*logins)
 
 	def login_user(self,user):
 		self.loader.login_user(user)
 		return login_user(user)
```

### Comparing `temod-flask-2.0.6/src/temod_flask/security/authentification/users.py` & `temod_flask-2.0.7/src/temod_flask/security/authentification/users.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,12 +108,16 @@
 			return super(TemodUser,self).__getattribute__(name)
 		except:
 			return getattr(self.user,name)
 
 	def get_id(self):
 		return self.user[self.identifier]
 
+	@property
+	def is_anonymous(self):
+		return self.user is None
+
 	def __getitem__(self,name):
 		return self.user[name]
 
 	def __setitem__(self,name,value):
 		self.user[name] = value
```

### Comparing `temod-flask-2.0.6/src/temod_flask/security/authority/alarm.py` & `temod_flask-2.0.7/src/temod_flask/security/authority/alarm.py`

 * *Files identical despite different names*

### Comparing `temod-flask-2.0.6/src/temod_flask/security/authority/exceptions.py` & `temod_flask-2.0.7/src/temod_flask/security/authority/exceptions.py`

 * *Files identical despite different names*

### Comparing `temod-flask-2.0.6/src/temod_flask/security/authority/gardian.py` & `temod_flask-2.0.7/src/temod_flask/security/authority/gardian.py`

 * *Files identical despite different names*

### Comparing `temod-flask-2.0.6/src/temod_flask/security/authority/right.py` & `temod_flask-2.0.7/src/temod_flask/security/authority/right.py`

 * *Files identical despite different names*

### Comparing `temod-flask-2.0.6/src/temod_flask/utils/content_readers.py` & `temod_flask-2.0.7/src/temod_flask/utils/content_readers.py`

 * *Files identical despite different names*

### Comparing `temod-flask-2.0.6/src/temod_flask.egg-info/PKG-INFO` & `temod_flask-2.0.7/src/temod_flask.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: temod-flask
-Version: 2.0.6
+Version: 2.0.7
 Summary: Connects python-flask features with Temod data models
 Author-email: PyAxolotl <abdellatifzied.saada@gmail.com>
 Project-URL: Homepage, https://github.com/TuburboMajus/temod-flask
 Project-URL: Bug Tracker, https://github.com/TuburboMajus/temod-flask/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `temod-flask-2.0.6/src/temod_flask.egg-info/SOURCES.txt` & `temod_flask-2.0.7/src/temod_flask.egg-info/SOURCES.txt`

 * *Files identical despite different names*

