# Comparing `tmp/bioat-0.9.0.tar.gz` & `tmp/bioat-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bioat-0.9.0.tar", max compression
+gzip compressed data, was "bioat-0.9.1.tar", max compression
```

## Comparing `bioat-0.9.0.tar` & `bioat-0.9.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0     1080 2023-11-22 08:24:09.310091 bioat-0.9.0/LICENSE
--rw-r--r--   0        0        0     1088 2023-11-22 12:01:38.876152 bioat-0.9.0/README.md
--rw-r--r--   0        0        0     1124 2024-02-22 08:55:30.712949 bioat-0.9.0/pyproject.toml
--rw-r--r--   0        0        0      704 2023-11-28 14:06:07.931403 bioat-0.9.0/src/bioat/__init__.py
--rw-r--r--   0        0        0      418 2023-11-22 08:24:09.760447 bioat-0.9.0/src/bioat/__main__.py
--rw-r--r--   0        0        0      897 2023-11-22 08:24:09.760509 bioat-0.9.0/src/bioat/about.py
--rw-r--r--   0        0        0    13678 2023-11-22 08:24:09.760698 bioat-0.9.0/src/bioat/bamtools.py
--rw-r--r--   0        0        0      669 2023-11-22 08:24:09.760764 bioat-0.9.0/src/bioat/bedtools.py
--rw-r--r--   0        0        0     2045 2023-11-22 08:24:09.760841 bioat-0.9.0/src/bioat/cli.py
--rw-r--r--   0        0        0     2915 2024-02-22 07:33:55.491031 bioat-0.9.0/src/bioat/crisprtools.py
--rw-r--r--   0        0        0    14504 2023-11-22 08:24:09.761075 bioat-0.9.0/src/bioat/detect_seq.py
--rw-r--r--   0        0        0      794 2023-11-22 08:24:09.761134 bioat-0.9.0/src/bioat/exceptions.py
--rw-r--r--   0        0        0     8643 2024-01-04 14:23:13.643512 bioat-0.9.0/src/bioat/fastxtools.py
--rw-r--r--   0        0        0      818 2023-11-22 08:24:09.761290 bioat-0.9.0/src/bioat/genome.py
--rw-r--r--   0        0        0     5806 2023-11-22 08:24:09.761378 bioat-0.9.0/src/bioat/hictools.py
--rw-r--r--   0        0        0        0 2023-11-22 08:24:09.761430 bioat-0.9.0/src/bioat/lib/__init__.py
--rw-r--r--   0        0        0     1061 2023-11-22 08:24:09.761513 bioat-0.9.0/src/bioat/lib/_dev_tools.py
--rw-r--r--   0        0        0     9873 2023-11-22 08:24:09.761762 bioat-0.9.0/src/bioat/lib/circos/example_data_barplot.csv
--rw-r--r--   0        0        0    30782 2023-11-22 08:24:09.761893 bioat-0.9.0/src/bioat/lib/circos/example_data_chromosome_cytoband.csv
--rw-r--r--   0        0        0      427 2023-11-22 08:24:09.761966 bioat-0.9.0/src/bioat/lib/circos/example_data_chromosome_general.csv
--rw-r--r--   0        0        0     5143 2023-11-22 08:24:09.762053 bioat-0.9.0/src/bioat/lib/circos/example_data_links.csv
--rw-r--r--   0        0        0     9856 2023-11-22 08:24:09.762263 bioat-0.9.0/src/bioat/lib/circos/example_data_point.csv
--rw-r--r--   0        0        0     9107 2023-11-22 08:24:09.762471 bioat-0.9.0/src/bioat/lib/circos/example_data_rect_gradual.csv
--rw-r--r--   0        0        0      478 2023-11-22 08:24:09.762533 bioat-0.9.0/src/bioat/lib/circos/hg38_chromosome_length.csv
--rw-r--r--   0        0        0    31651 2023-11-22 08:24:09.762657 bioat-0.9.0/src/bioat/lib/circos/hg38_cytoBand.csv
--rw-r--r--   0        0        0      424 2023-11-22 08:24:09.762724 bioat-0.9.0/src/bioat/lib/circos/mm10_chromosome_length.csv
--rw-r--r--   0        0        0    13849 2023-11-22 08:24:09.762900 bioat-0.9.0/src/bioat/lib/circos/mm10_cytoBand.csv
--rw-r--r--   0        0        0     6304 2023-11-22 08:24:09.762990 bioat-0.9.0/src/bioat/lib/libalignment.py
--rw-r--r--   0        0        0    77524 2023-11-22 08:24:09.763212 bioat-0.9.0/src/bioat/lib/libcircos.py
--rw-r--r--   0        0        0     4503 2023-11-22 08:24:09.763361 bioat-0.9.0/src/bioat/lib/libcolor.py
--rw-r--r--   0        0        0     6587 2023-12-07 13:20:21.574618 bioat-0.9.0/src/bioat/lib/libcrispr.py
--rw-r--r--   0        0        0     4160 2023-12-07 07:53:35.925816 bioat-0.9.0/src/bioat/lib/libdataclasses.py
--rw-r--r--   0        0        0   155137 2023-11-22 08:24:09.763897 bioat-0.9.0/src/bioat/lib/libdetect_seq.py
--rw-r--r--   0        0        0    25226 2024-02-22 08:54:50.004689 bioat-0.9.0/src/bioat/lib/libfastx.py
--rw-r--r--   0        0        0    69739 2024-02-12 09:46:28.927366 bioat-0.9.0/src/bioat/lib/libjgi.py
--rw-r--r--   0        0        0     1030 2024-02-12 09:47:10.968695 bioat-0.9.0/src/bioat/lib/libpandas.py
--rw-r--r--   0        0        0      282 2023-12-27 02:57:02.595803 bioat-0.9.0/src/bioat/lib/libpath.py
--rw-r--r--   0        0        0     1720 2023-11-22 08:24:09.764393 bioat-0.9.0/src/bioat/lib/libplot.py
--rw-r--r--   0        0        0      509 2023-11-22 08:24:09.764466 bioat-0.9.0/src/bioat/lib/libsnakemake.py
--rw-r--r--   0        0        0     3172 2023-12-05 13:19:29.496301 bioat-0.9.0/src/bioat/lib/libspider.py
--rw-r--r--   0        0        0     1458 2024-02-12 09:49:53.352098 bioat-0.9.0/src/bioat/logger.py
--rw-r--r--   0        0        0     3856 2024-02-05 03:21:12.426836 bioat-0.9.0/src/bioat/metatools.py
--rw-r--r--   0        0        0    10983 2023-11-22 08:24:09.765009 bioat-0.9.0/src/bioat/searchtools.py
--rw-r--r--   0        0        0     5709 2023-11-22 08:24:09.765096 bioat-0.9.0/src/bioat/systemtools.py
--rw-r--r--   0        0        0     4129 2023-11-22 08:24:09.765186 bioat-0.9.0/src/bioat/tabletools.py
--rw-r--r--   0        0        0    81452 2023-11-22 08:24:09.765445 bioat-0.9.0/src/bioat/target_seq.py
--rw-r--r--   0        0        0      560 2024-02-22 08:55:07.687752 bioat-0.9.0/src/bioat/version.py
--rw-r--r--   0        0        0     2378 1970-01-01 00:00:00.000000 bioat-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1080 2023-11-22 08:24:09.310091 bioat-0.9.1/LICENSE
+-rw-r--r--   0        0        0     1088 2023-11-22 12:01:38.876152 bioat-0.9.1/README.md
+-rw-r--r--   0        0        0     1124 2024-02-22 10:04:49.941355 bioat-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0      704 2023-11-28 14:06:07.931403 bioat-0.9.1/src/bioat/__init__.py
+-rw-r--r--   0        0        0      418 2023-11-22 08:24:09.760447 bioat-0.9.1/src/bioat/__main__.py
+-rw-r--r--   0        0        0      897 2023-11-22 08:24:09.760509 bioat-0.9.1/src/bioat/about.py
+-rw-r--r--   0        0        0    13678 2023-11-22 08:24:09.760698 bioat-0.9.1/src/bioat/bamtools.py
+-rw-r--r--   0        0        0      669 2023-11-22 08:24:09.760764 bioat-0.9.1/src/bioat/bedtools.py
+-rw-r--r--   0        0        0     2045 2023-11-22 08:24:09.760841 bioat-0.9.1/src/bioat/cli.py
+-rw-r--r--   0        0        0     2915 2024-02-22 07:33:55.491031 bioat-0.9.1/src/bioat/crisprtools.py
+-rw-r--r--   0        0        0    14504 2023-11-22 08:24:09.761075 bioat-0.9.1/src/bioat/detect_seq.py
+-rw-r--r--   0        0        0      794 2023-11-22 08:24:09.761134 bioat-0.9.1/src/bioat/exceptions.py
+-rw-r--r--   0        0        0     8643 2024-01-04 14:23:13.643512 bioat-0.9.1/src/bioat/fastxtools.py
+-rw-r--r--   0        0        0      818 2023-11-22 08:24:09.761290 bioat-0.9.1/src/bioat/genome.py
+-rw-r--r--   0        0        0     5806 2023-11-22 08:24:09.761378 bioat-0.9.1/src/bioat/hictools.py
+-rw-r--r--   0        0        0        0 2023-11-22 08:24:09.761430 bioat-0.9.1/src/bioat/lib/__init__.py
+-rw-r--r--   0        0        0     1061 2023-11-22 08:24:09.761513 bioat-0.9.1/src/bioat/lib/_dev_tools.py
+-rw-r--r--   0        0        0     9873 2023-11-22 08:24:09.761762 bioat-0.9.1/src/bioat/lib/circos/example_data_barplot.csv
+-rw-r--r--   0        0        0    30782 2023-11-22 08:24:09.761893 bioat-0.9.1/src/bioat/lib/circos/example_data_chromosome_cytoband.csv
+-rw-r--r--   0        0        0      427 2023-11-22 08:24:09.761966 bioat-0.9.1/src/bioat/lib/circos/example_data_chromosome_general.csv
+-rw-r--r--   0        0        0     5143 2023-11-22 08:24:09.762053 bioat-0.9.1/src/bioat/lib/circos/example_data_links.csv
+-rw-r--r--   0        0        0     9856 2023-11-22 08:24:09.762263 bioat-0.9.1/src/bioat/lib/circos/example_data_point.csv
+-rw-r--r--   0        0        0     9107 2023-11-22 08:24:09.762471 bioat-0.9.1/src/bioat/lib/circos/example_data_rect_gradual.csv
+-rw-r--r--   0        0        0      478 2023-11-22 08:24:09.762533 bioat-0.9.1/src/bioat/lib/circos/hg38_chromosome_length.csv
+-rw-r--r--   0        0        0    31651 2023-11-22 08:24:09.762657 bioat-0.9.1/src/bioat/lib/circos/hg38_cytoBand.csv
+-rw-r--r--   0        0        0      424 2023-11-22 08:24:09.762724 bioat-0.9.1/src/bioat/lib/circos/mm10_chromosome_length.csv
+-rw-r--r--   0        0        0    13849 2023-11-22 08:24:09.762900 bioat-0.9.1/src/bioat/lib/circos/mm10_cytoBand.csv
+-rw-r--r--   0        0        0     6304 2023-11-22 08:24:09.762990 bioat-0.9.1/src/bioat/lib/libalignment.py
+-rw-r--r--   0        0        0    77524 2023-11-22 08:24:09.763212 bioat-0.9.1/src/bioat/lib/libcircos.py
+-rw-r--r--   0        0        0     4503 2023-11-22 08:24:09.763361 bioat-0.9.1/src/bioat/lib/libcolor.py
+-rw-r--r--   0        0        0     6587 2023-12-07 13:20:21.574618 bioat-0.9.1/src/bioat/lib/libcrispr.py
+-rw-r--r--   0        0        0     4160 2023-12-07 07:53:35.925816 bioat-0.9.1/src/bioat/lib/libdataclasses.py
+-rw-r--r--   0        0        0   155137 2023-11-22 08:24:09.763897 bioat-0.9.1/src/bioat/lib/libdetect_seq.py
+-rw-r--r--   0        0        0    26124 2024-02-22 10:03:59.555985 bioat-0.9.1/src/bioat/lib/libfastx.py
+-rw-r--r--   0        0        0    69739 2024-02-12 09:46:28.927366 bioat-0.9.1/src/bioat/lib/libjgi.py
+-rw-r--r--   0        0        0     1030 2024-02-12 09:47:10.968695 bioat-0.9.1/src/bioat/lib/libpandas.py
+-rw-r--r--   0        0        0      282 2023-12-27 02:57:02.595803 bioat-0.9.1/src/bioat/lib/libpath.py
+-rw-r--r--   0        0        0     1720 2023-11-22 08:24:09.764393 bioat-0.9.1/src/bioat/lib/libplot.py
+-rw-r--r--   0        0        0      509 2023-11-22 08:24:09.764466 bioat-0.9.1/src/bioat/lib/libsnakemake.py
+-rw-r--r--   0        0        0     3172 2023-12-05 13:19:29.496301 bioat-0.9.1/src/bioat/lib/libspider.py
+-rw-r--r--   0        0        0     1458 2024-02-12 09:49:53.352098 bioat-0.9.1/src/bioat/logger.py
+-rw-r--r--   0        0        0     3856 2024-02-05 03:21:12.426836 bioat-0.9.1/src/bioat/metatools.py
+-rw-r--r--   0        0        0    10983 2023-11-22 08:24:09.765009 bioat-0.9.1/src/bioat/searchtools.py
+-rw-r--r--   0        0        0     5709 2023-11-22 08:24:09.765096 bioat-0.9.1/src/bioat/systemtools.py
+-rw-r--r--   0        0        0     4129 2023-11-22 08:24:09.765186 bioat-0.9.1/src/bioat/tabletools.py
+-rw-r--r--   0        0        0    81452 2023-11-22 08:24:09.765445 bioat-0.9.1/src/bioat/target_seq.py
+-rw-r--r--   0        0        0      560 2024-02-22 10:04:34.652141 bioat-0.9.1/src/bioat/version.py
+-rw-r--r--   0        0        0     2378 1970-01-01 00:00:00.000000 bioat-0.9.1/PKG-INFO
```

### Comparing `bioat-0.9.0/LICENSE` & `bioat-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bioat-0.9.0/README.md` & `bioat-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `bioat-0.9.0/pyproject.toml` & `bioat-0.9.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bioat"
-version = "0.9.0"
+version = "0.9.1"
 description = "Bioinformatic toolkit with python (It's still under development!)"
 license = "MIT"
 authors = ["Herman Zhao <hermanzhaozzzz@gmail.com>"]
 repository = "https://github.com/hermanzhaozzzz/bioat"
 homepage = "https://github.com/hermanzhaozzzz/bioat"
 # README file(s) are used as the package description
 readme = "README.md"
```

