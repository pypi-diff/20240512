# Comparing `tmp/lolcatt-0.3.1.tar.gz` & `tmp/lolcatt-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lolcatt-0.3.1.tar", last modified: Sat May 11 16:47:28 2024, max compression
+gzip compressed data, was "lolcatt-0.4.1.tar", last modified: Sat May 11 20:54:52 2024, max compression
```

## Comparing `lolcatt-0.3.1.tar` & `lolcatt-0.4.1.tar`

### file list

```diff
@@ -1,163 +1,78 @@
-drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 16:47:28.289271 lolcatt-0.3.1/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1001)     1074 2023-07-23 10:21:40.000000 lolcatt-0.3.1/LICENSE
--rw-rw-r--   0 atav1st   (1000) atav1st   (1001)      239 2023-07-23 10:21:40.000000 lolcatt-0.3.1/MANIFEST.in
--rw-r--r--   0 atav1st   (1000) atav1st   (1001)     4312 2024-05-11 16:47:28.289271 lolcatt-0.3.1/PKG-INFO
--rw-rw-r--   0 atav1st   (1000) atav1st   (1001)     3504 2023-07-23 10:25:50.000000 lolcatt-0.3.1/README.rst
-drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 16:47:28.192604 lolcatt-0.3.1/docs/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1001)      608 2023-07-23 10:21:40.000000 lolcatt-0.3.1/docs/Makefile
-drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 16:47:28.145938 lolcatt-0.3.1/docs/_build/
-drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 16:47:28.145938 lolcatt-0.3.1/docs/_build/html/
-drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 16:47:28.209271 lolcatt-0.3.1/docs/_build/html/_static/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1001)    14813 2023-07-23 10:39:33.000000 lolcatt-0.3.1/docs/_build/html/_static/basic.css
--rw-rw-r--   0 atav1st   (1000) atav1st   (1001)       84 2023-07-23 10:21:40.000000 lolcatt-0.3.1/docs/_build/html/_static/custom.css
--rw-rw-r--   0 atav1st   (1000) atav1st   (1001)      286 2023-05-12 22:36:26.000000 lolcatt-0.3.1/docs/_build/html/_static/file.png
--rw-rw-r--   0 atav1st   (1000) atav1st   (1001)       90 2023-05-12 22:36:26.000000 lolcatt-0.3.1/docs/_build/html/_static/minus.png
--rw-rw-r--   0 atav1st   (1000) atav1st   (1001)     4208 2023-07-23 10:39:33.000000 lolcatt-0.3.1/docs/_build/html/_static/nature.css
--rw-rw-r--   0 atav1st   (1000) atav1st   (1001)       90 2023-05-12 22:36:26.000000 lolcatt-0.3.1/docs/_build/html/_static/plus.png
--rw-rw-r--   0 atav1st   (1000) atav1st   (1001)     4956 2023-07-23 10:39:33.000000 lolcatt-0.3.1/docs/_build/html/_static/pygments.css
--rw-rw-r--   0 atav1st   (1000) atav1st   (1001)    26168 2023-07-23 10:21:40.000000 lolcatt-0.3.1/docs/_build/html/_static/screenshot.png
-drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 16:47:28.212604 lolcatt-0.3.1/docs/_static/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1001)       84 2023-07-23 10:21:40.000000 lolcatt-0.3.1/docs/_static/custom.css
--rw-rw-r--   0 atav1st   (1000) atav1st   (1001)    26168 2023-07-23 10:21:40.000000 lolcatt-0.3.1/docs/_static/screenshot.png
--rw-rw-r--   0 atav1st   (1000) atav1st   (1001)     4983 2023-07-23 10:21:40.000000 lolcatt-0.3.1/docs/conf.py
--rw-rw-r--   0 atav1st   (1000) atav1st   (1001)      264 2023-07-23 10:21:40.000000 lolcatt-0.3.1/docs/index.rst
--rw-rw-r--   0 atav1st   (1000) atav1st   (1001)     1138 2023-07-23 10:21:40.000000 lolcatt-0.3.1/docs/installation.rst
--rw-rw-r--   0 atav1st   (1000) atav1st   (1001)      346 2023-07-23 10:21:40.000000 lolcatt-0.3.1/docs/lolcatt.casting.rst
--rw-rw-r--   0 atav1st   (1000) atav1st   (1001)      517 2023-07-23 10:39:30.000000 lolcatt-0.3.1/docs/lolcatt.rst
--rw-rw-r--   0 atav1st   (1000) atav1st   (1001)     1232 2023-07-23 10:21:40.000000 lolcatt-0.3.1/docs/lolcatt.ui.rst
--rw-rw-r--   0 atav1st   (1000) atav1st   (1001)      331 2023-07-23 10:21:40.000000 lolcatt-0.3.1/docs/lolcatt.utils.rst
--rw-rw-r--   0 atav1st   (1000) atav1st   (1001)      805 2023-07-23 10:21:40.000000 lolcatt-0.3.1/docs/make.bat
--rw-rw-r--   0 atav1st   (1000) atav1st   (1001)       58 2023-07-23 10:39:30.000000 lolcatt-0.3.1/docs/modules.rst
--rw-rw-r--   0 atav1st   (1000) atav1st   (1001)       27 2023-07-23 10:21:40.000000 lolcatt-0.3.1/docs/readme.rst
--rw-rw-r--   0 atav1st   (1000) atav1st   (1001)       69 2023-07-23 10:21:40.000000 lolcatt-0.3.1/docs/usage.rst
-drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 16:47:28.212604 lolcatt-0.3.1/lolcatt/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1001)       41 2023-07-16 00:01:30.000000 lolcatt-0.3.1/lolcatt/.githash
--rw-r--r--   0 atav1st   (1000) atav1st   (1001)      125 2024-05-11 16:44:59.000000 lolcatt-0.3.1/lolcatt/__init__.py
--rw-r--r--   0 atav1st   (1000) atav1st   (1001)     1378 2024-05-11 16:30:11.000000 lolcatt-0.3.1/lolcatt/app.py
-drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 16:47:28.215937 lolcatt-0.3.1/lolcatt/casting/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1001)        0 2023-07-23 10:21:40.000000 lolcatt-0.3.1/lolcatt/casting/__init__.py
--rw-rw-r--   0 atav1st   (1000) atav1st   (1001)    10035 2023-10-29 15:57:12.000000 lolcatt-0.3.1/lolcatt/casting/caster.py
--rw-rw-r--   0 atav1st   (1000) atav1st   (1001)     1336 2023-10-29 15:57:47.000000 lolcatt-0.3.1/lolcatt/casting/youtube_playlist_handler.py
--rw-r--r--   0 atav1st   (1000) atav1st   (1001)     1827 2024-05-11 16:41:39.000000 lolcatt-0.3.1/lolcatt/cli.py
-drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 16:47:28.219271 lolcatt-0.3.1/lolcatt/ui/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1001)        0 2023-07-23 10:21:40.000000 lolcatt-0.3.1/lolcatt/ui/__init__.py
--rw-r--r--   0 atav1st   (1000) atav1st   (1001)     1579 2024-05-11 16:30:11.000000 lolcatt-0.3.1/lolcatt/ui/lolcatt.css
--rw-rw-r--   0 atav1st   (1000) atav1st   (1001)     4860 2023-10-29 15:57:12.000000 lolcatt-0.3.1/lolcatt/ui/lolcatt_controls.py
--rw-rw-r--   0 atav1st   (1000) atav1st   (1001)     1265 2023-07-23 10:25:25.000000 lolcatt-0.3.1/lolcatt/ui/lolcatt_device_info.py
--rw-r--r--   0 atav1st   (1000) atav1st   (1001)     1640 2024-05-11 16:30:11.000000 lolcatt-0.3.1/lolcatt/ui/lolcatt_playback_info.py
--rw-rw-r--   0 atav1st   (1000) atav1st   (1001)     3068 2023-07-23 10:25:50.000000 lolcatt-0.3.1/lolcatt/ui/lolcatt_progress.py
--rw-rw-r--   0 atav1st   (1000) atav1st   (1001)     3016 2023-10-29 15:57:12.000000 lolcatt-0.3.1/lolcatt/ui/lolcatt_url_input.py
-drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 16:47:28.219271 lolcatt-0.3.1/lolcatt/utils/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1001)        0 2023-07-23 10:21:40.000000 lolcatt-0.3.1/lolcatt/utils/__init__.py
--rw-rw-r--   0 atav1st   (1000) atav1st   (1001)     2422 2023-10-29 15:57:52.000000 lolcatt-0.3.1/lolcatt/utils/utils.py
-drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 16:47:28.289271 lolcatt-0.3.1/lolcatt.egg-info/
--rw-r--r--   0 atav1st   (1000) atav1st   (1001)     4312 2024-05-11 16:47:27.000000 lolcatt-0.3.1/lolcatt.egg-info/PKG-INFO
--rw-r--r--   0 atav1st   (1000) atav1st   (1001)     5711 2024-05-11 16:47:28.000000 lolcatt-0.3.1/lolcatt.egg-info/SOURCES.txt
--rw-r--r--   0 atav1st   (1000) atav1st   (1001)        1 2024-05-11 16:47:27.000000 lolcatt-0.3.1/lolcatt.egg-info/dependency_links.txt
--rw-r--r--   0 atav1st   (1000) atav1st   (1001)       45 2024-05-11 16:47:27.000000 lolcatt-0.3.1/lolcatt.egg-info/entry_points.txt
--rw-r--r--   0 atav1st   (1000) atav1st   (1001)        1 2024-05-09 17:01:17.000000 lolcatt-0.3.1/lolcatt.egg-info/not-zip-safe
--rw-r--r--   0 atav1st   (1000) atav1st   (1001)       54 2024-05-11 16:47:27.000000 lolcatt-0.3.1/lolcatt.egg-info/requires.txt
--rw-r--r--   0 atav1st   (1000) atav1st   (1001)        8 2024-05-11 16:47:27.000000 lolcatt-0.3.1/lolcatt.egg-info/top_level.txt
--rw-r--r--   0 atav1st   (1000) atav1st   (1001)      559 2024-05-11 16:44:59.000000 lolcatt-0.3.1/pyproject.toml
--rw-r--r--   0 atav1st   (1000) atav1st   (1001)       38 2024-05-11 16:47:28.289271 lolcatt-0.3.1/setup.cfg
--rw-r--r--   0 atav1st   (1000) atav1st   (1001)     1556 2024-05-11 16:44:59.000000 lolcatt-0.3.1/setup.py
-drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 16:47:28.219271 lolcatt-0.3.1/tests/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1001)       37 2023-07-23 10:21:40.000000 lolcatt-0.3.1/tests/__init__.py
--rw-rw-r--   0 atav1st   (1000) atav1st   (1001)      211 2023-07-23 10:21:40.000000 lolcatt-0.3.1/tests/test_lolcatt.py
-drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 16:47:28.149271 lolcatt-0.3.1/venv/
-drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 16:47:28.149271 lolcatt-0.3.1/venv/lib/
-drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 16:47:28.149271 lolcatt-0.3.1/venv/lib/python3.10/
-drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 16:47:28.149271 lolcatt-0.3.1/venv/lib/python3.10/site-packages/
-drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 16:47:28.149271 lolcatt-0.3.1/venv/lib/python3.10/site-packages/docutils/
-drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 16:47:28.149271 lolcatt-0.3.1/venv/lib/python3.10/site-packages/docutils/writers/
-drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 16:47:28.222604 lolcatt-0.3.1/venv/lib/python3.10/site-packages/docutils/writers/html4css1/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1001)     7219 2023-07-16 15:28:55.000000 lolcatt-0.3.1/venv/lib/python3.10/site-packages/docutils/writers/html4css1/html4css1.css
-drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 16:47:28.249271 lolcatt-0.3.1/venv/lib/python3.10/site-packages/docutils/writers/html5_polyglot/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1001)     6261 2023-07-16 15:28:55.000000 lolcatt-0.3.1/venv/lib/python3.10/site-packages/docutils/writers/html5_polyglot/math.css
--rw-rw-r--   0 atav1st   (1000) atav1st   (1001)     7388 2023-07-16 15:28:55.000000 lolcatt-0.3.1/venv/lib/python3.10/site-packages/docutils/writers/html5_polyglot/minimal.css
--rw-rw-r--   0 atav1st   (1000) atav1st   (1001)     7749 2023-07-16 15:28:55.000000 lolcatt-0.3.1/venv/lib/python3.10/site-packages/docutils/writers/html5_polyglot/plain.css
--rw-rw-r--   0 atav1st   (1000) atav1st   (1001)    11895 2023-07-16 15:28:55.000000 lolcatt-0.3.1/venv/lib/python3.10/site-packages/docutils/writers/html5_polyglot/responsive.css
--rw-rw-r--   0 atav1st   (1000) atav1st   (1001)    12023 2023-07-16 15:28:55.000000 lolcatt-0.3.1/venv/lib/python3.10/site-packages/docutils/writers/html5_polyglot/tuftig.css
-drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 16:47:28.249271 lolcatt-0.3.1/venv/lib/python3.10/site-packages/docutils/writers/pep_html/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1001)     6367 2023-07-16 15:28:55.000000 lolcatt-0.3.1/venv/lib/python3.10/site-packages/docutils/writers/pep_html/pep.css
-drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 16:47:28.149271 lolcatt-0.3.1/venv/lib/python3.10/site-packages/docutils/writers/s5_html/
-drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 16:47:28.149271 lolcatt-0.3.1/venv/lib/python3.10/site-packages/docutils/writers/s5_html/themes/
-drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 16:47:28.252604 lolcatt-0.3.1/venv/lib/python3.10/site-packages/docutils/writers/s5_html/themes/big-black/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1001)      910 2023-07-16 15:28:55.000000 lolcatt-0.3.1/venv/lib/python3.10/site-packages/docutils/writers/s5_html/themes/big-black/framing.css
--rw-rw-r--   0 atav1st   (1000) atav1st   (1001)     3605 2023-07-16 15:28:55.000000 lolcatt-0.3.1/venv/lib/python3.10/site-packages/docutils/writers/s5_html/themes/big-black/pretty.css
-drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 16:47:28.255937 lolcatt-0.3.1/venv/lib/python3.10/site-packages/docutils/writers/s5_html/themes/big-white/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1001)      905 2023-07-16 15:28:55.000000 lolcatt-0.3.1/venv/lib/python3.10/site-packages/docutils/writers/s5_html/themes/big-white/framing.css
--rw-rw-r--   0 atav1st   (1000) atav1st   (1001)     3565 2023-07-16 15:28:55.000000 lolcatt-0.3.1/venv/lib/python3.10/site-packages/docutils/writers/s5_html/themes/big-white/pretty.css
-drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 16:47:28.262604 lolcatt-0.3.1/venv/lib/python3.10/site-packages/docutils/writers/s5_html/themes/default/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1001)     1002 2023-07-16 15:28:55.000000 lolcatt-0.3.1/venv/lib/python3.10/site-packages/docutils/writers/s5_html/themes/default/framing.css
--rw-rw-r--   0 atav1st   (1000) atav1st   (1001)      261 2023-07-16 15:28:55.000000 lolcatt-0.3.1/venv/lib/python3.10/site-packages/docutils/writers/s5_html/themes/default/opera.css
--rw-rw-r--   0 atav1st   (1000) atav1st   (1001)      648 2023-07-16 15:28:55.000000 lolcatt-0.3.1/venv/lib/python3.10/site-packages/docutils/writers/s5_html/themes/default/outline.css
--rw-rw-r--   0 atav1st   (1000) atav1st   (1001)     4383 2023-07-16 15:28:55.000000 lolcatt-0.3.1/venv/lib/python3.10/site-packages/docutils/writers/s5_html/themes/default/pretty.css
--rw-rw-r--   0 atav1st   (1000) atav1st   (1001)      818 2023-07-16 15:28:55.000000 lolcatt-0.3.1/venv/lib/python3.10/site-packages/docutils/writers/s5_html/themes/default/print.css
--rw-rw-r--   0 atav1st   (1000) atav1st   (1001)      450 2023-07-16 15:28:55.000000 lolcatt-0.3.1/venv/lib/python3.10/site-packages/docutils/writers/s5_html/themes/default/s5-core.css
--rw-rw-r--   0 atav1st   (1000) atav1st   (1001)      283 2023-07-16 15:28:55.000000 lolcatt-0.3.1/venv/lib/python3.10/site-packages/docutils/writers/s5_html/themes/default/slides.css
-drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 16:47:28.262604 lolcatt-0.3.1/venv/lib/python3.10/site-packages/docutils/writers/s5_html/themes/medium-black/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1001)     4029 2023-07-16 15:28:55.000000 lolcatt-0.3.1/venv/lib/python3.10/site-packages/docutils/writers/s5_html/themes/medium-black/pretty.css
-drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 16:47:28.262604 lolcatt-0.3.1/venv/lib/python3.10/site-packages/docutils/writers/s5_html/themes/medium-white/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1001)      943 2023-07-16 15:28:55.000000 lolcatt-0.3.1/venv/lib/python3.10/site-packages/docutils/writers/s5_html/themes/medium-white/framing.css
--rw-rw-r--   0 atav1st   (1000) atav1st   (1001)     3989 2023-07-16 15:28:55.000000 lolcatt-0.3.1/venv/lib/python3.10/site-packages/docutils/writers/s5_html/themes/medium-white/pretty.css
-drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 16:47:28.265937 lolcatt-0.3.1/venv/lib/python3.10/site-packages/docutils/writers/s5_html/themes/small-black/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1001)     4028 2023-07-16 15:28:55.000000 lolcatt-0.3.1/venv/lib/python3.10/site-packages/docutils/writers/s5_html/themes/small-black/pretty.css
-drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 16:47:28.265937 lolcatt-0.3.1/venv/lib/python3.10/site-packages/docutils/writers/s5_html/themes/small-white/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1001)      940 2023-07-16 15:28:55.000000 lolcatt-0.3.1/venv/lib/python3.10/site-packages/docutils/writers/s5_html/themes/small-white/framing.css
--rw-rw-r--   0 atav1st   (1000) atav1st   (1001)     3999 2023-07-16 15:28:55.000000 lolcatt-0.3.1/venv/lib/python3.10/site-packages/docutils/writers/s5_html/themes/small-white/pretty.css
-drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 16:47:28.265937 lolcatt-0.3.1/venv/lib/python3.10/site-packages/lolcatt/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1001)       41 2023-07-16 15:29:01.000000 lolcatt-0.3.1/venv/lib/python3.10/site-packages/lolcatt/.githash
-drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 16:47:28.149271 lolcatt-0.3.1/venv/lib/python3.10/site-packages/lolcatt/ui/
-drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 16:47:28.269271 lolcatt-0.3.1/venv/lib/python3.10/site-packages/lolcatt/ui/ui_textual/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1001)     1579 2023-07-16 15:29:01.000000 lolcatt-0.3.1/venv/lib/python3.10/site-packages/lolcatt/ui/ui_textual/lolcatt.css
-drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 16:47:28.272604 lolcatt-0.3.1/venv/lib/python3.10/site-packages/textual/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1001)     3515 2023-07-16 15:29:00.000000 lolcatt-0.3.1/venv/lib/python3.10/site-packages/textual/demo.css
-drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 16:47:28.149271 lolcatt-0.3.1/venv/lib64/
-drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 16:47:28.149271 lolcatt-0.3.1/venv/lib64/python3.10/
-drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 16:47:28.155938 lolcatt-0.3.1/venv/lib64/python3.10/site-packages/
-drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 16:47:28.149271 lolcatt-0.3.1/venv/lib64/python3.10/site-packages/docutils/
-drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 16:47:28.149271 lolcatt-0.3.1/venv/lib64/python3.10/site-packages/docutils/writers/
-drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 16:47:28.285937 lolcatt-0.3.1/venv/lib64/python3.10/site-packages/docutils/writers/html4css1/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1001)     7219 2023-07-16 15:28:55.000000 lolcatt-0.3.1/venv/lib64/python3.10/site-packages/docutils/writers/html4css1/html4css1.css
-drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 16:47:28.285937 lolcatt-0.3.1/venv/lib64/python3.10/site-packages/docutils/writers/html5_polyglot/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1001)     6261 2023-07-16 15:28:55.000000 lolcatt-0.3.1/venv/lib64/python3.10/site-packages/docutils/writers/html5_polyglot/math.css
--rw-rw-r--   0 atav1st   (1000) atav1st   (1001)     7388 2023-07-16 15:28:55.000000 lolcatt-0.3.1/venv/lib64/python3.10/site-packages/docutils/writers/html5_polyglot/minimal.css
--rw-rw-r--   0 atav1st   (1000) atav1st   (1001)     7749 2023-07-16 15:28:55.000000 lolcatt-0.3.1/venv/lib64/python3.10/site-packages/docutils/writers/html5_polyglot/plain.css
--rw-rw-r--   0 atav1st   (1000) atav1st   (1001)    11895 2023-07-16 15:28:55.000000 lolcatt-0.3.1/venv/lib64/python3.10/site-packages/docutils/writers/html5_polyglot/responsive.css
--rw-rw-r--   0 atav1st   (1000) atav1st   (1001)    12023 2023-07-16 15:28:55.000000 lolcatt-0.3.1/venv/lib64/python3.10/site-packages/docutils/writers/html5_polyglot/tuftig.css
-drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 16:47:28.285937 lolcatt-0.3.1/venv/lib64/python3.10/site-packages/docutils/writers/pep_html/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1001)     6367 2023-07-16 15:28:55.000000 lolcatt-0.3.1/venv/lib64/python3.10/site-packages/docutils/writers/pep_html/pep.css
-drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 16:47:28.149271 lolcatt-0.3.1/venv/lib64/python3.10/site-packages/docutils/writers/s5_html/
-drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 16:47:28.152604 lolcatt-0.3.1/venv/lib64/python3.10/site-packages/docutils/writers/s5_html/themes/
-drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 16:47:28.285937 lolcatt-0.3.1/venv/lib64/python3.10/site-packages/docutils/writers/s5_html/themes/big-black/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1001)      910 2023-07-16 15:28:55.000000 lolcatt-0.3.1/venv/lib64/python3.10/site-packages/docutils/writers/s5_html/themes/big-black/framing.css
--rw-rw-r--   0 atav1st   (1000) atav1st   (1001)     3605 2023-07-16 15:28:55.000000 lolcatt-0.3.1/venv/lib64/python3.10/site-packages/docutils/writers/s5_html/themes/big-black/pretty.css
-drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 16:47:28.285937 lolcatt-0.3.1/venv/lib64/python3.10/site-packages/docutils/writers/s5_html/themes/big-white/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1001)      905 2023-07-16 15:28:55.000000 lolcatt-0.3.1/venv/lib64/python3.10/site-packages/docutils/writers/s5_html/themes/big-white/framing.css
--rw-rw-r--   0 atav1st   (1000) atav1st   (1001)     3565 2023-07-16 15:28:55.000000 lolcatt-0.3.1/venv/lib64/python3.10/site-packages/docutils/writers/s5_html/themes/big-white/pretty.css
-drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 16:47:28.289271 lolcatt-0.3.1/venv/lib64/python3.10/site-packages/docutils/writers/s5_html/themes/default/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1001)     1002 2023-07-16 15:28:55.000000 lolcatt-0.3.1/venv/lib64/python3.10/site-packages/docutils/writers/s5_html/themes/default/framing.css
--rw-rw-r--   0 atav1st   (1000) atav1st   (1001)      261 2023-07-16 15:28:55.000000 lolcatt-0.3.1/venv/lib64/python3.10/site-packages/docutils/writers/s5_html/themes/default/opera.css
--rw-rw-r--   0 atav1st   (1000) atav1st   (1001)      648 2023-07-16 15:28:55.000000 lolcatt-0.3.1/venv/lib64/python3.10/site-packages/docutils/writers/s5_html/themes/default/outline.css
--rw-rw-r--   0 atav1st   (1000) atav1st   (1001)     4383 2023-07-16 15:28:55.000000 lolcatt-0.3.1/venv/lib64/python3.10/site-packages/docutils/writers/s5_html/themes/default/pretty.css
--rw-rw-r--   0 atav1st   (1000) atav1st   (1001)      818 2023-07-16 15:28:55.000000 lolcatt-0.3.1/venv/lib64/python3.10/site-packages/docutils/writers/s5_html/themes/default/print.css
--rw-rw-r--   0 atav1st   (1000) atav1st   (1001)      450 2023-07-16 15:28:55.000000 lolcatt-0.3.1/venv/lib64/python3.10/site-packages/docutils/writers/s5_html/themes/default/s5-core.css
--rw-rw-r--   0 atav1st   (1000) atav1st   (1001)      283 2023-07-16 15:28:55.000000 lolcatt-0.3.1/venv/lib64/python3.10/site-packages/docutils/writers/s5_html/themes/default/slides.css
-drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 16:47:28.289271 lolcatt-0.3.1/venv/lib64/python3.10/site-packages/docutils/writers/s5_html/themes/medium-black/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1001)     4029 2023-07-16 15:28:55.000000 lolcatt-0.3.1/venv/lib64/python3.10/site-packages/docutils/writers/s5_html/themes/medium-black/pretty.css
-drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 16:47:28.289271 lolcatt-0.3.1/venv/lib64/python3.10/site-packages/docutils/writers/s5_html/themes/medium-white/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1001)      943 2023-07-16 15:28:55.000000 lolcatt-0.3.1/venv/lib64/python3.10/site-packages/docutils/writers/s5_html/themes/medium-white/framing.css
--rw-rw-r--   0 atav1st   (1000) atav1st   (1001)     3989 2023-07-16 15:28:55.000000 lolcatt-0.3.1/venv/lib64/python3.10/site-packages/docutils/writers/s5_html/themes/medium-white/pretty.css
-drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 16:47:28.289271 lolcatt-0.3.1/venv/lib64/python3.10/site-packages/docutils/writers/s5_html/themes/small-black/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1001)     4028 2023-07-16 15:28:55.000000 lolcatt-0.3.1/venv/lib64/python3.10/site-packages/docutils/writers/s5_html/themes/small-black/pretty.css
-drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 16:47:28.289271 lolcatt-0.3.1/venv/lib64/python3.10/site-packages/docutils/writers/s5_html/themes/small-white/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1001)      940 2023-07-16 15:28:55.000000 lolcatt-0.3.1/venv/lib64/python3.10/site-packages/docutils/writers/s5_html/themes/small-white/framing.css
--rw-rw-r--   0 atav1st   (1000) atav1st   (1001)     3999 2023-07-16 15:28:55.000000 lolcatt-0.3.1/venv/lib64/python3.10/site-packages/docutils/writers/s5_html/themes/small-white/pretty.css
-drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 16:47:28.289271 lolcatt-0.3.1/venv/lib64/python3.10/site-packages/lolcatt/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1001)       41 2023-07-16 15:29:01.000000 lolcatt-0.3.1/venv/lib64/python3.10/site-packages/lolcatt/.githash
-drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 16:47:28.155938 lolcatt-0.3.1/venv/lib64/python3.10/site-packages/lolcatt/ui/
-drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 16:47:28.289271 lolcatt-0.3.1/venv/lib64/python3.10/site-packages/lolcatt/ui/ui_textual/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1001)     1579 2023-07-16 15:29:01.000000 lolcatt-0.3.1/venv/lib64/python3.10/site-packages/lolcatt/ui/ui_textual/lolcatt.css
-drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 16:47:28.289271 lolcatt-0.3.1/venv/lib64/python3.10/site-packages/textual/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1001)     3515 2023-07-16 15:29:00.000000 lolcatt-0.3.1/venv/lib64/python3.10/site-packages/textual/demo.css
+drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 20:54:52.482034 lolcatt-0.4.1/
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)     1074 2023-07-23 10:21:40.000000 lolcatt-0.4.1/LICENSE
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)      240 2024-05-11 20:35:15.000000 lolcatt-0.4.1/MANIFEST.in
+-rw-r--r--   0 atav1st   (1000) atav1st   (1001)     4447 2024-05-11 20:54:52.482034 lolcatt-0.4.1/PKG-INFO
+-rw-r--r--   0 atav1st   (1000) atav1st   (1001)     3639 2024-05-11 20:34:34.000000 lolcatt-0.4.1/README.rst
+drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 20:54:50.105368 lolcatt-0.4.1/docs/
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)      608 2023-07-23 10:21:40.000000 lolcatt-0.4.1/docs/Makefile
+drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 20:54:50.102035 lolcatt-0.4.1/docs/_build/
+drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 20:54:50.102035 lolcatt-0.4.1/docs/_build/html/
+drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 20:54:52.452034 lolcatt-0.4.1/docs/_build/html/_static/
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)    14813 2023-07-23 10:39:33.000000 lolcatt-0.4.1/docs/_build/html/_static/basic.css
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)       84 2023-07-23 10:21:40.000000 lolcatt-0.4.1/docs/_build/html/_static/custom.css
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)      286 2023-05-12 22:36:26.000000 lolcatt-0.4.1/docs/_build/html/_static/file.png
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)       90 2023-05-12 22:36:26.000000 lolcatt-0.4.1/docs/_build/html/_static/minus.png
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)     4208 2023-07-23 10:39:33.000000 lolcatt-0.4.1/docs/_build/html/_static/nature.css
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)       90 2023-05-12 22:36:26.000000 lolcatt-0.4.1/docs/_build/html/_static/plus.png
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)     4956 2023-07-23 10:39:33.000000 lolcatt-0.4.1/docs/_build/html/_static/pygments.css
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)    26168 2023-07-23 10:21:40.000000 lolcatt-0.4.1/docs/_build/html/_static/screenshot.png
+drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 20:54:52.455367 lolcatt-0.4.1/docs/_static/
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)       84 2023-07-23 10:21:40.000000 lolcatt-0.4.1/docs/_static/custom.css
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)    26168 2023-07-23 10:21:40.000000 lolcatt-0.4.1/docs/_static/screenshot.png
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)     4983 2023-07-23 10:21:40.000000 lolcatt-0.4.1/docs/conf.py
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)      264 2023-07-23 10:21:40.000000 lolcatt-0.4.1/docs/index.rst
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)     1138 2023-07-23 10:21:40.000000 lolcatt-0.4.1/docs/installation.rst
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)      346 2023-07-23 10:21:40.000000 lolcatt-0.4.1/docs/lolcatt.casting.rst
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)      517 2023-07-23 10:39:30.000000 lolcatt-0.4.1/docs/lolcatt.rst
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)     1232 2023-07-23 10:21:40.000000 lolcatt-0.4.1/docs/lolcatt.ui.rst
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)      331 2023-07-23 10:21:40.000000 lolcatt-0.4.1/docs/lolcatt.utils.rst
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)      805 2023-07-23 10:21:40.000000 lolcatt-0.4.1/docs/make.bat
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)       58 2023-07-23 10:39:30.000000 lolcatt-0.4.1/docs/modules.rst
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)       27 2023-07-23 10:21:40.000000 lolcatt-0.4.1/docs/readme.rst
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)       69 2023-07-23 10:21:40.000000 lolcatt-0.4.1/docs/usage.rst
+drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 20:54:52.455367 lolcatt-0.4.1/lolcatt/
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)       41 2023-07-16 00:01:30.000000 lolcatt-0.4.1/lolcatt/.githash
+-rw-r--r--   0 atav1st   (1000) atav1st   (1001)      125 2024-05-11 20:50:05.000000 lolcatt-0.4.1/lolcatt/__init__.py
+-rw-r--r--   0 atav1st   (1000) atav1st   (1001)     1714 2024-05-11 20:34:34.000000 lolcatt-0.4.1/lolcatt/app.py
+drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 20:54:52.455367 lolcatt-0.4.1/lolcatt/casting/
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)        0 2023-07-23 10:21:40.000000 lolcatt-0.4.1/lolcatt/casting/__init__.py
+-rw-r--r--   0 atav1st   (1000) atav1st   (1001)    11287 2024-05-11 20:34:34.000000 lolcatt-0.4.1/lolcatt/casting/caster.py
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)     1336 2023-10-29 15:57:47.000000 lolcatt-0.4.1/lolcatt/casting/youtube_playlist_handler.py
+-rw-r--r--   0 atav1st   (1000) atav1st   (1001)     1827 2024-05-11 20:23:39.000000 lolcatt-0.4.1/lolcatt/cli.py
+drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 20:54:52.455367 lolcatt-0.4.1/lolcatt/ui/
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)        0 2023-07-23 10:21:40.000000 lolcatt-0.4.1/lolcatt/ui/__init__.py
+-rw-r--r--   0 atav1st   (1000) atav1st   (1001)     1918 2024-05-11 20:34:34.000000 lolcatt-0.4.1/lolcatt/ui/lolcatt.tcss
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)     4860 2023-10-29 15:57:12.000000 lolcatt-0.4.1/lolcatt/ui/lolcatt_controls.py
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)     1265 2023-07-23 10:25:25.000000 lolcatt-0.4.1/lolcatt/ui/lolcatt_device_info.py
+-rw-r--r--   0 atav1st   (1000) atav1st   (1001)     1933 2024-05-11 20:34:34.000000 lolcatt-0.4.1/lolcatt/ui/lolcatt_playback_info.py
+-rw-r--r--   0 atav1st   (1000) atav1st   (1001)     2186 2024-05-11 20:47:38.000000 lolcatt-0.4.1/lolcatt/ui/lolcatt_playlist.py
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)     3068 2023-07-23 10:25:50.000000 lolcatt-0.4.1/lolcatt/ui/lolcatt_progress.py
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)     3016 2023-10-29 15:57:12.000000 lolcatt-0.4.1/lolcatt/ui/lolcatt_url_input.py
+drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 20:54:52.458701 lolcatt-0.4.1/lolcatt/utils/
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)        0 2023-07-23 10:21:40.000000 lolcatt-0.4.1/lolcatt/utils/__init__.py
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)     2422 2023-10-29 15:57:52.000000 lolcatt-0.4.1/lolcatt/utils/utils.py
+drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 20:54:52.482034 lolcatt-0.4.1/lolcatt.egg-info/
+-rw-r--r--   0 atav1st   (1000) atav1st   (1001)     4447 2024-05-11 20:54:49.000000 lolcatt-0.4.1/lolcatt.egg-info/PKG-INFO
+-rw-r--r--   0 atav1st   (1000) atav1st   (1001)     1423 2024-05-11 20:54:50.000000 lolcatt-0.4.1/lolcatt.egg-info/SOURCES.txt
+-rw-r--r--   0 atav1st   (1000) atav1st   (1001)        1 2024-05-11 20:54:49.000000 lolcatt-0.4.1/lolcatt.egg-info/dependency_links.txt
+-rw-r--r--   0 atav1st   (1000) atav1st   (1001)       45 2024-05-11 20:54:49.000000 lolcatt-0.4.1/lolcatt.egg-info/entry_points.txt
+-rw-r--r--   0 atav1st   (1000) atav1st   (1001)        1 2024-05-11 20:54:49.000000 lolcatt-0.4.1/lolcatt.egg-info/not-zip-safe
+-rw-r--r--   0 atav1st   (1000) atav1st   (1001)       54 2024-05-11 20:54:49.000000 lolcatt-0.4.1/lolcatt.egg-info/requires.txt
+-rw-r--r--   0 atav1st   (1000) atav1st   (1001)        8 2024-05-11 20:54:49.000000 lolcatt-0.4.1/lolcatt.egg-info/top_level.txt
+-rw-r--r--   0 atav1st   (1000) atav1st   (1001)      559 2024-05-11 20:50:05.000000 lolcatt-0.4.1/pyproject.toml
+-rw-r--r--   0 atav1st   (1000) atav1st   (1001)       38 2024-05-11 20:54:52.482034 lolcatt-0.4.1/setup.cfg
+-rw-r--r--   0 atav1st   (1000) atav1st   (1001)     1556 2024-05-11 20:50:05.000000 lolcatt-0.4.1/setup.py
+drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 20:54:52.458701 lolcatt-0.4.1/tests/
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)       37 2023-07-23 10:21:40.000000 lolcatt-0.4.1/tests/__init__.py
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)      211 2023-07-23 10:21:40.000000 lolcatt-0.4.1/tests/test_lolcatt.py
+drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 20:54:50.102035 lolcatt-0.4.1/venv/
+drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 20:54:50.102035 lolcatt-0.4.1/venv/lib/
+drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 20:54:50.102035 lolcatt-0.4.1/venv/lib/python3.10/
+drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 20:54:50.102035 lolcatt-0.4.1/venv/lib/python3.10/site-packages/
+drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 20:54:52.458701 lolcatt-0.4.1/venv/lib/python3.10/site-packages/lolcatt/
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)       41 2023-07-16 15:29:01.000000 lolcatt-0.4.1/venv/lib/python3.10/site-packages/lolcatt/.githash
+drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 20:54:50.102035 lolcatt-0.4.1/venv/lib64/
+drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 20:54:50.102035 lolcatt-0.4.1/venv/lib64/python3.10/
+drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 20:54:50.102035 lolcatt-0.4.1/venv/lib64/python3.10/site-packages/
+drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 20:54:52.482034 lolcatt-0.4.1/venv/lib64/python3.10/site-packages/lolcatt/
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)       41 2023-07-16 15:29:01.000000 lolcatt-0.4.1/venv/lib64/python3.10/site-packages/lolcatt/.githash
```

### Comparing `lolcatt-0.3.1/LICENSE` & `lolcatt-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lolcatt-0.3.1/PKG-INFO` & `lolcatt-0.4.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lolcatt
-Version: 0.3.1
+Version: 0.4.1
 Summary: A TUI wrapper around `catt`.
 Home-page: https://github.com/LokiLuciferase/lolcatt
 Author: Lukas Lüftinger
 Author-email: lukas.lueftinger@outlook.com
 License: MIT license
 Keywords: lolcatt
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -49,15 +49,15 @@
 .. image:: https://raw.githubusercontent.com/LokiLuciferase/lolcatt/master/docs/_static/screenshot.png
    :align: center
    :alt:
 
 
 Dependencies
 ------------
