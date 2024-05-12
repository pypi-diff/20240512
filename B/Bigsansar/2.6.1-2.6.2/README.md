# Comparing `tmp/bigsansar-2.6.1.tar.gz` & `tmp/bigsansar-2.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bigsansar-2.6.1.tar", last modified: Sun May 12 03:47:04 2024, max compression
+gzip compressed data, was "bigsansar-2.6.2.tar", last modified: Sun May 12 03:57:47 2024, max compression
```

## Comparing `bigsansar-2.6.1.tar` & `bigsansar-2.6.2.tar`

### file list

```diff
@@ -1,197 +1,197 @@
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 03:47:04.452508 bigsansar-2.6.1/
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 03:47:04.452508 bigsansar-2.6.1/Bigsansar.egg-info/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     5310 2024-05-12 03:47:04.000000 bigsansar-2.6.1/Bigsansar.egg-info/PKG-INFO
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     7368 2024-05-12 03:47:04.000000 bigsansar-2.6.1/Bigsansar.egg-info/SOURCES.txt
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        1 2024-05-12 03:47:04.000000 bigsansar-2.6.1/Bigsansar.egg-info/dependency_links.txt
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)       50 2024-05-12 03:47:04.000000 bigsansar-2.6.1/Bigsansar.egg-info/entry_points.txt
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)       98 2024-05-12 03:47:04.000000 bigsansar-2.6.1/Bigsansar.egg-info/requires.txt
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)       10 2024-05-12 03:47:04.000000 bigsansar-2.6.1/Bigsansar.egg-info/top_level.txt
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1073 2024-04-10 03:12:24.000000 bigsansar-2.6.1/LICENSE
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     5310 2024-05-12 03:47:04.452508 bigsansar-2.6.1/PKG-INFO
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     4385 2024-05-12 03:45:06.000000 bigsansar-2.6.1/README.md
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 03:47:04.282508 bigsansar-2.6.1/bigsansar/
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/__init__.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)       63 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/admin.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      188 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/apps.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 03:47:04.282508 bigsansar-2.6.1/bigsansar/contrib/
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/contrib/__init__.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 03:47:04.292508 bigsansar-2.6.1/bigsansar/contrib/account/
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/contrib/account/__init__.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      489 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/contrib/account/admin.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      275 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/contrib/account/apps.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1155 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/contrib/account/forms.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 03:47:04.292508 bigsansar-2.6.1/bigsansar/contrib/account/migrations/
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      969 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/contrib/account/migrations/0001_initial.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      400 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/contrib/account/migrations/0002_alter_userinfo_options.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/contrib/account/migrations/__init__.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      539 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/contrib/account/models.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      340 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/contrib/account/signals.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 03:47:04.292508 bigsansar-2.6.1/bigsansar/contrib/account/templates/
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/contrib/account/templates/__init__.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)       60 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/contrib/account/tests.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/contrib/account/urls.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/contrib/account/views.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 03:47:04.302508 bigsansar-2.6.1/bigsansar/contrib/advance/
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/contrib/advance/__init__.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      165 2024-05-12 03:46:34.000000 bigsansar-2.6.1/bigsansar/contrib/advance/admin.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      202 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/contrib/advance/apps.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      357 2024-05-11 07:59:27.000000 bigsansar-2.6.1/bigsansar/contrib/advance/cf_url.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     4583 2024-04-16 12:22:05.000000 bigsansar-2.6.1/bigsansar/contrib/advance/forms.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 03:47:04.312508 bigsansar-2.6.1/bigsansar/contrib/advance/migrations/
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1000 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/contrib/advance/migrations/0001_initial.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      367 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/contrib/advance/migrations/0002_alter_css_options.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1050 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/contrib/advance/migrations/0003_javascript.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      386 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/contrib/advance/migrations/0004_alter_javascript_options.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      296 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/contrib/advance/migrations/0005_delete_css.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      289 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/contrib/advance/migrations/0006_delete_javascript.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1075 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/contrib/advance/migrations/0007_initial.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      527 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/contrib/advance/migrations/0008_sidebarsettings.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      631 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/contrib/advance/migrations/0009_sidebarsettings_user.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1000 2024-04-10 05:16:13.000000 bigsansar-2.6.1/bigsansar/contrib/advance/migrations/0010_cloudflare_api.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      391 2024-04-13 11:41:57.000000 bigsansar-2.6.1/bigsansar/contrib/advance/migrations/0011_rename_account_global_api_key_cloudflare_api_global_api_key.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      637 2024-04-16 11:46:02.000000 bigsansar-2.6.1/bigsansar/contrib/advance/migrations/0012_cloudflare_api_ip_address_cloudflare_api_ip_address2.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/contrib/advance/migrations/__init__.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1356 2024-04-16 11:46:06.000000 bigsansar-2.6.1/bigsansar/contrib/advance/models.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 03:47:04.312508 bigsansar-2.6.1/bigsansar/contrib/advance/templatetags/
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/contrib/advance/templatetags/__init__.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1797 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/contrib/advance/templatetags/nav_bar.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)       60 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/contrib/advance/tests.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      721 2024-04-16 11:03:13.000000 bigsansar-2.6.1/bigsansar/contrib/advance/urls.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)    20765 2024-05-12 03:40:41.000000 bigsansar-2.6.1/bigsansar/contrib/advance/views.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 03:47:04.332508 bigsansar-2.6.1/bigsansar/contrib/blogs/
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/contrib/blogs/__init__.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     2238 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/contrib/blogs/admin.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      188 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/contrib/blogs/apps.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      261 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/contrib/blogs/forms.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 03:47:04.332508 bigsansar-2.6.1/bigsansar/contrib/blogs/migrations/
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     2261 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/contrib/blogs/migrations/0001_initial.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      367 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/contrib/blogs/migrations/0002_post_visitor.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/contrib/blogs/migrations/__init__.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     2028 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/contrib/blogs/models.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 03:47:04.332508 bigsansar-2.6.1/bigsansar/contrib/blogs/templatetags/
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/contrib/blogs/templatetags/__init__.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1478 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/contrib/blogs/templatetags/blogs.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)       60 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/contrib/blogs/tests.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)       63 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/contrib/blogs/views.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 03:47:04.352508 bigsansar-2.6.1/bigsansar/contrib/sites/
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/contrib/sites/__init__.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1719 2024-05-11 15:54:05.000000 bigsansar-2.6.1/bigsansar/contrib/sites/admin.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      196 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/contrib/sites/apps.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     4435 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/contrib/sites/forms.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 03:47:04.372508 bigsansar-2.6.1/bigsansar/contrib/sites/migrations/
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1847 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/contrib/sites/migrations/0001_initial.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      819 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/contrib/sites/migrations/0002_default_domain.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      385 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/contrib/sites/migrations/0003_domains_default.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      386 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/contrib/sites/migrations/0004_alter_domains_default.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      331 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/contrib/sites/migrations/0005_remove_domains_default.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      653 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/contrib/sites/migrations/0006_default_domain_default_domain_and_more.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      410 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/contrib/sites/migrations/0007_alter_default_domain_default_domain.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      411 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/contrib/sites/migrations/0008_domains_primary_domain.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      346 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/contrib/sites/migrations/0009_remove_default_domain_default_domain.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      422 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/contrib/sites/migrations/0010_alter_domains_description.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      405 2024-05-09 10:32:01.000000 bigsansar-2.6.1/bigsansar/contrib/sites/migrations/0011_domains_zone_id.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/contrib/sites/migrations/__init__.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     2453 2024-05-09 10:31:51.000000 bigsansar-2.6.1/bigsansar/contrib/sites/models.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 03:47:04.372508 bigsansar-2.6.1/bigsansar/contrib/sites/templatetags/
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/contrib/sites/templatetags/__init__.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      394 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/contrib/sites/templatetags/pages.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)       60 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/contrib/sites/tests.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      547 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/contrib/sites/urls.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     9258 2024-04-10 10:36:13.000000 bigsansar-2.6.1/bigsansar/contrib/sites/views.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/contrib/urls.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/contrib/views.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 03:47:04.372508 bigsansar-2.6.1/bigsansar/core/
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1018 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/core/__init__.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      402 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/core/host.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     9710 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/core/init.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      640 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/core/pip_package.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)    16740 2024-05-11 16:16:09.000000 bigsansar-2.6.1/bigsansar/core/ubuntu.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 03:47:04.372508 bigsansar-2.6.1/bigsansar/etc/
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     7287 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/etc/apache2.conf
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1638 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/etc/config_chroot.sh
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     5123 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/etc/db.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     3236 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/etc/sshd_config
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 03:47:04.372508 bigsansar-2.6.1/bigsansar/management/
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/management/__init__.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 03:47:04.372508 bigsansar-2.6.1/bigsansar/management/commands/
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/management/commands/__init__.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1076 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/management/commands/createuser.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1023 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/management/commands/setup_server.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 03:47:04.392508 bigsansar-2.6.1/bigsansar/migrations/
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/migrations/__init__.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)       57 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/models.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 03:47:04.392508 bigsansar-2.6.1/bigsansar/static/
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/static/__init__.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 03:47:04.262508 bigsansar-2.6.1/bigsansar/static/ckeditor/
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 03:47:04.262508 bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 03:47:04.262508 bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 03:47:04.392508 bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 03:47:04.392508 bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/images/
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1258 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/images/icon-hdpi.png
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1165 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/images/icon.png
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 03:47:04.412508 bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1337 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ar.js
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1654 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/bg.js
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1184 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/cs.js
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1078 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/de.js
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1514 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/el.js
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1024 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/en.js
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1084 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/es.js
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1079 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/et.js
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1161 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/eu.js
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      960 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/fi.js
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1051 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/fr.js
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1226 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/he.js
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1166 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/hu.js
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1081 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/it.js
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1171 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ja.js
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1229 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ko.js
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1035 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/nb.js
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1022 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/nl.js
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1040 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/nn.js
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1120 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/pl.js
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1151 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/pt-br.js
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1153 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/pt.js
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1539 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ru.js
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1173 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/sk.js
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1206 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/tr.js
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1538 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/uk.js
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1067 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/vi.js
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      916 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/zh.js
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)    13371 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/plugin.js
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     9230 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/static/logo.png
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      551 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/static/style.css
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 03:47:04.422508 bigsansar-2.6.1/bigsansar/templates/
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      947 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/templates/404.html
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/templates/__init__.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      164 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/templates/acc_active_email.html
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 03:47:04.452508 bigsansar-2.6.1/bigsansar/templates/admin/
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)    10272 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/templates/admin/account_info.html
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      519 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/templates/admin/admin_update.html
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      878 2024-04-13 11:47:55.000000 bigsansar-2.6.1/bigsansar/templates/admin/cf_config.html
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      558 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/templates/admin/chpass.html
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      558 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/templates/admin/chuname.html
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     4745 2024-05-12 03:43:14.000000 bigsansar-2.6.1/bigsansar/templates/admin/cloudflare.html
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      549 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/templates/admin/create_domain.html
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1637 2024-05-11 15:51:11.000000 bigsansar-2.6.1/bigsansar/templates/admin/db_cloudflare.html
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     8866 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/templates/admin/domain_manage.html
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1019 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/templates/admin/edit_domain.html
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      566 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/templates/admin/editprofile.html
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      979 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/templates/admin/login.html
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     6004 2024-04-16 11:03:44.000000 bigsansar-2.6.1/bigsansar/templates/admin/nav.html
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      947 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/templates/admin/page_create.html
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      948 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/templates/admin/page_delete.html
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      717 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/templates/admin/page_edit.html
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1622 2024-05-11 07:51:33.000000 bigsansar-2.6.1/bigsansar/templates/base.html
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1898 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/templates/blog_preview.html
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     2197 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/templates/default.html
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     2200 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/templates/defaultpage.html
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      719 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/templates/parking.html
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      101 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/templates/script.html
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      411 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/templates/sitemap.html
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      101 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/templates/styles.html
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)       60 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/tests.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1209 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/urls.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     4595 2024-04-10 03:12:24.000000 bigsansar-2.6.1/bigsansar/views.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       38 2024-05-12 03:47:04.452508 bigsansar-2.6.1/setup.cfg
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1914 2024-05-12 03:44:39.000000 bigsansar-2.6.1/setup.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 03:57:47.602518 bigsansar-2.6.2/
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 03:57:47.592518 bigsansar-2.6.2/Bigsansar.egg-info/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     5310 2024-05-12 03:57:47.000000 bigsansar-2.6.2/Bigsansar.egg-info/PKG-INFO
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     7368 2024-05-12 03:57:47.000000 bigsansar-2.6.2/Bigsansar.egg-info/SOURCES.txt
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        1 2024-05-12 03:57:47.000000 bigsansar-2.6.2/Bigsansar.egg-info/dependency_links.txt
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)       50 2024-05-12 03:57:47.000000 bigsansar-2.6.2/Bigsansar.egg-info/entry_points.txt
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)       98 2024-05-12 03:57:47.000000 bigsansar-2.6.2/Bigsansar.egg-info/requires.txt
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)       10 2024-05-12 03:57:47.000000 bigsansar-2.6.2/Bigsansar.egg-info/top_level.txt
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1073 2024-04-10 03:12:24.000000 bigsansar-2.6.2/LICENSE
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     5310 2024-05-12 03:57:47.602518 bigsansar-2.6.2/PKG-INFO
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     4385 2024-05-12 03:45:06.000000 bigsansar-2.6.2/README.md
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 03:57:47.512519 bigsansar-2.6.2/bigsansar/
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/__init__.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)       63 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/admin.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      188 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/apps.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 03:57:47.512519 bigsansar-2.6.2/bigsansar/contrib/
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/contrib/__init__.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 03:57:47.522518 bigsansar-2.6.2/bigsansar/contrib/account/
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/contrib/account/__init__.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      489 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/contrib/account/admin.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      275 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/contrib/account/apps.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1155 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/contrib/account/forms.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 03:57:47.522518 bigsansar-2.6.2/bigsansar/contrib/account/migrations/
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      969 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/contrib/account/migrations/0001_initial.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      400 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/contrib/account/migrations/0002_alter_userinfo_options.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/contrib/account/migrations/__init__.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      539 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/contrib/account/models.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      340 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/contrib/account/signals.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 03:57:47.522518 bigsansar-2.6.2/bigsansar/contrib/account/templates/
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/contrib/account/templates/__init__.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)       60 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/contrib/account/tests.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/contrib/account/urls.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/contrib/account/views.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 03:57:47.522518 bigsansar-2.6.2/bigsansar/contrib/advance/
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/contrib/advance/__init__.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      165 2024-05-12 03:46:34.000000 bigsansar-2.6.2/bigsansar/contrib/advance/admin.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      202 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/contrib/advance/apps.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      357 2024-05-11 07:59:27.000000 bigsansar-2.6.2/bigsansar/contrib/advance/cf_url.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     4583 2024-04-16 12:22:05.000000 bigsansar-2.6.2/bigsansar/contrib/advance/forms.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 03:57:47.542518 bigsansar-2.6.2/bigsansar/contrib/advance/migrations/
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1000 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/contrib/advance/migrations/0001_initial.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      367 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/contrib/advance/migrations/0002_alter_css_options.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1050 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/contrib/advance/migrations/0003_javascript.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      386 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/contrib/advance/migrations/0004_alter_javascript_options.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      296 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/contrib/advance/migrations/0005_delete_css.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      289 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/contrib/advance/migrations/0006_delete_javascript.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1075 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/contrib/advance/migrations/0007_initial.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      527 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/contrib/advance/migrations/0008_sidebarsettings.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      631 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/contrib/advance/migrations/0009_sidebarsettings_user.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1000 2024-04-10 05:16:13.000000 bigsansar-2.6.2/bigsansar/contrib/advance/migrations/0010_cloudflare_api.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      391 2024-04-13 11:41:57.000000 bigsansar-2.6.2/bigsansar/contrib/advance/migrations/0011_rename_account_global_api_key_cloudflare_api_global_api_key.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      637 2024-04-16 11:46:02.000000 bigsansar-2.6.2/bigsansar/contrib/advance/migrations/0012_cloudflare_api_ip_address_cloudflare_api_ip_address2.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/contrib/advance/migrations/__init__.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1356 2024-04-16 11:46:06.000000 bigsansar-2.6.2/bigsansar/contrib/advance/models.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 03:57:47.542518 bigsansar-2.6.2/bigsansar/contrib/advance/templatetags/
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/contrib/advance/templatetags/__init__.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1797 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/contrib/advance/templatetags/nav_bar.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)       60 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/contrib/advance/tests.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      721 2024-04-16 11:03:13.000000 bigsansar-2.6.2/bigsansar/contrib/advance/urls.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)    21045 2024-05-12 03:57:26.000000 bigsansar-2.6.2/bigsansar/contrib/advance/views.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 03:57:47.542518 bigsansar-2.6.2/bigsansar/contrib/blogs/
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/contrib/blogs/__init__.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     2238 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/contrib/blogs/admin.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      188 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/contrib/blogs/apps.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      261 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/contrib/blogs/forms.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 03:57:47.542518 bigsansar-2.6.2/bigsansar/contrib/blogs/migrations/
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     2261 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/contrib/blogs/migrations/0001_initial.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      367 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/contrib/blogs/migrations/0002_post_visitor.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/contrib/blogs/migrations/__init__.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     2028 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/contrib/blogs/models.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 03:57:47.542518 bigsansar-2.6.2/bigsansar/contrib/blogs/templatetags/
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/contrib/blogs/templatetags/__init__.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1478 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/contrib/blogs/templatetags/blogs.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)       60 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/contrib/blogs/tests.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)       63 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/contrib/blogs/views.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 03:57:47.542518 bigsansar-2.6.2/bigsansar/contrib/sites/
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/contrib/sites/__init__.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1719 2024-05-11 15:54:05.000000 bigsansar-2.6.2/bigsansar/contrib/sites/admin.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      196 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/contrib/sites/apps.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     4435 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/contrib/sites/forms.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 03:57:47.552518 bigsansar-2.6.2/bigsansar/contrib/sites/migrations/
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1847 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/contrib/sites/migrations/0001_initial.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      819 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/contrib/sites/migrations/0002_default_domain.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      385 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/contrib/sites/migrations/0003_domains_default.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      386 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/contrib/sites/migrations/0004_alter_domains_default.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      331 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/contrib/sites/migrations/0005_remove_domains_default.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      653 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/contrib/sites/migrations/0006_default_domain_default_domain_and_more.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      410 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/contrib/sites/migrations/0007_alter_default_domain_default_domain.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      411 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/contrib/sites/migrations/0008_domains_primary_domain.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      346 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/contrib/sites/migrations/0009_remove_default_domain_default_domain.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      422 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/contrib/sites/migrations/0010_alter_domains_description.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      405 2024-05-09 10:32:01.000000 bigsansar-2.6.2/bigsansar/contrib/sites/migrations/0011_domains_zone_id.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/contrib/sites/migrations/__init__.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     2453 2024-05-09 10:31:51.000000 bigsansar-2.6.2/bigsansar/contrib/sites/models.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 03:57:47.552518 bigsansar-2.6.2/bigsansar/contrib/sites/templatetags/
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/contrib/sites/templatetags/__init__.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      394 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/contrib/sites/templatetags/pages.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)       60 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/contrib/sites/tests.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      547 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/contrib/sites/urls.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     9258 2024-04-10 10:36:13.000000 bigsansar-2.6.2/bigsansar/contrib/sites/views.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/contrib/urls.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/contrib/views.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 03:57:47.562518 bigsansar-2.6.2/bigsansar/core/
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1018 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/core/__init__.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      402 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/core/host.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     9710 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/core/init.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      640 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/core/pip_package.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)    16740 2024-05-11 16:16:09.000000 bigsansar-2.6.2/bigsansar/core/ubuntu.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 03:57:47.562518 bigsansar-2.6.2/bigsansar/etc/
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     7287 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/etc/apache2.conf
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1638 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/etc/config_chroot.sh
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     5123 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/etc/db.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     3236 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/etc/sshd_config
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 03:57:47.562518 bigsansar-2.6.2/bigsansar/management/
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/management/__init__.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 03:57:47.562518 bigsansar-2.6.2/bigsansar/management/commands/
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/management/commands/__init__.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1076 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/management/commands/createuser.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1023 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/management/commands/setup_server.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 03:57:47.562518 bigsansar-2.6.2/bigsansar/migrations/
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/migrations/__init__.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)       57 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/models.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 03:57:47.562518 bigsansar-2.6.2/bigsansar/static/
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/static/__init__.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 03:57:47.492519 bigsansar-2.6.2/bigsansar/static/ckeditor/
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 03:57:47.492519 bigsansar-2.6.2/bigsansar/static/ckeditor/ckeditor/
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 03:57:47.492519 bigsansar-2.6.2/bigsansar/static/ckeditor/ckeditor/plugins/
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 03:57:47.562518 bigsansar-2.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 03:57:47.572518 bigsansar-2.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/images/
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1258 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/images/icon-hdpi.png
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1165 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/images/icon.png
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 03:57:47.592518 bigsansar-2.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1337 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ar.js
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1654 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/bg.js
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1184 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/cs.js
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1078 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/de.js
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1514 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/el.js
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1024 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/en.js
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1084 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/es.js
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1079 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/et.js
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1161 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/eu.js
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      960 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/fi.js
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1051 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/fr.js
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1226 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/he.js
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1166 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/hu.js
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1081 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/it.js
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1171 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ja.js
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1229 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ko.js
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1035 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/nb.js
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1022 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/nl.js
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1040 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/nn.js
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1120 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/pl.js
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1151 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/pt-br.js
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1153 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/pt.js
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1539 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ru.js
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1173 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/sk.js
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1206 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/tr.js
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1538 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/uk.js
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1067 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/vi.js
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      916 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/zh.js
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)    13371 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/plugin.js
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     9230 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/static/logo.png
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      551 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/static/style.css
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 03:57:47.592518 bigsansar-2.6.2/bigsansar/templates/
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      947 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/templates/404.html
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/templates/__init__.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      164 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/templates/acc_active_email.html
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 03:57:47.592518 bigsansar-2.6.2/bigsansar/templates/admin/
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)    10272 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/templates/admin/account_info.html
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      519 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/templates/admin/admin_update.html
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      878 2024-04-13 11:47:55.000000 bigsansar-2.6.2/bigsansar/templates/admin/cf_config.html
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      558 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/templates/admin/chpass.html
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      558 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/templates/admin/chuname.html
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     4745 2024-05-12 03:57:06.000000 bigsansar-2.6.2/bigsansar/templates/admin/cloudflare.html
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      549 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/templates/admin/create_domain.html
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1637 2024-05-11 15:51:11.000000 bigsansar-2.6.2/bigsansar/templates/admin/db_cloudflare.html
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     8866 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/templates/admin/domain_manage.html
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1019 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/templates/admin/edit_domain.html
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      566 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/templates/admin/editprofile.html
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      979 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/templates/admin/login.html
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     6004 2024-04-16 11:03:44.000000 bigsansar-2.6.2/bigsansar/templates/admin/nav.html
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      947 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/templates/admin/page_create.html
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      948 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/templates/admin/page_delete.html
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      717 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/templates/admin/page_edit.html
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1622 2024-05-11 07:51:33.000000 bigsansar-2.6.2/bigsansar/templates/base.html
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1898 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/templates/blog_preview.html
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     2197 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/templates/default.html
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     2200 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/templates/defaultpage.html
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      719 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/templates/parking.html
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      101 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/templates/script.html
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      411 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/templates/sitemap.html
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      101 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/templates/styles.html
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)       60 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/tests.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1209 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/urls.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     4595 2024-04-10 03:12:24.000000 bigsansar-2.6.2/bigsansar/views.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       38 2024-05-12 03:57:47.602518 bigsansar-2.6.2/setup.cfg
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1914 2024-05-12 03:57:33.000000 bigsansar-2.6.2/setup.py
```

### Comparing `bigsansar-2.6.1/Bigsansar.egg-info/PKG-INFO` & `bigsansar-2.6.2/Bigsansar.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Bigsansar
-Version: 2.6.1
+Version: 2.6.2
 Summary: Build one in minutes with bigsansar - a visual site building tool!
 Home-page: https://github.com/pokhrelb9/bigsansar
 Author: Bikash Pokhrel
 Author-email: bigsansaroffice@gmail.com
 Project-URL: Bug Tracker, https://github.com/pokhrelb9/bigsansar/issues
 Project-URL: Documentations, https://docs.bigsansar.com/
 Keywords: python,django host,bigsansar,django,django sites framework,django flatpages
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Bigsansar Version: 2.6.1 Summary: Build one in
+Metadata-Version: 2.1 Name: Bigsansar Version: 2.6.2 Summary: Build one in
 minutes with bigsansar - a visual site building tool! Home-page: https://
 github.com/pokhrelb9/bigsansar Author: Bikash Pokhrel Author-email:
 bigsansaroffice@gmail.com Project-URL: Bug Tracker, https://github.com/
 pokhrelb9/bigsansar/issues Project-URL: Documentations, https://
 docs.bigsansar.com/ Keywords: python,django host,bigsansar,django,django sites
 framework,django flatpages Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
