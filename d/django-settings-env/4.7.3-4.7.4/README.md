# Comparing `tmp/django_settings_env-4.7.3.tar.gz` & `tmp/django_settings_env-4.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_settings_env-4.7.3.tar", max compression
+gzip compressed data, was "django_settings_env-4.7.4.tar", max compression
```

## Comparing `django_settings_env-4.7.3.tar` & `django_settings_env-4.7.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1086 2024-05-12 01:13:18.641049 django_settings_env-4.7.3/LICENSE
--rw-r--r--   0        0        0     7225 2024-05-12 01:13:18.645049 django_settings_env-4.7.3/README.md
--rw-r--r--   0        0        0      216 2024-05-12 01:13:18.645049 django_settings_env-4.7.3/django_settings_env/__init__.py
--rw-r--r--   0        0        0     2001 2024-05-12 01:13:18.645049 django_settings_env-4.7.3/django_settings_env/deferred.py
--rw-r--r--   0        0        0    22812 2024-05-12 01:13:18.645049 django_settings_env-4.7.3/django_settings_env/env_django.py
--rw-r--r--   0        0        0      889 2024-05-12 01:13:18.645049 django_settings_env-4.7.3/pyproject.toml
--rw-r--r--   0        0        0     7906 1970-01-01 00:00:00.000000 django_settings_env-4.7.3/PKG-INFO
+-rw-r--r--   0        0        0     1086 2024-05-12 09:47:07.519223 django_settings_env-4.7.4/LICENSE
+-rw-r--r--   0        0        0     7225 2024-05-12 09:47:07.519223 django_settings_env-4.7.4/README.md
+-rw-r--r--   0        0        0      216 2024-05-12 09:47:07.519223 django_settings_env-4.7.4/django_settings_env/__init__.py
+-rw-r--r--   0        0        0     2001 2024-05-12 09:47:07.519223 django_settings_env-4.7.4/django_settings_env/deferred.py
+-rw-r--r--   0        0        0    21646 2024-05-12 09:47:07.519223 django_settings_env-4.7.4/django_settings_env/env_django.py
+-rw-r--r--   0        0        0      885 2024-05-12 09:47:07.519223 django_settings_env-4.7.4/pyproject.toml
+-rw-r--r--   0        0        0     7906 1970-01-01 00:00:00.000000 django_settings_env-4.7.4/PKG-INFO
```

### Comparing `django_settings_env-4.7.3/LICENSE` & `django_settings_env-4.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `django_settings_env-4.7.3/README.md` & `django_settings_env-4.7.4/README.md`

 * *Files identical despite different names*

### Comparing `django_settings_env-4.7.3/django_settings_env/deferred.py` & `django_settings_env-4.7.4/django_settings_env/deferred.py`

 * *Files identical despite different names*

### Comparing `django_settings_env-4.7.3/django_settings_env/env_django.py` & `django_settings_env-4.7.4/django_settings_env/env_django.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # -*- coding: utf-8 -*-
 """
 Wrapper around os.environ with django config value parsers
 """
 
 import contextlib
+from typing import List
 from urllib.parse import parse_qs, unquote_plus, urlparse, urlunparse
 
 from django.core.exceptions import ImproperlyConfigured
 from django.utils.encoding import smart_str
 from django.utils.version import get_complete_version
 from envex import Env
 
@@ -100,16 +101,16 @@
         "backend": "mq.backends.sqs_backend.create_backend",
     },
     "amazon-sqs": {
         "backend": "mq.backends.sqs_backend.create_backend",
     },
 }
 _QUEUE_BASE_OPTIONS = []
-_DEFAULT_ENV_PREFIX = "DJANGO_"
-_DEFAULT_PREFIX = object()
+_DEFAULT_PREFIX = "DJANGO_"
+_USE_DEFAULT_PREFIX = object()
 
 
 class DjangoEnv(Env):
     """
     Wrapper around os.environ with .env enhancement django, and Hashicorp vault support
     """
 
