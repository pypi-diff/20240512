# Comparing `tmp/sphinxcontrib_confluencebuilder-2.5.1.tar.gz` & `tmp/sphinxcontrib_confluencebuilder-2.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinxcontrib_confluencebuilder-2.5.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "sphinxcontrib_confluencebuilder-2.5.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `sphinxcontrib_confluencebuilder-2.5.1.tar` & `sphinxcontrib_confluencebuilder-2.5.2.tar`

### file list

```diff
@@ -1,156 +1,156 @@
--rw-r--r--   0        0        0     1540 2024-04-06 20:22:16.495082 sphinxcontrib_confluencebuilder-2.5.1/AUTHORS
--rw-r--r--   0        0        0     1340 2024-04-06 20:22:16.495082 sphinxcontrib_confluencebuilder-2.5.1/LICENSE
--rw-r--r--   0        0        0     1617 2024-04-06 20:22:16.495082 sphinxcontrib_confluencebuilder-2.5.1/LICENSE-3RD-PARTY
--rw-r--r--   0        0        0      143 2024-04-06 20:22:16.495082 sphinxcontrib_confluencebuilder-2.5.1/MANIFEST.in
--rw-r--r--   0        0        0     3660 2024-04-06 20:22:16.495082 sphinxcontrib_confluencebuilder-2.5.1/README.md
--rw-r--r--   0        0        0     1790 2024-04-06 20:22:16.499081 sphinxcontrib_confluencebuilder-2.5.1/pyproject.toml
--rw-r--r--   0        0        0    20337 2024-04-06 20:22:16.499081 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/__init__.py
--rw-r--r--   0        0        0     3878 2024-04-06 20:22:16.499081 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/__main__.py
--rw-r--r--   0        0        0    14226 2024-04-06 20:22:16.499081 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/assets.py
--rw-r--r--   0        0        0    50952 2024-04-06 20:22:16.499081 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/builder.py
--rw-r--r--   0        0        0        0 2024-04-06 20:22:16.499081 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/cmd/__init__.py
--rw-r--r--   0        0        0     2363 2024-04-06 20:22:16.499081 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/cmd/build.py
--rw-r--r--   0        0        0    15782 2024-04-06 20:22:16.499081 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/cmd/conntest.py
--rw-r--r--   0        0        0    11304 2024-04-06 20:22:16.499081 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/cmd/report.py
--rw-r--r--   0        0        0     6495 2024-04-06 20:22:16.499081 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/cmd/wipe.py
--rw-r--r--   0        0        0     2396 2024-04-06 20:22:16.499081 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/compat.py
--rw-r--r--   0        0        0     2897 2024-04-06 20:22:16.499081 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/config/__init__.py
--rw-r--r--   0        0        0    27153 2024-04-06 20:22:16.503081 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/config/checks.py
--rw-r--r--   0        0        0     6066 2024-04-06 20:22:16.503081 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/config/defaults.py
--rw-r--r--   0        0        0     2604 2024-04-06 20:22:16.503081 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/config/env.py
--rw-r--r--   0        0        0    11061 2024-04-06 20:22:16.503081 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/config/exceptions.py
--rw-r--r--   0        0        0     3446 2024-04-06 20:22:16.503081 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/config/manager.py
--rw-r--r--   0        0        0     4937 2024-04-06 20:22:16.503081 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/config/notifications.py
--rw-r--r--   0        0        0    16619 2024-04-06 20:22:16.503081 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/config/validation.py
--rw-r--r--   0        0        0     1007 2024-04-06 20:22:16.503081 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/debug.py
--rw-r--r--   0        0        0    11794 2024-04-06 20:22:16.503081 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/directives.py
--rw-r--r--   0        0        0     7713 2024-04-06 20:22:16.503081 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/env.py
--rw-r--r--   0        0        0     9773 2024-04-06 20:22:16.503081 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/exceptions.py
--rw-r--r--   0        0        0     2929 2024-04-06 20:22:16.503081 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/intersphinx.py
--rw-r--r--   0        0        0      419 2024-04-06 20:22:16.503081 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/__init__.py
--rw-r--r--   0        0        0      590 2024-04-06 20:22:16.503081 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/ar/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1352 2024-04-06 20:22:16.503081 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/ar/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      533 2024-04-06 20:22:16.503081 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/bg/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1295 2024-04-06 20:22:16.503081 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/bg/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      458 2024-04-06 20:22:16.503081 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/bn/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1249 2024-04-06 20:22:16.503081 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/bn/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      500 2024-04-06 20:22:16.503081 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/ca/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1262 2024-04-06 20:22:16.503081 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/ca/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      526 2024-04-06 20:22:16.503081 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/cs/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1288 2024-04-06 20:22:16.503081 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/cs/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      579 2024-04-06 20:22:16.503081 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/cy/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1341 2024-04-06 20:22:16.503081 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/cy/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      499 2024-04-06 20:22:16.503081 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/da/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1261 2024-04-06 20:22:16.503081 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/da/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      503 2024-04-06 20:22:16.503081 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/de/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1265 2024-04-06 20:22:16.503081 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/de/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      518 2024-04-06 20:22:16.503081 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/el/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1280 2024-04-06 20:22:16.503081 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/el/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      460 2024-04-06 20:22:16.503081 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/eo/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1265 2024-04-06 20:22:16.503081 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/eo/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      458 2024-04-06 20:22:16.503081 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/es/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1252 2024-04-06 20:22:16.503081 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/es/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      505 2024-04-06 20:22:16.503081 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/et/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1267 2024-04-06 20:22:16.503081 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/et/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      500 2024-04-06 20:22:16.503081 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/eu/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1262 2024-04-06 20:22:16.503081 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/eu/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      505 2024-04-06 20:22:16.503081 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/fi/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1267 2024-04-06 20:22:16.503081 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/fi/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      503 2024-04-06 20:22:16.503081 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/fr/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1265 2024-04-06 20:22:16.503081 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/fr/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      507 2024-04-06 20:22:16.503081 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/he/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1298 2024-04-06 20:22:16.503081 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/he/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      535 2024-04-06 20:22:16.503081 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/hi/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1297 2024-04-06 20:22:16.503081 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/hi/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      573 2024-04-06 20:22:16.503081 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/hr/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1335 2024-04-06 20:22:16.503081 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/hr/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      510 2024-04-06 20:22:16.503081 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/hu/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1272 2024-04-06 20:22:16.503081 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/hu/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      497 2024-04-06 20:22:16.503081 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/id/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1259 2024-04-06 20:22:16.503081 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/id/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      458 2024-04-06 20:22:16.503081 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/it/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1249 2024-04-06 20:22:16.503081 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/it/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      499 2024-04-06 20:22:16.503081 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/ja/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1261 2024-04-06 20:22:16.503081 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/ja/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      492 2024-04-06 20:22:16.503081 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/ko/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1254 2024-04-06 20:22:16.503081 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/ko/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      609 2024-04-06 20:22:16.503081 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/lt/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1371 2024-04-06 20:22:16.503081 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/lt/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      535 2024-04-06 20:22:16.503081 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/lv/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1297 2024-04-06 20:22:16.503081 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/lv/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      535 2024-04-06 20:22:16.503081 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/mk/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1297 2024-04-06 20:22:16.503081 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/mk/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      509 2024-04-06 20:22:16.507082 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/nb/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1271 2024-04-06 20:22:16.507082 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/nb/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      551 2024-04-06 20:22:16.507082 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/ne/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1316 2024-04-06 20:22:16.507082 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/ne/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      498 2024-04-06 20:22:16.507082 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/nl/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1260 2024-04-06 20:22:16.507082 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/nl/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      648 2024-04-06 20:22:16.507082 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/pl/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1410 2024-04-06 20:22:16.507082 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/pl/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      513 2024-04-06 20:22:16.507082 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/pt_BR/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1278 2024-04-06 20:22:16.507082 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/pt_BR/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      546 2024-04-06 20:22:16.507082 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/ro/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1308 2024-04-06 20:22:16.507082 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/ro/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      623 2024-04-06 20:22:16.507082 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/ru/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1414 2024-04-06 20:22:16.507082 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/ru/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      458 2024-04-06 20:22:16.507082 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/si/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1252 2024-04-06 20:22:16.507082 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/si/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      527 2024-04-06 20:22:16.507082 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/sk/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1289 2024-04-06 20:22:16.507082 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/sk/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      512 2024-04-06 20:22:16.507082 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/sl/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1303 2024-04-06 20:22:16.507082 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/sl/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      871 2024-04-06 20:22:16.507082 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/sphinxcontrib.confluencebuilder.pot
--rw-r--r--   0        0        0      511 2024-04-06 20:22:16.507082 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/sq/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1273 2024-04-06 20:22:16.507082 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/sq/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      540 2024-04-06 20:22:16.507082 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/sr_CS/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1334 2024-04-06 20:22:16.507082 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/sr_CS/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      502 2024-04-06 20:22:16.507082 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/sv/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1267 2024-04-06 20:22:16.507082 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/sv/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      546 2024-04-06 20:22:16.507082 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/ta/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1308 2024-04-06 20:22:16.507082 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/ta/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      538 2024-04-06 20:22:16.507082 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/te/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1300 2024-04-06 20:22:16.507082 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/te/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      505 2024-04-06 20:22:16.507082 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/tr/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1267 2024-04-06 20:22:16.507082 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/tr/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      689 2024-04-06 20:22:16.507082 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/uk/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1451 2024-04-06 20:22:16.507082 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/uk/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      496 2024-04-06 20:22:16.507082 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/vi/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1258 2024-04-06 20:22:16.507082 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/vi/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      504 2024-04-06 20:22:16.507082 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/zh_TW/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1269 2024-04-06 20:22:16.507082 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/zh_TW/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0     4510 2024-04-06 20:22:16.507082 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/logger.py
--rw-r--r--   0        0        0     6595 2024-04-06 20:22:16.507082 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/nodes.py
--rw-r--r--   0        0        0    64600 2024-04-06 20:22:16.507082 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/publisher.py
--rw-r--r--   0        0        0      417 2024-04-06 20:22:16.507082 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/reportbuilder.py
--rw-r--r--   0        0        0    15261 2024-04-06 20:22:16.507082 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/rest.py
--rw-r--r--   0        0        0     7561 2024-04-06 20:22:16.507082 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/roles.py
--rw-r--r--   0        0        0    11519 2024-04-06 20:22:16.507082 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/singlebuilder.py
--rw-r--r--   0        0        0     9241 2024-04-06 20:22:16.507082 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/state.py
--rw-r--r--   0        0        0        0 2024-04-06 20:22:16.507082 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/std/__init__.py
--rw-r--r--   0        0        0    13507 2024-04-06 20:22:16.507082 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/std/confluence.py
--rw-r--r--   0        0        0      310 2024-04-06 20:22:16.507082 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/std/sphinx.py
--rw-r--r--   0        0        0     1968 2024-04-06 20:22:16.507082 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/storage/__init__.py
--rw-r--r--   0        0        0     4699 2024-04-06 20:22:16.507082 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/storage/index.py
--rw-r--r--   0        0        0     1434 2024-04-06 20:22:16.507082 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/storage/search.py
--rw-r--r--   0        0        0        0 2024-04-06 20:22:16.507082 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/storage/templates/__init__.py
--rw-r--r--   0        0        0     1871 2024-04-06 20:22:16.507082 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/storage/templates/domainindex.html
--rw-r--r--   0        0        0     1715 2024-04-06 20:22:16.507082 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/storage/templates/domainindex_v2.html
--rw-r--r--   0        0        0     2262 2024-04-06 20:22:16.507082 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/storage/templates/genindex.html
--rw-r--r--   0        0        0     2382 2024-04-06 20:22:16.507082 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/storage/templates/genindex_v2.html
--rw-r--r--   0        0        0      932 2024-04-06 20:22:16.507082 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/storage/templates/search.html
--rw-r--r--   0        0        0      988 2024-04-06 20:22:16.507082 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/storage/templates/search_v2.html
--rw-r--r--   0        0        0   140100 2024-04-06 20:22:16.511082 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/storage/translator.py
--rw-r--r--   0        0        0     7326 2024-04-06 20:22:16.511082 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/svg.py
--rw-r--r--   0        0        0     2099 2024-04-06 20:22:16.511082 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/transform.py
--rw-r--r--   0        0        0    17387 2024-04-06 20:22:16.511082 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/translator.py
--rw-r--r--   0        0        0    11723 2024-04-06 20:22:16.511082 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/transmute/__init__.py
--rw-r--r--   0        0        0     1858 2024-04-06 20:22:16.511082 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/transmute/ext_jupyter_sphinx.py
--rw-r--r--   0        0        0     1691 2024-04-06 20:22:16.511082 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/transmute/ext_nbsphinx.py
--rw-r--r--   0        0        0     2462 2024-04-06 20:22:16.511082 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/transmute/ext_sphinx_diagrams.py
--rw-r--r--   0        0        0     1509 2024-04-06 20:22:16.511082 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/transmute/ext_sphinx_gallery.py
--rw-r--r--   0        0        0     4173 2024-04-06 20:22:16.511082 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/transmute/ext_sphinx_toolbox.py
--rw-r--r--   0        0        0     2449 2024-04-06 20:22:16.511082 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/transmute/ext_sphinxcontrib_mermaid.py
--rw-r--r--   0        0        0    11927 2024-04-06 20:22:16.511082 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/util.py
--rw-r--r--   0        0        0      638 2024-04-06 20:22:16.511082 sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/writer.py
--rw-r--r--   0        0        0     5143 1970-01-01 00:00:00.000000 sphinxcontrib_confluencebuilder-2.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1540 2024-05-12 17:42:29.835533 sphinxcontrib_confluencebuilder-2.5.2/AUTHORS
+-rw-r--r--   0        0        0     1340 2024-05-12 17:42:29.835533 sphinxcontrib_confluencebuilder-2.5.2/LICENSE
+-rw-r--r--   0        0        0     1617 2024-05-12 17:42:29.835533 sphinxcontrib_confluencebuilder-2.5.2/LICENSE-3RD-PARTY
+-rw-r--r--   0        0        0      143 2024-05-12 17:42:29.835533 sphinxcontrib_confluencebuilder-2.5.2/MANIFEST.in
+-rw-r--r--   0        0        0     3660 2024-05-12 17:42:29.835533 sphinxcontrib_confluencebuilder-2.5.2/README.md
+-rw-r--r--   0        0        0     1790 2024-05-12 17:42:29.839533 sphinxcontrib_confluencebuilder-2.5.2/pyproject.toml
+-rw-r--r--   0        0        0    20337 2024-05-12 17:42:29.839533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/__init__.py
+-rw-r--r--   0        0        0     3878 2024-05-12 17:42:29.839533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/__main__.py
+-rw-r--r--   0        0        0    14226 2024-05-12 17:42:29.839533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/assets.py
+-rw-r--r--   0        0        0    50952 2024-05-12 17:42:29.839533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/builder.py
+-rw-r--r--   0        0        0        0 2024-05-12 17:42:29.839533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/cmd/__init__.py
+-rw-r--r--   0        0        0     2363 2024-05-12 17:42:29.839533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/cmd/build.py
+-rw-r--r--   0        0        0    15782 2024-05-12 17:42:29.839533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/cmd/conntest.py
+-rw-r--r--   0        0        0    11304 2024-05-12 17:42:29.839533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/cmd/report.py
+-rw-r--r--   0        0        0     6495 2024-05-12 17:42:29.839533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/cmd/wipe.py
+-rw-r--r--   0        0        0     2396 2024-05-12 17:42:29.839533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/compat.py
+-rw-r--r--   0        0        0     2897 2024-05-12 17:42:29.839533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/config/__init__.py
+-rw-r--r--   0        0        0    27153 2024-05-12 17:42:29.839533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/config/checks.py
+-rw-r--r--   0        0        0     6066 2024-05-12 17:42:29.839533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/config/defaults.py
+-rw-r--r--   0        0        0     2604 2024-05-12 17:42:29.839533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/config/env.py
+-rw-r--r--   0        0        0    11061 2024-05-12 17:42:29.843533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/config/exceptions.py
+-rw-r--r--   0        0        0     3446 2024-05-12 17:42:29.843533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/config/manager.py
+-rw-r--r--   0        0        0     4937 2024-05-12 17:42:29.843533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/config/notifications.py
+-rw-r--r--   0        0        0    16619 2024-05-12 17:42:29.843533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/config/validation.py
+-rw-r--r--   0        0        0     1007 2024-05-12 17:42:29.843533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/debug.py
+-rw-r--r--   0        0        0    11794 2024-05-12 17:42:29.843533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/directives.py
+-rw-r--r--   0        0        0     7713 2024-05-12 17:42:29.843533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/env.py
+-rw-r--r--   0        0        0     9773 2024-05-12 17:42:29.843533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/exceptions.py
+-rw-r--r--   0        0        0     2929 2024-05-12 17:42:29.843533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/intersphinx.py
+-rw-r--r--   0        0        0      419 2024-05-12 17:42:29.843533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/__init__.py
+-rw-r--r--   0        0        0      590 2024-05-12 17:42:29.843533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/ar/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1352 2024-05-12 17:42:29.843533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/ar/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      533 2024-05-12 17:42:29.843533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/bg/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1295 2024-05-12 17:42:29.843533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/bg/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      458 2024-05-12 17:42:29.843533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/bn/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1249 2024-05-12 17:42:29.843533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/bn/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      500 2024-05-12 17:42:29.843533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/ca/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1262 2024-05-12 17:42:29.843533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/ca/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      526 2024-05-12 17:42:29.843533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/cs/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1288 2024-05-12 17:42:29.843533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/cs/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      579 2024-05-12 17:42:29.843533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/cy/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1341 2024-05-12 17:42:29.843533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/cy/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      499 2024-05-12 17:42:29.843533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/da/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1261 2024-05-12 17:42:29.843533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/da/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      503 2024-05-12 17:42:29.843533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/de/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1265 2024-05-12 17:42:29.843533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/de/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      518 2024-05-12 17:42:29.843533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/el/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1280 2024-05-12 17:42:29.843533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/el/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      460 2024-05-12 17:42:29.843533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/eo/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1265 2024-05-12 17:42:29.843533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/eo/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      458 2024-05-12 17:42:29.843533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/es/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1252 2024-05-12 17:42:29.843533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/es/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      505 2024-05-12 17:42:29.843533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/et/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1267 2024-05-12 17:42:29.843533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/et/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      500 2024-05-12 17:42:29.843533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/eu/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1262 2024-05-12 17:42:29.843533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/eu/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      505 2024-05-12 17:42:29.843533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/fi/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1267 2024-05-12 17:42:29.843533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/fi/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      503 2024-05-12 17:42:29.843533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/fr/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1265 2024-05-12 17:42:29.843533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/fr/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      507 2024-05-12 17:42:29.843533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/he/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1298 2024-05-12 17:42:29.843533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/he/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      535 2024-05-12 17:42:29.843533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/hi/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1297 2024-05-12 17:42:29.843533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/hi/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      573 2024-05-12 17:42:29.843533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/hr/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1335 2024-05-12 17:42:29.843533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/hr/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      510 2024-05-12 17:42:29.843533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/hu/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1272 2024-05-12 17:42:29.843533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/hu/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      497 2024-05-12 17:42:29.843533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/id/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1259 2024-05-12 17:42:29.843533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/id/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      458 2024-05-12 17:42:29.843533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/it/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1249 2024-05-12 17:42:29.843533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/it/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      499 2024-05-12 17:42:29.843533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/ja/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1261 2024-05-12 17:42:29.843533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/ja/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      492 2024-05-12 17:42:29.843533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/ko/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1254 2024-05-12 17:42:29.843533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/ko/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      609 2024-05-12 17:42:29.843533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/lt/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1371 2024-05-12 17:42:29.843533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/lt/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      535 2024-05-12 17:42:29.843533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/lv/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1297 2024-05-12 17:42:29.843533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/lv/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      535 2024-05-12 17:42:29.843533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/mk/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1297 2024-05-12 17:42:29.843533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/mk/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      509 2024-05-12 17:42:29.843533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/nb/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1271 2024-05-12 17:42:29.843533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/nb/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      551 2024-05-12 17:42:29.847533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/ne/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1316 2024-05-12 17:42:29.847533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/ne/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      498 2024-05-12 17:42:29.847533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/nl/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1260 2024-05-12 17:42:29.847533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/nl/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      648 2024-05-12 17:42:29.847533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/pl/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1410 2024-05-12 17:42:29.847533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/pl/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      513 2024-05-12 17:42:29.847533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/pt_BR/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1278 2024-05-12 17:42:29.847533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/pt_BR/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      546 2024-05-12 17:42:29.847533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/ro/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1308 2024-05-12 17:42:29.847533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/ro/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      623 2024-05-12 17:42:29.847533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/ru/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1414 2024-05-12 17:42:29.847533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/ru/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      458 2024-05-12 17:42:29.847533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/si/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1252 2024-05-12 17:42:29.847533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/si/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      527 2024-05-12 17:42:29.847533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/sk/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1289 2024-05-12 17:42:29.847533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/sk/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      512 2024-05-12 17:42:29.847533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/sl/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1303 2024-05-12 17:42:29.847533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/sl/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      871 2024-05-12 17:42:29.847533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/sphinxcontrib.confluencebuilder.pot
+-rw-r--r--   0        0        0      511 2024-05-12 17:42:29.847533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/sq/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1273 2024-05-12 17:42:29.847533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/sq/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      540 2024-05-12 17:42:29.847533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/sr_CS/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1334 2024-05-12 17:42:29.847533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/sr_CS/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      502 2024-05-12 17:42:29.847533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/sv/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1267 2024-05-12 17:42:29.847533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/sv/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      546 2024-05-12 17:42:29.847533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/ta/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1308 2024-05-12 17:42:29.847533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/ta/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      538 2024-05-12 17:42:29.847533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/te/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1300 2024-05-12 17:42:29.847533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/te/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      505 2024-05-12 17:42:29.847533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/tr/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1267 2024-05-12 17:42:29.847533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/tr/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      689 2024-05-12 17:42:29.847533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/uk/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1451 2024-05-12 17:42:29.847533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/uk/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      496 2024-05-12 17:42:29.847533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/vi/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1258 2024-05-12 17:42:29.847533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/vi/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      504 2024-05-12 17:42:29.847533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/zh_TW/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1269 2024-05-12 17:42:29.847533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/zh_TW/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0     4510 2024-05-12 17:42:29.847533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/logger.py
+-rw-r--r--   0        0        0     6595 2024-05-12 17:42:29.847533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/nodes.py
+-rw-r--r--   0        0        0    64596 2024-05-12 17:42:29.847533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/publisher.py
+-rw-r--r--   0        0        0      417 2024-05-12 17:42:29.847533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/reportbuilder.py
+-rw-r--r--   0        0        0    15261 2024-05-12 17:42:29.847533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/rest.py
+-rw-r--r--   0        0        0     7561 2024-05-12 17:42:29.847533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/roles.py
+-rw-r--r--   0        0        0    11519 2024-05-12 17:42:29.847533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/singlebuilder.py
+-rw-r--r--   0        0        0     9241 2024-05-12 17:42:29.847533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/state.py
+-rw-r--r--   0        0        0        0 2024-05-12 17:42:29.847533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/std/__init__.py
+-rw-r--r--   0        0        0    13507 2024-05-12 17:42:29.847533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/std/confluence.py
+-rw-r--r--   0        0        0      310 2024-05-12 17:42:29.847533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/std/sphinx.py
+-rw-r--r--   0        0        0     1968 2024-05-12 17:42:29.847533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/storage/__init__.py
+-rw-r--r--   0        0        0     4699 2024-05-12 17:42:29.847533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/storage/index.py
+-rw-r--r--   0        0        0     1434 2024-05-12 17:42:29.847533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/storage/search.py
+-rw-r--r--   0        0        0        0 2024-05-12 17:42:29.847533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/storage/templates/__init__.py
+-rw-r--r--   0        0        0     1871 2024-05-12 17:42:29.847533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/storage/templates/domainindex.html
+-rw-r--r--   0        0        0     1715 2024-05-12 17:42:29.847533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/storage/templates/domainindex_v2.html
+-rw-r--r--   0        0        0     2262 2024-05-12 17:42:29.847533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/storage/templates/genindex.html
+-rw-r--r--   0        0        0     2382 2024-05-12 17:42:29.847533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/storage/templates/genindex_v2.html
+-rw-r--r--   0        0        0      932 2024-05-12 17:42:29.847533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/storage/templates/search.html
+-rw-r--r--   0        0        0      988 2024-05-12 17:42:29.847533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/storage/templates/search_v2.html
+-rw-r--r--   0        0        0   140100 2024-05-12 17:42:29.851533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/storage/translator.py
+-rw-r--r--   0        0        0     7326 2024-05-12 17:42:29.851533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/svg.py
+-rw-r--r--   0        0        0     2099 2024-05-12 17:42:29.851533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/transform.py
+-rw-r--r--   0        0        0    17387 2024-05-12 17:42:29.851533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/translator.py
+-rw-r--r--   0        0        0    11723 2024-05-12 17:42:29.851533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/transmute/__init__.py
+-rw-r--r--   0        0        0     1858 2024-05-12 17:42:29.851533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/transmute/ext_jupyter_sphinx.py
+-rw-r--r--   0        0        0     1691 2024-05-12 17:42:29.851533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/transmute/ext_nbsphinx.py
+-rw-r--r--   0        0        0     2462 2024-05-12 17:42:29.851533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/transmute/ext_sphinx_diagrams.py
+-rw-r--r--   0        0        0     1509 2024-05-12 17:42:29.851533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/transmute/ext_sphinx_gallery.py
+-rw-r--r--   0        0        0     4173 2024-05-12 17:42:29.851533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/transmute/ext_sphinx_toolbox.py
+-rw-r--r--   0        0        0     2449 2024-05-12 17:42:29.851533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/transmute/ext_sphinxcontrib_mermaid.py
+-rw-r--r--   0        0        0    11927 2024-05-12 17:42:29.851533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/util.py
+-rw-r--r--   0        0        0      638 2024-05-12 17:42:29.851533 sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/writer.py
+-rw-r--r--   0        0        0     5143 1970-01-01 00:00:00.000000 sphinxcontrib_confluencebuilder-2.5.2/PKG-INFO
```

