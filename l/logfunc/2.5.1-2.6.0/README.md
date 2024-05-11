# Comparing `tmp/logfunc-2.5.1.tar.gz` & `tmp/logfunc-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logfunc-2.5.1.tar", last modified: Fri May 10 21:25:00 2024, max compression
+gzip compressed data, was "logfunc-2.6.0.tar", last modified: Sat May 11 22:51:25 2024, max compression
```

## Comparing `logfunc-2.5.1.tar` & `logfunc-2.6.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 mym2       (501) staff       (20)        0 2024-05-10 21:25:00.761675 logfunc-2.5.1/
--rw-r--r--   0 mym2       (501) staff       (20)     1068 2023-09-03 19:49:58.000000 logfunc-2.5.1/LICENSE
--rw-r--r--   0 mym2       (501) staff       (20)     8661 2024-05-10 21:25:00.761510 logfunc-2.5.1/PKG-INFO
--rw-r--r--   0 mym2       (501) staff       (20)     6216 2024-05-10 01:36:04.000000 logfunc-2.5.1/README.md
-drwxr-xr-x   0 mym2       (501) staff       (20)        0 2024-05-10 21:25:00.760751 logfunc-2.5.1/logfunc/
--rw-r--r--   0 mym2       (501) staff       (20)       56 2024-05-10 21:20:35.000000 logfunc-2.5.1/logfunc/__init__.py
--rw-r--r--   0 mym2       (501) staff       (20)     2750 2024-05-10 01:36:11.000000 logfunc-2.5.1/logfunc/config.py
--rw-r--r--   0 mym2       (501) staff       (20)       21 2024-04-27 03:32:02.000000 logfunc-2.5.1/logfunc/defaults.py
--rw-r--r--   0 mym2       (501) staff       (20)     5799 2024-05-10 21:16:28.000000 logfunc-2.5.1/logfunc/main.py
--rw-r--r--   0 mym2       (501) staff       (20)      673 2024-02-23 01:13:48.000000 logfunc-2.5.1/logfunc/msgs.py
--rw-r--r--   0 mym2       (501) staff       (20)     3012 2024-05-10 01:36:21.000000 logfunc-2.5.1/logfunc/utils.py
--rw-r--r--   0 mym2       (501) staff       (20)       22 2024-05-10 21:20:54.000000 logfunc-2.5.1/logfunc/version.py
-drwxr-xr-x   0 mym2       (501) staff       (20)        0 2024-05-10 21:25:00.761287 logfunc-2.5.1/logfunc.egg-info/
--rw-r--r--   0 mym2       (501) staff       (20)     8661 2024-05-10 21:25:00.000000 logfunc-2.5.1/logfunc.egg-info/PKG-INFO
--rw-r--r--   0 mym2       (501) staff       (20)      291 2024-05-10 21:25:00.000000 logfunc-2.5.1/logfunc.egg-info/SOURCES.txt
--rw-r--r--   0 mym2       (501) staff       (20)        1 2024-05-10 21:25:00.000000 logfunc-2.5.1/logfunc.egg-info/dependency_links.txt
--rw-r--r--   0 mym2       (501) staff       (20)        8 2024-05-10 21:25:00.000000 logfunc-2.5.1/logfunc.egg-info/top_level.txt
--rw-r--r--   0 mym2       (501) staff       (20)     1217 2024-05-10 21:20:54.000000 logfunc-2.5.1/pyproject.toml
--rw-r--r--   0 mym2       (501) staff       (20)       38 2024-05-10 21:25:00.761725 logfunc-2.5.1/setup.cfg
--rw-r--r--   0 mym2       (501) staff       (20)     1237 2024-05-10 01:40:24.000000 logfunc-2.5.1/setup.py
+drwxr-xr-x   0 mym2       (501) staff       (20)        0 2024-05-11 22:51:25.615986 logfunc-2.6.0/
+-rw-r--r--   0 mym2       (501) staff       (20)     1068 2023-09-03 19:49:58.000000 logfunc-2.6.0/LICENSE
+-rw-r--r--   0 mym2       (501) staff       (20)     8257 2024-05-11 22:51:25.615807 logfunc-2.6.0/PKG-INFO
+-rw-r--r--   0 mym2       (501) staff       (20)     5812 2024-05-11 22:50:45.000000 logfunc-2.6.0/README.md
+drwxr-xr-x   0 mym2       (501) staff       (20)        0 2024-05-11 22:51:25.615091 logfunc-2.6.0/logfunc/
+-rw-r--r--   0 mym2       (501) staff       (20)       56 2024-05-10 21:20:35.000000 logfunc-2.6.0/logfunc/__init__.py
+-rw-r--r--   0 mym2       (501) staff       (20)     2822 2024-05-11 22:21:16.000000 logfunc-2.6.0/logfunc/config.py
+-rw-r--r--   0 mym2       (501) staff       (20)       44 2024-05-11 18:23:56.000000 logfunc-2.6.0/logfunc/defaults.py
+-rw-r--r--   0 mym2       (501) staff       (20)     6656 2024-05-11 22:48:04.000000 logfunc-2.6.0/logfunc/main.py
+-rw-r--r--   0 mym2       (501) staff       (20)      673 2024-02-23 01:13:48.000000 logfunc-2.6.0/logfunc/msgs.py
+-rw-r--r--   0 mym2       (501) staff       (20)     3238 2024-05-11 19:27:12.000000 logfunc-2.6.0/logfunc/utils.py
+-rw-r--r--   0 mym2       (501) staff       (20)       22 2024-05-11 22:31:27.000000 logfunc-2.6.0/logfunc/version.py
+drwxr-xr-x   0 mym2       (501) staff       (20)        0 2024-05-11 22:51:25.615603 logfunc-2.6.0/logfunc.egg-info/
+-rw-r--r--   0 mym2       (501) staff       (20)     8257 2024-05-11 22:51:25.000000 logfunc-2.6.0/logfunc.egg-info/PKG-INFO
+-rw-r--r--   0 mym2       (501) staff       (20)      291 2024-05-11 22:51:25.000000 logfunc-2.6.0/logfunc.egg-info/SOURCES.txt
+-rw-r--r--   0 mym2       (501) staff       (20)        1 2024-05-11 22:51:25.000000 logfunc-2.6.0/logfunc.egg-info/dependency_links.txt
+-rw-r--r--   0 mym2       (501) staff       (20)        8 2024-05-11 22:51:25.000000 logfunc-2.6.0/logfunc.egg-info/top_level.txt
+-rw-r--r--   0 mym2       (501) staff       (20)     1217 2024-05-11 22:31:27.000000 logfunc-2.6.0/pyproject.toml
+-rw-r--r--   0 mym2       (501) staff       (20)       38 2024-05-11 22:51:25.616028 logfunc-2.6.0/setup.cfg
+-rw-r--r--   0 mym2       (501) staff       (20)     1237 2024-05-10 01:40:24.000000 logfunc-2.6.0/setup.py
```

### Comparing `logfunc-2.5.1/LICENSE` & `logfunc-2.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `logfunc-2.5.1/PKG-INFO` & `logfunc-2.6.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logfunc
-Version: 2.5.1
+Version: 2.6.0
 Summary: An EASY TO USE function decorator for advanced logging of function execution, including arguments, return values, and execution time.
 Home-page: https://github.com/cc-d/logf/
 Author: Cary Carter
 Author-email: Cary Carter <ccarterdev@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Cary Carter
@@ -101,14 +101,15 @@
 - `log_args` & `log_return`: Control whether to log arguments and return values.
 - `max_str_len`: Limit the length of logged strings.
 - `log_exec_time`: Option to log the execution time.
 - `single_msg`: Consolidate all log data into a single message.
 - `use_print`: Choose to `print()` log messages instead of using standard logging.
 - `log_stack_info`: Pass `stack_info=$x` to `.log()` but not print
 - `use_logger`: Pass a logger name or logger object to use instead of logging.log
+- `identifier`: Add a unique identifier to enter/exit log messages.
 
 **print_all** used to be an env var, now just unset LOGF_LEVEL and set USE_PRINT=True for the same effect.
 
 ### Environment Variable Overrides
 
 Modify the behavior of `@logf()` using environment variables:
 
@@ -120,49 +121,48 @@
 | LOGF_USE_PRINT     | True, False          |
 | LOGF_STACK_INFO    | True, False          |
 | LOGF_LOG_EXEC_TIME | True, False          |
 | LOGF_LOG_ARGS      | True, False          |
 | LOGF_LOG_RETURN    | True, False          |
 | LOGF_USE_LOGGER    | 'logger_name'        |
 | LOGF_LOG_LEVEL     | DEBUG, INFO, WARNING |
+| LOGF_IDENTIFIER    | True, False          |
 
 See the following output for an example of how an env var will affect `@logf()` behaviour:
 
-Without `LOGF_USE_PRINT`:
+With `LOGF_USE_PRINT=True`:
 
 ```
