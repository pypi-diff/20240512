# Comparing `tmp/jzchatbot-59.83.93.tar.gz` & `tmp/jzchatbot-59.83.94.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jzchatbot-59.83.93.tar", last modified: Sun May 12 09:28:10 2024, max compression
+gzip compressed data, was "jzchatbot-59.83.94.tar", last modified: Sun May 12 09:50:42 2024, max compression
```

## Comparing `jzchatbot-59.83.93.tar` & `jzchatbot-59.83.94.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-12 09:28:10.889255 jzchatbot-59.83.93/
--rw-rw-rw-   0        0        0     1067 2024-05-09 03:25:46.000000 jzchatbot-59.83.93/LICENSE
--rw-rw-rw-   0        0        0      343 2024-05-12 09:28:10.887815 jzchatbot-59.83.93/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-05-10 01:46:29.000000 jzchatbot-59.83.93/README.md
-drwxrwxrwx   0        0        0        0 2024-05-12 09:28:10.861999 jzchatbot-59.83.93/jzchatbot/
--rw-rw-rw-   0        0        0     4145 2024-05-12 09:27:34.000000 jzchatbot-59.83.93/jzchatbot/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-12 09:28:10.886818 jzchatbot-59.83.93/jzchatbot.egg-info/
--rw-rw-rw-   0        0        0      343 2024-05-12 09:28:10.000000 jzchatbot-59.83.93/jzchatbot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      212 2024-05-12 09:28:10.000000 jzchatbot-59.83.93/jzchatbot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-12 09:28:10.000000 jzchatbot-59.83.93/jzchatbot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2024-05-12 09:28:10.000000 jzchatbot-59.83.93/jzchatbot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-12 09:28:10.000000 jzchatbot-59.83.93/jzchatbot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-12 09:28:10.889255 jzchatbot-59.83.93/setup.cfg
--rw-rw-rw-   0        0        0      530 2024-05-12 09:27:59.000000 jzchatbot-59.83.93/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-12 09:50:42.861928 jzchatbot-59.83.94/
+-rw-rw-rw-   0        0        0     1067 2024-05-09 03:25:46.000000 jzchatbot-59.83.94/LICENSE
+-rw-rw-rw-   0        0        0      343 2024-05-12 09:50:42.859645 jzchatbot-59.83.94/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-05-10 01:46:29.000000 jzchatbot-59.83.94/README.md
+drwxrwxrwx   0        0        0        0 2024-05-12 09:50:42.837113 jzchatbot-59.83.94/jzchatbot/
+-rw-rw-rw-   0        0        0     5665 2024-05-12 09:49:29.000000 jzchatbot-59.83.94/jzchatbot/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-12 09:50:42.858561 jzchatbot-59.83.94/jzchatbot.egg-info/
+-rw-rw-rw-   0        0        0      343 2024-05-12 09:50:42.000000 jzchatbot-59.83.94/jzchatbot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      212 2024-05-12 09:50:42.000000 jzchatbot-59.83.94/jzchatbot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-12 09:50:42.000000 jzchatbot-59.83.94/jzchatbot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2024-05-12 09:50:42.000000 jzchatbot-59.83.94/jzchatbot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-12 09:50:42.000000 jzchatbot-59.83.94/jzchatbot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-12 09:50:42.861928 jzchatbot-59.83.94/setup.cfg
+-rw-rw-rw-   0        0        0      530 2024-05-12 09:49:56.000000 jzchatbot-59.83.94/setup.py
```

### Comparing `jzchatbot-59.83.93/LICENSE` & `jzchatbot-59.83.94/LICENSE`

 * *Files identical despite different names*

### Comparing `jzchatbot-59.83.93/setup.py` & `jzchatbot-59.83.94/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools 
 
 with open("README.md", "r") as fh: 
 	description = fh.read() 
 
 setuptools.setup( 
 	name="jzchatbot", 
-	version="59.83.93", 
+	version="59.83.94", 
 	author="JZ Enterprises", 
 	packages=setuptools.find_packages(), 
 	description="A package that creates advanced AI chatbots", 
 	long_description=description, 
 	long_description_content_type="text/markdown", 
 	license='MIT', 
 	python_requires='>=3.8',
```

