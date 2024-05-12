# Comparing `tmp/ce_ui-1.7.2.tar.gz` & `tmp/ce_ui-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ce_ui-1.7.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "ce_ui-1.8.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ce_ui-1.7.2.tar` & `ce_ui-1.8.0.tar`

### file list

```diff
@@ -1,91 +1,92 @@
--rw-r--r--   0        0        0     1076 2024-03-22 11:53:30.970506 ce_ui-1.7.2/LICENSE
--rw-r--r--   0        0        0      429 2024-03-22 11:53:30.970506 ce_ui-1.7.2/README.rst
--rw-r--r--   0        0        0       47 2024-03-22 11:53:30.970506 ce_ui-1.7.2/ce_ui/__init__.py
--rw-r--r--   0        0        0      649 2024-03-22 11:53:30.970506 ce_ui-1.7.2/ce_ui/apps.py
--rw-r--r--   0        0        0     2550 2024-03-22 11:53:30.970506 ce_ui-1.7.2/ce_ui/context_processors.py
--rw-r--r--   0        0        0     3478 2024-03-22 11:53:30.970506 ce_ui-1.7.2/ce_ui/management/commands/import_terms.py
--rw-r--r--   0        0        0    11850 2024-03-22 11:53:30.970506 ce_ui-1.7.2/ce_ui/serializers.py
--rw-r--r--   0        0        0      415 2024-03-22 11:53:30.970506 ce_ui-1.7.2/ce_ui/signals.py
--rw-r--r--   0        0        0      167 2024-03-22 11:53:30.970506 ce_ui-1.7.2/ce_ui/static/images/README.md
--rw-r--r--   0        0        0     8883 2024-03-22 11:53:30.970506 ce_ui-1.7.2/ce_ui/static/images/cc/cc0-1.0.svg
--rw-r--r--   0        0        0    10236 2024-03-22 11:53:30.970506 ce_ui-1.7.2/ce_ui/static/images/cc/ccby-4.0.svg
--rw-r--r--   0        0        0    16462 2024-03-22 11:53:30.970506 ce_ui-1.7.2/ce_ui/static/images/cc/ccbysa-4.0.svg
--rw-r--r--   0        0        0     5067 2024-03-22 11:53:30.970506 ce_ui-1.7.2/ce_ui/static/images/ce_logo.svg
--rw-r--r--   0        0        0    16601 2024-03-22 11:53:30.970506 ce_ui-1.7.2/ce_ui/static/images/erc_logo.png
--rw-r--r--   0        0        0     2407 2024-03-22 11:53:30.970506 ce_ui-1.7.2/ce_ui/static/images/favicons/favicon.png
--rw-r--r--   0        0        0    19728 2024-03-22 11:53:30.970506 ce_ui-1.7.2/ce_ui/static/images/logo_livmats_small.jpg
--rw-r--r--   0        0        0    20123 2024-03-22 11:53:30.970506 ce_ui-1.7.2/ce_ui/static/images/pitt_logo.png
--rw-r--r--   0        0        0   819426 2024-03-22 11:53:30.974506 ce_ui-1.7.2/ce_ui/static/images/screenshot_contact_mechanics.png
--rw-r--r--   0        0        0  1107943 2024-03-22 11:53:30.982506 ce_ui-1.7.2/ce_ui/static/images/screenshot_psd.png
--rw-r--r--   0        0        0    51196 2024-03-22 11:53:30.982506 ce_ui-1.7.2/ce_ui/static/images/thumbnail_unavailable.png
--rw-r--r--   0        0        0     3355 2024-03-22 11:53:30.982506 ce_ui-1.7.2/ce_ui/static/images/uni_freiburg_logo.png
-lrwxr-xr-x   0        0        0        0 2024-03-22 11:53:30.982506 ce_ui-1.7.2/ce_ui/static/other/CHANGELOG.md -> ../../../CHANGELOG.md
--rw-r--r--   0        0        0    24306 2024-03-22 11:53:30.982506 ce_ui-1.7.2/ce_ui/static/other/TermsConditions-2.0.md
--rw-r--r--   0        0        0     5086 2024-03-22 11:53:30.982506 ce_ui-1.7.2/ce_ui/static/other/TermsConditions.md
--rw-r--r--   0        0        0     2735 2024-03-22 11:53:30.982506 ce_ui-1.7.2/ce_ui/static/other/TermsConditionsSupplement.md
--rw-r--r--   0        0        0     2736 2024-03-22 11:53:30.982506 ce_ui-1.7.2/ce_ui/static/vendor/openseadragon/FileSaver.min.js
--rw-r--r--   0        0        0    10404 2024-03-22 11:53:30.982506 ce_ui-1.7.2/ce_ui/static/vendor/openseadragon/FileSaver.min.js.map
--rw-r--r--   0        0        0    23965 2024-03-22 11:53:30.982506 ce_ui-1.7.2/ce_ui/static/vendor/openseadragon/openseadragon-scalebar.js
--rw-r--r--   0        0        0   247016 2024-03-22 11:53:30.982506 ce_ui-1.7.2/ce_ui/static/vendor/openseadragon/openseadragon.min.js
--rw-r--r--   0        0        0   301334 2024-03-22 11:53:30.986506 ce_ui-1.7.2/ce_ui/static/vendor/openseadragon/openseadragon.min.js.map
--rw-r--r--   0        0        0      573 2024-03-22 11:53:30.986506 ce_ui-1.7.2/ce_ui/templates/403.html
--rw-r--r--   0        0        0      167 2024-03-22 11:53:30.986506 ce_ui-1.7.2/ce_ui/templates/403_csrf.html
--rw-r--r--   0        0        0      269 2024-03-22 11:53:30.986506 ce_ui-1.7.2/ce_ui/templates/404.html
--rw-r--r--   0        0        0      582 2024-03-22 11:53:30.986506 ce_ui-1.7.2/ce_ui/templates/500.html
--rw-r--r--   0        0        0      242 2024-03-22 11:53:30.986506 ce_ui-1.7.2/ce_ui/templates/account/account_inactive.html
--rw-r--r--   0        0        0      254 2024-03-22 11:53:30.986506 ce_ui-1.7.2/ce_ui/templates/account/base.html
--rw-r--r--   0        0        0     2622 2024-03-22 11:53:30.986506 ce_ui-1.7.2/ce_ui/templates/account/email.html
--rw-r--r--   0        0        0      950 2024-03-22 11:53:30.986506 ce_ui-1.7.2/ce_ui/templates/account/email_confirm.html
--rw-r--r--   0        0        0     1455 2024-03-22 11:53:30.986506 ce_ui-1.7.2/ce_ui/templates/account/login.html
--rw-r--r--   0        0        0      540 2024-03-22 11:53:30.986506 ce_ui-1.7.2/ce_ui/templates/account/logout.html
--rw-r--r--   0        0        0      490 2024-03-22 11:53:30.986506 ce_ui-1.7.2/ce_ui/templates/account/password_change.html
--rw-r--r--   0        0        0      859 2024-03-22 11:53:30.986506 ce_ui-1.7.2/ce_ui/templates/account/password_reset.html
--rw-r--r--   0        0        0      473 2024-03-22 11:53:30.986506 ce_ui-1.7.2/ce_ui/templates/account/password_reset_done.html
--rw-r--r--   0        0        0      957 2024-03-22 11:53:30.986506 ce_ui-1.7.2/ce_ui/templates/account/password_reset_from_key.html
--rw-r--r--   0        0        0      250 2024-03-22 11:53:30.986506 ce_ui-1.7.2/ce_ui/templates/account/password_reset_from_key_done.html
--rw-r--r--   0        0        0      451 2024-03-22 11:53:30.986506 ce_ui-1.7.2/ce_ui/templates/account/password_set.html
--rw-r--r--   0        0        0      688 2024-03-22 11:53:30.986506 ce_ui-1.7.2/ce_ui/templates/account/signup.html
--rw-r--r--   0        0        0      263 2024-03-22 11:53:30.986506 ce_ui-1.7.2/ce_ui/templates/account/signup_closed.html
--rw-r--r--   0        0        0      436 2024-03-22 11:53:30.986506 ce_ui-1.7.2/ce_ui/templates/account/verification_sent.html
--rw-r--r--   0        0        0      796 2024-03-22 11:53:30.986506 ce_ui-1.7.2/ce_ui/templates/account/verified_email_required.html
--rw-r--r--   0        0        0     1102 2024-03-22 11:53:30.986506 ce_ui-1.7.2/ce_ui/templates/analysis/analyses_detail.html
--rw-r--r--   0        0        0      671 2024-03-22 11:53:30.986506 ce_ui-1.7.2/ce_ui/templates/analysis/analyses_list.html
--rw-r--r--   0        0        0    25061 2024-03-22 11:53:30.986506 ce_ui-1.7.2/ce_ui/templates/base.html
--rw-r--r--   0        0        0      149 2024-03-22 11:53:30.986506 ce_ui-1.7.2/ce_ui/templates/manager/fa5_icon.html
--rw-r--r--   0        0        0     1307 2024-03-22 11:53:30.986506 ce_ui-1.7.2/ce_ui/templates/manager/file_formats.html
--rw-r--r--   0        0        0     3809 2024-03-22 11:53:30.986506 ce_ui-1.7.2/ce_ui/templates/manager/select.html
--rw-r--r--   0        0        0      764 2024-03-22 11:53:30.986506 ce_ui-1.7.2/ce_ui/templates/manager/share.html
--rw-r--r--   0        0        0      722 2024-03-22 11:53:30.986506 ce_ui-1.7.2/ce_ui/templates/manager/surface_detail.html
--rw-r--r--   0        0        0      752 2024-03-22 11:53:30.986506 ce_ui-1.7.2/ce_ui/templates/manager/topography_detail.html
--rw-r--r--   0        0        0       26 2024-03-22 11:53:30.986506 ce_ui-1.7.2/ce_ui/templates/pages/about.html
--rw-r--r--   0        0        0     3958 2024-03-22 11:53:30.986506 ce_ui-1.7.2/ce_ui/templates/pages/basic_usage.html
--rw-r--r--   0        0        0     1151 2024-03-22 11:53:30.986506 ce_ui-1.7.2/ce_ui/templates/pages/help.html
--rw-r--r--   0        0        0     9071 2024-03-22 11:53:30.986506 ce_ui-1.7.2/ce_ui/templates/pages/home.html
--rw-r--r--   0        0        0     2082 2024-03-22 11:53:30.986506 ce_ui-1.7.2/ce_ui/templates/pages/termsconditions.html
--rw-r--r--   0        0        0      881 2024-03-22 11:53:30.986506 ce_ui-1.7.2/ce_ui/templates/tabnav/tabs.html
--rw-r--r--   0        0        0     1498 2024-03-22 11:53:30.986506 ce_ui-1.7.2/ce_ui/templates/users/user_detail.html
--rw-r--r--   0        0        0      474 2024-03-22 11:53:30.986506 ce_ui-1.7.2/ce_ui/templates/users/user_form.html
--rw-r--r--   0        0        0       69 2024-03-22 11:53:30.986506 ce_ui-1.7.2/ce_ui/templates/users/user_label.html
--rw-r--r--   0        0        0      426 2024-03-22 11:53:30.986506 ce_ui-1.7.2/ce_ui/templates/users/user_list.html
--rw-r--r--   0        0        0        0 2024-03-22 11:53:30.986506 ce_ui-1.7.2/ce_ui/templatetags/__init__.py
--rw-r--r--   0        0        0      487 2024-03-22 11:53:30.986506 ce_ui-1.7.2/ce_ui/templatetags/icon_tags.py
--rw-r--r--   0        0        0     2253 2024-03-22 11:53:30.986506 ce_ui-1.7.2/ce_ui/templatetags/tabnav_tags.py
--rw-r--r--   0        0        0        0 2024-03-22 11:53:30.986506 ce_ui-1.7.2/ce_ui/tests/__init__.py
--rw-r--r--   0        0        0      631 2024-03-22 11:53:30.986506 ce_ui-1.7.2/ce_ui/tests/conftest.py
--rw-r--r--   0        0        0      234 2024-03-22 11:53:30.986506 ce_ui-1.7.2/ce_ui/tests/fixtures.py
--rw-r--r--   0        0        0     1441 2024-03-22 11:53:30.986506 ce_ui-1.7.2/ce_ui/tests/test_anonymous.py
--rw-r--r--   0        0        0      245 2024-03-22 11:53:30.986506 ce_ui-1.7.2/ce_ui/tests/test_api.py
--rw-r--r--   0        0        0      576 2024-03-22 11:53:30.986506 ce_ui-1.7.2/ce_ui/tests/test_challenge_redirect.py
--rw-r--r--   0        0        0     2843 2024-03-22 11:53:30.986506 ce_ui-1.7.2/ce_ui/tests/test_handling.py
--rw-r--r--   0        0        0     1510 2024-03-22 11:53:30.986506 ce_ui-1.7.2/ce_ui/tests/test_prevent_url_guessing.py
--rw-r--r--   0        0        0    53839 2024-03-22 11:53:30.986506 ce_ui-1.7.2/ce_ui/tests/test_search.py
--rw-r--r--   0        0        0    13579 2024-03-22 11:53:30.986506 ce_ui-1.7.2/ce_ui/tests/test_select_tab.py
--rw-r--r--   0        0        0     7799 2024-03-22 11:53:30.986506 ce_ui-1.7.2/ce_ui/tests/test_utils.py
--rw-r--r--   0        0        0     2181 2024-03-22 11:53:30.986506 ce_ui-1.7.2/ce_ui/tests/test_welcome_page.py
--rw-r--r--   0        0        0      984 2024-03-22 11:53:30.986506 ce_ui-1.7.2/ce_ui/tests/utils.py
--rw-r--r--   0        0        0     4721 2024-03-22 11:53:30.986506 ce_ui-1.7.2/ce_ui/urls.py
--rw-r--r--   0        0        0    19875 2024-03-22 11:53:30.986506 ce_ui-1.7.2/ce_ui/utils.py
--rw-r--r--   0        0        0       86 2024-03-22 11:53:30.986506 ce_ui-1.7.2/ce_ui/version.py
--rw-r--r--   0        0        0    34148 2024-03-22 11:53:30.986506 ce_ui-1.7.2/ce_ui/views.py
--rw-r--r--   0        0        0     1819 2024-03-22 11:53:30.990506 ce_ui-1.7.2/pyproject.toml
--rw-r--r--   0        0        0     1596 1970-01-01 00:00:00.000000 ce_ui-1.7.2/PKG-INFO
+-rw-r--r--   0        0        0     1076 2024-05-12 21:08:17.313362 ce_ui-1.8.0/LICENSE
+-rw-r--r--   0        0        0      429 2024-05-12 21:08:17.313362 ce_ui-1.8.0/README.rst
+-rw-r--r--   0        0        0       47 2024-05-12 21:08:17.313362 ce_ui-1.8.0/ce_ui/__init__.py
+-rw-r--r--   0        0        0      649 2024-05-12 21:08:17.313362 ce_ui-1.8.0/ce_ui/apps.py
+-rw-r--r--   0        0        0     2550 2024-05-12 21:08:17.313362 ce_ui-1.8.0/ce_ui/context_processors.py
+-rw-r--r--   0        0        0     3478 2024-05-12 21:08:17.313362 ce_ui-1.8.0/ce_ui/management/commands/import_terms.py
+-rw-r--r--   0        0        0    11850 2024-05-12 21:08:17.313362 ce_ui-1.8.0/ce_ui/serializers.py
+-rw-r--r--   0        0        0      415 2024-05-12 21:08:17.313362 ce_ui-1.8.0/ce_ui/signals.py
+-rw-r--r--   0        0        0      167 2024-05-12 21:08:17.313362 ce_ui-1.8.0/ce_ui/static/images/README.md
+-rw-r--r--   0        0        0     8883 2024-05-12 21:08:17.313362 ce_ui-1.8.0/ce_ui/static/images/cc/cc0-1.0.svg
+-rw-r--r--   0        0        0    10236 2024-05-12 21:08:17.313362 ce_ui-1.8.0/ce_ui/static/images/cc/ccby-4.0.svg
+-rw-r--r--   0        0        0    16462 2024-05-12 21:08:17.313362 ce_ui-1.8.0/ce_ui/static/images/cc/ccbysa-4.0.svg
+-rw-r--r--   0        0        0     5067 2024-05-12 21:08:17.313362 ce_ui-1.8.0/ce_ui/static/images/ce_logo.svg
+-rw-r--r--   0        0        0    16601 2024-05-12 21:08:17.313362 ce_ui-1.8.0/ce_ui/static/images/erc_logo.png
+-rw-r--r--   0        0        0     2407 2024-05-12 21:08:17.313362 ce_ui-1.8.0/ce_ui/static/images/favicons/favicon.png
+-rw-r--r--   0        0        0    19728 2024-05-12 21:08:17.313362 ce_ui-1.8.0/ce_ui/static/images/logo_livmats_small.jpg
+-rw-r--r--   0        0        0    49148 2024-05-12 21:08:17.313362 ce_ui-1.8.0/ce_ui/static/images/nsf_logo.png
+-rw-r--r--   0        0        0    20123 2024-05-12 21:08:17.313362 ce_ui-1.8.0/ce_ui/static/images/pitt_logo.png
+-rw-r--r--   0        0        0   156800 2024-05-12 21:08:17.313362 ce_ui-1.8.0/ce_ui/static/images/screenshot_contact_mechanics.jpg
+-rw-r--r--   0        0        0   182968 2024-05-12 21:08:17.317362 ce_ui-1.8.0/ce_ui/static/images/screenshot_psd.jpg
+-rw-r--r--   0        0        0    51196 2024-05-12 21:08:17.317362 ce_ui-1.8.0/ce_ui/static/images/thumbnail_unavailable.png
+-rw-r--r--   0        0        0     3355 2024-05-12 21:08:17.317362 ce_ui-1.8.0/ce_ui/static/images/uni_freiburg_logo.png
+lrwxr-xr-x   0        0        0        0 2024-05-12 21:08:17.317362 ce_ui-1.8.0/ce_ui/static/other/CHANGELOG.md -> ../../../CHANGELOG.md
+-rw-r--r--   0        0        0    24306 2024-05-12 21:08:17.317362 ce_ui-1.8.0/ce_ui/static/other/TermsConditions-2.0.md
+-rw-r--r--   0        0        0     5086 2024-05-12 21:08:17.317362 ce_ui-1.8.0/ce_ui/static/other/TermsConditions.md
+-rw-r--r--   0        0        0     2735 2024-05-12 21:08:17.317362 ce_ui-1.8.0/ce_ui/static/other/TermsConditionsSupplement.md
+-rw-r--r--   0        0        0     2736 2024-05-12 21:08:17.317362 ce_ui-1.8.0/ce_ui/static/vendor/openseadragon/FileSaver.min.js
+-rw-r--r--   0        0        0    10404 2024-05-12 21:08:17.317362 ce_ui-1.8.0/ce_ui/static/vendor/openseadragon/FileSaver.min.js.map
+-rw-r--r--   0        0        0    23965 2024-05-12 21:08:17.317362 ce_ui-1.8.0/ce_ui/static/vendor/openseadragon/openseadragon-scalebar.js
+-rw-r--r--   0        0        0   247016 2024-05-12 21:08:17.317362 ce_ui-1.8.0/ce_ui/static/vendor/openseadragon/openseadragon.min.js
+-rw-r--r--   0        0        0   301334 2024-05-12 21:08:17.321362 ce_ui-1.8.0/ce_ui/static/vendor/openseadragon/openseadragon.min.js.map
+-rw-r--r--   0        0        0      573 2024-05-12 21:08:17.321362 ce_ui-1.8.0/ce_ui/templates/403.html
+-rw-r--r--   0        0        0      167 2024-05-12 21:08:17.321362 ce_ui-1.8.0/ce_ui/templates/403_csrf.html
+-rw-r--r--   0        0        0      269 2024-05-12 21:08:17.321362 ce_ui-1.8.0/ce_ui/templates/404.html
+-rw-r--r--   0        0        0      582 2024-05-12 21:08:17.321362 ce_ui-1.8.0/ce_ui/templates/500.html
+-rw-r--r--   0        0        0      242 2024-05-12 21:08:17.321362 ce_ui-1.8.0/ce_ui/templates/account/account_inactive.html
+-rw-r--r--   0        0        0      254 2024-05-12 21:08:17.321362 ce_ui-1.8.0/ce_ui/templates/account/base.html
+-rw-r--r--   0        0        0     2622 2024-05-12 21:08:17.321362 ce_ui-1.8.0/ce_ui/templates/account/email.html
+-rw-r--r--   0        0        0      950 2024-05-12 21:08:17.321362 ce_ui-1.8.0/ce_ui/templates/account/email_confirm.html
+-rw-r--r--   0        0        0     1455 2024-05-12 21:08:17.321362 ce_ui-1.8.0/ce_ui/templates/account/login.html
+-rw-r--r--   0        0        0      540 2024-05-12 21:08:17.321362 ce_ui-1.8.0/ce_ui/templates/account/logout.html
+-rw-r--r--   0        0        0      490 2024-05-12 21:08:17.321362 ce_ui-1.8.0/ce_ui/templates/account/password_change.html
+-rw-r--r--   0        0        0      859 2024-05-12 21:08:17.321362 ce_ui-1.8.0/ce_ui/templates/account/password_reset.html
+-rw-r--r--   0        0        0      473 2024-05-12 21:08:17.321362 ce_ui-1.8.0/ce_ui/templates/account/password_reset_done.html
+-rw-r--r--   0        0        0      957 2024-05-12 21:08:17.321362 ce_ui-1.8.0/ce_ui/templates/account/password_reset_from_key.html
+-rw-r--r--   0        0        0      250 2024-05-12 21:08:17.321362 ce_ui-1.8.0/ce_ui/templates/account/password_reset_from_key_done.html
+-rw-r--r--   0        0        0      451 2024-05-12 21:08:17.321362 ce_ui-1.8.0/ce_ui/templates/account/password_set.html
+-rw-r--r--   0        0        0      688 2024-05-12 21:08:17.321362 ce_ui-1.8.0/ce_ui/templates/account/signup.html
+-rw-r--r--   0        0        0      263 2024-05-12 21:08:17.321362 ce_ui-1.8.0/ce_ui/templates/account/signup_closed.html
+-rw-r--r--   0        0        0      436 2024-05-12 21:08:17.321362 ce_ui-1.8.0/ce_ui/templates/account/verification_sent.html
+-rw-r--r--   0        0        0      796 2024-05-12 21:08:17.321362 ce_ui-1.8.0/ce_ui/templates/account/verified_email_required.html
+-rw-r--r--   0        0        0     1102 2024-05-12 21:08:17.321362 ce_ui-1.8.0/ce_ui/templates/analysis/analyses_detail.html
+-rw-r--r--   0        0        0      671 2024-05-12 21:08:17.321362 ce_ui-1.8.0/ce_ui/templates/analysis/analyses_list.html
+-rw-r--r--   0        0        0    25249 2024-05-12 21:08:17.321362 ce_ui-1.8.0/ce_ui/templates/base.html
+-rw-r--r--   0        0        0      149 2024-05-12 21:08:17.321362 ce_ui-1.8.0/ce_ui/templates/manager/fa5_icon.html
+-rw-r--r--   0        0        0     1307 2024-05-12 21:08:17.321362 ce_ui-1.8.0/ce_ui/templates/manager/file_formats.html
+-rw-r--r--   0        0        0     3809 2024-05-12 21:08:17.321362 ce_ui-1.8.0/ce_ui/templates/manager/select.html
+-rw-r--r--   0        0        0      764 2024-05-12 21:08:17.321362 ce_ui-1.8.0/ce_ui/templates/manager/share.html
+-rw-r--r--   0        0        0      722 2024-05-12 21:08:17.321362 ce_ui-1.8.0/ce_ui/templates/manager/surface_detail.html
+-rw-r--r--   0        0        0      752 2024-05-12 21:08:17.321362 ce_ui-1.8.0/ce_ui/templates/manager/topography_detail.html
+-rw-r--r--   0        0        0       26 2024-05-12 21:08:17.321362 ce_ui-1.8.0/ce_ui/templates/pages/about.html
+-rw-r--r--   0        0        0     3958 2024-05-12 21:08:17.321362 ce_ui-1.8.0/ce_ui/templates/pages/basic_usage.html
+-rw-r--r--   0        0        0     1151 2024-05-12 21:08:17.321362 ce_ui-1.8.0/ce_ui/templates/pages/help.html
+-rw-r--r--   0        0        0    11034 2024-05-12 21:08:17.321362 ce_ui-1.8.0/ce_ui/templates/pages/home.html
+-rw-r--r--   0        0        0     2082 2024-05-12 21:08:17.321362 ce_ui-1.8.0/ce_ui/templates/pages/termsconditions.html
+-rw-r--r--   0        0        0      881 2024-05-12 21:08:17.321362 ce_ui-1.8.0/ce_ui/templates/tabnav/tabs.html
+-rw-r--r--   0        0        0     1498 2024-05-12 21:08:17.321362 ce_ui-1.8.0/ce_ui/templates/users/user_detail.html
+-rw-r--r--   0        0        0      474 2024-05-12 21:08:17.321362 ce_ui-1.8.0/ce_ui/templates/users/user_form.html
+-rw-r--r--   0        0        0       69 2024-05-12 21:08:17.321362 ce_ui-1.8.0/ce_ui/templates/users/user_label.html
+-rw-r--r--   0        0        0      426 2024-05-12 21:08:17.321362 ce_ui-1.8.0/ce_ui/templates/users/user_list.html
+-rw-r--r--   0        0        0        0 2024-05-12 21:08:17.321362 ce_ui-1.8.0/ce_ui/templatetags/__init__.py
+-rw-r--r--   0        0        0      487 2024-05-12 21:08:17.321362 ce_ui-1.8.0/ce_ui/templatetags/icon_tags.py
+-rw-r--r--   0        0        0     2253 2024-05-12 21:08:17.321362 ce_ui-1.8.0/ce_ui/templatetags/tabnav_tags.py
+-rw-r--r--   0        0        0        0 2024-05-12 21:08:17.321362 ce_ui-1.8.0/ce_ui/tests/__init__.py
+-rw-r--r--   0        0        0      631 2024-05-12 21:08:17.321362 ce_ui-1.8.0/ce_ui/tests/conftest.py
+-rw-r--r--   0        0        0      234 2024-05-12 21:08:17.321362 ce_ui-1.8.0/ce_ui/tests/fixtures.py
+-rw-r--r--   0        0        0     1441 2024-05-12 21:08:17.321362 ce_ui-1.8.0/ce_ui/tests/test_anonymous.py
+-rw-r--r--   0        0        0      245 2024-05-12 21:08:17.321362 ce_ui-1.8.0/ce_ui/tests/test_api.py
+-rw-r--r--   0        0        0      576 2024-05-12 21:08:17.321362 ce_ui-1.8.0/ce_ui/tests/test_challenge_redirect.py
+-rw-r--r--   0        0        0     2843 2024-05-12 21:08:17.321362 ce_ui-1.8.0/ce_ui/tests/test_handling.py
+-rw-r--r--   0        0        0     1510 2024-05-12 21:08:17.321362 ce_ui-1.8.0/ce_ui/tests/test_prevent_url_guessing.py
+-rw-r--r--   0        0        0    53839 2024-05-12 21:08:17.321362 ce_ui-1.8.0/ce_ui/tests/test_search.py
+-rw-r--r--   0        0        0    13579 2024-05-12 21:08:17.321362 ce_ui-1.8.0/ce_ui/tests/test_select_tab.py
+-rw-r--r--   0        0        0     7799 2024-05-12 21:08:17.321362 ce_ui-1.8.0/ce_ui/tests/test_utils.py
+-rw-r--r--   0        0        0     2181 2024-05-12 21:08:17.321362 ce_ui-1.8.0/ce_ui/tests/test_welcome_page.py
+-rw-r--r--   0        0        0      984 2024-05-12 21:08:17.321362 ce_ui-1.8.0/ce_ui/tests/utils.py
+-rw-r--r--   0        0        0     4721 2024-05-12 21:08:17.321362 ce_ui-1.8.0/ce_ui/urls.py
+-rw-r--r--   0        0        0    19875 2024-05-12 21:08:17.321362 ce_ui-1.8.0/ce_ui/utils.py
+-rw-r--r--   0        0        0       86 2024-05-12 21:08:17.321362 ce_ui-1.8.0/ce_ui/version.py
+-rw-r--r--   0        0        0    34148 2024-05-12 21:08:17.321362 ce_ui-1.8.0/ce_ui/views.py
+-rw-r--r--   0        0        0     1819 2024-05-12 21:08:17.325362 ce_ui-1.8.0/pyproject.toml
+-rw-r--r--   0        0        0     1596 1970-01-01 00:00:00.000000 ce_ui-1.8.0/PKG-INFO
```

