# Comparing `tmp/sbn-94.tar.gz` & `tmp/sbn-95.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sbn-94.tar", last modified: Fri Apr  5 13:12:56 2024, max compression
+gzip compressed data, was "sbn-95.tar", last modified: Sun May 12 05:56:48 2024, max compression
```

## Comparing `sbn-94.tar` & `sbn-95.tar`

### file list

```diff
@@ -1,92 +1,79 @@
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-05 13:12:56.600584 sbn-94/
--rw-r--r--   0 bart      (1000) bart      (1000)     2807 2024-04-05 13:01:11.000000 sbn-94/MANUAL.rst
--rw-r--r--   0 bart      (1000) bart      (1000)     2495 2024-04-05 13:12:56.600584 sbn-94/PKG-INFO
--rw-r--r--   0 bart      (1000) bart      (1000)     1933 2024-04-05 12:58:23.000000 sbn-94/README.rst
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-05 13:12:56.592584 sbn-94/docs/
--rw-r--r--   0 bart      (1000) bart      (1000)   180711 2024-04-05 12:12:33.000000 sbn-94/docs/ECHAabilify.png
--rw-r--r--   0 bart      (1000) bart      (1000)   193757 2024-04-05 12:12:33.000000 sbn-94/docs/ECHAclozapine.png
--rw-r--r--   0 bart      (1000) bart      (1000)   197697 2024-04-05 12:12:33.000000 sbn-94/docs/ECHAhaldol.png
--rw-r--r--   0 bart      (1000) bart      (1000)   232313 2024-04-05 12:12:33.000000 sbn-94/docs/ECHAzyprexa.png
--rw-r--r--   0 bart      (1000) bart      (1000)   245670 2024-04-05 12:12:33.000000 sbn-94/docs/OTP1.png
--rw-r--r--   0 bart      (1000) bart      (1000)   238095 2024-04-05 12:12:33.000000 sbn-94/docs/OTP2.png
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-05 13:12:56.592584 sbn-94/docs/_static/
--rw-r--r--   0 bart      (1000) bart      (1000)     1000 2024-04-05 12:12:33.000000 sbn-94/docs/_static/sbn.css
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-05 13:12:56.592584 sbn-94/docs/_templates/
--rw-r--r--   0 bart      (1000) bart      (1000)      291 2024-04-05 12:12:33.000000 sbn-94/docs/_templates/base.rst
--rw-r--r--   0 bart      (1000) bart      (1000)      543 2024-04-05 12:12:33.000000 sbn-94/docs/_templates/class.rst
--rw-r--r--   0 bart      (1000) bart      (1000)      879 2024-04-05 12:12:33.000000 sbn-94/docs/_templates/mine.rst
--rw-r--r--   0 bart      (1000) bart      (1000)      879 2024-04-05 12:12:33.000000 sbn-94/docs/_templates/module.rst
--rw-r--r--   0 bart      (1000) bart      (1000)     1434 2024-04-05 12:12:33.000000 sbn-94/docs/about.rst
--rw-r--r--   0 bart      (1000) bart      (1000)   130021 2024-04-05 12:12:33.000000 sbn-94/docs/arrest.png
--rw-r--r--   0 bart      (1000) bart      (1000)   256520 2024-04-05 12:12:33.000000 sbn-94/docs/banner.png
--rw-r--r--   0 bart      (1000) bart      (1000)  1685507 2024-04-05 12:12:33.000000 sbn-94/docs/bevestigd.jpg
--rw-r--r--   0 bart      (1000) bart      (1000)     3246 2024-04-05 12:12:33.000000 sbn-94/docs/conf.py
--rw-r--r--   0 bart      (1000) bart      (1000)      537 2024-04-05 12:12:33.000000 sbn-94/docs/evidence.rst
--rw-r--r--   0 bart      (1000) bart      (1000)    47740 2024-04-05 12:12:33.000000 sbn-94/docs/genocide.png
--rw-r--r--   0 bart      (1000) bart      (1000)      303 2024-04-05 12:12:33.000000 sbn-94/docs/guilty.rst
--rw-r--r--   0 bart      (1000) bart      (1000)     2087 2024-04-05 13:11:33.000000 sbn-94/docs/index.rst
--rw-r--r--   0 bart      (1000) bart      (1000)    69979 2024-04-05 12:12:33.000000 sbn-94/docs/informed.jpg
--rw-r--r--   0 bart      (1000) bart      (1000)   228393 2024-04-05 12:12:33.000000 sbn-94/docs/kamer.png
--rw-r--r--   0 bart      (1000) bart      (1000)     3413 2024-04-05 13:00:34.000000 sbn-94/docs/manual.rst
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-05 13:12:56.596583 sbn-94/docs/pdf/
--rw-r--r--   0 bart      (1000) bart      (1000)   238330 2024-04-05 12:12:33.000000 sbn-94/docs/pdf/EM_T04_OTP-CR-117_19.pdf
--rw-r--r--   0 bart      (1000) bart      (1000)   236671 2024-04-05 12:12:33.000000 sbn-94/docs/pdf/EM_T07_OTP-CR-117_19_001.pdf
--rw-r--r--   0 bart      (1000) bart      (1000)    41559 2024-04-05 12:12:33.000000 sbn-94/docs/pdf/Kamer.pdf
--rw-r--r--   0 bart      (1000) bart      (1000)   323490 2024-04-05 12:12:33.000000 sbn-94/docs/pdf/Rome-Statute.pdf
--rw-r--r--   0 bart      (1000) bart      (1000)    50044 2024-04-05 12:12:33.000000 sbn-94/docs/pdf/bevestigd.pdf
--rw-r--r--   0 bart      (1000) bart      (1000)     2196 2024-04-05 12:12:33.000000 sbn-94/docs/request.rst
--rw-r--r--   0 bart      (1000) bart      (1000)   179869 2024-04-05 12:12:33.000000 sbn-94/docs/skull.jpg
--rw-r--r--   0 bart      (1000) bart      (1000)   287102 2024-04-05 12:12:33.000000 sbn-94/docs/skull3.png
--rw-r--r--   0 bart      (1000) bart      (1000)     1494 2024-04-05 12:55:42.000000 sbn-94/docs/source.rst
--rw-r--r--   0 bart      (1000) bart      (1000)      176 2024-04-05 12:12:33.000000 sbn-94/docs/verbatim.rst
--rw-r--r--   0 bart      (1000) bart      (1000)   234877 2024-04-05 12:12:33.000000 sbn-94/docs/verbatim2.png
--rw-r--r--   0 bart      (1000) bart      (1000)    46476 2024-04-05 12:12:33.000000 sbn-94/docs/wallpaper.png
--rw-r--r--   0 bart      (1000) bart      (1000)     1120 2024-04-05 12:12:33.000000 sbn-94/docs/writings.rst
--rw-r--r--   0 bart      (1000) bart      (1000)     2073 2024-04-05 13:05:17.000000 sbn-94/pyproject.toml
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-05 13:12:56.596583 sbn-94/sbn/
--rw-r--r--   0 bart      (1000) bart      (1000)       84 2024-04-04 12:27:14.000000 sbn-94/sbn/__init__.py
--rw-r--r--   0 bart      (1000) bart      (1000)     3915 2024-04-04 13:15:53.000000 sbn-94/sbn/__main__.py
--rw-r--r--   0 bart      (1000) bart      (1000)      904 2024-04-04 11:48:34.000000 sbn-94/sbn/broker.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1582 2024-04-04 12:05:43.000000 sbn-94/sbn/client.py
--rw-r--r--   0 bart      (1000) bart      (1000)      321 2024-04-04 11:47:18.000000 sbn-94/sbn/default.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1738 2024-04-04 13:39:07.000000 sbn-94/sbn/errors.py
--rw-r--r--   0 bart      (1000) bart      (1000)      865 2024-04-04 11:46:43.000000 sbn-94/sbn/event.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1608 2024-04-04 12:10:33.000000 sbn-94/sbn/handler.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1442 2024-04-05 11:15:28.000000 sbn-94/sbn/interface.py
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-05 13:12:56.600584 sbn-94/sbn/modules/
--rw-r--r--   0 bart      (1000) bart      (1000)      436 2024-04-04 11:31:06.000000 sbn-94/sbn/modules/__init__.py
--rw-r--r--   0 bart      (1000) bart      (1000)      239 2024-04-05 11:22:25.000000 sbn-94/sbn/modules/cmd.py
--rw-r--r--   0 bart      (1000) bart      (1000)      254 2024-04-05 11:22:46.000000 sbn-94/sbn/modules/dbg.py
--rw-r--r--   0 bart      (1000) bart      (1000)      573 2024-04-05 11:23:11.000000 sbn-94/sbn/modules/err.py
--rw-r--r--   0 bart      (1000) bart      (1000)      424 2024-04-05 11:23:26.000000 sbn-94/sbn/modules/flt.py
--rw-r--r--   0 bart      (1000) bart      (1000)      826 2024-04-05 11:44:57.000000 sbn-94/sbn/modules/fnd.py
--rw-r--r--   0 bart      (1000) bart      (1000)    19015 2024-04-05 11:25:16.000000 sbn-94/sbn/modules/irc.py
--rw-r--r--   0 bart      (1000) bart      (1000)      841 2024-04-05 11:25:50.000000 sbn-94/sbn/modules/log.py
--rw-r--r--   0 bart      (1000) bart      (1000)     2482 2024-04-05 11:27:00.000000 sbn-94/sbn/modules/mbx.py
--rw-r--r--   0 bart      (1000) bart      (1000)    16468 2024-04-05 11:28:55.000000 sbn-94/sbn/modules/mdl.py
--rw-r--r--   0 bart      (1000) bart      (1000)      264 2024-04-05 11:29:51.000000 sbn-94/sbn/modules/mod.py
--rw-r--r--   0 bart      (1000) bart      (1000)     2428 2024-04-05 11:31:46.000000 sbn-94/sbn/modules/req.py
--rw-r--r--   0 bart      (1000) bart      (1000)    10937 2024-04-05 11:35:17.000000 sbn-94/sbn/modules/rss.py
--rw-r--r--   0 bart      (1000) bart      (1000)     3213 2024-04-05 11:36:34.000000 sbn-94/sbn/modules/rst.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1196 2024-04-05 11:37:54.000000 sbn-94/sbn/modules/tdo.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1082 2024-04-05 11:38:18.000000 sbn-94/sbn/modules/thr.py
--rw-r--r--   0 bart      (1000) bart      (1000)     5282 2024-04-05 11:42:28.000000 sbn-94/sbn/modules/tmr.py
--rw-r--r--   0 bart      (1000) bart      (1000)     3169 2024-04-05 11:42:03.000000 sbn-94/sbn/modules/udp.py
--rw-r--r--   0 bart      (1000) bart      (1000)     6154 2024-04-04 11:48:18.000000 sbn-94/sbn/object.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1814 2024-04-04 11:48:07.000000 sbn-94/sbn/parser.py
--rw-r--r--   0 bart      (1000) bart      (1000)     3435 2024-04-04 11:46:19.000000 sbn-94/sbn/persist.py
--rw-r--r--   0 bart      (1000) bart      (1000)      344 2024-04-04 11:47:29.000000 sbn-94/sbn/repeater.py
--rw-r--r--   0 bart      (1000) bart      (1000)     2029 2024-04-04 12:10:16.000000 sbn-94/sbn/thread.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1151 2024-04-04 11:46:52.000000 sbn-94/sbn/timer.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1235 2024-04-04 11:47:07.000000 sbn-94/sbn/utils.py
--rw-r--r--   0 bart      (1000) bart      (1000)      779 2024-04-04 12:09:42.000000 sbn-94/sbn/workdir.py
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-05 13:12:56.596583 sbn-94/sbn.egg-info/
--rw-r--r--   0 bart      (1000) bart      (1000)     2495 2024-04-05 13:12:56.000000 sbn-94/sbn.egg-info/PKG-INFO
--rw-r--r--   0 bart      (1000) bart      (1000)     1536 2024-04-05 13:12:56.000000 sbn-94/sbn.egg-info/SOURCES.txt
--rw-r--r--   0 bart      (1000) bart      (1000)        1 2024-04-05 13:12:56.000000 sbn-94/sbn.egg-info/dependency_links.txt
--rw-r--r--   0 bart      (1000) bart      (1000)       45 2024-04-05 13:12:56.000000 sbn-94/sbn.egg-info/entry_points.txt
--rw-r--r--   0 bart      (1000) bart      (1000)        7 2024-04-05 13:12:56.000000 sbn-94/sbn.egg-info/requires.txt
--rw-r--r--   0 bart      (1000) bart      (1000)        4 2024-04-05 13:12:56.000000 sbn-94/sbn.egg-info/top_level.txt
--rw-r--r--   0 bart      (1000) bart      (1000)        1 2024-04-05 13:12:56.000000 sbn-94/sbn.egg-info/zip-safe
--rw-r--r--   0 bart      (1000) bart      (1000)       38 2024-04-05 13:12:56.600584 sbn-94/setup.cfg
--rw-r--r--   0 bart      (1000) bart      (1000)      192 2024-04-05 12:12:33.000000 sbn-94/setup.py
+drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2024-05-12 05:56:48.304195 sbn-95/
+-rw-r--r--   0 bart      (1000) bart      (1001)     2494 2024-05-12 05:56:48.304195 sbn-95/PKG-INFO
+-rw-r--r--   0 bart      (1000) bart      (1001)     1932 2024-05-12 05:45:59.000000 sbn-95/README.rst
+drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2024-05-12 05:56:48.300195 sbn-95/docs/
+-rw-r--r--   0 bart      (1000) bart      (1001)   180711 2024-05-12 05:07:36.000000 sbn-95/docs/ECHAabilify.png
+-rw-r--r--   0 bart      (1000) bart      (1001)   193757 2024-05-12 05:07:36.000000 sbn-95/docs/ECHAclozapine.png
+-rw-r--r--   0 bart      (1000) bart      (1001)   197697 2024-05-12 05:07:36.000000 sbn-95/docs/ECHAhaldol.png
+-rw-r--r--   0 bart      (1000) bart      (1001)   232313 2024-05-12 05:07:36.000000 sbn-95/docs/ECHAzyprexa.png
+-rw-r--r--   0 bart      (1000) bart      (1001)   245670 2024-05-12 05:07:36.000000 sbn-95/docs/OTP1.png
+-rw-r--r--   0 bart      (1000) bart      (1001)   238095 2024-05-12 05:07:36.000000 sbn-95/docs/OTP2.png
+drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2024-05-12 05:56:48.300195 sbn-95/docs/_static/
+-rw-r--r--   0 bart      (1000) bart      (1001)     1000 2024-05-12 05:07:36.000000 sbn-95/docs/_static/sbn.css
+drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2024-05-12 05:56:48.300195 sbn-95/docs/_templates/
+-rw-r--r--   0 bart      (1000) bart      (1001)      291 2024-05-12 05:07:36.000000 sbn-95/docs/_templates/base.rst
+-rw-r--r--   0 bart      (1000) bart      (1001)      543 2024-05-12 05:07:36.000000 sbn-95/docs/_templates/class.rst
+-rw-r--r--   0 bart      (1000) bart      (1001)      879 2024-05-12 05:07:36.000000 sbn-95/docs/_templates/mine.rst
+-rw-r--r--   0 bart      (1000) bart      (1001)      879 2024-05-12 05:07:36.000000 sbn-95/docs/_templates/module.rst
+-rw-r--r--   0 bart      (1000) bart      (1001)     1178 2024-05-12 05:17:00.000000 sbn-95/docs/about.rst
+-rw-r--r--   0 bart      (1000) bart      (1001)   130021 2024-05-12 05:07:36.000000 sbn-95/docs/arrest.png
+-rw-r--r--   0 bart      (1000) bart      (1001)   256520 2024-05-12 05:07:36.000000 sbn-95/docs/banner.png
+-rw-r--r--   0 bart      (1000) bart      (1001)  1685507 2024-05-12 05:07:36.000000 sbn-95/docs/bevestigd.jpg
+-rw-r--r--   0 bart      (1000) bart      (1001)     3644 2024-05-12 05:18:53.000000 sbn-95/docs/conf.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      600 2024-05-12 05:17:00.000000 sbn-95/docs/evidence.rst
+-rw-r--r--   0 bart      (1000) bart      (1001)    47740 2024-05-12 05:07:36.000000 sbn-95/docs/genocide.png
+-rw-r--r--   0 bart      (1000) bart      (1001)      364 2024-05-12 05:17:00.000000 sbn-95/docs/guilty.rst
+-rw-r--r--   0 bart      (1000) bart      (1001)     2153 2024-05-12 05:17:00.000000 sbn-95/docs/index.rst
+-rw-r--r--   0 bart      (1000) bart      (1001)    69979 2024-05-12 05:07:36.000000 sbn-95/docs/informed.jpg
+-rw-r--r--   0 bart      (1000) bart      (1001)   228393 2024-05-12 05:07:36.000000 sbn-95/docs/kamer.png
+-rw-r--r--   0 bart      (1000) bart      (1001)     3457 2024-05-12 05:49:11.000000 sbn-95/docs/manual.rst
+drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2024-05-12 05:56:48.300195 sbn-95/docs/pdf/
+-rw-r--r--   0 bart      (1000) bart      (1001)   225470 2024-05-12 05:07:36.000000 sbn-95/docs/pdf/EM_Ack_OTP-CR-117_19.pdf
+-rw-r--r--   0 bart      (1000) bart      (1001)   238330 2024-05-12 05:07:36.000000 sbn-95/docs/pdf/EM_T04_OTP-CR-117_19.pdf
+-rw-r--r--   0 bart      (1000) bart      (1001)   236671 2024-05-12 05:07:36.000000 sbn-95/docs/pdf/EM_T07_OTP-CR-117_19_001.pdf
+-rw-r--r--   0 bart      (1000) bart      (1001)    41559 2024-05-12 05:07:36.000000 sbn-95/docs/pdf/Kamer.pdf
+-rw-r--r--   0 bart      (1000) bart      (1001)   323490 2024-05-12 05:07:36.000000 sbn-95/docs/pdf/Rome-Statute.pdf
+-rw-r--r--   0 bart      (1000) bart      (1001)    50044 2024-05-12 05:07:36.000000 sbn-95/docs/pdf/bevestigd.pdf
+-rw-r--r--   0 bart      (1000) bart      (1001)     2196 2024-05-12 05:17:00.000000 sbn-95/docs/request.rst
+-rw-r--r--   0 bart      (1000) bart      (1001)   179869 2024-05-12 05:07:36.000000 sbn-95/docs/skull.jpg
+-rw-r--r--   0 bart      (1000) bart      (1001)   287102 2024-05-12 05:07:36.000000 sbn-95/docs/skull3.png
+-rw-r--r--   0 bart      (1000) bart      (1001)      841 2024-05-12 05:20:24.000000 sbn-95/docs/source.rst
+-rw-r--r--   0 bart      (1000) bart      (1001)      176 2024-05-12 05:17:00.000000 sbn-95/docs/verbatim.rst
+-rw-r--r--   0 bart      (1000) bart      (1001)   256611 2024-05-12 05:51:27.000000 sbn-95/docs/verbatim6.png
+-rw-r--r--   0 bart      (1000) bart      (1001)    46476 2024-05-12 05:07:36.000000 sbn-95/docs/wallpaper.png
+-rw-r--r--   0 bart      (1000) bart      (1001)     1183 2024-05-12 05:17:00.000000 sbn-95/docs/writings.rst
+-rw-r--r--   0 bart      (1000) bart      (1001)     2102 2024-05-12 05:55:43.000000 sbn-95/pyproject.toml
+drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2024-05-12 05:56:48.300195 sbn-95/sbn/
+-rw-r--r--   0 bart      (1000) bart      (1001)       62 2024-05-12 05:08:36.000000 sbn-95/sbn/__init__.py
+-rwxr-xr-x   0 bart      (1000) bart      (1001)     3913 2024-05-12 05:37:03.000000 sbn-95/sbn/__main__.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      704 2024-05-12 05:08:36.000000 sbn-95/sbn/broker.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     4219 2024-05-12 05:08:36.000000 sbn-95/sbn/client.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     2328 2024-05-12 05:08:36.000000 sbn-95/sbn/disk.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     1954 2024-05-12 05:08:36.000000 sbn-95/sbn/find.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     2110 2024-05-12 05:08:36.000000 sbn-95/sbn/handler.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      490 2024-05-12 05:08:36.000000 sbn-95/sbn/log.py
+drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2024-05-12 05:56:48.304195 sbn-95/sbn/modules/
+-rw-r--r--   0 bart      (1000) bart      (1001)      355 2024-05-12 05:08:41.000000 sbn-95/sbn/modules/__init__.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      190 2024-05-12 05:08:41.000000 sbn-95/sbn/modules/cmd.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      351 2024-05-12 05:08:41.000000 sbn-95/sbn/modules/err.py
+-rw-r--r--   0 bart      (1000) bart      (1001)    18777 2024-05-12 05:08:41.000000 sbn-95/sbn/modules/irc.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      694 2024-05-12 05:08:41.000000 sbn-95/sbn/modules/log.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      385 2024-05-12 05:08:41.000000 sbn-95/sbn/modules/mod.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     2354 2024-05-12 05:08:41.000000 sbn-95/sbn/modules/req.py
+-rw-r--r--   0 bart      (1000) bart      (1001)    10762 2024-05-12 05:08:41.000000 sbn-95/sbn/modules/rss.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     1123 2024-05-12 05:08:41.000000 sbn-95/sbn/modules/tdo.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      991 2024-05-12 05:08:41.000000 sbn-95/sbn/modules/thr.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     5163 2024-05-12 05:08:41.000000 sbn-95/sbn/modules/tmr.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     6168 2024-05-12 05:08:36.000000 sbn-95/sbn/object.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     1421 2024-05-12 05:08:36.000000 sbn-95/sbn/run.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     4209 2024-05-12 05:08:36.000000 sbn-95/sbn/thread.py
+drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2024-05-12 05:56:48.300195 sbn-95/sbn.egg-info/
+-rw-r--r--   0 bart      (1000) bart      (1001)     2494 2024-05-12 05:56:48.000000 sbn-95/sbn.egg-info/PKG-INFO
+-rw-r--r--   0 bart      (1000) bart      (1001)     1327 2024-05-12 05:56:48.000000 sbn-95/sbn.egg-info/SOURCES.txt
+-rw-r--r--   0 bart      (1000) bart      (1001)        1 2024-05-12 05:56:48.000000 sbn-95/sbn.egg-info/dependency_links.txt
+-rw-r--r--   0 bart      (1000) bart      (1001)       74 2024-05-12 05:56:48.000000 sbn-95/sbn.egg-info/entry_points.txt
+-rw-r--r--   0 bart      (1000) bart      (1001)        7 2024-05-12 05:56:48.000000 sbn-95/sbn.egg-info/requires.txt
+-rw-r--r--   0 bart      (1000) bart      (1001)        4 2024-05-12 05:56:48.000000 sbn-95/sbn.egg-info/top_level.txt
+-rw-r--r--   0 bart      (1000) bart      (1001)        1 2024-05-12 05:56:48.000000 sbn-95/sbn.egg-info/zip-safe
+-rw-r--r--   0 bart      (1000) bart      (1001)       38 2024-05-12 05:56:48.304195 sbn-95/setup.cfg
+-rw-r--r--   0 bart      (1000) bart      (1001)      192 2024-05-12 05:07:36.000000 sbn-95/setup.py
```

### Comparing `sbn-94/PKG-INFO` & `sbn-95/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbn
-Version: 94
+Version: 95
 Summary: Skull, Bones and Number (OTP-CR-117/19)
 Author-email: Bart Thate <bthate@dds.nl>
 License: Public Domain
 Project-URL: home, https://pypi.org/project/sbn
 Project-URL: bugs, https://github.com/bthate/sbn/issues
 Project-URL: source, https://github.com/bthate/sbn
 Classifier: Development Status :: 3 - Alpha