### Comparing `bioat-0.9.0/src/bioat/__init__.py` & `bioat-0.9.1/src/bioat/__init__.py`

 * *Files identical despite different names*

### Comparing `bioat-0.9.0/src/bioat/about.py` & `bioat-0.9.1/src/bioat/about.py`

 * *Files identical despite different names*

### Comparing `bioat-0.9.0/src/bioat/bamtools.py` & `bioat-0.9.1/src/bioat/bamtools.py`

 * *Files identical despite different names*

### Comparing `bioat-0.9.0/src/bioat/bedtools.py` & `bioat-0.9.1/src/bioat/bedtools.py`

 * *Files identical despite different names*

### Comparing `bioat-0.9.0/src/bioat/cli.py` & `bioat-0.9.1/src/bioat/cli.py`

 * *Files identical despite different names*

### Comparing `bioat-0.9.0/src/bioat/crisprtools.py` & `bioat-0.9.1/src/bioat/crisprtools.py`

 * *Files identical despite different names*

### Comparing `bioat-0.9.0/src/bioat/detect_seq.py` & `bioat-0.9.1/src/bioat/detect_seq.py`

 * *Files identical despite different names*

### Comparing `bioat-0.9.0/src/bioat/exceptions.py` & `bioat-0.9.1/src/bioat/exceptions.py`

 * *Files identical despite different names*

