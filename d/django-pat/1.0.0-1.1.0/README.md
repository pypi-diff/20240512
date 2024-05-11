# Comparing `tmp/django_pat-1.0.0.tar.gz` & `tmp/django_pat-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_pat-1.0.0.tar", max compression
+gzip compressed data, was "django_pat-1.1.0.tar", max compression
```

## Comparing `django_pat-1.0.0.tar` & `django_pat-1.1.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1069 2023-02-19 19:03:00.014916 django_pat-1.0.0/LICENSE
--rw-r--r--   0        0        0     7405 2023-02-19 19:03:00.014916 django_pat-1.0.0/README.md
--rw-r--r--   0        0        0     1575 2023-02-19 19:03:00.014916 django_pat-1.0.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-02-19 19:03:00.014916 django_pat-1.0.0/src/django_pat/__init__.py
--rw-r--r--   0        0        0     1743 2023-02-19 19:03:00.014916 django_pat-1.0.0/src/django_pat/admin.py
--rw-r--r--   0        0        0      151 2023-02-19 19:03:00.014916 django_pat-1.0.0/src/django_pat/apps.py
--rw-r--r--   0        0        0     1023 2023-02-19 19:03:00.014916 django_pat-1.0.0/src/django_pat/http.py
--rw-r--r--   0        0        0     1376 2023-02-19 19:03:00.014916 django_pat-1.0.0/src/django_pat/middleware.py
--rw-r--r--   0        0        0     1308 2023-02-19 19:03:00.014916 django_pat-1.0.0/src/django_pat/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-02-19 19:03:00.014916 django_pat-1.0.0/src/django_pat/migrations/__init__.py
--rw-r--r--   0        0        0     2956 2023-02-19 19:03:00.014916 django_pat-1.0.0/src/django_pat/models.py
--rw-r--r--   0        0        0        0 2023-02-19 19:03:00.014916 django_pat-1.0.0/src/django_pat/rest_framework/__init__.py
--rw-r--r--   0        0        0     1039 2023-02-19 19:03:00.014916 django_pat-1.0.0/src/django_pat/rest_framework/auth.py
--rw-r--r--   0        0        0      237 2023-02-19 19:03:00.014916 django_pat-1.0.0/src/django_pat/rest_framework/urls.py
--rw-r--r--   0        0        0     1894 2023-02-19 19:03:00.014916 django_pat-1.0.0/src/django_pat/rest_framework/views.py
--rw-r--r--   0        0        0      176 2023-02-19 19:03:00.018916 django_pat-1.0.0/src/django_pat/templates/personal_access_token/confirm_delete.html
--rw-r--r--   0        0        0     1288 2023-02-19 19:03:00.018916 django_pat-1.0.0/src/django_pat/templates/personal_access_token/create.html
--rw-r--r--   0        0        0     1380 2023-02-19 19:03:00.018916 django_pat-1.0.0/src/django_pat/templates/personal_access_token/list.html
--rw-r--r--   0        0        0      456 2023-02-19 19:03:00.018916 django_pat-1.0.0/src/django_pat/urls.py
--rw-r--r--   0        0        0     1927 2023-02-19 19:03:00.018916 django_pat-1.0.0/src/django_pat/views.py
--rw-r--r--   0        0        0     8507 1970-01-01 00:00:00.000000 django_pat-1.0.0/setup.py
--rw-r--r--   0        0        0     8389 1970-01-01 00:00:00.000000 django_pat-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-11 23:03:07.957583 django_pat-1.1.0/LICENSE
+-rw-r--r--   0        0        0     7405 2024-05-11 23:03:07.957583 django_pat-1.1.0/README.md
+-rw-r--r--   0        0        0     1610 2024-05-11 23:03:07.957583 django_pat-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-11 23:03:07.957583 django_pat-1.1.0/src/django_pat/__init__.py
+-rw-r--r--   0        0        0     1743 2024-05-11 23:03:07.957583 django_pat-1.1.0/src/django_pat/admin.py
+-rw-r--r--   0        0        0      151 2024-05-11 23:03:07.957583 django_pat-1.1.0/src/django_pat/apps.py
+-rw-r--r--   0        0        0     1023 2024-05-11 23:03:07.957583 django_pat-1.1.0/src/django_pat/http.py
+-rw-r--r--   0        0        0     1376 2024-05-11 23:03:07.957583 django_pat-1.1.0/src/django_pat/middleware.py
+-rw-r--r--   0        0        0     1308 2024-05-11 23:03:07.957583 django_pat-1.1.0/src/django_pat/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2024-05-11 23:03:07.957583 django_pat-1.1.0/src/django_pat/migrations/__init__.py
+-rw-r--r--   0        0        0     2956 2024-05-11 23:03:07.957583 django_pat-1.1.0/src/django_pat/models.py
+-rw-r--r--   0        0        0        0 2024-05-11 23:03:07.957583 django_pat-1.1.0/src/django_pat/rest_framework/__init__.py
+-rw-r--r--   0        0        0     1039 2024-05-11 23:03:07.957583 django_pat-1.1.0/src/django_pat/rest_framework/auth.py
+-rw-r--r--   0        0        0      237 2024-05-11 23:03:07.957583 django_pat-1.1.0/src/django_pat/rest_framework/urls.py
+-rw-r--r--   0        0        0     1894 2024-05-11 23:03:07.957583 django_pat-1.1.0/src/django_pat/rest_framework/views.py
+-rw-r--r--   0        0        0      176 2024-05-11 23:03:07.957583 django_pat-1.1.0/src/django_pat/templates/personal_access_token/confirm_delete.html
+-rw-r--r--   0        0        0     1288 2024-05-11 23:03:07.957583 django_pat-1.1.0/src/django_pat/templates/personal_access_token/create.html
+-rw-r--r--   0        0        0     1380 2024-05-11 23:03:07.957583 django_pat-1.1.0/src/django_pat/templates/personal_access_token/list.html
+-rw-r--r--   0        0        0      456 2024-05-11 23:03:07.957583 django_pat-1.1.0/src/django_pat/urls.py
+-rw-r--r--   0        0        0     1927 2024-05-11 23:03:07.957583 django_pat-1.1.0/src/django_pat/views.py
+-rw-r--r--   0        0        0     8507 1970-01-01 00:00:00.000000 django_pat-1.1.0/setup.py
+-rw-r--r--   0        0        0     8428 1970-01-01 00:00:00.000000 django_pat-1.1.0/PKG-INFO
```

### Comparing `django_pat-1.0.0/LICENSE` & `django_pat-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_pat-1.0.0/README.md` & `django_pat-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `django_pat-1.0.0/pyproject.toml` & `django_pat-1.1.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 [tool.poetry]
 name = "django_pat"
-version = "1.0.0"
+version = "1.1.0"
 description = "A Django package for creating, using, and managing personal access tokens."
 readme = "README.md"
 authors = ["Chris Muthig <camuthig@gmail.com>"]
 license = "MIT"
 packages = [
     { include = "django_pat", from = "src" },
 ]
 classifiers = [
     "Framework :: Django :: 3.2",
     "Framework :: Django :: 4.0",
     "Framework :: Django :: 4.1",
+    "Framework :: Django :: 4.2",
 ]
 
 [tool.poetry.dependencies]
 python = ">= 3.7, < 3.12"
 django = [
     {version = "~3.2", python = "3.7"},
-    {version = ">= 3.2, < 4.2", python = ">= 3.8"},
+    {version = ">= 3.2, < 5.0", python = ">= 3.8"},
 ]
 
 djangorestframework = { version = "^3.11", optional = true }
 
 [tool.poetry.extras]
 djangorestframework = ["djangorestframework"]
 
@@ -30,17 +31,17 @@
 djangorestframework = "^3.11"
 pytest = "^7.1"
 pytest-django = "^4.5"
 pre-commit = "^2.18"
 flake8 = "^5.0"
 black = "^23.1"
 mypy = "^1.0"
-django-stubs = "^1.10"
-djangorestframework-stubs = "1.7.0"
-nox = "^2022.1"
+django-stubs = "^4.2"
+djangorestframework-stubs = "^3.14.0"
+nox = "^2024.4"
 isort = "^5.10"
 coverage = {extras = ["toml"], version = "^7.0.5"}
 pytest-cov = "^4.0.0"
 
 [tool.pytest.ini_options]
 pythonpath = ["src"]
 DJANGO_SETTINGS_MODULE = "tests.settings"
```

