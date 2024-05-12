# Comparing `tmp/sts_lib-0.31.1.tar.gz` & `tmp/sts_lib-0.31.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sts_lib-0.31.1.tar", last modified: Mon May  6 13:02:12 2024, max compression
+gzip compressed data, was "sts_lib-0.31.2.tar", last modified: Sun May 12 07:10:18 2024, max compression
```

## Comparing `sts_lib-0.31.1.tar` & `sts_lib-0.31.2.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 13:02:12.103569 sts_lib-0.31.1/
--rw-rw-rw-   0        0        0    11358 2024-04-19 09:05:26.000000 sts_lib-0.31.1/LICENSE
--rw-rw-rw-   0        0        0       13 2024-04-19 09:05:26.000000 sts_lib-0.31.1/MANIFEST.in
--rw-rw-rw-   0        0        0     6916 2024-05-06 13:02:12.103569 sts_lib-0.31.1/PKG-INFO
--rw-rw-rw-   0        0        0     5463 2024-04-29 19:01:51.000000 sts_lib-0.31.1/README.md
--rw-rw-rw-   0        0        0     1728 2024-05-06 13:02:12.103569 sts_lib-0.31.1/setup.cfg
--rw-rw-rw-   0        0        0       65 2024-04-19 09:05:26.000000 sts_lib-0.31.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-06 13:02:12.056712 sts_lib-0.31.1/sts/
--rw-rw-rw-   0        0        0    52356 2024-05-06 13:01:51.000000 sts_lib-0.31.1/sts/__init__.py
--rw-rw-rw-   0        0        0       89 2024-04-19 09:05:26.000000 sts_lib-0.31.1/sts/__main__.py
--rw-rw-rw-   0        0        0     7551 2024-05-05 14:57:54.000000 sts_lib-0.31.1/sts/cli.py
-drwxrwxrwx   0        0        0        0 2024-05-06 13:02:12.056712 sts_lib-0.31.1/sts/data/
-drwxrwxrwx   0        0        0        0 2024-05-06 13:02:12.072322 sts_lib-0.31.1/sts/data/config/
--rw-rw-rw-   0        0        0      915 2024-05-05 14:57:54.000000 sts_lib-0.31.1/sts/data/config/_default.json
--rw-rw-rw-   0        0        0      608 2024-05-05 08:43:39.000000 sts_lib-0.31.1/sts/data/config/hk2s.json
--rw-rw-rw-   0        0        0      346 2024-05-05 08:43:39.000000 sts_lib-0.31.1/sts/data/config/hk2t.json
--rw-rw-rw-   0        0        0      410 2024-05-05 14:57:54.000000 sts_lib-0.31.1/sts/data/config/jp2t.json
--rw-rw-rw-   0        0        0      419 2024-05-05 14:57:54.000000 sts_lib-0.31.1/sts/data/config/s2hk.json
--rw-rw-rw-   0        0        0      267 2024-05-05 14:57:54.000000 sts_lib-0.31.1/sts/data/config/s2t.json
--rw-rw-rw-   0        0        0      417 2024-05-05 14:57:54.000000 sts_lib-0.31.1/sts/data/config/s2tw.json
--rw-rw-rw-   0        0        0      607 2024-05-05 14:57:54.000000 sts_lib-0.31.1/sts/data/config/s2twp.json
--rw-rw-rw-   0        0        0      247 2024-05-05 08:43:39.000000 sts_lib-0.31.1/sts/data/config/t2hk.json
--rw-rw-rw-   0        0        0      261 2024-05-05 14:57:54.000000 sts_lib-0.31.1/sts/data/config/t2jp.json
--rw-rw-rw-   0        0        0      267 2024-05-05 08:43:39.000000 sts_lib-0.31.1/sts/data/config/t2s.json
--rw-rw-rw-   0        0        0      245 2024-05-05 08:43:39.000000 sts_lib-0.31.1/sts/data/config/t2tw.json
--rw-rw-rw-   0        0        0      606 2024-05-05 08:43:39.000000 sts_lib-0.31.1/sts/data/config/tw2s.json
--rw-rw-rw-   0        0        0      670 2024-05-05 14:57:54.000000 sts_lib-0.31.1/sts/data/config/tw2sp.json
--rw-rw-rw-   0        0        0      344 2024-05-05 08:43:39.000000 sts_lib-0.31.1/sts/data/config/tw2t.json
-drwxrwxrwx   0        0        0        0 2024-05-06 13:02:12.087946 sts_lib-0.31.1/sts/data/dictionary/
--rw-rw-rw-   0        0        0      595 2024-05-05 14:57:54.000000 sts_lib-0.31.1/sts/data/dictionary/HKVariants.txt
--rw-rw-rw-   0        0        0     2865 2024-05-05 08:43:39.000000 sts_lib-0.31.1/sts/data/dictionary/HKVariantsRevPhrases.txt
--rw-rw-rw-   0        0        0      103 2024-05-05 14:57:54.000000 sts_lib-0.31.1/sts/data/dictionary/JPShinjitaiCharacters.txt
--rw-rw-rw-   0        0        0     2720 2024-05-05 08:43:39.000000 sts_lib-0.31.1/sts/data/dictionary/JPShinjitaiPhrases.txt
--rw-rw-rw-   0        0        0     3307 2024-05-05 14:57:54.000000 sts_lib-0.31.1/sts/data/dictionary/JPVariants.txt
--rw-rw-rw-   0        0        0    38333 2024-05-05 14:57:54.000000 sts_lib-0.31.1/sts/data/dictionary/STCharacters.txt
--rw-rw-rw-   0        0        0  1053351 2024-05-05 14:57:54.000000 sts_lib-0.31.1/sts/data/dictionary/STPhrases.txt
--rw-rw-rw-   0        0        0    38740 2024-05-05 14:57:54.000000 sts_lib-0.31.1/sts/data/dictionary/TSCharacters.txt
--rw-rw-rw-   0        0        0     5438 2024-05-05 14:57:54.000000 sts_lib-0.31.1/sts/data/dictionary/TSPhrases.txt
--rw-rw-rw-   0        0        0     8014 2024-05-05 14:57:49.000000 sts_lib-0.31.1/sts/data/dictionary/TWPhrasesIT.txt
--rw-rw-rw-   0        0        0     2205 2024-05-05 08:43:39.000000 sts_lib-0.31.1/sts/data/dictionary/TWPhrasesName.txt
--rw-rw-rw-   0        0        0      608 2024-05-05 14:57:54.000000 sts_lib-0.31.1/sts/data/dictionary/TWPhrasesOther.txt
--rw-rw-rw-   0        0        0      351 2024-05-05 14:57:54.000000 sts_lib-0.31.1/sts/data/dictionary/TWVariants.txt
--rw-rw-rw-   0        0        0     1143 2024-05-05 08:43:39.000000 sts_lib-0.31.1/sts/data/dictionary/TWVariantsRevPhrases.txt
--rw-rw-rw-   0        0        0    22659 2024-05-06 12:58:41.000000 sts_lib-0.31.1/sts/data/htmlpage.tpl.html
-drwxrwxrwx   0        0        0        0 2024-05-06 13:02:12.087946 sts_lib-0.31.1/sts/data/scheme/
--rw-rw-rw-   0        0        0    21633 2024-05-06 13:01:48.000000 sts_lib-0.31.1/sts/data/scheme/st_multi.txt
--rw-rw-rw-   0        0        0      436 2024-05-06 13:01:48.000000 sts_lib-0.31.1/sts/data/scheme/ts_multi.txt
--rw-rw-rw-   0        0        0     2108 2024-05-06 13:01:48.000000 sts_lib-0.31.1/sts/data/scheme/variant.txt
-drwxrwxrwx   0        0        0        0 2024-05-06 13:02:12.103569 sts_lib-0.31.1/sts_lib.egg-info/
--rw-rw-rw-   0        0        0     6916 2024-05-06 13:02:12.000000 sts_lib-0.31.1/sts_lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1325 2024-05-06 13:02:12.000000 sts_lib-0.31.1/sts_lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 13:02:12.000000 sts_lib-0.31.1/sts_lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2024-05-06 13:02:12.000000 sts_lib-0.31.1/sts_lib.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      202 2024-05-06 13:02:12.000000 sts_lib-0.31.1/sts_lib.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-05-06 13:02:12.000000 sts_lib-0.31.1/sts_lib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-12 07:10:18.248735 sts_lib-0.31.2/
+-rw-rw-rw-   0        0        0    11358 2024-04-19 09:05:26.000000 sts_lib-0.31.2/LICENSE
+-rw-rw-rw-   0        0        0       13 2024-04-19 09:05:26.000000 sts_lib-0.31.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     6916 2024-05-12 07:10:18.248735 sts_lib-0.31.2/PKG-INFO
+-rw-rw-rw-   0        0        0     5463 2024-04-29 19:01:51.000000 sts_lib-0.31.2/README.md
+-rw-rw-rw-   0        0        0     1728 2024-05-12 07:10:18.250746 sts_lib-0.31.2/setup.cfg
+-rw-rw-rw-   0        0        0       65 2024-04-19 09:05:26.000000 sts_lib-0.31.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-12 07:10:18.169152 sts_lib-0.31.2/sts/
+-rw-rw-rw-   0        0        0    52886 2024-05-12 07:09:50.000000 sts_lib-0.31.2/sts/__init__.py
+-rw-rw-rw-   0        0        0       89 2024-04-19 09:05:26.000000 sts_lib-0.31.2/sts/__main__.py
+-rw-rw-rw-   0        0        0     7551 2024-05-07 18:11:46.000000 sts_lib-0.31.2/sts/cli.py
+drwxrwxrwx   0        0        0        0 2024-05-12 07:10:18.169152 sts_lib-0.31.2/sts/data/
+drwxrwxrwx   0        0        0        0 2024-05-12 07:10:18.178708 sts_lib-0.31.2/sts/data/config/
+-rw-rw-rw-   0        0        0      915 2024-05-08 13:34:57.000000 sts_lib-0.31.2/sts/data/config/_default.json
+-rw-rw-rw-   0        0        0      608 2024-05-08 13:34:57.000000 sts_lib-0.31.2/sts/data/config/hk2s.json
+-rw-rw-rw-   0        0        0      346 2024-05-08 13:34:57.000000 sts_lib-0.31.2/sts/data/config/hk2t.json
+-rw-rw-rw-   0        0        0      410 2024-05-08 13:34:57.000000 sts_lib-0.31.2/sts/data/config/jp2t.json
+-rw-rw-rw-   0        0        0      419 2024-05-08 13:34:57.000000 sts_lib-0.31.2/sts/data/config/s2hk.json
+-rw-rw-rw-   0        0        0      267 2024-05-08 13:34:57.000000 sts_lib-0.31.2/sts/data/config/s2t.json
+-rw-rw-rw-   0        0        0      417 2024-05-08 13:34:57.000000 sts_lib-0.31.2/sts/data/config/s2tw.json
+-rw-rw-rw-   0        0        0      607 2024-05-08 13:34:57.000000 sts_lib-0.31.2/sts/data/config/s2twp.json
+-rw-rw-rw-   0        0        0      247 2024-05-08 13:34:57.000000 sts_lib-0.31.2/sts/data/config/t2hk.json
+-rw-rw-rw-   0        0        0      261 2024-05-08 13:34:57.000000 sts_lib-0.31.2/sts/data/config/t2jp.json
+-rw-rw-rw-   0        0        0      267 2024-05-08 13:34:57.000000 sts_lib-0.31.2/sts/data/config/t2s.json
+-rw-rw-rw-   0        0        0      245 2024-05-08 13:34:57.000000 sts_lib-0.31.2/sts/data/config/t2tw.json
+-rw-rw-rw-   0        0        0      606 2024-05-08 13:34:57.000000 sts_lib-0.31.2/sts/data/config/tw2s.json
+-rw-rw-rw-   0        0        0      670 2024-05-08 13:34:57.000000 sts_lib-0.31.2/sts/data/config/tw2sp.json
+-rw-rw-rw-   0        0        0      344 2024-05-08 13:34:57.000000 sts_lib-0.31.2/sts/data/config/tw2t.json
+drwxrwxrwx   0        0        0        0 2024-05-12 07:10:18.189169 sts_lib-0.31.2/sts/data/dictionary/
+-rw-rw-rw-   0        0        0      595 2024-05-08 13:34:57.000000 sts_lib-0.31.2/sts/data/dictionary/HKVariants.txt
+-rw-rw-rw-   0        0        0     2865 2024-05-08 13:34:57.000000 sts_lib-0.31.2/sts/data/dictionary/HKVariantsRevPhrases.txt
+-rw-rw-rw-   0        0        0      103 2024-05-08 13:34:57.000000 sts_lib-0.31.2/sts/data/dictionary/JPShinjitaiCharacters.txt
+-rw-rw-rw-   0        0        0     2720 2024-05-08 13:34:57.000000 sts_lib-0.31.2/sts/data/dictionary/JPShinjitaiPhrases.txt
+-rw-rw-rw-   0        0        0     3307 2024-05-08 13:34:57.000000 sts_lib-0.31.2/sts/data/dictionary/JPVariants.txt
+-rw-rw-rw-   0        0        0    38333 2024-05-08 13:34:57.000000 sts_lib-0.31.2/sts/data/dictionary/STCharacters.txt
+-rw-rw-rw-   0        0        0  1053351 2024-05-08 13:34:57.000000 sts_lib-0.31.2/sts/data/dictionary/STPhrases.txt
+-rw-rw-rw-   0        0        0    38740 2024-05-08 13:34:57.000000 sts_lib-0.31.2/sts/data/dictionary/TSCharacters.txt
+-rw-rw-rw-   0        0        0     5438 2024-05-08 13:34:57.000000 sts_lib-0.31.2/sts/data/dictionary/TSPhrases.txt
+-rw-rw-rw-   0        0        0     8014 2024-05-08 13:34:57.000000 sts_lib-0.31.2/sts/data/dictionary/TWPhrasesIT.txt
+-rw-rw-rw-   0        0        0     2205 2024-05-08 13:34:57.000000 sts_lib-0.31.2/sts/data/dictionary/TWPhrasesName.txt
+-rw-rw-rw-   0        0        0      608 2024-05-08 13:34:57.000000 sts_lib-0.31.2/sts/data/dictionary/TWPhrasesOther.txt
+-rw-rw-rw-   0        0        0      351 2024-05-08 13:34:57.000000 sts_lib-0.31.2/sts/data/dictionary/TWVariants.txt
+-rw-rw-rw-   0        0        0     1143 2024-05-08 13:34:57.000000 sts_lib-0.31.2/sts/data/dictionary/TWVariantsRevPhrases.txt
+-rw-rw-rw-   0        0        0    22659 2024-05-11 09:04:03.000000 sts_lib-0.31.2/sts/data/htmlpage.tpl.html
+drwxrwxrwx   0        0        0        0 2024-05-12 07:10:18.219108 sts_lib-0.31.2/sts/data/scheme/
+-rw-rw-rw-   0        0        0    21633 2024-05-11 06:46:32.000000 sts_lib-0.31.2/sts/data/scheme/st_multi.txt
+-rw-rw-rw-   0        0        0      436 2024-05-11 06:46:32.000000 sts_lib-0.31.2/sts/data/scheme/ts_multi.txt
+-rw-rw-rw-   0        0        0     2108 2024-05-11 06:46:32.000000 sts_lib-0.31.2/sts/data/scheme/variant.txt
+drwxrwxrwx   0        0        0        0 2024-05-12 07:10:18.239124 sts_lib-0.31.2/sts_lib.egg-info/
+-rw-rw-rw-   0        0        0     6916 2024-05-12 07:10:18.000000 sts_lib-0.31.2/sts_lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1325 2024-05-12 07:10:18.000000 sts_lib-0.31.2/sts_lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-12 07:10:18.000000 sts_lib-0.31.2/sts_lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2024-05-12 07:10:18.000000 sts_lib-0.31.2/sts_lib.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      202 2024-05-12 07:10:18.000000 sts_lib-0.31.2/sts_lib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-05-12 07:10:18.000000 sts_lib-0.31.2/sts_lib.egg-info/top_level.txt
```

### Comparing `sts_lib-0.31.1/LICENSE` & `sts_lib-0.31.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sts_lib-0.31.1/PKG-INFO` & `sts_lib-0.31.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sts-lib
-Version: 0.31.1
+Version: 0.31.2
 Summary: An open library for flexible simplified-traditional Chinese text conversion.
 Home-page: https://github.com/danny0838/sts-lib
 Author: Danny Lin
 Author-email: danny0838@gmail.com
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: OS Independent
```

### Comparing `sts_lib-0.31.1/README.md` & `sts_lib-0.31.2/README.md`

 * *Files identical despite different names*

### Comparing `sts_lib-0.31.1/setup.cfg` & `sts_lib-0.31.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `sts_lib-0.31.1/sts/__init__.py` & `sts_lib-0.31.2/sts/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         @_lazyprop.setter
         def _lazyprop(self, value):
             setattr(self, attr_name, value)
 
         return _lazyprop
 
 
-__version__ = '0.31.1'
+__version__ = '0.31.2'
 
 StsDictMatch = namedtuple('StsDictMatch', ['conv', 'start', 'end'])
 StsDictConv = namedtuple('StsDictConv', ['key', 'values'])
 StsConvExclude = namedtuple('StsConvExclude', ['text'])
 
 
 class StreamList(list):
@@ -632,40 +632,41 @@
             parts: a string or iterable parts to be converted.
             include_short: include non-maximal-match conversions
             include_self: include source for every match
 
         Returns:
             a list of possible conversions.
         """
-        text = parts
+        _parts = parts
         parts = self._split(parts)
 
-        stack = [(parts, 0, 0)]
+        total = len(parts)
+        stack = [([], 0, 0)]
         substack = []
         results = {}
         while stack:
-            (parts, matched, nextindex) = data = stack.pop()
-            if nextindex < len(parts):
-                self._apply_enum_sub(substack, data, include_short=include_short, include_self=include_self)
+            (newparts, nextindex, matched) = data = stack.pop()
+            if nextindex < total:
+                self._apply_enum_sub(parts, substack, data, include_short=include_short, include_self=include_self)
                 while substack:
                     stack.append(substack.pop())
             elif matched > 0:
-                results[''.join(parts)] = True
+                results[''.join(newparts)] = None
 
         results = list(results)
 
         if not results:
-            results.append(text if isinstance(text, str) else ''.join(text))
+            results.append(_parts if isinstance(_parts, str) else ''.join(_parts))
 
         return results
 
-    def _apply_enum_sub(self, stack, data, include_short=False, include_self=False):
+    def _apply_enum_sub(self, parts, stack, data, include_short=False, include_self=False):
         """Helper function of apply_enum
         """
-        (parts, matched, index) = data
+        (newparts, index, matched) = data
         has_atomic_match = False
         i = math.inf
         while i > index:
             match = self.match(parts, index, i)
 
             if match is None:
                 break
@@ -676,35 +677,52 @@
             values = match.conv.values
             if include_self:
                 value = ''.join(match.conv.key)
                 if value not in values:
                     values = itertools.chain(values, (value,))
 
             for value in values:
-                result = parts[:index] + [value] + parts[match.end:]
-                stack.append((result, matched + 1, index + 1))
+                stack.append((newparts + [value], match.end, matched + 1))
 
             if not include_short:
                 return
 
             i = match.end - 1
 
-        # add atomic stepping (length = 1) case if none
-        #
-        # e.g.
-        # table: 采信 => 採信, 信息 => 訊息
-        # text: ["采", "信", "息"]
-        #
-        # We get a match ["采", "信", "息"] but no atomic match available.
-        #                 ^^^^^^^^^^
-        #
-        # Add ["采", "信", "息"] so that "采訊息" is not missed.
-        #             ^
+        """Add an atomic stepping (index + 1) case if not presented.
+
+        Example:
+            table:
+                信息 => 訊息
+            parts:
+                ['采', '信', '息']
+            data:
+                ([], 0, 0)
+
+            We get no match, which implies no atomic match (i.e. '采'). Add
+            data=([], 1, 0) so that the possible conversion ['采', '訊息'] is
+            not missing.
+
+        Example:
+            table:
+                采信 => 採信
+                信息 => 訊息
+            parts:
+                ['采', '信', '息']
+            data:
+                ([], 0, 0)
+
+            We get a match '采信' but no atomic match (i.e. '采'). Add
+            data=([], 1, 0) so that the possible conversion ['采', '訊息'] is
+            not missing.
+        """
         if not has_atomic_match:
-            stack.append((parts, matched, index + 1))
+            # reuse newparts for better performance
+            newparts.append(parts[index])
+            stack.append((newparts, index + 1, matched))
 
 
 class Table(StsDict):
     """A cache-boosted STS dictionary.
 
     This class implements a cache and a head-char checking mechanism to
     improve performance on text conversion than base StsDict.
```