### Comparing `bioat-0.9.0/src/bioat/fastxtools.py` & `bioat-0.9.1/src/bioat/fastxtools.py`

 * *Files identical despite different names*

### Comparing `bioat-0.9.0/src/bioat/genome.py` & `bioat-0.9.1/src/bioat/genome.py`

 * *Files identical despite different names*

### Comparing `bioat-0.9.0/src/bioat/hictools.py` & `bioat-0.9.1/src/bioat/hictools.py`

 * *Files identical despite different names*

### Comparing `bioat-0.9.0/src/bioat/lib/_dev_tools.py` & `bioat-0.9.1/src/bioat/lib/_dev_tools.py`

 * *Files identical despite different names*

### Comparing `bioat-0.9.0/src/bioat/lib/circos/example_data_barplot.csv` & `bioat-0.9.1/src/bioat/lib/circos/example_data_barplot.csv`

 * *Files identical despite different names*

### Comparing `bioat-0.9.0/src/bioat/lib/circos/example_data_chromosome_cytoband.csv` & `bioat-0.9.1/src/bioat/lib/circos/example_data_chromosome_cytoband.csv`

 * *Files identical despite different names*

### Comparing `bioat-0.9.0/src/bioat/lib/circos/example_data_links.csv` & `bioat-0.9.1/src/bioat/lib/circos/example_data_links.csv`

 * *Files identical despite different names*

