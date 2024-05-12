# Comparing `tmp/jzchatbot-59.83.95.tar.gz` & `tmp/jzchatbot-59.83.96.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jzchatbot-59.83.95.tar", last modified: Sun May 12 09:53:26 2024, max compression
+gzip compressed data, was "jzchatbot-59.83.96.tar", last modified: Sun May 12 09:59:12 2024, max compression
```

## Comparing `jzchatbot-59.83.95.tar` & `jzchatbot-59.83.96.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-12 09:53:26.691586 jzchatbot-59.83.95/
--rw-rw-rw-   0        0        0     1067 2024-05-09 03:25:46.000000 jzchatbot-59.83.95/LICENSE
--rw-rw-rw-   0        0        0      343 2024-05-12 09:53:26.690068 jzchatbot-59.83.95/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-05-10 01:46:29.000000 jzchatbot-59.83.95/README.md
-drwxrwxrwx   0        0        0        0 2024-05-12 09:53:26.672721 jzchatbot-59.83.95/jzchatbot/
--rw-rw-rw-   0        0        0     5667 2024-05-12 09:53:13.000000 jzchatbot-59.83.95/jzchatbot/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-12 09:53:26.688298 jzchatbot-59.83.95/jzchatbot.egg-info/
--rw-rw-rw-   0        0        0      343 2024-05-12 09:53:26.000000 jzchatbot-59.83.95/jzchatbot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      212 2024-05-12 09:53:26.000000 jzchatbot-59.83.95/jzchatbot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-12 09:53:26.000000 jzchatbot-59.83.95/jzchatbot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2024-05-12 09:53:26.000000 jzchatbot-59.83.95/jzchatbot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-12 09:53:26.000000 jzchatbot-59.83.95/jzchatbot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-12 09:53:26.691586 jzchatbot-59.83.95/setup.cfg
--rw-rw-rw-   0        0        0      530 2024-05-12 09:53:19.000000 jzchatbot-59.83.95/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-12 09:59:12.120389 jzchatbot-59.83.96/
+-rw-rw-rw-   0        0        0     1067 2024-05-09 03:25:46.000000 jzchatbot-59.83.96/LICENSE
+-rw-rw-rw-   0        0        0      343 2024-05-12 09:59:12.118642 jzchatbot-59.83.96/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-05-10 01:46:29.000000 jzchatbot-59.83.96/README.md
+drwxrwxrwx   0        0        0        0 2024-05-12 09:59:12.101419 jzchatbot-59.83.96/jzchatbot/
+-rw-rw-rw-   0        0        0     5664 2024-05-12 09:58:55.000000 jzchatbot-59.83.96/jzchatbot/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-12 09:59:12.117632 jzchatbot-59.83.96/jzchatbot.egg-info/
+-rw-rw-rw-   0        0        0      343 2024-05-12 09:59:11.000000 jzchatbot-59.83.96/jzchatbot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      212 2024-05-12 09:59:12.000000 jzchatbot-59.83.96/jzchatbot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-12 09:59:11.000000 jzchatbot-59.83.96/jzchatbot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2024-05-12 09:59:11.000000 jzchatbot-59.83.96/jzchatbot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-12 09:59:11.000000 jzchatbot-59.83.96/jzchatbot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-12 09:59:12.120389 jzchatbot-59.83.96/setup.cfg
+-rw-rw-rw-   0        0        0      530 2024-05-12 09:59:06.000000 jzchatbot-59.83.96/setup.py
```

### Comparing `jzchatbot-59.83.95/LICENSE` & `jzchatbot-59.83.96/LICENSE`

 * *Files identical despite different names*

### Comparing `jzchatbot-59.83.95/jzchatbot/__init__.py` & `jzchatbot-59.83.96/jzchatbot/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,17 +132,18 @@
         except sr.UnknownValueError:
             print("JZ: Sorry, I could not understand your speech.")
             return ""
         except sr.RequestError as e:
             print("JZ: Speech recognition request failed:", e)
             return ""
 
-    def usrinput(self):
+    def run(self):
         while True:
             user_input = self.listen_for_input()  # Listen for user speech input
             if user_input.lower() == 'exit':
                 break
             if user_input:
                 bot_response = self.generate_response(user_input)
                 print(f"{self.name}: {bot_response}")
                 self.speak(bot_response)
 
+
```

### Comparing `jzchatbot-59.83.95/setup.py` & `jzchatbot-59.83.96/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools 
 
 with open("README.md", "r") as fh: 
 	description = fh.read() 
 
 setuptools.setup( 
 	name="jzchatbot", 
-	version="59.83.95", 
+	version="59.83.96", 
 	author="JZ Enterprises", 
 	packages=setuptools.find_packages(), 
 	description="A package that creates advanced AI chatbots", 
 	long_description=description, 
 	long_description_content_type="text/markdown", 
 	license='MIT', 
 	python_requires='>=3.8',
```

