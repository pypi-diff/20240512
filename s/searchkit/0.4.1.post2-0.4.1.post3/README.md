# Comparing `tmp/searchkit-0.4.1.post2.tar.gz` & `tmp/searchkit-0.4.1.post3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "searchkit-0.4.1.post2.tar", last modified: Thu Apr 25 16:34:39 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