```

### Comparing `bigsansar-2.6.1/Bigsansar.egg-info/SOURCES.txt` & `bigsansar-2.6.2/Bigsansar.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.1/LICENSE` & `bigsansar-2.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.1/PKG-INFO` & `bigsansar-2.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Bigsansar
-Version: 2.6.1
+Version: 2.6.2
 Summary: Build one in minutes with bigsansar - a visual site building tool!
 Home-page: https://github.com/pokhrelb9/bigsansar
 Author: Bikash Pokhrel
 Author-email: bigsansaroffice@gmail.com
 Project-URL: Bug Tracker, https://github.com/pokhrelb9/bigsansar/issues
 Project-URL: Documentations, https://docs.bigsansar.com/
 Keywords: python,django host,bigsansar,django,django sites framework,django flatpages
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Bigsansar Version: 2.6.1 Summary: Build one in
+Metadata-Version: 2.1 Name: Bigsansar Version: 2.6.2 Summary: Build one in
 minutes with bigsansar - a visual site building tool! Home-page: https://
 github.com/pokhrelb9/bigsansar Author: Bikash Pokhrel Author-email:
 bigsansaroffice@gmail.com Project-URL: Bug Tracker, https://github.com/
 pokhrelb9/bigsansar/issues Project-URL: Documentations, https://
 docs.bigsansar.com/ Keywords: python,django host,bigsansar,django,django sites
 framework,django flatpages Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
