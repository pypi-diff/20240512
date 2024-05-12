# Comparing `tmp/django_easy_faq-1.8.tar.gz` & `tmp/django_easy_faq-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_easy_faq-1.8.tar", last modified: Thu May  9 01:25:33 2024, max compression
+gzip compressed data, was "django_easy_faq-1.9.tar", last modified: Sun May 12 19:20:31 2024, max compression
```

## Comparing `django_easy_faq-1.8.tar` & `django_easy_faq-1.9.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 01:25:33.007723 django_easy_faq-1.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-09 01:25:29.000000 django_easy_faq-1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-09 01:25:29.000000 django_easy_faq-1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    16054 2024-05-09 01:25:33.007723 django_easy_faq-1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15246 2024-05-09 01:25:29.000000 django_easy_faq-1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 01:25:33.003723 django_easy_faq-1.8/django_easy_faq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16054 2024-05-09 01:25:32.000000 django_easy_faq-1.8/django_easy_faq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-09 01:25:32.000000 django_easy_faq-1.8/django_easy_faq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 01:25:32.000000 django_easy_faq-1.8/django_easy_faq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-09 01:25:32.000000 django_easy_faq-1.8/django_easy_faq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-09 01:25:32.000000 django_easy_faq-1.8/django_easy_faq.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 01:25:33.003723 django_easy_faq-1.8/faq/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-09 01:25:29.000000 django_easy_faq-1.8/faq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-05-09 01:25:29.000000 django_easy_faq-1.8/faq/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-09 01:25:29.000000 django_easy_faq-1.8/faq/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-05-09 01:25:29.000000 django_easy_faq-1.8/faq/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 01:25:33.003723 django_easy_faq-1.8/faq/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     4124 2024-05-09 01:25:29.000000 django_easy_faq-1.8/faq/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-05-09 01:25:29.000000 django_easy_faq-1.8/faq/migrations/0002_alter_answer_id_alter_answerhelpful_id_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-09 01:25:29.000000 django_easy_faq-1.8/faq/migrations/0003_auto_20220619_0939.py
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-09 01:25:29.000000 django_easy_faq-1.8/faq/migrations/0004_alter_answer_slug_alter_category_slug.py
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-09 01:25:29.000000 django_easy_faq-1.8/faq/migrations/0005_rename_description_category__description.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-09 01:25:29.000000 django_easy_faq-1.8/faq/migrations/0006_answer_is_rich_text.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 01:25:29.000000 django_easy_faq-1.8/faq/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4859 2024-05-09 01:25:29.000000 django_easy_faq-1.8/faq/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-09 01:25:29.000000 django_easy_faq-1.8/faq/path_converters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-05-09 01:25:29.000000 django_easy_faq-1.8/faq/snippets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 01:25:32.999723 django_easy_faq-1.8/faq/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 01:25:33.003723 django_easy_faq-1.8/faq/templates/faq/
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-09 01:25:29.000000 django_easy_faq-1.8/faq/templates/faq/answer_form.html
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-09 01:25:29.000000 django_easy_faq-1.8/faq/templates/faq/base.html
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-09 01:25:29.000000 django_easy_faq-1.8/faq/templates/faq/categories_list.html
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-09 01:25:29.000000 django_easy_faq-1.8/faq/templates/faq/category_detail.html
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-09 01:25:29.000000 django_easy_faq-1.8/faq/templates/faq/comment_form.html
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-09 01:25:29.000000 django_easy_faq-1.8/faq/templates/faq/comments.html
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-09 01:25:29.000000 django_easy_faq-1.8/faq/templates/faq/question_base.html
--rw-r--r--   0 runner    (1001) docker     (127)     3103 2024-05-09 01:25:29.000000 django_easy_faq-1.8/faq/templates/faq/question_detail.html
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-09 01:25:29.000000 django_easy_faq-1.8/faq/templates/faq/question_form.html
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-09 01:25:29.000000 django_easy_faq-1.8/faq/templates/faq/questions_list.html
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-09 01:25:29.000000 django_easy_faq-1.8/faq/templates/faq/vote_form.html
--rw-r--r--   0 runner    (1001) docker     (127)     7539 2024-05-09 01:25:29.000000 django_easy_faq-1.8/faq/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     2879 2024-05-09 01:25:29.000000 django_easy_faq-1.8/faq/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)    12843 2024-05-09 01:25:29.000000 django_easy_faq-1.8/faq/views.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 01:25:33.007723 django_easy_faq-1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-05-09 01:25:29.000000 django_easy_faq-1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:20:31.482010 django_easy_faq-1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-12 19:20:27.000000 django_easy_faq-1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-12 19:20:27.000000 django_easy_faq-1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    16124 2024-05-12 19:20:31.482010 django_easy_faq-1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15317 2024-05-12 19:20:27.000000 django_easy_faq-1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:20:31.482010 django_easy_faq-1.9/django_easy_faq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16124 2024-05-12 19:20:31.000000 django_easy_faq-1.9/django_easy_faq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-12 19:20:31.000000 django_easy_faq-1.9/django_easy_faq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 19:20:31.000000 django_easy_faq-1.9/django_easy_faq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-12 19:20:31.000000 django_easy_faq-1.9/django_easy_faq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-12 19:20:31.000000 django_easy_faq-1.9/django_easy_faq.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:20:31.478010 django_easy_faq-1.9/faq/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-12 19:20:27.000000 django_easy_faq-1.9/faq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3506 2024-05-12 19:20:27.000000 django_easy_faq-1.9/faq/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-12 19:20:27.000000 django_easy_faq-1.9/faq/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-05-12 19:20:27.000000 django_easy_faq-1.9/faq/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:20:31.482010 django_easy_faq-1.9/faq/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     4124 2024-05-12 19:20:27.000000 django_easy_faq-1.9/faq/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-05-12 19:20:27.000000 django_easy_faq-1.9/faq/migrations/0002_alter_answer_id_alter_answerhelpful_id_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-12 19:20:27.000000 django_easy_faq-1.9/faq/migrations/0003_auto_20220619_0939.py
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-12 19:20:27.000000 django_easy_faq-1.9/faq/migrations/0004_alter_answer_slug_alter_category_slug.py
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-12 19:20:27.000000 django_easy_faq-1.9/faq/migrations/0005_rename_description_category__description.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-12 19:20:27.000000 django_easy_faq-1.9/faq/migrations/0006_answer_is_rich_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 19:20:27.000000 django_easy_faq-1.9/faq/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6242 2024-05-12 19:20:27.000000 django_easy_faq-1.9/faq/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-12 19:20:27.000000 django_easy_faq-1.9/faq/path_converters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-05-12 19:20:27.000000 django_easy_faq-1.9/faq/snippets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:20:31.478010 django_easy_faq-1.9/faq/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:20:31.482010 django_easy_faq-1.9/faq/templates/faq/
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-12 19:20:27.000000 django_easy_faq-1.9/faq/templates/faq/answer_form.html
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-12 19:20:27.000000 django_easy_faq-1.9/faq/templates/faq/base.html
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-12 19:20:27.000000 django_easy_faq-1.9/faq/templates/faq/categories_list.html
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-12 19:20:27.000000 django_easy_faq-1.9/faq/templates/faq/category_detail.html
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-12 19:20:27.000000 django_easy_faq-1.9/faq/templates/faq/comment_form.html
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-12 19:20:27.000000 django_easy_faq-1.9/faq/templates/faq/comments.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-12 19:20:27.000000 django_easy_faq-1.9/faq/templates/faq/question_base.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3103 2024-05-12 19:20:27.000000 django_easy_faq-1.9/faq/templates/faq/question_detail.html
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-12 19:20:27.000000 django_easy_faq-1.9/faq/templates/faq/question_form.html
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-12 19:20:27.000000 django_easy_faq-1.9/faq/templates/faq/questions_list.html
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-12 19:20:27.000000 django_easy_faq-1.9/faq/templates/faq/vote_form.html
+-rw-r--r--   0 runner    (1001) docker     (127)     7539 2024-05-12 19:20:27.000000 django_easy_faq-1.9/faq/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2879 2024-05-12 19:20:27.000000 django_easy_faq-1.9/faq/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12843 2024-05-12 19:20:27.000000 django_easy_faq-1.9/faq/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 19:20:31.482010 django_easy_faq-1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-05-12 19:20:27.000000 django_easy_faq-1.9/setup.py
```

### Comparing `django_easy_faq-1.8/LICENSE` & `django_easy_faq-1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `django_easy_faq-1.8/PKG-INFO` & `django_easy_faq-1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-easy-faq
-Version: 1.8
+Version: 1.9
 Summary: A Django app to add great FAQ functionality to website
 Home-page: https://github.com/smark-1/django-easy-faq/
 Download-URL: https://pypi.python.org/pypi/django-easy-faq
 License: MIT
 Keywords: django,faq
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -369,18 +369,20 @@
 
 1.0 added pypi distribution
 
 1.1 added more templates to override easily
 
 1.2 fixed bug in pypi distro not including faq app
 
-1.3 fixed bug where a slug must be filled out in admin even though slug gets auto generated to save for questions, answers, and categories. made questions, answers, categories slugs readonly in admin
+1.3 fixed bug where a slug must be filled out in admin even though slug gets auto generated to save for questions, answers, and categories. Made questions, answers, categories slugs readonly in admin
 
 1.4 added unicode option to add unicode slugs
 
 1.5 added login_required setting to allow faq app to be available to only logged in users
 
 1.6 fixed bug where no_category_description did not do remove the category description in the admin
 
 1.7 added support for django 5.0
 
 1.8 added support for richtext answers with django-tinymce
+
+1.9 added view onsite link in admin, added richtext answers in admin
```