### Comparing `django_pat-1.0.0/src/django_pat/admin.py` & `django_pat-1.1.0/src/django_pat/admin.py`

 * *Files identical despite different names*

### Comparing `django_pat-1.0.0/src/django_pat/http.py` & `django_pat-1.1.0/src/django_pat/http.py`

 * *Files identical despite different names*

### Comparing `django_pat-1.0.0/src/django_pat/middleware.py` & `django_pat-1.1.0/src/django_pat/middleware.py`

 * *Files identical despite different names*

### Comparing `django_pat-1.0.0/src/django_pat/migrations/0001_initial.py` & `django_pat-1.1.0/src/django_pat/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_pat-1.0.0/src/django_pat/models.py` & `django_pat-1.1.0/src/django_pat/models.py`

 * *Files identical despite different names*

### Comparing `django_pat-1.0.0/src/django_pat/rest_framework/auth.py` & `django_pat-1.1.0/src/django_pat/rest_framework/auth.py`

 * *Files identical despite different names*

### Comparing `django_pat-1.0.0/src/django_pat/rest_framework/views.py` & `django_pat-1.1.0/src/django_pat/rest_framework/views.py`

 * *Files identical despite different names*

### Comparing `django_pat-1.0.0/src/django_pat/templates/personal_access_token/create.html` & `django_pat-1.1.0/src/django_pat/templates/personal_access_token/create.html`

 * *Files identical despite different names*

