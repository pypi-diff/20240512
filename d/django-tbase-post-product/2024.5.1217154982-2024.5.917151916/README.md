# Comparing `tmp/django_tbase_post_product-2024.5.1217154982.tar.gz` & `tmp/django_tbase_post_product-2024.5.917151916.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_tbase_post_product-2024.5.1217154982.tar", last modified: Sun May 12 07:16:48 2024, max compression
+gzip compressed data, was "django_tbase_post_product-2024.5.917151916.tar", last modified: Wed May  8 18:07:06 2024, max compression
```

## Comparing `django_tbase_post_product-2024.5.1217154982.tar` & `django_tbase_post_product-2024.5.917151916.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2024-05-12 07:16:48.852632 django_tbase_post_product-2024.5.1217154982/
--rw-rw-r--   0 terry     (1000) terry     (1000)      143 2023-12-03 08:49:22.000000 django_tbase_post_product-2024.5.1217154982/MANIFEST.in
--rw-rw-r--   0 terry     (1000) terry     (1000)     2093 2024-05-12 07:16:48.852632 django_tbase_post_product-2024.5.1217154982/PKG-INFO
--rw-rw-r--   0 terry     (1000) terry     (1000)     1770 2024-05-12 07:16:30.000000 django_tbase_post_product-2024.5.1217154982/README.md
-drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2024-05-12 07:16:48.844632 django_tbase_post_product-2024.5.1217154982/django_tbase_post_product.egg-info/
--rw-rw-r--   0 terry     (1000) terry     (1000)     2093 2024-05-12 07:16:48.000000 django_tbase_post_product-2024.5.1217154982/django_tbase_post_product.egg-info/PKG-INFO
--rw-rw-r--   0 terry     (1000) terry     (1000)     2634 2024-05-12 07:16:48.000000 django_tbase_post_product-2024.5.1217154982/django_tbase_post_product.egg-info/SOURCES.txt
--rw-rw-r--   0 terry     (1000) terry     (1000)        1 2024-05-12 07:16:48.000000 django_tbase_post_product-2024.5.1217154982/django_tbase_post_product.egg-info/dependency_links.txt
--rw-rw-r--   0 terry     (1000) terry     (1000)       83 2024-05-12 07:16:48.000000 django_tbase_post_product-2024.5.1217154982/django_tbase_post_product.egg-info/requires.txt
--rw-rw-r--   0 terry     (1000) terry     (1000)       11 2024-05-12 07:16:48.000000 django_tbase_post_product-2024.5.1217154982/django_tbase_post_product.egg-info/top_level.txt
--rw-rw-r--   0 terry     (1000) terry     (1000)       38 2024-05-12 07:16:48.852632 django_tbase_post_product-2024.5.1217154982/setup.cfg
--rw-rw-r--   0 terry     (1000) terry     (1000)     2305 2023-12-03 08:49:22.000000 django_tbase_post_product-2024.5.1217154982/setup.py
-drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2024-05-12 07:16:48.844632 django_tbase_post_product-2024.5.1217154982/tbase_post/
--rw-rw-r--   0 terry     (1000) terry     (1000)     7569 2024-03-12 15:28:36.000000 django_tbase_post_product-2024.5.1217154982/tbase_post/0001_initial.py
--rw-rw-r--   0 terry     (1000) terry     (1000)        0 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.1217154982/tbase_post/__init__.py
-drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2024-05-12 07:16:48.848632 django_tbase_post_product-2024.5.1217154982/tbase_post/__pycache__/
--rw-rw-r--   0 terry     (1000) terry     (1000)      183 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.1217154982/tbase_post/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 terry     (1000) terry     (1000)     4983 2024-03-13 03:45:26.000000 django_tbase_post_product-2024.5.1217154982/tbase_post/__pycache__/admin.cpython-310.pyc
--rw-rw-r--   0 terry     (1000) terry     (1000)      464 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.1217154982/tbase_post/__pycache__/apps.cpython-310.pyc
--rw-rw-r--   0 terry     (1000) terry     (1000)     7593 2024-04-13 13:06:34.000000 django_tbase_post_product-2024.5.1217154982/tbase_post/__pycache__/models.cpython-310.pyc
--rw-rw-r--   0 terry     (1000) terry     (1000)     1095 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.1217154982/tbase_post/__pycache__/sitemaps.cpython-310.pyc
--rw-rw-r--   0 terry     (1000) terry     (1000)      224 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.1217154982/tbase_post/__pycache__/tests.cpython-310.pyc
--rw-rw-r--   0 terry     (1000) terry     (1000)     1343 2024-03-13 03:17:26.000000 django_tbase_post_product-2024.5.1217154982/tbase_post/__pycache__/urls.cpython-310.pyc
--rw-rw-r--   0 terry     (1000) terry     (1000)     7307 2024-05-08 16:40:04.000000 django_tbase_post_product-2024.5.1217154982/tbase_post/__pycache__/views.cpython-310.pyc
--rw-rw-r--   0 terry     (1000) terry     (1000)     6331 2024-03-13 03:45:25.000000 django_tbase_post_product-2024.5.1217154982/tbase_post/admin.py
--rw-rw-r--   0 terry     (1000) terry     (1000)      146 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.1217154982/tbase_post/apps.py
-drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2024-05-12 07:16:48.848632 django_tbase_post_product-2024.5.1217154982/tbase_post/migrations/
--rw-rw-r--   0 terry     (1000) terry     (1000)     7576 2024-05-08 16:43:18.000000 django_tbase_post_product-2024.5.1217154982/tbase_post/migrations/0001_initial.py
--rw-rw-r--   0 terry     (1000) terry     (1000)        0 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.1217154982/tbase_post/migrations/__init__.py
-drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2024-05-12 07:16:48.848632 django_tbase_post_product-2024.5.1217154982/tbase_post/migrations/__pycache__/
--rw-rw-r--   0 terry     (1000) terry     (1000)     5196 2024-05-08 16:43:28.000000 django_tbase_post_product-2024.5.1217154982/tbase_post/migrations/__pycache__/0001_initial.cpython-310.pyc
--rw-rw-r--   0 terry     (1000) terry     (1000)      194 2024-05-08 16:43:17.000000 django_tbase_post_product-2024.5.1217154982/tbase_post/migrations/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 terry     (1000) terry     (1000)    10357 2024-04-13 13:06:33.000000 django_tbase_post_product-2024.5.1217154982/tbase_post/models.py
--rw-rw-r--   0 terry     (1000) terry     (1000)      616 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.1217154982/tbase_post/sitemaps.py
-drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2024-05-12 07:16:48.844632 django_tbase_post_product-2024.5.1217154982/tbase_post/static/
-drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2024-05-12 07:16:48.848632 django_tbase_post_product-2024.5.1217154982/tbase_post/static/images/
--rw-rw-r--   0 terry     (1000) terry     (1000)    59619 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.1217154982/tbase_post/static/images/photo-1578707399887-e6d183c9e598.jpeg
--rw-rw-r--   0 terry     (1000) terry     (1000)       94 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.1217154982/tbase_post/static/images/photo-1578707399887-e6d183c9e598.jpeg:Zone.Identifier
-drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2024-05-12 07:16:48.848632 django_tbase_post_product-2024.5.1217154982/tbase_post/templates/
-drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2024-05-12 07:16:48.848632 django_tbase_post_product-2024.5.1217154982/tbase_post/templates/post/
--rw-rw-r--   0 terry     (1000) terry     (1000)     5333 2024-05-08 16:49:53.000000 django_tbase_post_product-2024.5.1217154982/tbase_post/templates/post/article_list_by_tag.html
--rw-rw-r--   0 terry     (1000) terry     (1000)     3809 2024-05-08 17:11:30.000000 django_tbase_post_product-2024.5.1217154982/tbase_post/templates/post/blog_index.html
--rw-rw-r--   0 terry     (1000) terry     (1000)    11430 2024-05-12 07:15:30.000000 django_tbase_post_product-2024.5.1217154982/tbase_post/templates/post/detail.html
-drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2024-05-12 07:16:48.852632 django_tbase_post_product-2024.5.1217154982/tbase_post/templates/post/extras/
--rw-rw-r--   0 terry     (1000) terry     (1000)      732 2024-05-08 17:02:46.000000 django_tbase_post_product-2024.5.1217154982/tbase_post/templates/post/extras/amazon_ads.html
--rw-rw-r--   0 terry     (1000) terry     (1000)      516 2024-05-08 17:02:35.000000 django_tbase_post_product-2024.5.1217154982/tbase_post/templates/post/extras/amazon_link.html
--rw-rw-r--   0 terry     (1000) terry     (1000)      415 2024-05-08 17:45:22.000000 django_tbase_post_product-2024.5.1217154982/tbase_post/templates/post/extras/get_previous_next_by_pk.html
--rw-rw-r--   0 terry     (1000) terry     (1000)      884 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.1217154982/tbase_post/templates/post/extras/hitcount_lowest_post.html
--rw-rw-r--   0 terry     (1000) terry     (1000)      818 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.1217154982/tbase_post/templates/post/extras/hitcount_top_post.html
--rw-rw-r--   0 terry     (1000) terry     (1000)     1870 2024-05-08 17:02:18.000000 django_tbase_post_product-2024.5.1217154982/tbase_post/templates/post/extras/last_update.html
--rw-rw-r--   0 terry     (1000) terry     (1000)      970 2024-05-08 17:02:05.000000 django_tbase_post_product-2024.5.1217154982/tbase_post/templates/post/extras/related_post_by_tags.html
--rw-rw-r--   0 terry     (1000) terry     (1000)      404 2024-05-08 16:54:27.000000 django_tbase_post_product-2024.5.1217154982/tbase_post/templates/post/extras/related_post_by_tags_mini.html
--rw-rw-r--   0 terry     (1000) terry     (1000)      827 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.1217154982/tbase_post/templates/post/extras/seo_top_links.html
--rw-rw-r--   0 terry     (1000) terry     (1000)      509 2024-05-08 17:00:09.000000 django_tbase_post_product-2024.5.1217154982/tbase_post/templates/post/extras/tags.html
--rw-rw-r--   0 terry     (1000) terry     (1000)      132 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.1217154982/tbase_post/templates/post/extras/templ.html
--rw-rw-r--   0 terry     (1000) terry     (1000)      576 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.1217154982/tbase_post/templates/post/extras/youtube_player.html
--rw-rw-r--   0 terry     (1000) terry     (1000)     2109 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.1217154982/tbase_post/templates/post/last_index.html
--rw-rw-r--   0 terry     (1000) terry     (1000)      255 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.1217154982/tbase_post/templates/post/prompt_task_detail copy.html
--rw-rw-r--   0 terry     (1000) terry     (1000)     4751 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.1217154982/tbase_post/templates/post/prompt_task_detail.html
--rw-rw-r--   0 terry     (1000) terry     (1000)      426 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.1217154982/tbase_post/templates/post/prompt_task_list.html
--rw-rw-r--   0 terry     (1000) terry     (1000)     2483 2024-03-13 03:47:25.000000 django_tbase_post_product-2024.5.1217154982/tbase_post/templates/post/prompt_task_post_detail.html
--rw-rw-r--   0 terry     (1000) terry     (1000)     4733 2024-03-13 03:36:27.000000 django_tbase_post_product-2024.5.1217154982/tbase_post/templates/post/prompt_task_post_list.html
--rw-rw-r--   0 terry     (1000) terry     (1000)      765 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.1217154982/tbase_post/templates/post_list.html
--rw-rw-r--   0 terry     (1000) terry     (1000)      391 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.1217154982/tbase_post/templates/sitemap.xml
-drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2024-05-12 07:16:48.852632 django_tbase_post_product-2024.5.1217154982/tbase_post/templatetags/
--rw-rw-r--   0 terry     (1000) terry     (1000)        0 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.1217154982/tbase_post/templatetags/__init__.py
-drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2024-05-12 07:16:48.852632 django_tbase_post_product-2024.5.1217154982/tbase_post/templatetags/__pycache__/
--rw-rw-r--   0 terry     (1000) terry     (1000)      196 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.1217154982/tbase_post/templatetags/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 terry     (1000) terry     (1000)      190 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.1217154982/tbase_post/templatetags/__pycache__/__init__.cpython-39.pyc
--rw-rw-r--   0 terry     (1000) terry     (1000)     6516 2024-05-08 16:31:29.000000 django_tbase_post_product-2024.5.1217154982/tbase_post/templatetags/__pycache__/post_extras.cpython-310.pyc
--rw-rw-r--   0 terry     (1000) terry     (1000)     4111 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.1217154982/tbase_post/templatetags/__pycache__/post_extras.cpython-39.pyc
--rw-rw-r--   0 terry     (1000) terry     (1000)    14032 2024-05-08 17:56:02.000000 django_tbase_post_product-2024.5.1217154982/tbase_post/templatetags/post_extras.py
--rw-rw-r--   0 terry     (1000) terry     (1000)       60 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.1217154982/tbase_post/tests.py
--rw-rw-r--   0 terry     (1000) terry     (1000)     1571 2024-03-13 03:17:25.000000 django_tbase_post_product-2024.5.1217154982/tbase_post/urls.py
--rw-rw-r--   0 terry     (1000) terry     (1000)    11938 2024-05-08 16:40:03.000000 django_tbase_post_product-2024.5.1217154982/tbase_post/views.py
+drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2024-05-08 18:07:06.354907 django_tbase_post_product-2024.5.917151916/
+-rw-rw-r--   0 terry     (1000) terry     (1000)      143 2023-12-03 08:49:22.000000 django_tbase_post_product-2024.5.917151916/MANIFEST.in
+-rw-rw-r--   0 terry     (1000) terry     (1000)     2030 2024-05-08 18:07:06.354907 django_tbase_post_product-2024.5.917151916/PKG-INFO
+-rw-rw-r--   0 terry     (1000) terry     (1000)     1708 2024-05-08 18:06:59.000000 django_tbase_post_product-2024.5.917151916/README.md
+drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2024-05-08 18:07:06.346907 django_tbase_post_product-2024.5.917151916/django_tbase_post_product.egg-info/
+-rw-rw-r--   0 terry     (1000) terry     (1000)     2030 2024-05-08 18:07:06.000000 django_tbase_post_product-2024.5.917151916/django_tbase_post_product.egg-info/PKG-INFO
+-rw-rw-r--   0 terry     (1000) terry     (1000)     2634 2024-05-08 18:07:06.000000 django_tbase_post_product-2024.5.917151916/django_tbase_post_product.egg-info/SOURCES.txt
+-rw-rw-r--   0 terry     (1000) terry     (1000)        1 2024-05-08 18:07:06.000000 django_tbase_post_product-2024.5.917151916/django_tbase_post_product.egg-info/dependency_links.txt
+-rw-rw-r--   0 terry     (1000) terry     (1000)       83 2024-05-08 18:07:06.000000 django_tbase_post_product-2024.5.917151916/django_tbase_post_product.egg-info/requires.txt
+-rw-rw-r--   0 terry     (1000) terry     (1000)       11 2024-05-08 18:07:06.000000 django_tbase_post_product-2024.5.917151916/django_tbase_post_product.egg-info/top_level.txt
+-rw-rw-r--   0 terry     (1000) terry     (1000)       38 2024-05-08 18:07:06.354907 django_tbase_post_product-2024.5.917151916/setup.cfg
+-rw-rw-r--   0 terry     (1000) terry     (1000)     2305 2023-12-03 08:49:22.000000 django_tbase_post_product-2024.5.917151916/setup.py
+drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2024-05-08 18:07:06.350907 django_tbase_post_product-2024.5.917151916/tbase_post/
+-rw-rw-r--   0 terry     (1000) terry     (1000)     7569 2024-03-12 15:28:36.000000 django_tbase_post_product-2024.5.917151916/tbase_post/0001_initial.py
+-rw-rw-r--   0 terry     (1000) terry     (1000)        0 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.917151916/tbase_post/__init__.py
+drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2024-05-08 18:07:06.350907 django_tbase_post_product-2024.5.917151916/tbase_post/__pycache__/
+-rw-rw-r--   0 terry     (1000) terry     (1000)      183 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.917151916/tbase_post/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 terry     (1000) terry     (1000)     4983 2024-03-13 03:45:26.000000 django_tbase_post_product-2024.5.917151916/tbase_post/__pycache__/admin.cpython-310.pyc
+-rw-rw-r--   0 terry     (1000) terry     (1000)      464 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.917151916/tbase_post/__pycache__/apps.cpython-310.pyc
+-rw-rw-r--   0 terry     (1000) terry     (1000)     7593 2024-04-13 13:06:34.000000 django_tbase_post_product-2024.5.917151916/tbase_post/__pycache__/models.cpython-310.pyc
+-rw-rw-r--   0 terry     (1000) terry     (1000)     1095 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.917151916/tbase_post/__pycache__/sitemaps.cpython-310.pyc
+-rw-rw-r--   0 terry     (1000) terry     (1000)      224 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.917151916/tbase_post/__pycache__/tests.cpython-310.pyc
+-rw-rw-r--   0 terry     (1000) terry     (1000)     1343 2024-03-13 03:17:26.000000 django_tbase_post_product-2024.5.917151916/tbase_post/__pycache__/urls.cpython-310.pyc
+-rw-rw-r--   0 terry     (1000) terry     (1000)     7307 2024-05-08 16:40:04.000000 django_tbase_post_product-2024.5.917151916/tbase_post/__pycache__/views.cpython-310.pyc
+-rw-rw-r--   0 terry     (1000) terry     (1000)     6331 2024-03-13 03:45:25.000000 django_tbase_post_product-2024.5.917151916/tbase_post/admin.py
+-rw-rw-r--   0 terry     (1000) terry     (1000)      146 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.917151916/tbase_post/apps.py
+drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2024-05-08 18:07:06.350907 django_tbase_post_product-2024.5.917151916/tbase_post/migrations/
+-rw-rw-r--   0 terry     (1000) terry     (1000)     7576 2024-05-08 16:43:18.000000 django_tbase_post_product-2024.5.917151916/tbase_post/migrations/0001_initial.py
+-rw-rw-r--   0 terry     (1000) terry     (1000)        0 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.917151916/tbase_post/migrations/__init__.py
+drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2024-05-08 18:07:06.350907 django_tbase_post_product-2024.5.917151916/tbase_post/migrations/__pycache__/
+-rw-rw-r--   0 terry     (1000) terry     (1000)     5196 2024-05-08 16:43:28.000000 django_tbase_post_product-2024.5.917151916/tbase_post/migrations/__pycache__/0001_initial.cpython-310.pyc
+-rw-rw-r--   0 terry     (1000) terry     (1000)      194 2024-05-08 16:43:17.000000 django_tbase_post_product-2024.5.917151916/tbase_post/migrations/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 terry     (1000) terry     (1000)    10357 2024-04-13 13:06:33.000000 django_tbase_post_product-2024.5.917151916/tbase_post/models.py
+-rw-rw-r--   0 terry     (1000) terry     (1000)      616 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.917151916/tbase_post/sitemaps.py
+drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2024-05-08 18:07:06.346907 django_tbase_post_product-2024.5.917151916/tbase_post/static/
+drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2024-05-08 18:07:06.350907 django_tbase_post_product-2024.5.917151916/tbase_post/static/images/
+-rw-rw-r--   0 terry     (1000) terry     (1000)    59619 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.917151916/tbase_post/static/images/photo-1578707399887-e6d183c9e598.jpeg
+-rw-rw-r--   0 terry     (1000) terry     (1000)       94 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.917151916/tbase_post/static/images/photo-1578707399887-e6d183c9e598.jpeg:Zone.Identifier
+drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2024-05-08 18:07:06.350907 django_tbase_post_product-2024.5.917151916/tbase_post/templates/
+drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2024-05-08 18:07:06.350907 django_tbase_post_product-2024.5.917151916/tbase_post/templates/post/
+-rw-rw-r--   0 terry     (1000) terry     (1000)     5333 2024-05-08 16:49:53.000000 django_tbase_post_product-2024.5.917151916/tbase_post/templates/post/article_list_by_tag.html
+-rw-rw-r--   0 terry     (1000) terry     (1000)     3809 2024-05-08 17:11:30.000000 django_tbase_post_product-2024.5.917151916/tbase_post/templates/post/blog_index.html
+-rw-rw-r--   0 terry     (1000) terry     (1000)    11424 2024-05-08 17:47:08.000000 django_tbase_post_product-2024.5.917151916/tbase_post/templates/post/detail.html
+drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2024-05-08 18:07:06.354907 django_tbase_post_product-2024.5.917151916/tbase_post/templates/post/extras/
+-rw-rw-r--   0 terry     (1000) terry     (1000)      732 2024-05-08 17:02:46.000000 django_tbase_post_product-2024.5.917151916/tbase_post/templates/post/extras/amazon_ads.html
+-rw-rw-r--   0 terry     (1000) terry     (1000)      516 2024-05-08 17:02:35.000000 django_tbase_post_product-2024.5.917151916/tbase_post/templates/post/extras/amazon_link.html
+-rw-rw-r--   0 terry     (1000) terry     (1000)      415 2024-05-08 17:45:22.000000 django_tbase_post_product-2024.5.917151916/tbase_post/templates/post/extras/get_previous_next_by_pk.html
+-rw-rw-r--   0 terry     (1000) terry     (1000)      884 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.917151916/tbase_post/templates/post/extras/hitcount_lowest_post.html
+-rw-rw-r--   0 terry     (1000) terry     (1000)      818 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.917151916/tbase_post/templates/post/extras/hitcount_top_post.html
+-rw-rw-r--   0 terry     (1000) terry     (1000)     1870 2024-05-08 17:02:18.000000 django_tbase_post_product-2024.5.917151916/tbase_post/templates/post/extras/last_update.html
+-rw-rw-r--   0 terry     (1000) terry     (1000)      970 2024-05-08 17:02:05.000000 django_tbase_post_product-2024.5.917151916/tbase_post/templates/post/extras/related_post_by_tags.html
+-rw-rw-r--   0 terry     (1000) terry     (1000)      404 2024-05-08 16:54:27.000000 django_tbase_post_product-2024.5.917151916/tbase_post/templates/post/extras/related_post_by_tags_mini.html
+-rw-rw-r--   0 terry     (1000) terry     (1000)      827 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.917151916/tbase_post/templates/post/extras/seo_top_links.html
+-rw-rw-r--   0 terry     (1000) terry     (1000)      509 2024-05-08 17:00:09.000000 django_tbase_post_product-2024.5.917151916/tbase_post/templates/post/extras/tags.html
+-rw-rw-r--   0 terry     (1000) terry     (1000)      132 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.917151916/tbase_post/templates/post/extras/templ.html
+-rw-rw-r--   0 terry     (1000) terry     (1000)      576 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.917151916/tbase_post/templates/post/extras/youtube_player.html
+-rw-rw-r--   0 terry     (1000) terry     (1000)     2109 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.917151916/tbase_post/templates/post/last_index.html
+-rw-rw-r--   0 terry     (1000) terry     (1000)      255 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.917151916/tbase_post/templates/post/prompt_task_detail copy.html
+-rw-rw-r--   0 terry     (1000) terry     (1000)     4751 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.917151916/tbase_post/templates/post/prompt_task_detail.html
+-rw-rw-r--   0 terry     (1000) terry     (1000)      426 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.917151916/tbase_post/templates/post/prompt_task_list.html
+-rw-rw-r--   0 terry     (1000) terry     (1000)     2483 2024-03-13 03:47:25.000000 django_tbase_post_product-2024.5.917151916/tbase_post/templates/post/prompt_task_post_detail.html
+-rw-rw-r--   0 terry     (1000) terry     (1000)     4733 2024-03-13 03:36:27.000000 django_tbase_post_product-2024.5.917151916/tbase_post/templates/post/prompt_task_post_list.html
+-rw-rw-r--   0 terry     (1000) terry     (1000)      765 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.917151916/tbase_post/templates/post_list.html
+-rw-rw-r--   0 terry     (1000) terry     (1000)      391 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.917151916/tbase_post/templates/sitemap.xml
+drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2024-05-08 18:07:06.354907 django_tbase_post_product-2024.5.917151916/tbase_post/templatetags/
+-rw-rw-r--   0 terry     (1000) terry     (1000)        0 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.917151916/tbase_post/templatetags/__init__.py
+drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2024-05-08 18:07:06.354907 django_tbase_post_product-2024.5.917151916/tbase_post/templatetags/__pycache__/
+-rw-rw-r--   0 terry     (1000) terry     (1000)      196 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.917151916/tbase_post/templatetags/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 terry     (1000) terry     (1000)      190 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.917151916/tbase_post/templatetags/__pycache__/__init__.cpython-39.pyc
+-rw-rw-r--   0 terry     (1000) terry     (1000)     6516 2024-05-08 16:31:29.000000 django_tbase_post_product-2024.5.917151916/tbase_post/templatetags/__pycache__/post_extras.cpython-310.pyc
+-rw-rw-r--   0 terry     (1000) terry     (1000)     4111 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.917151916/tbase_post/templatetags/__pycache__/post_extras.cpython-39.pyc
+-rw-rw-r--   0 terry     (1000) terry     (1000)    14032 2024-05-08 17:56:02.000000 django_tbase_post_product-2024.5.917151916/tbase_post/templatetags/post_extras.py
+-rw-rw-r--   0 terry     (1000) terry     (1000)       60 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.917151916/tbase_post/tests.py
+-rw-rw-r--   0 terry     (1000) terry     (1000)     1571 2024-03-13 03:17:25.000000 django_tbase_post_product-2024.5.917151916/tbase_post/urls.py
+-rw-rw-r--   0 terry     (1000) terry     (1000)    11938 2024-05-08 16:40:03.000000 django_tbase_post_product-2024.5.917151916/tbase_post/views.py
```

### Comparing `django_tbase_post_product-2024.5.1217154982/PKG-INFO` & `django_tbase_post_product-2024.5.917151916/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django_tbase_post_product
-Version: 2024.5.1217154982
+Version: 2024.5.917151916
 Summary: Terry django base post ,
 Home-page: https://terrychanorg.jetbrains.space/p/django-expand/repositories/tbase_post_product/files/README.md
 Author: Terry Chan
 Author-email: napoler2008@gmail.com
 Description-Content-Type: text/markdown
 
 # django-expand/tbase_post_product
