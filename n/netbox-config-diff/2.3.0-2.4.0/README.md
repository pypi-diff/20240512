# Comparing `tmp/netbox-config-diff-2.3.0.tar.gz` & `tmp/netbox_config_diff-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox-config-diff-2.3.0.tar", last modified: Thu Apr 11 13:48:39 2024, max compression
+gzip compressed data, was "netbox_config_diff-2.4.0.tar", last modified: Sun May 12 16:10:59 2024, max compression
```

## Comparing `netbox-config-diff-2.3.0.tar` & `netbox_config_diff-2.4.0.tar`

### file list

```diff
@@ -1,123 +1,127 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:48:39.202831 netbox-config-diff-2.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    19230 2024-04-11 13:48:39.202831 netbox-config-diff-2.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4969 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:48:39.186831 netbox-config-diff-2.3.0/development/
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/development/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:48:39.182831 netbox-config-diff-2.3.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:48:39.182831 netbox-config-diff-2.3.0/docs/media/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:48:39.190831 netbox-config-diff-2.3.0/docs/media/screenshots/
--rw-r--r--   0 runner    (1001) docker     (127)    31744 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/docs/media/screenshots/compliance-diff.png
--rw-r--r--   0 runner    (1001) docker     (127)    48801 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/docs/media/screenshots/compliance-error.png
--rw-r--r--   0 runner    (1001) docker     (127)    23740 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/docs/media/screenshots/compliance-list.png
--rw-r--r--   0 runner    (1001) docker     (127)    27108 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/docs/media/screenshots/compliance-missing-extra.png
--rw-r--r--   0 runner    (1001) docker     (127)    17602 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/docs/media/screenshots/compliance-ok.png
--rw-r--r--   0 runner    (1001) docker     (127)     9975 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/docs/media/screenshots/config-temp-substitute.png
--rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/docs/media/screenshots/cr-approve-button.png
--rw-r--r--   0 runner    (1001) docker     (127)    14192 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/docs/media/screenshots/cr-approved.png
--rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/docs/media/screenshots/cr-collecting-diff-button.png
--rw-r--r--   0 runner    (1001) docker     (127)    48412 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/docs/media/screenshots/cr-completed.png
--rw-r--r--   0 runner    (1001) docker     (127)    42240 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/docs/media/screenshots/cr-created.png
--rw-r--r--   0 runner    (1001) docker     (127)    65258 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/docs/media/screenshots/cr-diffs-tab.png
--rw-r--r--   0 runner    (1001) docker     (127)    20845 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/docs/media/screenshots/cr-job-log.png
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/docs/media/screenshots/cr-schedule-button.png
--rw-r--r--   0 runner    (1001) docker     (127)    14945 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/docs/media/screenshots/cr-scheduled.png
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/docs/media/screenshots/cr-unapprove-button.png
--rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/docs/media/screenshots/cr-unschedule-button.png
--rw-r--r--   0 runner    (1001) docker     (127)     9572 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/docs/media/screenshots/navbar.png
--rw-r--r--   0 runner    (1001) docker     (127)    28028 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/docs/media/screenshots/platformsetting.png
--rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/docs/media/screenshots/render-temp-substitute.png
--rw-r--r--   0 runner    (1001) docker     (127)    14783 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/docs/media/screenshots/script-list.png
--rw-r--r--   0 runner    (1001) docker     (127)    43979 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/docs/media/screenshots/script.png
--rw-r--r--   0 runner    (1001) docker     (127)    15868 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/docs/media/screenshots/substitute.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:48:39.190831 netbox-config-diff-2.3.0/netbox_config_diff/
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/netbox_config_diff/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:48:39.194831 netbox-config-diff-2.3.0/netbox_config_diff/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/netbox_config_diff/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5708 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/netbox_config_diff/api/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/netbox_config_diff/api/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     7891 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/netbox_config_diff/api/views.py
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/netbox_config_diff/choices.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:48:39.194831 netbox-config-diff-2.3.0/netbox_config_diff/compliance/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/netbox_config_diff/compliance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8722 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/netbox_config_diff/compliance/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/netbox_config_diff/compliance/secrets.py
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/netbox_config_diff/compliance/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:48:39.194831 netbox-config-diff-2.3.0/netbox_config_diff/configurator/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/netbox_config_diff/configurator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9773 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/netbox_config_diff/configurator/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/netbox_config_diff/configurator/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3924 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/netbox_config_diff/configurator/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     7258 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/netbox_config_diff/configurator/platforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/netbox_config_diff/configurator/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/netbox_config_diff/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4054 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/netbox_config_diff/filtersets.py
--rw-r--r--   0 runner    (1001) docker     (127)     6641 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/netbox_config_diff/forms.py
--rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/netbox_config_diff/graphql.py
--rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/netbox_config_diff/jobs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:48:39.198831 netbox-config-diff-2.3.0/netbox_config_diff/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/netbox_config_diff/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/netbox_config_diff/migrations/0002_add_script.py
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/netbox_config_diff/migrations/0003_configcompliance_actual_config_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)      925 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/netbox_config_diff/migrations/0004_update_script.py
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/netbox_config_diff/migrations/0005_configcompliance_extra_missing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/netbox_config_diff/migrations/0006_substitute.py
--rw-r--r--   0 runner    (1001) docker     (127)     2909 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/netbox_config_diff/migrations/0007_configurationrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/netbox_config_diff/migrations/0008_alter_configcompliance_device.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/netbox_config_diff/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:48:39.198831 netbox-config-diff-2.3.0/netbox_config_diff/models/
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/netbox_config_diff/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/netbox_config_diff/models/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4762 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/netbox_config_diff/models/data_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     7016 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/netbox_config_diff/models/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/netbox_config_diff/navigation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:48:39.198831 netbox-config-diff-2.3.0/netbox_config_diff/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/netbox_config_diff/scripts/config_diff.py
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/netbox_config_diff/search.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:48:39.182831 netbox-config-diff-2.3.0/netbox_config_diff/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:48:39.198831 netbox-config-diff-2.3.0/netbox_config_diff/static/netbox_config_diff/
--rw-r--r--   0 runner    (1001) docker     (127)  1000358 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/netbox_config_diff/static/netbox_config_diff/diff2html-ui.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     6661 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/netbox_config_diff/static/netbox_config_diff/diff2html.dark.min.css
--rw-r--r--   0 runner    (1001) docker     (127)     6543 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/netbox_config_diff/static/netbox_config_diff/diff2html.min.css
--rw-r--r--   0 runner    (1001) docker     (127)     2968 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/netbox_config_diff/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:48:39.186831 netbox-config-diff-2.3.0/netbox_config_diff/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:48:39.198831 netbox-config-diff-2.3.0/netbox_config_diff/templates/netbox_config_diff/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:48:39.198831 netbox-config-diff-2.3.0/netbox_config_diff/templates/netbox_config_diff/configcompliance/
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/netbox_config_diff/templates/netbox_config_diff/configcompliance/config.html
--rw-r--r--   0 runner    (1001) docker     (127)     2673 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/netbox_config_diff/templates/netbox_config_diff/configcompliance/data.html
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/netbox_config_diff/templates/netbox_config_diff/configcompliance/missing_extra.html
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/netbox_config_diff/templates/netbox_config_diff/configcompliance.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:48:39.202831 netbox-config-diff-2.3.0/netbox_config_diff/templates/netbox_config_diff/configurationrequest/
--rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/netbox_config_diff/templates/netbox_config_diff/configurationrequest/base.html
--rw-r--r--   0 runner    (1001) docker     (127)     3561 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/netbox_config_diff/templates/netbox_config_diff/configurationrequest/diffs.html
--rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/netbox_config_diff/templates/netbox_config_diff/configurationrequest.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:48:39.202831 netbox-config-diff-2.3.0/netbox_config_diff/templates/netbox_config_diff/inc/
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/netbox_config_diff/templates/netbox_config_diff/inc/diff.html
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/netbox_config_diff/templates/netbox_config_diff/inc/job_log.html
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/netbox_config_diff/templates/netbox_config_diff/platformsetting.html
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/netbox_config_diff/templates/netbox_config_diff/substitute.html
--rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/netbox_config_diff/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:48:39.202831 netbox-config-diff-2.3.0/netbox_config_diff/views/
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/netbox_config_diff/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/netbox_config_diff/views/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6839 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/netbox_config_diff/views/compliance.py
--rw-r--r--   0 runner    (1001) docker     (127)    12412 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/netbox_config_diff/views/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:48:39.202831 netbox-config-diff-2.3.0/netbox_config_diff.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    19230 2024-04-11 13:48:39.000000 netbox-config-diff-2.3.0/netbox_config_diff.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4177 2024-04-11 13:48:39.000000 netbox-config-diff-2.3.0/netbox_config_diff.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 13:48:39.000000 netbox-config-diff-2.3.0/netbox_config_diff.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-11 13:48:39.000000 netbox-config-diff-2.3.0/netbox_config_diff.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-11 13:48:39.000000 netbox-config-diff-2.3.0/netbox_config_diff.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:48:39.202831 netbox-config-diff-2.3.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 13:48:39.202831 netbox-config-diff-2.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:48:39.202831 netbox-config-diff-2.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2886 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/tests/factories.py
--rw-r--r--   0 runner    (1001) docker     (127)     6056 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/tests/test_compliance.py
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/tests/test_compliance_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-04-11 13:48:24.000000 netbox-config-diff-2.3.0/tests/test_urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:10:59.306658 netbox_config_diff-2.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-05-12 16:10:45.000000 netbox_config_diff-2.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-12 16:10:45.000000 netbox_config_diff-2.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    19264 2024-05-12 16:10:59.302658 netbox_config_diff-2.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4969 2024-05-12 16:10:45.000000 netbox_config_diff-2.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:10:59.282658 netbox_config_diff-2.4.0/development/
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-12 16:10:45.000000 netbox_config_diff-2.4.0/development/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:10:59.278658 netbox_config_diff-2.4.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:10:59.278658 netbox_config_diff-2.4.0/docs/media/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:10:59.290658 netbox_config_diff-2.4.0/docs/media/screenshots/
+-rw-r--r--   0 runner    (1001) docker     (127)    31744 2024-05-12 16:10:45.000000 netbox_config_diff-2.4.0/docs/media/screenshots/compliance-diff.png
+-rw-r--r--   0 runner    (1001) docker     (127)    48801 2024-05-12 16:10:45.000000 netbox_config_diff-2.4.0/docs/media/screenshots/compliance-error.png
+-rw-r--r--   0 runner    (1001) docker     (127)    23740 2024-05-12 16:10:45.000000 netbox_config_diff-2.4.0/docs/media/screenshots/compliance-list.png
+-rw-r--r--   0 runner    (1001) docker     (127)    27108 2024-05-12 16:10:45.000000 netbox_config_diff-2.4.0/docs/media/screenshots/compliance-missing-extra.png
+-rw-r--r--   0 runner    (1001) docker     (127)    17602 2024-05-12 16:10:45.000000 netbox_config_diff-2.4.0/docs/media/screenshots/compliance-ok.png
+-rw-r--r--   0 runner    (1001) docker     (127)    26518 2024-05-12 16:10:45.000000 netbox_config_diff-2.4.0/docs/media/screenshots/compliance-patch.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9975 2024-05-12 16:10:45.000000 netbox_config_diff-2.4.0/docs/media/screenshots/config-temp-substitute.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-05-12 16:10:45.000000 netbox_config_diff-2.4.0/docs/media/screenshots/cr-approve-button.png
+-rw-r--r--   0 runner    (1001) docker     (127)    14192 2024-05-12 16:10:45.000000 netbox_config_diff-2.4.0/docs/media/screenshots/cr-approved.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-05-12 16:10:45.000000 netbox_config_diff-2.4.0/docs/media/screenshots/cr-collecting-diff-button.png
+-rw-r--r--   0 runner    (1001) docker     (127)    48412 2024-05-12 16:10:45.000000 netbox_config_diff-2.4.0/docs/media/screenshots/cr-completed.png
+-rw-r--r--   0 runner    (1001) docker     (127)    42240 2024-05-12 16:10:45.000000 netbox_config_diff-2.4.0/docs/media/screenshots/cr-created.png
+-rw-r--r--   0 runner    (1001) docker     (127)    65258 2024-05-12 16:10:45.000000 netbox_config_diff-2.4.0/docs/media/screenshots/cr-diffs-tab.png
+-rw-r--r--   0 runner    (1001) docker     (127)    20845 2024-05-12 16:10:45.000000 netbox_config_diff-2.4.0/docs/media/screenshots/cr-job-log.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-12 16:10:45.000000 netbox_config_diff-2.4.0/docs/media/screenshots/cr-schedule-button.png
+-rw-r--r--   0 runner    (1001) docker     (127)    14945 2024-05-12 16:10:45.000000 netbox_config_diff-2.4.0/docs/media/screenshots/cr-scheduled.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-05-12 16:10:45.000000 netbox_config_diff-2.4.0/docs/media/screenshots/cr-unapprove-button.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-05-12 16:10:45.000000 netbox_config_diff-2.4.0/docs/media/screenshots/cr-unschedule-button.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9572 2024-05-12 16:10:45.000000 netbox_config_diff-2.4.0/docs/media/screenshots/navbar.png
+-rw-r--r--   0 runner    (1001) docker     (127)    28028 2024-05-12 16:10:45.000000 netbox_config_diff-2.4.0/docs/media/screenshots/platformsetting.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-05-12 16:10:45.000000 netbox_config_diff-2.4.0/docs/media/screenshots/render-temp-substitute.png
+-rw-r--r--   0 runner    (1001) docker     (127)    14783 2024-05-12 16:10:45.000000 netbox_config_diff-2.4.0/docs/media/screenshots/script-list.png
+-rw-r--r--   0 runner    (1001) docker     (127)    43979 2024-05-12 16:10:45.000000 netbox_config_diff-2.4.0/docs/media/screenshots/script.png
+-rw-r--r--   0 runner    (1001) docker     (127)    15868 2024-05-12 16:10:45.000000 netbox_config_diff-2.4.0/docs/media/screenshots/substitute.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:10:59.290658 netbox_config_diff-2.4.0/netbox_config_diff/
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-12 16:10:45.000000 netbox_config_diff-2.4.0/netbox_config_diff/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:10:59.290658 netbox_config_diff-2.4.0/netbox_config_diff/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 16:10:45.000000 netbox_config_diff-2.4.0/netbox_config_diff/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5729 2024-05-12 16:10:45.000000 netbox_config_diff-2.4.0/netbox_config_diff/api/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-12 16:10:45.000000 netbox_config_diff-2.4.0/netbox_config_diff/api/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7891 2024-05-12 16:10:45.000000 netbox_config_diff-2.4.0/netbox_config_diff/api/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-05-12 16:10:45.000000 netbox_config_diff-2.4.0/netbox_config_diff/choices.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:10:59.294658 netbox_config_diff-2.4.0/netbox_config_diff/compliance/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 16:10:45.000000 netbox_config_diff-2.4.0/netbox_config_diff/compliance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8900 2024-05-12 16:10:45.000000 netbox_config_diff-2.4.0/netbox_config_diff/compliance/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-05-12 16:10:45.000000 netbox_config_diff-2.4.0/netbox_config_diff/compliance/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-05-12 16:10:45.000000 netbox_config_diff-2.4.0/netbox_config_diff/compliance/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:10:59.294658 netbox_config_diff-2.4.0/netbox_config_diff/configurator/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 16:10:45.000000 netbox_config_diff-2.4.0/netbox_config_diff/configurator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9957 2024-05-12 16:10:45.000000 netbox_config_diff-2.4.0/netbox_config_diff/configurator/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-12 16:10:45.000000 netbox_config_diff-2.4.0/netbox_config_diff/configurator/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3924 2024-05-12 16:10:45.000000 netbox_config_diff-2.4.0/netbox_config_diff/configurator/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7258 2024-05-12 16:10:45.000000 netbox_config_diff-2.4.0/netbox_config_diff/configurator/platforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-05-12 16:10:45.000000 netbox_config_diff-2.4.0/netbox_config_diff/configurator/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-12 16:10:45.000000 netbox_config_diff-2.4.0/netbox_config_diff/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4054 2024-05-12 16:10:45.000000 netbox_config_diff-2.4.0/netbox_config_diff/filtersets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6641 2024-05-12 16:10:45.000000 netbox_config_diff-2.4.0/netbox_config_diff/forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-05-12 16:10:45.000000 netbox_config_diff-2.4.0/netbox_config_diff/graphql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-05-12 16:10:45.000000 netbox_config_diff-2.4.0/netbox_config_diff/jobs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:10:59.294658 netbox_config_diff-2.4.0/netbox_config_diff/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-05-12 16:10:45.000000 netbox_config_diff-2.4.0/netbox_config_diff/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-05-12 16:10:45.000000 netbox_config_diff-2.4.0/netbox_config_diff/migrations/0002_add_script.py
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-12 16:10:45.000000 netbox_config_diff-2.4.0/netbox_config_diff/migrations/0003_configcompliance_actual_config_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-12 16:10:45.000000 netbox_config_diff-2.4.0/netbox_config_diff/migrations/0004_update_script.py
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-12 16:10:45.000000 netbox_config_diff-2.4.0/netbox_config_diff/migrations/0005_configcompliance_extra_missing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-05-12 16:10:45.000000 netbox_config_diff-2.4.0/netbox_config_diff/migrations/0006_substitute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2909 2024-05-12 16:10:45.000000 netbox_config_diff-2.4.0/netbox_config_diff/migrations/0007_configurationrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-12 16:10:45.000000 netbox_config_diff-2.4.0/netbox_config_diff/migrations/0008_alter_configcompliance_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-12 16:10:45.000000 netbox_config_diff-2.4.0/netbox_config_diff/migrations/0009_configcompliance_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 16:10:45.000000 netbox_config_diff-2.4.0/netbox_config_diff/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:10:59.298658 netbox_config_diff-2.4.0/netbox_config_diff/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-12 16:10:45.000000 netbox_config_diff-2.4.0/netbox_config_diff/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-12 16:10:45.000000 netbox_config_diff-2.4.0/netbox_config_diff/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4830 2024-05-12 16:10:45.000000 netbox_config_diff-2.4.0/netbox_config_diff/models/data_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7072 2024-05-12 16:10:45.000000 netbox_config_diff-2.4.0/netbox_config_diff/models/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-05-12 16:10:45.000000 netbox_config_diff-2.4.0/netbox_config_diff/navigation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:10:59.298658 netbox_config_diff-2.4.0/netbox_config_diff/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-12 16:10:45.000000 netbox_config_diff-2.4.0/netbox_config_diff/scripts/config_diff.py
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-05-12 16:10:45.000000 netbox_config_diff-2.4.0/netbox_config_diff/search.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:10:59.282658 netbox_config_diff-2.4.0/netbox_config_diff/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:10:59.298658 netbox_config_diff-2.4.0/netbox_config_diff/static/netbox_config_diff/
+-rw-r--r--   0 runner    (1001) docker     (127)  1000358 2024-05-12 16:10:45.000000 netbox_config_diff-2.4.0/netbox_config_diff/static/netbox_config_diff/diff2html-ui.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6661 2024-05-12 16:10:45.000000 netbox_config_diff-2.4.0/netbox_config_diff/static/netbox_config_diff/diff2html.dark.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)     6543 2024-05-12 16:10:45.000000 netbox_config_diff-2.4.0/netbox_config_diff/static/netbox_config_diff/diff2html.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2968 2024-05-12 16:10:45.000000 netbox_config_diff-2.4.0/netbox_config_diff/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:10:59.282658 netbox_config_diff-2.4.0/netbox_config_diff/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:10:59.298658 netbox_config_diff-2.4.0/netbox_config_diff/templates/netbox_config_diff/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:10:59.298658 netbox_config_diff-2.4.0/netbox_config_diff/templates/netbox_config_diff/configcompliance/
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-12 16:10:45.000000 netbox_config_diff-2.4.0/netbox_config_diff/templates/netbox_config_diff/configcompliance/config.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2673 2024-05-12 16:10:45.000000 netbox_config_diff-2.4.0/netbox_config_diff/templates/netbox_config_diff/configcompliance/data.html
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-05-12 16:10:45.000000 netbox_config_diff-2.4.0/netbox_config_diff/templates/netbox_config_diff/configcompliance/missing_extra.html
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-12 16:10:45.000000 netbox_config_diff-2.4.0/netbox_config_diff/templates/netbox_config_diff/configcompliance/patch.html
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-12 16:10:45.000000 netbox_config_diff-2.4.0/netbox_config_diff/templates/netbox_config_diff/configcompliance.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:10:59.298658 netbox_config_diff-2.4.0/netbox_config_diff/templates/netbox_config_diff/configurationrequest/
+-rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-05-12 16:10:45.000000 netbox_config_diff-2.4.0/netbox_config_diff/templates/netbox_config_diff/configurationrequest/base.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3561 2024-05-12 16:10:45.000000 netbox_config_diff-2.4.0/netbox_config_diff/templates/netbox_config_diff/configurationrequest/diffs.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-05-12 16:10:45.000000 netbox_config_diff-2.4.0/netbox_config_diff/templates/netbox_config_diff/configurationrequest.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:10:59.302658 netbox_config_diff-2.4.0/netbox_config_diff/templates/netbox_config_diff/inc/
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-12 16:10:45.000000 netbox_config_diff-2.4.0/netbox_config_diff/templates/netbox_config_diff/inc/commands_card.html
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-05-12 16:10:45.000000 netbox_config_diff-2.4.0/netbox_config_diff/templates/netbox_config_diff/inc/diff.html
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-12 16:10:45.000000 netbox_config_diff-2.4.0/netbox_config_diff/templates/netbox_config_diff/inc/job_log.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-05-12 16:10:45.000000 netbox_config_diff-2.4.0/netbox_config_diff/templates/netbox_config_diff/platformsetting.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-05-12 16:10:45.000000 netbox_config_diff-2.4.0/netbox_config_diff/templates/netbox_config_diff/substitute.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-05-12 16:10:45.000000 netbox_config_diff-2.4.0/netbox_config_diff/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:10:59.302658 netbox_config_diff-2.4.0/netbox_config_diff/views/
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-12 16:10:45.000000 netbox_config_diff-2.4.0/netbox_config_diff/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-05-12 16:10:45.000000 netbox_config_diff-2.4.0/netbox_config_diff/views/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6411 2024-05-12 16:10:45.000000 netbox_config_diff-2.4.0/netbox_config_diff/views/compliance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12412 2024-05-12 16:10:45.000000 netbox_config_diff-2.4.0/netbox_config_diff/views/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:10:59.302658 netbox_config_diff-2.4.0/netbox_config_diff.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    19264 2024-05-12 16:10:59.000000 netbox_config_diff-2.4.0/netbox_config_diff.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4429 2024-05-12 16:10:59.000000 netbox_config_diff-2.4.0/netbox_config_diff.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 16:10:59.000000 netbox_config_diff-2.4.0/netbox_config_diff.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-12 16:10:59.000000 netbox_config_diff-2.4.0/netbox_config_diff.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-12 16:10:59.000000 netbox_config_diff-2.4.0/netbox_config_diff.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-05-12 16:10:45.000000 netbox_config_diff-2.4.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:10:59.302658 netbox_config_diff-2.4.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-12 16:10:45.000000 netbox_config_diff-2.4.0/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-12 16:10:45.000000 netbox_config_diff-2.4.0/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-12 16:10:45.000000 netbox_config_diff-2.4.0/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 16:10:59.306658 netbox_config_diff-2.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:10:59.302658 netbox_config_diff-2.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-05-12 16:10:45.000000 netbox_config_diff-2.4.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2886 2024-05-12 16:10:45.000000 netbox_config_diff-2.4.0/tests/factories.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6077 2024-05-12 16:10:45.000000 netbox_config_diff-2.4.0/tests/test_compliance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-05-12 16:10:45.000000 netbox_config_diff-2.4.0/tests/test_compliance_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-05-12 16:10:45.000000 netbox_config_diff-2.4.0/tests/test_urls.py
```

### Comparing `netbox-config-diff-2.3.0/LICENSE` & `netbox_config_diff-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.3.0/PKG-INFO` & `netbox_config_diff-2.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-config-diff
-Version: 2.3.0
+Version: 2.4.0
 Summary: Push rendered device configurations from NetBox to devices and apply them.
 Author: Artem Kotik
 Author-email: miaow2@yandex.ru
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -214,14 +214,15 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: hier-config==2.2.3
 Requires-Dist: netutils==1.5.0
 Requires-Dist: scrapli[asyncssh]==2023.07.30
 Requires-Dist: scrapli-cfg==2023.07.30
 Requires-Dist: scrapli-community==2023.07.30
 Provides-Extra: dev
 Requires-Dist: ruff==0.1.2; extra == "dev"
 Provides-Extra: test