-mym2@Carys-MacBook-Pro liberfy-cli % ./cli user me
-Namespace(cmd='user', act='me')
-email='a@a.a' id='a4c3f7ac-4649-4e74-ad07-1cd8e9626bbc'
-```
-
-With `LOGF_USE_PRINT=True`: (jwt here isnt sensitive so no worries)
-
-```
-mym2@Carys-MacBook-Pro liberfy-cli % LOGF_USE_PRINT=True ./cli user me
-async_main | () {}
-setup_argparse | () {}
-setup_argparse() 0.00144s | ArgumentParser(prog='main.py', usage=None, description='CLI for user, project, sync directory, and directory file management.', formatter_class=<class 'argparse.HelpFormatter'>, conflict_handler='error', add_help=True)
-apicmd | (ArgumentParser(prog='main.py', usage=None, description='CLI for user, project, sync directory, and directory file management.', formatter_class=<class 'argparse.HelpFormatter'>, conflict_handler='error', add_help=True),) {}
-Namespace(cmd='user', act='me')
-me | () {}
-get | ('/u/me',) {}
-_method | ('get', '/u/me') {}
-_inject_auth | ({},) {}
-load_token | () {}
-load_token() 0.00004s | eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJleHAiOjE2OTQ1NTQ1MjAsInN1YiI6ImFAYS5hIiwiaWF0IjoxNjk0NTQ3MzIwfQ.p6NPOEAedaV6SzBkv3XYWTGmZ4sdAEshk76wacV6Jlw
-_inject_auth() 0.00005s | {'headers': {'Authorization': 'Bearer eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJleHAiOjE2OTQ1NTQ1MjAsInN1YiI6ImFAYS5hIiwiaWF0IjoxNjk0NTQ3MzIwfQ.p6NPOEAedaV6SzBkv3XYWTGmZ4sdAEshk76wacV6Jlw'}}
-resp_exceptions | (<Response [200 OK]>,) {}
-resp_exceptions() 0.00002s | None
-_method() 0.01756s | {'email': 'a@a.a', 'id': 'a4c3f7ac-4649-4e74-ad07-1cd8e9626bbc'}
-get() 0.01757s | {'email': 'a@a.a', 'id': 'a4c3f7ac-4649-4e74-ad07-1cd8e9626bbc'}
-me() 0.01760s | email='a@a.a' id='a4c3f7ac-4649-4e74-ad07-1cd8e9626bbc'
-apicmd() 0.01773s | email='a@a.a' id='a4c3f7ac-4649-4e74-ad07-1cd8e9626bbc'
-email='a@a.a' id='a4c3f7ac-4649-4e74-ad07-1cd8e9626bbc'
-async_main() 0.01922s | email='a@a.a' id='a4c3f7ac-4649-4e74-ad07-1cd8e9626bbc'
+mym2@Carys-MacBook-Pro logf % gitpoll ~/test
+Running once...
+-> __init__()[CwKVbK] | (<CmdExec >, 'git rev-parse --abbrev-ref HEAD') {}
+<- __init__()[CwKVbK] 0.0048s | None
+-> __init__()[BIimGf] | (<CmdExec >, 'git config --get branch.test.remote') {}
+<- __init__()[BIimGf] 0.0040s | None
+-> __init__()[ED1XW0] | (<CmdExec >, 'git config --get branch.test.merge') {}
+<- __init__()[ED1XW0] 0.0039s | None
+-> __init__()[dsPXjJ] | (<CmdExec >, 'git rev-parse refs/remotes//') {}
+<- __init__()[dsPXjJ] 0.0044s | None
+-> __init__()[5rkgc9] | (<CmdExec >, 'git rev-parse HEAD') {}
+<- __init__()[5rkgc9] 0.0037s | None
+-> __init__()[GDti62] | (<CmdExec >, 'git fetch') {}
+<- __init__()[GDti62] 1.1160s | None
+```
+
+With `LOGF_SINGLE_MSG=True`:
+
+```
+mym2@Carys-MacBook-Pro logf % gitpoll ~/test
+Running once...
+__init__() 0.0050s | (<CmdExec >, 'git rev-parse --abbrev-ref HEAD') {} | None
+__init__() 0.0041s | (<CmdExec >, 'git config --get branch.test.remote') {} | None
+__init__() 0.0041s | (<CmdExec >, 'git config --get branch.test.merge') {} | None
+__init__() 0.0041s | (<CmdExec >, 'git rev-parse refs/remotes//') {} | None
+__init__() 0.0038s | (<CmdExec >, 'git rev-parse HEAD') {} | None
+__init__() 1.0993s | (<CmdExec >, 'git fetch') {} | None
 ```
 
 ### Real-world Examples
 
 Here are a couple of real-world examples of `@logf()` usage:
 
 ```python