@@ -137,49 +138,49 @@
         @param engine: (optional) str vault secrets engine (default=None)
         @param mount_point: (optional) str vault secrets mount point (default=None, determined by engine)
         @param timeout: (optional) int timeout for connecting to vault (default=5)
         @param working_dirs: (optional) bool whether to include PWD/CWD (default=True)
         -
         @param kwargs: (optional) environment variables to add/override
         """
-        self.prefix = kwargs.pop("prefix", _DEFAULT_ENV_PREFIX)
+        self.prefix = kwargs.pop("prefix", _DEFAULT_PREFIX)
         # by default, use Django config exception in preference to KeyError
         kwargs.setdefault("exception", ImproperlyConfigured)
         # change default to read .env files and search parents as well
         kwargs.setdefault("readenv", True)
         kwargs.setdefault("parents", True)
         super().__init__(*args, **kwargs)
 
     def _with_prefix(self, var, prefix):
-        if prefix is _DEFAULT_PREFIX:
+        if prefix is _USE_DEFAULT_PREFIX:
             prefix = self.prefix
         if var and prefix and not var.startswith(prefix) and not self.is_set(var):
             var = f"{prefix}{var}"
         return var
 
-    def get(self, var, default=None, prefix=_DEFAULT_PREFIX):
+    def get(self, var, default=None, prefix=_USE_DEFAULT_PREFIX):
         return super().get(self._with_prefix(var, prefix=prefix), default)
 
-    def int(self, var, default=None, prefix=_DEFAULT_PREFIX) -> int:
+    def int(self, var, default=None, prefix=_USE_DEFAULT_PREFIX) -> int:
         val = self.get(var, default, prefix=prefix)
         return self._int(val)
 
-    def float(self, var, default=None, prefix=_DEFAULT_PREFIX) -> float:
+    def float(self, var, default=None, prefix=_USE_DEFAULT_PREFIX) -> float:
         val = self.get(var, default, prefix=prefix)
         return self._float(val)
 
-    def bool(self, var, default=None, prefix=_DEFAULT_PREFIX) -> bool:
+    def bool(self, var, default=None, prefix=_USE_DEFAULT_PREFIX) -> bool:
         val = self.get(var, default, prefix=prefix)
         return val if isinstance(val, (bool, int)) else self.is_true(val)
 
-    def list(self, var, default=None, prefix=_DEFAULT_PREFIX) -> list:
+    def list(self, var, default=None, prefix=_USE_DEFAULT_PREFIX) -> list:
         val = self.get(var, default, prefix=prefix)
         return val if isinstance(val, (list, tuple)) else self._list(val)
 
-    def check_var(self, var, default=None, prefix=_DEFAULT_PREFIX, raise_error=True):
+    def check_var(self, var, default=None, prefix=_USE_DEFAULT_PREFIX, raise_error=True):
         """
         override to insert prefix unless the raw var is set
         """
         var = self._with_prefix(var, prefix=prefix)
         return super().check_var(var, default=default, raise_error=raise_error)
 
     django_env_typemap = {
@@ -187,21 +188,21 @@
         "bool": bool,
         "float": float,
         "list": list,
     }
 
     # noinspection PyShadowingBuiltins
     def __call__(self, var=None, default=None, **kwargs):
-        prefix = kwargs.pop("prefix", _DEFAULT_PREFIX)
+        prefix = kwargs.pop("prefix", _USE_DEFAULT_PREFIX)
         # This is tied to django-class-settings (optional dependency), which allows
         # omitting the 'name' parameter and using the setting name instead
         if var is None:
             kwds = {
                 "name": var,
-                "prefix": prefix if prefix is None else self.prefix,
+                "prefix": prefix if prefix is _USE_DEFAULT_PREFIX else self.prefix,
                 "default": default,
             }
             # try using class_settings version if installed
             with contextlib.suppress(ImportError):
                 # noinspection PyUnresolvedReferences
                 from class_settings.env import DeferredEnv
 
@@ -236,15 +237,15 @@
         """
         url = self.check_var(var, default=default)
         # shortcut to avoid urlparse
         if url == "sqlite://:memory":
             return {"ENGINE": DB_SCHEMES["sqlite"], "NAME": ":memory:"}
 
         # otherwise, parse the url as normal
-        config = {}
+        config: dict = {}
         url = urlparse(url)
 
         path = smart_str(url.path[1:])
         path = unquote_plus(path.split("?", 2)[0])
 
         if url.scheme == "sqlite" and path == "":
             path = ":memory:"
@@ -264,23 +265,21 @@
                 hostname = hostname.split(":", 1)[0]
             hostname = hostname.replace("%2f", "/").replace("%2F", "/")
 
         engine = DB_SCHEMES[url.scheme] if engine is None else engine
         port = str(url.port) if url.port and engine == DB_SCHEMES["oracle"] else url.port
 
         # Update with configuration.
