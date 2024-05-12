# Comparing `tmp/plex_fuse-0.8.0.tar.gz` & `tmp/plex_fuse-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plex_fuse-0.8.0.tar", last modified: Sat May 11 11:27:48 2024, max compression
+gzip compressed data, was "plex_fuse-0.8.1.tar", last modified: Sat May 11 22:51:01 2024, max compression
```

## Comparing `plex_fuse-0.8.0.tar` & `plex_fuse-0.8.1.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 11:27:48.540728 plex_fuse-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-05-11 11:27:39.000000 plex_fuse-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5461 2024-05-11 11:27:48.540728 plex_fuse-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-05-11 11:27:39.000000 plex_fuse-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 11:27:48.540728 plex_fuse-0.8.0/plex_fuse.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5461 2024-05-11 11:27:48.000000 plex_fuse-0.8.0/plex_fuse.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-05-11 11:27:48.000000 plex_fuse-0.8.0/plex_fuse.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 11:27:48.000000 plex_fuse-0.8.0/plex_fuse.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-11 11:27:48.000000 plex_fuse-0.8.0/plex_fuse.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-11 11:27:48.000000 plex_fuse-0.8.0/plex_fuse.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-11 11:27:48.000000 plex_fuse-0.8.0/plex_fuse.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 11:27:48.536728 plex_fuse-0.8.0/plexfuse/
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-11 11:27:39.000000 plex_fuse-0.8.0/plexfuse/TimeoutLock.py
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-11 11:27:39.000000 plex_fuse-0.8.0/plexfuse/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-11 11:27:39.000000 plex_fuse-0.8.0/plexfuse/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 11:27:48.536728 plex_fuse-0.8.0/plexfuse/cache/
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-11 11:27:39.000000 plex_fuse-0.8.0/plexfuse/cache/CacheControl.py
--rw-r--r--   0 runner    (1001) docker     (127)      926 2024-05-11 11:27:39.000000 plex_fuse-0.8.0/plexfuse/cache/CachedPropertyCacheControl.py
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-05-11 11:27:39.000000 plex_fuse-0.8.0/plexfuse/cache/DelayedPropertyCacheControl.py
--rw-r--r--   0 runner    (1001) docker     (127)      991 2024-05-11 11:27:39.000000 plex_fuse-0.8.0/plexfuse/cache/FileCache.py
--rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-05-11 11:27:39.000000 plex_fuse-0.8.0/plexfuse/cache/HttpCache.py
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-05-11 11:27:39.000000 plex_fuse-0.8.0/plexfuse/cache/UserDictCacheControl.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 11:27:48.536728 plex_fuse-0.8.0/plexfuse/control/
--rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-05-11 11:27:39.000000 plex_fuse-0.8.0/plexfuse/control/Control.py
--rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-05-11 11:27:39.000000 plex_fuse-0.8.0/plexfuse/control/ControlListener.py
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-11 11:27:39.000000 plex_fuse-0.8.0/plexfuse/control/ControlVFS.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 11:27:48.536728 plex_fuse-0.8.0/plexfuse/fs/
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-11 11:27:39.000000 plex_fuse-0.8.0/plexfuse/fs/FsOptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-11 11:27:39.000000 plex_fuse-0.8.0/plexfuse/fs/PlexDirectory.py
--rw-r--r--   0 runner    (1001) docker     (127)     3987 2024-05-11 11:27:39.000000 plex_fuse-0.8.0/plexfuse/fs/PlexFS.py
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-11 11:27:39.000000 plex_fuse-0.8.0/plexfuse/fs/PlexFile.py
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-11 11:27:39.000000 plex_fuse-0.8.0/plexfuse/fs/RefCountedDict.py
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-11 11:27:39.000000 plex_fuse-0.8.0/plexfuse/fs/Timestampable.py
--rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-05-11 11:27:39.000000 plex_fuse-0.8.0/plexfuse/fs/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-05-11 11:27:39.000000 plex_fuse-0.8.0/plexfuse/fs/plex_errno.py
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-11 11:27:39.000000 plex_fuse-0.8.0/plexfuse/normalize.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 11:27:48.536728 plex_fuse-0.8.0/plexfuse/plex/
--rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-05-11 11:27:39.000000 plex_fuse-0.8.0/plexfuse/plex/Monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     7444 2024-05-11 11:27:39.000000 plex_fuse-0.8.0/plexfuse/plex/PlexApi.py
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-11 11:27:39.000000 plex_fuse-0.8.0/plexfuse/plex/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 11:27:48.540728 plex_fuse-0.8.0/plexfuse/vfs/
--rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-05-11 11:27:39.000000 plex_fuse-0.8.0/plexfuse/vfs/ChunkedFile.py
--rw-r--r--   0 runner    (1001) docker     (127)     3030 2024-05-11 11:27:39.000000 plex_fuse-0.8.0/plexfuse/vfs/Playable.py
--rw-r--r--   0 runner    (1001) docker     (127)     3846 2024-05-11 11:27:39.000000 plex_fuse-0.8.0/plexfuse/vfs/PlexVFS.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 11:27:48.540728 plex_fuse-0.8.0/plexfuse/vfs/entry/
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-11 11:27:39.000000 plex_fuse-0.8.0/plexfuse/vfs/entry/AttrEntry.py
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-11 11:27:39.000000 plex_fuse-0.8.0/plexfuse/vfs/entry/ControlSockEntry.py
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-11 11:27:39.000000 plex_fuse-0.8.0/plexfuse/vfs/entry/DirEntry.py
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-11 11:27:39.000000 plex_fuse-0.8.0/plexfuse/vfs/entry/EpisodeEntry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-05-11 11:27:39.000000 plex_fuse-0.8.0/plexfuse/vfs/entry/FileEntry.py
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-05-11 11:27:39.000000 plex_fuse-0.8.0/plexfuse/vfs/entry/LibraryEntry.py
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-11 11:27:39.000000 plex_fuse-0.8.0/plexfuse/vfs/entry/MovieEntry.py
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-11 11:27:39.000000 plex_fuse-0.8.0/plexfuse/vfs/entry/PathEntry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-11 11:27:39.000000 plex_fuse-0.8.0/plexfuse/vfs/entry/PlexMatchEntry.py
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-11 11:27:39.000000 plex_fuse-0.8.0/plexfuse/vfs/entry/SeasonEntry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-05-11 11:27:39.000000 plex_fuse-0.8.0/plexfuse/vfs/entry/SectionEntry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-11 11:27:39.000000 plex_fuse-0.8.0/plexfuse/vfs/entry/SubtitleEntry.py
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-11 11:27:39.000000 plex_fuse-0.8.0/plexfuse/vfs/entry/SymlinkEntry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-05-11 11:27:39.000000 plex_fuse-0.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 11:27:48.540728 plex_fuse-0.8.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 11:27:48.540728 plex_fuse-0.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-11 11:27:39.000000 plex_fuse-0.8.0/tests/test_RefCountedDict.py
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-05-11 11:27:39.000000 plex_fuse-0.8.0/tests/test_chunk_calc.py
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-11 11:27:39.000000 plex_fuse-0.8.0/tests/test_chunk_read.py
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-11 11:27:39.000000 plex_fuse-0.8.0/tests/test_file_copy.py
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-11 11:27:39.000000 plex_fuse-0.8.0/tests/test_file_copy_partial.py
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-05-11 11:27:39.000000 plex_fuse-0.8.0/tests/test_socket_control.py
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-11 11:27:39.000000 plex_fuse-0.8.0/tests/test_timeout_lock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 22:51:01.069550 plex_fuse-0.8.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-05-11 22:50:53.000000 plex_fuse-0.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5461 2024-05-11 22:51:01.065550 plex_fuse-0.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-05-11 22:50:53.000000 plex_fuse-0.8.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 22:51:01.065550 plex_fuse-0.8.1/plex_fuse.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5461 2024-05-11 22:51:01.000000 plex_fuse-0.8.1/plex_fuse.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-05-11 22:51:01.000000 plex_fuse-0.8.1/plex_fuse.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 22:51:01.000000 plex_fuse-0.8.1/plex_fuse.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-11 22:51:01.000000 plex_fuse-0.8.1/plex_fuse.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-11 22:51:01.000000 plex_fuse-0.8.1/plex_fuse.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-11 22:51:01.000000 plex_fuse-0.8.1/plex_fuse.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 22:51:01.061550 plex_fuse-0.8.1/plexfuse/
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-11 22:50:53.000000 plex_fuse-0.8.1/plexfuse/TimeoutLock.py
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-11 22:50:53.000000 plex_fuse-0.8.1/plexfuse/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-11 22:50:53.000000 plex_fuse-0.8.1/plexfuse/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 22:51:01.061550 plex_fuse-0.8.1/plexfuse/cache/
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-11 22:50:53.000000 plex_fuse-0.8.1/plexfuse/cache/CacheControl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-05-11 22:50:53.000000 plex_fuse-0.8.1/plexfuse/cache/CachedPropertyCacheControl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-05-11 22:50:53.000000 plex_fuse-0.8.1/plexfuse/cache/DelayedPropertyCacheControl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-05-11 22:50:53.000000 plex_fuse-0.8.1/plexfuse/cache/FileCache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-05-11 22:50:53.000000 plex_fuse-0.8.1/plexfuse/cache/HttpCache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-05-11 22:50:53.000000 plex_fuse-0.8.1/plexfuse/cache/UserDictCacheControl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 22:51:01.061550 plex_fuse-0.8.1/plexfuse/control/
+-rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-05-11 22:50:53.000000 plex_fuse-0.8.1/plexfuse/control/Control.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-05-11 22:50:53.000000 plex_fuse-0.8.1/plexfuse/control/ControlListener.py
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-11 22:50:53.000000 plex_fuse-0.8.1/plexfuse/control/ControlVFS.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 22:51:01.061550 plex_fuse-0.8.1/plexfuse/fs/
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-11 22:50:53.000000 plex_fuse-0.8.1/plexfuse/fs/FsOptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-11 22:50:53.000000 plex_fuse-0.8.1/plexfuse/fs/PlexDirectory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4165 2024-05-11 22:50:53.000000 plex_fuse-0.8.1/plexfuse/fs/PlexFS.py
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-11 22:50:53.000000 plex_fuse-0.8.1/plexfuse/fs/PlexFile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-11 22:50:53.000000 plex_fuse-0.8.1/plexfuse/fs/RefCountedDict.py
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-11 22:50:53.000000 plex_fuse-0.8.1/plexfuse/fs/Timestampable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-05-11 22:50:53.000000 plex_fuse-0.8.1/plexfuse/fs/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-05-11 22:50:53.000000 plex_fuse-0.8.1/plexfuse/fs/plex_errno.py
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-11 22:50:53.000000 plex_fuse-0.8.1/plexfuse/normalize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 22:51:01.061550 plex_fuse-0.8.1/plexfuse/plex/
+-rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-05-11 22:50:53.000000 plex_fuse-0.8.1/plexfuse/plex/Monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7444 2024-05-11 22:50:53.000000 plex_fuse-0.8.1/plexfuse/plex/PlexApi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-11 22:50:53.000000 plex_fuse-0.8.1/plexfuse/plex/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 22:51:01.065550 plex_fuse-0.8.1/plexfuse/vfs/
+-rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-05-11 22:50:53.000000 plex_fuse-0.8.1/plexfuse/vfs/ChunkedFile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3030 2024-05-11 22:50:53.000000 plex_fuse-0.8.1/plexfuse/vfs/Playable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3846 2024-05-11 22:50:53.000000 plex_fuse-0.8.1/plexfuse/vfs/PlexVFS.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 22:51:01.065550 plex_fuse-0.8.1/plexfuse/vfs/entry/
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-11 22:50:53.000000 plex_fuse-0.8.1/plexfuse/vfs/entry/AttrEntry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-11 22:50:53.000000 plex_fuse-0.8.1/plexfuse/vfs/entry/ControlSockEntry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-11 22:50:53.000000 plex_fuse-0.8.1/plexfuse/vfs/entry/DirEntry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-11 22:50:53.000000 plex_fuse-0.8.1/plexfuse/vfs/entry/EpisodeEntry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-05-11 22:50:53.000000 plex_fuse-0.8.1/plexfuse/vfs/entry/FileEntry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-05-11 22:50:53.000000 plex_fuse-0.8.1/plexfuse/vfs/entry/LibraryEntry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-11 22:50:53.000000 plex_fuse-0.8.1/plexfuse/vfs/entry/MovieEntry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-11 22:50:53.000000 plex_fuse-0.8.1/plexfuse/vfs/entry/PathEntry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-11 22:50:53.000000 plex_fuse-0.8.1/plexfuse/vfs/entry/PlexMatchEntry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-11 22:50:53.000000 plex_fuse-0.8.1/plexfuse/vfs/entry/SeasonEntry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-05-11 22:50:53.000000 plex_fuse-0.8.1/plexfuse/vfs/entry/SectionEntry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-11 22:50:53.000000 plex_fuse-0.8.1/plexfuse/vfs/entry/SubtitleEntry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-11 22:50:53.000000 plex_fuse-0.8.1/plexfuse/vfs/entry/SymlinkEntry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-05-11 22:50:53.000000 plex_fuse-0.8.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 22:51:01.069550 plex_fuse-0.8.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 22:51:01.065550 plex_fuse-0.8.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-11 22:50:53.000000 plex_fuse-0.8.1/tests/test_RefCountedDict.py
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-05-11 22:50:53.000000 plex_fuse-0.8.1/tests/test_chunk_calc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-11 22:50:53.000000 plex_fuse-0.8.1/tests/test_chunk_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-11 22:50:53.000000 plex_fuse-0.8.1/tests/test_file_copy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-11 22:50:53.000000 plex_fuse-0.8.1/tests/test_file_copy_partial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-05-11 22:50:53.000000 plex_fuse-0.8.1/tests/test_socket_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-11 22:50:53.000000 plex_fuse-0.8.1/tests/test_timeout_lock.py
```

### Comparing `plex_fuse-0.8.0/LICENSE` & `plex_fuse-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `plex_fuse-0.8.0/PKG-INFO` & `plex_fuse-0.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plex-fuse
-Version: 0.8.0
+Version: 0.8.1
 Summary: Plex FUSE Filesystem - Mount Remote Plex Media Server contents as local filesystem
 Author-email: Elan Ruusamäe <glen@pld-linux.org>
 License: BSD 3-Clause License
         
         Copyright (c) 2023-2024, Elan Ruusamäe
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `plex_fuse-0.8.0/README.md` & `plex_fuse-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `plex_fuse-0.8.0/plex_fuse.egg-info/PKG-INFO` & `plex_fuse-0.8.1/plex_fuse.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plex-fuse
-Version: 0.8.0
+Version: 0.8.1
 Summary: Plex FUSE Filesystem - Mount Remote Plex Media Server contents as local filesystem
 Author-email: Elan Ruusamäe <glen@pld-linux.org>
 License: BSD 3-Clause License
         
         Copyright (c) 2023-2024, Elan Ruusamäe
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `plex_fuse-0.8.0/plex_fuse.egg-info/SOURCES.txt` & `plex_fuse-0.8.1/plex_fuse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `plex_fuse-0.8.0/plexfuse/TimeoutLock.py` & `plex_fuse-0.8.1/plexfuse/TimeoutLock.py`

 * *Files identical despite different names*