@@ -32,18 +32,15 @@
     'taggit',
 
  ]
 ```
 
 
 ## 更新
-- 2024/05/12
-注销掉底部广告（banner-amazon-footer）
-
-- 2024/05/9
+- 2024/05/1
 优化内部链接，增加相关链接和上下文链接
 - 2024/05/1
 注销掉底部广告（banner-amazon-footer）
 
 
 - 2024/04/13
 优化展示
```

### Comparing `django_tbase_post_product-2024.5.1217154982/README.md` & `django_tbase_post_product-2024.5.917151916/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -23,18 +23,15 @@
     'taggit',
 
  ]
 ```
 
 
 ## 更新
-- 2024/05/12
-注销掉底部广告（banner-amazon-footer）
-
-- 2024/05/9
+- 2024/05/1
 优化内部链接，增加相关链接和上下文链接
 - 2024/05/1
 注销掉底部广告（banner-amazon-footer）
 
 
 - 2024/04/13
 优化展示
```

### Comparing `django_tbase_post_product-2024.5.1217154982/django_tbase_post_product.egg-info/PKG-INFO` & `django_tbase_post_product-2024.5.917151916/django_tbase_post_product.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-tbase-post-product
-Version: 2024.5.1217154982
+Version: 2024.5.917151916
 Summary: Terry django base post ,
 Home-page: https://terrychanorg.jetbrains.space/p/django-expand/repositories/tbase_post_product/files/README.md
 Author: Terry Chan
 Author-email: napoler2008@gmail.com
 Description-Content-Type: text/markdown
 
 # django-expand/tbase_post_product