```

### Comparing `netbox-config-diff-2.3.0/README.md` & `netbox_config_diff-2.4.0/README.md`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.3.0/development/configuration.py` & `netbox_config_diff-2.4.0/development/configuration.py`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.3.0/docs/media/screenshots/compliance-diff.png` & `netbox_config_diff-2.4.0/docs/media/screenshots/compliance-diff.png`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.3.0/docs/media/screenshots/compliance-error.png` & `netbox_config_diff-2.4.0/docs/media/screenshots/compliance-error.png`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.3.0/docs/media/screenshots/compliance-list.png` & `netbox_config_diff-2.4.0/docs/media/screenshots/compliance-list.png`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.3.0/docs/media/screenshots/compliance-missing-extra.png` & `netbox_config_diff-2.4.0/docs/media/screenshots/compliance-missing-extra.png`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.3.0/docs/media/screenshots/compliance-ok.png` & `netbox_config_diff-2.4.0/docs/media/screenshots/compliance-ok.png`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.3.0/docs/media/screenshots/config-temp-substitute.png` & `netbox_config_diff-2.4.0/docs/media/screenshots/config-temp-substitute.png`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.3.0/docs/media/screenshots/cr-approve-button.png` & `netbox_config_diff-2.4.0/docs/media/screenshots/cr-approve-button.png`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.3.0/docs/media/screenshots/cr-approved.png` & `netbox_config_diff-2.4.0/docs/media/screenshots/cr-approved.png`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.3.0/docs/media/screenshots/cr-collecting-diff-button.png` & `netbox_config_diff-2.4.0/docs/media/screenshots/cr-collecting-diff-button.png`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.3.0/docs/media/screenshots/cr-completed.png` & `netbox_config_diff-2.4.0/docs/media/screenshots/cr-completed.png`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.3.0/docs/media/screenshots/cr-created.png` & `netbox_config_diff-2.4.0/docs/media/screenshots/cr-created.png`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.3.0/docs/media/screenshots/cr-diffs-tab.png` & `netbox_config_diff-2.4.0/docs/media/screenshots/cr-diffs-tab.png`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.3.0/docs/media/screenshots/cr-job-log.png` & `netbox_config_diff-2.4.0/docs/media/screenshots/cr-job-log.png`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.3.0/docs/media/screenshots/cr-schedule-button.png` & `netbox_config_diff-2.4.0/docs/media/screenshots/cr-schedule-button.png`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.3.0/docs/media/screenshots/cr-scheduled.png` & `netbox_config_diff-2.4.0/docs/media/screenshots/cr-scheduled.png`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.3.0/docs/media/screenshots/cr-unapprove-button.png` & `netbox_config_diff-2.4.0/docs/media/screenshots/cr-unapprove-button.png`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.3.0/docs/media/screenshots/cr-unschedule-button.png` & `netbox_config_diff-2.4.0/docs/media/screenshots/cr-unschedule-button.png`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.3.0/docs/media/screenshots/navbar.png` & `netbox_config_diff-2.4.0/docs/media/screenshots/navbar.png`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.3.0/docs/media/screenshots/platformsetting.png` & `netbox_config_diff-2.4.0/docs/media/screenshots/platformsetting.png`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.3.0/docs/media/screenshots/render-temp-substitute.png` & `netbox_config_diff-2.4.0/docs/media/screenshots/render-temp-substitute.png`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.3.0/docs/media/screenshots/script-list.png` & `netbox_config_diff-2.4.0/docs/media/screenshots/script-list.png`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.3.0/docs/media/screenshots/script.png` & `netbox_config_diff-2.4.0/docs/media/screenshots/script.png`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.3.0/docs/media/screenshots/substitute.png` & `netbox_config_diff-2.4.0/docs/media/screenshots/substitute.png`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.3.0/netbox_config_diff/__init__.py` & `netbox_config_diff-2.4.0/netbox_config_diff/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from extras.plugins import PluginConfig
 
 __author__ = "Artem Kotik"
 __email__ = "miaow2@yandex.ru"
-__version__ = "2.3.0"
+__version__ = "2.4.0"
 
 
 class ConfigDiffConfig(PluginConfig):
     name = "netbox_config_diff"
     verbose_name = "NetBox Config Diff Plugin"
     description = "Find diff between the intended device configuration and actual."
     author = __author__
```

