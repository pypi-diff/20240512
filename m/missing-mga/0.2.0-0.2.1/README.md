# Comparing `tmp/missing_mga-0.2.0.tar.gz` & `tmp/missing_mga-0.2.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "missing_mga-0.2.0.tar", last modified: Sun May 12 13:29:36 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