### Comparing `bioat-0.9.0/src/bioat/lib/circos/example_data_point.csv` & `bioat-0.9.1/src/bioat/lib/circos/example_data_point.csv`

 * *Files identical despite different names*

### Comparing `bioat-0.9.0/src/bioat/lib/circos/example_data_rect_gradual.csv` & `bioat-0.9.1/src/bioat/lib/circos/example_data_rect_gradual.csv`

 * *Files identical despite different names*

### Comparing `bioat-0.9.0/src/bioat/lib/circos/hg38_cytoBand.csv` & `bioat-0.9.1/src/bioat/lib/circos/hg38_cytoBand.csv`

 * *Files identical despite different names*

### Comparing `bioat-0.9.0/src/bioat/lib/circos/mm10_cytoBand.csv` & `bioat-0.9.1/src/bioat/lib/circos/mm10_cytoBand.csv`

 * *Files identical despite different names*

### Comparing `bioat-0.9.0/src/bioat/lib/libalignment.py` & `bioat-0.9.1/src/bioat/lib/libalignment.py`

 * *Files identical despite different names*

### Comparing `bioat-0.9.0/src/bioat/lib/libcircos.py` & `bioat-0.9.1/src/bioat/lib/libcircos.py`

 * *Files identical despite different names*

### Comparing `bioat-0.9.0/src/bioat/lib/libcolor.py` & `bioat-0.9.1/src/bioat/lib/libcolor.py`

 * *Files identical despite different names*