### Comparing `netbox-config-diff-2.3.0/netbox_config_diff/api/serializers.py` & `netbox_config_diff-2.4.0/netbox_config_diff/api/serializers.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,14 +25,15 @@
             "display",
             "device",
             "status",
             "error",
             "diff",
             "rendered_config",
             "actual_config",
+            "patch",
             "missing",
             "extra",
             "created",
             "last_updated",
         )
```

### Comparing `netbox-config-diff-2.3.0/netbox_config_diff/api/views.py` & `netbox_config_diff-2.4.0/netbox_config_diff/api/views.py`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.3.0/netbox_config_diff/choices.py` & `netbox_config_diff-2.4.0/netbox_config_diff/choices.py`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.3.0/netbox_config_diff/compliance/base.py` & `netbox_config_diff-2.4.0/netbox_config_diff/compliance/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from netutils.config.compliance import diff_network_config
 from utilities.exceptions import AbortScript
 from utilities.utils import render_jinja2
 
 from netbox_config_diff.models import ConplianceDeviceDataClass
 
 from .secrets import SecretsMixin
-from .utils import PLATFORM_MAPPING, CustomChoiceVar, exclude_lines, get_unified_diff
+from .utils import PLATFORM_MAPPING, CustomChoiceVar, exclude_lines, get_remediation_commands, get_unified_diff
 
 
 class ConfigDiffBase(SecretsMixin):
     site = ObjectVar(
         model=Site,
         required=False,
         description="Run compliance for devices (with primary IP, platform) in this site",
@@ -200,7 +200,10 @@
             if device.platform in PLATFORM_MAPPING:
                 device.missing = diff_network_config(
                     device.rendered_config, cleaned_config, PLATFORM_MAPPING[device.platform]
                 )
                 device.extra = diff_network_config(
                     cleaned_config, device.rendered_config, PLATFORM_MAPPING[device.platform]
                 )
+            device.patch = get_remediation_commands(
+                device.name, device.platform, cleaned_config, device.rendered_config
+            )
```

### Comparing `netbox-config-diff-2.3.0/netbox_config_diff/compliance/secrets.py` & `netbox_config_diff-2.4.0/netbox_config_diff/compliance/secrets.py`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.3.0/netbox_config_diff/compliance/utils.py` & `netbox_config_diff-2.4.0/netbox_config_diff/compliance/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import re
 from difflib import unified_diff
 
 from django.forms import ChoiceField
 from extras.scripts import ScriptVariable
+from hier_config import Host
 
 PLATFORM_MAPPING = {
     "arista_eos": "arista_eos",
     "cisco_aireos": "cisco_aireos",
     "aruba_aoscx": "aruba_aoscx",
     "cisco_asa": "cisco_asa",
     "cisco_iosxe": "cisco_ios",
@@ -15,14 +16,23 @@
     "juniper_junos": "juniper_junos",
     "mikrotik_routeros": "mikrotik_routeros",
     "nokia_sros": "nokia_sros",
     "paloalto_panos": "paloalto_panos",
     "ruckus_fastiron": "ruckus_fastiron",
 }
 
+REMEDIATION_MAPPING = {
+    "arista_eos": "eos",
+    "cisco_iosxe": "ios",
+    "cisco_iosxr": "iosxr",
+    "cisco_nxos": "nxos",
+    "juniper_junos": "junos",
+    "vyos_vyos": "vyos",
+}
+
 
 class CustomChoiceVar(ScriptVariable):
     form_field = ChoiceField
 
     def __init__(self, choices, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.field_attrs["choices"] = choices
@@ -39,7 +49,14 @@
     return "\n".join(diff).strip()
 
 
 def exclude_lines(text: str, regexs: list) -> str:
     for item in regexs:
         text = re.sub(item, "", text, flags=re.I | re.M)
     return text.strip()
+
+
+def get_remediation_commands(name: str, platform: str, actual_config: str, rendered_config: str) -> str:
+    host = Host(hostname=name, os=REMEDIATION_MAPPING.get(platform, "ios"))
+    host.load_running_config(config_text=actual_config)
+    host.load_generated_config(config_text=rendered_config)
+    return host.remediation_config_filtered_text(include_tags={}, exclude_tags={})
```

### Comparing `netbox-config-diff-2.3.0/netbox_config_diff/configurator/base.py` & `netbox_config_diff-2.4.0/netbox_config_diff/configurator/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from netutils.config.compliance import diff_network_config
 from scrapli import AsyncScrapli
 from scrapli_cfg.platform.base.async_platform import AsyncScrapliCfgPlatform
 from scrapli_cfg.response import ScrapliCfgResponse
 from utilities.utils import NetBoxFakeRequest
 
 from netbox_config_diff.compliance.secrets import SecretsMixin
-from netbox_config_diff.compliance.utils import PLATFORM_MAPPING, get_unified_diff
+from netbox_config_diff.compliance.utils import PLATFORM_MAPPING, get_remediation_commands, get_unified_diff
 from netbox_config_diff.configurator.exceptions import DeviceConfigurationError, DeviceValidationError
 from netbox_config_diff.configurator.utils import CustomLogger
 from netbox_config_diff.constants import ACCEPTABLE_DRIVERS
 from netbox_config_diff.models import ConfiguratorDeviceDataClass
 
 from .factory import AsyncScrapliCfg
 
@@ -133,14 +133,17 @@
             self.logger.add_diff(device.name, diff=device.diff)
             device.missing = diff_network_config(
                 device.rendered_config, device.actual_config, PLATFORM_MAPPING[device.platform]
             )
             device.extra = diff_network_config(
                 device.actual_config, device.rendered_config, PLATFORM_MAPPING[device.platform]
             )
+            device.patch = get_remediation_commands(
+                device.name, device.platform, device.actual_config, device.rendered_config
+            )
             self.logger.log_info(f"Got diff from {device.name}")
         except Exception:
             error = traceback.format_exc()
             device.error = error
             self.logger.log_failure(error)
             self.logger.add_diff(device.name, error=error)
```

### Comparing `netbox-config-diff-2.3.0/netbox_config_diff/configurator/factory.py` & `netbox_config_diff-2.4.0/netbox_config_diff/configurator/factory.py`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.3.0/netbox_config_diff/configurator/platforms.py` & `netbox_config_diff-2.4.0/netbox_config_diff/configurator/platforms.py`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.3.0/netbox_config_diff/configurator/utils.py` & `netbox_config_diff-2.4.0/netbox_config_diff/configurator/utils.py`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.3.0/netbox_config_diff/filtersets.py` & `netbox_config_diff-2.4.0/netbox_config_diff/filtersets.py`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.3.0/netbox_config_diff/forms.py` & `netbox_config_diff-2.4.0/netbox_config_diff/forms.py`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.3.0/netbox_config_diff/graphql.py` & `netbox_config_diff-2.4.0/netbox_config_diff/graphql.py`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.3.0/netbox_config_diff/jobs.py` & `netbox_config_diff-2.4.0/netbox_config_diff/jobs.py`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.3.0/netbox_config_diff/migrations/0001_initial.py` & `netbox_config_diff-2.4.0/netbox_config_diff/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.3.0/netbox_config_diff/migrations/0002_add_script.py` & `netbox_config_diff-2.4.0/netbox_config_diff/migrations/0002_add_script.py`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.3.0/netbox_config_diff/migrations/0003_configcompliance_actual_config_and_more.py` & `netbox_config_diff-2.4.0/netbox_config_diff/migrations/0003_configcompliance_actual_config_and_more.py`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.3.0/netbox_config_diff/migrations/0004_update_script.py` & `netbox_config_diff-2.4.0/netbox_config_diff/migrations/0004_update_script.py`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.3.0/netbox_config_diff/migrations/0006_substitute.py` & `netbox_config_diff-2.4.0/netbox_config_diff/migrations/0006_substitute.py`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.3.0/netbox_config_diff/migrations/0007_configurationrequest.py` & `netbox_config_diff-2.4.0/netbox_config_diff/migrations/0007_configurationrequest.py`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.3.0/netbox_config_diff/migrations/0008_alter_configcompliance_device.py` & `netbox_config_diff-2.4.0/netbox_config_diff/migrations/0008_alter_configcompliance_device.py`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.3.0/netbox_config_diff/models/data_models.py` & `netbox_config_diff-2.4.0/netbox_config_diff/models/data_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     password: str
     exclude_regex: str | None = None
     rendered_config: str | None = None
     actual_config: str | None = None
     diff: str = ""
     missing: str | None = None
     extra: str | None = None
+    patch: str | None = None
     error: str = ""
     config_error: str | None = None
     auth_strict_key: bool = False
     auth_secondary: str | None = None
     transport: str = "asyncssh"
 
     def __str__(self) -> str:
@@ -95,14 +96,15 @@
             "status": status,
             "diff": self.diff or "",
             "error": self.error or "",
             "rendered_config": self.rendered_config or "",
             "actual_config": self.actual_config or "",
             "missing": self.missing or "",
             "extra": self.extra or "",
+            "patch": self.patch or "",
         }
 
     def send_to_db(self) -> None:
         try:
             obj = ConfigCompliance.objects.get(device_id=self.pk)
             if obj.status != self.get_status():
                 obj.update(commit=True, **self.to_db())
```

### Comparing `netbox-config-diff-2.3.0/netbox_config_diff/models/models.py` & `netbox_config_diff-2.4.0/netbox_config_diff/models/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,14 +45,17 @@
     )
     missing = models.TextField(
         blank=True,
     )
     extra = models.TextField(
         blank=True,
     )