### Comparing `plex_fuse-0.8.0/plexfuse/cache/CacheControl.py` & `plex_fuse-0.8.1/plexfuse/cache/CacheControl.py`

 * *Files identical despite different names*

### Comparing `plex_fuse-0.8.0/plexfuse/cache/CachedPropertyCacheControl.py` & `plex_fuse-0.8.1/plexfuse/cache/CachedPropertyCacheControl.py`

 * *Files identical despite different names*

### Comparing `plex_fuse-0.8.0/plexfuse/cache/DelayedPropertyCacheControl.py` & `plex_fuse-0.8.1/plexfuse/cache/DelayedPropertyCacheControl.py`

 * *Files identical despite different names*

### Comparing `plex_fuse-0.8.0/plexfuse/cache/FileCache.py` & `plex_fuse-0.8.1/plexfuse/cache/FileCache.py`

 * *Files identical despite different names*

### Comparing `plex_fuse-0.8.0/plexfuse/cache/HttpCache.py` & `plex_fuse-0.8.1/plexfuse/cache/HttpCache.py`

 * *Files identical despite different names*

### Comparing `plex_fuse-0.8.0/plexfuse/cache/UserDictCacheControl.py` & `plex_fuse-0.8.1/plexfuse/cache/UserDictCacheControl.py`

 * *Files identical despite different names*

