# Comparing `tmp/cheeseapi-1.1.5.tar.gz` & `tmp/cheeseapi-1.2.0.tar.gz`

## Comparing `cheeseapi-1.1.5.tar` & `cheeseapi-1.2.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 cheeseapi-1.1.5/CheeseAPI/__init__.py
--rw-r--r--   0        0        0     7395 2020-02-02 00:00:00.000000 cheeseapi-1.1.5/CheeseAPI/app.py
--rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 cheeseapi-1.1.5/CheeseAPI/cors.py
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 cheeseapi-1.1.5/CheeseAPI/exception.py
--rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 cheeseapi-1.1.5/CheeseAPI/file.py
--rw-r--r--   0        0        0    32435 2020-02-02 00:00:00.000000 cheeseapi-1.1.5/CheeseAPI/handle.py
--rw-r--r--   0        0        0     4493 2020-02-02 00:00:00.000000 cheeseapi-1.1.5/CheeseAPI/protocol.py
--rw-r--r--   0        0        0     4771 2020-02-02 00:00:00.000000 cheeseapi-1.1.5/CheeseAPI/request.py
--rw-r--r--   0        0        0    17621 2020-02-02 00:00:00.000000 cheeseapi-1.1.5/CheeseAPI/response.py
--rw-r--r--   0        0        0    13136 2020-02-02 00:00:00.000000 cheeseapi-1.1.5/CheeseAPI/route.py
--rw-r--r--   0        0        0    10363 2020-02-02 00:00:00.000000 cheeseapi-1.1.5/CheeseAPI/schedule.py
--rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 cheeseapi-1.1.5/CheeseAPI/server.py
--rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 cheeseapi-1.1.5/CheeseAPI/signal.py
--rw-r--r--   0        0        0     8558 2020-02-02 00:00:00.000000 cheeseapi-1.1.5/CheeseAPI/text.py
--rw-r--r--   0        0        0    12835 2020-02-02 00:00:00.000000 cheeseapi-1.1.5/CheeseAPI/validator.py
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 cheeseapi-1.1.5/CheeseAPI/websocket.py
--rw-r--r--   0        0        0     2974 2020-02-02 00:00:00.000000 cheeseapi-1.1.5/CheeseAPI/workspace.py
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 cheeseapi-1.1.5/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 cheeseapi-1.1.5/LICENSE
--rw-r--r--   0        0        0     5007 2020-02-02 00:00:00.000000 cheeseapi-1.1.5/README.md
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 cheeseapi-1.1.5/pyproject.toml
--rw-r--r--   0        0        0     5477 2020-02-02 00:00:00.000000 cheeseapi-1.1.5/PKG-INFO
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 cheeseapi-1.2.0/CheeseAPI/__init__.py
+-rw-r--r--   0        0        0     7395 2020-02-02 00:00:00.000000 cheeseapi-1.2.0/CheeseAPI/app.py
+-rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 cheeseapi-1.2.0/CheeseAPI/cors.py
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 cheeseapi-1.2.0/CheeseAPI/exception.py
+-rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 cheeseapi-1.2.0/CheeseAPI/file.py
+-rw-r--r--   0        0        0    32445 2020-02-02 00:00:00.000000 cheeseapi-1.2.0/CheeseAPI/handle.py
+-rw-r--r--   0        0        0     4484 2020-02-02 00:00:00.000000 cheeseapi-1.2.0/CheeseAPI/protocol.py
+-rw-r--r--   0        0        0     4771 2020-02-02 00:00:00.000000 cheeseapi-1.2.0/CheeseAPI/request.py
+-rw-r--r--   0        0        0    17621 2020-02-02 00:00:00.000000 cheeseapi-1.2.0/CheeseAPI/response.py
+-rw-r--r--   0        0        0    13136 2020-02-02 00:00:00.000000 cheeseapi-1.2.0/CheeseAPI/route.py
+-rw-r--r--   0        0        0    10363 2020-02-02 00:00:00.000000 cheeseapi-1.2.0/CheeseAPI/schedule.py
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 cheeseapi-1.2.0/CheeseAPI/server.py
+-rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 cheeseapi-1.2.0/CheeseAPI/signal.py
+-rw-r--r--   0        0        0     8546 2020-02-02 00:00:00.000000 cheeseapi-1.2.0/CheeseAPI/text.py
+-rw-r--r--   0        0        0    12835 2020-02-02 00:00:00.000000 cheeseapi-1.2.0/CheeseAPI/validator.py
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 cheeseapi-1.2.0/CheeseAPI/websocket.py
+-rw-r--r--   0        0        0     2974 2020-02-02 00:00:00.000000 cheeseapi-1.2.0/CheeseAPI/workspace.py
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 cheeseapi-1.2.0/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 cheeseapi-1.2.0/LICENSE
+-rw-r--r--   0        0        0     5007 2020-02-02 00:00:00.000000 cheeseapi-1.2.0/README.md
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 cheeseapi-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     5477 2020-02-02 00:00:00.000000 cheeseapi-1.2.0/PKG-INFO
```

### Comparing `cheeseapi-1.1.5/CheeseAPI/app.py` & `cheeseapi-1.2.0/CheeseAPI/app.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.1.5/CheeseAPI/cors.py` & `cheeseapi-1.2.0/CheeseAPI/cors.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.1.5/CheeseAPI/exception.py` & `cheeseapi-1.2.0/CheeseAPI/exception.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.1.5/CheeseAPI/file.py` & `cheeseapi-1.2.0/CheeseAPI/file.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.1.5/CheeseAPI/handle.py` & `cheeseapi-1.2.0/CheeseAPI/handle.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,15 @@
         for filename in os.listdir(modulePath):
             filePath = os.path.join(modulePath, filename)
             if os.path.isfile(filePath) and filename.endswith('.py'):
                 __import__(f'{name}.{filename[:-3]}', fromlist = [''])
 
     def loadLocalModules(self):
         foldernames = self._app.localModules.copy()
