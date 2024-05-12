# Comparing `tmp/ap0dl-1.5.2.tar.gz` & `tmp/ap0dl-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ap0dl-1.5.2.tar", max compression
+gzip compressed data, was "ap0dl-1.6.0.tar", max compression
```

## Comparing `ap0dl-1.5.2.tar` & `ap0dl-1.6.0.tar`

### file list

```diff
@@ -1,94 +1,101 @@
--rw-r--r--   0        0        0        0 2023-01-06 15:35:10.000000 ap0dl-1.5.2/ap0dl/__init__.py
--rw-r--r--   0        0        0     3140 2023-01-07 11:33:52.555402 ap0dl-1.5.2/ap0dl/__main__.py
--rw-r--r--   0        0        0       71 2023-01-06 15:35:10.000000 ap0dl-1.5.2/ap0dl/core/__init__.py
--rw-r--r--   0        0        0       18 2023-01-09 18:16:43.517984 ap0dl-1.5.2/ap0dl/core/__version__.py
--rw-r--r--   0        0        0        0 2023-01-06 15:35:10.000000 ap0dl-1.5.2/ap0dl/core/cli/__init__.py
--rw-r--r--   0        0        0        0 2023-01-06 15:35:10.000000 ap0dl-1.5.2/ap0dl/core/cli/commands/__init__.py
--rw-r--r--   0        0        0     4281 2023-01-07 09:58:31.791882 ap0dl-1.5.2/ap0dl/core/cli/commands/download.py
--rw-r--r--   0        0        0     1344 2023-01-07 09:58:11.276621 ap0dl-1.5.2/ap0dl/core/cli/commands/grab.py
--rw-r--r--   0        0        0     3272 2023-01-07 09:57:47.785786 ap0dl-1.5.2/ap0dl/core/cli/commands/schedule.py
--rw-r--r--   0        0        0     1644 2023-01-07 09:56:51.825422 ap0dl-1.5.2/ap0dl/core/cli/commands/search.py
--rw-r--r--   0        0        0     8451 2023-01-07 09:56:24.137795 ap0dl-1.5.2/ap0dl/core/cli/commands/stream.py
--rw-r--r--   0        0        0     3318 2023-01-07 09:55:40.163967 ap0dl-1.5.2/ap0dl/core/cli/commands/update.py
--rw-r--r--   0        0        0      112 2023-01-06 15:35:10.000000 ap0dl-1.5.2/ap0dl/core/cli/exit_codes.py
--rw-r--r--   0        0        0     4308 2023-01-06 15:35:10.000000 ap0dl-1.5.2/ap0dl/core/cli/helpers/__init__.py
--rw-r--r--   0        0        0     1762 2023-01-06 15:35:10.000000 ap0dl-1.5.2/ap0dl/core/cli/helpers/aniskip.py
--rw-r--r--   0        0        0     2313 2023-01-07 14:33:58.289567 ap0dl-1.5.2/ap0dl/core/cli/helpers/banner.py
--rw-r--r--   0        0        0      251 2023-01-07 10:49:06.101833 ap0dl-1.5.2/ap0dl/core/cli/helpers/constants.py
--rw-r--r--   0        0        0     4250 2023-01-06 15:35:10.000000 ap0dl-1.5.2/ap0dl/core/cli/helpers/decorators.py
--rw-r--r--   0        0        0     1093 2023-01-06 15:35:10.000000 ap0dl-1.5.2/ap0dl/core/cli/helpers/fuzzysearch.py
--rw-r--r--   0        0        0     6940 2023-01-06 15:35:10.000000 ap0dl-1.5.2/ap0dl/core/cli/helpers/intelliq.py
--rw-r--r--   0        0        0     2589 2023-01-06 15:35:10.000000 ap0dl-1.5.2/ap0dl/core/cli/helpers/logger.py
--rw-r--r--   0        0        0     1567 2023-01-06 15:35:10.000000 ap0dl-1.5.2/ap0dl/core/cli/helpers/player.py
--rw-r--r--   0        0        0      343 2023-01-06 15:35:10.000000 ap0dl-1.5.2/ap0dl/core/cli/helpers/players/__init__.py
--rw-r--r--   0        0        0      733 2023-01-06 15:35:10.000000 ap0dl-1.5.2/ap0dl/core/cli/helpers/players/android.py
--rw-r--r--   0        0        0     2094 2023-01-09 17:58:19.524086 ap0dl-1.5.2/ap0dl/core/cli/helpers/players/base_player.py
--rw-r--r--   0        0        0      713 2023-01-06 15:35:10.000000 ap0dl-1.5.2/ap0dl/core/cli/helpers/players/ffplay.py
--rw-r--r--   0        0        0     2498 2023-01-06 15:35:10.000000 ap0dl-1.5.2/ap0dl/core/cli/helpers/players/mpv.py
--rw-r--r--   0        0        0     1503 2023-01-06 15:35:10.000000 ap0dl-1.5.2/ap0dl/core/cli/helpers/players/vlc.py
--rw-r--r--   0        0        0     1429 2023-01-06 15:35:10.000000 ap0dl-1.5.2/ap0dl/core/cli/helpers/processors.py
--rw-r--r--   0        0        0     5612 2023-01-06 15:35:10.000000 ap0dl-1.5.2/ap0dl/core/cli/helpers/prompts.py
--rw-r--r--   0        0        0     3069 2023-01-07 13:37:31.983317 ap0dl-1.5.2/ap0dl/core/cli/helpers/rpc.py
--rw-r--r--   0        0        0     6525 2023-01-07 14:31:27.297179 ap0dl-1.5.2/ap0dl/core/cli/helpers/searcher.py
--rw-r--r--   0        0        0      895 2023-01-06 15:35:10.000000 ap0dl-1.5.2/ap0dl/core/cli/helpers/special.py
--rw-r--r--   0        0        0     2004 2023-01-06 15:35:10.000000 ap0dl-1.5.2/ap0dl/core/cli/helpers/stream_handlers.py
--rw-r--r--   0        0        0     1441 2023-01-09 18:02:32.421776 ap0dl-1.5.2/ap0dl/core/cli/http_client.py
--rw-r--r--   0        0        0       26 2023-01-06 15:35:10.000000 ap0dl-1.5.2/ap0dl/core/codebase/__init__.py
--rw-r--r--   0        0        0       55 2023-01-06 15:35:10.000000 ap0dl-1.5.2/ap0dl/core/codebase/downloader/__init__.py
--rw-r--r--   0        0        0    52198 2023-01-06 15:35:10.000000 ap0dl-1.5.2/ap0dl/core/codebase/downloader/content_mt.py
--rw-r--r--   0        0        0     7053 2023-01-06 15:35:10.000000 ap0dl-1.5.2/ap0dl/core/codebase/downloader/ffmpeg.py
--rw-r--r--   0        0        0     9039 2023-01-06 15:35:10.000000 ap0dl-1.5.2/ap0dl/core/codebase/downloader/handle.py
--rw-r--r--   0        0        0     4844 2023-01-06 15:35:10.000000 ap0dl-1.5.2/ap0dl/core/codebase/downloader/hls.py
--rw-r--r--   0        0        0     1473 2023-01-06 15:35:10.000000 ap0dl-1.5.2/ap0dl/core/codebase/downloader/idmanlib.py
--rw-r--r--   0        0        0      434 2023-01-06 15:35:10.000000 ap0dl-1.5.2/ap0dl/core/codebase/extractors/__init__.py
--rw-r--r--   0        0        0     1371 2023-01-06 15:35:10.000000 ap0dl-1.5.2/ap0dl/core/codebase/extractors/dailymotion/__init__.py
--rw-r--r--   0        0        0      866 2023-01-06 15:35:10.000000 ap0dl-1.5.2/ap0dl/core/codebase/extractors/doodstream/__init__.py
--rw-r--r--   0        0        0     2148 2023-01-06 15:35:10.000000 ap0dl-1.5.2/ap0dl/core/codebase/extractors/gogoplay/__init__.py
--rw-r--r--   0        0        0     1087 2023-01-06 15:35:10.000000 ap0dl-1.5.2/ap0dl/core/codebase/extractors/mp4upload/__init__.py
--rw-r--r--   0        0        0       32 2023-01-06 15:35:10.000000 ap0dl-1.5.2/ap0dl/core/codebase/extractors/mycloud/__init__.py
--rw-r--r--   0        0        0      990 2023-01-06 15:35:10.000000 ap0dl-1.5.2/ap0dl/core/codebase/extractors/okru/__init__.py
--rw-r--r--   0        0        0     1449 2023-01-06 15:35:10.000000 ap0dl-1.5.2/ap0dl/core/codebase/extractors/rapidvideo/__init__.py
--rw-r--r--   0        0        0     2103 2023-01-06 15:35:10.000000 ap0dl-1.5.2/ap0dl/core/codebase/extractors/rapidvideo/polling.py
--rw-r--r--   0        0        0      812 2023-01-06 15:35:10.000000 ap0dl-1.5.2/ap0dl/core/codebase/extractors/rapidvideo/utils.py
--rw-r--r--   0        0        0      899 2023-01-06 15:35:10.000000 ap0dl-1.5.2/ap0dl/core/codebase/extractors/streamlare/__init__.py
--rw-r--r--   0        0        0     1103 2023-01-06 15:35:10.000000 ap0dl-1.5.2/ap0dl/core/codebase/extractors/streamsb/__init__.py
--rw-r--r--   0        0        0      910 2023-01-06 15:35:10.000000 ap0dl-1.5.2/ap0dl/core/codebase/extractors/streamtape/__init__.py
--rw-r--r--   0        0        0      373 2023-01-06 15:35:10.000000 ap0dl-1.5.2/ap0dl/core/codebase/extractors/videobin/__init__.py
--rw-r--r--   0        0        0     2349 2023-01-06 15:35:10.000000 ap0dl-1.5.2/ap0dl/core/codebase/extractors/vidstream/__init__.py
--rw-r--r--   0        0        0     1968 2023-01-06 15:35:10.000000 ap0dl-1.5.2/ap0dl/core/codebase/helpers/__init__.py
--rw-r--r--   0        0        0      331 2023-01-06 15:35:10.000000 ap0dl-1.5.2/ap0dl/core/codebase/helpers/optopt.py
--rw-r--r--   0        0        0     2579 2023-01-06 15:35:10.000000 ap0dl-1.5.2/ap0dl/core/codebase/helpers/uwu.py
--rw-r--r--   0        0        0     1034 2023-01-06 15:35:10.000000 ap0dl-1.5.2/ap0dl/core/codebase/providers/__init__.py
--rw-r--r--   0        0        0     5134 2023-01-06 15:35:10.000000 ap0dl-1.5.2/ap0dl/core/codebase/providers/allanime/__init__.py
--rw-r--r--   0        0        0     2068 2023-01-06 15:35:10.000000 ap0dl-1.5.2/ap0dl/core/codebase/providers/allanime/superscrapers.py
--rw-r--r--   0        0        0     2320 2023-01-06 15:35:10.000000 ap0dl-1.5.2/ap0dl/core/codebase/providers/animekaizoku/__init__.py
--rw-r--r--   0        0        0     2402 2023-01-06 15:35:10.000000 ap0dl-1.5.2/ap0dl/core/codebase/providers/animeonsen/__init__.py
--rw-r--r--   0        0        0     1733 2023-01-06 15:35:10.000000 ap0dl-1.5.2/ap0dl/core/codebase/providers/animeout/__init__.py
--rw-r--r--   0        0        0     2903 2023-01-06 15:35:10.000000 ap0dl-1.5.2/ap0dl/core/codebase/providers/animepahe/__init__.py
--rw-r--r--   0        0        0     1751 2023-01-06 15:35:10.000000 ap0dl-1.5.2/ap0dl/core/codebase/providers/animepahe/inner/__init__.py
--rw-r--r--   0        0        0     1009 2023-01-06 15:35:10.000000 ap0dl-1.5.2/ap0dl/core/codebase/providers/animepahe/inner/archive.py
--rw-r--r--   0        0        0     2823 2023-01-06 15:35:10.000000 ap0dl-1.5.2/ap0dl/core/codebase/providers/animexin/__init__.py
--rw-r--r--   0        0        0      394 2023-01-06 15:35:10.000000 ap0dl-1.5.2/ap0dl/core/codebase/providers/animixplay/__init__.py
--rw-r--r--   0        0        0     1187 2023-01-06 15:35:10.000000 ap0dl-1.5.2/ap0dl/core/codebase/providers/animixplay/hardstream.py
--rw-r--r--   0        0        0     2740 2023-01-06 15:35:10.000000 ap0dl-1.5.2/ap0dl/core/codebase/providers/animixplay/stream_url.py
--rw-r--r--   0        0        0     1688 2023-01-06 15:35:10.000000 ap0dl-1.5.2/ap0dl/core/codebase/providers/animtime/__init__.py
--rw-r--r--   0        0        0     2866 2023-01-06 15:35:10.000000 ap0dl-1.5.2/ap0dl/core/codebase/providers/crunchyroll/__init__.py
--rw-r--r--   0        0        0     2322 2023-01-06 15:35:10.000000 ap0dl-1.5.2/ap0dl/core/codebase/providers/gogoanime/__init__.py
--rw-r--r--   0        0        0      924 2023-01-06 15:35:10.000000 ap0dl-1.5.2/ap0dl/core/codebase/providers/hahomoe/__init__.py
--rw-r--r--   0        0        0     1793 2023-01-06 15:35:10.000000 ap0dl-1.5.2/ap0dl/core/codebase/providers/hentaistream/__init__.py
--rw-r--r--   0        0        0     3112 2023-01-06 15:35:10.000000 ap0dl-1.5.2/ap0dl/core/codebase/providers/kamyroll/__init__.py
--rw-r--r--   0        0        0     2889 2023-01-06 15:35:10.000000 ap0dl-1.5.2/ap0dl/core/codebase/providers/kamyroll/api.py
--rw-r--r--   0        0        0     1819 2023-01-06 15:35:10.000000 ap0dl-1.5.2/ap0dl/core/codebase/providers/kawaiifu/__init__.py
--rw-r--r--   0        0        0     2213 2023-01-06 15:35:10.000000 ap0dl-1.5.2/ap0dl/core/codebase/providers/nineanime/__init__.py
--rw-r--r--   0        0        0     1721 2023-01-06 15:35:10.000000 ap0dl-1.5.2/ap0dl/core/codebase/providers/nineanime/decipher.py
--rw-r--r--   0        0        0     1983 2023-01-06 15:35:10.000000 ap0dl-1.5.2/ap0dl/core/codebase/providers/tenshimoe/__init__.py
--rw-r--r--   0        0        0     1260 2023-01-06 15:35:10.000000 ap0dl-1.5.2/ap0dl/core/codebase/providers/twistmoe/__init__.py
--rw-r--r--   0        0        0     1611 2023-01-06 15:35:10.000000 ap0dl-1.5.2/ap0dl/core/codebase/providers/twistmoe/stream_url.py
--rw-r--r--   0        0        0     2473 2023-01-06 15:35:10.000000 ap0dl-1.5.2/ap0dl/core/codebase/providers/zoro/__init__.py
--rw-r--r--   0        0        0     6032 2023-01-09 18:06:36.508356 ap0dl-1.5.2/ap0dl/core/config/__init__.py
--rw-r--r--   0        0        0     4305 2023-01-09 18:01:01.522289 ap0dl-1.5.2/ap0dl/core/package_resolver.py
--rw-r--r--   0        0        0    35149 2023-01-06 15:35:10.000000 ap0dl-1.5.2/LICENSE
--rw-r--r--   0        0        0      743 2023-01-09 18:16:11.640944 ap0dl-1.5.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-01-06 15:35:10.000000 ap0dl-1.5.2/readme.txt
--rw-r--r--   0        0        0     2794 1970-01-01 00:00:00.000000 ap0dl-1.5.2/setup.py
--rw-r--r--   0        0        0     1183 1970-01-01 00:00:00.000000 ap0dl-1.5.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-05-12 11:01:23.765279 ap0dl-1.6.0/LICENSE
+-rw-r--r--   0        0        0       20 2024-05-12 17:39:42.649462 ap0dl-1.6.0/ap0dl/__init__.py
+-rw-r--r--   0        0        0     3188 2024-05-12 18:28:55.981563 ap0dl-1.6.0/ap0dl/__main__.py
+-rw-r--r--   0        0        0       71 2024-05-12 17:39:42.649462 ap0dl-1.6.0/ap0dl/core/__init__.py
+-rw-r--r--   0        0        0      368 2024-05-12 18:33:41.891488 ap0dl-1.6.0/ap0dl/core/__version__.py
+-rw-r--r--   0        0        0        0 2024-05-12 17:39:42.649462 ap0dl-1.6.0/ap0dl/core/cli/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-12 17:39:42.649462 ap0dl-1.6.0/ap0dl/core/cli/commands/__init__.py
+-rw-r--r--   0        0        0     4891 2024-05-12 18:27:02.478718 ap0dl-1.6.0/ap0dl/core/cli/commands/download.py
+-rw-r--r--   0        0        0     1344 2024-05-12 18:27:11.318716 ap0dl-1.6.0/ap0dl/core/cli/commands/grab.py
+-rw-r--r--   0        0        0     3272 2024-05-12 18:27:25.888712 ap0dl-1.6.0/ap0dl/core/cli/commands/schedule.py
+-rw-r--r--   0        0        0     1644 2024-05-12 18:27:34.783858 ap0dl-1.6.0/ap0dl/core/cli/commands/search.py
+-rw-r--r--   0        0        0     8704 2024-05-12 18:29:21.341557 ap0dl-1.6.0/ap0dl/core/cli/commands/stream.py
+-rw-r--r--   0        0        0     3318 2024-05-12 18:27:50.341583 ap0dl-1.6.0/ap0dl/core/cli/commands/update.py
+-rw-r--r--   0        0        0      112 2024-05-12 17:39:42.649462 ap0dl-1.6.0/ap0dl/core/cli/exit_codes.py
+-rw-r--r--   0        0        0     4805 2024-05-12 17:53:49.659240 ap0dl-1.6.0/ap0dl/core/cli/helpers/__init__.py
+-rw-r--r--   0        0        0     1762 2024-05-12 17:53:49.659240 ap0dl-1.6.0/ap0dl/core/cli/helpers/aniskip.py
+-rw-r--r--   0        0        0     2313 2024-05-12 18:34:55.991469 ap0dl-1.6.0/ap0dl/core/cli/helpers/banner.py
+-rw-r--r--   0        0        0      240 2024-05-12 18:30:52.211534 ap0dl-1.6.0/ap0dl/core/cli/helpers/constants.py
+-rw-r--r--   0        0        0     4250 2024-05-12 17:53:49.659240 ap0dl-1.6.0/ap0dl/core/cli/helpers/decorators.py
+-rw-r--r--   0        0        0     1093 2024-05-12 17:53:49.659240 ap0dl-1.6.0/ap0dl/core/cli/helpers/fuzzysearch.py
+-rw-r--r--   0        0        0     9628 2024-05-12 18:34:20.451478 ap0dl-1.6.0/ap0dl/core/cli/helpers/intelliq.py
+-rw-r--r--   0        0        0     2589 2024-05-12 17:53:49.659240 ap0dl-1.6.0/ap0dl/core/cli/helpers/logger.py
+-rw-r--r--   0        0        0     1567 2024-05-12 17:53:49.659240 ap0dl-1.6.0/ap0dl/core/cli/helpers/player.py
+-rw-r--r--   0        0        0      343 2024-05-12 17:53:49.659240 ap0dl-1.6.0/ap0dl/core/cli/helpers/players/__init__.py
+-rw-r--r--   0        0        0      757 2024-05-12 17:53:49.659240 ap0dl-1.6.0/ap0dl/core/cli/helpers/players/android.py
+-rw-r--r--   0        0        0     2093 2024-05-12 18:33:54.101487 ap0dl-1.6.0/ap0dl/core/cli/helpers/players/base_player.py
+-rw-r--r--   0        0        0      725 2024-05-12 17:53:49.669240 ap0dl-1.6.0/ap0dl/core/cli/helpers/players/ffplay.py
+-rw-r--r--   0        0        0     2744 2024-05-12 17:53:49.669240 ap0dl-1.6.0/ap0dl/core/cli/helpers/players/mpv.py
+-rw-r--r--   0        0        0     1750 2024-05-12 17:53:49.669240 ap0dl-1.6.0/ap0dl/core/cli/helpers/players/vlc.py
+-rw-r--r--   0        0        0     1476 2024-05-12 17:53:49.669240 ap0dl-1.6.0/ap0dl/core/cli/helpers/processors.py
+-rw-r--r--   0        0        0     5095 2024-05-12 17:53:49.669240 ap0dl-1.6.0/ap0dl/core/cli/helpers/prompts.py
+-rw-r--r--   0        0        0     2994 2024-05-12 18:31:31.091524 ap0dl-1.6.0/ap0dl/core/cli/helpers/rpc.py
+-rw-r--r--   0        0        0     6818 2024-05-12 18:33:31.151491 ap0dl-1.6.0/ap0dl/core/cli/helpers/searcher.py
+-rw-r--r--   0        0        0     1009 2024-05-12 17:53:49.669240 ap0dl-1.6.0/ap0dl/core/cli/helpers/special.py
+-rw-r--r--   0        0        0     2004 2024-05-12 17:53:49.669240 ap0dl-1.6.0/ap0dl/core/cli/helpers/stream_handlers.py
+-rw-r--r--   0        0        0      544 2024-05-12 18:33:13.081496 ap0dl-1.6.0/ap0dl/core/cli/http_client.py
+-rw-r--r--   0        0        0       26 2024-05-12 17:39:42.649462 ap0dl-1.6.0/ap0dl/core/codebase/__init__.py
+-rw-r--r--   0        0        0       55 2024-05-12 17:39:42.649462 ap0dl-1.6.0/ap0dl/core/codebase/downloader/__init__.py
+-rw-r--r--   0        0        0     7357 2024-05-12 17:39:42.649462 ap0dl-1.6.0/ap0dl/core/codebase/downloader/ffmpeg.py
+-rw-r--r--   0        0        0    11780 2024-05-12 18:32:43.691505 ap0dl-1.6.0/ap0dl/core/codebase/downloader/handle.py
+-rw-r--r--   0        0        0     4844 2024-05-12 17:39:42.649462 ap0dl-1.6.0/ap0dl/core/codebase/downloader/hls.py
+-rw-r--r--   0        0        0     1994 2024-05-12 17:39:42.649462 ap0dl-1.6.0/ap0dl/core/codebase/downloader/idmanlib.py
+-rw-r--r--   0        0        0      434 2024-05-12 17:39:42.649462 ap0dl-1.6.0/ap0dl/core/codebase/extractors/__init__.py
+-rw-r--r--   0        0        0     1371 2024-05-12 17:39:42.649462 ap0dl-1.6.0/ap0dl/core/codebase/extractors/dailymotion/__init__.py
+-rw-r--r--   0        0        0      866 2024-05-12 17:39:42.649462 ap0dl-1.6.0/ap0dl/core/codebase/extractors/doodstream/__init__.py
+-rw-r--r--   0        0        0     2148 2024-05-12 17:39:42.649462 ap0dl-1.6.0/ap0dl/core/codebase/extractors/gogoplay/__init__.py
+-rw-r--r--   0        0        0     1087 2024-05-12 17:39:42.649462 ap0dl-1.6.0/ap0dl/core/codebase/extractors/mp4upload/__init__.py
+-rw-r--r--   0        0        0       32 2024-05-12 17:39:42.649462 ap0dl-1.6.0/ap0dl/core/codebase/extractors/mycloud/__init__.py
+-rw-r--r--   0        0        0      990 2024-05-12 17:39:42.649462 ap0dl-1.6.0/ap0dl/core/codebase/extractors/okru/__init__.py
+-rw-r--r--   0        0        0     1176 2024-05-12 17:39:42.649462 ap0dl-1.6.0/ap0dl/core/codebase/extractors/rapidvideo/__init__.py
+-rw-r--r--   0        0        0     2103 2024-05-12 17:39:42.649462 ap0dl-1.6.0/ap0dl/core/codebase/extractors/rapidvideo/polling.py
+-rw-r--r--   0        0        0     1075 2024-05-12 17:39:42.649462 ap0dl-1.6.0/ap0dl/core/codebase/extractors/rapidvideo/utils.py
+-rw-r--r--   0        0        0      899 2024-05-12 17:39:42.649462 ap0dl-1.6.0/ap0dl/core/codebase/extractors/streamlare/__init__.py
+-rw-r--r--   0        0        0     1103 2024-05-12 17:39:42.649462 ap0dl-1.6.0/ap0dl/core/codebase/extractors/streamsb/__init__.py
+-rw-r--r--   0        0        0      910 2024-05-12 17:39:42.649462 ap0dl-1.6.0/ap0dl/core/codebase/extractors/streamtape/__init__.py
+-rw-r--r--   0        0        0      373 2024-05-12 17:39:42.649462 ap0dl-1.6.0/ap0dl/core/codebase/extractors/videobin/__init__.py
+-rw-r--r--   0        0        0      875 2024-05-12 17:39:42.649462 ap0dl-1.6.0/ap0dl/core/codebase/extractors/vidstream/__init__.py
+-rw-r--r--   0        0        0     1883 2024-05-12 18:29:31.861554 ap0dl-1.6.0/ap0dl/core/codebase/helpers/__init__.py
+-rw-r--r--   0        0        0     2039 2024-05-12 18:30:19.261543 ap0dl-1.6.0/ap0dl/core/codebase/helpers/superscrapers.py
+-rw-r--r--   0        0        0     2579 2024-05-12 17:39:42.649462 ap0dl-1.6.0/ap0dl/core/codebase/helpers/uwu.py
+-rw-r--r--   0        0        0     1034 2024-05-12 17:39:42.649462 ap0dl-1.6.0/ap0dl/core/codebase/providers/__init__.py
+-rw-r--r--   0        0        0     6188 2024-05-12 17:39:42.649462 ap0dl-1.6.0/ap0dl/core/codebase/providers/allanime/__init__.py
+-rw-r--r--   0        0        0     5368 2024-05-12 18:30:10.781545 ap0dl-1.6.0/ap0dl/core/codebase/providers/allanime/gql_api.py
+-rw-r--r--   0        0        0     2320 2024-05-12 17:39:42.649462 ap0dl-1.6.0/ap0dl/core/codebase/providers/animekaizoku/__init__.py
+-rw-r--r--   0        0        0     2402 2024-05-12 17:39:42.649462 ap0dl-1.6.0/ap0dl/core/codebase/providers/animeonsen/__init__.py
+-rw-r--r--   0        0        0     1742 2024-05-12 17:39:42.649462 ap0dl-1.6.0/ap0dl/core/codebase/providers/animeout/__init__.py
+-rw-r--r--   0        0        0     2748 2024-05-12 18:30:28.711541 ap0dl-1.6.0/ap0dl/core/codebase/providers/animepahe/__init__.py
+-rw-r--r--   0        0        0     1751 2024-05-12 17:39:42.649462 ap0dl-1.6.0/ap0dl/core/codebase/providers/animepahe/inner/__init__.py
+-rw-r--r--   0        0        0     1009 2024-05-12 17:39:42.649462 ap0dl-1.6.0/ap0dl/core/codebase/providers/animepahe/inner/archive.py
+-rw-r--r--   0        0        0     2823 2024-05-12 17:39:42.649462 ap0dl-1.6.0/ap0dl/core/codebase/providers/animexin/__init__.py
+-rw-r--r--   0        0        0      394 2024-05-12 17:39:42.649462 ap0dl-1.6.0/ap0dl/core/codebase/providers/animixplay/__init__.py
+-rw-r--r--   0        0        0     1187 2024-05-12 17:39:42.649462 ap0dl-1.6.0/ap0dl/core/codebase/providers/animixplay/hardstream.py
+-rw-r--r--   0        0        0     2740 2024-05-12 17:39:42.649462 ap0dl-1.6.0/ap0dl/core/codebase/providers/animixplay/stream_url.py
+-rw-r--r--   0        0        0     1845 2024-05-12 18:26:20.258729 ap0dl-1.6.0/ap0dl/core/codebase/providers/animtime/__init__.py
+-rw-r--r--   0        0        0     2866 2024-05-12 17:39:42.649462 ap0dl-1.6.0/ap0dl/core/codebase/providers/crunchyroll/__init__.py
+-rw-r--r--   0        0        0     2259 2024-05-12 17:39:42.649462 ap0dl-1.6.0/ap0dl/core/codebase/providers/gogoanime/__init__.py
+-rw-r--r--   0        0        0     1511 2024-05-12 17:39:42.649462 ap0dl-1.6.0/ap0dl/core/codebase/providers/hahomoe/__init__.py
+-rw-r--r--   0        0        0     2240 2024-05-12 17:39:42.649462 ap0dl-1.6.0/ap0dl/core/codebase/providers/hentaistream/__init__.py
+-rw-r--r--   0        0        0     2814 2024-05-12 17:39:42.649462 ap0dl-1.6.0/ap0dl/core/codebase/providers/kamyroll/__init__.py
+-rw-r--r--   0        0        0     2889 2024-05-12 18:29:40.811553 ap0dl-1.6.0/ap0dl/core/codebase/providers/kamyroll/api.py
+-rw-r--r--   0        0        0     1819 2024-05-12 17:39:42.649462 ap0dl-1.6.0/ap0dl/core/codebase/providers/kawaiifu/__init__.py
+-rw-r--r--   0        0        0     2309 2024-05-12 18:29:54.541549 ap0dl-1.6.0/ap0dl/core/codebase/providers/marinmoe/__init__.py
+-rw-r--r--   0        0        0     2565 2024-05-12 17:39:42.649462 ap0dl-1.6.0/ap0dl/core/codebase/providers/nineanime/__init__.py
+-rw-r--r--   0        0        0     1695 2024-05-12 17:39:42.649462 ap0dl-1.6.0/ap0dl/core/codebase/providers/nineanime/decipher.py
+-rw-r--r--   0        0        0     1260 2024-05-12 17:39:42.649462 ap0dl-1.6.0/ap0dl/core/codebase/providers/twistmoe/__init__.py
+-rw-r--r--   0        0        0     1611 2024-05-12 17:39:42.649462 ap0dl-1.6.0/ap0dl/core/codebase/providers/twistmoe/stream_url.py
+-rw-r--r--   0        0        0     1901 2024-05-12 17:39:42.649462 ap0dl-1.6.0/ap0dl/core/codebase/providers/yugen/__init__.py
+-rw-r--r--   0        0        0     2542 2024-05-12 17:39:42.659462 ap0dl-1.6.0/ap0dl/core/codebase/providers/zoro/__init__.py
+-rw-r--r--   0        0        0     6155 2024-05-12 18:29:10.541560 ap0dl-1.6.0/ap0dl/core/config/__init__.py
+-rw-r--r--   0        0        0     4302 2024-05-12 18:34:39.311475 ap0dl-1.6.0/ap0dl/core/package_resolver.py
+-rw-r--r--   0        0        0      282 2024-05-12 18:32:53.881502 ap0dl-1.6.0/ap0dl/utils/__init__.py
+-rw-r--r--   0        0        0     7275 2024-05-12 18:33:22.361492 ap0dl-1.6.0/ap0dl/utils/http_caching.py
+-rw-r--r--   0        0        0     3930 2024-05-12 18:33:03.061499 ap0dl-1.6.0/ap0dl/utils/http_client.py
+-rw-r--r--   0        0        0     6049 2024-05-12 17:39:42.659462 ap0dl-1.6.0/ap0dl/utils/media_downloader.py
+-rw-r--r--   0        0        0      394 2024-05-12 18:30:01.671548 ap0dl-1.6.0/ap0dl/utils/optopt.py
+-rw-r--r--   0        0        0     1898 2024-05-12 17:39:42.659462 ap0dl-1.6.0/ap0dl/utils/powertools.py
+-rw-r--r--   0        0        0     1775 2024-05-12 18:34:30.511476 ap0dl-1.6.0/ap0dl/utils/searching.py
+-rw-r--r--   0        0        0     1047 2024-05-12 17:39:42.659462 ap0dl-1.6.0/ap0dl/utils/serverfiles.py
+-rw-r--r--   0        0        0      866 2024-05-12 19:04:36.471002 ap0dl-1.6.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-12 11:01:23.775279 ap0dl-1.6.0/readme.txt
+-rw-r--r--   0        0        0     1288 1970-01-01 00:00:00.000000 ap0dl-1.6.0/PKG-INFO
```

### Comparing `ap0dl-1.5.2/ap0dl/__main__.py` & `ap0dl-1.6.0/ap0dl/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -62,24 +62,27 @@
             style="bold white",
         ),
     ):
         for greeting in stream_handlers.iter_greetings():
             console.print(greeting, style="white")
 
         if not disable_update:
