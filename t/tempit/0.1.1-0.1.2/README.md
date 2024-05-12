# Comparing `tmp/tempit-0.1.1.tar.gz` & `tmp/tempit-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tempit-0.1.1.tar", last modified: Sat May 11 15:04:11 2024, max compression
+gzip compressed data, was "tempit-0.1.2.tar", last modified: Sun May 12 18:23:18 2024, max compression
```

## Comparing `tempit-0.1.1.tar` & `tempit-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 mcrespo    (501) staff       (20)        0 2024-05-11 15:04:11.699437 tempit-0.1.1/
--rw-r--r--   0 mcrespo    (501) staff       (20)     1068 2024-05-11 14:15:52.000000 tempit-0.1.1/LICENSE.txt
--rw-r--r--   0 mcrespo    (501) staff       (20)     3325 2024-05-11 15:04:11.699227 tempit-0.1.1/PKG-INFO
--rw-r--r--   0 mcrespo    (501) staff       (20)     2789 2024-05-11 14:15:52.000000 tempit-0.1.1/README.md
--rw-r--r--   0 mcrespo    (501) staff       (20)       38 2024-05-11 15:04:11.699482 tempit-0.1.1/setup.cfg
--rw-r--r--   0 mcrespo    (501) staff       (20)      736 2024-05-11 15:02:14.000000 tempit-0.1.1/setup.py
-drwxr-xr-x   0 mcrespo    (501) staff       (20)        0 2024-05-11 15:04:11.698073 tempit-0.1.1/tempit/
--rw-r--r--   0 mcrespo    (501) staff       (20)       47 2024-05-11 14:15:52.000000 tempit-0.1.1/tempit/__init__.py
--rw-r--r--   0 mcrespo    (501) staff       (20)     9352 2024-05-11 14:15:52.000000 tempit-0.1.1/tempit/core.py
--rw-r--r--   0 mcrespo    (501) staff       (20)     5353 2024-05-11 14:15:52.000000 tempit-0.1.1/tempit/utils.py
-drwxr-xr-x   0 mcrespo    (501) staff       (20)        0 2024-05-11 15:04:11.699020 tempit-0.1.1/tempit.egg-info/
--rw-r--r--   0 mcrespo    (501) staff       (20)     3325 2024-05-11 15:04:11.000000 tempit-0.1.1/tempit.egg-info/PKG-INFO
--rw-r--r--   0 mcrespo    (501) staff       (20)      221 2024-05-11 15:04:11.000000 tempit-0.1.1/tempit.egg-info/SOURCES.txt
--rw-r--r--   0 mcrespo    (501) staff       (20)        1 2024-05-11 15:04:11.000000 tempit-0.1.1/tempit.egg-info/dependency_links.txt
--rw-r--r--   0 mcrespo    (501) staff       (20)        7 2024-05-11 15:04:11.000000 tempit-0.1.1/tempit.egg-info/top_level.txt
-drwxr-xr-x   0 mcrespo    (501) staff       (20)        0 2024-05-11 15:04:11.698768 tempit-0.1.1/tests/
--rw-r--r--   0 mcrespo    (501) staff       (20)    10413 2024-05-11 14:15:52.000000 tempit-0.1.1/tests/test_tempit.py
+drwxr-xr-x   0 mcrespo    (501) staff       (20)        0 2024-05-12 18:23:18.932289 tempit-0.1.2/
+-rw-r--r--   0 mcrespo    (501) staff       (20)     1068 2024-05-11 14:15:52.000000 tempit-0.1.2/LICENSE.txt
+-rw-r--r--   0 mcrespo    (501) staff       (20)     3748 2024-05-12 18:23:18.932033 tempit-0.1.2/PKG-INFO
+-rw-r--r--   0 mcrespo    (501) staff       (20)     3128 2024-05-12 10:42:15.000000 tempit-0.1.2/README.md
+-rw-r--r--   0 mcrespo    (501) staff       (20)       38 2024-05-12 18:23:18.932341 tempit-0.1.2/setup.cfg
+-rw-r--r--   0 mcrespo    (501) staff       (20)      808 2024-05-12 17:03:50.000000 tempit-0.1.2/setup.py
+drwxr-xr-x   0 mcrespo    (501) staff       (20)        0 2024-05-12 18:23:18.930832 tempit-0.1.2/tempit/
+-rw-r--r--   0 mcrespo    (501) staff       (20)       47 2024-05-11 14:15:52.000000 tempit-0.1.2/tempit/__init__.py
+-rw-r--r--   0 mcrespo    (501) staff       (20)     9442 2024-05-12 18:10:08.000000 tempit-0.1.2/tempit/core.py
+-rw-r--r--   0 mcrespo    (501) staff       (20)     5353 2024-05-12 10:36:44.000000 tempit-0.1.2/tempit/utils.py
+drwxr-xr-x   0 mcrespo    (501) staff       (20)        0 2024-05-12 18:23:18.931822 tempit-0.1.2/tempit.egg-info/
+-rw-r--r--   0 mcrespo    (501) staff       (20)     3748 2024-05-12 18:23:18.000000 tempit-0.1.2/tempit.egg-info/PKG-INFO
+-rw-r--r--   0 mcrespo    (501) staff       (20)      250 2024-05-12 18:23:18.000000 tempit-0.1.2/tempit.egg-info/SOURCES.txt
+-rw-r--r--   0 mcrespo    (501) staff       (20)        1 2024-05-12 18:23:18.000000 tempit-0.1.2/tempit.egg-info/dependency_links.txt
+-rw-r--r--   0 mcrespo    (501) staff       (20)        7 2024-05-12 18:23:18.000000 tempit-0.1.2/tempit.egg-info/requires.txt
+-rw-r--r--   0 mcrespo    (501) staff       (20)        7 2024-05-12 18:23:18.000000 tempit-0.1.2/tempit.egg-info/top_level.txt
+drwxr-xr-x   0 mcrespo    (501) staff       (20)        0 2024-05-12 18:23:18.931587 tempit-0.1.2/tests/
+-rw-r--r--   0 mcrespo    (501) staff       (20)    12230 2024-05-12 18:04:54.000000 tempit-0.1.2/tests/test_tempit.py
```

### Comparing `tempit-0.1.1/LICENSE.txt` & `tempit-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tempit-0.1.1/PKG-INFO` & `tempit-0.1.2/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: tempit
-Version: 0.1.1
-Summary: A dead simple time decorator
-Home-page: https://github.com/mcrespoae/tempit
-Author: mcrespoae
-Author-email: info@mariocrespo.es
-Keywords: tempit,time,decorator,performance,multithreading,benchmark
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Intended Audience :: Developers
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 # Tempit
 
 Tempit is a Python package designed to simplify the process of measuring the execution time of your functions through a straightforward decorator.
 
 ## Installation
 
 You can install Tempit using pip:
@@ -49,15 +33,15 @@
 Function my_function took 10.5908ms.
 ```
 
 ### Advanced Usage
 
 ```python
 from tempit import tempit
-@tempit(run_times=20, concurrency_mode="multithreading", verbose=True)
+@tempit(run_times=20, concurrent_execution=True, verbose=True)
 def my_function_with_args(a:int = 1, b:int = 2):
     return a + b
 
 result = my_function_with_args(1, b=2)
 ```
 
 This will provide detailed output:
@@ -82,24 +66,24 @@
 More examples can be found in the [examples.py](examples/examples.py) script.
 
 ## Features
 
 - Simplified usage.
 - Accurate measurement of function execution time.
 - Support for `classmethod` and `staticmethods`.
-- Multithreading mode for performance measurement.
+- Parallel execution mode for performance measurement.
 - Human-readable time formatting.
 - Optional verbose mode for detailed information.
 
 ## Parameters
 
 Using the decorator @tempit without any parameters executes the function once and displays the execution time. However, you can enhance the experience using the following arguments:
 
 - `run_times` (int, optional): Specifies the number of function executions. Defaults to 1.
-- `concurrency_mode` (str, optional): Determines the concurrency mode for function execution. Options are "multithreading" and "none". Defaults to "multithreading".
+- `concurrency_mode` (bool, optional): Determines the concurrency mode for the function execution. It uses [joblib](https://pypi.org/project/joblib/) for parallel computing. The  default execution backend is "loky" but if the function is being triggered other than the main thread or main process, the backend will be changed to multithreading to aovid pickle errors. If, for any other reason, fails, the program will try to execute the func run_times non concurrently in the main process. Defaults to True.
 - `verbose` (bool, optional): Controls whether detailed information is printed after execution. Defaults to False.
 
 ## Contributing
 
 Contributions are welcome! Please follow these guidelines when contributing:
 
 1. Fork the repository.
```

### Comparing `tempit-0.1.1/setup.py` & `tempit-0.1.2/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from setuptools import setup
 
-VERSION = "0.1.1"
+VERSION = "0.1.2"
 setup(
     name="tempit",
     version=VERSION,
     author="mcrespoae",
     author_email="info@mariocrespo.es",
     packages=["tempit"],
     description="A dead simple time decorator",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/mcrespoae/tempit",
-    install_requires=[],
+    install_requires=["joblib"],
     python_requires=">=3.8",
-    keywords=["tempit", "time", "decorator", "performance", "multithreading", "benchmark"],
+    keywords=["tempit", "time", "decorator", "performance", "concurrency", "parallel", "benchmark"],
     classifiers=[
+        "Development Status :: 5 - Production/Stable",
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Intended Audience :: Developers",
     ],
 )
