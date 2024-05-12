# Comparing `tmp/picodi-0.6.0.tar.gz` & `tmp/picodi-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "picodi-0.6.0.tar", max compression
+gzip compressed data, was "picodi-0.7.0.tar", max compression
```

## Comparing `picodi-0.6.0.tar` & `picodi-0.7.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1064 2024-05-11 14:33:47.444728 picodi-0.6.0/LICENSE
--rw-r--r--   0        0        0     7352 2024-05-11 14:33:47.444728 picodi-0.6.0/README.md
--rw-r--r--   0        0        0      266 2024-05-11 14:33:47.444728 picodi-0.6.0/picodi/__init__.py
--rw-r--r--   0        0        0     2005 2024-05-11 14:33:47.444728 picodi-0.6.0/picodi/_internal.py
--rw-r--r--   0        0        0    10133 2024-05-11 14:33:47.444728 picodi-0.6.0/picodi/_picodi.py
--rw-r--r--   0        0        0     1284 2024-05-11 14:33:47.444728 picodi-0.6.0/picodi/_scopes.py
--rw-r--r--   0        0        0     1649 2024-05-11 14:33:47.444728 picodi-0.6.0/picodi/helpers.py
--rw-r--r--   0        0        0        0 2024-05-11 14:33:47.444728 picodi-0.6.0/picodi/py.typed
--rw-r--r--   0        0        0     2604 2024-05-11 14:33:47.448727 picodi-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     8114 1970-01-01 00:00:00.000000 picodi-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-05-12 19:05:12.108964 picodi-0.7.0/LICENSE
+-rw-r--r--   0        0        0    10134 2024-05-12 19:05:12.108964 picodi-0.7.0/README.md
+-rw-r--r--   0        0        0      252 2024-05-12 19:05:12.108964 picodi-0.7.0/picodi/__init__.py
+-rw-r--r--   0        0        0     1900 2024-05-12 19:05:12.108964 picodi-0.7.0/picodi/_internal.py
+-rw-r--r--   0        0        0    13996 2024-05-12 19:05:12.108964 picodi-0.7.0/picodi/_picodi.py
+-rw-r--r--   0        0        0     1284 2024-05-12 19:05:12.108964 picodi-0.7.0/picodi/_scopes.py
+-rw-r--r--   0        0        0     1625 2024-05-12 19:05:12.112964 picodi-0.7.0/picodi/helpers.py
+-rw-r--r--   0        0        0        0 2024-05-12 19:05:12.112964 picodi-0.7.0/picodi/py.typed
+-rw-r--r--   0        0        0     2657 2024-05-12 19:05:12.112964 picodi-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0    10896 1970-01-01 00:00:00.000000 picodi-0.7.0/PKG-INFO
```

### Comparing `picodi-0.6.0/LICENSE` & `picodi-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `picodi-0.6.0/README.md` & `picodi-0.7.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,37 @@
 # Picodi - Python DI (Dependency Injection) Library
 
 [![Build Status](https://github.com/yakimka/picodi/actions/workflows/workflow-ci.yml/badge.svg?branch=main&event=push)](https://github.com/yakimka/picodi/actions/workflows/workflow-ci.yml)
 [![Codecov](https://codecov.io/gh/yakimka/picodi/branch/main/graph/badge.svg)](https://codecov.io/gh/yakimka/picodi)
 [![PyPI - Version](https://img.shields.io/pypi/v/picodi.svg)](https://pypi.org/project/picodi/)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/picodi)
 
-Simple Dependency Injection for Python.
-This library supports both synchronous and asynchronous contexts
+Picodi simplifies Dependency Injection (DI) for Python applications.
+DI is a design pattern that allows objects to receive their dependencies from
+an external source rather than creating them internally.
+This library supports both synchronous and asynchronous contexts,
 and offers features like resource lifecycle management.
 
+## Table of Contents
+
+- [Status](#status)
+- [Installation](#installation)
+- [Features](#features)
+- [Basic Usage](#basic-usage)
+  - [Declaring dependencies](#declaring-dependencies)
+  - [Injecting dependencies](#injecting-dependencies)
+  - [Declaring dependencies that acts like a context manager](#declaring-dependencies-that-acts-like-a-context-manager)
+  - [Declaring resource dependencies](#declaring-resource-dependencies)
+  - [Resolving async dependencies in sync functions](#resolving-async-dependencies-in-sync-functions)
+  - [Using picodi with web frameworks](#using-picodi-with-web-frameworks)
+  - [Helper functions](#helper-functions)
+- [API Reference](#api-reference)
+- [License](#license)
+- [Credits](#credits)
+
 ## Status
 
 Picodi is currently in the experimental stage.
 Public APIs may change without notice until the library reaches a 1.x.x version.
 Use it at your own risk.
 
 ## Installation
@@ -28,102 +47,95 @@
 - ⏱️ Supports both sync and async contexts
 - 🔄 Resource lifecycle management
 - 🔍 Type hints support
 - 🐍 Python 3.10+
 
 ## Basic Usage
 
-Picodi uses decorators, functions and generators to provide and inject dependencies:
+Picodi uses decorators, functions and generators to provide and inject dependencies.
 
 ### Declaring dependencies
 
 Dependencies can be simple functions or generators that act as context managers.
 
 ```python