-        for foldername in self._app.preferred_localModules:
+        for foldername in reversed(self._app.preferred_localModules):
             if foldername in foldernames:
                 foldernames.remove(foldername)
                 foldernames.insert(0, foldername)
         for foldername in self._app.exclude_localModules:
             if foldername in foldernames:
                 foldernames.remove(foldername)
```

### Comparing `cheeseapi-1.1.5/CheeseAPI/protocol.py` & `cheeseapi-1.2.0/CheeseAPI/protocol.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,15 +58,16 @@
             asyncio.get_event_loop().create_task(app._handle.http(self))
 
     def on_body(self, body: bytes):
         if self.request.body is None:
             self.request._body = b''
         self.request._body += body
 
-        if len(self.request.body) == int(self.request.headers.get('Content-Length', 0)):
+    def on_message_complete(self):
+        if not self.parser.should_upgrade():
             self.request._parseBody()
             asyncio.get_event_loop().create_task(app._handle.http(self))
 
     def connection_lost(self, exc: Exception | None):
         self.transport.close()
 
 class WebsocketProtocol(WebSocketServerProtocol):
```

### Comparing `cheeseapi-1.1.5/CheeseAPI/request.py` & `cheeseapi-1.2.0/CheeseAPI/request.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.1.5/CheeseAPI/response.py` & `cheeseapi-1.2.0/CheeseAPI/response.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.1.5/CheeseAPI/route.py` & `cheeseapi-1.2.0/CheeseAPI/route.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.1.5/CheeseAPI/schedule.py` & `cheeseapi-1.2.0/CheeseAPI/schedule.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.1.5/CheeseAPI/server.py` & `cheeseapi-1.2.0/CheeseAPI/server.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.1.5/CheeseAPI/signal.py` & `cheeseapi-1.2.0/CheeseAPI/signal.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.1.5/CheeseAPI/text.py` & `cheeseapi-1.2.0/CheeseAPI/text.py`

 * *Files 0% similar despite different names*

```diff
@@ -149,16 +149,16 @@
         return [
             (message, styledMessage)
         ]
 
     def validator_requiredMessage(self, scope: str, key: str) -> str:
         return f'The {scope}.{key} is required'
 
-    def validator_typeMessage(self, scope: str, key: str, expected_type: object) -> str:
-        return f'The {scope}.{key} cannot be converted to {expected_type.__name__}'
+    def validator_typeMessage(self, scope: str, key: str, expected_type: str) -> str:
+        return f'The {scope}.{key} cannot be converted to {expected_type}'
 
     def validator_patternMessage(self, scope: str, key: str) -> str:
         return f'The {scope}.{key} regular check error'
 
     def validator_minMessage(self, scope: str, key: str, min: object) -> str:
         return f'The {scope}.{key} cannot be less than {min}'
```

### Comparing `cheeseapi-1.1.5/CheeseAPI/validator.py` & `cheeseapi-1.2.0/CheeseAPI/validator.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 from CheeseAPI.response import Response, BaseResponse
 from CheeseAPI.request import Request
 
 if TYPE_CHECKING:
     from CheeseAPI.app import App
 
 class ValidateError(Exception):
-    def __init__(self, response: BaseResponse = Response('校验错误', 400)):
+    def __init__(self, response: BaseResponse | None = None):
         '''
         在自定义校验函数中抛出此错误，可结束校验并直接返回响应体。
         '''
 
