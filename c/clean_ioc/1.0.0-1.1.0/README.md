# Comparing `tmp/clean_ioc-1.0.0.tar.gz` & `tmp/clean_ioc-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clean_ioc-1.0.0.tar", max compression
+gzip compressed data, was "clean_ioc-1.1.0.tar", max compression
```

## Comparing `clean_ioc-1.0.0.tar` & `clean_ioc-1.1.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     3641 2024-05-09 22:47:16.993779 clean_ioc-1.0.0/CHANGES.rst
--rw-r--r--   0        0        0     1067 2024-05-09 22:47:16.993779 clean_ioc-1.0.0/LICENSE
--rw-r--r--   0        0        0    20278 2024-05-09 22:47:16.993779 clean_ioc-1.0.0/README.md
--rw-r--r--   0        0        0       20 2024-05-09 22:47:16.993779 clean_ioc-1.0.0/clean_ioc/__init__.py
--rw-r--r--   0        0        0     2118 2024-05-09 22:47:16.993779 clean_ioc-1.0.0/clean_ioc/bundles.py
--rw-r--r--   0        0        0    62149 2024-05-09 22:47:16.993779 clean_ioc-1.0.0/clean_ioc/core.py
--rw-r--r--   0        0        0       20 2024-05-09 22:47:16.993779 clean_ioc-1.0.0/clean_ioc/ext/fastapi/__init__.py
--rw-r--r--   0        0        0     1909 2024-05-09 22:47:16.993779 clean_ioc-1.0.0/clean_ioc/ext/fastapi/core.py
--rw-r--r--   0        0        0     1255 2024-05-09 22:47:16.993779 clean_ioc-1.0.0/clean_ioc/ext/fastapi/dependencies.py
--rw-r--r--   0        0        0        0 2024-05-09 22:47:16.993779 clean_ioc-1.0.0/clean_ioc/ext/fastapi/py.typed
--rw-r--r--   0        0        0     1262 2024-05-09 22:47:16.997779 clean_ioc-1.0.0/clean_ioc/factories.py
--rw-r--r--   0        0        0     2662 2024-05-09 22:47:16.997779 clean_ioc-1.0.0/clean_ioc/functional_utils.py
--rw-r--r--   0        0        0      563 2024-05-09 22:47:16.997779 clean_ioc-1.0.0/clean_ioc/list_reduction_filters.py
--rw-r--r--   0        0        0     1779 2024-05-09 22:47:16.997779 clean_ioc-1.0.0/clean_ioc/node_filters.py
--rw-r--r--   0        0        0        0 2024-05-09 22:47:16.997779 clean_ioc-1.0.0/clean_ioc/py.typed
--rw-r--r--   0        0        0     4807 2024-05-09 22:47:16.997779 clean_ioc-1.0.0/clean_ioc/registration_filters.py
--rw-r--r--   0        0        0      962 2024-05-09 22:47:16.997779 clean_ioc-1.0.0/clean_ioc/type_filters.py
--rw-r--r--   0        0        0     6920 2024-05-09 22:47:16.997779 clean_ioc-1.0.0/clean_ioc/typing_utils.py
--rw-r--r--   0        0        0     1828 2024-05-09 22:47:16.997779 clean_ioc-1.0.0/clean_ioc/utils.py
--rw-r--r--   0        0        0      564 2024-05-09 22:47:16.997779 clean_ioc-1.0.0/clean_ioc/value_factories.py
--rw-r--r--   0        0        0     2146 2024-05-09 22:47:16.997779 clean_ioc-1.0.0/pyproject.toml
--rw-r--r--   0        0        0    21058 1970-01-01 00:00:00.000000 clean_ioc-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     4195 2024-05-12 00:53:43.029482 clean_ioc-1.1.0/CHANGES.rst
+-rw-r--r--   0        0        0     1067 2024-05-12 00:53:43.029482 clean_ioc-1.1.0/LICENSE
+-rw-r--r--   0        0        0    20278 2024-05-12 00:53:43.029482 clean_ioc-1.1.0/README.md
+-rw-r--r--   0        0        0       20 2024-05-12 00:53:43.029482 clean_ioc-1.1.0/clean_ioc/__init__.py
+-rw-r--r--   0        0        0     2118 2024-05-12 00:53:43.029482 clean_ioc-1.1.0/clean_ioc/bundles.py
+-rw-r--r--   0        0        0    62448 2024-05-12 00:53:43.033482 clean_ioc-1.1.0/clean_ioc/core.py
+-rw-r--r--   0        0        0       20 2024-05-12 00:53:43.033482 clean_ioc-1.1.0/clean_ioc/ext/fastapi/__init__.py
+-rw-r--r--   0        0        0     1909 2024-05-12 00:53:43.033482 clean_ioc-1.1.0/clean_ioc/ext/fastapi/core.py
+-rw-r--r--   0        0        0     1255 2024-05-12 00:53:43.033482 clean_ioc-1.1.0/clean_ioc/ext/fastapi/dependencies.py
+-rw-r--r--   0        0        0        0 2024-05-12 00:53:43.033482 clean_ioc-1.1.0/clean_ioc/ext/fastapi/py.typed
+-rw-r--r--   0        0        0     1262 2024-05-12 00:53:43.033482 clean_ioc-1.1.0/clean_ioc/factories.py
+-rw-r--r--   0        0        0     2662 2024-05-12 00:53:43.033482 clean_ioc-1.1.0/clean_ioc/functional_utils.py
+-rw-r--r--   0        0        0      563 2024-05-12 00:53:43.033482 clean_ioc-1.1.0/clean_ioc/list_reduction_filters.py
+-rw-r--r--   0        0        0     1779 2024-05-12 00:53:43.033482 clean_ioc-1.1.0/clean_ioc/node_filters.py
+-rw-r--r--   0        0        0        0 2024-05-12 00:53:43.033482 clean_ioc-1.1.0/clean_ioc/py.typed
+-rw-r--r--   0        0        0     4807 2024-05-12 00:53:43.033482 clean_ioc-1.1.0/clean_ioc/registration_filters.py
+-rw-r--r--   0        0        0      962 2024-05-12 00:53:43.033482 clean_ioc-1.1.0/clean_ioc/type_filters.py
+-rw-r--r--   0        0        0     6920 2024-05-12 00:53:43.033482 clean_ioc-1.1.0/clean_ioc/typing_utils.py
+-rw-r--r--   0        0        0     1828 2024-05-12 00:53:43.033482 clean_ioc-1.1.0/clean_ioc/utils.py
+-rw-r--r--   0        0        0      564 2024-05-12 00:53:43.033482 clean_ioc-1.1.0/clean_ioc/value_factories.py
+-rw-r--r--   0        0        0     2146 2024-05-12 00:53:43.033482 clean_ioc-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0    21058 1970-01-01 00:00:00.000000 clean_ioc-1.1.0/PKG-INFO
```

### Comparing `clean_ioc-1.0.0/CHANGES.rst` & `clean_ioc-1.1.0/CHANGES.rst`

 * *Files 5% similar despite different names*

```diff
@@ -138,8 +138,26 @@
     more registration filters
     improve typing for nodes
 
 
 0.18.0
 -----
     container.register(ServiceType, ImplementationType) now allows resolving from implementation types
