# Comparing `tmp/anycrc-0.6.1.tar.gz` & `tmp/anycrc-0.6.2-cp310-cp310-musllinux_1_1_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anycrc-0.6.1.tar", last modified: Wed May  8 12:25:32 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

