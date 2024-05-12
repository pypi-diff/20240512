# Comparing `tmp/sphyrna_service_manager-0.3.0.tar.gz` & `tmp/sphyrna_service_manager-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphyrna_service_manager-0.3.0.tar", max compression
+gzip compressed data, was "sphyrna_service_manager-0.3.7.tar", max compression
```

## Comparing `sphyrna_service_manager-0.3.0.tar` & `sphyrna_service_manager-0.3.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0        0 2024-02-04 05:39:16.967290 sphyrna_service_manager-0.3.0/README.md
--rw-r--r--   0        0        0      914 2024-04-15 00:07:31.162765 sphyrna_service_manager-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      558 2024-04-18 03:51:06.297129 sphyrna_service_manager-0.3.0/src/main/python/sphyrna/service_manager/__init__.py
--rw-r--r--   0        0        0      543 2024-04-18 03:51:06.737467 sphyrna_service_manager-0.3.0/src/main/python/sphyrna/service_manager/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0     3205 2024-04-15 00:25:08.957024 sphyrna_service_manager-0.3.0/src/main/python/sphyrna/service_manager/__pycache__/service.cpython-312.pyc
--rw-r--r--   0        0        0     1912 2024-04-14 17:41:03.989683 sphyrna_service_manager-0.3.0/src/main/python/sphyrna/service_manager/__pycache__/service_configuration.cpython-312.pyc
--rw-r--r--   0        0        0     2147 2024-04-15 00:24:53.346862 sphyrna_service_manager-0.3.0/src/main/python/sphyrna/service_manager/__pycache__/service_instance_provider.cpython-312.pyc
--rw-r--r--   0        0        0     5268 2024-04-15 00:45:12.135590 sphyrna_service_manager-0.3.0/src/main/python/sphyrna/service_manager/__pycache__/service_lifecycle_controller.cpython-312.pyc
--rw-r--r--   0        0        0     3176 2024-04-15 00:14:21.996585 sphyrna_service_manager-0.3.0/src/main/python/sphyrna/service_manager/__pycache__/service_manager.cpython-312.pyc
--rw-r--r--   0        0        0    11712 2024-04-15 00:43:00.227229 sphyrna_service_manager-0.3.0/src/main/python/sphyrna/service_manager/__pycache__/service_manager_strategy.cpython-312.pyc
--rw-r--r--   0        0        0     2095 2024-04-15 00:25:08.506102 sphyrna_service_manager-0.3.0/src/main/python/sphyrna/service_manager/service.py
--rw-r--r--   0        0        0     1081 2024-04-14 17:41:03.556091 sphyrna_service_manager-0.3.0/src/main/python/sphyrna/service_manager/service_configuration.py
--rw-r--r--   0        0        0     1168 2024-04-15 00:22:12.739346 sphyrna_service_manager-0.3.0/src/main/python/sphyrna/service_manager/service_instance_provider.py
--rw-r--r--   0        0        0     3887 2024-04-15 00:45:11.674827 sphyrna_service_manager-0.3.0/src/main/python/sphyrna/service_manager/service_lifecycle_controller.py
--rw-r--r--   0        0        0     2351 2024-04-15 00:14:21.519220 sphyrna_service_manager-0.3.0/src/main/python/sphyrna/service_manager/service_manager.py
--rw-r--r--   0        0        0    10673 2024-04-15 00:42:59.756495 sphyrna_service_manager-0.3.0/src/main/python/sphyrna/service_manager/service_manager_strategy.py
--rw-r--r--   0        0        0      410 1970-01-01 00:00:00.000000 sphyrna_service_manager-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-05-12 07:20:59.898995 sphyrna_service_manager-0.3.7/README.md
+-rw-r--r--   0        0        0      914 2024-05-12 07:20:59.899293 sphyrna_service_manager-0.3.7/pyproject.toml
+-rw-r--r--   0        0        0      558 2024-05-12 07:20:59.899742 sphyrna_service_manager-0.3.7/src/main/python/sphyrna/service_manager/__init__.py
+-rw-r--r--   0        0        0      559 2024-05-12 07:21:31.265548 sphyrna_service_manager-0.3.7/src/main/python/sphyrna/service_manager/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0     3221 2024-05-12 07:21:31.268218 sphyrna_service_manager-0.3.7/src/main/python/sphyrna/service_manager/__pycache__/service.cpython-312.pyc
+-rw-r--r--   0        0        0     1936 2024-05-12 07:21:31.266462 sphyrna_service_manager-0.3.7/src/main/python/sphyrna/service_manager/__pycache__/service_configuration.cpython-312.pyc
+-rw-r--r--   0        0        0     2163 2024-05-12 07:21:31.267337 sphyrna_service_manager-0.3.7/src/main/python/sphyrna/service_manager/__pycache__/service_instance_provider.cpython-312.pyc
+-rw-r--r--   0        0        0     5284 2024-05-12 07:21:31.269517 sphyrna_service_manager-0.3.7/src/main/python/sphyrna/service_manager/__pycache__/service_lifecycle_controller.cpython-312.pyc
+-rw-r--r--   0        0        0     3192 2024-05-12 07:21:31.277315 sphyrna_service_manager-0.3.7/src/main/python/sphyrna/service_manager/__pycache__/service_manager.cpython-312.pyc
+-rw-r--r--   0        0        0    11728 2024-05-12 07:21:31.276326 sphyrna_service_manager-0.3.7/src/main/python/sphyrna/service_manager/__pycache__/service_manager_strategy.cpython-312.pyc
+-rw-r--r--   0        0        0     2095 2024-05-12 07:20:59.900535 sphyrna_service_manager-0.3.7/src/main/python/sphyrna/service_manager/service.py
+-rw-r--r--   0        0        0     1081 2024-05-12 07:20:59.900601 sphyrna_service_manager-0.3.7/src/main/python/sphyrna/service_manager/service_configuration.py
+-rw-r--r--   0        0        0     1168 2024-05-12 07:20:59.900670 sphyrna_service_manager-0.3.7/src/main/python/sphyrna/service_manager/service_instance_provider.py
+-rw-r--r--   0        0        0     3887 2024-05-12 07:20:59.900757 sphyrna_service_manager-0.3.7/src/main/python/sphyrna/service_manager/service_lifecycle_controller.py
+-rw-r--r--   0        0        0     2351 2024-05-12 07:20:59.900830 sphyrna_service_manager-0.3.7/src/main/python/sphyrna/service_manager/service_manager.py
+-rw-r--r--   0        0        0    10673 2024-05-12 07:20:59.900919 sphyrna_service_manager-0.3.7/src/main/python/sphyrna/service_manager/service_manager_strategy.py
+-rw-r--r--   0        0        0      410 1970-01-01 00:00:00.000000 sphyrna_service_manager-0.3.7/PKG-INFO
```

### Comparing `sphyrna_service_manager-0.3.0/pyproject.toml` & `sphyrna_service_manager-0.3.7/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sphyrna-service-manager"
-version = "0.3.0"
+version = "0.3.7"
 description = "Python implementation of a service manager framework"
 authors = ["Scott Goldstein <sgoldstein@apache.org>"]
 readme = "README.md"
 packages = [{include = "src/main/python/sphyrna"}]
 
 [tool.poetry.dependencies]
 python = "^3.12"
```

### Comparing `sphyrna_service_manager-0.3.0/src/main/python/sphyrna/service_manager/__init__.py` & `sphyrna_service_manager-0.3.7/src/main/python/sphyrna/service_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `sphyrna_service_manager-0.3.0/src/main/python/sphyrna/service_manager/__pycache__/__init__.cpython-312.pyc` & `sphyrna_service_manager-0.3.7/src/main/python/sphyrna/service_manager/__pycache__/__init__.cpython-312.pyc`

 * *Files 4% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xcb0d0d0a
-moddate:  0xaa982066 (Thu Apr 18 03:51:06 2024 UTC)
+moddate:  0xdb6d4066 (Sun May 12 07:20:59 2024 UTC)
 files sz: 558
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 2
    flags     : 0
    code
@@ -67,11 +67,11 @@
       ('service_manager',)
       ('service',)
       None
    names      ('__doc__', '', 'service_configuration', 'service_instance_provider', 'service_lifecycle_controller', 'service_manager_strategy', 'service_manager', 'service')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   '/Users/kameleon/Code/service/packages/pythonlib/src/main/python/sphyrna/service_manager/__init__.py'
+   filename   '/Users/kameleon/Code/service/target/checkout/packages/pythonlib/src/main/python/sphyrna/service_manager/__init__.py'
    name       '<module>'
    firstlineno 1
    lnotab 0x00ff020104050c030c030c030c030c03
```

### Comparing `sphyrna_service_manager-0.3.0/src/main/python/sphyrna/service_manager/__pycache__/service.cpython-312.pyc` & `sphyrna_service_manager-0.3.7/src/main/python/sphyrna/service_manager/__pycache__/service.cpython-312.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xcb0d0d0a
-moddate:  0xe4731c66 (Mon Apr 15 00:25:08 2024 UTC)
+moddate:  0xdb6d4066 (Sun May 12 07:20:59 2024 UTC)
 files sz: 2095
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
@@ -51,26 +51,26 @@
                 68 LOAD_NAME                2 (TypeVar)
                 70 LOAD_CONST               8 ('ConfigurationT')
                 72 LOAD_CONST               9 ('ServiceConfiguration')
                 74 KW_NAMES                 7
                 76 CALL                     2
    
     19          86 PUSH_NULL
-                88 LOAD_CONST              10 (<code object <generic parameters of Service>, file "/Users/kameleon/Code/service/packages/pythonlib/src/main/python/sphyrna/service_manager/service.py", line 19>)
+                88 LOAD_CONST              10 (<code object <generic parameters of Service>, file "/Users/kameleon/Code/service/target/checkout/packages/pythonlib/src/main/python/sphyrna/service_manager/service.py", line 19>)
                 90 MAKE_FUNCTION            0
                 92 CALL                     0
    
     45         102 PUSH_NULL
-               104 LOAD_CONST              11 (<code object <generic parameters of BaseService>, file "/Users/kameleon/Code/service/packages/pythonlib/src/main/python/sphyrna/service_manager/service.py", line 45>)
+               104 LOAD_CONST              11 (<code object <generic parameters of BaseService>, file "/Users/kameleon/Code/service/target/checkout/packages/pythonlib/src/main/python/sphyrna/service_manager/service.py", line 45>)
                106 MAKE_FUNCTION            0
                108 CALL                     0
    
     66         118 PUSH_NULL
                120 LOAD_BUILD_CLASS
-               122 LOAD_CONST              12 (<code object ServiceException, file "/Users/kameleon/Code/service/packages/pythonlib/src/main/python/sphyrna/service_manager/service.py", line 66>)
+               122 LOAD_CONST              12 (<code object ServiceException, file "/Users/kameleon/Code/service/target/checkout/packages/pythonlib/src/main/python/sphyrna/service_manager/service.py", line 66>)
                124 MAKE_FUNCTION            0
                126 LOAD_CONST              13 ('ServiceException')
                128 LOAD_NAME               12 (Exception)
                130 CALL                     3
                140 PRECALL                 14
    consts
       '\n    service module defines a Service class/interface\n'
@@ -103,15 +103,15 @@
                       14 BUILD_TUPLE              1
                       16 STORE_DEREF              1 (.type_params)
                  >>   18 PUSH_NULL
                       20 LOAD_BUILD_CLASS
                       22 LOAD_CLOSURE             1 (.type_params)
                       24 LOAD_CLOSURE             2 (ConfigurationT)
                       26 BUILD_TUPLE              2
-                      28 LOAD_CONST               1 (<code object Service, file "/Users/kameleon/Code/service/packages/pythonlib/src/main/python/sphyrna/service_manager/service.py", line 19>)
+                      28 LOAD_CONST               1 (<code object Service, file "/Users/kameleon/Code/service/target/checkout/packages/pythonlib/src/main/python/sphyrna/service_manager/service.py", line 19>)
                       30 MAKE_FUNCTION            8 (closure)
                       32 LOAD_CONST               2 ('Service')
                       34 LOAD_DEREF               1 (.type_params)
                       36 POP_JUMP_BACKWARD_IF_NOT_NONE    10 (to 18)
                       38 STORE_FAST               0 (.generic_base)
                       40 LOAD_GLOBAL              0 (ABC)
                       52 CALL                     4
@@ -145,39 +145,39 @@
                
                 23          24 LOAD_CONST               2 ('configuration')
                             26 ASYNC_GEN_WRAP
                        >>   28 POP_JUMP_BACKWARD_IF_TRUE     1 (to 28)
                             30 LOAD_CONST               3 ('return')
                             32 LOAD_CONST               4 (None)
                             34 BUILD_TUPLE              4
-                            36 LOAD_CONST               5 (<code object init, file "/Users/kameleon/Code/service/packages/pythonlib/src/main/python/sphyrna/service_manager/service.py", line 22>)
+                            36 LOAD_CONST               5 (<code object init, file "/Users/kameleon/Code/service/target/checkout/packages/pythonlib/src/main/python/sphyrna/service_manager/service.py", line 22>)
                             38 MAKE_FUNCTION            4 (annotations)
                
                 22          40 CALL                     0
                
                 29          50 LOAD_NAME                5 (abstractmethod)
                
                 30          52 LOAD_CONST               9 (('return', None))
-                            54 LOAD_CONST               6 (<code object start, file "/Users/kameleon/Code/service/packages/pythonlib/src/main/python/sphyrna/service_manager/service.py", line 29>)
+                            54 LOAD_CONST               6 (<code object start, file "/Users/kameleon/Code/service/target/checkout/packages/pythonlib/src/main/python/sphyrna/service_manager/service.py", line 29>)
                             56 MAKE_FUNCTION            4 (annotations)
                
                 29          58 CALL                     0
                
                 33          68 LOAD_NAME                5 (abstractmethod)
                
                 34          70 LOAD_CONST               9 (('return', None))
-                            72 LOAD_CONST               7 (<code object stop, file "/Users/kameleon/Code/service/packages/pythonlib/src/main/python/sphyrna/service_manager/service.py", line 33>)
+                            72 LOAD_CONST               7 (<code object stop, file "/Users/kameleon/Code/service/target/checkout/packages/pythonlib/src/main/python/sphyrna/service_manager/service.py", line 33>)
                             74 MAKE_FUNCTION            4 (annotations)
                
                 33          76 CALL                     0
                
                 37          86 LOAD_NAME                5 (abstractmethod)
                
                 38          88 LOAD_CONST               9 (('return', None))
-                            90 LOAD_CONST               8 (<code object destroy, file "/Users/kameleon/Code/service/packages/pythonlib/src/main/python/sphyrna/service_manager/service.py", line 37>)
+                            90 LOAD_CONST               8 (<code object destroy, file "/Users/kameleon/Code/service/target/checkout/packages/pythonlib/src/main/python/sphyrna/service_manager/service.py", line 37>)
                             92 MAKE_FUNCTION            4 (annotations)
                
                 37          94 CALL                     0
                            104 PRECALL                  4
                consts
                   'Service'
                   'A Service is a predefined component of functionality with a lifecycle managed by the ServiceManger.'
@@ -195,15 +195,15 @@
                      consts
                         'Initialize the service instance\n\n        Args:\n            configuration (C): Service level configuration'
                         None
                      names      ()
                      varnames   ('self', 'configuration')
                      freevars   ()
                      cellvars   ()
-                     filename   '/Users/kameleon/Code/service/packages/pythonlib/src/main/python/sphyrna/service_manager/service.py'
+                     filename   '/Users/kameleon/Code/service/target/checkout/packages/pythonlib/src/main/python/sphyrna/service_manager/service.py'
                      name       'init'
                      firstlineno 22
                      lnotab 0x
                   code
                      argcount  : 1
                      nlocals   : 1
                      stacksize : 0
@@ -214,15 +214,15 @@
                      consts
                         'Start the service instances'
                         None
                      names      ()
                      varnames   ('self',)
                      freevars   ()
                      cellvars   ()
-                     filename   '/Users/kameleon/Code/service/packages/pythonlib/src/main/python/sphyrna/service_manager/service.py'
+                     filename   '/Users/kameleon/Code/service/target/checkout/packages/pythonlib/src/main/python/sphyrna/service_manager/service.py'
                      name       'start'
                      firstlineno 29
                      lnotab 0x
                   code
                      argcount  : 1
                      nlocals   : 1
                      stacksize : 0
@@ -233,15 +233,15 @@
                      consts
                         'Stop the service instance'
                         None
                      names      ()
                      varnames   ('self',)
                      freevars   ()
                      cellvars   ()
-                     filename   '/Users/kameleon/Code/service/packages/pythonlib/src/main/python/sphyrna/service_manager/service.py'
+                     filename   '/Users/kameleon/Code/service/target/checkout/packages/pythonlib/src/main/python/sphyrna/service_manager/service.py'
                      name       'stop'
                      firstlineno 33
                      lnotab 0x
                   code
                      argcount  : 1
                      nlocals   : 1
                      stacksize : 0
@@ -252,35 +252,35 @@
                      consts
                         'Destroy the service instance.  Can be used to clean up memory or other resources'
                         None
                      names      ()
                      varnames   ('self',)
                      freevars   ()
                      cellvars   ()
-                     filename   '/Users/kameleon/Code/service/packages/pythonlib/src/main/python/sphyrna/service_manager/service.py'
+                     filename   '/Users/kameleon/Code/service/target/checkout/packages/pythonlib/src/main/python/sphyrna/service_manager/service.py'
                      name       'destroy'
                      firstlineno 37
                      lnotab 0x
                   ('return', None)
                names      ('__name__', '__module__', '__qualname__', '__type_params__', '__doc__', 'abstractmethod', 'init', 'start', 'stop', 'destroy')
                varnames   ()
                freevars   ('.type_params', 'ConfigurationT')
                cellvars   ()
-               filename   '/Users/kameleon/Code/service/packages/pythonlib/src/main/python/sphyrna/service_manager/service.py'
+               filename   '/Users/kameleon/Code/service/target/checkout/packages/pythonlib/src/main/python/sphyrna/service_manager/service.py'
                name       'Service'
                firstlineno 19
                lnotab
                   0x12010402020110ff08010206020106ff08010203020106ff0801020302
                   0106ff0801
             'Service'
          names      ('ABC',)
          varnames   ('.generic_base',)
          freevars   ()
          cellvars   ('.type_params', 'ConfigurationT')
-         filename   '/Users/kameleon/Code/service/packages/pythonlib/src/main/python/sphyrna/service_manager/service.py'
+         filename   '/Users/kameleon/Code/service/target/checkout/packages/pythonlib/src/main/python/sphyrna/service_manager/service.py'
          name       '<generic parameters of Service>'
          firstlineno 19
          lnotab 0x
       code
          argcount  : 0
          nlocals   : 1
          stacksize : 6
@@ -300,15 +300,15 @@
                       14 BUILD_TUPLE              1
                       16 STORE_DEREF              1 (.type_params)
                  >>   18 PUSH_NULL
                       20 LOAD_BUILD_CLASS
                       22 LOAD_CLOSURE             1 (.type_params)
                       24 LOAD_CLOSURE             2 (ConfigurationT)
                       26 BUILD_TUPLE              2
-                      28 LOAD_CONST               1 (<code object BaseService, file "/Users/kameleon/Code/service/packages/pythonlib/src/main/python/sphyrna/service_manager/service.py", line 45>)
+                      28 LOAD_CONST               1 (<code object BaseService, file "/Users/kameleon/Code/service/target/checkout/packages/pythonlib/src/main/python/sphyrna/service_manager/service.py", line 45>)
                       30 MAKE_FUNCTION            8 (closure)
                       32 LOAD_CONST               2 ('BaseService')
                       34 LOAD_DEREF               1 (.type_params)
                       36 POP_JUMP_BACKWARD_IF_NOT_NONE    10 (to 18)
                       38 STORE_FAST               0 (.generic_base)
                       40 LOAD_GLOBAL              0 (Service)
                       52 CALL                     4
@@ -339,30 +339,30 @@
                
                 51          22 LOAD_CONST               2 ('configuration')
                             24 ASYNC_GEN_WRAP
                        >>   26 POP_JUMP_BACKWARD_IF_TRUE     1 (to 26)
                             28 LOAD_CONST               3 ('return')
                             30 LOAD_CONST               4 (None)
                             32 BUILD_TUPLE              4
-                            34 LOAD_CONST               5 (<code object init, file "/Users/kameleon/Code/service/packages/pythonlib/src/main/python/sphyrna/service_manager/service.py", line 51>)
+                            34 LOAD_CONST               5 (<code object init, file "/Users/kameleon/Code/service/target/checkout/packages/pythonlib/src/main/python/sphyrna/service_manager/service.py", line 51>)
                             36 MAKE_FUNCTION            4 (annotations)
                             38 STORE_NAME               5 (init)
                
                 54          40 LOAD_CONST               9 (('return', None))
-                            42 LOAD_CONST               6 (<code object start, file "/Users/kameleon/Code/service/packages/pythonlib/src/main/python/sphyrna/service_manager/service.py", line 54>)
+                            42 LOAD_CONST               6 (<code object start, file "/Users/kameleon/Code/service/target/checkout/packages/pythonlib/src/main/python/sphyrna/service_manager/service.py", line 54>)
                             44 MAKE_FUNCTION            4 (annotations)
                             46 STORE_NAME               6 (start)
                
                 57          48 LOAD_CONST               9 (('return', None))
-                            50 LOAD_CONST               7 (<code object stop, file "/Users/kameleon/Code/service/packages/pythonlib/src/main/python/sphyrna/service_manager/service.py", line 57>)
+                            50 LOAD_CONST               7 (<code object stop, file "/Users/kameleon/Code/service/target/checkout/packages/pythonlib/src/main/python/sphyrna/service_manager/service.py", line 57>)
                             52 MAKE_FUNCTION            4 (annotations)
                             54 STORE_NAME               7 (stop)
                
                 60          56 LOAD_CONST               9 (('return', None))
-                            58 LOAD_CONST               8 (<code object destroy, file "/Users/kameleon/Code/service/packages/pythonlib/src/main/python/sphyrna/service_manager/service.py", line 60>)
+                            58 LOAD_CONST               8 (<code object destroy, file "/Users/kameleon/Code/service/target/checkout/packages/pythonlib/src/main/python/sphyrna/service_manager/service.py", line 60>)
                             60 MAKE_FUNCTION            4 (annotations)
                             62 STORE_NAME               8 (destroy)
                             64 PRECALL                  4
                consts
                   'BaseService'
                   '\n    Base instance of a Service which is a noop for all methods.  Extend to create a new service and\n    implement the methods that are required\n    '
                   'configuration'
@@ -379,15 +379,15 @@
                       52           2 PRECALL                  0
                      consts
                         None
                      names      ()
                      varnames   ('self', 'configuration')
                      freevars   ()
                      cellvars   ()
-                     filename   '/Users/kameleon/Code/service/packages/pythonlib/src/main/python/sphyrna/service_manager/service.py'
+                     filename   '/Users/kameleon/Code/service/target/checkout/packages/pythonlib/src/main/python/sphyrna/service_manager/service.py'
                      name       'init'
                      firstlineno 51
                      lnotab 0x0201
                   code
                      argcount  : 1
                      nlocals   : 1
                      stacksize : 0
@@ -398,15 +398,15 @@
                       55           2 PRECALL                  0
                      consts
                         None
                      names      ()
                      varnames   ('self',)
                      freevars   ()
                      cellvars   ()
-                     filename   '/Users/kameleon/Code/service/packages/pythonlib/src/main/python/sphyrna/service_manager/service.py'
+                     filename   '/Users/kameleon/Code/service/target/checkout/packages/pythonlib/src/main/python/sphyrna/service_manager/service.py'
                      name       'start'
                      firstlineno 54
                      lnotab 0x0201
                   code
                      argcount  : 1
                      nlocals   : 1
                      stacksize : 0
@@ -417,15 +417,15 @@
                       58           2 PRECALL                  0
                      consts
                         None
                      names      ()
                      varnames   ('self',)
                      freevars   ()
                      cellvars   ()
-                     filename   '/Users/kameleon/Code/service/packages/pythonlib/src/main/python/sphyrna/service_manager/service.py'
+                     filename   '/Users/kameleon/Code/service/target/checkout/packages/pythonlib/src/main/python/sphyrna/service_manager/service.py'
                      name       'stop'
                      firstlineno 57
                      lnotab 0x0201
                   code
                      argcount  : 1
                      nlocals   : 1
                      stacksize : 0
@@ -436,33 +436,33 @@
                       61           2 PRECALL                  0
                      consts
                         None
                      names      ()
                      varnames   ('self',)
                      freevars   ()
                      cellvars   ()
-                     filename   '/Users/kameleon/Code/service/packages/pythonlib/src/main/python/sphyrna/service_manager/service.py'
+                     filename   '/Users/kameleon/Code/service/target/checkout/packages/pythonlib/src/main/python/sphyrna/service_manager/service.py'
                      name       'destroy'
                      firstlineno 60
                      lnotab 0x0201
                   ('return', None)
                names      ('__name__', '__module__', '__qualname__', '__type_params__', '__doc__', 'init', 'start', 'stop', 'destroy')
                varnames   ()
                freevars   ('.type_params', 'ConfigurationT')
                cellvars   ()
-               filename   '/Users/kameleon/Code/service/packages/pythonlib/src/main/python/sphyrna/service_manager/service.py'
+               filename   '/Users/kameleon/Code/service/target/checkout/packages/pythonlib/src/main/python/sphyrna/service_manager/service.py'
                name       'BaseService'
                firstlineno 45
                lnotab 0x12010405120308030803
             'BaseService'
          names      ('Service',)
          varnames   ('.generic_base',)
          freevars   ()
          cellvars   ('.type_params', 'ConfigurationT')
-         filename   '/Users/kameleon/Code/service/packages/pythonlib/src/main/python/sphyrna/service_manager/service.py'
+         filename   '/Users/kameleon/Code/service/target/checkout/packages/pythonlib/src/main/python/sphyrna/service_manager/service.py'
          name       '<generic parameters of BaseService>'
          firstlineno 45
          lnotab 0x
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
@@ -481,21 +481,21 @@
             'ServiceException'
             '\n    Service API Exception\n    '
             None
          names      ('__name__', '__module__', '__qualname__', '__doc__')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   '/Users/kameleon/Code/service/packages/pythonlib/src/main/python/sphyrna/service_manager/service.py'
+         filename   '/Users/kameleon/Code/service/target/checkout/packages/pythonlib/src/main/python/sphyrna/service_manager/service.py'
          name       'ServiceException'
          firstlineno 66
          lnotab 0x0a01
       'ServiceException'
       None
    names      ('__doc__', 'typing', 'TypeVar', 'abc', 'ABC', 'abstractmethod', 'sphyrna.service_manager.service_configuration', 'ServiceConfiguration', 'ServiceT', 'ConfigurationT', 'Service', 'BaseService', 'Exception', 'ServiceException')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   '/Users/kameleon/Code/service/packages/pythonlib/src/main/python/sphyrna/service_manager/service.py'
+   filename   '/Users/kameleon/Code/service/target/checkout/packages/pythonlib/src/main/python/sphyrna/service_manager/service.py'
    name       '<module>'
    firstlineno 1
    lnotab 0x00ff020104040c0110040c0414011404101a1015
```

### Comparing `sphyrna_service_manager-0.3.0/src/main/python/sphyrna/service_manager/__pycache__/service_configuration.cpython-312.pyc` & `sphyrna_service_manager-0.3.7/src/main/python/sphyrna/service_manager/__pycache__/service_configuration.cpython-312.pyc`

 * *Files 3% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xcb0d0d0a
-moddate:  0x2f151c66 (Sun Apr 14 17:41:03 2024 UTC)
+moddate:  0xdb6d4066 (Sun May 12 07:20:59 2024 UTC)
 files sz: 1081
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 7
    flags     : 0
    code
@@ -43,23 +43,23 @@
                 48 LOAD_NAME                8 (float)
                 50 LOAD_NAME                9 (str)
                 52 LOAD_NAME               10 (bool)
                 54 CALL                     5
    
     11          64 PUSH_NULL
                 66 LOAD_BUILD_CLASS
-                68 LOAD_CONST               5 (<code object ServiceConfiguration, file "/Users/kameleon/Code/service/packages/pythonlib/src/main/python/service_manager/service_configuration.py", line 11>)
+                68 LOAD_CONST               5 (<code object ServiceConfiguration, file "/Users/kameleon/Code/service/target/checkout/packages/pythonlib/src/main/python/sphyrna/service_manager/service_configuration.py", line 11>)
                 70 MAKE_FUNCTION            0
                 72 LOAD_CONST               6 ('ServiceConfiguration')
                 74 LOAD_NAME                5 (ABC)
                 76 CALL                     3
    
     21          86 PUSH_NULL
                 88 LOAD_BUILD_CLASS
-                90 LOAD_CONST               7 (<code object DefaultServiceConfigurationImpl, file "/Users/kameleon/Code/service/packages/pythonlib/src/main/python/service_manager/service_configuration.py", line 21>)
+                90 LOAD_CONST               7 (<code object DefaultServiceConfigurationImpl, file "/Users/kameleon/Code/service/target/checkout/packages/pythonlib/src/main/python/sphyrna/service_manager/service_configuration.py", line 21>)
                 92 MAKE_FUNCTION            0
                 94 LOAD_CONST               8 ('DefaultServiceConfigurationImpl')
                 96 LOAD_NAME               12 (ServiceConfiguration)
                 98 CALL                     3
    
     36         108 PUSH_NULL
                110 LOAD_NAME               13 (DefaultServiceConfigurationImpl)
@@ -119,24 +119,24 @@
                consts
                   '\n        Retrieve the configuration parameters for the service\n        '
                   None
                names      ()
                varnames   ('self',)
                freevars   ()
                cellvars   ()
-               filename   '/Users/kameleon/Code/service/packages/pythonlib/src/main/python/service_manager/service_configuration.py'
+               filename   '/Users/kameleon/Code/service/target/checkout/packages/pythonlib/src/main/python/sphyrna/service_manager/service_configuration.py'
                name       'poperty_map'
                firstlineno 14
                lnotab 0x
             None
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'abstractmethod', 'Mapping', 'str', 'ConfigValue', 'poperty_map')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   '/Users/kameleon/Code/service/packages/pythonlib/src/main/python/service_manager/service_configuration.py'
+         filename   '/Users/kameleon/Code/service/target/checkout/packages/pythonlib/src/main/python/sphyrna/service_manager/service_configuration.py'
          name       'ServiceConfiguration'
          firstlineno 11
          lnotab 0x0a010402020114ff0801
       'ServiceConfiguration'
       code
          argcount  : 0
          nlocals   : 0
@@ -189,15 +189,15 @@
                             16 PRECALL                  0
                consts
                   None
                names      ('_property_map',)
                varnames   ('self', 'properties')
                freevars   ()
                cellvars   ()
-               filename   '/Users/kameleon/Code/service/packages/pythonlib/src/main/python/service_manager/service_configuration.py'
+               filename   '/Users/kameleon/Code/service/target/checkout/packages/pythonlib/src/main/python/sphyrna/service_manager/service_configuration.py'
                name       '__init__'
                firstlineno 27
                lnotab 0x0201
             'return'
             code
                argcount  : 1
                nlocals   : 1
@@ -216,31 +216,31 @@
                             24 RETURN_VALUE
                consts
                   None
                names      ('_property_map',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
-               filename   '/Users/kameleon/Code/service/packages/pythonlib/src/main/python/service_manager/service_configuration.py'
+               filename   '/Users/kameleon/Code/service/target/checkout/packages/pythonlib/src/main/python/sphyrna/service_manager/service_configuration.py'
                name       'poperty_map'
                firstlineno 30
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'Mapping', 'str', 'ConfigValue', '__init__', 'poperty_map')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   '/Users/kameleon/Code/service/packages/pythonlib/src/main/python/service_manager/service_configuration.py'
+         filename   '/Users/kameleon/Code/service/target/checkout/packages/pythonlib/src/main/python/sphyrna/service_manager/service_configuration.py'
          name       'DefaultServiceConfigurationImpl'
          firstlineno 21
          lnotab 0x0a0104051603
       'DefaultServiceConfigurationImpl'
       'EMPTY_SERVICE_CONFIGURATION'
       None
    names      ('__doc__', 'typing', 'TypeVar', 'Mapping', 'abc', 'ABC', 'abstractmethod', 'int', 'float', 'str', 'bool', 'ConfigValue', 'ServiceConfiguration', 'DefaultServiceConfigurationImpl', 'EMPTY_SERVICE_CONFIGURATION', '__annotations__')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   '/Users/kameleon/Code/service/packages/pythonlib/src/main/python/service_manager/service_configuration.py'
+   filename   '/Users/kameleon/Code/service/target/checkout/packages/pythonlib/src/main/python/sphyrna/service_manager/service_configuration.py'
    name       '<module>'
    firstlineno 1
    lnotab 0x00ff02010604100110021803160a160f
```

