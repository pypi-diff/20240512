# Comparing `tmp/kimimaro-3.6.0.tar.gz` & `tmp/kimimaro-3.7.0-cp38-cp38-macosx_10_9_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kimimaro-3.6.0.tar", last modified: Thu May  2 18:00:57 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

