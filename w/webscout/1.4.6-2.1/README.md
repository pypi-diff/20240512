# Comparing `tmp/webscout-1.4.6.tar.gz` & `tmp/webscout-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webscout-1.4.6.tar", last modified: Fri May 10 15:14:11 2024, max compression
+gzip compressed data, was "webscout-2.1.tar", last modified: Sat May 11 10:54:09 2024, max compression
```

## Comparing `webscout-1.4.6.tar` & `webscout-2.1.tar`

### file list

```diff
@@ -1,51 +1,68 @@
-drwxrwxrwx   0        0        0        0 2024-05-10 15:14:11.541437 webscout-1.4.6/
-drwxrwxrwx   0        0        0        0 2024-05-10 15:14:11.238857 webscout-1.4.6/DeepWEBS/
--rw-rw-rw-   0        0        0        0 2024-05-08 15:52:48.000000 webscout-1.4.6/DeepWEBS/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-10 15:14:11.254874 webscout-1.4.6/DeepWEBS/documents/
--rw-rw-rw-   0        0        0        0 2024-05-08 15:52:48.000000 webscout-1.4.6/DeepWEBS/documents/__init__.py
--rw-rw-rw-   0        0        0     4049 2024-05-08 15:52:48.000000 webscout-1.4.6/DeepWEBS/documents/query_results_extractor.py
--rw-rw-rw-   0        0        0     5272 2024-05-08 15:52:48.000000 webscout-1.4.6/DeepWEBS/documents/webpage_content_extractor.py
-drwxrwxrwx   0        0        0        0 2024-05-10 15:14:11.297797 webscout-1.4.6/DeepWEBS/networks/
--rw-rw-rw-   0        0        0        0 2024-05-08 15:52:48.000000 webscout-1.4.6/DeepWEBS/networks/__init__.py
--rw-rw-rw-   0        0        0     3183 2024-05-08 15:52:48.000000 webscout-1.4.6/DeepWEBS/networks/filepath_converter.py
--rw-rw-rw-   0        0        0     1966 2024-05-08 15:52:48.000000 webscout-1.4.6/DeepWEBS/networks/google_searcher.py
--rw-rw-rw-   0        0        0      726 2024-05-08 15:52:48.000000 webscout-1.4.6/DeepWEBS/networks/network_configs.py
--rw-rw-rw-   0        0        0     3590 2024-05-08 15:52:48.000000 webscout-1.4.6/DeepWEBS/networks/webpage_fetcher.py
-drwxrwxrwx   0        0        0        0 2024-05-10 15:14:11.344177 webscout-1.4.6/DeepWEBS/utilsdw/
--rw-rw-rw-   0        0        0        0 2024-05-08 15:52:48.000000 webscout-1.4.6/DeepWEBS/utilsdw/__init__.py
--rw-rw-rw-   0        0        0     2472 2024-05-08 15:52:48.000000 webscout-1.4.6/DeepWEBS/utilsdw/enver.py
--rw-rw-rw-   0        0        0     8174 2024-05-08 15:52:48.000000 webscout-1.4.6/DeepWEBS/utilsdw/logger.py
--rw-rw-rw-   0        0        0     3150 2024-05-08 15:52:48.000000 webscout-1.4.6/LICENSE.md
--rw-rw-rw-   0        0        0    43356 2024-05-10 15:14:11.536437 webscout-1.4.6/PKG-INFO
--rw-rw-rw-   0        0        0    41114 2024-05-10 02:21:13.000000 webscout-1.4.6/README.md
--rw-rw-rw-   0        0        0       42 2024-05-10 15:14:11.544441 webscout-1.4.6/setup.cfg
--rw-rw-rw-   0        0        0     2741 2024-05-10 15:13:41.000000 webscout-1.4.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-10 15:14:11.485783 webscout-1.4.6/webscout/
--rw-rw-rw-   0        0        0   226181 2024-05-10 14:33:23.000000 webscout-1.4.6/webscout/AI.py
--rw-rw-rw-   0        0        0    17297 2024-05-10 14:45:32.000000 webscout-1.4.6/webscout/AIauto.py
--rw-rw-rw-   0        0        0     4710 2024-05-08 15:52:48.000000 webscout-1.4.6/webscout/AIbase.py
--rw-rw-rw-   0        0        0    33233 2024-05-10 14:47:44.000000 webscout-1.4.6/webscout/AIutel.py
--rw-rw-rw-   0        0        0     7332 2024-05-08 15:52:48.000000 webscout-1.4.6/webscout/DWEBS.py
--rw-rw-rw-   0        0        0     1910 2024-05-08 15:52:48.000000 webscout-1.4.6/webscout/LLM.py
--rw-rw-rw-   0        0        0     1104 2024-05-10 14:47:33.000000 webscout-1.4.6/webscout/__init__.py
--rw-rw-rw-   0        0        0      126 2024-05-08 15:52:48.000000 webscout-1.4.6/webscout/__main__.py
--rw-rw-rw-   0        0        0      711 2024-05-10 14:40:09.000000 webscout-1.4.6/webscout/async_providers.py
--rw-rw-rw-   0        0        0    17059 2024-05-08 15:52:48.000000 webscout-1.4.6/webscout/cli.py
--rw-rw-rw-   0        0        0      498 2024-05-10 14:34:10.000000 webscout-1.4.6/webscout/exceptions.py
--rw-rw-rw-   0        0        0    24489 2024-05-10 14:33:00.000000 webscout-1.4.6/webscout/g4f.py
--rw-rw-rw-   0        0        0      692 2024-05-08 15:52:48.000000 webscout-1.4.6/webscout/models.py
--rw-rw-rw-   0        0        0     5896 2024-05-08 15:52:48.000000 webscout-1.4.6/webscout/tempid.py
--rw-rw-rw-   0        0        0    20622 2024-05-08 15:52:48.000000 webscout-1.4.6/webscout/transcriber.py
--rw-rw-rw-   0        0        0     2603 2024-05-09 03:33:11.000000 webscout-1.4.6/webscout/utils.py
--rw-rw-rw-   0        0        0       25 2024-05-10 04:42:09.000000 webscout-1.4.6/webscout/version.py
--rw-rw-rw-   0        0        0      967 2024-05-08 15:52:48.000000 webscout-1.4.6/webscout/voice.py
--rw-rw-rw-   0        0        0    83660 2024-05-10 14:56:15.000000 webscout-1.4.6/webscout/webai.py
--rw-rw-rw-   0        0        0     3159 2024-05-10 15:13:22.000000 webscout-1.4.6/webscout/webscout_search.py
--rw-rw-rw-   0        0        0    42902 2024-05-10 04:39:59.000000 webscout-1.4.6/webscout/webscout_search_async.py
-drwxrwxrwx   0        0        0        0 2024-05-10 15:14:11.529066 webscout-1.4.6/webscout.egg-info/
--rw-rw-rw-   0        0        0    43356 2024-05-10 15:14:10.000000 webscout-1.4.6/webscout.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1061 2024-05-10 15:14:10.000000 webscout-1.4.6/webscout.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 15:14:10.000000 webscout-1.4.6/webscout.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      197 2024-05-10 15:14:10.000000 webscout-1.4.6/webscout.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      320 2024-05-10 15:14:10.000000 webscout-1.4.6/webscout.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-05-10 15:14:10.000000 webscout-1.4.6/webscout.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-11 10:54:09.808851 webscout-2.1/
+drwxrwxrwx   0        0        0        0 2024-05-11 10:54:09.248842 webscout-2.1/DeepWEBS/
+-rw-rw-rw-   0        0        0        0 2024-05-08 15:52:48.000000 webscout-2.1/DeepWEBS/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-11 10:54:09.261538 webscout-2.1/DeepWEBS/documents/
+-rw-rw-rw-   0        0        0        0 2024-05-08 15:52:48.000000 webscout-2.1/DeepWEBS/documents/__init__.py
+-rw-rw-rw-   0        0        0     4049 2024-05-08 15:52:48.000000 webscout-2.1/DeepWEBS/documents/query_results_extractor.py
+-rw-rw-rw-   0        0        0     5272 2024-05-08 15:52:48.000000 webscout-2.1/DeepWEBS/documents/webpage_content_extractor.py
+drwxrwxrwx   0        0        0        0 2024-05-11 10:54:09.283533 webscout-2.1/DeepWEBS/networks/
+-rw-rw-rw-   0        0        0        0 2024-05-08 15:52:48.000000 webscout-2.1/DeepWEBS/networks/__init__.py
+-rw-rw-rw-   0        0        0     3183 2024-05-08 15:52:48.000000 webscout-2.1/DeepWEBS/networks/filepath_converter.py
+-rw-rw-rw-   0        0        0     1966 2024-05-08 15:52:48.000000 webscout-2.1/DeepWEBS/networks/google_searcher.py
+-rw-rw-rw-   0        0        0      726 2024-05-08 15:52:48.000000 webscout-2.1/DeepWEBS/networks/network_configs.py
+-rw-rw-rw-   0        0        0     3590 2024-05-08 15:52:48.000000 webscout-2.1/DeepWEBS/networks/webpage_fetcher.py
+drwxrwxrwx   0        0        0        0 2024-05-11 10:54:09.296537 webscout-2.1/DeepWEBS/utilsdw/
+-rw-rw-rw-   0        0        0        0 2024-05-08 15:52:48.000000 webscout-2.1/DeepWEBS/utilsdw/__init__.py
+-rw-rw-rw-   0        0        0     2472 2024-05-08 15:52:48.000000 webscout-2.1/DeepWEBS/utilsdw/enver.py
+-rw-rw-rw-   0        0        0     8174 2024-05-08 15:52:48.000000 webscout-2.1/DeepWEBS/utilsdw/logger.py
+-rw-rw-rw-   0        0        0     3150 2024-05-08 15:52:48.000000 webscout-2.1/LICENSE.md
+-rw-rw-rw-   0        0        0    45744 2024-05-11 10:54:09.803849 webscout-2.1/PKG-INFO
+-rw-rw-rw-   0        0        0    43454 2024-05-11 10:39:51.000000 webscout-2.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-11 10:54:09.809853 webscout-2.1/setup.cfg
+-rw-rw-rw-   0        0        0     2781 2024-05-11 10:53:41.000000 webscout-2.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-11 10:54:09.649287 webscout-2.1/webscout/
+-rw-rw-rw-   0        0        0    17297 2024-05-10 14:45:32.000000 webscout-2.1/webscout/AIauto.py
+-rw-rw-rw-   0        0        0     4710 2024-05-08 15:52:48.000000 webscout-2.1/webscout/AIbase.py
+-rw-rw-rw-   0        0        0    33233 2024-05-10 14:47:44.000000 webscout-2.1/webscout/AIutel.py
+-rw-rw-rw-   0        0        0     7332 2024-05-08 15:52:48.000000 webscout-2.1/webscout/DWEBS.py
+-rw-rw-rw-   0        0        0     1910 2024-05-08 15:52:48.000000 webscout-2.1/webscout/LLM.py
+drwxrwxrwx   0        0        0        0 2024-05-11 10:54:09.793853 webscout-2.1/webscout/Provider/
+-rw-rw-rw-   0        0        0    16743 2024-05-11 08:19:16.000000 webscout-2.1/webscout/Provider/Blackboxai.py
+-rw-rw-rw-   0        0        0     8489 2024-05-11 08:19:31.000000 webscout-2.1/webscout/Provider/Cohere.py
+-rw-rw-rw-   0        0        0     8235 2024-05-11 08:19:44.000000 webscout-2.1/webscout/Provider/Gemini.py
+-rw-rw-rw-   0        0        0    20583 2024-05-11 08:19:52.000000 webscout-2.1/webscout/Provider/Groq.py
+-rw-rw-rw-   0        0        0    15405 2024-05-11 08:20:01.000000 webscout-2.1/webscout/Provider/Koboldai.py
+-rw-rw-rw-   0        0        0    19519 2024-05-11 08:20:16.000000 webscout-2.1/webscout/Provider/Leo.py
+-rw-rw-rw-   0        0        0    17089 2024-05-11 08:20:22.000000 webscout-2.1/webscout/Provider/Llama2.py
+-rw-rw-rw-   0        0        0    18404 2024-05-11 08:20:30.000000 webscout-2.1/webscout/Provider/OpenGPT.py
+-rw-rw-rw-   0        0        0    20107 2024-05-11 08:20:26.000000 webscout-2.1/webscout/Provider/Openai.py
+-rw-rw-rw-   0        0        0     8597 2024-05-11 08:20:36.000000 webscout-2.1/webscout/Provider/Perplexity.py
+-rw-rw-rw-   0        0        0    19390 2024-05-11 08:20:42.000000 webscout-2.1/webscout/Provider/Phind.py
+-rw-rw-rw-   0        0        0     8692 2024-05-11 08:20:50.000000 webscout-2.1/webscout/Provider/Reka.py
+-rw-rw-rw-   0        0        0    11616 2024-05-11 08:20:56.000000 webscout-2.1/webscout/Provider/ThinkAnyAI.py
+-rw-rw-rw-   0        0        0     8809 2024-05-11 08:21:00.000000 webscout-2.1/webscout/Provider/Xjai.py
+-rw-rw-rw-   0        0        0    19398 2024-05-11 08:21:06.000000 webscout-2.1/webscout/Provider/Yepchat.py
+-rw-rw-rw-   0        0        0     7756 2024-05-11 08:21:09.000000 webscout-2.1/webscout/Provider/Youchat.py
+-rw-rw-rw-   0        0        0     1223 2024-05-11 10:50:35.000000 webscout-2.1/webscout/Provider/__init__.py
+-rw-rw-rw-   0        0        0     2264 2024-05-11 10:50:52.000000 webscout-2.1/webscout/__init__.py
+-rw-rw-rw-   0        0        0      126 2024-05-08 15:52:48.000000 webscout-2.1/webscout/__main__.py
+-rw-rw-rw-   0        0        0      711 2024-05-10 14:40:09.000000 webscout-2.1/webscout/async_providers.py
+-rw-rw-rw-   0        0        0    17059 2024-05-08 15:52:48.000000 webscout-2.1/webscout/cli.py
+-rw-rw-rw-   0        0        0      498 2024-05-10 14:34:10.000000 webscout-2.1/webscout/exceptions.py
+-rw-rw-rw-   0        0        0    24489 2024-05-10 14:33:00.000000 webscout-2.1/webscout/g4f.py
+-rw-rw-rw-   0        0        0      692 2024-05-08 15:52:48.000000 webscout-2.1/webscout/models.py
+-rw-rw-rw-   0        0        0     5896 2024-05-08 15:52:48.000000 webscout-2.1/webscout/tempid.py
+-rw-rw-rw-   0        0        0    20622 2024-05-08 15:52:48.000000 webscout-2.1/webscout/transcriber.py
+-rw-rw-rw-   0        0        0     2603 2024-05-09 03:33:11.000000 webscout-2.1/webscout/utils.py
+-rw-rw-rw-   0        0        0       23 2024-05-11 09:00:53.000000 webscout-2.1/webscout/version.py
+-rw-rw-rw-   0        0        0      967 2024-05-08 15:52:48.000000 webscout-2.1/webscout/voice.py
+-rw-rw-rw-   0        0        0    84163 2024-05-11 10:17:38.000000 webscout-2.1/webscout/webai.py
+-rw-rw-rw-   0        0        0     3159 2024-05-10 15:13:22.000000 webscout-2.1/webscout/webscout_search.py
+-rw-rw-rw-   0        0        0    42902 2024-05-10 04:39:59.000000 webscout-2.1/webscout/webscout_search_async.py
+drwxrwxrwx   0        0        0        0 2024-05-11 10:54:09.799851 webscout-2.1/webscout.egg-info/
+-rw-rw-rw-   0        0        0    45744 2024-05-11 10:54:08.000000 webscout-2.1/webscout.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1531 2024-05-11 10:54:09.000000 webscout-2.1/webscout.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-11 10:54:08.000000 webscout-2.1/webscout.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      197 2024-05-11 10:54:08.000000 webscout-2.1/webscout.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      338 2024-05-11 10:54:08.000000 webscout-2.1/webscout.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-05-11 10:54:08.000000 webscout-2.1/webscout.egg-info/top_level.txt
```

### Comparing `webscout-1.4.6/DeepWEBS/documents/query_results_extractor.py` & `webscout-2.1/DeepWEBS/documents/query_results_extractor.py`

 * *Files identical despite different names*

### Comparing `webscout-1.4.6/DeepWEBS/documents/webpage_content_extractor.py` & `webscout-2.1/DeepWEBS/documents/webpage_content_extractor.py`

 * *Files identical despite different names*

### Comparing `webscout-1.4.6/DeepWEBS/networks/filepath_converter.py` & `webscout-2.1/DeepWEBS/networks/filepath_converter.py`

 * *Files identical despite different names*

### Comparing `webscout-1.4.6/DeepWEBS/networks/google_searcher.py` & `webscout-2.1/DeepWEBS/networks/google_searcher.py`

 * *Files identical despite different names*

### Comparing `webscout-1.4.6/DeepWEBS/networks/network_configs.py` & `webscout-2.1/DeepWEBS/networks/network_configs.py`

 * *Files identical despite different names*

### Comparing `webscout-1.4.6/DeepWEBS/networks/webpage_fetcher.py` & `webscout-2.1/DeepWEBS/networks/webpage_fetcher.py`

 * *Files identical despite different names*

### Comparing `webscout-1.4.6/DeepWEBS/utilsdw/enver.py` & `webscout-2.1/DeepWEBS/utilsdw/enver.py`

 * *Files identical despite different names*

### Comparing `webscout-1.4.6/DeepWEBS/utilsdw/logger.py` & `webscout-2.1/DeepWEBS/utilsdw/logger.py`

 * *Files identical despite different names*

### Comparing `webscout-1.4.6/LICENSE.md` & `webscout-2.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `webscout-1.4.6/PKG-INFO` & `webscout-2.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webscout
-Version: 1.4.6
+Version: 2.1
 Summary: Search for anything using the Google, DuckDuckGo, phind.com. Also containes AI models, can transcribe yt videos, temporary email and phone number generation, have TTS support and webai(terminal gpt and open interpeter)
 Author: OEvortex
 Author-email: helpingai5@gmail.com
 License: HelpingAI Simplified Universal License
 Project-URL: Documentation, https://github.com/OE-LUCIFER/Webscout/wiki
 Project-URL: Source, https://github.com/OE-LUCIFER/Webscout
 Project-URL: Tracker, https://github.com/OE-LUCIFER/Webscout/issues
@@ -46,29 +46,31 @@
 Requires-Dist: tiktoken
 Requires-Dist: tldextract
 Requires-Dist: orjson
 Requires-Dist: PyYAML
 Requires-Dist: appdirs
 Requires-Dist: GoogleBard1>=2.1.4
 Requires-Dist: tls_client
+Requires-Dist: clipman
+Requires-Dist: playsound
 Provides-Extra: dev
 Requires-Dist: ruff>=0.1.6; extra == "dev"
 Requires-Dist: pytest>=7.4.2; extra == "dev"
 
 <div align="center">
   <!-- Replace `#` with your actual links -->
   <a href="https://t.me/devsdocode"><img alt="Telegram" src="https://img.shields.io/badge/Telegram-2CA5E0?style=for-the-badge&logo=telegram&logoColor=white"></a>
   <a href="https://www.instagram.com/sree.shades_/"><img alt="Instagram" src="https://img.shields.io/badge/Instagram-E4405F?style=for-the-badge&logo=instagram&logoColor=white"></a>
   <a href="https://www.linkedin.com/in/developer-sreejan/"><img alt="LinkedIn" src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"></a>
   <a href="https://buymeacoffee.com/devsdocode"><img alt="Buy Me A Coffee" src="https://img.shields.io/badge/Buy%20Me%20A%20Coffee-FFDD00?style=for-the-badge&logo=buymeacoffee&logoColor=black"></a>
 </div>
 
 <div align="center">
   <!-- Replace `#` with your actual links -->
-  <a href="https://youtube.com/@@OEvortex">&#10148; Vortex's YouTube Channel</a>
+  <a href="https://youtube.com/@OEvortex">&#10148; Vortex's YouTube Channel</a>
   </div>
 <div align="center">
   <a href="https://youtube.com/@devsdocode">&#10148; Devs Do Code's YouTube Channel</a>
 </div>
 
 
 
