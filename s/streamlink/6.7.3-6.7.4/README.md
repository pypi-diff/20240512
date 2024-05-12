# Comparing `tmp/streamlink-6.7.3.tar.gz` & `tmp/streamlink-6.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlink-6.7.3.tar", last modified: Sun Apr 14 15:40:52 2024, max compression
+gzip compressed data, was "streamlink-6.7.4.tar", last modified: Sun May 12 11:17:37 2024, max compression
```

## Comparing `streamlink-6.7.3.tar` & `streamlink-6.7.4.tar`

### file list

```diff
@@ -1,674 +1,675 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:52.296392 streamlink-6.7.3/
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-14 15:40:22.000000 streamlink-6.7.3/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)   100542 2024-04-14 15:40:22.000000 streamlink-6.7.3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-04-14 15:40:22.000000 streamlink-6.7.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-14 15:40:22.000000 streamlink-6.7.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6438 2024-04-14 15:40:52.296392 streamlink-6.7.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4486 2024-04-14 15:40:22.000000 streamlink-6.7.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:52.204392 streamlink-6.7.3/build_backend/
--rw-r--r--   0 runner    (1001) docker     (127)     3370 2024-04-14 15:40:22.000000 streamlink-6.7.3/build_backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      898 2024-04-14 15:40:22.000000 streamlink-6.7.3/build_backend/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     3588 2024-04-14 15:40:22.000000 streamlink-6.7.3/build_backend/onbuild.py
--rw-r--r--   0 runner    (1001) docker     (127)    15908 2024-04-14 15:40:22.000000 streamlink-6.7.3/build_backend/plugins_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-04-14 15:40:22.000000 streamlink-6.7.3/build_backend/test_build_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     3577 2024-04-14 15:40:22.000000 streamlink-6.7.3/build_backend/test_onbuild.py
--rw-r--r--   0 runner    (1001) docker     (127)    37280 2024-04-14 15:40:22.000000 streamlink-6.7.3/build_backend/test_plugins_json.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:52.196392 streamlink-6.7.3/completions/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:52.204392 streamlink-6.7.3/completions/bash/
--rw-r--r--   0 runner    (1001) docker     (127)    10164 2024-04-14 15:40:47.000000 streamlink-6.7.3/completions/bash/streamlink
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:52.204392 streamlink-6.7.3/completions/zsh/
--rw-r--r--   0 runner    (1001) docker     (127)    36671 2024-04-14 15:40:48.000000 streamlink-6.7.3/completions/zsh/_streamlink
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-14 15:40:22.000000 streamlink-6.7.3/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:52.208392 streamlink-6.7.3/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     5813 2024-04-14 15:40:22.000000 streamlink-6.7.3/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:52.196392 streamlink-6.7.3/docs/_build/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:52.208392 streamlink-6.7.3/docs/_build/man/
--rw-r--r--   0 runner    (1001) docker     (127)    41171 2024-04-14 15:40:46.000000 streamlink-6.7.3/docs/_build/man/streamlink.1
--rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-04-14 15:40:22.000000 streamlink-6.7.3/docs/_man.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:52.212392 streamlink-6.7.3/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)    12092 2024-04-14 15:40:22.000000 streamlink-6.7.3/docs/_static/apple-touch-icon.png
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-04-14 15:40:22.000000 streamlink-6.7.3/docs/_static/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-04-14 15:40:22.000000 streamlink-6.7.3/docs/_static/favicon-32x32.png
--rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-04-14 15:40:22.000000 streamlink-6.7.3/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-04-14 15:40:22.000000 streamlink-6.7.3/docs/_static/icon-ffmpeg.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-04-14 15:40:22.000000 streamlink-6.7.3/docs/_static/icon-python.svg
--rw-r--r--   0 runner    (1001) docker     (127)    18593 2024-04-14 15:40:22.000000 streamlink-6.7.3/docs/_static/icon.svg
--rw-r--r--   0 runner    (1001) docker     (127)    15790 2024-04-14 15:40:22.000000 streamlink-6.7.3/docs/_static/opengraph-image.png
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-14 15:40:22.000000 streamlink-6.7.3/docs/_static/site.webmanifest
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:52.212392 streamlink-6.7.3/docs/_static/styles/
--rw-r--r--   0 runner    (1001) docker     (127)     7707 2024-04-14 15:40:22.000000 streamlink-6.7.3/docs/_static/styles/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:52.212392 streamlink-6.7.3/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-04-14 15:40:22.000000 streamlink-6.7.3/docs/_templates/base.html
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-04-14 15:40:22.000000 streamlink-6.7.3/docs/_templates/page.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:52.212392 streamlink-6.7.3/docs/_templates/sidebar/
--rw-r--r--   0 runner    (1001) docker     (127)      908 2024-04-14 15:40:22.000000 streamlink-6.7.3/docs/_templates/sidebar/brand.html
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-14 15:40:22.000000 streamlink-6.7.3/docs/_templates/sidebar/github-buttons.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:52.212392 streamlink-6.7.3/docs/api/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-14 15:40:22.000000 streamlink-6.7.3/docs/api/cache.rst
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-14 15:40:22.000000 streamlink-6.7.3/docs/api/exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-14 15:40:22.000000 streamlink-6.7.3/docs/api/options.rst
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-14 15:40:22.000000 streamlink-6.7.3/docs/api/plugin.rst
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-14 15:40:22.000000 streamlink-6.7.3/docs/api/session.rst
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-14 15:40:22.000000 streamlink-6.7.3/docs/api/stream.rst
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-14 15:40:22.000000 streamlink-6.7.3/docs/api/streamlink.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11275 2024-04-14 15:40:22.000000 streamlink-6.7.3/docs/api/validate.rst
--rw-r--r--   0 runner    (1001) docker     (127)      742 2024-04-14 15:40:22.000000 streamlink-6.7.3/docs/api/webbrowser.rst
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-14 15:40:22.000000 streamlink-6.7.3/docs/api.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:52.212392 streamlink-6.7.3/docs/api_guide/
--rw-r--r--   0 runner    (1001) docker     (127)     4429 2024-04-14 15:40:22.000000 streamlink-6.7.3/docs/api_guide/quickstart.rst
--rw-r--r--   0 runner    (1001) docker     (127)    17250 2024-04-14 15:40:22.000000 streamlink-6.7.3/docs/api_guide/validate.rst
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-14 15:40:22.000000 streamlink-6.7.3/docs/api_guide.rst
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-14 15:40:22.000000 streamlink-6.7.3/docs/applications.rst
--rw-r--r--   0 runner    (1001) docker     (127)   100542 2024-04-14 15:40:22.000000 streamlink-6.7.3/docs/changelog.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:52.212392 streamlink-6.7.3/docs/cli/
--rw-r--r--   0 runner    (1001) docker     (127)     4530 2024-04-14 15:40:22.000000 streamlink-6.7.3/docs/cli/config.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3179 2024-04-14 15:40:22.000000 streamlink-6.7.3/docs/cli/metadata.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-04-14 15:40:22.000000 streamlink-6.7.3/docs/cli/plugin-sideloading.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:52.216392 streamlink-6.7.3/docs/cli/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-04-14 15:40:22.000000 streamlink-6.7.3/docs/cli/plugins/crunchyroll.rst
--rw-r--r--   0 runner    (1001) docker     (127)    10202 2024-04-14 15:40:22.000000 streamlink-6.7.3/docs/cli/plugins/twitch.rst
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-14 15:40:22.000000 streamlink-6.7.3/docs/cli/plugins.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3003 2024-04-14 15:40:22.000000 streamlink-6.7.3/docs/cli/protocols.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-14 15:40:22.000000 streamlink-6.7.3/docs/cli/proxy.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6882 2024-04-14 15:40:22.000000 streamlink-6.7.3/docs/cli/tutorial.rst
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-04-14 15:40:22.000000 streamlink-6.7.3/docs/cli.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7916 2024-04-14 15:40:22.000000 streamlink-6.7.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)    11426 2024-04-14 15:40:22.000000 streamlink-6.7.3/docs/deprecations.rst
--rw-r--r--   0 runner    (1001) docker     (127)    10409 2024-04-14 15:40:22.000000 streamlink-6.7.3/docs/developing.rst
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-14 15:40:22.000000 streamlink-6.7.3/docs/docutils.conf
--rw-r--r--   0 runner    (1001) docker     (127)     3013 2024-04-14 15:40:22.000000 streamlink-6.7.3/docs/donate.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6552 2024-04-14 15:40:22.000000 streamlink-6.7.3/docs/ext_argparse.py
--rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-04-14 15:40:22.000000 streamlink-6.7.3/docs/ext_github.py
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-14 15:40:22.000000 streamlink-6.7.3/docs/ext_html_template_vars.py
--rw-r--r--   0 runner    (1001) docker     (127)     8465 2024-04-14 15:40:22.000000 streamlink-6.7.3/docs/ext_plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-14 15:40:22.000000 streamlink-6.7.3/docs/ext_releaseref.py
--rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-04-14 15:40:22.000000 streamlink-6.7.3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)    25334 2024-04-14 15:40:22.000000 streamlink-6.7.3/docs/install.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11739 2024-04-14 15:40:22.000000 streamlink-6.7.3/docs/migrations.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3401 2024-04-14 15:40:22.000000 streamlink-6.7.3/docs/players.rst
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-14 15:40:22.000000 streamlink-6.7.3/docs/plugins.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3404 2024-04-14 15:40:22.000000 streamlink-6.7.3/docs/thirdparty.rst
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-14 15:40:22.000000 streamlink-6.7.3/docs-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)    18593 2024-04-14 15:40:22.000000 streamlink-6.7.3/icon.svg
--rw-r--r--   0 runner    (1001) docker     (127)     6814 2024-04-14 15:40:52.300392 streamlink-6.7.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:52.216392 streamlink-6.7.3/script/
--rwxr-xr-x   0 runner    (1001) docker     (127)      802 2024-04-14 15:40:22.000000 streamlink-6.7.3/script/build-shell-completions.sh
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 15:40:52.296392 streamlink-6.7.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3161 2024-04-14 15:40:52.300392 streamlink-6.7.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:52.200392 streamlink-6.7.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:52.216392 streamlink-6.7.3/src/streamlink/
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-14 15:40:52.300392 streamlink-6.7.3/src/streamlink/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3934 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/buffers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4918 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/compat.py
--rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     8007 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    10961 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/options.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:52.216392 streamlink-6.7.3/src/streamlink/packages/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/packages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6194 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/packages/requests_file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:52.216392 streamlink-6.7.3/src/streamlink/plugin/
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:52.220392 streamlink-6.7.3/src/streamlink/plugin/api/
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugin/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugin/api/http_session.py
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugin/api/useragents.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:52.220392 streamlink-6.7.3/src/streamlink/plugin/api/validate/
--rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugin/api/validate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugin/api/validate/_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)    13127 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugin/api/validate/_schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)    11763 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugin/api/validate/_validate.py
--rw-r--r--   0 runner    (1001) docker     (127)    19587 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugin/api/validate/_validators.py
--rw-r--r--   0 runner    (1001) docker     (127)     6614 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugin/api/websocket.py
--rw-r--r--   0 runner    (1001) docker     (127)    26032 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugin/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:52.240392 streamlink-6.7.3/src/streamlink/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9677 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/abematv.py
--rw-r--r--   0 runner    (1001) docker     (127)     6520 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/adultswim.py
--rw-r--r--   0 runner    (1001) docker     (127)     7622 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/afreeca.py
--rw-r--r--   0 runner    (1001) docker     (127)     5633 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/albavision.py
--rw-r--r--   0 runner    (1001) docker     (127)     3896 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/aloula.py
--rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/app17.py
--rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/ard_live.py
--rw-r--r--   0 runner    (1001) docker     (127)     4769 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/ard_mediathek.py
--rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/artetv.py
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/atpchallenger.py
--rw-r--r--   0 runner    (1001) docker     (127)     3002 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/atresplayer.py
--rw-r--r--   0 runner    (1001) docker     (127)     8328 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/bbciplayer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3956 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/bfmtv.py
--rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/bigo.py
--rw-r--r--   0 runner    (1001) docker     (127)     5642 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/bilibili.py
--rw-r--r--   0 runner    (1001) docker     (127)     3642 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/blazetv.py
--rw-r--r--   0 runner    (1001) docker     (127)     4539 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/bloomberg.py
--rw-r--r--   0 runner    (1001) docker     (127)     5014 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/booyah.py
--rw-r--r--   0 runner    (1001) docker     (127)     3737 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/brightcove.py
--rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/btv.py
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/cbsnews.py
--rw-r--r--   0 runner    (1001) docker     (127)     3489 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/cdnbg.py
--rw-r--r--   0 runner    (1001) docker     (127)     7082 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/ceskatelevize.py
--rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/cinergroup.py
--rw-r--r--   0 runner    (1001) docker     (127)     2540 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/clubbingtv.py
--rw-r--r--   0 runner    (1001) docker     (127)     3976 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/cmmedia.py
--rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/cnews.py
--rw-r--r--   0 runner    (1001) docker     (127)    14036 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/crunchyroll.py
--rw-r--r--   0 runner    (1001) docker     (127)     4264 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/dailymotion.py
--rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/dash.py
--rw-r--r--   0 runner    (1001) docker     (127)     4255 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/delfi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3514 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/deutschewelle.py
--rw-r--r--   0 runner    (1001) docker     (127)     4468 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/dlive.py
--rw-r--r--   0 runner    (1001) docker     (127)     5773 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/dogan.py
--rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/dogus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/drdk.py
--rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/earthcam.py
--rw-r--r--   0 runner    (1001) docker     (127)     3504 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/euronews.py
--rw-r--r--   0 runner    (1001) docker     (127)     5512 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/facebook.py
--rw-r--r--   0 runner    (1001) docker     (127)     8421 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/filmon.py
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/galatasaraytv.py
--rw-r--r--   0 runner    (1001) docker     (127)      960 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/goltelevision.py
--rw-r--r--   0 runner    (1001) docker     (127)     5307 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/goodgame.py
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/googledrive.py
--rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/gulli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/hiplayer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/hls.py
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/http.py
--rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/htv.py
--rw-r--r--   0 runner    (1001) docker     (127)     2763 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/huajiao.py
--rw-r--r--   0 runner    (1001) docker     (127)     4227 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/huya.py
--rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/idf1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/indihometv.py
--rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/invintus.py
--rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/kugou.py
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/linelive.py
--rw-r--r--   0 runner    (1001) docker     (127)     4493 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/livestream.py
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/lnk.py
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/lrt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/ltv_lsm_lv.py
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/mangomolo.py
--rw-r--r--   0 runner    (1001) docker     (127)     5255 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/mdstrm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/mediaklikk.py
--rw-r--r--   0 runner    (1001) docker     (127)     3740 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/mediavitrina.py
--rw-r--r--   0 runner    (1001) docker     (127)     7100 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/mildom.py
--rw-r--r--   0 runner    (1001) docker     (127)     4120 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/mitele.py
--rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/mixcloud.py
--rw-r--r--   0 runner    (1001) docker     (127)     5132 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/mjunoon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/mrtmk.py
--rw-r--r--   0 runner    (1001) docker     (127)     4685 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/n13tv.py
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/nasaplus.py
--rw-r--r--   0 runner    (1001) docker     (127)      820 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/nhkworld.py
--rw-r--r--   0 runner    (1001) docker     (127)    10573 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/nicolive.py
--rw-r--r--   0 runner    (1001) docker     (127)     3671 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/nimotv.py
--rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/nos.py
--rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/nownews.py
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/nowtvtr.py
--rw-r--r--   0 runner    (1001) docker     (127)     3660 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/nrk.py
--rw-r--r--   0 runner    (1001) docker     (127)     4564 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/okru.py
--rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/olympicchannel.py
--rw-r--r--   0 runner    (1001) docker     (127)     4202 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/oneplusone.py
--rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/onetv.py
--rw-r--r--   0 runner    (1001) docker     (127)     5833 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/openrectv.py
--rw-r--r--   0 runner    (1001) docker     (127)     3270 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/pandalive.py
--rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/piaulizaportal.py
--rw-r--r--   0 runner    (1001) docker     (127)     4779 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/picarto.py
--rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/piczel.py
--rw-r--r--   0 runner    (1001) docker     (127)     6543 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/pixiv.py
--rw-r--r--   0 runner    (1001) docker     (127)     6981 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/pluto.py
--rw-r--r--   0 runner    (1001) docker     (127)     5115 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/pluzz.py
--rw-r--r--   0 runner    (1001) docker     (127)     3988 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/radiko.py
--rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/radionet.py
--rw-r--r--   0 runner    (1001) docker     (127)     6447 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/raiplay.py
--rw-r--r--   0 runner    (1001) docker     (127)     3221 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/reuters.py
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/rtpa.py
--rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/rtpplay.py
--rw-r--r--   0 runner    (1001) docker     (127)     6597 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/rtve.py
--rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/rtvs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3760 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/ruv.py
--rw-r--r--   0 runner    (1001) docker     (127)     3265 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/sbscokr.py
--rw-r--r--   0 runner    (1001) docker     (127)     2886 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/showroom.py
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/sportal.py
--rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/sportschau.py
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/ssh101.py
--rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/stadium.py
--rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/steam.py
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/streamable.py
--rw-r--r--   0 runner    (1001) docker     (127)     5739 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/streann.py
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/stv.py
--rw-r--r--   0 runner    (1001) docker     (127)     5355 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/svtplay.py
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/swisstxt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/telefe.py
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/telemadrid.py
--rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/tf1.py
--rw-r--r--   0 runner    (1001) docker     (127)     6625 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/trovo.py
--rw-r--r--   0 runner    (1001) docker     (127)     3357 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/turkuvaz.py
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/tv360.py
--rw-r--r--   0 runner    (1001) docker     (127)     3625 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/tv3cat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/tv4play.py
--rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/tv5monde.py
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/tv8.py
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/tv999.py
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/tvibo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2625 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/tviplayer.py
--rw-r--r--   0 runner    (1001) docker     (127)     8870 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/tvp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/tvrby.py
--rw-r--r--   0 runner    (1001) docker     (127)      898 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/tvrplus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/tvtoya.py
--rw-r--r--   0 runner    (1001) docker     (127)     6132 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/twitcasting.py
--rw-r--r--   0 runner    (1001) docker     (127)    33594 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/twitch.py
--rw-r--r--   0 runner    (1001) docker     (127)    19213 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/ustreamtv.py
--rw-r--r--   0 runner    (1001) docker     (127)     5775 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/ustvnow.py
--rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/vidio.py
--rw-r--r--   0 runner    (1001) docker     (127)     8563 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/vimeo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/vinhlongtv.py
--rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/vk.py
--rw-r--r--   0 runner    (1001) docker     (127)     3347 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/vkplay.py
--rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/vtvgo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2647 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/webtv.py
--rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/welt.py
--rw-r--r--   0 runner    (1001) docker     (127)     4880 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/wwenetwork.py
--rw-r--r--   0 runner    (1001) docker     (127)    15401 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/youtube.py
--rw-r--r--   0 runner    (1001) docker     (127)     3871 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/yupptv.py
--rw-r--r--   0 runner    (1001) docker     (127)    12860 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/zattoo.py
--rw-r--r--   0 runner    (1001) docker     (127)     3435 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/zdf_mediathek.py
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/zeenews.py
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/zengatv.py
--rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/plugins/zhanqi.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:52.244392 streamlink-6.7.3/src/streamlink/session/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/session/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9325 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/session/http.py
--rw-r--r--   0 runner    (1001) docker     (127)    12151 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/session/http.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    19101 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/session/options.py
--rw-r--r--   0 runner    (1001) docker     (127)    13238 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/session/plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)     7495 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/session/session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:52.244392 streamlink-6.7.3/src/streamlink/stream/
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/stream/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:52.244392 streamlink-6.7.3/src/streamlink/stream/dash/
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/stream/dash/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14067 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/stream/dash/dash.py
--rw-r--r--   0 runner    (1001) docker     (127)    36858 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/stream/dash/manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/stream/dash/segment.py
--rw-r--r--   0 runner    (1001) docker     (127)    10466 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/stream/ffmpegmux.py
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/stream/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/stream/filtered.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:52.244392 streamlink-6.7.3/src/streamlink/stream/hls/
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/stream/hls/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    33983 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/stream/hls/hls.py
--rw-r--r--   0 runner    (1001) docker     (127)    21481 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/stream/hls/m3u8.py
--rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/stream/hls/segment.py
--rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/stream/http.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:52.244392 streamlink-6.7.3/src/streamlink/stream/segmented/
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/stream/segmented/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/stream/segmented/concurrent.py
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/stream/segmented/segment.py
--rw-r--r--   0 runner    (1001) docker     (127)     8118 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/stream/segmented/segmented.py
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/stream/stream.py
--rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/stream/wrappers.py
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/user_input.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:52.248392 streamlink-6.7.3/src/streamlink/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3101 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/utils/args.py
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/utils/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/utils/crypto.py
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/utils/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/utils/formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5655 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/utils/l10n.py
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/utils/module.py
--rw-r--r--   0 runner    (1001) docker     (127)     3362 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/utils/named_pipe.py
--rw-r--r--   0 runner    (1001) docker     (127)     3582 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/utils/parse.py
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/utils/path.py
--rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/utils/processoutput.py
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/utils/random.py
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/utils/socket.py
--rw-r--r--   0 runner    (1001) docker     (127)     3510 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/utils/times.py
--rw-r--r--   0 runner    (1001) docker     (127)     5367 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/utils/url.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:52.248392 streamlink-6.7.3/src/streamlink/webbrowser/
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/webbrowser/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:52.248392 streamlink-6.7.3/src/streamlink/webbrowser/cdp/
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/webbrowser/cdp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19581 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/webbrowser/cdp/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    13939 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/webbrowser/cdp/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:52.252392 streamlink-6.7.3/src/streamlink/webbrowser/cdp/devtools/
--rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/webbrowser/cdp/devtools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21632 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/webbrowser/cdp/devtools/browser.py
--rw-r--r--   0 runner    (1001) docker     (127)    49407 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/webbrowser/cdp/devtools/debugger.py
--rw-r--r--   0 runner    (1001) docker     (127)    61679 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/webbrowser/cdp/devtools/dom.py
--rw-r--r--   0 runner    (1001) docker     (127)    26084 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/webbrowser/cdp/devtools/emulation.py
--rw-r--r--   0 runner    (1001) docker     (127)    19534 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/webbrowser/cdp/devtools/fetch.py
--rw-r--r--   0 runner    (1001) docker     (127)    27632 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/webbrowser/cdp/devtools/input_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/webbrowser/cdp/devtools/inspector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3084 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/webbrowser/cdp/devtools/io.py
--rw-r--r--   0 runner    (1001) docker     (127)   130706 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/webbrowser/cdp/devtools/network.py
--rw-r--r--   0 runner    (1001) docker     (127)   107521 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/webbrowser/cdp/devtools/page.py
--rw-r--r--   0 runner    (1001) docker     (127)    62110 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/webbrowser/cdp/devtools/runtime.py
--rw-r--r--   0 runner    (1001) docker     (127)    17300 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/webbrowser/cdp/devtools/security.py
--rw-r--r--   0 runner    (1001) docker     (127)    24082 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/webbrowser/cdp/devtools/target.py
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/webbrowser/cdp/devtools/util.py
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/webbrowser/cdp/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     8564 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/webbrowser/chromium.py
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/webbrowser/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5296 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink/webbrowser/webbrowser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:52.296392 streamlink-6.7.3/src/streamlink.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6438 2024-04-14 15:40:52.000000 streamlink-6.7.3/src/streamlink.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    19654 2024-04-14 15:40:52.000000 streamlink-6.7.3/src/streamlink.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 15:40:52.000000 streamlink-6.7.3/src/streamlink.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-14 15:40:52.000000 streamlink-6.7.3/src/streamlink.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-14 15:40:52.000000 streamlink-6.7.3/src/streamlink.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-14 15:40:52.000000 streamlink-6.7.3/src/streamlink.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:52.252392 streamlink-6.7.3/src/streamlink_cli/
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink_cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink_cli/_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    49425 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink_cli/argparser.py
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink_cli/compat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink_cli/console.py
--rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink_cli/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    31969 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink_cli/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:52.256392 streamlink-6.7.3/src/streamlink_cli/output/
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink_cli/output/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink_cli/output/abc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink_cli/output/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     3511 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink_cli/output/http.py
--rw-r--r--   0 runner    (1001) docker     (127)    10265 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink_cli/output/player.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink_cli/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     4918 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink_cli/streamrunner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:52.256392 streamlink-6.7.3/src/streamlink_cli/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink_cli/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink_cli/utils/formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink_cli/utils/path.py
--rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink_cli/utils/player.py
--rw-r--r--   0 runner    (1001) docker     (127)    10391 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink_cli/utils/progress.py
--rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-04-14 15:40:22.000000 streamlink-6.7.3/src/streamlink_cli/utils/versioncheck.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:52.256392 streamlink-6.7.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:52.260392 streamlink-6.7.3/tests/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:52.260392 streamlink-6.7.3/tests/cli/output/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/cli/output/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/cli/output/test_file.py
--rw-r--r--   0 runner    (1001) docker     (127)    13144 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/cli/output/test_player.py
--rw-r--r--   0 runner    (1001) docker     (127)     7425 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/cli/test_argparser.py
--rw-r--r--   0 runner    (1001) docker     (127)     3775 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/cli/test_cmdline.py
--rw-r--r--   0 runner    (1001) docker     (127)     3928 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/cli/test_cmdline_title.py
--rw-r--r--   0 runner    (1001) docker     (127)     5018 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/cli/test_console.py
--rw-r--r--   0 runner    (1001) docker     (127)    18037 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/cli/test_main.py
--rw-r--r--   0 runner    (1001) docker     (127)     4446 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/cli/test_main_check_file_output.py
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/cli/test_main_formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)    16038 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/cli/test_main_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     7236 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/cli/test_main_setup_config_args.py
--rw-r--r--   0 runner    (1001) docker     (127)     4420 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/cli/test_plugin_args_and_options.py
--rw-r--r--   0 runner    (1001) docker     (127)    23211 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/cli/test_streamrunner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:52.260392 streamlink-6.7.3/tests/cli/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/cli/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3521 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/cli/utils/test_formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6167 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/cli/utils/test_path.py
--rw-r--r--   0 runner    (1001) docker     (127)     5367 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/cli/utils/test_player.py
--rw-r--r--   0 runner    (1001) docker     (127)    15076 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/cli/utils/test_progress.py
--rw-r--r--   0 runner    (1001) docker     (127)     6783 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/cli/utils/test_versioncheck.py
--rw-r--r--   0 runner    (1001) docker     (127)     3695 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:52.260392 streamlink-6.7.3/tests/mixins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10778 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/mixins/stream_hls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:52.260392 streamlink-6.7.3/tests/plugin/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:52.260392 streamlink-6.7.3/tests/plugin/override/
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugin/override/testplugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugin/testplugin.py
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugin/testplugin_invalid.py
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugin/testplugin_missing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:52.284392 streamlink-6.7.3/tests/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)     6265 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2736 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_abematv.py
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_adultswim.py
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_afreeca.py
--rw-r--r--   0 runner    (1001) docker     (127)     2617 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_albavision.py
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_aloula.py
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_app17.py
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_ard_live.py
--rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_ard_mediathek.py
--rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_artetv.py
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_atpchallenger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_atresplayer.py
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_bbciplayer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_bfmtv.py
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_bigo.py
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_bilibili.py
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_blazetv.py
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_bloomberg.py
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_booyah.py
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_brightcove.py
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_btv.py
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_cbsnews.py
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_cdnbg.py
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_ceskatelevize.py
--rw-r--r--   0 runner    (1001) docker     (127)      722 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_cinergroup.py
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_clubbingtv.py
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_cmmedia.py
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_cnews.py
--rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_crunchyroll.py
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_dailymotion.py
--rw-r--r--   0 runner    (1001) docker     (127)     4226 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_dash.py
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_delfi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_deutschewelle.py
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_dlive.py
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_dogan.py
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_dogus.py
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_drdk.py
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_earthcam.py
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_euronews.py
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_facebook.py
--rw-r--r--   0 runner    (1001) docker     (127)     3618 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_filmon.py
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_galatasaraytv.py
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_goltelevision.py
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_goodgame.py
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_googledrive.py
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_gulli.py
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_hiplayer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5329 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_hls.py
--rw-r--r--   0 runner    (1001) docker     (127)     2706 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_http.py
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_htv.py
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_huajiao.py
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_huya.py
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_idf1.py
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_indihometv.py
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_invintus.py
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_kugou.py
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_linelive.py
--rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_livestream.py
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_lnk.py
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_lrt.py
--rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_ltv_lsm_lv.py
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_mangomolo.py
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_mdstrm.py
--rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_mediaklikk.py
--rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_mediavitrina.py
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_mildom.py
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_mitele.py
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_mixcloud.py
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_mjunoon.py
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_mrtmk.py
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_n13tv.py
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_nasaplus.py
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_nhkworld.py
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_nicolive.py
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_nimotv.py
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_nos.py
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_nownews.py
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_nowtvtr.py
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_nrk.py
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_okru.py
--rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_olympicchannel.py
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_oneplusone.py
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_onetv.py
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_openrectv.py
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_pandalive.py
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_piaulizaportal.py
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_picarto.py
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_piczel.py
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_pixiv.py
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_pluto.py
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_pluzz.py
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_radiko.py
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_radionet.py
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_raiplay.py
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_reuters.py
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_rtpa.py
--rw-r--r--   0 runner    (1001) docker     (127)     2833 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_rtpplay.py
--rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_rtve.py
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_rtvs.py
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_ruv.py
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_sbscokr.py
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_showroom.py
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_sportal.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_sportschau.py
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_ssh101.py
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_stadium.py
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_steam.py
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_streamable.py
--rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_streann.py
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_stv.py
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_svtplay.py
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_swisstxt.py
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_telefe.py
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_telemadrid.py
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_tf1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_trovo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_turkuvaz.py
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_tv360.py
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_tv3cat.py
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_tv4play.py
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_tv5monde.py
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_tv8.py
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_tv999.py
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_tvibo.py
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_tviplayer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_tvp.py
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_tvrby.py
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_tvrplus.py
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_tvtoya.py
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_twitcasting.py
--rw-r--r--   0 runner    (1001) docker     (127)    35577 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_twitch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_ustreamtv.py
--rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_ustvnow.py
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_vidio.py
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_vimeo.py
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_vinhlongtv.py
--rw-r--r--   0 runner    (1001) docker     (127)     3013 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_vk.py
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_vkplay.py
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_vtvgo.py
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_webtv.py
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_welt.py
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_wwenetwork.py
--rw-r--r--   0 runner    (1001) docker     (127)     3347 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_youtube.py
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_yupptv.py
--rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_zattoo.py
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_zdf_mediathek.py
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_zeenews.py
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_zengatv.py
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/plugins/test_zhanqi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:52.284392 streamlink-6.7.3/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:52.200392 streamlink-6.7.3/tests/resources/cli/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:52.284392 streamlink-6.7.3/tests/resources/cli/config/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/resources/cli/config/custom
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/resources/cli/config/primary
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/resources/cli/config/primary.testplugin
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/resources/cli/config/secondary
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/resources/cli/config/secondary.testplugin
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:52.288392 streamlink-6.7.3/tests/resources/dash/
--rw-r--r--   0 runner    (1001) docker     (127)     4060 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/resources/dash/test_1.mpd
--rw-r--r--   0 runner    (1001) docker     (127)     4152 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/resources/dash/test_10.mpd
--rw-r--r--   0 runner    (1001) docker     (127)     9187 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/resources/dash/test_11_static.mpd
--rw-r--r--   0 runner    (1001) docker     (127)     6153 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/resources/dash/test_2.mpd
--rw-r--r--   0 runner    (1001) docker     (127)     2675 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/resources/dash/test_3.mpd
--rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/resources/dash/test_8.mpd
--rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/resources/dash/test_9.mpd
--rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/resources/dash/test_dynamic_segment_list_no_duration.mpd
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/resources/dash/test_dynamic_segment_list_p1.mpd
--rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/resources/dash/test_dynamic_segment_list_p2.mpd
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/resources/dash/test_dynamic_segment_list_p3.mpd
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/resources/dash/test_dynamic_segment_list_p4.mpd
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/resources/dash/test_dynamic_segment_list_p5.mpd
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/resources/dash/test_dynamic_timeline_continued_p1.mpd
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/resources/dash/test_dynamic_timeline_continued_p2.mpd
--rw-r--r--   0 runner    (1001) docker     (127)     2482 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/resources/dash/test_nested_baseurls.mpd
--rw-r--r--   0 runner    (1001) docker     (127)     2909 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/resources/dash/test_no_segment_list_or_template.mpd
--rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/resources/dash/test_segment_list.mpd
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/resources/dash/test_segments_byterange.mpd
--rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/resources/dash/test_segments_dynamic_number.mpd
--rw-r--r--   0 runner    (1001) docker     (127)     3874 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/resources/dash/test_static_no_publish_time.mpd
--rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/resources/dash/test_suggested_presentation_delay.mpd
--rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/resources/dash/test_timeline_ids.mpd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:52.288392 streamlink-6.7.3/tests/resources/hls/
--rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/resources/hls/test_1.m3u8
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/resources/hls/test_2.m3u8
--rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/resources/hls/test_date.m3u8
--rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/resources/hls/test_master.m3u8
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/resources/hls/test_master_twitch_vod.m3u8
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/resources/hls/test_multivariant_bandwidth.m3u8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:52.292392 streamlink-6.7.3/tests/session/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/session/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4846 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/session/test_http.py
--rw-r--r--   0 runner    (1001) docker     (127)    12344 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/session/test_options.py
--rw-r--r--   0 runner    (1001) docker     (127)    23380 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/session/test_plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)     9044 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/session/test_session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:52.292392 streamlink-6.7.3/tests/stream/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/stream/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:52.292392 streamlink-6.7.3/tests/stream/dash/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/stream/dash/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21720 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/stream/dash/test_dash.py
--rw-r--r--   0 runner    (1001) docker     (127)    29634 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/stream/dash/test_manifest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:52.292392 streamlink-6.7.3/tests/stream/hls/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/stream/hls/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    48313 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/stream/hls/test_hls.py
--rw-r--r--   0 runner    (1001) docker     (127)     8193 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/stream/hls/test_hls_filtered.py
--rw-r--r--   0 runner    (1001) docker     (127)    20206 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/stream/hls/test_m3u8.py
--rw-r--r--   0 runner    (1001) docker     (127)    18343 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/stream/test_ffmpegmux.py
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/stream/test_file.py
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/stream/test_segmented.py
--rw-r--r--   0 runner    (1001) docker     (127)     4211 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/stream/test_stream_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     3777 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/stream/test_stream_to_url.py
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/stream/test_stream_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (127)    49815 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/test_api_validate.py
--rw-r--r--   0 runner    (1001) docker     (127)     8905 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/test_api_websocket.py
--rw-r--r--   0 runner    (1001) docker     (127)     8023 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/test_buffers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5298 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     4637 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/test_compat.py
--rw-r--r--   0 runner    (1001) docker     (127)    11028 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    10047 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/test_options.py
--rw-r--r--   0 runner    (1001) docker     (127)    18714 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/test_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2689 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/test_plugin_userinput.py
--rw-r--r--   0 runner    (1001) docker     (127)     8080 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/test_plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/test_streamlink_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:52.292392 streamlink-6.7.3/tests/testutils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/testutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3395 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/testutils/handshake.py
--rw-r--r--   0 runner    (1001) docker     (127)     6803 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/testutils/test_handshake.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:52.296392 streamlink-6.7.3/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7616 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/utils/test_args.py
--rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/utils/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/utils/test_crypto.py
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/utils/test_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3050 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/utils/test_formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5743 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/utils/test_l10n.py
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/utils/test_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     7041 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/utils/test_named_pipe.py
--rw-r--r--   0 runner    (1001) docker     (127)     6102 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/utils/test_parse.py
--rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/utils/test_path.py
--rw-r--r--   0 runner    (1001) docker     (127)     8365 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/utils/test_processoutput.py
--rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/utils/test_random.py
--rw-r--r--   0 runner    (1001) docker     (127)     9308 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/utils/test_times.py
--rw-r--r--   0 runner    (1001) docker     (127)     5631 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/utils/test_url.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:52.296392 streamlink-6.7.3/tests/webbrowser/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/webbrowser/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:40:52.296392 streamlink-6.7.3/tests/webbrowser/cdp/
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/webbrowser/cdp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/webbrowser/cdp/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    39762 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/webbrowser/cdp/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    31342 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/webbrowser/cdp/test_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/webbrowser/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     8224 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/webbrowser/test_chromium.py
--rw-r--r--   0 runner    (1001) docker     (127)     6889 2024-04-14 15:40:22.000000 streamlink-6.7.3/tests/webbrowser/test_webbrowser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:17:37.655250 streamlink-6.7.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-12 11:17:09.000000 streamlink-6.7.4/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)   101586 2024-05-12 11:17:09.000000 streamlink-6.7.4/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-05-12 11:17:09.000000 streamlink-6.7.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-12 11:17:09.000000 streamlink-6.7.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6463 2024-05-12 11:17:37.655250 streamlink-6.7.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4486 2024-05-12 11:17:09.000000 streamlink-6.7.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:17:37.555251 streamlink-6.7.4/build_backend/
+-rw-r--r--   0 runner    (1001) docker     (127)     3370 2024-05-12 11:17:09.000000 streamlink-6.7.4/build_backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-05-12 11:17:09.000000 streamlink-6.7.4/build_backend/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3588 2024-05-12 11:17:09.000000 streamlink-6.7.4/build_backend/onbuild.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15924 2024-05-12 11:17:09.000000 streamlink-6.7.4/build_backend/plugins_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-05-12 11:17:09.000000 streamlink-6.7.4/build_backend/test_build_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3577 2024-05-12 11:17:09.000000 streamlink-6.7.4/build_backend/test_onbuild.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37280 2024-05-12 11:17:09.000000 streamlink-6.7.4/build_backend/test_plugins_json.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:17:37.547251 streamlink-6.7.4/completions/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:17:37.555251 streamlink-6.7.4/completions/bash/
+-rw-r--r--   0 runner    (1001) docker     (127)    10192 2024-05-12 11:17:32.000000 streamlink-6.7.4/completions/bash/streamlink
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:17:37.555251 streamlink-6.7.4/completions/zsh/
+-rw-r--r--   0 runner    (1001) docker     (127)    36756 2024-05-12 11:17:33.000000 streamlink-6.7.4/completions/zsh/_streamlink
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-12 11:17:09.000000 streamlink-6.7.4/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:17:37.559251 streamlink-6.7.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     5813 2024-05-12 11:17:09.000000 streamlink-6.7.4/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:17:37.547251 streamlink-6.7.4/docs/_build/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:17:37.559251 streamlink-6.7.4/docs/_build/man/
+-rw-r--r--   0 runner    (1001) docker     (127)    41634 2024-05-12 11:17:31.000000 streamlink-6.7.4/docs/_build/man/streamlink.1
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-05-12 11:17:09.000000 streamlink-6.7.4/docs/_man.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:17:37.559251 streamlink-6.7.4/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    12092 2024-05-12 11:17:09.000000 streamlink-6.7.4/docs/_static/apple-touch-icon.png
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-12 11:17:09.000000 streamlink-6.7.4/docs/_static/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-05-12 11:17:09.000000 streamlink-6.7.4/docs/_static/favicon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-05-12 11:17:09.000000 streamlink-6.7.4/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-05-12 11:17:09.000000 streamlink-6.7.4/docs/_static/icon-ffmpeg.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-12 11:17:09.000000 streamlink-6.7.4/docs/_static/icon-python.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    18593 2024-05-12 11:17:09.000000 streamlink-6.7.4/docs/_static/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    15790 2024-05-12 11:17:09.000000 streamlink-6.7.4/docs/_static/opengraph-image.png
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-05-12 11:17:09.000000 streamlink-6.7.4/docs/_static/site.webmanifest
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:17:37.563251 streamlink-6.7.4/docs/_static/styles/
+-rw-r--r--   0 runner    (1001) docker     (127)     7825 2024-05-12 11:17:09.000000 streamlink-6.7.4/docs/_static/styles/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:17:37.563251 streamlink-6.7.4/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-05-12 11:17:09.000000 streamlink-6.7.4/docs/_templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-05-12 11:17:09.000000 streamlink-6.7.4/docs/_templates/page.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:17:37.563251 streamlink-6.7.4/docs/_templates/sidebar/
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-05-12 11:17:09.000000 streamlink-6.7.4/docs/_templates/sidebar/brand.html
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-12 11:17:09.000000 streamlink-6.7.4/docs/_templates/sidebar/github-buttons.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:17:37.563251 streamlink-6.7.4/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-12 11:17:09.000000 streamlink-6.7.4/docs/api/cache.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-12 11:17:09.000000 streamlink-6.7.4/docs/api/exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-12 11:17:09.000000 streamlink-6.7.4/docs/api/options.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-12 11:17:09.000000 streamlink-6.7.4/docs/api/plugin.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-12 11:17:09.000000 streamlink-6.7.4/docs/api/session.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-12 11:17:09.000000 streamlink-6.7.4/docs/api/stream.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-12 11:17:09.000000 streamlink-6.7.4/docs/api/streamlink.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11275 2024-05-12 11:17:09.000000 streamlink-6.7.4/docs/api/validate.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-05-12 11:17:09.000000 streamlink-6.7.4/docs/api/webbrowser.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-12 11:17:09.000000 streamlink-6.7.4/docs/api.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:17:37.563251 streamlink-6.7.4/docs/api_guide/
+-rw-r--r--   0 runner    (1001) docker     (127)     4429 2024-05-12 11:17:09.000000 streamlink-6.7.4/docs/api_guide/quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    17250 2024-05-12 11:17:09.000000 streamlink-6.7.4/docs/api_guide/validate.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-12 11:17:09.000000 streamlink-6.7.4/docs/api_guide.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-12 11:17:09.000000 streamlink-6.7.4/docs/applications.rst
+-rw-r--r--   0 runner    (1001) docker     (127)   101586 2024-05-12 11:17:09.000000 streamlink-6.7.4/docs/changelog.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:17:37.563251 streamlink-6.7.4/docs/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     4530 2024-05-12 11:17:09.000000 streamlink-6.7.4/docs/cli/config.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3179 2024-05-12 11:17:09.000000 streamlink-6.7.4/docs/cli/metadata.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-05-12 11:17:09.000000 streamlink-6.7.4/docs/cli/plugin-sideloading.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:17:37.563251 streamlink-6.7.4/docs/cli/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-05-12 11:17:09.000000 streamlink-6.7.4/docs/cli/plugins/crunchyroll.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10202 2024-05-12 11:17:09.000000 streamlink-6.7.4/docs/cli/plugins/twitch.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-12 11:17:09.000000 streamlink-6.7.4/docs/cli/plugins.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3003 2024-05-12 11:17:09.000000 streamlink-6.7.4/docs/cli/protocols.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-12 11:17:09.000000 streamlink-6.7.4/docs/cli/proxy.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6882 2024-05-12 11:17:09.000000 streamlink-6.7.4/docs/cli/tutorial.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-12 11:17:09.000000 streamlink-6.7.4/docs/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7916 2024-05-12 11:17:09.000000 streamlink-6.7.4/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11426 2024-05-12 11:17:09.000000 streamlink-6.7.4/docs/deprecations.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10413 2024-05-12 11:17:09.000000 streamlink-6.7.4/docs/developing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-12 11:17:09.000000 streamlink-6.7.4/docs/docutils.conf
+-rw-r--r--   0 runner    (1001) docker     (127)     3013 2024-05-12 11:17:09.000000 streamlink-6.7.4/docs/donate.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6552 2024-05-12 11:17:09.000000 streamlink-6.7.4/docs/ext_argparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-05-12 11:17:09.000000 streamlink-6.7.4/docs/ext_github.py
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-12 11:17:09.000000 streamlink-6.7.4/docs/ext_html_template_vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8465 2024-05-12 11:17:09.000000 streamlink-6.7.4/docs/ext_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-05-12 11:17:09.000000 streamlink-6.7.4/docs/ext_releaseref.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-05-12 11:17:09.000000 streamlink-6.7.4/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    26139 2024-05-12 11:17:09.000000 streamlink-6.7.4/docs/install.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11739 2024-05-12 11:17:09.000000 streamlink-6.7.4/docs/migrations.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3401 2024-05-12 11:17:09.000000 streamlink-6.7.4/docs/players.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-12 11:17:09.000000 streamlink-6.7.4/docs/plugins.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3404 2024-05-12 11:17:09.000000 streamlink-6.7.4/docs/thirdparty.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-12 11:17:09.000000 streamlink-6.7.4/docs-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    18593 2024-05-12 11:17:09.000000 streamlink-6.7.4/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     6838 2024-05-12 11:17:37.659250 streamlink-6.7.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:17:37.563251 streamlink-6.7.4/script/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      802 2024-05-12 11:17:09.000000 streamlink-6.7.4/script/build-shell-completions.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 11:17:37.655250 streamlink-6.7.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3161 2024-05-12 11:17:37.659250 streamlink-6.7.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:17:37.551251 streamlink-6.7.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:17:37.567251 streamlink-6.7.4/src/streamlink/
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-12 11:17:37.659250 streamlink-6.7.4/src/streamlink/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3934 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/buffers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4918 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2661 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8007 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10961 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/options.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:17:37.567251 streamlink-6.7.4/src/streamlink/packages/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/packages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6194 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/packages/requests_file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:17:37.567251 streamlink-6.7.4/src/streamlink/plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:17:37.567251 streamlink-6.7.4/src/streamlink/plugin/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugin/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugin/api/http_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugin/api/useragents.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:17:37.571251 streamlink-6.7.4/src/streamlink/plugin/api/validate/
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugin/api/validate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugin/api/validate/_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13127 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugin/api/validate/_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11763 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugin/api/validate/_validate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19587 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugin/api/validate/_validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6614 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugin/api/websocket.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26032 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugin/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:17:37.595251 streamlink-6.7.4/src/streamlink/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9677 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/abematv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6520 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/adultswim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7884 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/afreeca.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5633 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/albavision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3896 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/aloula.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/app17.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/ard_live.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4769 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/ard_mediathek.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/artetv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/atpchallenger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3002 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/atresplayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8328 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/bbciplayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3956 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/bfmtv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/bigo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5642 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/bilibili.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3642 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/blazetv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4539 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/bloomberg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5014 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/booyah.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3737 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/brightcove.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/btv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/cbsnews.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3489 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/cdnbg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7082 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/ceskatelevize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6430 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/chzzk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/cinergroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2540 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/clubbingtv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3976 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/cmmedia.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/cnews.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14036 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/crunchyroll.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4264 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/dailymotion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/dash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4255 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/delfi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3514 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/deutschewelle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4468 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/dlive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5773 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/dogan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/dogus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/drdk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/earthcam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3504 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/euronews.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5512 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/facebook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8421 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/filmon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/galatasaraytv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/goltelevision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5307 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/goodgame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/googledrive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/gulli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/hiplayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/hls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/http.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/htv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2763 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/huajiao.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4227 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/huya.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/idf1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/indihometv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/invintus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/kugou.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/linelive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4493 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/livestream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/lnk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/lrt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/ltv_lsm_lv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/mangomolo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5255 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/mdstrm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/mediaklikk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3740 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/mediavitrina.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7100 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/mildom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4120 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/mitele.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/mixcloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5132 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/mjunoon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/mrtmk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4685 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/n13tv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/nasaplus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/nhkworld.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10573 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/nicolive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3671 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/nimotv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/nos.py
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/nowtvtr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3660 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/nrk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4564 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/okru.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/olympicchannel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4202 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/oneplusone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/onetv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5833 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/openrectv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3270 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/pandalive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/piaulizaportal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4779 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/picarto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/piczel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6543 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/pixiv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6981 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/pluto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5115 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/pluzz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3988 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/radiko.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/radionet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6447 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/raiplay.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3221 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/reuters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/rtpa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/rtpplay.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6597 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/rtve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/rtvs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3760 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/ruv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3265 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/sbscokr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2886 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/showroom.py
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/sportal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/sportschau.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/ssh101.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/stadium.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/steam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/streamable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5739 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/streann.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/stv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5355 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/svtplay.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/swisstxt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/telefe.py
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/telemadrid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/tf1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6625 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/trovo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4205 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/turkuvaz.py
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/tv360.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3625 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/tv3cat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/tv4play.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/tv5monde.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/tv8.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/tv999.py
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/tvibo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2625 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/tviplayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8870 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/tvp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/tvrby.py
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/tvrplus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/tvtoya.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6132 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/twitcasting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33591 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/twitch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19213 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/ustreamtv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5775 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/ustvnow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/vidio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8563 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/vimeo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/vinhlongtv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/vk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3347 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/vkplay.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/vtvgo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2647 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/webtv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/welt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4880 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/wwenetwork.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15401 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/youtube.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3871 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/yupptv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12860 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/zattoo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3435 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/zdf_mediathek.py
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/zeenews.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/zengatv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/plugins/zhanqi.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:17:37.595251 streamlink-6.7.4/src/streamlink/session/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/session/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9325 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/session/http.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12151 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/session/http.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    19101 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/session/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13238 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/session/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7495 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/session/session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:17:37.595251 streamlink-6.7.4/src/streamlink/stream/
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/stream/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:17:37.599251 streamlink-6.7.4/src/streamlink/stream/dash/
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/stream/dash/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14067 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/stream/dash/dash.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36858 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/stream/dash/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/stream/dash/segment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10466 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/stream/ffmpegmux.py
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/stream/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/stream/filtered.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:17:37.599251 streamlink-6.7.4/src/streamlink/stream/hls/
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/stream/hls/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33983 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/stream/hls/hls.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21481 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/stream/hls/m3u8.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/stream/hls/segment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/stream/http.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:17:37.599251 streamlink-6.7.4/src/streamlink/stream/segmented/
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/stream/segmented/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/stream/segmented/concurrent.py
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/stream/segmented/segment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8118 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/stream/segmented/segmented.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/stream/stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/stream/wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/user_input.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:17:37.603251 streamlink-6.7.4/src/streamlink/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3101 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/utils/args.py
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/utils/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/utils/crypto.py
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/utils/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/utils/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5655 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/utils/l10n.py
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/utils/module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3362 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/utils/named_pipe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3582 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/utils/parse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/utils/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/utils/processoutput.py
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/utils/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/utils/socket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3510 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/utils/times.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5367 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/utils/url.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:17:37.603251 streamlink-6.7.4/src/streamlink/webbrowser/
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/webbrowser/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:17:37.603251 streamlink-6.7.4/src/streamlink/webbrowser/cdp/
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/webbrowser/cdp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19581 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/webbrowser/cdp/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13939 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/webbrowser/cdp/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:17:37.607251 streamlink-6.7.4/src/streamlink/webbrowser/cdp/devtools/
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/webbrowser/cdp/devtools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21632 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/webbrowser/cdp/devtools/browser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49407 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/webbrowser/cdp/devtools/debugger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61679 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/webbrowser/cdp/devtools/dom.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26084 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/webbrowser/cdp/devtools/emulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19534 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/webbrowser/cdp/devtools/fetch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27632 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/webbrowser/cdp/devtools/input_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/webbrowser/cdp/devtools/inspector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3084 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/webbrowser/cdp/devtools/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)   130706 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/webbrowser/cdp/devtools/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)   107521 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/webbrowser/cdp/devtools/page.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62110 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/webbrowser/cdp/devtools/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17300 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/webbrowser/cdp/devtools/security.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24082 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/webbrowser/cdp/devtools/target.py
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/webbrowser/cdp/devtools/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/webbrowser/cdp/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8564 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/webbrowser/chromium.py
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/webbrowser/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5299 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink/webbrowser/webbrowser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:17:37.655250 streamlink-6.7.4/src/streamlink.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6463 2024-05-12 11:17:37.000000 streamlink-6.7.4/src/streamlink.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    19683 2024-05-12 11:17:37.000000 streamlink-6.7.4/src/streamlink.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 11:17:37.000000 streamlink-6.7.4/src/streamlink.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-12 11:17:37.000000 streamlink-6.7.4/src/streamlink.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-12 11:17:37.000000 streamlink-6.7.4/src/streamlink.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-12 11:17:37.000000 streamlink-6.7.4/src/streamlink.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:17:37.611250 streamlink-6.7.4/src/streamlink_cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink_cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink_cli/_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49425 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink_cli/argparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink_cli/compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2528 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink_cli/console.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink_cli/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink_cli/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32371 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink_cli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:17:37.611250 streamlink-6.7.4/src/streamlink_cli/output/
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink_cli/output/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink_cli/output/abc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink_cli/output/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3511 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink_cli/output/http.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10265 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink_cli/output/player.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink_cli/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     4918 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink_cli/streamrunner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:17:37.611250 streamlink-6.7.4/src/streamlink_cli/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink_cli/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink_cli/utils/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink_cli/utils/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink_cli/utils/player.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10391 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink_cli/utils/progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-05-12 11:17:09.000000 streamlink-6.7.4/src/streamlink_cli/utils/versioncheck.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:17:37.615251 streamlink-6.7.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:17:37.615251 streamlink-6.7.4/tests/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:17:37.615251 streamlink-6.7.4/tests/cli/output/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/cli/output/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/cli/output/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13144 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/cli/output/test_player.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7425 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/cli/test_argparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3775 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/cli/test_cmdline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3928 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/cli/test_cmdline_title.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4163 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/cli/test_console.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18122 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/cli/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4527 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/cli/test_main_check_file_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/cli/test_main_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16409 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/cli/test_main_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7236 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/cli/test_main_setup_config_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4420 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/cli/test_plugin_args_and_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23211 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/cli/test_streamrunner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:17:37.619251 streamlink-6.7.4/tests/cli/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/cli/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3521 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/cli/utils/test_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6167 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/cli/utils/test_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5367 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/cli/utils/test_player.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15076 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/cli/utils/test_progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6783 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/cli/utils/test_versioncheck.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3695 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:17:37.619251 streamlink-6.7.4/tests/mixins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10778 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/mixins/stream_hls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:17:37.619251 streamlink-6.7.4/tests/plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:17:37.619251 streamlink-6.7.4/tests/plugin/override/
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugin/override/testplugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugin/testplugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugin/testplugin_invalid.py
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugin/testplugin_missing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:17:37.643251 streamlink-6.7.4/tests/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)     6265 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2736 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_abematv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_adultswim.py
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_afreeca.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2617 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_albavision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_aloula.py
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_app17.py
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_ard_live.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_ard_mediathek.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_artetv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_atpchallenger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_atresplayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_bbciplayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_bfmtv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_bigo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_bilibili.py
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_blazetv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_bloomberg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_booyah.py
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_brightcove.py
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_btv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_cbsnews.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_cdnbg.py
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_ceskatelevize.py
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_chzzk.py
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_cinergroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_clubbingtv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_cmmedia.py
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_cnews.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_crunchyroll.py
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_dailymotion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4226 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_dash.py
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_delfi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_deutschewelle.py
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_dlive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_dogan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_dogus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_drdk.py
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_earthcam.py
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_euronews.py
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_facebook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3618 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_filmon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_galatasaraytv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_goltelevision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_goodgame.py
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_googledrive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_gulli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_hiplayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5329 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_hls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2706 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_http.py
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_htv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_huajiao.py
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_huya.py
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_idf1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_indihometv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_invintus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_kugou.py
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_linelive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_livestream.py
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_lnk.py
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_lrt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_ltv_lsm_lv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_mangomolo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_mdstrm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_mediaklikk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_mediavitrina.py
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_mildom.py
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_mitele.py
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_mixcloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_mjunoon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_mrtmk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_n13tv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_nasaplus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_nhkworld.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_nicolive.py
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_nimotv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_nos.py
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_nowtvtr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_nrk.py
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_okru.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_olympicchannel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_oneplusone.py
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_onetv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_openrectv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_pandalive.py
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_piaulizaportal.py
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_picarto.py
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_piczel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_pixiv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_pluto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_pluzz.py
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_radiko.py
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_radionet.py
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_raiplay.py
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_reuters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_rtpa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2833 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_rtpplay.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_rtve.py
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_rtvs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_ruv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_sbscokr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_showroom.py
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_sportal.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_sportschau.py
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_ssh101.py
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_stadium.py
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_steam.py
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_streamable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_streann.py
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_stv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_svtplay.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_swisstxt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_telefe.py
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_telemadrid.py
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_tf1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_trovo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_turkuvaz.py
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_tv360.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_tv3cat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_tv4play.py
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_tv5monde.py
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_tv8.py
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_tv999.py
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_tvibo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_tviplayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_tvp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_tvrby.py
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_tvrplus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_tvtoya.py
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_twitcasting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35577 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_twitch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_ustreamtv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_ustvnow.py
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_vidio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_vimeo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_vinhlongtv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3013 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_vk.py
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_vkplay.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_vtvgo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_webtv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_welt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_wwenetwork.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3347 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_youtube.py
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_yupptv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_zattoo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_zdf_mediathek.py
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_zeenews.py
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_zengatv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/plugins/test_zhanqi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:17:37.643251 streamlink-6.7.4/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:17:37.551251 streamlink-6.7.4/tests/resources/cli/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:17:37.643251 streamlink-6.7.4/tests/resources/cli/config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/resources/cli/config/custom
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/resources/cli/config/primary
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/resources/cli/config/primary.testplugin
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/resources/cli/config/secondary
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/resources/cli/config/secondary.testplugin
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:17:37.647251 streamlink-6.7.4/tests/resources/dash/
+-rw-r--r--   0 runner    (1001) docker     (127)     4060 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/resources/dash/test_1.mpd
+-rw-r--r--   0 runner    (1001) docker     (127)     4152 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/resources/dash/test_10.mpd
+-rw-r--r--   0 runner    (1001) docker     (127)     9187 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/resources/dash/test_11_static.mpd
+-rw-r--r--   0 runner    (1001) docker     (127)     6153 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/resources/dash/test_2.mpd
+-rw-r--r--   0 runner    (1001) docker     (127)     2675 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/resources/dash/test_3.mpd
+-rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/resources/dash/test_8.mpd
+-rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/resources/dash/test_9.mpd
+-rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/resources/dash/test_dynamic_segment_list_no_duration.mpd
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/resources/dash/test_dynamic_segment_list_p1.mpd
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/resources/dash/test_dynamic_segment_list_p2.mpd
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/resources/dash/test_dynamic_segment_list_p3.mpd
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/resources/dash/test_dynamic_segment_list_p4.mpd
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/resources/dash/test_dynamic_segment_list_p5.mpd
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/resources/dash/test_dynamic_timeline_continued_p1.mpd
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/resources/dash/test_dynamic_timeline_continued_p2.mpd
+-rw-r--r--   0 runner    (1001) docker     (127)     2482 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/resources/dash/test_nested_baseurls.mpd
+-rw-r--r--   0 runner    (1001) docker     (127)     2909 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/resources/dash/test_no_segment_list_or_template.mpd
+-rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/resources/dash/test_segment_list.mpd
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/resources/dash/test_segments_byterange.mpd
+-rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/resources/dash/test_segments_dynamic_number.mpd
+-rw-r--r--   0 runner    (1001) docker     (127)     3874 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/resources/dash/test_static_no_publish_time.mpd
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/resources/dash/test_suggested_presentation_delay.mpd
+-rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/resources/dash/test_timeline_ids.mpd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:17:37.647251 streamlink-6.7.4/tests/resources/hls/
+-rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/resources/hls/test_1.m3u8
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/resources/hls/test_2.m3u8
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/resources/hls/test_date.m3u8
+-rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/resources/hls/test_master.m3u8
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/resources/hls/test_master_twitch_vod.m3u8
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/resources/hls/test_multivariant_bandwidth.m3u8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:17:37.647251 streamlink-6.7.4/tests/session/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/session/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4846 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/session/test_http.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12344 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/session/test_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23380 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/session/test_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9044 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/session/test_session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:17:37.651250 streamlink-6.7.4/tests/stream/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/stream/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:17:37.651250 streamlink-6.7.4/tests/stream/dash/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/stream/dash/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21720 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/stream/dash/test_dash.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29634 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/stream/dash/test_manifest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:17:37.651250 streamlink-6.7.4/tests/stream/hls/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/stream/hls/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48313 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/stream/hls/test_hls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8193 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/stream/hls/test_hls_filtered.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20206 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/stream/hls/test_m3u8.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18343 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/stream/test_ffmpegmux.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/stream/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/stream/test_segmented.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4211 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/stream/test_stream_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3777 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/stream/test_stream_to_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/stream/test_stream_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49815 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/test_api_validate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8905 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/test_api_websocket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8023 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/test_buffers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5298 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4637 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/test_compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11028 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10047 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/test_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18714 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/test_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2689 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/test_plugin_userinput.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8080 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/test_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/test_streamlink_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:17:37.651250 streamlink-6.7.4/tests/testutils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/testutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3411 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/testutils/handshake.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6803 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/testutils/test_handshake.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:17:37.655250 streamlink-6.7.4/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7616 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/utils/test_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/utils/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/utils/test_crypto.py
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/utils/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3050 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/utils/test_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5743 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/utils/test_l10n.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/utils/test_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7041 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/utils/test_named_pipe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6102 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/utils/test_parse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/utils/test_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8365 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/utils/test_processoutput.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/utils/test_random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9308 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/utils/test_times.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5631 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/utils/test_url.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:17:37.655250 streamlink-6.7.4/tests/webbrowser/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/webbrowser/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:17:37.655250 streamlink-6.7.4/tests/webbrowser/cdp/
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/webbrowser/cdp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/webbrowser/cdp/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39759 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/webbrowser/cdp/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31345 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/webbrowser/cdp/test_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/webbrowser/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8252 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/webbrowser/test_chromium.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6863 2024-05-12 11:17:09.000000 streamlink-6.7.4/tests/webbrowser/test_webbrowser.py
```

### Comparing `streamlink-6.7.3/CHANGELOG.md` & `streamlink-6.7.4/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,27 @@
 # Changelog
 