+            from ap0dl.utils.optopt import regexlib
+
             from .core.cli.http_client import client
-            from .core.codebase.helpers.optopt import regexlib
 
             branch, version_file = constants.VERSION_FILE_PATH
 
+            upstream_response = client.get(
+                f"https://raw.githubusercontent.com/{author}/{repository_name}/{branch}/{version_file}"
+            )
+
             upstream_version = regexlib.search(
-                r'__core__ = "(.*?)"',
-                client.get(
-                    f"https://raw.githubusercontent.com/{author}/{repository_name}/{branch}/{version_file}"
-                ).text,
+                r'name = "ap0dl"\nversion = "(.+?)"',
+                upstream_response.text,
             ).group(1)
 
             tuplisied_upstream, tuplised_current_version = tuple(
                 map(int, upstream_version.split("."))
             ), tuple(map(int, __version__.__core__.split(".")))
 
             if tuplisied_upstream > tuplised_current_version:
```

### Comparing `ap0dl-1.5.2/ap0dl/core/cli/commands/download.py` & `ap0dl-1.6.0/ap0dl/core/cli/commands/download.py`

 * *Files 5% similar despite different names*

```diff
@@ -69,15 +69,14 @@
         if special:
             streams = list(helpers.special.special_parser(streams, special))
 
         download_directory = Path(download_dir).resolve(strict=True)
         content_name = sanitize_filename(anime["name"])
 
         content_dir = download_directory / content_name