-        config.update(
-            {
-                "NAME": path or "",
-                "USER": url.username or "",
-                "PASSWORD": url.password or "",
-                "HOST": hostname,
-                "PORT": port or "",
-            }
-        )
+        config |= {
+            "NAME": path or "",
+            "USER": url.username or "",
+            "PASSWORD": url.password or "",
+            "HOST": hostname,
+            "PORT": port or "",
+        }
 
         if url.scheme == "postgres" and path.startswith("/"):
             config["HOST"], config["NAME"] = path.rsplit("/", 1)
 
         elif url.scheme == "oracle":
             if path == "":
                 config["NAME"], config["HOST"] = config["HOST"], ""
@@ -290,32 +289,32 @@
                 config["PORT"] = str(config["PORT"])
 
         db_options = {}
         # Pass the query string into OPTIONS.
         if url.query:
             for key, values in parse_qs(url.query).items():
                 if key.upper() in _DB_BASE_OPTIONS:
-                    config.update({key.upper(): values[0]})
+                    config[key.upper()] = values[0]
                 else:
-                    db_options.update({key: self._int(values[0])})
+                    db_options[key] = self._int(values[0])
 
             # Support for Postgres Schema URLs
             if "currentSchema" in db_options and engine in (
                 "django.contrib.gis.db.backends.postgis",
                 "django.db.backends.postgresql_psycopg2",
                 "django_redshift_backend",
             ):
                 db_options["options"] = "-c search_path={0}".format(db_options.pop("currentSchema"))
 
         if options:
             for key, value in options.items():
                 if key.upper() in _DB_BASE_OPTIONS:
-                    config.update({key.upper(): value})
+                    config[key.upper()] = value
                 else:
-                    db_options.update({key: value})
+                    db_options[key] = value
         if db_options:
             config["OPTIONS"] = {k.upper(): v for k, v in db_options.items()}
         if engine:
             config["ENGINE"] = engine
         return config
 
     def cache_url(self, var=DEFAULT_CACHE_ENV, *, default=None, backend=None, options=None):
@@ -330,50 +329,30 @@
         url = urlparse(self.check_var(var, default=default))
 
         location = url.netloc.split(",")
         if len(location) == 1:
             location = location[0]
 
         config = {
-            "BACKEND": backend if backend else CACHE_SCHEMES[url.scheme],
+            "BACKEND": backend or CACHE_SCHEMES[url.scheme],
             "LOCATION": location,
         }
 
         # Add the drive to LOCATION
         if url.scheme == "filecache":
-            config.update(
-                {
-                    "LOCATION": url.netloc + url.path,
-                }
-            )
+            config["LOCATION"] = url.netloc + url.path
 
         if url.path and url.scheme in ["unix", "memcache", "pymemcache"]:
-            config.update(
-                {
-                    "LOCATION": f"unix:{url.path}",
-                }
-            )
+            config["LOCATION"] = f"unix:{url.path}"
         elif url.scheme.startswith("redis"):
             scheme = url.scheme.replace("cache", "") if url.hostname else "unix"
             locations = [f"{scheme}://{smart_str(loc)}{url.path}" for loc in url.netloc.split(",")]
             config["LOCATION"] = locations[0] if len(locations) == 1 else locations
 
-        cache_options = {}
-        if url.query:
-            for key, values in parse_qs(url.query).items():
-                opt = {smart_str(key).upper(): smart_str(values[0], strings_only=True)}
-                if key.upper() in _CACHE_BASE_OPTIONS:
-                    config.update(opt)
-                else:
-                    cache_options.update(opt)
-
-        if options:
-            cache_options.update({k.upper(): v for k, v in options.items()})
-        config["OPTIONS"] = cache_options
-        return config
+        return self._parse_options(url.query, config, options, _CACHE_BASE_OPTIONS)
 
     def email_url(self, var=DEFAULT_EMAIL_ENV, *, default=None, backend=None, options=None):
         """parse an email URL, based on django-environ
         :param var: environment variable to use
         :param default: default value if var is unset
         :param backend: override parsed email backend
         :param options: specify email options (as dict)
@@ -394,36 +373,22 @@
         }
 
         if backend:
             config["EMAIL_BACKEND"] = backend
         elif url.scheme in EMAIL_SCHEMES:
             config["EMAIL_BACKEND"] = EMAIL_SCHEMES[url.scheme]
         else:
-            raise self.exception("Invalid email schema %s" % url.scheme)
+            raise self.exception(f"Invalid email schema {url.scheme}")
 
         if url.scheme in ("smtps", "smtp+tls"):
             config["EMAIL_USE_TLS"] = True
         elif url.scheme == "smtp+ssl":
             config["EMAIL_USE_SSL"] = True
 
-        email_options = {}
-        if url.query:
-            for key, values in parse_qs(url.query).items():
-                opt = {smart_str(key).upper(): self._int(values[0])}
-                if key.upper() in _EMAIL_BASE_OPTIONS:
-                    config.update(opt)
-                else:
-                    email_options.update(opt)
-
-        if options:
-            email_options.update(options)
-        if email_options:
-            config["OPTIONS"] = {k.upper(): v for k, v in email_options.items()}
-
-        return config
+        return self._parse_options(url.query, config, options, _EMAIL_BASE_OPTIONS)
 
     def search_url(self, var=DEFAULT_SEARCH_ENV, *, default=None, engine=None, options=None):
         """parse a search URL from environment, based on django-environ
         :param var: environment variable to use
         :param default: default value if var is unset
         :param engine: override parsed storage engine
         :param options: specify storage options (as dict)