### Comparing `ce_ui-1.7.2/LICENSE` & `ce_ui-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ce_ui-1.7.2/ce_ui/apps.py` & `ce_ui-1.8.0/ce_ui/apps.py`

 * *Files identical despite different names*

### Comparing `ce_ui-1.7.2/ce_ui/context_processors.py` & `ce_ui-1.8.0/ce_ui/context_processors.py`

 * *Files identical despite different names*

### Comparing `ce_ui-1.7.2/ce_ui/management/commands/import_terms.py` & `ce_ui-1.8.0/ce_ui/management/commands/import_terms.py`

 * *Files identical despite different names*

### Comparing `ce_ui-1.7.2/ce_ui/serializers.py` & `ce_ui-1.8.0/ce_ui/serializers.py`

 * *Files identical despite different names*

### Comparing `ce_ui-1.7.2/ce_ui/static/images/cc/cc0-1.0.svg` & `ce_ui-1.8.0/ce_ui/static/images/cc/cc0-1.0.svg`

 * *Files identical despite different names*

### Comparing `ce_ui-1.7.2/ce_ui/static/images/cc/ccby-4.0.svg` & `ce_ui-1.8.0/ce_ui/static/images/cc/ccby-4.0.svg`

 * *Files identical despite different names*

### Comparing `ce_ui-1.7.2/ce_ui/static/images/cc/ccbysa-4.0.svg` & `ce_ui-1.8.0/ce_ui/static/images/cc/ccbysa-4.0.svg`

 * *Files identical despite different names*

