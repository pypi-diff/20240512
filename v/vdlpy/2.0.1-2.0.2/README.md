# Comparing `tmp/vdlpy-2.0.1.tar.gz` & `tmp/vdlpy-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vdlpy-2.0.1.tar", last modified: Fri Mar  8 22:07:49 2024, max compression
+gzip compressed data, was "vdlpy-2.0.2.tar", last modified: Sun May 12 11:29:47 2024, max compression
```

## Comparing `vdlpy-2.0.1.tar` & `vdlpy-2.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-03-08 22:07:49.764206 vdlpy-2.0.1/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      409 2023-10-02 10:24:38.000000 vdlpy-2.0.1/LICENSE
--rw-r--r--   0 gitlab-runner   (997) gitlab-runner   (997)      980 2024-03-08 22:07:49.764206 vdlpy-2.0.1/PKG-INFO
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      383 2023-10-02 10:24:38.000000 vdlpy-2.0.1/README.md
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       85 2023-10-02 10:24:38.000000 vdlpy-2.0.1/pyproject.toml
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      711 2024-03-08 22:07:49.764206 vdlpy-2.0.1/setup.cfg
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-03-08 22:07:49.760206 vdlpy-2.0.1/src/
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-03-08 22:07:49.764206 vdlpy-2.0.1/src/vdlpy/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      325 2023-10-02 10:24:38.000000 vdlpy-2.0.1/src/vdlpy/__init__.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     5368 2023-10-02 10:24:38.000000 vdlpy-2.0.1/src/vdlpy/parts.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    37384 2024-02-26 22:24:27.000000 vdlpy-2.0.1/src/vdlpy/vdl.py
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-03-08 22:07:49.764206 vdlpy-2.0.1/src/vdlpy.egg-info/
--rw-r--r--   0 gitlab-runner   (997) gitlab-runner   (997)      980 2024-03-08 22:07:49.000000 vdlpy-2.0.1/src/vdlpy.egg-info/PKG-INFO
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      232 2024-03-08 22:07:49.000000 vdlpy-2.0.1/src/vdlpy.egg-info/SOURCES.txt
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)        1 2024-03-08 22:07:49.000000 vdlpy-2.0.1/src/vdlpy.egg-info/dependency_links.txt
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)        6 2024-03-08 22:07:49.000000 vdlpy-2.0.1/src/vdlpy.egg-info/top_level.txt
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-05-12 11:29:47.328141 vdlpy-2.0.2/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      409 2023-10-02 10:24:38.000000 vdlpy-2.0.2/LICENSE
+-rw-r--r--   0 gitlab-runner   (997) gitlab-runner   (997)      980 2024-05-12 11:29:47.328141 vdlpy-2.0.2/PKG-INFO
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      383 2023-10-02 10:24:38.000000 vdlpy-2.0.2/README.md
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       85 2023-10-02 10:24:38.000000 vdlpy-2.0.2/pyproject.toml
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      711 2024-05-12 11:29:47.328141 vdlpy-2.0.2/setup.cfg
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-05-12 11:29:47.324141 vdlpy-2.0.2/src/
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-05-12 11:29:47.328141 vdlpy-2.0.2/src/vdlpy/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      325 2023-10-02 10:24:38.000000 vdlpy-2.0.2/src/vdlpy/__init__.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     5368 2023-10-02 10:24:38.000000 vdlpy-2.0.2/src/vdlpy/parts.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    38243 2024-05-12 11:29:41.000000 vdlpy-2.0.2/src/vdlpy/vdl.py
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-05-12 11:29:47.328141 vdlpy-2.0.2/src/vdlpy.egg-info/
+-rw-r--r--   0 gitlab-runner   (997) gitlab-runner   (997)      980 2024-05-12 11:29:47.000000 vdlpy-2.0.2/src/vdlpy.egg-info/PKG-INFO
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      232 2024-05-12 11:29:47.000000 vdlpy-2.0.2/src/vdlpy.egg-info/SOURCES.txt
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)        1 2024-05-12 11:29:47.000000 vdlpy-2.0.2/src/vdlpy.egg-info/dependency_links.txt
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)        6 2024-05-12 11:29:47.000000 vdlpy-2.0.2/src/vdlpy.egg-info/top_level.txt
```

### Comparing `vdlpy-2.0.1/PKG-INFO` & `vdlpy-2.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdlpy
-Version: 2.0.1
+Version: 2.0.2
 Summary: Python interface to virtual data lakes
 Home-page: https://gitlab.com/vdl-open/pi/
 Author: Chris Harding
 Author-email: chris@lacibus.net
 Project-URL: Documentation, https://vdl-open.gitlab.io/pi/vdlpy.html
 Project-URL: Issue Tracker, https://gitlab.com/vdl-open/pi/-/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `vdlpy-2.0.1/setup.cfg` & `vdlpy-2.0.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = vdlpy
