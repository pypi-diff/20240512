# Comparing `tmp/RootsWeatherProject-1.0.8.tar.gz` & `tmp/RootsWeatherProject-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RootsWeatherProject-1.0.8.tar", last modified: Sun Jan 21 13:40:31 2024, max compression
+gzip compressed data, was "RootsWeatherProject-1.0.9.tar", last modified: Mon Jan 22 07:07:21 2024, max compression
```

## Comparing `RootsWeatherProject-1.0.8.tar` & `RootsWeatherProject-1.0.9.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-21 13:40:31.659129 RootsWeatherProject-1.0.8/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-21 13:40:31.627129 RootsWeatherProject-1.0.8/ImageGrabber/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-21 06:03:55.000000 RootsWeatherProject-1.0.8/ImageGrabber/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-21 13:40:31.627129 RootsWeatherProject-1.0.8/ImageGrabber/imageGrabber/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-21 06:03:55.000000 RootsWeatherProject-1.0.8/ImageGrabber/imageGrabber/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3212 2024-01-21 06:03:55.000000 RootsWeatherProject-1.0.8/ImageGrabber/imageGrabber/grabber.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-21 13:40:31.631129 RootsWeatherProject-1.0.8/ImageResolver/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-21 06:03:55.000000 RootsWeatherProject-1.0.8/ImageResolver/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-21 13:40:31.631129 RootsWeatherProject-1.0.8/ImageResolver/imageResolver/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-21 06:03:55.000000 RootsWeatherProject-1.0.8/ImageResolver/imageResolver/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2924 2024-01-21 12:55:45.000000 RootsWeatherProject-1.0.8/ImageResolver/imageResolver/resolver.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-21 13:40:31.631129 RootsWeatherProject-1.0.8/JobHandler/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-21 06:03:55.000000 RootsWeatherProject-1.0.8/JobHandler/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2831 2024-01-21 10:48:18.000000 RootsWeatherProject-1.0.8/JobHandler/jobHandler.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-21 13:40:31.631129 RootsWeatherProject-1.0.8/JobHandler/managers/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      862 2024-01-21 06:03:55.000000 RootsWeatherProject-1.0.8/JobHandler/managers/RegionURLManager.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-21 06:03:55.000000 RootsWeatherProject-1.0.8/JobHandler/managers/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-21 13:40:31.635129 RootsWeatherProject-1.0.8/LogHandler/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-21 06:03:55.000000 RootsWeatherProject-1.0.8/LogHandler/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      971 2024-01-21 13:40:08.000000 RootsWeatherProject-1.0.8/LogHandler/logHandler.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-21 13:40:31.635129 RootsWeatherProject-1.0.8/ManagerAPI/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       32 2024-01-21 06:03:55.000000 RootsWeatherProject-1.0.8/ManagerAPI/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-21 13:40:31.635129 RootsWeatherProject-1.0.8/ManagerAPI/api/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-21 06:03:55.000000 RootsWeatherProject-1.0.8/ManagerAPI/api/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      300 2024-01-21 06:03:55.000000 RootsWeatherProject-1.0.8/ManagerAPI/api/api.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-21 13:40:31.639129 RootsWeatherProject-1.0.8/ManagerAPI/api/managers/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-21 06:03:55.000000 RootsWeatherProject-1.0.8/ManagerAPI/api/managers/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1367 2024-01-21 06:03:55.000000 RootsWeatherProject-1.0.8/ManagerAPI/api/managers/connection_manager.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3647 2024-01-21 06:03:55.000000 RootsWeatherProject-1.0.8/ManagerAPI/api/managers/job_manager.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      656 2024-01-21 06:03:55.000000 RootsWeatherProject-1.0.8/ManagerAPI/api/managers/state_manager.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-21 13:40:31.639129 RootsWeatherProject-1.0.8/ManagerAPI/api/models/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-21 06:03:55.000000 RootsWeatherProject-1.0.8/ManagerAPI/api/models/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      878 2024-01-21 06:03:55.000000 RootsWeatherProject-1.0.8/ManagerAPI/api/models/managedJob.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-21 13:40:31.643129 RootsWeatherProject-1.0.8/ManagerAPI/api/routers/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-21 06:03:55.000000 RootsWeatherProject-1.0.8/ManagerAPI/api/routers/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2050 2024-01-21 09:22:43.000000 RootsWeatherProject-1.0.8/ManagerAPI/api/routers/auth.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3293 2024-01-21 06:03:55.000000 RootsWeatherProject-1.0.8/ManagerAPI/api/routers/jobs.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      385 2024-01-21 08:46:00.000000 RootsWeatherProject-1.0.8/ManagerAPI/server.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      523 2024-01-21 13:40:31.659129 RootsWeatherProject-1.0.8/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1277 2024-01-21 07:15:57.000000 RootsWeatherProject-1.0.8/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-21 13:40:31.647129 RootsWeatherProject-1.0.8/RootsWeatherProject.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      523 2024-01-21 13:40:31.000000 RootsWeatherProject-1.0.8/RootsWeatherProject.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1638 2024-01-21 13:40:31.000000 RootsWeatherProject-1.0.8/RootsWeatherProject.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-01-21 13:40:31.000000 RootsWeatherProject-1.0.8/RootsWeatherProject.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      286 2024-01-21 13:40:31.000000 RootsWeatherProject-1.0.8/RootsWeatherProject.egg-info/entry_points.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      143 2024-01-21 13:40:31.000000 RootsWeatherProject-1.0.8/RootsWeatherProject.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       91 2024-01-21 13:40:31.000000 RootsWeatherProject-1.0.8/RootsWeatherProject.egg-info/top_level.txt
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-21 13:40:31.647129 RootsWeatherProject-1.0.8/VideoMaker/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-21 06:03:55.000000 RootsWeatherProject-1.0.8/VideoMaker/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-21 13:40:31.647129 RootsWeatherProject-1.0.8/VideoMaker/videoMaker/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-21 06:03:55.000000 RootsWeatherProject-1.0.8/VideoMaker/videoMaker/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-21 13:40:31.651129 RootsWeatherProject-1.0.8/VideoMaker/videoMaker/managers/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-21 06:03:55.000000 RootsWeatherProject-1.0.8/VideoMaker/videoMaker/managers/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2770 2024-01-21 07:15:57.000000 RootsWeatherProject-1.0.8/VideoMaker/videoMaker/managers/video_manager.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1894 2024-01-21 06:03:55.000000 RootsWeatherProject-1.0.8/VideoMaker/videoMaker/videomaker.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-21 13:40:31.651129 RootsWeatherProject-1.0.8/VideoUploader/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-21 06:03:55.000000 RootsWeatherProject-1.0.8/VideoUploader/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-21 13:40:31.651129 RootsWeatherProject-1.0.8/VideoUploader/videoUploader/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-21 06:03:55.000000 RootsWeatherProject-1.0.8/VideoUploader/videoUploader/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-21 13:40:31.651129 RootsWeatherProject-1.0.8/VideoUploader/videoUploader/managers/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-21 06:03:55.000000 RootsWeatherProject-1.0.8/VideoUploader/videoUploader/managers/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3727 2024-01-21 06:03:55.000000 RootsWeatherProject-1.0.8/VideoUploader/videoUploader/managers/upload_manager.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2782 2024-01-21 06:03:55.000000 RootsWeatherProject-1.0.8/VideoUploader/videoUploader/uploader.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-01-21 13:40:31.659129 RootsWeatherProject-1.0.8/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1241 2024-01-21 13:40:08.000000 RootsWeatherProject-1.0.8/setup.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-21 13:40:31.659129 RootsWeatherProject-1.0.8/tests/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-21 06:03:55.000000 RootsWeatherProject-1.0.8/tests/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1336 2024-01-21 06:03:55.000000 RootsWeatherProject-1.0.8/tests/test_RegionURLManager.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      255 2024-01-21 06:03:55.000000 RootsWeatherProject-1.0.8/tests/test_api.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3353 2024-01-21 06:03:55.000000 RootsWeatherProject-1.0.8/tests/test_jobhandler.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      877 2024-01-21 13:40:08.000000 RootsWeatherProject-1.0.8/tests/test_loghandler.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-21 06:03:55.000000 RootsWeatherProject-1.0.8/tests/test_router_job.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      998 2024-01-21 06:03:55.000000 RootsWeatherProject-1.0.8/tests/test_state_manager.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-22 07:07:21.118812 RootsWeatherProject-1.0.9/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-22 07:07:21.086813 RootsWeatherProject-1.0.9/ImageGrabber/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-21 06:03:55.000000 RootsWeatherProject-1.0.9/ImageGrabber/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-22 07:07:21.086813 RootsWeatherProject-1.0.9/ImageGrabber/imageGrabber/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-21 06:03:55.000000 RootsWeatherProject-1.0.9/ImageGrabber/imageGrabber/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3221 2024-01-22 07:03:44.000000 RootsWeatherProject-1.0.9/ImageGrabber/imageGrabber/grabber.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-22 07:07:21.086813 RootsWeatherProject-1.0.9/ImageResolver/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-21 06:03:55.000000 RootsWeatherProject-1.0.9/ImageResolver/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-22 07:07:21.086813 RootsWeatherProject-1.0.9/ImageResolver/imageResolver/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-21 06:03:55.000000 RootsWeatherProject-1.0.9/ImageResolver/imageResolver/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2924 2024-01-21 12:55:45.000000 RootsWeatherProject-1.0.9/ImageResolver/imageResolver/resolver.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-22 07:07:21.090813 RootsWeatherProject-1.0.9/JobHandler/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-21 06:03:55.000000 RootsWeatherProject-1.0.9/JobHandler/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2831 2024-01-21 10:48:18.000000 RootsWeatherProject-1.0.9/JobHandler/jobHandler.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-22 07:07:21.090813 RootsWeatherProject-1.0.9/JobHandler/managers/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      862 2024-01-21 06:03:55.000000 RootsWeatherProject-1.0.9/JobHandler/managers/RegionURLManager.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-21 06:03:55.000000 RootsWeatherProject-1.0.9/JobHandler/managers/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-22 07:07:21.090813 RootsWeatherProject-1.0.9/LogHandler/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-21 06:03:55.000000 RootsWeatherProject-1.0.9/LogHandler/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      971 2024-01-21 13:40:08.000000 RootsWeatherProject-1.0.9/LogHandler/logHandler.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-22 07:07:21.094812 RootsWeatherProject-1.0.9/ManagerAPI/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       32 2024-01-21 06:03:55.000000 RootsWeatherProject-1.0.9/ManagerAPI/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-22 07:07:21.094812 RootsWeatherProject-1.0.9/ManagerAPI/api/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-21 06:03:55.000000 RootsWeatherProject-1.0.9/ManagerAPI/api/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      300 2024-01-21 06:03:55.000000 RootsWeatherProject-1.0.9/ManagerAPI/api/api.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-22 07:07:21.098812 RootsWeatherProject-1.0.9/ManagerAPI/api/managers/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-21 06:03:55.000000 RootsWeatherProject-1.0.9/ManagerAPI/api/managers/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1367 2024-01-21 06:03:55.000000 RootsWeatherProject-1.0.9/ManagerAPI/api/managers/connection_manager.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3647 2024-01-21 06:03:55.000000 RootsWeatherProject-1.0.9/ManagerAPI/api/managers/job_manager.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      656 2024-01-21 06:03:55.000000 RootsWeatherProject-1.0.9/ManagerAPI/api/managers/state_manager.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-22 07:07:21.098812 RootsWeatherProject-1.0.9/ManagerAPI/api/models/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-21 06:03:55.000000 RootsWeatherProject-1.0.9/ManagerAPI/api/models/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      878 2024-01-21 06:03:55.000000 RootsWeatherProject-1.0.9/ManagerAPI/api/models/managedJob.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-22 07:07:21.098812 RootsWeatherProject-1.0.9/ManagerAPI/api/routers/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-21 06:03:55.000000 RootsWeatherProject-1.0.9/ManagerAPI/api/routers/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2050 2024-01-21 09:22:43.000000 RootsWeatherProject-1.0.9/ManagerAPI/api/routers/auth.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3293 2024-01-21 06:03:55.000000 RootsWeatherProject-1.0.9/ManagerAPI/api/routers/jobs.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      385 2024-01-21 08:46:00.000000 RootsWeatherProject-1.0.9/ManagerAPI/server.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      523 2024-01-22 07:07:21.118812 RootsWeatherProject-1.0.9/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1277 2024-01-21 07:15:57.000000 RootsWeatherProject-1.0.9/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-22 07:07:21.102812 RootsWeatherProject-1.0.9/RootsWeatherProject.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      523 2024-01-22 07:07:20.000000 RootsWeatherProject-1.0.9/RootsWeatherProject.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1638 2024-01-22 07:07:20.000000 RootsWeatherProject-1.0.9/RootsWeatherProject.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-01-22 07:07:20.000000 RootsWeatherProject-1.0.9/RootsWeatherProject.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      286 2024-01-22 07:07:20.000000 RootsWeatherProject-1.0.9/RootsWeatherProject.egg-info/entry_points.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      143 2024-01-22 07:07:20.000000 RootsWeatherProject-1.0.9/RootsWeatherProject.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       91 2024-01-22 07:07:20.000000 RootsWeatherProject-1.0.9/RootsWeatherProject.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-22 07:07:21.106812 RootsWeatherProject-1.0.9/VideoMaker/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-21 06:03:55.000000 RootsWeatherProject-1.0.9/VideoMaker/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-22 07:07:21.106812 RootsWeatherProject-1.0.9/VideoMaker/videoMaker/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-21 06:03:55.000000 RootsWeatherProject-1.0.9/VideoMaker/videoMaker/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-22 07:07:21.106812 RootsWeatherProject-1.0.9/VideoMaker/videoMaker/managers/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-21 06:03:55.000000 RootsWeatherProject-1.0.9/VideoMaker/videoMaker/managers/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2770 2024-01-21 07:15:57.000000 RootsWeatherProject-1.0.9/VideoMaker/videoMaker/managers/video_manager.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1894 2024-01-21 06:03:55.000000 RootsWeatherProject-1.0.9/VideoMaker/videoMaker/videomaker.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-22 07:07:21.110812 RootsWeatherProject-1.0.9/VideoUploader/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-21 06:03:55.000000 RootsWeatherProject-1.0.9/VideoUploader/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-22 07:07:21.110812 RootsWeatherProject-1.0.9/VideoUploader/videoUploader/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-21 06:03:55.000000 RootsWeatherProject-1.0.9/VideoUploader/videoUploader/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-22 07:07:21.110812 RootsWeatherProject-1.0.9/VideoUploader/videoUploader/managers/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-21 06:03:55.000000 RootsWeatherProject-1.0.9/VideoUploader/videoUploader/managers/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3727 2024-01-21 06:03:55.000000 RootsWeatherProject-1.0.9/VideoUploader/videoUploader/managers/upload_manager.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2782 2024-01-21 06:03:55.000000 RootsWeatherProject-1.0.9/VideoUploader/videoUploader/uploader.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-01-22 07:07:21.118812 RootsWeatherProject-1.0.9/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1241 2024-01-22 07:06:49.000000 RootsWeatherProject-1.0.9/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-22 07:07:21.118812 RootsWeatherProject-1.0.9/tests/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-21 06:03:55.000000 RootsWeatherProject-1.0.9/tests/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1336 2024-01-21 06:03:55.000000 RootsWeatherProject-1.0.9/tests/test_RegionURLManager.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      255 2024-01-21 06:03:55.000000 RootsWeatherProject-1.0.9/tests/test_api.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3353 2024-01-21 06:03:55.000000 RootsWeatherProject-1.0.9/tests/test_jobhandler.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      877 2024-01-21 13:40:08.000000 RootsWeatherProject-1.0.9/tests/test_loghandler.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-21 06:03:55.000000 RootsWeatherProject-1.0.9/tests/test_router_job.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      998 2024-01-21 06:03:55.000000 RootsWeatherProject-1.0.9/tests/test_state_manager.py
```

### Comparing `RootsWeatherProject-1.0.8/ImageGrabber/imageGrabber/grabber.py` & `RootsWeatherProject-1.0.9/ImageGrabber/imageGrabber/grabber.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,24 +5,25 @@
 
 import logging as log
 from time import sleep
 import requests
 import os
 import threading
 