### Comparing `ce_ui-1.7.2/ce_ui/static/images/ce_logo.svg` & `ce_ui-1.8.0/ce_ui/static/images/ce_logo.svg`

 * *Files identical despite different names*

### Comparing `ce_ui-1.7.2/ce_ui/static/images/erc_logo.png` & `ce_ui-1.8.0/ce_ui/static/images/erc_logo.png`

 * *Files identical despite different names*

### Comparing `ce_ui-1.7.2/ce_ui/static/images/favicons/favicon.png` & `ce_ui-1.8.0/ce_ui/static/images/favicons/favicon.png`

 * *Files identical despite different names*

### Comparing `ce_ui-1.7.2/ce_ui/static/images/logo_livmats_small.jpg` & `ce_ui-1.8.0/ce_ui/static/images/logo_livmats_small.jpg`

 * *Files identical despite different names*

### Comparing `ce_ui-1.7.2/ce_ui/static/images/pitt_logo.png` & `ce_ui-1.8.0/ce_ui/static/images/pitt_logo.png`

 * *Files identical despite different names*

### Comparing `ce_ui-1.7.2/ce_ui/static/images/thumbnail_unavailable.png` & `ce_ui-1.8.0/ce_ui/static/images/thumbnail_unavailable.png`

 * *Files identical despite different names*

