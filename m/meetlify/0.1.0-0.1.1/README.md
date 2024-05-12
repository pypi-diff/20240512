# Comparing `tmp/meetlify-0.1.0.tar.gz` & `tmp/meetlify-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meetlify-0.1.0.tar", last modified: Sun May 12 01:55:28 2024, max compression
+gzip compressed data, was "meetlify-0.1.1.tar", last modified: Sun May 12 02:13:27 2024, max compression
```

## Comparing `meetlify-0.1.0.tar` & `meetlify-0.1.1.tar`

### file list

```diff
@@ -1,112 +1,112 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 01:55:28.969754 meetlify-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-12 01:55:20.000000 meetlify-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-12 01:55:20.000000 meetlify-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6355 2024-05-12 01:55:28.969754 meetlify-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3474 2024-05-12 01:55:20.000000 meetlify-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-12 01:55:20.000000 meetlify-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-12 01:55:28.969754 meetlify-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4746 2024-05-12 01:55:20.000000 meetlify-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 01:55:28.937754 meetlify-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 01:55:28.941754 meetlify-0.1.0/src/meetlify/
--rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-05-12 01:55:20.000000 meetlify-0.1.0/src/meetlify/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9154 2024-05-12 01:55:20.000000 meetlify-0.1.0/src/meetlify/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3149 2024-05-12 01:55:20.000000 meetlify-0.1.0/src/meetlify/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3517 2024-05-12 01:55:20.000000 meetlify-0.1.0/src/meetlify/configs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-05-12 01:55:20.000000 meetlify-0.1.0/src/meetlify/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     3005 2024-05-12 01:55:20.000000 meetlify-0.1.0/src/meetlify/meetup.py
--rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-05-12 01:55:20.000000 meetlify-0.1.0/src/meetlify/page.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 01:55:28.941754 meetlify-0.1.0/src/meetlify/share/
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-12 01:55:20.000000 meetlify-0.1.0/src/meetlify/share/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-12 01:55:20.000000 meetlify-0.1.0/src/meetlify/share/configs.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 01:55:28.937754 meetlify-0.1.0/src/meetlify/share/content/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 01:55:28.941754 meetlify-0.1.0/src/meetlify/share/content/images/
--rw-r--r--   0 runner    (1001) docker     (127)   128599 2024-05-12 01:55:20.000000 meetlify-0.1.0/src/meetlify/share/content/images/fatureimage.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 01:55:28.941754 meetlify-0.1.0/src/meetlify/share/content/meetups/
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-12 01:55:20.000000 meetlify-0.1.0/src/meetlify/share/content/meetups/0001.md
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-12 01:55:20.000000 meetlify-0.1.0/src/meetlify/share/content/meetups/0002.md
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-12 01:55:20.000000 meetlify-0.1.0/src/meetlify/share/content/meetups/0003.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 01:55:28.941754 meetlify-0.1.0/src/meetlify/share/content/pages/
--rw-r--r--   0 runner    (1001) docker     (127)     3984 2024-05-12 01:55:20.000000 meetlify-0.1.0/src/meetlify/share/content/pages/contact.md
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-12 01:55:20.000000 meetlify-0.1.0/src/meetlify/share/content/pages/home.md
--rw-r--r--   0 runner    (1001) docker     (127)     3915 2024-05-12 01:55:20.000000 meetlify-0.1.0/src/meetlify/share/content/pages/privacy.md
--rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-05-12 01:55:20.000000 meetlify-0.1.0/src/meetlify/share/content/pages/terms.md
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-12 01:55:20.000000 meetlify-0.1.0/src/meetlify/share/robots.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 01:55:28.937754 meetlify-0.1.0/src/meetlify/themes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 01:55:28.937754 meetlify-0.1.0/src/meetlify/themes/lindau/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 01:55:28.937754 meetlify-0.1.0/src/meetlify/themes/lindau/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 01:55:28.945754 meetlify-0.1.0/src/meetlify/themes/lindau/static/assets/
--rw-r--r--   0 runner    (1001) docker     (127)   362926 2024-05-12 01:55:20.000000 meetlify-0.1.0/src/meetlify/themes/lindau/static/assets/about.png
--rw-r--r--   0 runner    (1001) docker     (127)    50969 2024-05-12 01:55:20.000000 meetlify-0.1.0/src/meetlify/themes/lindau/static/assets/author.png
--rw-r--r--   0 runner    (1001) docker     (127)    10126 2024-05-12 01:55:20.000000 meetlify-0.1.0/src/meetlify/themes/lindau/static/assets/banner.png
--rw-r--r--   0 runner    (1001) docker     (127)    22993 2024-05-12 01:55:20.000000 meetlify-0.1.0/src/meetlify/themes/lindau/static/assets/favicon.png
--rw-r--r--   0 runner    (1001) docker     (127)     9139 2024-05-12 01:55:20.000000 meetlify-0.1.0/src/meetlify/themes/lindau/static/assets/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 01:55:28.957754 meetlify-0.1.0/src/meetlify/themes/lindau/static/css/
--rw-r--r--   0 runner    (1001) docker     (127)    70329 2024-05-12 01:55:20.000000 meetlify-0.1.0/src/meetlify/themes/lindau/static/css/bootstrap-grid.css
--rw-r--r--   0 runner    (1001) docker     (127)   203221 2024-05-12 01:55:20.000000 meetlify-0.1.0/src/meetlify/themes/lindau/static/css/bootstrap-grid.css.map
--rw-r--r--   0 runner    (1001) docker     (127)    51795 2024-05-12 01:55:20.000000 meetlify-0.1.0/src/meetlify/themes/lindau/static/css/bootstrap-grid.min.css
--rw-r--r--   0 runner    (1001) docker     (127)   115986 2024-05-12 01:55:20.000000 meetlify-0.1.0/src/meetlify/themes/lindau/static/css/bootstrap-grid.min.css.map
--rw-r--r--   0 runner    (1001) docker     (127)    70403 2024-05-12 01:55:20.000000 meetlify-0.1.0/src/meetlify/themes/lindau/static/css/bootstrap-grid.rtl.css
--rw-r--r--   0 runner    (1001) docker     (127)   203225 2024-05-12 01:55:20.000000 meetlify-0.1.0/src/meetlify/themes/lindau/static/css/bootstrap-grid.rtl.css.map
--rw-r--r--   0 runner    (1001) docker     (127)    51870 2024-05-12 01:55:20.000000 meetlify-0.1.0/src/meetlify/themes/lindau/static/css/bootstrap-grid.rtl.min.css
--rw-r--r--   0 runner    (1001) docker     (127)   116063 2024-05-12 01:55:20.000000 meetlify-0.1.0/src/meetlify/themes/lindau/static/css/bootstrap-grid.rtl.min.css.map
--rw-r--r--   0 runner    (1001) docker     (127)    65696 2024-05-12 01:55:20.000000 meetlify-0.1.0/src/meetlify/themes/lindau/static/css/bootstrap-icons.css
--rw-r--r--   0 runner    (1001) docker     (127)    12065 2024-05-12 01:55:20.000000 meetlify-0.1.0/src/meetlify/themes/lindau/static/css/bootstrap-reboot.css
--rw-r--r--   0 runner    (1001) docker     (127)   129371 2024-05-12 01:55:20.000000 meetlify-0.1.0/src/meetlify/themes/lindau/static/css/bootstrap-reboot.css.map
--rw-r--r--   0 runner    (1001) docker     (127)    10126 2024-05-12 01:55:20.000000 meetlify-0.1.0/src/meetlify/themes/lindau/static/css/bootstrap-reboot.min.css
--rw-r--r--   0 runner    (1001) docker     (127)    51369 2024-05-12 01:55:20.000000 meetlify-0.1.0/src/meetlify/themes/lindau/static/css/bootstrap-reboot.min.css.map
--rw-r--r--   0 runner    (1001) docker     (127)    12058 2024-05-12 01:55:20.000000 meetlify-0.1.0/src/meetlify/themes/lindau/static/css/bootstrap-reboot.rtl.css
--rw-r--r--   0 runner    (1001) docker     (127)   129386 2024-05-12 01:55:20.000000 meetlify-0.1.0/src/meetlify/themes/lindau/static/css/bootstrap-reboot.rtl.css.map
--rw-r--r--   0 runner    (1001) docker     (127)    10198 2024-05-12 01:55:20.000000 meetlify-0.1.0/src/meetlify/themes/lindau/static/css/bootstrap-reboot.rtl.min.css
--rw-r--r--   0 runner    (1001) docker     (127)    63943 2024-05-12 01:55:20.000000 meetlify-0.1.0/src/meetlify/themes/lindau/static/css/bootstrap-reboot.rtl.min.css.map
--rw-r--r--   0 runner    (1001) docker     (127)   107823 2024-05-12 01:55:20.000000 meetlify-0.1.0/src/meetlify/themes/lindau/static/css/bootstrap-utilities.css
--rw-r--r--   0 runner    (1001) docker     (127)   267535 2024-05-12 01:55:20.000000 meetlify-0.1.0/src/meetlify/themes/lindau/static/css/bootstrap-utilities.css.map
--rw-r--r--   0 runner    (1001) docker     (127)    85352 2024-05-12 01:55:20.000000 meetlify-0.1.0/src/meetlify/themes/lindau/static/css/bootstrap-utilities.min.css
--rw-r--r--   0 runner    (1001) docker     (127)   180381 2024-05-12 01:55:20.000000 meetlify-0.1.0/src/meetlify/themes/lindau/static/css/bootstrap-utilities.min.css.map
--rw-r--r--   0 runner    (1001) docker     (127)   107691 2024-05-12 01:55:20.000000 meetlify-0.1.0/src/meetlify/themes/lindau/static/css/bootstrap-utilities.rtl.css
--rw-r--r--   0 runner    (1001) docker     (127)   267476 2024-05-12 01:55:20.000000 meetlify-0.1.0/src/meetlify/themes/lindau/static/css/bootstrap-utilities.rtl.css.map
--rw-r--r--   0 runner    (1001) docker     (127)    85281 2024-05-12 01:55:20.000000 meetlify-0.1.0/src/meetlify/themes/lindau/static/css/bootstrap-utilities.rtl.min.css
--rw-r--r--   0 runner    (1001) docker     (127)   180217 2024-05-12 01:55:20.000000 meetlify-0.1.0/src/meetlify/themes/lindau/static/css/bootstrap-utilities.rtl.min.css.map
--rw-r--r--   0 runner    (1001) docker     (127)   281046 2024-05-12 01:55:20.000000 meetlify-0.1.0/src/meetlify/themes/lindau/static/css/bootstrap.css
--rw-r--r--   0 runner    (1001) docker     (127)   679755 2024-05-12 01:55:20.000000 meetlify-0.1.0/src/meetlify/themes/lindau/static/css/bootstrap.css.map
--rw-r--r--   0 runner    (1001) docker     (127)   232803 2024-05-12 01:55:20.000000 meetlify-0.1.0/src/meetlify/themes/lindau/static/css/bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (127)   589892 2024-05-12 01:55:20.000000 meetlify-0.1.0/src/meetlify/themes/lindau/static/css/bootstrap.min.css.map
--rw-r--r--   0 runner    (1001) docker     (127)   280259 2024-05-12 01:55:20.000000 meetlify-0.1.0/src/meetlify/themes/lindau/static/css/bootstrap.rtl.css
--rw-r--r--   0 runner    (1001) docker     (127)   679615 2024-05-12 01:55:20.000000 meetlify-0.1.0/src/meetlify/themes/lindau/static/css/bootstrap.rtl.css.map
--rw-r--r--   0 runner    (1001) docker     (127)   232911 2024-05-12 01:55:20.000000 meetlify-0.1.0/src/meetlify/themes/lindau/static/css/bootstrap.rtl.min.css
--rw-r--r--   0 runner    (1001) docker     (127)   589087 2024-05-12 01:55:20.000000 meetlify-0.1.0/src/meetlify/themes/lindau/static/css/bootstrap.rtl.min.css.map
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 01:55:28.957754 meetlify-0.1.0/src/meetlify/themes/lindau/static/css/fonts/
--rw-r--r--   0 runner    (1001) docker     (127)   113656 2024-05-12 01:55:20.000000 meetlify-0.1.0/src/meetlify/themes/lindau/static/css/fonts/bootstrap-icons.woff
--rw-r--r--   0 runner    (1001) docker     (127)    85044 2024-05-12 01:55:20.000000 meetlify-0.1.0/src/meetlify/themes/lindau/static/css/fonts/bootstrap-icons.woff2
--rw-r--r--   0 runner    (1001) docker     (127)   237143 2024-05-12 01:55:20.000000 meetlify-0.1.0/src/meetlify/themes/lindau/static/css/styles.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 01:55:28.965754 meetlify-0.1.0/src/meetlify/themes/lindau/static/js/
--rw-r--r--   0 runner    (1001) docker     (127)   207819 2024-05-12 01:55:20.000000 meetlify-0.1.0/src/meetlify/themes/lindau/static/js/bootstrap.bundle.js
--rw-r--r--   0 runner    (1001) docker     (127)   444579 2024-05-12 01:55:20.000000 meetlify-0.1.0/src/meetlify/themes/lindau/static/js/bootstrap.bundle.js.map
--rw-r--r--   0 runner    (1001) docker     (127)    80721 2024-05-12 01:55:20.000000 meetlify-0.1.0/src/meetlify/themes/lindau/static/js/bootstrap.bundle.min.js
--rw-r--r--   0 runner    (1001) docker     (127)   332090 2024-05-12 01:55:20.000000 meetlify-0.1.0/src/meetlify/themes/lindau/static/js/bootstrap.bundle.min.js.map
--rw-r--r--   0 runner    (1001) docker     (127)   135829 2024-05-12 01:55:20.000000 meetlify-0.1.0/src/meetlify/themes/lindau/static/js/bootstrap.esm.js
--rw-r--r--   0 runner    (1001) docker     (127)   305438 2024-05-12 01:55:20.000000 meetlify-0.1.0/src/meetlify/themes/lindau/static/js/bootstrap.esm.js.map
--rw-r--r--   0 runner    (1001) docker     (127)    73935 2024-05-12 01:55:20.000000 meetlify-0.1.0/src/meetlify/themes/lindau/static/js/bootstrap.esm.min.js
--rw-r--r--   0 runner    (1001) docker     (127)   222455 2024-05-12 01:55:20.000000 meetlify-0.1.0/src/meetlify/themes/lindau/static/js/bootstrap.esm.min.js.map
--rw-r--r--   0 runner    (1001) docker     (127)   145401 2024-05-12 01:55:20.000000 meetlify-0.1.0/src/meetlify/themes/lindau/static/js/bootstrap.js
--rw-r--r--   0 runner    (1001) docker     (127)   306606 2024-05-12 01:55:20.000000 meetlify-0.1.0/src/meetlify/themes/lindau/static/js/bootstrap.js.map
--rw-r--r--   0 runner    (1001) docker     (127)    60635 2024-05-12 01:55:20.000000 meetlify-0.1.0/src/meetlify/themes/lindau/static/js/bootstrap.min.js
--rw-r--r--   0 runner    (1001) docker     (127)   220561 2024-05-12 01:55:20.000000 meetlify-0.1.0/src/meetlify/themes/lindau/static/js/bootstrap.min.js.map
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-05-12 01:55:20.000000 meetlify-0.1.0/src/meetlify/themes/lindau/static/js/scripts.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 01:55:28.965754 meetlify-0.1.0/src/meetlify/themes/lindau/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     4164 2024-05-12 01:55:20.000000 meetlify-0.1.0/src/meetlify/themes/lindau/templates/404.html
--rw-r--r--   0 runner    (1001) docker     (127)     3138 2024-05-12 01:55:20.000000 meetlify-0.1.0/src/meetlify/themes/lindau/templates/base.html
--rw-r--r--   0 runner    (1001) docker     (127)     4991 2024-05-12 01:55:20.000000 meetlify-0.1.0/src/meetlify/themes/lindau/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-05-12 01:55:20.000000 meetlify-0.1.0/src/meetlify/themes/lindau/templates/meetup.html
--rw-r--r--   0 runner    (1001) docker     (127)     3785 2024-05-12 01:55:20.000000 meetlify-0.1.0/src/meetlify/themes/lindau/templates/meetups.html
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-12 01:55:20.000000 meetlify-0.1.0/src/meetlify/themes/lindau/templates/page.html
--rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-05-12 01:55:20.000000 meetlify-0.1.0/src/meetlify/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 01:55:28.965754 meetlify-0.1.0/src/meetlify.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6355 2024-05-12 01:55:28.000000 meetlify-0.1.0/src/meetlify.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4517 2024-05-12 01:55:28.000000 meetlify-0.1.0/src/meetlify.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 01:55:28.000000 meetlify-0.1.0/src/meetlify.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-12 01:55:28.000000 meetlify-0.1.0/src/meetlify.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 01:55:28.000000 meetlify-0.1.0/src/meetlify.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-12 01:55:28.000000 meetlify-0.1.0/src/meetlify.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-12 01:55:28.000000 meetlify-0.1.0/src/meetlify.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 01:55:28.965754 meetlify-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-05-12 01:55:20.000000 meetlify-0.1.0/tests/test_meetups.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:13:27.374513 meetlify-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-12 02:13:19.000000 meetlify-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-12 02:13:19.000000 meetlify-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6353 2024-05-12 02:13:27.374513 meetlify-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-05-12 02:13:19.000000 meetlify-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-12 02:13:19.000000 meetlify-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-12 02:13:27.374513 meetlify-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4746 2024-05-12 02:13:19.000000 meetlify-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:13:27.342513 meetlify-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:13:27.346513 meetlify-0.1.1/src/meetlify/
+-rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-05-12 02:13:19.000000 meetlify-0.1.1/src/meetlify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9154 2024-05-12 02:13:19.000000 meetlify-0.1.1/src/meetlify/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3149 2024-05-12 02:13:19.000000 meetlify-0.1.1/src/meetlify/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3517 2024-05-12 02:13:19.000000 meetlify-0.1.1/src/meetlify/configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-05-12 02:13:19.000000 meetlify-0.1.1/src/meetlify/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3005 2024-05-12 02:13:19.000000 meetlify-0.1.1/src/meetlify/meetup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-05-12 02:13:19.000000 meetlify-0.1.1/src/meetlify/page.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:13:27.346513 meetlify-0.1.1/src/meetlify/share/
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-12 02:13:19.000000 meetlify-0.1.1/src/meetlify/share/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-12 02:13:19.000000 meetlify-0.1.1/src/meetlify/share/configs.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:13:27.342513 meetlify-0.1.1/src/meetlify/share/content/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:13:27.346513 meetlify-0.1.1/src/meetlify/share/content/images/
+-rw-r--r--   0 runner    (1001) docker     (127)   128599 2024-05-12 02:13:19.000000 meetlify-0.1.1/src/meetlify/share/content/images/fatureimage.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:13:27.346513 meetlify-0.1.1/src/meetlify/share/content/meetups/
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-12 02:13:19.000000 meetlify-0.1.1/src/meetlify/share/content/meetups/0001.md
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-12 02:13:19.000000 meetlify-0.1.1/src/meetlify/share/content/meetups/0002.md
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-12 02:13:19.000000 meetlify-0.1.1/src/meetlify/share/content/meetups/0003.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:13:27.350513 meetlify-0.1.1/src/meetlify/share/content/pages/
+-rw-r--r--   0 runner    (1001) docker     (127)     3984 2024-05-12 02:13:19.000000 meetlify-0.1.1/src/meetlify/share/content/pages/contact.md
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-12 02:13:19.000000 meetlify-0.1.1/src/meetlify/share/content/pages/home.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3915 2024-05-12 02:13:19.000000 meetlify-0.1.1/src/meetlify/share/content/pages/privacy.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-05-12 02:13:19.000000 meetlify-0.1.1/src/meetlify/share/content/pages/terms.md
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-12 02:13:19.000000 meetlify-0.1.1/src/meetlify/share/robots.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:13:27.342513 meetlify-0.1.1/src/meetlify/themes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:13:27.342513 meetlify-0.1.1/src/meetlify/themes/lindau/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:13:27.342513 meetlify-0.1.1/src/meetlify/themes/lindau/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:13:27.350513 meetlify-0.1.1/src/meetlify/themes/lindau/static/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)   362926 2024-05-12 02:13:19.000000 meetlify-0.1.1/src/meetlify/themes/lindau/static/assets/about.png
+-rw-r--r--   0 runner    (1001) docker     (127)    50969 2024-05-12 02:13:19.000000 meetlify-0.1.1/src/meetlify/themes/lindau/static/assets/author.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10126 2024-05-12 02:13:19.000000 meetlify-0.1.1/src/meetlify/themes/lindau/static/assets/banner.png
+-rw-r--r--   0 runner    (1001) docker     (127)    22993 2024-05-12 02:13:19.000000 meetlify-0.1.1/src/meetlify/themes/lindau/static/assets/favicon.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9139 2024-05-12 02:13:19.000000 meetlify-0.1.1/src/meetlify/themes/lindau/static/assets/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:13:27.362513 meetlify-0.1.1/src/meetlify/themes/lindau/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)    70329 2024-05-12 02:13:19.000000 meetlify-0.1.1/src/meetlify/themes/lindau/static/css/bootstrap-grid.css
+-rw-r--r--   0 runner    (1001) docker     (127)   203221 2024-05-12 02:13:19.000000 meetlify-0.1.1/src/meetlify/themes/lindau/static/css/bootstrap-grid.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)    51795 2024-05-12 02:13:19.000000 meetlify-0.1.1/src/meetlify/themes/lindau/static/css/bootstrap-grid.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)   115986 2024-05-12 02:13:19.000000 meetlify-0.1.1/src/meetlify/themes/lindau/static/css/bootstrap-grid.min.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)    70403 2024-05-12 02:13:19.000000 meetlify-0.1.1/src/meetlify/themes/lindau/static/css/bootstrap-grid.rtl.css
+-rw-r--r--   0 runner    (1001) docker     (127)   203225 2024-05-12 02:13:19.000000 meetlify-0.1.1/src/meetlify/themes/lindau/static/css/bootstrap-grid.rtl.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)    51870 2024-05-12 02:13:19.000000 meetlify-0.1.1/src/meetlify/themes/lindau/static/css/bootstrap-grid.rtl.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)   116063 2024-05-12 02:13:19.000000 meetlify-0.1.1/src/meetlify/themes/lindau/static/css/bootstrap-grid.rtl.min.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)    65696 2024-05-12 02:13:19.000000 meetlify-0.1.1/src/meetlify/themes/lindau/static/css/bootstrap-icons.css
+-rw-r--r--   0 runner    (1001) docker     (127)    12065 2024-05-12 02:13:19.000000 meetlify-0.1.1/src/meetlify/themes/lindau/static/css/bootstrap-reboot.css
+-rw-r--r--   0 runner    (1001) docker     (127)   129371 2024-05-12 02:13:19.000000 meetlify-0.1.1/src/meetlify/themes/lindau/static/css/bootstrap-reboot.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)    10126 2024-05-12 02:13:19.000000 meetlify-0.1.1/src/meetlify/themes/lindau/static/css/bootstrap-reboot.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)    51369 2024-05-12 02:13:19.000000 meetlify-0.1.1/src/meetlify/themes/lindau/static/css/bootstrap-reboot.min.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)    12058 2024-05-12 02:13:19.000000 meetlify-0.1.1/src/meetlify/themes/lindau/static/css/bootstrap-reboot.rtl.css
+-rw-r--r--   0 runner    (1001) docker     (127)   129386 2024-05-12 02:13:19.000000 meetlify-0.1.1/src/meetlify/themes/lindau/static/css/bootstrap-reboot.rtl.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)    10198 2024-05-12 02:13:19.000000 meetlify-0.1.1/src/meetlify/themes/lindau/static/css/bootstrap-reboot.rtl.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)    63943 2024-05-12 02:13:19.000000 meetlify-0.1.1/src/meetlify/themes/lindau/static/css/bootstrap-reboot.rtl.min.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)   107823 2024-05-12 02:13:19.000000 meetlify-0.1.1/src/meetlify/themes/lindau/static/css/bootstrap-utilities.css
+-rw-r--r--   0 runner    (1001) docker     (127)   267535 2024-05-12 02:13:19.000000 meetlify-0.1.1/src/meetlify/themes/lindau/static/css/bootstrap-utilities.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)    85352 2024-05-12 02:13:19.000000 meetlify-0.1.1/src/meetlify/themes/lindau/static/css/bootstrap-utilities.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)   180381 2024-05-12 02:13:19.000000 meetlify-0.1.1/src/meetlify/themes/lindau/static/css/bootstrap-utilities.min.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)   107691 2024-05-12 02:13:19.000000 meetlify-0.1.1/src/meetlify/themes/lindau/static/css/bootstrap-utilities.rtl.css
+-rw-r--r--   0 runner    (1001) docker     (127)   267476 2024-05-12 02:13:19.000000 meetlify-0.1.1/src/meetlify/themes/lindau/static/css/bootstrap-utilities.rtl.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)    85281 2024-05-12 02:13:19.000000 meetlify-0.1.1/src/meetlify/themes/lindau/static/css/bootstrap-utilities.rtl.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)   180217 2024-05-12 02:13:19.000000 meetlify-0.1.1/src/meetlify/themes/lindau/static/css/bootstrap-utilities.rtl.min.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)   281046 2024-05-12 02:13:19.000000 meetlify-0.1.1/src/meetlify/themes/lindau/static/css/bootstrap.css
+-rw-r--r--   0 runner    (1001) docker     (127)   679755 2024-05-12 02:13:19.000000 meetlify-0.1.1/src/meetlify/themes/lindau/static/css/bootstrap.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)   232803 2024-05-12 02:13:19.000000 meetlify-0.1.1/src/meetlify/themes/lindau/static/css/bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)   589892 2024-05-12 02:13:19.000000 meetlify-0.1.1/src/meetlify/themes/lindau/static/css/bootstrap.min.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)   280259 2024-05-12 02:13:19.000000 meetlify-0.1.1/src/meetlify/themes/lindau/static/css/bootstrap.rtl.css
+-rw-r--r--   0 runner    (1001) docker     (127)   679615 2024-05-12 02:13:19.000000 meetlify-0.1.1/src/meetlify/themes/lindau/static/css/bootstrap.rtl.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)   232911 2024-05-12 02:13:19.000000 meetlify-0.1.1/src/meetlify/themes/lindau/static/css/bootstrap.rtl.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)   589087 2024-05-12 02:13:19.000000 meetlify-0.1.1/src/meetlify/themes/lindau/static/css/bootstrap.rtl.min.css.map
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:13:27.362513 meetlify-0.1.1/src/meetlify/themes/lindau/static/css/fonts/
+-rw-r--r--   0 runner    (1001) docker     (127)   113656 2024-05-12 02:13:19.000000 meetlify-0.1.1/src/meetlify/themes/lindau/static/css/fonts/bootstrap-icons.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    85044 2024-05-12 02:13:19.000000 meetlify-0.1.1/src/meetlify/themes/lindau/static/css/fonts/bootstrap-icons.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)   237143 2024-05-12 02:13:19.000000 meetlify-0.1.1/src/meetlify/themes/lindau/static/css/styles.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:13:27.370513 meetlify-0.1.1/src/meetlify/themes/lindau/static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)   207819 2024-05-12 02:13:19.000000 meetlify-0.1.1/src/meetlify/themes/lindau/static/js/bootstrap.bundle.js
+-rw-r--r--   0 runner    (1001) docker     (127)   444579 2024-05-12 02:13:19.000000 meetlify-0.1.1/src/meetlify/themes/lindau/static/js/bootstrap.bundle.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)    80721 2024-05-12 02:13:19.000000 meetlify-0.1.1/src/meetlify/themes/lindau/static/js/bootstrap.bundle.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)   332090 2024-05-12 02:13:19.000000 meetlify-0.1.1/src/meetlify/themes/lindau/static/js/bootstrap.bundle.min.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)   135829 2024-05-12 02:13:19.000000 meetlify-0.1.1/src/meetlify/themes/lindau/static/js/bootstrap.esm.js
+-rw-r--r--   0 runner    (1001) docker     (127)   305438 2024-05-12 02:13:19.000000 meetlify-0.1.1/src/meetlify/themes/lindau/static/js/bootstrap.esm.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)    73935 2024-05-12 02:13:19.000000 meetlify-0.1.1/src/meetlify/themes/lindau/static/js/bootstrap.esm.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)   222455 2024-05-12 02:13:19.000000 meetlify-0.1.1/src/meetlify/themes/lindau/static/js/bootstrap.esm.min.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)   145401 2024-05-12 02:13:19.000000 meetlify-0.1.1/src/meetlify/themes/lindau/static/js/bootstrap.js
+-rw-r--r--   0 runner    (1001) docker     (127)   306606 2024-05-12 02:13:19.000000 meetlify-0.1.1/src/meetlify/themes/lindau/static/js/bootstrap.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)    60635 2024-05-12 02:13:19.000000 meetlify-0.1.1/src/meetlify/themes/lindau/static/js/bootstrap.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)   220561 2024-05-12 02:13:19.000000 meetlify-0.1.1/src/meetlify/themes/lindau/static/js/bootstrap.min.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-05-12 02:13:19.000000 meetlify-0.1.1/src/meetlify/themes/lindau/static/js/scripts.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:13:27.370513 meetlify-0.1.1/src/meetlify/themes/lindau/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     4164 2024-05-12 02:13:19.000000 meetlify-0.1.1/src/meetlify/themes/lindau/templates/404.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3142 2024-05-12 02:13:19.000000 meetlify-0.1.1/src/meetlify/themes/lindau/templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4991 2024-05-12 02:13:19.000000 meetlify-0.1.1/src/meetlify/themes/lindau/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-05-12 02:13:19.000000 meetlify-0.1.1/src/meetlify/themes/lindau/templates/meetup.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3785 2024-05-12 02:13:19.000000 meetlify-0.1.1/src/meetlify/themes/lindau/templates/meetups.html
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-12 02:13:19.000000 meetlify-0.1.1/src/meetlify/themes/lindau/templates/page.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-05-12 02:13:19.000000 meetlify-0.1.1/src/meetlify/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:13:27.370513 meetlify-0.1.1/src/meetlify.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6353 2024-05-12 02:13:27.000000 meetlify-0.1.1/src/meetlify.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4517 2024-05-12 02:13:27.000000 meetlify-0.1.1/src/meetlify.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 02:13:27.000000 meetlify-0.1.1/src/meetlify.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-12 02:13:27.000000 meetlify-0.1.1/src/meetlify.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 02:13:27.000000 meetlify-0.1.1/src/meetlify.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-12 02:13:27.000000 meetlify-0.1.1/src/meetlify.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-12 02:13:27.000000 meetlify-0.1.1/src/meetlify.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:13:27.370513 meetlify-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-05-12 02:13:19.000000 meetlify-0.1.1/tests/test_meetups.py
```

### Comparing `meetlify-0.1.0/LICENSE` & `meetlify-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.0/PKG-INFO` & `meetlify-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: meetlify
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python Package to Generate Meetup Websites
 Home-page: https://github.com/pybodensee/meetlify