-        container.resolve(ServiceType) and container.resolve(ImplementationType) both work for resolving.
+        container.resolve(ServiceType) and container.resolve(ImplementationType) both work for resolving.
+
+0.18.1
+-----
+    FIX: pre_configurations failed wehen run in async mode.
+
+1.0.0
+-----
+    First proper release
+    Scopes can now spawn new scopes.
+    Pre configrations api has been improved
+    Scoped lifespan now acts as a singleton in a container
+    Container can now be used as a context manager the same way scopes can.
+    Container can now how scoped teardowns and generator factories on sigletons the same way scopes can.
+
+1.1.0
+-----
+    Decorators can now be functions or generators
+    Pre-configurations can now be functions or generators
```

### Comparing `clean_ioc-1.0.0/LICENSE` & `clean_ioc-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `clean_ioc-1.0.0/README.md` & `clean_ioc-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `clean_ioc-1.0.0/clean_ioc/bundles.py` & `clean_ioc-1.1.0/clean_ioc/bundles.py`

 * *Files identical despite different names*

### Comparing `clean_ioc-1.0.0/clean_ioc/core.py` & `clean_ioc-1.1.0/clean_ioc/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -178,25 +178,25 @@
     pre_configures: Node
     registration_name: str | None
     registration_tags: Iterable[Tag]
     instance: Any = UNKNOWN
     lifespan: Lifespan
     generic_mapping: GenericTypeMap
 