### Comparing `ce_ui-1.7.2/ce_ui/static/images/uni_freiburg_logo.png` & `ce_ui-1.8.0/ce_ui/static/images/uni_freiburg_logo.png`

 * *Files identical despite different names*

### Comparing `ce_ui-1.7.2/ce_ui/static/other/TermsConditions-2.0.md` & `ce_ui-1.8.0/ce_ui/static/other/TermsConditions-2.0.md`

 * *Files identical despite different names*

### Comparing `ce_ui-1.7.2/ce_ui/static/other/TermsConditions.md` & `ce_ui-1.8.0/ce_ui/static/other/TermsConditions.md`

 * *Files identical despite different names*

### Comparing `ce_ui-1.7.2/ce_ui/static/other/TermsConditionsSupplement.md` & `ce_ui-1.8.0/ce_ui/static/other/TermsConditionsSupplement.md`

 * *Files identical despite different names*

### Comparing `ce_ui-1.7.2/ce_ui/static/vendor/openseadragon/FileSaver.min.js` & `ce_ui-1.8.0/ce_ui/static/vendor/openseadragon/FileSaver.min.js`

 * *Files identical despite different names*

### Comparing `ce_ui-1.7.2/ce_ui/static/vendor/openseadragon/FileSaver.min.js.map` & `ce_ui-1.8.0/ce_ui/static/vendor/openseadragon/FileSaver.min.js.map`

 * *Files identical despite different names*

