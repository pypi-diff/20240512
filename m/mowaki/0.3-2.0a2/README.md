# Comparing `tmp/mowaki-0.3.tar.gz` & `tmp/mowaki-2.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mowaki-0.3.tar", last modified: Tue Apr  7 18:12:24 2020, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `mowaki-0.3.tar` & `mowaki-2.0a2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 samu      (1000) samu      (1000)        0 2020-04-07 18:12:24.000000 mowaki-0.3/
--rw-r--r--   0 samu      (1000) samu      (1000)     1701 2020-04-07 18:12:24.000000 mowaki-0.3/PKG-INFO
--rw-r--r--   0 samu      (1000) samu      (1000)      730 2020-04-07 18:12:10.000000 mowaki-0.3/README.rst
-drwxr-xr-x   0 samu      (1000) samu      (1000)        0 2020-04-07 18:12:24.000000 mowaki-0.3/mowaki/
--rw-r--r--   0 samu      (1000) samu      (1000)        0 2020-02-24 11:40:19.000000 mowaki-0.3/mowaki/__init__.py
-drwxr-xr-x   0 samu      (1000) samu      (1000)        0 2020-04-07 18:12:24.000000 mowaki-0.3/mowaki/auth/
--rw-r--r--   0 samu      (1000) samu      (1000)        0 2020-02-24 11:40:31.000000 mowaki-0.3/mowaki/auth/__init__.py
--rw-r--r--   0 samu      (1000) samu      (1000)     1611 2020-02-24 11:48:13.000000 mowaki-0.3/mowaki/auth/jwt.py
-drwxr-xr-x   0 samu      (1000) samu      (1000)        0 2020-04-07 18:12:24.000000 mowaki-0.3/mowaki/config/
--rw-r--r--   0 samu      (1000) samu      (1000)     1889 2020-04-07 18:06:05.000000 mowaki-0.3/mowaki/config/__init__.py
-drwxr-xr-x   0 samu      (1000) samu      (1000)        0 2020-04-07 18:12:24.000000 mowaki-0.3/mowaki/storage/
--rw-r--r--   0 samu      (1000) samu      (1000)     1893 2020-02-24 11:40:19.000000 mowaki-0.3/mowaki/storage/__init__.py
--rw-r--r--   0 samu      (1000) samu      (1000)     1668 2020-02-24 11:40:19.000000 mowaki-0.3/mowaki/storage/base.py
--rw-r--r--   0 samu      (1000) samu      (1000)     2045 2020-02-24 11:40:19.000000 mowaki-0.3/mowaki/storage/storage_file.py
--rw-r--r--   0 samu      (1000) samu      (1000)     3016 2020-02-24 11:40:19.000000 mowaki-0.3/mowaki/storage/storage_memory.py
--rw-r--r--   0 samu      (1000) samu      (1000)     3663 2020-02-24 11:40:19.000000 mowaki-0.3/mowaki/storage/storage_s3.py
--rw-r--r--   0 samu      (1000) samu      (1000)      929 2020-02-24 11:40:19.000000 mowaki-0.3/mowaki/storage/types.py
-drwxr-xr-x   0 samu      (1000) samu      (1000)        0 2020-04-07 18:12:24.000000 mowaki-0.3/mowaki.egg-info/
--rw-r--r--   0 samu      (1000) samu      (1000)     1701 2020-04-07 18:12:24.000000 mowaki-0.3/mowaki.egg-info/PKG-INFO
--rw-r--r--   0 samu      (1000) samu      (1000)      452 2020-04-07 18:12:24.000000 mowaki-0.3/mowaki.egg-info/SOURCES.txt
--rw-r--r--   0 samu      (1000) samu      (1000)        1 2020-04-07 18:12:24.000000 mowaki-0.3/mowaki.egg-info/dependency_links.txt
--rw-r--r--   0 samu      (1000) samu      (1000)        1 2020-02-24 11:49:06.000000 mowaki-0.3/mowaki.egg-info/not-zip-safe
--rw-r--r--   0 samu      (1000) samu      (1000)       57 2020-04-07 18:12:24.000000 mowaki-0.3/mowaki.egg-info/requires.txt
--rw-r--r--   0 samu      (1000) samu      (1000)        7 2020-04-07 18:12:24.000000 mowaki-0.3/mowaki.egg-info/top_level.txt
--rw-r--r--   0 samu      (1000) samu      (1000)       38 2020-04-07 18:12:24.000000 mowaki-0.3/setup.cfg
--rw-r--r--   0 samu      (1000) samu      (1000)     2024 2020-04-07 18:06:22.000000 mowaki-0.3/setup.py
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 mowaki-2.0a2/.travis.yml
+-rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 mowaki-2.0a2/setup.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mowaki-2.0a2/mowaki/__init__.py
+-rw-r--r--   0        0        0     2538 2020-02-02 00:00:00.000000 mowaki-2.0a2/mowaki/config.py
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 mowaki-2.0a2/mowaki/context.py
+-rw-r--r--   0        0        0     1247 2020-02-02 00:00:00.000000 mowaki-2.0a2/mowaki/crypto.py
+-rw-r--r--   0        0        0     2702 2020-02-02 00:00:00.000000 mowaki-2.0a2/mowaki/database.py
+-rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 mowaki-2.0a2/mowaki/email_composer.py
+-rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 mowaki-2.0a2/mowaki/jwt.py
+-rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 mowaki-2.0a2/mowaki/emailer/__init__.py
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 mowaki-2.0a2/mowaki/emailer/base.py
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 mowaki-2.0a2/mowaki/emailer/dummy.py
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 mowaki-2.0a2/mowaki/emailer/smtp.py
+-rw-r--r--   0        0        0     1893 2020-02-02 00:00:00.000000 mowaki-2.0a2/mowaki/storage/__init__.py
+-rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 mowaki-2.0a2/mowaki/storage/base.py
+-rw-r--r--   0        0        0     2045 2020-02-02 00:00:00.000000 mowaki-2.0a2/mowaki/storage/storage_file.py
+-rw-r--r--   0        0        0     3016 2020-02-02 00:00:00.000000 mowaki-2.0a2/mowaki/storage/storage_memory.py
+-rw-r--r--   0        0        0     3663 2020-02-02 00:00:00.000000 mowaki-2.0a2/mowaki/storage/storage_s3.py
+-rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 mowaki-2.0a2/mowaki/storage/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mowaki-2.0a2/tests/__init__.py
+-rw-r--r--   0        0        0     2592 2020-02-02 00:00:00.000000 mowaki-2.0a2/tests/test_config.py
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 mowaki-2.0a2/.gitignore
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 mowaki-2.0a2/LICENSE
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 mowaki-2.0a2/README.md
+-rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 mowaki-2.0a2/pyproject.toml
+-rw-r--r--   0        0        0     1911 2020-02-02 00:00:00.000000 mowaki-2.0a2/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `mowaki-0.3/mowaki/auth/jwt.py` & `mowaki-2.0a2/mowaki/jwt.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,28 @@
-from datetime import datetime
+from datetime import datetime, timedelta
 
 import jwt
 
 
 class TokenMaker:
 
     """Convenience object for issuing and validating JWT tokens.
 
     Keeps track of (and validates) secret, algorithm, issuer, and
     audience for a particular JWT token type.
     """
 
-    def __init__(self, secret, issuer=None, audience=None, validity=None,
-                 algorithm='HS256'):
-
+    def __init__(
+        self,
+        secret,
+        issuer=None,
+        audience=None,
+        validity=None,
+        algorithm="HS256",
+    ):
         self.secret = secret
         self.issuer = issuer
         self.audience = audience
         self.validity = validity
         self.algorithm = algorithm
 
     def issue(self, subject, validity=None, **kwargs):
@@ -32,33 +37,48 @@
                 Token validity.
 
             exp (datetime.datetime):
                 Token expiration date. Overrides validity.
         """
 
         claim = {
-            'sub': subject,
+            "sub": subject,
         }
 
         if self.issuer is not None:
-            claim['iss'] = self.issuer
+            claim["iss"] = self.issuer
 
         if self.audience is not None:
-            claim['aud'] = self.audience
+            claim["aud"] = self.audience
 
         if validity is None:
             validity = self.validity
 
         if validity is not None:
-            claim['exp'] = datetime.utcnow() + self.validity
+            claim["exp"] = datetime.utcnow() + timedelta(seconds=self.validity)
 
         claim.update(kwargs)
 
         return jwt.encode(claim, self.secret, algorithm=self.algorithm)
 
     def validate(self, token):
-        """Validate a JWT token, returning the contained data
-        """
+        """Validate a JWT token, returning the contained data"""
 
         return jwt.decode(
-            token, self.secret, algorithms=[self.algorithm],
-            issuer=self.issuer, audience=self.audience)
+            token,
+            self.secret,
+            algorithms=[self.algorithm],
+            issuer=self.issuer,
+            audience=self.audience,
+        )
+
+
+def get_unverified_header(token):
+    return jwt.get_unverified_header(token)
+
+
+def get_unverified_token_data(token):
+    return jwt.decode(token, options={"verify_signature": False})
+
+
+def get_token_audience(token):
+    return get_unverified_token_data(token)["aud"]
```

### Comparing `mowaki-0.3/mowaki/storage/__init__.py` & `mowaki-2.0a2/mowaki/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `mowaki-0.3/mowaki/storage/base.py` & `mowaki-2.0a2/mowaki/storage/base.py`

 * *Files identical despite different names*

### Comparing `mowaki-0.3/mowaki/storage/storage_file.py` & `mowaki-2.0a2/mowaki/storage/storage_file.py`

 * *Files identical despite different names*

### Comparing `mowaki-0.3/mowaki/storage/storage_memory.py` & `mowaki-2.0a2/mowaki/storage/storage_memory.py`

 * *Files identical despite different names*

### Comparing `mowaki-0.3/mowaki/storage/storage_s3.py` & `mowaki-2.0a2/mowaki/storage/storage_s3.py`

 * *Files identical despite different names*

### Comparing `mowaki-0.3/mowaki/storage/types.py` & `mowaki-2.0a2/mowaki/storage/types.py`

 * *Files identical despite different names*