### Comparing `django_easy_faq-1.8/README.md` & `django_easy_faq-1.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -347,18 +347,20 @@
 
 1.0 added pypi distribution
 
 1.1 added more templates to override easily
 
 1.2 fixed bug in pypi distro not including faq app
 
-1.3 fixed bug where a slug must be filled out in admin even though slug gets auto generated to save for questions, answers, and categories. made questions, answers, categories slugs readonly in admin
+1.3 fixed bug where a slug must be filled out in admin even though slug gets auto generated to save for questions, answers, and categories. Made questions, answers, categories slugs readonly in admin
 
 1.4 added unicode option to add unicode slugs
 
 1.5 added login_required setting to allow faq app to be available to only logged in users
 
 1.6 fixed bug where no_category_description did not do remove the category description in the admin
 
 1.7 added support for django 5.0
 
-1.8 added support for richtext answers with django-tinymce
+1.8 added support for richtext answers with django-tinymce
+
+1.9 added view onsite link in admin, added richtext answers in admin
```

#### html2text {}

```diff
@@ -163,13 +163,14 @@
 django-easy-faq aims to be the best faq app for django. It welcomes
 contributions of all types - issues, bugs, feature requests, documentation
 updates, tests and pull requests ## change log 0.4 fixed bug that logged out
 users can vote - which then raises exceptions 0.5 fixed migrations 1.0 added
 pypi distribution 1.1 added more templates to override easily 1.2 fixed bug in
 pypi distro not including faq app 1.3 fixed bug where a slug must be filled out
 in admin even though slug gets auto generated to save for questions, answers,