### Comparing `ce_ui-1.7.2/ce_ui/static/vendor/openseadragon/openseadragon-scalebar.js` & `ce_ui-1.8.0/ce_ui/static/vendor/openseadragon/openseadragon-scalebar.js`

 * *Files identical despite different names*

### Comparing `ce_ui-1.7.2/ce_ui/static/vendor/openseadragon/openseadragon.min.js` & `ce_ui-1.8.0/ce_ui/static/vendor/openseadragon/openseadragon.min.js`

 * *Files identical despite different names*

### Comparing `ce_ui-1.7.2/ce_ui/static/vendor/openseadragon/openseadragon.min.js.map` & `ce_ui-1.8.0/ce_ui/static/vendor/openseadragon/openseadragon.min.js.map`

 * *Files identical despite different names*

### Comparing `ce_ui-1.7.2/ce_ui/templates/403.html` & `ce_ui-1.8.0/ce_ui/templates/403.html`

 * *Files identical despite different names*

### Comparing `ce_ui-1.7.2/ce_ui/templates/500.html` & `ce_ui-1.8.0/ce_ui/templates/500.html`

 * *Files identical despite different names*

### Comparing `ce_ui-1.7.2/ce_ui/templates/account/email.html` & `ce_ui-1.8.0/ce_ui/templates/account/email.html`

 * *Files identical despite different names*