+    patch = models.TextField(
+        blank=True,
+    )
 
     objects = RestrictedQuerySet.as_manager()
 
     class Meta:
         ordering = ("device",)
 
     def __str__(self) -> str:
```

### Comparing `netbox-config-diff-2.3.0/netbox_config_diff/navigation.py` & `netbox_config_diff-2.4.0/netbox_config_diff/navigation.py`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.3.0/netbox_config_diff/search.py` & `netbox_config_diff-2.4.0/netbox_config_diff/search.py`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.3.0/netbox_config_diff/static/netbox_config_diff/diff2html-ui.min.js` & `netbox_config_diff-2.4.0/netbox_config_diff/static/netbox_config_diff/diff2html-ui.min.js`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.3.0/netbox_config_diff/static/netbox_config_diff/diff2html.dark.min.css` & `netbox_config_diff-2.4.0/netbox_config_diff/static/netbox_config_diff/diff2html.dark.min.css`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.3.0/netbox_config_diff/static/netbox_config_diff/diff2html.min.css` & `netbox_config_diff-2.4.0/netbox_config_diff/static/netbox_config_diff/diff2html.min.css`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.3.0/netbox_config_diff/tables.py` & `netbox_config_diff-2.4.0/netbox_config_diff/tables.py`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.3.0/netbox_config_diff/templates/netbox_config_diff/configcompliance/config.html` & `netbox_config_diff-2.4.0/netbox_config_diff/templates/netbox_config_diff/configcompliance/config.html`

 * *Files 11% similar despite different names*

```diff
@@ -4,22 +4,23 @@
 
 {% block content %}
   <div class="row">
     <div class="col">
       <div class="card">
         <div class="card-header">
           <div class="float-end">