### Comparing `bioat-0.9.0/src/bioat/lib/libcrispr.py` & `bioat-0.9.1/src/bioat/lib/libcrispr.py`

 * *Files identical despite different names*

### Comparing `bioat-0.9.0/src/bioat/lib/libdataclasses.py` & `bioat-0.9.1/src/bioat/lib/libdataclasses.py`

 * *Files identical despite different names*

### Comparing `bioat-0.9.0/src/bioat/lib/libdetect_seq.py` & `bioat-0.9.1/src/bioat/lib/libdetect_seq.py`

 * *Files identical despite different names*

### Comparing `bioat-0.9.0/src/bioat/lib/libfastx.py` & `bioat-0.9.1/src/bioat/lib/libfastx.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,16 +71,16 @@
     bed_pep = os.path.join(temp_dir, f"{input_fa}.pep.loc.bed")
     bed_crispr = os.path.join(temp_dir, f"{input_fa}.crispr.loc.bed")
     bed_cas = os.path.join(temp_dir, f"{input_fa}.cas.loc.bed")
     # info
     assembly_id = f"{os.path.basename(fa_input)}"
 
     tests = {
-        0: False,  # PASS # 0. filter contigs
-        1: False,  # PASS # 1. cas & protein annotation
+        0: True,  # PASS # 0. filter contigs
+        1: True,  # PASS # 1. cas & protein annotation
         2: True,  # PASS # 2. get crispr loci
         3: True,  # PASS # 3. get protein cds
         4: True,  # PASS # 4. cas loci vs protein cds
         5: True,  # PASS # 5. get cas faa
         6: True,  # PASS # 6. get crispr loci as scaffold
     }
     # -----------------------------