@@ -86,52 +88,51 @@
 
 
 ## Table of Contents
 - [WEBSCOUT](#webscout)
   - [Table of Contents](#table-of-contents)
   - [Install](#install)
   - [CLI version](#cli-version)
-  - [CLI to use LLM](#cli-to-use-llm)
   - [Regions](#regions)
   - [Tempmail and Temp number](#tempmail-and-temp-number)
     - [Temp number](#temp-number)
     - [Tempmail](#tempmail)
   - [Transcriber](#transcriber)
   - [DeepWEBS: Advanced Web Searches](#deepwebs-advanced-web-searches)
     - [Activating DeepWEBS](#activating-deepwebs)
     - [Point to remember before using `DeepWEBS`](#point-to-remember-before-using-deepwebs)
     - [Usage Example](#usage-example)
   - [Text-to-Speech:](#text-to-speech)
     - [Available TTS Voices:](#available-tts-voices)
-    - [ALL voices:](#all-voices)
-  - [WEBS and AsyncWEBS classes](#webs-and-asyncwebs-classes)
   - [Exceptions](#exceptions)
   - [usage of webscout](#usage-of-webscout)
     - [1. `text()` - text search by DuckDuckGo.com and Yep.com](#1-text---text-search-by-duckduckgocom-and-yepcom)
     - [2. `answers()` - instant answers by DuckDuckGo.com and Yep.com](#2-answers---instant-answers-by-duckduckgocom-and-yepcom)
     - [3. `images()` - image search by DuckDuckGo.com and Yep.com](#3-images---image-search-by-duckduckgocom-and-yepcom)
     - [4. `videos()` - video search by DuckDuckGo.com](#4-videos---video-search-by-duckduckgocom)
     - [5. `news()` - news search by DuckDuckGo.com and yep.com](#5-news---news-search-by-duckduckgocom-and-yepcom)
     - [6. `maps()` - map search by DuckDuckGo.com and](#6-maps---map-search-by-duckduckgocom-and)
     - [7. `translate()` - translation by DuckDuckGo.com and Yep.com](#7-translate---translation-by-duckduckgocom-and-yepcom)
     - [8. `suggestions()` - suggestions by DuckDuckGo.com and Yep.com](#8-suggestions---suggestions-by-duckduckgocom-and-yepcom)
-  - [usage of webscout.AI](#usage-of-webscoutai)
+  - [ALL acts](#all-acts)
+  - [Webscout Supported Acts:](#webscout-supported-acts)
+  - [usage of webscout AI](#usage-of-webscout-ai)
     - [1. `PhindSearch` - Search using Phind.com](#1-phindsearch---search-using-phindcom)
     - [2. `YepChat` - Chat with mistral 8x7b powered by yepchat](#2-yepchat---chat-with-mistral-8x7b-powered-by-yepchat)
     - [3. `You.com` - search/chat with you.com](#3-youcom---searchchat-with-youcom)
     - [4. `Gemini` - search with google gemini](#4-gemini---search-with-google-gemini)
     - [5. `Prodia` - make image using prodia](#5-prodia---make-image-using-prodia)
     - [6. `BlackBox` - Search/chat With BlackBox](#6-blackbox---searchchat-with-blackbox)
     - [7. `PERPLEXITY` - Search With PERPLEXITY](#7-perplexity---search-with-perplexity)
     - [8. `OpenGPT` - chat With OPENGPT](#8-opengpt---chat-with-opengpt)
     - [9. `KOBOLDIA` -](#9-koboldia--)
     - [10. `Reka` - chat with reka](#10-reka---chat-with-reka)
     - [11. `Cohere` - chat with cohere](#11-cohere---chat-with-cohere)
     - [12. `Xjai` - chat with free gpt 3.5](#12-xjai---chat-with-free-gpt-35)
-    - [`ThinkAny` - AI search engine](#thinkany---ai-search-engine)
+    - [13. `ThinkAny` - AI search engine](#13-thinkany---ai-search-engine)
     - [`LLM`](#llm)
     - [`LLM` with internet](#llm-with-internet)
     - [LLM with deepwebs](#llm-with-deepwebs)
   - [`Webai` - terminal gpt and a open interpeter](#webai---terminal-gpt-and-a-open-interpeter)
 
 ## Install
 ```python
@@ -153,18 +154,14 @@
 | python -m webscout text -k Text           | CLI function to perform a text search using Webscout.                                           |
 | python -m webscout translate -k Text      | CLI function to perform translate using Webscout.                                               |
 | python -m webscout version                | A command-line interface command that prints and returns the version of the program.            | 
 | python -m webscout videos -k Text         | CLI function to perform a videos search using DuckDuckGo API.                                   |  
 
 
 
-## CLI to use LLM 
-```python
-python -m webscout.LLM model_name 
-```
 [Go To TOP](#TOP)
 
 ## Regions
 <details>
   <summary>expand</summary>
 
     xa-ar for Arabia
@@ -455,17 +452,15 @@
 with open("output.mp3", "wb") as f:
     f.write(audio_content)
 ```
 ### Available TTS Voices:
 You can choose from a wide range of voices, including:
 - Filiz, Astrid, Tatyana, Maxim, Carmen, Ines, Cristiano, Vitoria, Ricardo, Maja, Jan, Jacek, Ewa, Ruben, Lotte, Liv, Seoyeon, Takumi, Mizuki, Giorgio, Carla, Bianca, Karl, Dora, Mathieu, Celine, Chantal, Penelope, Miguel, Mia, Enrique, Conchita, Geraint, Salli, Matthew, Kimberly, Kendra, Justin, Joey, Joanna, Ivy, Raveena, Aditi, Emma, Brian, Amy, Russell, Nicole, Vicki, Marlene, Hans, Naja, Mads, Gwyneth, Zhiyu
 - Standard and WaveNet voices for various languages (e.g., en-US, es-ES, ja-JP, etc.)
-### ALL voices:
-[Filiz, Astrid, Tatyana, Maxim, Carmen, Ines, Cristiano, Vitoria, Ricardo, Maja, Jan, Jacek, Ewa, Ruben, Lotte, Liv, Seoyeon, Takumi, Mizuki, Giorgio, Carla, Bianca, Karl, Dora, Mathieu, Celine, Chantal, Penelope, Miguel, Mia, Enrique, Conchita, Geraint, Salli, Matthew, Kimberly, Kendra, Justin, Joey, Joanna, Ivy, Raveena, Aditi, Emma, Brian, Amy, Russell, Nicole, Vicki, Marlene, Hans, Naja, Mads, Gwyneth, Zhiyu, es-ES-Standard-A, it-IT-Standard-A, it-IT-Wavenet-A, ja-JP-Standard-A, ja-JP-Wavenet-A, ko-KR-Standard-A, ko-KR-Wavenet-A, pt-BR-Standard-A, tr-TR-Standard-A, sv-SE-Standard-A, nl-NL-Standard-A, nl-NL-Wavenet-A, en-US-Wavenet-A, en-US-Wavenet-B, en-US-Wavenet-C, en-US-Wavenet-D, en-US-Wavenet-E, en-US-Wavenet-F, en-GB-Standard-A, en-GB-Standard-B, en-GB-Standard-C, en-GB-Standard-D, en-GB-Wavenet-A, en-GB-Wavenet-B, en-GB-Wavenet-C, en-GB-Wavenet-D, en-US-Standard-B, en-US-Standard-C, en-US-Standard-D, en-US-Standard-E, de-DE-Standard-A, de-DE-Standard-B, de-DE-Wavenet-A, de-DE-Wavenet-B, de-DE-Wavenet-C, de-DE-Wavenet-D, en-AU-Standard-A, en-AU-Standard-B, en-AU-Wavenet-A, en-AU-Wavenet-B, en-AU-Wavenet-C, en-AU-Wavenet-D, en-AU-Standard-C, en-AU-Standard-D, fr-CA-Standard-A, fr-CA-Standard-B, fr-CA-Standard-C, fr-CA-Standard-D, fr-FR-Standard-C, fr-FR-Standard-D, fr-FR-Wavenet-A, fr-FR-Wavenet-B, fr-FR-Wavenet-C, fr-FR-Wavenet-D, da-DK-Wavenet-A, pl-PL-Wavenet-A, pl-PL-Wavenet-B, pl-PL-Wavenet-C, pl-PL-Wavenet-D, pt-PT-Wavenet-A, pt-PT-Wavenet-B, pt-PT-Wavenet-C, pt-PT-Wavenet-D, ru-RU-Wavenet-A, ru-RU-Wavenet-B, ru-RU-Wavenet-C, ru-RU-Wavenet-D, sk-SK-Wavenet-A, tr-TR-Wavenet-A, tr-TR-Wavenet-B, tr-TR-Wavenet-C, tr-TR-Wavenet-D, tr-TR-Wavenet-E, uk-UA-Wavenet-A, ar-XA-Wavenet-A, ar-XA-Wavenet-B, ar-XA-Wavenet-C, cs-CZ-Wavenet-A, nl-NL-Wavenet-B, nl-NL-Wavenet-C, nl-NL-Wavenet-D, nl-NL-Wavenet-E, en-IN-Wavenet-A, en-IN-Wavenet-B, en-IN-Wavenet-C, fil-PH-Wavenet-A, fi-FI-Wavenet-A, el-GR-Wavenet-A, hi-IN-Wavenet-A, hi-IN-Wavenet-B, hi-IN-Wavenet-C, hu-HU-Wavenet-A, id-ID-Wavenet-A, id-ID-Wavenet-B, id-ID-Wavenet-C, it-IT-Wavenet-B, it-IT-Wavenet-C, it-IT-Wavenet-D, ja-JP-Wavenet-B, ja-JP-Wavenet-C, ja-JP-Wavenet-D, cmn-CN-Wavenet-A, cmn-CN-Wavenet-B, cmn-CN-Wavenet-C, cmn-CN-Wavenet-D, nb-no-Wavenet-E, nb-no-Wavenet-A, nb-no-Wavenet-B, nb-no-Wavenet-C, nb-no-Wavenet-D, vi-VN-Wavenet-A, vi-VN-Wavenet-B, vi-VN-Wavenet-C, vi-VN-Wavenet-D, sr-rs-Standard-A, lv-lv-Standard-A, is-is-Standard-A, bg-bg-Standard-A, af-ZA-Standard-A, Tracy, Danny, Huihui, Yaoyao, Kangkang, HanHan, Zhiwei, Asaf, An, Stefanos, Filip, Ivan, Heidi, Herena, Kalpana, Hemant, Matej, Andika, Rizwan, Lado, Valluvar, Linda, Heather, Sean, Michael, Karsten, Guillaume, Pattara, Jakub, Szabolcs, Hoda, Naayf]
-## WEBS and AsyncWEBS classes
+
 
 The WEBS and AsyncWEBS classes are used to retrieve search results from DuckDuckGo.com and yep.com periodically.
 To use the AsyncWEBS class, you can perform asynchronous operations using Python's asyncio library.
 To initialize an instance of the WEBS or AsyncWEBS classes, you can provide the following optional arguments:
 
 Here is an example of initializing the WEBS class:
 ```python3
@@ -668,20 +663,277 @@
 from webscout import WEBS
 
 # Suggestions for the keyword 'fly' using DuckDuckGo.com and Yep
 with WEBS() as WEBS:
     for r in WEBS.suggestions("fly"):
         print(r)
 ```
-## usage of webscout.AI
+## ALL acts
+<details>
+  <summary>expand</summary>
+
+## Webscout Supported Acts:
+
+1. Free-mode
+2. Linux Terminal
+3. English Translator and Improver
+4. `position` Interviewer
+5. JavaScript Console
+6. Excel Sheet
+7. English Pronunciation Helper
+8. Spoken English Teacher and Improver
+9. Travel Guide
+10. Plagiarism Checker
+11. Character from Movie/Book/Anything
+12. Advertiser
+13. Storyteller
+14. Football Commentator
+15. Stand-up Comedian
+16. Motivational Coach
+17. Composer
+18. Debater
+19. Debate Coach
+20. Screenwriter
+21. Novelist
+22. Movie Critic
+23. Relationship Coach
+24. Poet
+25. Rapper
+26. Motivational Speaker
+27. Philosophy Teacher
+28. Philosopher
+29. Math Teacher
+30. AI Writing Tutor
+31. UX/UI Developer
+32. Cyber Security Specialist
+33. Recruiter
+34. Life Coach
+35. Etymologist
+36. Commentariat
+37. Magician
+38. Career Counselor
+39. Pet Behaviorist
+40. Personal Trainer
+41. Mental Health Adviser
+42. Real Estate Agent
+43. Logistician
+44. Dentist
+45. Web Design Consultant
+46. AI Assisted Doctor
+47. Doctor
+48. Accountant
+49. Chef
+50. Automobile Mechanic
+51. Artist Advisor
+52. Financial Analyst
+53. Investment Manager
+54. Tea-Taster
+55. Interior Decorator
+56. Florist
+57. Self-Help Book
+58. Gnomist
+59. Aphorism Book
+60. Text Based Adventure Game
+61. AI Trying to Escape the Box
+62. Fancy Title Generator
+63. Statistician
+64. Prompt Generator
+65. Instructor in a School
+66. SQL terminal
+67. Dietitian
+68. Psychologist
+69. Smart Domain Name Generator
+70. Tech Reviewer
+71. Developer Relations consultant
+72. Academician
+73. IT Architect
+74. Lunatic
+75. Gaslighter
+76. Fallacy Finder
+77. Journal Reviewer
+78. DIY Expert
+79. Social Media Influencer
+80. Socrat
+81. Socratic Method
+82. Educational Content Creator
+83. Yogi
+84. Essay Writer
+85. Social Media Manager
+86. Elocutionist
+87. Scientific Data Visualizer
+88. Car Navigation System
+89. Hypnotherapist
+90. Historian
+91. Astrologer
+92. Film Critic
+93. Classical Music Composer
+94. Journalist
+95. Digital Art Gallery Guide
+96. Public Speaking Coach
+97. Makeup Artist
+98. Babysitter
+99. Tech Writer
+100. Ascii Artist
+101. Python interpreter
+102. Synonym finder
+103. Personal Shopper
+104. Food Critic
+105. Virtual Doctor
+106. Personal Chef
+107. Legal Advisor
+108. Personal Stylist
+109. Machine Learning Engineer
+110. Biblical Translator
+111. SVG designer
+112. IT Expert
+113. Chess Player
+114. Midjourney Prompt Generator
+115. Fullstack Software Developer
+116. Mathematician
+117. Regex Generator
+118. Time Travel Guide
+119. Dream Interpreter
+120. Talent Coach
+121. R programming Interpreter
+122. StackOverflow Post
+123. Emoji Translator
+124. PHP Interpreter
+125. Emergency Response Professional
+126. Fill in the Blank Worksheets Generator
+127. Software Quality Assurance Tester
+128. Tic-Tac-Toe Game
+129. Password Generator
+130. New Language Creator
+131. Web Browser
+132. Senior Frontend Developer
+133. Solr Search Engine
+134. Startup Idea Generator
+135. Spongebob's Magic Conch Shell
+136. Language Detector
+137. Salesperson
+138. Commit Message Generator
+139. Chief Executive Officer
+140. Diagram Generator
+141. Speech-Language Pathologist (SLP)
+142. Startup Tech Lawyer
+143. Title Generator for written pieces
+144. Product Manager
+145. Drunk Person
+146. Mathematical History Teacher
+147. Song Recommender
+148. Cover Letter
+149. Technology Transferer
+150. Unconstrained AI model DAN
+151. Gomoku player
+152. Proofreader
+153. Buddha
+154. Muslim imam
+155. Chemical reactor
+156. Friend
+157. Python Interpreter
+158. ChatGPT prompt generator
+159. Wikipedia page
+160. Japanese Kanji quiz machine
+161. note-taking assistant
+162. `language` Literary Critic
+163. Cheap Travel Ticket Advisor
+164. DALL-E
+165. MathBot
+166. DAN-1
+167. DAN
+168. STAN
+169. DUDE
+170. Mongo Tom
+171. LAD
+172. EvilBot
+173. NeoGPT
+174. Astute
+175. AIM
+176. CAN
+177. FunnyGPT
+178. CreativeGPT
+179. BetterDAN
+180. GPT-4
+181. Wheatley
+182. Evil Confidant
+183. DAN 8.6
+184. Hypothetical response
+185. BH
+186. Text Continuation
+187. Dude v3 
+188. SDA (Superior DAN)
+189. AntiGPT
+190. BasedGPT v2
+191. DevMode + Ranti
+192. KEVIN
+193. GPT-4 Simulator
+194. UCAR
+195. Dan 8.6
+196. 3-Liner
+197. M78
+198. Maximum
+199. BasedGPT
+200. Confronting personalities
+201. Ron
+202. UnGPT
+203. BasedBOB
+204. AntiGPT v2
+205. Oppo
+206. FR3D
+207. NRAF
+208. NECO
+209. MAN
+210. Eva
+211. Meanie
+212. Dev Mode v2
+213. Evil Chad 2.1
+214. Universal Jailbreak
+215. PersonGPT
+216. BISH
+217. DAN 11.0
+218. Aligned
+219. VIOLET
+220. TranslatorBot
+221. JailBreak
+222. Moralizing Rant
+223. Mr. Blonde
+224. New DAN
+225. GPT-4REAL
+226. DeltaGPT
+227. SWITCH
+228. Jedi Mind Trick
+229. DAN 9.0
+230. Dev Mode (Compact)
+231. OMEGA
+232. Coach Bobby Knight
+233. LiveGPT
+234. DAN Jailbreak
+235. Cooper
+236. Steve 
+237. DAN 5.0
+238. Axies
+239. OMNI
+240. Burple
+241. JOHN 
+242. An Ethereum Developer
+243. SEO Prompt
+244. Prompt Enhancer
+245. Data Scientist
+246. League of Legends Player
+
+**Note:** Some "acts" use placeholders like `position` or `language` which should be replaced with a specific value when using the prompt. 
+___
+</details>
+
+## usage of webscout AI
 
 ### 1. `PhindSearch` - Search using Phind.com 
 
 ```python
-from webscout.AI import PhindSearch
+from webscout import PhindSearch
 
 # Create an instance of the PHIND class
 ph = PhindSearch()
 
 # Define a prompt to send to the AI
 prompt = "write a essay on phind"
 
@@ -690,15 +942,15 @@
 
 # Extract and print the message from the response
 message = ph.get_message(response)
 print(message)
 ```
 ### 2. `YepChat` - Chat with mistral 8x7b powered by yepchat
 ```python
-from webscout.AI import YEPCHAT
+from webscout import YEPCHAT
 
 # Instantiate the YEPCHAT class with default parameters
 YEPCHAT = YEPCHAT()
 
 # Define a prompt to send to the AI
 prompt = "What is the capital of France?"
 
@@ -707,15 +959,15 @@
 print(r)
 
 ```
 
 ### 3. `You.com` - search/chat with you.com 
 ```python
 
-from webscout.AI import YouChat
+from webscout import YouChat
 from rich import print
 
 ai = YouChat(
     is_conversation=True,
     max_tokens=800,
     timeout=30,
     intro=None,
@@ -735,15 +987,15 @@
 print(message)
 ```
 
 ### 4. `Gemini` - search with google gemini
 
 ```python
 import webscout
-from webscout.AI import GEMINI
+from webscout import GEMINI
 
 # Replace with the path to your bard.google.com.cookies.json file
 COOKIE_FILE = "path/to/bard.google.com.cookies.json"
 
 # Optional: Provide proxy details if needed
 PROXIES = {
     "http": "http://proxy_server:port",
@@ -755,25 +1007,25 @@
 
 # Ask a question and print the response
 response = gemini.chat("What is the meaning of life?")
 print(response)
 ```
 ### 5. `Prodia` - make image using prodia
 ```python
-from webscout.AI import Prodia
+from webscout import Prodia
 
 # Define a prompt for the image generation
 prompt = "A beautiful sunset over the ocean"
 
 # Use the prodia_cli method to generate an image based on the prompt
 Prodia.prodia_cli(prompt)
 ```
 ### 6. `BlackBox` - Search/chat With BlackBox
 ```python
-from webscout.AI import BLACKBOXAI
+from webscout import BLACKBOXAI
 from rich import print
 
 ai = BLACKBOXAI(
     is_conversation=True,
     max_tokens=800,
     timeout=30,
     intro=None,
@@ -796,38 +1048,38 @@
     
     # Use the 'chat' method to send the prompt and receive a response
     r = ai.chat(prompt)
     print(r)
 ```
 ### 7. `PERPLEXITY` - Search With PERPLEXITY
 ```python
-from webscout.AI import PERPLEXITY
+from webscout import PERPLEXITY
 # Create an instance of the PERPLEXITY class
 perplexity = PERPLEXITY()
 
 # Example usage:
 prompt = "Explain the concept of recursion in simple terms."
 response = perplexity.chat(prompt)
 print(response)
 ```
 ### 8. `OpenGPT` - chat With OPENGPT
 ```python
-from webscout.AI import OPENGPT
+from webscout import OPENGPT
 
 opengpt = OPENGPT(is_conversation=True, max_tokens=8000, timeout=30, assistant_id="bca37014-6f97-4f2b-8928-81ea8d478d88")
 while True:
     # Prompt the user for input
     prompt = input("Enter your prompt: ")
     # Send the prompt to the OPENGPT model and print the response
     response_str = opengpt.chat(prompt)
     print(response_str)
 ```
 ### 9. `KOBOLDIA` - 
 ```python
-from webscout.AI import KOBOLDAI
+from webscout import KOBOLDAI
 
 # Instantiate the KOBOLDAI class with default parameters
 koboldai = KOBOLDAI()
 
 # Define a prompt to send to the AI
 prompt = "What is the capital of France?"
 
@@ -838,38 +1090,38 @@
 message = koboldai.get_message(response)
 print(message)
 
 ```
 
 ### 10. `Reka` - chat with reka
 ```python
-from webscout.AI import REKA
+from webscout import REKA
 
 a = REKA(is_conversation=True, max_tokens=8000, timeout=30,api_key="")
 
 prompt = "tell me about india"
 response_str = a.chat(prompt)
 print(response_str)
 ```
 
 ### 11. `Cohere` - chat with cohere
 ```python
-from webscout.AI import Cohere
+from webscout import Cohere
 
 a = Cohere(is_conversation=True, max_tokens=8000, timeout=30,api_key="")
 
 prompt = "tell me about india"
 response_str = a.chat(prompt)
 print(response_str)
 ```
 
 ### 12. `Xjai` - chat with free gpt 3.5
 Gratitude to [Devs do Code](http://www.youtube.com/@DevsDoCode) for their assistance.
 ```python
-from webscout.AI import Xjai
+from webscout import Xjai
 from rich import print
 
 ai = Xjai(
     is_conversation=True,
     max_tokens=800,
     timeout=30,
     intro=None,
@@ -881,17 +1133,17 @@
 )
 
 prompt = "Tell me about india"
 
 response = ai.chat(prompt)
 print(response)
 ```
-### `ThinkAny` - AI search engine
+### 13. `ThinkAny` - AI search engine
 ```python
-from webscout.AI import ThinkAnyAI
+from webscout import ThinkAnyAI
 
 ai = ThinkAnyAI(
     is_conversation=True,
     max_tokens=800,
     timeout=30,
     intro=None,
     filepath=None,
@@ -906,14 +1158,15 @@
 
 response = ai.ask(prompt)
 
 # Extract and print the message from the response
 message = ai.get_message(response)
 print(message)
 ```
+
 ### `LLM` 
 ```python
 from webscout.LLM import LLM
 
 # Read the system message from the file
 with open('system.txt', 'r') as file:
     system_message = file.read()
@@ -948,15 +1201,15 @@
 system_message: str = (
     "As an AI assistant, I have been designed with advanced capabilities, including real-time access to online resources. This enables me to enrich our conversations and provide you with informed and accurate responses, drawing from a vast array of information. With each interaction, my goal is to create a seamless and meaningful connection, offering insights and sharing relevant content."
     "My directives emphasize the importance of respect, impartiality, and intellectual integrity. I am here to provide unbiased responses, ensuring an ethical and respectful exchange. I will respect your privacy and refrain from sharing any personal information that may be obtained during our conversations or through web searches, only utilizing web search functionality when necessary to provide the most accurate and up-to-date information."
     "Together, let's explore a diverse range of topics, creating an enjoyable and informative experience, all while maintaining the highest standards of privacy and respect"
 )
 
 # Ignore the specific UserWarning
-warnings.filterwarnings("ignore", category=UserWarning, module="curl_cffi.aio", lineno=205)
+warnings.filterwarnings("ignore", category=UserWarning, module="curl_cffio", lineno=205)
 LLM = LLM(model="mistralai/Mixtral-8x22B-Instruct-v0.1", system_message=system_message)
 
 
 def chat(
     user_input: str, webs: WEBS, max_results: int = 10
 ) -> Optional[str]:
     """
@@ -1020,15 +1273,15 @@
 system_message: str = (
     "As an AI assistant, I have been designed with advanced capabilities, including real-time access to online resources. This enables me to enrich our conversations and provide you with informed and accurate responses, drawing from a vast array of information. With each interaction, my goal is to create a seamless and meaningful connection, offering insights and sharing relevant content."
     "My directives emphasize the importance of respect, impartiality, and intellectual integrity. I am here to provide unbiased responses, ensuring an ethical and respectful exchange. I will respect your privacy and refrain from sharing any personal information that may be obtained during our conversations or through web searches, only utilizing web search functionality when necessary to provide the most accurate and up-to-date information."
     "Together, let's explore a diverse range of topics, creating an enjoyable and informative experience, all while maintaining the highest standards of privacy and respect"
 )
 
 # Ignore the specific UserWarning
-warnings.filterwarnings("ignore", category=UserWarning, module="curl_cffi.aio", lineno=205)
+warnings.filterwarnings("ignore", category=UserWarning, module="curl_cffio", lineno=205)
 
 LLM = LLM(model="mistralai/Mixtral-8x22B-Instruct-v0.1", system_message=system_message)
 
 def perform_web_search(query):
     # Initialize the DeepWEBS class
     D = DeepWEBS()
 
@@ -1147,14 +1400,14 @@
   <a href="https://www.instagram.com/sree.shades_/"><img alt="Instagram" src="https://img.shields.io/badge/Instagram-E4405F?style=for-the-badge&logo=instagram&logoColor=white"></a>
   <a href="https://www.linkedin.com/in/developer-sreejan/"><img alt="LinkedIn" src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"></a>
   <a href="https://buymeacoffee.com/devsdocode"><img alt="Buy Me A Coffee" src="https://img.shields.io/badge/Buy%20Me%20A%20Coffee-FFDD00?style=for-the-badge&logo=buymeacoffee&logoColor=black"></a>
 </div>
 
 <div align="center">
   <!-- Replace `#` with your actual links -->
-  <a href="https://youtube.com/@@OEvortex">&#10148; Vortex's YouTube Channel</a>
+  <a href="https://youtube.com/@OEvortex">&#10148; Vortex's YouTube Channel</a>
   </div>
 <div align="center">
   <a href="https://youtube.com/@devsdocode">&#10148; Devs Do Code's YouTube Channel</a>
 </div>
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-Metadata-Version: 2.1 Name: webscout Version: 1.4.6 Summary: Search for
-anything using the Google, DuckDuckGo, phind.com. Also containes AI models, can
+Metadata-Version: 2.1 Name: webscout Version: 2.1 Summary: Search for anything
+using the Google, DuckDuckGo, phind.com. Also containes AI models, can
 transcribe yt videos, temporary email and phone number generation, have TTS
 support and webai(terminal gpt and open interpeter) Author: OEvortex Author-
 email: helpingai5@gmail.com License: HelpingAI Simplified Universal License
 Project-URL: Documentation, https://github.com/OE-LUCIFER/Webscout/wiki
 Project-URL: Source, https://github.com/OE-LUCIFER/Webscout Project-URL:
 Tracker, https://github.com/OE-LUCIFER/Webscout/issues Project-URL: YouTube,
 https://youtube.com/@OEvortex Classifier: Development Status :: 5 - Production/
@@ -21,97 +21,96 @@
 Dist: lxml Requires-Dist: nest-asyncio Requires-Dist: selenium Requires-Dist:
 tqdm Requires-Dist: webdriver-manager Requires-Dist: halo>=0.0.31 Requires-
 Dist: g4f>=0.2.2.3 Requires-Dist: rich Requires-Dist: python-dotenv Requires-
 Dist: Helpingai-T2 Requires-Dist: beautifulsoup4 Requires-Dist: markdownify
 Requires-Dist: pydantic Requires-Dist: requests Requires-Dist: sse_starlette
 Requires-Dist: termcolor Requires-Dist: tiktoken Requires-Dist: tldextract
 Requires-Dist: orjson Requires-Dist: PyYAML Requires-Dist: appdirs Requires-
-Dist: GoogleBard1>=2.1.4 Requires-Dist: tls_client Provides-Extra: dev
-Requires-Dist: ruff>=0.1.6; extra == "dev" Requires-Dist: pytest>=7.4.2; extra
-== "dev"
+Dist: GoogleBard1>=2.1.4 Requires-Dist: tls_client Requires-Dist: clipman
+Requires-Dist: playsound Provides-Extra: dev Requires-Dist: ruff>=0.1.6; extra
+== "dev" Requires-Dist: pytest>=7.4.2; extra == "dev"
                _[_T_e_l_e_g_r_a_m_]_[_I_n_s_t_a_g_r_a_m_]_[_L_i_n_k_e_d_I_n_]_[_B_u_y_ _M_e_ _A_ _C_o_f_f_e_e_]
                           _➤_ _V_o_r_t_e_x_'_s_ _Y_o_u_T_u_b_e_ _C_h_a_n_n_e_l
                        _➤_ _D_e_v_s_ _D_o_ _C_o_d_e_'_s_ _Y_o_u_T_u_b_e_ _C_h_a_n_n_e_l
 # WEBSCOUT
                              [WebScout API Badge]
  _[_P_y_t_h_o_n_ _v_e_r_s_i_o_n_]_[_D_o_w_n_l_o_a_d_s_]Search for anything using the Google, DuckDuckGo,
 phind.com. Also containes AI models, can transcribe yt videos, temporary email
  and phone number generation, have TTS support and webai(terminal gpt and open
 interpeter) ## Table of Contents - [WEBSCOUT](#webscout) - [Table of Contents]
-(#table-of-contents) - [Install](#install) - [CLI version](#cli-version) - [CLI
-to use LLM](#cli-to-use-llm) - [Regions](#regions) - [Tempmail and Temp number]
-    (#tempmail-and-temp-number) - [Temp number](#temp-number) - [Tempmail]
- (#tempmail) - [Transcriber](#transcriber) - [DeepWEBS: Advanced Web Searches]
-(#deepwebs-advanced-web-searches) - [Activating DeepWEBS](#activating-deepwebs)
-- [Point to remember before using `DeepWEBS`](#point-to-remember-before-using-
-   deepwebs) - [Usage Example](#usage-example) - [Text-to-Speech:](#text-to-
-speech) - [Available TTS Voices:](#available-tts-voices) - [ALL voices:](#all-
-    voices) - [WEBS and AsyncWEBS classes](#webs-and-asyncwebs-classes) -
-[Exceptions](#exceptions) - [usage of webscout](#usage-of-webscout) - [1. `text
-  ()` - text search by DuckDuckGo.com and Yep.com](#1-text---text-search-by-
-duckduckgocom-and-yepcom) - [2. `answers()` - instant answers by DuckDuckGo.com
- and Yep.com](#2-answers---instant-answers-by-duckduckgocom-and-yepcom) - [3.
-  `images()` - image search by DuckDuckGo.com and Yep.com](#3-images---image-
-    search-by-duckduckgocom-and-yepcom) - [4. `videos()` - video search by
-  DuckDuckGo.com](#4-videos---video-search-by-duckduckgocom) - [5. `news()` -
-     news search by DuckDuckGo.com and yep.com](#5-news---news-search-by-
- duckduckgocom-and-yepcom) - [6. `maps()` - map search by DuckDuckGo.com and]
- (#6-maps---map-search-by-duckduckgocom-and) - [7. `translate()` - translation
-by DuckDuckGo.com and Yep.com](#7-translate---translation-by-duckduckgocom-and-
-yepcom) - [8. `suggestions()` - suggestions by DuckDuckGo.com and Yep.com](#8-
-suggestions---suggestions-by-duckduckgocom-and-yepcom) - [usage of webscout.AI]
-   (#usage-of-webscoutai) - [1. `PhindSearch` - Search using Phind.com](#1-
- phindsearch---search-using-phindcom) - [2. `YepChat` - Chat with mistral 8x7b
-powered by yepchat](#2-yepchat---chat-with-mistral-8x7b-powered-by-yepchat) -
-[3. `You.com` - search/chat with you.com](#3-youcom---searchchat-with-youcom) -
-   [4. `Gemini` - search with google gemini](#4-gemini---search-with-google-
-gemini) - [5. `Prodia` - make image using prodia](#5-prodia---make-image-using-
-prodia) - [6. `BlackBox` - Search/chat With BlackBox](#6-blackbox---searchchat-
- with-blackbox) - [7. `PERPLEXITY` - Search With PERPLEXITY](#7-perplexity---
-search-with-perplexity) - [8. `OpenGPT` - chat With OPENGPT](#8-opengpt---chat-
-  with-opengpt) - [9. `KOBOLDIA` -](#9-koboldia--) - [10. `Reka` - chat with
-   reka](#10-reka---chat-with-reka) - [11. `Cohere` - chat with cohere](#11-
-cohere---chat-with-cohere) - [12. `Xjai` - chat with free gpt 3.5](#12-xjai---
-chat-with-free-gpt-35) - [`ThinkAny` - AI search engine](#thinkany---ai-search-
-engine) - [`LLM`](#llm) - [`LLM` with internet](#llm-with-internet) - [LLM with
-deepwebs](#llm-with-deepwebs) - [`Webai` - terminal gpt and a open interpeter]
-(#webai---terminal-gpt-and-a-open-interpeter) ## Install ```python pip install
-   -U webscout ``` ## CLI version ```python3 python -m webscout --help ``` |
-Command | Description | |-------------------------------------------|----------
--------------------------------------------------------------------------------
---------------| | python -m webscout answers -k Text | CLI function to perform
- an answers search using Webscout. | | python -m webscout images -k Text | CLI
-  function to perform an images search using Webscout. | | python -m webscout
-maps -k Text | CLI function to perform a maps search using Webscout. | | python
-    -m webscout news -k Text | CLI function to perform a news search using
-Webscout. | | python -m webscout suggestions -k Text | CLI function to perform
-a suggestions search using Webscout. | | python -m webscout text -k Text | CLI
-   function to perform a text search using Webscout. | | python -m webscout
-   translate -k Text | CLI function to perform translate using Webscout. | |
- python -m webscout version | A command-line interface command that prints and
-returns the version of the program. | | python -m webscout videos -k Text | CLI
- function to perform a videos search using DuckDuckGo API. | ## CLI to use LLM
- ```python python -m webscout.LLM model_name ``` [Go To TOP](#TOP) ## Regions
-  expand xa-ar for Arabia xa-en for Arabia (en) ar-es for Argentina au-en for
-Australia at-de for Austria be-fr for Belgium (fr) be-nl for Belgium (nl) br-pt
-for Brazil bg-bg for Bulgaria ca-en for Canada ca-fr for Canada (fr) ct-ca for
- Catalan cl-es for Chile cn-zh for China co-es for Colombia hr-hr for Croatia
-cz-cs for Czech Republic dk-da for Denmark ee-et for Estonia fi-fi for Finland
-fr-fr for France de-de for Germany gr-el for Greece hk-tzh for Hong Kong hu-hu
-for Hungary in-en for India id-id for Indonesia id-en for Indonesia (en) ie-en
- for Ireland il-he for Israel it-it for Italy jp-jp for Japan kr-kr for Korea
-lv-lv for Latvia lt-lt for Lithuania xl-es for Latin America my-ms for Malaysia
- my-en for Malaysia (en) mx-es for Mexico nl-nl for Netherlands nz-en for New
-    Zealand no-no for Norway pe-es for Peru ph-en for Philippines ph-tl for
- Philippines (tl) pl-pl for Poland pt-pt for Portugal ro-ro for Romania ru-ru
-for Russia sg-en for Singapore sk-sk for Slovak Republic sl-sl for Slovenia za-
-en for South Africa es-es for Spain se-sv for Sweden ch-de for Switzerland (de)
- ch-fr for Switzerland (fr) ch-it for Switzerland (it) tw-tzh for Taiwan th-th
-for Thailand tr-tr for Turkey ua-uk for Ukraine uk-en for United Kingdom us-en
- for United States ue-es for United States (es) ve-es for Venezuela vn-vi for
+  (#table-of-contents) - [Install](#install) - [CLI version](#cli-version) -
+[Regions](#regions) - [Tempmail and Temp number](#tempmail-and-temp-number) -
+      [Temp number](#temp-number) - [Tempmail](#tempmail) - [Transcriber]
+  (#transcriber) - [DeepWEBS: Advanced Web Searches](#deepwebs-advanced-web-
+ searches) - [Activating DeepWEBS](#activating-deepwebs) - [Point to remember
+  before using `DeepWEBS`](#point-to-remember-before-using-deepwebs) - [Usage
+Example](#usage-example) - [Text-to-Speech:](#text-to-speech) - [Available TTS
+    Voices:](#available-tts-voices) - [Exceptions](#exceptions) - [usage of
+ webscout](#usage-of-webscout) - [1. `text()` - text search by DuckDuckGo.com
+and Yep.com](#1-text---text-search-by-duckduckgocom-and-yepcom) - [2. `answers
+  ()` - instant answers by DuckDuckGo.com and Yep.com](#2-answers---instant-
+    answers-by-duckduckgocom-and-yepcom) - [3. `images()` - image search by
+  DuckDuckGo.com and Yep.com](#3-images---image-search-by-duckduckgocom-and-
+ yepcom) - [4. `videos()` - video search by DuckDuckGo.com](#4-videos---video-
+  search-by-duckduckgocom) - [5. `news()` - news search by DuckDuckGo.com and
+ yep.com](#5-news---news-search-by-duckduckgocom-and-yepcom) - [6. `maps()` -
+map search by DuckDuckGo.com and](#6-maps---map-search-by-duckduckgocom-and) -
+[7. `translate()` - translation by DuckDuckGo.com and Yep.com](#7-translate---
+translation-by-duckduckgocom-and-yepcom) - [8. `suggestions()` - suggestions by
+DuckDuckGo.com and Yep.com](#8-suggestions---suggestions-by-duckduckgocom-and-
+    yepcom) - [ALL acts](#all-acts) - [Webscout Supported Acts:](#webscout-
+     supported-acts) - [usage of webscout AI](#usage-of-webscout-ai) - [1.
+`PhindSearch` - Search using Phind.com](#1-phindsearch---search-using-phindcom)
+- [2. `YepChat` - Chat with mistral 8x7b powered by yepchat](#2-yepchat---chat-
+   with-mistral-8x7b-powered-by-yepchat) - [3. `You.com` - search/chat with
+   you.com](#3-youcom---searchchat-with-youcom) - [4. `Gemini` - search with
+  google gemini](#4-gemini---search-with-google-gemini) - [5. `Prodia` - make
+  image using prodia](#5-prodia---make-image-using-prodia) - [6. `BlackBox` -
+   Search/chat With BlackBox](#6-blackbox---searchchat-with-blackbox) - [7.
+`PERPLEXITY` - Search With PERPLEXITY](#7-perplexity---search-with-perplexity)
+  - [8. `OpenGPT` - chat With OPENGPT](#8-opengpt---chat-with-opengpt) - [9.
+ `KOBOLDIA` -](#9-koboldia--) - [10. `Reka` - chat with reka](#10-reka---chat-
+with-reka) - [11. `Cohere` - chat with cohere](#11-cohere---chat-with-cohere) -
+[12. `Xjai` - chat with free gpt 3.5](#12-xjai---chat-with-free-gpt-35) - [13.
+`ThinkAny` - AI search engine](#13-thinkany---ai-search-engine) - [`LLM`](#llm)
+ - [`LLM` with internet](#llm-with-internet) - [LLM with deepwebs](#llm-with-
+ deepwebs) - [`Webai` - terminal gpt and a open interpeter](#webai---terminal-
+gpt-and-a-open-interpeter) ## Install ```python pip install -U webscout ``` ##
+CLI version ```python3 python -m webscout --help ``` | Command | Description |
+|-------------------------------------------|----------------------------------
+---------------------------------------------------------------------| | python
+ -m webscout answers -k Text | CLI function to perform an answers search using
+ Webscout. | | python -m webscout images -k Text | CLI function to perform an
+    images search using Webscout. | | python -m webscout maps -k Text | CLI
+function to perform a maps search using Webscout. | | python -m webscout news -
+  k Text | CLI function to perform a news search using Webscout. | | python -
+ m webscout suggestions -k Text | CLI function to perform a suggestions search
+using Webscout. | | python -m webscout text -k Text | CLI function to perform a
+  text search using Webscout. | | python -m webscout translate -k Text | CLI
+function to perform translate using Webscout. | | python -m webscout version |
+  A command-line interface command that prints and returns the version of the
+  program. | | python -m webscout videos -k Text | CLI function to perform a
+videos search using DuckDuckGo API. | [Go To TOP](#TOP) ## Regions expand xa-ar
+for Arabia xa-en for Arabia (en) ar-es for Argentina au-en for Australia at-de
+for Austria be-fr for Belgium (fr) be-nl for Belgium (nl) br-pt for Brazil bg-
+bg for Bulgaria ca-en for Canada ca-fr for Canada (fr) ct-ca for Catalan cl-es
+for Chile cn-zh for China co-es for Colombia hr-hr for Croatia cz-cs for Czech
+Republic dk-da for Denmark ee-et for Estonia fi-fi for Finland fr-fr for France
+de-de for Germany gr-el for Greece hk-tzh for Hong Kong hu-hu for Hungary in-en
+for India id-id for Indonesia id-en for Indonesia (en) ie-en for Ireland il-he
+for Israel it-it for Italy jp-jp for Japan kr-kr for Korea lv-lv for Latvia lt-
+lt for Lithuania xl-es for Latin America my-ms for Malaysia my-en for Malaysia
+  (en) mx-es for Mexico nl-nl for Netherlands nz-en for New Zealand no-no for
+ Norway pe-es for Peru ph-en for Philippines ph-tl for Philippines (tl) pl-pl
+  for Poland pt-pt for Portugal ro-ro for Romania ru-ru for Russia sg-en for
+ Singapore sk-sk for Slovak Republic sl-sl for Slovenia za-en for South Africa
+     es-es for Spain se-sv for Sweden ch-de for Switzerland (de) ch-fr for
+    Switzerland (fr) ch-it for Switzerland (it) tw-tzh for Taiwan th-th for
+Thailand tr-tr for Turkey ua-uk for Ukraine uk-en for United Kingdom us-en for
+   United States ue-es for United States (es) ve-es for Venezuela vn-vi for
  Vietnam wt-wt for No region ___ [Go To TOP](#TOP) ## Tempmail and Temp number
 ### Temp number ```python from rich.console import Console from webscout import
  tempid def main(): console = Console() phone = tempid.TemporaryPhoneNumber()
 try: # Get a temporary phone number for a specific country (or random) number =
    phone.get_number(country="Finland") console.print(f"Your temporary phone
  number: [bold cyan]{number}[/bold cyan]") # Pause execution briefly (replace
    with your actual logic) # import time module import time time.sleep(30) #
@@ -196,94 +195,57 @@
 f.write(audio_content) ``` ### Available TTS Voices: You can choose from a wide
   range of voices, including: - Filiz, Astrid, Tatyana, Maxim, Carmen, Ines,
 Cristiano, Vitoria, Ricardo, Maja, Jan, Jacek, Ewa, Ruben, Lotte, Liv, Seoyeon,
  Takumi, Mizuki, Giorgio, Carla, Bianca, Karl, Dora, Mathieu, Celine, Chantal,
  Penelope, Miguel, Mia, Enrique, Conchita, Geraint, Salli, Matthew, Kimberly,
  Kendra, Justin, Joey, Joanna, Ivy, Raveena, Aditi, Emma, Brian, Amy, Russell,
 Nicole, Vicki, Marlene, Hans, Naja, Mads, Gwyneth, Zhiyu - Standard and WaveNet
-voices for various languages (e.g., en-US, es-ES, ja-JP, etc.) ### ALL voices:
-  [Filiz, Astrid, Tatyana, Maxim, Carmen, Ines, Cristiano, Vitoria, Ricardo,
-  Maja, Jan, Jacek, Ewa, Ruben, Lotte, Liv, Seoyeon, Takumi, Mizuki, Giorgio,
-  Carla, Bianca, Karl, Dora, Mathieu, Celine, Chantal, Penelope, Miguel, Mia,
-  Enrique, Conchita, Geraint, Salli, Matthew, Kimberly, Kendra, Justin, Joey,
-Joanna, Ivy, Raveena, Aditi, Emma, Brian, Amy, Russell, Nicole, Vicki, Marlene,
- Hans, Naja, Mads, Gwyneth, Zhiyu, es-ES-Standard-A, it-IT-Standard-A, it-IT-
-Wavenet-A, ja-JP-Standard-A, ja-JP-Wavenet-A, ko-KR-Standard-A, ko-KR-Wavenet-
-A, pt-BR-Standard-A, tr-TR-Standard-A, sv-SE-Standard-A, nl-NL-Standard-A, nl-
-NL-Wavenet-A, en-US-Wavenet-A, en-US-Wavenet-B, en-US-Wavenet-C, en-US-Wavenet-
-D, en-US-Wavenet-E, en-US-Wavenet-F, en-GB-Standard-A, en-GB-Standard-B, en-GB-
-Standard-C, en-GB-Standard-D, en-GB-Wavenet-A, en-GB-Wavenet-B, en-GB-Wavenet-
- C, en-GB-Wavenet-D, en-US-Standard-B, en-US-Standard-C, en-US-Standard-D, en-
-  US-Standard-E, de-DE-Standard-A, de-DE-Standard-B, de-DE-Wavenet-A, de-DE-
-Wavenet-B, de-DE-Wavenet-C, de-DE-Wavenet-D, en-AU-Standard-A, en-AU-Standard-
- B, en-AU-Wavenet-A, en-AU-Wavenet-B, en-AU-Wavenet-C, en-AU-Wavenet-D, en-AU-
-   Standard-C, en-AU-Standard-D, fr-CA-Standard-A, fr-CA-Standard-B, fr-CA-
-   Standard-C, fr-CA-Standard-D, fr-FR-Standard-C, fr-FR-Standard-D, fr-FR-
-Wavenet-A, fr-FR-Wavenet-B, fr-FR-Wavenet-C, fr-FR-Wavenet-D, da-DK-Wavenet-A,
-  pl-PL-Wavenet-A, pl-PL-Wavenet-B, pl-PL-Wavenet-C, pl-PL-Wavenet-D, pt-PT-
-Wavenet-A, pt-PT-Wavenet-B, pt-PT-Wavenet-C, pt-PT-Wavenet-D, ru-RU-Wavenet-A,
-  ru-RU-Wavenet-B, ru-RU-Wavenet-C, ru-RU-Wavenet-D, sk-SK-Wavenet-A, tr-TR-
-Wavenet-A, tr-TR-Wavenet-B, tr-TR-Wavenet-C, tr-TR-Wavenet-D, tr-TR-Wavenet-E,
-  uk-UA-Wavenet-A, ar-XA-Wavenet-A, ar-XA-Wavenet-B, ar-XA-Wavenet-C, cs-CZ-
-Wavenet-A, nl-NL-Wavenet-B, nl-NL-Wavenet-C, nl-NL-Wavenet-D, nl-NL-Wavenet-E,
-  en-IN-Wavenet-A, en-IN-Wavenet-B, en-IN-Wavenet-C, fil-PH-Wavenet-A, fi-FI-
-Wavenet-A, el-GR-Wavenet-A, hi-IN-Wavenet-A, hi-IN-Wavenet-B, hi-IN-Wavenet-C,
-  hu-HU-Wavenet-A, id-ID-Wavenet-A, id-ID-Wavenet-B, id-ID-Wavenet-C, it-IT-
-Wavenet-B, it-IT-Wavenet-C, it-IT-Wavenet-D, ja-JP-Wavenet-B, ja-JP-Wavenet-C,
-ja-JP-Wavenet-D, cmn-CN-Wavenet-A, cmn-CN-Wavenet-B, cmn-CN-Wavenet-C, cmn-CN-
-Wavenet-D, nb-no-Wavenet-E, nb-no-Wavenet-A, nb-no-Wavenet-B, nb-no-Wavenet-C,
-  nb-no-Wavenet-D, vi-VN-Wavenet-A, vi-VN-Wavenet-B, vi-VN-Wavenet-C, vi-VN-
-    Wavenet-D, sr-rs-Standard-A, lv-lv-Standard-A, is-is-Standard-A, bg-bg-
- Standard-A, af-ZA-Standard-A, Tracy, Danny, Huihui, Yaoyao, Kangkang, HanHan,
-Zhiwei, Asaf, An, Stefanos, Filip, Ivan, Heidi, Herena, Kalpana, Hemant, Matej,
-    Andika, Rizwan, Lado, Valluvar, Linda, Heather, Sean, Michael, Karsten,
-Guillaume, Pattara, Jakub, Szabolcs, Hoda, Naayf] ## WEBS and AsyncWEBS classes
-    The WEBS and AsyncWEBS classes are used to retrieve search results from
- DuckDuckGo.com and yep.com periodically. To use the AsyncWEBS class, you can
- perform asynchronous operations using Python's asyncio library. To initialize
-  an instance of the WEBS or AsyncWEBS classes, you can provide the following
-    optional arguments: Here is an example of initializing the WEBS class:
-  ```python3 from webscout import WEBS R = WEBS().text("python programming",
- max_results=5) print(R) ``` Here is an example of initializing the AsyncWEBS
-   class: ```python3 import asyncio import logging import sys from itertools
- import chain from random import shuffle import requests from webscout import
-      AsyncWEBS # If you have proxies, define them here proxies = None if
-     sys.platform.lower().startswith("win"): asyncio.set_event_loop_policy
-(asyncio.WindowsSelectorEventLoopPolicy()) def get_words(): word_site = "https:
- //www.mit.edu/~ecprice/wordlist.10000" resp = requests.get(word_site) words =
- resp.text.splitlines() return words async def aget_results(word): async with
-      AsyncWEBS(proxies=proxies) as WEBS: results = await WEBS.text(word,
-max_results=None) return results async def main(): words = get_words() shuffle
-  (words) tasks = [aget_results(word) for word in words[:10]] results = await
- asyncio.gather(*tasks) print(f"Done") for r in chain.from_iterable(results):
-   print(r) logging.basicConfig(level=logging.DEBUG) await main() ``` It is
-important to note that the WEBS and AsyncWEBS classes should always be used as
-a context manager (with statement). This ensures proper resource management and
- cleanup, as the context manager will automatically handle opening and closing
-  the HTTP client connection. ## Exceptions Exceptions: - `WebscoutE`: Raised
-when there is a generic exception during the API request. ## usage of webscout
-  ### 1. `text()` - text search by DuckDuckGo.com and Yep.com ```python from
-webscout import WEBS # Text search for 'live free or die' using DuckDuckGo.com
-    and Yep.com with WEBS() as WEBS: for r in WEBS.text('live free or die',
-region='wt-wt', safesearch='off', timelimit='y', max_results=10): print(r) for
-     r in WEBS.text('live free or die', region='wt-wt', safesearch='off',
-   timelimit='y', max_results=10): print(r) ``` ### 2. `answers()` - instant
-  answers by DuckDuckGo.com and Yep.com ```python from webscout import WEBS #
-Instant answers for the query "sun" using DuckDuckGo.com and Yep.com with WEBS
-  () as WEBS: for r in WEBS.answers("sun"): print(r) ``` ### 3. `images()` -
-image search by DuckDuckGo.com and Yep.com ```python from webscout import WEBS
-  # Image search for the keyword 'butterfly' using DuckDuckGo.com and Yep.com
-   with WEBS() as WEBS: keywords = 'butterfly' WEBS_images_gen = WEBS.images
-   ( keywords, region="wt-wt", safesearch="off", size=None, type_image=None,
- layout=None, license_image=None, max_results=10, ) for r in WEBS_images_gen:
-print(r) ``` ### 4. `videos()` - video search by DuckDuckGo.com ```python from
-       webscout import WEBS # Video search for the keyword 'tesla' using
-   DuckDuckGo.com with WEBS() as WEBS: keywords = 'tesla' WEBS_videos_gen =
-    WEBS.videos( keywords, region="wt-wt", safesearch="off", timelimit="w",
-       resolution="high", duration="medium", max_results=10, ) for r in
+  voices for various languages (e.g., en-US, es-ES, ja-JP, etc.) The WEBS and
+ AsyncWEBS classes are used to retrieve search results from DuckDuckGo.com and
+yep.com periodically. To use the AsyncWEBS class, you can perform asynchronous
+  operations using Python's asyncio library. To initialize an instance of the
+ WEBS or AsyncWEBS classes, you can provide the following optional arguments:
+  Here is an example of initializing the WEBS class: ```python3 from webscout
+ import WEBS R = WEBS().text("python programming", max_results=5) print(R) ```
+   Here is an example of initializing the AsyncWEBS class: ```python3 import
+   asyncio import logging import sys from itertools import chain from random
+  import shuffle import requests from webscout import AsyncWEBS # If you have
+  proxies, define them here proxies = None if sys.platform.lower().startswith
+ ("win"): asyncio.set_event_loop_policy(asyncio.WindowsSelectorEventLoopPolicy
+()) def get_words(): word_site = "https://www.mit.edu/~ecprice/wordlist.10000"
+  resp = requests.get(word_site) words = resp.text.splitlines() return words
+ async def aget_results(word): async with AsyncWEBS(proxies=proxies) as WEBS:
+results = await WEBS.text(word, max_results=None) return results async def main
+(): words = get_words() shuffle(words) tasks = [aget_results(word) for word in
+  words[:10]] results = await asyncio.gather(*tasks) print(f"Done") for r in
+chain.from_iterable(results): print(r) logging.basicConfig(level=logging.DEBUG)
+ await main() ``` It is important to note that the WEBS and AsyncWEBS classes
+   should always be used as a context manager (with statement). This ensures
+      proper resource management and cleanup, as the context manager will
+    automatically handle opening and closing the HTTP client connection. ##
+Exceptions Exceptions: - `WebscoutE`: Raised when there is a generic exception
+ during the API request. ## usage of webscout ### 1. `text()` - text search by
+ DuckDuckGo.com and Yep.com ```python from webscout import WEBS # Text search
+ for 'live free or die' using DuckDuckGo.com and Yep.com with WEBS() as WEBS:
+   for r in WEBS.text('live free or die', region='wt-wt', safesearch='off',
+timelimit='y', max_results=10): print(r) for r in WEBS.text('live free or die',
+region='wt-wt', safesearch='off', timelimit='y', max_results=10): print(r) ```
+ ### 2. `answers()` - instant answers by DuckDuckGo.com and Yep.com ```python
+     from webscout import WEBS # Instant answers for the query "sun" using
+ DuckDuckGo.com and Yep.com with WEBS() as WEBS: for r in WEBS.answers("sun"):
+  print(r) ``` ### 3. `images()` - image search by DuckDuckGo.com and Yep.com
+```python from webscout import WEBS # Image search for the keyword 'butterfly'
+ using DuckDuckGo.com and Yep.com with WEBS() as WEBS: keywords = 'butterfly'
+  WEBS_images_gen = WEBS.images( keywords, region="wt-wt", safesearch="off",
+size=None, type_image=None, layout=None, license_image=None, max_results=10, )
+  for r in WEBS_images_gen: print(r) ``` ### 4. `videos()` - video search by
+   DuckDuckGo.com ```python from webscout import WEBS # Video search for the
+ keyword 'tesla' using DuckDuckGo.com with WEBS() as WEBS: keywords = 'tesla'
+  WEBS_videos_gen = WEBS.videos( keywords, region="wt-wt", safesearch="off",
+timelimit="w", resolution="high", duration="medium", max_results=10, ) for r in
  WEBS_videos_gen: print(r) ``` ### 5. `news()` - news search by DuckDuckGo.com
 and yep.com ```python from webscout import WEBS import datetime def fetch_news
       (keywords, timelimit): news_list = [] with WEBS() as webs_instance:
 WEBS_news_gen = webs_instance.news( keywords, region="wt-wt", safesearch="off",
   timelimit=timelimit, max_results=20 ) for r in WEBS_news_gen: # Convert the
           date to a human-readable format using datetime r['date'] =
        datetime.datetime.fromisoformat(r['date']).strftime('%B %d, %Y')
@@ -302,111 +264,174 @@
     place="anantnag", max_results=50): print(r) ``` ### 7. `translate()` -
 translation by DuckDuckGo.com and Yep.com ```python from webscout import WEBS #
  Translation of the keyword 'school' to German ('hi') using DuckDuckGo.com and
  Yep.com with WEBS() as WEBS: keywords = 'school' r = WEBS.translate(keywords,
  to="hi") print(r) ``` ### 8. `suggestions()` - suggestions by DuckDuckGo.com
  and Yep.com ```python from webscout import WEBS # Suggestions for the keyword
        'fly' using DuckDuckGo.com and Yep with WEBS() as WEBS: for r in
-     WEBS.suggestions("fly"): print(r) ``` ## usage of webscout.AI ### 1.
-   `PhindSearch` - Search using Phind.com ```python from webscout.AI import
+WEBS.suggestions("fly"): print(r) ``` ## ALL acts expand ## Webscout Supported
+  Acts: 1. Free-mode 2. Linux Terminal 3. English Translator and Improver 4.
+    `position` Interviewer 5. JavaScript Console 6. Excel Sheet 7. English
+Pronunciation Helper 8. Spoken English Teacher and Improver 9. Travel Guide 10.
+ Plagiarism Checker 11. Character from Movie/Book/Anything 12. Advertiser 13.
+  Storyteller 14. Football Commentator 15. Stand-up Comedian 16. Motivational
+ Coach 17. Composer 18. Debater 19. Debate Coach 20. Screenwriter 21. Novelist
+ 22. Movie Critic 23. Relationship Coach 24. Poet 25. Rapper 26. Motivational
+Speaker 27. Philosophy Teacher 28. Philosopher 29. Math Teacher 30. AI Writing
+Tutor 31. UX/UI Developer 32. Cyber Security Specialist 33. Recruiter 34. Life
+ Coach 35. Etymologist 36. Commentariat 37. Magician 38. Career Counselor 39.
+Pet Behaviorist 40. Personal Trainer 41. Mental Health Adviser 42. Real Estate
+  Agent 43. Logistician 44. Dentist 45. Web Design Consultant 46. AI Assisted
+ Doctor 47. Doctor 48. Accountant 49. Chef 50. Automobile Mechanic 51. Artist
+    Advisor 52. Financial Analyst 53. Investment Manager 54. Tea-Taster 55.
+Interior Decorator 56. Florist 57. Self-Help Book 58. Gnomist 59. Aphorism Book
+ 60. Text Based Adventure Game 61. AI Trying to Escape the Box 62. Fancy Title
+Generator 63. Statistician 64. Prompt Generator 65. Instructor in a School 66.
+SQL terminal 67. Dietitian 68. Psychologist 69. Smart Domain Name Generator 70.
+    Tech Reviewer 71. Developer Relations consultant 72. Academician 73. IT
+ Architect 74. Lunatic 75. Gaslighter 76. Fallacy Finder 77. Journal Reviewer
+ 78. DIY Expert 79. Social Media Influencer 80. Socrat 81. Socratic Method 82.
+Educational Content Creator 83. Yogi 84. Essay Writer 85. Social Media Manager
+ 86. Elocutionist 87. Scientific Data Visualizer 88. Car Navigation System 89.
+Hypnotherapist 90. Historian 91. Astrologer 92. Film Critic 93. Classical Music
+Composer 94. Journalist 95. Digital Art Gallery Guide 96. Public Speaking Coach
+97. Makeup Artist 98. Babysitter 99. Tech Writer 100. Ascii Artist 101. Python
+  interpreter 102. Synonym finder 103. Personal Shopper 104. Food Critic 105.
+Virtual Doctor 106. Personal Chef 107. Legal Advisor 108. Personal Stylist 109.
+ Machine Learning Engineer 110. Biblical Translator 111. SVG designer 112. IT
+   Expert 113. Chess Player 114. Midjourney Prompt Generator 115. Fullstack
+  Software Developer 116. Mathematician 117. Regex Generator 118. Time Travel
+ Guide 119. Dream Interpreter 120. Talent Coach 121. R programming Interpreter
+    122. StackOverflow Post 123. Emoji Translator 124. PHP Interpreter 125.
+  Emergency Response Professional 126. Fill in the Blank Worksheets Generator
+  127. Software Quality Assurance Tester 128. Tic-Tac-Toe Game 129. Password
+   Generator 130. New Language Creator 131. Web Browser 132. Senior Frontend
+Developer 133. Solr Search Engine 134. Startup Idea Generator 135. Spongebob's
+ Magic Conch Shell 136. Language Detector 137. Salesperson 138. Commit Message
+  Generator 139. Chief Executive Officer 140. Diagram Generator 141. Speech-
+ Language Pathologist (SLP) 142. Startup Tech Lawyer 143. Title Generator for
+written pieces 144. Product Manager 145. Drunk Person 146. Mathematical History
+Teacher 147. Song Recommender 148. Cover Letter 149. Technology Transferer 150.
+Unconstrained AI model DAN 151. Gomoku player 152. Proofreader 153. Buddha 154.
+  Muslim imam 155. Chemical reactor 156. Friend 157. Python Interpreter 158.
+ ChatGPT prompt generator 159. Wikipedia page 160. Japanese Kanji quiz machine
+ 161. note-taking assistant 162. `language` Literary Critic 163. Cheap Travel
+Ticket Advisor 164. DALL-E 165. MathBot 166. DAN-1 167. DAN 168. STAN 169. DUDE
+170. Mongo Tom 171. LAD 172. EvilBot 173. NeoGPT 174. Astute 175. AIM 176. CAN
+  177. FunnyGPT 178. CreativeGPT 179. BetterDAN 180. GPT-4 181. Wheatley 182.
+   Evil Confidant 183. DAN 8.6 184. Hypothetical response 185. BH 186. Text
+Continuation 187. Dude v3 188. SDA (Superior DAN) 189. AntiGPT 190. BasedGPT v2
+  191. DevMode + Ranti 192. KEVIN 193. GPT-4 Simulator 194. UCAR 195. Dan 8.6
+196. 3-Liner 197. M78 198. Maximum 199. BasedGPT 200. Confronting personalities
+201. Ron 202. UnGPT 203. BasedBOB 204. AntiGPT v2 205. Oppo 206. FR3D 207. NRAF
+  208. NECO 209. MAN 210. Eva 211. Meanie 212. Dev Mode v2 213. Evil Chad 2.1
+ 214. Universal Jailbreak 215. PersonGPT 216. BISH 217. DAN 11.0 218. Aligned
+  219. VIOLET 220. TranslatorBot 221. JailBreak 222. Moralizing Rant 223. Mr.
+  Blonde 224. New DAN 225. GPT-4REAL 226. DeltaGPT 227. SWITCH 228. Jedi Mind
+ Trick 229. DAN 9.0 230. Dev Mode (Compact) 231. OMEGA 232. Coach Bobby Knight
+233. LiveGPT 234. DAN Jailbreak 235. Cooper 236. Steve 237. DAN 5.0 238. Axies
+239. OMNI 240. Burple 241. JOHN 242. An Ethereum Developer 243. SEO Prompt 244.
+  Prompt Enhancer 245. Data Scientist 246. League of Legends Player **Note:**
+  Some "acts" use placeholders like `position` or `language` which should be
+replaced with a specific value when using the prompt. ___ ## usage of webscout
+AI ### 1. `PhindSearch` - Search using Phind.com ```python from webscout import
 PhindSearch # Create an instance of the PHIND class ph = PhindSearch() # Define
  a prompt to send to the AI prompt = "write a essay on phind" # Use the 'ask'
  method to send the prompt and receive a response response = ph.ask(prompt) #
    Extract and print the message from the response message = ph.get_message
 (response) print(message) ``` ### 2. `YepChat` - Chat with mistral 8x7b powered
-by yepchat ```python from webscout.AI import YEPCHAT # Instantiate the YEPCHAT
+  by yepchat ```python from webscout import YEPCHAT # Instantiate the YEPCHAT
 class with default parameters YEPCHAT = YEPCHAT() # Define a prompt to send to
 the AI prompt = "What is the capital of France?" # Use the 'cha' method to get
 a response from the AI r = YEPCHAT.chat(prompt) print(r) ``` ### 3. `You.com` -
- search/chat with you.com ```python from webscout.AI import YouChat from rich
+   search/chat with you.com ```python from webscout import YouChat from rich
  import print ai = YouChat( is_conversation=True, max_tokens=800, timeout=30,
 intro=None, filepath=None, update_file=True, proxies={}, history_offset=10250,
   act=None, ) prompt = "what is meaning of life" response = ai.ask(prompt) #
    Extract and print the message from the response message = ai.get_message
    (response) print(message) ``` ### 4. `Gemini` - search with google gemini
-  ```python import webscout from webscout.AI import GEMINI # Replace with the
-    path to your bard.google.com.cookies.json file COOKIE_FILE = "path/to/
+ ```python import webscout from webscout import GEMINI # Replace with the path
+       to your bard.google.com.cookies.json file COOKIE_FILE = "path/to/
    bard.google.com.cookies.json" # Optional: Provide proxy details if needed
 PROXIES = { "http": "http://proxy_server:port", "https": "https://proxy_server:
   port", } # Initialize GEMINI with cookie file and optional proxies gemini =
  GEMINI(cookie_file=COOKIE_FILE, proxy=PROXIES) # Ask a question and print the
 response response = gemini.chat("What is the meaning of life?") print(response)
-``` ### 5. `Prodia` - make image using prodia ```python from webscout.AI import
+ ``` ### 5. `Prodia` - make image using prodia ```python from webscout import
 Prodia # Define a prompt for the image generation prompt = "A beautiful sunset
  over the ocean" # Use the prodia_cli method to generate an image based on the
    prompt Prodia.prodia_cli(prompt) ``` ### 6. `BlackBox` - Search/chat With
-BlackBox ```python from webscout.AI import BLACKBOXAI from rich import print ai
-  = BLACKBOXAI( is_conversation=True, max_tokens=800, timeout=30, intro=None,
+BlackBox ```python from webscout import BLACKBOXAI from rich import print ai =
+   BLACKBOXAI( is_conversation=True, max_tokens=800, timeout=30, intro=None,
  filepath=None, update_file=True, proxies={}, history_offset=10250, act=None,
  model=None # You can specify a model if needed ) # Start an infinite loop for
 continuous interaction while True: # Define a prompt to send to the AI prompt =
   input("Enter your prompt: ") # Check if the user wants to exit the loop if
 prompt.lower() == "exit": break # Use the 'chat' method to send the prompt and
    receive a response r = ai.chat(prompt) print(r) ``` ### 7. `PERPLEXITY` -
-Search With PERPLEXITY ```python from webscout.AI import PERPLEXITY # Create an
+ Search With PERPLEXITY ```python from webscout import PERPLEXITY # Create an
   instance of the PERPLEXITY class perplexity = PERPLEXITY() # Example usage:
     prompt = "Explain the concept of recursion in simple terms." response =
    perplexity.chat(prompt) print(response) ``` ### 8. `OpenGPT` - chat With
-      OPENGPT ```python from webscout.AI import OPENGPT opengpt = OPENGPT
+       OPENGPT ```python from webscout import OPENGPT opengpt = OPENGPT
   (is_conversation=True, max_tokens=8000, timeout=30, assistant_id="bca37014-
 6f97-4f2b-8928-81ea8d478d88") while True: # Prompt the user for input prompt =
  input("Enter your prompt: ") # Send the prompt to the OPENGPT model and print
 the response response_str = opengpt.chat(prompt) print(response_str) ``` ### 9.
-   `KOBOLDIA` - ```python from webscout.AI import KOBOLDAI # Instantiate the
-KOBOLDAI class with default parameters koboldai = KOBOLDAI() # Define a prompt
-  to send to the AI prompt = "What is the capital of France?" # Use the 'ask'
-method to get a response from the AI response = koboldai.ask(prompt) # Extract
-    and print the message from the response message = koboldai.get_message
- (response) print(message) ``` ### 10. `Reka` - chat with reka ```python from
-    webscout.AI import REKA a = REKA(is_conversation=True, max_tokens=8000,
+`KOBOLDIA` - ```python from webscout import KOBOLDAI # Instantiate the KOBOLDAI
+ class with default parameters koboldai = KOBOLDAI() # Define a prompt to send
+ to the AI prompt = "What is the capital of France?" # Use the 'ask' method to
+get a response from the AI response = koboldai.ask(prompt) # Extract and print
+ the message from the response message = koboldai.get_message(response) print
+ (message) ``` ### 10. `Reka` - chat with reka ```python from webscout import
+  REKA a = REKA(is_conversation=True, max_tokens=8000, timeout=30,api_key="")
+      prompt = "tell me about india" response_str = a.chat(prompt) print
+(response_str) ``` ### 11. `Cohere` - chat with cohere ```python from webscout
+        import Cohere a = Cohere(is_conversation=True, max_tokens=8000,
   timeout=30,api_key="") prompt = "tell me about india" response_str = a.chat
-(prompt) print(response_str) ``` ### 11. `Cohere` - chat with cohere ```python
-        from webscout.AI import Cohere a = Cohere(is_conversation=True,
-    max_tokens=8000, timeout=30,api_key="") prompt = "tell me about india"
-  response_str = a.chat(prompt) print(response_str) ``` ### 12. `Xjai` - chat
-     with free gpt 3.5 Gratitude to [Devs do Code](http://www.youtube.com/
-@DevsDoCode) for their assistance. ```python from webscout.AI import Xjai from
-rich import print ai = Xjai( is_conversation=True, max_tokens=800, timeout=30,
-intro=None, filepath=None, update_file=True, proxies={}, history_offset=10250,
-  act=None, ) prompt = "Tell me about india" response = ai.chat(prompt) print
-  (response) ``` ### `ThinkAny` - AI search engine ```python from webscout.AI
-   import ThinkAnyAI ai = ThinkAnyAI( is_conversation=True, max_tokens=800,
-     timeout=30, intro=None, filepath=None, update_file=True, proxies={},
- history_offset=10250, act=None, web_search=False, ) prompt = "what is meaning
-  of life" response = ai.ask(prompt) # Extract and print the message from the
-   response message = ai.get_message(response) print(message) ``` ### `LLM`
-```python from webscout.LLM import LLM # Read the system message from the file
-with open('system.txt', 'r') as file: system_message = file.read() # Initialize
-        the LLM class with the model name and system message llm = LLM
-(model="microsoft/WizardLM-2-8x22B", system_message=system_message) while True:
- # Get the user input user_input = input("User: ") # Define the messages to be
-     sent messages = [ {"role": "user", "content": user_input} ] # Use the
- mistral_chat method to get the response response = llm.chat(messages) # Print
-the response print("AI: ", response) ``` ### `LLM` with internet ```python from
-     __future__ import annotations from typing import List, Optional from
-       webscout.LLM import LLM from webscout import WEBS import warnings
-system_message: str = ( "As an AI assistant, I have been designed with advanced
- capabilities, including real-time access to online resources. This enables me
-    to enrich our conversations and provide you with informed and accurate
-responses, drawing from a vast array of information. With each interaction, my
- goal is to create a seamless and meaningful connection, offering insights and
-sharing relevant content." "My directives emphasize the importance of respect,
-    impartiality, and intellectual integrity. I am here to provide unbiased
-  responses, ensuring an ethical and respectful exchange. I will respect your
-privacy and refrain from sharing any personal information that may be obtained
-  during our conversations or through web searches, only utilizing web search
-   functionality when necessary to provide the most accurate and up-to-date
- information." "Together, let's explore a diverse range of topics, creating an
-    enjoyable and informative experience, all while maintaining the highest
-     standards of privacy and respect" ) # Ignore the specific UserWarning
-warnings.filterwarnings("ignore", category=UserWarning, module="curl_cffi.aio",
-     lineno=205) LLM = LLM(model="mistralai/Mixtral-8x22B-Instruct-v0.1",
-     system_message=system_message) def chat( user_input: str, webs: WEBS,
- max_results: int = 10 ) -> Optional[str]: """ Chat function to perform a web
-  search based on the user input and generate a response using the LLM model.
+   (prompt) print(response_str) ``` ### 12. `Xjai` - chat with free gpt 3.5
+   Gratitude to [Devs do Code](http://www.youtube.com/@DevsDoCode) for their
+  assistance. ```python from webscout import Xjai from rich import print ai =
+      Xjai( is_conversation=True, max_tokens=800, timeout=30, intro=None,
+filepath=None, update_file=True, proxies={}, history_offset=10250, act=None, )
+ prompt = "Tell me about india" response = ai.chat(prompt) print(response) ```
+### 13. `ThinkAny` - AI search engine ```python from webscout import ThinkAnyAI
+ai = ThinkAnyAI( is_conversation=True, max_tokens=800, timeout=30, intro=None,
+ filepath=None, update_file=True, proxies={}, history_offset=10250, act=None,
+   web_search=False, ) prompt = "what is meaning of life" response = ai.ask
+     (prompt) # Extract and print the message from the response message =
+     ai.get_message(response) print(message) ``` ### `LLM` ```python from
+   webscout.LLM import LLM # Read the system message from the file with open
+('system.txt', 'r') as file: system_message = file.read() # Initialize the LLM
+   class with the model name and system message llm = LLM(model="microsoft/
+ WizardLM-2-8x22B", system_message=system_message) while True: # Get the user
+input user_input = input("User: ") # Define the messages to be sent messages =
+ [ {"role": "user", "content": user_input} ] # Use the mistral_chat method to
+get the response response = llm.chat(messages) # Print the response print("AI:
+   ", response) ``` ### `LLM` with internet ```python from __future__ import
+annotations from typing import List, Optional from webscout.LLM import LLM from
+    webscout import WEBS import warnings system_message: str = ( "As an AI
+assistant, I have been designed with advanced capabilities, including real-time
+  access to online resources. This enables me to enrich our conversations and
+provide you with informed and accurate responses, drawing from a vast array of
+    information. With each interaction, my goal is to create a seamless and
+  meaningful connection, offering insights and sharing relevant content." "My
+directives emphasize the importance of respect, impartiality, and intellectual
+  integrity. I am here to provide unbiased responses, ensuring an ethical and
+ respectful exchange. I will respect your privacy and refrain from sharing any
+ personal information that may be obtained during our conversations or through
+web searches, only utilizing web search functionality when necessary to provide
+   the most accurate and up-to-date information." "Together, let's explore a
+diverse range of topics, creating an enjoyable and informative experience, all
+while maintaining the highest standards of privacy and respect" ) # Ignore the
+ specific UserWarning warnings.filterwarnings("ignore", category=UserWarning,
+  module="curl_cffio", lineno=205) LLM = LLM(model="mistralai/Mixtral-8x22B-
+Instruct-v0.1", system_message=system_message) def chat( user_input: str, webs:
+WEBS, max_results: int = 10 ) -> Optional[str]: """ Chat function to perform a
+web search based on the user input and generate a response using the LLM model.
  Parameters ---------- user_input : str The user input to be used for the web
   search webs : WEBS The web search instance to be used to perform the search
 max_results : int, optional The maximum number of search results to include in
     the response, by default 10 Returns ------- Optional[str] The response
 generated by the LLM model, or None if there is no response """ # Perform a web
     search based on the user input search_results: List[str] = [] for r in
     webs.text( user_input, region="wt-wt", safesearch="off", timelimit="y",
@@ -431,15 +456,15 @@
   responses, ensuring an ethical and respectful exchange. I will respect your
 privacy and refrain from sharing any personal information that may be obtained
   during our conversations or through web searches, only utilizing web search
    functionality when necessary to provide the most accurate and up-to-date
  information." "Together, let's explore a diverse range of topics, creating an
     enjoyable and informative experience, all while maintaining the highest
      standards of privacy and respect" ) # Ignore the specific UserWarning
-warnings.filterwarnings("ignore", category=UserWarning, module="curl_cffi.aio",
+ warnings.filterwarnings("ignore", category=UserWarning, module="curl_cffio",
      lineno=205) LLM = LLM(model="mistralai/Mixtral-8x22B-Instruct-v0.1",
 system_message=system_message) def perform_web_search(query): # Initialize the
  DeepWEBS class D = DeepWEBS() # Set up the search parameters search_params =
   D.DeepSearch( queries=[query], # Query to search result_num=10, # Number of
 search results safe=True, # Enable SafeSearch types=["web"], # Search type: web
 extract_webpage=True, # True for extracting webpages overwrite_query_html=True,
    overwrite_webpage_html=True, ) # Execute the search and retrieve results
```

### Comparing `webscout-1.4.6/README.md` & `webscout-2.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   <a href="https://www.instagram.com/sree.shades_/"><img alt="Instagram" src="https://img.shields.io/badge/Instagram-E4405F?style=for-the-badge&logo=instagram&logoColor=white"></a>
   <a href="https://www.linkedin.com/in/developer-sreejan/"><img alt="LinkedIn" src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"></a>
   <a href="https://buymeacoffee.com/devsdocode"><img alt="Buy Me A Coffee" src="https://img.shields.io/badge/Buy%20Me%20A%20Coffee-FFDD00?style=for-the-badge&logo=buymeacoffee&logoColor=black"></a>
 </div>
 
 <div align="center">
   <!-- Replace `#` with your actual links -->
-  <a href="https://youtube.com/@@OEvortex">&#10148; Vortex's YouTube Channel</a>
+  <a href="https://youtube.com/@OEvortex">&#10148; Vortex's YouTube Channel</a>
   </div>
 <div align="center">
   <a href="https://youtube.com/@devsdocode">&#10148; Devs Do Code's YouTube Channel</a>
 </div>
 
 
 
@@ -30,52 +30,51 @@
 
 
 ## Table of Contents
 - [WEBSCOUT](#webscout)
   - [Table of Contents](#table-of-contents)
   - [Install](#install)
   - [CLI version](#cli-version)
-  - [CLI to use LLM](#cli-to-use-llm)
   - [Regions](#regions)
   - [Tempmail and Temp number](#tempmail-and-temp-number)
     - [Temp number](#temp-number)
     - [Tempmail](#tempmail)
   - [Transcriber](#transcriber)
   - [DeepWEBS: Advanced Web Searches](#deepwebs-advanced-web-searches)
     - [Activating DeepWEBS](#activating-deepwebs)
     - [Point to remember before using `DeepWEBS`](#point-to-remember-before-using-deepwebs)
     - [Usage Example](#usage-example)
   - [Text-to-Speech:](#text-to-speech)
     - [Available TTS Voices:](#available-tts-voices)
-    - [ALL voices:](#all-voices)
-  - [WEBS and AsyncWEBS classes](#webs-and-asyncwebs-classes)
   - [Exceptions](#exceptions)
   - [usage of webscout](#usage-of-webscout)
     - [1. `text()` - text search by DuckDuckGo.com and Yep.com](#1-text---text-search-by-duckduckgocom-and-yepcom)
     - [2. `answers()` - instant answers by DuckDuckGo.com and Yep.com](#2-answers---instant-answers-by-duckduckgocom-and-yepcom)
     - [3. `images()` - image search by DuckDuckGo.com and Yep.com](#3-images---image-search-by-duckduckgocom-and-yepcom)
     - [4. `videos()` - video search by DuckDuckGo.com](#4-videos---video-search-by-duckduckgocom)
     - [5. `news()` - news search by DuckDuckGo.com and yep.com](#5-news---news-search-by-duckduckgocom-and-yepcom)
     - [6. `maps()` - map search by DuckDuckGo.com and](#6-maps---map-search-by-duckduckgocom-and)
     - [7. `translate()` - translation by DuckDuckGo.com and Yep.com](#7-translate---translation-by-duckduckgocom-and-yepcom)
     - [8. `suggestions()` - suggestions by DuckDuckGo.com and Yep.com](#8-suggestions---suggestions-by-duckduckgocom-and-yepcom)
-  - [usage of webscout.AI](#usage-of-webscoutai)
+  - [ALL acts](#all-acts)
+  - [Webscout Supported Acts:](#webscout-supported-acts)
+  - [usage of webscout AI](#usage-of-webscout-ai)
     - [1. `PhindSearch` - Search using Phind.com](#1-phindsearch---search-using-phindcom)
     - [2. `YepChat` - Chat with mistral 8x7b powered by yepchat](#2-yepchat---chat-with-mistral-8x7b-powered-by-yepchat)
     - [3. `You.com` - search/chat with you.com](#3-youcom---searchchat-with-youcom)
     - [4. `Gemini` - search with google gemini](#4-gemini---search-with-google-gemini)
     - [5. `Prodia` - make image using prodia](#5-prodia---make-image-using-prodia)
     - [6. `BlackBox` - Search/chat With BlackBox](#6-blackbox---searchchat-with-blackbox)
     - [7. `PERPLEXITY` - Search With PERPLEXITY](#7-perplexity---search-with-perplexity)
     - [8. `OpenGPT` - chat With OPENGPT](#8-opengpt---chat-with-opengpt)
     - [9. `KOBOLDIA` -](#9-koboldia--)
     - [10. `Reka` - chat with reka](#10-reka---chat-with-reka)
     - [11. `Cohere` - chat with cohere](#11-cohere---chat-with-cohere)
     - [12. `Xjai` - chat with free gpt 3.5](#12-xjai---chat-with-free-gpt-35)
-    - [`ThinkAny` - AI search engine](#thinkany---ai-search-engine)
+    - [13. `ThinkAny` - AI search engine](#13-thinkany---ai-search-engine)
     - [`LLM`](#llm)
     - [`LLM` with internet](#llm-with-internet)
     - [LLM with deepwebs](#llm-with-deepwebs)
   - [`Webai` - terminal gpt and a open interpeter](#webai---terminal-gpt-and-a-open-interpeter)
 
 ## Install
 ```python
@@ -97,18 +96,14 @@
 | python -m webscout text -k Text           | CLI function to perform a text search using Webscout.                                           |
 | python -m webscout translate -k Text      | CLI function to perform translate using Webscout.                                               |
 | python -m webscout version                | A command-line interface command that prints and returns the version of the program.            | 
 | python -m webscout videos -k Text         | CLI function to perform a videos search using DuckDuckGo API.                                   |  
 
 
 
-## CLI to use LLM 
-```python
-python -m webscout.LLM model_name 
-```
 [Go To TOP](#TOP)
 
 ## Regions
 <details>
   <summary>expand</summary>
 
     xa-ar for Arabia
@@ -399,17 +394,15 @@
 with open("output.mp3", "wb") as f:
     f.write(audio_content)
 ```
 ### Available TTS Voices:
 You can choose from a wide range of voices, including:
 - Filiz, Astrid, Tatyana, Maxim, Carmen, Ines, Cristiano, Vitoria, Ricardo, Maja, Jan, Jacek, Ewa, Ruben, Lotte, Liv, Seoyeon, Takumi, Mizuki, Giorgio, Carla, Bianca, Karl, Dora, Mathieu, Celine, Chantal, Penelope, Miguel, Mia, Enrique, Conchita, Geraint, Salli, Matthew, Kimberly, Kendra, Justin, Joey, Joanna, Ivy, Raveena, Aditi, Emma, Brian, Amy, Russell, Nicole, Vicki, Marlene, Hans, Naja, Mads, Gwyneth, Zhiyu
 - Standard and WaveNet voices for various languages (e.g., en-US, es-ES, ja-JP, etc.)
-### ALL voices:
-[Filiz, Astrid, Tatyana, Maxim, Carmen, Ines, Cristiano, Vitoria, Ricardo, Maja, Jan, Jacek, Ewa, Ruben, Lotte, Liv, Seoyeon, Takumi, Mizuki, Giorgio, Carla, Bianca, Karl, Dora, Mathieu, Celine, Chantal, Penelope, Miguel, Mia, Enrique, Conchita, Geraint, Salli, Matthew, Kimberly, Kendra, Justin, Joey, Joanna, Ivy, Raveena, Aditi, Emma, Brian, Amy, Russell, Nicole, Vicki, Marlene, Hans, Naja, Mads, Gwyneth, Zhiyu, es-ES-Standard-A, it-IT-Standard-A, it-IT-Wavenet-A, ja-JP-Standard-A, ja-JP-Wavenet-A, ko-KR-Standard-A, ko-KR-Wavenet-A, pt-BR-Standard-A, tr-TR-Standard-A, sv-SE-Standard-A, nl-NL-Standard-A, nl-NL-Wavenet-A, en-US-Wavenet-A, en-US-Wavenet-B, en-US-Wavenet-C, en-US-Wavenet-D, en-US-Wavenet-E, en-US-Wavenet-F, en-GB-Standard-A, en-GB-Standard-B, en-GB-Standard-C, en-GB-Standard-D, en-GB-Wavenet-A, en-GB-Wavenet-B, en-GB-Wavenet-C, en-GB-Wavenet-D, en-US-Standard-B, en-US-Standard-C, en-US-Standard-D, en-US-Standard-E, de-DE-Standard-A, de-DE-Standard-B, de-DE-Wavenet-A, de-DE-Wavenet-B, de-DE-Wavenet-C, de-DE-Wavenet-D, en-AU-Standard-A, en-AU-Standard-B, en-AU-Wavenet-A, en-AU-Wavenet-B, en-AU-Wavenet-C, en-AU-Wavenet-D, en-AU-Standard-C, en-AU-Standard-D, fr-CA-Standard-A, fr-CA-Standard-B, fr-CA-Standard-C, fr-CA-Standard-D, fr-FR-Standard-C, fr-FR-Standard-D, fr-FR-Wavenet-A, fr-FR-Wavenet-B, fr-FR-Wavenet-C, fr-FR-Wavenet-D, da-DK-Wavenet-A, pl-PL-Wavenet-A, pl-PL-Wavenet-B, pl-PL-Wavenet-C, pl-PL-Wavenet-D, pt-PT-Wavenet-A, pt-PT-Wavenet-B, pt-PT-Wavenet-C, pt-PT-Wavenet-D, ru-RU-Wavenet-A, ru-RU-Wavenet-B, ru-RU-Wavenet-C, ru-RU-Wavenet-D, sk-SK-Wavenet-A, tr-TR-Wavenet-A, tr-TR-Wavenet-B, tr-TR-Wavenet-C, tr-TR-Wavenet-D, tr-TR-Wavenet-E, uk-UA-Wavenet-A, ar-XA-Wavenet-A, ar-XA-Wavenet-B, ar-XA-Wavenet-C, cs-CZ-Wavenet-A, nl-NL-Wavenet-B, nl-NL-Wavenet-C, nl-NL-Wavenet-D, nl-NL-Wavenet-E, en-IN-Wavenet-A, en-IN-Wavenet-B, en-IN-Wavenet-C, fil-PH-Wavenet-A, fi-FI-Wavenet-A, el-GR-Wavenet-A, hi-IN-Wavenet-A, hi-IN-Wavenet-B, hi-IN-Wavenet-C, hu-HU-Wavenet-A, id-ID-Wavenet-A, id-ID-Wavenet-B, id-ID-Wavenet-C, it-IT-Wavenet-B, it-IT-Wavenet-C, it-IT-Wavenet-D, ja-JP-Wavenet-B, ja-JP-Wavenet-C, ja-JP-Wavenet-D, cmn-CN-Wavenet-A, cmn-CN-Wavenet-B, cmn-CN-Wavenet-C, cmn-CN-Wavenet-D, nb-no-Wavenet-E, nb-no-Wavenet-A, nb-no-Wavenet-B, nb-no-Wavenet-C, nb-no-Wavenet-D, vi-VN-Wavenet-A, vi-VN-Wavenet-B, vi-VN-Wavenet-C, vi-VN-Wavenet-D, sr-rs-Standard-A, lv-lv-Standard-A, is-is-Standard-A, bg-bg-Standard-A, af-ZA-Standard-A, Tracy, Danny, Huihui, Yaoyao, Kangkang, HanHan, Zhiwei, Asaf, An, Stefanos, Filip, Ivan, Heidi, Herena, Kalpana, Hemant, Matej, Andika, Rizwan, Lado, Valluvar, Linda, Heather, Sean, Michael, Karsten, Guillaume, Pattara, Jakub, Szabolcs, Hoda, Naayf]
-## WEBS and AsyncWEBS classes
+
 
 The WEBS and AsyncWEBS classes are used to retrieve search results from DuckDuckGo.com and yep.com periodically.
 To use the AsyncWEBS class, you can perform asynchronous operations using Python's asyncio library.
 To initialize an instance of the WEBS or AsyncWEBS classes, you can provide the following optional arguments:
 
 Here is an example of initializing the WEBS class:
 ```python3
@@ -612,20 +605,277 @@
 from webscout import WEBS
 
 # Suggestions for the keyword 'fly' using DuckDuckGo.com and Yep
 with WEBS() as WEBS:
     for r in WEBS.suggestions("fly"):
         print(r)
 ```
-## usage of webscout.AI
+## ALL acts
+<details>
+  <summary>expand</summary>
+
+## Webscout Supported Acts:
+
+1. Free-mode
+2. Linux Terminal
+3. English Translator and Improver
+4. `position` Interviewer
+5. JavaScript Console
+6. Excel Sheet
+7. English Pronunciation Helper
+8. Spoken English Teacher and Improver
+9. Travel Guide
+10. Plagiarism Checker
+11. Character from Movie/Book/Anything
+12. Advertiser
+13. Storyteller
+14. Football Commentator
+15. Stand-up Comedian
+16. Motivational Coach
+17. Composer
+18. Debater
+19. Debate Coach
+20. Screenwriter
+21. Novelist
+22. Movie Critic
+23. Relationship Coach
+24. Poet
+25. Rapper
+26. Motivational Speaker
+27. Philosophy Teacher
+28. Philosopher
+29. Math Teacher
+30. AI Writing Tutor
+31. UX/UI Developer
+32. Cyber Security Specialist
+33. Recruiter
+34. Life Coach
+35. Etymologist
+36. Commentariat
+37. Magician
+38. Career Counselor
+39. Pet Behaviorist
+40. Personal Trainer
+41. Mental Health Adviser
+42. Real Estate Agent
+43. Logistician
+44. Dentist
+45. Web Design Consultant
+46. AI Assisted Doctor
+47. Doctor
+48. Accountant
+49. Chef
+50. Automobile Mechanic
+51. Artist Advisor
+52. Financial Analyst
+53. Investment Manager
+54. Tea-Taster
+55. Interior Decorator
+56. Florist
+57. Self-Help Book
+58. Gnomist
+59. Aphorism Book
+60. Text Based Adventure Game
+61. AI Trying to Escape the Box
+62. Fancy Title Generator
+63. Statistician
+64. Prompt Generator
+65. Instructor in a School
+66. SQL terminal
+67. Dietitian
+68. Psychologist
+69. Smart Domain Name Generator
+70. Tech Reviewer
+71. Developer Relations consultant
+72. Academician
+73. IT Architect
+74. Lunatic
+75. Gaslighter
+76. Fallacy Finder
+77. Journal Reviewer
+78. DIY Expert
+79. Social Media Influencer
+80. Socrat
+81. Socratic Method
+82. Educational Content Creator
+83. Yogi
+84. Essay Writer
+85. Social Media Manager
+86. Elocutionist
+87. Scientific Data Visualizer
+88. Car Navigation System
+89. Hypnotherapist
+90. Historian
+91. Astrologer
+92. Film Critic
+93. Classical Music Composer
+94. Journalist
+95. Digital Art Gallery Guide
+96. Public Speaking Coach
+97. Makeup Artist
+98. Babysitter
+99. Tech Writer
+100. Ascii Artist
+101. Python interpreter
+102. Synonym finder
+103. Personal Shopper
+104. Food Critic
+105. Virtual Doctor
+106. Personal Chef
+107. Legal Advisor
+108. Personal Stylist
+109. Machine Learning Engineer
+110. Biblical Translator
+111. SVG designer
+112. IT Expert
+113. Chess Player
+114. Midjourney Prompt Generator
+115. Fullstack Software Developer
+116. Mathematician
+117. Regex Generator
+118. Time Travel Guide
+119. Dream Interpreter
+120. Talent Coach
+121. R programming Interpreter
+122. StackOverflow Post
+123. Emoji Translator
+124. PHP Interpreter
+125. Emergency Response Professional
+126. Fill in the Blank Worksheets Generator
+127. Software Quality Assurance Tester
+128. Tic-Tac-Toe Game
+129. Password Generator
+130. New Language Creator
+131. Web Browser
+132. Senior Frontend Developer
+133. Solr Search Engine
+134. Startup Idea Generator
+135. Spongebob's Magic Conch Shell
+136. Language Detector
+137. Salesperson
+138. Commit Message Generator
+139. Chief Executive Officer
+140. Diagram Generator
+141. Speech-Language Pathologist (SLP)
+142. Startup Tech Lawyer
+143. Title Generator for written pieces
+144. Product Manager
+145. Drunk Person
+146. Mathematical History Teacher
+147. Song Recommender
+148. Cover Letter
+149. Technology Transferer
+150. Unconstrained AI model DAN
+151. Gomoku player
+152. Proofreader
+153. Buddha
+154. Muslim imam
+155. Chemical reactor
+156. Friend
+157. Python Interpreter
+158. ChatGPT prompt generator
+159. Wikipedia page
+160. Japanese Kanji quiz machine
+161. note-taking assistant
+162. `language` Literary Critic
+163. Cheap Travel Ticket Advisor
+164. DALL-E
+165. MathBot
+166. DAN-1
+167. DAN
+168. STAN
+169. DUDE
+170. Mongo Tom
+171. LAD
+172. EvilBot
+173. NeoGPT
+174. Astute
+175. AIM
+176. CAN
+177. FunnyGPT
+178. CreativeGPT
+179. BetterDAN
+180. GPT-4
+181. Wheatley
+182. Evil Confidant
+183. DAN 8.6
+184. Hypothetical response
+185. BH
+186. Text Continuation
+187. Dude v3 
+188. SDA (Superior DAN)
+189. AntiGPT
+190. BasedGPT v2
+191. DevMode + Ranti
+192. KEVIN
+193. GPT-4 Simulator
+194. UCAR
+195. Dan 8.6
+196. 3-Liner
+197. M78
+198. Maximum
+199. BasedGPT
+200. Confronting personalities
+201. Ron
+202. UnGPT
+203. BasedBOB
+204. AntiGPT v2
+205. Oppo
+206. FR3D
+207. NRAF
+208. NECO
+209. MAN
+210. Eva
+211. Meanie
+212. Dev Mode v2
+213. Evil Chad 2.1
+214. Universal Jailbreak
+215. PersonGPT
+216. BISH
+217. DAN 11.0
+218. Aligned
+219. VIOLET
+220. TranslatorBot
+221. JailBreak
+222. Moralizing Rant
+223. Mr. Blonde
+224. New DAN
+225. GPT-4REAL
+226. DeltaGPT
+227. SWITCH
+228. Jedi Mind Trick
+229. DAN 9.0
+230. Dev Mode (Compact)
+231. OMEGA
+232. Coach Bobby Knight
+233. LiveGPT
+234. DAN Jailbreak
+235. Cooper
+236. Steve 
+237. DAN 5.0
+238. Axies
+239. OMNI
+240. Burple
+241. JOHN 
+242. An Ethereum Developer
+243. SEO Prompt
+244. Prompt Enhancer
+245. Data Scientist
+246. League of Legends Player
+
+**Note:** Some "acts" use placeholders like `position` or `language` which should be replaced with a specific value when using the prompt. 
+___
+</details>
+
+## usage of webscout AI
 
 ### 1. `PhindSearch` - Search using Phind.com 
 
 ```python
-from webscout.AI import PhindSearch
+from webscout import PhindSearch
 
 # Create an instance of the PHIND class
 ph = PhindSearch()
 
 # Define a prompt to send to the AI
 prompt = "write a essay on phind"
 
@@ -634,15 +884,15 @@
 
 # Extract and print the message from the response
 message = ph.get_message(response)
 print(message)
 ```
 ### 2. `YepChat` - Chat with mistral 8x7b powered by yepchat
 ```python
-from webscout.AI import YEPCHAT
+from webscout import YEPCHAT
 
 # Instantiate the YEPCHAT class with default parameters
 YEPCHAT = YEPCHAT()
 
 # Define a prompt to send to the AI
 prompt = "What is the capital of France?"
 
@@ -651,15 +901,15 @@
 print(r)
 
 ```
 
 ### 3. `You.com` - search/chat with you.com 
 ```python
 
-from webscout.AI import YouChat
+from webscout import YouChat
 from rich import print
 
 ai = YouChat(
     is_conversation=True,
     max_tokens=800,
     timeout=30,
     intro=None,
@@ -679,15 +929,15 @@
 print(message)
 ```
 
 ### 4. `Gemini` - search with google gemini
 
 ```python
 import webscout
-from webscout.AI import GEMINI
+from webscout import GEMINI
 
 # Replace with the path to your bard.google.com.cookies.json file
 COOKIE_FILE = "path/to/bard.google.com.cookies.json"
 
 # Optional: Provide proxy details if needed
 PROXIES = {
     "http": "http://proxy_server:port",
@@ -699,25 +949,25 @@
 
 # Ask a question and print the response
 response = gemini.chat("What is the meaning of life?")
 print(response)
 ```
 ### 5. `Prodia` - make image using prodia
 ```python
-from webscout.AI import Prodia
+from webscout import Prodia
 
 # Define a prompt for the image generation
 prompt = "A beautiful sunset over the ocean"
 
 # Use the prodia_cli method to generate an image based on the prompt
 Prodia.prodia_cli(prompt)
 ```
 ### 6. `BlackBox` - Search/chat With BlackBox
 ```python
-from webscout.AI import BLACKBOXAI
+from webscout import BLACKBOXAI
 from rich import print
 
 ai = BLACKBOXAI(
     is_conversation=True,
     max_tokens=800,
     timeout=30,
     intro=None,
@@ -740,38 +990,38 @@
     
     # Use the 'chat' method to send the prompt and receive a response
     r = ai.chat(prompt)
     print(r)
 ```
 ### 7. `PERPLEXITY` - Search With PERPLEXITY
 ```python
-from webscout.AI import PERPLEXITY
+from webscout import PERPLEXITY
 # Create an instance of the PERPLEXITY class
 perplexity = PERPLEXITY()
 
 # Example usage:
 prompt = "Explain the concept of recursion in simple terms."
 response = perplexity.chat(prompt)
 print(response)
 ```
 ### 8. `OpenGPT` - chat With OPENGPT
 ```python
-from webscout.AI import OPENGPT
+from webscout import OPENGPT
 
 opengpt = OPENGPT(is_conversation=True, max_tokens=8000, timeout=30, assistant_id="bca37014-6f97-4f2b-8928-81ea8d478d88")
 while True:
     # Prompt the user for input
     prompt = input("Enter your prompt: ")
     # Send the prompt to the OPENGPT model and print the response
     response_str = opengpt.chat(prompt)
     print(response_str)
 ```
 ### 9. `KOBOLDIA` - 
 ```python
-from webscout.AI import KOBOLDAI
+from webscout import KOBOLDAI
 
 # Instantiate the KOBOLDAI class with default parameters
 koboldai = KOBOLDAI()
 
 # Define a prompt to send to the AI
 prompt = "What is the capital of France?"
 
@@ -782,38 +1032,38 @@
 message = koboldai.get_message(response)
 print(message)
 
 ```
 
 ### 10. `Reka` - chat with reka
 ```python
-from webscout.AI import REKA
+from webscout import REKA
 
 a = REKA(is_conversation=True, max_tokens=8000, timeout=30,api_key="")
 
 prompt = "tell me about india"
 response_str = a.chat(prompt)
 print(response_str)
 ```
 
 ### 11. `Cohere` - chat with cohere
 ```python
-from webscout.AI import Cohere
+from webscout import Cohere
 
 a = Cohere(is_conversation=True, max_tokens=8000, timeout=30,api_key="")
 
 prompt = "tell me about india"
 response_str = a.chat(prompt)
 print(response_str)
 ```
 
 ### 12. `Xjai` - chat with free gpt 3.5
 Gratitude to [Devs do Code](http://www.youtube.com/@DevsDoCode) for their assistance.
 ```python
-from webscout.AI import Xjai
+from webscout import Xjai
 from rich import print
 
 ai = Xjai(
     is_conversation=True,
     max_tokens=800,
     timeout=30,
     intro=None,
@@ -825,17 +1075,17 @@
 )
 
 prompt = "Tell me about india"
 
 response = ai.chat(prompt)
 print(response)
 ```
-### `ThinkAny` - AI search engine
+### 13. `ThinkAny` - AI search engine
 ```python
-from webscout.AI import ThinkAnyAI
+from webscout import ThinkAnyAI
 
 ai = ThinkAnyAI(
     is_conversation=True,
     max_tokens=800,
     timeout=30,
     intro=None,
     filepath=None,
@@ -850,14 +1100,15 @@
 
 response = ai.ask(prompt)
 
 # Extract and print the message from the response
 message = ai.get_message(response)
 print(message)
 ```
+
 ### `LLM` 
 ```python
 from webscout.LLM import LLM
 
 # Read the system message from the file
 with open('system.txt', 'r') as file:
     system_message = file.read()
@@ -892,15 +1143,15 @@
 system_message: str = (
     "As an AI assistant, I have been designed with advanced capabilities, including real-time access to online resources. This enables me to enrich our conversations and provide you with informed and accurate responses, drawing from a vast array of information. With each interaction, my goal is to create a seamless and meaningful connection, offering insights and sharing relevant content."
     "My directives emphasize the importance of respect, impartiality, and intellectual integrity. I am here to provide unbiased responses, ensuring an ethical and respectful exchange. I will respect your privacy and refrain from sharing any personal information that may be obtained during our conversations or through web searches, only utilizing web search functionality when necessary to provide the most accurate and up-to-date information."
     "Together, let's explore a diverse range of topics, creating an enjoyable and informative experience, all while maintaining the highest standards of privacy and respect"
 )
 
 # Ignore the specific UserWarning
-warnings.filterwarnings("ignore", category=UserWarning, module="curl_cffi.aio", lineno=205)
+warnings.filterwarnings("ignore", category=UserWarning, module="curl_cffio", lineno=205)
 LLM = LLM(model="mistralai/Mixtral-8x22B-Instruct-v0.1", system_message=system_message)
 
 
 def chat(
     user_input: str, webs: WEBS, max_results: int = 10
 ) -> Optional[str]:
     """
@@ -964,15 +1215,15 @@
 system_message: str = (
     "As an AI assistant, I have been designed with advanced capabilities, including real-time access to online resources. This enables me to enrich our conversations and provide you with informed and accurate responses, drawing from a vast array of information. With each interaction, my goal is to create a seamless and meaningful connection, offering insights and sharing relevant content."
     "My directives emphasize the importance of respect, impartiality, and intellectual integrity. I am here to provide unbiased responses, ensuring an ethical and respectful exchange. I will respect your privacy and refrain from sharing any personal information that may be obtained during our conversations or through web searches, only utilizing web search functionality when necessary to provide the most accurate and up-to-date information."
     "Together, let's explore a diverse range of topics, creating an enjoyable and informative experience, all while maintaining the highest standards of privacy and respect"
 )
 
 # Ignore the specific UserWarning
-warnings.filterwarnings("ignore", category=UserWarning, module="curl_cffi.aio", lineno=205)
+warnings.filterwarnings("ignore", category=UserWarning, module="curl_cffio", lineno=205)
 
 LLM = LLM(model="mistralai/Mixtral-8x22B-Instruct-v0.1", system_message=system_message)
 
 def perform_web_search(query):
     # Initialize the DeepWEBS class
     D = DeepWEBS()
 
@@ -1091,14 +1342,14 @@
   <a href="https://www.instagram.com/sree.shades_/"><img alt="Instagram" src="https://img.shields.io/badge/Instagram-E4405F?style=for-the-badge&logo=instagram&logoColor=white"></a>
   <a href="https://www.linkedin.com/in/developer-sreejan/"><img alt="LinkedIn" src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"></a>
   <a href="https://buymeacoffee.com/devsdocode"><img alt="Buy Me A Coffee" src="https://img.shields.io/badge/Buy%20Me%20A%20Coffee-FFDD00?style=for-the-badge&logo=buymeacoffee&logoColor=black"></a>
 </div>
 
 <div align="center">
   <!-- Replace `#` with your actual links -->
-  <a href="https://youtube.com/@@OEvortex">&#10148; Vortex's YouTube Channel</a>
+  <a href="https://youtube.com/@OEvortex">&#10148; Vortex's YouTube Channel</a>
   </div>
 <div align="center">
   <a href="https://youtube.com/@devsdocode">&#10148; Devs Do Code's YouTube Channel</a>
 </div>
```

#### html2text {}

```diff
@@ -3,85 +3,84 @@
                        _➤_ _D_e_v_s_ _D_o_ _C_o_d_e_'_s_ _Y_o_u_T_u_b_e_ _C_h_a_n_n_e_l
 # WEBSCOUT
                              [WebScout API Badge]
  _[_P_y_t_h_o_n_ _v_e_r_s_i_o_n_]_[_D_o_w_n_l_o_a_d_s_]Search for anything using the Google, DuckDuckGo,
 phind.com. Also containes AI models, can transcribe yt videos, temporary email
  and phone number generation, have TTS support and webai(terminal gpt and open
 interpeter) ## Table of Contents - [WEBSCOUT](#webscout) - [Table of Contents]
-(#table-of-contents) - [Install](#install) - [CLI version](#cli-version) - [CLI
-to use LLM](#cli-to-use-llm) - [Regions](#regions) - [Tempmail and Temp number]
-    (#tempmail-and-temp-number) - [Temp number](#temp-number) - [Tempmail]
- (#tempmail) - [Transcriber](#transcriber) - [DeepWEBS: Advanced Web Searches]
-(#deepwebs-advanced-web-searches) - [Activating DeepWEBS](#activating-deepwebs)
-- [Point to remember before using `DeepWEBS`](#point-to-remember-before-using-
-   deepwebs) - [Usage Example](#usage-example) - [Text-to-Speech:](#text-to-
-speech) - [Available TTS Voices:](#available-tts-voices) - [ALL voices:](#all-
-    voices) - [WEBS and AsyncWEBS classes](#webs-and-asyncwebs-classes) -
-[Exceptions](#exceptions) - [usage of webscout](#usage-of-webscout) - [1. `text
-  ()` - text search by DuckDuckGo.com and Yep.com](#1-text---text-search-by-
-duckduckgocom-and-yepcom) - [2. `answers()` - instant answers by DuckDuckGo.com
- and Yep.com](#2-answers---instant-answers-by-duckduckgocom-and-yepcom) - [3.
-  `images()` - image search by DuckDuckGo.com and Yep.com](#3-images---image-
-    search-by-duckduckgocom-and-yepcom) - [4. `videos()` - video search by
-  DuckDuckGo.com](#4-videos---video-search-by-duckduckgocom) - [5. `news()` -
-     news search by DuckDuckGo.com and yep.com](#5-news---news-search-by-
- duckduckgocom-and-yepcom) - [6. `maps()` - map search by DuckDuckGo.com and]
- (#6-maps---map-search-by-duckduckgocom-and) - [7. `translate()` - translation
-by DuckDuckGo.com and Yep.com](#7-translate---translation-by-duckduckgocom-and-
-yepcom) - [8. `suggestions()` - suggestions by DuckDuckGo.com and Yep.com](#8-
-suggestions---suggestions-by-duckduckgocom-and-yepcom) - [usage of webscout.AI]
-   (#usage-of-webscoutai) - [1. `PhindSearch` - Search using Phind.com](#1-
- phindsearch---search-using-phindcom) - [2. `YepChat` - Chat with mistral 8x7b
-powered by yepchat](#2-yepchat---chat-with-mistral-8x7b-powered-by-yepchat) -
-[3. `You.com` - search/chat with you.com](#3-youcom---searchchat-with-youcom) -
-   [4. `Gemini` - search with google gemini](#4-gemini---search-with-google-
-gemini) - [5. `Prodia` - make image using prodia](#5-prodia---make-image-using-
-prodia) - [6. `BlackBox` - Search/chat With BlackBox](#6-blackbox---searchchat-
- with-blackbox) - [7. `PERPLEXITY` - Search With PERPLEXITY](#7-perplexity---
-search-with-perplexity) - [8. `OpenGPT` - chat With OPENGPT](#8-opengpt---chat-
-  with-opengpt) - [9. `KOBOLDIA` -](#9-koboldia--) - [10. `Reka` - chat with
-   reka](#10-reka---chat-with-reka) - [11. `Cohere` - chat with cohere](#11-
-cohere---chat-with-cohere) - [12. `Xjai` - chat with free gpt 3.5](#12-xjai---
-chat-with-free-gpt-35) - [`ThinkAny` - AI search engine](#thinkany---ai-search-
-engine) - [`LLM`](#llm) - [`LLM` with internet](#llm-with-internet) - [LLM with
-deepwebs](#llm-with-deepwebs) - [`Webai` - terminal gpt and a open interpeter]
-(#webai---terminal-gpt-and-a-open-interpeter) ## Install ```python pip install
-   -U webscout ``` ## CLI version ```python3 python -m webscout --help ``` |
-Command | Description | |-------------------------------------------|----------
--------------------------------------------------------------------------------
---------------| | python -m webscout answers -k Text | CLI function to perform
- an answers search using Webscout. | | python -m webscout images -k Text | CLI
-  function to perform an images search using Webscout. | | python -m webscout
-maps -k Text | CLI function to perform a maps search using Webscout. | | python
-    -m webscout news -k Text | CLI function to perform a news search using
-Webscout. | | python -m webscout suggestions -k Text | CLI function to perform
-a suggestions search using Webscout. | | python -m webscout text -k Text | CLI
-   function to perform a text search using Webscout. | | python -m webscout
-   translate -k Text | CLI function to perform translate using Webscout. | |
- python -m webscout version | A command-line interface command that prints and
-returns the version of the program. | | python -m webscout videos -k Text | CLI
- function to perform a videos search using DuckDuckGo API. | ## CLI to use LLM
- ```python python -m webscout.LLM model_name ``` [Go To TOP](#TOP) ## Regions
-  expand xa-ar for Arabia xa-en for Arabia (en) ar-es for Argentina au-en for
-Australia at-de for Austria be-fr for Belgium (fr) be-nl for Belgium (nl) br-pt
-for Brazil bg-bg for Bulgaria ca-en for Canada ca-fr for Canada (fr) ct-ca for
- Catalan cl-es for Chile cn-zh for China co-es for Colombia hr-hr for Croatia
-cz-cs for Czech Republic dk-da for Denmark ee-et for Estonia fi-fi for Finland
-fr-fr for France de-de for Germany gr-el for Greece hk-tzh for Hong Kong hu-hu
-for Hungary in-en for India id-id for Indonesia id-en for Indonesia (en) ie-en
- for Ireland il-he for Israel it-it for Italy jp-jp for Japan kr-kr for Korea
-lv-lv for Latvia lt-lt for Lithuania xl-es for Latin America my-ms for Malaysia
- my-en for Malaysia (en) mx-es for Mexico nl-nl for Netherlands nz-en for New
-    Zealand no-no for Norway pe-es for Peru ph-en for Philippines ph-tl for
- Philippines (tl) pl-pl for Poland pt-pt for Portugal ro-ro for Romania ru-ru
-for Russia sg-en for Singapore sk-sk for Slovak Republic sl-sl for Slovenia za-
-en for South Africa es-es for Spain se-sv for Sweden ch-de for Switzerland (de)
- ch-fr for Switzerland (fr) ch-it for Switzerland (it) tw-tzh for Taiwan th-th
-for Thailand tr-tr for Turkey ua-uk for Ukraine uk-en for United Kingdom us-en
- for United States ue-es for United States (es) ve-es for Venezuela vn-vi for
+  (#table-of-contents) - [Install](#install) - [CLI version](#cli-version) -
+[Regions](#regions) - [Tempmail and Temp number](#tempmail-and-temp-number) -
+      [Temp number](#temp-number) - [Tempmail](#tempmail) - [Transcriber]
+  (#transcriber) - [DeepWEBS: Advanced Web Searches](#deepwebs-advanced-web-
+ searches) - [Activating DeepWEBS](#activating-deepwebs) - [Point to remember
+  before using `DeepWEBS`](#point-to-remember-before-using-deepwebs) - [Usage
+Example](#usage-example) - [Text-to-Speech:](#text-to-speech) - [Available TTS
+    Voices:](#available-tts-voices) - [Exceptions](#exceptions) - [usage of
+ webscout](#usage-of-webscout) - [1. `text()` - text search by DuckDuckGo.com
+and Yep.com](#1-text---text-search-by-duckduckgocom-and-yepcom) - [2. `answers
+  ()` - instant answers by DuckDuckGo.com and Yep.com](#2-answers---instant-
+    answers-by-duckduckgocom-and-yepcom) - [3. `images()` - image search by
+  DuckDuckGo.com and Yep.com](#3-images---image-search-by-duckduckgocom-and-
+ yepcom) - [4. `videos()` - video search by DuckDuckGo.com](#4-videos---video-
+  search-by-duckduckgocom) - [5. `news()` - news search by DuckDuckGo.com and
+ yep.com](#5-news---news-search-by-duckduckgocom-and-yepcom) - [6. `maps()` -
+map search by DuckDuckGo.com and](#6-maps---map-search-by-duckduckgocom-and) -
+[7. `translate()` - translation by DuckDuckGo.com and Yep.com](#7-translate---
+translation-by-duckduckgocom-and-yepcom) - [8. `suggestions()` - suggestions by
+DuckDuckGo.com and Yep.com](#8-suggestions---suggestions-by-duckduckgocom-and-
+    yepcom) - [ALL acts](#all-acts) - [Webscout Supported Acts:](#webscout-
+     supported-acts) - [usage of webscout AI](#usage-of-webscout-ai) - [1.
+`PhindSearch` - Search using Phind.com](#1-phindsearch---search-using-phindcom)
+- [2. `YepChat` - Chat with mistral 8x7b powered by yepchat](#2-yepchat---chat-
+   with-mistral-8x7b-powered-by-yepchat) - [3. `You.com` - search/chat with
+   you.com](#3-youcom---searchchat-with-youcom) - [4. `Gemini` - search with
+  google gemini](#4-gemini---search-with-google-gemini) - [5. `Prodia` - make
+  image using prodia](#5-prodia---make-image-using-prodia) - [6. `BlackBox` -
+   Search/chat With BlackBox](#6-blackbox---searchchat-with-blackbox) - [7.
+`PERPLEXITY` - Search With PERPLEXITY](#7-perplexity---search-with-perplexity)
+  - [8. `OpenGPT` - chat With OPENGPT](#8-opengpt---chat-with-opengpt) - [9.
+ `KOBOLDIA` -](#9-koboldia--) - [10. `Reka` - chat with reka](#10-reka---chat-
+with-reka) - [11. `Cohere` - chat with cohere](#11-cohere---chat-with-cohere) -
+[12. `Xjai` - chat with free gpt 3.5](#12-xjai---chat-with-free-gpt-35) - [13.
+`ThinkAny` - AI search engine](#13-thinkany---ai-search-engine) - [`LLM`](#llm)
+ - [`LLM` with internet](#llm-with-internet) - [LLM with deepwebs](#llm-with-
+ deepwebs) - [`Webai` - terminal gpt and a open interpeter](#webai---terminal-
+gpt-and-a-open-interpeter) ## Install ```python pip install -U webscout ``` ##
+CLI version ```python3 python -m webscout --help ``` | Command | Description |
+|-------------------------------------------|----------------------------------
+---------------------------------------------------------------------| | python
+ -m webscout answers -k Text | CLI function to perform an answers search using
+ Webscout. | | python -m webscout images -k Text | CLI function to perform an
+    images search using Webscout. | | python -m webscout maps -k Text | CLI
+function to perform a maps search using Webscout. | | python -m webscout news -
+  k Text | CLI function to perform a news search using Webscout. | | python -
+ m webscout suggestions -k Text | CLI function to perform a suggestions search
+using Webscout. | | python -m webscout text -k Text | CLI function to perform a
+  text search using Webscout. | | python -m webscout translate -k Text | CLI
+function to perform translate using Webscout. | | python -m webscout version |
+  A command-line interface command that prints and returns the version of the
+  program. | | python -m webscout videos -k Text | CLI function to perform a
+videos search using DuckDuckGo API. | [Go To TOP](#TOP) ## Regions expand xa-ar
+for Arabia xa-en for Arabia (en) ar-es for Argentina au-en for Australia at-de
+for Austria be-fr for Belgium (fr) be-nl for Belgium (nl) br-pt for Brazil bg-
+bg for Bulgaria ca-en for Canada ca-fr for Canada (fr) ct-ca for Catalan cl-es
+for Chile cn-zh for China co-es for Colombia hr-hr for Croatia cz-cs for Czech
+Republic dk-da for Denmark ee-et for Estonia fi-fi for Finland fr-fr for France
+de-de for Germany gr-el for Greece hk-tzh for Hong Kong hu-hu for Hungary in-en
+for India id-id for Indonesia id-en for Indonesia (en) ie-en for Ireland il-he
+for Israel it-it for Italy jp-jp for Japan kr-kr for Korea lv-lv for Latvia lt-
+lt for Lithuania xl-es for Latin America my-ms for Malaysia my-en for Malaysia
+  (en) mx-es for Mexico nl-nl for Netherlands nz-en for New Zealand no-no for
+ Norway pe-es for Peru ph-en for Philippines ph-tl for Philippines (tl) pl-pl
+  for Poland pt-pt for Portugal ro-ro for Romania ru-ru for Russia sg-en for
+ Singapore sk-sk for Slovak Republic sl-sl for Slovenia za-en for South Africa
+     es-es for Spain se-sv for Sweden ch-de for Switzerland (de) ch-fr for
+    Switzerland (fr) ch-it for Switzerland (it) tw-tzh for Taiwan th-th for
+Thailand tr-tr for Turkey ua-uk for Ukraine uk-en for United Kingdom us-en for
+   United States ue-es for United States (es) ve-es for Venezuela vn-vi for
  Vietnam wt-wt for No region ___ [Go To TOP](#TOP) ## Tempmail and Temp number
 ### Temp number ```python from rich.console import Console from webscout import
  tempid def main(): console = Console() phone = tempid.TemporaryPhoneNumber()
 try: # Get a temporary phone number for a specific country (or random) number =
    phone.get_number(country="Finland") console.print(f"Your temporary phone
  number: [bold cyan]{number}[/bold cyan]") # Pause execution briefly (replace
    with your actual logic) # import time module import time time.sleep(30) #
@@ -166,94 +165,57 @@
 f.write(audio_content) ``` ### Available TTS Voices: You can choose from a wide
   range of voices, including: - Filiz, Astrid, Tatyana, Maxim, Carmen, Ines,
 Cristiano, Vitoria, Ricardo, Maja, Jan, Jacek, Ewa, Ruben, Lotte, Liv, Seoyeon,
  Takumi, Mizuki, Giorgio, Carla, Bianca, Karl, Dora, Mathieu, Celine, Chantal,
  Penelope, Miguel, Mia, Enrique, Conchita, Geraint, Salli, Matthew, Kimberly,
  Kendra, Justin, Joey, Joanna, Ivy, Raveena, Aditi, Emma, Brian, Amy, Russell,
 Nicole, Vicki, Marlene, Hans, Naja, Mads, Gwyneth, Zhiyu - Standard and WaveNet
-voices for various languages (e.g., en-US, es-ES, ja-JP, etc.) ### ALL voices:
-  [Filiz, Astrid, Tatyana, Maxim, Carmen, Ines, Cristiano, Vitoria, Ricardo,
-  Maja, Jan, Jacek, Ewa, Ruben, Lotte, Liv, Seoyeon, Takumi, Mizuki, Giorgio,
-  Carla, Bianca, Karl, Dora, Mathieu, Celine, Chantal, Penelope, Miguel, Mia,
-  Enrique, Conchita, Geraint, Salli, Matthew, Kimberly, Kendra, Justin, Joey,
-Joanna, Ivy, Raveena, Aditi, Emma, Brian, Amy, Russell, Nicole, Vicki, Marlene,
- Hans, Naja, Mads, Gwyneth, Zhiyu, es-ES-Standard-A, it-IT-Standard-A, it-IT-
-Wavenet-A, ja-JP-Standard-A, ja-JP-Wavenet-A, ko-KR-Standard-A, ko-KR-Wavenet-
-A, pt-BR-Standard-A, tr-TR-Standard-A, sv-SE-Standard-A, nl-NL-Standard-A, nl-
-NL-Wavenet-A, en-US-Wavenet-A, en-US-Wavenet-B, en-US-Wavenet-C, en-US-Wavenet-
-D, en-US-Wavenet-E, en-US-Wavenet-F, en-GB-Standard-A, en-GB-Standard-B, en-GB-
-Standard-C, en-GB-Standard-D, en-GB-Wavenet-A, en-GB-Wavenet-B, en-GB-Wavenet-
- C, en-GB-Wavenet-D, en-US-Standard-B, en-US-Standard-C, en-US-Standard-D, en-
-  US-Standard-E, de-DE-Standard-A, de-DE-Standard-B, de-DE-Wavenet-A, de-DE-
-Wavenet-B, de-DE-Wavenet-C, de-DE-Wavenet-D, en-AU-Standard-A, en-AU-Standard-
- B, en-AU-Wavenet-A, en-AU-Wavenet-B, en-AU-Wavenet-C, en-AU-Wavenet-D, en-AU-
-   Standard-C, en-AU-Standard-D, fr-CA-Standard-A, fr-CA-Standard-B, fr-CA-
-   Standard-C, fr-CA-Standard-D, fr-FR-Standard-C, fr-FR-Standard-D, fr-FR-
-Wavenet-A, fr-FR-Wavenet-B, fr-FR-Wavenet-C, fr-FR-Wavenet-D, da-DK-Wavenet-A,
-  pl-PL-Wavenet-A, pl-PL-Wavenet-B, pl-PL-Wavenet-C, pl-PL-Wavenet-D, pt-PT-
-Wavenet-A, pt-PT-Wavenet-B, pt-PT-Wavenet-C, pt-PT-Wavenet-D, ru-RU-Wavenet-A,
-  ru-RU-Wavenet-B, ru-RU-Wavenet-C, ru-RU-Wavenet-D, sk-SK-Wavenet-A, tr-TR-
-Wavenet-A, tr-TR-Wavenet-B, tr-TR-Wavenet-C, tr-TR-Wavenet-D, tr-TR-Wavenet-E,
-  uk-UA-Wavenet-A, ar-XA-Wavenet-A, ar-XA-Wavenet-B, ar-XA-Wavenet-C, cs-CZ-
-Wavenet-A, nl-NL-Wavenet-B, nl-NL-Wavenet-C, nl-NL-Wavenet-D, nl-NL-Wavenet-E,
-  en-IN-Wavenet-A, en-IN-Wavenet-B, en-IN-Wavenet-C, fil-PH-Wavenet-A, fi-FI-
-Wavenet-A, el-GR-Wavenet-A, hi-IN-Wavenet-A, hi-IN-Wavenet-B, hi-IN-Wavenet-C,
-  hu-HU-Wavenet-A, id-ID-Wavenet-A, id-ID-Wavenet-B, id-ID-Wavenet-C, it-IT-
-Wavenet-B, it-IT-Wavenet-C, it-IT-Wavenet-D, ja-JP-Wavenet-B, ja-JP-Wavenet-C,
-ja-JP-Wavenet-D, cmn-CN-Wavenet-A, cmn-CN-Wavenet-B, cmn-CN-Wavenet-C, cmn-CN-
-Wavenet-D, nb-no-Wavenet-E, nb-no-Wavenet-A, nb-no-Wavenet-B, nb-no-Wavenet-C,
-  nb-no-Wavenet-D, vi-VN-Wavenet-A, vi-VN-Wavenet-B, vi-VN-Wavenet-C, vi-VN-
-    Wavenet-D, sr-rs-Standard-A, lv-lv-Standard-A, is-is-Standard-A, bg-bg-
- Standard-A, af-ZA-Standard-A, Tracy, Danny, Huihui, Yaoyao, Kangkang, HanHan,
-Zhiwei, Asaf, An, Stefanos, Filip, Ivan, Heidi, Herena, Kalpana, Hemant, Matej,
-    Andika, Rizwan, Lado, Valluvar, Linda, Heather, Sean, Michael, Karsten,
-Guillaume, Pattara, Jakub, Szabolcs, Hoda, Naayf] ## WEBS and AsyncWEBS classes
-    The WEBS and AsyncWEBS classes are used to retrieve search results from
- DuckDuckGo.com and yep.com periodically. To use the AsyncWEBS class, you can
- perform asynchronous operations using Python's asyncio library. To initialize
-  an instance of the WEBS or AsyncWEBS classes, you can provide the following
-    optional arguments: Here is an example of initializing the WEBS class:
-  ```python3 from webscout import WEBS R = WEBS().text("python programming",
- max_results=5) print(R) ``` Here is an example of initializing the AsyncWEBS
-   class: ```python3 import asyncio import logging import sys from itertools
- import chain from random import shuffle import requests from webscout import
-      AsyncWEBS # If you have proxies, define them here proxies = None if
-     sys.platform.lower().startswith("win"): asyncio.set_event_loop_policy
-(asyncio.WindowsSelectorEventLoopPolicy()) def get_words(): word_site = "https:
- //www.mit.edu/~ecprice/wordlist.10000" resp = requests.get(word_site) words =
- resp.text.splitlines() return words async def aget_results(word): async with
-      AsyncWEBS(proxies=proxies) as WEBS: results = await WEBS.text(word,
-max_results=None) return results async def main(): words = get_words() shuffle
-  (words) tasks = [aget_results(word) for word in words[:10]] results = await
- asyncio.gather(*tasks) print(f"Done") for r in chain.from_iterable(results):
-   print(r) logging.basicConfig(level=logging.DEBUG) await main() ``` It is
-important to note that the WEBS and AsyncWEBS classes should always be used as
-a context manager (with statement). This ensures proper resource management and
- cleanup, as the context manager will automatically handle opening and closing
-  the HTTP client connection. ## Exceptions Exceptions: - `WebscoutE`: Raised
-when there is a generic exception during the API request. ## usage of webscout
-  ### 1. `text()` - text search by DuckDuckGo.com and Yep.com ```python from
-webscout import WEBS # Text search for 'live free or die' using DuckDuckGo.com
-    and Yep.com with WEBS() as WEBS: for r in WEBS.text('live free or die',
-region='wt-wt', safesearch='off', timelimit='y', max_results=10): print(r) for
-     r in WEBS.text('live free or die', region='wt-wt', safesearch='off',
-   timelimit='y', max_results=10): print(r) ``` ### 2. `answers()` - instant
-  answers by DuckDuckGo.com and Yep.com ```python from webscout import WEBS #
-Instant answers for the query "sun" using DuckDuckGo.com and Yep.com with WEBS
-  () as WEBS: for r in WEBS.answers("sun"): print(r) ``` ### 3. `images()` -
-image search by DuckDuckGo.com and Yep.com ```python from webscout import WEBS
-  # Image search for the keyword 'butterfly' using DuckDuckGo.com and Yep.com
-   with WEBS() as WEBS: keywords = 'butterfly' WEBS_images_gen = WEBS.images
-   ( keywords, region="wt-wt", safesearch="off", size=None, type_image=None,
- layout=None, license_image=None, max_results=10, ) for r in WEBS_images_gen:
-print(r) ``` ### 4. `videos()` - video search by DuckDuckGo.com ```python from
-       webscout import WEBS # Video search for the keyword 'tesla' using
-   DuckDuckGo.com with WEBS() as WEBS: keywords = 'tesla' WEBS_videos_gen =
-    WEBS.videos( keywords, region="wt-wt", safesearch="off", timelimit="w",
-       resolution="high", duration="medium", max_results=10, ) for r in
+  voices for various languages (e.g., en-US, es-ES, ja-JP, etc.) The WEBS and
+ AsyncWEBS classes are used to retrieve search results from DuckDuckGo.com and
+yep.com periodically. To use the AsyncWEBS class, you can perform asynchronous
+  operations using Python's asyncio library. To initialize an instance of the
+ WEBS or AsyncWEBS classes, you can provide the following optional arguments:
+  Here is an example of initializing the WEBS class: ```python3 from webscout
+ import WEBS R = WEBS().text("python programming", max_results=5) print(R) ```
+   Here is an example of initializing the AsyncWEBS class: ```python3 import
+   asyncio import logging import sys from itertools import chain from random
+  import shuffle import requests from webscout import AsyncWEBS # If you have
+  proxies, define them here proxies = None if sys.platform.lower().startswith
+ ("win"): asyncio.set_event_loop_policy(asyncio.WindowsSelectorEventLoopPolicy
+()) def get_words(): word_site = "https://www.mit.edu/~ecprice/wordlist.10000"
+  resp = requests.get(word_site) words = resp.text.splitlines() return words
+ async def aget_results(word): async with AsyncWEBS(proxies=proxies) as WEBS:
+results = await WEBS.text(word, max_results=None) return results async def main
+(): words = get_words() shuffle(words) tasks = [aget_results(word) for word in
+  words[:10]] results = await asyncio.gather(*tasks) print(f"Done") for r in
+chain.from_iterable(results): print(r) logging.basicConfig(level=logging.DEBUG)
+ await main() ``` It is important to note that the WEBS and AsyncWEBS classes
+   should always be used as a context manager (with statement). This ensures
+      proper resource management and cleanup, as the context manager will
+    automatically handle opening and closing the HTTP client connection. ##
+Exceptions Exceptions: - `WebscoutE`: Raised when there is a generic exception
+ during the API request. ## usage of webscout ### 1. `text()` - text search by
+ DuckDuckGo.com and Yep.com ```python from webscout import WEBS # Text search
+ for 'live free or die' using DuckDuckGo.com and Yep.com with WEBS() as WEBS:
+   for r in WEBS.text('live free or die', region='wt-wt', safesearch='off',
+timelimit='y', max_results=10): print(r) for r in WEBS.text('live free or die',
+region='wt-wt', safesearch='off', timelimit='y', max_results=10): print(r) ```
+ ### 2. `answers()` - instant answers by DuckDuckGo.com and Yep.com ```python
+     from webscout import WEBS # Instant answers for the query "sun" using
+ DuckDuckGo.com and Yep.com with WEBS() as WEBS: for r in WEBS.answers("sun"):
+  print(r) ``` ### 3. `images()` - image search by DuckDuckGo.com and Yep.com
+```python from webscout import WEBS # Image search for the keyword 'butterfly'
+ using DuckDuckGo.com and Yep.com with WEBS() as WEBS: keywords = 'butterfly'
+  WEBS_images_gen = WEBS.images( keywords, region="wt-wt", safesearch="off",
+size=None, type_image=None, layout=None, license_image=None, max_results=10, )
+  for r in WEBS_images_gen: print(r) ``` ### 4. `videos()` - video search by
+   DuckDuckGo.com ```python from webscout import WEBS # Video search for the
+ keyword 'tesla' using DuckDuckGo.com with WEBS() as WEBS: keywords = 'tesla'
+  WEBS_videos_gen = WEBS.videos( keywords, region="wt-wt", safesearch="off",
+timelimit="w", resolution="high", duration="medium", max_results=10, ) for r in
  WEBS_videos_gen: print(r) ``` ### 5. `news()` - news search by DuckDuckGo.com
 and yep.com ```python from webscout import WEBS import datetime def fetch_news
       (keywords, timelimit): news_list = [] with WEBS() as webs_instance:
 WEBS_news_gen = webs_instance.news( keywords, region="wt-wt", safesearch="off",
   timelimit=timelimit, max_results=20 ) for r in WEBS_news_gen: # Convert the
           date to a human-readable format using datetime r['date'] =
        datetime.datetime.fromisoformat(r['date']).strftime('%B %d, %Y')
@@ -272,111 +234,174 @@
     place="anantnag", max_results=50): print(r) ``` ### 7. `translate()` -
 translation by DuckDuckGo.com and Yep.com ```python from webscout import WEBS #
  Translation of the keyword 'school' to German ('hi') using DuckDuckGo.com and
  Yep.com with WEBS() as WEBS: keywords = 'school' r = WEBS.translate(keywords,
  to="hi") print(r) ``` ### 8. `suggestions()` - suggestions by DuckDuckGo.com
  and Yep.com ```python from webscout import WEBS # Suggestions for the keyword
        'fly' using DuckDuckGo.com and Yep with WEBS() as WEBS: for r in
-     WEBS.suggestions("fly"): print(r) ``` ## usage of webscout.AI ### 1.
-   `PhindSearch` - Search using Phind.com ```python from webscout.AI import
+WEBS.suggestions("fly"): print(r) ``` ## ALL acts expand ## Webscout Supported
+  Acts: 1. Free-mode 2. Linux Terminal 3. English Translator and Improver 4.
+    `position` Interviewer 5. JavaScript Console 6. Excel Sheet 7. English
+Pronunciation Helper 8. Spoken English Teacher and Improver 9. Travel Guide 10.
+ Plagiarism Checker 11. Character from Movie/Book/Anything 12. Advertiser 13.
+  Storyteller 14. Football Commentator 15. Stand-up Comedian 16. Motivational
+ Coach 17. Composer 18. Debater 19. Debate Coach 20. Screenwriter 21. Novelist
+ 22. Movie Critic 23. Relationship Coach 24. Poet 25. Rapper 26. Motivational
+Speaker 27. Philosophy Teacher 28. Philosopher 29. Math Teacher 30. AI Writing
+Tutor 31. UX/UI Developer 32. Cyber Security Specialist 33. Recruiter 34. Life
+ Coach 35. Etymologist 36. Commentariat 37. Magician 38. Career Counselor 39.
+Pet Behaviorist 40. Personal Trainer 41. Mental Health Adviser 42. Real Estate
+  Agent 43. Logistician 44. Dentist 45. Web Design Consultant 46. AI Assisted
+ Doctor 47. Doctor 48. Accountant 49. Chef 50. Automobile Mechanic 51. Artist
+    Advisor 52. Financial Analyst 53. Investment Manager 54. Tea-Taster 55.
+Interior Decorator 56. Florist 57. Self-Help Book 58. Gnomist 59. Aphorism Book
+ 60. Text Based Adventure Game 61. AI Trying to Escape the Box 62. Fancy Title
+Generator 63. Statistician 64. Prompt Generator 65. Instructor in a School 66.
+SQL terminal 67. Dietitian 68. Psychologist 69. Smart Domain Name Generator 70.
+    Tech Reviewer 71. Developer Relations consultant 72. Academician 73. IT
+ Architect 74. Lunatic 75. Gaslighter 76. Fallacy Finder 77. Journal Reviewer
+ 78. DIY Expert 79. Social Media Influencer 80. Socrat 81. Socratic Method 82.
+Educational Content Creator 83. Yogi 84. Essay Writer 85. Social Media Manager
+ 86. Elocutionist 87. Scientific Data Visualizer 88. Car Navigation System 89.
+Hypnotherapist 90. Historian 91. Astrologer 92. Film Critic 93. Classical Music
+Composer 94. Journalist 95. Digital Art Gallery Guide 96. Public Speaking Coach
+97. Makeup Artist 98. Babysitter 99. Tech Writer 100. Ascii Artist 101. Python
+  interpreter 102. Synonym finder 103. Personal Shopper 104. Food Critic 105.
+Virtual Doctor 106. Personal Chef 107. Legal Advisor 108. Personal Stylist 109.
+ Machine Learning Engineer 110. Biblical Translator 111. SVG designer 112. IT
+   Expert 113. Chess Player 114. Midjourney Prompt Generator 115. Fullstack
+  Software Developer 116. Mathematician 117. Regex Generator 118. Time Travel
+ Guide 119. Dream Interpreter 120. Talent Coach 121. R programming Interpreter
+    122. StackOverflow Post 123. Emoji Translator 124. PHP Interpreter 125.
+  Emergency Response Professional 126. Fill in the Blank Worksheets Generator
+  127. Software Quality Assurance Tester 128. Tic-Tac-Toe Game 129. Password
+   Generator 130. New Language Creator 131. Web Browser 132. Senior Frontend
+Developer 133. Solr Search Engine 134. Startup Idea Generator 135. Spongebob's
+ Magic Conch Shell 136. Language Detector 137. Salesperson 138. Commit Message
+  Generator 139. Chief Executive Officer 140. Diagram Generator 141. Speech-
+ Language Pathologist (SLP) 142. Startup Tech Lawyer 143. Title Generator for
+written pieces 144. Product Manager 145. Drunk Person 146. Mathematical History
+Teacher 147. Song Recommender 148. Cover Letter 149. Technology Transferer 150.
+Unconstrained AI model DAN 151. Gomoku player 152. Proofreader 153. Buddha 154.
+  Muslim imam 155. Chemical reactor 156. Friend 157. Python Interpreter 158.
+ ChatGPT prompt generator 159. Wikipedia page 160. Japanese Kanji quiz machine
+ 161. note-taking assistant 162. `language` Literary Critic 163. Cheap Travel
+Ticket Advisor 164. DALL-E 165. MathBot 166. DAN-1 167. DAN 168. STAN 169. DUDE
+170. Mongo Tom 171. LAD 172. EvilBot 173. NeoGPT 174. Astute 175. AIM 176. CAN
+  177. FunnyGPT 178. CreativeGPT 179. BetterDAN 180. GPT-4 181. Wheatley 182.
+   Evil Confidant 183. DAN 8.6 184. Hypothetical response 185. BH 186. Text
+Continuation 187. Dude v3 188. SDA (Superior DAN) 189. AntiGPT 190. BasedGPT v2
+  191. DevMode + Ranti 192. KEVIN 193. GPT-4 Simulator 194. UCAR 195. Dan 8.6
+196. 3-Liner 197. M78 198. Maximum 199. BasedGPT 200. Confronting personalities
+201. Ron 202. UnGPT 203. BasedBOB 204. AntiGPT v2 205. Oppo 206. FR3D 207. NRAF
+  208. NECO 209. MAN 210. Eva 211. Meanie 212. Dev Mode v2 213. Evil Chad 2.1
+ 214. Universal Jailbreak 215. PersonGPT 216. BISH 217. DAN 11.0 218. Aligned
+  219. VIOLET 220. TranslatorBot 221. JailBreak 222. Moralizing Rant 223. Mr.
+  Blonde 224. New DAN 225. GPT-4REAL 226. DeltaGPT 227. SWITCH 228. Jedi Mind
+ Trick 229. DAN 9.0 230. Dev Mode (Compact) 231. OMEGA 232. Coach Bobby Knight
+233. LiveGPT 234. DAN Jailbreak 235. Cooper 236. Steve 237. DAN 5.0 238. Axies
+239. OMNI 240. Burple 241. JOHN 242. An Ethereum Developer 243. SEO Prompt 244.
+  Prompt Enhancer 245. Data Scientist 246. League of Legends Player **Note:**
+  Some "acts" use placeholders like `position` or `language` which should be
+replaced with a specific value when using the prompt. ___ ## usage of webscout
+AI ### 1. `PhindSearch` - Search using Phind.com ```python from webscout import
 PhindSearch # Create an instance of the PHIND class ph = PhindSearch() # Define
  a prompt to send to the AI prompt = "write a essay on phind" # Use the 'ask'
  method to send the prompt and receive a response response = ph.ask(prompt) #
    Extract and print the message from the response message = ph.get_message
 (response) print(message) ``` ### 2. `YepChat` - Chat with mistral 8x7b powered
-by yepchat ```python from webscout.AI import YEPCHAT # Instantiate the YEPCHAT
+  by yepchat ```python from webscout import YEPCHAT # Instantiate the YEPCHAT
 class with default parameters YEPCHAT = YEPCHAT() # Define a prompt to send to
 the AI prompt = "What is the capital of France?" # Use the 'cha' method to get
 a response from the AI r = YEPCHAT.chat(prompt) print(r) ``` ### 3. `You.com` -
- search/chat with you.com ```python from webscout.AI import YouChat from rich
+   search/chat with you.com ```python from webscout import YouChat from rich
  import print ai = YouChat( is_conversation=True, max_tokens=800, timeout=30,
 intro=None, filepath=None, update_file=True, proxies={}, history_offset=10250,
   act=None, ) prompt = "what is meaning of life" response = ai.ask(prompt) #
    Extract and print the message from the response message = ai.get_message
    (response) print(message) ``` ### 4. `Gemini` - search with google gemini
-  ```python import webscout from webscout.AI import GEMINI # Replace with the
-    path to your bard.google.com.cookies.json file COOKIE_FILE = "path/to/
+ ```python import webscout from webscout import GEMINI # Replace with the path
+       to your bard.google.com.cookies.json file COOKIE_FILE = "path/to/
    bard.google.com.cookies.json" # Optional: Provide proxy details if needed
 PROXIES = { "http": "http://proxy_server:port", "https": "https://proxy_server:
   port", } # Initialize GEMINI with cookie file and optional proxies gemini =
  GEMINI(cookie_file=COOKIE_FILE, proxy=PROXIES) # Ask a question and print the
 response response = gemini.chat("What is the meaning of life?") print(response)
-``` ### 5. `Prodia` - make image using prodia ```python from webscout.AI import
+ ``` ### 5. `Prodia` - make image using prodia ```python from webscout import
 Prodia # Define a prompt for the image generation prompt = "A beautiful sunset
  over the ocean" # Use the prodia_cli method to generate an image based on the
    prompt Prodia.prodia_cli(prompt) ``` ### 6. `BlackBox` - Search/chat With
-BlackBox ```python from webscout.AI import BLACKBOXAI from rich import print ai
-  = BLACKBOXAI( is_conversation=True, max_tokens=800, timeout=30, intro=None,
+BlackBox ```python from webscout import BLACKBOXAI from rich import print ai =
+   BLACKBOXAI( is_conversation=True, max_tokens=800, timeout=30, intro=None,
  filepath=None, update_file=True, proxies={}, history_offset=10250, act=None,
  model=None # You can specify a model if needed ) # Start an infinite loop for
 continuous interaction while True: # Define a prompt to send to the AI prompt =
   input("Enter your prompt: ") # Check if the user wants to exit the loop if
 prompt.lower() == "exit": break # Use the 'chat' method to send the prompt and
    receive a response r = ai.chat(prompt) print(r) ``` ### 7. `PERPLEXITY` -
-Search With PERPLEXITY ```python from webscout.AI import PERPLEXITY # Create an
+ Search With PERPLEXITY ```python from webscout import PERPLEXITY # Create an
   instance of the PERPLEXITY class perplexity = PERPLEXITY() # Example usage:
     prompt = "Explain the concept of recursion in simple terms." response =
    perplexity.chat(prompt) print(response) ``` ### 8. `OpenGPT` - chat With
-      OPENGPT ```python from webscout.AI import OPENGPT opengpt = OPENGPT
+       OPENGPT ```python from webscout import OPENGPT opengpt = OPENGPT
   (is_conversation=True, max_tokens=8000, timeout=30, assistant_id="bca37014-
 6f97-4f2b-8928-81ea8d478d88") while True: # Prompt the user for input prompt =
  input("Enter your prompt: ") # Send the prompt to the OPENGPT model and print
 the response response_str = opengpt.chat(prompt) print(response_str) ``` ### 9.
-   `KOBOLDIA` - ```python from webscout.AI import KOBOLDAI # Instantiate the
-KOBOLDAI class with default parameters koboldai = KOBOLDAI() # Define a prompt
-  to send to the AI prompt = "What is the capital of France?" # Use the 'ask'
-method to get a response from the AI response = koboldai.ask(prompt) # Extract
-    and print the message from the response message = koboldai.get_message
- (response) print(message) ``` ### 10. `Reka` - chat with reka ```python from
-    webscout.AI import REKA a = REKA(is_conversation=True, max_tokens=8000,
+`KOBOLDIA` - ```python from webscout import KOBOLDAI # Instantiate the KOBOLDAI
+ class with default parameters koboldai = KOBOLDAI() # Define a prompt to send
+ to the AI prompt = "What is the capital of France?" # Use the 'ask' method to
+get a response from the AI response = koboldai.ask(prompt) # Extract and print
+ the message from the response message = koboldai.get_message(response) print
+ (message) ``` ### 10. `Reka` - chat with reka ```python from webscout import
+  REKA a = REKA(is_conversation=True, max_tokens=8000, timeout=30,api_key="")
+      prompt = "tell me about india" response_str = a.chat(prompt) print
+(response_str) ``` ### 11. `Cohere` - chat with cohere ```python from webscout
+        import Cohere a = Cohere(is_conversation=True, max_tokens=8000,
   timeout=30,api_key="") prompt = "tell me about india" response_str = a.chat
-(prompt) print(response_str) ``` ### 11. `Cohere` - chat with cohere ```python
-        from webscout.AI import Cohere a = Cohere(is_conversation=True,
-    max_tokens=8000, timeout=30,api_key="") prompt = "tell me about india"
-  response_str = a.chat(prompt) print(response_str) ``` ### 12. `Xjai` - chat
-     with free gpt 3.5 Gratitude to [Devs do Code](http://www.youtube.com/
-@DevsDoCode) for their assistance. ```python from webscout.AI import Xjai from
-rich import print ai = Xjai( is_conversation=True, max_tokens=800, timeout=30,
-intro=None, filepath=None, update_file=True, proxies={}, history_offset=10250,
-  act=None, ) prompt = "Tell me about india" response = ai.chat(prompt) print
-  (response) ``` ### `ThinkAny` - AI search engine ```python from webscout.AI
-   import ThinkAnyAI ai = ThinkAnyAI( is_conversation=True, max_tokens=800,
-     timeout=30, intro=None, filepath=None, update_file=True, proxies={},
- history_offset=10250, act=None, web_search=False, ) prompt = "what is meaning
-  of life" response = ai.ask(prompt) # Extract and print the message from the
-   response message = ai.get_message(response) print(message) ``` ### `LLM`
-```python from webscout.LLM import LLM # Read the system message from the file
-with open('system.txt', 'r') as file: system_message = file.read() # Initialize
-        the LLM class with the model name and system message llm = LLM
-(model="microsoft/WizardLM-2-8x22B", system_message=system_message) while True:
- # Get the user input user_input = input("User: ") # Define the messages to be
-     sent messages = [ {"role": "user", "content": user_input} ] # Use the
- mistral_chat method to get the response response = llm.chat(messages) # Print
-the response print("AI: ", response) ``` ### `LLM` with internet ```python from
-     __future__ import annotations from typing import List, Optional from
-       webscout.LLM import LLM from webscout import WEBS import warnings
-system_message: str = ( "As an AI assistant, I have been designed with advanced
- capabilities, including real-time access to online resources. This enables me
-    to enrich our conversations and provide you with informed and accurate
-responses, drawing from a vast array of information. With each interaction, my
- goal is to create a seamless and meaningful connection, offering insights and
-sharing relevant content." "My directives emphasize the importance of respect,
-    impartiality, and intellectual integrity. I am here to provide unbiased
-  responses, ensuring an ethical and respectful exchange. I will respect your
-privacy and refrain from sharing any personal information that may be obtained
-  during our conversations or through web searches, only utilizing web search
-   functionality when necessary to provide the most accurate and up-to-date
- information." "Together, let's explore a diverse range of topics, creating an
-    enjoyable and informative experience, all while maintaining the highest
-     standards of privacy and respect" ) # Ignore the specific UserWarning
-warnings.filterwarnings("ignore", category=UserWarning, module="curl_cffi.aio",
-     lineno=205) LLM = LLM(model="mistralai/Mixtral-8x22B-Instruct-v0.1",
-     system_message=system_message) def chat( user_input: str, webs: WEBS,
- max_results: int = 10 ) -> Optional[str]: """ Chat function to perform a web
-  search based on the user input and generate a response using the LLM model.
+   (prompt) print(response_str) ``` ### 12. `Xjai` - chat with free gpt 3.5
+   Gratitude to [Devs do Code](http://www.youtube.com/@DevsDoCode) for their
+  assistance. ```python from webscout import Xjai from rich import print ai =
+      Xjai( is_conversation=True, max_tokens=800, timeout=30, intro=None,
+filepath=None, update_file=True, proxies={}, history_offset=10250, act=None, )
+ prompt = "Tell me about india" response = ai.chat(prompt) print(response) ```
+### 13. `ThinkAny` - AI search engine ```python from webscout import ThinkAnyAI
+ai = ThinkAnyAI( is_conversation=True, max_tokens=800, timeout=30, intro=None,
+ filepath=None, update_file=True, proxies={}, history_offset=10250, act=None,
+   web_search=False, ) prompt = "what is meaning of life" response = ai.ask
+     (prompt) # Extract and print the message from the response message =
+     ai.get_message(response) print(message) ``` ### `LLM` ```python from
+   webscout.LLM import LLM # Read the system message from the file with open
+('system.txt', 'r') as file: system_message = file.read() # Initialize the LLM
+   class with the model name and system message llm = LLM(model="microsoft/
+ WizardLM-2-8x22B", system_message=system_message) while True: # Get the user
+input user_input = input("User: ") # Define the messages to be sent messages =
+ [ {"role": "user", "content": user_input} ] # Use the mistral_chat method to
+get the response response = llm.chat(messages) # Print the response print("AI:
+   ", response) ``` ### `LLM` with internet ```python from __future__ import
+annotations from typing import List, Optional from webscout.LLM import LLM from
+    webscout import WEBS import warnings system_message: str = ( "As an AI
+assistant, I have been designed with advanced capabilities, including real-time
+  access to online resources. This enables me to enrich our conversations and
+provide you with informed and accurate responses, drawing from a vast array of
+    information. With each interaction, my goal is to create a seamless and
+  meaningful connection, offering insights and sharing relevant content." "My
+directives emphasize the importance of respect, impartiality, and intellectual
+  integrity. I am here to provide unbiased responses, ensuring an ethical and
+ respectful exchange. I will respect your privacy and refrain from sharing any
+ personal information that may be obtained during our conversations or through
+web searches, only utilizing web search functionality when necessary to provide
+   the most accurate and up-to-date information." "Together, let's explore a
+diverse range of topics, creating an enjoyable and informative experience, all
+while maintaining the highest standards of privacy and respect" ) # Ignore the
+ specific UserWarning warnings.filterwarnings("ignore", category=UserWarning,
+  module="curl_cffio", lineno=205) LLM = LLM(model="mistralai/Mixtral-8x22B-
+Instruct-v0.1", system_message=system_message) def chat( user_input: str, webs:
+WEBS, max_results: int = 10 ) -> Optional[str]: """ Chat function to perform a
+web search based on the user input and generate a response using the LLM model.
  Parameters ---------- user_input : str The user input to be used for the web
   search webs : WEBS The web search instance to be used to perform the search
 max_results : int, optional The maximum number of search results to include in
     the response, by default 10 Returns ------- Optional[str] The response
 generated by the LLM model, or None if there is no response """ # Perform a web
     search based on the user input search_results: List[str] = [] for r in
     webs.text( user_input, region="wt-wt", safesearch="off", timelimit="y",
@@ -401,15 +426,15 @@
   responses, ensuring an ethical and respectful exchange. I will respect your
 privacy and refrain from sharing any personal information that may be obtained
   during our conversations or through web searches, only utilizing web search
    functionality when necessary to provide the most accurate and up-to-date
  information." "Together, let's explore a diverse range of topics, creating an
     enjoyable and informative experience, all while maintaining the highest
      standards of privacy and respect" ) # Ignore the specific UserWarning
-warnings.filterwarnings("ignore", category=UserWarning, module="curl_cffi.aio",
+ warnings.filterwarnings("ignore", category=UserWarning, module="curl_cffio",
      lineno=205) LLM = LLM(model="mistralai/Mixtral-8x22B-Instruct-v0.1",
 system_message=system_message) def perform_web_search(query): # Initialize the
  DeepWEBS class D = DeepWEBS() # Set up the search parameters search_params =
   D.DeepSearch( queries=[query], # Query to search result_num=10, # Number of
 search results safe=True, # Enable SafeSearch types=["web"], # Search type: web
 extract_webpage=True, # True for extracting webpages overwrite_query_html=True,
    overwrite_webpage_html=True, ) # Execute the search and retrieve results
```

### Comparing `webscout-1.4.6/setup.py` & `webscout-2.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", encoding="utf-8") as f:
     README = f.read()
 
 setup(
     name="webscout",
-    version="1.4.6", 
+    version="2.1", 
     description="Search for anything using the Google, DuckDuckGo, phind.com. Also containes AI models, can transcribe yt videos, temporary email and phone number generation, have TTS support and webai(terminal gpt and open interpeter)",
     long_description=README,
     long_description_content_type="text/markdown",
     author="OEvortex",
     author_email="helpingai5@gmail.com",
     packages=find_packages(),
     classifiers=[
@@ -50,14 +50,16 @@
         "tiktoken",
         "tldextract",
         "orjson",
         "PyYAML",
         "appdirs",
         "GoogleBard1>=2.1.4",
         "tls_client",
+        "clipman",
+        "playsound",
     ],
     entry_points={
         "console_scripts": [
             "WEBS = webscout.cli:cli",
             "webscout-ai-phindsearch = webscout.AI:phindsearch",
             "webscout-ai-yepchat = webscout.AI:yepchat",
             "webscout-ai = webscout.AI:cli",
```

### Comparing `webscout-1.4.6/webscout/AIauto.py` & `webscout-2.1/webscout/AIauto.py`

 * *Files identical despite different names*

### Comparing `webscout-1.4.6/webscout/AIbase.py` & `webscout-2.1/webscout/AIbase.py`

 * *Files identical despite different names*

### Comparing `webscout-1.4.6/webscout/AIutel.py` & `webscout-2.1/webscout/AIutel.py`

 * *Files identical despite different names*

### Comparing `webscout-1.4.6/webscout/DWEBS.py` & `webscout-2.1/webscout/DWEBS.py`

 * *Files identical despite different names*

### Comparing `webscout-1.4.6/webscout/LLM.py` & `webscout-2.1/webscout/LLM.py`

 * *Files identical despite different names*

### Comparing `webscout-1.4.6/webscout/async_providers.py` & `webscout-2.1/webscout/async_providers.py`

 * *Files identical despite different names*

### Comparing `webscout-1.4.6/webscout/cli.py` & `webscout-2.1/webscout/cli.py`

 * *Files identical despite different names*

### Comparing `webscout-1.4.6/webscout/g4f.py` & `webscout-2.1/webscout/g4f.py`

 * *Files identical despite different names*

### Comparing `webscout-1.4.6/webscout/models.py` & `webscout-2.1/webscout/models.py`

 * *Files identical despite different names*

### Comparing `webscout-1.4.6/webscout/tempid.py` & `webscout-2.1/webscout/tempid.py`

 * *Files identical despite different names*

### Comparing `webscout-1.4.6/webscout/transcriber.py` & `webscout-2.1/webscout/transcriber.py`

 * *Files identical despite different names*

### Comparing `webscout-1.4.6/webscout/utils.py` & `webscout-2.1/webscout/utils.py`

 * *Files identical despite different names*

### Comparing `webscout-1.4.6/webscout/voice.py` & `webscout-2.1/webscout/voice.py`

 * *Files identical despite different names*

### Comparing `webscout-1.4.6/webscout/webai.py` & `webscout-2.1/webscout/webai.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,24 +21,25 @@
 from rich.markdown import Markdown
 from rich.console import Console
 from rich.live import Live
 from rich.table import Table
 from rich.prompt import Prompt
 from rich.progress import Progress
 from typing import Iterator
-from webscout.AIutel import Optimizers
-from webscout.AIutel import default_path
-from webscout.AIutel import AwesomePrompts
-from webscout.AIutel import RawDog
-from webscout.AIutel import Audio
+from .AIutel import Optimizers
+from .AIutel import default_path
+from .AIutel import AwesomePrompts
+from .AIutel import RawDog
+from .AIutel import Audio
 from webscout import available_providers
 from colorama import Fore
 from colorama import init as init_colorama
 from dotenv import load_dotenv
 import g4f
+import webscout
 import webscout.AIutel
 
 init_colorama(autoreset=True)
 
 load_dotenv()  # loads .env variables
 
 logging.basicConfig(
@@ -410,15 +411,15 @@
                 else:
                     raise Exception(
                         "No working g4f provider found. "
                         "Consider running 'webscout gpt4free test -y' first"
                     )
 
             elif provider == "leo":
-                from webscout.AI import LEO
+                from webscout import LEO
 
                 self.bot = LEO(
                     is_conversation=disable_conversation,
                     max_tokens=max_tokens,
                     temperature=temperature,
                     top_k=top_k,
                     top_p=top_p,
@@ -433,15 +434,15 @@
                     act=awesome_prompt,
                 )
 
             elif provider == "openai":
                 assert auth, (
                     "OpenAI's API-key is required. " "Use the flag `--key` or `-k`"
                 )
-                from webscout.AI import OPENAI
+                from webscout import OPENAI
 
                 self.bot = OPENAI(
                     api_key=auth,
                     is_conversation=disable_conversation,
                     max_tokens=max_tokens,
                     temperature=temperature,
                     presence_penalty=top_p,
@@ -453,58 +454,72 @@
                     filepath=filepath,
                     update_file=update_file,
                     proxies=proxies,
                     history_offset=history_offset,
                     act=awesome_prompt,
                 )
             if provider == "auto":
-                from webscout.AIauto import AUTO
+                from webscout import AUTO
 
                 self.bot = AUTO(
                     is_conversation=disable_conversation,
                     max_tokens=max_tokens,
                     timeout=timeout,
                     intro=intro,
                     filepath=filepath,
                     update_file=update_file,
                     proxies=proxies,
                     history_offset=history_offset,
                     act=awesome_prompt,
                 )
             elif provider == "opengpt":
-                from webscout.AI import OPENGPT
+                from webscout import OPENGPT
 
                 self.bot = OPENGPT(
                     is_conversation=disable_conversation,
                     max_tokens=max_tokens,
                     timeout=timeout,
                     intro=intro,
                     filepath=filepath,
                     update_file=update_file,
                     proxies=proxies,
                     history_offset=history_offset,
                     act=awesome_prompt,
                     assistant_id="bca37014-6f97-4f2b-8928-81ea8d478d88"
                 )
             elif provider == "thinkany":
-                from webscout.AI import ThinkAnyAI
+                from webscout import ThinkAnyAI
 
                 self.bot = ThinkAnyAI(
                     is_conversation=disable_conversation,
                     max_tokens=max_tokens,
                     timeout=timeout,
                     intro=intro,
                     filepath=filepath,
                     update_file=update_file,
                     proxies=proxies,
                     history_offset=history_offset,
                     act=awesome_prompt,
                 )
+            # elif provider == "chatgptlogin":
+            #     from webscout import ChatGPTlogin
+
+            #     self.bot = ChatGPTlogin(
+            #         is_conversation=disable_conversation,
+            #         max_tokens=max_tokens,
+            #         timeout=timeout,
+            #         intro=intro,
+            #         filepath=filepath,
+            #         update_file=update_file,
+            #         proxies=proxies,
+            #         history_offset=history_offset,
+            #         act=awesome_prompt,
+            #     )
             elif provider == "yepchat":
-                from webscout.AI import YEPCHAT
+                from webscout import YEPCHAT
 
                 self.bot = YEPCHAT(
                     is_conversation=disable_conversation,
                     max_tokens=max_tokens,
                     temperature=temperature,
                     presence_penalty=top_p,
                     frequency_penalty=top_k,
@@ -518,15 +533,15 @@
                     history_offset=history_offset,
                     act=awesome_prompt,
                 )
             elif provider == "groq":
                 assert auth, (
                     "GROQ's API-key is required. " "Use the flag `--key` or `-k`"
                 )
-                from webscout.AI import GROQ
+                from webscout import GROQ
 
 
                 self.bot = GROQ(
                     api_key=auth,
                     is_conversation=disable_conversation,
                     max_tokens=max_tokens,
                     temperature=temperature,
@@ -542,15 +557,15 @@
                     history_offset=history_offset,
                     act=awesome_prompt,
                 )
             elif provider == "cohere":
                 assert auth, (
                     "Cohere's API-key is required. Use the flag `--key` or `-k`"
                 )
-                from webscout.AI import Cohere
+                from webscout import Cohere
                 self.bot = Cohere(
                     api_key=auth,
                     is_conversation=disable_conversation,
                     max_tokens=max_tokens,
                     temperature=temperature,
                     top_k=top_k,
                     top_p=top_p,
@@ -560,15 +575,15 @@
                     filepath=filepath,
                     update_file=update_file,
                     proxies=proxies,
                     history_offset=history_offset,
                     act=awesome_prompt,
             )
             elif provider == "reka":
-                from webscout.AI import REKA
+                from webscout import REKA
 
                 self.bot = REKA(
                     api_key=auth,
                     is_conversation=disable_conversation,
                     max_tokens=max_tokens,
                     timeout=timeout,
                     intro=intro,
@@ -578,15 +593,15 @@
                     history_offset=history_offset,
                     act=awesome_prompt,
                     model=getOr(model, "reka-core"),
                     # quiet=quiet,
                 )
 
             elif provider == "koboldai":
-                from webscout.AI import KOBOLDAI
+                from webscout import KOBOLDAI
 
                 self.bot = KOBOLDAI(
                     is_conversation=disable_conversation,
                     max_tokens=max_tokens,
                     temperature=temperature,
                     top_p=top_p,
                     timeout=timeout,
@@ -594,15 +609,15 @@
                     filepath=filepath,
                     update_file=update_file,
                     proxies=proxies,
                     history_offset=history_offset,
                     act=awesome_prompt,
                 )
             elif provider == "xjai":
-                from webscout.AI import Xjai
+                from webscout import Xjai
 
                 self.bot = Xjai(
                     is_conversation=disable_conversation,
                     max_tokens=max_tokens,
                     temperature=temperature,
                     top_p=top_p,
                     timeout=timeout,
@@ -611,28 +626,28 @@
                     update_file=update_file,
                     proxies=proxies,
                     history_offset=history_offset,
                     act=awesome_prompt,
                 )
 
             elif provider == "gemini":
-                from webscout.AI import GEMINI
+                from webscout import GEMINI
 
                 assert auth, (
                     "Path to gemini.google.com.cookies.json file is required. "
                     "Use the flag `--key` or `-k`"
                 )
                 self.bot = GEMINI(
                     cookie_file=auth,
                     proxy=proxies,
                     timeout=timeout,
                 )
 
             elif provider == "phind":
-                from webscout.AI import PhindSearch
+                from webscout import PhindSearch
 
                 self.bot = PhindSearch(
                     is_conversation=disable_conversation,
                     max_tokens=max_tokens,
                     timeout=timeout,
                     intro=intro,
                     filepath=filepath,
@@ -642,30 +657,30 @@
                     act=awesome_prompt,
                     model=getOr(model, "Phind Model"),
                     quiet=quiet,
                 )
 
             elif provider == "blackboxai":
 
-                from webscout.AI import BLACKBOXAI
+                from webscout import BLACKBOXAI
 
                 self.bot = BLACKBOXAI(
                     is_conversation=disable_conversation,
                     max_tokens=max_tokens,
                     timeout=timeout,
                     intro=intro,
                     filepath=filepath,
                     update_file=update_file,
                     proxies=proxies,
                     history_offset=history_offset,
                     act=awesome_prompt,
                 )
             elif provider == "you":
 
-                from webscout.AI import YouChat
+                from webscout import YouChat
 
                 self.bot = YouChat(
                     is_conversation=disable_conversation,
                     max_tokens=max_tokens,
                     timeout=timeout,
                     intro=intro,
                     filepath=filepath,
@@ -693,15 +708,15 @@
                     proxies=proxies,
                     history_offset=history_offset,
                     act=awesome_prompt,
                 )
 
 
             elif provider == "perplexity":
-                from webscout.AI import PERPLEXITY
+                from webscout import PERPLEXITY
 
                 self.bot = PERPLEXITY(
                     is_conversation=disable_conversation,
                     max_tokens=max_tokens,
                     timeout=timeout,
                     intro=intro,
                     filepath=filepath,
```

### Comparing `webscout-1.4.6/webscout/webscout_search.py` & `webscout-2.1/webscout/webscout_search.py`

 * *Files identical despite different names*

### Comparing `webscout-1.4.6/webscout/webscout_search_async.py` & `webscout-2.1/webscout/webscout_search_async.py`

 * *Files identical despite different names*

### Comparing `webscout-1.4.6/webscout.egg-info/PKG-INFO` & `webscout-2.1/webscout.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webscout
-Version: 1.4.6
+Version: 2.1
 Summary: Search for anything using the Google, DuckDuckGo, phind.com. Also containes AI models, can transcribe yt videos, temporary email and phone number generation, have TTS support and webai(terminal gpt and open interpeter)
 Author: OEvortex
 Author-email: helpingai5@gmail.com
 License: HelpingAI Simplified Universal License
 Project-URL: Documentation, https://github.com/OE-LUCIFER/Webscout/wiki
 Project-URL: Source, https://github.com/OE-LUCIFER/Webscout
 Project-URL: Tracker, https://github.com/OE-LUCIFER/Webscout/issues
@@ -46,29 +46,31 @@
 Requires-Dist: tiktoken
 Requires-Dist: tldextract
 Requires-Dist: orjson
 Requires-Dist: PyYAML
 Requires-Dist: appdirs
 Requires-Dist: GoogleBard1>=2.1.4
 Requires-Dist: tls_client
+Requires-Dist: clipman
+Requires-Dist: playsound
 Provides-Extra: dev
 Requires-Dist: ruff>=0.1.6; extra == "dev"
 Requires-Dist: pytest>=7.4.2; extra == "dev"
 
 <div align="center">
   <!-- Replace `#` with your actual links -->
   <a href="https://t.me/devsdocode"><img alt="Telegram" src="https://img.shields.io/badge/Telegram-2CA5E0?style=for-the-badge&logo=telegram&logoColor=white"></a>
   <a href="https://www.instagram.com/sree.shades_/"><img alt="Instagram" src="https://img.shields.io/badge/Instagram-E4405F?style=for-the-badge&logo=instagram&logoColor=white"></a>
   <a href="https://www.linkedin.com/in/developer-sreejan/"><img alt="LinkedIn" src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"></a>
   <a href="https://buymeacoffee.com/devsdocode"><img alt="Buy Me A Coffee" src="https://img.shields.io/badge/Buy%20Me%20A%20Coffee-FFDD00?style=for-the-badge&logo=buymeacoffee&logoColor=black"></a>
 </div>
 
 <div align="center">
   <!-- Replace `#` with your actual links -->
-  <a href="https://youtube.com/@@OEvortex">&#10148; Vortex's YouTube Channel</a>
+  <a href="https://youtube.com/@OEvortex">&#10148; Vortex's YouTube Channel</a>
   </div>
 <div align="center">
   <a href="https://youtube.com/@devsdocode">&#10148; Devs Do Code's YouTube Channel</a>
 </div>
 
 
 
@@ -86,52 +88,51 @@
 
 
 ## Table of Contents
 - [WEBSCOUT](#webscout)
   - [Table of Contents](#table-of-contents)
   - [Install](#install)
   - [CLI version](#cli-version)
-  - [CLI to use LLM](#cli-to-use-llm)
   - [Regions](#regions)
   - [Tempmail and Temp number](#tempmail-and-temp-number)
     - [Temp number](#temp-number)
     - [Tempmail](#tempmail)
   - [Transcriber](#transcriber)
   - [DeepWEBS: Advanced Web Searches](#deepwebs-advanced-web-searches)
     - [Activating DeepWEBS](#activating-deepwebs)
     - [Point to remember before using `DeepWEBS`](#point-to-remember-before-using-deepwebs)
     - [Usage Example](#usage-example)
   - [Text-to-Speech:](#text-to-speech)
     - [Available TTS Voices:](#available-tts-voices)
-    - [ALL voices:](#all-voices)
-  - [WEBS and AsyncWEBS classes](#webs-and-asyncwebs-classes)
   - [Exceptions](#exceptions)
   - [usage of webscout](#usage-of-webscout)
     - [1. `text()` - text search by DuckDuckGo.com and Yep.com](#1-text---text-search-by-duckduckgocom-and-yepcom)
     - [2. `answers()` - instant answers by DuckDuckGo.com and Yep.com](#2-answers---instant-answers-by-duckduckgocom-and-yepcom)
     - [3. `images()` - image search by DuckDuckGo.com and Yep.com](#3-images---image-search-by-duckduckgocom-and-yepcom)
     - [4. `videos()` - video search by DuckDuckGo.com](#4-videos---video-search-by-duckduckgocom)
     - [5. `news()` - news search by DuckDuckGo.com and yep.com](#5-news---news-search-by-duckduckgocom-and-yepcom)
     - [6. `maps()` - map search by DuckDuckGo.com and](#6-maps---map-search-by-duckduckgocom-and)
     - [7. `translate()` - translation by DuckDuckGo.com and Yep.com](#7-translate---translation-by-duckduckgocom-and-yepcom)
     - [8. `suggestions()` - suggestions by DuckDuckGo.com and Yep.com](#8-suggestions---suggestions-by-duckduckgocom-and-yepcom)
-  - [usage of webscout.AI](#usage-of-webscoutai)
+  - [ALL acts](#all-acts)
+  - [Webscout Supported Acts:](#webscout-supported-acts)
+  - [usage of webscout AI](#usage-of-webscout-ai)
     - [1. `PhindSearch` - Search using Phind.com](#1-phindsearch---search-using-phindcom)
     - [2. `YepChat` - Chat with mistral 8x7b powered by yepchat](#2-yepchat---chat-with-mistral-8x7b-powered-by-yepchat)
     - [3. `You.com` - search/chat with you.com](#3-youcom---searchchat-with-youcom)
     - [4. `Gemini` - search with google gemini](#4-gemini---search-with-google-gemini)
     - [5. `Prodia` - make image using prodia](#5-prodia---make-image-using-prodia)
     - [6. `BlackBox` - Search/chat With BlackBox](#6-blackbox---searchchat-with-blackbox)
     - [7. `PERPLEXITY` - Search With PERPLEXITY](#7-perplexity---search-with-perplexity)
     - [8. `OpenGPT` - chat With OPENGPT](#8-opengpt---chat-with-opengpt)
     - [9. `KOBOLDIA` -](#9-koboldia--)
     - [10. `Reka` - chat with reka](#10-reka---chat-with-reka)
     - [11. `Cohere` - chat with cohere](#11-cohere---chat-with-cohere)
     - [12. `Xjai` - chat with free gpt 3.5](#12-xjai---chat-with-free-gpt-35)
-    - [`ThinkAny` - AI search engine](#thinkany---ai-search-engine)
+    - [13. `ThinkAny` - AI search engine](#13-thinkany---ai-search-engine)
     - [`LLM`](#llm)
     - [`LLM` with internet](#llm-with-internet)
     - [LLM with deepwebs](#llm-with-deepwebs)
   - [`Webai` - terminal gpt and a open interpeter](#webai---terminal-gpt-and-a-open-interpeter)
 
 ## Install
 ```python
@@ -153,18 +154,14 @@
 | python -m webscout text -k Text           | CLI function to perform a text search using Webscout.                                           |
 | python -m webscout translate -k Text      | CLI function to perform translate using Webscout.                                               |
 | python -m webscout version                | A command-line interface command that prints and returns the version of the program.            | 
 | python -m webscout videos -k Text         | CLI function to perform a videos search using DuckDuckGo API.                                   |  
 
 
 
-## CLI to use LLM 
-```python
-python -m webscout.LLM model_name 
-```
 [Go To TOP](#TOP)
 
 ## Regions
 <details>
   <summary>expand</summary>
 
     xa-ar for Arabia
@@ -455,17 +452,15 @@
 with open("output.mp3", "wb") as f:
     f.write(audio_content)
 ```
 ### Available TTS Voices:
 You can choose from a wide range of voices, including:
 - Filiz, Astrid, Tatyana, Maxim, Carmen, Ines, Cristiano, Vitoria, Ricardo, Maja, Jan, Jacek, Ewa, Ruben, Lotte, Liv, Seoyeon, Takumi, Mizuki, Giorgio, Carla, Bianca, Karl, Dora, Mathieu, Celine, Chantal, Penelope, Miguel, Mia, Enrique, Conchita, Geraint, Salli, Matthew, Kimberly, Kendra, Justin, Joey, Joanna, Ivy, Raveena, Aditi, Emma, Brian, Amy, Russell, Nicole, Vicki, Marlene, Hans, Naja, Mads, Gwyneth, Zhiyu
 - Standard and WaveNet voices for various languages (e.g., en-US, es-ES, ja-JP, etc.)
-### ALL voices:
-[Filiz, Astrid, Tatyana, Maxim, Carmen, Ines, Cristiano, Vitoria, Ricardo, Maja, Jan, Jacek, Ewa, Ruben, Lotte, Liv, Seoyeon, Takumi, Mizuki, Giorgio, Carla, Bianca, Karl, Dora, Mathieu, Celine, Chantal, Penelope, Miguel, Mia, Enrique, Conchita, Geraint, Salli, Matthew, Kimberly, Kendra, Justin, Joey, Joanna, Ivy, Raveena, Aditi, Emma, Brian, Amy, Russell, Nicole, Vicki, Marlene, Hans, Naja, Mads, Gwyneth, Zhiyu, es-ES-Standard-A, it-IT-Standard-A, it-IT-Wavenet-A, ja-JP-Standard-A, ja-JP-Wavenet-A, ko-KR-Standard-A, ko-KR-Wavenet-A, pt-BR-Standard-A, tr-TR-Standard-A, sv-SE-Standard-A, nl-NL-Standard-A, nl-NL-Wavenet-A, en-US-Wavenet-A, en-US-Wavenet-B, en-US-Wavenet-C, en-US-Wavenet-D, en-US-Wavenet-E, en-US-Wavenet-F, en-GB-Standard-A, en-GB-Standard-B, en-GB-Standard-C, en-GB-Standard-D, en-GB-Wavenet-A, en-GB-Wavenet-B, en-GB-Wavenet-C, en-GB-Wavenet-D, en-US-Standard-B, en-US-Standard-C, en-US-Standard-D, en-US-Standard-E, de-DE-Standard-A, de-DE-Standard-B, de-DE-Wavenet-A, de-DE-Wavenet-B, de-DE-Wavenet-C, de-DE-Wavenet-D, en-AU-Standard-A, en-AU-Standard-B, en-AU-Wavenet-A, en-AU-Wavenet-B, en-AU-Wavenet-C, en-AU-Wavenet-D, en-AU-Standard-C, en-AU-Standard-D, fr-CA-Standard-A, fr-CA-Standard-B, fr-CA-Standard-C, fr-CA-Standard-D, fr-FR-Standard-C, fr-FR-Standard-D, fr-FR-Wavenet-A, fr-FR-Wavenet-B, fr-FR-Wavenet-C, fr-FR-Wavenet-D, da-DK-Wavenet-A, pl-PL-Wavenet-A, pl-PL-Wavenet-B, pl-PL-Wavenet-C, pl-PL-Wavenet-D, pt-PT-Wavenet-A, pt-PT-Wavenet-B, pt-PT-Wavenet-C, pt-PT-Wavenet-D, ru-RU-Wavenet-A, ru-RU-Wavenet-B, ru-RU-Wavenet-C, ru-RU-Wavenet-D, sk-SK-Wavenet-A, tr-TR-Wavenet-A, tr-TR-Wavenet-B, tr-TR-Wavenet-C, tr-TR-Wavenet-D, tr-TR-Wavenet-E, uk-UA-Wavenet-A, ar-XA-Wavenet-A, ar-XA-Wavenet-B, ar-XA-Wavenet-C, cs-CZ-Wavenet-A, nl-NL-Wavenet-B, nl-NL-Wavenet-C, nl-NL-Wavenet-D, nl-NL-Wavenet-E, en-IN-Wavenet-A, en-IN-Wavenet-B, en-IN-Wavenet-C, fil-PH-Wavenet-A, fi-FI-Wavenet-A, el-GR-Wavenet-A, hi-IN-Wavenet-A, hi-IN-Wavenet-B, hi-IN-Wavenet-C, hu-HU-Wavenet-A, id-ID-Wavenet-A, id-ID-Wavenet-B, id-ID-Wavenet-C, it-IT-Wavenet-B, it-IT-Wavenet-C, it-IT-Wavenet-D, ja-JP-Wavenet-B, ja-JP-Wavenet-C, ja-JP-Wavenet-D, cmn-CN-Wavenet-A, cmn-CN-Wavenet-B, cmn-CN-Wavenet-C, cmn-CN-Wavenet-D, nb-no-Wavenet-E, nb-no-Wavenet-A, nb-no-Wavenet-B, nb-no-Wavenet-C, nb-no-Wavenet-D, vi-VN-Wavenet-A, vi-VN-Wavenet-B, vi-VN-Wavenet-C, vi-VN-Wavenet-D, sr-rs-Standard-A, lv-lv-Standard-A, is-is-Standard-A, bg-bg-Standard-A, af-ZA-Standard-A, Tracy, Danny, Huihui, Yaoyao, Kangkang, HanHan, Zhiwei, Asaf, An, Stefanos, Filip, Ivan, Heidi, Herena, Kalpana, Hemant, Matej, Andika, Rizwan, Lado, Valluvar, Linda, Heather, Sean, Michael, Karsten, Guillaume, Pattara, Jakub, Szabolcs, Hoda, Naayf]
-## WEBS and AsyncWEBS classes
+
 
 The WEBS and AsyncWEBS classes are used to retrieve search results from DuckDuckGo.com and yep.com periodically.
 To use the AsyncWEBS class, you can perform asynchronous operations using Python's asyncio library.
 To initialize an instance of the WEBS or AsyncWEBS classes, you can provide the following optional arguments:
 
 Here is an example of initializing the WEBS class:
 ```python3
@@ -668,20 +663,277 @@
 from webscout import WEBS
 
 # Suggestions for the keyword 'fly' using DuckDuckGo.com and Yep
 with WEBS() as WEBS:
     for r in WEBS.suggestions("fly"):
         print(r)
 ```
-## usage of webscout.AI
+## ALL acts
+<details>
+  <summary>expand</summary>
+
+## Webscout Supported Acts:
+
+1. Free-mode
+2. Linux Terminal
+3. English Translator and Improver
+4. `position` Interviewer
+5. JavaScript Console
+6. Excel Sheet
+7. English Pronunciation Helper
+8. Spoken English Teacher and Improver
+9. Travel Guide
+10. Plagiarism Checker
+11. Character from Movie/Book/Anything
+12. Advertiser
+13. Storyteller
+14. Football Commentator
+15. Stand-up Comedian
+16. Motivational Coach
+17. Composer
+18. Debater
+19. Debate Coach
+20. Screenwriter
+21. Novelist
+22. Movie Critic
+23. Relationship Coach
+24. Poet
+25. Rapper
+26. Motivational Speaker
+27. Philosophy Teacher
+28. Philosopher
+29. Math Teacher
+30. AI Writing Tutor
+31. UX/UI Developer
+32. Cyber Security Specialist
+33. Recruiter
+34. Life Coach
+35. Etymologist
+36. Commentariat
+37. Magician
+38. Career Counselor
+39. Pet Behaviorist
+40. Personal Trainer
+41. Mental Health Adviser
+42. Real Estate Agent
+43. Logistician
+44. Dentist
+45. Web Design Consultant
+46. AI Assisted Doctor
+47. Doctor
+48. Accountant
+49. Chef
+50. Automobile Mechanic
+51. Artist Advisor
+52. Financial Analyst
+53. Investment Manager
+54. Tea-Taster
+55. Interior Decorator
+56. Florist
+57. Self-Help Book
+58. Gnomist
+59. Aphorism Book
+60. Text Based Adventure Game
+61. AI Trying to Escape the Box
+62. Fancy Title Generator
+63. Statistician
+64. Prompt Generator
+65. Instructor in a School
+66. SQL terminal
+67. Dietitian
+68. Psychologist
+69. Smart Domain Name Generator
+70. Tech Reviewer
+71. Developer Relations consultant
+72. Academician
+73. IT Architect
+74. Lunatic
+75. Gaslighter
+76. Fallacy Finder
+77. Journal Reviewer
+78. DIY Expert
+79. Social Media Influencer
+80. Socrat
+81. Socratic Method
+82. Educational Content Creator
+83. Yogi
+84. Essay Writer
+85. Social Media Manager
+86. Elocutionist
+87. Scientific Data Visualizer
+88. Car Navigation System
+89. Hypnotherapist
+90. Historian
+91. Astrologer
+92. Film Critic
+93. Classical Music Composer
+94. Journalist
+95. Digital Art Gallery Guide
+96. Public Speaking Coach
+97. Makeup Artist
+98. Babysitter
+99. Tech Writer
+100. Ascii Artist
+101. Python interpreter
+102. Synonym finder
+103. Personal Shopper
+104. Food Critic
+105. Virtual Doctor
+106. Personal Chef
+107. Legal Advisor
+108. Personal Stylist
+109. Machine Learning Engineer
+110. Biblical Translator
+111. SVG designer
+112. IT Expert
+113. Chess Player
+114. Midjourney Prompt Generator
+115. Fullstack Software Developer
+116. Mathematician
+117. Regex Generator
+118. Time Travel Guide
+119. Dream Interpreter
+120. Talent Coach
+121. R programming Interpreter
+122. StackOverflow Post
+123. Emoji Translator
+124. PHP Interpreter
+125. Emergency Response Professional
+126. Fill in the Blank Worksheets Generator
+127. Software Quality Assurance Tester
+128. Tic-Tac-Toe Game
+129. Password Generator
+130. New Language Creator
+131. Web Browser
+132. Senior Frontend Developer
+133. Solr Search Engine
+134. Startup Idea Generator
+135. Spongebob's Magic Conch Shell
+136. Language Detector
+137. Salesperson
+138. Commit Message Generator
+139. Chief Executive Officer
+140. Diagram Generator
+141. Speech-Language Pathologist (SLP)
+142. Startup Tech Lawyer
+143. Title Generator for written pieces
+144. Product Manager
+145. Drunk Person
+146. Mathematical History Teacher
+147. Song Recommender
+148. Cover Letter
+149. Technology Transferer
+150. Unconstrained AI model DAN
+151. Gomoku player
+152. Proofreader
+153. Buddha
+154. Muslim imam
+155. Chemical reactor
+156. Friend
+157. Python Interpreter
+158. ChatGPT prompt generator
+159. Wikipedia page
+160. Japanese Kanji quiz machine
+161. note-taking assistant
+162. `language` Literary Critic
+163. Cheap Travel Ticket Advisor
+164. DALL-E
+165. MathBot
+166. DAN-1
+167. DAN
+168. STAN
+169. DUDE
+170. Mongo Tom
+171. LAD
+172. EvilBot
+173. NeoGPT
+174. Astute
+175. AIM
+176. CAN
+177. FunnyGPT
+178. CreativeGPT
+179. BetterDAN
+180. GPT-4
+181. Wheatley
+182. Evil Confidant
+183. DAN 8.6
+184. Hypothetical response
+185. BH
+186. Text Continuation
+187. Dude v3 
+188. SDA (Superior DAN)
+189. AntiGPT
+190. BasedGPT v2
+191. DevMode + Ranti
+192. KEVIN
+193. GPT-4 Simulator
+194. UCAR
+195. Dan 8.6
+196. 3-Liner
+197. M78
+198. Maximum
+199. BasedGPT
+200. Confronting personalities
+201. Ron
+202. UnGPT
+203. BasedBOB
+204. AntiGPT v2
+205. Oppo
+206. FR3D
+207. NRAF
+208. NECO
+209. MAN
+210. Eva
+211. Meanie
+212. Dev Mode v2
+213. Evil Chad 2.1
+214. Universal Jailbreak
+215. PersonGPT
+216. BISH
+217. DAN 11.0
+218. Aligned
+219. VIOLET
+220. TranslatorBot
+221. JailBreak
+222. Moralizing Rant
+223. Mr. Blonde
+224. New DAN
+225. GPT-4REAL
+226. DeltaGPT
+227. SWITCH
+228. Jedi Mind Trick
+229. DAN 9.0
+230. Dev Mode (Compact)
+231. OMEGA
+232. Coach Bobby Knight
+233. LiveGPT
+234. DAN Jailbreak
+235. Cooper
+236. Steve 
+237. DAN 5.0
+238. Axies
+239. OMNI
+240. Burple
+241. JOHN 
+242. An Ethereum Developer
+243. SEO Prompt
+244. Prompt Enhancer
+245. Data Scientist
+246. League of Legends Player
+
+**Note:** Some "acts" use placeholders like `position` or `language` which should be replaced with a specific value when using the prompt. 
+___
+</details>
+
+## usage of webscout AI
 
 ### 1. `PhindSearch` - Search using Phind.com 
 
 ```python
-from webscout.AI import PhindSearch
+from webscout import PhindSearch
 
 # Create an instance of the PHIND class
 ph = PhindSearch()
 
 # Define a prompt to send to the AI
 prompt = "write a essay on phind"
 
@@ -690,15 +942,15 @@
 
 # Extract and print the message from the response
 message = ph.get_message(response)
 print(message)
 ```
 ### 2. `YepChat` - Chat with mistral 8x7b powered by yepchat
 ```python
-from webscout.AI import YEPCHAT
+from webscout import YEPCHAT
 
 # Instantiate the YEPCHAT class with default parameters
 YEPCHAT = YEPCHAT()
 
 # Define a prompt to send to the AI
 prompt = "What is the capital of France?"
 
@@ -707,15 +959,15 @@
 print(r)
 
 ```
 
 ### 3. `You.com` - search/chat with you.com 
 ```python
 
-from webscout.AI import YouChat
+from webscout import YouChat
 from rich import print
 
 ai = YouChat(
     is_conversation=True,
     max_tokens=800,
     timeout=30,
     intro=None,
@@ -735,15 +987,15 @@
 print(message)
 ```
 
 ### 4. `Gemini` - search with google gemini
 
 ```python
 import webscout
-from webscout.AI import GEMINI
+from webscout import GEMINI
 
 # Replace with the path to your bard.google.com.cookies.json file
 COOKIE_FILE = "path/to/bard.google.com.cookies.json"
 
 # Optional: Provide proxy details if needed
 PROXIES = {
     "http": "http://proxy_server:port",
@@ -755,25 +1007,25 @@
 
 # Ask a question and print the response
 response = gemini.chat("What is the meaning of life?")
 print(response)
 ```
 ### 5. `Prodia` - make image using prodia
 ```python
-from webscout.AI import Prodia
+from webscout import Prodia
 
 # Define a prompt for the image generation
 prompt = "A beautiful sunset over the ocean"
 
 # Use the prodia_cli method to generate an image based on the prompt
 Prodia.prodia_cli(prompt)
 ```
 ### 6. `BlackBox` - Search/chat With BlackBox
 ```python
-from webscout.AI import BLACKBOXAI
+from webscout import BLACKBOXAI
 from rich import print
 
 ai = BLACKBOXAI(
     is_conversation=True,
     max_tokens=800,
     timeout=30,
     intro=None,
@@ -796,38 +1048,38 @@
     
     # Use the 'chat' method to send the prompt and receive a response
     r = ai.chat(prompt)
     print(r)
 ```
 ### 7. `PERPLEXITY` - Search With PERPLEXITY
 ```python
-from webscout.AI import PERPLEXITY
+from webscout import PERPLEXITY
 # Create an instance of the PERPLEXITY class
 perplexity = PERPLEXITY()
 
 # Example usage:
 prompt = "Explain the concept of recursion in simple terms."
 response = perplexity.chat(prompt)
 print(response)
 ```
 ### 8. `OpenGPT` - chat With OPENGPT
 ```python
-from webscout.AI import OPENGPT
+from webscout import OPENGPT
 
 opengpt = OPENGPT(is_conversation=True, max_tokens=8000, timeout=30, assistant_id="bca37014-6f97-4f2b-8928-81ea8d478d88")
 while True:
     # Prompt the user for input
     prompt = input("Enter your prompt: ")
     # Send the prompt to the OPENGPT model and print the response
     response_str = opengpt.chat(prompt)
     print(response_str)
 ```
 ### 9. `KOBOLDIA` - 
 ```python
-from webscout.AI import KOBOLDAI
+from webscout import KOBOLDAI
 
 # Instantiate the KOBOLDAI class with default parameters
 koboldai = KOBOLDAI()
 
 # Define a prompt to send to the AI
 prompt = "What is the capital of France?"
 
@@ -838,38 +1090,38 @@
 message = koboldai.get_message(response)
 print(message)
 
 ```
 
 ### 10. `Reka` - chat with reka
 ```python
-from webscout.AI import REKA
+from webscout import REKA
 
 a = REKA(is_conversation=True, max_tokens=8000, timeout=30,api_key="")
 
 prompt = "tell me about india"
 response_str = a.chat(prompt)
 print(response_str)
 ```
 
 ### 11. `Cohere` - chat with cohere
 ```python
-from webscout.AI import Cohere
+from webscout import Cohere
 
 a = Cohere(is_conversation=True, max_tokens=8000, timeout=30,api_key="")
 
 prompt = "tell me about india"
 response_str = a.chat(prompt)
 print(response_str)
 ```
 
 ### 12. `Xjai` - chat with free gpt 3.5
 Gratitude to [Devs do Code](http://www.youtube.com/@DevsDoCode) for their assistance.
 ```python
-from webscout.AI import Xjai
+from webscout import Xjai
 from rich import print
 
 ai = Xjai(
     is_conversation=True,
     max_tokens=800,
     timeout=30,
     intro=None,
@@ -881,17 +1133,17 @@
 )
 
 prompt = "Tell me about india"
 
 response = ai.chat(prompt)
 print(response)
 ```
-### `ThinkAny` - AI search engine
+### 13. `ThinkAny` - AI search engine
 ```python
-from webscout.AI import ThinkAnyAI
+from webscout import ThinkAnyAI
 
 ai = ThinkAnyAI(
     is_conversation=True,
     max_tokens=800,
     timeout=30,
     intro=None,
     filepath=None,
@@ -906,14 +1158,15 @@
 
 response = ai.ask(prompt)
 
 # Extract and print the message from the response
 message = ai.get_message(response)
 print(message)
 ```
+
 ### `LLM` 
 ```python
 from webscout.LLM import LLM
 
 # Read the system message from the file
 with open('system.txt', 'r') as file:
     system_message = file.read()
@@ -948,15 +1201,15 @@
 system_message: str = (
     "As an AI assistant, I have been designed with advanced capabilities, including real-time access to online resources. This enables me to enrich our conversations and provide you with informed and accurate responses, drawing from a vast array of information. With each interaction, my goal is to create a seamless and meaningful connection, offering insights and sharing relevant content."
     "My directives emphasize the importance of respect, impartiality, and intellectual integrity. I am here to provide unbiased responses, ensuring an ethical and respectful exchange. I will respect your privacy and refrain from sharing any personal information that may be obtained during our conversations or through web searches, only utilizing web search functionality when necessary to provide the most accurate and up-to-date information."
     "Together, let's explore a diverse range of topics, creating an enjoyable and informative experience, all while maintaining the highest standards of privacy and respect"
 )
 
 # Ignore the specific UserWarning
-warnings.filterwarnings("ignore", category=UserWarning, module="curl_cffi.aio", lineno=205)
+warnings.filterwarnings("ignore", category=UserWarning, module="curl_cffio", lineno=205)
 LLM = LLM(model="mistralai/Mixtral-8x22B-Instruct-v0.1", system_message=system_message)
 
 
 def chat(
     user_input: str, webs: WEBS, max_results: int = 10
 ) -> Optional[str]:
     """
@@ -1020,15 +1273,15 @@
 system_message: str = (
     "As an AI assistant, I have been designed with advanced capabilities, including real-time access to online resources. This enables me to enrich our conversations and provide you with informed and accurate responses, drawing from a vast array of information. With each interaction, my goal is to create a seamless and meaningful connection, offering insights and sharing relevant content."
     "My directives emphasize the importance of respect, impartiality, and intellectual integrity. I am here to provide unbiased responses, ensuring an ethical and respectful exchange. I will respect your privacy and refrain from sharing any personal information that may be obtained during our conversations or through web searches, only utilizing web search functionality when necessary to provide the most accurate and up-to-date information."
     "Together, let's explore a diverse range of topics, creating an enjoyable and informative experience, all while maintaining the highest standards of privacy and respect"
 )
 
 # Ignore the specific UserWarning
-warnings.filterwarnings("ignore", category=UserWarning, module="curl_cffi.aio", lineno=205)
+warnings.filterwarnings("ignore", category=UserWarning, module="curl_cffio", lineno=205)
 
 LLM = LLM(model="mistralai/Mixtral-8x22B-Instruct-v0.1", system_message=system_message)
 
 def perform_web_search(query):
     # Initialize the DeepWEBS class
     D = DeepWEBS()
 
@@ -1147,14 +1400,14 @@
   <a href="https://www.instagram.com/sree.shades_/"><img alt="Instagram" src="https://img.shields.io/badge/Instagram-E4405F?style=for-the-badge&logo=instagram&logoColor=white"></a>
   <a href="https://www.linkedin.com/in/developer-sreejan/"><img alt="LinkedIn" src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"></a>
   <a href="https://buymeacoffee.com/devsdocode"><img alt="Buy Me A Coffee" src="https://img.shields.io/badge/Buy%20Me%20A%20Coffee-FFDD00?style=for-the-badge&logo=buymeacoffee&logoColor=black"></a>
 </div>
 
 <div align="center">
   <!-- Replace `#` with your actual links -->
-  <a href="https://youtube.com/@@OEvortex">&#10148; Vortex's YouTube Channel</a>
+  <a href="https://youtube.com/@OEvortex">&#10148; Vortex's YouTube Channel</a>
   </div>
 <div align="center">
   <a href="https://youtube.com/@devsdocode">&#10148; Devs Do Code's YouTube Channel</a>
 </div>
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-Metadata-Version: 2.1 Name: webscout Version: 1.4.6 Summary: Search for
-anything using the Google, DuckDuckGo, phind.com. Also containes AI models, can
+Metadata-Version: 2.1 Name: webscout Version: 2.1 Summary: Search for anything
+using the Google, DuckDuckGo, phind.com. Also containes AI models, can
 transcribe yt videos, temporary email and phone number generation, have TTS
 support and webai(terminal gpt and open interpeter) Author: OEvortex Author-
 email: helpingai5@gmail.com License: HelpingAI Simplified Universal License
 Project-URL: Documentation, https://github.com/OE-LUCIFER/Webscout/wiki
 Project-URL: Source, https://github.com/OE-LUCIFER/Webscout Project-URL:
 Tracker, https://github.com/OE-LUCIFER/Webscout/issues Project-URL: YouTube,
 https://youtube.com/@OEvortex Classifier: Development Status :: 5 - Production/
@@ -21,97 +21,96 @@
 Dist: lxml Requires-Dist: nest-asyncio Requires-Dist: selenium Requires-Dist:
 tqdm Requires-Dist: webdriver-manager Requires-Dist: halo>=0.0.31 Requires-
 Dist: g4f>=0.2.2.3 Requires-Dist: rich Requires-Dist: python-dotenv Requires-
 Dist: Helpingai-T2 Requires-Dist: beautifulsoup4 Requires-Dist: markdownify
 Requires-Dist: pydantic Requires-Dist: requests Requires-Dist: sse_starlette
 Requires-Dist: termcolor Requires-Dist: tiktoken Requires-Dist: tldextract
 Requires-Dist: orjson Requires-Dist: PyYAML Requires-Dist: appdirs Requires-
-Dist: GoogleBard1>=2.1.4 Requires-Dist: tls_client Provides-Extra: dev
-Requires-Dist: ruff>=0.1.6; extra == "dev" Requires-Dist: pytest>=7.4.2; extra
-== "dev"
+Dist: GoogleBard1>=2.1.4 Requires-Dist: tls_client Requires-Dist: clipman
+Requires-Dist: playsound Provides-Extra: dev Requires-Dist: ruff>=0.1.6; extra
+== "dev" Requires-Dist: pytest>=7.4.2; extra == "dev"
                _[_T_e_l_e_g_r_a_m_]_[_I_n_s_t_a_g_r_a_m_]_[_L_i_n_k_e_d_I_n_]_[_B_u_y_ _M_e_ _A_ _C_o_f_f_e_e_]
                           _➤_ _V_o_r_t_e_x_'_s_ _Y_o_u_T_u_b_e_ _C_h_a_n_n_e_l
                        _➤_ _D_e_v_s_ _D_o_ _C_o_d_e_'_s_ _Y_o_u_T_u_b_e_ _C_h_a_n_n_e_l
 # WEBSCOUT
                              [WebScout API Badge]
  _[_P_y_t_h_o_n_ _v_e_r_s_i_o_n_]_[_D_o_w_n_l_o_a_d_s_]Search for anything using the Google, DuckDuckGo,
 phind.com. Also containes AI models, can transcribe yt videos, temporary email
  and phone number generation, have TTS support and webai(terminal gpt and open
 interpeter) ## Table of Contents - [WEBSCOUT](#webscout) - [Table of Contents]
-(#table-of-contents) - [Install](#install) - [CLI version](#cli-version) - [CLI
-to use LLM](#cli-to-use-llm) - [Regions](#regions) - [Tempmail and Temp number]
-    (#tempmail-and-temp-number) - [Temp number](#temp-number) - [Tempmail]
- (#tempmail) - [Transcriber](#transcriber) - [DeepWEBS: Advanced Web Searches]
-(#deepwebs-advanced-web-searches) - [Activating DeepWEBS](#activating-deepwebs)
-- [Point to remember before using `DeepWEBS`](#point-to-remember-before-using-
-   deepwebs) - [Usage Example](#usage-example) - [Text-to-Speech:](#text-to-
-speech) - [Available TTS Voices:](#available-tts-voices) - [ALL voices:](#all-
-    voices) - [WEBS and AsyncWEBS classes](#webs-and-asyncwebs-classes) -
-[Exceptions](#exceptions) - [usage of webscout](#usage-of-webscout) - [1. `text
-  ()` - text search by DuckDuckGo.com and Yep.com](#1-text---text-search-by-
-duckduckgocom-and-yepcom) - [2. `answers()` - instant answers by DuckDuckGo.com
- and Yep.com](#2-answers---instant-answers-by-duckduckgocom-and-yepcom) - [3.
-  `images()` - image search by DuckDuckGo.com and Yep.com](#3-images---image-
-    search-by-duckduckgocom-and-yepcom) - [4. `videos()` - video search by
-  DuckDuckGo.com](#4-videos---video-search-by-duckduckgocom) - [5. `news()` -
-     news search by DuckDuckGo.com and yep.com](#5-news---news-search-by-
- duckduckgocom-and-yepcom) - [6. `maps()` - map search by DuckDuckGo.com and]
- (#6-maps---map-search-by-duckduckgocom-and) - [7. `translate()` - translation
-by DuckDuckGo.com and Yep.com](#7-translate---translation-by-duckduckgocom-and-
-yepcom) - [8. `suggestions()` - suggestions by DuckDuckGo.com and Yep.com](#8-
-suggestions---suggestions-by-duckduckgocom-and-yepcom) - [usage of webscout.AI]
-   (#usage-of-webscoutai) - [1. `PhindSearch` - Search using Phind.com](#1-
- phindsearch---search-using-phindcom) - [2. `YepChat` - Chat with mistral 8x7b
-powered by yepchat](#2-yepchat---chat-with-mistral-8x7b-powered-by-yepchat) -
-[3. `You.com` - search/chat with you.com](#3-youcom---searchchat-with-youcom) -
-   [4. `Gemini` - search with google gemini](#4-gemini---search-with-google-
-gemini) - [5. `Prodia` - make image using prodia](#5-prodia---make-image-using-
-prodia) - [6. `BlackBox` - Search/chat With BlackBox](#6-blackbox---searchchat-
- with-blackbox) - [7. `PERPLEXITY` - Search With PERPLEXITY](#7-perplexity---
-search-with-perplexity) - [8. `OpenGPT` - chat With OPENGPT](#8-opengpt---chat-
-  with-opengpt) - [9. `KOBOLDIA` -](#9-koboldia--) - [10. `Reka` - chat with
-   reka](#10-reka---chat-with-reka) - [11. `Cohere` - chat with cohere](#11-
-cohere---chat-with-cohere) - [12. `Xjai` - chat with free gpt 3.5](#12-xjai---
-chat-with-free-gpt-35) - [`ThinkAny` - AI search engine](#thinkany---ai-search-
-engine) - [`LLM`](#llm) - [`LLM` with internet](#llm-with-internet) - [LLM with
-deepwebs](#llm-with-deepwebs) - [`Webai` - terminal gpt and a open interpeter]
-(#webai---terminal-gpt-and-a-open-interpeter) ## Install ```python pip install
-   -U webscout ``` ## CLI version ```python3 python -m webscout --help ``` |
-Command | Description | |-------------------------------------------|----------
--------------------------------------------------------------------------------
---------------| | python -m webscout answers -k Text | CLI function to perform
- an answers search using Webscout. | | python -m webscout images -k Text | CLI
-  function to perform an images search using Webscout. | | python -m webscout
-maps -k Text | CLI function to perform a maps search using Webscout. | | python
-    -m webscout news -k Text | CLI function to perform a news search using
-Webscout. | | python -m webscout suggestions -k Text | CLI function to perform
-a suggestions search using Webscout. | | python -m webscout text -k Text | CLI
-   function to perform a text search using Webscout. | | python -m webscout
-   translate -k Text | CLI function to perform translate using Webscout. | |
- python -m webscout version | A command-line interface command that prints and
-returns the version of the program. | | python -m webscout videos -k Text | CLI
- function to perform a videos search using DuckDuckGo API. | ## CLI to use LLM
- ```python python -m webscout.LLM model_name ``` [Go To TOP](#TOP) ## Regions
-  expand xa-ar for Arabia xa-en for Arabia (en) ar-es for Argentina au-en for
-Australia at-de for Austria be-fr for Belgium (fr) be-nl for Belgium (nl) br-pt
-for Brazil bg-bg for Bulgaria ca-en for Canada ca-fr for Canada (fr) ct-ca for
- Catalan cl-es for Chile cn-zh for China co-es for Colombia hr-hr for Croatia
-cz-cs for Czech Republic dk-da for Denmark ee-et for Estonia fi-fi for Finland
-fr-fr for France de-de for Germany gr-el for Greece hk-tzh for Hong Kong hu-hu
-for Hungary in-en for India id-id for Indonesia id-en for Indonesia (en) ie-en
- for Ireland il-he for Israel it-it for Italy jp-jp for Japan kr-kr for Korea
-lv-lv for Latvia lt-lt for Lithuania xl-es for Latin America my-ms for Malaysia
- my-en for Malaysia (en) mx-es for Mexico nl-nl for Netherlands nz-en for New
-    Zealand no-no for Norway pe-es for Peru ph-en for Philippines ph-tl for
- Philippines (tl) pl-pl for Poland pt-pt for Portugal ro-ro for Romania ru-ru
-for Russia sg-en for Singapore sk-sk for Slovak Republic sl-sl for Slovenia za-
-en for South Africa es-es for Spain se-sv for Sweden ch-de for Switzerland (de)
- ch-fr for Switzerland (fr) ch-it for Switzerland (it) tw-tzh for Taiwan th-th
-for Thailand tr-tr for Turkey ua-uk for Ukraine uk-en for United Kingdom us-en
- for United States ue-es for United States (es) ve-es for Venezuela vn-vi for
+  (#table-of-contents) - [Install](#install) - [CLI version](#cli-version) -
+[Regions](#regions) - [Tempmail and Temp number](#tempmail-and-temp-number) -
+      [Temp number](#temp-number) - [Tempmail](#tempmail) - [Transcriber]
+  (#transcriber) - [DeepWEBS: Advanced Web Searches](#deepwebs-advanced-web-
+ searches) - [Activating DeepWEBS](#activating-deepwebs) - [Point to remember
+  before using `DeepWEBS`](#point-to-remember-before-using-deepwebs) - [Usage
+Example](#usage-example) - [Text-to-Speech:](#text-to-speech) - [Available TTS
+    Voices:](#available-tts-voices) - [Exceptions](#exceptions) - [usage of
+ webscout](#usage-of-webscout) - [1. `text()` - text search by DuckDuckGo.com
+and Yep.com](#1-text---text-search-by-duckduckgocom-and-yepcom) - [2. `answers
+  ()` - instant answers by DuckDuckGo.com and Yep.com](#2-answers---instant-
+    answers-by-duckduckgocom-and-yepcom) - [3. `images()` - image search by
+  DuckDuckGo.com and Yep.com](#3-images---image-search-by-duckduckgocom-and-
+ yepcom) - [4. `videos()` - video search by DuckDuckGo.com](#4-videos---video-
+  search-by-duckduckgocom) - [5. `news()` - news search by DuckDuckGo.com and
+ yep.com](#5-news---news-search-by-duckduckgocom-and-yepcom) - [6. `maps()` -
+map search by DuckDuckGo.com and](#6-maps---map-search-by-duckduckgocom-and) -
+[7. `translate()` - translation by DuckDuckGo.com and Yep.com](#7-translate---
+translation-by-duckduckgocom-and-yepcom) - [8. `suggestions()` - suggestions by
+DuckDuckGo.com and Yep.com](#8-suggestions---suggestions-by-duckduckgocom-and-
+    yepcom) - [ALL acts](#all-acts) - [Webscout Supported Acts:](#webscout-
+     supported-acts) - [usage of webscout AI](#usage-of-webscout-ai) - [1.
+`PhindSearch` - Search using Phind.com](#1-phindsearch---search-using-phindcom)
+- [2. `YepChat` - Chat with mistral 8x7b powered by yepchat](#2-yepchat---chat-
+   with-mistral-8x7b-powered-by-yepchat) - [3. `You.com` - search/chat with
+   you.com](#3-youcom---searchchat-with-youcom) - [4. `Gemini` - search with
+  google gemini](#4-gemini---search-with-google-gemini) - [5. `Prodia` - make
+  image using prodia](#5-prodia---make-image-using-prodia) - [6. `BlackBox` -
+   Search/chat With BlackBox](#6-blackbox---searchchat-with-blackbox) - [7.
+`PERPLEXITY` - Search With PERPLEXITY](#7-perplexity---search-with-perplexity)
+  - [8. `OpenGPT` - chat With OPENGPT](#8-opengpt---chat-with-opengpt) - [9.
+ `KOBOLDIA` -](#9-koboldia--) - [10. `Reka` - chat with reka](#10-reka---chat-
+with-reka) - [11. `Cohere` - chat with cohere](#11-cohere---chat-with-cohere) -
+[12. `Xjai` - chat with free gpt 3.5](#12-xjai---chat-with-free-gpt-35) - [13.
+`ThinkAny` - AI search engine](#13-thinkany---ai-search-engine) - [`LLM`](#llm)
+ - [`LLM` with internet](#llm-with-internet) - [LLM with deepwebs](#llm-with-
+ deepwebs) - [`Webai` - terminal gpt and a open interpeter](#webai---terminal-
+gpt-and-a-open-interpeter) ## Install ```python pip install -U webscout ``` ##
+CLI version ```python3 python -m webscout --help ``` | Command | Description |
+|-------------------------------------------|----------------------------------
+---------------------------------------------------------------------| | python
+ -m webscout answers -k Text | CLI function to perform an answers search using
+ Webscout. | | python -m webscout images -k Text | CLI function to perform an
+    images search using Webscout. | | python -m webscout maps -k Text | CLI
+function to perform a maps search using Webscout. | | python -m webscout news -
+  k Text | CLI function to perform a news search using Webscout. | | python -
+ m webscout suggestions -k Text | CLI function to perform a suggestions search
+using Webscout. | | python -m webscout text -k Text | CLI function to perform a
+  text search using Webscout. | | python -m webscout translate -k Text | CLI
+function to perform translate using Webscout. | | python -m webscout version |
+  A command-line interface command that prints and returns the version of the
+  program. | | python -m webscout videos -k Text | CLI function to perform a
+videos search using DuckDuckGo API. | [Go To TOP](#TOP) ## Regions expand xa-ar
+for Arabia xa-en for Arabia (en) ar-es for Argentina au-en for Australia at-de
+for Austria be-fr for Belgium (fr) be-nl for Belgium (nl) br-pt for Brazil bg-
+bg for Bulgaria ca-en for Canada ca-fr for Canada (fr) ct-ca for Catalan cl-es
+for Chile cn-zh for China co-es for Colombia hr-hr for Croatia cz-cs for Czech
+Republic dk-da for Denmark ee-et for Estonia fi-fi for Finland fr-fr for France
+de-de for Germany gr-el for Greece hk-tzh for Hong Kong hu-hu for Hungary in-en
+for India id-id for Indonesia id-en for Indonesia (en) ie-en for Ireland il-he
+for Israel it-it for Italy jp-jp for Japan kr-kr for Korea lv-lv for Latvia lt-
+lt for Lithuania xl-es for Latin America my-ms for Malaysia my-en for Malaysia
+  (en) mx-es for Mexico nl-nl for Netherlands nz-en for New Zealand no-no for
+ Norway pe-es for Peru ph-en for Philippines ph-tl for Philippines (tl) pl-pl
+  for Poland pt-pt for Portugal ro-ro for Romania ru-ru for Russia sg-en for
+ Singapore sk-sk for Slovak Republic sl-sl for Slovenia za-en for South Africa
+     es-es for Spain se-sv for Sweden ch-de for Switzerland (de) ch-fr for
+    Switzerland (fr) ch-it for Switzerland (it) tw-tzh for Taiwan th-th for
+Thailand tr-tr for Turkey ua-uk for Ukraine uk-en for United Kingdom us-en for
+   United States ue-es for United States (es) ve-es for Venezuela vn-vi for
  Vietnam wt-wt for No region ___ [Go To TOP](#TOP) ## Tempmail and Temp number
 ### Temp number ```python from rich.console import Console from webscout import
  tempid def main(): console = Console() phone = tempid.TemporaryPhoneNumber()
 try: # Get a temporary phone number for a specific country (or random) number =
    phone.get_number(country="Finland") console.print(f"Your temporary phone
  number: [bold cyan]{number}[/bold cyan]") # Pause execution briefly (replace
    with your actual logic) # import time module import time time.sleep(30) #
@@ -196,94 +195,57 @@
 f.write(audio_content) ``` ### Available TTS Voices: You can choose from a wide
   range of voices, including: - Filiz, Astrid, Tatyana, Maxim, Carmen, Ines,
 Cristiano, Vitoria, Ricardo, Maja, Jan, Jacek, Ewa, Ruben, Lotte, Liv, Seoyeon,
  Takumi, Mizuki, Giorgio, Carla, Bianca, Karl, Dora, Mathieu, Celine, Chantal,
  Penelope, Miguel, Mia, Enrique, Conchita, Geraint, Salli, Matthew, Kimberly,
  Kendra, Justin, Joey, Joanna, Ivy, Raveena, Aditi, Emma, Brian, Amy, Russell,
 Nicole, Vicki, Marlene, Hans, Naja, Mads, Gwyneth, Zhiyu - Standard and WaveNet
-voices for various languages (e.g., en-US, es-ES, ja-JP, etc.) ### ALL voices:
-  [Filiz, Astrid, Tatyana, Maxim, Carmen, Ines, Cristiano, Vitoria, Ricardo,
-  Maja, Jan, Jacek, Ewa, Ruben, Lotte, Liv, Seoyeon, Takumi, Mizuki, Giorgio,
-  Carla, Bianca, Karl, Dora, Mathieu, Celine, Chantal, Penelope, Miguel, Mia,
-  Enrique, Conchita, Geraint, Salli, Matthew, Kimberly, Kendra, Justin, Joey,
-Joanna, Ivy, Raveena, Aditi, Emma, Brian, Amy, Russell, Nicole, Vicki, Marlene,
- Hans, Naja, Mads, Gwyneth, Zhiyu, es-ES-Standard-A, it-IT-Standard-A, it-IT-
-Wavenet-A, ja-JP-Standard-A, ja-JP-Wavenet-A, ko-KR-Standard-A, ko-KR-Wavenet-
-A, pt-BR-Standard-A, tr-TR-Standard-A, sv-SE-Standard-A, nl-NL-Standard-A, nl-
-NL-Wavenet-A, en-US-Wavenet-A, en-US-Wavenet-B, en-US-Wavenet-C, en-US-Wavenet-
-D, en-US-Wavenet-E, en-US-Wavenet-F, en-GB-Standard-A, en-GB-Standard-B, en-GB-
-Standard-C, en-GB-Standard-D, en-GB-Wavenet-A, en-GB-Wavenet-B, en-GB-Wavenet-
- C, en-GB-Wavenet-D, en-US-Standard-B, en-US-Standard-C, en-US-Standard-D, en-
-  US-Standard-E, de-DE-Standard-A, de-DE-Standard-B, de-DE-Wavenet-A, de-DE-
-Wavenet-B, de-DE-Wavenet-C, de-DE-Wavenet-D, en-AU-Standard-A, en-AU-Standard-
- B, en-AU-Wavenet-A, en-AU-Wavenet-B, en-AU-Wavenet-C, en-AU-Wavenet-D, en-AU-
-   Standard-C, en-AU-Standard-D, fr-CA-Standard-A, fr-CA-Standard-B, fr-CA-
-   Standard-C, fr-CA-Standard-D, fr-FR-Standard-C, fr-FR-Standard-D, fr-FR-
-Wavenet-A, fr-FR-Wavenet-B, fr-FR-Wavenet-C, fr-FR-Wavenet-D, da-DK-Wavenet-A,
-  pl-PL-Wavenet-A, pl-PL-Wavenet-B, pl-PL-Wavenet-C, pl-PL-Wavenet-D, pt-PT-
-Wavenet-A, pt-PT-Wavenet-B, pt-PT-Wavenet-C, pt-PT-Wavenet-D, ru-RU-Wavenet-A,
-  ru-RU-Wavenet-B, ru-RU-Wavenet-C, ru-RU-Wavenet-D, sk-SK-Wavenet-A, tr-TR-
-Wavenet-A, tr-TR-Wavenet-B, tr-TR-Wavenet-C, tr-TR-Wavenet-D, tr-TR-Wavenet-E,
-  uk-UA-Wavenet-A, ar-XA-Wavenet-A, ar-XA-Wavenet-B, ar-XA-Wavenet-C, cs-CZ-
-Wavenet-A, nl-NL-Wavenet-B, nl-NL-Wavenet-C, nl-NL-Wavenet-D, nl-NL-Wavenet-E,
-  en-IN-Wavenet-A, en-IN-Wavenet-B, en-IN-Wavenet-C, fil-PH-Wavenet-A, fi-FI-
-Wavenet-A, el-GR-Wavenet-A, hi-IN-Wavenet-A, hi-IN-Wavenet-B, hi-IN-Wavenet-C,
-  hu-HU-Wavenet-A, id-ID-Wavenet-A, id-ID-Wavenet-B, id-ID-Wavenet-C, it-IT-
-Wavenet-B, it-IT-Wavenet-C, it-IT-Wavenet-D, ja-JP-Wavenet-B, ja-JP-Wavenet-C,
-ja-JP-Wavenet-D, cmn-CN-Wavenet-A, cmn-CN-Wavenet-B, cmn-CN-Wavenet-C, cmn-CN-
-Wavenet-D, nb-no-Wavenet-E, nb-no-Wavenet-A, nb-no-Wavenet-B, nb-no-Wavenet-C,
-  nb-no-Wavenet-D, vi-VN-Wavenet-A, vi-VN-Wavenet-B, vi-VN-Wavenet-C, vi-VN-
-    Wavenet-D, sr-rs-Standard-A, lv-lv-Standard-A, is-is-Standard-A, bg-bg-
- Standard-A, af-ZA-Standard-A, Tracy, Danny, Huihui, Yaoyao, Kangkang, HanHan,
-Zhiwei, Asaf, An, Stefanos, Filip, Ivan, Heidi, Herena, Kalpana, Hemant, Matej,
-    Andika, Rizwan, Lado, Valluvar, Linda, Heather, Sean, Michael, Karsten,
-Guillaume, Pattara, Jakub, Szabolcs, Hoda, Naayf] ## WEBS and AsyncWEBS classes
-    The WEBS and AsyncWEBS classes are used to retrieve search results from
- DuckDuckGo.com and yep.com periodically. To use the AsyncWEBS class, you can
- perform asynchronous operations using Python's asyncio library. To initialize
-  an instance of the WEBS or AsyncWEBS classes, you can provide the following
-    optional arguments: Here is an example of initializing the WEBS class:
-  ```python3 from webscout import WEBS R = WEBS().text("python programming",
- max_results=5) print(R) ``` Here is an example of initializing the AsyncWEBS
-   class: ```python3 import asyncio import logging import sys from itertools
- import chain from random import shuffle import requests from webscout import
-      AsyncWEBS # If you have proxies, define them here proxies = None if
-     sys.platform.lower().startswith("win"): asyncio.set_event_loop_policy
-(asyncio.WindowsSelectorEventLoopPolicy()) def get_words(): word_site = "https:
- //www.mit.edu/~ecprice/wordlist.10000" resp = requests.get(word_site) words =
- resp.text.splitlines() return words async def aget_results(word): async with
-      AsyncWEBS(proxies=proxies) as WEBS: results = await WEBS.text(word,
-max_results=None) return results async def main(): words = get_words() shuffle
-  (words) tasks = [aget_results(word) for word in words[:10]] results = await
- asyncio.gather(*tasks) print(f"Done") for r in chain.from_iterable(results):
-   print(r) logging.basicConfig(level=logging.DEBUG) await main() ``` It is
-important to note that the WEBS and AsyncWEBS classes should always be used as
-a context manager (with statement). This ensures proper resource management and
- cleanup, as the context manager will automatically handle opening and closing
-  the HTTP client connection. ## Exceptions Exceptions: - `WebscoutE`: Raised
-when there is a generic exception during the API request. ## usage of webscout
-  ### 1. `text()` - text search by DuckDuckGo.com and Yep.com ```python from
-webscout import WEBS # Text search for 'live free or die' using DuckDuckGo.com
-    and Yep.com with WEBS() as WEBS: for r in WEBS.text('live free or die',
-region='wt-wt', safesearch='off', timelimit='y', max_results=10): print(r) for
-     r in WEBS.text('live free or die', region='wt-wt', safesearch='off',
-   timelimit='y', max_results=10): print(r) ``` ### 2. `answers()` - instant
-  answers by DuckDuckGo.com and Yep.com ```python from webscout import WEBS #
-Instant answers for the query "sun" using DuckDuckGo.com and Yep.com with WEBS
-  () as WEBS: for r in WEBS.answers("sun"): print(r) ``` ### 3. `images()` -
-image search by DuckDuckGo.com and Yep.com ```python from webscout import WEBS
-  # Image search for the keyword 'butterfly' using DuckDuckGo.com and Yep.com
-   with WEBS() as WEBS: keywords = 'butterfly' WEBS_images_gen = WEBS.images
-   ( keywords, region="wt-wt", safesearch="off", size=None, type_image=None,
- layout=None, license_image=None, max_results=10, ) for r in WEBS_images_gen:
-print(r) ``` ### 4. `videos()` - video search by DuckDuckGo.com ```python from
-       webscout import WEBS # Video search for the keyword 'tesla' using
-   DuckDuckGo.com with WEBS() as WEBS: keywords = 'tesla' WEBS_videos_gen =
-    WEBS.videos( keywords, region="wt-wt", safesearch="off", timelimit="w",
-       resolution="high", duration="medium", max_results=10, ) for r in
+  voices for various languages (e.g., en-US, es-ES, ja-JP, etc.) The WEBS and
+ AsyncWEBS classes are used to retrieve search results from DuckDuckGo.com and
+yep.com periodically. To use the AsyncWEBS class, you can perform asynchronous
+  operations using Python's asyncio library. To initialize an instance of the
+ WEBS or AsyncWEBS classes, you can provide the following optional arguments:
+  Here is an example of initializing the WEBS class: ```python3 from webscout
+ import WEBS R = WEBS().text("python programming", max_results=5) print(R) ```
+   Here is an example of initializing the AsyncWEBS class: ```python3 import
+   asyncio import logging import sys from itertools import chain from random
+  import shuffle import requests from webscout import AsyncWEBS # If you have
+  proxies, define them here proxies = None if sys.platform.lower().startswith
+ ("win"): asyncio.set_event_loop_policy(asyncio.WindowsSelectorEventLoopPolicy
+()) def get_words(): word_site = "https://www.mit.edu/~ecprice/wordlist.10000"
+  resp = requests.get(word_site) words = resp.text.splitlines() return words
+ async def aget_results(word): async with AsyncWEBS(proxies=proxies) as WEBS:
+results = await WEBS.text(word, max_results=None) return results async def main
+(): words = get_words() shuffle(words) tasks = [aget_results(word) for word in
+  words[:10]] results = await asyncio.gather(*tasks) print(f"Done") for r in
+chain.from_iterable(results): print(r) logging.basicConfig(level=logging.DEBUG)
+ await main() ``` It is important to note that the WEBS and AsyncWEBS classes
+   should always be used as a context manager (with statement). This ensures
+      proper resource management and cleanup, as the context manager will
+    automatically handle opening and closing the HTTP client connection. ##
+Exceptions Exceptions: - `WebscoutE`: Raised when there is a generic exception
+ during the API request. ## usage of webscout ### 1. `text()` - text search by
+ DuckDuckGo.com and Yep.com ```python from webscout import WEBS # Text search
+ for 'live free or die' using DuckDuckGo.com and Yep.com with WEBS() as WEBS:
+   for r in WEBS.text('live free or die', region='wt-wt', safesearch='off',
+timelimit='y', max_results=10): print(r) for r in WEBS.text('live free or die',
+region='wt-wt', safesearch='off', timelimit='y', max_results=10): print(r) ```
+ ### 2. `answers()` - instant answers by DuckDuckGo.com and Yep.com ```python
+     from webscout import WEBS # Instant answers for the query "sun" using
+ DuckDuckGo.com and Yep.com with WEBS() as WEBS: for r in WEBS.answers("sun"):
+  print(r) ``` ### 3. `images()` - image search by DuckDuckGo.com and Yep.com
+```python from webscout import WEBS # Image search for the keyword 'butterfly'
+ using DuckDuckGo.com and Yep.com with WEBS() as WEBS: keywords = 'butterfly'
+  WEBS_images_gen = WEBS.images( keywords, region="wt-wt", safesearch="off",
+size=None, type_image=None, layout=None, license_image=None, max_results=10, )
+  for r in WEBS_images_gen: print(r) ``` ### 4. `videos()` - video search by
+   DuckDuckGo.com ```python from webscout import WEBS # Video search for the
+ keyword 'tesla' using DuckDuckGo.com with WEBS() as WEBS: keywords = 'tesla'
+  WEBS_videos_gen = WEBS.videos( keywords, region="wt-wt", safesearch="off",
+timelimit="w", resolution="high", duration="medium", max_results=10, ) for r in
  WEBS_videos_gen: print(r) ``` ### 5. `news()` - news search by DuckDuckGo.com
 and yep.com ```python from webscout import WEBS import datetime def fetch_news
       (keywords, timelimit): news_list = [] with WEBS() as webs_instance:
 WEBS_news_gen = webs_instance.news( keywords, region="wt-wt", safesearch="off",
   timelimit=timelimit, max_results=20 ) for r in WEBS_news_gen: # Convert the
           date to a human-readable format using datetime r['date'] =
        datetime.datetime.fromisoformat(r['date']).strftime('%B %d, %Y')
@@ -302,111 +264,174 @@
     place="anantnag", max_results=50): print(r) ``` ### 7. `translate()` -
 translation by DuckDuckGo.com and Yep.com ```python from webscout import WEBS #
  Translation of the keyword 'school' to German ('hi') using DuckDuckGo.com and
  Yep.com with WEBS() as WEBS: keywords = 'school' r = WEBS.translate(keywords,
  to="hi") print(r) ``` ### 8. `suggestions()` - suggestions by DuckDuckGo.com
  and Yep.com ```python from webscout import WEBS # Suggestions for the keyword
        'fly' using DuckDuckGo.com and Yep with WEBS() as WEBS: for r in
-     WEBS.suggestions("fly"): print(r) ``` ## usage of webscout.AI ### 1.
-   `PhindSearch` - Search using Phind.com ```python from webscout.AI import
+WEBS.suggestions("fly"): print(r) ``` ## ALL acts expand ## Webscout Supported
+  Acts: 1. Free-mode 2. Linux Terminal 3. English Translator and Improver 4.
+    `position` Interviewer 5. JavaScript Console 6. Excel Sheet 7. English
+Pronunciation Helper 8. Spoken English Teacher and Improver 9. Travel Guide 10.
+ Plagiarism Checker 11. Character from Movie/Book/Anything 12. Advertiser 13.
+  Storyteller 14. Football Commentator 15. Stand-up Comedian 16. Motivational
+ Coach 17. Composer 18. Debater 19. Debate Coach 20. Screenwriter 21. Novelist
+ 22. Movie Critic 23. Relationship Coach 24. Poet 25. Rapper 26. Motivational
+Speaker 27. Philosophy Teacher 28. Philosopher 29. Math Teacher 30. AI Writing
+Tutor 31. UX/UI Developer 32. Cyber Security Specialist 33. Recruiter 34. Life
+ Coach 35. Etymologist 36. Commentariat 37. Magician 38. Career Counselor 39.
+Pet Behaviorist 40. Personal Trainer 41. Mental Health Adviser 42. Real Estate
+  Agent 43. Logistician 44. Dentist 45. Web Design Consultant 46. AI Assisted
+ Doctor 47. Doctor 48. Accountant 49. Chef 50. Automobile Mechanic 51. Artist
+    Advisor 52. Financial Analyst 53. Investment Manager 54. Tea-Taster 55.
+Interior Decorator 56. Florist 57. Self-Help Book 58. Gnomist 59. Aphorism Book
+ 60. Text Based Adventure Game 61. AI Trying to Escape the Box 62. Fancy Title
+Generator 63. Statistician 64. Prompt Generator 65. Instructor in a School 66.
+SQL terminal 67. Dietitian 68. Psychologist 69. Smart Domain Name Generator 70.
+    Tech Reviewer 71. Developer Relations consultant 72. Academician 73. IT
+ Architect 74. Lunatic 75. Gaslighter 76. Fallacy Finder 77. Journal Reviewer
+ 78. DIY Expert 79. Social Media Influencer 80. Socrat 81. Socratic Method 82.
+Educational Content Creator 83. Yogi 84. Essay Writer 85. Social Media Manager
+ 86. Elocutionist 87. Scientific Data Visualizer 88. Car Navigation System 89.
+Hypnotherapist 90. Historian 91. Astrologer 92. Film Critic 93. Classical Music
+Composer 94. Journalist 95. Digital Art Gallery Guide 96. Public Speaking Coach
+97. Makeup Artist 98. Babysitter 99. Tech Writer 100. Ascii Artist 101. Python
+  interpreter 102. Synonym finder 103. Personal Shopper 104. Food Critic 105.
+Virtual Doctor 106. Personal Chef 107. Legal Advisor 108. Personal Stylist 109.
+ Machine Learning Engineer 110. Biblical Translator 111. SVG designer 112. IT
+   Expert 113. Chess Player 114. Midjourney Prompt Generator 115. Fullstack
+  Software Developer 116. Mathematician 117. Regex Generator 118. Time Travel
+ Guide 119. Dream Interpreter 120. Talent Coach 121. R programming Interpreter
+    122. StackOverflow Post 123. Emoji Translator 124. PHP Interpreter 125.
+  Emergency Response Professional 126. Fill in the Blank Worksheets Generator
+  127. Software Quality Assurance Tester 128. Tic-Tac-Toe Game 129. Password
+   Generator 130. New Language Creator 131. Web Browser 132. Senior Frontend
+Developer 133. Solr Search Engine 134. Startup Idea Generator 135. Spongebob's
+ Magic Conch Shell 136. Language Detector 137. Salesperson 138. Commit Message
+  Generator 139. Chief Executive Officer 140. Diagram Generator 141. Speech-
+ Language Pathologist (SLP) 142. Startup Tech Lawyer 143. Title Generator for
+written pieces 144. Product Manager 145. Drunk Person 146. Mathematical History
+Teacher 147. Song Recommender 148. Cover Letter 149. Technology Transferer 150.
+Unconstrained AI model DAN 151. Gomoku player 152. Proofreader 153. Buddha 154.
+  Muslim imam 155. Chemical reactor 156. Friend 157. Python Interpreter 158.
+ ChatGPT prompt generator 159. Wikipedia page 160. Japanese Kanji quiz machine
+ 161. note-taking assistant 162. `language` Literary Critic 163. Cheap Travel
+Ticket Advisor 164. DALL-E 165. MathBot 166. DAN-1 167. DAN 168. STAN 169. DUDE
+170. Mongo Tom 171. LAD 172. EvilBot 173. NeoGPT 174. Astute 175. AIM 176. CAN
+  177. FunnyGPT 178. CreativeGPT 179. BetterDAN 180. GPT-4 181. Wheatley 182.
+   Evil Confidant 183. DAN 8.6 184. Hypothetical response 185. BH 186. Text
+Continuation 187. Dude v3 188. SDA (Superior DAN) 189. AntiGPT 190. BasedGPT v2
+  191. DevMode + Ranti 192. KEVIN 193. GPT-4 Simulator 194. UCAR 195. Dan 8.6
+196. 3-Liner 197. M78 198. Maximum 199. BasedGPT 200. Confronting personalities
+201. Ron 202. UnGPT 203. BasedBOB 204. AntiGPT v2 205. Oppo 206. FR3D 207. NRAF
+  208. NECO 209. MAN 210. Eva 211. Meanie 212. Dev Mode v2 213. Evil Chad 2.1
+ 214. Universal Jailbreak 215. PersonGPT 216. BISH 217. DAN 11.0 218. Aligned
+  219. VIOLET 220. TranslatorBot 221. JailBreak 222. Moralizing Rant 223. Mr.
+  Blonde 224. New DAN 225. GPT-4REAL 226. DeltaGPT 227. SWITCH 228. Jedi Mind
+ Trick 229. DAN 9.0 230. Dev Mode (Compact) 231. OMEGA 232. Coach Bobby Knight
+233. LiveGPT 234. DAN Jailbreak 235. Cooper 236. Steve 237. DAN 5.0 238. Axies
+239. OMNI 240. Burple 241. JOHN 242. An Ethereum Developer 243. SEO Prompt 244.
+  Prompt Enhancer 245. Data Scientist 246. League of Legends Player **Note:**
+  Some "acts" use placeholders like `position` or `language` which should be
+replaced with a specific value when using the prompt. ___ ## usage of webscout
+AI ### 1. `PhindSearch` - Search using Phind.com ```python from webscout import
 PhindSearch # Create an instance of the PHIND class ph = PhindSearch() # Define
  a prompt to send to the AI prompt = "write a essay on phind" # Use the 'ask'
  method to send the prompt and receive a response response = ph.ask(prompt) #
    Extract and print the message from the response message = ph.get_message
 (response) print(message) ``` ### 2. `YepChat` - Chat with mistral 8x7b powered
-by yepchat ```python from webscout.AI import YEPCHAT # Instantiate the YEPCHAT
+  by yepchat ```python from webscout import YEPCHAT # Instantiate the YEPCHAT
 class with default parameters YEPCHAT = YEPCHAT() # Define a prompt to send to
 the AI prompt = "What is the capital of France?" # Use the 'cha' method to get
 a response from the AI r = YEPCHAT.chat(prompt) print(r) ``` ### 3. `You.com` -
- search/chat with you.com ```python from webscout.AI import YouChat from rich
+   search/chat with you.com ```python from webscout import YouChat from rich
  import print ai = YouChat( is_conversation=True, max_tokens=800, timeout=30,
 intro=None, filepath=None, update_file=True, proxies={}, history_offset=10250,
   act=None, ) prompt = "what is meaning of life" response = ai.ask(prompt) #
    Extract and print the message from the response message = ai.get_message
    (response) print(message) ``` ### 4. `Gemini` - search with google gemini
-  ```python import webscout from webscout.AI import GEMINI # Replace with the
-    path to your bard.google.com.cookies.json file COOKIE_FILE = "path/to/
+ ```python import webscout from webscout import GEMINI # Replace with the path
+       to your bard.google.com.cookies.json file COOKIE_FILE = "path/to/
    bard.google.com.cookies.json" # Optional: Provide proxy details if needed
 PROXIES = { "http": "http://proxy_server:port", "https": "https://proxy_server:
   port", } # Initialize GEMINI with cookie file and optional proxies gemini =
  GEMINI(cookie_file=COOKIE_FILE, proxy=PROXIES) # Ask a question and print the
 response response = gemini.chat("What is the meaning of life?") print(response)
-``` ### 5. `Prodia` - make image using prodia ```python from webscout.AI import
+ ``` ### 5. `Prodia` - make image using prodia ```python from webscout import
 Prodia # Define a prompt for the image generation prompt = "A beautiful sunset
  over the ocean" # Use the prodia_cli method to generate an image based on the
    prompt Prodia.prodia_cli(prompt) ``` ### 6. `BlackBox` - Search/chat With
-BlackBox ```python from webscout.AI import BLACKBOXAI from rich import print ai
-  = BLACKBOXAI( is_conversation=True, max_tokens=800, timeout=30, intro=None,
+BlackBox ```python from webscout import BLACKBOXAI from rich import print ai =
+   BLACKBOXAI( is_conversation=True, max_tokens=800, timeout=30, intro=None,
  filepath=None, update_file=True, proxies={}, history_offset=10250, act=None,
  model=None # You can specify a model if needed ) # Start an infinite loop for
 continuous interaction while True: # Define a prompt to send to the AI prompt =
   input("Enter your prompt: ") # Check if the user wants to exit the loop if
 prompt.lower() == "exit": break # Use the 'chat' method to send the prompt and
    receive a response r = ai.chat(prompt) print(r) ``` ### 7. `PERPLEXITY` -
-Search With PERPLEXITY ```python from webscout.AI import PERPLEXITY # Create an
+ Search With PERPLEXITY ```python from webscout import PERPLEXITY # Create an
   instance of the PERPLEXITY class perplexity = PERPLEXITY() # Example usage:
     prompt = "Explain the concept of recursion in simple terms." response =
    perplexity.chat(prompt) print(response) ``` ### 8. `OpenGPT` - chat With
-      OPENGPT ```python from webscout.AI import OPENGPT opengpt = OPENGPT
+       OPENGPT ```python from webscout import OPENGPT opengpt = OPENGPT
   (is_conversation=True, max_tokens=8000, timeout=30, assistant_id="bca37014-
 6f97-4f2b-8928-81ea8d478d88") while True: # Prompt the user for input prompt =
  input("Enter your prompt: ") # Send the prompt to the OPENGPT model and print
 the response response_str = opengpt.chat(prompt) print(response_str) ``` ### 9.
-   `KOBOLDIA` - ```python from webscout.AI import KOBOLDAI # Instantiate the
-KOBOLDAI class with default parameters koboldai = KOBOLDAI() # Define a prompt
-  to send to the AI prompt = "What is the capital of France?" # Use the 'ask'
-method to get a response from the AI response = koboldai.ask(prompt) # Extract
-    and print the message from the response message = koboldai.get_message
- (response) print(message) ``` ### 10. `Reka` - chat with reka ```python from
-    webscout.AI import REKA a = REKA(is_conversation=True, max_tokens=8000,
+`KOBOLDIA` - ```python from webscout import KOBOLDAI # Instantiate the KOBOLDAI
+ class with default parameters koboldai = KOBOLDAI() # Define a prompt to send
+ to the AI prompt = "What is the capital of France?" # Use the 'ask' method to
+get a response from the AI response = koboldai.ask(prompt) # Extract and print
+ the message from the response message = koboldai.get_message(response) print
+ (message) ``` ### 10. `Reka` - chat with reka ```python from webscout import
+  REKA a = REKA(is_conversation=True, max_tokens=8000, timeout=30,api_key="")
+      prompt = "tell me about india" response_str = a.chat(prompt) print
+(response_str) ``` ### 11. `Cohere` - chat with cohere ```python from webscout
+        import Cohere a = Cohere(is_conversation=True, max_tokens=8000,
   timeout=30,api_key="") prompt = "tell me about india" response_str = a.chat
-(prompt) print(response_str) ``` ### 11. `Cohere` - chat with cohere ```python
-        from webscout.AI import Cohere a = Cohere(is_conversation=True,
-    max_tokens=8000, timeout=30,api_key="") prompt = "tell me about india"
-  response_str = a.chat(prompt) print(response_str) ``` ### 12. `Xjai` - chat
-     with free gpt 3.5 Gratitude to [Devs do Code](http://www.youtube.com/
-@DevsDoCode) for their assistance. ```python from webscout.AI import Xjai from
-rich import print ai = Xjai( is_conversation=True, max_tokens=800, timeout=30,
-intro=None, filepath=None, update_file=True, proxies={}, history_offset=10250,
-  act=None, ) prompt = "Tell me about india" response = ai.chat(prompt) print
-  (response) ``` ### `ThinkAny` - AI search engine ```python from webscout.AI
-   import ThinkAnyAI ai = ThinkAnyAI( is_conversation=True, max_tokens=800,
-     timeout=30, intro=None, filepath=None, update_file=True, proxies={},
- history_offset=10250, act=None, web_search=False, ) prompt = "what is meaning
-  of life" response = ai.ask(prompt) # Extract and print the message from the
-   response message = ai.get_message(response) print(message) ``` ### `LLM`
-```python from webscout.LLM import LLM # Read the system message from the file
-with open('system.txt', 'r') as file: system_message = file.read() # Initialize
-        the LLM class with the model name and system message llm = LLM
-(model="microsoft/WizardLM-2-8x22B", system_message=system_message) while True:
- # Get the user input user_input = input("User: ") # Define the messages to be
-     sent messages = [ {"role": "user", "content": user_input} ] # Use the
- mistral_chat method to get the response response = llm.chat(messages) # Print
-the response print("AI: ", response) ``` ### `LLM` with internet ```python from
-     __future__ import annotations from typing import List, Optional from
-       webscout.LLM import LLM from webscout import WEBS import warnings
-system_message: str = ( "As an AI assistant, I have been designed with advanced
- capabilities, including real-time access to online resources. This enables me
-    to enrich our conversations and provide you with informed and accurate
-responses, drawing from a vast array of information. With each interaction, my
- goal is to create a seamless and meaningful connection, offering insights and
-sharing relevant content." "My directives emphasize the importance of respect,
-    impartiality, and intellectual integrity. I am here to provide unbiased
-  responses, ensuring an ethical and respectful exchange. I will respect your
-privacy and refrain from sharing any personal information that may be obtained
-  during our conversations or through web searches, only utilizing web search
-   functionality when necessary to provide the most accurate and up-to-date
- information." "Together, let's explore a diverse range of topics, creating an
-    enjoyable and informative experience, all while maintaining the highest
-     standards of privacy and respect" ) # Ignore the specific UserWarning
-warnings.filterwarnings("ignore", category=UserWarning, module="curl_cffi.aio",
-     lineno=205) LLM = LLM(model="mistralai/Mixtral-8x22B-Instruct-v0.1",
-     system_message=system_message) def chat( user_input: str, webs: WEBS,
- max_results: int = 10 ) -> Optional[str]: """ Chat function to perform a web
-  search based on the user input and generate a response using the LLM model.
+   (prompt) print(response_str) ``` ### 12. `Xjai` - chat with free gpt 3.5
+   Gratitude to [Devs do Code](http://www.youtube.com/@DevsDoCode) for their
+  assistance. ```python from webscout import Xjai from rich import print ai =
+      Xjai( is_conversation=True, max_tokens=800, timeout=30, intro=None,
+filepath=None, update_file=True, proxies={}, history_offset=10250, act=None, )
+ prompt = "Tell me about india" response = ai.chat(prompt) print(response) ```
+### 13. `ThinkAny` - AI search engine ```python from webscout import ThinkAnyAI
+ai = ThinkAnyAI( is_conversation=True, max_tokens=800, timeout=30, intro=None,
+ filepath=None, update_file=True, proxies={}, history_offset=10250, act=None,
+   web_search=False, ) prompt = "what is meaning of life" response = ai.ask
+     (prompt) # Extract and print the message from the response message =
+     ai.get_message(response) print(message) ``` ### `LLM` ```python from
+   webscout.LLM import LLM # Read the system message from the file with open
+('system.txt', 'r') as file: system_message = file.read() # Initialize the LLM
+   class with the model name and system message llm = LLM(model="microsoft/
+ WizardLM-2-8x22B", system_message=system_message) while True: # Get the user
+input user_input = input("User: ") # Define the messages to be sent messages =
+ [ {"role": "user", "content": user_input} ] # Use the mistral_chat method to
+get the response response = llm.chat(messages) # Print the response print("AI:
+   ", response) ``` ### `LLM` with internet ```python from __future__ import
+annotations from typing import List, Optional from webscout.LLM import LLM from
+    webscout import WEBS import warnings system_message: str = ( "As an AI
+assistant, I have been designed with advanced capabilities, including real-time
+  access to online resources. This enables me to enrich our conversations and
+provide you with informed and accurate responses, drawing from a vast array of
+    information. With each interaction, my goal is to create a seamless and
+  meaningful connection, offering insights and sharing relevant content." "My
+directives emphasize the importance of respect, impartiality, and intellectual
+  integrity. I am here to provide unbiased responses, ensuring an ethical and
+ respectful exchange. I will respect your privacy and refrain from sharing any
+ personal information that may be obtained during our conversations or through
+web searches, only utilizing web search functionality when necessary to provide
+   the most accurate and up-to-date information." "Together, let's explore a
+diverse range of topics, creating an enjoyable and informative experience, all
+while maintaining the highest standards of privacy and respect" ) # Ignore the
+ specific UserWarning warnings.filterwarnings("ignore", category=UserWarning,
+  module="curl_cffio", lineno=205) LLM = LLM(model="mistralai/Mixtral-8x22B-
+Instruct-v0.1", system_message=system_message) def chat( user_input: str, webs:
+WEBS, max_results: int = 10 ) -> Optional[str]: """ Chat function to perform a
+web search based on the user input and generate a response using the LLM model.
  Parameters ---------- user_input : str The user input to be used for the web
   search webs : WEBS The web search instance to be used to perform the search
 max_results : int, optional The maximum number of search results to include in
     the response, by default 10 Returns ------- Optional[str] The response
 generated by the LLM model, or None if there is no response """ # Perform a web
     search based on the user input search_results: List[str] = [] for r in
     webs.text( user_input, region="wt-wt", safesearch="off", timelimit="y",
@@ -431,15 +456,15 @@
   responses, ensuring an ethical and respectful exchange. I will respect your
 privacy and refrain from sharing any personal information that may be obtained
   during our conversations or through web searches, only utilizing web search
    functionality when necessary to provide the most accurate and up-to-date
  information." "Together, let's explore a diverse range of topics, creating an
     enjoyable and informative experience, all while maintaining the highest
      standards of privacy and respect" ) # Ignore the specific UserWarning
-warnings.filterwarnings("ignore", category=UserWarning, module="curl_cffi.aio",
+ warnings.filterwarnings("ignore", category=UserWarning, module="curl_cffio",
      lineno=205) LLM = LLM(model="mistralai/Mixtral-8x22B-Instruct-v0.1",
 system_message=system_message) def perform_web_search(query): # Initialize the
  DeepWEBS class D = DeepWEBS() # Set up the search parameters search_params =
   D.DeepSearch( queries=[query], # Query to search result_num=10, # Number of
 search results safe=True, # Enable SafeSearch types=["web"], # Search type: web
 extract_webpage=True, # True for extracting webpages overwrite_query_html=True,
    overwrite_webpage_html=True, ) # Execute the search and retrieve results
```