-import asyncio
-import random
-
-
-# this is a simple function that returns a random port number
+# A simple function returning a static number,
 #   and this function can be used as a dependency
-def get_random_db_port() -> int:
-    return random.randint(1024, 49151)
+def get_meaning_of_life():
+    return 42
 
 
-# or async version
-async def get_random_db_port_async() -> int:
-    await asyncio.sleep(1)
-    return random.randint(1024, 49151)
+# A generator to manage database connections, cleaning up after usage
+def get_meaning_of_life():
+    print("setup")
+    yield 42
+    print("teardown")
+
+
+# Or async version
+async def get_meaning_of_life():
+    print("setup")
+    yield 42
+    print("teardown")
 ```
 
 ### Injecting dependencies
 
 Declare dependencies in function arguments using the `Provide` function.
-Use the `inject` decorator if you want to resolve `Provide` dependencies on function call:
+Use the `inject` decorator to automatically inject dependencies into a function.
 
 ```python
-import random
-
 from picodi import inject, Provide
 
 
-def get_random_db_port() -> int:
-    return random.randint(1024, 49151)
+def get_db_port() -> int:
+    return 8000
 
 
 @inject
-def get_connection_settings(port: int = Provide(get_random_db_port)):
+def get_connection_settings(port: int = Provide(get_db_port)):
     return {"port": port}
-
-# get_connection_settings() will return
-# a dictionary with a random port number on every call
 ```
 
 ### Declaring dependencies that acts like a context manager
 
-You can also use a generator to declare dependencies that need to be cleaned up after use:
+You can use a generator to declare dependencies that need to be cleaned up after use.
 
 ```python
-from typing import Generator
-
 from picodi import Provide, inject
 
 
-# also can be async, just use `async def`
-def get_db() -> Generator[str, None, None]:
+def get_db():
     yield "db connection"
     print("closing db connection")
 
 
 @inject
 def process_data(db: str = Provide(get_db)) -> None:
     print("processing data in db:", db)
-
-process_data()
-# -> processing data in db: db connection
-# -> closing db connection
 ```
 
+`get_db` and `process_data` also can be async, just add `async` keyword before `def`.
+
 ### Declaring resource dependencies
 
 Use the `resource` decorator to declare a resource,
 which ensures that the provided function is treated as a singleton
-and that its lifecycle is managed across the application:
+and that its lifecycle is managed across the application.
 
 ```python
 import asyncio
 import random
-from typing import AsyncGenerator
 
 from picodi import Provide, inject, resource, shutdown_resources
 
 
 # useful for managing resources like connections
 @resource
-async def get_db_port() -> AsyncGenerator[int, None]:
+async def get_db_port():
     yield random.randint(1024, 49151)
     print("closing db port")
 
 
 @inject
 async def check_port(port: int = Provide(get_db_port)) -> None:
     print("checking port:", port)
@@ -142,66 +154,52 @@
 # -> checking port: 24090
 # -> shutting down resources
 # -> closing db port
 ```
 
 ### Resolving async dependencies in sync functions
 
-If you try to resolve async dependencies in sync functions, you may get not what you expect.
+Attempting to resolve async dependencies in sync functions may not work as expected,
+resulting in unexpected behaviors like receiving a coroutine object instead of the actual value.
 
 ```python
-import asyncio
-
-from picodi import Provide, inject
-
-
 async def get_db_port() -> int:
     return 8080
 
 
 @inject
 def print_port(port: int = Provide(get_db_port)) -> None:
     print("port is:", port)
-
-
-async def main() -> None:
-    print_port()
-
-
-asyncio.run(main())
-# -> port is: <coroutine object get_db_port at 0x1037741a0>
+    # port is: <coroutine object get_db_port at 0x1037741a0>
 ```
 
 But if your dependency is a resource,
 you can use `init_resources` on startup to resolve dependencies and then use cached values,
-even in sync functions:
+even in sync functions.
+But regular async functions will still need to be used only in async context.
 
 ```python
 import asyncio
-from typing import AsyncGenerator
 
 from picodi import Provide, init_resources, inject, resource
 
 @resource
-async def get_db_port() -> AsyncGenerator[int, None]:
+async def get_db_port():
     yield 8080
 
 
 @inject
 def print_port(port: int = Provide(get_db_port)) -> None:
     print("port is:", port)
+    # -> port is: 8080
 
 
 async def main() -> None:
     await init_resources()
     print_port()
