# Comparing `tmp/bigsansar-2.6.3.tar.gz` & `tmp/bigsansar-2.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bigsansar-2.6.3.tar", last modified: Sun May 12 04:57:48 2024, max compression
+gzip compressed data, was "bigsansar-2.6.4.tar", last modified: Sun May 12 05:52:30 2024, max compression
```

## Comparing `bigsansar-2.6.3.tar` & `bigsansar-2.6.4.tar`

### file list

```diff
@@ -1,197 +1,197 @@
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 04:57:48.462521 bigsansar-2.6.3/
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 04:57:48.462521 bigsansar-2.6.3/Bigsansar.egg-info/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     5310 2024-05-12 04:57:48.000000 bigsansar-2.6.3/Bigsansar.egg-info/PKG-INFO
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     7368 2024-05-12 04:57:48.000000 bigsansar-2.6.3/Bigsansar.egg-info/SOURCES.txt
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        1 2024-05-12 04:57:48.000000 bigsansar-2.6.3/Bigsansar.egg-info/dependency_links.txt
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)       50 2024-05-12 04:57:48.000000 bigsansar-2.6.3/Bigsansar.egg-info/entry_points.txt
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)       98 2024-05-12 04:57:48.000000 bigsansar-2.6.3/Bigsansar.egg-info/requires.txt
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)       10 2024-05-12 04:57:48.000000 bigsansar-2.6.3/Bigsansar.egg-info/top_level.txt
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1073 2024-04-10 03:12:24.000000 bigsansar-2.6.3/LICENSE
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     5310 2024-05-12 04:57:48.462521 bigsansar-2.6.3/PKG-INFO
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     4385 2024-05-12 03:45:06.000000 bigsansar-2.6.3/README.md
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 04:57:48.342521 bigsansar-2.6.3/bigsansar/
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/__init__.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)       63 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/admin.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      188 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/apps.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 04:57:48.342521 bigsansar-2.6.3/bigsansar/contrib/
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/contrib/__init__.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 04:57:48.362521 bigsansar-2.6.3/bigsansar/contrib/account/
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/contrib/account/__init__.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      489 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/contrib/account/admin.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      275 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/contrib/account/apps.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1155 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/contrib/account/forms.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 04:57:48.362521 bigsansar-2.6.3/bigsansar/contrib/account/migrations/
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      969 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/contrib/account/migrations/0001_initial.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      400 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/contrib/account/migrations/0002_alter_userinfo_options.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/contrib/account/migrations/__init__.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      539 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/contrib/account/models.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      340 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/contrib/account/signals.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 04:57:48.362521 bigsansar-2.6.3/bigsansar/contrib/account/templates/
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/contrib/account/templates/__init__.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)       60 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/contrib/account/tests.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/contrib/account/urls.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/contrib/account/views.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 04:57:48.362521 bigsansar-2.6.3/bigsansar/contrib/advance/
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/contrib/advance/__init__.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      165 2024-05-12 03:46:34.000000 bigsansar-2.6.3/bigsansar/contrib/advance/admin.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      202 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/contrib/advance/apps.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      357 2024-05-11 07:59:27.000000 bigsansar-2.6.3/bigsansar/contrib/advance/cf_url.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     4583 2024-04-16 12:22:05.000000 bigsansar-2.6.3/bigsansar/contrib/advance/forms.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 04:57:48.362521 bigsansar-2.6.3/bigsansar/contrib/advance/migrations/
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1000 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/contrib/advance/migrations/0001_initial.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      367 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/contrib/advance/migrations/0002_alter_css_options.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1050 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/contrib/advance/migrations/0003_javascript.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      386 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/contrib/advance/migrations/0004_alter_javascript_options.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      296 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/contrib/advance/migrations/0005_delete_css.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      289 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/contrib/advance/migrations/0006_delete_javascript.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1075 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/contrib/advance/migrations/0007_initial.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      527 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/contrib/advance/migrations/0008_sidebarsettings.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      631 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/contrib/advance/migrations/0009_sidebarsettings_user.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1000 2024-04-10 05:16:13.000000 bigsansar-2.6.3/bigsansar/contrib/advance/migrations/0010_cloudflare_api.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      391 2024-04-13 11:41:57.000000 bigsansar-2.6.3/bigsansar/contrib/advance/migrations/0011_rename_account_global_api_key_cloudflare_api_global_api_key.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      637 2024-04-16 11:46:02.000000 bigsansar-2.6.3/bigsansar/contrib/advance/migrations/0012_cloudflare_api_ip_address_cloudflare_api_ip_address2.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/contrib/advance/migrations/__init__.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1356 2024-04-16 11:46:06.000000 bigsansar-2.6.3/bigsansar/contrib/advance/models.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 04:57:48.372521 bigsansar-2.6.3/bigsansar/contrib/advance/templatetags/
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/contrib/advance/templatetags/__init__.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1797 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/contrib/advance/templatetags/nav_bar.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)       60 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/contrib/advance/tests.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      721 2024-04-16 11:03:13.000000 bigsansar-2.6.3/bigsansar/contrib/advance/urls.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)    21045 2024-05-12 03:57:26.000000 bigsansar-2.6.3/bigsansar/contrib/advance/views.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 04:57:48.372521 bigsansar-2.6.3/bigsansar/contrib/blogs/
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/contrib/blogs/__init__.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     2238 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/contrib/blogs/admin.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      188 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/contrib/blogs/apps.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      261 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/contrib/blogs/forms.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 04:57:48.372521 bigsansar-2.6.3/bigsansar/contrib/blogs/migrations/
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     2261 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/contrib/blogs/migrations/0001_initial.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      367 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/contrib/blogs/migrations/0002_post_visitor.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/contrib/blogs/migrations/__init__.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     2028 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/contrib/blogs/models.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 04:57:48.372521 bigsansar-2.6.3/bigsansar/contrib/blogs/templatetags/
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/contrib/blogs/templatetags/__init__.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1478 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/contrib/blogs/templatetags/blogs.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)       60 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/contrib/blogs/tests.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)       63 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/contrib/blogs/views.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 04:57:48.382521 bigsansar-2.6.3/bigsansar/contrib/sites/
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/contrib/sites/__init__.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1719 2024-05-11 15:54:05.000000 bigsansar-2.6.3/bigsansar/contrib/sites/admin.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      196 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/contrib/sites/apps.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     4435 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/contrib/sites/forms.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 04:57:48.382521 bigsansar-2.6.3/bigsansar/contrib/sites/migrations/
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1847 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/contrib/sites/migrations/0001_initial.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      819 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/contrib/sites/migrations/0002_default_domain.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      385 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/contrib/sites/migrations/0003_domains_default.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      386 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/contrib/sites/migrations/0004_alter_domains_default.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      331 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/contrib/sites/migrations/0005_remove_domains_default.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      653 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/contrib/sites/migrations/0006_default_domain_default_domain_and_more.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      410 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/contrib/sites/migrations/0007_alter_default_domain_default_domain.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      411 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/contrib/sites/migrations/0008_domains_primary_domain.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      346 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/contrib/sites/migrations/0009_remove_default_domain_default_domain.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      422 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/contrib/sites/migrations/0010_alter_domains_description.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      405 2024-05-09 10:32:01.000000 bigsansar-2.6.3/bigsansar/contrib/sites/migrations/0011_domains_zone_id.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/contrib/sites/migrations/__init__.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     2453 2024-05-09 10:31:51.000000 bigsansar-2.6.3/bigsansar/contrib/sites/models.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 04:57:48.382521 bigsansar-2.6.3/bigsansar/contrib/sites/templatetags/
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/contrib/sites/templatetags/__init__.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      394 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/contrib/sites/templatetags/pages.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)       60 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/contrib/sites/tests.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      547 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/contrib/sites/urls.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     9258 2024-04-10 10:36:13.000000 bigsansar-2.6.3/bigsansar/contrib/sites/views.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/contrib/urls.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/contrib/views.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 04:57:48.392521 bigsansar-2.6.3/bigsansar/core/
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1018 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/core/__init__.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      402 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/core/host.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     9710 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/core/init.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      640 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/core/pip_package.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)    17221 2024-05-12 04:55:35.000000 bigsansar-2.6.3/bigsansar/core/ubuntu.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 04:57:48.392521 bigsansar-2.6.3/bigsansar/etc/
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     7287 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/etc/apache2.conf
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1638 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/etc/config_chroot.sh
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     5123 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/etc/db.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     3236 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/etc/sshd_config
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 04:57:48.392521 bigsansar-2.6.3/bigsansar/management/
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/management/__init__.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 04:57:48.392521 bigsansar-2.6.3/bigsansar/management/commands/
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/management/commands/__init__.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1076 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/management/commands/createuser.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1023 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/management/commands/setup_server.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 04:57:48.392521 bigsansar-2.6.3/bigsansar/migrations/
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/migrations/__init__.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)       57 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/models.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 04:57:48.392521 bigsansar-2.6.3/bigsansar/static/
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/static/__init__.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 04:57:48.322521 bigsansar-2.6.3/bigsansar/static/ckeditor/
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 04:57:48.322521 bigsansar-2.6.3/bigsansar/static/ckeditor/ckeditor/
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 04:57:48.322521 bigsansar-2.6.3/bigsansar/static/ckeditor/ckeditor/plugins/
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 04:57:48.392521 bigsansar-2.6.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 04:57:48.392521 bigsansar-2.6.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/images/
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1258 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/images/icon-hdpi.png
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1165 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/images/icon.png
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 04:57:48.422521 bigsansar-2.6.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1337 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ar.js
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1654 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/bg.js
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1184 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/cs.js
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1078 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/de.js
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1514 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/el.js
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1024 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/en.js
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1084 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/es.js
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1079 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/et.js
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1161 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/eu.js
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      960 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/fi.js
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1051 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/fr.js
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1226 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/he.js
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1166 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/hu.js
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1081 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/it.js
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1171 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ja.js
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1229 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ko.js
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1035 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/nb.js
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1022 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/nl.js
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1040 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/nn.js
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1120 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/pl.js
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1151 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/pt-br.js
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1153 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/pt.js
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1539 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ru.js
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1173 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/sk.js
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1206 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/tr.js
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1538 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/uk.js
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1067 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/vi.js
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      916 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/zh.js
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)    13371 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/plugin.js
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     9230 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/static/logo.png
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      551 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/static/style.css
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 04:57:48.432521 bigsansar-2.6.3/bigsansar/templates/
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      947 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/templates/404.html
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/templates/__init__.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      164 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/templates/acc_active_email.html
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 04:57:48.462521 bigsansar-2.6.3/bigsansar/templates/admin/
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)    10272 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/templates/admin/account_info.html
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      519 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/templates/admin/admin_update.html
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      878 2024-04-13 11:47:55.000000 bigsansar-2.6.3/bigsansar/templates/admin/cf_config.html
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      558 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/templates/admin/chpass.html
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      558 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/templates/admin/chuname.html
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     4745 2024-05-12 04:16:59.000000 bigsansar-2.6.3/bigsansar/templates/admin/cloudflare.html
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      549 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/templates/admin/create_domain.html
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1637 2024-05-11 15:51:11.000000 bigsansar-2.6.3/bigsansar/templates/admin/db_cloudflare.html
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     8866 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/templates/admin/domain_manage.html
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1019 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/templates/admin/edit_domain.html
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      566 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/templates/admin/editprofile.html
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      979 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/templates/admin/login.html
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     6004 2024-04-16 11:03:44.000000 bigsansar-2.6.3/bigsansar/templates/admin/nav.html
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      947 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/templates/admin/page_create.html
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      948 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/templates/admin/page_delete.html
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      717 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/templates/admin/page_edit.html
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1622 2024-05-11 07:51:33.000000 bigsansar-2.6.3/bigsansar/templates/base.html
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1898 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/templates/blog_preview.html
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     2197 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/templates/default.html
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     2200 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/templates/defaultpage.html
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      719 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/templates/parking.html
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      101 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/templates/script.html
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      411 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/templates/sitemap.html
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      101 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/templates/styles.html
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)       60 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/tests.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1209 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/urls.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     4595 2024-04-10 03:12:24.000000 bigsansar-2.6.3/bigsansar/views.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       38 2024-05-12 04:57:48.462521 bigsansar-2.6.3/setup.cfg
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1914 2024-05-12 04:56:09.000000 bigsansar-2.6.3/setup.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 05:52:30.852524 bigsansar-2.6.4/
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 05:52:30.852524 bigsansar-2.6.4/Bigsansar.egg-info/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     5310 2024-05-12 05:52:30.000000 bigsansar-2.6.4/Bigsansar.egg-info/PKG-INFO
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     7368 2024-05-12 05:52:30.000000 bigsansar-2.6.4/Bigsansar.egg-info/SOURCES.txt
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        1 2024-05-12 05:52:30.000000 bigsansar-2.6.4/Bigsansar.egg-info/dependency_links.txt
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)       50 2024-05-12 05:52:30.000000 bigsansar-2.6.4/Bigsansar.egg-info/entry_points.txt
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)       98 2024-05-12 05:52:30.000000 bigsansar-2.6.4/Bigsansar.egg-info/requires.txt
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)       10 2024-05-12 05:52:30.000000 bigsansar-2.6.4/Bigsansar.egg-info/top_level.txt
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1073 2024-04-10 03:12:24.000000 bigsansar-2.6.4/LICENSE
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     5310 2024-05-12 05:52:30.852524 bigsansar-2.6.4/PKG-INFO
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     4385 2024-05-12 03:45:06.000000 bigsansar-2.6.4/README.md
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 05:52:30.732524 bigsansar-2.6.4/bigsansar/
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/__init__.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)       63 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/admin.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      188 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/apps.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 05:52:30.732524 bigsansar-2.6.4/bigsansar/contrib/
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/contrib/__init__.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 05:52:30.742524 bigsansar-2.6.4/bigsansar/contrib/account/
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/contrib/account/__init__.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      489 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/contrib/account/admin.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      275 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/contrib/account/apps.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1155 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/contrib/account/forms.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 05:52:30.742524 bigsansar-2.6.4/bigsansar/contrib/account/migrations/
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      969 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/contrib/account/migrations/0001_initial.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      400 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/contrib/account/migrations/0002_alter_userinfo_options.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/contrib/account/migrations/__init__.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      539 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/contrib/account/models.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      340 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/contrib/account/signals.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 05:52:30.742524 bigsansar-2.6.4/bigsansar/contrib/account/templates/
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/contrib/account/templates/__init__.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)       60 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/contrib/account/tests.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/contrib/account/urls.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/contrib/account/views.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 05:52:30.752524 bigsansar-2.6.4/bigsansar/contrib/advance/
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/contrib/advance/__init__.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      165 2024-05-12 03:46:34.000000 bigsansar-2.6.4/bigsansar/contrib/advance/admin.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      202 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/contrib/advance/apps.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      357 2024-05-11 07:59:27.000000 bigsansar-2.6.4/bigsansar/contrib/advance/cf_url.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     4583 2024-04-16 12:22:05.000000 bigsansar-2.6.4/bigsansar/contrib/advance/forms.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 05:52:30.772524 bigsansar-2.6.4/bigsansar/contrib/advance/migrations/
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1000 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/contrib/advance/migrations/0001_initial.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      367 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/contrib/advance/migrations/0002_alter_css_options.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1050 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/contrib/advance/migrations/0003_javascript.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      386 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/contrib/advance/migrations/0004_alter_javascript_options.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      296 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/contrib/advance/migrations/0005_delete_css.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      289 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/contrib/advance/migrations/0006_delete_javascript.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1075 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/contrib/advance/migrations/0007_initial.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      527 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/contrib/advance/migrations/0008_sidebarsettings.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      631 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/contrib/advance/migrations/0009_sidebarsettings_user.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1000 2024-04-10 05:16:13.000000 bigsansar-2.6.4/bigsansar/contrib/advance/migrations/0010_cloudflare_api.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      391 2024-04-13 11:41:57.000000 bigsansar-2.6.4/bigsansar/contrib/advance/migrations/0011_rename_account_global_api_key_cloudflare_api_global_api_key.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      637 2024-04-16 11:46:02.000000 bigsansar-2.6.4/bigsansar/contrib/advance/migrations/0012_cloudflare_api_ip_address_cloudflare_api_ip_address2.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/contrib/advance/migrations/__init__.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1356 2024-04-16 11:46:06.000000 bigsansar-2.6.4/bigsansar/contrib/advance/models.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 05:52:30.772524 bigsansar-2.6.4/bigsansar/contrib/advance/templatetags/
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/contrib/advance/templatetags/__init__.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1797 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/contrib/advance/templatetags/nav_bar.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)       60 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/contrib/advance/tests.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      721 2024-04-16 11:03:13.000000 bigsansar-2.6.4/bigsansar/contrib/advance/urls.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)    21006 2024-05-12 05:48:56.000000 bigsansar-2.6.4/bigsansar/contrib/advance/views.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 05:52:30.772524 bigsansar-2.6.4/bigsansar/contrib/blogs/
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/contrib/blogs/__init__.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     2238 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/contrib/blogs/admin.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      188 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/contrib/blogs/apps.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      261 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/contrib/blogs/forms.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 05:52:30.782524 bigsansar-2.6.4/bigsansar/contrib/blogs/migrations/
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     2261 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/contrib/blogs/migrations/0001_initial.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      367 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/contrib/blogs/migrations/0002_post_visitor.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/contrib/blogs/migrations/__init__.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     2028 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/contrib/blogs/models.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 05:52:30.782524 bigsansar-2.6.4/bigsansar/contrib/blogs/templatetags/
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/contrib/blogs/templatetags/__init__.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1478 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/contrib/blogs/templatetags/blogs.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)       60 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/contrib/blogs/tests.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)       63 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/contrib/blogs/views.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 05:52:30.792524 bigsansar-2.6.4/bigsansar/contrib/sites/
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/contrib/sites/__init__.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1647 2024-05-12 05:33:47.000000 bigsansar-2.6.4/bigsansar/contrib/sites/admin.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      196 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/contrib/sites/apps.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     4435 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/contrib/sites/forms.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 05:52:30.792524 bigsansar-2.6.4/bigsansar/contrib/sites/migrations/
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1847 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/contrib/sites/migrations/0001_initial.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      819 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/contrib/sites/migrations/0002_default_domain.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      385 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/contrib/sites/migrations/0003_domains_default.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      386 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/contrib/sites/migrations/0004_alter_domains_default.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      331 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/contrib/sites/migrations/0005_remove_domains_default.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      653 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/contrib/sites/migrations/0006_default_domain_default_domain_and_more.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      410 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/contrib/sites/migrations/0007_alter_default_domain_default_domain.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      411 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/contrib/sites/migrations/0008_domains_primary_domain.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      346 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/contrib/sites/migrations/0009_remove_default_domain_default_domain.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      422 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/contrib/sites/migrations/0010_alter_domains_description.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      405 2024-05-09 10:32:01.000000 bigsansar-2.6.4/bigsansar/contrib/sites/migrations/0011_domains_zone_id.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/contrib/sites/migrations/__init__.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     2453 2024-05-09 10:31:51.000000 bigsansar-2.6.4/bigsansar/contrib/sites/models.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 05:52:30.812524 bigsansar-2.6.4/bigsansar/contrib/sites/templatetags/
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/contrib/sites/templatetags/__init__.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      394 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/contrib/sites/templatetags/pages.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)       60 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/contrib/sites/tests.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      547 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/contrib/sites/urls.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     9258 2024-04-10 10:36:13.000000 bigsansar-2.6.4/bigsansar/contrib/sites/views.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/contrib/urls.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/contrib/views.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 05:52:30.812524 bigsansar-2.6.4/bigsansar/core/
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1018 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/core/__init__.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      402 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/core/host.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     9710 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/core/init.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      640 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/core/pip_package.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)    17221 2024-05-12 04:55:35.000000 bigsansar-2.6.4/bigsansar/core/ubuntu.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 05:52:30.812524 bigsansar-2.6.4/bigsansar/etc/
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     7287 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/etc/apache2.conf
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1638 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/etc/config_chroot.sh
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     5123 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/etc/db.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     3236 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/etc/sshd_config
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 05:52:30.812524 bigsansar-2.6.4/bigsansar/management/
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/management/__init__.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 05:52:30.812524 bigsansar-2.6.4/bigsansar/management/commands/
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/management/commands/__init__.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1076 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/management/commands/createuser.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1023 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/management/commands/setup_server.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 05:52:30.812524 bigsansar-2.6.4/bigsansar/migrations/
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/migrations/__init__.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)       57 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/models.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 05:52:30.812524 bigsansar-2.6.4/bigsansar/static/
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/static/__init__.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 05:52:30.712524 bigsansar-2.6.4/bigsansar/static/ckeditor/
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 05:52:30.712524 bigsansar-2.6.4/bigsansar/static/ckeditor/ckeditor/
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 05:52:30.712524 bigsansar-2.6.4/bigsansar/static/ckeditor/ckeditor/plugins/
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 05:52:30.812524 bigsansar-2.6.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 05:52:30.812524 bigsansar-2.6.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/images/
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1258 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/images/icon-hdpi.png
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1165 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/images/icon.png
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 05:52:30.832524 bigsansar-2.6.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1337 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ar.js
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1654 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/bg.js
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1184 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/cs.js
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1078 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/de.js
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1514 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/el.js
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1024 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/en.js
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1084 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/es.js
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1079 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/et.js
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1161 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/eu.js
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      960 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/fi.js
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1051 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/fr.js
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1226 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/he.js
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1166 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/hu.js
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1081 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/it.js
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1171 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ja.js
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1229 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ko.js
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1035 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/nb.js
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1022 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/nl.js
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1040 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/nn.js
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1120 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/pl.js
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1151 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/pt-br.js
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1153 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/pt.js
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1539 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ru.js
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1173 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/sk.js
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1206 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/tr.js
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1538 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/uk.js
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1067 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/vi.js
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      916 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/zh.js
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)    13371 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/plugin.js
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     9230 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/static/logo.png
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      551 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/static/style.css
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 05:52:30.842524 bigsansar-2.6.4/bigsansar/templates/
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      947 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/templates/404.html
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/templates/__init__.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      164 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/templates/acc_active_email.html
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-12 05:52:30.852524 bigsansar-2.6.4/bigsansar/templates/admin/
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)    10272 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/templates/admin/account_info.html
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      519 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/templates/admin/admin_update.html
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      878 2024-04-13 11:47:55.000000 bigsansar-2.6.4/bigsansar/templates/admin/cf_config.html
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      558 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/templates/admin/chpass.html
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      558 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/templates/admin/chuname.html
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     4745 2024-05-12 04:16:59.000000 bigsansar-2.6.4/bigsansar/templates/admin/cloudflare.html
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      549 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/templates/admin/create_domain.html
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1637 2024-05-11 15:51:11.000000 bigsansar-2.6.4/bigsansar/templates/admin/db_cloudflare.html
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     8866 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/templates/admin/domain_manage.html
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1019 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/templates/admin/edit_domain.html
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      566 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/templates/admin/editprofile.html
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      979 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/templates/admin/login.html
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     6004 2024-04-16 11:03:44.000000 bigsansar-2.6.4/bigsansar/templates/admin/nav.html
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      947 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/templates/admin/page_create.html
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      948 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/templates/admin/page_delete.html
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      717 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/templates/admin/page_edit.html
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1622 2024-05-11 07:51:33.000000 bigsansar-2.6.4/bigsansar/templates/base.html
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1898 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/templates/blog_preview.html
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     2197 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/templates/default.html
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     2200 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/templates/defaultpage.html
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      719 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/templates/parking.html
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      101 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/templates/script.html
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      411 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/templates/sitemap.html
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      101 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/templates/styles.html
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)       60 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/tests.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1209 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/urls.py
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     4595 2024-04-10 03:12:24.000000 bigsansar-2.6.4/bigsansar/views.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       38 2024-05-12 05:52:30.852524 bigsansar-2.6.4/setup.cfg
+-rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1914 2024-05-12 05:52:00.000000 bigsansar-2.6.4/setup.py
```

### Comparing `bigsansar-2.6.3/Bigsansar.egg-info/PKG-INFO` & `bigsansar-2.6.4/Bigsansar.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Bigsansar
-Version: 2.6.3
+Version: 2.6.4
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
-Metadata-Version: 2.1 Name: Bigsansar Version: 2.6.3 Summary: Build one in
+Metadata-Version: 2.1 Name: Bigsansar Version: 2.6.4 Summary: Build one in
 minutes with bigsansar - a visual site building tool! Home-page: https://
 github.com/pokhrelb9/bigsansar Author: Bikash Pokhrel Author-email:
 bigsansaroffice@gmail.com Project-URL: Bug Tracker, https://github.com/
 pokhrelb9/bigsansar/issues Project-URL: Documentations, https://
 docs.bigsansar.com/ Keywords: python,django host,bigsansar,django,django sites
 framework,django flatpages Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