@@ -106,14 +106,17 @@
         logger.debug(f"checking if @ {fa_filtered} is empty.")
 
         if os.path.getsize(fa_filtered) == 0:
             # don't consider gz file. because it is a temp file.
             logger.warning(f"fa_filtered @ {fa_filtered} is empty! will touch an empty output file @ {fa_pep_cas}")
             with open(fa_pep_cas, 'wt') as f:
                 f.write('')
+            if output_crispr_info_tab:
+                with open(output_crispr_info_tab, 'wt') as f:
+                    f.write('')
             logger.info("End, exit.")
             return  # just return output file as an empty file
     # -----------------------------
     # 1. cas & protein annotation
     # -----------------------------
     if tests[1]:
         logger.info("1.cas & protein annotation")
@@ -144,14 +147,16 @@
         # ...
         logger.debug("subprocess call for pilercr")
         subprocess.check_call(  # don't export help doc for output crispr info
             [pilercr, "-noinfo", "-in", fa_filtered, "-out", f_pilercr],
             stderr=open("/dev/null", "wt") if log_level != "DEBUG" else sys.stderr,
         )
         logger.debug(f"call has returned, check output @ {f_pilercr}")
+        # if fa_filtered is empty, just return empty fa_pep_cas
+        logger.debug(f"checking if @ {fa_filtered} is empty.")
     # -----------------------------
     # 2.get crispr loci
     # -----------------------------
     if tests[2]:
         logger.info("2.get crispr loci")
         with open(f_pilercr, "rt") as wrapper_i, open(bed_crispr, "wt") as wrapper_o:
             lines = wrapper_i.readlines()
@@ -298,14 +303,26 @@
                         ls_rep_info.append([repeat_seq_rep, repeat_length_rep, spacer_length_rep])
                         continue
                     ls_temp.append([f'{assembly_id}+{contig_id}+{array_id}', info])
                 ls_all.append(ls_temp)
 
                 ls_df = []
 
