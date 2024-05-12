# Comparing `tmp/gpt-researcher-0.4.0.tar.gz` & `tmp/gpt-researcher-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt-researcher-0.4.0.tar", last modified: Fri May 10 05:40:12 2024, max compression
+gzip compressed data, was "gpt-researcher-0.4.1.tar", last modified: Sun May 12 07:07:43 2024, max compression
```

## Comparing `gpt-researcher-0.4.0.tar` & `gpt-researcher-0.4.1.tar`

### file list

```diff
@@ -1,103 +1,103 @@
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-10 05:40:12.311574 gpt-researcher-0.4.0/
--rw-r--r--   0 assafel    (501) staff       (20)     1069 2024-04-22 11:21:41.000000 gpt-researcher-0.4.0/LICENSE
--rw-r--r--   0 assafel    (501) staff       (20)    10742 2024-05-10 05:40:12.310802 gpt-researcher-0.4.0/PKG-INFO
--rw-r--r--   0 assafel    (501) staff       (20)    10019 2024-05-10 05:38:04.000000 gpt-researcher-0.4.0/README.md
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-10 05:40:12.244535 gpt-researcher-0.4.0/backend/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.4.0/backend/__init__.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-10 05:40:12.245882 gpt-researcher-0.4.0/backend/report_type/
--rw-r--r--   0 assafel    (501) staff       (20)      165 2024-04-22 11:21:41.000000 gpt-researcher-0.4.0/backend/report_type/__init__.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-10 05:40:12.247496 gpt-researcher-0.4.0/backend/report_type/basic_report/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.4.0/backend/report_type/basic_report/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)      777 2024-04-22 11:21:41.000000 gpt-researcher-0.4.0/backend/report_type/basic_report/basic_report.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-10 05:40:12.248993 gpt-researcher-0.4.0/backend/report_type/detailed_report/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.4.0/backend/report_type/detailed_report/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     6012 2024-04-22 11:21:41.000000 gpt-researcher-0.4.0/backend/report_type/detailed_report/detailed_report.py
--rw-r--r--   0 assafel    (501) staff       (20)     2327 2024-04-30 14:44:06.000000 gpt-researcher-0.4.0/backend/server.py
--rw-r--r--   0 assafel    (501) staff       (20)     2689 2024-04-30 14:43:31.000000 gpt-researcher-0.4.0/backend/utils.py
--rw-r--r--   0 assafel    (501) staff       (20)     2822 2024-04-22 11:21:41.000000 gpt-researcher-0.4.0/backend/websocket_manager.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-10 05:40:12.250090 gpt-researcher-0.4.0/gpt_researcher/
--rw-r--r--   0 assafel    (501) staff       (20)      100 2023-11-13 18:29:19.000000 gpt-researcher-0.4.0/gpt_researcher/__init__.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-10 05:40:12.255190 gpt-researcher-0.4.0/gpt_researcher/config/
--rw-r--r--   0 assafel    (501) staff       (20)       48 2023-11-13 18:29:19.000000 gpt-researcher-0.4.0/gpt_researcher/config/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     2094 2024-04-22 11:21:41.000000 gpt-researcher-0.4.0/gpt_researcher/config/config.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-10 05:40:12.258223 gpt-researcher-0.4.0/gpt_researcher/context/
--rw-r--r--   0 assafel    (501) staff       (20)      140 2023-11-19 07:01:11.000000 gpt-researcher-0.4.0/gpt_researcher/context/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     1796 2024-05-09 12:40:13.000000 gpt-researcher-0.4.0/gpt_researcher/context/compression.py
--rw-r--r--   0 assafel    (501) staff       (20)      801 2023-11-19 07:01:11.000000 gpt-researcher-0.4.0/gpt_researcher/context/retriever.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-10 05:40:12.259148 gpt-researcher-0.4.0/gpt_researcher/llm_provider/
--rw-r--r--   0 assafel    (501) staff       (20)      226 2024-04-22 11:21:41.000000 gpt-researcher-0.4.0/gpt_researcher/llm_provider/__init__.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-10 05:40:12.260674 gpt-researcher-0.4.0/gpt_researcher/llm_provider/azureopenai/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.4.0/gpt_researcher/llm_provider/azureopenai/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     3068 2024-04-22 11:21:41.000000 gpt-researcher-0.4.0/gpt_researcher/llm_provider/azureopenai/azureopenai.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-10 05:40:12.262613 gpt-researcher-0.4.0/gpt_researcher/llm_provider/google/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.4.0/gpt_researcher/llm_provider/google/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     3670 2024-04-22 11:21:41.000000 gpt-researcher-0.4.0/gpt_researcher/llm_provider/google/google.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-10 05:40:12.264787 gpt-researcher-0.4.0/gpt_researcher/llm_provider/openai/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.4.0/gpt_researcher/llm_provider/openai/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     2450 2024-05-08 07:24:47.000000 gpt-researcher-0.4.0/gpt_researcher/llm_provider/openai/openai.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-10 05:40:12.270211 gpt-researcher-0.4.0/gpt_researcher/master/
--rw-r--r--   0 assafel    (501) staff       (20)       61 2023-11-13 18:29:19.000000 gpt-researcher-0.4.0/gpt_researcher/master/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     9331 2024-05-10 05:37:26.000000 gpt-researcher-0.4.0/gpt_researcher/master/agent.py
--rw-r--r--   0 assafel    (501) staff       (20)    12460 2024-05-08 07:24:47.000000 gpt-researcher-0.4.0/gpt_researcher/master/functions.py
--rw-r--r--   0 assafel    (501) staff       (20)    13398 2024-05-06 06:02:27.000000 gpt-researcher-0.4.0/gpt_researcher/master/prompts.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-10 05:40:12.273404 gpt-researcher-0.4.0/gpt_researcher/memory/
--rw-r--r--   0 assafel    (501) staff       (20)       31 2023-11-19 07:01:11.000000 gpt-researcher-0.4.0/gpt_researcher/memory/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     1077 2024-05-09 06:30:45.000000 gpt-researcher-0.4.0/gpt_researcher/memory/embeddings.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-10 05:40:12.274661 gpt-researcher-0.4.0/gpt_researcher/retrievers/
--rw-r--r--   0 assafel    (501) staff       (20)      510 2023-12-18 08:18:37.000000 gpt-researcher-0.4.0/gpt_researcher/retrievers/__init__.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-10 05:40:12.276666 gpt-researcher-0.4.0/gpt_researcher/retrievers/bing/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2023-12-08 11:24:31.000000 gpt-researcher-0.4.0/gpt_researcher/retrievers/bing/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     2240 2023-12-08 11:24:31.000000 gpt-researcher-0.4.0/gpt_researcher/retrievers/bing/bing.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-10 05:40:12.278665 gpt-researcher-0.4.0/gpt_researcher/retrievers/duckduckgo/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.4.0/gpt_researcher/retrievers/duckduckgo/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)      479 2024-05-06 05:46:56.000000 gpt-researcher-0.4.0/gpt_researcher/retrievers/duckduckgo/duckduckgo.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-10 05:40:12.280248 gpt-researcher-0.4.0/gpt_researcher/retrievers/google/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.4.0/gpt_researcher/retrievers/google/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     2535 2023-11-19 07:01:11.000000 gpt-researcher-0.4.0/gpt_researcher/retrievers/google/google.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-10 05:40:12.282224 gpt-researcher-0.4.0/gpt_researcher/retrievers/searx/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.4.0/gpt_researcher/retrievers/searx/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     1294 2024-04-22 11:21:41.000000 gpt-researcher-0.4.0/gpt_researcher/retrievers/searx/searx.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-10 05:40:12.284350 gpt-researcher-0.4.0/gpt_researcher/retrievers/serpapi/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.4.0/gpt_researcher/retrievers/serpapi/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     2232 2023-11-25 13:46:26.000000 gpt-researcher-0.4.0/gpt_researcher/retrievers/serpapi/serpapi.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-10 05:40:12.286997 gpt-researcher-0.4.0/gpt_researcher/retrievers/serper/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.4.0/gpt_researcher/retrievers/serper/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     2117 2023-11-25 13:46:26.000000 gpt-researcher-0.4.0/gpt_researcher/retrievers/serper/serper.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-10 05:40:12.288977 gpt-researcher-0.4.0/gpt_researcher/retrievers/tavily_news/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2023-12-18 08:18:37.000000 gpt-researcher-0.4.0/gpt_researcher/retrievers/tavily_news/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     1281 2023-12-18 08:18:37.000000 gpt-researcher-0.4.0/gpt_researcher/retrievers/tavily_news/tavily_news.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-10 05:40:12.291178 gpt-researcher-0.4.0/gpt_researcher/retrievers/tavily_search/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.4.0/gpt_researcher/retrievers/tavily_search/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     1675 2024-05-09 06:46:00.000000 gpt-researcher-0.4.0/gpt_researcher/retrievers/tavily_search/tavily_search.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-10 05:40:12.293632 gpt-researcher-0.4.0/gpt_researcher/scraper/
--rw-r--r--   0 assafel    (501) staff       (20)      398 2024-03-17 08:29:46.000000 gpt-researcher-0.4.0/gpt_researcher/scraper/__init__.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-10 05:40:12.295851 gpt-researcher-0.4.0/gpt_researcher/scraper/arxiv/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.4.0/gpt_researcher/scraper/arxiv/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)      762 2024-03-12 13:09:58.000000 gpt-researcher-0.4.0/gpt_researcher/scraper/arxiv/arxiv.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-10 05:40:12.298137 gpt-researcher-0.4.0/gpt_researcher/scraper/beautiful_soup/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.4.0/gpt_researcher/scraper/beautiful_soup/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     1992 2024-03-12 13:09:58.000000 gpt-researcher-0.4.0/gpt_researcher/scraper/beautiful_soup/beautiful_soup.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-10 05:40:12.300188 gpt-researcher-0.4.0/gpt_researcher/scraper/newspaper/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.4.0/gpt_researcher/scraper/newspaper/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     1312 2024-03-12 13:09:58.000000 gpt-researcher-0.4.0/gpt_researcher/scraper/newspaper/newspaper.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-10 05:40:12.302231 gpt-researcher-0.4.0/gpt_researcher/scraper/pymupdf/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.4.0/gpt_researcher/scraper/pymupdf/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)      640 2024-03-12 13:09:58.000000 gpt-researcher-0.4.0/gpt_researcher/scraper/pymupdf/pymupdf.py
--rw-r--r--   0 assafel    (501) staff       (20)     3111 2024-03-17 08:29:46.000000 gpt-researcher-0.4.0/gpt_researcher/scraper/scraper.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-10 05:40:12.304395 gpt-researcher-0.4.0/gpt_researcher/scraper/web_base_loader/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.4.0/gpt_researcher/scraper/web_base_loader/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     1074 2024-03-12 13:09:58.000000 gpt-researcher-0.4.0/gpt_researcher/scraper/web_base_loader/web_base_loader.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-10 05:40:12.309239 gpt-researcher-0.4.0/gpt_researcher/utils/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.4.0/gpt_researcher/utils/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)      274 2024-04-22 11:21:41.000000 gpt-researcher-0.4.0/gpt_researcher/utils/enum.py
--rw-r--r--   0 assafel    (501) staff       (20)     5108 2024-04-22 11:21:41.000000 gpt-researcher-0.4.0/gpt_researcher/utils/llm.py
--rw-r--r--   0 assafel    (501) staff       (20)      216 2024-04-22 11:21:41.000000 gpt-researcher-0.4.0/gpt_researcher/utils/validators.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-10 05:40:12.253625 gpt-researcher-0.4.0/gpt_researcher.egg-info/
--rw-r--r--   0 assafel    (501) staff       (20)    10742 2024-05-10 05:40:12.000000 gpt-researcher-0.4.0/gpt_researcher.egg-info/PKG-INFO
--rw-r--r--   0 assafel    (501) staff       (20)     2727 2024-05-10 05:40:12.000000 gpt-researcher-0.4.0/gpt_researcher.egg-info/SOURCES.txt
--rw-r--r--   0 assafel    (501) staff       (20)        1 2024-05-10 05:40:12.000000 gpt-researcher-0.4.0/gpt_researcher.egg-info/dependency_links.txt
--rw-r--r--   0 assafel    (501) staff       (20)      342 2024-05-10 05:40:12.000000 gpt-researcher-0.4.0/gpt_researcher.egg-info/requires.txt
--rw-r--r--   0 assafel    (501) staff       (20)       23 2024-05-10 05:40:12.000000 gpt-researcher-0.4.0/gpt_researcher.egg-info/top_level.txt
--rw-r--r--   0 assafel    (501) staff       (20)     1156 2024-04-27 17:11:32.000000 gpt-researcher-0.4.0/pyproject.toml
--rw-r--r--   0 assafel    (501) staff       (20)       38 2024-05-10 05:40:12.311797 gpt-researcher-0.4.0/setup.cfg
--rw-r--r--   0 assafel    (501) staff       (20)     1176 2024-05-10 05:39:51.000000 gpt-researcher-0.4.0/setup.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-12 07:07:43.655246 gpt-researcher-0.4.1/
+-rw-r--r--   0 assafel    (501) staff       (20)     1069 2024-04-22 11:21:41.000000 gpt-researcher-0.4.1/LICENSE
+-rw-r--r--   0 assafel    (501) staff       (20)    11566 2024-05-12 07:07:43.654761 gpt-researcher-0.4.1/PKG-INFO
+-rw-r--r--   0 assafel    (501) staff       (20)    10843 2024-05-12 06:41:48.000000 gpt-researcher-0.4.1/README.md
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-12 07:07:43.612336 gpt-researcher-0.4.1/backend/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.4.1/backend/__init__.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-12 07:07:43.613129 gpt-researcher-0.4.1/backend/report_type/
+-rw-r--r--   0 assafel    (501) staff       (20)      165 2024-04-22 11:21:41.000000 gpt-researcher-0.4.1/backend/report_type/__init__.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-12 07:07:43.614721 gpt-researcher-0.4.1/backend/report_type/basic_report/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.4.1/backend/report_type/basic_report/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)      777 2024-04-22 11:21:41.000000 gpt-researcher-0.4.1/backend/report_type/basic_report/basic_report.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-12 07:07:43.616558 gpt-researcher-0.4.1/backend/report_type/detailed_report/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.4.1/backend/report_type/detailed_report/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     6012 2024-04-22 11:21:41.000000 gpt-researcher-0.4.1/backend/report_type/detailed_report/detailed_report.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2327 2024-04-30 14:44:06.000000 gpt-researcher-0.4.1/backend/server.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2689 2024-04-30 14:43:31.000000 gpt-researcher-0.4.1/backend/utils.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2822 2024-04-22 11:21:41.000000 gpt-researcher-0.4.1/backend/websocket_manager.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-12 07:07:43.617303 gpt-researcher-0.4.1/gpt_researcher/
+-rw-r--r--   0 assafel    (501) staff       (20)      100 2023-11-13 18:29:19.000000 gpt-researcher-0.4.1/gpt_researcher/__init__.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-12 07:07:43.622441 gpt-researcher-0.4.1/gpt_researcher/config/
+-rw-r--r--   0 assafel    (501) staff       (20)       48 2023-11-13 18:29:19.000000 gpt-researcher-0.4.1/gpt_researcher/config/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2114 2024-05-12 07:06:09.000000 gpt-researcher-0.4.1/gpt_researcher/config/config.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-12 07:07:43.624783 gpt-researcher-0.4.1/gpt_researcher/context/
+-rw-r--r--   0 assafel    (501) staff       (20)      140 2023-11-19 07:01:11.000000 gpt-researcher-0.4.1/gpt_researcher/context/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1796 2024-05-09 12:40:13.000000 gpt-researcher-0.4.1/gpt_researcher/context/compression.py
+-rw-r--r--   0 assafel    (501) staff       (20)      801 2023-11-19 07:01:11.000000 gpt-researcher-0.4.1/gpt_researcher/context/retriever.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-12 07:07:43.625491 gpt-researcher-0.4.1/gpt_researcher/llm_provider/
+-rw-r--r--   0 assafel    (501) staff       (20)      226 2024-04-22 11:21:41.000000 gpt-researcher-0.4.1/gpt_researcher/llm_provider/__init__.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-12 07:07:43.626513 gpt-researcher-0.4.1/gpt_researcher/llm_provider/azureopenai/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.4.1/gpt_researcher/llm_provider/azureopenai/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     3068 2024-04-22 11:21:41.000000 gpt-researcher-0.4.1/gpt_researcher/llm_provider/azureopenai/azureopenai.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-12 07:07:43.627849 gpt-researcher-0.4.1/gpt_researcher/llm_provider/google/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.4.1/gpt_researcher/llm_provider/google/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     3670 2024-04-22 11:21:41.000000 gpt-researcher-0.4.1/gpt_researcher/llm_provider/google/google.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-12 07:07:43.629465 gpt-researcher-0.4.1/gpt_researcher/llm_provider/openai/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.4.1/gpt_researcher/llm_provider/openai/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2450 2024-05-08 07:24:47.000000 gpt-researcher-0.4.1/gpt_researcher/llm_provider/openai/openai.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-12 07:07:43.632017 gpt-researcher-0.4.1/gpt_researcher/master/
+-rw-r--r--   0 assafel    (501) staff       (20)       61 2023-11-13 18:29:19.000000 gpt-researcher-0.4.1/gpt_researcher/master/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     9331 2024-05-10 05:37:26.000000 gpt-researcher-0.4.1/gpt_researcher/master/agent.py
+-rw-r--r--   0 assafel    (501) staff       (20)    12460 2024-05-08 07:24:47.000000 gpt-researcher-0.4.1/gpt_researcher/master/functions.py
+-rw-r--r--   0 assafel    (501) staff       (20)    13398 2024-05-06 06:02:27.000000 gpt-researcher-0.4.1/gpt_researcher/master/prompts.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-12 07:07:43.633344 gpt-researcher-0.4.1/gpt_researcher/memory/
+-rw-r--r--   0 assafel    (501) staff       (20)       31 2023-11-19 07:01:11.000000 gpt-researcher-0.4.1/gpt_researcher/memory/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1077 2024-05-09 06:30:45.000000 gpt-researcher-0.4.1/gpt_researcher/memory/embeddings.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-12 07:07:43.634396 gpt-researcher-0.4.1/gpt_researcher/retrievers/
+-rw-r--r--   0 assafel    (501) staff       (20)      510 2023-12-18 08:18:37.000000 gpt-researcher-0.4.1/gpt_researcher/retrievers/__init__.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-12 07:07:43.635455 gpt-researcher-0.4.1/gpt_researcher/retrievers/bing/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2023-12-08 11:24:31.000000 gpt-researcher-0.4.1/gpt_researcher/retrievers/bing/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2240 2023-12-08 11:24:31.000000 gpt-researcher-0.4.1/gpt_researcher/retrievers/bing/bing.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-12 07:07:43.636488 gpt-researcher-0.4.1/gpt_researcher/retrievers/duckduckgo/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.4.1/gpt_researcher/retrievers/duckduckgo/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)      479 2024-05-06 05:46:56.000000 gpt-researcher-0.4.1/gpt_researcher/retrievers/duckduckgo/duckduckgo.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-12 07:07:43.637930 gpt-researcher-0.4.1/gpt_researcher/retrievers/google/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.4.1/gpt_researcher/retrievers/google/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2535 2023-11-19 07:01:11.000000 gpt-researcher-0.4.1/gpt_researcher/retrievers/google/google.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-12 07:07:43.639167 gpt-researcher-0.4.1/gpt_researcher/retrievers/searx/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.4.1/gpt_researcher/retrievers/searx/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1294 2024-04-22 11:21:41.000000 gpt-researcher-0.4.1/gpt_researcher/retrievers/searx/searx.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-12 07:07:43.640329 gpt-researcher-0.4.1/gpt_researcher/retrievers/serpapi/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.4.1/gpt_researcher/retrievers/serpapi/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2232 2023-11-25 13:46:26.000000 gpt-researcher-0.4.1/gpt_researcher/retrievers/serpapi/serpapi.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-12 07:07:43.641893 gpt-researcher-0.4.1/gpt_researcher/retrievers/serper/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.4.1/gpt_researcher/retrievers/serper/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2117 2023-11-25 13:46:26.000000 gpt-researcher-0.4.1/gpt_researcher/retrievers/serper/serper.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-12 07:07:43.643088 gpt-researcher-0.4.1/gpt_researcher/retrievers/tavily_news/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2023-12-18 08:18:37.000000 gpt-researcher-0.4.1/gpt_researcher/retrievers/tavily_news/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1281 2023-12-18 08:18:37.000000 gpt-researcher-0.4.1/gpt_researcher/retrievers/tavily_news/tavily_news.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-12 07:07:43.644083 gpt-researcher-0.4.1/gpt_researcher/retrievers/tavily_search/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.4.1/gpt_researcher/retrievers/tavily_search/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1675 2024-05-09 06:46:00.000000 gpt-researcher-0.4.1/gpt_researcher/retrievers/tavily_search/tavily_search.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-12 07:07:43.645643 gpt-researcher-0.4.1/gpt_researcher/scraper/
+-rw-r--r--   0 assafel    (501) staff       (20)      398 2024-03-17 08:29:46.000000 gpt-researcher-0.4.1/gpt_researcher/scraper/__init__.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-12 07:07:43.646750 gpt-researcher-0.4.1/gpt_researcher/scraper/arxiv/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.4.1/gpt_researcher/scraper/arxiv/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)      762 2024-03-12 13:09:58.000000 gpt-researcher-0.4.1/gpt_researcher/scraper/arxiv/arxiv.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-12 07:07:43.647786 gpt-researcher-0.4.1/gpt_researcher/scraper/beautiful_soup/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.4.1/gpt_researcher/scraper/beautiful_soup/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1992 2024-03-12 13:09:58.000000 gpt-researcher-0.4.1/gpt_researcher/scraper/beautiful_soup/beautiful_soup.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-12 07:07:43.648797 gpt-researcher-0.4.1/gpt_researcher/scraper/newspaper/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.4.1/gpt_researcher/scraper/newspaper/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1312 2024-03-12 13:09:58.000000 gpt-researcher-0.4.1/gpt_researcher/scraper/newspaper/newspaper.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-12 07:07:43.650199 gpt-researcher-0.4.1/gpt_researcher/scraper/pymupdf/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.4.1/gpt_researcher/scraper/pymupdf/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)      640 2024-03-12 13:09:58.000000 gpt-researcher-0.4.1/gpt_researcher/scraper/pymupdf/pymupdf.py
+-rw-r--r--   0 assafel    (501) staff       (20)     3111 2024-03-17 08:29:46.000000 gpt-researcher-0.4.1/gpt_researcher/scraper/scraper.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-12 07:07:43.651427 gpt-researcher-0.4.1/gpt_researcher/scraper/web_base_loader/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.4.1/gpt_researcher/scraper/web_base_loader/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1074 2024-03-12 13:09:58.000000 gpt-researcher-0.4.1/gpt_researcher/scraper/web_base_loader/web_base_loader.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-12 07:07:43.654037 gpt-researcher-0.4.1/gpt_researcher/utils/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.4.1/gpt_researcher/utils/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)      274 2024-04-22 11:21:41.000000 gpt-researcher-0.4.1/gpt_researcher/utils/enum.py
+-rw-r--r--   0 assafel    (501) staff       (20)     5108 2024-04-22 11:21:41.000000 gpt-researcher-0.4.1/gpt_researcher/utils/llm.py
+-rw-r--r--   0 assafel    (501) staff       (20)      216 2024-04-22 11:21:41.000000 gpt-researcher-0.4.1/gpt_researcher/utils/validators.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-12 07:07:43.620799 gpt-researcher-0.4.1/gpt_researcher.egg-info/
+-rw-r--r--   0 assafel    (501) staff       (20)    11566 2024-05-12 07:07:43.000000 gpt-researcher-0.4.1/gpt_researcher.egg-info/PKG-INFO
+-rw-r--r--   0 assafel    (501) staff       (20)     2727 2024-05-12 07:07:43.000000 gpt-researcher-0.4.1/gpt_researcher.egg-info/SOURCES.txt
+-rw-r--r--   0 assafel    (501) staff       (20)        1 2024-05-12 07:07:43.000000 gpt-researcher-0.4.1/gpt_researcher.egg-info/dependency_links.txt
+-rw-r--r--   0 assafel    (501) staff       (20)      342 2024-05-12 07:07:43.000000 gpt-researcher-0.4.1/gpt_researcher.egg-info/requires.txt
+-rw-r--r--   0 assafel    (501) staff       (20)       23 2024-05-12 07:07:43.000000 gpt-researcher-0.4.1/gpt_researcher.egg-info/top_level.txt
+-rw-r--r--   0 assafel    (501) staff       (20)     1156 2024-04-27 17:11:32.000000 gpt-researcher-0.4.1/pyproject.toml
+-rw-r--r--   0 assafel    (501) staff       (20)       38 2024-05-12 07:07:43.655432 gpt-researcher-0.4.1/setup.cfg
+-rw-r--r--   0 assafel    (501) staff       (20)     1176 2024-05-12 07:07:20.000000 gpt-researcher-0.4.1/setup.py
```

### Comparing `gpt-researcher-0.4.0/LICENSE` & `gpt-researcher-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.4.0/PKG-INFO` & `gpt-researcher-0.4.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,7 @@
-Metadata-Version: 2.1
-Name: gpt-researcher
-Version: 0.4.0
-Summary: GPT Researcher is an autonomous agent designed for comprehensive online research on a variety of tasks.
-Home-page: https://github.com/assafelovic/gpt-researcher
-Author: Assaf Elovic
-Author-email: assaf.elovic@gmail.com
-License: MIT
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Education
-Classifier: Intended Audience :: Science/Research
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # 🔎 GPT Researcher
 [![Official Website](https://img.shields.io/badge/Official%20Website-gptr.dev-blue?style=for-the-badge&logo=world&logoColor=white)](https://gptr.dev)
 [![Discord Follow](https://dcbadge.vercel.app/api/server/2pFkc83fRq?style=for-the-badge)](https://discord.com/invite/2pFkc83fRq)
 
 [![GitHub Repo stars](https://img.shields.io/github/stars/assafelovic/gpt-researcher?style=social)](https://github.com/assafelovic/gpt-researcher)
 [![Twitter Follow](https://img.shields.io/twitter/follow/assaf_elovic?style=social)](https://twitter.com/assaf_elovic)
 [![PyPI version](https://badge.fury.io/py/gpt-researcher.svg)](https://badge.fury.io/py/gpt-researcher)
@@ -102,20 +84,15 @@
 For Linux/Windows temporary setup, use the export method:
 
 ```bash
 export OPENAI_API_KEY={Your OpenAI API Key here}
 export TAVILY_API_KEY={Your Tavily API Key here}
 ```
 
-For a more permanent setup, create a `.env` file in the current `gpt-researcher` directory and input the keys as follows:
-
-```bash
-OPENAI_API_KEY={Your OpenAI API Key here}
-TAVILY_API_KEY={Your Tavily API Key here}
-```
+For a more permanent setup, create a `.env` file in the current `gpt-researcher` directory and input the env vars (without `export`).
 
 - **For LLM, we recommend [OpenAI GPT](https://platform.openai.com/docs/guides/gpt)**, but you can use any other LLM model (including open sources) supported by [Langchain Adapter](https://python.langchain.com/docs/integrations/adapters/openai/), simply change the llm model and provider in config/config.py. 
 - **For web search API, we recommend [Tavily Search API](https://app.tavily.com)**, but you can also refer to other search APIs of your choice by changing the search provider in config/config.py to `"duckduckgo"`, `"googleAPI"`, `"bing"`, `"googleSerp"`, `"searx"` and more. Then add the corresponding env API key as seen in the config.py file.
 
 ### Quickstart
 
 > **Step 1** - Install dependencies
@@ -143,30 +120,38 @@
 
 ```python
 from gpt_researcher import GPTResearcher
 
 query = "why is Nvidia stock going up?"
 researcher = GPTResearcher(query=query, report_type="research_report")
 # Conduct research on the given query
-research_data = await researcher.conduct_research()
+research_result = await researcher.conduct_research()
 # Write the report
 report = await researcher.write_report()
 ```
 
 **For more examples and configurations, please refer to the [PIP documentation](https://docs.tavily.com/docs/gpt-researcher/pip-package) page.**
 
+## 👪 Multi-Agent Assistant
+As AI evolves from prompt engineering and RAG to multi-agent systems, we're excited to introduce our new multi-agent assistant built with [LangGraph](https://python.langchain.com/v0.1/docs/langgraph/).
+
+By using LangGraph, the research process can be significantly improved in depth and quality by leveraging multiple agents with specialized skills. Inspired by the recent [STORM](https://arxiv.org/abs/2402.14207) paper, this project showcases how a team of AI agents can work together to conduct research on a given topic, from planning to publication.
+
+An average run generates a 5-6 page research report in multiple formats such as PDF, Docx and Markdown.
+
+Check it out [here](https://github.com/assafelovic/gpt-researcher/tree/master/multi_agents) or head over to our [documentation](https://docs.tavily.com/docs/gpt-researcher/agent_frameworks) for more information.
 
 ## 🚀 Contributing
 We highly welcome contributions! Please check out [contributing](https://github.com/assafelovic/gpt-researcher/blob/master/CONTRIBUTING.md) if you're interested.
 
 Please check out our [roadmap](https://trello.com/b/3O7KBePw/gpt-researcher-roadmap) page and reach out to us via our [Discord community](https://discord.gg/2pFkc83fRq) if you're interested in joining our mission.
 
 ## ✉️ Support / Contact us
 - [Community Discord](https://discord.gg/spBgZmm3Xe)
-- Our email: assafelovic@gmail.com
+- Author Email: assaf.elovic@gmail.com
 
 ## 🛡 Disclaimer
 
 This project, GPT Researcher, is an experimental application and is provided "as-is" without any warranty, express or implied. We are sharing codes for academic purposes under the MIT license. Nothing herein is academic advice, and NOT a recommendation to use in academic or research papers.
 
 Our view on unbiased research claims:
 1. The main goal of GPT Researcher is to reduce incorrect and biased facts. How? We assume that the more sites we scrape the less chances of incorrect data. By scraping over 20 sites per research, and choosing the most frequent information, the chances that they are all wrong is extremely low.
```

### Comparing `gpt-researcher-0.4.0/README.md` & `gpt-researcher-0.4.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+Metadata-Version: 2.1
+Name: gpt-researcher
+Version: 0.4.1
+Summary: GPT Researcher is an autonomous agent designed for comprehensive online research on a variety of tasks.
+Home-page: https://github.com/assafelovic/gpt-researcher
+Author: Assaf Elovic
+Author-email: assaf.elovic@gmail.com
+License: MIT
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Education
+Classifier: Intended Audience :: Science/Research
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # 🔎 GPT Researcher
 [![Official Website](https://img.shields.io/badge/Official%20Website-gptr.dev-blue?style=for-the-badge&logo=world&logoColor=white)](https://gptr.dev)
 [![Discord Follow](https://dcbadge.vercel.app/api/server/2pFkc83fRq?style=for-the-badge)](https://discord.com/invite/2pFkc83fRq)
 
 [![GitHub Repo stars](https://img.shields.io/github/stars/assafelovic/gpt-researcher?style=social)](https://github.com/assafelovic/gpt-researcher)
 [![Twitter Follow](https://img.shields.io/twitter/follow/assaf_elovic?style=social)](https://twitter.com/assaf_elovic)
 [![PyPI version](https://badge.fury.io/py/gpt-researcher.svg)](https://badge.fury.io/py/gpt-researcher)
@@ -84,20 +102,15 @@
 For Linux/Windows temporary setup, use the export method:
 
 ```bash
 export OPENAI_API_KEY={Your OpenAI API Key here}
 export TAVILY_API_KEY={Your Tavily API Key here}
 ```
 
-For a more permanent setup, create a `.env` file in the current `gpt-researcher` directory and input the keys as follows:
-
-```bash
-OPENAI_API_KEY={Your OpenAI API Key here}
-TAVILY_API_KEY={Your Tavily API Key here}
-```
+For a more permanent setup, create a `.env` file in the current `gpt-researcher` directory and input the env vars (without `export`).
 
 - **For LLM, we recommend [OpenAI GPT](https://platform.openai.com/docs/guides/gpt)**, but you can use any other LLM model (including open sources) supported by [Langchain Adapter](https://python.langchain.com/docs/integrations/adapters/openai/), simply change the llm model and provider in config/config.py. 
 - **For web search API, we recommend [Tavily Search API](https://app.tavily.com)**, but you can also refer to other search APIs of your choice by changing the search provider in config/config.py to `"duckduckgo"`, `"googleAPI"`, `"bing"`, `"googleSerp"`, `"searx"` and more. Then add the corresponding env API key as seen in the config.py file.
 
 ### Quickstart
 
 > **Step 1** - Install dependencies
@@ -125,30 +138,38 @@
 
 ```python
 from gpt_researcher import GPTResearcher
 
 query = "why is Nvidia stock going up?"
 researcher = GPTResearcher(query=query, report_type="research_report")
 # Conduct research on the given query
-research_data = await researcher.conduct_research()
+research_result = await researcher.conduct_research()
 # Write the report
 report = await researcher.write_report()
 ```
 
 **For more examples and configurations, please refer to the [PIP documentation](https://docs.tavily.com/docs/gpt-researcher/pip-package) page.**
 
+## 👪 Multi-Agent Assistant
+As AI evolves from prompt engineering and RAG to multi-agent systems, we're excited to introduce our new multi-agent assistant built with [LangGraph](https://python.langchain.com/v0.1/docs/langgraph/).
+
+By using LangGraph, the research process can be significantly improved in depth and quality by leveraging multiple agents with specialized skills. Inspired by the recent [STORM](https://arxiv.org/abs/2402.14207) paper, this project showcases how a team of AI agents can work together to conduct research on a given topic, from planning to publication.
+
+An average run generates a 5-6 page research report in multiple formats such as PDF, Docx and Markdown.
+
+Check it out [here](https://github.com/assafelovic/gpt-researcher/tree/master/multi_agents) or head over to our [documentation](https://docs.tavily.com/docs/gpt-researcher/agent_frameworks) for more information.
 
 ## 🚀 Contributing
 We highly welcome contributions! Please check out [contributing](https://github.com/assafelovic/gpt-researcher/blob/master/CONTRIBUTING.md) if you're interested.
 
 Please check out our [roadmap](https://trello.com/b/3O7KBePw/gpt-researcher-roadmap) page and reach out to us via our [Discord community](https://discord.gg/2pFkc83fRq) if you're interested in joining our mission.
 
 ## ✉️ Support / Contact us
 - [Community Discord](https://discord.gg/spBgZmm3Xe)
-- Our email: assafelovic@gmail.com
+- Author Email: assaf.elovic@gmail.com
 
 ## 🛡 Disclaimer
 
 This project, GPT Researcher, is an experimental application and is provided "as-is" without any warranty, express or implied. We are sharing codes for academic purposes under the MIT license. Nothing herein is academic advice, and NOT a recommendation to use in academic or research papers.
 
 Our view on unbiased research claims:
 1. The main goal of GPT Researcher is to reduce incorrect and biased facts. How? We assume that the more sites we scrape the less chances of incorrect data. By scraping over 20 sites per research, and choosing the most frequent information, the chances that they are all wrong is extremely low.
```

### Comparing `gpt-researcher-0.4.0/backend/report_type/basic_report/basic_report.py` & `gpt-researcher-0.4.1/backend/report_type/basic_report/basic_report.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.4.0/backend/report_type/detailed_report/detailed_report.py` & `gpt-researcher-0.4.1/backend/report_type/detailed_report/detailed_report.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.4.0/backend/server.py` & `gpt-researcher-0.4.1/backend/server.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.4.0/backend/utils.py` & `gpt-researcher-0.4.1/backend/utils.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.4.0/backend/websocket_manager.py` & `gpt-researcher-0.4.1/backend/websocket_manager.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.4.0/gpt_researcher/config/config.py` & `gpt-researcher-0.4.1/gpt_researcher/config/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 class Config:
     """Config class for GPT Researcher."""
 
     def __init__(self, config_file: str = None):
         """Initialize the config class."""
-        self.config_file = config_file if config_file else os.getenv('CONFIG_FILE')
+        self.config_file = os.path.expanduser(config_file) if config_file else os.getenv('CONFIG_FILE')
         self.retriever = os.getenv('SEARCH_RETRIEVER', "tavily")
         self.embedding_provider = os.getenv('EMBEDDING_PROVIDER', 'openai')
         self.llm_provider = os.getenv('LLM_PROVIDER', "openai")
         self.fast_llm_model = os.getenv('FAST_LLM_MODEL', "gpt-3.5-turbo-16k")
         self.smart_llm_model = os.getenv('SMART_LLM_MODEL', "gpt-4-turbo")
         self.fast_token_limit = int(os.getenv('FAST_TOKEN_LIMIT', 2000))
         self.smart_token_limit = int(os.getenv('SMART_TOKEN_LIMIT', 4000))
```

### Comparing `gpt-researcher-0.4.0/gpt_researcher/context/compression.py` & `gpt-researcher-0.4.1/gpt_researcher/context/compression.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.4.0/gpt_researcher/context/retriever.py` & `gpt-researcher-0.4.1/gpt_researcher/context/retriever.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.4.0/gpt_researcher/llm_provider/azureopenai/azureopenai.py` & `gpt-researcher-0.4.1/gpt_researcher/llm_provider/azureopenai/azureopenai.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.4.0/gpt_researcher/llm_provider/google/google.py` & `gpt-researcher-0.4.1/gpt_researcher/llm_provider/google/google.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.4.0/gpt_researcher/llm_provider/openai/openai.py` & `gpt-researcher-0.4.1/gpt_researcher/llm_provider/openai/openai.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.4.0/gpt_researcher/master/agent.py` & `gpt-researcher-0.4.1/gpt_researcher/master/agent.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.4.0/gpt_researcher/master/functions.py` & `gpt-researcher-0.4.1/gpt_researcher/master/functions.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.4.0/gpt_researcher/master/prompts.py` & `gpt-researcher-0.4.1/gpt_researcher/master/prompts.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.4.0/gpt_researcher/memory/embeddings.py` & `gpt-researcher-0.4.1/gpt_researcher/memory/embeddings.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.4.0/gpt_researcher/retrievers/bing/bing.py` & `gpt-researcher-0.4.1/gpt_researcher/retrievers/bing/bing.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.4.0/gpt_researcher/retrievers/google/google.py` & `gpt-researcher-0.4.1/gpt_researcher/retrievers/google/google.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.4.0/gpt_researcher/retrievers/searx/searx.py` & `gpt-researcher-0.4.1/gpt_researcher/retrievers/searx/searx.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.4.0/gpt_researcher/retrievers/serpapi/serpapi.py` & `gpt-researcher-0.4.1/gpt_researcher/retrievers/serpapi/serpapi.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.4.0/gpt_researcher/retrievers/serper/serper.py` & `gpt-researcher-0.4.1/gpt_researcher/retrievers/serper/serper.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.4.0/gpt_researcher/retrievers/tavily_news/tavily_news.py` & `gpt-researcher-0.4.1/gpt_researcher/retrievers/tavily_news/tavily_news.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.4.0/gpt_researcher/retrievers/tavily_search/tavily_search.py` & `gpt-researcher-0.4.1/gpt_researcher/retrievers/tavily_search/tavily_search.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.4.0/gpt_researcher/scraper/arxiv/arxiv.py` & `gpt-researcher-0.4.1/gpt_researcher/scraper/arxiv/arxiv.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.4.0/gpt_researcher/scraper/beautiful_soup/beautiful_soup.py` & `gpt-researcher-0.4.1/gpt_researcher/scraper/beautiful_soup/beautiful_soup.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.4.0/gpt_researcher/scraper/newspaper/newspaper.py` & `gpt-researcher-0.4.1/gpt_researcher/scraper/newspaper/newspaper.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.4.0/gpt_researcher/scraper/pymupdf/pymupdf.py` & `gpt-researcher-0.4.1/gpt_researcher/scraper/pymupdf/pymupdf.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.4.0/gpt_researcher/scraper/scraper.py` & `gpt-researcher-0.4.1/gpt_researcher/scraper/scraper.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.4.0/gpt_researcher/scraper/web_base_loader/web_base_loader.py` & `gpt-researcher-0.4.1/gpt_researcher/scraper/web_base_loader/web_base_loader.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.4.0/gpt_researcher/utils/llm.py` & `gpt-researcher-0.4.1/gpt_researcher/utils/llm.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.4.0/gpt_researcher.egg-info/PKG-INFO` & `gpt-researcher-0.4.1/gpt_researcher.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-researcher
-Version: 0.4.0
+Version: 0.4.1
 Summary: GPT Researcher is an autonomous agent designed for comprehensive online research on a variety of tasks.
 Home-page: https://github.com/assafelovic/gpt-researcher
 Author: Assaf Elovic
 Author-email: assaf.elovic@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
@@ -102,20 +102,15 @@
 For Linux/Windows temporary setup, use the export method:
 
 ```bash
 export OPENAI_API_KEY={Your OpenAI API Key here}
 export TAVILY_API_KEY={Your Tavily API Key here}
 ```
 
-For a more permanent setup, create a `.env` file in the current `gpt-researcher` directory and input the keys as follows:
-
-```bash
-OPENAI_API_KEY={Your OpenAI API Key here}
-TAVILY_API_KEY={Your Tavily API Key here}
-```
+For a more permanent setup, create a `.env` file in the current `gpt-researcher` directory and input the env vars (without `export`).
 
 - **For LLM, we recommend [OpenAI GPT](https://platform.openai.com/docs/guides/gpt)**, but you can use any other LLM model (including open sources) supported by [Langchain Adapter](https://python.langchain.com/docs/integrations/adapters/openai/), simply change the llm model and provider in config/config.py. 
 - **For web search API, we recommend [Tavily Search API](https://app.tavily.com)**, but you can also refer to other search APIs of your choice by changing the search provider in config/config.py to `"duckduckgo"`, `"googleAPI"`, `"bing"`, `"googleSerp"`, `"searx"` and more. Then add the corresponding env API key as seen in the config.py file.
 
 ### Quickstart
 
 > **Step 1** - Install dependencies
@@ -143,30 +138,38 @@
 
 ```python
 from gpt_researcher import GPTResearcher
 
 query = "why is Nvidia stock going up?"
 researcher = GPTResearcher(query=query, report_type="research_report")
 # Conduct research on the given query
-research_data = await researcher.conduct_research()
+research_result = await researcher.conduct_research()
 # Write the report
 report = await researcher.write_report()
 ```
 
 **For more examples and configurations, please refer to the [PIP documentation](https://docs.tavily.com/docs/gpt-researcher/pip-package) page.**
 
+## 👪 Multi-Agent Assistant
+As AI evolves from prompt engineering and RAG to multi-agent systems, we're excited to introduce our new multi-agent assistant built with [LangGraph](https://python.langchain.com/v0.1/docs/langgraph/).
+
+By using LangGraph, the research process can be significantly improved in depth and quality by leveraging multiple agents with specialized skills. Inspired by the recent [STORM](https://arxiv.org/abs/2402.14207) paper, this project showcases how a team of AI agents can work together to conduct research on a given topic, from planning to publication.
+
+An average run generates a 5-6 page research report in multiple formats such as PDF, Docx and Markdown.
+
+Check it out [here](https://github.com/assafelovic/gpt-researcher/tree/master/multi_agents) or head over to our [documentation](https://docs.tavily.com/docs/gpt-researcher/agent_frameworks) for more information.
 
 ## 🚀 Contributing
 We highly welcome contributions! Please check out [contributing](https://github.com/assafelovic/gpt-researcher/blob/master/CONTRIBUTING.md) if you're interested.
 
 Please check out our [roadmap](https://trello.com/b/3O7KBePw/gpt-researcher-roadmap) page and reach out to us via our [Discord community](https://discord.gg/2pFkc83fRq) if you're interested in joining our mission.
 
 ## ✉️ Support / Contact us
 - [Community Discord](https://discord.gg/spBgZmm3Xe)
-- Our email: assafelovic@gmail.com
+- Author Email: assaf.elovic@gmail.com
 
 ## 🛡 Disclaimer
 
 This project, GPT Researcher, is an experimental application and is provided "as-is" without any warranty, express or implied. We are sharing codes for academic purposes under the MIT license. Nothing herein is academic advice, and NOT a recommendation to use in academic or research papers.
 
 Our view on unbiased research claims:
 1. The main goal of GPT Researcher is to reduce incorrect and biased facts. How? We assume that the more sites we scrape the less chances of incorrect data. By scraping over 20 sites per research, and choosing the most frequent information, the chances that they are all wrong is extremely low.
```

### Comparing `gpt-researcher-0.4.0/gpt_researcher.egg-info/SOURCES.txt` & `gpt-researcher-0.4.1/gpt_researcher.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.4.0/pyproject.toml` & `gpt-researcher-0.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.4.0/setup.py` & `gpt-researcher-0.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = f.read()
 
 with open("requirements.txt", "r") as f:
     reqs = [line.strip() for line in f if ('selenium' not in line and 'webdriver' not in line)]
 
 setup(
     name="gpt-researcher",
-    version="0.4.0",
+    version="0.4.1",
     description="GPT Researcher is an autonomous agent designed for comprehensive online research on a variety of tasks.",
     package_dir={'gpt_researcher': 'gpt_researcher'},
     packages=find_packages(),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/assafelovic/gpt-researcher",
     author="Assaf Elovic",
```

