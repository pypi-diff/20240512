# Comparing `tmp/ALLM-1.0.4-py3-none-any.whl.zip` & `tmp/ALLM-1.0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 4081 bytes, number of entries: 5
--rw-rw-rw-  2.0 fat     7664 b- defN 24-May-11 18:27 ALLM-1.0.4.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-11 18:27 ALLM-1.0.4.dist-info/WHEEL
--rw-rw-rw-  2.0 fat      556 b- defN 24-May-11 18:27 ALLM-1.0.4.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat        1 b- defN 24-May-11 18:27 ALLM-1.0.4.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      378 b- defN 24-May-11 18:27 ALLM-1.0.4.dist-info/RECORD
-5 files, 8691 bytes uncompressed, 3373 bytes compressed:  61.2%
+Zip file size: 4076 bytes, number of entries: 5
+-rw-rw-rw-  2.0 fat     7664 b- defN 24-May-11 18:43 ALLM-1.0.5.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-11 18:43 ALLM-1.0.5.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat      517 b- defN 24-May-11 18:43 ALLM-1.0.5.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat        1 b- defN 24-May-11 18:43 ALLM-1.0.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      378 b- defN 24-May-11 18:43 ALLM-1.0.5.dist-info/RECORD
+5 files, 8652 bytes uncompressed, 3368 bytes compressed:  61.1%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
-Filename: ALLM-1.0.4.dist-info/METADATA
+Filename: ALLM-1.0.5.dist-info/METADATA
 Comment: 
 
-Filename: ALLM-1.0.4.dist-info/WHEEL
+Filename: ALLM-1.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: ALLM-1.0.4.dist-info/entry_points.txt
+Filename: ALLM-1.0.5.dist-info/entry_points.txt
 Comment: 
 
-Filename: ALLM-1.0.4.dist-info/top_level.txt
+Filename: ALLM-1.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: ALLM-1.0.4.dist-info/RECORD
+Filename: ALLM-1.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `ALLM-1.0.4.dist-info/METADATA` & `ALLM-1.0.5.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ALLM
-Version: 1.0.4
+Version: 1.0.5
 Summary: A simple and efficient python library for fast inference of GGUF Large Language Models.
 Author: All Advance AI
 Author-email: allmdev@allaai.com
 Maintainer: All Advance AI
 Maintainer-email: allmdev@allaai.com
 Keywords: GGUF,GGUF Large Language Model,GGUF Large Language Models,GGUF Large Language Modeling,GGUF Large Language Modeling Library
 Description-Content-Type: text/markdown
```

## Comparing `ALLM-1.0.4.dist-info/entry_points.txt` & `ALLM-1.0.5.dist-info/entry_points.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [console_scripts]
-allm-agentapi = ALLMDEV.agentapi:main
-allm-agentapi-azure = ALLMDEV.azureagentapi:main
-allm-agentapi-vertex = ALLMDEV.vertexagentapi:main
-allm-agentchat = ALLMDEV.agentchat:main
-allm-agentchat-azure = ALLMDEV.azureagentchat:main
-allm-agentchat-vertex = ALLMDEV.vertexagentchat:main
-allm-newagent = ALLMDEV.newagent:main
-allm-run = ALLMDEV.cli:main
-allm-run-azure = ALLMDEV.azurecli:main
-allm-run-vertex = ALLMDEV.vertexcli:main
-allm-serve = ALLMDEV.serve:main
-allm-studio = ALLMDEV.studio:main
-allm-updateagent = ALLMDEV.updateagent:main
+allm-agentapi = ALLM.agentapi:main
+allm-agentapi-azure = ALLM.azureagentapi:main
+allm-agentapi-vertex = ALLM.vertexagentapi:main
+allm-agentchat = ALLM.agentchat:main
+allm-agentchat-azure = ALLM.azureagentchat:main
+allm-agentchat-vertex = ALLM.vertexagentchat:main
+allm-newagent = ALLM.newagent:main
+allm-run = ALLM.cli:main
+allm-run-azure = ALLM.azurecli:main
+allm-run-vertex = ALLM.vertexcli:main
+allm-serve = ALLM.serve:main
+allm-studio = ALLM.studio:main
+allm-updateagent = ALLM.updateagent:main
```