### Comparing `django_pat-1.0.0/src/django_pat/templates/personal_access_token/list.html` & `django_pat-1.1.0/src/django_pat/templates/personal_access_token/list.html`

 * *Files identical despite different names*

### Comparing `django_pat-1.0.0/src/django_pat/views.py` & `django_pat-1.1.0/src/django_pat/views.py`

 * *Files identical despite different names*

### Comparing `django_pat-1.0.0/setup.py` & `django_pat-1.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,20 +8,20 @@
 ['django_pat', 'django_pat.migrations', 'django_pat.rest_framework']
 
 package_data = \
 {'': ['*'], 'django_pat': ['templates/personal_access_token/*']}
 
 extras_require = \
 {':python_version == "3.7"': ['django>=3.2,<3.3'],
- ':python_version >= "3.8"': ['django>=3.2,<4.2'],
+ ':python_version >= "3.8"': ['django>=3.2,<5.0'],
  'djangorestframework': ['djangorestframework>=3.11,<4.0']}
 
 setup_kwargs = {
     'name': 'django-pat',
-    'version': '1.0.0',
+    'version': '1.1.0',
     'description': 'A Django package for creating, using, and managing personal access tokens.',
     'long_description': '# Django PAT (Personal Access Tokens)\n\n![Tests](https://github.com/camuthig/django-pat/actions/workflows/ci.yml/badge.svg)\n[![codecov](https://codecov.io/gh/camuthig/django-pat/branch/main/graph/badge.svg?token=GAGIIZXC95)](https://codecov.io/gh/camuthig/django-pat)\n[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)\n[![Source Code](https://img.shields.io/badge/Source-code-lightgrey)](https://github.com/camuthig/django-pat)\n![PyPI](https://img.shields.io/pypi/v/django-pat)\n![Python Versions](https://img.shields.io/pypi/pyversions/django-pat)\n![Django Versions](https://img.shields.io/pypi/djversions/django-pat?label=django)\n\nThis application creates personal access tokens that clients can send via HTTP headers to authenticate as a particular user.\nThis application expands on the standard functionality provided in REST Framework tokens by allowing users to create\nmore than one token and cycle/revoke tokens for security purposes.\n\nPersonal access tokens are API keys that allow clients to pass a secure value to an API without having to first exchange\na username and password. This  makes interactions between machines straightforward and consistent. While these tokens are\neasy to use, it is important to ensure they are secure. This application accomplishes this security by:\n\n1. Hashing all token values after creation. This ensures admins of the application and malicious actors are never be able\n   to access token values in plain text via a data breach.\n2. Allowing for tokens to be "cycled". This is accomplished by revoking existing tokens and creating new ones. Clients\n   can do this easily via APIs on a regular basis or as needed, if they believe a token has been compromised.\n\n## Usage\n\nBy default, both the standard middleware and the REST Framework authentication will look for the token in the\n`Authorization` HTTP header with a prefix of `Access-Token`. So this might look like\n\n```\nAuthorization: Access-Token 41ecea63-66eb-4e6a-bffd-e85cd29718ab\n```\n\n### Initial Setup\n1. Install the package: `pip install django-pat`\n2. Add `django_pat` to the `INSTALLED_APPS` of your project\n3. Add the `PAT_SECRET` value to your settings file to hash secrets. This value should be kept secret!\n    ```python\n    PAT_SECRET = "super-secret-hashing-key"\n    ```\n\n\n### Django Middleware\n\n1. Add the middleware to your middleware stack\n   ```python\n   MIDDLEWARE = [\n       "django.contrib.auth.middleware.AuthenticationMiddleware",\n       "django_pat.middleware.PatAuthenticationMiddleware",\n   ]\n   ```\n\n### REST Framework\n\n1. Add the authentication class to your DRF default authentication classes\n   ```python\n   REST_FRAMEWORK = {\n       "DEFAULT_AUTHENTICATION_CLASSES": [\n           "django_pat.rest_framework.auth.PatAuthentication",\n           "rest_framework.authentication.SessionAuthentication",\n       ],\n   }\n   ```\n\n**Optional: Add Personal Access Token Views**\n\nAPIs can be added to your Django application to create, retrieve, and revoke tokens out of the box. This will create new Django Rest Routes at `/personalAccessTokens`\n\n```python\n# urls.py\nfrom django.urls import include\nfrom django.urls import path\n\nfrom django_pat.rest_framework.urls import router as pat_router\n\nurlpatterns = [\n    # other routes...\n\n    path("api/", include(pat_router.urls)),\n]\n```\n\nAlternatively, the `PersonalAccessTokenViewSet` can be added to any route you prefer.\n\n## Configuration\n\nAlong with the `PAT_SECRET` value that is required, you can also configure certain behaviors of the package in your Django\napplication settings.\n\n* `PAT_CUSTOM_HEADER` - Sets the HTTP header to check for the token. This defaults to `Authorization`\n* `PAT_CUSTOM_HEADER_PREFIX` - Sets the prefix for the header value. This defaults to `Access-Token`. The middleware\n    and the REST authentication expect a space between the prefix and the token value.\n* `PAT_USES_SHARED_HEADER` - If set to True, then the package will not attempt to validate the prefix on the authorization\n    header. This is most useful when different prefixes are used for different types of authentication, but are all sent\n    using the same HTTP header.\n\n## Implementation Details\n\nAccess token values are implemented as UUID4 values. These are sufficiently unique to remain secure and avoid collisions.\n\n## Security Concerns\n\n**Personal access token records should NOT be deleted from the database, even if revoked.** If tokens are deleted, there is the\npossibility that the token value could be reassigned to a different user at a later time. If the user originally provided\nthe token retains it, they may later use it to inadvertently access the API as the new user. The default behavior of this\napplication in the admin is to _revoke_ token instead of deleting them, and it is recommended users follow this same\npattern.\n\nIf a brute force attack is a concern, then rate limiting should be applied to API views. The possibility of brute\nforcing all possible UUID4 values is unlikely, but rate limiting provides another way to avoid it.\n\n## Alternative Packages\n\n* [Django REST Framework API Key](https://florimondmanca.github.io/djangorestframework-api-key/guide/) This project\n  similarly provides the ability to create and manage API keys for machine-to-machine API calls. It is focused on\n  supporting unauthorized requests, i.e. those not linked to a particular user. There are a few reasons I chose to go\n  with a different option.\n  * The Django REST Framework API Keys is tightly coupled with Django REST Framework. I wanted this package to support\n    DRF without being coupled to it, such that developers who want to build APIs without DRF have the option.\n  * The default behavior of Django REST Framework API Keys is not linked to users. The key can be extended to have a\n    reference to the user, but this requires additional configuration and the default model table is still created for\n    the base API key model. This means that by default developers will be able to use existing user permissions with\n    working with a User API Key. See: [Issue 180](https://github.com/florimondmanca/djangorestframework-api-key/issues/180)\n  * The Django REST Framework API Key encryption technique used by the application creates a slower API. This has been\n    alleviated in Django User API Key by using HMAC hashing instead. See:\n    [Issue 173](https://github.com/florimondmanca/djangorestframework-api-key/issues/173)\n  * The primary key pattern of the Django REST Framework API Key records use special characters, making them difficult\n    to encode for browsers. See: [Issue 128](https://github.com/florimondmanca/djangorestframework-api-key/issues/128)\n* [Django REST Framework TokenAuthentication](https://www.django-rest-framework.org/api-guide/authentication/#tokenauthentication)\n  The standard DRF `TokenAuthentication` model has a couple of drawbacks that this project attempts to avoid by\n  expanding on the pattern. In the standard token pattern:\n  * The token value is stored in a plain-text format\n  * The token value acts as the primary key of the token. If building an API to retrieve the token, you would not\n    want to use this key in a URL, as it would go over the network in plain-text.\n  * Each user can only have a single token.\n  * Revoking one user\'s token opens up the possibility of generating the same token again for a different user.\n',
     'author': 'Chris Muthig',
     'author_email': 'camuthig@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `django_pat-1.0.0/PKG-INFO` & `django_pat-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 Metadata-Version: 2.1
 Name: django-pat
-Version: 1.0.0
+Version: 1.1.0
 Summary: A Django package for creating, using, and managing personal access tokens.
 License: MIT
 Author: Chris Muthig
 Author-email: camuthig@gmail.com
 Requires-Python: >=3.7,<3.12
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: djangorestframework
 Requires-Dist: django (>=3.2,<3.3) ; python_version == "3.7"
-Requires-Dist: django (>=3.2,<4.2) ; python_version >= "3.8"
+Requires-Dist: django (>=3.2,<5.0) ; python_version >= "3.8"
 Requires-Dist: djangorestframework (>=3.11,<4.0) ; extra == "djangorestframework"
 Description-Content-Type: text/markdown
 
 # Django PAT (Personal Access Tokens)
 
 ![Tests](https://github.com/camuthig/django-pat/actions/workflows/ci.yml/badge.svg)
 [![codecov](https://codecov.io/gh/camuthig/django-pat/branch/main/graph/badge.svg?token=GAGIIZXC95)](https://codecov.io/gh/camuthig/django-pat)
```

