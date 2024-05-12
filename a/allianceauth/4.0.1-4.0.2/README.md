# Comparing `tmp/allianceauth-4.0.1.tar.gz` & `tmp/allianceauth-4.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "allianceauth-4.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "allianceauth-4.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `allianceauth-4.0.1.tar` & `allianceauth-4.0.2.tar`

### file list

```diff
@@ -1,839 +1,846 @@
--rw-r--r--   0        0        0    18026 2024-03-21 09:38:59.598781 allianceauth-4.0.1/LICENSE
--rw-r--r--   0        0        0     4980 2024-03-21 09:38:59.598781 allianceauth-4.0.1/README.md
--rw-r--r--   0        0        0      352 2024-03-21 09:38:59.598781 allianceauth-4.0.1/allianceauth/__init__.py
--rw-r--r--   0        0        0        0 2024-03-21 09:38:59.709781 allianceauth-4.0.1/allianceauth/analytics/__init__.py
--rw-r--r--   0        0        0      401 2024-03-21 09:38:59.598781 allianceauth-4.0.1/allianceauth/analytics/admin.py
--rw-r--r--   0        0        0      130 2024-03-21 09:38:59.598781 allianceauth-4.0.1/allianceauth/analytics/apps.py
--rw-r--r--   0        0        0      456 2024-03-21 09:38:59.598781 allianceauth-4.0.1/allianceauth/analytics/fixtures/disable_analytics.json
--rw-r--r--   0        0        0     1664 2024-03-21 09:38:59.598781 allianceauth-4.0.1/allianceauth/analytics/migrations/0001_initial.py
--rw-r--r--   0        0        0     1072 2024-03-21 09:38:59.598781 allianceauth-4.0.1/allianceauth/analytics/migrations/0002_add_AA_Team_Token.py
--rw-r--r--   0        0        0      907 2024-03-21 09:38:59.598781 allianceauth-4.0.1/allianceauth/analytics/migrations/0003_Generate_Identifier.py
--rw-r--r--   0        0        0     1650 2024-03-21 09:38:59.598781 allianceauth-4.0.1/allianceauth/analytics/migrations/0004_auto_20211015_0502.py
--rw-r--r--   0        0        0      495 2024-03-21 09:38:59.598781 allianceauth-4.0.1/allianceauth/analytics/migrations/0005_alter_analyticspath_ignore_path.py
--rw-r--r--   0        0        0     1413 2024-03-21 09:38:59.598781 allianceauth-4.0.1/allianceauth/analytics/migrations/0006_more_ignore_paths.py
--rw-r--r--   0        0        0      407 2024-03-21 09:38:59.598781 allianceauth-4.0.1/allianceauth/analytics/migrations/0007_analyticstokens_secret.py
--rw-r--r--   0        0        0     2451 2024-03-21 09:38:59.598781 allianceauth-4.0.1/allianceauth/analytics/migrations/0008_add_AA_GA-4_Team_Token .py
--rw-r--r--   0        0        0      672 2024-03-21 09:38:59.599781 allianceauth-4.0.1/allianceauth/analytics/migrations/0009_remove_analyticstokens_ignore_paths_and_more.py
--rw-r--r--   0        0        0        0 2024-03-21 09:38:59.712781 allianceauth-4.0.1/allianceauth/analytics/migrations/__init__.py
--rw-r--r--   0        0        0     1173 2024-03-21 09:38:59.599781 allianceauth-4.0.1/allianceauth/analytics/models.py
--rw-r--r--   0        0        0     5449 2024-03-21 09:38:59.599781 allianceauth-4.0.1/allianceauth/analytics/tasks.py
--rw-r--r--   0        0        0        0 2024-03-21 09:38:59.712781 allianceauth-4.0.1/allianceauth/analytics/tests/__init__.py
--rw-r--r--   0        0        0      951 2024-03-21 09:38:59.599781 allianceauth-4.0.1/allianceauth/analytics/tests/test_models.py
--rw-r--r--   0        0        0     2007 2024-03-21 09:38:59.599781 allianceauth-4.0.1/allianceauth/analytics/tests/test_tasks.py
--rw-r--r--   0        0        0     1535 2024-03-21 09:38:59.599781 allianceauth-4.0.1/allianceauth/analytics/tests/test_utils.py
--rw-r--r--   0        0        0      777 2024-03-21 09:38:59.599781 allianceauth-4.0.1/allianceauth/analytics/utils.py
--rw-r--r--   0        0        0     1178 2024-03-21 09:38:59.599781 allianceauth-4.0.1/allianceauth/apps.py
--rw-r--r--   0        0        0        0 2024-03-21 09:38:59.712781 allianceauth-4.0.1/allianceauth/authentication/__init__.py
--rw-r--r--   0        0        0    21182 2024-03-21 09:38:59.599781 allianceauth-4.0.1/allianceauth/authentication/admin.py
--rw-r--r--   0        0        0     1345 2024-03-21 09:38:59.599781 allianceauth-4.0.1/allianceauth/authentication/app_settings.py
--rw-r--r--   0        0        0      514 2024-03-21 09:38:59.599781 allianceauth-4.0.1/allianceauth/authentication/apps.py
--rw-r--r--   0        0        0     1243 2024-03-21 09:38:59.599781 allianceauth-4.0.1/allianceauth/authentication/auth_hooks.py
--rw-r--r--   0        0        0     5150 2024-03-21 09:38:59.599781 allianceauth-4.0.1/allianceauth/authentication/backends.py
--rw-r--r--   0        0        0      434 2024-03-21 09:38:59.599781 allianceauth-4.0.1/allianceauth/authentication/checks.py
--rw-r--r--   0        0        0      641 2024-03-21 09:38:59.599781 allianceauth-4.0.1/allianceauth/authentication/constants.py
--rw-r--r--   0        0        0        0 2024-03-21 09:38:59.712781 allianceauth-4.0.1/allianceauth/authentication/core/__init__.py
--rw-r--r--   0        0        0     1307 2024-03-21 09:38:59.600781 allianceauth-4.0.1/allianceauth/authentication/core/celery_workers.py
--rw-r--r--   0        0        0     3063 2024-03-21 09:38:59.600781 allianceauth-4.0.1/allianceauth/authentication/decorators.py
--rw-r--r--   0        0        0     2480 2024-03-21 09:38:59.600781 allianceauth-4.0.1/allianceauth/authentication/forms.py
--rw-r--r--   0        0        0      776 2024-03-21 09:38:59.600781 allianceauth-4.0.1/allianceauth/authentication/hmac_urls.py
--rw-r--r--   0        0        0        0 2024-03-21 09:38:59.715781 allianceauth-4.0.1/allianceauth/authentication/management/__init__.py
--rw-r--r--   0        0        0        0 2024-03-21 09:38:59.715781 allianceauth-4.0.1/allianceauth/authentication/management/commands/__init__.py
--rw-r--r--   0        0        0     1026 2024-03-21 09:38:59.600781 allianceauth-4.0.1/allianceauth/authentication/management/commands/checkmains.py
--rw-r--r--   0        0        0     2709 2024-03-21 09:38:59.600781 allianceauth-4.0.1/allianceauth/authentication/managers.py
--rw-r--r--   0        0        0     2422 2024-03-21 09:38:59.600781 allianceauth-4.0.1/allianceauth/authentication/middleware.py
--rw-r--r--   0        0        0     3147 2024-03-21 09:38:59.600781 allianceauth-4.0.1/allianceauth/authentication/migrations/0001_initial.py
--rw-r--r--   0        0        0      474 2024-03-21 09:38:59.600781 allianceauth-4.0.1/allianceauth/authentication/migrations/0002_auto_20160907_1914.py
--rw-r--r--   0        0        0      509 2024-03-21 09:38:59.600781 allianceauth-4.0.1/allianceauth/authentication/migrations/0003_authservicesinfo_state.py
--rw-r--r--   0        0        0     2543 2024-03-21 09:38:59.600781 allianceauth-4.0.1/allianceauth/authentication/migrations/0004_create_permissions.py
--rw-r--r--   0        0        0     1144 2024-03-21 09:38:59.600781 allianceauth-4.0.1/allianceauth/authentication/migrations/0005_delete_perms.py
--rw-r--r--   0        0        0     1324 2024-03-21 09:38:59.600781 allianceauth-4.0.1/allianceauth/authentication/migrations/0006_auto_20160910_0542.py
--rw-r--r--   0        0        0      347 2024-03-21 09:38:59.600781 allianceauth-4.0.1/allianceauth/authentication/migrations/0007_remove_authservicesinfo_is_blue.py
--rw-r--r--   0        0        0      319 2024-03-21 09:38:59.600781 allianceauth-4.0.1/allianceauth/authentication/migrations/0008_set_state.py
--rw-r--r--   0        0        0      532 2024-03-21 09:38:59.600781 allianceauth-4.0.1/allianceauth/authentication/migrations/0009_auto_20161021_0228.py
--rw-r--r--   0        0        0     1235 2024-03-21 09:38:59.600781 allianceauth-4.0.1/allianceauth/authentication/migrations/0010_only_one_authservicesinfo.py
--rw-r--r--   0        0        0      538 2024-03-21 09:38:59.600781 allianceauth-4.0.1/allianceauth/authentication/migrations/0011_authservicesinfo_user_onetoonefield.py
--rw-r--r--   0        0        0     1567 2024-03-21 09:38:59.600781 allianceauth-4.0.1/allianceauth/authentication/migrations/0012_remove_add_delete_authservicesinfo_permissions.py
--rw-r--r--   0        0        0     1914 2024-03-21 09:38:59.600781 allianceauth-4.0.1/allianceauth/authentication/migrations/0013_service_modules.py
--rw-r--r--   0        0        0      660 2024-03-21 09:38:59.600781 allianceauth-4.0.1/allianceauth/authentication/migrations/0014_fleetup_permission.py
--rw-r--r--   0        0        0    13077 2024-03-21 09:38:59.601781 allianceauth-4.0.1/allianceauth/authentication/migrations/0015_user_profiles.py
--rw-r--r--   0        0        0     1637 2024-03-21 09:38:59.601781 allianceauth-4.0.1/allianceauth/authentication/migrations/0016_ownershiprecord.py
--rw-r--r--   0        0        0      612 2024-03-21 09:38:59.601781 allianceauth-4.0.1/allianceauth/authentication/migrations/0017_remove_fleetup_permission.py
--rw-r--r--   0        0        0      410 2024-03-21 09:38:59.601781 allianceauth-4.0.1/allianceauth/authentication/migrations/0018_alter_state_name_length.py
--rw-r--r--   0        0        0      545 2024-03-21 09:38:59.601781 allianceauth-4.0.1/allianceauth/authentication/migrations/0018_state_member_factions.py
--rw-r--r--   0        0        0      295 2024-03-21 09:38:59.601781 allianceauth-4.0.1/allianceauth/authentication/migrations/0019_merge_20211026_0919.py
--rw-r--r--   0        0        0      841 2024-03-21 09:38:59.601781 allianceauth-4.0.1/allianceauth/authentication/migrations/0020_userprofile_language_userprofile_night_mode.py
--rw-r--r--   0        0        0     1004 2024-03-21 09:38:59.601781 allianceauth-4.0.1/allianceauth/authentication/migrations/0021_alter_userprofile_language.py
--rw-r--r--   0        0        0      529 2024-03-21 09:38:59.601781 allianceauth-4.0.1/allianceauth/authentication/migrations/0022_userprofile_theme.py
--rw-r--r--   0        0        0        0 2024-03-21 09:38:59.721780 allianceauth-4.0.1/allianceauth/authentication/migrations/__init__.py
--rw-r--r--   0        0        0     6015 2024-03-21 09:38:59.601781 allianceauth-4.0.1/allianceauth/authentication/models.py
--rw-r--r--   0        0        0     7806 2024-03-21 09:38:59.601781 allianceauth-4.0.1/allianceauth/authentication/signals.py
--rw-r--r--   0        0        0      506 2024-03-21 09:38:59.601781 allianceauth-4.0.1/allianceauth/authentication/static/allianceauth/authentication/css/admin.css
--rw-r--r--   0        0        0   161344 2024-03-21 09:38:59.602781 allianceauth-4.0.1/allianceauth/authentication/static/allianceauth/authentication/img/background.jpg
--rw-r--r--   0        0        0     2308 2024-03-21 09:38:59.602781 allianceauth-4.0.1/allianceauth/authentication/static/allianceauth/authentication/img/sso/EVE_SSO_Login_Buttons_Large_Black.png
--rw-r--r--   0        0        0     2248 2024-03-21 09:38:59.602781 allianceauth-4.0.1/allianceauth/authentication/static/allianceauth/authentication/img/sso/EVE_SSO_Login_Buttons_Large_White.png
--rw-r--r--   0        0        0        0 2024-03-21 09:38:59.721780 allianceauth-4.0.1/allianceauth/authentication/task_statistics/__init__.py
--rw-r--r--   0        0        0     1536 2024-03-21 09:38:59.602781 allianceauth-4.0.1/allianceauth/authentication/task_statistics/counters.py
--rw-r--r--   0        0        0     3257 2024-03-21 09:38:59.602781 allianceauth-4.0.1/allianceauth/authentication/task_statistics/event_series.py
--rw-r--r--   0        0        0     1174 2024-03-21 09:38:59.602781 allianceauth-4.0.1/allianceauth/authentication/task_statistics/helpers.py
--rw-r--r--   0        0        0     1217 2024-03-21 09:38:59.603781 allianceauth-4.0.1/allianceauth/authentication/task_statistics/signals.py
--rw-r--r--   0        0        0        0 2024-03-21 09:38:59.721780 allianceauth-4.0.1/allianceauth/authentication/task_statistics/tests/__init__.py
--rw-r--r--   0        0        0     1704 2024-03-21 09:38:59.603781 allianceauth-4.0.1/allianceauth/authentication/task_statistics/tests/test_counters.py
--rw-r--r--   0        0        0     5137 2024-03-21 09:38:59.603781 allianceauth-4.0.1/allianceauth/authentication/task_statistics/tests/test_event_series.py
--rw-r--r--   0        0        0     1009 2024-03-21 09:38:59.603781 allianceauth-4.0.1/allianceauth/authentication/task_statistics/tests/test_helpers.py
--rw-r--r--   0        0        0     2719 2024-03-21 09:38:59.603781 allianceauth-4.0.1/allianceauth/authentication/task_statistics/tests/test_signals.py
--rw-r--r--   0        0        0     1661 2024-03-21 09:38:59.603781 allianceauth-4.0.1/allianceauth/authentication/tasks.py
--rw-r--r--   0        0        0      423 2024-03-21 09:38:59.603781 allianceauth-4.0.1/allianceauth/authentication/templates/authentication/dashboard.html
--rw-r--r--   0        0        0      188 2024-03-21 09:38:59.603781 allianceauth-4.0.1/allianceauth/authentication/templates/authentication/dashboard_bs3.html
--rw-r--r--   0        0        0     2476 2024-03-21 09:38:59.603781 allianceauth-4.0.1/allianceauth/authentication/templates/authentication/dashboard_characters.html
--rw-r--r--   0        0        0      838 2024-03-21 09:38:59.603781 allianceauth-4.0.1/allianceauth/authentication/templates/authentication/dashboard_groups.html
--rw-r--r--   0        0        0     3043 2024-03-21 09:38:59.603781 allianceauth-4.0.1/allianceauth/authentication/templates/authentication/tokens.html
--rw-r--r--   0        0        0     2001 2024-03-21 09:38:59.603781 allianceauth-4.0.1/allianceauth/authentication/templates/public/base.html
--rw-r--r--   0        0        0      674 2024-03-21 09:38:59.603781 allianceauth-4.0.1/allianceauth/authentication/templates/public/lang_select.html
--rw-r--r--   0        0        0      493 2024-03-21 09:38:59.603781 allianceauth-4.0.1/allianceauth/authentication/templates/public/login.html
--rw-r--r--   0        0        0     1604 2024-03-21 09:38:59.603781 allianceauth-4.0.1/allianceauth/authentication/templates/public/middle_box.html
--rw-r--r--   0        0        0      956 2024-03-21 09:38:59.604781 allianceauth-4.0.1/allianceauth/authentication/templates/public/register.html
--rw-r--r--   0        0        0      199 2024-03-21 09:38:59.604781 allianceauth-4.0.1/allianceauth/authentication/templates/registration/activate.html
--rw-r--r--   0        0        0      346 2024-03-21 09:38:59.604781 allianceauth-4.0.1/allianceauth/authentication/templates/registration/activation_email.txt
--rw-r--r--   0        0        0      446 2024-03-21 09:38:59.604781 allianceauth-4.0.1/allianceauth/authentication/templates/registration/activation_email_html.txt
--rw-r--r--   0        0        0       49 2024-03-21 09:38:59.604781 allianceauth-4.0.1/allianceauth/authentication/templates/registration/activation_email_subject.txt
--rw-r--r--   0        0        0      833 2024-03-21 09:38:59.604781 allianceauth-4.0.1/allianceauth/authentication/tests/__init__.py
--rw-r--r--   0        0        0        0 2024-03-21 09:38:59.723780 allianceauth-4.0.1/allianceauth/authentication/tests/core/__init__.py
--rw-r--r--   0        0        0     2685 2024-03-21 09:38:59.604781 allianceauth-4.0.1/allianceauth/authentication/tests/core/test_celery_workers.py
--rw-r--r--   0        0        0    29475 2024-03-21 09:38:59.604781 allianceauth-4.0.1/allianceauth/authentication/tests/test_admin.py
--rw-r--r--   0        0        0     3456 2024-03-21 09:38:59.604781 allianceauth-4.0.1/allianceauth/authentication/tests/test_app_settings.py
--rw-r--r--   0        0        0     7427 2024-03-21 09:38:59.604781 allianceauth-4.0.1/allianceauth/authentication/tests/test_backend.py
--rw-r--r--   0        0        0     1517 2024-03-21 09:38:59.604781 allianceauth-4.0.1/allianceauth/authentication/tests/test_commands.py
--rw-r--r--   0        0        0     3538 2024-03-21 09:38:59.604781 allianceauth-4.0.1/allianceauth/authentication/tests/test_decorators.py
--rw-r--r--   0        0        0     6316 2024-03-21 09:38:59.605781 allianceauth-4.0.1/allianceauth/authentication/tests/test_middleware.py
--rw-r--r--   0        0        0    11478 2024-03-21 09:38:59.605781 allianceauth-4.0.1/allianceauth/authentication/tests/test_models.py
--rw-r--r--   0        0        0     3154 2024-03-21 09:38:59.605781 allianceauth-4.0.1/allianceauth/authentication/tests/test_signals.py
--rw-r--r--   0        0        0    10730 2024-03-21 09:38:59.605781 allianceauth-4.0.1/allianceauth/authentication/tests/test_templatetags.py
--rw-r--r--   0        0        0     5865 2024-03-21 09:38:59.605781 allianceauth-4.0.1/allianceauth/authentication/tests/test_views.py
--rw-r--r--   0        0        0     1170 2024-03-21 09:38:59.605781 allianceauth-4.0.1/allianceauth/authentication/urls.py
--rw-r--r--   0        0        0    14250 2024-03-21 09:38:59.605781 allianceauth-4.0.1/allianceauth/authentication/views.py
--rw-r--r--   0        0        0        0 2024-03-21 09:38:59.723780 allianceauth-4.0.1/allianceauth/bin/__init__.py
--rw-r--r--   0        0        0     3680 2024-03-21 09:38:59.605781 allianceauth-4.0.1/allianceauth/bin/allianceauth.py
--rw-r--r--   0        0        0      274 2024-03-21 09:38:59.605781 allianceauth-4.0.1/allianceauth/context_processors.py
--rw-r--r--   0        0        0        0 2024-03-21 09:38:59.723780 allianceauth-4.0.1/allianceauth/corputils/__init__.py
--rw-r--r--   0        0        0      140 2024-03-21 09:38:59.605781 allianceauth-4.0.1/allianceauth/corputils/admin.py
--rw-r--r--   0        0        0      130 2024-03-21 09:38:59.605781 allianceauth-4.0.1/allianceauth/corputils/apps.py
--rw-r--r--   0        0        0     1043 2024-03-21 09:38:59.605781 allianceauth-4.0.1/allianceauth/corputils/auth_hooks.py
--rw-r--r--   0        0        0     1970 2024-03-21 09:38:59.605781 allianceauth-4.0.1/allianceauth/corputils/managers.py
--rw-r--r--   0        0        0     1417 2024-03-21 09:38:59.606781 allianceauth-4.0.1/allianceauth/corputils/migrations/0001_initial.py
--rw-r--r--   0        0        0     5358 2024-03-21 09:38:59.606781 allianceauth-4.0.1/allianceauth/corputils/migrations/0002_migrate_permissions.py
--rw-r--r--   0        0        0      844 2024-03-21 09:38:59.606781 allianceauth-4.0.1/allianceauth/corputils/migrations/0003_granular_permissions.py
--rw-r--r--   0        0        0     2029 2024-03-21 09:38:59.606781 allianceauth-4.0.1/allianceauth/corputils/migrations/0004_member_models.py
--rw-r--r--   0        0        0     1516 2024-03-21 09:38:59.606781 allianceauth-4.0.1/allianceauth/corputils/migrations/0005_cleanup_permissions.py
--rw-r--r--   0        0        0        0 2024-03-21 09:38:59.723780 allianceauth-4.0.1/allianceauth/corputils/migrations/__init__.py
--rw-r--r--   0        0        0     7223 2024-03-21 09:38:59.606781 allianceauth-4.0.1/allianceauth/corputils/models.py
--rw-r--r--   0        0        0   947431 2024-03-21 09:38:59.608781 allianceauth-4.0.1/allianceauth/corputils/swagger.json
--rw-r--r--   0        0        0      298 2024-03-21 09:38:59.608781 allianceauth-4.0.1/allianceauth/corputils/tasks.py
--rw-r--r--   0        0        0     1991 2024-03-21 09:38:59.608781 allianceauth-4.0.1/allianceauth/corputils/templates/corputils/base.html
--rw-r--r--   0        0        0    14560 2024-03-21 09:38:59.608781 allianceauth-4.0.1/allianceauth/corputils/templates/corputils/corpstats.html
--rw-r--r--   0        0        0     2268 2024-03-21 09:38:59.609781 allianceauth-4.0.1/allianceauth/corputils/templates/corputils/search.html
--rw-r--r--   0        0        0    16016 2024-03-21 09:38:59.609781 allianceauth-4.0.1/allianceauth/corputils/tests.py
--rw-r--r--   0        0        0      393 2024-03-21 09:38:59.609781 allianceauth-4.0.1/allianceauth/corputils/urls.py
--rw-r--r--   0        0        0     6999 2024-03-21 09:38:59.609781 allianceauth-4.0.1/allianceauth/corputils/views.py
--rw-r--r--   0        0        0        0 2024-03-21 09:38:59.724780 allianceauth-4.0.1/allianceauth/eveonline/__init__.py
--rw-r--r--   0        0        0     7277 2024-03-21 09:38:59.609781 allianceauth-4.0.1/allianceauth/eveonline/admin.py
--rw-r--r--   0        0        0      130 2024-03-21 09:38:59.609781 allianceauth-4.0.1/allianceauth/eveonline/apps.py
--rw-r--r--   0        0        0        0 2024-03-21 09:38:59.724780 allianceauth-4.0.1/allianceauth/eveonline/autogroups/__init__.py
--rw-r--r--   0        0        0     1320 2024-03-21 09:38:59.609781 allianceauth-4.0.1/allianceauth/eveonline/autogroups/admin.py
--rw-r--r--   0        0        0      229 2024-03-21 09:38:59.609781 allianceauth-4.0.1/allianceauth/eveonline/autogroups/apps.py
--rw-r--r--   0        0        0     4024 2024-03-21 09:38:59.609781 allianceauth-4.0.1/allianceauth/eveonline/autogroups/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2024-03-21 09:38:59.724780 allianceauth-4.0.1/allianceauth/eveonline/autogroups/migrations/__init__.py
--rw-r--r--   0        0        0    10691 2024-03-21 09:38:59.609781 allianceauth-4.0.1/allianceauth/eveonline/autogroups/models.py
--rw-r--r--   0        0        0     2625 2024-03-21 09:38:59.609781 allianceauth-4.0.1/allianceauth/eveonline/autogroups/signals.py
--rw-r--r--   0        0        0     1403 2024-03-21 09:38:59.609781 allianceauth-4.0.1/allianceauth/eveonline/autogroups/tests/__init__.py
--rw-r--r--   0        0        0     3221 2024-03-21 09:38:59.610781 allianceauth-4.0.1/allianceauth/eveonline/autogroups/tests/test_managers.py
--rw-r--r--   0        0        0    12334 2024-03-21 09:38:59.610781 allianceauth-4.0.1/allianceauth/eveonline/autogroups/tests/test_models.py
--rw-r--r--   0        0        0     7961 2024-03-21 09:38:59.610781 allianceauth-4.0.1/allianceauth/eveonline/autogroups/tests/test_signals.py
--rw-r--r--   0        0        0      646 2024-03-21 09:38:59.610781 allianceauth-4.0.1/allianceauth/eveonline/evelinks/__init__.py
--rw-r--r--   0        0        0     1496 2024-03-21 09:38:59.610781 allianceauth-4.0.1/allianceauth/eveonline/evelinks/dotlan.py
--rw-r--r--   0        0        0     3730 2024-03-21 09:38:59.610781 allianceauth-4.0.1/allianceauth/eveonline/evelinks/eveimageserver.py
--rw-r--r--   0        0        0     1229 2024-03-21 09:38:59.610781 allianceauth-4.0.1/allianceauth/eveonline/evelinks/evewho.py
--rw-r--r--   0        0        0        0 2024-03-21 09:38:59.724780 allianceauth-4.0.1/allianceauth/eveonline/evelinks/tests/__init__.py
--rw-r--r--   0        0        0     7329 2024-03-21 09:38:59.610781 allianceauth-4.0.1/allianceauth/eveonline/evelinks/tests/test_evelinks.py
--rw-r--r--   0        0        0    11505 2024-03-21 09:38:59.610781 allianceauth-4.0.1/allianceauth/eveonline/evelinks/tests/test_templatetags.py
--rw-r--r--   0        0        0     1700 2024-03-21 09:38:59.610781 allianceauth-4.0.1/allianceauth/eveonline/evelinks/zkillboard.py
--rw-r--r--   0        0        0     3350 2024-03-21 09:38:59.610781 allianceauth-4.0.1/allianceauth/eveonline/managers.py
--rw-r--r--   0        0        0     3133 2024-03-21 09:38:59.610781 allianceauth-4.0.1/allianceauth/eveonline/migrations/0001_initial.py
--rw-r--r--   0        0        0      332 2024-03-21 09:38:59.610781 allianceauth-4.0.1/allianceauth/eveonline/migrations/0002_remove_eveapikeypair_error_count.py
--rw-r--r--   0        0        0      797 2024-03-21 09:38:59.610781 allianceauth-4.0.1/allianceauth/eveonline/migrations/0003_auto_20161026_0149.py
--rw-r--r--   0        0        0      403 2024-03-21 09:38:59.610781 allianceauth-4.0.1/allianceauth/eveonline/migrations/0004_eveapikeypair_sso_verified.py
--rw-r--r--   0        0        0      354 2024-03-21 09:38:59.610781 allianceauth-4.0.1/allianceauth/eveonline/migrations/0005_remove_eveallianceinfo_member_count.py
--rw-r--r--   0        0        0      655 2024-03-21 09:38:59.611781 allianceauth-4.0.1/allianceauth/eveonline/migrations/0006_allow_null_evecharacter_alliance.py
--rw-r--r--   0        0        0     4599 2024-03-21 09:38:59.611781 allianceauth-4.0.1/allianceauth/eveonline/migrations/0007_unique_id_name.py
--rw-r--r--   0        0        0      854 2024-03-21 09:38:59.611781 allianceauth-4.0.1/allianceauth/eveonline/migrations/0008_remove_apikeys.py
--rw-r--r--   0        0        0      519 2024-03-21 09:38:59.611781 allianceauth-4.0.1/allianceauth/eveonline/migrations/0009_on_delete.py
--rw-r--r--   0        0        0      596 2024-03-21 09:38:59.611781 allianceauth-4.0.1/allianceauth/eveonline/migrations/0010_alliance_ticker.py
--rw-r--r--   0        0        0     1297 2024-03-21 09:38:59.611781 allianceauth-4.0.1/allianceauth/eveonline/migrations/0011_ids_to_integers.py
--rw-r--r--   0        0        0     1121 2024-03-21 09:38:59.611781 allianceauth-4.0.1/allianceauth/eveonline/migrations/0012_index_additions.py
--rw-r--r--   0        0        0      428 2024-03-21 09:38:59.611781 allianceauth-4.0.1/allianceauth/eveonline/migrations/0013_evecorporationinfo_ceo_id.py
--rw-r--r--   0        0        0      416 2024-03-21 09:38:59.611781 allianceauth-4.0.1/allianceauth/eveonline/migrations/0014_auto_20210105_1413.py
--rw-r--r--   0        0        0     1201 2024-03-21 09:38:59.611781 allianceauth-4.0.1/allianceauth/eveonline/migrations/0015_factions.py
--rw-r--r--   0        0        0      409 2024-03-21 09:38:59.611781 allianceauth-4.0.1/allianceauth/eveonline/migrations/0016_character_names_are_not_unique.py
--rw-r--r--   0        0        0      623 2024-03-21 09:38:59.611781 allianceauth-4.0.1/allianceauth/eveonline/migrations/0017_alliance_and_corp_names_are_not_unique.py
--rw-r--r--   0        0        0        0 2024-03-21 09:38:59.726781 allianceauth-4.0.1/allianceauth/eveonline/migrations/__init__.py
--rw-r--r--   0        0        0    14052 2024-03-21 09:38:59.611781 allianceauth-4.0.1/allianceauth/eveonline/models.py
--rw-r--r--   0        0        0     9958 2024-03-21 09:38:59.611781 allianceauth-4.0.1/allianceauth/eveonline/providers.py
--rw-r--r--   0        0        0    41989 2024-03-21 09:38:59.612781 allianceauth-4.0.1/allianceauth/eveonline/swagger.json
--rw-r--r--   0        0        0     3808 2024-03-21 09:38:59.612781 allianceauth-4.0.1/allianceauth/eveonline/tasks.py
--rw-r--r--   0        0        0        0 2024-03-21 09:38:59.726781 allianceauth-4.0.1/allianceauth/eveonline/templatetags/__init__.py
--rw-r--r--   0        0        0     8354 2024-03-21 09:38:59.612781 allianceauth-4.0.1/allianceauth/eveonline/templatetags/evelinks.py
--rw-r--r--   0        0        0     4194 2024-03-21 09:38:59.612781 allianceauth-4.0.1/allianceauth/eveonline/templatetags/examples.html
--rw-r--r--   0        0        0      739 2024-03-21 09:38:59.613781 allianceauth-4.0.1/allianceauth/eveonline/tests/__init__.py
--rw-r--r--   0        0        0     6043 2024-03-21 09:38:59.613781 allianceauth-4.0.1/allianceauth/eveonline/tests/esi_client_stub.py
--rw-r--r--   0        0        0   297070 2024-03-21 09:38:59.613781 allianceauth-4.0.1/allianceauth/eveonline/tests/swagger_old.json
--rw-r--r--   0        0        0    10079 2024-03-21 09:38:59.613781 allianceauth-4.0.1/allianceauth/eveonline/tests/test_managers.py
--rw-r--r--   0        0        0    23361 2024-03-21 09:38:59.613781 allianceauth-4.0.1/allianceauth/eveonline/tests/test_models.py
--rw-r--r--   0        0        0    23834 2024-03-21 09:38:59.614781 allianceauth-4.0.1/allianceauth/eveonline/tests/test_providers.py
--rw-r--r--   0        0        0    10117 2024-03-21 09:38:59.614781 allianceauth-4.0.1/allianceauth/eveonline/tests/test_tasks.py
--rw-r--r--   0        0        0        0 2024-03-21 09:38:59.726781 allianceauth-4.0.1/allianceauth/eveonline/views.py
--rw-r--r--   0        0        0        0 2024-03-21 09:38:59.726781 allianceauth-4.0.1/allianceauth/fleetactivitytracking/__init__.py
--rw-r--r--   0        0        0      156 2024-03-21 09:38:59.614781 allianceauth-4.0.1/allianceauth/fleetactivitytracking/admin.py
--rw-r--r--   0        0        0      148 2024-03-21 09:38:59.614781 allianceauth-4.0.1/allianceauth/fleetactivitytracking/apps.py
--rw-r--r--   0        0        0      494 2024-03-21 09:38:59.614781 allianceauth-4.0.1/allianceauth/fleetactivitytracking/auth_hooks.py
--rw-r--r--   0        0        0      360 2024-03-21 09:38:59.614781 allianceauth-4.0.1/allianceauth/fleetactivitytracking/forms.py
--rw-r--r--   0        0        0     2291 2024-03-21 09:38:59.614781 allianceauth-4.0.1/allianceauth/fleetactivitytracking/migrations/0001_initial.py
--rw-r--r--   0        0        0      489 2024-03-21 09:38:59.614781 allianceauth-4.0.1/allianceauth/fleetactivitytracking/migrations/0002_auto_20160905_2220.py
--rw-r--r--   0        0        0      460 2024-03-21 09:38:59.614781 allianceauth-4.0.1/allianceauth/fleetactivitytracking/migrations/0003_auto_20160906_2354.py
--rw-r--r--   0        0        0      414 2024-03-21 09:38:59.614781 allianceauth-4.0.1/allianceauth/fleetactivitytracking/migrations/0004_make_strings_more_stringy.py
--rw-r--r--   0        0        0      510 2024-03-21 09:38:59.614781 allianceauth-4.0.1/allianceauth/fleetactivitytracking/migrations/0005_remove_fat_name.py
--rw-r--r--   0        0        0      397 2024-03-21 09:38:59.614781 allianceauth-4.0.1/allianceauth/fleetactivitytracking/migrations/0006_auto_20180803_0430.py
--rw-r--r--   0        0        0      606 2024-03-21 09:38:59.614781 allianceauth-4.0.1/allianceauth/fleetactivitytracking/migrations/0007_sentinel_user.py
--rw-r--r--   0        0        0        0 2024-03-21 09:38:59.728780 allianceauth-4.0.1/allianceauth/fleetactivitytracking/migrations/__init__.py
--rw-r--r--   0        0        0     1122 2024-03-21 09:38:59.614781 allianceauth-4.0.1/allianceauth/fleetactivitytracking/models.py
--rw-r--r--   0        0        0   947431 2024-03-21 09:38:59.616781 allianceauth-4.0.1/allianceauth/fleetactivitytracking/swagger.json
--rw-r--r--   0        0        0     1851 2024-03-21 09:38:59.617781 allianceauth-4.0.1/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/characternotexisting.html
--rw-r--r--   0        0        0     1880 2024-03-21 09:38:59.617781 allianceauth-4.0.1/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/fatlinkcreate.html
--rw-r--r--   0        0        0     2811 2024-03-21 09:38:59.617781 allianceauth-4.0.1/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/fatlinkmodify.html
--rw-r--r--   0        0        0     4516 2024-03-21 09:38:59.617781 allianceauth-4.0.1/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/fatlinkpersonalmonthlystatisticsview.html
--rw-r--r--   0        0        0     1725 2024-03-21 09:38:59.617781 allianceauth-4.0.1/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/fatlinkpersonalstatisticsview.html
--rw-r--r--   0        0        0     2730 2024-03-21 09:38:59.617781 allianceauth-4.0.1/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/fatlinkstatisticscorpview.html
--rw-r--r--   0        0        0     3011 2024-03-21 09:38:59.617781 allianceauth-4.0.1/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/fatlinkstatisticsview.html
--rw-r--r--   0        0        0     5912 2024-03-21 09:38:59.617781 allianceauth-4.0.1/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/fatlinkview.html
--rw-r--r--   0        0        0     1386 2024-03-21 09:38:59.617781 allianceauth-4.0.1/allianceauth/fleetactivitytracking/urls.py
--rw-r--r--   0        0        0    16656 2024-03-21 09:38:59.617781 allianceauth-4.0.1/allianceauth/fleetactivitytracking/views.py
--rw-r--r--   0        0        0       32 2024-03-21 09:38:59.617781 allianceauth-4.0.1/allianceauth/framework/__init__.py
--rw-r--r--   0        0        0     1421 2024-03-21 09:38:59.617781 allianceauth-4.0.1/allianceauth/framework/api/evecharacter.py
--rw-r--r--   0        0        0     1723 2024-03-21 09:38:59.617781 allianceauth-4.0.1/allianceauth/framework/api/user.py
--rw-r--r--   0        0        0      202 2024-03-21 09:38:59.617781 allianceauth-4.0.1/allianceauth/framework/apps.py
--rw-r--r--   0        0        0     3174 2024-03-21 09:38:59.617781 allianceauth-4.0.1/allianceauth/framework/static/allianceauth/framework/css/auth-framework.css
--rw-r--r--   0        0        0      317 2024-03-21 09:38:59.617781 allianceauth-4.0.1/allianceauth/framework/templates/framework/header/page-header.html
--rw-r--r--   0        0        0       31 2024-03-21 09:38:59.618781 allianceauth-4.0.1/allianceauth/framework/tests/__init__.py
--rw-r--r--   0        0        0     4468 2024-03-21 09:38:59.618781 allianceauth-4.0.1/allianceauth/framework/tests/test_api_user.py
--rw-r--r--   0        0        0        0 2024-03-21 09:38:59.728780 allianceauth-4.0.1/allianceauth/groupmanagement/__init__.py
--rw-r--r--   0        0        0     8978 2024-03-21 09:38:59.618781 allianceauth-4.0.1/allianceauth/groupmanagement/admin.py
--rw-r--r--   0        0        0      252 2024-03-21 09:38:59.618781 allianceauth-4.0.1/allianceauth/groupmanagement/apps.py
--rw-r--r--   0        0        0     2336 2024-03-21 09:38:59.618781 allianceauth-4.0.1/allianceauth/groupmanagement/auth_hooks.py
--rw-r--r--   0        0        0     2466 2024-03-21 09:38:59.618781 allianceauth-4.0.1/allianceauth/groupmanagement/forms.py
--rw-r--r--   0        0        0     4341 2024-03-21 09:38:59.618781 allianceauth-4.0.1/allianceauth/groupmanagement/managers.py
--rw-r--r--   0        0        0     2243 2024-03-21 09:38:59.618781 allianceauth-4.0.1/allianceauth/groupmanagement/migrations/0001_initial.py
--rw-r--r--   0        0        0      685 2024-03-21 09:38:59.618781 allianceauth-4.0.1/allianceauth/groupmanagement/migrations/0002_auto_20160906_2354.py
--rw-r--r--   0        0        0      261 2024-03-21 09:38:59.618781 allianceauth-4.0.1/allianceauth/groupmanagement/migrations/0003_default_groups.py
--rw-r--r--   0        0        0     4322 2024-03-21 09:38:59.618781 allianceauth-4.0.1/allianceauth/groupmanagement/migrations/0004_authgroup.py
--rw-r--r--   0        0        0      631 2024-03-21 09:38:59.618781 allianceauth-4.0.1/allianceauth/groupmanagement/migrations/0005_authgroup_public.py
--rw-r--r--   0        0        0      607 2024-03-21 09:38:59.618781 allianceauth-4.0.1/allianceauth/groupmanagement/migrations/0006_request_groups_perm.py
--rw-r--r--   0        0        0      877 2024-03-21 09:38:59.618781 allianceauth-4.0.1/allianceauth/groupmanagement/migrations/0007_on_delete.py
--rw-r--r--   0        0        0     1430 2024-03-21 09:38:59.618781 allianceauth-4.0.1/allianceauth/groupmanagement/migrations/0008_remove_authgroup_permissions.py
--rw-r--r--   0        0        0     1100 2024-03-21 09:38:59.618781 allianceauth-4.0.1/allianceauth/groupmanagement/migrations/0009_requestlog.py
--rw-r--r--   0        0        0      614 2024-03-21 09:38:59.618781 allianceauth-4.0.1/allianceauth/groupmanagement/migrations/0010_authgroup_states.py
--rw-r--r--   0        0        0      456 2024-03-21 09:38:59.618781 allianceauth-4.0.1/allianceauth/groupmanagement/migrations/0011_requestlog_date.py
--rw-r--r--   0        0        0      672 2024-03-21 09:38:59.618781 allianceauth-4.0.1/allianceauth/groupmanagement/migrations/0012_group_leads.py
--rw-r--r--   0        0        0      397 2024-03-21 09:38:59.618781 allianceauth-4.0.1/allianceauth/groupmanagement/migrations/0013_fix_requestlog_date_field.py
--rw-r--r--   0        0        0      410 2024-03-21 09:38:59.619781 allianceauth-4.0.1/allianceauth/groupmanagement/migrations/0014_auto_20200918_1412.py
--rw-r--r--   0        0        0      567 2024-03-21 09:38:59.619781 allianceauth-4.0.1/allianceauth/groupmanagement/migrations/0015_make_descriptions_great_again.py
--rw-r--r--   0        0        0      353 2024-03-21 09:38:59.619781 allianceauth-4.0.1/allianceauth/groupmanagement/migrations/0016_remove_grouprequest_status_field.py
--rw-r--r--   0        0        0     2296 2024-03-21 09:38:59.619781 allianceauth-4.0.1/allianceauth/groupmanagement/migrations/0017_improve_groups_documentation.py
--rw-r--r--   0        0        0     1082 2024-03-21 09:38:59.619781 allianceauth-4.0.1/allianceauth/groupmanagement/migrations/0018_reservedgroupname.py
--rw-r--r--   0        0        0      520 2024-03-21 09:38:59.619781 allianceauth-4.0.1/allianceauth/groupmanagement/migrations/0019_adding_restricted_to_groups.py
--rw-r--r--   0        0        0        0 2024-03-21 09:38:59.730780 allianceauth-4.0.1/allianceauth/groupmanagement/migrations/__init__.py
--rw-r--r--   0        0        0     8132 2024-03-21 09:38:59.619781 allianceauth-4.0.1/allianceauth/groupmanagement/models.py
--rw-r--r--   0        0        0     1465 2024-03-21 09:38:59.619781 allianceauth-4.0.1/allianceauth/groupmanagement/signals.py
--rw-r--r--   0        0        0      333 2024-03-21 09:38:59.619781 allianceauth-4.0.1/allianceauth/groupmanagement/tasks.py
--rw-r--r--   0        0        0     4516 2024-03-21 09:38:59.619781 allianceauth-4.0.1/allianceauth/groupmanagement/templates/groupmanagement/audit.html
--rw-r--r--   0        0        0     4003 2024-03-21 09:38:59.619781 allianceauth-4.0.1/allianceauth/groupmanagement/templates/groupmanagement/groupmembers.html
--rw-r--r--   0        0        0     3764 2024-03-21 09:38:59.619781 allianceauth-4.0.1/allianceauth/groupmanagement/templates/groupmanagement/groupmembership.html
--rw-r--r--   0        0        0     4854 2024-03-21 09:38:59.619781 allianceauth-4.0.1/allianceauth/groupmanagement/templates/groupmanagement/groups.html
--rw-r--r--   0        0        0     8485 2024-03-21 09:38:59.619781 allianceauth-4.0.1/allianceauth/groupmanagement/templates/groupmanagement/index.html
--rw-r--r--   0        0        0      445 2024-03-21 09:38:59.619781 allianceauth-4.0.1/allianceauth/groupmanagement/templates/groupmanagement/menu.html
--rw-r--r--   0        0        0      254 2024-03-21 09:38:59.619781 allianceauth-4.0.1/allianceauth/groupmanagement/tests/__init__.py
--rw-r--r--   0        0        0    27572 2024-03-21 09:38:59.620781 allianceauth-4.0.1/allianceauth/groupmanagement/tests/test_admin.py
--rw-r--r--   0        0        0    17375 2024-03-21 09:38:59.620781 allianceauth-4.0.1/allianceauth/groupmanagement/tests/test_managers.py
--rw-r--r--   0        0        0    11668 2024-03-21 09:38:59.620781 allianceauth-4.0.1/allianceauth/groupmanagement/tests/test_models.py
--rw-r--r--   0        0        0     4950 2024-03-21 09:38:59.620781 allianceauth-4.0.1/allianceauth/groupmanagement/tests/test_signals.py
--rw-r--r--   0        0        0     3999 2024-03-21 09:38:59.620781 allianceauth-4.0.1/allianceauth/groupmanagement/tests/test_views.py
--rw-r--r--   0        0        0     1651 2024-03-21 09:38:59.620781 allianceauth-4.0.1/allianceauth/groupmanagement/urls.py
--rw-r--r--   0        0        0    20437 2024-03-21 09:38:59.620781 allianceauth-4.0.1/allianceauth/groupmanagement/views.py
--rw-r--r--   0        0        0     4570 2024-03-21 09:38:59.620781 allianceauth-4.0.1/allianceauth/hooks.py
--rw-r--r--   0        0        0        0 2024-03-21 09:38:59.734780 allianceauth-4.0.1/allianceauth/hrapplications/__init__.py
--rw-r--r--   0        0        0      693 2024-03-21 09:38:59.620781 allianceauth-4.0.1/allianceauth/hrapplications/admin.py
--rw-r--r--   0        0        0      145 2024-03-21 09:38:59.620781 allianceauth-4.0.1/allianceauth/hrapplications/apps.py
--rw-r--r--   0        0        0     1023 2024-03-21 09:38:59.620781 allianceauth-4.0.1/allianceauth/hrapplications/auth_hooks.py
--rw-r--r--   0        0        0      353 2024-03-21 09:38:59.620781 allianceauth-4.0.1/allianceauth/hrapplications/forms.py
--rw-r--r--   0        0        0      900 2024-03-21 09:38:59.620781 allianceauth-4.0.1/allianceauth/hrapplications/managers.py
--rw-r--r--   0        0        0     6662 2024-03-21 09:38:59.620781 allianceauth-4.0.1/allianceauth/hrapplications/migrations/0001_initial.py
--rw-r--r--   0        0        0     1036 2024-03-21 09:38:59.620781 allianceauth-4.0.1/allianceauth/hrapplications/migrations/0002_choices_for_questions.py
--rw-r--r--   0        0        0      415 2024-03-21 09:38:59.620781 allianceauth-4.0.1/allianceauth/hrapplications/migrations/0003_applicationquestion_multi_select.py
--rw-r--r--   0        0        0     1461 2024-03-21 09:38:59.621781 allianceauth-4.0.1/allianceauth/hrapplications/migrations/0004_make_strings_more_stringy.py
--rw-r--r--   0        0        0      558 2024-03-21 09:38:59.621781 allianceauth-4.0.1/allianceauth/hrapplications/migrations/0005_sorted_questions.py
--rw-r--r--   0        0        0     1946 2024-03-21 09:38:59.621781 allianceauth-4.0.1/allianceauth/hrapplications/migrations/0006_remove_legacy_models.py
--rw-r--r--   0        0        0      427 2024-03-21 09:38:59.621781 allianceauth-4.0.1/allianceauth/hrapplications/migrations/0007_auto_20200918_1412.py
--rw-r--r--   0        0        0        0 2024-03-21 09:38:59.734780 allianceauth-4.0.1/allianceauth/hrapplications/migrations/__init__.py
--rw-r--r--   0        0        0     3237 2024-03-21 09:38:59.621781 allianceauth-4.0.1/allianceauth/hrapplications/models.py
--rw-r--r--   0        0        0     1411 2024-03-21 09:38:59.621781 allianceauth-4.0.1/allianceauth/hrapplications/templates/hrapplications/corpchoice.html
--rw-r--r--   0        0        0     2946 2024-03-21 09:38:59.621781 allianceauth-4.0.1/allianceauth/hrapplications/templates/hrapplications/create.html
--rw-r--r--   0        0        0    12438 2024-03-21 09:38:59.621781 allianceauth-4.0.1/allianceauth/hrapplications/templates/hrapplications/management.html
--rw-r--r--   0        0        0     1308 2024-03-21 09:38:59.621781 allianceauth-4.0.1/allianceauth/hrapplications/templates/hrapplications/partials/modals/search.html
--rw-r--r--   0        0        0     2772 2024-03-21 09:38:59.621781 allianceauth-4.0.1/allianceauth/hrapplications/templates/hrapplications/searchview.html
--rw-r--r--   0        0        0     8251 2024-03-21 09:38:59.621781 allianceauth-4.0.1/allianceauth/hrapplications/templates/hrapplications/view.html
--rw-r--r--   0        0        0     4165 2024-03-21 09:38:59.621781 allianceauth-4.0.1/allianceauth/hrapplications/tests.py
--rw-r--r--   0        0        0     1113 2024-03-21 09:38:59.621781 allianceauth-4.0.1/allianceauth/hrapplications/urls.py
--rw-r--r--   0        0        0    12011 2024-03-21 09:38:59.621781 allianceauth-4.0.1/allianceauth/hrapplications/views.py
--rw-r--r--   0        0        0    45125 2024-03-21 09:38:59.622781 allianceauth-4.0.1/allianceauth/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0   100410 2024-03-21 09:38:59.622781 allianceauth-4.0.1/allianceauth/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      380 2024-03-21 09:38:59.623781 allianceauth-4.0.1/allianceauth/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    83104 2024-03-21 09:38:59.623781 allianceauth-4.0.1/allianceauth/locale/en/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    35108 2024-03-21 09:38:59.623781 allianceauth-4.0.1/allianceauth/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    96449 2024-03-21 09:38:59.623781 allianceauth-4.0.1/allianceauth/locale/es/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    46059 2024-03-21 09:38:59.624781 allianceauth-4.0.1/allianceauth/locale/fr_FR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0   101519 2024-03-21 09:38:59.624781 allianceauth-4.0.1/allianceauth/locale/fr_FR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    44568 2024-03-21 09:38:59.624781 allianceauth-4.0.1/allianceauth/locale/it_IT/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0   100361 2024-03-21 09:38:59.625781 allianceauth-4.0.1/allianceauth/locale/it_IT/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    49616 2024-03-21 09:38:59.625781 allianceauth-4.0.1/allianceauth/locale/ja/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0   104688 2024-03-21 09:38:59.625781 allianceauth-4.0.1/allianceauth/locale/ja/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    46390 2024-03-21 09:38:59.625781 allianceauth-4.0.1/allianceauth/locale/ko_KR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0   101604 2024-03-21 09:38:59.626781 allianceauth-4.0.1/allianceauth/locale/ko_KR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    45746 2024-03-21 09:38:59.626781 allianceauth-4.0.1/allianceauth/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0   106164 2024-03-21 09:38:59.626781 allianceauth-4.0.1/allianceauth/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    57333 2024-03-21 09:38:59.627781 allianceauth-4.0.1/allianceauth/locale/uk/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0   112647 2024-03-21 09:38:59.627781 allianceauth-4.0.1/allianceauth/locale/uk/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    26591 2024-03-21 09:38:59.627781 allianceauth-4.0.1/allianceauth/locale/zh_Hans/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    91902 2024-03-21 09:38:59.627781 allianceauth-4.0.1/allianceauth/locale/zh_Hans/LC_MESSAGES/django.po
--rw-r--r--   0        0        0        0 2024-03-21 09:38:59.734780 allianceauth-4.0.1/allianceauth/menu/__init__.py
--rw-r--r--   0        0        0     3721 2024-03-21 09:38:59.627781 allianceauth-4.0.1/allianceauth/menu/admin.py
--rw-r--r--   0        0        0      459 2024-03-21 09:38:59.627781 allianceauth-4.0.1/allianceauth/menu/apps.py
--rw-r--r--   0        0        0      485 2024-03-21 09:38:59.627781 allianceauth-4.0.1/allianceauth/menu/constants.py
--rw-r--r--   0        0        0        0 2024-03-21 09:38:59.734780 allianceauth-4.0.1/allianceauth/menu/core/__init__.py
--rw-r--r--   0        0        0     1363 2024-03-21 09:38:59.627781 allianceauth-4.0.1/allianceauth/menu/core/menu_item_hooks.py
--rw-r--r--   0        0        0      892 2024-03-21 09:38:59.627781 allianceauth-4.0.1/allianceauth/menu/core/smart_sync.py
--rw-r--r--   0        0        0      688 2024-03-21 09:38:59.627781 allianceauth-4.0.1/allianceauth/menu/filters.py
--rw-r--r--   0        0        0     1397 2024-03-21 09:38:59.628781 allianceauth-4.0.1/allianceauth/menu/forms.py
--rw-r--r--   0        0        0     1932 2024-03-21 09:38:59.628781 allianceauth-4.0.1/allianceauth/menu/hooks.py
--rw-r--r--   0        0        0     2288 2024-03-21 09:38:59.628781 allianceauth-4.0.1/allianceauth/menu/managers.py
--rw-r--r--   0        0        0     3143 2024-03-21 09:38:59.628781 allianceauth-4.0.1/allianceauth/menu/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2024-03-21 09:38:59.734780 allianceauth-4.0.1/allianceauth/menu/migrations/__init__.py
--rw-r--r--   0        0        0     4094 2024-03-21 09:38:59.628781 allianceauth-4.0.1/allianceauth/menu/models.py
--rw-r--r--   0        0        0      289 2024-03-21 09:38:59.628781 allianceauth-4.0.1/allianceauth/menu/templates/admin/menu/menuitem/change_list.html
--rw-r--r--   0        0        0       62 2024-03-21 09:38:59.628781 allianceauth-4.0.1/allianceauth/menu/templates/menu/menu-block.html
--rw-r--r--   0        0        0     2009 2024-03-21 09:38:59.628781 allianceauth-4.0.1/allianceauth/menu/templates/menu/menu-item-bs5.html
--rw-r--r--   0        0        0      101 2024-03-21 09:38:59.628781 allianceauth-4.0.1/allianceauth/menu/templates/menu/menu-logo.html
--rw-r--r--   0        0        0      535 2024-03-21 09:38:59.628781 allianceauth-4.0.1/allianceauth/menu/templates/menu/menu-notification-block.html
--rw-r--r--   0        0        0     5068 2024-03-21 09:38:59.628781 allianceauth-4.0.1/allianceauth/menu/templates/menu/menu-user.html
--rw-r--r--   0        0        0     1308 2024-03-21 09:38:59.628781 allianceauth-4.0.1/allianceauth/menu/templates/menu/sortable-side-menu.html
--rw-r--r--   0        0        0        0 2024-03-21 09:38:59.734780 allianceauth-4.0.1/allianceauth/menu/templatetags/__init__.py
--rw-r--r--   0        0        0      893 2024-03-21 09:38:59.628781 allianceauth-4.0.1/allianceauth/menu/templatetags/menu_items.py
--rw-r--r--   0        0        0     5996 2024-03-21 09:38:59.628781 allianceauth-4.0.1/allianceauth/menu/templatetags/menu_menu_items.py
--rw-r--r--   0        0        0        0 2024-03-21 09:38:59.734780 allianceauth-4.0.1/allianceauth/menu/tests/__init__.py
--rw-r--r--   0        0        0        0 2024-03-21 09:38:59.734780 allianceauth-4.0.1/allianceauth/menu/tests/core/__init__.py
--rw-r--r--   0        0        0     1799 2024-03-21 09:38:59.628781 allianceauth-4.0.1/allianceauth/menu/tests/core/test_menu_item_hooks.py
--rw-r--r--   0        0        0     1153 2024-03-21 09:38:59.629781 allianceauth-4.0.1/allianceauth/menu/tests/core/test_smart_sync.py
--rw-r--r--   0        0        0     2763 2024-03-21 09:38:59.629781 allianceauth-4.0.1/allianceauth/menu/tests/factories.py
--rw-r--r--   0        0        0        0 2024-03-21 09:38:59.734780 allianceauth-4.0.1/allianceauth/menu/tests/integration/__init__.py
--rw-r--r--   0        0        0     6367 2024-03-21 09:38:59.629781 allianceauth-4.0.1/allianceauth/menu/tests/integration/test_admin.py
--rw-r--r--   0        0        0     3736 2024-03-21 09:38:59.629781 allianceauth-4.0.1/allianceauth/menu/tests/integration/test_dashboard.py
--rw-r--r--   0        0        0        0 2024-03-21 09:38:59.734780 allianceauth-4.0.1/allianceauth/menu/tests/templatetags/__init__.py
--rw-r--r--   0        0        0     1688 2024-03-21 09:38:59.629781 allianceauth-4.0.1/allianceauth/menu/tests/templatetags/test_menu_items.py
--rw-r--r--   0        0        0    11656 2024-03-21 09:38:59.629781 allianceauth-4.0.1/allianceauth/menu/tests/templatetags/test_menu_menu_items.py
--rw-r--r--   0        0        0      833 2024-03-21 09:38:59.629781 allianceauth-4.0.1/allianceauth/menu/tests/test_forms.py
--rw-r--r--   0        0        0     2511 2024-03-21 09:38:59.629781 allianceauth-4.0.1/allianceauth/menu/tests/test_hooks.py
--rw-r--r--   0        0        0     3470 2024-03-21 09:38:59.629781 allianceauth-4.0.1/allianceauth/menu/tests/test_managers.py
--rw-r--r--   0        0        0     4831 2024-03-21 09:38:59.629781 allianceauth-4.0.1/allianceauth/menu/tests/test_models.py
--rw-r--r--   0        0        0     1177 2024-03-21 09:38:59.629781 allianceauth-4.0.1/allianceauth/menu/tests/utils.py
--rw-r--r--   0        0        0        0 2024-03-21 09:38:59.734780 allianceauth-4.0.1/allianceauth/models.py
--rw-r--r--   0        0        0       39 2024-03-21 09:38:59.629781 allianceauth-4.0.1/allianceauth/notifications/__init__.py
--rw-r--r--   0        0        0     1138 2024-03-21 09:38:59.629781 allianceauth-4.0.1/allianceauth/notifications/admin.py
--rw-r--r--   0        0        0      142 2024-03-21 09:38:59.629781 allianceauth-4.0.1/allianceauth/notifications/apps.py
--rw-r--r--   0        0        0     1320 2024-03-21 09:38:59.629781 allianceauth-4.0.1/allianceauth/notifications/core.py
--rw-r--r--   0        0        0      998 2024-03-21 09:38:59.629781 allianceauth-4.0.1/allianceauth/notifications/handlers.py
--rw-r--r--   0        0        0     3907 2024-03-21 09:38:59.629781 allianceauth-4.0.1/allianceauth/notifications/managers.py
--rw-r--r--   0        0        0     1117 2024-03-21 09:38:59.629781 allianceauth-4.0.1/allianceauth/notifications/migrations/0001_initial.py
--rw-r--r--   0        0        0      353 2024-03-21 09:38:59.630781 allianceauth-4.0.1/allianceauth/notifications/migrations/0002_auto_20160910_1649.py
--rw-r--r--   0        0        0      514 2024-03-21 09:38:59.630781 allianceauth-4.0.1/allianceauth/notifications/migrations/0003_make_strings_more_stringy.py
--rw-r--r--   0        0        0      714 2024-03-21 09:38:59.630781 allianceauth-4.0.1/allianceauth/notifications/migrations/0004_performance_tuning.py
--rw-r--r--   0        0        0      512 2024-03-21 09:38:59.630781 allianceauth-4.0.1/allianceauth/notifications/migrations/0005_fix_level_choices.py
--rw-r--r--   0        0        0        0 2024-03-21 09:38:59.735780 allianceauth-4.0.1/allianceauth/notifications/migrations/__init__.py
--rw-r--r--   0        0        0     2772 2024-03-21 09:38:59.630781 allianceauth-4.0.1/allianceauth/notifications/models.py
--rw-r--r--   0        0        0     1857 2024-03-21 09:38:59.630781 allianceauth-4.0.1/allianceauth/notifications/templates/notifications/list.html
--rw-r--r--   0        0        0     1070 2024-03-21 09:38:59.630781 allianceauth-4.0.1/allianceauth/notifications/templates/notifications/list_partial.html
--rw-r--r--   0        0        0      736 2024-03-21 09:38:59.630781 allianceauth-4.0.1/allianceauth/notifications/templates/notifications/view.html
--rw-r--r--   0        0        0        0 2024-03-21 09:38:59.735780 allianceauth-4.0.1/allianceauth/notifications/templatetags/__init__.py
--rw-r--r--   0        0        0     1156 2024-03-21 09:38:59.630781 allianceauth-4.0.1/allianceauth/notifications/templatetags/auth_notifications.py
--rw-r--r--   0        0        0        0 2024-03-21 09:38:59.735780 allianceauth-4.0.1/allianceauth/notifications/tests/__init__.py
--rw-r--r--   0        0        0     3073 2024-03-21 09:38:59.630781 allianceauth-4.0.1/allianceauth/notifications/tests/test_core.py
--rw-r--r--   0        0        0     2392 2024-03-21 09:38:59.630781 allianceauth-4.0.1/allianceauth/notifications/tests/test_handlers.py
--rw-r--r--   0        0        0     1120 2024-03-21 09:38:59.630781 allianceauth-4.0.1/allianceauth/notifications/tests/test_init.py
--rw-r--r--   0        0        0     9437 2024-03-21 09:38:59.630781 allianceauth-4.0.1/allianceauth/notifications/tests/test_managers.py
--rw-r--r--   0        0        0     2398 2024-03-21 09:38:59.630781 allianceauth-4.0.1/allianceauth/notifications/tests/test_models.py
--rw-r--r--   0        0        0     2975 2024-03-21 09:38:59.630781 allianceauth-4.0.1/allianceauth/notifications/tests/test_templatetags.py
--rw-r--r--   0        0        0     1463 2024-03-21 09:38:59.630781 allianceauth-4.0.1/allianceauth/notifications/tests/test_views.py
--rw-r--r--   0        0        0      674 2024-03-21 09:38:59.630781 allianceauth-4.0.1/allianceauth/notifications/urls.py
--rw-r--r--   0        0        0     3522 2024-03-21 09:38:59.630781 allianceauth-4.0.1/allianceauth/notifications/views.py
--rw-r--r--   0        0        0        0 2024-03-21 09:38:59.735780 allianceauth-4.0.1/allianceauth/optimer/__init__.py
--rw-r--r--   0        0        0      158 2024-03-21 09:38:59.631781 allianceauth-4.0.1/allianceauth/optimer/admin.py
--rw-r--r--   0        0        0      124 2024-03-21 09:38:59.631781 allianceauth-4.0.1/allianceauth/optimer/apps.py
--rw-r--r--   0        0        0     1183 2024-03-21 09:38:59.631781 allianceauth-4.0.1/allianceauth/optimer/auth_hooks.py
--rw-r--r--   0        0        0     1368 2024-03-21 09:38:59.631781 allianceauth-4.0.1/allianceauth/optimer/form.py
--rw-r--r--   0        0        0     1047 2024-03-21 09:38:59.631781 allianceauth-4.0.1/allianceauth/optimer/form_widgets.py
--rw-r--r--   0        0        0     1452 2024-03-21 09:38:59.631781 allianceauth-4.0.1/allianceauth/optimer/migrations/0001_initial.py
--rw-r--r--   0        0        0      424 2024-03-21 09:38:59.631781 allianceauth-4.0.1/allianceauth/optimer/migrations/0002_auto_20170413_0442.py
--rw-r--r--   0        0        0     1076 2024-03-21 09:38:59.631781 allianceauth-4.0.1/allianceauth/optimer/migrations/0003_make_strings_more_stringy.py
--rw-r--r--   0        0        0      507 2024-03-21 09:38:59.631781 allianceauth-4.0.1/allianceauth/optimer/migrations/0004_on_delete.py
--rw-r--r--   0        0        0     1447 2024-03-21 09:38:59.631781 allianceauth-4.0.1/allianceauth/optimer/migrations/0005_add_type_and_description.py
--rw-r--r--   0        0        0        0 2024-03-21 09:38:59.736780 allianceauth-4.0.1/allianceauth/optimer/migrations/__init__.py
--rw-r--r--   0        0        0     1247 2024-03-21 09:38:59.631781 allianceauth-4.0.1/allianceauth/optimer/models.py
--rw-r--r--   0        0        0     1980 2024-03-21 09:38:59.631781 allianceauth-4.0.1/allianceauth/optimer/templates/optimer/add.html
--rw-r--r--   0        0        0     1803 2024-03-21 09:38:59.631781 allianceauth-4.0.1/allianceauth/optimer/templates/optimer/dashboard.ops.html
--rw-r--r--   0        0        0     2612 2024-03-21 09:38:59.631781 allianceauth-4.0.1/allianceauth/optimer/templates/optimer/fleetoptable.html
--rw-r--r--   0        0        0     4378 2024-03-21 09:38:59.631781 allianceauth-4.0.1/allianceauth/optimer/templates/optimer/management.html
--rw-r--r--   0        0        0     1986 2024-03-21 09:38:59.631781 allianceauth-4.0.1/allianceauth/optimer/templates/optimer/update.html
--rw-r--r--   0        0        0       26 2024-03-21 09:38:59.631781 allianceauth-4.0.1/allianceauth/optimer/tests.py
--rw-r--r--   0        0        0      336 2024-03-21 09:38:59.631781 allianceauth-4.0.1/allianceauth/optimer/urls.py
--rw-r--r--   0        0        0     7139 2024-03-21 09:38:59.632781 allianceauth-4.0.1/allianceauth/optimer/views.py
--rw-r--r--   0        0        0        0 2024-03-21 09:38:59.736780 allianceauth-4.0.1/allianceauth/permissions_tool/__init__.py
--rw-r--r--   0        0        0      150 2024-03-21 09:38:59.632781 allianceauth-4.0.1/allianceauth/permissions_tool/apps.py
--rw-r--r--   0        0        0      821 2024-03-21 09:38:59.632781 allianceauth-4.0.1/allianceauth/permissions_tool/auth_hooks.py
--rw-r--r--   0        0        0      589 2024-03-21 09:38:59.632781 allianceauth-4.0.1/allianceauth/permissions_tool/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2024-03-21 09:38:59.741780 allianceauth-4.0.1/allianceauth/permissions_tool/migrations/__init__.py
--rw-r--r--   0        0        0      258 2024-03-21 09:38:59.632781 allianceauth-4.0.1/allianceauth/permissions_tool/models.py
--rw-r--r--   0        0        0     3874 2024-03-21 09:38:59.632781 allianceauth-4.0.1/allianceauth/permissions_tool/templates/permissions_tool/audit.html
--rw-r--r--   0        0        0      789 2024-03-21 09:38:59.632781 allianceauth-4.0.1/allianceauth/permissions_tool/templates/permissions_tool/audit_row.html
--rw-r--r--   0        0        0     4553 2024-03-21 09:38:59.632781 allianceauth-4.0.1/allianceauth/permissions_tool/templates/permissions_tool/overview.html
--rw-r--r--   0        0        0     5067 2024-03-21 09:38:59.632781 allianceauth-4.0.1/allianceauth/permissions_tool/tests.py
--rw-r--r--   0        0        0      340 2024-03-21 09:38:59.632781 allianceauth-4.0.1/allianceauth/permissions_tool/urls.py
--rw-r--r--   0        0        0     2610 2024-03-21 09:38:59.632781 allianceauth-4.0.1/allianceauth/permissions_tool/views.py
--rw-r--r--   0        0        0        0 2024-03-21 09:38:59.742780 allianceauth-4.0.1/allianceauth/project_template/__init__.py
--rw-r--r--   0        0        0        0 2024-03-21 09:38:59.742780 allianceauth-4.0.1/allianceauth/project_template/log/.gitkeep
--rw-r--r--   0        0        0      821 2024-03-21 09:38:59.632781 allianceauth-4.0.1/allianceauth/project_template/manage.py
--rw-r--r--   0        0        0       38 2024-03-21 09:38:59.632781 allianceauth-4.0.1/allianceauth/project_template/project_name/__init__.py
--rw-r--r--   0        0        0     1417 2024-03-21 09:38:59.633781 allianceauth-4.0.1/allianceauth/project_template/project_name/celery.py
--rw-r--r--   0        0        0        0 2024-03-21 09:38:59.742780 allianceauth-4.0.1/allianceauth/project_template/project_name/settings/__init__.py
--rw-r--r--   0        0        0     9147 2024-03-21 09:38:59.633781 allianceauth-4.0.1/allianceauth/project_template/project_name/settings/base.py
--rw-r--r--   0        0        0     3260 2024-03-21 09:38:59.633781 allianceauth-4.0.1/allianceauth/project_template/project_name/settings/local.py
--rw-r--r--   0        0        0        0 2024-03-21 09:38:59.742780 allianceauth-4.0.1/allianceauth/project_template/project_name/static/.gitkeep
--rw-r--r--   0        0        0        0 2024-03-21 09:38:59.742780 allianceauth-4.0.1/allianceauth/project_template/project_name/templates/.gitkeep
--rw-r--r--   0        0        0      329 2024-03-21 09:38:59.633781 allianceauth-4.0.1/allianceauth/project_template/project_name/urls.py
--rw-r--r--   0        0        0      432 2024-03-21 09:38:59.633781 allianceauth-4.0.1/allianceauth/project_template/project_name/wsgi.py
--rw-r--r--   0        0        0     1408 2024-03-21 09:38:59.633781 allianceauth-4.0.1/allianceauth/project_template/supervisor.conf
--rw-r--r--   0        0        0        0 2024-03-21 09:38:59.743780 allianceauth-4.0.1/allianceauth/services/__init__.py
--rw-r--r--   0        0        0     3954 2024-03-21 09:38:59.633781 allianceauth-4.0.1/allianceauth/services/abstract.py
--rw-r--r--   0        0        0     2162 2024-03-21 09:38:59.633781 allianceauth-4.0.1/allianceauth/services/admin.py
--rw-r--r--   0        0        0      179 2024-03-21 09:38:59.633781 allianceauth-4.0.1/allianceauth/services/apps.py
--rw-r--r--   0        0        0      662 2024-03-21 09:38:59.633781 allianceauth-4.0.1/allianceauth/services/auth_hooks.py
--rw-r--r--   0        0        0     2117 2024-03-21 09:38:59.633781 allianceauth-4.0.1/allianceauth/services/forms.py
--rw-r--r--   0        0        0     9149 2024-03-21 09:38:59.633781 allianceauth-4.0.1/allianceauth/services/hooks.py
--rw-r--r--   0        0        0        0 2024-03-21 09:38:59.743780 allianceauth-4.0.1/allianceauth/services/management/__init__.py
--rw-r--r--   0        0        0        0 2024-03-21 09:38:59.743780 allianceauth-4.0.1/allianceauth/services/management/commands/__init__.py
--rw-r--r--   0        0        0      469 2024-03-21 09:38:59.634781 allianceauth-4.0.1/allianceauth/services/management/commands/verify_service_accounts.py
--rw-r--r--   0        0        0      483 2024-03-21 09:38:59.634781 allianceauth-4.0.1/allianceauth/services/migrations/0001_squashed_0003_delete_groupcache.py
--rw-r--r--   0        0        0     1220 2024-03-21 09:38:59.634781 allianceauth-4.0.1/allianceauth/services/migrations/0002_nameformatter.py
--rw-r--r--   0        0        0      522 2024-03-21 09:38:59.634781 allianceauth-4.0.1/allianceauth/services/migrations/0003_remove_broken_link.py
--rw-r--r--   0        0        0        0 2024-03-21 09:38:59.744780 allianceauth-4.0.1/allianceauth/services/migrations/__init__.py
--rw-r--r--   0        0        0     1000 2024-03-21 09:38:59.634781 allianceauth-4.0.1/allianceauth/services/models.py
--rw-r--r--   0        0        0        0 2024-03-21 09:38:59.744780 allianceauth-4.0.1/allianceauth/services/modules/__init__.py
--rw-r--r--   0        0        0       30 2024-03-21 09:38:59.634781 allianceauth-4.0.1/allianceauth/services/modules/discord/__init__.py
--rw-r--r--   0        0        0     1070 2024-03-21 09:38:59.634781 allianceauth-4.0.1/allianceauth/services/modules/discord/admin.py
--rw-r--r--   0        0        0     1290 2024-03-21 09:38:59.634781 allianceauth-4.0.1/allianceauth/services/modules/discord/api.py
--rw-r--r--   0        0        0     1062 2024-03-21 09:38:59.634781 allianceauth-4.0.1/allianceauth/services/modules/discord/app_settings.py
--rw-r--r--   0        0        0      148 2024-03-21 09:38:59.634781 allianceauth-4.0.1/allianceauth/services/modules/discord/apps.py
--rw-r--r--   0        0        0     5974 2024-03-21 09:38:59.634781 allianceauth-4.0.1/allianceauth/services/modules/discord/auth_hooks.py
--rw-r--r--   0        0        0     4446 2024-03-21 09:38:59.634781 allianceauth-4.0.1/allianceauth/services/modules/discord/core.py
--rw-r--r--   0        0        0      372 2024-03-21 09:38:59.634781 allianceauth-4.0.1/allianceauth/services/modules/discord/discord_client/__init__.py
--rw-r--r--   0        0        0     1681 2024-03-21 09:38:59.634781 allianceauth-4.0.1/allianceauth/services/modules/discord/discord_client/app_settings.py
--rw-r--r--   0        0        0    28997 2024-03-21 09:38:59.634781 allianceauth-4.0.1/allianceauth/services/modules/discord/discord_client/client.py
--rw-r--r--   0        0        0     1009 2024-03-21 09:38:59.634781 allianceauth-4.0.1/allianceauth/services/modules/discord/discord_client/exceptions.py
--rw-r--r--   0        0        0     4590 2024-03-21 09:38:59.635781 allianceauth-4.0.1/allianceauth/services/modules/discord/discord_client/helpers.py
--rw-r--r--   0        0        0     3853 2024-03-21 09:38:59.635781 allianceauth-4.0.1/allianceauth/services/modules/discord/discord_client/models.py
--rw-r--r--   0        0        0        0 2024-03-21 09:38:59.745780 allianceauth-4.0.1/allianceauth/services/modules/discord/discord_client/tests/__init__.py
--rw-r--r--   0        0        0     5027 2024-03-21 09:38:59.635781 allianceauth-4.0.1/allianceauth/services/modules/discord/discord_client/tests/example_objects.json
--rw-r--r--   0        0        0     3013 2024-03-21 09:38:59.635781 allianceauth-4.0.1/allianceauth/services/modules/discord/discord_client/tests/factories.py
--rw-r--r--   0        0        0     2784 2024-03-21 09:38:59.635781 allianceauth-4.0.1/allianceauth/services/modules/discord/discord_client/tests/piloting_concurrency.py
--rw-r--r--   0        0        0     4477 2024-03-21 09:38:59.635781 allianceauth-4.0.1/allianceauth/services/modules/discord/discord_client/tests/piloting_functionality.py
--rw-r--r--   0        0        0      904 2024-03-21 09:38:59.635781 allianceauth-4.0.1/allianceauth/services/modules/discord/discord_client/tests/rate_limits.md
--rw-r--r--   0        0        0    56114 2024-03-21 09:38:59.635781 allianceauth-4.0.1/allianceauth/services/modules/discord/discord_client/tests/test_client.py
--rw-r--r--   0        0        0     1045 2024-03-21 09:38:59.635781 allianceauth-4.0.1/allianceauth/services/modules/discord/discord_client/tests/test_exceptions.py
--rw-r--r--   0        0        0     9724 2024-03-21 09:38:59.635781 allianceauth-4.0.1/allianceauth/services/modules/discord/discord_client/tests/test_helpers.py
--rw-r--r--   0        0        0     4966 2024-03-21 09:38:59.635781 allianceauth-4.0.1/allianceauth/services/modules/discord/discord_client/tests/test_models.py
--rw-r--r--   0        0        0     6281 2024-03-21 09:38:59.635781 allianceauth-4.0.1/allianceauth/services/modules/discord/managers.py
--rw-r--r--   0        0        0      680 2024-03-21 09:38:59.635781 allianceauth-4.0.1/allianceauth/services/modules/discord/migrations/0001_initial.py
--rw-r--r--   0        0        0     2067 2024-03-21 09:38:59.635781 allianceauth-4.0.1/allianceauth/services/modules/discord/migrations/0002_service_permissions.py
--rw-r--r--   0        0        0     1538 2024-03-21 09:38:59.635781 allianceauth-4.0.1/allianceauth/services/modules/discord/migrations/0003_big_overhaul.py
--rw-r--r--   0        0        0        0 2024-03-21 09:38:59.745780 allianceauth-4.0.1/allianceauth/services/modules/discord/migrations/__init__.py
--rw-r--r--   0        0        0     7138 2024-03-21 09:38:59.636781 allianceauth-4.0.1/allianceauth/services/modules/discord/models.py
--rw-r--r--   0        0        0     9517 2024-03-21 09:38:59.636781 allianceauth-4.0.1/allianceauth/services/modules/discord/tasks.py
--rw-r--r--   0        0        0     1508 2024-03-21 09:38:59.636781 allianceauth-4.0.1/allianceauth/services/modules/discord/templates/services/discord/discord_service_ctrl.html
--rw-r--r--   0        0        0      480 2024-03-21 09:38:59.636781 allianceauth-4.0.1/allianceauth/services/modules/discord/tests/__init__.py
--rw-r--r--   0        0        0      917 2024-03-21 09:38:59.636781 allianceauth-4.0.1/allianceauth/services/modules/discord/tests/factories.py
--rw-r--r--   0        0        0     2639 2024-03-21 09:38:59.636781 allianceauth-4.0.1/allianceauth/services/modules/discord/tests/piloting_tasks.py
--rw-r--r--   0        0        0    10400 2024-03-21 09:38:59.636781 allianceauth-4.0.1/allianceauth/services/modules/discord/tests/test_admin.py
--rw-r--r--   0        0        0      525 2024-03-21 09:38:59.636781 allianceauth-4.0.1/allianceauth/services/modules/discord/tests/test_api.py
--rw-r--r--   0        0        0     7200 2024-03-21 09:38:59.636781 allianceauth-4.0.1/allianceauth/services/modules/discord/tests/test_auth_hooks.py
--rw-r--r--   0        0        0     8456 2024-03-21 09:38:59.636781 allianceauth-4.0.1/allianceauth/services/modules/discord/tests/test_core.py
--rw-r--r--   0        0        0    29715 2024-03-21 09:38:59.636781 allianceauth-4.0.1/allianceauth/services/modules/discord/tests/test_integration.py
--rw-r--r--   0        0        0    19956 2024-03-21 09:38:59.636781 allianceauth-4.0.1/allianceauth/services/modules/discord/tests/test_managers.py
--rw-r--r--   0        0        0    11474 2024-03-21 09:38:59.637781 allianceauth-4.0.1/allianceauth/services/modules/discord/tests/test_models.py
--rw-r--r--   0        0        0    17995 2024-03-21 09:38:59.637781 allianceauth-4.0.1/allianceauth/services/modules/discord/tests/test_tasks.py
--rw-r--r--   0        0        0     3201 2024-03-21 09:38:59.637781 allianceauth-4.0.1/allianceauth/services/modules/discord/tests/test_utils.py
--rw-r--r--   0        0        0     6783 2024-03-21 09:38:59.637781 allianceauth-4.0.1/allianceauth/services/modules/discord/tests/test_views.py
--rw-r--r--   0        0        0      538 2024-03-21 09:38:59.637781 allianceauth-4.0.1/allianceauth/services/modules/discord/urls.py
--rw-r--r--   0        0        0     2561 2024-03-21 09:38:59.637781 allianceauth-4.0.1/allianceauth/services/modules/discord/utils.py
--rw-r--r--   0        0        0     3635 2024-03-21 09:38:59.637781 allianceauth-4.0.1/allianceauth/services/modules/discord/views.py
--rw-r--r--   0        0        0        0 2024-03-21 09:38:59.746780 allianceauth-4.0.1/allianceauth/services/modules/discourse/__init__.py
--rw-r--r--   0        0        0      264 2024-03-21 09:38:59.637781 allianceauth-4.0.1/allianceauth/services/modules/discourse/admin.py
--rw-r--r--   0        0        0      154 2024-03-21 09:38:59.637781 allianceauth-4.0.1/allianceauth/services/modules/discourse/apps.py
--rw-r--r--   0        0        0     1878 2024-03-21 09:38:59.637781 allianceauth-4.0.1/allianceauth/services/modules/discourse/auth_hooks.py
--rw-r--r--   0        0        0     7039 2024-03-21 09:38:59.637781 allianceauth-4.0.1/allianceauth/services/modules/discourse/manager.py
--rw-r--r--   0        0        0      677 2024-03-21 09:38:59.637781 allianceauth-4.0.1/allianceauth/services/modules/discourse/migrations/0001_initial.py
--rw-r--r--   0        0        0     2096 2024-03-21 09:38:59.637781 allianceauth-4.0.1/allianceauth/services/modules/discourse/migrations/0002_service_permissions.py
--rw-r--r--   0        0        0        0 2024-03-21 09:38:59.747780 allianceauth-4.0.1/allianceauth/services/modules/discourse/migrations/__init__.py
--rw-r--r--   0        0        0      529 2024-03-21 09:38:59.637781 allianceauth-4.0.1/allianceauth/services/modules/discourse/models.py
--rw-r--r--   0        0        0      533 2024-03-21 09:38:59.637781 allianceauth-4.0.1/allianceauth/services/modules/discourse/providers.py
--rw-r--r--   0        0        0     2276 2024-03-21 09:38:59.637781 allianceauth-4.0.1/allianceauth/services/modules/discourse/tasks.py
--rw-r--r--   0        0        0      663 2024-03-21 09:38:59.638781 allianceauth-4.0.1/allianceauth/services/modules/discourse/templates/services/discourse/discourse_service_ctrl.html
--rw-r--r--   0        0        0     5209 2024-03-21 09:38:59.638781 allianceauth-4.0.1/allianceauth/services/modules/discourse/tests.py
--rw-r--r--   0        0        0      176 2024-03-21 09:38:59.638781 allianceauth-4.0.1/allianceauth/services/modules/discourse/urls.py
--rw-r--r--   0        0        0     3486 2024-03-21 09:38:59.638781 allianceauth-4.0.1/allianceauth/services/modules/discourse/views.py
--rw-r--r--   0        0        0        0 2024-03-21 09:38:59.747780 allianceauth-4.0.1/allianceauth/services/modules/example/__init__.py
--rw-r--r--   0        0        0      156 2024-03-21 09:38:59.638781 allianceauth-4.0.1/allianceauth/services/modules/example/apps.py
--rw-r--r--   0        0        0     1336 2024-03-21 09:38:59.638781 allianceauth-4.0.1/allianceauth/services/modules/example/auth_hooks.py
--rw-r--r--   0        0        0      411 2024-03-21 09:38:59.638781 allianceauth-4.0.1/allianceauth/services/modules/example/models.py
--rw-r--r--   0        0        0      206 2024-03-21 09:38:59.638781 allianceauth-4.0.1/allianceauth/services/modules/example/urls.py
--rw-r--r--   0        0        0       22 2024-03-21 09:38:59.638781 allianceauth-4.0.1/allianceauth/services/modules/example/views.py
--rw-r--r--   0        0        0        0 2024-03-21 09:38:59.748780 allianceauth-4.0.1/allianceauth/services/modules/ips4/__init__.py
--rw-r--r--   0        0        0      240 2024-03-21 09:38:59.638781 allianceauth-4.0.1/allianceauth/services/modules/ips4/admin.py
--rw-r--r--   0        0        0      139 2024-03-21 09:38:59.638781 allianceauth-4.0.1/allianceauth/services/modules/ips4/apps.py
--rw-r--r--   0        0        0     1554 2024-03-21 09:38:59.638781 allianceauth-4.0.1/allianceauth/services/modules/ips4/auth_hooks.py
--rw-r--r--   0        0        0     4199 2024-03-21 09:38:59.638781 allianceauth-4.0.1/allianceauth/services/modules/ips4/manager.py
--rw-r--r--   0        0        0      737 2024-03-21 09:38:59.639781 allianceauth-4.0.1/allianceauth/services/modules/ips4/migrations/0001_initial.py
--rw-r--r--   0        0        0     2025 2024-03-21 09:38:59.639781 allianceauth-4.0.1/allianceauth/services/modules/ips4/migrations/0002_service_permissions.py
--rw-r--r--   0        0        0        0 2024-03-21 09:38:59.749780 allianceauth-4.0.1/allianceauth/services/modules/ips4/migrations/__init__.py
--rw-r--r--   0        0        0      558 2024-03-21 09:38:59.639781 allianceauth-4.0.1/allianceauth/services/modules/ips4/models.py
--rw-r--r--   0        0        0     1104 2024-03-21 09:38:59.639781 allianceauth-4.0.1/allianceauth/services/modules/ips4/tasks.py
--rw-r--r--   0        0        0     6035 2024-03-21 09:38:59.639781 allianceauth-4.0.1/allianceauth/services/modules/ips4/tests.py
--rw-r--r--   0        0        0      495 2024-03-21 09:38:59.639781 allianceauth-4.0.1/allianceauth/services/modules/ips4/urls.py
--rw-r--r--   0        0        0     4825 2024-03-21 09:38:59.639781 allianceauth-4.0.1/allianceauth/services/modules/ips4/views.py
--rw-r--r--   0        0        0        0 2024-03-21 09:38:59.749780 allianceauth-4.0.1/allianceauth/services/modules/mumble/__init__.py
--rw-r--r--   0        0        0      455 2024-03-21 09:38:59.639781 allianceauth-4.0.1/allianceauth/services/modules/mumble/admin.py
--rw-r--r--   0        0        0      145 2024-03-21 09:38:59.639781 allianceauth-4.0.1/allianceauth/services/modules/mumble/apps.py
--rw-r--r--   0        0        0     2958 2024-03-21 09:38:59.639781 allianceauth-4.0.1/allianceauth/services/modules/mumble/auth_hooks.py
--rw-r--r--   0        0        0      726 2024-03-21 09:38:59.639781 allianceauth-4.0.1/allianceauth/services/modules/mumble/migrations/0001_initial.py
--rw-r--r--   0        0        0     2868 2024-03-21 09:38:59.639781 allianceauth-4.0.1/allianceauth/services/modules/mumble/migrations/0001_squashed_0011_auto_20201011_1009.py
--rw-r--r--   0        0        0      316 2024-03-21 09:38:59.639781 allianceauth-4.0.1/allianceauth/services/modules/mumble/migrations/0002_auto_20161212_0100.py
--rw-r--r--   0        0        0      613 2024-03-21 09:38:59.639781 allianceauth-4.0.1/allianceauth/services/modules/mumble/migrations/0003_mumbleuser_user.py
--rw-r--r--   0        0        0      548 2024-03-21 09:38:59.639781 allianceauth-4.0.1/allianceauth/services/modules/mumble/migrations/0004_auto_20161214_1024.py
--rw-r--r--   0        0        0      561 2024-03-21 09:38:59.639781 allianceauth-4.0.1/allianceauth/services/modules/mumble/migrations/0005_mumbleuser_hashfn.py
--rw-r--r--   0        0        0     2063 2024-03-21 09:38:59.639781 allianceauth-4.0.1/allianceauth/services/modules/mumble/migrations/0006_service_permissions.py
--rw-r--r--   0        0        0      679 2024-03-21 09:38:59.639781 allianceauth-4.0.1/allianceauth/services/modules/mumble/migrations/0007_not_null_user.py
--rw-r--r--   0        0        0      398 2024-03-21 09:38:59.639781 allianceauth-4.0.1/allianceauth/services/modules/mumble/migrations/0008_mumbleuser_display_name.py
--rw-r--r--   0        0        0     1181 2024-03-21 09:38:59.639781 allianceauth-4.0.1/allianceauth/services/modules/mumble/migrations/0009_set_mumble_dissplay_names.py
--rw-r--r--   0        0        0      554 2024-03-21 09:38:59.639781 allianceauth-4.0.1/allianceauth/services/modules/mumble/migrations/0010_mumbleuser_certhash.py
--rw-r--r--   0        0        0      390 2024-03-21 09:38:59.639781 allianceauth-4.0.1/allianceauth/services/modules/mumble/migrations/0011_auto_20201011_1009.py
--rw-r--r--   0        0        0     1508 2024-03-21 09:38:59.640781 allianceauth-4.0.1/allianceauth/services/modules/mumble/migrations/0012_mumble_client_info.py
--rw-r--r--   0        0        0        0 2024-03-21 09:38:59.757780 allianceauth-4.0.1/allianceauth/services/modules/mumble/migrations/__init__.py
--rw-r--r--   0        0        0     5630 2024-03-21 09:38:59.640781 allianceauth-4.0.1/allianceauth/services/modules/mumble/models.py
--rw-r--r--   0        0        0     3142 2024-03-21 09:38:59.640781 allianceauth-4.0.1/allianceauth/services/modules/mumble/tasks.py
--rw-r--r--   0        0        0     1655 2024-03-21 09:38:59.640781 allianceauth-4.0.1/allianceauth/services/modules/mumble/templates/services/mumble/mumble_service_ctrl.html
--rw-r--r--   0        0        0     8632 2024-03-21 09:38:59.640781 allianceauth-4.0.1/allianceauth/services/modules/mumble/tests.py
--rw-r--r--   0        0        0      560 2024-03-21 09:38:59.640781 allianceauth-4.0.1/allianceauth/services/modules/mumble/urls.py
--rw-r--r--   0        0        0      994 2024-03-21 09:38:59.640781 allianceauth-4.0.1/allianceauth/services/modules/mumble/views.py
--rw-r--r--   0        0        0        0 2024-03-21 09:38:59.757780 allianceauth-4.0.1/allianceauth/services/modules/openfire/__init__.py
--rw-r--r--   0        0        0      317 2024-03-21 09:38:59.640781 allianceauth-4.0.1/allianceauth/services/modules/openfire/admin.py
--rw-r--r--   0        0        0      151 2024-03-21 09:38:59.640781 allianceauth-4.0.1/allianceauth/services/modules/openfire/apps.py
--rw-r--r--   0        0        0     3648 2024-03-21 09:38:59.640781 allianceauth-4.0.1/allianceauth/services/modules/openfire/auth_hooks.py
--rw-r--r--   0        0        0      263 2024-03-21 09:38:59.640781 allianceauth-4.0.1/allianceauth/services/modules/openfire/forms.py
--rw-r--r--   0        0        0     8321 2024-03-21 09:38:59.640781 allianceauth-4.0.1/allianceauth/services/modules/openfire/manager.py
--rw-r--r--   0        0        0      687 2024-03-21 09:38:59.640781 allianceauth-4.0.1/allianceauth/services/modules/openfire/migrations/0001_initial.py
--rw-r--r--   0        0        0     2073 2024-03-21 09:38:59.640781 allianceauth-4.0.1/allianceauth/services/modules/openfire/migrations/0002_service_permissions.py
--rw-r--r--   0        0        0        0 2024-03-21 09:38:59.757780 allianceauth-4.0.1/allianceauth/services/modules/openfire/migrations/__init__.py
--rw-r--r--   0        0        0      495 2024-03-21 09:38:59.640781 allianceauth-4.0.1/allianceauth/services/modules/openfire/models.py
--rw-r--r--   0        0        0     2620 2024-03-21 09:38:59.640781 allianceauth-4.0.1/allianceauth/services/modules/openfire/tasks.py
--rw-r--r--   0        0        0     1533 2024-03-21 09:38:59.641781 allianceauth-4.0.1/allianceauth/services/modules/openfire/templates/services/openfire/broadcast.html
--rw-r--r--   0        0        0     9478 2024-03-21 09:38:59.641781 allianceauth-4.0.1/allianceauth/services/modules/openfire/tests.py
--rw-r--r--   0        0        0      585 2024-03-21 09:38:59.641781 allianceauth-4.0.1/allianceauth/services/modules/openfire/urls.py
--rw-r--r--   0        0        0     7688 2024-03-21 09:38:59.641781 allianceauth-4.0.1/allianceauth/services/modules/openfire/views.py
--rw-r--r--   0        0        0        0 2024-03-21 09:38:59.757780 allianceauth-4.0.1/allianceauth/services/modules/phpbb3/__init__.py
--rw-r--r--   0        0        0      310 2024-03-21 09:38:59.641781 allianceauth-4.0.1/allianceauth/services/modules/phpbb3/admin.py
--rw-r--r--   0        0        0      145 2024-03-21 09:38:59.641781 allianceauth-4.0.1/allianceauth/services/modules/phpbb3/apps.py
--rw-r--r--   0        0        0     2196 2024-03-21 09:38:59.641781 allianceauth-4.0.1/allianceauth/services/modules/phpbb3/auth_hooks.py
--rw-r--r--   0        0        0    13459 2024-03-21 09:38:59.641781 allianceauth-4.0.1/allianceauth/services/modules/phpbb3/manager.py
--rw-r--r--   0        0        0      683 2024-03-21 09:38:59.641781 allianceauth-4.0.1/allianceauth/services/modules/phpbb3/migrations/0001_initial.py
--rw-r--r--   0        0        0     2049 2024-03-21 09:38:59.641781 allianceauth-4.0.1/allianceauth/services/modules/phpbb3/migrations/0002_service_permissions.py
--rw-r--r--   0        0        0        0 2024-03-21 09:38:59.758780 allianceauth-4.0.1/allianceauth/services/modules/phpbb3/migrations/__init__.py
--rw-r--r--   0        0        0      487 2024-03-21 09:38:59.641781 allianceauth-4.0.1/allianceauth/services/modules/phpbb3/models.py
--rw-r--r--   0        0        0     2478 2024-03-21 09:38:59.641781 allianceauth-4.0.1/allianceauth/services/modules/phpbb3/tasks.py
--rw-r--r--   0        0        0     8189 2024-03-21 09:38:59.641781 allianceauth-4.0.1/allianceauth/services/modules/phpbb3/tests.py
--rw-r--r--   0        0        0      504 2024-03-21 09:38:59.641781 allianceauth-4.0.1/allianceauth/services/modules/phpbb3/urls.py
--rw-r--r--   0        0        0     5139 2024-03-21 09:38:59.641781 allianceauth-4.0.1/allianceauth/services/modules/phpbb3/views.py
--rw-r--r--   0        0        0        0 2024-03-21 09:38:59.758780 allianceauth-4.0.1/allianceauth/services/modules/smf/__init__.py
--rw-r--r--   0        0        0      302 2024-03-21 09:38:59.641781 allianceauth-4.0.1/allianceauth/services/modules/smf/admin.py
--rw-r--r--   0        0        0      136 2024-03-21 09:38:59.641781 allianceauth-4.0.1/allianceauth/services/modules/smf/apps.py
--rw-r--r--   0        0        0     2408 2024-03-21 09:38:59.641781 allianceauth-4.0.1/allianceauth/services/modules/smf/auth_hooks.py
--rw-r--r--   0        0        0    14780 2024-03-21 09:38:59.641781 allianceauth-4.0.1/allianceauth/services/modules/smf/manager.py
--rw-r--r--   0        0        0      677 2024-03-21 09:38:59.642781 allianceauth-4.0.1/allianceauth/services/modules/smf/migrations/0001_initial.py
--rw-r--r--   0        0        0     2011 2024-03-21 09:38:59.642781 allianceauth-4.0.1/allianceauth/services/modules/smf/migrations/0002_service_permissions.py
--rw-r--r--   0        0        0      694 2024-03-21 09:38:59.642781 allianceauth-4.0.1/allianceauth/services/modules/smf/migrations/0003_set_smf_displayed_names.py
--rw-r--r--   0        0        0        0 2024-03-21 09:38:59.761780 allianceauth-4.0.1/allianceauth/services/modules/smf/migrations/__init__.py
--rw-r--r--   0        0        0      475 2024-03-21 09:38:59.642781 allianceauth-4.0.1/allianceauth/services/modules/smf/models.py
--rw-r--r--   0        0        0     3740 2024-03-21 09:38:59.642781 allianceauth-4.0.1/allianceauth/services/modules/smf/tasks.py
--rw-r--r--   0        0        0     8057 2024-03-21 09:38:59.642781 allianceauth-4.0.1/allianceauth/services/modules/smf/tests.py
--rw-r--r--   0        0        0      489 2024-03-21 09:38:59.642781 allianceauth-4.0.1/allianceauth/services/modules/smf/urls.py
--rw-r--r--   0        0        0     5143 2024-03-21 09:38:59.642781 allianceauth-4.0.1/allianceauth/services/modules/smf/views.py
--rw-r--r--   0        0        0        0 2024-03-21 09:38:59.761780 allianceauth-4.0.1/allianceauth/services/modules/teamspeak3/__init__.py
--rw-r--r--   0        0        0     1872 2024-03-21 09:38:59.642781 allianceauth-4.0.1/allianceauth/services/modules/teamspeak3/admin.py
--rw-r--r--   0        0        0      209 2024-03-21 09:38:59.642781 allianceauth-4.0.1/allianceauth/services/modules/teamspeak3/apps.py
--rw-r--r--   0        0        0     2128 2024-03-21 09:38:59.642781 allianceauth-4.0.1/allianceauth/services/modules/teamspeak3/auth_hooks.py
--rw-r--r--   0        0        0      500 2024-03-21 09:38:59.642781 allianceauth-4.0.1/allianceauth/services/modules/teamspeak3/forms.py
--rw-r--r--   0        0        0    12601 2024-03-21 09:38:59.642781 allianceauth-4.0.1/allianceauth/services/modules/teamspeak3/manager.py
--rw-r--r--   0        0        0     1995 2024-03-21 09:38:59.642781 allianceauth-4.0.1/allianceauth/services/modules/teamspeak3/migrations/0001_initial.py
--rw-r--r--   0        0        0      538 2024-03-21 09:38:59.642781 allianceauth-4.0.1/allianceauth/services/modules/teamspeak3/migrations/0002_auto_20161212_0133.py
--rw-r--r--   0        0        0      781 2024-03-21 09:38:59.642781 allianceauth-4.0.1/allianceauth/services/modules/teamspeak3/migrations/0003_teamspeak3user.py
--rw-r--r--   0        0        0     2116 2024-03-21 09:38:59.642781 allianceauth-4.0.1/allianceauth/services/modules/teamspeak3/migrations/0004_service_permissions.py
--rw-r--r--   0        0        0      784 2024-03-21 09:38:59.642781 allianceauth-4.0.1/allianceauth/services/modules/teamspeak3/migrations/0005_stategroup.py
--rw-r--r--   0        0        0        0 2024-03-21 09:38:59.762780 allianceauth-4.0.1/allianceauth/services/modules/teamspeak3/migrations/__init__.py
--rw-r--r--   0        0        0     1567 2024-03-21 09:38:59.642781 allianceauth-4.0.1/allianceauth/services/modules/teamspeak3/models.py
--rw-r--r--   0        0        0     1723 2024-03-21 09:38:59.642781 allianceauth-4.0.1/allianceauth/services/modules/teamspeak3/signals.py
--rw-r--r--   0        0        0     3780 2024-03-21 09:38:59.643781 allianceauth-4.0.1/allianceauth/services/modules/teamspeak3/tasks.py
--rw-r--r--   0        0        0      296 2024-03-21 09:38:59.643781 allianceauth-4.0.1/allianceauth/services/modules/teamspeak3/templates/admin/teamspeak3/authts/change_list.html
--rw-r--r--   0        0        0     1472 2024-03-21 09:38:59.643781 allianceauth-4.0.1/allianceauth/services/modules/teamspeak3/templates/services/teamspeak3/teamspeak3_service_ctrl.html
--rw-r--r--   0        0        0     1121 2024-03-21 09:38:59.643781 allianceauth-4.0.1/allianceauth/services/modules/teamspeak3/templates/services/teamspeak3/teamspeakjoin.html
--rw-r--r--   0        0        0    21498 2024-03-21 09:38:59.643781 allianceauth-4.0.1/allianceauth/services/modules/teamspeak3/tests.py
--rw-r--r--   0        0        0      661 2024-03-21 09:38:59.643781 allianceauth-4.0.1/allianceauth/services/modules/teamspeak3/urls.py
--rw-r--r--   0        0        0       23 2024-03-21 09:38:59.643781 allianceauth-4.0.1/allianceauth/services/modules/teamspeak3/util/__init__.py
--rw-r--r--   0        0        0    15106 2024-03-21 09:38:59.643781 allianceauth-4.0.1/allianceauth/services/modules/teamspeak3/util/ts3.py
--rw-r--r--   0        0        0     5138 2024-03-21 09:38:59.643781 allianceauth-4.0.1/allianceauth/services/modules/teamspeak3/views.py
--rw-r--r--   0        0        0        0 2024-03-21 09:38:59.762780 allianceauth-4.0.1/allianceauth/services/modules/xenforo/__init__.py
--rw-r--r--   0        0        0      314 2024-03-21 09:38:59.643781 allianceauth-4.0.1/allianceauth/services/modules/xenforo/admin.py
--rw-r--r--   0        0        0      148 2024-03-21 09:38:59.643781 allianceauth-4.0.1/allianceauth/services/modules/xenforo/apps.py
--rw-r--r--   0        0        0     1779 2024-03-21 09:38:59.644781 allianceauth-4.0.1/allianceauth/services/modules/xenforo/auth_hooks.py
--rw-r--r--   0        0        0     3685 2024-03-21 09:38:59.644781 allianceauth-4.0.1/allianceauth/services/modules/xenforo/manager.py
--rw-r--r--   0        0        0      685 2024-03-21 09:38:59.644781 allianceauth-4.0.1/allianceauth/services/modules/xenforo/migrations/0001_initial.py
--rw-r--r--   0        0        0     2067 2024-03-21 09:38:59.644781 allianceauth-4.0.1/allianceauth/services/modules/xenforo/migrations/0002_service_permissions.py
--rw-r--r--   0        0        0        0 2024-03-21 09:38:59.763780 allianceauth-4.0.1/allianceauth/services/modules/xenforo/migrations/__init__.py
--rw-r--r--   0        0        0      491 2024-03-21 09:38:59.644781 allianceauth-4.0.1/allianceauth/services/modules/xenforo/models.py
--rw-r--r--   0        0        0     1268 2024-03-21 09:38:59.644781 allianceauth-4.0.1/allianceauth/services/modules/xenforo/tasks.py
--rw-r--r--   0        0        0     7153 2024-03-21 09:38:59.644781 allianceauth-4.0.1/allianceauth/services/modules/xenforo/tests.py
--rw-r--r--   0        0        0      529 2024-03-21 09:38:59.644781 allianceauth-4.0.1/allianceauth/services/modules/xenforo/urls.py
--rw-r--r--   0        0        0     4821 2024-03-21 09:38:59.644781 allianceauth-4.0.1/allianceauth/services/modules/xenforo/views.py
--rw-r--r--   0        0        0    10087 2024-03-21 09:38:59.644781 allianceauth-4.0.1/allianceauth/services/signals.py
--rw-r--r--   0        0        0      126 2024-03-21 09:38:59.644781 allianceauth-4.0.1/allianceauth/services/static/allianceauth/services/admin.css
--rw-r--r--   0        0        0     1937 2024-03-21 09:38:59.644781 allianceauth-4.0.1/allianceauth/services/tasks.py
--rw-r--r--   0        0        0       57 2024-03-21 09:38:59.644781 allianceauth-4.0.1/allianceauth/services/templates/public/menublock.html
--rw-r--r--   0        0        0      335 2024-03-21 09:38:59.644781 allianceauth-4.0.1/allianceauth/services/templates/public/menuitem.html
--rw-r--r--   0        0        0     1566 2024-03-21 09:38:59.644781 allianceauth-4.0.1/allianceauth/services/templates/services/fleetformattertool.html
--rw-r--r--   0        0        0     1232 2024-03-21 09:38:59.644781 allianceauth-4.0.1/allianceauth/services/templates/services/service_confirm_delete.html
--rw-r--r--   0        0        0     1285 2024-03-21 09:38:59.644781 allianceauth-4.0.1/allianceauth/services/templates/services/service_credentials.html
--rw-r--r--   0        0        0     1147 2024-03-21 09:38:59.645781 allianceauth-4.0.1/allianceauth/services/templates/services/service_password.html
--rw-r--r--   0        0        0      239 2024-03-21 09:38:59.645781 allianceauth-4.0.1/allianceauth/services/templates/services/service_status.html
--rw-r--r--   0        0        0      100 2024-03-21 09:38:59.645781 allianceauth-4.0.1/allianceauth/services/templates/services/service_username.html
--rw-r--r--   0        0        0     2422 2024-03-21 09:38:59.645781 allianceauth-4.0.1/allianceauth/services/templates/services/services.html
--rw-r--r--   0        0        0     1233 2024-03-21 09:38:59.645781 allianceauth-4.0.1/allianceauth/services/templates/services/services_ctrl.html
--rw-r--r--   0        0        0      832 2024-03-21 09:38:59.645781 allianceauth-4.0.1/allianceauth/services/templates/services/services_ctrl_base.html
--rw-r--r--   0        0        0        0 2024-03-21 09:38:59.764780 allianceauth-4.0.1/allianceauth/services/tests/__init__.py
--rw-r--r--   0        0        0     1048 2024-03-21 09:38:59.645781 allianceauth-4.0.1/allianceauth/services/tests/test_hooks.py
--rw-r--r--   0        0        0      514 2024-03-21 09:38:59.645781 allianceauth-4.0.1/allianceauth/services/tests/test_models.py
--rw-r--r--   0        0        0     4316 2024-03-21 09:38:59.645781 allianceauth-4.0.1/allianceauth/services/tests/test_nameformatter.py
--rw-r--r--   0        0        0    12299 2024-03-21 09:38:59.645781 allianceauth-4.0.1/allianceauth/services/tests/test_signals.py
--rw-r--r--   0        0        0     3248 2024-03-21 09:38:59.645781 allianceauth-4.0.1/allianceauth/services/tests/test_tasks.py
--rw-r--r--   0        0        0      530 2024-03-21 09:38:59.645781 allianceauth-4.0.1/allianceauth/services/urls.py
--rw-r--r--   0        0        0     2450 2024-03-21 09:38:59.645781 allianceauth-4.0.1/allianceauth/services/views.py
--rw-r--r--   0        0        0        0 2024-03-21 09:38:59.764780 allianceauth-4.0.1/allianceauth/srp/__init__.py
--rw-r--r--   0        0        0      205 2024-03-21 09:38:59.645781 allianceauth-4.0.1/allianceauth/srp/admin.py
--rw-r--r--   0        0        0      112 2024-03-21 09:38:59.645781 allianceauth-4.0.1/allianceauth/srp/apps.py
--rw-r--r--   0        0        0      960 2024-03-21 09:38:59.645781 allianceauth-4.0.1/allianceauth/srp/auth_hooks.py
--rw-r--r--   0        0        0     1724 2024-03-21 09:38:59.645781 allianceauth-4.0.1/allianceauth/srp/form.py
--rw-r--r--   0        0        0     1961 2024-03-21 09:38:59.646781 allianceauth-4.0.1/allianceauth/srp/managers.py
--rw-r--r--   0        0        0     2265 2024-03-21 09:38:59.646781 allianceauth-4.0.1/allianceauth/srp/migrations/0001_initial.py
--rw-r--r--   0        0        0      488 2024-03-21 09:38:59.646781 allianceauth-4.0.1/allianceauth/srp/migrations/0002_srpuserrequest_srp_status_choices.py
--rw-r--r--   0        0        0     2048 2024-03-21 09:38:59.646781 allianceauth-4.0.1/allianceauth/srp/migrations/0003_make_strings_more_stringy.py
--rw-r--r--   0        0        0      746 2024-03-21 09:38:59.646781 allianceauth-4.0.1/allianceauth/srp/migrations/0004_on_delete.py
--rw-r--r--   0        0        0        0 2024-03-21 09:38:59.765780 allianceauth-4.0.1/allianceauth/srp/migrations/__init__.py
--rw-r--r--   0        0        0     1991 2024-03-21 09:38:59.646781 allianceauth-4.0.1/allianceauth/srp/models.py
--rw-r--r--   0        0        0      388 2024-03-21 09:38:59.646781 allianceauth-4.0.1/allianceauth/srp/providers.py
--rw-r--r--   0        0        0    24877 2024-03-21 09:38:59.646781 allianceauth-4.0.1/allianceauth/srp/swagger.json
--rw-r--r--   0        0        0     2597 2024-03-21 09:38:59.646781 allianceauth-4.0.1/allianceauth/srp/templates/srp/add.html
--rw-r--r--   0        0        0    13408 2024-03-21 09:38:59.646781 allianceauth-4.0.1/allianceauth/srp/templates/srp/data.html
--rw-r--r--   0        0        0     6364 2024-03-21 09:38:59.646781 allianceauth-4.0.1/allianceauth/srp/templates/srp/management.html
--rw-r--r--   0        0        0     1432 2024-03-21 09:38:59.646781 allianceauth-4.0.1/allianceauth/srp/templates/srp/request.html
--rw-r--r--   0        0        0     1765 2024-03-21 09:38:59.646781 allianceauth-4.0.1/allianceauth/srp/templates/srp/update.html
--rw-r--r--   0        0        0        0 2024-03-21 09:38:59.765780 allianceauth-4.0.1/allianceauth/srp/tests/__init__.py
--rw-r--r--   0        0        0     3623 2024-03-21 09:38:59.646781 allianceauth-4.0.1/allianceauth/srp/tests/test_managers.py
--rw-r--r--   0        0        0    28605 2024-03-21 09:38:59.646781 allianceauth-4.0.1/allianceauth/srp/tests/testdata/get_killmails_killmail_id_killmail_hash_81973979.json
--rw-r--r--   0        0        0      363 2024-03-21 09:38:59.646781 allianceauth-4.0.1/allianceauth/srp/tests/testdata/zkillboard_killmail_api_81973979.json
--rw-r--r--   0        0        0     1342 2024-03-21 09:38:59.647781 allianceauth-4.0.1/allianceauth/srp/urls.py
--rw-r--r--   0        0        0    17762 2024-03-21 09:38:59.647781 allianceauth-4.0.1/allianceauth/srp/views.py
--rw-r--r--   0        0        0     4616 2024-03-21 09:38:59.647781 allianceauth-4.0.1/allianceauth/static/allianceauth/css/auth-base.css
--rw-r--r--   0        0        0     1173 2024-03-21 09:38:59.647781 allianceauth-4.0.1/allianceauth/static/allianceauth/css/checkbox.css
--rw-r--r--   0        0        0      865 2024-03-21 09:38:59.647781 allianceauth-4.0.1/allianceauth/static/allianceauth/css/themes/bootstrap-locals.less
--rw-r--r--   0        0        0     1078 2024-03-21 09:38:59.647781 allianceauth-4.0.1/allianceauth/static/allianceauth/css/themes/darkly/LICENSE
--rw-r--r--   0        0        0      624 2024-03-21 09:38:59.647781 allianceauth-4.0.1/allianceauth/static/allianceauth/css/themes/darkly/darkly.less
--rw-r--r--   0        0        0   122466 2024-03-21 09:38:59.648781 allianceauth-4.0.1/allianceauth/static/allianceauth/css/themes/darkly/darkly.min.css
--rw-r--r--   0        0        0      979 2024-03-21 09:38:59.648781 allianceauth-4.0.1/allianceauth/static/allianceauth/css/themes/flatly-shared.less
--rw-r--r--   0        0        0     1078 2024-03-21 09:38:59.648781 allianceauth-4.0.1/allianceauth/static/allianceauth/css/themes/flatly/LICENSE
--rw-r--r--   0        0        0      985 2024-03-21 09:38:59.648781 allianceauth-4.0.1/allianceauth/static/allianceauth/css/themes/flatly/flatly.less
--rw-r--r--   0        0        0   123138 2024-03-21 09:38:59.648781 allianceauth-4.0.1/allianceauth/static/allianceauth/css/themes/flatly/flatly.min.css
--rwxr-xr-x   0        0        0    21465 2024-03-21 09:38:59.648781 allianceauth-4.0.1/allianceauth/static/allianceauth/icons/allianceauth.png
--rw-r--r--   0        0        0     7686 2024-03-21 09:38:59.648781 allianceauth-4.0.1/allianceauth/static/allianceauth/icons/android-chrome-192x192.png
--rw-r--r--   0        0        0    26346 2024-03-21 09:38:59.648781 allianceauth-4.0.1/allianceauth/static/allianceauth/icons/android-chrome-512x512.png
--rw-r--r--   0        0        0     7160 2024-03-21 09:38:59.649781 allianceauth-4.0.1/allianceauth/static/allianceauth/icons/apple-touch-icon.png
--rw-r--r--   0        0        0      272 2024-03-21 09:38:59.649781 allianceauth-4.0.1/allianceauth/static/allianceauth/icons/browserconfig.xml
--rw-r--r--   0        0        0      941 2024-03-21 09:38:59.649781 allianceauth-4.0.1/allianceauth/static/allianceauth/icons/favicon-16x16.png
--rw-r--r--   0        0        0     1565 2024-03-21 09:38:59.649781 allianceauth-4.0.1/allianceauth/static/allianceauth/icons/favicon-32x32.png
--rwxr-xr-x   0        0        0     2180 2024-03-21 09:38:59.649781 allianceauth-4.0.1/allianceauth/static/allianceauth/icons/favicon-96x96.png
--rw-r--r--   0        0        0    15086 2024-03-21 09:38:59.649781 allianceauth-4.0.1/allianceauth/static/allianceauth/icons/favicon.ico
--rw-r--r--   0        0        0     4681 2024-03-21 09:38:59.649781 allianceauth-4.0.1/allianceauth/static/allianceauth/icons/mstile-150x150.png
--rw-r--r--   0        0        0     2590 2024-03-21 09:38:59.649781 allianceauth-4.0.1/allianceauth/static/allianceauth/icons/safari-pinned-tab.svg
--rw-r--r--   0        0        0      478 2024-03-21 09:38:59.649781 allianceauth-4.0.1/allianceauth/static/allianceauth/icons/site.webmanifest
--rw-r--r--   0        0        0    10836 2024-03-21 09:38:59.649781 allianceauth-4.0.1/allianceauth/static/allianceauth/images/auth-logo.png
--rw-r--r--   0        0        0     2278 2024-03-21 09:38:59.649781 allianceauth-4.0.1/allianceauth/static/allianceauth/images/auth-logo.svg
--rw-r--r--   0        0        0      573 2024-03-21 09:38:59.649781 allianceauth-4.0.1/allianceauth/static/allianceauth/js/eve-time.js
--rw-r--r--   0        0        0     1070 2024-03-21 09:38:59.649781 allianceauth-4.0.1/allianceauth/static/allianceauth/js/filterDropDown/LICENSE
--rw-r--r--   0        0        0    10422 2024-03-21 09:38:59.649781 allianceauth-4.0.1/allianceauth/static/allianceauth/js/filterDropDown/filterDropDown.js
--rw-r--r--   0        0        0     4205 2024-03-21 09:38:59.649781 allianceauth-4.0.1/allianceauth/static/allianceauth/js/filterDropDown/filterDropDown.min.js
--rw-r--r--   0        0        0     7090 2024-03-21 09:38:59.649781 allianceauth-4.0.1/allianceauth/static/allianceauth/js/jquery-ui/1.12.1/css/images/ui-icons_444444_256x240.png
--rw-r--r--   0        0        0     7074 2024-03-21 09:38:59.650781 allianceauth-4.0.1/allianceauth/static/allianceauth/js/jquery-ui/1.12.1/css/images/ui-icons_555555_256x240.png
--rw-r--r--   0        0        0     4618 2024-03-21 09:38:59.650781 allianceauth-4.0.1/allianceauth/static/allianceauth/js/jquery-ui/1.12.1/css/images/ui-icons_777620_256x240.png
--rw-r--r--   0        0        0     7111 2024-03-21 09:38:59.650781 allianceauth-4.0.1/allianceauth/static/allianceauth/js/jquery-ui/1.12.1/css/images/ui-icons_777777_256x240.png
--rw-r--r--   0        0        0     4618 2024-03-21 09:38:59.650781 allianceauth-4.0.1/allianceauth/static/allianceauth/js/jquery-ui/1.12.1/css/images/ui-icons_cc0000_256x240.png
--rw-r--r--   0        0        0     6487 2024-03-21 09:38:59.650781 allianceauth-4.0.1/allianceauth/static/allianceauth/js/jquery-ui/1.12.1/css/images/ui-icons_ffffff_256x240.png
--rw-r--r--   0        0        0    15830 2024-03-21 09:38:59.650781 allianceauth-4.0.1/allianceauth/static/allianceauth/js/jquery-ui/1.12.1/css/jquery-ui.min.css
--rw-r--r--   0        0        0     7142 2024-03-21 09:38:59.650781 allianceauth-4.0.1/allianceauth/static/allianceauth/js/jquery-ui/1.13.2/css/images/ui-icons_444444_256x240.png
--rw-r--r--   0        0        0     7126 2024-03-21 09:38:59.650781 allianceauth-4.0.1/allianceauth/static/allianceauth/js/jquery-ui/1.13.2/css/images/ui-icons_555555_256x240.png
--rw-r--r--   0        0        0     4670 2024-03-21 09:38:59.650781 allianceauth-4.0.1/allianceauth/static/allianceauth/js/jquery-ui/1.13.2/css/images/ui-icons_777620_256x240.png
--rw-r--r--   0        0        0     7163 2024-03-21 09:38:59.650781 allianceauth-4.0.1/allianceauth/static/allianceauth/js/jquery-ui/1.13.2/css/images/ui-icons_777777_256x240.png
--rw-r--r--   0        0        0     4670 2024-03-21 09:38:59.650781 allianceauth-4.0.1/allianceauth/static/allianceauth/js/jquery-ui/1.13.2/css/images/ui-icons_cc0000_256x240.png
--rw-r--r--   0        0        0     6539 2024-03-21 09:38:59.650781 allianceauth-4.0.1/allianceauth/static/allianceauth/js/jquery-ui/1.13.2/css/images/ui-icons_ffffff_256x240.png
--rw-r--r--   0        0        0    15842 2024-03-21 09:38:59.650781 allianceauth-4.0.1/allianceauth/static/allianceauth/js/jquery-ui/1.13.2/css/jquery-ui.min.css
--rw-r--r--   0        0        0     2391 2024-03-21 09:38:59.650781 allianceauth-4.0.1/allianceauth/static/allianceauth/js/refresh-notification-icon.js
--rw-r--r--   0        0        0     2636 2024-03-21 09:38:59.650781 allianceauth-4.0.1/allianceauth/static/allianceauth/js/refresh_notifications.js
--rw-r--r--   0        0        0     1170 2024-03-21 09:38:59.650781 allianceauth-4.0.1/allianceauth/static/allianceauth/js/timerboard.js
--rw-r--r--   0        0        0     1056 2024-03-21 09:38:59.650781 allianceauth-4.0.1/allianceauth/static/allianceauth/js/timers.js
--rw-r--r--   0        0        0       26 2024-03-21 09:38:59.650781 allianceauth-4.0.1/allianceauth/static/robots.txt
--rw-r--r--   0        0        0      119 2024-03-21 09:38:59.651781 allianceauth-4.0.1/allianceauth/templates/admin/base_site.html
--rw-r--r--   0        0        0      403 2024-03-21 09:38:59.651781 allianceauth-4.0.1/allianceauth/templates/allianceauth/admin-status/celery_bar_partial.html
--rw-r--r--   0        0        0     1282 2024-03-21 09:38:59.651781 allianceauth-4.0.1/allianceauth/templates/allianceauth/admin-status/esi_check.html
--rw-r--r--   0        0        0       47 2024-03-21 09:38:59.651781 allianceauth-4.0.1/allianceauth/templates/allianceauth/admin-status/include.html
--rw-r--r--   0        0        0     8149 2024-03-21 09:38:59.651781 allianceauth-4.0.1/allianceauth/templates/allianceauth/admin-status/overview.html
--rw-r--r--   0        0        0     5607 2024-03-21 09:38:59.651781 allianceauth-4.0.1/allianceauth/templates/allianceauth/base-bs5.html
--rw-r--r--   0        0        0     2443 2024-03-21 09:38:59.651781 allianceauth-4.0.1/allianceauth/templates/allianceauth/base.html
--rw-r--r--   0        0        0     1289 2024-03-21 09:38:59.651781 allianceauth-4.0.1/allianceauth/templates/allianceauth/error.html
--rw-r--r--   0        0        0      928 2024-03-21 09:38:59.651781 allianceauth-4.0.1/allianceauth/templates/allianceauth/icons.html
--rw-r--r--   0        0        0      996 2024-03-21 09:38:59.651781 allianceauth-4.0.1/allianceauth/templates/allianceauth/messages-bs5.html
--rw-r--r--   0        0        0     1115 2024-03-21 09:38:59.651781 allianceauth-4.0.1/allianceauth/templates/allianceauth/messages.html
--rw-r--r--   0        0        0      263 2024-03-21 09:38:59.651781 allianceauth-4.0.1/allianceauth/templates/allianceauth/night-toggle.html
--rw-r--r--   0        0        0      450 2024-03-21 09:38:59.651781 allianceauth-4.0.1/allianceauth/templates/allianceauth/notifications_menu_item.html
--rw-r--r--   0        0        0      879 2024-03-21 09:38:59.651781 allianceauth-4.0.1/allianceauth/templates/allianceauth/side-menu.html
--rw-r--r--   0        0        0      904 2024-03-21 09:38:59.651781 allianceauth-4.0.1/allianceauth/templates/allianceauth/top-menu-admin.html
--rw-r--r--   0        0        0      580 2024-03-21 09:38:59.651781 allianceauth-4.0.1/allianceauth/templates/allianceauth/top-menu-rh-default.html
--rw-r--r--   0        0        0     3086 2024-03-21 09:38:59.651781 allianceauth-4.0.1/allianceauth/templates/allianceauth/top-menu-user-dropdown.html
--rw-r--r--   0        0        0     1576 2024-03-21 09:38:59.651781 allianceauth-4.0.1/allianceauth/templates/allianceauth/top-menu.html
--rw-r--r--   0        0        0       96 2024-03-21 09:38:59.651781 allianceauth-4.0.1/allianceauth/templates/bundles/auth-base-css.html
--rw-r--r--   0        0        0      111 2024-03-21 09:38:59.652781 allianceauth-4.0.1/allianceauth/templates/bundles/auth-framework-css.html
--rw-r--r--   0        0        0      171 2024-03-21 09:38:59.652781 allianceauth-4.0.1/allianceauth/templates/bundles/bootstrap-css-bs5.html
--rw-r--r--   0        0        0     1269 2024-03-21 09:38:59.652781 allianceauth-4.0.1/allianceauth/templates/bundles/bootstrap-css.html
--rw-r--r--   0        0        0      503 2024-03-21 09:38:59.652781 allianceauth-4.0.1/allianceauth/templates/bundles/bootstrap-js-bs5.html
--rw-r--r--   0        0        0      613 2024-03-21 09:38:59.652781 allianceauth-4.0.1/allianceauth/templates/bundles/bootstrap-js.html
--rw-r--r--   0        0        0       95 2024-03-21 09:38:59.652781 allianceauth-4.0.1/allianceauth/templates/bundles/checkbox-css.html
--rw-r--r--   0        0        0      343 2024-03-21 09:38:59.652781 allianceauth-4.0.1/allianceauth/templates/bundles/clipboard-js.html
--rw-r--r--   0        0        0      369 2024-03-21 09:38:59.652781 allianceauth-4.0.1/allianceauth/templates/bundles/datatables-css-bs5.html
--rw-r--r--   0        0        0      365 2024-03-21 09:38:59.652781 allianceauth-4.0.1/allianceauth/templates/bundles/datatables-css.html
--rw-r--r--   0        0        0      628 2024-03-21 09:38:59.652781 allianceauth-4.0.1/allianceauth/templates/bundles/datatables-js-bs5.html
--rw-r--r--   0        0        0      626 2024-03-21 09:38:59.652781 allianceauth-4.0.1/allianceauth/templates/bundles/datatables-js.html
--rw-r--r--   0        0        0       86 2024-03-21 09:38:59.652781 allianceauth-4.0.1/allianceauth/templates/bundles/evetime-js.html
--rw-r--r--   0        0        0      111 2024-03-21 09:38:59.652781 allianceauth-4.0.1/allianceauth/templates/bundles/filterdropdown-js.html
--rw-r--r--   0        0        0      350 2024-03-21 09:38:59.652781 allianceauth-4.0.1/allianceauth/templates/bundles/fontawesome.html
--rw-r--r--   0        0        0      237 2024-03-21 09:38:59.652781 allianceauth-4.0.1/allianceauth/templates/bundles/image-auth-logo.html
--rw-r--r--   0        0        0      392 2024-03-21 09:38:59.652781 allianceauth-4.0.1/allianceauth/templates/bundles/jquery-datetimepicker-css.html
--rw-r--r--   0        0        0      387 2024-03-21 09:38:59.652781 allianceauth-4.0.1/allianceauth/templates/bundles/jquery-datetimepicker-js.html
--rw-r--r--   0        0        0      321 2024-03-21 09:38:59.652781 allianceauth-4.0.1/allianceauth/templates/bundles/jquery-js.html
--rw-r--r--   0        0        0      500 2024-03-21 09:38:59.652781 allianceauth-4.0.1/allianceauth/templates/bundles/jquery-ui-css.html
--rw-r--r--   0        0        0      333 2024-03-21 09:38:59.652781 allianceauth-4.0.1/allianceauth/templates/bundles/jquery-ui-js.html
--rw-r--r--   0        0        0      344 2024-03-21 09:38:59.652781 allianceauth-4.0.1/allianceauth/templates/bundles/jquery-visibility-js.html
--rw-r--r--   0        0        0      579 2024-03-21 09:38:59.652781 allianceauth-4.0.1/allianceauth/templates/bundles/moment-js.html
--rw-r--r--   0        0        0      103 2024-03-21 09:38:59.652781 allianceauth-4.0.1/allianceauth/templates/bundles/refresh-notification-icon-js.html
--rw-r--r--   0        0        0       99 2024-03-21 09:38:59.652781 allianceauth-4.0.1/allianceauth/templates/bundles/refresh-notifications-js.html
--rw-r--r--   0        0        0       88 2024-03-21 09:38:59.652781 allianceauth-4.0.1/allianceauth/templates/bundles/timerboard-js.html
--rw-r--r--   0        0        0       84 2024-03-21 09:38:59.652781 allianceauth-4.0.1/allianceauth/templates/bundles/timers-js.html
--rw-r--r--   0        0        0      368 2024-03-21 09:38:59.652781 allianceauth-4.0.1/allianceauth/templates/bundles/x-editable-js.html
--rw-r--r--   0        0        0      375 2024-03-21 09:38:59.652781 allianceauth-4.0.1/allianceauth/templates/bundles/x-editable.css.html
--rw-r--r--   0        0        0        0 2024-03-21 09:38:59.779780 allianceauth-4.0.1/allianceauth/templatetags/__init__.py
--rw-r--r--   0        0        0     5665 2024-03-21 09:38:59.653781 allianceauth-4.0.1/allianceauth/templatetags/admin_status.py
--rw-r--r--   0        0        0        0 2024-03-21 09:38:59.780780 allianceauth-4.0.1/allianceauth/tests/__init__.py
--rw-r--r--   0        0        0    11465 2024-03-21 09:38:59.653781 allianceauth-4.0.1/allianceauth/tests/auth_utils.py
--rw-r--r--   0        0        0     2061 2024-03-21 09:38:59.653781 allianceauth-4.0.1/allianceauth/tests/test_auth_utils.py
--rw-r--r--   0        0        0     2897 2024-03-21 09:38:59.653781 allianceauth-4.0.1/allianceauth/tests/test_urls.py
--rw-r--r--   0        0        0     1403 2024-03-21 09:38:59.653781 allianceauth-4.0.1/allianceauth/tests/test_views.py
--rw-r--r--   0        0        0        0 2024-03-21 09:38:59.780780 allianceauth-4.0.1/allianceauth/theme/__init__.py
--rw-r--r--   0        0        0      153 2024-03-21 09:38:59.653781 allianceauth-4.0.1/allianceauth/theme/apps.py
--rw-r--r--   0        0        0        0 2024-03-21 09:38:59.780780 allianceauth-4.0.1/allianceauth/theme/bootstrap/__init__.py
--rw-r--r--   0        0        0      241 2024-03-21 09:38:59.653781 allianceauth-4.0.1/allianceauth/theme/bootstrap/apps.py
--rw-r--r--   0        0        0     1778 2024-03-21 09:38:59.653781 allianceauth-4.0.1/allianceauth/theme/bootstrap/auth_hooks.py
--rw-r--r--   0        0        0        0 2024-03-21 09:38:59.780780 allianceauth-4.0.1/allianceauth/theme/darkly/__init__.py
--rw-r--r--   0        0        0      240 2024-03-21 09:38:59.653781 allianceauth-4.0.1/allianceauth/theme/darkly/apps.py
--rw-r--r--   0        0        0     1232 2024-03-21 09:38:59.653781 allianceauth-4.0.1/allianceauth/theme/darkly/auth_hooks.py
--rw-r--r--   0        0        0        0 2024-03-21 09:38:59.780780 allianceauth-4.0.1/allianceauth/theme/flatly/__init__.py
--rw-r--r--   0        0        0      240 2024-03-21 09:38:59.653781 allianceauth-4.0.1/allianceauth/theme/flatly/apps.py
--rw-r--r--   0        0        0     1227 2024-03-21 09:38:59.653781 allianceauth-4.0.1/allianceauth/theme/flatly/auth_hooks.py
--rw-r--r--   0        0        0     1537 2024-03-21 09:38:59.653781 allianceauth-4.0.1/allianceauth/theme/hooks.py
--rw-r--r--   0        0        0        0 2024-03-21 09:38:59.780780 allianceauth-4.0.1/allianceauth/theme/materia/__init__.py
--rw-r--r--   0        0        0      244 2024-03-21 09:38:59.653781 allianceauth-4.0.1/allianceauth/theme/materia/apps.py
--rw-r--r--   0        0        0     1243 2024-03-21 09:38:59.653781 allianceauth-4.0.1/allianceauth/theme/materia/auth_hooks.py
--rw-r--r--   0        0        0        0 2024-03-21 09:38:59.780780 allianceauth-4.0.1/allianceauth/theme/templates/__init__.py
--rw-r--r--   0        0        0        0 2024-03-21 09:38:59.780780 allianceauth-4.0.1/allianceauth/theme/templates/theme/__init__.py
--rw-r--r--   0        0        0      389 2024-03-21 09:38:59.654781 allianceauth-4.0.1/allianceauth/theme/templates/theme/theme_imports_css.html
--rw-r--r--   0        0        0      376 2024-03-21 09:38:59.654781 allianceauth-4.0.1/allianceauth/theme/templates/theme/theme_imports_js.html
--rw-r--r--   0        0        0      494 2024-03-21 09:38:59.654781 allianceauth-4.0.1/allianceauth/theme/templates/theme/theme_select.html
--rw-r--r--   0        0        0        0 2024-03-21 09:38:59.781780 allianceauth-4.0.1/allianceauth/theme/templatetags/__init__.py
--rw-r--r--   0        0        0     1921 2024-03-21 09:38:59.654781 allianceauth-4.0.1/allianceauth/theme/templatetags/theme_tags.py
--rw-r--r--   0        0        0        0 2024-03-21 09:38:59.781780 allianceauth-4.0.1/allianceauth/thirdparty/__init__.py
--rw-r--r--   0        0        0        0 2024-03-21 09:38:59.781780 allianceauth-4.0.1/allianceauth/thirdparty/navhelper/__init__.py
--rw-r--r--   0        0        0        0 2024-03-21 09:38:59.781780 allianceauth-4.0.1/allianceauth/thirdparty/navhelper/templatetags/__init__.py
--rw-r--r--   0        0        0     2876 2024-03-21 09:38:59.654781 allianceauth-4.0.1/allianceauth/thirdparty/navhelper/templatetags/navactive.py
--rw-r--r--   0        0        0     3407 2024-03-21 09:38:59.654781 allianceauth-4.0.1/allianceauth/thirdparty/navhelper/tests.py
--rw-r--r--   0        0        0        0 2024-03-21 09:38:59.781780 allianceauth-4.0.1/allianceauth/timerboard/__init__.py
--rw-r--r--   0        0        0      111 2024-03-21 09:38:59.654781 allianceauth-4.0.1/allianceauth/timerboard/admin.py
--rw-r--r--   0        0        0      133 2024-03-21 09:38:59.654781 allianceauth-4.0.1/allianceauth/timerboard/apps.py
--rw-r--r--   0        0        0     1141 2024-03-21 09:38:59.654781 allianceauth-4.0.1/allianceauth/timerboard/auth_hooks.py
--rw-r--r--   0        0        0     5267 2024-03-21 09:38:59.654781 allianceauth-4.0.1/allianceauth/timerboard/form.py
--rw-r--r--   0        0        0     1629 2024-03-21 09:38:59.654781 allianceauth-4.0.1/allianceauth/timerboard/migrations/0001_initial.py
--rw-r--r--   0        0        0     1063 2024-03-21 09:38:59.654781 allianceauth-4.0.1/allianceauth/timerboard/migrations/0002_make_strings_more_stringy.py
--rw-r--r--   0        0        0      763 2024-03-21 09:38:59.654781 allianceauth-4.0.1/allianceauth/timerboard/migrations/0003_on_delete.py
--rw-r--r--   0        0        0      811 2024-03-21 09:38:59.654781 allianceauth-4.0.1/allianceauth/timerboard/migrations/0004_timer_type.py
--rw-r--r--   0        0        0      410 2024-03-21 09:38:59.654781 allianceauth-4.0.1/allianceauth/timerboard/migrations/0005_alter_timer_planet_moon.py
--rw-r--r--   0        0        0        0 2024-03-21 09:38:59.781780 allianceauth-4.0.1/allianceauth/timerboard/migrations/__init__.py
--rw-r--r--   0        0        0     1593 2024-03-21 09:38:59.654781 allianceauth-4.0.1/allianceauth/timerboard/models.py
--rw-r--r--   0        0        0     3069 2024-03-21 09:38:59.654781 allianceauth-4.0.1/allianceauth/timerboard/templates/timerboard/dashboard.timers.html
--rw-r--r--   0        0        0     1917 2024-03-21 09:38:59.654781 allianceauth-4.0.1/allianceauth/timerboard/templates/timerboard/form.html
--rw-r--r--   0        0        0      147 2024-03-21 09:38:59.654781 allianceauth-4.0.1/allianceauth/timerboard/templates/timerboard/index_button.html
--rw-r--r--   0        0        0     1021 2024-03-21 09:38:59.655781 allianceauth-4.0.1/allianceauth/timerboard/templates/timerboard/timer_confirm_delete.html
--rw-r--r--   0        0        0      810 2024-03-21 09:38:59.655781 allianceauth-4.0.1/allianceauth/timerboard/templates/timerboard/timer_create_form.html
--rw-r--r--   0        0        0      830 2024-03-21 09:38:59.655781 allianceauth-4.0.1/allianceauth/timerboard/templates/timerboard/timer_update_form.html
--rw-r--r--   0        0        0     8191 2024-03-21 09:38:59.655781 allianceauth-4.0.1/allianceauth/timerboard/templates/timerboard/timertable.html
--rw-r--r--   0        0        0     5121 2024-03-21 09:38:59.655781 allianceauth-4.0.1/allianceauth/timerboard/templates/timerboard/view.html
--rw-r--r--   0        0        0     8741 2024-03-21 09:38:59.655781 allianceauth-4.0.1/allianceauth/timerboard/tests.py
--rw-r--r--   0        0        0      358 2024-03-21 09:38:59.655781 allianceauth-4.0.1/allianceauth/timerboard/urls.py
--rw-r--r--   0        0        0     4075 2024-03-21 09:38:59.655781 allianceauth-4.0.1/allianceauth/timerboard/views.py
--rw-r--r--   0        0        0     2688 2024-03-21 09:38:59.655781 allianceauth-4.0.1/allianceauth/urls.py
--rw-r--r--   0        0        0        0 2024-03-21 09:38:59.782780 allianceauth-4.0.1/allianceauth/utils/__init__.py
--rw-r--r--   0        0        0      568 2024-03-21 09:38:59.655781 allianceauth-4.0.1/allianceauth/utils/cache.py
--rw-r--r--   0        0        0     1971 2024-03-21 09:38:59.655781 allianceauth-4.0.1/allianceauth/utils/counters.py
--rw-r--r--   0        0        0      615 2024-03-21 09:38:59.655781 allianceauth-4.0.1/allianceauth/utils/django.py
--rw-r--r--   0        0        0      844 2024-03-21 09:38:59.655781 allianceauth-4.0.1/allianceauth/utils/testing.py
--rw-r--r--   0        0        0        0 2024-03-21 09:38:59.782780 allianceauth-4.0.1/allianceauth/utils/tests/__init__.py
--rw-r--r--   0        0        0     1194 2024-03-21 09:38:59.655781 allianceauth-4.0.1/allianceauth/utils/tests/test_cache.py
--rw-r--r--   0        0        0     3328 2024-03-21 09:38:59.655781 allianceauth-4.0.1/allianceauth/utils/tests/test_counters.py
--rw-r--r--   0        0        0      777 2024-03-21 09:38:59.655781 allianceauth-4.0.1/allianceauth/utils/tests/test_django.py
--rw-r--r--   0        0        0      310 2024-03-21 09:38:59.655781 allianceauth-4.0.1/allianceauth/utils/tests/test_testing.py
--rw-r--r--   0        0        0     3289 2024-03-21 09:38:59.655781 allianceauth-4.0.1/allianceauth/views.py
--rw-r--r--   0        0        0     2436 2024-03-21 09:38:59.673781 allianceauth-4.0.1/pyproject.toml
--rw-r--r--   0        0        0     7463 1970-01-01 00:00:00.000000 allianceauth-4.0.1/PKG-INFO
+-rw-r--r--   0        0        0    18026 2024-05-12 10:07:44.141393 allianceauth-4.0.2/LICENSE
+-rw-r--r--   0        0        0     4980 2024-05-12 10:07:44.141393 allianceauth-4.0.2/README.md
+-rw-r--r--   0        0        0      352 2024-05-12 10:07:44.141393 allianceauth-4.0.2/allianceauth/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-12 10:07:44.285393 allianceauth-4.0.2/allianceauth/analytics/__init__.py
+-rw-r--r--   0        0        0      401 2024-05-12 10:07:44.141393 allianceauth-4.0.2/allianceauth/analytics/admin.py
+-rw-r--r--   0        0        0      130 2024-05-12 10:07:44.141393 allianceauth-4.0.2/allianceauth/analytics/apps.py
+-rw-r--r--   0        0        0      456 2024-05-12 10:07:44.141393 allianceauth-4.0.2/allianceauth/analytics/fixtures/disable_analytics.json
+-rw-r--r--   0        0        0     1664 2024-05-12 10:07:44.142393 allianceauth-4.0.2/allianceauth/analytics/migrations/0001_initial.py
+-rw-r--r--   0        0        0     1072 2024-05-12 10:07:44.142393 allianceauth-4.0.2/allianceauth/analytics/migrations/0002_add_AA_Team_Token.py
+-rw-r--r--   0        0        0      907 2024-05-12 10:07:44.142393 allianceauth-4.0.2/allianceauth/analytics/migrations/0003_Generate_Identifier.py
+-rw-r--r--   0        0        0     1650 2024-05-12 10:07:44.142393 allianceauth-4.0.2/allianceauth/analytics/migrations/0004_auto_20211015_0502.py
+-rw-r--r--   0        0        0      495 2024-05-12 10:07:44.142393 allianceauth-4.0.2/allianceauth/analytics/migrations/0005_alter_analyticspath_ignore_path.py
+-rw-r--r--   0        0        0     1413 2024-05-12 10:07:44.142393 allianceauth-4.0.2/allianceauth/analytics/migrations/0006_more_ignore_paths.py
+-rw-r--r--   0        0        0      407 2024-05-12 10:07:44.142393 allianceauth-4.0.2/allianceauth/analytics/migrations/0007_analyticstokens_secret.py
+-rw-r--r--   0        0        0     2451 2024-05-12 10:07:44.142393 allianceauth-4.0.2/allianceauth/analytics/migrations/0008_add_AA_GA-4_Team_Token .py
+-rw-r--r--   0        0        0      672 2024-05-12 10:07:44.142393 allianceauth-4.0.2/allianceauth/analytics/migrations/0009_remove_analyticstokens_ignore_paths_and_more.py
+-rw-r--r--   0        0        0        0 2024-05-12 10:07:44.296393 allianceauth-4.0.2/allianceauth/analytics/migrations/__init__.py
+-rw-r--r--   0        0        0     1173 2024-05-12 10:07:44.142393 allianceauth-4.0.2/allianceauth/analytics/models.py
+-rw-r--r--   0        0        0     5449 2024-05-12 10:07:44.142393 allianceauth-4.0.2/allianceauth/analytics/tasks.py
+-rw-r--r--   0        0        0        0 2024-05-12 10:07:44.296393 allianceauth-4.0.2/allianceauth/analytics/tests/__init__.py
+-rw-r--r--   0        0        0      951 2024-05-12 10:07:44.142393 allianceauth-4.0.2/allianceauth/analytics/tests/test_models.py
+-rw-r--r--   0        0        0     2007 2024-05-12 10:07:44.142393 allianceauth-4.0.2/allianceauth/analytics/tests/test_tasks.py
+-rw-r--r--   0        0        0     1535 2024-05-12 10:07:44.143393 allianceauth-4.0.2/allianceauth/analytics/tests/test_utils.py
+-rw-r--r--   0        0        0      777 2024-05-12 10:07:44.143393 allianceauth-4.0.2/allianceauth/analytics/utils.py
+-rw-r--r--   0        0        0     1178 2024-05-12 10:07:44.143393 allianceauth-4.0.2/allianceauth/apps.py
+-rw-r--r--   0        0        0        0 2024-05-12 10:07:44.296393 allianceauth-4.0.2/allianceauth/authentication/__init__.py
+-rw-r--r--   0        0        0    21182 2024-05-12 10:07:44.143393 allianceauth-4.0.2/allianceauth/authentication/admin.py
+-rw-r--r--   0        0        0     1345 2024-05-12 10:07:44.143393 allianceauth-4.0.2/allianceauth/authentication/app_settings.py
+-rw-r--r--   0        0        0      514 2024-05-12 10:07:44.143393 allianceauth-4.0.2/allianceauth/authentication/apps.py
+-rw-r--r--   0        0        0     1243 2024-05-12 10:07:44.143393 allianceauth-4.0.2/allianceauth/authentication/auth_hooks.py
+-rw-r--r--   0        0        0     5150 2024-05-12 10:07:44.143393 allianceauth-4.0.2/allianceauth/authentication/backends.py
+-rw-r--r--   0        0        0      434 2024-05-12 10:07:44.143393 allianceauth-4.0.2/allianceauth/authentication/checks.py
+-rw-r--r--   0        0        0      641 2024-05-12 10:07:44.143393 allianceauth-4.0.2/allianceauth/authentication/constants.py
+-rw-r--r--   0        0        0        0 2024-05-12 10:07:44.296393 allianceauth-4.0.2/allianceauth/authentication/core/__init__.py
+-rw-r--r--   0        0        0     1307 2024-05-12 10:07:44.143393 allianceauth-4.0.2/allianceauth/authentication/core/celery_workers.py
+-rw-r--r--   0        0        0     3063 2024-05-12 10:07:44.143393 allianceauth-4.0.2/allianceauth/authentication/decorators.py
+-rw-r--r--   0        0        0     2480 2024-05-12 10:07:44.144393 allianceauth-4.0.2/allianceauth/authentication/forms.py
+-rw-r--r--   0        0        0      776 2024-05-12 10:07:44.144393 allianceauth-4.0.2/allianceauth/authentication/hmac_urls.py
+-rw-r--r--   0        0        0        0 2024-05-12 10:07:44.296393 allianceauth-4.0.2/allianceauth/authentication/management/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-12 10:07:44.296393 allianceauth-4.0.2/allianceauth/authentication/management/commands/__init__.py
+-rw-r--r--   0        0        0     1026 2024-05-12 10:07:44.144393 allianceauth-4.0.2/allianceauth/authentication/management/commands/checkmains.py
+-rw-r--r--   0        0        0     2709 2024-05-12 10:07:44.144393 allianceauth-4.0.2/allianceauth/authentication/managers.py
+-rw-r--r--   0        0        0     2422 2024-05-12 10:07:44.144393 allianceauth-4.0.2/allianceauth/authentication/middleware.py
+-rw-r--r--   0        0        0     3147 2024-05-12 10:07:44.144393 allianceauth-4.0.2/allianceauth/authentication/migrations/0001_initial.py
+-rw-r--r--   0        0        0      474 2024-05-12 10:07:44.144393 allianceauth-4.0.2/allianceauth/authentication/migrations/0002_auto_20160907_1914.py
+-rw-r--r--   0        0        0      509 2024-05-12 10:07:44.144393 allianceauth-4.0.2/allianceauth/authentication/migrations/0003_authservicesinfo_state.py
+-rw-r--r--   0        0        0     2543 2024-05-12 10:07:44.144393 allianceauth-4.0.2/allianceauth/authentication/migrations/0004_create_permissions.py
+-rw-r--r--   0        0        0     1144 2024-05-12 10:07:44.144393 allianceauth-4.0.2/allianceauth/authentication/migrations/0005_delete_perms.py
+-rw-r--r--   0        0        0     1324 2024-05-12 10:07:44.145393 allianceauth-4.0.2/allianceauth/authentication/migrations/0006_auto_20160910_0542.py
+-rw-r--r--   0        0        0      347 2024-05-12 10:07:44.145393 allianceauth-4.0.2/allianceauth/authentication/migrations/0007_remove_authservicesinfo_is_blue.py
+-rw-r--r--   0        0        0      319 2024-05-12 10:07:44.145393 allianceauth-4.0.2/allianceauth/authentication/migrations/0008_set_state.py
+-rw-r--r--   0        0        0      532 2024-05-12 10:07:44.145393 allianceauth-4.0.2/allianceauth/authentication/migrations/0009_auto_20161021_0228.py
+-rw-r--r--   0        0        0     1235 2024-05-12 10:07:44.145393 allianceauth-4.0.2/allianceauth/authentication/migrations/0010_only_one_authservicesinfo.py
+-rw-r--r--   0        0        0      538 2024-05-12 10:07:44.145393 allianceauth-4.0.2/allianceauth/authentication/migrations/0011_authservicesinfo_user_onetoonefield.py
+-rw-r--r--   0        0        0     1567 2024-05-12 10:07:44.145393 allianceauth-4.0.2/allianceauth/authentication/migrations/0012_remove_add_delete_authservicesinfo_permissions.py
+-rw-r--r--   0        0        0     1914 2024-05-12 10:07:44.145393 allianceauth-4.0.2/allianceauth/authentication/migrations/0013_service_modules.py
+-rw-r--r--   0        0        0      660 2024-05-12 10:07:44.145393 allianceauth-4.0.2/allianceauth/authentication/migrations/0014_fleetup_permission.py
+-rw-r--r--   0        0        0    13077 2024-05-12 10:07:44.145393 allianceauth-4.0.2/allianceauth/authentication/migrations/0015_user_profiles.py
+-rw-r--r--   0        0        0     1637 2024-05-12 10:07:44.145393 allianceauth-4.0.2/allianceauth/authentication/migrations/0016_ownershiprecord.py
+-rw-r--r--   0        0        0      612 2024-05-12 10:07:44.145393 allianceauth-4.0.2/allianceauth/authentication/migrations/0017_remove_fleetup_permission.py
+-rw-r--r--   0        0        0      410 2024-05-12 10:07:44.145393 allianceauth-4.0.2/allianceauth/authentication/migrations/0018_alter_state_name_length.py
+-rw-r--r--   0        0        0      545 2024-05-12 10:07:44.145393 allianceauth-4.0.2/allianceauth/authentication/migrations/0018_state_member_factions.py
+-rw-r--r--   0        0        0      295 2024-05-12 10:07:44.146393 allianceauth-4.0.2/allianceauth/authentication/migrations/0019_merge_20211026_0919.py
+-rw-r--r--   0        0        0      841 2024-05-12 10:07:44.146393 allianceauth-4.0.2/allianceauth/authentication/migrations/0020_userprofile_language_userprofile_night_mode.py
+-rw-r--r--   0        0        0     1004 2024-05-12 10:07:44.146393 allianceauth-4.0.2/allianceauth/authentication/migrations/0021_alter_userprofile_language.py
+-rw-r--r--   0        0        0      529 2024-05-12 10:07:44.146393 allianceauth-4.0.2/allianceauth/authentication/migrations/0022_userprofile_theme.py
+-rw-r--r--   0        0        0      683 2024-05-12 10:07:44.146393 allianceauth-4.0.2/allianceauth/authentication/migrations/0023_alter_userprofile_language.py
+-rw-r--r--   0        0        0        0 2024-05-12 10:07:44.296393 allianceauth-4.0.2/allianceauth/authentication/migrations/__init__.py
+-rw-r--r--   0        0        0     6050 2024-05-12 10:07:44.146393 allianceauth-4.0.2/allianceauth/authentication/models.py
+-rw-r--r--   0        0        0     7806 2024-05-12 10:07:44.146393 allianceauth-4.0.2/allianceauth/authentication/signals.py
+-rw-r--r--   0        0        0      506 2024-05-12 10:07:44.146393 allianceauth-4.0.2/allianceauth/authentication/static/allianceauth/authentication/css/admin.css
+-rw-r--r--   0        0        0   161344 2024-05-12 10:07:44.147393 allianceauth-4.0.2/allianceauth/authentication/static/allianceauth/authentication/img/background.jpg
+-rw-r--r--   0        0        0     2308 2024-05-12 10:07:44.147393 allianceauth-4.0.2/allianceauth/authentication/static/allianceauth/authentication/img/sso/EVE_SSO_Login_Buttons_Large_Black.png
+-rw-r--r--   0        0        0     2248 2024-05-12 10:07:44.147393 allianceauth-4.0.2/allianceauth/authentication/static/allianceauth/authentication/img/sso/EVE_SSO_Login_Buttons_Large_White.png
+-rw-r--r--   0        0        0        0 2024-05-12 10:07:44.296393 allianceauth-4.0.2/allianceauth/authentication/task_statistics/__init__.py
+-rw-r--r--   0        0        0     1536 2024-05-12 10:07:44.148393 allianceauth-4.0.2/allianceauth/authentication/task_statistics/counters.py
+-rw-r--r--   0        0        0     3257 2024-05-12 10:07:44.148393 allianceauth-4.0.2/allianceauth/authentication/task_statistics/event_series.py
+-rw-r--r--   0        0        0     1174 2024-05-12 10:07:44.148393 allianceauth-4.0.2/allianceauth/authentication/task_statistics/helpers.py
+-rw-r--r--   0        0        0     1217 2024-05-12 10:07:44.148393 allianceauth-4.0.2/allianceauth/authentication/task_statistics/signals.py
+-rw-r--r--   0        0        0        0 2024-05-12 10:07:44.296393 allianceauth-4.0.2/allianceauth/authentication/task_statistics/tests/__init__.py
+-rw-r--r--   0        0        0     1704 2024-05-12 10:07:44.148393 allianceauth-4.0.2/allianceauth/authentication/task_statistics/tests/test_counters.py
+-rw-r--r--   0        0        0     5137 2024-05-12 10:07:44.148393 allianceauth-4.0.2/allianceauth/authentication/task_statistics/tests/test_event_series.py
+-rw-r--r--   0        0        0     1009 2024-05-12 10:07:44.148393 allianceauth-4.0.2/allianceauth/authentication/task_statistics/tests/test_helpers.py
+-rw-r--r--   0        0        0     2719 2024-05-12 10:07:44.148393 allianceauth-4.0.2/allianceauth/authentication/task_statistics/tests/test_signals.py
+-rw-r--r--   0        0        0     1661 2024-05-12 10:07:44.148393 allianceauth-4.0.2/allianceauth/authentication/tasks.py
+-rw-r--r--   0        0        0      423 2024-05-12 10:07:44.148393 allianceauth-4.0.2/allianceauth/authentication/templates/authentication/dashboard.html
+-rw-r--r--   0        0        0      188 2024-05-12 10:07:44.148393 allianceauth-4.0.2/allianceauth/authentication/templates/authentication/dashboard_bs3.html
+-rw-r--r--   0        0        0     2476 2024-05-12 10:07:44.149393 allianceauth-4.0.2/allianceauth/authentication/templates/authentication/dashboard_characters.html
+-rw-r--r--   0        0        0      838 2024-05-12 10:07:44.149393 allianceauth-4.0.2/allianceauth/authentication/templates/authentication/dashboard_groups.html
+-rw-r--r--   0        0        0     3043 2024-05-12 10:07:44.149393 allianceauth-4.0.2/allianceauth/authentication/templates/authentication/tokens.html
+-rw-r--r--   0        0        0     2001 2024-05-12 10:07:44.149393 allianceauth-4.0.2/allianceauth/authentication/templates/public/base.html
+-rw-r--r--   0        0        0      674 2024-05-12 10:07:44.149393 allianceauth-4.0.2/allianceauth/authentication/templates/public/lang_select.html
+-rw-r--r--   0        0        0      493 2024-05-12 10:07:44.149393 allianceauth-4.0.2/allianceauth/authentication/templates/public/login.html
+-rw-r--r--   0        0        0     1604 2024-05-12 10:07:44.149393 allianceauth-4.0.2/allianceauth/authentication/templates/public/middle_box.html
+-rw-r--r--   0        0        0      956 2024-05-12 10:07:44.149393 allianceauth-4.0.2/allianceauth/authentication/templates/public/register.html
+-rw-r--r--   0        0        0      199 2024-05-12 10:07:44.149393 allianceauth-4.0.2/allianceauth/authentication/templates/registration/activate.html
+-rw-r--r--   0        0        0      346 2024-05-12 10:07:44.149393 allianceauth-4.0.2/allianceauth/authentication/templates/registration/activation_email.txt
+-rw-r--r--   0        0        0      446 2024-05-12 10:07:44.149393 allianceauth-4.0.2/allianceauth/authentication/templates/registration/activation_email_html.txt
+-rw-r--r--   0        0        0       49 2024-05-12 10:07:44.149393 allianceauth-4.0.2/allianceauth/authentication/templates/registration/activation_email_subject.txt
+-rw-r--r--   0        0        0      833 2024-05-12 10:07:44.150393 allianceauth-4.0.2/allianceauth/authentication/tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-12 10:07:44.303393 allianceauth-4.0.2/allianceauth/authentication/tests/core/__init__.py
+-rw-r--r--   0        0        0     2685 2024-05-12 10:07:44.150393 allianceauth-4.0.2/allianceauth/authentication/tests/core/test_celery_workers.py
+-rw-r--r--   0        0        0    29475 2024-05-12 10:07:44.150393 allianceauth-4.0.2/allianceauth/authentication/tests/test_admin.py
+-rw-r--r--   0        0        0     3456 2024-05-12 10:07:44.150393 allianceauth-4.0.2/allianceauth/authentication/tests/test_app_settings.py
+-rw-r--r--   0        0        0     7427 2024-05-12 10:07:44.150393 allianceauth-4.0.2/allianceauth/authentication/tests/test_backend.py
+-rw-r--r--   0        0        0     1517 2024-05-12 10:07:44.150393 allianceauth-4.0.2/allianceauth/authentication/tests/test_commands.py
+-rw-r--r--   0        0        0     3538 2024-05-12 10:07:44.150393 allianceauth-4.0.2/allianceauth/authentication/tests/test_decorators.py
+-rw-r--r--   0        0        0     6316 2024-05-12 10:07:44.150393 allianceauth-4.0.2/allianceauth/authentication/tests/test_middleware.py
+-rw-r--r--   0        0        0    11478 2024-05-12 10:07:44.150393 allianceauth-4.0.2/allianceauth/authentication/tests/test_models.py
+-rw-r--r--   0        0        0     3154 2024-05-12 10:07:44.150393 allianceauth-4.0.2/allianceauth/authentication/tests/test_signals.py
+-rw-r--r--   0        0        0    10730 2024-05-12 10:07:44.151393 allianceauth-4.0.2/allianceauth/authentication/tests/test_templatetags.py
+-rw-r--r--   0        0        0     5865 2024-05-12 10:07:44.151393 allianceauth-4.0.2/allianceauth/authentication/tests/test_views.py
+-rw-r--r--   0        0        0     1170 2024-05-12 10:07:44.151393 allianceauth-4.0.2/allianceauth/authentication/urls.py
+-rw-r--r--   0        0        0    14250 2024-05-12 10:07:44.151393 allianceauth-4.0.2/allianceauth/authentication/views.py
+-rw-r--r--   0        0        0        0 2024-05-12 10:07:44.303393 allianceauth-4.0.2/allianceauth/bin/__init__.py
+-rw-r--r--   0        0        0     3680 2024-05-12 10:07:44.151393 allianceauth-4.0.2/allianceauth/bin/allianceauth.py
+-rw-r--r--   0        0        0      274 2024-05-12 10:07:44.151393 allianceauth-4.0.2/allianceauth/context_processors.py
+-rw-r--r--   0        0        0        0 2024-05-12 10:07:44.303393 allianceauth-4.0.2/allianceauth/corputils/__init__.py
+-rw-r--r--   0        0        0      140 2024-05-12 10:07:44.151393 allianceauth-4.0.2/allianceauth/corputils/admin.py
+-rw-r--r--   0        0        0      130 2024-05-12 10:07:44.151393 allianceauth-4.0.2/allianceauth/corputils/apps.py
+-rw-r--r--   0        0        0     1043 2024-05-12 10:07:44.151393 allianceauth-4.0.2/allianceauth/corputils/auth_hooks.py
+-rw-r--r--   0        0        0     1970 2024-05-12 10:07:44.151393 allianceauth-4.0.2/allianceauth/corputils/managers.py
+-rw-r--r--   0        0        0     1417 2024-05-12 10:07:44.151393 allianceauth-4.0.2/allianceauth/corputils/migrations/0001_initial.py
+-rw-r--r--   0        0        0     5358 2024-05-12 10:07:44.152393 allianceauth-4.0.2/allianceauth/corputils/migrations/0002_migrate_permissions.py
+-rw-r--r--   0        0        0      844 2024-05-12 10:07:44.152393 allianceauth-4.0.2/allianceauth/corputils/migrations/0003_granular_permissions.py
+-rw-r--r--   0        0        0     2029 2024-05-12 10:07:44.152393 allianceauth-4.0.2/allianceauth/corputils/migrations/0004_member_models.py
+-rw-r--r--   0        0        0     1516 2024-05-12 10:07:44.152393 allianceauth-4.0.2/allianceauth/corputils/migrations/0005_cleanup_permissions.py
+-rw-r--r--   0        0        0        0 2024-05-12 10:07:44.303393 allianceauth-4.0.2/allianceauth/corputils/migrations/__init__.py
+-rw-r--r--   0        0        0     7223 2024-05-12 10:07:44.152393 allianceauth-4.0.2/allianceauth/corputils/models.py
+-rw-r--r--   0        0        0   947431 2024-05-12 10:07:44.155393 allianceauth-4.0.2/allianceauth/corputils/swagger.json
+-rw-r--r--   0        0        0      298 2024-05-12 10:07:44.155393 allianceauth-4.0.2/allianceauth/corputils/tasks.py
+-rw-r--r--   0        0        0     1991 2024-05-12 10:07:44.155393 allianceauth-4.0.2/allianceauth/corputils/templates/corputils/base.html
+-rw-r--r--   0        0        0    14560 2024-05-12 10:07:44.155393 allianceauth-4.0.2/allianceauth/corputils/templates/corputils/corpstats.html
+-rw-r--r--   0        0        0     2268 2024-05-12 10:07:44.155393 allianceauth-4.0.2/allianceauth/corputils/templates/corputils/search.html
+-rw-r--r--   0        0        0    16016 2024-05-12 10:07:44.155393 allianceauth-4.0.2/allianceauth/corputils/tests.py
+-rw-r--r--   0        0        0      393 2024-05-12 10:07:44.155393 allianceauth-4.0.2/allianceauth/corputils/urls.py
+-rw-r--r--   0        0        0     6999 2024-05-12 10:07:44.155393 allianceauth-4.0.2/allianceauth/corputils/views.py
+-rw-r--r--   0        0        0        0 2024-05-12 10:07:44.303393 allianceauth-4.0.2/allianceauth/eveonline/__init__.py
+-rw-r--r--   0        0        0     7277 2024-05-12 10:07:44.156393 allianceauth-4.0.2/allianceauth/eveonline/admin.py
+-rw-r--r--   0        0        0      130 2024-05-12 10:07:44.156393 allianceauth-4.0.2/allianceauth/eveonline/apps.py
+-rw-r--r--   0        0        0        0 2024-05-12 10:07:44.303393 allianceauth-4.0.2/allianceauth/eveonline/autogroups/__init__.py
+-rw-r--r--   0        0        0     1320 2024-05-12 10:07:44.156393 allianceauth-4.0.2/allianceauth/eveonline/autogroups/admin.py
+-rw-r--r--   0        0        0      229 2024-05-12 10:07:44.156393 allianceauth-4.0.2/allianceauth/eveonline/autogroups/apps.py
+-rw-r--r--   0        0        0     4024 2024-05-12 10:07:44.156393 allianceauth-4.0.2/allianceauth/eveonline/autogroups/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2024-05-12 10:07:44.303393 allianceauth-4.0.2/allianceauth/eveonline/autogroups/migrations/__init__.py
+-rw-r--r--   0        0        0    10691 2024-05-12 10:07:44.156393 allianceauth-4.0.2/allianceauth/eveonline/autogroups/models.py
+-rw-r--r--   0        0        0     2625 2024-05-12 10:07:44.156393 allianceauth-4.0.2/allianceauth/eveonline/autogroups/signals.py
+-rw-r--r--   0        0        0     1403 2024-05-12 10:07:44.156393 allianceauth-4.0.2/allianceauth/eveonline/autogroups/tests/__init__.py
+-rw-r--r--   0        0        0     3221 2024-05-12 10:07:44.156393 allianceauth-4.0.2/allianceauth/eveonline/autogroups/tests/test_managers.py
+-rw-r--r--   0        0        0    12334 2024-05-12 10:07:44.156393 allianceauth-4.0.2/allianceauth/eveonline/autogroups/tests/test_models.py
+-rw-r--r--   0        0        0     7961 2024-05-12 10:07:44.157393 allianceauth-4.0.2/allianceauth/eveonline/autogroups/tests/test_signals.py
+-rw-r--r--   0        0        0      646 2024-05-12 10:07:44.157393 allianceauth-4.0.2/allianceauth/eveonline/evelinks/__init__.py
+-rw-r--r--   0        0        0     1496 2024-05-12 10:07:44.157393 allianceauth-4.0.2/allianceauth/eveonline/evelinks/dotlan.py
+-rw-r--r--   0        0        0     3730 2024-05-12 10:07:44.157393 allianceauth-4.0.2/allianceauth/eveonline/evelinks/eveimageserver.py
+-rw-r--r--   0        0        0     1229 2024-05-12 10:07:44.157393 allianceauth-4.0.2/allianceauth/eveonline/evelinks/evewho.py
+-rw-r--r--   0        0        0        0 2024-05-12 10:07:44.303393 allianceauth-4.0.2/allianceauth/eveonline/evelinks/tests/__init__.py
+-rw-r--r--   0        0        0     7329 2024-05-12 10:07:44.157393 allianceauth-4.0.2/allianceauth/eveonline/evelinks/tests/test_evelinks.py
+-rw-r--r--   0        0        0    11505 2024-05-12 10:07:44.157393 allianceauth-4.0.2/allianceauth/eveonline/evelinks/tests/test_templatetags.py
+-rw-r--r--   0        0        0     1700 2024-05-12 10:07:44.157393 allianceauth-4.0.2/allianceauth/eveonline/evelinks/zkillboard.py
+-rw-r--r--   0        0        0     3350 2024-05-12 10:07:44.157393 allianceauth-4.0.2/allianceauth/eveonline/managers.py
+-rw-r--r--   0        0        0     3133 2024-05-12 10:07:44.157393 allianceauth-4.0.2/allianceauth/eveonline/migrations/0001_initial.py
+-rw-r--r--   0        0        0      332 2024-05-12 10:07:44.158393 allianceauth-4.0.2/allianceauth/eveonline/migrations/0002_remove_eveapikeypair_error_count.py
+-rw-r--r--   0        0        0      797 2024-05-12 10:07:44.158393 allianceauth-4.0.2/allianceauth/eveonline/migrations/0003_auto_20161026_0149.py
+-rw-r--r--   0        0        0      403 2024-05-12 10:07:44.158393 allianceauth-4.0.2/allianceauth/eveonline/migrations/0004_eveapikeypair_sso_verified.py
+-rw-r--r--   0        0        0      354 2024-05-12 10:07:44.158393 allianceauth-4.0.2/allianceauth/eveonline/migrations/0005_remove_eveallianceinfo_member_count.py
+-rw-r--r--   0        0        0      655 2024-05-12 10:07:44.158393 allianceauth-4.0.2/allianceauth/eveonline/migrations/0006_allow_null_evecharacter_alliance.py
+-rw-r--r--   0        0        0     4599 2024-05-12 10:07:44.158393 allianceauth-4.0.2/allianceauth/eveonline/migrations/0007_unique_id_name.py
+-rw-r--r--   0        0        0      854 2024-05-12 10:07:44.158393 allianceauth-4.0.2/allianceauth/eveonline/migrations/0008_remove_apikeys.py
+-rw-r--r--   0        0        0      519 2024-05-12 10:07:44.158393 allianceauth-4.0.2/allianceauth/eveonline/migrations/0009_on_delete.py
+-rw-r--r--   0        0        0      596 2024-05-12 10:07:44.158393 allianceauth-4.0.2/allianceauth/eveonline/migrations/0010_alliance_ticker.py
+-rw-r--r--   0        0        0     1297 2024-05-12 10:07:44.158393 allianceauth-4.0.2/allianceauth/eveonline/migrations/0011_ids_to_integers.py
+-rw-r--r--   0        0        0     1121 2024-05-12 10:07:44.158393 allianceauth-4.0.2/allianceauth/eveonline/migrations/0012_index_additions.py
+-rw-r--r--   0        0        0      428 2024-05-12 10:07:44.158393 allianceauth-4.0.2/allianceauth/eveonline/migrations/0013_evecorporationinfo_ceo_id.py
+-rw-r--r--   0        0        0      416 2024-05-12 10:07:44.158393 allianceauth-4.0.2/allianceauth/eveonline/migrations/0014_auto_20210105_1413.py
+-rw-r--r--   0        0        0     1201 2024-05-12 10:07:44.158393 allianceauth-4.0.2/allianceauth/eveonline/migrations/0015_factions.py
+-rw-r--r--   0        0        0      409 2024-05-12 10:07:44.158393 allianceauth-4.0.2/allianceauth/eveonline/migrations/0016_character_names_are_not_unique.py
+-rw-r--r--   0        0        0      623 2024-05-12 10:07:44.158393 allianceauth-4.0.2/allianceauth/eveonline/migrations/0017_alliance_and_corp_names_are_not_unique.py
+-rw-r--r--   0        0        0        0 2024-05-12 10:07:44.303393 allianceauth-4.0.2/allianceauth/eveonline/migrations/__init__.py
+-rw-r--r--   0        0        0    14052 2024-05-12 10:07:44.159393 allianceauth-4.0.2/allianceauth/eveonline/models.py
+-rw-r--r--   0        0        0     9958 2024-05-12 10:07:44.159393 allianceauth-4.0.2/allianceauth/eveonline/providers.py
+-rw-r--r--   0        0        0    41989 2024-05-12 10:07:44.159393 allianceauth-4.0.2/allianceauth/eveonline/swagger.json
+-rw-r--r--   0        0        0     3808 2024-05-12 10:07:44.159393 allianceauth-4.0.2/allianceauth/eveonline/tasks.py
+-rw-r--r--   0        0        0        0 2024-05-12 10:07:44.303393 allianceauth-4.0.2/allianceauth/eveonline/templatetags/__init__.py
+-rw-r--r--   0        0        0     8354 2024-05-12 10:07:44.159393 allianceauth-4.0.2/allianceauth/eveonline/templatetags/evelinks.py
+-rw-r--r--   0        0        0     4194 2024-05-12 10:07:44.159393 allianceauth-4.0.2/allianceauth/eveonline/templatetags/examples.html
+-rw-r--r--   0        0        0      739 2024-05-12 10:07:44.159393 allianceauth-4.0.2/allianceauth/eveonline/tests/__init__.py
+-rw-r--r--   0        0        0     6043 2024-05-12 10:07:44.159393 allianceauth-4.0.2/allianceauth/eveonline/tests/esi_client_stub.py
+-rw-r--r--   0        0        0   297070 2024-05-12 10:07:44.160393 allianceauth-4.0.2/allianceauth/eveonline/tests/swagger_old.json
+-rw-r--r--   0        0        0    10079 2024-05-12 10:07:44.160393 allianceauth-4.0.2/allianceauth/eveonline/tests/test_managers.py
+-rw-r--r--   0        0        0    23361 2024-05-12 10:07:44.161393 allianceauth-4.0.2/allianceauth/eveonline/tests/test_models.py
+-rw-r--r--   0        0        0    23834 2024-05-12 10:07:44.161393 allianceauth-4.0.2/allianceauth/eveonline/tests/test_providers.py
+-rw-r--r--   0        0        0    10117 2024-05-12 10:07:44.161393 allianceauth-4.0.2/allianceauth/eveonline/tests/test_tasks.py
+-rw-r--r--   0        0        0        0 2024-05-12 10:07:44.303393 allianceauth-4.0.2/allianceauth/eveonline/views.py
+-rw-r--r--   0        0        0        0 2024-05-12 10:07:44.304393 allianceauth-4.0.2/allianceauth/fleetactivitytracking/__init__.py
+-rw-r--r--   0        0        0      156 2024-05-12 10:07:44.161393 allianceauth-4.0.2/allianceauth/fleetactivitytracking/admin.py
+-rw-r--r--   0        0        0      148 2024-05-12 10:07:44.161393 allianceauth-4.0.2/allianceauth/fleetactivitytracking/apps.py
+-rw-r--r--   0        0        0      494 2024-05-12 10:07:44.161393 allianceauth-4.0.2/allianceauth/fleetactivitytracking/auth_hooks.py
+-rw-r--r--   0        0        0      360 2024-05-12 10:07:44.161393 allianceauth-4.0.2/allianceauth/fleetactivitytracking/forms.py
+-rw-r--r--   0        0        0     2291 2024-05-12 10:07:44.161393 allianceauth-4.0.2/allianceauth/fleetactivitytracking/migrations/0001_initial.py
+-rw-r--r--   0        0        0      489 2024-05-12 10:07:44.161393 allianceauth-4.0.2/allianceauth/fleetactivitytracking/migrations/0002_auto_20160905_2220.py
+-rw-r--r--   0        0        0      460 2024-05-12 10:07:44.161393 allianceauth-4.0.2/allianceauth/fleetactivitytracking/migrations/0003_auto_20160906_2354.py
+-rw-r--r--   0        0        0      414 2024-05-12 10:07:44.162393 allianceauth-4.0.2/allianceauth/fleetactivitytracking/migrations/0004_make_strings_more_stringy.py
+-rw-r--r--   0        0        0      510 2024-05-12 10:07:44.162393 allianceauth-4.0.2/allianceauth/fleetactivitytracking/migrations/0005_remove_fat_name.py
+-rw-r--r--   0        0        0      397 2024-05-12 10:07:44.162393 allianceauth-4.0.2/allianceauth/fleetactivitytracking/migrations/0006_auto_20180803_0430.py
+-rw-r--r--   0        0        0      606 2024-05-12 10:07:44.162393 allianceauth-4.0.2/allianceauth/fleetactivitytracking/migrations/0007_sentinel_user.py
+-rw-r--r--   0        0        0        0 2024-05-12 10:07:44.311393 allianceauth-4.0.2/allianceauth/fleetactivitytracking/migrations/__init__.py
+-rw-r--r--   0        0        0     1122 2024-05-12 10:07:44.162393 allianceauth-4.0.2/allianceauth/fleetactivitytracking/models.py
+-rw-r--r--   0        0        0   947431 2024-05-12 10:07:44.164393 allianceauth-4.0.2/allianceauth/fleetactivitytracking/swagger.json
+-rw-r--r--   0        0        0     1851 2024-05-12 10:07:44.165393 allianceauth-4.0.2/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/characternotexisting.html
+-rw-r--r--   0        0        0     1880 2024-05-12 10:07:44.165393 allianceauth-4.0.2/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/fatlinkcreate.html
+-rw-r--r--   0        0        0     2811 2024-05-12 10:07:44.165393 allianceauth-4.0.2/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/fatlinkmodify.html
+-rw-r--r--   0        0        0     4516 2024-05-12 10:07:44.165393 allianceauth-4.0.2/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/fatlinkpersonalmonthlystatisticsview.html
+-rw-r--r--   0        0        0     1725 2024-05-12 10:07:44.165393 allianceauth-4.0.2/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/fatlinkpersonalstatisticsview.html
+-rw-r--r--   0        0        0     2730 2024-05-12 10:07:44.165393 allianceauth-4.0.2/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/fatlinkstatisticscorpview.html
+-rw-r--r--   0        0        0     3011 2024-05-12 10:07:44.165393 allianceauth-4.0.2/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/fatlinkstatisticsview.html
+-rw-r--r--   0        0        0     5912 2024-05-12 10:07:44.165393 allianceauth-4.0.2/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/fatlinkview.html
+-rw-r--r--   0        0        0     1386 2024-05-12 10:07:44.165393 allianceauth-4.0.2/allianceauth/fleetactivitytracking/urls.py
+-rw-r--r--   0        0        0    16656 2024-05-12 10:07:44.165393 allianceauth-4.0.2/allianceauth/fleetactivitytracking/views.py
+-rw-r--r--   0        0        0       32 2024-05-12 10:07:44.165393 allianceauth-4.0.2/allianceauth/framework/__init__.py
+-rw-r--r--   0        0        0     1421 2024-05-12 10:07:44.166393 allianceauth-4.0.2/allianceauth/framework/api/evecharacter.py
+-rw-r--r--   0        0        0     1723 2024-05-12 10:07:44.166393 allianceauth-4.0.2/allianceauth/framework/api/user.py
+-rw-r--r--   0        0        0      202 2024-05-12 10:07:44.166393 allianceauth-4.0.2/allianceauth/framework/apps.py
+-rw-r--r--   0        0        0     3174 2024-05-12 10:07:44.166393 allianceauth-4.0.2/allianceauth/framework/static/allianceauth/framework/css/auth-framework.css
+-rw-r--r--   0        0        0      336 2024-05-12 10:07:44.166393 allianceauth-4.0.2/allianceauth/framework/templates/framework/header/page-header.html
+-rw-r--r--   0        0        0       31 2024-05-12 10:07:44.166393 allianceauth-4.0.2/allianceauth/framework/tests/__init__.py
+-rw-r--r--   0        0        0     4468 2024-05-12 10:07:44.166393 allianceauth-4.0.2/allianceauth/framework/tests/test_api_user.py
+-rw-r--r--   0        0        0        0 2024-05-12 10:07:44.311393 allianceauth-4.0.2/allianceauth/groupmanagement/__init__.py
+-rw-r--r--   0        0        0     8978 2024-05-12 10:07:44.166393 allianceauth-4.0.2/allianceauth/groupmanagement/admin.py
+-rw-r--r--   0        0        0      252 2024-05-12 10:07:44.167393 allianceauth-4.0.2/allianceauth/groupmanagement/apps.py
+-rw-r--r--   0        0        0     2336 2024-05-12 10:07:44.167393 allianceauth-4.0.2/allianceauth/groupmanagement/auth_hooks.py
+-rw-r--r--   0        0        0     2466 2024-05-12 10:07:44.167393 allianceauth-4.0.2/allianceauth/groupmanagement/forms.py
+-rw-r--r--   0        0        0     4341 2024-05-12 10:07:44.167393 allianceauth-4.0.2/allianceauth/groupmanagement/managers.py
+-rw-r--r--   0        0        0     2243 2024-05-12 10:07:44.167393 allianceauth-4.0.2/allianceauth/groupmanagement/migrations/0001_initial.py
+-rw-r--r--   0        0        0      685 2024-05-12 10:07:44.167393 allianceauth-4.0.2/allianceauth/groupmanagement/migrations/0002_auto_20160906_2354.py
+-rw-r--r--   0        0        0      261 2024-05-12 10:07:44.167393 allianceauth-4.0.2/allianceauth/groupmanagement/migrations/0003_default_groups.py
+-rw-r--r--   0        0        0     4322 2024-05-12 10:07:44.167393 allianceauth-4.0.2/allianceauth/groupmanagement/migrations/0004_authgroup.py
+-rw-r--r--   0        0        0      631 2024-05-12 10:07:44.167393 allianceauth-4.0.2/allianceauth/groupmanagement/migrations/0005_authgroup_public.py
+-rw-r--r--   0        0        0      607 2024-05-12 10:07:44.167393 allianceauth-4.0.2/allianceauth/groupmanagement/migrations/0006_request_groups_perm.py
+-rw-r--r--   0        0        0      877 2024-05-12 10:07:44.167393 allianceauth-4.0.2/allianceauth/groupmanagement/migrations/0007_on_delete.py
+-rw-r--r--   0        0        0     1430 2024-05-12 10:07:44.167393 allianceauth-4.0.2/allianceauth/groupmanagement/migrations/0008_remove_authgroup_permissions.py
+-rw-r--r--   0        0        0     1100 2024-05-12 10:07:44.167393 allianceauth-4.0.2/allianceauth/groupmanagement/migrations/0009_requestlog.py
+-rw-r--r--   0        0        0      614 2024-05-12 10:07:44.167393 allianceauth-4.0.2/allianceauth/groupmanagement/migrations/0010_authgroup_states.py
+-rw-r--r--   0        0        0      456 2024-05-12 10:07:44.168393 allianceauth-4.0.2/allianceauth/groupmanagement/migrations/0011_requestlog_date.py
+-rw-r--r--   0        0        0      672 2024-05-12 10:07:44.168393 allianceauth-4.0.2/allianceauth/groupmanagement/migrations/0012_group_leads.py
+-rw-r--r--   0        0        0      397 2024-05-12 10:07:44.168393 allianceauth-4.0.2/allianceauth/groupmanagement/migrations/0013_fix_requestlog_date_field.py
+-rw-r--r--   0        0        0      410 2024-05-12 10:07:44.168393 allianceauth-4.0.2/allianceauth/groupmanagement/migrations/0014_auto_20200918_1412.py
+-rw-r--r--   0        0        0      567 2024-05-12 10:07:44.168393 allianceauth-4.0.2/allianceauth/groupmanagement/migrations/0015_make_descriptions_great_again.py
+-rw-r--r--   0        0        0      353 2024-05-12 10:07:44.168393 allianceauth-4.0.2/allianceauth/groupmanagement/migrations/0016_remove_grouprequest_status_field.py
+-rw-r--r--   0        0        0     2296 2024-05-12 10:07:44.168393 allianceauth-4.0.2/allianceauth/groupmanagement/migrations/0017_improve_groups_documentation.py
+-rw-r--r--   0        0        0     1082 2024-05-12 10:07:44.168393 allianceauth-4.0.2/allianceauth/groupmanagement/migrations/0018_reservedgroupname.py
+-rw-r--r--   0        0        0      520 2024-05-12 10:07:44.168393 allianceauth-4.0.2/allianceauth/groupmanagement/migrations/0019_adding_restricted_to_groups.py
+-rw-r--r--   0        0        0        0 2024-05-12 10:07:44.311393 allianceauth-4.0.2/allianceauth/groupmanagement/migrations/__init__.py
+-rw-r--r--   0        0        0     8132 2024-05-12 10:07:44.168393 allianceauth-4.0.2/allianceauth/groupmanagement/models.py
+-rw-r--r--   0        0        0     1465 2024-05-12 10:07:44.168393 allianceauth-4.0.2/allianceauth/groupmanagement/signals.py
+-rw-r--r--   0        0        0      333 2024-05-12 10:07:44.168393 allianceauth-4.0.2/allianceauth/groupmanagement/tasks.py
+-rw-r--r--   0        0        0     4516 2024-05-12 10:07:44.168393 allianceauth-4.0.2/allianceauth/groupmanagement/templates/groupmanagement/audit.html
+-rw-r--r--   0        0        0     4003 2024-05-12 10:07:44.169393 allianceauth-4.0.2/allianceauth/groupmanagement/templates/groupmanagement/groupmembers.html
+-rw-r--r--   0        0        0     3764 2024-05-12 10:07:44.169393 allianceauth-4.0.2/allianceauth/groupmanagement/templates/groupmanagement/groupmembership.html
+-rw-r--r--   0        0        0     4854 2024-05-12 10:07:44.169393 allianceauth-4.0.2/allianceauth/groupmanagement/templates/groupmanagement/groups.html
+-rw-r--r--   0        0        0     8485 2024-05-12 10:07:44.169393 allianceauth-4.0.2/allianceauth/groupmanagement/templates/groupmanagement/index.html
+-rw-r--r--   0        0        0      445 2024-05-12 10:07:44.169393 allianceauth-4.0.2/allianceauth/groupmanagement/templates/groupmanagement/menu.html
+-rw-r--r--   0        0        0      254 2024-05-12 10:07:44.169393 allianceauth-4.0.2/allianceauth/groupmanagement/tests/__init__.py
+-rw-r--r--   0        0        0    27572 2024-05-12 10:07:44.169393 allianceauth-4.0.2/allianceauth/groupmanagement/tests/test_admin.py
+-rw-r--r--   0        0        0    17375 2024-05-12 10:07:44.169393 allianceauth-4.0.2/allianceauth/groupmanagement/tests/test_managers.py
+-rw-r--r--   0        0        0    11668 2024-05-12 10:07:44.169393 allianceauth-4.0.2/allianceauth/groupmanagement/tests/test_models.py
+-rw-r--r--   0        0        0     4950 2024-05-12 10:07:44.170393 allianceauth-4.0.2/allianceauth/groupmanagement/tests/test_signals.py
+-rw-r--r--   0        0        0     3999 2024-05-12 10:07:44.170393 allianceauth-4.0.2/allianceauth/groupmanagement/tests/test_views.py
+-rw-r--r--   0        0        0     1651 2024-05-12 10:07:44.170393 allianceauth-4.0.2/allianceauth/groupmanagement/urls.py
+-rw-r--r--   0        0        0    20437 2024-05-12 10:07:44.170393 allianceauth-4.0.2/allianceauth/groupmanagement/views.py
+-rw-r--r--   0        0        0     4570 2024-05-12 10:07:44.170393 allianceauth-4.0.2/allianceauth/hooks.py
+-rw-r--r--   0        0        0        0 2024-05-12 10:07:44.319393 allianceauth-4.0.2/allianceauth/hrapplications/__init__.py
+-rw-r--r--   0        0        0      693 2024-05-12 10:07:44.170393 allianceauth-4.0.2/allianceauth/hrapplications/admin.py
+-rw-r--r--   0        0        0      145 2024-05-12 10:07:44.170393 allianceauth-4.0.2/allianceauth/hrapplications/apps.py
+-rw-r--r--   0        0        0     1023 2024-05-12 10:07:44.170393 allianceauth-4.0.2/allianceauth/hrapplications/auth_hooks.py
+-rw-r--r--   0        0        0      353 2024-05-12 10:07:44.170393 allianceauth-4.0.2/allianceauth/hrapplications/forms.py
+-rw-r--r--   0        0        0      900 2024-05-12 10:07:44.170393 allianceauth-4.0.2/allianceauth/hrapplications/managers.py
+-rw-r--r--   0        0        0     6662 2024-05-12 10:07:44.171393 allianceauth-4.0.2/allianceauth/hrapplications/migrations/0001_initial.py
+-rw-r--r--   0        0        0     1036 2024-05-12 10:07:44.171393 allianceauth-4.0.2/allianceauth/hrapplications/migrations/0002_choices_for_questions.py
+-rw-r--r--   0        0        0      415 2024-05-12 10:07:44.171393 allianceauth-4.0.2/allianceauth/hrapplications/migrations/0003_applicationquestion_multi_select.py
+-rw-r--r--   0        0        0     1461 2024-05-12 10:07:44.171393 allianceauth-4.0.2/allianceauth/hrapplications/migrations/0004_make_strings_more_stringy.py
+-rw-r--r--   0        0        0      558 2024-05-12 10:07:44.171393 allianceauth-4.0.2/allianceauth/hrapplications/migrations/0005_sorted_questions.py
+-rw-r--r--   0        0        0     1946 2024-05-12 10:07:44.171393 allianceauth-4.0.2/allianceauth/hrapplications/migrations/0006_remove_legacy_models.py
+-rw-r--r--   0        0        0      427 2024-05-12 10:07:44.171393 allianceauth-4.0.2/allianceauth/hrapplications/migrations/0007_auto_20200918_1412.py
+-rw-r--r--   0        0        0        0 2024-05-12 10:07:44.319393 allianceauth-4.0.2/allianceauth/hrapplications/migrations/__init__.py
+-rw-r--r--   0        0        0     3237 2024-05-12 10:07:44.171393 allianceauth-4.0.2/allianceauth/hrapplications/models.py
+-rw-r--r--   0        0        0     1411 2024-05-12 10:07:44.171393 allianceauth-4.0.2/allianceauth/hrapplications/templates/hrapplications/corpchoice.html
+-rw-r--r--   0        0        0     2946 2024-05-12 10:07:44.171393 allianceauth-4.0.2/allianceauth/hrapplications/templates/hrapplications/create.html
+-rw-r--r--   0        0        0    12438 2024-05-12 10:07:44.171393 allianceauth-4.0.2/allianceauth/hrapplications/templates/hrapplications/management.html
+-rw-r--r--   0        0        0     1308 2024-05-12 10:07:44.172393 allianceauth-4.0.2/allianceauth/hrapplications/templates/hrapplications/partials/modals/search.html
+-rw-r--r--   0        0        0     2772 2024-05-12 10:07:44.172393 allianceauth-4.0.2/allianceauth/hrapplications/templates/hrapplications/searchview.html
+-rw-r--r--   0        0        0     8251 2024-05-12 10:07:44.172393 allianceauth-4.0.2/allianceauth/hrapplications/templates/hrapplications/view.html
+-rw-r--r--   0        0        0     4165 2024-05-12 10:07:44.172393 allianceauth-4.0.2/allianceauth/hrapplications/tests.py
+-rw-r--r--   0        0        0     1113 2024-05-12 10:07:44.172393 allianceauth-4.0.2/allianceauth/hrapplications/urls.py
+-rw-r--r--   0        0        0    12011 2024-05-12 10:07:44.172393 allianceauth-4.0.2/allianceauth/hrapplications/views.py
+-rw-r--r--   0        0        0     7262 2024-05-12 10:07:44.172393 allianceauth-4.0.2/allianceauth/locale/cs/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    85931 2024-05-12 10:07:44.173393 allianceauth-4.0.2/allianceauth/locale/cs/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    45125 2024-05-12 10:07:44.174393 allianceauth-4.0.2/allianceauth/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0   100544 2024-05-12 10:07:44.174393 allianceauth-4.0.2/allianceauth/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      380 2024-05-12 10:07:44.174393 allianceauth-4.0.2/allianceauth/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    83238 2024-05-12 10:07:44.175393 allianceauth-4.0.2/allianceauth/locale/en/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    35108 2024-05-12 10:07:44.175393 allianceauth-4.0.2/allianceauth/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    96583 2024-05-12 10:07:44.175393 allianceauth-4.0.2/allianceauth/locale/es/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    46059 2024-05-12 10:07:44.176393 allianceauth-4.0.2/allianceauth/locale/fr_FR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0   101728 2024-05-12 10:07:44.176393 allianceauth-4.0.2/allianceauth/locale/fr_FR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    44568 2024-05-12 10:07:44.177393 allianceauth-4.0.2/allianceauth/locale/it_IT/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0   100475 2024-05-12 10:07:44.177393 allianceauth-4.0.2/allianceauth/locale/it_IT/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    49616 2024-05-12 10:07:44.177393 allianceauth-4.0.2/allianceauth/locale/ja/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0   104822 2024-05-12 10:07:44.178393 allianceauth-4.0.2/allianceauth/locale/ja/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    46390 2024-05-12 10:07:44.178393 allianceauth-4.0.2/allianceauth/locale/ko_KR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0   101738 2024-05-12 10:07:44.178393 allianceauth-4.0.2/allianceauth/locale/ko_KR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    17293 2024-05-12 10:07:44.179393 allianceauth-4.0.2/allianceauth/locale/nl/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    88812 2024-05-12 10:07:44.179393 allianceauth-4.0.2/allianceauth/locale/nl/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    45885 2024-05-12 10:07:44.179393 allianceauth-4.0.2/allianceauth/locale/pl_PL/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0   101247 2024-05-12 10:07:44.179393 allianceauth-4.0.2/allianceauth/locale/pl_PL/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    45746 2024-05-12 10:07:44.180393 allianceauth-4.0.2/allianceauth/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0   106362 2024-05-12 10:07:44.180393 allianceauth-4.0.2/allianceauth/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    57333 2024-05-12 10:07:44.181393 allianceauth-4.0.2/allianceauth/locale/uk/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0   112781 2024-05-12 10:07:44.181393 allianceauth-4.0.2/allianceauth/locale/uk/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    26591 2024-05-12 10:07:44.181393 allianceauth-4.0.2/allianceauth/locale/zh_Hans/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    92036 2024-05-12 10:07:44.182393 allianceauth-4.0.2/allianceauth/locale/zh_Hans/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0        0 2024-05-12 10:07:44.319393 allianceauth-4.0.2/allianceauth/menu/__init__.py
+-rw-r--r--   0        0        0     3721 2024-05-12 10:07:44.182393 allianceauth-4.0.2/allianceauth/menu/admin.py
+-rw-r--r--   0        0        0      459 2024-05-12 10:07:44.182393 allianceauth-4.0.2/allianceauth/menu/apps.py
+-rw-r--r--   0        0        0      485 2024-05-12 10:07:44.182393 allianceauth-4.0.2/allianceauth/menu/constants.py
+-rw-r--r--   0        0        0        0 2024-05-12 10:07:44.319393 allianceauth-4.0.2/allianceauth/menu/core/__init__.py
+-rw-r--r--   0        0        0     1363 2024-05-12 10:07:44.182393 allianceauth-4.0.2/allianceauth/menu/core/menu_item_hooks.py
+-rw-r--r--   0        0        0      892 2024-05-12 10:07:44.182393 allianceauth-4.0.2/allianceauth/menu/core/smart_sync.py
+-rw-r--r--   0        0        0      688 2024-05-12 10:07:44.182393 allianceauth-4.0.2/allianceauth/menu/filters.py
+-rw-r--r--   0        0        0     1397 2024-05-12 10:07:44.182393 allianceauth-4.0.2/allianceauth/menu/forms.py
+-rw-r--r--   0        0        0     1932 2024-05-12 10:07:44.182393 allianceauth-4.0.2/allianceauth/menu/hooks.py
+-rw-r--r--   0        0        0     2288 2024-05-12 10:07:44.182393 allianceauth-4.0.2/allianceauth/menu/managers.py
+-rw-r--r--   0        0        0     3143 2024-05-12 10:07:44.182393 allianceauth-4.0.2/allianceauth/menu/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2024-05-12 10:07:44.320393 allianceauth-4.0.2/allianceauth/menu/migrations/__init__.py
+-rw-r--r--   0        0        0     4094 2024-05-12 10:07:44.182393 allianceauth-4.0.2/allianceauth/menu/models.py
+-rw-r--r--   0        0        0      289 2024-05-12 10:07:44.183393 allianceauth-4.0.2/allianceauth/menu/templates/admin/menu/menuitem/change_list.html
+-rw-r--r--   0        0        0       62 2024-05-12 10:07:44.183393 allianceauth-4.0.2/allianceauth/menu/templates/menu/menu-block.html
+-rw-r--r--   0        0        0     2009 2024-05-12 10:07:44.183393 allianceauth-4.0.2/allianceauth/menu/templates/menu/menu-item-bs5.html
+-rw-r--r--   0        0        0      101 2024-05-12 10:07:44.183393 allianceauth-4.0.2/allianceauth/menu/templates/menu/menu-logo.html
+-rw-r--r--   0        0        0      535 2024-05-12 10:07:44.183393 allianceauth-4.0.2/allianceauth/menu/templates/menu/menu-notification-block.html
+-rw-r--r--   0        0        0     5068 2024-05-12 10:07:44.183393 allianceauth-4.0.2/allianceauth/menu/templates/menu/menu-user.html
+-rw-r--r--   0        0        0     1308 2024-05-12 10:07:44.183393 allianceauth-4.0.2/allianceauth/menu/templates/menu/sortable-side-menu.html
+-rw-r--r--   0        0        0        0 2024-05-12 10:07:44.320393 allianceauth-4.0.2/allianceauth/menu/templatetags/__init__.py
+-rw-r--r--   0        0        0      893 2024-05-12 10:07:44.183393 allianceauth-4.0.2/allianceauth/menu/templatetags/menu_items.py
+-rw-r--r--   0        0        0     5996 2024-05-12 10:07:44.183393 allianceauth-4.0.2/allianceauth/menu/templatetags/menu_menu_items.py
+-rw-r--r--   0        0        0        0 2024-05-12 10:07:44.320393 allianceauth-4.0.2/allianceauth/menu/tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-12 10:07:44.320393 allianceauth-4.0.2/allianceauth/menu/tests/core/__init__.py
+-rw-r--r--   0        0        0     1799 2024-05-12 10:07:44.184393 allianceauth-4.0.2/allianceauth/menu/tests/core/test_menu_item_hooks.py
+-rw-r--r--   0        0        0     1153 2024-05-12 10:07:44.184393 allianceauth-4.0.2/allianceauth/menu/tests/core/test_smart_sync.py
+-rw-r--r--   0        0        0     2763 2024-05-12 10:07:44.184393 allianceauth-4.0.2/allianceauth/menu/tests/factories.py
+-rw-r--r--   0        0        0        0 2024-05-12 10:07:44.320393 allianceauth-4.0.2/allianceauth/menu/tests/integration/__init__.py
+-rw-r--r--   0        0        0     6367 2024-05-12 10:07:44.184393 allianceauth-4.0.2/allianceauth/menu/tests/integration/test_admin.py
+-rw-r--r--   0        0        0     3736 2024-05-12 10:07:44.184393 allianceauth-4.0.2/allianceauth/menu/tests/integration/test_dashboard.py
+-rw-r--r--   0        0        0        0 2024-05-12 10:07:44.320393 allianceauth-4.0.2/allianceauth/menu/tests/templatetags/__init__.py
+-rw-r--r--   0        0        0     1688 2024-05-12 10:07:44.184393 allianceauth-4.0.2/allianceauth/menu/tests/templatetags/test_menu_items.py
+-rw-r--r--   0        0        0    11656 2024-05-12 10:07:44.184393 allianceauth-4.0.2/allianceauth/menu/tests/templatetags/test_menu_menu_items.py
+-rw-r--r--   0        0        0      833 2024-05-12 10:07:44.184393 allianceauth-4.0.2/allianceauth/menu/tests/test_forms.py
+-rw-r--r--   0        0        0     2511 2024-05-12 10:07:44.184393 allianceauth-4.0.2/allianceauth/menu/tests/test_hooks.py
+-rw-r--r--   0        0        0     3470 2024-05-12 10:07:44.184393 allianceauth-4.0.2/allianceauth/menu/tests/test_managers.py
+-rw-r--r--   0        0        0     4831 2024-05-12 10:07:44.184393 allianceauth-4.0.2/allianceauth/menu/tests/test_models.py
+-rw-r--r--   0        0        0     1177 2024-05-12 10:07:44.185393 allianceauth-4.0.2/allianceauth/menu/tests/utils.py
+-rw-r--r--   0        0        0        0 2024-05-12 10:07:44.320393 allianceauth-4.0.2/allianceauth/models.py
+-rw-r--r--   0        0        0       39 2024-05-12 10:07:44.185393 allianceauth-4.0.2/allianceauth/notifications/__init__.py
+-rw-r--r--   0        0        0     1138 2024-05-12 10:07:44.185393 allianceauth-4.0.2/allianceauth/notifications/admin.py
+-rw-r--r--   0        0        0      142 2024-05-12 10:07:44.185393 allianceauth-4.0.2/allianceauth/notifications/apps.py
+-rw-r--r--   0        0        0     1320 2024-05-12 10:07:44.185393 allianceauth-4.0.2/allianceauth/notifications/core.py
+-rw-r--r--   0        0        0      998 2024-05-12 10:07:44.185393 allianceauth-4.0.2/allianceauth/notifications/handlers.py
+-rw-r--r--   0        0        0     3907 2024-05-12 10:07:44.185393 allianceauth-4.0.2/allianceauth/notifications/managers.py
+-rw-r--r--   0        0        0     1117 2024-05-12 10:07:44.185393 allianceauth-4.0.2/allianceauth/notifications/migrations/0001_initial.py
+-rw-r--r--   0        0        0      353 2024-05-12 10:07:44.185393 allianceauth-4.0.2/allianceauth/notifications/migrations/0002_auto_20160910_1649.py
+-rw-r--r--   0        0        0      514 2024-05-12 10:07:44.185393 allianceauth-4.0.2/allianceauth/notifications/migrations/0003_make_strings_more_stringy.py
+-rw-r--r--   0        0        0      714 2024-05-12 10:07:44.185393 allianceauth-4.0.2/allianceauth/notifications/migrations/0004_performance_tuning.py
+-rw-r--r--   0        0        0      512 2024-05-12 10:07:44.185393 allianceauth-4.0.2/allianceauth/notifications/migrations/0005_fix_level_choices.py
+-rw-r--r--   0        0        0        0 2024-05-12 10:07:44.329393 allianceauth-4.0.2/allianceauth/notifications/migrations/__init__.py
+-rw-r--r--   0        0        0     2772 2024-05-12 10:07:44.185393 allianceauth-4.0.2/allianceauth/notifications/models.py
+-rw-r--r--   0        0        0     1857 2024-05-12 10:07:44.186393 allianceauth-4.0.2/allianceauth/notifications/templates/notifications/list.html
+-rw-r--r--   0        0        0     1070 2024-05-12 10:07:44.186393 allianceauth-4.0.2/allianceauth/notifications/templates/notifications/list_partial.html
+-rw-r--r--   0        0        0      736 2024-05-12 10:07:44.186393 allianceauth-4.0.2/allianceauth/notifications/templates/notifications/view.html
+-rw-r--r--   0        0        0        0 2024-05-12 10:07:44.329393 allianceauth-4.0.2/allianceauth/notifications/templatetags/__init__.py
+-rw-r--r--   0        0        0     1156 2024-05-12 10:07:44.186393 allianceauth-4.0.2/allianceauth/notifications/templatetags/auth_notifications.py
+-rw-r--r--   0        0        0        0 2024-05-12 10:07:44.329393 allianceauth-4.0.2/allianceauth/notifications/tests/__init__.py
+-rw-r--r--   0        0        0     3073 2024-05-12 10:07:44.186393 allianceauth-4.0.2/allianceauth/notifications/tests/test_core.py
+-rw-r--r--   0        0        0     2392 2024-05-12 10:07:44.186393 allianceauth-4.0.2/allianceauth/notifications/tests/test_handlers.py
+-rw-r--r--   0        0        0     1120 2024-05-12 10:07:44.186393 allianceauth-4.0.2/allianceauth/notifications/tests/test_init.py
+-rw-r--r--   0        0        0     9437 2024-05-12 10:07:44.186393 allianceauth-4.0.2/allianceauth/notifications/tests/test_managers.py
+-rw-r--r--   0        0        0     2398 2024-05-12 10:07:44.186393 allianceauth-4.0.2/allianceauth/notifications/tests/test_models.py
+-rw-r--r--   0        0        0     2975 2024-05-12 10:07:44.186393 allianceauth-4.0.2/allianceauth/notifications/tests/test_templatetags.py
+-rw-r--r--   0        0        0     1463 2024-05-12 10:07:44.187393 allianceauth-4.0.2/allianceauth/notifications/tests/test_views.py
+-rw-r--r--   0        0        0      674 2024-05-12 10:07:44.187393 allianceauth-4.0.2/allianceauth/notifications/urls.py
+-rw-r--r--   0        0        0     3522 2024-05-12 10:07:44.187393 allianceauth-4.0.2/allianceauth/notifications/views.py
+-rw-r--r--   0        0        0        0 2024-05-12 10:07:44.329393 allianceauth-4.0.2/allianceauth/optimer/__init__.py
+-rw-r--r--   0        0        0      158 2024-05-12 10:07:44.187393 allianceauth-4.0.2/allianceauth/optimer/admin.py
+-rw-r--r--   0        0        0      124 2024-05-12 10:07:44.187393 allianceauth-4.0.2/allianceauth/optimer/apps.py
+-rw-r--r--   0        0        0     1183 2024-05-12 10:07:44.187393 allianceauth-4.0.2/allianceauth/optimer/auth_hooks.py
+-rw-r--r--   0        0        0     1368 2024-05-12 10:07:44.187393 allianceauth-4.0.2/allianceauth/optimer/form.py
+-rw-r--r--   0        0        0     1047 2024-05-12 10:07:44.187393 allianceauth-4.0.2/allianceauth/optimer/form_widgets.py
+-rw-r--r--   0        0        0     1452 2024-05-12 10:07:44.187393 allianceauth-4.0.2/allianceauth/optimer/migrations/0001_initial.py
+-rw-r--r--   0        0        0      424 2024-05-12 10:07:44.187393 allianceauth-4.0.2/allianceauth/optimer/migrations/0002_auto_20170413_0442.py
+-rw-r--r--   0        0        0     1076 2024-05-12 10:07:44.187393 allianceauth-4.0.2/allianceauth/optimer/migrations/0003_make_strings_more_stringy.py
+-rw-r--r--   0        0        0      507 2024-05-12 10:07:44.187393 allianceauth-4.0.2/allianceauth/optimer/migrations/0004_on_delete.py
+-rw-r--r--   0        0        0     1447 2024-05-12 10:07:44.187393 allianceauth-4.0.2/allianceauth/optimer/migrations/0005_add_type_and_description.py
+-rw-r--r--   0        0        0        0 2024-05-12 10:07:44.329393 allianceauth-4.0.2/allianceauth/optimer/migrations/__init__.py
+-rw-r--r--   0        0        0     1247 2024-05-12 10:07:44.187393 allianceauth-4.0.2/allianceauth/optimer/models.py
+-rw-r--r--   0        0        0     1980 2024-05-12 10:07:44.188393 allianceauth-4.0.2/allianceauth/optimer/templates/optimer/add.html
+-rw-r--r--   0        0        0     1803 2024-05-12 10:07:44.188393 allianceauth-4.0.2/allianceauth/optimer/templates/optimer/dashboard.ops.html
+-rw-r--r--   0        0        0     2612 2024-05-12 10:07:44.188393 allianceauth-4.0.2/allianceauth/optimer/templates/optimer/fleetoptable.html
+-rw-r--r--   0        0        0     4378 2024-05-12 10:07:44.188393 allianceauth-4.0.2/allianceauth/optimer/templates/optimer/management.html
+-rw-r--r--   0        0        0     1986 2024-05-12 10:07:44.188393 allianceauth-4.0.2/allianceauth/optimer/templates/optimer/update.html
+-rw-r--r--   0        0        0       26 2024-05-12 10:07:44.188393 allianceauth-4.0.2/allianceauth/optimer/tests.py
+-rw-r--r--   0        0        0      336 2024-05-12 10:07:44.188393 allianceauth-4.0.2/allianceauth/optimer/urls.py
+-rw-r--r--   0        0        0     7139 2024-05-12 10:07:44.188393 allianceauth-4.0.2/allianceauth/optimer/views.py
+-rw-r--r--   0        0        0        0 2024-05-12 10:07:44.329393 allianceauth-4.0.2/allianceauth/permissions_tool/__init__.py
+-rw-r--r--   0        0        0      150 2024-05-12 10:07:44.188393 allianceauth-4.0.2/allianceauth/permissions_tool/apps.py
+-rw-r--r--   0        0        0      821 2024-05-12 10:07:44.188393 allianceauth-4.0.2/allianceauth/permissions_tool/auth_hooks.py
+-rw-r--r--   0        0        0      589 2024-05-12 10:07:44.189393 allianceauth-4.0.2/allianceauth/permissions_tool/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2024-05-12 10:07:44.329393 allianceauth-4.0.2/allianceauth/permissions_tool/migrations/__init__.py
+-rw-r--r--   0        0        0      258 2024-05-12 10:07:44.189393 allianceauth-4.0.2/allianceauth/permissions_tool/models.py
+-rw-r--r--   0        0        0     3874 2024-05-12 10:07:44.189393 allianceauth-4.0.2/allianceauth/permissions_tool/templates/permissions_tool/audit.html
+-rw-r--r--   0        0        0      789 2024-05-12 10:07:44.189393 allianceauth-4.0.2/allianceauth/permissions_tool/templates/permissions_tool/audit_row.html
+-rw-r--r--   0        0        0     4553 2024-05-12 10:07:44.189393 allianceauth-4.0.2/allianceauth/permissions_tool/templates/permissions_tool/overview.html
+-rw-r--r--   0        0        0     5067 2024-05-12 10:07:44.189393 allianceauth-4.0.2/allianceauth/permissions_tool/tests.py
+-rw-r--r--   0        0        0      340 2024-05-12 10:07:44.189393 allianceauth-4.0.2/allianceauth/permissions_tool/urls.py
+-rw-r--r--   0        0        0     2610 2024-05-12 10:07:44.189393 allianceauth-4.0.2/allianceauth/permissions_tool/views.py
+-rw-r--r--   0        0        0        0 2024-05-12 10:07:44.330393 allianceauth-4.0.2/allianceauth/project_template/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-12 10:07:44.330393 allianceauth-4.0.2/allianceauth/project_template/log/.gitkeep
+-rw-r--r--   0        0        0      821 2024-05-12 10:07:44.189393 allianceauth-4.0.2/allianceauth/project_template/manage.py
+-rw-r--r--   0        0        0       38 2024-05-12 10:07:44.190393 allianceauth-4.0.2/allianceauth/project_template/project_name/__init__.py
+-rw-r--r--   0        0        0     1417 2024-05-12 10:07:44.190393 allianceauth-4.0.2/allianceauth/project_template/project_name/celery.py
+-rw-r--r--   0        0        0        0 2024-05-12 10:07:44.330393 allianceauth-4.0.2/allianceauth/project_template/project_name/settings/__init__.py
+-rw-r--r--   0        0        0     9169 2024-05-12 10:07:44.190393 allianceauth-4.0.2/allianceauth/project_template/project_name/settings/base.py
+-rw-r--r--   0        0        0     3260 2024-05-12 10:07:44.190393 allianceauth-4.0.2/allianceauth/project_template/project_name/settings/local.py
+-rw-r--r--   0        0        0        0 2024-05-12 10:07:44.339393 allianceauth-4.0.2/allianceauth/project_template/project_name/static/.gitkeep
+-rw-r--r--   0        0        0        0 2024-05-12 10:07:44.339393 allianceauth-4.0.2/allianceauth/project_template/project_name/templates/.gitkeep
+-rw-r--r--   0        0        0      329 2024-05-12 10:07:44.190393 allianceauth-4.0.2/allianceauth/project_template/project_name/urls.py
+-rw-r--r--   0        0        0      432 2024-05-12 10:07:44.190393 allianceauth-4.0.2/allianceauth/project_template/project_name/wsgi.py
+-rw-r--r--   0        0        0     1408 2024-05-12 10:07:44.190393 allianceauth-4.0.2/allianceauth/project_template/supervisor.conf
+-rw-r--r--   0        0        0        0 2024-05-12 10:07:44.339393 allianceauth-4.0.2/allianceauth/services/__init__.py
+-rw-r--r--   0        0        0     3954 2024-05-12 10:07:44.190393 allianceauth-4.0.2/allianceauth/services/abstract.py
+-rw-r--r--   0        0        0     2162 2024-05-12 10:07:44.190393 allianceauth-4.0.2/allianceauth/services/admin.py
+-rw-r--r--   0        0        0      179 2024-05-12 10:07:44.191393 allianceauth-4.0.2/allianceauth/services/apps.py
+-rw-r--r--   0        0        0      662 2024-05-12 10:07:44.191393 allianceauth-4.0.2/allianceauth/services/auth_hooks.py
+-rw-r--r--   0        0        0     2117 2024-05-12 10:07:44.191393 allianceauth-4.0.2/allianceauth/services/forms.py
+-rw-r--r--   0        0        0     9149 2024-05-12 10:07:44.191393 allianceauth-4.0.2/allianceauth/services/hooks.py
+-rw-r--r--   0        0        0        0 2024-05-12 10:07:44.339393 allianceauth-4.0.2/allianceauth/services/management/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-12 10:07:44.339393 allianceauth-4.0.2/allianceauth/services/management/commands/__init__.py
+-rw-r--r--   0        0        0      469 2024-05-12 10:07:44.191393 allianceauth-4.0.2/allianceauth/services/management/commands/verify_service_accounts.py
+-rw-r--r--   0        0        0      483 2024-05-12 10:07:44.191393 allianceauth-4.0.2/allianceauth/services/migrations/0001_squashed_0003_delete_groupcache.py
+-rw-r--r--   0        0        0     1220 2024-05-12 10:07:44.191393 allianceauth-4.0.2/allianceauth/services/migrations/0002_nameformatter.py
+-rw-r--r--   0        0        0      522 2024-05-12 10:07:44.191393 allianceauth-4.0.2/allianceauth/services/migrations/0003_remove_broken_link.py
+-rw-r--r--   0        0        0        0 2024-05-12 10:07:44.339393 allianceauth-4.0.2/allianceauth/services/migrations/__init__.py
+-rw-r--r--   0        0        0     1000 2024-05-12 10:07:44.191393 allianceauth-4.0.2/allianceauth/services/models.py
+-rw-r--r--   0        0        0        0 2024-05-12 10:07:44.339393 allianceauth-4.0.2/allianceauth/services/modules/__init__.py
+-rw-r--r--   0        0        0       30 2024-05-12 10:07:44.192393 allianceauth-4.0.2/allianceauth/services/modules/discord/__init__.py
+-rw-r--r--   0        0        0     1070 2024-05-12 10:07:44.192393 allianceauth-4.0.2/allianceauth/services/modules/discord/admin.py
+-rw-r--r--   0        0        0     1290 2024-05-12 10:07:44.192393 allianceauth-4.0.2/allianceauth/services/modules/discord/api.py
+-rw-r--r--   0        0        0     1062 2024-05-12 10:07:44.192393 allianceauth-4.0.2/allianceauth/services/modules/discord/app_settings.py
+-rw-r--r--   0        0        0      148 2024-05-12 10:07:44.192393 allianceauth-4.0.2/allianceauth/services/modules/discord/apps.py
+-rw-r--r--   0        0        0     5974 2024-05-12 10:07:44.192393 allianceauth-4.0.2/allianceauth/services/modules/discord/auth_hooks.py
+-rw-r--r--   0        0        0     4446 2024-05-12 10:07:44.192393 allianceauth-4.0.2/allianceauth/services/modules/discord/core.py
+-rw-r--r--   0        0        0      372 2024-05-12 10:07:44.192393 allianceauth-4.0.2/allianceauth/services/modules/discord/discord_client/__init__.py
+-rw-r--r--   0        0        0     1681 2024-05-12 10:07:44.192393 allianceauth-4.0.2/allianceauth/services/modules/discord/discord_client/app_settings.py
+-rw-r--r--   0        0        0    28997 2024-05-12 10:07:44.192393 allianceauth-4.0.2/allianceauth/services/modules/discord/discord_client/client.py
+-rw-r--r--   0        0        0     1009 2024-05-12 10:07:44.192393 allianceauth-4.0.2/allianceauth/services/modules/discord/discord_client/exceptions.py
+-rw-r--r--   0        0        0     4590 2024-05-12 10:07:44.192393 allianceauth-4.0.2/allianceauth/services/modules/discord/discord_client/helpers.py
+-rw-r--r--   0        0        0     3853 2024-05-12 10:07:44.193393 allianceauth-4.0.2/allianceauth/services/modules/discord/discord_client/models.py
+-rw-r--r--   0        0        0        0 2024-05-12 10:07:44.339393 allianceauth-4.0.2/allianceauth/services/modules/discord/discord_client/tests/__init__.py
+-rw-r--r--   0        0        0     5027 2024-05-12 10:07:44.193393 allianceauth-4.0.2/allianceauth/services/modules/discord/discord_client/tests/example_objects.json
+-rw-r--r--   0        0        0     3013 2024-05-12 10:07:44.193393 allianceauth-4.0.2/allianceauth/services/modules/discord/discord_client/tests/factories.py
+-rw-r--r--   0        0        0     2784 2024-05-12 10:07:44.193393 allianceauth-4.0.2/allianceauth/services/modules/discord/discord_client/tests/piloting_concurrency.py
+-rw-r--r--   0        0        0     4477 2024-05-12 10:07:44.193393 allianceauth-4.0.2/allianceauth/services/modules/discord/discord_client/tests/piloting_functionality.py
+-rw-r--r--   0        0        0      904 2024-05-12 10:07:44.193393 allianceauth-4.0.2/allianceauth/services/modules/discord/discord_client/tests/rate_limits.md
+-rw-r--r--   0        0        0    56114 2024-05-12 10:07:44.193393 allianceauth-4.0.2/allianceauth/services/modules/discord/discord_client/tests/test_client.py
+-rw-r--r--   0        0        0     1045 2024-05-12 10:07:44.193393 allianceauth-4.0.2/allianceauth/services/modules/discord/discord_client/tests/test_exceptions.py
+-rw-r--r--   0        0        0     9724 2024-05-12 10:07:44.193393 allianceauth-4.0.2/allianceauth/services/modules/discord/discord_client/tests/test_helpers.py
+-rw-r--r--   0        0        0     4966 2024-05-12 10:07:44.194393 allianceauth-4.0.2/allianceauth/services/modules/discord/discord_client/tests/test_models.py
+-rw-r--r--   0        0        0     6281 2024-05-12 10:07:44.194393 allianceauth-4.0.2/allianceauth/services/modules/discord/managers.py
+-rw-r--r--   0        0        0      680 2024-05-12 10:07:44.194393 allianceauth-4.0.2/allianceauth/services/modules/discord/migrations/0001_initial.py
+-rw-r--r--   0        0        0     2067 2024-05-12 10:07:44.194393 allianceauth-4.0.2/allianceauth/services/modules/discord/migrations/0002_service_permissions.py
+-rw-r--r--   0        0        0     1538 2024-05-12 10:07:44.194393 allianceauth-4.0.2/allianceauth/services/modules/discord/migrations/0003_big_overhaul.py
+-rw-r--r--   0        0        0        0 2024-05-12 10:07:44.339393 allianceauth-4.0.2/allianceauth/services/modules/discord/migrations/__init__.py
+-rw-r--r--   0        0        0     7138 2024-05-12 10:07:44.194393 allianceauth-4.0.2/allianceauth/services/modules/discord/models.py
+-rw-r--r--   0        0        0     9517 2024-05-12 10:07:44.194393 allianceauth-4.0.2/allianceauth/services/modules/discord/tasks.py
+-rw-r--r--   0        0        0     1508 2024-05-12 10:07:44.194393 allianceauth-4.0.2/allianceauth/services/modules/discord/templates/services/discord/discord_service_ctrl.html
+-rw-r--r--   0        0        0      480 2024-05-12 10:07:44.194393 allianceauth-4.0.2/allianceauth/services/modules/discord/tests/__init__.py
+-rw-r--r--   0        0        0      917 2024-05-12 10:07:44.194393 allianceauth-4.0.2/allianceauth/services/modules/discord/tests/factories.py
+-rw-r--r--   0        0        0     2639 2024-05-12 10:07:44.195393 allianceauth-4.0.2/allianceauth/services/modules/discord/tests/piloting_tasks.py
+-rw-r--r--   0        0        0    10400 2024-05-12 10:07:44.195393 allianceauth-4.0.2/allianceauth/services/modules/discord/tests/test_admin.py
+-rw-r--r--   0        0        0      525 2024-05-12 10:07:44.195393 allianceauth-4.0.2/allianceauth/services/modules/discord/tests/test_api.py
+-rw-r--r--   0        0        0     7200 2024-05-12 10:07:44.195393 allianceauth-4.0.2/allianceauth/services/modules/discord/tests/test_auth_hooks.py
+-rw-r--r--   0        0        0     8456 2024-05-12 10:07:44.195393 allianceauth-4.0.2/allianceauth/services/modules/discord/tests/test_core.py
+-rw-r--r--   0        0        0    29715 2024-05-12 10:07:44.195393 allianceauth-4.0.2/allianceauth/services/modules/discord/tests/test_integration.py
+-rw-r--r--   0        0        0    19956 2024-05-12 10:07:44.195393 allianceauth-4.0.2/allianceauth/services/modules/discord/tests/test_managers.py
+-rw-r--r--   0        0        0    11474 2024-05-12 10:07:44.195393 allianceauth-4.0.2/allianceauth/services/modules/discord/tests/test_models.py
+-rw-r--r--   0        0        0    17995 2024-05-12 10:07:44.196393 allianceauth-4.0.2/allianceauth/services/modules/discord/tests/test_tasks.py
+-rw-r--r--   0        0        0     3201 2024-05-12 10:07:44.196393 allianceauth-4.0.2/allianceauth/services/modules/discord/tests/test_utils.py
+-rw-r--r--   0        0        0     6783 2024-05-12 10:07:44.196393 allianceauth-4.0.2/allianceauth/services/modules/discord/tests/test_views.py
+-rw-r--r--   0        0        0      538 2024-05-12 10:07:44.196393 allianceauth-4.0.2/allianceauth/services/modules/discord/urls.py
+-rw-r--r--   0        0        0     2561 2024-05-12 10:07:44.196393 allianceauth-4.0.2/allianceauth/services/modules/discord/utils.py
+-rw-r--r--   0        0        0     3635 2024-05-12 10:07:44.196393 allianceauth-4.0.2/allianceauth/services/modules/discord/views.py
+-rw-r--r--   0        0        0        0 2024-05-12 10:07:44.339393 allianceauth-4.0.2/allianceauth/services/modules/discourse/__init__.py
+-rw-r--r--   0        0        0      264 2024-05-12 10:07:44.196393 allianceauth-4.0.2/allianceauth/services/modules/discourse/admin.py
+-rw-r--r--   0        0        0      154 2024-05-12 10:07:44.196393 allianceauth-4.0.2/allianceauth/services/modules/discourse/apps.py
+-rw-r--r--   0        0        0     1878 2024-05-12 10:07:44.196393 allianceauth-4.0.2/allianceauth/services/modules/discourse/auth_hooks.py
+-rw-r--r--   0        0        0     7039 2024-05-12 10:07:44.196393 allianceauth-4.0.2/allianceauth/services/modules/discourse/manager.py
+-rw-r--r--   0        0        0      677 2024-05-12 10:07:44.197393 allianceauth-4.0.2/allianceauth/services/modules/discourse/migrations/0001_initial.py
+-rw-r--r--   0        0        0     2096 2024-05-12 10:07:44.197393 allianceauth-4.0.2/allianceauth/services/modules/discourse/migrations/0002_service_permissions.py
+-rw-r--r--   0        0        0        0 2024-05-12 10:07:44.343393 allianceauth-4.0.2/allianceauth/services/modules/discourse/migrations/__init__.py
+-rw-r--r--   0        0        0      529 2024-05-12 10:07:44.197393 allianceauth-4.0.2/allianceauth/services/modules/discourse/models.py
+-rw-r--r--   0        0        0      533 2024-05-12 10:07:44.197393 allianceauth-4.0.2/allianceauth/services/modules/discourse/providers.py
+-rw-r--r--   0        0        0     2276 2024-05-12 10:07:44.197393 allianceauth-4.0.2/allianceauth/services/modules/discourse/tasks.py
+-rw-r--r--   0        0        0      663 2024-05-12 10:07:44.197393 allianceauth-4.0.2/allianceauth/services/modules/discourse/templates/services/discourse/discourse_service_ctrl.html
+-rw-r--r--   0        0        0     5209 2024-05-12 10:07:44.197393 allianceauth-4.0.2/allianceauth/services/modules/discourse/tests.py
+-rw-r--r--   0        0        0      176 2024-05-12 10:07:44.197393 allianceauth-4.0.2/allianceauth/services/modules/discourse/urls.py
+-rw-r--r--   0        0        0     3486 2024-05-12 10:07:44.197393 allianceauth-4.0.2/allianceauth/services/modules/discourse/views.py
+-rw-r--r--   0        0        0        0 2024-05-12 10:07:44.343393 allianceauth-4.0.2/allianceauth/services/modules/example/__init__.py
+-rw-r--r--   0        0        0      156 2024-05-12 10:07:44.197393 allianceauth-4.0.2/allianceauth/services/modules/example/apps.py
+-rw-r--r--   0        0        0     1336 2024-05-12 10:07:44.197393 allianceauth-4.0.2/allianceauth/services/modules/example/auth_hooks.py
+-rw-r--r--   0        0        0      411 2024-05-12 10:07:44.198393 allianceauth-4.0.2/allianceauth/services/modules/example/models.py
+-rw-r--r--   0        0        0      206 2024-05-12 10:07:44.198393 allianceauth-4.0.2/allianceauth/services/modules/example/urls.py
+-rw-r--r--   0        0        0       22 2024-05-12 10:07:44.198393 allianceauth-4.0.2/allianceauth/services/modules/example/views.py
+-rw-r--r--   0        0        0        0 2024-05-12 10:07:44.343393 allianceauth-4.0.2/allianceauth/services/modules/ips4/__init__.py
+-rw-r--r--   0        0        0      240 2024-05-12 10:07:44.198393 allianceauth-4.0.2/allianceauth/services/modules/ips4/admin.py
+-rw-r--r--   0        0        0      139 2024-05-12 10:07:44.198393 allianceauth-4.0.2/allianceauth/services/modules/ips4/apps.py
+-rw-r--r--   0        0        0     1554 2024-05-12 10:07:44.198393 allianceauth-4.0.2/allianceauth/services/modules/ips4/auth_hooks.py
+-rw-r--r--   0        0        0     4199 2024-05-12 10:07:44.198393 allianceauth-4.0.2/allianceauth/services/modules/ips4/manager.py
+-rw-r--r--   0        0        0      737 2024-05-12 10:07:44.198393 allianceauth-4.0.2/allianceauth/services/modules/ips4/migrations/0001_initial.py
+-rw-r--r--   0        0        0     2025 2024-05-12 10:07:44.198393 allianceauth-4.0.2/allianceauth/services/modules/ips4/migrations/0002_service_permissions.py
+-rw-r--r--   0        0        0        0 2024-05-12 10:07:44.343393 allianceauth-4.0.2/allianceauth/services/modules/ips4/migrations/__init__.py
+-rw-r--r--   0        0        0      558 2024-05-12 10:07:44.198393 allianceauth-4.0.2/allianceauth/services/modules/ips4/models.py
+-rw-r--r--   0        0        0     1104 2024-05-12 10:07:44.198393 allianceauth-4.0.2/allianceauth/services/modules/ips4/tasks.py
+-rw-r--r--   0        0        0     6035 2024-05-12 10:07:44.199393 allianceauth-4.0.2/allianceauth/services/modules/ips4/tests.py
+-rw-r--r--   0        0        0      495 2024-05-12 10:07:44.199393 allianceauth-4.0.2/allianceauth/services/modules/ips4/urls.py
+-rw-r--r--   0        0        0     4825 2024-05-12 10:07:44.199393 allianceauth-4.0.2/allianceauth/services/modules/ips4/views.py
+-rw-r--r--   0        0        0        0 2024-05-12 10:07:44.343393 allianceauth-4.0.2/allianceauth/services/modules/mumble/__init__.py
+-rw-r--r--   0        0        0      455 2024-05-12 10:07:44.199393 allianceauth-4.0.2/allianceauth/services/modules/mumble/admin.py
+-rw-r--r--   0        0        0      145 2024-05-12 10:07:44.199393 allianceauth-4.0.2/allianceauth/services/modules/mumble/apps.py
+-rw-r--r--   0        0        0     2958 2024-05-12 10:07:44.199393 allianceauth-4.0.2/allianceauth/services/modules/mumble/auth_hooks.py
+-rw-r--r--   0        0        0      726 2024-05-12 10:07:44.199393 allianceauth-4.0.2/allianceauth/services/modules/mumble/migrations/0001_initial.py
+-rw-r--r--   0        0        0     2868 2024-05-12 10:07:44.199393 allianceauth-4.0.2/allianceauth/services/modules/mumble/migrations/0001_squashed_0011_auto_20201011_1009.py
+-rw-r--r--   0        0        0      316 2024-05-12 10:07:44.199393 allianceauth-4.0.2/allianceauth/services/modules/mumble/migrations/0002_auto_20161212_0100.py
+-rw-r--r--   0        0        0      613 2024-05-12 10:07:44.199393 allianceauth-4.0.2/allianceauth/services/modules/mumble/migrations/0003_mumbleuser_user.py
+-rw-r--r--   0        0        0      548 2024-05-12 10:07:44.200393 allianceauth-4.0.2/allianceauth/services/modules/mumble/migrations/0004_auto_20161214_1024.py
+-rw-r--r--   0        0        0      561 2024-05-12 10:07:44.200393 allianceauth-4.0.2/allianceauth/services/modules/mumble/migrations/0005_mumbleuser_hashfn.py
+-rw-r--r--   0        0        0     2063 2024-05-12 10:07:44.200393 allianceauth-4.0.2/allianceauth/services/modules/mumble/migrations/0006_service_permissions.py
+-rw-r--r--   0        0        0      679 2024-05-12 10:07:44.200393 allianceauth-4.0.2/allianceauth/services/modules/mumble/migrations/0007_not_null_user.py
+-rw-r--r--   0        0        0      398 2024-05-12 10:07:44.200393 allianceauth-4.0.2/allianceauth/services/modules/mumble/migrations/0008_mumbleuser_display_name.py
+-rw-r--r--   0        0        0     1181 2024-05-12 10:07:44.200393 allianceauth-4.0.2/allianceauth/services/modules/mumble/migrations/0009_set_mumble_dissplay_names.py
+-rw-r--r--   0        0        0      554 2024-05-12 10:07:44.200393 allianceauth-4.0.2/allianceauth/services/modules/mumble/migrations/0010_mumbleuser_certhash.py
+-rw-r--r--   0        0        0      390 2024-05-12 10:07:44.200393 allianceauth-4.0.2/allianceauth/services/modules/mumble/migrations/0011_auto_20201011_1009.py
+-rw-r--r--   0        0        0     1508 2024-05-12 10:07:44.200393 allianceauth-4.0.2/allianceauth/services/modules/mumble/migrations/0012_mumble_client_info.py
+-rw-r--r--   0        0        0        0 2024-05-12 10:07:44.352393 allianceauth-4.0.2/allianceauth/services/modules/mumble/migrations/__init__.py
+-rw-r--r--   0        0        0     5630 2024-05-12 10:07:44.200393 allianceauth-4.0.2/allianceauth/services/modules/mumble/models.py
+-rw-r--r--   0        0        0     3142 2024-05-12 10:07:44.200393 allianceauth-4.0.2/allianceauth/services/modules/mumble/tasks.py
+-rw-r--r--   0        0        0     1655 2024-05-12 10:07:44.201393 allianceauth-4.0.2/allianceauth/services/modules/mumble/templates/services/mumble/mumble_service_ctrl.html
+-rw-r--r--   0        0        0     8632 2024-05-12 10:07:44.201393 allianceauth-4.0.2/allianceauth/services/modules/mumble/tests.py
+-rw-r--r--   0        0        0      560 2024-05-12 10:07:44.201393 allianceauth-4.0.2/allianceauth/services/modules/mumble/urls.py
+-rw-r--r--   0        0        0      994 2024-05-12 10:07:44.201393 allianceauth-4.0.2/allianceauth/services/modules/mumble/views.py
+-rw-r--r--   0        0        0        0 2024-05-12 10:07:44.352393 allianceauth-4.0.2/allianceauth/services/modules/openfire/__init__.py
+-rw-r--r--   0        0        0      317 2024-05-12 10:07:44.201393 allianceauth-4.0.2/allianceauth/services/modules/openfire/admin.py
+-rw-r--r--   0        0        0      151 2024-05-12 10:07:44.201393 allianceauth-4.0.2/allianceauth/services/modules/openfire/apps.py
+-rw-r--r--   0        0        0     3648 2024-05-12 10:07:44.201393 allianceauth-4.0.2/allianceauth/services/modules/openfire/auth_hooks.py
+-rw-r--r--   0        0        0      263 2024-05-12 10:07:44.201393 allianceauth-4.0.2/allianceauth/services/modules/openfire/forms.py
+-rw-r--r--   0        0        0     8321 2024-05-12 10:07:44.201393 allianceauth-4.0.2/allianceauth/services/modules/openfire/manager.py
+-rw-r--r--   0        0        0      687 2024-05-12 10:07:44.201393 allianceauth-4.0.2/allianceauth/services/modules/openfire/migrations/0001_initial.py
+-rw-r--r--   0        0        0     2073 2024-05-12 10:07:44.202393 allianceauth-4.0.2/allianceauth/services/modules/openfire/migrations/0002_service_permissions.py
+-rw-r--r--   0        0        0        0 2024-05-12 10:07:44.352393 allianceauth-4.0.2/allianceauth/services/modules/openfire/migrations/__init__.py
+-rw-r--r--   0        0        0      495 2024-05-12 10:07:44.202393 allianceauth-4.0.2/allianceauth/services/modules/openfire/models.py
+-rw-r--r--   0        0        0     2620 2024-05-12 10:07:44.202393 allianceauth-4.0.2/allianceauth/services/modules/openfire/tasks.py
+-rw-r--r--   0        0        0     1533 2024-05-12 10:07:44.202393 allianceauth-4.0.2/allianceauth/services/modules/openfire/templates/services/openfire/broadcast.html
+-rw-r--r--   0        0        0     9478 2024-05-12 10:07:44.202393 allianceauth-4.0.2/allianceauth/services/modules/openfire/tests.py
+-rw-r--r--   0        0        0      585 2024-05-12 10:07:44.202393 allianceauth-4.0.2/allianceauth/services/modules/openfire/urls.py
+-rw-r--r--   0        0        0     7688 2024-05-12 10:07:44.202393 allianceauth-4.0.2/allianceauth/services/modules/openfire/views.py
+-rw-r--r--   0        0        0        0 2024-05-12 10:07:44.362393 allianceauth-4.0.2/allianceauth/services/modules/phpbb3/__init__.py
+-rw-r--r--   0        0        0      310 2024-05-12 10:07:44.202393 allianceauth-4.0.2/allianceauth/services/modules/phpbb3/admin.py
+-rw-r--r--   0        0        0      145 2024-05-12 10:07:44.202393 allianceauth-4.0.2/allianceauth/services/modules/phpbb3/apps.py
+-rw-r--r--   0        0        0     2196 2024-05-12 10:07:44.202393 allianceauth-4.0.2/allianceauth/services/modules/phpbb3/auth_hooks.py
+-rw-r--r--   0        0        0    13459 2024-05-12 10:07:44.203393 allianceauth-4.0.2/allianceauth/services/modules/phpbb3/manager.py
+-rw-r--r--   0        0        0      683 2024-05-12 10:07:44.203393 allianceauth-4.0.2/allianceauth/services/modules/phpbb3/migrations/0001_initial.py
+-rw-r--r--   0        0        0     2049 2024-05-12 10:07:44.203393 allianceauth-4.0.2/allianceauth/services/modules/phpbb3/migrations/0002_service_permissions.py
+-rw-r--r--   0        0        0        0 2024-05-12 10:07:44.363393 allianceauth-4.0.2/allianceauth/services/modules/phpbb3/migrations/__init__.py
+-rw-r--r--   0        0        0      487 2024-05-12 10:07:44.203393 allianceauth-4.0.2/allianceauth/services/modules/phpbb3/models.py
+-rw-r--r--   0        0        0     2478 2024-05-12 10:07:44.203393 allianceauth-4.0.2/allianceauth/services/modules/phpbb3/tasks.py
+-rw-r--r--   0        0        0     8189 2024-05-12 10:07:44.203393 allianceauth-4.0.2/allianceauth/services/modules/phpbb3/tests.py
+-rw-r--r--   0        0        0      504 2024-05-12 10:07:44.203393 allianceauth-4.0.2/allianceauth/services/modules/phpbb3/urls.py
+-rw-r--r--   0        0        0     5139 2024-05-12 10:07:44.203393 allianceauth-4.0.2/allianceauth/services/modules/phpbb3/views.py
+-rw-r--r--   0        0        0        0 2024-05-12 10:07:44.363393 allianceauth-4.0.2/allianceauth/services/modules/smf/__init__.py
+-rw-r--r--   0        0        0      302 2024-05-12 10:07:44.203393 allianceauth-4.0.2/allianceauth/services/modules/smf/admin.py
+-rw-r--r--   0        0        0      136 2024-05-12 10:07:44.203393 allianceauth-4.0.2/allianceauth/services/modules/smf/apps.py
+-rw-r--r--   0        0        0     2408 2024-05-12 10:07:44.203393 allianceauth-4.0.2/allianceauth/services/modules/smf/auth_hooks.py
+-rw-r--r--   0        0        0    14780 2024-05-12 10:07:44.204393 allianceauth-4.0.2/allianceauth/services/modules/smf/manager.py
+-rw-r--r--   0        0        0      677 2024-05-12 10:07:44.204393 allianceauth-4.0.2/allianceauth/services/modules/smf/migrations/0001_initial.py
+-rw-r--r--   0        0        0     2011 2024-05-12 10:07:44.204393 allianceauth-4.0.2/allianceauth/services/modules/smf/migrations/0002_service_permissions.py
+-rw-r--r--   0        0        0      694 2024-05-12 10:07:44.204393 allianceauth-4.0.2/allianceauth/services/modules/smf/migrations/0003_set_smf_displayed_names.py
+-rw-r--r--   0        0        0        0 2024-05-12 10:07:44.363393 allianceauth-4.0.2/allianceauth/services/modules/smf/migrations/__init__.py
+-rw-r--r--   0        0        0      475 2024-05-12 10:07:44.204393 allianceauth-4.0.2/allianceauth/services/modules/smf/models.py
+-rw-r--r--   0        0        0     3740 2024-05-12 10:07:44.204393 allianceauth-4.0.2/allianceauth/services/modules/smf/tasks.py
+-rw-r--r--   0        0        0     8057 2024-05-12 10:07:44.204393 allianceauth-4.0.2/allianceauth/services/modules/smf/tests.py
+-rw-r--r--   0        0        0      489 2024-05-12 10:07:44.204393 allianceauth-4.0.2/allianceauth/services/modules/smf/urls.py
+-rw-r--r--   0        0        0     5143 2024-05-12 10:07:44.204393 allianceauth-4.0.2/allianceauth/services/modules/smf/views.py
+-rw-r--r--   0        0        0        0 2024-05-12 10:07:44.363393 allianceauth-4.0.2/allianceauth/services/modules/teamspeak3/__init__.py
+-rw-r--r--   0        0        0     1872 2024-05-12 10:07:44.204393 allianceauth-4.0.2/allianceauth/services/modules/teamspeak3/admin.py
+-rw-r--r--   0        0        0      209 2024-05-12 10:07:44.204393 allianceauth-4.0.2/allianceauth/services/modules/teamspeak3/apps.py
+-rw-r--r--   0        0        0     2128 2024-05-12 10:07:44.204393 allianceauth-4.0.2/allianceauth/services/modules/teamspeak3/auth_hooks.py
+-rw-r--r--   0        0        0      500 2024-05-12 10:07:44.204393 allianceauth-4.0.2/allianceauth/services/modules/teamspeak3/forms.py
+-rw-r--r--   0        0        0    12601 2024-05-12 10:07:44.205393 allianceauth-4.0.2/allianceauth/services/modules/teamspeak3/manager.py
+-rw-r--r--   0        0        0     1995 2024-05-12 10:07:44.205393 allianceauth-4.0.2/allianceauth/services/modules/teamspeak3/migrations/0001_initial.py
+-rw-r--r--   0        0        0      538 2024-05-12 10:07:44.205393 allianceauth-4.0.2/allianceauth/services/modules/teamspeak3/migrations/0002_auto_20161212_0133.py
+-rw-r--r--   0        0        0      781 2024-05-12 10:07:44.205393 allianceauth-4.0.2/allianceauth/services/modules/teamspeak3/migrations/0003_teamspeak3user.py
+-rw-r--r--   0        0        0     2116 2024-05-12 10:07:44.205393 allianceauth-4.0.2/allianceauth/services/modules/teamspeak3/migrations/0004_service_permissions.py
+-rw-r--r--   0        0        0      784 2024-05-12 10:07:44.205393 allianceauth-4.0.2/allianceauth/services/modules/teamspeak3/migrations/0005_stategroup.py
+-rw-r--r--   0        0        0        0 2024-05-12 10:07:44.363393 allianceauth-4.0.2/allianceauth/services/modules/teamspeak3/migrations/__init__.py
+-rw-r--r--   0        0        0     1567 2024-05-12 10:07:44.205393 allianceauth-4.0.2/allianceauth/services/modules/teamspeak3/models.py
+-rw-r--r--   0        0        0     1723 2024-05-12 10:07:44.205393 allianceauth-4.0.2/allianceauth/services/modules/teamspeak3/signals.py
+-rw-r--r--   0        0        0     3780 2024-05-12 10:07:44.205393 allianceauth-4.0.2/allianceauth/services/modules/teamspeak3/tasks.py
+-rw-r--r--   0        0        0      296 2024-05-12 10:07:44.206393 allianceauth-4.0.2/allianceauth/services/modules/teamspeak3/templates/admin/teamspeak3/authts/change_list.html
+-rw-r--r--   0        0        0     1472 2024-05-12 10:07:44.206393 allianceauth-4.0.2/allianceauth/services/modules/teamspeak3/templates/services/teamspeak3/teamspeak3_service_ctrl.html
+-rw-r--r--   0        0        0     1121 2024-05-12 10:07:44.206393 allianceauth-4.0.2/allianceauth/services/modules/teamspeak3/templates/services/teamspeak3/teamspeakjoin.html
+-rw-r--r--   0        0        0    21498 2024-05-12 10:07:44.206393 allianceauth-4.0.2/allianceauth/services/modules/teamspeak3/tests.py
+-rw-r--r--   0        0        0      661 2024-05-12 10:07:44.206393 allianceauth-4.0.2/allianceauth/services/modules/teamspeak3/urls.py
+-rw-r--r--   0        0        0       23 2024-05-12 10:07:44.206393 allianceauth-4.0.2/allianceauth/services/modules/teamspeak3/util/__init__.py
+-rw-r--r--   0        0        0    15106 2024-05-12 10:07:44.206393 allianceauth-4.0.2/allianceauth/services/modules/teamspeak3/util/ts3.py
+-rw-r--r--   0        0        0     5138 2024-05-12 10:07:44.207393 allianceauth-4.0.2/allianceauth/services/modules/teamspeak3/views.py
+-rw-r--r--   0        0        0        0 2024-05-12 10:07:44.363393 allianceauth-4.0.2/allianceauth/services/modules/xenforo/__init__.py
+-rw-r--r--   0        0        0      314 2024-05-12 10:07:44.207393 allianceauth-4.0.2/allianceauth/services/modules/xenforo/admin.py
+-rw-r--r--   0        0        0      148 2024-05-12 10:07:44.207393 allianceauth-4.0.2/allianceauth/services/modules/xenforo/apps.py
+-rw-r--r--   0        0        0     1779 2024-05-12 10:07:44.207393 allianceauth-4.0.2/allianceauth/services/modules/xenforo/auth_hooks.py
+-rw-r--r--   0        0        0     3685 2024-05-12 10:07:44.207393 allianceauth-4.0.2/allianceauth/services/modules/xenforo/manager.py
+-rw-r--r--   0        0        0      685 2024-05-12 10:07:44.207393 allianceauth-4.0.2/allianceauth/services/modules/xenforo/migrations/0001_initial.py
+-rw-r--r--   0        0        0     2067 2024-05-12 10:07:44.207393 allianceauth-4.0.2/allianceauth/services/modules/xenforo/migrations/0002_service_permissions.py
+-rw-r--r--   0        0        0        0 2024-05-12 10:07:44.368393 allianceauth-4.0.2/allianceauth/services/modules/xenforo/migrations/__init__.py
+-rw-r--r--   0        0        0      491 2024-05-12 10:07:44.207393 allianceauth-4.0.2/allianceauth/services/modules/xenforo/models.py
+-rw-r--r--   0        0        0     1268 2024-05-12 10:07:44.207393 allianceauth-4.0.2/allianceauth/services/modules/xenforo/tasks.py
+-rw-r--r--   0        0        0     7153 2024-05-12 10:07:44.207393 allianceauth-4.0.2/allianceauth/services/modules/xenforo/tests.py
+-rw-r--r--   0        0        0      529 2024-05-12 10:07:44.207393 allianceauth-4.0.2/allianceauth/services/modules/xenforo/urls.py
+-rw-r--r--   0        0        0     4821 2024-05-12 10:07:44.207393 allianceauth-4.0.2/allianceauth/services/modules/xenforo/views.py
+-rw-r--r--   0        0        0    10087 2024-05-12 10:07:44.208393 allianceauth-4.0.2/allianceauth/services/signals.py
+-rw-r--r--   0        0        0      126 2024-05-12 10:07:44.208393 allianceauth-4.0.2/allianceauth/services/static/allianceauth/services/admin.css
+-rw-r--r--   0        0        0     1937 2024-05-12 10:07:44.208393 allianceauth-4.0.2/allianceauth/services/tasks.py
+-rw-r--r--   0        0        0       57 2024-05-12 10:07:44.208393 allianceauth-4.0.2/allianceauth/services/templates/public/menublock.html
+-rw-r--r--   0        0        0      335 2024-05-12 10:07:44.208393 allianceauth-4.0.2/allianceauth/services/templates/public/menuitem.html
+-rw-r--r--   0        0        0     1566 2024-05-12 10:07:44.208393 allianceauth-4.0.2/allianceauth/services/templates/services/fleetformattertool.html
+-rw-r--r--   0        0        0     1232 2024-05-12 10:07:44.208393 allianceauth-4.0.2/allianceauth/services/templates/services/service_confirm_delete.html
+-rw-r--r--   0        0        0     1285 2024-05-12 10:07:44.208393 allianceauth-4.0.2/allianceauth/services/templates/services/service_credentials.html
+-rw-r--r--   0        0        0     1147 2024-05-12 10:07:44.208393 allianceauth-4.0.2/allianceauth/services/templates/services/service_password.html
+-rw-r--r--   0        0        0      239 2024-05-12 10:07:44.208393 allianceauth-4.0.2/allianceauth/services/templates/services/service_status.html
+-rw-r--r--   0        0        0      100 2024-05-12 10:07:44.208393 allianceauth-4.0.2/allianceauth/services/templates/services/service_username.html
+-rw-r--r--   0        0        0     2422 2024-05-12 10:07:44.209393 allianceauth-4.0.2/allianceauth/services/templates/services/services.html
+-rw-r--r--   0        0        0     1233 2024-05-12 10:07:44.209393 allianceauth-4.0.2/allianceauth/services/templates/services/services_ctrl.html
+-rw-r--r--   0        0        0      832 2024-05-12 10:07:44.209393 allianceauth-4.0.2/allianceauth/services/templates/services/services_ctrl_base.html
+-rw-r--r--   0        0        0        0 2024-05-12 10:07:44.368393 allianceauth-4.0.2/allianceauth/services/tests/__init__.py
+-rw-r--r--   0        0        0     1048 2024-05-12 10:07:44.209393 allianceauth-4.0.2/allianceauth/services/tests/test_hooks.py
+-rw-r--r--   0        0        0      514 2024-05-12 10:07:44.209393 allianceauth-4.0.2/allianceauth/services/tests/test_models.py
+-rw-r--r--   0        0        0     4316 2024-05-12 10:07:44.209393 allianceauth-4.0.2/allianceauth/services/tests/test_nameformatter.py
+-rw-r--r--   0        0        0    12299 2024-05-12 10:07:44.209393 allianceauth-4.0.2/allianceauth/services/tests/test_signals.py
+-rw-r--r--   0        0        0     3248 2024-05-12 10:07:44.209393 allianceauth-4.0.2/allianceauth/services/tests/test_tasks.py
+-rw-r--r--   0        0        0      530 2024-05-12 10:07:44.209393 allianceauth-4.0.2/allianceauth/services/urls.py
+-rw-r--r--   0        0        0     2450 2024-05-12 10:07:44.209393 allianceauth-4.0.2/allianceauth/services/views.py
+-rw-r--r--   0        0        0        0 2024-05-12 10:07:44.368393 allianceauth-4.0.2/allianceauth/srp/__init__.py
+-rw-r--r--   0        0        0      205 2024-05-12 10:07:44.209393 allianceauth-4.0.2/allianceauth/srp/admin.py
+-rw-r--r--   0        0        0      112 2024-05-12 10:07:44.209393 allianceauth-4.0.2/allianceauth/srp/apps.py
+-rw-r--r--   0        0        0      960 2024-05-12 10:07:44.209393 allianceauth-4.0.2/allianceauth/srp/auth_hooks.py
+-rw-r--r--   0        0        0     1724 2024-05-12 10:07:44.210393 allianceauth-4.0.2/allianceauth/srp/form.py
+-rw-r--r--   0        0        0     1961 2024-05-12 10:07:44.210393 allianceauth-4.0.2/allianceauth/srp/managers.py
+-rw-r--r--   0        0        0     2265 2024-05-12 10:07:44.210393 allianceauth-4.0.2/allianceauth/srp/migrations/0001_initial.py
+-rw-r--r--   0        0        0      488 2024-05-12 10:07:44.210393 allianceauth-4.0.2/allianceauth/srp/migrations/0002_srpuserrequest_srp_status_choices.py
+-rw-r--r--   0        0        0     2048 2024-05-12 10:07:44.210393 allianceauth-4.0.2/allianceauth/srp/migrations/0003_make_strings_more_stringy.py
+-rw-r--r--   0        0        0      746 2024-05-12 10:07:44.210393 allianceauth-4.0.2/allianceauth/srp/migrations/0004_on_delete.py
+-rw-r--r--   0        0        0        0 2024-05-12 10:07:44.368393 allianceauth-4.0.2/allianceauth/srp/migrations/__init__.py
+-rw-r--r--   0        0        0     1991 2024-05-12 10:07:44.210393 allianceauth-4.0.2/allianceauth/srp/models.py
+-rw-r--r--   0        0        0      388 2024-05-12 10:07:44.210393 allianceauth-4.0.2/allianceauth/srp/providers.py
+-rw-r--r--   0        0        0    24877 2024-05-12 10:07:44.210393 allianceauth-4.0.2/allianceauth/srp/swagger.json
+-rw-r--r--   0        0        0     2597 2024-05-12 10:07:44.210393 allianceauth-4.0.2/allianceauth/srp/templates/srp/add.html
+-rw-r--r--   0        0        0    13408 2024-05-12 10:07:44.211393 allianceauth-4.0.2/allianceauth/srp/templates/srp/data.html
+-rw-r--r--   0        0        0     6364 2024-05-12 10:07:44.211393 allianceauth-4.0.2/allianceauth/srp/templates/srp/management.html
+-rw-r--r--   0        0        0     1432 2024-05-12 10:07:44.211393 allianceauth-4.0.2/allianceauth/srp/templates/srp/request.html
+-rw-r--r--   0        0        0     1765 2024-05-12 10:07:44.211393 allianceauth-4.0.2/allianceauth/srp/templates/srp/update.html
+-rw-r--r--   0        0        0        0 2024-05-12 10:07:44.368393 allianceauth-4.0.2/allianceauth/srp/tests/__init__.py
+-rw-r--r--   0        0        0     3623 2024-05-12 10:07:44.211393 allianceauth-4.0.2/allianceauth/srp/tests/test_managers.py
+-rw-r--r--   0        0        0    28605 2024-05-12 10:07:44.211393 allianceauth-4.0.2/allianceauth/srp/tests/testdata/get_killmails_killmail_id_killmail_hash_81973979.json
+-rw-r--r--   0        0        0      363 2024-05-12 10:07:44.211393 allianceauth-4.0.2/allianceauth/srp/tests/testdata/zkillboard_killmail_api_81973979.json
+-rw-r--r--   0        0        0     1342 2024-05-12 10:07:44.211393 allianceauth-4.0.2/allianceauth/srp/urls.py
+-rw-r--r--   0        0        0    17762 2024-05-12 10:07:44.211393 allianceauth-4.0.2/allianceauth/srp/views.py
+-rw-r--r--   0        0        0     4616 2024-05-12 10:07:44.212393 allianceauth-4.0.2/allianceauth/static/allianceauth/css/auth-base.css
+-rw-r--r--   0        0        0     1173 2024-05-12 10:07:44.212393 allianceauth-4.0.2/allianceauth/static/allianceauth/css/checkbox.css
+-rw-r--r--   0        0        0      865 2024-05-12 10:07:44.212393 allianceauth-4.0.2/allianceauth/static/allianceauth/css/themes/bootstrap-locals.less
+-rw-r--r--   0        0        0     1078 2024-05-12 10:07:44.212393 allianceauth-4.0.2/allianceauth/static/allianceauth/css/themes/darkly/LICENSE
+-rw-r--r--   0        0        0      624 2024-05-12 10:07:44.212393 allianceauth-4.0.2/allianceauth/static/allianceauth/css/themes/darkly/darkly.less
+-rw-r--r--   0        0        0   122466 2024-05-12 10:07:44.213393 allianceauth-4.0.2/allianceauth/static/allianceauth/css/themes/darkly/darkly.min.css
+-rw-r--r--   0        0        0      979 2024-05-12 10:07:44.213393 allianceauth-4.0.2/allianceauth/static/allianceauth/css/themes/flatly-shared.less
+-rw-r--r--   0        0        0     1078 2024-05-12 10:07:44.213393 allianceauth-4.0.2/allianceauth/static/allianceauth/css/themes/flatly/LICENSE
+-rw-r--r--   0        0        0      985 2024-05-12 10:07:44.213393 allianceauth-4.0.2/allianceauth/static/allianceauth/css/themes/flatly/flatly.less
+-rw-r--r--   0        0        0   123138 2024-05-12 10:07:44.213393 allianceauth-4.0.2/allianceauth/static/allianceauth/css/themes/flatly/flatly.min.css
+-rwxr-xr-x   0        0        0    21465 2024-05-12 10:07:44.214393 allianceauth-4.0.2/allianceauth/static/allianceauth/icons/allianceauth.png
+-rw-r--r--   0        0        0     7686 2024-05-12 10:07:44.214393 allianceauth-4.0.2/allianceauth/static/allianceauth/icons/android-chrome-192x192.png
+-rw-r--r--   0        0        0    26346 2024-05-12 10:07:44.214393 allianceauth-4.0.2/allianceauth/static/allianceauth/icons/android-chrome-512x512.png
+-rw-r--r--   0        0        0     7160 2024-05-12 10:07:44.214393 allianceauth-4.0.2/allianceauth/static/allianceauth/icons/apple-touch-icon.png
+-rw-r--r--   0        0        0      272 2024-05-12 10:07:44.214393 allianceauth-4.0.2/allianceauth/static/allianceauth/icons/browserconfig.xml
+-rw-r--r--   0        0        0      941 2024-05-12 10:07:44.214393 allianceauth-4.0.2/allianceauth/static/allianceauth/icons/favicon-16x16.png
+-rw-r--r--   0        0        0     1565 2024-05-12 10:07:44.214393 allianceauth-4.0.2/allianceauth/static/allianceauth/icons/favicon-32x32.png
+-rwxr-xr-x   0        0        0     2180 2024-05-12 10:07:44.214393 allianceauth-4.0.2/allianceauth/static/allianceauth/icons/favicon-96x96.png
+-rw-r--r--   0        0        0    15086 2024-05-12 10:07:44.214393 allianceauth-4.0.2/allianceauth/static/allianceauth/icons/favicon.ico
+-rw-r--r--   0        0        0     4681 2024-05-12 10:07:44.214393 allianceauth-4.0.2/allianceauth/static/allianceauth/icons/mstile-150x150.png
+-rw-r--r--   0        0        0     2590 2024-05-12 10:07:44.215393 allianceauth-4.0.2/allianceauth/static/allianceauth/icons/safari-pinned-tab.svg
+-rw-r--r--   0        0        0      478 2024-05-12 10:07:44.215393 allianceauth-4.0.2/allianceauth/static/allianceauth/icons/site.webmanifest
+-rw-r--r--   0        0        0    10836 2024-05-12 10:07:44.215393 allianceauth-4.0.2/allianceauth/static/allianceauth/images/auth-logo.png
+-rw-r--r--   0        0        0     2278 2024-05-12 10:07:44.215393 allianceauth-4.0.2/allianceauth/static/allianceauth/images/auth-logo.svg
+-rw-r--r--   0        0        0      573 2024-05-12 10:07:44.215393 allianceauth-4.0.2/allianceauth/static/allianceauth/js/eve-time.js
+-rw-r--r--   0        0        0     1070 2024-05-12 10:07:44.215393 allianceauth-4.0.2/allianceauth/static/allianceauth/js/filterDropDown/LICENSE
+-rw-r--r--   0        0        0    10422 2024-05-12 10:07:44.215393 allianceauth-4.0.2/allianceauth/static/allianceauth/js/filterDropDown/filterDropDown.js
+-rw-r--r--   0        0        0     4205 2024-05-12 10:07:44.215393 allianceauth-4.0.2/allianceauth/static/allianceauth/js/filterDropDown/filterDropDown.min.js
+-rw-r--r--   0        0        0     7090 2024-05-12 10:07:44.215393 allianceauth-4.0.2/allianceauth/static/allianceauth/js/jquery-ui/1.12.1/css/images/ui-icons_444444_256x240.png
+-rw-r--r--   0        0        0     7074 2024-05-12 10:07:44.216393 allianceauth-4.0.2/allianceauth/static/allianceauth/js/jquery-ui/1.12.1/css/images/ui-icons_555555_256x240.png
+-rw-r--r--   0        0        0     4618 2024-05-12 10:07:44.216393 allianceauth-4.0.2/allianceauth/static/allianceauth/js/jquery-ui/1.12.1/css/images/ui-icons_777620_256x240.png
+-rw-r--r--   0        0        0     7111 2024-05-12 10:07:44.216393 allianceauth-4.0.2/allianceauth/static/allianceauth/js/jquery-ui/1.12.1/css/images/ui-icons_777777_256x240.png
+-rw-r--r--   0        0        0     4618 2024-05-12 10:07:44.216393 allianceauth-4.0.2/allianceauth/static/allianceauth/js/jquery-ui/1.12.1/css/images/ui-icons_cc0000_256x240.png
+-rw-r--r--   0        0        0     6487 2024-05-12 10:07:44.216393 allianceauth-4.0.2/allianceauth/static/allianceauth/js/jquery-ui/1.12.1/css/images/ui-icons_ffffff_256x240.png
+-rw-r--r--   0        0        0    15830 2024-05-12 10:07:44.216393 allianceauth-4.0.2/allianceauth/static/allianceauth/js/jquery-ui/1.12.1/css/jquery-ui.min.css
+-rw-r--r--   0        0        0     7142 2024-05-12 10:07:44.216393 allianceauth-4.0.2/allianceauth/static/allianceauth/js/jquery-ui/1.13.2/css/images/ui-icons_444444_256x240.png
+-rw-r--r--   0        0        0     7126 2024-05-12 10:07:44.216393 allianceauth-4.0.2/allianceauth/static/allianceauth/js/jquery-ui/1.13.2/css/images/ui-icons_555555_256x240.png
+-rw-r--r--   0        0        0     4670 2024-05-12 10:07:44.216393 allianceauth-4.0.2/allianceauth/static/allianceauth/js/jquery-ui/1.13.2/css/images/ui-icons_777620_256x240.png
+-rw-r--r--   0        0        0     7163 2024-05-12 10:07:44.217393 allianceauth-4.0.2/allianceauth/static/allianceauth/js/jquery-ui/1.13.2/css/images/ui-icons_777777_256x240.png
+-rw-r--r--   0        0        0     4670 2024-05-12 10:07:44.217393 allianceauth-4.0.2/allianceauth/static/allianceauth/js/jquery-ui/1.13.2/css/images/ui-icons_cc0000_256x240.png
+-rw-r--r--   0        0        0     6539 2024-05-12 10:07:44.217393 allianceauth-4.0.2/allianceauth/static/allianceauth/js/jquery-ui/1.13.2/css/images/ui-icons_ffffff_256x240.png
+-rw-r--r--   0        0        0    15842 2024-05-12 10:07:44.217393 allianceauth-4.0.2/allianceauth/static/allianceauth/js/jquery-ui/1.13.2/css/jquery-ui.min.css
+-rw-r--r--   0        0        0     2391 2024-05-12 10:07:44.217393 allianceauth-4.0.2/allianceauth/static/allianceauth/js/refresh-notification-icon.js
+-rw-r--r--   0        0        0     2636 2024-05-12 10:07:44.217393 allianceauth-4.0.2/allianceauth/static/allianceauth/js/refresh_notifications.js
+-rw-r--r--   0        0        0     1170 2024-05-12 10:07:44.217393 allianceauth-4.0.2/allianceauth/static/allianceauth/js/timerboard.js
+-rw-r--r--   0        0        0     1056 2024-05-12 10:07:44.217393 allianceauth-4.0.2/allianceauth/static/allianceauth/js/timers.js
+-rw-r--r--   0        0        0       26 2024-05-12 10:07:44.217393 allianceauth-4.0.2/allianceauth/static/robots.txt
+-rw-r--r--   0        0        0      119 2024-05-12 10:07:44.217393 allianceauth-4.0.2/allianceauth/templates/admin/base_site.html
+-rw-r--r--   0        0        0      403 2024-05-12 10:07:44.217393 allianceauth-4.0.2/allianceauth/templates/allianceauth/admin-status/celery_bar_partial.html
+-rw-r--r--   0        0        0     1282 2024-05-12 10:07:44.217393 allianceauth-4.0.2/allianceauth/templates/allianceauth/admin-status/esi_check.html
+-rw-r--r--   0        0        0       47 2024-05-12 10:07:44.218393 allianceauth-4.0.2/allianceauth/templates/allianceauth/admin-status/include.html
+-rw-r--r--   0        0        0     8149 2024-05-12 10:07:44.218393 allianceauth-4.0.2/allianceauth/templates/allianceauth/admin-status/overview.html
+-rw-r--r--   0        0        0     5350 2024-05-12 10:07:44.218393 allianceauth-4.0.2/allianceauth/templates/allianceauth/base-bs5.html
+-rw-r--r--   0        0        0     2443 2024-05-12 10:07:44.218393 allianceauth-4.0.2/allianceauth/templates/allianceauth/base.html
+-rw-r--r--   0        0        0     1289 2024-05-12 10:07:44.218393 allianceauth-4.0.2/allianceauth/templates/allianceauth/error.html
+-rw-r--r--   0        0        0      928 2024-05-12 10:07:44.218393 allianceauth-4.0.2/allianceauth/templates/allianceauth/icons.html
+-rw-r--r--   0        0        0      996 2024-05-12 10:07:44.218393 allianceauth-4.0.2/allianceauth/templates/allianceauth/messages-bs5.html
+-rw-r--r--   0        0        0     1115 2024-05-12 10:07:44.218393 allianceauth-4.0.2/allianceauth/templates/allianceauth/messages.html
+-rw-r--r--   0        0        0      263 2024-05-12 10:07:44.218393 allianceauth-4.0.2/allianceauth/templates/allianceauth/night-toggle.html
+-rw-r--r--   0        0        0      450 2024-05-12 10:07:44.218393 allianceauth-4.0.2/allianceauth/templates/allianceauth/notifications_menu_item.html
+-rw-r--r--   0        0        0      879 2024-05-12 10:07:44.218393 allianceauth-4.0.2/allianceauth/templates/allianceauth/side-menu.html
+-rw-r--r--   0        0        0      904 2024-05-12 10:07:44.218393 allianceauth-4.0.2/allianceauth/templates/allianceauth/top-menu-admin.html
+-rw-r--r--   0        0        0      855 2024-05-12 10:07:44.218393 allianceauth-4.0.2/allianceauth/templates/allianceauth/top-menu-rh-default.html
+-rw-r--r--   0        0        0     3086 2024-05-12 10:07:44.218393 allianceauth-4.0.2/allianceauth/templates/allianceauth/top-menu-user-dropdown.html
+-rw-r--r--   0        0        0     1576 2024-05-12 10:07:44.218393 allianceauth-4.0.2/allianceauth/templates/allianceauth/top-menu.html
+-rw-r--r--   0        0        0       96 2024-05-12 10:07:44.219393 allianceauth-4.0.2/allianceauth/templates/bundles/auth-base-css.html
+-rw-r--r--   0        0        0      111 2024-05-12 10:07:44.219393 allianceauth-4.0.2/allianceauth/templates/bundles/auth-framework-css.html
+-rw-r--r--   0        0        0      171 2024-05-12 10:07:44.219393 allianceauth-4.0.2/allianceauth/templates/bundles/bootstrap-css-bs5.html
+-rw-r--r--   0        0        0     1269 2024-05-12 10:07:44.219393 allianceauth-4.0.2/allianceauth/templates/bundles/bootstrap-css.html
+-rw-r--r--   0        0        0      503 2024-05-12 10:07:44.219393 allianceauth-4.0.2/allianceauth/templates/bundles/bootstrap-js-bs5.html
+-rw-r--r--   0        0        0      613 2024-05-12 10:07:44.219393 allianceauth-4.0.2/allianceauth/templates/bundles/bootstrap-js.html
+-rw-r--r--   0        0        0       95 2024-05-12 10:07:44.219393 allianceauth-4.0.2/allianceauth/templates/bundles/checkbox-css.html
+-rw-r--r--   0        0        0      343 2024-05-12 10:07:44.219393 allianceauth-4.0.2/allianceauth/templates/bundles/clipboard-js.html
+-rw-r--r--   0        0        0      369 2024-05-12 10:07:44.219393 allianceauth-4.0.2/allianceauth/templates/bundles/datatables-css-bs5.html
+-rw-r--r--   0        0        0      365 2024-05-12 10:07:44.219393 allianceauth-4.0.2/allianceauth/templates/bundles/datatables-css.html
+-rw-r--r--   0        0        0      628 2024-05-12 10:07:44.219393 allianceauth-4.0.2/allianceauth/templates/bundles/datatables-js-bs5.html
+-rw-r--r--   0        0        0      626 2024-05-12 10:07:44.219393 allianceauth-4.0.2/allianceauth/templates/bundles/datatables-js.html
+-rw-r--r--   0        0        0       86 2024-05-12 10:07:44.219393 allianceauth-4.0.2/allianceauth/templates/bundles/evetime-js.html
+-rw-r--r--   0        0        0      111 2024-05-12 10:07:44.219393 allianceauth-4.0.2/allianceauth/templates/bundles/filterdropdown-js.html
+-rw-r--r--   0        0        0      350 2024-05-12 10:07:44.219393 allianceauth-4.0.2/allianceauth/templates/bundles/fontawesome.html
+-rw-r--r--   0        0        0      237 2024-05-12 10:07:44.219393 allianceauth-4.0.2/allianceauth/templates/bundles/image-auth-logo.html
+-rw-r--r--   0        0        0      392 2024-05-12 10:07:44.220393 allianceauth-4.0.2/allianceauth/templates/bundles/jquery-datetimepicker-css.html
+-rw-r--r--   0        0        0      387 2024-05-12 10:07:44.220393 allianceauth-4.0.2/allianceauth/templates/bundles/jquery-datetimepicker-js.html
+-rw-r--r--   0        0        0      321 2024-05-12 10:07:44.220393 allianceauth-4.0.2/allianceauth/templates/bundles/jquery-js.html
+-rw-r--r--   0        0        0      500 2024-05-12 10:07:44.220393 allianceauth-4.0.2/allianceauth/templates/bundles/jquery-ui-css.html
+-rw-r--r--   0        0        0      333 2024-05-12 10:07:44.220393 allianceauth-4.0.2/allianceauth/templates/bundles/jquery-ui-js.html
+-rw-r--r--   0        0        0      344 2024-05-12 10:07:44.220393 allianceauth-4.0.2/allianceauth/templates/bundles/jquery-visibility-js.html
+-rw-r--r--   0        0        0      579 2024-05-12 10:07:44.220393 allianceauth-4.0.2/allianceauth/templates/bundles/moment-js.html
+-rw-r--r--   0        0        0      103 2024-05-12 10:07:44.220393 allianceauth-4.0.2/allianceauth/templates/bundles/refresh-notification-icon-js.html
+-rw-r--r--   0        0        0       99 2024-05-12 10:07:44.220393 allianceauth-4.0.2/allianceauth/templates/bundles/refresh-notifications-js.html
+-rw-r--r--   0        0        0       88 2024-05-12 10:07:44.220393 allianceauth-4.0.2/allianceauth/templates/bundles/timerboard-js.html
+-rw-r--r--   0        0        0       84 2024-05-12 10:07:44.220393 allianceauth-4.0.2/allianceauth/templates/bundles/timers-js.html
+-rw-r--r--   0        0        0      368 2024-05-12 10:07:44.220393 allianceauth-4.0.2/allianceauth/templates/bundles/x-editable-js.html
+-rw-r--r--   0        0        0      375 2024-05-12 10:07:44.220393 allianceauth-4.0.2/allianceauth/templates/bundles/x-editable.css.html
+-rw-r--r--   0        0        0        0 2024-05-12 10:07:44.372393 allianceauth-4.0.2/allianceauth/templatetags/__init__.py
+-rw-r--r--   0        0        0     5665 2024-05-12 10:07:44.220393 allianceauth-4.0.2/allianceauth/templatetags/admin_status.py
+-rw-r--r--   0        0        0        0 2024-05-12 10:07:44.372393 allianceauth-4.0.2/allianceauth/tests/__init__.py
+-rw-r--r--   0        0        0    11465 2024-05-12 10:07:44.221393 allianceauth-4.0.2/allianceauth/tests/auth_utils.py
+-rw-r--r--   0        0        0     2061 2024-05-12 10:07:44.221393 allianceauth-4.0.2/allianceauth/tests/test_auth_utils.py
+-rw-r--r--   0        0        0     2897 2024-05-12 10:07:44.221393 allianceauth-4.0.2/allianceauth/tests/test_urls.py
+-rw-r--r--   0        0        0     1403 2024-05-12 10:07:44.221393 allianceauth-4.0.2/allianceauth/tests/test_views.py
+-rw-r--r--   0        0        0        0 2024-05-12 10:07:44.372393 allianceauth-4.0.2/allianceauth/theme/__init__.py
+-rw-r--r--   0        0        0      153 2024-05-12 10:07:44.221393 allianceauth-4.0.2/allianceauth/theme/apps.py
+-rw-r--r--   0        0        0        0 2024-05-12 10:07:44.372393 allianceauth-4.0.2/allianceauth/theme/bootstrap/__init__.py
+-rw-r--r--   0        0        0      241 2024-05-12 10:07:44.221393 allianceauth-4.0.2/allianceauth/theme/bootstrap/apps.py
+-rw-r--r--   0        0        0     1778 2024-05-12 10:07:44.221393 allianceauth-4.0.2/allianceauth/theme/bootstrap/auth_hooks.py
+-rw-r--r--   0        0        0        0 2024-05-12 10:07:44.372393 allianceauth-4.0.2/allianceauth/theme/darkly/__init__.py
+-rw-r--r--   0        0        0      240 2024-05-12 10:07:44.221393 allianceauth-4.0.2/allianceauth/theme/darkly/apps.py
+-rw-r--r--   0        0        0     1232 2024-05-12 10:07:44.221393 allianceauth-4.0.2/allianceauth/theme/darkly/auth_hooks.py
+-rw-r--r--   0        0        0        0 2024-05-12 10:07:44.372393 allianceauth-4.0.2/allianceauth/theme/flatly/__init__.py
+-rw-r--r--   0        0        0      240 2024-05-12 10:07:44.221393 allianceauth-4.0.2/allianceauth/theme/flatly/apps.py
+-rw-r--r--   0        0        0     1227 2024-05-12 10:07:44.221393 allianceauth-4.0.2/allianceauth/theme/flatly/auth_hooks.py
+-rw-r--r--   0        0        0     1537 2024-05-12 10:07:44.222393 allianceauth-4.0.2/allianceauth/theme/hooks.py
+-rw-r--r--   0        0        0        0 2024-05-12 10:07:44.372393 allianceauth-4.0.2/allianceauth/theme/materia/__init__.py
+-rw-r--r--   0        0        0      244 2024-05-12 10:07:44.222393 allianceauth-4.0.2/allianceauth/theme/materia/apps.py
+-rw-r--r--   0        0        0     1243 2024-05-12 10:07:44.222393 allianceauth-4.0.2/allianceauth/theme/materia/auth_hooks.py
+-rw-r--r--   0        0        0        0 2024-05-12 10:07:44.372393 allianceauth-4.0.2/allianceauth/theme/templates/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-12 10:07:44.372393 allianceauth-4.0.2/allianceauth/theme/templates/theme/__init__.py
+-rw-r--r--   0        0        0      389 2024-05-12 10:07:44.222393 allianceauth-4.0.2/allianceauth/theme/templates/theme/theme_imports_css.html
+-rw-r--r--   0        0        0      376 2024-05-12 10:07:44.222393 allianceauth-4.0.2/allianceauth/theme/templates/theme/theme_imports_js.html
+-rw-r--r--   0        0        0      494 2024-05-12 10:07:44.222393 allianceauth-4.0.2/allianceauth/theme/templates/theme/theme_select.html
+-rw-r--r--   0        0        0        0 2024-05-12 10:07:44.373393 allianceauth-4.0.2/allianceauth/theme/templatetags/__init__.py
+-rw-r--r--   0        0        0     1921 2024-05-12 10:07:44.222393 allianceauth-4.0.2/allianceauth/theme/templatetags/theme_tags.py
+-rw-r--r--   0        0        0        0 2024-05-12 10:07:44.373393 allianceauth-4.0.2/allianceauth/thirdparty/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-12 10:07:44.373393 allianceauth-4.0.2/allianceauth/thirdparty/navhelper/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-12 10:07:44.373393 allianceauth-4.0.2/allianceauth/thirdparty/navhelper/templatetags/__init__.py
+-rw-r--r--   0        0        0     2876 2024-05-12 10:07:44.223393 allianceauth-4.0.2/allianceauth/thirdparty/navhelper/templatetags/navactive.py
+-rw-r--r--   0        0        0     3407 2024-05-12 10:07:44.223393 allianceauth-4.0.2/allianceauth/thirdparty/navhelper/tests.py
+-rw-r--r--   0        0        0        0 2024-05-12 10:07:44.373393 allianceauth-4.0.2/allianceauth/timerboard/__init__.py
+-rw-r--r--   0        0        0      111 2024-05-12 10:07:44.223393 allianceauth-4.0.2/allianceauth/timerboard/admin.py
+-rw-r--r--   0        0        0      133 2024-05-12 10:07:44.223393 allianceauth-4.0.2/allianceauth/timerboard/apps.py
+-rw-r--r--   0        0        0     1141 2024-05-12 10:07:44.223393 allianceauth-4.0.2/allianceauth/timerboard/auth_hooks.py
+-rw-r--r--   0        0        0     5267 2024-05-12 10:07:44.223393 allianceauth-4.0.2/allianceauth/timerboard/form.py
+-rw-r--r--   0        0        0     1629 2024-05-12 10:07:44.223393 allianceauth-4.0.2/allianceauth/timerboard/migrations/0001_initial.py
+-rw-r--r--   0        0        0     1063 2024-05-12 10:07:44.223393 allianceauth-4.0.2/allianceauth/timerboard/migrations/0002_make_strings_more_stringy.py
+-rw-r--r--   0        0        0      763 2024-05-12 10:07:44.223393 allianceauth-4.0.2/allianceauth/timerboard/migrations/0003_on_delete.py
+-rw-r--r--   0        0        0      811 2024-05-12 10:07:44.223393 allianceauth-4.0.2/allianceauth/timerboard/migrations/0004_timer_type.py
+-rw-r--r--   0        0        0      410 2024-05-12 10:07:44.223393 allianceauth-4.0.2/allianceauth/timerboard/migrations/0005_alter_timer_planet_moon.py
+-rw-r--r--   0        0        0        0 2024-05-12 10:07:44.374393 allianceauth-4.0.2/allianceauth/timerboard/migrations/__init__.py
+-rw-r--r--   0        0        0     1593 2024-05-12 10:07:44.223393 allianceauth-4.0.2/allianceauth/timerboard/models.py
+-rw-r--r--   0        0        0     3069 2024-05-12 10:07:44.223393 allianceauth-4.0.2/allianceauth/timerboard/templates/timerboard/dashboard.timers.html
+-rw-r--r--   0        0        0     1917 2024-05-12 10:07:44.224393 allianceauth-4.0.2/allianceauth/timerboard/templates/timerboard/form.html
+-rw-r--r--   0        0        0      147 2024-05-12 10:07:44.224393 allianceauth-4.0.2/allianceauth/timerboard/templates/timerboard/index_button.html
+-rw-r--r--   0        0        0     1021 2024-05-12 10:07:44.224393 allianceauth-4.0.2/allianceauth/timerboard/templates/timerboard/timer_confirm_delete.html
+-rw-r--r--   0        0        0      810 2024-05-12 10:07:44.224393 allianceauth-4.0.2/allianceauth/timerboard/templates/timerboard/timer_create_form.html
+-rw-r--r--   0        0        0      830 2024-05-12 10:07:44.224393 allianceauth-4.0.2/allianceauth/timerboard/templates/timerboard/timer_update_form.html
+-rw-r--r--   0        0        0     8213 2024-05-12 10:07:44.224393 allianceauth-4.0.2/allianceauth/timerboard/templates/timerboard/timertable.html
+-rw-r--r--   0        0        0     5121 2024-05-12 10:07:44.224393 allianceauth-4.0.2/allianceauth/timerboard/templates/timerboard/view.html
+-rw-r--r--   0        0        0     8741 2024-05-12 10:07:44.224393 allianceauth-4.0.2/allianceauth/timerboard/tests.py
+-rw-r--r--   0        0        0      358 2024-05-12 10:07:44.224393 allianceauth-4.0.2/allianceauth/timerboard/urls.py
+-rw-r--r--   0        0        0     4075 2024-05-12 10:07:44.224393 allianceauth-4.0.2/allianceauth/timerboard/views.py
+-rw-r--r--   0        0        0     2688 2024-05-12 10:07:44.224393 allianceauth-4.0.2/allianceauth/urls.py
+-rw-r--r--   0        0        0        0 2024-05-12 10:07:44.374393 allianceauth-4.0.2/allianceauth/utils/__init__.py
+-rw-r--r--   0        0        0      568 2024-05-12 10:07:44.224393 allianceauth-4.0.2/allianceauth/utils/cache.py
+-rw-r--r--   0        0        0     1971 2024-05-12 10:07:44.225393 allianceauth-4.0.2/allianceauth/utils/counters.py
+-rw-r--r--   0        0        0      615 2024-05-12 10:07:44.225393 allianceauth-4.0.2/allianceauth/utils/django.py
+-rw-r--r--   0        0        0      844 2024-05-12 10:07:44.225393 allianceauth-4.0.2/allianceauth/utils/testing.py
+-rw-r--r--   0        0        0        0 2024-05-12 10:07:44.375393 allianceauth-4.0.2/allianceauth/utils/tests/__init__.py
+-rw-r--r--   0        0        0     1194 2024-05-12 10:07:44.225393 allianceauth-4.0.2/allianceauth/utils/tests/test_cache.py
+-rw-r--r--   0        0        0     3328 2024-05-12 10:07:44.225393 allianceauth-4.0.2/allianceauth/utils/tests/test_counters.py
+-rw-r--r--   0        0        0      777 2024-05-12 10:07:44.225393 allianceauth-4.0.2/allianceauth/utils/tests/test_django.py
+-rw-r--r--   0        0        0      310 2024-05-12 10:07:44.225393 allianceauth-4.0.2/allianceauth/utils/tests/test_testing.py
+-rw-r--r--   0        0        0     3289 2024-05-12 10:07:44.225393 allianceauth-4.0.2/allianceauth/views.py
+-rw-r--r--   0        0        0     2498 2024-05-12 10:07:44.248393 allianceauth-4.0.2/pyproject.toml
+-rw-r--r--   0        0        0     7491 1970-01-01 00:00:00.000000 allianceauth-4.0.2/PKG-INFO
```

### Comparing `allianceauth-4.0.1/LICENSE` & `allianceauth-4.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/README.md` & `allianceauth-4.0.2/README.md`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/analytics/migrations/0001_initial.py` & `allianceauth-4.0.2/allianceauth/analytics/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/analytics/migrations/0002_add_AA_Team_Token.py` & `allianceauth-4.0.2/allianceauth/analytics/migrations/0002_add_AA_Team_Token.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/analytics/migrations/0003_Generate_Identifier.py` & `allianceauth-4.0.2/allianceauth/analytics/migrations/0003_Generate_Identifier.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/analytics/migrations/0004_auto_20211015_0502.py` & `allianceauth-4.0.2/allianceauth/analytics/migrations/0004_auto_20211015_0502.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/analytics/migrations/0006_more_ignore_paths.py` & `allianceauth-4.0.2/allianceauth/analytics/migrations/0006_more_ignore_paths.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/analytics/migrations/0008_add_AA_GA-4_Team_Token .py` & `allianceauth-4.0.2/allianceauth/analytics/migrations/0008_add_AA_GA-4_Team_Token .py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/analytics/migrations/0009_remove_analyticstokens_ignore_paths_and_more.py` & `allianceauth-4.0.2/allianceauth/analytics/migrations/0009_remove_analyticstokens_ignore_paths_and_more.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/analytics/models.py` & `allianceauth-4.0.2/allianceauth/analytics/models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/analytics/tasks.py` & `allianceauth-4.0.2/allianceauth/analytics/tasks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/analytics/tests/test_models.py` & `allianceauth-4.0.2/allianceauth/analytics/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/analytics/tests/test_tasks.py` & `allianceauth-4.0.2/allianceauth/analytics/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/analytics/tests/test_utils.py` & `allianceauth-4.0.2/allianceauth/analytics/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/analytics/utils.py` & `allianceauth-4.0.2/allianceauth/analytics/utils.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/apps.py` & `allianceauth-4.0.2/allianceauth/apps.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/authentication/admin.py` & `allianceauth-4.0.2/allianceauth/authentication/admin.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/authentication/app_settings.py` & `allianceauth-4.0.2/allianceauth/authentication/app_settings.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/authentication/apps.py` & `allianceauth-4.0.2/allianceauth/authentication/apps.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/authentication/auth_hooks.py` & `allianceauth-4.0.2/allianceauth/authentication/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/authentication/backends.py` & `allianceauth-4.0.2/allianceauth/authentication/backends.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/authentication/constants.py` & `allianceauth-4.0.2/allianceauth/authentication/constants.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/authentication/core/celery_workers.py` & `allianceauth-4.0.2/allianceauth/authentication/core/celery_workers.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/authentication/decorators.py` & `allianceauth-4.0.2/allianceauth/authentication/decorators.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/authentication/forms.py` & `allianceauth-4.0.2/allianceauth/authentication/forms.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/authentication/hmac_urls.py` & `allianceauth-4.0.2/allianceauth/authentication/hmac_urls.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/authentication/management/commands/checkmains.py` & `allianceauth-4.0.2/allianceauth/authentication/management/commands/checkmains.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/authentication/managers.py` & `allianceauth-4.0.2/allianceauth/authentication/managers.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/authentication/middleware.py` & `allianceauth-4.0.2/allianceauth/authentication/middleware.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/authentication/migrations/0001_initial.py` & `allianceauth-4.0.2/allianceauth/authentication/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/authentication/migrations/0004_create_permissions.py` & `allianceauth-4.0.2/allianceauth/authentication/migrations/0004_create_permissions.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/authentication/migrations/0005_delete_perms.py` & `allianceauth-4.0.2/allianceauth/authentication/migrations/0005_delete_perms.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/authentication/migrations/0006_auto_20160910_0542.py` & `allianceauth-4.0.2/allianceauth/authentication/migrations/0006_auto_20160910_0542.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/authentication/migrations/0009_auto_20161021_0228.py` & `allianceauth-4.0.2/allianceauth/authentication/migrations/0009_auto_20161021_0228.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/authentication/migrations/0010_only_one_authservicesinfo.py` & `allianceauth-4.0.2/allianceauth/authentication/migrations/0010_only_one_authservicesinfo.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/authentication/migrations/0011_authservicesinfo_user_onetoonefield.py` & `allianceauth-4.0.2/allianceauth/authentication/migrations/0011_authservicesinfo_user_onetoonefield.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/authentication/migrations/0012_remove_add_delete_authservicesinfo_permissions.py` & `allianceauth-4.0.2/allianceauth/authentication/migrations/0012_remove_add_delete_authservicesinfo_permissions.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/authentication/migrations/0013_service_modules.py` & `allianceauth-4.0.2/allianceauth/authentication/migrations/0013_service_modules.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/authentication/migrations/0014_fleetup_permission.py` & `allianceauth-4.0.2/allianceauth/authentication/migrations/0014_fleetup_permission.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/authentication/migrations/0015_user_profiles.py` & `allianceauth-4.0.2/allianceauth/authentication/migrations/0015_user_profiles.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/authentication/migrations/0016_ownershiprecord.py` & `allianceauth-4.0.2/allianceauth/authentication/migrations/0016_ownershiprecord.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/authentication/migrations/0017_remove_fleetup_permission.py` & `allianceauth-4.0.2/allianceauth/authentication/migrations/0017_remove_fleetup_permission.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/authentication/migrations/0018_state_member_factions.py` & `allianceauth-4.0.2/allianceauth/authentication/migrations/0018_state_member_factions.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/authentication/migrations/0020_userprofile_language_userprofile_night_mode.py` & `allianceauth-4.0.2/allianceauth/authentication/migrations/0020_userprofile_language_userprofile_night_mode.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/authentication/migrations/0021_alter_userprofile_language.py` & `allianceauth-4.0.2/allianceauth/authentication/migrations/0021_alter_userprofile_language.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/authentication/migrations/0022_userprofile_theme.py` & `allianceauth-4.0.2/allianceauth/authentication/migrations/0022_userprofile_theme.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/authentication/models.py` & `allianceauth-4.0.2/allianceauth/authentication/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,14 +74,15 @@
         CHINESE = 'zh-hans', _('Chinese Simplified')
         RUSSIAN = 'ru', _('Russian')
         KOREAN = 'ko', _('Korean')
         FRENCH = 'fr', _('French')
         JAPANESE = 'ja', _('Japanese')
         ITALIAN = 'it', _('Italian')
         UKRAINIAN = 'uk', _('Ukrainian')
+        POLISH = 'pl', _("Polish")
 
     user = models.OneToOneField(
         User,
         related_name='profile',
         on_delete=models.CASCADE)
     main_character = models.OneToOneField(
         EveCharacter,
```

### Comparing `allianceauth-4.0.1/allianceauth/authentication/signals.py` & `allianceauth-4.0.2/allianceauth/authentication/signals.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/authentication/static/allianceauth/authentication/img/background.jpg` & `allianceauth-4.0.2/allianceauth/authentication/static/allianceauth/authentication/img/background.jpg`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/authentication/static/allianceauth/authentication/img/sso/EVE_SSO_Login_Buttons_Large_Black.png` & `allianceauth-4.0.2/allianceauth/authentication/static/allianceauth/authentication/img/sso/EVE_SSO_Login_Buttons_Large_Black.png`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/authentication/static/allianceauth/authentication/img/sso/EVE_SSO_Login_Buttons_Large_White.png` & `allianceauth-4.0.2/allianceauth/authentication/static/allianceauth/authentication/img/sso/EVE_SSO_Login_Buttons_Large_White.png`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/authentication/task_statistics/counters.py` & `allianceauth-4.0.2/allianceauth/authentication/task_statistics/counters.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/authentication/task_statistics/event_series.py` & `allianceauth-4.0.2/allianceauth/authentication/task_statistics/event_series.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/authentication/task_statistics/helpers.py` & `allianceauth-4.0.2/allianceauth/authentication/task_statistics/helpers.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/authentication/task_statistics/signals.py` & `allianceauth-4.0.2/allianceauth/authentication/task_statistics/signals.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/authentication/task_statistics/tests/test_counters.py` & `allianceauth-4.0.2/allianceauth/authentication/task_statistics/tests/test_counters.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/authentication/task_statistics/tests/test_event_series.py` & `allianceauth-4.0.2/allianceauth/authentication/task_statistics/tests/test_event_series.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/authentication/task_statistics/tests/test_helpers.py` & `allianceauth-4.0.2/allianceauth/authentication/task_statistics/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/authentication/task_statistics/tests/test_signals.py` & `allianceauth-4.0.2/allianceauth/authentication/task_statistics/tests/test_signals.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/authentication/tasks.py` & `allianceauth-4.0.2/allianceauth/authentication/tasks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/authentication/templates/authentication/dashboard_characters.html` & `allianceauth-4.0.2/allianceauth/authentication/templates/authentication/dashboard_characters.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/authentication/templates/authentication/dashboard_groups.html` & `allianceauth-4.0.2/allianceauth/authentication/templates/authentication/dashboard_groups.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/authentication/templates/authentication/tokens.html` & `allianceauth-4.0.2/allianceauth/authentication/templates/authentication/tokens.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/authentication/templates/public/base.html` & `allianceauth-4.0.2/allianceauth/authentication/templates/public/base.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/authentication/templates/public/lang_select.html` & `allianceauth-4.0.2/allianceauth/authentication/templates/public/lang_select.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/authentication/templates/public/middle_box.html` & `allianceauth-4.0.2/allianceauth/authentication/templates/public/middle_box.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/authentication/templates/public/register.html` & `allianceauth-4.0.2/allianceauth/authentication/templates/public/register.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/authentication/tests/__init__.py` & `allianceauth-4.0.2/allianceauth/authentication/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/authentication/tests/core/test_celery_workers.py` & `allianceauth-4.0.2/allianceauth/authentication/tests/core/test_celery_workers.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/authentication/tests/test_admin.py` & `allianceauth-4.0.2/allianceauth/authentication/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/authentication/tests/test_app_settings.py` & `allianceauth-4.0.2/allianceauth/authentication/tests/test_app_settings.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/authentication/tests/test_backend.py` & `allianceauth-4.0.2/allianceauth/authentication/tests/test_backend.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/authentication/tests/test_commands.py` & `allianceauth-4.0.2/allianceauth/authentication/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/authentication/tests/test_decorators.py` & `allianceauth-4.0.2/allianceauth/authentication/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/authentication/tests/test_middleware.py` & `allianceauth-4.0.2/allianceauth/authentication/tests/test_middleware.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/authentication/tests/test_models.py` & `allianceauth-4.0.2/allianceauth/authentication/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/authentication/tests/test_signals.py` & `allianceauth-4.0.2/allianceauth/authentication/tests/test_signals.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/authentication/tests/test_templatetags.py` & `allianceauth-4.0.2/allianceauth/authentication/tests/test_templatetags.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/authentication/tests/test_views.py` & `allianceauth-4.0.2/allianceauth/authentication/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/authentication/urls.py` & `allianceauth-4.0.2/allianceauth/authentication/urls.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/authentication/views.py` & `allianceauth-4.0.2/allianceauth/authentication/views.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/bin/allianceauth.py` & `allianceauth-4.0.2/allianceauth/bin/allianceauth.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/corputils/auth_hooks.py` & `allianceauth-4.0.2/allianceauth/corputils/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/corputils/managers.py` & `allianceauth-4.0.2/allianceauth/corputils/managers.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/corputils/migrations/0001_initial.py` & `allianceauth-4.0.2/allianceauth/corputils/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/corputils/migrations/0002_migrate_permissions.py` & `allianceauth-4.0.2/allianceauth/corputils/migrations/0002_migrate_permissions.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/corputils/migrations/0003_granular_permissions.py` & `allianceauth-4.0.2/allianceauth/corputils/migrations/0003_granular_permissions.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/corputils/migrations/0004_member_models.py` & `allianceauth-4.0.2/allianceauth/corputils/migrations/0004_member_models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/corputils/migrations/0005_cleanup_permissions.py` & `allianceauth-4.0.2/allianceauth/corputils/migrations/0005_cleanup_permissions.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/corputils/models.py` & `allianceauth-4.0.2/allianceauth/corputils/models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/corputils/swagger.json` & `allianceauth-4.0.2/allianceauth/corputils/swagger.json`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/corputils/templates/corputils/base.html` & `allianceauth-4.0.2/allianceauth/corputils/templates/corputils/base.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/corputils/templates/corputils/corpstats.html` & `allianceauth-4.0.2/allianceauth/corputils/templates/corputils/corpstats.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/corputils/templates/corputils/search.html` & `allianceauth-4.0.2/allianceauth/corputils/templates/corputils/search.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/corputils/tests.py` & `allianceauth-4.0.2/allianceauth/corputils/tests.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/corputils/views.py` & `allianceauth-4.0.2/allianceauth/corputils/views.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/eveonline/admin.py` & `allianceauth-4.0.2/allianceauth/eveonline/admin.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/eveonline/autogroups/admin.py` & `allianceauth-4.0.2/allianceauth/eveonline/autogroups/admin.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/eveonline/autogroups/migrations/0001_initial.py` & `allianceauth-4.0.2/allianceauth/eveonline/autogroups/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/eveonline/autogroups/models.py` & `allianceauth-4.0.2/allianceauth/eveonline/autogroups/models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/eveonline/autogroups/signals.py` & `allianceauth-4.0.2/allianceauth/eveonline/autogroups/signals.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/eveonline/autogroups/tests/__init__.py` & `allianceauth-4.0.2/allianceauth/eveonline/autogroups/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/eveonline/autogroups/tests/test_managers.py` & `allianceauth-4.0.2/allianceauth/eveonline/autogroups/tests/test_managers.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/eveonline/autogroups/tests/test_models.py` & `allianceauth-4.0.2/allianceauth/eveonline/autogroups/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/eveonline/autogroups/tests/test_signals.py` & `allianceauth-4.0.2/allianceauth/eveonline/autogroups/tests/test_signals.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/eveonline/evelinks/__init__.py` & `allianceauth-4.0.2/allianceauth/eveonline/evelinks/__init__.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/eveonline/evelinks/dotlan.py` & `allianceauth-4.0.2/allianceauth/eveonline/evelinks/dotlan.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/eveonline/evelinks/eveimageserver.py` & `allianceauth-4.0.2/allianceauth/eveonline/evelinks/eveimageserver.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/eveonline/evelinks/evewho.py` & `allianceauth-4.0.2/allianceauth/eveonline/evelinks/evewho.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/eveonline/evelinks/tests/test_evelinks.py` & `allianceauth-4.0.2/allianceauth/eveonline/evelinks/tests/test_evelinks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/eveonline/evelinks/tests/test_templatetags.py` & `allianceauth-4.0.2/allianceauth/eveonline/evelinks/tests/test_templatetags.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/eveonline/evelinks/zkillboard.py` & `allianceauth-4.0.2/allianceauth/eveonline/evelinks/zkillboard.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/eveonline/managers.py` & `allianceauth-4.0.2/allianceauth/eveonline/managers.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/eveonline/migrations/0001_initial.py` & `allianceauth-4.0.2/allianceauth/eveonline/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/eveonline/migrations/0003_auto_20161026_0149.py` & `allianceauth-4.0.2/allianceauth/eveonline/migrations/0003_auto_20161026_0149.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/eveonline/migrations/0006_allow_null_evecharacter_alliance.py` & `allianceauth-4.0.2/allianceauth/eveonline/migrations/0006_allow_null_evecharacter_alliance.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/eveonline/migrations/0007_unique_id_name.py` & `allianceauth-4.0.2/allianceauth/eveonline/migrations/0007_unique_id_name.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/eveonline/migrations/0008_remove_apikeys.py` & `allianceauth-4.0.2/allianceauth/eveonline/migrations/0008_remove_apikeys.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/eveonline/migrations/0009_on_delete.py` & `allianceauth-4.0.2/allianceauth/eveonline/migrations/0009_on_delete.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/eveonline/migrations/0010_alliance_ticker.py` & `allianceauth-4.0.2/allianceauth/eveonline/migrations/0010_alliance_ticker.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/eveonline/migrations/0011_ids_to_integers.py` & `allianceauth-4.0.2/allianceauth/eveonline/migrations/0011_ids_to_integers.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/eveonline/migrations/0012_index_additions.py` & `allianceauth-4.0.2/allianceauth/eveonline/migrations/0012_index_additions.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/eveonline/migrations/0015_factions.py` & `allianceauth-4.0.2/allianceauth/eveonline/migrations/0015_factions.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/eveonline/migrations/0017_alliance_and_corp_names_are_not_unique.py` & `allianceauth-4.0.2/allianceauth/eveonline/migrations/0017_alliance_and_corp_names_are_not_unique.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/eveonline/models.py` & `allianceauth-4.0.2/allianceauth/eveonline/models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/eveonline/providers.py` & `allianceauth-4.0.2/allianceauth/eveonline/providers.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/eveonline/swagger.json` & `allianceauth-4.0.2/allianceauth/eveonline/swagger.json`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/eveonline/tasks.py` & `allianceauth-4.0.2/allianceauth/eveonline/tasks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/eveonline/templatetags/evelinks.py` & `allianceauth-4.0.2/allianceauth/eveonline/templatetags/evelinks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/eveonline/templatetags/examples.html` & `allianceauth-4.0.2/allianceauth/eveonline/templatetags/examples.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/eveonline/tests/__init__.py` & `allianceauth-4.0.2/allianceauth/eveonline/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/eveonline/tests/esi_client_stub.py` & `allianceauth-4.0.2/allianceauth/eveonline/tests/esi_client_stub.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/eveonline/tests/swagger_old.json` & `allianceauth-4.0.2/allianceauth/eveonline/tests/swagger_old.json`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/eveonline/tests/test_managers.py` & `allianceauth-4.0.2/allianceauth/eveonline/tests/test_managers.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/eveonline/tests/test_models.py` & `allianceauth-4.0.2/allianceauth/eveonline/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/eveonline/tests/test_providers.py` & `allianceauth-4.0.2/allianceauth/eveonline/tests/test_providers.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/eveonline/tests/test_tasks.py` & `allianceauth-4.0.2/allianceauth/eveonline/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/fleetactivitytracking/migrations/0001_initial.py` & `allianceauth-4.0.2/allianceauth/fleetactivitytracking/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/fleetactivitytracking/migrations/0007_sentinel_user.py` & `allianceauth-4.0.2/allianceauth/fleetactivitytracking/migrations/0007_sentinel_user.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/fleetactivitytracking/models.py` & `allianceauth-4.0.2/allianceauth/fleetactivitytracking/models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/fleetactivitytracking/swagger.json` & `allianceauth-4.0.2/allianceauth/fleetactivitytracking/swagger.json`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/characternotexisting.html` & `allianceauth-4.0.2/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/characternotexisting.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/fatlinkcreate.html` & `allianceauth-4.0.2/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/fatlinkcreate.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/fatlinkmodify.html` & `allianceauth-4.0.2/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/fatlinkmodify.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/fatlinkpersonalmonthlystatisticsview.html` & `allianceauth-4.0.2/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/fatlinkpersonalmonthlystatisticsview.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/fatlinkpersonalstatisticsview.html` & `allianceauth-4.0.2/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/fatlinkpersonalstatisticsview.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/fatlinkstatisticscorpview.html` & `allianceauth-4.0.2/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/fatlinkstatisticscorpview.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/fatlinkstatisticsview.html` & `allianceauth-4.0.2/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/fatlinkstatisticsview.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/fatlinkview.html` & `allianceauth-4.0.2/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/fatlinkview.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/fleetactivitytracking/urls.py` & `allianceauth-4.0.2/allianceauth/fleetactivitytracking/urls.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/fleetactivitytracking/views.py` & `allianceauth-4.0.2/allianceauth/fleetactivitytracking/views.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/framework/api/evecharacter.py` & `allianceauth-4.0.2/allianceauth/framework/api/evecharacter.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/framework/api/user.py` & `allianceauth-4.0.2/allianceauth/framework/api/user.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/framework/static/allianceauth/framework/css/auth-framework.css` & `allianceauth-4.0.2/allianceauth/framework/static/allianceauth/framework/css/auth-framework.css`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/framework/tests/test_api_user.py` & `allianceauth-4.0.2/allianceauth/framework/tests/test_api_user.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/groupmanagement/admin.py` & `allianceauth-4.0.2/allianceauth/groupmanagement/admin.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/groupmanagement/auth_hooks.py` & `allianceauth-4.0.2/allianceauth/groupmanagement/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/groupmanagement/forms.py` & `allianceauth-4.0.2/allianceauth/groupmanagement/forms.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/groupmanagement/managers.py` & `allianceauth-4.0.2/allianceauth/groupmanagement/managers.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/groupmanagement/migrations/0001_initial.py` & `allianceauth-4.0.2/allianceauth/groupmanagement/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/groupmanagement/migrations/0002_auto_20160906_2354.py` & `allianceauth-4.0.2/allianceauth/groupmanagement/migrations/0002_auto_20160906_2354.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/groupmanagement/migrations/0004_authgroup.py` & `allianceauth-4.0.2/allianceauth/groupmanagement/migrations/0004_authgroup.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/groupmanagement/migrations/0005_authgroup_public.py` & `allianceauth-4.0.2/allianceauth/groupmanagement/migrations/0005_authgroup_public.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/groupmanagement/migrations/0006_request_groups_perm.py` & `allianceauth-4.0.2/allianceauth/groupmanagement/migrations/0006_request_groups_perm.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/groupmanagement/migrations/0007_on_delete.py` & `allianceauth-4.0.2/allianceauth/groupmanagement/migrations/0007_on_delete.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/groupmanagement/migrations/0008_remove_authgroup_permissions.py` & `allianceauth-4.0.2/allianceauth/groupmanagement/migrations/0008_remove_authgroup_permissions.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/groupmanagement/migrations/0009_requestlog.py` & `allianceauth-4.0.2/allianceauth/groupmanagement/migrations/0009_requestlog.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/groupmanagement/migrations/0010_authgroup_states.py` & `allianceauth-4.0.2/allianceauth/groupmanagement/migrations/0010_authgroup_states.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/groupmanagement/migrations/0012_group_leads.py` & `allianceauth-4.0.2/allianceauth/groupmanagement/migrations/0012_group_leads.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/groupmanagement/migrations/0015_make_descriptions_great_again.py` & `allianceauth-4.0.2/allianceauth/groupmanagement/migrations/0015_make_descriptions_great_again.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/groupmanagement/migrations/0017_improve_groups_documentation.py` & `allianceauth-4.0.2/allianceauth/groupmanagement/migrations/0017_improve_groups_documentation.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/groupmanagement/migrations/0018_reservedgroupname.py` & `allianceauth-4.0.2/allianceauth/groupmanagement/migrations/0018_reservedgroupname.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/groupmanagement/migrations/0019_adding_restricted_to_groups.py` & `allianceauth-4.0.2/allianceauth/groupmanagement/migrations/0019_adding_restricted_to_groups.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/groupmanagement/models.py` & `allianceauth-4.0.2/allianceauth/groupmanagement/models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/groupmanagement/signals.py` & `allianceauth-4.0.2/allianceauth/groupmanagement/signals.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/groupmanagement/templates/groupmanagement/audit.html` & `allianceauth-4.0.2/allianceauth/groupmanagement/templates/groupmanagement/audit.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/groupmanagement/templates/groupmanagement/groupmembers.html` & `allianceauth-4.0.2/allianceauth/groupmanagement/templates/groupmanagement/groupmembers.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/groupmanagement/templates/groupmanagement/groupmembership.html` & `allianceauth-4.0.2/allianceauth/groupmanagement/templates/groupmanagement/groupmembership.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/groupmanagement/templates/groupmanagement/groups.html` & `allianceauth-4.0.2/allianceauth/groupmanagement/templates/groupmanagement/groups.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/groupmanagement/templates/groupmanagement/index.html` & `allianceauth-4.0.2/allianceauth/groupmanagement/templates/groupmanagement/index.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/groupmanagement/tests/test_admin.py` & `allianceauth-4.0.2/allianceauth/groupmanagement/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/groupmanagement/tests/test_managers.py` & `allianceauth-4.0.2/allianceauth/groupmanagement/tests/test_managers.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/groupmanagement/tests/test_models.py` & `allianceauth-4.0.2/allianceauth/groupmanagement/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/groupmanagement/tests/test_signals.py` & `allianceauth-4.0.2/allianceauth/groupmanagement/tests/test_signals.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/groupmanagement/tests/test_views.py` & `allianceauth-4.0.2/allianceauth/groupmanagement/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/groupmanagement/urls.py` & `allianceauth-4.0.2/allianceauth/groupmanagement/urls.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/groupmanagement/views.py` & `allianceauth-4.0.2/allianceauth/groupmanagement/views.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/hooks.py` & `allianceauth-4.0.2/allianceauth/hooks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/hrapplications/admin.py` & `allianceauth-4.0.2/allianceauth/hrapplications/admin.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/hrapplications/auth_hooks.py` & `allianceauth-4.0.2/allianceauth/hrapplications/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/hrapplications/managers.py` & `allianceauth-4.0.2/allianceauth/hrapplications/managers.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/hrapplications/migrations/0001_initial.py` & `allianceauth-4.0.2/allianceauth/hrapplications/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/hrapplications/migrations/0002_choices_for_questions.py` & `allianceauth-4.0.2/allianceauth/hrapplications/migrations/0002_choices_for_questions.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/hrapplications/migrations/0004_make_strings_more_stringy.py` & `allianceauth-4.0.2/allianceauth/hrapplications/migrations/0004_make_strings_more_stringy.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/hrapplications/migrations/0005_sorted_questions.py` & `allianceauth-4.0.2/allianceauth/hrapplications/migrations/0005_sorted_questions.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/hrapplications/migrations/0006_remove_legacy_models.py` & `allianceauth-4.0.2/allianceauth/hrapplications/migrations/0006_remove_legacy_models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/hrapplications/models.py` & `allianceauth-4.0.2/allianceauth/hrapplications/models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/hrapplications/templates/hrapplications/corpchoice.html` & `allianceauth-4.0.2/allianceauth/hrapplications/templates/hrapplications/corpchoice.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/hrapplications/templates/hrapplications/create.html` & `allianceauth-4.0.2/allianceauth/hrapplications/templates/hrapplications/create.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/hrapplications/templates/hrapplications/management.html` & `allianceauth-4.0.2/allianceauth/hrapplications/templates/hrapplications/management.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/hrapplications/templates/hrapplications/partials/modals/search.html` & `allianceauth-4.0.2/allianceauth/hrapplications/templates/hrapplications/partials/modals/search.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/hrapplications/templates/hrapplications/searchview.html` & `allianceauth-4.0.2/allianceauth/hrapplications/templates/hrapplications/searchview.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/hrapplications/templates/hrapplications/view.html` & `allianceauth-4.0.2/allianceauth/hrapplications/templates/hrapplications/view.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/hrapplications/tests.py` & `allianceauth-4.0.2/allianceauth/hrapplications/tests.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/hrapplications/urls.py` & `allianceauth-4.0.2/allianceauth/hrapplications/urls.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/hrapplications/views.py` & `allianceauth-4.0.2/allianceauth/hrapplications/views.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/locale/de/LC_MESSAGES/django.mo` & `allianceauth-4.0.2/allianceauth/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/locale/de/LC_MESSAGES/django.po` & `allianceauth-4.0.2/allianceauth/locale/de/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Peter Pfeufer, 2024
 # 
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-03-13 19:10+1000\n"
+"POT-Creation-Date: 2024-05-12 19:15+1000\n"
 "PO-Revision-Date: 2023-11-08 13:50+0000\n"
 "Last-Translator: Peter Pfeufer, 2024\n"
 "Language-Team: German (https://app.transifex.com/alliance-auth/teams/107430/de/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: de\n"
@@ -1445,14 +1445,16 @@
 msgstr "Admin"
 
 #: allianceauth/menu/templates/menu/menu-user.html:80
 msgid "Sign Out"
 msgstr "Ausloggen"
 
 #: allianceauth/menu/templates/menu/menu-user.html:84
+#: allianceauth/templates/allianceauth/top-menu-rh-default.html:17
+#: allianceauth/templates/allianceauth/top-menu-rh-default.html:18
 msgid "Sign In"
 msgstr "Einloggen"
 
 #: allianceauth/notifications/models.py:21
 msgid "danger"
 msgstr "Gefahr"
```

### Comparing `allianceauth-4.0.1/allianceauth/locale/en/LC_MESSAGES/django.po` & `allianceauth-4.0.2/allianceauth/locale/en/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 000000c0: 232c 2066 757a 7a79 0a6d 7367 6964 2022  #, fuzzy.msgid "
 000000d0: 220a 6d73 6773 7472 2022 220a 2250 726f  ".msgstr ""."Pro
 000000e0: 6a65 6374 2d49 642d 5665 7273 696f 6e3a  ject-Id-Version:
 000000f0: 2050 4143 4b41 4745 2056 4552 5349 4f4e   PACKAGE VERSION
 00000100: 5c6e 220a 2252 6570 6f72 742d 4d73 6769  \n"."Report-Msgi
 00000110: 642d 4275 6773 2d54 6f3a 205c 6e22 0a22  d-Bugs-To: \n"."
 00000120: 504f 542d 4372 6561 7469 6f6e 2d44 6174  POT-Creation-Dat
-00000130: 653a 2032 3032 342d 3033 2d31 3320 3139  e: 2024-03-13 19
-00000140: 3a31 302b 3130 3030 5c6e 220a 2250 4f2d  :10+1000\n"."PO-
+00000130: 653a 2032 3032 342d 3035 2d31 3220 3139  e: 2024-05-12 19
+00000140: 3a31 352b 3130 3030 5c6e 220a 2250 4f2d  :15+1000\n"."PO-
 00000150: 5265 7669 7369 6f6e 2d44 6174 653a 2059  Revision-Date: Y
 00000160: 4541 522d 4d4f 2d44 4120 484f 3a4d 492b  EAR-MO-DA HO:MI+
 00000170: 5a4f 4e45 5c6e 220a 224c 6173 742d 5472  ZONE\n"."Last-Tr
 00000180: 616e 736c 6174 6f72 3a20 4655 4c4c 204e  anslator: FULL N
 00000190: 414d 4520 3c45 4d41 494c 4041 4444 5245  AME <EMAIL@ADDRE
 000001a0: 5353 3e5c 6e22 0a22 4c61 6e67 7561 6765  SS>\n"."Language
 000001b0: 2d54 6561 6d3a 204c 414e 4755 4147 4520  -Team: LANGUAGE 
@@ -2917,2278 +2917,2287 @@
 0000b640: 7468 2f6d 656e 752f 7465 6d70 6c61 7465  th/menu/template
 0000b650: 732f 6d65 6e75 2f6d 656e 752d 7573 6572  s/menu/menu-user
 0000b660: 2e68 746d 6c3a 3830 0a6d 7367 6964 2022  .html:80.msgid "
 0000b670: 5369 676e 204f 7574 220a 6d73 6773 7472  Sign Out".msgstr
 0000b680: 2022 220a 0a23 3a20 616c 6c69 616e 6365   ""..#: alliance
 0000b690: 6175 7468 2f6d 656e 752f 7465 6d70 6c61  auth/menu/templa
 0000b6a0: 7465 732f 6d65 6e75 2f6d 656e 752d 7573  tes/menu/menu-us
-0000b6b0: 6572 2e68 746d 6c3a 3834 0a6d 7367 6964  er.html:84.msgid
-0000b6c0: 2022 5369 676e 2049 6e22 0a6d 7367 7374   "Sign In".msgst
-0000b6d0: 7220 2222 0a0a 233a 2061 6c6c 6961 6e63  r ""..#: allianc
-0000b6e0: 6561 7574 682f 6e6f 7469 6669 6361 7469  eauth/notificati
-0000b6f0: 6f6e 732f 6d6f 6465 6c73 2e70 793a 3231  ons/models.py:21
-0000b700: 0a6d 7367 6964 2022 6461 6e67 6572 220a  .msgid "danger".
-0000b710: 6d73 6773 7472 2022 220a 0a23 3a20 616c  msgstr ""..#: al
-0000b720: 6c69 616e 6365 6175 7468 2f6e 6f74 6966  lianceauth/notif
-0000b730: 6963 6174 696f 6e73 2f6d 6f64 656c 732e  ications/models.
-0000b740: 7079 3a32 320a 6d73 6769 6420 2277 6172  py:22.msgid "war
-0000b750: 6e69 6e67 220a 6d73 6773 7472 2022 220a  ning".msgstr "".
-0000b760: 0a23 3a20 616c 6c69 616e 6365 6175 7468  .#: allianceauth
-0000b770: 2f6e 6f74 6966 6963 6174 696f 6e73 2f6d  /notifications/m
-0000b780: 6f64 656c 732e 7079 3a32 330a 6d73 6769  odels.py:23.msgi
-0000b790: 6420 2269 6e66 6f22 0a6d 7367 7374 7220  d "info".msgstr 
-0000b7a0: 2222 0a0a 233a 2061 6c6c 6961 6e63 6561  ""..#: alliancea
-0000b7b0: 7574 682f 6e6f 7469 6669 6361 7469 6f6e  uth/notification
-0000b7c0: 732f 6d6f 6465 6c73 2e70 793a 3234 0a6d  s/models.py:24.m
-0000b7d0: 7367 6964 2022 7375 6363 6573 7322 0a6d  sgid "success".m
-0000b7e0: 7367 7374 7220 2222 0a0a 233a 2061 6c6c  sgstr ""..#: all
-0000b7f0: 6961 6e63 6561 7574 682f 6e6f 7469 6669  ianceauth/notifi
-0000b800: 6361 7469 6f6e 732f 7465 6d70 6c61 7465  cations/template
-0000b810: 732f 6e6f 7469 6669 6361 7469 6f6e 732f  s/notifications/
-0000b820: 6c69 7374 2e68 746d 6c3a 3137 0a6d 7367  list.html:17.msg
-0000b830: 6964 2022 556e 7265 6164 220a 6d73 6773  id "Unread".msgs
-0000b840: 7472 2022 220a 0a23 3a20 616c 6c69 616e  tr ""..#: allian
-0000b850: 6365 6175 7468 2f6e 6f74 6966 6963 6174  ceauth/notificat
-0000b860: 696f 6e73 2f74 656d 706c 6174 6573 2f6e  ions/templates/n
-0000b870: 6f74 6966 6963 6174 696f 6e73 2f6c 6973  otifications/lis
-0000b880: 742e 6874 6d6c 3a32 340a 6d73 6769 6420  t.html:24.msgid 
-0000b890: 2252 6561 6422 0a6d 7367 7374 7220 2222  "Read".msgstr ""
-0000b8a0: 0a0a 233a 2061 6c6c 6961 6e63 6561 7574  ..#: allianceaut
-0000b8b0: 682f 6e6f 7469 6669 6361 7469 6f6e 732f  h/notifications/
-0000b8c0: 7465 6d70 6c61 7465 732f 6e6f 7469 6669  templates/notifi
-0000b8d0: 6361 7469 6f6e 732f 6c69 7374 2e68 746d  cations/list.htm
-0000b8e0: 6c3a 3332 0a6d 7367 6964 2022 4d61 726b  l:32.msgid "Mark
-0000b8f0: 2061 6c6c 206e 6f74 6966 6963 6174 696f   all notificatio
-0000b900: 6e73 2061 7320 7265 6164 220a 6d73 6773  ns as read".msgs
-0000b910: 7472 2022 220a 0a23 3a20 616c 6c69 616e  tr ""..#: allian
-0000b920: 6365 6175 7468 2f6e 6f74 6966 6963 6174  ceauth/notificat
-0000b930: 696f 6e73 2f74 656d 706c 6174 6573 2f6e  ions/templates/n
-0000b940: 6f74 6966 6963 6174 696f 6e73 2f6c 6973  otifications/lis
-0000b950: 742e 6874 6d6c 3a33 380a 6d73 6769 6420  t.html:38.msgid 
-0000b960: 2244 656c 6574 6520 616c 6c20 7265 6164  "Delete all read
-0000b970: 206e 6f74 6966 6963 6174 696f 6e73 220a   notifications".
-0000b980: 6d73 6773 7472 2022 220a 0a23 3a20 616c  msgstr ""..#: al
-0000b990: 6c69 616e 6365 6175 7468 2f6e 6f74 6966  lianceauth/notif
-0000b9a0: 6963 6174 696f 6e73 2f74 656d 706c 6174  ications/templat
-0000b9b0: 6573 2f6e 6f74 6966 6963 6174 696f 6e73  es/notifications
-0000b9c0: 2f6c 6973 745f 7061 7274 6961 6c2e 6874  /list_partial.ht
-0000b9d0: 6d6c 3a36 0a6d 7367 6964 2022 5469 6d65  ml:6.msgid "Time
-0000b9e0: 7374 616d 7022 0a6d 7367 7374 7220 2222  stamp".msgstr ""
-0000b9f0: 0a0a 233a 2061 6c6c 6961 6e63 6561 7574  ..#: allianceaut
-0000ba00: 682f 6e6f 7469 6669 6361 7469 6f6e 732f  h/notifications/
-0000ba10: 7465 6d70 6c61 7465 732f 6e6f 7469 6669  templates/notifi
-0000ba20: 6361 7469 6f6e 732f 6c69 7374 5f70 6172  cations/list_par
-0000ba30: 7469 616c 2e68 746d 6c3a 370a 6d73 6769  tial.html:7.msgi
-0000ba40: 6420 2254 6974 6c65 220a 6d73 6773 7472  d "Title".msgstr
-0000ba50: 2022 220a 0a23 3a20 616c 6c69 616e 6365   ""..#: alliance
-0000ba60: 6175 7468 2f6e 6f74 6966 6963 6174 696f  auth/notificatio
-0000ba70: 6e73 2f74 656d 706c 6174 6573 2f6e 6f74  ns/templates/not
-0000ba80: 6966 6963 6174 696f 6e73 2f6c 6973 745f  ifications/list_
-0000ba90: 7061 7274 6961 6c2e 6874 6d6c 3a32 380a  partial.html:28.
-0000baa0: 6d73 6769 6420 224e 6f20 6e6f 7469 6669  msgid "No notifi
-0000bab0: 6361 7469 6f6e 732e 220a 6d73 6773 7472  cations.".msgstr
-0000bac0: 2022 220a 0a23 3a20 616c 6c69 616e 6365   ""..#: alliance
-0000bad0: 6175 7468 2f6e 6f74 6966 6963 6174 696f  auth/notificatio
-0000bae0: 6e73 2f74 656d 706c 6174 6573 2f6e 6f74  ns/templates/not
-0000baf0: 6966 6963 6174 696f 6e73 2f76 6965 772e  ifications/view.
-0000bb00: 6874 6d6c 3a35 0a23 3a20 616c 6c69 616e  html:5.#: allian
-0000bb10: 6365 6175 7468 2f6e 6f74 6966 6963 6174  ceauth/notificat
-0000bb20: 696f 6e73 2f74 656d 706c 6174 6573 2f6e  ions/templates/n
-0000bb30: 6f74 6966 6963 6174 696f 6e73 2f76 6965  otifications/vie
-0000bb40: 772e 6874 6d6c 3a39 0a6d 7367 6964 2022  w.html:9.msgid "
-0000bb50: 5669 6577 204e 6f74 6966 6963 6174 696f  View Notificatio
-0000bb60: 6e22 0a6d 7367 7374 7220 2222 0a0a 233a  n".msgstr ""..#:
-0000bb70: 2061 6c6c 6961 6e63 6561 7574 682f 6e6f   allianceauth/no
-0000bb80: 7469 6669 6361 7469 6f6e 732f 7669 6577  tifications/view
-0000bb90: 732e 7079 3a35 320a 6d73 6769 6420 2259  s.py:52.msgid "Y
-0000bba0: 6f75 2061 7265 206e 6f74 2061 7574 686f  ou are not autho
-0000bbb0: 7269 7a65 6420 746f 2076 6965 7720 7468  rized to view th
-0000bbc0: 6174 206e 6f74 6966 6963 6174 696f 6e2e  at notification.
-0000bbd0: 220a 6d73 6773 7472 2022 220a 0a23 3a20  ".msgstr ""..#: 
-0000bbe0: 616c 6c69 616e 6365 6175 7468 2f6e 6f74  allianceauth/not
-0000bbf0: 6966 6963 6174 696f 6e73 2f76 6965 7773  ifications/views
-0000bc00: 2e70 793a 3638 0a6d 7367 6964 2022 4465  .py:68.msgid "De
-0000bc10: 6c65 7465 6420 6e6f 7469 6669 6361 7469  leted notificati
-0000bc20: 6f6e 2e22 0a6d 7367 7374 7220 2222 0a0a  on.".msgstr ""..
-0000bc30: 233a 2061 6c6c 6961 6e63 6561 7574 682f  #: allianceauth/
-0000bc40: 6e6f 7469 6669 6361 7469 6f6e 732f 7669  notifications/vi
-0000bc50: 6577 732e 7079 3a37 350a 6d73 6769 6420  ews.py:75.msgid 
-0000bc60: 2246 6169 6c65 6420 746f 206c 6f63 6174  "Failed to locat
-0000bc70: 6520 6e6f 7469 6669 6361 7469 6f6e 2e22  e notification."
-0000bc80: 0a6d 7367 7374 7220 2222 0a0a 233a 2061  .msgstr ""..#: a
-0000bc90: 6c6c 6961 6e63 6561 7574 682f 6e6f 7469  llianceauth/noti
-0000bca0: 6669 6361 7469 6f6e 732f 7669 6577 732e  fications/views.
-0000bcb0: 7079 3a38 330a 6d73 6769 6420 224d 6172  py:83.msgid "Mar
-0000bcc0: 6b65 6420 616c 6c20 6e6f 7469 6669 6361  ked all notifica
-0000bcd0: 7469 6f6e 7320 6173 2072 6561 642e 220a  tions as read.".
-0000bce0: 6d73 6773 7472 2022 220a 0a23 3a20 616c  msgstr ""..#: al
-0000bcf0: 6c69 616e 6365 6175 7468 2f6e 6f74 6966  lianceauth/notif
-0000bd00: 6963 6174 696f 6e73 2f76 6965 7773 2e70  ications/views.p
-0000bd10: 793a 3931 0a6d 7367 6964 2022 4465 6c65  y:91.msgid "Dele
-0000bd20: 7465 6420 616c 6c20 7265 6164 206e 6f74  ted all read not
-0000bd30: 6966 6963 6174 696f 6e73 2e22 0a6d 7367  ifications.".msg
-0000bd40: 7374 7220 2222 0a0a 233a 2061 6c6c 6961  str ""..#: allia
-0000bd50: 6e63 6561 7574 682f 6f70 7469 6d65 722f  nceauth/optimer/
-0000bd60: 6175 7468 5f68 6f6f 6b73 2e70 793a 3132  auth_hooks.py:12
-0000bd70: 0a6d 7367 6964 2022 466c 6565 7420 4f70  .msgid "Fleet Op
-0000bd80: 6572 6174 696f 6e73 220a 6d73 6773 7472  erations".msgstr
-0000bd90: 2022 220a 0a23 3a20 616c 6c69 616e 6365   ""..#: alliance
-0000bda0: 6175 7468 2f6f 7074 696d 6572 2f66 6f72  auth/optimer/for
-0000bdb0: 6d2e 7079 3a31 320a 233a 2061 6c6c 6961  m.py:12.#: allia
-0000bdc0: 6e63 6561 7574 682f 6f70 7469 6d65 722f  nceauth/optimer/
-0000bdd0: 7465 6d70 6c61 7465 732f 6f70 7469 6d65  templates/optime
-0000bde0: 722f 666c 6565 746f 7074 6162 6c65 2e68  r/fleetoptable.h
-0000bdf0: 746d 6c3a 3131 0a6d 7367 6964 2022 446f  tml:11.msgid "Do
-0000be00: 6374 7269 6e65 220a 6d73 6773 7472 2022  ctrine".msgstr "
-0000be10: 220a 0a23 3a20 616c 6c69 616e 6365 6175  "..#: allianceau
-0000be20: 7468 2f6f 7074 696d 6572 2f66 6f72 6d2e  th/optimer/form.
-0000be30: 7079 3a31 340a 233a 2061 6c6c 6961 6e63  py:14.#: allianc
-0000be40: 6561 7574 682f 6f70 7469 6d65 722f 7465  eauth/optimer/te
-0000be50: 6d70 6c61 7465 732f 6f70 7469 6d65 722f  mplates/optimer/
-0000be60: 666c 6565 746f 7074 6162 6c65 2e68 746d  fleetoptable.htm
-0000be70: 6c3a 3133 0a6d 7367 6964 2022 5374 6172  l:13.msgid "Star
-0000be80: 7420 5469 6d65 220a 6d73 6773 7472 2022  t Time".msgstr "
-0000be90: 220a 0a23 3a20 616c 6c69 616e 6365 6175  "..#: allianceau
-0000bea0: 7468 2f6f 7074 696d 6572 2f66 6f72 6d2e  th/optimer/form.
-0000beb0: 7079 3a31 350a 233a 2061 6c6c 6961 6e63  py:15.#: allianc
-0000bec0: 6561 7574 682f 6f70 7469 6d65 722f 7465  eauth/optimer/te
-0000bed0: 6d70 6c61 7465 732f 6f70 7469 6d65 722f  mplates/optimer/
-0000bee0: 666c 6565 746f 7074 6162 6c65 2e68 746d  fleetoptable.htm
-0000bef0: 6c3a 390a 6d73 6769 6420 224f 7065 7261  l:9.msgid "Opera
-0000bf00: 7469 6f6e 204e 616d 6522 0a6d 7367 7374  tion Name".msgst
-0000bf10: 7220 2222 0a0a 233a 2061 6c6c 6961 6e63  r ""..#: allianc
-0000bf20: 6561 7574 682f 6f70 7469 6d65 722f 666f  eauth/optimer/fo
-0000bf30: 726d 2e70 793a 3136 0a6d 7367 6964 2022  rm.py:16.msgid "
-0000bf40: 4f70 6572 6174 696f 6e20 5479 7065 220a  Operation Type".
-0000bf50: 6d73 6773 7472 2022 220a 0a23 3a20 616c  msgstr ""..#: al
-0000bf60: 6c69 616e 6365 6175 7468 2f6f 7074 696d  lianceauth/optim
-0000bf70: 6572 2f66 6f72 6d2e 7079 3a31 370a 233a  er/form.py:17.#:
-0000bf80: 2061 6c6c 6961 6e63 6561 7574 682f 7372   allianceauth/sr
-0000bf90: 702f 7465 6d70 6c61 7465 732f 7372 702f  p/templates/srp/
-0000bfa0: 6d61 6e61 6765 6d65 6e74 2e68 746d 6c3a  management.html:
-0000bfb0: 3437 0a6d 7367 6964 2022 466c 6565 7420  47.msgid "Fleet 
-0000bfc0: 436f 6d6d 616e 6465 7222 0a6d 7367 7374  Commander".msgst
-0000bfd0: 7220 2222 0a0a 233a 2061 6c6c 6961 6e63  r ""..#: allianc
-0000bfe0: 6561 7574 682f 6f70 7469 6d65 722f 666f  eauth/optimer/fo
-0000bff0: 726d 2e70 793a 3232 2061 6c6c 6961 6e63  rm.py:22 allianc
-0000c000: 6561 7574 682f 7372 702f 666f 726d 2e70  eauth/srp/form.p
-0000c010: 793a 3134 0a23 3a20 616c 6c69 616e 6365  y:14.#: alliance
-0000c020: 6175 7468 2f73 7270 2f74 656d 706c 6174  auth/srp/templat
-0000c030: 6573 2f73 7270 2f64 6174 612e 6874 6d6c  es/srp/data.html
-0000c040: 3a37 310a 6d73 6769 6420 2241 6464 6974  :71.msgid "Addit
-0000c050: 696f 6e61 6c20 496e 666f 220a 6d73 6773  ional Info".msgs
-0000c060: 7472 2022 220a 0a23 3a20 616c 6c69 616e  tr ""..#: allian
-0000c070: 6365 6175 7468 2f6f 7074 696d 6572 2f66  ceauth/optimer/f
-0000c080: 6f72 6d2e 7079 3a32 330a 6d73 6769 6420  orm.py:23.msgid 
-0000c090: 2228 4f70 7469 6f6e 616c 2920 4465 7363  "(Optional) Desc
-0000c0a0: 7269 6265 2074 6865 206f 7065 7261 7469  ribe the operati
-0000c0b0: 6f6e 2077 6974 6820 6120 636f 7570 6c65  on with a couple
-0000c0c0: 206f 6620 7368 6f72 7420 776f 7264 732e   of short words.
-0000c0d0: 220a 6d73 6773 7472 2022 220a 0a23 3a20  ".msgstr ""..#: 
-0000c0e0: 616c 6c69 616e 6365 6175 7468 2f6f 7074  allianceauth/opt
-0000c0f0: 696d 6572 2f74 656d 706c 6174 6573 2f6f  imer/templates/o
-0000c100: 7074 696d 6572 2f61 6464 2e68 746d 6c3a  ptimer/add.html:
-0000c110: 380a 233a 2061 6c6c 6961 6e63 6561 7574  8.#: allianceaut
-0000c120: 682f 6f70 7469 6d65 722f 7465 6d70 6c61  h/optimer/templa
-0000c130: 7465 732f 6f70 7469 6d65 722f 6d61 6e61  tes/optimer/mana
-0000c140: 6765 6d65 6e74 2e68 746d 6c3a 3138 0a6d  gement.html:18.m
-0000c150: 7367 6964 2022 4372 6561 7465 204f 7065  sgid "Create Ope
-0000c160: 7261 7469 6f6e 220a 6d73 6773 7472 2022  ration".msgstr "
-0000c170: 220a 0a23 3a20 616c 6c69 616e 6365 6175  "..#: allianceau
-0000c180: 7468 2f6f 7074 696d 6572 2f74 656d 706c  th/optimer/templ
-0000c190: 6174 6573 2f6f 7074 696d 6572 2f61 6464  ates/optimer/add
-0000c1a0: 2e68 746d 6c3a 3132 0a23 3a20 616c 6c69  .html:12.#: alli
-0000c1b0: 616e 6365 6175 7468 2f6f 7074 696d 6572  anceauth/optimer
-0000c1c0: 2f74 656d 706c 6174 6573 2f6f 7074 696d  /templates/optim
-0000c1d0: 6572 2f6d 616e 6167 656d 656e 742e 6874  er/management.ht
-0000c1e0: 6d6c 3a31 310a 233a 2061 6c6c 6961 6e63  ml:11.#: allianc
-0000c1f0: 6561 7574 682f 6f70 7469 6d65 722f 7465  eauth/optimer/te
-0000c200: 6d70 6c61 7465 732f 6f70 7469 6d65 722f  mplates/optimer/
-0000c210: 7570 6461 7465 2e68 746d 6c3a 3132 0a6d  update.html:12.m
-0000c220: 7367 6964 2022 466c 6565 7420 4f70 6572  sgid "Fleet Oper
-0000c230: 6174 696f 6e20 5469 6d65 7273 220a 6d73  ation Timers".ms
-0000c240: 6773 7472 2022 220a 0a23 3a20 616c 6c69  gstr ""..#: alli
-0000c250: 616e 6365 6175 7468 2f6f 7074 696d 6572  anceauth/optimer
-0000c260: 2f74 656d 706c 6174 6573 2f6f 7074 696d  /templates/optim
-0000c270: 6572 2f61 6464 2e68 746d 6c3a 3231 0a6d  er/add.html:21.m
-0000c280: 7367 6964 2022 4372 6561 7465 2046 6c65  sgid "Create Fle
-0000c290: 6574 204f 7065 7261 7469 6f6e 220a 6d73  et Operation".ms
-0000c2a0: 6773 7472 2022 220a 0a23 3a20 616c 6c69  gstr ""..#: alli
-0000c2b0: 616e 6365 6175 7468 2f6f 7074 696d 6572  anceauth/optimer
-0000c2c0: 2f74 656d 706c 6174 6573 2f6f 7074 696d  /templates/optim
-0000c2d0: 6572 2f61 6464 2e68 746d 6c3a 3237 0a23  er/add.html:27.#
-0000c2e0: 3a20 616c 6c69 616e 6365 6175 7468 2f6f  : allianceauth/o
-0000c2f0: 7074 696d 6572 2f74 656d 706c 6174 6573  ptimer/templates
-0000c300: 2f6f 7074 696d 6572 2f75 7064 6174 652e  /optimer/update.
-0000c310: 6874 6d6c 3a32 370a 6d73 6769 6420 2246  html:27.msgid "F
-0000c320: 6c65 6574 206f 7065 7261 7469 6f6e 2064  leet operation d
-0000c330: 6574 6169 6c73 220a 6d73 6773 7472 2022  etails".msgstr "
-0000c340: 220a 0a23 3a20 616c 6c69 616e 6365 6175  "..#: allianceau
-0000c350: 7468 2f6f 7074 696d 6572 2f74 656d 706c  th/optimer/templ
-0000c360: 6174 6573 2f6f 7074 696d 6572 2f61 6464  ates/optimer/add
-0000c370: 2e68 746d 6c3a 3430 0a6d 7367 6964 2022  .html:40.msgid "
-0000c380: 4372 6561 7465 2066 6c65 6574 206f 7065  Create fleet ope
-0000c390: 7261 7469 6f6e 220a 6d73 6773 7472 2022  ration".msgstr "
-0000c3a0: 220a 0a23 3a20 616c 6c69 616e 6365 6175  "..#: allianceau
-0000c3b0: 7468 2f6f 7074 696d 6572 2f74 656d 706c  th/optimer/templ
-0000c3c0: 6174 6573 2f6f 7074 696d 6572 2f64 6173  ates/optimer/das
-0000c3d0: 6862 6f61 7264 2e6f 7073 2e68 746d 6c3a  hboard.ops.html:
-0000c3e0: 370a 6d73 6769 6420 2255 7063 6f6d 696e  7.msgid "Upcomin
-0000c3f0: 6720 466c 6565 7473 220a 6d73 6773 7472  g Fleets".msgstr
-0000c400: 2022 220a 0a23 3a20 616c 6c69 616e 6365   ""..#: alliance
-0000c410: 6175 7468 2f6f 7074 696d 6572 2f74 656d  auth/optimer/tem
-0000c420: 706c 6174 6573 2f6f 7074 696d 6572 2f64  plates/optimer/d
-0000c430: 6173 6862 6f61 7264 2e6f 7073 2e68 746d  ashboard.ops.htm
-0000c440: 6c3a 3134 0a6d 7367 6964 2022 4f70 6572  l:14.msgid "Oper
-0000c450: 6174 696f 6e22 0a6d 7367 7374 7220 2222  ation".msgstr ""
-0000c460: 0a0a 233a 2061 6c6c 6961 6e63 6561 7574  ..#: allianceaut
-0000c470: 682f 6f70 7469 6d65 722f 7465 6d70 6c61  h/optimer/templa
-0000c480: 7465 732f 6f70 7469 6d65 722f 6461 7368  tes/optimer/dash
-0000c490: 626f 6172 642e 6f70 732e 6874 6d6c 3a31  board.ops.html:1
-0000c4a0: 360a 233a 2061 6c6c 6961 6e63 6561 7574  6.#: allianceaut
-0000c4b0: 682f 6f70 7469 6d65 722f 7465 6d70 6c61  h/optimer/templa
-0000c4c0: 7465 732f 6f70 7469 6d65 722f 666c 6565  tes/optimer/flee
-0000c4d0: 746f 7074 6162 6c65 2e68 746d 6c3a 3132  toptable.html:12
-0000c4e0: 0a6d 7367 6964 2022 466f 726d 2055 7020  .msgid "Form Up 
-0000c4f0: 5379 7374 656d 220a 6d73 6773 7472 2022  System".msgstr "
-0000c500: 220a 0a23 3a20 616c 6c69 616e 6365 6175  "..#: allianceau
-0000c510: 7468 2f6f 7074 696d 6572 2f74 656d 706c  th/optimer/templ
-0000c520: 6174 6573 2f6f 7074 696d 6572 2f64 6173  ates/optimer/das
-0000c530: 6862 6f61 7264 2e6f 7073 2e68 746d 6c3a  hboard.ops.html:
-0000c540: 3137 0a23 3a20 616c 6c69 616e 6365 6175  17.#: allianceau
-0000c550: 7468 2f74 696d 6572 626f 6172 642f 7465  th/timerboard/te
-0000c560: 6d70 6c61 7465 732f 7469 6d65 7262 6f61  mplates/timerboa
-0000c570: 7264 2f64 6173 6862 6f61 7264 2e74 696d  rd/dashboard.tim
-0000c580: 6572 732e 6874 6d6c 3a31 370a 6d73 6769  ers.html:17.msgi
-0000c590: 6420 2245 5645 2054 696d 6522 0a6d 7367  d "EVE Time".msg
-0000c5a0: 7374 7220 2222 0a0a 233a 2061 6c6c 6961  str ""..#: allia
-0000c5b0: 6e63 6561 7574 682f 6f70 7469 6d65 722f  nceauth/optimer/
-0000c5c0: 7465 6d70 6c61 7465 732f 6f70 7469 6d65  templates/optime
-0000c5d0: 722f 666c 6565 746f 7074 6162 6c65 2e68  r/fleetoptable.h
-0000c5e0: 746d 6c3a 3134 0a23 3a20 616c 6c69 616e  tml:14.#: allian
-0000c5f0: 6365 6175 7468 2f74 696d 6572 626f 6172  ceauth/timerboar
-0000c600: 642f 7465 6d70 6c61 7465 732f 7469 6d65  d/templates/time
-0000c610: 7262 6f61 7264 2f74 696d 6572 7461 626c  rboard/timertabl
-0000c620: 652e 6874 6d6c 3a31 320a 6d73 6769 6420  e.html:12.msgid 
-0000c630: 224c 6f63 616c 2054 696d 6522 0a6d 7367  "Local Time".msg
-0000c640: 7374 7220 2222 0a0a 233a 2061 6c6c 6961  str ""..#: allia
-0000c650: 6e63 6561 7574 682f 6f70 7469 6d65 722f  nceauth/optimer/
-0000c660: 7465 6d70 6c61 7465 732f 6f70 7469 6d65  templates/optime
-0000c670: 722f 666c 6565 746f 7074 6162 6c65 2e68  r/fleetoptable.h
-0000c680: 746d 6c3a 3136 0a6d 7367 6964 2022 4643  tml:16.msgid "FC
-0000c690: 220a 6d73 6773 7472 2022 220a 0a23 3a20  ".msgstr ""..#: 
-0000c6a0: 616c 6c69 616e 6365 6175 7468 2f6f 7074  allianceauth/opt
-0000c6b0: 696d 6572 2f74 656d 706c 6174 6573 2f6f  imer/templates/o
-0000c6c0: 7074 696d 6572 2f6d 616e 6167 656d 656e  ptimer/managemen
-0000c6d0: 742e 6874 6d6c 3a37 0a6d 7367 6964 2022  t.html:7.msgid "
-0000c6e0: 466c 6565 7420 4f70 6572 6174 696f 6e20  Fleet Operation 
-0000c6f0: 4d61 6e61 6765 6d65 6e74 220a 6d73 6773  Management".msgs
-0000c700: 7472 2022 220a 0a23 3a20 616c 6c69 616e  tr ""..#: allian
-0000c710: 6365 6175 7468 2f6f 7074 696d 6572 2f74  ceauth/optimer/t
-0000c720: 656d 706c 6174 6573 2f6f 7074 696d 6572  emplates/optimer
-0000c730: 2f6d 616e 6167 656d 656e 742e 6874 6d6c  /management.html
-0000c740: 3a32 380a 233a 2061 6c6c 6961 6e63 6561  :28.#: alliancea
-0000c750: 7574 682f 7469 6d65 7262 6f61 7264 2f74  uth/timerboard/t
-0000c760: 656d 706c 6174 6573 2f74 696d 6572 626f  emplates/timerbo
-0000c770: 6172 642f 7669 6577 2e68 746d 6c3a 3331  ard/view.html:31
-0000c780: 0a6d 7367 6964 2022 4375 7272 656e 7420  .msgid "Current 
-0000c790: 4576 6520 5469 6d65 3a22 0a6d 7367 7374  Eve Time:".msgst
-0000c7a0: 7220 2222 0a0a 233a 2061 6c6c 6961 6e63  r ""..#: allianc
-0000c7b0: 6561 7574 682f 6f70 7469 6d65 722f 7465  eauth/optimer/te
-0000c7c0: 6d70 6c61 7465 732f 6f70 7469 6d65 722f  mplates/optimer/
-0000c7d0: 6d61 6e61 6765 6d65 6e74 2e68 746d 6c3a  management.html:
-0000c7e0: 3336 0a6d 7367 6964 2022 4e65 7874 2046  36.msgid "Next F
-0000c7f0: 6c65 6574 204f 7065 7261 7469 6f6e 7322  leet Operations"
-0000c800: 0a6d 7367 7374 7220 2222 0a0a 233a 2061  .msgstr ""..#: a
-0000c810: 6c6c 6961 6e63 6561 7574 682f 6f70 7469  llianceauth/opti
-0000c820: 6d65 722f 7465 6d70 6c61 7465 732f 6f70  mer/templates/op
-0000c830: 7469 6d65 722f 6d61 6e61 6765 6d65 6e74  timer/management
-0000c840: 2e68 746d 6c3a 3434 0a23 3a20 616c 6c69  .html:44.#: alli
-0000c850: 616e 6365 6175 7468 2f74 696d 6572 626f  anceauth/timerbo
-0000c860: 6172 642f 7465 6d70 6c61 7465 732f 7469  ard/templates/ti
-0000c870: 6d65 7262 6f61 7264 2f76 6965 772e 6874  merboard/view.ht
-0000c880: 6d6c 3a36 320a 6d73 6769 6420 224e 6f20  ml:62.msgid "No 
-0000c890: 7570 636f 6d69 6e67 2074 696d 6572 732e  upcoming timers.
-0000c8a0: 220a 6d73 6773 7472 2022 220a 0a23 3a20  ".msgstr ""..#: 
-0000c8b0: 616c 6c69 616e 6365 6175 7468 2f6f 7074  allianceauth/opt
-0000c8c0: 696d 6572 2f74 656d 706c 6174 6573 2f6f  imer/templates/o
-0000c8d0: 7074 696d 6572 2f6d 616e 6167 656d 656e  ptimer/managemen
-0000c8e0: 742e 6874 6d6c 3a35 320a 6d73 6769 6420  t.html:52.msgid 
-0000c8f0: 2250 6173 7420 466c 6565 7420 4f70 6572  "Past Fleet Oper
-0000c900: 6174 696f 6e73 220a 6d73 6773 7472 2022  ations".msgstr "
-0000c910: 220a 0a23 3a20 616c 6c69 616e 6365 6175  "..#: allianceau
-0000c920: 7468 2f6f 7074 696d 6572 2f74 656d 706c  th/optimer/templ
-0000c930: 6174 6573 2f6f 7074 696d 6572 2f6d 616e  ates/optimer/man
-0000c940: 6167 656d 656e 742e 6874 6d6c 3a36 300a  agement.html:60.
-0000c950: 233a 2061 6c6c 6961 6e63 6561 7574 682f  #: allianceauth/
-0000c960: 7469 6d65 7262 6f61 7264 2f74 656d 706c  timerboard/templ
-0000c970: 6174 6573 2f74 696d 6572 626f 6172 642f  ates/timerboard/
-0000c980: 7669 6577 2e68 746d 6c3a 3830 0a6d 7367  view.html:80.msg
-0000c990: 6964 2022 4e6f 2070 6173 7420 7469 6d65  id "No past time
-0000c9a0: 7273 2e22 0a6d 7367 7374 7220 2222 0a0a  rs.".msgstr ""..
-0000c9b0: 233a 2061 6c6c 6961 6e63 6561 7574 682f  #: allianceauth/
-0000c9c0: 6f70 7469 6d65 722f 7465 6d70 6c61 7465  optimer/template
-0000c9d0: 732f 6f70 7469 6d65 722f 7570 6461 7465  s/optimer/update
-0000c9e0: 2e68 746d 6c3a 380a 233a 2061 6c6c 6961  .html:8.#: allia
-0000c9f0: 6e63 6561 7574 682f 6f70 7469 6d65 722f  nceauth/optimer/
-0000ca00: 7465 6d70 6c61 7465 732f 6f70 7469 6d65  templates/optime
-0000ca10: 722f 7570 6461 7465 2e68 746d 6c3a 3231  r/update.html:21
-0000ca20: 0a6d 7367 6964 2022 5570 6461 7465 2046  .msgid "Update F
-0000ca30: 6c65 6574 204f 7065 7261 7469 6f6e 220a  leet Operation".
-0000ca40: 6d73 6773 7472 2022 220a 0a23 3a20 616c  msgstr ""..#: al
-0000ca50: 6c69 616e 6365 6175 7468 2f6f 7074 696d  lianceauth/optim
-0000ca60: 6572 2f74 656d 706c 6174 6573 2f6f 7074  er/templates/opt
-0000ca70: 696d 6572 2f75 7064 6174 652e 6874 6d6c  imer/update.html
-0000ca80: 3a34 300a 6d73 6769 6420 2255 7064 6174  :40.msgid "Updat
-0000ca90: 6520 666c 6565 7420 6f70 6572 6174 696f  e fleet operatio
-0000caa0: 6e22 0a6d 7367 7374 7220 2222 0a0a 233a  n".msgstr ""..#:
-0000cab0: 2061 6c6c 6961 6e63 6561 7574 682f 6f70   allianceauth/op
-0000cac0: 7469 6d65 722f 7669 6577 732e 7079 3a39  timer/views.py:9
-0000cad0: 310a 232c 2070 7974 686f 6e2d 666f 726d  1.#, python-form
-0000cae0: 6174 0a6d 7367 6964 2022 4372 6561 7465  at.msgid "Create
-0000caf0: 6420 6f70 6572 6174 696f 6e20 7469 6d65  d operation time
-0000cb00: 7220 666f 7220 2528 6f70 6e61 6d65 2973  r for %(opname)s
-0000cb10: 2e22 0a6d 7367 7374 7220 2222 0a0a 233a  .".msgstr ""..#:
-0000cb20: 2061 6c6c 6961 6e63 6561 7574 682f 6f70   allianceauth/op
-0000cb30: 7469 6d65 722f 7669 6577 732e 7079 3a31  timer/views.py:1
-0000cb40: 3230 0a23 2c20 7079 7468 6f6e 2d66 6f72  20.#, python-for
-0000cb50: 6d61 740a 6d73 6769 6420 2252 656d 6f76  mat.msgid "Remov
-0000cb60: 6564 206f 7065 7261 7469 6f6e 2074 696d  ed operation tim
-0000cb70: 6572 2066 6f72 2025 286f 706e 616d 6529  er for %(opname)
-0000cb80: 732e 220a 6d73 6773 7472 2022 220a 0a23  s.".msgstr ""..#
-0000cb90: 3a20 616c 6c69 616e 6365 6175 7468 2f6f  : allianceauth/o
-0000cba0: 7074 696d 6572 2f76 6965 7773 2e70 793a  ptimer/views.py:
-0000cbb0: 3137 310a 232c 2070 7974 686f 6e2d 666f  171.#, python-fo
-0000cbc0: 726d 6174 0a6d 7367 6964 2022 5361 7665  rmat.msgid "Save
-0000cbd0: 6420 6368 616e 6765 7320 746f 206f 7065  d changes to ope
-0000cbe0: 7261 7469 6f6e 2074 696d 6572 2066 6f72  ration timer for
-0000cbf0: 2025 286f 706e 616d 6529 732e 220a 6d73   %(opname)s.".ms
-0000cc00: 6773 7472 2022 220a 0a23 3a20 616c 6c69  gstr ""..#: alli
-0000cc10: 616e 6365 6175 7468 2f70 6572 6d69 7373  anceauth/permiss
-0000cc20: 696f 6e73 5f74 6f6f 6c2f 7465 6d70 6c61  ions_tool/templa
-0000cc30: 7465 732f 7065 726d 6973 7369 6f6e 735f  tes/permissions_
-0000cc40: 746f 6f6c 2f61 7564 6974 2e68 746d 6c3a  tool/audit.html:
-0000cc50: 360a 233a 2061 6c6c 6961 6e63 6561 7574  6.#: allianceaut
-0000cc60: 682f 7065 726d 6973 7369 6f6e 735f 746f  h/permissions_to
-0000cc70: 6f6c 2f74 656d 706c 6174 6573 2f70 6572  ol/templates/per
-0000cc80: 6d69 7373 696f 6e73 5f74 6f6f 6c2f 6175  missions_tool/au
-0000cc90: 6469 742e 6874 6d6c 3a31 300a 233a 2061  dit.html:10.#: a
-0000cca0: 6c6c 6961 6e63 6561 7574 682f 7065 726d  llianceauth/perm
-0000ccb0: 6973 7369 6f6e 735f 746f 6f6c 2f74 656d  issions_tool/tem
-0000ccc0: 706c 6174 6573 2f70 6572 6d69 7373 696f  plates/permissio
-0000ccd0: 6e73 5f74 6f6f 6c2f 6175 6469 742e 6874  ns_tool/audit.ht
-0000cce0: 6d6c 3a31 360a 233a 2061 6c6c 6961 6e63  ml:16.#: allianc
-0000ccf0: 6561 7574 682f 7065 726d 6973 7369 6f6e  eauth/permission
-0000cd00: 735f 746f 6f6c 2f74 656d 706c 6174 6573  s_tool/templates
-0000cd10: 2f70 6572 6d69 7373 696f 6e73 5f74 6f6f  /permissions_too
-0000cd20: 6c2f 6f76 6572 7669 6577 2e68 746d 6c3a  l/overview.html:
-0000cd30: 3130 0a6d 7367 6964 2022 5065 726d 6973  10.msgid "Permis
-0000cd40: 7369 6f6e 7320 4175 6469 7422 0a6d 7367  sions Audit".msg
-0000cd50: 7374 7220 2222 0a0a 233a 2061 6c6c 6961  str ""..#: allia
-0000cd60: 6e63 6561 7574 682f 7065 726d 6973 7369  nceauth/permissi
-0000cd70: 6f6e 735f 746f 6f6c 2f74 656d 706c 6174  ons_tool/templat
-0000cd80: 6573 2f70 6572 6d69 7373 696f 6e73 5f74  es/permissions_t
-0000cd90: 6f6f 6c2f 6175 6469 742e 6874 6d6c 3a33  ool/audit.html:3
-0000cda0: 310a 6d73 6769 6420 2255 7365 7220 2f20  1.msgid "User / 
-0000cdb0: 4368 6172 6163 7465 7222 0a6d 7367 7374  Character".msgst
-0000cdc0: 7220 2222 0a0a 233a 2061 6c6c 6961 6e63  r ""..#: allianc
-0000cdd0: 6561 7574 682f 7065 726d 6973 7369 6f6e  eauth/permission
-0000cde0: 735f 746f 6f6c 2f74 656d 706c 6174 6573  s_tool/templates
-0000cdf0: 2f70 6572 6d69 7373 696f 6e73 5f74 6f6f  /permissions_too
-0000ce00: 6c2f 6f76 6572 7669 6577 2e68 746d 6c3a  l/overview.html:
-0000ce10: 360a 6d73 6769 6420 2250 6572 6d69 7373  6.msgid "Permiss
-0000ce20: 696f 6e73 204f 7665 7276 6965 7722 0a6d  ions Overview".m
-0000ce30: 7367 7374 7220 2222 0a0a 233a 2061 6c6c  sgstr ""..#: all
-0000ce40: 6961 6e63 6561 7574 682f 7065 726d 6973  ianceauth/permis
-0000ce50: 7369 6f6e 735f 746f 6f6c 2f74 656d 706c  sions_tool/templ
-0000ce60: 6174 6573 2f70 6572 6d69 7373 696f 6e73  ates/permissions
-0000ce70: 5f74 6f6f 6c2f 6f76 6572 7669 6577 2e68  _tool/overview.h
-0000ce80: 746d 6c3a 3137 0a6d 7367 6964 2022 5368  tml:17.msgid "Sh
-0000ce90: 6f77 696e 6720 6f6e 6c79 2061 7070 6c69  owing only appli
-0000cea0: 6564 2070 6572 6d69 7373 696f 6e73 220a  ed permissions".
-0000ceb0: 6d73 6773 7472 2022 220a 0a23 3a20 616c  msgstr ""..#: al
-0000cec0: 6c69 616e 6365 6175 7468 2f70 6572 6d69  lianceauth/permi
-0000ced0: 7373 696f 6e73 5f74 6f6f 6c2f 7465 6d70  ssions_tool/temp
-0000cee0: 6c61 7465 732f 7065 726d 6973 7369 6f6e  lates/permission
-0000cef0: 735f 746f 6f6c 2f6f 7665 7276 6965 772e  s_tool/overview.
-0000cf00: 6874 6d6c 3a31 380a 6d73 6769 6420 2253  html:18.msgid "S
-0000cf10: 686f 7720 416c 6c22 0a6d 7367 7374 7220  how All".msgstr 
-0000cf20: 2222 0a0a 233a 2061 6c6c 6961 6e63 6561  ""..#: alliancea
-0000cf30: 7574 682f 7065 726d 6973 7369 6f6e 735f  uth/permissions_
-0000cf40: 746f 6f6c 2f74 656d 706c 6174 6573 2f70  tool/templates/p
-0000cf50: 6572 6d69 7373 696f 6e73 5f74 6f6f 6c2f  ermissions_tool/
-0000cf60: 6f76 6572 7669 6577 2e68 746d 6c3a 3230  overview.html:20
-0000cf70: 0a6d 7367 6964 2022 5368 6f77 696e 6720  .msgid "Showing 
-0000cf80: 616c 6c20 7065 726d 6973 7369 6f6e 7322  all permissions"
-0000cf90: 0a6d 7367 7374 7220 2222 0a0a 233a 2061  .msgstr ""..#: a
-0000cfa0: 6c6c 6961 6e63 6561 7574 682f 7065 726d  llianceauth/perm
-0000cfb0: 6973 7369 6f6e 735f 746f 6f6c 2f74 656d  issions_tool/tem
-0000cfc0: 706c 6174 6573 2f70 6572 6d69 7373 696f  plates/permissio
-0000cfd0: 6e73 5f74 6f6f 6c2f 6f76 6572 7669 6577  ns_tool/overview
-0000cfe0: 2e68 746d 6c3a 3231 0a6d 7367 6964 2022  .html:21.msgid "
-0000cff0: 5368 6f77 2041 7070 6c69 6564 220a 6d73  Show Applied".ms
-0000d000: 6773 7472 2022 220a 0a23 3a20 616c 6c69  gstr ""..#: alli
-0000d010: 616e 6365 6175 7468 2f70 6572 6d69 7373  anceauth/permiss
-0000d020: 696f 6e73 5f74 6f6f 6c2f 7465 6d70 6c61  ions_tool/templa
-0000d030: 7465 732f 7065 726d 6973 7369 6f6e 735f  tes/permissions_
-0000d040: 746f 6f6c 2f6f 7665 7276 6965 772e 6874  tool/overview.ht
-0000d050: 6d6c 3a32 390a 6d73 6769 6420 2241 7070  ml:29.msgid "App
-0000d060: 220a 6d73 6773 7472 2022 220a 0a23 3a20  ".msgstr ""..#: 
-0000d070: 616c 6c69 616e 6365 6175 7468 2f70 6572  allianceauth/per
-0000d080: 6d69 7373 696f 6e73 5f74 6f6f 6c2f 7465  missions_tool/te
-0000d090: 6d70 6c61 7465 732f 7065 726d 6973 7369  mplates/permissi
-0000d0a0: 6f6e 735f 746f 6f6c 2f6f 7665 7276 6965  ons_tool/overvie
-0000d0b0: 772e 6874 6d6c 3a33 300a 6d73 6769 6420  w.html:30.msgid 
-0000d0c0: 224d 6f64 656c 220a 6d73 6773 7472 2022  "Model".msgstr "
-0000d0d0: 220a 0a23 3a20 616c 6c69 616e 6365 6175  "..#: allianceau
-0000d0e0: 7468 2f70 6572 6d69 7373 696f 6e73 5f74  th/permissions_t
-0000d0f0: 6f6f 6c2f 7465 6d70 6c61 7465 732f 7065  ool/templates/pe
-0000d100: 726d 6973 7369 6f6e 735f 746f 6f6c 2f6f  rmissions_tool/o
-0000d110: 7665 7276 6965 772e 6874 6d6c 3a33 310a  verview.html:31.
-0000d120: 6d73 6769 6420 2243 6f64 6520 4e61 6d65  msgid "Code Name
-0000d130: 220a 6d73 6773 7472 2022 220a 0a23 3a20  ".msgstr ""..#: 
-0000d140: 616c 6c69 616e 6365 6175 7468 2f70 6572  allianceauth/per
-0000d150: 6d69 7373 696f 6e73 5f74 6f6f 6c2f 7465  missions_tool/te
-0000d160: 6d70 6c61 7465 732f 7065 726d 6973 7369  mplates/permissi
-0000d170: 6f6e 735f 746f 6f6c 2f6f 7665 7276 6965  ons_tool/overvie
-0000d180: 772e 6874 6d6c 3a33 350a 6d73 6769 6420  w.html:35.msgid 
-0000d190: 2253 7461 7465 7322 0a6d 7367 7374 7220  "States".msgstr 
-0000d1a0: 2222 0a0a 233a 2061 6c6c 6961 6e63 6561  ""..#: alliancea
-0000d1b0: 7574 682f 7365 7276 6963 6573 2f61 6273  uth/services/abs
-0000d1c0: 7472 6163 742e 7079 3a37 320a 6d73 6769  tract.py:72.msgi
-0000d1d0: 6420 2254 6861 7420 7365 7276 6963 6520  d "That service 
-0000d1e0: 6163 636f 756e 7420 616c 7265 6164 7920  account already 
-0000d1f0: 6578 6973 7473 220a 6d73 6773 7472 2022  exists".msgstr "
-0000d200: 220a 0a23 3a20 616c 6c69 616e 6365 6175  "..#: allianceau
-0000d210: 7468 2f73 6572 7669 6365 732f 6162 7374  th/services/abst
-0000d220: 7261 6374 2e70 793a 3130 330a 232c 2070  ract.py:103.#, p
-0000d230: 7974 686f 6e2d 6272 6163 652d 666f 726d  ython-brace-form
-0000d240: 6174 0a6d 7367 6964 2022 5375 6363 6573  at.msgid "Succes
-0000d250: 7366 756c 6c79 2073 6574 2079 6f75 7220  sfully set your 
-0000d260: 7b73 656c 662e 7365 7276 6963 655f 6e61  {self.service_na
-0000d270: 6d65 7d20 7061 7373 776f 7264 220a 6d73  me} password".ms
+0000b6b0: 6572 2e68 746d 6c3a 3834 0a23 3a20 616c  er.html:84.#: al
+0000b6c0: 6c69 616e 6365 6175 7468 2f74 656d 706c  lianceauth/templ
+0000b6d0: 6174 6573 2f61 6c6c 6961 6e63 6561 7574  ates/allianceaut
+0000b6e0: 682f 746f 702d 6d65 6e75 2d72 682d 6465  h/top-menu-rh-de
+0000b6f0: 6661 756c 742e 6874 6d6c 3a31 370a 233a  fault.html:17.#:
+0000b700: 2061 6c6c 6961 6e63 6561 7574 682f 7465   allianceauth/te
+0000b710: 6d70 6c61 7465 732f 616c 6c69 616e 6365  mplates/alliance
+0000b720: 6175 7468 2f74 6f70 2d6d 656e 752d 7268  auth/top-menu-rh
+0000b730: 2d64 6566 6175 6c74 2e68 746d 6c3a 3138  -default.html:18
+0000b740: 0a6d 7367 6964 2022 5369 676e 2049 6e22  .msgid "Sign In"
+0000b750: 0a6d 7367 7374 7220 2222 0a0a 233a 2061  .msgstr ""..#: a
+0000b760: 6c6c 6961 6e63 6561 7574 682f 6e6f 7469  llianceauth/noti
+0000b770: 6669 6361 7469 6f6e 732f 6d6f 6465 6c73  fications/models
+0000b780: 2e70 793a 3231 0a6d 7367 6964 2022 6461  .py:21.msgid "da
+0000b790: 6e67 6572 220a 6d73 6773 7472 2022 220a  nger".msgstr "".
+0000b7a0: 0a23 3a20 616c 6c69 616e 6365 6175 7468  .#: allianceauth
+0000b7b0: 2f6e 6f74 6966 6963 6174 696f 6e73 2f6d  /notifications/m
+0000b7c0: 6f64 656c 732e 7079 3a32 320a 6d73 6769  odels.py:22.msgi
+0000b7d0: 6420 2277 6172 6e69 6e67 220a 6d73 6773  d "warning".msgs
+0000b7e0: 7472 2022 220a 0a23 3a20 616c 6c69 616e  tr ""..#: allian
+0000b7f0: 6365 6175 7468 2f6e 6f74 6966 6963 6174  ceauth/notificat
+0000b800: 696f 6e73 2f6d 6f64 656c 732e 7079 3a32  ions/models.py:2
+0000b810: 330a 6d73 6769 6420 2269 6e66 6f22 0a6d  3.msgid "info".m
+0000b820: 7367 7374 7220 2222 0a0a 233a 2061 6c6c  sgstr ""..#: all
+0000b830: 6961 6e63 6561 7574 682f 6e6f 7469 6669  ianceauth/notifi
+0000b840: 6361 7469 6f6e 732f 6d6f 6465 6c73 2e70  cations/models.p
+0000b850: 793a 3234 0a6d 7367 6964 2022 7375 6363  y:24.msgid "succ
+0000b860: 6573 7322 0a6d 7367 7374 7220 2222 0a0a  ess".msgstr ""..
+0000b870: 233a 2061 6c6c 6961 6e63 6561 7574 682f  #: allianceauth/
+0000b880: 6e6f 7469 6669 6361 7469 6f6e 732f 7465  notifications/te
+0000b890: 6d70 6c61 7465 732f 6e6f 7469 6669 6361  mplates/notifica
+0000b8a0: 7469 6f6e 732f 6c69 7374 2e68 746d 6c3a  tions/list.html:
+0000b8b0: 3137 0a6d 7367 6964 2022 556e 7265 6164  17.msgid "Unread
+0000b8c0: 220a 6d73 6773 7472 2022 220a 0a23 3a20  ".msgstr ""..#: 
+0000b8d0: 616c 6c69 616e 6365 6175 7468 2f6e 6f74  allianceauth/not
+0000b8e0: 6966 6963 6174 696f 6e73 2f74 656d 706c  ifications/templ
+0000b8f0: 6174 6573 2f6e 6f74 6966 6963 6174 696f  ates/notificatio
+0000b900: 6e73 2f6c 6973 742e 6874 6d6c 3a32 340a  ns/list.html:24.
+0000b910: 6d73 6769 6420 2252 6561 6422 0a6d 7367  msgid "Read".msg
+0000b920: 7374 7220 2222 0a0a 233a 2061 6c6c 6961  str ""..#: allia
+0000b930: 6e63 6561 7574 682f 6e6f 7469 6669 6361  nceauth/notifica
+0000b940: 7469 6f6e 732f 7465 6d70 6c61 7465 732f  tions/templates/
+0000b950: 6e6f 7469 6669 6361 7469 6f6e 732f 6c69  notifications/li
+0000b960: 7374 2e68 746d 6c3a 3332 0a6d 7367 6964  st.html:32.msgid
+0000b970: 2022 4d61 726b 2061 6c6c 206e 6f74 6966   "Mark all notif
+0000b980: 6963 6174 696f 6e73 2061 7320 7265 6164  ications as read
+0000b990: 220a 6d73 6773 7472 2022 220a 0a23 3a20  ".msgstr ""..#: 
+0000b9a0: 616c 6c69 616e 6365 6175 7468 2f6e 6f74  allianceauth/not
+0000b9b0: 6966 6963 6174 696f 6e73 2f74 656d 706c  ifications/templ
+0000b9c0: 6174 6573 2f6e 6f74 6966 6963 6174 696f  ates/notificatio
+0000b9d0: 6e73 2f6c 6973 742e 6874 6d6c 3a33 380a  ns/list.html:38.
+0000b9e0: 6d73 6769 6420 2244 656c 6574 6520 616c  msgid "Delete al
+0000b9f0: 6c20 7265 6164 206e 6f74 6966 6963 6174  l read notificat
+0000ba00: 696f 6e73 220a 6d73 6773 7472 2022 220a  ions".msgstr "".
+0000ba10: 0a23 3a20 616c 6c69 616e 6365 6175 7468  .#: allianceauth
+0000ba20: 2f6e 6f74 6966 6963 6174 696f 6e73 2f74  /notifications/t
+0000ba30: 656d 706c 6174 6573 2f6e 6f74 6966 6963  emplates/notific
+0000ba40: 6174 696f 6e73 2f6c 6973 745f 7061 7274  ations/list_part
+0000ba50: 6961 6c2e 6874 6d6c 3a36 0a6d 7367 6964  ial.html:6.msgid
+0000ba60: 2022 5469 6d65 7374 616d 7022 0a6d 7367   "Timestamp".msg
+0000ba70: 7374 7220 2222 0a0a 233a 2061 6c6c 6961  str ""..#: allia
+0000ba80: 6e63 6561 7574 682f 6e6f 7469 6669 6361  nceauth/notifica
+0000ba90: 7469 6f6e 732f 7465 6d70 6c61 7465 732f  tions/templates/
+0000baa0: 6e6f 7469 6669 6361 7469 6f6e 732f 6c69  notifications/li
+0000bab0: 7374 5f70 6172 7469 616c 2e68 746d 6c3a  st_partial.html:
+0000bac0: 370a 6d73 6769 6420 2254 6974 6c65 220a  7.msgid "Title".
+0000bad0: 6d73 6773 7472 2022 220a 0a23 3a20 616c  msgstr ""..#: al
+0000bae0: 6c69 616e 6365 6175 7468 2f6e 6f74 6966  lianceauth/notif
+0000baf0: 6963 6174 696f 6e73 2f74 656d 706c 6174  ications/templat
+0000bb00: 6573 2f6e 6f74 6966 6963 6174 696f 6e73  es/notifications
+0000bb10: 2f6c 6973 745f 7061 7274 6961 6c2e 6874  /list_partial.ht
+0000bb20: 6d6c 3a32 380a 6d73 6769 6420 224e 6f20  ml:28.msgid "No 
+0000bb30: 6e6f 7469 6669 6361 7469 6f6e 732e 220a  notifications.".
+0000bb40: 6d73 6773 7472 2022 220a 0a23 3a20 616c  msgstr ""..#: al
+0000bb50: 6c69 616e 6365 6175 7468 2f6e 6f74 6966  lianceauth/notif
+0000bb60: 6963 6174 696f 6e73 2f74 656d 706c 6174  ications/templat
+0000bb70: 6573 2f6e 6f74 6966 6963 6174 696f 6e73  es/notifications
+0000bb80: 2f76 6965 772e 6874 6d6c 3a35 0a23 3a20  /view.html:5.#: 
+0000bb90: 616c 6c69 616e 6365 6175 7468 2f6e 6f74  allianceauth/not
+0000bba0: 6966 6963 6174 696f 6e73 2f74 656d 706c  ifications/templ
+0000bbb0: 6174 6573 2f6e 6f74 6966 6963 6174 696f  ates/notificatio
+0000bbc0: 6e73 2f76 6965 772e 6874 6d6c 3a39 0a6d  ns/view.html:9.m
+0000bbd0: 7367 6964 2022 5669 6577 204e 6f74 6966  sgid "View Notif
+0000bbe0: 6963 6174 696f 6e22 0a6d 7367 7374 7220  ication".msgstr 
+0000bbf0: 2222 0a0a 233a 2061 6c6c 6961 6e63 6561  ""..#: alliancea
+0000bc00: 7574 682f 6e6f 7469 6669 6361 7469 6f6e  uth/notification
+0000bc10: 732f 7669 6577 732e 7079 3a35 320a 6d73  s/views.py:52.ms
+0000bc20: 6769 6420 2259 6f75 2061 7265 206e 6f74  gid "You are not
+0000bc30: 2061 7574 686f 7269 7a65 6420 746f 2076   authorized to v
+0000bc40: 6965 7720 7468 6174 206e 6f74 6966 6963  iew that notific
+0000bc50: 6174 696f 6e2e 220a 6d73 6773 7472 2022  ation.".msgstr "
+0000bc60: 220a 0a23 3a20 616c 6c69 616e 6365 6175  "..#: allianceau
+0000bc70: 7468 2f6e 6f74 6966 6963 6174 696f 6e73  th/notifications
+0000bc80: 2f76 6965 7773 2e70 793a 3638 0a6d 7367  /views.py:68.msg
+0000bc90: 6964 2022 4465 6c65 7465 6420 6e6f 7469  id "Deleted noti
+0000bca0: 6669 6361 7469 6f6e 2e22 0a6d 7367 7374  fication.".msgst
+0000bcb0: 7220 2222 0a0a 233a 2061 6c6c 6961 6e63  r ""..#: allianc
+0000bcc0: 6561 7574 682f 6e6f 7469 6669 6361 7469  eauth/notificati
+0000bcd0: 6f6e 732f 7669 6577 732e 7079 3a37 350a  ons/views.py:75.
+0000bce0: 6d73 6769 6420 2246 6169 6c65 6420 746f  msgid "Failed to
+0000bcf0: 206c 6f63 6174 6520 6e6f 7469 6669 6361   locate notifica
+0000bd00: 7469 6f6e 2e22 0a6d 7367 7374 7220 2222  tion.".msgstr ""
+0000bd10: 0a0a 233a 2061 6c6c 6961 6e63 6561 7574  ..#: allianceaut
+0000bd20: 682f 6e6f 7469 6669 6361 7469 6f6e 732f  h/notifications/
+0000bd30: 7669 6577 732e 7079 3a38 330a 6d73 6769  views.py:83.msgi
+0000bd40: 6420 224d 6172 6b65 6420 616c 6c20 6e6f  d "Marked all no
+0000bd50: 7469 6669 6361 7469 6f6e 7320 6173 2072  tifications as r
+0000bd60: 6561 642e 220a 6d73 6773 7472 2022 220a  ead.".msgstr "".
+0000bd70: 0a23 3a20 616c 6c69 616e 6365 6175 7468  .#: allianceauth
+0000bd80: 2f6e 6f74 6966 6963 6174 696f 6e73 2f76  /notifications/v
+0000bd90: 6965 7773 2e70 793a 3931 0a6d 7367 6964  iews.py:91.msgid
+0000bda0: 2022 4465 6c65 7465 6420 616c 6c20 7265   "Deleted all re
+0000bdb0: 6164 206e 6f74 6966 6963 6174 696f 6e73  ad notifications
+0000bdc0: 2e22 0a6d 7367 7374 7220 2222 0a0a 233a  .".msgstr ""..#:
+0000bdd0: 2061 6c6c 6961 6e63 6561 7574 682f 6f70   allianceauth/op
+0000bde0: 7469 6d65 722f 6175 7468 5f68 6f6f 6b73  timer/auth_hooks
+0000bdf0: 2e70 793a 3132 0a6d 7367 6964 2022 466c  .py:12.msgid "Fl
+0000be00: 6565 7420 4f70 6572 6174 696f 6e73 220a  eet Operations".
+0000be10: 6d73 6773 7472 2022 220a 0a23 3a20 616c  msgstr ""..#: al
+0000be20: 6c69 616e 6365 6175 7468 2f6f 7074 696d  lianceauth/optim
+0000be30: 6572 2f66 6f72 6d2e 7079 3a31 320a 233a  er/form.py:12.#:
+0000be40: 2061 6c6c 6961 6e63 6561 7574 682f 6f70   allianceauth/op
+0000be50: 7469 6d65 722f 7465 6d70 6c61 7465 732f  timer/templates/
+0000be60: 6f70 7469 6d65 722f 666c 6565 746f 7074  optimer/fleetopt
+0000be70: 6162 6c65 2e68 746d 6c3a 3131 0a6d 7367  able.html:11.msg
+0000be80: 6964 2022 446f 6374 7269 6e65 220a 6d73  id "Doctrine".ms
+0000be90: 6773 7472 2022 220a 0a23 3a20 616c 6c69  gstr ""..#: alli
+0000bea0: 616e 6365 6175 7468 2f6f 7074 696d 6572  anceauth/optimer
+0000beb0: 2f66 6f72 6d2e 7079 3a31 340a 233a 2061  /form.py:14.#: a
+0000bec0: 6c6c 6961 6e63 6561 7574 682f 6f70 7469  llianceauth/opti
+0000bed0: 6d65 722f 7465 6d70 6c61 7465 732f 6f70  mer/templates/op
+0000bee0: 7469 6d65 722f 666c 6565 746f 7074 6162  timer/fleetoptab
+0000bef0: 6c65 2e68 746d 6c3a 3133 0a6d 7367 6964  le.html:13.msgid
+0000bf00: 2022 5374 6172 7420 5469 6d65 220a 6d73   "Start Time".ms
+0000bf10: 6773 7472 2022 220a 0a23 3a20 616c 6c69  gstr ""..#: alli
+0000bf20: 616e 6365 6175 7468 2f6f 7074 696d 6572  anceauth/optimer
+0000bf30: 2f66 6f72 6d2e 7079 3a31 350a 233a 2061  /form.py:15.#: a
+0000bf40: 6c6c 6961 6e63 6561 7574 682f 6f70 7469  llianceauth/opti
+0000bf50: 6d65 722f 7465 6d70 6c61 7465 732f 6f70  mer/templates/op
+0000bf60: 7469 6d65 722f 666c 6565 746f 7074 6162  timer/fleetoptab
+0000bf70: 6c65 2e68 746d 6c3a 390a 6d73 6769 6420  le.html:9.msgid 
+0000bf80: 224f 7065 7261 7469 6f6e 204e 616d 6522  "Operation Name"
+0000bf90: 0a6d 7367 7374 7220 2222 0a0a 233a 2061  .msgstr ""..#: a
+0000bfa0: 6c6c 6961 6e63 6561 7574 682f 6f70 7469  llianceauth/opti
+0000bfb0: 6d65 722f 666f 726d 2e70 793a 3136 0a6d  mer/form.py:16.m
+0000bfc0: 7367 6964 2022 4f70 6572 6174 696f 6e20  sgid "Operation 
+0000bfd0: 5479 7065 220a 6d73 6773 7472 2022 220a  Type".msgstr "".
+0000bfe0: 0a23 3a20 616c 6c69 616e 6365 6175 7468  .#: allianceauth
+0000bff0: 2f6f 7074 696d 6572 2f66 6f72 6d2e 7079  /optimer/form.py
+0000c000: 3a31 370a 233a 2061 6c6c 6961 6e63 6561  :17.#: alliancea
+0000c010: 7574 682f 7372 702f 7465 6d70 6c61 7465  uth/srp/template
+0000c020: 732f 7372 702f 6d61 6e61 6765 6d65 6e74  s/srp/management
+0000c030: 2e68 746d 6c3a 3437 0a6d 7367 6964 2022  .html:47.msgid "
+0000c040: 466c 6565 7420 436f 6d6d 616e 6465 7222  Fleet Commander"
+0000c050: 0a6d 7367 7374 7220 2222 0a0a 233a 2061  .msgstr ""..#: a
+0000c060: 6c6c 6961 6e63 6561 7574 682f 6f70 7469  llianceauth/opti
+0000c070: 6d65 722f 666f 726d 2e70 793a 3232 2061  mer/form.py:22 a
+0000c080: 6c6c 6961 6e63 6561 7574 682f 7372 702f  llianceauth/srp/
+0000c090: 666f 726d 2e70 793a 3134 0a23 3a20 616c  form.py:14.#: al
+0000c0a0: 6c69 616e 6365 6175 7468 2f73 7270 2f74  lianceauth/srp/t
+0000c0b0: 656d 706c 6174 6573 2f73 7270 2f64 6174  emplates/srp/dat
+0000c0c0: 612e 6874 6d6c 3a37 310a 6d73 6769 6420  a.html:71.msgid 
+0000c0d0: 2241 6464 6974 696f 6e61 6c20 496e 666f  "Additional Info
+0000c0e0: 220a 6d73 6773 7472 2022 220a 0a23 3a20  ".msgstr ""..#: 
+0000c0f0: 616c 6c69 616e 6365 6175 7468 2f6f 7074  allianceauth/opt
+0000c100: 696d 6572 2f66 6f72 6d2e 7079 3a32 330a  imer/form.py:23.
+0000c110: 6d73 6769 6420 2228 4f70 7469 6f6e 616c  msgid "(Optional
+0000c120: 2920 4465 7363 7269 6265 2074 6865 206f  ) Describe the o
+0000c130: 7065 7261 7469 6f6e 2077 6974 6820 6120  peration with a 
+0000c140: 636f 7570 6c65 206f 6620 7368 6f72 7420  couple of short 
+0000c150: 776f 7264 732e 220a 6d73 6773 7472 2022  words.".msgstr "
+0000c160: 220a 0a23 3a20 616c 6c69 616e 6365 6175  "..#: allianceau
+0000c170: 7468 2f6f 7074 696d 6572 2f74 656d 706c  th/optimer/templ
+0000c180: 6174 6573 2f6f 7074 696d 6572 2f61 6464  ates/optimer/add
+0000c190: 2e68 746d 6c3a 380a 233a 2061 6c6c 6961  .html:8.#: allia
+0000c1a0: 6e63 6561 7574 682f 6f70 7469 6d65 722f  nceauth/optimer/
+0000c1b0: 7465 6d70 6c61 7465 732f 6f70 7469 6d65  templates/optime
+0000c1c0: 722f 6d61 6e61 6765 6d65 6e74 2e68 746d  r/management.htm
+0000c1d0: 6c3a 3138 0a6d 7367 6964 2022 4372 6561  l:18.msgid "Crea
+0000c1e0: 7465 204f 7065 7261 7469 6f6e 220a 6d73  te Operation".ms
+0000c1f0: 6773 7472 2022 220a 0a23 3a20 616c 6c69  gstr ""..#: alli
+0000c200: 616e 6365 6175 7468 2f6f 7074 696d 6572  anceauth/optimer
+0000c210: 2f74 656d 706c 6174 6573 2f6f 7074 696d  /templates/optim
+0000c220: 6572 2f61 6464 2e68 746d 6c3a 3132 0a23  er/add.html:12.#
+0000c230: 3a20 616c 6c69 616e 6365 6175 7468 2f6f  : allianceauth/o
+0000c240: 7074 696d 6572 2f74 656d 706c 6174 6573  ptimer/templates
+0000c250: 2f6f 7074 696d 6572 2f6d 616e 6167 656d  /optimer/managem
+0000c260: 656e 742e 6874 6d6c 3a31 310a 233a 2061  ent.html:11.#: a
+0000c270: 6c6c 6961 6e63 6561 7574 682f 6f70 7469  llianceauth/opti
+0000c280: 6d65 722f 7465 6d70 6c61 7465 732f 6f70  mer/templates/op
+0000c290: 7469 6d65 722f 7570 6461 7465 2e68 746d  timer/update.htm
+0000c2a0: 6c3a 3132 0a6d 7367 6964 2022 466c 6565  l:12.msgid "Flee
+0000c2b0: 7420 4f70 6572 6174 696f 6e20 5469 6d65  t Operation Time
+0000c2c0: 7273 220a 6d73 6773 7472 2022 220a 0a23  rs".msgstr ""..#
+0000c2d0: 3a20 616c 6c69 616e 6365 6175 7468 2f6f  : allianceauth/o
+0000c2e0: 7074 696d 6572 2f74 656d 706c 6174 6573  ptimer/templates
+0000c2f0: 2f6f 7074 696d 6572 2f61 6464 2e68 746d  /optimer/add.htm
+0000c300: 6c3a 3231 0a6d 7367 6964 2022 4372 6561  l:21.msgid "Crea
+0000c310: 7465 2046 6c65 6574 204f 7065 7261 7469  te Fleet Operati
+0000c320: 6f6e 220a 6d73 6773 7472 2022 220a 0a23  on".msgstr ""..#
+0000c330: 3a20 616c 6c69 616e 6365 6175 7468 2f6f  : allianceauth/o
+0000c340: 7074 696d 6572 2f74 656d 706c 6174 6573  ptimer/templates
+0000c350: 2f6f 7074 696d 6572 2f61 6464 2e68 746d  /optimer/add.htm
+0000c360: 6c3a 3237 0a23 3a20 616c 6c69 616e 6365  l:27.#: alliance
+0000c370: 6175 7468 2f6f 7074 696d 6572 2f74 656d  auth/optimer/tem
+0000c380: 706c 6174 6573 2f6f 7074 696d 6572 2f75  plates/optimer/u
+0000c390: 7064 6174 652e 6874 6d6c 3a32 370a 6d73  pdate.html:27.ms
+0000c3a0: 6769 6420 2246 6c65 6574 206f 7065 7261  gid "Fleet opera
+0000c3b0: 7469 6f6e 2064 6574 6169 6c73 220a 6d73  tion details".ms
+0000c3c0: 6773 7472 2022 220a 0a23 3a20 616c 6c69  gstr ""..#: alli
+0000c3d0: 616e 6365 6175 7468 2f6f 7074 696d 6572  anceauth/optimer
+0000c3e0: 2f74 656d 706c 6174 6573 2f6f 7074 696d  /templates/optim
+0000c3f0: 6572 2f61 6464 2e68 746d 6c3a 3430 0a6d  er/add.html:40.m
+0000c400: 7367 6964 2022 4372 6561 7465 2066 6c65  sgid "Create fle
+0000c410: 6574 206f 7065 7261 7469 6f6e 220a 6d73  et operation".ms
+0000c420: 6773 7472 2022 220a 0a23 3a20 616c 6c69  gstr ""..#: alli
+0000c430: 616e 6365 6175 7468 2f6f 7074 696d 6572  anceauth/optimer
+0000c440: 2f74 656d 706c 6174 6573 2f6f 7074 696d  /templates/optim
+0000c450: 6572 2f64 6173 6862 6f61 7264 2e6f 7073  er/dashboard.ops
+0000c460: 2e68 746d 6c3a 370a 6d73 6769 6420 2255  .html:7.msgid "U
+0000c470: 7063 6f6d 696e 6720 466c 6565 7473 220a  pcoming Fleets".
+0000c480: 6d73 6773 7472 2022 220a 0a23 3a20 616c  msgstr ""..#: al
+0000c490: 6c69 616e 6365 6175 7468 2f6f 7074 696d  lianceauth/optim
+0000c4a0: 6572 2f74 656d 706c 6174 6573 2f6f 7074  er/templates/opt
+0000c4b0: 696d 6572 2f64 6173 6862 6f61 7264 2e6f  imer/dashboard.o
+0000c4c0: 7073 2e68 746d 6c3a 3134 0a6d 7367 6964  ps.html:14.msgid
+0000c4d0: 2022 4f70 6572 6174 696f 6e22 0a6d 7367   "Operation".msg
+0000c4e0: 7374 7220 2222 0a0a 233a 2061 6c6c 6961  str ""..#: allia
+0000c4f0: 6e63 6561 7574 682f 6f70 7469 6d65 722f  nceauth/optimer/
+0000c500: 7465 6d70 6c61 7465 732f 6f70 7469 6d65  templates/optime
+0000c510: 722f 6461 7368 626f 6172 642e 6f70 732e  r/dashboard.ops.
+0000c520: 6874 6d6c 3a31 360a 233a 2061 6c6c 6961  html:16.#: allia
+0000c530: 6e63 6561 7574 682f 6f70 7469 6d65 722f  nceauth/optimer/
+0000c540: 7465 6d70 6c61 7465 732f 6f70 7469 6d65  templates/optime
+0000c550: 722f 666c 6565 746f 7074 6162 6c65 2e68  r/fleetoptable.h
+0000c560: 746d 6c3a 3132 0a6d 7367 6964 2022 466f  tml:12.msgid "Fo
+0000c570: 726d 2055 7020 5379 7374 656d 220a 6d73  rm Up System".ms
+0000c580: 6773 7472 2022 220a 0a23 3a20 616c 6c69  gstr ""..#: alli
+0000c590: 616e 6365 6175 7468 2f6f 7074 696d 6572  anceauth/optimer
+0000c5a0: 2f74 656d 706c 6174 6573 2f6f 7074 696d  /templates/optim
+0000c5b0: 6572 2f64 6173 6862 6f61 7264 2e6f 7073  er/dashboard.ops
+0000c5c0: 2e68 746d 6c3a 3137 0a23 3a20 616c 6c69  .html:17.#: alli
+0000c5d0: 616e 6365 6175 7468 2f74 696d 6572 626f  anceauth/timerbo
+0000c5e0: 6172 642f 7465 6d70 6c61 7465 732f 7469  ard/templates/ti
+0000c5f0: 6d65 7262 6f61 7264 2f64 6173 6862 6f61  merboard/dashboa
+0000c600: 7264 2e74 696d 6572 732e 6874 6d6c 3a31  rd.timers.html:1
+0000c610: 370a 6d73 6769 6420 2245 5645 2054 696d  7.msgid "EVE Tim
+0000c620: 6522 0a6d 7367 7374 7220 2222 0a0a 233a  e".msgstr ""..#:
+0000c630: 2061 6c6c 6961 6e63 6561 7574 682f 6f70   allianceauth/op
+0000c640: 7469 6d65 722f 7465 6d70 6c61 7465 732f  timer/templates/
+0000c650: 6f70 7469 6d65 722f 666c 6565 746f 7074  optimer/fleetopt
+0000c660: 6162 6c65 2e68 746d 6c3a 3134 0a23 3a20  able.html:14.#: 
+0000c670: 616c 6c69 616e 6365 6175 7468 2f74 696d  allianceauth/tim
+0000c680: 6572 626f 6172 642f 7465 6d70 6c61 7465  erboard/template
+0000c690: 732f 7469 6d65 7262 6f61 7264 2f74 696d  s/timerboard/tim
+0000c6a0: 6572 7461 626c 652e 6874 6d6c 3a31 320a  ertable.html:12.
+0000c6b0: 6d73 6769 6420 224c 6f63 616c 2054 696d  msgid "Local Tim
+0000c6c0: 6522 0a6d 7367 7374 7220 2222 0a0a 233a  e".msgstr ""..#:
+0000c6d0: 2061 6c6c 6961 6e63 6561 7574 682f 6f70   allianceauth/op
+0000c6e0: 7469 6d65 722f 7465 6d70 6c61 7465 732f  timer/templates/
+0000c6f0: 6f70 7469 6d65 722f 666c 6565 746f 7074  optimer/fleetopt
+0000c700: 6162 6c65 2e68 746d 6c3a 3136 0a6d 7367  able.html:16.msg
+0000c710: 6964 2022 4643 220a 6d73 6773 7472 2022  id "FC".msgstr "
+0000c720: 220a 0a23 3a20 616c 6c69 616e 6365 6175  "..#: allianceau
+0000c730: 7468 2f6f 7074 696d 6572 2f74 656d 706c  th/optimer/templ
+0000c740: 6174 6573 2f6f 7074 696d 6572 2f6d 616e  ates/optimer/man
+0000c750: 6167 656d 656e 742e 6874 6d6c 3a37 0a6d  agement.html:7.m
+0000c760: 7367 6964 2022 466c 6565 7420 4f70 6572  sgid "Fleet Oper
+0000c770: 6174 696f 6e20 4d61 6e61 6765 6d65 6e74  ation Management
+0000c780: 220a 6d73 6773 7472 2022 220a 0a23 3a20  ".msgstr ""..#: 
+0000c790: 616c 6c69 616e 6365 6175 7468 2f6f 7074  allianceauth/opt
+0000c7a0: 696d 6572 2f74 656d 706c 6174 6573 2f6f  imer/templates/o
+0000c7b0: 7074 696d 6572 2f6d 616e 6167 656d 656e  ptimer/managemen
+0000c7c0: 742e 6874 6d6c 3a32 380a 233a 2061 6c6c  t.html:28.#: all
+0000c7d0: 6961 6e63 6561 7574 682f 7469 6d65 7262  ianceauth/timerb
+0000c7e0: 6f61 7264 2f74 656d 706c 6174 6573 2f74  oard/templates/t
+0000c7f0: 696d 6572 626f 6172 642f 7669 6577 2e68  imerboard/view.h
+0000c800: 746d 6c3a 3331 0a6d 7367 6964 2022 4375  tml:31.msgid "Cu
+0000c810: 7272 656e 7420 4576 6520 5469 6d65 3a22  rrent Eve Time:"
+0000c820: 0a6d 7367 7374 7220 2222 0a0a 233a 2061  .msgstr ""..#: a
+0000c830: 6c6c 6961 6e63 6561 7574 682f 6f70 7469  llianceauth/opti
+0000c840: 6d65 722f 7465 6d70 6c61 7465 732f 6f70  mer/templates/op
+0000c850: 7469 6d65 722f 6d61 6e61 6765 6d65 6e74  timer/management
+0000c860: 2e68 746d 6c3a 3336 0a6d 7367 6964 2022  .html:36.msgid "
+0000c870: 4e65 7874 2046 6c65 6574 204f 7065 7261  Next Fleet Opera
+0000c880: 7469 6f6e 7322 0a6d 7367 7374 7220 2222  tions".msgstr ""
+0000c890: 0a0a 233a 2061 6c6c 6961 6e63 6561 7574  ..#: allianceaut
+0000c8a0: 682f 6f70 7469 6d65 722f 7465 6d70 6c61  h/optimer/templa
+0000c8b0: 7465 732f 6f70 7469 6d65 722f 6d61 6e61  tes/optimer/mana
+0000c8c0: 6765 6d65 6e74 2e68 746d 6c3a 3434 0a23  gement.html:44.#
+0000c8d0: 3a20 616c 6c69 616e 6365 6175 7468 2f74  : allianceauth/t
+0000c8e0: 696d 6572 626f 6172 642f 7465 6d70 6c61  imerboard/templa
+0000c8f0: 7465 732f 7469 6d65 7262 6f61 7264 2f76  tes/timerboard/v
+0000c900: 6965 772e 6874 6d6c 3a36 320a 6d73 6769  iew.html:62.msgi
+0000c910: 6420 224e 6f20 7570 636f 6d69 6e67 2074  d "No upcoming t
+0000c920: 696d 6572 732e 220a 6d73 6773 7472 2022  imers.".msgstr "
+0000c930: 220a 0a23 3a20 616c 6c69 616e 6365 6175  "..#: allianceau
+0000c940: 7468 2f6f 7074 696d 6572 2f74 656d 706c  th/optimer/templ
+0000c950: 6174 6573 2f6f 7074 696d 6572 2f6d 616e  ates/optimer/man
+0000c960: 6167 656d 656e 742e 6874 6d6c 3a35 320a  agement.html:52.
+0000c970: 6d73 6769 6420 2250 6173 7420 466c 6565  msgid "Past Flee
+0000c980: 7420 4f70 6572 6174 696f 6e73 220a 6d73  t Operations".ms
+0000c990: 6773 7472 2022 220a 0a23 3a20 616c 6c69  gstr ""..#: alli
+0000c9a0: 616e 6365 6175 7468 2f6f 7074 696d 6572  anceauth/optimer
+0000c9b0: 2f74 656d 706c 6174 6573 2f6f 7074 696d  /templates/optim
+0000c9c0: 6572 2f6d 616e 6167 656d 656e 742e 6874  er/management.ht
+0000c9d0: 6d6c 3a36 300a 233a 2061 6c6c 6961 6e63  ml:60.#: allianc
+0000c9e0: 6561 7574 682f 7469 6d65 7262 6f61 7264  eauth/timerboard
+0000c9f0: 2f74 656d 706c 6174 6573 2f74 696d 6572  /templates/timer
+0000ca00: 626f 6172 642f 7669 6577 2e68 746d 6c3a  board/view.html:
+0000ca10: 3830 0a6d 7367 6964 2022 4e6f 2070 6173  80.msgid "No pas
+0000ca20: 7420 7469 6d65 7273 2e22 0a6d 7367 7374  t timers.".msgst
+0000ca30: 7220 2222 0a0a 233a 2061 6c6c 6961 6e63  r ""..#: allianc
+0000ca40: 6561 7574 682f 6f70 7469 6d65 722f 7465  eauth/optimer/te
+0000ca50: 6d70 6c61 7465 732f 6f70 7469 6d65 722f  mplates/optimer/
+0000ca60: 7570 6461 7465 2e68 746d 6c3a 380a 233a  update.html:8.#:
+0000ca70: 2061 6c6c 6961 6e63 6561 7574 682f 6f70   allianceauth/op
+0000ca80: 7469 6d65 722f 7465 6d70 6c61 7465 732f  timer/templates/
+0000ca90: 6f70 7469 6d65 722f 7570 6461 7465 2e68  optimer/update.h
+0000caa0: 746d 6c3a 3231 0a6d 7367 6964 2022 5570  tml:21.msgid "Up
+0000cab0: 6461 7465 2046 6c65 6574 204f 7065 7261  date Fleet Opera
+0000cac0: 7469 6f6e 220a 6d73 6773 7472 2022 220a  tion".msgstr "".
+0000cad0: 0a23 3a20 616c 6c69 616e 6365 6175 7468  .#: allianceauth
+0000cae0: 2f6f 7074 696d 6572 2f74 656d 706c 6174  /optimer/templat
+0000caf0: 6573 2f6f 7074 696d 6572 2f75 7064 6174  es/optimer/updat
+0000cb00: 652e 6874 6d6c 3a34 300a 6d73 6769 6420  e.html:40.msgid 
+0000cb10: 2255 7064 6174 6520 666c 6565 7420 6f70  "Update fleet op
+0000cb20: 6572 6174 696f 6e22 0a6d 7367 7374 7220  eration".msgstr 
+0000cb30: 2222 0a0a 233a 2061 6c6c 6961 6e63 6561  ""..#: alliancea
+0000cb40: 7574 682f 6f70 7469 6d65 722f 7669 6577  uth/optimer/view
+0000cb50: 732e 7079 3a39 310a 232c 2070 7974 686f  s.py:91.#, pytho
+0000cb60: 6e2d 666f 726d 6174 0a6d 7367 6964 2022  n-format.msgid "
+0000cb70: 4372 6561 7465 6420 6f70 6572 6174 696f  Created operatio
+0000cb80: 6e20 7469 6d65 7220 666f 7220 2528 6f70  n timer for %(op
+0000cb90: 6e61 6d65 2973 2e22 0a6d 7367 7374 7220  name)s.".msgstr 
+0000cba0: 2222 0a0a 233a 2061 6c6c 6961 6e63 6561  ""..#: alliancea
+0000cbb0: 7574 682f 6f70 7469 6d65 722f 7669 6577  uth/optimer/view
+0000cbc0: 732e 7079 3a31 3230 0a23 2c20 7079 7468  s.py:120.#, pyth
+0000cbd0: 6f6e 2d66 6f72 6d61 740a 6d73 6769 6420  on-format.msgid 
+0000cbe0: 2252 656d 6f76 6564 206f 7065 7261 7469  "Removed operati
+0000cbf0: 6f6e 2074 696d 6572 2066 6f72 2025 286f  on timer for %(o
+0000cc00: 706e 616d 6529 732e 220a 6d73 6773 7472  pname)s.".msgstr
+0000cc10: 2022 220a 0a23 3a20 616c 6c69 616e 6365   ""..#: alliance
+0000cc20: 6175 7468 2f6f 7074 696d 6572 2f76 6965  auth/optimer/vie
+0000cc30: 7773 2e70 793a 3137 310a 232c 2070 7974  ws.py:171.#, pyt
+0000cc40: 686f 6e2d 666f 726d 6174 0a6d 7367 6964  hon-format.msgid
+0000cc50: 2022 5361 7665 6420 6368 616e 6765 7320   "Saved changes 
+0000cc60: 746f 206f 7065 7261 7469 6f6e 2074 696d  to operation tim
+0000cc70: 6572 2066 6f72 2025 286f 706e 616d 6529  er for %(opname)
+0000cc80: 732e 220a 6d73 6773 7472 2022 220a 0a23  s.".msgstr ""..#
+0000cc90: 3a20 616c 6c69 616e 6365 6175 7468 2f70  : allianceauth/p
+0000cca0: 6572 6d69 7373 696f 6e73 5f74 6f6f 6c2f  ermissions_tool/
+0000ccb0: 7465 6d70 6c61 7465 732f 7065 726d 6973  templates/permis
+0000ccc0: 7369 6f6e 735f 746f 6f6c 2f61 7564 6974  sions_tool/audit
+0000ccd0: 2e68 746d 6c3a 360a 233a 2061 6c6c 6961  .html:6.#: allia
+0000cce0: 6e63 6561 7574 682f 7065 726d 6973 7369  nceauth/permissi
+0000ccf0: 6f6e 735f 746f 6f6c 2f74 656d 706c 6174  ons_tool/templat
+0000cd00: 6573 2f70 6572 6d69 7373 696f 6e73 5f74  es/permissions_t
+0000cd10: 6f6f 6c2f 6175 6469 742e 6874 6d6c 3a31  ool/audit.html:1
+0000cd20: 300a 233a 2061 6c6c 6961 6e63 6561 7574  0.#: allianceaut
+0000cd30: 682f 7065 726d 6973 7369 6f6e 735f 746f  h/permissions_to
+0000cd40: 6f6c 2f74 656d 706c 6174 6573 2f70 6572  ol/templates/per
+0000cd50: 6d69 7373 696f 6e73 5f74 6f6f 6c2f 6175  missions_tool/au
+0000cd60: 6469 742e 6874 6d6c 3a31 360a 233a 2061  dit.html:16.#: a
+0000cd70: 6c6c 6961 6e63 6561 7574 682f 7065 726d  llianceauth/perm
+0000cd80: 6973 7369 6f6e 735f 746f 6f6c 2f74 656d  issions_tool/tem
+0000cd90: 706c 6174 6573 2f70 6572 6d69 7373 696f  plates/permissio
+0000cda0: 6e73 5f74 6f6f 6c2f 6f76 6572 7669 6577  ns_tool/overview
+0000cdb0: 2e68 746d 6c3a 3130 0a6d 7367 6964 2022  .html:10.msgid "
+0000cdc0: 5065 726d 6973 7369 6f6e 7320 4175 6469  Permissions Audi
+0000cdd0: 7422 0a6d 7367 7374 7220 2222 0a0a 233a  t".msgstr ""..#:
+0000cde0: 2061 6c6c 6961 6e63 6561 7574 682f 7065   allianceauth/pe
+0000cdf0: 726d 6973 7369 6f6e 735f 746f 6f6c 2f74  rmissions_tool/t
+0000ce00: 656d 706c 6174 6573 2f70 6572 6d69 7373  emplates/permiss
+0000ce10: 696f 6e73 5f74 6f6f 6c2f 6175 6469 742e  ions_tool/audit.
+0000ce20: 6874 6d6c 3a33 310a 6d73 6769 6420 2255  html:31.msgid "U
+0000ce30: 7365 7220 2f20 4368 6172 6163 7465 7222  ser / Character"
+0000ce40: 0a6d 7367 7374 7220 2222 0a0a 233a 2061  .msgstr ""..#: a
+0000ce50: 6c6c 6961 6e63 6561 7574 682f 7065 726d  llianceauth/perm
+0000ce60: 6973 7369 6f6e 735f 746f 6f6c 2f74 656d  issions_tool/tem
+0000ce70: 706c 6174 6573 2f70 6572 6d69 7373 696f  plates/permissio
+0000ce80: 6e73 5f74 6f6f 6c2f 6f76 6572 7669 6577  ns_tool/overview
+0000ce90: 2e68 746d 6c3a 360a 6d73 6769 6420 2250  .html:6.msgid "P
+0000cea0: 6572 6d69 7373 696f 6e73 204f 7665 7276  ermissions Overv
+0000ceb0: 6965 7722 0a6d 7367 7374 7220 2222 0a0a  iew".msgstr ""..
+0000cec0: 233a 2061 6c6c 6961 6e63 6561 7574 682f  #: allianceauth/
+0000ced0: 7065 726d 6973 7369 6f6e 735f 746f 6f6c  permissions_tool
+0000cee0: 2f74 656d 706c 6174 6573 2f70 6572 6d69  /templates/permi
+0000cef0: 7373 696f 6e73 5f74 6f6f 6c2f 6f76 6572  ssions_tool/over
+0000cf00: 7669 6577 2e68 746d 6c3a 3137 0a6d 7367  view.html:17.msg
+0000cf10: 6964 2022 5368 6f77 696e 6720 6f6e 6c79  id "Showing only
+0000cf20: 2061 7070 6c69 6564 2070 6572 6d69 7373   applied permiss
+0000cf30: 696f 6e73 220a 6d73 6773 7472 2022 220a  ions".msgstr "".
+0000cf40: 0a23 3a20 616c 6c69 616e 6365 6175 7468  .#: allianceauth
+0000cf50: 2f70 6572 6d69 7373 696f 6e73 5f74 6f6f  /permissions_too
+0000cf60: 6c2f 7465 6d70 6c61 7465 732f 7065 726d  l/templates/perm
+0000cf70: 6973 7369 6f6e 735f 746f 6f6c 2f6f 7665  issions_tool/ove
+0000cf80: 7276 6965 772e 6874 6d6c 3a31 380a 6d73  rview.html:18.ms
+0000cf90: 6769 6420 2253 686f 7720 416c 6c22 0a6d  gid "Show All".m
+0000cfa0: 7367 7374 7220 2222 0a0a 233a 2061 6c6c  sgstr ""..#: all
+0000cfb0: 6961 6e63 6561 7574 682f 7065 726d 6973  ianceauth/permis
+0000cfc0: 7369 6f6e 735f 746f 6f6c 2f74 656d 706c  sions_tool/templ
+0000cfd0: 6174 6573 2f70 6572 6d69 7373 696f 6e73  ates/permissions
+0000cfe0: 5f74 6f6f 6c2f 6f76 6572 7669 6577 2e68  _tool/overview.h
+0000cff0: 746d 6c3a 3230 0a6d 7367 6964 2022 5368  tml:20.msgid "Sh
+0000d000: 6f77 696e 6720 616c 6c20 7065 726d 6973  owing all permis
+0000d010: 7369 6f6e 7322 0a6d 7367 7374 7220 2222  sions".msgstr ""
+0000d020: 0a0a 233a 2061 6c6c 6961 6e63 6561 7574  ..#: allianceaut
+0000d030: 682f 7065 726d 6973 7369 6f6e 735f 746f  h/permissions_to
+0000d040: 6f6c 2f74 656d 706c 6174 6573 2f70 6572  ol/templates/per
+0000d050: 6d69 7373 696f 6e73 5f74 6f6f 6c2f 6f76  missions_tool/ov
+0000d060: 6572 7669 6577 2e68 746d 6c3a 3231 0a6d  erview.html:21.m
+0000d070: 7367 6964 2022 5368 6f77 2041 7070 6c69  sgid "Show Appli
+0000d080: 6564 220a 6d73 6773 7472 2022 220a 0a23  ed".msgstr ""..#
+0000d090: 3a20 616c 6c69 616e 6365 6175 7468 2f70  : allianceauth/p
+0000d0a0: 6572 6d69 7373 696f 6e73 5f74 6f6f 6c2f  ermissions_tool/
+0000d0b0: 7465 6d70 6c61 7465 732f 7065 726d 6973  templates/permis
+0000d0c0: 7369 6f6e 735f 746f 6f6c 2f6f 7665 7276  sions_tool/overv
+0000d0d0: 6965 772e 6874 6d6c 3a32 390a 6d73 6769  iew.html:29.msgi
+0000d0e0: 6420 2241 7070 220a 6d73 6773 7472 2022  d "App".msgstr "
+0000d0f0: 220a 0a23 3a20 616c 6c69 616e 6365 6175  "..#: allianceau
+0000d100: 7468 2f70 6572 6d69 7373 696f 6e73 5f74  th/permissions_t
+0000d110: 6f6f 6c2f 7465 6d70 6c61 7465 732f 7065  ool/templates/pe
+0000d120: 726d 6973 7369 6f6e 735f 746f 6f6c 2f6f  rmissions_tool/o
+0000d130: 7665 7276 6965 772e 6874 6d6c 3a33 300a  verview.html:30.
+0000d140: 6d73 6769 6420 224d 6f64 656c 220a 6d73  msgid "Model".ms
+0000d150: 6773 7472 2022 220a 0a23 3a20 616c 6c69  gstr ""..#: alli
+0000d160: 616e 6365 6175 7468 2f70 6572 6d69 7373  anceauth/permiss
+0000d170: 696f 6e73 5f74 6f6f 6c2f 7465 6d70 6c61  ions_tool/templa
+0000d180: 7465 732f 7065 726d 6973 7369 6f6e 735f  tes/permissions_
+0000d190: 746f 6f6c 2f6f 7665 7276 6965 772e 6874  tool/overview.ht
+0000d1a0: 6d6c 3a33 310a 6d73 6769 6420 2243 6f64  ml:31.msgid "Cod
+0000d1b0: 6520 4e61 6d65 220a 6d73 6773 7472 2022  e Name".msgstr "
+0000d1c0: 220a 0a23 3a20 616c 6c69 616e 6365 6175  "..#: allianceau
+0000d1d0: 7468 2f70 6572 6d69 7373 696f 6e73 5f74  th/permissions_t
+0000d1e0: 6f6f 6c2f 7465 6d70 6c61 7465 732f 7065  ool/templates/pe
+0000d1f0: 726d 6973 7369 6f6e 735f 746f 6f6c 2f6f  rmissions_tool/o
+0000d200: 7665 7276 6965 772e 6874 6d6c 3a33 350a  verview.html:35.
+0000d210: 6d73 6769 6420 2253 7461 7465 7322 0a6d  msgid "States".m
+0000d220: 7367 7374 7220 2222 0a0a 233a 2061 6c6c  sgstr ""..#: all
+0000d230: 6961 6e63 6561 7574 682f 7365 7276 6963  ianceauth/servic
+0000d240: 6573 2f61 6273 7472 6163 742e 7079 3a37  es/abstract.py:7
+0000d250: 320a 6d73 6769 6420 2254 6861 7420 7365  2.msgid "That se
+0000d260: 7276 6963 6520 6163 636f 756e 7420 616c  rvice account al
+0000d270: 7265 6164 7920 6578 6973 7473 220a 6d73  ready exists".ms
 0000d280: 6773 7472 2022 220a 0a23 3a20 616c 6c69  gstr ""..#: alli
 0000d290: 616e 6365 6175 7468 2f73 6572 7669 6365  anceauth/service
-0000d2a0: 732f 6175 7468 5f68 6f6f 6b73 2e70 793a  s/auth_hooks.py:
-0000d2b0: 3132 0a6d 7367 6964 2022 5365 7276 6963  12.msgid "Servic
-0000d2c0: 6573 220a 6d73 6773 7472 2022 220a 0a23  es".msgstr ""..#
-0000d2d0: 3a20 616c 6c69 616e 6365 6175 7468 2f73  : allianceauth/s
-0000d2e0: 6572 7669 6365 732f 666f 726d 732e 7079  ervices/forms.py
-0000d2f0: 3a36 0a6d 7367 6964 2022 4e61 6d65 206f  :6.msgid "Name o
-0000d300: 6620 466c 6565 743a 220a 6d73 6773 7472  f Fleet:".msgstr
-0000d310: 2022 220a 0a23 3a20 616c 6c69 616e 6365   ""..#: alliance
-0000d320: 6175 7468 2f73 6572 7669 6365 732f 666f  auth/services/fo
-0000d330: 726d 732e 7079 3a37 0a6d 7367 6964 2022  rms.py:7.msgid "
-0000d340: 466c 6565 7420 436f 6d6d 616e 6465 723a  Fleet Commander:
-0000d350: 220a 6d73 6773 7472 2022 220a 0a23 3a20  ".msgstr ""..#: 
-0000d360: 616c 6c69 616e 6365 6175 7468 2f73 6572  allianceauth/ser
-0000d370: 7669 6365 732f 666f 726d 732e 7079 3a38  vices/forms.py:8
-0000d380: 0a6d 7367 6964 2022 466c 6565 7420 436f  .msgid "Fleet Co
-0000d390: 6d6d 733a 220a 6d73 6773 7472 2022 220a  mms:".msgstr "".
-0000d3a0: 0a23 3a20 616c 6c69 616e 6365 6175 7468  .#: allianceauth
-0000d3b0: 2f73 6572 7669 6365 732f 666f 726d 732e  /services/forms.
-0000d3c0: 7079 3a39 0a6d 7367 6964 2022 466c 6565  py:9.msgid "Flee
-0000d3d0: 7420 5479 7065 3a22 0a6d 7367 7374 7220  t Type:".msgstr 
-0000d3e0: 2222 0a0a 233a 2061 6c6c 6961 6e63 6561  ""..#: alliancea
-0000d3f0: 7574 682f 7365 7276 6963 6573 2f66 6f72  uth/services/for
-0000d400: 6d73 2e70 793a 3130 0a6d 7367 6964 2022  ms.py:10.msgid "
-0000d410: 5368 6970 2050 7269 6f72 6974 6965 733a  Ship Priorities:
-0000d420: 220a 6d73 6773 7472 2022 220a 0a23 3a20  ".msgstr ""..#: 
-0000d430: 616c 6c69 616e 6365 6175 7468 2f73 6572  allianceauth/ser
-0000d440: 7669 6365 732f 666f 726d 732e 7079 3a31  vices/forms.py:1
-0000d450: 310a 6d73 6769 6420 2246 6f72 6d75 7020  1.msgid "Formup 
-0000d460: 4c6f 6361 7469 6f6e 3a22 0a6d 7367 7374  Location:".msgst
-0000d470: 7220 2222 0a0a 233a 2061 6c6c 6961 6e63  r ""..#: allianc
-0000d480: 6561 7574 682f 7365 7276 6963 6573 2f66  eauth/services/f
-0000d490: 6f72 6d73 2e70 793a 3132 0a6d 7367 6964  orms.py:12.msgid
-0000d4a0: 2022 466f 726d 7570 2054 696d 653a 220a   "Formup Time:".
-0000d4b0: 6d73 6773 7472 2022 220a 0a23 3a20 616c  msgstr ""..#: al
-0000d4c0: 6c69 616e 6365 6175 7468 2f73 6572 7669  lianceauth/servi
-0000d4d0: 6365 732f 666f 726d 732e 7079 3a31 330a  ces/forms.py:13.
-0000d4e0: 6d73 6769 6420 2245 7870 6563 7465 6420  msgid "Expected 
-0000d4f0: 4475 7261 7469 6f6e 3a22 0a6d 7367 7374  Duration:".msgst
-0000d500: 7220 2222 0a0a 233a 2061 6c6c 6961 6e63  r ""..#: allianc
-0000d510: 6561 7574 682f 7365 7276 6963 6573 2f66  eauth/services/f
-0000d520: 6f72 6d73 2e70 793a 3134 0a6d 7367 6964  orms.py:14.msgid
-0000d530: 2022 5075 7270 6f73 653a 220a 6d73 6773   "Purpose:".msgs
-0000d540: 7472 2022 220a 0a23 3a20 616c 6c69 616e  tr ""..#: allian
-0000d550: 6365 6175 7468 2f73 6572 7669 6365 732f  ceauth/services/
-0000d560: 666f 726d 732e 7079 3a31 350a 6d73 6769  forms.py:15.msgi
-0000d570: 6420 2252 6569 6d62 7572 7361 626c 653f  d "Reimbursable?
-0000d580: 2a22 0a6d 7367 7374 7220 2222 0a0a 233a  *".msgstr ""..#:
-0000d590: 2061 6c6c 6961 6e63 6561 7574 682f 7365   allianceauth/se
-0000d5a0: 7276 6963 6573 2f66 6f72 6d73 2e70 793a  rvices/forms.py:
-0000d5b0: 3135 2061 6c6c 6961 6e63 6561 7574 682f  15 allianceauth/
-0000d5c0: 7365 7276 6963 6573 2f66 6f72 6d73 2e70  services/forms.p
-0000d5d0: 793a 3136 0a6d 7367 6964 2022 5965 7322  y:16.msgid "Yes"
-0000d5e0: 0a6d 7367 7374 7220 2222 0a0a 233a 2061  .msgstr ""..#: a
-0000d5f0: 6c6c 6961 6e63 6561 7574 682f 7365 7276  llianceauth/serv
-0000d600: 6963 6573 2f66 6f72 6d73 2e70 793a 3135  ices/forms.py:15
-0000d610: 2061 6c6c 6961 6e63 6561 7574 682f 7365   allianceauth/se
-0000d620: 7276 6963 6573 2f66 6f72 6d73 2e70 793a  rvices/forms.py:
-0000d630: 3136 0a6d 7367 6964 2022 4e6f 220a 6d73  16.msgid "No".ms
-0000d640: 6773 7472 2022 220a 0a23 3a20 616c 6c69  gstr ""..#: alli
-0000d650: 616e 6365 6175 7468 2f73 6572 7669 6365  anceauth/service
-0000d660: 732f 666f 726d 732e 7079 3a31 360a 6d73  s/forms.py:16.ms
-0000d670: 6769 6420 2249 6d70 6f72 7461 6e74 3f2a  gid "Important?*
-0000d680: 220a 6d73 6773 7472 2022 220a 0a23 3a20  ".msgstr ""..#: 
-0000d690: 616c 6c69 616e 6365 6175 7468 2f73 6572  allianceauth/ser
-0000d6a0: 7669 6365 732f 666f 726d 732e 7079 3a32  vices/forms.py:2
-0000d6b0: 3120 616c 6c69 616e 6365 6175 7468 2f73  1 allianceauth/s
-0000d6c0: 6572 7669 6365 732f 666f 726d 732e 7079  ervices/forms.py
-0000d6d0: 3a33 310a 6d73 6769 6420 2250 6173 7377  :31.msgid "Passw
-0000d6e0: 6f72 6422 0a6d 7367 7374 7220 2222 0a0a  ord".msgstr ""..
-0000d6f0: 233a 2061 6c6c 6961 6e63 6561 7574 682f  #: allianceauth/
-0000d700: 7365 7276 6963 6573 2f66 6f72 6d73 2e70  services/forms.p
-0000d710: 793a 3236 2061 6c6c 6961 6e63 6561 7574  y:26 allianceaut
-0000d720: 682f 7365 7276 6963 6573 2f66 6f72 6d73  h/services/forms
-0000d730: 2e70 793a 3336 0a6d 7367 6964 2022 5061  .py:36.msgid "Pa
-0000d740: 7373 776f 7264 206d 7573 7420 6265 2061  ssword must be a
-0000d750: 7420 6c65 6173 7420 3820 6368 6172 6163  t least 8 charac
-0000d760: 7465 7273 206c 6f6e 672e 220a 6d73 6773  ters long.".msgs
-0000d770: 7472 2022 220a 0a23 3a20 616c 6c69 616e  tr ""..#: allian
-0000d780: 6365 6175 7468 2f73 6572 7669 6365 732f  ceauth/services/
-0000d790: 6d6f 6475 6c65 732f 6469 7363 6f72 642f  modules/discord/
-0000d7a0: 6d6f 6465 6c73 2e70 793a 3138 370a 6d73  models.py:187.ms
-0000d7b0: 6769 6420 2244 6973 636f 7264 2041 6363  gid "Discord Acc
-0000d7c0: 6f75 6e74 2044 6973 6162 6c65 6422 0a6d  ount Disabled".m
-0000d7d0: 7367 7374 7220 2222 0a0a 233a 2061 6c6c  sgstr ""..#: all
-0000d7e0: 6961 6e63 6561 7574 682f 7365 7276 6963  ianceauth/servic
-0000d7f0: 6573 2f6d 6f64 756c 6573 2f64 6973 636f  es/modules/disco
-0000d800: 7264 2f6d 6f64 656c 732e 7079 3a31 3839  rd/models.py:189
-0000d810: 0a6d 7367 6964 2022 220a 2259 6f75 7220  .msgid ""."Your 
-0000d820: 4469 7363 6f72 6420 6163 636f 756e 7420  Discord account 
-0000d830: 7761 7320 6469 7361 626c 6564 2061 7574  was disabled aut
-0000d840: 6f6d 6174 6963 616c 6c79 2062 7920 4175  omatically by Au
-0000d850: 7468 2e20 4966 2079 6f75 2074 6869 6e6b  th. If you think
-0000d860: 2074 6869 7320 220a 2277 6173 2061 206d   this "."was a m
-0000d870: 6973 7461 6b65 2c20 706c 6561 7365 2063  istake, please c
-0000d880: 6f6e 7461 6374 2061 6e20 6164 6d69 6e2e  ontact an admin.
-0000d890: 220a 6d73 6773 7472 2022 220a 0a23 3a20  ".msgstr ""..#: 
-0000d8a0: 616c 6c69 616e 6365 6175 7468 2f73 6572  allianceauth/ser
-0000d8b0: 7669 6365 732f 6d6f 6475 6c65 732f 6469  vices/modules/di
-0000d8c0: 7363 6f72 642f 7465 6d70 6c61 7465 732f  scord/templates/
-0000d8d0: 7365 7276 6963 6573 2f64 6973 636f 7264  services/discord
-0000d8e0: 2f64 6973 636f 7264 5f73 6572 7669 6365  /discord_service
-0000d8f0: 5f63 7472 6c2e 6874 6d6c 3a32 360a 233a  _ctrl.html:26.#:
-0000d900: 2061 6c6c 6961 6e63 6561 7574 682f 7365   allianceauth/se
-0000d910: 7276 6963 6573 2f6d 6f64 756c 6573 2f6d  rvices/modules/m
-0000d920: 756d 626c 652f 7465 6d70 6c61 7465 732f  umble/templates/
-0000d930: 7365 7276 6963 6573 2f6d 756d 626c 652f  services/mumble/
-0000d940: 6d75 6d62 6c65 5f73 6572 7669 6365 5f63  mumble_service_c
-0000d950: 7472 6c2e 6874 6d6c 3a32 300a 6d73 6769  trl.html:20.msgi
-0000d960: 6420 2241 6374 6976 6174 6522 0a6d 7367  d "Activate".msg
-0000d970: 7374 7220 2222 0a0a 233a 2061 6c6c 6961  str ""..#: allia
-0000d980: 6e63 6561 7574 682f 7365 7276 6963 6573  nceauth/services
-0000d990: 2f6d 6f64 756c 6573 2f64 6973 636f 7264  /modules/discord
-0000d9a0: 2f74 656d 706c 6174 6573 2f73 6572 7669  /templates/servi
-0000d9b0: 6365 732f 6469 7363 6f72 642f 6469 7363  ces/discord/disc
-0000d9c0: 6f72 645f 7365 7276 6963 655f 6374 726c  ord_service_ctrl
-0000d9d0: 2e68 746d 6c3a 3332 0a23 3a20 616c 6c69  .html:32.#: alli
-0000d9e0: 616e 6365 6175 7468 2f73 6572 7669 6365  anceauth/service
-0000d9f0: 732f 6d6f 6475 6c65 732f 6d75 6d62 6c65  s/modules/mumble
-0000da00: 2f74 656d 706c 6174 6573 2f73 6572 7669  /templates/servi
-0000da10: 6365 732f 6d75 6d62 6c65 2f6d 756d 626c  ces/mumble/mumbl
-0000da20: 655f 7365 7276 6963 655f 6374 726c 2e68  e_service_ctrl.h
-0000da30: 746d 6c3a 3332 0a6d 7367 6964 2022 5265  tml:32.msgid "Re
-0000da40: 7365 7420 5061 7373 776f 7264 220a 6d73  set Password".ms
-0000da50: 6773 7472 2022 220a 0a23 3a20 616c 6c69  gstr ""..#: alli
-0000da60: 616e 6365 6175 7468 2f73 6572 7669 6365  anceauth/service
-0000da70: 732f 6d6f 6475 6c65 732f 6469 7363 6f72  s/modules/discor
-0000da80: 642f 7465 6d70 6c61 7465 732f 7365 7276  d/templates/serv
-0000da90: 6963 6573 2f64 6973 636f 7264 2f64 6973  ices/discord/dis
-0000daa0: 636f 7264 5f73 6572 7669 6365 5f63 7472  cord_service_ctr
-0000dab0: 6c2e 6874 6d6c 3a33 380a 233a 2061 6c6c  l.html:38.#: all
-0000dac0: 6961 6e63 6561 7574 682f 7365 7276 6963  ianceauth/servic
-0000dad0: 6573 2f6d 6f64 756c 6573 2f6d 756d 626c  es/modules/mumbl
-0000dae0: 652f 7465 6d70 6c61 7465 732f 7365 7276  e/templates/serv
-0000daf0: 6963 6573 2f6d 756d 626c 652f 6d75 6d62  ices/mumble/mumb
-0000db00: 6c65 5f73 6572 7669 6365 5f63 7472 6c2e  le_service_ctrl.
-0000db10: 6874 6d6c 3a33 380a 6d73 6769 6420 2244  html:38.msgid "D
-0000db20: 6561 6374 6976 6174 6522 0a6d 7367 7374  eactivate".msgst
-0000db30: 7220 2222 0a0a 233a 2061 6c6c 6961 6e63  r ""..#: allianc
-0000db40: 6561 7574 682f 7365 7276 6963 6573 2f6d  eauth/services/m
-0000db50: 6f64 756c 6573 2f64 6973 636f 7264 2f74  odules/discord/t
-0000db60: 656d 706c 6174 6573 2f73 6572 7669 6365  emplates/service
-0000db70: 732f 6469 7363 6f72 642f 6469 7363 6f72  s/discord/discor
-0000db80: 645f 7365 7276 6963 655f 6374 726c 2e68  d_service_ctrl.h
-0000db90: 746d 6c3a 3435 0a6d 7367 6964 2022 4c69  tml:45.msgid "Li
-0000dba0: 6e6b 2044 6973 636f 7264 2053 6572 7665  nk Discord Serve
-0000dbb0: 7222 0a6d 7367 7374 7220 2222 0a0a 233a  r".msgstr ""..#:
-0000dbc0: 2061 6c6c 6961 6e63 6561 7574 682f 7365   allianceauth/se
-0000dbd0: 7276 6963 6573 2f6d 6f64 756c 6573 2f64  rvices/modules/d
-0000dbe0: 6973 636f 7264 2f76 6965 7773 2e70 793a  iscord/views.py:
-0000dbf0: 3330 0a6d 7367 6964 2022 4465 6163 7469  30.msgid "Deacti
-0000dc00: 7661 7465 6420 4469 7363 6f72 6420 6163  vated Discord ac
-0000dc10: 636f 756e 742e 220a 6d73 6773 7472 2022  count.".msgstr "
-0000dc20: 220a 0a23 3a20 616c 6c69 616e 6365 6175  "..#: allianceau
-0000dc30: 7468 2f73 6572 7669 6365 732f 6d6f 6475  th/services/modu
-0000dc40: 6c65 732f 6469 7363 6f72 642f 7669 6577  les/discord/view
-0000dc50: 732e 7079 3a33 360a 233a 2061 6c6c 6961  s.py:36.#: allia
-0000dc60: 6e63 6561 7574 682f 7365 7276 6963 6573  nceauth/services
-0000dc70: 2f6d 6f64 756c 6573 2f64 6973 636f 7264  /modules/discord
-0000dc80: 2f76 6965 7773 2e70 793a 3539 0a6d 7367  /views.py:59.msg
-0000dc90: 6964 2022 416e 2065 7272 6f72 206f 6363  id "An error occ
-0000dca0: 7572 7265 6420 7768 696c 6520 7072 6f63  urred while proc
-0000dcb0: 6573 7369 6e67 2079 6f75 7220 4469 7363  essing your Disc
-0000dcc0: 6f72 6420 6163 636f 756e 742e 220a 6d73  ord account.".ms
-0000dcd0: 6773 7472 2022 220a 0a23 3a20 616c 6c69  gstr ""..#: alli
-0000dce0: 616e 6365 6175 7468 2f73 6572 7669 6365  anceauth/service
-0000dcf0: 732f 6d6f 6475 6c65 732f 6469 7363 6f72  s/modules/discor
-0000dd00: 642f 7669 6577 732e 7079 3a31 3032 0a6d  d/views.py:102.m
-0000dd10: 7367 6964 2022 596f 7572 2044 6973 636f  sgid "Your Disco
-0000dd20: 7264 2061 6363 6f75 6e74 2068 6173 2062  rd account has b
-0000dd30: 6565 6e20 7375 6363 6573 7366 756c 6c79  een successfully
-0000dd40: 2061 6374 6976 6174 6564 2e22 0a6d 7367   activated.".msg
-0000dd50: 7374 7220 2222 0a0a 233a 2061 6c6c 6961  str ""..#: allia
-0000dd60: 6e63 6561 7574 682f 7365 7276 6963 6573  nceauth/services
-0000dd70: 2f6d 6f64 756c 6573 2f64 6973 636f 7264  /modules/discord
-0000dd80: 2f76 6965 7773 2e70 793a 3130 380a 6d73  /views.py:108.ms
-0000dd90: 6769 6420 2222 0a22 416e 2065 7272 6f72  gid ""."An error
-0000dda0: 206f 6363 7572 7265 6420 7768 696c 6520   occurred while 
-0000ddb0: 7472 7969 6e67 2074 6f20 6163 7469 7661  trying to activa
-0000ddc0: 7465 2079 6f75 7220 4469 7363 6f72 6420  te your Discord 
-0000ddd0: 6163 636f 756e 742e 2050 6c65 6173 6520  account. Please 
-0000dde0: 7472 7920 220a 2261 6761 696e 2e22 0a6d  try "."again.".m
-0000ddf0: 7367 7374 7220 2222 0a0a 233a 2061 6c6c  sgstr ""..#: all
-0000de00: 6961 6e63 6561 7574 682f 7365 7276 6963  ianceauth/servic
-0000de10: 6573 2f6d 6f64 756c 6573 2f64 6973 636f  es/modules/disco
-0000de20: 7572 7365 2f74 656d 706c 6174 6573 2f73  urse/templates/s
-0000de30: 6572 7669 6365 732f 6469 7363 6f75 7273  ervices/discours
-0000de40: 652f 6469 7363 6f75 7273 655f 7365 7276  e/discourse_serv
-0000de50: 6963 655f 6374 726c 2e68 746d 6c3a 350a  ice_ctrl.html:5.
-0000de60: 6d73 6769 6420 2244 6973 636f 7572 7365  msgid "Discourse
-0000de70: 220a 6d73 6773 7472 2022 220a 0a23 3a20  ".msgstr ""..#: 
-0000de80: 616c 6c69 616e 6365 6175 7468 2f73 6572  allianceauth/ser
-0000de90: 7669 6365 732f 6d6f 6475 6c65 732f 6469  vices/modules/di
-0000dea0: 7363 6f75 7273 652f 7465 6d70 6c61 7465  scourse/template
-0000deb0: 732f 7365 7276 6963 6573 2f64 6973 636f  s/services/disco
-0000dec0: 7572 7365 2f64 6973 636f 7572 7365 5f73  urse/discourse_s
-0000ded0: 6572 7669 6365 5f63 7472 6c2e 6874 6d6c  ervice_ctrl.html
-0000dee0: 3a31 380a 6d73 6769 6420 2253 534f 206c  :18.msgid "SSO l
-0000def0: 6f67 696e 2061 6374 6976 6522 0a6d 7367  ogin active".msg
-0000df00: 7374 7220 2222 0a0a 233a 2061 6c6c 6961  str ""..#: allia
-0000df10: 6e63 6561 7574 682f 7365 7276 6963 6573  nceauth/services
-0000df20: 2f6d 6f64 756c 6573 2f64 6973 636f 7572  /modules/discour
-0000df30: 7365 2f74 656d 706c 6174 6573 2f73 6572  se/templates/ser
-0000df40: 7669 6365 732f 6469 7363 6f75 7273 652f  vices/discourse/
-0000df50: 6469 7363 6f75 7273 655f 7365 7276 6963  discourse_servic
-0000df60: 655f 6374 726c 2e68 746d 6c3a 3233 0a6d  e_ctrl.html:23.m
-0000df70: 7367 6964 2022 476f 2074 6f20 666f 7275  sgid "Go to foru
-0000df80: 6d73 220a 6d73 6773 7472 2022 220a 0a23  ms".msgstr ""..#
-0000df90: 3a20 616c 6c69 616e 6365 6175 7468 2f73  : allianceauth/s
-0000dfa0: 6572 7669 6365 732f 6d6f 6475 6c65 732f  ervices/modules/
-0000dfb0: 6469 7363 6f75 7273 652f 7669 6577 732e  discourse/views.
-0000dfc0: 7079 3a32 390a 6d73 6769 6420 2259 6f75  py:29.msgid "You
-0000dfd0: 2061 7265 206e 6f74 2061 7574 686f 7269   are not authori
-0000dfe0: 7a65 6420 746f 2061 6363 6573 7320 4469  zed to access Di
-0000dff0: 7363 6f75 7273 652e 220a 6d73 6773 7472  scourse.".msgstr
-0000e000: 2022 220a 0a23 3a20 616c 6c69 616e 6365   ""..#: alliance
-0000e010: 6175 7468 2f73 6572 7669 6365 732f 6d6f  auth/services/mo
-0000e020: 6475 6c65 732f 6469 7363 6f75 7273 652f  dules/discourse/
-0000e030: 7669 6577 732e 7079 3a33 340a 6d73 6769  views.py:34.msgi
-0000e040: 6420 2259 6f75 206d 7573 7420 6861 7665  d "You must have
-0000e050: 2061 206d 6169 6e20 6368 6172 6163 7465   a main characte
-0000e060: 7220 7365 7420 746f 2061 6363 6573 7320  r set to access 
-0000e070: 4469 7363 6f75 7273 652e 220a 6d73 6773  Discourse.".msgs
-0000e080: 7472 2022 220a 0a23 3a20 616c 6c69 616e  tr ""..#: allian
-0000e090: 6365 6175 7468 2f73 6572 7669 6365 732f  ceauth/services/
-0000e0a0: 6d6f 6475 6c65 732f 6469 7363 6f75 7273  modules/discours
-0000e0b0: 652f 7669 6577 732e 7079 3a34 340a 6d73  e/views.py:44.ms
-0000e0c0: 6769 6420 2222 0a22 4e6f 2053 534f 2070  gid ""."No SSO p
-0000e0d0: 6179 6c6f 6164 206f 7220 7369 676e 6174  ayload or signat
-0000e0e0: 7572 652e 2050 6c65 6173 6520 636f 6e74  ure. Please cont
-0000e0f0: 6163 7420 7375 7070 6f72 7420 6966 2074  act support if t
-0000e100: 6869 7320 7072 6f62 6c65 6d20 7065 7273  his problem pers
-0000e110: 6973 7473 2e22 0a6d 7367 7374 7220 2222  ists.".msgstr ""
-0000e120: 0a0a 233a 2061 6c6c 6961 6e63 6561 7574  ..#: allianceaut
-0000e130: 682f 7365 7276 6963 6573 2f6d 6f64 756c  h/services/modul
-0000e140: 6573 2f64 6973 636f 7572 7365 2f76 6965  es/discourse/vie
-0000e150: 7773 2e70 793a 3534 0a23 3a20 616c 6c69  ws.py:54.#: alli
-0000e160: 616e 6365 6175 7468 2f73 6572 7669 6365  anceauth/service
-0000e170: 732f 6d6f 6475 6c65 732f 6469 7363 6f75  s/modules/discou
-0000e180: 7273 652f 7669 6577 732e 7079 3a36 320a  rse/views.py:62.
-0000e190: 6d73 6769 6420 2249 6e76 616c 6964 2070  msgid "Invalid p
-0000e1a0: 6179 6c6f 6164 2e20 506c 6561 7365 2063  ayload. Please c
-0000e1b0: 6f6e 7461 6374 2073 7570 706f 7274 2069  ontact support i
-0000e1c0: 6620 7468 6973 2070 726f 626c 656d 2070  f this problem p
-0000e1d0: 6572 7369 7374 732e 220a 6d73 6773 7472  ersists.".msgstr
-0000e1e0: 2022 220a 0a23 3a20 616c 6c69 616e 6365   ""..#: alliance
-0000e1f0: 6175 7468 2f73 6572 7669 6365 732f 6d6f  auth/services/mo
-0000e200: 6475 6c65 732f 6970 7334 2f76 6965 7773  dules/ips4/views
-0000e210: 2e70 793a 3331 0a6d 7367 6964 2022 4163  .py:31.msgid "Ac
-0000e220: 7469 7661 7465 6420 4950 5375 6974 6534  tivated IPSuite4
-0000e230: 2061 6363 6f75 6e74 2e22 0a6d 7367 7374   account.".msgst
-0000e240: 7220 2222 0a0a 233a 2061 6c6c 6961 6e63  r ""..#: allianc
-0000e250: 6561 7574 682f 7365 7276 6963 6573 2f6d  eauth/services/m
-0000e260: 6f64 756c 6573 2f69 7073 342f 7669 6577  odules/ips4/view
-0000e270: 732e 7079 3a33 390a 233a 2061 6c6c 6961  s.py:39.#: allia
-0000e280: 6e63 6561 7574 682f 7365 7276 6963 6573  nceauth/services
-0000e290: 2f6d 6f64 756c 6573 2f69 7073 342f 7669  /modules/ips4/vi
-0000e2a0: 6577 732e 7079 3a36 300a 233a 2061 6c6c  ews.py:60.#: all
-0000e2b0: 6961 6e63 6561 7574 682f 7365 7276 6963  ianceauth/servic
-0000e2c0: 6573 2f6d 6f64 756c 6573 2f69 7073 342f  es/modules/ips4/
-0000e2d0: 7669 6577 732e 7079 3a38 310a 233a 2061  views.py:81.#: a
-0000e2e0: 6c6c 6961 6e63 6561 7574 682f 7365 7276  llianceauth/serv
-0000e2f0: 6963 6573 2f6d 6f64 756c 6573 2f69 7073  ices/modules/ips
-0000e300: 342f 7669 6577 732e 7079 3a31 3031 0a6d  4/views.py:101.m
-0000e310: 7367 6964 2022 416e 2065 7272 6f72 206f  sgid "An error o
-0000e320: 6363 7572 7265 6420 7768 696c 6520 7072  ccurred while pr
-0000e330: 6f63 6573 7369 6e67 2079 6f75 7220 4950  ocessing your IP
-0000e340: 5375 6974 6534 2061 6363 6f75 6e74 2e22  Suite4 account."
-0000e350: 0a6d 7367 7374 7220 2222 0a0a 233a 2061  .msgstr ""..#: a
-0000e360: 6c6c 6961 6e63 6561 7574 682f 7365 7276  llianceauth/serv
-0000e370: 6963 6573 2f6d 6f64 756c 6573 2f69 7073  ices/modules/ips
-0000e380: 342f 7669 6577 732e 7079 3a35 320a 6d73  4/views.py:52.ms
-0000e390: 6769 6420 2252 6573 6574 2049 5053 7569  gid "Reset IPSui
-0000e3a0: 7465 3420 7061 7373 776f 7264 2e22 0a6d  te4 password.".m
-0000e3b0: 7367 7374 7220 2222 0a0a 233a 2061 6c6c  sgstr ""..#: all
-0000e3c0: 6961 6e63 6561 7574 682f 7365 7276 6963  ianceauth/servic
-0000e3d0: 6573 2f6d 6f64 756c 6573 2f69 7073 342f  es/modules/ips4/
-0000e3e0: 7669 6577 732e 7079 3a37 380a 6d73 6769  views.py:78.msgi
-0000e3f0: 6420 2253 6574 2049 5053 7569 7465 3420  d "Set IPSuite4 
-0000e400: 7061 7373 776f 7264 2e22 0a6d 7367 7374  password.".msgst
-0000e410: 7220 2222 0a0a 233a 2061 6c6c 6961 6e63  r ""..#: allianc
-0000e420: 6561 7574 682f 7365 7276 6963 6573 2f6d  eauth/services/m
-0000e430: 6f64 756c 6573 2f69 7073 342f 7669 6577  odules/ips4/view
-0000e440: 732e 7079 3a39 380a 6d73 6769 6420 2244  s.py:98.msgid "D
-0000e450: 6561 6374 6976 6174 6564 2049 5053 7569  eactivated IPSui
-0000e460: 7465 3420 6163 636f 756e 742e 220a 6d73  te4 account.".ms
-0000e470: 6773 7472 2022 220a 0a23 3a20 616c 6c69  gstr ""..#: alli
-0000e480: 616e 6365 6175 7468 2f73 6572 7669 6365  anceauth/service
-0000e490: 732f 6d6f 6475 6c65 732f 6d75 6d62 6c65  s/modules/mumble
-0000e4a0: 2f74 656d 706c 6174 6573 2f73 6572 7669  /templates/servi
-0000e4b0: 6365 732f 6d75 6d62 6c65 2f6d 756d 626c  ces/mumble/mumbl
-0000e4c0: 655f 7365 7276 6963 655f 6374 726c 2e68  e_service_ctrl.h
-0000e4d0: 746d 6c3a 3236 0a23 3a20 616c 6c69 616e  tml:26.#: allian
-0000e4e0: 6365 6175 7468 2f73 6572 7669 6365 732f  ceauth/services/
-0000e4f0: 7465 6d70 6c61 7465 732f 7365 7276 6963  templates/servic
-0000e500: 6573 2f73 6572 7669 6365 5f70 6173 7377  es/service_passw
-0000e510: 6f72 642e 6874 6d6c 3a32 360a 6d73 6769  ord.html:26.msgi
-0000e520: 6420 2253 6574 2050 6173 7377 6f72 6422  d "Set Password"
-0000e530: 0a6d 7367 7374 7220 2222 0a0a 233a 2061  .msgstr ""..#: a
-0000e540: 6c6c 6961 6e63 6561 7574 682f 7365 7276  llianceauth/serv
-0000e550: 6963 6573 2f6d 6f64 756c 6573 2f6d 756d  ices/modules/mum
-0000e560: 626c 652f 7465 6d70 6c61 7465 732f 7365  ble/templates/se
-0000e570: 7276 6963 6573 2f6d 756d 626c 652f 6d75  rvices/mumble/mu
-0000e580: 6d62 6c65 5f73 6572 7669 6365 5f63 7472  mble_service_ctr
-0000e590: 6c2e 6874 6d6c 3a34 340a 6d73 6769 6420  l.html:44.msgid 
-0000e5a0: 2243 6f6e 6e65 6374 220a 6d73 6773 7472  "Connect".msgstr
-0000e5b0: 2022 220a 0a23 3a20 616c 6c69 616e 6365   ""..#: alliance
-0000e5c0: 6175 7468 2f73 6572 7669 6365 732f 6d6f  auth/services/mo
-0000e5d0: 6475 6c65 732f 6f70 656e 6669 7265 2f61  dules/openfire/a
-0000e5e0: 7574 685f 686f 6f6b 732e 7079 3a32 370a  uth_hooks.py:27.
-0000e5f0: 6d73 6769 6420 224a 6162 6265 7222 0a6d  msgid "Jabber".m
-0000e600: 7367 7374 7220 2222 0a0a 233a 2061 6c6c  sgstr ""..#: all
-0000e610: 6961 6e63 6561 7574 682f 7365 7276 6963  ianceauth/servic
-0000e620: 6573 2f6d 6f64 756c 6573 2f6f 7065 6e66  es/modules/openf
-0000e630: 6972 652f 6175 7468 5f68 6f6f 6b73 2e70  ire/auth_hooks.p
-0000e640: 793a 3830 0a23 3a20 616c 6c69 616e 6365  y:80.#: alliance
-0000e650: 6175 7468 2f73 6572 7669 6365 732f 6d6f  auth/services/mo
-0000e660: 6475 6c65 732f 6f70 656e 6669 7265 2f74  dules/openfire/t
-0000e670: 656d 706c 6174 6573 2f73 6572 7669 6365  emplates/service
-0000e680: 732f 6f70 656e 6669 7265 2f62 726f 6164  s/openfire/broad
-0000e690: 6361 7374 2e68 746d 6c3a 370a 233a 2061  cast.html:7.#: a
-0000e6a0: 6c6c 6961 6e63 6561 7574 682f 7365 7276  llianceauth/serv
-0000e6b0: 6963 6573 2f6d 6f64 756c 6573 2f6f 7065  ices/modules/ope
-0000e6c0: 6e66 6972 652f 7465 6d70 6c61 7465 732f  nfire/templates/
-0000e6d0: 7365 7276 6963 6573 2f6f 7065 6e66 6972  services/openfir
-0000e6e0: 652f 6272 6f61 6463 6173 742e 6874 6d6c  e/broadcast.html
-0000e6f0: 3a31 310a 233a 2061 6c6c 6961 6e63 6561  :11.#: alliancea
-0000e700: 7574 682f 7365 7276 6963 6573 2f6d 6f64  uth/services/mod
-0000e710: 756c 6573 2f6f 7065 6e66 6972 652f 7465  ules/openfire/te
-0000e720: 6d70 6c61 7465 732f 7365 7276 6963 6573  mplates/services
-0000e730: 2f6f 7065 6e66 6972 652f 6272 6f61 6463  /openfire/broadc
-0000e740: 6173 742e 6874 6d6c 3a31 390a 6d73 6769  ast.html:19.msgi
-0000e750: 6420 224a 6162 6265 7220 4272 6f61 6463  d "Jabber Broadc
-0000e760: 6173 7422 0a6d 7367 7374 7220 2222 0a0a  ast".msgstr ""..
-0000e770: 233a 2061 6c6c 6961 6e63 6561 7574 682f  #: allianceauth/
-0000e780: 7365 7276 6963 6573 2f6d 6f64 756c 6573  services/modules
-0000e790: 2f6f 7065 6e66 6972 652f 6175 7468 5f68  /openfire/auth_h
-0000e7a0: 6f6f 6b73 2e70 793a 3935 0a6d 7367 6964  ooks.py:95.msgid
-0000e7b0: 2022 466c 6565 7420 4272 6f61 6463 6173   "Fleet Broadcas
-0000e7c0: 7420 466f 726d 6174 7465 7222 0a6d 7367  t Formatter".msg
-0000e7d0: 7374 7220 2222 0a0a 233a 2061 6c6c 6961  str ""..#: allia
-0000e7e0: 6e63 6561 7574 682f 7365 7276 6963 6573  nceauth/services
-0000e7f0: 2f6d 6f64 756c 6573 2f6f 7065 6e66 6972  /modules/openfir
-0000e800: 652f 666f 726d 732e 7079 3a37 0a6d 7367  e/forms.py:7.msg
-0000e810: 6964 2022 4d65 7373 6167 6522 0a6d 7367  id "Message".msg
-0000e820: 7374 7220 2222 0a0a 233a 2061 6c6c 6961  str ""..#: allia
-0000e830: 6e63 6561 7574 682f 7365 7276 6963 6573  nceauth/services
-0000e840: 2f6d 6f64 756c 6573 2f6f 7065 6e66 6972  /modules/openfir
-0000e850: 652f 7465 6d70 6c61 7465 732f 7365 7276  e/templates/serv
-0000e860: 6963 6573 2f6f 7065 6e66 6972 652f 6272  ices/openfire/br
-0000e870: 6f61 6463 6173 742e 6874 6d6c 3a32 380a  oadcast.html:28.
-0000e880: 6d73 6769 6420 2242 726f 6164 6361 7374  msgid "Broadcast
-0000e890: 2053 656e 7421 2122 0a6d 7367 7374 7220   Sent!!".msgstr 
-0000e8a0: 2222 0a0a 233a 2061 6c6c 6961 6e63 6561  ""..#: alliancea
-0000e8b0: 7574 682f 7365 7276 6963 6573 2f6d 6f64  uth/services/mod
-0000e8c0: 756c 6573 2f6f 7065 6e66 6972 652f 7465  ules/openfire/te
-0000e8d0: 6d70 6c61 7465 732f 7365 7276 6963 6573  mplates/services
-0000e8e0: 2f6f 7065 6e66 6972 652f 6272 6f61 6463  /openfire/broadc
-0000e8f0: 6173 742e 6874 6d6c 3a33 380a 6d73 6769  ast.html:38.msgi
-0000e900: 6420 2242 726f 6164 6361 7374 220a 6d73  d "Broadcast".ms
-0000e910: 6773 7472 2022 220a 0a23 3a20 616c 6c69  gstr ""..#: alli
-0000e920: 616e 6365 6175 7468 2f73 6572 7669 6365  anceauth/service
-0000e930: 732f 6d6f 6475 6c65 732f 6f70 656e 6669  s/modules/openfi
-0000e940: 7265 2f76 6965 7773 2e70 793a 3335 0a6d  re/views.py:35.m
-0000e950: 7367 6964 2022 4163 7469 7661 7465 6420  sgid "Activated 
-0000e960: 4a61 6262 6572 2061 6363 6f75 6e74 2e22  Jabber account."
-0000e970: 0a6d 7367 7374 7220 2222 0a0a 233a 2061  .msgstr ""..#: a
-0000e980: 6c6c 6961 6e63 6561 7574 682f 7365 7276  llianceauth/serv
-0000e990: 6963 6573 2f6d 6f64 756c 6573 2f6f 7065  ices/modules/ope
-0000e9a0: 6e66 6972 652f 7669 6577 732e 7079 3a34  nfire/views.py:4
-0000e9b0: 330a 233a 2061 6c6c 6961 6e63 6561 7574  3.#: allianceaut
-0000e9c0: 682f 7365 7276 6963 6573 2f6d 6f64 756c  h/services/modul
-0000e9d0: 6573 2f6f 7065 6e66 6972 652f 7669 6577  es/openfire/view
-0000e9e0: 732e 7079 3a35 360a 233a 2061 6c6c 6961  s.py:56.#: allia
-0000e9f0: 6e63 6561 7574 682f 7365 7276 6963 6573  nceauth/services
-0000ea00: 2f6d 6f64 756c 6573 2f6f 7065 6e66 6972  /modules/openfir
-0000ea10: 652f 7669 6577 732e 7079 3a37 360a 233a  e/views.py:76.#:
-0000ea20: 2061 6c6c 6961 6e63 6561 7574 682f 7365   allianceauth/se
-0000ea30: 7276 6963 6573 2f6d 6f64 756c 6573 2f6f  rvices/modules/o
-0000ea40: 7065 6e66 6972 652f 7669 6577 732e 7079  penfire/views.py
-0000ea50: 3a31 3437 0a6d 7367 6964 2022 416e 2065  :147.msgid "An e
-0000ea60: 7272 6f72 206f 6363 7572 7265 6420 7768  rror occurred wh
-0000ea70: 696c 6520 7072 6f63 6573 7369 6e67 2079  ile processing y
-0000ea80: 6f75 7220 4a61 6262 6572 2061 6363 6f75  our Jabber accou
-0000ea90: 6e74 2e22 0a6d 7367 7374 7220 2222 0a0a  nt.".msgstr ""..
-0000eaa0: 233a 2061 6c6c 6961 6e63 6561 7574 682f  #: allianceauth/
-0000eab0: 7365 7276 6963 6573 2f6d 6f64 756c 6573  services/modules
-0000eac0: 2f6f 7065 6e66 6972 652f 7669 6577 732e  /openfire/views.
-0000ead0: 7079 3a36 390a 6d73 6769 6420 2252 6573  py:69.msgid "Res
-0000eae0: 6574 204a 6162 6265 7220 7061 7373 776f  et Jabber passwo
-0000eaf0: 7264 2e22 0a6d 7367 7374 7220 2222 0a0a  rd.".msgstr ""..
-0000eb00: 233a 2061 6c6c 6961 6e63 6561 7574 682f  #: allianceauth/
-0000eb10: 7365 7276 6963 6573 2f6d 6f64 756c 6573  services/modules
-0000eb20: 2f6f 7065 6e66 6972 652f 7669 6577 732e  /openfire/views.
-0000eb30: 7079 3a31 3135 0a23 2c20 7079 7468 6f6e  py:115.#, python
-0000eb40: 2d66 6f72 6d61 740a 6d73 6769 6420 2253  -format.msgid "S
-0000eb50: 656e 7420 4a61 6262 6572 2062 726f 6164  ent Jabber broad
-0000eb60: 6361 7374 2074 6f20 2573 220a 6d73 6773  cast to %s".msgs
-0000eb70: 7472 2022 220a 0a23 3a20 616c 6c69 616e  tr ""..#: allian
-0000eb80: 6365 6175 7468 2f73 6572 7669 6365 732f  ceauth/services/
-0000eb90: 6d6f 6475 6c65 732f 6f70 656e 6669 7265  modules/openfire
-0000eba0: 2f76 6965 7773 2e70 793a 3134 340a 6d73  /views.py:144.ms
-0000ebb0: 6769 6420 2253 6574 206a 6162 6265 7220  gid "Set jabber 
-0000ebc0: 7061 7373 776f 7264 2e22 0a6d 7367 7374  password.".msgst
-0000ebd0: 7220 2222 0a0a 233a 2061 6c6c 6961 6e63  r ""..#: allianc
-0000ebe0: 6561 7574 682f 7365 7276 6963 6573 2f6d  eauth/services/m
-0000ebf0: 6f64 756c 6573 2f70 6870 6262 332f 7669  odules/phpbb3/vi
-0000ec00: 6577 732e 7079 3a33 340a 6d73 6769 6420  ews.py:34.msgid 
-0000ec10: 2241 6374 6976 6174 6564 2066 6f72 756d  "Activated forum
-0000ec20: 2061 6363 6f75 6e74 2e22 0a6d 7367 7374   account.".msgst
-0000ec30: 7220 2222 0a0a 233a 2061 6c6c 6961 6e63  r ""..#: allianc
-0000ec40: 6561 7574 682f 7365 7276 6963 6573 2f6d  eauth/services/m
-0000ec50: 6f64 756c 6573 2f70 6870 6262 332f 7669  odules/phpbb3/vi
-0000ec60: 6577 732e 7079 3a34 320a 233a 2061 6c6c  ews.py:42.#: all
-0000ec70: 6961 6e63 6561 7574 682f 7365 7276 6963  ianceauth/servic
-0000ec80: 6573 2f6d 6f64 756c 6573 2f70 6870 6262  es/modules/phpbb
-0000ec90: 332f 7669 6577 732e 7079 3a35 360a 233a  3/views.py:56.#:
-0000eca0: 2061 6c6c 6961 6e63 6561 7574 682f 7365   allianceauth/se
-0000ecb0: 7276 6963 6573 2f6d 6f64 756c 6573 2f70  rvices/modules/p
-0000ecc0: 6870 6262 332f 7669 6577 732e 7079 3a37  hpbb3/views.py:7
-0000ecd0: 380a 233a 2061 6c6c 6961 6e63 6561 7574  8.#: allianceaut
-0000ece0: 682f 7365 7276 6963 6573 2f6d 6f64 756c  h/services/modul
-0000ecf0: 6573 2f70 6870 6262 332f 7669 6577 732e  es/phpbb3/views.
-0000ed00: 7079 3a31 3031 0a6d 7367 6964 2022 416e  py:101.msgid "An
-0000ed10: 2065 7272 6f72 206f 6363 7572 7265 6420   error occurred 
-0000ed20: 7768 696c 6520 7072 6f63 6573 7369 6e67  while processing
-0000ed30: 2079 6f75 7220 666f 7275 6d20 6163 636f   your forum acco
-0000ed40: 756e 742e 220a 6d73 6773 7472 2022 220a  unt.".msgstr "".
-0000ed50: 0a23 3a20 616c 6c69 616e 6365 6175 7468  .#: allianceauth
-0000ed60: 2f73 6572 7669 6365 732f 6d6f 6475 6c65  /services/module
-0000ed70: 732f 7068 7062 6233 2f76 6965 7773 2e70  s/phpbb3/views.p
-0000ed80: 793a 3533 0a6d 7367 6964 2022 4465 6163  y:53.msgid "Deac
-0000ed90: 7469 7661 7465 6420 666f 7275 6d20 6163  tivated forum ac
-0000eda0: 636f 756e 742e 220a 6d73 6773 7472 2022  count.".msgstr "
-0000edb0: 220a 0a23 3a20 616c 6c69 616e 6365 6175  "..#: allianceau
-0000edc0: 7468 2f73 6572 7669 6365 732f 6d6f 6475  th/services/modu
-0000edd0: 6c65 732f 7068 7062 6233 2f76 6965 7773  les/phpbb3/views
-0000ede0: 2e70 793a 3730 0a6d 7367 6964 2022 5265  .py:70.msgid "Re
-0000edf0: 7365 7420 666f 7275 6d20 7061 7373 776f  set forum passwo
-0000ee00: 7264 2e22 0a6d 7367 7374 7220 2222 0a0a  rd.".msgstr ""..
-0000ee10: 233a 2061 6c6c 6961 6e63 6561 7574 682f  #: allianceauth/
-0000ee20: 7365 7276 6963 6573 2f6d 6f64 756c 6573  services/modules
-0000ee30: 2f70 6870 6262 332f 7669 6577 732e 7079  /phpbb3/views.py
-0000ee40: 3a39 380a 6d73 6769 6420 2253 6574 2066  :98.msgid "Set f
-0000ee50: 6f72 756d 2070 6173 7377 6f72 642e 220a  orum password.".
-0000ee60: 6d73 6773 7472 2022 220a 0a23 3a20 616c  msgstr ""..#: al
-0000ee70: 6c69 616e 6365 6175 7468 2f73 6572 7669  lianceauth/servi
-0000ee80: 6365 732f 6d6f 6475 6c65 732f 736d 662f  ces/modules/smf/
-0000ee90: 7669 6577 732e 7079 3a35 320a 6d73 6769  views.py:52.msgi
-0000eea0: 6420 2241 6374 6976 6174 6564 2053 4d46  d "Activated SMF
-0000eeb0: 2061 6363 6f75 6e74 2e22 0a6d 7367 7374   account.".msgst
-0000eec0: 7220 2222 0a0a 233a 2061 6c6c 6961 6e63  r ""..#: allianc
-0000eed0: 6561 7574 682f 7365 7276 6963 6573 2f6d  eauth/services/m
-0000eee0: 6f64 756c 6573 2f73 6d66 2f76 6965 7773  odules/smf/views
-0000eef0: 2e70 793a 3635 0a23 3a20 616c 6c69 616e  .py:65.#: allian
-0000ef00: 6365 6175 7468 2f73 6572 7669 6365 732f  ceauth/services/
-0000ef10: 6d6f 6475 6c65 732f 736d 662f 7669 6577  modules/smf/view
-0000ef20: 732e 7079 3a38 310a 233a 2061 6c6c 6961  s.py:81.#: allia
-0000ef30: 6e63 6561 7574 682f 7365 7276 6963 6573  nceauth/services
-0000ef40: 2f6d 6f64 756c 6573 2f73 6d66 2f76 6965  /modules/smf/vie
-0000ef50: 7773 2e70 793a 3130 320a 233a 2061 6c6c  ws.py:102.#: all
-0000ef60: 6961 6e63 6561 7574 682f 7365 7276 6963  ianceauth/servic
-0000ef70: 6573 2f6d 6f64 756c 6573 2f73 6d66 2f76  es/modules/smf/v
-0000ef80: 6965 7773 2e70 793a 3132 340a 6d73 6769  iews.py:124.msgi
-0000ef90: 6420 2241 6e20 6572 726f 7220 6f63 6375  d "An error occu
-0000efa0: 7272 6564 2077 6869 6c65 2070 726f 6365  rred while proce
-0000efb0: 7373 696e 6720 796f 7572 2053 4d46 2061  ssing your SMF a
-0000efc0: 6363 6f75 6e74 2e22 0a6d 7367 7374 7220  ccount.".msgstr 
-0000efd0: 2222 0a0a 233a 2061 6c6c 6961 6e63 6561  ""..#: alliancea
-0000efe0: 7574 682f 7365 7276 6963 6573 2f6d 6f64  uth/services/mod
-0000eff0: 756c 6573 2f73 6d66 2f76 6965 7773 2e70  ules/smf/views.p
-0000f000: 793a 3738 0a6d 7367 6964 2022 4465 6163  y:78.msgid "Deac
-0000f010: 7469 7661 7465 6420 534d 4620 6163 636f  tivated SMF acco
-0000f020: 756e 742e 220a 6d73 6773 7472 2022 220a  unt.".msgstr "".
-0000f030: 0a23 3a20 616c 6c69 616e 6365 6175 7468  .#: allianceauth
-0000f040: 2f73 6572 7669 6365 732f 6d6f 6475 6c65  /services/module
-0000f050: 732f 736d 662f 7669 6577 732e 7079 3a39  s/smf/views.py:9
-0000f060: 350a 6d73 6769 6420 2252 6573 6574 2053  5.msgid "Reset S
-0000f070: 4d46 2070 6173 7377 6f72 642e 220a 6d73  MF password.".ms
-0000f080: 6773 7472 2022 220a 0a23 3a20 616c 6c69  gstr ""..#: alli
-0000f090: 616e 6365 6175 7468 2f73 6572 7669 6365  anceauth/service
-0000f0a0: 732f 6d6f 6475 6c65 732f 736d 662f 7669  s/modules/smf/vi
-0000f0b0: 6577 732e 7079 3a31 3231 0a6d 7367 6964  ews.py:121.msgid
-0000f0c0: 2022 5365 7420 534d 4620 7061 7373 776f   "Set SMF passwo
-0000f0d0: 7264 2e22 0a6d 7367 7374 7220 2222 0a0a  rd.".msgstr ""..
-0000f0e0: 233a 2061 6c6c 6961 6e63 6561 7574 682f  #: allianceauth/
-0000f0f0: 7365 7276 6963 6573 2f6d 6f64 756c 6573  services/modules
-0000f100: 2f74 6561 6d73 7065 616b 332f 666f 726d  /teamspeak3/form
-0000f110: 732e 7079 3a31 340a 232c 2070 7974 686f  s.py:14.#, pytho
-0000f120: 6e2d 666f 726d 6174 0a6d 7367 6964 2022  n-format.msgid "
-0000f130: 556e 6162 6c65 2074 6f20 6c6f 6361 7465  Unable to locate
-0000f140: 2075 7365 7220 2573 206f 6e20 7365 7276   user %s on serv
-0000f150: 6572 220a 6d73 6773 7472 2022 220a 0a23  er".msgstr ""..#
-0000f160: 3a20 616c 6c69 616e 6365 6175 7468 2f73  : allianceauth/s
-0000f170: 6572 7669 6365 732f 6d6f 6475 6c65 732f  ervices/modules/
-0000f180: 7465 616d 7370 6561 6b33 2f74 656d 706c  teamspeak3/templ
-0000f190: 6174 6573 2f61 646d 696e 2f74 6561 6d73  ates/admin/teams
-0000f1a0: 7065 616b 332f 6175 7468 7473 2f63 6861  peak3/authts/cha
-0000f1b0: 6e67 655f 6c69 7374 2e68 746d 6c3a 3130  nge_list.html:10
-0000f1c0: 0a6d 7367 6964 2022 5570 6461 7465 2054  .msgid "Update T
-0000f1d0: 6561 6d53 7065 616b 3320 6772 6f75 7073  eamSpeak3 groups
-0000f1e0: 220a 6d73 6773 7472 2022 220a 0a23 3a20  ".msgstr ""..#: 
-0000f1f0: 616c 6c69 616e 6365 6175 7468 2f73 6572  allianceauth/ser
-0000f200: 7669 6365 732f 6d6f 6475 6c65 732f 7465  vices/modules/te
-0000f210: 616d 7370 6561 6b33 2f74 656d 706c 6174  amspeak3/templat
-0000f220: 6573 2f73 6572 7669 6365 732f 7465 616d  es/services/team
-0000f230: 7370 6561 6b33 2f74 6561 6d73 7065 616b  speak3/teamspeak
-0000f240: 335f 7365 7276 6963 655f 6374 726c 2e68  3_service_ctrl.h
-0000f250: 746d 6c3a 360a 6d73 6769 6420 2254 6561  tml:6.msgid "Tea
-0000f260: 6d73 7065 616b 2033 220a 6d73 6773 7472  mspeak 3".msgstr
-0000f270: 2022 220a 0a23 3a20 616c 6c69 616e 6365   ""..#: alliance
-0000f280: 6175 7468 2f73 6572 7669 6365 732f 6d6f  auth/services/mo
-0000f290: 6475 6c65 732f 7465 616d 7370 6561 6b33  dules/teamspeak3
-0000f2a0: 2f74 656d 706c 6174 6573 2f73 6572 7669  /templates/servi
-0000f2b0: 6365 732f 7465 616d 7370 6561 6b33 2f74  ces/teamspeak3/t
-0000f2c0: 6561 6d73 7065 616b 6a6f 696e 2e68 746d  eamspeakjoin.htm
-0000f2d0: 6c3a 360a 6d73 6769 6420 2256 6572 6966  l:6.msgid "Verif
-0000f2e0: 7920 5465 616d 5370 6561 6b33 220a 6d73  y TeamSpeak3".ms
-0000f2f0: 6773 7472 2022 220a 0a23 3a20 616c 6c69  gstr ""..#: alli
-0000f300: 616e 6365 6175 7468 2f73 6572 7669 6365  anceauth/service
-0000f310: 732f 6d6f 6475 6c65 732f 7465 616d 7370  s/modules/teamsp
-0000f320: 6561 6b33 2f74 656d 706c 6174 6573 2f73  eak3/templates/s
-0000f330: 6572 7669 6365 732f 7465 616d 7370 6561  ervices/teamspea
-0000f340: 6b33 2f74 6561 6d73 7065 616b 6a6f 696e  k3/teamspeakjoin
-0000f350: 2e68 746d 6c3a 3130 0a6d 7367 6964 2022  .html:10.msgid "
-0000f360: 5665 7269 6679 2054 6561 6d53 7065 616b  Verify TeamSpeak
-0000f370: 3320 4964 656e 7469 7479 220a 6d73 6773  3 Identity".msgs
-0000f380: 7472 2022 220a 0a23 3a20 616c 6c69 616e  tr ""..#: allian
-0000f390: 6365 6175 7468 2f73 6572 7669 6365 732f  ceauth/services/
-0000f3a0: 6d6f 6475 6c65 732f 7465 616d 7370 6561  modules/teamspea
-0000f3b0: 6b33 2f74 656d 706c 6174 6573 2f73 6572  k3/templates/ser
-0000f3c0: 7669 6365 732f 7465 616d 7370 6561 6b33  vices/teamspeak3
-0000f3d0: 2f74 6561 6d73 7065 616b 6a6f 696e 2e68  /teamspeakjoin.h
-0000f3e0: 746d 6c3a 3135 0a6d 7367 6964 2022 4a6f  tml:15.msgid "Jo
-0000f3f0: 696e 2053 6572 7665 7222 0a6d 7367 7374  in Server".msgst
-0000f400: 7220 2222 0a0a 233a 2061 6c6c 6961 6e63  r ""..#: allianc
-0000f410: 6561 7574 682f 7365 7276 6963 6573 2f6d  eauth/services/m
-0000f420: 6f64 756c 6573 2f74 6561 6d73 7065 616b  odules/teamspeak
-0000f430: 332f 7465 6d70 6c61 7465 732f 7365 7276  3/templates/serv
-0000f440: 6963 6573 2f74 6561 6d73 7065 616b 332f  ices/teamspeak3/
-0000f450: 7465 616d 7370 6561 6b6a 6f69 6e2e 6874  teamspeakjoin.ht
-0000f460: 6d6c 3a32 330a 233a 2061 6c6c 6961 6e63  ml:23.#: allianc
-0000f470: 6561 7574 682f 7365 7276 6963 6573 2f74  eauth/services/t
-0000f480: 656d 706c 6174 6573 2f73 6572 7669 6365  emplates/service
-0000f490: 732f 7365 7276 6963 655f 6372 6564 656e  s/service_creden
-0000f4a0: 7469 616c 732e 6874 6d6c 3a33 300a 233a  tials.html:30.#:
-0000f4b0: 2061 6c6c 6961 6e63 6561 7574 682f 7372   allianceauth/sr
-0000f4c0: 702f 7465 6d70 6c61 7465 732f 7372 702f  p/templates/srp/
-0000f4d0: 6164 642e 6874 6d6c 3a35 310a 6d73 6769  add.html:51.msgi
-0000f4e0: 6420 2243 6f6e 7469 6e75 6522 0a6d 7367  d "Continue".msg
-0000f4f0: 7374 7220 2222 0a0a 233a 2061 6c6c 6961  str ""..#: allia
-0000f500: 6e63 6561 7574 682f 7365 7276 6963 6573  nceauth/services
-0000f510: 2f6d 6f64 756c 6573 2f74 6561 6d73 7065  /modules/teamspe
-0000f520: 616b 332f 7669 6577 732e 7079 3a33 350a  ak3/views.py:35.
-0000f530: 6d73 6769 6420 2241 6374 6976 6174 6564  msgid "Activated
-0000f540: 2054 6561 6d53 7065 616b 3320 6163 636f   TeamSpeak3 acco
-0000f550: 756e 742e 220a 6d73 6773 7472 2022 220a  unt.".msgstr "".
-0000f560: 0a23 3a20 616c 6c69 616e 6365 6175 7468  .#: allianceauth
-0000f570: 2f73 6572 7669 6365 732f 6d6f 6475 6c65  /services/module
-0000f580: 732f 7465 616d 7370 6561 6b33 2f76 6965  s/teamspeak3/vie
-0000f590: 7773 2e70 793a 3338 0a23 3a20 616c 6c69  ws.py:38.#: alli
-0000f5a0: 616e 6365 6175 7468 2f73 6572 7669 6365  anceauth/service
-0000f5b0: 732f 6d6f 6475 6c65 732f 7465 616d 7370  s/modules/teamsp
-0000f5c0: 6561 6b33 2f76 6965 7773 2e70 793a 3734  eak3/views.py:74
-0000f5d0: 0a23 3a20 616c 6c69 616e 6365 6175 7468  .#: allianceauth
-0000f5e0: 2f73 6572 7669 6365 732f 6d6f 6475 6c65  /services/module
-0000f5f0: 732f 7465 616d 7370 6561 6b33 2f76 6965  s/teamspeak3/vie
-0000f600: 7773 2e70 793a 3130 300a 6d73 6769 6420  ws.py:100.msgid 
-0000f610: 2241 6e20 6572 726f 7220 6f63 6375 7272  "An error occurr
-0000f620: 6564 2077 6869 6c65 2070 726f 6365 7373  ed while process
-0000f630: 696e 6720 796f 7572 2054 6561 6d53 7065  ing your TeamSpe
-0000f640: 616b 3320 6163 636f 756e 742e 220a 6d73  ak3 account.".ms
-0000f650: 6773 7472 2022 220a 0a23 3a20 616c 6c69  gstr ""..#: alli
-0000f660: 616e 6365 6175 7468 2f73 6572 7669 6365  anceauth/service
-0000f670: 732f 6d6f 6475 6c65 732f 7465 616d 7370  s/modules/teamsp
-0000f680: 6561 6b33 2f76 6965 7773 2e70 793a 3731  eak3/views.py:71
-0000f690: 0a6d 7367 6964 2022 4465 6163 7469 7661  .msgid "Deactiva
-0000f6a0: 7465 6420 5465 616d 5370 6561 6b33 2061  ted TeamSpeak3 a
-0000f6b0: 6363 6f75 6e74 2e22 0a6d 7367 7374 7220  ccount.".msgstr 
-0000f6c0: 2222 0a0a 233a 2061 6c6c 6961 6e63 6561  ""..#: alliancea
-0000f6d0: 7574 682f 7365 7276 6963 6573 2f6d 6f64  uth/services/mod
-0000f6e0: 756c 6573 2f74 6561 6d73 7065 616b 332f  ules/teamspeak3/
-0000f6f0: 7669 6577 732e 7079 3a39 370a 6d73 6769  views.py:97.msgi
-0000f700: 6420 2252 6573 6574 2054 6561 6d53 7065  d "Reset TeamSpe
-0000f710: 616b 3320 7065 726d 6973 7369 6f6e 206b  ak3 permission k
-0000f720: 6579 2e22 0a6d 7367 7374 7220 2222 0a0a  ey.".msgstr ""..
-0000f730: 233a 2061 6c6c 6961 6e63 6561 7574 682f  #: allianceauth/
-0000f740: 7365 7276 6963 6573 2f6d 6f64 756c 6573  services/modules
-0000f750: 2f78 656e 666f 726f 2f76 6965 7773 2e70  /xenforo/views.p
-0000f760: 793a 3330 0a6d 7367 6964 2022 4163 7469  y:30.msgid "Acti
-0000f770: 7661 7465 6420 5865 6e46 6f72 6f20 6163  vated XenForo ac
-0000f780: 636f 756e 742e 220a 6d73 6773 7472 2022  count.".msgstr "
-0000f790: 220a 0a23 3a20 616c 6c69 616e 6365 6175  "..#: allianceau
-0000f7a0: 7468 2f73 6572 7669 6365 732f 6d6f 6475  th/services/modu
-0000f7b0: 6c65 732f 7865 6e66 6f72 6f2f 7669 6577  les/xenforo/view
-0000f7c0: 732e 7079 3a34 300a 233a 2061 6c6c 6961  s.py:40.#: allia
-0000f7d0: 6e63 6561 7574 682f 7365 7276 6963 6573  nceauth/services
-0000f7e0: 2f6d 6f64 756c 6573 2f78 656e 666f 726f  /modules/xenforo
-0000f7f0: 2f76 6965 7773 2e70 793a 3532 0a23 3a20  /views.py:52.#: 
-0000f800: 616c 6c69 616e 6365 6175 7468 2f73 6572  allianceauth/ser
-0000f810: 7669 6365 732f 6d6f 6475 6c65 732f 7865  vices/modules/xe
-0000f820: 6e66 6f72 6f2f 7669 6577 732e 7079 3a37  nforo/views.py:7
-0000f830: 330a 233a 2061 6c6c 6961 6e63 6561 7574  3.#: allianceaut
-0000f840: 682f 7365 7276 6963 6573 2f6d 6f64 756c  h/services/modul
-0000f850: 6573 2f78 656e 666f 726f 2f76 6965 7773  es/xenforo/views
-0000f860: 2e70 793a 3934 0a6d 7367 6964 2022 416e  .py:94.msgid "An
-0000f870: 2065 7272 6f72 206f 6363 7572 7265 6420   error occurred 
-0000f880: 7768 696c 6520 7072 6f63 6573 7369 6e67  while processing
-0000f890: 2079 6f75 7220 5865 6e46 6f72 6f20 6163   your XenForo ac
-0000f8a0: 636f 756e 742e 220a 6d73 6773 7472 2022  count.".msgstr "
-0000f8b0: 220a 0a23 3a20 616c 6c69 616e 6365 6175  "..#: allianceau
-0000f8c0: 7468 2f73 6572 7669 6365 732f 6d6f 6475  th/services/modu
-0000f8d0: 6c65 732f 7865 6e66 6f72 6f2f 7669 6577  les/xenforo/view
-0000f8e0: 732e 7079 3a35 300a 6d73 6769 6420 2244  s.py:50.msgid "D
-0000f8f0: 6561 6374 6976 6174 6564 2058 656e 466f  eactivated XenFo
-0000f900: 726f 2061 6363 6f75 6e74 2e22 0a6d 7367  ro account.".msg
-0000f910: 7374 7220 2222 0a0a 233a 2061 6c6c 6961  str ""..#: allia
-0000f920: 6e63 6561 7574 682f 7365 7276 6963 6573  nceauth/services
-0000f930: 2f6d 6f64 756c 6573 2f78 656e 666f 726f  /modules/xenforo
-0000f940: 2f76 6965 7773 2e70 793a 3635 0a6d 7367  /views.py:65.msg
-0000f950: 6964 2022 5265 7365 7420 5865 6e46 6f72  id "Reset XenFor
-0000f960: 6f20 6163 636f 756e 7420 7061 7373 776f  o account passwo
-0000f970: 7264 2e22 0a6d 7367 7374 7220 2222 0a0a  rd.".msgstr ""..
-0000f980: 233a 2061 6c6c 6961 6e63 6561 7574 682f  #: allianceauth/
-0000f990: 7365 7276 6963 6573 2f6d 6f64 756c 6573  services/modules
-0000f9a0: 2f78 656e 666f 726f 2f76 6965 7773 2e70  /xenforo/views.p
-0000f9b0: 793a 3931 0a6d 7367 6964 2022 4368 616e  y:91.msgid "Chan
-0000f9c0: 6765 6420 5865 6e46 6f72 6f20 7061 7373  ged XenForo pass
-0000f9d0: 776f 7264 2e22 0a6d 7367 7374 7220 2222  word.".msgstr ""
-0000f9e0: 0a0a 233a 2061 6c6c 6961 6e63 6561 7574  ..#: allianceaut
-0000f9f0: 682f 7365 7276 6963 6573 2f74 656d 706c  h/services/templ
-0000fa00: 6174 6573 2f73 6572 7669 6365 732f 666c  ates/services/fl
-0000fa10: 6565 7466 6f72 6d61 7474 6572 746f 6f6c  eetformattertool
-0000fa20: 2e68 746d 6c3a 360a 233a 2061 6c6c 6961  .html:6.#: allia
-0000fa30: 6e63 6561 7574 682f 7365 7276 6963 6573  nceauth/services
-0000fa40: 2f74 656d 706c 6174 6573 2f73 6572 7669  /templates/servi
-0000fa50: 6365 732f 666c 6565 7466 6f72 6d61 7474  ces/fleetformatt
-0000fa60: 6572 746f 6f6c 2e68 746d 6c3a 3130 0a6d  ertool.html:10.m
-0000fa70: 7367 6964 2022 466c 6565 7420 466f 726d  sgid "Fleet Form
-0000fa80: 6174 7465 7220 546f 6f6c 220a 6d73 6773  atter Tool".msgs
-0000fa90: 7472 2022 220a 0a23 3a20 616c 6c69 616e  tr ""..#: allian
-0000faa0: 6365 6175 7468 2f73 6572 7669 6365 732f  ceauth/services/
-0000fab0: 7465 6d70 6c61 7465 732f 7365 7276 6963  templates/servic
-0000fac0: 6573 2f66 6c65 6574 666f 726d 6174 7465  es/fleetformatte
-0000fad0: 7274 6f6f 6c2e 6874 6d6c 3a31 380a 6d73  rtool.html:18.ms
-0000fae0: 6769 6420 2246 6c65 6574 2044 6574 6169  gid "Fleet Detai
-0000faf0: 6c73 220a 6d73 6773 7472 2022 220a 0a23  ls".msgstr ""..#
-0000fb00: 3a20 616c 6c69 616e 6365 6175 7468 2f73  : allianceauth/s
-0000fb10: 6572 7669 6365 732f 7465 6d70 6c61 7465  ervices/template
-0000fb20: 732f 7365 7276 6963 6573 2f66 6c65 6574  s/services/fleet
-0000fb30: 666f 726d 6174 7465 7274 6f6f 6c2e 6874  formattertool.ht
-0000fb40: 6d6c 3a33 370a 6d73 6769 6420 2246 6f72  ml:37.msgid "For
-0000fb50: 6d61 7422 0a6d 7367 7374 7220 2222 0a0a  mat".msgstr ""..
-0000fb60: 233a 2061 6c6c 6961 6e63 6561 7574 682f  #: allianceauth/
-0000fb70: 7365 7276 6963 6573 2f74 656d 706c 6174  services/templat
-0000fb80: 6573 2f73 6572 7669 6365 732f 7365 7276  es/services/serv
-0000fb90: 6963 655f 636f 6e66 6972 6d5f 6465 6c65  ice_confirm_dele
-0000fba0: 7465 2e68 746d 6c3a 360a 233a 2061 6c6c  te.html:6.#: all
-0000fbb0: 6961 6e63 6561 7574 682f 7365 7276 6963  ianceauth/servic
-0000fbc0: 6573 2f74 656d 706c 6174 6573 2f73 6572  es/templates/ser
-0000fbd0: 7669 6365 732f 7365 7276 6963 655f 636f  vices/service_co
-0000fbe0: 6e66 6972 6d5f 6465 6c65 7465 2e68 746d  nfirm_delete.htm
-0000fbf0: 6c3a 3136 0a23 2c20 7079 7468 6f6e 2d66  l:16.#, python-f
-0000fc00: 6f72 6d61 740a 6d73 6769 6420 2244 656c  ormat.msgid "Del
-0000fc10: 6574 6520 2528 7365 7276 6963 655f 6e61  ete %(service_na
-0000fc20: 6d65 2973 2041 6363 6f75 6e74 3f22 0a6d  me)s Account?".m
-0000fc30: 7367 7374 7220 2222 0a0a 233a 2061 6c6c  sgstr ""..#: all
-0000fc40: 6961 6e63 6561 7574 682f 7365 7276 6963  ianceauth/servic
-0000fc50: 6573 2f74 656d 706c 6174 6573 2f73 6572  es/templates/ser
-0000fc60: 7669 6365 732f 7365 7276 6963 655f 636f  vices/service_co
-0000fc70: 6e66 6972 6d5f 6465 6c65 7465 2e68 746d  nfirm_delete.htm
-0000fc80: 6c3a 3130 0a23 3a20 616c 6c69 616e 6365  l:10.#: alliance
-0000fc90: 6175 7468 2f73 6572 7669 6365 732f 7465  auth/services/te
-0000fca0: 6d70 6c61 7465 732f 7365 7276 6963 6573  mplates/services
-0000fcb0: 2f73 6572 7669 6365 5f63 7265 6465 6e74  /service_credent
-0000fcc0: 6961 6c73 2e68 746d 6c3a 3130 0a23 3a20  ials.html:10.#: 
-0000fcd0: 616c 6c69 616e 6365 6175 7468 2f73 6572  allianceauth/ser
-0000fce0: 7669 6365 732f 7465 6d70 6c61 7465 732f  vices/templates/
-0000fcf0: 7365 7276 6963 6573 2f73 6572 7669 6365  services/service
-0000fd00: 5f70 6173 7377 6f72 642e 6874 6d6c 3a31  _password.html:1
-0000fd10: 310a 233a 2061 6c6c 6961 6e63 6561 7574  1.#: allianceaut
-0000fd20: 682f 7365 7276 6963 6573 2f74 656d 706c  h/services/templ
-0000fd30: 6174 6573 2f73 6572 7669 6365 732f 7365  ates/services/se
-0000fd40: 7276 6963 6573 2e68 746d 6c3a 390a 6d73  rvices.html:9.ms
-0000fd50: 6769 6420 2241 7661 696c 6162 6c65 2053  gid "Available S
-0000fd60: 6572 7669 6365 7322 0a6d 7367 7374 7220  ervices".msgstr 
-0000fd70: 2222 0a0a 233a 2061 6c6c 6961 6e63 6561  ""..#: alliancea
-0000fd80: 7574 682f 7365 7276 6963 6573 2f74 656d  uth/services/tem
-0000fd90: 706c 6174 6573 2f73 6572 7669 6365 732f  plates/services/
-0000fda0: 7365 7276 6963 655f 636f 6e66 6972 6d5f  service_confirm_
-0000fdb0: 6465 6c65 7465 2e68 746d 6c3a 3234 0a23  delete.html:24.#
-0000fdc0: 2c20 7079 7468 6f6e 2d66 6f72 6d61 740a  , python-format.
-0000fdd0: 6d73 6769 6420 2222 0a22 4172 6520 796f  msgid ""."Are yo
-0000fde0: 7520 7375 7265 2079 6f75 2077 616e 7420  u sure you want 
-0000fdf0: 746f 2064 656c 6574 6520 796f 7572 2025  to delete your %
-0000fe00: 2873 6572 7669 6365 5f6e 616d 6529 7320  (service_name)s 
-0000fe10: 6163 636f 756e 7420 2528 6f62 6a65 6374  account %(object
-0000fe20: 2973 3f22 0a6d 7367 7374 7220 2222 0a0a  )s?".msgstr ""..
-0000fe30: 233a 2061 6c6c 6961 6e63 6561 7574 682f  #: allianceauth/
-0000fe40: 7365 7276 6963 6573 2f74 656d 706c 6174  services/templat
-0000fe50: 6573 2f73 6572 7669 6365 732f 7365 7276  es/services/serv
-0000fe60: 6963 655f 6372 6564 656e 7469 616c 732e  ice_credentials.
-0000fe70: 6874 6d6c 3a36 0a23 3a20 616c 6c69 616e  html:6.#: allian
-0000fe80: 6365 6175 7468 2f73 6572 7669 6365 732f  ceauth/services/
-0000fe90: 7465 6d70 6c61 7465 732f 7365 7276 6963  templates/servic
-0000fea0: 6573 2f73 6572 7669 6365 5f63 7265 6465  es/service_crede
-0000feb0: 6e74 6961 6c73 2e68 746d 6c3a 3136 0a23  ntials.html:16.#
-0000fec0: 2c20 7079 7468 6f6e 2d66 6f72 6d61 740a  , python-format.
-0000fed0: 6d73 6769 6420 2225 2873 6572 7669 6365  msgid "%(service
-0000fee0: 5f6e 616d 6529 7320 4372 6564 656e 7469  _name)s Credenti
-0000fef0: 616c 7322 0a6d 7367 7374 7220 2222 0a0a  als".msgstr ""..
-0000ff00: 233a 2061 6c6c 6961 6e63 6561 7574 682f  #: allianceauth/
-0000ff10: 7365 7276 6963 6573 2f74 656d 706c 6174  services/templat
-0000ff20: 6573 2f73 6572 7669 6365 732f 7365 7276  es/services/serv
-0000ff30: 6963 655f 7061 7373 776f 7264 2e68 746d  ice_password.htm
-0000ff40: 6c3a 370a 232c 2070 7974 686f 6e2d 666f  l:7.#, python-fo
-0000ff50: 726d 6174 0a6d 7367 6964 2022 2528 7365  rmat.msgid "%(se
-0000ff60: 7276 6963 655f 6e61 6d65 2973 2050 6173  rvice_name)s Pas
-0000ff70: 7377 6f72 6420 4368 616e 6765 220a 6d73  sword Change".ms
-0000ff80: 6773 7472 2022 220a 0a23 3a20 616c 6c69  gstr ""..#: alli
-0000ff90: 616e 6365 6175 7468 2f73 6572 7669 6365  anceauth/service
-0000ffa0: 732f 7465 6d70 6c61 7465 732f 7365 7276  s/templates/serv
-0000ffb0: 6963 6573 2f73 6572 7669 6365 5f70 6173  ices/service_pas
-0000ffc0: 7377 6f72 642e 6874 6d6c 3a31 370a 232c  sword.html:17.#,
-0000ffd0: 2070 7974 686f 6e2d 666f 726d 6174 0a6d   python-format.m
-0000ffe0: 7367 6964 2022 5365 7420 2528 7365 7276  sgid "Set %(serv
-0000fff0: 6963 655f 6e61 6d65 2973 2050 6173 7377  ice_name)s Passw
-00010000: 6f72 6422 0a6d 7367 7374 7220 2222 0a0a  ord".msgstr ""..
-00010010: 233a 2061 6c6c 6961 6e63 6561 7574 682f  #: allianceauth/
-00010020: 7365 7276 6963 6573 2f74 656d 706c 6174  services/templat
-00010030: 6573 2f73 6572 7669 6365 732f 7365 7276  es/services/serv
-00010040: 6963 655f 7374 6174 7573 2e68 746d 6c3a  ice_status.html:
-00010050: 350a 6d73 6769 6420 2245 6e61 626c 6564  5.msgid "Enabled
-00010060: 220a 6d73 6773 7472 2022 220a 0a23 3a20  ".msgstr ""..#: 
-00010070: 616c 6c69 616e 6365 6175 7468 2f73 6572  allianceauth/ser
-00010080: 7669 6365 732f 7465 6d70 6c61 7465 732f  vices/templates/
-00010090: 7365 7276 6963 6573 2f73 6572 7669 6365  services/service
-000100a0: 5f73 7461 7475 732e 6874 6d6c 3a37 0a23  _status.html:7.#
-000100b0: 3a20 616c 6c69 616e 6365 6175 7468 2f73  : allianceauth/s
-000100c0: 7270 2f74 656d 706c 6174 6573 2f73 7270  rp/templates/srp
-000100d0: 2f6d 616e 6167 656d 656e 742e 6874 6d6c  /management.html
-000100e0: 3a37 380a 6d73 6769 6420 2244 6973 6162  :78.msgid "Disab
-000100f0: 6c65 6422 0a6d 7367 7374 7220 2222 0a0a  led".msgstr ""..
-00010100: 233a 2061 6c6c 6961 6e63 6561 7574 682f  #: allianceauth/
-00010110: 7365 7276 6963 6573 2f74 656d 706c 6174  services/templat
-00010120: 6573 2f73 6572 7669 6365 732f 7365 7276  es/services/serv
-00010130: 6963 6573 2e68 746d 6c3a 350a 6d73 6769  ices.html:5.msgi
-00010140: 6420 2253 6572 7669 6365 7320 4d61 6e61  d "Services Mana
-00010150: 6765 6d65 6e74 220a 6d73 6773 7472 2022  gement".msgstr "
-00010160: 220a 0a23 3a20 616c 6c69 616e 6365 6175  "..#: allianceau
-00010170: 7468 2f73 6572 7669 6365 732f 7465 6d70  th/services/temp
-00010180: 6c61 7465 732f 7365 7276 6963 6573 2f73  lates/services/s
-00010190: 6572 7669 6365 732e 6874 6d6c 3a32 300a  ervices.html:20.
-000101a0: 6d73 6769 6420 224c 6567 656e 6422 0a6d  msgid "Legend".m
-000101b0: 7367 7374 7220 2222 0a0a 233a 2061 6c6c  sgstr ""..#: all
-000101c0: 6961 6e63 6561 7574 682f 7365 7276 6963  ianceauth/servic
-000101d0: 6573 2f74 656d 706c 6174 6573 2f73 6572  es/templates/ser
-000101e0: 7669 6365 732f 7365 7276 6963 6573 2e68  vices/services.h
-000101f0: 746d 6c3a 3237 0a6d 7367 6964 2022 436c  tml:27.msgid "Cl
-00010200: 6963 6b20 746f 2061 6374 6976 6174 6520  ick to activate 
-00010210: 7468 6520 7365 7276 6963 6520 666f 7220  the service for 
-00010220: 796f 7572 2075 7365 722e 220a 6d73 6773  your user.".msgs
-00010230: 7472 2022 220a 0a23 3a20 616c 6c69 616e  tr ""..#: allian
-00010240: 6365 6175 7468 2f73 6572 7669 6365 732f  ceauth/services/
-00010250: 7465 6d70 6c61 7465 732f 7365 7276 6963  templates/servic
-00010260: 6573 2f73 6572 7669 6365 732e 6874 6d6c  es/services.html
-00010270: 3a33 360a 6d73 6769 6420 2243 6c69 636b  :36.msgid "Click
-00010280: 2074 6f20 6d61 6e75 616c 6c79 2073 6574   to manually set
-00010290: 2079 6f75 7220 7061 7373 776f 7264 2e22   your password."
-000102a0: 0a6d 7367 7374 7220 2222 0a0a 233a 2061  .msgstr ""..#: a
-000102b0: 6c6c 6961 6e63 6561 7574 682f 7365 7276  llianceauth/serv
-000102c0: 6963 6573 2f74 656d 706c 6174 6573 2f73  ices/templates/s
-000102d0: 6572 7669 6365 732f 7365 7276 6963 6573  ervices/services
-000102e0: 2e68 746d 6c3a 3435 0a6d 7367 6964 2022  .html:45.msgid "
-000102f0: 436c 6963 6b20 746f 2072 616e 646f 6d6c  Click to randoml
-00010300: 7920 6765 6e65 7261 7465 2079 6f75 7220  y generate your 
-00010310: 7061 7373 776f 7264 2e22 0a6d 7367 7374  password.".msgst
-00010320: 7220 2222 0a0a 233a 2061 6c6c 6961 6e63  r ""..#: allianc
-00010330: 6561 7574 682f 7365 7276 6963 6573 2f74  eauth/services/t
-00010340: 656d 706c 6174 6573 2f73 6572 7669 6365  emplates/service
-00010350: 732f 7365 7276 6963 6573 2e68 746d 6c3a  s/services.html:
-00010360: 3534 0a6d 7367 6964 2022 436c 6963 6b20  54.msgid "Click 
-00010370: 746f 2064 6561 6374 6976 6174 6520 7468  to deactivate th
-00010380: 6520 7365 7276 6963 6520 666f 7220 796f  e service for yo
-00010390: 7572 2075 7365 7222 0a6d 7367 7374 7220  ur user".msgstr 
-000103a0: 2222 0a0a 233a 2061 6c6c 6961 6e63 6561  ""..#: alliancea
-000103b0: 7574 682f 7365 7276 6963 6573 2f74 656d  uth/services/tem
-000103c0: 706c 6174 6573 2f73 6572 7669 6365 732f  plates/services/
-000103d0: 7365 7276 6963 6573 2e68 746d 6c3a 3630  services.html:60
-000103e0: 0a6d 7367 6964 2022 220a 2253 6f6d 6520  .msgid ""."Some 
-000103f0: 7365 7276 6963 6573 2070 726f 7669 6465  services provide
-00010400: 2064 6966 6665 7265 6e74 206f 7074 696f   different optio
-00010410: 6e73 2e20 486f 7665 7220 6f76 6572 2074  ns. Hover over t
-00010420: 6865 2062 7574 746f 6e73 2074 6f20 7365  he buttons to se
-00010430: 6520 6d6f 7265 2e22 0a6d 7367 7374 7220  e more.".msgstr 
-00010440: 2222 0a0a 233a 2061 6c6c 6961 6e63 6561  ""..#: alliancea
-00010450: 7574 682f 7372 702f 6175 7468 5f68 6f6f  uth/srp/auth_hoo
-00010460: 6b73 2e70 793a 3134 0a6d 7367 6964 2022  ks.py:14.msgid "
-00010470: 5368 6970 2052 6570 6c61 6365 6d65 6e74  Ship Replacement
-00010480: 220a 6d73 6773 7472 2022 220a 0a23 3a20  ".msgstr ""..#: 
-00010490: 616c 6c69 616e 6365 6175 7468 2f73 7270  allianceauth/srp
-000104a0: 2f66 6f72 6d2e 7079 3a39 2061 6c6c 6961  /form.py:9 allia
-000104b0: 6e63 6561 7574 682f 7372 702f 7465 6d70  nceauth/srp/temp
-000104c0: 6c61 7465 732f 7372 702f 6d61 6e61 6765  lates/srp/manage
-000104d0: 6d65 6e74 2e68 746d 6c3a 3435 0a6d 7367  ment.html:45.msg
-000104e0: 6964 2022 466c 6565 7420 5469 6d65 220a  id "Fleet Time".
-000104f0: 6d73 6773 7472 2022 220a 0a23 3a20 616c  msgstr ""..#: al
-00010500: 6c69 616e 6365 6175 7468 2f73 7270 2f66  lianceauth/srp/f
-00010510: 6f72 6d2e 7079 3a31 300a 233a 2061 6c6c  orm.py:10.#: all
-00010520: 6961 6e63 6561 7574 682f 7372 702f 7465  ianceauth/srp/te
-00010530: 6d70 6c61 7465 732f 7372 702f 6d61 6e61  mplates/srp/mana
-00010540: 6765 6d65 6e74 2e68 746d 6c3a 3436 0a6d  gement.html:46.m
-00010550: 7367 6964 2022 466c 6565 7420 446f 6374  sgid "Fleet Doct
-00010560: 7269 6e65 220a 6d73 6773 7472 2022 220a  rine".msgstr "".
-00010570: 0a23 3a20 616c 6c69 616e 6365 6175 7468  .#: allianceauth
-00010580: 2f73 7270 2f66 6f72 6d2e 7079 3a31 360a  /srp/form.py:16.
-00010590: 6d73 6769 6420 224b 696c 6c62 6f61 7264  msgid "Killboard
-000105a0: 204c 696e 6b20 287a 6b69 6c6c 626f 6172   Link (zkillboar
-000105b0: 642e 636f 6d20 6f72 206b 622e 6576 6574  d.com or kb.evet
-000105c0: 6f6f 6c73 2e6f 7267 2922 0a6d 7367 7374  ools.org)".msgst
-000105d0: 7220 2222 0a0a 233a 2061 6c6c 6961 6e63  r ""..#: allianc
-000105e0: 6561 7574 682f 7372 702f 666f 726d 2e70  eauth/srp/form.p
-000105f0: 793a 3334 0a6d 7367 6964 2022 496e 7661  y:34.msgid "Inva
-00010600: 6c69 6420 4c69 6e6b 2e20 506c 6561 7365  lid Link. Please
-00010610: 2075 7365 207a 6b69 6c6c 626f 6172 642e   use zkillboard.
-00010620: 636f 6d20 6f72 206b 622e 6576 6574 6f6f  com or kb.evetoo
-00010630: 6c73 2e6f 7267 220a 6d73 6773 7472 2022  ls.org".msgstr "
-00010640: 220a 0a23 3a20 616c 6c69 616e 6365 6175  "..#: allianceau
-00010650: 7468 2f73 7270 2f66 6f72 6d2e 7079 3a34  th/srp/form.py:4
-00010660: 360a 6d73 6769 6420 2249 6e76 616c 6964  6.msgid "Invalid
-00010670: 204c 696e 6b2e 2050 6c65 6173 6520 706f   Link. Please po
-00010680: 7374 2061 2064 6972 6563 7420 6c69 6e6b  st a direct link
-00010690: 2074 6f20 6120 6b69 6c6c 6d61 696c 2e22   to a killmail."
-000106a0: 0a6d 7367 7374 7220 2222 0a0a 233a 2061  .msgstr ""..#: a
-000106b0: 6c6c 6961 6e63 6561 7574 682f 7372 702f  llianceauth/srp/
-000106c0: 666f 726d 2e70 793a 3533 0a6d 7367 6964  form.py:53.msgid
-000106d0: 2022 4166 7465 7220 4163 7469 6f6e 2052   "After Action R
-000106e0: 6570 6f72 7420 4c69 6e6b 220a 6d73 6773  eport Link".msgs
-000106f0: 7472 2022 220a 0a23 3a20 616c 6c69 616e  tr ""..#: allian
-00010700: 6365 6175 7468 2f73 7270 2f74 656d 706c  ceauth/srp/templ
-00010710: 6174 6573 2f73 7270 2f61 6464 2e68 746d  ates/srp/add.htm
-00010720: 6c3a 370a 6d73 6769 6420 2253 5250 2046  l:7.msgid "SRP F
-00010730: 6c65 6574 2043 7265 6174 6522 0a6d 7367  leet Create".msg
-00010740: 7374 7220 2222 0a0a 233a 2061 6c6c 6961  str ""..#: allia
-00010750: 6e63 6561 7574 682f 7372 702f 7465 6d70  nceauth/srp/temp
-00010760: 6c61 7465 732f 7372 702f 6164 642e 6874  lates/srp/add.ht
-00010770: 6d6c 3a31 310a 233a 2061 6c6c 6961 6e63  ml:11.#: allianc
-00010780: 6561 7574 682f 7372 702f 7465 6d70 6c61  eauth/srp/templa
-00010790: 7465 732f 7372 702f 6461 7461 2e68 746d  tes/srp/data.htm
-000107a0: 6c3a 3131 0a23 3a20 616c 6c69 616e 6365  l:11.#: alliance
-000107b0: 6175 7468 2f73 7270 2f74 656d 706c 6174  auth/srp/templat
-000107c0: 6573 2f73 7270 2f6d 616e 6167 656d 656e  es/srp/managemen
-000107d0: 742e 6874 6d6c 3a31 310a 233a 2061 6c6c  t.html:11.#: all
-000107e0: 6961 6e63 6561 7574 682f 7372 702f 7465  ianceauth/srp/te
-000107f0: 6d70 6c61 7465 732f 7372 702f 7265 7175  mplates/srp/requ
-00010800: 6573 742e 6874 6d6c 3a31 310a 233a 2061  est.html:11.#: a
-00010810: 6c6c 6961 6e63 6561 7574 682f 7372 702f  llianceauth/srp/
-00010820: 7465 6d70 6c61 7465 732f 7372 702f 7570  templates/srp/up
-00010830: 6461 7465 2e68 746d 6c3a 3131 0a6d 7367  date.html:11.msg
-00010840: 6964 2022 5368 6970 2052 6570 6c61 6365  id "Ship Replace
-00010850: 6d65 6e74 2050 726f 6772 616d 220a 6d73  ment Program".ms
-00010860: 6773 7472 2022 220a 0a23 3a20 616c 6c69  gstr ""..#: alli
-00010870: 616e 6365 6175 7468 2f73 7270 2f74 656d  anceauth/srp/tem
-00010880: 706c 6174 6573 2f73 7270 2f61 6464 2e68  plates/srp/add.h
-00010890: 746d 6c3a 3230 0a6d 7367 6964 2022 4372  tml:20.msgid "Cr
-000108a0: 6561 7465 2053 5250 2046 6c65 6574 220a  eate SRP Fleet".
-000108b0: 6d73 6773 7472 2022 220a 0a23 3a20 616c  msgstr ""..#: al
-000108c0: 6c69 616e 6365 6175 7468 2f73 7270 2f74  lianceauth/srp/t
-000108d0: 656d 706c 6174 6573 2f73 7270 2f61 6464  emplates/srp/add
-000108e0: 2e68 746d 6c3a 3236 0a6d 7367 6964 2022  .html:26.msgid "
-000108f0: 5352 5020 666c 6565 7420 6465 7461 696c  SRP fleet detail
-00010900: 7322 0a6d 7367 7374 7220 2222 0a0a 233a  s".msgstr ""..#:
-00010910: 2061 6c6c 6961 6e63 6561 7574 682f 7372   allianceauth/sr
-00010920: 702f 7465 6d70 6c61 7465 732f 7372 702f  p/templates/srp/
-00010930: 6164 642e 6874 6d6c 3a34 300a 6d73 6769  add.html:40.msgi
-00010940: 6420 2243 7265 6174 6520 5352 5020 666c  d "Create SRP fl
-00010950: 6565 7422 0a6d 7367 7374 7220 2222 0a0a  eet".msgstr ""..
-00010960: 233a 2061 6c6c 6961 6e63 6561 7574 682f  #: allianceauth/
-00010970: 7372 702f 7465 6d70 6c61 7465 732f 7372  srp/templates/sr
-00010980: 702f 6164 642e 6874 6d6c 3a34 360a 6d73  p/add.html:46.ms
-00010990: 6769 6420 2247 6976 6520 7468 6973 206c  gid "Give this l
-000109a0: 696e 6b20 746f 2074 6865 206c 696e 6520  ink to the line 
-000109b0: 6d65 6d62 6572 732e 220a 6d73 6773 7472  members.".msgstr
-000109c0: 2022 220a 0a23 3a20 616c 6c69 616e 6365   ""..#: alliance
-000109d0: 6175 7468 2f73 7270 2f74 656d 706c 6174  auth/srp/templat
-000109e0: 6573 2f73 7270 2f64 6174 612e 6874 6d6c  es/srp/data.html
-000109f0: 3a37 0a23 3a20 616c 6c69 616e 6365 6175  :7.#: allianceau
-00010a00: 7468 2f73 7270 2f74 656d 706c 6174 6573  th/srp/templates
-00010a10: 2f73 7270 2f64 6174 612e 6874 6d6c 3a33  /srp/data.html:3
-00010a20: 380a 6d73 6769 6420 2253 5250 2046 6c65  8.msgid "SRP Fle
-00010a30: 6574 2044 6174 6122 0a6d 7367 7374 7220  et Data".msgstr 
-00010a40: 2222 0a0a 233a 2061 6c6c 6961 6e63 6561  ""..#: alliancea
-00010a50: 7574 682f 7372 702f 7465 6d70 6c61 7465  uth/srp/template
-00010a60: 732f 7372 702f 6461 7461 2e68 746d 6c3a  s/srp/data.html:
-00010a70: 3136 0a6d 7367 6964 2022 5669 6577 2046  16.msgid "View F
-00010a80: 6c65 6574 7322 0a6d 7367 7374 7220 2222  leets".msgstr ""
-00010a90: 0a0a 233a 2061 6c6c 6961 6e63 6561 7574  ..#: allianceaut
-00010aa0: 682f 7372 702f 7465 6d70 6c61 7465 732f  h/srp/templates/
-00010ab0: 7372 702f 6461 7461 2e68 746d 6c3a 3235  srp/data.html:25
-00010ac0: 0a6d 7367 6964 2022 4d61 726b 2049 6e63  .msgid "Mark Inc
-00010ad0: 6f6d 706c 6574 6522 0a6d 7367 7374 7220  omplete".msgstr 
-00010ae0: 2222 0a0a 233a 2061 6c6c 6961 6e63 6561  ""..#: alliancea
-00010af0: 7574 682f 7372 702f 7465 6d70 6c61 7465  uth/srp/template
-00010b00: 732f 7372 702f 6461 7461 2e68 746d 6c3a  s/srp/data.html:
-00010b10: 3239 0a6d 7367 6964 2022 4d61 726b 2043  29.msgid "Mark C
-00010b20: 6f6d 706c 6574 6564 220a 6d73 6773 7472  ompleted".msgstr
-00010b30: 2022 220a 0a23 3a20 616c 6c69 616e 6365   ""..#: alliance
-00010b40: 6175 7468 2f73 7270 2f74 656d 706c 6174  auth/srp/templat
-00010b50: 6573 2f73 7270 2f64 6174 612e 6874 6d6c  es/srp/data.html
-00010b60: 3a34 370a 233a 2061 6c6c 6961 6e63 6561  :47.#: alliancea
-00010b70: 7574 682f 7372 702f 7465 6d70 6c61 7465  uth/srp/template
-00010b80: 732f 7372 702f 6461 7461 2e68 746d 6c3a  s/srp/data.html:
-00010b90: 3133 380a 6d73 6769 6420 2254 6f74 616c  138.msgid "Total
-00010ba0: 204c 6f73 7365 733a 220a 6d73 6773 7472   Losses:".msgstr
-00010bb0: 2022 220a 0a23 3a20 616c 6c69 616e 6365   ""..#: alliance
-00010bc0: 6175 7468 2f73 7270 2f74 656d 706c 6174  auth/srp/templat
-00010bd0: 6573 2f73 7270 2f64 6174 612e 6874 6d6c  es/srp/data.html
-00010be0: 3a34 380a 233a 2061 6c6c 6961 6e63 6561  :48.#: alliancea
-00010bf0: 7574 682f 7372 702f 7465 6d70 6c61 7465  uth/srp/template
-00010c00: 732f 7372 702f 6461 7461 2e68 746d 6c3a  s/srp/data.html:
-00010c10: 3133 390a 233a 2061 6c6c 6961 6e63 6561  139.#: alliancea
-00010c20: 7574 682f 7372 702f 7465 6d70 6c61 7465  uth/srp/template
-00010c30: 732f 7372 702f 6d61 6e61 6765 6d65 6e74  s/srp/management
-00010c40: 2e68 746d 6c3a 3336 0a6d 7367 6964 2022  .html:36.msgid "
-00010c50: 546f 7461 6c20 4953 4b20 436f 7374 3a22  Total ISK Cost:"
-00010c60: 0a6d 7367 7374 7220 2222 0a0a 233a 2061  .msgstr ""..#: a
-00010c70: 6c6c 6961 6e63 6561 7574 682f 7372 702f  llianceauth/srp/
-00010c80: 7465 6d70 6c61 7465 732f 7372 702f 6461  templates/srp/da
-00010c90: 7461 2e68 746d 6c3a 3539 0a23 3a20 616c  ta.html:59.#: al
-00010ca0: 6c69 616e 6365 6175 7468 2f73 7270 2f74  lianceauth/srp/t
-00010cb0: 656d 706c 6174 6573 2f73 7270 2f64 6174  emplates/srp/dat
-00010cc0: 612e 6874 6d6c 3a31 3530 0a6d 7367 6964  a.html:150.msgid
-00010cd0: 2022 4172 6520 796f 7520 7375 7265 2079   "Are you sure y
-00010ce0: 6f75 2077 616e 7420 746f 2064 656c 6574  ou want to delet
-00010cf0: 6520 5352 5020 7265 7175 6573 7473 3f22  e SRP requests?"
-00010d00: 0a6d 7367 7374 7220 2222 0a0a 233a 2061  .msgstr ""..#: a
-00010d10: 6c6c 6961 6e63 6561 7574 682f 7372 702f  llianceauth/srp/
-00010d20: 7465 6d70 6c61 7465 732f 7372 702f 6461  templates/srp/da
-00010d30: 7461 2e68 746d 6c3a 3639 0a6d 7367 6964  ta.html:69.msgid
-00010d40: 2022 5069 6c6f 7420 4e61 6d65 220a 6d73   "Pilot Name".ms
-00010d50: 6773 7472 2022 220a 0a23 3a20 616c 6c69  gstr ""..#: alli
-00010d60: 616e 6365 6175 7468 2f73 7270 2f74 656d  anceauth/srp/tem
-00010d70: 706c 6174 6573 2f73 7270 2f64 6174 612e  plates/srp/data.
-00010d80: 6874 6d6c 3a37 300a 6d73 6769 6420 224b  html:70.msgid "K
-00010d90: 696c 6c62 6f61 7264 204c 696e 6b22 0a6d  illboard Link".m
-00010da0: 7367 7374 7220 2222 0a0a 233a 2061 6c6c  sgstr ""..#: all
-00010db0: 6961 6e63 6561 7574 682f 7372 702f 7465  ianceauth/srp/te
-00010dc0: 6d70 6c61 7465 732f 7372 702f 6461 7461  mplates/srp/data
-00010dd0: 2e68 746d 6c3a 3732 0a6d 7367 6964 2022  .html:72.msgid "
-00010de0: 5368 6970 2054 7970 6522 0a6d 7367 7374  Ship Type".msgst
-00010df0: 7220 2222 0a0a 233a 2061 6c6c 6961 6e63  r ""..#: allianc
-00010e00: 6561 7574 682f 7372 702f 7465 6d70 6c61  eauth/srp/templa
-00010e10: 7465 732f 7372 702f 6461 7461 2e68 746d  tes/srp/data.htm
-00010e20: 6c3a 3733 0a6d 7367 6964 2022 4b69 6c6c  l:73.msgid "Kill
-00010e30: 626f 6172 6420 4c6f 7373 2041 6d74 220a  board Loss Amt".
-00010e40: 6d73 6773 7472 2022 220a 0a23 3a20 616c  msgstr ""..#: al
-00010e50: 6c69 616e 6365 6175 7468 2f73 7270 2f74  lianceauth/srp/t
-00010e60: 656d 706c 6174 6573 2f73 7270 2f64 6174  emplates/srp/dat
-00010e70: 612e 6874 6d6c 3a37 350a 6d73 6769 6420  a.html:75.msgid 
-00010e80: 2253 5250 2049 534b 2043 6f73 7422 0a6d  "SRP ISK Cost".m
-00010e90: 7367 7374 7220 2222 0a0a 233a 2061 6c6c  sgstr ""..#: all
-00010ea0: 6961 6e63 6561 7574 682f 7372 702f 7465  ianceauth/srp/te
-00010eb0: 6d70 6c61 7465 732f 7372 702f 6461 7461  mplates/srp/data
-00010ec0: 2e68 746d 6c3a 3736 0a6d 7367 6964 2022  .html:76.msgid "
-00010ed0: 436c 6963 6b20 7661 6c75 6520 746f 2065  Click value to e
-00010ee0: 6469 7420 456e 7465 7220 746f 2073 6176  dit Enter to sav
-00010ef0: 6520 2620 6e65 7874 2045 5343 2074 6f20  e & next ESC to 
-00010f00: 6361 6e63 656c 220a 6d73 6773 7472 2022  cancel".msgstr "
-00010f10: 220a 0a23 3a20 616c 6c69 616e 6365 6175  "..#: allianceau
-00010f20: 7468 2f73 7270 2f74 656d 706c 6174 6573  th/srp/templates
-00010f30: 2f73 7270 2f64 6174 612e 6874 6d6c 3a37  /srp/data.html:7
-00010f40: 390a 6d73 6769 6420 2250 6f73 7420 5469  9.msgid "Post Ti
-00010f50: 6d65 220a 6d73 6773 7472 2022 220a 0a23  me".msgstr ""..#
-00010f60: 3a20 616c 6c69 616e 6365 6175 7468 2f73  : allianceauth/s
-00010f70: 7270 2f74 656d 706c 6174 6573 2f73 7270  rp/templates/srp
-00010f80: 2f64 6174 612e 6874 6d6c 3a39 380a 233a  /data.html:98.#:
-00010f90: 2061 6c6c 6961 6e63 6561 7574 682f 7372   allianceauth/sr
-00010fa0: 702f 7465 6d70 6c61 7465 732f 7372 702f  p/templates/srp/
-00010fb0: 6d61 6e61 6765 6d65 6e74 2e68 746d 6c3a  management.html:
-00010fc0: 3730 0a6d 7367 6964 2022 4c69 6e6b 220a  70.msgid "Link".
-00010fd0: 6d73 6773 7472 2022 220a 0a23 3a20 616c  msgstr ""..#: al
-00010fe0: 6c69 616e 6365 6175 7468 2f73 7270 2f74  lianceauth/srp/t
-00010ff0: 656d 706c 6174 6573 2f73 7270 2f64 6174  emplates/srp/dat
-00011000: 612e 6874 6d6c 3a31 3539 0a6d 7367 6964  a.html:159.msgid
-00011010: 2022 4e6f 2053 5250 2072 6571 7565 7374   "No SRP request
-00011020: 7320 666f 7220 7468 6973 2066 6c65 6574  s for this fleet
-00011030: 2e22 0a6d 7367 7374 7220 2222 0a0a 233a  .".msgstr ""..#:
-00011040: 2061 6c6c 6961 6e63 6561 7574 682f 7372   allianceauth/sr
-00011050: 702f 7465 6d70 6c61 7465 732f 7372 702f  p/templates/srp/
-00011060: 6d61 6e61 6765 6d65 6e74 2e68 746d 6c3a  management.html:
-00011070: 370a 6d73 6769 6420 2253 5250 204d 616e  7.msgid "SRP Man
-00011080: 6167 656d 656e 7422 0a6d 7367 7374 7220  agement".msgstr 
-00011090: 2222 0a0a 233a 2061 6c6c 6961 6e63 6561  ""..#: alliancea
-000110a0: 7574 682f 7372 702f 7465 6d70 6c61 7465  uth/srp/template
-000110b0: 732f 7372 702f 6d61 6e61 6765 6d65 6e74  s/srp/management
-000110c0: 2e68 746d 6c3a 3138 0a6d 7367 6964 2022  .html:18.msgid "
-000110d0: 5669 6577 2041 6c6c 220a 6d73 6773 7472  View All".msgstr
-000110e0: 2022 220a 0a23 3a20 616c 6c69 616e 6365   ""..#: alliance
-000110f0: 6175 7468 2f73 7270 2f74 656d 706c 6174  auth/srp/templat
-00011100: 6573 2f73 7270 2f6d 616e 6167 656d 656e  es/srp/managemen
-00011110: 742e 6874 6d6c 3a32 370a 6d73 6769 6420  t.html:27.msgid 
-00011120: 2241 6464 2053 5250 2046 6c65 6574 220a  "Add SRP Fleet".
-00011130: 6d73 6773 7472 2022 220a 0a23 3a20 616c  msgstr ""..#: al
-00011140: 6c69 616e 6365 6175 7468 2f73 7270 2f74  lianceauth/srp/t
-00011150: 656d 706c 6174 6573 2f73 7270 2f6d 616e  emplates/srp/man
-00011160: 6167 656d 656e 742e 6874 6d6c 3a34 380a  agement.html:48.
-00011170: 6d73 6769 6420 2246 6c65 6574 2041 4152  msgid "Fleet AAR
-00011180: 220a 6d73 6773 7472 2022 220a 0a23 3a20  ".msgstr ""..#: 
-00011190: 616c 6c69 616e 6365 6175 7468 2f73 7270  allianceauth/srp
-000111a0: 2f74 656d 706c 6174 6573 2f73 7270 2f6d  /templates/srp/m
-000111b0: 616e 6167 656d 656e 742e 6874 6d6c 3a34  anagement.html:4
-000111c0: 390a 6d73 6769 6420 2246 6c65 6574 2053  9.msgid "Fleet S
-000111d0: 5250 2043 6f64 6522 0a6d 7367 7374 7220  RP Code".msgstr 
-000111e0: 2222 0a0a 233a 2061 6c6c 6961 6e63 6561  ""..#: alliancea
-000111f0: 7574 682f 7372 702f 7465 6d70 6c61 7465  uth/srp/template
-00011200: 732f 7372 702f 6d61 6e61 6765 6d65 6e74  s/srp/management
-00011210: 2e68 746d 6c3a 3530 0a6d 7367 6964 2022  .html:50.msgid "
-00011220: 466c 6565 7420 4953 4b20 436f 7374 220a  Fleet ISK Cost".
-00011230: 6d73 6773 7472 2022 220a 0a23 3a20 616c  msgstr ""..#: al
-00011240: 6c69 616e 6365 6175 7468 2f73 7270 2f74  lianceauth/srp/t
-00011250: 656d 706c 6174 6573 2f73 7270 2f6d 616e  emplates/srp/man
-00011260: 6167 656d 656e 742e 6874 6d6c 3a35 310a  agement.html:51.
-00011270: 6d73 6769 6420 2253 5250 2053 7461 7475  msgid "SRP Statu
-00011280: 7322 0a6d 7367 7374 7220 2222 0a0a 233a  s".msgstr ""..#:
-00011290: 2061 6c6c 6961 6e63 6561 7574 682f 7372   allianceauth/sr
-000112a0: 702f 7465 6d70 6c61 7465 732f 7372 702f  p/templates/srp/
-000112b0: 6d61 6e61 6765 6d65 6e74 2e68 746d 6c3a  management.html:
-000112c0: 3532 0a6d 7367 6964 2022 5065 6e64 696e  52.msgid "Pendin
-000112d0: 6720 5265 7175 6573 7473 220a 6d73 6773  g Requests".msgs
-000112e0: 7472 2022 220a 0a23 3a20 616c 6c69 616e  tr ""..#: allian
-000112f0: 6365 6175 7468 2f73 7270 2f74 656d 706c  ceauth/srp/templ
-00011300: 6174 6573 2f73 7270 2f6d 616e 6167 656d  ates/srp/managem
-00011310: 656e 742e 6874 6d6c 3a39 310a 6d73 6769  ent.html:91.msgi
-00011320: 6420 2243 6f6d 706c 6574 6564 220a 6d73  d "Completed".ms
-00011330: 6773 7472 2022 220a 0a23 3a20 616c 6c69  gstr ""..#: alli
-00011340: 616e 6365 6175 7468 2f73 7270 2f74 656d  anceauth/srp/tem
-00011350: 706c 6174 6573 2f73 7270 2f6d 616e 6167  plates/srp/manag
-00011360: 656d 656e 742e 6874 6d6c 3a31 3038 0a6d  ement.html:108.m
-00011370: 7367 6964 2022 4172 6520 796f 7520 7375  sgid "Are you su
-00011380: 7265 2079 6f75 2077 616e 7420 746f 2064  re you want to d
-00011390: 656c 6574 6520 7468 6973 2053 5250 2063  elete this SRP c
-000113a0: 6f64 6520 616e 6420 6974 7320 636f 6e74  ode and its cont
-000113b0: 656e 7473 3f22 0a6d 7367 7374 7220 2222  ents?".msgstr ""
-000113c0: 0a0a 233a 2061 6c6c 6961 6e63 6561 7574  ..#: allianceaut
-000113d0: 682f 7372 702f 7465 6d70 6c61 7465 732f  h/srp/templates/
-000113e0: 7372 702f 6d61 6e61 6765 6d65 6e74 2e68  srp/management.h
-000113f0: 746d 6c3a 3132 390a 6d73 6769 6420 224e  tml:129.msgid "N
-00011400: 6f20 5352 5020 666c 6565 7473 2063 7265  o SRP fleets cre
-00011410: 6174 6564 2e22 0a6d 7367 7374 7220 2222  ated.".msgstr ""
-00011420: 0a0a 233a 2061 6c6c 6961 6e63 6561 7574  ..#: allianceaut
-00011430: 682f 7372 702f 7465 6d70 6c61 7465 732f  h/srp/templates/
-00011440: 7372 702f 7265 7175 6573 742e 6874 6d6c  srp/request.html
-00011450: 3a37 0a6d 7367 6964 2022 5352 5020 5265  :7.msgid "SRP Re
-00011460: 7175 6573 7422 0a6d 7367 7374 7220 2222  quest".msgstr ""
-00011470: 0a0a 233a 2061 6c6c 6961 6e63 6561 7574  ..#: allianceaut
-00011480: 682f 7372 702f 7465 6d70 6c61 7465 732f  h/srp/templates/
-00011490: 7372 702f 7265 7175 6573 742e 6874 6d6c  srp/request.html
-000114a0: 3a31 360a 6d73 6769 6420 2243 7265 6174  :16.msgid "Creat
-000114b0: 6520 5352 5020 5265 7175 6573 7422 0a6d  e SRP Request".m
-000114c0: 7367 7374 7220 2222 0a0a 233a 2061 6c6c  sgstr ""..#: all
-000114d0: 6961 6e63 6561 7574 682f 7372 702f 7465  ianceauth/srp/te
-000114e0: 6d70 6c61 7465 732f 7372 702f 7265 7175  mplates/srp/requ
-000114f0: 6573 742e 6874 6d6c 3a32 320a 6d73 6769  est.html:22.msgi
-00011500: 6420 2259 6f75 7220 5352 5020 7265 7175  d "Your SRP requ
-00011510: 6573 7422 0a6d 7367 7374 7220 2222 0a0a  est".msgstr ""..
-00011520: 233a 2061 6c6c 6961 6e63 6561 7574 682f  #: allianceauth/
-00011530: 7372 702f 7465 6d70 6c61 7465 732f 7372  srp/templates/sr
-00011540: 702f 7265 7175 6573 742e 6874 6d6c 3a33  p/request.html:3
-00011550: 350a 6d73 6769 6420 2243 7265 6174 6520  5.msgid "Create 
-00011560: 5352 5020 7265 7175 6573 7422 0a6d 7367  SRP request".msg
-00011570: 7374 7220 2222 0a0a 233a 2061 6c6c 6961  str ""..#: allia
-00011580: 6e63 6561 7574 682f 7372 702f 7465 6d70  nceauth/srp/temp
-00011590: 6c61 7465 732f 7372 702f 7570 6461 7465  lates/srp/update
-000115a0: 2e68 746d 6c3a 370a 233a 2061 6c6c 6961  .html:7.#: allia
-000115b0: 6e63 6561 7574 682f 7372 702f 7465 6d70  nceauth/srp/temp
-000115c0: 6c61 7465 732f 7372 702f 7570 6461 7465  lates/srp/update
-000115d0: 2e68 746d 6c3a 3136 0a6d 7367 6964 2022  .html:16.msgid "
-000115e0: 5570 6461 7465 2041 4152 204c 696e 6b22  Update AAR Link"
-000115f0: 0a6d 7367 7374 7220 2222 0a0a 233a 2061  .msgstr ""..#: a
-00011600: 6c6c 6961 6e63 6561 7574 682f 7372 702f  llianceauth/srp/
-00011610: 7465 6d70 6c61 7465 732f 7372 702f 7570  templates/srp/up
-00011620: 6461 7465 2e68 746d 6c3a 3232 0a6d 7367  date.html:22.msg
-00011630: 6964 2022 4166 7465 7220 4163 7469 6f6e  id "After Action
-00011640: 2052 6570 6f72 7422 0a6d 7367 7374 7220   Report".msgstr 
-00011650: 2222 0a0a 233a 2061 6c6c 6961 6e63 6561  ""..#: alliancea
-00011660: 7574 682f 7372 702f 7465 6d70 6c61 7465  uth/srp/template
-00011670: 732f 7372 702f 7570 6461 7465 2e68 746d  s/srp/update.htm
-00011680: 6c3a 3331 0a6d 7367 6964 2022 5352 5020  l:31.msgid "SRP 
-00011690: 466c 6565 7420 446f 6573 204e 6f74 2045  Fleet Does Not E
-000116a0: 7869 7374 220a 6d73 6773 7472 2022 220a  xist".msgstr "".
-000116b0: 0a23 3a20 616c 6c69 616e 6365 6175 7468  .#: allianceauth
-000116c0: 2f73 7270 2f74 656d 706c 6174 6573 2f73  /srp/templates/s
-000116d0: 7270 2f75 7064 6174 652e 6874 6d6c 3a34  rp/update.html:4
-000116e0: 300a 6d73 6769 6420 2255 7064 6174 6520  0.msgid "Update 
-000116f0: 4141 5220 6c69 6e6b 220a 6d73 6773 7472  AAR link".msgstr
-00011700: 2022 220a 0a23 3a20 616c 6c69 616e 6365   ""..#: alliance
-00011710: 6175 7468 2f73 7270 2f76 6965 7773 2e70  auth/srp/views.p
-00011720: 793a 3835 0a23 2c20 7079 7468 6f6e 2d66  y:85.#, python-f
-00011730: 6f72 6d61 740a 6d73 6769 6420 2243 7265  ormat.msgid "Cre
-00011740: 6174 6564 2053 5250 2066 6c65 6574 2025  ated SRP fleet %
-00011750: 2866 6c65 6574 6e61 6d65 2973 2e22 0a6d  (fleetname)s.".m
-00011760: 7367 7374 7220 2222 0a0a 233a 2061 6c6c  sgstr ""..#: all
-00011770: 6961 6e63 6561 7574 682f 7372 702f 7669  ianceauth/srp/vi
-00011780: 6577 732e 7079 3a31 3033 0a23 2c20 7079  ews.py:103.#, py
-00011790: 7468 6f6e 2d66 6f72 6d61 740a 6d73 6769  thon-format.msgi
-000117a0: 6420 2252 656d 6f76 6564 2053 5250 2066  d "Removed SRP f
-000117b0: 6c65 6574 2025 2866 6c65 6574 6e61 6d65  leet %(fleetname
-000117c0: 2973 2e22 0a6d 7367 7374 7220 2222 0a0a  )s.".msgstr ""..
-000117d0: 233a 2061 6c6c 6961 6e63 6561 7574 682f  #: allianceauth/
-000117e0: 7372 702f 7669 6577 732e 7079 3a31 3135  srp/views.py:115
-000117f0: 0a23 2c20 7079 7468 6f6e 2d66 6f72 6d61  .#, python-forma
-00011800: 740a 6d73 6769 6420 2244 6973 6162 6c65  t.msgid "Disable
-00011810: 6420 5352 5020 666c 6565 7420 2528 666c  d SRP fleet %(fl
-00011820: 6565 746e 616d 6529 732e 220a 6d73 6773  eetname)s.".msgs
-00011830: 7472 2022 220a 0a23 3a20 616c 6c69 616e  tr ""..#: allian
-00011840: 6365 6175 7468 2f73 7270 2f76 6965 7773  ceauth/srp/views
-00011850: 2e70 793a 3132 370a 232c 2070 7974 686f  .py:127.#, pytho
-00011860: 6e2d 666f 726d 6174 0a6d 7367 6964 2022  n-format.msgid "
-00011870: 456e 6162 6c65 6420 5352 5020 666c 6565  Enabled SRP flee
-00011880: 7420 2528 666c 6565 746e 616d 6529 732e  t %(fleetname)s.
-00011890: 220a 6d73 6773 7472 2022 220a 0a23 3a20  ".msgstr ""..#: 
-000118a0: 616c 6c69 616e 6365 6175 7468 2f73 7270  allianceauth/srp
-000118b0: 2f76 6965 7773 2e70 793a 3134 300a 232c  /views.py:140.#,
-000118c0: 2070 7974 686f 6e2d 666f 726d 6174 0a6d   python-format.m
-000118d0: 7367 6964 2022 4d61 726b 6564 2053 5250  sgid "Marked SRP
-000118e0: 2066 6c65 6574 2025 2866 6c65 6574 6e61   fleet %(fleetna
-000118f0: 6d65 2973 2061 7320 636f 6d70 6c65 7465  me)s as complete
-00011900: 642e 220a 6d73 6773 7472 2022 220a 0a23  d.".msgstr ""..#
-00011910: 3a20 616c 6c69 616e 6365 6175 7468 2f73  : allianceauth/s
-00011920: 7270 2f76 6965 7773 2e70 793a 3135 330a  rp/views.py:153.
-00011930: 232c 2070 7974 686f 6e2d 666f 726d 6174  #, python-format
-00011940: 0a6d 7367 6964 2022 4d61 726b 6564 2053  .msgid "Marked S
-00011950: 5250 2066 6c65 6574 2025 2866 6c65 6574  RP fleet %(fleet
-00011960: 6e61 6d65 2973 2061 7320 696e 636f 6d70  name)s as incomp
-00011970: 6c65 7465 2e22 0a6d 7367 7374 7220 2222  lete.".msgstr ""
-00011980: 0a0a 233a 2061 6c6c 6961 6e63 6561 7574  ..#: allianceaut
-00011990: 682f 7372 702f 7669 6577 732e 7079 3a31  h/srp/views.py:1
-000119a0: 3635 0a23 2c20 7079 7468 6f6e 2d66 6f72  65.#, python-for
-000119b0: 6d61 740a 6d73 6769 6420 2255 6e61 626c  mat.msgid "Unabl
-000119c0: 6520 746f 206c 6f63 6174 6520 5352 5020  e to locate SRP 
-000119d0: 636f 6465 2077 6974 6820 4944 2025 2873  code with ID %(s
-000119e0: 7270 666c 6565 7469 6429 7322 0a6d 7367  rpfleetid)s".msg
-000119f0: 7374 7220 2222 0a0a 233a 2061 6c6c 6961  str ""..#: allia
-00011a00: 6e63 6561 7574 682f 7372 702f 7669 6577  nceauth/srp/view
-00011a10: 732e 7079 3a31 3739 0a6d 7367 6964 2022  s.py:179.msgid "
-00011a20: 5468 6973 206b 696c 6c20 6d61 696c 2068  This kill mail h
-00011a30: 6173 2061 6c72 6561 6479 2062 6565 6e20  as already been 
-00011a40: 706f 7374 6564 2e22 0a6d 7367 7374 7220  posted.".msgstr 
-00011a50: 2222 0a0a 233a 2061 6c6c 6961 6e63 6561  ""..#: alliancea
-00011a60: 7574 682f 7372 702f 7669 6577 732e 7079  uth/srp/views.py
-00011a70: 3a32 3030 0a6d 7367 6964 2022 220a 2259  :200.msgid ""."Y
-00011a80: 6f75 7220 5352 5020 7265 7175 6573 7420  our SRP request 
-00011a90: 4b69 6c6c 6d61 696c 206c 696e 6b20 6973  Killmail link is
-00011aa0: 2069 6e76 616c 6964 2e20 506c 6561 7365   invalid. Please
-00011ab0: 206d 616b 6520 7375 7265 2079 6f75 2061   make sure you a
-00011ac0: 7265 2075 7369 6e67 2022 0a22 7a4b 696c  re using "."zKil
-00011ad0: 6c62 6f61 7264 2e22 0a6d 7367 7374 7220  lboard.".msgstr 
-00011ae0: 2222 0a0a 233a 2061 6c6c 6961 6e63 6561  ""..#: alliancea
-00011af0: 7574 682f 7372 702f 7669 6577 732e 7079  uth/srp/views.py
-00011b00: 3a32 3132 0a23 2c20 7079 7468 6f6e 2d66  :212.#, python-f
-00011b10: 6f72 6d61 740a 6d73 6769 6420 2253 7562  ormat.msgid "Sub
-00011b20: 6d69 7474 6564 2053 5250 2072 6571 7565  mitted SRP reque
-00011b30: 7374 2066 6f72 2079 6f75 7220 2528 7368  st for your %(sh
-00011b40: 6970 2973 2e22 0a6d 7367 7374 7220 2222  ip)s.".msgstr ""
-00011b50: 0a0a 233a 2061 6c6c 6961 6e63 6561 7574  ..#: allianceaut
-00011b60: 682f 7372 702f 7669 6577 732e 7079 3a32  h/srp/views.py:2
-00011b70: 3136 0a23 2c20 7079 7468 6f6e 2d66 6f72  16.#, python-for
-00011b80: 6d61 740a 6d73 6769 6420 2222 0a22 4368  mat.msgid ""."Ch
-00011b90: 6172 6163 7465 7220 2528 6368 6172 6964  aracter %(charid
-00011ba0: 2973 2064 6f65 7320 6e6f 7420 6265 6c6f  )s does not belo
-00011bb0: 6e67 2074 6f20 796f 7572 2041 7574 6820  ng to your Auth 
-00011bc0: 6163 636f 756e 742e 2050 6c65 6173 6520  account. Please 
-00011bd0: 6164 6420 7468 6520 220a 2241 5049 206b  add the "."API k
-00011be0: 6579 2066 6f72 2074 6869 7320 6368 6172  ey for this char
-00011bf0: 6163 7465 7220 616e 6420 7472 7920 6167  acter and try ag
-00011c00: 6169 6e22 0a6d 7367 7374 7220 2222 0a0a  ain".msgstr ""..
-00011c10: 233a 2061 6c6c 6961 6e63 6561 7574 682f  #: allianceauth/
-00011c20: 7372 702f 7669 6577 732e 7079 3a32 3336  srp/views.py:236
-00011c30: 2061 6c6c 6961 6e63 6561 7574 682f 7372   allianceauth/sr
-00011c40: 702f 7669 6577 732e 7079 3a32 3632 0a23  p/views.py:262.#
-00011c50: 3a20 616c 6c69 616e 6365 6175 7468 2f73  : allianceauth/s
-00011c60: 7270 2f76 6965 7773 2e70 793a 3330 300a  rp/views.py:300.
-00011c70: 6d73 6769 6420 224e 6f20 5352 5020 7265  msgid "No SRP re
-00011c80: 7175 6573 7473 2073 656c 6563 7465 6422  quests selected"
-00011c90: 0a6d 7367 7374 7220 2222 0a0a 233a 2061  .msgstr ""..#: a
-00011ca0: 6c6c 6961 6e63 6561 7574 682f 7372 702f  llianceauth/srp/
-00011cb0: 7669 6577 732e 7079 3a32 3437 2061 6c6c  views.py:247 all
-00011cc0: 6961 6e63 6561 7574 682f 7372 702f 7669  ianceauth/srp/vi
-00011cd0: 6577 732e 7079 3a32 3835 0a6d 7367 6964  ews.py:285.msgid
-00011ce0: 2022 556e 6162 6c65 2074 6f20 6c6f 6361   "Unable to loca
-00011cf0: 7465 2073 656c 6563 7465 6420 5352 5020  te selected SRP 
-00011d00: 7265 7175 6573 742e 220a 6d73 6773 7472  request.".msgstr
-00011d10: 2022 220a 0a23 3a20 616c 6c69 616e 6365   ""..#: alliance
-00011d20: 6175 7468 2f73 7270 2f76 6965 7773 2e70  auth/srp/views.p
-00011d30: 793a 3235 300a 232c 2070 7974 686f 6e2d  y:250.#, python-
-00011d40: 666f 726d 6174 0a6d 7367 6964 2022 4465  format.msgid "De
-00011d50: 6c65 7465 6420 2528 6e75 6d72 6571 7565  leted %(numreque
-00011d60: 7374 7329 7320 5352 5020 7265 7175 6573  sts)s SRP reques
-00011d70: 7473 220a 6d73 6773 7472 2022 220a 0a23  ts".msgstr ""..#
-00011d80: 3a20 616c 6c69 616e 6365 6175 7468 2f73  : allianceauth/s
-00011d90: 7270 2f76 6965 7773 2e70 793a 3238 380a  rp/views.py:288.
-00011da0: 232c 2070 7974 686f 6e2d 666f 726d 6174  #, python-format
-00011db0: 0a6d 7367 6964 2022 4170 7072 6f76 6564  .msgid "Approved
-00011dc0: 2025 286e 756d 7265 7175 6573 7473 2973   %(numrequests)s
-00011dd0: 2053 5250 2072 6571 7565 7374 7322 0a6d   SRP requests".m
-00011de0: 7367 7374 7220 2222 0a0a 233a 2061 6c6c  sgstr ""..#: all
-00011df0: 6961 6e63 6561 7574 682f 7372 702f 7669  ianceauth/srp/vi
-00011e00: 6577 732e 7079 3a33 3230 0a6d 7367 6964  ews.py:320.msgid
-00011e10: 2022 556e 6162 6c65 2074 6f20 6c6f 6361   "Unable to loca
-00011e20: 7465 2073 656c 6563 7465 6420 5352 5020  te selected SRP 
-00011e30: 7265 7175 6573 7422 0a6d 7367 7374 7220  request".msgstr 
-00011e40: 2222 0a0a 233a 2061 6c6c 6961 6e63 6561  ""..#: alliancea
-00011e50: 7574 682f 7372 702f 7669 6577 732e 7079  uth/srp/views.py
-00011e60: 3a33 3233 0a23 2c20 7079 7468 6f6e 2d66  :323.#, python-f
-00011e70: 6f72 6d61 740a 6d73 6769 6420 2252 656a  ormat.msgid "Rej
-00011e80: 6563 7465 6420 2528 6e75 6d72 6571 7565  ected %(numreque
-00011e90: 7374 7329 7320 5352 5020 7265 7175 6573  sts)s SRP reques
-00011ea0: 7473 2e22 0a6d 7367 7374 7220 2222 0a0a  ts.".msgstr ""..
-00011eb0: 233a 2061 6c6c 6961 6e63 6561 7574 682f  #: allianceauth/
-00011ec0: 7372 702f 7669 6577 732e 7079 3a33 3336  srp/views.py:336
-00011ed0: 0a23 2c20 7079 7468 6f6e 2d66 6f72 6d61  .#, python-forma
-00011ee0: 740a 6d73 6769 6420 2255 6e61 626c 6520  t.msgid "Unable 
-00011ef0: 746f 206c 6f63 6174 6520 5352 5020 7265  to locate SRP re
-00011f00: 7175 6573 7420 7769 7468 2049 4420 2528  quest with ID %(
-00011f10: 7265 7175 6573 7469 6429 7322 0a6d 7367  requestid)s".msg
-00011f20: 7374 7220 2222 0a0a 233a 2061 6c6c 6961  str ""..#: allia
-00011f30: 6e63 6561 7574 682f 7372 702f 7669 6577  nceauth/srp/view
-00011f40: 732e 7079 3a33 3630 0a23 2c20 7079 7468  s.py:360.#, pyth
-00011f50: 6f6e 2d66 6f72 6d61 740a 6d73 6769 6420  on-format.msgid 
-00011f60: 2253 6176 6564 2063 6861 6e67 6573 2074  "Saved changes t
-00011f70: 6f20 5352 5020 666c 6565 7420 2528 666c  o SRP fleet %(fl
-00011f80: 6565 746e 616d 6529 7322 0a6d 7367 7374  eetname)s".msgst
-00011f90: 7220 2222 0a0a 233a 2061 6c6c 6961 6e63  r ""..#: allianc
-00011fa0: 6561 7574 682f 7465 6d70 6c61 7465 732f  eauth/templates/
-00011fb0: 616c 6c69 616e 6365 6175 7468 2f61 646d  allianceauth/adm
-00011fc0: 696e 2d73 7461 7475 732f 6573 695f 6368  in-status/esi_ch
-00011fd0: 6563 6b2e 6874 6d6c 3a34 0a6d 7367 6964  eck.html:4.msgid
-00011fe0: 2022 596f 7572 2053 6572 7665 7220 7265   "Your Server re
-00011ff0: 6365 6976 6564 2061 6e20 4553 4920 6572  ceived an ESI er
-00012000: 726f 7220 7265 7370 6f6e 7365 2063 6f64  ror response cod
-00012010: 6520 6f66 2022 0a6d 7367 7374 7220 2222  e of ".msgstr ""
-00012020: 0a0a 233a 2061 6c6c 6961 6e63 6561 7574  ..#: allianceaut
-00012030: 682f 7465 6d70 6c61 7465 732f 616c 6c69  h/templates/alli
-00012040: 616e 6365 6175 7468 2f61 646d 696e 2d73  anceauth/admin-s
-00012050: 7461 7475 732f 6f76 6572 7669 6577 2e68  tatus/overview.h
-00012060: 746d 6c3a 3131 0a6d 7367 6964 2022 416c  tml:11.msgid "Al
-00012070: 6c69 616e 6365 2041 7574 6820 4e6f 7469  liance Auth Noti
-00012080: 6669 6361 7469 6f6e 7322 0a6d 7367 7374  fications".msgst
-00012090: 7220 2222 0a0a 233a 2061 6c6c 6961 6e63  r ""..#: allianc
-000120a0: 6561 7574 682f 7465 6d70 6c61 7465 732f  eauth/templates/
-000120b0: 616c 6c69 616e 6365 6175 7468 2f61 646d  allianceauth/adm
-000120c0: 696e 2d73 7461 7475 732f 6f76 6572 7669  in-status/overvi
-000120d0: 6577 2e68 746d 6c3a 3231 0a6d 7367 6964  ew.html:21.msgid
-000120e0: 2022 436c 6f73 6564 220a 6d73 6773 7472   "Closed".msgstr
-000120f0: 2022 220a 0a23 3a20 616c 6c69 616e 6365   ""..#: alliance
-00012100: 6175 7468 2f74 656d 706c 6174 6573 2f61  auth/templates/a
-00012110: 6c6c 6961 6e63 6561 7574 682f 6164 6d69  llianceauth/admi
-00012120: 6e2d 7374 6174 7573 2f6f 7665 7276 6965  n-status/overvie
-00012130: 772e 6874 6d6c 3a32 370a 6d73 6769 6420  w.html:27.msgid 
-00012140: 224e 6f20 6e6f 7469 6669 6361 7469 6f6e  "No notification
-00012150: 7320 6174 2074 6869 7320 7469 6d65 220a  s at this time".
-00012160: 6d73 6773 7472 2022 220a 0a23 3a20 616c  msgstr ""..#: al
-00012170: 6c69 616e 6365 6175 7468 2f74 656d 706c  lianceauth/templ
-00012180: 6174 6573 2f61 6c6c 6961 6e63 6561 7574  ates/allianceaut
-00012190: 682f 6164 6d69 6e2d 7374 6174 7573 2f6f  h/admin-status/o
-000121a0: 7665 7276 6965 772e 6874 6d6c 3a33 360a  verview.html:36.
-000121b0: 6d73 6769 6420 2250 6f77 6572 6564 2062  msgid "Powered b
-000121c0: 7920 4769 744c 6162 220a 6d73 6773 7472  y GitLab".msgstr
-000121d0: 2022 220a 0a23 3a20 616c 6c69 616e 6365   ""..#: alliance
-000121e0: 6175 7468 2f74 656d 706c 6174 6573 2f61  auth/templates/a
-000121f0: 6c6c 6961 6e63 6561 7574 682f 6164 6d69  llianceauth/admi
-00012200: 6e2d 7374 6174 7573 2f6f 7665 7276 6965  n-status/overvie
-00012210: 772e 6874 6d6c 3a34 320a 6d73 6769 6420  w.html:42.msgid 
-00012220: 2253 7570 706f 7274 2044 6973 636f 7264  "Support Discord
-00012230: 220a 6d73 6773 7472 2022 220a 0a23 3a20  ".msgstr ""..#: 
-00012240: 616c 6c69 616e 6365 6175 7468 2f74 656d  allianceauth/tem
-00012250: 706c 6174 6573 2f61 6c6c 6961 6e63 6561  plates/alliancea
-00012260: 7574 682f 6164 6d69 6e2d 7374 6174 7573  uth/admin-status
-00012270: 2f6f 7665 7276 6965 772e 6874 6d6c 3a35  /overview.html:5
-00012280: 390a 233a 2061 6c6c 6961 6e63 6561 7574  9.#: allianceaut
-00012290: 682f 7465 6d70 6c61 7465 732f 616c 6c69  h/templates/alli
-000122a0: 616e 6365 6175 7468 2f61 646d 696e 2d73  anceauth/admin-s
-000122b0: 7461 7475 732f 6f76 6572 7669 6577 2e68  tatus/overview.h
-000122c0: 746d 6c3a 3633 0a6d 7367 6964 2022 536f  tml:63.msgid "So
-000122d0: 6674 7761 7265 2056 6572 7369 6f6e 220a  ftware Version".
-000122e0: 6d73 6773 7472 2022 220a 0a23 3a20 616c  msgstr ""..#: al
-000122f0: 6c69 616e 6365 6175 7468 2f74 656d 706c  lianceauth/templ
-00012300: 6174 6573 2f61 6c6c 6961 6e63 6561 7574  ates/allianceaut
-00012310: 682f 6164 6d69 6e2d 7374 6174 7573 2f6f  h/admin-status/o
-00012320: 7665 7276 6965 772e 6874 6d6c 3a36 360a  verview.html:66.
-00012330: 6d73 6769 6420 2243 7572 7265 6e74 220a  msgid "Current".
-00012340: 6d73 6773 7472 2022 220a 0a23 3a20 616c  msgstr ""..#: al
-00012350: 6c69 616e 6365 6175 7468 2f74 656d 706c  lianceauth/templ
-00012360: 6174 6573 2f61 6c6c 6961 6e63 6561 7574  ates/allianceaut
-00012370: 682f 6164 6d69 6e2d 7374 6174 7573 2f6f  h/admin-status/o
-00012380: 7665 7276 6965 772e 6874 6d6c 3a37 330a  verview.html:73.
-00012390: 6d73 6769 6420 224c 6174 6573 7420 5374  msgid "Latest St
-000123a0: 6162 6c65 220a 6d73 6773 7472 2022 220a  able".msgstr "".
-000123b0: 0a23 3a20 616c 6c69 616e 6365 6175 7468  .#: allianceauth
-000123c0: 2f74 656d 706c 6174 6573 2f61 6c6c 6961  /templates/allia
-000123d0: 6e63 6561 7574 682f 6164 6d69 6e2d 7374  nceauth/admin-st
-000123e0: 6174 7573 2f6f 7665 7276 6965 772e 6874  atus/overview.ht
-000123f0: 6d6c 3a37 380a 6d73 6769 6420 2255 7064  ml:78.msgid "Upd
-00012400: 6174 6520 6176 6169 6c61 626c 6522 0a6d  ate available".m
-00012410: 7367 7374 7220 2222 0a0a 233a 2061 6c6c  sgstr ""..#: all
-00012420: 6961 6e63 6561 7574 682f 7465 6d70 6c61  ianceauth/templa
-00012430: 7465 732f 616c 6c69 616e 6365 6175 7468  tes/allianceauth
-00012440: 2f61 646d 696e 2d73 7461 7475 732f 6f76  /admin-status/ov
-00012450: 6572 7669 6577 2e68 746d 6c3a 3836 0a6d  erview.html:86.m
-00012460: 7367 6964 2022 4c61 7465 7374 2050 7265  sgid "Latest Pre
-00012470: 2d52 656c 6561 7365 220a 6d73 6773 7472  -Release".msgstr
-00012480: 2022 220a 0a23 3a20 616c 6c69 616e 6365   ""..#: alliance
-00012490: 6175 7468 2f74 656d 706c 6174 6573 2f61  auth/templates/a
-000124a0: 6c6c 6961 6e63 6561 7574 682f 6164 6d69  llianceauth/admi
-000124b0: 6e2d 7374 6174 7573 2f6f 7665 7276 6965  n-status/overvie
-000124c0: 772e 6874 6d6c 3a39 310a 6d73 6769 6420  w.html:91.msgid 
-000124d0: 2250 7265 2d52 656c 6561 7365 2061 7661  "Pre-Release ava
-000124e0: 696c 6162 6c65 220a 6d73 6773 7472 2022  ilable".msgstr "
-000124f0: 220a 0a23 3a20 616c 6c69 616e 6365 6175  "..#: allianceau
-00012500: 7468 2f74 656d 706c 6174 6573 2f61 6c6c  th/templates/all
-00012510: 6961 6e63 6561 7574 682f 6164 6d69 6e2d  ianceauth/admin-
-00012520: 7374 6174 7573 2f6f 7665 7276 6965 772e  status/overview.
-00012530: 6874 6d6c 3a31 3032 0a6d 7367 6964 2022  html:102.msgid "
-00012540: 5461 736b 2051 7565 7565 220a 6d73 6773  Task Queue".msgs
-00012550: 7472 2022 220a 0a23 3a20 616c 6c69 616e  tr ""..#: allian
-00012560: 6365 6175 7468 2f74 656d 706c 6174 6573  ceauth/templates
-00012570: 2f61 6c6c 6961 6e63 6561 7574 682f 6164  /allianceauth/ad
-00012580: 6d69 6e2d 7374 6174 7573 2f6f 7665 7276  min-status/overv
-00012590: 6965 772e 6874 6d6c 3a31 3037 0a23 2c20  iew.html:107.#, 
-000125a0: 7079 7468 6f6e 2d66 6f72 6d61 740a 6d73  python-format.ms
-000125b0: 6769 6420 2222 0a22 5c6e 220a 2220 2020  gid ""."\n"."   
-000125c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000125d0: 2020 2020 2020 2020 2053 7461 7475 7320           Status 
-000125e0: 6f66 2025 2874 6f74 616c 2973 2070 726f  of %(total)s pro
-000125f0: 6365 7373 6564 2074 6173 6b73 20e2 80a2  cessed tasks ...
-00012600: 206c 6173 7420 220a 2225 286c 6174 6573   last "."%(lates
-00012610: 7429 735c 6e22 0a22 2020 2020 2020 2020  t)s\n"."        
-00012620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012630: 220a 6d73 6773 7472 2022 220a 0a23 3a20  ".msgstr ""..#: 
-00012640: 616c 6c69 616e 6365 6175 7468 2f74 656d  allianceauth/tem
-00012650: 706c 6174 6573 2f61 6c6c 6961 6e63 6561  plates/alliancea
-00012660: 7574 682f 6164 6d69 6e2d 7374 6174 7573  uth/admin-status
-00012670: 2f6f 7665 7276 6965 772e 6874 6d6c 3a31  /overview.html:1
-00012680: 3233 0a6d 7367 6964 2022 7275 6e6e 696e  23.msgid "runnin
-00012690: 6722 0a6d 7367 7374 7220 2222 0a0a 233a  g".msgstr ""..#:
-000126a0: 2061 6c6c 6961 6e63 6561 7574 682f 7465   allianceauth/te
-000126b0: 6d70 6c61 7465 732f 616c 6c69 616e 6365  mplates/alliance
-000126c0: 6175 7468 2f61 646d 696e 2d73 7461 7475  auth/admin-statu
-000126d0: 732f 6f76 6572 7669 6577 2e68 746d 6c3a  s/overview.html:
-000126e0: 3132 340a 6d73 6769 6420 2271 7565 7565  124.msgid "queue
-000126f0: 6422 0a6d 7367 7374 7220 2222 0a0a 233a  d".msgstr ""..#:
-00012700: 2061 6c6c 6961 6e63 6561 7574 682f 7465   allianceauth/te
-00012710: 6d70 6c61 7465 732f 616c 6c69 616e 6365  mplates/alliance
-00012720: 6175 7468 2f74 6f70 2d6d 656e 752d 6164  auth/top-menu-ad
-00012730: 6d69 6e2e 6874 6d6c 3a31 390a 6d73 6769  min.html:19.msgi
-00012740: 6420 2241 4120 446f 6375 6d65 6e74 6174  d "AA Documentat
-00012750: 696f 6e22 0a6d 7367 7374 7220 2222 0a0a  ion".msgstr ""..
-00012760: 233a 2061 6c6c 6961 6e63 6561 7574 682f  #: allianceauth/
-00012770: 7465 6d70 6c61 7465 732f 616c 6c69 616e  templates/allian
-00012780: 6365 6175 7468 2f74 6f70 2d6d 656e 752d  ceauth/top-menu-
-00012790: 6164 6d69 6e2e 6874 6d6c 3a32 360a 6d73  admin.html:26.ms
-000127a0: 6769 6420 2241 4120 5375 7070 6f72 7420  gid "AA Support 
-000127b0: 4469 7363 6f72 6422 0a6d 7367 7374 7220  Discord".msgstr 
-000127c0: 2222 0a0a 233a 2061 6c6c 6961 6e63 6561  ""..#: alliancea
-000127d0: 7574 682f 7465 6d70 6c61 7465 732f 616c  uth/templates/al
-000127e0: 6c69 616e 6365 6175 7468 2f74 6f70 2d6d  lianceauth/top-m
-000127f0: 656e 752d 7573 6572 2d64 726f 7064 6f77  enu-user-dropdow
-00012800: 6e2e 6874 6d6c 3a31 300a 233a 2061 6c6c  n.html:10.#: all
-00012810: 6961 6e63 6561 7574 682f 7465 6d70 6c61  ianceauth/templa
-00012820: 7465 732f 616c 6c69 616e 6365 6175 7468  tes/allianceauth
-00012830: 2f74 6f70 2d6d 656e 752d 7573 6572 2d64  /top-menu-user-d
-00012840: 726f 7064 6f77 6e2e 6874 6d6c 3a31 360a  ropdown.html:16.
-00012850: 6d73 6769 6420 2255 7365 7220 4d65 6e75  msgid "User Menu
-00012860: 220a 6d73 6773 7472 2022 220a 0a23 3a20  ".msgstr ""..#: 
-00012870: 616c 6c69 616e 6365 6175 7468 2f74 656d  allianceauth/tem
-00012880: 706c 6174 6573 2f61 6c6c 6961 6e63 6561  plates/alliancea
-00012890: 7574 682f 746f 702d 6d65 6e75 2d75 7365  uth/top-menu-use
-000128a0: 722d 6472 6f70 646f 776e 2e68 746d 6c3a  r-dropdown.html:
-000128b0: 3637 0a6d 7367 6964 2022 4c6f 676f 7574  67.msgid "Logout
-000128c0: 220a 6d73 6773 7472 2022 220a 0a23 3a20  ".msgstr ""..#: 
-000128d0: 616c 6c69 616e 6365 6175 7468 2f74 656d  allianceauth/tem
-000128e0: 706c 6174 6573 2f61 6c6c 6961 6e63 6561  plates/alliancea
-000128f0: 7574 682f 746f 702d 6d65 6e75 2e68 746d  uth/top-menu.htm
-00012900: 6c3a 380a 6d73 6769 6420 2254 6f67 676c  l:8.msgid "Toggl
-00012910: 6520 6e61 7669 6761 7469 6f6e 220a 6d73  e navigation".ms
-00012920: 6773 7472 2022 220a 0a23 3a20 616c 6c69  gstr ""..#: alli
-00012930: 616e 6365 6175 7468 2f74 6865 6d65 2f74  anceauth/theme/t
-00012940: 656d 706c 6174 6573 2f74 6865 6d65 2f74  emplates/theme/t
-00012950: 6865 6d65 5f73 656c 6563 742e 6874 6d6c  heme_select.html
-00012960: 3a37 0a6d 7367 6964 2022 5365 6c65 6374  :7.msgid "Select
-00012970: 2054 6865 6d65 220a 6d73 6773 7472 2022   Theme".msgstr "
-00012980: 220a 0a23 3a20 616c 6c69 616e 6365 6175  "..#: allianceau
-00012990: 7468 2f74 696d 6572 626f 6172 642f 666f  th/timerboard/fo
-000129a0: 726d 2e70 793a 3533 0a23 3a20 616c 6c69  rm.py:53.#: alli
-000129b0: 616e 6365 6175 7468 2f74 696d 6572 626f  anceauth/timerbo
-000129c0: 6172 642f 7465 6d70 6c61 7465 732f 7469  ard/templates/ti
-000129d0: 6d65 7262 6f61 7264 2f74 696d 6572 7461  merboard/timerta
-000129e0: 626c 652e 6874 6d6c 3a31 3732 0a6d 7367  ble.html:172.msg
-000129f0: 6964 2022 4f74 6865 7222 0a6d 7367 7374  id "Other".msgst
-00012a00: 7220 2222 0a0a 233a 2061 6c6c 6961 6e63  r ""..#: allianc
-00012a10: 6561 7574 682f 7469 6d65 7262 6f61 7264  eauth/timerboard
-00012a20: 2f66 6f72 6d2e 7079 3a35 340a 233a 2061  /form.py:54.#: a
-00012a30: 6c6c 6961 6e63 6561 7574 682f 7469 6d65  llianceauth/time
-00012a40: 7262 6f61 7264 2f74 656d 706c 6174 6573  rboard/templates
-00012a50: 2f74 696d 6572 626f 6172 642f 6461 7368  /timerboard/dash
-00012a60: 626f 6172 642e 7469 6d65 7273 2e68 746d  board.timers.htm
-00012a70: 6c3a 3338 0a23 3a20 616c 6c69 616e 6365  l:38.#: alliance
-00012a80: 6175 7468 2f74 696d 6572 626f 6172 642f  auth/timerboard/
-00012a90: 7465 6d70 6c61 7465 732f 7469 6d65 7262  templates/timerb
-00012aa0: 6f61 7264 2f74 696d 6572 7461 626c 652e  oard/timertable.
-00012ab0: 6874 6d6c 3a34 340a 6d73 6769 6420 2246  html:44.msgid "F
-00012ac0: 7269 656e 646c 7922 0a6d 7367 7374 7220  riendly".msgstr 
-00012ad0: 2222 0a0a 233a 2061 6c6c 6961 6e63 6561  ""..#: alliancea
-00012ae0: 7574 682f 7469 6d65 7262 6f61 7264 2f66  uth/timerboard/f
-00012af0: 6f72 6d2e 7079 3a35 350a 233a 2061 6c6c  orm.py:55.#: all
-00012b00: 6961 6e63 6561 7574 682f 7469 6d65 7262  ianceauth/timerb
-00012b10: 6f61 7264 2f74 656d 706c 6174 6573 2f74  oard/templates/t
-00012b20: 696d 6572 626f 6172 642f 6461 7368 626f  imerboard/dashbo
-00012b30: 6172 642e 7469 6d65 7273 2e68 746d 6c3a  ard.timers.html:
-00012b40: 3333 0a23 3a20 616c 6c69 616e 6365 6175  33.#: allianceau
-00012b50: 7468 2f74 696d 6572 626f 6172 642f 7465  th/timerboard/te
-00012b60: 6d70 6c61 7465 732f 7469 6d65 7262 6f61  mplates/timerboa
-00012b70: 7264 2f74 696d 6572 7461 626c 652e 6874  rd/timertable.ht
-00012b80: 6d6c 3a33 380a 6d73 6769 6420 2248 6f73  ml:38.msgid "Hos
-00012b90: 7469 6c65 220a 6d73 6773 7472 2022 220a  tile".msgstr "".
-00012ba0: 0a23 3a20 616c 6c69 616e 6365 6175 7468  .#: allianceauth
-00012bb0: 2f74 696d 6572 626f 6172 642f 666f 726d  /timerboard/form
-00012bc0: 2e70 793a 3536 0a23 3a20 616c 6c69 616e  .py:56.#: allian
-00012bd0: 6365 6175 7468 2f74 696d 6572 626f 6172  ceauth/timerboar
-00012be0: 642f 7465 6d70 6c61 7465 732f 7469 6d65  d/templates/time
-00012bf0: 7262 6f61 7264 2f64 6173 6862 6f61 7264  rboard/dashboard
-00012c00: 2e74 696d 6572 732e 6874 6d6c 3a34 330a  .timers.html:43.
-00012c10: 233a 2061 6c6c 6961 6e63 6561 7574 682f  #: allianceauth/
-00012c20: 7469 6d65 7262 6f61 7264 2f74 656d 706c  timerboard/templ
-00012c30: 6174 6573 2f74 696d 6572 626f 6172 642f  ates/timerboard/
-00012c40: 7469 6d65 7274 6162 6c65 2e68 746d 6c3a  timertable.html:
-00012c50: 3530 0a6d 7367 6964 2022 4e65 7574 7261  50.msgid "Neutra
-00012c60: 6c22 0a6d 7367 7374 7220 2222 0a0a 233a  l".msgstr ""..#:
-00012c70: 2061 6c6c 6961 6e63 6561 7574 682f 7469   allianceauth/ti
-00012c80: 6d65 7262 6f61 7264 2f66 6f72 6d2e 7079  merboard/form.py
-00012c90: 3a35 380a 233a 2061 6c6c 6961 6e63 6561  :58.#: alliancea
-00012ca0: 7574 682f 7469 6d65 7262 6f61 7264 2f74  uth/timerboard/t
-00012cb0: 656d 706c 6174 6573 2f74 696d 6572 626f  emplates/timerbo
-00012cc0: 6172 642f 6461 7368 626f 6172 642e 7469  ard/dashboard.ti
-00012cd0: 6d65 7273 2e68 746d 6c3a 3133 0a23 3a20  mers.html:13.#: 
-00012ce0: 616c 6c69 616e 6365 6175 7468 2f74 696d  allianceauth/tim
-00012cf0: 6572 626f 6172 642f 7465 6d70 6c61 7465  erboard/template
-00012d00: 732f 7469 6d65 7262 6f61 7264 2f74 696d  s/timerboard/tim
-00012d10: 6572 7461 626c 652e 6874 6d6c 3a37 0a6d  ertable.html:7.m
-00012d20: 7367 6964 2022 4465 7461 696c 7322 0a6d  sgid "Details".m
-00012d30: 7367 7374 7220 2222 0a0a 233a 2061 6c6c  sgstr ""..#: all
-00012d40: 6961 6e63 6561 7574 682f 7469 6d65 7262  ianceauth/timerb
-00012d50: 6f61 7264 2f66 6f72 6d2e 7079 3a36 300a  oard/form.py:60.
-00012d60: 6d73 6769 6420 2250 6c61 6e65 742f 4d6f  msgid "Planet/Mo
-00012d70: 6f6e 220a 6d73 6773 7472 2022 220a 0a23  on".msgstr ""..#
-00012d80: 3a20 616c 6c69 616e 6365 6175 7468 2f74  : allianceauth/t
-00012d90: 696d 6572 626f 6172 642f 666f 726d 2e70  imerboard/form.p
-00012da0: 793a 3631 0a6d 7367 6964 2022 5374 7275  y:61.msgid "Stru
-00012db0: 6374 7572 6520 5479 7065 220a 6d73 6773  cture Type".msgs
-00012dc0: 7472 2022 220a 0a23 3a20 616c 6c69 616e  tr ""..#: allian
-00012dd0: 6365 6175 7468 2f74 696d 6572 626f 6172  ceauth/timerboar
-00012de0: 642f 666f 726d 2e70 793a 3632 0a6d 7367  d/form.py:62.msg
-00012df0: 6964 2022 5469 6d65 7220 5479 7065 220a  id "Timer Type".
-00012e00: 6d73 6773 7472 2022 220a 0a23 3a20 616c  msgstr ""..#: al
-00012e10: 6c69 616e 6365 6175 7468 2f74 696d 6572  lianceauth/timer
-00012e20: 626f 6172 642f 666f 726d 2e70 793a 3633  board/form.py:63
-00012e30: 0a23 3a20 616c 6c69 616e 6365 6175 7468  .#: allianceauth
-00012e40: 2f74 696d 6572 626f 6172 642f 7465 6d70  /timerboard/temp
-00012e50: 6c61 7465 732f 7469 6d65 7262 6f61 7264  lates/timerboard
-00012e60: 2f74 696d 6572 7461 626c 652e 6874 6d6c  /timertable.html
-00012e70: 3a38 0a6d 7367 6964 2022 4f62 6a65 6374  :8.msgid "Object
-00012e80: 6976 6522 0a6d 7367 7374 7220 2222 0a0a  ive".msgstr ""..
-00012e90: 233a 2061 6c6c 6961 6e63 6561 7574 682f  #: allianceauth/
-00012ea0: 7469 6d65 7262 6f61 7264 2f66 6f72 6d2e  timerboard/form.
-00012eb0: 7079 3a36 340a 6d73 6769 6420 2241 6273  py:64.msgid "Abs
-00012ec0: 6f6c 7574 6520 5469 6d65 7222 0a6d 7367  olute Timer".msg
-00012ed0: 7374 7220 2222 0a0a 233a 2061 6c6c 6961  str ""..#: allia
-00012ee0: 6e63 6561 7574 682f 7469 6d65 7262 6f61  nceauth/timerboa
-00012ef0: 7264 2f66 6f72 6d2e 7079 3a36 350a 6d73  rd/form.py:65.ms
-00012f00: 6769 6420 2244 6174 6520 616e 6420 5469  gid "Date and Ti
-00012f10: 6d65 220a 6d73 6773 7472 2022 220a 0a23  me".msgstr ""..#
-00012f20: 3a20 616c 6c69 616e 6365 6175 7468 2f74  : allianceauth/t
-00012f30: 696d 6572 626f 6172 642f 666f 726d 2e70  imerboard/form.p
-00012f40: 793a 3636 0a6d 7367 6964 2022 4461 7973  y:66.msgid "Days
-00012f50: 2052 656d 6169 6e69 6e67 220a 6d73 6773   Remaining".msgs
-00012f60: 7472 2022 220a 0a23 3a20 616c 6c69 616e  tr ""..#: allian
-00012f70: 6365 6175 7468 2f74 696d 6572 626f 6172  ceauth/timerboar
-00012f80: 642f 666f 726d 2e70 793a 3637 0a6d 7367  d/form.py:67.msg
-00012f90: 6964 2022 486f 7572 7320 5265 6d61 696e  id "Hours Remain
-00012fa0: 696e 6722 0a6d 7367 7374 7220 2222 0a0a  ing".msgstr ""..
-00012fb0: 233a 2061 6c6c 6961 6e63 6561 7574 682f  #: allianceauth/
-00012fc0: 7469 6d65 7262 6f61 7264 2f66 6f72 6d2e  timerboard/form.
-00012fd0: 7079 3a36 390a 6d73 6769 6420 224d 696e  py:69.msgid "Min
-00012fe0: 7574 6573 2052 656d 6169 6e69 6e67 220a  utes Remaining".
-00012ff0: 6d73 6773 7472 2022 220a 0a23 3a20 616c  msgstr ""..#: al
-00013000: 6c69 616e 6365 6175 7468 2f74 696d 6572  lianceauth/timer
-00013010: 626f 6172 642f 666f 726d 2e70 793a 3731  board/form.py:71
-00013020: 0a6d 7367 6964 2022 496d 706f 7274 616e  .msgid "Importan
-00013030: 7422 0a6d 7367 7374 7220 2222 0a0a 233a  t".msgstr ""..#:
-00013040: 2061 6c6c 6961 6e63 6561 7574 682f 7469   allianceauth/ti
-00013050: 6d65 7262 6f61 7264 2f66 6f72 6d2e 7079  merboard/form.py
-00013060: 3a37 320a 6d73 6769 6420 2243 6f72 702d  :72.msgid "Corp-
-00013070: 5265 7374 7269 6374 6564 220a 6d73 6773  Restricted".msgs
-00013080: 7472 2022 220a 0a23 3a20 616c 6c69 616e  tr ""..#: allian
-00013090: 6365 6175 7468 2f74 696d 6572 626f 6172  ceauth/timerboar
-000130a0: 642f 6d6f 6465 6c73 2e70 793a 3134 0a6d  d/models.py:14.m
-000130b0: 7367 6964 2022 4e6f 7420 5370 6563 6966  sgid "Not Specif
-000130c0: 6965 6422 0a6d 7367 7374 7220 2222 0a0a  ied".msgstr ""..
-000130d0: 233a 2061 6c6c 6961 6e63 6561 7574 682f  #: allianceauth/
-000130e0: 7469 6d65 7262 6f61 7264 2f6d 6f64 656c  timerboard/model
-000130f0: 732e 7079 3a31 350a 6d73 6769 6420 2253  s.py:15.msgid "S
-00013100: 6869 656c 6422 0a6d 7367 7374 7220 2222  hield".msgstr ""
-00013110: 0a0a 233a 2061 6c6c 6961 6e63 6561 7574  ..#: allianceaut
-00013120: 682f 7469 6d65 7262 6f61 7264 2f6d 6f64  h/timerboard/mod
-00013130: 656c 732e 7079 3a31 360a 6d73 6769 6420  els.py:16.msgid 
-00013140: 2241 726d 6f72 220a 6d73 6773 7472 2022  "Armor".msgstr "
-00013150: 220a 0a23 3a20 616c 6c69 616e 6365 6175  "..#: allianceau
-00013160: 7468 2f74 696d 6572 626f 6172 642f 6d6f  th/timerboard/mo
-00013170: 6465 6c73 2e70 793a 3137 0a6d 7367 6964  dels.py:17.msgid
-00013180: 2022 4875 6c6c 220a 6d73 6773 7472 2022   "Hull".msgstr "
-00013190: 220a 0a23 3a20 616c 6c69 616e 6365 6175  "..#: allianceau
-000131a0: 7468 2f74 696d 6572 626f 6172 642f 6d6f  th/timerboard/mo
-000131b0: 6465 6c73 2e70 793a 3138 0a6d 7367 6964  dels.py:18.msgid
-000131c0: 2022 4669 6e61 6c22 0a6d 7367 7374 7220   "Final".msgstr 
-000131d0: 2222 0a0a 233a 2061 6c6c 6961 6e63 6561  ""..#: alliancea
-000131e0: 7574 682f 7469 6d65 7262 6f61 7264 2f6d  uth/timerboard/m
-000131f0: 6f64 656c 732e 7079 3a31 390a 6d73 6769  odels.py:19.msgi
-00013200: 6420 2241 6e63 686f 7269 6e67 220a 6d73  d "Anchoring".ms
+0000d2a0: 732f 6162 7374 7261 6374 2e70 793a 3130  s/abstract.py:10
+0000d2b0: 330a 232c 2070 7974 686f 6e2d 6272 6163  3.#, python-brac
+0000d2c0: 652d 666f 726d 6174 0a6d 7367 6964 2022  e-format.msgid "
+0000d2d0: 5375 6363 6573 7366 756c 6c79 2073 6574  Successfully set
+0000d2e0: 2079 6f75 7220 7b73 656c 662e 7365 7276   your {self.serv
+0000d2f0: 6963 655f 6e61 6d65 7d20 7061 7373 776f  ice_name} passwo
+0000d300: 7264 220a 6d73 6773 7472 2022 220a 0a23  rd".msgstr ""..#
+0000d310: 3a20 616c 6c69 616e 6365 6175 7468 2f73  : allianceauth/s
+0000d320: 6572 7669 6365 732f 6175 7468 5f68 6f6f  ervices/auth_hoo
+0000d330: 6b73 2e70 793a 3132 0a6d 7367 6964 2022  ks.py:12.msgid "
+0000d340: 5365 7276 6963 6573 220a 6d73 6773 7472  Services".msgstr
+0000d350: 2022 220a 0a23 3a20 616c 6c69 616e 6365   ""..#: alliance
+0000d360: 6175 7468 2f73 6572 7669 6365 732f 666f  auth/services/fo
+0000d370: 726d 732e 7079 3a36 0a6d 7367 6964 2022  rms.py:6.msgid "
+0000d380: 4e61 6d65 206f 6620 466c 6565 743a 220a  Name of Fleet:".
+0000d390: 6d73 6773 7472 2022 220a 0a23 3a20 616c  msgstr ""..#: al
+0000d3a0: 6c69 616e 6365 6175 7468 2f73 6572 7669  lianceauth/servi
+0000d3b0: 6365 732f 666f 726d 732e 7079 3a37 0a6d  ces/forms.py:7.m
+0000d3c0: 7367 6964 2022 466c 6565 7420 436f 6d6d  sgid "Fleet Comm
+0000d3d0: 616e 6465 723a 220a 6d73 6773 7472 2022  ander:".msgstr "
+0000d3e0: 220a 0a23 3a20 616c 6c69 616e 6365 6175  "..#: allianceau
+0000d3f0: 7468 2f73 6572 7669 6365 732f 666f 726d  th/services/form
+0000d400: 732e 7079 3a38 0a6d 7367 6964 2022 466c  s.py:8.msgid "Fl
+0000d410: 6565 7420 436f 6d6d 733a 220a 6d73 6773  eet Comms:".msgs
+0000d420: 7472 2022 220a 0a23 3a20 616c 6c69 616e  tr ""..#: allian
+0000d430: 6365 6175 7468 2f73 6572 7669 6365 732f  ceauth/services/
+0000d440: 666f 726d 732e 7079 3a39 0a6d 7367 6964  forms.py:9.msgid
+0000d450: 2022 466c 6565 7420 5479 7065 3a22 0a6d   "Fleet Type:".m
+0000d460: 7367 7374 7220 2222 0a0a 233a 2061 6c6c  sgstr ""..#: all
+0000d470: 6961 6e63 6561 7574 682f 7365 7276 6963  ianceauth/servic
+0000d480: 6573 2f66 6f72 6d73 2e70 793a 3130 0a6d  es/forms.py:10.m
+0000d490: 7367 6964 2022 5368 6970 2050 7269 6f72  sgid "Ship Prior
+0000d4a0: 6974 6965 733a 220a 6d73 6773 7472 2022  ities:".msgstr "
+0000d4b0: 220a 0a23 3a20 616c 6c69 616e 6365 6175  "..#: allianceau
+0000d4c0: 7468 2f73 6572 7669 6365 732f 666f 726d  th/services/form
+0000d4d0: 732e 7079 3a31 310a 6d73 6769 6420 2246  s.py:11.msgid "F
+0000d4e0: 6f72 6d75 7020 4c6f 6361 7469 6f6e 3a22  ormup Location:"
+0000d4f0: 0a6d 7367 7374 7220 2222 0a0a 233a 2061  .msgstr ""..#: a
+0000d500: 6c6c 6961 6e63 6561 7574 682f 7365 7276  llianceauth/serv
+0000d510: 6963 6573 2f66 6f72 6d73 2e70 793a 3132  ices/forms.py:12
+0000d520: 0a6d 7367 6964 2022 466f 726d 7570 2054  .msgid "Formup T
+0000d530: 696d 653a 220a 6d73 6773 7472 2022 220a  ime:".msgstr "".
+0000d540: 0a23 3a20 616c 6c69 616e 6365 6175 7468  .#: allianceauth
+0000d550: 2f73 6572 7669 6365 732f 666f 726d 732e  /services/forms.
+0000d560: 7079 3a31 330a 6d73 6769 6420 2245 7870  py:13.msgid "Exp
+0000d570: 6563 7465 6420 4475 7261 7469 6f6e 3a22  ected Duration:"
+0000d580: 0a6d 7367 7374 7220 2222 0a0a 233a 2061  .msgstr ""..#: a
+0000d590: 6c6c 6961 6e63 6561 7574 682f 7365 7276  llianceauth/serv
+0000d5a0: 6963 6573 2f66 6f72 6d73 2e70 793a 3134  ices/forms.py:14
+0000d5b0: 0a6d 7367 6964 2022 5075 7270 6f73 653a  .msgid "Purpose:
+0000d5c0: 220a 6d73 6773 7472 2022 220a 0a23 3a20  ".msgstr ""..#: 
+0000d5d0: 616c 6c69 616e 6365 6175 7468 2f73 6572  allianceauth/ser
+0000d5e0: 7669 6365 732f 666f 726d 732e 7079 3a31  vices/forms.py:1
+0000d5f0: 350a 6d73 6769 6420 2252 6569 6d62 7572  5.msgid "Reimbur
+0000d600: 7361 626c 653f 2a22 0a6d 7367 7374 7220  sable?*".msgstr 
+0000d610: 2222 0a0a 233a 2061 6c6c 6961 6e63 6561  ""..#: alliancea
+0000d620: 7574 682f 7365 7276 6963 6573 2f66 6f72  uth/services/for
+0000d630: 6d73 2e70 793a 3135 2061 6c6c 6961 6e63  ms.py:15 allianc
+0000d640: 6561 7574 682f 7365 7276 6963 6573 2f66  eauth/services/f
+0000d650: 6f72 6d73 2e70 793a 3136 0a6d 7367 6964  orms.py:16.msgid
+0000d660: 2022 5965 7322 0a6d 7367 7374 7220 2222   "Yes".msgstr ""
+0000d670: 0a0a 233a 2061 6c6c 6961 6e63 6561 7574  ..#: allianceaut
+0000d680: 682f 7365 7276 6963 6573 2f66 6f72 6d73  h/services/forms
+0000d690: 2e70 793a 3135 2061 6c6c 6961 6e63 6561  .py:15 alliancea
+0000d6a0: 7574 682f 7365 7276 6963 6573 2f66 6f72  uth/services/for
+0000d6b0: 6d73 2e70 793a 3136 0a6d 7367 6964 2022  ms.py:16.msgid "
+0000d6c0: 4e6f 220a 6d73 6773 7472 2022 220a 0a23  No".msgstr ""..#
+0000d6d0: 3a20 616c 6c69 616e 6365 6175 7468 2f73  : allianceauth/s
+0000d6e0: 6572 7669 6365 732f 666f 726d 732e 7079  ervices/forms.py
+0000d6f0: 3a31 360a 6d73 6769 6420 2249 6d70 6f72  :16.msgid "Impor
+0000d700: 7461 6e74 3f2a 220a 6d73 6773 7472 2022  tant?*".msgstr "
+0000d710: 220a 0a23 3a20 616c 6c69 616e 6365 6175  "..#: allianceau
+0000d720: 7468 2f73 6572 7669 6365 732f 666f 726d  th/services/form
+0000d730: 732e 7079 3a32 3120 616c 6c69 616e 6365  s.py:21 alliance
+0000d740: 6175 7468 2f73 6572 7669 6365 732f 666f  auth/services/fo
+0000d750: 726d 732e 7079 3a33 310a 6d73 6769 6420  rms.py:31.msgid 
+0000d760: 2250 6173 7377 6f72 6422 0a6d 7367 7374  "Password".msgst
+0000d770: 7220 2222 0a0a 233a 2061 6c6c 6961 6e63  r ""..#: allianc
+0000d780: 6561 7574 682f 7365 7276 6963 6573 2f66  eauth/services/f
+0000d790: 6f72 6d73 2e70 793a 3236 2061 6c6c 6961  orms.py:26 allia
+0000d7a0: 6e63 6561 7574 682f 7365 7276 6963 6573  nceauth/services
+0000d7b0: 2f66 6f72 6d73 2e70 793a 3336 0a6d 7367  /forms.py:36.msg
+0000d7c0: 6964 2022 5061 7373 776f 7264 206d 7573  id "Password mus
+0000d7d0: 7420 6265 2061 7420 6c65 6173 7420 3820  t be at least 8 
+0000d7e0: 6368 6172 6163 7465 7273 206c 6f6e 672e  characters long.
+0000d7f0: 220a 6d73 6773 7472 2022 220a 0a23 3a20  ".msgstr ""..#: 
+0000d800: 616c 6c69 616e 6365 6175 7468 2f73 6572  allianceauth/ser
+0000d810: 7669 6365 732f 6d6f 6475 6c65 732f 6469  vices/modules/di
+0000d820: 7363 6f72 642f 6d6f 6465 6c73 2e70 793a  scord/models.py:
+0000d830: 3138 370a 6d73 6769 6420 2244 6973 636f  187.msgid "Disco
+0000d840: 7264 2041 6363 6f75 6e74 2044 6973 6162  rd Account Disab
+0000d850: 6c65 6422 0a6d 7367 7374 7220 2222 0a0a  led".msgstr ""..
+0000d860: 233a 2061 6c6c 6961 6e63 6561 7574 682f  #: allianceauth/
+0000d870: 7365 7276 6963 6573 2f6d 6f64 756c 6573  services/modules
+0000d880: 2f64 6973 636f 7264 2f6d 6f64 656c 732e  /discord/models.
+0000d890: 7079 3a31 3839 0a6d 7367 6964 2022 220a  py:189.msgid "".
+0000d8a0: 2259 6f75 7220 4469 7363 6f72 6420 6163  "Your Discord ac
+0000d8b0: 636f 756e 7420 7761 7320 6469 7361 626c  count was disabl
+0000d8c0: 6564 2061 7574 6f6d 6174 6963 616c 6c79  ed automatically
+0000d8d0: 2062 7920 4175 7468 2e20 4966 2079 6f75   by Auth. If you
+0000d8e0: 2074 6869 6e6b 2074 6869 7320 220a 2277   think this "."w
+0000d8f0: 6173 2061 206d 6973 7461 6b65 2c20 706c  as a mistake, pl
+0000d900: 6561 7365 2063 6f6e 7461 6374 2061 6e20  ease contact an 
+0000d910: 6164 6d69 6e2e 220a 6d73 6773 7472 2022  admin.".msgstr "
+0000d920: 220a 0a23 3a20 616c 6c69 616e 6365 6175  "..#: allianceau
+0000d930: 7468 2f73 6572 7669 6365 732f 6d6f 6475  th/services/modu
+0000d940: 6c65 732f 6469 7363 6f72 642f 7465 6d70  les/discord/temp
+0000d950: 6c61 7465 732f 7365 7276 6963 6573 2f64  lates/services/d
+0000d960: 6973 636f 7264 2f64 6973 636f 7264 5f73  iscord/discord_s
+0000d970: 6572 7669 6365 5f63 7472 6c2e 6874 6d6c  ervice_ctrl.html
+0000d980: 3a32 360a 233a 2061 6c6c 6961 6e63 6561  :26.#: alliancea
+0000d990: 7574 682f 7365 7276 6963 6573 2f6d 6f64  uth/services/mod
+0000d9a0: 756c 6573 2f6d 756d 626c 652f 7465 6d70  ules/mumble/temp
+0000d9b0: 6c61 7465 732f 7365 7276 6963 6573 2f6d  lates/services/m
+0000d9c0: 756d 626c 652f 6d75 6d62 6c65 5f73 6572  umble/mumble_ser
+0000d9d0: 7669 6365 5f63 7472 6c2e 6874 6d6c 3a32  vice_ctrl.html:2
+0000d9e0: 300a 6d73 6769 6420 2241 6374 6976 6174  0.msgid "Activat
+0000d9f0: 6522 0a6d 7367 7374 7220 2222 0a0a 233a  e".msgstr ""..#:
+0000da00: 2061 6c6c 6961 6e63 6561 7574 682f 7365   allianceauth/se
+0000da10: 7276 6963 6573 2f6d 6f64 756c 6573 2f64  rvices/modules/d
+0000da20: 6973 636f 7264 2f74 656d 706c 6174 6573  iscord/templates
+0000da30: 2f73 6572 7669 6365 732f 6469 7363 6f72  /services/discor
+0000da40: 642f 6469 7363 6f72 645f 7365 7276 6963  d/discord_servic
+0000da50: 655f 6374 726c 2e68 746d 6c3a 3332 0a23  e_ctrl.html:32.#
+0000da60: 3a20 616c 6c69 616e 6365 6175 7468 2f73  : allianceauth/s
+0000da70: 6572 7669 6365 732f 6d6f 6475 6c65 732f  ervices/modules/
+0000da80: 6d75 6d62 6c65 2f74 656d 706c 6174 6573  mumble/templates
+0000da90: 2f73 6572 7669 6365 732f 6d75 6d62 6c65  /services/mumble
+0000daa0: 2f6d 756d 626c 655f 7365 7276 6963 655f  /mumble_service_
+0000dab0: 6374 726c 2e68 746d 6c3a 3332 0a6d 7367  ctrl.html:32.msg
+0000dac0: 6964 2022 5265 7365 7420 5061 7373 776f  id "Reset Passwo
+0000dad0: 7264 220a 6d73 6773 7472 2022 220a 0a23  rd".msgstr ""..#
+0000dae0: 3a20 616c 6c69 616e 6365 6175 7468 2f73  : allianceauth/s
+0000daf0: 6572 7669 6365 732f 6d6f 6475 6c65 732f  ervices/modules/
+0000db00: 6469 7363 6f72 642f 7465 6d70 6c61 7465  discord/template
+0000db10: 732f 7365 7276 6963 6573 2f64 6973 636f  s/services/disco
+0000db20: 7264 2f64 6973 636f 7264 5f73 6572 7669  rd/discord_servi
+0000db30: 6365 5f63 7472 6c2e 6874 6d6c 3a33 380a  ce_ctrl.html:38.
+0000db40: 233a 2061 6c6c 6961 6e63 6561 7574 682f  #: allianceauth/
+0000db50: 7365 7276 6963 6573 2f6d 6f64 756c 6573  services/modules
+0000db60: 2f6d 756d 626c 652f 7465 6d70 6c61 7465  /mumble/template
+0000db70: 732f 7365 7276 6963 6573 2f6d 756d 626c  s/services/mumbl
+0000db80: 652f 6d75 6d62 6c65 5f73 6572 7669 6365  e/mumble_service
+0000db90: 5f63 7472 6c2e 6874 6d6c 3a33 380a 6d73  _ctrl.html:38.ms
+0000dba0: 6769 6420 2244 6561 6374 6976 6174 6522  gid "Deactivate"
+0000dbb0: 0a6d 7367 7374 7220 2222 0a0a 233a 2061  .msgstr ""..#: a
+0000dbc0: 6c6c 6961 6e63 6561 7574 682f 7365 7276  llianceauth/serv
+0000dbd0: 6963 6573 2f6d 6f64 756c 6573 2f64 6973  ices/modules/dis
+0000dbe0: 636f 7264 2f74 656d 706c 6174 6573 2f73  cord/templates/s
+0000dbf0: 6572 7669 6365 732f 6469 7363 6f72 642f  ervices/discord/
+0000dc00: 6469 7363 6f72 645f 7365 7276 6963 655f  discord_service_
+0000dc10: 6374 726c 2e68 746d 6c3a 3435 0a6d 7367  ctrl.html:45.msg
+0000dc20: 6964 2022 4c69 6e6b 2044 6973 636f 7264  id "Link Discord
+0000dc30: 2053 6572 7665 7222 0a6d 7367 7374 7220   Server".msgstr 
+0000dc40: 2222 0a0a 233a 2061 6c6c 6961 6e63 6561  ""..#: alliancea
+0000dc50: 7574 682f 7365 7276 6963 6573 2f6d 6f64  uth/services/mod
+0000dc60: 756c 6573 2f64 6973 636f 7264 2f76 6965  ules/discord/vie
+0000dc70: 7773 2e70 793a 3330 0a6d 7367 6964 2022  ws.py:30.msgid "
+0000dc80: 4465 6163 7469 7661 7465 6420 4469 7363  Deactivated Disc
+0000dc90: 6f72 6420 6163 636f 756e 742e 220a 6d73  ord account.".ms
+0000dca0: 6773 7472 2022 220a 0a23 3a20 616c 6c69  gstr ""..#: alli
+0000dcb0: 616e 6365 6175 7468 2f73 6572 7669 6365  anceauth/service
+0000dcc0: 732f 6d6f 6475 6c65 732f 6469 7363 6f72  s/modules/discor
+0000dcd0: 642f 7669 6577 732e 7079 3a33 360a 233a  d/views.py:36.#:
+0000dce0: 2061 6c6c 6961 6e63 6561 7574 682f 7365   allianceauth/se
+0000dcf0: 7276 6963 6573 2f6d 6f64 756c 6573 2f64  rvices/modules/d
+0000dd00: 6973 636f 7264 2f76 6965 7773 2e70 793a  iscord/views.py:
+0000dd10: 3539 0a6d 7367 6964 2022 416e 2065 7272  59.msgid "An err
+0000dd20: 6f72 206f 6363 7572 7265 6420 7768 696c  or occurred whil
+0000dd30: 6520 7072 6f63 6573 7369 6e67 2079 6f75  e processing you
+0000dd40: 7220 4469 7363 6f72 6420 6163 636f 756e  r Discord accoun
+0000dd50: 742e 220a 6d73 6773 7472 2022 220a 0a23  t.".msgstr ""..#
+0000dd60: 3a20 616c 6c69 616e 6365 6175 7468 2f73  : allianceauth/s
+0000dd70: 6572 7669 6365 732f 6d6f 6475 6c65 732f  ervices/modules/
+0000dd80: 6469 7363 6f72 642f 7669 6577 732e 7079  discord/views.py
+0000dd90: 3a31 3032 0a6d 7367 6964 2022 596f 7572  :102.msgid "Your
+0000dda0: 2044 6973 636f 7264 2061 6363 6f75 6e74   Discord account
+0000ddb0: 2068 6173 2062 6565 6e20 7375 6363 6573   has been succes
+0000ddc0: 7366 756c 6c79 2061 6374 6976 6174 6564  sfully activated
+0000ddd0: 2e22 0a6d 7367 7374 7220 2222 0a0a 233a  .".msgstr ""..#:
+0000dde0: 2061 6c6c 6961 6e63 6561 7574 682f 7365   allianceauth/se
+0000ddf0: 7276 6963 6573 2f6d 6f64 756c 6573 2f64  rvices/modules/d
+0000de00: 6973 636f 7264 2f76 6965 7773 2e70 793a  iscord/views.py:
+0000de10: 3130 380a 6d73 6769 6420 2222 0a22 416e  108.msgid ""."An
+0000de20: 2065 7272 6f72 206f 6363 7572 7265 6420   error occurred 
+0000de30: 7768 696c 6520 7472 7969 6e67 2074 6f20  while trying to 
+0000de40: 6163 7469 7661 7465 2079 6f75 7220 4469  activate your Di
+0000de50: 7363 6f72 6420 6163 636f 756e 742e 2050  scord account. P
+0000de60: 6c65 6173 6520 7472 7920 220a 2261 6761  lease try "."aga
+0000de70: 696e 2e22 0a6d 7367 7374 7220 2222 0a0a  in.".msgstr ""..
+0000de80: 233a 2061 6c6c 6961 6e63 6561 7574 682f  #: allianceauth/
+0000de90: 7365 7276 6963 6573 2f6d 6f64 756c 6573  services/modules
+0000dea0: 2f64 6973 636f 7572 7365 2f74 656d 706c  /discourse/templ
+0000deb0: 6174 6573 2f73 6572 7669 6365 732f 6469  ates/services/di
+0000dec0: 7363 6f75 7273 652f 6469 7363 6f75 7273  scourse/discours
+0000ded0: 655f 7365 7276 6963 655f 6374 726c 2e68  e_service_ctrl.h
+0000dee0: 746d 6c3a 350a 6d73 6769 6420 2244 6973  tml:5.msgid "Dis
+0000def0: 636f 7572 7365 220a 6d73 6773 7472 2022  course".msgstr "
+0000df00: 220a 0a23 3a20 616c 6c69 616e 6365 6175  "..#: allianceau
+0000df10: 7468 2f73 6572 7669 6365 732f 6d6f 6475  th/services/modu
+0000df20: 6c65 732f 6469 7363 6f75 7273 652f 7465  les/discourse/te
+0000df30: 6d70 6c61 7465 732f 7365 7276 6963 6573  mplates/services
+0000df40: 2f64 6973 636f 7572 7365 2f64 6973 636f  /discourse/disco
+0000df50: 7572 7365 5f73 6572 7669 6365 5f63 7472  urse_service_ctr
+0000df60: 6c2e 6874 6d6c 3a31 380a 6d73 6769 6420  l.html:18.msgid 
+0000df70: 2253 534f 206c 6f67 696e 2061 6374 6976  "SSO login activ
+0000df80: 6522 0a6d 7367 7374 7220 2222 0a0a 233a  e".msgstr ""..#:
+0000df90: 2061 6c6c 6961 6e63 6561 7574 682f 7365   allianceauth/se
+0000dfa0: 7276 6963 6573 2f6d 6f64 756c 6573 2f64  rvices/modules/d
+0000dfb0: 6973 636f 7572 7365 2f74 656d 706c 6174  iscourse/templat
+0000dfc0: 6573 2f73 6572 7669 6365 732f 6469 7363  es/services/disc
+0000dfd0: 6f75 7273 652f 6469 7363 6f75 7273 655f  ourse/discourse_
+0000dfe0: 7365 7276 6963 655f 6374 726c 2e68 746d  service_ctrl.htm
+0000dff0: 6c3a 3233 0a6d 7367 6964 2022 476f 2074  l:23.msgid "Go t
+0000e000: 6f20 666f 7275 6d73 220a 6d73 6773 7472  o forums".msgstr
+0000e010: 2022 220a 0a23 3a20 616c 6c69 616e 6365   ""..#: alliance
+0000e020: 6175 7468 2f73 6572 7669 6365 732f 6d6f  auth/services/mo
+0000e030: 6475 6c65 732f 6469 7363 6f75 7273 652f  dules/discourse/
+0000e040: 7669 6577 732e 7079 3a32 390a 6d73 6769  views.py:29.msgi
+0000e050: 6420 2259 6f75 2061 7265 206e 6f74 2061  d "You are not a
+0000e060: 7574 686f 7269 7a65 6420 746f 2061 6363  uthorized to acc
+0000e070: 6573 7320 4469 7363 6f75 7273 652e 220a  ess Discourse.".
+0000e080: 6d73 6773 7472 2022 220a 0a23 3a20 616c  msgstr ""..#: al
+0000e090: 6c69 616e 6365 6175 7468 2f73 6572 7669  lianceauth/servi
+0000e0a0: 6365 732f 6d6f 6475 6c65 732f 6469 7363  ces/modules/disc
+0000e0b0: 6f75 7273 652f 7669 6577 732e 7079 3a33  ourse/views.py:3
+0000e0c0: 340a 6d73 6769 6420 2259 6f75 206d 7573  4.msgid "You mus
+0000e0d0: 7420 6861 7665 2061 206d 6169 6e20 6368  t have a main ch
+0000e0e0: 6172 6163 7465 7220 7365 7420 746f 2061  aracter set to a
+0000e0f0: 6363 6573 7320 4469 7363 6f75 7273 652e  ccess Discourse.
+0000e100: 220a 6d73 6773 7472 2022 220a 0a23 3a20  ".msgstr ""..#: 
+0000e110: 616c 6c69 616e 6365 6175 7468 2f73 6572  allianceauth/ser
+0000e120: 7669 6365 732f 6d6f 6475 6c65 732f 6469  vices/modules/di
+0000e130: 7363 6f75 7273 652f 7669 6577 732e 7079  scourse/views.py
+0000e140: 3a34 340a 6d73 6769 6420 2222 0a22 4e6f  :44.msgid ""."No
+0000e150: 2053 534f 2070 6179 6c6f 6164 206f 7220   SSO payload or 
+0000e160: 7369 676e 6174 7572 652e 2050 6c65 6173  signature. Pleas
+0000e170: 6520 636f 6e74 6163 7420 7375 7070 6f72  e contact suppor
+0000e180: 7420 6966 2074 6869 7320 7072 6f62 6c65  t if this proble
+0000e190: 6d20 7065 7273 6973 7473 2e22 0a6d 7367  m persists.".msg
+0000e1a0: 7374 7220 2222 0a0a 233a 2061 6c6c 6961  str ""..#: allia
+0000e1b0: 6e63 6561 7574 682f 7365 7276 6963 6573  nceauth/services
+0000e1c0: 2f6d 6f64 756c 6573 2f64 6973 636f 7572  /modules/discour
+0000e1d0: 7365 2f76 6965 7773 2e70 793a 3534 0a23  se/views.py:54.#
+0000e1e0: 3a20 616c 6c69 616e 6365 6175 7468 2f73  : allianceauth/s
+0000e1f0: 6572 7669 6365 732f 6d6f 6475 6c65 732f  ervices/modules/
+0000e200: 6469 7363 6f75 7273 652f 7669 6577 732e  discourse/views.
+0000e210: 7079 3a36 320a 6d73 6769 6420 2249 6e76  py:62.msgid "Inv
+0000e220: 616c 6964 2070 6179 6c6f 6164 2e20 506c  alid payload. Pl
+0000e230: 6561 7365 2063 6f6e 7461 6374 2073 7570  ease contact sup
+0000e240: 706f 7274 2069 6620 7468 6973 2070 726f  port if this pro
+0000e250: 626c 656d 2070 6572 7369 7374 732e 220a  blem persists.".
+0000e260: 6d73 6773 7472 2022 220a 0a23 3a20 616c  msgstr ""..#: al
+0000e270: 6c69 616e 6365 6175 7468 2f73 6572 7669  lianceauth/servi
+0000e280: 6365 732f 6d6f 6475 6c65 732f 6970 7334  ces/modules/ips4
+0000e290: 2f76 6965 7773 2e70 793a 3331 0a6d 7367  /views.py:31.msg
+0000e2a0: 6964 2022 4163 7469 7661 7465 6420 4950  id "Activated IP
+0000e2b0: 5375 6974 6534 2061 6363 6f75 6e74 2e22  Suite4 account."
+0000e2c0: 0a6d 7367 7374 7220 2222 0a0a 233a 2061  .msgstr ""..#: a
+0000e2d0: 6c6c 6961 6e63 6561 7574 682f 7365 7276  llianceauth/serv
+0000e2e0: 6963 6573 2f6d 6f64 756c 6573 2f69 7073  ices/modules/ips
+0000e2f0: 342f 7669 6577 732e 7079 3a33 390a 233a  4/views.py:39.#:
+0000e300: 2061 6c6c 6961 6e63 6561 7574 682f 7365   allianceauth/se
+0000e310: 7276 6963 6573 2f6d 6f64 756c 6573 2f69  rvices/modules/i
+0000e320: 7073 342f 7669 6577 732e 7079 3a36 300a  ps4/views.py:60.
+0000e330: 233a 2061 6c6c 6961 6e63 6561 7574 682f  #: allianceauth/
+0000e340: 7365 7276 6963 6573 2f6d 6f64 756c 6573  services/modules
+0000e350: 2f69 7073 342f 7669 6577 732e 7079 3a38  /ips4/views.py:8
+0000e360: 310a 233a 2061 6c6c 6961 6e63 6561 7574  1.#: allianceaut
+0000e370: 682f 7365 7276 6963 6573 2f6d 6f64 756c  h/services/modul
+0000e380: 6573 2f69 7073 342f 7669 6577 732e 7079  es/ips4/views.py
+0000e390: 3a31 3031 0a6d 7367 6964 2022 416e 2065  :101.msgid "An e
+0000e3a0: 7272 6f72 206f 6363 7572 7265 6420 7768  rror occurred wh
+0000e3b0: 696c 6520 7072 6f63 6573 7369 6e67 2079  ile processing y
+0000e3c0: 6f75 7220 4950 5375 6974 6534 2061 6363  our IPSuite4 acc
+0000e3d0: 6f75 6e74 2e22 0a6d 7367 7374 7220 2222  ount.".msgstr ""
+0000e3e0: 0a0a 233a 2061 6c6c 6961 6e63 6561 7574  ..#: allianceaut
+0000e3f0: 682f 7365 7276 6963 6573 2f6d 6f64 756c  h/services/modul
+0000e400: 6573 2f69 7073 342f 7669 6577 732e 7079  es/ips4/views.py
+0000e410: 3a35 320a 6d73 6769 6420 2252 6573 6574  :52.msgid "Reset
+0000e420: 2049 5053 7569 7465 3420 7061 7373 776f   IPSuite4 passwo
+0000e430: 7264 2e22 0a6d 7367 7374 7220 2222 0a0a  rd.".msgstr ""..
+0000e440: 233a 2061 6c6c 6961 6e63 6561 7574 682f  #: allianceauth/
+0000e450: 7365 7276 6963 6573 2f6d 6f64 756c 6573  services/modules
+0000e460: 2f69 7073 342f 7669 6577 732e 7079 3a37  /ips4/views.py:7
+0000e470: 380a 6d73 6769 6420 2253 6574 2049 5053  8.msgid "Set IPS
+0000e480: 7569 7465 3420 7061 7373 776f 7264 2e22  uite4 password."
+0000e490: 0a6d 7367 7374 7220 2222 0a0a 233a 2061  .msgstr ""..#: a
+0000e4a0: 6c6c 6961 6e63 6561 7574 682f 7365 7276  llianceauth/serv
+0000e4b0: 6963 6573 2f6d 6f64 756c 6573 2f69 7073  ices/modules/ips
+0000e4c0: 342f 7669 6577 732e 7079 3a39 380a 6d73  4/views.py:98.ms
+0000e4d0: 6769 6420 2244 6561 6374 6976 6174 6564  gid "Deactivated
+0000e4e0: 2049 5053 7569 7465 3420 6163 636f 756e   IPSuite4 accoun
+0000e4f0: 742e 220a 6d73 6773 7472 2022 220a 0a23  t.".msgstr ""..#
+0000e500: 3a20 616c 6c69 616e 6365 6175 7468 2f73  : allianceauth/s
+0000e510: 6572 7669 6365 732f 6d6f 6475 6c65 732f  ervices/modules/
+0000e520: 6d75 6d62 6c65 2f74 656d 706c 6174 6573  mumble/templates
+0000e530: 2f73 6572 7669 6365 732f 6d75 6d62 6c65  /services/mumble
+0000e540: 2f6d 756d 626c 655f 7365 7276 6963 655f  /mumble_service_
+0000e550: 6374 726c 2e68 746d 6c3a 3236 0a23 3a20  ctrl.html:26.#: 
+0000e560: 616c 6c69 616e 6365 6175 7468 2f73 6572  allianceauth/ser
+0000e570: 7669 6365 732f 7465 6d70 6c61 7465 732f  vices/templates/
+0000e580: 7365 7276 6963 6573 2f73 6572 7669 6365  services/service
+0000e590: 5f70 6173 7377 6f72 642e 6874 6d6c 3a32  _password.html:2
+0000e5a0: 360a 6d73 6769 6420 2253 6574 2050 6173  6.msgid "Set Pas
+0000e5b0: 7377 6f72 6422 0a6d 7367 7374 7220 2222  sword".msgstr ""
+0000e5c0: 0a0a 233a 2061 6c6c 6961 6e63 6561 7574  ..#: allianceaut
+0000e5d0: 682f 7365 7276 6963 6573 2f6d 6f64 756c  h/services/modul
+0000e5e0: 6573 2f6d 756d 626c 652f 7465 6d70 6c61  es/mumble/templa
+0000e5f0: 7465 732f 7365 7276 6963 6573 2f6d 756d  tes/services/mum
+0000e600: 626c 652f 6d75 6d62 6c65 5f73 6572 7669  ble/mumble_servi
+0000e610: 6365 5f63 7472 6c2e 6874 6d6c 3a34 340a  ce_ctrl.html:44.
+0000e620: 6d73 6769 6420 2243 6f6e 6e65 6374 220a  msgid "Connect".
+0000e630: 6d73 6773 7472 2022 220a 0a23 3a20 616c  msgstr ""..#: al
+0000e640: 6c69 616e 6365 6175 7468 2f73 6572 7669  lianceauth/servi
+0000e650: 6365 732f 6d6f 6475 6c65 732f 6f70 656e  ces/modules/open
+0000e660: 6669 7265 2f61 7574 685f 686f 6f6b 732e  fire/auth_hooks.
+0000e670: 7079 3a32 370a 6d73 6769 6420 224a 6162  py:27.msgid "Jab
+0000e680: 6265 7222 0a6d 7367 7374 7220 2222 0a0a  ber".msgstr ""..
+0000e690: 233a 2061 6c6c 6961 6e63 6561 7574 682f  #: allianceauth/
+0000e6a0: 7365 7276 6963 6573 2f6d 6f64 756c 6573  services/modules
+0000e6b0: 2f6f 7065 6e66 6972 652f 6175 7468 5f68  /openfire/auth_h
+0000e6c0: 6f6f 6b73 2e70 793a 3830 0a23 3a20 616c  ooks.py:80.#: al
+0000e6d0: 6c69 616e 6365 6175 7468 2f73 6572 7669  lianceauth/servi
+0000e6e0: 6365 732f 6d6f 6475 6c65 732f 6f70 656e  ces/modules/open
+0000e6f0: 6669 7265 2f74 656d 706c 6174 6573 2f73  fire/templates/s
+0000e700: 6572 7669 6365 732f 6f70 656e 6669 7265  ervices/openfire
+0000e710: 2f62 726f 6164 6361 7374 2e68 746d 6c3a  /broadcast.html:
+0000e720: 370a 233a 2061 6c6c 6961 6e63 6561 7574  7.#: allianceaut
+0000e730: 682f 7365 7276 6963 6573 2f6d 6f64 756c  h/services/modul
+0000e740: 6573 2f6f 7065 6e66 6972 652f 7465 6d70  es/openfire/temp
+0000e750: 6c61 7465 732f 7365 7276 6963 6573 2f6f  lates/services/o
+0000e760: 7065 6e66 6972 652f 6272 6f61 6463 6173  penfire/broadcas
+0000e770: 742e 6874 6d6c 3a31 310a 233a 2061 6c6c  t.html:11.#: all
+0000e780: 6961 6e63 6561 7574 682f 7365 7276 6963  ianceauth/servic
+0000e790: 6573 2f6d 6f64 756c 6573 2f6f 7065 6e66  es/modules/openf
+0000e7a0: 6972 652f 7465 6d70 6c61 7465 732f 7365  ire/templates/se
+0000e7b0: 7276 6963 6573 2f6f 7065 6e66 6972 652f  rvices/openfire/
+0000e7c0: 6272 6f61 6463 6173 742e 6874 6d6c 3a31  broadcast.html:1
+0000e7d0: 390a 6d73 6769 6420 224a 6162 6265 7220  9.msgid "Jabber 
+0000e7e0: 4272 6f61 6463 6173 7422 0a6d 7367 7374  Broadcast".msgst
+0000e7f0: 7220 2222 0a0a 233a 2061 6c6c 6961 6e63  r ""..#: allianc
+0000e800: 6561 7574 682f 7365 7276 6963 6573 2f6d  eauth/services/m
+0000e810: 6f64 756c 6573 2f6f 7065 6e66 6972 652f  odules/openfire/
+0000e820: 6175 7468 5f68 6f6f 6b73 2e70 793a 3935  auth_hooks.py:95
+0000e830: 0a6d 7367 6964 2022 466c 6565 7420 4272  .msgid "Fleet Br
+0000e840: 6f61 6463 6173 7420 466f 726d 6174 7465  oadcast Formatte
+0000e850: 7222 0a6d 7367 7374 7220 2222 0a0a 233a  r".msgstr ""..#:
+0000e860: 2061 6c6c 6961 6e63 6561 7574 682f 7365   allianceauth/se
+0000e870: 7276 6963 6573 2f6d 6f64 756c 6573 2f6f  rvices/modules/o
+0000e880: 7065 6e66 6972 652f 666f 726d 732e 7079  penfire/forms.py
+0000e890: 3a37 0a6d 7367 6964 2022 4d65 7373 6167  :7.msgid "Messag
+0000e8a0: 6522 0a6d 7367 7374 7220 2222 0a0a 233a  e".msgstr ""..#:
+0000e8b0: 2061 6c6c 6961 6e63 6561 7574 682f 7365   allianceauth/se
+0000e8c0: 7276 6963 6573 2f6d 6f64 756c 6573 2f6f  rvices/modules/o
+0000e8d0: 7065 6e66 6972 652f 7465 6d70 6c61 7465  penfire/template
+0000e8e0: 732f 7365 7276 6963 6573 2f6f 7065 6e66  s/services/openf
+0000e8f0: 6972 652f 6272 6f61 6463 6173 742e 6874  ire/broadcast.ht
+0000e900: 6d6c 3a32 380a 6d73 6769 6420 2242 726f  ml:28.msgid "Bro
+0000e910: 6164 6361 7374 2053 656e 7421 2122 0a6d  adcast Sent!!".m
+0000e920: 7367 7374 7220 2222 0a0a 233a 2061 6c6c  sgstr ""..#: all
+0000e930: 6961 6e63 6561 7574 682f 7365 7276 6963  ianceauth/servic
+0000e940: 6573 2f6d 6f64 756c 6573 2f6f 7065 6e66  es/modules/openf
+0000e950: 6972 652f 7465 6d70 6c61 7465 732f 7365  ire/templates/se
+0000e960: 7276 6963 6573 2f6f 7065 6e66 6972 652f  rvices/openfire/
+0000e970: 6272 6f61 6463 6173 742e 6874 6d6c 3a33  broadcast.html:3
+0000e980: 380a 6d73 6769 6420 2242 726f 6164 6361  8.msgid "Broadca
+0000e990: 7374 220a 6d73 6773 7472 2022 220a 0a23  st".msgstr ""..#
+0000e9a0: 3a20 616c 6c69 616e 6365 6175 7468 2f73  : allianceauth/s
+0000e9b0: 6572 7669 6365 732f 6d6f 6475 6c65 732f  ervices/modules/
+0000e9c0: 6f70 656e 6669 7265 2f76 6965 7773 2e70  openfire/views.p
+0000e9d0: 793a 3335 0a6d 7367 6964 2022 4163 7469  y:35.msgid "Acti
+0000e9e0: 7661 7465 6420 4a61 6262 6572 2061 6363  vated Jabber acc
+0000e9f0: 6f75 6e74 2e22 0a6d 7367 7374 7220 2222  ount.".msgstr ""
+0000ea00: 0a0a 233a 2061 6c6c 6961 6e63 6561 7574  ..#: allianceaut
+0000ea10: 682f 7365 7276 6963 6573 2f6d 6f64 756c  h/services/modul
+0000ea20: 6573 2f6f 7065 6e66 6972 652f 7669 6577  es/openfire/view
+0000ea30: 732e 7079 3a34 330a 233a 2061 6c6c 6961  s.py:43.#: allia
+0000ea40: 6e63 6561 7574 682f 7365 7276 6963 6573  nceauth/services
+0000ea50: 2f6d 6f64 756c 6573 2f6f 7065 6e66 6972  /modules/openfir
+0000ea60: 652f 7669 6577 732e 7079 3a35 360a 233a  e/views.py:56.#:
+0000ea70: 2061 6c6c 6961 6e63 6561 7574 682f 7365   allianceauth/se
+0000ea80: 7276 6963 6573 2f6d 6f64 756c 6573 2f6f  rvices/modules/o
+0000ea90: 7065 6e66 6972 652f 7669 6577 732e 7079  penfire/views.py
+0000eaa0: 3a37 360a 233a 2061 6c6c 6961 6e63 6561  :76.#: alliancea
+0000eab0: 7574 682f 7365 7276 6963 6573 2f6d 6f64  uth/services/mod
+0000eac0: 756c 6573 2f6f 7065 6e66 6972 652f 7669  ules/openfire/vi
+0000ead0: 6577 732e 7079 3a31 3437 0a6d 7367 6964  ews.py:147.msgid
+0000eae0: 2022 416e 2065 7272 6f72 206f 6363 7572   "An error occur
+0000eaf0: 7265 6420 7768 696c 6520 7072 6f63 6573  red while proces
+0000eb00: 7369 6e67 2079 6f75 7220 4a61 6262 6572  sing your Jabber
+0000eb10: 2061 6363 6f75 6e74 2e22 0a6d 7367 7374   account.".msgst
+0000eb20: 7220 2222 0a0a 233a 2061 6c6c 6961 6e63  r ""..#: allianc
+0000eb30: 6561 7574 682f 7365 7276 6963 6573 2f6d  eauth/services/m
+0000eb40: 6f64 756c 6573 2f6f 7065 6e66 6972 652f  odules/openfire/
+0000eb50: 7669 6577 732e 7079 3a36 390a 6d73 6769  views.py:69.msgi
+0000eb60: 6420 2252 6573 6574 204a 6162 6265 7220  d "Reset Jabber 
+0000eb70: 7061 7373 776f 7264 2e22 0a6d 7367 7374  password.".msgst
+0000eb80: 7220 2222 0a0a 233a 2061 6c6c 6961 6e63  r ""..#: allianc
+0000eb90: 6561 7574 682f 7365 7276 6963 6573 2f6d  eauth/services/m
+0000eba0: 6f64 756c 6573 2f6f 7065 6e66 6972 652f  odules/openfire/
+0000ebb0: 7669 6577 732e 7079 3a31 3135 0a23 2c20  views.py:115.#, 
+0000ebc0: 7079 7468 6f6e 2d66 6f72 6d61 740a 6d73  python-format.ms
+0000ebd0: 6769 6420 2253 656e 7420 4a61 6262 6572  gid "Sent Jabber
+0000ebe0: 2062 726f 6164 6361 7374 2074 6f20 2573   broadcast to %s
+0000ebf0: 220a 6d73 6773 7472 2022 220a 0a23 3a20  ".msgstr ""..#: 
+0000ec00: 616c 6c69 616e 6365 6175 7468 2f73 6572  allianceauth/ser
+0000ec10: 7669 6365 732f 6d6f 6475 6c65 732f 6f70  vices/modules/op
+0000ec20: 656e 6669 7265 2f76 6965 7773 2e70 793a  enfire/views.py:
+0000ec30: 3134 340a 6d73 6769 6420 2253 6574 206a  144.msgid "Set j
+0000ec40: 6162 6265 7220 7061 7373 776f 7264 2e22  abber password."
+0000ec50: 0a6d 7367 7374 7220 2222 0a0a 233a 2061  .msgstr ""..#: a
+0000ec60: 6c6c 6961 6e63 6561 7574 682f 7365 7276  llianceauth/serv
+0000ec70: 6963 6573 2f6d 6f64 756c 6573 2f70 6870  ices/modules/php
+0000ec80: 6262 332f 7669 6577 732e 7079 3a33 340a  bb3/views.py:34.
+0000ec90: 6d73 6769 6420 2241 6374 6976 6174 6564  msgid "Activated
+0000eca0: 2066 6f72 756d 2061 6363 6f75 6e74 2e22   forum account."
+0000ecb0: 0a6d 7367 7374 7220 2222 0a0a 233a 2061  .msgstr ""..#: a
+0000ecc0: 6c6c 6961 6e63 6561 7574 682f 7365 7276  llianceauth/serv
+0000ecd0: 6963 6573 2f6d 6f64 756c 6573 2f70 6870  ices/modules/php
+0000ece0: 6262 332f 7669 6577 732e 7079 3a34 320a  bb3/views.py:42.
+0000ecf0: 233a 2061 6c6c 6961 6e63 6561 7574 682f  #: allianceauth/
+0000ed00: 7365 7276 6963 6573 2f6d 6f64 756c 6573  services/modules
+0000ed10: 2f70 6870 6262 332f 7669 6577 732e 7079  /phpbb3/views.py
+0000ed20: 3a35 360a 233a 2061 6c6c 6961 6e63 6561  :56.#: alliancea
+0000ed30: 7574 682f 7365 7276 6963 6573 2f6d 6f64  uth/services/mod
+0000ed40: 756c 6573 2f70 6870 6262 332f 7669 6577  ules/phpbb3/view
+0000ed50: 732e 7079 3a37 380a 233a 2061 6c6c 6961  s.py:78.#: allia
+0000ed60: 6e63 6561 7574 682f 7365 7276 6963 6573  nceauth/services
+0000ed70: 2f6d 6f64 756c 6573 2f70 6870 6262 332f  /modules/phpbb3/
+0000ed80: 7669 6577 732e 7079 3a31 3031 0a6d 7367  views.py:101.msg
+0000ed90: 6964 2022 416e 2065 7272 6f72 206f 6363  id "An error occ
+0000eda0: 7572 7265 6420 7768 696c 6520 7072 6f63  urred while proc
+0000edb0: 6573 7369 6e67 2079 6f75 7220 666f 7275  essing your foru
+0000edc0: 6d20 6163 636f 756e 742e 220a 6d73 6773  m account.".msgs
+0000edd0: 7472 2022 220a 0a23 3a20 616c 6c69 616e  tr ""..#: allian
+0000ede0: 6365 6175 7468 2f73 6572 7669 6365 732f  ceauth/services/
+0000edf0: 6d6f 6475 6c65 732f 7068 7062 6233 2f76  modules/phpbb3/v
+0000ee00: 6965 7773 2e70 793a 3533 0a6d 7367 6964  iews.py:53.msgid
+0000ee10: 2022 4465 6163 7469 7661 7465 6420 666f   "Deactivated fo
+0000ee20: 7275 6d20 6163 636f 756e 742e 220a 6d73  rum account.".ms
+0000ee30: 6773 7472 2022 220a 0a23 3a20 616c 6c69  gstr ""..#: alli
+0000ee40: 616e 6365 6175 7468 2f73 6572 7669 6365  anceauth/service
+0000ee50: 732f 6d6f 6475 6c65 732f 7068 7062 6233  s/modules/phpbb3
+0000ee60: 2f76 6965 7773 2e70 793a 3730 0a6d 7367  /views.py:70.msg
+0000ee70: 6964 2022 5265 7365 7420 666f 7275 6d20  id "Reset forum 
+0000ee80: 7061 7373 776f 7264 2e22 0a6d 7367 7374  password.".msgst
+0000ee90: 7220 2222 0a0a 233a 2061 6c6c 6961 6e63  r ""..#: allianc
+0000eea0: 6561 7574 682f 7365 7276 6963 6573 2f6d  eauth/services/m
+0000eeb0: 6f64 756c 6573 2f70 6870 6262 332f 7669  odules/phpbb3/vi
+0000eec0: 6577 732e 7079 3a39 380a 6d73 6769 6420  ews.py:98.msgid 
+0000eed0: 2253 6574 2066 6f72 756d 2070 6173 7377  "Set forum passw
+0000eee0: 6f72 642e 220a 6d73 6773 7472 2022 220a  ord.".msgstr "".
+0000eef0: 0a23 3a20 616c 6c69 616e 6365 6175 7468  .#: allianceauth
+0000ef00: 2f73 6572 7669 6365 732f 6d6f 6475 6c65  /services/module
+0000ef10: 732f 736d 662f 7669 6577 732e 7079 3a35  s/smf/views.py:5
+0000ef20: 320a 6d73 6769 6420 2241 6374 6976 6174  2.msgid "Activat
+0000ef30: 6564 2053 4d46 2061 6363 6f75 6e74 2e22  ed SMF account."
+0000ef40: 0a6d 7367 7374 7220 2222 0a0a 233a 2061  .msgstr ""..#: a
+0000ef50: 6c6c 6961 6e63 6561 7574 682f 7365 7276  llianceauth/serv
+0000ef60: 6963 6573 2f6d 6f64 756c 6573 2f73 6d66  ices/modules/smf
+0000ef70: 2f76 6965 7773 2e70 793a 3635 0a23 3a20  /views.py:65.#: 
+0000ef80: 616c 6c69 616e 6365 6175 7468 2f73 6572  allianceauth/ser
+0000ef90: 7669 6365 732f 6d6f 6475 6c65 732f 736d  vices/modules/sm
+0000efa0: 662f 7669 6577 732e 7079 3a38 310a 233a  f/views.py:81.#:
+0000efb0: 2061 6c6c 6961 6e63 6561 7574 682f 7365   allianceauth/se
+0000efc0: 7276 6963 6573 2f6d 6f64 756c 6573 2f73  rvices/modules/s
+0000efd0: 6d66 2f76 6965 7773 2e70 793a 3130 320a  mf/views.py:102.
+0000efe0: 233a 2061 6c6c 6961 6e63 6561 7574 682f  #: allianceauth/
+0000eff0: 7365 7276 6963 6573 2f6d 6f64 756c 6573  services/modules
+0000f000: 2f73 6d66 2f76 6965 7773 2e70 793a 3132  /smf/views.py:12
+0000f010: 340a 6d73 6769 6420 2241 6e20 6572 726f  4.msgid "An erro
+0000f020: 7220 6f63 6375 7272 6564 2077 6869 6c65  r occurred while
+0000f030: 2070 726f 6365 7373 696e 6720 796f 7572   processing your
+0000f040: 2053 4d46 2061 6363 6f75 6e74 2e22 0a6d   SMF account.".m
+0000f050: 7367 7374 7220 2222 0a0a 233a 2061 6c6c  sgstr ""..#: all
+0000f060: 6961 6e63 6561 7574 682f 7365 7276 6963  ianceauth/servic
+0000f070: 6573 2f6d 6f64 756c 6573 2f73 6d66 2f76  es/modules/smf/v
+0000f080: 6965 7773 2e70 793a 3738 0a6d 7367 6964  iews.py:78.msgid
+0000f090: 2022 4465 6163 7469 7661 7465 6420 534d   "Deactivated SM
+0000f0a0: 4620 6163 636f 756e 742e 220a 6d73 6773  F account.".msgs
+0000f0b0: 7472 2022 220a 0a23 3a20 616c 6c69 616e  tr ""..#: allian
+0000f0c0: 6365 6175 7468 2f73 6572 7669 6365 732f  ceauth/services/
+0000f0d0: 6d6f 6475 6c65 732f 736d 662f 7669 6577  modules/smf/view
+0000f0e0: 732e 7079 3a39 350a 6d73 6769 6420 2252  s.py:95.msgid "R
+0000f0f0: 6573 6574 2053 4d46 2070 6173 7377 6f72  eset SMF passwor
+0000f100: 642e 220a 6d73 6773 7472 2022 220a 0a23  d.".msgstr ""..#
+0000f110: 3a20 616c 6c69 616e 6365 6175 7468 2f73  : allianceauth/s
+0000f120: 6572 7669 6365 732f 6d6f 6475 6c65 732f  ervices/modules/
+0000f130: 736d 662f 7669 6577 732e 7079 3a31 3231  smf/views.py:121
+0000f140: 0a6d 7367 6964 2022 5365 7420 534d 4620  .msgid "Set SMF 
+0000f150: 7061 7373 776f 7264 2e22 0a6d 7367 7374  password.".msgst
+0000f160: 7220 2222 0a0a 233a 2061 6c6c 6961 6e63  r ""..#: allianc
+0000f170: 6561 7574 682f 7365 7276 6963 6573 2f6d  eauth/services/m
+0000f180: 6f64 756c 6573 2f74 6561 6d73 7065 616b  odules/teamspeak
+0000f190: 332f 666f 726d 732e 7079 3a31 340a 232c  3/forms.py:14.#,
+0000f1a0: 2070 7974 686f 6e2d 666f 726d 6174 0a6d   python-format.m
+0000f1b0: 7367 6964 2022 556e 6162 6c65 2074 6f20  sgid "Unable to 
+0000f1c0: 6c6f 6361 7465 2075 7365 7220 2573 206f  locate user %s o
+0000f1d0: 6e20 7365 7276 6572 220a 6d73 6773 7472  n server".msgstr
+0000f1e0: 2022 220a 0a23 3a20 616c 6c69 616e 6365   ""..#: alliance
+0000f1f0: 6175 7468 2f73 6572 7669 6365 732f 6d6f  auth/services/mo
+0000f200: 6475 6c65 732f 7465 616d 7370 6561 6b33  dules/teamspeak3
+0000f210: 2f74 656d 706c 6174 6573 2f61 646d 696e  /templates/admin
+0000f220: 2f74 6561 6d73 7065 616b 332f 6175 7468  /teamspeak3/auth
+0000f230: 7473 2f63 6861 6e67 655f 6c69 7374 2e68  ts/change_list.h
+0000f240: 746d 6c3a 3130 0a6d 7367 6964 2022 5570  tml:10.msgid "Up
+0000f250: 6461 7465 2054 6561 6d53 7065 616b 3320  date TeamSpeak3 
+0000f260: 6772 6f75 7073 220a 6d73 6773 7472 2022  groups".msgstr "
+0000f270: 220a 0a23 3a20 616c 6c69 616e 6365 6175  "..#: allianceau
+0000f280: 7468 2f73 6572 7669 6365 732f 6d6f 6475  th/services/modu
+0000f290: 6c65 732f 7465 616d 7370 6561 6b33 2f74  les/teamspeak3/t
+0000f2a0: 656d 706c 6174 6573 2f73 6572 7669 6365  emplates/service
+0000f2b0: 732f 7465 616d 7370 6561 6b33 2f74 6561  s/teamspeak3/tea
+0000f2c0: 6d73 7065 616b 335f 7365 7276 6963 655f  mspeak3_service_
+0000f2d0: 6374 726c 2e68 746d 6c3a 360a 6d73 6769  ctrl.html:6.msgi
+0000f2e0: 6420 2254 6561 6d73 7065 616b 2033 220a  d "Teamspeak 3".
+0000f2f0: 6d73 6773 7472 2022 220a 0a23 3a20 616c  msgstr ""..#: al
+0000f300: 6c69 616e 6365 6175 7468 2f73 6572 7669  lianceauth/servi
+0000f310: 6365 732f 6d6f 6475 6c65 732f 7465 616d  ces/modules/team
+0000f320: 7370 6561 6b33 2f74 656d 706c 6174 6573  speak3/templates
+0000f330: 2f73 6572 7669 6365 732f 7465 616d 7370  /services/teamsp
+0000f340: 6561 6b33 2f74 6561 6d73 7065 616b 6a6f  eak3/teamspeakjo
+0000f350: 696e 2e68 746d 6c3a 360a 6d73 6769 6420  in.html:6.msgid 
+0000f360: 2256 6572 6966 7920 5465 616d 5370 6561  "Verify TeamSpea
+0000f370: 6b33 220a 6d73 6773 7472 2022 220a 0a23  k3".msgstr ""..#
+0000f380: 3a20 616c 6c69 616e 6365 6175 7468 2f73  : allianceauth/s
+0000f390: 6572 7669 6365 732f 6d6f 6475 6c65 732f  ervices/modules/
+0000f3a0: 7465 616d 7370 6561 6b33 2f74 656d 706c  teamspeak3/templ
+0000f3b0: 6174 6573 2f73 6572 7669 6365 732f 7465  ates/services/te
+0000f3c0: 616d 7370 6561 6b33 2f74 6561 6d73 7065  amspeak3/teamspe
+0000f3d0: 616b 6a6f 696e 2e68 746d 6c3a 3130 0a6d  akjoin.html:10.m
+0000f3e0: 7367 6964 2022 5665 7269 6679 2054 6561  sgid "Verify Tea
+0000f3f0: 6d53 7065 616b 3320 4964 656e 7469 7479  mSpeak3 Identity
+0000f400: 220a 6d73 6773 7472 2022 220a 0a23 3a20  ".msgstr ""..#: 
+0000f410: 616c 6c69 616e 6365 6175 7468 2f73 6572  allianceauth/ser
+0000f420: 7669 6365 732f 6d6f 6475 6c65 732f 7465  vices/modules/te
+0000f430: 616d 7370 6561 6b33 2f74 656d 706c 6174  amspeak3/templat
+0000f440: 6573 2f73 6572 7669 6365 732f 7465 616d  es/services/team
+0000f450: 7370 6561 6b33 2f74 6561 6d73 7065 616b  speak3/teamspeak
+0000f460: 6a6f 696e 2e68 746d 6c3a 3135 0a6d 7367  join.html:15.msg
+0000f470: 6964 2022 4a6f 696e 2053 6572 7665 7222  id "Join Server"
+0000f480: 0a6d 7367 7374 7220 2222 0a0a 233a 2061  .msgstr ""..#: a
+0000f490: 6c6c 6961 6e63 6561 7574 682f 7365 7276  llianceauth/serv
+0000f4a0: 6963 6573 2f6d 6f64 756c 6573 2f74 6561  ices/modules/tea
+0000f4b0: 6d73 7065 616b 332f 7465 6d70 6c61 7465  mspeak3/template
+0000f4c0: 732f 7365 7276 6963 6573 2f74 6561 6d73  s/services/teams
+0000f4d0: 7065 616b 332f 7465 616d 7370 6561 6b6a  peak3/teamspeakj
+0000f4e0: 6f69 6e2e 6874 6d6c 3a32 330a 233a 2061  oin.html:23.#: a
+0000f4f0: 6c6c 6961 6e63 6561 7574 682f 7365 7276  llianceauth/serv
+0000f500: 6963 6573 2f74 656d 706c 6174 6573 2f73  ices/templates/s
+0000f510: 6572 7669 6365 732f 7365 7276 6963 655f  ervices/service_
+0000f520: 6372 6564 656e 7469 616c 732e 6874 6d6c  credentials.html
+0000f530: 3a33 300a 233a 2061 6c6c 6961 6e63 6561  :30.#: alliancea
+0000f540: 7574 682f 7372 702f 7465 6d70 6c61 7465  uth/srp/template
+0000f550: 732f 7372 702f 6164 642e 6874 6d6c 3a35  s/srp/add.html:5
+0000f560: 310a 6d73 6769 6420 2243 6f6e 7469 6e75  1.msgid "Continu
+0000f570: 6522 0a6d 7367 7374 7220 2222 0a0a 233a  e".msgstr ""..#:
+0000f580: 2061 6c6c 6961 6e63 6561 7574 682f 7365   allianceauth/se
+0000f590: 7276 6963 6573 2f6d 6f64 756c 6573 2f74  rvices/modules/t
+0000f5a0: 6561 6d73 7065 616b 332f 7669 6577 732e  eamspeak3/views.
+0000f5b0: 7079 3a33 350a 6d73 6769 6420 2241 6374  py:35.msgid "Act
+0000f5c0: 6976 6174 6564 2054 6561 6d53 7065 616b  ivated TeamSpeak
+0000f5d0: 3320 6163 636f 756e 742e 220a 6d73 6773  3 account.".msgs
+0000f5e0: 7472 2022 220a 0a23 3a20 616c 6c69 616e  tr ""..#: allian
+0000f5f0: 6365 6175 7468 2f73 6572 7669 6365 732f  ceauth/services/
+0000f600: 6d6f 6475 6c65 732f 7465 616d 7370 6561  modules/teamspea
+0000f610: 6b33 2f76 6965 7773 2e70 793a 3338 0a23  k3/views.py:38.#
+0000f620: 3a20 616c 6c69 616e 6365 6175 7468 2f73  : allianceauth/s
+0000f630: 6572 7669 6365 732f 6d6f 6475 6c65 732f  ervices/modules/
+0000f640: 7465 616d 7370 6561 6b33 2f76 6965 7773  teamspeak3/views
+0000f650: 2e70 793a 3734 0a23 3a20 616c 6c69 616e  .py:74.#: allian
+0000f660: 6365 6175 7468 2f73 6572 7669 6365 732f  ceauth/services/
+0000f670: 6d6f 6475 6c65 732f 7465 616d 7370 6561  modules/teamspea
+0000f680: 6b33 2f76 6965 7773 2e70 793a 3130 300a  k3/views.py:100.
+0000f690: 6d73 6769 6420 2241 6e20 6572 726f 7220  msgid "An error 
+0000f6a0: 6f63 6375 7272 6564 2077 6869 6c65 2070  occurred while p
+0000f6b0: 726f 6365 7373 696e 6720 796f 7572 2054  rocessing your T
+0000f6c0: 6561 6d53 7065 616b 3320 6163 636f 756e  eamSpeak3 accoun
+0000f6d0: 742e 220a 6d73 6773 7472 2022 220a 0a23  t.".msgstr ""..#
+0000f6e0: 3a20 616c 6c69 616e 6365 6175 7468 2f73  : allianceauth/s
+0000f6f0: 6572 7669 6365 732f 6d6f 6475 6c65 732f  ervices/modules/
+0000f700: 7465 616d 7370 6561 6b33 2f76 6965 7773  teamspeak3/views
+0000f710: 2e70 793a 3731 0a6d 7367 6964 2022 4465  .py:71.msgid "De
+0000f720: 6163 7469 7661 7465 6420 5465 616d 5370  activated TeamSp
+0000f730: 6561 6b33 2061 6363 6f75 6e74 2e22 0a6d  eak3 account.".m
+0000f740: 7367 7374 7220 2222 0a0a 233a 2061 6c6c  sgstr ""..#: all
+0000f750: 6961 6e63 6561 7574 682f 7365 7276 6963  ianceauth/servic
+0000f760: 6573 2f6d 6f64 756c 6573 2f74 6561 6d73  es/modules/teams
+0000f770: 7065 616b 332f 7669 6577 732e 7079 3a39  peak3/views.py:9
+0000f780: 370a 6d73 6769 6420 2252 6573 6574 2054  7.msgid "Reset T
+0000f790: 6561 6d53 7065 616b 3320 7065 726d 6973  eamSpeak3 permis
+0000f7a0: 7369 6f6e 206b 6579 2e22 0a6d 7367 7374  sion key.".msgst
+0000f7b0: 7220 2222 0a0a 233a 2061 6c6c 6961 6e63  r ""..#: allianc
+0000f7c0: 6561 7574 682f 7365 7276 6963 6573 2f6d  eauth/services/m
+0000f7d0: 6f64 756c 6573 2f78 656e 666f 726f 2f76  odules/xenforo/v
+0000f7e0: 6965 7773 2e70 793a 3330 0a6d 7367 6964  iews.py:30.msgid
+0000f7f0: 2022 4163 7469 7661 7465 6420 5865 6e46   "Activated XenF
+0000f800: 6f72 6f20 6163 636f 756e 742e 220a 6d73  oro account.".ms
+0000f810: 6773 7472 2022 220a 0a23 3a20 616c 6c69  gstr ""..#: alli
+0000f820: 616e 6365 6175 7468 2f73 6572 7669 6365  anceauth/service
+0000f830: 732f 6d6f 6475 6c65 732f 7865 6e66 6f72  s/modules/xenfor
+0000f840: 6f2f 7669 6577 732e 7079 3a34 300a 233a  o/views.py:40.#:
+0000f850: 2061 6c6c 6961 6e63 6561 7574 682f 7365   allianceauth/se
+0000f860: 7276 6963 6573 2f6d 6f64 756c 6573 2f78  rvices/modules/x
+0000f870: 656e 666f 726f 2f76 6965 7773 2e70 793a  enforo/views.py:
+0000f880: 3532 0a23 3a20 616c 6c69 616e 6365 6175  52.#: allianceau
+0000f890: 7468 2f73 6572 7669 6365 732f 6d6f 6475  th/services/modu
+0000f8a0: 6c65 732f 7865 6e66 6f72 6f2f 7669 6577  les/xenforo/view
+0000f8b0: 732e 7079 3a37 330a 233a 2061 6c6c 6961  s.py:73.#: allia
+0000f8c0: 6e63 6561 7574 682f 7365 7276 6963 6573  nceauth/services
+0000f8d0: 2f6d 6f64 756c 6573 2f78 656e 666f 726f  /modules/xenforo
+0000f8e0: 2f76 6965 7773 2e70 793a 3934 0a6d 7367  /views.py:94.msg
+0000f8f0: 6964 2022 416e 2065 7272 6f72 206f 6363  id "An error occ
+0000f900: 7572 7265 6420 7768 696c 6520 7072 6f63  urred while proc
+0000f910: 6573 7369 6e67 2079 6f75 7220 5865 6e46  essing your XenF
+0000f920: 6f72 6f20 6163 636f 756e 742e 220a 6d73  oro account.".ms
+0000f930: 6773 7472 2022 220a 0a23 3a20 616c 6c69  gstr ""..#: alli
+0000f940: 616e 6365 6175 7468 2f73 6572 7669 6365  anceauth/service
+0000f950: 732f 6d6f 6475 6c65 732f 7865 6e66 6f72  s/modules/xenfor
+0000f960: 6f2f 7669 6577 732e 7079 3a35 300a 6d73  o/views.py:50.ms
+0000f970: 6769 6420 2244 6561 6374 6976 6174 6564  gid "Deactivated
+0000f980: 2058 656e 466f 726f 2061 6363 6f75 6e74   XenForo account
+0000f990: 2e22 0a6d 7367 7374 7220 2222 0a0a 233a  .".msgstr ""..#:
+0000f9a0: 2061 6c6c 6961 6e63 6561 7574 682f 7365   allianceauth/se
+0000f9b0: 7276 6963 6573 2f6d 6f64 756c 6573 2f78  rvices/modules/x
+0000f9c0: 656e 666f 726f 2f76 6965 7773 2e70 793a  enforo/views.py:
+0000f9d0: 3635 0a6d 7367 6964 2022 5265 7365 7420  65.msgid "Reset 
+0000f9e0: 5865 6e46 6f72 6f20 6163 636f 756e 7420  XenForo account 
+0000f9f0: 7061 7373 776f 7264 2e22 0a6d 7367 7374  password.".msgst
+0000fa00: 7220 2222 0a0a 233a 2061 6c6c 6961 6e63  r ""..#: allianc
+0000fa10: 6561 7574 682f 7365 7276 6963 6573 2f6d  eauth/services/m
+0000fa20: 6f64 756c 6573 2f78 656e 666f 726f 2f76  odules/xenforo/v
+0000fa30: 6965 7773 2e70 793a 3931 0a6d 7367 6964  iews.py:91.msgid
+0000fa40: 2022 4368 616e 6765 6420 5865 6e46 6f72   "Changed XenFor
+0000fa50: 6f20 7061 7373 776f 7264 2e22 0a6d 7367  o password.".msg
+0000fa60: 7374 7220 2222 0a0a 233a 2061 6c6c 6961  str ""..#: allia
+0000fa70: 6e63 6561 7574 682f 7365 7276 6963 6573  nceauth/services
+0000fa80: 2f74 656d 706c 6174 6573 2f73 6572 7669  /templates/servi
+0000fa90: 6365 732f 666c 6565 7466 6f72 6d61 7474  ces/fleetformatt
+0000faa0: 6572 746f 6f6c 2e68 746d 6c3a 360a 233a  ertool.html:6.#:
+0000fab0: 2061 6c6c 6961 6e63 6561 7574 682f 7365   allianceauth/se
+0000fac0: 7276 6963 6573 2f74 656d 706c 6174 6573  rvices/templates
+0000fad0: 2f73 6572 7669 6365 732f 666c 6565 7466  /services/fleetf
+0000fae0: 6f72 6d61 7474 6572 746f 6f6c 2e68 746d  ormattertool.htm
+0000faf0: 6c3a 3130 0a6d 7367 6964 2022 466c 6565  l:10.msgid "Flee
+0000fb00: 7420 466f 726d 6174 7465 7220 546f 6f6c  t Formatter Tool
+0000fb10: 220a 6d73 6773 7472 2022 220a 0a23 3a20  ".msgstr ""..#: 
+0000fb20: 616c 6c69 616e 6365 6175 7468 2f73 6572  allianceauth/ser
+0000fb30: 7669 6365 732f 7465 6d70 6c61 7465 732f  vices/templates/
+0000fb40: 7365 7276 6963 6573 2f66 6c65 6574 666f  services/fleetfo
+0000fb50: 726d 6174 7465 7274 6f6f 6c2e 6874 6d6c  rmattertool.html
+0000fb60: 3a31 380a 6d73 6769 6420 2246 6c65 6574  :18.msgid "Fleet
+0000fb70: 2044 6574 6169 6c73 220a 6d73 6773 7472   Details".msgstr
+0000fb80: 2022 220a 0a23 3a20 616c 6c69 616e 6365   ""..#: alliance
+0000fb90: 6175 7468 2f73 6572 7669 6365 732f 7465  auth/services/te
+0000fba0: 6d70 6c61 7465 732f 7365 7276 6963 6573  mplates/services
+0000fbb0: 2f66 6c65 6574 666f 726d 6174 7465 7274  /fleetformattert
+0000fbc0: 6f6f 6c2e 6874 6d6c 3a33 370a 6d73 6769  ool.html:37.msgi
+0000fbd0: 6420 2246 6f72 6d61 7422 0a6d 7367 7374  d "Format".msgst
+0000fbe0: 7220 2222 0a0a 233a 2061 6c6c 6961 6e63  r ""..#: allianc
+0000fbf0: 6561 7574 682f 7365 7276 6963 6573 2f74  eauth/services/t
+0000fc00: 656d 706c 6174 6573 2f73 6572 7669 6365  emplates/service
+0000fc10: 732f 7365 7276 6963 655f 636f 6e66 6972  s/service_confir
+0000fc20: 6d5f 6465 6c65 7465 2e68 746d 6c3a 360a  m_delete.html:6.
+0000fc30: 233a 2061 6c6c 6961 6e63 6561 7574 682f  #: allianceauth/
+0000fc40: 7365 7276 6963 6573 2f74 656d 706c 6174  services/templat
+0000fc50: 6573 2f73 6572 7669 6365 732f 7365 7276  es/services/serv
+0000fc60: 6963 655f 636f 6e66 6972 6d5f 6465 6c65  ice_confirm_dele
+0000fc70: 7465 2e68 746d 6c3a 3136 0a23 2c20 7079  te.html:16.#, py
+0000fc80: 7468 6f6e 2d66 6f72 6d61 740a 6d73 6769  thon-format.msgi
+0000fc90: 6420 2244 656c 6574 6520 2528 7365 7276  d "Delete %(serv
+0000fca0: 6963 655f 6e61 6d65 2973 2041 6363 6f75  ice_name)s Accou
+0000fcb0: 6e74 3f22 0a6d 7367 7374 7220 2222 0a0a  nt?".msgstr ""..
+0000fcc0: 233a 2061 6c6c 6961 6e63 6561 7574 682f  #: allianceauth/
+0000fcd0: 7365 7276 6963 6573 2f74 656d 706c 6174  services/templat
+0000fce0: 6573 2f73 6572 7669 6365 732f 7365 7276  es/services/serv
+0000fcf0: 6963 655f 636f 6e66 6972 6d5f 6465 6c65  ice_confirm_dele
+0000fd00: 7465 2e68 746d 6c3a 3130 0a23 3a20 616c  te.html:10.#: al
+0000fd10: 6c69 616e 6365 6175 7468 2f73 6572 7669  lianceauth/servi
+0000fd20: 6365 732f 7465 6d70 6c61 7465 732f 7365  ces/templates/se
+0000fd30: 7276 6963 6573 2f73 6572 7669 6365 5f63  rvices/service_c
+0000fd40: 7265 6465 6e74 6961 6c73 2e68 746d 6c3a  redentials.html:
+0000fd50: 3130 0a23 3a20 616c 6c69 616e 6365 6175  10.#: allianceau
+0000fd60: 7468 2f73 6572 7669 6365 732f 7465 6d70  th/services/temp
+0000fd70: 6c61 7465 732f 7365 7276 6963 6573 2f73  lates/services/s
+0000fd80: 6572 7669 6365 5f70 6173 7377 6f72 642e  ervice_password.
+0000fd90: 6874 6d6c 3a31 310a 233a 2061 6c6c 6961  html:11.#: allia
+0000fda0: 6e63 6561 7574 682f 7365 7276 6963 6573  nceauth/services
+0000fdb0: 2f74 656d 706c 6174 6573 2f73 6572 7669  /templates/servi
+0000fdc0: 6365 732f 7365 7276 6963 6573 2e68 746d  ces/services.htm
+0000fdd0: 6c3a 390a 6d73 6769 6420 2241 7661 696c  l:9.msgid "Avail
+0000fde0: 6162 6c65 2053 6572 7669 6365 7322 0a6d  able Services".m
+0000fdf0: 7367 7374 7220 2222 0a0a 233a 2061 6c6c  sgstr ""..#: all
+0000fe00: 6961 6e63 6561 7574 682f 7365 7276 6963  ianceauth/servic
+0000fe10: 6573 2f74 656d 706c 6174 6573 2f73 6572  es/templates/ser
+0000fe20: 7669 6365 732f 7365 7276 6963 655f 636f  vices/service_co
+0000fe30: 6e66 6972 6d5f 6465 6c65 7465 2e68 746d  nfirm_delete.htm
+0000fe40: 6c3a 3234 0a23 2c20 7079 7468 6f6e 2d66  l:24.#, python-f
+0000fe50: 6f72 6d61 740a 6d73 6769 6420 2222 0a22  ormat.msgid ""."
+0000fe60: 4172 6520 796f 7520 7375 7265 2079 6f75  Are you sure you
+0000fe70: 2077 616e 7420 746f 2064 656c 6574 6520   want to delete 
+0000fe80: 796f 7572 2025 2873 6572 7669 6365 5f6e  your %(service_n
+0000fe90: 616d 6529 7320 6163 636f 756e 7420 2528  ame)s account %(
+0000fea0: 6f62 6a65 6374 2973 3f22 0a6d 7367 7374  object)s?".msgst
+0000feb0: 7220 2222 0a0a 233a 2061 6c6c 6961 6e63  r ""..#: allianc
+0000fec0: 6561 7574 682f 7365 7276 6963 6573 2f74  eauth/services/t
+0000fed0: 656d 706c 6174 6573 2f73 6572 7669 6365  emplates/service
+0000fee0: 732f 7365 7276 6963 655f 6372 6564 656e  s/service_creden
+0000fef0: 7469 616c 732e 6874 6d6c 3a36 0a23 3a20  tials.html:6.#: 
+0000ff00: 616c 6c69 616e 6365 6175 7468 2f73 6572  allianceauth/ser
+0000ff10: 7669 6365 732f 7465 6d70 6c61 7465 732f  vices/templates/
+0000ff20: 7365 7276 6963 6573 2f73 6572 7669 6365  services/service
+0000ff30: 5f63 7265 6465 6e74 6961 6c73 2e68 746d  _credentials.htm
+0000ff40: 6c3a 3136 0a23 2c20 7079 7468 6f6e 2d66  l:16.#, python-f
+0000ff50: 6f72 6d61 740a 6d73 6769 6420 2225 2873  ormat.msgid "%(s
+0000ff60: 6572 7669 6365 5f6e 616d 6529 7320 4372  ervice_name)s Cr
+0000ff70: 6564 656e 7469 616c 7322 0a6d 7367 7374  edentials".msgst
+0000ff80: 7220 2222 0a0a 233a 2061 6c6c 6961 6e63  r ""..#: allianc
+0000ff90: 6561 7574 682f 7365 7276 6963 6573 2f74  eauth/services/t
+0000ffa0: 656d 706c 6174 6573 2f73 6572 7669 6365  emplates/service
+0000ffb0: 732f 7365 7276 6963 655f 7061 7373 776f  s/service_passwo
+0000ffc0: 7264 2e68 746d 6c3a 370a 232c 2070 7974  rd.html:7.#, pyt
+0000ffd0: 686f 6e2d 666f 726d 6174 0a6d 7367 6964  hon-format.msgid
+0000ffe0: 2022 2528 7365 7276 6963 655f 6e61 6d65   "%(service_name
+0000fff0: 2973 2050 6173 7377 6f72 6420 4368 616e  )s Password Chan
+00010000: 6765 220a 6d73 6773 7472 2022 220a 0a23  ge".msgstr ""..#
+00010010: 3a20 616c 6c69 616e 6365 6175 7468 2f73  : allianceauth/s
+00010020: 6572 7669 6365 732f 7465 6d70 6c61 7465  ervices/template
+00010030: 732f 7365 7276 6963 6573 2f73 6572 7669  s/services/servi
+00010040: 6365 5f70 6173 7377 6f72 642e 6874 6d6c  ce_password.html
+00010050: 3a31 370a 232c 2070 7974 686f 6e2d 666f  :17.#, python-fo
+00010060: 726d 6174 0a6d 7367 6964 2022 5365 7420  rmat.msgid "Set 
+00010070: 2528 7365 7276 6963 655f 6e61 6d65 2973  %(service_name)s
+00010080: 2050 6173 7377 6f72 6422 0a6d 7367 7374   Password".msgst
+00010090: 7220 2222 0a0a 233a 2061 6c6c 6961 6e63  r ""..#: allianc
+000100a0: 6561 7574 682f 7365 7276 6963 6573 2f74  eauth/services/t
+000100b0: 656d 706c 6174 6573 2f73 6572 7669 6365  emplates/service
+000100c0: 732f 7365 7276 6963 655f 7374 6174 7573  s/service_status
+000100d0: 2e68 746d 6c3a 350a 6d73 6769 6420 2245  .html:5.msgid "E
+000100e0: 6e61 626c 6564 220a 6d73 6773 7472 2022  nabled".msgstr "
+000100f0: 220a 0a23 3a20 616c 6c69 616e 6365 6175  "..#: allianceau
+00010100: 7468 2f73 6572 7669 6365 732f 7465 6d70  th/services/temp
+00010110: 6c61 7465 732f 7365 7276 6963 6573 2f73  lates/services/s
+00010120: 6572 7669 6365 5f73 7461 7475 732e 6874  ervice_status.ht
+00010130: 6d6c 3a37 0a23 3a20 616c 6c69 616e 6365  ml:7.#: alliance
+00010140: 6175 7468 2f73 7270 2f74 656d 706c 6174  auth/srp/templat
+00010150: 6573 2f73 7270 2f6d 616e 6167 656d 656e  es/srp/managemen
+00010160: 742e 6874 6d6c 3a37 380a 6d73 6769 6420  t.html:78.msgid 
+00010170: 2244 6973 6162 6c65 6422 0a6d 7367 7374  "Disabled".msgst
+00010180: 7220 2222 0a0a 233a 2061 6c6c 6961 6e63  r ""..#: allianc
+00010190: 6561 7574 682f 7365 7276 6963 6573 2f74  eauth/services/t
+000101a0: 656d 706c 6174 6573 2f73 6572 7669 6365  emplates/service
+000101b0: 732f 7365 7276 6963 6573 2e68 746d 6c3a  s/services.html:
+000101c0: 350a 6d73 6769 6420 2253 6572 7669 6365  5.msgid "Service
+000101d0: 7320 4d61 6e61 6765 6d65 6e74 220a 6d73  s Management".ms
+000101e0: 6773 7472 2022 220a 0a23 3a20 616c 6c69  gstr ""..#: alli
+000101f0: 616e 6365 6175 7468 2f73 6572 7669 6365  anceauth/service
+00010200: 732f 7465 6d70 6c61 7465 732f 7365 7276  s/templates/serv
+00010210: 6963 6573 2f73 6572 7669 6365 732e 6874  ices/services.ht
+00010220: 6d6c 3a32 300a 6d73 6769 6420 224c 6567  ml:20.msgid "Leg
+00010230: 656e 6422 0a6d 7367 7374 7220 2222 0a0a  end".msgstr ""..
+00010240: 233a 2061 6c6c 6961 6e63 6561 7574 682f  #: allianceauth/
+00010250: 7365 7276 6963 6573 2f74 656d 706c 6174  services/templat
+00010260: 6573 2f73 6572 7669 6365 732f 7365 7276  es/services/serv
+00010270: 6963 6573 2e68 746d 6c3a 3237 0a6d 7367  ices.html:27.msg
+00010280: 6964 2022 436c 6963 6b20 746f 2061 6374  id "Click to act
+00010290: 6976 6174 6520 7468 6520 7365 7276 6963  ivate the servic
+000102a0: 6520 666f 7220 796f 7572 2075 7365 722e  e for your user.
+000102b0: 220a 6d73 6773 7472 2022 220a 0a23 3a20  ".msgstr ""..#: 
+000102c0: 616c 6c69 616e 6365 6175 7468 2f73 6572  allianceauth/ser
+000102d0: 7669 6365 732f 7465 6d70 6c61 7465 732f  vices/templates/
+000102e0: 7365 7276 6963 6573 2f73 6572 7669 6365  services/service
+000102f0: 732e 6874 6d6c 3a33 360a 6d73 6769 6420  s.html:36.msgid 
+00010300: 2243 6c69 636b 2074 6f20 6d61 6e75 616c  "Click to manual
+00010310: 6c79 2073 6574 2079 6f75 7220 7061 7373  ly set your pass
+00010320: 776f 7264 2e22 0a6d 7367 7374 7220 2222  word.".msgstr ""
+00010330: 0a0a 233a 2061 6c6c 6961 6e63 6561 7574  ..#: allianceaut
+00010340: 682f 7365 7276 6963 6573 2f74 656d 706c  h/services/templ
+00010350: 6174 6573 2f73 6572 7669 6365 732f 7365  ates/services/se
+00010360: 7276 6963 6573 2e68 746d 6c3a 3435 0a6d  rvices.html:45.m
+00010370: 7367 6964 2022 436c 6963 6b20 746f 2072  sgid "Click to r
+00010380: 616e 646f 6d6c 7920 6765 6e65 7261 7465  andomly generate
+00010390: 2079 6f75 7220 7061 7373 776f 7264 2e22   your password."
+000103a0: 0a6d 7367 7374 7220 2222 0a0a 233a 2061  .msgstr ""..#: a
+000103b0: 6c6c 6961 6e63 6561 7574 682f 7365 7276  llianceauth/serv
+000103c0: 6963 6573 2f74 656d 706c 6174 6573 2f73  ices/templates/s
+000103d0: 6572 7669 6365 732f 7365 7276 6963 6573  ervices/services
+000103e0: 2e68 746d 6c3a 3534 0a6d 7367 6964 2022  .html:54.msgid "
+000103f0: 436c 6963 6b20 746f 2064 6561 6374 6976  Click to deactiv
+00010400: 6174 6520 7468 6520 7365 7276 6963 6520  ate the service 
+00010410: 666f 7220 796f 7572 2075 7365 7222 0a6d  for your user".m
+00010420: 7367 7374 7220 2222 0a0a 233a 2061 6c6c  sgstr ""..#: all
+00010430: 6961 6e63 6561 7574 682f 7365 7276 6963  ianceauth/servic
+00010440: 6573 2f74 656d 706c 6174 6573 2f73 6572  es/templates/ser
+00010450: 7669 6365 732f 7365 7276 6963 6573 2e68  vices/services.h
+00010460: 746d 6c3a 3630 0a6d 7367 6964 2022 220a  tml:60.msgid "".
+00010470: 2253 6f6d 6520 7365 7276 6963 6573 2070  "Some services p
+00010480: 726f 7669 6465 2064 6966 6665 7265 6e74  rovide different
+00010490: 206f 7074 696f 6e73 2e20 486f 7665 7220   options. Hover 
+000104a0: 6f76 6572 2074 6865 2062 7574 746f 6e73  over the buttons
+000104b0: 2074 6f20 7365 6520 6d6f 7265 2e22 0a6d   to see more.".m
+000104c0: 7367 7374 7220 2222 0a0a 233a 2061 6c6c  sgstr ""..#: all
+000104d0: 6961 6e63 6561 7574 682f 7372 702f 6175  ianceauth/srp/au
+000104e0: 7468 5f68 6f6f 6b73 2e70 793a 3134 0a6d  th_hooks.py:14.m
+000104f0: 7367 6964 2022 5368 6970 2052 6570 6c61  sgid "Ship Repla
+00010500: 6365 6d65 6e74 220a 6d73 6773 7472 2022  cement".msgstr "
+00010510: 220a 0a23 3a20 616c 6c69 616e 6365 6175  "..#: allianceau
+00010520: 7468 2f73 7270 2f66 6f72 6d2e 7079 3a39  th/srp/form.py:9
+00010530: 2061 6c6c 6961 6e63 6561 7574 682f 7372   allianceauth/sr
+00010540: 702f 7465 6d70 6c61 7465 732f 7372 702f  p/templates/srp/
+00010550: 6d61 6e61 6765 6d65 6e74 2e68 746d 6c3a  management.html:
+00010560: 3435 0a6d 7367 6964 2022 466c 6565 7420  45.msgid "Fleet 
+00010570: 5469 6d65 220a 6d73 6773 7472 2022 220a  Time".msgstr "".
+00010580: 0a23 3a20 616c 6c69 616e 6365 6175 7468  .#: allianceauth
+00010590: 2f73 7270 2f66 6f72 6d2e 7079 3a31 300a  /srp/form.py:10.
+000105a0: 233a 2061 6c6c 6961 6e63 6561 7574 682f  #: allianceauth/
+000105b0: 7372 702f 7465 6d70 6c61 7465 732f 7372  srp/templates/sr
+000105c0: 702f 6d61 6e61 6765 6d65 6e74 2e68 746d  p/management.htm
+000105d0: 6c3a 3436 0a6d 7367 6964 2022 466c 6565  l:46.msgid "Flee
+000105e0: 7420 446f 6374 7269 6e65 220a 6d73 6773  t Doctrine".msgs
+000105f0: 7472 2022 220a 0a23 3a20 616c 6c69 616e  tr ""..#: allian
+00010600: 6365 6175 7468 2f73 7270 2f66 6f72 6d2e  ceauth/srp/form.
+00010610: 7079 3a31 360a 6d73 6769 6420 224b 696c  py:16.msgid "Kil
+00010620: 6c62 6f61 7264 204c 696e 6b20 287a 6b69  lboard Link (zki
+00010630: 6c6c 626f 6172 642e 636f 6d20 6f72 206b  llboard.com or k
+00010640: 622e 6576 6574 6f6f 6c73 2e6f 7267 2922  b.evetools.org)"
+00010650: 0a6d 7367 7374 7220 2222 0a0a 233a 2061  .msgstr ""..#: a
+00010660: 6c6c 6961 6e63 6561 7574 682f 7372 702f  llianceauth/srp/
+00010670: 666f 726d 2e70 793a 3334 0a6d 7367 6964  form.py:34.msgid
+00010680: 2022 496e 7661 6c69 6420 4c69 6e6b 2e20   "Invalid Link. 
+00010690: 506c 6561 7365 2075 7365 207a 6b69 6c6c  Please use zkill
+000106a0: 626f 6172 642e 636f 6d20 6f72 206b 622e  board.com or kb.
+000106b0: 6576 6574 6f6f 6c73 2e6f 7267 220a 6d73  evetools.org".ms
+000106c0: 6773 7472 2022 220a 0a23 3a20 616c 6c69  gstr ""..#: alli
+000106d0: 616e 6365 6175 7468 2f73 7270 2f66 6f72  anceauth/srp/for
+000106e0: 6d2e 7079 3a34 360a 6d73 6769 6420 2249  m.py:46.msgid "I
+000106f0: 6e76 616c 6964 204c 696e 6b2e 2050 6c65  nvalid Link. Ple
+00010700: 6173 6520 706f 7374 2061 2064 6972 6563  ase post a direc
+00010710: 7420 6c69 6e6b 2074 6f20 6120 6b69 6c6c  t link to a kill
+00010720: 6d61 696c 2e22 0a6d 7367 7374 7220 2222  mail.".msgstr ""
+00010730: 0a0a 233a 2061 6c6c 6961 6e63 6561 7574  ..#: allianceaut
+00010740: 682f 7372 702f 666f 726d 2e70 793a 3533  h/srp/form.py:53
+00010750: 0a6d 7367 6964 2022 4166 7465 7220 4163  .msgid "After Ac
+00010760: 7469 6f6e 2052 6570 6f72 7420 4c69 6e6b  tion Report Link
+00010770: 220a 6d73 6773 7472 2022 220a 0a23 3a20  ".msgstr ""..#: 
+00010780: 616c 6c69 616e 6365 6175 7468 2f73 7270  allianceauth/srp
+00010790: 2f74 656d 706c 6174 6573 2f73 7270 2f61  /templates/srp/a
+000107a0: 6464 2e68 746d 6c3a 370a 6d73 6769 6420  dd.html:7.msgid 
+000107b0: 2253 5250 2046 6c65 6574 2043 7265 6174  "SRP Fleet Creat
+000107c0: 6522 0a6d 7367 7374 7220 2222 0a0a 233a  e".msgstr ""..#:
+000107d0: 2061 6c6c 6961 6e63 6561 7574 682f 7372   allianceauth/sr
+000107e0: 702f 7465 6d70 6c61 7465 732f 7372 702f  p/templates/srp/
+000107f0: 6164 642e 6874 6d6c 3a31 310a 233a 2061  add.html:11.#: a
+00010800: 6c6c 6961 6e63 6561 7574 682f 7372 702f  llianceauth/srp/
+00010810: 7465 6d70 6c61 7465 732f 7372 702f 6461  templates/srp/da
+00010820: 7461 2e68 746d 6c3a 3131 0a23 3a20 616c  ta.html:11.#: al
+00010830: 6c69 616e 6365 6175 7468 2f73 7270 2f74  lianceauth/srp/t
+00010840: 656d 706c 6174 6573 2f73 7270 2f6d 616e  emplates/srp/man
+00010850: 6167 656d 656e 742e 6874 6d6c 3a31 310a  agement.html:11.
+00010860: 233a 2061 6c6c 6961 6e63 6561 7574 682f  #: allianceauth/
+00010870: 7372 702f 7465 6d70 6c61 7465 732f 7372  srp/templates/sr
+00010880: 702f 7265 7175 6573 742e 6874 6d6c 3a31  p/request.html:1
+00010890: 310a 233a 2061 6c6c 6961 6e63 6561 7574  1.#: allianceaut
+000108a0: 682f 7372 702f 7465 6d70 6c61 7465 732f  h/srp/templates/
+000108b0: 7372 702f 7570 6461 7465 2e68 746d 6c3a  srp/update.html:
+000108c0: 3131 0a6d 7367 6964 2022 5368 6970 2052  11.msgid "Ship R
+000108d0: 6570 6c61 6365 6d65 6e74 2050 726f 6772  eplacement Progr
+000108e0: 616d 220a 6d73 6773 7472 2022 220a 0a23  am".msgstr ""..#
+000108f0: 3a20 616c 6c69 616e 6365 6175 7468 2f73  : allianceauth/s
+00010900: 7270 2f74 656d 706c 6174 6573 2f73 7270  rp/templates/srp
+00010910: 2f61 6464 2e68 746d 6c3a 3230 0a6d 7367  /add.html:20.msg
+00010920: 6964 2022 4372 6561 7465 2053 5250 2046  id "Create SRP F
+00010930: 6c65 6574 220a 6d73 6773 7472 2022 220a  leet".msgstr "".
+00010940: 0a23 3a20 616c 6c69 616e 6365 6175 7468  .#: allianceauth
+00010950: 2f73 7270 2f74 656d 706c 6174 6573 2f73  /srp/templates/s
+00010960: 7270 2f61 6464 2e68 746d 6c3a 3236 0a6d  rp/add.html:26.m
+00010970: 7367 6964 2022 5352 5020 666c 6565 7420  sgid "SRP fleet 
+00010980: 6465 7461 696c 7322 0a6d 7367 7374 7220  details".msgstr 
+00010990: 2222 0a0a 233a 2061 6c6c 6961 6e63 6561  ""..#: alliancea
+000109a0: 7574 682f 7372 702f 7465 6d70 6c61 7465  uth/srp/template
+000109b0: 732f 7372 702f 6164 642e 6874 6d6c 3a34  s/srp/add.html:4
+000109c0: 300a 6d73 6769 6420 2243 7265 6174 6520  0.msgid "Create 
+000109d0: 5352 5020 666c 6565 7422 0a6d 7367 7374  SRP fleet".msgst
+000109e0: 7220 2222 0a0a 233a 2061 6c6c 6961 6e63  r ""..#: allianc
+000109f0: 6561 7574 682f 7372 702f 7465 6d70 6c61  eauth/srp/templa
+00010a00: 7465 732f 7372 702f 6164 642e 6874 6d6c  tes/srp/add.html
+00010a10: 3a34 360a 6d73 6769 6420 2247 6976 6520  :46.msgid "Give 
+00010a20: 7468 6973 206c 696e 6b20 746f 2074 6865  this link to the
+00010a30: 206c 696e 6520 6d65 6d62 6572 732e 220a   line members.".
+00010a40: 6d73 6773 7472 2022 220a 0a23 3a20 616c  msgstr ""..#: al
+00010a50: 6c69 616e 6365 6175 7468 2f73 7270 2f74  lianceauth/srp/t
+00010a60: 656d 706c 6174 6573 2f73 7270 2f64 6174  emplates/srp/dat
+00010a70: 612e 6874 6d6c 3a37 0a23 3a20 616c 6c69  a.html:7.#: alli
+00010a80: 616e 6365 6175 7468 2f73 7270 2f74 656d  anceauth/srp/tem
+00010a90: 706c 6174 6573 2f73 7270 2f64 6174 612e  plates/srp/data.
+00010aa0: 6874 6d6c 3a33 380a 6d73 6769 6420 2253  html:38.msgid "S
+00010ab0: 5250 2046 6c65 6574 2044 6174 6122 0a6d  RP Fleet Data".m
+00010ac0: 7367 7374 7220 2222 0a0a 233a 2061 6c6c  sgstr ""..#: all
+00010ad0: 6961 6e63 6561 7574 682f 7372 702f 7465  ianceauth/srp/te
+00010ae0: 6d70 6c61 7465 732f 7372 702f 6461 7461  mplates/srp/data
+00010af0: 2e68 746d 6c3a 3136 0a6d 7367 6964 2022  .html:16.msgid "
+00010b00: 5669 6577 2046 6c65 6574 7322 0a6d 7367  View Fleets".msg
+00010b10: 7374 7220 2222 0a0a 233a 2061 6c6c 6961  str ""..#: allia
+00010b20: 6e63 6561 7574 682f 7372 702f 7465 6d70  nceauth/srp/temp
+00010b30: 6c61 7465 732f 7372 702f 6461 7461 2e68  lates/srp/data.h
+00010b40: 746d 6c3a 3235 0a6d 7367 6964 2022 4d61  tml:25.msgid "Ma
+00010b50: 726b 2049 6e63 6f6d 706c 6574 6522 0a6d  rk Incomplete".m
+00010b60: 7367 7374 7220 2222 0a0a 233a 2061 6c6c  sgstr ""..#: all
+00010b70: 6961 6e63 6561 7574 682f 7372 702f 7465  ianceauth/srp/te
+00010b80: 6d70 6c61 7465 732f 7372 702f 6461 7461  mplates/srp/data
+00010b90: 2e68 746d 6c3a 3239 0a6d 7367 6964 2022  .html:29.msgid "
+00010ba0: 4d61 726b 2043 6f6d 706c 6574 6564 220a  Mark Completed".
+00010bb0: 6d73 6773 7472 2022 220a 0a23 3a20 616c  msgstr ""..#: al
+00010bc0: 6c69 616e 6365 6175 7468 2f73 7270 2f74  lianceauth/srp/t
+00010bd0: 656d 706c 6174 6573 2f73 7270 2f64 6174  emplates/srp/dat
+00010be0: 612e 6874 6d6c 3a34 370a 233a 2061 6c6c  a.html:47.#: all
+00010bf0: 6961 6e63 6561 7574 682f 7372 702f 7465  ianceauth/srp/te
+00010c00: 6d70 6c61 7465 732f 7372 702f 6461 7461  mplates/srp/data
+00010c10: 2e68 746d 6c3a 3133 380a 6d73 6769 6420  .html:138.msgid 
+00010c20: 2254 6f74 616c 204c 6f73 7365 733a 220a  "Total Losses:".
+00010c30: 6d73 6773 7472 2022 220a 0a23 3a20 616c  msgstr ""..#: al
+00010c40: 6c69 616e 6365 6175 7468 2f73 7270 2f74  lianceauth/srp/t
+00010c50: 656d 706c 6174 6573 2f73 7270 2f64 6174  emplates/srp/dat
+00010c60: 612e 6874 6d6c 3a34 380a 233a 2061 6c6c  a.html:48.#: all
+00010c70: 6961 6e63 6561 7574 682f 7372 702f 7465  ianceauth/srp/te
+00010c80: 6d70 6c61 7465 732f 7372 702f 6461 7461  mplates/srp/data
+00010c90: 2e68 746d 6c3a 3133 390a 233a 2061 6c6c  .html:139.#: all
+00010ca0: 6961 6e63 6561 7574 682f 7372 702f 7465  ianceauth/srp/te
+00010cb0: 6d70 6c61 7465 732f 7372 702f 6d61 6e61  mplates/srp/mana
+00010cc0: 6765 6d65 6e74 2e68 746d 6c3a 3336 0a6d  gement.html:36.m
+00010cd0: 7367 6964 2022 546f 7461 6c20 4953 4b20  sgid "Total ISK 
+00010ce0: 436f 7374 3a22 0a6d 7367 7374 7220 2222  Cost:".msgstr ""
+00010cf0: 0a0a 233a 2061 6c6c 6961 6e63 6561 7574  ..#: allianceaut
+00010d00: 682f 7372 702f 7465 6d70 6c61 7465 732f  h/srp/templates/
+00010d10: 7372 702f 6461 7461 2e68 746d 6c3a 3539  srp/data.html:59
+00010d20: 0a23 3a20 616c 6c69 616e 6365 6175 7468  .#: allianceauth
+00010d30: 2f73 7270 2f74 656d 706c 6174 6573 2f73  /srp/templates/s
+00010d40: 7270 2f64 6174 612e 6874 6d6c 3a31 3530  rp/data.html:150
+00010d50: 0a6d 7367 6964 2022 4172 6520 796f 7520  .msgid "Are you 
+00010d60: 7375 7265 2079 6f75 2077 616e 7420 746f  sure you want to
+00010d70: 2064 656c 6574 6520 5352 5020 7265 7175   delete SRP requ
+00010d80: 6573 7473 3f22 0a6d 7367 7374 7220 2222  ests?".msgstr ""
+00010d90: 0a0a 233a 2061 6c6c 6961 6e63 6561 7574  ..#: allianceaut
+00010da0: 682f 7372 702f 7465 6d70 6c61 7465 732f  h/srp/templates/
+00010db0: 7372 702f 6461 7461 2e68 746d 6c3a 3639  srp/data.html:69
+00010dc0: 0a6d 7367 6964 2022 5069 6c6f 7420 4e61  .msgid "Pilot Na
+00010dd0: 6d65 220a 6d73 6773 7472 2022 220a 0a23  me".msgstr ""..#
+00010de0: 3a20 616c 6c69 616e 6365 6175 7468 2f73  : allianceauth/s
+00010df0: 7270 2f74 656d 706c 6174 6573 2f73 7270  rp/templates/srp
+00010e00: 2f64 6174 612e 6874 6d6c 3a37 300a 6d73  /data.html:70.ms
+00010e10: 6769 6420 224b 696c 6c62 6f61 7264 204c  gid "Killboard L
+00010e20: 696e 6b22 0a6d 7367 7374 7220 2222 0a0a  ink".msgstr ""..
+00010e30: 233a 2061 6c6c 6961 6e63 6561 7574 682f  #: allianceauth/
+00010e40: 7372 702f 7465 6d70 6c61 7465 732f 7372  srp/templates/sr
+00010e50: 702f 6461 7461 2e68 746d 6c3a 3732 0a6d  p/data.html:72.m
+00010e60: 7367 6964 2022 5368 6970 2054 7970 6522  sgid "Ship Type"
+00010e70: 0a6d 7367 7374 7220 2222 0a0a 233a 2061  .msgstr ""..#: a
+00010e80: 6c6c 6961 6e63 6561 7574 682f 7372 702f  llianceauth/srp/
+00010e90: 7465 6d70 6c61 7465 732f 7372 702f 6461  templates/srp/da
+00010ea0: 7461 2e68 746d 6c3a 3733 0a6d 7367 6964  ta.html:73.msgid
+00010eb0: 2022 4b69 6c6c 626f 6172 6420 4c6f 7373   "Killboard Loss
+00010ec0: 2041 6d74 220a 6d73 6773 7472 2022 220a   Amt".msgstr "".
+00010ed0: 0a23 3a20 616c 6c69 616e 6365 6175 7468  .#: allianceauth
+00010ee0: 2f73 7270 2f74 656d 706c 6174 6573 2f73  /srp/templates/s
+00010ef0: 7270 2f64 6174 612e 6874 6d6c 3a37 350a  rp/data.html:75.
+00010f00: 6d73 6769 6420 2253 5250 2049 534b 2043  msgid "SRP ISK C
+00010f10: 6f73 7422 0a6d 7367 7374 7220 2222 0a0a  ost".msgstr ""..
+00010f20: 233a 2061 6c6c 6961 6e63 6561 7574 682f  #: allianceauth/
+00010f30: 7372 702f 7465 6d70 6c61 7465 732f 7372  srp/templates/sr
+00010f40: 702f 6461 7461 2e68 746d 6c3a 3736 0a6d  p/data.html:76.m
+00010f50: 7367 6964 2022 436c 6963 6b20 7661 6c75  sgid "Click valu
+00010f60: 6520 746f 2065 6469 7420 456e 7465 7220  e to edit Enter 
+00010f70: 746f 2073 6176 6520 2620 6e65 7874 2045  to save & next E
+00010f80: 5343 2074 6f20 6361 6e63 656c 220a 6d73  SC to cancel".ms
+00010f90: 6773 7472 2022 220a 0a23 3a20 616c 6c69  gstr ""..#: alli
+00010fa0: 616e 6365 6175 7468 2f73 7270 2f74 656d  anceauth/srp/tem
+00010fb0: 706c 6174 6573 2f73 7270 2f64 6174 612e  plates/srp/data.
+00010fc0: 6874 6d6c 3a37 390a 6d73 6769 6420 2250  html:79.msgid "P
+00010fd0: 6f73 7420 5469 6d65 220a 6d73 6773 7472  ost Time".msgstr
+00010fe0: 2022 220a 0a23 3a20 616c 6c69 616e 6365   ""..#: alliance
+00010ff0: 6175 7468 2f73 7270 2f74 656d 706c 6174  auth/srp/templat
+00011000: 6573 2f73 7270 2f64 6174 612e 6874 6d6c  es/srp/data.html
+00011010: 3a39 380a 233a 2061 6c6c 6961 6e63 6561  :98.#: alliancea
+00011020: 7574 682f 7372 702f 7465 6d70 6c61 7465  uth/srp/template
+00011030: 732f 7372 702f 6d61 6e61 6765 6d65 6e74  s/srp/management
+00011040: 2e68 746d 6c3a 3730 0a6d 7367 6964 2022  .html:70.msgid "
+00011050: 4c69 6e6b 220a 6d73 6773 7472 2022 220a  Link".msgstr "".
+00011060: 0a23 3a20 616c 6c69 616e 6365 6175 7468  .#: allianceauth
+00011070: 2f73 7270 2f74 656d 706c 6174 6573 2f73  /srp/templates/s
+00011080: 7270 2f64 6174 612e 6874 6d6c 3a31 3539  rp/data.html:159
+00011090: 0a6d 7367 6964 2022 4e6f 2053 5250 2072  .msgid "No SRP r
+000110a0: 6571 7565 7374 7320 666f 7220 7468 6973  equests for this
+000110b0: 2066 6c65 6574 2e22 0a6d 7367 7374 7220   fleet.".msgstr 
+000110c0: 2222 0a0a 233a 2061 6c6c 6961 6e63 6561  ""..#: alliancea
+000110d0: 7574 682f 7372 702f 7465 6d70 6c61 7465  uth/srp/template
+000110e0: 732f 7372 702f 6d61 6e61 6765 6d65 6e74  s/srp/management
+000110f0: 2e68 746d 6c3a 370a 6d73 6769 6420 2253  .html:7.msgid "S
+00011100: 5250 204d 616e 6167 656d 656e 7422 0a6d  RP Management".m
+00011110: 7367 7374 7220 2222 0a0a 233a 2061 6c6c  sgstr ""..#: all
+00011120: 6961 6e63 6561 7574 682f 7372 702f 7465  ianceauth/srp/te
+00011130: 6d70 6c61 7465 732f 7372 702f 6d61 6e61  mplates/srp/mana
+00011140: 6765 6d65 6e74 2e68 746d 6c3a 3138 0a6d  gement.html:18.m
+00011150: 7367 6964 2022 5669 6577 2041 6c6c 220a  sgid "View All".
+00011160: 6d73 6773 7472 2022 220a 0a23 3a20 616c  msgstr ""..#: al
+00011170: 6c69 616e 6365 6175 7468 2f73 7270 2f74  lianceauth/srp/t
+00011180: 656d 706c 6174 6573 2f73 7270 2f6d 616e  emplates/srp/man
+00011190: 6167 656d 656e 742e 6874 6d6c 3a32 370a  agement.html:27.
+000111a0: 6d73 6769 6420 2241 6464 2053 5250 2046  msgid "Add SRP F
+000111b0: 6c65 6574 220a 6d73 6773 7472 2022 220a  leet".msgstr "".
+000111c0: 0a23 3a20 616c 6c69 616e 6365 6175 7468  .#: allianceauth
+000111d0: 2f73 7270 2f74 656d 706c 6174 6573 2f73  /srp/templates/s
+000111e0: 7270 2f6d 616e 6167 656d 656e 742e 6874  rp/management.ht
+000111f0: 6d6c 3a34 380a 6d73 6769 6420 2246 6c65  ml:48.msgid "Fle
+00011200: 6574 2041 4152 220a 6d73 6773 7472 2022  et AAR".msgstr "
+00011210: 220a 0a23 3a20 616c 6c69 616e 6365 6175  "..#: allianceau
+00011220: 7468 2f73 7270 2f74 656d 706c 6174 6573  th/srp/templates
+00011230: 2f73 7270 2f6d 616e 6167 656d 656e 742e  /srp/management.
+00011240: 6874 6d6c 3a34 390a 6d73 6769 6420 2246  html:49.msgid "F
+00011250: 6c65 6574 2053 5250 2043 6f64 6522 0a6d  leet SRP Code".m
+00011260: 7367 7374 7220 2222 0a0a 233a 2061 6c6c  sgstr ""..#: all
+00011270: 6961 6e63 6561 7574 682f 7372 702f 7465  ianceauth/srp/te
+00011280: 6d70 6c61 7465 732f 7372 702f 6d61 6e61  mplates/srp/mana
+00011290: 6765 6d65 6e74 2e68 746d 6c3a 3530 0a6d  gement.html:50.m
+000112a0: 7367 6964 2022 466c 6565 7420 4953 4b20  sgid "Fleet ISK 
+000112b0: 436f 7374 220a 6d73 6773 7472 2022 220a  Cost".msgstr "".
+000112c0: 0a23 3a20 616c 6c69 616e 6365 6175 7468  .#: allianceauth
+000112d0: 2f73 7270 2f74 656d 706c 6174 6573 2f73  /srp/templates/s
+000112e0: 7270 2f6d 616e 6167 656d 656e 742e 6874  rp/management.ht
+000112f0: 6d6c 3a35 310a 6d73 6769 6420 2253 5250  ml:51.msgid "SRP
+00011300: 2053 7461 7475 7322 0a6d 7367 7374 7220   Status".msgstr 
+00011310: 2222 0a0a 233a 2061 6c6c 6961 6e63 6561  ""..#: alliancea
+00011320: 7574 682f 7372 702f 7465 6d70 6c61 7465  uth/srp/template
+00011330: 732f 7372 702f 6d61 6e61 6765 6d65 6e74  s/srp/management
+00011340: 2e68 746d 6c3a 3532 0a6d 7367 6964 2022  .html:52.msgid "
+00011350: 5065 6e64 696e 6720 5265 7175 6573 7473  Pending Requests
+00011360: 220a 6d73 6773 7472 2022 220a 0a23 3a20  ".msgstr ""..#: 
+00011370: 616c 6c69 616e 6365 6175 7468 2f73 7270  allianceauth/srp
+00011380: 2f74 656d 706c 6174 6573 2f73 7270 2f6d  /templates/srp/m
+00011390: 616e 6167 656d 656e 742e 6874 6d6c 3a39  anagement.html:9
+000113a0: 310a 6d73 6769 6420 2243 6f6d 706c 6574  1.msgid "Complet
+000113b0: 6564 220a 6d73 6773 7472 2022 220a 0a23  ed".msgstr ""..#
+000113c0: 3a20 616c 6c69 616e 6365 6175 7468 2f73  : allianceauth/s
+000113d0: 7270 2f74 656d 706c 6174 6573 2f73 7270  rp/templates/srp
+000113e0: 2f6d 616e 6167 656d 656e 742e 6874 6d6c  /management.html
+000113f0: 3a31 3038 0a6d 7367 6964 2022 4172 6520  :108.msgid "Are 
+00011400: 796f 7520 7375 7265 2079 6f75 2077 616e  you sure you wan
+00011410: 7420 746f 2064 656c 6574 6520 7468 6973  t to delete this
+00011420: 2053 5250 2063 6f64 6520 616e 6420 6974   SRP code and it
+00011430: 7320 636f 6e74 656e 7473 3f22 0a6d 7367  s contents?".msg
+00011440: 7374 7220 2222 0a0a 233a 2061 6c6c 6961  str ""..#: allia
+00011450: 6e63 6561 7574 682f 7372 702f 7465 6d70  nceauth/srp/temp
+00011460: 6c61 7465 732f 7372 702f 6d61 6e61 6765  lates/srp/manage
+00011470: 6d65 6e74 2e68 746d 6c3a 3132 390a 6d73  ment.html:129.ms
+00011480: 6769 6420 224e 6f20 5352 5020 666c 6565  gid "No SRP flee
+00011490: 7473 2063 7265 6174 6564 2e22 0a6d 7367  ts created.".msg
+000114a0: 7374 7220 2222 0a0a 233a 2061 6c6c 6961  str ""..#: allia
+000114b0: 6e63 6561 7574 682f 7372 702f 7465 6d70  nceauth/srp/temp
+000114c0: 6c61 7465 732f 7372 702f 7265 7175 6573  lates/srp/reques
+000114d0: 742e 6874 6d6c 3a37 0a6d 7367 6964 2022  t.html:7.msgid "
+000114e0: 5352 5020 5265 7175 6573 7422 0a6d 7367  SRP Request".msg
+000114f0: 7374 7220 2222 0a0a 233a 2061 6c6c 6961  str ""..#: allia
+00011500: 6e63 6561 7574 682f 7372 702f 7465 6d70  nceauth/srp/temp
+00011510: 6c61 7465 732f 7372 702f 7265 7175 6573  lates/srp/reques
+00011520: 742e 6874 6d6c 3a31 360a 6d73 6769 6420  t.html:16.msgid 
+00011530: 2243 7265 6174 6520 5352 5020 5265 7175  "Create SRP Requ
+00011540: 6573 7422 0a6d 7367 7374 7220 2222 0a0a  est".msgstr ""..
+00011550: 233a 2061 6c6c 6961 6e63 6561 7574 682f  #: allianceauth/
+00011560: 7372 702f 7465 6d70 6c61 7465 732f 7372  srp/templates/sr
+00011570: 702f 7265 7175 6573 742e 6874 6d6c 3a32  p/request.html:2
+00011580: 320a 6d73 6769 6420 2259 6f75 7220 5352  2.msgid "Your SR
+00011590: 5020 7265 7175 6573 7422 0a6d 7367 7374  P request".msgst
+000115a0: 7220 2222 0a0a 233a 2061 6c6c 6961 6e63  r ""..#: allianc
+000115b0: 6561 7574 682f 7372 702f 7465 6d70 6c61  eauth/srp/templa
+000115c0: 7465 732f 7372 702f 7265 7175 6573 742e  tes/srp/request.
+000115d0: 6874 6d6c 3a33 350a 6d73 6769 6420 2243  html:35.msgid "C
+000115e0: 7265 6174 6520 5352 5020 7265 7175 6573  reate SRP reques
+000115f0: 7422 0a6d 7367 7374 7220 2222 0a0a 233a  t".msgstr ""..#:
+00011600: 2061 6c6c 6961 6e63 6561 7574 682f 7372   allianceauth/sr
+00011610: 702f 7465 6d70 6c61 7465 732f 7372 702f  p/templates/srp/
+00011620: 7570 6461 7465 2e68 746d 6c3a 370a 233a  update.html:7.#:
+00011630: 2061 6c6c 6961 6e63 6561 7574 682f 7372   allianceauth/sr
+00011640: 702f 7465 6d70 6c61 7465 732f 7372 702f  p/templates/srp/
+00011650: 7570 6461 7465 2e68 746d 6c3a 3136 0a6d  update.html:16.m
+00011660: 7367 6964 2022 5570 6461 7465 2041 4152  sgid "Update AAR
+00011670: 204c 696e 6b22 0a6d 7367 7374 7220 2222   Link".msgstr ""
+00011680: 0a0a 233a 2061 6c6c 6961 6e63 6561 7574  ..#: allianceaut
+00011690: 682f 7372 702f 7465 6d70 6c61 7465 732f  h/srp/templates/
+000116a0: 7372 702f 7570 6461 7465 2e68 746d 6c3a  srp/update.html:
+000116b0: 3232 0a6d 7367 6964 2022 4166 7465 7220  22.msgid "After 
+000116c0: 4163 7469 6f6e 2052 6570 6f72 7422 0a6d  Action Report".m
+000116d0: 7367 7374 7220 2222 0a0a 233a 2061 6c6c  sgstr ""..#: all
+000116e0: 6961 6e63 6561 7574 682f 7372 702f 7465  ianceauth/srp/te
+000116f0: 6d70 6c61 7465 732f 7372 702f 7570 6461  mplates/srp/upda
+00011700: 7465 2e68 746d 6c3a 3331 0a6d 7367 6964  te.html:31.msgid
+00011710: 2022 5352 5020 466c 6565 7420 446f 6573   "SRP Fleet Does
+00011720: 204e 6f74 2045 7869 7374 220a 6d73 6773   Not Exist".msgs
+00011730: 7472 2022 220a 0a23 3a20 616c 6c69 616e  tr ""..#: allian
+00011740: 6365 6175 7468 2f73 7270 2f74 656d 706c  ceauth/srp/templ
+00011750: 6174 6573 2f73 7270 2f75 7064 6174 652e  ates/srp/update.
+00011760: 6874 6d6c 3a34 300a 6d73 6769 6420 2255  html:40.msgid "U
+00011770: 7064 6174 6520 4141 5220 6c69 6e6b 220a  pdate AAR link".
+00011780: 6d73 6773 7472 2022 220a 0a23 3a20 616c  msgstr ""..#: al
+00011790: 6c69 616e 6365 6175 7468 2f73 7270 2f76  lianceauth/srp/v
+000117a0: 6965 7773 2e70 793a 3835 0a23 2c20 7079  iews.py:85.#, py
+000117b0: 7468 6f6e 2d66 6f72 6d61 740a 6d73 6769  thon-format.msgi
+000117c0: 6420 2243 7265 6174 6564 2053 5250 2066  d "Created SRP f
+000117d0: 6c65 6574 2025 2866 6c65 6574 6e61 6d65  leet %(fleetname
+000117e0: 2973 2e22 0a6d 7367 7374 7220 2222 0a0a  )s.".msgstr ""..
+000117f0: 233a 2061 6c6c 6961 6e63 6561 7574 682f  #: allianceauth/
+00011800: 7372 702f 7669 6577 732e 7079 3a31 3033  srp/views.py:103
+00011810: 0a23 2c20 7079 7468 6f6e 2d66 6f72 6d61  .#, python-forma
+00011820: 740a 6d73 6769 6420 2252 656d 6f76 6564  t.msgid "Removed
+00011830: 2053 5250 2066 6c65 6574 2025 2866 6c65   SRP fleet %(fle
+00011840: 6574 6e61 6d65 2973 2e22 0a6d 7367 7374  etname)s.".msgst
+00011850: 7220 2222 0a0a 233a 2061 6c6c 6961 6e63  r ""..#: allianc
+00011860: 6561 7574 682f 7372 702f 7669 6577 732e  eauth/srp/views.
+00011870: 7079 3a31 3135 0a23 2c20 7079 7468 6f6e  py:115.#, python
+00011880: 2d66 6f72 6d61 740a 6d73 6769 6420 2244  -format.msgid "D
+00011890: 6973 6162 6c65 6420 5352 5020 666c 6565  isabled SRP flee
+000118a0: 7420 2528 666c 6565 746e 616d 6529 732e  t %(fleetname)s.
+000118b0: 220a 6d73 6773 7472 2022 220a 0a23 3a20  ".msgstr ""..#: 
+000118c0: 616c 6c69 616e 6365 6175 7468 2f73 7270  allianceauth/srp
+000118d0: 2f76 6965 7773 2e70 793a 3132 370a 232c  /views.py:127.#,
+000118e0: 2070 7974 686f 6e2d 666f 726d 6174 0a6d   python-format.m
+000118f0: 7367 6964 2022 456e 6162 6c65 6420 5352  sgid "Enabled SR
+00011900: 5020 666c 6565 7420 2528 666c 6565 746e  P fleet %(fleetn
+00011910: 616d 6529 732e 220a 6d73 6773 7472 2022  ame)s.".msgstr "
+00011920: 220a 0a23 3a20 616c 6c69 616e 6365 6175  "..#: allianceau
+00011930: 7468 2f73 7270 2f76 6965 7773 2e70 793a  th/srp/views.py:
+00011940: 3134 300a 232c 2070 7974 686f 6e2d 666f  140.#, python-fo
+00011950: 726d 6174 0a6d 7367 6964 2022 4d61 726b  rmat.msgid "Mark
+00011960: 6564 2053 5250 2066 6c65 6574 2025 2866  ed SRP fleet %(f
+00011970: 6c65 6574 6e61 6d65 2973 2061 7320 636f  leetname)s as co
+00011980: 6d70 6c65 7465 642e 220a 6d73 6773 7472  mpleted.".msgstr
+00011990: 2022 220a 0a23 3a20 616c 6c69 616e 6365   ""..#: alliance
+000119a0: 6175 7468 2f73 7270 2f76 6965 7773 2e70  auth/srp/views.p
+000119b0: 793a 3135 330a 232c 2070 7974 686f 6e2d  y:153.#, python-
+000119c0: 666f 726d 6174 0a6d 7367 6964 2022 4d61  format.msgid "Ma
+000119d0: 726b 6564 2053 5250 2066 6c65 6574 2025  rked SRP fleet %
+000119e0: 2866 6c65 6574 6e61 6d65 2973 2061 7320  (fleetname)s as 
+000119f0: 696e 636f 6d70 6c65 7465 2e22 0a6d 7367  incomplete.".msg
+00011a00: 7374 7220 2222 0a0a 233a 2061 6c6c 6961  str ""..#: allia
+00011a10: 6e63 6561 7574 682f 7372 702f 7669 6577  nceauth/srp/view
+00011a20: 732e 7079 3a31 3635 0a23 2c20 7079 7468  s.py:165.#, pyth
+00011a30: 6f6e 2d66 6f72 6d61 740a 6d73 6769 6420  on-format.msgid 
+00011a40: 2255 6e61 626c 6520 746f 206c 6f63 6174  "Unable to locat
+00011a50: 6520 5352 5020 636f 6465 2077 6974 6820  e SRP code with 
+00011a60: 4944 2025 2873 7270 666c 6565 7469 6429  ID %(srpfleetid)
+00011a70: 7322 0a6d 7367 7374 7220 2222 0a0a 233a  s".msgstr ""..#:
+00011a80: 2061 6c6c 6961 6e63 6561 7574 682f 7372   allianceauth/sr
+00011a90: 702f 7669 6577 732e 7079 3a31 3739 0a6d  p/views.py:179.m
+00011aa0: 7367 6964 2022 5468 6973 206b 696c 6c20  sgid "This kill 
+00011ab0: 6d61 696c 2068 6173 2061 6c72 6561 6479  mail has already
+00011ac0: 2062 6565 6e20 706f 7374 6564 2e22 0a6d   been posted.".m
+00011ad0: 7367 7374 7220 2222 0a0a 233a 2061 6c6c  sgstr ""..#: all
+00011ae0: 6961 6e63 6561 7574 682f 7372 702f 7669  ianceauth/srp/vi
+00011af0: 6577 732e 7079 3a32 3030 0a6d 7367 6964  ews.py:200.msgid
+00011b00: 2022 220a 2259 6f75 7220 5352 5020 7265   ""."Your SRP re
+00011b10: 7175 6573 7420 4b69 6c6c 6d61 696c 206c  quest Killmail l
+00011b20: 696e 6b20 6973 2069 6e76 616c 6964 2e20  ink is invalid. 
+00011b30: 506c 6561 7365 206d 616b 6520 7375 7265  Please make sure
+00011b40: 2079 6f75 2061 7265 2075 7369 6e67 2022   you are using "
+00011b50: 0a22 7a4b 696c 6c62 6f61 7264 2e22 0a6d  ."zKillboard.".m
+00011b60: 7367 7374 7220 2222 0a0a 233a 2061 6c6c  sgstr ""..#: all
+00011b70: 6961 6e63 6561 7574 682f 7372 702f 7669  ianceauth/srp/vi
+00011b80: 6577 732e 7079 3a32 3132 0a23 2c20 7079  ews.py:212.#, py
+00011b90: 7468 6f6e 2d66 6f72 6d61 740a 6d73 6769  thon-format.msgi
+00011ba0: 6420 2253 7562 6d69 7474 6564 2053 5250  d "Submitted SRP
+00011bb0: 2072 6571 7565 7374 2066 6f72 2079 6f75   request for you
+00011bc0: 7220 2528 7368 6970 2973 2e22 0a6d 7367  r %(ship)s.".msg
+00011bd0: 7374 7220 2222 0a0a 233a 2061 6c6c 6961  str ""..#: allia
+00011be0: 6e63 6561 7574 682f 7372 702f 7669 6577  nceauth/srp/view
+00011bf0: 732e 7079 3a32 3136 0a23 2c20 7079 7468  s.py:216.#, pyth
+00011c00: 6f6e 2d66 6f72 6d61 740a 6d73 6769 6420  on-format.msgid 
+00011c10: 2222 0a22 4368 6172 6163 7465 7220 2528  ""."Character %(
+00011c20: 6368 6172 6964 2973 2064 6f65 7320 6e6f  charid)s does no
+00011c30: 7420 6265 6c6f 6e67 2074 6f20 796f 7572  t belong to your
+00011c40: 2041 7574 6820 6163 636f 756e 742e 2050   Auth account. P
+00011c50: 6c65 6173 6520 6164 6420 7468 6520 220a  lease add the ".
+00011c60: 2241 5049 206b 6579 2066 6f72 2074 6869  "API key for thi
+00011c70: 7320 6368 6172 6163 7465 7220 616e 6420  s character and 
+00011c80: 7472 7920 6167 6169 6e22 0a6d 7367 7374  try again".msgst
+00011c90: 7220 2222 0a0a 233a 2061 6c6c 6961 6e63  r ""..#: allianc
+00011ca0: 6561 7574 682f 7372 702f 7669 6577 732e  eauth/srp/views.
+00011cb0: 7079 3a32 3336 2061 6c6c 6961 6e63 6561  py:236 alliancea
+00011cc0: 7574 682f 7372 702f 7669 6577 732e 7079  uth/srp/views.py
+00011cd0: 3a32 3632 0a23 3a20 616c 6c69 616e 6365  :262.#: alliance
+00011ce0: 6175 7468 2f73 7270 2f76 6965 7773 2e70  auth/srp/views.p
+00011cf0: 793a 3330 300a 6d73 6769 6420 224e 6f20  y:300.msgid "No 
+00011d00: 5352 5020 7265 7175 6573 7473 2073 656c  SRP requests sel
+00011d10: 6563 7465 6422 0a6d 7367 7374 7220 2222  ected".msgstr ""
+00011d20: 0a0a 233a 2061 6c6c 6961 6e63 6561 7574  ..#: allianceaut
+00011d30: 682f 7372 702f 7669 6577 732e 7079 3a32  h/srp/views.py:2
+00011d40: 3437 2061 6c6c 6961 6e63 6561 7574 682f  47 allianceauth/
+00011d50: 7372 702f 7669 6577 732e 7079 3a32 3835  srp/views.py:285
+00011d60: 0a6d 7367 6964 2022 556e 6162 6c65 2074  .msgid "Unable t
+00011d70: 6f20 6c6f 6361 7465 2073 656c 6563 7465  o locate selecte
+00011d80: 6420 5352 5020 7265 7175 6573 742e 220a  d SRP request.".
+00011d90: 6d73 6773 7472 2022 220a 0a23 3a20 616c  msgstr ""..#: al
+00011da0: 6c69 616e 6365 6175 7468 2f73 7270 2f76  lianceauth/srp/v
+00011db0: 6965 7773 2e70 793a 3235 300a 232c 2070  iews.py:250.#, p
+00011dc0: 7974 686f 6e2d 666f 726d 6174 0a6d 7367  ython-format.msg
+00011dd0: 6964 2022 4465 6c65 7465 6420 2528 6e75  id "Deleted %(nu
+00011de0: 6d72 6571 7565 7374 7329 7320 5352 5020  mrequests)s SRP 
+00011df0: 7265 7175 6573 7473 220a 6d73 6773 7472  requests".msgstr
+00011e00: 2022 220a 0a23 3a20 616c 6c69 616e 6365   ""..#: alliance
+00011e10: 6175 7468 2f73 7270 2f76 6965 7773 2e70  auth/srp/views.p
+00011e20: 793a 3238 380a 232c 2070 7974 686f 6e2d  y:288.#, python-
+00011e30: 666f 726d 6174 0a6d 7367 6964 2022 4170  format.msgid "Ap
+00011e40: 7072 6f76 6564 2025 286e 756d 7265 7175  proved %(numrequ
+00011e50: 6573 7473 2973 2053 5250 2072 6571 7565  ests)s SRP reque
+00011e60: 7374 7322 0a6d 7367 7374 7220 2222 0a0a  sts".msgstr ""..
+00011e70: 233a 2061 6c6c 6961 6e63 6561 7574 682f  #: allianceauth/
+00011e80: 7372 702f 7669 6577 732e 7079 3a33 3230  srp/views.py:320
+00011e90: 0a6d 7367 6964 2022 556e 6162 6c65 2074  .msgid "Unable t
+00011ea0: 6f20 6c6f 6361 7465 2073 656c 6563 7465  o locate selecte
+00011eb0: 6420 5352 5020 7265 7175 6573 7422 0a6d  d SRP request".m
+00011ec0: 7367 7374 7220 2222 0a0a 233a 2061 6c6c  sgstr ""..#: all
+00011ed0: 6961 6e63 6561 7574 682f 7372 702f 7669  ianceauth/srp/vi
+00011ee0: 6577 732e 7079 3a33 3233 0a23 2c20 7079  ews.py:323.#, py
+00011ef0: 7468 6f6e 2d66 6f72 6d61 740a 6d73 6769  thon-format.msgi
+00011f00: 6420 2252 656a 6563 7465 6420 2528 6e75  d "Rejected %(nu
+00011f10: 6d72 6571 7565 7374 7329 7320 5352 5020  mrequests)s SRP 
+00011f20: 7265 7175 6573 7473 2e22 0a6d 7367 7374  requests.".msgst
+00011f30: 7220 2222 0a0a 233a 2061 6c6c 6961 6e63  r ""..#: allianc
+00011f40: 6561 7574 682f 7372 702f 7669 6577 732e  eauth/srp/views.
+00011f50: 7079 3a33 3336 0a23 2c20 7079 7468 6f6e  py:336.#, python
+00011f60: 2d66 6f72 6d61 740a 6d73 6769 6420 2255  -format.msgid "U
+00011f70: 6e61 626c 6520 746f 206c 6f63 6174 6520  nable to locate 
+00011f80: 5352 5020 7265 7175 6573 7420 7769 7468  SRP request with
+00011f90: 2049 4420 2528 7265 7175 6573 7469 6429   ID %(requestid)
+00011fa0: 7322 0a6d 7367 7374 7220 2222 0a0a 233a  s".msgstr ""..#:
+00011fb0: 2061 6c6c 6961 6e63 6561 7574 682f 7372   allianceauth/sr
+00011fc0: 702f 7669 6577 732e 7079 3a33 3630 0a23  p/views.py:360.#
+00011fd0: 2c20 7079 7468 6f6e 2d66 6f72 6d61 740a  , python-format.
+00011fe0: 6d73 6769 6420 2253 6176 6564 2063 6861  msgid "Saved cha
+00011ff0: 6e67 6573 2074 6f20 5352 5020 666c 6565  nges to SRP flee
+00012000: 7420 2528 666c 6565 746e 616d 6529 7322  t %(fleetname)s"
+00012010: 0a6d 7367 7374 7220 2222 0a0a 233a 2061  .msgstr ""..#: a
+00012020: 6c6c 6961 6e63 6561 7574 682f 7465 6d70  llianceauth/temp
+00012030: 6c61 7465 732f 616c 6c69 616e 6365 6175  lates/allianceau
+00012040: 7468 2f61 646d 696e 2d73 7461 7475 732f  th/admin-status/
+00012050: 6573 695f 6368 6563 6b2e 6874 6d6c 3a34  esi_check.html:4
+00012060: 0a6d 7367 6964 2022 596f 7572 2053 6572  .msgid "Your Ser
+00012070: 7665 7220 7265 6365 6976 6564 2061 6e20  ver received an 
+00012080: 4553 4920 6572 726f 7220 7265 7370 6f6e  ESI error respon
+00012090: 7365 2063 6f64 6520 6f66 2022 0a6d 7367  se code of ".msg
+000120a0: 7374 7220 2222 0a0a 233a 2061 6c6c 6961  str ""..#: allia
+000120b0: 6e63 6561 7574 682f 7465 6d70 6c61 7465  nceauth/template
+000120c0: 732f 616c 6c69 616e 6365 6175 7468 2f61  s/allianceauth/a
+000120d0: 646d 696e 2d73 7461 7475 732f 6f76 6572  dmin-status/over
+000120e0: 7669 6577 2e68 746d 6c3a 3131 0a6d 7367  view.html:11.msg
+000120f0: 6964 2022 416c 6c69 616e 6365 2041 7574  id "Alliance Aut
+00012100: 6820 4e6f 7469 6669 6361 7469 6f6e 7322  h Notifications"
+00012110: 0a6d 7367 7374 7220 2222 0a0a 233a 2061  .msgstr ""..#: a
+00012120: 6c6c 6961 6e63 6561 7574 682f 7465 6d70  llianceauth/temp
+00012130: 6c61 7465 732f 616c 6c69 616e 6365 6175  lates/allianceau
+00012140: 7468 2f61 646d 696e 2d73 7461 7475 732f  th/admin-status/
+00012150: 6f76 6572 7669 6577 2e68 746d 6c3a 3231  overview.html:21
+00012160: 0a6d 7367 6964 2022 436c 6f73 6564 220a  .msgid "Closed".
+00012170: 6d73 6773 7472 2022 220a 0a23 3a20 616c  msgstr ""..#: al
+00012180: 6c69 616e 6365 6175 7468 2f74 656d 706c  lianceauth/templ
+00012190: 6174 6573 2f61 6c6c 6961 6e63 6561 7574  ates/allianceaut
+000121a0: 682f 6164 6d69 6e2d 7374 6174 7573 2f6f  h/admin-status/o
+000121b0: 7665 7276 6965 772e 6874 6d6c 3a32 370a  verview.html:27.
+000121c0: 6d73 6769 6420 224e 6f20 6e6f 7469 6669  msgid "No notifi
+000121d0: 6361 7469 6f6e 7320 6174 2074 6869 7320  cations at this 
+000121e0: 7469 6d65 220a 6d73 6773 7472 2022 220a  time".msgstr "".
+000121f0: 0a23 3a20 616c 6c69 616e 6365 6175 7468  .#: allianceauth
+00012200: 2f74 656d 706c 6174 6573 2f61 6c6c 6961  /templates/allia
+00012210: 6e63 6561 7574 682f 6164 6d69 6e2d 7374  nceauth/admin-st
+00012220: 6174 7573 2f6f 7665 7276 6965 772e 6874  atus/overview.ht
+00012230: 6d6c 3a33 360a 6d73 6769 6420 2250 6f77  ml:36.msgid "Pow
+00012240: 6572 6564 2062 7920 4769 744c 6162 220a  ered by GitLab".
+00012250: 6d73 6773 7472 2022 220a 0a23 3a20 616c  msgstr ""..#: al
+00012260: 6c69 616e 6365 6175 7468 2f74 656d 706c  lianceauth/templ
+00012270: 6174 6573 2f61 6c6c 6961 6e63 6561 7574  ates/allianceaut
+00012280: 682f 6164 6d69 6e2d 7374 6174 7573 2f6f  h/admin-status/o
+00012290: 7665 7276 6965 772e 6874 6d6c 3a34 320a  verview.html:42.
+000122a0: 6d73 6769 6420 2253 7570 706f 7274 2044  msgid "Support D
+000122b0: 6973 636f 7264 220a 6d73 6773 7472 2022  iscord".msgstr "
+000122c0: 220a 0a23 3a20 616c 6c69 616e 6365 6175  "..#: allianceau
+000122d0: 7468 2f74 656d 706c 6174 6573 2f61 6c6c  th/templates/all
+000122e0: 6961 6e63 6561 7574 682f 6164 6d69 6e2d  ianceauth/admin-
+000122f0: 7374 6174 7573 2f6f 7665 7276 6965 772e  status/overview.
+00012300: 6874 6d6c 3a35 390a 233a 2061 6c6c 6961  html:59.#: allia
+00012310: 6e63 6561 7574 682f 7465 6d70 6c61 7465  nceauth/template
+00012320: 732f 616c 6c69 616e 6365 6175 7468 2f61  s/allianceauth/a
+00012330: 646d 696e 2d73 7461 7475 732f 6f76 6572  dmin-status/over
+00012340: 7669 6577 2e68 746d 6c3a 3633 0a6d 7367  view.html:63.msg
+00012350: 6964 2022 536f 6674 7761 7265 2056 6572  id "Software Ver
+00012360: 7369 6f6e 220a 6d73 6773 7472 2022 220a  sion".msgstr "".
+00012370: 0a23 3a20 616c 6c69 616e 6365 6175 7468  .#: allianceauth
+00012380: 2f74 656d 706c 6174 6573 2f61 6c6c 6961  /templates/allia
+00012390: 6e63 6561 7574 682f 6164 6d69 6e2d 7374  nceauth/admin-st
+000123a0: 6174 7573 2f6f 7665 7276 6965 772e 6874  atus/overview.ht
+000123b0: 6d6c 3a36 360a 6d73 6769 6420 2243 7572  ml:66.msgid "Cur
+000123c0: 7265 6e74 220a 6d73 6773 7472 2022 220a  rent".msgstr "".
+000123d0: 0a23 3a20 616c 6c69 616e 6365 6175 7468  .#: allianceauth
+000123e0: 2f74 656d 706c 6174 6573 2f61 6c6c 6961  /templates/allia
+000123f0: 6e63 6561 7574 682f 6164 6d69 6e2d 7374  nceauth/admin-st
+00012400: 6174 7573 2f6f 7665 7276 6965 772e 6874  atus/overview.ht
+00012410: 6d6c 3a37 330a 6d73 6769 6420 224c 6174  ml:73.msgid "Lat
+00012420: 6573 7420 5374 6162 6c65 220a 6d73 6773  est Stable".msgs
+00012430: 7472 2022 220a 0a23 3a20 616c 6c69 616e  tr ""..#: allian
+00012440: 6365 6175 7468 2f74 656d 706c 6174 6573  ceauth/templates
+00012450: 2f61 6c6c 6961 6e63 6561 7574 682f 6164  /allianceauth/ad
+00012460: 6d69 6e2d 7374 6174 7573 2f6f 7665 7276  min-status/overv
+00012470: 6965 772e 6874 6d6c 3a37 380a 6d73 6769  iew.html:78.msgi
+00012480: 6420 2255 7064 6174 6520 6176 6169 6c61  d "Update availa
+00012490: 626c 6522 0a6d 7367 7374 7220 2222 0a0a  ble".msgstr ""..
+000124a0: 233a 2061 6c6c 6961 6e63 6561 7574 682f  #: allianceauth/
+000124b0: 7465 6d70 6c61 7465 732f 616c 6c69 616e  templates/allian
+000124c0: 6365 6175 7468 2f61 646d 696e 2d73 7461  ceauth/admin-sta
+000124d0: 7475 732f 6f76 6572 7669 6577 2e68 746d  tus/overview.htm
+000124e0: 6c3a 3836 0a6d 7367 6964 2022 4c61 7465  l:86.msgid "Late
+000124f0: 7374 2050 7265 2d52 656c 6561 7365 220a  st Pre-Release".
+00012500: 6d73 6773 7472 2022 220a 0a23 3a20 616c  msgstr ""..#: al
+00012510: 6c69 616e 6365 6175 7468 2f74 656d 706c  lianceauth/templ
+00012520: 6174 6573 2f61 6c6c 6961 6e63 6561 7574  ates/allianceaut
+00012530: 682f 6164 6d69 6e2d 7374 6174 7573 2f6f  h/admin-status/o
+00012540: 7665 7276 6965 772e 6874 6d6c 3a39 310a  verview.html:91.
+00012550: 6d73 6769 6420 2250 7265 2d52 656c 6561  msgid "Pre-Relea
+00012560: 7365 2061 7661 696c 6162 6c65 220a 6d73  se available".ms
+00012570: 6773 7472 2022 220a 0a23 3a20 616c 6c69  gstr ""..#: alli
+00012580: 616e 6365 6175 7468 2f74 656d 706c 6174  anceauth/templat
+00012590: 6573 2f61 6c6c 6961 6e63 6561 7574 682f  es/allianceauth/
+000125a0: 6164 6d69 6e2d 7374 6174 7573 2f6f 7665  admin-status/ove
+000125b0: 7276 6965 772e 6874 6d6c 3a31 3032 0a6d  rview.html:102.m
+000125c0: 7367 6964 2022 5461 736b 2051 7565 7565  sgid "Task Queue
+000125d0: 220a 6d73 6773 7472 2022 220a 0a23 3a20  ".msgstr ""..#: 
+000125e0: 616c 6c69 616e 6365 6175 7468 2f74 656d  allianceauth/tem
+000125f0: 706c 6174 6573 2f61 6c6c 6961 6e63 6561  plates/alliancea
+00012600: 7574 682f 6164 6d69 6e2d 7374 6174 7573  uth/admin-status
+00012610: 2f6f 7665 7276 6965 772e 6874 6d6c 3a31  /overview.html:1
+00012620: 3037 0a23 2c20 7079 7468 6f6e 2d66 6f72  07.#, python-for
+00012630: 6d61 740a 6d73 6769 6420 2222 0a22 5c6e  mat.msgid ""."\n
+00012640: 220a 2220 2020 2020 2020 2020 2020 2020  "."             
+00012650: 2020 2020 2020 2020 2020 2020 2020 2053                 S
+00012660: 7461 7475 7320 6f66 2025 2874 6f74 616c  tatus of %(total
+00012670: 2973 2070 726f 6365 7373 6564 2074 6173  )s processed tas
+00012680: 6b73 20e2 80a2 206c 6173 7420 220a 2225  ks ... last "."%
+00012690: 286c 6174 6573 7429 735c 6e22 0a22 2020  (latest)s\n"."  
+000126a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000126b0: 2020 2020 2020 220a 6d73 6773 7472 2022        ".msgstr "
+000126c0: 220a 0a23 3a20 616c 6c69 616e 6365 6175  "..#: allianceau
+000126d0: 7468 2f74 656d 706c 6174 6573 2f61 6c6c  th/templates/all
+000126e0: 6961 6e63 6561 7574 682f 6164 6d69 6e2d  ianceauth/admin-
+000126f0: 7374 6174 7573 2f6f 7665 7276 6965 772e  status/overview.
+00012700: 6874 6d6c 3a31 3233 0a6d 7367 6964 2022  html:123.msgid "
+00012710: 7275 6e6e 696e 6722 0a6d 7367 7374 7220  running".msgstr 
+00012720: 2222 0a0a 233a 2061 6c6c 6961 6e63 6561  ""..#: alliancea
+00012730: 7574 682f 7465 6d70 6c61 7465 732f 616c  uth/templates/al
+00012740: 6c69 616e 6365 6175 7468 2f61 646d 696e  lianceauth/admin
+00012750: 2d73 7461 7475 732f 6f76 6572 7669 6577  -status/overview
+00012760: 2e68 746d 6c3a 3132 340a 6d73 6769 6420  .html:124.msgid 
+00012770: 2271 7565 7565 6422 0a6d 7367 7374 7220  "queued".msgstr 
+00012780: 2222 0a0a 233a 2061 6c6c 6961 6e63 6561  ""..#: alliancea
+00012790: 7574 682f 7465 6d70 6c61 7465 732f 616c  uth/templates/al
+000127a0: 6c69 616e 6365 6175 7468 2f74 6f70 2d6d  lianceauth/top-m
+000127b0: 656e 752d 6164 6d69 6e2e 6874 6d6c 3a31  enu-admin.html:1
+000127c0: 390a 6d73 6769 6420 2241 4120 446f 6375  9.msgid "AA Docu
+000127d0: 6d65 6e74 6174 696f 6e22 0a6d 7367 7374  mentation".msgst
+000127e0: 7220 2222 0a0a 233a 2061 6c6c 6961 6e63  r ""..#: allianc
+000127f0: 6561 7574 682f 7465 6d70 6c61 7465 732f  eauth/templates/
+00012800: 616c 6c69 616e 6365 6175 7468 2f74 6f70  allianceauth/top
+00012810: 2d6d 656e 752d 6164 6d69 6e2e 6874 6d6c  -menu-admin.html
+00012820: 3a32 360a 6d73 6769 6420 2241 4120 5375  :26.msgid "AA Su
+00012830: 7070 6f72 7420 4469 7363 6f72 6422 0a6d  pport Discord".m
+00012840: 7367 7374 7220 2222 0a0a 233a 2061 6c6c  sgstr ""..#: all
+00012850: 6961 6e63 6561 7574 682f 7465 6d70 6c61  ianceauth/templa
+00012860: 7465 732f 616c 6c69 616e 6365 6175 7468  tes/allianceauth
+00012870: 2f74 6f70 2d6d 656e 752d 7573 6572 2d64  /top-menu-user-d
+00012880: 726f 7064 6f77 6e2e 6874 6d6c 3a31 300a  ropdown.html:10.
+00012890: 233a 2061 6c6c 6961 6e63 6561 7574 682f  #: allianceauth/
+000128a0: 7465 6d70 6c61 7465 732f 616c 6c69 616e  templates/allian
+000128b0: 6365 6175 7468 2f74 6f70 2d6d 656e 752d  ceauth/top-menu-
+000128c0: 7573 6572 2d64 726f 7064 6f77 6e2e 6874  user-dropdown.ht
+000128d0: 6d6c 3a31 360a 6d73 6769 6420 2255 7365  ml:16.msgid "Use
+000128e0: 7220 4d65 6e75 220a 6d73 6773 7472 2022  r Menu".msgstr "
+000128f0: 220a 0a23 3a20 616c 6c69 616e 6365 6175  "..#: allianceau
+00012900: 7468 2f74 656d 706c 6174 6573 2f61 6c6c  th/templates/all
+00012910: 6961 6e63 6561 7574 682f 746f 702d 6d65  ianceauth/top-me
+00012920: 6e75 2d75 7365 722d 6472 6f70 646f 776e  nu-user-dropdown
+00012930: 2e68 746d 6c3a 3637 0a6d 7367 6964 2022  .html:67.msgid "
+00012940: 4c6f 676f 7574 220a 6d73 6773 7472 2022  Logout".msgstr "
+00012950: 220a 0a23 3a20 616c 6c69 616e 6365 6175  "..#: allianceau
+00012960: 7468 2f74 656d 706c 6174 6573 2f61 6c6c  th/templates/all
+00012970: 6961 6e63 6561 7574 682f 746f 702d 6d65  ianceauth/top-me
+00012980: 6e75 2e68 746d 6c3a 380a 6d73 6769 6420  nu.html:8.msgid 
+00012990: 2254 6f67 676c 6520 6e61 7669 6761 7469  "Toggle navigati
+000129a0: 6f6e 220a 6d73 6773 7472 2022 220a 0a23  on".msgstr ""..#
+000129b0: 3a20 616c 6c69 616e 6365 6175 7468 2f74  : allianceauth/t
+000129c0: 6865 6d65 2f74 656d 706c 6174 6573 2f74  heme/templates/t
+000129d0: 6865 6d65 2f74 6865 6d65 5f73 656c 6563  heme/theme_selec
+000129e0: 742e 6874 6d6c 3a37 0a6d 7367 6964 2022  t.html:7.msgid "
+000129f0: 5365 6c65 6374 2054 6865 6d65 220a 6d73  Select Theme".ms
+00012a00: 6773 7472 2022 220a 0a23 3a20 616c 6c69  gstr ""..#: alli
+00012a10: 616e 6365 6175 7468 2f74 696d 6572 626f  anceauth/timerbo
+00012a20: 6172 642f 666f 726d 2e70 793a 3533 0a23  ard/form.py:53.#
+00012a30: 3a20 616c 6c69 616e 6365 6175 7468 2f74  : allianceauth/t
+00012a40: 696d 6572 626f 6172 642f 7465 6d70 6c61  imerboard/templa
+00012a50: 7465 732f 7469 6d65 7262 6f61 7264 2f74  tes/timerboard/t
+00012a60: 696d 6572 7461 626c 652e 6874 6d6c 3a31  imertable.html:1
+00012a70: 3732 0a6d 7367 6964 2022 4f74 6865 7222  72.msgid "Other"
+00012a80: 0a6d 7367 7374 7220 2222 0a0a 233a 2061  .msgstr ""..#: a
+00012a90: 6c6c 6961 6e63 6561 7574 682f 7469 6d65  llianceauth/time
+00012aa0: 7262 6f61 7264 2f66 6f72 6d2e 7079 3a35  rboard/form.py:5
+00012ab0: 340a 233a 2061 6c6c 6961 6e63 6561 7574  4.#: allianceaut
+00012ac0: 682f 7469 6d65 7262 6f61 7264 2f74 656d  h/timerboard/tem
+00012ad0: 706c 6174 6573 2f74 696d 6572 626f 6172  plates/timerboar
+00012ae0: 642f 6461 7368 626f 6172 642e 7469 6d65  d/dashboard.time
+00012af0: 7273 2e68 746d 6c3a 3338 0a23 3a20 616c  rs.html:38.#: al
+00012b00: 6c69 616e 6365 6175 7468 2f74 696d 6572  lianceauth/timer
+00012b10: 626f 6172 642f 7465 6d70 6c61 7465 732f  board/templates/
+00012b20: 7469 6d65 7262 6f61 7264 2f74 696d 6572  timerboard/timer
+00012b30: 7461 626c 652e 6874 6d6c 3a34 340a 6d73  table.html:44.ms
+00012b40: 6769 6420 2246 7269 656e 646c 7922 0a6d  gid "Friendly".m
+00012b50: 7367 7374 7220 2222 0a0a 233a 2061 6c6c  sgstr ""..#: all
+00012b60: 6961 6e63 6561 7574 682f 7469 6d65 7262  ianceauth/timerb
+00012b70: 6f61 7264 2f66 6f72 6d2e 7079 3a35 350a  oard/form.py:55.
+00012b80: 233a 2061 6c6c 6961 6e63 6561 7574 682f  #: allianceauth/
+00012b90: 7469 6d65 7262 6f61 7264 2f74 656d 706c  timerboard/templ
+00012ba0: 6174 6573 2f74 696d 6572 626f 6172 642f  ates/timerboard/
+00012bb0: 6461 7368 626f 6172 642e 7469 6d65 7273  dashboard.timers
+00012bc0: 2e68 746d 6c3a 3333 0a23 3a20 616c 6c69  .html:33.#: alli
+00012bd0: 616e 6365 6175 7468 2f74 696d 6572 626f  anceauth/timerbo
+00012be0: 6172 642f 7465 6d70 6c61 7465 732f 7469  ard/templates/ti
+00012bf0: 6d65 7262 6f61 7264 2f74 696d 6572 7461  merboard/timerta
+00012c00: 626c 652e 6874 6d6c 3a33 380a 6d73 6769  ble.html:38.msgi
+00012c10: 6420 2248 6f73 7469 6c65 220a 6d73 6773  d "Hostile".msgs
+00012c20: 7472 2022 220a 0a23 3a20 616c 6c69 616e  tr ""..#: allian
+00012c30: 6365 6175 7468 2f74 696d 6572 626f 6172  ceauth/timerboar
+00012c40: 642f 666f 726d 2e70 793a 3536 0a23 3a20  d/form.py:56.#: 
+00012c50: 616c 6c69 616e 6365 6175 7468 2f74 696d  allianceauth/tim
+00012c60: 6572 626f 6172 642f 7465 6d70 6c61 7465  erboard/template
+00012c70: 732f 7469 6d65 7262 6f61 7264 2f64 6173  s/timerboard/das
+00012c80: 6862 6f61 7264 2e74 696d 6572 732e 6874  hboard.timers.ht
+00012c90: 6d6c 3a34 330a 233a 2061 6c6c 6961 6e63  ml:43.#: allianc
+00012ca0: 6561 7574 682f 7469 6d65 7262 6f61 7264  eauth/timerboard
+00012cb0: 2f74 656d 706c 6174 6573 2f74 696d 6572  /templates/timer
+00012cc0: 626f 6172 642f 7469 6d65 7274 6162 6c65  board/timertable
+00012cd0: 2e68 746d 6c3a 3530 0a6d 7367 6964 2022  .html:50.msgid "
+00012ce0: 4e65 7574 7261 6c22 0a6d 7367 7374 7220  Neutral".msgstr 
+00012cf0: 2222 0a0a 233a 2061 6c6c 6961 6e63 6561  ""..#: alliancea
+00012d00: 7574 682f 7469 6d65 7262 6f61 7264 2f66  uth/timerboard/f
+00012d10: 6f72 6d2e 7079 3a35 380a 233a 2061 6c6c  orm.py:58.#: all
+00012d20: 6961 6e63 6561 7574 682f 7469 6d65 7262  ianceauth/timerb
+00012d30: 6f61 7264 2f74 656d 706c 6174 6573 2f74  oard/templates/t
+00012d40: 696d 6572 626f 6172 642f 6461 7368 626f  imerboard/dashbo
+00012d50: 6172 642e 7469 6d65 7273 2e68 746d 6c3a  ard.timers.html:
+00012d60: 3133 0a23 3a20 616c 6c69 616e 6365 6175  13.#: allianceau
+00012d70: 7468 2f74 696d 6572 626f 6172 642f 7465  th/timerboard/te
+00012d80: 6d70 6c61 7465 732f 7469 6d65 7262 6f61  mplates/timerboa
+00012d90: 7264 2f74 696d 6572 7461 626c 652e 6874  rd/timertable.ht
+00012da0: 6d6c 3a37 0a6d 7367 6964 2022 4465 7461  ml:7.msgid "Deta
+00012db0: 696c 7322 0a6d 7367 7374 7220 2222 0a0a  ils".msgstr ""..
+00012dc0: 233a 2061 6c6c 6961 6e63 6561 7574 682f  #: allianceauth/
+00012dd0: 7469 6d65 7262 6f61 7264 2f66 6f72 6d2e  timerboard/form.
+00012de0: 7079 3a36 300a 6d73 6769 6420 2250 6c61  py:60.msgid "Pla
+00012df0: 6e65 742f 4d6f 6f6e 220a 6d73 6773 7472  net/Moon".msgstr
+00012e00: 2022 220a 0a23 3a20 616c 6c69 616e 6365   ""..#: alliance
+00012e10: 6175 7468 2f74 696d 6572 626f 6172 642f  auth/timerboard/
+00012e20: 666f 726d 2e70 793a 3631 0a6d 7367 6964  form.py:61.msgid
+00012e30: 2022 5374 7275 6374 7572 6520 5479 7065   "Structure Type
+00012e40: 220a 6d73 6773 7472 2022 220a 0a23 3a20  ".msgstr ""..#: 
+00012e50: 616c 6c69 616e 6365 6175 7468 2f74 696d  allianceauth/tim
+00012e60: 6572 626f 6172 642f 666f 726d 2e70 793a  erboard/form.py:
+00012e70: 3632 0a6d 7367 6964 2022 5469 6d65 7220  62.msgid "Timer 
+00012e80: 5479 7065 220a 6d73 6773 7472 2022 220a  Type".msgstr "".
+00012e90: 0a23 3a20 616c 6c69 616e 6365 6175 7468  .#: allianceauth
+00012ea0: 2f74 696d 6572 626f 6172 642f 666f 726d  /timerboard/form
+00012eb0: 2e70 793a 3633 0a23 3a20 616c 6c69 616e  .py:63.#: allian
+00012ec0: 6365 6175 7468 2f74 696d 6572 626f 6172  ceauth/timerboar
+00012ed0: 642f 7465 6d70 6c61 7465 732f 7469 6d65  d/templates/time
+00012ee0: 7262 6f61 7264 2f74 696d 6572 7461 626c  rboard/timertabl
+00012ef0: 652e 6874 6d6c 3a38 0a6d 7367 6964 2022  e.html:8.msgid "
+00012f00: 4f62 6a65 6374 6976 6522 0a6d 7367 7374  Objective".msgst
+00012f10: 7220 2222 0a0a 233a 2061 6c6c 6961 6e63  r ""..#: allianc
+00012f20: 6561 7574 682f 7469 6d65 7262 6f61 7264  eauth/timerboard
+00012f30: 2f66 6f72 6d2e 7079 3a36 340a 6d73 6769  /form.py:64.msgi
+00012f40: 6420 2241 6273 6f6c 7574 6520 5469 6d65  d "Absolute Time
+00012f50: 7222 0a6d 7367 7374 7220 2222 0a0a 233a  r".msgstr ""..#:
+00012f60: 2061 6c6c 6961 6e63 6561 7574 682f 7469   allianceauth/ti
+00012f70: 6d65 7262 6f61 7264 2f66 6f72 6d2e 7079  merboard/form.py
+00012f80: 3a36 350a 6d73 6769 6420 2244 6174 6520  :65.msgid "Date 
+00012f90: 616e 6420 5469 6d65 220a 6d73 6773 7472  and Time".msgstr
+00012fa0: 2022 220a 0a23 3a20 616c 6c69 616e 6365   ""..#: alliance
+00012fb0: 6175 7468 2f74 696d 6572 626f 6172 642f  auth/timerboard/
+00012fc0: 666f 726d 2e70 793a 3636 0a6d 7367 6964  form.py:66.msgid
+00012fd0: 2022 4461 7973 2052 656d 6169 6e69 6e67   "Days Remaining
+00012fe0: 220a 6d73 6773 7472 2022 220a 0a23 3a20  ".msgstr ""..#: 
+00012ff0: 616c 6c69 616e 6365 6175 7468 2f74 696d  allianceauth/tim
+00013000: 6572 626f 6172 642f 666f 726d 2e70 793a  erboard/form.py:
+00013010: 3637 0a6d 7367 6964 2022 486f 7572 7320  67.msgid "Hours 
+00013020: 5265 6d61 696e 696e 6722 0a6d 7367 7374  Remaining".msgst
+00013030: 7220 2222 0a0a 233a 2061 6c6c 6961 6e63  r ""..#: allianc
+00013040: 6561 7574 682f 7469 6d65 7262 6f61 7264  eauth/timerboard
+00013050: 2f66 6f72 6d2e 7079 3a36 390a 6d73 6769  /form.py:69.msgi
+00013060: 6420 224d 696e 7574 6573 2052 656d 6169  d "Minutes Remai
+00013070: 6e69 6e67 220a 6d73 6773 7472 2022 220a  ning".msgstr "".
+00013080: 0a23 3a20 616c 6c69 616e 6365 6175 7468  .#: allianceauth
+00013090: 2f74 696d 6572 626f 6172 642f 666f 726d  /timerboard/form
+000130a0: 2e70 793a 3731 0a6d 7367 6964 2022 496d  .py:71.msgid "Im
+000130b0: 706f 7274 616e 7422 0a6d 7367 7374 7220  portant".msgstr 
+000130c0: 2222 0a0a 233a 2061 6c6c 6961 6e63 6561  ""..#: alliancea
+000130d0: 7574 682f 7469 6d65 7262 6f61 7264 2f66  uth/timerboard/f
+000130e0: 6f72 6d2e 7079 3a37 320a 6d73 6769 6420  orm.py:72.msgid 
+000130f0: 2243 6f72 702d 5265 7374 7269 6374 6564  "Corp-Restricted
+00013100: 220a 6d73 6773 7472 2022 220a 0a23 3a20  ".msgstr ""..#: 
+00013110: 616c 6c69 616e 6365 6175 7468 2f74 696d  allianceauth/tim
+00013120: 6572 626f 6172 642f 6d6f 6465 6c73 2e70  erboard/models.p
+00013130: 793a 3134 0a6d 7367 6964 2022 4e6f 7420  y:14.msgid "Not 
+00013140: 5370 6563 6966 6965 6422 0a6d 7367 7374  Specified".msgst
+00013150: 7220 2222 0a0a 233a 2061 6c6c 6961 6e63  r ""..#: allianc
+00013160: 6561 7574 682f 7469 6d65 7262 6f61 7264  eauth/timerboard
+00013170: 2f6d 6f64 656c 732e 7079 3a31 350a 6d73  /models.py:15.ms
+00013180: 6769 6420 2253 6869 656c 6422 0a6d 7367  gid "Shield".msg
+00013190: 7374 7220 2222 0a0a 233a 2061 6c6c 6961  str ""..#: allia
+000131a0: 6e63 6561 7574 682f 7469 6d65 7262 6f61  nceauth/timerboa
+000131b0: 7264 2f6d 6f64 656c 732e 7079 3a31 360a  rd/models.py:16.
+000131c0: 6d73 6769 6420 2241 726d 6f72 220a 6d73  msgid "Armor".ms
+000131d0: 6773 7472 2022 220a 0a23 3a20 616c 6c69  gstr ""..#: alli
+000131e0: 616e 6365 6175 7468 2f74 696d 6572 626f  anceauth/timerbo
+000131f0: 6172 642f 6d6f 6465 6c73 2e70 793a 3137  ard/models.py:17
+00013200: 0a6d 7367 6964 2022 4875 6c6c 220a 6d73  .msgid "Hull".ms
 00013210: 6773 7472 2022 220a 0a23 3a20 616c 6c69  gstr ""..#: alli
 00013220: 616e 6365 6175 7468 2f74 696d 6572 626f  anceauth/timerbo
-00013230: 6172 642f 6d6f 6465 6c73 2e70 793a 3230  ard/models.py:20
-00013240: 0a6d 7367 6964 2022 556e 616e 6368 6f72  .msgid "Unanchor
-00013250: 696e 6722 0a6d 7367 7374 7220 2222 0a0a  ing".msgstr ""..
-00013260: 233a 2061 6c6c 6961 6e63 6561 7574 682f  #: allianceauth/
-00013270: 7469 6d65 7262 6f61 7264 2f74 656d 706c  timerboard/templ
-00013280: 6174 6573 2f74 696d 6572 626f 6172 642f  ates/timerboard/
-00013290: 6461 7368 626f 6172 642e 7469 6d65 7273  dashboard.timers
-000132a0: 2e68 746d 6c3a 370a 233a 2061 6c6c 6961  .html:7.#: allia
-000132b0: 6e63 6561 7574 682f 7469 6d65 7262 6f61  nceauth/timerboa
-000132c0: 7264 2f74 656d 706c 6174 6573 2f74 696d  rd/templates/tim
-000132d0: 6572 626f 6172 642f 7669 6577 2e68 746d  erboard/view.htm
-000132e0: 6c3a 3533 0a6d 7367 6964 2022 5570 636f  l:53.msgid "Upco
-000132f0: 6d69 6e67 2054 696d 6572 7322 0a6d 7367  ming Timers".msg
-00013300: 7374 7220 2222 0a0a 233a 2061 6c6c 6961  str ""..#: allia
-00013310: 6e63 6561 7574 682f 7469 6d65 7262 6f61  nceauth/timerboa
-00013320: 7264 2f74 656d 706c 6174 6573 2f74 696d  rd/templates/tim
-00013330: 6572 626f 6172 642f 6461 7368 626f 6172  erboard/dashboar
-00013340: 642e 7469 6d65 7273 2e68 746d 6c3a 3134  d.timers.html:14
-00013350: 0a6d 7367 6964 2022 5469 6d65 7222 0a6d  .msgid "Timer".m
-00013360: 7367 7374 7220 2222 0a0a 233a 2061 6c6c  sgstr ""..#: all
-00013370: 6961 6e63 6561 7574 682f 7469 6d65 7262  ianceauth/timerb
-00013380: 6f61 7264 2f74 656d 706c 6174 6573 2f74  oard/templates/t
-00013390: 696d 6572 626f 6172 642f 666f 726d 2e68  imerboard/form.h
-000133a0: 746d 6c3a 3130 0a23 3a20 616c 6c69 616e  tml:10.#: allian
-000133b0: 6365 6175 7468 2f74 696d 6572 626f 6172  ceauth/timerboar
-000133c0: 642f 7465 6d70 6c61 7465 732f 7469 6d65  d/templates/time
-000133d0: 7262 6f61 7264 2f74 696d 6572 5f63 6f6e  rboard/timer_con
-000133e0: 6669 726d 5f64 656c 6574 652e 6874 6d6c  firm_delete.html
-000133f0: 3a31 300a 233a 2061 6c6c 6961 6e63 6561  :10.#: alliancea
-00013400: 7574 682f 7469 6d65 7262 6f61 7264 2f74  uth/timerboard/t
-00013410: 656d 706c 6174 6573 2f74 696d 6572 626f  emplates/timerbo
-00013420: 6172 642f 7669 6577 2e68 746d 6c3a 3133  ard/view.html:13
-00013430: 0a6d 7367 6964 2022 5374 7275 6374 7572  .msgid "Structur
-00013440: 6520 5469 6d65 7273 220a 6d73 6773 7472  e Timers".msgstr
-00013450: 2022 220a 0a23 3a20 616c 6c69 616e 6365   ""..#: alliance
-00013460: 6175 7468 2f74 696d 6572 626f 6172 642f  auth/timerboard/
-00013470: 7465 6d70 6c61 7465 732f 7469 6d65 7262  templates/timerb
-00013480: 6f61 7264 2f66 6f72 6d2e 6874 6d6c 3a32  oard/form.html:2
-00013490: 350a 6d73 6769 6420 2253 7472 7563 7475  5.msgid "Structu
-000134a0: 7265 2054 696d 6572 2044 6574 6169 6c73  re Timer Details
-000134b0: 220a 6d73 6773 7472 2022 220a 0a23 3a20  ".msgstr ""..#: 
-000134c0: 616c 6c69 616e 6365 6175 7468 2f74 696d  allianceauth/tim
-000134d0: 6572 626f 6172 642f 7465 6d70 6c61 7465  erboard/template
-000134e0: 732f 7469 6d65 7262 6f61 7264 2f74 696d  s/timerboard/tim
-000134f0: 6572 5f63 6f6e 6669 726d 5f64 656c 6574  er_confirm_delet
-00013500: 652e 6874 6d6c 3a36 0a23 3a20 616c 6c69  e.html:6.#: alli
-00013510: 616e 6365 6175 7468 2f74 696d 6572 626f  anceauth/timerbo
-00013520: 6172 642f 7465 6d70 6c61 7465 732f 7469  ard/templates/ti
-00013530: 6d65 7262 6f61 7264 2f74 696d 6572 5f63  merboard/timer_c
-00013540: 6f6e 6669 726d 5f64 656c 6574 652e 6874  onfirm_delete.ht
-00013550: 6d6c 3a31 350a 6d73 6769 6420 2244 656c  ml:15.msgid "Del
-00013560: 6574 6520 5469 6d65 7222 0a6d 7367 7374  ete Timer".msgst
-00013570: 7220 2222 0a0a 233a 2061 6c6c 6961 6e63  r ""..#: allianc
-00013580: 6561 7574 682f 7469 6d65 7262 6f61 7264  eauth/timerboard
-00013590: 2f74 656d 706c 6174 6573 2f74 696d 6572  /templates/timer
-000135a0: 626f 6172 642f 7469 6d65 725f 636f 6e66  board/timer_conf
-000135b0: 6972 6d5f 6465 6c65 7465 2e68 746d 6c3a  irm_delete.html:
-000135c0: 3236 0a23 2c20 7079 7468 6f6e 2d66 6f72  26.#, python-for
-000135d0: 6d61 740a 6d73 6769 6420 2241 7265 2079  mat.msgid "Are y
-000135e0: 6f75 2073 7572 6520 796f 7520 7761 6e74  ou sure you want
-000135f0: 2074 6f20 6465 6c65 7465 2074 696d 6572   to delete timer
-00013600: 205c 2225 286f 626a 6563 7429 735c 223f   \"%(object)s\"?
-00013610: 220a 6d73 6773 7472 2022 220a 0a23 3a20  ".msgstr ""..#: 
-00013620: 616c 6c69 616e 6365 6175 7468 2f74 696d  allianceauth/tim
-00013630: 6572 626f 6172 642f 7465 6d70 6c61 7465  erboard/template
-00013640: 732f 7469 6d65 7262 6f61 7264 2f74 696d  s/timerboard/tim
-00013650: 6572 5f63 7265 6174 655f 666f 726d 2e68  er_create_form.h
-00013660: 746d 6c3a 350a 233a 2061 6c6c 6961 6e63  tml:5.#: allianc
-00013670: 6561 7574 682f 7469 6d65 7262 6f61 7264  eauth/timerboard
-00013680: 2f74 656d 706c 6174 6573 2f74 696d 6572  /templates/timer
-00013690: 626f 6172 642f 7469 6d65 725f 6372 6561  board/timer_crea
-000136a0: 7465 5f66 6f72 6d2e 6874 6d6c 3a31 330a  te_form.html:13.
-000136b0: 6d73 6769 6420 2243 7265 6174 6520 5469  msgid "Create Ti
-000136c0: 6d65 7222 0a6d 7367 7374 7220 2222 0a0a  mer".msgstr ""..
-000136d0: 233a 2061 6c6c 6961 6e63 6561 7574 682f  #: allianceauth/
-000136e0: 7469 6d65 7262 6f61 7264 2f74 656d 706c  timerboard/templ
-000136f0: 6174 6573 2f74 696d 6572 626f 6172 642f  ates/timerboard/
-00013700: 7469 6d65 725f 6372 6561 7465 5f66 6f72  timer_create_for
-00013710: 6d2e 6874 6d6c 3a39 0a23 3a20 616c 6c69  m.html:9.#: alli
-00013720: 616e 6365 6175 7468 2f74 696d 6572 626f  anceauth/timerbo
-00013730: 6172 642f 7465 6d70 6c61 7465 732f 7469  ard/templates/ti
-00013740: 6d65 7262 6f61 7264 2f76 6965 772e 6874  merboard/view.ht
-00013750: 6d6c 3a32 310a 6d73 6769 6420 2243 7265  ml:21.msgid "Cre
-00013760: 6174 6520 5374 7275 6374 7572 6520 5469  ate Structure Ti
-00013770: 6d65 7222 0a6d 7367 7374 7220 2222 0a0a  mer".msgstr ""..
-00013780: 233a 2061 6c6c 6961 6e63 6561 7574 682f  #: allianceauth/
-00013790: 7469 6d65 7262 6f61 7264 2f74 656d 706c  timerboard/templ
-000137a0: 6174 6573 2f74 696d 6572 626f 6172 642f  ates/timerboard/
-000137b0: 7469 6d65 725f 7570 6461 7465 5f66 6f72  timer_update_for
-000137c0: 6d2e 6874 6d6c 3a35 0a23 3a20 616c 6c69  m.html:5.#: alli
-000137d0: 616e 6365 6175 7468 2f74 696d 6572 626f  anceauth/timerbo
-000137e0: 6172 642f 7465 6d70 6c61 7465 732f 7469  ard/templates/ti
-000137f0: 6d65 7262 6f61 7264 2f74 696d 6572 5f75  merboard/timer_u
-00013800: 7064 6174 655f 666f 726d 2e68 746d 6c3a  pdate_form.html:
-00013810: 390a 233a 2061 6c6c 6961 6e63 6561 7574  9.#: allianceaut
-00013820: 682f 7469 6d65 7262 6f61 7264 2f74 656d  h/timerboard/tem
-00013830: 706c 6174 6573 2f74 696d 6572 626f 6172  plates/timerboar
-00013840: 642f 7469 6d65 725f 7570 6461 7465 5f66  d/timer_update_f
-00013850: 6f72 6d2e 6874 6d6c 3a31 330a 6d73 6769  orm.html:13.msgi
-00013860: 6420 2255 7064 6174 6520 5374 7275 6374  d "Update Struct
-00013870: 7572 6520 5469 6d65 7222 0a6d 7367 7374  ure Timer".msgst
-00013880: 7220 2222 0a0a 233a 2061 6c6c 6961 6e63  r ""..#: allianc
-00013890: 6561 7574 682f 7469 6d65 7262 6f61 7264  eauth/timerboard
-000138a0: 2f74 656d 706c 6174 6573 2f74 696d 6572  /templates/timer
-000138b0: 626f 6172 642f 7469 6d65 7274 6162 6c65  board/timertable
-000138c0: 2e68 746d 6c3a 3130 0a6d 7367 6964 2022  .html:10.msgid "
-000138d0: 5374 7275 6374 7572 6522 0a6d 7367 7374  Structure".msgst
-000138e0: 7220 2222 0a0a 233a 2061 6c6c 6961 6e63  r ""..#: allianc
-000138f0: 6561 7574 682f 7469 6d65 7262 6f61 7264  eauth/timerboard
-00013900: 2f74 656d 706c 6174 6573 2f74 696d 6572  /templates/timer
-00013910: 626f 6172 642f 7469 6d65 7274 6162 6c65  board/timertable
-00013920: 2e68 746d 6c3a 3634 0a6d 7367 6964 2022  .html:64.msgid "
-00013930: 504f 434f 220a 6d73 6773 7472 2022 220a  POCO".msgstr "".
-00013940: 0a23 3a20 616c 6c69 616e 6365 6175 7468  .#: allianceauth
-00013950: 2f74 696d 6572 626f 6172 642f 7465 6d70  /timerboard/temp
-00013960: 6c61 7465 732f 7469 6d65 7262 6f61 7264  lates/timerboard
-00013970: 2f74 696d 6572 7461 626c 652e 6874 6d6c  /timertable.html
-00013980: 3a37 300a 6d73 6769 6420 2249 2d48 5542  :70.msgid "I-HUB
-00013990: 220a 6d73 6773 7472 2022 220a 0a23 3a20  ".msgstr ""..#: 
-000139a0: 616c 6c69 616e 6365 6175 7468 2f74 696d  allianceauth/tim
-000139b0: 6572 626f 6172 642f 7465 6d70 6c61 7465  erboard/template
-000139c0: 732f 7469 6d65 7262 6f61 7264 2f74 696d  s/timerboard/tim
-000139d0: 6572 7461 626c 652e 6874 6d6c 3a37 360a  ertable.html:76.
-000139e0: 6d73 6769 6420 2254 4355 220a 6d73 6773  msgid "TCU".msgs
-000139f0: 7472 2022 220a 0a23 3a20 616c 6c69 616e  tr ""..#: allian
-00013a00: 6365 6175 7468 2f74 696d 6572 626f 6172  ceauth/timerboar
-00013a10: 642f 7465 6d70 6c61 7465 732f 7469 6d65  d/templates/time
-00013a20: 7262 6f61 7264 2f74 696d 6572 7461 626c  rboard/timertabl
-00013a30: 652e 6874 6d6c 3a38 320a 6d73 6769 6420  e.html:82.msgid 
-00013a40: 2250 4f53 205b 535d 220a 6d73 6773 7472  "POS [S]".msgstr
-00013a50: 2022 220a 0a23 3a20 616c 6c69 616e 6365   ""..#: alliance
-00013a60: 6175 7468 2f74 696d 6572 626f 6172 642f  auth/timerboard/
-00013a70: 7465 6d70 6c61 7465 732f 7469 6d65 7262  templates/timerb
-00013a80: 6f61 7264 2f74 696d 6572 7461 626c 652e  oard/timertable.
-00013a90: 6874 6d6c 3a38 380a 6d73 6769 6420 2250  html:88.msgid "P
-00013aa0: 4f53 205b 4d5d 220a 6d73 6773 7472 2022  OS [M]".msgstr "
-00013ab0: 220a 0a23 3a20 616c 6c69 616e 6365 6175  "..#: allianceau
-00013ac0: 7468 2f74 696d 6572 626f 6172 642f 7465  th/timerboard/te
-00013ad0: 6d70 6c61 7465 732f 7469 6d65 7262 6f61  mplates/timerboa
-00013ae0: 7264 2f74 696d 6572 7461 626c 652e 6874  rd/timertable.ht
-00013af0: 6d6c 3a39 340a 6d73 6769 6420 2250 4f53  ml:94.msgid "POS
-00013b00: 205b 4c5d 220a 6d73 6773 7472 2022 220a   [L]".msgstr "".
-00013b10: 0a23 3a20 616c 6c69 616e 6365 6175 7468  .#: allianceauth
-00013b20: 2f74 696d 6572 626f 6172 642f 7465 6d70  /timerboard/temp
-00013b30: 6c61 7465 732f 7469 6d65 7262 6f61 7264  lates/timerboard
-00013b40: 2f74 696d 6572 7461 626c 652e 6874 6d6c  /timertable.html
-00013b50: 3a31 3030 0a6d 7367 6964 2022 4173 7472  :100.msgid "Astr
-00013b60: 6168 7573 220a 6d73 6773 7472 2022 220a  ahus".msgstr "".
-00013b70: 0a23 3a20 616c 6c69 616e 6365 6175 7468  .#: allianceauth
-00013b80: 2f74 696d 6572 626f 6172 642f 7465 6d70  /timerboard/temp
-00013b90: 6c61 7465 732f 7469 6d65 7262 6f61 7264  lates/timerboard
-00013ba0: 2f74 696d 6572 7461 626c 652e 6874 6d6c  /timertable.html
-00013bb0: 3a31 3036 0a6d 7367 6964 2022 466f 7274  :106.msgid "Fort
-00013bc0: 697a 6172 220a 6d73 6773 7472 2022 220a  izar".msgstr "".
-00013bd0: 0a23 3a20 616c 6c69 616e 6365 6175 7468  .#: allianceauth
-00013be0: 2f74 696d 6572 626f 6172 642f 7465 6d70  /timerboard/temp
-00013bf0: 6c61 7465 732f 7469 6d65 7262 6f61 7264  lates/timerboard
-00013c00: 2f74 696d 6572 7461 626c 652e 6874 6d6c  /timertable.html
-00013c10: 3a31 3132 0a6d 7367 6964 2022 4b65 6570  :112.msgid "Keep
-00013c20: 7374 6172 220a 6d73 6773 7472 2022 220a  star".msgstr "".
-00013c30: 0a23 3a20 616c 6c69 616e 6365 6175 7468  .#: allianceauth
-00013c40: 2f74 696d 6572 626f 6172 642f 7465 6d70  /timerboard/temp
-00013c50: 6c61 7465 732f 7469 6d65 7262 6f61 7264  lates/timerboard
-00013c60: 2f74 696d 6572 7461 626c 652e 6874 6d6c  /timertable.html
-00013c70: 3a31 3138 0a6d 7367 6964 2022 5261 6974  :118.msgid "Rait
-00013c80: 6172 7522 0a6d 7367 7374 7220 2222 0a0a  aru".msgstr ""..
-00013c90: 233a 2061 6c6c 6961 6e63 6561 7574 682f  #: allianceauth/
-00013ca0: 7469 6d65 7262 6f61 7264 2f74 656d 706c  timerboard/templ
-00013cb0: 6174 6573 2f74 696d 6572 626f 6172 642f  ates/timerboard/
-00013cc0: 7469 6d65 7274 6162 6c65 2e68 746d 6c3a  timertable.html:
-00013cd0: 3132 340a 6d73 6769 6420 2241 7a62 656c  124.msgid "Azbel
-00013ce0: 220a 6d73 6773 7472 2022 220a 0a23 3a20  ".msgstr ""..#: 
-00013cf0: 616c 6c69 616e 6365 6175 7468 2f74 696d  allianceauth/tim
-00013d00: 6572 626f 6172 642f 7465 6d70 6c61 7465  erboard/template
-00013d10: 732f 7469 6d65 7262 6f61 7264 2f74 696d  s/timerboard/tim
-00013d20: 6572 7461 626c 652e 6874 6d6c 3a31 3330  ertable.html:130
-00013d30: 0a6d 7367 6964 2022 536f 7469 796f 220a  .msgid "Sotiyo".
-00013d40: 6d73 6773 7472 2022 220a 0a23 3a20 616c  msgstr ""..#: al
-00013d50: 6c69 616e 6365 6175 7468 2f74 696d 6572  lianceauth/timer
-00013d60: 626f 6172 642f 7465 6d70 6c61 7465 732f  board/templates/
-00013d70: 7469 6d65 7262 6f61 7264 2f74 696d 6572  timerboard/timer
-00013d80: 7461 626c 652e 6874 6d6c 3a31 3336 0a6d  table.html:136.m
-00013d90: 7367 6964 2022 4174 6861 6e6f 7222 0a6d  sgid "Athanor".m
-00013da0: 7367 7374 7220 2222 0a0a 233a 2061 6c6c  sgstr ""..#: all
-00013db0: 6961 6e63 6561 7574 682f 7469 6d65 7262  ianceauth/timerb
-00013dc0: 6f61 7264 2f74 656d 706c 6174 6573 2f74  oard/templates/t
-00013dd0: 696d 6572 626f 6172 642f 7469 6d65 7274  imerboard/timert
-00013de0: 6162 6c65 2e68 746d 6c3a 3134 320a 6d73  able.html:142.ms
-00013df0: 6769 6420 2254 6174 6172 6122 0a6d 7367  gid "Tatara".msg
-00013e00: 7374 7220 2222 0a0a 233a 2061 6c6c 6961  str ""..#: allia
-00013e10: 6e63 6561 7574 682f 7469 6d65 7262 6f61  nceauth/timerboa
-00013e20: 7264 2f74 656d 706c 6174 6573 2f74 696d  rd/templates/tim
-00013e30: 6572 626f 6172 642f 7469 6d65 7274 6162  erboard/timertab
-00013e40: 6c65 2e68 746d 6c3a 3134 380a 6d73 6769  le.html:148.msgi
-00013e50: 6420 2243 796e 6f20 4265 6163 6f6e 220a  d "Cyno Beacon".
-00013e60: 6d73 6773 7472 2022 220a 0a23 3a20 616c  msgstr ""..#: al
-00013e70: 6c69 616e 6365 6175 7468 2f74 696d 6572  lianceauth/timer
-00013e80: 626f 6172 642f 7465 6d70 6c61 7465 732f  board/templates/
-00013e90: 7469 6d65 7262 6f61 7264 2f74 696d 6572  timerboard/timer
-00013ea0: 7461 626c 652e 6874 6d6c 3a31 3534 0a6d  table.html:154.m
-00013eb0: 7367 6964 2022 4379 6e6f 204a 616d 6d65  sgid "Cyno Jamme
-00013ec0: 7222 0a6d 7367 7374 7220 2222 0a0a 233a  r".msgstr ""..#:
-00013ed0: 2061 6c6c 6961 6e63 6561 7574 682f 7469   allianceauth/ti
-00013ee0: 6d65 7262 6f61 7264 2f74 656d 706c 6174  merboard/templat
-00013ef0: 6573 2f74 696d 6572 626f 6172 642f 7469  es/timerboard/ti
-00013f00: 6d65 7274 6162 6c65 2e68 746d 6c3a 3136  mertable.html:16
-00013f10: 300a 6d73 6769 6420 2241 6e73 6962 6c65  0.msgid "Ansible
-00013f20: 7820 4a75 6d70 2047 6174 6522 0a6d 7367  x Jump Gate".msg
-00013f30: 7374 7220 2222 0a0a 233a 2061 6c6c 6961  str ""..#: allia
-00013f40: 6e63 6561 7574 682f 7469 6d65 7262 6f61  nceauth/timerboa
-00013f50: 7264 2f74 656d 706c 6174 6573 2f74 696d  rd/templates/tim
-00013f60: 6572 626f 6172 642f 7469 6d65 7274 6162  erboard/timertab
-00013f70: 6c65 2e68 746d 6c3a 3136 360a 6d73 6769  le.html:166.msgi
-00013f80: 6420 224d 6f6f 6e20 4d69 6e69 6e67 2043  d "Moon Mining C
-00013f90: 7963 6c65 220a 6d73 6773 7472 2022 220a  ycle".msgstr "".
-00013fa0: 0a23 3a20 616c 6c69 616e 6365 6175 7468  .#: allianceauth
-00013fb0: 2f74 696d 6572 626f 6172 642f 7465 6d70  /timerboard/temp
-00013fc0: 6c61 7465 732f 7469 6d65 7262 6f61 7264  lates/timerboard
-00013fd0: 2f76 6965 772e 6874 6d6c 3a39 0a6d 7367  /view.html:9.msg
-00013fe0: 6964 2022 5374 7275 6374 7572 6520 5469  id "Structure Ti
-00013ff0: 6d65 7220 4d61 6e61 6765 6d65 6e74 220a  mer Management".
-00014000: 6d73 6773 7472 2022 220a 0a23 3a20 616c  msgstr ""..#: al
-00014010: 6c69 616e 6365 6175 7468 2f74 696d 6572  lianceauth/timer
-00014020: 626f 6172 642f 7465 6d70 6c61 7465 732f  board/templates/
-00014030: 7469 6d65 7262 6f61 7264 2f76 6965 772e  timerboard/view.
-00014040: 6874 6d6c 3a34 300a 6d73 6769 6420 2243  html:40.msgid "C
-00014050: 6f72 706f 7261 7469 6f6e 2054 696d 6572  orporation Timer
-00014060: 7322 0a6d 7367 7374 7220 2222 0a0a 233a  s".msgstr ""..#:
-00014070: 2061 6c6c 6961 6e63 6561 7574 682f 7469   allianceauth/ti
-00014080: 6d65 7262 6f61 7264 2f74 656d 706c 6174  merboard/templat
-00014090: 6573 2f74 696d 6572 626f 6172 642f 7669  es/timerboard/vi
-000140a0: 6577 2e68 746d 6c3a 3731 0a6d 7367 6964  ew.html:71.msgid
-000140b0: 2022 5061 7374 2054 696d 6572 7322 0a6d   "Past Timers".m
-000140c0: 7367 7374 7220 2222 0a0a 233a 2061 6c6c  sgstr ""..#: all
-000140d0: 6961 6e63 6561 7574 682f 7469 6d65 7262  ianceauth/timerb
-000140e0: 6f61 7264 2f76 6965 7773 2e70 793a 3835  oard/views.py:85
-000140f0: 0a23 2c20 7079 7468 6f6e 2d66 6f72 6d61  .#, python-forma
-00014100: 740a 6d73 6769 6420 2241 6464 6564 206e  t.msgid "Added n
-00014110: 6577 2074 696d 6572 2069 6e20 2528 7379  ew timer in %(sy
-00014120: 7374 656d 2973 2061 7420 2528 7469 6d65  stem)s at %(time
-00014130: 2973 2e22 0a6d 7367 7374 7220 2222 0a0a  )s.".msgstr ""..
-00014140: 233a 2061 6c6c 6961 6e63 6561 7574 682f  #: allianceauth/
-00014150: 7469 6d65 7262 6f61 7264 2f76 6965 7773  timerboard/views
-00014160: 2e70 793a 3935 0a6d 7367 6964 2022 5361  .py:95.msgid "Sa
-00014170: 7665 6420 6368 616e 6765 7320 746f 2074  ved changes to t
-00014180: 6865 2074 696d 6572 2e22 0a6d 7367 7374  he timer.".msgst
-00014190: 7220 2222 0a0a 233a 2061 6c6c 6961 6e63  r ""..#: allianc
-000141a0: 6561 7574 682f 7669 6577 732e 7079 3a35  eauth/views.py:5
-000141b0: 350a 6d73 6769 6420 2242 6164 2052 6571  5.msgid "Bad Req
-000141c0: 7565 7374 220a 6d73 6773 7472 2022 220a  uest".msgstr "".
-000141d0: 0a23 3a20 616c 6c69 616e 6365 6175 7468  .#: allianceauth
-000141e0: 2f76 6965 7773 2e70 793a 3537 2061 6c6c  /views.py:57 all
-000141f0: 6961 6e63 6561 7574 682f 7669 6577 732e  ianceauth/views.
-00014200: 7079 3a38 370a 6d73 6769 6420 2222 0a22  py:87.msgid ""."
-00014210: 4175 7468 2065 6e63 6f75 6e74 6572 6564  Auth encountered
-00014220: 2061 6e20 6572 726f 7220 7072 6f63 6573   an error proces
-00014230: 7369 6e67 2079 6f75 7220 7265 7175 6573  sing your reques
-00014240: 742c 2070 6c65 6173 6520 7472 7920 6167  t, please try ag
-00014250: 6169 6e2e 2049 6620 7468 6520 220a 2265  ain. If the "."e
-00014260: 7272 6f72 2070 6572 7369 7374 732c 2070  rror persists, p
-00014270: 6c65 6173 6520 636f 6e74 6163 7420 7468  lease contact th
-00014280: 6520 6164 6d69 6e69 7374 7261 746f 7273  e administrators
-00014290: 2e22 0a6d 7367 7374 7220 2222 0a0a 233a  .".msgstr ""..#:
-000142a0: 2061 6c6c 6961 6e63 6561 7574 682f 7669   allianceauth/vi
-000142b0: 6577 732e 7079 3a36 350a 6d73 6769 6420  ews.py:65.msgid 
-000142c0: 2250 6572 6d69 7373 696f 6e20 4465 6e69  "Permission Deni
-000142d0: 6564 220a 6d73 6773 7472 2022 220a 0a23  ed".msgstr ""..#
-000142e0: 3a20 616c 6c69 616e 6365 6175 7468 2f76  : allianceauth/v
-000142f0: 6965 7773 2e70 793a 3637 0a6d 7367 6964  iews.py:67.msgid
-00014300: 2022 220a 2259 6f75 2064 6f20 6e6f 7420   ""."You do not 
-00014310: 6861 7665 2070 6572 6d69 7373 696f 6e20  have permission 
-00014320: 746f 2061 6363 6573 7320 7468 6520 7265  to access the re
-00014330: 7175 6573 7465 6420 7061 6765 2e20 4966  quested page. If
-00014340: 2079 6f75 2062 656c 6965 7665 2074 6869   you believe thi
-00014350: 7320 220a 2269 7320 696e 2065 7272 6f72  s "."is in error
-00014360: 2070 6c65 6173 6520 636f 6e74 6163 7420   please contact 
-00014370: 7468 6520 6164 6d69 6e69 7374 7261 746f  the administrato
-00014380: 7273 2e22 0a6d 7367 7374 7220 2222 0a0a  rs.".msgstr ""..
-00014390: 233a 2061 6c6c 6961 6e63 6561 7574 682f  #: allianceauth/
-000143a0: 7669 6577 732e 7079 3a37 350a 6d73 6769  views.py:75.msgi
-000143b0: 6420 2250 6167 6520 4e6f 7420 466f 756e  d "Page Not Foun
-000143c0: 6422 0a6d 7367 7374 7220 2222 0a0a 233a  d".msgstr ""..#:
-000143d0: 2061 6c6c 6961 6e63 6561 7574 682f 7669   allianceauth/vi
-000143e0: 6577 732e 7079 3a37 370a 6d73 6769 6420  ews.py:77.msgid 
-000143f0: 2222 0a22 5061 6765 2064 6f65 7320 6e6f  ""."Page does no
-00014400: 7420 6578 6973 742e 2049 6620 796f 7520  t exist. If you 
-00014410: 6265 6c69 6576 6520 7468 6973 2069 7320  believe this is 
-00014420: 696e 2065 7272 6f72 2070 6c65 6173 6520  in error please 
-00014430: 636f 6e74 6163 7420 7468 6520 220a 2261  contact the "."a
-00014440: 646d 696e 6973 7472 6174 6f72 732e 2022  dministrators. "
-00014450: 0a6d 7367 7374 7220 2222 0a0a 233a 2061  .msgstr ""..#: a
-00014460: 6c6c 6961 6e63 6561 7574 682f 7669 6577  llianceauth/view
-00014470: 732e 7079 3a38 350a 6d73 6769 6420 2249  s.py:85.msgid "I
-00014480: 6e74 6572 6e61 6c20 5365 7276 6572 2045  nternal Server E
-00014490: 7272 6f72 220a 6d73 6773 7472 2022 220a  rror".msgstr "".
+00013230: 6172 642f 6d6f 6465 6c73 2e70 793a 3138  ard/models.py:18
+00013240: 0a6d 7367 6964 2022 4669 6e61 6c22 0a6d  .msgid "Final".m
+00013250: 7367 7374 7220 2222 0a0a 233a 2061 6c6c  sgstr ""..#: all
+00013260: 6961 6e63 6561 7574 682f 7469 6d65 7262  ianceauth/timerb
+00013270: 6f61 7264 2f6d 6f64 656c 732e 7079 3a31  oard/models.py:1
+00013280: 390a 6d73 6769 6420 2241 6e63 686f 7269  9.msgid "Anchori
+00013290: 6e67 220a 6d73 6773 7472 2022 220a 0a23  ng".msgstr ""..#
+000132a0: 3a20 616c 6c69 616e 6365 6175 7468 2f74  : allianceauth/t
+000132b0: 696d 6572 626f 6172 642f 6d6f 6465 6c73  imerboard/models
+000132c0: 2e70 793a 3230 0a6d 7367 6964 2022 556e  .py:20.msgid "Un
+000132d0: 616e 6368 6f72 696e 6722 0a6d 7367 7374  anchoring".msgst
+000132e0: 7220 2222 0a0a 233a 2061 6c6c 6961 6e63  r ""..#: allianc
+000132f0: 6561 7574 682f 7469 6d65 7262 6f61 7264  eauth/timerboard
+00013300: 2f74 656d 706c 6174 6573 2f74 696d 6572  /templates/timer
+00013310: 626f 6172 642f 6461 7368 626f 6172 642e  board/dashboard.
+00013320: 7469 6d65 7273 2e68 746d 6c3a 370a 233a  timers.html:7.#:
+00013330: 2061 6c6c 6961 6e63 6561 7574 682f 7469   allianceauth/ti
+00013340: 6d65 7262 6f61 7264 2f74 656d 706c 6174  merboard/templat
+00013350: 6573 2f74 696d 6572 626f 6172 642f 7669  es/timerboard/vi
+00013360: 6577 2e68 746d 6c3a 3533 0a6d 7367 6964  ew.html:53.msgid
+00013370: 2022 5570 636f 6d69 6e67 2054 696d 6572   "Upcoming Timer
+00013380: 7322 0a6d 7367 7374 7220 2222 0a0a 233a  s".msgstr ""..#:
+00013390: 2061 6c6c 6961 6e63 6561 7574 682f 7469   allianceauth/ti
+000133a0: 6d65 7262 6f61 7264 2f74 656d 706c 6174  merboard/templat
+000133b0: 6573 2f74 696d 6572 626f 6172 642f 6461  es/timerboard/da
+000133c0: 7368 626f 6172 642e 7469 6d65 7273 2e68  shboard.timers.h
+000133d0: 746d 6c3a 3134 0a6d 7367 6964 2022 5469  tml:14.msgid "Ti
+000133e0: 6d65 7222 0a6d 7367 7374 7220 2222 0a0a  mer".msgstr ""..
+000133f0: 233a 2061 6c6c 6961 6e63 6561 7574 682f  #: allianceauth/
+00013400: 7469 6d65 7262 6f61 7264 2f74 656d 706c  timerboard/templ
+00013410: 6174 6573 2f74 696d 6572 626f 6172 642f  ates/timerboard/
+00013420: 666f 726d 2e68 746d 6c3a 3130 0a23 3a20  form.html:10.#: 
+00013430: 616c 6c69 616e 6365 6175 7468 2f74 696d  allianceauth/tim
+00013440: 6572 626f 6172 642f 7465 6d70 6c61 7465  erboard/template
+00013450: 732f 7469 6d65 7262 6f61 7264 2f74 696d  s/timerboard/tim
+00013460: 6572 5f63 6f6e 6669 726d 5f64 656c 6574  er_confirm_delet
+00013470: 652e 6874 6d6c 3a31 300a 233a 2061 6c6c  e.html:10.#: all
+00013480: 6961 6e63 6561 7574 682f 7469 6d65 7262  ianceauth/timerb
+00013490: 6f61 7264 2f74 656d 706c 6174 6573 2f74  oard/templates/t
+000134a0: 696d 6572 626f 6172 642f 7669 6577 2e68  imerboard/view.h
+000134b0: 746d 6c3a 3133 0a6d 7367 6964 2022 5374  tml:13.msgid "St
+000134c0: 7275 6374 7572 6520 5469 6d65 7273 220a  ructure Timers".
+000134d0: 6d73 6773 7472 2022 220a 0a23 3a20 616c  msgstr ""..#: al
+000134e0: 6c69 616e 6365 6175 7468 2f74 696d 6572  lianceauth/timer
+000134f0: 626f 6172 642f 7465 6d70 6c61 7465 732f  board/templates/
+00013500: 7469 6d65 7262 6f61 7264 2f66 6f72 6d2e  timerboard/form.
+00013510: 6874 6d6c 3a32 350a 6d73 6769 6420 2253  html:25.msgid "S
+00013520: 7472 7563 7475 7265 2054 696d 6572 2044  tructure Timer D
+00013530: 6574 6169 6c73 220a 6d73 6773 7472 2022  etails".msgstr "
+00013540: 220a 0a23 3a20 616c 6c69 616e 6365 6175  "..#: allianceau
+00013550: 7468 2f74 696d 6572 626f 6172 642f 7465  th/timerboard/te
+00013560: 6d70 6c61 7465 732f 7469 6d65 7262 6f61  mplates/timerboa
+00013570: 7264 2f74 696d 6572 5f63 6f6e 6669 726d  rd/timer_confirm
+00013580: 5f64 656c 6574 652e 6874 6d6c 3a36 0a23  _delete.html:6.#
+00013590: 3a20 616c 6c69 616e 6365 6175 7468 2f74  : allianceauth/t
+000135a0: 696d 6572 626f 6172 642f 7465 6d70 6c61  imerboard/templa
+000135b0: 7465 732f 7469 6d65 7262 6f61 7264 2f74  tes/timerboard/t
+000135c0: 696d 6572 5f63 6f6e 6669 726d 5f64 656c  imer_confirm_del
+000135d0: 6574 652e 6874 6d6c 3a31 350a 6d73 6769  ete.html:15.msgi
+000135e0: 6420 2244 656c 6574 6520 5469 6d65 7222  d "Delete Timer"
+000135f0: 0a6d 7367 7374 7220 2222 0a0a 233a 2061  .msgstr ""..#: a
+00013600: 6c6c 6961 6e63 6561 7574 682f 7469 6d65  llianceauth/time
+00013610: 7262 6f61 7264 2f74 656d 706c 6174 6573  rboard/templates
+00013620: 2f74 696d 6572 626f 6172 642f 7469 6d65  /timerboard/time
+00013630: 725f 636f 6e66 6972 6d5f 6465 6c65 7465  r_confirm_delete
+00013640: 2e68 746d 6c3a 3236 0a23 2c20 7079 7468  .html:26.#, pyth
+00013650: 6f6e 2d66 6f72 6d61 740a 6d73 6769 6420  on-format.msgid 
+00013660: 2241 7265 2079 6f75 2073 7572 6520 796f  "Are you sure yo
+00013670: 7520 7761 6e74 2074 6f20 6465 6c65 7465  u want to delete
+00013680: 2074 696d 6572 205c 2225 286f 626a 6563   timer \"%(objec
+00013690: 7429 735c 223f 220a 6d73 6773 7472 2022  t)s\"?".msgstr "
+000136a0: 220a 0a23 3a20 616c 6c69 616e 6365 6175  "..#: allianceau
+000136b0: 7468 2f74 696d 6572 626f 6172 642f 7465  th/timerboard/te
+000136c0: 6d70 6c61 7465 732f 7469 6d65 7262 6f61  mplates/timerboa
+000136d0: 7264 2f74 696d 6572 5f63 7265 6174 655f  rd/timer_create_
+000136e0: 666f 726d 2e68 746d 6c3a 350a 233a 2061  form.html:5.#: a
+000136f0: 6c6c 6961 6e63 6561 7574 682f 7469 6d65  llianceauth/time
+00013700: 7262 6f61 7264 2f74 656d 706c 6174 6573  rboard/templates
+00013710: 2f74 696d 6572 626f 6172 642f 7469 6d65  /timerboard/time
+00013720: 725f 6372 6561 7465 5f66 6f72 6d2e 6874  r_create_form.ht
+00013730: 6d6c 3a31 330a 6d73 6769 6420 2243 7265  ml:13.msgid "Cre
+00013740: 6174 6520 5469 6d65 7222 0a6d 7367 7374  ate Timer".msgst
+00013750: 7220 2222 0a0a 233a 2061 6c6c 6961 6e63  r ""..#: allianc
+00013760: 6561 7574 682f 7469 6d65 7262 6f61 7264  eauth/timerboard
+00013770: 2f74 656d 706c 6174 6573 2f74 696d 6572  /templates/timer
+00013780: 626f 6172 642f 7469 6d65 725f 6372 6561  board/timer_crea
+00013790: 7465 5f66 6f72 6d2e 6874 6d6c 3a39 0a23  te_form.html:9.#
+000137a0: 3a20 616c 6c69 616e 6365 6175 7468 2f74  : allianceauth/t
+000137b0: 696d 6572 626f 6172 642f 7465 6d70 6c61  imerboard/templa
+000137c0: 7465 732f 7469 6d65 7262 6f61 7264 2f76  tes/timerboard/v
+000137d0: 6965 772e 6874 6d6c 3a32 310a 6d73 6769  iew.html:21.msgi
+000137e0: 6420 2243 7265 6174 6520 5374 7275 6374  d "Create Struct
+000137f0: 7572 6520 5469 6d65 7222 0a6d 7367 7374  ure Timer".msgst
+00013800: 7220 2222 0a0a 233a 2061 6c6c 6961 6e63  r ""..#: allianc
+00013810: 6561 7574 682f 7469 6d65 7262 6f61 7264  eauth/timerboard
+00013820: 2f74 656d 706c 6174 6573 2f74 696d 6572  /templates/timer
+00013830: 626f 6172 642f 7469 6d65 725f 7570 6461  board/timer_upda
+00013840: 7465 5f66 6f72 6d2e 6874 6d6c 3a35 0a23  te_form.html:5.#
+00013850: 3a20 616c 6c69 616e 6365 6175 7468 2f74  : allianceauth/t
+00013860: 696d 6572 626f 6172 642f 7465 6d70 6c61  imerboard/templa
+00013870: 7465 732f 7469 6d65 7262 6f61 7264 2f74  tes/timerboard/t
+00013880: 696d 6572 5f75 7064 6174 655f 666f 726d  imer_update_form
+00013890: 2e68 746d 6c3a 390a 233a 2061 6c6c 6961  .html:9.#: allia
+000138a0: 6e63 6561 7574 682f 7469 6d65 7262 6f61  nceauth/timerboa
+000138b0: 7264 2f74 656d 706c 6174 6573 2f74 696d  rd/templates/tim
+000138c0: 6572 626f 6172 642f 7469 6d65 725f 7570  erboard/timer_up
+000138d0: 6461 7465 5f66 6f72 6d2e 6874 6d6c 3a31  date_form.html:1
+000138e0: 330a 6d73 6769 6420 2255 7064 6174 6520  3.msgid "Update 
+000138f0: 5374 7275 6374 7572 6520 5469 6d65 7222  Structure Timer"
+00013900: 0a6d 7367 7374 7220 2222 0a0a 233a 2061  .msgstr ""..#: a
+00013910: 6c6c 6961 6e63 6561 7574 682f 7469 6d65  llianceauth/time
+00013920: 7262 6f61 7264 2f74 656d 706c 6174 6573  rboard/templates
+00013930: 2f74 696d 6572 626f 6172 642f 7469 6d65  /timerboard/time
+00013940: 7274 6162 6c65 2e68 746d 6c3a 3130 0a6d  rtable.html:10.m
+00013950: 7367 6964 2022 5374 7275 6374 7572 6522  sgid "Structure"
+00013960: 0a6d 7367 7374 7220 2222 0a0a 233a 2061  .msgstr ""..#: a
+00013970: 6c6c 6961 6e63 6561 7574 682f 7469 6d65  llianceauth/time
+00013980: 7262 6f61 7264 2f74 656d 706c 6174 6573  rboard/templates
+00013990: 2f74 696d 6572 626f 6172 642f 7469 6d65  /timerboard/time
+000139a0: 7274 6162 6c65 2e68 746d 6c3a 3634 0a6d  rtable.html:64.m
+000139b0: 7367 6964 2022 504f 434f 220a 6d73 6773  sgid "POCO".msgs
+000139c0: 7472 2022 220a 0a23 3a20 616c 6c69 616e  tr ""..#: allian
+000139d0: 6365 6175 7468 2f74 696d 6572 626f 6172  ceauth/timerboar
+000139e0: 642f 7465 6d70 6c61 7465 732f 7469 6d65  d/templates/time
+000139f0: 7262 6f61 7264 2f74 696d 6572 7461 626c  rboard/timertabl
+00013a00: 652e 6874 6d6c 3a37 300a 6d73 6769 6420  e.html:70.msgid 
+00013a10: 2249 2d48 5542 220a 6d73 6773 7472 2022  "I-HUB".msgstr "
+00013a20: 220a 0a23 3a20 616c 6c69 616e 6365 6175  "..#: allianceau
+00013a30: 7468 2f74 696d 6572 626f 6172 642f 7465  th/timerboard/te
+00013a40: 6d70 6c61 7465 732f 7469 6d65 7262 6f61  mplates/timerboa
+00013a50: 7264 2f74 696d 6572 7461 626c 652e 6874  rd/timertable.ht
+00013a60: 6d6c 3a37 360a 6d73 6769 6420 2254 4355  ml:76.msgid "TCU
+00013a70: 220a 6d73 6773 7472 2022 220a 0a23 3a20  ".msgstr ""..#: 
+00013a80: 616c 6c69 616e 6365 6175 7468 2f74 696d  allianceauth/tim
+00013a90: 6572 626f 6172 642f 7465 6d70 6c61 7465  erboard/template
+00013aa0: 732f 7469 6d65 7262 6f61 7264 2f74 696d  s/timerboard/tim
+00013ab0: 6572 7461 626c 652e 6874 6d6c 3a38 320a  ertable.html:82.
+00013ac0: 6d73 6769 6420 2250 4f53 205b 535d 220a  msgid "POS [S]".
+00013ad0: 6d73 6773 7472 2022 220a 0a23 3a20 616c  msgstr ""..#: al
+00013ae0: 6c69 616e 6365 6175 7468 2f74 696d 6572  lianceauth/timer
+00013af0: 626f 6172 642f 7465 6d70 6c61 7465 732f  board/templates/
+00013b00: 7469 6d65 7262 6f61 7264 2f74 696d 6572  timerboard/timer
+00013b10: 7461 626c 652e 6874 6d6c 3a38 380a 6d73  table.html:88.ms
+00013b20: 6769 6420 2250 4f53 205b 4d5d 220a 6d73  gid "POS [M]".ms
+00013b30: 6773 7472 2022 220a 0a23 3a20 616c 6c69  gstr ""..#: alli
+00013b40: 616e 6365 6175 7468 2f74 696d 6572 626f  anceauth/timerbo
+00013b50: 6172 642f 7465 6d70 6c61 7465 732f 7469  ard/templates/ti
+00013b60: 6d65 7262 6f61 7264 2f74 696d 6572 7461  merboard/timerta
+00013b70: 626c 652e 6874 6d6c 3a39 340a 6d73 6769  ble.html:94.msgi
+00013b80: 6420 2250 4f53 205b 4c5d 220a 6d73 6773  d "POS [L]".msgs
+00013b90: 7472 2022 220a 0a23 3a20 616c 6c69 616e  tr ""..#: allian
+00013ba0: 6365 6175 7468 2f74 696d 6572 626f 6172  ceauth/timerboar
+00013bb0: 642f 7465 6d70 6c61 7465 732f 7469 6d65  d/templates/time
+00013bc0: 7262 6f61 7264 2f74 696d 6572 7461 626c  rboard/timertabl
+00013bd0: 652e 6874 6d6c 3a31 3030 0a6d 7367 6964  e.html:100.msgid
+00013be0: 2022 4173 7472 6168 7573 220a 6d73 6773   "Astrahus".msgs
+00013bf0: 7472 2022 220a 0a23 3a20 616c 6c69 616e  tr ""..#: allian
+00013c00: 6365 6175 7468 2f74 696d 6572 626f 6172  ceauth/timerboar
+00013c10: 642f 7465 6d70 6c61 7465 732f 7469 6d65  d/templates/time
+00013c20: 7262 6f61 7264 2f74 696d 6572 7461 626c  rboard/timertabl
+00013c30: 652e 6874 6d6c 3a31 3036 0a6d 7367 6964  e.html:106.msgid
+00013c40: 2022 466f 7274 697a 6172 220a 6d73 6773   "Fortizar".msgs
+00013c50: 7472 2022 220a 0a23 3a20 616c 6c69 616e  tr ""..#: allian
+00013c60: 6365 6175 7468 2f74 696d 6572 626f 6172  ceauth/timerboar
+00013c70: 642f 7465 6d70 6c61 7465 732f 7469 6d65  d/templates/time
+00013c80: 7262 6f61 7264 2f74 696d 6572 7461 626c  rboard/timertabl
+00013c90: 652e 6874 6d6c 3a31 3132 0a6d 7367 6964  e.html:112.msgid
+00013ca0: 2022 4b65 6570 7374 6172 220a 6d73 6773   "Keepstar".msgs
+00013cb0: 7472 2022 220a 0a23 3a20 616c 6c69 616e  tr ""..#: allian
+00013cc0: 6365 6175 7468 2f74 696d 6572 626f 6172  ceauth/timerboar
+00013cd0: 642f 7465 6d70 6c61 7465 732f 7469 6d65  d/templates/time
+00013ce0: 7262 6f61 7264 2f74 696d 6572 7461 626c  rboard/timertabl
+00013cf0: 652e 6874 6d6c 3a31 3138 0a6d 7367 6964  e.html:118.msgid
+00013d00: 2022 5261 6974 6172 7522 0a6d 7367 7374   "Raitaru".msgst
+00013d10: 7220 2222 0a0a 233a 2061 6c6c 6961 6e63  r ""..#: allianc
+00013d20: 6561 7574 682f 7469 6d65 7262 6f61 7264  eauth/timerboard
+00013d30: 2f74 656d 706c 6174 6573 2f74 696d 6572  /templates/timer
+00013d40: 626f 6172 642f 7469 6d65 7274 6162 6c65  board/timertable
+00013d50: 2e68 746d 6c3a 3132 340a 6d73 6769 6420  .html:124.msgid 
+00013d60: 2241 7a62 656c 220a 6d73 6773 7472 2022  "Azbel".msgstr "
+00013d70: 220a 0a23 3a20 616c 6c69 616e 6365 6175  "..#: allianceau
+00013d80: 7468 2f74 696d 6572 626f 6172 642f 7465  th/timerboard/te
+00013d90: 6d70 6c61 7465 732f 7469 6d65 7262 6f61  mplates/timerboa
+00013da0: 7264 2f74 696d 6572 7461 626c 652e 6874  rd/timertable.ht
+00013db0: 6d6c 3a31 3330 0a6d 7367 6964 2022 536f  ml:130.msgid "So
+00013dc0: 7469 796f 220a 6d73 6773 7472 2022 220a  tiyo".msgstr "".
+00013dd0: 0a23 3a20 616c 6c69 616e 6365 6175 7468  .#: allianceauth
+00013de0: 2f74 696d 6572 626f 6172 642f 7465 6d70  /timerboard/temp
+00013df0: 6c61 7465 732f 7469 6d65 7262 6f61 7264  lates/timerboard
+00013e00: 2f74 696d 6572 7461 626c 652e 6874 6d6c  /timertable.html
+00013e10: 3a31 3336 0a6d 7367 6964 2022 4174 6861  :136.msgid "Atha
+00013e20: 6e6f 7222 0a6d 7367 7374 7220 2222 0a0a  nor".msgstr ""..
+00013e30: 233a 2061 6c6c 6961 6e63 6561 7574 682f  #: allianceauth/
+00013e40: 7469 6d65 7262 6f61 7264 2f74 656d 706c  timerboard/templ
+00013e50: 6174 6573 2f74 696d 6572 626f 6172 642f  ates/timerboard/
+00013e60: 7469 6d65 7274 6162 6c65 2e68 746d 6c3a  timertable.html:
+00013e70: 3134 320a 6d73 6769 6420 2254 6174 6172  142.msgid "Tatar
+00013e80: 6122 0a6d 7367 7374 7220 2222 0a0a 233a  a".msgstr ""..#:
+00013e90: 2061 6c6c 6961 6e63 6561 7574 682f 7469   allianceauth/ti
+00013ea0: 6d65 7262 6f61 7264 2f74 656d 706c 6174  merboard/templat
+00013eb0: 6573 2f74 696d 6572 626f 6172 642f 7469  es/timerboard/ti
+00013ec0: 6d65 7274 6162 6c65 2e68 746d 6c3a 3134  mertable.html:14
+00013ed0: 380a 6d73 6769 6420 2243 796e 6f20 4265  8.msgid "Cyno Be
+00013ee0: 6163 6f6e 220a 6d73 6773 7472 2022 220a  acon".msgstr "".
+00013ef0: 0a23 3a20 616c 6c69 616e 6365 6175 7468  .#: allianceauth
+00013f00: 2f74 696d 6572 626f 6172 642f 7465 6d70  /timerboard/temp
+00013f10: 6c61 7465 732f 7469 6d65 7262 6f61 7264  lates/timerboard
+00013f20: 2f74 696d 6572 7461 626c 652e 6874 6d6c  /timertable.html
+00013f30: 3a31 3534 0a6d 7367 6964 2022 4379 6e6f  :154.msgid "Cyno
+00013f40: 204a 616d 6d65 7222 0a6d 7367 7374 7220   Jammer".msgstr 
+00013f50: 2222 0a0a 233a 2061 6c6c 6961 6e63 6561  ""..#: alliancea
+00013f60: 7574 682f 7469 6d65 7262 6f61 7264 2f74  uth/timerboard/t
+00013f70: 656d 706c 6174 6573 2f74 696d 6572 626f  emplates/timerbo
+00013f80: 6172 642f 7469 6d65 7274 6162 6c65 2e68  ard/timertable.h
+00013f90: 746d 6c3a 3136 300a 6d73 6769 6420 2241  tml:160.msgid "A
+00013fa0: 6e73 6962 6c65 7820 4a75 6d70 2047 6174  nsiblex Jump Gat
+00013fb0: 6522 0a6d 7367 7374 7220 2222 0a0a 233a  e".msgstr ""..#:
+00013fc0: 2061 6c6c 6961 6e63 6561 7574 682f 7469   allianceauth/ti
+00013fd0: 6d65 7262 6f61 7264 2f74 656d 706c 6174  merboard/templat
+00013fe0: 6573 2f74 696d 6572 626f 6172 642f 7469  es/timerboard/ti
+00013ff0: 6d65 7274 6162 6c65 2e68 746d 6c3a 3136  mertable.html:16
+00014000: 360a 6d73 6769 6420 224d 6f6f 6e20 4d69  6.msgid "Moon Mi
+00014010: 6e69 6e67 2043 7963 6c65 220a 6d73 6773  ning Cycle".msgs
+00014020: 7472 2022 220a 0a23 3a20 616c 6c69 616e  tr ""..#: allian
+00014030: 6365 6175 7468 2f74 696d 6572 626f 6172  ceauth/timerboar
+00014040: 642f 7465 6d70 6c61 7465 732f 7469 6d65  d/templates/time
+00014050: 7262 6f61 7264 2f76 6965 772e 6874 6d6c  rboard/view.html
+00014060: 3a39 0a6d 7367 6964 2022 5374 7275 6374  :9.msgid "Struct
+00014070: 7572 6520 5469 6d65 7220 4d61 6e61 6765  ure Timer Manage
+00014080: 6d65 6e74 220a 6d73 6773 7472 2022 220a  ment".msgstr "".
+00014090: 0a23 3a20 616c 6c69 616e 6365 6175 7468  .#: allianceauth
+000140a0: 2f74 696d 6572 626f 6172 642f 7465 6d70  /timerboard/temp
+000140b0: 6c61 7465 732f 7469 6d65 7262 6f61 7264  lates/timerboard
+000140c0: 2f76 6965 772e 6874 6d6c 3a34 300a 6d73  /view.html:40.ms
+000140d0: 6769 6420 2243 6f72 706f 7261 7469 6f6e  gid "Corporation
+000140e0: 2054 696d 6572 7322 0a6d 7367 7374 7220   Timers".msgstr 
+000140f0: 2222 0a0a 233a 2061 6c6c 6961 6e63 6561  ""..#: alliancea
+00014100: 7574 682f 7469 6d65 7262 6f61 7264 2f74  uth/timerboard/t
+00014110: 656d 706c 6174 6573 2f74 696d 6572 626f  emplates/timerbo
+00014120: 6172 642f 7669 6577 2e68 746d 6c3a 3731  ard/view.html:71
+00014130: 0a6d 7367 6964 2022 5061 7374 2054 696d  .msgid "Past Tim
+00014140: 6572 7322 0a6d 7367 7374 7220 2222 0a0a  ers".msgstr ""..
+00014150: 233a 2061 6c6c 6961 6e63 6561 7574 682f  #: allianceauth/
+00014160: 7469 6d65 7262 6f61 7264 2f76 6965 7773  timerboard/views
+00014170: 2e70 793a 3835 0a23 2c20 7079 7468 6f6e  .py:85.#, python
+00014180: 2d66 6f72 6d61 740a 6d73 6769 6420 2241  -format.msgid "A
+00014190: 6464 6564 206e 6577 2074 696d 6572 2069  dded new timer i
+000141a0: 6e20 2528 7379 7374 656d 2973 2061 7420  n %(system)s at 
+000141b0: 2528 7469 6d65 2973 2e22 0a6d 7367 7374  %(time)s.".msgst
+000141c0: 7220 2222 0a0a 233a 2061 6c6c 6961 6e63  r ""..#: allianc
+000141d0: 6561 7574 682f 7469 6d65 7262 6f61 7264  eauth/timerboard
+000141e0: 2f76 6965 7773 2e70 793a 3935 0a6d 7367  /views.py:95.msg
+000141f0: 6964 2022 5361 7665 6420 6368 616e 6765  id "Saved change
+00014200: 7320 746f 2074 6865 2074 696d 6572 2e22  s to the timer."
+00014210: 0a6d 7367 7374 7220 2222 0a0a 233a 2061  .msgstr ""..#: a
+00014220: 6c6c 6961 6e63 6561 7574 682f 7669 6577  llianceauth/view
+00014230: 732e 7079 3a35 350a 6d73 6769 6420 2242  s.py:55.msgid "B
+00014240: 6164 2052 6571 7565 7374 220a 6d73 6773  ad Request".msgs
+00014250: 7472 2022 220a 0a23 3a20 616c 6c69 616e  tr ""..#: allian
+00014260: 6365 6175 7468 2f76 6965 7773 2e70 793a  ceauth/views.py:
+00014270: 3537 2061 6c6c 6961 6e63 6561 7574 682f  57 allianceauth/
+00014280: 7669 6577 732e 7079 3a38 370a 6d73 6769  views.py:87.msgi
+00014290: 6420 2222 0a22 4175 7468 2065 6e63 6f75  d ""."Auth encou
+000142a0: 6e74 6572 6564 2061 6e20 6572 726f 7220  ntered an error 
+000142b0: 7072 6f63 6573 7369 6e67 2079 6f75 7220  processing your 
+000142c0: 7265 7175 6573 742c 2070 6c65 6173 6520  request, please 
+000142d0: 7472 7920 6167 6169 6e2e 2049 6620 7468  try again. If th
+000142e0: 6520 220a 2265 7272 6f72 2070 6572 7369  e "."error persi
+000142f0: 7374 732c 2070 6c65 6173 6520 636f 6e74  sts, please cont
+00014300: 6163 7420 7468 6520 6164 6d69 6e69 7374  act the administ
+00014310: 7261 746f 7273 2e22 0a6d 7367 7374 7220  rators.".msgstr 
+00014320: 2222 0a0a 233a 2061 6c6c 6961 6e63 6561  ""..#: alliancea
+00014330: 7574 682f 7669 6577 732e 7079 3a36 350a  uth/views.py:65.
+00014340: 6d73 6769 6420 2250 6572 6d69 7373 696f  msgid "Permissio
+00014350: 6e20 4465 6e69 6564 220a 6d73 6773 7472  n Denied".msgstr
+00014360: 2022 220a 0a23 3a20 616c 6c69 616e 6365   ""..#: alliance
+00014370: 6175 7468 2f76 6965 7773 2e70 793a 3637  auth/views.py:67
+00014380: 0a6d 7367 6964 2022 220a 2259 6f75 2064  .msgid ""."You d
+00014390: 6f20 6e6f 7420 6861 7665 2070 6572 6d69  o not have permi
+000143a0: 7373 696f 6e20 746f 2061 6363 6573 7320  ssion to access 
+000143b0: 7468 6520 7265 7175 6573 7465 6420 7061  the requested pa
+000143c0: 6765 2e20 4966 2079 6f75 2062 656c 6965  ge. If you belie
+000143d0: 7665 2074 6869 7320 220a 2269 7320 696e  ve this "."is in
+000143e0: 2065 7272 6f72 2070 6c65 6173 6520 636f   error please co
+000143f0: 6e74 6163 7420 7468 6520 6164 6d69 6e69  ntact the admini
+00014400: 7374 7261 746f 7273 2e22 0a6d 7367 7374  strators.".msgst
+00014410: 7220 2222 0a0a 233a 2061 6c6c 6961 6e63  r ""..#: allianc
+00014420: 6561 7574 682f 7669 6577 732e 7079 3a37  eauth/views.py:7
+00014430: 350a 6d73 6769 6420 2250 6167 6520 4e6f  5.msgid "Page No
+00014440: 7420 466f 756e 6422 0a6d 7367 7374 7220  t Found".msgstr 
+00014450: 2222 0a0a 233a 2061 6c6c 6961 6e63 6561  ""..#: alliancea
+00014460: 7574 682f 7669 6577 732e 7079 3a37 370a  uth/views.py:77.
+00014470: 6d73 6769 6420 2222 0a22 5061 6765 2064  msgid ""."Page d
+00014480: 6f65 7320 6e6f 7420 6578 6973 742e 2049  oes not exist. I
+00014490: 6620 796f 7520 6265 6c69 6576 6520 7468  f you believe th
+000144a0: 6973 2069 7320 696e 2065 7272 6f72 2070  is is in error p
+000144b0: 6c65 6173 6520 636f 6e74 6163 7420 7468  lease contact th
+000144c0: 6520 220a 2261 646d 696e 6973 7472 6174  e "."administrat
+000144d0: 6f72 732e 2022 0a6d 7367 7374 7220 2222  ors. ".msgstr ""
+000144e0: 0a0a 233a 2061 6c6c 6961 6e63 6561 7574  ..#: allianceaut
+000144f0: 682f 7669 6577 732e 7079 3a38 350a 6d73  h/views.py:85.ms
+00014500: 6769 6420 2249 6e74 6572 6e61 6c20 5365  gid "Internal Se
+00014510: 7276 6572 2045 7272 6f72 220a 6d73 6773  rver Error".msgs
+00014520: 7472 2022 220a                           tr "".
```

### Comparing `allianceauth-4.0.1/allianceauth/locale/es/LC_MESSAGES/django.mo` & `allianceauth-4.0.2/allianceauth/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/locale/es/LC_MESSAGES/django.po` & `allianceauth-4.0.2/allianceauth/locale/es/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # trenus, 2023
 # 
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-03-13 19:10+1000\n"
+"POT-Creation-Date: 2024-05-12 19:15+1000\n"
 "PO-Revision-Date: 2023-11-08 13:50+0000\n"
 "Last-Translator: trenus, 2023\n"
 "Language-Team: Spanish (https://app.transifex.com/alliance-auth/teams/107430/es/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: es\n"
@@ -1435,14 +1435,16 @@
 msgstr "Administrador"
 
 #: allianceauth/menu/templates/menu/menu-user.html:80
 msgid "Sign Out"
 msgstr ""
 
 #: allianceauth/menu/templates/menu/menu-user.html:84
+#: allianceauth/templates/allianceauth/top-menu-rh-default.html:17
+#: allianceauth/templates/allianceauth/top-menu-rh-default.html:18
 msgid "Sign In"
 msgstr ""
 
 #: allianceauth/notifications/models.py:21
 msgid "danger"
 msgstr "peligro"
```

### Comparing `allianceauth-4.0.1/allianceauth/locale/fr_FR/LC_MESSAGES/django.mo` & `allianceauth-4.0.2/allianceauth/locale/fr_FR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/locale/fr_FR/LC_MESSAGES/django.po` & `allianceauth-4.0.2/allianceauth/locale/fr_FR/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
-#
+# 
 # Translators:
 # Mickael Gr4vity, 2023
 # rockclodbuster, 2023
 # Keven D. <theenarki@gmail.com>, 2023
 # Mohssine Daghghar, 2023
 # Philippe Querin-Laporte <philippe.querin@hotmail.com>, 2023
 # draktanar KarazGrong <umbre@fallenstarscreations.com>, 2023
 # Geoffrey Fabbro, 2023
 # Idea, 2024
-#
+# Joel Falknau <ozirascal@gmail.com>, 2024
+# 
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-03-13 19:10+1000\n"
+"POT-Creation-Date: 2024-05-12 19:15+1000\n"
 "PO-Revision-Date: 2023-11-08 13:50+0000\n"
-"Last-Translator: Idea, 2024\n"
+"Last-Translator: Joel Falknau <ozirascal@gmail.com>, 2024\n"
 "Language-Team: French (France) (https://app.transifex.com/alliance-auth/teams/107430/fr_FR/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: fr_FR\n"
 "Plural-Forms: nplurals=3; plural=(n == 0 || n == 1) ? 0 : n != 0 && n % 1000000 == 0 ? 1 : 2;\n"
 
@@ -1454,14 +1455,16 @@
 msgstr "Administrateur"
 
 #: allianceauth/menu/templates/menu/menu-user.html:80
 msgid "Sign Out"
 msgstr "Se Déconnecter"
 
 #: allianceauth/menu/templates/menu/menu-user.html:84
+#: allianceauth/templates/allianceauth/top-menu-rh-default.html:17
+#: allianceauth/templates/allianceauth/top-menu-rh-default.html:18
 msgid "Sign In"
 msgstr "Se Connecter"
 
 #: allianceauth/notifications/models.py:21
 msgid "danger"
 msgstr "danger"
```

### Comparing `allianceauth-4.0.1/allianceauth/locale/it_IT/LC_MESSAGES/django.mo` & `allianceauth-4.0.2/allianceauth/locale/it_IT/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/locale/it_IT/LC_MESSAGES/django.po` & `allianceauth-4.0.2/allianceauth/locale/it_IT/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -2,24 +2,24 @@
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 # 
 # Translators:
 # Alessandro Cresti, 2023
 # Linus Hope, 2023
-# Thomas Turini, 2024
+# Tuz, 2024
 # 
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-03-13 19:10+1000\n"
+"POT-Creation-Date: 2024-05-12 19:15+1000\n"
 "PO-Revision-Date: 2023-11-08 13:50+0000\n"
-"Last-Translator: Thomas Turini, 2024\n"
+"Last-Translator: Tuz, 2024\n"
 "Language-Team: Italian (Italy) (https://app.transifex.com/alliance-auth/teams/107430/it_IT/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: it_IT\n"
 "Plural-Forms: nplurals=3; plural=n == 1 ? 0 : n != 0 && n % 1000000 == 0 ? 1 : 2;\n"
 
@@ -1452,14 +1452,16 @@
 msgstr "Amministratore"
 
 #: allianceauth/menu/templates/menu/menu-user.html:80
 msgid "Sign Out"
 msgstr "Sign Out"
 
 #: allianceauth/menu/templates/menu/menu-user.html:84
+#: allianceauth/templates/allianceauth/top-menu-rh-default.html:17
+#: allianceauth/templates/allianceauth/top-menu-rh-default.html:18
 msgid "Sign In"
 msgstr "Sign In"
 
 #: allianceauth/notifications/models.py:21
 msgid "danger"
 msgstr "pericolo"
```

### Comparing `allianceauth-4.0.1/allianceauth/locale/ja/LC_MESSAGES/django.mo` & `allianceauth-4.0.2/allianceauth/locale/ja/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/locale/ja/LC_MESSAGES/django.po` & `allianceauth-4.0.2/allianceauth/locale/ja/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # kotaneko, 2024
 # 
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-03-13 19:10+1000\n"
+"POT-Creation-Date: 2024-05-12 19:15+1000\n"
 "PO-Revision-Date: 2023-11-08 13:50+0000\n"
 "Last-Translator: kotaneko, 2024\n"
 "Language-Team: Japanese (https://app.transifex.com/alliance-auth/teams/107430/ja/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: ja\n"
@@ -1401,14 +1401,16 @@
 msgstr "管理者"
 
 #: allianceauth/menu/templates/menu/menu-user.html:80
 msgid "Sign Out"
 msgstr "サインアウト"
 
 #: allianceauth/menu/templates/menu/menu-user.html:84
+#: allianceauth/templates/allianceauth/top-menu-rh-default.html:17
+#: allianceauth/templates/allianceauth/top-menu-rh-default.html:18
 msgid "Sign In"
 msgstr "サインイン"
 
 #: allianceauth/notifications/models.py:21
 msgid "danger"
 msgstr "危険"
```

### Comparing `allianceauth-4.0.1/allianceauth/locale/ko_KR/LC_MESSAGES/django.mo` & `allianceauth-4.0.2/allianceauth/locale/ko_KR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/locale/ko_KR/LC_MESSAGES/django.po` & `allianceauth-4.0.2/allianceauth/locale/ko_KR/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Woojin Kang, 2024
 # 
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-03-13 19:10+1000\n"
+"POT-Creation-Date: 2024-05-12 19:15+1000\n"
 "PO-Revision-Date: 2023-11-08 13:50+0000\n"
 "Last-Translator: Woojin Kang, 2024\n"
 "Language-Team: Korean (Korea) (https://app.transifex.com/alliance-auth/teams/107430/ko_KR/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: ko_KR\n"
@@ -1410,14 +1410,16 @@
 msgstr "어드민"
 
 #: allianceauth/menu/templates/menu/menu-user.html:80
 msgid "Sign Out"
 msgstr "탈퇴"
 
 #: allianceauth/menu/templates/menu/menu-user.html:84
+#: allianceauth/templates/allianceauth/top-menu-rh-default.html:17
+#: allianceauth/templates/allianceauth/top-menu-rh-default.html:18
 msgid "Sign In"
 msgstr "가입"
 
 #: allianceauth/notifications/models.py:21
 msgid "danger"
 msgstr "위험"
```

### Comparing `allianceauth-4.0.1/allianceauth/locale/ru/LC_MESSAGES/django.mo` & `allianceauth-4.0.2/allianceauth/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/locale/ru/LC_MESSAGES/django.po` & `allianceauth-4.0.2/allianceauth/locale/ru/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
-#
+# 
 # Translators:
 # Андрей Зубков <and.vareba81@gmail.com>, 2023
 # Yuriy K <thedjcooltv@gmail.com>, 2023
 # Alexander Gess <de.alex.gess@gmail.com>, 2023
 # Filipp Chertiev <f@fzfx.ru>, 2023
 # Ruslan Virchich, 2024
-#
+# Joel Falknau <ozirascal@gmail.com>, 2024
+# 
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-03-13 19:10+1000\n"
+"POT-Creation-Date: 2024-05-12 19:15+1000\n"
 "PO-Revision-Date: 2023-11-08 13:50+0000\n"
-"Last-Translator: Ruslan Virchich, 2024\n"
+"Last-Translator: Joel Falknau <ozirascal@gmail.com>, 2024\n"
 "Language-Team: Russian (https://app.transifex.com/alliance-auth/teams/107430/ru/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: ru\n"
 "Plural-Forms: nplurals=4; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && n%10<=4 && (n%100<12 || n%100>14) ? 1 : n%10==0 || (n%10>=5 && n%10<=9) || (n%100>=11 && n%100<=14)? 2 : 3);\n"
 
@@ -1431,14 +1432,16 @@
 msgstr "Администратор"
 
 #: allianceauth/menu/templates/menu/menu-user.html:80
 msgid "Sign Out"
 msgstr ""
 
 #: allianceauth/menu/templates/menu/menu-user.html:84
+#: allianceauth/templates/allianceauth/top-menu-rh-default.html:17
+#: allianceauth/templates/allianceauth/top-menu-rh-default.html:18
 msgid "Sign In"
 msgstr ""
 
 #: allianceauth/notifications/models.py:21
 msgid "danger"
 msgstr "опасн"
```

### Comparing `allianceauth-4.0.1/allianceauth/locale/uk/LC_MESSAGES/django.mo` & `allianceauth-4.0.2/allianceauth/locale/uk/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/locale/uk/LC_MESSAGES/django.po` & `allianceauth-4.0.2/allianceauth/locale/uk/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Andrii Yukhymchak, 2024
 # 
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-03-13 19:10+1000\n"
+"POT-Creation-Date: 2024-05-12 19:15+1000\n"
 "PO-Revision-Date: 2023-11-08 13:50+0000\n"
 "Last-Translator: Andrii Yukhymchak, 2024\n"
 "Language-Team: Ukrainian (https://app.transifex.com/alliance-auth/teams/107430/uk/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: uk\n"
@@ -1450,14 +1450,16 @@
 msgstr "Адміністратор"
 
 #: allianceauth/menu/templates/menu/menu-user.html:80
 msgid "Sign Out"
 msgstr "Вийти"
 
 #: allianceauth/menu/templates/menu/menu-user.html:84
+#: allianceauth/templates/allianceauth/top-menu-rh-default.html:17
+#: allianceauth/templates/allianceauth/top-menu-rh-default.html:18
 msgid "Sign In"
 msgstr "Увійти"
 
 #: allianceauth/notifications/models.py:21
 msgid "danger"
 msgstr "небезпека"
```

### Comparing `allianceauth-4.0.1/allianceauth/locale/zh_Hans/LC_MESSAGES/django.mo` & `allianceauth-4.0.2/allianceauth/locale/zh_Hans/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/locale/zh_Hans/LC_MESSAGES/django.po` & `allianceauth-4.0.2/allianceauth/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # Joel Falknau <ozirascal@gmail.com>, 2023
 # 
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-03-13 19:10+1000\n"
+"POT-Creation-Date: 2024-05-12 19:15+1000\n"
 "PO-Revision-Date: 2023-11-08 13:50+0000\n"
 "Last-Translator: Joel Falknau <ozirascal@gmail.com>, 2023\n"
 "Language-Team: Chinese Simplified (https://app.transifex.com/alliance-auth/teams/107430/zh-Hans/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: zh-Hans\n"
@@ -1387,14 +1387,16 @@
 msgstr "管理员"
 
 #: allianceauth/menu/templates/menu/menu-user.html:80
 msgid "Sign Out"
 msgstr ""
 
 #: allianceauth/menu/templates/menu/menu-user.html:84
+#: allianceauth/templates/allianceauth/top-menu-rh-default.html:17
+#: allianceauth/templates/allianceauth/top-menu-rh-default.html:18
 msgid "Sign In"
 msgstr ""
 
 #: allianceauth/notifications/models.py:21
 msgid "danger"
 msgstr "危险"
```

### Comparing `allianceauth-4.0.1/allianceauth/menu/admin.py` & `allianceauth-4.0.2/allianceauth/menu/admin.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/menu/core/menu_item_hooks.py` & `allianceauth-4.0.2/allianceauth/menu/core/menu_item_hooks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/menu/core/smart_sync.py` & `allianceauth-4.0.2/allianceauth/menu/core/smart_sync.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/menu/filters.py` & `allianceauth-4.0.2/allianceauth/menu/filters.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/menu/forms.py` & `allianceauth-4.0.2/allianceauth/menu/forms.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/menu/hooks.py` & `allianceauth-4.0.2/allianceauth/menu/hooks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/menu/managers.py` & `allianceauth-4.0.2/allianceauth/menu/managers.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/menu/migrations/0001_initial.py` & `allianceauth-4.0.2/allianceauth/menu/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/menu/models.py` & `allianceauth-4.0.2/allianceauth/menu/models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/menu/templates/menu/menu-item-bs5.html` & `allianceauth-4.0.2/allianceauth/menu/templates/menu/menu-item-bs5.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/menu/templates/menu/menu-notification-block.html` & `allianceauth-4.0.2/allianceauth/menu/templates/menu/menu-notification-block.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/menu/templates/menu/menu-user.html` & `allianceauth-4.0.2/allianceauth/menu/templates/menu/menu-user.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/menu/templates/menu/sortable-side-menu.html` & `allianceauth-4.0.2/allianceauth/menu/templates/menu/sortable-side-menu.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/menu/templatetags/menu_items.py` & `allianceauth-4.0.2/allianceauth/menu/templatetags/menu_items.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/menu/templatetags/menu_menu_items.py` & `allianceauth-4.0.2/allianceauth/menu/templatetags/menu_menu_items.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/menu/tests/core/test_menu_item_hooks.py` & `allianceauth-4.0.2/allianceauth/menu/tests/core/test_menu_item_hooks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/menu/tests/core/test_smart_sync.py` & `allianceauth-4.0.2/allianceauth/menu/tests/core/test_smart_sync.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/menu/tests/factories.py` & `allianceauth-4.0.2/allianceauth/menu/tests/factories.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/menu/tests/integration/test_admin.py` & `allianceauth-4.0.2/allianceauth/menu/tests/integration/test_admin.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/menu/tests/integration/test_dashboard.py` & `allianceauth-4.0.2/allianceauth/menu/tests/integration/test_dashboard.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/menu/tests/templatetags/test_menu_items.py` & `allianceauth-4.0.2/allianceauth/menu/tests/templatetags/test_menu_items.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/menu/tests/templatetags/test_menu_menu_items.py` & `allianceauth-4.0.2/allianceauth/menu/tests/templatetags/test_menu_menu_items.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/menu/tests/test_forms.py` & `allianceauth-4.0.2/allianceauth/menu/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/menu/tests/test_hooks.py` & `allianceauth-4.0.2/allianceauth/menu/tests/test_hooks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/menu/tests/test_managers.py` & `allianceauth-4.0.2/allianceauth/menu/tests/test_managers.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/menu/tests/test_models.py` & `allianceauth-4.0.2/allianceauth/menu/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/menu/tests/utils.py` & `allianceauth-4.0.2/allianceauth/menu/tests/utils.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/notifications/admin.py` & `allianceauth-4.0.2/allianceauth/notifications/admin.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/notifications/core.py` & `allianceauth-4.0.2/allianceauth/notifications/core.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/notifications/handlers.py` & `allianceauth-4.0.2/allianceauth/notifications/handlers.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/notifications/managers.py` & `allianceauth-4.0.2/allianceauth/notifications/managers.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/notifications/migrations/0001_initial.py` & `allianceauth-4.0.2/allianceauth/notifications/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/notifications/migrations/0003_make_strings_more_stringy.py` & `allianceauth-4.0.2/allianceauth/notifications/migrations/0003_make_strings_more_stringy.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/notifications/migrations/0004_performance_tuning.py` & `allianceauth-4.0.2/allianceauth/notifications/migrations/0004_performance_tuning.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/notifications/migrations/0005_fix_level_choices.py` & `allianceauth-4.0.2/allianceauth/notifications/migrations/0005_fix_level_choices.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/notifications/models.py` & `allianceauth-4.0.2/allianceauth/notifications/models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/notifications/templates/notifications/list.html` & `allianceauth-4.0.2/allianceauth/notifications/templates/notifications/list.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/notifications/templates/notifications/list_partial.html` & `allianceauth-4.0.2/allianceauth/notifications/templates/notifications/list_partial.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/notifications/templates/notifications/view.html` & `allianceauth-4.0.2/allianceauth/notifications/templates/notifications/view.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/notifications/templatetags/auth_notifications.py` & `allianceauth-4.0.2/allianceauth/notifications/templatetags/auth_notifications.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/notifications/tests/test_core.py` & `allianceauth-4.0.2/allianceauth/notifications/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/notifications/tests/test_handlers.py` & `allianceauth-4.0.2/allianceauth/notifications/tests/test_handlers.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/notifications/tests/test_init.py` & `allianceauth-4.0.2/allianceauth/notifications/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/notifications/tests/test_managers.py` & `allianceauth-4.0.2/allianceauth/notifications/tests/test_managers.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/notifications/tests/test_models.py` & `allianceauth-4.0.2/allianceauth/notifications/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/notifications/tests/test_templatetags.py` & `allianceauth-4.0.2/allianceauth/notifications/tests/test_templatetags.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/notifications/tests/test_views.py` & `allianceauth-4.0.2/allianceauth/notifications/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/notifications/urls.py` & `allianceauth-4.0.2/allianceauth/notifications/urls.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/notifications/views.py` & `allianceauth-4.0.2/allianceauth/notifications/views.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/optimer/auth_hooks.py` & `allianceauth-4.0.2/allianceauth/optimer/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/optimer/form.py` & `allianceauth-4.0.2/allianceauth/optimer/form.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/optimer/form_widgets.py` & `allianceauth-4.0.2/allianceauth/optimer/form_widgets.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/optimer/migrations/0001_initial.py` & `allianceauth-4.0.2/allianceauth/optimer/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/optimer/migrations/0003_make_strings_more_stringy.py` & `allianceauth-4.0.2/allianceauth/optimer/migrations/0003_make_strings_more_stringy.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/optimer/migrations/0005_add_type_and_description.py` & `allianceauth-4.0.2/allianceauth/optimer/migrations/0005_add_type_and_description.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/optimer/models.py` & `allianceauth-4.0.2/allianceauth/optimer/models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/optimer/templates/optimer/add.html` & `allianceauth-4.0.2/allianceauth/optimer/templates/optimer/add.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/optimer/templates/optimer/dashboard.ops.html` & `allianceauth-4.0.2/allianceauth/optimer/templates/optimer/dashboard.ops.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/optimer/templates/optimer/fleetoptable.html` & `allianceauth-4.0.2/allianceauth/optimer/templates/optimer/fleetoptable.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/optimer/templates/optimer/management.html` & `allianceauth-4.0.2/allianceauth/optimer/templates/optimer/management.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/optimer/templates/optimer/update.html` & `allianceauth-4.0.2/allianceauth/optimer/templates/optimer/update.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/optimer/views.py` & `allianceauth-4.0.2/allianceauth/optimer/views.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/permissions_tool/auth_hooks.py` & `allianceauth-4.0.2/allianceauth/permissions_tool/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/permissions_tool/migrations/0001_initial.py` & `allianceauth-4.0.2/allianceauth/permissions_tool/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/permissions_tool/templates/permissions_tool/audit.html` & `allianceauth-4.0.2/allianceauth/permissions_tool/templates/permissions_tool/audit.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/permissions_tool/templates/permissions_tool/audit_row.html` & `allianceauth-4.0.2/allianceauth/permissions_tool/templates/permissions_tool/audit_row.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/permissions_tool/templates/permissions_tool/overview.html` & `allianceauth-4.0.2/allianceauth/permissions_tool/templates/permissions_tool/overview.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/permissions_tool/tests.py` & `allianceauth-4.0.2/allianceauth/permissions_tool/tests.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/permissions_tool/views.py` & `allianceauth-4.0.2/allianceauth/permissions_tool/views.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/project_template/manage.py` & `allianceauth-4.0.2/allianceauth/project_template/manage.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/project_template/project_name/celery.py` & `allianceauth-4.0.2/allianceauth/project_template/project_name/celery.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/project_template/project_name/settings/base.py` & `allianceauth-4.0.2/allianceauth/project_template/project_name/settings/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,14 +98,15 @@
     ("zh-hans", "Chinese Simplified"),
     ("ru", "Russian"),
     ("ko", "Korean"),
     ("fr", "French"),
     ("ja", "Japanese"),
     ("it", "Italian"),
     ("uk", "Ukrainian"),
+    ("pl", "Polish"),
 )
 
 TEMPLATES = [
     {
         'BACKEND': 'django.template.backends.django.DjangoTemplates',
         'DIRS': [os.path.join(PROJECT_DIR, 'templates')],
         'APP_DIRS': True,
```

### Comparing `allianceauth-4.0.1/allianceauth/project_template/project_name/settings/local.py` & `allianceauth-4.0.2/allianceauth/project_template/project_name/settings/local.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/project_template/supervisor.conf` & `allianceauth-4.0.2/allianceauth/project_template/supervisor.conf`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/abstract.py` & `allianceauth-4.0.2/allianceauth/services/abstract.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/admin.py` & `allianceauth-4.0.2/allianceauth/services/admin.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/auth_hooks.py` & `allianceauth-4.0.2/allianceauth/services/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/forms.py` & `allianceauth-4.0.2/allianceauth/services/forms.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/hooks.py` & `allianceauth-4.0.2/allianceauth/services/hooks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/migrations/0002_nameformatter.py` & `allianceauth-4.0.2/allianceauth/services/migrations/0002_nameformatter.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/migrations/0003_remove_broken_link.py` & `allianceauth-4.0.2/allianceauth/services/migrations/0003_remove_broken_link.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/models.py` & `allianceauth-4.0.2/allianceauth/services/models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/modules/discord/admin.py` & `allianceauth-4.0.2/allianceauth/services/modules/discord/admin.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/modules/discord/api.py` & `allianceauth-4.0.2/allianceauth/services/modules/discord/api.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/modules/discord/app_settings.py` & `allianceauth-4.0.2/allianceauth/services/modules/discord/app_settings.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/modules/discord/auth_hooks.py` & `allianceauth-4.0.2/allianceauth/services/modules/discord/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/modules/discord/core.py` & `allianceauth-4.0.2/allianceauth/services/modules/discord/core.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/modules/discord/discord_client/app_settings.py` & `allianceauth-4.0.2/allianceauth/services/modules/discord/discord_client/app_settings.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/modules/discord/discord_client/client.py` & `allianceauth-4.0.2/allianceauth/services/modules/discord/discord_client/client.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/modules/discord/discord_client/exceptions.py` & `allianceauth-4.0.2/allianceauth/services/modules/discord/discord_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/modules/discord/discord_client/helpers.py` & `allianceauth-4.0.2/allianceauth/services/modules/discord/discord_client/helpers.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/modules/discord/discord_client/models.py` & `allianceauth-4.0.2/allianceauth/services/modules/discord/discord_client/models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/modules/discord/discord_client/tests/example_objects.json` & `allianceauth-4.0.2/allianceauth/services/modules/discord/discord_client/tests/example_objects.json`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/modules/discord/discord_client/tests/factories.py` & `allianceauth-4.0.2/allianceauth/services/modules/discord/discord_client/tests/factories.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/modules/discord/discord_client/tests/piloting_concurrency.py` & `allianceauth-4.0.2/allianceauth/services/modules/discord/discord_client/tests/piloting_concurrency.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/modules/discord/discord_client/tests/piloting_functionality.py` & `allianceauth-4.0.2/allianceauth/services/modules/discord/discord_client/tests/piloting_functionality.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/modules/discord/discord_client/tests/rate_limits.md` & `allianceauth-4.0.2/allianceauth/services/modules/discord/discord_client/tests/rate_limits.md`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/modules/discord/discord_client/tests/test_client.py` & `allianceauth-4.0.2/allianceauth/services/modules/discord/discord_client/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/modules/discord/discord_client/tests/test_exceptions.py` & `allianceauth-4.0.2/allianceauth/services/modules/discord/discord_client/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/modules/discord/discord_client/tests/test_helpers.py` & `allianceauth-4.0.2/allianceauth/services/modules/discord/discord_client/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/modules/discord/discord_client/tests/test_models.py` & `allianceauth-4.0.2/allianceauth/services/modules/discord/discord_client/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/modules/discord/managers.py` & `allianceauth-4.0.2/allianceauth/services/modules/discord/managers.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/modules/discord/migrations/0001_initial.py` & `allianceauth-4.0.2/allianceauth/services/modules/discord/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/modules/discord/migrations/0002_service_permissions.py` & `allianceauth-4.0.2/allianceauth/services/modules/discord/migrations/0002_service_permissions.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/modules/discord/migrations/0003_big_overhaul.py` & `allianceauth-4.0.2/allianceauth/services/modules/discord/migrations/0003_big_overhaul.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/modules/discord/models.py` & `allianceauth-4.0.2/allianceauth/services/modules/discord/models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/modules/discord/tasks.py` & `allianceauth-4.0.2/allianceauth/services/modules/discord/tasks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/modules/discord/templates/services/discord/discord_service_ctrl.html` & `allianceauth-4.0.2/allianceauth/services/modules/discord/templates/services/discord/discord_service_ctrl.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/modules/discord/tests/factories.py` & `allianceauth-4.0.2/allianceauth/services/modules/discord/tests/factories.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/modules/discord/tests/piloting_tasks.py` & `allianceauth-4.0.2/allianceauth/services/modules/discord/tests/piloting_tasks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/modules/discord/tests/test_admin.py` & `allianceauth-4.0.2/allianceauth/services/modules/discord/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/modules/discord/tests/test_api.py` & `allianceauth-4.0.2/allianceauth/services/modules/discord/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/modules/discord/tests/test_auth_hooks.py` & `allianceauth-4.0.2/allianceauth/services/modules/discord/tests/test_auth_hooks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/modules/discord/tests/test_core.py` & `allianceauth-4.0.2/allianceauth/services/modules/discord/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/modules/discord/tests/test_integration.py` & `allianceauth-4.0.2/allianceauth/services/modules/discord/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/modules/discord/tests/test_managers.py` & `allianceauth-4.0.2/allianceauth/services/modules/discord/tests/test_managers.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/modules/discord/tests/test_models.py` & `allianceauth-4.0.2/allianceauth/services/modules/discord/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/modules/discord/tests/test_tasks.py` & `allianceauth-4.0.2/allianceauth/services/modules/discord/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/modules/discord/tests/test_utils.py` & `allianceauth-4.0.2/allianceauth/services/modules/discord/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/modules/discord/tests/test_views.py` & `allianceauth-4.0.2/allianceauth/services/modules/discord/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/modules/discord/urls.py` & `allianceauth-4.0.2/allianceauth/services/modules/discord/urls.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/modules/discord/utils.py` & `allianceauth-4.0.2/allianceauth/services/modules/discord/utils.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/modules/discord/views.py` & `allianceauth-4.0.2/allianceauth/services/modules/discord/views.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/modules/discourse/auth_hooks.py` & `allianceauth-4.0.2/allianceauth/services/modules/discourse/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/modules/discourse/manager.py` & `allianceauth-4.0.2/allianceauth/services/modules/discourse/manager.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/modules/discourse/migrations/0001_initial.py` & `allianceauth-4.0.2/allianceauth/services/modules/discourse/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/modules/discourse/migrations/0002_service_permissions.py` & `allianceauth-4.0.2/allianceauth/services/modules/discourse/migrations/0002_service_permissions.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/modules/discourse/models.py` & `allianceauth-4.0.2/allianceauth/services/modules/discourse/models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/modules/discourse/providers.py` & `allianceauth-4.0.2/allianceauth/services/modules/discourse/providers.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/modules/discourse/tasks.py` & `allianceauth-4.0.2/allianceauth/services/modules/discourse/tasks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/modules/discourse/templates/services/discourse/discourse_service_ctrl.html` & `allianceauth-4.0.2/allianceauth/services/modules/discourse/templates/services/discourse/discourse_service_ctrl.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/modules/discourse/tests.py` & `allianceauth-4.0.2/allianceauth/services/modules/discourse/tests.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/modules/discourse/views.py` & `allianceauth-4.0.2/allianceauth/services/modules/discourse/views.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/modules/example/auth_hooks.py` & `allianceauth-4.0.2/allianceauth/services/modules/example/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/modules/ips4/auth_hooks.py` & `allianceauth-4.0.2/allianceauth/services/modules/ips4/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/modules/ips4/manager.py` & `allianceauth-4.0.2/allianceauth/services/modules/ips4/manager.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/modules/ips4/migrations/0001_initial.py` & `allianceauth-4.0.2/allianceauth/services/modules/ips4/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/modules/ips4/migrations/0002_service_permissions.py` & `allianceauth-4.0.2/allianceauth/services/modules/ips4/migrations/0002_service_permissions.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/modules/ips4/models.py` & `allianceauth-4.0.2/allianceauth/services/modules/ips4/models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/modules/ips4/tasks.py` & `allianceauth-4.0.2/allianceauth/services/modules/ips4/tasks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/modules/ips4/tests.py` & `allianceauth-4.0.2/allianceauth/services/modules/ips4/tests.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/modules/ips4/views.py` & `allianceauth-4.0.2/allianceauth/services/modules/ips4/views.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/modules/mumble/auth_hooks.py` & `allianceauth-4.0.2/allianceauth/services/modules/mumble/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/modules/mumble/migrations/0001_initial.py` & `allianceauth-4.0.2/allianceauth/services/modules/mumble/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/modules/mumble/migrations/0001_squashed_0011_auto_20201011_1009.py` & `allianceauth-4.0.2/allianceauth/services/modules/mumble/migrations/0001_squashed_0011_auto_20201011_1009.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/modules/mumble/migrations/0003_mumbleuser_user.py` & `allianceauth-4.0.2/allianceauth/services/modules/mumble/migrations/0003_mumbleuser_user.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/modules/mumble/migrations/0004_auto_20161214_1024.py` & `allianceauth-4.0.2/allianceauth/services/modules/mumble/migrations/0004_auto_20161214_1024.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/modules/mumble/migrations/0005_mumbleuser_hashfn.py` & `allianceauth-4.0.2/allianceauth/services/modules/mumble/migrations/0005_mumbleuser_hashfn.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/modules/mumble/migrations/0006_service_permissions.py` & `allianceauth-4.0.2/allianceauth/services/modules/mumble/migrations/0006_service_permissions.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/modules/mumble/migrations/0007_not_null_user.py` & `allianceauth-4.0.2/allianceauth/services/modules/mumble/migrations/0007_not_null_user.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/modules/mumble/migrations/0009_set_mumble_dissplay_names.py` & `allianceauth-4.0.2/allianceauth/services/modules/mumble/migrations/0009_set_mumble_dissplay_names.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/modules/mumble/migrations/0010_mumbleuser_certhash.py` & `allianceauth-4.0.2/allianceauth/services/modules/mumble/migrations/0010_mumbleuser_certhash.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/modules/mumble/migrations/0012_mumble_client_info.py` & `allianceauth-4.0.2/allianceauth/services/modules/mumble/migrations/0012_mumble_client_info.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/modules/mumble/models.py` & `allianceauth-4.0.2/allianceauth/services/modules/mumble/models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/modules/mumble/tasks.py` & `allianceauth-4.0.2/allianceauth/services/modules/mumble/tasks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/modules/mumble/templates/services/mumble/mumble_service_ctrl.html` & `allianceauth-4.0.2/allianceauth/services/modules/mumble/templates/services/mumble/mumble_service_ctrl.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/modules/mumble/tests.py` & `allianceauth-4.0.2/allianceauth/services/modules/mumble/tests.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/modules/mumble/urls.py` & `allianceauth-4.0.2/allianceauth/services/modules/mumble/urls.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/modules/mumble/views.py` & `allianceauth-4.0.2/allianceauth/services/modules/mumble/views.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/modules/openfire/auth_hooks.py` & `allianceauth-4.0.2/allianceauth/services/modules/openfire/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/modules/openfire/manager.py` & `allianceauth-4.0.2/allianceauth/services/modules/openfire/manager.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/modules/openfire/migrations/0001_initial.py` & `allianceauth-4.0.2/allianceauth/services/modules/openfire/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/modules/openfire/migrations/0002_service_permissions.py` & `allianceauth-4.0.2/allianceauth/services/modules/openfire/migrations/0002_service_permissions.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/modules/openfire/tasks.py` & `allianceauth-4.0.2/allianceauth/services/modules/openfire/tasks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/modules/openfire/templates/services/openfire/broadcast.html` & `allianceauth-4.0.2/allianceauth/services/modules/openfire/templates/services/openfire/broadcast.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/modules/openfire/tests.py` & `allianceauth-4.0.2/allianceauth/services/modules/openfire/tests.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/modules/openfire/urls.py` & `allianceauth-4.0.2/allianceauth/services/modules/openfire/urls.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/modules/openfire/views.py` & `allianceauth-4.0.2/allianceauth/services/modules/openfire/views.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/modules/phpbb3/auth_hooks.py` & `allianceauth-4.0.2/allianceauth/services/modules/phpbb3/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/modules/phpbb3/manager.py` & `allianceauth-4.0.2/allianceauth/services/modules/phpbb3/manager.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/modules/phpbb3/migrations/0001_initial.py` & `allianceauth-4.0.2/allianceauth/services/modules/phpbb3/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/modules/phpbb3/migrations/0002_service_permissions.py` & `allianceauth-4.0.2/allianceauth/services/modules/phpbb3/migrations/0002_service_permissions.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/modules/phpbb3/tasks.py` & `allianceauth-4.0.2/allianceauth/services/modules/phpbb3/tasks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/modules/phpbb3/tests.py` & `allianceauth-4.0.2/allianceauth/services/modules/phpbb3/tests.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/modules/phpbb3/views.py` & `allianceauth-4.0.2/allianceauth/services/modules/phpbb3/views.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/modules/smf/auth_hooks.py` & `allianceauth-4.0.2/allianceauth/services/modules/smf/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/modules/smf/manager.py` & `allianceauth-4.0.2/allianceauth/services/modules/smf/manager.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/modules/smf/migrations/0001_initial.py` & `allianceauth-4.0.2/allianceauth/services/modules/smf/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/modules/smf/migrations/0002_service_permissions.py` & `allianceauth-4.0.2/allianceauth/services/modules/smf/migrations/0002_service_permissions.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/modules/smf/migrations/0003_set_smf_displayed_names.py` & `allianceauth-4.0.2/allianceauth/services/modules/smf/migrations/0003_set_smf_displayed_names.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/modules/smf/tasks.py` & `allianceauth-4.0.2/allianceauth/services/modules/smf/tasks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/modules/smf/tests.py` & `allianceauth-4.0.2/allianceauth/services/modules/smf/tests.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/modules/smf/views.py` & `allianceauth-4.0.2/allianceauth/services/modules/smf/views.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/modules/teamspeak3/admin.py` & `allianceauth-4.0.2/allianceauth/services/modules/teamspeak3/admin.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/modules/teamspeak3/auth_hooks.py` & `allianceauth-4.0.2/allianceauth/services/modules/teamspeak3/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/modules/teamspeak3/manager.py` & `allianceauth-4.0.2/allianceauth/services/modules/teamspeak3/manager.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/modules/teamspeak3/migrations/0001_initial.py` & `allianceauth-4.0.2/allianceauth/services/modules/teamspeak3/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/modules/teamspeak3/migrations/0002_auto_20161212_0133.py` & `allianceauth-4.0.2/allianceauth/services/modules/teamspeak3/migrations/0002_auto_20161212_0133.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/modules/teamspeak3/migrations/0003_teamspeak3user.py` & `allianceauth-4.0.2/allianceauth/services/modules/teamspeak3/migrations/0003_teamspeak3user.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/modules/teamspeak3/migrations/0004_service_permissions.py` & `allianceauth-4.0.2/allianceauth/services/modules/teamspeak3/migrations/0004_service_permissions.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/modules/teamspeak3/migrations/0005_stategroup.py` & `allianceauth-4.0.2/allianceauth/services/modules/teamspeak3/migrations/0005_stategroup.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/modules/teamspeak3/models.py` & `allianceauth-4.0.2/allianceauth/services/modules/teamspeak3/models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/modules/teamspeak3/signals.py` & `allianceauth-4.0.2/allianceauth/services/modules/teamspeak3/signals.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/modules/teamspeak3/tasks.py` & `allianceauth-4.0.2/allianceauth/services/modules/teamspeak3/tasks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/modules/teamspeak3/templates/services/teamspeak3/teamspeak3_service_ctrl.html` & `allianceauth-4.0.2/allianceauth/services/modules/teamspeak3/templates/services/teamspeak3/teamspeak3_service_ctrl.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/modules/teamspeak3/templates/services/teamspeak3/teamspeakjoin.html` & `allianceauth-4.0.2/allianceauth/services/modules/teamspeak3/templates/services/teamspeak3/teamspeakjoin.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/modules/teamspeak3/tests.py` & `allianceauth-4.0.2/allianceauth/services/modules/teamspeak3/tests.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/modules/teamspeak3/urls.py` & `allianceauth-4.0.2/allianceauth/services/modules/teamspeak3/urls.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/modules/teamspeak3/util/ts3.py` & `allianceauth-4.0.2/allianceauth/services/modules/teamspeak3/util/ts3.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/modules/teamspeak3/views.py` & `allianceauth-4.0.2/allianceauth/services/modules/teamspeak3/views.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/modules/xenforo/auth_hooks.py` & `allianceauth-4.0.2/allianceauth/services/modules/xenforo/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/modules/xenforo/manager.py` & `allianceauth-4.0.2/allianceauth/services/modules/xenforo/manager.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/modules/xenforo/migrations/0001_initial.py` & `allianceauth-4.0.2/allianceauth/services/modules/xenforo/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/modules/xenforo/migrations/0002_service_permissions.py` & `allianceauth-4.0.2/allianceauth/services/modules/xenforo/migrations/0002_service_permissions.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/modules/xenforo/tasks.py` & `allianceauth-4.0.2/allianceauth/services/modules/xenforo/tasks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/modules/xenforo/tests.py` & `allianceauth-4.0.2/allianceauth/services/modules/xenforo/tests.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/modules/xenforo/urls.py` & `allianceauth-4.0.2/allianceauth/services/modules/xenforo/urls.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/modules/xenforo/views.py` & `allianceauth-4.0.2/allianceauth/services/modules/xenforo/views.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/signals.py` & `allianceauth-4.0.2/allianceauth/services/signals.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/tasks.py` & `allianceauth-4.0.2/allianceauth/services/tasks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/templates/services/fleetformattertool.html` & `allianceauth-4.0.2/allianceauth/services/templates/services/fleetformattertool.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/templates/services/service_confirm_delete.html` & `allianceauth-4.0.2/allianceauth/services/templates/services/service_confirm_delete.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/templates/services/service_credentials.html` & `allianceauth-4.0.2/allianceauth/services/templates/services/service_credentials.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/templates/services/service_password.html` & `allianceauth-4.0.2/allianceauth/services/templates/services/service_password.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/templates/services/services.html` & `allianceauth-4.0.2/allianceauth/services/templates/services/services.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/templates/services/services_ctrl.html` & `allianceauth-4.0.2/allianceauth/services/templates/services/services_ctrl.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/templates/services/services_ctrl_base.html` & `allianceauth-4.0.2/allianceauth/services/templates/services/services_ctrl_base.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/tests/test_hooks.py` & `allianceauth-4.0.2/allianceauth/services/tests/test_hooks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/tests/test_models.py` & `allianceauth-4.0.2/allianceauth/services/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/tests/test_nameformatter.py` & `allianceauth-4.0.2/allianceauth/services/tests/test_nameformatter.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/tests/test_signals.py` & `allianceauth-4.0.2/allianceauth/services/tests/test_signals.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/tests/test_tasks.py` & `allianceauth-4.0.2/allianceauth/services/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/urls.py` & `allianceauth-4.0.2/allianceauth/services/urls.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/services/views.py` & `allianceauth-4.0.2/allianceauth/services/views.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/srp/auth_hooks.py` & `allianceauth-4.0.2/allianceauth/srp/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/srp/form.py` & `allianceauth-4.0.2/allianceauth/srp/form.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/srp/managers.py` & `allianceauth-4.0.2/allianceauth/srp/managers.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/srp/migrations/0001_initial.py` & `allianceauth-4.0.2/allianceauth/srp/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/srp/migrations/0003_make_strings_more_stringy.py` & `allianceauth-4.0.2/allianceauth/srp/migrations/0003_make_strings_more_stringy.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/srp/migrations/0004_on_delete.py` & `allianceauth-4.0.2/allianceauth/srp/migrations/0004_on_delete.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/srp/models.py` & `allianceauth-4.0.2/allianceauth/srp/models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/srp/swagger.json` & `allianceauth-4.0.2/allianceauth/srp/swagger.json`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/srp/templates/srp/add.html` & `allianceauth-4.0.2/allianceauth/srp/templates/srp/add.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/srp/templates/srp/data.html` & `allianceauth-4.0.2/allianceauth/srp/templates/srp/data.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/srp/templates/srp/management.html` & `allianceauth-4.0.2/allianceauth/srp/templates/srp/management.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/srp/templates/srp/request.html` & `allianceauth-4.0.2/allianceauth/srp/templates/srp/request.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/srp/templates/srp/update.html` & `allianceauth-4.0.2/allianceauth/srp/templates/srp/update.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/srp/tests/test_managers.py` & `allianceauth-4.0.2/allianceauth/srp/tests/test_managers.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/srp/tests/testdata/get_killmails_killmail_id_killmail_hash_81973979.json` & `allianceauth-4.0.2/allianceauth/srp/tests/testdata/get_killmails_killmail_id_killmail_hash_81973979.json`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/srp/urls.py` & `allianceauth-4.0.2/allianceauth/srp/urls.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/srp/views.py` & `allianceauth-4.0.2/allianceauth/srp/views.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/static/allianceauth/css/auth-base.css` & `allianceauth-4.0.2/allianceauth/static/allianceauth/css/auth-base.css`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/static/allianceauth/css/checkbox.css` & `allianceauth-4.0.2/allianceauth/static/allianceauth/css/checkbox.css`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/static/allianceauth/css/themes/bootstrap-locals.less` & `allianceauth-4.0.2/allianceauth/static/allianceauth/css/themes/bootstrap-locals.less`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/static/allianceauth/css/themes/darkly/LICENSE` & `allianceauth-4.0.2/allianceauth/static/allianceauth/css/themes/darkly/LICENSE`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/static/allianceauth/css/themes/darkly/darkly.less` & `allianceauth-4.0.2/allianceauth/static/allianceauth/css/themes/darkly/darkly.less`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/static/allianceauth/css/themes/darkly/darkly.min.css` & `allianceauth-4.0.2/allianceauth/static/allianceauth/css/themes/darkly/darkly.min.css`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/static/allianceauth/css/themes/flatly-shared.less` & `allianceauth-4.0.2/allianceauth/static/allianceauth/css/themes/flatly-shared.less`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/static/allianceauth/css/themes/flatly/LICENSE` & `allianceauth-4.0.2/allianceauth/static/allianceauth/css/themes/flatly/LICENSE`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/static/allianceauth/css/themes/flatly/flatly.less` & `allianceauth-4.0.2/allianceauth/static/allianceauth/css/themes/flatly/flatly.less`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/static/allianceauth/css/themes/flatly/flatly.min.css` & `allianceauth-4.0.2/allianceauth/static/allianceauth/css/themes/flatly/flatly.min.css`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/static/allianceauth/icons/allianceauth.png` & `allianceauth-4.0.2/allianceauth/static/allianceauth/icons/allianceauth.png`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/static/allianceauth/icons/android-chrome-192x192.png` & `allianceauth-4.0.2/allianceauth/static/allianceauth/icons/android-chrome-192x192.png`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/static/allianceauth/icons/android-chrome-512x512.png` & `allianceauth-4.0.2/allianceauth/static/allianceauth/icons/android-chrome-512x512.png`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/static/allianceauth/icons/apple-touch-icon.png` & `allianceauth-4.0.2/allianceauth/static/allianceauth/icons/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/static/allianceauth/icons/favicon-16x16.png` & `allianceauth-4.0.2/allianceauth/static/allianceauth/icons/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/static/allianceauth/icons/favicon-32x32.png` & `allianceauth-4.0.2/allianceauth/static/allianceauth/icons/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/static/allianceauth/icons/favicon-96x96.png` & `allianceauth-4.0.2/allianceauth/static/allianceauth/icons/favicon-96x96.png`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/static/allianceauth/icons/favicon.ico` & `allianceauth-4.0.2/allianceauth/static/allianceauth/icons/favicon.ico`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/static/allianceauth/icons/mstile-150x150.png` & `allianceauth-4.0.2/allianceauth/static/allianceauth/icons/mstile-150x150.png`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/static/allianceauth/icons/safari-pinned-tab.svg` & `allianceauth-4.0.2/allianceauth/static/allianceauth/icons/safari-pinned-tab.svg`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/static/allianceauth/images/auth-logo.png` & `allianceauth-4.0.2/allianceauth/static/allianceauth/images/auth-logo.png`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/static/allianceauth/images/auth-logo.svg` & `allianceauth-4.0.2/allianceauth/static/allianceauth/images/auth-logo.svg`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/static/allianceauth/js/eve-time.js` & `allianceauth-4.0.2/allianceauth/static/allianceauth/js/eve-time.js`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/static/allianceauth/js/filterDropDown/LICENSE` & `allianceauth-4.0.2/allianceauth/static/allianceauth/js/filterDropDown/LICENSE`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/static/allianceauth/js/filterDropDown/filterDropDown.js` & `allianceauth-4.0.2/allianceauth/static/allianceauth/js/filterDropDown/filterDropDown.js`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/static/allianceauth/js/filterDropDown/filterDropDown.min.js` & `allianceauth-4.0.2/allianceauth/static/allianceauth/js/filterDropDown/filterDropDown.min.js`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/static/allianceauth/js/jquery-ui/1.12.1/css/images/ui-icons_444444_256x240.png` & `allianceauth-4.0.2/allianceauth/static/allianceauth/js/jquery-ui/1.12.1/css/images/ui-icons_444444_256x240.png`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/static/allianceauth/js/jquery-ui/1.12.1/css/images/ui-icons_555555_256x240.png` & `allianceauth-4.0.2/allianceauth/static/allianceauth/js/jquery-ui/1.12.1/css/images/ui-icons_555555_256x240.png`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/static/allianceauth/js/jquery-ui/1.12.1/css/images/ui-icons_777620_256x240.png` & `allianceauth-4.0.2/allianceauth/static/allianceauth/js/jquery-ui/1.12.1/css/images/ui-icons_777620_256x240.png`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/static/allianceauth/js/jquery-ui/1.12.1/css/images/ui-icons_777777_256x240.png` & `allianceauth-4.0.2/allianceauth/static/allianceauth/js/jquery-ui/1.12.1/css/images/ui-icons_777777_256x240.png`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/static/allianceauth/js/jquery-ui/1.12.1/css/images/ui-icons_cc0000_256x240.png` & `allianceauth-4.0.2/allianceauth/static/allianceauth/js/jquery-ui/1.12.1/css/images/ui-icons_cc0000_256x240.png`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/static/allianceauth/js/jquery-ui/1.12.1/css/images/ui-icons_ffffff_256x240.png` & `allianceauth-4.0.2/allianceauth/static/allianceauth/js/jquery-ui/1.12.1/css/images/ui-icons_ffffff_256x240.png`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/static/allianceauth/js/jquery-ui/1.12.1/css/jquery-ui.min.css` & `allianceauth-4.0.2/allianceauth/static/allianceauth/js/jquery-ui/1.12.1/css/jquery-ui.min.css`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/static/allianceauth/js/jquery-ui/1.13.2/css/images/ui-icons_444444_256x240.png` & `allianceauth-4.0.2/allianceauth/static/allianceauth/js/jquery-ui/1.13.2/css/images/ui-icons_444444_256x240.png`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/static/allianceauth/js/jquery-ui/1.13.2/css/images/ui-icons_555555_256x240.png` & `allianceauth-4.0.2/allianceauth/static/allianceauth/js/jquery-ui/1.13.2/css/images/ui-icons_555555_256x240.png`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/static/allianceauth/js/jquery-ui/1.13.2/css/images/ui-icons_777620_256x240.png` & `allianceauth-4.0.2/allianceauth/static/allianceauth/js/jquery-ui/1.13.2/css/images/ui-icons_777620_256x240.png`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/static/allianceauth/js/jquery-ui/1.13.2/css/images/ui-icons_777777_256x240.png` & `allianceauth-4.0.2/allianceauth/static/allianceauth/js/jquery-ui/1.13.2/css/images/ui-icons_777777_256x240.png`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/static/allianceauth/js/jquery-ui/1.13.2/css/images/ui-icons_cc0000_256x240.png` & `allianceauth-4.0.2/allianceauth/static/allianceauth/js/jquery-ui/1.13.2/css/images/ui-icons_cc0000_256x240.png`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/static/allianceauth/js/jquery-ui/1.13.2/css/images/ui-icons_ffffff_256x240.png` & `allianceauth-4.0.2/allianceauth/static/allianceauth/js/jquery-ui/1.13.2/css/images/ui-icons_ffffff_256x240.png`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/static/allianceauth/js/jquery-ui/1.13.2/css/jquery-ui.min.css` & `allianceauth-4.0.2/allianceauth/static/allianceauth/js/jquery-ui/1.13.2/css/jquery-ui.min.css`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/static/allianceauth/js/refresh-notification-icon.js` & `allianceauth-4.0.2/allianceauth/static/allianceauth/js/refresh-notification-icon.js`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/static/allianceauth/js/refresh_notifications.js` & `allianceauth-4.0.2/allianceauth/static/allianceauth/js/refresh_notifications.js`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/static/allianceauth/js/timerboard.js` & `allianceauth-4.0.2/allianceauth/static/allianceauth/js/timerboard.js`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/static/allianceauth/js/timers.js` & `allianceauth-4.0.2/allianceauth/static/allianceauth/js/timers.js`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/templates/allianceauth/admin-status/esi_check.html` & `allianceauth-4.0.2/allianceauth/templates/allianceauth/admin-status/esi_check.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/templates/allianceauth/admin-status/overview.html` & `allianceauth-4.0.2/allianceauth/templates/allianceauth/admin-status/overview.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/templates/allianceauth/base-bs5.html` & `allianceauth-4.0.2/allianceauth/templates/allianceauth/base-bs5.html`

 * *Files 5% similar despite different names*

```diff
@@ -25,64 +25,61 @@
         {% include 'bundles/auth-framework-css.html' %}
 
         <style>
             .navbar-toggler.collapsed{
                 transform: rotate(180deg);
             }
 
-            {% if user.is_authenticated %}
-                .nav-padding {
-                    padding-top: {% header_padding_size %} !important;
-                }
-            {% endif %}
+            .nav-padding {
+                padding-top: {% header_padding_size %} !important;
+            }
         </style>
+
         {% block extra_css %}{% endblock extra_css %}
     </head>
 
     <body>
-        {% if user.is_authenticated %}
-            <!-- Top Menu, Blocks don't work in "include" tagged views -->
-            <nav class="navbar navbar-expand-lg navbar-dark fixed-top bg-primary">
-                <div class="container-fluid justify-content-start">
-                    {% if user.is_authenticated %}
-                        <a class="navbar-brand" data-bs-toggle="collapse" data-bs-target="#sidebar" role="button">
-                            <i class="fa-solid fa-bars ms-2 me-2"></i>
-                        </a>
-                    {% endif %}
-
-                    <div class="navbar-brand">
-                        {% block header_nav_brand %}{{ SITE_NAME }}{% endblock %}
-                    </div>
-
-                    <div class="collapse navbar-collapse ms-2 px-2" id="navbarexpand">
-                        <ul id="nav-left" class="nav navbar-nav me-auto">
-                            {% block header_nav_collapse_left %}
-                            {% endblock %}
-                        </ul>
-
-                        <ul id="nav-right" class="nav navbar-nav">
-                            {% block header_nav_collapse_right %}
-                            {% endblock %}
-                        </ul>
-
-                        <ul id="nav-right-character-control" class="nav navbar-nav">
-                            {% block header_nav_user_character_control %} <!-- Default to add char and swap main -->
-                                {% include 'allianceauth/top-menu-rh-default.html' %}
-                            {% endblock %}
+        <!-- Top Menu, Blocks don't work in "include" tagged views -->
+        <nav class="navbar navbar-expand-lg navbar-dark fixed-top bg-primary">
+            <div class="container-fluid justify-content-start">
+                <a class="navbar-brand" data-bs-toggle="collapse" data-bs-target="#sidebar" role="button">
+                    <i class="fa-solid fa-bars ms-2 me-2"></i>
+                </a>
 
-                            {% include 'menu/menu-notification-block.html' %}
-                        </ul>
-                    </div>
+                <div class="navbar-brand">
+                    {% block header_nav_brand %}{{ SITE_NAME }}{% endblock %}
+                </div>
 
-                    <a class="navbar-toggler navbar-brand border-0 collapsed" data-bs-toggle="collapse" data-bs-target="#navbarexpand" aria-controls="navbarColor01" aria-expanded="false" aria-label="Toggle navigation" style="margin-left: auto;">
-                        <i class="fa-solid fa-chevron-up"></i>
-                    </a>
+                <div class="collapse navbar-collapse ms-2 px-2" id="navbarexpand">
+                    <ul id="nav-left" class="nav navbar-nav me-auto">
+                        {% block header_nav_collapse_left %}
+                        {% endblock %}
+                    </ul>
+
+                    <ul id="nav-right" class="nav navbar-nav">
+                        {% block header_nav_collapse_right %}
+                        {% endblock %}
+                    </ul>
+
+                    <ul id="nav-right-character-control" class="nav navbar-nav">
+                        {% block header_nav_user_character_control %} <!-- Default to add char and swap main -->
+                            {% include 'allianceauth/top-menu-rh-default.html' %}
+                        {% endblock %}
+
+                        {% if user.is_authenticated %}
+                            {% include 'menu/menu-notification-block.html' %}
+                        {% endif %}
+                    </ul>
                 </div>
-            </nav>
-        {% endif %}
+
+                <a class="navbar-toggler navbar-brand border-0 collapsed" data-bs-toggle="collapse" data-bs-target="#navbarexpand" aria-controls="navbarColor01" aria-expanded="false" aria-label="Toggle navigation" style="margin-left: auto;">
+                    <i class="fa-solid fa-chevron-up"></i>
+                </a>
+            </div>
+        </nav>
         <!-- End Top Menu -->
 
         <!-- Body -->
         <main class="row flex-nowrap m-0">
             {% include 'menu/sortable-side-menu.html' %}
 
             <div class="nav-padding col flex-nowrap vh-100 overflow-auto">
```

#### html2text {}

```diff
@@ -1,22 +1,20 @@
 {% load static %} {% load i18n %} {% load navactive %} {% load
 auth_notifications %} {% load theme_tags %}
 % theme_html_tags %}>
 {% include 'allianceauth/icons.html' %}
 {% theme_css %} {% include 'bundles/fontawesome.html' %} {% include 'bundles/
 auth-framework-css.html' %}
 {% block extra_css %}{% endblock extra_css %}
-{% if user.is_authenticated %}
-{% if user.is_authenticated %} {% endif %}
 {% block header_nav_brand %}{{ SITE_NAME }}{% endblock %}
     * {% block header_nav_collapse_left %} {% endblock %}
     * {% block header_nav_collapse_right %} {% endblock %}
     * {% block header_nav_user_character_control %} {% include 'allianceauth/
-      top-menu-rh-default.html' %} {% endblock %} {% include 'menu/menu-
-      notification-block.html' %}
-{% endif %} {% include 'menu/sortable-side-menu.html' %}
+      top-menu-rh-default.html' %} {% endblock %} {% if user.is_authenticated
+      %} {% include 'menu/menu-notification-block.html' %} {% endif %}
+{% include 'menu/sortable-side-menu.html' %}
 {% include 'allianceauth/messages-bs5.html' %} {% block content %} {% endblock
 content %}
 {% include 'bundles/jquery-js.html' %} {% theme_js %} {% if
 user.is_authenticated %}
 {% include 'bundles/refresh-notification-icon-js.html' %} {% endif %} {% block
 extra_javascript %} {% endblock extra_javascript %}
```

### Comparing `allianceauth-4.0.1/allianceauth/templates/allianceauth/base.html` & `allianceauth-4.0.2/allianceauth/templates/allianceauth/base.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/templates/allianceauth/error.html` & `allianceauth-4.0.2/allianceauth/templates/allianceauth/error.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/templates/allianceauth/icons.html` & `allianceauth-4.0.2/allianceauth/templates/allianceauth/icons.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/templates/allianceauth/messages-bs5.html` & `allianceauth-4.0.2/allianceauth/templates/allianceauth/messages-bs5.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/templates/allianceauth/messages.html` & `allianceauth-4.0.2/allianceauth/templates/allianceauth/messages.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/templates/allianceauth/side-menu.html` & `allianceauth-4.0.2/allianceauth/templates/allianceauth/side-menu.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/templates/allianceauth/top-menu-admin.html` & `allianceauth-4.0.2/allianceauth/templates/allianceauth/top-menu-admin.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/templates/allianceauth/top-menu-rh-default.html` & `allianceauth-4.0.2/allianceauth/templates/allianceauth/top-menu-rh-default.html`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 {% load i18n %}
-
+{% if user.is_authenticated %}
 <li class="nav-item">
     <a href="{% url 'authentication:add_character' %}" class="nav-link" title="{% translate 'Add Character' %}">
         <i class="fa-solid fa-plus"></i>
         <span class="d-lg-none d-md-inline m-2">{% translate "Add Character" %}</span>
     </a>
 </li>
 <li class="nav-item">
     <a href="{% url 'authentication:change_main_character' %}" class="nav-link" title="{% translate 'Change Main' %}">
         <i class="fa-solid fa-shuffle"></i>
         <span class="d-lg-none d-md-inline m-2">{% translate "Change Main" %}</span>
     </a>
 </li>
+{% else %}
+<li class="nav-item">
+    <a href="{% url 'authentication:login' %}" class="nav-link" title="{% translate 'Sign In' %}">
+        <i class="fa-solid fa-right-to-bracket fa-fw "></i> {% translate "Sign In" %}
+    </a>
+</li>
+{% endif %}
```

#### html2text {}

```diff
@@ -1,3 +1,6 @@
-{% load i18n %}
+{% load i18n %} {% if user.is_authenticated %}
 _{_%_ _t_r_a_n_s_l_a_t_e_ _"_A_d_d_ _C_h_a_r_a_c_t_e_r_"_ _%_}
 _{_%_ _t_r_a_n_s_l_a_t_e_ _"_C_h_a_n_g_e_ _M_a_i_n_"_ _%_}
+{% else %}
+_{_%_ _t_r_a_n_s_l_a_t_e_ _"_S_i_g_n_ _I_n_"_ _%_}
+{% endif %}
```

### Comparing `allianceauth-4.0.1/allianceauth/templates/allianceauth/top-menu-user-dropdown.html` & `allianceauth-4.0.2/allianceauth/templates/allianceauth/top-menu-user-dropdown.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/templates/allianceauth/top-menu.html` & `allianceauth-4.0.2/allianceauth/templates/allianceauth/top-menu.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/templates/bundles/bootstrap-css.html` & `allianceauth-4.0.2/allianceauth/templates/bundles/bootstrap-css.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/templates/bundles/bootstrap-js.html` & `allianceauth-4.0.2/allianceauth/templates/bundles/bootstrap-js.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/templates/bundles/datatables-js-bs5.html` & `allianceauth-4.0.2/allianceauth/templates/bundles/datatables-js-bs5.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/templates/bundles/datatables-js.html` & `allianceauth-4.0.2/allianceauth/templates/bundles/datatables-js.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/templates/bundles/moment-js.html` & `allianceauth-4.0.2/allianceauth/templates/bundles/moment-js.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/templatetags/admin_status.py` & `allianceauth-4.0.2/allianceauth/templatetags/admin_status.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/tests/auth_utils.py` & `allianceauth-4.0.2/allianceauth/tests/auth_utils.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/tests/test_auth_utils.py` & `allianceauth-4.0.2/allianceauth/tests/test_auth_utils.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/tests/test_urls.py` & `allianceauth-4.0.2/allianceauth/tests/test_urls.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/tests/test_views.py` & `allianceauth-4.0.2/allianceauth/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/theme/bootstrap/auth_hooks.py` & `allianceauth-4.0.2/allianceauth/theme/bootstrap/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/theme/darkly/auth_hooks.py` & `allianceauth-4.0.2/allianceauth/theme/darkly/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/theme/flatly/auth_hooks.py` & `allianceauth-4.0.2/allianceauth/theme/flatly/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/theme/hooks.py` & `allianceauth-4.0.2/allianceauth/theme/hooks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/theme/materia/auth_hooks.py` & `allianceauth-4.0.2/allianceauth/theme/materia/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/theme/templatetags/theme_tags.py` & `allianceauth-4.0.2/allianceauth/theme/templatetags/theme_tags.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/thirdparty/navhelper/templatetags/navactive.py` & `allianceauth-4.0.2/allianceauth/thirdparty/navhelper/templatetags/navactive.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/thirdparty/navhelper/tests.py` & `allianceauth-4.0.2/allianceauth/thirdparty/navhelper/tests.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/timerboard/auth_hooks.py` & `allianceauth-4.0.2/allianceauth/timerboard/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/timerboard/form.py` & `allianceauth-4.0.2/allianceauth/timerboard/form.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/timerboard/migrations/0001_initial.py` & `allianceauth-4.0.2/allianceauth/timerboard/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/timerboard/migrations/0002_make_strings_more_stringy.py` & `allianceauth-4.0.2/allianceauth/timerboard/migrations/0002_make_strings_more_stringy.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/timerboard/migrations/0003_on_delete.py` & `allianceauth-4.0.2/allianceauth/timerboard/migrations/0003_on_delete.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/timerboard/migrations/0004_timer_type.py` & `allianceauth-4.0.2/allianceauth/timerboard/migrations/0004_timer_type.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/timerboard/models.py` & `allianceauth-4.0.2/allianceauth/timerboard/models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/timerboard/templates/timerboard/dashboard.timers.html` & `allianceauth-4.0.2/allianceauth/timerboard/templates/timerboard/dashboard.timers.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/timerboard/templates/timerboard/form.html` & `allianceauth-4.0.2/allianceauth/timerboard/templates/timerboard/form.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/timerboard/templates/timerboard/timer_confirm_delete.html` & `allianceauth-4.0.2/allianceauth/timerboard/templates/timerboard/timer_confirm_delete.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/timerboard/templates/timerboard/timer_create_form.html` & `allianceauth-4.0.2/allianceauth/timerboard/templates/timerboard/timer_create_form.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/timerboard/templates/timerboard/timer_update_form.html` & `allianceauth-4.0.2/allianceauth/timerboard/templates/timerboard/timer_update_form.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/timerboard/templates/timerboard/timertable.html` & `allianceauth-4.0.2/allianceauth/timerboard/templates/timerboard/timertable.html`

 * *Files 3% similar despite different names*

```diff
@@ -15,17 +15,17 @@
             {% if perms.auth.timer_management %}
                 <th class="text-center">{% translate "Action" %}</th>
             {% endif %}
         </tr>
 
         {% for timer in timers %}
             {% if timer.important == True %}
-                <tr class="table-danger">
+                <tr class="bg-danger bg-opacity-25">
             {% else %}
-                <tr class="table-info">
+                <tr class="bg-info bg-opacity-25">
             {% endif %}
 
                 <td style="width: 150px;" class="text-center">
                     {{ timer.details }}
 
                     {% if timer.timer_type != 'UNSPECIFIED' %}
                         <br>({{ timer.get_timer_type_display }})
```

### Comparing `allianceauth-4.0.1/allianceauth/timerboard/templates/timerboard/view.html` & `allianceauth-4.0.2/allianceauth/timerboard/templates/timerboard/view.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/timerboard/tests.py` & `allianceauth-4.0.2/allianceauth/timerboard/tests.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/timerboard/views.py` & `allianceauth-4.0.2/allianceauth/timerboard/views.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/urls.py` & `allianceauth-4.0.2/allianceauth/urls.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/utils/cache.py` & `allianceauth-4.0.2/allianceauth/utils/cache.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/utils/counters.py` & `allianceauth-4.0.2/allianceauth/utils/counters.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/utils/django.py` & `allianceauth-4.0.2/allianceauth/utils/django.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/utils/testing.py` & `allianceauth-4.0.2/allianceauth/utils/testing.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/utils/tests/test_cache.py` & `allianceauth-4.0.2/allianceauth/utils/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/utils/tests/test_counters.py` & `allianceauth-4.0.2/allianceauth/utils/tests/test_counters.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/utils/tests/test_django.py` & `allianceauth-4.0.2/allianceauth/utils/tests/test_django.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/allianceauth/views.py` & `allianceauth-4.0.2/allianceauth/views.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.1/pyproject.toml` & `allianceauth-4.0.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,101 +1,105 @@
 [build-system]
-requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
+requires = [
+    "flit-core<4,>=3.2",
+]
 
 [project]
 name = "allianceauth"
-dynamic = ["version", "description"]
 readme = "README.md"
-license = {file = "LICENSE"}
-requires-python = ">=3.8"
-authors = [
-    { name = "Alliance Auth", email = "adarnof@gmail.com" },
-]
 keywords = [
     "allianceauth",
     "eveonline",
 ]
+license = { file = "LICENSE" }
+authors = [
+    { name = "Alliance Auth", email = "adarnof@gmail.com" },
+]
+requires-python = ">=3.8"
 classifiers = [
     "Environment :: Web Environment",
     "Framework :: Django",
     "Framework :: Django :: 4.2",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: GNU General Public License v2 (GPLv2)",
     "Operating System :: POSIX :: Linux",
     "Programming Language :: Python",
+    "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Topic :: Internet :: WWW/HTTP",
     "Topic :: Internet :: WWW/HTTP :: Dynamic Content",
 ]
+dynamic = [
+    "description",
+    "version",
+]
 dependencies = [
     "bcrypt",
     "beautifulsoup4",
+    "celery<6,>=5.2",
     "celery-once>=3.0.1",
-    "celery>=5.2.0,<6",
-    'django-bootstrap5>=23.3',
+    "django<5,>=4.2",
     "django-bootstrap-form",
-    "django-celery-beat>=2.3.0",
-    "django-esi>=5.0.0",
-    "django-redis>=5.2.0",
-    "django-registration>=3.3,<3.4",
+    "django-bootstrap5>=23.3",
+    "django-celery-beat>=2.3",
+    "django-esi>=5",
+    "django-redis>=5.2",
+    "django-registration<3.4,>=3.3",
     "django-sortedm2m",
-    "django>=4.2,<5",
     "dnspython",
-    "mysqlclient>=2.1.0",
+    "mysqlclient>=2.1",
     "openfire-restapi",
-    "packaging>=21.0",
+    "packaging>=21",
     "passlib",
     "pydiscourse",
     "python-slugify>=1.2",
-    "redis>=4.0.0",
-    "requests-oauthlib",
+    "redis>=4",
     "requests>=2.9.1",
+    "requests-oauthlib",
     "semantic-version",
     "slixmpp",
 ]
-
-[project.optional-dependencies]
-test = [
-    "coverage>=4.3.1",
-    "django-webtest",
-    "requests-mock>=1.2.0"
-]
-docs = [
-    "sphinx",
-    "sphinx_rtd_theme>=2.0.0,<3.0.0",
+optional-dependencies.docs = [
     "myst-parser",
-    "sphinxcontrib-django",
+    "sphinx",
     "sphinx-copybutton",
+    "sphinx-rtd-theme<3,>=2",
     "sphinx-tabs",
+    "sphinxcontrib-django",
 ]
-
-[project.scripts]
-allianceauth = "allianceauth.bin.allianceauth:main"
-
-[project.urls]
-Homepage = "https://gitlab.com/allianceauth/allianceauth"
-Documentation = "https://allianceauth.readthedocs.io/"
-Source = "https://gitlab.com/allianceauth/allianceauth"
-Tracker = "https://gitlab.com/allianceauth/allianceauth/-/issues"
+optional-dependencies.test = [
+    "coverage>=4.3.1",
+    "django-webtest",
+    "requests-mock>=1.2",
+]
+urls.Documentation = "https://allianceauth.readthedocs.io/"
+urls.Homepage = "https://gitlab.com/allianceauth/allianceauth"
+urls.Source = "https://gitlab.com/allianceauth/allianceauth"
+urls.Tracker = "https://gitlab.com/allianceauth/allianceauth/-/issues"
+scripts.allianceauth = "allianceauth.bin.allianceauth:main"
 
 [tool.flit.module]
 name = "allianceauth"
 
 [tool.isort]
 profile = "django"
 sections = [
     "FUTURE",
     "STDLIB",
     "THIRDPARTY",
     "DJANGO",
     "ESI",
     "FIRSTPARTY",
-    "LOCALFOLDER"
+    "LOCALFOLDER",
+]
+known_esi = [
+    "esi",
+]
+known_django = [
+    "django",
 ]
-known_esi = ["esi"]
-known_django = ["django"]
 skip_gitignore = true
```

### Comparing `allianceauth-4.0.1/PKG-INFO` & `allianceauth-4.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,62 +1,63 @@
 Metadata-Version: 2.1
 Name: allianceauth
-Version: 4.0.1
+Version: 4.0.2
 Summary: An auth system for EVE Online to help in-game organizations
 Keywords: allianceauth,eveonline
 Author-email: Alliance Auth <adarnof@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Dist: bcrypt
 Requires-Dist: beautifulsoup4
+Requires-Dist: celery<6,>=5.2
 Requires-Dist: celery-once>=3.0.1
-Requires-Dist: celery>=5.2.0,<6
-Requires-Dist: django-bootstrap5>=23.3
+Requires-Dist: django<5,>=4.2
 Requires-Dist: django-bootstrap-form
-Requires-Dist: django-celery-beat>=2.3.0
-Requires-Dist: django-esi>=5.0.0
-Requires-Dist: django-redis>=5.2.0
-Requires-Dist: django-registration>=3.3,<3.4
+Requires-Dist: django-bootstrap5>=23.3
+Requires-Dist: django-celery-beat>=2.3
+Requires-Dist: django-esi>=5
+Requires-Dist: django-redis>=5.2
+Requires-Dist: django-registration<3.4,>=3.3
 Requires-Dist: django-sortedm2m
-Requires-Dist: django>=4.2,<5
 Requires-Dist: dnspython
-Requires-Dist: mysqlclient>=2.1.0
+Requires-Dist: mysqlclient>=2.1
 Requires-Dist: openfire-restapi
-Requires-Dist: packaging>=21.0
+Requires-Dist: packaging>=21
 Requires-Dist: passlib
 Requires-Dist: pydiscourse
 Requires-Dist: python-slugify>=1.2
-Requires-Dist: redis>=4.0.0
-Requires-Dist: requests-oauthlib
+Requires-Dist: redis>=4
 Requires-Dist: requests>=2.9.1
+Requires-Dist: requests-oauthlib
 Requires-Dist: semantic-version
 Requires-Dist: slixmpp
-Requires-Dist: sphinx ; extra == "docs"
-Requires-Dist: sphinx_rtd_theme>=2.0.0,<3.0.0 ; extra == "docs"
 Requires-Dist: myst-parser ; extra == "docs"
-Requires-Dist: sphinxcontrib-django ; extra == "docs"
+Requires-Dist: sphinx ; extra == "docs"
 Requires-Dist: sphinx-copybutton ; extra == "docs"
+Requires-Dist: sphinx-rtd-theme<3,>=2 ; extra == "docs"
 Requires-Dist: sphinx-tabs ; extra == "docs"
+Requires-Dist: sphinxcontrib-django ; extra == "docs"
 Requires-Dist: coverage>=4.3.1 ; extra == "test"
 Requires-Dist: django-webtest ; extra == "test"
-Requires-Dist: requests-mock>=1.2.0 ; extra == "test"
+Requires-Dist: requests-mock>=1.2 ; extra == "test"
 Project-URL: Documentation, https://allianceauth.readthedocs.io/
 Project-URL: Homepage, https://gitlab.com/allianceauth/allianceauth
 Project-URL: Source, https://gitlab.com/allianceauth/allianceauth
 Project-URL: Tracker, https://gitlab.com/allianceauth/allianceauth/-/issues
 Provides-Extra: docs
 Provides-Extra: test
```

