# Comparing `tmp/zebrafy-1.1.0.tar.gz` & `tmp/zebrafy-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zebrafy-1.1.0.tar", last modified: Sun Mar 24 00:42:57 2024, max compression
+gzip compressed data, was "zebrafy-1.1.1.tar", last modified: Sun May 12 01:59:26 2024, max compression
```

## Comparing `zebrafy-1.1.0.tar` & `zebrafy-1.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 m         (1000) m         (1000)        0 2024-03-24 00:42:57.789950 zebrafy-1.1.0/
--rw-r--r--   0 m         (1000) m         (1000)     7652 2023-08-06 02:30:03.000000 zebrafy-1.1.0/LICENSE.txt
--rw-r--r--   0 m         (1000) m         (1000)    10399 2024-03-24 00:42:57.789950 zebrafy-1.1.0/PKG-INFO
--rw-r--r--   0 m         (1000) m         (1000)     8906 2024-03-24 00:36:13.000000 zebrafy-1.1.0/README.rst
--rw-r--r--   0 m         (1000) m         (1000)     1780 2024-03-24 00:36:09.000000 zebrafy-1.1.0/pyproject.toml
--rw-r--r--   0 m         (1000) m         (1000)       38 2024-03-24 00:42:57.789950 zebrafy-1.1.0/setup.cfg
-drwxr-xr-x   0 m         (1000) m         (1000)        0 2024-03-24 00:42:57.785951 zebrafy-1.1.0/tests/
--rw-r--r--   0 m         (1000) m         (1000)    21335 2024-03-24 00:36:09.000000 zebrafy-1.1.0/tests/test_zebrafy.py
-drwxr-xr-x   0 m         (1000) m         (1000)        0 2024-03-24 00:42:57.789950 zebrafy-1.1.0/zebrafy/
--rw-r--r--   0 m         (1000) m         (1000)      196 2024-03-24 00:36:09.000000 zebrafy-1.1.0/zebrafy/__init__.py
--rw-r--r--   0 m         (1000) m         (1000)     3401 2023-10-28 06:18:28.000000 zebrafy-1.1.0/zebrafy/crc.py
--rw-r--r--   0 m         (1000) m         (1000)     6644 2024-03-24 00:36:09.000000 zebrafy-1.1.0/zebrafy/graphic_field.py
--rw-r--r--   0 m         (1000) m         (1000)    11276 2024-03-24 00:36:09.000000 zebrafy-1.1.0/zebrafy/zebrafy_image.py
--rw-r--r--   0 m         (1000) m         (1000)    10362 2024-03-24 00:36:09.000000 zebrafy-1.1.0/zebrafy/zebrafy_pdf.py
--rw-r--r--   0 m         (1000) m         (1000)     5654 2024-03-24 00:36:09.000000 zebrafy-1.1.0/zebrafy/zebrafy_zpl.py
-drwxr-xr-x   0 m         (1000) m         (1000)        0 2024-03-24 00:42:57.789950 zebrafy-1.1.0/zebrafy.egg-info/
--rw-r--r--   0 m         (1000) m         (1000)    10399 2024-03-24 00:42:57.000000 zebrafy-1.1.0/zebrafy.egg-info/PKG-INFO
--rw-r--r--   0 m         (1000) m         (1000)      344 2024-03-24 00:42:57.000000 zebrafy-1.1.0/zebrafy.egg-info/SOURCES.txt
--rw-r--r--   0 m         (1000) m         (1000)        1 2024-03-24 00:42:57.000000 zebrafy-1.1.0/zebrafy.egg-info/dependency_links.txt
--rw-r--r--   0 m         (1000) m         (1000)      107 2024-03-24 00:42:57.000000 zebrafy-1.1.0/zebrafy.egg-info/requires.txt
--rw-r--r--   0 m         (1000) m         (1000)        8 2024-03-24 00:42:57.000000 zebrafy-1.1.0/zebrafy.egg-info/top_level.txt
+drwxr-xr-x   0 m         (1000) m         (1000)        0 2024-05-12 01:59:26.310485 zebrafy-1.1.1/
+-rw-r--r--   0 m         (1000) m         (1000)     7652 2023-08-06 02:30:03.000000 zebrafy-1.1.1/LICENSE.txt
+-rw-r--r--   0 m         (1000) m         (1000)    11154 2024-05-12 01:59:26.310485 zebrafy-1.1.1/PKG-INFO
+-rw-r--r--   0 m         (1000) m         (1000)     9661 2024-05-12 01:57:46.000000 zebrafy-1.1.1/README.rst
+-rw-r--r--   0 m         (1000) m         (1000)     1780 2024-05-12 01:57:16.000000 zebrafy-1.1.1/pyproject.toml
+-rw-r--r--   0 m         (1000) m         (1000)       38 2024-05-12 01:59:26.310485 zebrafy-1.1.1/setup.cfg
+drwxr-xr-x   0 m         (1000) m         (1000)        0 2024-05-12 01:59:26.310485 zebrafy-1.1.1/tests/
+-rw-r--r--   0 m         (1000) m         (1000)    21962 2024-05-12 01:58:41.000000 zebrafy-1.1.1/tests/test_zebrafy.py
+drwxr-xr-x   0 m         (1000) m         (1000)        0 2024-05-12 01:59:26.310485 zebrafy-1.1.1/zebrafy/
+-rw-r--r--   0 m         (1000) m         (1000)      196 2024-05-12 01:58:20.000000 zebrafy-1.1.1/zebrafy/__init__.py
+-rw-r--r--   0 m         (1000) m         (1000)     3401 2023-10-28 06:18:28.000000 zebrafy-1.1.1/zebrafy/crc.py
+-rw-r--r--   0 m         (1000) m         (1000)     6644 2024-03-24 00:36:09.000000 zebrafy-1.1.1/zebrafy/graphic_field.py
+-rw-r--r--   0 m         (1000) m         (1000)    11276 2024-03-24 00:36:09.000000 zebrafy-1.1.1/zebrafy/zebrafy_image.py
+-rw-r--r--   0 m         (1000) m         (1000)    11394 2024-05-12 01:56:42.000000 zebrafy-1.1.1/zebrafy/zebrafy_pdf.py
+-rw-r--r--   0 m         (1000) m         (1000)     5654 2024-03-24 00:36:09.000000 zebrafy-1.1.1/zebrafy/zebrafy_zpl.py
+drwxr-xr-x   0 m         (1000) m         (1000)        0 2024-05-12 01:59:26.310485 zebrafy-1.1.1/zebrafy.egg-info/
+-rw-r--r--   0 m         (1000) m         (1000)    11154 2024-05-12 01:59:26.000000 zebrafy-1.1.1/zebrafy.egg-info/PKG-INFO
+-rw-r--r--   0 m         (1000) m         (1000)      344 2024-05-12 01:59:26.000000 zebrafy-1.1.1/zebrafy.egg-info/SOURCES.txt
+-rw-r--r--   0 m         (1000) m         (1000)        1 2024-05-12 01:59:26.000000 zebrafy-1.1.1/zebrafy.egg-info/dependency_links.txt
+-rw-r--r--   0 m         (1000) m         (1000)      107 2024-05-12 01:59:26.000000 zebrafy-1.1.1/zebrafy.egg-info/requires.txt
+-rw-r--r--   0 m         (1000) m         (1000)        8 2024-05-12 01:59:26.000000 zebrafy-1.1.1/zebrafy.egg-info/top_level.txt
```

### Comparing `zebrafy-1.1.0/LICENSE.txt` & `zebrafy-1.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zebrafy-1.1.0/PKG-INFO` & `zebrafy-1.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zebrafy
-Version: 1.1.0
+Version: 1.1.1
 Summary: Python library for converting PDF and images to Zebra Programming Language (ZPL)
 Author-email: Miika Nissi <miika@miikanissi.com>
 Maintainer-email: Miika Nissi <miika@miikanissi.com>
 License: LGPLv3
 Project-URL: Homepage, https://github.com/miikanissi/zebrafy/
 Project-URL: Documentation, https://zebrafy.readthedocs.io/
 Classifier: Development Status :: 4 - Beta
