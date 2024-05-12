# Comparing `tmp/b7w-cli-0.1.9.tar.gz` & `tmp/b7w_cli-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "b7w-cli-0.1.9.tar", max compression
+gzip compressed data, was "b7w_cli-0.3.0.tar", max compression
```

## Comparing `b7w-cli-0.1.9.tar` & `b7w_cli-0.3.0.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0     1070 2022-07-28 20:28:54.922335 b7w-cli-0.1.9/LICENSE
--rw-r--r--   0        0        0      293 2022-07-28 20:28:54.922335 b7w-cli-0.1.9/README.md
--rw-r--r--   0        0        0      513 2022-07-28 20:28:54.922335 b7w-cli-0.1.9/pyproject.toml
--rw-r--r--   0        0        0       22 2022-07-28 20:30:57.731691 b7w-cli-0.1.9/src/b7w_cli/__init__.py
--rw-r--r--   0        0        0     1739 2022-07-28 20:28:54.922335 b7w-cli-0.1.9/src/b7w_cli/cli.py
--rw-r--r--   0        0        0     3563 2022-07-28 20:28:54.922335 b7w-cli-0.1.9/src/b7w_cli/images.py
--rw-r--r--   0        0        0      485 2022-07-28 20:28:54.922335 b7w-cli-0.1.9/src/b7w_cli/mac.py
--rw-r--r--   0        0        0     1396 2022-07-28 20:28:54.922335 b7w-cli-0.1.9/src/b7w_cli/utils.py
--rw-r--r--   0        0        0     1740 2022-07-28 20:28:54.922335 b7w-cli-0.1.9/src/b7w_cli/video.py
--rw-r--r--   0        0        0     1118 2022-07-28 20:30:59.118050 b7w-cli-0.1.9/setup.py
--rw-r--r--   0        0        0      935 2022-07-28 20:30:59.118334 b7w-cli-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-05-12 14:28:28.841400 b7w_cli-0.3.0/LICENSE
+-rw-r--r--   0        0        0      293 2024-05-12 14:28:28.841400 b7w_cli-0.3.0/README.md
+-rw-r--r--   0        0        0      539 2024-05-12 14:28:28.841400 b7w_cli-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-05-12 14:29:11.549839 b7w_cli-0.3.0/src/b7w_cli/__init__.py
+-rw-r--r--   0        0        0     1883 2024-05-12 14:28:28.841400 b7w_cli-0.3.0/src/b7w_cli/cli.py
+-rw-r--r--   0        0        0     4104 2024-05-12 14:28:28.841400 b7w_cli-0.3.0/src/b7w_cli/images.py
+-rw-r--r--   0        0        0      485 2024-05-12 14:28:28.841400 b7w_cli-0.3.0/src/b7w_cli/mac.py
+-rw-r--r--   0        0        0     1535 2024-05-12 14:28:28.841400 b7w_cli-0.3.0/src/b7w_cli/utils.py
+-rw-r--r--   0        0        0     1740 2024-05-12 14:28:28.841400 b7w_cli-0.3.0/src/b7w_cli/video.py
+-rw-r--r--   0        0        0      931 1970-01-01 00:00:00.000000 b7w_cli-0.3.0/PKG-INFO
```

### Comparing `b7w-cli-0.1.9/LICENSE` & `b7w_cli-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `b7w-cli-0.1.9/src/b7w_cli/cli.py` & `b7w_cli-0.3.0/src/b7w_cli/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,19 +13,21 @@
 
 @main.group()
 def img():
     pass
 
 
 @img.command()
+@click.argument('paths', nargs=-1, type=click.Path(exists=True, file_okay=False))
 @timeit
-def organise():
-    organise_ext()
-    organise_raw()
-    organise_video()
+def organise(paths):
+    for path in paths or ('.',):
+        organise_ext(path)
+        organise_raw(path)
+        organise_video(path)
 
 
 @img.command()
 @click.option('--force', is_flag=True, default=False, help='Do not confirm')
 @timeit
 def merge(force):
     merge_raws(force)
```

### Comparing `b7w-cli-0.1.9/src/b7w_cli/images.py` & `b7w_cli-0.3.0/src/b7w_cli/images.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,70 +1,70 @@
 import os
-import shutil
 import time
 from itertools import chain
 from pathlib import Path
 
-from b7w_cli.utils import iter_files
+from b7w_cli.utils import iter_files, script
 
 
-def organise_ext():
+def organise_ext(base_path):
     """
     Rename upper case extensions to lover case
     """
     start = time.time()
     count = 0
     extensions = ('.JPG', '.MOV', '.MP4',)
-    files = (i for i in iter_files('.') if i.suffix in extensions)
+    files = (i for i in iter_files(base_path) if i.suffix in extensions)
     for path in files:
         new_name = path.with_suffix(path.suffix.lower())
         path.rename(new_name)
-        print('Rename ' + new_name.as_posix())
+        print('[{0}] Rename {1} '.format(base_path, new_name.as_posix()))
         count += 1
 
     elapsed = int(time.time() - start)
