# Comparing `tmp/django_settings_env-4.7.1.tar.gz` & `tmp/django_settings_env-4.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_settings_env-4.7.1.tar", max compression
+gzip compressed data, was "django_settings_env-4.7.3.tar", max compression
```

## Comparing `django_settings_env-4.7.1.tar` & `django_settings_env-4.7.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1086 2024-01-10 03:47:57.463266 django_settings_env-4.7.1/LICENSE
--rw-r--r--   0        0        0     7225 2024-01-10 03:47:57.463266 django_settings_env-4.7.1/README.md
--rw-r--r--   0        0        0      216 2024-01-10 03:47:57.463266 django_settings_env-4.7.1/django_settings_env/__init__.py
--rw-r--r--   0        0        0     1978 2024-01-10 03:47:57.463266 django_settings_env-4.7.1/django_settings_env/deferred.py
--rw-r--r--   0        0        0    22740 2024-01-10 03:47:57.463266 django_settings_env-4.7.1/django_settings_env/env_django.py
--rw-r--r--   0        0        0      832 2024-01-10 03:47:57.463266 django_settings_env-4.7.1/pyproject.toml
--rw-r--r--   0        0        0     7885 1970-01-01 00:00:00.000000 django_settings_env-4.7.1/PKG-INFO
+-rw-r--r--   0        0        0     1086 2024-05-12 01:13:18.641049 django_settings_env-4.7.3/LICENSE
+-rw-r--r--   0        0        0     7225 2024-05-12 01:13:18.645049 django_settings_env-4.7.3/README.md
+-rw-r--r--   0        0        0      216 2024-05-12 01:13:18.645049 django_settings_env-4.7.3/django_settings_env/__init__.py
+-rw-r--r--   0        0        0     2001 2024-05-12 01:13:18.645049 django_settings_env-4.7.3/django_settings_env/deferred.py
+-rw-r--r--   0        0        0    22812 2024-05-12 01:13:18.645049 django_settings_env-4.7.3/django_settings_env/env_django.py
+-rw-r--r--   0        0        0      889 2024-05-12 01:13:18.645049 django_settings_env-4.7.3/pyproject.toml
+-rw-r--r--   0        0        0     7906 1970-01-01 00:00:00.000000 django_settings_env-4.7.3/PKG-INFO
```

### Comparing `django_settings_env-4.7.1/LICENSE` & `django_settings_env-4.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django_settings_env-4.7.1/README.md` & `django_settings_env-4.7.3/README.md`

 * *Files identical despite different names*

### Comparing `django_settings_env-4.7.1/django_settings_env/deferred.py` & `django_settings_env-4.7.3/django_settings_env/deferred.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,17 +9,17 @@
         return LazySettings.__getattribute__(self, name)
 
 
 def deferred_handler():
     # at least one DeferredSetting is being used, so override the __getattr__ handler for the setting module
     # to catch any DeferredSetting use and return an appropriate value from the environment
     if not getattr(deferred_handler, "enabled", False):
-        # need to overrite both because __getattr__ is not called if the setting is defined (no longer lazy)
-        LazySettings.__getattr__ = deferred_getattr(LazySettings.__getattr__)
-        LazySettings.__getattribute__ = deferred_getattribute(LazySettings.__getattribute__)
+        # need to overwrite both because __getattr__ is not called if the setting is defined (no longer lazy)
+        setattr(LazySettings, '__getattr__', deferred_getattr(LazySettings.__getattr__))
+        setattr(LazySettings, '__getattribute__', deferred_getattribute(LazySettings.__getattribute__))
         deferred_handler.enabled = True
 
 
 class DeferredSetting:
     # similar to django-class-settings DeferredEnv but simpler
     # and handles settings at module level not in a Settings class
```

### Comparing `django_settings_env-4.7.1/django_settings_env/env_django.py` & `django_settings_env-4.7.3/django_settings_env/env_django.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # -*- coding: utf-8 -*-
 """
 Wrapper around os.environ with django config value parsers
 """
+
+import contextlib
 from urllib.parse import parse_qs, unquote_plus, urlparse, urlunparse
 
 from django.core.exceptions import ImproperlyConfigured
 from django.utils.encoding import smart_str
 from django.utils.version import get_complete_version
 from envex import Env
 