```

### Comparing `bigsansar-2.6.1/README.md` & `bigsansar-2.6.2/README.md`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.1/bigsansar/contrib/account/forms.py` & `bigsansar-2.6.2/bigsansar/contrib/account/forms.py`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.1/bigsansar/contrib/account/migrations/0001_initial.py` & `bigsansar-2.6.2/bigsansar/contrib/account/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.1/bigsansar/contrib/account/models.py` & `bigsansar-2.6.2/bigsansar/contrib/account/models.py`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.1/bigsansar/contrib/advance/forms.py` & `bigsansar-2.6.2/bigsansar/contrib/advance/forms.py`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.1/bigsansar/contrib/advance/migrations/0001_initial.py` & `bigsansar-2.6.2/bigsansar/contrib/advance/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.1/bigsansar/contrib/advance/migrations/0003_javascript.py` & `bigsansar-2.6.2/bigsansar/contrib/advance/migrations/0003_javascript.py`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.1/bigsansar/contrib/advance/migrations/0007_initial.py` & `bigsansar-2.6.2/bigsansar/contrib/advance/migrations/0007_initial.py`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.1/bigsansar/contrib/advance/migrations/0008_sidebarsettings.py` & `bigsansar-2.6.2/bigsansar/contrib/advance/migrations/0008_sidebarsettings.py`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.1/bigsansar/contrib/advance/migrations/0009_sidebarsettings_user.py` & `bigsansar-2.6.2/bigsansar/contrib/advance/migrations/0009_sidebarsettings_user.py`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.1/bigsansar/contrib/advance/migrations/0010_cloudflare_api.py` & `bigsansar-2.6.2/bigsansar/contrib/advance/migrations/0010_cloudflare_api.py`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.1/bigsansar/contrib/advance/migrations/0012_cloudflare_api_ip_address_cloudflare_api_ip_address2.py` & `bigsansar-2.6.2/bigsansar/contrib/advance/migrations/0012_cloudflare_api_ip_address_cloudflare_api_ip_address2.py`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.1/bigsansar/contrib/advance/models.py` & `bigsansar-2.6.2/bigsansar/contrib/advance/models.py`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.1/bigsansar/contrib/advance/templatetags/nav_bar.py` & `bigsansar-2.6.2/bigsansar/contrib/advance/templatetags/nav_bar.py`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.1/bigsansar/contrib/advance/urls.py` & `bigsansar-2.6.2/bigsansar/contrib/advance/urls.py`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.1/bigsansar/contrib/advance/views.py` & `bigsansar-2.6.2/bigsansar/contrib/advance/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -354,14 +354,16 @@
                                 domains.objects.create(user=request.user, domain=zone, Description=zone, zone_id=zone_id)
                                 
                                 #get_id = domains.objects.get(user=user, domain=zone).id
                                 messages.success(request, 'updated Successfully Created')
                                 return redirect(f'/admin/cf/')
                         
                             else:
+                                cloudflare_api.objects.update_or_create(defaults={'user': user, 'main_domain_name': zone, 'account_id': account_id, 'ip_address':
+                                                                                            ip1, 'ip_address2': ip2})
                                 domains.objects.filter(user=user, domain=zone).update(zone_id=zone_id)
                                 messages.success(request, 'updated Successfully Created')
                                 return redirect(f'/admin/cf/')
                             
                         
                         else:
                             messages.warning(request, "'error': 'Failed to fetch data from Cloudflare API Account id or domain already exists'")
```