-- Python 3.8+
+- Python 3.10+ (older versions >= 3.6 might work, but are not tested)
 - catt_ (will be installed automatically)
 - yt-dlp_ (will be installed automatically)
 - Optional: A font containing FontAwesome icons to allow displaying of fancy icons on buttons. The freely available NerdFont_ collection is recommended. Fancy icons can be disabled and replaced by text (see below).
 
 
 Installation
 ------------
@@ -70,15 +70,15 @@
 Quckstart
 ----------
 
 At first we need to determine the name of the chromecast device we want to cast to. To do so, run ``lolcatt --scan``.
 To start the UI, run ``lolcatt -d '<device name or alias>'`` (or simply ``lolcatt`` if a default device is set).
 A default device and device aliases can be set in the ``catt`` configuration file (per default under ``~/.config/catt/config.cfg``), see catt_'s documentation for more information.
 
-To cast, paste either a URL or a path to a local file into the input field and press enter. To add a URL or path to the playback queue instead of playing immediately, hit Ctrl+s instead of enter. To seek, tap the progress bar.
+To cast, paste either a URL or a path to a local file into the input field and press enter. To add a URL or path to the playback queue instead of playing immediately, hit Ctrl+s instead of enter. To view and navigate in the queue, tap the name of the currently playing item. To seek, tap the progress bar.
 
 For URLs, all websites supported by yt-dlp_ (which handles media download under the hood) are supported. Find a list of supported websites here_. For local media, most common video and image formats are supported.
 
 Youtube playlists are supported, and each contained video will be added to the playback queue. By specifying a cookie file in the config (per default under ``~/.config/lolcatt/config.toml``), you can also access private YouTube playlists such as "Watch Later" (https://www.youtube.com/playlist?list=WL), and ensure played YouTube videos are marked as watched.
 
 
 Troubleshooting
```

### Comparing `lolcatt-0.3.1/README.rst` & `lolcatt-0.4.1/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 .. image:: https://raw.githubusercontent.com/LokiLuciferase/lolcatt/master/docs/_static/screenshot.png
    :align: center
    :alt:
 
 
 Dependencies
 ------------
-- Python 3.8+
+- Python 3.10+ (older versions >= 3.6 might work, but are not tested)
 - catt_ (will be installed automatically)
 - yt-dlp_ (will be installed automatically)
 - Optional: A font containing FontAwesome icons to allow displaying of fancy icons on buttons. The freely available NerdFont_ collection is recommended. Fancy icons can be disabled and replaced by text (see below).
 
 
 Installation
 ------------
@@ -45,15 +45,15 @@
 Quckstart
 ----------
 
 At first we need to determine the name of the chromecast device we want to cast to. To do so, run ``lolcatt --scan``.
 To start the UI, run ``lolcatt -d '<device name or alias>'`` (or simply ``lolcatt`` if a default device is set).
 A default device and device aliases can be set in the ``catt`` configuration file (per default under ``~/.config/catt/config.cfg``), see catt_'s documentation for more information.
 
-To cast, paste either a URL or a path to a local file into the input field and press enter. To add a URL or path to the playback queue instead of playing immediately, hit Ctrl+s instead of enter. To seek, tap the progress bar.
+To cast, paste either a URL or a path to a local file into the input field and press enter. To add a URL or path to the playback queue instead of playing immediately, hit Ctrl+s instead of enter. To view and navigate in the queue, tap the name of the currently playing item. To seek, tap the progress bar.
 
 For URLs, all websites supported by yt-dlp_ (which handles media download under the hood) are supported. Find a list of supported websites here_. For local media, most common video and image formats are supported.
 
 Youtube playlists are supported, and each contained video will be added to the playback queue. By specifying a cookie file in the config (per default under ``~/.config/lolcatt/config.toml``), you can also access private YouTube playlists such as "Watch Later" (https://www.youtube.com/playlist?list=WL), and ensure played YouTube videos are marked as watched.
 
 
 Troubleshooting
```

### Comparing `lolcatt-0.3.1/docs/Makefile` & `lolcatt-0.4.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `lolcatt-0.3.1/docs/_build/html/_static/basic.css` & `lolcatt-0.4.1/docs/_build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `lolcatt-0.3.1/docs/_build/html/_static/nature.css` & `lolcatt-0.4.1/docs/_build/html/_static/nature.css`

 * *Files identical despite different names*

### Comparing `lolcatt-0.3.1/docs/_build/html/_static/pygments.css` & `lolcatt-0.4.1/docs/_build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `lolcatt-0.3.1/docs/_build/html/_static/screenshot.png` & `lolcatt-0.4.1/docs/_build/html/_static/screenshot.png`

 * *Files identical despite different names*

### Comparing `lolcatt-0.3.1/docs/_static/screenshot.png` & `lolcatt-0.4.1/docs/_static/screenshot.png`

 * *Files identical despite different names*

### Comparing `lolcatt-0.3.1/docs/conf.py` & `lolcatt-0.4.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `lolcatt-0.3.1/docs/installation.rst` & `lolcatt-0.4.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `lolcatt-0.3.1/docs/lolcatt.rst` & `lolcatt-0.4.1/docs/lolcatt.rst`

 * *Files identical despite different names*

### Comparing `lolcatt-0.3.1/docs/lolcatt.ui.rst` & `lolcatt-0.4.1/docs/lolcatt.ui.rst`

 * *Files identical despite different names*

### Comparing `lolcatt-0.3.1/docs/make.bat` & `lolcatt-0.4.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `lolcatt-0.3.1/lolcatt/app.py` & `lolcatt-0.4.1/lolcatt/app.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from textual.containers import Container
 from textual.screen import Screen
 
 from lolcatt.casting.caster import Caster
 from lolcatt.ui.lolcatt_controls import LolCattControls
 from lolcatt.ui.lolcatt_device_info import LolCattDeviceInfo
 from lolcatt.ui.lolcatt_playback_info import LolCattPlaybackInfo
+from lolcatt.ui.lolcatt_playlist import LolCattPlaylist
 from lolcatt.ui.lolcatt_progress import LolCattProgress
 from lolcatt.ui.lolcatt_url_input import LolCattUrlInput
 
 
 class RemoteScreen(Screen):
     """A screen for the remote control UI."""
 
@@ -22,27 +23,37 @@
             LolCattProgress(),
             LolCattControls(),
             LolCattUrlInput(),
             id='app',
         )
 
 
+class PlaylistScreen(Screen):
+    """A screen for the playlist UI."""
+
+    def compose(self):
+        yield LolCattPlaylist()
+
+
 class LolCatt(App):
     """The main application class for lolcatt."""
 
-    CSS_PATH = 'ui/lolcatt.css'
+    CSS_PATH = 'ui/lolcatt.tcss'
 
     def __init__(self, device_name: str = None, config: Dict = None, *args, **kwargs):
         self.config = config
         self.caster = Caster(device_name, config=config)
         self.remote_screen = None
+        self.playlist_screen = None
         super().__init__(*args, **kwargs)
 
     def on_mount(self):
         self.remote_screen = RemoteScreen()
+        self.playlist_screen = PlaylistScreen()
         self.install_screen(self.remote_screen, name='remote')
+        self.install_screen(self.playlist_screen, name='playlist')
         self.push_screen('remote')
 
 
 if __name__ == '__main__':
     app = LolCatt('default')
     app.run()
```

### Comparing `lolcatt-0.3.1/lolcatt/casting/caster.py` & `lolcatt-0.4.1/lolcatt/casting/caster.py`

 * *Files 6% similar despite different names*

```diff
@@ -127,14 +127,37 @@
         if self._current_item is not None:
             self._queue.insert(0, self._current_item)
             self._current_item = None
         if len(self._played_queue) > 0:
             self._current_item = self._played_queue.pop()
             self.cast(self._current_item)
 
+    def cast_at_idx(self, idx: int):
+        """
+        Skips to the item at the given index in the queues.
+        """
+        if idx == 0:
+            return
+        if idx < 0:
+            prev_idx = len(self._played_queue) + idx
+            if prev_idx < 0:
+                return
+            self._queue.insert(0, self._current_item)
+            self._queue = self._played_queue[prev_idx + 1 :] + self._queue
+            self._played_queue = self._played_queue[: prev_idx + 1]
+            self._current_item = self._played_queue.pop(-1)
+        else:
+            if idx > len(self._queue):
+                return
+            self._played_queue.append(self._current_item)
+            self._played_queue += self._queue[: idx - 1]
+            self._current_item = self._queue.pop(idx - 1)
+            self._queue = self._queue[idx - 1 :]
+        self.cast(self._current_item)
+
     def stop_cast(self):
         """
         Stops the current cast.
         """
         if self._current_item is not None:
             self._played_queue.append(self._current_item)
             self._current_item = None
@@ -167,14 +190,30 @@
         """
         Returns the current queue.
 
         :return: The current queue.
         """
         return self._queue
 
+    def get_current_item(self) -> Optional[str]:
+        """
+        Returns the currently playing item.
+
+        :return: The currently playing item.
+        """
+        return self._current_item
+
+    def get_played_queue(self) -> List[str]:
+        """
+        Returns the played queue.
+
+        :return: The played queue.
+        """
+        return self._played_queue
+
     def get_available_devices(self) -> List[str]:
         """
         Runs Chromecast discovery and returns a list of available CattDevices.
 
         :return: A list of available CattDevices.
         """
         self._available_devices = discover()
```

### Comparing `lolcatt-0.3.1/lolcatt/casting/youtube_playlist_handler.py` & `lolcatt-0.4.1/lolcatt/casting/youtube_playlist_handler.py`

 * *Files identical despite different names*

### Comparing `lolcatt-0.3.1/lolcatt/cli.py` & `lolcatt-0.4.1/lolcatt/cli.py`

 * *Files identical despite different names*

### Comparing `lolcatt-0.3.1/lolcatt/ui/lolcatt.css` & `lolcatt-0.4.1/lolcatt/ui/lolcatt.tcss`

 * *Files 6% similar despite different names*

```diff
@@ -91,13 +91,37 @@
     margin-top: 0;
     margin-bottom: 0;
     margin-right: 1;
     margin-left: 1;
     border: grey;
 }
 
