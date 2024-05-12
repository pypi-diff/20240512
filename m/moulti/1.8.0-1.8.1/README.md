# Comparing `tmp/moulti-1.8.0.tar.gz` & `tmp/moulti-1.8.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moulti-1.8.0.tar", last modified: Sun May  5 16:13:18 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