```

### Comparing `bigsansar-2.6.3/Bigsansar.egg-info/SOURCES.txt` & `bigsansar-2.6.4/Bigsansar.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.3/LICENSE` & `bigsansar-2.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.3/PKG-INFO` & `bigsansar-2.6.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Bigsansar
-Version: 2.6.3
+Version: 2.6.4
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
-Metadata-Version: 2.1 Name: Bigsansar Version: 2.6.3 Summary: Build one in
+Metadata-Version: 2.1 Name: Bigsansar Version: 2.6.4 Summary: Build one in
 minutes with bigsansar - a visual site building tool! Home-page: https://
 github.com/pokhrelb9/bigsansar Author: Bikash Pokhrel Author-email:
 bigsansaroffice@gmail.com Project-URL: Bug Tracker, https://github.com/
 pokhrelb9/bigsansar/issues Project-URL: Documentations, https://
 docs.bigsansar.com/ Keywords: python,django host,bigsansar,django,django sites
 framework,django flatpages Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
```

### Comparing `bigsansar-2.6.3/README.md` & `bigsansar-2.6.4/README.md`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.3/bigsansar/contrib/account/forms.py` & `bigsansar-2.6.4/bigsansar/contrib/account/forms.py`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.3/bigsansar/contrib/account/migrations/0001_initial.py` & `bigsansar-2.6.4/bigsansar/contrib/account/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.3/bigsansar/contrib/account/models.py` & `bigsansar-2.6.4/bigsansar/contrib/account/models.py`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.3/bigsansar/contrib/advance/forms.py` & `bigsansar-2.6.4/bigsansar/contrib/advance/forms.py`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.3/bigsansar/contrib/advance/migrations/0001_initial.py` & `bigsansar-2.6.4/bigsansar/contrib/advance/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.3/bigsansar/contrib/advance/migrations/0003_javascript.py` & `bigsansar-2.6.4/bigsansar/contrib/advance/migrations/0003_javascript.py`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.3/bigsansar/contrib/advance/migrations/0007_initial.py` & `bigsansar-2.6.4/bigsansar/contrib/advance/migrations/0007_initial.py`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.3/bigsansar/contrib/advance/migrations/0008_sidebarsettings.py` & `bigsansar-2.6.4/bigsansar/contrib/advance/migrations/0008_sidebarsettings.py`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.3/bigsansar/contrib/advance/migrations/0009_sidebarsettings_user.py` & `bigsansar-2.6.4/bigsansar/contrib/advance/migrations/0009_sidebarsettings_user.py`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.3/bigsansar/contrib/advance/migrations/0010_cloudflare_api.py` & `bigsansar-2.6.4/bigsansar/contrib/advance/migrations/0010_cloudflare_api.py`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.3/bigsansar/contrib/advance/migrations/0012_cloudflare_api_ip_address_cloudflare_api_ip_address2.py` & `bigsansar-2.6.4/bigsansar/contrib/advance/migrations/0012_cloudflare_api_ip_address_cloudflare_api_ip_address2.py`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.3/bigsansar/contrib/advance/models.py` & `bigsansar-2.6.4/bigsansar/contrib/advance/models.py`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.3/bigsansar/contrib/advance/templatetags/nav_bar.py` & `bigsansar-2.6.4/bigsansar/contrib/advance/templatetags/nav_bar.py`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.3/bigsansar/contrib/advance/urls.py` & `bigsansar-2.6.4/bigsansar/contrib/advance/urls.py`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.3/bigsansar/contrib/advance/views.py` & `bigsansar-2.6.4/bigsansar/contrib/advance/views.py`

 * *Files 3% similar despite different names*