+            {% copy_content config_field %}
             <a href="?export=True" class="btn btn-sm btn-primary" role="button">
               <i class="mdi mdi-download" aria-hidden="true"></i> Download
             </a>
           </div>
           <h5>{{ header }}</h5>
         </div>
         {% if config %}
-          <pre class="card-body">{{ config }}</pre>
+          <pre class="card-body" id="{{ config_field }}">{{ config }}</pre>
         {% else %}
           <div class="card-body text-muted">No configuration</div>
         {% endif %}
       </div>
     </div>
   </div>
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,9 +1,10 @@
 {% extends "netbox_config_diff/configcompliance.html" %} {% block title %}{
 { object }} - {{ header }}{% endblock %} {% block content %}
+{% copy_content config_field %}
 _D_o_w_n_l_o_a_d
 **** {{{{ hheeaaddeerr }}}} ****
 {% if config %}
 {{ config }}
 {% else %}
 No configuration
 {% endif %}
```

### Comparing `netbox-config-diff-2.3.0/netbox_config_diff/templates/netbox_config_diff/configcompliance/data.html` & `netbox_config_diff-2.4.0/netbox_config_diff/templates/netbox_config_diff/configcompliance/data.html`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.3.0/netbox_config_diff/templates/netbox_config_diff/configurationrequest/base.html` & `netbox_config_diff-2.4.0/netbox_config_diff/templates/netbox_config_diff/configurationrequest/base.html`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.3.0/netbox_config_diff/templates/netbox_config_diff/configurationrequest/diffs.html` & `netbox_config_diff-2.4.0/netbox_config_diff/templates/netbox_config_diff/configurationrequest/diffs.html`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.3.0/netbox_config_diff/templates/netbox_config_diff/configurationrequest.html` & `netbox_config_diff-2.4.0/netbox_config_diff/templates/netbox_config_diff/configurationrequest.html`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.3.0/netbox_config_diff/templates/netbox_config_diff/inc/diff.html` & `netbox_config_diff-2.4.0/netbox_config_diff/templates/netbox_config_diff/inc/diff.html`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.3.0/netbox_config_diff/templates/netbox_config_diff/inc/job_log.html` & `netbox_config_diff-2.4.0/netbox_config_diff/templates/netbox_config_diff/inc/job_log.html`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.3.0/netbox_config_diff/templates/netbox_config_diff/platformsetting.html` & `netbox_config_diff-2.4.0/netbox_config_diff/templates/netbox_config_diff/platformsetting.html`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.3.0/netbox_config_diff/templates/netbox_config_diff/substitute.html` & `netbox_config_diff-2.4.0/netbox_config_diff/templates/netbox_config_diff/substitute.html`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.3.0/netbox_config_diff/urls.py` & `netbox_config_diff-2.4.0/netbox_config_diff/urls.py`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.3.0/netbox_config_diff/views/__init__.py` & `netbox_config_diff-2.4.0/netbox_config_diff/views/__init__.py`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.3.0/netbox_config_diff/views/compliance.py` & `netbox_config_diff-2.4.0/netbox_config_diff/views/compliance.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from dcim.models import Device
-from django.http import HttpResponse
 from django.shortcuts import redirect, render
 from django.utils.translation import gettext as _
 from netbox.views import generic
 from utilities.views import ViewTab, register_model_view
 
 from netbox_config_diff.filtersets import ConfigComplianceFilterSet, PlatformSettingFilterSet
 from netbox_config_diff.forms import (
@@ -11,46 +10,15 @@
     PlatformSettingBulkEditForm,
     PlatformSettingFilterForm,
     PlatformSettingForm,
 )
 from netbox_config_diff.models import ConfigCompliance, PlatformSetting
 from netbox_config_diff.tables import ConfigComplianceTable, PlatformSettingTable
 