-version = 2.0.1
+version = 2.0.2
 author = Chris Harding
 author_email = chris@lacibus.net
 description = Python interface to virtual data lakes
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://gitlab.com/vdl-open/pi/
 project_urls =
```

### Comparing `vdlpy-2.0.1/src/vdlpy/parts.py` & `vdlpy-2.0.2/src/vdlpy/parts.py`

 * *Files identical despite different names*

### Comparing `vdlpy-2.0.1/src/vdlpy/vdl.py` & `vdlpy-2.0.2/src/vdlpy/vdl.py`

 * *Files 6% similar despite different names*

```diff
@@ -186,22 +186,22 @@
         for change in changes:
             scanned_change = {}
         
             if isinstance(change, CreateItem):
                 scanned_change['change'] = 'create item'
                 scanned_change['handle'] = change.handle
                 scanned_change['source'] = change.source
-                if change.read is not None: scanned_change['read'] = change.read.itemid
-                if change.write is not None: scanned_change['write'] = change.write.itemid
+                if change.read is not None: scanned_change['read'] = repr(change.read)
+                if change.write is not None: scanned_change['write'] = repr(change.write)
         
             elif isinstance(change, UpdateItem):
                 scanned_change['change'] = 'update item'
                 scanned_change['item'] = change.item.itemid
-                if change.read is not None: scanned_change['read'] = change.read.itemid
-                if change.write is not None: scanned_change['write'] = change.write.itemid
+                if change.read is not None: scanned_change['read'] = repr(change.read)
+                if change.write is not None: scanned_change['write'] = repr(change.write)
         
             elif isinstance(change, DeleteItem):
                 scanned_change['change'] = 'delete item'
                 scanned_change['item'] = change.item.itemid
         
             elif isinstance(change, PutTriple):
                 scanned_change['change'] = 'put triple'
@@ -263,17 +263,24 @@
 
 class Constraint:
     '''
     A constraint on data to be retrieved from a virtual data lake.
     It has a subject, a verb, and an object, each of which can be
     given or unknown.
     
+    A given can be an item, a boolean, an int, a float, a string, 
+    a bytes object or a bytearray object. If it is an item, it can
+    be an `Itm` object or a `NamedItm` object. If it is not an item,
+    it is a python quantity of the appropriate type. 
+    
+    An unknown is a vdl Unknown object.
+    
     If a subject or a verb is given, then it must be an `Itm` object
     or a `NamedItm` object, because the subjects and verbs of triples
-    are items.  If an object of a constraint is given, it can be an 
+    are items.  If an object of a constraint is given, it can be an
     `Itm` object, a `NamedItm` object, a boolean, an int, a float,
     a string, a bytes object or a bytearray object. If a subject,
     verb or object is unknown, then it is an `Unknown` object.
     
     The data retrieved from a virtual data lake using a list of constraints
     consists of a list of dictionaries. Each dictionary represents a
     solution that satisfies the constraints. The dictionary maps the 
@@ -284,22 +291,19 @@
     unknown.
     '''
     
     def __init__(self, subj, vrb, obj):
         '''
         Construct a Constraint.
         
-        The supplied subject and verb can each be:
-          * an `Itm` object
-          * an `ItmName` object
-          * an `Unknown` object
+        The supplied subject and verb can each be an item or
+        an `Unknown` object
         
         The supplied object can be:
-          * an `Itm` object
-          * an `ItmName` object
+          * an item
           * an `Unknown` object
           * a bool
           * an int
           * a float
           * a str
           * a bytes object
           * a bytearray object
@@ -384,20 +388,23 @@
           * handle: a handle that can be used to refer to the created item 
             in subsequent changes. It can be supplied as an alphanumeric 
             string or as an `Unknown` object whose name is to be used as the
             handle. 
           * source(int): the numeric identifier of the source in which
             the item is to be created.
           * read: the read access level of the item to be created. 
-            This can be an `Itm` object or an `ItmName` object. 
-            It defaults to the access level of the session making the
-            request.
+            This is an item, specified as an `Itm` object or a `NamedItm`
+            object. It defaults to the access level of the session making
+            the request. Note that access levels defined in a source are
+            named items, even though they aren't shown on the source's Items
+            page. For example, the 'admin' access level of source 12 is 
+            NamedItem(12, 'admin').
           * write: the write access level of the item to be created. 
-            This can be an `Itm` object or an `ItmName` object. 
-            It defaults to the access level of the session making the
+            This is an item, specified as an `Itm` object or a `NamedItm`
+            object. It defaults to the access level of the session making the
             request.
             
         Raises: 
           * VdlException if the handle is neither a string nor an `Unknown` object.
         '''
         
         if isinstance(handle, str): self.handle = handle