### Comparing `sphinxcontrib_confluencebuilder-2.5.1/AUTHORS` & `sphinxcontrib_confluencebuilder-2.5.2/AUTHORS`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.5.1/LICENSE` & `sphinxcontrib_confluencebuilder-2.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.5.1/LICENSE-3RD-PARTY` & `sphinxcontrib_confluencebuilder-2.5.2/LICENSE-3RD-PARTY`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.5.1/README.md` & `sphinxcontrib_confluencebuilder-2.5.2/README.md`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.5.1/pyproject.toml` & `sphinxcontrib_confluencebuilder-2.5.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/__init__.py` & `sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
 # load imgmath extension if available to handle math configuration options
 try:
     from sphinx.ext import imgmath
 except ImportError:
     imgmath = None
 
-__version__ = '2.5.1'
+__version__ = '2.5.2'
 
 
 def setup(app):
     ConfluenceLogger.initialize()
     cm = app.config_manager_ = ConfigManager(app)
 
     app.require_sphinx('6.1')
```

### Comparing `sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/__main__.py` & `sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/__main__.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/assets.py` & `sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/assets.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/builder.py` & `sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/builder.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/cmd/build.py` & `sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/cmd/build.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/cmd/conntest.py` & `sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/cmd/conntest.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/cmd/report.py` & `sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/cmd/report.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/cmd/wipe.py` & `sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/cmd/wipe.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/compat.py` & `sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/compat.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/config/__init__.py` & `sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/config/__init__.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/config/checks.py` & `sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/config/checks.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/config/defaults.py` & `sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/config/defaults.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/config/env.py` & `sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/config/env.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/config/exceptions.py` & `sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/config/exceptions.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/config/manager.py` & `sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/config/manager.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/config/notifications.py` & `sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/config/notifications.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/config/validation.py` & `sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/config/validation.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/debug.py` & `sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/debug.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/directives.py` & `sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/directives.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/env.py` & `sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/env.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/exceptions.py` & `sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/exceptions.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/intersphinx.py` & `sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/intersphinx.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/ar/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo` & `sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/ar/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/ar/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/ar/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/bg/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo` & `sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/bg/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/bg/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/bg/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/bn/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/bn/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/ca/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/ca/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/cs/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo` & `sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/cs/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/cs/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/cs/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/cy/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo` & `sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/cy/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/cy/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/cy/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/da/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/da/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/de/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/de/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/el/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo` & `sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/el/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/el/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/el/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/eo/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/eo/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/es/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/es/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/et/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/et/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/eu/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/eu/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/fi/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/fi/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/fr/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/fr/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/he/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/he/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/hi/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo` & `sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/hi/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/hi/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/hi/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/hr/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo` & `sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/hr/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/hr/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/hr/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/hu/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/hu/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/id/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/id/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/it/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/it/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/ja/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/ja/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/ko/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/ko/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/lt/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo` & `sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/lt/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/lt/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/lt/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/lv/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo` & `sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/lv/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/lv/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/lv/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/mk/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo` & `sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/mk/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/mk/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/mk/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/nb/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/nb/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/ne/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo` & `sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/ne/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/ne/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/ne/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/nl/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/nl/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/pl/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo` & `sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/pl/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/pl/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/pl/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/pt_BR/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo` & `sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/pt_BR/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/pt_BR/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/pt_BR/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/ro/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo` & `sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/ro/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/ro/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/ro/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/ru/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo` & `sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/ru/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/ru/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/ru/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/si/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/si/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/sk/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo` & `sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/sk/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/sk/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/sk/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/sl/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo` & `sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/sl/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/sl/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/sl/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/sphinxcontrib.confluencebuilder.pot` & `sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/sphinxcontrib.confluencebuilder.pot`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/sq/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/sq/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/sr_CS/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo` & `sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/sr_CS/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/sr_CS/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/sr_CS/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/sv/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/sv/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/ta/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo` & `sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/ta/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/ta/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/ta/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/te/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo` & `sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/te/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/te/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/te/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/tr/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/tr/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/uk/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo` & `sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/uk/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/uk/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/uk/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/vi/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/vi/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/locale/zh_TW/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/locale/zh_TW/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/logger.py` & `sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/logger.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/nodes.py` & `sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/nodes.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/publisher.py` & `sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/publisher.py`

 * *Files 0% similar despite different names*

