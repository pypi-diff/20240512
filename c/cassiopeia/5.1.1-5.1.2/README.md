# Comparing `tmp/cassiopeia-5.1.1.tar.gz` & `tmp/cassiopeia-5.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cassiopeia-5.1.1.tar", last modified: Sun May  5 15:20:01 2024, max compression
+gzip compressed data, was "cassiopeia-5.1.2.tar", last modified: Sun May 12 02:26:11 2024, max compression
```

## Comparing `cassiopeia-5.1.1.tar` & `cassiopeia-5.1.2.tar`

### file list

```diff
@@ -1,133 +1,133 @@
-drwxrwxrwx   0        0        0        0 2024-05-05 15:20:01.212440 cassiopeia-5.1.1/
--rw-rw-rw-   0        0        0     1113 2023-02-12 18:12:02.000000 cassiopeia-5.1.1/LICENSE.txt
--rw-rw-rw-   0        0        0      268 2023-02-12 18:12:02.000000 cassiopeia-5.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0      858 2024-05-05 15:20:01.212440 cassiopeia-5.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     5799 2024-05-05 03:37:59.000000 cassiopeia-5.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-05 15:20:01.034539 cassiopeia-5.1.1/cassiopeia/
--rw-rw-rw-   0        0        0     1830 2024-05-05 14:50:16.000000 cassiopeia-5.1.1/cassiopeia/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-05 15:20:01.062246 cassiopeia-5.1.1/cassiopeia/_configuration/
--rw-rw-rw-   0        0        0     1260 2023-02-12 18:12:02.000000 cassiopeia-5.1.1/cassiopeia/_configuration/__init__.py
--rw-rw-rw-   0        0        0      378 2024-05-05 06:18:57.000000 cassiopeia-5.1.1/cassiopeia/_configuration/all_plugins.json
--rw-rw-rw-   0        0        0      679 2023-02-12 18:12:02.000000 cassiopeia-5.1.1/cassiopeia/_configuration/load.py
--rw-rw-rw-   0        0        0     7929 2024-05-05 03:37:59.000000 cassiopeia-5.1.1/cassiopeia/_configuration/settings.py
--rw-rw-rw-   0        0        0     6592 2024-05-05 14:49:28.000000 cassiopeia-5.1.1/cassiopeia/cassiopeia.py
-drwxrwxrwx   0        0        0        0 2024-05-05 15:20:01.102372 cassiopeia-5.1.1/cassiopeia/core/
--rw-rw-rw-   0        0        0      743 2024-05-05 06:21:33.000000 cassiopeia-5.1.1/cassiopeia/core/__init__.py
--rw-rw-rw-   0        0        0     5156 2024-05-05 14:53:17.000000 cassiopeia-5.1.1/cassiopeia/core/account.py
--rw-rw-rw-   0        0        0     1819 2023-02-12 18:12:02.000000 cassiopeia-5.1.1/cassiopeia/core/champion.py
--rw-rw-rw-   0        0        0     9656 2024-05-05 03:37:59.000000 cassiopeia-5.1.1/cassiopeia/core/championmastery.py
--rw-rw-rw-   0        0        0    13675 2023-02-12 18:12:02.000000 cassiopeia-5.1.1/cassiopeia/core/common.py
--rw-rw-rw-   0        0        0    20498 2024-05-05 03:37:59.000000 cassiopeia-5.1.1/cassiopeia/core/league.py
--rw-rw-rw-   0        0        0    73137 2024-05-05 03:37:59.000000 cassiopeia-5.1.1/cassiopeia/core/match.py
--rw-rw-rw-   0        0        0     5384 2024-05-05 03:37:59.000000 cassiopeia-5.1.1/cassiopeia/core/patch.py
--rw-rw-rw-   0        0        0    11495 2024-05-05 15:10:07.000000 cassiopeia-5.1.1/cassiopeia/core/spectator.py
-drwxrwxrwx   0        0        0        0 2024-05-05 15:20:01.119930 cassiopeia-5.1.1/cassiopeia/core/staticdata/
--rw-rw-rw-   0        0        0      392 2023-02-12 18:12:02.000000 cassiopeia-5.1.1/cassiopeia/core/staticdata/__init__.py
--rw-rw-rw-   0        0        0    30430 2023-02-12 18:12:02.000000 cassiopeia-5.1.1/cassiopeia/core/staticdata/champion.py
--rw-rw-rw-   0        0        0     2497 2023-02-12 18:12:02.000000 cassiopeia-5.1.1/cassiopeia/core/staticdata/common.py
--rw-rw-rw-   0        0        0    17615 2023-02-12 18:12:02.000000 cassiopeia-5.1.1/cassiopeia/core/staticdata/item.py
--rw-rw-rw-   0        0        0      734 2023-02-12 18:12:02.000000 cassiopeia-5.1.1/cassiopeia/core/staticdata/language.py
--rw-rw-rw-   0        0        0     2343 2023-02-12 18:12:02.000000 cassiopeia-5.1.1/cassiopeia/core/staticdata/languagestrings.py
--rw-rw-rw-   0        0        0     5877 2023-02-12 18:12:02.000000 cassiopeia-5.1.1/cassiopeia/core/staticdata/map.py
--rw-rw-rw-   0        0        0     6330 2023-02-12 18:12:02.000000 cassiopeia-5.1.1/cassiopeia/core/staticdata/profileicon.py
--rw-rw-rw-   0        0        0     3040 2023-02-12 18:12:02.000000 cassiopeia-5.1.1/cassiopeia/core/staticdata/realm.py
--rw-rw-rw-   0        0        0    10691 2024-05-05 03:37:59.000000 cassiopeia-5.1.1/cassiopeia/core/staticdata/rune.py
--rw-rw-rw-   0        0        0    12152 2023-02-12 18:12:02.000000 cassiopeia-5.1.1/cassiopeia/core/staticdata/summonerspell.py
--rw-rw-rw-   0        0        0      776 2023-02-12 18:12:02.000000 cassiopeia-5.1.1/cassiopeia/core/staticdata/version.py
--rw-rw-rw-   0        0        0     5634 2023-02-12 18:12:02.000000 cassiopeia-5.1.1/cassiopeia/core/status.py
--rw-rw-rw-   0        0        0     6833 2024-05-05 15:06:50.000000 cassiopeia-5.1.1/cassiopeia/core/summoner.py
--rw-rw-rw-   0        0        0    28741 2024-05-05 03:37:59.000000 cassiopeia-5.1.1/cassiopeia/data.py
-drwxrwxrwx   0        0        0        0 2024-05-05 15:20:01.126633 cassiopeia-5.1.1/cassiopeia/datastores/
--rw-rw-rw-   0        0        0      237 2023-02-12 18:12:02.000000 cassiopeia-5.1.1/cassiopeia/datastores/__init__.py
--rw-rw-rw-   0        0        0    56546 2024-05-05 03:37:59.000000 cassiopeia-5.1.1/cassiopeia/datastores/cache.py
--rw-rw-rw-   0        0        0     9819 2023-02-12 18:12:02.000000 cassiopeia-5.1.1/cassiopeia/datastores/common.py
--rw-rw-rw-   0        0        0    31133 2024-05-05 03:37:59.000000 cassiopeia-5.1.1/cassiopeia/datastores/ddragon.py
--rw-rw-rw-   0        0        0    31148 2024-05-05 14:59:41.000000 cassiopeia-5.1.1/cassiopeia/datastores/ghost.py
--rw-rw-rw-   0        0        0     2145 2023-02-12 18:12:02.000000 cassiopeia-5.1.1/cassiopeia/datastores/image.py
-drwxrwxrwx   0        0        0        0 2024-05-05 15:20:01.141162 cassiopeia-5.1.1/cassiopeia/datastores/kernel/
--rw-rw-rw-   0        0        0     1912 2024-05-05 06:23:06.000000 cassiopeia-5.1.1/cassiopeia/datastores/kernel/__init__.py
--rw-rw-rw-   0        0        0     2057 2024-05-05 03:37:59.000000 cassiopeia-5.1.1/cassiopeia/datastores/kernel/account.py
--rw-rw-rw-   0        0        0     2400 2023-02-12 18:12:02.000000 cassiopeia-5.1.1/cassiopeia/datastores/kernel/champion.py
--rw-rw-rw-   0        0        0     8555 2023-02-12 18:12:02.000000 cassiopeia-5.1.1/cassiopeia/datastores/kernel/championmastery.py
--rw-rw-rw-   0        0        0     4637 2023-02-12 18:12:02.000000 cassiopeia-5.1.1/cassiopeia/datastores/kernel/common.py
--rw-rw-rw-   0        0        0    11466 2023-02-12 18:12:02.000000 cassiopeia-5.1.1/cassiopeia/datastores/kernel/leagues.py
--rw-rw-rw-   0        0        0    12070 2023-02-12 18:12:02.000000 cassiopeia-5.1.1/cassiopeia/datastores/kernel/match.py
--rw-rw-rw-   0        0        0     3216 2024-05-05 15:01:18.000000 cassiopeia-5.1.1/cassiopeia/datastores/kernel/spectator.py
--rw-rw-rw-   0        0        0     3038 2024-04-10 05:17:47.000000 cassiopeia-5.1.1/cassiopeia/datastores/kernel/status.py
--rw-rw-rw-   0        0        0     2189 2024-05-05 03:37:59.000000 cassiopeia-5.1.1/cassiopeia/datastores/kernel/summoner.py
--rw-rw-rw-   0        0        0     4033 2024-04-10 05:26:46.000000 cassiopeia-5.1.1/cassiopeia/datastores/lolwikia.py
--rw-rw-rw-   0        0        0     2897 2023-02-12 18:12:02.000000 cassiopeia-5.1.1/cassiopeia/datastores/merakianalyticscdn.py
-drwxrwxrwx   0        0        0        0 2024-05-05 15:20:01.157551 cassiopeia-5.1.1/cassiopeia/datastores/riotapi/
--rw-rw-rw-   0        0        0     3565 2024-05-05 06:23:17.000000 cassiopeia-5.1.1/cassiopeia/datastores/riotapi/__init__.py
--rw-rw-rw-   0        0        0     2697 2024-05-05 03:37:59.000000 cassiopeia-5.1.1/cassiopeia/datastores/riotapi/account.py
--rw-rw-rw-   0        0        0     2643 2023-02-12 18:12:02.000000 cassiopeia-5.1.1/cassiopeia/datastores/riotapi/champion.py
--rw-rw-rw-   0        0        0    10255 2024-04-10 05:17:47.000000 cassiopeia-5.1.1/cassiopeia/datastores/riotapi/championmastery.py
--rw-rw-rw-   0        0        0    17773 2023-02-12 18:12:02.000000 cassiopeia-5.1.1/cassiopeia/datastores/riotapi/common.py
--rw-rw-rw-   0        0        0    15725 2023-02-12 18:12:02.000000 cassiopeia-5.1.1/cassiopeia/datastores/riotapi/leagues.py
--rw-rw-rw-   0        0        0     8276 2023-02-12 18:12:02.000000 cassiopeia-5.1.1/cassiopeia/datastores/riotapi/match.py
--rw-rw-rw-   0        0        0     3628 2024-05-05 15:04:20.000000 cassiopeia-5.1.1/cassiopeia/datastores/riotapi/spectator.py
--rw-rw-rw-   0        0        0     3530 2024-04-10 05:17:47.000000 cassiopeia-5.1.1/cassiopeia/datastores/riotapi/status.py
--rw-rw-rw-   0        0        0     2742 2024-05-05 03:37:59.000000 cassiopeia-5.1.1/cassiopeia/datastores/riotapi/summoner.py
--rw-rw-rw-   0        0        0    91633 2024-05-05 15:00:09.000000 cassiopeia-5.1.1/cassiopeia/datastores/uniquekeys.py
-drwxrwxrwx   0        0        0        0 2024-05-05 15:20:01.173065 cassiopeia-5.1.1/cassiopeia/dto/
--rw-rw-rw-   0        0        0        0 2023-02-12 18:12:02.000000 cassiopeia-5.1.1/cassiopeia/dto/__init__.py
--rw-rw-rw-   0        0        0       75 2024-05-05 03:37:59.000000 cassiopeia-5.1.1/cassiopeia/dto/account.py
--rw-rw-rw-   0        0        0       84 2023-02-12 18:12:02.000000 cassiopeia-5.1.1/cassiopeia/dto/champion.py
--rw-rw-rw-   0        0        0      196 2023-02-12 18:12:02.000000 cassiopeia-5.1.1/cassiopeia/dto/championmastery.py
--rw-rw-rw-   0        0        0      407 2023-02-12 18:12:02.000000 cassiopeia-5.1.1/cassiopeia/dto/common.py
--rw-rw-rw-   0        0        0      445 2023-02-12 18:12:02.000000 cassiopeia-5.1.1/cassiopeia/dto/league.py
--rw-rw-rw-   0        0        0      215 2023-02-12 18:12:02.000000 cassiopeia-5.1.1/cassiopeia/dto/match.py
--rw-rw-rw-   0        0        0       77 2023-02-12 18:12:02.000000 cassiopeia-5.1.1/cassiopeia/dto/patch.py
--rw-rw-rw-   0        0        0      133 2023-02-12 18:12:02.000000 cassiopeia-5.1.1/cassiopeia/dto/spectator.py
-drwxrwxrwx   0        0        0        0 2024-05-05 15:20:01.185887 cassiopeia-5.1.1/cassiopeia/dto/staticdata/
--rw-rw-rw-   0        0        0      516 2023-02-12 18:12:02.000000 cassiopeia-5.1.1/cassiopeia/dto/staticdata/__init__.py
--rw-rw-rw-   0        0        0      334 2023-02-12 18:12:02.000000 cassiopeia-5.1.1/cassiopeia/dto/staticdata/champion.py
--rw-rw-rw-   0        0        0        0 2023-02-12 18:12:02.000000 cassiopeia-5.1.1/cassiopeia/dto/staticdata/common.py
--rw-rw-rw-   0        0        0      118 2023-02-12 18:12:02.000000 cassiopeia-5.1.1/cassiopeia/dto/staticdata/item.py
--rw-rw-rw-   0        0        0      130 2023-02-12 18:12:02.000000 cassiopeia-5.1.1/cassiopeia/dto/staticdata/language.py
--rw-rw-rw-   0        0        0      116 2023-02-12 18:12:02.000000 cassiopeia-5.1.1/cassiopeia/dto/staticdata/map.py
--rw-rw-rw-   0        0        0      139 2023-02-12 18:12:02.000000 cassiopeia-5.1.1/cassiopeia/dto/staticdata/profileicon.py
--rw-rw-rw-   0        0        0       74 2023-02-12 18:12:02.000000 cassiopeia-5.1.1/cassiopeia/dto/staticdata/realm.py
--rw-rw-rw-   0        0        0      209 2023-02-12 18:12:02.000000 cassiopeia-5.1.1/cassiopeia/dto/staticdata/rune.py
--rw-rw-rw-   0        0        0      136 2023-02-12 18:12:02.000000 cassiopeia-5.1.1/cassiopeia/dto/staticdata/summonerspell.py
--rw-rw-rw-   0        0        0       80 2023-02-12 18:12:02.000000 cassiopeia-5.1.1/cassiopeia/dto/staticdata/version.py
--rw-rw-rw-   0        0        0       79 2023-02-12 18:12:02.000000 cassiopeia-5.1.1/cassiopeia/dto/status.py
--rw-rw-rw-   0        0        0       76 2023-02-12 18:12:02.000000 cassiopeia-5.1.1/cassiopeia/dto/summoner.py
--rw-rw-rw-   0        0        0    26420 2023-02-12 18:12:02.000000 cassiopeia-5.1.1/cassiopeia/profile_icon_names.json
-drwxrwxrwx   0        0        0        0 2024-05-05 15:20:01.185887 cassiopeia-5.1.1/cassiopeia/resources/
--rw-rw-rw-   0        0        0    15654 2023-02-12 18:12:02.000000 cassiopeia-5.1.1/cassiopeia/resources/summonersRiftAreas.png
-drwxrwxrwx   0        0        0        0 2024-05-05 15:20:01.188921 cassiopeia-5.1.1/cassiopeia/transformers/
--rw-rw-rw-   0        0        0      850 2024-05-05 06:23:23.000000 cassiopeia-5.1.1/cassiopeia/transformers/__init__.py
--rw-rw-rw-   0        0        0      888 2024-05-05 03:37:59.000000 cassiopeia-5.1.1/cassiopeia/transformers/account.py
--rw-rw-rw-   0        0        0     1091 2023-02-12 18:12:02.000000 cassiopeia-5.1.1/cassiopeia/transformers/champion.py
--rw-rw-rw-   0        0        0     2203 2023-02-12 18:12:02.000000 cassiopeia-5.1.1/cassiopeia/transformers/championmastery.py
--rw-rw-rw-   0        0        0     5348 2023-02-12 18:12:02.000000 cassiopeia-5.1.1/cassiopeia/transformers/leagues.py
--rw-rw-rw-   0        0        0     2974 2023-02-12 18:12:02.000000 cassiopeia-5.1.1/cassiopeia/transformers/match.py
--rw-rw-rw-   0        0        0     2665 2024-05-05 14:48:17.000000 cassiopeia-5.1.1/cassiopeia/transformers/spectator.py
--rw-rw-rw-   0        0        0    15350 2023-02-12 18:12:02.000000 cassiopeia-5.1.1/cassiopeia/transformers/staticdata.py
--rw-rw-rw-   0        0        0      947 2023-02-12 18:12:02.000000 cassiopeia-5.1.1/cassiopeia/transformers/status.py
--rw-rw-rw-   0        0        0      906 2024-05-05 03:37:59.000000 cassiopeia-5.1.1/cassiopeia/transformers/summoner.py
-drwxrwxrwx   0        0        0        0 2024-05-05 15:20:01.062246 cassiopeia-5.1.1/cassiopeia.egg-info/
--rw-rw-rw-   0        0        0      858 2024-05-05 15:20:00.000000 cassiopeia-5.1.1/cassiopeia.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3823 2024-05-05 15:20:00.000000 cassiopeia-5.1.1/cassiopeia.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-05 15:20:00.000000 cassiopeia-5.1.1/cassiopeia.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       65 2024-05-05 15:20:00.000000 cassiopeia-5.1.1/cassiopeia.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-05-05 15:20:00.000000 cassiopeia-5.1.1/cassiopeia.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2024-04-10 05:29:30.000000 cassiopeia-5.1.1/cassiopeia.egg-info/zip-safe
--rw-rw-rw-   0        0        0      123 2024-05-05 15:20:01.251256 cassiopeia-5.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1537 2024-05-05 15:18:27.000000 cassiopeia-5.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-05 15:20:01.212440 cassiopeia-5.1.1/test/
--rw-rw-rw-   0        0        0        0 2023-02-12 18:12:02.000000 cassiopeia-5.1.1/test/__init__.py
--rw-rw-rw-   0        0        0      532 2023-02-12 18:12:02.000000 cassiopeia-5.1.1/test/constants.py
--rw-rw-rw-   0        0        0     1369 2023-02-12 18:12:02.000000 cassiopeia-5.1.1/test/test_champion.py
--rw-rw-rw-   0        0        0     2201 2023-02-12 18:12:02.000000 cassiopeia-5.1.1/test/test_championmastery.py
--rw-rw-rw-   0        0        0      278 2023-02-12 18:12:02.000000 cassiopeia-5.1.1/test/test_championrotation.py
--rw-rw-rw-   0        0        0     9322 2024-05-05 14:50:20.000000 cassiopeia-5.1.1/test/test_examples.py
--rw-rw-rw-   0        0        0      689 2023-02-12 18:12:02.000000 cassiopeia-5.1.1/test/test_items.py
--rw-rw-rw-   0        0        0     2473 2023-02-12 18:12:02.000000 cassiopeia-5.1.1/test/test_league.py
--rw-rw-rw-   0        0        0      734 2023-02-12 18:12:02.000000 cassiopeia-5.1.1/test/test_map_location.py
--rw-rw-rw-   0        0        0     1413 2023-02-12 18:12:02.000000 cassiopeia-5.1.1/test/test_match.py
--rw-rw-rw-   0        0        0     2329 2023-02-12 18:12:02.000000 cassiopeia-5.1.1/test/test_matchhistory.py
--rw-rw-rw-   0        0        0      708 2023-02-12 18:12:02.000000 cassiopeia-5.1.1/test/test_patches.py
--rw-rw-rw-   0        0        0      879 2023-02-12 18:12:02.000000 cassiopeia-5.1.1/test/test_status.py
--rw-rw-rw-   0        0        0     2023 2023-02-12 18:12:02.000000 cassiopeia-5.1.1/test/test_summoner.py
+drwxrwxrwx   0        0        0        0 2024-05-12 02:26:11.353215 cassiopeia-5.1.2/
+-rw-rw-rw-   0        0        0     1113 2023-02-12 18:12:02.000000 cassiopeia-5.1.2/LICENSE.txt
+-rw-rw-rw-   0        0        0      268 2023-02-12 18:12:02.000000 cassiopeia-5.1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      858 2024-05-12 02:26:11.353215 cassiopeia-5.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3954 2024-05-05 15:24:00.000000 cassiopeia-5.1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-12 02:26:10.040417 cassiopeia-5.1.2/cassiopeia/
+-rw-rw-rw-   0        0        0     1830 2024-05-05 14:50:16.000000 cassiopeia-5.1.2/cassiopeia/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-12 02:26:10.124624 cassiopeia-5.1.2/cassiopeia/_configuration/
+-rw-rw-rw-   0        0        0     1260 2023-02-12 18:12:02.000000 cassiopeia-5.1.2/cassiopeia/_configuration/__init__.py
+-rw-rw-rw-   0        0        0      378 2024-05-05 06:18:57.000000 cassiopeia-5.1.2/cassiopeia/_configuration/all_plugins.json
+-rw-rw-rw-   0        0        0      679 2023-02-12 18:12:02.000000 cassiopeia-5.1.2/cassiopeia/_configuration/load.py
+-rw-rw-rw-   0        0        0     7929 2024-05-05 03:37:59.000000 cassiopeia-5.1.2/cassiopeia/_configuration/settings.py
+-rw-rw-rw-   0        0        0     6592 2024-05-05 14:49:28.000000 cassiopeia-5.1.2/cassiopeia/cassiopeia.py
+drwxrwxrwx   0        0        0        0 2024-05-12 02:26:10.253418 cassiopeia-5.1.2/cassiopeia/core/
+-rw-rw-rw-   0        0        0      743 2024-05-05 06:21:33.000000 cassiopeia-5.1.2/cassiopeia/core/__init__.py
+-rw-rw-rw-   0        0        0     5156 2024-05-05 14:53:17.000000 cassiopeia-5.1.2/cassiopeia/core/account.py
+-rw-rw-rw-   0        0        0     1819 2023-02-12 18:12:02.000000 cassiopeia-5.1.2/cassiopeia/core/champion.py
+-rw-rw-rw-   0        0        0     9656 2024-05-05 03:37:59.000000 cassiopeia-5.1.2/cassiopeia/core/championmastery.py
+-rw-rw-rw-   0        0        0    13675 2023-02-12 18:12:02.000000 cassiopeia-5.1.2/cassiopeia/core/common.py
+-rw-rw-rw-   0        0        0    20498 2024-05-05 03:37:59.000000 cassiopeia-5.1.2/cassiopeia/core/league.py
+-rw-rw-rw-   0        0        0    73137 2024-05-05 03:37:59.000000 cassiopeia-5.1.2/cassiopeia/core/match.py
+-rw-rw-rw-   0        0        0     5384 2024-05-05 03:37:59.000000 cassiopeia-5.1.2/cassiopeia/core/patch.py
+-rw-rw-rw-   0        0        0    11495 2024-05-05 15:10:07.000000 cassiopeia-5.1.2/cassiopeia/core/spectator.py
+drwxrwxrwx   0        0        0        0 2024-05-12 02:26:10.439198 cassiopeia-5.1.2/cassiopeia/core/staticdata/
+-rw-rw-rw-   0        0        0      392 2023-02-12 18:12:02.000000 cassiopeia-5.1.2/cassiopeia/core/staticdata/__init__.py
+-rw-rw-rw-   0        0        0    30430 2023-02-12 18:12:02.000000 cassiopeia-5.1.2/cassiopeia/core/staticdata/champion.py
+-rw-rw-rw-   0        0        0     2497 2023-02-12 18:12:02.000000 cassiopeia-5.1.2/cassiopeia/core/staticdata/common.py
+-rw-rw-rw-   0        0        0    17615 2023-02-12 18:12:02.000000 cassiopeia-5.1.2/cassiopeia/core/staticdata/item.py
+-rw-rw-rw-   0        0        0      734 2023-02-12 18:12:02.000000 cassiopeia-5.1.2/cassiopeia/core/staticdata/language.py
+-rw-rw-rw-   0        0        0     2343 2023-02-12 18:12:02.000000 cassiopeia-5.1.2/cassiopeia/core/staticdata/languagestrings.py
+-rw-rw-rw-   0        0        0     5877 2023-02-12 18:12:02.000000 cassiopeia-5.1.2/cassiopeia/core/staticdata/map.py
+-rw-rw-rw-   0        0        0     6330 2023-02-12 18:12:02.000000 cassiopeia-5.1.2/cassiopeia/core/staticdata/profileicon.py
+-rw-rw-rw-   0        0        0     3040 2023-02-12 18:12:02.000000 cassiopeia-5.1.2/cassiopeia/core/staticdata/realm.py
+-rw-rw-rw-   0        0        0    10691 2024-05-05 03:37:59.000000 cassiopeia-5.1.2/cassiopeia/core/staticdata/rune.py
+-rw-rw-rw-   0        0        0    12152 2023-02-12 18:12:02.000000 cassiopeia-5.1.2/cassiopeia/core/staticdata/summonerspell.py
+-rw-rw-rw-   0        0        0      776 2023-02-12 18:12:02.000000 cassiopeia-5.1.2/cassiopeia/core/staticdata/version.py
+-rw-rw-rw-   0        0        0     5634 2023-02-12 18:12:02.000000 cassiopeia-5.1.2/cassiopeia/core/status.py
+-rw-rw-rw-   0        0        0     6833 2024-05-05 15:06:50.000000 cassiopeia-5.1.2/cassiopeia/core/summoner.py
+-rw-rw-rw-   0        0        0    28741 2024-05-05 03:37:59.000000 cassiopeia-5.1.2/cassiopeia/data.py
+drwxrwxrwx   0        0        0        0 2024-05-12 02:26:10.563360 cassiopeia-5.1.2/cassiopeia/datastores/
+-rw-rw-rw-   0        0        0      237 2023-02-12 18:12:02.000000 cassiopeia-5.1.2/cassiopeia/datastores/__init__.py
+-rw-rw-rw-   0        0        0    56546 2024-05-05 03:37:59.000000 cassiopeia-5.1.2/cassiopeia/datastores/cache.py
+-rw-rw-rw-   0        0        0     9819 2023-02-12 18:12:02.000000 cassiopeia-5.1.2/cassiopeia/datastores/common.py
+-rw-rw-rw-   0        0        0    31133 2024-05-05 03:37:59.000000 cassiopeia-5.1.2/cassiopeia/datastores/ddragon.py
+-rw-rw-rw-   0        0        0    31148 2024-05-05 14:59:41.000000 cassiopeia-5.1.2/cassiopeia/datastores/ghost.py
+-rw-rw-rw-   0        0        0     2145 2023-02-12 18:12:02.000000 cassiopeia-5.1.2/cassiopeia/datastores/image.py
+drwxrwxrwx   0        0        0        0 2024-05-12 02:26:10.711836 cassiopeia-5.1.2/cassiopeia/datastores/kernel/
+-rw-rw-rw-   0        0        0     1912 2024-05-05 06:23:06.000000 cassiopeia-5.1.2/cassiopeia/datastores/kernel/__init__.py
+-rw-rw-rw-   0        0        0     2057 2024-05-05 03:37:59.000000 cassiopeia-5.1.2/cassiopeia/datastores/kernel/account.py
+-rw-rw-rw-   0        0        0     2400 2023-02-12 18:12:02.000000 cassiopeia-5.1.2/cassiopeia/datastores/kernel/champion.py
+-rw-rw-rw-   0        0        0     8555 2023-02-12 18:12:02.000000 cassiopeia-5.1.2/cassiopeia/datastores/kernel/championmastery.py
+-rw-rw-rw-   0        0        0     4637 2023-02-12 18:12:02.000000 cassiopeia-5.1.2/cassiopeia/datastores/kernel/common.py
+-rw-rw-rw-   0        0        0    11466 2023-02-12 18:12:02.000000 cassiopeia-5.1.2/cassiopeia/datastores/kernel/leagues.py
+-rw-rw-rw-   0        0        0    12070 2023-02-12 18:12:02.000000 cassiopeia-5.1.2/cassiopeia/datastores/kernel/match.py
+-rw-rw-rw-   0        0        0     3216 2024-05-05 15:01:18.000000 cassiopeia-5.1.2/cassiopeia/datastores/kernel/spectator.py
+-rw-rw-rw-   0        0        0     3038 2024-04-10 05:17:47.000000 cassiopeia-5.1.2/cassiopeia/datastores/kernel/status.py
+-rw-rw-rw-   0        0        0     2189 2024-05-05 03:37:59.000000 cassiopeia-5.1.2/cassiopeia/datastores/kernel/summoner.py
+-rw-rw-rw-   0        0        0     4033 2024-04-10 05:26:46.000000 cassiopeia-5.1.2/cassiopeia/datastores/lolwikia.py
+-rw-rw-rw-   0        0        0     2897 2023-02-12 18:12:02.000000 cassiopeia-5.1.2/cassiopeia/datastores/merakianalyticscdn.py
+drwxrwxrwx   0        0        0        0 2024-05-12 02:26:10.836524 cassiopeia-5.1.2/cassiopeia/datastores/riotapi/
+-rw-rw-rw-   0        0        0     3565 2024-05-05 06:23:17.000000 cassiopeia-5.1.2/cassiopeia/datastores/riotapi/__init__.py
+-rw-rw-rw-   0        0        0     2880 2024-05-12 02:24:35.000000 cassiopeia-5.1.2/cassiopeia/datastores/riotapi/account.py
+-rw-rw-rw-   0        0        0     2643 2023-02-12 18:12:02.000000 cassiopeia-5.1.2/cassiopeia/datastores/riotapi/champion.py
+-rw-rw-rw-   0        0        0    10255 2024-04-10 05:17:47.000000 cassiopeia-5.1.2/cassiopeia/datastores/riotapi/championmastery.py
+-rw-rw-rw-   0        0        0    17773 2023-02-12 18:12:02.000000 cassiopeia-5.1.2/cassiopeia/datastores/riotapi/common.py
+-rw-rw-rw-   0        0        0    15725 2023-02-12 18:12:02.000000 cassiopeia-5.1.2/cassiopeia/datastores/riotapi/leagues.py
+-rw-rw-rw-   0        0        0     8276 2023-02-12 18:12:02.000000 cassiopeia-5.1.2/cassiopeia/datastores/riotapi/match.py
+-rw-rw-rw-   0        0        0     3628 2024-05-05 15:04:20.000000 cassiopeia-5.1.2/cassiopeia/datastores/riotapi/spectator.py
+-rw-rw-rw-   0        0        0     3530 2024-04-10 05:17:47.000000 cassiopeia-5.1.2/cassiopeia/datastores/riotapi/status.py
+-rw-rw-rw-   0        0        0     2742 2024-05-05 03:37:59.000000 cassiopeia-5.1.2/cassiopeia/datastores/riotapi/summoner.py
+-rw-rw-rw-   0        0        0    91633 2024-05-05 15:00:09.000000 cassiopeia-5.1.2/cassiopeia/datastores/uniquekeys.py
+drwxrwxrwx   0        0        0        0 2024-05-12 02:26:10.958913 cassiopeia-5.1.2/cassiopeia/dto/
+-rw-rw-rw-   0        0        0        0 2023-02-12 18:12:02.000000 cassiopeia-5.1.2/cassiopeia/dto/__init__.py
+-rw-rw-rw-   0        0        0       75 2024-05-05 03:37:59.000000 cassiopeia-5.1.2/cassiopeia/dto/account.py
+-rw-rw-rw-   0        0        0       84 2023-02-12 18:12:02.000000 cassiopeia-5.1.2/cassiopeia/dto/champion.py
+-rw-rw-rw-   0        0        0      196 2023-02-12 18:12:02.000000 cassiopeia-5.1.2/cassiopeia/dto/championmastery.py
+-rw-rw-rw-   0        0        0      407 2023-02-12 18:12:02.000000 cassiopeia-5.1.2/cassiopeia/dto/common.py
+-rw-rw-rw-   0        0        0      445 2023-02-12 18:12:02.000000 cassiopeia-5.1.2/cassiopeia/dto/league.py
+-rw-rw-rw-   0        0        0      215 2023-02-12 18:12:02.000000 cassiopeia-5.1.2/cassiopeia/dto/match.py
+-rw-rw-rw-   0        0        0       77 2023-02-12 18:12:02.000000 cassiopeia-5.1.2/cassiopeia/dto/patch.py
+-rw-rw-rw-   0        0        0      133 2023-02-12 18:12:02.000000 cassiopeia-5.1.2/cassiopeia/dto/spectator.py
+drwxrwxrwx   0        0        0        0 2024-05-12 02:26:11.085586 cassiopeia-5.1.2/cassiopeia/dto/staticdata/
+-rw-rw-rw-   0        0        0      516 2023-02-12 18:12:02.000000 cassiopeia-5.1.2/cassiopeia/dto/staticdata/__init__.py
+-rw-rw-rw-   0        0        0      334 2023-02-12 18:12:02.000000 cassiopeia-5.1.2/cassiopeia/dto/staticdata/champion.py
+-rw-rw-rw-   0        0        0        0 2023-02-12 18:12:02.000000 cassiopeia-5.1.2/cassiopeia/dto/staticdata/common.py
+-rw-rw-rw-   0        0        0      118 2023-02-12 18:12:02.000000 cassiopeia-5.1.2/cassiopeia/dto/staticdata/item.py
+-rw-rw-rw-   0        0        0      130 2023-02-12 18:12:02.000000 cassiopeia-5.1.2/cassiopeia/dto/staticdata/language.py
+-rw-rw-rw-   0        0        0      116 2023-02-12 18:12:02.000000 cassiopeia-5.1.2/cassiopeia/dto/staticdata/map.py
+-rw-rw-rw-   0        0        0      139 2023-02-12 18:12:02.000000 cassiopeia-5.1.2/cassiopeia/dto/staticdata/profileicon.py
+-rw-rw-rw-   0        0        0       74 2023-02-12 18:12:02.000000 cassiopeia-5.1.2/cassiopeia/dto/staticdata/realm.py
+-rw-rw-rw-   0        0        0      209 2023-02-12 18:12:02.000000 cassiopeia-5.1.2/cassiopeia/dto/staticdata/rune.py
+-rw-rw-rw-   0        0        0      136 2023-02-12 18:12:02.000000 cassiopeia-5.1.2/cassiopeia/dto/staticdata/summonerspell.py
+-rw-rw-rw-   0        0        0       80 2023-02-12 18:12:02.000000 cassiopeia-5.1.2/cassiopeia/dto/staticdata/version.py
+-rw-rw-rw-   0        0        0       79 2023-02-12 18:12:02.000000 cassiopeia-5.1.2/cassiopeia/dto/status.py
+-rw-rw-rw-   0        0        0       76 2023-02-12 18:12:02.000000 cassiopeia-5.1.2/cassiopeia/dto/summoner.py
+-rw-rw-rw-   0        0        0    26420 2023-02-12 18:12:02.000000 cassiopeia-5.1.2/cassiopeia/profile_icon_names.json
+drwxrwxrwx   0        0        0        0 2024-05-12 02:26:11.088116 cassiopeia-5.1.2/cassiopeia/resources/
+-rw-rw-rw-   0        0        0    15654 2023-02-12 18:12:02.000000 cassiopeia-5.1.2/cassiopeia/resources/summonersRiftAreas.png
+drwxrwxrwx   0        0        0        0 2024-05-12 02:26:11.213543 cassiopeia-5.1.2/cassiopeia/transformers/
+-rw-rw-rw-   0        0        0      850 2024-05-05 06:23:23.000000 cassiopeia-5.1.2/cassiopeia/transformers/__init__.py
+-rw-rw-rw-   0        0        0      888 2024-05-05 03:37:59.000000 cassiopeia-5.1.2/cassiopeia/transformers/account.py
+-rw-rw-rw-   0        0        0     1091 2023-02-12 18:12:02.000000 cassiopeia-5.1.2/cassiopeia/transformers/champion.py
+-rw-rw-rw-   0        0        0     2203 2023-02-12 18:12:02.000000 cassiopeia-5.1.2/cassiopeia/transformers/championmastery.py
+-rw-rw-rw-   0        0        0     5348 2023-02-12 18:12:02.000000 cassiopeia-5.1.2/cassiopeia/transformers/leagues.py
+-rw-rw-rw-   0        0        0     2974 2023-02-12 18:12:02.000000 cassiopeia-5.1.2/cassiopeia/transformers/match.py
+-rw-rw-rw-   0        0        0     2665 2024-05-05 14:48:17.000000 cassiopeia-5.1.2/cassiopeia/transformers/spectator.py
+-rw-rw-rw-   0        0        0    15350 2023-02-12 18:12:02.000000 cassiopeia-5.1.2/cassiopeia/transformers/staticdata.py
+-rw-rw-rw-   0        0        0      947 2023-02-12 18:12:02.000000 cassiopeia-5.1.2/cassiopeia/transformers/status.py
+-rw-rw-rw-   0        0        0      906 2024-05-05 03:37:59.000000 cassiopeia-5.1.2/cassiopeia/transformers/summoner.py
+drwxrwxrwx   0        0        0        0 2024-05-12 02:26:10.079230 cassiopeia-5.1.2/cassiopeia.egg-info/
+-rw-rw-rw-   0        0        0      858 2024-05-12 02:26:09.000000 cassiopeia-5.1.2/cassiopeia.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3823 2024-05-12 02:26:09.000000 cassiopeia-5.1.2/cassiopeia.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-12 02:26:09.000000 cassiopeia-5.1.2/cassiopeia.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       65 2024-05-12 02:26:09.000000 cassiopeia-5.1.2/cassiopeia.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-12 02:26:09.000000 cassiopeia-5.1.2/cassiopeia.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2024-04-10 05:29:30.000000 cassiopeia-5.1.2/cassiopeia.egg-info/zip-safe
+-rw-rw-rw-   0        0        0      123 2024-05-12 02:26:11.359890 cassiopeia-5.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1537 2024-05-12 02:25:27.000000 cassiopeia-5.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-12 02:26:11.353215 cassiopeia-5.1.2/test/
+-rw-rw-rw-   0        0        0        0 2023-02-12 18:12:02.000000 cassiopeia-5.1.2/test/__init__.py
+-rw-rw-rw-   0        0        0      532 2023-02-12 18:12:02.000000 cassiopeia-5.1.2/test/constants.py
+-rw-rw-rw-   0        0        0     1369 2023-02-12 18:12:02.000000 cassiopeia-5.1.2/test/test_champion.py
+-rw-rw-rw-   0        0        0     2201 2023-02-12 18:12:02.000000 cassiopeia-5.1.2/test/test_championmastery.py
+-rw-rw-rw-   0        0        0      278 2023-02-12 18:12:02.000000 cassiopeia-5.1.2/test/test_championrotation.py
+-rw-rw-rw-   0        0        0     9322 2024-05-05 14:50:20.000000 cassiopeia-5.1.2/test/test_examples.py
+-rw-rw-rw-   0        0        0      689 2023-02-12 18:12:02.000000 cassiopeia-5.1.2/test/test_items.py
+-rw-rw-rw-   0        0        0     2473 2023-02-12 18:12:02.000000 cassiopeia-5.1.2/test/test_league.py
+-rw-rw-rw-   0        0        0      734 2023-02-12 18:12:02.000000 cassiopeia-5.1.2/test/test_map_location.py
+-rw-rw-rw-   0        0        0     1413 2023-02-12 18:12:02.000000 cassiopeia-5.1.2/test/test_match.py
+-rw-rw-rw-   0        0        0     2329 2023-02-12 18:12:02.000000 cassiopeia-5.1.2/test/test_matchhistory.py
+-rw-rw-rw-   0        0        0      708 2023-02-12 18:12:02.000000 cassiopeia-5.1.2/test/test_patches.py
+-rw-rw-rw-   0        0        0      879 2023-02-12 18:12:02.000000 cassiopeia-5.1.2/test/test_status.py
+-rw-rw-rw-   0        0        0     2023 2023-02-12 18:12:02.000000 cassiopeia-5.1.2/test/test_summoner.py
```

### Comparing `cassiopeia-5.1.1/LICENSE.txt` & `cassiopeia-5.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.1.1/PKG-INFO` & `cassiopeia-5.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cassiopeia
-Version: 5.1.1
+Version: 5.1.2
 Summary: Riot Games Developer API Wrapper (3rd Party)
 Home-page: https://github.com/meraki-analytics/cassiopeia
 Author: Jason Maldonis; Rob Rua
 Author-email: team@merakianalytics.com
 License: MIT
 Keywords: LoL,League of Legends,Riot Games,API,REST
 Classifier: Development Status :: 4 - Beta
