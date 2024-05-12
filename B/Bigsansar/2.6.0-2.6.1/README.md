# Comparing `tmp/bigsansar-2.6.0.tar.gz` & `tmp/bigsansar-2.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bigsansar-2.6.0.tar", last modified: Sat May 11 16:16:35 2024, max compression
+gzip compressed data, was "bigsansar-2.6.1.tar", last modified: Sun May 12 03:47:04 2024, max compression
```

## Comparing `bigsansar-2.6.0.tar` & `bigsansar-2.6.1.tar`

### file list

```diff
@@ -1,197 +1,197 @@
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-11 16:16:35.628165 bigsansar-2.6.0/
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-11 16:16:35.618165 bigsansar-2.6.0/Bigsansar.egg-info/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     5363 2024-05-11 16:16:35.000000 bigsansar-2.6.0/Bigsansar.egg-info/PKG-INFO
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     7368 2024-05-11 16:16:35.000000 bigsansar-2.6.0/Bigsansar.egg-info/SOURCES.txt
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        1 2024-05-11 16:16:35.000000 bigsansar-2.6.0/Bigsansar.egg-info/dependency_links.txt
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)       50 2024-05-11 16:16:35.000000 bigsansar-2.6.0/Bigsansar.egg-info/entry_points.txt
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)       98 2024-05-11 16:16:35.000000 bigsansar-2.6.0/Bigsansar.egg-info/requires.txt
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)       10 2024-05-11 16:16:35.000000 bigsansar-2.6.0/Bigsansar.egg-info/top_level.txt
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1073 2024-04-10 03:12:24.000000 bigsansar-2.6.0/LICENSE
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     5363 2024-05-11 16:16:35.628165 bigsansar-2.6.0/PKG-INFO
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     4438 2024-05-11 15:06:57.000000 bigsansar-2.6.0/README.md
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-11 16:16:35.428165 bigsansar-2.6.0/bigsansar/
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/__init__.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)       63 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/admin.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      188 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/apps.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-11 16:16:35.428165 bigsansar-2.6.0/bigsansar/contrib/
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/contrib/__init__.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-11 16:16:35.438165 bigsansar-2.6.0/bigsansar/contrib/account/
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/contrib/account/__init__.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      489 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/contrib/account/admin.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      275 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/contrib/account/apps.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1155 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/contrib/account/forms.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-11 16:16:35.448165 bigsansar-2.6.0/bigsansar/contrib/account/migrations/
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      969 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/contrib/account/migrations/0001_initial.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      400 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/contrib/account/migrations/0002_alter_userinfo_options.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/contrib/account/migrations/__init__.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      539 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/contrib/account/models.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      340 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/contrib/account/signals.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-11 16:16:35.448165 bigsansar-2.6.0/bigsansar/contrib/account/templates/
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/contrib/account/templates/__init__.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)       60 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/contrib/account/tests.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/contrib/account/urls.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/contrib/account/views.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-11 16:16:35.458165 bigsansar-2.6.0/bigsansar/contrib/advance/
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/contrib/advance/__init__.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      165 2024-05-11 15:55:11.000000 bigsansar-2.6.0/bigsansar/contrib/advance/admin.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      202 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/contrib/advance/apps.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      357 2024-05-11 07:59:27.000000 bigsansar-2.6.0/bigsansar/contrib/advance/cf_url.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     4583 2024-04-16 12:22:05.000000 bigsansar-2.6.0/bigsansar/contrib/advance/forms.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-11 16:16:35.468165 bigsansar-2.6.0/bigsansar/contrib/advance/migrations/
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1000 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/contrib/advance/migrations/0001_initial.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      367 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/contrib/advance/migrations/0002_alter_css_options.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1050 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/contrib/advance/migrations/0003_javascript.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      386 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/contrib/advance/migrations/0004_alter_javascript_options.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      296 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/contrib/advance/migrations/0005_delete_css.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      289 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/contrib/advance/migrations/0006_delete_javascript.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1075 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/contrib/advance/migrations/0007_initial.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      527 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/contrib/advance/migrations/0008_sidebarsettings.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      631 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/contrib/advance/migrations/0009_sidebarsettings_user.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1000 2024-04-10 05:16:13.000000 bigsansar-2.6.0/bigsansar/contrib/advance/migrations/0010_cloudflare_api.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      391 2024-04-13 11:41:57.000000 bigsansar-2.6.0/bigsansar/contrib/advance/migrations/0011_rename_account_global_api_key_cloudflare_api_global_api_key.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      637 2024-04-16 11:46:02.000000 bigsansar-2.6.0/bigsansar/contrib/advance/migrations/0012_cloudflare_api_ip_address_cloudflare_api_ip_address2.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/contrib/advance/migrations/__init__.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1356 2024-04-16 11:46:06.000000 bigsansar-2.6.0/bigsansar/contrib/advance/models.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-11 16:16:35.478165 bigsansar-2.6.0/bigsansar/contrib/advance/templatetags/
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/contrib/advance/templatetags/__init__.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1797 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/contrib/advance/templatetags/nav_bar.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)       60 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/contrib/advance/tests.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      721 2024-04-16 11:03:13.000000 bigsansar-2.6.0/bigsansar/contrib/advance/urls.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)    20737 2024-05-11 15:51:42.000000 bigsansar-2.6.0/bigsansar/contrib/advance/views.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-11 16:16:35.488165 bigsansar-2.6.0/bigsansar/contrib/blogs/
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/contrib/blogs/__init__.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     2238 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/contrib/blogs/admin.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      188 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/contrib/blogs/apps.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      261 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/contrib/blogs/forms.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-11 16:16:35.488165 bigsansar-2.6.0/bigsansar/contrib/blogs/migrations/
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     2261 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/contrib/blogs/migrations/0001_initial.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      367 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/contrib/blogs/migrations/0002_post_visitor.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/contrib/blogs/migrations/__init__.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     2028 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/contrib/blogs/models.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-11 16:16:35.488165 bigsansar-2.6.0/bigsansar/contrib/blogs/templatetags/
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/contrib/blogs/templatetags/__init__.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1478 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/contrib/blogs/templatetags/blogs.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)       60 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/contrib/blogs/tests.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)       63 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/contrib/blogs/views.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-11 16:16:35.508165 bigsansar-2.6.0/bigsansar/contrib/sites/
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/contrib/sites/__init__.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1719 2024-05-11 15:54:05.000000 bigsansar-2.6.0/bigsansar/contrib/sites/admin.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      196 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/contrib/sites/apps.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     4435 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/contrib/sites/forms.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-11 16:16:35.518165 bigsansar-2.6.0/bigsansar/contrib/sites/migrations/
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1847 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/contrib/sites/migrations/0001_initial.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      819 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/contrib/sites/migrations/0002_default_domain.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      385 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/contrib/sites/migrations/0003_domains_default.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      386 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/contrib/sites/migrations/0004_alter_domains_default.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      331 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/contrib/sites/migrations/0005_remove_domains_default.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      653 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/contrib/sites/migrations/0006_default_domain_default_domain_and_more.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      410 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/contrib/sites/migrations/0007_alter_default_domain_default_domain.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      411 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/contrib/sites/migrations/0008_domains_primary_domain.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      346 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/contrib/sites/migrations/0009_remove_default_domain_default_domain.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      422 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/contrib/sites/migrations/0010_alter_domains_description.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      405 2024-05-09 10:32:01.000000 bigsansar-2.6.0/bigsansar/contrib/sites/migrations/0011_domains_zone_id.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/contrib/sites/migrations/__init__.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     2453 2024-05-09 10:31:51.000000 bigsansar-2.6.0/bigsansar/contrib/sites/models.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-11 16:16:35.518165 bigsansar-2.6.0/bigsansar/contrib/sites/templatetags/
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/contrib/sites/templatetags/__init__.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      394 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/contrib/sites/templatetags/pages.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)       60 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/contrib/sites/tests.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      547 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/contrib/sites/urls.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     9258 2024-04-10 10:36:13.000000 bigsansar-2.6.0/bigsansar/contrib/sites/views.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/contrib/urls.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/contrib/views.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-11 16:16:35.528165 bigsansar-2.6.0/bigsansar/core/
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1018 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/core/__init__.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      402 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/core/host.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     9710 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/core/init.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      640 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/core/pip_package.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)    16740 2024-05-11 16:16:09.000000 bigsansar-2.6.0/bigsansar/core/ubuntu.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-11 16:16:35.538165 bigsansar-2.6.0/bigsansar/etc/
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     7287 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/etc/apache2.conf
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1638 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/etc/config_chroot.sh
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     5123 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/etc/db.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     3236 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/etc/sshd_config
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-11 16:16:35.538165 bigsansar-2.6.0/bigsansar/management/
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/management/__init__.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-11 16:16:35.538165 bigsansar-2.6.0/bigsansar/management/commands/
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/management/commands/__init__.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1076 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/management/commands/createuser.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1023 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/management/commands/setup_server.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-11 16:16:35.538165 bigsansar-2.6.0/bigsansar/migrations/
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/migrations/__init__.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)       57 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/models.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-11 16:16:35.548165 bigsansar-2.6.0/bigsansar/static/
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/static/__init__.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-11 16:16:35.388165 bigsansar-2.6.0/bigsansar/static/ckeditor/
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-11 16:16:35.388165 bigsansar-2.6.0/bigsansar/static/ckeditor/ckeditor/
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-11 16:16:35.388165 bigsansar-2.6.0/bigsansar/static/ckeditor/ckeditor/plugins/
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-11 16:16:35.548165 bigsansar-2.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-11 16:16:35.548165 bigsansar-2.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/images/
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1258 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/images/icon-hdpi.png
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1165 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/images/icon.png
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-11 16:16:35.588165 bigsansar-2.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1337 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ar.js
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1654 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/bg.js
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1184 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/cs.js
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1078 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/de.js
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1514 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/el.js
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1024 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/en.js
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1084 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/es.js
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1079 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/et.js
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1161 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/eu.js
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      960 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/fi.js
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1051 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/fr.js
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1226 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/he.js
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1166 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/hu.js
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1081 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/it.js
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1171 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ja.js
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1229 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ko.js
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1035 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/nb.js
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1022 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/nl.js
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1040 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/nn.js
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1120 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/pl.js
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1151 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/pt-br.js
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1153 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/pt.js
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1539 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ru.js
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1173 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/sk.js
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1206 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/tr.js
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1538 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/uk.js
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1067 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/vi.js
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      916 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/zh.js
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)    13371 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/plugin.js
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     9230 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/static/logo.png
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      551 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/static/style.css
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-11 16:16:35.598165 bigsansar-2.6.0/bigsansar/templates/
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      947 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/templates/404.html
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/templates/__init__.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      164 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/templates/acc_active_email.html
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-11 16:16:35.618165 bigsansar-2.6.0/bigsansar/templates/admin/
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)    10272 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/templates/admin/account_info.html
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      519 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/templates/admin/admin_update.html
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      878 2024-04-13 11:47:55.000000 bigsansar-2.6.0/bigsansar/templates/admin/cf_config.html
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      558 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/templates/admin/chpass.html
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      558 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/templates/admin/chuname.html
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     4405 2024-05-11 15:46:30.000000 bigsansar-2.6.0/bigsansar/templates/admin/cloudflare.html
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      549 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/templates/admin/create_domain.html
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1637 2024-05-11 15:51:11.000000 bigsansar-2.6.0/bigsansar/templates/admin/db_cloudflare.html
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     8866 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/templates/admin/domain_manage.html
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1019 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/templates/admin/edit_domain.html
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      566 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/templates/admin/editprofile.html
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      979 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/templates/admin/login.html
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     6004 2024-04-16 11:03:44.000000 bigsansar-2.6.0/bigsansar/templates/admin/nav.html
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      947 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/templates/admin/page_create.html
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      948 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/templates/admin/page_delete.html
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      717 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/templates/admin/page_edit.html
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1622 2024-05-11 07:51:33.000000 bigsansar-2.6.0/bigsansar/templates/base.html
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1898 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/templates/blog_preview.html
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     2197 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/templates/default.html
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     2200 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/templates/defaultpage.html
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      719 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/templates/parking.html
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      101 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/templates/script.html
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      411 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/templates/sitemap.html
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      101 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/templates/styles.html
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)       60 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/tests.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1209 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/urls.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     4595 2024-04-10 03:12:24.000000 bigsansar-2.6.0/bigsansar/views.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       38 2024-05-11 16:16:35.628165 bigsansar-2.6.0/setup.cfg
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1914 2024-05-11 16:16:22.000000 bigsansar-2.6.0/setup.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 03:47:04.452508 bigsansar-2.6.1/
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 03:47:04.452508 bigsansar-2.6.1/Bigsansar.egg-info/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     5310 2024-05-12 03:47:04.000000 bigsansar-2.6.1/Bigsansar.egg-info/PKG-INFO
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     7368 2024-05-12 03:47:04.000000 bigsansar-2.6.1/Bigsansar.egg-info/SOURCES.txt
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        1 2024-05-12 03:47:04.000000 bigsansar-2.6.1/Bigsansar.egg-info/dependency_links.txt
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)       50 2024-05-12 03:47:04.000000 bigsansar-2.6.1/Bigsansar.egg-info/entry_points.txt
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)       98 2024-05-12 03:47:04.000000 bigsansar-2.6.1/Bigsansar.egg-info/requires.txt
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)       10 2024-05-12 03:47:04.000000 bigsansar-2.6.1/Bigsansar.egg-info/top_level.txt
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1073 2024-04-10 03:12:24.000000 bigsansar-2.6.1/LICENSE
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     5310 2024-05-12 03:47:04.452508 bigsansar-2.6.1/PKG-INFO
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     4385 2024-05-12 03:45:06.000000 bigsansar-2.6.1/README.md
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 03:47:04.282508 bigsansar-2.6.1/bigsansar/
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/__init__.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)       63 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/admin.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      188 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/apps.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 03:47:04.282508 bigsansar-2.6.1/bigsansar/contrib/
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/contrib/__init__.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 03:47:04.292508 bigsansar-2.6.1/bigsansar/contrib/account/
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/contrib/account/__init__.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      489 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/contrib/account/admin.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      275 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/contrib/account/apps.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1155 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/contrib/account/forms.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 03:47:04.292508 bigsansar-2.6.1/bigsansar/contrib/account/migrations/
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      969 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/contrib/account/migrations/0001_initial.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      400 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/contrib/account/migrations/0002_alter_userinfo_options.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/contrib/account/migrations/__init__.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      539 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/contrib/account/models.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      340 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/contrib/account/signals.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 03:47:04.292508 bigsansar-2.6.1/bigsansar/contrib/account/templates/
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/contrib/account/templates/__init__.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)       60 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/contrib/account/tests.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/contrib/account/urls.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/contrib/account/views.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 03:47:04.302508 bigsansar-2.6.1/bigsansar/contrib/advance/
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/contrib/advance/__init__.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      165 2024-05-12 03:46:34.000000 bigsansar-2.6.1/bigsansar/contrib/advance/admin.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      202 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/contrib/advance/apps.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      357 2024-05-11 07:59:27.000000 bigsansar-2.6.1/bigsansar/contrib/advance/cf_url.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     4583 2024-04-16 12:22:05.000000 bigsansar-2.6.1/bigsansar/contrib/advance/forms.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 03:47:04.312508 bigsansar-2.6.1/bigsansar/contrib/advance/migrations/
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1000 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/contrib/advance/migrations/0001_initial.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      367 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/contrib/advance/migrations/0002_alter_css_options.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1050 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/contrib/advance/migrations/0003_javascript.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      386 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/contrib/advance/migrations/0004_alter_javascript_options.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      296 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/contrib/advance/migrations/0005_delete_css.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      289 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/contrib/advance/migrations/0006_delete_javascript.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1075 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/contrib/advance/migrations/0007_initial.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      527 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/contrib/advance/migrations/0008_sidebarsettings.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      631 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/contrib/advance/migrations/0009_sidebarsettings_user.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1000 2024-04-10 05:16:13.000000 bigsansar-2.6.1/bigsansar/contrib/advance/migrations/0010_cloudflare_api.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      391 2024-04-13 11:41:57.000000 bigsansar-2.6.1/bigsansar/contrib/advance/migrations/0011_rename_account_global_api_key_cloudflare_api_global_api_key.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      637 2024-04-16 11:46:02.000000 bigsansar-2.6.1/bigsansar/contrib/advance/migrations/0012_cloudflare_api_ip_address_cloudflare_api_ip_address2.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/contrib/advance/migrations/__init__.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1356 2024-04-16 11:46:06.000000 bigsansar-2.6.1/bigsansar/contrib/advance/models.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 03:47:04.312508 bigsansar-2.6.1/bigsansar/contrib/advance/templatetags/
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/contrib/advance/templatetags/__init__.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1797 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/contrib/advance/templatetags/nav_bar.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)       60 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/contrib/advance/tests.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      721 2024-04-16 11:03:13.000000 bigsansar-2.6.1/bigsansar/contrib/advance/urls.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)    20765 2024-05-12 03:40:41.000000 bigsansar-2.6.1/bigsansar/contrib/advance/views.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 03:47:04.332508 bigsansar-2.6.1/bigsansar/contrib/blogs/
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/contrib/blogs/__init__.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     2238 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/contrib/blogs/admin.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      188 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/contrib/blogs/apps.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      261 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/contrib/blogs/forms.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 03:47:04.332508 bigsansar-2.6.1/bigsansar/contrib/blogs/migrations/
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     2261 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/contrib/blogs/migrations/0001_initial.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      367 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/contrib/blogs/migrations/0002_post_visitor.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/contrib/blogs/migrations/__init__.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     2028 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/contrib/blogs/models.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 03:47:04.332508 bigsansar-2.6.1/bigsansar/contrib/blogs/templatetags/
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/contrib/blogs/templatetags/__init__.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1478 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/contrib/blogs/templatetags/blogs.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)       60 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/contrib/blogs/tests.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)       63 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/contrib/blogs/views.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 03:47:04.352508 bigsansar-2.6.1/bigsansar/contrib/sites/
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/contrib/sites/__init__.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1719 2024-05-11 15:54:05.000000 bigsansar-2.6.1/bigsansar/contrib/sites/admin.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      196 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/contrib/sites/apps.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     4435 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/contrib/sites/forms.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 03:47:04.372508 bigsansar-2.6.1/bigsansar/contrib/sites/migrations/
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1847 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/contrib/sites/migrations/0001_initial.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      819 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/contrib/sites/migrations/0002_default_domain.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      385 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/contrib/sites/migrations/0003_domains_default.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      386 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/contrib/sites/migrations/0004_alter_domains_default.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      331 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/contrib/sites/migrations/0005_remove_domains_default.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      653 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/contrib/sites/migrations/0006_default_domain_default_domain_and_more.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      410 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/contrib/sites/migrations/0007_alter_default_domain_default_domain.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      411 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/contrib/sites/migrations/0008_domains_primary_domain.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      346 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/contrib/sites/migrations/0009_remove_default_domain_default_domain.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      422 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/contrib/sites/migrations/0010_alter_domains_description.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      405 2024-05-09 10:32:01.000000 bigsansar-2.6.1/bigsansar/contrib/sites/migrations/0011_domains_zone_id.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/contrib/sites/migrations/__init__.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     2453 2024-05-09 10:31:51.000000 bigsansar-2.6.1/bigsansar/contrib/sites/models.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 03:47:04.372508 bigsansar-2.6.1/bigsansar/contrib/sites/templatetags/
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/contrib/sites/templatetags/__init__.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      394 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/contrib/sites/templatetags/pages.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)       60 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/contrib/sites/tests.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      547 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/contrib/sites/urls.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     9258 2024-04-10 10:36:13.000000 bigsansar-2.6.1/bigsansar/contrib/sites/views.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/contrib/urls.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/contrib/views.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 03:47:04.372508 bigsansar-2.6.1/bigsansar/core/
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1018 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/core/__init__.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      402 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/core/host.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     9710 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/core/init.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      640 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/core/pip_package.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)    16740 2024-05-11 16:16:09.000000 bigsansar-2.6.1/bigsansar/core/ubuntu.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 03:47:04.372508 bigsansar-2.6.1/bigsansar/etc/
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     7287 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/etc/apache2.conf
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1638 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/etc/config_chroot.sh
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     5123 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/etc/db.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     3236 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/etc/sshd_config
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 03:47:04.372508 bigsansar-2.6.1/bigsansar/management/
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/management/__init__.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 03:47:04.372508 bigsansar-2.6.1/bigsansar/management/commands/
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/management/commands/__init__.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1076 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/management/commands/createuser.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1023 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/management/commands/setup_server.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 03:47:04.392508 bigsansar-2.6.1/bigsansar/migrations/
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/migrations/__init__.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)       57 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/models.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 03:47:04.392508 bigsansar-2.6.1/bigsansar/static/
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/static/__init__.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 03:47:04.262508 bigsansar-2.6.1/bigsansar/static/ckeditor/
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 03:47:04.262508 bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 03:47:04.262508 bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 03:47:04.392508 bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 03:47:04.392508 bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/images/
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1258 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/images/icon-hdpi.png
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1165 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/images/icon.png
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 03:47:04.412508 bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1337 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ar.js
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1654 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/bg.js
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1184 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/cs.js
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1078 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/de.js
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1514 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/el.js
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1024 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/en.js
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1084 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/es.js
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1079 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/et.js
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1161 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/eu.js
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      960 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/fi.js
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1051 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/fr.js
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1226 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/he.js
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1166 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/hu.js
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1081 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/it.js
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1171 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ja.js
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1229 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ko.js
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1035 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/nb.js
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1022 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/nl.js
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1040 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/nn.js
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1120 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/pl.js
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1151 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/pt-br.js
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1153 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/pt.js
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1539 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ru.js
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1173 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/sk.js
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1206 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/tr.js
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1538 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/uk.js
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1067 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/vi.js
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      916 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/zh.js
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)    13371 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/plugin.js
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     9230 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/static/logo.png
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      551 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/static/style.css
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 03:47:04.422508 bigsansar-2.6.1/bigsansar/templates/
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      947 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/templates/404.html
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/templates/__init__.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      164 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/templates/acc_active_email.html
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 03:47:04.452508 bigsansar-2.6.1/bigsansar/templates/admin/
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)    10272 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/templates/admin/account_info.html
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      519 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/templates/admin/admin_update.html
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      878 2024-04-13 11:47:55.000000 bigsansar-2.6.1/bigsansar/templates/admin/cf_config.html
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      558 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/templates/admin/chpass.html
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      558 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/templates/admin/chuname.html
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     4745 2024-05-12 03:43:14.000000 bigsansar-2.6.1/bigsansar/templates/admin/cloudflare.html
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      549 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/templates/admin/create_domain.html
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1637 2024-05-11 15:51:11.000000 bigsansar-2.6.1/bigsansar/templates/admin/db_cloudflare.html
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     8866 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/templates/admin/domain_manage.html
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1019 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/templates/admin/edit_domain.html
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      566 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/templates/admin/editprofile.html
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      979 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/templates/admin/login.html
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     6004 2024-04-16 11:03:44.000000 bigsansar-2.6.1/bigsansar/templates/admin/nav.html
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      947 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/templates/admin/page_create.html
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      948 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/templates/admin/page_delete.html
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      717 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/templates/admin/page_edit.html
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1622 2024-05-11 07:51:33.000000 bigsansar-2.6.1/bigsansar/templates/base.html
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1898 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/templates/blog_preview.html
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     2197 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/templates/default.html
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     2200 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/templates/defaultpage.html
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      719 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/templates/parking.html
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      101 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/templates/script.html
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      411 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/templates/sitemap.html
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      101 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/templates/styles.html
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)       60 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/tests.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1209 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/urls.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     4595 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/views.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       38 2024-05-12 03:47:04.452508 bigsansar-2.6.1/setup.cfg
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1914 2024-05-12 03:44:39.000000 bigsansar-2.6.1/setup.py
```

### Comparing `bigsansar-2.6.0/Bigsansar.egg-info/PKG-INFO` & `bigsansar-2.6.1/Bigsansar.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Bigsansar
-Version: 2.6.0
+Version: 2.6.1
 Summary: Build one in minutes with bigsansar - a visual site building tool!
 Home-page: https://github.com/pokhrelb9/bigsansar
 Author: Bikash Pokhrel
 Author-email: bigsansaroffice@gmail.com
 Project-URL: Bug Tracker, https://github.com/pokhrelb9/bigsansar/issues
 Project-URL: Documentations, https://docs.bigsansar.com/
 Keywords: python,django host,bigsansar,django,django sites framework,django flatpages
