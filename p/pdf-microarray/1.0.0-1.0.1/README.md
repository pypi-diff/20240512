# Comparing `tmp/pdf_microarray-1.0.0.tar.gz` & `tmp/pdf_microarray-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdf_microarray-1.0.0.tar", max compression
+gzip compressed data, was "pdf_microarray-1.0.1.tar", max compression
```

## Comparing `pdf_microarray-1.0.0.tar` & `pdf_microarray-1.0.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    35149 2024-04-08 09:37:58.747842 pdf_microarray-1.0.0/LICENSE
--rw-r--r--   0        0        0     1872 2024-05-01 12:25:29.429257 pdf_microarray-1.0.0/README.md
--rw-r--r--   0        0        0        0 2024-04-21 07:11:46.667453 pdf_microarray-1.0.0/pdf_microarray/__init__.py
--rw-r--r--   0        0        0     3181 2024-05-01 12:24:06.432722 pdf_microarray-1.0.0/pdf_microarray/cli.py
--rw-r--r--   0        0        0     4449 2024-05-01 12:22:04.899726 pdf_microarray-1.0.0/pdf_microarray/pdf_extract.py
--rw-r--r--   0        0        0     9426 2024-05-01 12:22:44.961811 pdf_microarray-1.0.0/pdf_microarray/pdf_microarray.py
--rw-r--r--   0        0        0     2306 2024-05-01 12:23:59.470936 pdf_microarray-1.0.0/pdf_microarray/plot_microarray.py
--rw-r--r--   0        0        0     1081 2024-04-22 05:57:19.150258 pdf_microarray-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     3018 1970-01-01 00:00:00.000000 pdf_microarray-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-08 09:37:58.747842 pdf_microarray-1.0.1/LICENSE
+-rw-r--r--   0        0        0     2084 2024-05-12 09:17:13.473049 pdf_microarray-1.0.1/README.md
+-rw-r--r--   0        0        0        0 2024-04-21 07:11:46.667453 pdf_microarray-1.0.1/pdf_microarray/__init__.py
+-rw-r--r--   0        0        0     3726 2024-05-12 09:29:45.071980 pdf_microarray-1.0.1/pdf_microarray/cli.py
+-rw-r--r--   0        0        0     4449 2024-05-01 12:22:04.899726 pdf_microarray-1.0.1/pdf_microarray/pdf_extract.py
+-rw-r--r--   0        0        0     8463 2024-05-12 08:31:28.757560 pdf_microarray-1.0.1/pdf_microarray/pdf_microarray.py
+-rw-r--r--   0        0        0     3985 2024-05-12 09:28:55.064173 pdf_microarray-1.0.1/pdf_microarray/plot_microarray.py
+-rw-r--r--   0        0        0     1081 2024-05-12 09:24:00.380005 pdf_microarray-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     3230 1970-01-01 00:00:00.000000 pdf_microarray-1.0.1/PKG-INFO
```

### Comparing `pdf_microarray-1.0.0/LICENSE` & `pdf_microarray-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pdf_microarray-1.0.0/README.md` & `pdf_microarray-1.0.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 
 and stores the extracted text in a designated output directory.
 
 The processed text can then analyzed using the [Levenshtein distance](https://en.wikipedia.org/wiki/Levenshtein_distance) to detect the occurrences of specified words. A graphical representation of these occurrences is offered in a microarray format.
 
 ## Installation
 
+[Tesseract](https://github.com/tesseract-ocr/tesseract) is required for this CLI tool. Please follow the [installation](https://tesseract-ocr.github.io/tessdoc/Installation.html) instructions for your platform.
+
 ```bash
 pip install pipx
 pipx install pdf-microarray
 ```
 
 ## Usage
```

### Comparing `pdf_microarray-1.0.0/pdf_microarray/pdf_extract.py` & `pdf_microarray-1.0.1/pdf_microarray/pdf_extract.py`

 * *Files identical despite different names*

### Comparing `pdf_microarray-1.0.0/pdf_microarray/pdf_microarray.py` & `pdf_microarray-1.0.1/pdf_microarray/pdf_microarray.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 """
 Provides functionality for extracting and analyzing text from PDF documents,
-by using the Levenshtein distance to search for specific words, visualizing
-the results in a microarray plot format. It offers efficient processing by
-segmenting documents and utilizing multithreading.
+by using the Levenshtein distance to search for specific words. It offers
+efficient processing by segmenting documents and utilizing multithreading.
 """
 
 import os
 import re
 import time
 from collections import defaultdict
 from concurrent.futures import ThreadPoolExecutor
 from typing import NamedTuple
 
 import pandas as pd
 from thefuzz import fuzz
 
 from pdf_microarray.pdf_extract import PDFExtract, PDFInfo
-from pdf_microarray.plot_microarray import PlotMicroarray
 
 
 class Segment(NamedTuple):
     """
     A NamedTuple that stores metadata about a segment of a PDF document.
 
     Attributes:
@@ -39,34 +37,34 @@
 class PDFMicroarray:
     """
     A class responsible for extracting and analyzing text from PDF documents.
     It also supports plotting the results in a microarray format.
     """
 
     @classmethod
-    def process(cls, documents_path, processed_path, skip=False, threads=-1):
+    def process(cls, documents_path, processed_path, threads=-1, force=False):
         """
         Processes PDF documents into text, splitting them into segments to
         improve the extraction performance.
 
         Args:
             documents_path (str): Path to the directory containing PDF files.
             processed_path (str): Directory where processed segments are to be
             stored.
-            skip (bool): Whether to skip already processed documents.
-            Defaults to False.
             threads (int): Number of concurrent threads to use. Defaults to -1,
             which uses all available CPU cores.
+            force (bool): Whether to force the processing of already processed
+            documents. Defaults to False.
         """
 
         documents = cls._get_documents(documents_path)
         threads = os.cpu_count() if threads == -1 else threads
 
         document_segments = cls._compute_segments(
-            documents, processed_path, skip, max_pages=20
+            documents, processed_path, max_pages=20, force=force
         )
 
         print(
             f"Processing {len(documents)} PDFs",
             f"in {len(document_segments)} segments",
             f"using up to {threads} threads",
         )
@@ -82,70 +80,49 @@
 
         print(
             f"Processed {len(documents)} PDFs",
             f"in {round(time.time() - start_time, 1)} seconds",
         )
 
     @classmethod
-    def analyze(cls, processed_path, words_path, data_path, threshold=90):
+    def analyze(cls, processed_path, words_path, data_path):
         """
         Analyzes extracted text using the Levenshtein distance to find the
         occurrence of specific words.
 
         Args:
             processed_path (str): Path where processed segments are stored.
             words_path (str): Path to a file containing words to search for.
             data_path (str): Path where the results dataframe will be saved.
-            threshold (int): Minimum Levenshtein distance score (0-100) to
-            consider a match. Defaults to 90.
         """
 
         text = cls._get_processed_text(processed_path)
         words = cls._get_words(words_path)
 
         df = cls._calculate_scores(text, words)
-        df.map(lambda x: 1 if x >= threshold else 0)
 
         df.to_csv(data_path)
 
     @classmethod
-    def plot(cls, data_path, image_path=None, width=30, height=60):
-        """
-        Generates a plot representing data as a microarray.
-
-        Args:
-            data_path (str): Path to the CSV file containing data to plot.
-            image_path (str): Path where the plot image will be saved.
-            If None, the plot is just displayed. Defaults to None.
-            width (int): Width of the plot. Defaults to 30.
-            height (int): Height of the plot. Defaults to 60.
-        """
-        df = pd.read_csv(data_path, index_col=0, dtype={0: str})
-
-        return PlotMicroarray.plot(
-            df, image_path=image_path, width=width, height=height
-        )
-
-    @classmethod
-    def _compute_segments(cls, documents, processed_path, skip, max_pages):
+    def _compute_segments(cls, documents, processed_path, max_pages, force):
         document_segments = []
 
         for document_path in documents:
             total_pages = PDFInfo.get_page_count(document_path)
             segments = (total_pages + max_pages - 1) // max_pages
 
             for segment in range(segments):
                 first_page = segment * max_pages
                 last_page = min(first_page + max_pages - 1, total_pages - 1)
 
                 doc_proc_path = cls._get_processed_path(
                     document_path, processed_path, first_page, last_page
                 )
 
-                if skip and os.path.exists(doc_proc_path):
+                if os.path.exists(doc_proc_path) and not force:
                     print(
                         f"Skipping {document_path}",
                         f"(pages {first_page + 1}-{last_page + 1})",
                     )
                     continue
 
                 document_segment = Segment(
```

### Comparing `pdf_microarray-1.0.0/pyproject.toml` & `pdf_microarray-1.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "pdf-microarray"
-version = "1.0.0"
+version = "1.0.1"
 description = "A Python CLI tool designed to assist with literature research by visualizing the occurrence of words in PDF documents with a microarray format."
 authors = [
     "Björn Tropf",
     "Jan Tropf"
 ]
 include = ["LICENSE", "README.md"]
 license = "GPL-3.0-or-later"
```

### Comparing `pdf_microarray-1.0.0/PKG-INFO` & `pdf_microarray-1.0.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdf-microarray
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Python CLI tool designed to assist with literature research by visualizing the occurrence of words in PDF documents with a microarray format.
 Home-page: https://github.com/bjorntropf/PDFMicroarray
 License: GPL-3.0-or-later
 Keywords: pdf,microarray
 Author: Björn Tropf
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
@@ -38,14 +38,16 @@
 
 and stores the extracted text in a designated output directory.
 
 The processed text can then analyzed using the [Levenshtein distance](https://en.wikipedia.org/wiki/Levenshtein_distance) to detect the occurrences of specified words. A graphical representation of these occurrences is offered in a microarray format.
 
 ## Installation
 
+[Tesseract](https://github.com/tesseract-ocr/tesseract) is required for this CLI tool. Please follow the [installation](https://tesseract-ocr.github.io/tessdoc/Installation.html) instructions for your platform.
+
 ```bash
 pip install pipx
 pipx install pdf-microarray
 ```
 
 ## Usage
```

