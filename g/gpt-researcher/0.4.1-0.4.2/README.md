# Comparing `tmp/gpt-researcher-0.4.1.tar.gz` & `tmp/gpt-researcher-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt-researcher-0.4.1.tar", last modified: Sun May 12 07:07:43 2024, max compression
+gzip compressed data, was "gpt-researcher-0.4.2.tar", last modified: Sun May 12 07:20:43 2024, max compression
```

## Comparing `gpt-researcher-0.4.1.tar` & `gpt-researcher-0.4.2.tar`

### file list

```diff
@@ -1,103 +1,103 @@
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-12 07:07:43.655246 gpt-researcher-0.4.1/
--rw-r--r--   0 assafel    (501) staff       (20)     1069 2024-04-22 11:21:41.000000 gpt-researcher-0.4.1/LICENSE
--rw-r--r--   0 assafel    (501) staff       (20)    11566 2024-05-12 07:07:43.654761 gpt-researcher-0.4.1/PKG-INFO
--rw-r--r--   0 assafel    (501) staff       (20)    10843 2024-05-12 06:41:48.000000 gpt-researcher-0.4.1/README.md
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-12 07:07:43.612336 gpt-researcher-0.4.1/backend/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.4.1/backend/__init__.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-12 07:07:43.613129 gpt-researcher-0.4.1/backend/report_type/
--rw-r--r--   0 assafel    (501) staff       (20)      165 2024-04-22 11:21:41.000000 gpt-researcher-0.4.1/backend/report_type/__init__.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-12 07:07:43.614721 gpt-researcher-0.4.1/backend/report_type/basic_report/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.4.1/backend/report_type/basic_report/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)      777 2024-04-22 11:21:41.000000 gpt-researcher-0.4.1/backend/report_type/basic_report/basic_report.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-12 07:07:43.616558 gpt-researcher-0.4.1/backend/report_type/detailed_report/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.4.1/backend/report_type/detailed_report/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     6012 2024-04-22 11:21:41.000000 gpt-researcher-0.4.1/backend/report_type/detailed_report/detailed_report.py
--rw-r--r--   0 assafel    (501) staff       (20)     2327 2024-04-30 14:44:06.000000 gpt-researcher-0.4.1/backend/server.py
--rw-r--r--   0 assafel    (501) staff       (20)     2689 2024-04-30 14:43:31.000000 gpt-researcher-0.4.1/backend/utils.py
--rw-r--r--   0 assafel    (501) staff       (20)     2822 2024-04-22 11:21:41.000000 gpt-researcher-0.4.1/backend/websocket_manager.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-12 07:07:43.617303 gpt-researcher-0.4.1/gpt_researcher/
--rw-r--r--   0 assafel    (501) staff       (20)      100 2023-11-13 18:29:19.000000 gpt-researcher-0.4.1/gpt_researcher/__init__.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-12 07:07:43.622441 gpt-researcher-0.4.1/gpt_researcher/config/
--rw-r--r--   0 assafel    (501) staff       (20)       48 2023-11-13 18:29:19.000000 gpt-researcher-0.4.1/gpt_researcher/config/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     2114 2024-05-12 07:06:09.000000 gpt-researcher-0.4.1/gpt_researcher/config/config.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-12 07:07:43.624783 gpt-researcher-0.4.1/gpt_researcher/context/
--rw-r--r--   0 assafel    (501) staff       (20)      140 2023-11-19 07:01:11.000000 gpt-researcher-0.4.1/gpt_researcher/context/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     1796 2024-05-09 12:40:13.000000 gpt-researcher-0.4.1/gpt_researcher/context/compression.py
--rw-r--r--   0 assafel    (501) staff       (20)      801 2023-11-19 07:01:11.000000 gpt-researcher-0.4.1/gpt_researcher/context/retriever.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-12 07:07:43.625491 gpt-researcher-0.4.1/gpt_researcher/llm_provider/
--rw-r--r--   0 assafel    (501) staff       (20)      226 2024-04-22 11:21:41.000000 gpt-researcher-0.4.1/gpt_researcher/llm_provider/__init__.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-12 07:07:43.626513 gpt-researcher-0.4.1/gpt_researcher/llm_provider/azureopenai/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.4.1/gpt_researcher/llm_provider/azureopenai/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     3068 2024-04-22 11:21:41.000000 gpt-researcher-0.4.1/gpt_researcher/llm_provider/azureopenai/azureopenai.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-12 07:07:43.627849 gpt-researcher-0.4.1/gpt_researcher/llm_provider/google/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.4.1/gpt_researcher/llm_provider/google/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     3670 2024-04-22 11:21:41.000000 gpt-researcher-0.4.1/gpt_researcher/llm_provider/google/google.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-12 07:07:43.629465 gpt-researcher-0.4.1/gpt_researcher/llm_provider/openai/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.4.1/gpt_researcher/llm_provider/openai/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     2450 2024-05-08 07:24:47.000000 gpt-researcher-0.4.1/gpt_researcher/llm_provider/openai/openai.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-12 07:07:43.632017 gpt-researcher-0.4.1/gpt_researcher/master/
--rw-r--r--   0 assafel    (501) staff       (20)       61 2023-11-13 18:29:19.000000 gpt-researcher-0.4.1/gpt_researcher/master/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     9331 2024-05-10 05:37:26.000000 gpt-researcher-0.4.1/gpt_researcher/master/agent.py
--rw-r--r--   0 assafel    (501) staff       (20)    12460 2024-05-08 07:24:47.000000 gpt-researcher-0.4.1/gpt_researcher/master/functions.py
--rw-r--r--   0 assafel    (501) staff       (20)    13398 2024-05-06 06:02:27.000000 gpt-researcher-0.4.1/gpt_researcher/master/prompts.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-12 07:07:43.633344 gpt-researcher-0.4.1/gpt_researcher/memory/
--rw-r--r--   0 assafel    (501) staff       (20)       31 2023-11-19 07:01:11.000000 gpt-researcher-0.4.1/gpt_researcher/memory/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     1077 2024-05-09 06:30:45.000000 gpt-researcher-0.4.1/gpt_researcher/memory/embeddings.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-12 07:07:43.634396 gpt-researcher-0.4.1/gpt_researcher/retrievers/
--rw-r--r--   0 assafel    (501) staff       (20)      510 2023-12-18 08:18:37.000000 gpt-researcher-0.4.1/gpt_researcher/retrievers/__init__.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-12 07:07:43.635455 gpt-researcher-0.4.1/gpt_researcher/retrievers/bing/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2023-12-08 11:24:31.000000 gpt-researcher-0.4.1/gpt_researcher/retrievers/bing/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     2240 2023-12-08 11:24:31.000000 gpt-researcher-0.4.1/gpt_researcher/retrievers/bing/bing.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-12 07:07:43.636488 gpt-researcher-0.4.1/gpt_researcher/retrievers/duckduckgo/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.4.1/gpt_researcher/retrievers/duckduckgo/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)      479 2024-05-06 05:46:56.000000 gpt-researcher-0.4.1/gpt_researcher/retrievers/duckduckgo/duckduckgo.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-12 07:07:43.637930 gpt-researcher-0.4.1/gpt_researcher/retrievers/google/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.4.1/gpt_researcher/retrievers/google/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     2535 2023-11-19 07:01:11.000000 gpt-researcher-0.4.1/gpt_researcher/retrievers/google/google.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-12 07:07:43.639167 gpt-researcher-0.4.1/gpt_researcher/retrievers/searx/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.4.1/gpt_researcher/retrievers/searx/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     1294 2024-04-22 11:21:41.000000 gpt-researcher-0.4.1/gpt_researcher/retrievers/searx/searx.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-12 07:07:43.640329 gpt-researcher-0.4.1/gpt_researcher/retrievers/serpapi/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.4.1/gpt_researcher/retrievers/serpapi/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     2232 2023-11-25 13:46:26.000000 gpt-researcher-0.4.1/gpt_researcher/retrievers/serpapi/serpapi.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-12 07:07:43.641893 gpt-researcher-0.4.1/gpt_researcher/retrievers/serper/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.4.1/gpt_researcher/retrievers/serper/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     2117 2023-11-25 13:46:26.000000 gpt-researcher-0.4.1/gpt_researcher/retrievers/serper/serper.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-12 07:07:43.643088 gpt-researcher-0.4.1/gpt_researcher/retrievers/tavily_news/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2023-12-18 08:18:37.000000 gpt-researcher-0.4.1/gpt_researcher/retrievers/tavily_news/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     1281 2023-12-18 08:18:37.000000 gpt-researcher-0.4.1/gpt_researcher/retrievers/tavily_news/tavily_news.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-12 07:07:43.644083 gpt-researcher-0.4.1/gpt_researcher/retrievers/tavily_search/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.4.1/gpt_researcher/retrievers/tavily_search/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     1675 2024-05-09 06:46:00.000000 gpt-researcher-0.4.1/gpt_researcher/retrievers/tavily_search/tavily_search.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-12 07:07:43.645643 gpt-researcher-0.4.1/gpt_researcher/scraper/
--rw-r--r--   0 assafel    (501) staff       (20)      398 2024-03-17 08:29:46.000000 gpt-researcher-0.4.1/gpt_researcher/scraper/__init__.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-12 07:07:43.646750 gpt-researcher-0.4.1/gpt_researcher/scraper/arxiv/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.4.1/gpt_researcher/scraper/arxiv/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)      762 2024-03-12 13:09:58.000000 gpt-researcher-0.4.1/gpt_researcher/scraper/arxiv/arxiv.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-12 07:07:43.647786 gpt-researcher-0.4.1/gpt_researcher/scraper/beautiful_soup/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.4.1/gpt_researcher/scraper/beautiful_soup/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     1992 2024-03-12 13:09:58.000000 gpt-researcher-0.4.1/gpt_researcher/scraper/beautiful_soup/beautiful_soup.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-12 07:07:43.648797 gpt-researcher-0.4.1/gpt_researcher/scraper/newspaper/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.4.1/gpt_researcher/scraper/newspaper/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     1312 2024-03-12 13:09:58.000000 gpt-researcher-0.4.1/gpt_researcher/scraper/newspaper/newspaper.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-12 07:07:43.650199 gpt-researcher-0.4.1/gpt_researcher/scraper/pymupdf/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.4.1/gpt_researcher/scraper/pymupdf/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)      640 2024-03-12 13:09:58.000000 gpt-researcher-0.4.1/gpt_researcher/scraper/pymupdf/pymupdf.py
--rw-r--r--   0 assafel    (501) staff       (20)     3111 2024-03-17 08:29:46.000000 gpt-researcher-0.4.1/gpt_researcher/scraper/scraper.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-12 07:07:43.651427 gpt-researcher-0.4.1/gpt_researcher/scraper/web_base_loader/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.4.1/gpt_researcher/scraper/web_base_loader/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     1074 2024-03-12 13:09:58.000000 gpt-researcher-0.4.1/gpt_researcher/scraper/web_base_loader/web_base_loader.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-12 07:07:43.654037 gpt-researcher-0.4.1/gpt_researcher/utils/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.4.1/gpt_researcher/utils/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)      274 2024-04-22 11:21:41.000000 gpt-researcher-0.4.1/gpt_researcher/utils/enum.py
--rw-r--r--   0 assafel    (501) staff       (20)     5108 2024-04-22 11:21:41.000000 gpt-researcher-0.4.1/gpt_researcher/utils/llm.py
--rw-r--r--   0 assafel    (501) staff       (20)      216 2024-04-22 11:21:41.000000 gpt-researcher-0.4.1/gpt_researcher/utils/validators.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-12 07:07:43.620799 gpt-researcher-0.4.1/gpt_researcher.egg-info/
--rw-r--r--   0 assafel    (501) staff       (20)    11566 2024-05-12 07:07:43.000000 gpt-researcher-0.4.1/gpt_researcher.egg-info/PKG-INFO
--rw-r--r--   0 assafel    (501) staff       (20)     2727 2024-05-12 07:07:43.000000 gpt-researcher-0.4.1/gpt_researcher.egg-info/SOURCES.txt
--rw-r--r--   0 assafel    (501) staff       (20)        1 2024-05-12 07:07:43.000000 gpt-researcher-0.4.1/gpt_researcher.egg-info/dependency_links.txt
--rw-r--r--   0 assafel    (501) staff       (20)      342 2024-05-12 07:07:43.000000 gpt-researcher-0.4.1/gpt_researcher.egg-info/requires.txt
--rw-r--r--   0 assafel    (501) staff       (20)       23 2024-05-12 07:07:43.000000 gpt-researcher-0.4.1/gpt_researcher.egg-info/top_level.txt
--rw-r--r--   0 assafel    (501) staff       (20)     1156 2024-04-27 17:11:32.000000 gpt-researcher-0.4.1/pyproject.toml
--rw-r--r--   0 assafel    (501) staff       (20)       38 2024-05-12 07:07:43.655432 gpt-researcher-0.4.1/setup.cfg
--rw-r--r--   0 assafel    (501) staff       (20)     1176 2024-05-12 07:07:20.000000 gpt-researcher-0.4.1/setup.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-12 07:20:43.630723 gpt-researcher-0.4.2/
+-rw-r--r--   0 assafel    (501) staff       (20)     1069 2024-04-22 11:21:41.000000 gpt-researcher-0.4.2/LICENSE
+-rw-r--r--   0 assafel    (501) staff       (20)    11566 2024-05-12 07:20:43.630113 gpt-researcher-0.4.2/PKG-INFO
+-rw-r--r--   0 assafel    (501) staff       (20)    10843 2024-05-12 06:41:48.000000 gpt-researcher-0.4.2/README.md
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-12 07:20:43.589711 gpt-researcher-0.4.2/backend/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.4.2/backend/__init__.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-12 07:20:43.590249 gpt-researcher-0.4.2/backend/report_type/
+-rw-r--r--   0 assafel    (501) staff       (20)      165 2024-04-22 11:21:41.000000 gpt-researcher-0.4.2/backend/report_type/__init__.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-12 07:20:43.591293 gpt-researcher-0.4.2/backend/report_type/basic_report/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.4.2/backend/report_type/basic_report/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)      777 2024-04-22 11:21:41.000000 gpt-researcher-0.4.2/backend/report_type/basic_report/basic_report.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-12 07:20:43.592336 gpt-researcher-0.4.2/backend/report_type/detailed_report/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.4.2/backend/report_type/detailed_report/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     6012 2024-04-22 11:21:41.000000 gpt-researcher-0.4.2/backend/report_type/detailed_report/detailed_report.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2327 2024-04-30 14:44:06.000000 gpt-researcher-0.4.2/backend/server.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2689 2024-04-30 14:43:31.000000 gpt-researcher-0.4.2/backend/utils.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2822 2024-04-22 11:21:41.000000 gpt-researcher-0.4.2/backend/websocket_manager.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-12 07:20:43.592878 gpt-researcher-0.4.2/gpt_researcher/
+-rw-r--r--   0 assafel    (501) staff       (20)      100 2023-11-13 18:29:19.000000 gpt-researcher-0.4.2/gpt_researcher/__init__.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-12 07:20:43.596649 gpt-researcher-0.4.2/gpt_researcher/config/
+-rw-r--r--   0 assafel    (501) staff       (20)       48 2023-11-13 18:29:19.000000 gpt-researcher-0.4.2/gpt_researcher/config/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2115 2024-05-12 07:19:17.000000 gpt-researcher-0.4.2/gpt_researcher/config/config.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-12 07:20:43.598266 gpt-researcher-0.4.2/gpt_researcher/context/
+-rw-r--r--   0 assafel    (501) staff       (20)      140 2023-11-19 07:01:11.000000 gpt-researcher-0.4.2/gpt_researcher/context/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1796 2024-05-09 12:40:13.000000 gpt-researcher-0.4.2/gpt_researcher/context/compression.py
+-rw-r--r--   0 assafel    (501) staff       (20)      801 2023-11-19 07:01:11.000000 gpt-researcher-0.4.2/gpt_researcher/context/retriever.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-12 07:20:43.598849 gpt-researcher-0.4.2/gpt_researcher/llm_provider/
+-rw-r--r--   0 assafel    (501) staff       (20)      226 2024-04-22 11:21:41.000000 gpt-researcher-0.4.2/gpt_researcher/llm_provider/__init__.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-12 07:20:43.599843 gpt-researcher-0.4.2/gpt_researcher/llm_provider/azureopenai/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.4.2/gpt_researcher/llm_provider/azureopenai/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     3068 2024-04-22 11:21:41.000000 gpt-researcher-0.4.2/gpt_researcher/llm_provider/azureopenai/azureopenai.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-12 07:20:43.600857 gpt-researcher-0.4.2/gpt_researcher/llm_provider/google/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.4.2/gpt_researcher/llm_provider/google/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     3670 2024-04-22 11:21:41.000000 gpt-researcher-0.4.2/gpt_researcher/llm_provider/google/google.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-12 07:20:43.602006 gpt-researcher-0.4.2/gpt_researcher/llm_provider/openai/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.4.2/gpt_researcher/llm_provider/openai/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2450 2024-05-08 07:24:47.000000 gpt-researcher-0.4.2/gpt_researcher/llm_provider/openai/openai.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-12 07:20:43.604351 gpt-researcher-0.4.2/gpt_researcher/master/
+-rw-r--r--   0 assafel    (501) staff       (20)       61 2023-11-13 18:29:19.000000 gpt-researcher-0.4.2/gpt_researcher/master/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     9331 2024-05-10 05:37:26.000000 gpt-researcher-0.4.2/gpt_researcher/master/agent.py
+-rw-r--r--   0 assafel    (501) staff       (20)    12460 2024-05-08 07:24:47.000000 gpt-researcher-0.4.2/gpt_researcher/master/functions.py
+-rw-r--r--   0 assafel    (501) staff       (20)    13398 2024-05-06 06:02:27.000000 gpt-researcher-0.4.2/gpt_researcher/master/prompts.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-12 07:20:43.605561 gpt-researcher-0.4.2/gpt_researcher/memory/
+-rw-r--r--   0 assafel    (501) staff       (20)       31 2023-11-19 07:01:11.000000 gpt-researcher-0.4.2/gpt_researcher/memory/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1077 2024-05-09 06:30:45.000000 gpt-researcher-0.4.2/gpt_researcher/memory/embeddings.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-12 07:20:43.606096 gpt-researcher-0.4.2/gpt_researcher/retrievers/
+-rw-r--r--   0 assafel    (501) staff       (20)      510 2023-12-18 08:18:37.000000 gpt-researcher-0.4.2/gpt_researcher/retrievers/__init__.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-12 07:20:43.607066 gpt-researcher-0.4.2/gpt_researcher/retrievers/bing/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2023-12-08 11:24:31.000000 gpt-researcher-0.4.2/gpt_researcher/retrievers/bing/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2240 2023-12-08 11:24:31.000000 gpt-researcher-0.4.2/gpt_researcher/retrievers/bing/bing.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-12 07:20:43.608074 gpt-researcher-0.4.2/gpt_researcher/retrievers/duckduckgo/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.4.2/gpt_researcher/retrievers/duckduckgo/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)      479 2024-05-06 05:46:56.000000 gpt-researcher-0.4.2/gpt_researcher/retrievers/duckduckgo/duckduckgo.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-12 07:20:43.609064 gpt-researcher-0.4.2/gpt_researcher/retrievers/google/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.4.2/gpt_researcher/retrievers/google/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2535 2023-11-19 07:01:11.000000 gpt-researcher-0.4.2/gpt_researcher/retrievers/google/google.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-12 07:20:43.610041 gpt-researcher-0.4.2/gpt_researcher/retrievers/searx/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.4.2/gpt_researcher/retrievers/searx/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1294 2024-04-22 11:21:41.000000 gpt-researcher-0.4.2/gpt_researcher/retrievers/searx/searx.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-12 07:20:43.611598 gpt-researcher-0.4.2/gpt_researcher/retrievers/serpapi/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.4.2/gpt_researcher/retrievers/serpapi/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2232 2023-11-25 13:46:26.000000 gpt-researcher-0.4.2/gpt_researcher/retrievers/serpapi/serpapi.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-12 07:20:43.613126 gpt-researcher-0.4.2/gpt_researcher/retrievers/serper/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.4.2/gpt_researcher/retrievers/serper/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2117 2023-11-25 13:46:26.000000 gpt-researcher-0.4.2/gpt_researcher/retrievers/serper/serper.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-12 07:20:43.614902 gpt-researcher-0.4.2/gpt_researcher/retrievers/tavily_news/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2023-12-18 08:18:37.000000 gpt-researcher-0.4.2/gpt_researcher/retrievers/tavily_news/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1281 2023-12-18 08:18:37.000000 gpt-researcher-0.4.2/gpt_researcher/retrievers/tavily_news/tavily_news.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-12 07:20:43.616614 gpt-researcher-0.4.2/gpt_researcher/retrievers/tavily_search/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.4.2/gpt_researcher/retrievers/tavily_search/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1675 2024-05-09 06:46:00.000000 gpt-researcher-0.4.2/gpt_researcher/retrievers/tavily_search/tavily_search.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-12 07:20:43.618556 gpt-researcher-0.4.2/gpt_researcher/scraper/
+-rw-r--r--   0 assafel    (501) staff       (20)      398 2024-03-17 08:29:46.000000 gpt-researcher-0.4.2/gpt_researcher/scraper/__init__.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-12 07:20:43.620192 gpt-researcher-0.4.2/gpt_researcher/scraper/arxiv/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.4.2/gpt_researcher/scraper/arxiv/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)      762 2024-03-12 13:09:58.000000 gpt-researcher-0.4.2/gpt_researcher/scraper/arxiv/arxiv.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-12 07:20:43.622084 gpt-researcher-0.4.2/gpt_researcher/scraper/beautiful_soup/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.4.2/gpt_researcher/scraper/beautiful_soup/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1992 2024-03-12 13:09:58.000000 gpt-researcher-0.4.2/gpt_researcher/scraper/beautiful_soup/beautiful_soup.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-12 07:20:43.623596 gpt-researcher-0.4.2/gpt_researcher/scraper/newspaper/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.4.2/gpt_researcher/scraper/newspaper/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1312 2024-03-12 13:09:58.000000 gpt-researcher-0.4.2/gpt_researcher/scraper/newspaper/newspaper.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-12 07:20:43.625177 gpt-researcher-0.4.2/gpt_researcher/scraper/pymupdf/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.4.2/gpt_researcher/scraper/pymupdf/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)      640 2024-03-12 13:09:58.000000 gpt-researcher-0.4.2/gpt_researcher/scraper/pymupdf/pymupdf.py
+-rw-r--r--   0 assafel    (501) staff       (20)     3111 2024-03-17 08:29:46.000000 gpt-researcher-0.4.2/gpt_researcher/scraper/scraper.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-12 07:20:43.626454 gpt-researcher-0.4.2/gpt_researcher/scraper/web_base_loader/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.4.2/gpt_researcher/scraper/web_base_loader/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1074 2024-03-12 13:09:58.000000 gpt-researcher-0.4.2/gpt_researcher/scraper/web_base_loader/web_base_loader.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-12 07:20:43.628996 gpt-researcher-0.4.2/gpt_researcher/utils/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.4.2/gpt_researcher/utils/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)      274 2024-04-22 11:21:41.000000 gpt-researcher-0.4.2/gpt_researcher/utils/enum.py
+-rw-r--r--   0 assafel    (501) staff       (20)     5108 2024-04-22 11:21:41.000000 gpt-researcher-0.4.2/gpt_researcher/utils/llm.py
+-rw-r--r--   0 assafel    (501) staff       (20)      216 2024-04-22 11:21:41.000000 gpt-researcher-0.4.2/gpt_researcher/utils/validators.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-12 07:20:43.595579 gpt-researcher-0.4.2/gpt_researcher.egg-info/
+-rw-r--r--   0 assafel    (501) staff       (20)    11566 2024-05-12 07:20:43.000000 gpt-researcher-0.4.2/gpt_researcher.egg-info/PKG-INFO
+-rw-r--r--   0 assafel    (501) staff       (20)     2727 2024-05-12 07:20:43.000000 gpt-researcher-0.4.2/gpt_researcher.egg-info/SOURCES.txt
+-rw-r--r--   0 assafel    (501) staff       (20)        1 2024-05-12 07:20:43.000000 gpt-researcher-0.4.2/gpt_researcher.egg-info/dependency_links.txt
+-rw-r--r--   0 assafel    (501) staff       (20)      342 2024-05-12 07:20:43.000000 gpt-researcher-0.4.2/gpt_researcher.egg-info/requires.txt
+-rw-r--r--   0 assafel    (501) staff       (20)       23 2024-05-12 07:20:43.000000 gpt-researcher-0.4.2/gpt_researcher.egg-info/top_level.txt
+-rw-r--r--   0 assafel    (501) staff       (20)     1156 2024-04-27 17:11:32.000000 gpt-researcher-0.4.2/pyproject.toml
+-rw-r--r--   0 assafel    (501) staff       (20)       38 2024-05-12 07:20:43.630871 gpt-researcher-0.4.2/setup.cfg
+-rw-r--r--   0 assafel    (501) staff       (20)     1176 2024-05-12 07:20:23.000000 gpt-researcher-0.4.2/setup.py
```

### Comparing `gpt-researcher-0.4.1/LICENSE` & `gpt-researcher-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.4.1/PKG-INFO` & `gpt-researcher-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-researcher
-Version: 0.4.1
+Version: 0.4.2
 Summary: GPT Researcher is an autonomous agent designed for comprehensive online research on a variety of tasks.
 Home-page: https://github.com/assafelovic/gpt-researcher
 Author: Assaf Elovic
 Author-email: assaf.elovic@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