-and categories. made questions, answers, categories slugs readonly in admin 1.4
+and categories. Made questions, answers, categories slugs readonly in admin 1.4
 added unicode option to add unicode slugs 1.5 added login_required setting to
 allow faq app to be available to only logged in users 1.6 fixed bug where
 no_category_description did not do remove the category description in the admin
 1.7 added support for django 5.0 1.8 added support for richtext answers with
-django-tinymce
+django-tinymce 1.9 added view onsite link in admin, added richtext answers in
+admin
```

### Comparing `django_easy_faq-1.8/django_easy_faq.egg-info/PKG-INFO` & `django_easy_faq-1.9/django_easy_faq.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-easy-faq
-Version: 1.8
+Version: 1.9
 Summary: A Django app to add great FAQ functionality to website
 Home-page: https://github.com/smark-1/django-easy-faq/
 Download-URL: https://pypi.python.org/pypi/django-easy-faq
 License: MIT
 Keywords: django,faq
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -369,18 +369,20 @@
 
 1.0 added pypi distribution
 
 1.1 added more templates to override easily
 
 1.2 fixed bug in pypi distro not including faq app
 
-1.3 fixed bug where a slug must be filled out in admin even though slug gets auto generated to save for questions, answers, and categories. made questions, answers, categories slugs readonly in admin
+1.3 fixed bug where a slug must be filled out in admin even though slug gets auto generated to save for questions, answers, and categories. Made questions, answers, categories slugs readonly in admin
 
 1.4 added unicode option to add unicode slugs
 
 1.5 added login_required setting to allow faq app to be available to only logged in users
 
 1.6 fixed bug where no_category_description did not do remove the category description in the admin
 
 1.7 added support for django 5.0
 
 1.8 added support for richtext answers with django-tinymce