```diff
@@ -347,24 +347,29 @@
                             for record in dns_records:
                                 dns_response = requests.post(dns_url, json=record, headers=headers)
                             if dns_response.status_code == 200:
                                 cloudflare_api.objects.update_or_create(defaults={'user': user, 'main_domain_name': zone, 'account_id': account_id, 'ip_address':
                                                                                             ip1, 'ip_address2': ip2})
                                                                                              
                                 
-                                domains.objects.create(user=request.user, domain=zone, Description=zone, zone_id=zone_id)
+                                domains.objects.create(user=user, domain=zone, Description=zone, zone_id=zone_id)
                                 
                                 #get_id = domains.objects.get(user=user, domain=zone).id
                                 messages.success(request, 'updated Successfully Created')
                                 return redirect(f'/admin/cf/')
                         
                             else:
                                 cloudflare_api.objects.update_or_create(defaults={'user': user, 'main_domain_name': zone, 'account_id': account_id, 'ip_address':
                                                                                             ip1, 'ip_address2': ip2})
-                                domains.objects.filter(user=user, domain=zone).update(zone_id=zone_id)
+                                try:
+                                    
+                                    domains.objects.create(user=user, domain=zone, Description=zone, zone_id=zone_id)
+                                except:
+                                    domains.objects.filter(user=user, domain=zone).update(zone_id=zone_id)
+
                                 messages.success(request, 'updated Successfully Created')
                                 return redirect(f'/admin/cf/')
                             
                         
                         else:
                             messages.warning(request, "'error': 'Failed to fetch data from Cloudflare API Account id or domain already exists'")
                             return render(request, 'admin/cf_config.html', {'head': form_title, 'form': form})
@@ -418,17 +423,19 @@
 # def ff(request):
 #     domains.objects.create(user=request.user, domain='test.com', Description='')
 
 
 def ssl_origin(request):
     if request.user.is_authenticated:
         if request.user.is_superuser:
-            get_zone_id = domains.objects.get(domain=query.main_domain_name).zone_id
-            
             query = cloudflare_api.objects.latest('id')
+            get_domain_query = domains.objects.get(domain=query.main_domain_name)
+            get_zone_id = get_domain_query.zone_id
+            doamin_name = get_domain_query.domain
+            
             headers = {
                             'Content-Type': 'application/json',
                             'X-Auth-Email': query.email,
                             'X-Auth-Key': query.global_api_key
                         }
             url = f'https://api.cloudflare.com/client/v4/zones/{get_zone_id}/settings/ssl'
             
@@ -436,48 +443,36 @@
             data = {
                 "value": "strict"
             }
             response = requests.patch(url, json=data, headers=headers)
             if response.status_code == 200:
                 
                 url_for_cert = f"https://api.cloudflare.com/client/v4/zones/{get_zone_id}/ssl/certificate/packs"
-                # # Certificate and private key files
-                certificate_path = BASE_DIR / 'ssl/ssl-cert-snakeoil.pem'
-                # private_key_path = BASE_DIR / 'ssl/ssl-cert-snakeoil.key'
-
-                #  # Read certificate and private key contents
-                with open(certificate_path, "r") as cert_file:
-                    certificate = cert_file.read()
-                # with open(private_key_path, "r") as key_file:
-                #     private_key = key_file.read()
 
-
-                # data = {
-                #     "certificate": certificate,
-                #     "private_key": private_key,
-                #     "bundle_method": "ubiquitous"
-                # }
-                hostnames = ["bigsansar.com", "*.bigsansar.com"]
+                hostnames = [f"{doamin_name}", f"*.{doamin_name}"]
+                csr_path = BASE_DIR / 'ssl/server.csr'
+                # Read certificate and private key contents
+                with open(csr_path, "r") as pem_file:
+                    csr = pem_file.read()
 
                 data = {
-                        "certificate_request": certificate,
+                        "certificate_request": csr,
                         "hostnames": hostnames,
                         "requested_validity": 5475  # Validity in days (15 years)
                     }
+                # data = {
+                #         "csr": "-----BEGIN CERTIFICATE REQUEST-----\nMIICxzCCAa8CAQAwSDELMAkGA1UEBhMCVVMxFjAUBgNVBAgTDVNhbiBGcmFuY2lz\nY28xCzAJBgNVBAcTAkNBMRQwEgYDVQQDEwtleGFtcGxlLm5ldDCCASIwDQYJKoZI\nhvcNAQEBBQADggEPADCCAQoCggEBALxejtu4b+jPdFeFi6OUsye8TYJQBm3WfCvL\nHu5EvijMO/4Z2TImwASbwUF7Ir8OLgH+mGlQZeqyNvGoSOMEaZVXcYfpR1hlVak8\n4GGVr+04IGfOCqaBokaBFIwzclGZbzKmLGwIQioNxGfqFm6RGYGA3be2Je2iseBc\nN8GV1wYmvYE0RR+yWweJCTJ157exyRzu7sVxaEW9F87zBQLyOnwXc64rflXslRqi\ng7F7w5IaQYOl8yvmk/jEPCAha7fkiUfEpj4N12+oPRiMvleJF98chxjD4MH39c5I\nuOslULhrWunfh7GB1jwWNA9y44H0snrf+xvoy2TcHmxvma9Eln8CAwEAAaA6MDgG\nCSqGSIb3DQEJDjErMCkwJwYDVR0RBCAwHoILZXhhbXBsZS5uZXSCD3d3dy5leGFt\ncGxlLm5ldDANBgkqhkiG9w0BAQsFAAOCAQEAcBaX6dOnI8ncARrI9ZSF2AJX+8mx\npTHY2+Y2C0VvrVDGMtbBRH8R9yMbqWtlxeeNGf//LeMkSKSFa4kbpdx226lfui8/\nauRDBTJGx2R1ccUxmLZXx4my0W5iIMxunu+kez+BDlu7bTT2io0uXMRHue4i6quH\nyc5ibxvbJMjR7dqbcanVE10/34oprzXQsJ/VmSuZNXtjbtSKDlmcpw6To/eeAJ+J\nhXykcUihvHyG4A1m2R6qpANBjnA0pHexfwM/SgfzvpbvUg0T1ubmer8BgTwCKIWs\ndcWYTthM51JIqRBfNqy4QcBnX+GY05yltEEswQI55wdiS3CjTTA67sdbcQ==\n-----END CERTIFICATE REQUEST-----",
+                #         "hostnames": [
+                #             "bigsansar.com",
+                #             "*.bigsansar.com"
+                #         ],
+                #         "request_type": "origin-rsa",
+                #         "requested_validity": 5475
+                #     }
                 
-
-    #             data = {
-    #     "csr": "-----BEGIN CERTIFICATE REQUEST-----\nMIICxzCCAa8CAQAwSDELMAkGA1UEBhMCVVMxFjAUBgNVBAgTDVNhbiBGcmFuY2lz\nY28xCzAJBgNVBAcTAkNBMRQwEgYDVQQDEwtleGFtcGxlLm5ldDCCASIwDQYJKoZI\nhvcNAQEBBQADggEPADCCAQoCggEBALxejtu4b+jPdFeFi6OUsye8TYJQBm3WfCvL\nHu5EvijMO/4Z2TImwASbwUF7Ir8OLgH+mGlQZeqyNvGoSOMEaZVXcYfpR1hlVak8\n4GGVr+04IGfOCqaBokaBFIwzclGZbzKmLGwIQioNxGfqFm6RGYGA3be2Je2iseBc\nN8GV1wYmvYE0RR+yWweJCTJ157exyRzu7sVxaEW9F87zBQLyOnwXc64rflXslRqi\ng7F7w5IaQYOl8yvmk/jEPCAha7fkiUfEpj4N12+oPRiMvleJF98chxjD4MH39c5I\nuOslULhrWunfh7GB1jwWNA9y44H0snrf+xvoy2TcHmxvma9Eln8CAwEAAaA6MDgG\nCSqGSIb3DQEJDjErMCkwJwYDVR0RBCAwHoILZXhhbXBsZS5uZXSCD3d3dy5leGFt\ncGxlLm5ldDANBgkqhkiG9w0BAQsFAAOCAQEAcBaX6dOnI8ncARrI9ZSF2AJX+8mx\npTHY2+Y2C0VvrVDGMtbBRH8R9yMbqWtlxeeNGf//LeMkSKSFa4kbpdx226lfui8/\nauRDBTJGx2R1ccUxmLZXx4my0W5iIMxunu+kez+BDlu7bTT2io0uXMRHue4i6quH\nyc5ibxvbJMjR7dqbcanVE10/34oprzXQsJ/VmSuZNXtjbtSKDlmcpw6To/eeAJ+J\nhXykcUihvHyG4A1m2R6qpANBjnA0pHexfwM/SgfzvpbvUg0T1ubmer8BgTwCKIWs\ndcWYTthM51JIqRBfNqy4QcBnX+GY05yltEEswQI55wdiS3CjTTA67sdbcQ==\n-----END CERTIFICATE REQUEST-----",
-    #     "hostnames": [
-    #         "bigsansar.com",
-    #         "*.bigsansar.com"
-    #     ],
-    #     "request_type": "origin-rsa",
-    #     "requested_validity": 5475
-    # }
                 response2 = requests.post(url_for_cert, json=data, headers=headers)
                 if response2.status_code == 200:
                     data = response2.json()
                     return JsonResponse(data)
                 else:
                     return JsonResponse({'error': 'Failed to u.'}, status=500)
```

