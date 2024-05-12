# Comparing `tmp/mtok-4.3.0.tar.gz` & `tmp/mtok-5.0.0.tar.gz`

## Comparing `mtok-4.3.0.tar` & `mtok-5.0.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 mtok-4.3.0/.github/workflows/publish-on-pip.yml
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 mtok-4.3.0/.idea/.gitignore
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 mtok-4.3.0/.idea/misc.xml
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 mtok-4.3.0/.idea/modules.xml
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 mtok-4.3.0/.idea/mtok.iml
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 mtok-4.3.0/.idea/vcs.xml
--rw-r--r--   0        0        0     2092 2020-02-02 00:00:00.000000 mtok-4.3.0/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 mtok-4.3.0/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 mtok-4.3.0/src/mtok/__init__.py
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 mtok-4.3.0/src/mtok/helpers.py
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 mtok-4.3.0/src/mtok/mtok.py
--rw-r--r--   0        0        0     3510 2020-02-02 00:00:00.000000 mtok-4.3.0/.gitignore
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 mtok-4.3.0/README.md
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 mtok-4.3.0/pyproject.toml
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 mtok-4.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 mtok-5.0.0/.github/workflows/publish-on-pip.yml
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 mtok-5.0.0/.idea/.gitignore
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 mtok-5.0.0/.idea/misc.xml
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 mtok-5.0.0/.idea/modules.xml
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 mtok-5.0.0/.idea/mtok.iml
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 mtok-5.0.0/.idea/vcs.xml
+-rw-r--r--   0        0        0     2092 2020-02-02 00:00:00.000000 mtok-5.0.0/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 mtok-5.0.0/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 mtok-5.0.0/src/mtok/__init__.py
+-rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 mtok-5.0.0/src/mtok/helpers.py
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 mtok-5.0.0/src/mtok/mtok.py
+-rw-r--r--   0        0        0     3510 2020-02-02 00:00:00.000000 mtok-5.0.0/.gitignore
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 mtok-5.0.0/README.md
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 mtok-5.0.0/pyproject.toml
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 mtok-5.0.0/PKG-INFO
```

### Comparing `mtok-4.3.0/.github/workflows/publish-on-pip.yml` & `mtok-5.0.0/.github/workflows/publish-on-pip.yml`

 * *Files identical despite different names*

### Comparing `mtok-4.3.0/.idea/inspectionProfiles/Project_Default.xml` & `mtok-5.0.0/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `mtok-4.3.0/src/mtok/helpers.py` & `mtok-5.0.0/src/mtok/helpers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 import json
 from os import environ
 from pathlib import Path
 
 import requests
 
 class Const :
-    # local GitHub token absolute filepath $HOME/.gt.json, I assume it is in the home directory
-    lg = Path(environ['HOME']) / '.gt.json'
+    # local GitHub token absolute filepath $HOME/.g.json, I assume it is in the home directory
+    lg = Path(environ['HOME']) / '.g.json'
     # GitHub username
     gu = 'imahdimir'
+    g = 'g'
 
 c = Const()
 
-def get_gt() :
+def get_g() :
     with open(c.lg , 'r') as fi :
-        gt = json.load(fi)[c.gu]
+        gt = json.load(fi)[c.g]
     return gt
 
 def get_all_tokens_fr_tokens_repo() -> dict :
     """ Gets all tokens from the private tokens repo """
-    gt = get_gt()
+    gt = get_g()
 
     trg_repo = 'tokens'
     br = 'main'
     fn = 'main.json'
     url = ret_github_url_for_private_access_to_file(gt , trg_repo , br , fn)
 
     r = requests.get(url)
```

### Comparing `mtok-4.3.0/src/mtok/mtok.py` & `mtok-5.0.0/src/mtok/mtok.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from .helpers import c
 from .helpers import get_all_tokens_fr_tokens_repo
-from .helpers import get_gt
+from .helpers import get_g
 
 def get_token(key = None) :
     """ Gets the token by a key from the private tokens repo on my GitHub """
 
     if not c.lg.exists() :
         raise ValueError(f'GitHub Token Not Found.')
 
     # If key is None, return the GitHub token itself
     if key is None :
-        return get_gt()
+        return get_g()
 
     # Get all tokens from the private tokens repo
     all_toks = get_all_tokens_fr_tokens_repo()
 
     target_tok = all_toks[key]
 
     return target_tok
```

### Comparing `mtok-4.3.0/.gitignore` & `mtok-5.0.0/.gitignore`

 * *Files identical despite different names*