-    def has_registration_tag(self, name: str, value: str | None): ...
+    def has_registration_tag(self, name: str, value: str | None) -> bool: ...
     def unparent(self): ...
     @property
-    def implementation_type(self): ...
+    def implementation_type(self) -> type: ...
     @property
-    def instance_type(self): ...
+    def instance_type(self) -> type: ...
 
     @property
-    def bottom_decorated_node(self): ...
+    def bottom_decorated_node(self) -> Node: ...
     @property
-    def top_decorated_node(self): ...
+    def top_decorated_node(self) -> Node: ...
     def has_dependant_service_type(self, service_type: type) -> bool: ...
 
     def has_dependant_implementation_type(self, implementation_type: type) -> bool: ...
 
     def has_dependant_instance_type(self, instance_type: type) -> bool: ...
 
 
@@ -729,39 +729,42 @@
             logger.exception(f"Failed to run pre-configuration {self.configuration_fn}")
             if not self.continue_on_failure:
                 raise ex
 
     def run(self, context: _ResolvingContext, dependency_node: DependencyNode):
         resolved_dependencies = _resolve_dependencies(self.dependencies, context, dependency_node)
         with self._run_safely():
-            self.activator_class.activate(self.configuration_fn, resolved_dependencies, context, Lifespan.transient)
+            self.activator_class.activate(self.configuration_fn, resolved_dependencies, context, Lifespan.scoped)
 
     async def run_async(self, context: _ResolvingContext, dependency_node: DependencyNode):
         resolved_dependencies = await _resolve_dependencies_async(self.dependencies, context, dependency_node)
         with self._run_safely():
             await self.activator_class.activate_async(
-                self.configuration_fn, resolved_dependencies, context, Lifespan.transient
+                self.configuration_fn, resolved_dependencies, context, Lifespan.scoped
             )
 
 
 class Decorator:
     __slots__ = (
         "service_type",
         "decorated_node_filter",
         "parent_node_filter",
         "decorator_type",
         "decorated_arg",
         "registration_filter",
         "dependencies",
+        "activator_class",
     )
 
     def __init__(
         self,
         service_type: type,
-        decorator_type: type,
+        decorator_type: type | Callable,
+        *,
+        activator_class: type[Activator],
         registration_filter: RegistrationFilter,
         decorator_node_filter: NodeFilter,
         decorated_arg: str | None,
         dependency_config: DependencyConfig = {},
     ):
         self.service_type = service_type
         self.decorator_type = decorator_type
@@ -769,43 +772,38 @@
         dependencies = _set_up_dependencies(decorator_type, dependency_config)
 
         self.decorated_arg = decorated_arg or next(
             name for name, dep in dependencies.items() if dep.service_type == service_type
         )
         self.registration_filter = registration_filter
         self.decorated_node_filter = decorator_node_filter
+        self.activator_class = activator_class
 
         del dependencies[self.decorated_arg]
 
         self.dependencies: dict[str, Dependency] = dependencies
 
     def decorate(
-        self,
-        instance: Any,
-        context: _ResolvingContext,
-        dependency_node: DependencyNode,
+        self, instance: Any, context: _ResolvingContext, dependency_node: DependencyNode, registration: Registration
     ):
         resolved_dependencies = _resolve_dependencies(self.dependencies, context, dependency_node)
         resolved_dependencies[self.decorated_arg] = instance
 