-
-
-asyncio.run(main())
-# -> port is: 8080
 ```
 
 ## Using picodi with web frameworks
 
 Picodi can be used with web frameworks like FastAPI or Django.
 
 ```python
@@ -227,28 +225,64 @@
 async def read_root(redis: str = Depends(Provide(get_redis_connection))):
     return {"redis": redis}
 
 
 # uvicorn fastapi_di:app --reload
 ```
 
+### Helper functions
+
+#### `helpers.get_value`
+
+Function to get a value from a nested dictionary or object.
+Can be useful for getting single value from settings object
+and not be dependent on the type of the object.
+
+```python
+from picodi import inject, Provide
+from picodi.helpers import get_value
+
+def get_settings():
+    return {
+        "db": {
+            "host": "localhost",
+            "port": 8000
+        }
+    }
+
+
+@inject
+def get_setting(path: str, settings: dict = Provide(get_settings)):
+    value = get_value(path, settings)
+    return lambda: value
+
+
+@inject
+def get_connection(
+    host: str = Provide(get_setting(path="db.host")),
+    port: int = Provide(get_setting(path="db.port")),
+):
+    print("connecting to", host, port)
+    # -> connecting to localhost 8000
+```
+
 ## API Reference
 
 ### `Provide(dependency)`
 
 Marks a callable as a provider of a dependency.
-It manages the lifecycle of the dependency,
-including initialization and teardown if the dependency is a generator.
 
 - **Parameters**:
   - `dependency`: A callable that returns the dependency or a generator for context management.
 
 ### `inject(fn)`
 
 Decorator to automatically inject dependencies declared by `Provide` into a function.
+It manages the lifecycle of the dependency,
+including initialization and teardown if the dependency is a generator.
 
 Should be placed first in the decorator chain (on bottom).
 
 - **Parameters**:
   - `fn`: The function into which dependencies will be injected.
 
 ### `resource(fn)`
@@ -271,14 +305,64 @@
 ### `shutdown_resources()`
 
 Cleans up all resources.
 It should be called when the application is shutting down to ensure proper resource cleanup.
 
 Can be called as `shutdown_resources()` in sync context and `await shutdown_resources()` in async context.
 
+### `registry` object
+
+Registry object to manage dependencies and resources.
+
+#### `registry.override(dependency, new_dependency)`
+
+Overrides a dependency with a new one. It can be used as a decorator, context manager
+or a regular method call. The new dependency will be used instead of the old one.
+Useful for testing or changing dependencies at runtime.
+
+- **Parameters**:
+  - `dependency`: The dependency to override.
+  - `new_dependency`: The new dependency to use instead of the old one. Don't specify
+  this parameter when using as a decorator. When passing `None`, the original dependency
+  will be restored.
+
+```python
+from picodi import registry
+
+def get_settings():
+    raise NotImplementedError
+
+
+# as a decorator
+@registry.override(get_settings)
+def real_settings():
+    return {"real": "settings"}
+
+
+# as a context manager
+with registry.override(get_settings, real_settings):
+    ...
+
+# as a regular method call
+registry.override(get_settings, real_settings)
+registry.override(get_settings, None)  # clear override
+```
+
+#### `registry.clear_overrides()`
+
+Clears all overrides set by `registry.override()`.
+
+#### `registry.clear()`
+
+Clears all dependencies and resources. This method will not close any resources.
+So you need to manually call `shutdown_resources` before this method.
+
+Don't use this method in production code (only if you know what you are doing),
+it's mostly for testing purposes.
+
 ### `helpers` module
 
 Module with helper functions for working with dependencies.
 
 #### `helpers.get_value(path, obj, default)`
 
 Function to get a value from a nested dictionary or object.
```

### Comparing `picodi-0.6.0/picodi/_internal.py` & `picodi-0.7.0/picodi/_internal.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,28 +17,22 @@
 
 
 class ExitStack:
     def __init__(self) -> None:
         self._sync_stack = SyncExitStack()
         self._async_stack = AsyncExitStack()
 
-    def __enter__(self) -> ExitStack:
-        return self
-
     def __exit__(
         self,
         exc_type: type[BaseException] | None,
         exc: BaseException | None,
         traceback: TracebackType | None,
     ) -> bool | None:
         return self._sync_stack.__exit__(exc_type, exc, traceback)
 
-    async def __aenter__(self) -> ExitStack:
-        return self
-
     async def __aexit__(
         self,
         exc_type: type[BaseException] | None,
         exc: BaseException | None,
         traceback: TracebackType | None,
     ) -> bool | None:
         res_sync = self._sync_stack.__exit__(exc_type, exc, traceback)
@@ -47,15 +41,15 @@
 
     def enter_context(self, cm: AsyncContextManager | ContextManager) -> Any:
         if isinstance(cm, ContextManager):
             return self._sync_stack.enter_context(cm)
         elif isinstance(cm, AsyncContextManager):
             return self._async_stack.enter_async_context(cm)
 