@@ -15,20 +15,19 @@
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
 
 | **Information and Evidence Unit**
 | **Office of the Prosecutor**
 | **Post Office Box 19519**
 | **2500 CM The Hague**
-| **The Netherlands** ``OTP-CR-117/19``
-|
+| **The Netherlands** 
 |
 
 
-Hello Office of the Prosecutor,
+Hello Office of the Prosecutor, ``OTP-CR-117/19``
 
 i write you in the context of communications and claims under art.15 of 
 the Rome Statute. i want to inform the prosecutor that the king of the 
 netherlands and his government are commiting 3 of the 5 crimes defined 
 in the Rome Statute.
 
 The dutch government has introduced three new forced care laws, the Wfz
```

### Comparing `sbn-94/README.rst` & `sbn-95/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 | **Information and Evidence Unit**
 | **Office of the Prosecutor**
 | **Post Office Box 19519**
 | **2500 CM The Hague**
-| **The Netherlands** ``OTP-CR-117/19``
-|
+| **The Netherlands** 
 |
 
 
-Hello Office of the Prosecutor,
+Hello Office of the Prosecutor, ``OTP-CR-117/19``
 
 i write you in the context of communications and claims under art.15 of 
 the Rome Statute. i want to inform the prosecutor that the king of the 
 netherlands and his government are commiting 3 of the 5 crimes defined 
 in the Rome Statute.
 
 The dutch government has introduced three new forced care laws, the Wfz