-        return FactoryActivator.activate(
-            self.decorator_type, resolved_dependencies, context, lifespan=Lifespan.transient
+        return self.activator_class.activate(
+            self.decorator_type, resolved_dependencies, context, lifespan=registration.lifespan
         )
 
     async def decorate_async(
-        self,
-        instance: Any,
-        context: _ResolvingContext,
-        dependency_node: DependencyNode,
+        self, instance: Any, context: _ResolvingContext, dependency_node: DependencyNode, registration: Registration
     ):
         resolved_dependencies = await _resolve_dependencies_async(self.dependencies, context, dependency_node)
         resolved_dependencies[self.decorated_arg] = instance
 
-        return await FactoryActivator.activate_async(
-            self.decorator_type, resolved_dependencies, context, lifespan=Lifespan.transient
+        return await self.activator_class.activate_async(
+            self.decorator_type, resolved_dependencies, context, lifespan=registration.lifespan
         )
 
 
 class Registration(Protocol):
     service_type: type
     implementation: Callable
     lifespan: Lifespan
@@ -921,15 +919,15 @@
         for dec in context.find_decorators_that_apply(self, decorated_instance_node=new_instance_node):
             next_decorated_node = DependencyNode(
                 service_type=self.service_type,
                 implementation=dec.decorator_type,
                 lifespan=self.lifespan,
             )
             top_decorated_node.add_decorator(next_decorated_node)
-            built_instance = dec.decorate(built_instance, context, next_decorated_node)
+            built_instance = dec.decorate(built_instance, context, next_decorated_node, self)
             next_decorated_node.set_instance(built_instance)
             top_decorated_node = next_decorated_node
 
         context.new_instance_created(self, top_decorated_node)
         self.was_used = True
         return built_instance
 
@@ -963,15 +961,15 @@
         for dec in context.find_decorators_that_apply(self, decorated_instance_node=new_instance_node):
             next_decorated_node = DependencyNode(
                 service_type=self.service_type,
                 implementation=dec.decorator_type,
                 lifespan=self.lifespan,
             )
             top_decorated_node.add_decorator(next_decorated_node)
-            built_instance = await dec.decorate_async(built_instance, context, next_decorated_node)
+            built_instance = await dec.decorate_async(built_instance, context, next_decorated_node, self)
             next_decorated_node.set_instance(built_instance)
             top_decorated_node = next_decorated_node
 
         context.new_instance_created(self, top_decorated_node)
         self.was_used = True
         return built_instance
 
@@ -1005,15 +1003,15 @@
             scoped_teardown=scoped_teardown,
             tags=tags,
         )
 
         self._registrations[service_type].appendleft(registration)
         self._registrations[implementation].appendleft(registration)
 
-    def register_as_self(
+    def register_concrete(
         self,
         *,
         service_type: type[TService],
         lifespan: Lifespan,
         name: str | None,
         dependency_config: DependencyConfig,
         tags: Iterable[Tag] | None,
@@ -1095,24 +1093,25 @@
 
         self._registrations[service_type].appendleft(registration)
 
     def register_decorator(
         self,
         *,
         service_type: type,
-        decorator_type: type,
+        decorator_type: type | Callable,
         registration_filter: Callable[[_Registration], bool],
         decorator_node_filter: NodeFilter,
         decorated_arg: str | None,
         dependency_config: DependencyConfig,
     ):
         decorator = Decorator(
             service_type=service_type,
             decorator_type=decorator_type,
             registration_filter=registration_filter,
+            activator_class=self._get_activator_class(decorator_type),
             decorator_node_filter=decorator_node_filter,
             decorated_arg=decorated_arg,
             dependency_config=dependency_config,
         )
         self._decorators[service_type].appendleft(decorator)
 
     def register_pre_configuration(
@@ -1399,15 +1398,15 @@
                 name=name,
                 tags=tags,
                 dependency_config=dependency_config,
                 parent_node_filter=parent_node_filter,
                 scoped_teardown=scoped_teardown,
             )
         else:
-            self._registry.register_as_self(
+            self._registry.register_concrete(
                 service_type=service_type,
                 lifespan=lifespan,
                 name=name,
                 tags=tags,
                 dependency_config=dependency_config,
                 parent_node_filter=parent_node_filter,
                 scoped_teardown=scoped_teardown,
@@ -1429,15 +1428,15 @@
             dependency_config=dependency_config,
             continue_on_failure=continue_on_failure,
         )
 
     def register_decorator(
         self,
         service_type: type,
-        decorator_type: type,
+        decorator_type: type | Callable,
         *,
         registration_filter: Callable[[_Registration], bool] = default_registration_filter,
         decorator_node_filter: NodeFilter = default_decorated_node_filter,
         decorated_arg: str | None = None,
         dependency_config: DependencyConfig = {},
     ):
         self._registry.register_decorator(
```

### Comparing `clean_ioc-1.0.0/clean_ioc/ext/fastapi/core.py` & `clean_ioc-1.1.0/clean_ioc/ext/fastapi/core.py`

 * *Files identical despite different names*

### Comparing `clean_ioc-1.0.0/clean_ioc/ext/fastapi/dependencies.py` & `clean_ioc-1.1.0/clean_ioc/ext/fastapi/dependencies.py`

 * *Files identical despite different names*

### Comparing `clean_ioc-1.0.0/clean_ioc/factories.py` & `clean_ioc-1.1.0/clean_ioc/factories.py`

 * *Files identical despite different names*

### Comparing `clean_ioc-1.0.0/clean_ioc/functional_utils.py` & `clean_ioc-1.1.0/clean_ioc/functional_utils.py`

 * *Files identical despite different names*

### Comparing `clean_ioc-1.0.0/clean_ioc/list_reduction_filters.py` & `clean_ioc-1.1.0/clean_ioc/list_reduction_filters.py`

 * *Files identical despite different names*

### Comparing `clean_ioc-1.0.0/clean_ioc/node_filters.py` & `clean_ioc-1.1.0/clean_ioc/node_filters.py`

 * *Files identical despite different names*

### Comparing `clean_ioc-1.0.0/clean_ioc/registration_filters.py` & `clean_ioc-1.1.0/clean_ioc/registration_filters.py`

 * *Files identical despite different names*

### Comparing `clean_ioc-1.0.0/clean_ioc/type_filters.py` & `clean_ioc-1.1.0/clean_ioc/type_filters.py`

 * *Files identical despite different names*

### Comparing `clean_ioc-1.0.0/clean_ioc/typing_utils.py` & `clean_ioc-1.1.0/clean_ioc/typing_utils.py`

 * *Files identical despite different names*

### Comparing `clean_ioc-1.0.0/clean_ioc/utils.py` & `clean_ioc-1.1.0/clean_ioc/utils.py`

 * *Files identical despite different names*

### Comparing `clean_ioc-1.0.0/clean_ioc/value_factories.py` & `clean_ioc-1.1.0/clean_ioc/value_factories.py`

 * *Files identical despite different names*

### Comparing `clean_ioc-1.0.0/pyproject.toml` & `clean_ioc-1.1.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [tool.poetry]
 name = "clean_ioc"
-version = "1.0.0"
+version = "1.1.0"
 description = "An IOC Container for Python 3.10+"
 authors = ["Peter Daly"]
 license = "MIT"
-homepage = "https://github.com/peter-daly/clean_ioc"
+homepage = "https://peter-daly.github.io/clean_ioc/"
 repository = "https://github.com/peter-daly/clean_ioc"
-documentation = "https://github.com/peter-daly/clean_ioc"
+documentation = "https://peter-daly.github.io/clean_ioc/"
 readme = "README.md"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
 ]
 packages = [
     { include = "clean_ioc" },
 ]
```

### Comparing `clean_ioc-1.0.0/PKG-INFO` & `clean_ioc-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: clean_ioc
-Version: 1.0.0
+Version: 1.1.0
 Summary: An IOC Container for Python 3.10+
-Home-page: https://github.com/peter-daly/clean_ioc
+Home-page: https://peter-daly.github.io/clean_ioc/
 License: MIT
 Author: Peter Daly
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: fastapi
 Requires-Dist: fastapi (>=0.101.0,<0.102.0) ; extra == "fastapi"
-Project-URL: Documentation, https://github.com/peter-daly/clean_ioc
+Project-URL: Documentation, https://peter-daly.github.io/clean_ioc/
 Project-URL: Repository, https://github.com/peter-daly/clean_ioc
 Description-Content-Type: text/markdown
 
 # Clean IoC
 A simple dependency injection library for python that requires nothing of your application code (except that you use typing).
```