### Comparing `bigsansar-2.6.3/bigsansar/contrib/blogs/admin.py` & `bigsansar-2.6.4/bigsansar/contrib/blogs/admin.py`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.3/bigsansar/contrib/blogs/migrations/0001_initial.py` & `bigsansar-2.6.4/bigsansar/contrib/blogs/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.3/bigsansar/contrib/blogs/models.py` & `bigsansar-2.6.4/bigsansar/contrib/blogs/models.py`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.3/bigsansar/contrib/blogs/templatetags/blogs.py` & `bigsansar-2.6.4/bigsansar/contrib/blogs/templatetags/blogs.py`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.3/bigsansar/contrib/sites/admin.py` & `bigsansar-2.6.4/bigsansar/contrib/sites/admin.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,52 +1,52 @@
-# from django.contrib import admin
-# from django.contrib.admin import SimpleListFilter
-# from django.utils.translation import gettext_lazy as _
-# from bigsansar.contrib.sites.forms import create_domainform, customaddpageform, custompageform
-# from bigsansar.contrib.sites.models import default_domain, domains, pages
-# from django.contrib.auth.models import User
+from django.contrib import admin
+from django.contrib.admin import SimpleListFilter
+from django.utils.translation import gettext_lazy as _
+from bigsansar.contrib.sites.forms import create_domainform, customaddpageform, custompageform
+from bigsansar.contrib.sites.models import default_domain, domains, pages
+from django.contrib.auth.models import User
 
 
-# # Register your models here.
+# Register your models here.
 
 
-# class domain_filter(SimpleListFilter):
-#     title = _('Domains')  # a label for our filter
-#     parameter_name = "domain"  # you can put anything here
+class domain_filter(SimpleListFilter):
+    title = _('Domains')  # a label for our filter
+    parameter_name = "domain"  # you can put anything here
 