```

### Comparing `cassiopeia-5.1.1/cassiopeia/__init__.py` & `cassiopeia-5.1.2/cassiopeia/__init__.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.1.1/cassiopeia/_configuration/__init__.py` & `cassiopeia-5.1.2/cassiopeia/_configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.1.1/cassiopeia/_configuration/load.py` & `cassiopeia-5.1.2/cassiopeia/_configuration/load.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.1.1/cassiopeia/_configuration/settings.py` & `cassiopeia-5.1.2/cassiopeia/_configuration/settings.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.1.1/cassiopeia/cassiopeia.py` & `cassiopeia-5.1.2/cassiopeia/cassiopeia.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.1.1/cassiopeia/core/__init__.py` & `cassiopeia-5.1.2/cassiopeia/core/__init__.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.1.1/cassiopeia/core/account.py` & `cassiopeia-5.1.2/cassiopeia/core/account.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.1.1/cassiopeia/core/champion.py` & `cassiopeia-5.1.2/cassiopeia/core/champion.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.1.1/cassiopeia/core/championmastery.py` & `cassiopeia-5.1.2/cassiopeia/core/championmastery.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.1.1/cassiopeia/core/common.py` & `cassiopeia-5.1.2/cassiopeia/core/common.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.1.1/cassiopeia/core/league.py` & `cassiopeia-5.1.2/cassiopeia/core/league.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.1.1/cassiopeia/core/match.py` & `cassiopeia-5.1.2/cassiopeia/core/match.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.1.1/cassiopeia/core/patch.py` & `cassiopeia-5.1.2/cassiopeia/core/patch.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.1.1/cassiopeia/core/spectator.py` & `cassiopeia-5.1.2/cassiopeia/core/spectator.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.1.1/cassiopeia/core/staticdata/champion.py` & `cassiopeia-5.1.2/cassiopeia/core/staticdata/champion.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.1.1/cassiopeia/core/staticdata/common.py` & `cassiopeia-5.1.2/cassiopeia/core/staticdata/common.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.1.1/cassiopeia/core/staticdata/item.py` & `cassiopeia-5.1.2/cassiopeia/core/staticdata/item.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.1.1/cassiopeia/core/staticdata/language.py` & `cassiopeia-5.1.2/cassiopeia/core/staticdata/language.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.1.1/cassiopeia/core/staticdata/languagestrings.py` & `cassiopeia-5.1.2/cassiopeia/core/staticdata/languagestrings.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.1.1/cassiopeia/core/staticdata/map.py` & `cassiopeia-5.1.2/cassiopeia/core/staticdata/map.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.1.1/cassiopeia/core/staticdata/profileicon.py` & `cassiopeia-5.1.2/cassiopeia/core/staticdata/profileicon.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.1.1/cassiopeia/core/staticdata/realm.py` & `cassiopeia-5.1.2/cassiopeia/core/staticdata/realm.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.1.1/cassiopeia/core/staticdata/rune.py` & `cassiopeia-5.1.2/cassiopeia/core/staticdata/rune.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.1.1/cassiopeia/core/staticdata/summonerspell.py` & `cassiopeia-5.1.2/cassiopeia/core/staticdata/summonerspell.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.1.1/cassiopeia/core/staticdata/version.py` & `cassiopeia-5.1.2/cassiopeia/core/staticdata/version.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.1.1/cassiopeia/core/status.py` & `cassiopeia-5.1.2/cassiopeia/core/status.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.1.1/cassiopeia/core/summoner.py` & `cassiopeia-5.1.2/cassiopeia/core/summoner.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.1.1/cassiopeia/data.py` & `cassiopeia-5.1.2/cassiopeia/data.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.1.1/cassiopeia/datastores/cache.py` & `cassiopeia-5.1.2/cassiopeia/datastores/cache.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.1.1/cassiopeia/datastores/common.py` & `cassiopeia-5.1.2/cassiopeia/datastores/common.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.1.1/cassiopeia/datastores/ddragon.py` & `cassiopeia-5.1.2/cassiopeia/datastores/ddragon.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.1.1/cassiopeia/datastores/ghost.py` & `cassiopeia-5.1.2/cassiopeia/datastores/ghost.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.1.1/cassiopeia/datastores/image.py` & `cassiopeia-5.1.2/cassiopeia/datastores/image.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.1.1/cassiopeia/datastores/kernel/__init__.py` & `cassiopeia-5.1.2/cassiopeia/datastores/kernel/__init__.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.1.1/cassiopeia/datastores/kernel/account.py` & `cassiopeia-5.1.2/cassiopeia/datastores/kernel/account.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.1.1/cassiopeia/datastores/kernel/champion.py` & `cassiopeia-5.1.2/cassiopeia/datastores/kernel/champion.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.1.1/cassiopeia/datastores/kernel/championmastery.py` & `cassiopeia-5.1.2/cassiopeia/datastores/kernel/championmastery.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.1.1/cassiopeia/datastores/kernel/common.py` & `cassiopeia-5.1.2/cassiopeia/datastores/kernel/common.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.1.1/cassiopeia/datastores/kernel/leagues.py` & `cassiopeia-5.1.2/cassiopeia/datastores/kernel/leagues.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.1.1/cassiopeia/datastores/kernel/match.py` & `cassiopeia-5.1.2/cassiopeia/datastores/kernel/match.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.1.1/cassiopeia/datastores/kernel/spectator.py` & `cassiopeia-5.1.2/cassiopeia/datastores/kernel/spectator.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.1.1/cassiopeia/datastores/kernel/status.py` & `cassiopeia-5.1.2/cassiopeia/datastores/kernel/status.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.1.1/cassiopeia/datastores/kernel/summoner.py` & `cassiopeia-5.1.2/cassiopeia/datastores/kernel/summoner.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.1.1/cassiopeia/datastores/lolwikia.py` & `cassiopeia-5.1.2/cassiopeia/datastores/lolwikia.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.1.1/cassiopeia/datastores/merakianalyticscdn.py` & `cassiopeia-5.1.2/cassiopeia/datastores/merakianalyticscdn.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.1.1/cassiopeia/datastores/riotapi/__init__.py` & `cassiopeia-5.1.2/cassiopeia/datastores/riotapi/__init__.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.1.1/cassiopeia/datastores/riotapi/account.py` & `cassiopeia-5.1.2/cassiopeia/datastores/riotapi/account.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     DataSource,
     PipelineContext,
     Query,
     NotFoundError,
     validate_query,
 )
 from .common import RiotAPIService, APINotFoundError