### Comparing `ce_ui-1.7.2/ce_ui/templates/account/email_confirm.html` & `ce_ui-1.8.0/ce_ui/templates/account/email_confirm.html`

 * *Files identical despite different names*

### Comparing `ce_ui-1.7.2/ce_ui/templates/account/login.html` & `ce_ui-1.8.0/ce_ui/templates/account/login.html`

 * *Files identical despite different names*

### Comparing `ce_ui-1.7.2/ce_ui/templates/account/logout.html` & `ce_ui-1.8.0/ce_ui/templates/account/logout.html`

 * *Files identical despite different names*

### Comparing `ce_ui-1.7.2/ce_ui/templates/account/password_reset.html` & `ce_ui-1.8.0/ce_ui/templates/account/password_reset.html`

 * *Files identical despite different names*

### Comparing `ce_ui-1.7.2/ce_ui/templates/account/password_reset_from_key.html` & `ce_ui-1.8.0/ce_ui/templates/account/password_reset_from_key.html`

 * *Files identical despite different names*

### Comparing `ce_ui-1.7.2/ce_ui/templates/account/signup.html` & `ce_ui-1.8.0/ce_ui/templates/account/signup.html`

 * *Files identical despite different names*

### Comparing `ce_ui-1.7.2/ce_ui/templates/account/verified_email_required.html` & `ce_ui-1.8.0/ce_ui/templates/account/verified_email_required.html`

 * *Files identical despite different names*

### Comparing `ce_ui-1.7.2/ce_ui/templates/analysis/analyses_detail.html` & `ce_ui-1.8.0/ce_ui/templates/analysis/analyses_detail.html`

 * *Files identical despite different names*

### Comparing `ce_ui-1.7.2/ce_ui/templates/analysis/analyses_list.html` & `ce_ui-1.8.0/ce_ui/templates/analysis/analyses_list.html`

 * *Files identical despite different names*

### Comparing `ce_ui-1.7.2/ce_ui/templates/base.html` & `ce_ui-1.8.0/ce_ui/templates/base.html`

 * *Files 2% similar despite different names*

```diff
@@ -42,17 +42,17 @@
         {# Logo / name of the application #}
         <a class="navbar-brand ms-3" href="{% url 'home' %}"><img src="{% static 'images/ce_logo.svg' %}" height="25px">&nbsp
             contact.engineering</a>
         {% if request %}  {# in case of error 500, there is no request #}
             <div class="collapse navbar-collapse" id="navbar_supported_content">
 
                 {# Search Bar #}
-                <div class="navbar-nav flex-grow-1">
-                    <form class="form-inline" action="{% url 'ce_ui:select' %}" method="get">
-                        <div class="input-group" id="global-search">
+                <div class="navbar-nav flex-grow-1 ms-5 me-5">
+                    <form class="form-inline w-100" action="{% url 'ce_ui:select' %}" method="get">
+                        <div class="input-group w-100" id="global-search">
                             <label class="sr-only" for="global-search-input">Search Term</label>
                             <input class="form-control" type="search" id="global-search-input"
                                    placeholder="Search names, descriptions, and tags" name="search">
                             <button class="btn btn-outline-secondary" type="submit">{% fa5_icon 'search' %}</button>
                             <button class="btn btn-outline-secondary" type="button"
                                     data-toggle="modal" data-target="#search-help-modal"
                                     title="Tipps for searching">{% fa5_icon 'info-circle' %}</button>
@@ -175,31 +175,32 @@
 
     <!-- /#content-wrapper -->
 </div>
 
 <footer class="sticky-footer">
     <div class="container my-auto">
         <div class="copyright text-center my-auto">
-            <a href="https://pastewka.org/" target="_blank">
+            <a href="https://pastewka.org/" target="_blank" class="text-decoration-none">
                 <img src="{% static 'images/uni_freiburg_logo.png' %}" height="64px"></img>
             </a>
-            &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
-            <a href="http://www.engineering.pitt.edu/TevisJacobs/" target="_blank">
+            <a href="http://www.engineering.pitt.edu/TevisJacobs/" target="_blank" class="text-decoration-none">
                 <img src="{% static 'images/pitt_logo.png' %}" height="64px"></img>
             </a>
             &nbsp&nbsp&nbsp&#8213;&nbsp&nbsp&nbsp
             Funding by
             &nbsp&nbsp&nbsp
-            <a href="https://cordis.europa.eu/project/rcn/212185_en.html" target="_blank">
+            <a href="https://erc.europa.eu/" target="_blank" class="text-decoration-none">
                 <img src="{% static 'images/erc_logo.png' %}" height="64px"></img>
             </a>
-            &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
-            <a href="https://www.livmats.uni-freiburg.de/" target="_blank">
+            <a href="https://www.livmats.uni-freiburg.de/" target="_blank" class="text-decoration-none">
                 <img src="{% static 'images/logo_livmats_small.jpg' %}" height="64px"></img>
             </a>
+            <a href="https://www.nsf.gov/" target="_blank" class="text-decoration-none">
+                <img src="{% static 'images/nsf_logo.png' %}" height="64px"></img>
+            </a>
         </div>
     </div>
 </footer>
 
 <!-- /#page-wrapper -->
 <!-- Scroll to Top Button-->
 <a class="scroll-to-top rounded" href="#page-top" style="display: inline;">
```

#### html2text {}

```diff
@@ -25,17 +25,17 @@
 {# Places Messages #} {% if messages %} {% for message in messages %}
 {{ message }}
 {% endfor %} {% endif %} {# Insert actual content, see other templates #} {%
 block content %} {% endblock content %}
 {# Check for terms and conditions, show a pop up if there are changes #} {#
 show_terms_if_not_agreed #} {# <- enable by replacing # with % #} {# Note that
 the user can close the modal and it is reopened every new view #}
-_[_{_%_ _s_t_a_t_i_c_ _'_i_m_a_g_e_s_/_u_n_i___f_r_e_i_b_u_r_g___l_o_g_o_._p_n_g_'_ _%_}_]          _[_{_%_ _s_t_a_t_i_c_ _'_i_m_a_g_e_s_/
-_p_i_t_t___l_o_g_o_._p_n_g_'_ _%_}_]   ―    Funding by     _[_{_%_ _s_t_a_t_i_c_ _'_i_m_a_g_e_s_/_e_r_c___l_o_g_o_._p_n_g_'
-_%_}_]     _[_{_%_ _s_t_a_t_i_c_ _'_i_m_a_g_e_s_/_l_o_g_o___l_i_v_m_a_t_s___s_m_a_l_l_._j_p_g_'_ _%_}_]
+_[_{_%_ _s_t_a_t_i_c_ _'_i_m_a_g_e_s_/_u_n_i___f_r_e_i_b_u_r_g___l_o_g_o_._p_n_g_'_ _%_}_]_[_{_%_ _s_t_a_t_i_c_ _'_i_m_a_g_e_s_/_p_i_t_t___l_o_g_o_._p_n_g_'
+_%_}_]   ―    Funding by    _[_{_%_ _s_t_a_t_i_c_ _'_i_m_a_g_e_s_/_e_r_c___l_o_g_o_._p_n_g_'_ _%_}_]_[_{_%_ _s_t_a_t_i_c
+_'_i_m_a_g_e_s_/_l_o_g_o___l_i_v_m_a_t_s___s_m_a_l_l_._j_p_g_'_ _%_}_]_[_{_%_ _s_t_a_t_i_c_ _'_i_m_a_g_e_s_/_n_s_f___l_o_g_o_._p_n_g_'_ _%_}_]
 **** RReeaaddyy ttoo LLeeaavvee?? ****
 Select "Sign Out" below if you are ready to end your current session.
 Cancel _{_%_ _t_r_a_n_s_ _"_S_i_g_n_ _o_u_t_"_ _%_}
 **** VVeerrssiioonn iinnffoorrmmaattiioonn ****
 This cloud platform builds on the open source software packages summarized in
 the following list.
 MMoodduullee    VVeerrssiioonn             LLiicceennssee             LLiinnkkss
```