-from .base import BaseObjectDeleteView, BaseObjectEditView
-
-
-class BaseConfigComplianceConfigView(generic.ObjectView):
-    config_field = None
-    template_header = None
-
-    def get(self, request, **kwargs):
-        instance = self.get_object(**kwargs)
-        context = self.get_extra_context(request, instance)
-
-        if request.GET.get("export"):
-            response = HttpResponse(context["config"], content_type="text")
-            filename = f"{instance.device.name}_{self.config_field}.txt"
-            response["Content-Disposition"] = f'attachment; filename="{filename}"'
-            return response
-
-        return render(
-            request,
-            self.get_template_name(),
-            {
-                "object": instance,
-                "tab": self.tab,
-                **context,
-            },
-        )
-
-    def get_extra_context(self, request, instance):
-        return {
-            "header": self.template_header,
-            "config": getattr(instance, self.config_field),
-        }
+from .base import BaseConfigComplianceConfigView, BaseExportView, BaseObjectDeleteView, BaseObjectEditView
 
 
 @register_model_view(ConfigCompliance)
 class ConfigComplianceView(generic.ObjectView):
     queryset = ConfigCompliance.objects.all()
     base_template = "netbox_config_diff/configcompliance.html"
     template_name = "netbox_config_diff/configcompliance/data.html"