-from ...data import Platform
+from ...data import Platform, Continent
 from ...dto.account import AccountDto
 from ..uniquekeys import convert_region_to_platform
 
 T = TypeVar("T")
 
 
 class AccountAPI(RiotAPIService):
@@ -50,14 +50,17 @@
     @get.register(AccountDto)
     @validate_query(_validate_get_account_query, convert_region_to_platform)
     def get_account(
         self, query: MutableMapping[str, Any], context: PipelineContext = None
     ) -> AccountDto:
         platform: Platform = query["platform"]
         continent = platform.continent
+        # For some reason, Riot routes the SEA region/continent to ASIA for this endpoint.
+        if continent == Continent.sea:
+            continent = Continent.asia
         if "puuid" in query:
             puuid = query["puuid"]
             url = "https://{continent}.api.riotgames.com/riot/account/v1/accounts/by-puuid/{puuid}".format(
                 continent=continent.value.lower(), puuid=puuid
             )
             endpoint = "accounts/puuid"
         elif "name" in query and "tagline" in query:
```

### Comparing `cassiopeia-5.1.1/cassiopeia/datastores/riotapi/champion.py` & `cassiopeia-5.1.2/cassiopeia/datastores/riotapi/champion.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.1.1/cassiopeia/datastores/riotapi/championmastery.py` & `cassiopeia-5.1.2/cassiopeia/datastores/riotapi/championmastery.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.1.1/cassiopeia/datastores/riotapi/common.py` & `cassiopeia-5.1.2/cassiopeia/datastores/riotapi/common.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.1.1/cassiopeia/datastores/riotapi/leagues.py` & `cassiopeia-5.1.2/cassiopeia/datastores/riotapi/leagues.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.1.1/cassiopeia/datastores/riotapi/match.py` & `cassiopeia-5.1.2/cassiopeia/datastores/riotapi/match.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.1.1/cassiopeia/datastores/riotapi/spectator.py` & `cassiopeia-5.1.2/cassiopeia/datastores/riotapi/spectator.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.1.1/cassiopeia/datastores/riotapi/status.py` & `cassiopeia-5.1.2/cassiopeia/datastores/riotapi/status.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.1.1/cassiopeia/datastores/riotapi/summoner.py` & `cassiopeia-5.1.2/cassiopeia/datastores/riotapi/summoner.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.1.1/cassiopeia/datastores/uniquekeys.py` & `cassiopeia-5.1.2/cassiopeia/datastores/uniquekeys.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.1.1/cassiopeia/dto/staticdata/__init__.py` & `cassiopeia-5.1.2/cassiopeia/dto/staticdata/__init__.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.1.1/cassiopeia/profile_icon_names.json` & `cassiopeia-5.1.2/cassiopeia/profile_icon_names.json`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.1.1/cassiopeia/resources/summonersRiftAreas.png` & `cassiopeia-5.1.2/cassiopeia/resources/summonersRiftAreas.png`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.1.1/cassiopeia/transformers/__init__.py` & `cassiopeia-5.1.2/cassiopeia/transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.1.1/cassiopeia/transformers/account.py` & `cassiopeia-5.1.2/cassiopeia/transformers/account.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.1.1/cassiopeia/transformers/champion.py` & `cassiopeia-5.1.2/cassiopeia/transformers/champion.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.1.1/cassiopeia/transformers/championmastery.py` & `cassiopeia-5.1.2/cassiopeia/transformers/championmastery.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.1.1/cassiopeia/transformers/leagues.py` & `cassiopeia-5.1.2/cassiopeia/transformers/leagues.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.1.1/cassiopeia/transformers/match.py` & `cassiopeia-5.1.2/cassiopeia/transformers/match.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.1.1/cassiopeia/transformers/spectator.py` & `cassiopeia-5.1.2/cassiopeia/transformers/spectator.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.1.1/cassiopeia/transformers/staticdata.py` & `cassiopeia-5.1.2/cassiopeia/transformers/staticdata.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.1.1/cassiopeia/transformers/status.py` & `cassiopeia-5.1.2/cassiopeia/transformers/status.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.1.1/cassiopeia/transformers/summoner.py` & `cassiopeia-5.1.2/cassiopeia/transformers/summoner.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.1.1/cassiopeia.egg-info/PKG-INFO` & `cassiopeia-5.1.2/cassiopeia.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cassiopeia
-Version: 5.1.1
+Version: 5.1.2
 Summary: Riot Games Developer API Wrapper (3rd Party)
 Home-page: https://github.com/meraki-analytics/cassiopeia
 Author: Jason Maldonis; Rob Rua
 Author-email: team@merakianalytics.com
 License: MIT
 Keywords: LoL,League of Legends,Riot Games,API,REST
 Classifier: Development Status :: 4 - Beta
