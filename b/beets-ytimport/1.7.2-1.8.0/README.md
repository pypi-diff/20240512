# Comparing `tmp/beets_ytimport-1.7.2-py3-none-any.whl.zip` & `tmp/beets_ytimport-1.8.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 15592 bytes, number of entries: 11
--rw-r--r--  2.0 unx       75 b- defN 24-May-12 17:53 beetsplug/__init__.py
--rw-r--r--  2.0 unx    10618 b- defN 24-May-12 17:53 beetsplug/ytimport/__init__.py
--rw-r--r--  2.0 unx      468 b- defN 24-May-12 17:53 beetsplug/ytimport/config_default.yaml
--rw-r--r--  2.0 unx      413 b- defN 24-May-12 17:53 beetsplug/ytimport/safename.py
--rw-r--r--  2.0 unx     5280 b- defN 24-May-12 17:53 beetsplug/ytimport/split.py
--rw-r--r--  2.0 unx     6739 b- defN 24-May-12 17:53 beetsplug/ytimport/youtube.py
--rw-r--r--  2.0 unx    11357 b- defN 24-May-12 17:56 beets_ytimport-1.7.2.dist-info/LICENSE
--rw-r--r--  2.0 unx     5058 b- defN 24-May-12 17:56 beets_ytimport-1.7.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-12 17:56 beets_ytimport-1.7.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 24-May-12 17:56 beets_ytimport-1.7.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      936 b- defN 24-May-12 17:56 beets_ytimport-1.7.2.dist-info/RECORD
-11 files, 41046 bytes uncompressed, 13996 bytes compressed:  65.9%
+Zip file size: 15716 bytes, number of entries: 11
+-rw-r--r--  2.0 unx       75 b- defN 24-May-12 19:41 beetsplug/__init__.py
+-rw-r--r--  2.0 unx    11153 b- defN 24-May-12 19:41 beetsplug/ytimport/__init__.py
+-rw-r--r--  2.0 unx      468 b- defN 24-May-12 19:41 beetsplug/ytimport/config_default.yaml
+-rw-r--r--  2.0 unx      413 b- defN 24-May-12 19:41 beetsplug/ytimport/safename.py
+-rw-r--r--  2.0 unx     5280 b- defN 24-May-12 19:41 beetsplug/ytimport/split.py
+-rw-r--r--  2.0 unx     6739 b- defN 24-May-12 19:41 beetsplug/ytimport/youtube.py
+-rw-r--r--  2.0 unx    11357 b- defN 24-May-12 19:45 beets_ytimport-1.8.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     5058 b- defN 24-May-12 19:45 beets_ytimport-1.8.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-12 19:45 beets_ytimport-1.8.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 24-May-12 19:45 beets_ytimport-1.8.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      936 b- defN 24-May-12 19:45 beets_ytimport-1.8.0.dist-info/RECORD
+11 files, 41581 bytes uncompressed, 14120 bytes compressed:  66.0%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: beetsplug/ytimport/split.py
 Comment: 
 
 Filename: beetsplug/ytimport/youtube.py
 Comment: 
 
-Filename: beets_ytimport-1.7.2.dist-info/LICENSE
+Filename: beets_ytimport-1.8.0.dist-info/LICENSE
 Comment: 
 
-Filename: beets_ytimport-1.7.2.dist-info/METADATA
+Filename: beets_ytimport-1.8.0.dist-info/METADATA
 Comment: 
 
-Filename: beets_ytimport-1.7.2.dist-info/WHEEL
+Filename: beets_ytimport-1.8.0.dist-info/WHEEL
 Comment: 
 
-Filename: beets_ytimport-1.7.2.dist-info/top_level.txt
+Filename: beets_ytimport-1.8.0.dist-info/top_level.txt
 Comment: 
 
-Filename: beets_ytimport-1.7.2.dist-info/RECORD
+Filename: beets_ytimport-1.8.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## beetsplug/ytimport/__init__.py

