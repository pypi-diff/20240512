# Comparing `tmp/pyfmtools-5.1.tar.gz` & `tmp/pyfmtools-5.2-cp312-cp312-macosx_14_0_arm64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfmtools-5.1.tar", last modified: Thu May  9 01:15:28 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