@@ -431,73 +396,73 @@
         """
         url = urlparse(self.check_var(var, default=default))
 
         path = smart_str(url.path[1:])
         path = unquote_plus(path.split("?", 2)[0])
 
         if url.scheme not in SEARCH_SCHEMES:
-            raise self.exception("Invalid search schema %s" % url.scheme)
+            raise self.exception(f"Invalid search schema {url.scheme}")
 
-        config = {"ENGINE": engine if engine else SEARCH_SCHEMES[url.scheme]}
+        config = {"ENGINE": engine or SEARCH_SCHEMES[url.scheme]}
 
         # check common params
         params = {}
         if url.query:
             params = {smart_str(k): smart_str(v, strings_only=True) for k, v in parse_qs(url.query)}
-            if "EXCLUDED_INDEXES" in params.keys():
+            if "EXCLUDED_INDEXES" in params:
                 config["EXCLUDED_INDEXES"] = params["EXCLUDED_INDEXES"][0].split(",")
-            if "INCLUDE_SPELLING" in params.keys():
+            if "INCLUDE_SPELLING" in params:
                 config["INCLUDE_SPELLING"] = self.is_true(params["INCLUDE_SPELLING"][0])
-            if "BATCH_SIZE" in params.keys():
+            if "BATCH_SIZE" in params:
                 config["BATCH_SIZE"] = self._int(params["BATCH_SIZE"][0])
 
         if url.scheme == "simple":
             return config
         elif url.scheme in ["solr", "elasticsearch", "elasticsearch2"]:
-            if "KWARGS" in params.keys():
+            if "KWARGS" in params:
                 config["KWARGS"] = params["KWARGS"][0]
 
         # remove trailing slash
         if path.endswith("/"):
             path = path[:-1]
 
         if url.scheme == "solr":
             config["URL"] = urlunparse(("http",) + url[1:2] + (path,) + ("", "", ""))
-            if "TIMEOUT" in params.keys():
+            if "TIMEOUT" in params:
                 config["TIMEOUT"] = self._int(params["TIMEOUT"][0])
             return config
 
         if url.scheme.startswith("elasticsearch"):
             split = path.rsplit("/", 1)
 
             if len(split) > 1:
                 path = "/".join(split[:-1])
                 index = split[-1]
             else:
                 path = ""
                 index = split[0]
 
             config["URL"] = urlunparse(("http",) + url[1:2] + (path,) + ("", "", ""))
-            if "TIMEOUT" in params.keys():
+            if "TIMEOUT" in params:
                 config["TIMEOUT"] = self._int(params["TIMEOUT"][0])
             config["INDEX_NAME"] = index
         else:
-            config["PATH"] = "/" + path
+            config["PATH"] = f"/{path}"
 
             if url.scheme == "whoosh":
-                if "STORAGE" in params.keys():
+                if "STORAGE" in params:
                     config["STORAGE"] = params["STORAGE"][0]
-                if "POST_LIMIT" in params.keys():
+                if "POST_LIMIT" in params:
                     config["POST_LIMIT"] = self._int(params["POST_LIMIT"][0])
             elif url.scheme == "xapian":
-                if "FLAGS" in params.keys():
+                if "FLAGS" in params:
                     config["FLAGS"] = params["FLAGS"][0]
 
         if options:
-            config.update({k.upper(): v for k, v in options.items()})
+            config |= {k.upper(): v for k, v in options.items()}
 
         return config
 
     def queue_url(self, var=DEFAULT_QUEUE_ENV, *, default=None, backend=None, options=None):
         """
         Parse a url, mostly based on dj-database-url
         :param var: environment variable to use