```

### Comparing `cassiopeia-5.1.1/cassiopeia.egg-info/SOURCES.txt` & `cassiopeia-5.1.2/cassiopeia.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.1.1/setup.py` & `cassiopeia-5.1.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 # Require python 3.6
 if sys.version_info.major != 3 and sys.version_info.minor != 6:
     sys.exit("Cassiopeia requires Python 3.6.")
 
 setup(
     name="cassiopeia",
-    version="5.1.1",  # Keep the Cass version at parity with the largest Riot API major version, use the minor version for breaking changes, and the patch version for everything else
+    version="5.1.2",  # Keep the Cass version at parity with the largest Riot API major version, use the minor version for breaking changes, and the patch version for everything else
     author="Jason Maldonis; Rob Rua",
     author_email="team@merakianalytics.com",
     url="https://github.com/meraki-analytics/cassiopeia",
     description="Riot Games Developer API Wrapper (3rd Party)",
     keywords=["LoL", "League of Legends", "Riot Games", "API", "REST"],
     classifiers=[
         "Development Status :: 4 - Beta",
```

### Comparing `cassiopeia-5.1.1/test/constants.py` & `cassiopeia-5.1.2/test/constants.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.1.1/test/test_champion.py` & `cassiopeia-5.1.2/test/test_champion.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.1.1/test/test_championmastery.py` & `cassiopeia-5.1.2/test/test_championmastery.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.1.1/test/test_examples.py` & `cassiopeia-5.1.2/test/test_examples.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.1.1/test/test_items.py` & `cassiopeia-5.1.2/test/test_items.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.1.1/test/test_league.py` & `cassiopeia-5.1.2/test/test_league.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.1.1/test/test_map_location.py` & `cassiopeia-5.1.2/test/test_map_location.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.1.1/test/test_match.py` & `cassiopeia-5.1.2/test/test_match.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.1.1/test/test_matchhistory.py` & `cassiopeia-5.1.2/test/test_matchhistory.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.1.1/test/test_patches.py` & `cassiopeia-5.1.2/test/test_patches.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.1.1/test/test_status.py` & `cassiopeia-5.1.2/test/test_status.py`

 * *Files identical despite different names*

### Comparing `cassiopeia-5.1.1/test/test_summoner.py` & `cassiopeia-5.1.2/test/test_summoner.py`

 * *Files identical despite different names*

