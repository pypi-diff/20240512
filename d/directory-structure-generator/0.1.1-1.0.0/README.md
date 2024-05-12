# Comparing `tmp/directory_structure_generator-0.1.1.tar.gz` & `tmp/directory_structure_generator-1.0.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "directory_structure_generator-0.1.1.tar", last modified: Sun May 12 10:19:56 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

