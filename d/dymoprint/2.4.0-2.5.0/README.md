# Comparing `tmp/dymoprint-2.4.0.tar.gz` & `tmp/dymoprint-2.5.0.tar.gz`

## Comparing `dymoprint-2.4.0.tar` & `dymoprint-2.5.0.tar`

### file list

```diff
@@ -1,42 +1,44 @@
--rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 dymoprint-2.4.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 dymoprint-2.4.0/dymoprint.ini
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 dymoprint-2.4.0/.github/dependabot.yml
--rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 dymoprint-2.4.0/.github/workflows/pypi-publish.yml
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 dymoprint-2.4.0/.github/workflows/tests.yml
--rw-r--r--   0        0        0    34893 2020-02-02 00:00:00.000000 dymoprint-2.4.0/doc/DymoPrint_example_1.png
--rw-r--r--   0        0        0    40573 2020-02-02 00:00:00.000000 dymoprint-2.4.0/doc/DymoPrint_example_2.png
--rw-r--r--   0        0        0    37194 2020-02-02 00:00:00.000000 dymoprint-2.4.0/doc/DymoPrint_example_3.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dymoprint-2.4.0/src/__init__.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 dymoprint-2.4.0/src/dymoprint/__init__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 dymoprint-2.4.0/src/dymoprint/_version.py
--rwxr-xr-x   0        0        0     3811 2020-02-02 00:00:00.000000 dymoprint-2.4.0/src/dymoprint/barcode_writer.py
--rwxr-xr-x   0        0        0     7846 2020-02-02 00:00:00.000000 dymoprint-2.4.0/src/dymoprint/command_line.py
--rwxr-xr-x   0        0        0     2781 2020-02-02 00:00:00.000000 dymoprint-2.4.0/src/dymoprint/constants.py
--rw-r--r--   0        0        0     7362 2020-02-02 00:00:00.000000 dymoprint-2.4.0/src/dymoprint/detect.py
--rw-r--r--   0        0        0    12948 2020-02-02 00:00:00.000000 dymoprint-2.4.0/src/dymoprint/dymo_print_engines.py
--rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 dymoprint-2.4.0/src/dymoprint/font_config.py
--rw-r--r--   0        0        0     6504 2020-02-02 00:00:00.000000 dymoprint-2.4.0/src/dymoprint/gui.py
--rwxr-xr-x   0        0        0     7607 2020-02-02 00:00:00.000000 dymoprint-2.4.0/src/dymoprint/labeler.py
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 dymoprint-2.4.0/src/dymoprint/metadata.py
--rw-r--r--   0        0        0    15290 2020-02-02 00:00:00.000000 dymoprint-2.4.0/src/dymoprint/q_dymo_label_widgets.py
--rw-r--r--   0        0        0     6035 2020-02-02 00:00:00.000000 dymoprint-2.4.0/src/dymoprint/q_dymo_labels_list.py
--rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 dymoprint-2.4.0/src/dymoprint/unicode_blocks.py
--rwxr-xr-x   0        0        0      897 2020-02-02 00:00:00.000000 dymoprint-2.4.0/src/dymoprint/utils.py
--rw-r--r--   0        0        0   690516 2020-02-02 00:00:00.000000 dymoprint-2.4.0/src/dymoprint/resources/fonts/Carlito-Bold.ttf
--rw-r--r--   0        0        0   816716 2020-02-02 00:00:00.000000 dymoprint-2.4.0/src/dymoprint/resources/fonts/Carlito-BoldItalic.ttf
--rw-r--r--   0        0        0   623416 2020-02-02 00:00:00.000000 dymoprint-2.4.0/src/dymoprint/resources/fonts/Carlito-Italic.ttf
--rw-r--r--   0        0        0   635996 2020-02-02 00:00:00.000000 dymoprint-2.4.0/src/dymoprint/resources/fonts/Carlito-Regular.ttf
--rw-r--r--   0        0        0     4247 2020-02-02 00:00:00.000000 dymoprint-2.4.0/src/dymoprint/resources/fonts/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dymoprint-2.4.0/src/dymoprint/resources/fonts/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dymoprint-2.4.0/src/dymoprint/resources/icons/__init__.py
--rw-r--r--   0        0        0     6027 2020-02-02 00:00:00.000000 dymoprint-2.4.0/src/dymoprint/resources/icons/barcode_icon.png
--rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 dymoprint-2.4.0/src/dymoprint/resources/icons/barcode_text_icon.png
--rw-r--r--   0        0        0     2733 2020-02-02 00:00:00.000000 dymoprint-2.4.0/src/dymoprint/resources/icons/gui_icon.png
--rw-r--r--   0        0        0     5193 2020-02-02 00:00:00.000000 dymoprint-2.4.0/src/dymoprint/resources/icons/img_icon.png
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 dymoprint-2.4.0/src/dymoprint/resources/icons/qr_icon.png
--rw-r--r--   0        0        0     3506 2020-02-02 00:00:00.000000 dymoprint-2.4.0/src/dymoprint/resources/icons/txt_icon.png
--rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 dymoprint-2.4.0/.gitignore
--rw-r--r--   0        0        0    11324 2020-02-02 00:00:00.000000 dymoprint-2.4.0/LICENSE
--rw-r--r--   0        0        0     5682 2020-02-02 00:00:00.000000 dymoprint-2.4.0/README.md
--rw-r--r--   0        0        0     3350 2020-02-02 00:00:00.000000 dymoprint-2.4.0/pyproject.toml
--rw-r--r--   0        0        0     6869 2020-02-02 00:00:00.000000 dymoprint-2.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 dymoprint-2.5.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    42698 2020-02-02 00:00:00.000000 dymoprint-2.5.0/dymoprint-deprecation.webp
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 dymoprint-2.5.0/dymoprint.ini
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 dymoprint-2.5.0/.github/dependabot.yml
+-rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 dymoprint-2.5.0/.github/workflows/pre-commit-checks.yml
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 dymoprint-2.5.0/.github/workflows/pypi-publish.yml
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 dymoprint-2.5.0/.github/workflows/tests.yml
+-rw-r--r--   0        0        0    34893 2020-02-02 00:00:00.000000 dymoprint-2.5.0/doc/DymoPrint_example_1.png
+-rw-r--r--   0        0        0    40573 2020-02-02 00:00:00.000000 dymoprint-2.5.0/doc/DymoPrint_example_2.png
+-rw-r--r--   0        0        0    37194 2020-02-02 00:00:00.000000 dymoprint-2.5.0/doc/DymoPrint_example_3.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dymoprint-2.5.0/src/__init__.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 dymoprint-2.5.0/src/dymoprint/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 dymoprint-2.5.0/src/dymoprint/_version.py
+-rwxr-xr-x   0        0        0     3811 2020-02-02 00:00:00.000000 dymoprint-2.5.0/src/dymoprint/barcode_writer.py
+-rwxr-xr-x   0        0        0     8262 2020-02-02 00:00:00.000000 dymoprint-2.5.0/src/dymoprint/command_line.py
+-rwxr-xr-x   0        0        0     3936 2020-02-02 00:00:00.000000 dymoprint-2.5.0/src/dymoprint/constants.py
+-rw-r--r--   0        0        0     7362 2020-02-02 00:00:00.000000 dymoprint-2.5.0/src/dymoprint/detect.py
+-rw-r--r--   0        0        0    12948 2020-02-02 00:00:00.000000 dymoprint-2.5.0/src/dymoprint/dymo_print_engines.py
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 dymoprint-2.5.0/src/dymoprint/font_config.py
+-rw-r--r--   0        0        0     6824 2020-02-02 00:00:00.000000 dymoprint-2.5.0/src/dymoprint/gui.py
+-rwxr-xr-x   0        0        0     7607 2020-02-02 00:00:00.000000 dymoprint-2.5.0/src/dymoprint/labeler.py
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 dymoprint-2.5.0/src/dymoprint/metadata.py
+-rw-r--r--   0        0        0    15290 2020-02-02 00:00:00.000000 dymoprint-2.5.0/src/dymoprint/q_dymo_label_widgets.py
+-rw-r--r--   0        0        0     6035 2020-02-02 00:00:00.000000 dymoprint-2.5.0/src/dymoprint/q_dymo_labels_list.py
+-rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 dymoprint-2.5.0/src/dymoprint/unicode_blocks.py
+-rwxr-xr-x   0        0        0      897 2020-02-02 00:00:00.000000 dymoprint-2.5.0/src/dymoprint/utils.py
+-rw-r--r--   0        0        0   690516 2020-02-02 00:00:00.000000 dymoprint-2.5.0/src/dymoprint/resources/fonts/Carlito-Bold.ttf
+-rw-r--r--   0        0        0   816716 2020-02-02 00:00:00.000000 dymoprint-2.5.0/src/dymoprint/resources/fonts/Carlito-BoldItalic.ttf
+-rw-r--r--   0        0        0   623416 2020-02-02 00:00:00.000000 dymoprint-2.5.0/src/dymoprint/resources/fonts/Carlito-Italic.ttf
+-rw-r--r--   0        0        0   635996 2020-02-02 00:00:00.000000 dymoprint-2.5.0/src/dymoprint/resources/fonts/Carlito-Regular.ttf
+-rw-r--r--   0        0        0     4247 2020-02-02 00:00:00.000000 dymoprint-2.5.0/src/dymoprint/resources/fonts/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dymoprint-2.5.0/src/dymoprint/resources/fonts/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dymoprint-2.5.0/src/dymoprint/resources/icons/__init__.py
+-rw-r--r--   0        0        0     6027 2020-02-02 00:00:00.000000 dymoprint-2.5.0/src/dymoprint/resources/icons/barcode_icon.png
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 dymoprint-2.5.0/src/dymoprint/resources/icons/barcode_text_icon.png
+-rw-r--r--   0        0        0     2733 2020-02-02 00:00:00.000000 dymoprint-2.5.0/src/dymoprint/resources/icons/gui_icon.png
+-rw-r--r--   0        0        0     5193 2020-02-02 00:00:00.000000 dymoprint-2.5.0/src/dymoprint/resources/icons/img_icon.png
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 dymoprint-2.5.0/src/dymoprint/resources/icons/qr_icon.png
+-rw-r--r--   0        0        0     3506 2020-02-02 00:00:00.000000 dymoprint-2.5.0/src/dymoprint/resources/icons/txt_icon.png
+-rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 dymoprint-2.5.0/.gitignore
+-rw-r--r--   0        0        0    11324 2020-02-02 00:00:00.000000 dymoprint-2.5.0/LICENSE
+-rw-r--r--   0        0        0     1349 2020-02-02 00:00:00.000000 dymoprint-2.5.0/README.md
+-rw-r--r--   0        0        0     3350 2020-02-02 00:00:00.000000 dymoprint-2.5.0/pyproject.toml
+-rw-r--r--   0        0        0     2536 2020-02-02 00:00:00.000000 dymoprint-2.5.0/PKG-INFO
```