### Comparing `bigsansar-2.6.1/bigsansar/contrib/blogs/admin.py` & `bigsansar-2.6.2/bigsansar/contrib/blogs/admin.py`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.1/bigsansar/contrib/blogs/migrations/0001_initial.py` & `bigsansar-2.6.2/bigsansar/contrib/blogs/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.1/bigsansar/contrib/blogs/models.py` & `bigsansar-2.6.2/bigsansar/contrib/blogs/models.py`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.1/bigsansar/contrib/blogs/templatetags/blogs.py` & `bigsansar-2.6.2/bigsansar/contrib/blogs/templatetags/blogs.py`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.1/bigsansar/contrib/sites/admin.py` & `bigsansar-2.6.2/bigsansar/contrib/sites/admin.py`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.1/bigsansar/contrib/sites/forms.py` & `bigsansar-2.6.2/bigsansar/contrib/sites/forms.py`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.1/bigsansar/contrib/sites/migrations/0001_initial.py` & `bigsansar-2.6.2/bigsansar/contrib/sites/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.1/bigsansar/contrib/sites/migrations/0002_default_domain.py` & `bigsansar-2.6.2/bigsansar/contrib/sites/migrations/0002_default_domain.py`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.1/bigsansar/contrib/sites/migrations/0006_default_domain_default_domain_and_more.py` & `bigsansar-2.6.2/bigsansar/contrib/sites/migrations/0006_default_domain_default_domain_and_more.py`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.1/bigsansar/contrib/sites/models.py` & `bigsansar-2.6.2/bigsansar/contrib/sites/models.py`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.1/bigsansar/contrib/sites/urls.py` & `bigsansar-2.6.2/bigsansar/contrib/sites/urls.py`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.1/bigsansar/contrib/sites/views.py` & `bigsansar-2.6.2/bigsansar/contrib/sites/views.py`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.1/bigsansar/core/__init__.py` & `bigsansar-2.6.2/bigsansar/core/__init__.py`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.1/bigsansar/core/init.py` & `bigsansar-2.6.2/bigsansar/core/init.py`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.1/bigsansar/core/pip_package.py` & `bigsansar-2.6.2/bigsansar/core/pip_package.py`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.1/bigsansar/core/ubuntu.py` & `bigsansar-2.6.2/bigsansar/core/ubuntu.py`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.1/bigsansar/etc/apache2.conf` & `bigsansar-2.6.2/bigsansar/etc/apache2.conf`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.1/bigsansar/etc/config_chroot.sh` & `bigsansar-2.6.2/bigsansar/etc/config_chroot.sh`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.1/bigsansar/etc/db.py` & `bigsansar-2.6.2/bigsansar/etc/db.py`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.1/bigsansar/etc/sshd_config` & `bigsansar-2.6.2/bigsansar/etc/sshd_config`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.1/bigsansar/management/commands/createuser.py` & `bigsansar-2.6.2/bigsansar/management/commands/createuser.py`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.1/bigsansar/management/commands/setup_server.py` & `bigsansar-2.6.2/bigsansar/management/commands/setup_server.py`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/images/icon-hdpi.png` & `bigsansar-2.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/images/icon-hdpi.png`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/images/icon.png` & `bigsansar-2.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/images/icon.png`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ar.js` & `bigsansar-2.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ar.js`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/bg.js` & `bigsansar-2.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/bg.js`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/cs.js` & `bigsansar-2.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/cs.js`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/de.js` & `bigsansar-2.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/de.js`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/el.js` & `bigsansar-2.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/el.js`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/en.js` & `bigsansar-2.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/en.js`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/es.js` & `bigsansar-2.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/es.js`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/et.js` & `bigsansar-2.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/et.js`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/eu.js` & `bigsansar-2.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/eu.js`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/fi.js` & `bigsansar-2.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/fi.js`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/fr.js` & `bigsansar-2.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/fr.js`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/he.js` & `bigsansar-2.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/he.js`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/hu.js` & `bigsansar-2.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/hu.js`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/it.js` & `bigsansar-2.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/it.js`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ja.js` & `bigsansar-2.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ja.js`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ko.js` & `bigsansar-2.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ko.js`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/nb.js` & `bigsansar-2.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/nb.js`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/nl.js` & `bigsansar-2.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/nl.js`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/nn.js` & `bigsansar-2.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/nn.js`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/pl.js` & `bigsansar-2.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/pl.js`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/pt-br.js` & `bigsansar-2.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/pt-br.js`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/pt.js` & `bigsansar-2.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/pt.js`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ru.js` & `bigsansar-2.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ru.js`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/sk.js` & `bigsansar-2.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/sk.js`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/tr.js` & `bigsansar-2.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/tr.js`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/uk.js` & `bigsansar-2.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/uk.js`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/vi.js` & `bigsansar-2.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/vi.js`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/zh.js` & `bigsansar-2.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/zh.js`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/plugin.js` & `bigsansar-2.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/plugin.js`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.1/bigsansar/static/logo.png` & `bigsansar-2.6.2/bigsansar/static/logo.png`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.1/bigsansar/static/style.css` & `bigsansar-2.6.2/bigsansar/static/style.css`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.1/bigsansar/templates/404.html` & `bigsansar-2.6.2/bigsansar/templates/404.html`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.1/bigsansar/templates/admin/account_info.html` & `bigsansar-2.6.2/bigsansar/templates/admin/account_info.html`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.1/bigsansar/templates/admin/admin_update.html` & `bigsansar-2.6.2/bigsansar/templates/admin/admin_update.html`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.1/bigsansar/templates/admin/cf_config.html` & `bigsansar-2.6.2/bigsansar/templates/admin/cf_config.html`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.1/bigsansar/templates/admin/chpass.html` & `bigsansar-2.6.2/bigsansar/templates/admin/chpass.html`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.1/bigsansar/templates/admin/chuname.html` & `bigsansar-2.6.2/bigsansar/templates/admin/chuname.html`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.1/bigsansar/templates/admin/cloudflare.html` & `bigsansar-2.6.2/bigsansar/templates/admin/cloudflare.html`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.1/bigsansar/templates/admin/create_domain.html` & `bigsansar-2.6.2/bigsansar/templates/admin/create_domain.html`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.1/bigsansar/templates/admin/db_cloudflare.html` & `bigsansar-2.6.2/bigsansar/templates/admin/db_cloudflare.html`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.1/bigsansar/templates/admin/domain_manage.html` & `bigsansar-2.6.2/bigsansar/templates/admin/domain_manage.html`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.1/bigsansar/templates/admin/edit_domain.html` & `bigsansar-2.6.2/bigsansar/templates/admin/edit_domain.html`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.1/bigsansar/templates/admin/editprofile.html` & `bigsansar-2.6.2/bigsansar/templates/admin/editprofile.html`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.1/bigsansar/templates/admin/login.html` & `bigsansar-2.6.2/bigsansar/templates/admin/login.html`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.1/bigsansar/templates/admin/nav.html` & `bigsansar-2.6.2/bigsansar/templates/admin/nav.html`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.1/bigsansar/templates/admin/page_create.html` & `bigsansar-2.6.2/bigsansar/templates/admin/page_create.html`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.1/bigsansar/templates/admin/page_delete.html` & `bigsansar-2.6.2/bigsansar/templates/admin/page_delete.html`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.1/bigsansar/templates/admin/page_edit.html` & `bigsansar-2.6.2/bigsansar/templates/admin/page_edit.html`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.1/bigsansar/templates/base.html` & `bigsansar-2.6.2/bigsansar/templates/base.html`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.1/bigsansar/templates/blog_preview.html` & `bigsansar-2.6.2/bigsansar/templates/blog_preview.html`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.1/bigsansar/templates/default.html` & `bigsansar-2.6.2/bigsansar/templates/default.html`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.1/bigsansar/templates/defaultpage.html` & `bigsansar-2.6.2/bigsansar/templates/defaultpage.html`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.1/bigsansar/templates/parking.html` & `bigsansar-2.6.2/bigsansar/templates/parking.html`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.1/bigsansar/urls.py` & `bigsansar-2.6.2/bigsansar/urls.py`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.1/bigsansar/views.py` & `bigsansar-2.6.2/bigsansar/views.py`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.1/setup.py` & `bigsansar-2.6.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="Bigsansar",
-    version="2.6.1",
+    version="2.6.2",
     author="Bikash Pokhrel",
     author_email="bigsansaroffice@gmail.com",
     description="Build one in minutes with bigsansar - a visual site building tool!",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/pokhrelb9/bigsansar",
     project_urls={
```