```

### Comparing `gpt-researcher-0.4.1/README.md` & `gpt-researcher-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.4.1/backend/report_type/basic_report/basic_report.py` & `gpt-researcher-0.4.2/backend/report_type/basic_report/basic_report.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.4.1/backend/report_type/detailed_report/detailed_report.py` & `gpt-researcher-0.4.2/backend/report_type/detailed_report/detailed_report.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.4.1/backend/server.py` & `gpt-researcher-0.4.2/backend/server.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.4.1/backend/utils.py` & `gpt-researcher-0.4.2/backend/utils.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.4.1/backend/websocket_manager.py` & `gpt-researcher-0.4.2/backend/websocket_manager.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.4.1/gpt_researcher/config/config.py` & `gpt-researcher-0.4.2/gpt_researcher/config/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 class Config:
     """Config class for GPT Researcher."""
 
     def __init__(self, config_file: str = None):
         """Initialize the config class."""
         self.config_file = os.path.expanduser(config_file) if config_file else os.getenv('CONFIG_FILE')
-        self.retriever = os.getenv('SEARCH_RETRIEVER', "tavily")
+        self.retriever = os.getenv('RETRIEVER', "tavily")
         self.embedding_provider = os.getenv('EMBEDDING_PROVIDER', 'openai')
         self.llm_provider = os.getenv('LLM_PROVIDER', "openai")
         self.fast_llm_model = os.getenv('FAST_LLM_MODEL', "gpt-3.5-turbo-16k")
         self.smart_llm_model = os.getenv('SMART_LLM_MODEL', "gpt-4-turbo")
         self.fast_token_limit = int(os.getenv('FAST_TOKEN_LIMIT', 2000))
         self.smart_token_limit = int(os.getenv('SMART_TOKEN_LIMIT', 4000))
         self.browse_chunk_max_length = int(os.getenv('BROWSE_CHUNK_MAX_LENGTH', 8192))