### Comparing `dymoprint-2.4.0/.pre-commit-config.yaml` & `dymoprint-2.5.0/.pre-commit-config.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 repos:
 - repo: https://github.com/pre-commit/pre-commit-hooks
-  rev: v4.5.0
+  rev: v4.6.0
   hooks:
   - id: no-commit-to-branch
     args: [--branch, master, --branch, main]
   - id: trailing-whitespace
   - id: check-added-large-files
   - id: check-ast
   - id: check-json
@@ -14,31 +14,31 @@
   - id: debug-statements
   - id: end-of-file-fixer
   - id: requirements-txt-fixer
   - id: mixed-line-ending
     args: ['--fix=lf']
 
 - repo: https://github.com/asottile/pyupgrade
-  rev: v3.15.0
+  rev: v3.15.2
   hooks:
   - id: pyupgrade
     args: ["--py38-plus", "--keep-runtime-typing"]
 
 - repo: https://github.com/pycqa/isort
-  rev: 5.12.0
+  rev: 5.13.2
   hooks:
   - id: isort
     args: ["--settings-path=pyproject.toml"]
 
 - repo: https://github.com/psf/black
-  rev: 23.11.0
+  rev: 24.4.0
   hooks:
   - id: black
     language_version: python3
 
 - repo: https://github.com/pycqa/flake8