@@ -424,19 +431,22 @@
     def __init__(self, item, read, write=None):
         '''
         Construct a virtual data lake change that updates an item.
         
         Parameters:
           * item(`Itm`) the item to be updated.
           * read: the read access level that the item is to have. 
-            This can be an `Itm` object or an `ItmName` object. 
-            If it is None then the item's read level is not changed.
+            This is an item, specified as an `Itm` object or a `NamedItem`
+            object. If it is None then the item's read level is not changed.
+            Note that access levels defined in a source are named items, even
+            though they aren't shown on the source's Items page. For example,
+            the 'admin' access level of source 12 is NamedItem(12, 'admin').
           * write: the write access level that the item is to have. 
-            This can be an `Itm` object or an `ItmName` object. 
-            If it is not supplied or None then the item's write level
+            This is an item, specified as an `Itm` object or a `NamedItem`
+            object. If it is not supplied or None then the item's write level
             is not changed.
             
         Raises: 
           * VdlException if the item is not an `Itm` object, or if the
             read and write levels are both None.
         '''
         
@@ -491,24 +501,24 @@
         Construct a virtual data lake change that puts a triple.
         
         This method ensures that a triple with the given subject,
         verb and object exists in the virtual data lake. If one
         exists already, a new one will not be created.
         
         Parameters:
-          * subj: the subject. This can be specified by an `Itm` object, 
-            an `ItmName` object, or an `Unknown` that is the handle of 
-            an object created in a previous change.
-          * vrb: the verb. This can be specified by an `Itm` object, 
-            an `ItmName` object, or an `Unknown` that is the handle of 
-            an object created in a previous change.
+          * subj: the subject. This can be an item, specified as an
+            `Itm` object or a `NamedItem` object, or an `Unknown` that
+            is the handle of an object created in a previous change.
+          * vrb: the verb. This can be an item, specified as an `Itm`
+            object or a `NamedItem` object, or an `Unknown` that is 
+            the handle of an object created in a previous change.
           * obj: the object. This can be an item, a Boolean, an integer, 
             a real number, a text object or a binary object. An item is
-            specified by an `Itm` object, an `ItmName` object, or an
-            `Unknown` that is the handle of an object created in a 
+            specified as an `Itm` object or a `NamedItem` object, or is
+            an `Unknown` that is the handle of an object created in a
             previous change. A Boolean is given as a bool, an integer as 
             an int, a real number as a float, a text object as a string, 
             and a binary object as either a bytes or a bytearray.
         '''
     
         self.subj = subj
         self.vrb = vrb
@@ -529,21 +539,21 @@
         Construct a virtual data lake change that removes one or more triples.
         If an object is given, all triples with the given subject,
         verb and object are removed. (Normally, there will only be one
         such triple.) If no object is given, all triples with the given
         subject and verb are removed.
         
         Parameters:
-          * subj: the subject. This can be specified by an `Itm` object 
-            or an `ItmName` object.
-          * vrb: the verb. This can be specified by an `Itm` object or 
-            an `ItmName` object.
+          * subj: the subject. This is an item, specified as an `Itm`
+            object or a `NamedItem` object.
+          * vrb: the verb. This is an item, specified as an `Itm` object
+            or a `NamedItem` object.
           * obj: the object. This can be an item, a Boolean, an integer, 
             a real number, a text object or a binary object. An item is
-            specified by an `Itm` object or an `ItmName` object. A Boolean
+            specified as an `Itm` object or a `NamedItem`  object. A Boolean
             is given as a bool, an integer as an int, a real number as a
             float, a text object as a string, and a binary object as either
             a bytes or a bytearray.
         '''
     
         self.subj = subj
         self.vrb = vrb