@@ -44,15 +44,15 @@
     :target: https://github.com/miikanissi/zebrafy/actions/workflows/ci.yml
     :alt: CI
 
 .. image:: https://readthedocs.org/projects/zebrafy/badge/?version=latest
     :target: https://zebrafy.readthedocs.io/en/latest/?badge=latest
     :alt: Documentation Status
 
-.. image:: https://img.shields.io/badge/pypi-1.1.0-blue
+.. image:: https://img.shields.io/badge/pypi-1.1.1-blue
     :target: https://pypi.org/project/zebrafy/
     :alt: PyPi Package
 
 .. image:: https://img.shields.io/badge/license-LGPLv3-green
     :target: https://www.gnu.org/licenses/lgpl-3.0.en.html#license-text
     :alt: License
 
@@ -91,14 +91,22 @@
 | ``pos_x``            | Pixel x position of the graphic field in resulting ZPL (default ``0``)                                       |
 +----------------------+--------------------------------------------------------------------------------------------------------------+
 | ``pos_y``            | Pixel y position of the graphic field in resulting ZPL (default ``0``)                                       |
 +----------------------+--------------------------------------------------------------------------------------------------------------+
 | ``complete_zpl``     | Add ZPL header and footer or only get the ZPL graphic field output (``True`` or ``False``, default ``True``) |
 +----------------------+--------------------------------------------------------------------------------------------------------------+
 