+## streamlink 6.7.4 (2024-05-12)
+
+Patch release:
+
+- Refactored: CLI errors ([#5958](https://github.com/streamlink/streamlink/pull/5958))
+- Updated plugins:
+  - afreeca: updated stream qualities ([#5953](https://github.com/streamlink/streamlink/pull/5953))
+  - afreeca: added `--afreeca-stream-password` ([#5952](https://github.com/streamlink/streamlink/pull/5952))
+  - chzzk: new plugin ([#5731](https://github.com/streamlink/streamlink/pull/5731))
+  - nownews: removed plugin ([#5961](https://github.com/streamlink/streamlink/pull/5961))
+  - turkuvaz: fixed HLS streams ([#5946](https://github.com/streamlink/streamlink/pull/5946))
+- Docs: clarified plugin request rules ([#5949](https://github.com/streamlink/streamlink/pull/5949))
+- Build: fixed build issues on Windows ([#5990](https://github.com/streamlink/streamlink/pull/5990))
+- Build: removed `exceptiongroup` dependency on Python >= 3.11 ([#5987](https://github.com/streamlink/streamlink/pull/5987))
+
+[Full changelog](https://github.com/streamlink/streamlink/compare/6.7.3...6.7.4)
+
+
 ## streamlink 6.7.3 (2024-04-14)
 
 Patch release:
 
 - Fixed: file output paths being able to exceed max file/directory name length ([#5921](https://github.com/streamlink/streamlink/pull/5921), [#5925](https://github.com/streamlink/streamlink/pull/5925))
 - Fixed: propagation of `KeyboardInterrupt`/`SystemExit` in `streamlink.webbrowser` ([#5930](https://github.com/streamlink/streamlink/pull/5930))
 - Fixed: compatibility with `exceptiongroup<=1.1.1` ([#5930](https://github.com/streamlink/streamlink/pull/5930))
```

### Comparing `streamlink-6.7.3/LICENSE` & `streamlink-6.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/PKG-INFO` & `streamlink-6.7.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlink
-Version: 6.7.3
+Version: 6.7.4
 Summary: Streamlink is a command-line utility that extracts streams from various services and pipes them into a video player of choice.
 Author: Streamlink
 Author-email: streamlink@protonmail.com
 License: Simplified BSD
 Project-URL: Homepage, https://github.com/streamlink/streamlink
 Project-URL: Documentation, https://streamlink.github.io/
 Project-URL: Tracker, https://github.com/streamlink/streamlink/issues
@@ -28,15 +28,15 @@
 Classifier: Topic :: Multimedia :: Sound/Audio
 Classifier: Topic :: Multimedia :: Video
 Classifier: Topic :: Utilities
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: certifi
-Requires-Dist: exceptiongroup
+Requires-Dist: exceptiongroup; python_version < "3.11"
 Requires-Dist: isodate
 Requires-Dist: lxml<6,>=4.6.4
 Requires-Dist: pycountry
 Requires-Dist: pycryptodome<4,>=3.4.3
 Requires-Dist: PySocks!=1.5.7,>=1.5.6
 Requires-Dist: requests<3,>=2.26.0
 Requires-Dist: trio<1,>=0.22.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: streamlink Version: 6.7.3 Summary: Streamlink is a
+Metadata-Version: 2.1 Name: streamlink Version: 6.7.4 Summary: Streamlink is a
 command-line utility that extracts streams from various services and pipes them
 into a video player of choice. Author: Streamlink Author-email:
 streamlink@protonmail.com License: Simplified BSD Project-URL: Homepage, https:
 //github.com/streamlink/streamlink Project-URL: Documentation, https://
 streamlink.github.io/ Project-URL: Tracker, https://github.com/streamlink/
 streamlink/issues Project-URL: Source, https://github.com/streamlink/streamlink
 Project-URL: Funding, https://streamlink.github.io/latest/donate.html
@@ -14,20 +14,21 @@
 Programming Language :: Python :: 3 :: Only Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
 Topic :: Internet :: WWW/HTTP Classifier: Topic :: Multimedia :: Sound/Audio
 Classifier: Topic :: Multimedia :: Video Classifier: Topic :: Utilities
 Requires-Python: >=3.8 Description-Content-Type: text/markdown License-File:
-LICENSE Requires-Dist: certifi Requires-Dist: exceptiongroup Requires-Dist:
-isodate Requires-Dist: lxml<6,>=4.6.4 Requires-Dist: pycountry Requires-Dist:
-pycryptodome<4,>=3.4.3 Requires-Dist: PySocks!=1.5.7,>=1.5.6 Requires-Dist:
-requests<3,>=2.26.0 Requires-Dist: trio<1,>=0.22.0 Requires-Dist: trio-
-websocket<1,>=0.9.0 Requires-Dist: typing-extensions>=4.0.0 Requires-Dist:
-urllib3<3,>=1.26.0 Requires-Dist: websocket-client<2,>=1.2.1
+LICENSE Requires-Dist: certifi Requires-Dist: exceptiongroup; python_version <
+"3.11" Requires-Dist: isodate Requires-Dist: lxml<6,>=4.6.4 Requires-Dist:
+pycountry Requires-Dist: pycryptodome<4,>=3.4.3 Requires-Dist:
+PySocks!=1.5.7,>=1.5.6 Requires-Dist: requests<3,>=2.26.0 Requires-Dist:
+trio<1,>=0.22.0 Requires-Dist: trio-websocket<1,>=0.9.0 Requires-Dist: typing-
+extensions>=4.0.0 Requires-Dist: urllib3<3,>=1.26.0 Requires-Dist: websocket-
+client<2,>=1.2.1
                                ************ _SS_tt_rr_ee_aa_mm_ll_ii_nn_kk
                               _[[_SS_tt_rr_ee_aa_mm_ll_ii_nn_kk_]] ************
 _[_S_u_p_p_o_r_t_e_d_ _P_y_t_h_o_n_ _v_e_r_s_i_o_n_s_]_[_L_a_t_e_s_t_ _r_e_l_e_a_s_e_]_[_L_i_c_e_n_s_e_]_[_O_p_e_n_ _i_s_s_u_e_s_]_[_B_u_i_l_d_ _s_t_a_t_u_s_]
                             _[_O_v_e_r_a_l_l_ _c_o_d_e_ _c_o_v_e_r_a_g_e_]
  A Python library and command-line interface which pipes streams from various
                          services into a video player.
     Avoid resource-heavy and unoptimized websites, and still enjoy streamed
```

### Comparing `streamlink-6.7.3/README.md` & `streamlink-6.7.4/README.md`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/build_backend/__init__.py` & `streamlink-6.7.4/build_backend/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/build_backend/commands.py` & `streamlink-6.7.4/build_backend/commands.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/build_backend/onbuild.py` & `streamlink-6.7.4/build_backend/onbuild.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/build_backend/plugins_json.py` & `streamlink-6.7.4/build_backend/plugins_json.py`

 * *Files 1% similar despite different names*

```diff
@@ -439,15 +439,15 @@
 
 
 def build(pluginsdir: Path = DEFAULT_PLUGINSPATH) -> Output:
     data: Output = {}
     for file in pluginsdir.glob("*.py"):
         name = file.name
         plugin = re.sub(r"\.py$", "", name)
-        source = file.read_text()
+        source = file.read_text(encoding="utf-8")
 
         tree = ast.parse(source, str(file))
         visitor = PluginVisitor()
         try:
             visitor.visit(tree)
         except ParseError as err:
             raise SyntaxError(
```

### Comparing `streamlink-6.7.3/build_backend/test_build_backend.py` & `streamlink-6.7.4/build_backend/test_build_backend.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/build_backend/test_onbuild.py` & `streamlink-6.7.4/build_backend/test_onbuild.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/build_backend/test_plugins_json.py` & `streamlink-6.7.4/build_backend/test_plugins_json.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/completions/bash/streamlink` & `streamlink-6.7.4/completions/bash/streamlink`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # AUTOMATICALLY GENERATED by `shtab`
 
 
 
-_shtab_streamlink_cli_option_strings=('-h' '--help' '-V' '--version' '--plugins' '--plugin-dir' '--plugin-dirs' '--can-handle-url' '--can-handle-url-no-redirect' '--config' '--no-config' '-l' '--loglevel' '--logfile' '-Q' '--quiet' '-j' '--json' '--auto-version-check' '--version-check' '--locale' '--interface' '-4' '--ipv4' '-6' '--ipv6' '-p' '--player' '-a' '--player-args' '--player-env' '-v' '--verbose-player' '-n' '--player-fifo' '--fifo' '--player-http' '--player-continuous-http' '--player-external-http' '--player-external-http-continuous' '--player-external-http-interface' '--player-external-http-port' '--player-passthrough' '--player-no-close' '-t' '--title' '-o' '--output' '-O' '--stdout' '-r' '--record' '-R' '--record-and-pipe' '--fs-safe-rules' '-f' '--force' '--progress' '--force-progress' '--url' '--default-stream' '--stream-url' '--retry-streams' '--retry-max' '--retry-open' '--stream-types' '--stream-priority' '--stream-sorting-excludes' '--ringbuffer-size' '--stream-segment-attempts' '--stream-segment-threads' '--stream-segment-timeout' '--stream-timeout' '--mux-subtitles' '--hls-live-edge' '--hls-segment-stream-data' '--hls-playlist-reload-attempts' '--hls-playlist-reload-time' '--hls-segment-queue-threshold' '--hls-segment-ignore-names' '--hls-segment-key-uri' '--hls-audio-select' '--hls-start-offset' '--hls-duration' '--hls-live-restart' '--dash-manifest-reload-attempts' '--ffmpeg-ffmpeg' '--ffmpeg-no-validation' '--ffmpeg-verbose' '--ffmpeg-verbose-path' '--ffmpeg-fout' '--ffmpeg-video-transcode' '--ffmpeg-audio-transcode' '--ffmpeg-copyts' '--ffmpeg-start-at-zero' '--http-proxy' '--http-cookie' '--http-header' '--http-query-param' '--http-ignore-env' '--http-no-ssl-verify' '--http-disable-dh' '--http-ssl-cert' '--http-ssl-cert-crt-key' '--http-timeout' '--webbrowser' '--webbrowser-executable' '--webbrowser-timeout' '--webbrowser-cdp-host' '--webbrowser-cdp-port' '--webbrowser-cdp-timeout' '--webbrowser-headless' '--afreeca-username' '--afreeca-password' '--afreeca-purge-credentials' '--bbciplayer-username' '--bbciplayer-password' '--bbciplayer-hd' '--clubbingtv-username' '--clubbingtv-password' '--crunchyroll-username' '--crunchyroll-password' '--crunchyroll-purge-credentials' '--crunchyroll-session-id' '--niconico-email' '--niconico-password' '--niconico-user-session' '--niconico-purge-credentials' '--niconico-timeshift-offset' '--openrectv-email' '--openrectv-password' '--pixiv-sessionid' '--pixiv-devicetoken' '--pixiv-purge-credentials' '--pixiv-performer' '--raiplay-email' '--raiplay-password' '--raiplay-purge-credentials' '--steam-email' '--steam-password' '--streann-url' '--twitcasting-password' '--twitch-disable-ads' '--twitch-low-latency' '--twitch-api-header' '--twitch-access-token-param' '--twitch-purge-client-integrity' '--ustream-password' '--ustvnow-username' '--ustvnow-password' '--wwenetwork-email' '--wwenetwork-password' '--yupptv-boxid' '--yupptv-yuppflixtoken' '--yupptv-purge-credentials' '--zattoo-email' '--zattoo-password' '--zattoo-purge-credentials' '--zattoo-stream-types')
+_shtab_streamlink_cli_option_strings=('-h' '--help' '-V' '--version' '--plugins' '--plugin-dir' '--plugin-dirs' '--can-handle-url' '--can-handle-url-no-redirect' '--config' '--no-config' '-l' '--loglevel' '--logfile' '-Q' '--quiet' '-j' '--json' '--auto-version-check' '--version-check' '--locale' '--interface' '-4' '--ipv4' '-6' '--ipv6' '-p' '--player' '-a' '--player-args' '--player-env' '-v' '--verbose-player' '-n' '--player-fifo' '--fifo' '--player-http' '--player-continuous-http' '--player-external-http' '--player-external-http-continuous' '--player-external-http-interface' '--player-external-http-port' '--player-passthrough' '--player-no-close' '-t' '--title' '-o' '--output' '-O' '--stdout' '-r' '--record' '-R' '--record-and-pipe' '--fs-safe-rules' '-f' '--force' '--progress' '--force-progress' '--url' '--default-stream' '--stream-url' '--retry-streams' '--retry-max' '--retry-open' '--stream-types' '--stream-priority' '--stream-sorting-excludes' '--ringbuffer-size' '--stream-segment-attempts' '--stream-segment-threads' '--stream-segment-timeout' '--stream-timeout' '--mux-subtitles' '--hls-live-edge' '--hls-segment-stream-data' '--hls-playlist-reload-attempts' '--hls-playlist-reload-time' '--hls-segment-queue-threshold' '--hls-segment-ignore-names' '--hls-segment-key-uri' '--hls-audio-select' '--hls-start-offset' '--hls-duration' '--hls-live-restart' '--dash-manifest-reload-attempts' '--ffmpeg-ffmpeg' '--ffmpeg-no-validation' '--ffmpeg-verbose' '--ffmpeg-verbose-path' '--ffmpeg-fout' '--ffmpeg-video-transcode' '--ffmpeg-audio-transcode' '--ffmpeg-copyts' '--ffmpeg-start-at-zero' '--http-proxy' '--http-cookie' '--http-header' '--http-query-param' '--http-ignore-env' '--http-no-ssl-verify' '--http-disable-dh' '--http-ssl-cert' '--http-ssl-cert-crt-key' '--http-timeout' '--webbrowser' '--webbrowser-executable' '--webbrowser-timeout' '--webbrowser-cdp-host' '--webbrowser-cdp-port' '--webbrowser-cdp-timeout' '--webbrowser-headless' '--afreeca-username' '--afreeca-password' '--afreeca-purge-credentials' '--afreeca-stream-password' '--bbciplayer-username' '--bbciplayer-password' '--bbciplayer-hd' '--clubbingtv-username' '--clubbingtv-password' '--crunchyroll-username' '--crunchyroll-password' '--crunchyroll-purge-credentials' '--crunchyroll-session-id' '--niconico-email' '--niconico-password' '--niconico-user-session' '--niconico-purge-credentials' '--niconico-timeshift-offset' '--openrectv-email' '--openrectv-password' '--pixiv-sessionid' '--pixiv-devicetoken' '--pixiv-purge-credentials' '--pixiv-performer' '--raiplay-email' '--raiplay-password' '--raiplay-purge-credentials' '--steam-email' '--steam-password' '--streann-url' '--twitcasting-password' '--twitch-disable-ads' '--twitch-low-latency' '--twitch-api-header' '--twitch-access-token-param' '--twitch-purge-client-integrity' '--ustream-password' '--ustvnow-username' '--ustvnow-password' '--wwenetwork-email' '--wwenetwork-password' '--yupptv-boxid' '--yupptv-yuppflixtoken' '--yupptv-purge-credentials' '--zattoo-email' '--zattoo-password' '--zattoo-purge-credentials' '--zattoo-stream-types')
 
 
 
 _shtab_streamlink_cli__l_choices=('none' 'critical' 'error' 'warning' 'info' 'debug' 'trace' 'all')
 _shtab_streamlink_cli___loglevel_choices=('none' 'critical' 'error' 'warning' 'info' 'debug' 'trace' 'all')
 _shtab_streamlink_cli___fs_safe_rules_choices=('POSIX' 'Windows')
 _shtab_streamlink_cli___progress_choices=('yes' 'force' 'no')
```

### Comparing `streamlink-6.7.3/completions/zsh/_streamlink` & `streamlink-6.7.4/completions/zsh/_streamlink`

 * *Files 0% similar despite different names*

```diff
@@ -702,14 +702,15 @@
         When enabled, it stays completely hidden and doesn\'t require a desktop environment to run.
 
         Default is true.
         ]:webbrowser_headless:"
   "--afreeca-username[The username used to register with afreecatv.com.]:afreeca_username:"
   "--afreeca-password[A afreecatv.com account password to use with --afreeca-username.]:afreeca_password:"
   "--afreeca-purge-credentials[Purge cached AfreecaTV credentials to initiate a new session and reauthenticate.]"
+  "--afreeca-stream-password[The password for the stream.]:afreeca_stream_password:"
   "--bbciplayer-username[The username used to register with bbc.co.uk.]:bbciplayer_username:"
   "--bbciplayer-password[A bbc.co.uk account password to use with --bbciplayer-username.]:bbciplayer_password:"
   "--bbciplayer-hd[Prefer HD streams over local SD streams, some live programmes may not be broadcast in HD.]"
   "--clubbingtv-username[The username used to register with Clubbing TV.]:clubbingtv_username:"
   "--clubbingtv-password[A Clubbing TV account password to use with --clubbingtv-username.]:clubbingtv_password:"
   "--crunchyroll-username[A Crunchyroll username to allow access to restricted streams.]:crunchyroll_username:"
   "--crunchyroll-password[
```

### Comparing `streamlink-6.7.3/docs/Makefile` & `streamlink-6.7.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/docs/_build/man/streamlink.1` & `streamlink-6.7.4/docs/_build/man/streamlink.1`

 * *Files 4% similar despite different names*

```diff
@@ -23,44 +23,40 @@
 . RE
 .\" indent \\n[an-margin]
 .\" old: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .nr rst2man-indent-level -1
 .\" new: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .in \\n[rst2man-indent\\n[rst2man-indent-level]]u
 ..
-.TH "STREAMLINK" "1" "Apr 14, 2024" "6.7.3" "Streamlink"
+.TH "STREAMLINK" "1" "May 12, 2024" "6.7.4" "Streamlink"
 .SH NAME
 streamlink \- extracts streams from various services and pipes them into a video player of choice
 .SH SYNOPSIS
 .INDENT 0.0
 .INDENT 3.5
 .sp
-.nf
-.ft C
+.EX
 streamlink [OPTIONS] <URL> [STREAM]
-.ft P
-.fi
+.EE
 .UNINDENT
 .UNINDENT
 .SH EXAMPLES
 .INDENT 0.0
 .INDENT 3.5
 .sp
-.nf
-.ft C
+.EX
 streamlink \-\-loglevel debug youtu.be/VIDEO\-ID best
 streamlink \-\-player mpv \-\-player\-args \(aq\-\-no\-border \-\-no\-keepaspect\-window\(aq twitch.tv/CHANNEL 1080p60
 streamlink \-\-player\-external\-http \-\-player\-external\-http\-port 8888 URL STREAM
 streamlink \-\-output /path/to/file \-\-http\-timeout 60 URL STREAM
 streamlink \-\-stdout URL STREAM | ffmpeg \-i pipe:0 ...
 streamlink \-\-http\-header \(aqAuthorization=OAuth TOKEN\(aq \-\-http\-header \(aqReferer=URL\(aq URL STREAM
 streamlink \-\-hls\-live\-edge 5 \-\-stream\-segment\-threads 5 \(aqhls://https://host/playlist.m3u8\(aq best
 streamlink \-\-twitch\-low\-latency \-p mpv \-a \(aq\-\-cache=yes \-\-demuxer\-max\-back\-bytes=2G\(aq twitch.tv/CHANNEL best
-.ft P
-.fi
+.EE
 .UNINDENT
 .UNINDENT
 .SH OPTIONS
 .SS Positional arguments
 .INDENT 0.0
 .TP
 .B URL
@@ -79,19 +75,17 @@
 Use \fBbest\fP or \fBworst\fP for selecting the highest or lowest available
 quality.
 .sp
 Fallback streams can be specified by using a comma\-separated list:
 .INDENT 7.0
 .INDENT 3.5
 .sp
-.nf
-.ft C
+.EX
 \(dq720p,480p,best\(dq
-.ft P
-.fi
+.EE
 .UNINDENT
 .UNINDENT
 .sp
 If no stream is specified and \fI\%\-\-default\-stream\fP is not used, then a list
 of available streams will be printed.
 .UNINDENT
 .SS General options
@@ -177,43 +171,37 @@
 A value of \fB\-\fP (dash) will set the file name to an ISO8601\-like string
 and will choose the following default log directories.
 .sp
 Windows:
 .INDENT 7.0
 .INDENT 3.5
 .sp
-.nf
-.ft C
+.EX
 %TEMP%\estreamlink\elogs
-.ft P
-.fi
+.EE
 .UNINDENT
 .UNINDENT
 .sp
 macOS:
 .INDENT 7.0
 .INDENT 3.5
 .sp
-.nf
-.ft C
+.EX
 ${HOME}/Library/Logs/streamlink
-.ft P
-.fi
+.EE
 .UNINDENT
 .UNINDENT
 .sp
 Linux/BSD:
 .INDENT 7.0
 .INDENT 3.5
 .sp
-.nf
-.ft C
+.EX
 ${XDG_STATE_HOME:\-${HOME}/.local/state}/streamlink/logs
-.ft P
-.fi
+.EE
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
 .B \-Q
 .TP
@@ -319,19 +307,17 @@
 If unset, automatically generated player title arguments will be prepended to the parsed player arguments list.
 .UNINDENT
 .sp
 Example:
 .INDENT 7.0
 .INDENT 3.5
 .sp
-.nf
-.ft C
+.EX
 streamlink \-p vlc \-a \(dq\-\-play\-and\-exit \-\-no\-one\-instance\(dq <url> [stream]
-.ft P
-.fi
+.EE
 .UNINDENT
 .UNINDENT
 .sp
 Default is: \fB\(dq\(dq\fP\&.
 .UNINDENT
 .INDENT 0.0
 .TP
@@ -448,40 +434,38 @@
 .INDENT 0.0
 .TP
 .B \-t TITLE
 .TP
 .B \-\-title TITLE
 Change the title of the video player\(aqs window.
 .sp
-Please see the \(dq\fI\%Metadata variables\fP\(dq section of Streamlink\(aqs CLI documentation for all available metadata variables,
-as well as the \(dq\fI\%Plugins\fP\(dq section for the list of metadata variables defined in each plugin.
+Please see the \(dq\X'tty: link #variables'\fI\%Metadata variables\fP\X'tty: link'\(dq section of Streamlink\(aqs CLI documentation for all available metadata variables,
+as well as the \(dq\X'tty: link #plugins'\fI\%Plugins\fP\X'tty: link'\(dq section for the list of metadata variables defined in each plugin.
 .sp
 This option is only supported for the following players: mpv, potplayer, vlc
 .INDENT 7.0
 .TP
 .B VLC specific information:
 VLC does support special formatting variables on its own:
-\fI\%https://wiki.videolan.org/Documentation:Format_String/\fP
+\X'tty: link https://wiki.videolan.org/Documentation:Format_String/'\fI\%https://wiki.videolan.org/Documentation:Format_String/\fP\X'tty: link'
 .sp
 These variables are accessible in the \fI\%\-\-title\fP option by adding a backslash
 in front of the dollar sign which VLC uses as its formatting character.
 .sp
 For example, to put the current date in your VLC window title,
 the string \fB\e$A\fP could be inserted inside the \fI\%\-\-title\fP string.
 .UNINDENT
 .sp
 Example:
 .INDENT 7.0
 .INDENT 3.5
 .sp
-.nf
-.ft C
+.EX
 streamlink \-p mpv \-\-title \(dq{author} \- {category} \- {title}\(dq <URL> [STREAM]
-.ft P
-.fi
+.EE
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .SS File output options
 .INDENT 0.0
 .TP
 .B \-o FILENAME
@@ -490,28 +474,26 @@
 Write stream data to \fBFILENAME\fP instead of playing it. If \fBFILENAME\fP is set to \fB\-\fP (dash), then the stream data will be
 written to stdout, similar to the \fI\%\-\-stdout\fP argument.
 .sp
 Non\-existent directories and subdirectories will be created if they do not exist, if filesystem permissions allow.
 .sp
 You will be prompted if the file already exists.
 .sp
-Please see the \(dq\fI\%Metadata variables\fP\(dq section of Streamlink\(aqs CLI documentation for all available metadata variables,
-as well as the \(dq\fI\%Plugins\fP\(dq section for the list of metadata variables defined in each plugin.
+Please see the \(dq\X'tty: link #variables'\fI\%Metadata variables\fP\X'tty: link'\(dq section of Streamlink\(aqs CLI documentation for all available metadata variables,
+as well as the \(dq\X'tty: link #plugins'\fI\%Plugins\fP\X'tty: link'\(dq section for the list of metadata variables defined in each plugin.
 .sp
 Unsupported characters in substituted variables will be replaced with an underscore.
 .sp
 Example:
 .INDENT 7.0
 .INDENT 3.5
 .sp
-.nf
-.ft C
+.EX
 streamlink \-\-output \(dq~/recordings/{author}/{category}/{id}\-{time:%Y%m%d%H%M%S}.ts\(dq <URL> [STREAM]
-.ft P
-.fi
+.EE
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
 .B \-O
 .TP
@@ -526,56 +508,52 @@
 Open the stream in the player, while at the same time writing it to \fBFILENAME\fP\&. If \fBFILENAME\fP is set to \fB\-\fP (dash),
 then the stream data will be written to stdout, similar to the \fI\%\-\-stdout\fP argument, while still opening the player.
 .sp
 Non\-existent directories and subdirectories will be created if they do not exist, if filesystem permissions allow.
 .sp
 You will be prompted if the file already exists.
 .sp
-Please see the \(dq\fI\%Metadata variables\fP\(dq section of Streamlink\(aqs CLI documentation for all available metadata variables,
-as well as the \(dq\fI\%Plugins\fP\(dq section for the list of metadata variables defined in each plugin.
+Please see the \(dq\X'tty: link #variables'\fI\%Metadata variables\fP\X'tty: link'\(dq section of Streamlink\(aqs CLI documentation for all available metadata variables,
+as well as the \(dq\X'tty: link #plugins'\fI\%Plugins\fP\X'tty: link'\(dq section for the list of metadata variables defined in each plugin.
 .sp
 Unsupported characters in substituted variables will be replaced with an underscore.
 .sp
 Example:
 .INDENT 7.0
 .INDENT 3.5
 .sp
-.nf
-.ft C
+.EX
 streamlink \-\-record \(dq~/recordings/{author}/{category}/{id}\-{time:%Y%m%d%H%M%S}.ts\(dq <URL> [STREAM]
-.ft P
-.fi
+.EE
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
 .B \-R FILENAME
 .TP
 .B \-\-record\-and\-pipe FILENAME
 Write stream data to stdout, while at the same time writing it to \fBFILENAME\fP\&.
 .sp
 Non\-existent directories and subdirectories will be created if they do not exist, if filesystem permissions allow.
 .sp
 You will be prompted if the file already exists.
 .sp
-Please see the \(dq\fI\%Metadata variables\fP\(dq section of Streamlink\(aqs CLI documentation for all available metadata variables,
-as well as the \(dq\fI\%Plugins\fP\(dq section for the list of metadata variables defined in each plugin.
+Please see the \(dq\X'tty: link #variables'\fI\%Metadata variables\fP\X'tty: link'\(dq section of Streamlink\(aqs CLI documentation for all available metadata variables,
+as well as the \(dq\X'tty: link #plugins'\fI\%Plugins\fP\X'tty: link'\(dq section for the list of metadata variables defined in each plugin.
 .sp
 Unsupported characters in substituted variables will be replaced with an underscore.
 .sp
 Example:
 .INDENT 7.0
 .INDENT 3.5
 .sp
-.nf
-.ft C
+.EX
 streamlink \-\-record\-and\-pipe \(dq~/recordings/{author}/{category}/{id}\-{time:%Y%m%d%H%M%S}.ts\(dq <URL> [STREAM]
-.ft P
-.fi
+.EE
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
 .B \-\-fs\-safe\-rules
 The rules used to make formatting variables filesystem\-safe are chosen
@@ -633,19 +611,17 @@
 Use \fBbest\fP or \fBworst\fP for selecting the highest or lowest available
 quality.
 .sp
 Fallback streams can be specified by using a comma\-separated list:
 .INDENT 7.0
 .INDENT 3.5
 .sp
-.nf
-.ft C
+.EX
 \(dq720p,480p,best\(dq
-.ft P
-.fi
+.EE
 .UNINDENT
 .UNINDENT
 .sp
 This is an alternative to setting the stream using a positional argument
 and can be useful if set in a config file.
 .UNINDENT
 .INDENT 0.0
@@ -702,48 +678,42 @@
 inaccessible and new special stream synonyms \fBbest\-unfiltered\fP and \fBworst\-unfiltered\fP
 can be used as a fallback selection method.
 .sp
 Uses a filter expression in the format:
 .INDENT 7.0
 .INDENT 3.5
 .sp
-.nf
-.ft C
+.EX
 [operator]<value>
-.ft P
-.fi
+.EE
 .UNINDENT
 .UNINDENT
 .sp
 Valid operators are \fB>\fP, \fB>=\fP, \fB<\fP and \fB<=\fP\&. If no operator is specified then
 equality is tested.
 .sp
 For example this will exclude streams ranked higher than \(dq480p\(dq:
 .INDENT 7.0
 .INDENT 3.5
 .sp
-.nf
-.ft C
+.EX
 \-\-stream\-sorting\-excludes \(dq>480p\(dq
-.ft P
-.fi
+.EE
 .UNINDENT
 .UNINDENT
 .sp
 Multiple filters can be used by separating each expression with a comma.
 .sp
 For example this will exclude streams from two quality types:
 .INDENT 7.0
 .INDENT 3.5
 .sp
-.nf
-.ft C
+.EX
 \-\-stream\-sorting\-excludes \(dq>480p,>medium\(dq
-.ft P
-.fi
+.EE
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .SS Stream transport options
 .INDENT 0.0
 .TP
 .B \-\-ringbuffer\-size SIZE
@@ -889,33 +859,29 @@
 Override the segment encryption key URIs for encrypted streams.
 .sp
 The value can be templated using the following variables, which will be
 replaced with their respective part from the source segment URI:
 .INDENT 7.0
 .INDENT 3.5
 .sp
-.nf
-.ft C
+.EX
 {url} {scheme} {netloc} {path} {query}
-.ft P
-.fi
+.EE
 .UNINDENT
 .UNINDENT
 .sp
 Examples:
 .INDENT 7.0
 .INDENT 3.5
 .sp
-.nf
-.ft C
+.EX
 \-\-hls\-segment\-key\-uri \(dqhttps://example.com/hls/encryption_key\(dq
 \-\-hls\-segment\-key\-uri \(dq{scheme}://1.2.3.4{path}{query}\(dq
 \-\-hls\-segment\-key\-uri \(dq{scheme}://{netloc}/custom/path/to/key\(dq
-.ft P
-.fi
+.EE
 .UNINDENT
 .UNINDENT
 .sp
 Default is: \fBNone\fP\&.
 .UNINDENT
 .INDENT 0.0
 .TP
@@ -924,21 +890,19 @@
 when multiple audio sources are available. Can be \fB*\fP (asterisk) to download all
 audio sources.
 .sp
 Examples:
 .INDENT 7.0
 .INDENT 3.5
 .sp
-.nf
-.ft C
+.EX
 \-\-hls\-audio\-select \(dqEnglish,German\(dq
 \-\-hls\-audio\-select \(dqen,de\(dq
 \-\-hls\-audio\-select \(dq*\(dq
-.ft P
-.fi
+.EE
 .UNINDENT
 .UNINDENT
 .sp
 \fBNOTE:\fP
 .INDENT 7.0
 .INDENT 3.5
 This is only useful in special circumstances where the regular
@@ -1181,14 +1145,19 @@
 A afreecatv.com account password to use with \fI\%\-\-afreeca\-username\fP\&.
 .UNINDENT
 .INDENT 0.0
 .TP
 .B \-\-afreeca\-purge\-credentials
 Purge cached AfreecaTV credentials to initiate a new session and reauthenticate.
 .UNINDENT
+.INDENT 0.0
+.TP
+.B \-\-afreeca\-stream\-password STREAM_PASSWORD
+The password for the stream.
+.UNINDENT
 .SS Bbciplayer
 .INDENT 0.0
 .TP
 .B \-\-bbciplayer\-username USERNAME
 The username used to register with bbc.co.uk.
 .UNINDENT
 .INDENT 0.0
@@ -1464,24 +1433,24 @@
 .sp
 Default is: \fB\(dqdash\(dq\fP\&.
 .UNINDENT
 .SH BUGS
 .sp
 Please open a new issue on Streamlink\(aqs issue tracker on GitHub and use the appropriate issue forms:
 .sp
-\fI\%https://github.com/streamlink/streamlink/issues\fP
+\X'tty: link https://github.com/streamlink/streamlink/issues'\fI\%https://github.com/streamlink/streamlink/issues\fP\X'tty: link'
 .SH SEE ALSO
 .sp
 For more detailed information about config files, plugin sideloading, streaming protocols, proxy support, metadata,
 or plugin specific stuff, please see Streamlink\(aqs online CLI documentation here:
 .sp
-\fI\%https://streamlink.github.io/cli.html\fP
+\X'tty: link https://streamlink.github.io/cli.html'\fI\%https://streamlink.github.io/cli.html\fP\X'tty: link'
 .sp
 The list of available plugins and their descriptions can be found here:
 .sp
-\fI\%https://streamlink.github.io/plugins.html\fP
+\X'tty: link https://streamlink.github.io/plugins.html'\fI\%https://streamlink.github.io/plugins.html\fP\X'tty: link'
 .SH AUTHOR
 Streamlink Contributors
 .SH COPYRIGHT
 2024, Streamlink
 .\" Generated by docutils manpage writer.
 .
```

### Comparing `streamlink-6.7.3/docs/_man.rst` & `streamlink-6.7.4/docs/_man.rst`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/docs/_static/apple-touch-icon.png` & `streamlink-6.7.4/docs/_static/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/docs/_static/favicon-16x16.png` & `streamlink-6.7.4/docs/_static/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/docs/_static/favicon-32x32.png` & `streamlink-6.7.4/docs/_static/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/docs/_static/favicon.ico` & `streamlink-6.7.4/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/docs/_static/icon-ffmpeg.svg` & `streamlink-6.7.4/docs/_static/icon-ffmpeg.svg`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/docs/_static/icon-python.svg` & `streamlink-6.7.4/docs/_static/icon-python.svg`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/docs/_static/icon.svg` & `streamlink-6.7.4/docs/_static/icon.svg`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/docs/_static/opengraph-image.png` & `streamlink-6.7.4/docs/_static/opengraph-image.png`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/docs/_static/styles/custom.css` & `streamlink-6.7.4/docs/_static/styles/custom.css`

 * *Files 2% similar despite different names*

```diff
@@ -292,15 +292,21 @@
   Content
 */
 
 .installation-grid .fab {
   font-size: 5em;
 }
 
-.grid-with-icons .fas {
+.grid-with-icons .sd-card-header .fas {
+  width: 1em;
+  margin-left: -1.25em;
+  margin-right: .25em;
+}
+
+.grid-with-icons .sd-card-body .fas {
   padding-right: 0.1em;
   font-size: 1.75em;
   vertical-align: middle;
 }
 
 .grid-with-images img {
   width: auto;
```

### Comparing `streamlink-6.7.3/docs/_templates/base.html` & `streamlink-6.7.4/docs/_templates/base.html`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/docs/_templates/sidebar/brand.html` & `streamlink-6.7.4/docs/_templates/sidebar/brand.html`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/docs/_templates/sidebar/github-buttons.html` & `streamlink-6.7.4/docs/_templates/sidebar/github-buttons.html`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/docs/api/validate.rst` & `streamlink-6.7.4/docs/api/validate.rst`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/docs/api/webbrowser.rst` & `streamlink-6.7.4/docs/api/webbrowser.rst`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/docs/api_guide/quickstart.rst` & `streamlink-6.7.4/docs/api_guide/quickstart.rst`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/docs/api_guide/validate.rst` & `streamlink-6.7.4/docs/api_guide/validate.rst`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/docs/applications.rst` & `streamlink-6.7.4/docs/applications.rst`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/docs/changelog.md` & `streamlink-6.7.4/docs/changelog.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,27 @@
 # Changelog
 
+## streamlink 6.7.4 (2024-05-12)
+
+Patch release:
+
+- Refactored: CLI errors ([#5958](https://github.com/streamlink/streamlink/pull/5958))
+- Updated plugins:
+  - afreeca: updated stream qualities ([#5953](https://github.com/streamlink/streamlink/pull/5953))
+  - afreeca: added `--afreeca-stream-password` ([#5952](https://github.com/streamlink/streamlink/pull/5952))
+  - chzzk: new plugin ([#5731](https://github.com/streamlink/streamlink/pull/5731))
+  - nownews: removed plugin ([#5961](https://github.com/streamlink/streamlink/pull/5961))
+  - turkuvaz: fixed HLS streams ([#5946](https://github.com/streamlink/streamlink/pull/5946))
+- Docs: clarified plugin request rules ([#5949](https://github.com/streamlink/streamlink/pull/5949))
+- Build: fixed build issues on Windows ([#5990](https://github.com/streamlink/streamlink/pull/5990))
+- Build: removed `exceptiongroup` dependency on Python >= 3.11 ([#5987](https://github.com/streamlink/streamlink/pull/5987))
+
+[Full changelog](https://github.com/streamlink/streamlink/compare/6.7.3...6.7.4)
+
+
 ## streamlink 6.7.3 (2024-04-14)
 
 Patch release:
 
 - Fixed: file output paths being able to exceed max file/directory name length ([#5921](https://github.com/streamlink/streamlink/pull/5921), [#5925](https://github.com/streamlink/streamlink/pull/5925))
 - Fixed: propagation of `KeyboardInterrupt`/`SystemExit` in `streamlink.webbrowser` ([#5930](https://github.com/streamlink/streamlink/pull/5930))
 - Fixed: compatibility with `exceptiongroup<=1.1.1` ([#5930](https://github.com/streamlink/streamlink/pull/5930))
```

### Comparing `streamlink-6.7.3/docs/cli/config.rst` & `streamlink-6.7.4/docs/cli/config.rst`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/docs/cli/metadata.rst` & `streamlink-6.7.4/docs/cli/metadata.rst`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/docs/cli/plugin-sideloading.rst` & `streamlink-6.7.4/docs/cli/plugin-sideloading.rst`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/docs/cli/plugins/crunchyroll.rst` & `streamlink-6.7.4/docs/cli/plugins/crunchyroll.rst`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/docs/cli/plugins/twitch.rst` & `streamlink-6.7.4/docs/cli/plugins/twitch.rst`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/docs/cli/protocols.rst` & `streamlink-6.7.4/docs/cli/protocols.rst`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/docs/cli/proxy.rst` & `streamlink-6.7.4/docs/cli/proxy.rst`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/docs/cli/tutorial.rst` & `streamlink-6.7.4/docs/cli/tutorial.rst`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/docs/cli.rst` & `streamlink-6.7.4/docs/cli.rst`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/docs/conf.py` & `streamlink-6.7.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/docs/deprecations.rst` & `streamlink-6.7.4/docs/deprecations.rst`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/docs/developing.rst` & `streamlink-6.7.4/docs/developing.rst`

 * *Files 0% similar despite different names*

```diff
@@ -101,15 +101,15 @@
 
     # run automated tests
     pytest
     # or just run a subset of all tests
     pytest path/to/test-file.py::TestClassName::test_method_name ...
 
     # check code for linting errors
-    ruff .
+    ruff check
     # check code for typing errors
     mypy
 
     # build the documentation
     make --directory=docs clean html
     $BROWSER ./docs/_build/html/index.html
```

### Comparing `streamlink-6.7.3/docs/donate.rst` & `streamlink-6.7.4/docs/donate.rst`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/docs/ext_argparse.py` & `streamlink-6.7.4/docs/ext_argparse.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/docs/ext_github.py` & `streamlink-6.7.4/docs/ext_github.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/docs/ext_plugins.py` & `streamlink-6.7.4/docs/ext_plugins.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/docs/ext_releaseref.py` & `streamlink-6.7.4/docs/ext_releaseref.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/docs/index.rst` & `streamlink-6.7.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/docs/install.rst` & `streamlink-6.7.4/docs/install.rst`

 * *Files 4% similar despite different names*

```diff
@@ -132,20 +132,18 @@
       - Installing
     * - :octicon:`verified` AppImage
       - See the `Linux AppImages`_ section below
     * - :octicon:`verified` AppImage nightly builds
       - See the `Linux AppImages`_ section below
     * - :octicon:`verified` Python pip
       - See the `PyPI package and source code`_ section below
-    * - :octicon:`package-dependents` `Alpine Linux (edge, testing)`_
+    * - :octicon:`package-dependents` `ALT Linux (Sisyphus)`_
       - .. code-block:: bash
 
-            sudo apk add streamlink
-
-        `Enabling the edge/testing repository`_
+            sudo apt-get install streamlink
     * - :octicon:`package-dependents` `Arch Linux`_
       - .. code-block:: bash
 
             sudo pacman -S streamlink
     * - :octicon:`package-dependents` `Arch Linux (aur, git)`_
       - .. code-block:: bash
 
@@ -197,45 +195,49 @@
       - .. code-block:: bash
 
             sudo zypper install streamlink
     * - :octicon:`package-dependents` `Solus`_
       - .. code-block:: bash
 
             sudo eopkg install streamlink
+    * - :octicon:`package-dependents` `Void`_
+      - .. code-block:: bash
+
+            sudo xbps-install streamlink
 
-.. _Alpine Linux (edge, testing): https://pkgs.alpinelinux.org/packages?name=streamlink
+.. _ALT Linux (Sisyphus): https://packages.altlinux.org/en/sisyphus/srpms/streamlink/
 .. _Arch Linux: https://archlinux.org/packages/extra/any/streamlink/
 .. _Arch Linux (aur, git): https://aur.archlinux.org/packages/streamlink-git/
 .. _Debian (sid, testing): https://packages.debian.org/sid/streamlink
 .. _Debian (stable): https://packages.debian.org/bookworm-backports/streamlink
 .. _Fedora: https://src.fedoraproject.org/rpms/python-streamlink
 .. _FreeBSD (pkg): https://ports.freebsd.org/cgi/ports.cgi?query=streamlink&stype=name
 .. _FreeBSD (ports): https://www.freshports.org/multimedia/streamlink
 .. _Gentoo Linux: https://packages.gentoo.org/package/net-misc/streamlink
 .. _NixOS: https://github.com/NixOS/nixpkgs/tree/master/pkgs/applications/video/streamlink
 .. _openSUSE: https://build.opensuse.org/package/show/multimedia:apps/streamlink
 .. _Solus: https://github.com/getsolus/packages/tree/main/packages/s/streamlink
+.. _Void: https://github.com/void-linux/void-packages/tree/master/srcpkgs/streamlink
 
-.. _Enabling the edge/testing repository: https://wiki.alpinelinux.org/wiki/Repositories#Edge
 .. _Installing AUR packages: https://wiki.archlinux.org/index.php/Arch_User_Repository
 .. _Installing Debian backported packages: https://wiki.debian.org/Backports
 .. _NixOS channel: https://search.nixos.org/packages?show=streamlink&query=streamlink
 
 
 Package maintainers
 -------------------
 
 .. list-table::
     :header-rows: 1
     :class: table-custom-layout
 
     * - Distribution / Platform
       - Maintainer
-    * - Alpine Linux
-      - Robert Sacks <robert at sacks.email>
+    * - ALT Linux
+      - Vitaly Lipatov <lav at altlinux.ru>
     * - Arch
       - Giancarlo Razzolini <grazzolini at archlinux.org>
     * - Arch (aur, git)
       - Josip Ponjavic <josipponjavic at gmail.com>
     * - Chocolatey
       - Scott Walters <me at scowalt.com>
     * - Debian
@@ -248,14 +250,16 @@
       - soredake <fdsfgs at krutt.org>
     * - NixOS
       - Tuomas Tynkkynen <tuomas.tynkkynen at iki.fi>
     * - openSUSE
       - Simon Puchert <simonpuchert at alice.de>
     * - Solus
       - Joey Riches <josephriches at gmail.com>
+    * - Void
+      - Tom Strausbaugh <tstrausbaugh at straustech.net>
     * - Windows binaries
       - Sebastian Meyer <mail at bastimeyer.de>
     * - Linux AppImages
       - Sebastian Meyer <mail at bastimeyer.de>
 
 
 Package availability
@@ -440,15 +444,16 @@
         Used for generating the version string from git when building, or when running in an editable install.
         Not needed when building wheels and installing from the source distribution.
     * - runtime
       - `certifi`_
       - Used for loading the CA bundle extracted from the Mozilla Included CA Certificate List
     * - runtime
       - `exceptiongroup`_
-      - Used for ``ExceptionGroup`` handling, to allow writing compatible code on all supported Python versions
+      - Only required when ``python_version<"3.11"`` |br|
+        Used for ``ExceptionGroup`` handling
     * - runtime
       - `isodate`_
       - Used for parsing ISO8601 strings
     * - runtime
       - `lxml`_
       - Used for processing HTML and XML data
     * - runtime
@@ -541,39 +546,91 @@
         ^^^
         :fas:`download` GitHub actions build artifacts
 
         Built once each day at midnight UTC |br| :sub:`GitHub account required`
 
 **Flavors**
 
-.. list-table::
-    :header-rows: 2
-    :stub-columns: 1
-    :width: 100%
-
-    * -
-      - Installer
-      -
-      - Portable
-      -
-    * -
-      - 64 bit
-      - 32 bit
-      - 64 bit
-      - 32 bit
-    * - Latest Python
-      - :bdg-link-success-line:`Windows 10+ <https://github.com/streamlink/windows-builds/releases>`
-      - :bdg-link-primary-line:`Windows 10+ <https://github.com/streamlink/windows-builds/releases>`
-      - :bdg-link-success-line:`Windows 10+ <https://github.com/streamlink/windows-builds/releases>`
-      - :bdg-link-primary-line:`Windows 10+ <https://github.com/streamlink/windows-builds/releases>`
-    * - Python 3.8
-      - :bdg-link-secondary-line:`Windows 7 <https://github.com/streamlink/windows-builds/releases>`
-      - :bdg-link-secondary-line:`Windows 7 <https://github.com/streamlink/windows-builds/releases>`
-      - :bdg-link-secondary-line:`Windows 7 <https://github.com/streamlink/windows-builds/releases>`
-      - :bdg-link-secondary-line:`Windows 7 <https://github.com/streamlink/windows-builds/releases>`
+.. grid:: 2
+    :padding: 0
+    :class-container: grid-with-icons
+
+    .. grid-item-card::
+        :padding: 3
+        :class-header: sd-text-center
+        :class-footer: sd-text-center sd-bg-transparent sd-border-0
+
+        :fas:`gears` **Installer**
+        ^^^
+
+        - Adds itself to the system's ``PATH`` env var
+        - Automatically creates a :ref:`config file <cli/config:Configuration file>`
+        - Sets :option:`--ffmpeg-ffmpeg` in config file
+
+        +++
+        .. grid:: 2
+            :gutter: 1
+            :padding: 0
+
+            .. grid-item::
+                :class: sd-text-right
+
+                Windows 10+
+
+            .. grid-item::
+
+                :bdg-link-success-line:`x86_64 <https://github.com/streamlink/windows-builds/releases>`
+                :bdg-link-primary-line:`x86 <https://github.com/streamlink/windows-builds/releases>`
+
+            .. grid-item::
+                :class: sd-text-right
+
+                Windows 7 (py38)
+
+            .. grid-item::
+
+                :bdg-link-secondary-line:`x86_64 <https://github.com/streamlink/windows-builds/releases>`
+                :bdg-link-secondary-line:`x86 <https://github.com/streamlink/windows-builds/releases>`
+
+    .. grid-item-card::
+        :padding: 3
+        :class-header: sd-text-center
+        :class-footer: sd-text-center sd-bg-transparent sd-border-0
+
+        :fas:`file-zipper` **Portable archive**
+        ^^^
+
+        - No :ref:`config file <cli/config:Configuration file>` created automatically
+        - :option:`--ffmpeg-ffmpeg` must be set manually
+        - No pre-compiled Python bytecode
+
+        +++
+        .. grid:: 2
+            :gutter: 1
+            :padding: 0
+
+            .. grid-item::
+                :class: sd-text-right
+
+                Windows 10+
+
+            .. grid-item::
+
+                :bdg-link-success-line:`x86_64 <https://github.com/streamlink/windows-builds/releases>`
+                :bdg-link-primary-line:`x86 <https://github.com/streamlink/windows-builds/releases>`
+
+            .. grid-item::
+                :class: sd-text-right
+
+                Windows 7 (py38)
+
+            .. grid-item::
+
+                :bdg-link-secondary-line:`x86_64 <https://github.com/streamlink/windows-builds/releases>`
+                :bdg-link-secondary-line:`x86 <https://github.com/streamlink/windows-builds/releases>`
 
 **Contents**
 
 .. grid:: 3
     :padding: 0
     :class-container: grid-with-images
 
@@ -606,25 +663,14 @@
         :text-align: center
 
         .. image:: _static/icon-ffmpeg.svg
             :alt: FFmpeg
 
         FFmpeg |br| :sub:`for muxing streams`
 
-.. note::
-
-   The installers automatically create a :ref:`config file <cli/config:Configuration file>` if it doesn't exist yet and set the
-   value of the :option:`--ffmpeg-ffmpeg` CLI parameter to the path of the included FFmpeg binary. The portable archives
-   can't do that, and users need to create or update the config file themselves.
-
-   :fas:`triangle-exclamation` Please see the README of the `streamlink/windows-builds`_ repository for more information
-   about the differences between the installers and portable archives.
-
-.. _streamlink/windows-builds: https://github.com/streamlink/windows-builds
-
 
 Linux AppImages
 ---------------
 
 .. grid:: 2
     :padding: 0
     :class-container: grid-with-icons
```

### Comparing `streamlink-6.7.3/docs/migrations.rst` & `streamlink-6.7.4/docs/migrations.rst`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/docs/players.rst` & `streamlink-6.7.4/docs/players.rst`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/docs/plugins.rst` & `streamlink-6.7.4/docs/plugins.rst`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/docs/thirdparty.rst` & `streamlink-6.7.4/docs/thirdparty.rst`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/icon.svg` & `streamlink-6.7.4/icon.svg`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/pyproject.toml` & `streamlink-6.7.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,15 @@
   "scripts",
   "gui-scripts",
 ]
 
 requires-python = ">=3.8"
 dependencies = [
   "certifi",
-  "exceptiongroup",
+  "exceptiongroup ; python_version<'3.11'",
   "isodate",
   "lxml >=4.6.4,<6",
   "pycountry",
   "pycryptodome >=3.4.3,<4",
   "PySocks >=1.5.6,!=1.5.7",
   "requests >=2.26.0,<3",
   "trio >=0.22.0,<1",
```

### Comparing `streamlink-6.7.3/script/build-shell-completions.sh` & `streamlink-6.7.4/script/build-shell-completions.sh`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/setup.py` & `streamlink-6.7.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,9 +86,9 @@
         def get_cmdclasses(_):  # type: ignore[misc]
             return _
 
     setup(
         cmdclass=get_cmdclasses(cmdclass),
         entry_points=entry_points,
         data_files=data_files,
-        version="6.7.3",
+        version="6.7.4",
     )
```

### Comparing `streamlink-6.7.3/src/streamlink/__init__.py` & `streamlink-6.7.4/src/streamlink/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/api.py` & `streamlink-6.7.4/src/streamlink/api.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/buffers.py` & `streamlink-6.7.4/src/streamlink/buffers.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/cache.py` & `streamlink-6.7.4/src/streamlink/cache.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/compat.py` & `streamlink-6.7.4/src/streamlink/compat.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 import importlib
 import inspect
 import os
 import sys
 import warnings
 from typing import Any, Callable, Dict, Optional, Tuple
 
-# import exceptiongroup, so it can monkeypatch ExceptionGroup logic on <=py311
-import exceptiongroup  # noqa: F401
+
+try:
+    from builtins import BaseExceptionGroup, ExceptionGroup  # type: ignore[attr-defined]
+except ImportError:  # pragma: no cover
+    from exceptiongroup import BaseExceptionGroup, ExceptionGroup  # type: ignore[import]
+
 
 from streamlink.exceptions import StreamlinkDeprecationWarning
 
 
 # compatibility import of charset_normalizer/chardet via requests<3.0
 try:
     from requests.compat import chardet as charset_normalizer  # type: ignore
@@ -68,12 +72,14 @@
     # delete the deprecated module attributes and the imported `deprecated` function
     for item in items.keys() | [deprecated.__name__]:
         if item in mod_globals:
             del mod_globals[item]
 
 
 __all__ = [
+    "BaseExceptionGroup",
+    "ExceptionGroup",
     "deprecated",
     "detect_encoding",
     "is_darwin",
     "is_win32",
 ]
```

### Comparing `streamlink-6.7.3/src/streamlink/exceptions.py` & `streamlink-6.7.4/src/streamlink/exceptions.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/logger.py` & `streamlink-6.7.4/src/streamlink/logger.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/options.py` & `streamlink-6.7.4/src/streamlink/options.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/packages/requests_file.py` & `streamlink-6.7.4/src/streamlink/packages/requests_file.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugin/__init__.py` & `streamlink-6.7.4/src/streamlink/plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugin/api/useragents.py` & `streamlink-6.7.4/src/streamlink/plugin/api/useragents.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-ANDROID = "Mozilla/5.0 (Linux; Android 14) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/123.0.6312.80 Mobile Safari/537.36"
-CHROME = "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/123.0.0.0 Safari/537.36"
+ANDROID = "Mozilla/5.0 (Linux; Android 14) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/124.0.6367.82 Mobile Safari/537.36"
+CHROME = "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/124.0.0.0 Safari/537.36"
 CHROME_OS = "Mozilla/5.0 (X11; CrOS x86_64 15633.69.0) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/119.0.6045.212 Safari/537.36"
-FIREFOX = "Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:124.0) Gecko/20100101 Firefox/124.0"
+FIREFOX = "Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:125.0) Gecko/20100101 Firefox/125.0"
 IE_11 = "Mozilla/5.0 (Windows NT 10.0; WOW64; Trident/7.0; rv:11.0) like Gecko"
-IPHONE = "Mozilla/5.0 (iPhone; CPU iPhone OS 17_4_1 like Mac OS X) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/17.3.1 Mobile/15E148 Safari/604.1"
-OPERA = "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/123.0.0.0 Safari/537.36 OPR/109.0.0.0"
-SAFARI = "Mozilla/5.0 (Macintosh; Intel Mac OS X 14_4_1) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/17.3.1 Safari/605.1.15"
+IPHONE = "Mozilla/5.0 (iPhone; CPU iPhone OS 17_4_1 like Mac OS X) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/17.4.1 Mobile/15E148 Safari/604.1"
+OPERA = "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/124.0.0.0 Safari/537.36 OPR/109.0.0.0"
+SAFARI = "Mozilla/5.0 (Macintosh; Intel Mac OS X 14_4_1) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/17.4.1 Safari/605.1.15"
 
 # Backwards compatibility
 EDGE = CHROME
 FIREFOX_MAC = FIREFOX
 IE_6 = IE_7 = IE_8 = IE_9 = IE_11
 IPHONE_6 = IPAD = IPHONE
 SAFARI_7 = SAFARI_8 = SAFARI
```

### Comparing `streamlink-6.7.3/src/streamlink/plugin/api/validate/__init__.py` & `streamlink-6.7.4/src/streamlink/plugin/api/validate/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugin/api/validate/_exception.py` & `streamlink-6.7.4/src/streamlink/plugin/api/validate/_exception.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugin/api/validate/_schemas.py` & `streamlink-6.7.4/src/streamlink/plugin/api/validate/_schemas.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugin/api/validate/_validate.py` & `streamlink-6.7.4/src/streamlink/plugin/api/validate/_validate.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugin/api/validate/_validators.py` & `streamlink-6.7.4/src/streamlink/plugin/api/validate/_validators.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugin/api/websocket.py` & `streamlink-6.7.4/src/streamlink/plugin/api/websocket.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugin/plugin.py` & `streamlink-6.7.4/src/streamlink/plugin/plugin.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/abematv.py` & `streamlink-6.7.4/src/streamlink/plugins/abematv.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/adultswim.py` & `streamlink-6.7.4/src/streamlink/plugins/adultswim.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/afreeca.py` & `streamlink-6.7.4/src/streamlink/plugins/afreeca.py`

 * *Files 11% similar despite different names*

```diff
@@ -48,37 +48,41 @@
     help="A afreecatv.com account password to use with --afreeca-username.",
 )
 @pluginargument(
     "purge-credentials",
     action="store_true",
     help="Purge cached AfreecaTV credentials to initiate a new session and reauthenticate.",
 )
+@pluginargument(
+    "stream-password",
+    metavar="STREAM_PASSWORD",
+    help="The password for the stream.",
+)
 class AfreecaTV(Plugin):
     _re_bno = re.compile(r"window\.nBroadNo\s*=\s*(?P<bno>\d+);")
 
     CHANNEL_API_URL = "https://live.afreecatv.com/afreeca/player_live_api.php"
     CHANNEL_RESULT_OK = 1
-    QUALITYS = ["original", "hd", "sd"]
-    QUALITY_WEIGHTS = {
-        "original": 1080,
-        "hd": 720,
-        "sd": 480,
-    }
+    CHANNEL_LOGIN_REQUIRED = -6
 
     _schema_channel = validate.Schema(
         {
             "CHANNEL": {
                 "RESULT": validate.transform(int),
                 validate.optional("BPWD"): validate.any(str, None),
                 validate.optional("BNO"): validate.any(str, None),
                 validate.optional("RMD"): validate.any(str, None),
                 validate.optional("AID"): validate.any(str, None),
                 validate.optional("CDN"): validate.any(str, None),
                 validate.optional("BJNICK"): validate.any(str, None),
                 validate.optional("TITLE"): validate.any(str, None),
+                validate.optional("VIEWPRESET"): [{
+                    "label": str,
+                    "name": str,
+                }],
             },
         },
         validate.get("CHANNEL"),
     )
     _schema_stream = validate.Schema(
         {
             validate.optional("view_url"): validate.url(
@@ -94,44 +98,36 @@
             self.session.http.cookies.get("PdboxBbs")
             and self.session.http.cookies.get("PdboxSaveTicket")
             and self.session.http.cookies.get("PdboxTicket")
             and self.session.http.cookies.get("PdboxUser")
             and self.session.http.cookies.get("RDB")
         )
 
-    @classmethod
-    def stream_weight(cls, key):
-        weight = cls.QUALITY_WEIGHTS.get(key)
-        if weight:
-            return weight, "afreeca"
-
-        return Plugin.stream_weight(key)
-
     def _get_channel_info(self, broadcast, username):
         data = {
             "bid": username,
             "bno": broadcast,
             "from_api": "0",
             "mode": "landing",
             "player_type": "html5",
             "pwd": "",
             "stream_type": "common",
             "type": "live",
         }
         res = self.session.http.post(self.CHANNEL_API_URL, data=data)
         return self.session.http.json(res, schema=self._schema_channel)
 
-    def _get_hls_key(self, broadcast, username, quality):
+    def _get_hls_key(self, broadcast, username, quality, stream_password):
         data = {
             "bid": username,
             "bno": broadcast,
             "from_api": "0",
             "mode": "landing",
             "player_type": "html5",
-            "pwd": "",
+            "pwd": stream_password or "",
             "quality": quality,
             "stream_type": "common",
             "type": "aid",
         }
         res = self.session.http.post(self.CHANNEL_API_URL, data=data)
         return self.session.http.json(res, schema=self._schema_channel)
 
@@ -139,16 +135,16 @@
         params = {
             "return_type": "gs_cdn_pc_web",
             "broad_key": f"{broadcast}-common-{quality}-hls",
         }
         res = self.session.http.get(f"{rmd}/broad_stream_assign.html", params=params)
         return self.session.http.json(res, schema=self._schema_stream)
 
-    def _get_hls_stream(self, broadcast, username, quality, rmd):
-        keyjson = self._get_hls_key(broadcast, username, quality)
+    def _get_hls_stream(self, broadcast, username, quality, rmd, stream_password):
+        keyjson = self._get_hls_key(broadcast, username, quality, stream_password)
 
         if keyjson.get("RESULT") != self.CHANNEL_RESULT_OK:
             return
         key = keyjson.get("AID")
 
         info = self._get_stream_info(broadcast, quality, rmd)
 
@@ -173,14 +169,15 @@
             return False
         self.save_cookies()
         return True
 
     def _get_streams(self):
         login_username = self.get_option("username")
         login_password = self.get_option("password")
+        stream_password = self.get_option("stream-password")
 
         self.session.http.headers.update({"Referer": self.url, "Origin": "https://play.afreecatv.com"})
 
         if self.options.get("purge_credentials"):
             self.clear_cookies()
             self._authed = False
             log.info("All credentials were successfully removed")
@@ -203,31 +200,36 @@
             if not m:
                 log.error("Could not find broadcast number.")
                 return
             bno = m.group("bno")
 
         channel = self._get_channel_info(bno, username)
         log.trace(f"{channel!r}")
-        if channel.get("BPWD") == "Y":
-            log.error("Stream is Password-Protected")
-            return
-        elif channel.get("RESULT") == -6:
+        if channel.get("RESULT") == self.CHANNEL_LOGIN_REQUIRED:
             log.error("Login required")
             return
-        elif channel.get("RESULT") != self.CHANNEL_RESULT_OK:
+        if channel.get("RESULT") != self.CHANNEL_RESULT_OK:
             return
 
         (broadcast, rmd) = (channel.get("BNO"), channel.get("RMD"))
         if not (broadcast and rmd):
             return
 
         self.id = channel.get("BNO")
         self.author = channel.get("BJNICK")
         self.title = channel.get("TITLE")
 
-        for qkey in self.QUALITYS:
-            hls_stream = self._get_hls_stream(broadcast, username, qkey, rmd)
-            if hls_stream:
-                yield qkey, hls_stream
+        streams = {}
+        for item in channel.get("VIEWPRESET"):
+            if item["name"] == "auto":
+                continue
+            if hls_stream := self._get_hls_stream(broadcast, username, item["name"], rmd, stream_password):
+                streams[item["label"]] = hls_stream
+
+        if not streams and channel.get("BPWD") == "Y":
+            log.error("Stream is password protected")
+            return
+
+        return streams
 
 
 __plugin__ = AfreecaTV
```

### Comparing `streamlink-6.7.3/src/streamlink/plugins/albavision.py` & `streamlink-6.7.4/src/streamlink/plugins/albavision.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/aloula.py` & `streamlink-6.7.4/src/streamlink/plugins/aloula.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/app17.py` & `streamlink-6.7.4/src/streamlink/plugins/app17.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/ard_live.py` & `streamlink-6.7.4/src/streamlink/plugins/ard_live.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/ard_mediathek.py` & `streamlink-6.7.4/src/streamlink/plugins/ard_mediathek.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/artetv.py` & `streamlink-6.7.4/src/streamlink/plugins/artetv.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/atpchallenger.py` & `streamlink-6.7.4/src/streamlink/plugins/atpchallenger.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/atresplayer.py` & `streamlink-6.7.4/src/streamlink/plugins/atresplayer.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/bbciplayer.py` & `streamlink-6.7.4/src/streamlink/plugins/bbciplayer.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/bfmtv.py` & `streamlink-6.7.4/src/streamlink/plugins/bfmtv.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/bigo.py` & `streamlink-6.7.4/src/streamlink/plugins/bigo.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/bilibili.py` & `streamlink-6.7.4/src/streamlink/plugins/bilibili.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/blazetv.py` & `streamlink-6.7.4/src/streamlink/plugins/blazetv.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/bloomberg.py` & `streamlink-6.7.4/src/streamlink/plugins/bloomberg.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/booyah.py` & `streamlink-6.7.4/src/streamlink/plugins/booyah.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/brightcove.py` & `streamlink-6.7.4/src/streamlink/plugins/brightcove.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/btv.py` & `streamlink-6.7.4/src/streamlink/plugins/btv.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/cbsnews.py` & `streamlink-6.7.4/src/streamlink/plugins/cbsnews.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/cdnbg.py` & `streamlink-6.7.4/src/streamlink/plugins/cdnbg.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/ceskatelevize.py` & `streamlink-6.7.4/src/streamlink/plugins/ceskatelevize.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/cinergroup.py` & `streamlink-6.7.4/src/streamlink/plugins/cinergroup.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/clubbingtv.py` & `streamlink-6.7.4/src/streamlink/plugins/clubbingtv.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/cmmedia.py` & `streamlink-6.7.4/src/streamlink/plugins/cmmedia.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/cnews.py` & `streamlink-6.7.4/src/streamlink/plugins/cnews.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/crunchyroll.py` & `streamlink-6.7.4/src/streamlink/plugins/crunchyroll.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/dailymotion.py` & `streamlink-6.7.4/src/streamlink/plugins/dailymotion.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/dash.py` & `streamlink-6.7.4/src/streamlink/plugins/dash.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/delfi.py` & `streamlink-6.7.4/src/streamlink/plugins/delfi.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/deutschewelle.py` & `streamlink-6.7.4/src/streamlink/plugins/deutschewelle.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/dlive.py` & `streamlink-6.7.4/src/streamlink/plugins/dlive.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/dogan.py` & `streamlink-6.7.4/src/streamlink/plugins/dogan.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/dogus.py` & `streamlink-6.7.4/src/streamlink/plugins/dogus.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/drdk.py` & `streamlink-6.7.4/src/streamlink/plugins/drdk.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/earthcam.py` & `streamlink-6.7.4/src/streamlink/plugins/earthcam.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/euronews.py` & `streamlink-6.7.4/src/streamlink/plugins/euronews.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/facebook.py` & `streamlink-6.7.4/src/streamlink/plugins/facebook.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/filmon.py` & `streamlink-6.7.4/src/streamlink/plugins/filmon.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/galatasaraytv.py` & `streamlink-6.7.4/src/streamlink/plugins/galatasaraytv.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/goltelevision.py` & `streamlink-6.7.4/src/streamlink/plugins/goltelevision.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/goodgame.py` & `streamlink-6.7.4/src/streamlink/plugins/goodgame.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/googledrive.py` & `streamlink-6.7.4/src/streamlink/plugins/googledrive.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/gulli.py` & `streamlink-6.7.4/src/streamlink/plugins/gulli.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/hiplayer.py` & `streamlink-6.7.4/src/streamlink/plugins/hiplayer.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/hls.py` & `streamlink-6.7.4/src/streamlink/plugins/hls.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/http.py` & `streamlink-6.7.4/src/streamlink/plugins/http.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/htv.py` & `streamlink-6.7.4/src/streamlink/plugins/htv.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/huajiao.py` & `streamlink-6.7.4/src/streamlink/plugins/huajiao.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/huya.py` & `streamlink-6.7.4/src/streamlink/plugins/huya.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/idf1.py` & `streamlink-6.7.4/src/streamlink/plugins/idf1.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/indihometv.py` & `streamlink-6.7.4/src/streamlink/plugins/indihometv.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/invintus.py` & `streamlink-6.7.4/src/streamlink/plugins/invintus.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/kugou.py` & `streamlink-6.7.4/src/streamlink/plugins/kugou.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/linelive.py` & `streamlink-6.7.4/src/streamlink/plugins/linelive.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/livestream.py` & `streamlink-6.7.4/src/streamlink/plugins/livestream.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/lnk.py` & `streamlink-6.7.4/src/streamlink/plugins/lnk.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/lrt.py` & `streamlink-6.7.4/src/streamlink/plugins/lrt.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/ltv_lsm_lv.py` & `streamlink-6.7.4/src/streamlink/plugins/ltv_lsm_lv.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/mangomolo.py` & `streamlink-6.7.4/src/streamlink/plugins/mangomolo.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/mdstrm.py` & `streamlink-6.7.4/src/streamlink/plugins/mdstrm.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/mediaklikk.py` & `streamlink-6.7.4/src/streamlink/plugins/mediaklikk.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/mediavitrina.py` & `streamlink-6.7.4/src/streamlink/plugins/mediavitrina.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/mildom.py` & `streamlink-6.7.4/src/streamlink/plugins/mildom.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/mitele.py` & `streamlink-6.7.4/src/streamlink/plugins/mitele.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/mixcloud.py` & `streamlink-6.7.4/src/streamlink/plugins/mixcloud.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/mjunoon.py` & `streamlink-6.7.4/src/streamlink/plugins/mjunoon.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/mrtmk.py` & `streamlink-6.7.4/src/streamlink/plugins/mrtmk.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/n13tv.py` & `streamlink-6.7.4/src/streamlink/plugins/n13tv.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/nasaplus.py` & `streamlink-6.7.4/src/streamlink/plugins/nasaplus.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/nhkworld.py` & `streamlink-6.7.4/src/streamlink/plugins/nhkworld.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/nicolive.py` & `streamlink-6.7.4/src/streamlink/plugins/nicolive.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/nimotv.py` & `streamlink-6.7.4/src/streamlink/plugins/nimotv.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/nos.py` & `streamlink-6.7.4/src/streamlink/plugins/nos.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/nowtvtr.py` & `streamlink-6.7.4/src/streamlink/plugins/nowtvtr.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/nrk.py` & `streamlink-6.7.4/src/streamlink/plugins/nrk.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/okru.py` & `streamlink-6.7.4/src/streamlink/plugins/okru.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/olympicchannel.py` & `streamlink-6.7.4/src/streamlink/plugins/olympicchannel.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/oneplusone.py` & `streamlink-6.7.4/src/streamlink/plugins/oneplusone.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/onetv.py` & `streamlink-6.7.4/src/streamlink/plugins/onetv.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/openrectv.py` & `streamlink-6.7.4/src/streamlink/plugins/openrectv.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/pandalive.py` & `streamlink-6.7.4/src/streamlink/plugins/pandalive.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/piaulizaportal.py` & `streamlink-6.7.4/src/streamlink/plugins/piaulizaportal.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/picarto.py` & `streamlink-6.7.4/src/streamlink/plugins/picarto.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/piczel.py` & `streamlink-6.7.4/src/streamlink/plugins/piczel.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/pixiv.py` & `streamlink-6.7.4/src/streamlink/plugins/pixiv.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/pluto.py` & `streamlink-6.7.4/src/streamlink/plugins/pluto.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/pluzz.py` & `streamlink-6.7.4/src/streamlink/plugins/pluzz.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/radiko.py` & `streamlink-6.7.4/src/streamlink/plugins/radiko.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/radionet.py` & `streamlink-6.7.4/src/streamlink/plugins/radionet.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/raiplay.py` & `streamlink-6.7.4/src/streamlink/plugins/raiplay.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/reuters.py` & `streamlink-6.7.4/src/streamlink/plugins/reuters.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/rtpa.py` & `streamlink-6.7.4/src/streamlink/plugins/rtpa.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/rtpplay.py` & `streamlink-6.7.4/src/streamlink/plugins/rtpplay.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/rtve.py` & `streamlink-6.7.4/src/streamlink/plugins/rtve.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/rtvs.py` & `streamlink-6.7.4/src/streamlink/plugins/rtvs.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/ruv.py` & `streamlink-6.7.4/src/streamlink/plugins/ruv.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/sbscokr.py` & `streamlink-6.7.4/src/streamlink/plugins/sbscokr.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/showroom.py` & `streamlink-6.7.4/src/streamlink/plugins/showroom.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/sportal.py` & `streamlink-6.7.4/src/streamlink/plugins/sportal.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/sportschau.py` & `streamlink-6.7.4/src/streamlink/plugins/sportschau.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/ssh101.py` & `streamlink-6.7.4/src/streamlink/plugins/ssh101.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/stadium.py` & `streamlink-6.7.4/src/streamlink/plugins/stadium.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/steam.py` & `streamlink-6.7.4/src/streamlink/plugins/steam.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/streamable.py` & `streamlink-6.7.4/src/streamlink/plugins/streamable.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/streann.py` & `streamlink-6.7.4/src/streamlink/plugins/streann.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/stv.py` & `streamlink-6.7.4/src/streamlink/plugins/stv.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/svtplay.py` & `streamlink-6.7.4/src/streamlink/plugins/svtplay.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/swisstxt.py` & `streamlink-6.7.4/src/streamlink/plugins/swisstxt.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/telefe.py` & `streamlink-6.7.4/src/streamlink/plugins/telefe.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/telemadrid.py` & `streamlink-6.7.4/src/streamlink/plugins/telemadrid.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/tf1.py` & `streamlink-6.7.4/src/streamlink/plugins/tf1.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/trovo.py` & `streamlink-6.7.4/src/streamlink/plugins/trovo.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/turkuvaz.py` & `streamlink-6.7.4/src/streamlink/plugins/vkplay.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,111 +1,97 @@
 """
-$description Turkish live TV channels from Turkuvaz Media Group, including Ahaber, ATV, Minika COCUK and MinikaGO.
-$url a2tv.com.tr
-$url ahaber.com.tr
-$url anews.com.tr
-$url apara.com.tr
-$url aspor.com.tr
-$url atv.com.tr
-$url atvavrupa.tv
-$url minikacocuk.com.tr
-$url minikago.com.tr
-$url vavtv.com.tr
-$type live, vod
+$description Russian live-streaming platform for gaming and esports, owned by VKontakte.
+$url live.vkplay.ru
+$type live
 $metadata id
+$metadata author
+$metadata category
 $metadata title
-$region various
 """
 
 import logging
 import re
 
 from streamlink.plugin import Plugin, pluginmatcher
 from streamlink.plugin.api import validate
 from streamlink.stream.hls import HLSStream
 
 
 log = logging.getLogger(__name__)
 
 
-@pluginmatcher(re.compile(r"""
-    https?://(?:www\.)?
-    (?:
-        atvavrupa\.tv
-        |
-        (?:a2tv|ahaber|anews|apara|aspor|atv|minikacocuk|minikago|vavtv)\.com\.tr
-    )
-""", re.VERBOSE))
-class Turkuvaz(Plugin):
+@pluginmatcher(re.compile(
+    r"https?://(?:live\.vkplay\.ru|vkplay\.live)/(?P<channel_name>\w+)/?$",
+))
+class VKplay(Plugin):
+    API_URL = "https://api.live.vkplay.ru/v1"
+
     def _get_streams(self):
-        _find_and_get_attrs = validate.Schema(
-            validate.xml_find(".//div[@data-videoid][@data-websiteid]"),
-            validate.union_get("data-videoid", "data-websiteid"),
-        )
+        self.author = self.match["channel_name"]
+        log.debug(f"Channel name: {self.author}")
 
-        id_data = self.session.http.get(
-            self.url,
+        data = self.session.http.get(
+            f"{self.API_URL}/blog/{self.author}/public_video_stream",
+            headers={"Referer": self.url},
+            acceptable_status=(200, 404),
             schema=validate.Schema(
-                validate.parse_html(),
+                validate.parse_json(),
                 validate.any(
-                    _find_and_get_attrs,
                     validate.all(
-                        validate.xml_xpath_string(
-                            ".//script[contains(text(),'data-videoid') and contains(text(),'data-websiteid')]/text()",
-                        ),
-                        validate.none_or_all(
-                            str,
-                            validate.regex(re.compile(r"""var\s+tmdPlayer\s*=\s*(?P<q>["'])(.*?)(?P=q)""")),
-                            validate.get(0),
-                            validate.parse_html(),
-                            _find_and_get_attrs,
+                        {"error": str, "error_description": str},
+                        validate.get("error_description"),
+                    ),
+                    validate.all(
+                        {
+                            validate.optional("category"): validate.all(
+                                {
+                                    "title": str,
+                                },
+                                validate.get("title"),
+                            ),
+                            "title": str,
+                            "data": validate.any(
+                                [
+                                    validate.all(
+                                        {
+                                            "vid": str,
+                                            "playerUrls": [
+                                                validate.all(
+                                                    {
+                                                        "type": str,
+                                                        "url": validate.any("", validate.url()),
+                                                    },
+                                                    validate.union_get("type", "url"),
+                                                ),
+                                            ],
+                                        },
+                                        validate.union_get("vid", "playerUrls"),
+                                    ),
+                                ],
+                                [],
+                            ),
+                        },
+                        validate.union_get(
+                            "category",
+                            "title",
+                            ("data", 0),
                         ),
                     ),
                 ),
             ),
         )
-
-        if not id_data:
+        if isinstance(data, str):
+            log.error(data)
             return
 
-        video_id, website_id = id_data
-        log.debug(f"video_id={video_id}")
-        log.debug(f"website_id={website_id}")
-
-        self.id, self.title, hls_url = self.session.http.get(
-            f"https://videojs.tmgrup.com.tr/getvideo/{website_id}/{video_id}",
-            schema=validate.Schema(
-                validate.parse_json(),
-                {
-                    "success": True,
-                    "video": {
-                        "VideoId": str,
-                        "Title": str,
-                        "VideoSmilUrl": validate.url(),
-                    },
-                },
-                validate.get("video"),
-                validate.union_get("VideoId", "Title", "VideoSmilUrl"),
-            ),
-        )
-        log.debug(f"hls_url={hls_url}")
+        self.category, self.title, streamdata = data
+        if not streamdata:
+            return
 
-        secure_hls_url = self.session.http.get(
-            "https://securevideotoken.tmgrup.com.tr/webtv/secure",
-            params=f"url={hls_url}",
-            headers={"Referer": self.url},
-            schema=validate.Schema(
-                validate.parse_json(),
-                {
-                    "Success": True,
-                    "Url": validate.url(),
-                },
-                validate.get("Url"),
-            ),
-        )
-        log.debug(f"secure_hls_url={secure_hls_url}")
+        self.id, streams = streamdata
 
-        if secure_hls_url:
-            return HLSStream.parse_variant_playlist(self.session, secure_hls_url)
+        for streamtype, streamurl in streams:
+            if streamurl and streamtype == "live_hls":
+                return HLSStream.parse_variant_playlist(self.session, streamurl)
 
 
-__plugin__ = Turkuvaz
+__plugin__ = VKplay
```

### Comparing `streamlink-6.7.3/src/streamlink/plugins/tv360.py` & `streamlink-6.7.4/src/streamlink/plugins/tv360.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/tv3cat.py` & `streamlink-6.7.4/src/streamlink/plugins/tv3cat.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/tv4play.py` & `streamlink-6.7.4/src/streamlink/plugins/tv4play.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/tv5monde.py` & `streamlink-6.7.4/src/streamlink/plugins/tv5monde.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/tv8.py` & `streamlink-6.7.4/src/streamlink/plugins/tv8.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/tv999.py` & `streamlink-6.7.4/src/streamlink/plugins/tv999.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/tvibo.py` & `streamlink-6.7.4/src/streamlink/plugins/tvibo.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/tviplayer.py` & `streamlink-6.7.4/src/streamlink/plugins/tviplayer.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/tvp.py` & `streamlink-6.7.4/src/streamlink/plugins/tvp.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/tvrby.py` & `streamlink-6.7.4/src/streamlink/plugins/tvrby.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/tvrplus.py` & `streamlink-6.7.4/src/streamlink/plugins/tvrplus.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/tvtoya.py` & `streamlink-6.7.4/src/streamlink/plugins/tvtoya.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/twitcasting.py` & `streamlink-6.7.4/src/streamlink/plugins/twitcasting.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/twitch.py` & `streamlink-6.7.4/src/streamlink/plugins/twitch.py`

 * *Files 0% similar despite different names*

```diff
@@ -537,15 +537,15 @@
     def acquire(
         cls,
         session: Streamlink,
         channel: str,
         headers: Mapping[str, str],
         device_id: str,
     ) -> Optional[Tuple[str, int]]:
-        from exceptiongroup import BaseExceptionGroup  # noqa: PLC0415, I001
+        from streamlink.compat import BaseExceptionGroup  # noqa: PLC0415
         from streamlink.webbrowser.cdp import CDPClient, CDPClientSession, devtools  # noqa: PLC0415
 
         url = f"https://www.twitch.tv/{channel}"
         js_get_integrity_token = cls.JS_INTEGRITY_TOKEN \
             .replace("SCRIPT_SOURCE", cls.URL_P_SCRIPT) \
             .replace("HEADERS", json_dumps(headers)) \
             .replace("DEVICE_ID", device_id)
```

### Comparing `streamlink-6.7.3/src/streamlink/plugins/ustreamtv.py` & `streamlink-6.7.4/src/streamlink/plugins/ustreamtv.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/ustvnow.py` & `streamlink-6.7.4/src/streamlink/plugins/ustvnow.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/vidio.py` & `streamlink-6.7.4/src/streamlink/plugins/vidio.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/vimeo.py` & `streamlink-6.7.4/src/streamlink/plugins/vimeo.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/vinhlongtv.py` & `streamlink-6.7.4/src/streamlink/plugins/vinhlongtv.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/vk.py` & `streamlink-6.7.4/src/streamlink/plugins/vk.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/vkplay.py` & `streamlink-6.7.4/src/streamlink/plugins/zdf_mediathek.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,97 +1,96 @@
 """
-$description Russian live-streaming platform for gaming and esports, owned by VKontakte.
-$url live.vkplay.ru
-$type live
-$metadata id
-$metadata author
-$metadata category
-$metadata title
+$description Live TV channels and video on-demand service from ZDF, a German public, independent broadcaster.
+$url zdf.de
+$type live, vod
+$region Germany
 """
 
 import logging
 import re
+from urllib.parse import urlparse, urlunparse
 
 from streamlink.plugin import Plugin, pluginmatcher
 from streamlink.plugin.api import validate
 from streamlink.stream.hls import HLSStream
+from streamlink.utils.url import url_concat
 
 
 log = logging.getLogger(__name__)
 
 
 @pluginmatcher(re.compile(
-    r"https?://(?:live\.vkplay\.ru|vkplay\.live)/(?P<channel_name>\w+)/?$",
+    r"https?://(\w+\.)?(zdf\.de|3sat\.de)/",
 ))
-class VKplay(Plugin):
-    API_URL = "https://api.live.vkplay.ru/v1"
+class ZDFMediathek(Plugin):
+    PLAYER_ID = "ngplayer_2_4"
 
     def _get_streams(self):
-        self.author = self.match["channel_name"]
-        log.debug(f"Channel name: {self.author}")
-
-        data = self.session.http.get(
-            f"{self.API_URL}/blog/{self.author}/public_video_stream",
-            headers={"Referer": self.url},
-            acceptable_status=(200, 404),
-            schema=validate.Schema(
+        zdf_json = self.session.http.get(self.url, schema=validate.Schema(
+            validate.parse_html(),
+            validate.xml_xpath_string(".//*[@data-zdfplayer-jsb][1]/@data-zdfplayer-jsb"),
+            validate.none_or_all(
                 validate.parse_json(),
-                validate.any(
-                    validate.all(
-                        {"error": str, "error_description": str},
-                        validate.get("error_description"),
-                    ),
-                    validate.all(
-                        {
-                            validate.optional("category"): validate.all(
-                                {
-                                    "title": str,
-                                },
-                                validate.get("title"),
-                            ),
-                            "title": str,
-                            "data": validate.any(
-                                [
-                                    validate.all(
-                                        {
-                                            "vid": str,
-                                            "playerUrls": [
-                                                validate.all(
-                                                    {
-                                                        "type": str,
-                                                        "url": validate.any("", validate.url()),
-                                                    },
-                                                    validate.union_get("type", "url"),
-                                                ),
-                                            ],
-                                        },
-                                        validate.union_get("vid", "playerUrls"),
-                                    ),
-                                ],
-                                [],
-                            ),
-                        },
-                        validate.union_get(
-                            "category",
-                            "title",
-                            ("data", 0),
-                        ),
-                    ),
-                ),
+                {
+                    "apiToken": str,
+                    "content": validate.url(),
+                },
+                validate.union_get("apiToken", "content"),
             ),
-        )
-        if isinstance(data, str):
-            log.error(data)
+        ))
+        if zdf_json is None:
             return
 
-        self.category, self.title, streamdata = data
-        if not streamdata:
-            return
+        apiToken, apiUrl = zdf_json
 
-        self.id, streams = streamdata
-
-        for streamtype, streamurl in streams:
-            if streamurl and streamtype == "live_hls":
-                return HLSStream.parse_variant_playlist(self.session, streamurl)
+        headers = {
+            "Accept": "application/vnd.de.zdf.v1.0+json;charset=UTF-8",
+            "Api-Auth": f"Bearer {apiToken}",
+            "Referer": self.url,
+        }
+
+        pApiUrl = urlparse(apiUrl)
+        apiUrlBase = urlunparse((pApiUrl.scheme, pApiUrl.netloc, "", "", "", ""))
+        apiUrlPath = self.session.http.get(apiUrl, headers=headers, schema=validate.Schema(
+            validate.parse_json(),
+            {"mainVideoContent": {
+                "http://zdf.de/rels/target": {
+                    "http://zdf.de/rels/streams/ptmd-template": str,
+                },
+            }},
+            validate.get(("mainVideoContent", "http://zdf.de/rels/target", "http://zdf.de/rels/streams/ptmd-template")),
+            validate.transform(lambda template: template.format(playerId=self.PLAYER_ID).replace(" ", "")),
+        ))
+
+        stream_request_url = url_concat(apiUrlBase, apiUrlPath)
+        data = self.session.http.get(stream_request_url, headers=headers, schema=validate.Schema(
+            validate.parse_json(),
+            {"priorityList": [{
+                "formitaeten": validate.all(
+                    [{
+                        "type": str,
+                        "qualities": validate.all(
+                            [{
+                                "quality": str,
+                                "audio": {
+                                    "tracks": [{
+                                        "uri": validate.url(),
+                                    }],
+                                },
+                            }],
+                            validate.filter(lambda obj: obj["quality"] == "auto"),
+                        ),
+                    }],
+                    validate.filter(lambda obj: obj["type"] == "h264_aac_ts_http_m3u8_http"),
+                ),
+            }]},
+            validate.get("priorityList"),
+        ))
+
+        for priority in data:
+            for formitaeten in priority["formitaeten"]:
+                for quality in formitaeten["qualities"]:
+                    for audio in quality["audio"]["tracks"]:
+                        yield from HLSStream.parse_variant_playlist(self.session, audio["uri"], headers=headers).items()
 
 
-__plugin__ = VKplay
+__plugin__ = ZDFMediathek
```

### Comparing `streamlink-6.7.3/src/streamlink/plugins/vtvgo.py` & `streamlink-6.7.4/src/streamlink/plugins/vtvgo.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/webtv.py` & `streamlink-6.7.4/src/streamlink/plugins/webtv.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/welt.py` & `streamlink-6.7.4/src/streamlink/plugins/welt.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/wwenetwork.py` & `streamlink-6.7.4/src/streamlink/plugins/wwenetwork.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/youtube.py` & `streamlink-6.7.4/src/streamlink/plugins/youtube.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/yupptv.py` & `streamlink-6.7.4/src/streamlink/plugins/yupptv.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/zattoo.py` & `streamlink-6.7.4/src/streamlink/plugins/zattoo.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/zeenews.py` & `streamlink-6.7.4/src/streamlink/plugins/zeenews.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/zengatv.py` & `streamlink-6.7.4/src/streamlink/plugins/zengatv.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/plugins/zhanqi.py` & `streamlink-6.7.4/src/streamlink/plugins/zhanqi.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/session/http.py` & `streamlink-6.7.4/src/streamlink/session/http.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/session/http.pyi` & `streamlink-6.7.4/src/streamlink/session/http.pyi`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/session/options.py` & `streamlink-6.7.4/src/streamlink/session/options.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/session/plugins.py` & `streamlink-6.7.4/src/streamlink/session/plugins.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/session/session.py` & `streamlink-6.7.4/src/streamlink/session/session.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/stream/dash/dash.py` & `streamlink-6.7.4/src/streamlink/stream/dash/dash.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/stream/dash/manifest.py` & `streamlink-6.7.4/src/streamlink/stream/dash/manifest.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/stream/dash/segment.py` & `streamlink-6.7.4/src/streamlink/stream/dash/segment.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/stream/ffmpegmux.py` & `streamlink-6.7.4/src/streamlink/stream/ffmpegmux.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/stream/file.py` & `streamlink-6.7.4/src/streamlink/stream/file.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/stream/filtered.py` & `streamlink-6.7.4/src/streamlink/stream/filtered.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/stream/hls/hls.py` & `streamlink-6.7.4/src/streamlink/stream/hls/hls.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/stream/hls/m3u8.py` & `streamlink-6.7.4/src/streamlink/stream/hls/m3u8.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/stream/hls/segment.py` & `streamlink-6.7.4/src/streamlink/stream/hls/segment.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/stream/http.py` & `streamlink-6.7.4/src/streamlink/stream/http.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/stream/segmented/concurrent.py` & `streamlink-6.7.4/src/streamlink/stream/segmented/concurrent.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/stream/segmented/segmented.py` & `streamlink-6.7.4/src/streamlink/stream/segmented/segmented.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/stream/stream.py` & `streamlink-6.7.4/src/streamlink/stream/stream.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/stream/wrappers.py` & `streamlink-6.7.4/src/streamlink/stream/wrappers.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/user_input.py` & `streamlink-6.7.4/src/streamlink/user_input.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/utils/__init__.py` & `streamlink-6.7.4/src/streamlink/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/utils/args.py` & `streamlink-6.7.4/src/streamlink/utils/args.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/utils/cache.py` & `streamlink-6.7.4/src/streamlink/utils/cache.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/utils/crypto.py` & `streamlink-6.7.4/src/streamlink/utils/crypto.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/utils/data.py` & `streamlink-6.7.4/src/streamlink/utils/data.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/utils/formatter.py` & `streamlink-6.7.4/src/streamlink/utils/formatter.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/utils/l10n.py` & `streamlink-6.7.4/src/streamlink/utils/l10n.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/utils/module.py` & `streamlink-6.7.4/src/streamlink/utils/module.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/utils/named_pipe.py` & `streamlink-6.7.4/src/streamlink/utils/named_pipe.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/utils/parse.py` & `streamlink-6.7.4/src/streamlink/utils/parse.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/utils/processoutput.py` & `streamlink-6.7.4/src/streamlink/utils/processoutput.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/utils/random.py` & `streamlink-6.7.4/src/streamlink/utils/random.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/utils/socket.py` & `streamlink-6.7.4/src/streamlink/utils/socket.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/utils/times.py` & `streamlink-6.7.4/src/streamlink/utils/times.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/utils/url.py` & `streamlink-6.7.4/src/streamlink/utils/url.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/webbrowser/cdp/client.py` & `streamlink-6.7.4/src/streamlink/webbrowser/cdp/client.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/webbrowser/cdp/connection.py` & `streamlink-6.7.4/src/streamlink/webbrowser/cdp/connection.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/webbrowser/cdp/devtools/__init__.py` & `streamlink-6.7.4/src/streamlink/webbrowser/cdp/devtools/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/webbrowser/cdp/devtools/browser.py` & `streamlink-6.7.4/src/streamlink/webbrowser/cdp/devtools/browser.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/webbrowser/cdp/devtools/debugger.py` & `streamlink-6.7.4/src/streamlink/webbrowser/cdp/devtools/debugger.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/webbrowser/cdp/devtools/dom.py` & `streamlink-6.7.4/src/streamlink/webbrowser/cdp/devtools/dom.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/webbrowser/cdp/devtools/emulation.py` & `streamlink-6.7.4/src/streamlink/webbrowser/cdp/devtools/emulation.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/webbrowser/cdp/devtools/fetch.py` & `streamlink-6.7.4/src/streamlink/webbrowser/cdp/devtools/fetch.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/webbrowser/cdp/devtools/input_.py` & `streamlink-6.7.4/src/streamlink/webbrowser/cdp/devtools/input_.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/webbrowser/cdp/devtools/inspector.py` & `streamlink-6.7.4/src/streamlink/webbrowser/cdp/devtools/inspector.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/webbrowser/cdp/devtools/io.py` & `streamlink-6.7.4/src/streamlink/webbrowser/cdp/devtools/io.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/webbrowser/cdp/devtools/network.py` & `streamlink-6.7.4/src/streamlink/webbrowser/cdp/devtools/network.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/webbrowser/cdp/devtools/page.py` & `streamlink-6.7.4/src/streamlink/webbrowser/cdp/devtools/page.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/webbrowser/cdp/devtools/runtime.py` & `streamlink-6.7.4/src/streamlink/webbrowser/cdp/devtools/runtime.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/webbrowser/cdp/devtools/security.py` & `streamlink-6.7.4/src/streamlink/webbrowser/cdp/devtools/security.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/webbrowser/cdp/devtools/target.py` & `streamlink-6.7.4/src/streamlink/webbrowser/cdp/devtools/target.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/webbrowser/cdp/devtools/util.py` & `streamlink-6.7.4/src/streamlink/webbrowser/cdp/devtools/util.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/webbrowser/chromium.py` & `streamlink-6.7.4/src/streamlink/webbrowser/chromium.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink/webbrowser/webbrowser.py` & `streamlink-6.7.4/src/streamlink/webbrowser/webbrowser.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 from contextlib import asynccontextmanager, contextmanager
 from functools import partial
 from pathlib import Path
 from subprocess import DEVNULL
 from typing import AsyncContextManager, AsyncGenerator, Generator, List, Optional, Union
 
 import trio
-from exceptiongroup import BaseExceptionGroup
 
+from streamlink.compat import BaseExceptionGroup
 from streamlink.utils.path import resolve_executable
 from streamlink.webbrowser.exceptions import WebbrowserError
 
 
 log = logging.getLogger(__name__)
```

### Comparing `streamlink-6.7.3/src/streamlink.egg-info/PKG-INFO` & `streamlink-6.7.4/src/streamlink.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlink
-Version: 6.7.3
+Version: 6.7.4
 Summary: Streamlink is a command-line utility that extracts streams from various services and pipes them into a video player of choice.
 Author: Streamlink
 Author-email: streamlink@protonmail.com
 License: Simplified BSD
 Project-URL: Homepage, https://github.com/streamlink/streamlink
 Project-URL: Documentation, https://streamlink.github.io/
 Project-URL: Tracker, https://github.com/streamlink/streamlink/issues
@@ -28,15 +28,15 @@
 Classifier: Topic :: Multimedia :: Sound/Audio
 Classifier: Topic :: Multimedia :: Video
 Classifier: Topic :: Utilities
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: certifi
-Requires-Dist: exceptiongroup
+Requires-Dist: exceptiongroup; python_version < "3.11"
 Requires-Dist: isodate
 Requires-Dist: lxml<6,>=4.6.4
 Requires-Dist: pycountry
 Requires-Dist: pycryptodome<4,>=3.4.3
 Requires-Dist: PySocks!=1.5.7,>=1.5.6
 Requires-Dist: requests<3,>=2.26.0
 Requires-Dist: trio<1,>=0.22.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: streamlink Version: 6.7.3 Summary: Streamlink is a
+Metadata-Version: 2.1 Name: streamlink Version: 6.7.4 Summary: Streamlink is a
 command-line utility that extracts streams from various services and pipes them
 into a video player of choice. Author: Streamlink Author-email:
 streamlink@protonmail.com License: Simplified BSD Project-URL: Homepage, https:
 //github.com/streamlink/streamlink Project-URL: Documentation, https://
 streamlink.github.io/ Project-URL: Tracker, https://github.com/streamlink/
 streamlink/issues Project-URL: Source, https://github.com/streamlink/streamlink
 Project-URL: Funding, https://streamlink.github.io/latest/donate.html
@@ -14,20 +14,21 @@
 Programming Language :: Python :: 3 :: Only Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
 Topic :: Internet :: WWW/HTTP Classifier: Topic :: Multimedia :: Sound/Audio
 Classifier: Topic :: Multimedia :: Video Classifier: Topic :: Utilities
 Requires-Python: >=3.8 Description-Content-Type: text/markdown License-File:
-LICENSE Requires-Dist: certifi Requires-Dist: exceptiongroup Requires-Dist:
-isodate Requires-Dist: lxml<6,>=4.6.4 Requires-Dist: pycountry Requires-Dist:
-pycryptodome<4,>=3.4.3 Requires-Dist: PySocks!=1.5.7,>=1.5.6 Requires-Dist:
-requests<3,>=2.26.0 Requires-Dist: trio<1,>=0.22.0 Requires-Dist: trio-
-websocket<1,>=0.9.0 Requires-Dist: typing-extensions>=4.0.0 Requires-Dist:
-urllib3<3,>=1.26.0 Requires-Dist: websocket-client<2,>=1.2.1
+LICENSE Requires-Dist: certifi Requires-Dist: exceptiongroup; python_version <
+"3.11" Requires-Dist: isodate Requires-Dist: lxml<6,>=4.6.4 Requires-Dist:
+pycountry Requires-Dist: pycryptodome<4,>=3.4.3 Requires-Dist:
+PySocks!=1.5.7,>=1.5.6 Requires-Dist: requests<3,>=2.26.0 Requires-Dist:
+trio<1,>=0.22.0 Requires-Dist: trio-websocket<1,>=0.9.0 Requires-Dist: typing-
+extensions>=4.0.0 Requires-Dist: urllib3<3,>=1.26.0 Requires-Dist: websocket-
+client<2,>=1.2.1
                                ************ _SS_tt_rr_ee_aa_mm_ll_ii_nn_kk
                               _[[_SS_tt_rr_ee_aa_mm_ll_ii_nn_kk_]] ************
 _[_S_u_p_p_o_r_t_e_d_ _P_y_t_h_o_n_ _v_e_r_s_i_o_n_s_]_[_L_a_t_e_s_t_ _r_e_l_e_a_s_e_]_[_L_i_c_e_n_s_e_]_[_O_p_e_n_ _i_s_s_u_e_s_]_[_B_u_i_l_d_ _s_t_a_t_u_s_]
                             _[_O_v_e_r_a_l_l_ _c_o_d_e_ _c_o_v_e_r_a_g_e_]
  A Python library and command-line interface which pipes streams from various
                          services into a video player.
     Avoid resource-heavy and unoptimized websites, and still enjoy streamed
```

### Comparing `streamlink-6.7.3/src/streamlink.egg-info/SOURCES.txt` & `streamlink-6.7.4/src/streamlink.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -127,14 +127,15 @@
 src/streamlink/plugins/bloomberg.py
 src/streamlink/plugins/booyah.py
 src/streamlink/plugins/brightcove.py
 src/streamlink/plugins/btv.py
 src/streamlink/plugins/cbsnews.py
 src/streamlink/plugins/cdnbg.py
 src/streamlink/plugins/ceskatelevize.py
+src/streamlink/plugins/chzzk.py
 src/streamlink/plugins/cinergroup.py
 src/streamlink/plugins/clubbingtv.py
 src/streamlink/plugins/cmmedia.py
 src/streamlink/plugins/cnews.py
 src/streamlink/plugins/crunchyroll.py
 src/streamlink/plugins/dailymotion.py
 src/streamlink/plugins/dash.py
@@ -179,15 +180,14 @@
 src/streamlink/plugins/mrtmk.py
 src/streamlink/plugins/n13tv.py
 src/streamlink/plugins/nasaplus.py
 src/streamlink/plugins/nhkworld.py
 src/streamlink/plugins/nicolive.py
 src/streamlink/plugins/nimotv.py
 src/streamlink/plugins/nos.py
-src/streamlink/plugins/nownews.py
 src/streamlink/plugins/nowtvtr.py
 src/streamlink/plugins/nrk.py
 src/streamlink/plugins/okru.py
 src/streamlink/plugins/olympicchannel.py
 src/streamlink/plugins/oneplusone.py
 src/streamlink/plugins/onetv.py
 src/streamlink/plugins/openrectv.py
@@ -323,14 +323,15 @@
 src/streamlink_cli/__init__.py
 src/streamlink_cli/__main__.py
 src/streamlink_cli/_parser.py
 src/streamlink_cli/argparser.py
 src/streamlink_cli/compat.py
 src/streamlink_cli/console.py
 src/streamlink_cli/constants.py
+src/streamlink_cli/exceptions.py
 src/streamlink_cli/main.py
 src/streamlink_cli/py.typed
 src/streamlink_cli/streamrunner.py
 src/streamlink_cli/output/__init__.py
 src/streamlink_cli/output/abc.py
 src/streamlink_cli/output/file.py
 src/streamlink_cli/output/http.py
@@ -403,14 +404,15 @@
 tests/plugins/test_bloomberg.py
 tests/plugins/test_booyah.py
 tests/plugins/test_brightcove.py
 tests/plugins/test_btv.py
 tests/plugins/test_cbsnews.py
 tests/plugins/test_cdnbg.py
 tests/plugins/test_ceskatelevize.py
+tests/plugins/test_chzzk.py
 tests/plugins/test_cinergroup.py
 tests/plugins/test_clubbingtv.py
 tests/plugins/test_cmmedia.py
 tests/plugins/test_cnews.py
 tests/plugins/test_crunchyroll.py
 tests/plugins/test_dailymotion.py
 tests/plugins/test_dash.py
@@ -455,15 +457,14 @@
 tests/plugins/test_mrtmk.py
 tests/plugins/test_n13tv.py
 tests/plugins/test_nasaplus.py
 tests/plugins/test_nhkworld.py
 tests/plugins/test_nicolive.py
 tests/plugins/test_nimotv.py
 tests/plugins/test_nos.py
-tests/plugins/test_nownews.py
 tests/plugins/test_nowtvtr.py
 tests/plugins/test_nrk.py
 tests/plugins/test_okru.py
 tests/plugins/test_olympicchannel.py
 tests/plugins/test_oneplusone.py
 tests/plugins/test_onetv.py
 tests/plugins/test_openrectv.py
```

### Comparing `streamlink-6.7.3/src/streamlink_cli/argparser.py` & `streamlink-6.7.4/src/streamlink_cli/argparser.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink_cli/console.py` & `streamlink-6.7.4/src/streamlink_cli/console.py`

 * *Files 9% similar despite different names*

```diff
@@ -78,20 +78,9 @@
                     continue
                 out.update(**obj)
             out.update(**keywords)
 
         msg = dumps(out, cls=JSONEncoder, indent=2)
         self.output.write(f"{msg}\n")
 
-        if isinstance(out, dict) and out.get("error"):
-            sys.exit(1)
-
-    def exit(self, msg: str) -> None:
-        if self.json:
-            self.msg_json(error=msg)
-        else:
-            self.msg(f"error: {msg}")
-
-        sys.exit(1)
-
 
 __all__ = ["ConsoleOutput", "ConsoleUserInputRequester"]
```

### Comparing `streamlink-6.7.3/src/streamlink_cli/constants.py` & `streamlink-6.7.4/src/streamlink_cli/constants.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink_cli/main.py` & `streamlink-6.7.4/src/streamlink_cli/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,28 +8,29 @@
 import ssl
 import sys
 import warnings
 from contextlib import closing, suppress
 from gettext import gettext
 from pathlib import Path
 from time import sleep
-from typing import Any, Dict, List, Optional, Type, Union
+from typing import Any, List, Mapping, Optional, Type, Union
 
 import streamlink.logger as logger
 from streamlink import NoPluginError, PluginError, StreamError, Streamlink, __version__ as streamlink_version
 from streamlink.exceptions import FatalPluginError, StreamlinkDeprecationWarning
 from streamlink.options import Options
 from streamlink.plugin import Plugin
 from streamlink.stream.stream import Stream, StreamIO
 from streamlink.utils.named_pipe import NamedPipe
 from streamlink.utils.times import LOCAL as LOCALTIMEZONE
 from streamlink_cli.argparser import ArgumentParser, build_parser, setup_session_options
 from streamlink_cli.compat import DeprecatedPath, stdout
 from streamlink_cli.console import ConsoleOutput, ConsoleUserInputRequester
 from streamlink_cli.constants import CONFIG_FILES, DEFAULT_STREAM_METADATA, LOG_DIR, PLUGIN_DIRS, STREAM_SYNONYMS
+from streamlink_cli.exceptions import StreamlinkCLIError
 from streamlink_cli.output import FileOutput, HTTPOutput, PlayerOutput
 from streamlink_cli.streamrunner import StreamRunner
 from streamlink_cli.utils import Formatter, datetime
 from streamlink_cli.utils.versioncheck import check_version
 
 
 QUIET_OPTIONS = ("json", "stream_url", "quiet")
@@ -75,18 +76,18 @@
     log.info(f"Writing output to\n{realpath}")
     log.debug("Checking file output")
 
     if realpath.is_file() and not force:
         if sys.stdin.isatty():
             answer = console.ask(f"File {path} already exists! Overwrite it? [y/N] ")
             if not answer or answer.lower() != "y":
-                sys.exit()
+                raise StreamlinkCLIError()
         else:
             log.error(f"File {path} already exists, use --force to overwrite it.")
-            sys.exit()
+            raise StreamlinkCLIError()
 
     return FileOutput(filename=realpath)
 
 
 def create_output(formatter: Formatter) -> Union[FileOutput, PlayerOutput]:
     """Decides where to write the stream.
 
@@ -95,48 +96,37 @@
      - A subprocess' stdin pipe
      - A named pipe that the subprocess reads from
      - A regular file
 
     """
 
     if (args.output or args.stdout) and (args.record or args.record_and_pipe):
-        console.exit("Cannot use record options with other file output options.")
-        return  # type: ignore
+        raise StreamlinkCLIError("Cannot use record options with other file output options.")
 
     if args.output:
         if args.output == "-":
             return FileOutput(fd=stdout)
         else:
             return check_file_output(formatter.path(args.output, args.fs_safe_rules), args.force)
 
     elif args.stdout:
         return FileOutput(fd=stdout)
 
     elif args.record_and_pipe:
         record = check_file_output(formatter.path(args.record_and_pipe, args.fs_safe_rules), args.force)
         return FileOutput(fd=stdout, record=record)
 
-    elif not args.player:
-        console.exit(
-            "The default player (VLC) does not seem to be installed."
-            + " You must specify the path to a player executable with --player,"
-            + " a file path to save the stream with --output,"
-            + " or pipe the stream to another program with --stdout.",
-        )
-        return  # type: ignore
-
-    else:
+    elif args.player:
         http = namedpipe = record = None
 
         if args.player_fifo:
             try:
                 namedpipe = NamedPipe()  # type: ignore[abstract]  # ???
             except OSError as err:
-                console.exit(f"Failed to create pipe: {err}")
-                return  # type: ignore
+                raise StreamlinkCLIError(f"Failed to create pipe: {err}") from err
         elif args.player_http:
             http = create_http_server()
 
         if args.record:
             if args.record == "-":
                 record = FileOutput(fd=stdout)
             else:
@@ -152,45 +142,51 @@
             kill=not args.player_no_close,
             namedpipe=namedpipe,
             http=http,
             record=record,
             title=formatter.title(args.title, defaults=DEFAULT_STREAM_METADATA) if args.title else args.url,
         )
 
+    raise StreamlinkCLIError(
+        "The default player (VLC) does not seem to be installed."
+        + " You must specify the path to a player executable with --player,"
+        + " a file path to save the stream with --output,"
+        + " or pipe the stream to another program with --stdout.",
+    )
+
 
 def create_http_server(host: Optional[str] = None, port: int = 0) -> HTTPOutput:
     """
     Create an HTTP server listening on a given host and port.
     If host is None, listen on all available interfaces.
     If port is 0, listen on a random high port.
     """
 
     try:
         httpoutput = HTTPOutput(host, port)
         httpoutput.start_server()
         return httpoutput
     except OSError as err:
-        console.exit(f"Failed to create HTTP server: {err}")
-        raise
+        raise StreamlinkCLIError(f"Failed to create HTTP server: {err}") from err
 
 
 def output_stream_http(
     plugin: Plugin,
-    initial_streams: Dict[str, Stream],
+    initial_streams: Mapping[str, Stream],
     formatter: Formatter,
     external: bool = False,
     continuous: bool = True,
     port: int = 0,
 ):
     """Continuously output the stream over HTTP."""
     global output
 
     if not external:
         if not args.player:
-            console.exit(
+            raise StreamlinkCLIError(
                 "The default player (VLC) does not seem to be installed."
                 + " You must specify the path to a player executable with --player.",
             )
 
         server = create_http_server()
         player = output = PlayerOutput(
             path=args.player,
@@ -202,15 +198,15 @@
         )
 
         try:
             log.info(f"Starting player: {args.player}")
             if player:
                 player.open()
         except OSError as err:
-            console.exit(f"Failed to start player: {args.player} ({err})")
+            raise StreamlinkCLIError(f"Failed to start player: {args.player} ({err})") from err
     else:
         server = create_http_server(args.player_external_http_interface, port)
         player = None
 
         log.info("Starting server, access with one of:")
         for url in server.urls:
             log.info(f" {url}")
@@ -255,16 +251,15 @@
 
         if stream_fd and prebuffer:
             log.debug("Writing stream to player")
             stream_runner = StreamRunner(stream_fd, server)
             try:
                 stream_runner.run(prebuffer)
             except OSError as err:
-                # TODO: refactor all console.exit() calls
-                console.exit(str(err))
+                raise StreamlinkCLIError() from err
 
         if not continuous:
             break
 
         server.close()
 
     if player:
@@ -275,16 +270,15 @@
 def output_stream_passthrough(stream, formatter: Formatter):
     """Prepares a filename to be passed to the player."""
     global output
 
     try:
         url = stream.to_url()
     except TypeError:
-        console.exit("The stream specified cannot be translated to a URL")
-        return False
+        raise StreamlinkCLIError("The stream specified cannot be translated to a URL") from None
 
     output = PlayerOutput(
         path=args.player,
         args=args.player_args,
         env=args.player_env,
         quiet=not args.verbose_player,
         call=True,
@@ -292,16 +286,15 @@
         title=formatter.title(args.title, defaults=DEFAULT_STREAM_METADATA) if args.title else args.url,
     )
 
     try:
         log.info(f"Starting player: {args.player}")
         output.open()
     except OSError as err:
-        console.exit(f"Failed to start player: {args.player} ({err})")
-        return False
+        raise StreamlinkCLIError(f"Failed to start player: {args.player} ({err})") from err
 
     return True
 
 
 def open_stream(stream):
     """Opens a stream and reads 8192 bytes from it.
 
@@ -346,26 +339,25 @@
             stream_fd, prebuffer = open_stream(stream)
             success_open = True
             break
         except StreamError as err:
             log.error(f"Try {i + 1}/{args.retry_open}: Could not open stream {stream} ({err})")
 
     if not success_open:
-        return console.exit(f"Could not open stream {stream}, tried {args.retry_open} times, exiting")
+        raise StreamlinkCLIError(f"Could not open stream {stream}, tried {args.retry_open} times, exiting")
 
     try:
         output.open()
     except OSError as err:
         if isinstance(output, PlayerOutput):
-            console.exit(f"Failed to start player: {args.player} ({err})")
+            raise StreamlinkCLIError(f"Failed to start player: {args.player} ({err})") from err
         elif output.filename:
-            console.exit(f"Failed to open output: {output.filename} ({err})")
+            raise StreamlinkCLIError(f"Failed to open output: {output.filename} ({err})") from err
         else:
-            console.exit(f"Failed to open output ({err}")
-        return
+            raise StreamlinkCLIError(f"Failed to open output ({err})") from err
 
     try:
         with closing(output):
             log.debug("Writing stream to output")
             show_progress = args.progress == "force" or args.progress == "yes" and sys.stderr.isatty()
             if args.force_progress:
                 show_progress = True
@@ -376,21 +368,20 @@
                 )
             # TODO: finally clean up the global variable mess and refactor the streamlink_cli package
             # noinspection PyUnboundLocalVariable
             stream_runner = StreamRunner(stream_fd, output, show_progress=show_progress)
             # noinspection PyUnboundLocalVariable
             stream_runner.run(prebuffer)
     except OSError as err:
-        # TODO: refactor all console.exit() calls
-        console.exit(str(err))
+        raise StreamlinkCLIError() from err
 
     return True
 
 
-def handle_stream(plugin: Plugin, streams: Dict[str, Stream], stream_name: str) -> None:
+def handle_stream(plugin: Plugin, streams: Mapping[str, Stream], stream_name: str) -> None:
     """Decides what to do with the selected stream.
 
     Depending on arguments it can be one of these:
      - Output JSON represenation
      - Output the stream URL
      - Continuously output the stream over HTTP
      - Output stream data to selected output
@@ -407,15 +398,15 @@
             metadata=plugin.get_metadata(),
         )
 
     elif args.stream_url:
         try:
             console.msg(stream.to_url())
         except TypeError:
-            console.exit("The stream specified cannot be translated to a URL")
+            raise StreamlinkCLIError("The stream specified cannot be translated to a URL") from None
 
     else:
         # Find any streams with a '_alt' suffix and attempt
         # to use these in case the main stream is not usable.
         alt_streams = list(filter(lambda k: f"{stream_name}_alt" in k, sorted(streams.keys())))
 
         file_output = args.output or args.stdout
@@ -444,22 +435,22 @@
                 log.info(f"Opening stream: {name} ({stream_type})")
                 success = output_stream(stream, formatter)
 
             if success:
                 break
 
 
-def fetch_streams(plugin: Plugin) -> Dict[str, Stream]:
+def fetch_streams(plugin: Plugin) -> Mapping[str, Stream]:
     """Fetches streams using correct parameters."""
 
     return plugin.streams(stream_types=args.stream_types,
                           sorting_excludes=args.stream_sorting_excludes)
 
 
-def fetch_streams_with_retry(plugin: Plugin, interval: float, count: int) -> Optional[Dict[str, Stream]]:
+def fetch_streams_with_retry(plugin: Plugin, interval: float, count: int) -> Optional[Mapping[str, Stream]]:
     """Attempts to fetch streams repeatedly
        until some are returned or limit hit."""
 
     try:
         streams = fetch_streams(plugin)
     except PluginError as err:
         log.error(err)
@@ -483,26 +474,26 @@
             attempts += 1
             if attempts >= count:
                 break
 
     return streams
 
 
-def resolve_stream_name(streams: Dict[str, Stream], stream_name: str) -> str:
+def resolve_stream_name(streams: Mapping[str, Stream], stream_name: str) -> str:
     """Returns the real stream name of a synonym."""
 
     if stream_name in STREAM_SYNONYMS and stream_name in streams:
         for name, stream in streams.items():
             if stream is streams[stream_name] and name not in STREAM_SYNONYMS:
                 return name
 
     return stream_name
 
 
-def format_valid_streams(plugin: Plugin, streams: Dict[str, Stream]) -> str:
+def format_valid_streams(plugin: Plugin, streams: Mapping[str, Stream]) -> str:
     """Formats a dict of streams.
 
     Filters out synonyms and displays them next to
     the stream they point to.
 
     Streams are sorted according to their quality
     (based on plugin.stream_weight).
@@ -551,53 +542,53 @@
                 retry_streams = args.retry_streams
             if args.retry_max:
                 retry_max = args.retry_max
             streams = fetch_streams_with_retry(plugin, retry_streams, retry_max)
         else:
             streams = fetch_streams(plugin)
     except NoPluginError:
-        console.exit(f"No plugin can handle URL: {args.url}")
+        raise StreamlinkCLIError(f"No plugin can handle URL: {args.url}") from None
     except PluginError as err:
-        console.exit(str(err))
+        raise StreamlinkCLIError() from err
 
     if not streams:
-        console.exit(f"No playable streams found on this URL: {args.url}")
+        raise StreamlinkCLIError(f"No playable streams found on this URL: {args.url}")
 
     if args.default_stream and not args.stream and not args.json:
         args.stream = args.default_stream
 
     if args.stream:
         validstreams = format_valid_streams(plugin, streams)
         for stream_name in args.stream:
             if stream_name in streams:
                 log.info(f"Available streams: {validstreams}")
                 handle_stream(plugin, streams, stream_name)
                 return
 
         errmsg = f"The specified stream(s) '{', '.join(args.stream)}' could not be found"
-        if args.json:
-            console.msg_json(
-                plugin=plugin.module,
-                metadata=plugin.get_metadata(),
-                streams=streams,
-                error=errmsg,
-            )
-        else:
-            console.exit(f"{errmsg}.\n       Available streams: {validstreams}")
+        if not args.json:
+            raise StreamlinkCLIError(f"{errmsg}.\n       Available streams: {validstreams}")
+        console.msg_json(
+            plugin=plugin.module,
+            metadata=plugin.get_metadata(),
+            streams=streams,
+            error=errmsg,
+        )
+        raise StreamlinkCLIError()
     elif args.json:
         console.msg_json(
             plugin=plugin.module,
             metadata=plugin.get_metadata(),
             streams=streams,
         )
     elif args.stream_url:
         try:
             console.msg(streams[list(streams)[-1]].to_manifest_url())
         except TypeError:
-            console.exit("The stream specified cannot be translated to a URL")
+            raise StreamlinkCLIError("The stream specified cannot be translated to a URL") from None
     else:
         validstreams = format_valid_streams(plugin, streams)
         console.msg(f"Available streams: {validstreams}")
 
 
 def print_plugins():
     """Outputs a list of all plugins Streamlink has loaded."""
@@ -956,9 +947,18 @@
 
     return error_code
 
 
 def main():
     parser = build_parser()
     setup(parser)
-    error_code = run(parser)
-    sys.exit(error_code)
+    try:
+        exit_code = run(parser)
+    except StreamlinkCLIError as err:
+        exit_code = err.code
+        if msg := str(err):  # pragma: no branch
+            if console.json:
+                console.msg_json({"error": msg})
+            else:
+                console.msg(f"error: {msg}")
+
+    sys.exit(exit_code)
```

### Comparing `streamlink-6.7.3/src/streamlink_cli/output/abc.py` & `streamlink-6.7.4/src/streamlink_cli/output/abc.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink_cli/output/file.py` & `streamlink-6.7.4/src/streamlink_cli/output/file.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink_cli/output/http.py` & `streamlink-6.7.4/src/streamlink_cli/output/http.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink_cli/output/player.py` & `streamlink-6.7.4/src/streamlink_cli/output/player.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink_cli/streamrunner.py` & `streamlink-6.7.4/src/streamlink_cli/streamrunner.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink_cli/utils/__init__.py` & `streamlink-6.7.4/src/streamlink_cli/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink_cli/utils/formatter.py` & `streamlink-6.7.4/src/streamlink_cli/utils/formatter.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink_cli/utils/path.py` & `streamlink-6.7.4/src/streamlink_cli/utils/path.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink_cli/utils/player.py` & `streamlink-6.7.4/src/streamlink_cli/utils/player.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink_cli/utils/progress.py` & `streamlink-6.7.4/src/streamlink_cli/utils/progress.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/src/streamlink_cli/utils/versioncheck.py` & `streamlink-6.7.4/src/streamlink_cli/utils/versioncheck.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/__init__.py` & `streamlink-6.7.4/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/cli/output/test_file.py` & `streamlink-6.7.4/tests/cli/output/test_file.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/cli/output/test_player.py` & `streamlink-6.7.4/tests/cli/output/test_player.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/cli/test_argparser.py` & `streamlink-6.7.4/tests/cli/test_argparser.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/cli/test_cmdline.py` & `streamlink-6.7.4/tests/cli/test_cmdline.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/cli/test_cmdline_title.py` & `streamlink-6.7.4/tests/cli/test_cmdline_title.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/cli/test_console.py` & `streamlink-6.7.4/tests/cli/test_console.py`

 * *Files 10% similar despite different names*

```diff
@@ -76,38 +76,14 @@
                 "foo": "bar",
                 "baz": "qux"
               }
             ]
         """).lstrip()
         assert test_list1 == ["foo", "bar"]
 
-    def test_msg_json_error(self):
-        output = StringIO()
-        console = ConsoleOutput(output, json=True)
-        with pytest.raises(SystemExit) as cm:
-            console.msg_json({"error": "bad"})
-        assert cm.value.code == 1
-        assert output.getvalue() == '{\n  "error": "bad"\n}\n'
-
-    def test_exit(self):
-        output = StringIO()
-        console = ConsoleOutput(output)
-        with pytest.raises(SystemExit) as cm:
-            console.exit("error")
-        assert cm.value.code == 1
-        assert output.getvalue() == "error: error\n"
-
-    def test_exit_json(self):
-        output = StringIO()
-        console = ConsoleOutput(output, json=True)
-        with pytest.raises(SystemExit) as cm:
-            console.exit("error")
-        assert cm.value.code == 1
-        assert output.getvalue() == '{\n  "error": "error"\n}\n'
-
     def test_ask(self, monkeypatch: pytest.MonkeyPatch):
         monkeypatch.setattr("builtins.input", Mock(return_value="hello"))
 
         output = StringIO()
         console = ConsoleOutput(output)
         assert console.ask("test: ") == "hello"
         assert output.getvalue() == "test: "
```

### Comparing `streamlink-6.7.3/tests/cli/test_main.py` & `streamlink-6.7.4/tests/cli/test_main.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from unittest.mock import Mock, call, patch
 
 import pytest
 
 from streamlink.exceptions import PluginError, StreamError, StreamlinkDeprecationWarning
 from streamlink.stream.stream import Stream
 from streamlink_cli.compat import stdout
+from streamlink_cli.exceptions import StreamlinkCLIError
 from streamlink_cli.main import (
     Formatter,
     NoPluginError,
     create_output,
     format_valid_streams,
     handle_stream,
     handle_url,
@@ -101,21 +102,21 @@
 
 
 class TestCLIMainHandleUrl:
     @pytest.mark.parametrize(("side_effect", "expected"), [
         (NoPluginError("foo"), "No plugin can handle URL: fakeurl"),
         (PluginError("bar"), "bar"),
     ])
-    def test_error(self, side_effect, expected):
-        with patch("streamlink_cli.main.args", Mock(url="fakeurl")), \
-             patch("streamlink_cli.main.streamlink", resolve_url=Mock(side_effect=side_effect)), \
-             patch("streamlink_cli.main.console", exit=Mock(side_effect=SystemExit)) as mock_console:
-            with pytest.raises(SystemExit):
-                handle_url()
-            assert mock_console.exit.mock_calls == [call(expected)]
+    def test_error(self, monkeypatch: pytest.MonkeyPatch, side_effect: Exception, expected: str):
+        monkeypatch.setattr("streamlink_cli.main.args", Namespace(url="fakeurl"))
+        monkeypatch.setattr("streamlink_cli.main.streamlink", Mock(resolve_url=Mock(side_effect=side_effect)))
+        with pytest.raises(StreamlinkCLIError) as excinfo:
+            handle_url()
+        assert str(excinfo.value) == expected
+        assert excinfo.value.code == 1
 
 
 class TestCLIMainJsonAndStreamUrl(unittest.TestCase):
     @patch("streamlink_cli.main.args", json=True, stream_url=True, subprocess_cmdline=False)
     @patch("streamlink_cli.main.console")
     def test_handle_stream_with_json_and_stream_url(self, console, args):
         stream = Mock()
@@ -131,29 +132,29 @@
             metadata=dict(
                 id="test-id-1234-5678",
                 author="Tѥst Āuƭhǿr",
                 category=None,
                 title="Test Title",
             ),
         )]
-        assert console.error.mock_calls == []
         console.msg_json.mock_calls.clear()
 
         args.json = False
         handle_stream(plugin, streams, "best")
         assert console.msg.mock_calls == [call(stream.to_url())]
         assert console.msg_json.mock_calls == []
-        assert console.error.mock_calls == []
         console.msg.mock_calls.clear()
 
         stream.to_url.side_effect = TypeError()
-        handle_stream(plugin, streams, "best")
+        with pytest.raises(StreamlinkCLIError) as excinfo:
+            handle_stream(plugin, streams, "best")
         assert console.msg.mock_calls == []
         assert console.msg_json.mock_calls == []
-        assert console.exit.mock_calls == [call("The stream specified cannot be translated to a URL")]
+        assert str(excinfo.value) == "The stream specified cannot be translated to a URL"
+        assert excinfo.value.code == 1
 
     @patch("streamlink_cli.main.args", json=True, stream_url=True, stream=[], default_stream=[], retry_max=0, retry_streams=0)
     @patch("streamlink_cli.main.console")
     def test_handle_url_with_json_and_stream_url(self, console, args):
         stream = Mock()
         streams = dict(worst=Mock(), best=stream)
 
@@ -177,23 +178,23 @@
             assert console.error.mock_calls == []
             console.msg_json.mock_calls.clear()
 
             args.json = False
             handle_url()
             assert console.msg.mock_calls == [call(stream.to_manifest_url())]
             assert console.msg_json.mock_calls == []
-            assert console.error.mock_calls == []
             console.msg.mock_calls.clear()
 
             stream.to_manifest_url.side_effect = TypeError()
-            handle_url()
+            with pytest.raises(StreamlinkCLIError) as excinfo:
+                handle_url()
             assert console.msg.mock_calls == []
             assert console.msg_json.mock_calls == []
-            assert console.exit.mock_calls == [call("The stream specified cannot be translated to a URL")]
-            console.exit.mock_calls.clear()
+            assert str(excinfo.value) == "The stream specified cannot be translated to a URL"
+            assert excinfo.value.code == 1
 
 
 # TODO: don't use Mock() for mocking args, use a custom argparse.Namespace instead
 class TestCLIMainCreateOutput(unittest.TestCase):
     @patch("streamlink_cli.main.args")
     @patch("streamlink_cli.main.console", Mock())
     @patch("streamlink_cli.main.DEFAULT_STREAM_METADATA", {"title": "bar"})
@@ -351,35 +352,35 @@
         assert output.env == {"VAR1": "abc", "VAR2": "def"}
         assert type(output.record) is FileOutput
         assert output.record.filename is None
         assert output.record.fd is stdout
         assert output.record.record is None
 
     @patch("streamlink_cli.main.args")
-    @patch("streamlink_cli.main.console")
-    def test_create_output_record_and_other_file_output(self, console: Mock, args: Mock):
+    def test_create_output_record_and_other_file_output(self, args: Mock):
         formatter = Formatter({})
         args.output = None
         args.stdout = True
         args.record_and_pipe = True
-        create_output(formatter)
-        console.exit.assert_called_with("Cannot use record options with other file output options.")
+        with pytest.raises(StreamlinkCLIError) as excinfo:
+            create_output(formatter)
+        assert str(excinfo.value) == "Cannot use record options with other file output options."
+        assert excinfo.value.code == 1
 
     @patch("streamlink_cli.main.args")
-    @patch("streamlink_cli.main.console")
-    def test_create_output_no_default_player(self, console: Mock, args: Mock):
+    def test_create_output_no_default_player(self, args: Mock):
         formatter = Formatter({})
         args.output = None
         args.stdout = False
         args.record_and_pipe = False
         args.player = None
-        console.exit.side_effect = SystemExit
-        with pytest.raises(SystemExit):
+        with pytest.raises(StreamlinkCLIError) as excinfo:
             create_output(formatter)
-        assert re.search(r"^The default player \(\w+\) does not seem to be installed\.", console.exit.call_args_list[0][0][0])
+        assert re.search(r"^The default player \(\w+\) does not seem to be installed\.", str(excinfo.value))
+        assert excinfo.value.code == 1
 
 
 class TestCLIMainHandleStream(unittest.TestCase):
     @patch("streamlink_cli.main.output_stream")
     @patch("streamlink_cli.main.args")
     def test_handle_stream_output_stream(self, args: Mock, mock_output_stream: Mock):
         args.json = False
@@ -401,38 +402,38 @@
         assert mock_output_stream.call_count == 1
         paramStream, paramFormatter = mock_output_stream.call_args[0]
         assert paramStream is stream
         assert isinstance(paramFormatter, Formatter)
 
 
 class TestCLIMainOutputStream:
-    def test_stream_failure_no_output_open(self, caplog: pytest.LogCaptureFixture):
+    def test_stream_failure_no_output_open(self, monkeypatch: pytest.MonkeyPatch, caplog: pytest.LogCaptureFixture):
         output = Mock()
         stream = Mock(
             __str__=lambda _: "fake-stream",
             open=Mock(side_effect=StreamError("failure")),
         )
         formatter = Mock()
 
         caplog.set_level(1, "streamlink.cli")
 
-        with patch("streamlink_cli.main.args", Namespace(retry_open=2)), \
-             patch("streamlink_cli.main.console") as mock_console, \
-             patch("streamlink_cli.main.output"), \
-             patch("streamlink_cli.main.create_output", return_value=output):
+        monkeypatch.setattr("streamlink_cli.main.args", Namespace(retry_open=2))
+        monkeypatch.setattr("streamlink_cli.main.output", output)
+        monkeypatch.setattr("streamlink_cli.main.create_output", Mock(return_value=output))
+
+        with pytest.raises(StreamlinkCLIError) as excinfo:
             output_stream(stream, formatter)
 
         assert [(record.levelname, record.module, record.message) for record in caplog.records] == [
             ("error", "main", "Try 1/2: Could not open stream fake-stream (Could not open stream: failure)"),
             ("error", "main", "Try 2/2: Could not open stream fake-stream (Could not open stream: failure)"),
         ]
-        assert mock_console.exit.call_args_list == [
-            call("Could not open stream fake-stream, tried 2 times, exiting"),
-        ]
         assert not output.open.called, "Does not open the output on stream error"
+        assert str(excinfo.value) == "Could not open stream fake-stream, tried 2 times, exiting"
+        assert excinfo.value.code == 1
 
     @pytest.mark.parametrize(
         ("args", "isatty", "deprecation", "expected"),
         [
             ({"progress": "yes", "force_progress": False}, True, False, True),
             ({"progress": "no", "force_progress": False}, True, False, False),
             ({"progress": "yes", "force_progress": False}, False, False, False),
```

### Comparing `streamlink-6.7.3/tests/cli/test_main_check_file_output.py` & `streamlink-6.7.4/tests/cli/test_main_check_file_output.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from contextlib import nullcontext
 from pathlib import Path, PurePosixPath
 from typing import TYPE_CHECKING
 from unittest.mock import Mock, call
 
 import pytest
 
+from streamlink_cli.exceptions import StreamlinkCLIError
 from streamlink_cli.main import check_file_output
 from streamlink_cli.output.file import FileOutput
 
 
 if TYPE_CHECKING:  # pragma: no cover
     _BasePath = PurePosixPath
 else:
@@ -79,15 +80,15 @@
         ],
         id="file exists, force",
     ),
     pytest.param(
         {"exists": True},
         False,
         {"isatty": False},
-        pytest.raises(SystemExit),
+        pytest.raises(StreamlinkCLIError),
         [
             ("streamlink.cli", "info", "Writing output to\n/path/to/file"),
             ("streamlink.cli", "debug", "Checking file output"),
             ("streamlink.cli", "error", "File file already exists, use --force to overwrite it."),
         ],
         id="file exists, no TTY",
     ),
@@ -114,20 +115,20 @@
     pytest.param(
         {"ask": "y"},
         nullcontext(),
         id="yes",
     ),
     pytest.param(
         {"ask": "n"},
-        pytest.raises(SystemExit),
+        pytest.raises(StreamlinkCLIError),
         id="no",
     ),
     pytest.param(
         {"ask": None},
-        pytest.raises(SystemExit),
+        pytest.raises(StreamlinkCLIError),
         id="error",
     ),
 ], indirect=["prompt"])
 def test_prompt(
     caplog: pytest.LogCaptureFixture,
     path: Path,
     prompt: Mock,
```

### Comparing `streamlink-6.7.3/tests/cli/test_main_formatter.py` & `streamlink-6.7.4/tests/cli/test_main_formatter.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/cli/test_main_logging.py` & `streamlink-6.7.4/tests/cli/test_main_logging.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 import pytest
 
 import streamlink_cli.main
 import tests
 from streamlink.session import Streamlink
 from streamlink_cli.argparser import ArgumentParser
+from streamlink_cli.exceptions import StreamlinkCLIError
 from streamlink_cli.main import build_parser
 
 
 @pytest.fixture(autouse=True)
 def argv(request: pytest.FixtureRequest, monkeypatch: pytest.MonkeyPatch):
     argv = getattr(request, "param", [])
     monkeypatch.setattr("sys.argv", ["streamlink", *argv])
@@ -86,22 +87,35 @@
 
     @pytest.mark.parametrize(("argv", "stdout", "stderr"), [
         pytest.param([], "[cli][info] a\n[test_main_logging][error] b\nerror: c\n", "", id="no-pipe-no-json"),
         pytest.param(["--json"], "{\n  \"error\": \"c\"\n}\n", "", id="no-pipe-json"),
         pytest.param(["--stdout"], "", "[cli][info] a\n[test_main_logging][error] b\nerror: c\n", id="pipe-no-json"),
         pytest.param(["--stdout", "--json"], "", "{\n  \"error\": \"c\"\n}\n", id="pipe-json"),
     ], indirect=["argv"])
-    def test_output(self, capsys: pytest.CaptureFixture, parser: ArgumentParser, argv: list, stdout: str, stderr: str):
-        streamlink_cli.main.setup(parser)
-
-        childlogger = logging.getLogger("streamlink.test_main_logging")
-        streamlink_cli.main.log.info("a")
-        childlogger.error("b")
-        with pytest.raises(SystemExit):
-            streamlink_cli.main.console.exit("c")
+    def test_output(
+        self,
+        monkeypatch: pytest.MonkeyPatch,
+        capsys: pytest.CaptureFixture,
+        parser: ArgumentParser,
+        argv: list,
+        stdout: str,
+        stderr: str,
+    ):
+        def run(_parser):
+            childlogger = logging.getLogger("streamlink.test_main_logging")
+            streamlink_cli.main.log.info("a")
+            childlogger.error("b")
+            raise StreamlinkCLIError("c")
+
+        monkeypatch.setattr("streamlink_cli.main.build_parser", lambda: parser)
+        monkeypatch.setattr("streamlink_cli.main.run", run)
+
+        with pytest.raises(SystemExit) as excinfo:
+            streamlink_cli.main.main()
+        assert excinfo.value.code == 1
 
         out, err = capsys.readouterr()
         assert out == stdout
         assert err == stderr
 
 
 class TestInfos:
```

### Comparing `streamlink-6.7.3/tests/cli/test_main_setup_config_args.py` & `streamlink-6.7.4/tests/cli/test_main_setup_config_args.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/cli/test_plugin_args_and_options.py` & `streamlink-6.7.4/tests/cli/test_plugin_args_and_options.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/cli/test_streamrunner.py` & `streamlink-6.7.4/tests/cli/test_streamrunner.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/cli/utils/test_formatter.py` & `streamlink-6.7.4/tests/cli/utils/test_formatter.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/cli/utils/test_path.py` & `streamlink-6.7.4/tests/cli/utils/test_path.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/cli/utils/test_player.py` & `streamlink-6.7.4/tests/cli/utils/test_player.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/cli/utils/test_progress.py` & `streamlink-6.7.4/tests/cli/utils/test_progress.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/cli/utils/test_versioncheck.py` & `streamlink-6.7.4/tests/cli/utils/test_versioncheck.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/conftest.py` & `streamlink-6.7.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/mixins/stream_hls.py` & `streamlink-6.7.4/tests/mixins/stream_hls.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/plugin/testplugin.py` & `streamlink-6.7.4/tests/plugin/testplugin.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/plugins/__init__.py` & `streamlink-6.7.4/tests/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/plugins/conftest.py` & `streamlink-6.7.4/tests/plugins/conftest.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/plugins/test_abematv.py` & `streamlink-6.7.4/tests/plugins/test_abematv.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/plugins/test_adultswim.py` & `streamlink-6.7.4/tests/plugins/test_adultswim.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/plugins/test_afreeca.py` & `streamlink-6.7.4/tests/plugins/test_afreeca.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/plugins/test_albavision.py` & `streamlink-6.7.4/tests/plugins/test_albavision.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/plugins/test_aloula.py` & `streamlink-6.7.4/tests/plugins/test_aloula.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/plugins/test_ard_mediathek.py` & `streamlink-6.7.4/tests/plugins/test_ard_mediathek.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/plugins/test_artetv.py` & `streamlink-6.7.4/tests/plugins/test_artetv.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/plugins/test_atpchallenger.py` & `streamlink-6.7.4/tests/plugins/test_atpchallenger.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/plugins/test_atresplayer.py` & `streamlink-6.7.4/tests/plugins/test_atresplayer.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/plugins/test_bbciplayer.py` & `streamlink-6.7.4/tests/plugins/test_bbciplayer.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/plugins/test_bfmtv.py` & `streamlink-6.7.4/tests/plugins/test_bfmtv.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/plugins/test_blazetv.py` & `streamlink-6.7.4/tests/plugins/test_blazetv.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/plugins/test_bloomberg.py` & `streamlink-6.7.4/tests/plugins/test_bloomberg.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/plugins/test_booyah.py` & `streamlink-6.7.4/tests/plugins/test_booyah.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/plugins/test_cbsnews.py` & `streamlink-6.7.4/tests/plugins/test_cbsnews.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/plugins/test_cdnbg.py` & `streamlink-6.7.4/tests/plugins/test_cdnbg.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/plugins/test_ceskatelevize.py` & `streamlink-6.7.4/tests/plugins/test_ceskatelevize.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/plugins/test_cinergroup.py` & `streamlink-6.7.4/tests/plugins/test_cinergroup.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/plugins/test_cmmedia.py` & `streamlink-6.7.4/tests/plugins/test_cmmedia.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/plugins/test_crunchyroll.py` & `streamlink-6.7.4/tests/plugins/test_crunchyroll.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/plugins/test_dailymotion.py` & `streamlink-6.7.4/tests/plugins/test_dailymotion.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/plugins/test_dash.py` & `streamlink-6.7.4/tests/plugins/test_dash.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/plugins/test_delfi.py` & `streamlink-6.7.4/tests/plugins/test_delfi.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/plugins/test_deutschewelle.py` & `streamlink-6.7.4/tests/plugins/test_deutschewelle.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/plugins/test_dlive.py` & `streamlink-6.7.4/tests/plugins/test_dlive.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/plugins/test_dogan.py` & `streamlink-6.7.4/tests/plugins/test_dogan.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/plugins/test_drdk.py` & `streamlink-6.7.4/tests/plugins/test_drdk.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/plugins/test_euronews.py` & `streamlink-6.7.4/tests/plugins/test_euronews.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/plugins/test_facebook.py` & `streamlink-6.7.4/tests/plugins/test_facebook.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/plugins/test_filmon.py` & `streamlink-6.7.4/tests/plugins/test_filmon.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/plugins/test_goltelevision.py` & `streamlink-6.7.4/tests/plugins/test_goltelevision.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/plugins/test_goodgame.py` & `streamlink-6.7.4/tests/plugins/test_goodgame.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/plugins/test_gulli.py` & `streamlink-6.7.4/tests/plugins/test_gulli.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/plugins/test_hls.py` & `streamlink-6.7.4/tests/plugins/test_hls.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/plugins/test_http.py` & `streamlink-6.7.4/tests/plugins/test_http.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/plugins/test_htv.py` & `streamlink-6.7.4/tests/plugins/test_htv.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/plugins/test_idf1.py` & `streamlink-6.7.4/tests/plugins/test_idf1.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/plugins/test_invintus.py` & `streamlink-6.7.4/tests/plugins/test_invintus.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/plugins/test_kugou.py` & `streamlink-6.7.4/tests/plugins/test_kugou.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/plugins/test_livestream.py` & `streamlink-6.7.4/tests/plugins/test_livestream.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/plugins/test_lnk.py` & `streamlink-6.7.4/tests/plugins/test_lnk.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/plugins/test_lrt.py` & `streamlink-6.7.4/tests/plugins/test_lrt.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/plugins/test_ltv_lsm_lv.py` & `streamlink-6.7.4/tests/plugins/test_ltv_lsm_lv.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/plugins/test_mangomolo.py` & `streamlink-6.7.4/tests/plugins/test_mangomolo.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/plugins/test_mdstrm.py` & `streamlink-6.7.4/tests/plugins/test_mdstrm.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/plugins/test_mediaklikk.py` & `streamlink-6.7.4/tests/plugins/test_mediaklikk.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/plugins/test_mediavitrina.py` & `streamlink-6.7.4/tests/plugins/test_mediavitrina.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/plugins/test_mitele.py` & `streamlink-6.7.4/tests/plugins/test_mitele.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/plugins/test_mixcloud.py` & `streamlink-6.7.4/tests/plugins/test_mixcloud.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/plugins/test_n13tv.py` & `streamlink-6.7.4/tests/plugins/test_n13tv.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/plugins/test_nasaplus.py` & `streamlink-6.7.4/tests/plugins/test_nasaplus.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/plugins/test_nicolive.py` & `streamlink-6.7.4/tests/plugins/test_nicolive.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/plugins/test_nos.py` & `streamlink-6.7.4/tests/plugins/test_nos.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/plugins/test_nrk.py` & `streamlink-6.7.4/tests/plugins/test_nrk.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/plugins/test_olympicchannel.py` & `streamlink-6.7.4/tests/plugins/test_olympicchannel.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/plugins/test_oneplusone.py` & `streamlink-6.7.4/tests/plugins/test_oneplusone.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/plugins/test_onetv.py` & `streamlink-6.7.4/tests/plugins/test_onetv.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/plugins/test_piaulizaportal.py` & `streamlink-6.7.4/tests/plugins/test_piaulizaportal.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/plugins/test_picarto.py` & `streamlink-6.7.4/tests/plugins/test_picarto.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/plugins/test_pluto.py` & `streamlink-6.7.4/tests/plugins/test_pluto.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/plugins/test_pluzz.py` & `streamlink-6.7.4/tests/plugins/test_pluzz.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/plugins/test_radionet.py` & `streamlink-6.7.4/tests/plugins/test_radionet.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/plugins/test_raiplay.py` & `streamlink-6.7.4/tests/plugins/test_raiplay.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/plugins/test_reuters.py` & `streamlink-6.7.4/tests/plugins/test_reuters.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/plugins/test_rtpplay.py` & `streamlink-6.7.4/tests/plugins/test_rtpplay.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/plugins/test_rtve.py` & `streamlink-6.7.4/tests/plugins/test_rtve.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/plugins/test_rtvs.py` & `streamlink-6.7.4/tests/plugins/test_rtvs.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/plugins/test_ruv.py` & `streamlink-6.7.4/tests/plugins/test_ruv.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/plugins/test_sbscokr.py` & `streamlink-6.7.4/tests/plugins/test_sbscokr.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/plugins/test_showroom.py` & `streamlink-6.7.4/tests/plugins/test_showroom.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/plugins/test_steam.py` & `streamlink-6.7.4/tests/plugins/test_steam.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/plugins/test_streann.py` & `streamlink-6.7.4/tests/plugins/test_streann.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/plugins/test_svtplay.py` & `streamlink-6.7.4/tests/plugins/test_svtplay.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/plugins/test_swisstxt.py` & `streamlink-6.7.4/tests/plugins/test_swisstxt.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/plugins/test_telefe.py` & `streamlink-6.7.4/tests/plugins/test_telefe.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/plugins/test_tf1.py` & `streamlink-6.7.4/tests/plugins/test_tf1.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/plugins/test_trovo.py` & `streamlink-6.7.4/tests/plugins/test_trovo.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/plugins/test_turkuvaz.py` & `streamlink-6.7.4/tests/plugins/test_turkuvaz.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,17 +24,15 @@
         "https://vavtv.com.tr/canli-yayin",  # vavtv
 
         # vods
         "https://www.ahaber.com.tr/video/yasam-videolari/samsunda-sel-sularindan-kacma-ani-kamerada",
         "https://www.anews.com.tr/webtv/world/pro-ukraine-militia-says-it-has-captured-russian-soldiers",
         "https://www.apara.com.tr/video/ekonomide-bugun/bist-100de-kar-satislari-derinlesir-mi",
         "https://www.aspor.com.tr/webtv/galatasaray/galatasaraydan-forma-tanitiminda-fenerbahceye-gonderme",
-        "https://www.atv.com.tr/kurulus-osman/127-bolum/izle",
         "https://www.atvavrupa.tv/diger-program//ozelvideo/izle",
-        "https://www.minikacocuk.com.tr/webtv/olly/bolum/olly-eylul-tanitim",
         "https://www.minikago.com.tr/webtv/mondo-yan/bolum/mondo-yan-eylul-tanitim",
         "https://vavtv.com.tr/vavradyo/video/guncel/munafiklarin-ozellikleri-nelerdir",
 
         # other links for info/doc
         "https://www.atv.com.tr/webtv/canli-yayin",  # redirect to atv.com.tr/canli-yayin
         "https://www.ahaber.com.tr/canli-yayin-atv.html",  # links to atv.com.tr/webtv/canli-yayin
     ]
```

### Comparing `streamlink-6.7.3/tests/plugins/test_tv3cat.py` & `streamlink-6.7.4/tests/plugins/test_tv3cat.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/plugins/test_tv4play.py` & `streamlink-6.7.4/tests/plugins/test_tv4play.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/plugins/test_tv5monde.py` & `streamlink-6.7.4/tests/plugins/test_tv5monde.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/plugins/test_tvp.py` & `streamlink-6.7.4/tests/plugins/test_tvp.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/plugins/test_tvrby.py` & `streamlink-6.7.4/tests/plugins/test_tvrby.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/plugins/test_tvrplus.py` & `streamlink-6.7.4/tests/plugins/test_tvrplus.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/plugins/test_twitch.py` & `streamlink-6.7.4/tests/plugins/test_twitch.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/plugins/test_ustreamtv.py` & `streamlink-6.7.4/tests/plugins/test_ustreamtv.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/plugins/test_ustvnow.py` & `streamlink-6.7.4/tests/plugins/test_ustvnow.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/plugins/test_vimeo.py` & `streamlink-6.7.4/tests/plugins/test_vimeo.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/plugins/test_vinhlongtv.py` & `streamlink-6.7.4/tests/plugins/test_vinhlongtv.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/plugins/test_vk.py` & `streamlink-6.7.4/tests/plugins/test_vk.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/plugins/test_vkplay.py` & `streamlink-6.7.4/tests/plugins/test_vkplay.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/plugins/test_vtvgo.py` & `streamlink-6.7.4/tests/plugins/test_vtvgo.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/plugins/test_webtv.py` & `streamlink-6.7.4/tests/plugins/test_webtv.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/plugins/test_welt.py` & `streamlink-6.7.4/tests/plugins/test_welt.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/plugins/test_youtube.py` & `streamlink-6.7.4/tests/plugins/test_youtube.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/plugins/test_zattoo.py` & `streamlink-6.7.4/tests/plugins/test_zattoo.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/plugins/test_zdf_mediathek.py` & `streamlink-6.7.4/tests/plugins/test_zdf_mediathek.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/plugins/test_zengatv.py` & `streamlink-6.7.4/tests/plugins/test_zengatv.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/resources/__init__.py` & `streamlink-6.7.4/tests/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/resources/dash/test_1.mpd` & `streamlink-6.7.4/tests/resources/dash/test_1.mpd`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/resources/dash/test_10.mpd` & `streamlink-6.7.4/tests/resources/dash/test_10.mpd`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/resources/dash/test_11_static.mpd` & `streamlink-6.7.4/tests/resources/dash/test_11_static.mpd`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/resources/dash/test_2.mpd` & `streamlink-6.7.4/tests/resources/dash/test_2.mpd`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/resources/dash/test_3.mpd` & `streamlink-6.7.4/tests/resources/dash/test_3.mpd`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/resources/dash/test_8.mpd` & `streamlink-6.7.4/tests/resources/dash/test_8.mpd`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/resources/dash/test_9.mpd` & `streamlink-6.7.4/tests/resources/dash/test_9.mpd`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/resources/dash/test_dynamic_segment_list_no_duration.mpd` & `streamlink-6.7.4/tests/resources/dash/test_dynamic_segment_list_no_duration.mpd`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/resources/dash/test_dynamic_segment_list_p1.mpd` & `streamlink-6.7.4/tests/resources/dash/test_dynamic_segment_list_p1.mpd`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/resources/dash/test_dynamic_segment_list_p2.mpd` & `streamlink-6.7.4/tests/resources/dash/test_dynamic_segment_list_p2.mpd`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/resources/dash/test_dynamic_segment_list_p3.mpd` & `streamlink-6.7.4/tests/resources/dash/test_dynamic_segment_list_p3.mpd`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/resources/dash/test_dynamic_segment_list_p4.mpd` & `streamlink-6.7.4/tests/resources/dash/test_dynamic_segment_list_p4.mpd`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/resources/dash/test_dynamic_segment_list_p5.mpd` & `streamlink-6.7.4/tests/resources/dash/test_dynamic_segment_list_p5.mpd`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/resources/dash/test_dynamic_timeline_continued_p1.mpd` & `streamlink-6.7.4/tests/resources/dash/test_dynamic_timeline_continued_p1.mpd`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/resources/dash/test_dynamic_timeline_continued_p2.mpd` & `streamlink-6.7.4/tests/resources/dash/test_dynamic_timeline_continued_p2.mpd`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/resources/dash/test_nested_baseurls.mpd` & `streamlink-6.7.4/tests/resources/dash/test_nested_baseurls.mpd`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/resources/dash/test_no_segment_list_or_template.mpd` & `streamlink-6.7.4/tests/resources/dash/test_no_segment_list_or_template.mpd`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/resources/dash/test_segment_list.mpd` & `streamlink-6.7.4/tests/resources/dash/test_segment_list.mpd`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/resources/dash/test_segments_byterange.mpd` & `streamlink-6.7.4/tests/resources/dash/test_segments_byterange.mpd`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/resources/dash/test_segments_dynamic_number.mpd` & `streamlink-6.7.4/tests/resources/dash/test_segments_dynamic_number.mpd`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/resources/dash/test_static_no_publish_time.mpd` & `streamlink-6.7.4/tests/resources/dash/test_static_no_publish_time.mpd`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/resources/dash/test_suggested_presentation_delay.mpd` & `streamlink-6.7.4/tests/resources/dash/test_suggested_presentation_delay.mpd`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/resources/dash/test_timeline_ids.mpd` & `streamlink-6.7.4/tests/resources/dash/test_timeline_ids.mpd`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/resources/hls/test_1.m3u8` & `streamlink-6.7.4/tests/resources/hls/test_1.m3u8`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/resources/hls/test_2.m3u8` & `streamlink-6.7.4/tests/resources/hls/test_2.m3u8`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/resources/hls/test_date.m3u8` & `streamlink-6.7.4/tests/resources/hls/test_date.m3u8`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/resources/hls/test_master.m3u8` & `streamlink-6.7.4/tests/resources/hls/test_master.m3u8`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/resources/hls/test_master_twitch_vod.m3u8` & `streamlink-6.7.4/tests/resources/hls/test_master_twitch_vod.m3u8`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/resources/hls/test_multivariant_bandwidth.m3u8` & `streamlink-6.7.4/tests/resources/hls/test_multivariant_bandwidth.m3u8`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/session/test_http.py` & `streamlink-6.7.4/tests/session/test_http.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/session/test_options.py` & `streamlink-6.7.4/tests/session/test_options.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/session/test_plugins.py` & `streamlink-6.7.4/tests/session/test_plugins.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/session/test_session.py` & `streamlink-6.7.4/tests/session/test_session.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/stream/dash/test_dash.py` & `streamlink-6.7.4/tests/stream/dash/test_dash.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/stream/dash/test_manifest.py` & `streamlink-6.7.4/tests/stream/dash/test_manifest.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/stream/hls/test_hls.py` & `streamlink-6.7.4/tests/stream/hls/test_hls.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/stream/hls/test_hls_filtered.py` & `streamlink-6.7.4/tests/stream/hls/test_hls_filtered.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/stream/hls/test_m3u8.py` & `streamlink-6.7.4/tests/stream/hls/test_m3u8.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/stream/test_ffmpegmux.py` & `streamlink-6.7.4/tests/stream/test_ffmpegmux.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/stream/test_file.py` & `streamlink-6.7.4/tests/stream/test_file.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/stream/test_stream_json.py` & `streamlink-6.7.4/tests/stream/test_stream_json.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/stream/test_stream_to_url.py` & `streamlink-6.7.4/tests/stream/test_stream_to_url.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/stream/test_stream_wrappers.py` & `streamlink-6.7.4/tests/stream/test_stream_wrappers.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/test_api_validate.py` & `streamlink-6.7.4/tests/test_api_validate.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/test_api_websocket.py` & `streamlink-6.7.4/tests/test_api_websocket.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/test_buffers.py` & `streamlink-6.7.4/tests/test_buffers.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/test_cache.py` & `streamlink-6.7.4/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/test_compat.py` & `streamlink-6.7.4/tests/test_compat.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/test_logger.py` & `streamlink-6.7.4/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/test_options.py` & `streamlink-6.7.4/tests/test_options.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/test_plugin.py` & `streamlink-6.7.4/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/test_plugin_userinput.py` & `streamlink-6.7.4/tests/test_plugin_userinput.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/test_plugins.py` & `streamlink-6.7.4/tests/test_plugins.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/test_streamlink_api.py` & `streamlink-6.7.4/tests/test_streamlink_api.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/testutils/handshake.py` & `streamlink-6.7.4/tests/testutils/handshake.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,15 +80,15 @@
 
 
 def _sync2async(obj, name, method):
     meth = getattr(obj, method)
 
     @wraps(meth)
     async def wrapper(*args, **kwargs):
-        async def task():
+        async def task():  # noqa: RUF029
             try:
                 value = meth(*args, **kwargs)
             except Exception as err:
                 future.set_exception(err)
             else:
                 future.set_result(value)
```

### Comparing `streamlink-6.7.3/tests/testutils/test_handshake.py` & `streamlink-6.7.4/tests/testutils/test_handshake.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/utils/test_args.py` & `streamlink-6.7.4/tests/utils/test_args.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/utils/test_cache.py` & `streamlink-6.7.4/tests/utils/test_cache.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/utils/test_crypto.py` & `streamlink-6.7.4/tests/utils/test_crypto.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/utils/test_data.py` & `streamlink-6.7.4/tests/utils/test_data.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/utils/test_formatter.py` & `streamlink-6.7.4/tests/utils/test_formatter.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/utils/test_l10n.py` & `streamlink-6.7.4/tests/utils/test_l10n.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/utils/test_module.py` & `streamlink-6.7.4/tests/utils/test_module.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/utils/test_named_pipe.py` & `streamlink-6.7.4/tests/utils/test_named_pipe.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/utils/test_parse.py` & `streamlink-6.7.4/tests/utils/test_parse.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/utils/test_path.py` & `streamlink-6.7.4/tests/utils/test_path.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/utils/test_processoutput.py` & `streamlink-6.7.4/tests/utils/test_processoutput.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/utils/test_random.py` & `streamlink-6.7.4/tests/utils/test_random.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/utils/test_times.py` & `streamlink-6.7.4/tests/utils/test_times.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/utils/test_url.py` & `streamlink-6.7.4/tests/utils/test_url.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/webbrowser/cdp/__init__.py` & `streamlink-6.7.4/tests/webbrowser/cdp/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/webbrowser/cdp/conftest.py` & `streamlink-6.7.4/tests/webbrowser/cdp/conftest.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/webbrowser/cdp/test_client.py` & `streamlink-6.7.4/tests/webbrowser/cdp/test_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from contextlib import nullcontext
 from typing import Awaitable, Callable, Union, cast
 from unittest.mock import ANY, AsyncMock, Mock, call
 
 import pytest
 import trio
-from exceptiongroup import ExceptionGroup
 from trio.testing import wait_all_tasks_blocked
 
+from streamlink.compat import ExceptionGroup
 from streamlink.session import Streamlink
 from streamlink.webbrowser.cdp.client import CDPClient, CDPClientSession, RequestPausedHandler
 from streamlink.webbrowser.cdp.connection import CDPConnection, CDPSession
 from streamlink.webbrowser.cdp.devtools.fetch import RequestPaused
 from streamlink.webbrowser.cdp.devtools.target import SessionID, TargetID
 from streamlink.webbrowser.cdp.exceptions import CDPError
 from tests.webbrowser.cdp import FakeWebsocketConnection
@@ -38,15 +38,15 @@
 @pytest.fixture()
 async def cdp_client(session: Streamlink, chromium_webbrowser: Mock, websocket_connection: FakeWebsocketConnection):
     async with CDPClient.run(session) as cdp_client:
         yield cdp_client
 
 
 @pytest.fixture()
-async def cdp_client_session(request: pytest.FixtureRequest, cdp_client: CDPClient):
+def cdp_client_session(request: pytest.FixtureRequest, cdp_client: CDPClient):
     target_id = TargetID("01234")
     session_id = SessionID("56789")
     session = cdp_client.cdp_connection.sessions[session_id] = CDPSession(
         cdp_client.cdp_connection.websocket,
         target_id=target_id,
         session_id=session_id,
         cmd_timeout=cdp_client.cdp_connection.cmd_timeout,
```

### Comparing `streamlink-6.7.3/tests/webbrowser/cdp/test_connection.py` & `streamlink-6.7.4/tests/webbrowser/cdp/test_connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 from dataclasses import dataclass
 from functools import partial
 from typing import Dict, Generator, Optional, Type
 from unittest.mock import AsyncMock
 
 import pytest
 import trio
-from exceptiongroup import ExceptionGroup
 from trio.testing import MockClock, wait_all_tasks_blocked
 from trio_websocket import CloseReason, ConnectionClosed, ConnectionTimeout  # type: ignore[import]
 
+from streamlink.compat import ExceptionGroup
 from streamlink.webbrowser.cdp.connection import CDPConnection, CDPEventListener, CDPSession
 from streamlink.webbrowser.cdp.devtools.target import SessionID, TargetID
 from streamlink.webbrowser.cdp.devtools.util import T_JSON_DICT
 from streamlink.webbrowser.cdp.exceptions import CDPError
 from tests.webbrowser.cdp import FakeWebsocketConnection
```

### Comparing `streamlink-6.7.3/tests/webbrowser/conftest.py` & `streamlink-6.7.4/tests/webbrowser/conftest.py`

 * *Files identical despite different names*

### Comparing `streamlink-6.7.3/tests/webbrowser/test_chromium.py` & `streamlink-6.7.4/tests/webbrowser/test_chromium.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,14 +110,15 @@
 
 
 @pytest.mark.trio()
 @pytest.mark.parametrize("host", ["127.0.0.1", "::1"])
 @pytest.mark.parametrize("port", [None, 1234])
 async def test_launch(monkeypatch: pytest.MonkeyPatch, mock_clock, webbrowser_launch, host, port):
     async def fake_find_free_port(_):
+        await trio.sleep(0)
         return 1234
 
     monkeypatch.setattr("streamlink.webbrowser.chromium.find_free_port_ipv4", fake_find_free_port)
     monkeypatch.setattr("streamlink.webbrowser.chromium.find_free_port_ipv6", fake_find_free_port)
 
     webbrowser = ChromiumWebbrowser(host=host, port=port)
```

### Comparing `streamlink-6.7.3/tests/webbrowser/test_webbrowser.py` & `streamlink-6.7.4/tests/webbrowser/test_webbrowser.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,17 +3,16 @@
 from contextlib import AbstractContextManager, nullcontext
 from pathlib import Path
 from signal import SIGTERM
 from typing import List, Optional
 
 import pytest
 import trio
-from exceptiongroup import BaseExceptionGroup
 
-from streamlink.compat import is_win32
+from streamlink.compat import BaseExceptionGroup, is_win32
 from streamlink.webbrowser.exceptions import WebbrowserError
 from streamlink.webbrowser.webbrowser import Webbrowser
 
 
 class _FakeWebbrowser(Webbrowser):
     @classmethod
     def launch_args(cls) -> List[str]:
```

