# Comparing `tmp/fastapi_problem-0.7.1.tar.gz` & `tmp/fastapi_problem-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_problem-0.7.1.tar", max compression
+gzip compressed data, was "fastapi_problem-0.7.2.tar", max compression
```

## Comparing `fastapi_problem-0.7.1.tar` & `fastapi_problem-0.7.2.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0    11307 2024-05-01 10:08:05.397058 fastapi_problem-0.7.1/LICENSE
--rw-r--r--   0        0        0     5013 2024-05-01 10:08:05.397058 fastapi_problem-0.7.1/README.md
--rw-r--r--   0        0        0     2243 2024-05-01 10:08:05.401058 fastapi_problem-0.7.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-01 10:08:05.401058 fastapi_problem-0.7.1/src/fastapi_problem/__init__.py
--rw-r--r--   0        0        0      220 2024-05-01 10:08:05.401058 fastapi_problem-0.7.1/src/fastapi_problem/cors.py
--rw-r--r--   0        0        0     2308 2024-05-01 10:08:05.401058 fastapi_problem-0.7.1/src/fastapi_problem/error.py
--rw-r--r--   0        0        0        0 2024-05-01 10:08:05.401058 fastapi_problem-0.7.1/src/fastapi_problem/handler/__init__.py
--rw-r--r--   0        0        0     4571 2024-05-01 10:08:05.401058 fastapi_problem-0.7.1/src/fastapi_problem/handler/fastapi.py
--rw-r--r--   0        0        0     6175 2024-05-01 10:08:05.401058 fastapi_problem-0.7.1/src/fastapi_problem/handler/starlette.py
--rw-r--r--   0        0        0      297 2024-05-01 10:08:05.401058 fastapi_problem-0.7.1/src/fastapi_problem/handler/util.py
--rw-r--r--   0        0        0     5720 1970-01-01 00:00:00.000000 fastapi_problem-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0    11307 2024-05-12 20:39:02.122127 fastapi_problem-0.7.2/LICENSE
+-rw-r--r--   0        0        0     1905 2024-05-12 20:39:02.122127 fastapi_problem-0.7.2/README.md
+-rw-r--r--   0        0        0     2228 2024-05-12 20:39:02.122127 fastapi_problem-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-12 20:39:02.122127 fastapi_problem-0.7.2/src/fastapi_problem/__init__.py
+-rw-r--r--   0        0        0      220 2024-05-12 20:39:02.122127 fastapi_problem-0.7.2/src/fastapi_problem/cors.py
+-rw-r--r--   0        0        0     3349 2024-05-12 20:39:02.122127 fastapi_problem-0.7.2/src/fastapi_problem/error.py
+-rw-r--r--   0        0        0        0 2024-05-12 20:39:02.122127 fastapi_problem-0.7.2/src/fastapi_problem/handler/__init__.py
+-rw-r--r--   0        0        0     5955 2024-05-12 20:39:02.122127 fastapi_problem-0.7.2/src/fastapi_problem/handler/base.py
+-rw-r--r--   0        0        0     3094 2024-05-12 20:39:02.122127 fastapi_problem-0.7.2/src/fastapi_problem/handler/fastapi.py
+-rw-r--r--   0        0        0     2225 2024-05-12 20:39:02.122127 fastapi_problem-0.7.2/src/fastapi_problem/handler/starlette.py
+-rw-r--r--   0        0        0      297 2024-05-12 20:39:02.122127 fastapi_problem-0.7.2/src/fastapi_problem/handler/util.py
+-rw-r--r--   0        0        0     2602 1970-01-01 00:00:00.000000 fastapi_problem-0.7.2/PKG-INFO
```

### Comparing `fastapi_problem-0.7.1/LICENSE` & `fastapi_problem-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_problem-0.7.1/pyproject.toml` & `fastapi_problem-0.7.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [tool.poetry]
 name = "fastapi-problem"