+Additionally, **ZebrafyPDF** supports the following optional parameters:
+
++----------------------+--------------------------------------------------------------------------------------------------------------+
+| Parameter            | Description                                                                                                  |
++======================+==============================================================================================================+
+| ``split_pages``      | Split the PDF into separate ZPL labels for each page (``True`` or ``False``, default ``False``)              |
++----------------------+--------------------------------------------------------------------------------------------------------------+
+
 Getting Started
 ---------------
 
 Installation
 ^^^^^^^^^^^^
 
 .. code-block:: console
```

### Comparing `zebrafy-1.1.0/README.rst` & `zebrafy-1.1.1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     :target: https://github.com/miikanissi/zebrafy/actions/workflows/ci.yml
     :alt: CI
 
 .. image:: https://readthedocs.org/projects/zebrafy/badge/?version=latest
     :target: https://zebrafy.readthedocs.io/en/latest/?badge=latest
     :alt: Documentation Status
 
-.. image:: https://img.shields.io/badge/pypi-1.1.0-blue
+.. image:: https://img.shields.io/badge/pypi-1.1.1-blue
     :target: https://pypi.org/project/zebrafy/
     :alt: PyPi Package
 
 .. image:: https://img.shields.io/badge/license-LGPLv3-green
     :target: https://www.gnu.org/licenses/lgpl-3.0.en.html#license-text
     :alt: License
 
@@ -55,14 +55,22 @@
 | ``pos_x``            | Pixel x position of the graphic field in resulting ZPL (default ``0``)                                       |
 +----------------------+--------------------------------------------------------------------------------------------------------------+
 | ``pos_y``            | Pixel y position of the graphic field in resulting ZPL (default ``0``)                                       |
 +----------------------+--------------------------------------------------------------------------------------------------------------+
 | ``complete_zpl``     | Add ZPL header and footer or only get the ZPL graphic field output (``True`` or ``False``, default ``True``) |
 +----------------------+--------------------------------------------------------------------------------------------------------------+
 