@@ -130,14 +132,15 @@
         @param token: (optional) vault token, default is $VAULT_TOKEN or ~/.vault-token
         @param cert: (optional) tuple (cert, key) or str path to client cert/key files
         @param verify: (optional) bool | str whether to verify server cert or set ca cert path (default=True)
         @param cache_enabled: (optional) bool whether to cache secrets (default=True)
         @param base_path: (optional) str base path for secrets (default=None)
         @param engine: (optional) str vault secrets engine (default=None)
         @param mount_point: (optional) str vault secrets mount point (default=None, determined by engine)
+        @param timeout: (optional) int timeout for connecting to vault (default=5)
         @param working_dirs: (optional) bool whether to include PWD/CWD (default=True)
         -
         @param kwargs: (optional) environment variables to add/override
         """
         self.prefix = kwargs.pop("prefix", _DEFAULT_ENV_PREFIX)
         # by default, use Django config exception in preference to KeyError
         kwargs.setdefault("exception", ImproperlyConfigured)
@@ -194,37 +197,33 @@
         if var is None:
             kwds = {
                 "name": var,
                 "prefix": prefix if prefix is None else self.prefix,
                 "default": default,
             }
             # try using class_settings version if installed
-            try:
+            with contextlib.suppress(ImportError):
                 # noinspection PyUnresolvedReferences
                 from class_settings.env import DeferredEnv
 
                 return DeferredEnv(self, kwargs=kwds, optional=kwargs.get("optional", False))
-            except ImportError:
-                pass
             # otherwise, use our own implementation (handles module level vars)
             from .deferred import DeferredSetting
 
             # class settings not installed
             return DeferredSetting(env=self, kwargs=kwds)
 
         # set to the provided default if not already set
         if default is not None and not self.is_set(var):
             self.set(var, default)
         # resolve entry point by the type
-        try:
+        with contextlib.suppress(KeyError):
             _type = kwargs.pop("type", "str")
             _type = _type if isinstance(_type, str) else _type.__name__
             return self.django_env_typemap[_type](self, var, default=default, prefix=prefix)
-        except KeyError:
-            pass
         return self.get(var, default=default, prefix=prefix)
 
     # Django-specific additions
 
     def database_url(self, var=DEFAULT_DATABASE_ENV, *, default=None, engine=None, options=None):
         """
         Parse the url, mostly based on dj-database-url
```

### Comparing `django_settings_env-4.7.1/pyproject.toml` & `django_settings_env-4.7.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 [tool.poetry]
 name = "django-settings-env"
-version = "4.7.1"
+version = "4.7.3"
 description = "12-factor.net settings support for Django with .env and HashiCorp Vault support"
 authors = ["David Nugent <davidn@uniquode.io>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
-Django = ">= 3.1"
-envex = ">= 3.0"
+Django = ">=3.1"
+envex = ">=3.0"
 django-class-settings = { version = "^0.2", optional = true }
 
 [tool.poetry.group.test.dependencies]
 pytest = ">7.0"
-pytest-cov = "^4.1.0"
+pytest-cov = ">=4.1,<6.0"
 
 [tool.poetry.group.dev.dependencies]
-black = "^23.7.0"
-isort = "^5.12.0"
-ruff = "^0.0.285"
+ruff = "^0.4.4"
 pre-commit = "^3.3.3"
 
 [tool.poetry.extras]
 django-class-settings = ["django-class-settings"]
+hvac = ["hvac"]
+
+[tool.poetry.group.vault.dependencies]
+hvac = ">= 1.1.1"
 
 [tool.pytest.ini-options]
 minversion = "7.0"
+addopts = "-ra -q"
 pythonpath = [ "django_settings_env" ]
 testpaths = [ "tests" ]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `django_settings_env-4.7.1/PKG-INFO` & `django_settings_env-4.7.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: django-settings-env
-Version: 4.7.1
+Version: 4.7.3
 Summary: 12-factor.net settings support for Django with .env and HashiCorp Vault support
 Author: David Nugent
 Author-email: davidn@uniquode.io
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: django-class-settings
+Provides-Extra: hvac
 Requires-Dist: Django (>=3.1)
 Requires-Dist: django-class-settings (>=0.2,<0.3) ; extra == "django-class-settings"
 Requires-Dist: envex (>=3.0)
 Description-Content-Type: text/markdown
 
 # django-settings-env
```