-        content_dir.mkdir(exist_ok=True)
 
         console.print(
             "The project will download to:",
             Text(content_dir.resolve().as_posix(), style="bold"),
         )
         total = len(streams)
 
@@ -89,43 +88,57 @@
             )
             raise SystemExit(exit_codes.NO_CONTENT_FOUND)
 
         with helpers.stream_handlers.context_raiser(
             console, f"Now downloading {content_name!r}", name="downloading"
         ):
             for count, (stream_urls_caller, episode_number) in enumerate(streams, 1):
-
-                content_title = "E{:02d}".format(int(episode_number))
                 stream_urls = helpers.ensure_extraction(
                     http_client.client, stream_urls_caller
                 )
 
+                content_title = f"E{int(episode_number):02d}"
+
                 if not stream_urls:
                     console.print(
                         Text(
                             f"Could not find any streams for {content_title!r} :/.",
                         )
                     )
                     continue
 
                 console.print(
                     f"Currently downloading: {content_title!r}. [dim]{total-count:d} episodes in queue.[/]",
                 )
 
-                success, reason = helpers.download(
-                    http_client.client,
-                    logger,
-                    content_dir,
-                    content_title,
-                    stream_urls,
-                    quality,
-                    idm=idm,
+                expected_download_path = content_dir / content_title
+
+                status_enum, exception = helpers.safe_download_callback(
+                    session=http_client.client,
+                    logger=logger,
+                    stream_urls=stream_urls,
+                    quality=quality,
+                    expected_download_path=expected_download_path,
+                    use_internet_download_manager=idm,
                     retry_timeout=AUTO_RETRY,
                     log_level=log_level,
                 )
 
-                if not success:
+                if status_enum == helpers.SafeCaseEnum.NO_CONTENT_FOUND:
+                    console.print(
+                        f"Could not find any streams for {content_title!r}",
+                    )
+                    continue
+
+                if status_enum == helpers.SafeCaseEnum.EXTRACTION_ERROR:
+                    console.print(
+                        f"Could not extract any streams for {content_title!r} due to: {exception!r}",
+                    )
+                    continue
+
+                if status_enum == helpers.SafeCaseEnum.DOWNLOADER_EXCEPTION:
                     console.print(
                         Text(
-                            f"Could not download {content_title!r} because of {reason!r} :/, a good option would be to retry using better providers :/.",
+                            f"Internal downloader error occured for {content_title!r}.",
                         )
                     )
+                    continue
```

### Comparing `ap0dl-1.5.2/ap0dl/core/cli/commands/grab.py` & `ap0dl-1.6.0/ap0dl/core/cli/commands/grab.py`

 * *Files identical despite different names*

### Comparing `ap0dl-1.5.2/ap0dl/core/cli/commands/schedule.py` & `ap0dl-1.6.0/ap0dl/core/cli/commands/schedule.py`

 * *Files identical despite different names*

### Comparing `ap0dl-1.5.2/ap0dl/core/cli/commands/search.py` & `ap0dl-1.6.0/ap0dl/core/cli/commands/search.py`

 * *Files identical despite different names*

### Comparing `ap0dl-1.5.2/ap0dl/core/cli/commands/stream.py` & `ap0dl-1.6.0/ap0dl/core/cli/commands/stream.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import base64
 import logging
 
 import click
 import yarl
+from rich.errors import MarkupError
 from rich.text import Text
 
 from ...__version__ import __core__
 from ...codebase import providers
 from ...config import (
     CHECK_FOR_UPDATES,
     DEFAULT_PLAYER,
@@ -42,14 +43,15 @@
 )
 def ap0dl_stream(
     query, special, quality, player_opts, player, index, log_level, **kwargs
 ):
     """
     Streamer call for ap0dl streaming session.
     """
+
     r = kwargs.get("range")
     console = helpers.stream_handlers.get_console()
 
     logger = logging.getLogger("streamer")
 
     if player_opts is not None:
         player_opts = tuple(click.parser.split_arg_string(player_opts))
@@ -74,15 +76,14 @@
         console,
         Text(
             f"Scraping juicy streams from {provider!r}@{anime['anime_url']}",
             style="bold magenta",
         ),
         name="scraping",
     ):