+Additionally, **ZebrafyPDF** supports the following optional parameters:
+
++----------------------+--------------------------------------------------------------------------------------------------------------+
+| Parameter            | Description                                                                                                  |
++======================+==============================================================================================================+
+| ``split_pages``      | Split the PDF into separate ZPL labels for each page (``True`` or ``False``, default ``False``)              |
++----------------------+--------------------------------------------------------------------------------------------------------------+
+
 Getting Started
 ---------------
 
 Installation
 ^^^^^^^^^^^^
 
 .. code-block:: console
```

### Comparing `zebrafy-1.1.0/pyproject.toml` & `zebrafy-1.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "zebrafy"
-version = "1.1.0"
+version = "1.1.1"
 description = "Python library for converting PDF and images to Zebra Programming Language (ZPL)"
 classifiers = [
     "Development Status :: 4 - Beta",
     "License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)",
     "Operating System :: OS Independent",
     "Natural Language :: English",
     "Programming Language :: Python",
```

### Comparing `zebrafy-1.1.0/tests/test_zebrafy.py` & `zebrafy-1.1.1/tests/test_zebrafy.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
             os.path.join(os.path.join(os.path.dirname(__file__), "static"), file_name),
             open_mode,
         ) as file:
             return file.read()
 
     def test_version(self):
         """Test package version."""
-        self.assertEqual(__version__, "1.1.0")
+        self.assertEqual(__version__, "1.1.1")
 
     ###########
     # CRC Tests
     ###########
     def test_crc_data_bytes(self):
         with self.assertRaises(ValueError):
             CRC(None)
@@ -398,14 +398,23 @@
         pdf = self._read_static_file("test_pdf.pdf")
         zebrafy_pdf = ZebrafyPDF(pdf)
         with self.assertRaises(ValueError):
             zebrafy_pdf.complete_zpl = None
         with self.assertRaises(TypeError):
             zebrafy_pdf.complete_zpl = "123"
 
+    def test_zebrafy_pdf_split_pages(self):
+        """Test ZebrafyPDF split pages"""
+        pdf = self._read_static_file("test_pdf.pdf")
+        zebrafy_pdf = ZebrafyPDF(pdf)
+        with self.assertRaises(ValueError):
+            zebrafy_pdf.split_pages = None
+        with self.assertRaises(TypeError):
+            zebrafy_pdf.split_pages = "123"
+
     def test_pdf_to_default_zpl(self):
         """Test PDF to ZPL with default options."""
         default_zpl = ZebrafyPDF(self._read_static_file("test_pdf.pdf")).to_zpl()
         self.assertEqual(default_zpl, self._read_static_file("test_pdf_ascii.zpl"))
 
     def test_pdf_to_ascii_zpl(self):
         """Test PDF to ZPL with A (ASCII) compression."""
@@ -446,20 +455,27 @@
         """Test PDF to ZPL without dithering the PDF and high threshold."""
         gf_zpl = ZebrafyPDF(
             self._read_static_file("test_pdf.pdf"), dither=False, threshold=215
         ).to_zpl()
         self.assertEqual(gf_zpl, self._read_static_file("test_pdf_high_threshold.zpl"))
 
     def test_pdf_to_zpl_width_height(self):
-        """Test PDF to ZPL without dithering the PDF and high threshold."""
+        """Test PDF to ZPL with set width and height."""
         gf_zpl = ZebrafyPDF(
             self._read_static_file("test_pdf.pdf"), width=720, height=1280
         ).to_zpl()
         self.assertEqual(gf_zpl, self._read_static_file("test_pdf_width_height.zpl"))
 
+    def test_pdf_to_zpl_split_pages(self):
+        """Test PDF to ZPL with split pages."""
+        gf_zpl = ZebrafyPDF(
+            self._read_static_file("test_pdf.pdf"), split_pages=True
+        ).to_zpl()
+        self.assertEqual(gf_zpl, self._read_static_file("test_pdf_split_pages.zpl"))
+
     ##################
     # ZebrafyZPL Tests
     ##################
     def test_zebrafy_zpl_zpl_data(self):
         with self.assertRaises(ValueError):
             ZebrafyZPL(None)
         with self.assertRaises(TypeError):