@@ -192,23 +192,26 @@
 
 Output should look like this:
 
 ```sh
 ---------- coverage: platform darwin, python 3.11.5-final-0 ----------
 Name                  Stmts   Miss  Cover   Missing
 ---------------------------------------------------
-logfunc/__init__.py       1      0   100%
-logfunc/config.py        22      0   100%
-logfunc/defaults.py       1      0   100%
-logfunc/main.py         107      0   100%
-logfunc/utils.py         28      0   100%
-tests.py                282      0   100%
+logfunc/__init__.py       2      0   100%
+logfunc/config.py        59      0   100%
+logfunc/defaults.py       2      0   100%
+logfunc/main.py          69      0   100%
+logfunc/msgs.py           8      0   100%
+logfunc/utils.py         35      0   100%
+logfunc/version.py        1      0   100%
 ---------------------------------------------------
-TOTAL                   441      0   100%
+TOTAL                   176      0   100%
 
+
+==================================== 25 passed in 0.06s
 ```
 
 You can also just run the `tests.py` file directly.
 
 ## Contributing
 
 Contributions are welcome! Please feel free to submit a pull request or open an issue.
```

### Comparing `logfunc-2.5.1/logfunc/config.py` & `logfunc-2.6.0/logfunc/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     'LOGF_LEVEL',
     'LOGF_LOG_ARGS',
     'LOGF_LOG_RETURN',
     'LOGF_LOG_EXEC_TIME',
     'LOGF_USE_LOGGER',
     'LOGF_LOG_LEVEL',
     'LOGF_STACK_INFO',