@@ -83,28 +51,22 @@
     tab = ViewTab(
         label=_(template_header),
         weight=510,
     )
 
 
 @register_model_view(ConfigCompliance, "missing-extra")
-class ConfigComplianceMissingExtraConfigView(generic.ObjectView):
+class ConfigComplianceMissingExtraConfigView(BaseExportView):
     queryset = ConfigCompliance.objects.all()
     template_name = "netbox_config_diff/configcompliance/missing_extra.html"
     tab = ViewTab(
         label=_("Missing/Extra"),
         weight=520,
     )
 
-    def export_parts(self, name, lines, suffix):
-        response = HttpResponse(lines, content_type="text")
-        filename = f"{name}_{suffix}.txt"
-        response["Content-Disposition"] = f'attachment; filename="{filename}"'
-        return response
-
     def get(self, request, **kwargs):
         instance = self.get_object(**kwargs)
         context = self.get_extra_context(request, instance)
 
         if request.GET.get("export_missing"):
             return self.export_parts(instance.device.name, instance.missing, "missing")
 
@@ -113,14 +75,41 @@
 
         return render(
             request,
             self.get_template_name(),
             {
                 "object": instance,
                 "tab": self.tab,
+                **context,
+            },
+        )
+
+
+@register_model_view(ConfigCompliance, "patch")
+class ConfigCompliancePatchView(BaseExportView):
+    queryset = ConfigCompliance.objects.all()
+    template_name = "netbox_config_diff/configcompliance/patch.html"
+    tab = ViewTab(
+        label=_("Patch"),
+        weight=515,
+    )
+
+    def get(self, request, **kwargs):
+        instance = self.get_object(**kwargs)
+        context = self.get_extra_context(request, instance)
+
+        if request.GET.get("export_patch"):
+            return self.export_parts(instance.device.name, instance.patch, "patch")
+
+        return render(
+            request,
+            self.get_template_name(),
+            {
+                "object": instance,
+                "tab": self.tab,
                 **context,
             },
         )
 
 
 @register_model_view(Device, "config_compliance", "config-compliance")
 class ConfigComplianceDeviceView(generic.ObjectView):