+
+1.9 added view onsite link in admin, added richtext answers in admin
```

### Comparing `django_easy_faq-1.8/django_easy_faq.egg-info/SOURCES.txt` & `django_easy_faq-1.9/django_easy_faq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django_easy_faq-1.8/faq/forms.py` & `django_easy_faq-1.9/faq/forms.py`

 * *Files identical despite different names*

### Comparing `django_easy_faq-1.8/faq/migrations/0001_initial.py` & `django_easy_faq-1.9/faq/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_easy_faq-1.8/faq/migrations/0002_alter_answer_id_alter_answerhelpful_id_and_more.py` & `django_easy_faq-1.9/faq/migrations/0002_alter_answer_id_alter_answerhelpful_id_and_more.py`

 * *Files identical despite different names*

### Comparing `django_easy_faq-1.8/faq/migrations/0004_alter_answer_slug_alter_category_slug.py` & `django_easy_faq-1.9/faq/migrations/0004_alter_answer_slug_alter_category_slug.py`

 * *Files identical despite different names*

### Comparing `django_easy_faq-1.8/faq/models.py` & `django_easy_faq-1.9/faq/models.py`

 * *Files 26% similar despite different names*

```diff
@@ -34,15 +34,14 @@
     def get_absolute_url(self):
         # if using categories
         if "no_category" not in settings.FAQ_SETTINGS:
             return reverse("faq:question_detail", args=(self.category.slug, self.slug))
         else:
             return reverse("faq:question_detail", args=(self.slug,))
 
-
     class Meta:
         app_label = 'faq'
 
 
 class Answer(models.Model):
     question = models.ForeignKey(Question, on_delete=models.CASCADE)
     answer = models.TextField()
@@ -73,14 +72,21 @@
             self.slug = new_slug
         # if answer is not new
         if self.pk:
             self.helpful = self.get_helpful()
             self.not_helpful = self.get_not_helpful()
         super().save(*args, **kwargs)
 
+    def get_absolute_url(self):
+        # if using categories
+        if "no_category" not in settings.FAQ_SETTINGS:
+            return reverse("faq:question_detail", args=(self.question.category.slug, self.question.slug))
+        else:
+            return reverse("faq:question_detail", args=(self.question.slug,))
+
 
 class Category(models.Model):
     name = models.CharField(max_length=50, unique=True)
     _description = models.TextField()
     slug = models.SlugField(max_length=50, unique=True, blank=True)
 
     def __str__(self):
@@ -98,28 +104,38 @@
         else:
             return self._description
 
     def save(self, *args, **kwargs):
         self.slug = slugify(self.name, allow_unicode='allow_unicode' in settings.FAQ_SETTINGS)[:50]
         return super().save(*args, **kwargs)
 