-IMAGE_DIR = os.getenv("IMAGE_DESTINATION", "./images")
 
 '''
 Iterate over the image links and download the images to the attached longhorn volume at /images
 '''
 
 
 def grab_images(job: ManagedJobModel, request_base_url: str, request_timeout: int = 10, max_threads: int = 10):
 
     log.info(f'Grabbing images for job: {job.job_id}')
+    
+    IMAGE_DIR = os.getenv("IMAGE_DESTINATION", "./images")
 
     IMAGE_DESTINATION = f'{IMAGE_DIR}/{job.job_id}/'
     if not os.path.exists(IMAGE_DESTINATION):
         os.makedirs(IMAGE_DESTINATION)
 
     def download_image(image_name):
         url = request_base_url + image_name
```

### Comparing `RootsWeatherProject-1.0.8/ImageResolver/imageResolver/resolver.py` & `RootsWeatherProject-1.0.9/ImageResolver/imageResolver/resolver.py`

 * *Files identical despite different names*

### Comparing `RootsWeatherProject-1.0.8/JobHandler/jobHandler.py` & `RootsWeatherProject-1.0.9/JobHandler/jobHandler.py`

 * *Files identical despite different names*

### Comparing `RootsWeatherProject-1.0.8/JobHandler/managers/RegionURLManager.py` & `RootsWeatherProject-1.0.9/JobHandler/managers/RegionURLManager.py`

 * *Files identical despite different names*

### Comparing `RootsWeatherProject-1.0.8/LogHandler/logHandler.py` & `RootsWeatherProject-1.0.9/LogHandler/logHandler.py`

 * *Files identical despite different names*

### Comparing `RootsWeatherProject-1.0.8/ManagerAPI/api/managers/connection_manager.py` & `RootsWeatherProject-1.0.9/ManagerAPI/api/managers/connection_manager.py`

 * *Files identical despite different names*

### Comparing `RootsWeatherProject-1.0.8/ManagerAPI/api/managers/job_manager.py` & `RootsWeatherProject-1.0.9/ManagerAPI/api/managers/job_manager.py`

 * *Files identical despite different names*

### Comparing `RootsWeatherProject-1.0.8/ManagerAPI/api/managers/state_manager.py` & `RootsWeatherProject-1.0.9/ManagerAPI/api/managers/state_manager.py`

 * *Files identical despite different names*

### Comparing `RootsWeatherProject-1.0.8/ManagerAPI/api/models/managedJob.py` & `RootsWeatherProject-1.0.9/ManagerAPI/api/models/managedJob.py`

 * *Files identical despite different names*

### Comparing `RootsWeatherProject-1.0.8/ManagerAPI/api/routers/auth.py` & `RootsWeatherProject-1.0.9/ManagerAPI/api/routers/auth.py`

 * *Files identical despite different names*

### Comparing `RootsWeatherProject-1.0.8/ManagerAPI/api/routers/jobs.py` & `RootsWeatherProject-1.0.9/ManagerAPI/api/routers/jobs.py`

 * *Files identical despite different names*

### Comparing `RootsWeatherProject-1.0.8/PKG-INFO` & `RootsWeatherProject-1.0.9/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RootsWeatherProject
-Version: 1.0.8
+Version: 1.0.9
 Summary: A package holding microservices to create video from compiled weather image data
 Home-page: https://github.com/johncanthony/RootsWeatherProject
 Author: John Anthony
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `RootsWeatherProject-1.0.8/README.md` & `RootsWeatherProject-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `RootsWeatherProject-1.0.8/RootsWeatherProject.egg-info/PKG-INFO` & `RootsWeatherProject-1.0.9/RootsWeatherProject.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RootsWeatherProject
-Version: 1.0.8
+Version: 1.0.9
 Summary: A package holding microservices to create video from compiled weather image data
 Home-page: https://github.com/johncanthony/RootsWeatherProject
 Author: John Anthony
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `RootsWeatherProject-1.0.8/RootsWeatherProject.egg-info/SOURCES.txt` & `RootsWeatherProject-1.0.9/RootsWeatherProject.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `RootsWeatherProject-1.0.8/VideoMaker/videoMaker/managers/video_manager.py` & `RootsWeatherProject-1.0.9/VideoMaker/videoMaker/managers/video_manager.py`

 * *Files identical despite different names*

### Comparing `RootsWeatherProject-1.0.8/VideoMaker/videoMaker/videomaker.py` & `RootsWeatherProject-1.0.9/VideoMaker/videoMaker/videomaker.py`

 * *Files identical despite different names*

### Comparing `RootsWeatherProject-1.0.8/VideoUploader/videoUploader/managers/upload_manager.py` & `RootsWeatherProject-1.0.9/VideoUploader/videoUploader/managers/upload_manager.py`

 * *Files identical despite different names*

### Comparing `RootsWeatherProject-1.0.8/VideoUploader/videoUploader/uploader.py` & `RootsWeatherProject-1.0.9/VideoUploader/videoUploader/uploader.py`

 * *Files identical despite different names*

### Comparing `RootsWeatherProject-1.0.8/setup.py` & `RootsWeatherProject-1.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='RootsWeatherProject',
-    version='1.0.8',
+    version='1.0.9',
     packages=find_packages(),
     install_requires=['pytest', 'fastapi', 'pydantic', 'uvicorn', 'httpx', 'redis', 'requests',
                       'beautifulsoup4', 'bs4', 'setuptools', 'ffmpeg-python', 'google_auth_oauthlib',
                       'google-api-python-client'],
     author='John Anthony',
     description='A package holding microservices to create video from compiled weather image data',
     url='https://github.com/johncanthony/RootsWeatherProject',
```

### Comparing `RootsWeatherProject-1.0.8/tests/test_RegionURLManager.py` & `RootsWeatherProject-1.0.9/tests/test_RegionURLManager.py`

 * *Files identical despite different names*

### Comparing `RootsWeatherProject-1.0.8/tests/test_jobhandler.py` & `RootsWeatherProject-1.0.9/tests/test_jobhandler.py`

 * *Files identical despite different names*

### Comparing `RootsWeatherProject-1.0.8/tests/test_loghandler.py` & `RootsWeatherProject-1.0.9/tests/test_loghandler.py`

 * *Files identical despite different names*

### Comparing `RootsWeatherProject-1.0.8/tests/test_state_manager.py` & `RootsWeatherProject-1.0.9/tests/test_state_manager.py`

 * *Files identical despite different names*