-        self.response = response
+        self.response: BaseResponse | None = response
 
 class Bool:
     '''
     将满足小写后等于true或false的字符串转为`bool`。
     '''
 
     def __new__(cls, value: str) -> bool:
@@ -36,16 +36,16 @@
 class Validator:
     def __init__(self,
         scope: Literal['form', 'headers', 'args', 'path', 'cookie'],
         key: str,
         *,
         required: bool = False,
         default: Any = None,
-        type: List[object | Callable] | object | Callable | None = None,
-        expected_type: object | None = None,
+        type: List[object | Callable] | object | Callable = str,
+        expected_type: str | None = None,
         pattern: str | None = None,
         min: object | None = None,
         max: object | None = None,
         enum: List[Any] = [],
         fn: Callable | None = None,
         response: Response | None = None
     ):
@@ -53,28 +53,28 @@
         可能的示例：
 
         ```python
         import datetime
 
         from CheeseAPI import Validator
 
-        Validator('form', 'date', type = [ float, datetime.datetime.fromtimestamp ], expected_type = datetime.datetime)
+        Validator('form', 'date', type = [ float, datetime.datetime.fromtimestamp ], expected_type = 'timestamp')
 
         Validator('form', 'gender', enum = [ 'man', 'woman', None ])
 
         Validator('form', 'idCard', pattern = r'^[1-9]\\d{5}(18|19|20)\\d{2}(0[1-9]|1[0-2])(0[1-9]|[1-2]\\d|3[0-1])\\d{3}[\\dXx]$', response = Response('身份证格式错误', 400))
         ```
 
         - Args
 
             - scope: 域范围。form: request.form；headers: request.headers；args: request.args；path: request.path中的动态路由；cookie: request.cookie。
 
             - type: 遵循`self.type(value) -> object`的类或函数；支持list按顺序转换类型。
 
-            - expected_type: 期望的数据类型，对type转换后的结果进行二次校验。
+            - expected_type: 期望的数据类型，不参与校验，仅供提示。
 
             - default: 默认值；该值仍会执行校验流程，而不是直接应用。
 
             - pattern: 对于`str`类型的数据，使用正则表达式进行验证。
 
             - enum: 指定某些特定的值。
 
@@ -97,15 +97,15 @@
 
                 若有返回值，则为该参数的最终值。
         '''
 
         self._scope: Literal['form', 'headers', 'args', 'path', 'cookie'] = scope
         self.key: str = key
         self._type: List[object | Callable] | object | Callable = type
-        self._expected_type: object = type if expected_type is None else expected_type
+        self._expected_type: str = type.__name__ if expected_type is None else expected_type
         self.required: bool = required
         self._default: Any = default
         self._pattern: str | None = pattern
         self.min: object | None = min
         self.max: object | None = max
         if self.min is not None and self.max is not None and self.min > self.max:
             raise ValueError('最小范围不能大于最大范围')
@@ -128,16 +128,14 @@
             if self.type is not None:
                 try:
                     if isinstance(self.type, list):
                         for type in self.type:
                             validatedForm[f'{self.scope}.{self.key}'] = type(validatedForm[f'{self.scope}.{self.key}'])
                     else:
                         validatedForm[f'{self.scope}.{self.key}'] = self.type(validatedForm[f'{self.scope}.{self.key}'])
-                    if not isinstance(validatedForm[f'{self.scope}.{self.key}'], self.expected_type):
-                        raise Exception()
                 except:
                     raise ValidateError(self.response or Response(app._text.validator_typeMessage(self.scope, self.key, self.expected_type), 400))
 
             if self.pattern and not re.match(self.pattern, validatedForm[f'{self.scope}.{self.key}']):
                 raise ValidateError(self.response or Response(app._text.validator_patternMessage(self.scope, self.key), 400))
 
             if self.min and validatedForm[f'{self.scope}.{self.key}'] < self.min:
@@ -146,21 +144,24 @@
             if self.max and validatedForm[f'{self.scope}.{self.key}'] > self.max:
                 raise ValidateError(self.response or Response(app._text.validator_maxMessage(self.scope, self.key, self.max), 400))
 
             if self.enum and validatedForm[f'{self.scope}.{self.key}'] not in self.enum:
                 raise ValidateError(self.response or Response(app._text.validator_enumMessage(self.scope, self.key, self.enum), 400))
 
             if self.fn:
-                _value = await self.fn(*args, **{
-                    'request': request,
-                    'validatedForm': validatedForm,
-                    **kwargs
-                })
-                if _value is not None:
-                    validatedForm[f'{self.scope}.{self.key}'] = _value
+                try:
+                    _value = await self.fn(*args, **{
+                        'request': request,
+                        'validatedForm': validatedForm,
+                        **kwargs
+                    })
+                    if _value is not None:
+                        validatedForm[f'{self.scope}.{self.key}'] = _value
+                except ValidateError as e:
+                    raise ValidateError(e.response or self.response or Response(status = 500))
 
     @property
     def scope(self) -> Literal['form', 'headers', 'args', 'path', 'cookie']:
         '''
         域范围。
 
         - form: request.form。