### Comparing `plex_fuse-0.8.0/plexfuse/control/Control.py` & `plex_fuse-0.8.1/plexfuse/control/Control.py`

 * *Files identical despite different names*

### Comparing `plex_fuse-0.8.0/plexfuse/control/ControlListener.py` & `plex_fuse-0.8.1/plexfuse/control/ControlListener.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,30 +49,30 @@
         server = socket.socket(socket.AF_UNIX, socket.SOCK_STREAM)
         server.bind(self.path)
         server.listen()
 
         return server
 
     def close_socket(self):
-        socket = self.socket
+        s = self.socket
         self.socket = None
-        socket.close()
+        s.shutdown(socket.SHUT_RDWR)
+        s.close()
         if os.path.exists(self.path):
             os.unlink(self.path)
 
     def handle(self):
-        while True:
+        while self.socket is not None:
             try:
                 conn, addr = self.socket.accept()
+            except OSError as e:
+                print(e)
+                continue
             except ConnectionAbortedError as e:
                 print(e)
-                # Server is shutting down
-                if not self.socket:
-                    print("No more socket, exiting")
-                    return
                 continue
 
             datagram = conn.recv(128)
             if datagram:
                 tokens = datagram.decode().strip().split()
                 if tokens[0] in self.control.commands:
                     response = self.control.action(tokens[0])