```

### Comparing `tempit-0.1.1/tempit/core.py` & `tempit-0.1.2/tempit/core.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,91 +1,77 @@
 import time
 from functools import partial, wraps
-from queue import Queue
 from typing import Any, Callable, Dict, List, Tuple
 
 from .utils import print_tempit_values
 
-CONCURRENCY_MODES_AVAILABLE = ["multithreading", "none"]
 
-
-def tempit(*args: Any, run_times: int = 1, concurrency_mode: str = "multithreading", verbose: bool = False) -> Callable:
+def tempit(*args: Any, run_times: int = 1, concurrent_execution: bool = True, verbose: bool = False) -> Callable:
     """
     Decorator function that measures the execution time of a given function. It can be called like @tempit or using arguments @tempit(...)
 
     Args:
         args: contains the function to be decorated if no arguments are provided when calling the decorator
         run_times (int, optional): The number of times the function should be executed. Defaults to 1.
-        concurrency_mode (str, optional): The concurrency mode to use for executing the function.
-            Possible values are "multithreading" and "none". Defaults to "multithreading".
+        concurrent_execution (bool, optional): This parameter will allow for the concurrent execution of the function using joblib.
+                                               The default execution backend is "loky" but if the function is being triggered other than the main thread or main process, the backend will be changed to multithreading.
+                                               If the execution of the concurrency fails, it will try to execute the func run_times non concurrently in the main process.
+                                               Defaults to True.
         verbose (bool, optional): Whether to print detailed information after execution. Defaults to False.
 
     Returns:
         Callable: The decorated function if arguments are provided, otherwise a partial function.
 
     Raises:
         RuntimeError: If the concurrency mode fails, the function is executed in the main process.
 
     Notes:
         - If `run_times` is less than 1, it will be set to 1.
-        - If `concurrency_mode` is not one of the available concurrency modes, it will be set to "multithreading".
         - If the function is a method, the first argument will be removed from `args_to_print`.
         - If the function is a class method, the first argument will be replaced with the class itself.
         - If the function is a static method, the first argument will be removed.
 
     Example:
-        @tempit(run_times=5, concurrency_mode="multithreading", verbose=True)
+        @tempit(run_times=5, concurrent_execution=True, verbose=True)
         def my_function(arg1, arg2):
             # function body
 
         @tempit
         def my_function(arg1, arg2):
             # function body
 
         # The decorated function can be used as usual
         result = my_function(arg1_value, arg2_value)
     """
 
     def decorator(
-        func: Callable, run_times: int = 1, concurrency_mode: str = "multithreading", verbose: bool = False
+        func: Callable, run_times: int = 1, concurrent_execution: bool = True, verbose: bool = False
     ) -> Callable:
         @wraps(func)
         def tempit_wrapper(*args: Tuple, **kwargs: Dict) -> Any:
-            validated_concurrency_mode = validate_concurrency_mode(concurrency_mode)
             callable_func, args, args_to_print = extract_callable_and_args_if_method(func, *args)
             result, total_times, real_time = function_execution(
                 callable_func,
                 run_times,
-                validated_concurrency_mode,
+                concurrent_execution,
                 *args,
                 **kwargs,
             )
 
             print_tempit_values(run_times, verbose, callable_func, total_times, real_time, *args_to_print, **kwargs)
 
             return result
 
         return tempit_wrapper
 
     if args:  # If arguments are not provided, return a decorator
-        return decorator(*args, run_times=run_times, concurrency_mode=concurrency_mode, verbose=verbose)
+        return decorator(*args, run_times=run_times, concurrent_execution=concurrent_execution, verbose=verbose)
 
     else:  # Otherwise, return a partial function