@@ -189,24 +190,24 @@
         return self._type
 
     @type.setter
     def type(self, value: object | Callable | None):
         self._type = value
 
     @property
-    def expected_type(self) -> object:
+    def expected_type(self) -> str:
         '''
-        期望的数据类型，对type转换后的结果进行二次校验。
+        期望的数据类型，不参与校验，仅供提示。
         '''
 
         return self._expected_type
 
     @expected_type.setter
-    def expected_type(self, value: object | None):
-        self._expected_type = self.type if value is None else value
+    def expected_type(self, value: str | None):
+        self._expected_type = self.type.__name__ if value is None else value
 
     @property
     def default(self) -> Any:
         '''
         默认值；该值仍会执行校验流程，而不是直接应用。
         '''
 
@@ -299,15 +300,15 @@
         date = datetime.datetime.now()
         if validatedForm['form.birthDate'] > date:
             raise ValidateError(Response('出生日期异常', 400))
 
     @app.route.get('/')
     @validator([
         Validator('form', 'name', required = True),
-        Validator('form', 'birthDate', type = [ float, datetime.datetime.fromtimestamp ], expected_type = datetime.datetime, fn = birthDateValidator),
+        Validator('form', 'birthDate', type = [ float, datetime.datetime.fromtimestamp ], expected_type = 'timestamp', fn = birthDateValidator),
         Validator('form', 'gender', enum = [ 'man', 'woman', None ]),
         Validator('form', 'idCard', pattern = r'^[1-9]\\d{5}(18|19|20)\\d{2}(0[1-9]|1[0-2])(0[1-9]|[1-2]\\d|3[0-1])\\d{3}[\\dXx]$', response = Response('身份证格式错误', 400))
     ])
     async def test(*args, validatedForm: Dict[str, Any], **kwargs):
         ...
     ```
 
@@ -323,15 +324,15 @@
         date = datetime.datetime.now()
         if validatedForm['form.birthDate'] > date:
             raise ValidateError(Response('出生日期异常', 400))
 
     @app.route.get('/')
     @validator([
         Validator('form', 'name', required = True),
-        Validator('form', 'birthDate', type = [ float, datetime.datetime.fromtimestamp ], expected_type = datetime.datetime),
+        Validator('form', 'birthDate', type = [ float, datetime.datetime.fromtimestamp ], expected_type = 'timestamp'),
         Validator('form', 'gender', enum = [ 'man', 'woman', None ]),
         Validator('form', 'idCard', pattern = r'^[1-9]\\d{5}(18|19|20)\\d{2}(0[1-9]|1[0-2])(0[1-9]|[1-2]\\d|3[0-1])\\d{3}[\\dXx]$', response = Response('身份证格式错误', 400)),
         Validator('form', 'birthDate', fn = birthDateValidator)
     ])
     async def test(*args, validatedForm: Dict[str, Any], **kwargs):
         ...
     ```
```

### Comparing `cheeseapi-1.1.5/CheeseAPI/websocket.py` & `cheeseapi-1.2.0/CheeseAPI/websocket.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.1.5/CheeseAPI/workspace.py` & `cheeseapi-1.2.0/CheeseAPI/workspace.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.1.5/LICENSE` & `cheeseapi-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.1.5/README.md` & `cheeseapi-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.1.5/pyproject.toml` & `cheeseapi-1.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "hatchling" ]
 build-backend = "hatchling.build"
 
 [project]
 name = "CheeseAPI"
-version = "1.1.5"
+version = "1.2.0"
 description = "一款web协程框架。"
 readme = "README.md"
 license-files = { paths = [ "LICENSE" ] }
 authors = [
     { name = "Cheese Unknown", email = "cheese@cheese.ren" }
 ]
 keywords = [ 'API', 'BackEnd' ]
```

### Comparing `cheeseapi-1.1.5/PKG-INFO` & `cheeseapi-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: CheeseAPI
-Version: 1.1.5
+Version: 1.2.0
 Summary: 一款web协程框架。
 Project-URL: Source, https://github.com/CheeseUnknown/CheeseAPI
 Author-email: Cheese Unknown <cheese@cheese.ren>
 License-File: LICENSE
 Keywords: API,BackEnd
 Requires-Dist: cheeselog==1.0.*
 Requires-Dist: cheesesignal==1.1.*
```