@@ -35,9 +35,9 @@
     def load_config_file(self) -> None:
         """Load the config file."""
         if self.config_file is None:
             return None
         with open(self.config_file, "r") as f:
             config = json.load(f)
         for key, value in config.items():
-            self.__dict__[key] = value
+            self.__dict__[key.lower()] = value
```

### Comparing `gpt-researcher-0.4.1/gpt_researcher/context/compression.py` & `gpt-researcher-0.4.2/gpt_researcher/context/compression.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.4.1/gpt_researcher/context/retriever.py` & `gpt-researcher-0.4.2/gpt_researcher/context/retriever.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.4.1/gpt_researcher/llm_provider/azureopenai/azureopenai.py` & `gpt-researcher-0.4.2/gpt_researcher/llm_provider/azureopenai/azureopenai.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.4.1/gpt_researcher/llm_provider/google/google.py` & `gpt-researcher-0.4.2/gpt_researcher/llm_provider/google/google.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.4.1/gpt_researcher/llm_provider/openai/openai.py` & `gpt-researcher-0.4.2/gpt_researcher/llm_provider/openai/openai.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.4.1/gpt_researcher/master/agent.py` & `gpt-researcher-0.4.2/gpt_researcher/master/agent.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.4.1/gpt_researcher/master/functions.py` & `gpt-researcher-0.4.2/gpt_researcher/master/functions.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.4.1/gpt_researcher/master/prompts.py` & `gpt-researcher-0.4.2/gpt_researcher/master/prompts.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.4.1/gpt_researcher/memory/embeddings.py` & `gpt-researcher-0.4.2/gpt_researcher/memory/embeddings.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.4.1/gpt_researcher/retrievers/bing/bing.py` & `gpt-researcher-0.4.2/gpt_researcher/retrievers/bing/bing.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.4.1/gpt_researcher/retrievers/google/google.py` & `gpt-researcher-0.4.2/gpt_researcher/retrievers/google/google.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.4.1/gpt_researcher/retrievers/searx/searx.py` & `gpt-researcher-0.4.2/gpt_researcher/retrievers/searx/searx.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.4.1/gpt_researcher/retrievers/serpapi/serpapi.py` & `gpt-researcher-0.4.2/gpt_researcher/retrievers/serpapi/serpapi.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.4.1/gpt_researcher/retrievers/serper/serper.py` & `gpt-researcher-0.4.2/gpt_researcher/retrievers/serper/serper.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.4.1/gpt_researcher/retrievers/tavily_news/tavily_news.py` & `gpt-researcher-0.4.2/gpt_researcher/retrievers/tavily_news/tavily_news.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.4.1/gpt_researcher/retrievers/tavily_search/tavily_search.py` & `gpt-researcher-0.4.2/gpt_researcher/retrievers/tavily_search/tavily_search.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.4.1/gpt_researcher/scraper/arxiv/arxiv.py` & `gpt-researcher-0.4.2/gpt_researcher/scraper/arxiv/arxiv.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.4.1/gpt_researcher/scraper/beautiful_soup/beautiful_soup.py` & `gpt-researcher-0.4.2/gpt_researcher/scraper/beautiful_soup/beautiful_soup.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.4.1/gpt_researcher/scraper/newspaper/newspaper.py` & `gpt-researcher-0.4.2/gpt_researcher/scraper/newspaper/newspaper.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.4.1/gpt_researcher/scraper/pymupdf/pymupdf.py` & `gpt-researcher-0.4.2/gpt_researcher/scraper/pymupdf/pymupdf.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.4.1/gpt_researcher/scraper/scraper.py` & `gpt-researcher-0.4.2/gpt_researcher/scraper/scraper.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.4.1/gpt_researcher/scraper/web_base_loader/web_base_loader.py` & `gpt-researcher-0.4.2/gpt_researcher/scraper/web_base_loader/web_base_loader.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.4.1/gpt_researcher/utils/llm.py` & `gpt-researcher-0.4.2/gpt_researcher/utils/llm.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.4.1/gpt_researcher.egg-info/PKG-INFO` & `gpt-researcher-0.4.2/gpt_researcher.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-researcher
-Version: 0.4.1
+Version: 0.4.2
 Summary: GPT Researcher is an autonomous agent designed for comprehensive online research on a variety of tasks.
 Home-page: https://github.com/assafelovic/gpt-researcher
 Author: Assaf Elovic
 Author-email: assaf.elovic@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
```

### Comparing `gpt-researcher-0.4.1/gpt_researcher.egg-info/SOURCES.txt` & `gpt-researcher-0.4.2/gpt_researcher.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.4.1/pyproject.toml` & `gpt-researcher-0.4.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.4.1/setup.py` & `gpt-researcher-0.4.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = f.read()
 
 with open("requirements.txt", "r") as f:
     reqs = [line.strip() for line in f if ('selenium' not in line and 'webdriver' not in line)]
 
 setup(
     name="gpt-researcher",
-    version="0.4.1",
+    version="0.4.2",
     description="GPT Researcher is an autonomous agent designed for comprehensive online research on a variety of tasks.",
     package_dir={'gpt_researcher': 'gpt_researcher'},
     packages=find_packages(),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/assafelovic/gpt-researcher",
     author="Assaf Elovic",
```