@@ -519,57 +484,55 @@
 
         config = {"QUEUE_BACKEND": backend if backend is None else conf["backend"]}
 
         if url.scheme.startswith("amazon"):
             path = f"https://{url.hostname}"
             if port:
                 path += f":{port}"
-            config.update({"AWS_SQS_ENDPOINT": path})
+            config["AWS_SQS_ENDPOINT"] = path
 
         elif url.scheme.startswith("rabbit"):
             config = {
                 "QUEUE_BACKEND": backend or config["QUEUE_BACKEND"],
                 "RABBITMQ_HOST": url.hostname or "",
                 "RABBITMQ_PORT": port,
             }
             if not url.hostname:
-                config.update(
-                    {
-                        "QUEUE_LOCATION": f"unix://{url.netloc}{url.path}",
-                        "RABBITMQ_LOCATION": f"unix://{url.netloc}{url.path}",
-                        "RABBITMQ_PORT": "",
-                    }
-                )
+                config |= {
+                    "QUEUE_LOCATION": f"unix://{url.netloc}{url.path}",
+                    "RABBITMQ_LOCATION": f"unix://{url.netloc}{url.path}",
+                    "RABBITMQ_PORT": "",
+                }
 
         elif url.scheme == "redis":
             scheme = url.scheme if url.hostname else "unix"
             locations = [f"{scheme}://{loc}{url.path}" for loc in url.netloc.split(",")]
             if not backend:
-                config.update({"QUEUE_LOCATION": locations[0] if len(locations) == 1 else locations})
+                config["QUEUE_LOCATION"] = locations[0] if len(locations) == 1 else locations
 
         else:
-            config.update({"PATH": path or "", "HOST": url.hostname, "PORT": port or ""})
+            config |= {"PATH": path or "", "HOST": url.hostname, "PORT": port or ""}
 
         if url.username:
-            config.update(
-                {
-                    "USER": url.username or "",
-                    "PASSWORD": url.password or "",
-                }
-            )
+            config |= {
+                "USER": url.username or "",
+                "PASSWORD": url.password or "",
+            }
 
-        queue_options = {}
-        if url.query:
-            for key, values in parse_qs(url.query).items():
+        return self._parse_options(url.query, config, options, _QUEUE_BASE_OPTIONS)
+
+    @staticmethod
+    def _parse_options(query: str, config: dict, options: dict|None, base_options: List[str]):
+        qs_options = {}
+        if query:
+            for key, values in parse_qs(query).items():
                 opt = {smart_str(key).upper(): smart_str(values[0], strings_only=True)}
-                if key.upper() in _QUEUE_BASE_OPTIONS:
-                    config.update(opt)
+                if key.upper() in base_options:
+                    config |= opt
                 else:
-                    queue_options.update(opt)
+                    qs_options |= opt
 
-        if options:
-            queue_options.update(options)
-        if queue_options:
-            config["OPTIONS"] = {k.upper(): v for k, v in queue_options.items()}
+        qs_options.update(options or {})
+        if qs_options:
+            config["OPTIONS"] = {k.upper(): v for k, v in qs_options.items()}
 
-        # return configuration.
         return config
```

### Comparing `django_settings_env-4.7.3/pyproject.toml` & `django_settings_env-4.7.4/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "django-settings-env"
-version = "4.7.3"
+version = "4.7.4"
 description = "12-factor.net settings support for Django with .env and HashiCorp Vault support"
 authors = ["David Nugent <davidn@uniquode.io>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 Django = ">=3.1"
 envex = ">=3.0"
 django-class-settings = { version = "^0.2", optional = true }
 
 [tool.poetry.group.test.dependencies]
-pytest = ">7.0"
-pytest-cov = ">=4.1,<6.0"
+pytest = "^8.2.0"
+pytest-cov = "^5.0"
 
 [tool.poetry.group.dev.dependencies]
 ruff = "^0.4.4"
 pre-commit = "^3.3.3"
 
 [tool.poetry.extras]
 django-class-settings = ["django-class-settings"]
```

### Comparing `django_settings_env-4.7.3/PKG-INFO` & `django_settings_env-4.7.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-settings-env
-Version: 4.7.3
+Version: 4.7.4
 Summary: 12-factor.net settings support for Django with .env and HashiCorp Vault support
 Author: David Nugent
 Author-email: davidn@uniquode.io
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