-        raise TypeError(f"Unsupported context manager: {cm}")
+        raise TypeError(f"Unsupported context manager: {cm}")  # pragma: no cover
 
     def close(self) -> Awaitable:
         self.__exit__(None, None, None)
         if is_async_environment():
             return self.__aexit__(None, None, None)
         return DummyAwaitable()
```

### Comparing `picodi-0.6.0/picodi/_picodi.py` & `picodi-0.7.0/picodi/_picodi.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,46 +1,172 @@
 from __future__ import annotations
 
 import asyncio
 import functools
 import inspect
 import threading
-from collections.abc import Awaitable, Callable
+from collections.abc import Awaitable, Callable, Generator, Iterable, Iterator
 from contextlib import asynccontextmanager, contextmanager
-from dataclasses import asdict, dataclass, field
-from functools import wraps
-from typing import (
-    TYPE_CHECKING,
-    Any,
-    AsyncContextManager,
-    ContextManager,
-    ParamSpec,
-    TypeVar,
-    cast,
-)
+from dataclasses import asdict, dataclass
+from typing import TYPE_CHECKING, Any, NamedTuple, ParamSpec, TypeVar, cast
 
 from picodi._internal import DummyAwaitable
 from picodi._scopes import GlobalScope, NullScope, Scope, SingletonScope
 
 if TYPE_CHECKING:
     from inspect import BoundArguments, Signature
 
 DependencyCallable = Callable[..., Any]
 T = TypeVar("T")
 P = ParamSpec("P")
 TC = TypeVar("TC", bound=Callable)
 
+unset = object()
 
-_unset = object()
-_lock = threading.RLock()
-_registry: dict[DependencyCallable, Provider] = {}
+
+class RegistryStorage:
+    def __init__(self) -> None:
+        self.deps: dict[DependencyCallable, Provider] = {}
+        self.overrides: dict[DependencyCallable, DependencyCallable] = {}
+        self.lock = threading.RLock()
+
+    def __iter__(self) -> Iterator[Provider]:
+        return iter(self.deps.values())
+
+
+class InternalRegistry:
+    def __init__(self, storage: RegistryStorage) -> None:
+        self._storage = storage
+
+    def add(
+        self,
+        dependency: DependencyCallable,
+        scope_class: type[Scope] = NullScope,
+        in_use: bool = True,
+        override_scope: bool = False,
+    ) -> None:
+        """
+        Add a dependency to the registry. If the dependency is already in the registry,
+        it `in_use` flag can be updated, but the scope class cannot be changed.
+        If the dependency is not in the registry, it will be added with the provided
+        scope class and `in_use` flag.
+        """
+        with self._storage.lock:
+            if dependency in self._storage.deps:
+                provider = self._storage.deps[dependency]
+                to_replace = provider.replace(
+                    scope_class=(scope_class if override_scope else None),
+                    # If the provider is already in use, keep it in use
+                    # otherwise, use the new value. For example, if a provider
+                    # is already in use and we want to replace it with a resource,
+                    # we should keep it in use. If it's already a resource and we
+                    # want to replace it with a regular dependency, we should set
+                    # is_use to True.
+                    in_use=(provider.in_use or in_use),
+                )
+                if to_replace != provider:
+                    self._storage.deps[dependency] = to_replace
+            else:
+                self._storage.deps[dependency] = Provider.from_dependency(
+                    dependency=dependency,
+                    scope_class=scope_class,
+                    in_use=in_use,
+                )
+
+    def get(self, dependency: DependencyCallable) -> Provider:
+        with self._storage.lock:
+            if self._storage.overrides.get(dependency):
+                dependency = self._storage.overrides[dependency]
+            return self._storage.deps[dependency]
+
+    def filter(self, predicate: Callable[[Provider], bool]) -> Iterable[Provider]:
+        return filter(predicate, self._storage)
+
+
+class Registry:
+    def __init__(
+        self, storage: RegistryStorage, internal_registry: InternalRegistry
+    ) -> None:
+        self._storage = storage
+        self._internal_registry = internal_registry
+
+    def override(
+        self,
+        dependency: DependencyCallable,
+        new_dependency: DependencyCallable | None | object = unset,
+    ) -> Callable[[DependencyCallable], DependencyCallable]:
+        """
+        Override a dependency with a new one. It can be used as a decorator,
+        as a context manager or as a regular method call. New dependency will be
+        added to the registry.
+        Examples:
+        ```
+        @registry.override(get_settings)
+        def real_settings():
+            return {"real": "settings"}
+
+        with registry.override(get_settings, real_settings):
+            ...
+
+        registry.override(get_settings, real_settings)
+        registry.override(get_settings, None)  # clear override
+        """
+
+        def decorator(override_to: DependencyCallable) -> DependencyCallable:
+            self._internal_registry.add(override_to, in_use=True)
+            if dependency is override_to:
+                raise ValueError("Cannot override a dependency with itself")
+            self._storage.overrides[dependency] = override_to
+            return override_to
+
+        if new_dependency is unset:
+            return decorator
+
+        with self._storage.lock:
+            original_dependency = self._storage.overrides.get(dependency)
+            if callable(new_dependency):
+                decorator(new_dependency)
+            else:
+                self._storage.overrides.pop(dependency, None)
+
+        @contextmanager
+        def manage_context() -> Generator[None, None, None]:
+            try:
+                yield
+            finally:
+                self.override(dependency, original_dependency)
+
+        return manage_context()
+
+    def clear(self) -> None:
+        """
+        Clear the registry. It will remove all dependencies and overrides.
+        This method will not close any resources. So you need to manually call
+        `shutdown_resources` before this method.
+        """
+        with self._storage.lock:
+            self._storage.deps.clear()
+            self._storage.overrides.clear()
+
+    def clear_overrides(self) -> None:
+        """
+        Clear all overrides. It will remove all overrides, but keep the dependencies.
+        """
+        with self._storage.lock:
+            self._storage.overrides.clear()
+
+
+_registry_storage = RegistryStorage()
+_internal_registry = InternalRegistry(_registry_storage)
+registry = Registry(_registry_storage, _internal_registry)
 _scopes: dict[type[Scope], Scope] = {
     NullScope: NullScope(),
     SingletonScope: SingletonScope(),
 }