```

### Comparing `zebrafy-1.1.0/zebrafy/crc.py` & `zebrafy-1.1.1/zebrafy/crc.py`

 * *Files identical despite different names*

### Comparing `zebrafy-1.1.0/zebrafy/graphic_field.py` & `zebrafy-1.1.1/zebrafy/graphic_field.py`

 * *Files identical despite different names*

### Comparing `zebrafy-1.1.0/zebrafy/zebrafy_image.py` & `zebrafy-1.1.1/zebrafy/zebrafy_image.py`

 * *Files identical despite different names*

### Comparing `zebrafy-1.1.0/zebrafy/zebrafy_pdf.py` & `zebrafy-1.1.1/zebrafy/zebrafy_pdf.py`

 * *Files 8% similar despite different names*

```diff
@@ -55,14 +55,16 @@
     to ``128``
     :param width: Width of the PDF in the resulting ZPL. If ``0``, use default PDF \
     width, defaults to ``0``
     :param height: Height of the PDF in the resulting ZPL. If ``0``, use default \
     PDF height, defaults to ``0``
     :param pos_x: X position of the PDF on the resulting ZPL, defaults to ``0``
     :param pos_y: Y position of the PDF on the resulting ZPL, defaults to ``0``
+    :param split_pages: Split each PDF page as a new ZPL label  \
+    (only applies if complete_zpl is set), defaults to ``False``
     :param complete_zpl: Return a complete ZPL with header and footer included. \
     Otherwise return only the graphic field, defaults to ``True``
 
     .. deprecated:: 1.1.0
         The `compression_type` parameter is deprecated in favor of `format` and will \
         be removed in version 2.0.0.
     """
@@ -75,14 +77,15 @@
         invert: bool = None,
         dither: bool = None,
         threshold: int = None,
         width: int = None,
         height: int = None,
         pos_x: int = None,
         pos_y: int = None,
+        split_pages: bool = None,
         complete_zpl: bool = None,
     ):
         self.pdf_bytes = pdf_bytes
         if format is None:
             if compression_type is None:
                 format = "ASCII"
             else:
@@ -105,14 +108,17 @@
         self.height = height
         if pos_x is None:
             pos_x = 0
         self.pos_x = pos_x
         if pos_y is None:
             pos_y = 0
         self.pos_y = pos_y
+        if split_pages is None:
+            split_pages = False
+        self.split_pages = split_pages
         if complete_zpl is None:
             complete_zpl = True
         self.complete_zpl = complete_zpl
 
     pdf_bytes = property(operator.attrgetter("_pdf_bytes"))
 
     @pdf_bytes.setter
@@ -245,14 +251,28 @@
             raise TypeError(
                 "Y position must be an integer. {param_type} was given.".format(
                     param_type=type(y)
                 )
             )
         self._pos_y = y
 
+    split_pages = property(operator.attrgetter("_split_pages"))
+
+    @split_pages.setter
+    def split_pages(self, s):
+        if s is None:
+            raise ValueError("Split pages cannot be empty.")
+        if not isinstance(s, bool):
+            raise TypeError(
+                "Split pages must be a boolean. {param_type} was given.".format(
+                    param_type=type(s)
+                )
+            )
+        self._split_pages = s
+
     complete_zpl = property(operator.attrgetter("_complete_zpl"))
 
     @complete_zpl.setter
     def complete_zpl(self, c):
         if c is None:
             raise ValueError("Complete ZPL cannot be empty.")
         if not isinstance(c, bool):
@@ -279,15 +299,15 @@
         Converts PDF bytes to Zebra Programming Language (ZPL).
 
         :returns: A complete ZPL file string which can be sent to a ZPL compatible \
         printer or a ZPL graphic field if complete_zpl is not set.
         """
         # Open and convert image to grayscale
         pdf = PdfDocument(self._pdf_bytes)
