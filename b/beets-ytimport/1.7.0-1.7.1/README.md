# Comparing `tmp/beets_ytimport-1.7.0-py3-none-any.whl.zip` & `tmp/beets_ytimport-1.7.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 15592 bytes, number of entries: 11
--rw-r--r--  2.0 unx       75 b- defN 24-Mar-29 02:53 beetsplug/__init__.py
--rw-r--r--  2.0 unx    10634 b- defN 24-Mar-29 02:53 beetsplug/ytimport/__init__.py
--rw-r--r--  2.0 unx      468 b- defN 24-Mar-29 02:53 beetsplug/ytimport/config_default.yaml
--rw-r--r--  2.0 unx      413 b- defN 24-Mar-29 02:53 beetsplug/ytimport/safename.py
--rw-r--r--  2.0 unx     5280 b- defN 24-Mar-29 02:53 beetsplug/ytimport/split.py
--rw-r--r--  2.0 unx     6739 b- defN 24-Mar-29 02:53 beetsplug/ytimport/youtube.py
--rw-r--r--  2.0 unx    11357 b- defN 24-Mar-29 02:56 beets_ytimport-1.7.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     5058 b- defN 24-Mar-29 02:56 beets_ytimport-1.7.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Mar-29 02:56 beets_ytimport-1.7.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 24-Mar-29 02:56 beets_ytimport-1.7.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      936 b- defN 24-Mar-29 02:56 beets_ytimport-1.7.0.dist-info/RECORD
-11 files, 41062 bytes uncompressed, 13996 bytes compressed:  65.9%
+Zip file size: 15568 bytes, number of entries: 11
+-rw-r--r--  2.0 unx       75 b- defN 24-May-12 17:39 beetsplug/__init__.py
+-rw-r--r--  2.0 unx    10433 b- defN 24-May-12 17:39 beetsplug/ytimport/__init__.py
+-rw-r--r--  2.0 unx      468 b- defN 24-May-12 17:39 beetsplug/ytimport/config_default.yaml
+-rw-r--r--  2.0 unx      413 b- defN 24-May-12 17:39 beetsplug/ytimport/safename.py
+-rw-r--r--  2.0 unx     5280 b- defN 24-May-12 17:39 beetsplug/ytimport/split.py
+-rw-r--r--  2.0 unx     6739 b- defN 24-May-12 17:39 beetsplug/ytimport/youtube.py
+-rw-r--r--  2.0 unx    11357 b- defN 24-May-12 17:43 beets_ytimport-1.7.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     5058 b- defN 24-May-12 17:43 beets_ytimport-1.7.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-12 17:43 beets_ytimport-1.7.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 24-May-12 17:43 beets_ytimport-1.7.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      936 b- defN 24-May-12 17:43 beets_ytimport-1.7.1.dist-info/RECORD
+11 files, 40861 bytes uncompressed, 13972 bytes compressed:  65.8%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: beetsplug/ytimport/split.py
 Comment: 
 
 Filename: beetsplug/ytimport/youtube.py
 Comment: 
 
-Filename: beets_ytimport-1.7.0.dist-info/LICENSE
+Filename: beets_ytimport-1.7.1.dist-info/LICENSE
 Comment: 
 
-Filename: beets_ytimport-1.7.0.dist-info/METADATA
+Filename: beets_ytimport-1.7.1.dist-info/METADATA
 Comment: 
 
-Filename: beets_ytimport-1.7.0.dist-info/WHEEL
+Filename: beets_ytimport-1.7.1.dist-info/WHEEL
 Comment: 
 
-Filename: beets_ytimport-1.7.0.dist-info/top_level.txt
+Filename: beets_ytimport-1.7.1.dist-info/top_level.txt
 Comment: 
 
-Filename: beets_ytimport-1.7.0.dist-info/RECORD
+Filename: beets_ytimport-1.7.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## beetsplug/ytimport/__init__.py

