# Comparing `tmp/tileget-0.3.1.tar.gz` & `tmp/tileget-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tileget-0.3.1.tar", max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `tileget-0.3.1.tar` & `tileget-0.4.0.tar`

### file list

```diff
@@ -1,6 +1,11 @@
--rw-r--r--   0        0        0     1055 2024-03-04 01:10:23.272409 tileget-0.3.1/LICENSE
--rw-r--r--   0        0        0     1721 2024-03-04 01:10:23.276409 tileget-0.3.1/README.md
--rw-r--r--   0        0        0      507 2024-03-04 01:10:23.276409 tileget-0.3.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-04 01:10:23.276409 tileget-0.3.1/tileget/__init__.py
--rw-r--r--   0        0        0     5618 2024-03-04 01:10:23.276409 tileget-0.3.1/tileget/__main__.py
--rw-r--r--   0        0        0     2351 1970-01-01 00:00:00.000000 tileget-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 tileget-0.4.0/requirements-dev.lock
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 tileget-0.4.0/requirements.lock
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 tileget-0.4.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tileget-0.4.0/tileget/__init__.py
+-rw-r--r--   0        0        0     4499 2020-02-02 00:00:00.000000 tileget-0.4.0/tileget/__main__.py
+-rw-r--r--   0        0        0     3722 2020-02-02 00:00:00.000000 tileget-0.4.0/tileget/arg.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 tileget-0.4.0/.gitignore
+-rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 tileget-0.4.0/LICENSE
+-rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 tileget-0.4.0/README.md
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 tileget-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 tileget-0.4.0/PKG-INFO
```

### Comparing `tileget-0.3.1/LICENSE` & `tileget-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tileget-0.3.1/README.md` & `tileget-0.4.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,54 +1,55 @@
+Metadata-Version: 2.3
+Name: tileget
+Version: 0.4.0
+Summary: Tile download utility - easily download xyz-tile data
+License-File: LICENSE
+Requires-Python: >=3.10
+Requires-Dist: pyproj>=3.6.1
+Requires-Dist: shapely>=2.0.3
+Requires-Dist: tiletanic>=1.1.0
+Description-Content-Type: text/markdown
+
 # tileget
 
 Tile download utility - easily download xyz-tile data.
 
 ## installation
 
 ```sh
 pip install tileget
 ```
 
 ## usage
 
 ```
-usage: tileget [-h] [--extent EXTENT EXTENT EXTENT EXTENT]
-                   [--geojson GEOJSON] [--minzoom MINZOOM] [--maxzoom MAXZOOM]
-                   [--interval INTERVAL] [--overwrite] [--timeout TIMEOUT]
-                   [--parallel PARALLEL]
-                   tileurl output_dir
+usage: __main__.py [-h] [-e OUTPUT_DIR] [-o OUTPUT_FILE] [--extent EXTENT EXTENT EXTENT EXTENT] [--geojson GEOJSON] [--minzoom MINZOOM] [--maxzoom MAXZOOM] [--interval INTERVAL] [--overwrite] [--timeout TIMEOUT] [--tms]
+                   tileurl
 
 xyz-tile download tool
 
 positional arguments:
   tileurl               xyz-tile url in {z}/{x}/{y} template
-  output_dir            output dir
 
-optional arguments:
+options:
   -h, --help            show this help message and exit
+  -e OUTPUT_DIR, --output_dir OUTPUT_DIR
+                        output dir
+  -o OUTPUT_FILE, --output_file OUTPUT_FILE
+                        output mbtiles file
   --extent EXTENT EXTENT EXTENT EXTENT
                         min_lon min_lat max_lon max_lat, whitespace delimited
-  --geojson GEOJSON     path to geojson file to get tile covered by features
+  --geojson GEOJSON     path to geojson file of Feature or FeatureCollection
   --minzoom MINZOOM     default to 0
   --maxzoom MAXZOOM     default to 16
-  --interval INTERVAL   time taken after each-request, set as miliseconds in
-                        interger, default to 500
+  --interval INTERVAL   time taken after each-request, set as miliseconds in interger, default to 500
   --overwrite           overwrite existing files
-  --timeout TIMEOUT     wait response until this value, set as seconds in
-                        integer, default to 5
-  --parallel PARALLEL   num of parallel requests
+  --timeout TIMEOUT     wait response until this value, set as miliseconds in integer, default to 5000
+  --tms                 if set, parse z/x/y as TMS
 ```
 
 ### examples
 
-#### get tiles in extent [141.23 40.56 142.45 43.78] and in zoomlevels 0-12
-
-
-```sh
-tileget https://cyberjapandata.gsi.go.jp/xyz/seamlessphoto/{z}/{x}/{y}.jpg ./output_dir --extent 141.23 40.56 142.45 43.78 --maxzoom 12
-```
-
-#### parallel download - 4 threads, zoomlevels 5-13
-
 ```sh
-tileget https://cyberjapandata.gsi.go.jp/xyz/seamlessphoto/{z}/{x}/{y}.jpg ./output_dir --extent 141.23 40.56 142.45 43.78 --minzoom 5 --maxzoom 13 --parallel 4
+tileget https://cyberjapandata.gsi.go.jp/xyz/seamlessphoto/{z}/{x}/{y}.jpg -e ./output_dir --extent 141.23 40.56 142.45 43.78 --maxzoom 12
+tileget https://cyberjapandata.gsi.go.jp/xyz/seamlessphoto/{z}/{x}/{y}.jpg -o ./output.mbtiles
 ```
```