```

### Comparing `plex_fuse-0.8.0/plexfuse/control/ControlVFS.py` & `plex_fuse-0.8.1/plexfuse/control/ControlVFS.py`

 * *Files identical despite different names*

### Comparing `plex_fuse-0.8.0/plexfuse/fs/PlexFS.py` & `plex_fuse-0.8.1/plexfuse/fs/PlexFS.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from plexfuse.fs.plex_errno import plex_errno
 from plexfuse.fs.PlexDirectory import PlexDirectory
 from plexfuse.fs.PlexFile import PlexFile
 from plexfuse.fs.RefCountedDict import RefCountedDict
 from plexfuse.normalize import normalize
 from plexfuse.plex.Monitor import Monitor
 from plexfuse.plex.PlexApi import PlexApi
+from plexfuse.sentry import sentry
 from plexfuse.TimeoutLock import TimeoutLock
 from plexfuse.vfs.entry.DirEntry import DirEntry
 from plexfuse.vfs.PlexVFS import PlexVFS
 
 
 class PlexFS(fuse.Fuse):
     control: ControlListener | None
@@ -45,14 +46,17 @@
         cache_path = self.options.cache_path if self.options.cache_path else PlexApi.CACHE_PATH
         PlexApi.CACHE_PATH = Path(cache_path).absolute()
         PlexApi.HTTP_CACHE = self.options.http_cache
         print(f"fsinit: CACHE_PATH={PlexApi.CACHE_PATH}")
         print(f"fsinit: HTTP_CACHE={PlexApi.HTTP_CACHE}")
         print(f"fsinit: control_path={self.options.control_path}")
         print(f"fsinit: listen_events={self.options.listen_events}")