+    'LOGF_IDENTIFIER',
 )
 
 
 class Cfg:
     def __init__(self, **kwargs):
         self.level = kwargs.get('level')
         self.max_str = kwargs.get('max_str_len')
@@ -33,14 +34,15 @@
         self.single = kwargs.get('single_msg')
         self.use_print = kwargs.get('use_print')
         self.log_args = kwargs.get('log_args')
         self.log_return = kwargs.get('log_return')
         self.use_logger = kwargs.get('use_logger')
         self.logf_log_level = kwargs.get('logf_log_level')
         self.log_stack = kwargs.get('log_stack_info')
+        self.identifier = kwargs.get('identifier')
 
         # Override attributes based on environment variables
         for ev in EVARS:
             _ev = os.environ.get(ev)
             if _ev is not None:
                 if ev == 'LOGF_MAX_STR_LEN':
                     self.max_str = None if _ev.lower() == 'none' else int(_ev)
@@ -54,25 +56,25 @@
                     self.log_return = _ev.lower() == 'true'
                 elif ev == 'LOGF_LOG_EXEC_TIME':
                     self.log_time = _ev.lower() == 'true'
                 elif ev == 'LOGF_USE_LOGGER':
                     self.use_logger = getLogger(_ev) if _ev else None
                 elif ev == 'LOGF_STACK_INFO':
                     self.log_stack = _ev.lower() == 'true'
-                elif ev == 'LOGF_SINGLE_EXCEPTION':
-                    self.single_ex = _ev.lower() == 'true'
                 elif ev == 'LOGF_LOG_LEVEL':
                     self.logf_log_level = str(_ev).upper()
+                elif ev == 'LOGF_IDENTIFIER':
+                    self.identifier = _ev.lower() == 'true'
 
 
 ARGSSTR = '{func_args} {func_kwargs}'