### Comparing `ce_ui-1.7.2/ce_ui/templates/manager/file_formats.html` & `ce_ui-1.8.0/ce_ui/templates/manager/file_formats.html`

 * *Files identical despite different names*

### Comparing `ce_ui-1.7.2/ce_ui/templates/manager/select.html` & `ce_ui-1.8.0/ce_ui/templates/manager/select.html`

 * *Files identical despite different names*

### Comparing `ce_ui-1.7.2/ce_ui/templates/manager/share.html` & `ce_ui-1.8.0/ce_ui/templates/manager/share.html`

 * *Files identical despite different names*

### Comparing `ce_ui-1.7.2/ce_ui/templates/manager/surface_detail.html` & `ce_ui-1.8.0/ce_ui/templates/manager/surface_detail.html`

 * *Files identical despite different names*

### Comparing `ce_ui-1.7.2/ce_ui/templates/manager/topography_detail.html` & `ce_ui-1.8.0/ce_ui/templates/manager/topography_detail.html`

 * *Files identical despite different names*

### Comparing `ce_ui-1.7.2/ce_ui/templates/pages/basic_usage.html` & `ce_ui-1.8.0/ce_ui/templates/pages/basic_usage.html`

 * *Files identical despite different names*

### Comparing `ce_ui-1.7.2/ce_ui/templates/pages/help.html` & `ce_ui-1.8.0/ce_ui/templates/pages/help.html`

 * *Files identical despite different names*

### Comparing `ce_ui-1.7.2/ce_ui/templates/pages/home.html` & `ce_ui-1.8.0/ce_ui/templates/pages/home.html`

 * *Files 15% similar despite different names*

```diff
@@ -20,22 +20,43 @@
                     </p>
                 </div>
             </div>
             <div class="container">
                 {% if request.user.is_anonymous %}
                     <div class="row">
                         <div class="col-6">
-                            <a href="/ui/html/analysis-detail/14/?subjects=eyJzdXJmYWNlIjogWzE1MDVdfQ==">
-                                <img src="{% static 'images/screenshot_psd.png' %}" width="100%"/>
-                            </a>
+                            <div class="opacity-container">
+                                <a href="/ui/html/analysis-detail/14/?subjects=eyJzdXJmYWNlIjogWzE1MDVdfQ==">
+                                    <img class="image"
+                                         src="{% static 'images/screenshot_psd.png' %}"
+                                         width="100%"/>
+                                </a>
+                                <div class="middle">
+                                    <a href="/ui/html/analysis-detail/14/?subjects=eyJzdXJmYWNlIjogWzE1MDVdfQ=="
+                                       class="btn btn-secondary">
+                                        Combine analyses on multiple measurements into a complete
+                                        statistical representation of a surface.
+                                    </a>
+                                </div>
+                            </div>
                         </div>
                         <div class="col-6">
-                            <a href="/ui/html/analysis-detail/18/?subjects=eyJ0b3BvZ3JhcGh5IjpbMTk1OV19">
-                                <img src="{% static 'images/screenshot_contact_mechanics.png' %}" width="100%"/>
-                            </a>
+                            <div class="opacity-container">
+                                <a href="/ui/html/analysis-detail/18/?subjects=eyJ0b3BvZ3JhcGh5IjpbMTk1OV19">
+                                    <img class="image"
+                                         src="{% static 'images/screenshot_contact_mechanics.png' %}"
+                                         width="100%"/>
+                                </a>
+                                <div class="middle">
+                                    <a href="/ui/html/analysis-detail/18/?subjects=eyJ0b3BvZ3JhcGh5IjpbMTk1OV19"
+                                       class="btn btn-secondary">
+                                        Carry out contact mechanical calculations with the boundary element method.
+                                    </a>
+                                </div>
+                            </div>
                         </div>
                     </div>
                 {% else %}
                     <div class="row">
                         <div class="col-xl-3 col-sm-6 mb-3">
                             <a href="{% url 'ce_ui:select' %}" class="card-link text-decoration-none">
                                 <div class="card text-white bg-primary o-hidden h-100">
@@ -132,16 +153,26 @@
                             <p><em>Digital surface twins</em> can be <em>shared</em> with others for collaboration. You
                                 decide whether
                                 your collaborators can modify them or not.</p>
                             <p>Digital surface twins can also be <em>published</em> to make them citable and accessible
                                 for everyone.</p>
                         </div>
                     {% else %}
-                        <div class="col-md-12">
-                            <h2>Login via ORCID</h2>
+                        <div class="col-md-6">
+                            <h2>Browse published digital surface twins</h2>
+                            <p>A <em>digital surface twin</em> combines multiple measurements of a real-life surface,
+                                together with descriptive metadata.
+                            <p>
+                                <a id="orcid-log-in-link" class="btn btn-secondary" href="{% url 'ce_ui:select' %}">
+                                    Browse digital surface twins
+                                </a>
+                            </p>
+                        </div>
+                        <div class="col-md-6">
+                            <h2>Sign in to upload measurements</h2>
                             <p>
                                 Please allow the ORCID site to authenticate yourself to contact.engineering.
                                 If you don't have an ORCID account yet, you will be able to register.
                             </p>
                             <p>
                                 <a id="orcid-log-in-link" class="btn btn-secondary"
                                    href="{% provider_login_url 'orcid' method="oauth2" %}">
```

#### html2text {}