### Comparing `sphyrna_service_manager-0.3.0/src/main/python/sphyrna/service_manager/__pycache__/service_instance_provider.cpython-312.pyc` & `sphyrna_service_manager-0.3.7/src/main/python/sphyrna/service_manager/__pycache__/service_instance_provider.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Mon Apr 15 00:22:12 2024 UTC, .py size: 1168 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 3473 1c66 9004 0000  ........4s.f....
+00000000: cb0d 0d0a 0000 0000 db6d 4066 9004 0000  .........m@f....
 00000010: e300 0000 0000 0000 0000 0000 0006 0000  ................
 00000020: 0000 0000 00f3 5000 0000 9700 6400 5a00  ......P.....d.Z.
 00000030: 6401 6402 6c01 6d02 5a02 6d03 5a03 0100  d.d.l.m.Z.m.Z...
 00000040: 6401 6403 6c04 6d05 5a05 0100 0200 6404  d.d.l.m.Z.....d.
 00000050: 8400 ab00 0000 0000 0000 5a06 0200 4700  ..........Z...G.
 00000060: 6405 8400 6406 6506 6505 1900 0000 ab03  d...d.e.e.......
 00000070: 0000 0000 0000 5a07 7907 2908 7a89 0a54  ......Z.y.).z..T
@@ -36,100 +36,101 @@
 00000230: 2061 2073 6572 7669 6365 2e0a 2020 2020   a service..    
 00000240: da06 7265 7475 726e 6301 0000 0000 0000  ..returnc.......
 00000250: 0000 0000 0000 0000 0013 0000 00f3 0400  ................
 00000260: 0000 9700 7901 2902 7a2b 0a20 2020 2020  ....y.).z+.     
 00000270: 2020 2043 7265 6174 6520 6120 5365 7276     Create a Serv
 00000280: 6963 6520 696e 7374 616e 6365 0a20 2020  ice instance.   
 00000290: 2020 2020 204e a900 a901 da04 7365 6c66       N......self
-000002a0: 7301 0000 0020 fa74 2f55 7365 7273 2f6b  s.... .t/Users/k
+000002a0: 7301 0000 0020 fa84 2f55 7365 7273 2f6b  s.... ../Users/k
 000002b0: 616d 656c 656f 6e2f 436f 6465 2f73 6572  ameleon/Code/ser
-000002c0: 7669 6365 2f70 6163 6b61 6765 732f 7079  vice/packages/py
-000002d0: 7468 6f6e 6c69 622f 7372 632f 6d61 696e  thonlib/src/main
-000002e0: 2f70 7974 686f 6e2f 7370 6879 726e 612f  /python/sphyrna/
-000002f0: 7365 7276 6963 655f 6d61 6e61 6765 722f  service_manager/
-00000300: 7365 7276 6963 655f 696e 7374 616e 6365  service_instance
-00000310: 5f70 726f 7669 6465 722e 7079 da17 6372  _provider.py..cr
-00000320: 6561 7465 5f73 6572 7669 6365 5f69 6e73  eate_service_ins
-00000330: 7461 6e63 657a 2f53 6572 7669 6365 496e  tancez/ServiceIn
-00000340: 7374 616e 6365 5072 6f76 6964 6572 2e63  stanceProvider.c
-00000350: 7265 6174 655f 7365 7276 6963 655f 696e  reate_service_in
-00000360: 7374 616e 6365 1100 0000 7302 0000 0081  stance....s.....
-00000370: 00f3 0000 0000 4e29 07da 085f 5f6e 616d  ......N)...__nam
-00000380: 655f 5fda 0a5f 5f6d 6f64 756c 655f 5fda  e__..__module__.
-00000390: 0c5f 5f71 7561 6c6e 616d 655f 5fda 0f5f  .__qualname__.._
-000003a0: 5f74 7970 655f 7061 7261 6d73 5f5f da07  _type_params__..
-000003b0: 5f5f 646f 635f 5f72 0400 0000 720f 0000  __doc__r....r...
-000003c0: 0029 02da 0c2e 7479 7065 5f70 6172 616d  .)....type_param
-000003d0: 7372 0500 0000 7302 0000 0080 8072 0e00  sr....s......r..
-000003e0: 0000 7208 0000 0072 0800 0000 0c00 0000  ..r....r........
-000003f0: 7323 0000 00f8 8700 f102 0205 08f0 0800  s#..............
-00000400: 0614 f002 0305 0ca9 18f2 0003 050c f303  ................
-00000410: 0006 14f1 0203 050c 7210 0000 0072 0800  ........r....r..
-00000420: 0000 2901 7203 0000 0029 03da 0d2e 6765  ..).r....)....ge
-00000430: 6e65 7269 635f 6261 7365 7216 0000 0072  neric_baser....r
-00000440: 0500 0000 7303 0000 0020 4040 720e 0000  ....s.... @@r...
-00000450: 00fa 2f3c 6765 6e65 7269 6320 7061 7261  ../<generic para
-00000460: 6d65 7465 7273 206f 6620 5365 7276 6963  meters of Servic
-00000470: 6549 6e73 7461 6e63 6550 726f 7669 6465  eInstanceProvide
-00000480: 723e 7218 0000 000c 0000 0073 1600 0000  r>r........s....
-00000490: f980 009c 68f7 0009 010c f300 0901 0cac  ....h...........
-000004a0: 03f5 0009 010c 7210 0000 0063 0000 0000  ......r....c....
-000004b0: 0000 0000 0000 0000 0200 0000 0000 0000  ................
-000004c0: f328 0000 0097 0065 005a 0164 005a 0264  .(.....e.Z.d.Z.d
-000004d0: 015a 0364 0265 0466 0264 0384 045a 0564  .Z.d.e.f.d...Z.d
-000004e0: 0465 0666 0264 0584 045a 0779 0629 07da  .e.f.d...Z.y.)..
-000004f0: 2244 6566 6175 6c74 5365 7276 6963 6549  "DefaultServiceI
-00000500: 6e73 7461 6e63 6550 726f 7669 6465 7249  nstanceProviderI
-00000510: 6d70 6c7a 9a0a 2020 2020 4465 6661 756c  mplz..    Defaul
-00000520: 7453 6572 7669 6365 496e 7374 616e 6365  tServiceInstance
-00000530: 5072 6f76 6964 6572 496d 706c 2069 7320  ProviderImpl is 
-00000540: 6120 7365 7276 6963 6520 7072 6f76 6964  a service provid
-00000550: 6572 2074 6861 7420 7369 6d70 6c79 2069  er that simply i
-00000560: 6e76 6f6b 6573 2074 6865 2070 726f 7669  nvokes the provi
-00000570: 6465 6420 7365 7276 6963 6520 636f 6e73  ded service cons
-00000580: 7472 7563 746f 7220 746f 0a20 2020 2063  tructor to.    c
-00000590: 7265 6174 6520 7468 6520 7365 7276 6963  reate the servic
-000005a0: 6520 696e 7374 616e 6365 0a20 2020 20da  e instance.    .
-000005b0: 0d73 6572 7669 6365 5f63 6c61 7373 6302  .service_classc.
-000005c0: 0000 0000 0000 0000 0000 0002 0000 0003  ................
-000005d0: 0000 00f3 1200 0000 9700 7c01 7c00 5f00  ..........|.|._.
-000005e0: 0000 0000 0000 0000 7900 2901 4ea9 0172  ........y.).N..r
-000005f0: 1b00 0000 2902 720d 0000 0072 1b00 0000  ....).r....r....
-00000600: 7302 0000 0020 2072 0e00 0000 da08 5f5f  s....  r......__
-00000610: 696e 6974 5f5f 7a2b 4465 6661 756c 7453  init__z+DefaultS
-00000620: 6572 7669 6365 496e 7374 616e 6365 5072  erviceInstancePr
-00000630: 6f76 6964 6572 496d 706c 2e5f 5f69 6e69  oviderImpl.__ini
-00000640: 745f 5f20 0000 0073 0a00 0000 8000 d81d  t__ ...s........
-00000650: 2a88 04d5 081a 7210 0000 0072 0900 0000  *.....r....r....
-00000660: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
-00000670: 0003 0000 00f3 2200 0000 9700 7c00 6a01  ......".....|.j.
-00000680: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000690: 0000 ab00 0000 0000 0000 5300 2901 7a39  ..........S.).z9
-000006a0: 0a20 2020 2020 2020 2043 7265 6174 6520  .        Create 
-000006b0: 616e 2069 6e73 7461 6e63 6520 6f66 2074  an instance of t
-000006c0: 6865 2073 6572 7669 6365 2063 6c61 7373  he service class
-000006d0: 0a20 2020 2020 2020 2072 1d00 0000 720c  .        r....r.
-000006e0: 0000 0073 0100 0000 2072 0e00 0000 720f  ...s.... r....r.
-000006f0: 0000 007a 3a44 6566 6175 6c74 5365 7276  ...z:DefaultServ
-00000700: 6963 6549 6e73 7461 6e63 6550 726f 7669  iceInstanceProvi
-00000710: 6465 7249 6d70 6c2e 6372 6561 7465 5f73  derImpl.create_s
-00000720: 6572 7669 6365 5f69 6e73 7461 6e63 6523  ervice_instance#
-00000730: 0000 0073 1300 0000 8000 f008 0010 14d7  ...s............
-00000740: 0f21 d10f 21d3 0f23 d008 2372 1000 0000  .!..!..#..#r....
-00000750: 4e29 0872 1100 0000 7212 0000 0072 1300  N).r....r....r..
-00000760: 0000 7215 0000 00da 0474 7970 6572 1e00  ..r......typer..
-00000770: 0000 7205 0000 0072 0f00 0000 720b 0000  ..r....r....r...
-00000780: 0072 1000 0000 720e 0000 0072 1a00 0000  .r....r....r....
-00000790: 721a 0000 001a 0000 0073 1f00 0000 8400  r........s......
-000007a0: f102 0305 08f0 0a01 052b a064 f300 0105  .........+.d....
-000007b0: 2bf0 0604 0524 a818 f400 0405 2472 1000  +....$......$r..
-000007c0: 0000 721a 0000 004e 2908 7215 0000 00da  ..r....N).r.....
-000007d0: 0361 6263 7203 0000 0072 0400 0000 da1f  .abcr....r......
-000007e0: 7370 6879 726e 612e 7365 7276 6963 655f  sphyrna.service_
-000007f0: 6d61 6e61 6765 722e 7365 7276 6963 6572  manager.servicer
-00000800: 0500 0000 7208 0000 0072 1a00 0000 720b  ....r....r....r.
-00000810: 0000 0072 1000 0000 720e 0000 00fa 083c  ...r....r......<
-00000820: 6d6f 6475 6c65 3e72 2300 0000 0100 0000  module>r#.......
-00000830: 7329 0000 00f0 0301 0101 f102 0301 04f7  s)..............
-00000840: 0a00 0124 e500 34f7 0809 010c f41c 0d01  ...$..4.........
-00000850: 24d0 2940 c018 d129 4af5 000d 0124 7210  $.)@...)J....$r.
-00000860: 0000 00                                  ...
+000002c0: 7669 6365 2f74 6172 6765 742f 6368 6563  vice/target/chec
+000002d0: 6b6f 7574 2f70 6163 6b61 6765 732f 7079  kout/packages/py
+000002e0: 7468 6f6e 6c69 622f 7372 632f 6d61 696e  thonlib/src/main
+000002f0: 2f70 7974 686f 6e2f 7370 6879 726e 612f  /python/sphyrna/
+00000300: 7365 7276 6963 655f 6d61 6e61 6765 722f  service_manager/
+00000310: 7365 7276 6963 655f 696e 7374 616e 6365  service_instance
+00000320: 5f70 726f 7669 6465 722e 7079 da17 6372  _provider.py..cr
+00000330: 6561 7465 5f73 6572 7669 6365 5f69 6e73  eate_service_ins
+00000340: 7461 6e63 657a 2f53 6572 7669 6365 496e  tancez/ServiceIn
+00000350: 7374 616e 6365 5072 6f76 6964 6572 2e63  stanceProvider.c
+00000360: 7265 6174 655f 7365 7276 6963 655f 696e  reate_service_in
+00000370: 7374 616e 6365 1100 0000 7302 0000 0081  stance....s.....
+00000380: 00f3 0000 0000 4e29 07da 085f 5f6e 616d  ......N)...__nam
+00000390: 655f 5fda 0a5f 5f6d 6f64 756c 655f 5fda  e__..__module__.
+000003a0: 0c5f 5f71 7561 6c6e 616d 655f 5fda 0f5f  .__qualname__.._
+000003b0: 5f74 7970 655f 7061 7261 6d73 5f5f da07  _type_params__..
+000003c0: 5f5f 646f 635f 5f72 0400 0000 720f 0000  __doc__r....r...
+000003d0: 0029 02da 0c2e 7479 7065 5f70 6172 616d  .)....type_param
+000003e0: 7372 0500 0000 7302 0000 0080 8072 0e00  sr....s......r..
+000003f0: 0000 7208 0000 0072 0800 0000 0c00 0000  ..r....r........
+00000400: 7323 0000 00f8 8700 f102 0205 08f0 0800  s#..............
+00000410: 0614 f002 0305 0ca9 18f2 0003 050c f303  ................
+00000420: 0006 14f1 0203 050c 7210 0000 0072 0800  ........r....r..
+00000430: 0000 2901 7203 0000 0029 03da 0d2e 6765  ..).r....)....ge
+00000440: 6e65 7269 635f 6261 7365 7216 0000 0072  neric_baser....r
+00000450: 0500 0000 7303 0000 0020 4040 720e 0000  ....s.... @@r...
+00000460: 00fa 2f3c 6765 6e65 7269 6320 7061 7261  ../<generic para
+00000470: 6d65 7465 7273 206f 6620 5365 7276 6963  meters of Servic
+00000480: 6549 6e73 7461 6e63 6550 726f 7669 6465  eInstanceProvide
+00000490: 723e 7218 0000 000c 0000 0073 1600 0000  r>r........s....
+000004a0: f980 009c 68f7 0009 010c f300 0901 0cac  ....h...........
+000004b0: 03f5 0009 010c 7210 0000 0063 0000 0000  ......r....c....
+000004c0: 0000 0000 0000 0000 0200 0000 0000 0000  ................
+000004d0: f328 0000 0097 0065 005a 0164 005a 0264  .(.....e.Z.d.Z.d
+000004e0: 015a 0364 0265 0466 0264 0384 045a 0564  .Z.d.e.f.d...Z.d
+000004f0: 0465 0666 0264 0584 045a 0779 0629 07da  .e.f.d...Z.y.)..
+00000500: 2244 6566 6175 6c74 5365 7276 6963 6549  "DefaultServiceI
+00000510: 6e73 7461 6e63 6550 726f 7669 6465 7249  nstanceProviderI
+00000520: 6d70 6c7a 9a0a 2020 2020 4465 6661 756c  mplz..    Defaul
+00000530: 7453 6572 7669 6365 496e 7374 616e 6365  tServiceInstance
+00000540: 5072 6f76 6964 6572 496d 706c 2069 7320  ProviderImpl is 
+00000550: 6120 7365 7276 6963 6520 7072 6f76 6964  a service provid
+00000560: 6572 2074 6861 7420 7369 6d70 6c79 2069  er that simply i
+00000570: 6e76 6f6b 6573 2074 6865 2070 726f 7669  nvokes the provi
+00000580: 6465 6420 7365 7276 6963 6520 636f 6e73  ded service cons
+00000590: 7472 7563 746f 7220 746f 0a20 2020 2063  tructor to.    c
+000005a0: 7265 6174 6520 7468 6520 7365 7276 6963  reate the servic
+000005b0: 6520 696e 7374 616e 6365 0a20 2020 20da  e instance.    .
+000005c0: 0d73 6572 7669 6365 5f63 6c61 7373 6302  .service_classc.
+000005d0: 0000 0000 0000 0000 0000 0002 0000 0003  ................
+000005e0: 0000 00f3 1200 0000 9700 7c01 7c00 5f00  ..........|.|._.
+000005f0: 0000 0000 0000 0000 7900 2901 4ea9 0172  ........y.).N..r
+00000600: 1b00 0000 2902 720d 0000 0072 1b00 0000  ....).r....r....
+00000610: 7302 0000 0020 2072 0e00 0000 da08 5f5f  s....  r......__
+00000620: 696e 6974 5f5f 7a2b 4465 6661 756c 7453  init__z+DefaultS
+00000630: 6572 7669 6365 496e 7374 616e 6365 5072  erviceInstancePr
+00000640: 6f76 6964 6572 496d 706c 2e5f 5f69 6e69  oviderImpl.__ini
+00000650: 745f 5f20 0000 0073 0a00 0000 8000 d81d  t__ ...s........
+00000660: 2a88 04d5 081a 7210 0000 0072 0900 0000  *.....r....r....
+00000670: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
+00000680: 0003 0000 00f3 2200 0000 9700 7c00 6a01  ......".....|.j.
+00000690: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000006a0: 0000 ab00 0000 0000 0000 5300 2901 7a39  ..........S.).z9
+000006b0: 0a20 2020 2020 2020 2043 7265 6174 6520  .        Create 
+000006c0: 616e 2069 6e73 7461 6e63 6520 6f66 2074  an instance of t
+000006d0: 6865 2073 6572 7669 6365 2063 6c61 7373  he service class
+000006e0: 0a20 2020 2020 2020 2072 1d00 0000 720c  .        r....r.
+000006f0: 0000 0073 0100 0000 2072 0e00 0000 720f  ...s.... r....r.
+00000700: 0000 007a 3a44 6566 6175 6c74 5365 7276  ...z:DefaultServ
+00000710: 6963 6549 6e73 7461 6e63 6550 726f 7669  iceInstanceProvi
+00000720: 6465 7249 6d70 6c2e 6372 6561 7465 5f73  derImpl.create_s
+00000730: 6572 7669 6365 5f69 6e73 7461 6e63 6523  ervice_instance#
+00000740: 0000 0073 1300 0000 8000 f008 0010 14d7  ...s............
+00000750: 0f21 d10f 21d3 0f23 d008 2372 1000 0000  .!..!..#..#r....
+00000760: 4e29 0872 1100 0000 7212 0000 0072 1300  N).r....r....r..
+00000770: 0000 7215 0000 00da 0474 7970 6572 1e00  ..r......typer..
+00000780: 0000 7205 0000 0072 0f00 0000 720b 0000  ..r....r....r...
+00000790: 0072 1000 0000 720e 0000 0072 1a00 0000  .r....r....r....
+000007a0: 721a 0000 001a 0000 0073 1f00 0000 8400  r........s......
+000007b0: f102 0305 08f0 0a01 052b a064 f300 0105  .........+.d....
+000007c0: 2bf0 0604 0524 a818 f400 0405 2472 1000  +....$......$r..
+000007d0: 0000 721a 0000 004e 2908 7215 0000 00da  ..r....N).r.....
+000007e0: 0361 6263 7203 0000 0072 0400 0000 da1f  .abcr....r......
+000007f0: 7370 6879 726e 612e 7365 7276 6963 655f  sphyrna.service_
+00000800: 6d61 6e61 6765 722e 7365 7276 6963 6572  manager.servicer
+00000810: 0500 0000 7208 0000 0072 1a00 0000 720b  ....r....r....r.
+00000820: 0000 0072 1000 0000 720e 0000 00fa 083c  ...r....r......<
+00000830: 6d6f 6475 6c65 3e72 2300 0000 0100 0000  module>r#.......
+00000840: 7329 0000 00f0 0301 0101 f102 0301 04f7  s)..............
+00000850: 0a00 0124 e500 34f7 0809 010c f41c 0d01  ...$..4.........
+00000860: 24d0 2940 c018 d129 4af5 000d 0124 7210  $.)@...)J....$r.
+00000870: 0000 00                                  ...
```

### Comparing `sphyrna_service_manager-0.3.0/src/main/python/sphyrna/service_manager/__pycache__/service_lifecycle_controller.cpython-312.pyc` & `sphyrna_service_manager-0.3.7/src/main/python/sphyrna/service_manager/__pycache__/service_lifecycle_controller.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Mon Apr 15 00:45:11 2024 UTC, .py size: 3887 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 9778 1c66 2f0f 0000  .........x.f/...
+00000000: cb0d 0d0a 0000 0000 db6d 4066 2f0f 0000  .........m@f/...
 00000010: e300 0000 0000 0000 0000 0000 0004 0000  ................
 00000020: 0000 0000 00f3 9000 0000 9700 6400 5a00  ............d.Z.
 00000030: 6401 6402 6c01 6d02 5a02 6d03 5a03 0100  d.d.l.m.Z.m.Z...
 00000040: 6401 6403 6c04 6d05 5a05 0100 6401 6404  d.d.l.m.Z...d.d.
 00000050: 6c06 6d07 5a07 0100 6401 6405 6c08 6d09  l.m.Z...d.d.l.m.
 00000060: 5a09 6d0a 5a0a 6d0b 5a0b 0100 6401 6406  Z.m.Z.m.Z...d.d.
 00000070: 6c0c 6d0d 5a0d 0100 6401 6407 6c0e 6d0f  l.m.Z...d.d.l.m.
@@ -75,256 +75,257 @@
 000004a0: 2073 6572 7669 6365 0a20 2020 2020 2020   service.       
 000004b0: 2020 2020 2020 2020 636c 6173 730a 2020          class.  
 000004c0: 2020 2020 2020 4070 6172 616d 2063 6f6e        @param con
 000004d0: 6669 6720 7365 7276 6963 6520 6c65 7665  fig service leve
 000004e0: 6c20 636f 6e66 6967 7572 6174 696f 6e0a  l configuration.
 000004f0: 2020 2020 2020 2020 4ea9 00a9 03da 0473          N......s
 00000500: 656c 6672 0f00 0000 7210 0000 0073 0300  elfr....r....s..
-00000510: 0000 2020 20fa 772f 5573 6572 732f 6b61  ..   .w/Users/ka
+00000510: 0000 2020 20fa 872f 5573 6572 732f 6b61  ..   ../Users/ka
 00000520: 6d65 6c65 6f6e 2f43 6f64 652f 7365 7276  meleon/Code/serv