```diff
@@ -83,18 +83,18 @@
                 #    h = dict([l.split(': ', 1) for l in headers.strip().split('\n')[1:]])
                 youtube.download(urls, ytdir, format=opts.format, min_len=opts.min_length, max_len=opts.max_length, max_len_nochapter=opts.max_length_nochapter, split=opts.split_tracks, like=opts.likes, reimport=opts.reimport, auth_headers=h)
             else:
                 print('Nothing to download')
             if opts.do_import:
                 print('Importing downloaded songs into beets library')
                 if opts.group_albums:
-                    self._import_files(lib, opts, albums_dir, True)
-                    self._import_files(lib, opts, singles_dir, False)
+                    self._import_files(lib, opts, albums_dir, False)
+                    self._import_files(lib, opts, singles_dir, True)
                 else:
-                    self._import_files(lib, opts, ytdir, False)
+                    self._import_files(lib, opts, ytdir, True)
             else:
                 print('Skipping import')
 
         p = OptionParser()
         p.add_option('--directory', type='string', metavar='DIR',
             default=self.config['directory'].get(),
             dest='directory', help='directory to download Youtube files to')
@@ -164,39 +164,36 @@
             default=False,
             dest='pretend', help="don't import but print the files when importing")
 
         c = Subcommand('ytimport', parser=p, help='import songs from Youtube')
         c.func = run_import_cmd
         return [c]
 
-    def _import_files(self, lib, opts, src_dir, group_albums):
+    def _import_files(self, lib, opts, src_dir, singletons):
         user_incremental = config['import']['incremental'].get()
         user_resume = config['import']['resume'].get()
         user_move = config['import']['move'].get()
         user_quiet = config['import']['quiet'].get()
         user_quiet_fallback = config['import']['quiet_fallback'].get()
-        user_group_albums = config['import']['group_albums'].get()
         user_singletons = config['import']['singletons'].get()
         user_pretend = config['import']['pretend'].get()
         user_set_fields = {k: v.get() for k,v in config['import']['set_fields'].items()}
         try:
             config['import']['incremental'] = not opts.reimport
             config['import']['resume'] = True
             config['import']['move'] = True
             config['import']['pretend'] = opts.pretend
-            config['import']['group_albums'] = group_albums
-            config['import']['singletons'] = not group_albums
+            config['import']['singletons'] = singletons
             config['import']['set_fields'] = opts.set
             config['import']['quiet'] = opts.quiet
             if opts.quiet_fallback:
                 config['import']['quiet_fallback'] = opts.quiet_fallback
             import_files(lib, [src_dir], None)
         finally: # revert global import configuration changes
             config['import']['incremental'] = user_incremental
             config['import']['resume'] = user_resume
             config['import']['move'] = user_move
             config['import']['pretend'] = user_pretend
-            config['import']['group_albums'] = user_group_albums
             config['import']['singletons'] = user_singletons
             config['import']['set_fields'] = user_set_fields
             config['import']['quiet'] = user_quiet
             config['import']['quiet_fallback'] = user_quiet_fallback
```

## Comparing `beets_ytimport-1.7.0.dist-info/LICENSE` & `beets_ytimport-1.7.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `beets_ytimport-1.7.0.dist-info/METADATA` & `beets_ytimport-1.7.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beets-ytimport
-Version: 1.7.0
+Version: 1.7.1
 Summary: Download audio from Youtube into your Beets library
 Home-page: https://github.com/mgoltzsche/beets-ytimport
 Author: Max Goltzsche
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
 Classifier: License :: OSI Approved :: Apache Software License
```

## Comparing `beets_ytimport-1.7.0.dist-info/RECORD` & `beets_ytimport-1.7.1.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 beetsplug/__init__.py,sha256=QDJyS5jtJnGFsSuOx43ZvLBCOrHImm8NrZk5f9URWdk,75
-beetsplug/ytimport/__init__.py,sha256=p5p5bHSaavECKrQOM_0K9GabMGLUHwrlUhYVtSRIWI8,10634
+beetsplug/ytimport/__init__.py,sha256=iiwewVBDJPcROZzZWzW0uGn7wnri-sUwkWgI76fr7Sc,10433
 beetsplug/ytimport/config_default.yaml,sha256=uHFv5cbeLeGXvoxJEGLpYw39sqvkvu6S8Kr6GDmEkAI,468
 beetsplug/ytimport/safename.py,sha256=O3iqwuxiWHO_d-pQ-MGTul51DN57QSOMGgYE-Tc9ILY,413
 beetsplug/ytimport/split.py,sha256=3wLEAMz-w8U1evbbt_m2VjB_0rkdwBR33mtDvnExGvg,5280
 beetsplug/ytimport/youtube.py,sha256=TSLrmPPWTi1GvOKwAtKvCt2iAZq8GcenPyfigp_f1MM,6739
-beets_ytimport-1.7.0.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-beets_ytimport-1.7.0.dist-info/METADATA,sha256=wzoWB9Qg2qnIHFGLc9TOBbgi2MIGxaS5tfOZInjJCIw,5058
-beets_ytimport-1.7.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-beets_ytimport-1.7.0.dist-info/top_level.txt,sha256=za8u6CXAGbgac8cUyn9NlsgXqqq-_4HHZcNmJnfmyWc,10
-beets_ytimport-1.7.0.dist-info/RECORD,,
+beets_ytimport-1.7.1.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+beets_ytimport-1.7.1.dist-info/METADATA,sha256=Z-UD4qEkCrabnPJKQ-2XxKEH2G-KT64zFysSH9EofSU,5058
+beets_ytimport-1.7.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+beets_ytimport-1.7.1.dist-info/top_level.txt,sha256=za8u6CXAGbgac8cUyn9NlsgXqqq-_4HHZcNmJnfmyWc,10
+beets_ytimport-1.7.1.dist-info/RECORD,,
```