-#     def lookups(self, request, model_admin):
-#         # This is where you create filter options; we have two:
-#         qs = model_admin.get_queryset(request)
-#         return qs.values_list('domain_id', 'domain__domain').order_by('domain').distinct()
+    def lookups(self, request, model_admin):
+        # This is where you create filter options; we have two:
+        qs = model_admin.get_queryset(request)
+        return qs.values_list('domain_id', 'domain__domain').order_by('domain').distinct()
 
-#     def queryset(self, request, queryset):
+    def queryset(self, request, queryset):
 
-#         # This is where you process parameters selected by use via filter options:
-#         if self.value():
-#             return queryset.filter(domain=self.value())
+        # This is where you process parameters selected by use via filter options:
+        if self.value():
+            return queryset.filter(domain=self.value())
 
 
 
 
-# class pageadmin(admin.ModelAdmin):
-#     add_form = customaddpageform
-#     form = custompageform
-#     prepopulated_fields = {"slug": ("title",)}
-#     list_display = ['slug', 'domain', 'publish_date', 'visitor']
-#     list_filter = (domain_filter,)
-#     search_fields = ['slug']
+class pageadmin(admin.ModelAdmin):
+    add_form = customaddpageform
+    form = custompageform
+    prepopulated_fields = {"slug": ("title",)}
+    list_display = ['slug', 'domain', 'publish_date', 'visitor']
+    list_filter = (domain_filter,)
+    search_fields = ['slug']
 