-00000530: 6963 652f 7061 636b 6167 6573 2f70 7974  ice/packages/pyt
-00000540: 686f 6e6c 6962 2f73 7263 2f6d 6169 6e2f  honlib/src/main/
-00000550: 7079 7468 6f6e 2f73 7068 7972 6e61 2f73  python/sphyrna/s
-00000560: 6572 7669 6365 5f6d 616e 6167 6572 2f73  ervice_manager/s
-00000570: 6572 7669 6365 5f6c 6966 6563 7963 6c65  ervice_lifecycle
-00000580: 5f63 6f6e 7472 6f6c 6c65 722e 7079 da04  _controller.py..
-00000590: 696e 6974 7a1f 5365 7276 6963 654c 6966  initz.ServiceLif
-000005a0: 6563 7963 6c65 436f 6e74 726f 6c6c 6572  ecycleController
-000005b0: 2e69 6e69 7416 0000 00f3 0200 0000 8100  .init...........
-000005c0: f300 0000 0063 0100 0000 0000 0000 0000  .....c..........
-000005d0: 0000 0000 0000 1300 0000 f304 0000 0097  ................
-000005e0: 0079 0129 027a 3d0a 2020 2020 2020 2020  .y.).z=.        
-000005f0: 5368 7574 646f 776e 2074 6865 2073 6572  Shutdown the ser
-00000600: 7669 6365 206c 6966 6563 7963 6c65 2061  vice lifecycle a
-00000610: 6e64 2063 6c65 616e 2075 700a 2020 2020  nd clean up.    
-00000620: 2020 2020 4e72 1300 0000 a901 7215 0000      Nr......r...
-00000630: 0073 0100 0000 2072 1600 0000 da08 7368  .s.... r......sh
-00000640: 7574 646f 776e 7a23 5365 7276 6963 654c  utdownz#ServiceL
-00000650: 6966 6563 7963 6c65 436f 6e74 726f 6c6c  ifecycleControll
-00000660: 6572 2e73 6875 7464 6f77 6e23 0000 0072  er.shutdown#...r
-00000670: 1800 0000 7219 0000 0063 0100 0000 0000  ....r....c......
-00000680: 0000 0000 0000 0000 0000 1300 0000 f304  ................
-00000690: 0000 0097 0079 0129 027a 510a 2020 2020  .....y.).zQ.    
-000006a0: 2020 2020 5265 7472 6965 7665 2061 2073      Retrieve a s
-000006b0: 6572 7669 6365 2069 6e73 7461 6e63 650a  ervice instance.
-000006c0: 0a20 2020 2020 2020 2040 7265 7475 726e  .        @return
-000006d0: 2061 2073 6572 7669 6365 2069 6e73 7461   a service insta
-000006e0: 6e63 650a 2020 2020 2020 2020 4e72 1300  nce.        Nr..
-000006f0: 0000 721b 0000 0073 0100 0000 2072 1600  ..r....s.... r..
-00000700: 0000 da0b 6765 745f 7365 7276 6963 657a  ....get_servicez
-00000710: 2653 6572 7669 6365 4c69 6665 6379 636c  &ServiceLifecycl
-00000720: 6543 6f6e 7472 6f6c 6c65 722e 6765 745f  eController.get_
-00000730: 7365 7276 6963 6528 0000 0072 1800 0000  service(...r....
-00000740: 7219 0000 00a9 0272 1100 0000 4e29 0ada  r......r....N)..
-00000750: 085f 5f6e 616d 655f 5fda 0a5f 5f6d 6f64  .__name__..__mod
-00000760: 756c 655f 5fda 0c5f 5f71 7561 6c6e 616d  ule__..__qualnam
-00000770: 655f 5fda 0f5f 5f74 7970 655f 7061 7261  e__..__type_para
-00000780: 6d73 5f5f da07 5f5f 646f 635f 5f72 0400  ms__..__doc__r..
-00000790: 0000 720a 0000 0072 1700 0000 721c 0000  ..r....r....r...
-000007a0: 0072 1e00 0000 a903 da0c 2e74 7970 655f  .r.........type_
-000007b0: 7061 7261 6d73 7209 0000 0072 0800 0000  paramsr....r....
-000007c0: 7303 0000 0080 8080 7216 0000 0072 0e00  s.......r....r..
-000007d0: 0000 720e 0000 000f 0000 0073 5d00 0000  ..r........s]...
-000007e0: f887 00f1 0204 0508 f00c 0006 14f0 020a  ................
-000007f0: 050c e023 3ab9 38d1 2344 f005 0a05 0cf1  ...#:.8.#D......
-00000800: 0600 111f f007 0a05 0cf0 0800 0a0e f209  ................
-00000810: 0a05 0cf3 0300 0614 f002 0a05 0cf3 1803  ................
-00000820: 050c f00a 0006 14f0 0205 050c 9958 f200  .............X..
-00000830: 0505 0cf3 0300 0614 f102 0505 0c72 1900  .............r..
-00000840: 0000 720e 0000 0029 0172 0300 0000 a904  ..r....).r......
-00000850: da0d 2e67 656e 6572 6963 5f62 6173 6572  ...generic_baser
-00000860: 2600 0000 7209 0000 0072 0800 0000 7304  &...r....r....s.
-00000870: 0000 0020 4040 4072 1600 0000 fa32 3c67  ... @@@r.....2<g
-00000880: 656e 6572 6963 2070 6172 616d 6574 6572  eneric parameter
-00000890: 7320 6f66 2053 6572 7669 6365 4c69 6665  s of ServiceLife
-000008a0: 6379 636c 6543 6f6e 7472 6f6c 6c65 723e  cycleController>
-000008b0: 7229 0000 000f 0000 0073 1a00 0000 fa80  r).......s......
-000008c0: 00a3 18ab 3ea0 18f7 001f 010c f400 1f01  ....>...........
-000008d0: 0cbc 33f5 001f 010c 7219 0000 0063 0000  ..3.....r....c..
-000008e0: 0000 0000 0000 0000 0000 0700 0000 0300  ................
-000008f0: 0000 f354 0000 0087 0187 0287 0397 0064  ...T...........d
-00000900: 00ad 0778 018a 0364 01ad 0778 018a 0266  ...x...d...x...f
-00000910: 028a 0102 0047 0088 0188 0288 0366 0364  .....G.......f.d
-00000920: 0284 0864 0389 01ad 0a7d 0074 0000 0000  ...d.....}.t....
-00000930: 0000 0000 0089 0389 0266 0219 0000 007c  .........f.....|
-00000940: 00ab 0400 0000 0000 0053 0029 0472 0800  .........S.).r..
-00000950: 0000 7209 0000 0063 0000 0000 0000 0000  ..r....c........
-00000960: 0000 0000 0700 0000 0000 0000 f370 0000  .............p..
-00000970: 0095 0397 0065 005a 0164 005a 0257 00b0  .....e.Z.d.Z.W..
-00000980: 005a 0364 015a 0464 0284 005a 0565 0664  .Z.d.Z.d...Z.e.d
-00000990: 0365 0757 00b0 0219 0000 0064 0457 00b0  .e.W.......d.W..
-000009a0: 0164 0564 0666 0664 0784 04ab 0000 0000  .d.d.f.d........
-000009b0: 0000 005a 0865 0664 0557 00b0 0266 0264  ...Z.e.d.W...f.d
-000009c0: 0884 04ab 0000 0000 0000 005a 0965 0664  ...........Z.e.d
-000009d0: 0a64 0984 04ab 0000 0000 0000 005a 0a79  .d...........Z.y
-000009e0: 0629 0bda 2753 696e 676c 6574 6f6e 5365  .)..'SingletonSe
-000009f0: 7276 6963 654c 6966 6563 7963 6c65 436f  rviceLifecycleCo
-00000a00: 6e74 726f 6c6c 6572 496d 706c 7a36 0a20  ntrollerImplz6. 
-00000a10: 2020 204c 6966 6563 7963 6c65 2063 6f6e     Lifecycle con
-00000a20: 7472 6f6c 6c65 7220 7468 6174 2063 7265  troller that cre
-00000a30: 6174 6573 2073 696e 676c 6574 6f6e 730a  ates singletons.
-00000a40: 2020 2020 6301 0000 0000 0000 0000 0000      c...........
-00000a50: 0002 0000 0013 0000 00f3 3600 0000 9700  ..........6.....
-00000a60: 6400 7c00 5f00 0000 0000 0000 0000 7402  d.|._.........t.
-00000a70: 0000 0000 0000 0000 7c00 5f02 0000 0000  ........|._.....
-00000a80: 0000 0000 6400 7c00 5f03 0000 0000 0000  ....d.|._.......
-00000a90: 0000 7900 a901 4e29 04da 1a5f 7365 7276  ..y...N)..._serv
-00000aa0: 6963 655f 696e 7374 616e 6365 5f70 726f  ice_instance_pro
-00000ab0: 7669 6465 7272 0b00 0000 da07 5f63 6f6e  viderr......_con
-00000ac0: 6669 67da 135f 7369 6e67 6c65 746f 6e5f  fig.._singleton_
-00000ad0: 696e 7374 616e 6365 721b 0000 0073 0100  instancer....s..
-00000ae0: 0000 2072 1600 0000 da08 5f5f 696e 6974  .. r......__init
-00000af0: 5f5f 7a30 5369 6e67 6c65 746f 6e53 6572  __z0SingletonSer
-00000b00: 7669 6365 4c69 6665 6379 636c 6543 6f6e  viceLifecycleCon
-00000b10: 7472 6f6c 6c65 7249 6d70 6c2e 5f5f 696e  trollerImpl.__in
-00000b20: 6974 5f5f 3b00 0000 7319 0000 0080 00d8  it__;...s.......
-00000b30: 2a2e 8804 d408 27dc 1732 8804 8c0c d823  *.....'..2.....#
-00000b40: 2788 04d5 0820 7219 0000 0072 0f00 0000  '.... r....r....
-00000b50: 7210 0000 0072 1100 0000 4e63 0300 0000  r....r....Nc....
-00000b60: 0000 0000 0000 0000 0200 0000 1300 0000  ................
-00000b70: f320 0000 0097 007c 017c 005f 0000 0000  . .....|.|._....
-00000b80: 0000 0000 007c 027c 005f 0100 0000 0000  .....|.|._......
-00000b90: 0000 0079 0072 2e00 0000 2902 722f 0000  ...y.r....).r/..
-00000ba0: 0072 3000 0000 7214 0000 0073 0300 0000  .r0...r....s....
-00000bb0: 2020 2072 1600 0000 7217 0000 007a 2c53     r....r....z,S
-00000bc0: 696e 676c 6574 6f6e 5365 7276 6963 654c  ingletonServiceL
-00000bd0: 6966 6563 7963 6c65 436f 6e74 726f 6c6c  ifecycleControll
-00000be0: 6572 496d 706c 2e69 6e69 7440 0000 0073  erImpl.init@...s
-00000bf0: 1400 0000 8000 f012 002b 4401 8804 d408  .........+D.....
-00000c00: 27d8 171d 8804 8d0c 7219 0000 0063 0100  '.......r....c..
-00000c10: 0000 0000 0000 0000 0000 0400 0000 1300  ................
-00000c20: 0000 f34c 0100 0097 0074 0100 0000 0000  ...L.....t......
-00000c30: 0000 007c 0064 01ab 0200 0000 0000 0072  ...|.d.........r
-00000c40: 0c7c 006a 0200 0000 0000 0000 0000 0000  .|.j............
-00000c50: 0000 0000 0000 0080 8174 0100 0000 0000  .........t......
-00000c60: 0000 007c 0064 02ab 0200 0000 0000 0072  ...|.d.........r
-00000c70: 0c7c 006a 0400 0000 0000 0000 0000 0000  .|.j............
-00000c80: 0000 0000 0000 0080 0b74 0700 0000 0000  .........t......
-00000c90: 0000 0064 03ab 0100 0000 0000 0082 017c  ...d...........|
-00000ca0: 006a 0400 0000 0000 0000 0000 0000 0000  .j..............
-00000cb0: 0000 0000 006a 0900 0000 0000 0000 0000  .....j..........
-00000cc0: 0000 0000 0000 0000 00ab 0000 0000 0000  ................
-00000cd0: 007c 005f 0100 0000 0000 0000 007c 006a  .|._.........|.j
-00000ce0: 0200 0000 0000 0000 0000 0000 0000 0000  ................
-00000cf0: 0000 006a 0b00 0000 0000 0000 0000 0000  ...j............
-00000d00: 0000 0000 0000 007c 006a 0c00 0000 0000  .......|.j......
-00000d10: 0000 0000 0000 0000 0000 0000 00ab 0100  ................
-00000d20: 0000 0000 0001 007c 006a 0200 0000 0000  .......|.j......
-00000d30: 0000 0000 0000 0000 0000 0000 006a 0f00  .............j..
-00000d40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000d50: 00ab 0000 0000 0000 0001 007c 006a 0200  ...........|.j..
-00000d60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000d70: 0053 0029 044e 7231 0000 0072 2f00 0000  .S.).Nr1...r/...
-00000d80: 7a31 556e 6578 7065 6374 6564 2073 7461  z1Unexpected sta
-00000d90: 7465 2e20 5365 7276 6963 6549 6e73 7461  te. ServiceInsta
-00000da0: 6e63 6550 726f 7669 6465 7220 6e6f 7420  nceProvider not 
-00000db0: 7365 7429 08da 0768 6173 6174 7472 7231  set)...hasattrr1
-00000dc0: 0000 0072 2f00 0000 7207 0000 00da 1763  ...r/...r......c
-00000dd0: 7265 6174 655f 7365 7276 6963 655f 696e  reate_service_in
-00000de0: 7374 616e 6365 7217 0000 0072 3000 0000  stancer....r0...
-00000df0: da05 7374 6172 7472 1b00 0000 7301 0000  ..startr....s...
-00000e00: 0020 7216 0000 0072 1e00 0000 7a33 5369  . r....r....z3Si
-00000e10: 6e67 6c65 746f 6e53 6572 7669 6365 4c69  ngletonServiceLi
-00000e20: 6665 6379 636c 6543 6f6e 7472 6f6c 6c65  fecycleControlle
-00000e30: 7249 6d70 6c2e 6765 745f 7365 7276 6963  rImpl.get_servic
-00000e40: 654c 0000 0073 9600 0000 8000 f40a 0011  eL...s..........
-00000e50: 1898 04d0 1e33 d410 34d8 0c10 d70c 24d1  .....3..4.....$.
-00000e60: 0c24 d00c 2ce4 141b 9844 d022 3ed4 143f  .$..,....D.">..?
-00000e70: d810 14d7 102f d110 2fd0 1037 e416 26d8  ...../../..7..&.
-00000e80: 1447 f303 0217 12f0 0002 1112 f00a 0011  .G..............
-00000e90: 15d7 102f d110 2fd7 1047 d110 47d3 1049  .../../..G..G..I
-00000ea0: f003 000d 11d4 0c24 f006 000d 11d7 0c24  .......$.......$
-00000eb0: d10c 24d7 0c29 d10c 29a8 24af 2ca9 2cd4  ..$..)..).$.,.,.
-00000ec0: 0c37 d80c 10d7 0c24 d10c 24d7 0c2a d10c  .7.....$..$..*..
-00000ed0: 2ad4 0c2c e00f 13d7 0f27 d10f 27d0 0827  *..,.....'..'..'
-00000ee0: 7219 0000 0063 0100 0000 0000 0000 0000  r....c..........
-00000ef0: 0000 0400 0000 1300 0000 f3ce 0000 0097  ................
-00000f00: 0074 0100 0000 0000 0000 007c 0064 01ab  .t.........|.d..
-00000f10: 0200 0000 0000 0072 477c 006a 0200 0000  .......rG|.j....
-00000f20: 0000 0000 0000 0000 0000 0000 0000 0081  ................
-00000f30: 3b7c 006a 0200 0000 0000 0000 0000 0000  ;|.j............
-00000f40: 0000 0000 0000 006a 0500 0000 0000 0000  .......j........
-00000f50: 0000 0000 0000 0000 0000 00ab 0000 0000  ................
-00000f60: 0000 0001 007c 006a 0200 0000 0000 0000  .....|.j........
-00000f70: 0000 0000 0000 0000 0000 006a 0700 0000  ...........j....
-00000f80: 0000 0000 0000 0000 0000 0000 0000 00ab  ................
-00000f90: 0000 0000 0000 0001 0064 007c 005f 0100  .........d.|._..
-00000fa0: 0000 0000 0000 0074 0800 0000 0000 0000  .......t........
-00000fb0: 007c 005f 0500 0000 0000 0000 0064 007c  .|._.........d.|
-00000fc0: 005f 0600 0000 0000 0000 0079 0029 024e  ._.........y.).N
-00000fd0: 7231 0000 0029 0772 3500 0000 7231 0000  r1...).r5...r1..
-00000fe0: 00da 0473 746f 70da 0764 6573 7472 6f79  ...stop..destroy
-00000ff0: 720b 0000 0072 3000 0000 722f 0000 0072  r....r0...r/...r
-00001000: 1b00 0000 7301 0000 0020 7216 0000 0072  ....s.... r....r
-00001010: 1c00 0000 7a30 5369 6e67 6c65 746f 6e53  ....z0SingletonS
-00001020: 6572 7669 6365 4c69 6665 6379 636c 6543  erviceLifecycleC
-00001030: 6f6e 7472 6f6c 6c65 7249 6d70 6c2e 7368  ontrollerImpl.sh
-00001040: 7574 646f 776e 6300 0000 7356 0000 0080  utdownc...sV....
-00001050: 00f4 0a00 0c13 9034 d019 2ed4 0b2f d80c  .......4...../..
-00001060: 10d7 0c24 d10c 24d0 0c30 e00c 10d7 0c24  ...$..$..0.....$
-00001070: d10c 24d7 0c29 d10c 29d4 0c2b d80c 10d7  ..$..)..)..+....
-00001080: 0c24 d10c 24d7 0c2c d10c 2cd4 0c2e d827  .$..$..,..,....'
-00001090: 2b88 44d4 0c24 e417 3288 048c 0cd8 2a2e  +.D..$..2.....*.
-000010a0: 8804 d508 2772 1900 0000 721f 0000 0029  ....'r....r....)
-000010b0: 0b72 2000 0000 7221 0000 0072 2200 0000  .r ...r!...r"...
-000010c0: 7223 0000 0072 2400 0000 7232 0000 0072  r#...r$...r2...r
-000010d0: 0600 0000 720a 0000 0072 1700 0000 721e  ....r....r....r.
-000010e0: 0000 0072 1c00 0000 7225 0000 0073 0300  ...r....r%...s..
-000010f0: 0000 8080 8072 1600 0000 722c 0000 0072  .....r....r,...r
-00001100: 2c00 0000 3400 0000 7371 0000 00f8 8700  ,...4...sq......
-00001110: f106 0205 08f2 0803 0528 f00a 0006 0ef0  .........(......
-00001120: 0209 051e e023 3ab9 38d1 2344 f005 0905  .....#:.8.#D....
-00001130: 1ef1 0600 111f f007 0905 1ef0 0800 0a0e  ................
-00001140: f209 0905 1ef3 0300 060e f002 0905 1ef0  ................
-00001150: 1600 060e f002 1405 2899 58f2 0014 0528  ........(.X....(
-00001160: f303 0006 0ef0 0214 0528 f02c 0006 0ef2  .........(.,....
-00001170: 020c 052f f303 0006 0ef1 020c 052f 7219  .../........./r.
-00001180: 0000 0072 2c00 0000 2901 720e 0000 0072  ...r,...).r....r
-00001190: 2700 0000 7304 0000 0020 4040 4072 1600  '...s.... @@@r..
-000011a0: 0000 fa3f 3c67 656e 6572 6963 2070 6172  ...?<generic par
-000011b0: 616d 6574 6572 7320 6f66 2053 696e 676c  ameters of Singl
-000011c0: 6574 6f6e 5365 7276 6963 654c 6966 6563  etonServiceLifec
-000011d0: 7963 6c65 436f 6e74 726f 6c6c 6572 496d  ycleControllerIm
-000011e0: 706c 3e72 3b00 0000 3400 0000 7325 0000  pl>r;...4...s%..
-000011f0: 00fa 8000 ab68 bb0e a868 f700 3c01 2ff4  .....h...h..<./.
-00001200: 003c 012f dc04 1e98 78a8 1ed0 1f37 d104  .<./....x....7..
-00001210: 38f5 033c 012f 7219 0000 0063 0000 0000  8..<./r....c....
-00001220: 0000 0000 0000 0000 0300 0000 0000 0000  ................
-00001230: f326 0000 0097 0065 005a 0164 005a 0255  .&.....e.Z.d.Z.U
-00001240: 0064 015a 0365 045a 0565 0665 0719 0000  .d.Z.e.Z.e.e....
-00001250: 0065 0864 023c 0000 0079 0329 04da 204b  .e.d.<...y.).. K
-00001260: 6e6f 776e 5365 7276 6963 654c 6966 6563  nownServiceLifec
-00001270: 7963 6c65 436f 6e74 726f 6c6c 6572 737a  ycleControllersz
-00001280: 3b0a 2020 2020 4b6e 6f77 6e20 5365 7276  ;.    Known Serv
-00001290: 6963 654c 6966 6563 7963 6c65 436f 6e74  iceLifecycleCont
-000012a0: 726f 6c6c 6572 2069 6d70 6c65 6d65 6e74  roller implement
-000012b0: 6174 696f 6e73 2e0a 2020 2020 da09 5349  ations..    ..SI
-000012c0: 4e47 4c45 544f 4e4e 2909 7220 0000 0072  NGLETONN).r ...r
-000012d0: 2100 0000 7222 0000 0072 2400 0000 722c  !...r"...r$...r,
-000012e0: 0000 0072 3e00 0000 7205 0000 00da 0474  ...r>...r......t
-000012f0: 7970 65da 0f5f 5f61 6e6e 6f74 6174 696f  ype..__annotatio
-00001300: 6e73 5f5f 7213 0000 0072 1900 0000 7216  ns__r....r....r.
-00001310: 0000 0072 3d00 0000 723d 0000 0073 0000  ...r=...r=...s..
-00001320: 0073 1800 0000 8500 f102 0205 08f0 0800  .s..............
-00001330: 1e45 0180 4988 7590 5489 7bd4 0444 7219  .E..I.u.T.{..Dr.
-00001340: 0000 0072 3d00 0000 4e29 1372 2400 0000  ...r=...N).r$...
-00001350: da03 6162 6372 0300 0000 7204 0000 00da  ..abcr....r.....
-00001360: 0674 7970 696e 6772 0500 0000 da11 7479  .typingr......ty
-00001370: 7069 6e67 5f65 7874 656e 7369 6f6e 7372  ping_extensionsr
-00001380: 0600 0000 da1f 7370 6879 726e 612e 7365  ......sphyrna.se
-00001390: 7276 6963 655f 6d61 6e61 6765 722e 7365  rvice_manager.se
-000013a0: 7276 6963 6572 0700 0000 7208 0000 0072  rvicer....r....r
-000013b0: 0900 0000 da31 7370 6879 726e 612e 7365  .....1sphyrna.se
-000013c0: 7276 6963 655f 6d61 6e61 6765 722e 7365  rvice_manager.se
-000013d0: 7276 6963 655f 696e 7374 616e 6365 5f70  rvice_instance_p
-000013e0: 726f 7669 6465 7272 0a00 0000 da2d 7370  roviderr.....-sp
-000013f0: 6879 726e 612e 7365 7276 6963 655f 6d61  hyrna.service_ma
-00001400: 6e61 6765 722e 7365 7276 6963 655f 636f  nager.service_co
-00001410: 6e66 6967 7572 6174 696f 6e72 0b00 0000  nfigurationr....
-00001420: 720e 0000 0072 2c00 0000 723d 0000 0072  r....r,...r=...r
-00001430: 1300 0000 7219 0000 0072 1600 0000 fa08  ....r....r......
-00001440: 3c6d 6f64 756c 653e 7247 0000 0001 0000  <module>rG......
-00001450: 0073 3900 0000 f003 0101 01f1 0203 0104  .s9.............
-00001460: f70a 0001 24dd 0018 dd00 26df 0056 d100  ....$.....&..V..
-00001470: 56dd 0055 dd00 55f7 081f 010c f74a 013c  V..U..U......J.<
-00001480: 012f f77e 0105 0145 01f2 0005 0145 0172  ./.~...E.....E.r
-00001490: 1900 0000                                ....
+00000530: 6963 652f 7461 7267 6574 2f63 6865 636b  ice/target/check
+00000540: 6f75 742f 7061 636b 6167 6573 2f70 7974  out/packages/pyt
+00000550: 686f 6e6c 6962 2f73 7263 2f6d 6169 6e2f  honlib/src/main/
+00000560: 7079 7468 6f6e 2f73 7068 7972 6e61 2f73  python/sphyrna/s
+00000570: 6572 7669 6365 5f6d 616e 6167 6572 2f73  ervice_manager/s
+00000580: 6572 7669 6365 5f6c 6966 6563 7963 6c65  ervice_lifecycle
+00000590: 5f63 6f6e 7472 6f6c 6c65 722e 7079 da04  _controller.py..
+000005a0: 696e 6974 7a1f 5365 7276 6963 654c 6966  initz.ServiceLif
+000005b0: 6563 7963 6c65 436f 6e74 726f 6c6c 6572  ecycleController
+000005c0: 2e69 6e69 7416 0000 00f3 0200 0000 8100  .init...........
+000005d0: f300 0000 0063 0100 0000 0000 0000 0000  .....c..........
+000005e0: 0000 0000 0000 1300 0000 f304 0000 0097  ................
+000005f0: 0079 0129 027a 3d0a 2020 2020 2020 2020  .y.).z=.        
+00000600: 5368 7574 646f 776e 2074 6865 2073 6572  Shutdown the ser
+00000610: 7669 6365 206c 6966 6563 7963 6c65 2061  vice lifecycle a
+00000620: 6e64 2063 6c65 616e 2075 700a 2020 2020  nd clean up.    
+00000630: 2020 2020 4e72 1300 0000 a901 7215 0000      Nr......r...
+00000640: 0073 0100 0000 2072 1600 0000 da08 7368  .s.... r......sh
+00000650: 7574 646f 776e 7a23 5365 7276 6963 654c  utdownz#ServiceL
+00000660: 6966 6563 7963 6c65 436f 6e74 726f 6c6c  ifecycleControll
+00000670: 6572 2e73 6875 7464 6f77 6e23 0000 0072  er.shutdown#...r
+00000680: 1800 0000 7219 0000 0063 0100 0000 0000  ....r....c......
+00000690: 0000 0000 0000 0000 0000 1300 0000 f304  ................
+000006a0: 0000 0097 0079 0129 027a 510a 2020 2020  .....y.).zQ.    
+000006b0: 2020 2020 5265 7472 6965 7665 2061 2073      Retrieve a s
+000006c0: 6572 7669 6365 2069 6e73 7461 6e63 650a  ervice instance.
+000006d0: 0a20 2020 2020 2020 2040 7265 7475 726e  .        @return
+000006e0: 2061 2073 6572 7669 6365 2069 6e73 7461   a service insta
+000006f0: 6e63 650a 2020 2020 2020 2020 4e72 1300  nce.        Nr..
+00000700: 0000 721b 0000 0073 0100 0000 2072 1600  ..r....s.... r..
+00000710: 0000 da0b 6765 745f 7365 7276 6963 657a  ....get_servicez
+00000720: 2653 6572 7669 6365 4c69 6665 6379 636c  &ServiceLifecycl
+00000730: 6543 6f6e 7472 6f6c 6c65 722e 6765 745f  eController.get_
+00000740: 7365 7276 6963 6528 0000 0072 1800 0000  service(...r....
+00000750: 7219 0000 00a9 0272 1100 0000 4e29 0ada  r......r....N)..
+00000760: 085f 5f6e 616d 655f 5fda 0a5f 5f6d 6f64  .__name__..__mod
+00000770: 756c 655f 5fda 0c5f 5f71 7561 6c6e 616d  ule__..__qualnam
+00000780: 655f 5fda 0f5f 5f74 7970 655f 7061 7261  e__..__type_para
+00000790: 6d73 5f5f da07 5f5f 646f 635f 5f72 0400  ms__..__doc__r..
+000007a0: 0000 720a 0000 0072 1700 0000 721c 0000  ..r....r....r...
+000007b0: 0072 1e00 0000 a903 da0c 2e74 7970 655f  .r.........type_
+000007c0: 7061 7261 6d73 7209 0000 0072 0800 0000  paramsr....r....
+000007d0: 7303 0000 0080 8080 7216 0000 0072 0e00  s.......r....r..
+000007e0: 0000 720e 0000 000f 0000 0073 5d00 0000  ..r........s]...
+000007f0: f887 00f1 0204 0508 f00c 0006 14f0 020a  ................
+00000800: 050c e023 3ab9 38d1 2344 f005 0a05 0cf1  ...#:.8.#D......
+00000810: 0600 111f f007 0a05 0cf0 0800 0a0e f209  ................
+00000820: 0a05 0cf3 0300 0614 f002 0a05 0cf3 1803  ................
+00000830: 050c f00a 0006 14f0 0205 050c 9958 f200  .............X..
+00000840: 0505 0cf3 0300 0614 f102 0505 0c72 1900  .............r..
+00000850: 0000 720e 0000 0029 0172 0300 0000 a904  ..r....).r......
+00000860: da0d 2e67 656e 6572 6963 5f62 6173 6572  ...generic_baser
+00000870: 2600 0000 7209 0000 0072 0800 0000 7304  &...r....r....s.
+00000880: 0000 0020 4040 4072 1600 0000 fa32 3c67  ... @@@r.....2<g
+00000890: 656e 6572 6963 2070 6172 616d 6574 6572  eneric parameter
+000008a0: 7320 6f66 2053 6572 7669 6365 4c69 6665  s of ServiceLife
+000008b0: 6379 636c 6543 6f6e 7472 6f6c 6c65 723e  cycleController>
+000008c0: 7229 0000 000f 0000 0073 1a00 0000 fa80  r).......s......
+000008d0: 00a3 18ab 3ea0 18f7 001f 010c f400 1f01  ....>...........
+000008e0: 0cbc 33f5 001f 010c 7219 0000 0063 0000  ..3.....r....c..
+000008f0: 0000 0000 0000 0000 0000 0700 0000 0300  ................
+00000900: 0000 f354 0000 0087 0187 0287 0397 0064  ...T...........d
+00000910: 00ad 0778 018a 0364 01ad 0778 018a 0266  ...x...d...x...f
+00000920: 028a 0102 0047 0088 0188 0288 0366 0364  .....G.......f.d
+00000930: 0284 0864 0389 01ad 0a7d 0074 0000 0000  ...d.....}.t....
+00000940: 0000 0000 0089 0389 0266 0219 0000 007c  .........f.....|
+00000950: 00ab 0400 0000 0000 0053 0029 0472 0800  .........S.).r..
+00000960: 0000 7209 0000 0063 0000 0000 0000 0000  ..r....c........
+00000970: 0000 0000 0700 0000 0000 0000 f370 0000  .............p..
+00000980: 0095 0397 0065 005a 0164 005a 0257 00b0  .....e.Z.d.Z.W..
+00000990: 005a 0364 015a 0464 0284 005a 0565 0664  .Z.d.Z.d...Z.e.d
+000009a0: 0365 0757 00b0 0219 0000 0064 0457 00b0  .e.W.......d.W..
+000009b0: 0164 0564 0666 0664 0784 04ab 0000 0000  .d.d.f.d........
+000009c0: 0000 005a 0865 0664 0557 00b0 0266 0264  ...Z.e.d.W...f.d
+000009d0: 0884 04ab 0000 0000 0000 005a 0965 0664  ...........Z.e.d
+000009e0: 0a64 0984 04ab 0000 0000 0000 005a 0a79  .d...........Z.y
+000009f0: 0629 0bda 2753 696e 676c 6574 6f6e 5365  .)..'SingletonSe
+00000a00: 7276 6963 654c 6966 6563 7963 6c65 436f  rviceLifecycleCo
+00000a10: 6e74 726f 6c6c 6572 496d 706c 7a36 0a20  ntrollerImplz6. 
+00000a20: 2020 204c 6966 6563 7963 6c65 2063 6f6e     Lifecycle con
+00000a30: 7472 6f6c 6c65 7220 7468 6174 2063 7265  troller that cre
+00000a40: 6174 6573 2073 696e 676c 6574 6f6e 730a  ates singletons.
+00000a50: 2020 2020 6301 0000 0000 0000 0000 0000      c...........
+00000a60: 0002 0000 0013 0000 00f3 3600 0000 9700  ..........6.....
+00000a70: 6400 7c00 5f00 0000 0000 0000 0000 7402  d.|._.........t.
+00000a80: 0000 0000 0000 0000 7c00 5f02 0000 0000  ........|._.....
+00000a90: 0000 0000 6400 7c00 5f03 0000 0000 0000  ....d.|._.......
+00000aa0: 0000 7900 a901 4e29 04da 1a5f 7365 7276  ..y...N)..._serv
+00000ab0: 6963 655f 696e 7374 616e 6365 5f70 726f  ice_instance_pro
+00000ac0: 7669 6465 7272 0b00 0000 da07 5f63 6f6e  viderr......_con
+00000ad0: 6669 67da 135f 7369 6e67 6c65 746f 6e5f  fig.._singleton_
+00000ae0: 696e 7374 616e 6365 721b 0000 0073 0100  instancer....s..
+00000af0: 0000 2072 1600 0000 da08 5f5f 696e 6974  .. r......__init
+00000b00: 5f5f 7a30 5369 6e67 6c65 746f 6e53 6572  __z0SingletonSer
+00000b10: 7669 6365 4c69 6665 6379 636c 6543 6f6e  viceLifecycleCon
+00000b20: 7472 6f6c 6c65 7249 6d70 6c2e 5f5f 696e  trollerImpl.__in
+00000b30: 6974 5f5f 3b00 0000 7319 0000 0080 00d8  it__;...s.......
+00000b40: 2a2e 8804 d408 27dc 1732 8804 8c0c d823  *.....'..2.....#
+00000b50: 2788 04d5 0820 7219 0000 0072 0f00 0000  '.... r....r....
+00000b60: 7210 0000 0072 1100 0000 4e63 0300 0000  r....r....Nc....
+00000b70: 0000 0000 0000 0000 0200 0000 1300 0000  ................
+00000b80: f320 0000 0097 007c 017c 005f 0000 0000  . .....|.|._....
+00000b90: 0000 0000 007c 027c 005f 0100 0000 0000  .....|.|._......
+00000ba0: 0000 0079 0072 2e00 0000 2902 722f 0000  ...y.r....).r/..
+00000bb0: 0072 3000 0000 7214 0000 0073 0300 0000  .r0...r....s....
+00000bc0: 2020 2072 1600 0000 7217 0000 007a 2c53     r....r....z,S
+00000bd0: 696e 676c 6574 6f6e 5365 7276 6963 654c  ingletonServiceL
+00000be0: 6966 6563 7963 6c65 436f 6e74 726f 6c6c  ifecycleControll
+00000bf0: 6572 496d 706c 2e69 6e69 7440 0000 0073  erImpl.init@...s
+00000c00: 1400 0000 8000 f012 002b 4401 8804 d408  .........+D.....
+00000c10: 27d8 171d 8804 8d0c 7219 0000 0063 0100  '.......r....c..
+00000c20: 0000 0000 0000 0000 0000 0400 0000 1300  ................
+00000c30: 0000 f34c 0100 0097 0074 0100 0000 0000  ...L.....t......
+00000c40: 0000 007c 0064 01ab 0200 0000 0000 0072  ...|.d.........r
+00000c50: 0c7c 006a 0200 0000 0000 0000 0000 0000  .|.j............
+00000c60: 0000 0000 0000 0080 8174 0100 0000 0000  .........t......
+00000c70: 0000 007c 0064 02ab 0200 0000 0000 0072  ...|.d.........r
+00000c80: 0c7c 006a 0400 0000 0000 0000 0000 0000  .|.j............
+00000c90: 0000 0000 0000 0080 0b74 0700 0000 0000  .........t......
+00000ca0: 0000 0064 03ab 0100 0000 0000 0082 017c  ...d...........|
+00000cb0: 006a 0400 0000 0000 0000 0000 0000 0000  .j..............
+00000cc0: 0000 0000 006a 0900 0000 0000 0000 0000  .....j..........
+00000cd0: 0000 0000 0000 0000 00ab 0000 0000 0000  ................
+00000ce0: 007c 005f 0100 0000 0000 0000 007c 006a  .|._.........|.j
+00000cf0: 0200 0000 0000 0000 0000 0000 0000 0000  ................
+00000d00: 0000 006a 0b00 0000 0000 0000 0000 0000  ...j............
+00000d10: 0000 0000 0000 007c 006a 0c00 0000 0000  .......|.j......
+00000d20: 0000 0000 0000 0000 0000 0000 00ab 0100  ................
+00000d30: 0000 0000 0001 007c 006a 0200 0000 0000  .......|.j......
+00000d40: 0000 0000 0000 0000 0000 0000 006a 0f00  .............j..
+00000d50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000d60: 00ab 0000 0000 0000 0001 007c 006a 0200  ...........|.j..
+00000d70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000d80: 0053 0029 044e 7231 0000 0072 2f00 0000  .S.).Nr1...r/...
+00000d90: 7a31 556e 6578 7065 6374 6564 2073 7461  z1Unexpected sta
+00000da0: 7465 2e20 5365 7276 6963 6549 6e73 7461  te. ServiceInsta
+00000db0: 6e63 6550 726f 7669 6465 7220 6e6f 7420  nceProvider not 
+00000dc0: 7365 7429 08da 0768 6173 6174 7472 7231  set)...hasattrr1
+00000dd0: 0000 0072 2f00 0000 7207 0000 00da 1763  ...r/...r......c
+00000de0: 7265 6174 655f 7365 7276 6963 655f 696e  reate_service_in
+00000df0: 7374 616e 6365 7217 0000 0072 3000 0000  stancer....r0...
+00000e00: da05 7374 6172 7472 1b00 0000 7301 0000  ..startr....s...
+00000e10: 0020 7216 0000 0072 1e00 0000 7a33 5369  . r....r....z3Si
+00000e20: 6e67 6c65 746f 6e53 6572 7669 6365 4c69  ngletonServiceLi
+00000e30: 6665 6379 636c 6543 6f6e 7472 6f6c 6c65  fecycleControlle
+00000e40: 7249 6d70 6c2e 6765 745f 7365 7276 6963  rImpl.get_servic
+00000e50: 654c 0000 0073 9600 0000 8000 f40a 0011  eL...s..........
+00000e60: 1898 04d0 1e33 d410 34d8 0c10 d70c 24d1  .....3..4.....$.
+00000e70: 0c24 d00c 2ce4 141b 9844 d022 3ed4 143f  .$..,....D.">..?
+00000e80: d810 14d7 102f d110 2fd0 1037 e416 26d8  ...../../..7..&.
+00000e90: 1447 f303 0217 12f0 0002 1112 f00a 0011  .G..............
+00000ea0: 15d7 102f d110 2fd7 1047 d110 47d3 1049  .../../..G..G..I
+00000eb0: f003 000d 11d4 0c24 f006 000d 11d7 0c24  .......$.......$
+00000ec0: d10c 24d7 0c29 d10c 29a8 24af 2ca9 2cd4  ..$..)..).$.,.,.
+00000ed0: 0c37 d80c 10d7 0c24 d10c 24d7 0c2a d10c  .7.....$..$..*..
+00000ee0: 2ad4 0c2c e00f 13d7 0f27 d10f 27d0 0827  *..,.....'..'..'
+00000ef0: 7219 0000 0063 0100 0000 0000 0000 0000  r....c..........
+00000f00: 0000 0400 0000 1300 0000 f3ce 0000 0097  ................
+00000f10: 0074 0100 0000 0000 0000 007c 0064 01ab  .t.........|.d..
+00000f20: 0200 0000 0000 0072 477c 006a 0200 0000  .......rG|.j....
+00000f30: 0000 0000 0000 0000 0000 0000 0000 0081  ................
+00000f40: 3b7c 006a 0200 0000 0000 0000 0000 0000  ;|.j............
+00000f50: 0000 0000 0000 006a 0500 0000 0000 0000  .......j........
+00000f60: 0000 0000 0000 0000 0000 00ab 0000 0000  ................
+00000f70: 0000 0001 007c 006a 0200 0000 0000 0000  .....|.j........
+00000f80: 0000 0000 0000 0000 0000 006a 0700 0000  ...........j....
+00000f90: 0000 0000 0000 0000 0000 0000 0000 00ab  ................
+00000fa0: 0000 0000 0000 0001 0064 007c 005f 0100  .........d.|._..
+00000fb0: 0000 0000 0000 0074 0800 0000 0000 0000  .......t........
+00000fc0: 007c 005f 0500 0000 0000 0000 0064 007c  .|._.........d.|
+00000fd0: 005f 0600 0000 0000 0000 0079 0029 024e  ._.........y.).N
+00000fe0: 7231 0000 0029 0772 3500 0000 7231 0000  r1...).r5...r1..
+00000ff0: 00da 0473 746f 70da 0764 6573 7472 6f79  ...stop..destroy
+00001000: 720b 0000 0072 3000 0000 722f 0000 0072  r....r0...r/...r
+00001010: 1b00 0000 7301 0000 0020 7216 0000 0072  ....s.... r....r
+00001020: 1c00 0000 7a30 5369 6e67 6c65 746f 6e53  ....z0SingletonS
+00001030: 6572 7669 6365 4c69 6665 6379 636c 6543  erviceLifecycleC
+00001040: 6f6e 7472 6f6c 6c65 7249 6d70 6c2e 7368  ontrollerImpl.sh
+00001050: 7574 646f 776e 6300 0000 7356 0000 0080  utdownc...sV....
+00001060: 00f4 0a00 0c13 9034 d019 2ed4 0b2f d80c  .......4...../..
+00001070: 10d7 0c24 d10c 24d0 0c30 e00c 10d7 0c24  ...$..$..0.....$
+00001080: d10c 24d7 0c29 d10c 29d4 0c2b d80c 10d7  ..$..)..)..+....
+00001090: 0c24 d10c 24d7 0c2c d10c 2cd4 0c2e d827  .$..$..,..,....'
+000010a0: 2b88 44d4 0c24 e417 3288 048c 0cd8 2a2e  +.D..$..2.....*.
+000010b0: 8804 d508 2772 1900 0000 721f 0000 0029  ....'r....r....)
+000010c0: 0b72 2000 0000 7221 0000 0072 2200 0000  .r ...r!...r"...
+000010d0: 7223 0000 0072 2400 0000 7232 0000 0072  r#...r$...r2...r
+000010e0: 0600 0000 720a 0000 0072 1700 0000 721e  ....r....r....r.
+000010f0: 0000 0072 1c00 0000 7225 0000 0073 0300  ...r....r%...s..
+00001100: 0000 8080 8072 1600 0000 722c 0000 0072  .....r....r,...r
+00001110: 2c00 0000 3400 0000 7371 0000 00f8 8700  ,...4...sq......
+00001120: f106 0205 08f2 0803 0528 f00a 0006 0ef0  .........(......
+00001130: 0209 051e e023 3ab9 38d1 2344 f005 0905  .....#:.8.#D....
+00001140: 1ef1 0600 111f f007 0905 1ef0 0800 0a0e  ................
+00001150: f209 0905 1ef3 0300 060e f002 0905 1ef0  ................
+00001160: 1600 060e f002 1405 2899 58f2 0014 0528  ........(.X....(
+00001170: f303 0006 0ef0 0214 0528 f02c 0006 0ef2  .........(.,....
+00001180: 020c 052f f303 0006 0ef1 020c 052f 7219  .../........./r.
+00001190: 0000 0072 2c00 0000 2901 720e 0000 0072  ...r,...).r....r
+000011a0: 2700 0000 7304 0000 0020 4040 4072 1600  '...s.... @@@r..
+000011b0: 0000 fa3f 3c67 656e 6572 6963 2070 6172  ...?<generic par
+000011c0: 616d 6574 6572 7320 6f66 2053 696e 676c  ameters of Singl
+000011d0: 6574 6f6e 5365 7276 6963 654c 6966 6563  etonServiceLifec
+000011e0: 7963 6c65 436f 6e74 726f 6c6c 6572 496d  ycleControllerIm
+000011f0: 706c 3e72 3b00 0000 3400 0000 7325 0000  pl>r;...4...s%..
+00001200: 00fa 8000 ab68 bb0e a868 f700 3c01 2ff4  .....h...h..<./.
+00001210: 003c 012f dc04 1e98 78a8 1ed0 1f37 d104  .<./....x....7..
+00001220: 38f5 033c 012f 7219 0000 0063 0000 0000  8..<./r....c....
+00001230: 0000 0000 0000 0000 0300 0000 0000 0000  ................
+00001240: f326 0000 0097 0065 005a 0164 005a 0255  .&.....e.Z.d.Z.U
+00001250: 0064 015a 0365 045a 0565 0665 0719 0000  .d.Z.e.Z.e.e....
+00001260: 0065 0864 023c 0000 0079 0329 04da 204b  .e.d.<...y.).. K
+00001270: 6e6f 776e 5365 7276 6963 654c 6966 6563  nownServiceLifec
+00001280: 7963 6c65 436f 6e74 726f 6c6c 6572 737a  ycleControllersz
+00001290: 3b0a 2020 2020 4b6e 6f77 6e20 5365 7276  ;.    Known Serv
+000012a0: 6963 654c 6966 6563 7963 6c65 436f 6e74  iceLifecycleCont
+000012b0: 726f 6c6c 6572 2069 6d70 6c65 6d65 6e74  roller implement
+000012c0: 6174 696f 6e73 2e0a 2020 2020 da09 5349  ations..    ..SI
+000012d0: 4e47 4c45 544f 4e4e 2909 7220 0000 0072  NGLETONN).r ...r
+000012e0: 2100 0000 7222 0000 0072 2400 0000 722c  !...r"...r$...r,
+000012f0: 0000 0072 3e00 0000 7205 0000 00da 0474  ...r>...r......t
+00001300: 7970 65da 0f5f 5f61 6e6e 6f74 6174 696f  ype..__annotatio
+00001310: 6e73 5f5f 7213 0000 0072 1900 0000 7216  ns__r....r....r.
+00001320: 0000 0072 3d00 0000 723d 0000 0073 0000  ...r=...r=...s..
+00001330: 0073 1800 0000 8500 f102 0205 08f0 0800  .s..............
+00001340: 1e45 0180 4988 7590 5489 7bd4 0444 7219  .E..I.u.T.{..Dr.
+00001350: 0000 0072 3d00 0000 4e29 1372 2400 0000  ...r=...N).r$...
+00001360: da03 6162 6372 0300 0000 7204 0000 00da  ..abcr....r.....
+00001370: 0674 7970 696e 6772 0500 0000 da11 7479  .typingr......ty
+00001380: 7069 6e67 5f65 7874 656e 7369 6f6e 7372  ping_extensionsr
+00001390: 0600 0000 da1f 7370 6879 726e 612e 7365  ......sphyrna.se
+000013a0: 7276 6963 655f 6d61 6e61 6765 722e 7365  rvice_manager.se
+000013b0: 7276 6963 6572 0700 0000 7208 0000 0072  rvicer....r....r
+000013c0: 0900 0000 da31 7370 6879 726e 612e 7365  .....1sphyrna.se
+000013d0: 7276 6963 655f 6d61 6e61 6765 722e 7365  rvice_manager.se
+000013e0: 7276 6963 655f 696e 7374 616e 6365 5f70  rvice_instance_p
+000013f0: 726f 7669 6465 7272 0a00 0000 da2d 7370  roviderr.....-sp
+00001400: 6879 726e 612e 7365 7276 6963 655f 6d61  hyrna.service_ma
+00001410: 6e61 6765 722e 7365 7276 6963 655f 636f  nager.service_co
+00001420: 6e66 6967 7572 6174 696f 6e72 0b00 0000  nfigurationr....
+00001430: 720e 0000 0072 2c00 0000 723d 0000 0072  r....r,...r=...r
+00001440: 1300 0000 7219 0000 0072 1600 0000 fa08  ....r....r......
+00001450: 3c6d 6f64 756c 653e 7247 0000 0001 0000  <module>rG......
+00001460: 0073 3900 0000 f003 0101 01f1 0203 0104  .s9.............
+00001470: f70a 0001 24dd 0018 dd00 26df 0056 d100  ....$.....&..V..
+00001480: 56dd 0055 dd00 55f7 081f 010c f74a 013c  V..U..U......J.<
+00001490: 012f f77e 0105 0145 01f2 0005 0145 0172  ./.~...E.....E.r
+000014a0: 1900 0000                                ....
```

### Comparing `sphyrna_service_manager-0.3.0/src/main/python/sphyrna/service_manager/__pycache__/service_manager.cpython-312.pyc` & `sphyrna_service_manager-0.3.7/src/main/python/sphyrna/service_manager/__pycache__/service_manager.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Mon Apr 15 00:14:21 2024 UTC, .py size: 2351 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 5d71 1c66 2f09 0000  ........]q.f/...
+00000000: cb0d 0d0a 0000 0000 db6d 4066 2f09 0000  .........m@f/...
 00000010: e300 0000 0000 0000 0000 0000 0004 0000  ................
 00000020: 0000 0000 00f3 4800 0000 9700 6400 5a00  ......H.....d.Z.
 00000030: 6401 6402 6c01 6d02 5a02 6d03 5a03 0100  d.d.l.m.Z.m.Z...
 00000040: 6401 6403 6c04 6d05 5a05 0100 6401 6404  d.d.l.m.Z...d.d.
 00000050: 6c06 6d07 5a07 6d08 5a08 0100 0200 4700  l.m.Z.m.Z.....G.
 00000060: 6405 8400 6406 ab02 0000 0000 0000 5a09  d...d.........Z.
 00000070: 7907 2908 7a7f 0a54 6869 7320 6d6f 6475  y.).z..This modu