+#playlist_box {
+    layout: vertical;
+    align: center middle;
+    dock: top;
+    max-height: 18;
+    max-width: 41;
+}
+
+#playlist_close_btn {
+    max-width: 5;
+    max-height: 3;
+}
+
+#playlist > ListItem {
+    padding-top: 1;
+    padding-bottom: 1;
+    padding-left: 2;
+    padding-right: 2;
+}
+
+#playlist_item_0 {
+    text-style: bold;
+}
+
 #app {
     layout: vertical;
     align: center middle;
     dock: top;
     max-width: 41;
 }
```

### Comparing `lolcatt-0.3.1/lolcatt/ui/lolcatt_controls.py` & `lolcatt-0.4.1/lolcatt/ui/lolcatt_controls.py`

 * *Files identical despite different names*

### Comparing `lolcatt-0.3.1/lolcatt/ui/lolcatt_device_info.py` & `lolcatt-0.4.1/lolcatt/ui/lolcatt_device_info.py`

 * *Files identical despite different names*

### Comparing `lolcatt-0.3.1/lolcatt/ui/lolcatt_playback_info.py` & `lolcatt-0.4.1/lolcatt/ui/lolcatt_playback_info.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from textual.containers import Container
+from textual.events import Click
 from textual.reactive import reactive
 from textual.widgets import Label