@@ -573,25 +583,25 @@
         
         If a triple with the subject, verb and object exists already, 
         a new one need not be created. If more than one triple 
         with the given subject and verb exists, then all but one
         will be deleted.
         
         Parameters:
-          * subj: the subject. This can be specified by an `Itm` object, 
-            or an `ItmName` object.
-          * vrb: the verb. This can be specified by an `Itm` object, 
-            or an `ItmName` object.
+          * subj: the subject. This is specified as an `Itm` object or a
+            `NamedItem` object.
+          * vrb: the verb. This is specified as an `Itm` object or a
+            `NamedItem` object.
           * obj: the object. This can be an item, a Boolean, an integer, 
-            a real number, a text object or a binary object. An item is
-            specified by an `Itm` object, an `ItmName` object, or a 
-            handle of an object created in a previous change. A Boolean
-            is given as a bool, an integer as an int, a real number as a
-            float, a text object as a string, and a binary object as either
-            a bytes or a bytearray.
+            a real number, a text object or a binary object. An item can
+            be specified as an `Itm` object or a `NamedItem` object, or by
+            an `Unknown` that is the handle of an object created in a
+            previous change. A Boolean is given as a bool, an integer as an
+            int, a real number as a float, a text object as a string, and a
+            binary object as either a bytes or a bytearray.
         '''
     
         self.subj = subj
         self.vrb = vrb
         self.obj = obj
         
         
@@ -917,19 +927,19 @@
         bytearray object.
       
     For an 'unknown' entry, the value is a dict with one entry:
     'unknown' whose value is the name of the unknown.
     
     Parameters:
       * spec: a specification of the subject, verb, or object.
-        For a given item, this can be an `Itm` or `ItmName` object. 
-        For a given piece of data, it can be a bool, int, float, or
-        str. For a binary object, it is the name of a files dict entry
-        whose value is a bytes, or bytearray object. For an unknown 
-        quantity, it is an `Unknown` object.
+        For a given item, this can be specified as an `Itm` object
+        or a `NamedItem` object. For a given piece of data, it can be
+        a bool, int, float, or str. For a binary object, it is the name
+        of a files dict entry whose value is a bytes, or bytearray
+        object. For an unknown quantity, it is an `Unknown` object.
       
     Raises:
       * VdlException if the specification is invalid
       
     Returns:
       * the representation of the specified quantity.
     '''
@@ -953,18 +963,19 @@
       * TEXT: the value is then a str
       * BINARY: the value is then the name of an entry in the
         files dict, and the value of that entry is a bytes or 
         bytearray object.
     
     Parameters:
       * spec: a specification of the subject, verb, or object.
-        For a given item, this can be an `Itm` or `ItmName` object. 
-        For a given piece of data, it can be a bool, int, float, or
-        str. For a binary object, it is the name of a files dict entry
-        whose value is a bytes, or bytearray object. 
+        For a given item, this can be specified as an `Itm` object
+        or a `NamedItem` object. For a given piece of data, it can
+        be a  bool, int, float, or str. For a binary object, it is
+        the name of a files dict entry whose value is a bytes, or
+        bytearray object. 
       * files: a dict of binary values
       
     Raises:
       * VdlException if the specification is invalid
       
     Returns:
       * the representation of the specified quantity.
```

### Comparing `vdlpy-2.0.1/src/vdlpy.egg-info/PKG-INFO` & `vdlpy-2.0.2/src/vdlpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdlpy
-Version: 2.0.1
+Version: 2.0.2
 Summary: Python interface to virtual data lakes
 Home-page: https://gitlab.com/vdl-open/pi/
 Author: Chris Harding
 Author-email: chris@lacibus.net
 Project-URL: Documentation, https://vdl-open.gitlab.io/pi/vdlpy.html
 Project-URL: Issue Tracker, https://gitlab.com/vdl-open/pi/-/issues
 Classifier: Programming Language :: Python :: 3
```

