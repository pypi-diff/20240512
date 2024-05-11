# Comparing `tmp/nokey-0.4.0.tar.gz` & `tmp/nokey-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nokey-0.4.0.tar", last modified: Thu May  9 00:37:27 2024, max compression
+gzip compressed data, was "nokey-0.5.0.tar", max compression
```

## Comparing `nokey-0.4.0.tar` & `nokey-0.5.0.tar`

### file list

```diff
@@ -1,90 +1,61 @@
-drwx------   0 root         (0) root         (0)        0 2024-05-09 00:37:27.362013 nokey-0.4.0/
--rw-------   0 root         (0) root         (0)     1068 2024-04-10 23:28:41.000000 nokey-0.4.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3756 2024-05-09 00:37:27.362013 nokey-0.4.0/PKG-INFO
--rw-------   0 root         (0) root         (0)     3178 2024-05-09 00:35:34.000000 nokey-0.4.0/README.md
-drwx------   0 root         (0) root         (0)        0 2024-05-09 00:37:27.050013 nokey-0.4.0/nokey/
--rw-------   0 root         (0) root         (0)        0 2024-05-09 00:33:11.000000 nokey-0.4.0/nokey/__init__.py
-drwx------   0 root         (0) root         (0)        0 2024-05-09 00:37:27.074013 nokey-0.4.0/nokey/activities/
--rw-------   0 root         (0) root         (0)     5116 2024-05-09 00:33:11.000000 nokey-0.4.0/nokey/activities/bored_api.py
-drwx------   0 root         (0) root         (0)        0 2024-05-09 00:37:27.082013 nokey-0.4.0/nokey/animals/
--rw-------   0 root         (0) root         (0)        0 2024-05-09 00:33:11.000000 nokey-0.4.0/nokey/animals/__init__.py
--rw-------   0 root         (0) root         (0)     2754 2024-05-09 00:33:11.000000 nokey-0.4.0/nokey/animals/dog_api.py
-drwx------   0 root         (0) root         (0)        0 2024-05-09 00:37:27.086013 nokey-0.4.0/nokey/art_and_images/
--rw-------   0 root         (0) root         (0)     7770 2024-05-09 00:33:11.000000 nokey-0.4.0/nokey/art_and_images/lorem_picsum.py
-drwx------   0 root         (0) root         (0)        0 2024-05-09 00:37:27.098013 nokey-0.4.0/nokey/books_and_literature/
--rw-------   0 root         (0) root         (0)        0 2024-05-09 00:33:11.000000 nokey-0.4.0/nokey/books_and_literature/__init__.py
--rw-------   0 root         (0) root         (0)     6079 2024-05-09 00:33:11.000000 nokey-0.4.0/nokey/books_and_literature/gutendex.py
-drwx------   0 root         (0) root         (0)        0 2024-05-09 00:37:27.106013 nokey-0.4.0/nokey/calendar/
--rw-------   0 root         (0) root         (0)        0 2024-05-09 00:33:11.000000 nokey-0.4.0/nokey/calendar/__init__.py
--rw-------   0 root         (0) root         (0)     4848 2024-05-09 00:33:11.000000 nokey-0.4.0/nokey/calendar/nager_date.py
-drwx------   0 root         (0) root         (0)        0 2024-05-09 00:37:27.118013 nokey-0.4.0/nokey/country_info/
--rw-------   0 root         (0) root         (0)        0 2024-05-09 00:33:11.000000 nokey-0.4.0/nokey/country_info/__init__.py
--rw-------   0 root         (0) root         (0)     4740 2024-05-09 00:33:11.000000 nokey-0.4.0/nokey/country_info/rest_country.py
-drwx------   0 root         (0) root         (0)        0 2024-05-09 00:37:27.150013 nokey-0.4.0/nokey/developer_tools/
--rw-------   0 root         (0) root         (0)        0 2024-05-09 00:33:11.000000 nokey-0.4.0/nokey/developer_tools/__init__.py
--rw-------   0 root         (0) root         (0)     3945 2024-05-09 00:33:11.000000 nokey-0.4.0/nokey/developer_tools/apis_guru.py
--rw-------   0 root         (0) root         (0)     3564 2024-05-09 00:33:11.000000 nokey-0.4.0/nokey/developer_tools/filter_lists.py
--rw-------   0 root         (0) root         (0)     2578 2024-05-09 00:33:11.000000 nokey-0.4.0/nokey/developer_tools/microlink.py
--rw-------   0 root         (0) root         (0)     7314 2024-05-09 00:33:11.000000 nokey-0.4.0/nokey/developer_tools/url_haus.py
--rw-------   0 root         (0) root         (0)     1621 2024-05-09 00:33:11.000000 nokey-0.4.0/nokey/developer_tools/url_shortener.py
-drwx------   0 root         (0) root         (0)        0 2024-05-09 00:37:27.158013 nokey-0.4.0/nokey/education/
--rw-------   0 root         (0) root         (0)        0 2024-05-09 00:33:11.000000 nokey-0.4.0/nokey/education/__init__.py
--rw-------   0 root         (0) root         (0)     2348 2024-05-09 00:33:11.000000 nokey-0.4.0/nokey/education/university_domains_and_names.py
-drwx------   0 root         (0) root         (0)        0 2024-05-09 00:37:27.186013 nokey-0.4.0/nokey/finance_and_crypto/
--rw-------   0 root         (0) root         (0)        0 2024-05-09 00:33:11.000000 nokey-0.4.0/nokey/finance_and_crypto/__init__.py
--rw-------   0 root         (0) root         (0)     5877 2024-05-09 00:33:11.000000 nokey-0.4.0/nokey/finance_and_crypto/coinmap.py
--rw-------   0 root         (0) root         (0)     2513 2024-05-09 00:33:11.000000 nokey-0.4.0/nokey/finance_and_crypto/exchange_api.py
--rw-------   0 root         (0) root         (0)     1127 2024-05-09 00:33:11.000000 nokey-0.4.0/nokey/finance_and_crypto/wall_street_bets.py
-drwx------   0 root         (0) root         (0)        0 2024-05-09 00:37:27.198013 nokey-0.4.0/nokey/food/
--rw-------   0 root         (0) root         (0)        0 2024-05-09 00:33:11.000000 nokey-0.4.0/nokey/food/__init__.py
--rw-------   0 root         (0) root         (0)     3198 2024-05-09 00:33:11.000000 nokey-0.4.0/nokey/food/fruityvice.py
-drwx------   0 root         (0) root         (0)        0 2024-05-09 00:37:27.210013 nokey-0.4.0/nokey/games/
--rw-------   0 root         (0) root         (0)        0 2024-05-09 00:33:11.000000 nokey-0.4.0/nokey/games/__init__.py
--rw-------   0 root         (0) root         (0)     6542 2024-05-09 00:33:11.000000 nokey-0.4.0/nokey/games/free_to_game.py
--rw-------   0 root         (0) root         (0)     5382 2024-05-09 00:33:11.000000 nokey-0.4.0/nokey/games/open_trivia_db.py
-drwx------   0 root         (0) root         (0)        0 2024-05-09 00:37:27.226013 nokey-0.4.0/nokey/geolocation/
--rw-------   0 root         (0) root         (0)        0 2024-05-09 00:33:11.000000 nokey-0.4.0/nokey/geolocation/__init__.py
--rw-------   0 root         (0) root         (0)     1045 2024-05-09 00:33:11.000000 nokey-0.4.0/nokey/geolocation/ip_api.py
--rw-------   0 root         (0) root         (0)     1874 2024-05-09 00:33:11.000000 nokey-0.4.0/nokey/geolocation/zippopotamus.py
-drwx------   0 root         (0) root         (0)        0 2024-05-09 00:37:27.242013 nokey-0.4.0/nokey/government/
--rw-------   0 root         (0) root         (0)        0 2024-05-09 00:33:11.000000 nokey-0.4.0/nokey/government/__init__.py
--rw-------   0 root         (0) root         (0)    10654 2024-05-09 00:33:11.000000 nokey-0.4.0/nokey/government/federal_register.py
--rw-------   0 root         (0) root         (0)   157333 2024-05-09 00:33:11.000000 nokey-0.4.0/nokey/government/usa_spending.py
-drwx------   0 root         (0) root         (0)        0 2024-05-09 00:37:27.266013 nokey-0.4.0/nokey/helperFuncs/
--rw-------   0 root         (0) root         (0)        0 2024-05-09 00:33:11.000000 nokey-0.4.0/nokey/helperFuncs/__init__.py
--rw-------   0 root         (0) root         (0)      822 2024-05-09 00:33:11.000000 nokey-0.4.0/nokey/helperFuncs/get_api_list.py
--rw-------   0 root         (0) root         (0)     5137 2024-05-09 00:33:11.000000 nokey-0.4.0/nokey/helperFuncs/make_request.py
--rw-------   0 root         (0) root         (0)      970 2024-05-09 00:33:11.000000 nokey-0.4.0/nokey/helperFuncs/nokey_apis.py
-drwx------   0 root         (0) root         (0)        0 2024-05-09 00:37:27.274013 nokey-0.4.0/nokey/inspiration/
--rw-------   0 root         (0) root         (0)        0 2024-05-09 00:33:11.000000 nokey-0.4.0/nokey/inspiration/__init__.py
--rw-------   0 root         (0) root         (0)     5925 2024-05-09 00:33:11.000000 nokey-0.4.0/nokey/inspiration/dictum.py
-drwx------   0 root         (0) root         (0)        0 2024-05-09 00:37:27.286013 nokey-0.4.0/nokey/jokes/
--rw-------   0 root         (0) root         (0)        0 2024-05-09 00:33:11.000000 nokey-0.4.0/nokey/jokes/__init__.py
--rw-------   0 root         (0) root         (0)     3004 2024-05-09 00:33:11.000000 nokey-0.4.0/nokey/jokes/joke_api.py
-drwx------   0 root         (0) root         (0)        0 2024-05-09 00:37:27.294013 nokey-0.4.0/nokey/language/
--rw-------   0 root         (0) root         (0)        0 2024-05-09 00:33:11.000000 nokey-0.4.0/nokey/language/__init__.py
--rw-------   0 root         (0) root         (0)     1185 2024-05-09 00:33:11.000000 nokey-0.4.0/nokey/language/free_dictionary.py
-drwx------   0 root         (0) root         (0)        0 2024-05-09 00:37:27.306013 nokey-0.4.0/nokey/random/
--rw-------   0 root         (0) root         (0)        0 2024-05-09 00:33:11.000000 nokey-0.4.0/nokey/random/__init__.py
--rw-------   0 root         (0) root         (0)     1119 2024-05-09 00:33:11.000000 nokey-0.4.0/nokey/random/random_user.py
-drwx------   0 root         (0) root         (0)        0 2024-05-09 00:37:27.318013 nokey-0.4.0/nokey/science_and_nature/
--rw-------   0 root         (0) root         (0)        0 2024-05-09 00:33:11.000000 nokey-0.4.0/nokey/science_and_nature/__init__.py
--rw-------   0 root         (0) root         (0)    50596 2024-05-09 00:33:11.000000 nokey-0.4.0/nokey/science_and_nature/integrated_taxonomic_information_system.py
--rw-------   0 root         (0) root         (0)     2948 2024-05-09 00:33:11.000000 nokey-0.4.0/nokey/science_and_nature/nobel_prize.py
-drwx------   0 root         (0) root         (0)        0 2024-05-09 00:37:27.330013 nokey-0.4.0/nokey/spaceflight/
--rw-------   0 root         (0) root         (0)        0 2024-05-09 00:33:11.000000 nokey-0.4.0/nokey/spaceflight/__init__.py
--rw-------   0 root         (0) root         (0)     8784 2024-05-09 00:33:11.000000 nokey-0.4.0/nokey/spaceflight/spaceflight_news.py
-drwx------   0 root         (0) root         (0)        0 2024-05-09 00:37:27.338013 nokey-0.4.0/nokey/tv_and_film/
--rw-------   0 root         (0) root         (0)        0 2024-05-09 00:33:11.000000 nokey-0.4.0/nokey/tv_and_film/__init__.py
--rw-------   0 root         (0) root         (0)    43523 2024-05-09 00:33:11.000000 nokey-0.4.0/nokey/tv_and_film/star_trek_api.py
-drwx------   0 root         (0) root         (0)        0 2024-05-09 00:37:27.350013 nokey-0.4.0/nokey/weather/
--rw-------   0 root         (0) root         (0)        0 2024-05-09 00:33:11.000000 nokey-0.4.0/nokey/weather/__init__.py
--rw-------   0 root         (0) root         (0)    26115 2024-05-09 00:33:11.000000 nokey-0.4.0/nokey/weather/national_weather_service.py
-drwx------   0 root         (0) root         (0)        0 2024-05-09 00:37:27.358013 nokey-0.4.0/nokey.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3756 2024-05-09 00:37:26.000000 nokey-0.4.0/nokey.egg-info/PKG-INFO
--rw-------   0 root         (0) root         (0)     1979 2024-05-09 00:37:26.000000 nokey-0.4.0/nokey.egg-info/SOURCES.txt
--rw-------   0 root         (0) root         (0)        1 2024-05-09 00:37:26.000000 nokey-0.4.0/nokey.egg-info/dependency_links.txt
--rw-------   0 root         (0) root         (0)       27 2024-05-09 00:37:26.000000 nokey-0.4.0/nokey.egg-info/requires.txt
--rw-------   0 root         (0) root         (0)        6 2024-05-09 00:37:26.000000 nokey-0.4.0/nokey.egg-info/top_level.txt
--rw-------   0 root         (0) root         (0)      557 2024-05-09 00:36:14.000000 nokey-0.4.0/pyproject.toml
--rw-------   0 root         (0) root         (0)       38 2024-05-09 00:37:27.366013 nokey-0.4.0/setup.cfg
+-rw-r--r--   0        0        0     1068 2024-04-10 23:28:41.225586 nokey-0.5.0/LICENSE
+-rw-r--r--   0        0        0     3236 2024-05-11 23:20:17.607494 nokey-0.5.0/README.md
+-rw-r--r--   0        0        0        0 2024-05-11 23:18:00.967494 nokey-0.5.0/nokey/__init__.py
+-rw-r--r--   0        0        0     5116 2024-05-11 23:18:00.979494 nokey-0.5.0/nokey/activities/bored_api.py
+-rw-r--r--   0        0        0        0 2024-05-11 23:18:00.939494 nokey-0.5.0/nokey/animals/__init__.py
+-rw-r--r--   0        0        0     2754 2024-05-11 23:18:00.935494 nokey-0.5.0/nokey/animals/dog_api.py
+-rw-r--r--   0        0        0        0 2024-05-11 23:18:01.035494 nokey-0.5.0/nokey/art_and_images/__init__.py
+-rw-r--r--   0        0        0    92946 2024-05-11 23:18:01.031494 nokey-0.5.0/nokey/art_and_images/artic.py
+-rw-r--r--   0        0        0     7770 2024-05-11 23:18:01.035494 nokey-0.5.0/nokey/art_and_images/lorem_picsum.py
+-rw-r--r--   0        0        0        0 2024-05-11 23:18:00.923494 nokey-0.5.0/nokey/books_and_literature/__init__.py
+-rw-r--r--   0        0        0     6079 2024-05-11 23:18:00.919494 nokey-0.5.0/nokey/books_and_literature/gutendex.py
+-rw-r--r--   0        0        0        0 2024-05-11 23:18:01.103494 nokey-0.5.0/nokey/calendar/__init__.py
+-rw-r--r--   0        0        0     4848 2024-05-11 23:18:01.099494 nokey-0.5.0/nokey/calendar/nager_date.py
+-rw-r--r--   0        0        0        0 2024-05-11 23:18:01.043494 nokey-0.5.0/nokey/country_info/__init__.py
+-rw-r--r--   0        0        0     4740 2024-05-11 23:18:01.043494 nokey-0.5.0/nokey/country_info/rest_country.py
+-rw-r--r--   0        0        0        0 2024-05-11 23:18:00.895494 nokey-0.5.0/nokey/developer_tools/__init__.py
+-rw-r--r--   0        0        0     3945 2024-05-11 23:18:00.887494 nokey-0.5.0/nokey/developer_tools/apis_guru.py
+-rw-r--r--   0        0        0     3564 2024-05-11 23:18:00.883494 nokey-0.5.0/nokey/developer_tools/filter_lists.py
+-rw-r--r--   0        0        0     2578 2024-05-11 23:18:00.883494 nokey-0.5.0/nokey/developer_tools/microlink.py
+-rw-r--r--   0        0        0     7314 2024-05-11 23:18:00.895494 nokey-0.5.0/nokey/developer_tools/url_haus.py
+-rw-r--r--   0        0        0     1621 2024-05-11 23:18:00.891494 nokey-0.5.0/nokey/developer_tools/url_shortener.py
+-rw-r--r--   0        0        0        0 2024-05-11 23:18:00.927494 nokey-0.5.0/nokey/education/__init__.py
+-rw-r--r--   0        0        0     2348 2024-05-11 23:18:00.931494 nokey-0.5.0/nokey/education/university_domains_and_names.py
+-rw-r--r--   0        0        0        0 2024-05-11 23:18:01.083494 nokey-0.5.0/nokey/finance_and_crypto/__init__.py
+-rw-r--r--   0        0        0     5877 2024-05-11 23:18:01.075494 nokey-0.5.0/nokey/finance_and_crypto/coinmap.py
+-rw-r--r--   0        0        0     2513 2024-05-11 23:18:01.079494 nokey-0.5.0/nokey/finance_and_crypto/exchange_api.py
+-rw-r--r--   0        0        0     1127 2024-05-11 23:18:01.087494 nokey-0.5.0/nokey/finance_and_crypto/wall_street_bets.py
+-rw-r--r--   0        0        0        0 2024-05-11 23:18:01.059494 nokey-0.5.0/nokey/food/__init__.py
+-rw-r--r--   0        0        0     3198 2024-05-11 23:18:01.059494 nokey-0.5.0/nokey/food/fruityvice.py
+-rw-r--r--   0        0        0        0 2024-05-11 23:18:01.011494 nokey-0.5.0/nokey/games/__init__.py
+-rw-r--r--   0        0        0     6542 2024-05-11 23:18:01.011494 nokey-0.5.0/nokey/games/free_to_game.py
+-rw-r--r--   0        0        0     5382 2024-05-11 23:18:01.007494 nokey-0.5.0/nokey/games/open_trivia_db.py
+-rw-r--r--   0        0        0        0 2024-05-11 23:18:01.019494 nokey-0.5.0/nokey/geolocation/__init__.py
+-rw-r--r--   0        0        0     1045 2024-05-11 23:18:01.023494 nokey-0.5.0/nokey/geolocation/ip_api.py
+-rw-r--r--   0        0        0     1874 2024-05-11 23:18:01.019494 nokey-0.5.0/nokey/geolocation/zippopotamus.py
+-rw-r--r--   0        0        0        0 2024-05-11 23:18:00.875494 nokey-0.5.0/nokey/government/__init__.py
+-rw-r--r--   0        0        0    10654 2024-05-11 23:18:00.867494 nokey-0.5.0/nokey/government/federal_register.py
+-rw-r--r--   0        0        0   157333 2024-05-11 23:18:00.875494 nokey-0.5.0/nokey/government/usa_spending.py
+-rw-r--r--   0        0        0        0 2024-05-11 23:18:00.955494 nokey-0.5.0/nokey/helperFuncs/__init__.py
+-rw-r--r--   0        0        0      822 2024-05-11 23:18:00.947494 nokey-0.5.0/nokey/helperFuncs/get_api_list.py
+-rw-r--r--   0        0        0     5137 2024-05-11 23:18:00.951494 nokey-0.5.0/nokey/helperFuncs/make_request.py
+-rw-r--r--   0        0        0      998 2024-05-11 23:18:00.947494 nokey-0.5.0/nokey/helperFuncs/nokey_apis.py
+-rw-r--r--   0        0        0        0 2024-05-11 23:18:00.911494 nokey-0.5.0/nokey/inspiration/__init__.py
+-rw-r--r--   0        0        0     5925 2024-05-11 23:18:00.915494 nokey-0.5.0/nokey/inspiration/dictum.py
+-rw-r--r--   0        0        0        0 2024-05-11 23:18:01.051494 nokey-0.5.0/nokey/jokes/__init__.py
+-rw-r--r--   0        0        0     3004 2024-05-11 23:18:01.051494 nokey-0.5.0/nokey/jokes/joke_api.py
+-rw-r--r--   0        0        0        0 2024-05-11 23:18:01.095494 nokey-0.5.0/nokey/language/__init__.py
+-rw-r--r--   0        0        0     1185 2024-05-11 23:18:01.091494 nokey-0.5.0/nokey/language/free_dictionary.py
+-rw-r--r--   0        0        0        0 2024-05-11 23:18:00.999494 nokey-0.5.0/nokey/random/__init__.py
+-rw-r--r--   0        0        0     1119 2024-05-11 23:18:00.999494 nokey-0.5.0/nokey/random/random_user.py
+-rw-r--r--   0        0        0        0 2024-05-11 23:18:00.991494 nokey-0.5.0/nokey/science_and_nature/__init__.py
+-rw-r--r--   0        0        0    50596 2024-05-11 23:18:00.987494 nokey-0.5.0/nokey/science_and_nature/integrated_taxonomic_information_system.py
+-rw-r--r--   0        0        0     2948 2024-05-11 23:18:00.991494 nokey-0.5.0/nokey/science_and_nature/nobel_prize.py
+-rw-r--r--   0        0        0        0 2024-05-11 23:18:00.963494 nokey-0.5.0/nokey/spaceflight/__init__.py
+-rw-r--r--   0        0        0     8784 2024-05-11 23:18:00.959494 nokey-0.5.0/nokey/spaceflight/spaceflight_news.py
+-rw-r--r--   0        0        0        0 2024-05-11 23:18:01.071494 nokey-0.5.0/nokey/tv_and_film/__init__.py
+-rw-r--r--   0        0        0    43523 2024-05-11 23:18:01.067494 nokey-0.5.0/nokey/tv_and_film/star_trek_api.py
+-rw-r--r--   0        0        0        0 2024-05-11 23:18:00.903494 nokey-0.5.0/nokey/weather/__init__.py
+-rw-r--r--   0        0        0    26115 2024-05-11 23:18:00.907494 nokey-0.5.0/nokey/weather/national_weather_service.py
+-rw-r--r--   0        0        0      684 2024-05-11 23:33:58.711494 nokey-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     4112 1970-01-01 00:00:00.000000 nokey-0.5.0/PKG-INFO
```

### Comparing `nokey-0.4.0/LICENSE` & `nokey-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nokey-0.4.0/PKG-INFO` & `nokey-0.5.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: nokey
-Version: 0.4.0
-Summary: A python package for accessing APIs that require no key.
-Author-email: Spyder Rex <billyjohnsonauthor@gmail.com>
-Project-URL: Homepage, https://github.com/SpyderRex/nokey
-Project-URL: Issues, https://github.com/Spyder/nokey/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: requests
-Requires-Dist: xmltodict==0.13.0
-
 # nokey - Access APIs without a Key
 
 nokey is a Python package designed to provide easy access to various APIs that do not require an API key for authentication. This project aims to simplify the process of interacting with different APIs by offering a unified interface for accessing them, all within a single Python package.
 
 ## Features
 
 - Access a growing collection of keyless APIs conveniently from one place.