@@ -19,18 +19,19 @@
 Requires-Dist: django-phonenumber-field[phonenumberslite]
 Requires-Dist: django-ckeditor
 Requires-Dist: requests
 Requires-Dist: pillow
 Requires-Dist: fontawesomefree
 
 ## New update
+* fixed some bug in cloudflare api
 * Working in to cloudflare 
 * fixed some bugs
 * added new db table for nav always open or close.
-* now you can install bigsansar package in to ubuntu and all setup with on command lines
+
 
 # How to get Bigsansar
 
 Bigsansar is available open-source under the [MIT](https://en.wikipedia.org/wiki/MIT_License) license. We recommend using the latest version of Python 3.
 Bigsansar is Fully based on django and linux ubuntu.  You can use [bigsansar](https://bigsansar.com) for install packaged.
 You can use
 [bigsansar](https://bigsansar.com)
```

#### html2text {}

```diff
@@ -1,51 +1,51 @@
-Metadata-Version: 2.1 Name: Bigsansar Version: 2.6.0 Summary: Build one in
+Metadata-Version: 2.1 Name: Bigsansar Version: 2.6.1 Summary: Build one in
 minutes with bigsansar - a visual site building tool! Home-page: https://
 github.com/pokhrelb9/bigsansar Author: Bikash Pokhrel Author-email:
 bigsansaroffice@gmail.com Project-URL: Bug Tracker, https://github.com/
 pokhrelb9/bigsansar/issues Project-URL: Documentations, https://
 docs.bigsansar.com/ Keywords: python,django host,bigsansar,django,django sites
 framework,django flatpages Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: POSIX :: Linux Classifier: Operating System :: OS Independent Requires-
 Python: >=3.6 Description-Content-Type: text/markdown License-File: LICENSE
 Requires-Dist: django Requires-Dist: django-phonenumber-field[phonenumberslite]
 Requires-Dist: django-ckeditor Requires-Dist: requests Requires-Dist: pillow
-Requires-Dist: fontawesomefree ## New update * Working in to cloudflare * fixed
-some bugs * added new db table for nav always open or close. * now you can
-install bigsansar package in to ubuntu and all setup with on command lines #
-How to get Bigsansar Bigsansar is available open-source under the [MIT](https:/
-/en.wikipedia.org/wiki/MIT_License) license. We recommend using the latest
-version of Python 3. Bigsansar is Fully based on django and linux ubuntu. You
-can use [bigsansar](https://bigsansar.com) for install packaged. You can use
-[bigsansar](https://bigsansar.com) for install packaged. view our tutorials in
-[youtube](https://youtube.com/bigsansar) for playlist: [bigsansar for django]
-(https://www.youtube.com/playlist?list=PLbGzLu1WXrFUXw7qr6AMz5_iEkEAPV_Vs) #
-Get the latest development version The latest and greatest Bigsasnar version is
-the one thatâs in our Git repository (our revision-control system). This is
-only for experienced users who want to try incoming changes and help identify
-bugs before an official release. Get it using this shell command, which
-requires [Git](https://https://git-scm.com/): `git clone https://github.com/
-pokhrelb9/bigsansar.git` You can also download a [gzipped tarball](https://
-https://pypi.org/project/Bigsansar/#files) of the development version. This
-archive is updated every time we commit code. # After you install bigsansar 1)
-Type `bigsansar init` command for **automatically** setup server for internal
-configurations. ** this command valid into vertualenv for developer # for full
-setup in to server this is work only on ubuntu os 2) type ` python manage.py
-setup_server` commend for fully setup into server . [How to Setup a Full Server
-with BigSansar, Django, and Ubuntu ](https://youtu.be/j8YN6x9XdR4) # some
-usefull link [sitemap.xml](http://localhost/sitemap.xml) [script.js](http://
-localhost/script.js) [styles.css](http://localhost/styles.css) # how to edit
-sitemap , js and css from pages create a page **slug** name with sitemap,script
-, styles # How to change admin URL in server side with domain go to
-**VirtualHost.py** file and change **localhost** with your subdomain ## Some
-usefull commands: `python3 manage.py createuser` - get unlimited users. ##
-templatetags for extends and include {% extends '/.html' %} {% include '/.html'
-%} ## load blog list in templates `{% load blogs %} {% get_blog as bloglist %}
-{% for list in bloglist %}
+Requires-Dist: fontawesomefree ## New update * fixed some bug in cloudflare api
+* Working in to cloudflare * fixed some bugs * added new db table for nav
+always open or close. # How to get Bigsansar Bigsansar is available open-source
+under the [MIT](https://en.wikipedia.org/wiki/MIT_License) license. We
+recommend using the latest version of Python 3. Bigsansar is Fully based on
+django and linux ubuntu. You can use [bigsansar](https://bigsansar.com) for
+install packaged. You can use [bigsansar](https://bigsansar.com) for install
+packaged. view our tutorials in [youtube](https://youtube.com/bigsansar) for
+playlist: [bigsansar for django](https://www.youtube.com/
+playlist?list=PLbGzLu1WXrFUXw7qr6AMz5_iEkEAPV_Vs) # Get the latest development
+version The latest and greatest Bigsasnar version is the one thatâs in our
+Git repository (our revision-control system). This is only for experienced
+users who want to try incoming changes and help identify bugs before an
+official release. Get it using this shell command, which requires [Git](https:/
+/https://git-scm.com/): `git clone https://github.com/pokhrelb9/bigsansar.git`
+You can also download a [gzipped tarball](https://https://pypi.org/project/
+Bigsansar/#files) of the development version. This archive is updated every
+time we commit code. # After you install bigsansar 1) Type `bigsansar init`
+command for **automatically** setup server for internal configurations. ** this
+command valid into vertualenv for developer # for full setup in to server this
+is work only on ubuntu os 2) type ` python manage.py setup_server` commend for
+fully setup into server . [How to Setup a Full Server with BigSansar, Django,
+and Ubuntu ](https://youtu.be/j8YN6x9XdR4) # some usefull link [sitemap.xml]
+(http://localhost/sitemap.xml) [script.js](http://localhost/script.js)
+[styles.css](http://localhost/styles.css) # how to edit sitemap , js and css
+from pages create a page **slug** name with sitemap,script , styles # How to
+change admin URL in server side with domain go to **VirtualHost.py** file and
+change **localhost** with your subdomain ## Some usefull commands: `python3
+manage.py createuser` - get unlimited users. ## templatetags for extends and
+include {% extends '/.html' %} {% include '/.html' %} ## load blog list in
+templates `{% load blogs %} {% get_blog as bloglist %} {% for list in bloglist
+%}
 **** {{{{lliisstt..ttiittllee}}}} -- {{{{ lliisstt..ddoommaaiinn }}}} ****
 {{list.body|slice:":100"}} - {{ list.publish_date }}
 _R_e_a_d_ _M_o_r_e
 {% endfor %}` ## get single blog objects `{% load blogs %} {% get_blog_object
 as get_blog %} {{ get_blog.title }} {{ get_blog.thumbnails }} {
 { get_blog.publish_date }} {{ get_blog.domain }} {{ get_blog.id }} {
 { get_blog.slug }} {{ get_blog.body | safe }} {{ get_blog.visitor }} ` ## Count
```

### Comparing `bigsansar-2.6.0/Bigsansar.egg-info/SOURCES.txt` & `bigsansar-2.6.1/Bigsansar.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.0/LICENSE` & `bigsansar-2.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.0/PKG-INFO` & `bigsansar-2.6.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Bigsansar
-Version: 2.6.0
+Version: 2.6.1
 Summary: Build one in minutes with bigsansar - a visual site building tool!
 Home-page: https://github.com/pokhrelb9/bigsansar
 Author: Bikash Pokhrel
 Author-email: bigsansaroffice@gmail.com
 Project-URL: Bug Tracker, https://github.com/pokhrelb9/bigsansar/issues
 Project-URL: Documentations, https://docs.bigsansar.com/
 Keywords: python,django host,bigsansar,django,django sites framework,django flatpages
@@ -19,18 +19,19 @@
 Requires-Dist: django-phonenumber-field[phonenumberslite]
 Requires-Dist: django-ckeditor
 Requires-Dist: requests
 Requires-Dist: pillow
 Requires-Dist: fontawesomefree
 
 ## New update
+* fixed some bug in cloudflare api
 * Working in to cloudflare 
 * fixed some bugs
 * added new db table for nav always open or close.
-* now you can install bigsansar package in to ubuntu and all setup with on command lines
+
 
 # How to get Bigsansar
 
 Bigsansar is available open-source under the [MIT](https://en.wikipedia.org/wiki/MIT_License) license. We recommend using the latest version of Python 3.
 Bigsansar is Fully based on django and linux ubuntu.  You can use [bigsansar](https://bigsansar.com) for install packaged.
 You can use
 [bigsansar](https://bigsansar.com)
```

#### html2text {}

```diff
@@ -1,51 +1,51 @@
-Metadata-Version: 2.1 Name: Bigsansar Version: 2.6.0 Summary: Build one in
+Metadata-Version: 2.1 Name: Bigsansar Version: 2.6.1 Summary: Build one in
 minutes with bigsansar - a visual site building tool! Home-page: https://
 github.com/pokhrelb9/bigsansar Author: Bikash Pokhrel Author-email:
 bigsansaroffice@gmail.com Project-URL: Bug Tracker, https://github.com/
 pokhrelb9/bigsansar/issues Project-URL: Documentations, https://
 docs.bigsansar.com/ Keywords: python,django host,bigsansar,django,django sites
 framework,django flatpages Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: POSIX :: Linux Classifier: Operating System :: OS Independent Requires-
 Python: >=3.6 Description-Content-Type: text/markdown License-File: LICENSE
 Requires-Dist: django Requires-Dist: django-phonenumber-field[phonenumberslite]
 Requires-Dist: django-ckeditor Requires-Dist: requests Requires-Dist: pillow
-Requires-Dist: fontawesomefree ## New update * Working in to cloudflare * fixed
-some bugs * added new db table for nav always open or close. * now you can
-install bigsansar package in to ubuntu and all setup with on command lines #
-How to get Bigsansar Bigsansar is available open-source under the [MIT](https:/
-/en.wikipedia.org/wiki/MIT_License) license. We recommend using the latest
-version of Python 3. Bigsansar is Fully based on django and linux ubuntu. You
-can use [bigsansar](https://bigsansar.com) for install packaged. You can use
-[bigsansar](https://bigsansar.com) for install packaged. view our tutorials in
-[youtube](https://youtube.com/bigsansar) for playlist: [bigsansar for django]
-(https://www.youtube.com/playlist?list=PLbGzLu1WXrFUXw7qr6AMz5_iEkEAPV_Vs) #
-Get the latest development version The latest and greatest Bigsasnar version is
-the one thatâs in our Git repository (our revision-control system). This is
-only for experienced users who want to try incoming changes and help identify
-bugs before an official release. Get it using this shell command, which
-requires [Git](https://https://git-scm.com/): `git clone https://github.com/
-pokhrelb9/bigsansar.git` You can also download a [gzipped tarball](https://
-https://pypi.org/project/Bigsansar/#files) of the development version. This
-archive is updated every time we commit code. # After you install bigsansar 1)
-Type `bigsansar init` command for **automatically** setup server for internal
-configurations. ** this command valid into vertualenv for developer # for full
-setup in to server this is work only on ubuntu os 2) type ` python manage.py
-setup_server` commend for fully setup into server . [How to Setup a Full Server
-with BigSansar, Django, and Ubuntu ](https://youtu.be/j8YN6x9XdR4) # some
-usefull link [sitemap.xml](http://localhost/sitemap.xml) [script.js](http://
-localhost/script.js) [styles.css](http://localhost/styles.css) # how to edit
-sitemap , js and css from pages create a page **slug** name with sitemap,script
-, styles # How to change admin URL in server side with domain go to
-**VirtualHost.py** file and change **localhost** with your subdomain ## Some
-usefull commands: `python3 manage.py createuser` - get unlimited users. ##
-templatetags for extends and include {% extends '/.html' %} {% include '/.html'
-%} ## load blog list in templates `{% load blogs %} {% get_blog as bloglist %}
-{% for list in bloglist %}
+Requires-Dist: fontawesomefree ## New update * fixed some bug in cloudflare api
+* Working in to cloudflare * fixed some bugs * added new db table for nav
+always open or close. # How to get Bigsansar Bigsansar is available open-source
+under the [MIT](https://en.wikipedia.org/wiki/MIT_License) license. We
+recommend using the latest version of Python 3. Bigsansar is Fully based on
+django and linux ubuntu. You can use [bigsansar](https://bigsansar.com) for
+install packaged. You can use [bigsansar](https://bigsansar.com) for install
+packaged. view our tutorials in [youtube](https://youtube.com/bigsansar) for
+playlist: [bigsansar for django](https://www.youtube.com/
+playlist?list=PLbGzLu1WXrFUXw7qr6AMz5_iEkEAPV_Vs) # Get the latest development
+version The latest and greatest Bigsasnar version is the one thatâs in our
+Git repository (our revision-control system). This is only for experienced
+users who want to try incoming changes and help identify bugs before an
+official release. Get it using this shell command, which requires [Git](https:/
+/https://git-scm.com/): `git clone https://github.com/pokhrelb9/bigsansar.git`
+You can also download a [gzipped tarball](https://https://pypi.org/project/
+Bigsansar/#files) of the development version. This archive is updated every
+time we commit code. # After you install bigsansar 1) Type `bigsansar init`
+command for **automatically** setup server for internal configurations. ** this
+command valid into vertualenv for developer # for full setup in to server this
+is work only on ubuntu os 2) type ` python manage.py setup_server` commend for
+fully setup into server . [How to Setup a Full Server with BigSansar, Django,
+and Ubuntu ](https://youtu.be/j8YN6x9XdR4) # some usefull link [sitemap.xml]
+(http://localhost/sitemap.xml) [script.js](http://localhost/script.js)
+[styles.css](http://localhost/styles.css) # how to edit sitemap , js and css
+from pages create a page **slug** name with sitemap,script , styles # How to
+change admin URL in server side with domain go to **VirtualHost.py** file and
+change **localhost** with your subdomain ## Some usefull commands: `python3
+manage.py createuser` - get unlimited users. ## templatetags for extends and
+include {% extends '/.html' %} {% include '/.html' %} ## load blog list in
+templates `{% load blogs %} {% get_blog as bloglist %} {% for list in bloglist
+%}
 **** {{{{lliisstt..ttiittllee}}}} -- {{{{ lliisstt..ddoommaaiinn }}}} ****
 {{list.body|slice:":100"}} - {{ list.publish_date }}
 _R_e_a_d_ _M_o_r_e
 {% endfor %}` ## get single blog objects `{% load blogs %} {% get_blog_object
 as get_blog %} {{ get_blog.title }} {{ get_blog.thumbnails }} {
 { get_blog.publish_date }} {{ get_blog.domain }} {{ get_blog.id }} {
 { get_blog.slug }} {{ get_blog.body | safe }} {{ get_blog.visitor }} ` ## Count
```

### Comparing `bigsansar-2.6.0/README.md` & `bigsansar-2.6.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 ## New update
+* fixed some bug in cloudflare api
 * Working in to cloudflare 
 * fixed some bugs
 * added new db table for nav always open or close.
-* now you can install bigsansar package in to ubuntu and all setup with on command lines
+
 
 # How to get Bigsansar
 
 Bigsansar is available open-source under the [MIT](https://en.wikipedia.org/wiki/MIT_License) license. We recommend using the latest version of Python 3.
 Bigsansar is Fully based on django and linux ubuntu.  You can use [bigsansar](https://bigsansar.com) for install packaged.
 You can use
 [bigsansar](https://bigsansar.com)
```

#### html2text {}

```diff
@@ -1,26 +1,25 @@
-## New update * Working in to cloudflare * fixed some bugs * added new db table
-for nav always open or close. * now you can install bigsansar package in to
-ubuntu and all setup with on command lines # How to get Bigsansar Bigsansar is
-available open-source under the [MIT](https://en.wikipedia.org/wiki/
-MIT_License) license. We recommend using the latest version of Python 3.
-Bigsansar is Fully based on django and linux ubuntu. You can use [bigsansar]
-(https://bigsansar.com) for install packaged. You can use [bigsansar](https://
-bigsansar.com) for install packaged. view our tutorials in [youtube](https://
-youtube.com/bigsansar) for playlist: [bigsansar for django](https://
-www.youtube.com/playlist?list=PLbGzLu1WXrFUXw7qr6AMz5_iEkEAPV_Vs) # Get the
-latest development version The latest and greatest Bigsasnar version is the one
-thatâs in our Git repository (our revision-control system). This is only for
-experienced users who want to try incoming changes and help identify bugs
-before an official release. Get it using this shell command, which requires
-[Git](https://https://git-scm.com/): `git clone https://github.com/pokhrelb9/
-bigsansar.git` You can also download a [gzipped tarball](https://https://
-pypi.org/project/Bigsansar/#files) of the development version. This archive is
-updated every time we commit code. # After you install bigsansar 1) Type
-`bigsansar init` command for **automatically** setup server for internal
+## New update * fixed some bug in cloudflare api * Working in to cloudflare *
+fixed some bugs * added new db table for nav always open or close. # How to get
+Bigsansar Bigsansar is available open-source under the [MIT](https://
+en.wikipedia.org/wiki/MIT_License) license. We recommend using the latest
+version of Python 3. Bigsansar is Fully based on django and linux ubuntu. You
+can use [bigsansar](https://bigsansar.com) for install packaged. You can use
+[bigsansar](https://bigsansar.com) for install packaged. view our tutorials in
+[youtube](https://youtube.com/bigsansar) for playlist: [bigsansar for django]
+(https://www.youtube.com/playlist?list=PLbGzLu1WXrFUXw7qr6AMz5_iEkEAPV_Vs) #
+Get the latest development version The latest and greatest Bigsasnar version is
+the one thatâs in our Git repository (our revision-control system). This is
+only for experienced users who want to try incoming changes and help identify
+bugs before an official release. Get it using this shell command, which
+requires [Git](https://https://git-scm.com/): `git clone https://github.com/
+pokhrelb9/bigsansar.git` You can also download a [gzipped tarball](https://
+https://pypi.org/project/Bigsansar/#files) of the development version. This
+archive is updated every time we commit code. # After you install bigsansar 1)
+Type `bigsansar init` command for **automatically** setup server for internal
 configurations. ** this command valid into vertualenv for developer # for full
 setup in to server this is work only on ubuntu os 2) type ` python manage.py
 setup_server` commend for fully setup into server . [How to Setup a Full Server
 with BigSansar, Django, and Ubuntu ](https://youtu.be/j8YN6x9XdR4) # some
 usefull link [sitemap.xml](http://localhost/sitemap.xml) [script.js](http://
 localhost/script.js) [styles.css](http://localhost/styles.css) # how to edit
 sitemap , js and css from pages create a page **slug** name with sitemap,script
```

### Comparing `bigsansar-2.6.0/bigsansar/contrib/account/forms.py` & `bigsansar-2.6.1/bigsansar/contrib/account/forms.py`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.0/bigsansar/contrib/account/migrations/0001_initial.py` & `bigsansar-2.6.1/bigsansar/contrib/account/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.0/bigsansar/contrib/account/models.py` & `bigsansar-2.6.1/bigsansar/contrib/account/models.py`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.0/bigsansar/contrib/advance/forms.py` & `bigsansar-2.6.1/bigsansar/contrib/advance/forms.py`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.0/bigsansar/contrib/advance/migrations/0001_initial.py` & `bigsansar-2.6.1/bigsansar/contrib/advance/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.0/bigsansar/contrib/advance/migrations/0003_javascript.py` & `bigsansar-2.6.1/bigsansar/contrib/advance/migrations/0003_javascript.py`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.0/bigsansar/contrib/advance/migrations/0007_initial.py` & `bigsansar-2.6.1/bigsansar/contrib/advance/migrations/0007_initial.py`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.0/bigsansar/contrib/advance/migrations/0008_sidebarsettings.py` & `bigsansar-2.6.1/bigsansar/contrib/advance/migrations/0008_sidebarsettings.py`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.0/bigsansar/contrib/advance/migrations/0009_sidebarsettings_user.py` & `bigsansar-2.6.1/bigsansar/contrib/advance/migrations/0009_sidebarsettings_user.py`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.0/bigsansar/contrib/advance/migrations/0010_cloudflare_api.py` & `bigsansar-2.6.1/bigsansar/contrib/advance/migrations/0010_cloudflare_api.py`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.0/bigsansar/contrib/advance/migrations/0012_cloudflare_api_ip_address_cloudflare_api_ip_address2.py` & `bigsansar-2.6.1/bigsansar/contrib/advance/migrations/0012_cloudflare_api_ip_address_cloudflare_api_ip_address2.py`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.0/bigsansar/contrib/advance/models.py` & `bigsansar-2.6.1/bigsansar/contrib/advance/models.py`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.0/bigsansar/contrib/advance/templatetags/nav_bar.py` & `bigsansar-2.6.1/bigsansar/contrib/advance/templatetags/nav_bar.py`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.0/bigsansar/contrib/advance/urls.py` & `bigsansar-2.6.1/bigsansar/contrib/advance/urls.py`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.0/bigsansar/contrib/advance/views.py` & `bigsansar-2.6.1/bigsansar/contrib/advance/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -218,15 +218,15 @@
 
                     else:
                         return JsonResponse({'error': 'Failed to retrieve Cloudflare SSL/TLS encryption mode.'}, status=500)
                     
                     ns = response.json()['result']['name_servers']
                     return render(request, 'admin/cloudflare.html', {'cf': query, 'ssl_value': get_ssl_status, 'status': response.json()['result']['status'], 'name_servers1': ns[0], 'name_servers2': ns[1]})
                 else:
-                    return JsonResponse({'error': 'Failed to retrieve Cloudflare nameservers.'}, status=500)
+                    return render(request, 'admin/db_cloudflare.html')
             except:
                 return render(request, 'admin/db_cloudflare.html')
             
         else:
             return render(request, '404.html')
     
     else:
@@ -346,23 +346,25 @@
                                         ]
                             for record in dns_records:
                                 dns_response = requests.post(dns_url, json=record, headers=headers)
                             if dns_response.status_code == 200:
                                 cloudflare_api.objects.update_or_create(defaults={'user': user, 'main_domain_name': zone, 'account_id': account_id, 'ip_address':
                                                                                             ip1, 'ip_address2': ip2})
                                                                                              
+                                
                                 domains.objects.create(user=request.user, domain=zone, Description=zone, zone_id=zone_id)
-                            
+                                
                                 #get_id = domains.objects.get(user=user, domain=zone).id
                                 messages.success(request, 'updated Successfully Created')
                                 return redirect(f'/admin/cf/')
                         
                             else:
-                                messages.warning(request, f"'error': 'Failed to add ip address to the {zone}'")
-                                return render(request, 'admin/cf_config.html', {'head': form_title, 'form': form})
+                                domains.objects.filter(user=user, domain=zone).update(zone_id=zone_id)
+                                messages.success(request, 'updated Successfully Created')
+                                return redirect(f'/admin/cf/')
                             
                         
                         else:
                             messages.warning(request, "'error': 'Failed to fetch data from Cloudflare API Account id or domain already exists'")
                             return render(request, 'admin/cf_config.html', {'head': form_title, 'form': form})
 
                 else:
```

### Comparing `bigsansar-2.6.0/bigsansar/contrib/blogs/admin.py` & `bigsansar-2.6.1/bigsansar/contrib/blogs/admin.py`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.0/bigsansar/contrib/blogs/migrations/0001_initial.py` & `bigsansar-2.6.1/bigsansar/contrib/blogs/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.0/bigsansar/contrib/blogs/models.py` & `bigsansar-2.6.1/bigsansar/contrib/blogs/models.py`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.0/bigsansar/contrib/blogs/templatetags/blogs.py` & `bigsansar-2.6.1/bigsansar/contrib/blogs/templatetags/blogs.py`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.0/bigsansar/contrib/sites/admin.py` & `bigsansar-2.6.1/bigsansar/contrib/sites/admin.py`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.0/bigsansar/contrib/sites/forms.py` & `bigsansar-2.6.1/bigsansar/contrib/sites/forms.py`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.0/bigsansar/contrib/sites/migrations/0001_initial.py` & `bigsansar-2.6.1/bigsansar/contrib/sites/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.0/bigsansar/contrib/sites/migrations/0002_default_domain.py` & `bigsansar-2.6.1/bigsansar/contrib/sites/migrations/0002_default_domain.py`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.0/bigsansar/contrib/sites/migrations/0006_default_domain_default_domain_and_more.py` & `bigsansar-2.6.1/bigsansar/contrib/sites/migrations/0006_default_domain_default_domain_and_more.py`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.0/bigsansar/contrib/sites/models.py` & `bigsansar-2.6.1/bigsansar/contrib/sites/models.py`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.0/bigsansar/contrib/sites/urls.py` & `bigsansar-2.6.1/bigsansar/contrib/sites/urls.py`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.0/bigsansar/contrib/sites/views.py` & `bigsansar-2.6.1/bigsansar/contrib/sites/views.py`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.0/bigsansar/core/__init__.py` & `bigsansar-2.6.1/bigsansar/core/__init__.py`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.0/bigsansar/core/init.py` & `bigsansar-2.6.1/bigsansar/core/init.py`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.0/bigsansar/core/pip_package.py` & `bigsansar-2.6.1/bigsansar/core/pip_package.py`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.0/bigsansar/core/ubuntu.py` & `bigsansar-2.6.1/bigsansar/core/ubuntu.py`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.0/bigsansar/etc/apache2.conf` & `bigsansar-2.6.1/bigsansar/etc/apache2.conf`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.0/bigsansar/etc/config_chroot.sh` & `bigsansar-2.6.1/bigsansar/etc/config_chroot.sh`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.0/bigsansar/etc/db.py` & `bigsansar-2.6.1/bigsansar/etc/db.py`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.0/bigsansar/etc/sshd_config` & `bigsansar-2.6.1/bigsansar/etc/sshd_config`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.0/bigsansar/management/commands/createuser.py` & `bigsansar-2.6.1/bigsansar/management/commands/createuser.py`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.0/bigsansar/management/commands/setup_server.py` & `bigsansar-2.6.1/bigsansar/management/commands/setup_server.py`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/images/icon-hdpi.png` & `bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/images/icon-hdpi.png`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/images/icon.png` & `bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/images/icon.png`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ar.js` & `bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ar.js`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/bg.js` & `bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/bg.js`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/cs.js` & `bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/cs.js`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/de.js` & `bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/de.js`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/el.js` & `bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/el.js`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/en.js` & `bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/en.js`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/es.js` & `bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/es.js`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/et.js` & `bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/et.js`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/eu.js` & `bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/eu.js`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/fi.js` & `bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/fi.js`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/fr.js` & `bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/fr.js`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/he.js` & `bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/he.js`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/hu.js` & `bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/hu.js`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/it.js` & `bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/it.js`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ja.js` & `bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ja.js`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ko.js` & `bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ko.js`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/nb.js` & `bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/nb.js`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/nl.js` & `bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/nl.js`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/nn.js` & `bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/nn.js`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/pl.js` & `bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/pl.js`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/pt-br.js` & `bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/pt-br.js`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/pt.js` & `bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/pt.js`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ru.js` & `bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ru.js`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/sk.js` & `bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/sk.js`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/tr.js` & `bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/tr.js`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/uk.js` & `bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/uk.js`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/vi.js` & `bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/vi.js`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/zh.js` & `bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/zh.js`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.0/bigsansar/static/ckeditor/ckeditor/plugins/youtube/plugin.js` & `bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/plugin.js`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.0/bigsansar/static/logo.png` & `bigsansar-2.6.1/bigsansar/static/logo.png`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.0/bigsansar/static/style.css` & `bigsansar-2.6.1/bigsansar/static/style.css`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.0/bigsansar/templates/404.html` & `bigsansar-2.6.1/bigsansar/templates/404.html`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.0/bigsansar/templates/admin/account_info.html` & `bigsansar-2.6.1/bigsansar/templates/admin/account_info.html`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.0/bigsansar/templates/admin/admin_update.html` & `bigsansar-2.6.1/bigsansar/templates/admin/admin_update.html`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.0/bigsansar/templates/admin/cf_config.html` & `bigsansar-2.6.1/bigsansar/templates/admin/cf_config.html`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.0/bigsansar/templates/admin/chpass.html` & `bigsansar-2.6.1/bigsansar/templates/admin/chpass.html`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.0/bigsansar/templates/admin/chuname.html` & `bigsansar-2.6.1/bigsansar/templates/admin/chuname.html`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.0/bigsansar/templates/admin/cloudflare.html` & `bigsansar-2.6.1/bigsansar/templates/admin/cloudflare.html`

 * *Files 6% similar despite different names*

```diff
@@ -22,14 +22,25 @@
 </style>
 </head>
 <body>
     
    
 
 <div id="info-box" class="info-box">
+    {% if messages %}
+		{% for message in messages %}
+		{% if message.tags %}
+		<div class="alert alert-{{ message.tags }} alert-dismissible fade show" role="alert">
+			{{ message }}
+			<button type="button" class="btn-close" data-bs-dismiss="alert" aria-label="Close">
+			</button>
+		</div>
+		{% endif %}
+		{% endfor %}
+		{% endif %}
     {% if status == 'pending' %}
     <div class="card">
         <div class="card-header">
             {{ cf.main_domain_name }} is not active on Cloudflare yet
         </div>
         <div class="card-body">
             <p class="card-text">
@@ -38,15 +49,15 @@
             <li>{{ name_servers1 }}</li>
             <li>{{ name_servers2 }}</li>
         </ul>
             </p>
         </div>
     </div>
     {% else %}
-    {% endif %}
+    
     
     {% if ssl_value == 'strict' %}
     <svg xmlns="http://www.w3.org/2000/svg" class="d-none">
         <symbol id="check-circle-fill" viewBox="0 0 16 16">
           <path d="M16 8A8 8 0 1 1 0 8a8 8 0 0 1 16 0zm-3.97-3.03a.75.75 0 0 0-1.08.022L7.477 9.417 5.384 7.323a.75.75 0 0 0-1.06 1.06L6.97 11.03a.75.75 0 0 0 1.079-.02l3.992-4.99a.75.75 0 0 0-.01-1.05z"/>
         </symbol>
         <symbol id="info-fill" viewBox="0 0 16 16">
@@ -68,14 +79,15 @@
           <path d="M8.982 1.566a1.13 1.13 0 0 0-1.96 0L.165 13.233c-.457.778.091 1.767.98 1.767h13.713c.889 0 1.438-.99.98-1.767L8.982 1.566zM8 5c.535 0 .954.462.9.995l-.35 3.507a.552.552 0 0 1-1.1 0L7.1 5.995A.905.905 0 0 1 8 5zm.002 6a1 1 0 1 1 0 2 1 1 0 0 1 0-2z"/>
         </svg>
         <div>
     Encrypts end-to-end, but requires a trusted CA or Cloudflare Origin CA certificate on the server. <a href="/admin/cf/ssl_origin">Setup</a> encryption of traffic between your origin server and Cloudflare.
         </div>
     </div>
     {% endif %}
+    {% endif %}
    
     <br/>
     <br/>
     <div class="row">
         <div class="col-sm-3">
             <h6 class="mb-0">Email</h6>
         </div>
```

#### html2text {}

```diff
@@ -1,22 +1,24 @@
 {% extends 'base.html' %} {%block title %} bigsansar - Cloudflare configrations
 {% endblock %} {% block head %} {% load static %}
 {% endblock %} {% block body %} {% include 'admin/nav.html' %}
-{% if status == 'pending' %}
+{% if messages %} {% for message in messages %} {% if message.tags %}
+{{ message }}
+{% endif %} {% endfor %} {% endif %} {% if status == 'pending' %}
 {{ cf.main_domain_name }} is not active on Cloudflare yet
 Your assigned Cloudflare nameservers:
     * {{ name_servers1 }}
     * {{ name_servers2 }}
-{% else %} {% endif %} {% if ssl_value == 'strict' %}
+{% else %} {% if ssl_value == 'strict' %}
 Your SSL/TLS encryption mode is Full (strict)
 {% else %}
 Encrypts end-to-end, but requires a trusted CA or Cloudflare Origin CA
 certificate on the server. _S_e_t_u_p encryption of traffic between your origin
 server and Cloudflare.
-{% endif %}
+{% endif %} {% endif %}
 
 ** EEmmaaiill **
 {{ cf.email }}
 ===============================================================================
 ** DDoommaaiinn **
 {{ cf.main_domain_name }}
 ===============================================================================
```

### Comparing `bigsansar-2.6.0/bigsansar/templates/admin/create_domain.html` & `bigsansar-2.6.1/bigsansar/templates/admin/create_domain.html`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.0/bigsansar/templates/admin/db_cloudflare.html` & `bigsansar-2.6.1/bigsansar/templates/admin/db_cloudflare.html`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.0/bigsansar/templates/admin/domain_manage.html` & `bigsansar-2.6.1/bigsansar/templates/admin/domain_manage.html`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.0/bigsansar/templates/admin/edit_domain.html` & `bigsansar-2.6.1/bigsansar/templates/admin/edit_domain.html`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.0/bigsansar/templates/admin/editprofile.html` & `bigsansar-2.6.1/bigsansar/templates/admin/editprofile.html`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.0/bigsansar/templates/admin/login.html` & `bigsansar-2.6.1/bigsansar/templates/admin/login.html`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.0/bigsansar/templates/admin/nav.html` & `bigsansar-2.6.1/bigsansar/templates/admin/nav.html`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.0/bigsansar/templates/admin/page_create.html` & `bigsansar-2.6.1/bigsansar/templates/admin/page_create.html`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.0/bigsansar/templates/admin/page_delete.html` & `bigsansar-2.6.1/bigsansar/templates/admin/page_delete.html`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.0/bigsansar/templates/admin/page_edit.html` & `bigsansar-2.6.1/bigsansar/templates/admin/page_edit.html`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.0/bigsansar/templates/base.html` & `bigsansar-2.6.1/bigsansar/templates/base.html`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.0/bigsansar/templates/blog_preview.html` & `bigsansar-2.6.1/bigsansar/templates/blog_preview.html`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.0/bigsansar/templates/default.html` & `bigsansar-2.6.1/bigsansar/templates/default.html`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.0/bigsansar/templates/defaultpage.html` & `bigsansar-2.6.1/bigsansar/templates/defaultpage.html`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.0/bigsansar/templates/parking.html` & `bigsansar-2.6.1/bigsansar/templates/parking.html`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.0/bigsansar/urls.py` & `bigsansar-2.6.1/bigsansar/urls.py`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.0/bigsansar/views.py` & `bigsansar-2.6.1/bigsansar/views.py`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.0/setup.py` & `bigsansar-2.6.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="Bigsansar",
-    version="2.6.0",
+    version="2.6.1",
     author="Bikash Pokhrel",
     author_email="bigsansaroffice@gmail.com",
     description="Build one in minutes with bigsansar - a visual site building tool!",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/pokhrelb9/bigsansar",
     project_urls={
```