```diff
@@ -1514,16 +1514,16 @@
             update_page['ancestors'] = [{'id': '1'}]
 
         # if this is an api v2 mode, prepare any extra requests needed for
         # populating ancestors or metadata information
         pending_new_labels = []
         pending_prop_requests = []
         if self.api_mode == 'v2':
-            orig_metadata = page.get('metadata', None)
-            update_metadata = update_page.pop('metadata', None)
+            orig_metadata = page.get('metadata', {})
+            update_metadata = update_page.pop('metadata', {})
 
             # configure parent page for this page update
             #
             # For v2, we need to strip out `ancestors` and place it with an
             # expected `parentId` value.
             ancestors_request = update_page.pop('ancestors', None)
             if ancestors_request:
```

### Comparing `sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/rest.py` & `sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/rest.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/roles.py` & `sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/roles.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/singlebuilder.py` & `sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/singlebuilder.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/state.py` & `sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/state.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/std/confluence.py` & `sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/std/confluence.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/storage/__init__.py` & `sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/storage/index.py` & `sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/storage/index.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/storage/search.py` & `sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/storage/search.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/storage/templates/domainindex.html` & `sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/storage/templates/domainindex.html`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/storage/templates/domainindex_v2.html` & `sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/storage/templates/domainindex_v2.html`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/storage/templates/genindex.html` & `sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/storage/templates/genindex.html`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/storage/templates/genindex_v2.html` & `sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/storage/templates/genindex_v2.html`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/storage/templates/search.html` & `sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/storage/templates/search.html`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/storage/templates/search_v2.html` & `sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/storage/templates/search_v2.html`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/storage/translator.py` & `sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/storage/translator.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/svg.py` & `sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/svg.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/transform.py` & `sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/transform.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/translator.py` & `sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/translator.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/transmute/__init__.py` & `sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/transmute/__init__.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/transmute/ext_jupyter_sphinx.py` & `sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/transmute/ext_jupyter_sphinx.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/transmute/ext_nbsphinx.py` & `sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/transmute/ext_nbsphinx.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/transmute/ext_sphinx_diagrams.py` & `sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/transmute/ext_sphinx_diagrams.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/transmute/ext_sphinx_gallery.py` & `sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/transmute/ext_sphinx_gallery.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/transmute/ext_sphinx_toolbox.py` & `sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/transmute/ext_sphinx_toolbox.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/transmute/ext_sphinxcontrib_mermaid.py` & `sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/transmute/ext_sphinxcontrib_mermaid.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/util.py` & `sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/util.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.5.1/sphinxcontrib/confluencebuilder/writer.py` & `sphinxcontrib_confluencebuilder-2.5.2/sphinxcontrib/confluencebuilder/writer.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.5.1/PKG-INFO` & `sphinxcontrib_confluencebuilder-2.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinxcontrib-confluencebuilder
-Version: 2.5.1
+Version: 2.5.2
 Summary: Sphinx extension to build Atlassian Confluence Storage Markup
 Author-email: Anthony Shaw <anthonyshaw@apache.org>
 Maintainer-email: James Knight <james.d.knight@live.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