+from textual.widgets import ListItem
 from textual.widgets import Static
 
 from lolcatt.utils.utils import marquee
 
 
 class LolCattPlaybackInfo(Static):
     label_str = reactive('')
@@ -44,7 +46,13 @@
     def compose(self):
         yield Container(self.label, id='playback_info')
 
     def on_mount(self):
         self.set_interval(
             interval=self.app.caster.get_update_interval(), callback=self._update_label
         )
+
+    def on_click(self, event: Click):
+        queue = self.app.caster.get_queue()
+        queuelist = [ListItem(Label(x)) for x in queue]
+        self.app.playlist_list = queuelist
+        self.app.push_screen('playlist')
```

### Comparing `lolcatt-0.3.1/lolcatt/ui/lolcatt_progress.py` & `lolcatt-0.4.1/lolcatt/ui/lolcatt_progress.py`

 * *Files identical despite different names*

### Comparing `lolcatt-0.3.1/lolcatt/ui/lolcatt_url_input.py` & `lolcatt-0.4.1/lolcatt/ui/lolcatt_url_input.py`

 * *Files identical despite different names*

### Comparing `lolcatt-0.3.1/lolcatt/utils/utils.py` & `lolcatt-0.4.1/lolcatt/utils/utils.py`

 * *Files identical despite different names*

### Comparing `lolcatt-0.3.1/lolcatt.egg-info/PKG-INFO` & `lolcatt-0.4.1/lolcatt.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lolcatt
-Version: 0.3.1
+Version: 0.4.1
 Summary: A TUI wrapper around `catt`.
 Home-page: https://github.com/LokiLuciferase/lolcatt
 Author: Lukas Lüftinger
 Author-email: lukas.lueftinger@outlook.com
 License: MIT license
 Keywords: lolcatt
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -49,15 +49,15 @@
 .. image:: https://raw.githubusercontent.com/LokiLuciferase/lolcatt/master/docs/_static/screenshot.png
    :align: center
    :alt:
 
 
 Dependencies
 ------------
