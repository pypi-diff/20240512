# Comparing `tmp/adafruit_circuitpython_requests-3.2.8.tar.gz` & `tmp/adafruit_circuitpython_requests-3.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit_circuitpython_requests-3.2.8.tar", last modified: Sun Apr 28 21:52:30 2024, max compression
+gzip compressed data, was "adafruit_circuitpython_requests-3.2.9.tar", last modified: Sun May 12 19:50:14 2024, max compression
```

## Comparing `adafruit_circuitpython_requests-3.2.8.tar` & `adafruit_circuitpython_requests-3.2.9.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 21:52:30.648459 adafruit_circuitpython_requests-3.2.8/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 21:52:30.636459 adafruit_circuitpython_requests-3.2.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 21:52:30.636459 adafruit_circuitpython_requests-3.2.8/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-28 21:52:21.000000 adafruit_circuitpython_requests-3.2.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 21:52:30.640459 adafruit_circuitpython_requests-3.2.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-28 21:52:21.000000 adafruit_circuitpython_requests-3.2.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-28 21:52:21.000000 adafruit_circuitpython_requests-3.2.8/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-28 21:52:21.000000 adafruit_circuitpython_requests-3.2.8/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-28 21:52:21.000000 adafruit_circuitpython_requests-3.2.8/.github/workflows/release_pypi.yml
--rwxr-xr-x   0 runner    (1001) docker     (127)     1724 2024-04-28 21:52:21.000000 adafruit_circuitpython_requests-3.2.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-04-28 21:52:21.000000 adafruit_circuitpython_requests-3.2.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    13078 2024-04-28 21:52:21.000000 adafruit_circuitpython_requests-3.2.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-28 21:52:21.000000 adafruit_circuitpython_requests-3.2.8/.readthedocs.yaml
--rwxr-xr-x   0 runner    (1001) docker     (127)     6147 2024-04-28 21:52:21.000000 adafruit_circuitpython_requests-3.2.8/CODE_OF_CONDUCT.md
--rwxr-xr-x   0 runner    (1001) docker     (127)     1098 2024-04-28 21:52:21.000000 adafruit_circuitpython_requests-3.2.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 21:52:30.640459 adafruit_circuitpython_requests-3.2.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (127)    16814 2024-04-28 21:52:21.000000 adafruit_circuitpython_requests-3.2.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-28 21:52:21.000000 adafruit_circuitpython_requests-3.2.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-28 21:52:21.000000 adafruit_circuitpython_requests-3.2.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-04-28 21:52:30.648459 adafruit_circuitpython_requests-3.2.8/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)     2642 2024-04-28 21:52:21.000000 adafruit_circuitpython_requests-3.2.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-28 21:52:21.000000 adafruit_circuitpython_requests-3.2.8/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 21:52:30.648459 adafruit_circuitpython_requests-3.2.8/adafruit_circuitpython_requests.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-04-28 21:52:30.000000 adafruit_circuitpython_requests-3.2.8/adafruit_circuitpython_requests.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-04-28 21:52:30.000000 adafruit_circuitpython_requests-3.2.8/adafruit_circuitpython_requests.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 21:52:30.000000 adafruit_circuitpython_requests-3.2.8/adafruit_circuitpython_requests.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-28 21:52:30.000000 adafruit_circuitpython_requests-3.2.8/adafruit_circuitpython_requests.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-28 21:52:30.000000 adafruit_circuitpython_requests-3.2.8/adafruit_circuitpython_requests.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    21326 2024-04-28 21:52:28.000000 adafruit_circuitpython_requests-3.2.8/adafruit_requests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 21:52:30.640459 adafruit_circuitpython_requests-3.2.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 21:52:30.640459 adafruit_circuitpython_requests-3.2.8/docs/_static/
--rwxr-xr-x   0 runner    (1001) docker     (127)     4414 2024-04-28 21:52:21.000000 adafruit_circuitpython_requests-3.2.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-28 21:52:21.000000 adafruit_circuitpython_requests-3.2.8/docs/_static/favicon.ico.license
--rwxr-xr-x   0 runner    (1001) docker     (127)      267 2024-04-28 21:52:21.000000 adafruit_circuitpython_requests-3.2.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-28 21:52:21.000000 adafruit_circuitpython_requests-3.2.8/docs/api.rst.license
--rwxr-xr-x   0 runner    (1001) docker     (127)     5400 2024-04-28 21:52:21.000000 adafruit_circuitpython_requests-3.2.8/docs/conf.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      803 2024-04-28 21:52:21.000000 adafruit_circuitpython_requests-3.2.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-28 21:52:21.000000 adafruit_circuitpython_requests-3.2.8/docs/examples.rst.license
--rwxr-xr-x   0 runner    (1001) docker     (127)      973 2024-04-28 21:52:21.000000 adafruit_circuitpython_requests-3.2.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-28 21:52:21.000000 adafruit_circuitpython_requests-3.2.8/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-28 21:52:21.000000 adafruit_circuitpython_requests-3.2.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 21:52:30.636459 adafruit_circuitpython_requests-3.2.8/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 21:52:30.644459 adafruit_circuitpython_requests-3.2.8/examples/cpython/
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-28 21:52:28.000000 adafruit_circuitpython_requests-3.2.8/examples/cpython/requests_cpython_advanced.py
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-04-28 21:52:28.000000 adafruit_circuitpython_requests-3.2.8/examples/cpython/requests_cpython_simpletest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 21:52:30.644459 adafruit_circuitpython_requests-3.2.8/examples/esp32spi/
--rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-04-28 21:52:28.000000 adafruit_circuitpython_requests-3.2.8/examples/esp32spi/requests_esp32spi_advanced.py
--rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-04-28 21:52:28.000000 adafruit_circuitpython_requests-3.2.8/examples/esp32spi/requests_esp32spi_simpletest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 21:52:30.644459 adafruit_circuitpython_requests-3.2.8/examples/fona/
--rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-04-28 21:52:28.000000 adafruit_circuitpython_requests-3.2.8/examples/fona/requests_fona_advanced.py
--rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-04-28 21:52:28.000000 adafruit_circuitpython_requests-3.2.8/examples/fona/requests_fona_simpletest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 21:52:30.644459 adafruit_circuitpython_requests-3.2.8/examples/wifi/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 21:52:30.644459 adafruit_circuitpython_requests-3.2.8/examples/wifi/expanded/
--rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-04-28 21:52:28.000000 adafruit_circuitpython_requests-3.2.8/examples/wifi/expanded/requests_wifi_adafruit_discord_active_online.py
--rw-r--r--   0 runner    (1001) docker     (127)     3480 2024-04-28 21:52:28.000000 adafruit_circuitpython_requests-3.2.8/examples/wifi/expanded/requests_wifi_api_discord.py
--rw-r--r--   0 runner    (1001) docker     (127)    15772 2024-04-28 21:52:28.000000 adafruit_circuitpython_requests-3.2.8/examples/wifi/expanded/requests_wifi_api_fitbit.py
--rw-r--r--   0 runner    (1001) docker     (127)     3239 2024-04-28 21:52:28.000000 adafruit_circuitpython_requests-3.2.8/examples/wifi/expanded/requests_wifi_api_github.py
--rw-r--r--   0 runner    (1001) docker     (127)     4241 2024-04-28 21:52:28.000000 adafruit_circuitpython_requests-3.2.8/examples/wifi/expanded/requests_wifi_api_mastodon.py
--rw-r--r--   0 runner    (1001) docker     (127)     6840 2024-04-28 21:52:28.000000 adafruit_circuitpython_requests-3.2.8/examples/wifi/expanded/requests_wifi_api_openskynetwork_private.py
--rw-r--r--   0 runner    (1001) docker     (127)     7123 2024-04-28 21:52:28.000000 adafruit_circuitpython_requests-3.2.8/examples/wifi/expanded/requests_wifi_api_openskynetwork_private_area.py
--rw-r--r--   0 runner    (1001) docker     (127)     6294 2024-04-28 21:52:28.000000 adafruit_circuitpython_requests-3.2.8/examples/wifi/expanded/requests_wifi_api_openskynetwork_public.py
--rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-04-28 21:52:28.000000 adafruit_circuitpython_requests-3.2.8/examples/wifi/expanded/requests_wifi_api_premiereleague.py
--rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-04-28 21:52:28.000000 adafruit_circuitpython_requests-3.2.8/examples/wifi/expanded/requests_wifi_api_queuetimes.py
--rw-r--r--   0 runner    (1001) docker     (127)     5131 2024-04-28 21:52:28.000000 adafruit_circuitpython_requests-3.2.8/examples/wifi/expanded/requests_wifi_api_rocketlaunch_live.py
--rw-r--r--   0 runner    (1001) docker     (127)     4053 2024-04-28 21:52:28.000000 adafruit_circuitpython_requests-3.2.8/examples/wifi/expanded/requests_wifi_api_steam.py
--rw-r--r--   0 runner    (1001) docker     (127)     6306 2024-04-28 21:52:28.000000 adafruit_circuitpython_requests-3.2.8/examples/wifi/expanded/requests_wifi_api_twitch.py
--rw-r--r--   0 runner    (1001) docker     (127)     3971 2024-04-28 21:52:28.000000 adafruit_circuitpython_requests-3.2.8/examples/wifi/expanded/requests_wifi_api_youtube.py
--rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-04-28 21:52:28.000000 adafruit_circuitpython_requests-3.2.8/examples/wifi/expanded/requests_wifi_multiple_cookies.py
--rw-r--r--   0 runner    (1001) docker     (127)     4876 2024-04-28 21:52:28.000000 adafruit_circuitpython_requests-3.2.8/examples/wifi/expanded/requests_wifi_status_codes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-04-28 21:52:28.000000 adafruit_circuitpython_requests-3.2.8/examples/wifi/requests_wifi_advanced.py
--rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-04-28 21:52:28.000000 adafruit_circuitpython_requests-3.2.8/examples/wifi/requests_wifi_simpletest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 21:52:30.648459 adafruit_circuitpython_requests-3.2.8/examples/wiznet5k/
--rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-04-28 21:52:28.000000 adafruit_circuitpython_requests-3.2.8/examples/wiznet5k/requests_wiznet5k_advanced.py
--rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-04-28 21:52:28.000000 adafruit_circuitpython_requests-3.2.8/examples/wiznet5k/requests_wiznet5k_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-28 21:52:21.000000 adafruit_circuitpython_requests-3.2.8/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-28 21:52:28.000000 adafruit_circuitpython_requests-3.2.8/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (127)      166 2024-04-28 21:52:21.000000 adafruit_circuitpython_requests-3.2.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 21:52:30.648459 adafruit_circuitpython_requests-3.2.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 21:52:30.648459 adafruit_circuitpython_requests-3.2.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4007 2024-04-28 21:52:28.000000 adafruit_circuitpython_requests-3.2.8/tests/chunk_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    10156 2024-04-28 21:52:28.000000 adafruit_circuitpython_requests-3.2.8/tests/chunked_redirect_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2625 2024-04-28 21:52:28.000000 adafruit_circuitpython_requests-3.2.8/tests/concurrent_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-28 21:52:28.000000 adafruit_circuitpython_requests-3.2.8/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3063 2024-04-28 21:52:28.000000 adafruit_circuitpython_requests-3.2.8/tests/header_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-04-28 21:52:28.000000 adafruit_circuitpython_requests-3.2.8/tests/method_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3068 2024-04-28 21:52:28.000000 adafruit_circuitpython_requests-3.2.8/tests/mocket.py
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-28 21:52:28.000000 adafruit_circuitpython_requests-3.2.8/tests/parse_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-04-28 21:52:28.000000 adafruit_circuitpython_requests-3.2.8/tests/protocol_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     6399 2024-04-28 21:52:28.000000 adafruit_circuitpython_requests-3.2.8/tests/reuse_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-28 21:52:21.000000 adafruit_circuitpython_requests-3.2.8/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:50:14.128449 adafruit_circuitpython_requests-3.2.9/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:50:14.116448 adafruit_circuitpython_requests-3.2.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:50:14.116448 adafruit_circuitpython_requests-3.2.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-12 19:50:01.000000 adafruit_circuitpython_requests-3.2.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:50:14.120449 adafruit_circuitpython_requests-3.2.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-12 19:50:01.000000 adafruit_circuitpython_requests-3.2.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-12 19:50:01.000000 adafruit_circuitpython_requests-3.2.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-05-12 19:50:01.000000 adafruit_circuitpython_requests-3.2.9/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-12 19:50:01.000000 adafruit_circuitpython_requests-3.2.9/.github/workflows/release_pypi.yml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1724 2024-05-12 19:50:01.000000 adafruit_circuitpython_requests-3.2.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-05-12 19:50:01.000000 adafruit_circuitpython_requests-3.2.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    13078 2024-05-12 19:50:01.000000 adafruit_circuitpython_requests-3.2.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-12 19:50:01.000000 adafruit_circuitpython_requests-3.2.9/.readthedocs.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6147 2024-05-12 19:50:01.000000 adafruit_circuitpython_requests-3.2.9/CODE_OF_CONDUCT.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1098 2024-05-12 19:50:01.000000 adafruit_circuitpython_requests-3.2.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:50:14.120449 adafruit_circuitpython_requests-3.2.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (127)    16814 2024-05-12 19:50:01.000000 adafruit_circuitpython_requests-3.2.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-12 19:50:01.000000 adafruit_circuitpython_requests-3.2.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-12 19:50:01.000000 adafruit_circuitpython_requests-3.2.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-05-12 19:50:14.128449 adafruit_circuitpython_requests-3.2.9/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2642 2024-05-12 19:50:01.000000 adafruit_circuitpython_requests-3.2.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-12 19:50:01.000000 adafruit_circuitpython_requests-3.2.9/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:50:14.128449 adafruit_circuitpython_requests-3.2.9/adafruit_circuitpython_requests.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-05-12 19:50:14.000000 adafruit_circuitpython_requests-3.2.9/adafruit_circuitpython_requests.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-05-12 19:50:14.000000 adafruit_circuitpython_requests-3.2.9/adafruit_circuitpython_requests.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 19:50:14.000000 adafruit_circuitpython_requests-3.2.9/adafruit_circuitpython_requests.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-12 19:50:14.000000 adafruit_circuitpython_requests-3.2.9/adafruit_circuitpython_requests.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-12 19:50:14.000000 adafruit_circuitpython_requests-3.2.9/adafruit_circuitpython_requests.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    21326 2024-05-12 19:50:11.000000 adafruit_circuitpython_requests-3.2.9/adafruit_requests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:50:14.120449 adafruit_circuitpython_requests-3.2.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:50:14.120449 adafruit_circuitpython_requests-3.2.9/docs/_static/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4414 2024-05-12 19:50:01.000000 adafruit_circuitpython_requests-3.2.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-12 19:50:01.000000 adafruit_circuitpython_requests-3.2.9/docs/_static/favicon.ico.license
+-rwxr-xr-x   0 runner    (1001) docker     (127)      267 2024-05-12 19:50:01.000000 adafruit_circuitpython_requests-3.2.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-12 19:50:01.000000 adafruit_circuitpython_requests-3.2.9/docs/api.rst.license
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5400 2024-05-12 19:50:01.000000 adafruit_circuitpython_requests-3.2.9/docs/conf.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      803 2024-05-12 19:50:01.000000 adafruit_circuitpython_requests-3.2.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-12 19:50:01.000000 adafruit_circuitpython_requests-3.2.9/docs/examples.rst.license
+-rwxr-xr-x   0 runner    (1001) docker     (127)      973 2024-05-12 19:50:01.000000 adafruit_circuitpython_requests-3.2.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-12 19:50:01.000000 adafruit_circuitpython_requests-3.2.9/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-12 19:50:01.000000 adafruit_circuitpython_requests-3.2.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:50:14.116448 adafruit_circuitpython_requests-3.2.9/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:50:14.120449 adafruit_circuitpython_requests-3.2.9/examples/cpython/
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-12 19:50:11.000000 adafruit_circuitpython_requests-3.2.9/examples/cpython/requests_cpython_advanced.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-05-12 19:50:11.000000 adafruit_circuitpython_requests-3.2.9/examples/cpython/requests_cpython_simpletest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:50:14.124449 adafruit_circuitpython_requests-3.2.9/examples/esp32spi/
+-rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-05-12 19:50:11.000000 adafruit_circuitpython_requests-3.2.9/examples/esp32spi/requests_esp32spi_advanced.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-05-12 19:50:11.000000 adafruit_circuitpython_requests-3.2.9/examples/esp32spi/requests_esp32spi_simpletest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:50:14.124449 adafruit_circuitpython_requests-3.2.9/examples/fona/
+-rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-05-12 19:50:11.000000 adafruit_circuitpython_requests-3.2.9/examples/fona/requests_fona_advanced.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-05-12 19:50:11.000000 adafruit_circuitpython_requests-3.2.9/examples/fona/requests_fona_simpletest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:50:14.124449 adafruit_circuitpython_requests-3.2.9/examples/wifi/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:50:14.124449 adafruit_circuitpython_requests-3.2.9/examples/wifi/expanded/
+-rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-05-12 19:50:11.000000 adafruit_circuitpython_requests-3.2.9/examples/wifi/expanded/requests_wifi_adafruit_discord_active_online.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3480 2024-05-12 19:50:11.000000 adafruit_circuitpython_requests-3.2.9/examples/wifi/expanded/requests_wifi_api_discord.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15772 2024-05-12 19:50:11.000000 adafruit_circuitpython_requests-3.2.9/examples/wifi/expanded/requests_wifi_api_fitbit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3239 2024-05-12 19:50:11.000000 adafruit_circuitpython_requests-3.2.9/examples/wifi/expanded/requests_wifi_api_github.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4241 2024-05-12 19:50:11.000000 adafruit_circuitpython_requests-3.2.9/examples/wifi/expanded/requests_wifi_api_mastodon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6840 2024-05-12 19:50:11.000000 adafruit_circuitpython_requests-3.2.9/examples/wifi/expanded/requests_wifi_api_openskynetwork_private.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7123 2024-05-12 19:50:11.000000 adafruit_circuitpython_requests-3.2.9/examples/wifi/expanded/requests_wifi_api_openskynetwork_private_area.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6294 2024-05-12 19:50:11.000000 adafruit_circuitpython_requests-3.2.9/examples/wifi/expanded/requests_wifi_api_openskynetwork_public.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-05-12 19:50:11.000000 adafruit_circuitpython_requests-3.2.9/examples/wifi/expanded/requests_wifi_api_premiereleague.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-05-12 19:50:11.000000 adafruit_circuitpython_requests-3.2.9/examples/wifi/expanded/requests_wifi_api_queuetimes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5131 2024-05-12 19:50:11.000000 adafruit_circuitpython_requests-3.2.9/examples/wifi/expanded/requests_wifi_api_rocketlaunch_live.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4053 2024-05-12 19:50:11.000000 adafruit_circuitpython_requests-3.2.9/examples/wifi/expanded/requests_wifi_api_steam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6306 2024-05-12 19:50:11.000000 adafruit_circuitpython_requests-3.2.9/examples/wifi/expanded/requests_wifi_api_twitch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3971 2024-05-12 19:50:11.000000 adafruit_circuitpython_requests-3.2.9/examples/wifi/expanded/requests_wifi_api_youtube.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-05-12 19:50:11.000000 adafruit_circuitpython_requests-3.2.9/examples/wifi/expanded/requests_wifi_multiple_cookies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4876 2024-05-12 19:50:11.000000 adafruit_circuitpython_requests-3.2.9/examples/wifi/expanded/requests_wifi_status_codes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-05-12 19:50:11.000000 adafruit_circuitpython_requests-3.2.9/examples/wifi/requests_wifi_advanced.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-05-12 19:50:11.000000 adafruit_circuitpython_requests-3.2.9/examples/wifi/requests_wifi_simpletest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:50:14.124449 adafruit_circuitpython_requests-3.2.9/examples/wiznet5k/
+-rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-05-12 19:50:11.000000 adafruit_circuitpython_requests-3.2.9/examples/wiznet5k/requests_wiznet5k_advanced.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-05-12 19:50:11.000000 adafruit_circuitpython_requests-3.2.9/examples/wiznet5k/requests_wiznet5k_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-12 19:50:01.000000 adafruit_circuitpython_requests-3.2.9/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-05-12 19:50:11.000000 adafruit_circuitpython_requests-3.2.9/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      166 2024-05-12 19:50:01.000000 adafruit_circuitpython_requests-3.2.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 19:50:14.128449 adafruit_circuitpython_requests-3.2.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:50:14.128449 adafruit_circuitpython_requests-3.2.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4007 2024-05-12 19:50:11.000000 adafruit_circuitpython_requests-3.2.9/tests/chunk_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10156 2024-05-12 19:50:11.000000 adafruit_circuitpython_requests-3.2.9/tests/chunked_redirect_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2625 2024-05-12 19:50:11.000000 adafruit_circuitpython_requests-3.2.9/tests/concurrent_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-12 19:50:11.000000 adafruit_circuitpython_requests-3.2.9/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3063 2024-05-12 19:50:11.000000 adafruit_circuitpython_requests-3.2.9/tests/header_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-05-12 19:50:11.000000 adafruit_circuitpython_requests-3.2.9/tests/method_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3068 2024-05-12 19:50:11.000000 adafruit_circuitpython_requests-3.2.9/tests/mocket.py
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-12 19:50:11.000000 adafruit_circuitpython_requests-3.2.9/tests/parse_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2310 2024-05-12 19:50:11.000000 adafruit_circuitpython_requests-3.2.9/tests/protocol_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6399 2024-05-12 19:50:11.000000 adafruit_circuitpython_requests-3.2.9/tests/reuse_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-05-12 19:50:01.000000 adafruit_circuitpython_requests-3.2.9/tox.ini
```

### Comparing `adafruit_circuitpython_requests-3.2.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit_circuitpython_requests-3.2.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.8/.gitignore` & `adafruit_circuitpython_requests-3.2.9/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.8/.pre-commit-config.yaml` & `adafruit_circuitpython_requests-3.2.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.8/.pylintrc` & `adafruit_circuitpython_requests-3.2.9/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.8/CODE_OF_CONDUCT.md` & `adafruit_circuitpython_requests-3.2.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.8/LICENSE` & `adafruit_circuitpython_requests-3.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.8/LICENSES/CC-BY-4.0.txt` & `adafruit_circuitpython_requests-3.2.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.8/LICENSES/MIT.txt` & `adafruit_circuitpython_requests-3.2.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.8/LICENSES/Unlicense.txt` & `adafruit_circuitpython_requests-3.2.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.8/PKG-INFO` & `adafruit_circuitpython_requests-3.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-requests
-Version: 3.2.8
+Version: 3.2.9
 Summary: A requests-like library for web interfacing
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_Requests
 Keywords: adafruit,blinka,circuitpython,micropython,requests,requests,,networking
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit_circuitpython_requests-3.2.8/README.rst` & `adafruit_circuitpython_requests-3.2.9/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.8/adafruit_circuitpython_requests.egg-info/PKG-INFO` & `adafruit_circuitpython_requests-3.2.9/adafruit_circuitpython_requests.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-requests
-Version: 3.2.8
+Version: 3.2.9
 Summary: A requests-like library for web interfacing
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_Requests
 Keywords: adafruit,blinka,circuitpython,micropython,requests,requests,,networking
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit_circuitpython_requests-3.2.8/adafruit_circuitpython_requests.egg-info/SOURCES.txt` & `adafruit_circuitpython_requests-3.2.9/adafruit_circuitpython_requests.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.8/adafruit_requests.py` & `adafruit_circuitpython_requests-3.2.9/adafruit_requests.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
   https://github.com/adafruit/circuitpython/releases
 
 * Adafruit's Connection Manager library:
   https://github.com/adafruit/Adafruit_CircuitPython_ConnectionManager
 
 """
 
-__version__ = "3.2.8"
+__version__ = "3.2.9"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_Requests.git"
 
 import errno
 import json as json_module
 import sys
 
 from adafruit_connection_manager import get_connection_manager
```

### Comparing `adafruit_circuitpython_requests-3.2.8/docs/_static/favicon.ico` & `adafruit_circuitpython_requests-3.2.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.8/docs/conf.py` & `adafruit_circuitpython_requests-3.2.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.8/docs/examples.rst` & `adafruit_circuitpython_requests-3.2.9/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.8/docs/index.rst` & `adafruit_circuitpython_requests-3.2.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.8/examples/cpython/requests_cpython_advanced.py` & `adafruit_circuitpython_requests-3.2.9/examples/cpython/requests_cpython_advanced.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.8/examples/cpython/requests_cpython_simpletest.py` & `adafruit_circuitpython_requests-3.2.9/examples/cpython/requests_cpython_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.8/examples/esp32spi/requests_esp32spi_advanced.py` & `adafruit_circuitpython_requests-3.2.9/examples/esp32spi/requests_esp32spi_advanced.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.8/examples/esp32spi/requests_esp32spi_simpletest.py` & `adafruit_circuitpython_requests-3.2.9/examples/esp32spi/requests_esp32spi_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.8/examples/fona/requests_fona_advanced.py` & `adafruit_circuitpython_requests-3.2.9/examples/fona/requests_fona_advanced.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.8/examples/fona/requests_fona_simpletest.py` & `adafruit_circuitpython_requests-3.2.9/examples/fona/requests_fona_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.8/examples/wifi/expanded/requests_wifi_adafruit_discord_active_online.py` & `adafruit_circuitpython_requests-3.2.9/examples/wifi/expanded/requests_wifi_adafruit_discord_active_online.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.8/examples/wifi/expanded/requests_wifi_api_discord.py` & `adafruit_circuitpython_requests-3.2.9/examples/wifi/expanded/requests_wifi_api_discord.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.8/examples/wifi/expanded/requests_wifi_api_fitbit.py` & `adafruit_circuitpython_requests-3.2.9/examples/wifi/expanded/requests_wifi_api_fitbit.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.8/examples/wifi/expanded/requests_wifi_api_github.py` & `adafruit_circuitpython_requests-3.2.9/examples/wifi/expanded/requests_wifi_api_github.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.8/examples/wifi/expanded/requests_wifi_api_mastodon.py` & `adafruit_circuitpython_requests-3.2.9/examples/wifi/expanded/requests_wifi_api_mastodon.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.8/examples/wifi/expanded/requests_wifi_api_openskynetwork_private.py` & `adafruit_circuitpython_requests-3.2.9/examples/wifi/expanded/requests_wifi_api_openskynetwork_private.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.8/examples/wifi/expanded/requests_wifi_api_openskynetwork_private_area.py` & `adafruit_circuitpython_requests-3.2.9/examples/wifi/expanded/requests_wifi_api_openskynetwork_private_area.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.8/examples/wifi/expanded/requests_wifi_api_openskynetwork_public.py` & `adafruit_circuitpython_requests-3.2.9/examples/wifi/expanded/requests_wifi_api_openskynetwork_public.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.8/examples/wifi/expanded/requests_wifi_api_premiereleague.py` & `adafruit_circuitpython_requests-3.2.9/examples/wifi/expanded/requests_wifi_api_premiereleague.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.8/examples/wifi/expanded/requests_wifi_api_queuetimes.py` & `adafruit_circuitpython_requests-3.2.9/examples/wifi/expanded/requests_wifi_api_queuetimes.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.8/examples/wifi/expanded/requests_wifi_api_rocketlaunch_live.py` & `adafruit_circuitpython_requests-3.2.9/examples/wifi/expanded/requests_wifi_api_rocketlaunch_live.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.8/examples/wifi/expanded/requests_wifi_api_steam.py` & `adafruit_circuitpython_requests-3.2.9/examples/wifi/expanded/requests_wifi_api_steam.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.8/examples/wifi/expanded/requests_wifi_api_twitch.py` & `adafruit_circuitpython_requests-3.2.9/examples/wifi/expanded/requests_wifi_api_twitch.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.8/examples/wifi/expanded/requests_wifi_api_youtube.py` & `adafruit_circuitpython_requests-3.2.9/examples/wifi/expanded/requests_wifi_api_youtube.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.8/examples/wifi/expanded/requests_wifi_multiple_cookies.py` & `adafruit_circuitpython_requests-3.2.9/examples/wifi/expanded/requests_wifi_multiple_cookies.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.8/examples/wifi/expanded/requests_wifi_status_codes.py` & `adafruit_circuitpython_requests-3.2.9/examples/wifi/expanded/requests_wifi_status_codes.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.8/examples/wifi/requests_wifi_advanced.py` & `adafruit_circuitpython_requests-3.2.9/examples/wifi/requests_wifi_advanced.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.8/examples/wifi/requests_wifi_simpletest.py` & `adafruit_circuitpython_requests-3.2.9/examples/wifi/requests_wifi_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.8/examples/wiznet5k/requests_wiznet5k_advanced.py` & `adafruit_circuitpython_requests-3.2.9/examples/wiznet5k/requests_wiznet5k_advanced.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.8/examples/wiznet5k/requests_wiznet5k_simpletest.py` & `adafruit_circuitpython_requests-3.2.9/examples/wiznet5k/requests_wiznet5k_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.8/pyproject.toml` & `adafruit_circuitpython_requests-3.2.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-requests"
 description = "A requests-like library for web interfacing"
-version = "3.2.8"
+version = "3.2.9"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_Requests"}
 keywords = [
     "adafruit",
```

### Comparing `adafruit_circuitpython_requests-3.2.8/tests/chunk_test.py` & `adafruit_circuitpython_requests-3.2.9/tests/chunk_test.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.8/tests/chunked_redirect_test.py` & `adafruit_circuitpython_requests-3.2.9/tests/chunked_redirect_test.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.8/tests/concurrent_test.py` & `adafruit_circuitpython_requests-3.2.9/tests/concurrent_test.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.8/tests/conftest.py` & `adafruit_circuitpython_requests-3.2.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.8/tests/header_test.py` & `adafruit_circuitpython_requests-3.2.9/tests/header_test.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.8/tests/method_test.py` & `adafruit_circuitpython_requests-3.2.9/tests/method_test.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.8/tests/mocket.py` & `adafruit_circuitpython_requests-3.2.9/tests/mocket.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.8/tests/parse_test.py` & `adafruit_circuitpython_requests-3.2.9/tests/parse_test.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.8/tests/protocol_test.py` & `adafruit_circuitpython_requests-3.2.9/tests/protocol_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from unittest import mock
 
 import mocket
 import pytest
 
 
 def test_get_https_no_ssl(requests):
-    with pytest.raises(AttributeError):
+    with pytest.raises(ValueError):
         requests.get("https://" + mocket.MOCK_ENDPOINT_1)
 
 
 def test_get_https_text(sock, requests_ssl):
     response = requests_ssl.get("https://" + mocket.MOCK_ENDPOINT_1)
 
     sock.connect.assert_called_once_with((mocket.MOCK_HOST_1, 443))
```

### Comparing `adafruit_circuitpython_requests-3.2.8/tests/reuse_test.py` & `adafruit_circuitpython_requests-3.2.9/tests/reuse_test.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_requests-3.2.8/tox.ini` & `adafruit_circuitpython_requests-3.2.9/tox.ini`

 * *Files identical despite different names*