+_lock = threading.RLock()
 
 
 def Provide(dependency: DependencyCallable, /) -> Any:  # noqa: N802
     """
     Declare a provider.
     It takes a single "dependency" callable (like a function).
     Don't call it directly, picodi will call it for you.
@@ -58,20 +184,15 @@
         print("closing db connection")
 
     @inject
     def my_service(db: str = Provide(get_db)):
         assert db == "db connection"
     ```
     """
-    with _lock:
-        if dependency not in _registry:
-            _registry[dependency] = Provider.from_dependency(dependency, in_use=True)
-        elif not _registry[dependency].in_use:
-            _registry[dependency] = _registry[dependency].replace(in_use=True)
-
+    _internal_registry.add(dependency)
     return Dependency(dependency)
 
 
 def inject(fn: Callable[P, T]) -> Callable[P, T]:
     """
     Decorator to inject dependencies into a function.
     Use it in combination with `Provide` to declare dependencies.
@@ -120,50 +241,49 @@
                 bound.arguments[name] = get_value()
 
             result = fn(*bound.args, **bound.kwargs)
             for scope in _scopes.values():
                 scope.close_local()
             return result
 
-    wrapper._picodi_inject_ = True  # type: ignore[attr-defined] # noqa: SF01
     return wrapper  # type: ignore[return-value]
 
 
 def resource(fn: TC) -> TC:
     """
     Decorator to declare a resource. Resource is a dependency that should be
     called only once, cached and shared across the application.
     On shutdown, all resources will be closed
     (you need to call `shutdown_resources` manually).
     Use it with a dependency generator function to declare a resource.
     Should be placed last in the decorator chain (on top).
     """
-    with _lock:
-        if fn in _registry:
-            provider = _registry[fn].replace(scope_class=SingletonScope)
-        else:
-            provider = Provider.from_dependency(
-                fn, scope_class=SingletonScope, in_use=False
-            )
-        _registry[fn] = provider
+    _internal_registry.add(
+        fn,
+        scope_class=SingletonScope,
+        in_use=False,
+        override_scope=True,
+    )
     return fn
 
 
 def init_resources() -> Awaitable:
     """
     Call this function to close all resources. Usually, it should be called
     when your application is shutting down.
     """
     async_resources = []
-    for provider in _registry.values():
-        if provider.in_use and issubclass(provider.scope_class, GlobalScope):
-            if provider.is_async:
-                async_resources.append(_resolve_value_async(provider))
-            else:
-                _resolve_value(provider)
+    global_providers = _internal_registry.filter(
+        lambda p: p.in_use and issubclass(p.scope_class, GlobalScope)
+    )
+    for provider in global_providers:
+        if provider.is_async:
+            async_resources.append(_resolve_value_async(provider))
+        else:
+            _resolve_value(provider)
 
     if async_resources:
         return asyncio.gather(*async_resources)
     return DummyAwaitable()
 
 
 def shutdown_resources() -> Awaitable:
@@ -175,58 +295,37 @@
     for scope in _scopes.values():
         coro = scope.close_global()
         if coro is not None:
             tasks.append(coro)
     return asyncio.gather(*tasks)
 
 
-def make_dependency(fn: Callable[P, T], *args: Any, **kwargs: Any) -> Callable[..., T]:
-    signature = inspect.signature(fn)
-    bound = signature.bind(*args, **kwargs)
-    bound.apply_defaults()
-
-    if not getattr(fn, "_picodi_inject_", None):
-        fn = inject(fn)
-
-    @wraps(fn)
-    def wrapper(*args_in: P.args, **kwargs_in: P.kwargs) -> T:
-        bound_inner = signature.bind_partial(*args_in, **kwargs_in)
-        bound.arguments.update(bound_inner.arguments)
-        return fn(*bound.args, **bound.kwargs)
-
-    return wrapper
-
-
-CallableManager = Callable[..., AsyncContextManager | ContextManager]
-
-
-@dataclass(frozen=True)
-class Dependency:
+class Dependency(NamedTuple):
     original: DependencyCallable
 
     def __call__(self) -> Dependency:
         return self
 
     def get_provider(self) -> Provider:
-        return _registry[self.original]
+        return _internal_registry.get(self.original)
 
 
 @dataclass(frozen=True)
 class Provider:
     dependency: DependencyCallable
-    is_async: bool = field(compare=False)
-    scope_class: type[Scope] = field(compare=False)
-    in_use: bool = field(compare=False)
+    is_async: bool
+    scope_class: type[Scope]
+    in_use: bool
 
     @classmethod
     def from_dependency(
         cls,
         dependency: DependencyCallable,
-        scope_class: type[Scope] = NullScope,
-        in_use: bool = False,
+        scope_class: type[Scope],
+        in_use: bool,
     ) -> Provider:
         is_async = inspect.iscoroutinefunction(
             dependency
         ) or inspect.isasyncgenfunction(dependency)
         return cls(
             dependency=dependency,
             is_async=is_async,
```

### Comparing `picodi-0.6.0/picodi/_scopes.py` & `picodi-0.7.0/picodi/_scopes.py`

 * *Files identical despite different names*

### Comparing `picodi-0.6.0/picodi/helpers.py` & `picodi-0.7.0/picodi/helpers.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,18 +14,18 @@
     """
     Get attribute from nested objects.
     If the attribute is not found, raise an AttributeError if default is not provided.
     If default is provided, return it.
 
     Example:
     ```
-    obj = SimpleNamespace(foo=SimpleNamespace(bar=SimpleNamespace(baz=42)))
-    get_attribute("foo.bar.baz", obj)  # 42
-    get_attribute("foo.bar.baz2", obj)  # AttributeError
-    get_attribute("foo.bar.baz2", obj, default=12)  # 12
+    obj = SimpleNamespace(foo=SimpleNamespace(bar={"baz": 42}))
+    get_value("foo.bar.baz", obj)  # 42
+    get_value("foo.bar.baz2", obj)  # AttributeError
+    get_value("foo.bar.baz2", obj, default=12)  # 12
     ```
     """
     if not path:
         raise ValueError("Empty path")
     if not isinstance(path, str):
         raise TypeError("Path must be a string")
```

### Comparing `picodi-0.6.0/pyproject.toml` & `picodi-0.7.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "picodi"
 description = "Simple Dependency Injection for Python"
-version = "0.6.0"
+version = "0.7.0"
 license = "MIT"
 authors = [
   "yakimka"
 ]
 
 readme = "README.md"
 
@@ -89,15 +89,17 @@
 
 [tool.coverage.run]
 branch = true
 
 [tool.coverage.report]
 precision = 2
 exclude_lines = [
+  "pragma: no cover",
   "if TYPE_CHECKING:",
+  "raise NotImplementedError",
 ]
 
 [tool.mypy]
 files = ["."]
 exclude = ["tests/"]
 ##
 # mypy configurations: https://mypy.readthedocs.io/en/latest/config_file.html
```

### Comparing `picodi-0.6.0/PKG-INFO` & `picodi-0.7.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: picodi
-Version: 0.6.0
+Version: 0.7.0
 Summary: Simple Dependency Injection for Python
 Home-page: https://github.com/yakimka/picodi
 License: MIT
 Author: yakimka
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -21,18 +21,37 @@
 # Picodi - Python DI (Dependency Injection) Library
 
 [![Build Status](https://github.com/yakimka/picodi/actions/workflows/workflow-ci.yml/badge.svg?branch=main&event=push)](https://github.com/yakimka/picodi/actions/workflows/workflow-ci.yml)
 [![Codecov](https://codecov.io/gh/yakimka/picodi/branch/main/graph/badge.svg)](https://codecov.io/gh/yakimka/picodi)
 [![PyPI - Version](https://img.shields.io/pypi/v/picodi.svg)](https://pypi.org/project/picodi/)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/picodi)
 
-Simple Dependency Injection for Python.
-This library supports both synchronous and asynchronous contexts
+Picodi simplifies Dependency Injection (DI) for Python applications.
+DI is a design pattern that allows objects to receive their dependencies from
+an external source rather than creating them internally.
+This library supports both synchronous and asynchronous contexts,
 and offers features like resource lifecycle management.
 
+## Table of Contents
+
+- [Status](#status)
+- [Installation](#installation)
+- [Features](#features)
+- [Basic Usage](#basic-usage)
+  - [Declaring dependencies](#declaring-dependencies)
+  - [Injecting dependencies](#injecting-dependencies)
+  - [Declaring dependencies that acts like a context manager](#declaring-dependencies-that-acts-like-a-context-manager)
+  - [Declaring resource dependencies](#declaring-resource-dependencies)
+  - [Resolving async dependencies in sync functions](#resolving-async-dependencies-in-sync-functions)
+  - [Using picodi with web frameworks](#using-picodi-with-web-frameworks)
+  - [Helper functions](#helper-functions)
+- [API Reference](#api-reference)
+- [License](#license)
+- [Credits](#credits)
+
 ## Status
 
 Picodi is currently in the experimental stage.
 Public APIs may change without notice until the library reaches a 1.x.x version.
 Use it at your own risk.
 
 ## Installation
@@ -48,102 +67,95 @@
 - ⏱️ Supports both sync and async contexts
 - 🔄 Resource lifecycle management
 - 🔍 Type hints support
 - 🐍 Python 3.10+
 
 ## Basic Usage
 
-Picodi uses decorators, functions and generators to provide and inject dependencies:
+Picodi uses decorators, functions and generators to provide and inject dependencies.
 
 ### Declaring dependencies
 
 Dependencies can be simple functions or generators that act as context managers.
 
 ```python
-import asyncio
-import random
-
-
-# this is a simple function that returns a random port number
+# A simple function returning a static number,
 #   and this function can be used as a dependency
-def get_random_db_port() -> int:
-    return random.randint(1024, 49151)
+def get_meaning_of_life():
+    return 42
 
 
-# or async version
-async def get_random_db_port_async() -> int:
-    await asyncio.sleep(1)
-    return random.randint(1024, 49151)
+# A generator to manage database connections, cleaning up after usage
+def get_meaning_of_life():
+    print("setup")
+    yield 42
+    print("teardown")
+
+
+# Or async version
+async def get_meaning_of_life():
+    print("setup")
+    yield 42
+    print("teardown")
 ```
 
 ### Injecting dependencies
 
 Declare dependencies in function arguments using the `Provide` function.
-Use the `inject` decorator if you want to resolve `Provide` dependencies on function call:
+Use the `inject` decorator to automatically inject dependencies into a function.
 
 ```python
-import random
-
 from picodi import inject, Provide
 
 
-def get_random_db_port() -> int:
-    return random.randint(1024, 49151)
+def get_db_port() -> int:
+    return 8000
 
 
 @inject
-def get_connection_settings(port: int = Provide(get_random_db_port)):
+def get_connection_settings(port: int = Provide(get_db_port)):
     return {"port": port}
-
-# get_connection_settings() will return
-# a dictionary with a random port number on every call
 ```
 
 ### Declaring dependencies that acts like a context manager
 
-You can also use a generator to declare dependencies that need to be cleaned up after use:
+You can use a generator to declare dependencies that need to be cleaned up after use.
 
 ```python
-from typing import Generator
-
 from picodi import Provide, inject
 
 
-# also can be async, just use `async def`
-def get_db() -> Generator[str, None, None]:
+def get_db():
     yield "db connection"
     print("closing db connection")
 
 
 @inject
 def process_data(db: str = Provide(get_db)) -> None:
     print("processing data in db:", db)
-
-process_data()
-# -> processing data in db: db connection
-# -> closing db connection
 ```
 
+`get_db` and `process_data` also can be async, just add `async` keyword before `def`.
+
 ### Declaring resource dependencies
 
 Use the `resource` decorator to declare a resource,
 which ensures that the provided function is treated as a singleton
-and that its lifecycle is managed across the application:
+and that its lifecycle is managed across the application.
 
 ```python
 import asyncio
 import random
-from typing import AsyncGenerator
 
 from picodi import Provide, inject, resource, shutdown_resources
 
 
 # useful for managing resources like connections
 @resource
-async def get_db_port() -> AsyncGenerator[int, None]:
+async def get_db_port():
     yield random.randint(1024, 49151)
     print("closing db port")
 
 
 @inject
 async def check_port(port: int = Provide(get_db_port)) -> None:
     print("checking port:", port)
@@ -162,66 +174,52 @@
 # -> checking port: 24090
 # -> shutting down resources
 # -> closing db port
 ```
 
 ### Resolving async dependencies in sync functions
 
-If you try to resolve async dependencies in sync functions, you may get not what you expect.
+Attempting to resolve async dependencies in sync functions may not work as expected,
+resulting in unexpected behaviors like receiving a coroutine object instead of the actual value.
 
 ```python
-import asyncio
-
-from picodi import Provide, inject
-
-
 async def get_db_port() -> int:
     return 8080
 
 
 @inject
 def print_port(port: int = Provide(get_db_port)) -> None:
     print("port is:", port)
-
-
-async def main() -> None:
-    print_port()
-
-
-asyncio.run(main())
-# -> port is: <coroutine object get_db_port at 0x1037741a0>
+    # port is: <coroutine object get_db_port at 0x1037741a0>
 ```
 
 But if your dependency is a resource,
 you can use `init_resources` on startup to resolve dependencies and then use cached values,
-even in sync functions:
+even in sync functions.
+But regular async functions will still need to be used only in async context.
 
 ```python
 import asyncio
-from typing import AsyncGenerator
 
 from picodi import Provide, init_resources, inject, resource
 
 @resource
-async def get_db_port() -> AsyncGenerator[int, None]:
+async def get_db_port():
     yield 8080
 
 
 @inject
 def print_port(port: int = Provide(get_db_port)) -> None:
     print("port is:", port)
+    # -> port is: 8080
 
 
 async def main() -> None:
     await init_resources()
     print_port()
-
-
-asyncio.run(main())
-# -> port is: 8080
 ```
 
 ## Using picodi with web frameworks
 
 Picodi can be used with web frameworks like FastAPI or Django.
 
 ```python
@@ -247,28 +245,64 @@
 async def read_root(redis: str = Depends(Provide(get_redis_connection))):
     return {"redis": redis}
 
 
 # uvicorn fastapi_di:app --reload
 ```
 
+### Helper functions
+
+#### `helpers.get_value`
+
+Function to get a value from a nested dictionary or object.
+Can be useful for getting single value from settings object
+and not be dependent on the type of the object.
+
+```python
+from picodi import inject, Provide
+from picodi.helpers import get_value
+
+def get_settings():
+    return {
+        "db": {
+            "host": "localhost",
+            "port": 8000
+        }
+    }
+
+
+@inject
+def get_setting(path: str, settings: dict = Provide(get_settings)):
+    value = get_value(path, settings)
+    return lambda: value
+
+
+@inject
+def get_connection(
+    host: str = Provide(get_setting(path="db.host")),
+    port: int = Provide(get_setting(path="db.port")),
+):
+    print("connecting to", host, port)
+    # -> connecting to localhost 8000
+```
+
 ## API Reference
 
 ### `Provide(dependency)`
 
 Marks a callable as a provider of a dependency.
-It manages the lifecycle of the dependency,
-including initialization and teardown if the dependency is a generator.
 
 - **Parameters**:
   - `dependency`: A callable that returns the dependency or a generator for context management.
 
 ### `inject(fn)`
 
 Decorator to automatically inject dependencies declared by `Provide` into a function.
+It manages the lifecycle of the dependency,
+including initialization and teardown if the dependency is a generator.
 
 Should be placed first in the decorator chain (on bottom).
 
 - **Parameters**:
   - `fn`: The function into which dependencies will be injected.
 
 ### `resource(fn)`
@@ -291,14 +325,64 @@
 ### `shutdown_resources()`
 
 Cleans up all resources.
 It should be called when the application is shutting down to ensure proper resource cleanup.
 
 Can be called as `shutdown_resources()` in sync context and `await shutdown_resources()` in async context.
 
+### `registry` object
+
+Registry object to manage dependencies and resources.
+
+#### `registry.override(dependency, new_dependency)`
+
+Overrides a dependency with a new one. It can be used as a decorator, context manager
+or a regular method call. The new dependency will be used instead of the old one.
+Useful for testing or changing dependencies at runtime.
+
+- **Parameters**:
+  - `dependency`: The dependency to override.
+  - `new_dependency`: The new dependency to use instead of the old one. Don't specify
+  this parameter when using as a decorator. When passing `None`, the original dependency
+  will be restored.
+
+```python
+from picodi import registry
+
+def get_settings():
+    raise NotImplementedError
+
+
+# as a decorator
+@registry.override(get_settings)
+def real_settings():
+    return {"real": "settings"}
+
+
+# as a context manager
+with registry.override(get_settings, real_settings):
+    ...
+
+# as a regular method call
+registry.override(get_settings, real_settings)
+registry.override(get_settings, None)  # clear override
+```
+
+#### `registry.clear_overrides()`
+
+Clears all overrides set by `registry.override()`.
+
+#### `registry.clear()`
+
+Clears all dependencies and resources. This method will not close any resources.
+So you need to manually call `shutdown_resources` before this method.
+
+Don't use this method in production code (only if you know what you are doing),
+it's mostly for testing purposes.
+
 ### `helpers` module
 
 Module with helper functions for working with dependencies.
 
 #### `helpers.get_value(path, obj, default)`
 
 Function to get a value from a nested dictionary or object.
```