-- Python 3.8+
+- Python 3.10+ (older versions >= 3.6 might work, but are not tested)
 - catt_ (will be installed automatically)
 - yt-dlp_ (will be installed automatically)
 - Optional: A font containing FontAwesome icons to allow displaying of fancy icons on buttons. The freely available NerdFont_ collection is recommended. Fancy icons can be disabled and replaced by text (see below).
 
 
 Installation
 ------------
@@ -70,15 +70,15 @@
 Quckstart
 ----------
 
 At first we need to determine the name of the chromecast device we want to cast to. To do so, run ``lolcatt --scan``.
 To start the UI, run ``lolcatt -d '<device name or alias>'`` (or simply ``lolcatt`` if a default device is set).
 A default device and device aliases can be set in the ``catt`` configuration file (per default under ``~/.config/catt/config.cfg``), see catt_'s documentation for more information.
 
-To cast, paste either a URL or a path to a local file into the input field and press enter. To add a URL or path to the playback queue instead of playing immediately, hit Ctrl+s instead of enter. To seek, tap the progress bar.
+To cast, paste either a URL or a path to a local file into the input field and press enter. To add a URL or path to the playback queue instead of playing immediately, hit Ctrl+s instead of enter. To view and navigate in the queue, tap the name of the currently playing item. To seek, tap the progress bar.
 
 For URLs, all websites supported by yt-dlp_ (which handles media download under the hood) are supported. Find a list of supported websites here_. For local media, most common video and image formats are supported.
 
 Youtube playlists are supported, and each contained video will be added to the playback queue. By specifying a cookie file in the config (per default under ``~/.config/lolcatt/config.toml``), you can also access private YouTube playlists such as "Watch Later" (https://www.youtube.com/playlist?list=WL), and ensure played YouTube videos are marked as watched.
 
 
 Troubleshooting
```

### Comparing `lolcatt-0.3.1/pyproject.toml` & `lolcatt-0.4.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
   | buck-out
   | build
   | dist
 )/
 '''
 
 [tool.bumpver]
-current_version = "0.3.1"
+current_version = "0.4.1"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `lolcatt-0.3.1/setup.py` & `lolcatt-0.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,10 +40,10 @@
     include_package_data=True,
     keywords='lolcatt',
     name='lolcatt',
     packages=find_packages(include=['lolcatt', 'lolcatt.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/LokiLuciferase/lolcatt',
-    version='0.3.1',
+    version='0.4.1',
     zip_safe=False,
 )
```

