# Comparing `tmp/bltzr-0.1.1.tar.gz` & `tmp/bltzr-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bltzr-0.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "bltzr-0.1.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `bltzr-0.1.1.tar` & `bltzr-0.1.2.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0       77 2024-05-10 22:07:11.834380 bltzr-0.1.1/.gitignore
--rw-r--r--   0        0        0    32422 2024-05-10 21:57:53.815373 bltzr-0.1.1/LICENSE
--rw-r--r--   0        0        0       36 2024-05-10 22:02:00.244932 bltzr-0.1.1/README.md
--rw-r--r--   0        0        0      408 2024-05-10 22:00:38.155078 bltzr-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      111 2024-05-10 22:04:02.764715 bltzr-0.1.1/src/bltzr/__init__.py
--rw-r--r--   0        0        0     4095 2024-05-10 21:55:11.962332 bltzr-0.1.1/src/bltzr/tokenizer.py
--rw-r--r--   0        0        0      315 1970-01-01 00:00:00.000000 bltzr-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       77 2024-05-10 22:07:11.834380 bltzr-0.1.2/.gitignore
+-rw-r--r--   0        0        0    32422 2024-05-10 21:57:53.815373 bltzr-0.1.2/LICENSE
+-rw-r--r--   0        0        0       36 2024-05-10 22:02:00.244932 bltzr-0.1.2/README.md
+-rw-r--r--   0        0        0      429 2024-05-11 00:47:32.828658 bltzr-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      134 2024-05-11 15:23:51.416799 bltzr-0.1.2/src/bltzr/__init__.py
+-rw-r--r--   0        0        0     5427 2024-05-11 15:22:55.960161 bltzr-0.1.2/src/bltzr/dataset.py
+-rw-r--r--   0        0        0     3968 2024-05-11 15:22:55.960161 bltzr-0.1.2/src/bltzr/tokenizer.py
+-rw-r--r--   0        0        0      393 1970-01-01 00:00:00.000000 bltzr-0.1.2/PKG-INFO
```

### Comparing `bltzr-0.1.1/LICENSE` & `bltzr-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bltzr-0.1.1/src/bltzr/tokenizer.py` & `bltzr-0.1.2/src/bltzr/tokenizer.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,19 +35,16 @@
    277: '</REPLY>',    #
 
    278: '<USR>',       # Reserved for future use =)
    279: '<PAD>'        # The last special token should always be the padding token
 }
 
 class Tokenizer:
-    def __init__(self, special_tokens=None):
-        if special_tokens is not None:
-            self.special_tokens = special_tokens
-        else:
-            self.special_tokens = SPECIAL_TOKENS
+    def __init__(self):
+        self.special_tokens = SPECIAL_TOKENS
         self.vocab = list(range(256)) + list(self.special_tokens.keys())
 
     def get_token_id(self, token):
         token_list = list(self.special_tokens.values())
         for idx, t in enumerate(token_list):
             if t == token:
                 return 256 + idx
```