```diff
@@ -4,15 +4,18 @@
 This is a web-based application that allows you to: Store and organize surface
 measurements, characterize surface topography, analyze contact properties and
 (if you wish) share your data with collaborators or even publish your datasets.
 For more information on this site _p_l_e_a_s_e_ _r_e_a_d_ _t_h_e_ _a_c_c_o_m_p_a_n_y_i_n_g_ _o_p_e_n_ _a_c_c_e_s_s
 _p_a_p_e_r.
 {% if request.user.is_anonymous %}
 _[_{_%_ _s_t_a_t_i_c_ _'_i_m_a_g_e_s_/_s_c_r_e_e_n_s_h_o_t___p_s_d_._p_n_g_'_ _%_}_]
+_C_o_m_b_i_n_e_ _a_n_a_l_y_s_e_s_ _o_n_ _m_u_l_t_i_p_l_e_ _m_e_a_s_u_r_e_m_e_n_t_s_ _i_n_t_o_ _a_ _c_o_m_p_l_e_t_e_ _s_t_a_t_i_s_t_i_c_a_l
+_r_e_p_r_e_s_e_n_t_a_t_i_o_n_ _o_f_ _a_ _s_u_r_f_a_c_e_.
 _[_{_%_ _s_t_a_t_i_c_ _'_i_m_a_g_e_s_/_s_c_r_e_e_n_s_h_o_t___c_o_n_t_a_c_t___m_e_c_h_a_n_i_c_s_._p_n_g_'_ _%_}_]
+_C_a_r_r_y_ _o_u_t_ _c_o_n_t_a_c_t_ _m_e_c_h_a_n_i_c_a_l_ _c_a_l_c_u_l_a_t_i_o_n_s_ _w_i_t_h_ _t_h_e_ _b_o_u_n_d_a_r_y_ _e_l_e_m_e_n_t_ _m_e_t_h_o_d_.
 {% else %}
 _Y_o_u_ _h_a_v_e
 _{_{_ _n_u_m___s_u_r_f_a_c_e_s_ _}_}
 _d_i_g_i_t_a_l_ _s_u_r_f_a_c_e_ _t_w_i_n_s_.
 _Y_o_u_ _h_a_v_e
 _{_{_ _n_u_m___t_o_p_o_g_r_a_p_h_i_e_s_ _}_}
 _i_n_d_i_v_i_d_u_a_l_ _m_e_a_s_u_r_e_m_e_n_t_s_.
@@ -40,13 +43,17 @@
 spectral density of a ddiiggiittaall ssuurrffaaccee ttwwiinn.
 ****** SShhaarriinngg && ppuubblliisshhiinngg ******
 DDiiggiittaall ssuurrffaaccee ttwwiinnss can be sshhaarreedd with others for collaboration. You decide
 whether your collaborators can modify them or not.
 Digital surface twins can also be ppuubblliisshheedd to make them citable and accessible
 for everyone.
 {% else %}
-********** LLooggiinn vviiaa OORRCCIIDD **********
+********** BBrroowwssee ppuubblliisshheedd ddiiggiittaall ssuurrffaaccee ttwwiinnss **********
+A ddiiggiittaall ssuurrffaaccee ttwwiinn combines multiple measurements of a real-life surface,
+together with descriptive metadata.
+_B_r_o_w_s_e_ _d_i_g_i_t_a_l_ _s_u_r_f_a_c_e_ _t_w_i_n_s
+********** SSiiggnn iinn ttoo uuppllooaadd mmeeaassuurreemmeennttss **********
 Please allow the ORCID site to authenticate yourself to contact.engineering. If
 you don't have an ORCID account yet, you will be able to register.
 }"> Sign in using your ORCID account
 {% endif %}
 {% endblock %}
```

### Comparing `ce_ui-1.7.2/ce_ui/templates/pages/termsconditions.html` & `ce_ui-1.8.0/ce_ui/templates/pages/termsconditions.html`

 * *Files identical despite different names*

### Comparing `ce_ui-1.7.2/ce_ui/templates/tabnav/tabs.html` & `ce_ui-1.8.0/ce_ui/templates/tabnav/tabs.html`

 * *Files identical despite different names*

### Comparing `ce_ui-1.7.2/ce_ui/templates/users/user_detail.html` & `ce_ui-1.8.0/ce_ui/templates/users/user_detail.html`

 * *Files identical despite different names*

### Comparing `ce_ui-1.7.2/ce_ui/templatetags/tabnav_tags.py` & `ce_ui-1.8.0/ce_ui/templatetags/tabnav_tags.py`

 * *Files identical despite different names*

### Comparing `ce_ui-1.7.2/ce_ui/tests/conftest.py` & `ce_ui-1.8.0/ce_ui/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ce_ui-1.7.2/ce_ui/tests/test_anonymous.py` & `ce_ui-1.8.0/ce_ui/tests/test_anonymous.py`

 * *Files identical despite different names*

### Comparing `ce_ui-1.7.2/ce_ui/tests/test_challenge_redirect.py` & `ce_ui-1.8.0/ce_ui/tests/test_challenge_redirect.py`

 * *Files identical despite different names*

### Comparing `ce_ui-1.7.2/ce_ui/tests/test_handling.py` & `ce_ui-1.8.0/ce_ui/tests/test_handling.py`

 * *Files identical despite different names*

### Comparing `ce_ui-1.7.2/ce_ui/tests/test_prevent_url_guessing.py` & `ce_ui-1.8.0/ce_ui/tests/test_prevent_url_guessing.py`

 * *Files identical despite different names*

### Comparing `ce_ui-1.7.2/ce_ui/tests/test_search.py` & `ce_ui-1.8.0/ce_ui/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `ce_ui-1.7.2/ce_ui/tests/test_select_tab.py` & `ce_ui-1.8.0/ce_ui/tests/test_select_tab.py`

 * *Files identical despite different names*

### Comparing `ce_ui-1.7.2/ce_ui/tests/test_utils.py` & `ce_ui-1.8.0/ce_ui/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `ce_ui-1.7.2/ce_ui/tests/test_welcome_page.py` & `ce_ui-1.8.0/ce_ui/tests/test_welcome_page.py`

 * *Files identical despite different names*

### Comparing `ce_ui-1.7.2/ce_ui/tests/utils.py` & `ce_ui-1.8.0/ce_ui/tests/utils.py`

 * *Files identical despite different names*

### Comparing `ce_ui-1.7.2/ce_ui/urls.py` & `ce_ui-1.8.0/ce_ui/urls.py`

 * *Files identical despite different names*

### Comparing `ce_ui-1.7.2/ce_ui/utils.py` & `ce_ui-1.8.0/ce_ui/utils.py`

 * *Files identical despite different names*

### Comparing `ce_ui-1.7.2/ce_ui/views.py` & `ce_ui-1.8.0/ce_ui/views.py`

 * *Files identical despite different names*

### Comparing `ce_ui-1.7.2/pyproject.toml` & `ce_ui-1.8.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ce_ui-1.7.2/PKG-INFO` & `ce_ui-1.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ce-ui
-Version: 1.7.2
+Version: 1.8.0
 Summary: The user-facing interface of contact.engineering.
 Author-email: Michael Röttger <info@michael-roettger.de>, Lars Pastewka <lars.pastewka@imtek.uni-freiburg.de>
 Requires-Python: >=3.8.0
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

