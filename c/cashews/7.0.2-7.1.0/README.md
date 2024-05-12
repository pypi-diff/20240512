# Comparing `tmp/cashews-7.0.2.tar.gz` & `tmp/cashews-7.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cashews-7.0.2.tar", last modified: Tue Mar 12 06:40:50 2024, max compression
+gzip compressed data, was "cashews-7.1.0.tar", last modified: Sun May 12 10:28:29 2024, max compression
```

## Comparing `cashews-7.0.2.tar` & `cashews-7.1.0.tar`

### file list

```diff
@@ -1,102 +1,102 @@
-drwxr-xr-x   0 dmitrykryukov   (501) staff       (20)        0 2024-03-12 06:40:50.362064 cashews-7.0.2/
--rw-r--r--   0 dmitrykryukov   (501) staff       (20)     1081 2024-02-12 21:47:12.000000 cashews-7.0.2/LICENSE
--rw-r--r--   0 dmitrykryukov   (501) staff       (20)    32693 2024-03-12 06:40:50.361333 cashews-7.0.2/PKG-INFO
--rw-r--r--   0 dmitrykryukov   (501) staff       (20)    31065 2024-02-12 21:47:12.000000 cashews-7.0.2/README.md
-drwxr-xr-x   0 dmitrykryukov   (501) staff       (20)        0 2024-03-12 06:40:50.236548 cashews-7.0.2/cashews/
--rw-r--r--   0 dmitrykryukov   (501) staff       (20)     2085 2024-03-09 13:39:00.000000 cashews-7.0.2/cashews/__init__.py
--rw-r--r--   0 dmitrykryukov   (501) staff       (20)     2033 2024-03-10 19:26:57.000000 cashews-7.0.2/cashews/_typing.py
-drwxr-xr-x   0 dmitrykryukov   (501) staff       (20)        0 2024-03-12 06:40:50.253012 cashews-7.0.2/cashews/backends/
--rw-r--r--   0 dmitrykryukov   (501) staff       (20)        0 2024-02-12 21:47:12.000000 cashews-7.0.2/cashews/backends/__init__.py
--rw-r--r--   0 dmitrykryukov   (501) staff       (20)     9317 2024-03-10 19:26:57.000000 cashews-7.0.2/cashews/backends/diskcache.py
--rw-r--r--   0 dmitrykryukov   (501) staff       (20)     6774 2024-03-10 19:26:57.000000 cashews-7.0.2/cashews/backends/interface.py
--rw-r--r--   0 dmitrykryukov   (501) staff       (20)     9232 2024-03-10 19:26:57.000000 cashews-7.0.2/cashews/backends/memory.py
-drwxr-xr-x   0 dmitrykryukov   (501) staff       (20)        0 2024-03-12 06:40:50.256298 cashews-7.0.2/cashews/backends/redis/
--rw-r--r--   0 dmitrykryukov   (501) staff       (20)      213 2024-02-12 21:47:12.000000 cashews-7.0.2/cashews/backends/redis/__init__.py
--rw-r--r--   0 dmitrykryukov   (501) staff       (20)    11174 2024-03-10 19:32:26.000000 cashews-7.0.2/cashews/backends/redis/backend.py
--rw-r--r--   0 dmitrykryukov   (501) staff       (20)     1999 2024-03-09 08:24:17.000000 cashews-7.0.2/cashews/backends/redis/client.py
--rw-r--r--   0 dmitrykryukov   (501) staff       (20)    12663 2024-03-10 19:26:57.000000 cashews-7.0.2/cashews/backends/redis/client_side.py
--rw-r--r--   0 dmitrykryukov   (501) staff       (20)    11944 2024-03-10 19:34:50.000000 cashews-7.0.2/cashews/backends/transaction.py
--rw-r--r--   0 dmitrykryukov   (501) staff       (20)     1186 2024-03-09 13:39:00.000000 cashews-7.0.2/cashews/cache_condition.py
--rw-r--r--   0 dmitrykryukov   (501) staff       (20)      920 2024-02-12 21:47:12.000000 cashews-7.0.2/cashews/commands.py
-drwxr-xr-x   0 dmitrykryukov   (501) staff       (20)        0 2024-03-12 06:40:50.262400 cashews-7.0.2/cashews/contrib/
--rw-r--r--   0 dmitrykryukov   (501) staff       (20)      109 2024-03-09 08:24:17.000000 cashews-7.0.2/cashews/contrib/__init__.py
--rw-r--r--   0 dmitrykryukov   (501) staff       (20)     1724 2024-03-09 13:39:00.000000 cashews-7.0.2/cashews/contrib/_starlette.py
--rw-r--r--   0 dmitrykryukov   (501) staff       (20)     5940 2024-03-10 19:26:57.000000 cashews-7.0.2/cashews/contrib/fastapi.py
--rw-r--r--   0 dmitrykryukov   (501) staff       (20)     1337 2024-03-10 19:26:57.000000 cashews-7.0.2/cashews/contrib/prometheus.py
-drwxr-xr-x   0 dmitrykryukov   (501) staff       (20)        0 2024-03-12 06:40:50.267909 cashews-7.0.2/cashews/decorators/
--rw-r--r--   0 dmitrykryukov   (501) staff       (20)      829 2024-02-12 21:47:12.000000 cashews-7.0.2/cashews/decorators/__init__.py
--rw-r--r--   0 dmitrykryukov   (501) staff       (20)     7546 2024-03-09 13:39:00.000000 cashews-7.0.2/cashews/decorators/bloom.py
-drwxr-xr-x   0 dmitrykryukov   (501) staff       (20)        0 2024-03-12 06:40:50.275684 cashews-7.0.2/cashews/decorators/cache/
--rw-r--r--   0 dmitrykryukov   (501) staff       (20)        0 2024-02-12 21:47:12.000000 cashews-7.0.2/cashews/decorators/cache/__init__.py
--rw-r--r--   0 dmitrykryukov   (501) staff       (20)      202 2024-02-12 21:47:12.000000 cashews-7.0.2/cashews/decorators/cache/_exception.py
--rw-r--r--   0 dmitrykryukov   (501) staff       (20)     2073 2024-03-09 13:39:00.000000 cashews-7.0.2/cashews/decorators/cache/defaults.py
--rw-r--r--   0 dmitrykryukov   (501) staff       (20)     4709 2024-03-09 13:39:00.000000 cashews-7.0.2/cashews/decorators/cache/early.py
--rw-r--r--   0 dmitrykryukov   (501) staff       (20)     2868 2024-03-09 13:39:00.000000 cashews-7.0.2/cashews/decorators/cache/fail.py
--rw-r--r--   0 dmitrykryukov   (501) staff       (20)     3805 2024-03-09 13:39:00.000000 cashews-7.0.2/cashews/decorators/cache/hit.py
--rw-r--r--   0 dmitrykryukov   (501) staff       (20)     2543 2024-03-09 13:39:00.000000 cashews-7.0.2/cashews/decorators/cache/iterator.py
--rw-r--r--   0 dmitrykryukov   (501) staff       (20)     2936 2024-03-09 13:39:00.000000 cashews-7.0.2/cashews/decorators/cache/simple.py
--rw-r--r--   0 dmitrykryukov   (501) staff       (20)     3528 2024-03-09 13:39:00.000000 cashews-7.0.2/cashews/decorators/cache/soft.py
--rw-r--r--   0 dmitrykryukov   (501) staff       (20)     3087 2024-03-09 13:39:00.000000 cashews-7.0.2/cashews/decorators/circuit_breaker.py
--rw-r--r--   0 dmitrykryukov   (501) staff       (20)     3397 2024-03-09 08:24:17.000000 cashews-7.0.2/cashews/decorators/locked.py
--rw-r--r--   0 dmitrykryukov   (501) staff       (20)     2382 2024-02-12 21:47:12.000000 cashews-7.0.2/cashews/decorators/rate.py
--rw-r--r--   0 dmitrykryukov   (501) staff       (20)     2366 2024-03-09 13:39:00.000000 cashews-7.0.2/cashews/decorators/rate_slide.py
--rw-r--r--   0 dmitrykryukov   (501) staff       (20)      957 2024-03-09 08:24:17.000000 cashews-7.0.2/cashews/exceptions.py
--rw-r--r--   0 dmitrykryukov   (501) staff       (20)     5298 2024-02-12 21:47:12.000000 cashews-7.0.2/cashews/formatter.py
--rw-r--r--   0 dmitrykryukov   (501) staff       (20)     2411 2024-03-09 13:39:00.000000 cashews-7.0.2/cashews/helpers.py
--rw-r--r--   0 dmitrykryukov   (501) staff       (20)     5997 2024-03-10 19:26:57.000000 cashews-7.0.2/cashews/key.py
--rw-r--r--   0 dmitrykryukov   (501) staff       (20)      673 2024-03-09 13:39:00.000000 cashews-7.0.2/cashews/key_context.py
--rw-r--r--   0 dmitrykryukov   (501) staff       (20)     1984 2024-02-12 21:47:12.000000 cashews-7.0.2/cashews/picklers.py
--rw-r--r--   0 dmitrykryukov   (501) staff       (20)        0 2024-02-12 21:47:12.000000 cashews-7.0.2/cashews/py.typed
--rw-r--r--   0 dmitrykryukov   (501) staff       (20)     8398 2024-03-09 13:39:00.000000 cashews-7.0.2/cashews/serialize.py
--rw-r--r--   0 dmitrykryukov   (501) staff       (20)     1415 2024-03-09 13:39:00.000000 cashews-7.0.2/cashews/ttl.py
-drwxr-xr-x   0 dmitrykryukov   (501) staff       (20)        0 2024-03-12 06:40:50.284200 cashews-7.0.2/cashews/utils/
--rw-r--r--   0 dmitrykryukov   (501) staff       (20)      273 2024-02-12 21:47:12.000000 cashews-7.0.2/cashews/utils/__init__.py
--rw-r--r--   0 dmitrykryukov   (501) staff       (20)     1376 2024-03-10 19:33:27.000000 cashews-7.0.2/cashews/utils/_bitarray.py
--rw-r--r--   0 dmitrykryukov   (501) staff       (20)     1674 2024-03-10 19:31:01.000000 cashews-7.0.2/cashews/utils/_bitarray_lib.py
--rw-r--r--   0 dmitrykryukov   (501) staff       (20)      922 2024-03-09 13:39:00.000000 cashews-7.0.2/cashews/utils/object_size.py
--rw-r--r--   0 dmitrykryukov   (501) staff       (20)      927 2024-02-12 21:47:12.000000 cashews-7.0.2/cashews/utils/split_hash.py
--rw-r--r--   0 dmitrykryukov   (501) staff       (20)     2043 2024-03-09 13:39:00.000000 cashews-7.0.2/cashews/validation.py
-drwxr-xr-x   0 dmitrykryukov   (501) staff       (20)        0 2024-03-12 06:40:50.296059 cashews-7.0.2/cashews/wrapper/
--rw-r--r--   0 dmitrykryukov   (501) staff       (20)      651 2024-02-12 21:47:12.000000 cashews-7.0.2/cashews/wrapper/__init__.py
--rw-r--r--   0 dmitrykryukov   (501) staff       (20)      623 2024-02-12 21:47:12.000000 cashews-7.0.2/cashews/wrapper/auto_init.py
--rw-r--r--   0 dmitrykryukov   (501) staff       (20)     2772 2024-03-09 13:39:00.000000 cashews-7.0.2/cashews/wrapper/backend_settings.py
--rw-r--r--   0 dmitrykryukov   (501) staff       (20)     1979 2024-03-09 13:39:00.000000 cashews-7.0.2/cashews/wrapper/callback.py
--rw-r--r--   0 dmitrykryukov   (501) staff       (20)     7460 2024-03-10 19:26:57.000000 cashews-7.0.2/cashews/wrapper/commands.py
--rw-r--r--   0 dmitrykryukov   (501) staff       (20)    12941 2024-03-09 13:39:00.000000 cashews-7.0.2/cashews/wrapper/decorators.py
--rw-r--r--   0 dmitrykryukov   (501) staff       (20)     1646 2024-03-10 19:26:57.000000 cashews-7.0.2/cashews/wrapper/disable_control.py
--rw-r--r--   0 dmitrykryukov   (501) staff       (20)     4786 2024-03-09 13:39:00.000000 cashews-7.0.2/cashews/wrapper/tags.py
--rw-r--r--   0 dmitrykryukov   (501) staff       (20)      961 2024-03-09 13:39:00.000000 cashews-7.0.2/cashews/wrapper/time_condition.py
--rw-r--r--   0 dmitrykryukov   (501) staff       (20)     4349 2024-03-09 13:39:00.000000 cashews-7.0.2/cashews/wrapper/transaction.py
--rw-r--r--   0 dmitrykryukov   (501) staff       (20)     3257 2024-03-10 19:26:57.000000 cashews-7.0.2/cashews/wrapper/wrapper.py
-drwxr-xr-x   0 dmitrykryukov   (501) staff       (20)        0 2024-03-12 06:40:50.331780 cashews-7.0.2/cashews.egg-info/
--rw-r--r--   0 dmitrykryukov   (501) staff       (20)    32693 2024-03-12 06:40:50.000000 cashews-7.0.2/cashews.egg-info/PKG-INFO
--rw-r--r--   0 dmitrykryukov   (501) staff       (20)     2441 2024-03-12 06:40:50.000000 cashews-7.0.2/cashews.egg-info/SOURCES.txt
--rw-r--r--   0 dmitrykryukov   (501) staff       (20)        1 2024-03-12 06:40:50.000000 cashews-7.0.2/cashews.egg-info/dependency_links.txt
--rw-r--r--   0 dmitrykryukov   (501) staff       (20)        1 2024-03-12 06:40:50.000000 cashews-7.0.2/cashews.egg-info/not-zip-safe
--rw-r--r--   0 dmitrykryukov   (501) staff       (20)      202 2024-03-12 06:40:50.000000 cashews-7.0.2/cashews.egg-info/requires.txt
--rw-r--r--   0 dmitrykryukov   (501) staff       (20)        8 2024-03-12 06:40:50.000000 cashews-7.0.2/cashews.egg-info/top_level.txt
--rw-r--r--   0 dmitrykryukov   (501) staff       (20)      313 2024-03-10 19:26:57.000000 cashews-7.0.2/pyproject.toml
--rw-r--r--   0 dmitrykryukov   (501) staff       (20)     1320 2024-03-12 06:40:50.363574 cashews-7.0.2/setup.cfg
--rw-r--r--   0 dmitrykryukov   (501) staff       (20)       52 2024-02-12 21:47:12.000000 cashews-7.0.2/setup.py
-drwxr-xr-x   0 dmitrykryukov   (501) staff       (20)        0 2024-03-12 06:40:50.330191 cashews-7.0.2/tests/
--rw-r--r--   0 dmitrykryukov   (501) staff       (20)     8541 2024-03-09 13:39:00.000000 cashews-7.0.2/tests/test_backend_commands.py
--rw-r--r--   0 dmitrykryukov   (501) staff       (20)     1484 2024-02-12 21:47:12.000000 cashews-7.0.2/tests/test_blooms.py
--rw-r--r--   0 dmitrykryukov   (501) staff       (20)     8539 2024-02-12 21:47:12.000000 cashews-7.0.2/tests/test_cache.py
--rw-r--r--   0 dmitrykryukov   (501) staff       (20)     2234 2024-03-09 08:24:17.000000 cashews-7.0.2/tests/test_cache_exception.py
--rw-r--r--   0 dmitrykryukov   (501) staff       (20)      600 2024-02-12 21:47:12.000000 cashews-7.0.2/tests/test_callback.py
--rw-r--r--   0 dmitrykryukov   (501) staff       (20)     1561 2024-03-09 13:39:00.000000 cashews-7.0.2/tests/test_circuit_breaker.py
--rw-r--r--   0 dmitrykryukov   (501) staff       (20)     6148 2024-03-10 19:26:57.000000 cashews-7.0.2/tests/test_client_side_cache.py
--rw-r--r--   0 dmitrykryukov   (501) staff       (20)     5586 2024-02-12 21:47:12.000000 cashews-7.0.2/tests/test_disable_control.py
--rw-r--r--   0 dmitrykryukov   (501) staff       (20)     2402 2024-03-09 08:24:17.000000 cashews-7.0.2/tests/test_invalidate.py
--rw-r--r--   0 dmitrykryukov   (501) staff       (20)      663 2024-02-12 21:47:12.000000 cashews-7.0.2/tests/test_iterators_cache.py
--rw-r--r--   0 dmitrykryukov   (501) staff       (20)     5838 2024-03-09 13:39:00.000000 cashews-7.0.2/tests/test_key.py
--rw-r--r--   0 dmitrykryukov   (501) staff       (20)     1899 2024-02-12 21:47:12.000000 cashews-7.0.2/tests/test_lock_decorator.py
--rw-r--r--   0 dmitrykryukov   (501) staff       (20)     2360 2024-02-12 21:47:12.000000 cashews-7.0.2/tests/test_middleware.py
--rw-r--r--   0 dmitrykryukov   (501) staff       (20)     8367 2024-03-09 08:24:17.000000 cashews-7.0.2/tests/test_pickle_serializer.py
--rw-r--r--   0 dmitrykryukov   (501) staff       (20)     2289 2024-03-10 19:26:57.000000 cashews-7.0.2/tests/test_rate_limit.py
--rw-r--r--   0 dmitrykryukov   (501) staff       (20)     2566 2024-03-10 19:26:57.000000 cashews-7.0.2/tests/test_redis_down.py
--rw-r--r--   0 dmitrykryukov   (501) staff       (20)     2830 2024-03-09 13:39:00.000000 cashews-7.0.2/tests/test_settings_url.py
--rw-r--r--   0 dmitrykryukov   (501) staff       (20)     7288 2024-03-09 08:24:17.000000 cashews-7.0.2/tests/test_tags_feature.py
--rw-r--r--   0 dmitrykryukov   (501) staff       (20)     9959 2024-03-10 19:26:57.000000 cashews-7.0.2/tests/test_transaction.py
--rw-r--r--   0 dmitrykryukov   (501) staff       (20)     2963 2024-03-09 13:39:00.000000 cashews-7.0.2/tests/test_utils.py
--rw-r--r--   0 dmitrykryukov   (501) staff       (20)     8233 2024-03-09 13:39:00.000000 cashews-7.0.2/tests/test_wrapper.py
+drwxr-xr-x   0 dmitrykryukov   (501) staff       (20)        0 2024-05-12 10:28:29.604432 cashews-7.1.0/
+-rw-r--r--   0 dmitrykryukov   (501) staff       (20)     1081 2024-02-12 21:47:12.000000 cashews-7.1.0/LICENSE
+-rw-r--r--   0 dmitrykryukov   (501) staff       (20)    33261 2024-05-12 10:28:29.604193 cashews-7.1.0/PKG-INFO
+-rw-r--r--   0 dmitrykryukov   (501) staff       (20)    31506 2024-05-12 10:12:45.000000 cashews-7.1.0/README.md
+drwxr-xr-x   0 dmitrykryukov   (501) staff       (20)        0 2024-05-12 10:28:29.555591 cashews-7.1.0/cashews/
+-rw-r--r--   0 dmitrykryukov   (501) staff       (20)     2085 2024-03-09 13:39:00.000000 cashews-7.1.0/cashews/__init__.py
+-rw-r--r--   0 dmitrykryukov   (501) staff       (20)     2033 2024-03-10 19:26:57.000000 cashews-7.1.0/cashews/_typing.py
+drwxr-xr-x   0 dmitrykryukov   (501) staff       (20)        0 2024-05-12 10:28:29.560574 cashews-7.1.0/cashews/backends/
+-rw-r--r--   0 dmitrykryukov   (501) staff       (20)        0 2024-02-12 21:47:12.000000 cashews-7.1.0/cashews/backends/__init__.py
+-rw-r--r--   0 dmitrykryukov   (501) staff       (20)     9317 2024-03-10 19:26:57.000000 cashews-7.1.0/cashews/backends/diskcache.py
+-rw-r--r--   0 dmitrykryukov   (501) staff       (20)     6774 2024-03-10 19:26:57.000000 cashews-7.1.0/cashews/backends/interface.py
+-rw-r--r--   0 dmitrykryukov   (501) staff       (20)     9212 2024-05-12 10:12:45.000000 cashews-7.1.0/cashews/backends/memory.py
+drwxr-xr-x   0 dmitrykryukov   (501) staff       (20)        0 2024-05-12 10:28:29.562967 cashews-7.1.0/cashews/backends/redis/
+-rw-r--r--   0 dmitrykryukov   (501) staff       (20)      213 2024-02-12 21:47:12.000000 cashews-7.1.0/cashews/backends/redis/__init__.py
+-rw-r--r--   0 dmitrykryukov   (501) staff       (20)    11226 2024-05-12 10:12:45.000000 cashews-7.1.0/cashews/backends/redis/backend.py
+-rw-r--r--   0 dmitrykryukov   (501) staff       (20)     1999 2024-03-09 08:24:17.000000 cashews-7.1.0/cashews/backends/redis/client.py
+-rw-r--r--   0 dmitrykryukov   (501) staff       (20)    12732 2024-05-12 10:12:45.000000 cashews-7.1.0/cashews/backends/redis/client_side.py
+-rw-r--r--   0 dmitrykryukov   (501) staff       (20)    11944 2024-03-10 19:34:50.000000 cashews-7.1.0/cashews/backends/transaction.py
+-rw-r--r--   0 dmitrykryukov   (501) staff       (20)     1186 2024-03-09 13:39:00.000000 cashews-7.1.0/cashews/cache_condition.py
+-rw-r--r--   0 dmitrykryukov   (501) staff       (20)      920 2024-02-12 21:47:12.000000 cashews-7.1.0/cashews/commands.py
+drwxr-xr-x   0 dmitrykryukov   (501) staff       (20)        0 2024-05-12 10:28:29.564784 cashews-7.1.0/cashews/contrib/
+-rw-r--r--   0 dmitrykryukov   (501) staff       (20)      136 2024-05-12 10:12:45.000000 cashews-7.1.0/cashews/contrib/__init__.py
+-rw-r--r--   0 dmitrykryukov   (501) staff       (20)     1724 2024-03-09 13:39:00.000000 cashews-7.1.0/cashews/contrib/_starlette.py
+-rw-r--r--   0 dmitrykryukov   (501) staff       (20)     6630 2024-05-12 10:12:45.000000 cashews-7.1.0/cashews/contrib/fastapi.py
+-rw-r--r--   0 dmitrykryukov   (501) staff       (20)     1337 2024-03-10 19:26:57.000000 cashews-7.1.0/cashews/contrib/prometheus.py
+drwxr-xr-x   0 dmitrykryukov   (501) staff       (20)        0 2024-05-12 10:28:29.569040 cashews-7.1.0/cashews/decorators/
+-rw-r--r--   0 dmitrykryukov   (501) staff       (20)      829 2024-02-12 21:47:12.000000 cashews-7.1.0/cashews/decorators/__init__.py
+-rw-r--r--   0 dmitrykryukov   (501) staff       (20)     7546 2024-03-09 13:39:00.000000 cashews-7.1.0/cashews/decorators/bloom.py
+drwxr-xr-x   0 dmitrykryukov   (501) staff       (20)        0 2024-05-12 10:28:29.574809 cashews-7.1.0/cashews/decorators/cache/
+-rw-r--r--   0 dmitrykryukov   (501) staff       (20)        0 2024-02-12 21:47:12.000000 cashews-7.1.0/cashews/decorators/cache/__init__.py
+-rw-r--r--   0 dmitrykryukov   (501) staff       (20)      202 2024-02-12 21:47:12.000000 cashews-7.1.0/cashews/decorators/cache/_exception.py
+-rw-r--r--   0 dmitrykryukov   (501) staff       (20)     2073 2024-03-09 13:39:00.000000 cashews-7.1.0/cashews/decorators/cache/defaults.py
+-rw-r--r--   0 dmitrykryukov   (501) staff       (20)     4709 2024-03-09 13:39:00.000000 cashews-7.1.0/cashews/decorators/cache/early.py
+-rw-r--r--   0 dmitrykryukov   (501) staff       (20)     2868 2024-03-09 13:39:00.000000 cashews-7.1.0/cashews/decorators/cache/fail.py
+-rw-r--r--   0 dmitrykryukov   (501) staff       (20)     3805 2024-03-09 13:39:00.000000 cashews-7.1.0/cashews/decorators/cache/hit.py
+-rw-r--r--   0 dmitrykryukov   (501) staff       (20)     2543 2024-03-09 13:39:00.000000 cashews-7.1.0/cashews/decorators/cache/iterator.py
+-rw-r--r--   0 dmitrykryukov   (501) staff       (20)     2936 2024-03-09 13:39:00.000000 cashews-7.1.0/cashews/decorators/cache/simple.py
+-rw-r--r--   0 dmitrykryukov   (501) staff       (20)     3528 2024-03-09 13:39:00.000000 cashews-7.1.0/cashews/decorators/cache/soft.py
+-rw-r--r--   0 dmitrykryukov   (501) staff       (20)     3087 2024-03-09 13:39:00.000000 cashews-7.1.0/cashews/decorators/circuit_breaker.py
+-rw-r--r--   0 dmitrykryukov   (501) staff       (20)     3397 2024-03-09 08:24:17.000000 cashews-7.1.0/cashews/decorators/locked.py
+-rw-r--r--   0 dmitrykryukov   (501) staff       (20)     2382 2024-02-12 21:47:12.000000 cashews-7.1.0/cashews/decorators/rate.py
+-rw-r--r--   0 dmitrykryukov   (501) staff       (20)     2366 2024-03-09 13:39:00.000000 cashews-7.1.0/cashews/decorators/rate_slide.py
+-rw-r--r--   0 dmitrykryukov   (501) staff       (20)      957 2024-03-09 08:24:17.000000 cashews-7.1.0/cashews/exceptions.py
+-rw-r--r--   0 dmitrykryukov   (501) staff       (20)     5321 2024-05-12 10:12:45.000000 cashews-7.1.0/cashews/formatter.py
+-rw-r--r--   0 dmitrykryukov   (501) staff       (20)     2411 2024-03-09 13:39:00.000000 cashews-7.1.0/cashews/helpers.py
+-rw-r--r--   0 dmitrykryukov   (501) staff       (20)     5997 2024-03-10 19:26:57.000000 cashews-7.1.0/cashews/key.py
+-rw-r--r--   0 dmitrykryukov   (501) staff       (20)      673 2024-03-09 13:39:00.000000 cashews-7.1.0/cashews/key_context.py
+-rw-r--r--   0 dmitrykryukov   (501) staff       (20)     1984 2024-02-12 21:47:12.000000 cashews-7.1.0/cashews/picklers.py
+-rw-r--r--   0 dmitrykryukov   (501) staff       (20)        0 2024-02-12 21:47:12.000000 cashews-7.1.0/cashews/py.typed
+-rw-r--r--   0 dmitrykryukov   (501) staff       (20)     8428 2024-05-12 10:12:45.000000 cashews-7.1.0/cashews/serialize.py
+-rw-r--r--   0 dmitrykryukov   (501) staff       (20)     1415 2024-03-09 13:39:00.000000 cashews-7.1.0/cashews/ttl.py
+drwxr-xr-x   0 dmitrykryukov   (501) staff       (20)        0 2024-05-12 10:28:29.577476 cashews-7.1.0/cashews/utils/
+-rw-r--r--   0 dmitrykryukov   (501) staff       (20)      273 2024-02-12 21:47:12.000000 cashews-7.1.0/cashews/utils/__init__.py
+-rw-r--r--   0 dmitrykryukov   (501) staff       (20)     1397 2024-05-12 10:12:45.000000 cashews-7.1.0/cashews/utils/_bitarray.py
+-rw-r--r--   0 dmitrykryukov   (501) staff       (20)     1695 2024-05-12 10:12:45.000000 cashews-7.1.0/cashews/utils/_bitarray_lib.py
+-rw-r--r--   0 dmitrykryukov   (501) staff       (20)      922 2024-03-09 13:39:00.000000 cashews-7.1.0/cashews/utils/object_size.py
+-rw-r--r--   0 dmitrykryukov   (501) staff       (20)      927 2024-02-12 21:47:12.000000 cashews-7.1.0/cashews/utils/split_hash.py
+-rw-r--r--   0 dmitrykryukov   (501) staff       (20)     2043 2024-03-09 13:39:00.000000 cashews-7.1.0/cashews/validation.py
+drwxr-xr-x   0 dmitrykryukov   (501) staff       (20)        0 2024-05-12 10:28:29.584981 cashews-7.1.0/cashews/wrapper/
+-rw-r--r--   0 dmitrykryukov   (501) staff       (20)      651 2024-02-12 21:47:12.000000 cashews-7.1.0/cashews/wrapper/__init__.py
+-rw-r--r--   0 dmitrykryukov   (501) staff       (20)      623 2024-02-12 21:47:12.000000 cashews-7.1.0/cashews/wrapper/auto_init.py
+-rw-r--r--   0 dmitrykryukov   (501) staff       (20)     2772 2024-03-09 13:39:00.000000 cashews-7.1.0/cashews/wrapper/backend_settings.py
+-rw-r--r--   0 dmitrykryukov   (501) staff       (20)     1979 2024-03-09 13:39:00.000000 cashews-7.1.0/cashews/wrapper/callback.py
+-rw-r--r--   0 dmitrykryukov   (501) staff       (20)     7460 2024-03-10 19:26:57.000000 cashews-7.1.0/cashews/wrapper/commands.py
+-rw-r--r--   0 dmitrykryukov   (501) staff       (20)    12941 2024-03-09 13:39:00.000000 cashews-7.1.0/cashews/wrapper/decorators.py
+-rw-r--r--   0 dmitrykryukov   (501) staff       (20)     1646 2024-03-10 19:26:57.000000 cashews-7.1.0/cashews/wrapper/disable_control.py
+-rw-r--r--   0 dmitrykryukov   (501) staff       (20)     4294 2024-05-12 10:12:45.000000 cashews-7.1.0/cashews/wrapper/tags.py
+-rw-r--r--   0 dmitrykryukov   (501) staff       (20)      961 2024-03-09 13:39:00.000000 cashews-7.1.0/cashews/wrapper/time_condition.py
+-rw-r--r--   0 dmitrykryukov   (501) staff       (20)     4349 2024-03-09 13:39:00.000000 cashews-7.1.0/cashews/wrapper/transaction.py
+-rw-r--r--   0 dmitrykryukov   (501) staff       (20)     3257 2024-03-10 19:26:57.000000 cashews-7.1.0/cashews/wrapper/wrapper.py
+drwxr-xr-x   0 dmitrykryukov   (501) staff       (20)        0 2024-05-12 10:28:29.601405 cashews-7.1.0/cashews.egg-info/
+-rw-r--r--   0 dmitrykryukov   (501) staff       (20)    33261 2024-05-12 10:28:29.000000 cashews-7.1.0/cashews.egg-info/PKG-INFO
+-rw-r--r--   0 dmitrykryukov   (501) staff       (20)     2441 2024-05-12 10:28:29.000000 cashews-7.1.0/cashews.egg-info/SOURCES.txt
+-rw-r--r--   0 dmitrykryukov   (501) staff       (20)        1 2024-05-12 10:28:29.000000 cashews-7.1.0/cashews.egg-info/dependency_links.txt
+-rw-r--r--   0 dmitrykryukov   (501) staff       (20)        1 2024-05-12 10:28:29.000000 cashews-7.1.0/cashews.egg-info/not-zip-safe
+-rw-r--r--   0 dmitrykryukov   (501) staff       (20)      263 2024-05-12 10:28:29.000000 cashews-7.1.0/cashews.egg-info/requires.txt
+-rw-r--r--   0 dmitrykryukov   (501) staff       (20)        8 2024-05-12 10:28:29.000000 cashews-7.1.0/cashews.egg-info/top_level.txt
+-rw-r--r--   0 dmitrykryukov   (501) staff       (20)      313 2024-05-12 10:12:36.000000 cashews-7.1.0/pyproject.toml
+-rw-r--r--   0 dmitrykryukov   (501) staff       (20)     1383 2024-05-12 10:28:29.605121 cashews-7.1.0/setup.cfg
+-rw-r--r--   0 dmitrykryukov   (501) staff       (20)       52 2024-02-12 21:47:12.000000 cashews-7.1.0/setup.py
+drwxr-xr-x   0 dmitrykryukov   (501) staff       (20)        0 2024-05-12 10:28:29.600870 cashews-7.1.0/tests/
+-rw-r--r--   0 dmitrykryukov   (501) staff       (20)     8712 2024-05-12 10:12:45.000000 cashews-7.1.0/tests/test_backend_commands.py
+-rw-r--r--   0 dmitrykryukov   (501) staff       (20)     1549 2024-05-12 10:12:45.000000 cashews-7.1.0/tests/test_blooms.py
+-rw-r--r--   0 dmitrykryukov   (501) staff       (20)     8505 2024-05-12 10:12:45.000000 cashews-7.1.0/tests/test_cache.py
+-rw-r--r--   0 dmitrykryukov   (501) staff       (20)     2201 2024-05-12 10:12:45.000000 cashews-7.1.0/tests/test_cache_exception.py
+-rw-r--r--   0 dmitrykryukov   (501) staff       (20)      551 2024-05-12 10:12:45.000000 cashews-7.1.0/tests/test_callback.py
+-rw-r--r--   0 dmitrykryukov   (501) staff       (20)     1527 2024-05-12 10:12:45.000000 cashews-7.1.0/tests/test_circuit_breaker.py
+-rw-r--r--   0 dmitrykryukov   (501) staff       (20)     6146 2024-05-12 10:12:45.000000 cashews-7.1.0/tests/test_client_side_cache.py
+-rw-r--r--   0 dmitrykryukov   (501) staff       (20)     5537 2024-05-12 10:12:45.000000 cashews-7.1.0/tests/test_disable_control.py
+-rw-r--r--   0 dmitrykryukov   (501) staff       (20)     2353 2024-05-12 10:12:45.000000 cashews-7.1.0/tests/test_invalidate.py
+-rw-r--r--   0 dmitrykryukov   (501) staff       (20)      614 2024-05-12 10:12:45.000000 cashews-7.1.0/tests/test_iterators_cache.py
+-rw-r--r--   0 dmitrykryukov   (501) staff       (20)     5838 2024-03-09 13:39:00.000000 cashews-7.1.0/tests/test_key.py
+-rw-r--r--   0 dmitrykryukov   (501) staff       (20)     1865 2024-05-12 10:12:45.000000 cashews-7.1.0/tests/test_lock_decorator.py
+-rw-r--r--   0 dmitrykryukov   (501) staff       (20)     2311 2024-05-12 10:12:45.000000 cashews-7.1.0/tests/test_middleware.py
+-rw-r--r--   0 dmitrykryukov   (501) staff       (20)     8295 2024-05-12 10:12:45.000000 cashews-7.1.0/tests/test_pickle_serializer.py
+-rw-r--r--   0 dmitrykryukov   (501) staff       (20)     2255 2024-05-12 10:12:45.000000 cashews-7.1.0/tests/test_rate_limit.py
+-rw-r--r--   0 dmitrykryukov   (501) staff       (20)     2560 2024-05-12 10:12:45.000000 cashews-7.1.0/tests/test_redis_down.py
+-rw-r--r--   0 dmitrykryukov   (501) staff       (20)     2826 2024-05-12 10:12:45.000000 cashews-7.1.0/tests/test_settings_url.py
+-rw-r--r--   0 dmitrykryukov   (501) staff       (20)     7672 2024-05-12 10:12:45.000000 cashews-7.1.0/tests/test_tags_feature.py
+-rw-r--r--   0 dmitrykryukov   (501) staff       (20)     9925 2024-05-12 10:12:45.000000 cashews-7.1.0/tests/test_transaction.py
+-rw-r--r--   0 dmitrykryukov   (501) staff       (20)     2963 2024-03-09 13:39:00.000000 cashews-7.1.0/tests/test_utils.py
+-rw-r--r--   0 dmitrykryukov   (501) staff       (20)     8199 2024-05-12 10:12:45.000000 cashews-7.1.0/tests/test_wrapper.py
```

### Comparing `cashews-7.0.2/LICENSE` & `cashews-7.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cashews-7.0.2/PKG-INFO` & `cashews-7.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cashews
-Version: 7.0.2
+Version: 7.1.0
 Summary: cache tools with async power
 Home-page: https://github.com/Krukov/cashews/
 Author: Dmitry Kryukov
 Author-email: glebov.ru@gmail.com
 License: MIT
 Keywords: cache aio async multicache aiocache
 Classifier: Development Status :: 5 - Production/Stable