-ENTER_MSG = '{func_name}() | {args_str}'
-EXIT_MSG_NO_RETURN = '{func_name}() {exec_time}s'
-EXIT_MSG = '{func_name}() {exec_time}s | {result}'
-SINGLE_MSG = '{func_name}() {exec_time}s | {args_str} | {result}'
+ENTER_MSG = '-> {func_name}() | {args_str}'
+EXIT_MSG_NO_RETURN = '{func_name}() {exec_time}'
+EXIT_MSG = '<- {func_name}() {exec_time} | {result}'
+SINGLE_MSG = '{func_name}() {exec_time} | {args_str} | {result}'
 ENTER_MSG_NO_ARGS = '{func_name}()'
 
 
 class MSG_FORMATS:
     argstr = ARGSSTR
     enter = ENTER_MSG
     enter_no_args = ENTER_MSG_NO_ARGS
```

### Comparing `logfunc-2.5.1/logfunc/main.py` & `logfunc-2.6.0/logfunc/main.py`

 * *Files 20% similar despite different names*

```diff
@@ -20,32 +20,39 @@
     Iterable,
     Coroutine as Co,
     List,
     Tuple,
 )
 from logging import getLogger, Logger
 
-from .utils import loglevel_int, handle_log, trunc_str, build_argstr
+from .utils import (
+    loglevel_int,
+    handle_log,
+    trunc_str,
+    build_argstr,
+    identifier as _get_id,
+)
 from .config import EVARS, MSG_FORMATS, Cfg
 
-from .defaults import TRUNC_STR_LEN
+from .defaults import TRUNC_STR_LEN, EXEC_TIME_FMT
 
 from . import msgs
 
 
 def logf(
     level: Opt[U[int, str]] = None,
     log_args: bool = True,
     log_return: bool = True,
     max_str_len: U[int, None] = TRUNC_STR_LEN,
     log_exec_time: bool = True,
     single_msg: bool = False,
     use_print: bool = False,
     use_logger: Opt[U[Logger, str]] = None,
     log_stack_info: bool = False,
+    identifier: bool = True,
     **kwargs
 ) -> U[Call[..., Any], Co[Any, Any, Any]]:
     """A highly customizable function decorator meant for effortless
     leave-and-forget logging of function calls, both synchronous and
     asynchronous. Logs the function name, arguments, return value and
     execution time.
     Args:
@@ -63,29 +70,33 @@
             into a single message? Default False
         use_print (bool): Should the log messages be printed instead of logged?
             Default False
         use_logger (Optional[Union[Logger, str]]): logger/logger name
             to use for  Defaults to None. If None, log is used.
         log_stack_info (bool): stack_info kwarg for log
             Can be overridden by the evar LOGF_STACK_INFO.
-            Defaults to False
+            Default: False
+        identifier (bool): A unique identifier for enter/exits. Equivalent to
+            evar LOGF_IDENTIFIER.
+            Default: True
     Returns:
         The executed decorated function or coroutine result.
     """
 
     cfg = Cfg(
         level=level,
         max_str_len=max_str_len,
         log_exec_time=kwargs.get('measure_time', log_exec_time),
         single_msg=single_msg,
         log_stack_info=log_stack_info,
         use_print=use_print,
         log_args=log_args,
         log_return=log_return,
         use_logger=use_logger,
+        identifier=identifier,
     )
 
     # if param use_logger is a string, convert it to a logger
     if cfg.use_logger is not None and not isinstance(cfg.use_logger, Logger):
         cfg.use_logger = getLogger(use_logger)
 
     def wrapper(func: Call[..., Any]) -> U[Call[..., Any], Co[Any, Any, Any]]:
@@ -93,90 +104,119 @@
 
         # ensure only last traceback is logged
 
         if _insp.iscoroutinefunction(func):
 
             @wraps(func)
             async def decorator(*args, **kwargs) -> Any:
+                _id = _get_id() if cfg.identifier and not cfg.single else None
 
                 _start = aio.get_event_loop().time() if cfg.log_time else None
-                argstr = _enter(fname, args, kwargs, cfg)
+                argstr = _enter(fname, args, kwargs, cfg, _id)
                 result = await func(*args, **kwargs)
 
                 _msg_exit(
                     result,
                     fname,
                     argstr,
                     _endtime(_start, aio.get_event_loop().time()),
                     cfg,
+                    _id,
                 )
 
                 return result
 
         # handle sync funcs
         else:
 
             @wraps(func)
             def decorator(*args, **kwargs) -> Any:
-
+                _id = _get_id() if cfg.identifier and not cfg.single else None
                 _start = time.time() if cfg.log_time else None
