# Comparing `tmp/bw_processing-0.9.2.tar.gz` & `tmp/bw_processing-0.9.3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bw_processing-0.9.2.tar", last modified: Sat May 11 22:57:16 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