-Download-URL: https://github.com/pybodensee/meetlify/releases/v0.1.0.tar.gz
+Download-URL: https://github.com/pybodensee/meetlify/releases/v0.1.1.tar.gz
 Author: Faisal Shahzad
 Author-email: pybodensee@gmail.com
 License: MIT
 Keywords: meetups,static-site-generators,seo,python
 Classifier: Development Status :: 1 - Planning
 Classifier: Environment :: Console
 Classifier: Environment :: X11 Applications
@@ -53,25 +53,25 @@
 Requires-Dist: twine; extra == "dev"
 Requires-Dist: wheel; extra == "dev"
 Requires-Dist: mkdocs; extra == "dev"
 Requires-Dist: mkdocs-gen-files; extra == "dev"
 Requires-Dist: mkdocstrings[python]; extra == "dev"
 Requires-Dist: pymdown-extensions; extra == "dev"
 Provides-Extra: all
-Requires-Dist: python-language-server[all]; extra == "all"
-Requires-Dist: mkdocstrings[python]; extra == "all"
 Requires-Dist: mkdocs; extra == "all"
-Requires-Dist: pytest; extra == "all"
-Requires-Dist: mkdocs-gen-files; extra == "all"
-Requires-Dist: twine; extra == "all"
+Requires-Dist: wheel; extra == "all"
+Requires-Dist: pymdown-extensions; extra == "all"
 Requires-Dist: black; extra == "all"
 Requires-Dist: setuptools; extra == "all"