@@ -141,14 +125,19 @@
 
 ## tv_and_film
 Star Trek API
 
 ## books_and_literature
 Gutendex
 
+## art_and_images
+Lorum Picsum
+
+Art Institute of Chicago
+
 # Future Roadmap
 As the project grows, we envision expanding the collection of keyless APIs to cover a wide range of categories. Your feedback and contributions will play a crucial role in shaping the future of nokey.
 
 # License
 This project is licensed under the MIT License - see the LICENSE file for details.
 
 # Documentation
```

### Comparing `nokey-0.4.0/nokey/activities/bored_api.py` & `nokey-0.5.0/nokey/activities/bored_api.py`

 * *Files identical despite different names*

### Comparing `nokey-0.4.0/nokey/animals/dog_api.py` & `nokey-0.5.0/nokey/animals/dog_api.py`

 * *Files identical despite different names*

### Comparing `nokey-0.4.0/nokey/art_and_images/lorem_picsum.py` & `nokey-0.5.0/nokey/art_and_images/lorem_picsum.py`

 * *Files identical despite different names*

### Comparing `nokey-0.4.0/nokey/books_and_literature/gutendex.py` & `nokey-0.5.0/nokey/books_and_literature/gutendex.py`

 * *Files identical despite different names*

### Comparing `nokey-0.4.0/nokey/calendar/nager_date.py` & `nokey-0.5.0/nokey/calendar/nager_date.py`

 * *Files identical despite different names*

### Comparing `nokey-0.4.0/nokey/country_info/rest_country.py` & `nokey-0.5.0/nokey/country_info/rest_country.py`

 * *Files identical despite different names*

### Comparing `nokey-0.4.0/nokey/developer_tools/apis_guru.py` & `nokey-0.5.0/nokey/developer_tools/apis_guru.py`

 * *Files identical despite different names*

### Comparing `nokey-0.4.0/nokey/developer_tools/filter_lists.py` & `nokey-0.5.0/nokey/developer_tools/filter_lists.py`

 * *Files identical despite different names*

### Comparing `nokey-0.4.0/nokey/developer_tools/microlink.py` & `nokey-0.5.0/nokey/developer_tools/microlink.py`

 * *Files identical despite different names*

### Comparing `nokey-0.4.0/nokey/developer_tools/url_haus.py` & `nokey-0.5.0/nokey/developer_tools/url_haus.py`

 * *Files identical despite different names*

### Comparing `nokey-0.4.0/nokey/developer_tools/url_shortener.py` & `nokey-0.5.0/nokey/developer_tools/url_shortener.py`

 * *Files identical despite different names*

### Comparing `nokey-0.4.0/nokey/education/university_domains_and_names.py` & `nokey-0.5.0/nokey/education/university_domains_and_names.py`

 * *Files identical despite different names*

### Comparing `nokey-0.4.0/nokey/finance_and_crypto/coinmap.py` & `nokey-0.5.0/nokey/finance_and_crypto/coinmap.py`

 * *Files identical despite different names*

### Comparing `nokey-0.4.0/nokey/finance_and_crypto/exchange_api.py` & `nokey-0.5.0/nokey/finance_and_crypto/exchange_api.py`

 * *Files identical despite different names*

### Comparing `nokey-0.4.0/nokey/finance_and_crypto/wall_street_bets.py` & `nokey-0.5.0/nokey/finance_and_crypto/wall_street_bets.py`

 * *Files identical despite different names*

### Comparing `nokey-0.4.0/nokey/food/fruityvice.py` & `nokey-0.5.0/nokey/food/fruityvice.py`

 * *Files identical despite different names*

### Comparing `nokey-0.4.0/nokey/games/free_to_game.py` & `nokey-0.5.0/nokey/games/free_to_game.py`

 * *Files identical despite different names*

### Comparing `nokey-0.4.0/nokey/games/open_trivia_db.py` & `nokey-0.5.0/nokey/games/open_trivia_db.py`

 * *Files identical despite different names*

### Comparing `nokey-0.4.0/nokey/geolocation/ip_api.py` & `nokey-0.5.0/nokey/geolocation/ip_api.py`

 * *Files identical despite different names*

### Comparing `nokey-0.4.0/nokey/geolocation/zippopotamus.py` & `nokey-0.5.0/nokey/geolocation/zippopotamus.py`

 * *Files identical despite different names*

### Comparing `nokey-0.4.0/nokey/government/federal_register.py` & `nokey-0.5.0/nokey/government/federal_register.py`

 * *Files identical despite different names*

### Comparing `nokey-0.4.0/nokey/government/usa_spending.py` & `nokey-0.5.0/nokey/government/usa_spending.py`

 * *Files identical despite different names*

### Comparing `nokey-0.4.0/nokey/helperFuncs/get_api_list.py` & `nokey-0.5.0/nokey/helperFuncs/get_api_list.py`

 * *Files identical despite different names*

### Comparing `nokey-0.4.0/nokey/helperFuncs/make_request.py` & `nokey-0.5.0/nokey/helperFuncs/make_request.py`

 * *Files identical despite different names*

### Comparing `nokey-0.4.0/nokey/helperFuncs/nokey_apis.py` & `nokey-0.5.0/nokey/helperFuncs/nokey_apis.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,11 +13,11 @@
     "developer_tools": ["URL Shortener", "URLHaus", "APIsGuru", "Microlink", "FilterLists"],
     "inspiration": ["Dictum"],
     "language": ["Free Dictionary"],
     "games": ["Free To Game", "Open Trivia Database"],
     "activities": ["Bored API"],
     "calendar": ["Nager.Date"],
     "government": ["Federal Register", "USA Spending"],