+        print(f"fsinit: sentry_dsn={self.options.sentry_dsn}")
+        if self.options.sentry_dsn:
+            sentry(self.options.sentry_dsn)
         if self.options.control_path:
             control = Control(self.plex, self, self.vfs)
             self.control = ControlListener(self.options.control_path, control).start()
         if self.options.listen_events:
             self.monitor = Monitor(self.plex).start()
 
     def fsdestroy(self):
```

### Comparing `plex_fuse-0.8.0/plexfuse/fs/RefCountedDict.py` & `plex_fuse-0.8.1/plexfuse/fs/RefCountedDict.py`

 * *Files identical despite different names*

### Comparing `plex_fuse-0.8.0/plexfuse/fs/main.py` & `plex_fuse-0.8.1/plexfuse/fs/main.py`

 * *Files 14% similar despite different names*

```diff
@@ -28,13 +28,16 @@
                              help="cache http requests using requests-cache")
     server.parser.add_option(mountopt="listen_events",
                              default=False, action="store_true",
                              help="listen for events from Plex Media Server")
     server.parser.add_option(mountopt="control_path", metavar="PATH",
                              default=None,
                              help="path to control socket [default: %default]")
+    server.parser.add_option(mountopt="sentry_dsn", metavar="DSN",
+                             default=None,
+                             help="sentry dsn to enable logging to Sentry.io")
     server.parse(values=server.options, errex=1)
     server.main()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `plex_fuse-0.8.0/plexfuse/fs/plex_errno.py` & `plex_fuse-0.8.1/plexfuse/fs/plex_errno.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import errno
 from functools import wraps
 
 import plexapi
 import requests
 import urllib3
 
+from plexfuse.sentry import capture_exception
+
 
 def plex_errno(f):
     # https://stackoverflow.com/questions/28965795/how-can-i-reuse-exception-handling-code-for-multiple-functions-in-python
     """
     handle exceptions from plex setting appropriate errno
     """
 
@@ -17,19 +19,22 @@
         try:
             return f(*args, **kwargs)
         except (urllib3.exceptions.ReadTimeoutError,
                 requests.exceptions.ConnectionError,
                 requests.exceptions.ReadTimeout,
                 TimeoutError) as e:
             print(f"ERROR: Plex: {f.__module__}.{f.__name__}({args[1:]}, {kwargs}): {type(e)}: {e}")
+            capture_exception(e)
             return -errno.ETIMEDOUT
         except plexapi.exceptions.BadRequest as e:
             print(f"ERROR: Plex: {f.__module__}.{f.__name__}({args[1:]}, {kwargs}): {e}")
+            capture_exception(e)
             return -errno.ENETUNREACH
         except KeyError as e:
             print(f"ERROR: Plex: {f.__module__}.{f.__name__}: Unsupported path: {e}")
             return -errno.ENOENT
         except Exception as e:
             print(f"ERROR: Plex: Unknown error {type(e)}: {e}")
+            capture_exception(e)
             return -errno.ENOENT
 
     return decorated
```