@@ -68,132 +68,133 @@
 00000430: 6f72 7465 6420 6279 2074 6865 2061 7373  orted by the ass
 00000440: 6f63 6961 7465 640a 2020 2020 2020 2020  ociated.        
 00000450: 5365 7276 6963 654c 6966 6563 7963 6c65  ServiceLifecycle
 00000460: 4d61 6e61 6765 720a 2020 2020 2020 2020  Manager.        
 00000470: 2903 7209 0000 0072 0a00 0000 da0b 6765  ).r....r......ge
 00000480: 745f 7365 7276 6963 6529 03da 0363 6c73  t_service)...cls
 00000490: 720b 0000 0072 0c00 0000 7303 0000 0020  r....r....s.... 
-000004a0: 2020 fa6a 2f55 7365 7273 2f6b 616d 656c    .j/Users/kamel
+000004a0: 2020 fa7a 2f55 7365 7273 2f6b 616d 656c    .z/Users/kamel
 000004b0: 656f 6e2f 436f 6465 2f73 6572 7669 6365  eon/Code/service
-000004c0: 2f70 6163 6b61 6765 732f 7079 7468 6f6e  /packages/python
-000004d0: 6c69 622f 7372 632f 6d61 696e 2f70 7974  lib/src/main/pyt
-000004e0: 686f 6e2f 7370 6879 726e 612f 7365 7276  hon/sphyrna/serv
-000004f0: 6963 655f 6d61 6e61 6765 722f 7365 7276  ice_manager/serv
-00000500: 6963 655f 6d61 6e61 6765 722e 7079 720f  ice_manager.pyr.
-00000510: 0000 007a 1a53 6572 7669 6365 4d61 6e61  ...z.ServiceMana
-00000520: 6765 722e 6765 745f 7365 7276 6963 6517  ger.get_service.
-00000530: 0000 0073 1d00 0000 8000 f41c 0010 1ed7  ...s............
-00000540: 0f37 d10f 37d7 0f43 d10f 43c0 44c8 26d3  .7..7..C..C.D.&.
-00000550: 0f51 d008 51f3 0000 0000 6302 0000 0000  .Q..Q.....c.....
-00000560: 0000 0000 0000 0003 0000 0003 0000 00f3  ................
-00000570: 4000 0000 9700 7400 0000 0000 0000 0000  @.....t.........
-00000580: 6a02 0000 0000 0000 0000 0000 0000 0000  j...............
-00000590: 0000 0000 6a05 0000 0000 0000 0000 0000  ....j...........
-000005a0: 0000 0000 0000 0000 7c01 ab01 0000 0000  ........|.......
-000005b0: 0000 5300 2901 7a51 0a20 2020 2020 2020  ..S.).zQ.       
-000005c0: 2044 6574 6572 6d69 6e65 2069 6620 6120   Determine if a 
-000005d0: 7365 7276 6963 6520 7769 7468 2074 6865  service with the
-000005e0: 2073 7065 6369 6669 6564 206e 616d 6520   specified name 
-000005f0: 6861 7320 6265 656e 2064 6566 696e 6564  has been defined
-00000600: 0a20 2020 2020 2020 2029 0372 0900 0000  .        ).r....
-00000610: 720a 0000 00da 1269 735f 7365 7276 6963  r......is_servic
-00000620: 655f 6465 6669 6e65 6429 0272 1000 0000  e_defined).r....
-00000630: 720b 0000 0073 0200 0000 2020 7211 0000  r....s....  r...
-00000640: 0072 1400 0000 7a21 5365 7276 6963 654d  .r....z!ServiceM
-00000650: 616e 6167 6572 2e69 735f 7365 7276 6963  anager.is_servic
-00000660: 655f 6465 6669 6e65 6427 0000 0073 1b00  e_defined'...s..
-00000670: 0000 8000 f40a 0010 1ed7 0f37 d10f 37d7  ...........7..7.
-00000680: 0f4a d10f 4ac8 34d3 0f50 d008 5072 1200  .J..J.4..P..Pr..
-00000690: 0000 4e63 0100 0000 0000 0000 0000 0000  ..Nc............
-000006a0: 0200 0000 0300 0000 f340 0000 0097 0074  .........@.....t
-000006b0: 0000 0000 0000 0000 006a 0200 0000 0000  .........j......
-000006c0: 0000 0000 0000 0000 0000 0000 006a 0500  .............j..
-000006d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000006e0: 00ab 0000 0000 0000 0001 0079 0129 027a  ...........y.).z
-000006f0: 490a 2020 2020 2020 2020 5368 7574 646f  I.        Shutdo
-00000700: 776e 2074 6865 2053 6572 7669 6365 4d61  wn the ServiceMa
-00000710: 6e61 6765 7220 616e 6420 616c 6c20 6173  nager and all as
-00000720: 736f 6369 6174 6564 2073 6572 7669 6365  sociated service
-00000730: 730a 2020 2020 2020 2020 4e29 0372 0900  s.        N).r..
-00000740: 0000 720a 0000 00da 0873 6875 7464 6f77  ..r......shutdow
-00000750: 6e29 0172 1000 0000 7301 0000 0020 7211  n).r....s.... r.
-00000760: 0000 0072 1600 0000 7a17 5365 7276 6963  ...r....z.Servic
-00000770: 654d 616e 6167 6572 2e73 6875 7464 6f77  eManager.shutdow
-00000780: 6e2e 0000 0073 1600 0000 8000 f40a 0009  n....s..........
-00000790: 17d7 0830 d108 30d7 0839 d108 39d5 083b  ...0..0..9..9..;
-000007a0: 7212 0000 00da 0f73 7472 6174 6567 795f  r......strategy_
-000007b0: 746f 5f73 6574 6302 0000 0000 0000 0000  to_setc.........
-000007c0: 0000 0002 0000 0003 0000 00f3 1a00 0000  ................
-000007d0: 9700 7c01 7400 0000 0000 0000 0000 5f01  ..|.t........._.
-000007e0: 0000 0000 0000 0000 7901 2902 619d 0100  ........y.).a...
-000007f0: 000a 2020 2020 2020 2020 5365 7420 7468  ..        Set th
-00000800: 6520 7365 7276 6963 6520 6d61 6e61 6765  e service manage
-00000810: 7220 7374 7261 7465 6779 2e20 2054 6869  r strategy.  Thi
-00000820: 7320 7374 7261 7465 6779 2077 696c 6c20  s strategy will 
-00000830: 6265 2075 7365 6420 746f 2072 6574 7269  be used to retri
-00000840: 6576 6520 7365 7276 6963 6573 0a20 2020  eve services.   
-00000850: 2020 2020 2062 6173 6564 206f 6e20 7468       based on th
-00000860: 6520 616c 676f 7269 7468 6d20 6465 6669  e algorithm defi
-00000870: 6e65 6420 696e 2074 6865 2053 6572 7669  ned in the Servi
-00000880: 6365 4d61 6e61 6765 7246 6163 746f 7279  ceManagerFactory
-00000890: 2069 6d70 6c65 6d65 6e74 6e61 7461 7469   implementnatati
-000008a0: 6f6e 0a0a 2020 2020 2020 2020 496e 2074  on..        In t
-000008b0: 6865 2066 7574 7572 652c 2061 2053 6572  he future, a Ser
-000008c0: 7669 6365 4d61 6e61 6765 7220 6d61 7920  viceManager may 
-000008d0: 6265 2061 626c 6520 746f 2075 7365 206d  be able to use m
-000008e0: 756c 7469 706c 6520 7374 7261 7465 6769  ultiple strategi
-000008f0: 6573 2063 6f6e 6375 7272 656e 746c 792e  es concurrently.
-00000900: 2020 4173 206f 6620 7468 6520 6375 7272    As of the curr
-00000910: 656e 7420 4150 492c 2069 740a 2020 2020  ent API, it.    
-00000920: 2020 2020 6f6e 6c79 2073 7570 706f 7274      only support
-00000930: 7320 6120 7369 6e67 6c65 2073 7472 6174  s a single strat
-00000940: 6567 790a 0a20 2020 2020 2020 2040 7061  egy..        @pa
-00000950: 7261 6d20 7374 7261 7465 6779 546f 5365  ram strategyToSe
-00000960: 7420 7468 6520 7365 7276 6963 6520 6d61  t the service ma
-00000970: 6e61 6765 7220 7374 7261 7465 6779 2074  nager strategy t
-00000980: 6f20 7365 740a 2020 2020 2020 2020 4e29  o set.        N)
-00000990: 0272 0900 0000 720a 0000 0029 0272 1000  .r....r....).r..
-000009a0: 0000 7217 0000 0073 0200 0000 2020 7211  ..r....s....  r.
-000009b0: 0000 00da 1473 6574 5f64 6566 6175 6c74  .....set_default
-000009c0: 5f73 7472 6174 6567 797a 2353 6572 7669  _strategyz#Servi
-000009d0: 6365 4d61 6e61 6765 722e 7365 745f 6465  ceManager.set_de
-000009e0: 6661 756c 745f 7374 7261 7465 6779 3500  fault_strategy5.
-000009f0: 0000 730d 0000 0080 00f0 1600 3443 018c  ..s.........4C..
-00000a00: 0ed5 0830 7212 0000 0029 0272 0d00 0000  ...0r....).r....
-00000a10: 4e29 12da 085f 5f6e 616d 655f 5fda 0a5f  N)...__name__.._
-00000a20: 5f6d 6f64 756c 655f 5fda 0c5f 5f71 7561  _module__..__qua
-00000a30: 6c6e 616d 655f 5fda 075f 5f64 6f63 5f5f  lname__..__doc__
-00000a40: 7206 0000 0072 0a00 0000 7207 0000 00da  r....r....r.....
-00000a50: 0f5f 5f61 6e6e 6f74 6174 696f 6e73 5f5f  .__annotations__
-00000a60: da0b 636c 6173 736d 6574 686f 6472 0500  ..classmethodr..
-00000a70: 0000 da03 7374 7272 0300 0000 7204 0000  ....strr....r...
-00000a80: 0072 0f00 0000 da04 626f 6f6c 7214 0000  .r......boolr...
-00000a90: 0072 1600 0000 7219 0000 00a9 0072 1200  .r....r......r..
-00000aa0: 0000 7211 0000 0072 0900 0000 7209 0000  ..r....r....r...
-00000ab0: 000e 0000 0073 ac00 0000 8500 f102 0405  .....s..........
-00000ac0: 08f1 0c00 3955 01d3 3856 d004 1dd0 1f35  ....9U..8V.....5
-00000ad0: d304 56e0 0510 e031 4cf1 030d 0552 01d8  ..V....1L....R..
-00000ae0: 1316 f003 0d05 5201 d820 2ef0 030d 0552  ......R.. .....R
-00000af0: 01e0 0911 f205 0d05 5201 f303 0006 11f0  ........R.......
-00000b00: 020d 0552 01f0 1e00 0611 f002 0405 5101  ...R..........Q.
-00000b10: a063 f000 0405 5101 a864 f200 0405 5101  .c....Q..d....Q.
-00000b20: f303 0006 11f0 0204 0551 01f0 0c00 0611  .........Q......
-00000b30: f202 0405 3cf3 0300 0611 f002 0405 3cf0  ....<.........<.
-00000b40: 0c00 0611 f002 0a05 4301 d033 49f0 000a  ........C..3I...
-00000b50: 0543 01c8 64f2 000a 0543 01f3 0300 0611  .C..d....C......
-00000b60: f102 0a05 4301 7212 0000 0072 0900 0000  ....C.r....r....
-00000b70: 4e29 0a72 1d00 0000 da1f 7370 6879 726e  N).r......sphyrn
-00000b80: 612e 7365 7276 6963 655f 6d61 6e61 6765  a.service_manage
-00000b90: 722e 7365 7276 6963 6572 0300 0000 7204  r.servicer....r.
-00000ba0: 0000 00da 2d73 7068 7972 6e61 2e73 6572  ....-sphyrna.ser
-00000bb0: 7669 6365 5f6d 616e 6167 6572 2e73 6572  vice_manager.ser
-00000bc0: 7669 6365 5f63 6f6e 6669 6775 7261 7469  vice_configurati
-00000bd0: 6f6e 7205 0000 00da 3073 7068 7972 6e61  onr.....0sphyrna
-00000be0: 2e73 6572 7669 6365 5f6d 616e 6167 6572  .service_manager
+000004c0: 2f74 6172 6765 742f 6368 6563 6b6f 7574  /target/checkout
+000004d0: 2f70 6163 6b61 6765 732f 7079 7468 6f6e  /packages/python
+000004e0: 6c69 622f 7372 632f 6d61 696e 2f70 7974  lib/src/main/pyt
+000004f0: 686f 6e2f 7370 6879 726e 612f 7365 7276  hon/sphyrna/serv
+00000500: 6963 655f 6d61 6e61 6765 722f 7365 7276  ice_manager/serv
+00000510: 6963 655f 6d61 6e61 6765 722e 7079 720f  ice_manager.pyr.
+00000520: 0000 007a 1a53 6572 7669 6365 4d61 6e61  ...z.ServiceMana
+00000530: 6765 722e 6765 745f 7365 7276 6963 6517  ger.get_service.
+00000540: 0000 0073 1d00 0000 8000 f41c 0010 1ed7  ...s............
+00000550: 0f37 d10f 37d7 0f43 d10f 43c0 44c8 26d3  .7..7..C..C.D.&.
+00000560: 0f51 d008 51f3 0000 0000 6302 0000 0000  .Q..Q.....c.....
+00000570: 0000 0000 0000 0003 0000 0003 0000 00f3  ................
+00000580: 4000 0000 9700 7400 0000 0000 0000 0000  @.....t.........
+00000590: 6a02 0000 0000 0000 0000 0000 0000 0000  j...............
+000005a0: 0000 0000 6a05 0000 0000 0000 0000 0000  ....j...........
+000005b0: 0000 0000 0000 0000 7c01 ab01 0000 0000  ........|.......
+000005c0: 0000 5300 2901 7a51 0a20 2020 2020 2020  ..S.).zQ.       
+000005d0: 2044 6574 6572 6d69 6e65 2069 6620 6120   Determine if a 
+000005e0: 7365 7276 6963 6520 7769 7468 2074 6865  service with the
+000005f0: 2073 7065 6369 6669 6564 206e 616d 6520   specified name 
+00000600: 6861 7320 6265 656e 2064 6566 696e 6564  has been defined
+00000610: 0a20 2020 2020 2020 2029 0372 0900 0000  .        ).r....
+00000620: 720a 0000 00da 1269 735f 7365 7276 6963  r......is_servic
+00000630: 655f 6465 6669 6e65 6429 0272 1000 0000  e_defined).r....
+00000640: 720b 0000 0073 0200 0000 2020 7211 0000  r....s....  r...
+00000650: 0072 1400 0000 7a21 5365 7276 6963 654d  .r....z!ServiceM
+00000660: 616e 6167 6572 2e69 735f 7365 7276 6963  anager.is_servic
+00000670: 655f 6465 6669 6e65 6427 0000 0073 1b00  e_defined'...s..
+00000680: 0000 8000 f40a 0010 1ed7 0f37 d10f 37d7  ...........7..7.
+00000690: 0f4a d10f 4ac8 34d3 0f50 d008 5072 1200  .J..J.4..P..Pr..
+000006a0: 0000 4e63 0100 0000 0000 0000 0000 0000  ..Nc............
+000006b0: 0200 0000 0300 0000 f340 0000 0097 0074  .........@.....t
+000006c0: 0000 0000 0000 0000 006a 0200 0000 0000  .........j......
+000006d0: 0000 0000 0000 0000 0000 0000 006a 0500  .............j..
+000006e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000006f0: 00ab 0000 0000 0000 0001 0079 0129 027a  ...........y.).z
+00000700: 490a 2020 2020 2020 2020 5368 7574 646f  I.        Shutdo
+00000710: 776e 2074 6865 2053 6572 7669 6365 4d61  wn the ServiceMa
+00000720: 6e61 6765 7220 616e 6420 616c 6c20 6173  nager and all as
+00000730: 736f 6369 6174 6564 2073 6572 7669 6365  sociated service
+00000740: 730a 2020 2020 2020 2020 4e29 0372 0900  s.        N).r..
+00000750: 0000 720a 0000 00da 0873 6875 7464 6f77  ..r......shutdow
+00000760: 6e29 0172 1000 0000 7301 0000 0020 7211  n).r....s.... r.
+00000770: 0000 0072 1600 0000 7a17 5365 7276 6963  ...r....z.Servic
+00000780: 654d 616e 6167 6572 2e73 6875 7464 6f77  eManager.shutdow
+00000790: 6e2e 0000 0073 1600 0000 8000 f40a 0009  n....s..........
+000007a0: 17d7 0830 d108 30d7 0839 d108 39d5 083b  ...0..0..9..9..;
+000007b0: 7212 0000 00da 0f73 7472 6174 6567 795f  r......strategy_
+000007c0: 746f 5f73 6574 6302 0000 0000 0000 0000  to_setc.........
+000007d0: 0000 0002 0000 0003 0000 00f3 1a00 0000  ................
+000007e0: 9700 7c01 7400 0000 0000 0000 0000 5f01  ..|.t........._.
+000007f0: 0000 0000 0000 0000 7901 2902 619d 0100  ........y.).a...
+00000800: 000a 2020 2020 2020 2020 5365 7420 7468  ..        Set th
+00000810: 6520 7365 7276 6963 6520 6d61 6e61 6765  e service manage
+00000820: 7220 7374 7261 7465 6779 2e20 2054 6869  r strategy.  Thi
+00000830: 7320 7374 7261 7465 6779 2077 696c 6c20  s strategy will 
+00000840: 6265 2075 7365 6420 746f 2072 6574 7269  be used to retri
+00000850: 6576 6520 7365 7276 6963 6573 0a20 2020  eve services.   
+00000860: 2020 2020 2062 6173 6564 206f 6e20 7468       based on th
+00000870: 6520 616c 676f 7269 7468 6d20 6465 6669  e algorithm defi
+00000880: 6e65 6420 696e 2074 6865 2053 6572 7669  ned in the Servi
+00000890: 6365 4d61 6e61 6765 7246 6163 746f 7279  ceManagerFactory
+000008a0: 2069 6d70 6c65 6d65 6e74 6e61 7461 7469   implementnatati
+000008b0: 6f6e 0a0a 2020 2020 2020 2020 496e 2074  on..        In t
+000008c0: 6865 2066 7574 7572 652c 2061 2053 6572  he future, a Ser
+000008d0: 7669 6365 4d61 6e61 6765 7220 6d61 7920  viceManager may 
+000008e0: 6265 2061 626c 6520 746f 2075 7365 206d  be able to use m
+000008f0: 756c 7469 706c 6520 7374 7261 7465 6769  ultiple strategi
+00000900: 6573 2063 6f6e 6375 7272 656e 746c 792e  es concurrently.
+00000910: 2020 4173 206f 6620 7468 6520 6375 7272    As of the curr
+00000920: 656e 7420 4150 492c 2069 740a 2020 2020  ent API, it.    
+00000930: 2020 2020 6f6e 6c79 2073 7570 706f 7274      only support
+00000940: 7320 6120 7369 6e67 6c65 2073 7472 6174  s a single strat
+00000950: 6567 790a 0a20 2020 2020 2020 2040 7061  egy..        @pa
+00000960: 7261 6d20 7374 7261 7465 6779 546f 5365  ram strategyToSe
+00000970: 7420 7468 6520 7365 7276 6963 6520 6d61  t the service ma
+00000980: 6e61 6765 7220 7374 7261 7465 6779 2074  nager strategy t
+00000990: 6f20 7365 740a 2020 2020 2020 2020 4e29  o set.        N)
+000009a0: 0272 0900 0000 720a 0000 0029 0272 1000  .r....r....).r..
+000009b0: 0000 7217 0000 0073 0200 0000 2020 7211  ..r....s....  r.
+000009c0: 0000 00da 1473 6574 5f64 6566 6175 6c74  .....set_default
+000009d0: 5f73 7472 6174 6567 797a 2353 6572 7669  _strategyz#Servi
+000009e0: 6365 4d61 6e61 6765 722e 7365 745f 6465  ceManager.set_de
+000009f0: 6661 756c 745f 7374 7261 7465 6779 3500  fault_strategy5.
+00000a00: 0000 730d 0000 0080 00f0 1600 3443 018c  ..s.........4C..
+00000a10: 0ed5 0830 7212 0000 0029 0272 0d00 0000  ...0r....).r....
+00000a20: 4e29 12da 085f 5f6e 616d 655f 5fda 0a5f  N)...__name__.._
+00000a30: 5f6d 6f64 756c 655f 5fda 0c5f 5f71 7561  _module__..__qua
+00000a40: 6c6e 616d 655f 5fda 075f 5f64 6f63 5f5f  lname__..__doc__
+00000a50: 7206 0000 0072 0a00 0000 7207 0000 00da  r....r....r.....
+00000a60: 0f5f 5f61 6e6e 6f74 6174 696f 6e73 5f5f  .__annotations__
+00000a70: da0b 636c 6173 736d 6574 686f 6472 0500  ..classmethodr..
+00000a80: 0000 da03 7374 7272 0300 0000 7204 0000  ....strr....r...
+00000a90: 0072 0f00 0000 da04 626f 6f6c 7214 0000  .r......boolr...
+00000aa0: 0072 1600 0000 7219 0000 00a9 0072 1200  .r....r......r..
+00000ab0: 0000 7211 0000 0072 0900 0000 7209 0000  ..r....r....r...
+00000ac0: 000e 0000 0073 ac00 0000 8500 f102 0405  .....s..........
+00000ad0: 08f1 0c00 3955 01d3 3856 d004 1dd0 1f35  ....9U..8V.....5
+00000ae0: d304 56e0 0510 e031 4cf1 030d 0552 01d8  ..V....1L....R..
+00000af0: 1316 f003 0d05 5201 d820 2ef0 030d 0552  ......R.. .....R
+00000b00: 01e0 0911 f205 0d05 5201 f303 0006 11f0  ........R.......
+00000b10: 020d 0552 01f0 1e00 0611 f002 0405 5101  ...R..........Q.
+00000b20: a063 f000 0405 5101 a864 f200 0405 5101  .c....Q..d....Q.
+00000b30: f303 0006 11f0 0204 0551 01f0 0c00 0611  .........Q......
+00000b40: f202 0405 3cf3 0300 0611 f002 0405 3cf0  ....<.........<.
+00000b50: 0c00 0611 f002 0a05 4301 d033 49f0 000a  ........C..3I...
+00000b60: 0543 01c8 64f2 000a 0543 01f3 0300 0611  .C..d....C......
+00000b70: f102 0a05 4301 7212 0000 0072 0900 0000  ....C.r....r....
+00000b80: 4e29 0a72 1d00 0000 da1f 7370 6879 726e  N).r......sphyrn
+00000b90: 612e 7365 7276 6963 655f 6d61 6e61 6765  a.service_manage
+00000ba0: 722e 7365 7276 6963 6572 0300 0000 7204  r.servicer....r.
+00000bb0: 0000 00da 2d73 7068 7972 6e61 2e73 6572  ....-sphyrna.ser
+00000bc0: 7669 6365 5f6d 616e 6167 6572 2e73 6572  vice_manager.ser
+00000bd0: 7669 6365 5f63 6f6e 6669 6775 7261 7469  vice_configurati
+00000be0: 6f6e 7205 0000 00da 3073 7068 7972 6e61  onr.....0sphyrna
 00000bf0: 2e73 6572 7669 6365 5f6d 616e 6167 6572  .service_manager
-00000c00: 5f73 7472 6174 6567 7972 0600 0000 7207  _strategyr....r.
-00000c10: 0000 0072 0900 0000 7222 0000 0072 1200  ...r....r"...r..
-00000c20: 0000 7211 0000 00fa 083c 6d6f 6475 6c65  ..r......<module
-00000c30: 3e72 2600 0000 0100 0000 7324 0000 00f0  >r&.......s$....
-00000c40: 0301 0101 f102 0301 04f7 0a00 0145 01dd  .............E..
-00000c50: 0055 f702 0301 02f7 0c32 0143 01f2 0032  .U.......2.C...2
-00000c60: 0143 0172 1200 0000                      .C.r....
+00000c00: 2e73 6572 7669 6365 5f6d 616e 6167 6572  .service_manager
+00000c10: 5f73 7472 6174 6567 7972 0600 0000 7207  _strategyr....r.
+00000c20: 0000 0072 0900 0000 7222 0000 0072 1200  ...r....r"...r..
+00000c30: 0000 7211 0000 00fa 083c 6d6f 6475 6c65  ..r......<module
+00000c40: 3e72 2600 0000 0100 0000 7324 0000 00f0  >r&.......s$....
+00000c50: 0301 0101 f102 0301 04f7 0a00 0145 01dd  .............E..
+00000c60: 0055 f702 0301 02f7 0c32 0143 01f2 0032  .U.......2.C...2
+00000c70: 0143 0172 1200 0000                      .C.r....
```

### Comparing `sphyrna_service_manager-0.3.0/src/main/python/sphyrna/service_manager/__pycache__/service_manager_strategy.cpython-312.pyc` & `sphyrna_service_manager-0.3.7/src/main/python/sphyrna/service_manager/__pycache__/service_manager_strategy.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Mon Apr 15 00:42:59 2024 UTC, .py size: 10673 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 1378 1c66 b129 0000  .........x.f.)..
+00000000: cb0d 0d0a 0000 0000 db6d 4066 b129 0000  .........m@f.)..
 00000010: e300 0000 0000 0000 0000 0000 0005 0000  ................
 00000020: 0000 0000 00f3 ba00 0000 9700 6400 5a00  ............d.Z.
 00000030: 6401 6402 6c01 6d02 5a02 6d03 5a03 0100  d.d.l.m.Z.m.Z...
 00000040: 6401 6403 6c04 6d05 5a05 0100 6401 6404  d.d.l.m.Z...d.d.
 00000050: 6c06 6d07 5a07 6d08 5a08 6d09 5a09 0100  l.m.Z.m.Z.m.Z...
 00000060: 6401 6405 6c0a 6d0b 5a0b 6d0c 5a0c 0100  d.d.l.m.Z.m.Z...
 00000070: 6401 6406 6c0d 6d0e 5a0e 6d0f 5a0f 0100  d.d.l.m.Z.m.Z...