+    def get_absolute_url(self):
+        return reverse("faq:category_detail", args=(self.slug,))
+
 
 class FAQComment(models.Model):
     user = models.ForeignKey(settings.AUTH_USER_MODEL, on_delete=models.CASCADE, null=True)
     comment = models.TextField()
     question = models.ForeignKey(Question, on_delete=models.CASCADE)
     post_time = models.DateTimeField(auto_now_add=True)
 
     def __str__(self):
         return self.comment
 
     class Meta:
         ordering = ['question', '-post_time']
         app_label = 'faq'
 
+    def get_absolute_url(self):
+        # if using categories
+        if "no_category" not in settings.FAQ_SETTINGS:
+            return reverse("faq:question_detail", args=(self.question.category.slug, self.question.slug))
+        else:
+            return reverse("faq:question_detail", args=(self.question.slug,))
+
 
 class AnswerHelpful(models.Model):
     user = models.ForeignKey(settings.AUTH_USER_MODEL, on_delete=models.CASCADE)
     answer = models.ForeignKey(Answer, on_delete=models.CASCADE)
     vote = models.BooleanField()
 
     def __str__(self):
@@ -130,14 +146,22 @@
 
         return str(self.answer) + '- ' + vote_var
 
     class Meta:
         ordering = ['answer', 'vote']
         app_label = 'faq'
 
+    def get_absolute_url(self):
+        # if using categories
+        if "no_category" not in settings.FAQ_SETTINGS:
+            return reverse("faq:question_detail", args=(self.answer.question.category.slug, self.answer.question.slug))
+        else:
+            return reverse("faq:question_detail", args=(self.answer.question.slug,))
+
+
 
 class QuestionHelpful(models.Model):
     user = models.ForeignKey(settings.AUTH_USER_MODEL, on_delete=models.CASCADE)
     question = models.ForeignKey(Question, on_delete=models.CASCADE)
     vote = models.BooleanField()
 
     def __str__(self):
@@ -147,7 +171,14 @@
             vote_var = 'dislike'
 
         return str(self.question) + '- ' + vote_var
 
     class Meta:
         ordering = ['question', 'vote']
         app_label = 'faq'
+
+    def get_absolute_url(self):
+        # if using categories
+        if "no_category" not in settings.FAQ_SETTINGS:
+            return reverse("faq:question_detail", args=(self.question.category.slug, self.question.slug))
+        else:
+            return reverse("faq:question_detail", args=(self.question.slug,))
```

### Comparing `django_easy_faq-1.8/faq/snippets.py` & `django_easy_faq-1.9/faq/snippets.py`

 * *Files identical despite different names*

### Comparing `django_easy_faq-1.8/faq/templates/faq/category_detail.html` & `django_easy_faq-1.9/faq/templates/faq/category_detail.html`

 * *Files identical despite different names*

### Comparing `django_easy_faq-1.8/faq/templates/faq/comments.html` & `django_easy_faq-1.9/faq/templates/faq/comments.html`

 * *Files identical despite different names*

### Comparing `django_easy_faq-1.8/faq/templates/faq/question_base.html` & `django_easy_faq-1.9/faq/templates/faq/question_base.html`

 * *Files identical despite different names*

### Comparing `django_easy_faq-1.8/faq/templates/faq/question_detail.html` & `django_easy_faq-1.9/faq/templates/faq/question_detail.html`

 * *Files identical despite different names*

### Comparing `django_easy_faq-1.8/faq/tests.py` & `django_easy_faq-1.9/faq/tests.py`

 * *Files identical despite different names*

### Comparing `django_easy_faq-1.8/faq/urls.py` & `django_easy_faq-1.9/faq/urls.py`

 * *Files identical despite different names*

### Comparing `django_easy_faq-1.8/faq/views.py` & `django_easy_faq-1.9/faq/views.py`

 * *Files identical despite different names*

### Comparing `django_easy_faq-1.8/setup.py` & `django_easy_faq-1.9/setup.py`

 * *Files identical despite different names*