-version = "0.7.1"
+version = "0.7.2"
 description = "FastAPI support for RFC9457 problems."
 authors = ["Daniel Edgecombe <edgy.edgemond@gmail.com>"]
 license = "Apache-2.0"
-repository="https://github.com/EdgyEdgemond/fastapi-problem/"
-homepage="https://github.com/EdgyEdgemond/fastapi-problem/"
+repository="https://github.com/NRWLDev/fastapi-problem/"
+homepage="https://github.com/NRWLDev/fastapi-problem/"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 
 [tool.poetry.dev-dependencies]
 
@@ -23,15 +23,15 @@
 pytest-random-order = "^1.0"
 
 # Style
 ruff = "^0.3.0"
 pre-commit = "^3.0.2"
 
 [tool.bumpversion]
-current_version = "0.7.1"
+current_version = "0.7.2"
 commit = true
 tag = true
 
 [[tool.bumpversion.files]]
 filename = "README.md"
 
 [[tool.bumpversion.files]]
@@ -60,15 +60,15 @@
 
 [tool.coverage.report]
 sort = "cover"
 fail_under = 95
 show_missing = true
 skip_covered = true
 exclude_lines = [
-    "if typing.TYPE_CHECKING:",
+    "if t.TYPE_CHECKING:",
 ]
 
 [tool.coverage.run]
 branch = true
 source = ["src/fastapi_problem"]
 
 [tool.ruff]