-        graphic_fields = ""
+        graphic_fields = []
         for page in pdf:
             bitmap = page.render(scale=1, rotation=0)
             pil_image = bitmap.to_pil()
             zebrafy_image = ZebrafyImage(
                 pil_image,
                 format=self._format,
                 invert=self._invert,
@@ -295,13 +315,23 @@
                 threshold=self._threshold,
                 width=self._width,
                 height=self._height,
                 pos_x=self._pos_x,
                 pos_y=self._pos_y,
                 complete_zpl=False,
             )
-            graphic_fields += zebrafy_image.to_zpl() + "\n"
 
+            page_zpl = zebrafy_image.to_zpl() + "\n"
+
+            graphic_fields.append(page_zpl)
+
+        zpl_string = ""
         if self._complete_zpl:
-            return "^XA\n" + graphic_fields + "^XZ\n"
+            if self._split_pages:
+                for graphic_field in graphic_fields:
+                    zpl_string += "^XA\n" + graphic_field + "^XZ\n"
+            else:
+                zpl_string = "^XA\n" + "".join(graphic_fields) + "^XZ\n"
+        else:
+            zpl_string = "".join(graphic_fields)
 
-        return graphic_fields
+        return zpl_string
```

### Comparing `zebrafy-1.1.0/zebrafy/zebrafy_zpl.py` & `zebrafy-1.1.1/zebrafy/zebrafy_zpl.py`

 * *Files identical despite different names*

### Comparing `zebrafy-1.1.0/zebrafy.egg-info/PKG-INFO` & `zebrafy-1.1.1/zebrafy.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zebrafy
-Version: 1.1.0
+Version: 1.1.1
 Summary: Python library for converting PDF and images to Zebra Programming Language (ZPL)
 Author-email: Miika Nissi <miika@miikanissi.com>
 Maintainer-email: Miika Nissi <miika@miikanissi.com>
 License: LGPLv3
 Project-URL: Homepage, https://github.com/miikanissi/zebrafy/
 Project-URL: Documentation, https://zebrafy.readthedocs.io/
 Classifier: Development Status :: 4 - Beta
@@ -44,15 +44,15 @@
     :target: https://github.com/miikanissi/zebrafy/actions/workflows/ci.yml
     :alt: CI
 
 .. image:: https://readthedocs.org/projects/zebrafy/badge/?version=latest
     :target: https://zebrafy.readthedocs.io/en/latest/?badge=latest
     :alt: Documentation Status
 
-.. image:: https://img.shields.io/badge/pypi-1.1.0-blue
+.. image:: https://img.shields.io/badge/pypi-1.1.1-blue
     :target: https://pypi.org/project/zebrafy/
     :alt: PyPi Package
 
 .. image:: https://img.shields.io/badge/license-LGPLv3-green
     :target: https://www.gnu.org/licenses/lgpl-3.0.en.html#license-text
     :alt: License
 
@@ -91,14 +91,22 @@
 | ``pos_x``            | Pixel x position of the graphic field in resulting ZPL (default ``0``)                                       |
 +----------------------+--------------------------------------------------------------------------------------------------------------+
 | ``pos_y``            | Pixel y position of the graphic field in resulting ZPL (default ``0``)                                       |
 +----------------------+--------------------------------------------------------------------------------------------------------------+
 | ``complete_zpl``     | Add ZPL header and footer or only get the ZPL graphic field output (``True`` or ``False``, default ``True``) |
 +----------------------+--------------------------------------------------------------------------------------------------------------+
 
+Additionally, **ZebrafyPDF** supports the following optional parameters:
+
++----------------------+--------------------------------------------------------------------------------------------------------------+
+| Parameter            | Description                                                                                                  |
++======================+==============================================================================================================+
+| ``split_pages``      | Split the PDF into separate ZPL labels for each page (``True`` or ``False``, default ``False``)              |
++----------------------+--------------------------------------------------------------------------------------------------------------+
+
 Getting Started
 ---------------
 
 Installation
 ^^^^^^^^^^^^
 
 .. code-block:: console
```