@@ -67,666 +67,667 @@
 00000420: 2054 6869 7320 6d75 7374 2062 6520 7375   This must be su
 00000430: 7070 6f72 7465 6420 6279 2074 6865 2061  pported by the a
 00000440: 7373 6f63 6961 7465 640a 2020 2020 2020  ssociated.      
 00000450: 2020 5365 7276 6963 654c 6966 6563 7963    ServiceLifecyc
 00000460: 6c65 4d61 6e61 6765 720a 2020 2020 2020  leManager.      
 00000470: 2020 4ea9 0029 03da 0473 656c 6672 1100    N..)...selfr..
 00000480: 0000 7212 0000 0073 0300 0000 2020 20fa  ..r....s....   .
-00000490: 732f 5573 6572 732f 6b61 6d65 6c65 6f6e  s/Users/kameleon
-000004a0: 2f43 6f64 652f 7365 7276 6963 652f 7061  /Code/service/pa
-000004b0: 636b 6167 6573 2f70 7974 686f 6e6c 6962  ckages/pythonlib
-000004c0: 2f73 7263 2f6d 6169 6e2f 7079 7468 6f6e  /src/main/python
-000004d0: 2f73 7068 7972 6e61 2f73 6572 7669 6365  /sphyrna/service
-000004e0: 5f6d 616e 6167 6572 2f73 6572 7669 6365  _manager/service
-000004f0: 5f6d 616e 6167 6572 5f73 7472 6174 6567  _manager_strateg
-00000500: 792e 7079 da0b 6765 745f 7365 7276 6963  y.py..get_servic
-00000510: 657a 2253 6572 7669 6365 4d61 6e61 6765  ez"ServiceManage
-00000520: 7253 7472 6174 6567 792e 6765 745f 7365  rStrategy.get_se
-00000530: 7276 6963 651d 0000 00f3 0200 0000 8100  rvice...........
-00000540: f300 0000 0063 0200 0000 0000 0000 0000  .....c..........
-00000550: 0000 0000 0000 0300 0000 f304 0000 0097  ................
-00000560: 0079 0129 027a 510a 2020 2020 2020 2020  .y.).zQ.        
-00000570: 4465 7465 726d 696e 6520 6966 2061 2073  Determine if a s
-00000580: 6572 7669 6365 2077 6974 6820 7468 6520  ervice with the 
-00000590: 7370 6563 6966 6965 6420 6e61 6d65 2068  specified name h
-000005a0: 6173 2062 6565 6e20 6465 6669 6e65 640a  as been defined.
-000005b0: 2020 2020 2020 2020 4e72 1500 0000 a902          Nr......
-000005c0: 7216 0000 0072 1100 0000 7302 0000 0020  r....r....s.... 
-000005d0: 2072 1700 0000 da12 6973 5f73 6572 7669   r......is_servi
-000005e0: 6365 5f64 6566 696e 6564 7a29 5365 7276  ce_definedz)Serv
-000005f0: 6963 654d 616e 6167 6572 5374 7261 7465  iceManagerStrate
-00000600: 6779 2e69 735f 7365 7276 6963 655f 6465  gy.is_service_de
-00000610: 6669 6e65 6429 0000 0072 1900 0000 721a  fined)...r....r.
-00000620: 0000 004e 6301 0000 0000 0000 0000 0000  ...Nc...........
-00000630: 0000 0000 0003 0000 00f3 0400 0000 9700  ................
-00000640: 7901 2902 7a49 0a20 2020 2020 2020 2053  y.).zI.        S
-00000650: 6875 7464 6f77 6e20 7468 6520 5365 7276  hutdown the Serv
-00000660: 6963 654d 616e 6167 6572 2061 6e64 2061  iceManager and a
-00000670: 6c6c 2061 7373 6f63 6961 7465 6420 7365  ll associated se
-00000680: 7276 6963 6573 0a20 2020 2020 2020 204e  rvices.        N
-00000690: 7215 0000 00a9 0172 1600 0000 7301 0000  r......r....s...
-000006a0: 0020 7217 0000 00da 0873 6875 7464 6f77  . r......shutdow
-000006b0: 6e7a 1f53 6572 7669 6365 4d61 6e61 6765  nz.ServiceManage
-000006c0: 7253 7472 6174 6567 792e 7368 7574 646f  rStrategy.shutdo
-000006d0: 776e 2f00 0000 7219 0000 0072 1a00 0000  wn/...r....r....
-000006e0: a902 7213 0000 004e 290d da08 5f5f 6e61  ..r....N)...__na
-000006f0: 6d65 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f  me__..__module__
-00000700: da0c 5f5f 7175 616c 6e61 6d65 5f5f da07  ..__qualname__..
-00000710: 5f5f 646f 635f 5f72 0400 0000 7209 0000  __doc__r....r...
-00000720: 00da 0373 7472 7206 0000 0072 0800 0000  ...strr....r....
-00000730: 7218 0000 00da 0462 6f6f 6c72 1d00 0000  r......boolr....
-00000740: 7220 0000 0072 1500 0000 721a 0000 0072  r ...r....r....r
-00000750: 1700 0000 7210 0000 0072 1000 0000 1800  ....r....r......
-00000760: 0000 736c 0000 0084 00f1 0202 0508 f008  ..sl............
-00000770: 0006 14e0 324d f103 0905 0cd8 1417 f003  ....2M..........
-00000780: 0905 0cd8 212f f003 0905 0ce0 0911 f205  ....!/..........
-00000790: 0905 0cf3 0300 0614 f002 0905 0cf0 1600  ................
-000007a0: 0614 f002 0305 0ca0 73f0 0003 050c a874  ........s......t
-000007b0: f200 0305 0cf3 0300 0614 f002 0305 0cf0  ................
-000007c0: 0a00 0614 f202 0305 0cf3 0300 0614 f102  ................
-000007d0: 0305 0c72 1a00 0000 7210 0000 0063 0000  ...r....r....c..
-000007e0: 0000 0000 0000 0000 0000 0500 0000 0300  ................
-000007f0: 0000 f334 0000 0087 0187 0297 0064 00ad  ...4.........d..
-00000800: 0778 018a 0266 018a 0102 0047 0088 0188  .x...f.....G....
-00000810: 0266 0264 0184 0864 0289 01ad 0a7d 007c  .f.d...d.....}.|
-00000820: 00ab 0300 0000 0000 0053 0029 0372 0800  .........S.).r..
-00000830: 0000 6300 0000 0000 0000 0000 0000 0007  ..c.............
-00000840: 0000 0000 0000 00f3 6600 0000 9502 9700  ........f.......
-00000850: 6500 5a01 6400 5a02 5700 b000 5a03 6401  e.Z.d.Z.W...Z.d.
-00000860: 5a04 6402 6505 6602 6403 6506 5700 b001  Z.d.e.f.d.e.W...
-00000870: 6507 6602 1900 0000 6404 6508 5700 b001  e.f.....d.e.W...
-00000880: 1900 0000 6405 6509 6606 6406 8405 5a0a  ....d.e.f.d...Z.
-00000890: 6407 650b 6602 6408 8404 5a0c 6407 6508  d.e.f.d...Z.d.e.
-000008a0: 5700 b001 1900 0000 6602 6409 8404 5a0d  W.......f.d...Z.
-000008b0: 7902 290a da11 5365 7276 6963 6544 6566  y.)...ServiceDef
-000008c0: 696e 6974 696f 6e7a 180a 2020 2020 496e  initionz..    In
-000008d0: 7465 726e 616c 2063 6c61 7373 0a20 2020  ternal class.   
-000008e0: 204e da1c 7365 7276 6963 655f 6c69 6665   N..service_life
-000008f0: 6379 636c 655f 636f 6e74 726f 6c6c 6572  cycle_controller
-00000900: da19 7365 7276 6963 655f 696e 7374 616e  ..service_instan
-00000910: 6365 5f70 726f 7669 6465 7272 1200 0000  ce_providerr....
-00000920: 6304 0000 0000 0000 0000 0000 0002 0000  c...............
-00000930: 0013 0000 00f3 2e00 0000 9700 7c01 7c00  ............|.|.
-00000940: 5f00 0000 0000 0000 0000 7c02 7c00 5f01  _.........|.|._.
-00000950: 0000 0000 0000 0000 7c03 7c00 5f02 0000  ........|.|._...
-00000960: 0000 0000 0000 7900 a901 4e29 0372 2b00  ......y...N).r+.
-00000970: 0000 da1a 5f73 6572 7669 6365 5f69 6e73  ...._service_ins
-00000980: 7461 6e63 655f 7072 6f76 6964 6572 da15  tance_provider..
-00000990: 7365 7276 6963 655f 636f 6e66 6967 7572  service_configur
-000009a0: 6174 696f 6e29 0472 1600 0000 722b 0000  ation).r....r+..
-000009b0: 0072 2c00 0000 7212 0000 0073 0400 0000  .r,...r....s....
-000009c0: 2020 2020 7217 0000 00da 085f 5f69 6e69      r......__ini
-000009d0: 745f 5f7a 1a53 6572 7669 6365 4465 6669  t__z.ServiceDefi
-000009e0: 6e69 7469 6f6e 2e5f 5f69 6e69 745f 5f3e  nition.__init__>
-000009f0: 0000 0073 1d00 0000 8000 f010 002d 4901  ...s.........-I.
-00000a00: 8804 d408 29d8 2a43 8804 d408 27d8 252b  ....).*C....'.%+
-00000a10: 8804 d508 2272 1a00 0000 7213 0000 0063  ...."r....r....c
-00000a20: 0100 0000 0000 0000 0000 0000 0400 0000  ................
-00000a30: 1300 0000 f33a 0000 0097 0074 0100 0000  .....:.....t....
-00000a40: 0000 0000 007c 0064 01ab 0200 0000 0000  .....|.d........
-00000a50: 0078 0172 0e01 007c 006a 0200 0000 0000  .x.r...|.j......
-00000a60: 0000 0000 0000 0000 0000 0000 0064 0275  .............d.u
-00000a70: 0153 0029 037a 5c0a 2020 2020 2020 2020  .S.).z\.        
-00000a80: 4368 6563 6b20 6966 2074 6865 2069 6e73  Check if the ins
-00000a90: 7461 6e63 6520 7072 6f76 6964 6572 2068  tance provider h
-00000aa0: 6173 2062 6565 6e20 6465 6669 6e65 6420  as been defined 
-00000ab0: 666f 7220 7468 6973 2053 6572 7669 6365  for this Service
-00000ac0: 4465 6669 6e69 7469 6f6e 0a20 2020 2020  Definition.     
-00000ad0: 2020 2072 2f00 0000 4e29 02da 0768 6173     r/...N)...has
-00000ae0: 6174 7472 722f 0000 0072 1f00 0000 7301  attrr/...r....s.
-00000af0: 0000 0020 7217 0000 00da 1d68 6173 5f73  ... r......has_s
-00000b00: 6572 7669 6365 5f69 6e73 7461 6e63 655f  ervice_instance_
-00000b10: 7072 6f76 6964 6572 7a2f 5365 7276 6963  providerz/Servic
-00000b20: 6544 6566 696e 6974 696f 6e2e 6861 735f  eDefinition.has_
-00000b30: 7365 7276 6963 655f 696e 7374 616e 6365  service_instance
-00000b40: 5f70 726f 7669 6465 724a 0000 0073 2700  _providerJ...s'.
-00000b50: 0000 8000 f408 0011 1898 04d0 1e3a d310  .............:..
-00000b60: 3bf2 0002 100a d80c 10d7 0c2b d10c 2bb0  ;..........+..+.
-00000b70: 34d0 0c37 f003 0209 0a72 1a00 0000 6301  4..7.....r....c.
-00000b80: 0000 0000 0000 0000 0000 0003 0000 0013  ................
-00000b90: 0000 00f3 5000 0000 9700 7c00 6a01 0000  ....P.....|.j...
-00000ba0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000bb0: ab00 0000 0000 0000 730b 7403 0000 0000  ........s.t.....
-00000bc0: 0000 0000 6401 ab01 0000 0000 0000 8201  ....d...........
-00000bd0: 7c00 6a04 0000 0000 0000 0000 0000 0000  |.j.............
-00000be0: 0000 0000 0000 5300 2902 7a81 0a20 2020  ......S.).z..   
-00000bf0: 2020 2020 2052 6574 7269 6576 6520 7468       Retrieve th
-00000c00: 6520 7365 7276 6963 6520 696e 7374 616e  e service instan
-00000c10: 6365 2070 726f 7669 6465 7220 666f 7220  ce provider for 
-00000c20: 7468 6973 2053 6572 7669 6365 4465 6669  this ServiceDefi
-00000c30: 6e69 7469 6f6e 0a20 2020 2020 2020 2046  nition.        F
-00000c40: 4958 4d45 202d 2043 6865 636b 2050 7974  IXME - Check Pyt
-00000c50: 686f 6e20 5072 6f70 6572 7479 2073 7570  hon Property sup
-00000c60: 706f 7274 0a20 2020 2020 2020 207a 3967  port.        z9g
-00000c70: 6574 2073 6572 7669 6365 496e 7374 616e  et serviceInstan
-00000c80: 6365 5072 6f76 6964 6572 2063 616c 6c65  ceProvider calle
-00000c90: 6420 7768 656e 206f 6e65 2064 6f65 736e  d when one doesn
-00000ca0: 2774 2065 7869 7374 2903 7234 0000 0072  't exist).r4...r
-00000cb0: 0700 0000 722f 0000 0072 1f00 0000 7301  ....r/...r....s.
-00000cc0: 0000 0020 7217 0000 00da 1d67 6574 5f73  ... r......get_s
-00000cd0: 6572 7669 6365 5f69 6e73 7461 6e63 655f  ervice_instance_
-00000ce0: 7072 6f76 6964 6572 7a2f 5365 7276 6963  providerz/Servic
-00000cf0: 6544 6566 696e 6974 696f 6e2e 6765 745f  eDefinition.get_
-00000d00: 7365 7276 6963 655f 696e 7374 616e 6365  service_instance
-00000d10: 5f70 726f 7669 6465 7252 0000 0073 2e00  _providerR...s..
-00000d20: 0000 8000 f00a 0010 14d7 0f31 d10f 31d4  ...........1..1.
-00000d30: 0f33 dc12 22d8 104b f303 0213 0ef0 0002  .3.."..K........
-00000d40: 0d0e f008 0010 14d7 0f2e d10f 2ed0 082e  ................
-00000d50: 721a 0000 0029 0e72 2200 0000 7223 0000  r....).r"...r#..
-00000d60: 0072 2400 0000 da0f 5f5f 7479 7065 5f70  .r$.....__type_p
-00000d70: 6172 616d 735f 5f72 2500 0000 7209 0000  arams__r%...r...
-00000d80: 0072 0e00 0000 7206 0000 0072 0c00 0000  .r....r....r....
-00000d90: 720a 0000 0072 3100 0000 7227 0000 0072  r....r1...r'...r
-00000da0: 3400 0000 7236 0000 0029 02da 0c2e 7479  4...r6...)....ty
-00000db0: 7065 5f70 6172 616d 7372 0800 0000 7302  pe_paramsr....s.
-00000dc0: 0000 0080 8072 1700 0000 722a 0000 0072  .....r....r*...r
-00000dd0: 2a00 0000 3700 0000 7363 0000 00f8 8700  *...7...sc......
-00000de0: f102 0205 08f0 1600 4801 4c01 d827 42f1  ........H.L..'B.
-00000df0: 0d0a 052c e026 40d9 0c14 906e d00c 24f1  ...,.&@....n..$.
-00000e00: 0302 270a f005 0a05 2cf0 0a00 243b b938  ..'.....,...$;.8
-00000e10: d123 44f0 0b0a 052c f00c 0011 25f3 0d0a  .#D....,....%...
-00000e20: 052c f018 0605 0aa8 74f3 0006 050a f010  .,......t.......
-00000e30: 0a05 2fd0 2f46 c178 d12f 50f4 000a 052f  .././F.x./P..../
-00000e40: 721a 0000 0072 2a00 0000 7215 0000 0029  r....r*...r....)
-00000e50: 03da 0d2e 6765 6e65 7269 635f 6261 7365  ....generic_base
-00000e60: 7238 0000 0072 0800 0000 7303 0000 0020  r8...r....s.... 
-00000e70: 4040 7217 0000 00fa 293c 6765 6e65 7269  @@r.....)<generi
-00000e80: 6320 7061 7261 6d65 7465 7273 206f 6620  c parameters of 
-00000e90: 5365 7276 6963 6544 6566 696e 6974 696f  ServiceDefinitio
-00000ea0: 6e3e 723a 0000 0037 0000 0073 1400 0000  n>r:...7...s....
-00000eb0: f980 009c 08f7 0025 012f f700 2501 2ff1  .......%./..%./.
-00000ec0: 0025 012f 721a 0000 0063 0000 0000 0000  .%./r....c......
-00000ed0: 0000 0000 0000 0d00 0000 0000 0000 f3fe  ................
-00000ee0: 0000 0097 0065 005a 0164 005a 0264 015a  .....e.Z.d.Z.d.Z
-00000ef0: 0364 0284 005a 0409 0064 1564 0465 0564  .d...Z...d.d.e.d
-00000f00: 0565 0665 0765 0866 0219 0000 0064 0665  .e.e.e.f.....d.e
-00000f10: 0964 0764 0866 0864 0984 055a 0a65 0b64  .d.d.f.d...Z.e.d
-00000f20: 0366 0264 0465 0564 0a65 0c65 0719 0000  .f.d.e.d.e.e....
-00000f30: 0064 0565 0665 0765 0866 0219 0000 0064  .d.e.e.e.f.....d
-00000f40: 0b65 0864 0665 0964 0765 0966 0c64 0c84  .e.d.e.d.e.f.d..
-00000f50: 055a 0d65 0b64 0366 0264 0465 0564 0d65  .Z.e.d.f.d.e.d.e
-00000f60: 0e64 0e65 0e64 0b65 0864 0665 0964 0764  .d.e.d.e.d.e.d.d
-00000f70: 0866 0c64 0f84 055a 0f65 0b64 0366 0264  .f.d...Z.e.d.f.d
-00000f80: 0465 0564 0d65 0e64 0b65 0864 0665 0964  .e.d.e.d.e.d.e.d
-00000f90: 0764 0866 0a64 1084 055a 1065 0b66 0164  .d.f.d...Z.e.f.d
-00000fa0: 0465 0564 0b65 0864 0765 0766 0664 1184  .e.d.e.d.e.f.d..
-00000fb0: 055a 1164 0465 0564 0765 0966 0464 1284  .Z.d.e.d.e.f.d..
-00000fc0: 045a 1264 1664 1384 045a 1364 0465 0564  .Z.d.d...Z.d.e.d
-00000fd0: 0665 0964 0764 0866 0664 1484 045a 1479  .e.d.d.f.d...Z.y
-00000fe0: 0829 17da 2144 6566 6175 6c74 5365 7276  .)..!DefaultServ
-00000ff0: 6963 654d 616e 6167 6572 5374 7261 7465  iceManagerStrate
-00001000: 6779 496d 706c 7a7d 0a20 2020 2054 6869  gyImplz}.    Thi
-00001010: 7320 6973 2074 6865 2064 6566 6175 6c74  s is the default
-00001020: 2073 6572 7669 6365 206d 616e 6167 6572   service manager
-00001030: 2073 7472 6174 6567 792e 0a20 2020 2049   strategy..    I
-00001040: 7427 7320 7573 6564 2062 7920 636c 6965  t's used by clie
-00001050: 6e74 7320 746f 2070 726f 6772 616d 6d65  nts to programme
-00001060: 7469 6361 6c6c 7920 7265 6769 7374 6572  tically register
-00001070: 2f64 6566 696e 6520 7365 7276 6963 6573  /define services
-00001080: 0a20 2020 2063 0100 0000 0000 0000 0000  .    c..........
-00001090: 0000 0200 0000 0300 0000 f320 0000 0097  ........... ....
-000010a0: 0069 007c 005f 0000 0000 0000 0000 0069  .i.|._.........i
-000010b0: 007c 005f 0100 0000 0000 0000 0079 0072  .|._.........y.r
-000010c0: 2e00 0000 2902 da20 5f63 6f6e 7472 6f6c  ....).. _control
-000010d0: 6c65 7273 5f66 6f72 5f61 6374 6976 655f  lers_for_active_
-000010e0: 7365 7276 6963 6573 da14 5f73 6572 7669  services.._servi
-000010f0: 6365 5f64 6566 696e 6974 696f 6e73 721f  ce_definitionsr.
-00001100: 0000 0073 0100 0000 2072 1700 0000 7231  ...s.... r....r1
-00001110: 0000 007a 2a44 6566 6175 6c74 5365 7276  ...z*DefaultServ
-00001120: 6963 654d 616e 6167 6572 5374 7261 7465  iceManagerStrate
-00001130: 6779 496d 706c 2e5f 5f69 6e69 745f 5f65  gyImpl.__init__e
-00001140: 0000 0073 1b00 0000 8000 f006 000d 0ff0  ...s............
-00001150: 0500 090d d408 2df0 0600 4d01 4f01 8804  ......-...M.O...
-00001160: d508 2172 1a00 0000 4672 1100 0000 722b  ..!r....Fr....r+
-00001170: 0000 00da 086f 7665 7272 6964 6572 1300  .....overrider..
-00001180: 0000 4e63 0400 0000 0000 0000 0000 0000  ..Nc............
-00001190: 0400 0000 0300 0000 f378 0000 0097 007c  .........x.....|
-000011a0: 017c 006a 0000 0000 0000 0000 0000 0000  .|.j............
-000011b0: 0000 0000 0000 0076 0072 127c 006a 0300  .......v.r.|.j..
-000011c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000011d0: 007c 017c 03ab 0200 0000 0000 0001 0074  .|.|...........t
-000011e0: 0500 0000 0000 0000 007c 02ab 0100 0000  .........|......
-000011f0: 0000 007d 047c 047c 006a 0000 0000 0000  ...}.|.|.j......
-00001200: 0000 0000 0000 0000 0000 0000 007c 013c  .............|.<
-00001210: 0000 0079 0129 0261 6a03 0000 0a20 2020  ...y.).aj....   
-00001220: 2020 2020 2052 6567 6973 7465 7220 6120       Register a 
-00001230: 7365 7276 6963 652e 2020 5468 6973 2069  service.  This i
-00001240: 7320 7468 6520 6d69 6e69 6d61 6c20 6e75  s the minimal nu
-00001250: 6d62 6572 206f 6620 696e 7075 7473 206e  mber of inputs n
-00001260: 6565 6465 6420 746f 2072 6567 6973 7465  eeded to registe
-00001270: 7220 6120 6e65 7720 7365 7276 6963 652e  r a new service.
-00001280: 0a0a 2020 2020 2020 2020 494d 504f 5254  ..        IMPORT
-00001290: 414e 5420 4e4f 5445 3a20 4966 2072 6567  ANT NOTE: If reg
-000012a0: 6973 7465 7269 6e67 2061 206c 6966 6563  istering a lifec
-000012b0: 7963 6c65 2063 6f6e 7472 6f6c 6c65 7220  ycle controller 
-000012c0: 7468 726f 7567 6820 7468 6973 206d 6574  through this met
-000012d0: 686f 642c 2074 6865 2069 6e69 7428 7365  hod, the init(se
-000012e0: 7276 6963 6549 6e73 7461 6e63 6550 726f  rviceInstancePro
-000012f0: 7669 6465 723a 0a20 2020 2020 2020 2053  vider:.        S
-00001300: 6572 7669 6365 496e 7374 616e 6365 5072  erviceInstancePr
-00001310: 6f76 6964 6572 5b54 5d2c 2063 6f6e 6669  ovider[T], confi
-00001320: 673a 2043 2920 6d65 7468 6f64 2077 696c  g: C) method wil
-00001330: 6c20 4e4f 5420 6265 2063 616c 6c65 642e  l NOT be called.
-00001340: 2020 4966 2069 7420 6d75 7374 2062 6520    If it must be 
-00001350: 6361 6c6c 6564 2c20 6974 2073 686f 756c  called, it shoul
-00001360: 6420 6265 2069 6e76 6f6b 6564 2062 790a  d be invoked by.
-00001370: 2020 2020 2020 2020 7468 6520 636c 6965          the clie
-00001380: 6e74 2062 6566 6f72 6520 7265 6769 7374  nt before regist
-00001390: 6572 696e 6720 7468 6520 7365 7276 6963  ering the servic
-000013a0: 650a 0a20 2020 2020 2020 2040 7061 7261  e..        @para
-000013b0: 6d20 6e61 6d65 0a20 2020 2020 2020 2020  m name.         
-000013c0: 2020 2020 2020 2020 2020 2074 6865 206e             the n
-000013d0: 616d 6520 6f66 2074 6865 2064 6566 696e  ame of the defin
-000013e0: 6564 2073 6572 7669 6365 0a20 2020 2020  ed service.     
-000013f0: 2020 2040 7061 7261 6d20 7365 7276 6963     @param servic
-00001400: 654c 6966 6563 7963 6c65 436f 6e74 726f  eLifecycleContro
-00001410: 6c6c 6572 0a20 2020 2020 2020 2020 2020  ller.           
-00001420: 2020 2020 2020 2020 2063 6f6e 7472 6f6c           control
-00001430: 7320 7468 6520 7365 7276 6963 6520 6c69  s the service li
-00001440: 6665 7963 6c65 2e20 466f 7220 6b6e 6f77  feycle. For know
-00001450: 6e20 636f 6e74 726f 6c6c 6572 732c 0a20  n controllers,. 
-00001460: 2020 2020 2020 2073 6565 207b 404b 6e6f         see {@Kno
-00001470: 776e 5365 7276 6963 654c 6966 6563 7963  wnServiceLifecyc
-00001480: 6c65 436f 6e74 726f 6c6c 6572 737d 0a20  leControllers}. 
-00001490: 2020 2020 2020 2040 7061 7261 6d20 6f76         @param ov
-000014a0: 6572 7269 6465 0a20 2020 2020 2020 2020  erride.         
-000014b0: 2020 2020 2020 2020 2020 2041 6e20 6f70             An op
-000014c0: 7469 6f6e 616c 2062 6f6f 6c20 696e 6469  tional bool indi
-000014d0: 6361 7469 6e67 2077 6865 7468 6572 206f  cating whether o
-000014e0: 7220 6e6f 7420 746f 206f 7665 7272 6964  r not to overrid
-000014f0: 6520 616e 0a20 2020 2020 2020 2065 7869  e an.        exi
-00001500: 7374 696e 6720 6465 6669 6e74 696f 6e20  sting defintion 
-00001510: 7769 7468 2074 6865 2073 616d 6520 6e61  with the same na
-00001520: 6d65 2e20 4966 2073 656c 6620 6973 2066  me. If self is f
-00001530: 616c 7365 2061 6e64 2061 2073 6572 7669  alse and a servi
-00001540: 6365 0a20 2020 2020 2020 2064 6566 696e  ce.        defin
-00001550: 6974 696f 6e20 616c 7265 6164 7920 6578  ition already ex
-00001560: 6973 7473 2c20 616e 2065 7272 6f72 2077  ists, an error w
-00001570: 696c 6c20 6265 2074 6872 6f77 6e0a 2020  ill be thrown.  
-00001580: 2020 2020 2020 4ea9 0372 3f00 0000 da18        N..r?.....
-00001590: 5f68 616e 646c 655f 7365 7276 6963 655f  _handle_service_
-000015a0: 6f76 6572 7269 6465 722a 0000 0029 0572  overrider*...).r
-000015b0: 1600 0000 7211 0000 0072 2b00 0000 7240  ....r....r+...r@
-000015c0: 0000 00da 1273 6572 7669 6365 5f64 6566  .....service_def
-000015d0: 696e 6974 696f 6e73 0500 0000 2020 2020  initions....    
-000015e0: 2072 1700 0000 da23 7265 6769 7374 6572   r.....#register
-000015f0: 5f73 6572 7669 6365 5f62 795f 636f 6e74  _service_by_cont
-00001600: 726f 6c6c 6572 5f6f 6e6c 797a 4544 6566  roller_onlyzEDef
-00001610: 6175 6c74 5365 7276 6963 654d 616e 6167  aultServiceManag
-00001620: 6572 5374 7261 7465 6779 496d 706c 2e72  erStrategyImpl.r
-00001630: 6567 6973 7465 725f 7365 7276 6963 655f  egister_service_
-00001640: 6279 5f63 6f6e 7472 6f6c 6c65 725f 6f6e  by_controller_on
-00001650: 6c79 6b00 0000 7342 0000 0080 00f0 3200  lyk...sB......2.
-00001660: 0c10 9034 d713 2cd1 132c d10b 2cd8 0c10  ...4..,..,..,...
-00001670: d70c 29d1 0c29 a824 b008 d40c 39e4 3a4b  ..)..).$....9.:K
-00001680: d80c 28f3 0302 3b0a d008 1af0 0600 2b3d  ..(...;.......+=
-00001690: 8804 d708 21d1 0821 a024 d208 2772 1a00  ....!..!.$..'r..
-000016a0: 0000 722c 0000 0072 1200 0000 6306 0000  ..r,...r....c...
-000016b0: 0000 0000 0000 0000 0005 0000 0003 0000  ................
-000016c0: 00f3 7c00 0000 9700 7c01 7c00 6a00 0000  ..|.....|.|.j...
-000016d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000016e0: 7600 7212 7c00 6a03 0000 0000 0000 0000  v.r.|.j.........
-000016f0: 0000 0000 0000 0000 0000 7c01 7c05 ab02  ..........|.|...
-00001700: 0000 0000 0000 0100 7405 0000 0000 0000  ........t.......
-00001710: 0000 7c03 7c02 7c04 ab03 0000 0000 0000  ..|.|.|.........
-00001720: 7d06 7c06 7c00 6a00 0000 0000 0000 0000  }.|.|.j.........
-00001730: 0000 0000 0000 0000 0000 7c01 3c00 0000  ..........|.<...
-00001740: 7901 2902 7a8c 0a20 2020 2020 2020 2052  y.).z..        R
-00001750: 6567 6973 7465 7220 6120 7365 7276 6963  egister a servic
-00001760: 652c 2070 726f 7669 6469 6e67 2074 6865  e, providing the
-00001770: 2073 6572 7669 6365 206e 616d 652c 2069   service name, i
-00001780: 6e73 7461 6e63 6520 7072 6f76 6964 6572  nstance provider
-00001790: 2c20 6c69 6665 6379 636c 6520 636f 6e74  , lifecycle cont
-000017a0: 726f 6c6c 6572 2061 6e64 0a20 2020 2020  roller and.     
-000017b0: 2020 206f 7074 696f 6e61 6c20 636f 6e66     optional conf
-000017c0: 6967 7572 6174 696f 6e0a 2020 2020 2020  iguration.      
-000017d0: 2020 4e72 4200 0000 2907 7216 0000 0072    NrB...).r....r
-000017e0: 1100 0000 722c 0000 0072 2b00 0000 7212  ....r,...r+...r.
-000017f0: 0000 0072 4000 0000 7244 0000 0073 0700  ...r@...rD...s..
-00001800: 0000 2020 2020 2020 2072 1700 0000 da10  ..       r......
-00001810: 7265 6769 7374 6572 5f73 6572 7669 6365  register_service
-00001820: 7a32 4465 6661 756c 7453 6572 7669 6365  z2DefaultService
-00001830: 4d61 6e61 6765 7253 7472 6174 6567 7949  ManagerStrategyI
-00001840: 6d70 6c2e 7265 6769 7374 6572 5f73 6572  mpl.register_ser
-00001850: 7669 6365 8c00 0000 7347 0000 0080 00f0  vice....sG......
-00001860: 1c00 0c10 9034 d713 2cd1 132c d10b 2cd8  .....4..,..,..,.
-00001870: 0c10 d70c 29d1 0c29 a824 b008 d40c 39e4  ....)..).$....9.
-00001880: 3a4b d80c 28d0 2a43 c056 f303 023b 0ad0  :K..(.*C.V...;..
-00001890: 081a f006 002b 3d88 04d7 0821 d108 21a0  .....+=....!..!.
-000018a0: 24d2 0827 721a 0000 00da 0d73 6572 7669  $..'r......servi
-000018b0: 6365 5f63 6c61 7373 da22 7365 7276 6963  ce_class."servic
-000018c0: 655f 6c69 6665 6379 636c 655f 636f 6e74  e_lifecycle_cont
-000018d0: 726f 6c6c 6572 5f63 6c61 7373 6306 0000  roller_classc...
-000018e0: 0000 0000 0000 0000 0007 0000 0003 0000  ................
-000018f0: 00f3 5200 0000 9700 7401 0000 0000 0000  ..R.....t.......
-00001900: 0000 7c02 ab01 0000 0000 0000 7d06 0200  ..|.........}...
-00001910: 7c03 ab00 0000 0000 0000 7d07 7c00 6a03  |.........}.|.j.
-00001920: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001930: 0000 7c01 7c06 7c07 7c04 7c05 ab05 0000  ..|.|.|.|.|.....
-00001940: 0000 0000 0100 7901 2902 6144 0300 000a  ......y.).aD....
-00001950: 2020 2020 2020 2020 5265 6769 7374 6572          Register
-00001960: 2061 2073 6572 7669 6365 2070 726f 7669   a service provi
-00001970: 6469 6e67 2061 2063 6f6e 7472 7563 746f  ding a contructo
-00001980: 7220 6d65 7468 6f64 2066 6f72 2061 2073  r method for a s
-00001990: 6572 7669 6365 2063 6c61 7373 2061 6e64  ervice class and
-000019a0: 2073 6572 7669 6365 206c 6966 6563 7963   service lifecyc
-000019b0: 6c65 2063 6f6e 7472 6f6c 6c65 7220 636c  le controller cl
-000019c0: 6173 730a 0a20 2020 2020 2020 2040 7061  ass..        @pa
-000019d0: 7261 6d20 6e61 6d65 0a20 2020 2020 2020  ram name.       
-000019e0: 2020 2020 2020 2020 2020 2020 2074 6865               the
-000019f0: 206e 616d 6520 6f66 2074 6865 2064 6566   name of the def
-00001a00: 696e 6564 2073 6572 7669 6365 0a20 2020  ined service.   
-00001a10: 2020 2020 2040 7061 7261 6d20 7365 7276       @param serv
-00001a20: 6963 6543 6c61 7373 0a20 2020 2020 2020  iceClass.       
-00001a30: 2020 2020 2020 2020 2020 2020 2074 6865               the
-00001a40: 2063 6c61 7373 2074 6861 7420 696d 706c   class that impl
-00001a50: 656d 656e 7473 2074 6865 2073 6572 7669  ements the servi
-00001a60: 6365 0a20 2020 2020 2020 2040 7061 7261  ce.        @para
-00001a70: 6d20 7365 7276 6963 654c 6966 6563 7963  m serviceLifecyc
-00001a80: 6c65 436f 6e74 726f 6c6c 6572 436c 6173  leControllerClas
-00001a90: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
-00001aa0: 2020 2020 2020 7468 6520 636c 6173 7320        the class 
-00001ab0: 7468 6174 2063 6f6e 7472 6f6c 7320 7468  that controls th
-00001ac0: 6520 7365 7276 6963 6520 6c69 6665 7963  e service lifeyc
-00001ad0: 6c65 2e20 466f 7220 6b6e 6f77 6e20 636f  le. For known co
-00001ae0: 6e74 726f 6c6c 6572 732c 0a20 2020 2020  ntrollers,.     
-00001af0: 2020 2073 6565 207b 404b 6e6f 776e 5365     see {@KnownSe
-00001b00: 7276 6963 654c 6966 6563 7963 6c65 436f  rviceLifecycleCo
-00001b10: 6e74 726f 6c6c 6572 737d 0a20 2020 2020  ntrollers}.     
-00001b20: 2020 2040 7061 7261 6d20 636f 6e66 6967     @param config
-00001b30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001b40: 2020 2020 2041 6e20 4f70 7469 6f6e 616c       An Optional
-00001b50: 2063 6f6e 6669 6720 6d61 7920 6265 2073   config may be s
-00001b60: 7570 706c 6965 6420 666f 7220 7365 7276  upplied for serv
-00001b70: 6963 6520 6465 6669 6e69 7469 6f6e 206c  ice definition l
-00001b80: 6576 656c 0a20 2020 2020 2020 2063 6f6e  evel.        con
-00001b90: 6669 6775 7261 7469 6f6e 2e0a 2020 2020  figuration..    
-00001ba0: 2020 2020 4070 6172 616d 206f 7665 7272      @param overr
-00001bb0: 6964 650a 2020 2020 2020 2020 2020 2020  ide.            
-00001bc0: 2020 2020 2020 2020 416e 206f 7074 696f          An optio
-00001bd0: 6e61 6c20 626f 6f6c 2069 6e64 6963 6174  nal bool indicat
-00001be0: 696e 6720 7768 6574 6865 7220 6f72 206e  ing whether or n
-00001bf0: 6f74 2074 6f20 6f76 6572 7269 6465 2061  ot to override a
-00001c00: 6e0a 2020 2020 2020 2020 6578 6973 7469  n.        existi
-00001c10: 6e67 2064 6566 696e 7469 6f6e 2077 6974  ng defintion wit
-00001c20: 6820 7468 6520 7361 6d65 206e 616d 652e  h the same name.
-00001c30: 2049 6620 7365 6c66 2069 7320 6661 6c73   If self is fals
-00001c40: 6520 616e 6420 6120 7365 7276 6963 650a  e and a service.
-00001c50: 2020 2020 2020 2020 6465 6669 6e69 7469          definiti
-00001c60: 6f6e 2061 6c72 6561 6479 2065 7869 7374  on already exist
-00001c70: 732c 2061 6e20 6572 726f 7220 7769 6c6c  s, an error will
-00001c80: 2062 6520 7468 726f 776e 0a20 2020 2020   be thrown.     
-00001c90: 2020 204e 2902 720b 0000 0072 4700 0000     N).r....rG...
-00001ca0: 2908 7216 0000 0072 1100 0000 7248 0000  ).r....r....rH..
-00001cb0: 0072 4900 0000 7212 0000 0072 4000 0000  .rI...r....r@...
-00001cc0: da10 7365 7276 6963 655f 7072 6f76 6964  ..service_provid
-00001cd0: 6572 722b 0000 0073 0800 0000 2020 2020  err+...s....    
-00001ce0: 2020 2020 7217 0000 00da 1972 6567 6973      r......regis
-00001cf0: 7465 725f 7365 7276 6963 655f 6279 5f63  ter_service_by_c
-00001d00: 6c61 7373 7a3b 4465 6661 756c 7453 6572  lassz;DefaultSer
-00001d10: 7669 6365 4d61 6e61 6765 7253 7472 6174  viceManagerStrat
-00001d20: 6567 7949 6d70 6c2e 7265 6769 7374 6572  egyImpl.register
-00001d30: 5f73 6572 7669 6365 5f62 795f 636c 6173  _service_by_clas
-00001d40: 73a3 0000 0073 3300 0000 8000 f436 001c  s....s3......6..
-00001d50: 3eb8 6dd3 1b4c d008 18d9 2749 d327 4bd0  >.m..L....'I.'K.
-00001d60: 0824 d808 0cd7 081d d108 1dd8 0c10 d012  .$..............
-00001d70: 22d0 2440 c026 c828 f503 0209 0a72 1a00  ".$@.&.(.....r..
-00001d80: 0000 6305 0000 0000 0000 0000 0000 0007  ..c.............
-00001d90: 0000 0003 0000 00f3 4a00 0000 9700 7c00  ........J.....|.
-00001da0: 6a01 0000 0000 0000 0000 0000 0000 0000  j...............
-00001db0: 0000 0000 7c01 7c02 7402 0000 0000 0000  ....|.|.t.......
-00001dc0: 0000 6a04 0000 0000 0000 0000 0000 0000  ..j.............
-00001dd0: 0000 0000 0000 7c03 7c04 ab05 0000 0000  ......|.|.......
-00001de0: 0000 0100 7901 2902 616d 0200 000a 2020  ....y.).am....  
-00001df0: 2020 2020 2020 5265 6769 7374 6572 2061        Register a
-00001e00: 2073 6572 7669 6365 2074 6861 7420 6861   service that ha
-00001e10: 7320 6120 7369 6e67 6c65 746f 6e20 6c69  s a singleton li
-00001e20: 6665 6379 636c 6520 286f 6e6c 7920 6f6e  fecycle (only on
-00001e30: 6520 696e 7374 616e 6365 2065 7869 7374  e instance exist
-00001e40: 7329 0a0a 2020 2020 2020 2020 4070 6172  s)..        @par
-00001e50: 616d 206e 616d 650a 2020 2020 2020 2020  am name.        
-00001e60: 2020 2020 2020 2020 2020 2020 7468 6520              the 
-00001e70: 6e61 6d65 206f 6620 7468 6520 6465 6669  name of the defi
-00001e80: 6e65 6420 7365 7276 6963 650a 2020 2020  ned service.    
-00001e90: 2020 2020 4070 6172 616d 2073 6572 7669      @param servi
-00001ea0: 6365 436c 6173 730a 2020 2020 2020 2020  ceClass.        
-00001eb0: 2020 2020 2020 2020 2020 2020 7468 6520              the 
-00001ec0: 636c 6173 7320 7468 6174 2069 6d70 6c65  class that imple
-00001ed0: 6d65 6e74 7320 7468 6520 7365 7276 6963  ments the servic
-00001ee0: 650a 2020 2020 2020 2020 4070 6172 616d  e.        @param
-00001ef0: 2063 6f6e 6669 670a 2020 2020 2020 2020   config.        
-00001f00: 2020 2020 2020 2020 2020 2020 416e 204f              An O
-00001f10: 7074 696f 6e61 6c20 636f 6e66 6967 206d  ptional config m
-00001f20: 6179 2062 6520 7375 7070 6c69 6564 2066  ay be supplied f
-00001f30: 6f72 2073 6572 7669 6365 2064 6566 696e  or service defin
-00001f40: 6974 696f 6e20 6c65 7665 6c0a 2020 2020  ition level.    
-00001f50: 2020 2020 636f 6e66 6967 7572 6174 696f      configuratio
-00001f60: 6e2e 0a20 2020 2020 2020 2040 7061 7261  n..        @para
-00001f70: 6d20 6f76 6572 7269 6465 0a20 2020 2020  m override.     
-00001f80: 2020 2020 2020 2020 2020 2020 2020 2041                 A
-00001f90: 6e20 6f70 7469 6f6e 616c 2062 6f6f 6c20  n optional bool 
-00001fa0: 696e 6469 6361 7469 6e67 2077 6865 7468  indicating wheth
-00001fb0: 6572 206f 7220 6e6f 7420 746f 206f 7665  er or not to ove
-00001fc0: 7272 6964 6520 616e 0a20 2020 2020 2020  rride an.       
-00001fd0: 2065 7869 7374 696e 6720 6465 6669 6e74   existing defint
-00001fe0: 696f 6e20 7769 7468 2074 6865 2073 616d  ion with the sam
-00001ff0: 6520 6e61 6d65 2e20 4966 2073 656c 6620  e name. If self 
-00002000: 6973 2066 616c 7365 2061 6e64 2061 2073  is false and a s
-00002010: 6572 7669 6365 0a20 2020 2020 2020 2064  ervice.        d
-00002020: 6566 696e 6974 696f 6e20 616c 7265 6164  efinition alread
-00002030: 7920 6578 6973 7473 2c20 616e 2065 7272  y exists, an err
-00002040: 6f72 2077 696c 6c20 6265 2074 6872 6f77  or will be throw
-00002050: 6e0a 2020 2020 2020 2020 4e29 0372 4c00  n.        N).rL.
-00002060: 0000 720d 0000 00da 0953 494e 474c 4554  ..r......SINGLET
-00002070: 4f4e 2905 7216 0000 0072 1100 0000 7248  ON).r....r....rH
-00002080: 0000 0072 1200 0000 7240 0000 0073 0500  ...r....r@...s..
-00002090: 0000 2020 2020 2072 1700 0000 da1a 7265  ..     r......re
-000020a0: 6769 7374 6572 5f73 696e 676c 6574 6f6e  gister_singleton
-000020b0: 5f73 6572 7669 6365 7a3c 4465 6661 756c  _servicez<Defaul
-000020c0: 7453 6572 7669 6365 4d61 6e61 6765 7253  tServiceManagerS
-000020d0: 7472 6174 6567 7949 6d70 6c2e 7265 6769  trategyImpl.regi
-000020e0: 7374 6572 5f73 696e 676c 6574 6f6e 5f73  ster_singleton_s
-000020f0: 6572 7669 6365 c400 0000 7327 0000 0080  ervice....s'....
-00002100: 00f0 2c00 090d d708 26d1 0826 d80c 10d8  ..,.....&..&....
-00002110: 0c19 dc0c 2cd7 0c36 d10c 36d8 0c12 d80c  ....,..6..6.....
-00002120: 14f5 0b06 090a 721a 0000 0063 0300 0000  ......r....c....
-00002130: 0000 0000 0000 0000 0400 0000 0300 0000  ................
-00002140: f37c 0100 0097 007c 017c 006a 0000 0000  .|.....|.|.j....
-00002150: 0000 0000 0000 0000 0000 0000 0000 0076  ...............v
-00002160: 0172 0e74 0300 0000 0000 0000 0064 017c  .r.t.........d.|
-00002170: 017a 0000 00ab 0100 0000 0000 0082 017c  .z.............|
-00002180: 017c 006a 0400 0000 0000 0000 0000 0000  .|.j............
-00002190: 0000 0000 0000 0076 0072 1f7c 006a 0400  .......v.r.|.j..
-000021a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000021b0: 007c 0119 0000 007d 037c 036a 1100 0000  .|.....}.|.j....
-000021c0: 0000 0000 0000 0000 0000 0000 0000 00ab  ................
-000021d0: 0000 0000 0000 0053 007c 006a 0000 0000  .......S.|.j....
-000021e0: 0000 0000 0000 0000 0000 0000 0000 007c  ...............|
-000021f0: 0119 0000 007d 047c 046a 0600 0000 0000  .....}.|.j......
-00002200: 0000 0000 0000 0000 0000 0000 007d 037c  .............}.|
-00002210: 046a 0900 0000 0000 0000 0000 0000 0000  .j..............
-00002220: 0000 0000 00ab 0000 0000 0000 0072 2a7c  .............r*|
-00002230: 036a 0b00 0000 0000 0000 0000 0000 0000  .j..............
-00002240: 0000 0000 007c 046a 0d00 0000 0000 0000  .....|.j........
-00002250: 0000 0000 0000 0000 0000 00ab 0000 0000  ................
-00002260: 0000 007c 046a 0e00 0000 0000 0000 0000  ...|.j..........
-00002270: 0000 0000 0000 0000 00ab 0200 0000 0000  ................
-00002280: 0001 007c 037c 006a 0400 0000 0000 0000  ...|.|.j........
-00002290: 0000 0000 0000 0000 0000 007c 013c 0000  ...........|.<..
-000022a0: 007c 036a 1100 0000 0000 0000 0000 0000  .|.j............
-000022b0: 0000 0000 0000 00ab 0000 0000 0000 0053  ...............S
-000022c0: 0029 024e 7a15 5365 7276 6963 6520 6e6f  .).Nz.Service no
-000022d0: 7420 6465 6669 6e65 643a 2029 0972 3f00  t defined: ).r?.
-000022e0: 0000 7207 0000 0072 3e00 0000 722b 0000  ..r....r>...r+..
-000022f0: 0072 3400 0000 da04 696e 6974 7236 0000  .r4.....initr6..
-00002300: 0072 3000 0000 7218 0000 0029 0572 1600  .r0...r....).r..
-00002310: 0000 7211 0000 0072 1200 0000 722b 0000  ..r....r....r+..
-00002320: 0072 4400 0000 7305 0000 0020 2020 2020  .rD...s....     
-00002330: 7217 0000 0072 1800 0000 7a2d 4465 6661  r....r....z-Defa
-00002340: 756c 7453 6572 7669 6365 4d61 6e61 6765  ultServiceManage
-00002350: 7253 7472 6174 6567 7949 6d70 6c2e 6765  rStrategyImpl.ge
-00002360: 745f 7365 7276 6963 65e2 0000 0073 d000  t_service....s..
-00002370: 0000 8000 f00c 000c 1090 74d7 1730 d117  ..........t..0..
-00002380: 30d1 0b30 dc12 22d0 233a b854 d123 41d3  0..0..".#:.T.#A.
-00002390: 1242 d00c 42f0 0600 0c10 9034 d713 38d1  .B..B......4..8.
-000023a0: 1338 d10b 38d8 2b2f d72b 50d1 2b50 d051  .8..8.+/.+P.+P.Q
-000023b0: 55d1 2b56 d00c 28f0 2200 102c d70f 37d1  U.+V..(."..,..7.
-000023c0: 0f37 d30f 39d0 0839 f01f 003f 4301 d73e  .7..9..9...?C..>
-000023d0: 57d1 3e57 d810 14f1 0302 3f0e d00c 1ef0  W.>W......?.....
-000023e0: 0800 1123 d710 3fd1 103f f003 000d 29f0  ...#..?..?....).
-000023f0: 0800 1022 d70f 3fd1 0f3f d40f 41d8 102c  ..."..?..?..A..,
-00002400: d710 31d1 1031 d814 26d7 1444 d114 44d3  ..1..1..&..D..D.
-00002410: 1446 d814 26d7 143c d114 3cf4 0503 1112  .F..&..<..<.....
-00002420: f00a 003b 5701 8844 d70c 31d1 0c31 b024  ...;W..D..1..1.$
-00002430: d10c 37e0 0f2b d70f 37d1 0f37 d30f 39d0  ..7..+..7..7..9.
-00002440: 0839 721a 0000 0063 0200 0000 0000 0000  .9r....c........
-00002450: 0000 0000 0200 0000 0300 0000 f31e 0000  ................
-00002460: 0097 007c 017c 006a 0000 0000 0000 0000  ...|.|.j........
-00002470: 0000 0000 0000 0000 0000 0076 0053 0072  ...........v.S.r
-00002480: 2e00 0000 2901 723f 0000 0072 1c00 0000  ....).r?...r....
-00002490: 7302 0000 0020 2072 1700 0000 721d 0000  s....  r....r...
-000024a0: 007a 3444 6566 6175 6c74 5365 7276 6963  .z4DefaultServic
-000024b0: 654d 616e 6167 6572 5374 7261 7465 6779  eManagerStrategy
-000024c0: 496d 706c 2e69 735f 7365 7276 6963 655f  Impl.is_service_
-000024d0: 6465 6669 6e65 6400 0100 0073 1300 0000  defined....s....
-000024e0: 8000 d80f 1390 74d7 1730 d117 30d0 0f30  ......t..0..0..0
-000024f0: d008 3072 1a00 0000 6301 0000 0000 0000  ..0r....c.......
-00002500: 0000 0000 0003 0000 0003 0000 00f3 ca00  ................
-00002510: 0000 9700 7c00 6a00 0000 0000 0000 0000  ....|.j.........
-00002520: 0000 0000 0000 0000 0000 6a03 0000 0000  ..........j.....
-00002530: 0000 0000 0000 0000 0000 0000 0000 ab00  ................
-00002540: 0000 0000 0000 4400 5d12 0000 7d01 7c01  ......D.]...}.|.
-00002550: 6a05 0000 0000 0000 0000 0000 0000 0000  j...............
-00002560: 0000 0000 ab00 0000 0000 0000 0100 8c14  ................
-00002570: 0400 7c00 6a00 0000 0000 0000 0000 0000  ..|.j...........
-00002580: 0000 0000 0000 0000 6a07 0000 0000 0000  ........j.......
-00002590: 0000 0000 0000 0000 0000 0000 ab00 0000  ................
-000025a0: 0000 0000 0100 7c00 6a08 0000 0000 0000  ......|.j.......
-000025b0: 0000 0000 0000 0000 0000 0000 6a07 0000  ............j...
-000025c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000025d0: ab00 0000 0000 0000 0100 7900 722e 0000  ..........y.r...
-000025e0: 0029 0572 3e00 0000 da06 7661 6c75 6573  .).r>.....values
-000025f0: 7220 0000 00da 0563 6c65 6172 723f 0000  r .....clearr?..
-00002600: 0029 0272 1600 0000 da17 6e65 7874 5f73  .).r......next_s
-00002610: 6572 7669 6365 5f63 6f6e 7472 6f6c 6c65  ervice_controlle
-00002620: 7273 0200 0000 2020 7217 0000 0072 2000  rs....  r....r .
-00002630: 0000 7a2a 4465 6661 756c 7453 6572 7669  ..z*DefaultServi
-00002640: 6365 4d61 6e61 6765 7253 7472 6174 6567  ceManagerStrateg
-00002650: 7949 6d70 6c2e 7368 7574 646f 776e 0301  yImpl.shutdown..
-00002660: 0000 7353 0000 0080 00d8 272b d727 4cd1  ..sS......'+.'L.
-00002670: 274c d727 53d1 2753 d327 55f2 0001 092f  'L.'S.'S.'U..../
-00002680: d00c 23d8 0c23 d70c 2cd1 0c2c d50c 2ef0  ..#..#..,..,....
-00002690: 0301 092f f006 0009 0dd7 082d d108 2dd7  .../.......-..-.
-000026a0: 0833 d108 33d4 0835 d808 0cd7 0821 d108  .3..3..5.....!..
-000026b0: 21d7 0827 d108 27d5 0829 721a 0000 0063  !..'..'..)r....c
-000026c0: 0300 0000 0000 0000 0000 0000 0400 0000  ................
-000026d0: 0300 0000 f3ba 0000 0097 007c 0272 497c  ...........|.rI|
-000026e0: 006a 0000 0000 0000 0000 0000 0000 0000  .j..............
-000026f0: 0000 0000 007c 013d 007c 017c 006a 0200  .....|.=.|.|.j..
-00002700: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002710: 0076 0072 2d7c 006a 0200 0000 0000 0000  .v.r-|.j........
-00002720: 0000 0000 0000 0000 0000 007c 0119 0000  ...........|....
-00002730: 007d 037c 036a 0500 0000 0000 0000 0000  .}.|.j..........
-00002740: 0000 0000 0000 0000 00ab 0000 0000 0000  ................
-00002750: 0001 007c 006a 0200 0000 0000 0000 0000  ...|.j..........
-00002760: 0000 0000 0000 0000 007c 013d 0079 0079  .........|.=.y.y
-00002770: 0074 0700 0000 0000 0000 0064 017c 017a  .t.........d.|.z
-00002780: 0000 0064 027a 0000 00ab 0100 0000 0000  ...d.z..........
-00002790: 0082 0129 034e 7a14 5365 7276 6963 6520  ...).Nz.Service 
-000027a0: 7769 7468 206e 616d 652c 203a 7a45 2c20  with name, :zE, 
-000027b0: 6973 2061 6c72 6561 6479 2064 6566 696e  is already defin
-000027c0: 6564 2e20 2053 7065 6369 6679 206f 7665  ed.  Specify ove
-000027d0: 7272 6964 653d 7472 7565 2069 6620 6974  rride=true if it
-000027e0: 2073 686f 756c 6420 6265 2072 6570 6c61   should be repla
-000027f0: 6365 6429 0472 3f00 0000 723e 0000 0072  ced).r?...r>...r
-00002800: 2000 0000 7207 0000 0029 0472 1600 0000   ...r....).r....
-00002810: 7211 0000 0072 4000 0000 da14 636f 6e74  r....r@.....cont
-00002820: 726f 6c6c 6572 5f74 6f5f 7265 6d6f 7665  roller_to_remove
-00002830: 7304 0000 0020 2020 2072 1700 0000 7243  s....    r....rC
-00002840: 0000 007a 3a44 6566 6175 6c74 5365 7276  ...z:DefaultServ
-00002850: 6963 654d 616e 6167 6572 5374 7261 7465  iceManagerStrate
-00002860: 6779 496d 706c 2e5f 6861 6e64 6c65 5f73  gyImpl._handle_s
-00002870: 6572 7669 6365 5f6f 7665 7272 6964 650a  ervice_override.
-00002880: 0100 0073 7400 0000 8000 d90b 13e0 1014  ...st...........
-00002890: d710 29d1 1029 a824 d010 2fd8 0f13 9074  ..)..).$../....t
-000028a0: d717 3cd1 173c d10f 3cd8 272b d727 4cd1  ..<..<..<.'+.'L.
-000028b0: 274c c854 d127 52d0 1024 d810 24d7 102d  'L.T.'R..$..$..-
-000028c0: d110 2dd4 102f d814 18d7 1439 d114 39b8  ..-../.....9..9.
-000028d0: 24d1 143f f007 0010 3df4 0a00 1323 d810  $..?....=....#..
-000028e0: 26d8 1216 f103 0111 17e0 1259 f105 0211  &..........Y....
-000028f0: 5a01 f303 0413 0ef0 0004 0d0e 721a 0000  Z...........r...
-00002900: 0029 0146 7221 0000 0029 1572 2200 0000  .).Fr!...).r"...
-00002910: 7223 0000 0072 2400 0000 7225 0000 0072  r#...r$...r%...r
-00002920: 3100 0000 7226 0000 0072 0e00 0000 7208  1...r&...r....r.
-00002930: 0000 0072 0600 0000 7227 0000 0072 4500  ...r....r'...rE.
-00002940: 0000 7209 0000 0072 0c00 0000 7247 0000  ..r....r....rG..
-00002950: 00da 0474 7970 6572 4c00 0000 724f 0000  ...typerL...rO..
-00002960: 0072 1800 0000 721d 0000 0072 2000 0000  .r....r....r ...
-00002970: 7243 0000 0072 1500 0000 721a 0000 0072  rC...r....r....r
-00002980: 1700 0000 723c 0000 0072 3c00 0000 5f00  ....r<...r<..._.
-00002990: 0000 7380 0100 0084 00f1 0203 0508 f20a  ..s.............
-000029a0: 0405 4f01 f018 001a 1ff1 0d1f 053d e00e  ..O..........=..
-000029b0: 11f0 051f 053d f006 0027 4101 d80c 1490  .....=...'A.....
-000029c0: 6ed0 0c24 f103 0227 0af0 071f 053d f00c  n..$...'.....=..
-000029d0: 0013 17f0 0d1f 053d f00e 000a 0ef3 0f1f  .......=........
-000029e0: 053d f050 0100 223d d819 1ef1 1114 053d  .=.P.."=.......=
-000029f0: e00e 11f0 0514 053d f006 0024 3bb8 38d1  .......=...$;.8.
-00002a00: 2344 f007 1405 3df0 0800 2741 01d8 0c14  #D....=...'A....
-00002a10: 906e d00c 24f1 0302 270a f009 1405 3df0  .n..$...'.....=.
-00002a20: 0e00 111f f00f 1405 3df0 1000 1317 f011  ........=.......
-00002a30: 1405 3df0 1200 0a0e f313 1405 3df0 3800  ..=.........=.8.
-00002a40: 223d d819 1ef1 0d1f 050a e00e 11f0 051f  "=..............
-00002a50: 050a f006 0018 1cf0 071f 050a f008 002d  ...............-
-00002a60: 31f0 091f 050a f00a 0011 1ff0 0b1f 050a  1...............
-00002a70: f00c 0013 17f0 0d1f 050a f00e 000a 0ef3  ................
-00002a80: 0f1f 050a f04a 0100 223d d819 1ef1 0b1c  .....J.."=......
-00002a90: 050a e00e 11f0 051c 050a f006 0018 1cf0  ................
-00002aa0: 071c 050a f008 0011 1ff0 091c 050a f00a  ................
-00002ab0: 0013 17f0 0b1c 050a f00c 000a 0ef3 0d1c  ................
-00002ac0: 050a f03e 0033 4e01 f103 1c05 3ad8 1417  ...>.3N.....:...
-00002ad0: f003 1c05 3ad8 212f f003 1c05 3ae0 0911  ....:.!/....:...
-00002ae0: f305 1c05 3af0 3c01 0531 a073 f000 0105  ....:.<..1.s....
-00002af0: 31a8 74f3 0001 0531 f306 0505 2af0 0e0d  1.t....1....*...
-00002b00: 050e a853 f000 0d05 0eb8 44f0 000d 050e  ...S......D.....
-00002b10: c054 f400 0d05 0e72 1a00 0000 723c 0000  .T.....r....r<..
-00002b20: 0063 0000 0000 0000 0000 0000 0000 0100  .c..............
-00002b30: 0000 0000 0000 f310 0000 0097 0065 005a  .............e.Z
-00002b40: 0164 005a 0264 015a 0379 0229 03da 1c43  .d.Z.d.Z.y.)...C
-00002b50: 6f6e 6669 6753 6572 7669 6365 4d61 6e61  onfigServiceMana
-00002b60: 6765 7253 7472 6174 6567 797a 690a 2020  gerStrategyzi.  
-00002b70: 2020 4120 7374 7261 7465 6779 2074 6861    A strategy tha
-00002b80: 7420 7265 6164 7320 7365 7276 6963 6520  t reads service 
-00002b90: 636f 6e66 6967 7572 6174 696f 6e20 6672  configuration fr
-00002ba0: 6f6d 2073 6572 7669 6365 436f 6e66 6967  om serviceConfig
-00002bb0: 2e6a 736f 6e2e 2020 4649 584d 4520 2d20  .json.  FIXME - 
-00002bc0: 546f 2042 6520 496d 706c 656d 656e 7465  To Be Implemente
-00002bd0: 640a 2020 2020 4e29 0472 2200 0000 7223  d.    N).r"...r#
-00002be0: 0000 0072 2400 0000 7225 0000 0072 1500  ...r$...r%...r..
-00002bf0: 0000 721a 0000 0072 1700 0000 725b 0000  ..r....r....r[..
-00002c00: 0072 5b00 0000 1c01 0000 7307 0000 0084  .r[.......s.....
-00002c10: 00f2 0202 0508 721a 0000 0072 5b00 0000  ......r....r[...
-00002c20: 4e29 1772 2500 0000 da03 6162 6372 0300  N).r%.....abcr..
-00002c30: 0000 7204 0000 00da 0674 7970 696e 6772  ..r......typingr
-00002c40: 0500 0000 da1f 7370 6879 726e 612e 7365  ......sphyrna.se
-00002c50: 7276 6963 655f 6d61 6e61 6765 722e 7365  rvice_manager.se
-00002c60: 7276 6963 6572 0600 0000 7207 0000 0072  rvicer....r....r
-00002c70: 0800 0000 da2d 7370 6879 726e 612e 7365  .....-sphyrna.se
-00002c80: 7276 6963 655f 6d61 6e61 6765 722e 7365  rvice_manager.se
-00002c90: 7276 6963 655f 636f 6e66 6967 7572 6174  rvice_configurat
-00002ca0: 696f 6e72 0900 0000 720a 0000 00da 3173  ionr....r.....1s
-00002cb0: 7068 7972 6e61 2e73 6572 7669 6365 5f6d  phyrna.service_m
-00002cc0: 616e 6167 6572 2e73 6572 7669 6365 5f69  anager.service_i
-00002cd0: 6e73 7461 6e63 655f 7072 6f76 6964 6572  nstance_provider
-00002ce0: 720b 0000 0072 0c00 0000 da34 7370 6879  r....r.....4sphy
-00002cf0: 726e 612e 7365 7276 6963 655f 6d61 6e61  rna.service_mana
-00002d00: 6765 722e 7365 7276 6963 655f 6c69 6665  ger.service_life
-00002d10: 6379 636c 655f 636f 6e74 726f 6c6c 6572  cycle_controller
-00002d20: 720d 0000 0072 0e00 0000 7210 0000 0072  r....r....r....r
-00002d30: 2a00 0000 723c 0000 0072 5b00 0000 7215  *...r<...r[...r.
-00002d40: 0000 0072 1a00 0000 7217 0000 00fa 083c  ...r....r......<
-00002d50: 6d6f 6475 6c65 3e72 6200 0000 0100 0000  module>rb.......
-00002d60: 7356 0000 00f0 0301 0101 f102 0301 04f7  sV..............
-00002d70: 0a00 0124 dd00 17e7 0056 d100 56f7 0203  ...$.....V..V...
-00002d80: 0102 f708 0301 02f7 0803 0102 f40c 1b01  ................
-00002d90: 0c98 53f4 001b 010c f73e 2501 2ff4 5001  ..S......>%./.P.
-00002da0: 7802 010e d028 3ef4 0078 0201 0ef4 7a05  x....(>..x....z.
-00002db0: 0301 08d0 2344 f500 0301 0872 1a00 0000  ....#D.....r....
+00000490: 832f 5573 6572 732f 6b61 6d65 6c65 6f6e  ./Users/kameleon
+000004a0: 2f43 6f64 652f 7365 7276 6963 652f 7461  /Code/service/ta
+000004b0: 7267 6574 2f63 6865 636b 6f75 742f 7061  rget/checkout/pa
+000004c0: 636b 6167 6573 2f70 7974 686f 6e6c 6962  ckages/pythonlib
+000004d0: 2f73 7263 2f6d 6169 6e2f 7079 7468 6f6e  /src/main/python
+000004e0: 2f73 7068 7972 6e61 2f73 6572 7669 6365  /sphyrna/service
+000004f0: 5f6d 616e 6167 6572 2f73 6572 7669 6365  _manager/service
+00000500: 5f6d 616e 6167 6572 5f73 7472 6174 6567  _manager_strateg
+00000510: 792e 7079 da0b 6765 745f 7365 7276 6963  y.py..get_servic
+00000520: 657a 2253 6572 7669 6365 4d61 6e61 6765  ez"ServiceManage
+00000530: 7253 7472 6174 6567 792e 6765 745f 7365  rStrategy.get_se
+00000540: 7276 6963 651d 0000 00f3 0200 0000 8100  rvice...........
+00000550: f300 0000 0063 0200 0000 0000 0000 0000  .....c..........
+00000560: 0000 0000 0000 0300 0000 f304 0000 0097  ................
+00000570: 0079 0129 027a 510a 2020 2020 2020 2020  .y.).zQ.        
+00000580: 4465 7465 726d 696e 6520 6966 2061 2073  Determine if a s
+00000590: 6572 7669 6365 2077 6974 6820 7468 6520  ervice with the 
+000005a0: 7370 6563 6966 6965 6420 6e61 6d65 2068  specified name h
+000005b0: 6173 2062 6565 6e20 6465 6669 6e65 640a  as been defined.
+000005c0: 2020 2020 2020 2020 4e72 1500 0000 a902          Nr......
+000005d0: 7216 0000 0072 1100 0000 7302 0000 0020  r....r....s.... 
+000005e0: 2072 1700 0000 da12 6973 5f73 6572 7669   r......is_servi
+000005f0: 6365 5f64 6566 696e 6564 7a29 5365 7276  ce_definedz)Serv
+00000600: 6963 654d 616e 6167 6572 5374 7261 7465  iceManagerStrate
+00000610: 6779 2e69 735f 7365 7276 6963 655f 6465  gy.is_service_de
+00000620: 6669 6e65 6429 0000 0072 1900 0000 721a  fined)...r....r.
+00000630: 0000 004e 6301 0000 0000 0000 0000 0000  ...Nc...........
+00000640: 0000 0000 0003 0000 00f3 0400 0000 9700  ................
+00000650: 7901 2902 7a49 0a20 2020 2020 2020 2053  y.).zI.        S
+00000660: 6875 7464 6f77 6e20 7468 6520 5365 7276  hutdown the Serv
+00000670: 6963 654d 616e 6167 6572 2061 6e64 2061  iceManager and a
+00000680: 6c6c 2061 7373 6f63 6961 7465 6420 7365  ll associated se
+00000690: 7276 6963 6573 0a20 2020 2020 2020 204e  rvices.        N
+000006a0: 7215 0000 00a9 0172 1600 0000 7301 0000  r......r....s...
+000006b0: 0020 7217 0000 00da 0873 6875 7464 6f77  . r......shutdow
+000006c0: 6e7a 1f53 6572 7669 6365 4d61 6e61 6765  nz.ServiceManage
+000006d0: 7253 7472 6174 6567 792e 7368 7574 646f  rStrategy.shutdo
+000006e0: 776e 2f00 0000 7219 0000 0072 1a00 0000  wn/...r....r....
+000006f0: a902 7213 0000 004e 290d da08 5f5f 6e61  ..r....N)...__na
+00000700: 6d65 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f  me__..__module__
+00000710: da0c 5f5f 7175 616c 6e61 6d65 5f5f da07  ..__qualname__..
+00000720: 5f5f 646f 635f 5f72 0400 0000 7209 0000  __doc__r....r...
+00000730: 00da 0373 7472 7206 0000 0072 0800 0000  ...strr....r....
+00000740: 7218 0000 00da 0462 6f6f 6c72 1d00 0000  r......boolr....
+00000750: 7220 0000 0072 1500 0000 721a 0000 0072  r ...r....r....r
+00000760: 1700 0000 7210 0000 0072 1000 0000 1800  ....r....r......
+00000770: 0000 736c 0000 0084 00f1 0202 0508 f008  ..sl............
+00000780: 0006 14e0 324d f103 0905 0cd8 1417 f003  ....2M..........
+00000790: 0905 0cd8 212f f003 0905 0ce0 0911 f205  ....!/..........
+000007a0: 0905 0cf3 0300 0614 f002 0905 0cf0 1600  ................
+000007b0: 0614 f002 0305 0ca0 73f0 0003 050c a874  ........s......t
+000007c0: f200 0305 0cf3 0300 0614 f002 0305 0cf0  ................
+000007d0: 0a00 0614 f202 0305 0cf3 0300 0614 f102  ................
+000007e0: 0305 0c72 1a00 0000 7210 0000 0063 0000  ...r....r....c..
+000007f0: 0000 0000 0000 0000 0000 0500 0000 0300  ................
+00000800: 0000 f334 0000 0087 0187 0297 0064 00ad  ...4.........d..
+00000810: 0778 018a 0266 018a 0102 0047 0088 0188  .x...f.....G....
+00000820: 0266 0264 0184 0864 0289 01ad 0a7d 007c  .f.d...d.....}.|
+00000830: 00ab 0300 0000 0000 0053 0029 0372 0800  .........S.).r..
+00000840: 0000 6300 0000 0000 0000 0000 0000 0007  ..c.............
+00000850: 0000 0000 0000 00f3 6600 0000 9502 9700  ........f.......
+00000860: 6500 5a01 6400 5a02 5700 b000 5a03 6401  e.Z.d.Z.W...Z.d.
+00000870: 5a04 6402 6505 6602 6403 6506 5700 b001  Z.d.e.f.d.e.W...
+00000880: 6507 6602 1900 0000 6404 6508 5700 b001  e.f.....d.e.W...
+00000890: 1900 0000 6405 6509 6606 6406 8405 5a0a  ....d.e.f.d...Z.
+000008a0: 6407 650b 6602 6408 8404 5a0c 6407 6508  d.e.f.d...Z.d.e.
+000008b0: 5700 b001 1900 0000 6602 6409 8404 5a0d  W.......f.d...Z.
+000008c0: 7902 290a da11 5365 7276 6963 6544 6566  y.)...ServiceDef
+000008d0: 696e 6974 696f 6e7a 180a 2020 2020 496e  initionz..    In
+000008e0: 7465 726e 616c 2063 6c61 7373 0a20 2020  ternal class.   
+000008f0: 204e da1c 7365 7276 6963 655f 6c69 6665   N..service_life
+00000900: 6379 636c 655f 636f 6e74 726f 6c6c 6572  cycle_controller
+00000910: da19 7365 7276 6963 655f 696e 7374 616e  ..service_instan
+00000920: 6365 5f70 726f 7669 6465 7272 1200 0000  ce_providerr....
+00000930: 6304 0000 0000 0000 0000 0000 0002 0000  c...............
+00000940: 0013 0000 00f3 2e00 0000 9700 7c01 7c00  ............|.|.
+00000950: 5f00 0000 0000 0000 0000 7c02 7c00 5f01  _.........|.|._.
+00000960: 0000 0000 0000 0000 7c03 7c00 5f02 0000  ........|.|._...
+00000970: 0000 0000 0000 7900 a901 4e29 0372 2b00  ......y...N).r+.
+00000980: 0000 da1a 5f73 6572 7669 6365 5f69 6e73  ...._service_ins
+00000990: 7461 6e63 655f 7072 6f76 6964 6572 da15  tance_provider..
+000009a0: 7365 7276 6963 655f 636f 6e66 6967 7572  service_configur
+000009b0: 6174 696f 6e29 0472 1600 0000 722b 0000  ation).r....r+..
+000009c0: 0072 2c00 0000 7212 0000 0073 0400 0000  .r,...r....s....
+000009d0: 2020 2020 7217 0000 00da 085f 5f69 6e69      r......__ini
+000009e0: 745f 5f7a 1a53 6572 7669 6365 4465 6669  t__z.ServiceDefi
+000009f0: 6e69 7469 6f6e 2e5f 5f69 6e69 745f 5f3e  nition.__init__>
+00000a00: 0000 0073 1d00 0000 8000 f010 002d 4901  ...s.........-I.
+00000a10: 8804 d408 29d8 2a43 8804 d408 27d8 252b  ....).*C....'.%+
+00000a20: 8804 d508 2272 1a00 0000 7213 0000 0063  ...."r....r....c
+00000a30: 0100 0000 0000 0000 0000 0000 0400 0000  ................
+00000a40: 1300 0000 f33a 0000 0097 0074 0100 0000  .....:.....t....
+00000a50: 0000 0000 007c 0064 01ab 0200 0000 0000  .....|.d........
+00000a60: 0078 0172 0e01 007c 006a 0200 0000 0000  .x.r...|.j......
+00000a70: 0000 0000 0000 0000 0000 0000 0064 0275  .............d.u
+00000a80: 0153 0029 037a 5c0a 2020 2020 2020 2020  .S.).z\.        
+00000a90: 4368 6563 6b20 6966 2074 6865 2069 6e73  Check if the ins
+00000aa0: 7461 6e63 6520 7072 6f76 6964 6572 2068  tance provider h
+00000ab0: 6173 2062 6565 6e20 6465 6669 6e65 6420  as been defined 
+00000ac0: 666f 7220 7468 6973 2053 6572 7669 6365  for this Service
+00000ad0: 4465 6669 6e69 7469 6f6e 0a20 2020 2020  Definition.     
+00000ae0: 2020 2072 2f00 0000 4e29 02da 0768 6173     r/...N)...has
+00000af0: 6174 7472 722f 0000 0072 1f00 0000 7301  attrr/...r....s.
+00000b00: 0000 0020 7217 0000 00da 1d68 6173 5f73  ... r......has_s
+00000b10: 6572 7669 6365 5f69 6e73 7461 6e63 655f  ervice_instance_
+00000b20: 7072 6f76 6964 6572 7a2f 5365 7276 6963  providerz/Servic
+00000b30: 6544 6566 696e 6974 696f 6e2e 6861 735f  eDefinition.has_
+00000b40: 7365 7276 6963 655f 696e 7374 616e 6365  service_instance
+00000b50: 5f70 726f 7669 6465 724a 0000 0073 2700  _providerJ...s'.
+00000b60: 0000 8000 f408 0011 1898 04d0 1e3a d310  .............:..
+00000b70: 3bf2 0002 100a d80c 10d7 0c2b d10c 2bb0  ;..........+..+.
+00000b80: 34d0 0c37 f003 0209 0a72 1a00 0000 6301  4..7.....r....c.
+00000b90: 0000 0000 0000 0000 0000 0003 0000 0013  ................
+00000ba0: 0000 00f3 5000 0000 9700 7c00 6a01 0000  ....P.....|.j...
+00000bb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000bc0: ab00 0000 0000 0000 730b 7403 0000 0000  ........s.t.....
+00000bd0: 0000 0000 6401 ab01 0000 0000 0000 8201  ....d...........
+00000be0: 7c00 6a04 0000 0000 0000 0000 0000 0000  |.j.............
+00000bf0: 0000 0000 0000 5300 2902 7a81 0a20 2020  ......S.).z..   
+00000c00: 2020 2020 2052 6574 7269 6576 6520 7468       Retrieve th
+00000c10: 6520 7365 7276 6963 6520 696e 7374 616e  e service instan
+00000c20: 6365 2070 726f 7669 6465 7220 666f 7220  ce provider for 
+00000c30: 7468 6973 2053 6572 7669 6365 4465 6669  this ServiceDefi
+00000c40: 6e69 7469 6f6e 0a20 2020 2020 2020 2046  nition.        F
+00000c50: 4958 4d45 202d 2043 6865 636b 2050 7974  IXME - Check Pyt
+00000c60: 686f 6e20 5072 6f70 6572 7479 2073 7570  hon Property sup
+00000c70: 706f 7274 0a20 2020 2020 2020 207a 3967  port.        z9g
+00000c80: 6574 2073 6572 7669 6365 496e 7374 616e  et serviceInstan
+00000c90: 6365 5072 6f76 6964 6572 2063 616c 6c65  ceProvider calle
+00000ca0: 6420 7768 656e 206f 6e65 2064 6f65 736e  d when one doesn
+00000cb0: 2774 2065 7869 7374 2903 7234 0000 0072  't exist).r4...r
+00000cc0: 0700 0000 722f 0000 0072 1f00 0000 7301  ....r/...r....s.
+00000cd0: 0000 0020 7217 0000 00da 1d67 6574 5f73  ... r......get_s
+00000ce0: 6572 7669 6365 5f69 6e73 7461 6e63 655f  ervice_instance_
+00000cf0: 7072 6f76 6964 6572 7a2f 5365 7276 6963  providerz/Servic
+00000d00: 6544 6566 696e 6974 696f 6e2e 6765 745f  eDefinition.get_
+00000d10: 7365 7276 6963 655f 696e 7374 616e 6365  service_instance
+00000d20: 5f70 726f 7669 6465 7252 0000 0073 2e00  _providerR...s..
+00000d30: 0000 8000 f00a 0010 14d7 0f31 d10f 31d4  ...........1..1.
+00000d40: 0f33 dc12 22d8 104b f303 0213 0ef0 0002  .3.."..K........
+00000d50: 0d0e f008 0010 14d7 0f2e d10f 2ed0 082e  ................
+00000d60: 721a 0000 0029 0e72 2200 0000 7223 0000  r....).r"...r#..
+00000d70: 0072 2400 0000 da0f 5f5f 7479 7065 5f70  .r$.....__type_p
+00000d80: 6172 616d 735f 5f72 2500 0000 7209 0000  arams__r%...r...
+00000d90: 0072 0e00 0000 7206 0000 0072 0c00 0000  .r....r....r....
+00000da0: 720a 0000 0072 3100 0000 7227 0000 0072  r....r1...r'...r
+00000db0: 3400 0000 7236 0000 0029 02da 0c2e 7479  4...r6...)....ty
+00000dc0: 7065 5f70 6172 616d 7372 0800 0000 7302  pe_paramsr....s.
+00000dd0: 0000 0080 8072 1700 0000 722a 0000 0072  .....r....r*...r
+00000de0: 2a00 0000 3700 0000 7363 0000 00f8 8700  *...7...sc......
+00000df0: f102 0205 08f0 1600 4801 4c01 d827 42f1  ........H.L..'B.
+00000e00: 0d0a 052c e026 40d9 0c14 906e d00c 24f1  ...,.&@....n..$.
+00000e10: 0302 270a f005 0a05 2cf0 0a00 243b b938  ..'.....,...$;.8
+00000e20: d123 44f0 0b0a 052c f00c 0011 25f3 0d0a  .#D....,....%...
+00000e30: 052c f018 0605 0aa8 74f3 0006 050a f010  .,......t.......
+00000e40: 0a05 2fd0 2f46 c178 d12f 50f4 000a 052f  .././F.x./P..../
+00000e50: 721a 0000 0072 2a00 0000 7215 0000 0029  r....r*...r....)
+00000e60: 03da 0d2e 6765 6e65 7269 635f 6261 7365  ....generic_base
+00000e70: 7238 0000 0072 0800 0000 7303 0000 0020  r8...r....s.... 
+00000e80: 4040 7217 0000 00fa 293c 6765 6e65 7269  @@r.....)<generi
+00000e90: 6320 7061 7261 6d65 7465 7273 206f 6620  c parameters of 
+00000ea0: 5365 7276 6963 6544 6566 696e 6974 696f  ServiceDefinitio
+00000eb0: 6e3e 723a 0000 0037 0000 0073 1400 0000  n>r:...7...s....
+00000ec0: f980 009c 08f7 0025 012f f700 2501 2ff1  .......%./..%./.
+00000ed0: 0025 012f 721a 0000 0063 0000 0000 0000  .%./r....c......
+00000ee0: 0000 0000 0000 0d00 0000 0000 0000 f3fe  ................
+00000ef0: 0000 0097 0065 005a 0164 005a 0264 015a  .....e.Z.d.Z.d.Z
+00000f00: 0364 0284 005a 0409 0064 1564 0465 0564  .d...Z...d.d.e.d
+00000f10: 0565 0665 0765 0866 0219 0000 0064 0665  .e.e.e.f.....d.e
+00000f20: 0964 0764 0866 0864 0984 055a 0a65 0b64  .d.d.f.d...Z.e.d
+00000f30: 0366 0264 0465 0564 0a65 0c65 0719 0000  .f.d.e.d.e.e....
+00000f40: 0064 0565 0665 0765 0866 0219 0000 0064  .d.e.e.e.f.....d
+00000f50: 0b65 0864 0665 0964 0765 0966 0c64 0c84  .e.d.e.d.e.f.d..
+00000f60: 055a 0d65 0b64 0366 0264 0465 0564 0d65  .Z.e.d.f.d.e.d.e
+00000f70: 0e64 0e65 0e64 0b65 0864 0665 0964 0764  .d.e.d.e.d.e.d.d
+00000f80: 0866 0c64 0f84 055a 0f65 0b64 0366 0264  .f.d...Z.e.d.f.d
+00000f90: 0465 0564 0d65 0e64 0b65 0864 0665 0964  .e.d.e.d.e.d.e.d
+00000fa0: 0764 0866 0a64 1084 055a 1065 0b66 0164  .d.f.d...Z.e.f.d
+00000fb0: 0465 0564 0b65 0864 0765 0766 0664 1184  .e.d.e.d.e.f.d..
+00000fc0: 055a 1164 0465 0564 0765 0966 0464 1284  .Z.d.e.d.e.f.d..
+00000fd0: 045a 1264 1664 1384 045a 1364 0465 0564  .Z.d.d...Z.d.e.d
+00000fe0: 0665 0964 0764 0866 0664 1484 045a 1479  .e.d.d.f.d...Z.y
+00000ff0: 0829 17da 2144 6566 6175 6c74 5365 7276  .)..!DefaultServ
+00001000: 6963 654d 616e 6167 6572 5374 7261 7465  iceManagerStrate
+00001010: 6779 496d 706c 7a7d 0a20 2020 2054 6869  gyImplz}.    Thi
+00001020: 7320 6973 2074 6865 2064 6566 6175 6c74  s is the default
+00001030: 2073 6572 7669 6365 206d 616e 6167 6572   service manager
+00001040: 2073 7472 6174 6567 792e 0a20 2020 2049   strategy..    I
+00001050: 7427 7320 7573 6564 2062 7920 636c 6965  t's used by clie
+00001060: 6e74 7320 746f 2070 726f 6772 616d 6d65  nts to programme
+00001070: 7469 6361 6c6c 7920 7265 6769 7374 6572  tically register
+00001080: 2f64 6566 696e 6520 7365 7276 6963 6573  /define services
+00001090: 0a20 2020 2063 0100 0000 0000 0000 0000  .    c..........
+000010a0: 0000 0200 0000 0300 0000 f320 0000 0097  ........... ....
+000010b0: 0069 007c 005f 0000 0000 0000 0000 0069  .i.|._.........i
+000010c0: 007c 005f 0100 0000 0000 0000 0079 0072  .|._.........y.r
+000010d0: 2e00 0000 2902 da20 5f63 6f6e 7472 6f6c  ....).. _control
+000010e0: 6c65 7273 5f66 6f72 5f61 6374 6976 655f  lers_for_active_
+000010f0: 7365 7276 6963 6573 da14 5f73 6572 7669  services.._servi
+00001100: 6365 5f64 6566 696e 6974 696f 6e73 721f  ce_definitionsr.
+00001110: 0000 0073 0100 0000 2072 1700 0000 7231  ...s.... r....r1
+00001120: 0000 007a 2a44 6566 6175 6c74 5365 7276  ...z*DefaultServ
+00001130: 6963 654d 616e 6167 6572 5374 7261 7465  iceManagerStrate
+00001140: 6779 496d 706c 2e5f 5f69 6e69 745f 5f65  gyImpl.__init__e
+00001150: 0000 0073 1b00 0000 8000 f006 000d 0ff0  ...s............
+00001160: 0500 090d d408 2df0 0600 4d01 4f01 8804  ......-...M.O...
+00001170: d508 2172 1a00 0000 4672 1100 0000 722b  ..!r....Fr....r+
+00001180: 0000 00da 086f 7665 7272 6964 6572 1300  .....overrider..
+00001190: 0000 4e63 0400 0000 0000 0000 0000 0000  ..Nc............
+000011a0: 0400 0000 0300 0000 f378 0000 0097 007c  .........x.....|
+000011b0: 017c 006a 0000 0000 0000 0000 0000 0000  .|.j............
+000011c0: 0000 0000 0000 0076 0072 127c 006a 0300  .......v.r.|.j..
+000011d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000011e0: 007c 017c 03ab 0200 0000 0000 0001 0074  .|.|...........t
+000011f0: 0500 0000 0000 0000 007c 02ab 0100 0000  .........|......
+00001200: 0000 007d 047c 047c 006a 0000 0000 0000  ...}.|.|.j......
+00001210: 0000 0000 0000 0000 0000 0000 007c 013c  .............|.<
+00001220: 0000 0079 0129 0261 6a03 0000 0a20 2020  ...y.).aj....   
+00001230: 2020 2020 2052 6567 6973 7465 7220 6120       Register a 
+00001240: 7365 7276 6963 652e 2020 5468 6973 2069  service.  This i
+00001250: 7320 7468 6520 6d69 6e69 6d61 6c20 6e75  s the minimal nu
+00001260: 6d62 6572 206f 6620 696e 7075 7473 206e  mber of inputs n
+00001270: 6565 6465 6420 746f 2072 6567 6973 7465  eeded to registe
+00001280: 7220 6120 6e65 7720 7365 7276 6963 652e  r a new service.
+00001290: 0a0a 2020 2020 2020 2020 494d 504f 5254  ..        IMPORT
+000012a0: 414e 5420 4e4f 5445 3a20 4966 2072 6567  ANT NOTE: If reg
+000012b0: 6973 7465 7269 6e67 2061 206c 6966 6563  istering a lifec
+000012c0: 7963 6c65 2063 6f6e 7472 6f6c 6c65 7220  ycle controller 
+000012d0: 7468 726f 7567 6820 7468 6973 206d 6574  through this met
+000012e0: 686f 642c 2074 6865 2069 6e69 7428 7365  hod, the init(se
+000012f0: 7276 6963 6549 6e73 7461 6e63 6550 726f  rviceInstancePro
+00001300: 7669 6465 723a 0a20 2020 2020 2020 2053  vider:.        S
+00001310: 6572 7669 6365 496e 7374 616e 6365 5072  erviceInstancePr
+00001320: 6f76 6964 6572 5b54 5d2c 2063 6f6e 6669  ovider[T], confi
+00001330: 673a 2043 2920 6d65 7468 6f64 2077 696c  g: C) method wil
+00001340: 6c20 4e4f 5420 6265 2063 616c 6c65 642e  l NOT be called.
+00001350: 2020 4966 2069 7420 6d75 7374 2062 6520    If it must be 
+00001360: 6361 6c6c 6564 2c20 6974 2073 686f 756c  called, it shoul
+00001370: 6420 6265 2069 6e76 6f6b 6564 2062 790a  d be invoked by.
+00001380: 2020 2020 2020 2020 7468 6520 636c 6965          the clie
+00001390: 6e74 2062 6566 6f72 6520 7265 6769 7374  nt before regist
+000013a0: 6572 696e 6720 7468 6520 7365 7276 6963  ering the servic
+000013b0: 650a 0a20 2020 2020 2020 2040 7061 7261  e..        @para
+000013c0: 6d20 6e61 6d65 0a20 2020 2020 2020 2020  m name.         
+000013d0: 2020 2020 2020 2020 2020 2074 6865 206e             the n
+000013e0: 616d 6520 6f66 2074 6865 2064 6566 696e  ame of the defin
+000013f0: 6564 2073 6572 7669 6365 0a20 2020 2020  ed service.     
+00001400: 2020 2040 7061 7261 6d20 7365 7276 6963     @param servic
+00001410: 654c 6966 6563 7963 6c65 436f 6e74 726f  eLifecycleContro
+00001420: 6c6c 6572 0a20 2020 2020 2020 2020 2020  ller.           
+00001430: 2020 2020 2020 2020 2063 6f6e 7472 6f6c           control
+00001440: 7320 7468 6520 7365 7276 6963 6520 6c69  s the service li
+00001450: 6665 7963 6c65 2e20 466f 7220 6b6e 6f77  feycle. For know
+00001460: 6e20 636f 6e74 726f 6c6c 6572 732c 0a20  n controllers,. 
+00001470: 2020 2020 2020 2073 6565 207b 404b 6e6f         see {@Kno
+00001480: 776e 5365 7276 6963 654c 6966 6563 7963  wnServiceLifecyc
+00001490: 6c65 436f 6e74 726f 6c6c 6572 737d 0a20  leControllers}. 
+000014a0: 2020 2020 2020 2040 7061 7261 6d20 6f76         @param ov
+000014b0: 6572 7269 6465 0a20 2020 2020 2020 2020  erride.         
+000014c0: 2020 2020 2020 2020 2020 2041 6e20 6f70             An op
+000014d0: 7469 6f6e 616c 2062 6f6f 6c20 696e 6469  tional bool indi
+000014e0: 6361 7469 6e67 2077 6865 7468 6572 206f  cating whether o
+000014f0: 7220 6e6f 7420 746f 206f 7665 7272 6964  r not to overrid
+00001500: 6520 616e 0a20 2020 2020 2020 2065 7869  e an.        exi
+00001510: 7374 696e 6720 6465 6669 6e74 696f 6e20  sting defintion 
+00001520: 7769 7468 2074 6865 2073 616d 6520 6e61  with the same na
+00001530: 6d65 2e20 4966 2073 656c 6620 6973 2066  me. If self is f
+00001540: 616c 7365 2061 6e64 2061 2073 6572 7669  alse and a servi
+00001550: 6365 0a20 2020 2020 2020 2064 6566 696e  ce.        defin
+00001560: 6974 696f 6e20 616c 7265 6164 7920 6578  ition already ex
+00001570: 6973 7473 2c20 616e 2065 7272 6f72 2077  ists, an error w
+00001580: 696c 6c20 6265 2074 6872 6f77 6e0a 2020  ill be thrown.  
+00001590: 2020 2020 2020 4ea9 0372 3f00 0000 da18        N..r?.....
+000015a0: 5f68 616e 646c 655f 7365 7276 6963 655f  _handle_service_
+000015b0: 6f76 6572 7269 6465 722a 0000 0029 0572  overrider*...).r
+000015c0: 1600 0000 7211 0000 0072 2b00 0000 7240  ....r....r+...r@
+000015d0: 0000 00da 1273 6572 7669 6365 5f64 6566  .....service_def
+000015e0: 696e 6974 696f 6e73 0500 0000 2020 2020  initions....    
+000015f0: 2072 1700 0000 da23 7265 6769 7374 6572   r.....#register
+00001600: 5f73 6572 7669 6365 5f62 795f 636f 6e74  _service_by_cont
+00001610: 726f 6c6c 6572 5f6f 6e6c 797a 4544 6566  roller_onlyzEDef
+00001620: 6175 6c74 5365 7276 6963 654d 616e 6167  aultServiceManag
+00001630: 6572 5374 7261 7465 6779 496d 706c 2e72  erStrategyImpl.r
+00001640: 6567 6973 7465 725f 7365 7276 6963 655f  egister_service_
+00001650: 6279 5f63 6f6e 7472 6f6c 6c65 725f 6f6e  by_controller_on
+00001660: 6c79 6b00 0000 7342 0000 0080 00f0 3200  lyk...sB......2.
+00001670: 0c10 9034 d713 2cd1 132c d10b 2cd8 0c10  ...4..,..,..,...
+00001680: d70c 29d1 0c29 a824 b008 d40c 39e4 3a4b  ..)..).$....9.:K
+00001690: d80c 28f3 0302 3b0a d008 1af0 0600 2b3d  ..(...;.......+=
+000016a0: 8804 d708 21d1 0821 a024 d208 2772 1a00  ....!..!.$..'r..
+000016b0: 0000 722c 0000 0072 1200 0000 6306 0000  ..r,...r....c...
+000016c0: 0000 0000 0000 0000 0005 0000 0003 0000  ................
+000016d0: 00f3 7c00 0000 9700 7c01 7c00 6a00 0000  ..|.....|.|.j...
+000016e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000016f0: 7600 7212 7c00 6a03 0000 0000 0000 0000  v.r.|.j.........
+00001700: 0000 0000 0000 0000 0000 7c01 7c05 ab02  ..........|.|...
+00001710: 0000 0000 0000 0100 7405 0000 0000 0000  ........t.......
+00001720: 0000 7c03 7c02 7c04 ab03 0000 0000 0000  ..|.|.|.........
+00001730: 7d06 7c06 7c00 6a00 0000 0000 0000 0000  }.|.|.j.........
+00001740: 0000 0000 0000 0000 0000 7c01 3c00 0000  ..........|.<...
+00001750: 7901 2902 7a8c 0a20 2020 2020 2020 2052  y.).z..        R
+00001760: 6567 6973 7465 7220 6120 7365 7276 6963  egister a servic
+00001770: 652c 2070 726f 7669 6469 6e67 2074 6865  e, providing the
+00001780: 2073 6572 7669 6365 206e 616d 652c 2069   service name, i
+00001790: 6e73 7461 6e63 6520 7072 6f76 6964 6572  nstance provider
+000017a0: 2c20 6c69 6665 6379 636c 6520 636f 6e74  , lifecycle cont
+000017b0: 726f 6c6c 6572 2061 6e64 0a20 2020 2020  roller and.     
+000017c0: 2020 206f 7074 696f 6e61 6c20 636f 6e66     optional conf
+000017d0: 6967 7572 6174 696f 6e0a 2020 2020 2020  iguration.      
+000017e0: 2020 4e72 4200 0000 2907 7216 0000 0072    NrB...).r....r
+000017f0: 1100 0000 722c 0000 0072 2b00 0000 7212  ....r,...r+...r.
+00001800: 0000 0072 4000 0000 7244 0000 0073 0700  ...r@...rD...s..
+00001810: 0000 2020 2020 2020 2072 1700 0000 da10  ..       r......
+00001820: 7265 6769 7374 6572 5f73 6572 7669 6365  register_service
+00001830: 7a32 4465 6661 756c 7453 6572 7669 6365  z2DefaultService
+00001840: 4d61 6e61 6765 7253 7472 6174 6567 7949  ManagerStrategyI
+00001850: 6d70 6c2e 7265 6769 7374 6572 5f73 6572  mpl.register_ser
+00001860: 7669 6365 8c00 0000 7347 0000 0080 00f0  vice....sG......
+00001870: 1c00 0c10 9034 d713 2cd1 132c d10b 2cd8  .....4..,..,..,.
+00001880: 0c10 d70c 29d1 0c29 a824 b008 d40c 39e4  ....)..).$....9.
+00001890: 3a4b d80c 28d0 2a43 c056 f303 023b 0ad0  :K..(.*C.V...;..
+000018a0: 081a f006 002b 3d88 04d7 0821 d108 21a0  .....+=....!..!.
+000018b0: 24d2 0827 721a 0000 00da 0d73 6572 7669  $..'r......servi
+000018c0: 6365 5f63 6c61 7373 da22 7365 7276 6963  ce_class."servic
+000018d0: 655f 6c69 6665 6379 636c 655f 636f 6e74  e_lifecycle_cont
+000018e0: 726f 6c6c 6572 5f63 6c61 7373 6306 0000  roller_classc...
+000018f0: 0000 0000 0000 0000 0007 0000 0003 0000  ................
+00001900: 00f3 5200 0000 9700 7401 0000 0000 0000  ..R.....t.......
+00001910: 0000 7c02 ab01 0000 0000 0000 7d06 0200  ..|.........}...
+00001920: 7c03 ab00 0000 0000 0000 7d07 7c00 6a03  |.........}.|.j.
+00001930: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001940: 0000 7c01 7c06 7c07 7c04 7c05 ab05 0000  ..|.|.|.|.|.....
+00001950: 0000 0000 0100 7901 2902 6144 0300 000a  ......y.).aD....
+00001960: 2020 2020 2020 2020 5265 6769 7374 6572          Register
+00001970: 2061 2073 6572 7669 6365 2070 726f 7669   a service provi
+00001980: 6469 6e67 2061 2063 6f6e 7472 7563 746f  ding a contructo
+00001990: 7220 6d65 7468 6f64 2066 6f72 2061 2073  r method for a s
+000019a0: 6572 7669 6365 2063 6c61 7373 2061 6e64  ervice class and
+000019b0: 2073 6572 7669 6365 206c 6966 6563 7963   service lifecyc
+000019c0: 6c65 2063 6f6e 7472 6f6c 6c65 7220 636c  le controller cl
+000019d0: 6173 730a 0a20 2020 2020 2020 2040 7061  ass..        @pa
+000019e0: 7261 6d20 6e61 6d65 0a20 2020 2020 2020  ram name.       
+000019f0: 2020 2020 2020 2020 2020 2020 2074 6865               the
+00001a00: 206e 616d 6520 6f66 2074 6865 2064 6566   name of the def
+00001a10: 696e 6564 2073 6572 7669 6365 0a20 2020  ined service.   
+00001a20: 2020 2020 2040 7061 7261 6d20 7365 7276       @param serv
+00001a30: 6963 6543 6c61 7373 0a20 2020 2020 2020  iceClass.       
+00001a40: 2020 2020 2020 2020 2020 2020 2074 6865               the
+00001a50: 2063 6c61 7373 2074 6861 7420 696d 706c   class that impl
+00001a60: 656d 656e 7473 2074 6865 2073 6572 7669  ements the servi
+00001a70: 6365 0a20 2020 2020 2020 2040 7061 7261  ce.        @para
+00001a80: 6d20 7365 7276 6963 654c 6966 6563 7963  m serviceLifecyc
+00001a90: 6c65 436f 6e74 726f 6c6c 6572 436c 6173  leControllerClas
+00001aa0: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
+00001ab0: 2020 2020 2020 7468 6520 636c 6173 7320        the class 
+00001ac0: 7468 6174 2063 6f6e 7472 6f6c 7320 7468  that controls th
+00001ad0: 6520 7365 7276 6963 6520 6c69 6665 7963  e service lifeyc
+00001ae0: 6c65 2e20 466f 7220 6b6e 6f77 6e20 636f  le. For known co
+00001af0: 6e74 726f 6c6c 6572 732c 0a20 2020 2020  ntrollers,.     
+00001b00: 2020 2073 6565 207b 404b 6e6f 776e 5365     see {@KnownSe
+00001b10: 7276 6963 654c 6966 6563 7963 6c65 436f  rviceLifecycleCo
+00001b20: 6e74 726f 6c6c 6572 737d 0a20 2020 2020  ntrollers}.     
+00001b30: 2020 2040 7061 7261 6d20 636f 6e66 6967     @param config
+00001b40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001b50: 2020 2020 2041 6e20 4f70 7469 6f6e 616c       An Optional
+00001b60: 2063 6f6e 6669 6720 6d61 7920 6265 2073   config may be s
+00001b70: 7570 706c 6965 6420 666f 7220 7365 7276  upplied for serv
+00001b80: 6963 6520 6465 6669 6e69 7469 6f6e 206c  ice definition l
+00001b90: 6576 656c 0a20 2020 2020 2020 2063 6f6e  evel.        con
+00001ba0: 6669 6775 7261 7469 6f6e 2e0a 2020 2020  figuration..    
+00001bb0: 2020 2020 4070 6172 616d 206f 7665 7272      @param overr
+00001bc0: 6964 650a 2020 2020 2020 2020 2020 2020  ide.            
+00001bd0: 2020 2020 2020 2020 416e 206f 7074 696f          An optio
+00001be0: 6e61 6c20 626f 6f6c 2069 6e64 6963 6174  nal bool indicat
+00001bf0: 696e 6720 7768 6574 6865 7220 6f72 206e  ing whether or n
+00001c00: 6f74 2074 6f20 6f76 6572 7269 6465 2061  ot to override a
+00001c10: 6e0a 2020 2020 2020 2020 6578 6973 7469  n.        existi
+00001c20: 6e67 2064 6566 696e 7469 6f6e 2077 6974  ng defintion wit
+00001c30: 6820 7468 6520 7361 6d65 206e 616d 652e  h the same name.
+00001c40: 2049 6620 7365 6c66 2069 7320 6661 6c73   If self is fals
+00001c50: 6520 616e 6420 6120 7365 7276 6963 650a  e and a service.
+00001c60: 2020 2020 2020 2020 6465 6669 6e69 7469          definiti
+00001c70: 6f6e 2061 6c72 6561 6479 2065 7869 7374  on already exist
+00001c80: 732c 2061 6e20 6572 726f 7220 7769 6c6c  s, an error will
+00001c90: 2062 6520 7468 726f 776e 0a20 2020 2020   be thrown.     
+00001ca0: 2020 204e 2902 720b 0000 0072 4700 0000     N).r....rG...
+00001cb0: 2908 7216 0000 0072 1100 0000 7248 0000  ).r....r....rH..
+00001cc0: 0072 4900 0000 7212 0000 0072 4000 0000  .rI...r....r@...
+00001cd0: da10 7365 7276 6963 655f 7072 6f76 6964  ..service_provid
+00001ce0: 6572 722b 0000 0073 0800 0000 2020 2020  err+...s....    
+00001cf0: 2020 2020 7217 0000 00da 1972 6567 6973      r......regis
+00001d00: 7465 725f 7365 7276 6963 655f 6279 5f63  ter_service_by_c
+00001d10: 6c61 7373 7a3b 4465 6661 756c 7453 6572  lassz;DefaultSer
+00001d20: 7669 6365 4d61 6e61 6765 7253 7472 6174  viceManagerStrat
+00001d30: 6567 7949 6d70 6c2e 7265 6769 7374 6572  egyImpl.register
+00001d40: 5f73 6572 7669 6365 5f62 795f 636c 6173  _service_by_clas
+00001d50: 73a3 0000 0073 3300 0000 8000 f436 001c  s....s3......6..
+00001d60: 3eb8 6dd3 1b4c d008 18d9 2749 d327 4bd0  >.m..L....'I.'K.
+00001d70: 0824 d808 0cd7 081d d108 1dd8 0c10 d012  .$..............
+00001d80: 22d0 2440 c026 c828 f503 0209 0a72 1a00  ".$@.&.(.....r..
+00001d90: 0000 6305 0000 0000 0000 0000 0000 0007  ..c.............
+00001da0: 0000 0003 0000 00f3 4a00 0000 9700 7c00  ........J.....|.
+00001db0: 6a01 0000 0000 0000 0000 0000 0000 0000  j...............
+00001dc0: 0000 0000 7c01 7c02 7402 0000 0000 0000  ....|.|.t.......
+00001dd0: 0000 6a04 0000 0000 0000 0000 0000 0000  ..j.............
+00001de0: 0000 0000 0000 7c03 7c04 ab05 0000 0000  ......|.|.......
+00001df0: 0000 0100 7901 2902 616d 0200 000a 2020  ....y.).am....  
+00001e00: 2020 2020 2020 5265 6769 7374 6572 2061        Register a
+00001e10: 2073 6572 7669 6365 2074 6861 7420 6861   service that ha
+00001e20: 7320 6120 7369 6e67 6c65 746f 6e20 6c69  s a singleton li
+00001e30: 6665 6379 636c 6520 286f 6e6c 7920 6f6e  fecycle (only on
+00001e40: 6520 696e 7374 616e 6365 2065 7869 7374  e instance exist
+00001e50: 7329 0a0a 2020 2020 2020 2020 4070 6172  s)..        @par
+00001e60: 616d 206e 616d 650a 2020 2020 2020 2020  am name.        
+00001e70: 2020 2020 2020 2020 2020 2020 7468 6520              the 
+00001e80: 6e61 6d65 206f 6620 7468 6520 6465 6669  name of the defi
+00001e90: 6e65 6420 7365 7276 6963 650a 2020 2020  ned service.    
+00001ea0: 2020 2020 4070 6172 616d 2073 6572 7669      @param servi
+00001eb0: 6365 436c 6173 730a 2020 2020 2020 2020  ceClass.        
+00001ec0: 2020 2020 2020 2020 2020 2020 7468 6520              the 
+00001ed0: 636c 6173 7320 7468 6174 2069 6d70 6c65  class that imple
+00001ee0: 6d65 6e74 7320 7468 6520 7365 7276 6963  ments the servic
+00001ef0: 650a 2020 2020 2020 2020 4070 6172 616d  e.        @param
+00001f00: 2063 6f6e 6669 670a 2020 2020 2020 2020   config.        
+00001f10: 2020 2020 2020 2020 2020 2020 416e 204f              An O
+00001f20: 7074 696f 6e61 6c20 636f 6e66 6967 206d  ptional config m
+00001f30: 6179 2062 6520 7375 7070 6c69 6564 2066  ay be supplied f
+00001f40: 6f72 2073 6572 7669 6365 2064 6566 696e  or service defin
+00001f50: 6974 696f 6e20 6c65 7665 6c0a 2020 2020  ition level.    
+00001f60: 2020 2020 636f 6e66 6967 7572 6174 696f      configuratio
+00001f70: 6e2e 0a20 2020 2020 2020 2040 7061 7261  n..        @para
+00001f80: 6d20 6f76 6572 7269 6465 0a20 2020 2020  m override.     
+00001f90: 2020 2020 2020 2020 2020 2020 2020 2041                 A
+00001fa0: 6e20 6f70 7469 6f6e 616c 2062 6f6f 6c20  n optional bool 
+00001fb0: 696e 6469 6361 7469 6e67 2077 6865 7468  indicating wheth
+00001fc0: 6572 206f 7220 6e6f 7420 746f 206f 7665  er or not to ove
+00001fd0: 7272 6964 6520 616e 0a20 2020 2020 2020  rride an.       
+00001fe0: 2065 7869 7374 696e 6720 6465 6669 6e74   existing defint
+00001ff0: 696f 6e20 7769 7468 2074 6865 2073 616d  ion with the sam
+00002000: 6520 6e61 6d65 2e20 4966 2073 656c 6620  e name. If self 
+00002010: 6973 2066 616c 7365 2061 6e64 2061 2073  is false and a s
+00002020: 6572 7669 6365 0a20 2020 2020 2020 2064  ervice.        d
+00002030: 6566 696e 6974 696f 6e20 616c 7265 6164  efinition alread
+00002040: 7920 6578 6973 7473 2c20 616e 2065 7272  y exists, an err
+00002050: 6f72 2077 696c 6c20 6265 2074 6872 6f77  or will be throw
+00002060: 6e0a 2020 2020 2020 2020 4e29 0372 4c00  n.        N).rL.
+00002070: 0000 720d 0000 00da 0953 494e 474c 4554  ..r......SINGLET
+00002080: 4f4e 2905 7216 0000 0072 1100 0000 7248  ON).r....r....rH
+00002090: 0000 0072 1200 0000 7240 0000 0073 0500  ...r....r@...s..
+000020a0: 0000 2020 2020 2072 1700 0000 da1a 7265  ..     r......re
+000020b0: 6769 7374 6572 5f73 696e 676c 6574 6f6e  gister_singleton
+000020c0: 5f73 6572 7669 6365 7a3c 4465 6661 756c  _servicez<Defaul
+000020d0: 7453 6572 7669 6365 4d61 6e61 6765 7253  tServiceManagerS
+000020e0: 7472 6174 6567 7949 6d70 6c2e 7265 6769  trategyImpl.regi
+000020f0: 7374 6572 5f73 696e 676c 6574 6f6e 5f73  ster_singleton_s
+00002100: 6572 7669 6365 c400 0000 7327 0000 0080  ervice....s'....
+00002110: 00f0 2c00 090d d708 26d1 0826 d80c 10d8  ..,.....&..&....
+00002120: 0c19 dc0c 2cd7 0c36 d10c 36d8 0c12 d80c  ....,..6..6.....
+00002130: 14f5 0b06 090a 721a 0000 0063 0300 0000  ......r....c....
+00002140: 0000 0000 0000 0000 0400 0000 0300 0000  ................
+00002150: f37c 0100 0097 007c 017c 006a 0000 0000  .|.....|.|.j....
+00002160: 0000 0000 0000 0000 0000 0000 0000 0076  ...............v
+00002170: 0172 0e74 0300 0000 0000 0000 0064 017c  .r.t.........d.|
+00002180: 017a 0000 00ab 0100 0000 0000 0082 017c  .z.............|
+00002190: 017c 006a 0400 0000 0000 0000 0000 0000  .|.j............
+000021a0: 0000 0000 0000 0076 0072 1f7c 006a 0400  .......v.r.|.j..
+000021b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000021c0: 007c 0119 0000 007d 037c 036a 1100 0000  .|.....}.|.j....
+000021d0: 0000 0000 0000 0000 0000 0000 0000 00ab  ................
+000021e0: 0000 0000 0000 0053 007c 006a 0000 0000  .......S.|.j....
+000021f0: 0000 0000 0000 0000 0000 0000 0000 007c  ...............|
+00002200: 0119 0000 007d 047c 046a 0600 0000 0000  .....}.|.j......
+00002210: 0000 0000 0000 0000 0000 0000 007d 037c  .............}.|
+00002220: 046a 0900 0000 0000 0000 0000 0000 0000  .j..............
+00002230: 0000 0000 00ab 0000 0000 0000 0072 2a7c  .............r*|
+00002240: 036a 0b00 0000 0000 0000 0000 0000 0000  .j..............
+00002250: 0000 0000 007c 046a 0d00 0000 0000 0000  .....|.j........
+00002260: 0000 0000 0000 0000 0000 00ab 0000 0000  ................
+00002270: 0000 007c 046a 0e00 0000 0000 0000 0000  ...|.j..........
+00002280: 0000 0000 0000 0000 00ab 0200 0000 0000  ................
+00002290: 0001 007c 037c 006a 0400 0000 0000 0000  ...|.|.j........
+000022a0: 0000 0000 0000 0000 0000 007c 013c 0000  ...........|.<..
+000022b0: 007c 036a 1100 0000 0000 0000 0000 0000  .|.j............
+000022c0: 0000 0000 0000 00ab 0000 0000 0000 0053  ...............S
+000022d0: 0029 024e 7a15 5365 7276 6963 6520 6e6f  .).Nz.Service no
+000022e0: 7420 6465 6669 6e65 643a 2029 0972 3f00  t defined: ).r?.
+000022f0: 0000 7207 0000 0072 3e00 0000 722b 0000  ..r....r>...r+..
+00002300: 0072 3400 0000 da04 696e 6974 7236 0000  .r4.....initr6..
+00002310: 0072 3000 0000 7218 0000 0029 0572 1600  .r0...r....).r..
+00002320: 0000 7211 0000 0072 1200 0000 722b 0000  ..r....r....r+..
+00002330: 0072 4400 0000 7305 0000 0020 2020 2020  .rD...s....     
+00002340: 7217 0000 0072 1800 0000 7a2d 4465 6661  r....r....z-Defa
+00002350: 756c 7453 6572 7669 6365 4d61 6e61 6765  ultServiceManage
+00002360: 7253 7472 6174 6567 7949 6d70 6c2e 6765  rStrategyImpl.ge
+00002370: 745f 7365 7276 6963 65e2 0000 0073 d000  t_service....s..
+00002380: 0000 8000 f00c 000c 1090 74d7 1730 d117  ..........t..0..
+00002390: 30d1 0b30 dc12 22d0 233a b854 d123 41d3  0..0..".#:.T.#A.
+000023a0: 1242 d00c 42f0 0600 0c10 9034 d713 38d1  .B..B......4..8.
+000023b0: 1338 d10b 38d8 2b2f d72b 50d1 2b50 d051  .8..8.+/.+P.+P.Q
+000023c0: 55d1 2b56 d00c 28f0 2200 102c d70f 37d1  U.+V..(."..,..7.
+000023d0: 0f37 d30f 39d0 0839 f01f 003f 4301 d73e  .7..9..9...?C..>
+000023e0: 57d1 3e57 d810 14f1 0302 3f0e d00c 1ef0  W.>W......?.....
+000023f0: 0800 1123 d710 3fd1 103f f003 000d 29f0  ...#..?..?....).
+00002400: 0800 1022 d70f 3fd1 0f3f d40f 41d8 102c  ..."..?..?..A..,
+00002410: d710 31d1 1031 d814 26d7 1444 d114 44d3  ..1..1..&..D..D.
+00002420: 1446 d814 26d7 143c d114 3cf4 0503 1112  .F..&..<..<.....
+00002430: f00a 003b 5701 8844 d70c 31d1 0c31 b024  ...;W..D..1..1.$
+00002440: d10c 37e0 0f2b d70f 37d1 0f37 d30f 39d0  ..7..+..7..7..9.
+00002450: 0839 721a 0000 0063 0200 0000 0000 0000  .9r....c........
+00002460: 0000 0000 0200 0000 0300 0000 f31e 0000  ................
+00002470: 0097 007c 017c 006a 0000 0000 0000 0000  ...|.|.j........
+00002480: 0000 0000 0000 0000 0000 0076 0053 0072  ...........v.S.r
+00002490: 2e00 0000 2901 723f 0000 0072 1c00 0000  ....).r?...r....
+000024a0: 7302 0000 0020 2072 1700 0000 721d 0000  s....  r....r...
+000024b0: 007a 3444 6566 6175 6c74 5365 7276 6963  .z4DefaultServic
+000024c0: 654d 616e 6167 6572 5374 7261 7465 6779  eManagerStrategy
+000024d0: 496d 706c 2e69 735f 7365 7276 6963 655f  Impl.is_service_
+000024e0: 6465 6669 6e65 6400 0100 0073 1300 0000  defined....s....
+000024f0: 8000 d80f 1390 74d7 1730 d117 30d0 0f30  ......t..0..0..0
+00002500: d008 3072 1a00 0000 6301 0000 0000 0000  ..0r....c.......
+00002510: 0000 0000 0003 0000 0003 0000 00f3 ca00  ................
+00002520: 0000 9700 7c00 6a00 0000 0000 0000 0000  ....|.j.........
+00002530: 0000 0000 0000 0000 0000 6a03 0000 0000  ..........j.....
+00002540: 0000 0000 0000 0000 0000 0000 0000 ab00  ................
+00002550: 0000 0000 0000 4400 5d12 0000 7d01 7c01  ......D.]...}.|.
+00002560: 6a05 0000 0000 0000 0000 0000 0000 0000  j...............
+00002570: 0000 0000 ab00 0000 0000 0000 0100 8c14  ................
+00002580: 0400 7c00 6a00 0000 0000 0000 0000 0000  ..|.j...........
+00002590: 0000 0000 0000 0000 6a07 0000 0000 0000  ........j.......
+000025a0: 0000 0000 0000 0000 0000 0000 ab00 0000  ................
+000025b0: 0000 0000 0100 7c00 6a08 0000 0000 0000  ......|.j.......
+000025c0: 0000 0000 0000 0000 0000 0000 6a07 0000  ............j...
+000025d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000025e0: ab00 0000 0000 0000 0100 7900 722e 0000  ..........y.r...
+000025f0: 0029 0572 3e00 0000 da06 7661 6c75 6573  .).r>.....values
+00002600: 7220 0000 00da 0563 6c65 6172 723f 0000  r .....clearr?..
+00002610: 0029 0272 1600 0000 da17 6e65 7874 5f73  .).r......next_s
+00002620: 6572 7669 6365 5f63 6f6e 7472 6f6c 6c65  ervice_controlle
+00002630: 7273 0200 0000 2020 7217 0000 0072 2000  rs....  r....r .
+00002640: 0000 7a2a 4465 6661 756c 7453 6572 7669  ..z*DefaultServi
+00002650: 6365 4d61 6e61 6765 7253 7472 6174 6567  ceManagerStrateg
+00002660: 7949 6d70 6c2e 7368 7574 646f 776e 0301  yImpl.shutdown..
+00002670: 0000 7353 0000 0080 00d8 272b d727 4cd1  ..sS......'+.'L.
+00002680: 274c d727 53d1 2753 d327 55f2 0001 092f  'L.'S.'S.'U..../
+00002690: d00c 23d8 0c23 d70c 2cd1 0c2c d50c 2ef0  ..#..#..,..,....
+000026a0: 0301 092f f006 0009 0dd7 082d d108 2dd7  .../.......-..-.
+000026b0: 0833 d108 33d4 0835 d808 0cd7 0821 d108  .3..3..5.....!..
+000026c0: 21d7 0827 d108 27d5 0829 721a 0000 0063  !..'..'..)r....c
+000026d0: 0300 0000 0000 0000 0000 0000 0400 0000  ................
+000026e0: 0300 0000 f3ba 0000 0097 007c 0272 497c  ...........|.rI|
+000026f0: 006a 0000 0000 0000 0000 0000 0000 0000  .j..............
+00002700: 0000 0000 007c 013d 007c 017c 006a 0200  .....|.=.|.|.j..
+00002710: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002720: 0076 0072 2d7c 006a 0200 0000 0000 0000  .v.r-|.j........
+00002730: 0000 0000 0000 0000 0000 007c 0119 0000  ...........|....
+00002740: 007d 037c 036a 0500 0000 0000 0000 0000  .}.|.j..........
+00002750: 0000 0000 0000 0000 00ab 0000 0000 0000  ................
+00002760: 0001 007c 006a 0200 0000 0000 0000 0000  ...|.j..........
+00002770: 0000 0000 0000 0000 007c 013d 0079 0079  .........|.=.y.y
+00002780: 0074 0700 0000 0000 0000 0064 017c 017a  .t.........d.|.z
+00002790: 0000 0064 027a 0000 00ab 0100 0000 0000  ...d.z..........
+000027a0: 0082 0129 034e 7a14 5365 7276 6963 6520  ...).Nz.Service 
+000027b0: 7769 7468 206e 616d 652c 203a 7a45 2c20  with name, :zE, 
+000027c0: 6973 2061 6c72 6561 6479 2064 6566 696e  is already defin
+000027d0: 6564 2e20 2053 7065 6369 6679 206f 7665  ed.  Specify ove
+000027e0: 7272 6964 653d 7472 7565 2069 6620 6974  rride=true if it
+000027f0: 2073 686f 756c 6420 6265 2072 6570 6c61   should be repla
+00002800: 6365 6429 0472 3f00 0000 723e 0000 0072  ced).r?...r>...r
+00002810: 2000 0000 7207 0000 0029 0472 1600 0000   ...r....).r....
+00002820: 7211 0000 0072 4000 0000 da14 636f 6e74  r....r@.....cont
+00002830: 726f 6c6c 6572 5f74 6f5f 7265 6d6f 7665  roller_to_remove
+00002840: 7304 0000 0020 2020 2072 1700 0000 7243  s....    r....rC
+00002850: 0000 007a 3a44 6566 6175 6c74 5365 7276  ...z:DefaultServ
+00002860: 6963 654d 616e 6167 6572 5374 7261 7465  iceManagerStrate
+00002870: 6779 496d 706c 2e5f 6861 6e64 6c65 5f73  gyImpl._handle_s
+00002880: 6572 7669 6365 5f6f 7665 7272 6964 650a  ervice_override.
+00002890: 0100 0073 7400 0000 8000 d90b 13e0 1014  ...st...........
+000028a0: d710 29d1 1029 a824 d010 2fd8 0f13 9074  ..)..).$../....t
+000028b0: d717 3cd1 173c d10f 3cd8 272b d727 4cd1  ..<..<..<.'+.'L.
+000028c0: 274c c854 d127 52d0 1024 d810 24d7 102d  'L.T.'R..$..$..-
+000028d0: d110 2dd4 102f d814 18d7 1439 d114 39b8  ..-../.....9..9.
+000028e0: 24d1 143f f007 0010 3df4 0a00 1323 d810  $..?....=....#..
+000028f0: 26d8 1216 f103 0111 17e0 1259 f105 0211  &..........Y....
+00002900: 5a01 f303 0413 0ef0 0004 0d0e 721a 0000  Z...........r...
+00002910: 0029 0146 7221 0000 0029 1572 2200 0000  .).Fr!...).r"...
+00002920: 7223 0000 0072 2400 0000 7225 0000 0072  r#...r$...r%...r
+00002930: 3100 0000 7226 0000 0072 0e00 0000 7208  1...r&...r....r.
+00002940: 0000 0072 0600 0000 7227 0000 0072 4500  ...r....r'...rE.
+00002950: 0000 7209 0000 0072 0c00 0000 7247 0000  ..r....r....rG..
+00002960: 00da 0474 7970 6572 4c00 0000 724f 0000  ...typerL...rO..
+00002970: 0072 1800 0000 721d 0000 0072 2000 0000  .r....r....r ...
+00002980: 7243 0000 0072 1500 0000 721a 0000 0072  rC...r....r....r
+00002990: 1700 0000 723c 0000 0072 3c00 0000 5f00  ....r<...r<..._.
+000029a0: 0000 7380 0100 0084 00f1 0203 0508 f20a  ..s.............
+000029b0: 0405 4f01 f018 001a 1ff1 0d1f 053d e00e  ..O..........=..
+000029c0: 11f0 051f 053d f006 0027 4101 d80c 1490  .....=...'A.....
+000029d0: 6ed0 0c24 f103 0227 0af0 071f 053d f00c  n..$...'.....=..
+000029e0: 0013 17f0 0d1f 053d f00e 000a 0ef3 0f1f  .......=........
+000029f0: 053d f050 0100 223d d819 1ef1 1114 053d  .=.P.."=.......=
+00002a00: e00e 11f0 0514 053d f006 0024 3bb8 38d1  .......=...$;.8.
+00002a10: 2344 f007 1405 3df0 0800 2741 01d8 0c14  #D....=...'A....
+00002a20: 906e d00c 24f1 0302 270a f009 1405 3df0  .n..$...'.....=.
+00002a30: 0e00 111f f00f 1405 3df0 1000 1317 f011  ........=.......
+00002a40: 1405 3df0 1200 0a0e f313 1405 3df0 3800  ..=.........=.8.
+00002a50: 223d d819 1ef1 0d1f 050a e00e 11f0 051f  "=..............
+00002a60: 050a f006 0018 1cf0 071f 050a f008 002d  ...............-
+00002a70: 31f0 091f 050a f00a 0011 1ff0 0b1f 050a  1...............
+00002a80: f00c 0013 17f0 0d1f 050a f00e 000a 0ef3  ................
+00002a90: 0f1f 050a f04a 0100 223d d819 1ef1 0b1c  .....J.."=......
+00002aa0: 050a e00e 11f0 051c 050a f006 0018 1cf0  ................
+00002ab0: 071c 050a f008 0011 1ff0 091c 050a f00a  ................
+00002ac0: 0013 17f0 0b1c 050a f00c 000a 0ef3 0d1c  ................
+00002ad0: 050a f03e 0033 4e01 f103 1c05 3ad8 1417  ...>.3N.....:...
+00002ae0: f003 1c05 3ad8 212f f003 1c05 3ae0 0911  ....:.!/....:...
+00002af0: f305 1c05 3af0 3c01 0531 a073 f000 0105  ....:.<..1.s....
+00002b00: 31a8 74f3 0001 0531 f306 0505 2af0 0e0d  1.t....1....*...
+00002b10: 050e a853 f000 0d05 0eb8 44f0 000d 050e  ...S......D.....
+00002b20: c054 f400 0d05 0e72 1a00 0000 723c 0000  .T.....r....r<..
+00002b30: 0063 0000 0000 0000 0000 0000 0000 0100  .c..............
+00002b40: 0000 0000 0000 f310 0000 0097 0065 005a  .............e.Z
+00002b50: 0164 005a 0264 015a 0379 0229 03da 1c43  .d.Z.d.Z.y.)...C
+00002b60: 6f6e 6669 6753 6572 7669 6365 4d61 6e61  onfigServiceMana
+00002b70: 6765 7253 7472 6174 6567 797a 690a 2020  gerStrategyzi.  
+00002b80: 2020 4120 7374 7261 7465 6779 2074 6861    A strategy tha
+00002b90: 7420 7265 6164 7320 7365 7276 6963 6520  t reads service 
+00002ba0: 636f 6e66 6967 7572 6174 696f 6e20 6672  configuration fr
+00002bb0: 6f6d 2073 6572 7669 6365 436f 6e66 6967  om serviceConfig
+00002bc0: 2e6a 736f 6e2e 2020 4649 584d 4520 2d20  .json.  FIXME - 
+00002bd0: 546f 2042 6520 496d 706c 656d 656e 7465  To Be Implemente
+00002be0: 640a 2020 2020 4e29 0472 2200 0000 7223  d.    N).r"...r#
+00002bf0: 0000 0072 2400 0000 7225 0000 0072 1500  ...r$...r%...r..
+00002c00: 0000 721a 0000 0072 1700 0000 725b 0000  ..r....r....r[..
+00002c10: 0072 5b00 0000 1c01 0000 7307 0000 0084  .r[.......s.....
+00002c20: 00f2 0202 0508 721a 0000 0072 5b00 0000  ......r....r[...
+00002c30: 4e29 1772 2500 0000 da03 6162 6372 0300  N).r%.....abcr..
+00002c40: 0000 7204 0000 00da 0674 7970 696e 6772  ..r......typingr
+00002c50: 0500 0000 da1f 7370 6879 726e 612e 7365  ......sphyrna.se
+00002c60: 7276 6963 655f 6d61 6e61 6765 722e 7365  rvice_manager.se
+00002c70: 7276 6963 6572 0600 0000 7207 0000 0072  rvicer....r....r
+00002c80: 0800 0000 da2d 7370 6879 726e 612e 7365  .....-sphyrna.se
+00002c90: 7276 6963 655f 6d61 6e61 6765 722e 7365  rvice_manager.se
+00002ca0: 7276 6963 655f 636f 6e66 6967 7572 6174  rvice_configurat
+00002cb0: 696f 6e72 0900 0000 720a 0000 00da 3173  ionr....r.....1s
+00002cc0: 7068 7972 6e61 2e73 6572 7669 6365 5f6d  phyrna.service_m
+00002cd0: 616e 6167 6572 2e73 6572 7669 6365 5f69  anager.service_i
+00002ce0: 6e73 7461 6e63 655f 7072 6f76 6964 6572  nstance_provider
+00002cf0: 720b 0000 0072 0c00 0000 da34 7370 6879  r....r.....4sphy
+00002d00: 726e 612e 7365 7276 6963 655f 6d61 6e61  rna.service_mana
+00002d10: 6765 722e 7365 7276 6963 655f 6c69 6665  ger.service_life
+00002d20: 6379 636c 655f 636f 6e74 726f 6c6c 6572  cycle_controller
+00002d30: 720d 0000 0072 0e00 0000 7210 0000 0072  r....r....r....r
+00002d40: 2a00 0000 723c 0000 0072 5b00 0000 7215  *...r<...r[...r.
+00002d50: 0000 0072 1a00 0000 7217 0000 00fa 083c  ...r....r......<
+00002d60: 6d6f 6475 6c65 3e72 6200 0000 0100 0000  module>rb.......
+00002d70: 7356 0000 00f0 0301 0101 f102 0301 04f7  sV..............
+00002d80: 0a00 0124 dd00 17e7 0056 d100 56f7 0203  ...$.....V..V...
+00002d90: 0102 f708 0301 02f7 0803 0102 f40c 1b01  ................
+00002da0: 0c98 53f4 001b 010c f73e 2501 2ff4 5001  ..S......>%./.P.
+00002db0: 7802 010e d028 3ef4 0078 0201 0ef4 7a05  x....(>..x....z.
+00002dc0: 0301 08d0 2344 f500 0301 0872 1a00 0000  ....#D.....r....
```

### Comparing `sphyrna_service_manager-0.3.0/src/main/python/sphyrna/service_manager/service.py` & `sphyrna_service_manager-0.3.7/src/main/python/sphyrna/service_manager/service.py`

 * *Files identical despite different names*

### Comparing `sphyrna_service_manager-0.3.0/src/main/python/sphyrna/service_manager/service_configuration.py` & `sphyrna_service_manager-0.3.7/src/main/python/sphyrna/service_manager/service_configuration.py`

 * *Files identical despite different names*

### Comparing `sphyrna_service_manager-0.3.0/src/main/python/sphyrna/service_manager/service_instance_provider.py` & `sphyrna_service_manager-0.3.7/src/main/python/sphyrna/service_manager/service_instance_provider.py`

 * *Files identical despite different names*

### Comparing `sphyrna_service_manager-0.3.0/src/main/python/sphyrna/service_manager/service_lifecycle_controller.py` & `sphyrna_service_manager-0.3.7/src/main/python/sphyrna/service_manager/service_lifecycle_controller.py`

 * *Files identical despite different names*

### Comparing `sphyrna_service_manager-0.3.0/src/main/python/sphyrna/service_manager/service_manager.py` & `sphyrna_service_manager-0.3.7/src/main/python/sphyrna/service_manager/service_manager.py`

 * *Files identical despite different names*

### Comparing `sphyrna_service_manager-0.3.0/src/main/python/sphyrna/service_manager/service_manager_strategy.py` & `sphyrna_service_manager-0.3.7/src/main/python/sphyrna/service_manager/service_manager_strategy.py`

 * *Files identical despite different names*