```

### Comparing `sbn-94/docs/ECHAabilify.png` & `sbn-95/docs/ECHAabilify.png`

 * *Files identical despite different names*

### Comparing `sbn-94/docs/ECHAclozapine.png` & `sbn-95/docs/ECHAclozapine.png`

 * *Files identical despite different names*

### Comparing `sbn-94/docs/ECHAhaldol.png` & `sbn-95/docs/ECHAhaldol.png`

 * *Files identical despite different names*

### Comparing `sbn-94/docs/ECHAzyprexa.png` & `sbn-95/docs/ECHAzyprexa.png`

 * *Files identical despite different names*

### Comparing `sbn-94/docs/OTP1.png` & `sbn-95/docs/OTP1.png`

 * *Files identical despite different names*

### Comparing `sbn-94/docs/OTP2.png` & `sbn-95/docs/OTP2.png`

 * *Files identical despite different names*

### Comparing `sbn-94/docs/_static/sbn.css` & `sbn-95/docs/_static/sbn.css`

 * *Files identical despite different names*

### Comparing `sbn-94/docs/_templates/class.rst` & `sbn-95/docs/_templates/class.rst`

 * *Files identical despite different names*

### Comparing `sbn-94/docs/_templates/mine.rst` & `sbn-95/docs/_templates/mine.rst`

 * *Files identical despite different names*

### Comparing `sbn-94/docs/_templates/module.rst` & `sbn-95/docs/_templates/module.rst`

 * *Files identical despite different names*

### Comparing `sbn-94/docs/about.rst` & `sbn-95/docs/about.rst`

 * *Files 17% similar despite different names*

```diff
@@ -1,30 +1,20 @@
 .. _about:
 
-
 .. raw:: html
 
-    <center>
-    <i>
-    By law, with the use of poison,
-    killing, torturing, castrating, destroying,
-    in whole or in part,
-    all elderly and all handicapped (Wzd), all criminals (Wfz)
-    and all psychiatric patients (WvGGZ)
-    here in the Netherlands
-    </i>
-    </center>
     <br>
 
+.. title:: About
 
-.. raw:: html
 
-    <br><br>
+.. raw:: html
 
-.. title:: About
+    <center><b>ABOUT</b></center>
+    <br>
 
 
 In 2018 i informed the king of the netherlands that what he calls
 medicine in his "care" laws are not medicine but poison. Proof of
 these medicine being poison were shown to the king, who's (personal)
 kabinet wrote back that "the king took note of what i have written".
```

### Comparing `sbn-94/docs/arrest.png` & `sbn-95/docs/arrest.png`

 * *Files identical despite different names*

### Comparing `sbn-94/docs/banner.png` & `sbn-95/docs/banner.png`

 * *Files identical despite different names*

### Comparing `sbn-94/docs/bevestigd.jpg` & `sbn-95/docs/bevestigd.jpg`

 * *Files identical despite different names*

### Comparing `sbn-94/docs/conf.py` & `sbn-95/docs/conf.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # This file is placed in the Public Domain.
 # -*- coding: utf-8 -*-
 #
 # pylint: disable=C,I,R
 # ruff: noqa: E402, E501
 
 
-"Skull, Bones and Number (OTP-CR-117/19)"
+"@KarimKhanQC reconsider OTP-CR-117/19"
 
 
 NAME = "sbn"
-VERSION = "41"
+VERSION = "95"
 
 
 import os
 import sys
 
 
 sys.setrecursionlimit(1500)
@@ -56,15 +56,15 @@
               'sphinx.ext.githubpages'
              ]
 
 
 # -- Options for HTML output -------------------------------------------------
 
 