-    "art_and_images": ["Lorem Picsum"],
+    "art_and_images": ["Lorem Picsum", "Art Institute of Chicago"],
     "tv_and_film": ["Star Trek API"],
     "books": ["Gutendex"]
 }
```

### Comparing `nokey-0.4.0/nokey/inspiration/dictum.py` & `nokey-0.5.0/nokey/inspiration/dictum.py`

 * *Files identical despite different names*

### Comparing `nokey-0.4.0/nokey/jokes/joke_api.py` & `nokey-0.5.0/nokey/jokes/joke_api.py`

 * *Files identical despite different names*

### Comparing `nokey-0.4.0/nokey/language/free_dictionary.py` & `nokey-0.5.0/nokey/language/free_dictionary.py`

 * *Files identical despite different names*

### Comparing `nokey-0.4.0/nokey/random/random_user.py` & `nokey-0.5.0/nokey/random/random_user.py`

 * *Files identical despite different names*

### Comparing `nokey-0.4.0/nokey/science_and_nature/integrated_taxonomic_information_system.py` & `nokey-0.5.0/nokey/science_and_nature/integrated_taxonomic_information_system.py`

 * *Files identical despite different names*

### Comparing `nokey-0.4.0/nokey/science_and_nature/nobel_prize.py` & `nokey-0.5.0/nokey/science_and_nature/nobel_prize.py`

 * *Files identical despite different names*

### Comparing `nokey-0.4.0/nokey/spaceflight/spaceflight_news.py` & `nokey-0.5.0/nokey/spaceflight/spaceflight_news.py`

 * *Files identical despite different names*

### Comparing `nokey-0.4.0/nokey/tv_and_film/star_trek_api.py` & `nokey-0.5.0/nokey/tv_and_film/star_trek_api.py`

 * *Files identical despite different names*

### Comparing `nokey-0.4.0/nokey/weather/national_weather_service.py` & `nokey-0.5.0/nokey/weather/national_weather_service.py`

 * *Files identical despite different names*

### Comparing `nokey-0.4.0/nokey.egg-info/PKG-INFO` & `nokey-0.5.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,29 @@
 Metadata-Version: 2.1
 Name: nokey