```diff
@@ -1,10 +1,12 @@
 import os
+import re
 import pathlib
 import mediafile
+import requests
 from beets.plugins import BeetsPlugin
 from beets.dbcore import types
 from beets.ui import Subcommand
 from beets.ui import _store_dict
 from beets.ui.commands import import_files
 from beets import config
 from optparse import OptionParser
@@ -47,56 +49,64 @@
             headers = opts.auth_headers
             if headers:
                 f = open(headers, 'r')
                 headers = f.read()
                 f.close()
             urls = [] + args
             if opts.url_file:
-                f = open(opts.url_file, 'r')
-                urls += f.readlines()
-                f.close()
+                add_urls = []
+                if re.match(r'^https?://', opts.url_file):
+                    add_urls = requests.get(opts.url_file).text.strip('\n').split('\n')
+                else:
+                    f = open(opts.url_file, 'r')
+                    add_urls = f.readlines()
+                    f.close()
+                urls += add_urls
+                self._log.info('Found {:n} URLs within URL file', len(add_urls))
             singles_dir = os.path.join(ytdir, 'singles')
             albums_dir = os.path.join(ytdir, 'albums')
             pathlib.Path(singles_dir).mkdir(parents=True, exist_ok=True)
             pathlib.Path(albums_dir).mkdir(parents=False, exist_ok=True)
             if opts.likes:
                 if opts.url_file or len(args) > 0:
                     raise Exception('Using --likes option in conjunction with --url-file or URL args is not supported!')
                 # TODO: mark like as tag within downloaded file already (to be able to distinguish likes also on local reimport)
-                print('Obtaining your liked songs from Youtube...')
+                self._log.info('Obtaining your liked songs from Youtube...')
                 if not headers:
-                    print('Using interactive authentication. To enable non-interactive authentication, set --auth-headers')
+                    self._log.info('Using interactive authentication. To enable non-interactive authentication, set --auth-headers')
                 auth = youtube.login(headers)
                 likedIds = youtube.likes(auth, opts.max_likes)
                 if len(likedIds) > opts.max_likes:
                     likedIds = likedIds[:opts.max_likes]
-                print('Found {:n} liked songs'.format(len(likedIds)))
+                self._log.info('Found {:n} liked songs', len(likedIds))
                 urls += ['https://www.youtube.com/watch?v='+id for id in likedIds]
             if not opts.reimport:
-                urls = [u for u in urls if not lib.items('comments:'+u)]
+                unknown_urls = [u for u in urls if not lib.items('comments:'+u)]
+                self._log.info('Ignoring {:n} known URLs', len(urls)-len(unknown_urls))
+                urls = unknown_urls
             if urls:
-                print('Downloading {:n} song(s) to {:s}'.format(len(urls), ytdir))
+                self._log.info('Downloading {:n} song(s) to {:s}', len(urls), ytdir)
                 h = {}
                 # TODO: authenticate download requests.
                 # The following makes download requests return a 400 reponse.
                 # Maybe a cookiefile with some picked cookies from the headers can be generated?
                 #if opts.auth and headers:
                 #    h = dict([l.split(': ', 1) for l in headers.strip().split('\n')[1:]])
                 youtube.download(urls, ytdir, format=opts.format, min_len=opts.min_length, max_len=opts.max_length, max_len_nochapter=opts.max_length_nochapter, split=opts.split_tracks, like=opts.likes, reimport=opts.reimport, auth_headers=h)
             else:
-                print('Nothing to download')
+                self._log.info('Nothing to download')
             if opts.do_import:
-                print('Importing downloaded songs into beets library')
+                self._log.info('Importing downloaded songs into beets library')
                 if opts.group_albums:
                     self._import_files(lib, opts, albums_dir, False)
                     self._import_files(lib, opts, singles_dir, True)
                 else:
                     self._import_files(lib, opts, ytdir, True)
             else:
-                print('Skipping import')
+                self._log.info('Skipping import')
 
         p = OptionParser()
         p.add_option('--directory', type='string', metavar='DIR',
             default=self.config['directory'].get(),
             dest='directory', help='directory to download Youtube files to')
         p.add_option('--format', type='string', metavar='FORMAT',
             default=self.config['format'].get(),
```

## Comparing `beets_ytimport-1.7.2.dist-info/LICENSE` & `beets_ytimport-1.8.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `beets_ytimport-1.7.2.dist-info/METADATA` & `beets_ytimport-1.8.0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beets-ytimport
-Version: 1.7.2
+Version: 1.8.0
 Summary: Download audio from Youtube into your Beets library
 Home-page: https://github.com/mgoltzsche/beets-ytimport
 Author: Max Goltzsche
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
 Classifier: License :: OSI Approved :: Apache Software License
```

## Comparing `beets_ytimport-1.7.2.dist-info/RECORD` & `beets_ytimport-1.8.0.dist-info/RECORD`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 beetsplug/__init__.py,sha256=QDJyS5jtJnGFsSuOx43ZvLBCOrHImm8NrZk5f9URWdk,75
-beetsplug/ytimport/__init__.py,sha256=X9V6nxGpZ4LzHHE4WdWyUo-FBlPAWOlO7pblzXNm1hc,10618
+beetsplug/ytimport/__init__.py,sha256=IP5Jgh0-us5pjWRWUvPwQlCKcEz3YLTq40SX51cCvx8,11153
 beetsplug/ytimport/config_default.yaml,sha256=uHFv5cbeLeGXvoxJEGLpYw39sqvkvu6S8Kr6GDmEkAI,468
 beetsplug/ytimport/safename.py,sha256=O3iqwuxiWHO_d-pQ-MGTul51DN57QSOMGgYE-Tc9ILY,413
 beetsplug/ytimport/split.py,sha256=3wLEAMz-w8U1evbbt_m2VjB_0rkdwBR33mtDvnExGvg,5280
 beetsplug/ytimport/youtube.py,sha256=TSLrmPPWTi1GvOKwAtKvCt2iAZq8GcenPyfigp_f1MM,6739
-beets_ytimport-1.7.2.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-beets_ytimport-1.7.2.dist-info/METADATA,sha256=gQCXaxrIXixHMGu30WW3C4dMRls246D4JZ_LcFMEEyw,5058
-beets_ytimport-1.7.2.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-beets_ytimport-1.7.2.dist-info/top_level.txt,sha256=za8u6CXAGbgac8cUyn9NlsgXqqq-_4HHZcNmJnfmyWc,10
-beets_ytimport-1.7.2.dist-info/RECORD,,
+beets_ytimport-1.8.0.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+beets_ytimport-1.8.0.dist-info/METADATA,sha256=3i78iYA12eQ5Rb-jYcO2B3z4UiZjgY7mSvhSYArREw0,5058
+beets_ytimport-1.8.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+beets_ytimport-1.8.0.dist-info/top_level.txt,sha256=za8u6CXAGbgac8cUyn9NlsgXqqq-_4HHZcNmJnfmyWc,10
+beets_ytimport-1.8.0.dist-info/RECORD,,
```