+                if not ls_all or ls_all == [None]:
+                    # don't consider gz file. because it is a temp file.
+                    logger.warning(
+                        f'find no crispr info in @ {fa_filtered}! will touch an empty output file @ {fa_pep_cas}')
+                    with open(fa_pep_cas, 'wt') as f:
+                        f.write('')
+                    if output_crispr_info_tab:
+                        with open(output_crispr_info_tab, 'wt') as f:
+                            f.write('')
+                    logger.info("End, exit.")
+                    return  # just return output file as an empty file
+
                 for idx, one in enumerate(ls_all):
                     ls_one_info = [i[:1] + ls_rep_info[idx] + i[1].split() for i in one]
                     if len(ls_one_info[0]) == len(ls_one_info[-1]):
                         pass
                     else:
                         ls_one_info[-1].insert(7, np.NaN)
                     df = pd.DataFrame(ls_one_info, columns=[
```

### Comparing `bioat-0.9.0/src/bioat/lib/libjgi.py` & `bioat-0.9.1/src/bioat/lib/libjgi.py`

 * *Files identical despite different names*

### Comparing `bioat-0.9.0/src/bioat/lib/libpandas.py` & `bioat-0.9.1/src/bioat/lib/libpandas.py`

 * *Files identical despite different names*

### Comparing `bioat-0.9.0/src/bioat/lib/libplot.py` & `bioat-0.9.1/src/bioat/lib/libplot.py`

 * *Files identical despite different names*

### Comparing `bioat-0.9.0/src/bioat/lib/libspider.py` & `bioat-0.9.1/src/bioat/lib/libspider.py`

 * *Files identical despite different names*

### Comparing `bioat-0.9.0/src/bioat/logger.py` & `bioat-0.9.1/src/bioat/logger.py`

 * *Files identical despite different names*

### Comparing `bioat-0.9.0/src/bioat/metatools.py` & `bioat-0.9.1/src/bioat/metatools.py`

 * *Files identical despite different names*

### Comparing `bioat-0.9.0/src/bioat/searchtools.py` & `bioat-0.9.1/src/bioat/searchtools.py`

 * *Files identical despite different names*

### Comparing `bioat-0.9.0/src/bioat/systemtools.py` & `bioat-0.9.1/src/bioat/systemtools.py`

 * *Files identical despite different names*

### Comparing `bioat-0.9.0/src/bioat/tabletools.py` & `bioat-0.9.1/src/bioat/tabletools.py`

 * *Files identical despite different names*

### Comparing `bioat-0.9.0/src/bioat/target_seq.py` & `bioat-0.9.1/src/bioat/target_seq.py`

 * *Files identical despite different names*

### Comparing `bioat-0.9.0/src/bioat/version.py` & `bioat-0.9.1/src/bioat/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import datetime
 import os
 
 project_toml: str = os.path.join(bioat.__path__[0], "version.py")
 sec = os.path.getmtime(project_toml)
 __upgrade_date__ = datetime.date.fromtimestamp(sec)
-__version__ = "0.9.0"
+__version__ = "0.9.1"
 
 __author__ = "Huanan Herman ZHAO @ Tsinghua University"
 __email__ = "hermanzhaozzzz AT gmail.com"
 __doc_format__ = "restructuredtext"
 __doc_address__ = "https://github.com/hermanzhaozzzz/bioat/tree/master/docs"
 __issue_address__ = "https://github.com/hermanzhaozzzz/bioat/issues"
 __repo_address__ = "https://github.com/hermanzhaozzzz/bioat"
```

### Comparing `bioat-0.9.0/PKG-INFO` & `bioat-0.9.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bioat
-Version: 0.9.0
+Version: 0.9.1
 Summary: Bioinformatic toolkit with python (It's still under development!)
 Home-page: https://github.com/hermanzhaozzzz/bioat
 License: MIT
 Author: Herman Zhao
 Author-email: hermanzhaozzzz@gmail.com
 Requires-Python: >=3.10.0
 Classifier: License :: OSI Approved :: MIT License
```