@@ -33,17 +33,19 @@
 Requires-Dist: hiredis; extra == "speedup"
 Provides-Extra: dill
 Requires-Dist: dill; extra == "dill"
 Provides-Extra: lint
 Requires-Dist: mypy>=1.5.0; extra == "lint"
 Requires-Dist: types-redis; extra == "lint"
 Provides-Extra: tests
-Requires-Dist: pytest; extra == "tests"
-Requires-Dist: pytest-asyncio==0.21.1; extra == "tests"
-Requires-Dist: hypothesis; extra == "tests"
+Requires-Dist: pytest==8.2.0; extra == "tests"
+Requires-Dist: pytest-asyncio==0.23.6; extra == "tests"
+Requires-Dist: pytest-cov==5.0.0; extra == "tests"
+Requires-Dist: pytest-rerunfailures==14.0; extra == "tests"
+Requires-Dist: hypothesis==6.100.2; extra == "tests"
 
 <h1 align="center">🥔 CASHEWS 🥔</h1>
 
 <p align="center">
     <em>Async cache framework with simple API to build fast and reliable applications</em>
 </p>
 
@@ -71,15 +73,15 @@
 - Support for multiple storage backends ([In-memory](#in-memory), [Redis](#redis), [DiskCache](diskcache))
 - Set TTL as a string ("2h5m"), as `timedelta` or use a function in case TTL depends on key parameters
 - Transactionality
 - Middlewares
 - Client-side cache (10x faster than simple cache with redis)
 - Bloom filters
 - Different cache invalidation techniques (time-based or tags)
-- Cache any objects securely with pickle (use [hash key](#redis))
+- Cache any objects securely with pickle (use [secret](#redis))
 - 2x faster than `aiocache` (with client side caching)
 
 ## Usage Example
 
 ```python
 from cashews import cache
 
@@ -123,17 +125,17 @@
 
 `cashews` provides a default cache, that you can setup in two different ways:
 
 ```python
 from cashews import cache
 
 # via url
-cache.setup("redis://0.0.0.0/?db=1&socket_connect_timeout=0.5&suppress=0&hash_key=my_secret&enable=1")
+cache.setup("redis://0.0.0.0/?db=1&socket_connect_timeout=0.5&suppress=0&secret=my_secret&enable=1")
 # or via kwargs
-cache.setup("redis://0.0.0.0/", db=1, wait_for_connection_timeout=0.5, suppress=False, hash_key=b"my_key", enable=True)
+cache.setup("redis://0.0.0.0/", db=1, wait_for_connection_timeout=0.5, suppress=False, secret=b"my_key", enable=True)
 ```
 
 Alternatively, you can create a cache instance yourself:
 
 ```python
 from cashews import Cache
 
@@ -195,16 +197,16 @@
 Any connection errors are suppressed, to disable it use `suppress=False` - a `CacheBackendInteractionError` will be raised
 
 If you would like to use [client-side cache](https://redis.io/topics/client-side-caching) set `client_side=True`
 
 Client side cache will add `cashews:` prefix for each key, to customize it use `client_side_prefix` option.
 
 ```python
-cache.setup("redis://0.0.0.0/?db=1&minsize=10&suppress=false&hash_key=my_secret", prefix="func")
-cache.setup("redis://0.0.0.0/2", password="my_pass", socket_connect_timeout=0.1, retry_on_timeout=True, hash_key="my_secret")
+cache.setup("redis://0.0.0.0/?db=1&minsize=10&suppress=false&secret=my_secret", prefix="func")
+cache.setup("redis://0.0.0.0/2", password="my_pass", socket_connect_timeout=0.1, retry_on_timeout=True, secret="my_secret")
 cache.setup("redis://0.0.0.0", client_side=True, client_side_prefix="my_prefix:", pickle_type="dill")
 ```
 
 For using secure connections to redis (over ssl) uri should have `rediss` as schema
 
 ```python
 cache.setup("rediss://0.0.0.0/", ssl_ca_certs="path/to/ca.crt", ssl_keyfile="path/to/client.key",ssl_certfile="path/to/client.crt",)
@@ -835,14 +837,23 @@
 async def items(page=1):
     ...
 ```
 
 Cashews provide the tag system: you can tag cache keys, so they will be stored in a separate [SET](https://redis.io/docs/data-types/sets/)
 to avoid high load on redis storage. To use the tags in a more efficient way please use it with the client side feature.
 
+> :warning: \*\*Warning: Tags require setting up default cache or cache for tags prefix
+> ```python
+> from cashews import cache
+> cache.setup(...)
+> # or
+> cache.setup_tags_backend(...)
+> ```
+
+
 ```python
 from cashews import cache
 
 cache.setup("redis://", client_side=True)
 
 @cache(ttl="1h", tags=["items", "page:{page}"])
 async def items(page=1):
@@ -1087,14 +1098,22 @@
 
 You may find a few middlewares useful that can help you to control a cache in you web application based on fastapi.
 
 1. `CacheEtagMiddleware` - middleware add Etag and check 'If-None-Match' header based on Etag
 2. `CacheRequestControlMiddleware` - middleware check and add `Cache-Control` header
 3. `CacheDeleteMiddleware` - clear cache for an endpoint based on `Clear-Site-Data` header
 
+> :warning: \*\*Warning: CacheEtagMiddleware requires setting up default cache or cache with prefix "fastapi:"
+> ```python
+> from cashews import cache
+> cache.setup(...)
+> # or
+> cache.setup(..., prefix="fastapi:")
+> ```
+
 Example:
 
 ```python
 from fastapi import FastAPI, Header, Query
 from fastapi.responses import StreamingResponse
 
 from cashews import cache
@@ -1170,12 +1189,12 @@
 
 tox // to run all tests for all python that is installed on your machine
 ```
 
 Or use `pytest`, but 2 tests always fail, it is OK:
 
 ```shell
-pip install .[tests,redis,diskcache,speedup] fastapi aiohttp requests
+pip install .[tests,redis,diskcache,speedup] fastapi aiohttp requests httpx SQLAlchemy prometheus-client
 
 pytest // run all tests with all backends
 pytest -m "not redis" // all tests without tests for redis backend
 ```
```

### Comparing `cashews-7.0.2/README.md` & `cashews-7.1.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 - Support for multiple storage backends ([In-memory](#in-memory), [Redis](#redis), [DiskCache](diskcache))
 - Set TTL as a string ("2h5m"), as `timedelta` or use a function in case TTL depends on key parameters
 - Transactionality
 - Middlewares
 - Client-side cache (10x faster than simple cache with redis)
 - Bloom filters
 - Different cache invalidation techniques (time-based or tags)
-- Cache any objects securely with pickle (use [hash key](#redis))
+- Cache any objects securely with pickle (use [secret](#redis))
 - 2x faster than `aiocache` (with client side caching)
 
 ## Usage Example
 
 ```python
 from cashews import cache
 
@@ -80,17 +80,17 @@
 
 `cashews` provides a default cache, that you can setup in two different ways:
 
 ```python
 from cashews import cache
 
 # via url
-cache.setup("redis://0.0.0.0/?db=1&socket_connect_timeout=0.5&suppress=0&hash_key=my_secret&enable=1")
+cache.setup("redis://0.0.0.0/?db=1&socket_connect_timeout=0.5&suppress=0&secret=my_secret&enable=1")
 # or via kwargs
-cache.setup("redis://0.0.0.0/", db=1, wait_for_connection_timeout=0.5, suppress=False, hash_key=b"my_key", enable=True)
+cache.setup("redis://0.0.0.0/", db=1, wait_for_connection_timeout=0.5, suppress=False, secret=b"my_key", enable=True)
 ```
 
 Alternatively, you can create a cache instance yourself:
 
 ```python
 from cashews import Cache
 
@@ -152,16 +152,16 @@
 Any connection errors are suppressed, to disable it use `suppress=False` - a `CacheBackendInteractionError` will be raised
 
 If you would like to use [client-side cache](https://redis.io/topics/client-side-caching) set `client_side=True`
 
 Client side cache will add `cashews:` prefix for each key, to customize it use `client_side_prefix` option.
 
 ```python
-cache.setup("redis://0.0.0.0/?db=1&minsize=10&suppress=false&hash_key=my_secret", prefix="func")
-cache.setup("redis://0.0.0.0/2", password="my_pass", socket_connect_timeout=0.1, retry_on_timeout=True, hash_key="my_secret")
+cache.setup("redis://0.0.0.0/?db=1&minsize=10&suppress=false&secret=my_secret", prefix="func")
+cache.setup("redis://0.0.0.0/2", password="my_pass", socket_connect_timeout=0.1, retry_on_timeout=True, secret="my_secret")
 cache.setup("redis://0.0.0.0", client_side=True, client_side_prefix="my_prefix:", pickle_type="dill")
 ```
 
 For using secure connections to redis (over ssl) uri should have `rediss` as schema
 
 ```python
 cache.setup("rediss://0.0.0.0/", ssl_ca_certs="path/to/ca.crt", ssl_keyfile="path/to/client.key",ssl_certfile="path/to/client.crt",)
@@ -792,14 +792,23 @@
 async def items(page=1):
     ...
 ```
 
 Cashews provide the tag system: you can tag cache keys, so they will be stored in a separate [SET](https://redis.io/docs/data-types/sets/)
 to avoid high load on redis storage. To use the tags in a more efficient way please use it with the client side feature.
 
+> :warning: \*\*Warning: Tags require setting up default cache or cache for tags prefix
+> ```python
+> from cashews import cache
+> cache.setup(...)
+> # or
+> cache.setup_tags_backend(...)
+> ```
+
+
 ```python
 from cashews import cache
 
 cache.setup("redis://", client_side=True)
 
 @cache(ttl="1h", tags=["items", "page:{page}"])
 async def items(page=1):
@@ -1044,14 +1053,22 @@
 
 You may find a few middlewares useful that can help you to control a cache in you web application based on fastapi.
 
 1. `CacheEtagMiddleware` - middleware add Etag and check 'If-None-Match' header based on Etag
 2. `CacheRequestControlMiddleware` - middleware check and add `Cache-Control` header
 3. `CacheDeleteMiddleware` - clear cache for an endpoint based on `Clear-Site-Data` header
 
+> :warning: \*\*Warning: CacheEtagMiddleware requires setting up default cache or cache with prefix "fastapi:"
+> ```python
+> from cashews import cache
+> cache.setup(...)
+> # or
+> cache.setup(..., prefix="fastapi:")
+> ```
+
 Example:
 
 ```python
 from fastapi import FastAPI, Header, Query
 from fastapi.responses import StreamingResponse
 
 from cashews import cache
@@ -1127,12 +1144,12 @@
 
 tox // to run all tests for all python that is installed on your machine
 ```
 
 Or use `pytest`, but 2 tests always fail, it is OK:
 
 ```shell
-pip install .[tests,redis,diskcache,speedup] fastapi aiohttp requests
+pip install .[tests,redis,diskcache,speedup] fastapi aiohttp requests httpx SQLAlchemy prometheus-client
 
 pytest // run all tests with all backends
 pytest -m "not redis" // all tests without tests for redis backend
 ```
```

### Comparing `cashews-7.0.2/cashews/__init__.py` & `cashews-7.1.0/cashews/__init__.py`

 * *Files identical despite different names*

### Comparing `cashews-7.0.2/cashews/_typing.py` & `cashews-7.1.0/cashews/_typing.py`

 * *Files identical despite different names*

### Comparing `cashews-7.0.2/cashews/backends/diskcache.py` & `cashews-7.1.0/cashews/backends/diskcache.py`

 * *Files identical despite different names*

### Comparing `cashews-7.0.2/cashews/backends/interface.py` & `cashews-7.1.0/cashews/backends/interface.py`

 * *Files identical despite different names*

### Comparing `cashews-7.0.2/cashews/backends/memory.py` & `cashews-7.1.0/cashews/backends/memory.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
 import asyncio
 import re
 import time
 from collections import OrderedDict
 from contextlib import suppress
+from copy import copy
 from typing import TYPE_CHECKING, Any, AsyncIterator, Iterable, Mapping, overload
 
 from cashews.serialize import SerializerMixin
 from cashews.utils import Bitarray, get_obj_size
 
 from .interface import NOT_EXIST, UNLIMITED, Backend
 
@@ -164,29 +165,27 @@
         return message
 
     async def get_bits(self, key: Key, *indexes: int, size: int = 1) -> tuple[int, ...]:
         array: Bitarray = await self._get(key, default=Bitarray("0"))
         return tuple(array.get(index, size) for index in indexes)
 
     async def incr_bits(self, key: Key, *indexes: int, size: int = 1, by: int = 1) -> tuple[int, ...]:
-        array: Bitarray | None = await self._get(key)
-        if array is None:
-            array = Bitarray("0")
-            self._set(key, array)
+        array: Bitarray = await self._get(key, default=Bitarray("0"))
         result = []
         for index in indexes:
             array.incr(index, size, by)
             result.append(array.get(index, size))
+        self._set(key, array)
         return tuple(result)
 
     def _set(self, key: Key, value: Value, expire: float | None = None):
         expire = time.time() + expire if expire else None
         if expire is None and key in self.store:
             expire, _ = self.store[key]
-        self.store[key] = (expire, value)
+        self.store[key] = (expire, copy(value))
         self.store.move_to_end(key)
         if len(self.store) > self.size:
             self.store.popitem(last=False)
 
     @overload
     async def _get(self, key: Key, default: Default) -> Value | Default: ...
```

### Comparing `cashews-7.0.2/cashews/backends/redis/backend.py` & `cashews-7.1.0/cashews/backends/redis/backend.py`

 * *Files 1% similar despite different names*

```diff
@@ -306,10 +306,11 @@
     async def set_pop(self, key: Key, count: int = 100) -> Iterable[str]:
         return [value.decode() for value in await self._client.spop(key, count)]  # type: ignore[union-attr]
 
     async def get_keys_count(self) -> int:
         return await self._client.dbsize()
 
     async def close(self):
-        await self._client.close()
-        await self._client.connection_pool.disconnect()
+        if self.__is_init and self._client:
+            await self._client.close()
+            await self._client.connection_pool.disconnect()
         self.__is_init = False
```

### Comparing `cashews-7.0.2/cashews/backends/redis/client.py` & `cashews-7.1.0/cashews/backends/redis/client.py`

 * *Files identical despite different names*

### Comparing `cashews-7.0.2/cashews/backends/redis/client_side.py` & `cashews-7.1.0/cashews/backends/redis/client_side.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,17 +35,23 @@
 from redis.exceptions import ConnectionError as RedisConnectionError
 
 from cashews._typing import Key, Value
 from cashews.backends.memory import Memory
 
 from . import Redis
 
+
+class _EmptyCopy:
+    def __copy__(self):
+        return self
+
+
 _REDIS_INVALIDATE_CHAN = "__redis__:invalidate"
 _empty = object()
-_empty_in_redis = object()  # set when we know that key not in redis
+_empty_in_redis = _EmptyCopy()  # set when we know that key not in redis
 _RECONNECT_WAIT = 10
 _DEFAULT_PREFIX = "cashews:"
 BCAST_ON = "CLIENT TRACKING on REDIRECT {client_id} BCAST PREFIX {prefix}"
 logger = logging.getLogger(__name__)
 
 
 class BcastClientSide(Redis):
```

### Comparing `cashews-7.0.2/cashews/backends/transaction.py` & `cashews-7.1.0/cashews/backends/transaction.py`

 * *Files identical despite different names*

### Comparing `cashews-7.0.2/cashews/cache_condition.py` & `cashews-7.1.0/cashews/cache_condition.py`

 * *Files identical despite different names*

### Comparing `cashews-7.0.2/cashews/commands.py` & `cashews-7.1.0/cashews/commands.py`

 * *Files identical despite different names*

### Comparing `cashews-7.0.2/cashews/contrib/_starlette.py` & `cashews-7.1.0/cashews/contrib/_starlette.py`

 * *Files identical despite different names*

### Comparing `cashews-7.0.2/cashews/contrib/fastapi.py` & `cashews-7.1.0/cashews/contrib/fastapi.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 from __future__ import annotations
 
 import contextlib
 from contextlib import nullcontext
 from contextvars import ContextVar
+from datetime import datetime
 from hashlib import blake2s
 from typing import Any, ContextManager, Sequence
 
 from starlette.middleware.base import BaseHTTPMiddleware, RequestResponseEndpoint
 from starlette.requests import Request
 from starlette.responses import Response
 from starlette.types import ASGIApp
 
 from cashews import Cache, Command, cache, invalidate_further
 from cashews._typing import TTL
 from cashews.picklers import DEFAULT_PICKLER
+from cashews.ttl import ttl_to_seconds
 
 _cache_max_age: ContextVar[int] = ContextVar("cache_control_max_age")
 
+PREFIX = "fastapi:"
 _CACHE_CONTROL_HEADER = "Cache-Control"
 _AGE_HEADER = "Age"
 _ETAG_HEADER = "ETag"
 _IF_NOT_MATCH_HEADER = "If-None-Match"
 _CLEAR_CACHE_HEADER = "Clear-Site-Data"
 
 _NO_CACHE = "no-cache"  # disable GET
@@ -36,15 +39,15 @@
     "CacheEtagMiddleware",
     "CacheDeleteMiddleware",
 ]
 
 
 def cache_control_ttl(default: TTL):
     def _ttl(*args, **kwargs):
-        return _cache_max_age.get(default)
+        return _cache_max_age.get(ttl_to_seconds(default))
 
     return _ttl
 
 
 class CacheRequestControlMiddleware(BaseHTTPMiddleware):
     def __init__(
         self,
@@ -59,112 +62,135 @@
         super().__init__(app)
 
     async def dispatch(self, request: Request, call_next: RequestResponseEndpoint) -> Response:
         context: ContextManager = nullcontext()
         cache_control_value = request.headers.get(_CACHE_CONTROL_HEADER)
         if request.method.lower() not in self._methods:
             return await call_next(request)
-        to_disable = self._to_disable(cache_control_value)
+        to_disable = _to_disable(cache_control_value)
         if to_disable:
             context = self._cache.disabling(*to_disable)
-        with context, self.max_age(cache_control_value), self._cache.detect as detector:
+        with context, max_age(cache_control_value), self._cache.detect as detector:
             response = await call_next(request)
             calls = detector.calls_list
             if calls:
                 key, _ = calls[0]
                 expire = await self._cache.get_expire(key)
                 if expire > 0:
                     response.headers[_CACHE_CONTROL_HEADER] = (
                         f"{_PRIVATE if self._private else _PUBLIC}, {_MAX_AGE}{expire}"
                     )
                     response.headers[_AGE_HEADER] = f"{expire}"
             else:
                 response.headers[_CACHE_CONTROL_HEADER] = _NO_CACHE
             return response
 
-    @contextlib.contextmanager
-    def max_age(self, cache_control_value: str | None):
-        if not cache_control_value:
-            yield
-            return
-        _max_age = self._get_max_age(cache_control_value)
-        reset_token = None
-        if _max_age:
-            reset_token = _cache_max_age.set(_max_age)
-        try:
-            yield
-        finally:
-            if reset_token:
-                _cache_max_age.reset(reset_token)
-
-    def _to_disable(self, cache_control_value: str | None) -> tuple[Command, ...]:
-        if cache_control_value == _NO_CACHE:
-            return (Command.GET,)
-        if cache_control_value == _NO_STORE:
-            return Command.GET, Command.SET
-        if cache_control_value and self._get_max_age(cache_control_value) == 0:
-            return Command.GET, Command.SET
-        return ()
 
-    @staticmethod
-    def _get_max_age(cache_control_value: str) -> int | None:
-        if _MAX_AGE not in cache_control_value:
-            return None
-        for cc_value_item in cache_control_value.split(","):
-            cc_value_item = cc_value_item.strip()
-            try:
-                key, value = cc_value_item.split("=")
-                if key == _MAX_AGE[:-1]:
-                    return int(value)
-            except (ValueError, TypeError):
-                continue
+@contextlib.contextmanager
+def max_age(cache_control_value: str | None):
+    if not cache_control_value:
+        yield
+        return
+    _max_age = _get_max_age(cache_control_value)
+    reset_token = None
+    if _max_age:
+        reset_token = _cache_max_age.set(_max_age)
+    try:
+        yield
+    finally:
+        if reset_token:
+            _cache_max_age.reset(reset_token)
+
+
+def _to_disable(cache_control_value: str | None) -> tuple[Command, ...]:
+    if cache_control_value == _NO_CACHE:
+        return (Command.GET,)
+    if cache_control_value == _NO_STORE:
+        return Command.GET, Command.SET
+    if cache_control_value and _get_max_age(cache_control_value) == 0:
+        return Command.GET, Command.SET
+    return ()
+
+
+def _get_max_age(cache_control_value: str) -> int | None:
+    if _MAX_AGE not in cache_control_value:
         return None
+    for cc_value_item in cache_control_value.split(","):
+        cc_value_item = cc_value_item.strip()
+        try:
+            key, value = cc_value_item.split("=")
+            if key == _MAX_AGE[:-1]:
+                return int(value)
+        except (ValueError, TypeError):
+            continue
+    return None
 
 
 class CacheEtagMiddleware(BaseHTTPMiddleware):
     def __init__(self, app: ASGIApp, cache_instance: Cache = cache):
         self._cache = cache_instance
         super().__init__(app)
 
     async def dispatch(self, request: Request, call_next: RequestResponseEndpoint):
         etag = request.headers.get(_IF_NOT_MATCH_HEADER)
-        if etag and await self._cache.exists(etag):
+        if etag and await self._cache.exists(self._get_etag_key(etag)):
             return Response(status_code=304)
 
-        set_key = None
+        set_key: None | str = None
 
         def set_callback(key: str, result: Any):
             nonlocal set_key
             set_key = key
 
         with self._cache.detect as detector, self._cache.callback(set_callback, cmd=Command.SET):
             response = await call_next(request)
             calls = detector.calls_list
             if not calls:
-                if set_key:
-                    etag = await self._get_etag(set_key)
-                    if etag:
-                        response.headers[_ETAG_HEADER] = etag
+                if set_key is not None:
+                    _etag = await self._set_etag(set_key)
+                    if _etag == etag:
+                        return Response(status_code=304)
+                    if _etag:
+                        response.headers[_ETAG_HEADER] = _etag
                 return response
 
             key, _ = calls[0]
-            etag = await self._get_etag(key)
-            if etag:
-                response.headers[_ETAG_HEADER] = etag
+            _etag = await self._set_etag(key)
+            if _etag == etag:
+                return Response(status_code=304)
+            if _etag:
+                response.headers[_ETAG_HEADER] = _etag
         return response
 
-    async def _get_etag(self, key: str) -> str:
-        data = await self._cache.get_raw(key)
-        expire = await self._cache.get_expire(key)
-        if not isinstance(data, bytes):
-            data = data.body if isinstance(data, Response) else DEFAULT_PICKLER.dumps(data)
-        etag = blake2s(data).hexdigest()
-        await self._cache.set(etag, True, expire=expire)
+    async def _set_etag(self, key: str) -> str:
+        data = await self._cache.get(key)
+        if _is_early_cache(data):
+            expire = (data[0] - datetime.utcnow()).total_seconds()  # type: ignore[index]
+        else:
+            expire = await self._cache.get_expire(key)
+        etag = _get_etag(data)
+        await self._cache.set(self._get_etag_key(etag), True, expire=expire)
         return etag
 
+    @staticmethod
+    def _get_etag_key(etag: str) -> str:
+        return f"{PREFIX}:etag:{etag}"
+
+
+def _get_etag(cached_data: Any) -> str:
+    if _is_early_cache(cached_data):
+        cached_data = cached_data[1]
+    if not isinstance(cached_data, bytes):
+        cached_data = cached_data.body if isinstance(cached_data, Response) else DEFAULT_PICKLER.dumps(cached_data)
+    return blake2s(cached_data).hexdigest()
+
+
+def _is_early_cache(data: Any) -> bool:
+    return isinstance(data, list) and isinstance(data[0], datetime)
+
 
 class CacheDeleteMiddleware(BaseHTTPMiddleware):
     async def dispatch(self, request: Request, call_next: RequestResponseEndpoint):
         if request.headers.get(_CLEAR_CACHE_HEADER) == _CLEAR_CACHE_HEADER_VALUE:
             with invalidate_further():
                 return await call_next(request)
         return await call_next(request)
```

### Comparing `cashews-7.0.2/cashews/contrib/prometheus.py` & `cashews-7.1.0/cashews/contrib/prometheus.py`

 * *Files identical despite different names*

### Comparing `cashews-7.0.2/cashews/decorators/__init__.py` & `cashews-7.1.0/cashews/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `cashews-7.0.2/cashews/decorators/bloom.py` & `cashews-7.1.0/cashews/decorators/bloom.py`

 * *Files identical despite different names*

### Comparing `cashews-7.0.2/cashews/decorators/cache/defaults.py` & `cashews-7.1.0/cashews/decorators/cache/defaults.py`

 * *Files identical despite different names*

### Comparing `cashews-7.0.2/cashews/decorators/cache/early.py` & `cashews-7.1.0/cashews/decorators/cache/early.py`

 * *Files identical despite different names*

### Comparing `cashews-7.0.2/cashews/decorators/cache/fail.py` & `cashews-7.1.0/cashews/decorators/cache/fail.py`

 * *Files identical despite different names*

### Comparing `cashews-7.0.2/cashews/decorators/cache/hit.py` & `cashews-7.1.0/cashews/decorators/cache/hit.py`

 * *Files identical despite different names*

### Comparing `cashews-7.0.2/cashews/decorators/cache/iterator.py` & `cashews-7.1.0/cashews/decorators/cache/iterator.py`

 * *Files identical despite different names*

### Comparing `cashews-7.0.2/cashews/decorators/cache/simple.py` & `cashews-7.1.0/cashews/decorators/cache/simple.py`

 * *Files identical despite different names*

### Comparing `cashews-7.0.2/cashews/decorators/cache/soft.py` & `cashews-7.1.0/cashews/decorators/cache/soft.py`

 * *Files identical despite different names*

### Comparing `cashews-7.0.2/cashews/decorators/circuit_breaker.py` & `cashews-7.1.0/cashews/decorators/circuit_breaker.py`

 * *Files identical despite different names*

### Comparing `cashews-7.0.2/cashews/decorators/locked.py` & `cashews-7.1.0/cashews/decorators/locked.py`

 * *Files identical despite different names*

### Comparing `cashews-7.0.2/cashews/decorators/rate.py` & `cashews-7.1.0/cashews/decorators/rate.py`

 * *Files identical despite different names*

### Comparing `cashews-7.0.2/cashews/decorators/rate_slide.py` & `cashews-7.1.0/cashews/decorators/rate_slide.py`

 * *Files identical despite different names*

### Comparing `cashews-7.0.2/cashews/exceptions.py` & `cashews-7.1.0/cashews/exceptions.py`

 * *Files identical despite different names*

### Comparing `cashews-7.0.2/cashews/formatter.py` & `cashews-7.1.0/cashews/formatter.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from string import Formatter
 from typing import Any, Callable, Dict, Iterable, Pattern, Tuple
 
 from . import key_context
 from ._typing import KeyOrTemplate, KeyTemplate
 
 TemplateValue = str
-_re_special_chars_map = {i: "\\" + chr(i) for i in b"()[]?*+-|^$\\.&~# \t\n\r\v\f"}
+_re_special_chars_map = {i: "\\" + chr(i) for i in b"()[]?*+-|^$\\&~# \t\n\r\v\f"}
 
 
 def _decode_bytes(value: bytes):
     try:
         return value.decode()
     except UnicodeDecodeError:
         return value.hex()
@@ -160,15 +160,16 @@
 def default_format(template: KeyTemplate, **values) -> KeyOrTemplate:
     _template_context = key_context.get()
     _template_context.update(values)
     return default_formatter.format(template, **_template_context)
 
 
 def _re_default(field_name):
-    return f"(?P<{field_name.replace('.', '_')}>.+)?"
+    field_name = field_name.split(".")[0]
+    return f"(?P<{field_name}>.+)?"
 
 
 _re_formatter = _ReplaceFormatter(default=_re_default)
 
 
 def template_to_re_pattern(template: KeyTemplate) -> Pattern:
     pattern = _re_formatter.format(template.translate(_re_special_chars_map))
```

### Comparing `cashews-7.0.2/cashews/helpers.py` & `cashews-7.1.0/cashews/helpers.py`

 * *Files identical despite different names*

### Comparing `cashews-7.0.2/cashews/key.py` & `cashews-7.1.0/cashews/key.py`

 * *Files identical despite different names*

### Comparing `cashews-7.0.2/cashews/key_context.py` & `cashews-7.1.0/cashews/key_context.py`

 * *Files identical despite different names*

### Comparing `cashews-7.0.2/cashews/picklers.py` & `cashews-7.1.0/cashews/picklers.py`

 * *Files identical despite different names*

### Comparing `cashews-7.0.2/cashews/serialize.py` & `cashews-7.1.0/cashews/serialize.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,14 +41,15 @@
         **kwargs: Any,
     ):
         super().__init__(*args, **kwargs)
         if hash_key is not _empty:
             warnings.warn(
                 "`hash_key` property was renamed to `secret` and will be removed in next release",
                 DeprecationWarning,
+                stacklevel=2,
             )
             secret = hash_key
 
         self._serializer = Serializer(check_repr=check_repr)
         if secret:
             self._serializer.set_signer(HashSigner(secret, digestmod))
```

### Comparing `cashews-7.0.2/cashews/ttl.py` & `cashews-7.1.0/cashews/ttl.py`

 * *Files identical despite different names*

### Comparing `cashews-7.0.2/cashews/utils/_bitarray.py` & `cashews-7.1.0/cashews/utils/_bitarray.py`

 * *Files 7% similar despite different names*

```diff
@@ -31,14 +31,16 @@
         value = min(max(0, value), 2**size - 1)
         self.set(index, value, size)
         return self
 
     def copy(self):
         return Bitarray(str(self), 2)
 
+    __copy__ = copy
+
     def to_int(self):
         return self._value
 
     def __str__(self):
         return f"{self._value:b}"
 
     def __eq__(self, other):
```

### Comparing `cashews-7.0.2/cashews/utils/_bitarray_lib.py` & `cashews-7.1.0/cashews/utils/_bitarray_lib.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,14 +36,16 @@
         value = min(max(0, value), 2**size - 1)
         self.set(index, value, size)
         return self
 
     def copy(self):
         return Bitarray(self._value.to01(), base=2)
 
+    __copy__ = copy
+
     def to_int(self):
         return util.ba2int(self._value, False)
 
     def __str__(self):
         return self._value.to01()
 
     def __eq__(self, other):
```

### Comparing `cashews-7.0.2/cashews/utils/object_size.py` & `cashews-7.1.0/cashews/utils/object_size.py`

 * *Files identical despite different names*

### Comparing `cashews-7.0.2/cashews/utils/split_hash.py` & `cashews-7.1.0/cashews/utils/split_hash.py`

 * *Files identical despite different names*

### Comparing `cashews-7.0.2/cashews/validation.py` & `cashews-7.1.0/cashews/validation.py`

 * *Files identical despite different names*

### Comparing `cashews-7.0.2/cashews/wrapper/__init__.py` & `cashews-7.1.0/cashews/wrapper/__init__.py`

 * *Files identical despite different names*

### Comparing `cashews-7.0.2/cashews/wrapper/auto_init.py` & `cashews-7.1.0/cashews/wrapper/auto_init.py`

 * *Files identical despite different names*

### Comparing `cashews-7.0.2/cashews/wrapper/backend_settings.py` & `cashews-7.1.0/cashews/wrapper/backend_settings.py`

 * *Files identical despite different names*

### Comparing `cashews-7.0.2/cashews/wrapper/callback.py` & `cashews-7.1.0/cashews/wrapper/callback.py`

 * *Files identical despite different names*

### Comparing `cashews-7.0.2/cashews/wrapper/commands.py` & `cashews-7.1.0/cashews/wrapper/commands.py`

 * *Files identical despite different names*

### Comparing `cashews-7.0.2/cashews/wrapper/decorators.py` & `cashews-7.1.0/cashews/wrapper/decorators.py`

 * *Files identical despite different names*

### Comparing `cashews-7.0.2/cashews/wrapper/disable_control.py` & `cashews-7.1.0/cashews/wrapper/disable_control.py`

 * *Files identical despite different names*

### Comparing `cashews-7.0.2/cashews/wrapper/tags.py` & `cashews-7.1.0/cashews/wrapper/tags.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from functools import lru_cache
 from typing import Dict, Iterable, List, Match, Optional, Pattern, Tuple
 
 from cashews._typing import TTL, Key, KeyOrTemplate, OnRemoveCallback, Tag, Tags, Value
 from cashews.backends.interface import Backend
-from cashews.exceptions import TagNotRegisteredError
 from cashews.formatter import default_format, template_to_re_pattern
 
 from .commands import CommandWrapper
 
 
 class TagsRegistry:
     def __init__(self, *args, **kwargs) -> None:
@@ -32,22 +31,14 @@
     def _match_patterns(key: Key, patterns: List[Pattern]) -> Optional[Match]:
         for pattern in patterns:
             match = pattern.fullmatch(key)
             if match:
                 return match
         return None
 
-    def check_tags_registered(self, key: Key, tags: Tags):
-        tags = set(tags)
-        key_tags = set(self.get_key_tags(key))
-        difference = tags.difference(key_tags)
-
-        if difference:
-            raise TagNotRegisteredError(f"tag: {difference} not registered: call cache.register_tag before using tags")
-
 
 class CommandsTagsWrapper(CommandWrapper):
     def __init__(self, name: str = ""):
         super().__init__(name)
         self._tags_registry = TagsRegistry()
         self._tags_key_prefix = "_tag:"
         self._on_remove_cb = self._on_remove_callback()
@@ -56,15 +47,15 @@
         return self.setup(
             settings_url,
             middlewares=middlewares,
             prefix=self._tags_key_prefix,
             **kwargs,
         )
 
-    @lru_cache(maxsize=1)
+    @lru_cache(maxsize=1)  # noqa: B019
     def _get_tags_backend(self):
         return self._get_backend(self._tags_key_prefix)
 
     @property
     def tags_backend(self):
         return self._get_tags_backend()
 
@@ -112,19 +103,17 @@
         value: Value,
         expire: Optional[TTL] = None,
         exist: Optional[bool] = None,
         tags: Tags = (),
     ) -> bool:
         _set = await super().set(key=key, value=value, expire=expire, exist=exist)
         if _set and tags:
-            self._tags_registry.check_tags_registered(key, tags)
             for tag in tags:
                 await self.set_add(self._tags_key_prefix + tag, key, expire=expire)
         return _set
 
     async def incr(self, key: Key, value: int = 1, expire: Optional[float] = None, tags: Tags = ()) -> int:
         _set = await super().incr(key=key, value=value, expire=expire)
         if _set and tags:
-            self._tags_registry.check_tags_registered(key, tags)
             for tag in tags:
                 await self.set_add(self._tags_key_prefix + tag, key, expire=expire)
         return _set
```

### Comparing `cashews-7.0.2/cashews/wrapper/time_condition.py` & `cashews-7.1.0/cashews/wrapper/time_condition.py`

 * *Files identical despite different names*

### Comparing `cashews-7.0.2/cashews/wrapper/transaction.py` & `cashews-7.1.0/cashews/wrapper/transaction.py`

 * *Files identical despite different names*

### Comparing `cashews-7.0.2/cashews/wrapper/wrapper.py` & `cashews-7.1.0/cashews/wrapper/wrapper.py`

 * *Files identical despite different names*

### Comparing `cashews-7.0.2/cashews.egg-info/PKG-INFO` & `cashews-7.1.0/cashews.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cashews
-Version: 7.0.2
+Version: 7.1.0
 Summary: cache tools with async power
 Home-page: https://github.com/Krukov/cashews/
 Author: Dmitry Kryukov
 Author-email: glebov.ru@gmail.com
 License: MIT
 Keywords: cache aio async multicache aiocache
 Classifier: Development Status :: 5 - Production/Stable
@@ -33,17 +33,19 @@
 Requires-Dist: hiredis; extra == "speedup"
 Provides-Extra: dill
 Requires-Dist: dill; extra == "dill"
 Provides-Extra: lint
 Requires-Dist: mypy>=1.5.0; extra == "lint"
 Requires-Dist: types-redis; extra == "lint"
 Provides-Extra: tests
-Requires-Dist: pytest; extra == "tests"
-Requires-Dist: pytest-asyncio==0.21.1; extra == "tests"
-Requires-Dist: hypothesis; extra == "tests"
+Requires-Dist: pytest==8.2.0; extra == "tests"
+Requires-Dist: pytest-asyncio==0.23.6; extra == "tests"
+Requires-Dist: pytest-cov==5.0.0; extra == "tests"
+Requires-Dist: pytest-rerunfailures==14.0; extra == "tests"
+Requires-Dist: hypothesis==6.100.2; extra == "tests"
 
 <h1 align="center">🥔 CASHEWS 🥔</h1>
 
 <p align="center">
     <em>Async cache framework with simple API to build fast and reliable applications</em>
 </p>
 
@@ -71,15 +73,15 @@
 - Support for multiple storage backends ([In-memory](#in-memory), [Redis](#redis), [DiskCache](diskcache))
 - Set TTL as a string ("2h5m"), as `timedelta` or use a function in case TTL depends on key parameters
 - Transactionality
 - Middlewares
 - Client-side cache (10x faster than simple cache with redis)
 - Bloom filters
 - Different cache invalidation techniques (time-based or tags)
-- Cache any objects securely with pickle (use [hash key](#redis))
+- Cache any objects securely with pickle (use [secret](#redis))
 - 2x faster than `aiocache` (with client side caching)
 
 ## Usage Example
 
 ```python
 from cashews import cache
 
@@ -123,17 +125,17 @@
 
 `cashews` provides a default cache, that you can setup in two different ways:
 
 ```python
 from cashews import cache
 
 # via url
-cache.setup("redis://0.0.0.0/?db=1&socket_connect_timeout=0.5&suppress=0&hash_key=my_secret&enable=1")
+cache.setup("redis://0.0.0.0/?db=1&socket_connect_timeout=0.5&suppress=0&secret=my_secret&enable=1")
 # or via kwargs
-cache.setup("redis://0.0.0.0/", db=1, wait_for_connection_timeout=0.5, suppress=False, hash_key=b"my_key", enable=True)
+cache.setup("redis://0.0.0.0/", db=1, wait_for_connection_timeout=0.5, suppress=False, secret=b"my_key", enable=True)
 ```
 
 Alternatively, you can create a cache instance yourself:
 
 ```python
 from cashews import Cache
 
@@ -195,16 +197,16 @@
 Any connection errors are suppressed, to disable it use `suppress=False` - a `CacheBackendInteractionError` will be raised
 
 If you would like to use [client-side cache](https://redis.io/topics/client-side-caching) set `client_side=True`
 
 Client side cache will add `cashews:` prefix for each key, to customize it use `client_side_prefix` option.
 
 ```python
-cache.setup("redis://0.0.0.0/?db=1&minsize=10&suppress=false&hash_key=my_secret", prefix="func")
-cache.setup("redis://0.0.0.0/2", password="my_pass", socket_connect_timeout=0.1, retry_on_timeout=True, hash_key="my_secret")
+cache.setup("redis://0.0.0.0/?db=1&minsize=10&suppress=false&secret=my_secret", prefix="func")
+cache.setup("redis://0.0.0.0/2", password="my_pass", socket_connect_timeout=0.1, retry_on_timeout=True, secret="my_secret")
 cache.setup("redis://0.0.0.0", client_side=True, client_side_prefix="my_prefix:", pickle_type="dill")
 ```
 
 For using secure connections to redis (over ssl) uri should have `rediss` as schema
 
 ```python
 cache.setup("rediss://0.0.0.0/", ssl_ca_certs="path/to/ca.crt", ssl_keyfile="path/to/client.key",ssl_certfile="path/to/client.crt",)
@@ -835,14 +837,23 @@
 async def items(page=1):
     ...
 ```
 
 Cashews provide the tag system: you can tag cache keys, so they will be stored in a separate [SET](https://redis.io/docs/data-types/sets/)
 to avoid high load on redis storage. To use the tags in a more efficient way please use it with the client side feature.
 
+> :warning: \*\*Warning: Tags require setting up default cache or cache for tags prefix
+> ```python
+> from cashews import cache
+> cache.setup(...)
+> # or
+> cache.setup_tags_backend(...)
+> ```
+
+
 ```python
 from cashews import cache
 
 cache.setup("redis://", client_side=True)
 
 @cache(ttl="1h", tags=["items", "page:{page}"])
 async def items(page=1):
@@ -1087,14 +1098,22 @@
 
 You may find a few middlewares useful that can help you to control a cache in you web application based on fastapi.
 
 1. `CacheEtagMiddleware` - middleware add Etag and check 'If-None-Match' header based on Etag
 2. `CacheRequestControlMiddleware` - middleware check and add `Cache-Control` header
 3. `CacheDeleteMiddleware` - clear cache for an endpoint based on `Clear-Site-Data` header
 
+> :warning: \*\*Warning: CacheEtagMiddleware requires setting up default cache or cache with prefix "fastapi:"
+> ```python
+> from cashews import cache
+> cache.setup(...)
+> # or
+> cache.setup(..., prefix="fastapi:")
+> ```
+
 Example:
 
 ```python
 from fastapi import FastAPI, Header, Query
 from fastapi.responses import StreamingResponse
 
 from cashews import cache
@@ -1170,12 +1189,12 @@
 
 tox // to run all tests for all python that is installed on your machine
 ```
 
 Or use `pytest`, but 2 tests always fail, it is OK:
 
 ```shell
-pip install .[tests,redis,diskcache,speedup] fastapi aiohttp requests
+pip install .[tests,redis,diskcache,speedup] fastapi aiohttp requests httpx SQLAlchemy prometheus-client
 
 pytest // run all tests with all backends
 pytest -m "not redis" // all tests without tests for redis backend
 ```
```

### Comparing `cashews-7.0.2/cashews.egg-info/SOURCES.txt` & `cashews-7.1.0/cashews.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cashews-7.0.2/setup.cfg` & `cashews-7.1.0/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = cashews
-version = 7.0.2
+version = 7.1.0
 url = https://github.com/Krukov/cashews/
 author = Dmitry Kryukov
 author_email = glebov.ru@gmail.com
 description = cache tools with async power
 keywords = cache aio async multicache aiocache
 long_description = file: README.md
 long_description_content_type = text/markdown
@@ -49,15 +49,17 @@
 	hiredis
 dill = 
 	dill
 lint = 
 	mypy >= 1.5.0
 	types-redis
 tests = 
-	pytest
-	pytest-asyncio==0.21.1
-	hypothesis
+	pytest==8.2.0
+	pytest-asyncio==0.23.6
+	pytest-cov==5.0.0
+	pytest-rerunfailures==14.0
+	hypothesis==6.100.2
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `cashews-7.0.2/tests/test_backend_commands.py` & `cashews-7.1.0/tests/test_backend_commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,28 +3,35 @@
 
 import pytest
 
 from cashews import Cache
 from cashews.backends.interface import NOT_EXIST, UNLIMITED
 from cashews.backends.memory import Memory
 
-pytestmark = pytest.mark.asyncio
 VALUE = Decimal("100.2")
 
 
 async def test_set_get(cache: Cache):
     await cache.set("key", VALUE)
     assert await cache.get("key") == VALUE
 
 
 async def test_set_get_bytes(cache: Cache):
     await cache.set("key", b"10")
     assert await cache.get("key") == b"10"
 
 
+async def test_mutation(cache):
+    obj = [1, 2, 3]
+    await cache.set("key", obj)
+    obj.append(4)
+    assert list(await cache.get("key")) != list(obj)
+    assert await cache.get("key") == [1, 2, 3]
+
+
 async def test_incr_get(cache: Cache):
     await cache.incr("key")
     assert await cache.get("key") == 1
 
 
 async def test_incr_value_get(cache: Cache):
     await cache.incr("key")
```

### Comparing `cashews-7.0.2/tests/test_blooms.py` & `cashews-7.1.0/tests/test_blooms.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 from unittest.mock import Mock
 
 import pytest
 
 from cashews.decorators.bloom import bloom
 
-pytestmark = pytest.mark.asyncio
+
+@pytest.fixture
+async def backend(raw_backend):
+    _backend, _ = raw_backend
+    yield _backend
 
 
 async def test_bloom_simple(cache):
     n = 100
     call = Mock()
 
     @cache.bloom(name="name:{k}", false_positives=1, capacity=n)
```

### Comparing `cashews-7.0.2/tests/test_cache.py` & `cashews-7.1.0/tests/test_cache.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 import asyncio
 from unittest.mock import Mock
 
 import pytest
 
 from cashews import Cache, decorators
 
-pytestmark = pytest.mark.asyncio
-
 EXPIRE = 0.02
 
 
 class CustomError(Exception):
     pass
```

### Comparing `cashews-7.0.2/tests/test_cache_exception.py` & `cashews-7.1.0/tests/test_cache_exception.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from unittest.mock import Mock
 
 import pytest
 
 from cashews import Cache, only_exceptions, with_exceptions
 
-pytestmark = pytest.mark.asyncio
 EXPIRE = 0.1
 
 
 class CustomError(Exception):
     pass
```

### Comparing `cashews-7.0.2/tests/test_callback.py` & `cashews-7.1.0/tests/test_callback.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,12 @@
 from unittest.mock import Mock
 
-import pytest
-
 from cashews.commands import Command
 from cashews.wrapper import Cache
 
-pytestmark = pytest.mark.asyncio
-
 
 async def test_with_callback_on_set(cache: Cache):
     call = Mock()
 
     with cache.callback(callback=call, cmd=Command.SET):
         await cache.set("test", "value")
```

### Comparing `cashews-7.0.2/tests/test_circuit_breaker.py` & `cashews-7.1.0/tests/test_circuit_breaker.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 import asyncio
 
 import pytest
 
 from cashews.exceptions import CircuitBreakerOpen
 
-pytestmark = pytest.mark.asyncio
-
 EXPIRE = 0.02
 
 
 class CustomError(Exception):
     pass
```

### Comparing `cashews-7.0.2/tests/test_client_side_cache.py` & `cashews-7.1.0/tests/test_client_side_cache.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 
 @pytest.fixture(name="create_cache")
 def _create_cache(redis_dsn, backend_factory):
     from cashews.backends.redis.client_side import BcastClientSide
 
     async def call(local_cache=None):
-        backend = backend_factory(BcastClientSide, redis_dsn, hash_key=None, local_cache=local_cache)
+        backend = backend_factory(BcastClientSide, redis_dsn, secret=None, local_cache=local_cache)
         await backend.init()
         await backend.clear()
         return backend
 
     return call
```

### Comparing `cashews-7.0.2/tests/test_disable_control.py` & `cashews-7.1.0/tests/test_disable_control.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,14 @@
 import asyncio
 from random import random
 from unittest.mock import Mock
 
-import pytest
-
 from cashews.commands import Command
 from cashews.wrapper import Cache
 
-pytestmark = pytest.mark.asyncio
-
 
 async def test_disable_cmd(cache):
     cache.disable(Command.INCR)
     await cache.set("test", 10)
     await cache.incr("test")
     assert await cache.get("test") == 10
```

### Comparing `cashews-7.0.2/tests/test_invalidate.py` & `cashews-7.1.0/tests/test_invalidate.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,13 @@
 import asyncio
 import random
 
-import pytest
-
 from cashews import Cache
 from cashews.validation import invalidate_further
 
-pytestmark = pytest.mark.asyncio
-
 
 async def test_invalidate_decor_str(cache: Cache):
     @cache(ttl=1, key="key:{arg}")
     async def func(arg):
         return random.random()
 
     @cache.invalidate("key:{arg}")
```

### Comparing `cashews-7.0.2/tests/test_iterators_cache.py` & `cashews-7.1.0/tests/test_iterators_cache.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,12 @@
 import asyncio
 from unittest.mock import Mock
 
-import pytest
-
 from cashews import Cache
 
-pytestmark = pytest.mark.asyncio
-
 
 async def test_iterator(cache: Cache):
     chunks = [b"a", b"b", b"c", b"d"]
     call = Mock()
 
     @cache.iterator(ttl=10, key="iterator")
     async def func():
```

### Comparing `cashews-7.0.2/tests/test_key.py` & `cashews-7.1.0/tests/test_key.py`

 * *Files identical despite different names*

### Comparing `cashews-7.0.2/tests/test_lock_decorator.py` & `cashews-7.1.0/tests/test_lock_decorator.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,14 @@
 from unittest.mock import Mock
 
 import pytest
 
 from cashews import decorators
 from cashews.backends.memory import Memory
 
-pytestmark = pytest.mark.asyncio
-
 
 async def test_lock_cache_parallel(cache):
     mock = Mock()
 
     @cache.locked(key="key", wait=False, ttl=10)
     async def func():
         await asyncio.sleep(0.1)
```

### Comparing `cashews-7.0.2/tests/test_middleware.py` & `cashews-7.1.0/tests/test_middleware.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,10 @@
-import pytest
-
 from cashews import Cache
 from cashews.helpers import add_prefix, all_keys_lower, memory_limit
 
-pytestmark = pytest.mark.asyncio
-
 
 async def test_all_keys_lower(cache: Cache, target):
     cache._add_backend(target, (all_keys_lower(),))
     await cache.get(key="KEY")
     target.get.assert_called_once_with(key="key", default=None)
 
     await cache.set(key="KEY", value="value")
```

### Comparing `cashews-7.0.2/tests/test_pickle_serializer.py` & `cashews-7.1.0/tests/test_pickle_serializer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,30 @@
 import dataclasses
 from collections import namedtuple
 from datetime import date, datetime, timedelta
 from decimal import Decimal
 
 import pytest
-import pytest_asyncio
 from hypothesis import example, given, settings
 from hypothesis import strategies as st
 
 from cashews.backends.memory import Memory
 from cashews.serialize import UnSecureDataError
 
-pytestmark = pytest.mark.asyncio
-
 
 @dataclasses.dataclass()
 class TestDC:
     test: str
     _: int
 
 
 NT = namedtuple("NT", ("test", "name"), defaults=[False, "test"])
 
 
-@pytest_asyncio.fixture(
+@pytest.fixture(
     name="cache",
     params=[
         "default_md5",
         "default_sum",
         "default_sha256",
         pytest.param("redis_md5", marks=pytest.mark.redis),
         pytest.param("redis_sum", marks=pytest.mark.redis),
@@ -36,21 +33,21 @@
     ],
 )
 async def _cache(request, redis_dsn):
     pickle_type, digestmod = request.param.split("_")
     if pickle_type == "redis":
         from cashews.backends.redis import Redis
 
-        redis = Redis(redis_dsn, hash_key="test", safe=False, digestmod=digestmod)
+        redis = Redis(redis_dsn, secret="test", safe=False, digestmod=digestmod)
         await redis.init()
         await redis.clear()
         yield redis
         await redis.close()
     else:
-        yield Memory(hash_key=b"test", digestmod=digestmod, pickle_type=pickle_type)
+        yield Memory(secret=b"test", digestmod=digestmod, pickle_type=pickle_type)
 
 
 @pytest.mark.parametrize(
     "value",
     (
         "test",
         b"test",
@@ -270,26 +267,26 @@
     cache = Memory()
     await cache.set(key, value)
     assert await cache.get(key) == value
 
 
 async def test_cache_from_hash_to_no_hash():
     val = Decimal("10.2")
-    cache = Memory(hash_key="test")
+    cache = Memory(secret="test")
     await cache.set("key", val)
 
     assert await cache.get("key") == val
     cache_no_hash = Memory()
     cache_no_hash.store = cache.store
     assert await cache_no_hash.get("key", default="default") == "default"
 
 
 async def test_cache_from_no_hash_to_hash():
     val = Decimal("10.2")
     cache = Memory()
     await cache.set("key", val)
 
     assert await cache.get("key") == val
-    cache_hash = Memory(hash_key="test")
+    cache_hash = Memory(secret="test")
     cache_hash.store = cache.store
 
     assert await cache_hash.get("key") == val
```

### Comparing `cashews-7.0.2/tests/test_rate_limit.py` & `cashews-7.1.0/tests/test_rate_limit.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,16 +2,14 @@
 import uuid
 from unittest.mock import Mock
 
 import pytest
 
 from cashews.exceptions import RateLimitError
 
-pytestmark = pytest.mark.asyncio
-
 
 @pytest.mark.parametrize("n", list(range(1, 10)))
 async def test_rate_limit_simple(cache, n):
     @cache.rate_limit(limit=n, period=1, prefix=str(uuid.uuid4()))
     async def func():
         return 1
```

### Comparing `cashews-7.0.2/tests/test_redis_down.py` & `cashews-7.1.0/tests/test_redis_down.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 def redis_backend():
     from cashews.backends.redis import Redis
 
     return Redis
 
 
 async def test_safe_redis(redis_backend):
-    redis = redis_backend(safe=True, address="redis://localhost:9223", hash_key=None)
+    redis = redis_backend(safe=True, address="redis://localhost:9223", secret=None)
     await redis.init()
 
     assert await redis.set("test", "test") is False
     assert await redis.set_raw("test", "test") is False
 
     assert await redis.set_lock("test", "test", 1) is False
     assert await redis.unlock("test", "test") is None
@@ -48,26 +48,26 @@
     await redis.delete_match("*")
 
     with pytest.raises(CacheBackendInteractionError):
         await redis.ping()
 
 
 async def test_unsafe_redis_down(redis_backend):
-    redis = redis_backend(safe=False, address="redis://localhost:9223", hash_key=None)
+    redis = redis_backend(safe=False, address="redis://localhost:9223", secret=None)
     await redis.init()
     with pytest.raises(CacheBackendInteractionError):
         await redis.ping()
     with pytest.raises(CacheBackendInteractionError):
         await redis.set("key", "value")
 
 
 async def test_cache_decorators_on_redis_down(redis_backend):
     mock = Mock(return_value="val")
     cache = Cache()
-    cache._add_backend(redis_backend(safe=True, address="redis://localhost:9223", hash_key=None))
+    cache._add_backend(redis_backend(safe=True, address="redis://localhost:9223", secret=None))
 
     @cache(ttl=1)
     @cache.failover(1)
     @cache.hit(ttl=1, cache_hits=1)
     @cache.circuit_breaker(ttl=1, errors_rate=1, period=1)
     @cache.rate_limit(ttl=1, limit=1, period=1)
     @cache.early(ttl=1)
```

### Comparing `cashews-7.0.2/tests/test_settings_url.py` & `cashews-7.1.0/tests/test_settings_url.py`

 * *Files 11% similar despite different names*

```diff
@@ -54,18 +54,18 @@
             "redis://localhost/0/?password=password",
             {
                 "address": "redis://localhost/0/",
                 "password": "password",
             },
         ),
         (
-            "redis://localhost/0/?hash_key=secret&password=test&safe=1&minsize=3&create_connection_timeout=0.1",  # noqa: E501
+            "redis://localhost/0/?secret=secret&password=test&safe=1&minsize=3&create_connection_timeout=0.1",  # noqa: E501
             {
                 "address": "redis://localhost/0/",
-                "hash_key": "secret",
+                "secret": "secret",
                 "password": "test",
                 "safe": True,
                 "minsize": 3,
                 "create_connection_timeout": 0.1,
             },
         ),
         (
```

### Comparing `cashews-7.0.2/tests/test_tags_feature.py` & `cashews-7.1.0/tests/test_tags_feature.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,16 +3,14 @@
 from typing import Union
 from unittest.mock import AsyncMock
 
 import pytest
 
 from cashews import Cache, key_context
 
-pytestmark = pytest.mark.asyncio
-
 
 def test_register_tags(cache: Cache):
     cache.register_tag("tag", "key")
     cache.register_tag("tag_template", "key{i}")
     cache.register_tag("tag_test:{i}", "key{i:len}:test")
     cache.register_tag("tag_func:{i:hash}", "key{i}:test")
     cache.register_tag("tag_context:{val}", "key{i}:test")
@@ -239,7 +237,23 @@
     async def cached(
         a: int,
         b: Union[int, None] = None,
     ) -> str:
         return f"{a}{b}"
 
     assert await cached(1) == "1None"
+
+
+async def test_template_tag_function(cache: Cache):
+    @cache(ttl="1m", key="{user.name:hash}:func", tags=["tag:{user.name}", "tag:{user.name:hash}"])
+    async def func(user):
+        return random()
+
+    class User:
+        def __init__(self, name):
+            self.name = name
+
+        def __hash__(self):
+            return hash(self.name)
+
+    await func(User("test"))
+    await cache.delete_tags("tag:test")
```

### Comparing `cashews-7.0.2/tests/test_transaction.py` & `cashews-7.1.0/tests/test_transaction.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,16 +4,14 @@
 import pytest
 
 from cashews import LockedError
 from cashews.backends.interface import NOT_EXIST, UNLIMITED
 from cashews.wrapper import Cache
 from cashews.wrapper.transaction import TransactionMode
 
-pytestmark = pytest.mark.asyncio
-
 
 @pytest.fixture(
     name="tx_mode",
     params=[
         TransactionMode.FAST,
         TransactionMode.LOCKED,
         TransactionMode.SERIALIZABLE,
```

### Comparing `cashews-7.0.2/tests/test_utils.py` & `cashews-7.1.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `cashews-7.0.2/tests/test_wrapper.py` & `cashews-7.1.0/tests/test_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,16 +5,14 @@
 
 from cashews.backends.memory import Memory
 from cashews.cache_condition import NOT_NONE
 from cashews.exceptions import NotConfiguredError
 from cashews.wrapper import Cache
 from cashews.wrapper.auto_init import create_auto_init
 
-pytestmark = pytest.mark.asyncio
-
 
 async def test_prefix_many(cache):
     await cache.init("mem://")
     await cache.init("mem://", prefix="-")
 
     await cache.set("key", "value")
     await cache.set("-:key", "-value")
```