### Comparing `plex_fuse-0.8.0/plexfuse/plex/Monitor.py` & `plex_fuse-0.8.1/plexfuse/plex/Monitor.py`

 * *Files identical despite different names*

### Comparing `plex_fuse-0.8.0/plexfuse/plex/PlexApi.py` & `plex_fuse-0.8.1/plexfuse/plex/PlexApi.py`

 * *Files identical despite different names*

### Comparing `plex_fuse-0.8.0/plexfuse/vfs/ChunkedFile.py` & `plex_fuse-0.8.1/plexfuse/vfs/ChunkedFile.py`

 * *Files identical despite different names*

### Comparing `plex_fuse-0.8.0/plexfuse/vfs/Playable.py` & `plex_fuse-0.8.1/plexfuse/vfs/Playable.py`

 * *Files identical despite different names*

### Comparing `plex_fuse-0.8.0/plexfuse/vfs/PlexVFS.py` & `plex_fuse-0.8.1/plexfuse/vfs/PlexVFS.py`

 * *Files identical despite different names*

### Comparing `plex_fuse-0.8.0/plexfuse/vfs/entry/FileEntry.py` & `plex_fuse-0.8.1/plexfuse/vfs/entry/FileEntry.py`

 * *Files identical despite different names*

### Comparing `plex_fuse-0.8.0/plexfuse/vfs/entry/LibraryEntry.py` & `plex_fuse-0.8.1/plexfuse/vfs/entry/LibraryEntry.py`

 * *Files identical despite different names*

### Comparing `plex_fuse-0.8.0/plexfuse/vfs/entry/PlexMatchEntry.py` & `plex_fuse-0.8.1/plexfuse/vfs/entry/PlexMatchEntry.py`

 * *Files identical despite different names*

### Comparing `plex_fuse-0.8.0/plexfuse/vfs/entry/SectionEntry.py` & `plex_fuse-0.8.1/plexfuse/vfs/entry/SectionEntry.py`

 * *Files identical despite different names*

### Comparing `plex_fuse-0.8.0/plexfuse/vfs/entry/SubtitleEntry.py` & `plex_fuse-0.8.1/plexfuse/vfs/entry/SubtitleEntry.py`

 * *Files identical despite different names*

### Comparing `plex_fuse-0.8.0/pyproject.toml` & `plex_fuse-0.8.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `plex_fuse-0.8.0/tests/test_RefCountedDict.py` & `plex_fuse-0.8.1/tests/test_RefCountedDict.py`

 * *Files identical despite different names*

### Comparing `plex_fuse-0.8.0/tests/test_chunk_calc.py` & `plex_fuse-0.8.1/tests/test_chunk_calc.py`

 * *Files identical despite different names*

### Comparing `plex_fuse-0.8.0/tests/test_chunk_read.py` & `plex_fuse-0.8.1/tests/test_chunk_read.py`

 * *Files identical despite different names*

### Comparing `plex_fuse-0.8.0/tests/test_file_copy_partial.py` & `plex_fuse-0.8.1/tests/test_file_copy_partial.py`

 * *Files identical despite different names*

### Comparing `plex_fuse-0.8.0/tests/test_socket_control.py` & `plex_fuse-0.8.1/tests/test_socket_control.py`

 * *Files identical despite different names*

### Comparing `plex_fuse-0.8.0/tests/test_timeout_lock.py` & `plex_fuse-0.8.1/tests/test_timeout_lock.py`

 * *Files identical despite different names*