-
         match, provider_module, _ = providers.get_provider(
             providers.append_protocol(anime.get("anime_url"))
         )
 
         streams = list(
             provider_module.fetcher(
                 http_client.client, anime.get("anime_url"), r, match
@@ -103,39 +104,35 @@
                 style="dim",
             )
             return exit(exit_codes.NO_CONTENT_FOUND)
 
         with helpers.stream_handlers.context_raiser(
             console, f"Now streaming {content_title!r}", name="streaming"
         ):
-
             for count, (stream_urls_caller, episode_number) in enumerate(streams, 1):
-
                 if episode_number == 0:
                     episode_text = "Special Episode"
                 else:
                     episode_text = f"Episode {episode_number}"
 
                 if content_title:
                     media_title = f"{content_title}: {episode_text}"
                 else:
                     media_title = episode_text
 
                 playing = True
 
                 while playing:
-
                     stream_urls = list(
                         helpers.ensure_extraction(
                             http_client.client, stream_urls_caller
                         )
                     )
 
                     if not stream_urls:
-
                         console.print(
                             Text(
                                 f"Could not find any streams for {episode_text!r} :/."
                             ),
                             Text(
                                 "Loading in DEBUG [--log-level=0] mode allows extraction retrial.",
                                 style="dim",
@@ -145,25 +142,24 @@
                         if log_level <= logging.DEBUG:
                             playing = click.confirm("Retry stream url extraction?")
 
                         continue
 
                     titles = set(_.get("title") for _ in stream_urls)
 
-                    if len(titles) > 1:
+                    if len(titles) > 1 and FORCE_STREAMING_QUALITY_SELECTION:
                         console.print(
                             Text(
                                 f"Multiple titles found for the same streams, multiple seasons may be available. Please adjust the quality string as required: {', '.join(map(repr, titles))}",
-                                dim=True,
+                                style="dim",
                             ),
                         )
 
                     selection = helpers.prompts.quality_prompt(
-                        logger,
-                        log_level,
+                        console,
                         stream_urls,
                         force_selection_string=quality
                         if FORCE_STREAMING_QUALITY_SELECTION
                         else None,
                     )
 
                     headers = selection.get("headers", {})
@@ -185,35 +181,40 @@
                         f"Currently playing: {episode_text!r}. [dim]{total-count:d} episodes in queue.[/]",
                         name="playing",
                     ):
                         if not headers:
                             shareable_url = yarl.URL(
                                 "https://plyr.link/p/player.html"
                             ).with_fragment(
-                                base64.urlsafe_b64encode(
+                                base64.b64encode(
                                     selection["stream_url"].encode()
                                 ).decode()
                             )
                             console.print(
                                 Text(
                                     f"This stream may be share-able [embeddable and playable as a single URL] (please note that subtitles, chapters and titles won't be embedded)."
                                 ),
                                 style="dim",
                             )
-                            console.print(
-                                f"[dim]Share-ables: [link={shareable_url}]embed[/], [link={selection['stream_url']}]direct url[/][/]"
-                            )
+
+                            try:
+                                console.print(
+                                    f"[dim]Share-ables: [link={shareable_url}]embed[/link], [link={selection['stream_url']}]direct url[/link][/dim]"
+                                )
+                            except MarkupError:
+                                pass
 
                         with streamer:
                             streamer.play(
                                 selection["stream_url"],
                                 title=media_title,
                                 headers=headers,
                                 subtitles=selection.get("subtitle", []),
                                 chapters=chapters,
+                                audio_tracks=selection.get("audio_tracks", []),
                             )
 
                             if DISCORD_PRESENCE:
                                 set_streaming_episode(
                                     http_client.client, content_title, episode_number
                                 )
```

### Comparing `ap0dl-1.5.2/ap0dl/core/cli/commands/update.py` & `ap0dl-1.6.0/ap0dl/core/cli/commands/update.py`

 * *Files identical despite different names*

### Comparing `ap0dl-1.5.2/ap0dl/core/cli/helpers/aniskip.py` & `ap0dl-1.6.0/ap0dl/core/cli/helpers/aniskip.py`

 * *Files identical despite different names*

### Comparing `ap0dl-1.5.2/ap0dl/core/cli/helpers/banner.py` & `ap0dl-1.6.0/ap0dl/core/cli/helpers/banner.py`

 * *Files identical despite different names*

### Comparing `ap0dl-1.5.2/ap0dl/core/cli/helpers/decorators.py` & `ap0dl-1.6.0/ap0dl/core/cli/helpers/decorators.py`

 * *Files identical despite different names*

### Comparing `ap0dl-1.5.2/ap0dl/core/cli/helpers/fuzzysearch.py` & `ap0dl-1.6.0/ap0dl/core/cli/helpers/fuzzysearch.py`

 * *Files identical despite different names*

### Comparing `ap0dl-1.5.2/ap0dl/core/cli/helpers/logger.py` & `ap0dl-1.6.0/ap0dl/core/cli/helpers/logger.py`

 * *Files identical despite different names*

### Comparing `ap0dl-1.5.2/ap0dl/core/cli/helpers/player.py` & `ap0dl-1.6.0/ap0dl/core/cli/helpers/player.py`

 * *Files identical despite different names*

### Comparing `ap0dl-1.5.2/ap0dl/core/cli/helpers/players/android.py` & `ap0dl-1.6.0/ap0dl/core/cli/helpers/players/android.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
         args = (
             "am",
             "start",
             "-a",
             self.intent,
             "-d",
             stream_url,
+            *self.args,
         )
 
         keys = set(kwargs.keys())
 
         if self.warnable_opts & keys:
             warn(
                 f"Android does not support {', '.join(map(repr, self.warnable_opts & keys))} options. "
```

### Comparing `ap0dl-1.5.2/ap0dl/core/cli/helpers/players/base_player.py` & `ap0dl-1.6.0/ap0dl/core/cli/helpers/players/base_player.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 BasePlayer, (c) 2022-present, ap0dl authors
 
-Note from developer, ap0:
+Note from developer, KR:
 
 This is the base class for all players. All players
 **must** inherit from this class.
 
     class YourPlayer(BasePlayer):
         ...
```

### Comparing `ap0dl-1.5.2/ap0dl/core/cli/helpers/players/ffplay.py` & `ap0dl-1.6.0/ap0dl/core/cli/helpers/players/ffplay.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     opts_spec = {
         "headers": "-headers",
         "metadata": "-metadata",
         "title_field": "title",
     }
 
     def play(self, stream_url, headers=None, title=None, opts=None, **kwargs):
-        args = (self.executable, stream_url)
+        args = (self.executable, *self.args, stream_url)
 
         if opts is not None:
             args += tuple(opts)
 
         if headers is not None:
             args += (
                 f"{self.opts_spec['headers']}={self.headers_joiner.join(f'{key}: {value}' for key, value in headers.items())}",
```

### Comparing `ap0dl-1.5.2/ap0dl/core/cli/helpers/players/mpv.py` & `ap0dl-1.6.0/ap0dl/core/cli/helpers/players/mpv.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,44 +1,49 @@
 from sys import platform
 from tempfile import NamedTemporaryFile
 
 from .base_player import BasePlayer
 
 
 class MPVDefaultPlayer(BasePlayer):
-
     optimisation_args = [
         "--force-window=immediate",
     ]
     headers_joiner = "\r\n"
 
     if platform == "win32":
         path_joiner = ";"
     else:
         path_joiner = ":"
 
     opts_spec = {
         "headers": "--http-header-fields",
         "title": "--title",
         "subtitles": "--sub-files",
+        "audios": "--audio-files",
         "media-title": "--force-media-title",
     }
 
     def play(
         self,
         stream_url,
         subtitles=None,
         headers=None,
         title=None,
         opts=None,
         chapters=None,
+        audio_tracks=None,
         **kwargs,
     ):
+        args = (self.executable, *self.args, stream_url)
 
-        args = (self.executable, stream_url)
+        if audio_tracks is not None:
+            args += (
+                f"{self.opts_spec['audios']}={self.path_joiner.join(audio_tracks)}",
+            )
 
         if opts is not None:
             args += tuple(opts)
 
         if headers is not None:
             args += (
                 f"{self.opts_spec['headers']}={self.headers_joiner.join(f'{key}: {value}' for key, value in headers.items())}",
@@ -52,15 +57,14 @@
 
         if subtitles is not None:
             args += (
                 f"{self.opts_spec['subtitles']}={self.path_joiner.join(subtitles)}",
             )
 
         if chapters:
-
             # NOTE: This could be achieved with a PIPE.
             # This is not done in this case because you
             # only PIPE one argument at a time, and this
             # is expected to be limiting in the future.
             # PIPE-ing whole media is more suitable.
 
             with NamedTemporaryFile("w", delete=False) as chapters_file:
@@ -86,15 +90,14 @@
 
 class CelluloidPlayer(MPVDefaultPlayer):
     optimisation_args = [
         "--new-window",
     ]
 
     def __new__(cls, *args, **kwargs):
-
         for key, value in cls.opts_spec.items():
             cls.opts_spec[key] = f"--mpv-{value.lstrip('-')}"
 
-        return cls
+        return super().__new__(cls)
 
 
 IINAPlayer = CelluloidPlayer
```

### Comparing `ap0dl-1.5.2/ap0dl/core/cli/helpers/players/vlc.py` & `ap0dl-1.6.0/ap0dl/core/cli/helpers/players/vlc.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,33 @@
 from warnings import warn
 
 from .base_player import BasePlayer
 
 
 class VLCPlayer(BasePlayer):
-
     optimisation_args = ("--http-forward-cookies",)
 
     opts_spec = {
         "http_referrer": "--http-referrer",
         "user_agent": "--user-agent",
         "subtitle": "--sub-file",
+        "audio": "--audio-file",
     }
 
     def play(
-        self, stream_url, subtitles=None, headers=None, title=None, opts=None, **kwargs
+        self,
+        stream_url,
+        subtitles=None,
+        headers=None,
+        title=None,
+        opts=None,
+        audio_tracks=None,
+        **kwargs,
     ):
-        args = (self.executable, stream_url)
+        args = (self.executable, *self.args, stream_url)
 
         if opts is not None:
             args += tuple(opts)
 
         if headers is not None:
             lowercased_headers = {key.lower(): value for key, value in headers.items()}
 
@@ -46,8 +53,11 @@
 
         if title is not None:
             args += (f"--meta-title={title}",)
 
         if subtitles is not None:
             args += tuple(f"--sub-file={subtitles}" for subtitles in subtitles)
 
+        if audio_tracks is not None:
+            args += tuple(f"--audio-file={audio_track}" for audio_track in audio_tracks)
+
         self.spawn(args)
```

### Comparing `ap0dl-1.5.2/ap0dl/core/cli/helpers/processors.py` & `ap0dl-1.6.0/ap0dl/core/cli/helpers/processors.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,8 +37,12 @@
 
     genexp = provider_searcher_mapping[provider](session, query)
 
     if auto_index is None:
         return prompt_user(console, genexp, provider)
 
     expanded = list(genexp)
+
+    if not expanded:
+        return {}, None
+
     return expanded[(auto_index - 1) % len(expanded)], provider
```

### Comparing `ap0dl-1.5.2/ap0dl/core/cli/helpers/rpc.py` & `ap0dl-1.6.0/ap0dl/core/cli/helpers/rpc.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import functools
 import time
 
 import pypresence
 
-AP0DL_APPLICATION_ID = 1061262926389973042
+ap0dl_APPLICATION_ID = 897850955373105222
 
 try:
-    presence_client = pypresence.Presence(AP0DL_APPLICATION_ID)
+    presence_client = pypresence.Presence(ap0dl_APPLICATION_ID)
 except (pypresence.DiscordNotFound, ConnectionError):
     raise RuntimeError("Could not connect to Discord.")
 
 presence_client.connect()
 
 presence_client.update(
     state="Queuing up the streams",
@@ -64,15 +64,15 @@
     anime = content_list[0]
 
     anime_attributes = anime["attributes"]
 
     image = anime_attributes["posterImage"]["original"]
     count = anime_attributes["episodeCount"]
     url = "https://kitsu.io/{}/{}".format(anime['type'], anime_attributes['slug'])
-    url_button = [ { "label": "View Anime", "url": url },  { "label": "ap0 project", "url": "https://github.com/rares9301/ap0dl" } ]
+    url_button = [ { "label": "View Anime", "url": url } ]
 
     if count:
         state += "/{}".format(count)
 
     if count is None or (episode > count):
         return presence_client.update(
             state=state,
```

### Comparing `ap0dl-1.5.2/ap0dl/core/cli/helpers/searcher.py` & `ap0dl-1.6.0/ap0dl/core/cli/helpers/searcher.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 """
 All the search algorithms for all the providers available in ap0dl.
 """
 
-import json
+from urllib.parse import unquote
 
 import lxml.html as htmlparser
 
+from ap0dl.core.codebase.providers.allanime import gql_api as allanime_gql_api
+from ap0dl.utils.powertools import ctx
+
 from ...codebase.helpers import uwu
 from ...codebase.providers.kamyroll.api import get_api
 from ...config import (
     ALLANIME,
     ANIMEKAIZOKU,
     ANIMEOUT,
     ANIMEPAHE,
     ANIMIXPLAY,
     GOGOANIME,
     HAHO,
     HENTAISTREAM,
     KAWAIIFU,
+    MARIN,
     NINEANIME,
-    TENSHI,
     TWIST,
+    YUGEN,
     ZORO,
 )
 from .fuzzysearch import search
 
 
 def search_9anime(session, query):
     nineanime_results = session.get(NINEANIME + "filter", params={"keyword": query})
@@ -45,63 +49,36 @@
         yield {
             "anime_url": ANIMEKAIZOKU + results.cssselect("a")[0].get("href"),
             "name": results.text_content(),
         }
 
 
 def search_allanime(session, query):
-
-    gql_response = session.get(
-        ALLANIME + "allanimeapi",
-        params={
-            "variables": json.dumps(
-                {
-                    "search": {
-                        "allowAdult": True,
-                        "allowUnknown": True,
-                        "query": query,
-                    },
-                    "limit": 40,
-                }
-            ),
-            "extensions": json.dumps(
-                {
-                    "persistedQuery": {
-                        "version": 1,
-                        "sha256Hash": "9c7a8bc1e095a34f2972699e8105f7aaf9082c6e1ccd56eab99c2f1a971152c6",
-                    }
-                }
-            ),
-        },
-    ).json()
-
-    for result in gql_response.get("data", {}).get("shows", {}).get("edges", []):
-        if any(a for _, a in result.get("availableEpisodes", {}).items()):
-            yield {
-                "anime_url": ALLANIME + f"anime/{result['_id']}",
-                "name": result["name"],
-            }
+    for result in allanime_gql_api.api.iter_search_results(session, query):
+        yield {
+            "anime_url": ALLANIME + f"anime/{result['_id']}",
+            "name": result["name"],
+        }
 
 
 def search_animepahe(session, query):
-
     animepahe_results = session.get(
         ANIMEPAHE + "api", params={"q": query, "m": "search"}
     )
     content = animepahe_results.json()
 
     for results in content.get("data", []):
         yield {
             "anime_url": ANIMEPAHE + "anime/" + results.get("session"),
             "name": results.get("title"),
         }
 
 
 def search_animeout(session, query):
-    animeout_results = session.cf_request("GET", ANIMEOUT, params={"s": query})
+    animeout_results = session.cf_request(session, "GET", ANIMEOUT, params={"s": query})
     content = htmlparser.fromstring(animeout_results.text)
 
     for result in content.xpath('//h3[@class="post-title entry-title"]/a'):
         yield {"anime_url": result.get("href"), "name": result.text_content()}
 
 
 def search_animixplay(session, query):
@@ -158,46 +135,81 @@
     for anime in kamyroll.iter_search_results(query):
         yield {
             "anime_url": f"{scheme}://www.crunchyroll.com/{anime['type']}/{anime['media_id']}",
             "name": anime["title"],
         }
 
 
-def search_tenshi(session, query, *, domain=TENSHI):
-    uwu.bypass_ddos_guard(session, domain)
-    tenshi_page = htmlparser.fromstring(
-        session.get(domain + "anime", params={"q": query}).text
+def search_marin(session, query, *, domain=MARIN):
+    session.get(domain, headers={"range": "bytes=0-0"})
+
+    response = session.post(
+        domain + "anime",
+        json={
+            "search": query,
+        },
+        headers={
+            "x-xsrf-token": unquote(session.cookies.get("XSRF-TOKEN")),
+            "x-inertia": "true",
+        },
     )
 
-    for result in tenshi_page.cssselect(".list > li > a"):
-        yield {"name": result.get("title"), "anime_url": result.get("href")}
+    ctx.update(marin_inertia_version=response.json().get("version"))
+
+    for result in (
+        response.json().get("props", {}).get("anime_list", {}).get("data", [])
+    ):
+        yield {
+            "name": result.get("title"),
+            "anime_url": domain + "anime/" + result.get("slug"),
+        }
+
+
+def search_yugen(session, query):
+    for result in search(
+        query,
+        htmlparser.fromstring(
+            session.get(YUGEN + "discover/", params={"dq": query}).text
+        ).cssselect("a.anime-meta[href][title]"),
+        processor=lambda r: r.get("title"),
+    ):
+        yield {
+            "name": result.get("title"),
+            "anime_url": YUGEN + result.get("href")[1:],
+        }
 
 
 def search_zoro(session, query):
     for result in htmlparser.fromstring(
         session.get(ZORO + "/search", params={"keyword": query}).text
     ).cssselect("a.item-qtip[title][data-id]"):
         yield {
             "name": result.get("title"),
             "anime_url": ZORO + result.get("href")[1:-11],
         }
 
 
 def search_h_ntai_stream(session, query):
     for result in htmlparser.fromstring(
-        session.get(HENTAISTREAM + "search/", params={"s": query}).text
-    ).cssselect("article > .bsx > a"):
+        session.get(HENTAISTREAM + "search", params={"s": query}).text
+    ).cssselect("a p.text-center"):
+        anchor = result.getparent().getparent()
         yield {
-            "name": result.get("title") or result.get("oldtitle"),
-            "anime_url": HENTAISTREAM + result.get("href")[1:],
+            "name": result.text_content(),
+            "anime_url": anchor.get("href"),
         }
 
 
 def search_haho(session, query):
-    yield from search_tenshi(session, query, domain=HAHO)
+    tenshi_page = htmlparser.fromstring(
+        session.get(HAHO + "anime", params={"q": query}).text
+    )
+
+    for result in tenshi_page.cssselect(".list > li > a"):
+        yield {"name": result.get("title"), "anime_url": result.get("href")}
 
 
 provider_searcher_mapping = {
     "9anime": search_9anime,
     "animekaizoku": search_animekaizoku,
     "allanime": search_allanime,
     "animepahe": search_animepahe,
@@ -207,11 +219,12 @@
     "kamyroll": lambda *args, **kwargs: search_crunchyroll(
         *args, **kwargs, scheme="kamyroll"
     ),
     "kawaiifu": search_kawaiifu,
     "gogoanime": search_gogoanime,
     "haho": search_haho,
     "hentaistream": search_h_ntai_stream,
-    "tenshi": search_tenshi,
+    "marin": search_marin,
     "twist": search_twist,
+    "yugen": search_yugen,
     "zoro": search_zoro,
 }
```

### Comparing `ap0dl-1.5.2/ap0dl/core/cli/helpers/special.py` & `ap0dl-1.6.0/ap0dl/core/cli/helpers/special.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,17 +2,15 @@
 Special arguments parser
 """
 
 import regex
 
 SPECIAL_PARSER = regex.compile(r"(?P<special>\D+)(-?\d*)", regex.IGNORECASE)
 
-strings = {
-    "last": ["l", "latest"],
-}
+strings = {"last": ["l", "latest"], "last*": ["l*", "latest*", "latest-all"]}
 
 
 def get_qualified_name(special):
     for key, values in strings.items():
         if special.lower() in (*values, key):
             return key
 
@@ -27,15 +25,17 @@
 
         special = get_qualified_name(special)
 
         if special is None:
             continue
 
         if special == "last":
-            returnee.extend(streams[-(index or 1) :])
+            returnee.extend([streams[-(index or 1)]])
         else:
+            if special == "last*":
+                returnee.extend(streams[-(index or 1) :])
+                returnee.extend(streams[: -(index or 1)])
             """
             More specials to be thought about.
             """
 
     yield from returnee
-    yield from (stream for stream in streams if stream not in returnee)
```

### Comparing `ap0dl-1.5.2/ap0dl/core/cli/helpers/stream_handlers.py` & `ap0dl-1.6.0/ap0dl/core/cli/helpers/stream_handlers.py`

 * *Files identical despite different names*

### Comparing `ap0dl-1.5.2/ap0dl/core/codebase/downloader/ffmpeg.py` & `ap0dl-1.6.0/ap0dl/core/codebase/downloader/ffmpeg.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-import contextlib
 import logging
-import os
 import shutil
 import subprocess
 from collections import defaultdict
 
 import regex
 from tqdm import tqdm
 
+from ...cli.helpers import intelliq
+
 executable = "ffmpeg"
 
 
 def has_ffmpeg():
     return bool(shutil.which(executable))
 
 
@@ -43,17 +43,19 @@
 
     """
 
     def it():
         """
         A generator, that is made for sorting and sending to another generator.
         """
-        for match in regex.finditer(b"Stream #(\d+):(\d+): Audio:.+ (\d+) Hz", stderr):
+        for match in regex.finditer(
+            rb"Stream #(\d+):([\d()]+): Audio:.+ (\d+) Hz", stderr
+        ):
             program, stream_id, freq = (_.decode() for _ in match.groups())
-            yield "{}:a:{}".format(program, stream_id), int(freq)
+            yield f"{program}:a:{stream_id}", int(freq)
 
     yield from sorted(it(), key=lambda x: x[1], reverse=True)
 
 
 def analyze_stream(logger: logging.Logger, url: str, headers: dict):
     """
     Converts the output of `ffmpeg -i $URL` to a partial stream info default dict.
@@ -98,28 +100,45 @@
 
 def iter_quality(quality_dict):
     """
     Iterates over the quality dict returned by `analyze_stream`.
     """
     for programs, streams in quality_dict.get("streams", {}).items():
         for stream, stream_info in streams.items():
-            yield "{}:v:{}".format(programs, stream), stream_info.get("quality") or 0, (
-                stream_info.get("audio") or [None, 0]
-            )[0][0]
+            yield {
+                "video": f"{programs}:v:{stream}",
+                "audio": (stream_info.get("audio") or [[None]])[0][0],
+                "quality": stream_info.get("quality"),
+            }
 
 
 def get_last(iterable):
     """
     Gets the last element from the iterable. Pretty self-explanatory.
     """
     expansion = [*iterable]
     if expansion:
         return expansion[-1]
 
 
+def iter_from_stream(stream, *, chars=b"\r\n"):
+    """
+    Iterates over a stream, and yields the output line by line.
+    """
+    buffer = b""
+    for char in iter(lambda: stream.read(1), b""):
+        if char in chars:
+            yield buffer
+            buffer = b""
+        else:
+            buffer += char
+    if buffer:
+        yield buffer
+
+
 def ffmpeg_to_tqdm(
     logger: logging.Logger, process: subprocess.Popen, duration: int, outfile_name: str
 ) -> subprocess.CompletedProcess:
     """
     tqdm wrapper for a ffmpeg process.
 
     Takes a logger `logger`, the ffmpeg child process `process`, duration of stream
@@ -133,22 +152,22 @@
     Returns
     ---
 
     `subprocess.Popen` but completed
 
     """
     progress_bar = tqdm(
-        desc="HLS, FFMPEG / GET {}.mkv".format(outfile_name),
+        desc="FFMPEG / {}".format(outfile_name),
         total=duration,
         unit="segment",
     )
     previous_span = 0
 
-    for stream in process.stdout:
-        logger.debug("[ffmpeg] {}".format(stream.decode().strip()))
+    for stream in iter_from_stream(process.stderr):
+        logger.debug(f"[ffmpeg] {stream.decode().strip()}")
         current = get_last(regex.finditer(b"\stime=((?:\d+:)+\d+)", stream))
         if current:
             in_seconds = (
                 parse_ffmpeg_duration(current.group(1).decode()) - previous_span
             )
             previous_span += in_seconds
             progress_bar.update(in_seconds)
@@ -156,19 +175,18 @@
     progress_bar.close()
     return process
 
 
 def ffmpeg_download(
     url: str,
     headers: dict,
-    outfile_name: str,
-    content_dir,
-    preferred_quality=1080,
+    expected_download_path,
+    preferred_quality: str = "1080",
     log_level=20,
-    **opts
+    **opts,
 ) -> int:
     """
     Downloads content using ffmpeg and optionally uses tqdm to wrap the progress
     bar.
 
     Initally, it fetches content information for the stream using `analyze_stream`.
 
@@ -178,66 +196,66 @@
 
     In logging level DEBUG, it shows the ffmpeg output.
 
     Returns
     ---
 
     `int` The ffmpeg child process' return code.
-
     """
 
-    logger = logging.getLogger("ffmpeg-hls-download[{}.mkv]".format(outfile_name))
+    logger = logging.getLogger(f"ffmpeg[{expected_download_path.name}]")
     logger.debug("Using ffmpeg to download content.")
 
     stream_info = analyze_stream(logger, url, headers)
 
-    file = content_dir / ("{}.mkv".format(outfile_name))
-
-    with contextlib.suppress(FileNotFoundError, OSError):
-        os.remove(file)
+    expected_download_path.unlink(missing_ok=True)
 
     args = [executable, "-hide_banner"]
 
     if headers:
         args.extend(
             ("-headers", "\r\n".join("{}:{}".format(k, v) for k, v in headers.items()))
         )
 
-    args.extend(("-i", url, "-c", "copy", file.as_posix()))
+    args.extend(("-i", url, "-c", "copy", expected_download_path.as_posix()))
 
-    for video, quality, audio in filter(
-        lambda x: x[1] <= preferred_quality,
-        sorted(iter_quality(stream_info), key=lambda x: x[1], reverse=True),
-    ):
-        if quality < preferred_quality:
-            logger.warning(
-                "Could not find the stream of desired quality {}, currently downloading {}.".format(
-                    preferred_quality, quality or "an unknown quality"
-                )
-            )
+    qualities = list(iter_quality(stream_info))
+    ffmpeg_video = sorted(
+        intelliq.filter_quality(qualities, preferred_quality) or qualities,
+        key=lambda q: q["quality"],
+        reverse=True,
+    )[0]
 
-        child = subprocess.Popen(
-            args + ["-map", video, "-map", audio],
-            stdout=subprocess.PIPE,
-            stderr=subprocess.STDOUT,
-        )
+    ffmpeg_args = args.copy()
 
-        if log_level > 20:
-            return child.wait()
+    if ffmpeg_video["video"]:
+        ffmpeg_args.extend(("-map", ffmpeg_video["video"]))
 
-        return ffmpeg_to_tqdm(
-            logger,
-            child,
-            duration=stream_info.get("duration"),
-            outfile_name=outfile_name,
-        ).returncode
+    if ffmpeg_video["audio"]:
+        ffmpeg_args.extend(("-map", ffmpeg_video["audio"]))
 
+    logger.debug(f"Calling PIPE child process for ffmpeg: {ffmpeg_args}")
 
-def merge_subtitles(video_path, out_path, subtitle_paths, log_level=20):
+    child = subprocess.Popen(
+        ffmpeg_args,
+        stderr=subprocess.PIPE,
+    )
+
+    if log_level > 20:
+        return child.wait()
 
+    return ffmpeg_to_tqdm(
+        logger,
+        child,
+        duration=stream_info.get("duration"),
+        outfile_name=expected_download_path.name,
+    ).returncode
+
+
+def merge_subtitles(video_path, out_path, subtitle_paths, log_level=20):
     args = [
         executable,
         "-hide_banner",
         "-i",
         video_path,
         "-c:v",
         "copy",
```

### Comparing `ap0dl-1.5.2/ap0dl/core/codebase/downloader/hls.py` & `ap0dl-1.6.0/ap0dl/core/codebase/downloader/hls.py`

 * *Files identical despite different names*

### Comparing `ap0dl-1.5.2/ap0dl/core/codebase/downloader/idmanlib.py` & `ap0dl-1.6.0/ap0dl/core/codebase/downloader/idmanlib.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,74 +1,95 @@
 """
 Internet Download Manager Support.
 
 This is made strictly for Windows.
 """
 
+import pathlib
 import time
+import typing
+from collections import namedtuple
 
-IDM_MID = ["{ECF21EAB-3AA8-4355-82BE-F777990001DD}", 1, 0]
-DOWNLOAD_FOLDER = "Downloads"
+import rich
 
-idmlib, client = None, None
+authentication = namedtuple(
+    "authentication", "username password", defaults=(None, None)
+)
 
 
-def supported():
-    return bool(idmlib)
+idmlib, idmlib_object = None, None
 
 
 try:
-    import comtypes.client as cc
+    from comtypes import client
 
-    idmlib = cc.GetModule(IDM_MID)
+    idmlib = client.GetModule(["{ECF21EAB-3AA8-4355-82BE-F777990001DD}", 1, 0])
 
-    client = cc.CreateObject(
+    idmlib_object = client.CreateObject(
         idmlib.CIDMLinkTransmitter, None, None, idmlib.ICIDMLinkTransmitter2
     )
-except BaseException:
+except Exception:
     pass
 
 
-def within_range(t, t1, t2):
-    return t1 <= t <= t2
+def supported():
+    return bool(idmlib)
 
 
 def idm_download(
-    url,
-    headers={},
-    form_data="",
-    auth=(None, None),
-    filename="",
-    download_folder=DOWNLOAD_FOLDER,
-    lflag=5,
+    url: str,
+    *,
+    headers: typing.Optional[typing.Dict[str, str]] = None,
+    form_data: typing.Optional[str] = None,
+    auth: authentication = authentication(),
+    filename: typing.Optional[str] = None,
+    download_folder: pathlib.Path = pathlib.Path("."),
+    lflag: int = 5,
 ):
-    return client.SendLinkToIDM(
+    return idmlib_object.SendLinkToIDM(
         url,
-        headers.get("referer", ""),
-        headers.get("cookie", ""),
+        headers.get("referer"),
+        headers.get("cookie"),
         form_data,
-        auth[0] or "",
-        auth[1] or "",
-        download_folder,
+        auth.username,
+        auth.password,
+        download_folder.resolve(strict=True).as_posix(),
         filename,
         lflag,
     )
 
 
 def wait_until_download(
     url,
-    headers={},
-    form_data="",
-    auth=(None, None),
-    filename="",
-    download_folder=DOWNLOAD_FOLDER,
+    download_folder: pathlib.Path,
+    headers=None,
+    form_data=None,
+    auth=authentication(),
+    filename=None,
 ):
     idm_download(
-        url, headers, form_data, auth, filename, download_folder.as_posix(), lflag=5
+        url,
+        headers=headers,
+        form_data=form_data,
+        auth=auth,
+        filename=filename,
+        download_folder=download_folder,
+        lflag=5,
     )
+
+    if filename is None:
+        return
+
     while not (download_folder / filename).exists():
         try:
             time.sleep(0.5)
         except KeyboardInterrupt:
-            return print(
-                "[IDM] Interrupted the wait for current download completion. Continuing with the next in queue."
+            console = rich.get_console()
+
+            console.print(
+                "[bold red]Detected KeyboardInterrupt[/], continue or terminate?",
             )
+
+            if console.input("[C/t]: ").lower() == "t":
+                raise
+
+            return
```

### Comparing `ap0dl-1.5.2/ap0dl/core/codebase/extractors/dailymotion/__init__.py` & `ap0dl-1.6.0/ap0dl/core/codebase/extractors/dailymotion/__init__.py`

 * *Files identical despite different names*

### Comparing `ap0dl-1.5.2/ap0dl/core/codebase/extractors/doodstream/__init__.py` & `ap0dl-1.6.0/ap0dl/core/codebase/extractors/doodstream/__init__.py`

 * *Files identical despite different names*

### Comparing `ap0dl-1.5.2/ap0dl/core/codebase/extractors/gogoplay/__init__.py` & `ap0dl-1.6.0/ap0dl/core/codebase/extractors/gogoplay/__init__.py`

 * *Files identical despite different names*

### Comparing `ap0dl-1.5.2/ap0dl/core/codebase/extractors/mp4upload/__init__.py` & `ap0dl-1.6.0/ap0dl/core/codebase/extractors/mp4upload/__init__.py`

 * *Files identical despite different names*

### Comparing `ap0dl-1.5.2/ap0dl/core/codebase/extractors/okru/__init__.py` & `ap0dl-1.6.0/ap0dl/core/codebase/extractors/okru/__init__.py`

 * *Files identical despite different names*

### Comparing `ap0dl-1.5.2/ap0dl/core/codebase/extractors/rapidvideo/polling.py` & `ap0dl-1.6.0/ap0dl/core/codebase/extractors/rapidvideo/polling.py`

 * *Files identical despite different names*

### Comparing `ap0dl-1.5.2/ap0dl/core/codebase/extractors/streamlare/__init__.py` & `ap0dl-1.6.0/ap0dl/core/codebase/extractors/streamlare/__init__.py`

 * *Files identical despite different names*

### Comparing `ap0dl-1.5.2/ap0dl/core/codebase/extractors/streamsb/__init__.py` & `ap0dl-1.6.0/ap0dl/core/codebase/extractors/streamsb/__init__.py`

 * *Files identical despite different names*

### Comparing `ap0dl-1.5.2/ap0dl/core/codebase/extractors/streamtape/__init__.py` & `ap0dl-1.6.0/ap0dl/core/codebase/extractors/streamtape/__init__.py`

 * *Files identical despite different names*

### Comparing `ap0dl-1.5.2/ap0dl/core/codebase/extractors/vidstream/__init__.py` & `ap0dl-1.6.0/ap0dl/core/codebase/providers/animtime/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,94 +1,66 @@
 import functools
-import json
-from base64 import b64decode
+from functools import partial
 
-import regex
+from ap0dl.utils.optopt import regexlib
 
-from ...providers.nineanime import decipher
+from ....config import ANIMTIME
+from ...helpers import construct_site_based_regex
 
-EMBED_URL_REGEX = regex.compile(r"(.+?/)(?:e(?:mbed)?)/([a-zA-Z0-9]+)")
+CONTENT_RE = regexlib.compile(r't\[t\.(?P<name>.+?)=(?P<id>\d+)\]="\1"')
+REGEX = construct_site_based_regex(ANIMTIME, extra_regex=r"/title/([^/?&]+)")
 
-SIMPLE_OPERATE_REGEX = regex.compile(r"[0-9]+\s+.+?\s+[0-9]+")
+MAIN_JS_RE = regexlib.compile(r'<script src="(main\..+?\.js)".+?>')
 
 
-CIPHER_ALGORITHM_DATA_ENDPOINT = (
-    "https://raw.githubusercontent.com/AnimeJeff/Overflow/main/syek"
-)
-
-
-def isolated_eval(code, *, builtins=None):
-    try:
-        return eval(code, {"__builtins__": builtins or {}}, {})
-    except Exception:
-        return None
+def get_content(content_id, js_content):
+    for content in CONTENT_RE.finditer(js_content):
+        if content.group("id") == content_id:
+            return content.group("name")
 
 
 @functools.lru_cache()
-def get_ciper_algorithm(session):
-    return json.loads(
-        b64decode(
-            b64decode(b64decode(session.get(CIPHER_ALGORITHM_DATA_ENDPOINT).content))
-        ).decode()
-    )
-
-
-def string_encrypt(text):
-    def repl(match):
-        value = ord(match.group(0)) + 13
-        return chr(
-            value if (90 if ord(match.group(0)) <= 90 else 122) >= value else value - 26
-        )
-
-    return regex.sub(r"[a-zA-Z]", repl, text)
+def get_js_content(session):
+    content = session.get(ANIMTIME).text
+    main_js = MAIN_JS_RE.search(content).group(1)
 
+    return session.get(ANIMTIME + main_js).text
 
-def conditional_encrypt(content, steps, b64_table):
 
-    for _ in steps:
-        if _ == "o":
-            content = decipher.encrypt(content, table=b64_table).replace("/", "_")
+def fetcher(session, url, check, match):
 
-        if _ == "s":
-            content = string_encrypt(content)
+    content = get_js_content(session)[374391:]
 
-        if _ == "a":
-            content = content[::-1]
+    anime = get_content(match.group(1), content)
 
-    return content
+    if anime is None:
+        return
 
-
-def extract(session, url, **opts):
-
-    match = EMBED_URL_REGEX.search(url)
-    algorithm = get_ciper_algorithm(session)
-
-    b64_table = algorithm["encryptKey"]
-
-    content_id = decipher.encrypt(
-        decipher.cipher_keyed(algorithm["cipherKey"], match.group(2)),
-        table=b64_table,
+    episode_count = int(
+        regexlib.search(rf"Ld\[Kd\.{regexlib.escape(anime)}\]=(\d+)", content).group(1)
     )
 
-    operations = algorithm["operations"]
+    constructor, end = regexlib.search(
+        regexlib.escape(f"Fd[Kd.{anime}]=function(t){{return")
+        + '"(.+?)"'
+        + regexlib.escape("+t+")
+        + r'"(.+?)"\}',
+        content,
+    ).groups()
+
+    for episode in range(1, episode_count + 1):
+        if check(episode):
+            yield partial(
+                lambda x: [{"stream_url": x, "headers": {"referer": ANIMTIME}}],
+                constructor + "{:03d}".format(episode) + end,
+            ), episode
+
+
+def metadata_fetcher(session, url, match):
+    content = get_js_content(session)[374391:]
 
-    dashes = conditional_encrypt(
-        "-".join(
-            str(
-                isolated_eval(
-                    str(ord(character)) + operations[str(count % len(operations))]
-                )
-            )
-            for count, character in enumerate(
-                conditional_encrypt(content_id, algorithm["pre"], b64_table)
-            )
-        ),
-        algorithm["post"],
-        b64_table,
-    )
+    anime_name = get_content(match.group(1), content)
 
-    vidstream_info = session.get(f"{match.group(1)}/{algorithm['mainKey']}/{dashes}")
+    if anime_name is not None:
+        anime_name = " ".join(regexlib.split(r"(?=[A-Z])", anime_name)).strip()
 
-    return [
-        {"stream_url": content.get("file", ""), "headers": {"referer": url}}
-        for content in vidstream_info.json()["data"].get("media", {}).get("sources", [])
-    ]
+    return {"titles": [anime_name]}
```

### Comparing `ap0dl-1.5.2/ap0dl/core/codebase/helpers/__init__.py` & `ap0dl-1.6.0/ap0dl/core/codebase/helpers/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 from collections import defaultdict
 from typing import Callable, DefaultDict, Dict, List, TypeVar
 
 import anitopy
+from anchor.strings import regexify_url
 
-from . import optopt
+from ap0dl.utils import optopt
+
+from . import superscrapers
 
 content_type = TypeVar("content_type")
 
 
 def construct_site_based_regex(
     site_url: "str", *, extra: "str" = "", extra_regex: "str" = ""
 ):
-    return optopt.regexlib.compile(
-        "(?:https?://)?(?:\\S+\\.)*{}".format(
-            optopt.regexlib.escape(
-                optopt.regexlib.search(
-                    r"(?:https?://)?((?:\S+\.)+[^/]+)/?", site_url
-                ).group(1)
-            )
-            + extra
-        )
-        + extra_regex
+    return regexify_url(
+        site_url,
+        extra=extra,
+        extra_re=extra_regex,
+        match_subdomains=False,
+        retain_scheme=False,
     )
 
 
 def append_protocol(uri: "str", *, protocol: "str" = "https"):
 
     if optopt.regexlib.search(r"^.+?://", uri):
         return uri
```

### Comparing `ap0dl-1.5.2/ap0dl/core/codebase/helpers/uwu.py` & `ap0dl-1.6.0/ap0dl/core/codebase/helpers/uwu.py`

 * *Files identical despite different names*

### Comparing `ap0dl-1.5.2/ap0dl/core/codebase/providers/__init__.py` & `ap0dl-1.6.0/ap0dl/core/codebase/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `ap0dl-1.5.2/ap0dl/core/codebase/providers/allanime/__init__.py` & `ap0dl-1.6.0/ap0dl/core/codebase/providers/allanime/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,180 +1,208 @@
 from collections import defaultdict
 from functools import partial
 
 import yarl
 
-from ....config import (
-    ALLANIME,
-    SUPERANIME_CRUNCHYROLL,
-    SUPERANIME_RETURN_ALL,
-    SUPERANIME_TYPE_OF,
-)
-from ...helpers import construct_site_based_regex, optopt
-from .superscrapers import iter_unpacked_from_packed_hls
+from ....config import ALLANIME, SUPERANIME_RETURN_ALL, SUPERANIME_TYPE_OF
+from ...helpers import construct_site_based_regex, optopt, superscrapers
+from .gql_api import api
 
-REGEX = construct_site_based_regex(ALLANIME, extra_regex=r"/anime/([^?&/]+)")
+REGEX = construct_site_based_regex(ALLANIME, extra_regex=r"/(?:anime|watch)/([^?&/]+)")
 
-SOURCE_EMBED_REGEX = optopt.regexlib.compile(
-    r'<iframe id="episode-frame" .+? src="(.+?)"'
-)
-SOURCE_URLS = optopt.regexlib.compile(
-    r'sourceUrl[:=]"(?P<url>.+?)"[;,](?:.+?\.)?priority[:=](?P<priority>.+?)[;,](?:.+?\.)?sourceName[:=](?P<name>.+?)[,;]'
+LEGACY_CONTENT_REGEX = optopt.regexlib.compile(
+    r'date:g,data:"({.+?})"}},calling:', optopt.regexlib.DOTALL
 )
-EPISODES_REGEX = optopt.regexlib.compile(r'\\"availableEpisodesDetail\\":({.+?})')
-TITLES_REGEX = optopt.regexlib.compile(r'<span class="mr-1">(.+?);?</span>')
-
-EMBED_RESOLVERS = {
-    '"Ok"': "okru",
-    '"Vid-mp4"': "gogoanime",
-    '"Mp4"': "mp4upload",
-    '"Sl-mp4"': "streamlare",
-    '"Ss-Hls"': "streamsb",
-}
 
 
 def iter_episodes(
     episode_dictionary: dict,
-    anime_page_url: str,
     *,
     selected_type_of: str = SUPERANIME_TYPE_OF,
 ):
     episodes = defaultdict(list)
 
     for type_of, episode_numbers in episode_dictionary.items():
         if type_of != selected_type_of:
             continue
 
         for episode in episode_numbers:
             episodes[int(episode) if episode.isdigit() else 0].append(
-                anime_page_url + "/episodes/{}/{}".format(type_of, episode)
+                (type_of, episode)
             )
 
     yield from sorted(episodes.items(), key=lambda x: x[0])
 
 
-def unicode_escape(string: str):
-    return string.encode("utf-8").decode("unicode_escape")
+def to_clock_json(url: str):
+    parsed = yarl.URL(url)
+    return parsed.with_name("clock.json").with_query(parsed.query).human_repr()
 
 
-def to_json_url(url: "yarl.URL"):
-    return url.with_name(url.name + ".json").with_query(url.query)
+def fetch_legacy(session, episode, type_of, show_id):
+    """
+    This is a fallback method for fetching the content of an episode
+    when the GQL hits server-side rate-limits.
+    """
+
+    match = LEGACY_CONTENT_REGEX.search(
+        session.get(
+            ALLANIME + f"watch/{show_id}//episode-{episode}-{type_of}",
+        ).text
+    )
 
+    if match:
+        return (
+            optopt.jsonlib.loads(match.group(1).replace('\\"', '"'))
+            .get("data", {})
+            .get("episode", {})
+        )
 
-def iter_prioritised(session, urls):
+    return {}
 
-    for url, (priority, name) in urls:
-        data = session.get(url.human_repr()).text
 
-        if data == "Wrongerror":
-            continue
+def one_digit_symmetric_xor(password: int, target: str):
+    def genexp():
+        for segment in bytearray.fromhex(target):
+            yield segment ^ password
 
-        json_parsed = optopt.jsonlib.loads(data)["links"]
+    return bytes(genexp()).decode("utf-8")
 
-        if isinstance(json_parsed, dict) and json_parsed.get("type") == "Not Found":
-            continue
 
-        def iter_all():
-            for link in json_parsed:
+def extract_content(
+    session,
+    content: "iter_episodes",
+    show_id: str,
+    *,
+    api_endpoint: str,
+    return_all: bool = SUPERANIME_RETURN_ALL,
+):
+    for type_of, episode in content:
+        api_response = api.fetch_episode(
+            session, show_id, episode, translation_type=type_of
+        )
 
-                stream_attr = {}
+        episode_info = api_response.get("episode") or fetch_legacy(
+            session, episode, type_of, show_id
+        )
 
-                if "resolution" in link:
-                    stream_attr["quality"] = link["resolution"]
+        if not episode_info:
+            continue
 
-                if "subtitles" in link:
-                    stream_attr["subtitle"] = [_["src"] for _ in link["subtitles"]]
+        attrs = {}
 
-                if "resolutionStr" in link:
-                    stream_attr["vrv"] = {
-                        "stream_type": link["resolutionStr"],
-                        "provider_configuration": SUPERANIME_CRUNCHYROLL,
-                    }
+        if "notes" in episode_info and episode_info["notes"]:
+            attrs.update(title=episode_info["notes"].replace("<note-split>", " // "))
 
-                stream_url = link["link"]
+        sources = sorted(
+            episode_info["sourceUrls"],
+            key=lambda value: value.get("priority", 0),
+            reverse=True,
+        )
 
-                yield from (
-                    iter_unpacked_from_packed_hls(
-                        session, yarl.URL(stream_url), stream_attribs=stream_attr
-                    )
+        if not sources:
+            continue
+
+        for source in sources:
+            if source["sourceUrl"][:2] == "--":
+                source["sourceUrl"] = one_digit_symmetric_xor(
+                    56, source["sourceUrl"][2:]
                 )
 
-        yield list(iter_all())
+            if source["sourceUrl"][0] == "/":
+                response = session.get(
+                    to_clock_json(api_endpoint + source["sourceUrl"])
+                )
 
+                if response.text in ("error", "error no result"):
+                    continue
 
-def extract_content(
-    session,
-    content: "iter_episodes",
-    *,
-    api_endpoint: "yarl.URL",
-    return_all: bool = SUPERANIME_RETURN_ALL,
-):
+                streams = response.json().get("links")
 
-    for url in content:
+                if not streams:
+                    continue
 
-        direct_providers = set()
-        embed_providers = set()
+                for stream_data in streams:
+                    subtitles = list(
+                        map(
+                            lambda subtitles: subtitles["src"],
+                            stream_data.get("subtitles", []),
+                        )
+                    )
 
-        content_page = session.get(url).text
+                    attrs.setdefault("subtitle", [])
+                    attrs["subtitle"].extend(subtitles)
 
-        has_on_embed = SOURCE_EMBED_REGEX.search(content_page)
+                    if "rawUrls" in stream_data and stream_data["rawUrls"]:
+                        audio_tracks = list(
+                            map(
+                                lambda data: data["url"],
+                                stream_data["rawUrls"].get("audios", []),
+                            )
+                        )
+
+                        for data in stream_data["rawUrls"]["vids"]:
+                            yield {
+                                "quality": data["height"],
+                                "stream_url": data["url"],
+                                "audio_tracks": audio_tracks,
+                                **attrs,
+                            }
+
+                        continue
+
+                    if "link" in stream_data and stream_data["link"]:
+                        url = stream_data["link"]
+                    else:
+                        if not stream_data["portData"]["streams"]:
+                            continue
 
-        if has_on_embed:
-            direct_providers.add(
-                (to_json_url(yarl.URL(has_on_embed.group(1))), ("", "embed"))
-            )
+                        stream = stream_data["portData"]["streams"][0]
 
-        for source_urls in SOURCE_URLS.finditer(content_page):
+                        url = stream["url"]
 
-            raw_url = unicode_escape(source_urls.group(1))
-            parsed_url = yarl.URL(raw_url)
+                    yield from superscrapers.iter_unpacked_from_packed_hls(
+                        session, yarl.URL(url), stream_attribs=attrs
+                    )
 
-            priority, name = source_urls.group("priority", "name")
+                    if not return_all:
+                        return
 
-            if parsed_url.host is None:
-                parsed_url = api_endpoint.join(to_json_url(parsed_url))
-                direct_providers.add((parsed_url, (priority, name)))
             else:
-                embed_providers.add((parsed_url, (priority, name)))
-
-        iterator = iter_prioritised(
-            session, sorted(direct_providers, key=lambda x: x[1][0])
-        )
-
-        if return_all:
-            yield from iterator
-        else:
-            child = next(iterator, None)
-
-            if child is not None:
-                yield from child
+                yield from superscrapers.iter_unpacked_from_packed_hls(
+                    session, yarl.URL(source["sourceUrl"]), stream_attribs=attrs
+                )
+                if not return_all:
+                    return
 
 
 def fetcher(session, url: "str", check, match):
-    anime_url = ALLANIME + f"anime/{match.group(1)}"
-
-    api_endpoint = yarl.URL(
+    api_endpoint = (
         session.get(ALLANIME + "getVersion").json().get("episodeIframeHead", "")
     )
 
-    for episode, content in iter_episodes(
-        optopt.jsonlib.loads(
-            EPISODES_REGEX.search(session.get(anime_url).text)
-            .group(1)
-            .replace('\\"', '"')
-        ),
-        anime_url,
-    ):
+    available_episodes = api.fetch_show_info(
+        session,
+        match.group(1),
+    ).get("availableEpisodesDetail", {})
+
+    for episode, content in iter_episodes(available_episodes):
         if check(episode):
             yield partial(
-                lambda session, content: list(
-                    extract_content(session, content, api_endpoint=api_endpoint)
+                lambda session, content, show_id: list(
+                    extract_content(
+                        session, content, show_id, api_endpoint=api_endpoint
+                    )
                 ),
                 session,
                 content,
+                match.group(1),
             ), episode
 
 
 def metadata_fetcher(session, url: "str", match):
-    anime_url = ALLANIME + f"anime/{match.group(1)}"
+    anime_name = api.fetch_show_info(
+        session,
+        match.group(1),
+    ).get("name", "")
 
-    return {"titles": TITLES_REGEX.findall(session.get(anime_url).text)}
+    return {"titles": [anime_name]}
```

### Comparing `ap0dl-1.5.2/ap0dl/core/codebase/providers/allanime/superscrapers.py` & `ap0dl-1.6.0/ap0dl/core/codebase/helpers/superscrapers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import yarl
 
-from ... import helpers
+from ap0dl.utils.optopt import regexlib
 
-VRV_RESPONSE_REGEX = helpers.optopt.regexlib.compile(
+VRV_RESPONSE_REGEX = regexlib.compile(
     r"^#EXT-X-STREAM-INF:.*?RESOLUTION=\d+x(?P<resolution>\d+).*?\n(.+?)$",
-    flags=helpers.optopt.regexlib.MULTILINE,
+    flags=regexlib.MULTILINE,
 )
-WIXMP_URL_REGEX = helpers.optopt.regexlib.compile(
+WIXMP_URL_REGEX = regexlib.compile(
     r"https://.+?/(?P<base>.+?/),(?P<resolutions>(?:\d+p,)+)"
 )
 
 
 def iter_ufph_vrv(session, url: yarl.URL, *, stream_attribs=None):
 
     if stream_attribs is not None:
```

### Comparing `ap0dl-1.5.2/ap0dl/core/codebase/providers/animekaizoku/__init__.py` & `ap0dl-1.6.0/ap0dl/core/codebase/providers/animekaizoku/__init__.py`

 * *Files identical despite different names*

### Comparing `ap0dl-1.5.2/ap0dl/core/codebase/providers/animeonsen/__init__.py` & `ap0dl-1.6.0/ap0dl/core/codebase/providers/animeonsen/__init__.py`

 * *Files identical despite different names*

### Comparing `ap0dl-1.5.2/ap0dl/core/codebase/providers/animeout/__init__.py` & `ap0dl-1.6.0/ap0dl/core/codebase/providers/animeout/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     if host_prefix in public_domains:
         url = url.with_host(f"{public_domains[host_prefix]}.{_}")
 
     return url.human_repr()
 
 
 def fetcher(session, url, check, match):
-    animeout_page = session.cf_request("GET", url)
+    animeout_page = session.cf_request(session, "GET", url)
     parsed = htmlparser.fromstring(animeout_page.text)
 
     downloadables = (
         yarl.URL(_.get("href"))
         for _ in parsed.cssselect('.article-content a[href$="mkv"]')
         if "Download" in _.text_content()
     )
```

### Comparing `ap0dl-1.5.2/ap0dl/core/codebase/providers/animepahe/__init__.py` & `ap0dl-1.6.0/ap0dl/core/codebase/providers/animepahe/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,75 +1,68 @@
 import functools
+from math import ceil
 
-import regex
+from ap0dl.utils import optopt
 
 from ....config import ANIMEPAHE
 from ...helpers import construct_site_based_regex
 from .inner import get_animepahe_url
 
 REGEX = construct_site_based_regex(ANIMEPAHE, extra_regex=r"/(anime|play)/([^?&/]+)")
 
-ID_RE = regex.compile(r'let id = "(.+?)"')
-KWIK_RE = regex.compile(r"Plyr\|(.+?)'")
+ID_RE = optopt.regexlib.compile(r'let id = "(.+?)"')
+KWIK_RE = optopt.regexlib.compile(r"Plyr\|(.+?)'")
 
-TITLES_REGEX = regex.compile(r"<h1>(.+?)</h1>")
+STREAMS_REGEX = optopt.regexlib.compile(
+    r'<a href="(?P<url>.+?)" .+? class="dropdown-item">.+? (?P<resolution>\d+)p.+?</a>'
+)
+
+TITLES_REGEX = optopt.regexlib.compile(r"<h1>(.+?)</h1>")
 
 
 def get_streams_from_embed_url(session, embed_uri):
     embed_page = session.get(embed_uri, headers={"referer": ANIMEPAHE}).text
     return "{}://{}-{}.{}.{}.{}/{}/{}/{}/{}.{}".format(
         *KWIK_RE.search(embed_page).group(1).split("|")[::-1]
     )
 
 
 def iter_stream_url_from_stream_session(session, release_id, stream_session):
-
     stream_url_data = session.get(
-        ANIMEPAHE + "api",
-        params={"m": "links", "id": release_id, "session": stream_session, "p": "kwik"},
+        ANIMEPAHE + f"play/{release_id}/{stream_session}",
     )
 
-    for qualities in stream_url_data.json().get("data", []):
-        for quality, data in qualities.items():
-            yield {
-                "quality": quality,
-                "stream_url": get_animepahe_url(session, data["kwik_pahewin"]),
-            }
+    for url, resolution in STREAMS_REGEX.findall(stream_url_data.text):
+        yield {
+            "quality": int(resolution),
+            "stream_url": get_animepahe_url(session, url),
+        }
 
 
 def iter_episode_streams(session, release_id, per_page, episode_number):
-
-    current_page = episode_number // per_page + 1
+    current_page = ceil(episode_number / per_page)
 
     episode = fetch_session(session, release_id, page=current_page)["data"][
         episode_number % per_page - 1
     ]
 
     yield from iter_stream_url_from_stream_session(
         session, release_id, episode["session"]
     )
 
 
-def bypass_ddos_guard(session):
-    js_bypass_uri = regex.search(
-        r"'(.*?)'", session.get("https://check.ddos-guard.net/check.js").text
-    ).group(1)
-    session.cookies.update(session.get(ANIMEPAHE + js_bypass_uri).cookies)
-
-
 @functools.lru_cache()
 def fetch_session(session, release_id, *, page=None):
     return session.get(
         ANIMEPAHE + "api",
         params={"m": "release", "id": release_id, "sort": "episode_asc", "page": page},
     ).json()
 
 
 def fetcher(session, url, check, match):
-
     if match.group(1) == "play":
         url = ANIMEPAHE + f"anime/{match.group(2)}"
 
     anime_page = session.get(url)
 
     release_id = ID_RE.search(anime_page.text).group(1)
```

### Comparing `ap0dl-1.5.2/ap0dl/core/codebase/providers/animepahe/inner/__init__.py` & `ap0dl-1.6.0/ap0dl/core/codebase/providers/animepahe/inner/__init__.py`

 * *Files identical despite different names*

### Comparing `ap0dl-1.5.2/ap0dl/core/codebase/providers/animepahe/inner/archive.py` & `ap0dl-1.6.0/ap0dl/core/codebase/providers/animepahe/inner/archive.py`

 * *Files identical despite different names*

### Comparing `ap0dl-1.5.2/ap0dl/core/codebase/providers/animexin/__init__.py` & `ap0dl-1.6.0/ap0dl/core/codebase/providers/animexin/__init__.py`

 * *Files identical despite different names*

### Comparing `ap0dl-1.5.2/ap0dl/core/codebase/providers/animixplay/hardstream.py` & `ap0dl-1.6.0/ap0dl/core/codebase/providers/animixplay/hardstream.py`

 * *Files identical despite different names*

### Comparing `ap0dl-1.5.2/ap0dl/core/codebase/providers/animixplay/stream_url.py` & `ap0dl-1.6.0/ap0dl/core/codebase/providers/animixplay/stream_url.py`

 * *Files identical despite different names*

### Comparing `ap0dl-1.5.2/ap0dl/core/codebase/providers/crunchyroll/__init__.py` & `ap0dl-1.6.0/ap0dl/core/codebase/providers/crunchyroll/__init__.py`

 * *Files identical despite different names*

### Comparing `ap0dl-1.5.2/ap0dl/core/codebase/providers/gogoanime/__init__.py` & `ap0dl-1.6.0/ap0dl/core/codebase/providers/gogoanime/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     GOGOANIME,
     extra_regex=r"/(?:(?P<episode_anime_slug>[^&?/]+)-episode-[\d-]+|category/(?P<anime_slug>[^&?/]+))",
 )
 
 ANIME_ID_REGEX = regex.compile(r'<input.+?value="(\d+)" id="movie_id"')
 EPISODE_LOAD_AJAX = "https://ajax.gogo-load.com/ajax/load-list-episode"
 
-TITLES_REGEX = regex.compile(r'<a href="/category/.+?" title=".+?">(.+?)</a>')
+TITLES_REGEX = regex.compile(r"<h1>(.+?)</h1>")
 
 
 def get_episode_list(session, anime_id):
     """
     Fetch all the episodes' url from GogoAnime using.
     """
     episode_page = session.get(
@@ -31,15 +31,15 @@
     )
     genexp = iter(
         htmlparser.fromstring(episode_page.text).cssselect(
             'a[class=""] , a[class=""]  > div.name'
         )
     )
 
-    for (a, div) in zip(genexp, genexp):
+    for a, div in zip(genexp, genexp):
         episode = div.text_content().split(" ")[1]
         yield float(episode) if "." in episode else int(episode), GOGOANIME + a.get(
             "href"
         ).strip(),
 
 
 def get_quality(url_text):
@@ -47,21 +47,20 @@
     if not match:
         return None
     return int(match.group(1))
 
 
 def get_embed_page(session, episode_url):
     content_parsed = htmlparser.fromstring(session.get(episode_url).text)
-    return "https:{}".format(content_parsed.cssselect("iframe")[0].get("src"))
+    return content_parsed.cssselect("iframe")[0].get("src")
 
 
 def fetcher(session, url, check, match):
-
     if match.group("episode_anime_slug"):
-        url = "{}category/{}".format(GOGOANIME, match.group("episode_anime_slug"))
+        url = f"{GOGOANIME}category/{match.group('episode_anime_slug')}"
 
     content_id = ANIME_ID_REGEX.search(session.get(url).text).group(1)
 
     for episode, episode_page in reversed(list(get_episode_list(session, content_id))):
         if check(episode):
             yield partial(
                 lambda e: [
```

### Comparing `ap0dl-1.5.2/ap0dl/core/codebase/providers/hentaistream/__init__.py` & `ap0dl-1.6.0/ap0dl/core/codebase/providers/hentaistream/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -6,56 +6,70 @@
 from ....config import HENTAISTREAM
 from ...helpers import construct_site_based_regex
 
 EPISODE_REGEX = regex.compile(r"/\d+/[^&?/]+")
 TITLES_REGEX = regex.compile(r'<h1 class="entry-title" itemprop="name">(.+?)</h1>')
 
 
-REGEX = construct_site_based_regex(
-    HENTAISTREAM, extra_regex=r"/hentai/([^?&/]+)(?:/\d+)?"
-)
+REGEX = construct_site_based_regex(HENTAISTREAM, extra_regex=r"/hentai/([^?&/]+)")
 
 EXTRACTOR_REGEX = regex.compile(r"src: '(.+?)',\s+type: '.+?',\s+size: (\d+),")
 SUBTITLE_URL_REGEX = regex.compile(r"subUrl: '(.+?)'")
 
 
 def fetch_streams(session, episode_url, **opts):
-
     episode_page = session.get(HENTAISTREAM + episode_url[1:]).text
     subtitles = SUBTITLE_URL_REGEX.findall(episode_page)
 
     for url, size in EXTRACTOR_REGEX.findall(episode_page):
-
         yield {
             "stream_url": url,
             "quality": int(size),
             "headers": {"referer": HENTAISTREAM},
             "subtitle": subtitles,
         }
 
 
 def fetcher(session, url, check, match):
+    response = session.get(match.group(0))
+    episode_page = htmlparser.fromstring(response.text)
 
-    episodes_page = htmlparser.fromstring(
-        session.get(HENTAISTREAM + f"hentai/" + match.group(1)).text
-    )
-
-    for urls in episodes_page.cssselect("div.eplister a"):
-        number, title, date = map(
-            htmlparser.HtmlElement.text_content, urls.cssselect('div[class^="epl"]')
-        )
-
-        episode_number = int(number) if number.isdigit() else 0
-
-        if check(episode_number):
-            yield partial(
-                lambda url, **opts: list(fetch_streams(session, url, **opts)),
-                urls.get("href"),
-                title=f"{title} ({date})",
-            ), episode_number
+    episode_id = episode_page.cssselect("input#e_id")[0].get("value")
+    csrf = response.cookies.get("XSRF-TOKEN")
 
+    data = session.post(
+        HENTAISTREAM + "player/api",
+        json={
+            "episode_id": episode_id,
+        },
+        headers={
+            "x-xsrf-token": csrf.replace("%3D", "="),
+        },
+    ).json()
+
+    resolutions = (1080, 720)
+
+    if data["resolution"] == "4k":
+        resolutions = (2160,) + resolutions
+
+    yield partial(
+        lambda _: _,
+        [
+            {
+                "title": data["title"],
+                "stream_url": data["stream_domains"][-1]
+                + "/"
+                + data["stream_url"]
+                + f"/{resolution}/manifest.mpd",
+                "subtitle": [
+                    data["stream_domains"][-1] + "/" + data["stream_url"] + f"/eng.ass",
+                ],
+                "quality": resolution,
+            }
+            for resolution in resolutions
+        ],
+    ), 1
 
-def metadata_fetcher(session, url, match):
 
-    episode_url = HENTAISTREAM + f"hentai/" + match.group(1)
-
-    return {"titles": TITLES_REGEX.findall(session.get(episode_url).text)}
+def metadata_fetcher(session, url, match):
+    page = htmlparser.fromstring(session.get(match.group(0)).text)
+    return {"titles": page.cssselect("h1.leading-tight")[0].text_content().strip()}
```

### Comparing `ap0dl-1.5.2/ap0dl/core/codebase/providers/kamyroll/__init__.py` & `ap0dl-1.6.0/ap0dl/core/codebase/providers/kamyroll/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -49,26 +49,19 @@
             _
             for _ in streams_data["streams"]
             if _["hardsub_locale"] == superanime_subtitle
         ] or streams_data["streams"]
         subtitles = streams_data["subtitles"]
 
         for stream in selected_streams:
-            hls_response = api.session.get(stream["url"]).text
-
-            for match in VRV_RESPONSE_REGEX.finditer(hls_response):
-
-                url_base, _, policies = match.group(2).partition("/index-v1-a1.m3u8")
-
-                yield {
-                    "stream_url": url_base + policies,
-                    "quality": int(match.group(1)),
-                    "subtitle": [fix_subtitle_url(_["url"]) for _ in subtitles],
-                    **stream_attrs,
-                }
+            yield {
+                "stream_url": stream["url"],
+                "subtitle": [fix_subtitle_url(_["url"]) for _ in subtitles],
+                **stream_attrs,
+            }
 
 
 @lru_cache()
 def fetch_episodes(api: Kamyroll, media_id):
     seasons = api.fetch_seasons(media_id)["items"]
     episodes = defaultdict(list)
```

### Comparing `ap0dl-1.5.2/ap0dl/core/codebase/providers/kamyroll/api.py` & `ap0dl-1.6.0/ap0dl/core/codebase/providers/kamyroll/api.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,24 +14,24 @@
         self.raw_token = {}
 
     def get_token(self):
         expires = self.raw_token.get("expires_in", 0)
 
         if expires < time.time():
 
-            response = self.session.post(
+            response = self.session.get(
                 self.API_URL + "auth/v1/token",
-                data={
+                params={
                     "device_id": "web",
-                    "device_type": "python.animdl",
+                    "device_type": "python.ap0dl",
                     "access_token": "HMbQeThWmZq4t7w",
                 },
-            ).json()
+            )
 
-            self.raw_token = response
+            self.raw_token = response.json()
         else:
             return f"{self.raw_token['token_type']} {self.raw_token['access_token']}"
 
         return self.get_token()
 
     def fetch_seasons(self, media_id, *, channel_id="crunchyroll", locale="en-US"):
         return self.session.get(
```

### Comparing `ap0dl-1.5.2/ap0dl/core/codebase/providers/kawaiifu/__init__.py` & `ap0dl-1.6.0/ap0dl/core/codebase/providers/kawaiifu/__init__.py`

 * *Files identical despite different names*

### Comparing `ap0dl-1.5.2/ap0dl/core/codebase/providers/nineanime/__init__.py` & `ap0dl-1.6.0/ap0dl/core/codebase/providers/nineanime/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,78 +1,82 @@
 from functools import partial
 
 import lxml.html as htmlparser
 import regex
 
 from ....config import NINEANIME
 from ...helpers import construct_site_based_regex
-from .decipher import decrypt_url
+from .decipher import vrf_api
 
 CONTENT_ID_REGEX = regex.compile(r'data-id="(.+?)"')
 
 REGEX = construct_site_based_regex(
     NINEANIME, extra_regex=r"/watch/[^&?/]+\.(?P<slug>[^&?/]+)"
 )
-TITLES_REGEX = regex.compile(r'<h1 class="title d-title" .+?>(.+?)</h1>')
+TITLES_REGEX = regex.compile(r'<h1 .+? class="title d-title" .+?>(.+?)</h1>')
 
 SOURCES = {
     "41": "vidstream",
     "28": "mycloud",
     "35": "mp4upload",
     "40": "streamtape",
     "43": "videovard",
     "44": "filemoon",
 }
 
-DECRYPTION_CODE = "hlPeNwkncH0fq9so"
-
 
 def fetch_episode(session, data_source):
+    episode_ids = data_source.get("data-ids")
 
     response = htmlparser.fromstring(
         session.get(
-            NINEANIME + f"ajax/server/list/{data_source.get('data-ids')}"
+            NINEANIME + f"ajax/server/list/{episode_ids}",
+            params={"vrf": vrf_api(session, episode_ids)},
         ).json()["result"]
     )
 
     for content_type_container in response.cssselect("div[data-type]"):
-
         for servers in content_type_container.cssselect("ul > li[data-sv-id]"):
-
             source = SOURCES[servers.get("data-sv-id")]
+            link_id = servers.get("data-link-id")
+
+            enc_content_url = session.get(
+                NINEANIME + f"ajax/server/{link_id}",
+                params={"vrf": vrf_api(session, link_id)},
+            ).json()["result"]["url"]
+
+            content_url = vrf_api(session, enc_content_url, endpoint="decrypt")
 
-            content_url = decrypt_url(
-                session.get(
-                    NINEANIME + f"ajax/server/{servers.get('data-link-id')}/"
-                ).json()["result"]["url"],
-                DECRYPTION_CODE,
-            )
             yield {
                 "stream_url": content_url,
                 "further_extraction": (
                     source,
                     {"headers": {"referer": NINEANIME}},
                 ),
                 "title": f"Episode {data_source.get('data-num')}, {content_type_container.get('data-type').upper()}",
             }
 
 
 def fetcher(session, url, check, match):
-
     content_id = CONTENT_ID_REGEX.search(session.get(url).text).group(1)
 
     for data_source in htmlparser.fromstring(
         session.get(
             NINEANIME + f"ajax/episode/list/{content_id}",
+            params={"vrf": vrf_api(session, content_id)},
         ).json()["result"]
     ).cssselect("a[data-num]"):
-        yield partial(
-            lambda data_source: list(fetch_episode(session, data_source)),
-            data_source,
-        ), data_source.get("data-num")
+        episode_string: str = data_source.get("data-num")
 
+        episode = int(episode_string) if episode_string.isdigit() else 0
 
-def metadata_fetcher(session, url, match):
+        if check(episode):
+            yield partial(
+                lambda data_source: list(fetch_episode(session, data_source)),
+                data_source,
+            ), episode
 
+
+def metadata_fetcher(session, url, match):
     response = session.get(url).text
 
     return {"titles": TITLES_REGEX.findall(response)}
```

### Comparing `ap0dl-1.5.2/ap0dl/core/codebase/providers/tenshimoe/__init__.py` & `ap0dl-1.6.0/ap0dl/core/codebase/providers/marinmoe/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,67 +1,94 @@
-from functools import partial
+import functools
 
-import lxml.html as htmlparser
-import regex
+from ap0dl.utils import optopt
+from ap0dl.utils.powertools import ctx
 
-from ....config import TENSHI
-from ...helpers import construct_site_based_regex, uwu
+from ....config import MARIN
+from ...helpers import construct_site_based_regex
 
-REGEX = construct_site_based_regex(TENSHI, extra_regex=r"/anime/([^?&/]+)")
-TITLES_REGEX = regex.compile(r'<h1 class="mb-3">(.+?)</h1>')
+REGEX = construct_site_based_regex(MARIN, extra_regex=r"/anime/([^?&/]+)")
 
 
-def post_processor(session, stream_page):
-    cookies = "__ddg1={}; __ddg2={}; __ddg2_={}".format(
-        session.cookies.get("__ddg1_", ""),
-        session.cookies.get("__ddg2", ""),
-        session.cookies.get("__ddg2_", ""),
-    )
-    yield from (
-        {
-            "quality": int(_.group(2)),
-            "stream_url": _.group(1),
-            "headers": {"cookie": cookies},
+class HashableDict(dict):
+    def __hash__(self):
+        return hash(tuple(sorted(self.items())))
+
+
+def get_inertia_version(session):
+
+    if "marin_inertia_version" in ctx:
+        return ctx["marin_inertia_version"]
+
+    response = session.get(MARIN)
+
+    intertia_version = optopt.regexlib.search(
+        r"version&quot;:&quot;(.+?)&quot;", response.text
+    ).group(1)
+
+    ctx.update(marin_inertia_version=intertia_version)
+
+    return intertia_version
+
+
+def iter_episode_streams(session, url):
+
+    episodes_data = session.get(
+        url,
+        headers={
+            "x-inertia": "true",
+            "x-inertia-version": get_inertia_version(session),
+        },
+    ).json()
+
+    props = episodes_data.get("props", {})
+
+    for episode in props.get("video", {}).get("data", {}).get("mirror", []):
+        code = episode.get("code", {})
+
+        yield {
+            "stream_url": code.get("file"),
+            "quality": code.get("width"),
+            "title": " // ".join(
+                _["text"]
+                for _ in props.get("episode", {}).get("data", {}).get("title")[:2]
+            ),
         }
-        for _ in regex.finditer(
-            r'<source src="(.+?)" .+? size="([0-9]+)">', stream_page, flags=regex.S
-        )
-    )
 
 
-def extract_urls(session, episode_page, *, post_processor):
-    episode_page_content = session.get(episode_page)
-    embed_page = (
-        htmlparser.fromstring(episode_page_content.text).cssselect("iframe") or [{}]
-    )[0].get("src")
-    yield from post_processor(
-        session, session.get(embed_page, headers={"referer": episode_page}).text
+@functools.lru_cache()
+def fetch_anime_data(session, url):
+    return HashableDict(
+        session.get(
+            url,
+            headers={
+                "x-inertia": "true",
+                "x-inertia-version": get_inertia_version(session),
+            },
+        ).json()
     )
 
 
-def fetcher(
-    session, url, check, match, *, post_processor=post_processor, domain=TENSHI
-):
-    uwu.bypass_ddos_guard(session, domain)
+def fetcher(session, url, check, match):
     url = match.group(0)
 
-    episode_list_page = session.get(url)
-    count = int(
-        htmlparser.fromstring(episode_list_page.text)
-        .cssselect("span.badge")[0]
-        .text_content()
-    )
+    anime_data = fetch_anime_data(session, url)
+
+    count = int(anime_data.get("props", {}).get("anime", {}).get("last_episode", 0))
 
     for episode in range(1, count + 1):
         if check(episode):
-            yield partial(
-                lambda c: [*extract_urls(session, c, post_processor=post_processor)],
-                "{}/{:d}".format(url, episode),
+            yield functools.partial(
+                lambda url: list(iter_episode_streams(session, url)),
+                f"{url}/{episode}",
             ), episode
 
 
-def metadata_fetcher(session, url, match, *, domain=TENSHI):
+def metadata_fetcher(session, url, match):
 
-    uwu.bypass_ddos_guard(session, domain)
     url = match.group(0)
 
-    return {"titles": TITLES_REGEX.findall(session.get(url).text)}
+    anime_data = fetch_anime_data(session, url)
+
+    return {
+        "titles": [anime_data.get("props", {}).get("anime", {}).get("title")],
+    }
```

### Comparing `ap0dl-1.5.2/ap0dl/core/codebase/providers/twistmoe/__init__.py` & `ap0dl-1.6.0/ap0dl/core/codebase/providers/twistmoe/__init__.py`

 * *Files identical despite different names*

### Comparing `ap0dl-1.5.2/ap0dl/core/codebase/providers/twistmoe/stream_url.py` & `ap0dl-1.6.0/ap0dl/core/codebase/providers/twistmoe/stream_url.py`

 * *Files identical despite different names*

### Comparing `ap0dl-1.5.2/ap0dl/core/codebase/providers/zoro/__init__.py` & `ap0dl-1.6.0/ap0dl/core/codebase/providers/zoro/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,16 +2,20 @@
 
 import lxml.html as htmlparser
 import regex
 
 from ....config import ZORO
 from ...helpers import construct_site_based_regex
 
-REGEX = construct_site_based_regex(ZORO, extra_regex=r"(/watch)?/[\w-]+-(\d+)")
-TITLES_REGEX = regex.compile(r'<h2 class="film-name dynamic-name" .+?>(.+?)</h2>')
+REGEX = construct_site_based_regex(
+    ZORO, extra_regex=r"(/watch)?/(?P<slug>[\w-]+-(?P<id>\d+))"
+)
+TITLES_REGEX = regex.compile(
+    r'<h2 class="film-name dynamic-name".+?>(.+?)</h2>', flags=regex.DOTALL
+)
 
 XHR_HEADERS = {
     "X-Requested-With": "XMLHttpRequest",
     "Referer": ZORO,
 }
 
 
@@ -58,15 +62,15 @@
                 {"headers": {"Referer": ZORO}},
             ),
             "title": "{} - {}".format(server.get("data-type", "").upper(), title),
         }
 
 
 def fetcher(session, url, check, match):
-    slug = match.group(2)
+    slug = match.group("id")
 
     for episode in htmlparser.fromstring(
         session.get(ZORO + f"ajax/v2/episode/list/{slug}", headers=XHR_HEADERS)
         .json()
         .get("html")
     ).cssselect("a[title][data-number][data-id]"):
         episode_number = int_or(episode.get("data-number", "") or "")
@@ -75,8 +79,10 @@
                 lambda d_id, t: list(extract_episode(session, d_id, t)),
                 d_id=episode.get("data-id"),
                 t=episode.get("title"),
             ), episode_number
 
 
 def metadata_fetcher(session, url, match):
-    return {"titles": TITLES_REGEX.findall(session.get(ZORO + match.group(2)).text)}
+    return {
+        "titles": TITLES_REGEX.findall(session.get(ZORO + match.group("slug")).text)
+    }
```

### Comparing `ap0dl-1.5.2/ap0dl/core/config/__init__.py` & `ap0dl-1.6.0/ap0dl/core/config/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,61 +21,61 @@
         if not isinstance(_, Path):
             _ = Path(_)
         if _.exists():
             return _
 
 
 if sys.platform == "win32":
-    USERPROFILE_AP0DL_PATH = (
+    USERPROFILE_ap0dl_PATH = (
         Path(os.getenv("LOCALAPPDATA", ".")) / ".config" / "ap0dl" / "config.yml"
     )
     OLD_DEPRECATED_PATH = Path(os.getenv("USERPROFILE")) / ".ap0dl" / "config.yml"
 
     if OLD_DEPRECATED_PATH.exists():
-        if not USERPROFILE_AP0DL_PATH.exists():
+        if not USERPROFILE_ap0dl_PATH.exists():
             warnings.warn(
                 f"The config file path @ {OLD_DEPRECATED_PATH.as_posix()} is deprecated and will be removed in the future. "
-                f"Please migrate to {USERPROFILE_AP0DL_PATH.as_posix()}. "
+                f"Please migrate to {USERPROFILE_ap0dl_PATH.as_posix()}. "
                 f"This is not done automatically because this project does not want to mess with your files.",
             )
-            USERPROFILE_AP0DLPATH = OLD_DEPRECATED_PATH
+            USERPROFILE_ap0dl_PATH = OLD_DEPRECATED_PATH
 
 else:
-    USERPROFILE_AP0DL_PATH = (
+    USERPROFILE_ap0dl_PATH = (
         Path(os.getenv("HOME", ".")) / ".config" / "ap0dl" / "config.yml"
     )
 
 CONFIGURATION_FILE_PATH = get_existent_path(
-    os.getenv("AP0DL_CONFIG", "./ap0dl_config.yml"),
+    os.getenv("ap0dl_CONFIG", "./ap0dl_config.yml"),
     "/ap0dl_config.yml",
-    USERPROFILE_AP0DL_PATH,
+    USERPROFILE_ap0dl_PATH,
 )
 
 DEFAULT_CONFIG = {
     "default_provider": "allanime",
     "site_urls": {
-        "9anime": "https://9anime.pl/",
-        "allanime": "https://allanime.site/",
+        "9anime": "https://aniwave.to/",
+        "allanime": "https://allanime.to/",
         "animekaizoku": "https://animekaizoku.com/",
-        "animeout": "https://animeout.xyz/",
-        "animepahe": "https://animepahe.com/",
+        "animeout": "https://www.animeout.xyz/",
+        "animepahe": "https://animepahe.ru/",
         "animeonsen": "https://animeonsen.xyz/",
         "animexin": "https://animexin.xyz/",
         "animixplay": "https://animixplay.to/",
         "animtime": "https://animtime.com/",
         "crunchyroll": "http://www.crunchyroll.com/",
         "kawaiifu": "https://kawaiifu.com/",
-        "gogoanime": "https://gogoanime.cm/",
+        "gogoanime": "https://gogoanime.bid/",
         "haho": "https://haho.moe/",
         "hentaistream": "https://hstream.moe/",
         "kamyroll_api": "https://kamyroll.herokuapp.com/",
-        "tenshi": "https://tenshi.moe/",
-        "nyaasi": "https://nyaa.si/",
+        "marin": "https://marin.moe/",
         "twist": "https://twist.moe/",
-        "zoro": "https://zoro.to/",
+        "yugen": "https://yugenanime.ro/",
+        "zoro": "https://aniwatch.to/",
     },
     "quality_string": "best[subtitle]/best",
     "default_player": "mpv",
     "players": {
         "mpv": {
             "executable": "mpv",
             "opts": [],
@@ -105,24 +105,25 @@
         "site_url": "https://graphql.anilist.co/",
         "date_format": "%b. %d, %A",
         "time_format": "%X",
     },
     "download_auto_retry": 300,
     "ffmpeg": {
         "executable": "ffmpeg",
-        "hls_download": False,
+        "use_for_downloads": False,
         "submerge": True,
     },
     "discord_presence": False,
     "fzf": {
         "executable": "fzf",
         "opts": [],
         "state": False,
     },
     "download_directory": ".",
+    "threaded_download": False,
     "check_for_updates": True,
     "force_streaming_quality_selection": True,
     "aniskip": False,
     "superanime": {
         "return_all": False,
         "type_of": "sub",
         "crunchyroll": {"subtitle_language": "en-US"},
@@ -146,19 +147,19 @@
 ANIMEXIN = SITE_URLS.get("animexin")
 ANIMIXPLAY = SITE_URLS.get("animixplay")
 ANIMTIME = SITE_URLS.get("animtime")
 CRUNCHYROLL = SITE_URLS.get("crunchyroll")
 KAWAIIFU = SITE_URLS.get("kawaiifu")
 KAMYROLL_API = SITE_URLS.get("kamyroll_api")
 GOGOANIME = SITE_URLS.get("gogoanime")
-NYAASI = SITE_URLS.get("nyaasi")
-TENSHI = SITE_URLS.get("tenshi")
+MARIN = SITE_URLS.get("marin")
 HAHO = SITE_URLS.get("haho")
 HENTAISTREAM = SITE_URLS.get("hentaistream")
 TWIST = SITE_URLS.get("twist")
+YUGEN = SITE_URLS.get("yugen")
 ZORO = SITE_URLS.get("zoro")
 
 QUALITY = CONFIG.get("quality_string")
 
 DEFAULT_PLAYER = CONFIG.get("default_player")
 PLAYERS = CONFIG.get("players")
 
@@ -170,25 +171,27 @@
 DEFAULT_PROVIDER = CONFIG.get("default_provider")
 
 AUTO_RETRY = CONFIG.get("download_auto_retry", 300) / 1000
 
 FFMPEG_SETTINGS = CONFIG.get("ffmpeg", {})
 
 FFMPEG_EXECUTABLE = FFMPEG_SETTINGS.get("executable", "ffmpeg")
-FFMPEG_HLS = FFMPEG_SETTINGS.get("hls_download", False)
+FFMPEG_USE_FOR_DOWNLOADS = FFMPEG_SETTINGS.get("use_for_downloads", False)
 FFMPEG_SUBMERGE = FFMPEG_SETTINGS.get("submerge", True)
 
 DISCORD_PRESENCE = CONFIG.get("discord_presence", False)
 
 FZF = CONFIG.get("fzf", {})
 FZF_EXECUTABLE = FZF.get("executable", "fzf")
 FZF_OPTS = FZF.get("opts", [])
 FZF_STATE = FZF.get("state", False)
 
 DOWNLOAD_DIRECTORY = CONFIG.get("download_directory", ".")
+THREADED_DOWNLOAD = CONFIG.get("threaded_download", False)
+
 CHECK_FOR_UPDATES = CONFIG.get("check_for_updates", True)
 FORCE_STREAMING_QUALITY_SELECTION = CONFIG.get(
     "force_streaming_quality_selection", True
 )
 
 USE_ANISKIP = CONFIG.get("aniskip", False)
```

### Comparing `ap0dl-1.5.2/ap0dl/core/package_resolver.py` & `ap0dl-1.6.0/ap0dl/core/package_resolver.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,14 @@
 
 
 def match_version(version_expression: str, version_string: str) -> bool:
     if version_expression is None:
         return True
 
     def single_matcher(single_expression: str):
-
         target_version = single_expression.lstrip("=<>~")
         expr = single_expression[: -len(target_version)]
 
         target = version.parse(target_version)
         current = version.parse(version_string)
 
         operators = {
@@ -73,15 +72,14 @@
         "https://www.lfd.uci.edu/~gohlke/pythonlibs/", follow_redirects=True
     ).text
 
 
 def iter_packages(
     session, package_name, version_expression: str = None, pc_arch: str = PC_ARCH
 ):
-
     WHEELS_REGEX = re.compile(rf"]'>({package_name}.+?{pc_arch}&#46;whl)<")
 
     for _ in WHEELS_REGEX.finditer(get_packages_page(session)):
         package = STRING_REGEX.sub(lambda match: chr(int(match.group(1))), _.group(1))
 
         _, package_version, *abis, _ = package.split("‑")
 
@@ -97,15 +95,14 @@
     import httpx
 
     pip_install_args = [sys.executable, "-m", "pip", "install"]
 
     session = httpx.Client()
 
     for package, version_expr in packages:
-
         pkg = pkginfo.get_metadata(package)
 
         if pkg is not None and match_version(version_expr, pkg.version):
             continue
 
         pip_pkg_string = package + (version_expr if version_expr else "")
```

### Comparing `ap0dl-1.5.2/LICENSE` & `ap0dl-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ap0dl-1.5.2/pyproject.toml` & `ap0dl-1.6.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,33 +1,37 @@
 [build-system]
 requires = [ "poetry-core>=1.0.0",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "ap0dl"
-version = "1.5.2"
+version = "1.6.0"
 description = "Efficient, fast, powerful and light-weight anime multi-purpose tool"
 readme = "readme.txt"
-authors = [ "rares9301 <rares.sarmasag@cnmbct.ro>",]
+authors = [ "rares9301 <rares.sarmasag@stud.acs.upb.ro>",]
 license = "GPT-3"
 
 [tool.poetry.dependencies]
 python = ">=3.7,<4.0"
 anchor-kr = "~=0.1.3"
 anitopy = "~=2.1.0"
-click = "~=8.0.4"
+click = ">=8.0.4,<8.2.0"
 comtypes = "~=1.1.11"
-cssselect = "~=1.1.0"
+cssselect = ">=1.1,<1.3"
 httpx = "~=0.23.0"
-tqdm = "~=4.62.3"
+tqdm = ">=4.62.3,<4.66.0"
 pycryptodomex = "~=3.14.1"
 regex = "~=2022.10.31"
 yarl = "~=1.8.1"
 pyyaml = "~=6.0"
-packaging = "^22.0"
+packaging = ">=22,<24"
 pkginfo = "^1.9.2"
-rich = "^13.0.0"
+rich = ">=13.3.1,<13.3.4"
 
 [tool.poetry.dev-dependencies]
 
 [tool.poetry.scripts]
 ap0dl = "ap0dl.__main__:__ap0dl_cli__"
+
+[tool.poetry.dependencies.lxml]
+version = "4.9.1"
+markers = "sys_platform != 'win32'"
```

### Comparing `ap0dl-1.5.2/PKG-INFO` & `ap0dl-1.6.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 Metadata-Version: 2.1
 Name: ap0dl
-Version: 1.5.2
+Version: 1.6.0
 Summary: Efficient, fast, powerful and light-weight anime multi-purpose tool
 License: GPT-3
 Author: rares9301
-Author-email: rares.sarmasag@cnmbct.ro
+Author-email: rares.sarmasag@stud.acs.upb.ro
 Requires-Python: >=3.7,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: anchor-kr (>=0.1.3,<0.2.0)
 Requires-Dist: anitopy (>=2.1.0,<2.2.0)
-Requires-Dist: click (>=8.0.4,<8.1.0)
+Requires-Dist: click (>=8.0.4,<8.2.0)
 Requires-Dist: comtypes (>=1.1.11,<1.2.0)
-Requires-Dist: cssselect (>=1.1.0,<1.2.0)
+Requires-Dist: cssselect (>=1.1,<1.3)
 Requires-Dist: httpx (>=0.23.0,<0.24.0)
-Requires-Dist: packaging (>=22.0,<23.0)
+Requires-Dist: lxml (==4.9.1) ; sys_platform != "win32"
+Requires-Dist: packaging (>=22,<24)
 Requires-Dist: pkginfo (>=1.9.2,<2.0.0)
 Requires-Dist: pycryptodomex (>=3.14.1,<3.15.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: regex (>=2022.10.31,<2022.11.0)
-Requires-Dist: rich (>=13.0.0,<14.0.0)
-Requires-Dist: tqdm (>=4.62.3,<4.63.0)
+Requires-Dist: rich (>=13.3.1,<13.3.4)
+Requires-Dist: tqdm (>=4.62.3,<4.66.0)
 Requires-Dist: yarl (>=1.8.1,<1.9.0)
 Description-Content-Type: text/plain
```