-  rev: 6.1.0
+  rev: 7.0.0
   hooks:
   - id: flake8
     args:
     - --max-line-length=88  # default of Black
     - --extend-ignore=E203  # conflicts with Black
```

### Comparing `dymoprint-2.4.0/.github/workflows/pypi-publish.yml` & `dymoprint-2.5.0/.github/workflows/pypi-publish.yml`

 * *Files 18% similar despite different names*

```diff
@@ -9,22 +9,22 @@
   deploy:
     runs-on: ubuntu-latest
     steps:
     - uses: actions/checkout@v4
       with:
         fetch-depth: 0
     - name: Set up Python
-      uses: actions/setup-python@v4
+      uses: actions/setup-python@v5
       with:
         python-version: '3.x'
     - name: Build
       run: |
         python -m pip install --upgrade pip build twine
         python -m build
     - name: Test wheels
       run: |
         python -m twine check dist/*
     - name: Publish
-      uses: pypa/gh-action-pypi-publish@v1.8.11
+      uses: pypa/gh-action-pypi-publish@v1.8.14
       with:
         user: ${{ secrets.PYPI_USERNAME }}
         password: ${{ secrets.PYPI_PASSWORD }}
```

### Comparing `dymoprint-2.4.0/.github/workflows/tests.yml` & `dymoprint-2.5.0/.github/workflows/tests.yml`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
       matrix:
         python-version: ["3.8", "3.9", "3.10", "3.11", "3.12"]
       fail-fast: false
 
     steps:
     - uses: actions/checkout@v4
     - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v4
+      uses: actions/setup-python@v5
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install tox tox-gh-actions
     - name: Test with tox
```

### Comparing `dymoprint-2.4.0/doc/DymoPrint_example_1.png` & `dymoprint-2.5.0/doc/DymoPrint_example_1.png`

 * *Files identical despite different names*

### Comparing `dymoprint-2.4.0/doc/DymoPrint_example_2.png` & `dymoprint-2.5.0/doc/DymoPrint_example_2.png`

 * *Files identical despite different names*

### Comparing `dymoprint-2.4.0/doc/DymoPrint_example_3.png` & `dymoprint-2.5.0/doc/DymoPrint_example_3.png`

 * *Files identical despite different names*

### Comparing `dymoprint-2.4.0/src/dymoprint/barcode_writer.py` & `dymoprint-2.5.0/src/dymoprint/barcode_writer.py`

 * *Files identical despite different names*

### Comparing `dymoprint-2.4.0/src/dymoprint/command_line.py` & `dymoprint-2.5.0/src/dymoprint/command_line.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
 from PIL import Image, ImageOps
 
 from . import __version__
 from .constants import (
     AVAILABLE_BARCODES,
     DEFAULT_MARGIN_PX,
+    DEPRECATION_MESSAGE_ANSI,
     PIXELS_PER_MM,
     USE_QR,
     e_qrcode,
 )
 from .dymo_print_engines import DymoRenderEngine, print_label
 from .font_config import font_filename
 from .metadata import our_metadata
@@ -159,107 +160,110 @@
 
     The print resolution is 7 pixels/mm, and margin is subtracted
     from each side."""
     return (mm * PIXELS_PER_MM) - margin * 2
 
 
 def main():
-    args = parse_args()
-    render_engine = DymoRenderEngine(args.t)
+    try:
+        args = parse_args()
+        render_engine = DymoRenderEngine(args.t)
 
-    # read config file
-    FONT_FILENAME = font_filename(args.s)
+        # read config file
+        FONT_FILENAME = font_filename(args.s)
 
-    labeltext = args.text
+        labeltext = args.text
 
-    if args.u is not None:
-        if os.path.isfile(args.u):
-            FONT_FILENAME = args.u
-        else:
-            die("Error: file '%s' not found." % args.u)
+        if args.u is not None:
+            if os.path.isfile(args.u):
+                FONT_FILENAME = args.u
+            else:
+                die("Error: file '%s' not found." % args.u)
 
-    # check if barcode, qrcode or text should be printed, use frames only on text
-    if args.qr and not USE_QR:
-        die("Error: %s" % e_qrcode)
+        # check if barcode, qrcode or text should be printed, use frames only on text
+        if args.qr and not USE_QR:
+            die("Error: %s" % e_qrcode)
 
-    if args.barcode and args.qr:
-        die("Error: can not print both QR and Barcode on the same label (yet)")
+        if args.barcode and args.qr:
+            die("Error: can not print both QR and Barcode on the same label (yet)")
 
-    if args.fixed_length is not None and (
-        args.min_length != 0 or args.max_length is not None
-    ):
-        die("Error: can't specify min/max and fixed length at the same time")
+        if args.fixed_length is not None and (
+            args.min_length != 0 or args.max_length is not None
+        ):
+            die("Error: can't specify min/max and fixed length at the same time")
 
-    if args.max_length is not None and args.max_length < args.min_length:
-        die("Error: maximum length is less than minimum length")
+        if args.max_length is not None and args.max_length < args.min_length:
+            die("Error: maximum length is less than minimum length")
 
-    bitmaps = []
+        bitmaps = []
 
-    if args.test_pattern:
-        bitmaps.append(render_engine.render_test(args.test_pattern))
+        if args.test_pattern:
+            bitmaps.append(render_engine.render_test(args.test_pattern))
 
-    if args.qr:
-        bitmaps.append(render_engine.render_qr(labeltext.pop(0)))
+        if args.qr:
+            bitmaps.append(render_engine.render_qr(labeltext.pop(0)))
 
-    elif args.barcode:
-        bitmaps.append(render_engine.render_barcode(labeltext.pop(0), args.barcode))
+        elif args.barcode:
+            bitmaps.append(render_engine.render_barcode(labeltext.pop(0), args.barcode))
 
-    elif args.barcode_text:
-        bitmaps.append(
-            render_engine.render_barcode_with_text(
-                labeltext.pop(0), args.barcode_text, FONT_FILENAME, args.f
+        elif args.barcode_text:
+            bitmaps.append(
+                render_engine.render_barcode_with_text(
+                    labeltext.pop(0), args.barcode_text, FONT_FILENAME, args.f
+                )
             )
-        )
 
-    if labeltext:
-        bitmaps.append(
-            render_engine.render_text(
-                text_lines=labeltext,
-                font_file_name=FONT_FILENAME,
-                frame_width_px=args.f,
-                font_size_ratio=int(args.scale) / 100.0,
-                align=args.a,
+        if labeltext:
+            bitmaps.append(
+                render_engine.render_text(
+                    text_lines=labeltext,
+                    font_file_name=FONT_FILENAME,
+                    frame_width_px=args.f,
+                    font_size_ratio=int(args.scale) / 100.0,
+                    align=args.a,
+                )
             )
-        )
 
-    if args.picture:
-        bitmaps.append(render_engine.render_picture(args.picture))
+        if args.picture:
+            bitmaps.append(render_engine.render_picture(args.picture))
+
+        margin = args.m
+        justify = args.j
+
+        if args.fixed_length is not None:
+            min_label_mm_len = args.fixed_length
+            max_label_mm_len = args.fixed_length
+        else:
+            min_label_mm_len = args.min_length
+            max_label_mm_len = args.max_length
 
-    margin = args.m
-    justify = args.j
+        min_payload_len_px = max(0, mm_to_payload_px(min_label_mm_len, margin))
+        max_payload_len_px = (
+            mm_to_payload_px(max_label_mm_len, margin)
+            if max_label_mm_len is not None
+            else None
+        )
 
-    if args.fixed_length is not None:
-        min_label_mm_len = args.fixed_length
-        max_label_mm_len = args.fixed_length
-    else:
-        min_label_mm_len = args.min_length
-        max_label_mm_len = args.max_length
-
-    min_payload_len_px = max(0, mm_to_payload_px(min_label_mm_len, margin))
-    max_payload_len_px = (
-        mm_to_payload_px(max_label_mm_len, margin)
-        if max_label_mm_len is not None
-        else None
-    )
-
-    label_bitmap = render_engine.merge_render(
-        bitmaps=bitmaps,
-        min_payload_len_px=min_payload_len_px,
-        max_payload_len_px=max_payload_len_px,
-        justify=justify,
-    )
-
-    # print or show the label
-    if args.preview or args.preview_inverted or args.imagemagick:
-        print("Demo mode: showing label..")
-        # fix size, adding print borders
-        label_image = Image.new(
-            "L", (margin + label_bitmap.width + margin, label_bitmap.height)
+        label_bitmap = render_engine.merge_render(
+            bitmaps=bitmaps,
+            min_payload_len_px=min_payload_len_px,
+            max_payload_len_px=max_payload_len_px,
+            justify=justify,
         )
-        label_image.paste(label_bitmap, (margin, 0))
-        if args.preview or args.preview_inverted:
-            label_rotated = label_bitmap.transpose(Image.ROTATE_270)
-            print(image_to_unicode(label_rotated, invert=args.preview_inverted))
-        if args.imagemagick:
-            ImageOps.invert(label_image).show()
-    else:
-        print_label(label_bitmap, margin_px=args.m, tape_size_mm=args.t)
+
+        # print or show the label
+        if args.preview or args.preview_inverted or args.imagemagick:
+            print("Demo mode: showing label..")
+            # fix size, adding print borders
+            label_image = Image.new(
+                "L", (margin + label_bitmap.width + margin, label_bitmap.height)
+            )
+            label_image.paste(label_bitmap, (margin, 0))
+            if args.preview or args.preview_inverted:
+                label_rotated = label_bitmap.transpose(Image.ROTATE_270)
+                print(image_to_unicode(label_rotated, invert=args.preview_inverted))
+            if args.imagemagick:
+                ImageOps.invert(label_image).show()
+        else:
+            print_label(label_bitmap, margin_px=args.m, tape_size_mm=args.t)
+    finally:
+        print(DEPRECATION_MESSAGE_ANSI)
```

### Comparing `dymoprint-2.4.0/src/dymoprint/detect.py` & `dymoprint-2.5.0/src/dymoprint/detect.py`

 * *Files identical despite different names*

### Comparing `dymoprint-2.4.0/src/dymoprint/dymo_print_engines.py` & `dymoprint-2.5.0/src/dymoprint/dymo_print_engines.py`

 * *Files identical despite different names*

### Comparing `dymoprint-2.4.0/src/dymoprint/font_config.py` & `dymoprint-2.5.0/src/dymoprint/font_config.py`

 * *Files identical despite different names*

### Comparing `dymoprint-2.4.0/src/dymoprint/gui.py` & `dymoprint-2.5.0/src/dymoprint/gui.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,24 +17,35 @@
     QSpinBox,
     QToolBar,
     QVBoxLayout,
     QWidget,
 )
 from usb.core import USBError
 
-from .constants import DEFAULT_MARGIN_PX, ICON_DIR
+from .constants import DEFAULT_MARGIN_PX, DEPRECATION_MESSAGE_POPUP, ICON_DIR
 from .dymo_print_engines import DymoRenderEngine, print_label
 from .q_dymo_labels_list import QDymoLabelList
 
 
+class DeprecationPopup(QMessageBox):
+    def __init__(self):
+        super().__init__()
+        self.setWindowTitle("Deprecation Warning")
+        self.setText(DEPRECATION_MESSAGE_POPUP)
+        self.setIcon(QMessageBox.Icon.Warning)
+
+
 class DymoPrintWindow(QWidget):
     label_bitmap: Optional[Image.Image]
 
     def __init__(self):
         super().__init__()
+        popup = DeprecationPopup()
+        popup.exec()
+
         self.render_engine = DymoRenderEngine(12)
         self.label_bitmap = None
 
         self.window_layout = QVBoxLayout()
         self.list = QDymoLabelList(self.render_engine)
         self.label_render = QLabel()
         self.print_button = QPushButton()
```

### Comparing `dymoprint-2.4.0/src/dymoprint/labeler.py` & `dymoprint-2.5.0/src/dymoprint/labeler.py`

 * *Files identical despite different names*

### Comparing `dymoprint-2.4.0/src/dymoprint/q_dymo_label_widgets.py` & `dymoprint-2.5.0/src/dymoprint/q_dymo_label_widgets.py`

 * *Files identical despite different names*

### Comparing `dymoprint-2.4.0/src/dymoprint/q_dymo_labels_list.py` & `dymoprint-2.5.0/src/dymoprint/q_dymo_labels_list.py`

 * *Files identical despite different names*

### Comparing `dymoprint-2.4.0/src/dymoprint/unicode_blocks.py` & `dymoprint-2.5.0/src/dymoprint/unicode_blocks.py`

 * *Files identical despite different names*

### Comparing `dymoprint-2.4.0/src/dymoprint/utils.py` & `dymoprint-2.5.0/src/dymoprint/utils.py`

 * *Files identical despite different names*

### Comparing `dymoprint-2.4.0/src/dymoprint/resources/fonts/Carlito-Bold.ttf` & `dymoprint-2.5.0/src/dymoprint/resources/fonts/Carlito-Bold.ttf`

 * *Files identical despite different names*

### Comparing `dymoprint-2.4.0/src/dymoprint/resources/fonts/Carlito-BoldItalic.ttf` & `dymoprint-2.5.0/src/dymoprint/resources/fonts/Carlito-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `dymoprint-2.4.0/src/dymoprint/resources/fonts/Carlito-Italic.ttf` & `dymoprint-2.5.0/src/dymoprint/resources/fonts/Carlito-Italic.ttf`

 * *Files identical despite different names*

### Comparing `dymoprint-2.4.0/src/dymoprint/resources/fonts/Carlito-Regular.ttf` & `dymoprint-2.5.0/src/dymoprint/resources/fonts/Carlito-Regular.ttf`

 * *Files identical despite different names*

### Comparing `dymoprint-2.4.0/src/dymoprint/resources/fonts/LICENSE` & `dymoprint-2.5.0/src/dymoprint/resources/fonts/LICENSE`

 * *Files identical despite different names*

### Comparing `dymoprint-2.4.0/src/dymoprint/resources/icons/barcode_icon.png` & `dymoprint-2.5.0/src/dymoprint/resources/icons/barcode_icon.png`

 * *Files identical despite different names*

### Comparing `dymoprint-2.4.0/src/dymoprint/resources/icons/gui_icon.png` & `dymoprint-2.5.0/src/dymoprint/resources/icons/gui_icon.png`

 * *Files identical despite different names*

### Comparing `dymoprint-2.4.0/src/dymoprint/resources/icons/img_icon.png` & `dymoprint-2.5.0/src/dymoprint/resources/icons/img_icon.png`

 * *Files identical despite different names*

### Comparing `dymoprint-2.4.0/src/dymoprint/resources/icons/txt_icon.png` & `dymoprint-2.5.0/src/dymoprint/resources/icons/txt_icon.png`

 * *Files identical despite different names*

### Comparing `dymoprint-2.4.0/.gitignore` & `dymoprint-2.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dymoprint-2.4.0/LICENSE` & `dymoprint-2.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dymoprint-2.4.0/pyproject.toml` & `dymoprint-2.5.0/pyproject.toml`

 * *Files identical despite different names*