-html_title = "Skull, Bones and Number (OTP-CR-117/19)"
+html_title = "@KarimKhanQC reconsider OTP-CR-117/19"
 html_style = 'sbn.css'
 html_static_path = ["_static"]
 html_css_files = ["sbn.css",]
 html_short_title = "%s %s" % (NAME, VERSION)
 html_sidebars = {
     '**': [
         'about.html',
@@ -109,25 +109,43 @@
 intersphinx_cache_limit = 1
 
 
 rst_prolog = '''.. image:: genocide.png
     :width: 100%
     :height: 2.6cm
     :target: index.html
+
+.. raw:: html
+
+    <center>
+    <i>
+    By law, with the use of poison, killing, torturing, castrating, destroying in whole or in part,
+    </i>
+    </center>
+    <center>
+    <i>
+    all elderly and all handicapped (Wzd), all criminals (Wfz) and all psychiatric patients (WvGGZ)
+    </i>
+    </center>
+    <center>
+    <i>
+    here in the Netherlands.
+    </i>
+    </center>
 '''
 
 rst_epilog = '''.. raw:: html
 
     <br>
     <br>
     <br>
     <center>
     <b>
 
-:ref:`about <about>` - :ref:`writings <writings>` - :ref:`evidence <evidence>` - :ref:`guilty <guilty>` - :ref:`reconsider <reconsider>`
+:ref:`about <about>` - :ref:`writings <writings>` - :ref:`evidence <evidence>` - :ref:`guilty <guilty>` - :ref:`reconsider <reconsider>` - :ref:`manual <manual>`
 
 
 .. raw:: html
 
     </b>
     </center>
```

### Comparing `sbn-94/docs/evidence.rst` & `sbn-95/docs/evidence.rst`

 * *Files 7% similar despite different names*

```diff
@@ -3,14 +3,20 @@
 .. raw:: html
 
     <br>
 
 .. title:: Evidence
 
 
+.. raw:: html
+
+    <center><b>EVIDENCE</b></center>
+    <br>
+
+
 .. _haldol:
 
 
 **HALDOL**
 
 
 .. raw:: html
```

### Comparing `sbn-94/docs/genocide.png` & `sbn-95/docs/genocide.png`

 * *Files identical despite different names*

### Comparing `sbn-94/docs/index.rst` & `sbn-95/docs/index.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,37 @@
 .. _reconsider:
 
 
 .. raw:: html
 
     <br>
 
-
 .. title:: Reconsider
 
 
+.. raw:: html
+
+    <center><b>RECONSIDER</b></center>
+    <br>
+
+
 | **Information and Evidence Unit**
 | **Office of the Prosecutor**
 | **Post Office Box 19519**
 | **2500 CM The Hague**
 | **The Netherlands** 
 |
 
+
 Hello Office of the Prosecutor, ``OTP-CR-117/19``
 
 i write you in the context of communications and claims under art.15 of 
 the Rome Statute. i want to inform the prosecutor that the king of the 
 netherlands and his government are commiting 3 of the 5 crimes defined 
-in the Rome Statute.
+in the Rome Statute. 
 
 The dutch government has introduced three new forced care laws, the Wfz 
 (wet forensische zorg) for criminals, the WvGGZ (Wet verplichte GGZ) for 
 the disturbed and addicted and the Wzd (Wet zorg en dwang) for the 
 handicapped.
 
 Both the chamber suggesting these laws to the king and the king himself
```

### Comparing `sbn-94/docs/informed.jpg` & `sbn-95/docs/informed.jpg`

 * *Files identical despite different names*

### Comparing `sbn-94/docs/kamer.png` & `sbn-95/docs/kamer.png`

 * *Files identical despite different names*

### Comparing `sbn-94/docs/manual.rst` & `sbn-95/docs/manual.rst`

 * *Files 13% similar despite different names*

```diff
@@ -1,65 +1,70 @@
 .. _manual:
 
-
 .. raw:: html
 
     <br>
 
 .. title:: Manual
 
 
+.. raw:: html
+
+    <center><b>MANUAL</b></center>
+    <br>
+
 **NAME**
 
-    **SBN** - Skull, Bones and Number (OTP-CR-117/19)
+    ``SBN``  --  Skull, Bones and Number (OTP-CR-117/19)
 
 
 **INSTALL**
 
 
 ::
 
     $ pipx install sbn
+    $ pipx ensurepath
 
 
 **SYNOPSIS**
 
 ::
 
-    sbn <cmd> [key=val] [key==val]
-    sbn [-a] [-c] [-d] [-v]
+    sbn  <cmd> [key=val] [key==val]
+    sbn  [-a] [-c] [-v]
+    sbnd [-v]
 
 
 **DESCRIPTION**
 
-    **SBN** holds evidence that king
+    ``SBN`` holds evidence that king
     netherlands is doing a genocide, a
     written response where king
     netherlands confirmed taking note
     of “what i have written”, namely
     :ref:`proof  <evidence>` that medicine
     he uses in treatement laws like zyprexa,
     haldol, abilify and clozapine are
     poison that make impotent, is both
     physical (contracted muscles) and
     mental (make people hallucinate)
     torture and kills members of the
     victim groups :ref:`. <source>`
 
-    **SBN** contains :ref:`correspondence <writings>`
-    with the International Criminal Court,
-    asking for arrest of the king of
-    the netherlands, for the genocide
-    he is committing with his new
-    treatement laws.
-
-    Current status is "no basis to proceed" 
-    :ref:`judgement <guilty>` of the prosecutor
-    which requires a "basis to prosecute" to
-    have the king actually arrested.
+    ``SBN`` contains :ref:`correspondence
+    <writings>` with the International Criminal
+    Court, asking for arrest of the king of the
+    netherlands, for the genocide he is committing
+    with his new treatement laws.
+
+    Current status is a :ref:`"no basis to proceed"
+    <writings>` judgement of the prosecutor which
+    requires a :ref:`"basis to prosecute" <reconsider>`
+    to have the king actually arrested.
 
 
 **USAGE**
 
     without any argument the bot does nothing
 
     ::
@@ -68,30 +73,30 @@
         $
 
     see list of commands
 
     ::
 
         $ sbn cmd
-        cfg,cmd,mre,now,pwd
+        cmd,dne,err,log,mod,req,tdo,thr,tmr
 
 
     start a console
 
     ::
 
         $ sbn -c 
         >
 
     use -v for verbose
 
     ::
 
         $ sbn -cv
-        SBN started CV started Sat Dec 2 17:53:24 2023
+        May 12 05:51:49 2024 GENOCIDE CV CMD,ERR,LOG,MOD,REQ,TDO,THR,TMR
         >
 
     start daemon
 
     ::
 
         $ sbnd
@@ -105,21 +110,14 @@
         $ sbn req
         Information and Evidence Unit
         Office of the Prosecutor
         Post Office Box 19519
         2500 CM The Hague
         The Netherlands
 
-    show how many died in the WvGGZ
-
-    ::
-
-        $ sbn now
-        4y18d patient #47324 died from mental illness (14/32/11682) every 44m59s
-    
 
 **CONFIGURATION**
 
     irc
 
     ::
 
@@ -144,38 +142,39 @@
         $ sbn nme <url> <name>
 
 
 **COMMANDS**
 
     ::
 
+        cfg - irc configuration
         cmd - commands
-        mod - show modules
-        now - show genocide stats
+        mre - displays cached output
+        pwd - sasl nickserv name/pass
         req - reconsider
 
 
 **SYSTEMD**
 
-    save the following it in /etc/systems/system/sbn.service
+    save the following it in /etc/systemd/system/sbn.service
     and replace "<user>" with the user running pipx
 
     ::
  
         [Unit]
         Description=Skull, Bones and Number (OTP-CR-117/19)
         Requires=network-online.target
         After=network-online.target
 
         [Service]
         Type=simple
         User=<user>
         Group=<user>
         WorkingDirectory=/home/<user>/.sbn
-        ExecStart=/home/<user>/.local/pipx/venvs/sbn/bin/sbn -d
+        ExecStart=/home/<user>/.local/pipx/venvs/sbn/bin/sbnd
         RemainAfterExit=yes
 
         [Install]
         WantedBy=default.target
 
 
     then run this
@@ -184,34 +183,34 @@
 
         $ mkdir ~/.sbn
         $ sudo systemctl enable sbn --now
 
     default channel/server is #sbn on localhost
 
 
+**SOURCE**
+
+    source is :ref:`here <source>`
+
+
 **FILES**
 
     ::
 
         ~/.sbn
         ~/.local/bin/sbn
+        ~/.local/bin/sbnd
         ~/.local/pipx/venvs/sbn/
 
 
-**SOURCE**
-
-
-   source code is :ref:`here <source>`
-
-
 **AUTHOR**
 
     ::
 
-        OTP-CR-117/19  <skullbonesandnumber@gmail.com>
+        Bart Thate <bthate@dds.nl>
 
 
 **COPYRIGHT**
 
     ::
 
         SBN is Public Domain.
```

### Comparing `sbn-94/docs/pdf/EM_T04_OTP-CR-117_19.pdf` & `sbn-95/docs/pdf/EM_T04_OTP-CR-117_19.pdf`

 * *Files identical despite different names*

### Comparing `sbn-94/docs/pdf/EM_T07_OTP-CR-117_19_001.pdf` & `sbn-95/docs/pdf/EM_T07_OTP-CR-117_19_001.pdf`

 * *Files identical despite different names*

### Comparing `sbn-94/docs/pdf/Kamer.pdf` & `sbn-95/docs/pdf/Kamer.pdf`

 * *Files identical despite different names*

### Comparing `sbn-94/docs/pdf/Rome-Statute.pdf` & `sbn-95/docs/pdf/Rome-Statute.pdf`

 * *Files identical despite different names*

### Comparing `sbn-94/docs/pdf/bevestigd.pdf` & `sbn-95/docs/pdf/bevestigd.pdf`

 * *Files identical despite different names*

### Comparing `sbn-94/docs/request.rst` & `sbn-95/docs/request.rst`

 * *Files identical despite different names*

### Comparing `sbn-94/docs/skull.jpg` & `sbn-95/docs/skull.jpg`

 * *Files identical despite different names*

### Comparing `sbn-94/docs/skull3.png` & `sbn-95/docs/skull3.png`

 * *Files identical despite different names*

### Comparing `sbn-94/docs/wallpaper.png` & `sbn-95/docs/wallpaper.png`

 * *Files identical despite different names*

### Comparing `sbn-94/docs/writings.rst` & `sbn-95/docs/writings.rst`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,20 @@
 .. raw:: html
 
     <br>
 
 .. title:: Writings
 
 
+.. raw:: html
+
+    <center><b>WRITINGS</b></center>
+    <br>
+
+
 **EMAIL 1**
 
 
 |
 | **From**: Bart Thate <bthate@dds.nl>
 | **To**: otp.informationdesk@icc-cpi.int
 | **Subject**: Information that the king of the netherlands is aware that the medicine administered with the use of new defines laws are proven to be poison and is commiting 3 of 5 genocide crimes on parts of the population here in the netherlands
```

### Comparing `sbn-94/pyproject.toml` & `sbn-95/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["setuptools>=43.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "sbn"
 description = "Skull, Bones and Number (OTP-CR-117/19)"
-version = "94"
+version = "95"
 authors = [
     {name = "Bart Thate", email = "bthate@dds.nl" },
 ]
 readme = "README.rst"
 license = { text="Public Domain"}
 classifiers=[
     'Development Status :: 3 - Alpha',
@@ -20,15 +20,16 @@
     'Topic :: Utilities'
 ]
 
 [project.optional-dependencies]
 dev = []
 
 [project.scripts]
-"sbn" = "sbn.__main__:wrapped"
+"sbn"  = "sbn.__main__:wrapped"
+"sbnd" = "sbn.__main__:daemoned"
 
 
 [project.urls]
 "home" = "https://pypi.org/project/sbn"
 "bugs" = "https://github.com/bthate/sbn/issues"
 "source" = "https://github.com/bthate/sbn"
 
@@ -40,54 +41,53 @@
 ]
 zip-safe = true
 
 
 [tool.setuptools.data-files]
 "share/doc/sbn" = [
     "README.rst",
-    "MANUAL.rst",
     "docs/about.rst",
     "docs/arrest.png",
     "docs/conf.py",
     "docs/ECHAhaldol.png",
     "docs/evidence.rst",
     "docs/genocide.png",
     "docs/informed.jpg",
     "docs/OTP1.png",
     "docs/skull.jpg",
     "docs/source.rst",
-    "docs/verbatim2.png",
+    "docs/verbatim6.png",
     "docs/banner.png",
     "docs/ECHAabilify.png",
     "docs/ECHAzyprexa.png",
     "docs/guilty.rst",
     "docs/kamer.png",
     "docs/OTP2.png",
     "docs/request.rst",
     "docs/skull3.png",
     "docs/verbatim.rst",
     "docs/writings.rst",
     "docs/bevestigd.jpg",
     "docs/ECHAclozapine.png",
     "docs/wallpaper.png",
     "docs/index.rst",
-    "docs/manual.rst",
-    "docs/wallpaper.png",
+    "docs/manual.rst"
 ]
 
 "share/doc/sbn/_static" = [
     "docs/_static/sbn.css",
 ]
 
 "share/doc/sbn/pdf" =  [
     "docs/pdf/bevestigd.pdf",
+    "docs/pdf/EM_Ack_OTP-CR-117_19.pdf",
     "docs/pdf/EM_T04_OTP-CR-117_19.pdf",
     "docs/pdf/EM_T07_OTP-CR-117_19_001.pdf",
     "docs/pdf/Kamer.pdf",
-    "docs/pdf/Rome-Statute.pdf",
+    "docs/pdf/Rome-Statute.pdf"
 ]
 
 "share/doc/sbn/_templates" = [
     "docs/_templates/base.rst",
     "docs/_templates/class.rst",
     "docs/_templates/mine.rst",
     "docs/_templates/module.rst"
```

### Comparing `sbn-94/sbn/__main__.py` & `sbn-95/sbn/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,173 +1,169 @@
 # This file is placed in the Public Domain.
 #
-# pylint: disable=C,R,W0105,W0212
-# ruff: noqa: E402
+# pylint: disable=C0413,W0212,W0611
 
 
 "main"
 
 
 import getpass
 import os
+import pathlib
 import pwd
+import readline
 import sys
 import termios
 import time
 
 
-from .client  import Client, cmnd
-from .default import Default
-from .errors  import Errors,debug
-from .event   import Event
-from .object  import cdir
-from .parser  import parse_cmd
-from .utils   import spl
-from .workdir import Workdir
-
-
-from . import modules
-
-Cfg          = Default()
-Cfg.mod      = "cmd,mod"
-Cfg.name     = sys.argv[0].split(os.sep)[-2]
-Cfg.dir      = os.path.expanduser(f"~/.{Cfg.name}")
-Cfg.pidfile  = os.path.join(Cfg.wd, f"{Cfg.name}.pid")
-Workdir.workdir = Cfg.dir
+sys.path.insert(0, os.getcwd())
 
 
-dte = time.ctime(time.time()).replace("  ", " ")
-ext = os._exit 
+from sbn.client  import Client, cmnd, parse
+from sbn.disk    import Workdir, skel
+from sbn.handler import Event
+from sbn.log     import debug, enable
+from sbn.object  import Default
+from sbn.run     import broker, init, scan
+from sbn.thread  import errors, setout
+
+
+from sbn import modules
+
+
+Cfg             = Default()
+Cfg.dis         = ""
+Cfg.mod         = "cmd,err,log,mod,req,tdo,thr,tmr"
+Cfg.opts        = ""
+Cfg.name        = "sbn"
+Cfg.version     = "95"
+Cfg.wdr         = os.path.expanduser(f"~/.{Cfg.name}")
+Cfg.pidfile     = os.path.join(Cfg.wdr, f"{Cfg.name}.pid")
+
+
+Workdir.workdir = Cfg.wdr
 
 
 class Console(Client):
 
     "Console"
 
+    def __init__(self):
+        Client.__init__(self)
+        broker.add(self)
+
     def announce(self, txt):
-        "blind announce"
+        "disable announce."
 
     def callback(self, evt):
-        "run and wait for callback to finish."
+        "wait for callback."
         Client.callback(self, evt)
-        evt.wait(5.0)
+        evt.wait()
 
     def poll(self):
-        "reconstruct event from input."
+        "poll console and create event."
         evt = Event()
         evt.orig = object.__repr__(self)
         evt.txt = input("> ")
         evt.type = "command"
         return evt
 
     def say(self, _channel, txt):
-        "say text in channel."
+        "print to console"
         txt = txt.encode('utf-8', 'replace').decode()
         print(txt)
 
 
 def daemon(pidfile, verbose=False):
-    "fork into the background."
+    "switch to background."
     pid = os.fork()
     if pid != 0:
-        ext(0)
+        os._exit(0)
     os.setsid()
     pid2 = os.fork()
     if pid2 != 0:
-        ext(0)
+        os._exit(0)
     if not verbose:
         with open('/dev/null', 'r', encoding="utf-8") as sis:
             os.dup2(sis.fileno(), sys.stdin.fileno())
         with open('/dev/null', 'a+', encoding="utf-8") as sos:
             os.dup2(sos.fileno(), sys.stdout.fileno())
         with open('/dev/null', 'a+', encoding="utf-8") as ses:
             os.dup2(ses.fileno(), sys.stderr.fileno())
     os.umask(0)
     os.chdir("/")
     if os.path.exists(pidfile):
         os.unlink(pidfile)
-    cdir(os.path.dirname(pidfile))
+    path = pathlib.Path(pidfile)
+    path.parent.mkdir(parents=True, exist_ok=True)
     with open(pidfile, "w", encoding="utf-8") as fds:
         fds.write(str(os.getpid()))
 
 
-def init(pkg, modstr, disable=""):
-    "start inits in modules."
-    mds = []
-    for modname in spl(modstr):
-        if modname in spl(disable):
-            continue
-        module = getattr(pkg, modname, None)
-        if not module:
-            continue
-        if "init" in dir(module):
-            module.init()
-            mds.append(module)
-    return mds
+def daemoned():
+    "run in background"
+    Cfg.opts += "d"
+    main()
 
 
 def privileges(username):
-    "lower privileges."
+    "drop privileges."
     pwnam = pwd.getpwnam(username)
     os.setgid(pwnam.pw_gid)
     os.setuid(pwnam.pw_uid)
 
 
 def wrap(func):
-    "restore terminal"
+    "restore console."
     old2 = None
     try:
         old2 = termios.tcgetattr(sys.stdin.fileno())
     except termios.error:
         pass
     try:
         func()
     except (KeyboardInterrupt, EOFError):
         print("")
     finally:
         if old2:
             termios.tcsetattr(sys.stdin.fileno(), termios.TCSADRAIN, old2)
 
 
-"runtime"
-
-
 def main():
-    "main code"
-    Workdir.skel()
-    Errors.enable(print)
-    parse_cmd(Cfg, " ".join(sys.argv[1:]))
-    result = None
-    if 'a' in Cfg.opts:
-        Cfg.mod = "," + ",".join(modules.__dir__())
+    "main"
+    parse(Cfg, " ".join(sys.argv[1:]))
+    skel()
+    if not "d" in Cfg.opts:
+        enable(print)
+        setout(print)
+    if "a" in Cfg.opts:
+        Cfg.mod = ",".join(modules.__dir__())
     if "v" in Cfg.opts:
-        debug(f"{Cfg.name.upper()} {Cfg.opts.upper()} started {dte}")
+        dte = " ".join(time.ctime(time.time()).replace("  ", " ").split()[1:])
+        debug(f'{dte} {Cfg.name.upper()} {Cfg.opts.upper()} {Cfg.mod.upper()}')
     if "h" in Cfg.opts:
         print(__doc__)
-        return result
     if "d" in Cfg.opts:
-        Cfg.mod = ",".join(modules.__dir__())
+        Cfg.mod  = ",".join(dir(modules))
         Cfg.user = getpass.getuser()
-        daemon(Cfg.pidfile, "v" in Cfg.opts)
+        daemon(Cfg.pidfile, "-v" in sys.argv)
         privileges(Cfg.user)
+        scan(modules, Cfg.mod)
         init(modules, Cfg.mod)
         while 1:
             time.sleep(1.0)
-    elif "c" in Cfg.opts:
-        init(modules, Cfg.mod)
+        return
+    scan(modules, Cfg.mod, Cfg.sets.dis)
+    if "c" in Cfg.opts:
+        init(modules, Cfg.mod, Cfg.sets.dis)
         csl = Console()
         csl.start()
         while 1:
             time.sleep(1.0)
     elif Cfg.otxt:
         cmnd(Cfg.otxt, print)
-    return result
-
-
-def wrapped():
-    "wrapped code"
-    wrap(main)
-    Errors.show()
 
 
 if __name__ == "__main__":
-    wrapped()
+    main()
+    errors()
```

### Comparing `sbn-94/sbn/handler.py` & `sbn-95/sbn/handler.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,55 +1,51 @@
 # This file is placed in the Public Domain.
-#
-# pylint: disable=C,R,W0105,W0212,W0718
 
 
 "handler"
 
 
 import queue
 import threading
 import _thread
 
 
-from .errors  import Errors
-from .object  import Object
-from .thread  import launch
+from .object import Default, Object
+from .thread import launch
+
+
+rpr = object.__repr__
 
 
 class Handler:
 
     "Handler"
 
     def __init__(self):
-        self.cbs = Object()
+        self.cbs      = Object()
         self.queue    = queue.Queue()
         self.stopped  = threading.Event()
         self.threaded = True
 
     def callback(self, evt):
         "call callback based on event type."
         func = getattr(self.cbs, evt.type, None)
-        if func:
-            if self.threaded:
-                evt._thr = launch(func, evt)
-            else:
-                func(evt)
+        if not func:
+            evt.ready()
+            return
+        evt._thr = launch(func, self, evt) # pylint: disable=W0212
 
     def loop(self):
         "proces events until interrupted."
         while not self.stopped.is_set():
             try:
                 evt = self.poll()
                 self.callback(evt)
             except (KeyboardInterrupt, EOFError):
                 _thread.interrupt_main()
-            except Exception as ex:
-                Errors.add(ex)
-                evt.ready()
 
     def poll(self):
         "function to return event."
         return self.queue.get()
 
     def put(self, evt):
         "put event into the queue."
@@ -64,17 +60,42 @@
         launch(self.loop)
 
     def stop(self):
         "stop the event loop."
         self.stopped.set()
 
 
-"interface"
+class Event(Default): # pylint: disable=R0902
+
+    "Event"
+
+    def __init__(self):
+        Default.__init__(self)
+        self._thr    = None
+        self._ready  = threading.Event()
+        self.done    = False
+        self.orig    = None
+        self.result  = []
+        self.txt     = ""
+        self.type    = "event"
+
+    def ready(self):
+        "event is ready."
+        self._ready.set()
+
+    def reply(self, txt):
+        "add text to the result"
+        self.result.append(txt)
+
+    def wait(self):
+        "wait for event to be ready."
+        if self._thr:
+            self._thr.join()
+        self._ready.wait()
+        return self.result
 
 
 def __dir__():
     return (
-        'Handler',
+        'Event',
+        'Handler'
     )
-
-
-__all__ = __dir__()
```

### Comparing `sbn-94/sbn/modules/irc.py` & `sbn-95/sbn/modules/irc.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,8 @@
 # This file is placed in the Public Domain.
-#
-# pylint: disable=C,R,W0105,W0718
-# ruff: noqa: F841
 
 
 "internet relay chat"
 
 
 import base64
 import os
@@ -14,53 +11,52 @@
 import ssl
 import textwrap
 import threading
 import time
 import _thread
 
 
-from ..broker  import Broker
-from ..client  import Client
-from ..default import Default
-from ..event   import Event
-from ..errors  import Errors, debug
-from ..object  import Object, edit, fmt, keys
-from ..persist import Persist, last, sync
-from ..thread  import launch
+from ..client  import Client, command
+from ..disk    import sync, whitelist
+from ..find    import last
+from ..handler import Event
+from ..log     import Logging, debug
+from ..object  import Default, Object, edit, fmt, keys, values
+from ..run     import broker
+from ..thread  import later, launch
 
 
 NAME    = __file__.split(os.sep)[-3]
-get     = Broker.get
 saylock = _thread.allocate_lock()
 
 
-Errors.filter = ["PING", "PONG", "PRIVMSG"]
+Logging.filter = ["PING", "PONG", "PRIVMSG"]
 
 
 def init():
     "initialize a irc bot."
     irc = IRC()
     irc.start()
     irc.events.joined.wait()
     return irc
 
 
 def shutdown():
     "shutdown irc bot."
-    for bot in Broker.all():
-        if "irc" not in type(bot):
+    for bot in values(broker.objs):
+        if "irc" not in str(type(bot)).lower():
             continue
         debug(f"IRC stopping {repr(bot)}")
         bot.state.pongcheck = True
         bot.state.keeprunning = False
         bot.events.connected.clear()
         bot.stop()
 
 
-class Config(Default):
+class Config(Default): # pylint: disable=R0902,R0903
 
     "Config"
 
     channel = f'#{NAME}'
     commands = True
     control = '!'
     edited = time.time()
@@ -82,15 +78,15 @@
         self.nick = self.nick or Config.nick
         self.port = self.port or Config.port
         self.realname = self.realname or Config.realname
         self.server = self.server or Config.server
         self.username = self.username or Config.username
 
 
-Persist.add(Config)
+whitelist(Config)
 
 
 class TextWrap(textwrap.TextWrapper):
 
     "TextWrap"
 
     def __init__(self):
@@ -206,15 +202,15 @@
         self.register('CAP', cb_cap)
         self.register('ERROR', cb_error)
         self.register('LOG', cb_log)
         self.register('NOTICE', cb_notice)
         self.register('PRIVMSG', cb_privmsg)
         self.register('QUIT', cb_quit)
         self.register("366", cb_ready)
-        Broker.add(self)
+        broker.add(self)
 
     def announce(self, txt):
         "announce on all channels."
         for channel in self.channels:
             self.oput(channel, txt)
 
     def docommand(self, cmd, *args):
@@ -273,16 +269,16 @@
             self.sock.shutdown(2)
         except (
                 ssl.SSLError,
                 OSError,
                 BrokenPipeError
                ) as _ex:
             pass
-        except Exception as ex:
-            Errors.add(ex)
+        except Exception as ex: # pylint: disable=W0718
+            later(ex)
 
     def doconnect(self, server, nck, port=6667):
         "loop until connected."
         while 1:
             try:
                 if self.connect(server, port):
                     break
@@ -356,14 +352,15 @@
         self.events.authed.wait()
         self.direct(f'NICK {nck}')
         self.direct(f'USER {nck} {server} {server} {nck}')
 
 
     def parsing(self, txt):
         "parse text into an event."
+        # pylint: disable=R0912,R0915
         rawstr = str(txt)
         rawstr = rawstr.replace('\u0001', '')
         rawstr = rawstr.replace('\001', '')
         debug(txt)
         obj = Event()
         obj.args = []
         obj.rawstr = rawstr
@@ -433,15 +430,15 @@
                     OSError,
                     socket.timeout,
                     ssl.SSLError,
                     ssl.SSLZeroReturnError,
                     ConnectionResetError,
                     BrokenPipeError
                    ) as ex:
-                Errors.add(ex)
+                later(ex)
                 self.stop()
                 debug("handler stopped")
                 evt = self.event(str(ex))
                 return evt
         try:
             txt = self.buffer.pop(0)
         except IndexError:
@@ -461,15 +458,15 @@
             except (
                     OSError,
                     ssl.SSLError,
                     ssl.SSLZeroReturnError,
                     ConnectionResetError,
                     BrokenPipeError
                    ) as ex:
-                Errors.add(ex)
+                later(ex)
                 self.stop()
                 return
         self.state.last = time.time()
         self.state.nrsend += 1
 
     def reconnect(self):
         "reconnect to server."
@@ -535,114 +532,97 @@
         Client.stop(self)
 
     def wait(self):
         "wait for ready."
         self.events.ready.wait()
 
 
-"callbacks"
-
-
-def cb_auth(evt):
+def cb_auth(bot, evt):
     "auth callback."
-    bot = get(evt.orig)
     bot.docommand(f'AUTHENTICATE {bot.cfg.password}')
 
 
-def cb_cap(evt):
+def cb_cap(bot, evt):
     "capabilities callback."
-    bot = get(evt.orig)
     if bot.cfg.password and 'ACK' in evt.arguments:
         bot.direct('AUTHENTICATE PLAIN')
     else:
         bot.direct('CAP REQ :sasl')
 
 
-def cb_error(evt):
+def cb_error(bot, evt):
     "error callback."
-    bot = get(evt.orig)
     if not bot.state.nrerror:
         bot.state.nrerror = 0
     bot.state.nrerror += 1
     bot.state.error = evt.txt
     debug(evt.txt)
 
 
-def cb_h903(evt):
+def cb_h903(bot, evt):
     "auth succeded callback."
-    bot = get(evt.orig)
     bot.direct('CAP END')
     bot.events.authed.set()
 
 
-def cb_h904(evt):
+def cb_h904(bot, evt):
     "auth succeded callback."
-    bot = get(evt.orig)
     bot.direct('CAP END')
     bot.events.authed.set()
 
 
-def cb_kill(evt):
+def cb_kill(bot, evt):
     "got killed callback."
 
 
-def cb_log(evt):
+def cb_log(bot, evt):
     "log callback."
 
 
-def cb_ready(evt):
+def cb_ready(bot, evt):
     "bot is ready callback."
-    bot = get(evt.orig)
-    if bot:
-        bot.events.ready.set()
+    bot.events.ready.set()
 
 
-def cb_001(evt):
+def cb_001(bot, evt):
     "first line received callback."
-    bot = get(evt.orig)
     bot.logon()
 
 
-def cb_notice(evt):
+def cb_notice(bot, evt):
     "notice callback."
-    bot = get(evt.orig)
     if evt.txt.startswith('VERSION'):
         txt = f'\001VERSION {NAME.upper()} 140 - {bot.cfg.username}\001'
         bot.docommand('NOTICE', evt.channel, txt)
 
 
-def cb_privmsg(evt):
+def cb_privmsg(bot, evt):
     "privmsg callback."
-    bot = get(evt.orig)
     if not bot.cfg.commands:
         return
     if evt.txt:
         if evt.txt[0] in ['!',]:
             evt.txt = evt.txt[1:]
         elif evt.txt.startswith(f'{bot.cfg.nick}:'):
             evt.txt = evt.txt[len(bot.cfg.nick)+1:]
         else:
             return
         if evt.txt:
             evt.txt = evt.txt[0].lower() + evt.txt[1:]
         debug(f"command from {evt.origin}: {evt.txt}")
-        bot.command(evt)
+        command(bot, evt)
 
 
-def cb_quit(evt):
+def cb_quit(bot, evt):
     "quit callback."
-    bot = get(evt.orig)
     debug(f"quit from {bot.cfg.server}")
     if evt.orig and evt.orig in bot.zelf:
         bot.stop()
 
 
-"commands"
-
-
 def cfg(event):
     "configure command."
     config = Config()
     path = last(config)
     if not event.sets:
         event.reply(
                     fmt(
@@ -658,15 +638,15 @@
 
 
 def mre(event):
     "show from output cache."
     if not event.channel:
         event.reply('channel is not set.')
         return
-    bot = Broker.get(event.orig)
+    bot = broker.get(event.orig)
     if 'cache' not in dir(bot):
         event.reply('bot is missing cache')
         return
     if event.channel not in bot.cache:
         event.reply(f'no output in {event.channel} cache.')
         return
     for _x in range(3):
@@ -685,15 +665,7 @@
     arg1 = event.args[0]
     arg2 = event.args[1]
     txt = f'\x00{arg1}\x00{arg2}'
     enc = txt.encode('ascii')
     base = base64.b64encode(enc)
     dcd = base.decode('ascii')
     event.reply(dcd)
-
-
-"register"
-
-
-Client.add(cfg)
-Client.add(mre)
-Client.add(pwd)
```

### Comparing `sbn-94/sbn/modules/log.py` & `sbn-95/sbn/modules/log.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,38 +1,30 @@
 # This file is placed in the Public Domain.
-#
-# pylint: disable=C,R,W0105
 
 
 "log text"
 
 
 import time
 
 
-from ..client  import Client
-from ..object  import Object
-from ..persist import Persist, find, fntime, sync
-from ..utils   import laps
+from ..client import laps
+from ..disk   import sync
+from ..find   import find, fntime
+from ..object import Object
 
 
-class Log(Object):
+class Log(Object): # pylint: disable=R0903
 
     "Log"
 
     def __init__(self):
-        Object.__init__()
+        super().__init__()
         self.txt = ''
 
-    def __yo__(self):
-        pass
-
-    def __yoyo__(self):
-        pass
-
 
 def log(event):
     "log text."
     if not event.rest:
         nmr = 0
         for fnm, obj in find('log'):
             lap = laps(time.time() - fntime(fnm))
@@ -41,13 +33,7 @@
         if not nmr:
             event.reply('no log')
         return
     obj = Log()
     obj.txt = event.rest
     sync(obj)
     event.reply('ok')
-
-
-"register"
-
-Client.add(log)
-Persist.add(Log)
```

### Comparing `sbn-94/sbn/modules/req.py` & `sbn-95/sbn/modules/req.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 # This file is placed in the Public Domain.
-#
-# pylint: disable=C.R,W0105
 
 
 """| **Information and Evidence Unit**
 | **Office of the Prosecutor**
 | **Post Office Box 19519**
 | **2500 CM The Hague**
 | **The Netherlands**
 |
+|
 
-Hello Office of the Prosecutor,
+Hello Office of the Prosecutor, ``OTP-CR-117/19``
 
 i write you in the context of communications and claims under art.15 of
 the Rome Statute. i want to inform the prosecutor that the king of the
 netherlands and his government are commiting 3 of the 5 crimes defined
 in the Rome Statute.
 
 The dutch government has introduced three new forced care laws, the Wfz
@@ -75,19 +74,10 @@
 
 
 (1) provided are the confirmation letters of both the chamber and the king.
 (2) your reference: OTP-CR-117/19
 """
 
 
-from ..client import Client
-
-
 def req(event):
-    "show request."
+    "reconsider"
     event.reply(__doc__)
-
-
-"register"
-
-
-Client.add(req)
```

### Comparing `sbn-94/sbn/modules/rss.py` & `sbn-95/sbn/modules/rss.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 # This file is placed in the Public Domain.
-#
-# pylint: disable=C,R,W0105
 
 
 "rich site syndicate"
 
 
 import html.parser
 import re
@@ -14,61 +12,59 @@
 import _thread
 
 
 from urllib.error import HTTPError, URLError
 from urllib.parse import quote_plus, urlencode
 
 
-from ..broker   import Broker
-from ..client   import Client
-from ..default  import Default
-from ..object   import Object, fmt, update
-from ..persist  import Persist, find, fntime, last, sync
-from ..repeater import Repeater
-from ..thread   import launch
-from ..utils    import laps, spl
+from ..client import laps
+from ..disk   import sync
+from ..find   import find, fntime, last
+from ..object import Default, Object, fmt, update, values
+from ..run    import broker, spl
+from ..thread import Repeater, launch
 
 
 def init():
     "start fetcher."
     fetcher = Fetcher()
     fetcher.start()
     return fetcher
 
 
-fetchlock = _thread.allocate_lock()
+DEBUG = False
 
 
-DEBUG = False
+fetchlock = _thread.allocate_lock()
 
 
 TEMPLATE = """<opml version="1.0">
     <head>
         <title>rssbot opml</title>
     </head>
     <body>
         <outline title="rssbot opml" text="24/7 feed fetcher">"""
 
 
-class Feed(Default):
+class Feed(Default): # pylint: disable=R0903
 
     "Feed"
 
 
-class Rss(Default):
+class Rss(Default): # pylint: disable=R0903
 
     "Rss"
 
     def __init__(self):
         Default.__init__(self)
         self.display_list = 'title,link,author'
         self.rss          = ''
 
 
-class Seen(Default):
+class Seen(Default): # pylint: disable=R0903
 
     "Seen"
 
     def __init__(self):
         Default.__init__(self)
         self.urls = []
 
@@ -129,15 +125,15 @@
             sync(self.seen, self.seenfn)
         txt = ''
         feedname = getattr(feed, 'name', None)
         if feedname:
             txt = f'[{feedname}] '
         for obj in result:
             txt2 = txt + self.display(obj)
-            for bot in Broker.all():
+            for bot in values(broker.objs):
                 if "announce" in dir(bot):
                     bot.announce(txt2.rstrip())
         return counter
 
     def run(self):
         "fetch all feeds."
         thrs = []
@@ -318,17 +314,14 @@
 
 
 def useragent(txt):
     "return useragent."
     return 'Mozilla/5.0 (X11; Linux x86_64) ' + txt
 
 
-"commands"
-
-
 def dpl(event):
     "set display items."
     if len(event.args) < 2:
         event.reply('dpl <stringinurl> <item1,item2>')
         return
     setter = {'display_list': event.args[1]}
     for _fn, feed in find('rss', {'rss': event.args[0]}):
@@ -411,20 +404,7 @@
         if result:
             event.reply(f'already got {url}')
             return
     feed = Rss()
     feed.rss = event.args[0]
     sync(feed)
     event.reply('ok')
-
-
-"register"
-
-
-Client.add(dpl)
-Client.add(exp)
-Client.add(nme)
-Client.add(rem)
-Client.add(res)
-Client.add(rss)
-Persist.add(Rss)
-Persist.add(Seen)
```

### Comparing `sbn-94/sbn/modules/thr.py` & `sbn-95/sbn/modules/thr.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 # This file is placed in the Public Domain.
-#
-# pylint: disable=C,R,W0105
 
 
 "show running threads"
 
 
 import threading
 import time
 
 
-from ..client  import Client
-from ..object  import Object, update
-from ..utils   import laps
+from ..client    import laps
+from ..object import Object, update
 
 
 STARTTIME = time.time()
 
 
 def thr(event):
     "show running threads."
@@ -37,13 +34,7 @@
     for uptime, txt in sorted(result, key=lambda x: x[1]):
         lap = laps(uptime)
         res.append(f'{txt}/{lap}')
     if res:
         event.reply(' '.join(res))
     else:
         event.reply('no threads')
-
-
-"initialize"
-
-
-Client.add(thr)
```

### Comparing `sbn-94/sbn/modules/tmr.py` & `sbn-95/sbn/modules/tmr.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,40 @@
 # This file is placed in the Public Domain.
-#
-# pylint: disable=C,R,W0105
 
 
 "timer"
 
 
 import datetime
 import re
 import time as ttime
 
 
-from ..broker  import Broker
-from ..client  import Client
-from ..event   import Event
+from ..client  import laps
+from ..disk    import sync
+from ..find    import find
 from ..object  import update
-from ..persist import Persist, find, sync
-from ..thread  import launch
-from ..timer   import Timer
-from ..utils   import laps
+from ..handler import Event
+from ..run     import broker
+from ..thread  import Timer, launch
+
+
+def init():
+    "start timers."
+    for _fn, obj in find("timer"):
+        if "time" not in obj:
+            continue
+        diff = float(obj.time) - ttime.time()
+        if diff > 0:
+            bot = broker.first()
+            evt = Event()
+            update(evt, obj)
+            evt.orig = object.__repr__(bot)
+            timer = Timer(diff, evt.show)
+            launch(timer.start)
 
 
 MONTHS = [
     'Bo',
     'Jan',
     'Feb',
     'Mar',
@@ -74,15 +86,15 @@
             (day, month, yea) = ymdre.groups()
     except ValueError:
         try:
             ymre = re.search(r'(\d+)-(\d+)', daystr)
             if ymre:
                 (day, month) = ymre.groups()
                 yea = ttime.strftime("%Y", ttime.localtime())
-        except Exception as ex:
+        except Exception as ex: # pylint: disable=W0212
             raise NoDate(daystr) from ex
     if day:
         day = int(day)
         month = int(month)
         yea = int(yea)
         date = f"{day} {MONTHS[month]} {yea}"
         return ttime.mktime(ttime.strptime(date, r"%d %b %Y"))
@@ -165,17 +177,14 @@
 
 
 def today():
     "return date."
     return str(datetime.datetime.today()).split()[0]
 
 
-"commands"
-
-
 def tmr(event):
     "add a timer."
     result = ""
     if not event.rest:
         nmr = 0
         for _fn, obj in find('timer'):
             lap = float(obj.time) - ttime.time()
@@ -213,32 +222,7 @@
     event.result = []
     event.result.append(event.rest)
     timer = Timer(diff, event.show, thrname=event.cmd)
     update(timer, event)
     sync(timer)
     launch(timer.start)
     return result
-
-
-"runtime"
-
-
-def init():
-    "start timers."
-    for _fn, obj in find("timer"):
-        if "time" not in obj:
-            continue
-        diff = float(obj.time) - ttime.time()
-        if diff > 0:
-            bot = Broker.first()
-            evt = Event()
-            update(evt, obj)
-            evt.orig = object.__repr__(bot)
-            timer = Timer(diff, evt.show)
-            launch(timer.start)
-
-
-"register"
-
-
-Client.add(tmr)
-Persist.add(Timer)
```

### Comparing `sbn-94/sbn/object.py` & `sbn-95/sbn/object.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 # This file is placed in the Public Domain.
-#
-# pylint: disable=C,R,W0105
 
 
-"object"
+"clean namespace"
 
 
 import json
-import os
 import pathlib
 import _thread
 
 
-disklock = _thread.allocate_lock()
+lock = _thread.allocate_lock()
 
 
-class Object:
+class Object: # pylint: disable=R0902
 
     "Object"
 
     def __contains__(self, key):
         return key in dir(self)
 
     def __iter__(self):
@@ -28,14 +25,22 @@
     def __len__(self):
         return len(self.__dict__)
 
     def __str__(self):
         return str(self.__dict__)
 
 
+class Default(Object): # pylint: disable=R0902,R0903
+
+    "Default"
+
+    def __getattr__(self, key):
+        return self.__dict__.get(key, "")
+
+
 def construct(obj, *args, **kwargs):
     "construct an object from provided arguments."
     if args:
         val = args[0]
         if isinstance(val, zip):
             update(obj, dict(val))
         elif isinstance(val, dict):
@@ -113,15 +118,15 @@
     if isinstance(obj, type({})):
         return obj.keys()
     return list(obj.__dict__.keys())
 
 
 def read(obj, pth):
     "read an object from file path."
-    with disklock:
+    with lock:
         with open(pth, 'r', encoding='utf-8') as ofile:
             update(obj, load(ofile))
 
 
 def search(obj, selector):
     "check if object matches provided values."
     res = False
@@ -148,16 +153,17 @@
 def values(obj):
     "return values of an object."
     return obj.__dict__.values()
 
 
 def write(obj, pth):
     "write an object to disk."
-    with disklock:
-        cdir(os.path.dirname(pth))
+    with lock:
+        path = pathlib.Path(pth)
+        path.parent.mkdir(parents=True, exist_ok=True)
         with open(pth, 'w', encoding='utf-8') as ofile:
             dump(obj, ofile, indent=4)
 
 
 class ObjectDecoder(json.JSONDecoder):
 
     "ObjectDecoder"
@@ -240,28 +246,18 @@
 
 def dumps(*args, **kw):
     "dump object to string."
     kw["cls"] = ObjectEncoder
     return json.dumps(*args, **kw)
 
 
-def cdir(pth):
-    "create directory."
-    if os.path.exists(pth):
-        return
-    pth = pathlib.Path(pth)
-    os.makedirs(pth, exist_ok=True)
-
-
-"interface"
-
-
 def __dir__():
     return (
         'Object',
+        'Default',
         'construct',
         'dump',
         'dumps',
         'edit',
         'fmt',
         'fqn',
         'hook',
@@ -271,10 +267,7 @@
         'loads',
         'read',
         'search',
         'update',
         'values',
         'write'
     )
-
-
-__all__ = __dir__()
```

### Comparing `sbn-94/sbn/persist.py` & `sbn-95/sbn/disk.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,147 +1,122 @@
 # This file is placed in the Public Domain.
-#
-# pylint: disable=C,R,W0105
 
 
-"persist"
+"disk"
 
 
 import datetime
+import inspect
 import os
-import time
+import pathlib
 
 
-from .default import Default
-from .object  import Object, fqn, read, search, update, write
-from .workdir import Workdir
+from .object import Object, fqn, read, write
 
 
-class Persist(Object):
+class Workdir(Object): # pylint: disable=R0903
 
-    "Persist"
+    "Workdir"
 
-    classes = Object()
-
-    @staticmethod
-    def add(clz):
-        "add class to whitelist."
-        name = str(clz).split()[1][1:-2]
-        setattr(Persist.classes, name, clz)
-
-    @staticmethod
-    def fns(mtc=""):
-        "show list of files."
-        dname = ''
-        pth = Workdir.store(mtc)
-        for rootdir, dirs, _files in os.walk(pth, topdown=False):
-            if dirs:
-                for dname in sorted(dirs):
-                    if dname.count('-') == 2:
-                        ddd = os.path.join(rootdir, dname)
-                        fls = sorted(os.listdir(ddd))
-                        for fll in fls:
-                            yield Workdir.strip(os.path.join(ddd, fll))
-
-    @staticmethod
-    def long(name):
-        "match from single name to long name."
-        split = name.split(".")[-1].lower()
-        res = name
-        for named in Persist.classes:
-            if split in named.split(".")[-1].lower():
-                res = named
-                break
-        if "." not in res:
-            for fnm in Workdir.types():
-                claz = fnm.split(".")[-1]
-                if fnm == claz.lower():
-                    res = fnm
-        return res
-
-
-def fntime(daystr):
-    "convert file name to it's saved time."
-    daystr = daystr.replace('_', ':')
-    datestr = ' '.join(daystr.split(os.sep)[-2:])
-    if '.' in datestr:
-        datestr, rest = datestr.rsplit('.', 1)
-    else:
-        rest = ''
-    timed = time.mktime(time.strptime(datestr, '%Y-%m-%d %H:%M:%S'))
-    if rest:
-        timed += float('.' + rest)
-    return timed
-
-
-def find(mtc, selector=None, index=None, deleted=False):
-    "find object matching the selector dict."
-    clz = Persist.long(mtc)
-    nrs = -1
-    for fnm in sorted(Persist.fns(clz), key=fntime):
-        obj = Default()
-        fetch(obj, fnm)
-        if not deleted and '__deleted__' in obj:
-            continue
-        if selector and not search(obj, selector):
-            continue
-        nrs += 1
-        if index is not None and nrs != int(index):
-            continue
-        yield (fnm, obj)
+    workdir = ""
 
 
 def fetch(obj, pth):
     "read object from disk."
-    pth2 = Workdir.store(pth)
+    pth2 = store(pth)
     read(obj, pth2)
-    return Workdir.strip(pth)
+    return strip(pth)
 
 
 def ident(obj):
     "return an id for an object."
     return os.path.join(
                         fqn(obj),
                         os.path.join(*str(datetime.datetime.now()).split())
                        )
 
 
-def last(obj, selector=None):
-    "return last object saved."
-    if selector is None:
-        selector = {}
-    result = sorted(
-                    find(fqn(obj), selector),
-                    key=lambda x: fntime(x[0])
-                   )
-    res = None
-    if result:
-        inp = result[-1]
-        update(obj, inp[-1])
-        res = inp[0]
-    return res
+def lsstore():
+    "return types stored."
+    return os.listdir(store())
+
+
+def skel():
+    "create directory,"
+    pth  = os.path.join(Workdir.workdir, "store", "")
+    path = pathlib.Path(pth)
+    path.mkdir(parents=True, exist_ok=True)
+
+
+def store(pth=""):
+    "return objects directory."
+    return os.path.join(Workdir.workdir, "store", pth)
+
+
+def strip(pth, nmr=3):
+    "reduce to path with directory."
+    return os.sep.join(pth.split(os.sep)[-nmr:])
+
 
 def sync(obj, pth=None):
     "sync object to disk."
     if pth is None:
         pth = ident(obj)
-    pth2 = Workdir.store(pth)
+    pth2 = store(pth)
     write(obj, pth2)
     return pth
 
 
-"interface"
+class Whitelist(Object): # pylint: disable=R0903
+
+    "Whitelist"
+
+    classes = Object()
+
+
+def scancls(mod) -> None:
+    "scan module for classes."
+    for key, clz in inspect.getmembers(mod, inspect.isclass):
+        if key.startswith("cb"):
+            continue
+        if not issubclass(clz, Object):
+            continue
+        whitelist(clz)
+
+
+def whitelist(clz):
+    "add class to whitelist."
+    name = str(clz).split()[1][1:-2]
+    setattr(Whitelist.classes, name, clz)
+
+
+def long(name):
+    "match from single name to long name."
+    split = name.split(".")[-1].lower()
+    res = name
+    for named in Whitelist.classes:
+        if split in named.split(".")[-1].lower():
+            res = named
+            break
+    if "." not in res:
+        for fnm in lsstore():
+            claz = fnm.split(".")[-1]
+            if fnm == claz.lower():
+                res = fnm
+    return res
 
 
 def __dir__():
     return (
-        'Persist',
+        'Whitelist',
+        'Workdir',
         'fetch',
-        'fntime',
-        'find',
-        'last',
         'ident',
+        'lsstore',
+        'long',
+        'scancls',
+        'skel',
+        'store',
+        'strip',
         'sync',
+        'whitelist'
     )
-
-
-__all__ = __dir__()
```

### Comparing `sbn-94/sbn.egg-info/PKG-INFO` & `sbn-95/sbn.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbn
-Version: 94
+Version: 95
 Summary: Skull, Bones and Number (OTP-CR-117/19)
 Author-email: Bart Thate <bthate@dds.nl>
 License: Public Domain
 Project-URL: home, https://pypi.org/project/sbn
 Project-URL: bugs, https://github.com/bthate/sbn/issues
 Project-URL: source, https://github.com/bthate/sbn
 Classifier: Development Status :: 3 - Alpha
@@ -15,20 +15,19 @@
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
 
 | **Information and Evidence Unit**
 | **Office of the Prosecutor**
 | **Post Office Box 19519**
 | **2500 CM The Hague**
-| **The Netherlands** ``OTP-CR-117/19``
-|
+| **The Netherlands** 
 |
 
 
-Hello Office of the Prosecutor,
+Hello Office of the Prosecutor, ``OTP-CR-117/19``
 
 i write you in the context of communications and claims under art.15 of 
 the Rome Statute. i want to inform the prosecutor that the king of the 
 netherlands and his government are commiting 3 of the 5 crimes defined 
 in the Rome Statute.
 
 The dutch government has introduced three new forced care laws, the Wfz
```