### Comparing `sts_lib-0.31.1/sts/cli.py` & `sts_lib-0.31.2/sts/cli.py`

 * *Files identical despite different names*

### Comparing `sts_lib-0.31.1/sts/data/config/_default.json` & `sts_lib-0.31.2/sts/data/config/_default.json`

 * *Files identical despite different names*

### Comparing `sts_lib-0.31.1/sts/data/config/hk2s.json` & `sts_lib-0.31.2/sts/data/config/hk2s.json`

 * *Files identical despite different names*

### Comparing `sts_lib-0.31.1/sts/data/config/s2twp.json` & `sts_lib-0.31.2/sts/data/config/s2twp.json`

 * *Files identical despite different names*

### Comparing `sts_lib-0.31.1/sts/data/config/tw2s.json` & `sts_lib-0.31.2/sts/data/config/tw2s.json`

 * *Files identical despite different names*

### Comparing `sts_lib-0.31.1/sts/data/config/tw2sp.json` & `sts_lib-0.31.2/sts/data/config/tw2sp.json`

 * *Files identical despite different names*

### Comparing `sts_lib-0.31.1/sts/data/dictionary/HKVariants.txt` & `sts_lib-0.31.2/sts/data/dictionary/HKVariants.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.31.1/sts/data/dictionary/HKVariantsRevPhrases.txt` & `sts_lib-0.31.2/sts/data/dictionary/HKVariantsRevPhrases.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.31.1/sts/data/dictionary/JPShinjitaiPhrases.txt` & `sts_lib-0.31.2/sts/data/dictionary/JPShinjitaiPhrases.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.31.1/sts/data/dictionary/JPVariants.txt` & `sts_lib-0.31.2/sts/data/dictionary/JPVariants.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.31.1/sts/data/dictionary/STCharacters.txt` & `sts_lib-0.31.2/sts/data/dictionary/STCharacters.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.31.1/sts/data/dictionary/STPhrases.txt` & `sts_lib-0.31.2/sts/data/dictionary/STPhrases.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.31.1/sts/data/dictionary/TSCharacters.txt` & `sts_lib-0.31.2/sts/data/dictionary/TSCharacters.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.31.1/sts/data/dictionary/TSPhrases.txt` & `sts_lib-0.31.2/sts/data/dictionary/TSPhrases.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.31.1/sts/data/dictionary/TWPhrasesIT.txt` & `sts_lib-0.31.2/sts/data/dictionary/TWPhrasesIT.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.31.1/sts/data/dictionary/TWPhrasesName.txt` & `sts_lib-0.31.2/sts/data/dictionary/TWPhrasesName.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.31.1/sts/data/dictionary/TWPhrasesOther.txt` & `sts_lib-0.31.2/sts/data/dictionary/TWPhrasesOther.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.31.1/sts/data/dictionary/TWVariantsRevPhrases.txt` & `sts_lib-0.31.2/sts/data/dictionary/TWVariantsRevPhrases.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.31.1/sts/data/htmlpage.tpl.html` & `sts_lib-0.31.2/sts/data/htmlpage.tpl.html`

 * *Files identical despite different names*

### Comparing `sts_lib-0.31.1/sts/data/scheme/st_multi.txt` & `sts_lib-0.31.2/sts/data/scheme/st_multi.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.31.1/sts/data/scheme/variant.txt` & `sts_lib-0.31.2/sts/data/scheme/variant.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.31.1/sts_lib.egg-info/PKG-INFO` & `sts_lib-0.31.2/sts_lib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sts-lib
-Version: 0.31.1
+Version: 0.31.2
 Summary: An open library for flexible simplified-traditional Chinese text conversion.
 Home-page: https://github.com/danny0838/sts-lib
 Author: Danny Lin
 Author-email: danny0838@gmail.com
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: OS Independent
```

### Comparing `sts_lib-0.31.1/sts_lib.egg-info/SOURCES.txt` & `sts_lib-0.31.2/sts_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