-        return partial(decorator, run_times=run_times, concurrency_mode=concurrency_mode, verbose=verbose)
-
-
-def validate_concurrency_mode(concurrency_mode: str) -> str:
-    """
-    Validates and normalizes the concurrency mode.
-    Args:
-        concurrency_mode (str): The concurrency mode to validate.
-    Returns:
-        str: The normalized concurrency mode if it is valid, otherwise "multithreading".
-    """
-    return concurrency_mode.lower() if concurrency_mode.lower() in CONCURRENCY_MODES_AVAILABLE else "multithreading"
+        return partial(decorator, run_times=run_times, concurrent_execution=concurrent_execution, verbose=verbose)
 
 
 def extract_callable_and_args_if_method(func, *args) -> Tuple[Callable, Tuple, Tuple]:
     """
     Extracts the callable function and arguments from a given function, if it is a method.
     Args:
         func (Callable): The function to extract the callable from.
@@ -108,15 +94,15 @@
         elif isinstance(func, staticmethod):
             args = args[1:]
 
     return callable_func, args, args_to_print
 
 
 def function_execution(
-    callable_func: Callable, run_times: int, concurrency_mode: str, *args: Tuple, **kwargs: Dict
+    callable_func: Callable, run_times: int, concurrent_execution: bool, *args: Tuple, **kwargs: Dict
 ) -> Tuple[Any, List[float], float]:
     """
     Run and measure the execution time of a function. It also returns the value of the function return and the execution times.
     Args:
         callable_func (Callable): The function to be executed.
         run_times (int): The number of times the function should be executed.
         concurrency_mode (str): The concurrency mode for executing the function.
@@ -125,18 +111,19 @@
     Returns:
         Tuple[Any, List[float], float]: A tuple containing the result of the function,
         a list of execution times for each run, and the total real time taken.
     """
     if run_times < 1:
         run_times = 1
     start_time = time.perf_counter()
-    if run_times > 1 and concurrency_mode != "none":
+    if run_times > 1 and concurrent_execution:
         try:
             result, total_times = tempit_with_concurrency(callable_func, run_times, *args, **kwargs)
-        except RuntimeError:
+        except RuntimeError as e:
+            print(e)
             result, total_times = tempit_main_process(callable_func, run_times, *args, **kwargs)
     else:
         result, total_times = tempit_main_process(callable_func, run_times, *args, **kwargs)
     end_time = time.perf_counter()
     real_time = end_time - start_time
 
     return result, total_times, real_time
@@ -164,56 +151,64 @@
         end_time: float = time.perf_counter()
         total_times.append(end_time - start_time)
     return result, total_times
 
 
 def tempit_with_concurrency(func: Callable, run_times: int, *args: Tuple, **kwargs: Dict) -> Tuple[Any, List[float]]:
     """
-    Executes a given function concurrently a specified number of times using a thread pool executor.
+    Executes a given function concurrently a specified number of times using joblib.
 
     Args:
         func (Callable): The function to be executed.
         run_times (int): The number of times the function should be executed.
         *args (Tuple): The positional arguments to be passed to the function.
         **kwargs (Dict): The keyword arguments to be passed to the function.
 
     Returns:
         Tuple[Any, List[float]]: A tuple containing the result of the function and a list of execution times for each run.