-Version: 0.4.0
+Version: 0.5.0
 Summary: A python package for accessing APIs that require no key.
-Author-email: Spyder Rex <billyjohnsonauthor@gmail.com>
-Project-URL: Homepage, https://github.com/SpyderRex/nokey
-Project-URL: Issues, https://github.com/Spyder/nokey/issues
-Classifier: Programming Language :: Python :: 3
+Home-page: https://github.com/SpyderRex/nokey
+License: MIT
+Keywords: API,requests,xmltodict
+Author: Spyder Rex
+Author-email: billyjohnsonauthor@gmail.com
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: requests (>=2.26.0,<3.0.0)
+Requires-Dist: xmltodict (==0.13.0)
+Project-URL: Repository, https://github.com/SpyderRex/nokey
 Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: requests
-Requires-Dist: xmltodict==0.13.0
 
 # nokey - Access APIs without a Key
 
 nokey is a Python package designed to provide easy access to various APIs that do not require an API key for authentication. This project aims to simplify the process of interacting with different APIs by offering a unified interface for accessing them, all within a single Python package.
 
 ## Features
 
@@ -141,18 +148,24 @@
 
 ## tv_and_film
 Star Trek API
 
 ## books_and_literature
 Gutendex
 
+## art_and_images
+Lorum Picsum
+
+Art Institute of Chicago
+
 # Future Roadmap
 As the project grows, we envision expanding the collection of keyless APIs to cover a wide range of categories. Your feedback and contributions will play a crucial role in shaping the future of nokey.
 
 # License
 This project is licensed under the MIT License - see the LICENSE file for details.
 
 # Documentation
 Check out the [docs](https://nokey.readthedocs.io/en/latest/).
 
 # Disclaimer:
 Be sure to read the API documentation if you plan to use any of the APIs for development. This package is for accessing keyless, free, open source APIs and I am not responsible for the content of the APIs themselves.
+
```