@@ -32,18 +32,15 @@
     'taggit',
 
  ]
 ```
 
 
 ## 更新
-- 2024/05/12
-注销掉底部广告（banner-amazon-footer）
-
-- 2024/05/9
+- 2024/05/1
 优化内部链接，增加相关链接和上下文链接
 - 2024/05/1
 注销掉底部广告（banner-amazon-footer）
 
 
 - 2024/04/13
 优化展示
```

### Comparing `django_tbase_post_product-2024.5.1217154982/django_tbase_post_product.egg-info/SOURCES.txt` & `django_tbase_post_product-2024.5.917151916/django_tbase_post_product.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2024.5.1217154982/setup.py` & `django_tbase_post_product-2024.5.917151916/setup.py`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2024.5.1217154982/tbase_post/0001_initial.py` & `django_tbase_post_product-2024.5.917151916/tbase_post/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2024.5.1217154982/tbase_post/__pycache__/admin.cpython-310.pyc` & `django_tbase_post_product-2024.5.917151916/tbase_post/__pycache__/admin.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2024.5.1217154982/tbase_post/__pycache__/models.cpython-310.pyc` & `django_tbase_post_product-2024.5.917151916/tbase_post/__pycache__/models.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2024.5.1217154982/tbase_post/__pycache__/sitemaps.cpython-310.pyc` & `django_tbase_post_product-2024.5.917151916/tbase_post/__pycache__/sitemaps.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2024.5.1217154982/tbase_post/__pycache__/urls.cpython-310.pyc` & `django_tbase_post_product-2024.5.917151916/tbase_post/__pycache__/urls.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2024.5.1217154982/tbase_post/__pycache__/views.cpython-310.pyc` & `django_tbase_post_product-2024.5.917151916/tbase_post/__pycache__/views.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2024.5.1217154982/tbase_post/admin.py` & `django_tbase_post_product-2024.5.917151916/tbase_post/admin.py`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2024.5.1217154982/tbase_post/migrations/0001_initial.py` & `django_tbase_post_product-2024.5.917151916/tbase_post/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2024.5.1217154982/tbase_post/migrations/__pycache__/0001_initial.cpython-310.pyc` & `django_tbase_post_product-2024.5.917151916/tbase_post/migrations/__pycache__/0001_initial.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2024.5.1217154982/tbase_post/models.py` & `django_tbase_post_product-2024.5.917151916/tbase_post/models.py`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2024.5.1217154982/tbase_post/sitemaps.py` & `django_tbase_post_product-2024.5.917151916/tbase_post/sitemaps.py`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2024.5.1217154982/tbase_post/static/images/photo-1578707399887-e6d183c9e598.jpeg` & `django_tbase_post_product-2024.5.917151916/tbase_post/static/images/photo-1578707399887-e6d183c9e598.jpeg`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2024.5.1217154982/tbase_post/templates/post/article_list_by_tag.html` & `django_tbase_post_product-2024.5.917151916/tbase_post/templates/post/article_list_by_tag.html`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2024.5.1217154982/tbase_post/templates/post/blog_index.html` & `django_tbase_post_product-2024.5.917151916/tbase_post/templates/post/blog_index.html`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2024.5.1217154982/tbase_post/templates/post/detail.html` & `django_tbase_post_product-2024.5.917151916/tbase_post/templates/post/detail.html`

 * *Files 0% similar despite different names*