+Requires-Dist: pytest; extra == "all"
+Requires-Dist: python-language-server[all]; extra == "all"
 Requires-Dist: pytest-cov; extra == "all"
-Requires-Dist: pymdown-extensions; extra == "all"
-Requires-Dist: wheel; extra == "all"
+Requires-Dist: mkdocs-gen-files; extra == "all"
+Requires-Dist: twine; extra == "all"
+Requires-Dist: mkdocstrings[python]; extra == "all"
 
 # meetlify
 
 Python based Static Site Genrators for Meetups/Meetup Webites.
 
 [![license](https://img.shields.io/pypi/l/meetlify.svg?style=flat-square "Project License: MIT")](https://github.com/pybodensee/meetlify/blob/master/LICENSE)
 [![status](https://img.shields.io/pypi/status/meetlify.svg?style=flat-square "Project Development Status")](https://github.com/pybodensee/meetlify/milestone/1)
@@ -130,8 +130,8 @@
 
 ## Contribute
 
 Pull Requests, Feature Suggestions, and collaborations are welcome.
 
 ## About Us
 
-This work is a collaborative effort of [PyBodensee](https://pybodensee.com/), and [pybodensee](https://pybodensee.com/).
+This work is a collaborative effort of [PyBodensee](https://pybodensee.com/), and [SerpWings](https://serpwings.com/).
```

### Comparing `meetlify-0.1.0/README.md` & `meetlify-0.1.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -59,8 +59,8 @@
 
 ## Contribute
 
 Pull Requests, Feature Suggestions, and collaborations are welcome.
 
 ## About Us
 
-This work is a collaborative effort of [PyBodensee](https://pybodensee.com/), and [pybodensee](https://pybodensee.com/).
+This work is a collaborative effort of [PyBodensee](https://pybodensee.com/), and [SerpWings](https://serpwings.com/).
```

### Comparing `meetlify-0.1.0/setup.py` & `meetlify-0.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.0/src/meetlify/__init__.py` & `meetlify-0.1.1/src/meetlify/__init__.py`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.0/src/meetlify/api.py` & `meetlify-0.1.1/src/meetlify/api.py`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.0/src/meetlify/cli.py` & `meetlify-0.1.1/src/meetlify/cli.py`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.0/src/meetlify/configs.py` & `meetlify-0.1.1/src/meetlify/configs.py`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.0/src/meetlify/constants.py` & `meetlify-0.1.1/src/meetlify/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,10 +33,10 @@
 
 # +++++++++++++++++++++++++++++++++++++++++++++++++++++
 # DATABASE/CONSTANTS LIST
 # +++++++++++++++++++++++++++++++++++++++++++++++++++++
 
 VERSION_MAJOR = 0
 VERSION_MINOR = 1
-VERSION_REVISION = 0
+VERSION_REVISION = 1
 
 FULL_VERSION = f"{VERSION_MAJOR}.{VERSION_MINOR}.{VERSION_REVISION}"
```

### Comparing `meetlify-0.1.0/src/meetlify/meetup.py` & `meetlify-0.1.1/src/meetlify/meetup.py`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.0/src/meetlify/page.py` & `meetlify-0.1.1/src/meetlify/page.py`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.0/src/meetlify/share/__init__.py` & `meetlify-0.1.1/src/meetlify/share/__init__.py`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.0/src/meetlify/share/configs.json` & `meetlify-0.1.1/src/meetlify/share/configs.json`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.0/src/meetlify/share/content/images/fatureimage.png` & `meetlify-0.1.1/src/meetlify/share/content/images/fatureimage.png`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.0/src/meetlify/share/content/meetups/0001.md` & `meetlify-0.1.1/src/meetlify/share/content/meetups/0001.md`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.0/src/meetlify/share/content/meetups/0002.md` & `meetlify-0.1.1/src/meetlify/share/content/meetups/0002.md`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.0/src/meetlify/share/content/meetups/0003.md` & `meetlify-0.1.1/src/meetlify/share/content/meetups/0003.md`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.0/src/meetlify/share/content/pages/contact.md` & `meetlify-0.1.1/src/meetlify/share/content/pages/contact.md`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.0/src/meetlify/share/content/pages/home.md` & `meetlify-0.1.1/src/meetlify/share/content/pages/home.md`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.0/src/meetlify/share/content/pages/privacy.md` & `meetlify-0.1.1/src/meetlify/share/content/pages/privacy.md`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.0/src/meetlify/share/content/pages/terms.md` & `meetlify-0.1.1/src/meetlify/share/content/pages/terms.md`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.0/src/meetlify/themes/lindau/static/assets/about.png` & `meetlify-0.1.1/src/meetlify/themes/lindau/static/assets/about.png`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.0/src/meetlify/themes/lindau/static/assets/author.png` & `meetlify-0.1.1/src/meetlify/themes/lindau/static/assets/author.png`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.0/src/meetlify/themes/lindau/static/assets/banner.png` & `meetlify-0.1.1/src/meetlify/themes/lindau/static/assets/banner.png`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.0/src/meetlify/themes/lindau/static/assets/favicon.png` & `meetlify-0.1.1/src/meetlify/themes/lindau/static/assets/favicon.png`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.0/src/meetlify/themes/lindau/static/assets/logo.png` & `meetlify-0.1.1/src/meetlify/themes/lindau/static/assets/logo.png`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.0/src/meetlify/themes/lindau/static/css/bootstrap-grid.css` & `meetlify-0.1.1/src/meetlify/themes/lindau/static/css/bootstrap-grid.css`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.0/src/meetlify/themes/lindau/static/css/bootstrap-grid.css.map` & `meetlify-0.1.1/src/meetlify/themes/lindau/static/css/bootstrap-grid.css.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.0/src/meetlify/themes/lindau/static/css/bootstrap-grid.min.css` & `meetlify-0.1.1/src/meetlify/themes/lindau/static/css/bootstrap-grid.min.css`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.0/src/meetlify/themes/lindau/static/css/bootstrap-grid.min.css.map` & `meetlify-0.1.1/src/meetlify/themes/lindau/static/css/bootstrap-grid.min.css.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.0/src/meetlify/themes/lindau/static/css/bootstrap-grid.rtl.css` & `meetlify-0.1.1/src/meetlify/themes/lindau/static/css/bootstrap-grid.rtl.css`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.0/src/meetlify/themes/lindau/static/css/bootstrap-grid.rtl.css.map` & `meetlify-0.1.1/src/meetlify/themes/lindau/static/css/bootstrap-grid.rtl.css.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.0/src/meetlify/themes/lindau/static/css/bootstrap-grid.rtl.min.css` & `meetlify-0.1.1/src/meetlify/themes/lindau/static/css/bootstrap-grid.rtl.min.css`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.0/src/meetlify/themes/lindau/static/css/bootstrap-grid.rtl.min.css.map` & `meetlify-0.1.1/src/meetlify/themes/lindau/static/css/bootstrap-grid.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.0/src/meetlify/themes/lindau/static/css/bootstrap-icons.css` & `meetlify-0.1.1/src/meetlify/themes/lindau/static/css/bootstrap-icons.css`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.0/src/meetlify/themes/lindau/static/css/bootstrap-reboot.css` & `meetlify-0.1.1/src/meetlify/themes/lindau/static/css/bootstrap-reboot.css`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.0/src/meetlify/themes/lindau/static/css/bootstrap-reboot.css.map` & `meetlify-0.1.1/src/meetlify/themes/lindau/static/css/bootstrap-reboot.css.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.0/src/meetlify/themes/lindau/static/css/bootstrap-reboot.min.css` & `meetlify-0.1.1/src/meetlify/themes/lindau/static/css/bootstrap-reboot.min.css`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.0/src/meetlify/themes/lindau/static/css/bootstrap-reboot.min.css.map` & `meetlify-0.1.1/src/meetlify/themes/lindau/static/css/bootstrap-reboot.min.css.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.0/src/meetlify/themes/lindau/static/css/bootstrap-reboot.rtl.css` & `meetlify-0.1.1/src/meetlify/themes/lindau/static/css/bootstrap-reboot.rtl.css`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.0/src/meetlify/themes/lindau/static/css/bootstrap-reboot.rtl.css.map` & `meetlify-0.1.1/src/meetlify/themes/lindau/static/css/bootstrap-reboot.rtl.css.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.0/src/meetlify/themes/lindau/static/css/bootstrap-reboot.rtl.min.css` & `meetlify-0.1.1/src/meetlify/themes/lindau/static/css/bootstrap-reboot.rtl.min.css`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.0/src/meetlify/themes/lindau/static/css/bootstrap-reboot.rtl.min.css.map` & `meetlify-0.1.1/src/meetlify/themes/lindau/static/css/bootstrap-reboot.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.0/src/meetlify/themes/lindau/static/css/bootstrap-utilities.css` & `meetlify-0.1.1/src/meetlify/themes/lindau/static/css/bootstrap-utilities.css`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.0/src/meetlify/themes/lindau/static/css/bootstrap-utilities.css.map` & `meetlify-0.1.1/src/meetlify/themes/lindau/static/css/bootstrap-utilities.css.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.0/src/meetlify/themes/lindau/static/css/bootstrap-utilities.min.css` & `meetlify-0.1.1/src/meetlify/themes/lindau/static/css/bootstrap-utilities.min.css`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.0/src/meetlify/themes/lindau/static/css/bootstrap-utilities.min.css.map` & `meetlify-0.1.1/src/meetlify/themes/lindau/static/css/bootstrap-utilities.min.css.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.0/src/meetlify/themes/lindau/static/css/bootstrap-utilities.rtl.css` & `meetlify-0.1.1/src/meetlify/themes/lindau/static/css/bootstrap-utilities.rtl.css`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.0/src/meetlify/themes/lindau/static/css/bootstrap-utilities.rtl.css.map` & `meetlify-0.1.1/src/meetlify/themes/lindau/static/css/bootstrap-utilities.rtl.css.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.0/src/meetlify/themes/lindau/static/css/bootstrap-utilities.rtl.min.css` & `meetlify-0.1.1/src/meetlify/themes/lindau/static/css/bootstrap-utilities.rtl.min.css`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.0/src/meetlify/themes/lindau/static/css/bootstrap-utilities.rtl.min.css.map` & `meetlify-0.1.1/src/meetlify/themes/lindau/static/css/bootstrap-utilities.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.0/src/meetlify/themes/lindau/static/css/bootstrap.css` & `meetlify-0.1.1/src/meetlify/themes/lindau/static/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.0/src/meetlify/themes/lindau/static/css/bootstrap.css.map` & `meetlify-0.1.1/src/meetlify/themes/lindau/static/css/bootstrap.css.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.0/src/meetlify/themes/lindau/static/css/bootstrap.min.css` & `meetlify-0.1.1/src/meetlify/themes/lindau/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.0/src/meetlify/themes/lindau/static/css/bootstrap.min.css.map` & `meetlify-0.1.1/src/meetlify/themes/lindau/static/css/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.0/src/meetlify/themes/lindau/static/css/bootstrap.rtl.css` & `meetlify-0.1.1/src/meetlify/themes/lindau/static/css/bootstrap.rtl.css`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.0/src/meetlify/themes/lindau/static/css/bootstrap.rtl.css.map` & `meetlify-0.1.1/src/meetlify/themes/lindau/static/css/bootstrap.rtl.css.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.0/src/meetlify/themes/lindau/static/css/bootstrap.rtl.min.css` & `meetlify-0.1.1/src/meetlify/themes/lindau/static/css/bootstrap.rtl.min.css`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.0/src/meetlify/themes/lindau/static/css/bootstrap.rtl.min.css.map` & `meetlify-0.1.1/src/meetlify/themes/lindau/static/css/bootstrap.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.0/src/meetlify/themes/lindau/static/css/fonts/bootstrap-icons.woff` & `meetlify-0.1.1/src/meetlify/themes/lindau/static/css/fonts/bootstrap-icons.woff`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.0/src/meetlify/themes/lindau/static/css/fonts/bootstrap-icons.woff2` & `meetlify-0.1.1/src/meetlify/themes/lindau/static/css/fonts/bootstrap-icons.woff2`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.0/src/meetlify/themes/lindau/static/css/styles.css` & `meetlify-0.1.1/src/meetlify/themes/lindau/static/css/styles.css`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.0/src/meetlify/themes/lindau/static/js/bootstrap.bundle.js` & `meetlify-0.1.1/src/meetlify/themes/lindau/static/js/bootstrap.bundle.js`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.0/src/meetlify/themes/lindau/static/js/bootstrap.bundle.js.map` & `meetlify-0.1.1/src/meetlify/themes/lindau/static/js/bootstrap.bundle.js.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.0/src/meetlify/themes/lindau/static/js/bootstrap.bundle.min.js` & `meetlify-0.1.1/src/meetlify/themes/lindau/static/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.0/src/meetlify/themes/lindau/static/js/bootstrap.bundle.min.js.map` & `meetlify-0.1.1/src/meetlify/themes/lindau/static/js/bootstrap.bundle.min.js.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.0/src/meetlify/themes/lindau/static/js/bootstrap.esm.js` & `meetlify-0.1.1/src/meetlify/themes/lindau/static/js/bootstrap.esm.js`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.0/src/meetlify/themes/lindau/static/js/bootstrap.esm.js.map` & `meetlify-0.1.1/src/meetlify/themes/lindau/static/js/bootstrap.esm.js.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.0/src/meetlify/themes/lindau/static/js/bootstrap.esm.min.js` & `meetlify-0.1.1/src/meetlify/themes/lindau/static/js/bootstrap.esm.min.js`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.0/src/meetlify/themes/lindau/static/js/bootstrap.esm.min.js.map` & `meetlify-0.1.1/src/meetlify/themes/lindau/static/js/bootstrap.esm.min.js.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.0/src/meetlify/themes/lindau/static/js/bootstrap.js` & `meetlify-0.1.1/src/meetlify/themes/lindau/static/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.0/src/meetlify/themes/lindau/static/js/bootstrap.js.map` & `meetlify-0.1.1/src/meetlify/themes/lindau/static/js/bootstrap.js.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.0/src/meetlify/themes/lindau/static/js/bootstrap.min.js` & `meetlify-0.1.1/src/meetlify/themes/lindau/static/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.0/src/meetlify/themes/lindau/static/js/bootstrap.min.js.map` & `meetlify-0.1.1/src/meetlify/themes/lindau/static/js/bootstrap.min.js.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.0/src/meetlify/themes/lindau/static/js/scripts.js` & `meetlify-0.1.1/src/meetlify/themes/lindau/static/js/scripts.js`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.0/src/meetlify/themes/lindau/templates/404.html` & `meetlify-0.1.1/src/meetlify/themes/lindau/templates/404.html`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.0/src/meetlify/themes/lindau/templates/base.html` & `meetlify-0.1.1/src/meetlify/themes/lindau/templates/base.html`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 <body class="d-flex flex-column h-100">
     <main class="flex-shrink-0">
         <!-- Navigation-->
         <nav class="navbar navbar-expand-lg navbar-dark bg-dark">
             <div class="container px-5">
                 <a class="navbar-brand" href="/">
-                    <img src="{{meta.URL}}/static/assets/logo.webp" width="80.6" height="30"
+                    <img src="{{meta.URL}}/static/assets/{{meta.logo}}" width="80.6" height="30"
                         class="d-inline-block align-top" alt="{{meta.name}} Logo"></a>
 
                 <a class="navbar-brand" href="/">{{meta.name}}</a>
                 <button class="navbar-toggler" type="button" data-bs-toggle="collapse"
                     data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent"
                     aria-expanded="false" aria-label="Toggle navigation"><span
                         class="navbar-toggler-icon"></span></button>
```

### Comparing `meetlify-0.1.0/src/meetlify/themes/lindau/templates/index.html` & `meetlify-0.1.1/src/meetlify/themes/lindau/templates/index.html`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.0/src/meetlify/themes/lindau/templates/meetup.html` & `meetlify-0.1.1/src/meetlify/themes/lindau/templates/meetup.html`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.0/src/meetlify/themes/lindau/templates/meetups.html` & `meetlify-0.1.1/src/meetlify/themes/lindau/templates/meetups.html`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.0/src/meetlify/utils.py` & `meetlify-0.1.1/src/meetlify/utils.py`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.0/src/meetlify.egg-info/PKG-INFO` & `meetlify-0.1.1/src/meetlify.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: meetlify
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python Package to Generate Meetup Websites
 Home-page: https://github.com/pybodensee/meetlify
-Download-URL: https://github.com/pybodensee/meetlify/releases/v0.1.0.tar.gz
+Download-URL: https://github.com/pybodensee/meetlify/releases/v0.1.1.tar.gz
 Author: Faisal Shahzad
 Author-email: pybodensee@gmail.com
 License: MIT
 Keywords: meetups,static-site-generators,seo,python
 Classifier: Development Status :: 1 - Planning
 Classifier: Environment :: Console
 Classifier: Environment :: X11 Applications
@@ -53,25 +53,25 @@
 Requires-Dist: twine; extra == "dev"
 Requires-Dist: wheel; extra == "dev"
 Requires-Dist: mkdocs; extra == "dev"
 Requires-Dist: mkdocs-gen-files; extra == "dev"
 Requires-Dist: mkdocstrings[python]; extra == "dev"
 Requires-Dist: pymdown-extensions; extra == "dev"
 Provides-Extra: all
-Requires-Dist: python-language-server[all]; extra == "all"
-Requires-Dist: mkdocstrings[python]; extra == "all"
 Requires-Dist: mkdocs; extra == "all"
-Requires-Dist: pytest; extra == "all"
-Requires-Dist: mkdocs-gen-files; extra == "all"
-Requires-Dist: twine; extra == "all"
+Requires-Dist: wheel; extra == "all"
+Requires-Dist: pymdown-extensions; extra == "all"
 Requires-Dist: black; extra == "all"
 Requires-Dist: setuptools; extra == "all"
+Requires-Dist: pytest; extra == "all"
+Requires-Dist: python-language-server[all]; extra == "all"
 Requires-Dist: pytest-cov; extra == "all"
-Requires-Dist: pymdown-extensions; extra == "all"
-Requires-Dist: wheel; extra == "all"
+Requires-Dist: mkdocs-gen-files; extra == "all"
+Requires-Dist: twine; extra == "all"
+Requires-Dist: mkdocstrings[python]; extra == "all"
 
 # meetlify
 
 Python based Static Site Genrators for Meetups/Meetup Webites.
 
 [![license](https://img.shields.io/pypi/l/meetlify.svg?style=flat-square "Project License: MIT")](https://github.com/pybodensee/meetlify/blob/master/LICENSE)
 [![status](https://img.shields.io/pypi/status/meetlify.svg?style=flat-square "Project Development Status")](https://github.com/pybodensee/meetlify/milestone/1)
@@ -130,8 +130,8 @@
 
 ## Contribute
 
 Pull Requests, Feature Suggestions, and collaborations are welcome.
 
 ## About Us
 
-This work is a collaborative effort of [PyBodensee](https://pybodensee.com/), and [pybodensee](https://pybodensee.com/).
+This work is a collaborative effort of [PyBodensee](https://pybodensee.com/), and [SerpWings](https://serpwings.com/).
```

### Comparing `meetlify-0.1.0/src/meetlify.egg-info/SOURCES.txt` & `meetlify-0.1.1/src/meetlify.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.0/tests/test_meetups.py` & `meetlify-0.1.1/tests/test_meetups.py`

 * *Files identical despite different names*