-    print('# Rename {0} file extensions in {1:d} min {2:d} sec'.format(count, elapsed // 60, elapsed % 60))
+    print('# [{0}] Rename {1} file extensions in {2:d} min {3:d} sec'.format(base_path, count, elapsed // 60,
+                                                                             elapsed % 60))
 
 
-def organise_raw():
+def organise_raw(base_path):
     """
     Move RAW to sub folder
     """
     start = time.time()
     count = 0
-    raw_path = 'RAW'
+    raw_path = Path(base_path, 'RAW')
     extensions = ('.RAF', '.CR2',)
-    files = [i for i in iter_files('.') if i.suffix in extensions]
-    if not Path(raw_path).exists() and files:
-        Path(raw_path).mkdir()
+    files = [i for i in iter_files(base_path) if i.suffix in extensions]
+    if not raw_path.exists() and files:
+        raw_path.mkdir()
     for f in files:
-        f.rename(f.parent / raw_path / f.name)
-        print('Move {} '.format(f.name))
+        f.rename(raw_path / f.name)
+        print('[{0}] Move {1} '.format(base_path, f.name))
         count += 1
     elapsed = int(time.time() - start)
-    print('# Move {0} raw files in {1:d} min {2:d} sec'.format(count, elapsed // 60, elapsed % 60))
+    print('# [{0}] Move {1} raw files in {2:d} min {3:d} sec'.format(base_path, count, elapsed // 60, elapsed % 60))
 
 
-def organise_video():
+def organise_video(base_path):
     """
     Move video to sub folder
     """
     start = time.time()
     count = 0
-    video_path = Path('VIDEO')
+    video_path = Path(base_path, 'VIDEO')
     extensions = ('.mov', '.mp4',)
-    files = [i for i in iter_files('.') if i.suffix in extensions]
+    files = [i for i in iter_files(base_path) if i.suffix in extensions]
     if not video_path.exists() and files:
         video_path.mkdir()
     for f in files:
-        f.rename(f.parent / video_path / f.name)
-        print('Move {} '.format(f.name))
+        f.rename(video_path / f.name)
+        print('[{0}] Move {1} '.format(base_path, f.name))
         count += 1
     elapsed = int(time.time() - start)
-    print('# Move {0} video files in {1:d} min {2:d} sec'.format(count, elapsed // 60, elapsed % 60))
+    print('# [{0}] Move {1} video files in {2:d} min {3:d} sec'.format(base_path, count, elapsed // 60, elapsed % 60))
 
 
 def merge_raws(force=False):
     start = time.time()
     raw_path = 'RAW'
     jpgs = {i.stem for i in iter_files('.')}
     raws = {i.stem for i in iter_files(raw_path)}
@@ -73,15 +73,19 @@
     if len(diff):
         print('Diff: ' + ', '.join(sorted(diff)))
         answer = 'y' if force else input('Are you sure to move to trash {} photos?(y/n): '.format(len(diff)))
         if answer == 'y':
             for raw_name in diff:
                 paths = Path(raw_path).glob(raw_name + '.*')
                 for p in paths:
-                    shutil.move(p, Path.home() / ".Trash" / p.name)
+                    code = script(f'tell app "Finder" to move (the POSIX file "{p.absolute().as_posix()}") to trash',
+                                  with_stdout=False)
+                    if code != 0:
+                        print(f'# Finder return {code} exit code, removing file {p.name}')
+                        p.unlink()
                     moved.append(p.name)
             print('Moved: ' + ', '.join(moved))
         else:
             print('Stop')
     else:
         print('No difference')
     elapsed = int(time.time() - start)
@@ -109,8 +113,11 @@
     paths = paths if paths else ('',)
 
     iterable = chain.from_iterable(iter_files(p, pattern='**/*.jpg') for p in paths)
     files = list(sorted(iterable, key=lambda x: x.name))
     count = len(files)
     args = ' '.join(i.as_posix() for i in files)
     print(f'Count:\t\t{count}')
-    os.system(f'open {args}')
+    if count:
+        os.system(f'open {args}')
+    else:
+        print('No files')
```

### Comparing `b7w-cli-0.1.9/src/b7w_cli/utils.py` & `b7w_cli-0.3.0/src/b7w_cli/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import functools
 import os
 import shlex
+import subprocess
+import sys
 from contextlib import contextmanager
 from pathlib import Path
 from time import time
 
 import toml
 
 DEFAULT_CONFIG = """
@@ -54,14 +56,17 @@
         for path in base.glob(pattern):
             if path.is_file() and not path.match('.*'):
                 yield path
     if base.is_file() and not base.match('.*'):
         yield base
 
 
-def script(text):
+def script(text, with_stdout=True):
     t = shlex.quote(text)
-    return os.system(f'osascript -e {t}')
+    if with_stdout:
+        return os.system(f'osascript -e {t}')
+    else:
+        return os.system(f'osascript -e {t} > /dev/null')
 
 
 def notification(title, text):
     script(f'display notification "{text}" with title "{title}"')
```

### Comparing `b7w-cli-0.1.9/src/b7w_cli/video.py` & `b7w_cli-0.3.0/src/b7w_cli/video.py`

 * *Files identical despite different names*

### Comparing `b7w-cli-0.1.9/PKG-INFO` & `b7w_cli-0.3.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: b7w-cli
-Version: 0.1.9
+Version: 0.3.0
 Summary: Useful cli for photos and other things
 Home-page: https://github.com/b7w/b7w-cli
 License: MIT
 Author: B7W
 Author-email: b7w@isudo.ru
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: click (>=8.1,<9.0)
+Requires-Dist: python-dateutil (>=2.9,<3.0)
 Requires-Dist: toml (>=0.10.1,<0.11.0)
 Project-URL: Repository, https://github.com/b7w/b7w-cli
 Description-Content-Type: text/markdown
 
 b7w-cli
 =======
```