-        If an exception was raised in one of the threads, the function will raise a RuntimeError and execute the function
-        in the main process non-concurrently.
+        If an exception was raised in one of the concurrent tasks, the function will raise a RuntimeError and returns control
+        to the main process, then the function will be executed in the main process non-concurrently.
     """
-    from concurrent.futures import ThreadPoolExecutor
+
+    from multiprocessing import current_process
     from os import cpu_count
+    from threading import current_thread
 
-    workers: int = max(2, cpu_count() - 1) if cpu_count() is not None else 2  # type: ignore
+    from joblib import Parallel, delayed
 
     def run_func(
         func: Callable,
-        exception_queue: Queue,
         *args: Tuple,
         **kwargs: Dict,
-    ):
+    ) -> Tuple[Any, float, bool]:
+
+        has_crashed: bool = False
         start_time = time.perf_counter()
         try:
             result: Any = func(*args, **kwargs)
-        except Exception as e:
-            print(e)
-            exception_queue.put(e)
+        except Exception:
+            has_crashed = True
             result = None
         finally:
             end_time = time.perf_counter()
-            return result, end_time - start_time
+            return result, end_time - start_time, has_crashed
 
-    exception_queue: Queue = Queue()  # Queue for passing exceptions to the main thread
-    total_times: List[float] = []
-    with ThreadPoolExecutor(max_workers=workers) as executor:
-        future_tasks = [executor.submit(run_func, func, exception_queue, *args, **kwargs) for _ in range(run_times)]
+    joblib_backend = None  # Default backend for joblib
+    # Rule of thumb, use at least 2 workers or at least the number of cores minus 1.
+    # It is not ideal for multithreading, but it will make good balance
+    workers: int = max(2, cpu_count() - 1) if cpu_count() is not None else 2  # type: ignore
 
-    for future in future_tasks:
-        result, total_time = future.result()
-        total_times.append(total_time)
-    # If an exception was raised in one of the threads, execute the func in the main thread
-    if not exception_queue.empty():
+    if current_process().name != "MainProcess" or current_thread().name != "MainThread":
+        joblib_backend = "threading"  # If we are running in other than the main process or main thread, use threading instead of multiprocessing
+
+    results: List[Tuple[Any, float, bool]] = Parallel(n_jobs=workers, backend=joblib_backend)(
+        delayed(run_func)(func, *args, **kwargs) for _ in range(run_times)
+    )  # type: ignore
+
+    if any(has_crashed for _, _, has_crashed in results):
         raise RuntimeError(
             "An exception was raised in one of the concurrent jobs. Trying to execute in the main process non-concurrently."
         )
-    return result if result else None, total_times
+
+    total_times = [total_time for _, total_time, has_crashed in results if not has_crashed]
+    result = results[0][0]
+    return result, total_times
```

### Comparing `tempit-0.1.1/tempit/utils.py` & `tempit-0.1.2/tempit/utils.py`

 * *Files identical despite different names*

### Comparing `tempit-0.1.1/tempit.egg-info/PKG-INFO` & `tempit-0.1.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: tempit
-Version: 0.1.1
+Version: 0.1.2
 Summary: A dead simple time decorator
 Home-page: https://github.com/mcrespoae/tempit
 Author: mcrespoae
 Author-email: info@mariocrespo.es
-Keywords: tempit,time,decorator,performance,multithreading,benchmark
+Keywords: tempit,time,decorator,performance,concurrency,parallel,benchmark
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
+Requires-Dist: joblib
 
 # Tempit
 
 Tempit is a Python package designed to simplify the process of measuring the execution time of your functions through a straightforward decorator.
 
 ## Installation
 
@@ -49,15 +51,15 @@
 Function my_function took 10.5908ms.
 ```
 
 ### Advanced Usage
 
 ```python
 from tempit import tempit
-@tempit(run_times=20, concurrency_mode="multithreading", verbose=True)
+@tempit(run_times=20, concurrent_execution=True, verbose=True)
 def my_function_with_args(a:int = 1, b:int = 2):
     return a + b
 
 result = my_function_with_args(1, b=2)
 ```
 
 This will provide detailed output:
@@ -82,24 +84,24 @@
 More examples can be found in the [examples.py](examples/examples.py) script.
 
 ## Features
 
 - Simplified usage.
 - Accurate measurement of function execution time.
 - Support for `classmethod` and `staticmethods`.
-- Multithreading mode for performance measurement.
+- Parallel execution mode for performance measurement.
 - Human-readable time formatting.
 - Optional verbose mode for detailed information.
 
 ## Parameters
 
 Using the decorator @tempit without any parameters executes the function once and displays the execution time. However, you can enhance the experience using the following arguments:
 
 - `run_times` (int, optional): Specifies the number of function executions. Defaults to 1.
-- `concurrency_mode` (str, optional): Determines the concurrency mode for function execution. Options are "multithreading" and "none". Defaults to "multithreading".
+- `concurrency_mode` (bool, optional): Determines the concurrency mode for the function execution. It uses [joblib](https://pypi.org/project/joblib/) for parallel computing. The  default execution backend is "loky" but if the function is being triggered other than the main thread or main process, the backend will be changed to multithreading to aovid pickle errors. If, for any other reason, fails, the program will try to execute the func run_times non concurrently in the main process. Defaults to True.
 - `verbose` (bool, optional): Controls whether detailed information is printed after execution. Defaults to False.
 
 ## Contributing
 
 Contributions are welcome! Please follow these guidelines when contributing:
 
 1. Fork the repository.
```

### Comparing `tempit-0.1.1/tests/test_tempit.py` & `tempit-0.1.2/tests/test_tempit.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,43 +1,47 @@
+import os
 import threading
 import time
 import unittest
 from concurrent.futures import ProcessPoolExecutor, ThreadPoolExecutor
+from multiprocessing import current_process
 
 from tempit.core import tempit
 from tempit.utils import format_time
 
+IN_GITHUB_ACTIONS = os.getenv("GITHUB_ACTIONS") == "true"
+
 
 class TempitTestClass:
     @tempit()
     def tempit_basic(self):
         time.sleep(0.01)
 
     @tempit
     def tempit_basic_no_parenthesis(self):
         time.sleep(0.01)
 
     @tempit(run_times=5)
     def test_tempit_with_concurrency(self):
         time.sleep(0.01)
 
-    @tempit(run_times=5, concurrency_mode="none", verbose=False)
+    @tempit(run_times=5, concurrent_execution=False, verbose=False)
     def test_tempit_no_concurrency(self):
         time.sleep(0.01)
 
-    @tempit(run_times=5, concurrency_mode="multithreading", verbose=True)
+    @tempit(run_times=5, concurrent_execution=True, verbose=True)
     def test_tempit_concurrency_verbose(self):
         time.sleep(0.01)
 
-    @tempit(run_times=10, concurrency_mode="multithreading", verbose=True)
-    def test_tempit_multithreading_crash(self):
-        current_thread = threading.current_thread()
-        if current_thread.name != "MainThread":
-            raise RuntimeError("Crashing intentionally for testing multithreading inside a class")
-        time.sleep(0.01)
+    @tempit(run_times=10, concurrent_execution=True, verbose=True)
+    def test_tempit_thread_crash(self, a: int = 1, b: int = 2, thread_name: str = "ThreadPoolExecutor-"):
+        current_thread_name = threading.current_thread().name
+        if not current_thread_name.startswith(thread_name):
+            raise RuntimeError("Crashing intentionally for testing other process inside a class")
+        return a + b
 
     def sum(self, a: int = 1, b: int = 2):
         return a + b
 
     @tempit(run_times=10)
     def test_tempit_args(self, a: int = 1, b: int = 2):
         return self.sum(a, b)
@@ -48,187 +52,73 @@
         return a + b
 
     @tempit(run_times=2, verbose=True)
     @classmethod
     def class_method(cls, a: int = 1, b: int = 2):
         return cls.__name__, a + b
 
-    @tempit(run_times=2, verbose=True)
-    @classmethod
-    def class_method_no_args(cls):
-        return cls.__name__, 1 + 2
-
-
-class TestTempitDecoratorFunction(unittest.TestCase):
-
-    def test_tempit_basic(self):
-        @tempit()
-        def my_function():
-            time.sleep(0.01)
-
-        start_time = time.time()
-        my_function()
-        end_time = time.time()
-
-        execution_time = end_time - start_time
-        self.assertAlmostEqual(execution_time, 0.01, delta=0.1)
-
-    def test_tempit_basic_no_parenthesis(self):
-        @tempit
-        def my_function():
-            time.sleep(0.01)
-
-        start_time = time.time()
-        my_function()
-        end_time = time.time()
-
-        execution_time = end_time - start_time
-        self.assertAlmostEqual(execution_time, 0.01, delta=0.01)
-
-    def test_tempit_with_concurrency(self):
-        @tempit(run_times=5, concurrency_mode="multithreading")
-        def my_function():
-            time.sleep(0.01)
-
-        start_time = time.time()
-        my_function()
-        end_time = time.time()
-
-        execution_time = end_time - start_time
-        self.assertAlmostEqual(execution_time, 0.01, delta=0.1)  # Check if execution time is close to 0.1 seconds
-
-    def test_tempit_no_concurrency(self):
-        @tempit(run_times=5, concurrency_mode="none")
-        def my_function():
-            time.sleep(0.01)
-
-        start_time = time.time()
-        my_function()
-        end_time = time.time()
-
-        execution_time = end_time - start_time
-        self.assertAlmostEqual(execution_time, 0.05, delta=0.1)
-
-    def test_tempit_multithreading_verbose(self):
-        # Just check it doesn't crash
-        @tempit(run_times=5, concurrency_mode="multithreading", verbose=True)
-        def my_function():
-            time.sleep(0.01)
-
-        start_time = time.time()
-        my_function()
-        end_time = time.time()
-
-        execution_time = end_time - start_time
-        self.assertAlmostEqual(execution_time, 0.01, delta=0.1)
-
-    def test_tempit_multithreading_crash(self):
-        # Just check if it the multihreading doesn't work, it should be executed in the main thread
-        @tempit(run_times=5, concurrency_mode="multithreading")
-        def my_function():
-            current_thread = threading.current_thread()
-            if current_thread.name != "MainThread":
-                raise RuntimeError("Crashing intentionally for testing multithreading outside class")
-            time.sleep(0.01)
-
-        start_time = time.time()
-        my_function()
-        end_time = time.time()
-
-        execution_time = end_time - start_time
-        self.assertAlmostEqual(execution_time, 0.05, delta=0.1)
-
-    def test_tempit_args(self):
-        @tempit(run_times=2, concurrency_mode="multithreading", verbose=True)
-        def my_function(a: int = 1, b: int = 2):
-            return a + b
-
-        start_time = time.time()
-        result = my_function(1, b=2)
-        end_time = time.time()
-
-        execution_time = end_time - start_time
-        self.assertLess(execution_time, 0.05)
-        self.assertEqual(result, 3)
-
-    def test_run_from_other_thread(self):
-        @tempit(run_times=2, concurrency_mode="multithreading", verbose=True)
-        def my_function(a: int = 1, b: int = 2):
-            return a + b
-
-        with ThreadPoolExecutor(max_workers=1) as executor:
-            future = executor.submit(my_function, 2, b=4)
-            result = future.result()
-
-        self.assertEqual(result, 6)
-
-    def test_run_from_other_process(self):
-        with ProcessPoolExecutor(max_workers=1) as executor:
-            future = executor.submit(my_process_function, 1, b=2)
-            result = future.result()
-
-        self.assertEqual(result, 3)
-
 
 class TestTempitDecoratorClass(unittest.TestCase):
     def setUp(self):
         self.test_class = TempitTestClass()
 
     def test_tempit_basic(self):
 
-        start_time = time.time()
+        start_time = time.perf_counter()
         self.test_class.tempit_basic()
-        end_time = time.time()
+        end_time = time.perf_counter()
 
         execution_time = end_time - start_time
         self.assertAlmostEqual(execution_time, 0.01, delta=0.01)
 
     def test_tempit_basic_no_parenthesis(self):
 
-        start_time = time.time()
+        start_time = time.perf_counter()
         self.test_class.tempit_basic_no_parenthesis()
-        end_time = time.time()
+        end_time = time.perf_counter()
 
         execution_time = end_time - start_time
         self.assertAlmostEqual(execution_time, 0.01, delta=0.01)
 
     def test_tempit_with_concurrency(self):
 
-        start_time = time.time()
+        start_time = time.perf_counter()
         self.test_class.test_tempit_with_concurrency()
-        end_time = time.time()
+        end_time = time.perf_counter()
 
         execution_time = end_time - start_time
         self.assertAlmostEqual(execution_time, 0.01, delta=0.1)
 
     def test_tempit_no_concurrency(self):
-        start_time = time.time()
+        start_time = time.perf_counter()
         self.test_class.test_tempit_no_concurrency()
-        end_time = time.time()
+        end_time = time.perf_counter()
 
         execution_time = end_time - start_time
         self.assertAlmostEqual(execution_time, 0.05, delta=0.1)
 
     def test_tempit_concurrency_verbose(self):
         # Just check it doesn't crash
-        start_time = time.time()
+        start_time = time.perf_counter()
         self.test_class.test_tempit_concurrency_verbose()
-        end_time = time.time()
+        end_time = time.perf_counter()
 
         execution_time = end_time - start_time
         self.assertAlmostEqual(execution_time, 0.01, delta=0.1)
 
-    def test_tempit_multithreading_crash(self):
-        # Just check if it the multihreading doesn't work, it should be executed in the main thread
-        start_time = time.time()
-        self.test_class.test_tempit_concurrency_verbose()
-        end_time = time.time()
-
+    def test_tempit_other_thread_crash(self):
+        # Just check if it the parallel execution doesn't work, it should be executed in the main thread
+        start_time = time.perf_counter()
+        with ThreadPoolExecutor(max_workers=1) as executor:
+            future = executor.submit(self.test_class.test_tempit_thread_crash, 1, b=2)
+            result = future.result()
+        end_time = time.perf_counter()
         execution_time = end_time - start_time
         self.assertAlmostEqual(execution_time, 0.05, delta=0.1)
+        self.assertEqual(result, 3)
 
     def test_tempit_args(self):
         result = self.test_class.test_tempit_args(1, b=2)
         self.assertEqual(result, 3)
 
     def test_tempit_static_method(self):
         result = self.test_class.static_method(1, b=2)
@@ -280,16 +170,166 @@
         with ProcessPoolExecutor(max_workers=1) as executor:
             future = executor.submit(self.test_class.static_method, 1, b=2)
             result = future.result()
 
         self.assertEqual(result, 3)
 
 
+class TestTempitDecoratorFunction(unittest.TestCase):
+
+    def test_tempit_basic(self):
+        @tempit()
+        def my_function():
+            time.sleep(0.01)
+
+        start_time = time.perf_counter()
+        my_function()
+        end_time = time.perf_counter()
+
+        execution_time = end_time - start_time
+        self.assertAlmostEqual(execution_time, 0.01, delta=0.1)
+
+    def test_tempit_basic_no_parenthesis(self):
+        @tempit
+        def my_function():
+            time.sleep(0.01)
+
+        start_time = time.perf_counter()
+        my_function()
+        end_time = time.perf_counter()
+
+        execution_time = end_time - start_time
+        self.assertAlmostEqual(execution_time, 0.01, delta=0.01)
+
+    def test_tempit_with_concurrency(self):
+        @tempit(run_times=5, concurrent_execution=True)
+        def my_function():
+            time.sleep(0.01)
+
+        start_time = time.perf_counter()
+        my_function()
+        end_time = time.perf_counter()
+
+        execution_time = end_time - start_time
+        self.assertAlmostEqual(execution_time, 0.01, delta=0.1)  # Check if execution time is close to 0.1 seconds
+
+    def test_tempit_no_concurrency(self):
+        @tempit(run_times=5, concurrent_execution=False)
+        def my_function():
+            time.sleep(0.01)
+
+        start_time = time.perf_counter()
+        my_function()
+        end_time = time.perf_counter()
+
+        execution_time = end_time - start_time
+        self.assertAlmostEqual(execution_time, 0.05, delta=0.1)
+
+    def test_tempit_multithreading_verbose(self):
+        # Just check it doesn't crash
+        @tempit(run_times=5, concurrent_execution=True, verbose=True)
+        def my_function():
+            time.sleep(0.01)
+
+        start_time = time.perf_counter()
+        my_function()
+        end_time = time.perf_counter()
+
+        execution_time = end_time - start_time
+        self.assertAlmostEqual(execution_time, 0.01, delta=0.1)
+
+    def test_tempit_multithreading_crash(self):
+        # Just check if it the multihreading doesn't work, it should be executed in the main thread
+        @tempit(run_times=5, concurrent_execution=True)
+        def my_function():
+            current_thread_name = threading.current_thread().name
+            process_name = current_process().name
+            if current_thread_name != "MainThread" or process_name != "MainProcess":
+                raise RuntimeError("Crashing intentionally for testing multithreading outside class")
+            time.sleep(0.01)
+
+        start_time = time.perf_counter()
+        my_function()
+        end_time = time.perf_counter()
+
+        execution_time = end_time - start_time
+        self.assertLess(execution_time, 0.5)
+
+    def test_tempit_args(self):
+        @tempit(run_times=2, concurrent_execution=True, verbose=True)
+        def my_function(a: int = 1, b: int = 2):
+            return a + b
+
+        start_time = time.perf_counter()
+        result = my_function(1, b=2)
+        end_time = time.perf_counter()
+
+        execution_time = end_time - start_time
+        self.assertLess(execution_time, 0.05)
+        self.assertEqual(result, 3)
+
+    def test_run_from_other_thread(self):
+        @tempit(run_times=2, concurrent_execution=True, verbose=True)
+        def my_function(a: int = 1, b: int = 2):
+            return a + b
+
+        with ThreadPoolExecutor(max_workers=1) as executor:
+            future = executor.submit(my_function, 2, b=4)
+            result = future.result()
+
+        self.assertEqual(result, 6)
+
+    def test_run_from_other_process(self):
+        with ProcessPoolExecutor(max_workers=1) as executor:
+            future = executor.submit(my_process_function, 1, b=2)
+            result = future.result()
+
+        self.assertEqual(result, 3)
+
+    @unittest.skipUnless(not IN_GITHUB_ACTIONS, "Skip if running in GitHub Actions: too expensive.")
+    def test_tempit_long_running_function(self):
+        @tempit(run_times=4, concurrent_execution=True)
+        def my_concurrent_function(a=2_000_000, n=16):
+            for _ in range(a):
+                pass  #
+            return fib(n=n)
+
+        @tempit(run_times=4, concurrent_execution=False)
+        def my_sequential_function(a=2_000_000, n=16):
+            for _ in range(a):
+                pass  #
+            return fib(n=n)
+
+        start_time = time.perf_counter()
+        result_concurrent = my_concurrent_function(200_000_000, n=32)
+        end_time = time.perf_counter()
+        execution_time_concurrent = end_time - start_time
+
+        start_time = time.perf_counter()
+        result_sequential = my_sequential_function(200_000_000, n=32)
+        end_time = time.perf_counter()
+        execution_time_sequential = end_time - start_time
+
+        # self.assertGreaterEqual(execution_time_sequential, lower_bound)
+        self.assertLessEqual(
+            execution_time_concurrent, (execution_time_sequential / 4) + (execution_time_sequential * 0.1)
+        )
+
+        self.assertEqual(result_concurrent, 2178309)
+        self.assertEqual(result_sequential, 2178309)
+
+
+def fib(n):
+    if n < 2:
+        return n
+    return fib(n - 2) + fib(n - 1)
+
+
 # Added here since calling a function from another process inside a test method doesn't work
-@tempit(run_times=2, concurrency_mode="multithreading", verbose=True)
+@tempit(run_times=2, concurrent_execution=True, verbose=True)
 def my_process_function(a: int = 1, b: int = 2):
     return a + b
 
 
 class TestFormatTime(unittest.TestCase):
     def test_format_time_microseconds(self):
         self.assertEqual(format_time(0.0005), "500.0000µs")
```