-#     def get_form(self, request, obj=None, **kwargs):
-#         """
-#         Use special form during foo creation
-#         """
-#         defaults = {}
-#         if obj is None:
-#             defaults['form'] = self.add_form
-#         defaults.update(kwargs)
-#         return super().get_form(request, obj, **defaults)
+    def get_form(self, request, obj=None, **kwargs):
+        """
+        Use special form during foo creation
+        """
+        defaults = {}
+        if obj is None:
+            defaults['form'] = self.add_form
+        defaults.update(kwargs)
+        return super().get_form(request, obj, **defaults)
         
 
 
-# admin.site.register(pages, pageadmin)
+admin.site.register(pages, pageadmin)
 
-# admin.site.register(domains)
+admin.site.register(domains)
```

### Comparing `bigsansar-2.6.3/bigsansar/contrib/sites/forms.py` & `bigsansar-2.6.4/bigsansar/contrib/sites/forms.py`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.3/bigsansar/contrib/sites/migrations/0001_initial.py` & `bigsansar-2.6.4/bigsansar/contrib/sites/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.3/bigsansar/contrib/sites/migrations/0002_default_domain.py` & `bigsansar-2.6.4/bigsansar/contrib/sites/migrations/0002_default_domain.py`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.3/bigsansar/contrib/sites/migrations/0006_default_domain_default_domain_and_more.py` & `bigsansar-2.6.4/bigsansar/contrib/sites/migrations/0006_default_domain_default_domain_and_more.py`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.3/bigsansar/contrib/sites/models.py` & `bigsansar-2.6.4/bigsansar/contrib/sites/models.py`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.3/bigsansar/contrib/sites/urls.py` & `bigsansar-2.6.4/bigsansar/contrib/sites/urls.py`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.3/bigsansar/contrib/sites/views.py` & `bigsansar-2.6.4/bigsansar/contrib/sites/views.py`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.3/bigsansar/core/__init__.py` & `bigsansar-2.6.4/bigsansar/core/__init__.py`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.3/bigsansar/core/init.py` & `bigsansar-2.6.4/bigsansar/core/init.py`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.3/bigsansar/core/pip_package.py` & `bigsansar-2.6.4/bigsansar/core/pip_package.py`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.3/bigsansar/core/ubuntu.py` & `bigsansar-2.6.4/bigsansar/core/ubuntu.py`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.3/bigsansar/etc/apache2.conf` & `bigsansar-2.6.4/bigsansar/etc/apache2.conf`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.3/bigsansar/etc/config_chroot.sh` & `bigsansar-2.6.4/bigsansar/etc/config_chroot.sh`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.3/bigsansar/etc/db.py` & `bigsansar-2.6.4/bigsansar/etc/db.py`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.3/bigsansar/etc/sshd_config` & `bigsansar-2.6.4/bigsansar/etc/sshd_config`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.3/bigsansar/management/commands/createuser.py` & `bigsansar-2.6.4/bigsansar/management/commands/createuser.py`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.3/bigsansar/management/commands/setup_server.py` & `bigsansar-2.6.4/bigsansar/management/commands/setup_server.py`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/images/icon-hdpi.png` & `bigsansar-2.6.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/images/icon-hdpi.png`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/images/icon.png` & `bigsansar-2.6.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/images/icon.png`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ar.js` & `bigsansar-2.6.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ar.js`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/bg.js` & `bigsansar-2.6.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/bg.js`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/cs.js` & `bigsansar-2.6.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/cs.js`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/de.js` & `bigsansar-2.6.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/de.js`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/el.js` & `bigsansar-2.6.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/el.js`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/en.js` & `bigsansar-2.6.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/en.js`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/es.js` & `bigsansar-2.6.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/es.js`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/et.js` & `bigsansar-2.6.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/et.js`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/eu.js` & `bigsansar-2.6.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/eu.js`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/fi.js` & `bigsansar-2.6.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/fi.js`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/fr.js` & `bigsansar-2.6.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/fr.js`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/he.js` & `bigsansar-2.6.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/he.js`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/hu.js` & `bigsansar-2.6.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/hu.js`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/it.js` & `bigsansar-2.6.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/it.js`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ja.js` & `bigsansar-2.6.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ja.js`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ko.js` & `bigsansar-2.6.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ko.js`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/nb.js` & `bigsansar-2.6.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/nb.js`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/nl.js` & `bigsansar-2.6.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/nl.js`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/nn.js` & `bigsansar-2.6.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/nn.js`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/pl.js` & `bigsansar-2.6.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/pl.js`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/pt-br.js` & `bigsansar-2.6.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/pt-br.js`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/pt.js` & `bigsansar-2.6.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/pt.js`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ru.js` & `bigsansar-2.6.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ru.js`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/sk.js` & `bigsansar-2.6.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/sk.js`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/tr.js` & `bigsansar-2.6.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/tr.js`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/uk.js` & `bigsansar-2.6.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/uk.js`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/vi.js` & `bigsansar-2.6.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/vi.js`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/zh.js` & `bigsansar-2.6.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/zh.js`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.3/bigsansar/static/ckeditor/ckeditor/plugins/youtube/plugin.js` & `bigsansar-2.6.4/bigsansar/static/ckeditor/ckeditor/plugins/youtube/plugin.js`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.3/bigsansar/static/logo.png` & `bigsansar-2.6.4/bigsansar/static/logo.png`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.3/bigsansar/static/style.css` & `bigsansar-2.6.4/bigsansar/static/style.css`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.3/bigsansar/templates/404.html` & `bigsansar-2.6.4/bigsansar/templates/404.html`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.3/bigsansar/templates/admin/account_info.html` & `bigsansar-2.6.4/bigsansar/templates/admin/account_info.html`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.3/bigsansar/templates/admin/admin_update.html` & `bigsansar-2.6.4/bigsansar/templates/admin/admin_update.html`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.3/bigsansar/templates/admin/cf_config.html` & `bigsansar-2.6.4/bigsansar/templates/admin/cf_config.html`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.3/bigsansar/templates/admin/chpass.html` & `bigsansar-2.6.4/bigsansar/templates/admin/chpass.html`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.3/bigsansar/templates/admin/chuname.html` & `bigsansar-2.6.4/bigsansar/templates/admin/chuname.html`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.3/bigsansar/templates/admin/cloudflare.html` & `bigsansar-2.6.4/bigsansar/templates/admin/cloudflare.html`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.3/bigsansar/templates/admin/create_domain.html` & `bigsansar-2.6.4/bigsansar/templates/admin/create_domain.html`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.3/bigsansar/templates/admin/db_cloudflare.html` & `bigsansar-2.6.4/bigsansar/templates/admin/db_cloudflare.html`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.3/bigsansar/templates/admin/domain_manage.html` & `bigsansar-2.6.4/bigsansar/templates/admin/domain_manage.html`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.3/bigsansar/templates/admin/edit_domain.html` & `bigsansar-2.6.4/bigsansar/templates/admin/edit_domain.html`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.3/bigsansar/templates/admin/editprofile.html` & `bigsansar-2.6.4/bigsansar/templates/admin/editprofile.html`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.3/bigsansar/templates/admin/login.html` & `bigsansar-2.6.4/bigsansar/templates/admin/login.html`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.3/bigsansar/templates/admin/nav.html` & `bigsansar-2.6.4/bigsansar/templates/admin/nav.html`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.3/bigsansar/templates/admin/page_create.html` & `bigsansar-2.6.4/bigsansar/templates/admin/page_create.html`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.3/bigsansar/templates/admin/page_delete.html` & `bigsansar-2.6.4/bigsansar/templates/admin/page_delete.html`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.3/bigsansar/templates/admin/page_edit.html` & `bigsansar-2.6.4/bigsansar/templates/admin/page_edit.html`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.3/bigsansar/templates/base.html` & `bigsansar-2.6.4/bigsansar/templates/base.html`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.3/bigsansar/templates/blog_preview.html` & `bigsansar-2.6.4/bigsansar/templates/blog_preview.html`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.3/bigsansar/templates/default.html` & `bigsansar-2.6.4/bigsansar/templates/default.html`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.3/bigsansar/templates/defaultpage.html` & `bigsansar-2.6.4/bigsansar/templates/defaultpage.html`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.3/bigsansar/templates/parking.html` & `bigsansar-2.6.4/bigsansar/templates/parking.html`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.3/bigsansar/urls.py` & `bigsansar-2.6.4/bigsansar/urls.py`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.3/bigsansar/views.py` & `bigsansar-2.6.4/bigsansar/views.py`

 * *Files identical despite different names*

### Comparing `bigsansar-2.6.3/setup.py` & `bigsansar-2.6.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="Bigsansar",
-    version="2.6.3",
+    version="2.6.4",
     author="Bikash Pokhrel",
     author_email="bigsansaroffice@gmail.com",
     description="Build one in minutes with bigsansar - a visual site building tool!",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/pokhrelb9/bigsansar",
     project_urls={
```