```

### Comparing `netbox-config-diff-2.3.0/netbox_config_diff/views/configuration.py` & `netbox_config_diff-2.4.0/netbox_config_diff/views/configuration.py`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.3.0/netbox_config_diff.egg-info/PKG-INFO` & `netbox_config_diff-2.4.0/netbox_config_diff.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-config-diff
-Version: 2.3.0
+Version: 2.4.0
 Summary: Push rendered device configurations from NetBox to devices and apply them.
 Author: Artem Kotik
 Author-email: miaow2@yandex.ru
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -214,14 +214,15 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: hier-config==2.2.3
 Requires-Dist: netutils==1.5.0
 Requires-Dist: scrapli[asyncssh]==2023.07.30
 Requires-Dist: scrapli-cfg==2023.07.30
 Requires-Dist: scrapli-community==2023.07.30
 Provides-Extra: dev
 Requires-Dist: ruff==0.1.2; extra == "dev"
 Provides-Extra: test
```

### Comparing `netbox-config-diff-2.3.0/netbox_config_diff.egg-info/SOURCES.txt` & `netbox_config_diff-2.4.0/netbox_config_diff.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 pyproject.toml
 development/configuration.py
 docs/media/screenshots/compliance-diff.png
 docs/media/screenshots/compliance-error.png
 docs/media/screenshots/compliance-list.png
 docs/media/screenshots/compliance-missing-extra.png
 docs/media/screenshots/compliance-ok.png
+docs/media/screenshots/compliance-patch.png
 docs/media/screenshots/config-temp-substitute.png
 docs/media/screenshots/cr-approve-button.png
 docs/media/screenshots/cr-approved.png
 docs/media/screenshots/cr-collecting-diff-button.png
 docs/media/screenshots/cr-completed.png
 docs/media/screenshots/cr-created.png
 docs/media/screenshots/cr-diffs-tab.png
@@ -60,14 +61,15 @@
 netbox_config_diff/migrations/0002_add_script.py
 netbox_config_diff/migrations/0003_configcompliance_actual_config_and_more.py
 netbox_config_diff/migrations/0004_update_script.py
 netbox_config_diff/migrations/0005_configcompliance_extra_missing.py
 netbox_config_diff/migrations/0006_substitute.py
 netbox_config_diff/migrations/0007_configurationrequest.py
 netbox_config_diff/migrations/0008_alter_configcompliance_device.py
+netbox_config_diff/migrations/0009_configcompliance_patch.py
 netbox_config_diff/migrations/__init__.py
 netbox_config_diff/models/__init__.py
 netbox_config_diff/models/base.py
 netbox_config_diff/models/data_models.py
 netbox_config_diff/models/models.py
 netbox_config_diff/scripts/config_diff.py
 netbox_config_diff/static/netbox_config_diff/diff2html-ui.min.js
@@ -76,16 +78,18 @@
 netbox_config_diff/templates/netbox_config_diff/configcompliance.html
 netbox_config_diff/templates/netbox_config_diff/configurationrequest.html
 netbox_config_diff/templates/netbox_config_diff/platformsetting.html
 netbox_config_diff/templates/netbox_config_diff/substitute.html
 netbox_config_diff/templates/netbox_config_diff/configcompliance/config.html
 netbox_config_diff/templates/netbox_config_diff/configcompliance/data.html
 netbox_config_diff/templates/netbox_config_diff/configcompliance/missing_extra.html
+netbox_config_diff/templates/netbox_config_diff/configcompliance/patch.html
 netbox_config_diff/templates/netbox_config_diff/configurationrequest/base.html
 netbox_config_diff/templates/netbox_config_diff/configurationrequest/diffs.html
+netbox_config_diff/templates/netbox_config_diff/inc/commands_card.html
 netbox_config_diff/templates/netbox_config_diff/inc/diff.html
 netbox_config_diff/templates/netbox_config_diff/inc/job_log.html
 netbox_config_diff/views/__init__.py
 netbox_config_diff/views/base.py
 netbox_config_diff/views/compliance.py
 netbox_config_diff/views/configuration.py
 requirements/base.txt
```

### Comparing `netbox-config-diff-2.3.0/pyproject.toml` & `netbox_config_diff-2.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.3.0/tests/conftest.py` & `netbox_config_diff-2.4.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.3.0/tests/factories.py` & `netbox_config_diff-2.4.0/tests/factories.py`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.3.0/tests/test_compliance.py` & `netbox_config_diff-2.4.0/tests/test_compliance.py`

 * *Files 1% similar despite different names*

```diff
@@ -151,8 +151,9 @@
         "status": status,
         "diff": diff,
         "error": error,
         "rendered_config": "",
         "actual_config": "",
         "missing": "",
         "extra": "",
+        "patch": "",
     }
```

### Comparing `netbox-config-diff-2.3.0/tests/test_compliance_utils.py` & `netbox_config_diff-2.4.0/tests/test_compliance_utils.py`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-2.3.0/tests/test_urls.py` & `netbox_config_diff-2.4.0/tests/test_urls.py`

 * *Files identical despite different names*