```diff
@@ -334,16 +334,16 @@
 var htmlStr = template('banner-amazon-tpl', data)
 $('#banner-amazon').html(htmlStr)
 
 data={}
 var htmlStr = template('banner-img-tpl', data)
 $('#banner-img').html(htmlStr)
 data={}
-// var htmlStr = template('banner-amazon-footer-tpl', data)
-// $('#banner-amazon-footer').html(htmlStr)
+var htmlStr = template('banner-amazon-footer-tpl', data)
+$('#banner-amazon-footer').html(htmlStr)
 
 </script>
 
  
 <!--标签-->
 {% tags object.tags 5 object.pk %}
  <!--标签end-->
```

### Comparing `django_tbase_post_product-2024.5.1217154982/tbase_post/templates/post/extras/amazon_ads.html` & `django_tbase_post_product-2024.5.917151916/tbase_post/templates/post/extras/amazon_ads.html`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2024.5.1217154982/tbase_post/templates/post/extras/amazon_link.html` & `django_tbase_post_product-2024.5.917151916/tbase_post/templates/post/extras/amazon_link.html`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2024.5.1217154982/tbase_post/templates/post/extras/hitcount_lowest_post.html` & `django_tbase_post_product-2024.5.917151916/tbase_post/templates/post/extras/hitcount_lowest_post.html`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2024.5.1217154982/tbase_post/templates/post/extras/hitcount_top_post.html` & `django_tbase_post_product-2024.5.917151916/tbase_post/templates/post/extras/hitcount_top_post.html`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2024.5.1217154982/tbase_post/templates/post/extras/last_update.html` & `django_tbase_post_product-2024.5.917151916/tbase_post/templates/post/extras/last_update.html`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2024.5.1217154982/tbase_post/templates/post/extras/related_post_by_tags.html` & `django_tbase_post_product-2024.5.917151916/tbase_post/templates/post/extras/related_post_by_tags.html`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2024.5.1217154982/tbase_post/templates/post/extras/seo_top_links.html` & `django_tbase_post_product-2024.5.917151916/tbase_post/templates/post/extras/seo_top_links.html`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2024.5.1217154982/tbase_post/templates/post/extras/youtube_player.html` & `django_tbase_post_product-2024.5.917151916/tbase_post/templates/post/extras/youtube_player.html`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2024.5.1217154982/tbase_post/templates/post/last_index.html` & `django_tbase_post_product-2024.5.917151916/tbase_post/templates/post/last_index.html`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2024.5.1217154982/tbase_post/templates/post/prompt_task_detail.html` & `django_tbase_post_product-2024.5.917151916/tbase_post/templates/post/prompt_task_detail.html`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2024.5.1217154982/tbase_post/templates/post/prompt_task_post_detail.html` & `django_tbase_post_product-2024.5.917151916/tbase_post/templates/post/prompt_task_post_detail.html`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2024.5.1217154982/tbase_post/templates/post/prompt_task_post_list.html` & `django_tbase_post_product-2024.5.917151916/tbase_post/templates/post/prompt_task_post_list.html`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2024.5.1217154982/tbase_post/templates/post_list.html` & `django_tbase_post_product-2024.5.917151916/tbase_post/templates/post_list.html`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2024.5.1217154982/tbase_post/templatetags/__pycache__/post_extras.cpython-310.pyc` & `django_tbase_post_product-2024.5.917151916/tbase_post/templatetags/__pycache__/post_extras.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2024.5.1217154982/tbase_post/templatetags/__pycache__/post_extras.cpython-39.pyc` & `django_tbase_post_product-2024.5.917151916/tbase_post/templatetags/__pycache__/post_extras.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2024.5.1217154982/tbase_post/templatetags/post_extras.py` & `django_tbase_post_product-2024.5.917151916/tbase_post/templatetags/post_extras.py`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2024.5.1217154982/tbase_post/urls.py` & `django_tbase_post_product-2024.5.917151916/tbase_post/urls.py`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2024.5.1217154982/tbase_post/views.py` & `django_tbase_post_product-2024.5.917151916/tbase_post/views.py`

 * *Files identical despite different names*