-                argstr = _enter(fname, args, kwargs, cfg)
+                argstr = _enter(fname, args, kwargs, cfg, _id)
                 result = func(*args, **kwargs)
 
                 _msg_exit(
-                    result, fname, _endtime(_start, time.time()), argstr, cfg
+                    result,
+                    fname,
+                    _endtime(_start, time.time()),
+                    argstr,
+                    cfg,
+                    _id,
                 )
                 return result
 
         return decorator
 
     return wrapper
 
 
-def _msg_enter(func_name: str, args_str: str, cfg: Cfg) -> None:
+def _msg_enter(
+    func_name: str, args_str: str, cfg: Cfg, id: U[str, None]
+) -> None:
     """Handles logging of the enter message for decorated functions."""
     if cfg.level is not None and cfg.logf_log_level is not None:
         if loglevel_int(cfg.level) < loglevel_int(cfg.logf_log_level):
             return
+
     logmsg = MSG_FORMATS.enter.format(func_name=func_name, args_str=args_str)
 
+    if id is not None:
+
+        logmsg = logmsg.replace('()', '()[%s]' % id, 1)
+
     if cfg.use_print:
         print(logmsg)
     else:
         handle_log(
             logmsg, cfg.level, cfg.use_logger, log_stack_info=cfg.log_stack
         )
 
+
 def _msg_exit(
-    result: Any, func_name: str, end_time: str, args_str: str, cfg: Cfg
+    result: Any,
+    func_name: str,
+    end_time: str,
+    args_str: str,
+    cfg: Cfg,
+    id: U[str, None],
 ) -> None:
     """Handles logging of the exit message for decorated functions."""
     if cfg.level is not None and cfg.logf_log_level is not None:
         if loglevel_int(cfg.level) < loglevel_int(cfg.logf_log_level):
             return
+
     logmsg = msgs.exit_msg(
         cfg.single,
         func_name,
         end_time,
         args_str,
         trunc_str(result, cfg.max_str) if cfg.log_return else '',
     )
+    if id is not None:
+        logmsg = logmsg.replace('()', '()[%s]' % id, 1)
 
     if cfg.use_print:
         print(logmsg)
     else:
         handle_log(
             logmsg, cfg.level, cfg.use_logger, log_stack_info=cfg.log_stack
         )
 
 
 def _endtime(start_time: U[float, None], end_time: U[float, None]) -> str:
     """Returns the time elapsed since the start time."""
-    return '' if start_time is None else '%.5f' % (end_time - start_time)
+    return (
+        ''
+        if start_time is None
+        else (EXEC_TIME_FMT % (end_time - start_time)) + 's'
+    )
 
 
-def _enter(func_name: str, args: Tuple, kwargs: Dict, cfg: Cfg) -> str:
+def _enter(
+    func_name: str, args: Tuple, kwargs: Dict, cfg: Cfg, id: U[str, None]
+) -> str:
     """Handles the enter for decorated functions and returns argstr"""
     argstr = build_argstr(args, kwargs, cfg.max_str, cfg.log_args)
     if not cfg.single:
-        _msg_enter(func_name, argstr, cfg)
+        _msg_enter(func_name, argstr, cfg, id)
     return argstr
```

### Comparing `logfunc-2.5.1/logfunc/msgs.py` & `logfunc-2.6.0/logfunc/msgs.py`

 * *Files identical despite different names*

### Comparing `logfunc-2.5.1/logfunc/utils.py` & `logfunc-2.6.0/logfunc/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,27 +1,13 @@
 import asyncio
 import logging
-import os
-import re
-import sys
-import time
-import traceback
+from random import choice
 import inspect as _insp
-from typing import (
-    Any,
-    Callable,
-    Dict,
-    Optional as Opt,
-    Tuple,
-    TypeVar,
-    Union,
-    Iterable,
-    Coroutine,
-)
-from .config import EVARS
+from typing import Any, Callable, Dict, Optional as Opt, Tuple, Union
+from .config import EVARS, ID_CHARS, ID_LEN
 from .msgs import MSG_FORMATS
 from .defaults import TRUNC_STR_LEN
 
 
 def build_argstr(
     args: Tuple, kwargs: Dict, max_length: Union[int, None], log_args: bool
 ) -> str:
@@ -97,7 +83,17 @@
     """
     level_int = loglevel_int(level) if level is not None else logging.DEBUG
 
     logfunc = logging.log if use_logger is None else use_logger.log
     logfunc(level_int, logmsg, stack_info=log_stack_info)
 
     return logfunc
+
+
+def identifier(len=ID_LEN, chars=ID_CHARS) -> str:
+    """Generates a random identifier string of a specified length.
+    ~len: the length of the identifier
+    ~chars: the characters to choose from
+    -> str: the msg with the identifier inserted
+    """
+
+    return ''.join(choice(chars) for _ in range(len))
```

### Comparing `logfunc-2.5.1/logfunc.egg-info/PKG-INFO` & `logfunc-2.6.0/logfunc.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logfunc
-Version: 2.5.1
+Version: 2.6.0
 Summary: An EASY TO USE function decorator for advanced logging of function execution, including arguments, return values, and execution time.
 Home-page: https://github.com/cc-d/logf/
 Author: Cary Carter
 Author-email: Cary Carter <ccarterdev@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Cary Carter
@@ -101,14 +101,15 @@
 - `log_args` & `log_return`: Control whether to log arguments and return values.
 - `max_str_len`: Limit the length of logged strings.
 - `log_exec_time`: Option to log the execution time.
 - `single_msg`: Consolidate all log data into a single message.
 - `use_print`: Choose to `print()` log messages instead of using standard logging.
 - `log_stack_info`: Pass `stack_info=$x` to `.log()` but not print
 - `use_logger`: Pass a logger name or logger object to use instead of logging.log
+- `identifier`: Add a unique identifier to enter/exit log messages.
 
 **print_all** used to be an env var, now just unset LOGF_LEVEL and set USE_PRINT=True for the same effect.
 
 ### Environment Variable Overrides
 
 Modify the behavior of `@logf()` using environment variables:
 
@@ -120,49 +121,48 @@
 | LOGF_USE_PRINT     | True, False          |
 | LOGF_STACK_INFO    | True, False          |
 | LOGF_LOG_EXEC_TIME | True, False          |
 | LOGF_LOG_ARGS      | True, False          |
 | LOGF_LOG_RETURN    | True, False          |
 | LOGF_USE_LOGGER    | 'logger_name'        |
 | LOGF_LOG_LEVEL     | DEBUG, INFO, WARNING |
+| LOGF_IDENTIFIER    | True, False          |
 
 See the following output for an example of how an env var will affect `@logf()` behaviour:
 
-Without `LOGF_USE_PRINT`:
+With `LOGF_USE_PRINT=True`:
 
 ```
-mym2@Carys-MacBook-Pro liberfy-cli % ./cli user me
-Namespace(cmd='user', act='me')
-email='a@a.a' id='a4c3f7ac-4649-4e74-ad07-1cd8e9626bbc'
-```
-
-With `LOGF_USE_PRINT=True`: (jwt here isnt sensitive so no worries)
-
-```
-mym2@Carys-MacBook-Pro liberfy-cli % LOGF_USE_PRINT=True ./cli user me
-async_main | () {}
-setup_argparse | () {}
-setup_argparse() 0.00144s | ArgumentParser(prog='main.py', usage=None, description='CLI for user, project, sync directory, and directory file management.', formatter_class=<class 'argparse.HelpFormatter'>, conflict_handler='error', add_help=True)
-apicmd | (ArgumentParser(prog='main.py', usage=None, description='CLI for user, project, sync directory, and directory file management.', formatter_class=<class 'argparse.HelpFormatter'>, conflict_handler='error', add_help=True),) {}
-Namespace(cmd='user', act='me')
-me | () {}
-get | ('/u/me',) {}
-_method | ('get', '/u/me') {}
-_inject_auth | ({},) {}
-load_token | () {}
-load_token() 0.00004s | eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJleHAiOjE2OTQ1NTQ1MjAsInN1YiI6ImFAYS5hIiwiaWF0IjoxNjk0NTQ3MzIwfQ.p6NPOEAedaV6SzBkv3XYWTGmZ4sdAEshk76wacV6Jlw
-_inject_auth() 0.00005s | {'headers': {'Authorization': 'Bearer eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJleHAiOjE2OTQ1NTQ1MjAsInN1YiI6ImFAYS5hIiwiaWF0IjoxNjk0NTQ3MzIwfQ.p6NPOEAedaV6SzBkv3XYWTGmZ4sdAEshk76wacV6Jlw'}}
-resp_exceptions | (<Response [200 OK]>,) {}
-resp_exceptions() 0.00002s | None
-_method() 0.01756s | {'email': 'a@a.a', 'id': 'a4c3f7ac-4649-4e74-ad07-1cd8e9626bbc'}
-get() 0.01757s | {'email': 'a@a.a', 'id': 'a4c3f7ac-4649-4e74-ad07-1cd8e9626bbc'}
-me() 0.01760s | email='a@a.a' id='a4c3f7ac-4649-4e74-ad07-1cd8e9626bbc'
-apicmd() 0.01773s | email='a@a.a' id='a4c3f7ac-4649-4e74-ad07-1cd8e9626bbc'
-email='a@a.a' id='a4c3f7ac-4649-4e74-ad07-1cd8e9626bbc'
-async_main() 0.01922s | email='a@a.a' id='a4c3f7ac-4649-4e74-ad07-1cd8e9626bbc'
+mym2@Carys-MacBook-Pro logf % gitpoll ~/test
+Running once...
+-> __init__()[CwKVbK] | (<CmdExec >, 'git rev-parse --abbrev-ref HEAD') {}
+<- __init__()[CwKVbK] 0.0048s | None
+-> __init__()[BIimGf] | (<CmdExec >, 'git config --get branch.test.remote') {}
+<- __init__()[BIimGf] 0.0040s | None
+-> __init__()[ED1XW0] | (<CmdExec >, 'git config --get branch.test.merge') {}
+<- __init__()[ED1XW0] 0.0039s | None
+-> __init__()[dsPXjJ] | (<CmdExec >, 'git rev-parse refs/remotes//') {}
+<- __init__()[dsPXjJ] 0.0044s | None
+-> __init__()[5rkgc9] | (<CmdExec >, 'git rev-parse HEAD') {}
+<- __init__()[5rkgc9] 0.0037s | None
+-> __init__()[GDti62] | (<CmdExec >, 'git fetch') {}
+<- __init__()[GDti62] 1.1160s | None
+```
+
+With `LOGF_SINGLE_MSG=True`:
+
+```
+mym2@Carys-MacBook-Pro logf % gitpoll ~/test
+Running once...
+__init__() 0.0050s | (<CmdExec >, 'git rev-parse --abbrev-ref HEAD') {} | None
+__init__() 0.0041s | (<CmdExec >, 'git config --get branch.test.remote') {} | None
+__init__() 0.0041s | (<CmdExec >, 'git config --get branch.test.merge') {} | None
+__init__() 0.0041s | (<CmdExec >, 'git rev-parse refs/remotes//') {} | None
+__init__() 0.0038s | (<CmdExec >, 'git rev-parse HEAD') {} | None
+__init__() 1.0993s | (<CmdExec >, 'git fetch') {} | None
 ```
 
 ### Real-world Examples
 
 Here are a couple of real-world examples of `@logf()` usage:
 
 ```python
@@ -192,23 +192,26 @@
 
 Output should look like this:
 
 ```sh
 ---------- coverage: platform darwin, python 3.11.5-final-0 ----------
 Name                  Stmts   Miss  Cover   Missing
 ---------------------------------------------------
-logfunc/__init__.py       1      0   100%
-logfunc/config.py        22      0   100%
-logfunc/defaults.py       1      0   100%
-logfunc/main.py         107      0   100%
-logfunc/utils.py         28      0   100%
-tests.py                282      0   100%
+logfunc/__init__.py       2      0   100%
+logfunc/config.py        59      0   100%
+logfunc/defaults.py       2      0   100%
+logfunc/main.py          69      0   100%
+logfunc/msgs.py           8      0   100%
+logfunc/utils.py         35      0   100%
+logfunc/version.py        1      0   100%
 ---------------------------------------------------
-TOTAL                   441      0   100%
+TOTAL                   176      0   100%
 
+
+==================================== 25 passed in 0.06s
 ```
 
 You can also just run the `tests.py` file directly.
 
 ## Contributing
 
 Contributions are welcome! Please feel free to submit a pull request or open an issue.
```

### Comparing `logfunc-2.5.1/pyproject.toml` & `logfunc-2.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=40.6.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "logfunc"
-version = '2.5.1'
+version = '2.6.0'
 description = "An EASY TO USE function decorator for advanced logging of function execution, including arguments, return values, and execution time."
 authors = [{name = "Cary Carter", email = "ccarterdev@gmail.com"}]
 license = {file = "LICENSE"}
 readme = "README.md"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
```

### Comparing `logfunc-2.5.1/setup.py` & `logfunc-2.6.0/setup.py`

 * *Files identical despite different names*