```

### Comparing `fastapi_problem-0.7.1/src/fastapi_problem/error.py` & `fastapi_problem-0.7.2/src/fastapi_problem/error.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,19 +3,20 @@
 https://www.rfc-editor.org/rfc/rfc9457.html
 """
 
 from __future__ import annotations
 
 import re
 import typing as t
+from warnings import warn
 
 CONVERT_RE = re.compile(r"(?<!^)(?=[A-Z])")
 
 
-class HttpException(Exception):  # noqa: N818
+class Problem(Exception):  # noqa: N818
     """
     A base exception designed to support all API error handling.
     All exceptions should inherit from this or a subclass of it (depending on the usage),
     this will allow all apps and libraries to maintain a common exception chain
     """
 
     def __init__(
@@ -28,15 +29,14 @@
     ) -> None:
         super().__init__(title)
         self._code = code
         self.title = title
         self.details = details
         self.status = status
         self.extras = kwargs
-        self.warn = True
 
     @property
     def type(self: t.Self) -> str:
         type_ = "".join(self.__class__.__name__.rsplit("Error", 1))
         type_ = CONVERT_RE.sub("-", type_).lower()
         return self._code if self._code else type_
 
@@ -61,30 +61,75 @@
 
         if strip_debug:
             ret = {k: v for k, v in ret.items() if k in ["type", "title", "status"]}
 
         return ret
 
 
-class HttpCodeException(HttpException):
+class HttpException(Problem):
+    def __init__(
+        self: t.Self,
+        title: str,
+        code: str | None = None,
+        details: str | None = None,
+        status: int = 500,
+        **kwargs,
+    ) -> None:
+        warn(
+            "HttpException use is deprecated, use `Problem` subclasses instead.",
+            FutureWarning,
+            stacklevel=2,
+        )
+        super().__init__(title, core=code, details=details, status=status, **kwargs)
+
+
+class StatusProblem(Problem):
     code = None
     title = "Base http exception."
     status = 500
 
     def __init__(self: t.Self, details: str | None = None, **kwargs) -> None:
-        self.warn = False
         super().__init__(self.title, code=self.code, details=details, status=self.status, **kwargs)
 
 
+class HttpCodeException(StatusProblem):
+    def __init__(self: t.Self, details: str | None = None, **kwargs) -> None:
+        warn(
+            "HttpCodeException use is deprecated, use `StatusProblem` subclasses instead.",
+            FutureWarning,
+            stacklevel=2,
+        )
+        super().__init__(details=details, **kwargs)
+
+
+class ServerProblem(StatusProblem): ...
+
+
 class ServerException(HttpCodeException): ...
 
 
+class BadRequestProblem(StatusProblem):
+    status = 400
+
+
 class BadRequestException(HttpCodeException):
     status = 400
 
 
+class UnauthorisedProblem(StatusProblem):
+    status = 401
+
+
 class UnauthorisedException(HttpCodeException):
     status = 401
 
 
+class NotFoundProblem(StatusProblem):
+    status = 404
+
+
 class NotFoundException(HttpCodeException):
     status = 404
+
+
+class ConflictProblem(StatusProblem):
+    status = 409
```

### Comparing `fastapi_problem-0.7.1/src/fastapi_problem/handler/starlette.py` & `fastapi_problem-0.7.2/src/fastapi_problem/handler/base.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,176 +1,164 @@
 from __future__ import annotations
 
 import http
 import logging
-import typing
+import typing as t
 
-from starlette.exceptions import HTTPException
 from starlette.middleware.cors import CORSMiddleware
+from starlette.requests import Request
 from starlette.responses import JSONResponse
 
-from fastapi_problem.error import HttpCodeException, HttpException
+from fastapi_problem.error import Problem, StatusProblem
 from fastapi_problem.handler.util import convert_status_code
 
-if typing.TYPE_CHECKING:
-    from starlette.applications import Starlette
-    from starlette.requests import Request
+if t.TYPE_CHECKING:
+    from starlette.exceptions import HTTPException
 
     from fastapi_problem.cors import CorsConfiguration
 
-logger_ = logging.getLogger(__name__)
-
-
-def cors_wrapper_factory(
-    cors: CorsConfiguration,
-    handler: typing.Callable[[Request, Exception], JSONResponse],
-) -> typing.Callable[[Request, Exception], JSONResponse]:
-    def wrapper(request: Request, exc: Exception) -> JSONResponse:
-        response = handler(request, exc)
-
-        # Since the CORSMiddleware is not executed when an unhandled server exception
-        # occurs, we need to manually set the CORS headers ourselves if we want the FE
-        # to receive a proper JSON 500, opposed to a CORS error.
-        # Setting CORS headers on server errors is a bit of a philosophical topic of
-        # discussion in many frameworks, and it is currently not handled in FastAPI.
-        # See dotnet core for a recent discussion, where ultimately it was
-        # decided to return CORS headers on server failures:
-        # https://github.com/dotnet/aspnetcore/issues/2378
-        origin = request.headers.get("origin")
-
-        if origin:
-            # Have the middleware do the heavy lifting for us to parse
-            # all the config, then update our response headers
-            mw = CORSMiddleware(
-                app=None,
-                allow_origins=cors.allow_origins,
-                allow_credentials=cors.allow_credentials,
-                allow_methods=cors.allow_methods,
-                allow_headers=cors.allow_headers,
-            )
 
-            # Logic directly from Starlette"s CORSMiddleware:
-            # https://github.com/encode/starlette/blob/master/starlette/middleware/cors.py#L152
-
-            response.headers.update(mw.simple_headers)
-            has_cookie = "cookie" in request.headers
-
-            # If request includes any cookie headers, then we must respond
-            # with the specific origin instead of "*".
-            if mw.allow_all_origins and has_cookie:
-                response.headers["Access-Control-Allow-Origin"] = origin
-
-            # If we only allow specific origins, then we have to mirror back
-            # the Origin header in the response.
-            elif not mw.allow_all_origins and mw.is_allowed_origin(origin=origin):
-                response.headers["Access-Control-Allow-Origin"] = origin
-                response.headers.add_vary_header("Origin")
+logger_ = logging.getLogger(__name__)
 
-        return response
+Handler = t.Callable[["ExceptionHandler", Request, Exception], tuple[dict, Problem]]
+PreHook = t.Callable[[Request, JSONResponse], JSONResponse]
+PostHook = t.Callable[[Request, Exception], None]
+
+
+def http_exception_handler(eh: ExceptionHandler, _request: Request, exc: HTTPException) -> tuple[dict, Problem]:
+    wrapper = eh.unhandled_wrappers.get(str(exc.status_code))
+    title, code = convert_status_code(exc.status_code)
+    details = exc.detail
+    ret = (
+        wrapper(details)
+        if wrapper
+        else Problem(
+            title=title,
+            code=code,
+            details=details,
+            status=exc.status_code,
+        )
+    )
+    headers = exc.headers or {}
 
-    return wrapper
+    return headers, ret
 
 
-def exception_handler_factory(
-    logger: logging.Logger,
-    unhandled_wrappers: dict[str, type[HttpCodeException]],
-    *,
-    strip_debug: bool = False,
-    strip_debug_codes: list[int] | None = None,
-) -> typing.Callable[[Exception], JSONResponse]:
-    unhandled_wrappers = unhandled_wrappers or {}
-    strip_debug_codes = strip_debug_codes or []
+class ExceptionHandler:
+    def __init__(  # noqa: PLR0913
+        self: t.Self,
+        logger: logging.Logger = logger_,
+        unhandled_wrappers: dict[str, type[StatusProblem]] | None = None,
+        handlers: dict[Exception, Handler] | None = None,
+        pre_hooks: list | None = None,
+        post_hooks: list[PostHook] | None = None,
+        *,
+        strip_debug: bool = False,
+        strip_debug_codes: list[int] | None = None,
+    ) -> None:
+        self.logger = logger
+        self.unhandled_wrappers = unhandled_wrappers or {}
+        self.handlers = handlers or {}
+        self.pre_hooks = pre_hooks or []
+        self.post_hooks = post_hooks or []
+        self.strip_debug = strip_debug
+        self.strip_debug_codes = strip_debug_codes or []
+
+    def __call__(self: t.Self, request: Request, exc: Exception) -> JSONResponse:
+        for pre_hook in self.pre_hooks:
+            pre_hook(request, exc)
 
-    def exception_handler(_request: Request, exc: Exception) -> JSONResponse:
-        wrapper = unhandled_wrappers.get("default")
+        wrapper = self.unhandled_wrappers.get("default", self.unhandled_wrappers.get("500"))
         ret = (
             wrapper(str(exc))
             if wrapper
-            else HttpException(
+            else Problem(
                 title="Unhandled exception occurred.",
                 details=str(exc),
                 code="unhandled-exception",
             )
         )
         headers = {}
 
-        if isinstance(exc, HTTPException):
-            wrapper = unhandled_wrappers.get(str(exc.status_code))
-            title, code = convert_status_code(exc.status_code)
-            details = exc.detail
-            ret = (
-                wrapper(details)
-                if wrapper
-                else HttpException(
-                    title=title,
-                    code=code,
-                    details=details,
-                    status=exc.status_code,
-                )
-            )
-            headers = exc.headers or headers
+        for exc_type, handler in self.handlers.items():
+            if isinstance(exc, exc_type):
+                headers_, ret = handler(self, request, exc)
+                headers.update(headers_)
+                break
 
-        if isinstance(exc, HttpException):
+        if isinstance(exc, Problem):
             ret = exc
 
         if ret.status >= http.HTTPStatus.INTERNAL_SERVER_ERROR:
-            logger.exception(ret.title, exc_info=(type(exc), exc, exc.__traceback__))
+            self.logger.exception(ret.title, exc_info=(type(exc), exc, exc.__traceback__))
 
-        strip_debug_ = strip_debug or ret.status in strip_debug_codes
+        strip_debug_ = self.strip_debug or ret.status in self.strip_debug_codes
 
         if strip_debug_ and (ret.details or ret.extras):
             msg = "Stripping debug information from exception."
-            logger.debug(msg)
+            self.logger.debug(msg)
 
             for k, v in {
                 "details": ret.details,
                 **ret.extras,
             }.items():
                 msg = f"Removed {k}: {v}"
-                logger.debug(msg)
+                self.logger.debug(msg)
 
         headers["content-type"] = "application/problem+json"
 
-        return JSONResponse(
+        response = JSONResponse(
             status_code=ret.status,
             content=ret.marshal(strip_debug=strip_debug_),
             headers=headers,
         )
 
-    return exception_handler
+        for post_hook in self.post_hooks:
+            response = post_hook(request, response)
 
+        return response
 
-def generate_handler(
-    logger: logging.Logger = logger_,
-    cors: CorsConfiguration | None = None,
-    unhandled_wrappers: dict[str, type[HttpCodeException]] | None = None,
-    *,
-    strip_debug: bool = False,
-    strip_debug_codes: list[int] | None = None,
-) -> typing.Callable:
-    handler = exception_handler_factory(
-        logger=logger,
-        unhandled_wrappers=unhandled_wrappers,
-        strip_debug=strip_debug,
-        strip_debug_codes=strip_debug_codes,
-    )
-    return cors_wrapper_factory(cors, handler) if cors else handler
 
+class CorsPostHook:
+    def __init__(self: t.Self, config: CorsConfiguration) -> None:
+        self.config = config
 
-def add_exception_handler(  # noqa: PLR0913
-    app: Starlette,
-    logger: logging.Logger = logger_,
-    cors: CorsConfiguration | None = None,
-    unhandled_wrappers: dict[str, type[HttpCodeException]] | None = None,
-    *,
-    strip_debug: bool = False,
-    strip_debug_codes: list[int] | None = None,
-) -> None:
-    eh = generate_handler(
-        logger,
-        cors,
-        unhandled_wrappers,
-        strip_debug=strip_debug,
-        strip_debug_codes=strip_debug_codes,
-    )
-    app.exception_handler(Exception)(eh)
-    app.exception_handler(HTTPException)(eh)
+    def __call__(self: t.Self, request: Request, response: JSONResponse) -> JSONResponse:
+        # Since the CORSMiddleware is not executed when an unhandled server exception
+        # occurs, we need to manually set the CORS headers ourselves if we want the FE
+        # to receive a proper JSON 500, opposed to a CORS error.
+        # Setting CORS headers on server errors is a bit of a philosophical topic of
+        # discussion in many frameworks, and it is currently not handled in FastAPI.
+        # See dotnet core for a recent discussion, where ultimately it was
+        # decided to return CORS headers on server failures:
+        # https://github.com/dotnet/aspnetcore/issues/2378
+        origin = request.headers.get("origin")
+
+        if origin:
+            # Have the middleware do the heavy lifting for us to parse
+            # all the config, then update our response headers
+            mw = CORSMiddleware(
+                app=None,
+                allow_origins=self.config.allow_origins,
+                allow_credentials=self.config.allow_credentials,
+                allow_methods=self.config.allow_methods,
+                allow_headers=self.config.allow_headers,
+            )
+
+            # Logic directly from Starlette"s CORSMiddleware:
+            # https://github.com/encode/starlette/blob/master/starlette/middleware/cors.py#L152
+
+            response.headers.update(mw.simple_headers)
+            has_cookie = "cookie" in request.headers
+
+            # If request includes any cookie headers, then we must respond
+            # with the specific origin instead of "*".
+            if mw.allow_all_origins and has_cookie:
+                response.headers["Access-Control-Allow-Origin"] = origin
+
+            # If we only allow specific origins, then we have to mirror back
+            # the Origin header in the response.
+            elif not mw.allow_all_origins and mw.is_allowed_origin(origin=origin):
+                response.headers["Access-Control-Allow-Origin"] = origin
+                response.headers.add_vary_header("Origin")
+
+        return response
```

